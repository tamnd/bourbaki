---
book: int
book_title: Integration
chapter: V
chapter_title: INTEGRATION OF MEASURES
section: 5
section_title: Measures defined by numerical densities
lang: vi
source: int-i-vi
book_pages: INT V.38-INT V.62, INT V.99-INT V.107
pdf_pages: 0293-0317, 0354-0362
extraction: ocr
subsections:
    - "no": 1
      title: Locally integrable functions
      page: 38
      pdf_page: 293
    - "no": 2
      title: Measures defined by numerical densities
      page: 40
      pdf_page: 295
    - "no": 3
      title: Integration with respect to a measure defined by a density
      page: 42
      pdf_page: 297
    - "no": 4
      title: Behavior of the product with respect to the usual operations
      page: 45
      pdf_page: 300
    - "no": 5
      title: Characterization of measures with base $\mu$
      page: 48
      pdf_page: 303
    - "no": 6
      title: Equivalent measures
      page: 52
      pdf_page: 307
    - "no": 7
      title: Alien measures
      page: 54
      pdf_page: 309
    - "no": 8
      title: 'Applications: I. Duality of the spaces $L^p$'
      page: 56
      pdf_page: 311
    - "no": 9
      title: 'Applications: II. Functions of measures'
      page: 60
      pdf_page: 315
    - "no": 10
      title: Diffuse measures; atomic measures
      page: 61
      pdf_page: 316
statements: 52
exercises: 31
content_sha256: 59ae08b2722925a6a198a4adf210da3a3eb4a8ed7bb17b1a44fcd6110338c92c
translated_from: content/en/int/V/05_s5_measures_defined_by_numerical_densities.md
source_content_sha256: 558c461f3e10e0b61d6e6a8d8129f54ba980ff5cc18f3a572913b450c90ee96e
translation_model: gpt-5.4-mini
translation_run: translate-vi-57dece11
glossary_version: 34
glossary_terms_sha256: 66cb581208be8267303af2d760ccda2b43a615bacbe00e2d3959ce3c0df5541d
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 5. ĐỘ ĐO ĐƯỢC XÁC ĐỊNH BỞI CÁC MẬT ĐỘ SỐ

### 1. Các hàm khả tích địa phương

#### Mệnh đề 1 {#int-v-s5-prop-1 .statement}

*Cho $g$ là một hàm được định nghĩa địa phương hầu khắp nơi trong $T$ (đối với độ đo dương $\mu$), với giá trị trong một không gian Banach $F$ (resp. in $\overline{\mathbf{R}}$). Các tính chất sau là tương đương:*

a) *Với mọi điểm $t \in T$, tồn tại một lân cận V của t sao cho hàm $g \varphi_V$ là $\mu$-khả tích.*

b) *Hàm g là $\mu$-đo được và, với mọi tập compact $K \subset T$, $\int^* |g|\varphi_K\,d\mu < +\infty$.*

c) *Với mọi hàm số $h \in \mathcal{K}(T)$, $gh$ là $\mu$-khả tích.*

Ta chứng minh rằng a) suy ra b); thật vậy, hàm g đo được theo nguyên lý địa phương hóa (Ch. IV, §5, No. 2, Mệnh đề 4). Mặt khác, với mọi $t \in K$ tồn tại, theo giả thiết, một lân cận $V_t$ của $t$ trong $T$ sao cho $g \varphi_{V_t}$ khả tích; do đó có thể phủ $K$ bởi một số hữu hạn các lân cận $V_i$ ($1 \leq i \leq n$) sao cho các hàm $g \varphi_{V_i}$ khả tích. Vì $|g| \varphi_K \leq \sum_{i=1}^n |g| \varphi_{V_i}$, nên $\int^* |g| \varphi_K \, d\mu < +\infty$.

Mặt khác, b) suy ra c), vì khi đó $gh$ là đo được, và nếu $L$ là giá compact của $h$ thì $|gh| \leq \|h\| \cdot |g| \varphi_L$, do đó $\int^* |gh| \, d\mu < +\infty$ theo giả thiết; vì vậy $gh$ khả tích theo tiêu chuẩn khả tích (Ch. IV, §5, No. 6, Định lý 5).

Cuối cùng, c) suy ra a). Thật vậy, với mọi $t \in T$ hãy lấy $V$ là một lân cận compact của $t$. Tồn tại một ánh xạ liên tục $h$ của $T$ vào $[0,1]$, bằng 1 trên $V$ và có giá compact (Ch. III, §1, No. 2, Bổ đề 1); theo giả thiết $gh$ khả tích, do đó $g \varphi_V = (gh) \varphi_V$ cũng khả tích (Ch. IV, §5, No. 6, Hệ quả 3 của Định lý 5).

#### Định nghĩa 1 {#int-v-s5-def-1 .statement}

*Một hàm* $g$, *được định nghĩa địa phương hầu khắp nơi trong* $T$ *(đối với độ đo dương* $\mu$*), *với giá trị trong một không gian Banach* $F$ *(resp. in* $\overline{\mathbf{R}}$*), *được gọi là khả tích địa phương đối với* $\mu$ *(hay khả tích địa phương theo* $\mu$*) nếu nó thỏa mãn các điều kiện* a), b), c) *của Mệnh đề 1.* *Nếu* $\theta$ *là một độ đo phức, một hàm* $g$ *được định nghĩa địa phương* $\theta$*-hầu khắp nơi được gọi là khả tích địa phương theo* $\theta$ *nếu nó khả tích địa phương đối với độ đo dương* $|\theta|$.

Nếu $g$ khả tích địa phương theo $\theta$, thì mọi hàm bằng $g$ địa phương hầu khắp nơi đều khả tích địa phương. Hiển nhiên tổng của hai hàm khả tích địa phương là khả tích địa phương. Các hàm nhận giá trị trong $F$, *được xác định khắp nơi* và khả tích địa phương đối với $\theta$, tạo thành một không gian vectơ ký hiệu $\mathcal{L}_{loc}^1(T, \theta; F)$; khi $F = \mathbf{R}$ hoặc $\mathbf{C}$, người ta thường lược bỏ nhắc đến $F$ nếu không có nhập nhằng. Không gian này luôn được trang bị (trừ khi có nói rõ ngược lại) tôpô được xác định bởi các nửa chuẩn $g \mapsto \int |g \varphi_K| \, d|\theta|$, trong đó $K$ chạy qua tập hợp các tập con compact của $T$. Không gian Hausdorff liên kết, tức thương của $\mathcal{L}_{loc}^1(T, \theta; F)$ theo không gian con $\mathcal{N}_F^\infty$ gồm các ánh xạ bằng không địa phương hầu khắp nơi, được ký hiệu là $L_{loc}^1(T, \theta; F)$. Các không gian $L_{loc}^1(T, \theta; F)$ và $L_{loc}^1(T, |\theta|; F)$ là như nhau.

Có thể chứng minh rằng các không gian vectơ tôpô vừa định nghĩa là *đầy đủ* (Bài tập 31).

Mọi hàm đo được $g$, tức bị chặn hầu khắp trên mọi tập compact, đều khả tích địa phương. Với mọi số $p$ sao cho $1 \leq p \leq +\infty$, mọi hàm $g \in \mathcal{L}_F^p$ đều khả tích địa phương; thật vậy, với mọi hàm $h \in \mathcal{H}(T)$, $h$ thuộc $\mathcal{L}^q$ (trong đó $q$ là số mũ liên hợp của $p$), do đó $gh$ là khả tích (Chương IV, §6, No. 4, Hệ quả 4 của Định lý 2).

Cho $F, G, H$ là ba không gian Banach, và $(u, v) \mapsto \Phi(u, v)$ là một ánh xạ song tuyến tính liên tục của $F \times G$ vào $H$. Nếu $f$ khả tích địa phương và nhận giá trị trong F, và nếu $g \in \mathcal{L}_G^\infty$, thì $\Phi(f, g)$ khả tích địa phương (Chương IV, §6, No. 4, Hệ quả 1 của Định lý 2).

### 2. Các độ đo được xác định bởi mật độ số

Cho $g$ là một hàm số dương được định nghĩa địa phương hầu khắp nơi theo $\mu$ trong T và khả tích địa phương theo $\mu$; khi đó tập các $t$ sao cho $g(t) = +\infty$ là một tập địa phương $\mu$-không đáng kể, vì $g \varphi_K$ là $\mu$-khả tích với mọi tập compact K (Chương IV, §2, No. 3, Mệnh đề 7). Bây giờ cho $g'$ là một hàm khả tích địa phương, dương và hữu hạn, bằng $g$ địa phương hầu khắp nơi theo $\mu$; đặt $\lambda'_t = g'(t) \varepsilon_t$. Ánh xạ $t \mapsto \lambda'_t$ của T vào $\mathcal{M}_+(T)$ là đo được yếu theo $\mu$ và khả tích theo vô hướng một cách thiết yếu (hay cũng vậy, cặp $(I, g')$, trong đó I là ánh xạ đồng nhất của T, là $\mu$-thích nghi); nguyên $\nu = \int \lambda'_t d\mu(t)$ không phụ thuộc vào hàm $g'$ cụ thể, bằng $g$ ở địa phương hầu khắp nơi, được dùng trong định nghĩa các độ đo $\lambda'_t$. Độ đo này $\nu$ được xác định bởi điều kiện

$$
\int f(t)\,d\nu(t) = \int f(t)g(t)\,d\mu(t) \quad \text{cho } f \in \mathcal{K}(T).
$$

Nếu bây giờ $\theta$ là một phép đo phức, và nếu $u$ là một hàm phức (hay một hàm nhận giá trị trong $\overline{\mathbf{R}}$) được xác định địa phương $\theta$-hầu khắp nơi và địa phương khả tích đối với $\theta$, ta có thể viết

$$
\begin{align*}
u &= g_1 - g_2 + i(g_3 - g_4) \\
\theta &= \mu_1 - \mu_2 + i(\mu_3 - \mu_4)
\end{align*}
$$

trong đó $\mu_1 = (\Re \theta)^+$, $\mu_2 = (\Re \theta)^-$, $\mu_3 = (\Im \theta)^+$, $\mu_4 = (\Im \theta)^-$ (Ch. III, §1, No. 5), và trong đó $g_1, g_2, g_3, g_4$ có các nghĩa tương tự; vì $|u|$ là địa phương $|\theta|$-khả tích, mỗi hàm dương $g_i$ ($i = 1, 2, 3, 4$) đều địa phương khả tích đối với từng phép đo dương $\mu_j$ ($j = 1, 2, 3, 4$), do đó ánh xạ

$$
f \mapsto \int f(t)u(t)\,d\theta(t)
$$

trên $\mathcal{K}(T)$ là một phép đo phức.

#### Định nghĩa 2 {#int-v-s5-def-2 .statement}

*Cho $\theta$ là một phép đo phức, và cho $u$ là một hàm phức (hay một hàm nhận giá trị trong $\overline{\mathbf{R}}$) được xác định địa phương $\theta$-hầu khắp nơi và địa phương $\theta$-khả tích. Phép đo phức $f \mapsto \int fu\,d\theta$ trên T được gọi là tích của phép đo $\theta$ với hàm $u$, hay là phép đo với mật độ $u$ đối với $\theta$, và được ký hiệu $u \cdot \theta$.*

Mọi phép đo phức là tích của một phép đo dương $\mu$ với một hàm địa phương $\mu$-khả tích được gọi là một phép đo có cơ sở $\mu$.

Quan hệ $\eta = u \cdot \theta$ một lần nữa, theo quy ước, được viết

$$
d\eta(t) = u(t)\, d\theta(t).
$$

Khi $u$ được định nghĩa khắp nơi và liên tục, ta thu được định nghĩa đã cho ở Ch. III, §1, No. 4. Hiển nhiên rằng nếu $u_1$ và $u_2$ đều địa phương $\theta$-khả tích, thì $(u_1 + u_2) \cdot \theta = u_1 \cdot \theta + u_2 \cdot \theta$. Tương tự, nếu $\theta_1$ và $\theta_2$ là hai phép đo trên $T$, và nếu $u$ là một hàm địa phương khả tích đối với $\theta_1$ và $\theta_2$, thì $u$ địa phương khả tích đối với $\theta_1 + \theta_2$ và ta có $u \cdot (\theta_1 + \theta_2) = u \cdot \theta_1 + u \cdot \theta_2$.

Từ nay về sau ta sẽ chỉ xét trường hợp các hàm được định nghĩa khắp nơi; phần mở rộng sang các hàm được định nghĩa địa phương hầu khắp nơi, điều này luôn hiển nhiên, để lại cho bạn đọc.

Mệnh đề sau cho phép, trong phần lớn các trường hợp, rút về trường hợp các phép đo dương từ trường hợp các phép đo phức:

#### Mệnh đề 2 {#int-v-s5-prop-2 .statement}

*Cho $\theta$ là một phép đo phức, và $u$ là một hàm phức địa phương $\theta$-khả tích; khi đó*

$$
|u \cdot \theta| = |u| \cdot |\theta|.
$$

Ta bắt đầu với một kết quả phụ trợ:

#### Bổ đề 1 {#int-v-s5-lem-1 .statement}

— *Cho $\theta$ là một phép đo phức, và cho $f$ là một phần tử của $\overline{\mathcal{L}}^1_C(T, \theta)$. Khi đó*

$$
\langle|\theta|, |f|\rangle = \sup_{c \in \mathcal{K}_1} |\langle\theta, cf\rangle| = \sup_{c \in \mathcal{B}_1} |\langle\theta, cf\rangle|,
$$

*trong đó $\mathcal{K}_1$ (tương ứng $\mathcal{B}_1$) ký hiệu tập hợp các hàm phức $c$, liên tục với giá compact (tương ứng Borel), sao cho $|c| \leq 1$.

Trước hết xét trường hợp $f \in \mathcal{K}(T; \mathbf{C})$. Hiển nhiên

$$
\sup_{c \in \mathcal{K}_1} |\langle\theta, cf\rangle| \leq \sup_{c \in \mathcal{B}_1} |\langle\theta, cf\rangle| \leq \langle|\theta|, |f|\rangle
$$

(Ch. IV, §4, No. 2, Mệnh đề 2). Mặt khác, cho $g$ là một phần tử của $\mathcal{K}(T; \mathbf{C})$ sao cho $|g| \leq |f|$; $g$ là giới hạn đều của một dãy $(g_n)$ gồm các phần tử của $\mathcal{K}(T; \mathbf{C})$ có giá được chứa trong tập mở $U$ gồm các $t$ sao cho $f(t) \neq 0$, và rõ ràng có thể giả sử rằng $|g_n| \leq |f|$ với mọi $n$. Đặt $c_n(t) = g_n(t)/f(t)$ với $t \in U$, $c_n(t) = 0$ với $t \notin U$; khi đó $c_n \in \mathcal{K}_1$, $g = \lim_{n \to \infty} c_n f$, vì thế $|\langle\theta, g\rangle| = \lim_{n \to \infty} |\langle\theta, c_n f\rangle|$, và cuối cùng

$$
\sup_{|g| \leq |f|, g \in \mathcal{K}(T; \mathbf{C})} |\langle\theta, g\rangle| \leq \sup_{c \in \mathcal{K}_1} |\langle\theta, cf\rangle|.
$$

Người ta kết luận bằng cách nhận thấy rằng vế thứ nhất của bất đẳng thức này bằng $\langle |\theta|, |f| \rangle$ (Ch. III, §1, No. 6, công thức (12)).

Tiếp theo, ký hiệu bởi $f$ một phần tử của $\overline{\mathcal{L}}_C^1(\theta)$, và ta hãy chứng minh rằng (4) lại đúng: chỉ cần kiểm tra rằng ba vế của quan hệ này phụ thuộc liên tục vào $f$ theo tôpô của $\overline{\mathcal{L}}_C^1(\theta)$, vì chúng trùng nhau trên không gian con trù mật $\mathcal{K}(T; \mathbf{C})$. Điều này suy ra ngay từ các bất đẳng thức sau, trong đó $f$ và $f'$ ký hiệu các phần tử của $\overline{\mathcal{L}}_C^1(\theta)$:

$$
|\langle |\theta|, |f| \rangle - \langle |\theta|, |f'| \rangle| \leq \langle |\theta|, |f - f'| \rangle = \overline{N}_1(f - f')
$$
$$
|\langle \theta, cf \rangle - \langle \theta, cf' \rangle| \leq \langle |\theta|, |c||f - f'| \rangle \leq \overline{N}_1(f - f')
$$

với mọi $c \in \mathcal{B}_1$. Bổ đề như vậy đã được thiết lập.

Chuyển sang chứng minh Mệnh đề 2, ta áp dụng bổ đề cho hàm số $uh$, trong đó $h$ thuộc $\mathcal{K}_+(T)$. Suy ra:

$$
\langle |\theta|, |uh| \rangle = \sup_{c \in \mathcal{K}_1} |\langle \theta, cuh \rangle| = \sup_{c \in \mathcal{K}_1} |\langle u \cdot \theta, ch \rangle| = \langle |u \cdot \theta|, h \rangle .
$$

Tuy nhiên, vế thứ nhất cũng bằng

$$
\langle |\theta|, |u|h \rangle = \langle |u| \cdot |\theta|, h \rangle .
$$

Hai độ đo $|u| \cdot |\theta|$ và $|u \cdot \theta|$ vì thế bằng nhau.

#### Hệ quả {#int-v-s5-n2-cor-1 .statement}

*Cho $g_1$ và $g_2$ là hai hàm số thực địa phương $\mu$-tích phân; khi đó*

$$
\inf(g_1 \cdot \mu, g_2 \cdot \mu) = \inf(g_1, g_2) \cdot \mu ; \quad \sup(g_1 \cdot \mu, g_2 \cdot \mu) = \sup(g_1, g_2) \cdot \mu .
$$

*Đặc biệt, nếu $g$ là một hàm số thực địa phương $\mu$-tích phân, thì*

$$
(g \cdot \mu)^+ = g^+ \cdot \mu ; \quad (g \cdot \mu)^- = g^- \cdot \mu .
$$

Điều này suy ra ngay từ Mệnh đề 2 và các công thức (6) của Ch. II, §1, No. 1.

### 3. Tích phân đối với một độ đo được xác định bởi một mật độ

*Trong các mệnh đề của tiểu mục này, $g$ ký hiệu một hàm số thực dương, xác định mọi nơi và địa phương $\mu$-tích phân, $\theta$ ký hiệu một độ đo phức, và $u$ một hàm phức địa phương $\theta$-tích phân.*

Những nhận xét ở No. 2 cho thấy các kết quả của §4 áp dụng được cho độ đo $\nu = g \cdot \mu = \int g(t) \varepsilon_t \, d\mu(t)$ (mặc dù độ đo $g(t) \varepsilon_t$ không được xác định trừ khi $g(t) \neq +\infty$). Ta do đó thu được mệnh đề sau:

#### Mệnh đề 3 {#int-v-s5-prop-3 .statement}

*Với mọi hàm số trị số $f \geqslant 0$ xác định trên $T$,*

$$
\int^\bullet f \, d\nu = \int^\bullet (f g) \, d\mu .
$$

Điều này suy ra từ Định lý 1 của §4, No. 2.

#### Hệ quả 1 {#int-v-s5-prop-3-cor-1 .statement}

*Để một hàm số $\mathbf{f}$, với giá trị trong một không gian Banach hoặc trong $\overline{\mathbf{R}}$, là không đáng kể địa phương đối với độ đo $u \cdot \theta$, cần và đủ rằng $u \mathbf{f}$ là không đáng kể địa phương đối với $\theta$. \*

Nói rằng $\mathbf{f}$ (tương ứng $u \mathbf{f}$) là không đáng kể địa phương đối với $u \cdot \theta$ (tương ứng đối với $\theta$) là tương đương với nói rằng $|\mathbf{f}|$ (tương ứng $|u| \cdot |\mathbf{f}|$) là không đáng kể địa phương đối với $|u \cdot \theta|$ (tương ứng đối với $|\theta|$). Do đó, theo Mệnh đề 2 của No. 2, ta quy về trường hợp $\mathbf{f}, u, \theta$ là dương; mệnh đề khi đó suy ra ngay từ Mệnh đề 3.

#### Hệ quả 2 {#int-v-s5-prop-3-cor-2 .statement}

*Cho $u_1$ và $u_2$ là hai hàm phức khả tích địa phương theo $\theta$. Để $u_1 \cdot \theta = u_2 \cdot \theta$, cần và đủ rằng $u_1$ và $u_2$ bằng nhau hầu khắp nơi địa phương.*

Ta ngay lập tức quy về việc chứng minh rằng $u \cdot \theta = 0$ kéo theo rằng $u(t) = 0$ hầu khắp nơi địa phương; nhưng $u \cdot \theta = 0$ có nghĩa là hàm 1 là không đáng kể địa phương đối với độ đo $u \cdot \theta$. Khi đó áp dụng Hệ quả 1.

#### Hệ quả 3 {#int-v-s5-prop-3-cor-3 .statement}

*Cho $u$ là một hàm phức khả tích địa phương đối với độ đo dương $\mu$. Để $u \cdot \mu$ là một độ đo dương, cần và đủ rằng $u(t) \geqslant 0$ hầu khắp nơi địa phương.*

Vì, $u \cdot \mu$ là dương khi và chỉ khi $u \cdot \mu = |u \cdot \mu| = |u| \cdot \mu$ (Mệnh đề 2), và điều này tương đương với $u = |u|$ hầu khắp nơi địa phương (Hệ quả 2).

#### Mệnh đề 4 {#int-v-s5-prop-4 .statement}

*Để một ánh xạ $f$ của $T$ vào một không gian tôpô $G$ là đo được đối với độ đo $u \cdot \theta$, cần và đủ rằng hạn chế của $f$, trên tập $\theta$-đo được $S$ của các $t$ sao cho $u(t) \neq 0$, là $\theta$-đo được.*

Khi $u$ và $\theta$ là dương, điều này suy ra ngay từ Mệnh đề 3 của §4, No. 3. Kết quả sau đó mở rộng sang trường hợp $u$ và $\theta$ là phức nhờ Mệnh đề 2.

#### Hệ quả {#int-v-s5-n3-cor-1 .statement}

*Cho $\mathbf{f}$ là một hàm số xác định trên $T$, với giá trị trong một không gian Banach $F$ hoặc trong $\overline{\mathbf{R}}$. Để $\mathbf{f}$ là $(u \cdot \theta)$-đo được, cần và đủ rằng $u \mathbf{f}$ là $\theta$-đo được.*

Vì, $u \mathbf{f}$ là mở rộng bởi 0 của $(u \mathbf{f})|S$ lên $T$.

#### Định lý 1 {#int-v-s5-thm-1 .statement}

*Cho $\mathbf{f}$ là một hàm xác định trên $T$, với giá trị trong một không gian Banach $F$ hoặc trong $\overline{\mathbf{R}}$. Để $\mathbf{f}$ khả tích hầu khắp nơi đối với* độ đo $\eta = u \cdot \theta$, cần và đủ rằng $uf$ khả tích hầu khắp nơi theo $\theta$, trong trường hợp đó

$$
\int f \, d\eta = \int (uf) \, d\theta .
$$

Giả sử thêm rằng $u$ liên tục và $u(t) \neq 0$ với mọi $t \in T$; khi đó $f$ khả tích đối với độ đo $\eta$ khi và chỉ khi $uf$ khả tích đối với $\theta$.

Trường hợp $u$ và $\theta$ dương suy ra ngay từ ĐL. 2 của §4, No. 4. Mệnh đề đầu tiên và mệnh đề cuối cùng của phát biểu khi đó suy ra ngay, vì $f$ khả tích hầu khắp nơi (tương ứng khả tích) đối với $\eta = u \cdot \theta$ khi và chỉ khi nó khả tích hầu khắp nơi (tương ứng khả tích) theo $|\eta| = |u| \cdot |\theta|$. Cuối cùng, giả sử $f$ khả tích hầu khắp nơi đối với $\eta$ (suy ra đối với $|\eta|$); ta dùng phép phân tích (2): $f$ khả tích hầu khắp nơi đối với từng độ đo $\eta_{ij} = g_i \cdot \mu_j$ ($i = 1, 2, 3, 4,\ j = 1, 2, 3, 4$), vì các độ đo này $\leq |\eta|$. Ta có

$$
\int f \, d\eta_{ij} = \int g_i f \, d\mu_j .
$$

Công thức (6) suy ra ngay từ đây.

#### Hệ quả {#int-v-s5-n3-cor-2 .statement}

Để độ đo $u \cdot \theta$ bị chặn, cần và đủ rằng $u$ khả tích hầu khắp nơi theo $\theta$.

#### Ví dụ {#int-v-s5-n3-exa-1 .statement}

Cho $A$ là một tập con của $T$; để $\varphi_A$ khả tích địa phương theo $\mu$, cần và đủ rằng $A$ là $\mu$-đo được. Giả sử điều kiện đó được thỏa mãn, đặt $\nu = \varphi_A \cdot \mu$; với mọi hàm số $f \geq 0$ xác định trên $T$, ta có

$$
\int^\bullet f \, d\nu = \int^\bullet f \varphi_A \, d\mu ,
$$

đại lượng này cũng được ký hiệu là $\int_A^\bullet f \, d\mu$ (xem Ch. IV, §5, No. 6). Để một ánh xạ $g$ từ $T$ vào một không gian tôpô $G$ là $\nu$-đo được, cần và đủ rằng hạn chế của $g$ trên $A$ là $\mu$-đo được. Để một ánh xạ $f$ từ $T$ vào một không gian Banach $F$ hoặc vào $\overline{\mathbf{R}}$ là khả tích hầu khắp nơi theo $\nu$, cần và đủ rằng $f \varphi_A$ khả tích hầu khắp nơi theo $\mu$, trong trường hợp đó

$$
\int f \, d\nu = \int f \varphi_A \, d\mu ,
$$

### 4. Sự tương thích của tích đối với các phép toán thông thường

#### Mệnh đề 5 {#int-v-s5-prop-5 .statement}

một biểu thức cũng được ký hiệu bởi $\int_A f \, d\mu$. Chú ý rằng nếu hai ánh xạ từ $T$ vào $G$ (tương ứng $F, \overline{\mathbf{R}}$) trùng nhau trên $A$, thì để một trong hai ánh xạ ấy là $\nu$-đo được (tương ứng khả tích thiết yếu theo $\nu$), điều kiện cần và đủ là ánh xạ kia cũng như vậy. Nếu bây giờ $g$ là một ánh xạ vào $G$ của một tập con tùy ý $B \supset A$ của $T$, ta nói rằng $g$ là $\mu$-đo được *trên* $A$ nếu một mở rộng tùy ý lên $T$ của hạn chế của $g$ lên $A$ là $\nu$-đo được, điều này tương đương với việc nói rằng hạn chế của $g$ lên $A$ là $\mu$-đo được. Một ánh xạ $f$ của $B$ vào một không gian Banach $F$, hoặc vào $\overline{\mathbf{R}}$, được gọi là *khả tích một cách thiết yếu* theo $\mu$ *trên* $A$ nếu một mở rộng $\overline{f}$ lên $T$ của hạn chế của $f$ lên $A$ là khả tích một cách thiết yếu theo $\nu$; khi đó ta đặt
$$
\int_A f \, d\mu = \int_A \overline{f} \, d\mu = \int \overline{f} \varphi_A \, d\mu,
$$
và ta nói rằng $\int_A f \, d\mu$ là *tích phân của* $f$ *trên* $A$ (hay *mở rộng đến* $A$). Nếu $f$ là một hàm số $\geqslant 0$ xác định trên $B \supset A$, ta định nghĩa tương tự $\int_A^* f \, d\mu$ và $\int_A^\bullet f \, d\mu$. Cuối cùng, một hàm số $g$ xác định trên $B \supset A$ được gọi là *khả tích địa phương* theo $\mu$ *trên* $A$ nếu một mở rộng $\overline{g}$ lên $T$ của hạn chế của $g$ lên $A$ là khả tích địa phương theo $\nu$: điều này tương đương với việc nói rằng, với mọi tập con compact $K$ của $T$, $\overline{g} \varphi_{K \cap A}$ là $\mu$-khả tích.

*Cho* $(\lambda_\alpha)_{\alpha \in A}$ *là một họ các độ đo dương trên* $T$, *có hướng theo quan hệ* $\leqslant$, *thừa nhận trong* $\mathcal{M}(T)$ *một supremum* $\lambda$. *Để một hàm số trị dương* $g$ *địa phương khả tích theo* $\lambda$, *cần và đủ rằng* $g$ *địa phương khả tích theo* $\lambda_\alpha$ *với mọi* $\alpha \in A$ *và rằng họ* $(g \cdot \lambda_\alpha)$ *bị chặn trên trong* $\mathcal{M}(T)$; *trong trường hợp này,
$$
g \cdot \lambda = \sup_{\alpha \in A} g \cdot \lambda_\alpha.
$$
Rõ ràng điều kiện là cần. Ngược lại, giả sử rằng $g$ địa phương khả tích đối với từng độ đo $\lambda_\alpha$ và rằng họ $(g \cdot \lambda_\alpha)_{\alpha \in A}$ bị chặn trên; ký hiệu supremum của nó là $\lambda'$. Khi đó hàm $g$ là $\lambda$-đo được (§ 1, No. 4, Hệ quả 2 của Mệnh đề 11); hơn nữa, với mọi hàm $h \in \mathcal{K}_+(T)$,
$$
\int^\bullet (hg) \, d\lambda = \sup_{\alpha \in A} \int^\bullet (hg) \, d\lambda_\alpha = \sup_{\alpha \in A} \int^\bullet h \, d(g \cdot \lambda_\alpha) = \int^\bullet h \, d\lambda'
$$
(§ 1, No. 4, Mệnh đề 11). Điều này trước hết suy ra rằng thành phần thứ nhất là hữu hạn với mọi $h$, do đó $g$ địa phương khả tích theo $\lambda$; vì vậy ký hiệu $\int^\bullet$ có thể được thay bằng $\int$, và công thức có thể viết là $\int h \, d(g \cdot \lambda) = \int h \, d\lambda'$. Suy ra $g \cdot \lambda = \lambda'$, và điều đó hoàn tất chứng minh.

#### Hệ quả {#int-v-s5-n4-cor-1 .statement}

— Giả sử rằng $\mu$ là tổng của một họ $(\mu_\alpha)_{\alpha \in A}$ các độ đo trên T. Để một hàm số trị dương g xác định trên T địa phương khả tích theo $\mu$, cần và đủ rằng g địa phương khả tích theo $\mu_\alpha$ với mọi $\alpha \in A$ và rằng họ $(g \cdot \mu_\alpha)_{\alpha \in A}$ là khả tổng. Trong trường hợp này,

$$
g \cdot \mu = \sum_{\alpha \in A} g \cdot \mu_\alpha.
$$

Cho $(g_\alpha)_{\alpha \in A}$ là một họ các hàm số trị dương $\mu$-đo được xác định trên T. Gọi $S_\alpha$ là tập hợp các $t \in T$ sao cho $g_\alpha(t) \neq 0$. Ta sẽ nói rằng họ $(g_\alpha)$ là *địa phương đếm được* nếu họ $(S_\alpha)$ là địa phương đếm được (Ch. IV, §5, No. 9); điều đó tương đương với việc nói rằng, với mọi tập compact K trong T, tập các $\alpha \in A$ sao cho $g_\alpha|K$ không đồng nhất bằng không là đếm được.

#### Mệnh đề 6 {#int-v-s5-prop-6 .statement}

— Cho $(g_\alpha)_{\alpha \in A}$ là một họ đếm được địa phương các hàm số trị dương địa phương khả tích theo $\mu$ xác định trên T. Để hàm $g = \sum_{\alpha \in A} g_\alpha$ địa phương khả tích theo $\mu$, cần và đủ rằng họ các độ đo $(g_\alpha \cdot \mu)_{\alpha \in A}$ là khả tổng, trong trường hợp đó

$$
g \cdot \mu = \sum_{\alpha \in A} g_\alpha \cdot \mu.
$$

It là rõ ràng rằng $g$ là $\mu$-đo được (Chương IV, §5, No. 2, Mệnh đề 4 và No. 4, Hệ quả 1 của Định lý 2). Để $g$ khả tích địa phương theo $\mu$, do đó cần và đủ rằng $\mu^\bullet(gf)$ hữu hạn với mọi $f \in \mathcal{H}_+(T)$. Bây giờ, vì tập các $\alpha \in A$ sao cho $g_\alpha f \neq 0$ là đếm được, ta có $\mu^\bullet(gf) = \sum_{\alpha \in A} \mu^\bullet(g_\alpha f)$ (§1, No. 1, Hệ quả của Mệnh đề 2). Đặt $\nu_\alpha = g_\alpha \cdot \mu$; điều kiện $\mu^\bullet(gf) < +\infty$ tương đương với điều kiện $\sum_{\alpha \in A} \nu_\alpha(f) < +\infty$: nói cách khác, $g$ khả tích địa phương theo $\mu$ khi và chỉ khi họ $(\nu_\alpha)$ khả tổng. Ký hiệu tổng của họ này là $\nu$, phép tính trên cho đẳng thức $\nu(f) = \mu^\bullet(gf)$, đẳng thức này tương đương với (8).

#### Hệ quả {#int-v-s5-n4-cor-2 .statement}

— Cho $(g_\alpha)$ là một dãy các hàm số thực khả tích địa phương theo $\mu$, sao cho dãy các độ đo $g_n \cdot \mu$ là tăng. Để dãy này có một cận trên trong không gian vectơ có thứ tự $\mathcal{M}(T)$ của các độ đo thực trên T, cần và đủ rằng hàm số $g = \sup g_n$ khả tích địa phương theo $\mu$; khi đó cận trên đúng trong $\mathcal{M}(T)$ của dãy $(g_n \cdot \mu)$ là độ đo $g \cdot \mu$.

Chỉ cần áp dụng Mệnh đề 6 cho các hàm số (dương địa phương hầu khắp nơi) $g'_n = g_{n+1} - g_n$.

#### Mệnh đề 7 {#int-v-s5-prop-7 .statement}

— Cho X là một không gian compact địa phương đếm được ở vô cùng, và cho $t \mapsto \lambda_t$ là một ánh xạ $\mu$-thích hợp của T vào $\mathcal{M}_+(X)$.

Cho $g$ là một hàm số dương xác định trên $X$, khả tích địa phương đối với độ đo $\nu = \int \lambda_t d\mu(t)$. Khi đó tập các $t \in T$ sao cho $g$ không khả tích địa phương theo $\lambda_t$ là không đáng kể địa phương đối với $\mu$, ánh xạ $t \mapsto g \cdot \lambda_t$ (được định nghĩa địa phương $\mu$-hầu khắp nơi) là $\mu$-thích hợp, và

$$
g \cdot \nu = \int (g \cdot \lambda_t) d\mu(t).
$$

Let $(K_n)_{n \in \mathbf{N}}$ be an increasing sequence of compact subsets of $X$ whose interiors cover $X$; if $\eta$ is any positive measure on $X$, to say that $g$ is locally $\eta$-integrable is equivalent to saying that $g \varphi_{K_n}$ is $\eta$-integrable for every $n$. Now let $H_n$ be the set of $t \in T$ such that $g \varphi_{K_n}$ is not $\lambda_t$-integrable, and let $H = \bigcup_n H_n$; since $H_n$ is locally $\mu$-negligible for all $n$ (§ 3, No. 3, Th. 1), the same is true of $H$, which establishes the first assertion of the statement. Replacing $\lambda_t$ by 0 for $t$ in $H$ (which does not change the measure $\nu$), we can suppose that $g$ is locally $\lambda_t$-integrable for every $t \in T$. For every $\nu$-measurable positive function $h$ defined on $X$, we have, by Prop. 3 and by Prop. 5 of § 3, No. 2,

$$
\int^\bullet h d(g \cdot \nu) = \int^\bullet (gh) d\nu = \int^\bullet d\mu(t) \int^\bullet (gh) d\lambda_t = \int^\bullet d\mu(t) \int^\bullet h d(g \cdot \lambda_t).
$$

This formula and Prop. 5 of § 3, No. 2 first show (on taking $h \in \mathcal{K}_+(X)$) that the mapping $t \mapsto g \cdot \lambda_t$ is scalarly essentially $\mu$-integrable, and that its integral is $g \cdot \nu$; in other words, the relation (9) holds. Next, let us replace $\mu$ by a positive measure $\mu' \leq \mu$, and let us take for $h$ a positive lower semi-continuous function: it follows at once from these relations that $t \mapsto g \cdot \lambda_t$ is $\mu$-adequate (§ 3, No. 1, Def. 1).

#### Mệnh đề 8 {#int-v-s5-prop-8 .statement}

*Cho $\theta$ là một độ đo phức trên $T$, $g_1$ là một hàm phức khả tích địa phương theo $\theta$, $\theta_1$ là độ đo $g_1 \cdot \theta$. Để một hàm phức $g_2$ xác định trên $T$ khả tích địa phương theo $\theta_1$, cần và đủ rằng $g_2 g_1$ khả tích địa phương theo $\theta$, trong trường hợp đó*

$$
g_2 \cdot \theta_1 = g_2 \cdot (g_1 \cdot \theta) = (g_2 g_1) \cdot \theta
$$
('công thức tính kết hợp').

Theo hệ quả của Prop. 4, nói rằng $g_2$ là $\theta_1$-đo được là tương đương với nói rằng $g_2 g_1$ là $\theta$-đo được. Giả sử điều kiện này được thỏa mãn. Với mọi hàm $f \in \mathcal{K}_+(T)$, nhờ các Mệnh đề 2 và 3, ta có

$$
\int^\bullet |g_2| f d|\theta_1| = \int^\bullet |g_2| f |g_1| d|\theta| = \int^\bullet |g_2 g_1| f d|\theta|.
$$

To nói rằng $g_2$ là khả tích địa phương theo $\theta_1$ do đó tương đương với việc nói rằng $g_2 g_1$ là khả tích địa phương theo $\theta$. Giả sử điều kiện này được thỏa mãn, theo Định lý 1 ta có

$$
\int f \, d(g_2 \cdot \theta_1) = \int f g_2 \, d\theta_1 = \int f g_2 g_1 \, d\theta = \int f \, d(g_2 g_1 \cdot \theta),
$$

một công thức tương đương với (10).

### 5. Đặc trưng hóa các độ đo với cơ sở $\mu$

#### Định lý 2 (Lebesgue–Nikodym) {#int-v-s5-thm-2 .statement}

— *Cho $\mu$ và $\nu$ là hai độ đo dương trên $T$. Các tính chất sau là tương đương:*

1) $\nu$ *là một độ đo với cơ sở $\mu$*.
2) *Mọi tập địa phương $\mu$-không đáng kể đều là địa phương $\nu$-không đáng kể*.
3) *Mọi tập compact $\mu$-không đáng kể đều là $\nu$-không đáng kể*.

Rõ ràng 1) kéo theo 2) (Hệ quả 1 của Mệnh đề 3), và 2) kéo theo 3). Ta sẽ chứng minh rằng 3) kéo theo 1). Trước hết ta nhận xét rằng nếu điều kiện 3) được thỏa mãn thì mọi tập $A$ vừa *khả đo được mọi nơi* vừa địa phương $\mu$-không đáng kể đều địa phương $\nu$-không đáng kể; thật vậy, $\nu^\bullet(A) = \sup \nu(K)$, trong đó $K$ chạy qua tập hợp các tập compact được chứa trong $A$ (§ 1, No. 3, Mệnh đề 10, a) và Ch. IV, § 4, No. 6, Hệ quả 2 của Định lý 4). Tiếp theo, ta sẽ thiết lập hai bổ đề.

#### Bổ đề 2 {#int-v-s5-lem-2 .statement}

— *Cho $\alpha$ là một độ đo dương bị chặn trên $T$, và $\beta$ là một độ đo thực trên $T$ sao cho $|\beta| \leq M \alpha$, trong đó $M$ là một hằng số dương. Khi đó, tồn tại một hàm thực $u$, khả tích theo $\alpha$, sao cho $\beta = u \cdot \alpha$*.

Cho $g$ là một phần tử của không gian $\mathcal{L}_\mathbf{R}^2(T, \alpha)$; $g$ là $\beta$-đo được và $\int^\bullet |g|^2 \, d|\beta| \leq M \int^\bullet |g|^2 \, d\alpha < +\infty$. Vì vậy hàm $g$ thuộc $\mathcal{L}^2(T, |\beta|)$, và cũng thuộc $\mathcal{L}^1(T, |\beta|)$ vì $\beta$ bị chặn. Theo bất đẳng thức Cauchy–Schwarz,

$$
|\beta(g)|^2 \leq \left( \int |g| \, d|\beta| \right)^2 \leq \left( \int d|\beta| \right) \left( \int |g|^2 \, d|\beta| \right) \leq M^2 \alpha(1) \, \alpha(|g|^2).
$$

Ánh xạ $g \mapsto \beta(g)$ do đó là một dạng tuyến tính liên tục trên $\mathcal{L}^2(T, \alpha)$. Vì không gian Hausdorff gắn với $\mathcal{L}^2(T, \alpha)$ là một không gian Hilbert, nên tồn tại (TVS, Ch. V, § 1, No. 7, Định lý 3) một hàm thực $u \in \mathcal{L}^2(T, \alpha)$, do đó cũng thuộc $\mathcal{L}^1(T, \alpha)$, sao cho $\beta(g) = \alpha(ug)$ với mọi $g \in \mathcal{L}^2(T, \alpha)$. Áp dụng quan hệ này cho $g \in \mathcal{K}(T)$, ta thấy rằng $\beta = u \cdot \alpha$.

#### Bổ đề 3 {#int-v-s5-lem-3 .statement}

— *Giả sử độ đo dương $\nu$ sao cho mọi tập compact $\mu$-không đáng kể đều $\nu$-không đáng kể. Gọi $\mathfrak{K}$ là tập hợp các tập compact $K$ của $T$ có tính chất sau:*

(11) Tồn tại một hằng số $M \geq 0$ sao cho $\varphi_K \cdot \nu \leq M \varphi_K \cdot \mu$.
Khi đó tập $\mathcal{K}$ trù mật trong $T$.

Nếu $K$ thỏa mãn (11), và nếu $A$ là một tập Borel được chứa trong $K$, thì suy ra ngay từ Mệnh đề 8 rằng $\varphi_A \cdot \nu \leq M \varphi_A \cdot \mu$; từ đó, ta suy ra rằng hợp của hai phần tử $K, K'$ của $\mathcal{K}$ thuộc $\mathcal{K}$ vì $\varphi_{K \cup K'} = \varphi_K + \varphi_A$, trong đó $A = K' \cap \complement K$. Để chứng minh bổ đề, còn lại phải chứng minh rằng mọi tập compact $L$ sao cho $\mu(L) > 0$ đều chứa một tập compact $K \in \mathcal{K}$ sao cho $\mu(K) > 0$ (Ch. IV, §5, No. 8, Mệnh đề 12). Chọn một số $M > \nu(L)/\mu(L)$ và áp dụng Bổ đề 1 cho độ đo dương bị chặn $\alpha = \varphi_L \cdot (\nu + M \mu)$ và độ đo $\beta = \varphi_L \cdot (\nu - M \mu)$. Nếu cần, thay hàm $u$ sao cho $\beta = u \cdot \alpha$ bằng một hàm bằng nó ở mọi nơi trừ một tập $\alpha$-gần như khắp, ta có thể giả sử rằng $u$ là đo được một cách phổ dụng (§3, No. 4, Mệnh đề 7) và bằng không ở ngoài $L$. Tập $H$ gồm các $t \in T$ sao cho $u(t) < 0$, vốn được chứa trong $L$, không thể là không đáng kể theo $\mu$, vì khi đó nó sẽ là không đáng kể theo $\nu$ (theo nhận xét đã nêu ở đầu chứng minh của Định lý 2), do đó là không đáng kể theo $\alpha$, và ta sẽ có $\beta(L) > 0$, điều này mâu thuẫn với việc chọn $M$. Gọi $K$ là một tập compact được chứa trong $H$, sao cho $\mu(K) > 0$; ta sẽ chứng minh rằng $K \in \mathcal{K}$, điều này sẽ hoàn tất chứng minh bổ đề. Theo Mệnh đề 8,

$$
\varphi_K \cdot (\nu - M \mu) = \varphi_K \cdot \beta = \varphi_K \cdot (u \cdot \alpha) = (\varphi_K u) \cdot \alpha .
$$

Hàm $\varphi_K u$ là âm, do đó quả thật ta có $\varphi_K \cdot \nu \leq M \varphi_K \cdot \mu$.

Bây giờ ta hãy hoàn tất chứng minh Định lý 2. Giả sử điều kiện 3) được thỏa và định nghĩa $\mathcal{K}$ như trong Bổ đề 3. Cho $(K_\alpha)_{\alpha \in A}$ là một họ địa phương đếm được các phần tử từng đôi một rời nhau của $\mathcal{K}$, sao cho tập $N = T - \bigcup_{\alpha \in A} K_\alpha$ là không đáng kể theo $\mu$ một cách địa phương (Ch. IV, §5, No. 9, Mệnh đề 14); vì họ $(K_\alpha)$ là địa phương đếm được, nên $N$ là đo được một cách phổ dụng và do đó là không đáng kể theo $\nu$ một cách địa phương. Đặt $\mu_\alpha = \varphi_{K_\alpha} \cdot \mu$, $\nu_\alpha = \varphi_{K_\alpha} \cdot \nu$; vì các hàm $\varphi_{K_\alpha}$ tạo thành một họ địa phương đếm được, có tổng bằng 1 gần như khắp một cách địa phương đối với $\mu$ và đối với $\nu$, Mệnh đề 6 suy ra rằng $\mu = \sum_{\alpha \in A} \mu_\alpha$, $\nu = \sum_{\alpha \in A} \nu_\alpha$. Mặt khác, theo định nghĩa của $\mathcal{K}$, với mọi $\alpha$ tồn tại một hằng số $M_\alpha$ sao cho $\nu_\alpha \leq M_\alpha \mu_\alpha$; do đó Bổ đề 2 suy ra sự tồn tại của một hàm $g_\alpha$, mà ta có thể giả sử bằng không ở ngoài $K_\alpha$ và dương (Hệ quả 3 của Mệnh đề 3), sao cho $\nu_\alpha = g_\alpha \cdot \mu_\alpha$. Do đó (No. 4, Mệnh đề 8)

$$
\nu_\alpha = g_\alpha \cdot \mu_\alpha = g_\alpha \cdot (\varphi_{K_\alpha} \cdot \mu) = (g_\alpha \varphi_{K_\alpha}) \cdot \mu = g_\alpha \cdot \mu .
$$

Set $g = \sum_{\alpha \in A} g_\alpha$; vì họ $(g_\alpha)$ là địa phương đếm được và họ $(\nu_\alpha)$ là khả tổng, Mệnh đề 6 suy ra rằng $g$ là địa phương $\mu$-khả tích, và rằng $\nu = g \cdot \mu$, điều đó chứng minh định lý.

#### Hệ quả 1 {#int-v-s5-thm-2-cor-1 .statement}

— Cho $\mathcal{N}$ là một tập các độ đo dương có cơ sở $\mu$, có supremum $\nu$ trong $\mathcal{M}(T)$; khi đó $\nu$ là một độ đo có cơ sở $\mu$.

Hệ quả của Mệnh đề 2 cho phép quy về trường hợp $\mathcal{N}$ là một tập có hướng tăng. Với mọi tập địa phương $\mu$-không đáng kể $A$ ta khi đó có, theo Mệnh đề 11 của §1, No. 4,

$$
\nu^\bullet(A) = \sup_{\lambda \in \mathcal{N}} \lambda^\bullet(A) = 0.
$$

Do đó Định lý 2 suy ra rằng $\nu$ là một độ đo có cơ sở $\mu$.

#### Hệ quả 2 {#int-v-s5-thm-2-cor-2 .statement}

— Cho $\nu$ là một độ đo thực trên $T$. Để $\nu$ thuộc vào dải được sinh bởi $\mu$ trong không gian có thứ tự theo dàn đầy đủ $\mathcal{M}(T)$ (Ch. II, §1, No. 5), điều kiện cần và đủ là $\nu$ là một độ đo có cơ sở $\mu$.

Xét $\nu^+$ và $\nu^-$, ta ngay lập tức quy về trường hợp một độ đo dương $\nu$ (No. 2, Hệ quả của Mệnh đề 2). Khi đó đặt $\nu_n = \inf(n\mu, \nu)$; $\nu$ thuộc vào dải được sinh bởi $\mu$ khi và chỉ khi $\nu = \sup_n \nu_n$ (Ch. II, §1, No. 5, Hệ quả của Mệnh đề 6). Bây giờ $\nu_n$, vì bị chặn trên bởi $n\mu$, là một độ đo có cơ sở $\mu$ theo Định lý 2; do đó quan hệ $\nu = \sup_n \nu_n$ suy ra rằng $\nu$ là một độ đo có cơ sở $\mu$ (Hệ quả 1). Ngược lại, giả sử rằng $\nu$ là một độ đo có cơ sở $\mu$: $\nu = g \cdot \mu$, trong đó $g$ là địa phương $\mu$-khả tích và dương. Khi đó $\nu_n = \inf(g, n) \cdot \mu$ (Hệ quả của Mệnh đề 2), và từ định lý của Lebesgue (Ch. IV, §4, No. 3, Mệnh đề 4) suy ra ngay rằng $\nu = \sup_n \nu_n$.

#### Hệ quả 3 {#int-v-s5-thm-2-cor-3 .statement}

— Cho $\theta$ là một độ đo phức; tồn tại một hàm đo được phổ quát $v$, với $|v| = 1$, sao cho $\theta = v \cdot |\theta|$, $|\theta| = \overline{v} \cdot \theta$.

Viết $\theta = \theta_1 - \theta_2 + i(\theta_3 - \theta_4)$, trong đó $\theta_1 = (\Re \theta)^+$, $\theta_2 = (\Re \theta)^-$, $\theta_3 = (\Im \theta)^+$, $\theta_4 = (\Im \theta)^-$; các độ đo dương $\theta_i$ ($i = 1, 2, 3, 4$), bị chặn trên bởi $|\theta|$ (Ch. III, §1, No. 6, công thức (17)), là các độ đo có cơ sở $|\theta|$ theo Định lý 2. Suy ra tồn tại một hàm địa phương $|\theta|$-khả tích $v$ sao cho $\theta = v \cdot |\theta|$. Mệnh đề 2 khi đó cho hệ thức $|\theta| = |v| \cdot |\theta|$, điều này suy ra rằng $|v| = 1$ địa phương $|\theta|$-hầu khắp nơi (Hệ quả 2 của Mệnh đề 3). Cuối cùng, theo Mệnh đề 8, $\overline{v} \cdot \theta = (v \overline{v}) \cdot |\theta| = |\theta|$. Vì hàm $v$ chỉ được xác định tới một hàm địa phương $|\theta|$-không đáng kể, ta có thể giả sử rằng $v$ là đo được phổ dụng (§3, No. 4, Mệnh đề 7) và rằng $|v| = 1$ mọi nơi.

#### Nhận xét 1 {#int-v-s5-n5-rem-1 .statement}

Giả sử rằng $\lambda$ là một độ đo dương, rằng $v$ là một hàm đo được theo $\lambda$ sao cho $|v| = 1$ địa phương $\lambda$-hầu khắp nơi (điều này suy ra rằng $v$ là địa phương $\lambda$-khả tích), và rằng $\theta = v \cdot \lambda$. Mệnh đề 2 cho thấy ngay lập tức rằng $\lambda = |\theta|$; nói cách khác, tính chất của mệnh đề trước đặc trưng cho độ đo dương $|\theta|$.

#### Nhận xét 2 {#int-v-s5-n5-rem-2 .statement}

Nếu $|\theta| \leq a \mu$, trong đó $\mu$ là một độ đo dương và $a$ là một số $\geq 0$, thì $\theta$ là một độ đo có cơ sở $\mu$.

#### Hệ quả 4 {#int-v-s5-thm-2-cor-4 .statement}

— Cho $\rho$ và $\theta$ là hai độ đo phức. Để tồn tại một hàm địa phương $\theta$-khả tích $u$ sao cho $\rho = u \cdot \theta$, điều kiện cần và đủ là mọi tập compact $\theta$-không đáng kể đều là $\rho$-không đáng kể.

Điều kiện này hiển nhiên là cần. Chiều ngược lại, giả sử rằng mọi tập compact $\theta$-không đáng kể đều là $\rho$-không đáng kể; Định lý 2 suy ra sự tồn tại của một hàm địa phương $|\theta|$-khả tích $g$ sao cho $|\rho| = g \cdot |\theta|$. Mặt khác, Hệ quả 3 suy ra sự tồn tại của một hàm $v_1$ (tương ứng $v_2$), có giá trị tuyệt đối bằng 1 và đo được đối với độ đo $|\rho|$ (tương ứng $\theta$), sao cho $\rho = v_1 \cdot |\rho|$ (tương ứng $|\theta| = \overline{v_2} \cdot \theta$). Khi đó, theo Mệnh đề 8, $\rho = u \cdot \theta$ với $u = v_1 g \overline{v_2}$.

#### Hệ quả 5 {#int-v-s5-thm-2-cor-5 .statement}

— Cho $\mu$ và $\nu$ là hai độ đo dương trên T. Các điều kiện 1), 2), 3) của Định lý 2 cũng tương đương với các điều kiện sau:

4) Với mọi hàm số thực $f \geq 0$ khả tích theo $\nu$ và với mọi số $\varepsilon > 0$, tồn tại một $\delta > 0$ sao cho các hệ thức $0 \leq h \leq f$ và $\int^* h \, d\mu \leq \delta$ suy ra $\int^* h \, d\nu < \varepsilon$.

5) Với mọi hàm $g \in \mathcal{K}_+(\mathrm{T})$ và mọi số $\varepsilon > 0$, tồn tại một $\delta > 0$ sao cho, với mọi $h \in \mathcal{K}_+(\mathrm{T})$ bị chặn trên bởi $g$ và thỏa mãn $\int h \, d\mu \leq \delta$, ta có $\int h \, d\nu \leq \varepsilon$.

6) Với mọi tập compact $K \subset \mathrm{T}$ và mọi số $\varepsilon > 0$, tồn tại một $\delta > 0$ sao cho các hệ thức $A \subset K$ và $\mu^*(A) \leq \delta$ suy ra $\nu^*(A) \leq \varepsilon$.

Các suy ra 4) $\Rightarrow$ 6) $\Rightarrow$ 3) là hiển nhiên.

Giả sử tồn tại một hàm hữu hạn $k \geq 0$, đo được mọi nơi và khả tích địa phương theo $\mu$, sao cho $\nu = k \cdot \mu$, và hãy chứng minh rằng điều kiện 4) được thỏa mãn. Cho $f$ là một hàm khả tích theo $\nu$ với $f \geq 0$, và cho $\varepsilon > 0$. Với mọi số nguyên $n \geq 0$, đặt $A_n$ là tập các $t \in \mathrm{T}$ sao cho $k(t) \geq n$. Các hàm $f \varphi_{A_n}$ tạo thành một dãy giảm, bị chặn trên bởi $f$ và hội tụ từng điểm về 0, do đó tồn tại một $N$ sao cho $\int f \varphi_{A_N} \, d\nu \leq \varepsilon/2$ (Ch. IV, §4, No. 3, Định lý 4). Nếu $h$ là một hàm trên $\mathrm{T}$ thỏa mãn $0 \leq h \leq f$ và $\int^* h \, d\mu \leq \varepsilon/2N$, thì

$$
\nu^*(h) \leq \nu^*(h \varphi_{A_N}) + \nu^*(h(1 - \varphi_{A_N}))
$$
$$
\leq \nu^*(f \varphi_{A_N}) + \mu^*(h(1 - \varphi_{A_N})k)
$$
$$
\leq \frac{\varepsilon}{2} + N \mu^*(h) \leq \varepsilon.
$$

Vậy ta đã chứng minh rằng các điều kiện 4) và 6) tương đương với các điều kiện của Định lý 2.

Hiển nhiên 4) suy ra 5). Sau cùng, nếu điều kiện 5) được thỏa mãn, thì $\nu$ thuộc dải được sinh bởi $\mu$ (Ch. II, §2, No. 2, Mệnh đề 5), do đó có cơ sở $\mu$ (Hệ quả 2).

#### Chú giải {#int-v-s5-n5-sch-1 .statement}

Với mọi $\dot{f} \in L^1_{\mathrm{loc}}(\mathrm{T}, \mu; \mathbf{R})$, đặt $\varphi(\dot{f}) = f \cdot \mu$, trong đó $f \in \dot{f}$; ánh xạ $\varphi$ là tuyến tính, tăng và đơn ánh (Hệ quả 2 của Mệnh đề 3), và ảnh của nó trong $\mathcal{M}(T)$ là dải B được sinh bởi $\mu$ (Hệ quả 2 của Định lý 2). Do đó ánh xạ $\varphi$ cho phép đồng nhất $L^1_{\text{loc}}(T, \mu; \mathbf{R})$ với một không gian các độ đo thực trên T; vì mọi không gian $L^p_R(T, \mu)$ đều là các không gian con của $L^1_{\text{loc}}(T, \mu; \mathbf{R})$, chúng cũng có thể được đồng nhất với các không gian con của $\mathcal{M}(T)$. Những xét đoán tương tự đúng cho các hàm và độ đo phức. Chú ý rằng ánh xạ $\varphi$ xét ở trên là một đẳng cấu của cấu trúc không gian vectơ có thứ tự của $L^1_{\text{loc}}$ và B, nhưng hiển nhiên không phải là một đẳng cấu đối với các cấu trúc *không gian vectơ tôpô* của các không gian này.

Vì mỗi dải trong một không gian hoàn toàn có thứ tự dàn tự nó cũng là một không gian hoàn toàn có thứ tự dàn (Ch. II, §1, No. 5), ta thấy rằng không gian $L^1_{\text{loc}}$ là *hoàn toàn có thứ tự dàn*; nhưng đáng nhớ rằng cận trên đúng trong $L^1_{\text{loc}}$ của một họ không đếm được $(\dot{f}_\alpha)$ các lớp tương đương chưa nhất thiết trùng với lớp của bao trên của các hàm $f_\alpha$. Tuy nhiên, ta đã thấy rằng đối với một *dãy tăng* $(f_n)$ các hàm khả tích địa phương theo $\mu$ có bao trên $f$ cũng khả tích địa phương theo $\mu$, thì $f \cdot \mu$ là cận trên đúng của dãy các độ đo $(f_n \cdot \mu)$ trong $\mathcal{M}(T)$ (Hệ quả của Mệnh đề 6).

Sau đây là một hệ quả thú vị của Hệ quả 3 của Định lý 2:

#### Mệnh đề 9 {#int-v-s5-prop-9 .statement}

*Cho $\theta$ là một độ đo phức bị chặn; để $\theta$ là một độ đo dương, điều kiện cần và đủ là $\| \theta \| = \theta(1)$.*.

Điều kiện này hiển nhiên là cần. Ngược lại, giả sử $\| \theta \| = \int d\theta$, và ký hiệu bởi $v$ một hàm đo được theo $|\theta|$ có trị tuyệt đối bằng 1 sao cho $\theta = v \cdot |\theta|$. Vì $\| \theta \| = \int d|\theta|$ (Ch. IV, §4, No. 7, Mệnh đề 12) và $\int d\theta = \int v \cdot d|\theta|$ (Định lý 1), giả thiết suy ra rằng $\int (1 - v) \, d|\theta| = 0$ và do đó $\int \mathcal{R}(1 - v) \, d|\theta| = 0$. Hàm $\mathcal{R}(1 - v)$, vì dương, nên bằng không hầu khắp nơi, điều này suy ra rằng $v = 1$ hầu khắp nơi và kết thúc chứng minh.

### 6. Các độ đo tương đương

#### Mệnh đề 10 {#int-v-s5-prop-10 .statement}

*Cho $\mu$ và $\nu$ là hai độ đo dương trên T. Các điều kiện sau là tương đương:
a) Các tập hợp không đáng kể địa phương là như nhau đối với $\mu$ và $\nu$.
b) Các dải do $\mu$ và $\nu$ sinh ra trong $\mathcal{M}(T)$ là trùng nhau.
c) Ta có $\nu = g \cdot \mu$, trong đó $g$ là khả tích địa phương theo $\mu$ và $g(t) > 0$ hầu khắp nơi địa phương đối với $\mu$.*

Các điều kiện a) và b) tương đương theo Hệ quả 2 của Định lý 2 của No. 5. Nếu chúng được thỏa mãn, thì $\nu = g \cdot \mu$ và $\mu = h \cdot \nu$, trong đó $g$ (tương ứng $h$) là dương và khả tích địa phương theo $\mu$ (tương ứng $\nu$). Vì vậy (No. 4, Mệnh đề 8) $hg$ là khả tích địa phương theo $\mu$ và $\mu = (hg) \cdot \mu$. Suy ra (No. 3, Hệ quả 2 của Mệnh đề 3) rằng $hg$ bằng 1 hầu khắp nơi địa phương theo $\mu$, do đó $g(t) > 0$ và $h(t) = 1/g(t)$ hầu khắp nơi địa phương theo $\mu$. Ngược lại, giả sử rằng $\nu = g \cdot \mu$ với $g(t) > 0$ hầu khắp nơi địa phương theo $\mu$;

vì $(1/g)g$ được xác định hầu khắp nơi địa phương và khả tích địa phương theo $\mu$, nên $1/g$ khả tích địa phương theo $\nu$ và $(1/g) \cdot \nu = \mu$ (No. 4, Mệnh đề 8).

#### Định nghĩa 3 {#int-v-s5-def-3 .statement}

*Hai độ đo phức $\theta, \theta'$ trên một không gian compact địa phương $T$ được gọi là tương đương nếu các độ đo $|\theta|$ và $|\theta'|$ thỏa mãn các điều kiện a), b), c) của Mệnh đề 10.*

Vì thế, để $\theta$ và $\theta'$ tương đương thì điều kiện cần và đủ là $|\theta|$ và $|\theta'|$ tương đương.

#### Nhận xét {#int-v-s5-n6-rem-1 .statement}

— Nếu $\mu$ và $\nu$ là hai độ đo dương tương đương thì các hàm khả đo được xác định trên $T$, nhận giá trị trong bất kỳ không gian tôpô nào $G$, là *giống nhau* đối với $\mu$ và $\nu$, như suy ra ngay từ Mệnh đề 4 của No. 3.

#### Mệnh đề 11 {#int-v-s5-prop-11 .statement}

*Cho $\mu$ là một độ đo dương trên $T$. Nếu $T$ đếm được ở vô cực, thì tồn tại một hàm liên tục $h$ sao cho $h(t) > 0$ với mọi $t \in T$ và sao cho độ đo $\nu = h \cdot \mu$ (tương đương với $\mu$) bị chặn.*

Cho $(K_n)$ là một dãy các tập compact lập thành một phủ của $T$ và, với mọi $n$, cho $f_n$ là một hàm trong $\mathcal{H}(T)$ sao cho $0 \leq f_n \leq 1$ và $f_n(t) = 1$ trên $K_n$ (Chương III, §1, No. 2, Bổ đề 1). Cho $(a_n)$ là một dãy các số $> 0$ sao cho $\sum_n a_n < +\infty$; khi đó chuỗi $h = \sum_n a_n f_n$ hội tụ chuẩn trong $T$, do đó $h$ là một hàm liên tục trên $T$, sao cho $h(t) > 0$ với mọi $t \in T$, theo cách dựng. Đặt $\nu = h \cdot \mu$, ta có (Mệnh đề 3 và Chương IV, §1, No. 3, Mệnh đề 13)

$$
\nu^*(1) = \int^* h \, d\mu \leq \sum_n a_n \int f_n \, d\mu .
$$

Lấy chẳng hạn $a_n = 2^{-n} (\int f_n \, d\mu)^{-1}$ khi $\int f_n \, d\mu > 1$, và $a_n = 2^{-n}$ trong trường hợp ngược lại, ta có $\sum_n a_n < +\infty$ và $\nu^*(1) < +\infty$, điều đó chứng minh mệnh đề.

#### Mệnh đề 12 {#int-v-s5-prop-12 .statement}

*Cho $(\mu_n)$ là một dãy các độ đo dương bị chặn trên $T$; tồn tại một độ đo dương bị chặn $\mu$ trên $T$ sao cho quan hệ $\mu^*(N) = 0$ tương đương với «$\mu_n^*(N) = 0$ với mọi $n$»; mỗi độ đo $\mu_n$ có cơ sở là $\mu$. Hơn nữa, nếu $\mu'$ là một độ đo dương thứ hai trên $T$ có tính chất này, thì $\mu$ và $\mu'$ tương đương.*

Phần cuối của mệnh đề suy ra ngay từ Định nghĩa 3. Để chứng minh sự tồn tại của $\mu$, ta có thể chỉ xét trường hợp $\mu_n \neq 0$ với mọi $n$; họ các độ đo $\mu_n / 2^n \| \mu_n \|$ khi đó khả tổng trong $\mathcal{M}(T)$, và tổng của nó $\mu$ thỏa $\| \mu \| \leq 1$. Hơn nữa, vì $\mu_n \leq 2^n \| \mu_n \| \cdot \mu$, quan hệ $\mu(N) = 0$ suy ra rằng $\mu_n(N) = 0$ với mọi $n$; ngược lại, nếu $N$ là một tập không đáng kể đối với mọi $\mu_n$, thì nó là địa phương không đáng kể đối với $\mu$

(§2, No. 2, Hệ quả 2 của Mệnh đề 1), do đó là $\mu$-không đáng kể vì $\mu$ bị chặn (§1, No. 2, Hệ quả 2 của Mệnh đề 7).

### 7. Các độ đo xa lạ

Cho hai độ đo thực $\rho, \sigma$ trên $T$, nhắc lại rằng $\rho$ và $\sigma$ được gọi là xa lạ với nhau nếu $\inf(|\rho|, |\sigma|) = 0$ trong $\mathcal{M}(T)$ (Ch. II, §1, No. 1). Các độ đo thực xa lạ với một độ đo cho trước được biết là tạo thành một dải (Ch. II, §1, No. 5, Định lý 1). Định nghĩa này có thể được mở rộng ngay lập tức sang trường hợp các độ đo phức.

#### Định nghĩa 4 {#int-v-s5-def-4 .statement}

*Người ta nói rằng một độ đo phức $\theta$ trên $T$ được tập trung trên một tập con $M$ của $T$, hay rằng $M$ mang $\theta$, nếu $\mathbf{C}M$ là địa phương không đáng kể đối với $\theta$.*

Tập $M$ mang $\theta$ khi và chỉ khi nó mang $|\theta|$. Tương đương với việc nói rằng $M$ mang $\theta$, hay rằng $M$ là $\theta$-đo được và $\theta = \varphi_M \cdot \theta$. Nếu $\theta$ được tập trung trên $M$, thì mọi độ đo có cơ sở $|\theta|$ đều được tập trung trên $M$.

#### Mệnh đề 13 {#int-v-s5-prop-13 .statement}

*Để hai độ đo phức $\rho$ và $\sigma$ trên $T$ xa lạ với nhau, điều kiện cần và đủ là tồn tại trong $T$ hai tập rời nhau $R$ và $S$ sao cho $\rho$ được tập trung trên $R$ và $\sigma$ trên $S$; $R$ và $S$ có thể được chọn là đo được phổ dụng.*

Đặt $\mu = |\rho|$, $\nu = |\sigma|$, $\lambda = \mu + \nu$; vì $\mu$ và $\nu$ bị chặn trên bởi $\lambda$, nên tồn tại hai hàm khả tích địa phương theo $\lambda$ là $u$ và $v$ (có thể giả sử là đo được theo mọi nhờ §3, No. 4, Mệnh đề 7) sao cho $\mu = u \cdot \lambda$, $\nu = v \cdot \lambda$. Khi đó

$$
\inf(|\rho|, |\sigma|) = \inf(\mu, \nu) = \inf(u, v) \cdot \lambda
$$

(No. 2, Hệ quả của Mệnh đề 2). Cho $A$ (tương ứng $B$) là tập hợp các $t \in T$ sao cho $u(t) > 0$ và $v(t) = 0$ (tương ứng $u(t) = 0$ và $v(t) > 0$). Nếu $\rho$ và $\sigma$ rời nhau, thì $\inf(u, v) = 0$ hầu khắp nơi địa phương theo $\lambda$ (No. 3, Hệ quả 2 của Mệnh đề 3), do đó các tập hợp đo được theo mọi rời nhau $A$ và $B$ mang $\mu$ và $\nu$, tương ứng. Ngược lại, giả sử rằng $\mu$ và $\nu$ lần lượt được mang bởi các tập hợp rời nhau $R$ và $S$; $\varphi_R$ là đo được đối với độ đo $\mu = u \cdot \lambda$, và $\mu = \varphi_R \cdot \mu$. Theo Mệnh đề 8 của No. 4, hàm $u' = u \varphi_R$ là $\lambda$-đo được, và $\mu = u' \cdot \lambda$. Tương tự, nếu $v' = v \varphi_S$ thì $\nu = v' \cdot \lambda$; suy ra bằng cách nhận thấy rằng $\inf(u', v') = 0$ (No. 2, Hệ quả của Mệnh đề 2).

#### Hệ quả 1 {#int-v-s5-prop-13-cor-1 .statement}

*Với mọi độ đo thực $\nu$ trên $T$, tồn tại hai tập hợp rời nhau $M, N$ mang $\nu^+$ và $\nu^-$, tương ứng.*

Cần cẩn thận để không nhầm lẫn khái niệm giá đỡ của một độ đo $\nu$, với khái niệm của một tập hợp nơi $\nu$ tập trung. Giá đỡ S của $\nu$ là tập đóng nhỏ nhất mang $\nu$ (Ch. III, § 2, No. 2, Mệnh đề 2 và Ch. IV, §2, No. 2, Mệnh đề 5). Tuy nhiên, có thể tồn tại các tập con của S khác với S và mang $\nu$. Nói chung, có thể có $\inf(\mu, \nu) = 0$ đối với hai độ đo dương $\mu$ và $\nu$ có cùng giá đỡ (Bài tập 5).

Cũng chú ý rằng giao của các tập hợp mang $\nu$ là tập hợp các điểm $t \in T$ sao cho $|\nu|(\{t\}) > 0$, và nó có thể rỗng (ví dụ, trong trường hợp độ đo Lebesgue); do đó, nói chung không có một tập hợp nhỏ nhất mang $\nu$.

#### Hệ quả 2 {#int-v-s5-prop-13-cor-2 .statement}

— Cho $\rho$ và $\sigma$ là hai độ đo phức rời nhau, và cho $\rho'$ và $\sigma'$ là hai độ đo phức có mật độ tương ứng đối với $\rho$ và $\sigma$; khi đó $\rho'$ và $\sigma'$ rời nhau.

#### Hệ quả 3 {#int-v-s5-prop-13-cor-3 .statement}

— Cho $\rho$ và $\sigma$ là hai độ đo phức rời nhau; khi đó $|\rho + \sigma| = |\rho| + |\sigma|$.

Ký hiệu bởi $v$ (tương ứng $w$) một hàm khả đo được một cách phổ quát có giá trị tuyệt đối bằng 1 sao cho $\rho = v \cdot |\rho|$ (tương ứng $\sigma = w \cdot |\sigma|$) (Hệ quả 3 của Định lý 2), và bởi A một tập hợp khả đo được một cách phổ quát mang $\rho$, sao cho $B = \mathbf{C}A$ mang $\sigma$ (Mệnh đề 13); khi đó cũng có $\rho + \sigma = (v \varphi_A + w \varphi_B) \cdot (|\rho| + |\sigma|)$. Vì hàm $v \varphi_A + w \varphi_B$ có giá trị tuyệt đối bằng 1, nên hệ quả suy ra từ Mệnh đề 2.

#### Định lý 3 (Lebesgue) {#int-v-s5-thm-3 .statement}

— Mỗi độ đo phức $\theta$ trên T có thể được viết theo một và chỉ một cách dưới dạng $\theta = g \cdot \mu + \theta'$, trong đó $g$ là địa phương $\mu$-khả tích và $\theta'$ là một độ đo rời nhau với $\mu$. Khi đó $|\theta| = |g| \cdot \mu + |\theta'|$.

Khi $\theta$ dương, điều này suy ra ngay từ định lý của F. Riesz (Ch. II, §1, No. 5, Định lý 1) áp dụng cho không gian có thứ tự dàn đầy đủ $\mathcal{M}(T)$ của các độ đo thực trên T, và cho dải sinh bởi $\mu$ trong không gian này, xét đến Hệ quả 2 của No. 5, Định lý 2; hơn nữa, $\theta'$ và $g \cdot \mu$ khi đó đều dương, điều này kéo theo rằng $g$ dương địa phương hầu khắp nơi theo $\mu$ (Hệ quả 3 của Mệnh đề 3). Để xét trường hợp $\theta$ không dương, đặt $\nu = |\theta|$, $\nu = f \cdot \mu + \nu'$ (trong đó $f$ dương và trong đó $\nu'$ và $\mu$ rời nhau với nhau), và $\theta = v \cdot \nu$, trong đó $v$ là một hàm khả đo được một cách phổ quát có giá trị tuyệt đối bằng 1 (Hệ quả 3 của Định lý 2). Khi đó ta có (Mệnh đề 8) $\theta = g \cdot \mu + \theta'$, với $g = v f$ (sao cho $|g| = f$) và $\theta' = v \cdot \nu'$ (sao cho $|\theta'| = \nu'$ theo Mệnh đề 2); các độ đo $\theta'$ và $\mu$ rời nhau với nhau theo Hệ quả 2 của Mệnh đề 13. Chỉ còn phải thiết lập tính duy nhất của phân tích. Vậy, giả sử rằng $\theta = g \cdot \mu + \theta' = g_1 \cdot \mu + \theta'_1$, trong đó $\theta'$ và $\theta'_1$ rời nhau với $\mu$; $|\theta' - \theta'_1|$ bị chặn trên bởi $|\theta'| + |\theta'_1|$, do đó $\theta' - \theta'_1$ rời nhau với $\mu$, suy ra cũng rời nhau với $(g_1 - g) \cdot \mu$. Quan hệ $\theta' - \theta'_1 = (g_1 - g) \cdot \mu$ khi đó suy ra rằng hai vế đều bằng không, điều này chứng minh tính duy nhất.

Nhắc lại (No. 5, Th. 2 và Chú giải) rằng không gian $L^1_{loc}(T, \mu; \mathbf{C})$ có thể được đồng nhất (nhờ ánh xạ $g \mapsto g \cdot \mu$) với một không gian con của $\mathcal{M}_\mathbf{C}(T)$. Với quy ước này, Định lý 3 có dạng sau:

#### Hệ quả {#int-v-s5-n7-cor-1 .statement}

— *Tồn tại một phép chiếu p của không gian $\mathcal{M}_\mathbf{C}(T)$ lên không gian $L^1_{\text{loc}}(T, \mu; \mathbf{C})$, có hạt nhân $\overline{p}^{-1}(0)$ là tập hợp các độ đo phức ngoại lai đối với $\mu$, sao cho*

$$
|\theta| = |p(\theta)| + |\theta - p(\theta)|,\quad p(|\theta|) = |p(\theta)|
$$

*đối với mọi độ đo phức $\theta$.*

Nếu $p$ được hạn chế trên tập các độ đo bị chặn, ta thu được một phép chiếu $p^1$ của không gian $\mathcal{M}_\mathbf{C}^1(T)$ lên không gian $L^1_\mathbf{C}(T, \mu)$; quan hệ $\| \theta \| = |\theta|(1)$ suy ra rằng $\| \theta \| = \| p^1(\theta) \| + \| \theta - p^1(\theta) \|$ đối với mọi độ đo phức bị chặn $\theta$.

### 8. Ứng dụng: I. Tính đối ngẫu của các không gian $L^p$

Ở đây ta chỉ xét trường hợp các không gian thực $L^p$.

Nhắc lại rằng hai số $p, q$ sao cho $1 \leq p \leq +\infty$, $1 \leq q \leq +\infty$, $1/p + 1/q = 1$ được gọi là *số mũ liên hợp* (Ch. IV, §6, No. 4). Mỗi hàm $g \in \mathcal{L}^q$ xác định một dạng tuyến tính liên tục $\theta_g$ trên $L^p$, thu được bằng cách chuyển qua thương bắt đầu từ dạng tuyến tính $f \mapsto \int fg\,d\mu$ trên $\mathcal{L}^p$, và ta có $N_q(g) = \| \theta_g \|$ (Ch. IV, §6, No. 4, Hệ quả của Mệnh đề 3). Chuyển qua thương, do đó từ ánh xạ $g \mapsto \theta_g$ ta suy ra một ánh xạ tuyến tính đẳng cự $\varphi$ của $L^q$ vào đối ngẫu $(L^p)'$ của $L^p$. Ta sẽ chứng minh rằng, với $1 \leq p < +\infty$, $\varphi$ ánh xạ $L^q$ *lên* $(L^p)'$, do đó về sau ta có thể đồng nhất không gian Banach $L^q$ với không gian Banach $(L^p)'$ nhờ đẳng cấu $\varphi$. Phát biểu theo cách khác:

#### Định lý 4 {#int-v-s5-thm-4 .statement}

— *Cho p và q là hai số mũ liên hợp sao cho $1 \leq p < +\infty$. Mỗi dạng tuyến tính liên tục trên $\mathcal{L}^p(T, \mu)$ đều có dạng $f \mapsto \int fg\,d\mu$, trong đó g là một hàm trong $\mathcal{L}^q(T, \mu)$ mà lớp của nó trong $L^q$ được xác định.*

Cho $\theta$ là một dạng tuyến tính liên tục trên $\mathcal{L}^p$; do đó, tồn tại một số $a \geq 0$ sao cho $|\theta(f)| \leq a \cdot N_p(f)$ với mọi hàm $f \in \mathcal{L}^p$. Xét hạn chế của $\theta$ lên không gian $\mathcal{K}(T)$ các hàm liên tục có giá compact: với mọi tập con compact K của T và mọi hàm $f \in \mathcal{K}(T, K)$ (không gian các hàm liên tục có giá compact được chứa trong K), ta có $N_p(f) \leq (\mu(K))^{1/p} \| f \|$; do đó tôpô cảm sinh trên $\mathcal{K}(T, K)$ bởi tôpô của $\mathcal{L}^p$ thô hơn tôpô hội tụ đều, và hạn chế của $\theta$ lên từng $\mathcal{K}(T, K)$ vì thế liên tục đối với tôpô sau. Điều này có nghĩa là hạn chế của $\theta$ lên $\mathcal{K}(T)$ là một *độ đo thực* $\nu$ (Ch. III, §1, No. 3, Định nghĩa 2).

Ta chứng minh rằng $|\nu|(|f|) \leq a \cdot N_p(f)$ với mọi hàm $f$ trong $\mathcal{K}(T)$. Chỉ cần chứng minh công thức này cho $f \geq 0$. Bây giờ, với mọi hàm $\psi$ trong $\mathcal{K}(T)$ sao cho $|\psi| \leq f$, ta có
$$
|\nu(\psi)| \leq a \cdot N_p(\psi) \leq a \cdot N_p(f);
$$
mệnh đề của chúng ta suy ra từ biểu thức của giá trị tuyệt đối của một độ đo cho trong Ch. III, §1, No. 6, công thức (12). Quan hệ $|\nu|(|f|) \leq a (\mu(|f|^p))^{1/p}$ được suy rộng ngay sang trường hợp $f$ là hàm đặc trưng của một tập compact, bằng cách chuyển sang bao dưới, và rồi suy ra rằng mọi tập compact $\mu$-không đáng kể đều là $\nu$-không đáng kể, sao cho $\nu$ là một độ đo *có cơ sở* $\mu$ (No. 5, Định lý 2).

Do đó, tồn tại một hàm dương $h_1$ khả tích địa phương theo $\mu$ sao cho $|\nu|(f) = \int f h_1 d\mu$ với mọi hàm $f \in \mathcal{K}(T)$. Ta chứng minh rằng $h_1$ địa phương hầu khắp nơi bằng một hàm trong $\mathcal{L}^q$. Nếu hàm $f \geq 0$ trong $\mathcal{K}(T)$ sao cho $N_p(f) \leq 1$, thì $\int f h_1 d\mu = |\nu|(f) \leq a$. Vì thế, với mọi ánh xạ liên tục $f_0$ của T vào $[0,1]$ có giá compact, ta có $\sup \int (f_0 h_1) f d\mu \leq a$ khi $f$ chạy qua tập các hàm $\geq 0$ trong $\mathcal{K}(T)$ sao cho $N_p(f) \leq 1$. Từ đó suy ra, bằng công thức (11) của Ch. IV, §6, No. 4, rằng $N_q(f_0 h_1) \leq a$. Suy ra từ đây rằng $\sup_{K} N_q(\varphi_K h_1) \leq a$ khi K chạy qua tập các tập con compact của T, và điều này chứng minh mệnh đề của chúng ta (§1, Mệnh đề 9).

Cho $v$ là một hàm thực đo được mọi nơi có giá trị tuyệt đối bằng 1 sao cho $\nu = v \cdot |\nu|$ (Hệ quả 3 của Định lý 2) và cho $g = v h_1$; khi đó $\nu = g \cdot \mu$, và $g$ thuộc $\mathcal{L}^q$. Với mọi hàm $f \in \mathcal{K}(T)$, ta có $\theta(f) = \nu(f) = \int f g d\mu$. Nói cách khác, các dạng tuyến tính liên tục $\theta$ và $\theta_g$ trùng nhau trên $\mathcal{K}(T)$; do đó chúng bằng nhau trên $\mathcal{L}^p$, vì $\mathcal{K}(T)$ trù mật trong $\mathcal{L}^p$, và điều này hoàn tất chứng minh.

#### Hệ quả {#int-v-s5-n8-cor-1 .statement}

— *Với mọi số p sao cho $1 < p < +\infty$, không gian Banach $L^p(T, \mu)$ là phản xạ.*

Nói chung, đối ngẫu của $L^\infty$ không đẳng cấu với $L^1$, do đó $L^1$ và $L^\infty$ không phản xạ (Bài tập 10). Chúng ta sẽ đặc trưng các dạng tuyến tính liên tục trên $L^\infty$ phát sinh, bằng cách chuyển sang thương, từ một dạng tuyến tính $g \mapsto \int f g d\mu$ trên $\mathcal{L}^\infty$, với $g \in \mathcal{L}^1$.

Không gian vectơ có thứ tự $L^\infty(T, \mu)$, là một không gian con của $L^1_{loc}(T, \mu)$, được sắp theo dàn đầy đủ; thật vậy, nếu $(f_\alpha)$ là một họ các hàm dương trong $\mathcal{L}^\infty$ mà tập hợp các lớp $(\dot{f}_\alpha)$ của nó bị chặn trên trong $L^\infty$, thì tồn tại một $a \geq 0$ sao cho $N_\infty(f_\alpha) \leq a$ với mọi $\alpha$. Vì $L^1_{loc}(T, \mu)$ được sắp theo dàn đầy đủ, họ $(\dot{f}_\alpha)$ có một cận trên đúng $\dot{h}$ trong $L^1_{loc}(T, \mu)$; nhưng vì $\dot{a} \geq \dot{f}_\alpha$ với mọi $\alpha$, ta có $\dot{h} \leq \dot{a}$, do đó $N_\infty(h) \leq a$, suy ra mệnh đề đã nêu.

#### Mệnh đề 14 {#int-v-s5-prop-14 .statement}

— *Để cho một dạng tuyến tính dương $\theta$ trên $\mathcal{L}^\infty$ có dạng $f \mapsto \int f g d\mu$, với $g \in \mathcal{L}^1$, thì cần và đủ rằng, với mọi họ có hướng tăng $(f_\alpha)_{\alpha \in A}$ các hàm dương trong $\mathcal{L}^\infty$ mà tập hợp các lớp $(\dot{f}_\alpha)_{\alpha \in A}$ của nó bị chặn trên trong $L^\infty$ và có $\dot{h}$ làm cận trên đúng trong không gian này, ta có*

$$
\theta(h) = \sup_{\alpha \in A} \theta(f_\alpha).
$$

Trước hết ta chứng minh rằng điều kiện là cần thiết. Độ đo $h \cdot \mu$ là cận trên đúng trong $\mathcal{M}(T)$ của tập các độ đo $f_\alpha \cdot \mu$ (No. 5, Chú giải); do đó (Ch. II, §2, No. 2), với mọi hàm $\varphi \geq 0$ trong $\mathcal{K}(T)$, ta có $\int h \varphi \, d\mu = \sup_{\alpha \in A} \int f_\alpha \varphi \, d\mu$. Nếu bây giờ $a$ là một số $\geq 0$ sao cho $N_\infty(f_\alpha) \leq a$ với mọi $\alpha \in A$ (điều này suy ra $N_\infty(h) \leq a$), thì với mọi $\varepsilon > 0$ tồn tại một $\varphi \in \mathcal{K}(T)$ sao cho $\varphi \geq 0$ và $N_1(g - \varphi) \leq \varepsilon$, từ đó suy ra rằng $\int f_\alpha |g - \varphi| \, d\mu \leq a \varepsilon$ với mọi $\alpha \in A$, và $\int h |g - \varphi| \, d\mu \leq a \varepsilon$. Vì $\sup_{\alpha \in A} \int f_\alpha g \, d\mu \leq \int h g \, d\mu$, điều này chứng tỏ rằng hai vế của bất đẳng thức này bằng nhau.

Để chứng minh rằng điều kiện là đủ, ta sẽ dùng bổ đề sau:

#### Bổ đề 4 {#int-v-s5-lem-4 .statement}

1° *Cho $f$ là một hàm nửa liên tục dưới và bị chặn, không âm trên $T$. Khi đó lớp $\dot{f}$ của nó trong $L^\infty$ là cận trên đúng của tập các lớp $\dot{\varphi}$, trong đó $\varphi$ chạy qua tập các hàm trong $\mathcal{K}(T)$ thỏa mãn $0 \leq \varphi \leq f$.*

2° *Cho $f$ là một hàm đo được và bị chặn, không âm trên $T$. Khi đó lớp $\dot{f}$ của nó trong $L^\infty$ là cận dưới đúng của tập các lớp $\dot{\psi}$, trong đó $\psi$ chạy qua tập các hàm nửa liên tục dưới và bị chặn trên $T$ sao cho $\psi \geq f$.*

1° Cho $f'$ là một hàm trong $\mathcal{L}^\infty$ sao cho $\dot{f}'$ là cận trên đúng trong $L^\infty$ của tập các lớp $\dot{\varphi}$ của các hàm $\varphi$ trong $\mathcal{K}(T)$ thỏa mãn $0 \leq \varphi \leq f$; hiển nhiên $\dot{f}' \leq \dot{f}$. Cho $U$ là một tập con mở tương đối compact của $T$; với mọi hàm $h$ trong $\mathcal{K}(T)$ thỏa mãn $0 \leq h \leq f \varphi_U$ ta có, theo định nghĩa, $h(t) \leq f'(t)$ địa phương hầu khắp nơi, do đó $h(t) \leq f'(t) \varphi_U(t)$ hầu khắp nơi; suy ra $\int h \, d\mu \leq \int f' \varphi_U \, d\mu$. Tuy nhiên, vì $f \varphi_U$ là nửa liên tục dưới, $\int f \varphi_U \, d\mu = \sup \int h \, d\mu$, trong đó $h$ chạy qua tập các hàm trong $\mathcal{K}(T)$ thỏa mãn $0 \leq h \leq f \varphi_U$ (Ch. IV, §1, No. 1, Định nghĩa 1); do đó

$$
\int f \varphi_U \, d\mu \leq \int f' \varphi_U \, d\mu,
$$

và vì $f' \varphi_U \leq f \varphi_U$ hầu khắp nơi, tất yếu $f \varphi_U = f' \varphi_U$ hầu khắp nơi, do đó $f = f'$ hầu khắp nơi địa phương.

2° Cho $f'$ là một hàm trong $\mathcal{L}^\infty$ sao cho $\dot{f}'$ là cận dưới đúng trong $L^\infty$ của tập các lớp $\dot{\psi}$ của các hàm nửa liên tục dưới $\psi$ bị chặn và $\geq f$; khi đó $\dot{f}' \geq \dot{f}$. Cho $K$ là một tập con compact của $T$; với mọi hàm nửa liên tục dưới $h$ bị chặn và $\geq f \varphi_K$, đặt $\overline{h}$ là hàm bằng $h$ trên $K$ và bằng $\|f\| + \|h\|$ trên $T - K$. Khi đó $\overline{h}$ là nửa liên tục dưới và $\geq f$, do đó theo định nghĩa $\overline{h}(t) \geq f'(t)$ hầu khắp nơi địa phương; suy ra $h(t) \geq f'(t)\varphi_K(t)$ hầu khắp nơi, do đó $\int h d\mu \geq \int f'\varphi_K d\mu$. Nhưng $\int f\varphi_K d\mu = \inf \int h d\mu$, trong đó $h$ chạy trên tập các hàm nửa liên tục dưới bị chặn và $\geq f\varphi_K$ (Ch. IV, §1, No. 3, Def. 3); do đó

$$
\int f\varphi_K d\mu \geq \int f'\varphi_K d\mu,
$$

và vì $f\varphi_K \leq f'\varphi_K$ hầu khắp nơi, tất yếu $f\varphi_K = f'\varphi_K$ hầu khắp nơi, do đó $f = f'$ hầu khắp nơi địa phương.

Bổ đề đã được chứng minh, cho $\theta$ là một dạng tuyến tính dương trên $\mathcal{L}^\infty$ thỏa mãn điều kiện trong phát biểu của Mệnh đề 14. Hạn chế của $\theta$ lên không gian $\mathcal{K}(T)$ là một độ đo dương $\nu$ trên $T$. Ta sẽ chứng minh rằng, với mọi hàm dương $f \in \mathcal{L}^\infty(T, \mu)$, ta có $\theta(f) = \nu^*(f)$. Trước hết, giả sử $f$ nửa liên tục dưới (và bị chặn); theo Bổ đề 4, $f$ là cận trên đúng của tập có hướng tăng các lớp $\dot{\varphi}$, trong đó $\varphi$ chạy qua tập có hướng $\Phi$ của các hàm trong $\mathcal{K}(T)$ sao cho $0 \leq \varphi \leq f$. Vì theo giả thiết $\theta(f) = \sup_{\varphi \in \Phi} \theta(\varphi)$, và $\nu^*(f) = \sup_{\varphi \in \Phi} \nu(\varphi)$ theo định nghĩa, nên mệnh đề của chúng ta được chứng minh trong trường hợp này. Thứ hai, giả sử $f$ là $\mu$-đo được và bị chặn; khi đó, theo định nghĩa, $\nu^*(f) = \inf_{\psi \in \Psi} \nu^*(\psi)$, trong đó $\psi$ chạy qua tập có hướng giảm $\Psi$ gồm các hàm nửa liên tục dưới, bị chặn và $\geq f$. Nếu $a \geq \|f\|$ thì, áp dụng giả thiết của phát biểu cho tập có hướng tăng các lớp của các hàm $a - \psi$, trong đó $\psi \in \Psi$ và $\psi \leq a$, ta thấy, nhờ bổ đề, rằng $\theta(f) = \inf_{\psi \in \Psi} \theta(\psi)$, do đó thật vậy $\theta(f) = \nu^*(f)$. Đặc biệt, với mọi hàm không đáng kể theo $\mu$ thỏa mãn $f \geq 0$, ta có $\theta(f) = 0$, do đó $\nu^*(f) = 0$ và suy ra (No. 5, Th. 2) $\nu$ là một độ đo *với cơ sở* $\mu$; hơn nữa, $\nu^*(1) = \theta(1) < +\infty$, suy ra (Cor. of Th. 1) $\nu = g \cdot \mu$ với $g \in \mathcal{L}^1(T, \mu)$. Cuối cùng, vì mọi hàm đo được theo $\mu$ đều đo được theo $\nu$, mọi hàm dương $f \in \mathcal{L}^\infty(T, \mu)$ đều khả tích theo $\nu$ và $\int fg d\mu = \nu^*(f) = \theta(f)$, điều đó kết thúc chứng minh.

Suy ra từ Mệnh đề 14 rằng các dạng tuyến tính trên $\mathcal{L}^\infty$ có dạng $f \mapsto \int fg d\mu$, với $g \in \mathcal{L}^1$, là các hiệu $\theta_1 - \theta_2$, trong đó $\theta_1$ và $\theta_2$ là các dạng tuyến tính dương thỏa mãn điều kiện của Mệnh đề 14.

### 9. Ứng dụng: II. Các hàm của các độ đo

Cho $\mu_1, \mu_2, \ldots, \mu_n$ là các độ đo thực trên T, và cho $u(x_1, \ldots, x_n)$ là một hàm số hữu hạn, được định nghĩa trên $\mathbf{R}^n$, và thuần nhất dương, tức là (Ch. I, §1, No. 1), sao cho

$$
u(\alpha x_1, \ldots, \alpha x_n) = \alpha u(x_1, \ldots, x_n)
$$

với mọi vô hướng $\alpha \geqslant 0$. Tồn tại các độ đo dương $\lambda$ trên T sao cho $|\mu_i| \leqslant \lambda$ với $1 \leqslant i \leqslant n$ (ví dụ, tổng $\sum_{i=1}^n |\mu_i|$). Cho $\lambda$ và $\lambda'$ là hai độ đo như thế trên T. Ta có thể viết $\mu_i = f_i \cdot \lambda = f'_i \cdot \lambda'$, trong đó $f_i$ (resp. $f'_i$) là đo được và bị chặn hầu khắp nơi đối với độ đo $\lambda$ (resp. $\lambda'$) (No. 5, Th. 2). Ta sẽ chứng minh kết quả sau: *để hàm số $u(f_1, \ldots, f_n)$ địa phương khả tích đối với $\lambda$, điều kiện cần và đủ là hàm số $u(f'_1, \ldots, f'_n)$ địa phương khả tích đối với $\lambda'$, trong trường hợp đó*

$$
u(f_1, \ldots, f_n) \cdot \lambda = u(f'_1, \ldots, f'_n) \cdot \lambda'.
$$

Vì $|\mu_i| \leqslant \inf(\lambda, \lambda')$, ta có thể chỉ xét trường hợp $\lambda \leqslant \lambda'$. Khi đó $\lambda = g \cdot \lambda'$, trong đó $g$ là một hàm $\lambda'$-đo được sao cho $0 \leqslant g \leqslant 1$ (No. 5, Th. 2); do đó (No. 4, Prop. 8)

$$
\mu_i = f_i \cdot (g \cdot \lambda') = (f_i g) \cdot \lambda';
$$

suy ra (No. 3, Cor. 2 of Prop. 3) rằng $f_i g$ bằng $f'_i$ địa phương hầu khắp nơi đối với $\lambda'$. Do đó, theo (12),

$$
u(f'_1, \ldots, f'_n) = u(f_1 g, \ldots, f_n g) = u(f_1, \ldots, f_n) g
$$

địa phương hầu khắp nơi đối với $\lambda'$. Để $u(f'_1, \ldots, f'_n)$ địa phương $\lambda'$-khả tích, do đó cần và đủ là $u(f_1, \ldots, f_n) g$ địa phương khả tích đối với $\lambda'$, do đó (No. 4, Prop. 8) là $u(f_1, \ldots, f_n)$ địa phương khả tích đối với $\lambda$; và khi đó (No. 4, Prop. 8)

$$
u(f'_1, \ldots, f'_n) \cdot \lambda' = (u(f_1, \ldots, f_n) g) \cdot \lambda' = u(f_1, \ldots, f_n) \cdot \lambda.
$$

Vì thế, độ đo $u(f_1, \ldots, f_n) \cdot \lambda$ chỉ phụ thuộc vào các độ đo $\mu_1, \ldots, \mu_n$ và hàm $u$; nó cũng được ký hiệu là $u(\mu_1, \ldots, \mu_n)$. Do đó, độ đo này được định nghĩa bất cứ khi nào $u$ là một hàm thuần nhất dương sao cho, với một độ đo dương $\lambda$ là cận trên của mọi $|\mu_i|$, $u(f_1, \ldots, f_n)$ địa phương $\lambda$-khả tích, trong đó $f_i$ là mật độ của $\mu_i$ đối với $\lambda$. Chú ý rằng điều kiện này được thỏa mãn khi $u$ là thuần nhất dương và *liên tục*: vì khi đó ta có
$$
|u(x_1, \ldots, x_n)| \leq a(|x_1| + |x_2| + \cdots + |x_n|)
$$
(*u* được bị chặn trong một lân cận đủ nhỏ của $(0, \ldots, 0)$)), và vì $u(f_1, \ldots, f_n)$ là $\lambda$-đo được (Ch. IV, §5, No. 3, Th. 1), nên nó địa phương $\lambda$-khả tích nhờ tiêu chuẩn khả tích (Ch. IV, §5, No. 6, Th. 5).

Cho $u_1, \ldots, u_p$ là các hàm số vô hướng thuần nhất dương được xác định trên $\mathbf{R}^n$, sao cho $p$ hàm $g_k = u_k(f_1, \ldots, f_n)$ $(1 \leq k \leq p)$ khả tích địa phương theo $\lambda$. Cho $v$ là một hàm số vô hướng thuần nhất dương được xác định trên $\mathbf{R}^p$ sao cho $v(g_1, \ldots, g_p)$ khả tích địa phương theo $\lambda$. Đặt
$$
w(x_1, \ldots, x_n) = v(u_1(x_1, \ldots, x_n), \ldots, u_p(x_1, \ldots, x_n)).
$$
Khi đó, hàm $w$ là thuần nhất dương, $w(f_1, \ldots, f_n)$ khả tích địa phương theo $\lambda$ và, theo định nghĩa,
$$
w(\mu_1, \ldots, \mu_n) = v(u_1(\mu_1, \ldots, \mu_n), \ldots, u_p(\mu_1, \ldots, \mu_n)).
$$

Trong trường hợp đặc biệt của các hàm $x^+, x^-, |x|, x+y, \inf(x, y), \sup(x, y)$, các độ đo được xác định bởi phương pháp vừa mô tả trùng nhau, tương ứng, với những độ đo đã được ký hiệu là $\mu^+, \mu^-, |\mu|, \mu+\nu, \inf(\mu, \nu), \sup(\mu, \nu)$; điều này suy ra ngay từ Hệ quả của Mệnh đề 2 của No. 2. Nếu $\mu$ và $\nu$ là hai độ đo thực, và $\theta = \mu + i\nu$, thì $|\theta| = \sqrt{\mu^2 + \nu^2}$; vì, cho $\lambda$ là một độ đo $\geq 0$ là một cận trên của $|\mu|$ và $|\nu|$, và cho $f, g$ là các hàm khả tích địa phương theo $\lambda$ sao cho $\mu = f \cdot \lambda,\ \nu = g \cdot \lambda$; khi đó
$$
\sqrt{\mu^2 + \nu^2} = \sqrt{f^2 + g^2} \cdot \lambda,
$$
$$
\theta = (f + ig) \cdot \lambda,\ \text{do đó (No. 2, Mệnh đề 2)}\ |\theta| = \sqrt{f^2 + g^2} \cdot \lambda.
$$
Phương pháp này có thể áp dụng cho hàm số vô hướng thuần nhất dương $(x_1^2 + \ldots + x_n^2)^{1/2}$ để định nghĩa độ dài của một đường cong trong $\mathbf{R}^n$.

### 10. Các độ đo phân tán; các độ đo nguyên tử

#### Định nghĩa 5 {#int-v-s5-def-5 .statement}

*Một độ đo $\theta$ trên T được gọi là phân tán nếu* $|\theta|(\{t\}) = 0$ *với mọi* $t \in T$.

#### Ví dụ {#int-v-s5-n10-exa-1 .statement}

— Độ đo Lebesgue trên $\mathbf{R}$ là phân tán (Ch. IV, §1, No. 3, *Nhận xét* 1).

Nói rằng $\theta$ là một độ đo phân tán trên $T$ tức là nói rằng mọi tập có phần bù hữu hạn đều mang $|\theta|$, hay nói cách khác $|\theta|$ xung khắc với mọi độ đo điểm. Do đó các độ đo phân tán tạo thành một dải trong $\mathcal{M}(T)$ (Ch. II, §1, No. 5, ĐL. 1).

Nhắc lại (Ch. III, §1, No. 3) rằng một độ đo phức $\rho$ trên $T$ được gọi là *nguyên tử* nếu nó có dạng $\sum_{t \in T} \alpha(t) \varepsilon_t$, trong đó $\alpha$ là một hàm phức trên $T$ sao cho $\sum_{t \in K} |\alpha(t)| < +\infty$ với mọi tập con compact $K$ của $T$, điều đó biểu thị rằng họ $(\alpha(t) \varepsilon_t)_{t \in T}$ là khả tổng (§2, No. 1, Nhận xét 2). Khi đó suy ra từ nhận xét theo sau Hệ quả 3 của Mệnh đề 2 của No. 5 rằng $|\rho| = \sum_{t \in T} |\alpha(t)| \varepsilon_t$. Hàm $\alpha$ xuất hiện trong các công thức này được xác định duy nhất, vì $\alpha(t) = \rho(\{t\})$. Một độ đo nguyên tử và một độ đo phân tán xung khắc với nhau.

#### Mệnh đề 15 {#int-v-s5-prop-15 .statement}

*Mọi độ đo phức $\sigma$ trên $T$ đều có thể viết một cách duy nhất dưới dạng $\rho + \theta$, trong đó $\rho$ là một độ đo nguyên tử và $\theta$ là một độ đo phân tán; khi đó ta có $|\sigma| = |\rho| + |\theta|$.*.

Tính duy nhất của phân tích là hiển nhiên vì, $\rho$ là nguyên tử và $\theta$ phân tán, tất yếu $\rho = \sum_{t \in T} \rho(\{t\}) \varepsilon_t = \sum_{t \in T} \sigma(\{t\}) \varepsilon_t$ và $\theta = \sigma - \rho$. Để thiết lập sự tồn tại, chỉ cần nhận thấy rằng $\sum_{t \in K} |\sigma(\{t\})| \leq |\sigma|(K) < +\infty$ với mọi tập compact $K$, do đó có thể đặt $\sum_{t \in T} \sigma(\{t\}) \varepsilon_t = \rho$. Độ đo $\sigma - \rho$ hiển nhiên là phân tán, và hệ thức $|\sigma| = |\rho| + |\sigma - \rho|$ suy ra ngay từ Hệ quả 3 của Mệnh đề 13 của No. 7.

Người ta nhận thấy rằng chứng minh này cho thấy nếu $\sigma$ được mang bởi một tập hợp $M$ và nếu $|\sigma|(\{t\}) > 0$ với mọi $t \in M$, thì $\sigma$ là *nguyên tử*.

### Bài tập {#int-v-s5-exercises}

Xem [các bài tập cho § 5](exercises/s5/).
