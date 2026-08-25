---
book: int
book_title: Integration
chapter: IX
chapter_title: MEASURES ON HAUSDORFF TOPOLOGICAL SPACES
section: 5
section_title: Measures on completely regular spaces
lang: vi
source: int-vii-ix
book_pages: INT IX.56-INT IX.72, INT IX.113-INT IX.117
pdf_pages: 0238-0254, 0295-0299
extraction: ocr
subsections:
    - "no": 1
      title: Measures and bounded continuous functions
      page: 56
      pdf_page: 238
    - "no": 2
      title: Bounded measures and linear forms on $\mathcal{C}^b(T)$
      page: 59
      pdf_page: 241
    - "no": 3
      title: Tight convergence of bounded measures
      page: 60
      pdf_page: 242
    - "no": 4
      title: 'Application: topological properties of the space $\mathcal{M}_+^b(T)$'
      page: 63
      pdf_page: 245
    - "no": 5
      title: Compactness criterion for tight convergence
      page: 64
      pdf_page: 246
    - "no": 6
      title: Tight convergence of measures and compact convergence of functions
      page: 67
      pdf_page: 249
    - "no": 7
      title: 'Application: the Laplace transformation'
      page: 68
      pdf_page: 250
statements: 33
exercises: 13
content_sha256: 8bae4b164451cbbec4ad5be76fea1b313cbfaffd513c53d5dd5fd429e8005915
translated_from: content/en/int/IX/05_s5_measures_on_completely_regular_spaces.md
source_content_sha256: 160d9c32a593ae0e84dcbc7a401963428f6758eb7ce0601b9dfaf2c7ddeb7626
translation_model: gpt-5.4-mini
translation_run: translate-vi-bb57bc71
glossary_version: 34
glossary_terms_sha256: 7a6de08a47ed83a43fe71b60fedf2e63e977a60672713fff28224808a92e3ab6
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 5. ĐỘ ĐO TRÊN CÁC KHÔNG GIAN HOÀN TOÀN CHÍNH QUY

Nếu T là một không gian tôpô, và F là một không gian Banach, ký hiệu $C^b(T; F)$ chỉ không gian các hàm liên tục bị chặn trên T nhận giá trị trong F, được trang bị chuẩn hội tụ đều. Nếu $F = \mathbf{R}$, ký hiệu này được viết tắt là $C^b(T)$, hoặc $C^b$ nếu không có nhập nhằng, và người ta ký hiệu bởi $C^b_+(T)$ hoặc $C^b_+$ nón các hàm dương trong $C^b(T)$. Không gian các độ đo phức bị chặn trên T sẽ được ký hiệu là $M^b(T; \mathbf{C})$, không gian các độ đo thực bị chặn bởi $M^b(T)$ hoặc $M^b$, và nón các độ đo dương bị chặn bởi $M^b_+(T)$ hoặc $M^b_+$.

### 1. Độ đo và các hàm liên tục bị chặn

Nhắc lại (GT, IX, §1, No. 5, Định nghĩa 4) rằng một không gian tôpô T được gọi là hoàn toàn chính quy nếu nó khả chuẩn hóa và Hausdorff. Điều này tương đương với nói rằng (loc. cit., Mệnh đề 3) T đồng phôi với một không gian con của một không gian compact. Nếu T hoàn toàn chính quy, thì mọi hàm số dương nửa liên tục dưới $f$ trên T là bao trên của tập có hướng tăng gồm các phần tử của $C^b_+(T)$ sao cho chúng $\leq f$, và mọi hàm số dương và bị chặn nửa liên tục trên $g$ là bao dưới của tập có hướng giảm gồm các phần tử của $C^b_+(T)$ sao cho chúng $\geq g$ (loc. cit., §1, No. 6, Mệnh đề 5). Ta sẽ cần bổ đề sau:

#### Bổ đề {#int-ix-s5-n1-lem-1 .statement}

Cho T là một không gian hoàn toàn chính quy, K là một tập con compact của T, và U là một tập con mở của T chứa K.
a) Tồn tại một tập con mở U' của T sao cho $K \subset U' \subset \overline{U'} \subset U$.
b) Cho f là một hàm liên tục xác định trên K nhận giá trị trong một khoảng I của $\mathbf{R}$ (resp. trong $\mathbf{C}$). Tồn tại một hàm liên tục bị chặn $f'$ trên T, nhận giá trị trong I (resp. trong $\mathbf{C}$), mở rộng f và bằng không trên $T - U$.

Chỉ cần xét trường hợp T là một không gian con của một không gian compact X. Cho V là một tập con mở của X sao cho $V \cap T = U$; ký hiệu V' là một tập mở trong X chứa K sao cho $\overline{V'} \subset V$, ký hiệu g là một hàm liên tục trên X nhận giá trị trong I (resp. trong $\mathbf{C}$) mở rộng f và bằng không trên $X - V$ (GT, IX, §4, No. 1, Mệnh đề 1). Điều kiện a) được thỏa mãn bằng cách lấy $U' = V' \cap T$, và b) bằng cách lấy $f'$ là hạn chế của g lên T.

#### Mệnh đề 1 {#int-ix-s5-prop-1 .statement}

— Cho T là một không gian hoàn toàn chính quy.
a) Cho $\mu$ là một độ đo dương trên T, và f là một hàm số $\geq 0$ xác định trên T và nửa liên tục dưới (resp. nửa liên tục trên, hữu hạn, có giá compact). Khi đó

(1) $\mu^\bullet(f) = \sup_{g \in I_f} \mu^\bullet(g)$ (resp. $\mu^\bullet(f) = \inf_{g \in S_f} \mu(g)$),

trong đó $I_f$ (resp. $S_f$) chỉ tập hợp các hàm liên tục bị chặn $g$ sao cho $0 \leq g \leq f$ (resp. $g \geq f$).

b) Cho $\theta$ là một độ đo phức trên $T$, và f là một hàm số $\geq 0$ xác định trên T và nửa liên tục dưới. Khi đó

(2) $|\theta|^\bullet(f) = \sup_g |\theta(g)|$,

trong đó g chạy qua tập các hàm phức liên tục bị chặn và khả tích theo $|\theta|$ sao cho $|g| \leq f$.

Công thức thứ nhất trong (1) là hiển nhiên, vì $I_f$ là một tập có hướng tăng các hàm liên tục có bao trên là $f$, và có thể áp dụng Mệnh đề 5 của §1, No. 6. Mệnh đề ấy cũng sẽ suy ra công thức thứ hai, nếu ta chứng minh rằng $S_f$ chứa một hàm liên tục bị chặn, $\mu$-khả tích. Vì vậy, cho $K$ là giá đỡ của $f$, và $M$ là cận trên đúng của $f$; vì $K$ là compact, nên $M$ là hữu hạn (GT, IV, §6, No. 2, Th. 3). Cho $U$ là một tập mở chứa $K$ và sao cho $\mu^\bullet(U) < +\infty$; tồn tại (Bổ đề) một hàm liên tục $g$ nhận giá trị trong $[0, M]$, bằng $M$ trên $K$ và bằng không ngoài $U$; khi đó $g \in S_f$ và $\mu^\bullet(g) \leq M \mu^\bullet(U) < +\infty$.

Chuyển sang b). Rõ ràng chỉ cần chứng minh rằng $|\theta|^\bullet(f) \leq \sup_g |\theta(g)|$.

Cho $a$ và $b$ là hai số thực sao cho $a < b < |\theta|^\bullet(f)$. Theo (1), tồn tại một hàm $h \in \mathcal{C}_+^b(T)$ sao cho $h \leq f$ và $|\theta|^\bullet(h) > b$; ký hiệu $M$ là cận trên đúng của $h$. Theo định nghĩa của $|\theta|^\bullet$ (§1, No. 2, Định nghĩa 4), tồn tại một tập con compact $K$ của $T$ sao cho $|\theta|_K^\bullet(h_K) > b$. Khi đó tồn tại một hàm phức liên tục $j$ trên $K$ sao cho $|j| \leq h_K$ và $|\theta_K(j)| > b$ (Ch. III, §1, No. 6). Chọn một tập mở $U$ chứa $K$ và sao cho $|\theta|^\bullet(U - K) \leq \frac{b - a}{M}$ (§1, No. 9, Mệnh đề 13 và 14); mở rộng $j$ thành một hàm phức liên tục $k$ trên $T$, bằng không ngoài $U$ (Bổ đề); với mọi $t \in T$, đặt

(3)
$$
g(t) = \begin{cases}
k(t) & \text{nếu } |k(t)| \leq h(t) \\
\frac{k(t)}{|k(t)|} h(t) & \text{nếu } |k(t)| > h(t)
\end{cases}
$$

Rõ ràng $|g| \leq h \leq f$, và $g = j$ trên $K$, do đó $||\theta_K(j)| - |\theta(g)|| = ||\theta(j^0)| - |\theta(g)|| \leq |\theta|^\bullet(|j^0 - g|) \leq M \cdot |\theta|^\bullet(U - K) \leq b - a$, suy ra $|\theta(g)| > a$. Mặt khác, ta hãy chứng minh rằng $g$ là một hàm liên tục:

vì $a$ chỉ thỏa mãn điều kiện duy nhất $a < |\theta|^*(f)$, điều này sẽ suy ra rằng vế thứ hai của (2) là $\geqslant$ vế thứ nhất, do đó mệnh đề. Bây giờ, cho $F$ (resp. $F'$) là tập hợp các $t \in T$ sao cho $|k(t)| \leq h(t)$ (resp. $|k(t)| \geq h(t)$). Vì các tập hợp này đóng, và hợp của chúng là $T$, chỉ cần chỉ ra rằng $g_F$ và $g_{F'}$ liên tục: giờ đây, tính chất này hiển nhiên đối với $g_F = k_F$, và cũng đúng đối với $g_{F'}$ tại các điểm mà $k(t) \neq 0$; mặt khác, nếu $t \in F'$ sao cho $k(t) = 0$, thì cũng có $h(t) = 0$, và bất đẳng thức $|g| \leq h$ suy ra rằng $g$ liên tục tại điểm $t$.

#### Nhận xét 1 {#int-ix-s5-n1-rem-1 .statement}

Cho $f$ là một hàm nửa liên tục dưới dương, và cho $J_f$ là tập hợp các hàm liên tục bị chặn dương bằng không ngoài một tập mở khả tích theo $\mu$ và bị chặn trên bởi $f$. Có thể chứng minh rằng $f$ là bao trên của $J_f$ và rằng $\mu^*(f) = \sup_{g \in J_f} \mu(g)$.

#### Nhận xét 2 {#int-ix-s5-n1-rem-2 .statement}

Nếu độ đo $\mu$ bị chặn, công thức $\mu^*(f) = \inf_{g \in S_f} \mu(g)$ hiển nhiên đúng với mọi hàm $f$ nửa liên tục trên, dương và bị chặn.

#### Mệnh đề 2 {#int-ix-s5-prop-2 .statement}

— *Cho $\eta$ và $\eta'$ là hai độ đo phức trên một không gian hoàn toàn chính quy $T$, sao cho $\eta(f) = \eta'(f)$ với mọi hàm $f \in \mathcal{C}^b(T)$ khả tích đối với $|\eta|$ và $|\eta'|$. Khi đó $\eta = \eta'$. \*

Ta hãy xét lại chứng minh của phần thứ hai của Mệnh đề 1, bằng cách đặt $\theta = \eta - \eta'$. Ta có thể yêu cầu tập mở U khả tích đối với $|\eta|$ và $|\eta'|$. Khi đó hàm $g$ khả tích đối với hai độ đo này, và quan hệ $\theta(g) = 0$ suy ra $a < 0$; do đó $|\theta|^*(f) = 0$ với mọi hàm nửa liên tục dưới dương $f$, do đó cuối cùng $|\theta| = 0$, khi lấy $f = +\infty$.

#### Mệnh đề 3 {#int-ix-s5-prop-3 .statement}

— *Cho $\mu$ là một độ đo dương trên một không gian hoàn toàn chính quy $T$, và cho $p \in [1, +\infty[$. Không gian $\mathcal{H}$ gồm các hàm $f \in \mathcal{C}^b(T)$, có giá đỡ được chứa trong một tập mở khả tích theo $\mu$, là trù mật trong $\mathcal{L}^p(\mu)$. \*

Theo Mệnh đề 15 của §1, No. 10, đủ để chỉ ra rằng nếu K là compact trong T, và nếu $g$ là mở rộng lên T bằng 0 của một hàm trong $\mathcal{C}_+(K)$ giữa 0 và 1, thì tồn tại một hàm $f \in \mathcal{C}_+^b(T)$, với giá đỡ được chứa trong một tập mở khả tích theo $\mu$, sao cho $\|f - g\|_p$ tùy ý nhỏ. Bây giờ, hãy lấy $\varepsilon$ là một số $> 0$, U là một lân cận mở của K sao cho $\mu^*(U - K) < \varepsilon$, V là một lân cận mở của K sao cho $\overline{V} \subset U$, và $f$ là một hàm có giá trị trong $[0, 1]$, liên tục, bằng $g$ trên K và bằng 0 ngoài V (Bổ đề). Khi đó hàm $|f - g|^p$ được chặn trên bởi $\varphi_{U-K}$; do đó $\|f - g\|_p \leq \varepsilon^{1/p}$, điều này chứng minh mệnh đề.

*Nhận xét 3).* — Có một mệnh đề tương tự cho các hàm nhận giá trị trong một không gian Banach F: không gian con $\mathcal{H} \otimes F$ của $\mathcal{C}^b(T; F)$ là trù mật trong $\mathcal{L}_F^p(\mu)$.

#### Mệnh đề 4 {#int-ix-s5-prop-4 .statement}

— *Để một độ đo phức bị chặn $\theta$ trên một không gian hoàn toàn chính quy T là dương, cần và đủ rằng $\theta(f) \geq 0$ với mọi hàm $f \in \mathcal{C}_+^b(T)$.*

Điều kiện cần là hiển nhiên. Để chứng minh tính đủ, ta xét lại chứng minh của mệnh đề trước, với $p = 1$ và $\mu = |\theta|$; các ký hiệu giữ nguyên, quan hệ $\mu^*(|f - g|) \leq \varepsilon$ và bất đẳng thức $\theta(f) \geq 0$ kéo theo $\theta_K(g_K) = \theta(g) \geq -\varepsilon$; vì $g_K$ là một phần tử tùy ý của $\mathcal{C}(K)$ giữa 0 và 1, nên độ đo $\theta_K$ là dương; do K là tùy ý, điều đó có nghĩa là $\theta$ là dương.

### 2. Các độ đo bị chặn và các dạng tuyến tính trên $\mathcal{C}^b(T)$

#### Mệnh đề 5 {#int-ix-s5-prop-5 .statement}

— *Cho T là một không gian hoàn toàn chính quy, và I là một dạng tuyến tính phức liên tục trên không gian chuẩn $\mathcal{C}^b(T; \mathbf{C})$. Để tồn tại một độ đo phức bị chặn $\theta$ trên T sao cho $\theta(f) = I(f)$ với mọi $f \in \mathcal{C}^b(T; \mathbf{C})$, cần và đủ rằng điều kiện sau được thỏa mãn:

(M) *Với mọi số $\varepsilon > 0$, tồn tại một tập con compact K của T sao cho các quan hệ $g \in \mathcal{C}^b(T; \mathbf{C}), |g| \leq 1, g_K = 0$ kéo theo $|I(g)| \leq \varepsilon$.

Khi đó độ đo $\theta$ là duy nhất.*

Tính duy nhất suy ra từ Mệnh đề 2 của No. 1. Ta hãy chứng minh rằng điều kiện (M) là cần. Cho $\theta$ là một độ đo phức bị chặn; lấy K là một tập compact sao cho $|\theta|^*(T - K) \leq \varepsilon$ (§1, No. 2, *Nhận xét 3*). Các giả thiết $|g| \leq 1, g_K = 0$ kéo theo $|g| \leq \varphi_{\mathbf{C}_K}$, do đó $|\theta(g)| \leq |\theta|^*(\varphi_{\mathbf{C}_K}) \leq \varepsilon$.

Ta chuyển sang chứng minh tính đủ. Cho X là compact hóa Stone–Čech của T (GT, IX, §1, Bài tập 7; hoặc TG, IX, §1, No. 6). Với mọi hàm $f \in \mathcal{C}(X; \mathbf{C})$, đặt $\nu(f) = I(f_T)$; theo cách này ta định nghĩa một dạng tuyến tính liên tục trên $\mathcal{C}(X; \mathbf{C})$, tức là một độ đo phức trên không gian compact X. Cho $\varepsilon$ là một số $> 0$, K là một tập compact thỏa mãn (M); vì hàm $\varphi_{\mathbf{C}_K}$ là nửa liên tục dưới và dương trên X, công thức (2) cho ta các quan hệ sau, trong đó $\mathcal{G}$ ký hiệu tập các hàm $g \in \mathcal{C}(X; \mathbf{C})$ sao cho $|g| \leq \varphi_{\mathbf{C}_K}$:

$$
|\nu|^*(X - K) = \sup_{g \in \mathcal{G}} |\nu(g)| = \sup_{g \in \mathcal{G}} |I(g_T)| \leq \varepsilon.
$$

Cho $(K_n)_{n \geq 1}$ là một dãy các tập con compact của $T$, sao cho mỗi $K_n$ thỏa mãn (M) với $\varepsilon = 1/n$, và đặt $S = \bigcup K_n$; $S$ là một tập Borel trong $X$, được chứa trong $T$, và $|\nu|^*(X - T) \leq |\nu|^*(X - S) \leq |\nu|^*(X - K_n) \leq 1/n$ với mọi $n$, do đó $T$ khả đo với $\nu$ và $\nu$ tập trung trên $T$. Cho $f$ là một hàm liên tục bị chặn trên $T$; vì $X$ là compact hóa Stone–Čech của $T$, $f$ có thể được mở rộng liên tục thành một hàm $g \in \mathcal{C}(X; \mathbf{C})$. Bây giờ cho $\mu$ là độ đo cảm sinh bởi $\nu$ trên $T$; ta có $\mu(f) = \nu(f^0)$. (1) Vì $\nu$ tập trung trên $T$, các hàm $f^0$ và $g$ bằng nhau $\nu$-hầu khắp, do đó $\mu(f) = \nu(g) = I(g_T) = I(f)$, và điều đó hoàn tất chứng minh.

#### Hệ quả {#int-ix-s5-n2-cor-1 .statement}

— *Với các ký hiệu như trong Mệnh đề 5, giả sử tồn tại một độ đo dương bị chặn $\mu$ trên $T$ sao cho $|I(f)| \leq \mu(|f|)$ với mọi $f \in \mathcal{C}^b(T; \mathbf{C})$; khi đó tồn tại một độ đo phức $\theta$ trên $T$ sao cho $\theta(f) = I(f)$ với mọi $f \in \mathcal{C}^b(T; \mathbf{C})$.

### 3. Sự hội tụ chặt của các độ đo bị chặn

Cho $T$ là một không gian chính quy hoàn toàn; dạng song tuyến tính
$$
(f, \mu) \mapsto \int f(t) \, d\mu(t)
$$
trên $\mathcal{C}^b(T) \times \mathcal{M}^b(T)$ đặt hai không gian này vào một tính đối ngẫu phân biệt. Thật vậy, điều đó rõ ràng là tính đối ngẫu phân biệt trên $\mathcal{C}^b(T)$ từ thực tế rằng các độ đo $\varepsilon_x \ (x \in T)$ thuộc $\mathcal{M}^b(T)$; nó là phân biệt trên $\mathcal{M}^b(T)$ theo Mệnh đề 2 của No. 1.

#### Định nghĩa 1 {#int-ix-s5-def-1 .statement}

*Tôpô yếu trên $\mathcal{M}^b(T)$, được liên kết với tính đối ngẫu nói trên giữa $\mathcal{C}^b(T)$ và $\mathcal{M}^b(T)$, được gọi là tôpô của sự hội tụ chặt (hay tôpô chặt) trên $\mathcal{M}^b(T)$. \*

Tôpô chặt là Hausdorff, theo các nhận xét trước định nghĩa. Chúng ta sẽ thường dùng trạng từ 'chặt' để chỉ 'theo nghĩa của tôpô chặt'. Trừ khi có nói khác, $\mathcal{M}^b(T)$ sẽ được trang bị tôpô chặt trong suốt phần còn lại của mục này.

Mọi phần tử của $\mathcal{C}^b(T)$ là một tổ hợp tuyến tính của các phần tử của $\mathcal{C}_+^b(T)$. Để một bộ lọc $\mathfrak{F}$ trên $\mathcal{M}^b(T)$ hội tụ chặt đến một độ đo bị chặn $\lambda$, cần và đủ rằng
$$
\lim_{\mu} \mu(f) = \lambda(f) \quad \text{đối với } \mathfrak{F} \text{ với mọi } f \in \mathcal{C}_+^b(T).
$$

#### Nhận xét 1 {#int-ix-s5-n3-rem-1 .statement}

Nếu $T$ là địa phương compact, tôpô chặt mịn hơn tôpô cảm sinh trên $\mathcal{M}^b(T)$ bởi tôpô vague, và hai tôpô này chỉ trùng nhau khi $T$ là compact. Thật vậy, nếu $T$ không compact, ánh xạ $t \mapsto \varepsilon_t$ hội tụ vague đến 0 đối với bộ lọc của các phần bù của các tập con tương đối compact của $T$, nhưng không hội tụ chặt đến 0, vì hàm 1 thuộc $\mathcal{C}^b(T)$ (về các quan hệ giữa hội tụ vague và hội tụ chặt, xem Mệnh đề 9).

(1) Quan hệ này chỉ mới được thiết lập ở trên (\S 2, No. 1, Mệnh đề 1) trong trường hợp $f$ và $\nu$ là dương. Mở rộng sang tình huống hiện tại, trong đó $f$ và $\nu$ là phức và bị chặn, là ngay lập tức theo tính tuyến tính.

#### Nhận xét 2 {#int-ix-s5-n3-rem-2 .statement}

Suy ra ngay lập tức từ Mệnh đề 4 rằng $\mathcal{M}_+^b(T)$ là đóng trong $\mathcal{M}^b(T)$.

#### Nhận xét 3 {#int-ix-s5-n3-rem-3 .statement}

Nếu T hoàn toàn chính quy, thì ánh xạ $t \mapsto \varepsilon_t$ của T vào $\mathcal{M}^b(T)$ là một đồng phôi (GT, IX, §1, No. 5).

#### Mệnh đề 6 {#int-ix-s5-prop-6 .statement}

— Cho T là một không gian hoàn toàn chính quy.

a) Cho f là một hàm số dưới nửa liên tục, nhận giá trị số, $\geqslant 0$, được xác định trên T; khi đó hàm $\mu \mapsto |\mu|^*(f)$ là dưới nửa liên tục trên $\mathcal{M}^b(T)$.

b) Cho f là một hàm bị chặn trên nửa liên tục, được xác định trên T; khi đó hàm $\mu \mapsto \mu(f)$ là trên nửa liên tục trên $\mathcal{M}_+^b(T)$.

Vì, ta thấy theo Mệnh đề 1 b) của No. 1 rằng $\mu \mapsto |\mu|^*(f)$ là bao trên của một họ các hàm có dạng $\mu \mapsto |\mu(g)|$ với $g \in \mathcal{C}^b(T)$, do đó liên tục đối với tôpô chặt. Điều này thiết lập a). Để chứng minh b), chỉ cần chọn một cận trên hằng C cho f, và viết $\mu(f) = \mu(C) - \mu(C - f)$; hàm $\mu \mapsto \mu(C)$ là liên tục, và hàm $\mu \mapsto \mu(C - f)$ là dưới nửa liên tục trên $\mathcal{M}_+^b(T)$ theo điều trên.

#### Mệnh đề 7 {#int-ix-s5-prop-7 .statement}

— Cho T là một không gian hoàn toàn chính quy. Cho $\mu$ là một độ đo dương bị chặn trên T, và cho f là một hàm dương bị chặn trên T, sao cho tập hợp các điểm của T tại đó f không liên tục là địa phương \mu-không đáng kể. Khi đó ánh xạ $\lambda \mapsto \lambda^*(f)$ của $\mathcal{M}_+^b(T)$ vào $\mathbf{R}$ là liên tục tại điểm $\mu$.

Với mọi $t \in T$, đặt $f'(t) = \liminf_{s \to t} f(s)$, $f''(t) = \limsup_{s \to t} f(s)$. Hiển nhiên $f' \leqslant f \leqslant f''$, với đẳng thức tại mọi điểm của T nơi f liên tục (do đó hầu khắp theo $\mu$). Mặt khác, $f'$ là dưới nửa liên tục, $f''$ là trên nửa liên tục và bị chặn (GT, IV, §6, No. 2, Prop. 4). Vì thế ta có các quan hệ sau theo Mệnh đề 6,

$$
\mu^*(f') \leqslant \liminf_{\lambda \to \mu} \lambda^*(f') \leqslant \liminf_{\lambda \to \mu} \lambda^*(f) \leqslant \mu^*(f) \leqslant \limsup_{\lambda \to \mu} \lambda^*(f)
$$
$$
\leqslant \limsup_{\lambda \to \mu} \lambda^*(f'') \leqslant \mu^*(f'').
$$

Suy ra bằng cách nhận thấy rằng $\mu^*(f') = \mu^*(f'')$, vì $f'$ và $f''$ bằng nhau địa phương hầu khắp theo $\mu$.

#### Mệnh đề 8 {#int-ix-s5-prop-8 .statement}

— Cho X là một không gian hoàn toàn chính quy, T là một không gian con của X, và i là đơn ánh chính tắc của T vào X. Ký hiệu W là tập hợp các độ đo dương bị chặn trên X tập trung trên T, được trang bị tôpô cảm sinh bởi $\mathcal{M}^b(X)$. Khi đó ánh xạ $\mu \mapsto i(\mu)$ của $\mathcal{M}_+^b(T)$ vào $\mathcal{M}^b(X)$ là một đồng phôi của $\mathcal{M}_+^b(T)$ lên W.

Ta lại ký hiệu i là ánh xạ $\mu \mapsto i(\mu)$ của $\mathcal{M}_+^b(T)$ vào $\mathcal{M}_+^b(X)$; i là đơn ánh (§2, No. 4, Prop. 8) và gửi $\mathcal{M}_+^b(T)$ vào W (§2, No. 3, Prop. 7). Nếu $\lambda \in W$, thì $\lambda = i(\lambda_T)$ (§2, No. 3, Prop. 7 b)). Do đó, i là một song ánh của $\mathcal{M}_+^b(T)$ lên W, và song ánh ngược của i là ánh xạ $r : \lambda \mapsto \lambda_T$ trên W. Mặt khác, $i$ là liên tục: vì, nếu $f \in \mathcal{C}^b(X)$, thì $\langle i(\mu), f \rangle = \langle \mu, f \circ i \rangle$, và $f \circ i$ thuộc $\mathcal{C}^b(T)$. Do đó, mọi sự quy về việc chứng minh rằng, với mọi độ đo $\mu \in W$ và mọi hàm $f \in \mathcal{C}^b_+(T)$, ta có

$$
\lim_{\lambda \to \mu, \lambda \in W} \lambda_T(f) = \mu_T(f),
$$

hay lại nữa

$$
\lim_{\lambda \to \mu, \lambda \in W} \lambda(f^0) = \mu(f^0).
$$

Cho $f^\infty$ là hàm trên $X$ trùng với $f$ trên $T$ và bằng $+\infty$ trên $X - T$, và cho $f'$ và $f''$ lần lượt là sự chính quy hóa nửa liên tục trên của $f^0$ và sự chính quy hóa nửa liên tục dưới của $f^\infty$ (GT, IV, §6, No. 2). Các quan hệ

$$
f'(x) = \limsup_{y \to x} f^0(y), \quad f''(x) = \liminf_{y \to x} f^\infty(y)
$$

ngay lập tức suy ra rằng $f'$ và $f''$ đều trùng với $f$ và $f^0$ trên $T$. Mệnh đề 6 khi đó dẫn tới

$$
\mu^\bullet(f') \geq \limsup_{\lambda \to \mu, \lambda \in W} \lambda^\bullet(f'), \quad \mu^\bullet(f'') \leq \liminf_{\lambda \to \mu, \lambda \in W} \lambda^\bullet(f'').
$$

Nhưng ta có thể thay $f'$ và $f''$ bởi $f^0$ trong hai công thức này, vì các độ đo $\lambda$ và $\mu$ được mang bởi $T$; do đó ta đã thu được quan hệ mong muốn.

Mệnh đề của Mệnh đề 8 chỉ đúng cho các độ đo dương: ánh xạ $\mu \mapsto i(\mu)$ của $\mathcal{M}^b(T)$ vào $\mathcal{M}^b(X)$ là đơn ánh và liên tục, nhưng nói chung không phải là một đồng phôi từ $\mathcal{M}^b(T)$ onto ảnh của nó. Chẳng hạn, lấy $X = \mathbf{R}$, $T = \mathbf{R} - \{0\}$; các độ đo $\lambda_t = \varepsilon_t - \varepsilon_{-t}$ ($t > 0$) hội tụ chặt về $0$ trong $X$ khi $t$ tiến tới $0$, nhưng không hội tụ chặt về $0$ trong $T$ (hàm đặc trưng của $]0, +\infty[$ thuộc $\mathcal{C}^b(T)$) (cf. tuy nhiên Hệ quả của Định lý 1 của No. 5).

#### Mệnh đề 9 {#int-ix-s5-prop-9 .statement}

— *Cho T là một không gian địa phương compact, và cho $\mathfrak{F}$ là một bộ lọc trên $\mathcal{M}^b_+(T)$ hội tụ mơ hồ về một độ đo bị chặn $\mu$. Để $\mathfrak{F}$ hội tụ chặt về $\mu$, điều kiện cần và đủ là $\lim_{\lambda} \lambda(1) = \mu(1)$ đối với $\mathfrak{F}$.*

Điều kiện này hiển nhiên là cần. Để chứng minh rằng nó đủ, ta ký hiệu $X$ là sự compact hóa Alexandroff của $T$ (GT, I, §9, No. 8) và ký hiệu $i$ là đơn ánh chính tắc của $T$ vào $X$. Theo Mệnh đề 8, mọi việc quy về việc chứng minh rằng $\lambda \mapsto i(\lambda)$ hội tụ chặt về $i(\mu)$ trong $\mathcal{M}^b(X)$ đối với $\mathfrak{F}$. Vì $\mu(1) < +\infty$, tồn tại một tập $A \in \mathfrak{F}$ sao cho tổng số khối lượng của các độ đo trong $A$ bị chặn bởi một số $M$; do đó chỉ cần kiểm tra rằng

$$
\lim_{\lambda, \mathfrak{F}} \int_X g \, d(i(\lambda)) = \int_X g \, d(i(\mu))
$$

đối với các hàm $g \in \mathcal{C}^b(X)$ tạo thành một tập hợp toàn phần trong $\mathcal{C}^b(X)$.

Hiện nay, đẳng thức này được thỏa mãn khi $g$ có giá compact trong $T$, do sự hội tụ vague của $\mathfrak{F}$ đến $\mu$, và cũng khi $g$ là một hàm hằng trên $X$, từ thực tế rằng $\lim_{\lambda, \mathfrak{F}} \lambda(1) = \mu(1)$. Vì các hàm thuộc hai kiểu trên tạo thành một tập hợp toàn phần trong $\mathcal{C}^b(X)$ (Ch. III, §1, No. 2, Mệnh đề 3), điều này hoàn tất chứng minh.

### 4. Ứng dụng: các tính chất tôpô của không gian $\mathcal{M}_+^b(T)$

Trước hết nhận thấy rằng nếu $T$ là một không gian chính quy hoàn toàn, thì $\mathcal{M}^b(T)$ là một không gian vectơ tôpô Hausdorff, do đó là chính quy hoàn toàn. Suy ra, $\mathcal{M}_+^b(T)$ là chính quy hoàn toàn.

#### Mệnh đề 10 {#int-ix-s5-prop-10 .statement}

*Cho $T$ là một không gian Polish; khi đó không gian $\mathcal{M}_+^b(T)$ là Polish đối với tôpô chặt.*

Ta bắt đầu bằng trường hợp $T$ là Polish và *compact*. Khi đó tập $U$ của các độ đo dương có khối lượng $\leq 1$ là compact (Ch. III, §1, No. 9, Hệ quả 2 của Mệnh đề 15), và tôpô cảm sinh trên $U$ bởi tôpô chặt (mà ở đây trùng với tôpô vague) cũng là tôpô cảm sinh bởi tôpô hội tụ từng điểm trên một tập hợp toàn phần của $\mathcal{C}(T)$ (*loc. cit.*, No. 10, Mệnh đề 17). Hiện nay, trong $\mathcal{C}(T)$ tồn tại một tập hợp toàn phần đếm được (GT, X, §3, No. 3, Định lý 1); do đó, $U$ là một không gian compact mêtrizable. Tập $V$ của các độ đo dương có khối lượng $< 1$ là mở trong $U$, do đó là một không gian Polish địa phương compact. Khi đó, ánh xạ $\mu \mapsto \frac{1}{1 + \mu(1)} \mu$ của $\mathcal{M}_+^b(T)$ lên $V$ là một đẳng cấu tôpô, với ánh xạ $\lambda \mapsto \frac{1}{1 - \lambda(1)} \lambda$ là đẳng cấu tôpô nghịch đảo.

Ta xét trường hợp $T$ là Polish; có thể giả sử rằng $T$ là giao của một dãy giảm $(G_n)$ các tập mở trong một không gian compact mêtrizable $X$ (GT, IX, §6, No. 1, Hệ quả 1 của Định lý 1); khi đó không gian $\mathcal{M}_+^b(T)$ đẳng cấu tôpô với không gian con $W$ của $\mathcal{M}_+^b(X)$ gồm các độ đo tập trung trên $T$ (No. 3, Mệnh đề 8), và chỉ cần chứng minh rằng $W$ là giao của một dãy các tập mở trong không gian Polish $\mathcal{M}_+^b(X)$ (GT, *loc. cit.*, Định lý 1). Bây giờ, ký hiệu $W_n$ là tập các độ đo $\mu \in \mathcal{M}_+^b(X)$ tập trung trên $G_n$; ánh xạ $h_n : \mu \mapsto \mu^*(X - G_n)$ trên $\mathcal{M}_+^b(X)$ là nửa liên tục trên (No. 3, Mệnh đề 6), và tập $A_k^n$ gồm các độ đo $\mu \in \mathcal{M}_+^b(X)$ sao cho $h_n(\mu) < 1/k$ do đó là mở với mọi $k \geq 1$ và mọi $n \in \mathbf{N}$. Chứng minh được hoàn tất bằng cách nhận thấy rằng $W = \bigcap_n W_n = \bigcap_{n,k} A_k^n$.

#### Hệ quả 1 {#int-ix-s5-prop-10-cor-1 .statement}

*Nếu T là một không gian mêtrizable kiểu đếm được, thì $\mathcal{M}_+^b(T)$ là mêtrizable kiểu đếm được đối với tôpô chặt.*

Thật vậy, cho $\hat{T}$ là bao đầy đủ của T đối với một metric xác định tôpô của T; không gian $\hat{T}$ là Polish, và $\mathcal{M}_+^b(T)$ đẳng cấu tôpô với không gian con của không gian Polish $\mathcal{M}_+^b(\hat{T})$ gồm các độ đo tập trung trên T (No. 3, Mệnh đề 8). Nhưng mọi không gian con của một không gian Polish đều mêtrizable kiểu đếm được (GT, IX, §2, No. 8).

#### Hệ quả 2 {#int-ix-s5-prop-10-cor-2 .statement}

*Nếu T là một không gian Souslin (tương ứng Lusin) chính quy hoàn toàn, thì không gian $\mathcal{M}_+^b(T)$ là Souslin (tương ứng Lusin).*

Xét một không gian Ba Lan P và một ánh xạ liên tục $f$ của P lên T (GT, IX, §6, No. 2, Định nghĩa 2). Cho $\tilde{f}$ là ánh xạ liên tục $\mu \mapsto f(\mu)$ từ $\mathcal{M}_+^b(P)$ vào $\mathcal{M}_+^b(T)$; không gian $\mathcal{M}_+^b(P)$ là Ba Lan theo Mệnh đề 10, và $\tilde{f}$ là toàn ánh (§2, No. 4, Mệnh đề 9); do đó không gian $\mathcal{M}_+^b(T)$ là Souslin. Tương tự, nếu T là Lusin, thì có thể giả sử $f$ là đơn ánh (GT, *loc. cit.*, No. 4, Mệnh đề 12); khi đó $\tilde{f}$ là đơn ánh (§2, No. 4, Mệnh đề 8), và vì thế $\mathcal{M}_+^b(T)$ là Lusin (GT, *loc. cit.*, No. 4, Mệnh đề 12).

Cho T là một không gian Souslin chính quy hoàn toàn (nhắc rằng, với điều này, chỉ cần T là Souslin và *chính quy* (TG, Phụ lục 1, Hệ quả của Mệnh đề 2)), và cho H là một tập con compact của $\mathcal{M}_+^b(T)$; khi đó H là compact và Souslin, do đó *metric hóa được*, đối với tôpô chặt (*loc. cit.*, Phụ lục 1, Hệ quả 2 của Mệnh đề 3).

### 5. Tiêu chuẩn compact cho hội tụ chặt

#### Định nghĩa 2 {#int-ix-s5-def-2 .statement}

*Cho T là một không gian tôpô, và cho H là một tập con của $\mathcal{M}^b(T)$; người ta nói rằng H thỏa mãn điều kiện Prokhorov nếu*
    a) $\sup_{\mu \in H} |\mu|(1) < +\infty$;
    b) *với mọi số $\varepsilon > 0$, tồn tại một tập con compact $K_\varepsilon$ của T sao cho*
    $$
    |\mu|(T - K_\varepsilon) \leq \varepsilon \quad \text{với mọi độ đo } \mu \in H.
    $$

Có thể chứng minh rằng nếu T là chính quy hoàn toàn, thì tập các điều kiện *a)* và *b)* tương đương với điều kiện sau: tồn tại một hàm thực $f \geq 1$ trên T sao cho tập các điểm t của T thỏa mãn $f(t) \leq c$ là compact với mọi $c \in \mathbf{R}_+$ (điều này đặc biệt suy ra rằng f là nửa liên tục dưới), và sao cho $\sup_{\mu \in H} |\mu|(f) < +\infty$. Hơn nữa, khi T là compact địa phương, ta thu được một mệnh đề tương đương bằng cách đòi hỏi f liên tục (xem Bài tập 10).

#### Mệnh đề 11 {#int-ix-s5-prop-11 .statement}

*Cho T là một không gian chính quy hoàn toàn, và cho H là một tập con của $\mathcal{M}^b(T)$ thỏa mãn điều kiện Prokhorov; khi đó bao đóng $\overline{H}$ của nó trong $\mathcal{M}^b(T)$ cũng thỏa mãn điều kiện Prokhorov.*

Vì, các hàm $\mu \mapsto |\mu|^*(1)$, $\mu \mapsto |\mu|^*(T - K_\varepsilon)$ là nửa liên tục dưới trên $\mathcal{M}^b(T)$ theo Mệnh đề 6 của No. 3.

Ý nghĩa của điều kiện Prokhorov xuất phát từ định lý sau, mà đảo lại của nó sẽ được khảo sát sau này (Định lý 2).

**Định lý 1 (Prokhorov).** — *Cho T là một không gian chính quy hoàn toàn, và cho H là một tập con của $\mathcal{M}^b(T)$ thỏa mãn điều kiện Prokhorov; khi đó H tương đối compact trong $\mathcal{M}^b(T)$ đối với tôpô chặt.*

Ta có thể giả sử rằng T là một không gian con của một không gian compact X; cho i là đơn ánh chính tắc của T vào X. Mặt khác, theo Mệnh đề 11, ta có thể giả sử rằng H là *đóng* trong $\mathcal{M}^b(T)$. Khi đó chỉ cần chứng minh rằng mọi siêu lọc $\mathfrak{U}$ trên H hội tụ trong $\mathcal{M}^b(T)$.

Ta sẽ bắt đầu với trường hợp $H \subset \mathcal{M}_+^b(T)$. Tổng khối lượng của các độ đo $\mu \in H$ bị chặn theo giả thiết, nên $i(\mu)$ hội tụ mơ hồ theo $\mathfrak{U}$, trong $\mathcal{M}_+(X)$, đến một độ đo $\nu \in \mathcal{M}_+(X)$ (Chương III, §1, No. 9, Hệ quả 2 của Mệnh đề 15); theo Mệnh đề 8 của No. 3, mọi việc quy về chứng minh rằng $\nu$ tập trung trên T. Bây giờ, cho $\varepsilon$ là một số $> 0$, và cho $K_\varepsilon$ là một tập con compact của T thỏa mãn công thức (6). Vì $X - K_\varepsilon$ là mở trong X, ta có, theo Mệnh đề 6 của No. 3 áp dụng trong X, các bất đẳng thức

$$
\nu^*(X - T) \leq \nu^*(X - K_\varepsilon) \leq \liminf_{\mu, \mathfrak{U}} i(\mu)^*(X - K_\varepsilon)
= \liminf_{\mu, \mathfrak{U}} \mu^*(T - K_\varepsilon) \leq \varepsilon;
$$

vì $\varepsilon > 0$ là tùy ý, định lý được chứng minh trong trường hợp đặc biệt này.

Ta chuyển sang trường hợp tổng quát; với mọi độ đo $\mu$ trên T, đặt

$$
a_1(\mu) = \Re(\mu)^+, \quad a_2(\mu) = \Re(\mu)^-, \quad a_3(\mu) = \Im(\mu)^+, \quad a_4(\mu) = \Im(\mu)^-;
$$

vì $\mu = a_1(\mu) - a_2(\mu) + ia_3(\mu) - ia_4(\mu)$, nên chỉ cần chứng minh rằng các ánh xạ $a_j$ ($j = 1, 2, 3, 4$) hội tụ chặt theo $\mathfrak{U}$. Nhưng tập $H_j$ gồm các độ đo $a_j(\mu)$, khi $\mu$ chạy qua H, thỏa mãn điều kiện Prokhorov nhờ hệ thức $|a_j(\mu)| \leq |\mu|$, và nằm trong $\mathcal{M}_+^b(T)$; do đó nó tương đối compact trong $\mathcal{M}_+^b(T)$ theo trường hợp đặc biệt, và khi ấy định lý suy ra ngay.

#### Hệ quả {#int-ix-s5-n5-cor-1 .statement}

==========

— Cho T là một không gian con của một không gian hoàn toàn chính quy X, và cho H là một tập con của $\mathcal{M}^b(T)$ thỏa mãn điều kiện của Prokhorov. Nếu i ký hiệu đơn ánh chính tắc của T vào X, thì hạn chế của ánh xạ $\mu \mapsto i(\mu)$ từ $\mathcal{M}^b(T)$ vào $\mathcal{M}^b(X)$ lên H là một đẳng cấu tôpô của H lên ảnh của nó.

Chỉ cần xét trường hợp H đóng (Mệnh đề 11), do đó compact; kết luận khi đó suy ra từ việc $\mu \mapsto i(\mu)$ liên tục và đơn ánh.

Nhắc lại rằng kết quả này cũng đúng cho một tập con tùy ý của $\mathcal{M}_+^b(T)$ (No. 3, Mệnh đề 8).

#### Định lý 2 {#int-ix-s5-thm-2 .statement}

— Cho T là một không gian địa phương compact, hoặc một không gian Polish, và cho H là một tập con tương đối compact của $\mathcal{M}_+^b(T)$; khi đó H thỏa mãn điều kiện của Prokhorov.

Ta có thể chỉ xét trường hợp H đóng, do đó compact. Các khối lượng toàn phần của các độ đo $\mu \in H$ hiển nhiên bị chặn, vì ánh xạ $\mu \mapsto \mu(1)$ liên tục, và mọi việc quy về chứng minh mệnh đề b) của Định nghĩa 2.

Trước hết giả sử T là địa phương compact. Cho $\varepsilon$ là một số $> 0$. Ta gán cho mỗi độ đo $\mu \in H$ một tập compact $K_\mu$ trong T sao cho $\mu^\bullet(T - K_\varepsilon) < \varepsilon$, rồi một lân cận mở tương đối compact $U_\mu$ của $K_\mu$. Vì hàm $\lambda \mapsto \lambda^\bullet(T - U_\mu)$ là nửa liên tục trên trên $\mathcal{M}_+^b(T)$ (No. 3, Mệnh đề 6), tập $V^\mu$ gồm các độ đo $\lambda \in H$ sao cho $\lambda^\bullet(T - U_\mu) < \varepsilon$ là một lân cận của $\mu$ trong H. Do đó tồn tại một tập con hữu hạn $H'$ của H sao cho các tập $V^\mu$ ($\mu \in H'$) phủ H. Ký hiệu K là tập compact $\bigcup_{\mu \in H'} \overline{U}_\mu$, ta có $\lambda^\bullet(T - K) < \varepsilon$ với mọi $\lambda \in H$.

Tiếp theo giả sử T là Polish. Ta không hạn chế tính tổng quát khi giả sử rằng T là giao của một dãy giảm $(T_p)_{p \geq 1}$ các tập con mở của một không gian compact X (GT, IX, §6, No. 1, Hệ quả 1 của Định lý 1). Gọi $i_p$ là đơn ánh của T vào $T_p$, và gọi $H_p$ là tập các độ đo có dạng $i_p(\lambda)$ với $\lambda \in H$; vì $H_p$ compact trong $\mathcal{M}_+^b(T_p)$, suy ra tồn tại một tập compact $K_p \subset T_p$ sao cho $\nu^\bullet(T_p - K_p) \leq \varepsilon 2^{-p}$ với mọi độ đo $\nu \in H_p$, theo kết quả trên áp dụng cho không gian địa phương compact $T_p$. Do đó cũng có $\nu^\bullet(T - (T \cap K_p)) \leq \varepsilon 2^{-p}$, và cuối cùng $\lambda^\bullet(T - (T \cap K_p)) \leq \varepsilon 2^{-p}$ với mọi độ đo $\lambda \in H$. Bây giờ đặt $K = \bigcap_p K_p$; tập K là compact và được chứa trong T, và, với mọi độ đo $\lambda \in H$, ta có $\lambda^\bullet(T - K) \leq \sum_p \lambda^\bullet(T - (T \cap K_p)) \leq \sum_p \varepsilon 2^{-p} = \varepsilon$. Vậy điều kiện của Prokhorov đã được xác minh.

### 6. Hội tụ chặt của độ đo và hội tụ compact của hàm

#### Mệnh đề 12 {#int-ix-s5-prop-12 .statement}

— Cho T là một không gian hoàn toàn chính quy, và cho B là quả cầu đơn vị của không gian định chuẩn $\mathcal{C}^b(T; \mathbf{C})$. Cho I là một dạng tuyến tính trên $\mathcal{C}^b(T; \mathbf{C})$. Để tồn tại một độ đo phức bị chặn $\theta$ trên T sao cho $I(f) = \theta(f)$ với mọi $f \in \mathcal{C}^b(T; \mathbf{C})$, cần và đủ là hạn chế của I lên B liên tục đối với tôpô hội tụ compact. Khi đó $\theta$ là duy nhất.

Ta hãy chứng minh rằng điều kiện trong phát biểu là cần. Cho $\theta$ là một độ đo phức bị chặn trên T, $\varepsilon$ là một số $> 0$, và K là một tập con compact của T sao cho $|\theta|^*(T - K) < \varepsilon$. Cho $f \in B$; ta ký hiệu U là lân cận của f trong B đối với tôpô hội tụ compact, gồm các hàm $g \in B$ sao cho $\sup_{x \in K} |g(x) - f(x)| \leq \varepsilon$. Khi đó, với mọi $g \in U$,

$$
|\theta(g) - \theta(f)| \leq \int_T |g - f| d|\theta| \leq \varepsilon |\theta|^*(K) + 2|\theta|^*(T - K) \leq (||\theta|| + 2)\varepsilon ,
$$

vì $|g - f|$ bị chặn trên bởi $\varepsilon$ trên K và bởi 2 trên $T - K$.

Ngược lại, xét một dạng tuyến tính I trên $\mathcal{C}^b(T; \mathbf{C})$ mà sự hạn chế của nó lên B liên tục đối với tôpô hội tụ compact. Khi đó, với mọi số $\varepsilon > 0$, tồn tại một số $a > 0$ và một tập con compact K của T sao cho các quan hệ $f \in B, \sup_{x \in K} |f(x)| \leq a$ kéo theo $|I(f)| \leq \varepsilon$. Mệnh đề 5 của No. 2 khi đó suy ra sự tồn tại của một độ đo phức bị chặn duy nhất $\theta$ sao cho $I(f) = \theta(f)$ với mọi $f \in \mathcal{C}^b(T; \mathbf{C})$.

#### Mệnh đề 13 {#int-ix-s5-prop-13 .statement}

— Cho T là một không gian compact địa phương, và H là một tập con bị chặn của không gian định chuẩn $\mathcal{C}^b(T; \mathbf{C})$. Ánh xạ $(\mu, f) \mapsto \mu(f)$ của $\mathcal{M}_+^b(T) \times H$ vào $\mathbf{C}$ khi đó liên tục, khi $\mathcal{M}_+^b(T)$ được trang bị tôpô chặt, và H với tôpô hội tụ compact.

Cho $\mu \in \mathcal{M}_+^b(T), f \in H$, và cho M là một số thực sao cho $||\mu|| < M$, và $|g| \leq M$ với mọi $g \in H$. Cho $\varepsilon$ là một số $> 0$ và chọn một tập con compact K của T sao cho $\mu^*(T - K) < \varepsilon$, rồi một lân cận mở tương đối compact S của K. Tập U gồm các độ đo $\lambda \in \mathcal{M}_+^b(T)$ thỏa mãn các bất đẳng thức

$$
\lambda^*(T) < M , \quad \lambda^*(T - S) < \varepsilon , \quad |\lambda(f) - \mu(f)| < \varepsilon
$$

khi đó là một lân cận của $\mu$ trong $\mathcal{M}_+^b(T)$ (No. 3, Mệnh đề 6). Ngoài ra, gọi V là lân cận của $f$ trong H gồm các hàm $g \in H$ sao cho

$$
\sup_{x \in S} |g(x) - f(x)| < \varepsilon .
$$

Cho $\lambda \in U$ và $g \in V$; vì hàm $|g - f|$ bị chặn trên bởi $\varepsilon$ trên S, và bởi $2M$ trên $T - S$, ta có
$$
|\lambda(g) - \lambda(f)| \leq \int_T |g - f| d\lambda \leq \varepsilon \lambda^*(S) + 2M \lambda^*(T - S) \leq 3M \varepsilon,
$$
từ đó suy ra
$$
|\lambda(g) - \mu(f)| \leq |\lambda(g) - \lambda(f)| + |\lambda(f) - \mu(f)| \leq (3M + 1)\varepsilon.
$$
Điều này chứng minh tính liên tục của ánh xạ $(\lambda, g) \mapsto \lambda(g)$ tại điểm $(\mu, f)$ của $\mathcal{M}_+^b(T) \times H$.

#### Nhận xét {#int-ix-s5-n6-rem-1 .statement}

Cho $T$ là một không gian chính quy hoàn toàn, $M$ là một tập con của $\mathcal{M}^b(T)$ thỏa mãn điều kiện Prokhorov, $H$ là một tập con bị chặn của $C^b(T)$. Một lập luận rất gần với lập luận vừa nêu có thể dùng để chứng minh rằng ánh xạ $(\lambda, g) \mapsto \lambda(g)$ của $M \times H$ vào $\mathbf{C}$ là liên tục khi $M$ được trang bị tôpô chặt và H với tôpô hội tụ compact.

#### Hệ quả {#int-ix-s5-n6-cor-1 .statement}

*Cho $T$ là một không gian hoàn toàn chính quy, $X$ là một không gian tôpô, và $f$ là một hàm nhận giá trị phức xác định trên $T \times X$, liên tục và bị chặn. Với mọi độ đo bị chặn $\mu$ trên $T$, ký hiệu $F_\mu$ là hàm trên $X$ được xác định bởi $F_\mu(x) = \int_T f(t, x) d\mu(t)$ với mọi $x \in X$.

a) Hàm $F_\mu$ liên tục và bị chặn với mọi độ đo bị chặn $\mu$.

b) Giả sử rằng $T$ là địa phương compact. Ánh xạ $\mu \mapsto F_\mu$ của $\mathcal{M}_+^b(T)$ vào $C^b(X; \mathbf{C})$ khi đó liên tục, nếu $\mathcal{M}_+^b(T)$ được trang bị tôpô chặt, và $C^b(X; \mathbf{C})$ với tôpô hội tụ trên các tập compact.

Với mọi $x \in X$, ký hiệu $f_x$ là hàm liên tục và bị chặn $t \mapsto f(t, x)$ trên $T$; ánh xạ $x \mapsto f_x$ của $X$ vào $C^b(T; \mathbf{C})$ có ảnh bị chặn, và nó liên tục nếu $C^b(T; \mathbf{C})$ được trang bị tôpô hội tụ trên các tập compact (GT, X, §3, No. 4, Định lý 3). Vì $F_\mu(x) = \mu(f_x)$, hàm $F_\mu$ liên tục theo Mệnh đề 12. Giả sử $T$ là địa phương compact; Mệnh đề 13 cho thấy rằng ánh xạ $(\mu, x) \mapsto F_\mu(x)$ của $\mathcal{M}_+^b(T) \times X$ vào $\mathbf{C}$ là liên tục; mệnh đề $b)$ suy ra từ đó (*loc. cit.*).

### 7. Ứng dụng: phép biến đổi Laplace

Trong mục này, ta ký hiệu $M$ là một monoid giao hoán, với luật hợp thành được viết theo phép cộng, được trang bị tôpô của một không gian *địa phương compact*, sao cho ánh xạ $(m, m') \mapsto m + m'$ của $M \times M$ vào $M$ liên tục. Phần tử trung hòa của $M$ được ký hiệu bởi $0$. Ta gọi *đặc trưng* của $M$ là mọi hàm phức liên tục bị chặn $\chi$ trên $M$ thỏa mãn các hệ thức
$$
\chi(m + m') = \chi(m) \cdot \chi(m'), \quad \chi(0) = 1, \quad |\chi(m)| \leq 1
$$

với $m, m'$ trong $M$. Nếu $\chi$ và $\chi'$ là các đặc trưng, thì $\chi \chi'$ cũng vậy. Tập các đặc trưng của $M$ là một monoid, ký hiệu $X$; hãy trang bị cho nó tôpô hội tụ trên các tập compact, khi đó ánh xạ $(\chi, \chi') \mapsto \chi \chi'$ của $X \times X$ vào $X$ là liên tục. Phần tử trung hòa của $X$ là hàm hằng 1.

Với mọi độ đo phức bị chặn $\mu$ trên $M$, người ta gọi *biến đổi Laplace* của $\mu$ là hàm $\mathcal{L}\mu$ trên $X$ được xác định bởi

$$
(\mathcal{L}\mu)(\chi) = \int_M \chi(m)\, d\mu(m).
$$

Theo Định lý 3 của GT, X, §3, No. 4, ánh xạ $(m, \chi) \mapsto \chi(m)$ từ $M \times X$ vào $\mathbf{C}$ là liên tục và bị chặn. Hệ quả của Mệnh đề 13 của No. 6 suy ra kết quả sau:

#### Mệnh đề 14 {#int-ix-s5-prop-14 .statement}

*Với mọi độ đo phức bị chặn $\mu$ trên $M$, hàm $\mathcal{L}\mu$ trên $X$ là liên tục và bị chặn. Nếu $\mathcal{M}_+^b(M)$ được trang bị tôpô chặt và $\mathcal{C}^b(X; \mathbf{C})$ được trang bị tôpô của sự hội tụ compact, thì ánh xạ $\mu \mapsto \mathcal{L}\mu$ từ $\mathcal{M}_+^b(M)$ vào $\mathcal{C}^b(X; \mathbf{C})$ là liên tục.*

Tập các đặc trưng của $M$ tiến tới 0 ở vô cùng sẽ được ký hiệu là $X_0$; tập này ổn định đối với phép nhân. Ta sẽ nói rằng một monoid con$^{(1)}$ S của $X$ là *đầy đủ* nếu S ổn định đối với ánh xạ $\chi \mapsto \overline{\chi}$, $S \cap X_0$ phân biệt các điểm của $M$ (GT, X, §4, No. 1, Định nghĩa 1) và nếu, với mọi $m \in M$, tồn tại một phần tử $\chi$ của $S \cap X_0$ sao cho $\chi(m) \neq 0$.

Giả sử thêm rằng $M$ là một nhóm Abel không compact. Cho $f$ là một hàm trên $M$ tiến tới 0 ở vô cùng; khi đó hàm $x \mapsto f(x)f(-x)$ trên $M$ cũng vậy, trong khi mọi đặc trưng $\chi$ của $M$ đều thỏa $\chi(x)\chi(-x) = \chi(0) = 1$. Suy ra $X_0$ rỗng, và $X$ không chứa bất kỳ monoid con đầy đủ nào. Do đó, Định lý 3 dưới đây không áp dụng cho các nhóm địa phương compact không compact.

#### Định lý 3 {#int-ix-s5-thm-3 .statement}

*Cho S là một monoid con đầy đủ của X.*
a) *Nếu $\mu$ và $\mu'$ là hai độ đo phức bị chặn trên $M$, sao cho $\mathcal{L}\mu$ và $\mathcal{L}\mu'$ có cùng hạn chế trên $S \cap X_0$, thì $\mu = \mu'$.*
b) *Cho $\mathfrak{F}$ là một bộ lọc trên $\mathcal{M}_+^b(M)$, sao cho $\mathcal{L}\lambda(s)$ có giới hạn $\Phi(s) \in \mathbf{C}$ đối với $\mathfrak{F}$ với mọi $s \in S$. Khi đó bộ lọc $\mathfrak{F}$ hội tụ mơ hồ đến một độ đo dương bị chặn $\mu$, và $\Phi(s) = \mathcal{L}\mu(s)$ với mọi $s \in S \cap X_0$.*
c) *Dưới các giả thiết của b), giả sử thêm rằng bao đóng của $S \cap X_0$ chứa 1, và hàm $\Phi$ trên S liên tục tại điểm 1. Khi đó $\mathfrak{F}$ hội tụ chặt đến $\mu$, và $\Phi(s) = \mathcal{L}\mu(s)$ với mọi $s \in S$.*

Ta sẽ ký hiệu bởi E đại số các hàm phức liên tục tiến tới 0 ở vô cùng trên $M$, và bởi $\mathfrak{A}$ không gian con tuyến tính của E được sinh bởi

\footnotetext{(1) Nhắc lại rằng một monoid con của một monoid A theo định nghĩa chứa phần tử trung hòa của A (A, I, §2, No. 1).}

bởi $S \cap X_0$; khi đó $\mathfrak{A}$ là một đại số con của $E$ ổn định dưới ánh xạ $f \mapsto \overline{f}$; vì $S$ là một monoid con đầy đủ của $X$, Hệ quả 2 của Mệnh đề 7 của GT, X, §4, No. 4 suy ra rằng $\mathfrak{A}$ trù mật trong $E$.

Chứng minh a): theo giả thiết, $\mu(f) = \mu'(f)$ với mọi $f \in \mathfrak{A}$; vì $\mu$ và $\mu'$ là các dạng tuyến tính liên tục trên $E$, điều này suy ra rằng $\mu(f) = \mu'(f)$ với $f \in E$, và đặc biệt với mọi hàm liên tục có giá đỡ compact, suy ra $\mu = \mu'$.

Ta đặt mình dưới các giả thiết của b). Số $\Phi(1) = \lim_{\lambda, \mathfrak{F}} \lambda(1)$ là thực và dương; cho một số thực $a > \Phi(1)$; vì $\| \lambda \| = \mathcal{L} \lambda(1)$ với $\lambda \in \mathcal{M}_+^b(M)$, quan hệ $\lim_{\lambda, \mathfrak{F}} \mathcal{L} \lambda(1) = \Phi(1)$ suy ra rằng tập hợp $H$ các độ đo $\lambda \in \mathcal{M}_+^b(M)$ sao cho $\| \lambda \| \leq a$ thuộc $\mathfrak{F}$. Vì $\mathcal{M}^b(M; \mathbf{C})$ có thể được đồng nhất với không gian đối ngẫu của không gian định chuẩn $E$ (Chương III, §1, No. 8 & §1, No. 2, Mệnh đề 3), không gian $H$ là compact đối với tôpô $\sigma(\mathcal{M}^b(M; \mathbf{C}), E)$. Mặt khác (TVS, III, §3, No. 4, Mệnh đề 5), tôpô này trùng trên $H$ với tôpô hội tụ từng điểm trên bất kỳ tập con toàn phần nào của $E$. Đặc biệt, vì $\mathfrak{A}$ trù mật trong $E$, và điều tương tự đúng với không gian các hàm liên tục có giá đỡ compact (Chương III, §1, No. 2, Mệnh đề 3), tôpô hội tụ từng điểm trên $S \cap X_0$ trùng trên $H$ với tôpô mờ, và $H$ là compact đối với tôpô này. Suy ra ngay rằng $\mathfrak{F}$ hội tụ theo tôpô mờ đến một độ đo $\mu \in H$, và $\mathcal{L} \mu(s) = \lim_{\lambda, \mathfrak{F}} \mathcal{L} \lambda(s)$ với mọi $s \in S \cap X_0$.

Cuối cùng, ta xét c). Vì các hàm $\Phi$ và $\mathcal{L} \mu$ liên tục tại điểm $1 \in S$, và bằng nhau trên $S \cap X_0$, lại vì $1$ thuộc bao đóng của $S \cap X_0$, ta có $\Phi(1) = \mathcal{L} \mu(1)$. Nói cách khác, $\lim_{\lambda, \mathfrak{F}} \lambda(1) = \mu(1)$. Mệnh đề 9 của No. 3 khi đó cho thấy rằng $\mu$ là giới hạn chặt của bộ lọc $\mathfrak{F}$. Mọi phần tử của $S$ đều là một hàm liên tục bị chặn trên $M$, điều này suy ra rằng $\Phi(s) = \lim_{\lambda, \mathfrak{F}} \lambda(s) = \mu(s) = \mathcal{L} \mu(s)$ với mọi $s \in S$.

#### Hệ quả {#int-ix-s5-n7-cor-1 .statement}

— *Cho $S$ là một monoid con đầy đủ của $X$, sao cho bao đóng của $S \cap X_0$ chứa 1. Gọi $L$ là tập con của $\mathcal{C}^b(S; \mathbf{C})$ gồm các hạn chế lên $S$ của các biến đổi Laplace của các độ đo $\lambda \in \mathcal{M}_+^b(M)$.*

a) *Tập $L$ đóng trong không gian $\mathcal{C}^b(S; \mathbf{C})$ được trang bị tôpô hội tụ điểm.*

b) *Ánh xạ $\lambda \mapsto (\mathcal{L} \lambda)_S$ là một đồng phôi từ $\mathcal{M}_+^b(M)$ lên $L$, nếu $\mathcal{M}_+^b(M)$ được trang bị tôpô chặt và $L$ được trang bị tôpô hội tụ điểm.*

c) *Tôpô hội tụ điểm và tôpô hội tụ trên compact trùng nhau trên $L$.*

Các mệnh đề $a)$ và $b)$ là những hệ quả ngay lập tức của Th. 3; mệnh đề $c)$ suy ra từ $b)$ và Mệnh đề 14, vì tôpô hội tụ trên compact mịn hơn tôpô hội tụ điểm.

Cần lưu ý rằng L không đóng trong tập tất cả các hàm phức bị chặn trên S, được trang bị tôpô hội tụ điểm. Chẳng hạn, hãy xét các ký hiệu của Ví dụ 2 dưới đây (M = \mathbf{R}_+, S được đồng nhất với \mathbf{R}_+). Các biến đổi Laplace của các độ đo $\varepsilon_n$ ($n \in \mathbf{N}$) là các hàm $t \mapsto e^{-nt}$ trên $\mathbf{R}_+$; khi $n$ tiến tới $+\infty$, các hàm này hội tụ điểm đến hàm bằng 1 khi $t = 0$ và bằng 0 khi $t \neq 0$, hàm này không thuộc L.

*Ví dụ 1).* — Lấy M là tập N các số nguyên dương, được trang bị luật cộng và tôpô rời rạc. Cho D là đĩa đơn vị của \mathbf{C} (tập các số phức có giá trị tuyệt đối $\leq 1$) được trang bị tôpô cảm sinh bởi \mathbf{C} và luật cảm sinh bởi phép nhân. Với mọi $z \in D$, ta ký hiệu bởi $f(z)$ đặc trưng $n \mapsto z^n$ của N. Với mọi đặc trưng $\chi$ của N, ký hiệu bởi $g(\chi)$ số phức $\chi(1) \in D$. Ta kiểm tra ngay lập tức rằng $f$ và $g$ là các đồng phôi nghịch đảo với nhau giữa D và X, điều này sẽ cho phép ta, từ nay về sau, *đồng nhất* X và D. Tập các đặc trưng tiến về 0 ở vô cực khi đó có thể được đồng nhất với tập $D_0$ gồm các số phức có giá trị tuyệt đối < 1. Cuối cùng, khoảng ]0, 1] của \mathbf{R} là một monoid con đầy đủ của D, và 1 thuộc bao đóng của ]0, 1[ \cap D_0 = ]0, 1[.

Mọi độ đo $\mu$ trên N có thể được viết duy nhất dưới dạng $\mu = \sum_{n \in \mathbf{N}} u_n \cdot \varepsilon^n$, và $\mu$ bị chặn khi và chỉ khi $\sum_n |u_n| < +\infty$; khi đó ta có $\mathcal{L}\mu(z) = \sum_{n \in \mathbf{N}} u_n z^n$ với $z \in D$. Hàm này liên tục trên D; người ta thường gọi nó là *hàm sinh* của dãy khả tổng $(u_n)_{n \in \mathbf{N}}$. Chuyển sang ngôn ngữ này, Th. 3 cho kết quả sau (xét đến Mệnh đề 9 của No. 3):

#### Mệnh đề 15 {#int-ix-s5-prop-15 .statement}

*Cho A là một tập hợp được trang bị một bộ lọc $\mathfrak{F}$. Với mọi $\alpha \in A$, cho $(u_{\alpha,n})_{n \in \mathbf{N}}$ là một dãy khả tổng các số dương, và cho $\Phi_\alpha$ là hàm xác định trên khoảng ]0, 1] của \mathbf{R} bởi $\Phi_\alpha(x) = \sum_{n \in \mathbf{N}} u_{\alpha,n} x^n$. Để tồn tại một dãy khả tổng $(u_n)_{n \in \mathbf{N}}$ các số dương sao cho*

$$
\lim_{\alpha, \mathfrak{F}} u_{\alpha,n} = u_n \quad \text{for all } n , \quad \lim_{\alpha, \mathfrak{F}} \sum_{n \in \mathbf{N}} u_{\alpha,n} = \sum_{n \in \mathbf{N}} u_n ,
$$

*thì cần và đủ rằng $\Phi_\alpha$ hội tụ điểm trên ]0, 1[, theo $\mathfrak{F}$, đến một hàm $\Phi$ liên tục tại điểm 1. Trong trường hợp này, $\Phi(x) = \sum_{n \in \mathbf{N}} u_n x^n$ với mọi $x \in ]0, 1[$.*

Các kết quả tương tự nhận được khi lấy $M$ là monoid $\mathbf{N}^n$, trong đó $n$ là một số nguyên $> 1$; khi đó không gian $X$ có thể được đồng nhất với $D^n$, và có thể chọn $]0, 1[^n$ làm monoid con đầy đủ. Chúng tôi để người đọc chép lại Định lý 3 trong trường hợp này.

Ví dụ 2). — Hãy lấy cho $M$ tập hợp $\mathbf{R}_+$, được trang bị luật cộng và tôpô thông thường. Cho $P$ là tập hợp các số phức $z$ có phần thực dương, được trang bị tôpô cảm sinh bởi $C$, và luật cảm sinh bởi phép cộng trong $C$. Với mọi $p \in P$, ký hiệu $f(p)$ là đặc trưng $x \mapsto e^{-px}$ của $\mathbf{R}_+$; dễ thấy rằng $f$ là một đẳng cấu của cấu trúc monoid tôpô của $P$ lên cấu trúc của $X$; ta sẽ đồng nhất $X$ với $P$ qua $f$. Hiển nhiên $\mathbf{R}_+$ là một monoid con đầy đủ của $P$, và Định lý 3 cho kết quả sau:

#### Mệnh đề 16 {#int-ix-s5-prop-16 .statement}

*Cho $A$ là một tập hợp được trang bị một bộ lọc $\mathcal{F}$. Với mọi $\alpha \in A$, cho $\mu_\alpha$ là một độ đo dương bị chặn trên $\mathbf{R}_+$, và cho $\Phi_\alpha$ là hàm xác định trên $\mathbf{R}_+$ bởi $\Phi_\alpha(p) = \int_0^{+\infty} e^{-px} d\mu_\alpha(x)$. Để ánh xạ $\alpha \mapsto \mu_\alpha$ hội tụ chặt theo $\mathcal{F}$ đến một độ đo dương bị chặn $\mu$, điều kiện cần và đủ là $\Phi_\alpha$ hội tụ từng điểm trên $\mathbf{R}_+$, theo $\mathcal{F}$, đến một hàm $\Phi$ liên tục tại điểm 0. Trong trường hợp này, $\Phi(p) = \int_0^{+\infty} e^{-px} d\mu(x)$ với mọi $p \in \mathbf{R}_+$. \*

Có các kết quả tương tự cho các monoid cộng tính $\mathbf{R}_+^n$ ($n$ là một số nguyên $> 1$); trong trường hợp này chúng tôi để người đọc chép lại Định lý 3.

### Bài tập {#int-ix-s5-exercises}

Xem [các bài tập cho § 5](exercises/s5/).
