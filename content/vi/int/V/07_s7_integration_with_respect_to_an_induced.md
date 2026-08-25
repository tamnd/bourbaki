---
book: int
book_title: Integration
chapter: V
chapter_title: INTEGRATION OF MEASURES
section: 7
section_title: Integration with respect to an induced measure
lang: vi
source: int-i-vi
book_pages: INT V.74-INT V.78, INT V.112-INT V.114
pdf_pages: 0329-0333, 0367-0369
extraction: ocr
subsections:
    - "no": 1
      title: Integration with respect to an induced measure
      page: 74
      pdf_page: 329
    - "no": 2
      title: Properties of induced measures
      page: 77
      pdf_page: 332
statements: 20
exercises: 11
content_sha256: cf682d1b137aea3f0b6e18e79c4e123c130c8d97923e48d77695d06e29c6f7be
translated_from: content/en/int/V/07_s7_integration_with_respect_to_an_induced.md
source_content_sha256: 4ecc2c2ebe5af11cad1fd2fc9b49c9e7ed029e1548c1c274e34065846fe89224
translation_model: gpt-5-6-mini
translation_run: translate-vi-5d1c0ce4
glossary_version: 34
glossary_terms_sha256: 9ecce355405918627c6ec78b3f1d9ff1ce5521d6f014a77a17843ee75f7806f1
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 7. TÍCH PHÂN ĐỐI VỚI MỘT ĐỘ ĐO CẢM SINH

### 1. Tích phân đối với một độ đo cảm sinh

Cho $X$ là một không gian con địa phương compact của $T$, $\mu$ là một độ đo dương trên $T$, và $\mu_X$ là độ đo cảm sinh trên $X$ bởi $\mu$ (Ch. IV, §5, No. 7). Với mọi $t \in T$, ta định nghĩa một độ đo $\lambda_t$ *trên* $X$ theo cách sau: $\lambda_t = \varepsilon_t$ nếu $t \in X$, $\lambda_t = 0$ nếu $t \in \mathbf{C}X$. Với mọi hàm số hữu hạn $g$ xác định trên $X$, $\int g(x) d\lambda_t(x) = g(t)$ nếu $t \in X$ và $\int g(x) d\lambda_t(x) = 0$ nếu $t \in \mathbf{C}X$. Nếu $g$ là một hàm trong $\mathcal{K}(X)$ thì do đó, theo định nghĩa của $\mu_X$,

$$
\mu_X(g) = \int \langle g, \lambda_t \rangle d\mu(t) .
$$

Điều này có nghĩa là ta có thể viết

$$
\mu_X = \int \lambda_t d\mu(t)
$$

(§3, No. 1).

Bây giờ ta định nghĩa một ánh xạ $\pi$ của T vào X bằng cách đặt $\pi(t) = t$ với $t \in X$, và $\pi(t) = t_0$ với $t \in \mathbf{C}X$, $t_0$ là một điểm tùy ý của X; ta có thể viết $\lambda_t = \varphi_X(t)\varepsilon_{\pi(t)}$ với mọi $t \in T$. Ánh xạ $\pi$ là $\mu$-đo được, vì các thu hẹp của nó trên X và $\mathbf{C}X$ là (Ch. IV, §5, No. 10, Mệnh đề 16); suy ra ngay rằng cặp $(\pi, \varphi_X)$ là $\mu$-thích nghi (§4, No. 1). Do đó ta có các kết quả sau:

#### Mệnh đề 1 {#int-v-s7-prop-1 .statement}

— *Đối với mọi hàm số* $g \geqslant 0$ *xác định trên* X,

$$
\int^\bullet g\,d\mu_X = \int_X g\,d\mu
$$

(xem §5, No. 3, *Ví dụ*, về ký hiệu $\int_X^\bullet$).

Xét đến các nhận xét trước đó và (2), quan hệ (3) suy ra từ Định lý 1 của §4.

#### Hệ quả 1 {#int-v-s7-prop-1-cor-1 .statement}

— *Đối với mọi tập con* B *của* X, $\mu_X^\bullet(B) = \mu^\bullet(B)$; *để* B *là* $\mu_X$*-không đáng kể địa phương, điều kiện cần và đủ là* B *là* $\mu$*-không đáng kể địa phương*.

#### Hệ quả 2 {#int-v-s7-prop-1-cor-2 .statement}

— *Cho* M *là một tập con của* T. *Nếu* $\mu$ *tập trung trên* M, *thì* $\mu_X$ *tập trung trên* $M \cap X$.

#### Hệ quả 3 {#int-v-s7-prop-1-cor-3 .statement}

— *Để độ đo* $\mu_X$ *bằng không, điều kiện cần và đủ là* X *là* $\mu$*-không đáng kể địa phương*.

#### Nhận xét {#int-v-s7-n1-rem-1 .statement}

— Nếu S là giá của $\mu$, thì $S \cap X$ (đóng trong X) chứa giá của $\mu_X$ theo Hệ quả 2, nhưng có thể phân biệt với nó. Ví dụ, nếu $\mu$ là một độ đo khuếch tán và X là một không gian con thu gọn thành một điểm, thì độ đo cảm sinh $\mu_X$ bằng không, do đó giá của nó là rỗng. Chú ý, tuy nhiên, rằng giá của $\mu_X$ bằng $S \cap X$ nếu X mở trong T.

#### Mệnh đề 2 {#int-v-s7-prop-2 .statement}

— *Để một ánh xạ* g *của* X *vào một không gian tôpô là* $\mu_X$*-đo được, điều kiện cần và đủ là* g *là* $\mu$*-đo được trong* X *(§5, No. 3, *Ví dụ*)*.

Điều này suy ra từ Mệnh đề 3 của §4.

#### Hệ quả {#int-v-s7-n1-cor-1 .statement}

— *Để một tập con* B *của* X *là* $\mu_X$*-đo được, điều kiện cần và đủ là* B *là* $\mu$*-đo được*.

#### Định lý 1 {#int-v-s7-thm-1 .statement}

— *Cho* g *là một hàm xác định trên* X, *với các giá trị trong* $\overline{\mathbf{R}}$ *hoặc trong một không gian Banach. Để* g *là* $\mu_X$*-nguyên cốt yếu, điều kiện cần* và đủ là $g$ *là* $\mu$*-nguyên cốt yếu trong* $X$ (\S 5, No. 3, Ví dụ), trong trường hợp đó

$$
\int g \, d\mu_X = \int_X g \, d\mu.
$$

Điều này suy ra từ Định lý 2 của \S 4.

#### Hệ quả 1 {#int-v-s7-thm-1-cor-1 .statement}

*Để một tập con B của X là* $\mu_X$*-nguyên cốt yếu, điều kiện cần và đủ là nó là* $\mu$*-nguyên cốt yếu, trong trường hợp đó* $\mu_X(B) = \mu(B)$.*

#### Hệ quả 2 {#int-v-s7-thm-1-cor-2 .statement}

*Cho g là một hàm phức xác định trên T và* $\mu$*-nguyên địa phương; hạn chế* $g_X$ *của g lên X khi đó là* $\mu_X$*-nguyên địa phương, và*

$$
(g \cdot \mu)_X = g_X \cdot \mu_X.
$$

Điều này suy ra ngay từ Định lý 1, áp dụng cho các hàm $fg_X$ ($f \in \mathcal{K}(X; \mathbf{C})$), và định nghĩa của độ đo cảm sinh trên X bởi một độ đo phức (Ch. IV, \S 5, No. 7).

#### Hệ quả 3 {#int-v-s7-thm-1-cor-3 .statement}

*Cho* $\theta$ *là một độ đo phức trên T; khi đó*

$$
|\theta|_X = |\theta_X|.
$$

Đặt $|\theta| = \mu$ và áp dụng Hệ quả 2 bằng cách lấy $g$ là một hàm phức có giá trị tuyệt đối 1 sao cho $\theta = g \cdot \mu$ (\S 5, No. 5, Hệ quả 3 của Định lý 2); khi đó $\theta_X = g_X \cdot \mu_X$; nhưng $g_X$ là một hàm có giá trị tuyệt đối 1, và công thức (6) suy ra từ Mệnh đề 2 của \S 5, No. 2.

#### Nhận xét {#int-v-s7-n1-rem-2 .statement}

— a) Hệ quả 3 đã được chứng minh bằng một phương pháp khác (Ch. IV, \S 5, No. 7, Bổ đề 3).
    b) Theo Hệ quả 3, các hệ quả 1,2,3 của Mệnh đề 1, Mệnh đề 2, Định lý 1 và các hệ quả 1,2 của nó mở rộng ngay cho một độ đo phức.

#### Chú giải {#int-v-s7-n1-sch-1 .statement}

— Với mọi hàm $f$ (tương ứng $g$) xác định trên $X$ (tương ứng $T$) với các giá trị trong không gian Banach $F$ hoặc trong $\overline{\mathbf{R}}$, ký hiệu $\zeta(f)$ (tương ứng $\rho(g)$) là mở rộng bằng 0 của $f$ lên $T$ (tương ứng là hạn chế của $g$ lên $X$). Khi đó $\zeta(\rho(g)) = \varphi_X \cdot g$, $\rho(\zeta(f)) = f$. Ta ký hiệu $\mu'$ là độ đo $\varphi_X \cdot \mu$ trên $T$. Với mọi $p \in [1, +\infty]$, các Mệnh đề 1 và 2 kéo theo rằng $\zeta$ ánh xạ $\mathcal{L}_F^p(X, \mu_X)$ vào $\mathcal{L}_F^p(T, \mu')$, và rằng $\rho$ ánh xạ $\mathcal{L}_F^p(T, \mu')$ lên $\mathcal{L}_F^p(X, \mu_X)$, với sự bảo toàn chuẩn trong cả hai trường hợp, cũng như bảo toàn tích phân khi $p = 1$ (Định lý 1); chuyển qua các không gian Hausdorff liên kết, ta thu được hai đẳng cấu nghịch đảo của nhau. Tương tự, nếu $\zeta$ và $\rho$ được áp dụng cho các hàm số dương, tích phân trên cốt yếu được bảo toàn (Mệnh đề 1). Như vậy, nếu ta đồng nhất một hàm trên $X$ với một hàm trên T bằng 0 trên X − T, và độ đo $\mu_X$ với độ đo $\mu'$, thì các bài toán liên quan đến các độ đo cảm sinh được quy về các bài toán liên quan đến các độ đo được xác định bởi mật độ, đã được xét trong §5. Kiểu lập luận này cũng áp dụng được cho các độ đo phức, theo Hệ quả 3 của Định lý 1.

### 2. Các tính chất của các độ đo cảm sinh

#### Mệnh đề 3 {#int-v-s7-prop-3 .statement}

— Cho X là một không gian con địa phương compact của T, và $\lambda$ là một độ đo phức trên X. Các tính chất sau là tương đương:
a) đơn ánh chính tắc $i : X \to T$ là $\lambda$-thực sự;
b) với mọi tập con compact K của T, $K \cap X$ là khả tích theo $\lambda$;
c) mọi điểm $t \in T$ đều có một lân cận V sao cho $V \cap X$ là khả tích theo $\lambda$;
d) tồn tại một độ đo $\theta$ trên T sao cho $\theta_X = \lambda$.
Nếu các điều kiện tương đương này được thỏa mãn, thì, với các ký hiệu như trong d),

$$
(i(\lambda))_X = \lambda \quad \text{và} \quad i(\lambda) = i(\theta_X) = \varphi_X \cdot \theta .
$$

Vì đơn ánh $i$ liên tục, tính tương đương của các tính chất a), b) và c) suy ra từ Mệnh đề 1 của §6, và nhận xét theo sau đó, áp dụng cho độ đo dương $|\lambda|$. Nếu $\lambda$ được cảm sinh trên X bởi một độ đo $\theta$ trên T, thì $|\lambda| = |\theta|_X$ (công thức (6)), do đó $|\lambda|(K \cap X) = |\theta|(K \cap X) \leq |\theta|(K) < +\infty$ (Mệnh đề 1) với mọi tập con compact K của T, nên d) suy ra b). Giả sử a) được thỏa mãn, và ta chứng minh rằng $(i(\lambda))_X = \lambda$, điều này sẽ suy ra d). Cho g là một phần tử của $\mathcal{H}(X; \mathbf{C})$; ký hiệu $g'$ là mở rộng bằng 0 của g lên T, ta có, theo định nghĩa của độ đo cảm sinh và sau đó theo Mệnh đề 7 của §6, No. 4,

$$
\int g \, d(i(\lambda))_X = \int g' \, d(i(\lambda)) = \int (g' \circ i) \, d\lambda = \int g \, d\lambda .
$$

Điều này hoàn tất chứng minh tính tương đương của bốn tính chất. Nếu $\lambda = \theta_X$ và $g \in \mathcal{H}(T; \mathbf{C})$, thì

$$
\int g \, d(i(\theta_X)) = \int (g \circ i) \, d(\theta_X) = \int g \varphi_X \, d\theta ,
$$

bởi vì $g \varphi_X$ là mở rộng bằng 0 của $g \circ i$ lên T. Điều này chứng minh công thức thứ hai của (7).

#### Hệ quả 1 {#int-v-s7-prop-3-cor-1 .statement}

— Nếu X đóng, thì mọi độ đo phức $\lambda$ trên X đều được cảm sinh bởi một độ đo trên T.

Thật vậy, nếu K là một tập compact trong T thì K ∩ X là compact, do đó khả tích theo λ.

#### Hệ quả 2 {#int-v-s7-prop-3-cor-2 .statement}

— Cho θ là một độ đo phức trên T, π là một ánh xạ θ-thực sự của T vào một không gian địa phương compact Y, và π_X là hạn chế của nó lên X. Khi đó π_X là θ_X-thực sự, và π_X(θ_X) = π(φ_X · θ).

Thật vậy, π_X = π ∘ i, trong đó i là đơn ánh chính tắc X → T. Khi θ dương, do đó hệ quả có thể được suy ra từ Mệnh đề 3 và tính bắc cầu của các độ đo ảnh (§6, No. 3, Mệnh đề 4). Trường hợp độ đo phức không dương sau đó suy ra bởi tính tuyến tính.

#### Mệnh đề 4 {#int-v-s7-prop-4 .statement}

— Cho X và Y là hai không gian con địa phương compact của T sao cho Y ⊂ X. Nếu θ là một độ đo phức trên T, thì độ đo (θ_X)_Y được cảm sinh bởi θ_X trên Y bằng θ_Y ('tính bắc cầu của các độ đo cảm sinh').

Chỉ cần nhận thấy rằng nếu g là một phần tử của $\mathcal{H}(Y; \mathbf{C})$, thì mở rộng bằng 0 của g lên T có thể nhận được bằng cách mở rộng bằng 0 mở rộng bằng 0 của g lên X, hoặc lại nữa, sử dụng các đồng nhất nhất trong Chú giải, rằng $φ_Y · θ = φ_Y(φ_X · θ)$ (§5, No. 4, Mệnh đề 8).

#### Mệnh đề 5 {#int-v-s7-prop-5 .statement}

— Cho $(\lambda_α)_{α ∈ A}$ là một họ có hướng tăng của các độ đo dương trên T, có một cận trên đúng λ, và cho X là một không gian con địa phương compact của T. Khi đó họ các độ đo cảm sinh $λ_α|X$ bị chặn trên trong $\mathcal{M}(X)$, và

$$
\sup_{α ∈ A} (λ_α|X) = λ|X.
$$

Theo các đồng nhất nhất trong Chú giải, mệnh đề này là một trường hợp riêng của Mệnh đề 5 của §5, No. 4.

#### Hệ quả {#int-v-s7-n2-cor-1 .statement}

— Cho $(\mu_i)_{i ∈ I}$ là một họ tổng được của các độ đo dương trên T, với tổng μ. Khi đó họ các độ đo cảm sinh $μ_i|X$ là tổng được, và

$$
\sum_{i ∈ I} (μ_i|X) = μ|X.
$$

#### Mệnh đề 6 {#int-v-s7-prop-6 .statement}

— Cho $Λ : t ↦ λ_t$ là một ánh xạ μ-thích hợp của T vào $\mathcal{M}_+(X)$, trong đó X là một không gian địa phương compact đếm được ở vô cực, và cho Y là một không gian con địa phương compact của X. Đặt $\int λ_t dμ(t) = ν$. Khi đó ánh xạ $t ↦ λ_t|Y$ của T vào $\mathcal{M}_+(Y)$ là μ-thích hợp, và

$$
\int (λ_t|Y) dμ(t) = ν|Y.
$$

Xét đến các đồng nhất nhất trong Chú giải, mệnh đề này là một trường hợp riêng của Mệnh đề 7 của §5, No. 4.

### Bài tập {#int-v-s7-exercises}

Xem [các bài tập của § 7](exercises/s7/).
