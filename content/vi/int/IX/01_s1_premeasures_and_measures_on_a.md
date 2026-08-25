---
book: int
book_title: Integration
chapter: IX
chapter_title: MEASURES ON HAUSDORFF TOPOLOGICAL SPACES
section: 1
section_title: Premeasures and measures on a topological space
lang: vi
source: int-vii-ix
pdf_pages: 0183-0204, 0288-0289
extraction: ocr
subsections:
    - "no": 1
      title: Encumbrances
      page: 0
      pdf_page: 183
    - "no": 2
      title: Premeasures and measures
      page: 3
      pdf_page: 185
    - "no": 3
      title: Examples of measures
      page: 6
      pdf_page: 188
    - "no": 4
      title: Locally negligible sets and functions
      page: 8
      pdf_page: 190
    - "no": 5
      title: Measurable sets and functions
      page: 9
      pdf_page: 191
    - "no": 6
      title: Directed families; support of a measure
      page: 11
      pdf_page: 193
    - "no": 7
      title: Upper envelopes and sums of measures
      page: 12
      pdf_page: 194
    - "no": 8
      title: Crushings
      page: 13
      pdf_page: 195
    - "no": 9
      title: Upper integral
      page: 17
      pdf_page: 199
    - "no": 10
      title: Integration theory
      page: 20
      pdf_page: 202
statements: 52
exercises: 10
content_sha256: ffd5be365ad9e2da598667bdde9ac1c334b5b1b847bb60f1daeb5f15b3f4e4e5
translated_from: content/en/int/IX/01_s1_premeasures_and_measures_on_a.md
source_content_sha256: 08cd64a9f736fcf3e935c7f25b844b7cb16ccedcafa8c3831a78cdb4a9369a30
translation_model: gpt-5.4-mini
translation_run: translate-vi-3557822e
glossary_version: 34
glossary_terms_sha256: f1e781727488069dcb4215c7962a41e5c0a9667ff5fb2e97735b4056ee857448
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 1. ĐỘ ĐO SƠ BỘ VÀ CÁC ĐỘ ĐO TRÊN MỘT KHÔNG GIAN TÔPÔ

### 1. Các định lượng

#### Định nghĩa 1 {#int-ix-s1-def-1 .statement}

— Cho T là một tập hợp. Người ta gọi một định lượng trên T bất kỳ ánh xạ p của $\mathcal{F}_+(T)$ vào $\overline{\mathbf{R}}_+$ thỏa các tính chất sau:
a) Nếu f và g là hai phần tử của $\mathcal{F}_+$ sao cho $f \leq g$, thì $p(f) \leq p(g)$.
b) Nếu f là một phần tử của $\mathcal{F}_+$, và t là một số $\geq 0$, thì $p(tf) = tp(f)$.

c) *Nếu f và g là hai phần tử của $\mathcal{F}_+$, thì $p(f + g) \leq p(f) + p(g)$.*
d) *Nếu $(f_n)$ là một dãy tăng của các phần tử của $\mathcal{F}_+$, và nếu $f = \lim_{n \to \infty} f_n$, thì $p(f) = \lim_{n \to \infty} p(f_n)$.*
*Nếu A là một tập con của T, ta viết $p(A)$ thay cho $p(\varphi_A)$.*

Điều kiện b) suy ra rằng $p(0) = 0$. Mặt khác, cho $(f_n)$ là một dãy các phần tử của $\mathcal{F}_+$; các điều kiện c) và d) suy ra bất đẳng thức

$$
p\left( \sum_n f_n \right) \leq \sum_n p(f_n)
$$

(*bất đẳng thức lồi đếm được*).

Chẳng hạn, cho T là một không gian địa phương compact, $\mu$ là một độ đo dương trên T; khi đó $\mu^*$ và $\mu^\bullet$ là các định lượng trên T. Điều này suy ra từ các Mệnh đề 10, 11, 12 và Định lý 3 của Ch. IV, §1, No. 3 đối với $\mu^*$, và từ Mệnh đề 1 của Ch. V, §1, No. 1 đối với $\mu^\bullet$.

#### Mệnh đề 1 {#int-ix-s1-prop-1 .statement}

*Cho $(p_\alpha)_{\alpha \in A}$ là một họ các định lượng trên T. Khi đó tổng và bao trên của họ $(p_\alpha)$ (trong $\mathcal{F}_+(\mathcal{F}_+(T))$) là các định lượng.*

Tổng của một họ hữu hạn các định lượng hiển nhiên là một định lượng, nên chỉ cần xét trường hợp bao trên. Các tính chất a), b), c) của Định nghĩa 1 hiển nhiên được thỏa mãn, chỉ còn phải chứng minh d). Đặt $p = \sup_\alpha p_\alpha$; khi đó, với các ký hiệu của Định nghĩa 1 d),

$$
p(f) = \sup_\alpha p_\alpha(f) = \sup_\alpha \sup_n p_\alpha(f_n) = \sup_n \sup_\alpha p_\alpha(f_n) = \sup_n p(f_n).
$$

#### Định nghĩa 2 {#int-ix-s1-def-2 .statement}

*Cho p là một định lượng trên một tập hợp T. Người ta nói rằng p là *bị chặn* nếu $p(T) < +\infty$. Nếu T là một không gian tôpô, p được gọi là *địa phương bị chặn* nếu mọi $x \in T$ đều có một lân cận V sao cho $p(V) < +\infty$.*

Từ các tính chất a) và c) của Định nghĩa 1 suy ra rằng $p(K) < +\infty$ đối với mọi tập con compact K của T. Đặc biệt, nếu T compact, thì mọi định lượng địa phương bị chặn trên T đều bị chặn.

Cho p là một định lượng trên một tập hợp T, và A là một tập con của T. Với mọi hàm $f \in \mathcal{F}_+(A)$, cho $f^0$ là phần kéo dài bởi 0 của f lên T; ánh xạ $f \mapsto p(f^0)$ trên $\mathcal{F}_+(A)$ khi đó là một định lượng, gọi là *định lượng cảm sinh bởi p* trên A, và được ký hiệu bởi $p|A$ hoặc $p_A$.

Cho T và U là hai tập hợp, $\pi$ là một ánh xạ từ T vào U, và p là một định lượng trên T. Định lượng $\pi(p)$ trên U, có giá trị với $f \in \mathcal{F}_+(U)$ được cho bởi

$$
(\pi(p))(f) = p(f \circ \pi),
$$

được gọi là *định lượng ảnh* của p dưới $\pi$.

Cho $p$ là một định lượng trên một tập hợp $T$; p được gọi là *tập trung* trên một tập con $A$ của $T$ nếu $p(T - A) = 0$.

#### Bổ đề 1 {#int-ix-s1-lem-1 .statement}

— *Nếu định lượng $p$ tập trung trên $A \subset T$, thì $p(f) = p(f \varphi_A)$ với mọi $f \in \mathcal{F}_+(T)$.*

Vì, đặt $T - A = B$, do đó $p(\varphi_B) = 0$; khi đó

$$
f \varphi_B \leq (+\infty) \cdot \varphi_B = \sup_{n \in \mathbf{N}} n \varphi_B,
$$

do đó $p(f \varphi_B) = 0$ theo các tính chất $a), b), d)$ của Định nghĩa 1. Suy ra từ $c)$ rằng $p(f) \leq p(f \varphi_A) + p(f \varphi_B) = p(f \varphi_A)$, và cuối cùng $p(f) = p(f \varphi_A)$ theo $a)$.

### 2. Tiền độ đo và độ đo

Cho $T$ là một không gian tôpô, và cho $\mathfrak{K}$ là tập hợp các tập con compact của $T$, được sắp thứ tự bởi phép bao hàm. Với mọi $K \in \mathfrak{K}$, đặt $\mathcal{M}(K; \mathbf{C})$ là tập hợp các độ đo phức trên $K$. Với mọi cặp $(K, L)$ gồm các phần tử của $\mathfrak{K}$ sao cho $K \subset L$, hãy gọi $\iota_{KL}$ là ánh xạ từ $\mathcal{M}(L; \mathbf{C})$ vào $\mathcal{M}(K; \mathbf{C})$ gán cho mỗi độ đo $\mu$ trên $L$ độ đo $\mu_K$ cảm sinh bởi $\mu$ trên $K$ (Ch. IV, §5, No. 7, Định nghĩa 4). Khi đó $\iota_{KM} = \iota_{KL} \circ \iota_{LM}$ khi $K$, $L$ và $M$ là các tập con compact của $T$ sao cho $K \subset L \subset M$; điều này suy ra từ tính bắc cầu của các độ đo cảm sinh (Ch. V, §7, No. 2, Mệnh đề 4). Các phần tử của *giới hạn ngược* của họ $(\mathcal{M}(K; \mathbf{C}))_{K \in \mathfrak{K}}$ đối với các ánh xạ $\iota_{KL}$ sẽ được gọi là *tiền độ đo* trên $T$. Nói cách khác:

#### Định nghĩa 3 {#int-ix-s1-def-3 .statement}

*Một ánh xạ trên một không gian tôpô $T$ được gọi là tiền độ đo nếu nó gán cho mỗi tập con compact $K$ của $T$ một độ đo $w_K$ trên $K$, và có tính chất sau đây:

*Nếu $K$ và $L$ là các tập con compact của $T$ sao cho $K \subset L$, thì độ đo $(w_L)_K$ cảm sinh bởi $w_L$ trên $K$ bằng $w_K$.

Tiền độ đo $w$ được gọi là thực (resp. dương) nếu mọi độ đo $w_K$ đều là thực (resp. dương).*

Cho $w$ và $w'$ là hai tiền độ đo trên $T$, $t$ là một số phức; các tiền độ đo $w + w'$ và $tw$ được xác định bởi các công thức $(w + w')_K = w_K + w'_K$, $(tw)_K = tw_K$ với mọi tập con compact $K$ của $T$. Các tiền độ đo trên $T$ hiển nhiên lập thành một không gian vectơ, được ký hiệu $\mathcal{P}(T; \mathbf{C})$; không gian các tiền độ đo thực sẽ được ký hiệu $\mathcal{P}(T; \mathbf{R})$, hay thường hơn $\mathcal{P}(T)$, và nón lồi của các tiền độ đo dương sẽ được ký hiệu $\mathcal{P}_+(T)$. Cho $w$ là một tiền độ đo; ánh xạ $K \mapsto |w_K|$ khi đó là một tiền độ đo trên $T$ (Ch. IV, §5, No. 7, Bổ đề 3), và sẽ được ký hiệu là $|w|$. Nếu $w$ là thực, ta đặt w^+ = \frac{1}{2}(|w| + w),\ w^- = \frac{1}{2}(|w| - w); hai tiền độ đo này dương, suy ra mọi tiền độ đo thực là hiệu của hai tiền độ đo dương. Rõ ràng $(w^+)_K = (w_K)^+$, $(w^-)_K = (w_K)^-$ với mọi tập con compact K của T.

Không gian vectơ $P(T)$ được sắp thứ tự bởi nón $P_+(T)$. Rõ ràng $w^+ = \sup(w, 0),\ w^- = \sup(-w, 0)$; do đó, $P(T)$ là một dàn có thứ tự và $\sup(w, w') = w + (w' - w)^+,\ \inf(w, w') = w - (w' - w)^-$. Hơn nữa, rõ ràng

$$
(\sup(w, w'))_K = \sup(w_K, w'_K),\quad (\inf(w, w'))_K = \inf(w_K, w'_K)
$$

với mọi tập con compact K của T.

#### Định nghĩa 4 {#int-ix-s1-def-4 .statement}

*Cho w là một tiền độ đo dương trên T. Ta sẽ đặt, với mọi hàm $f \in \mathcal{F}_+(T)$,*

$$(1)$$
$$
w^\bullet(f) = \sup_K (w_K)^\bullet(f_K),
$$

*trong đó K chạy qua tập các tập con compact của T.*

Với mỗi tập compact K, gọi $p^K$ là ảnh tải của tải $(w_K)^\bullet$ qua đơn ánh chính tắc của K vào T; $w^\bullet$ là bao trên của các tải $p^K$, nên là một tải (No. 1, Mệnh đề 1). Người ta nói rằng $w^\bullet$ là *nguyên trên cốt yếu* liên kết với tiền độ đo dương w. Người ta thường viết $\int^\bullet f\, dw$ hoặc $\int^\bullet f(t)\, dw(t)$ thay cho $w^\bullet(f)$.

*Nhận xét 1).* — Nếu v và w là hai tiền độ đo dương, thì $(v + w)^\bullet = v^\bullet + w^\bullet$ (Ch. V, §1, No. 1, Mệnh đề 3). Nếu v và w là hai tiền độ đo phức, thì $|v + w|^\bullet \leq |v|^\bullet + |w|^\bullet$.

#### Mệnh đề 2 {#int-ix-s1-prop-2 .statement}

*a) Cho w là một tiền độ đo dương. Với mọi tập con compact K của T, tải $(w^\bullet)_K$ cảm sinh bởi $w^\bullet$ trên K bằng $(w_K)^\bullet$. Với mọi hàm $f \in \mathcal{F}_+(T)$, ta có các hệ thức $(w_K)^\bullet(f_K) = w^\bullet(f_{\varphi_K})$ và*

$$(2)$$
$$
w^\bullet(f) = \sup_K w^\bullet(f_{\varphi_K}).
$$

*b) Ngược lại, cho p là một tải trên T thỏa mãn các điều kiện sau:
1) Với mọi tập con compact K của T, tồn tại một độ đo dương $w_K$ trên K sao cho $p_K = (w_K)^\bullet$.
2) Với mọi hàm $f \in \mathcal{F}_+(T)$, $p(f) = \sup_K p(f_{\varphi_K})$.
Ánh xạ $w : K \mapsto w_K$ khi đó là một tiền độ đo dương trên T, và $p = w^\bullet$.

Chứng minh a: cho $g \in \mathcal{F}_+(K)$ và gọi $g^0$ là phần mở rộng bằng không của g lên T; khi đó, theo định nghĩa của các tải cảm sinh,

$$
(w^\bullet)_K(g) = w^\bullet(g^0) = \sup_L (w_L)^\bullet(g^0|L),
$$

trong đó $L$ chạy qua tập hợp các tập compact của $T$, hoặc chỉ qua tập hợp những tập chứa $K$. Nhưng nếu $L$ chứa $K$, thì $(w_L)^\bullet(g^0|L) = (w_K)^\bullet(g)$ vì $g^0|L$ bằng không ở ngoài $K$ (Ch. V, §7, No. 1, Mệnh đề 1), điều này chứng minh mệnh đề đầu tiên. Do đó

$$
(w_K)^\bullet(f_K) = (w^\bullet)_K(f_K) = w^\bullet((f_K)^0) = w^\bullet(f_{\varphi_K})
$$

với mọi $f \in \mathcal{F}_+(T)$, và (2) chỉ là cách viết lại công thức (1).

Ta hãy chuyển sang $b$: độ đo $w_K$ xét trong 1) là duy nhất (Ch. V, §1, No. 1). Ta hãy chứng minh rằng ánh xạ $K \mapsto w_K$ là một tiền độ đo: cho $K$ và $L$ là hai tập compact sao cho $K \subset L$, và cho $\lambda$ là độ đo cảm sinh bởi $w_L$ trên $K$; mọi việc quy về chứng minh rằng $\lambda^\bullet = (w_K)^\bullet$. Bây giờ, $\lambda^\bullet = ((w_L)^\bullet)_K$ (Ch. V, §7, No. 1, Mệnh đề 1); vì $(w_L)^\bullet = p_L$, ta có $\lambda^\bullet = (p_L)_K = p_K = (w_K)^\bullet$.

Đặt $w$ là tiền độ đo $K \mapsto w_K$; vì $p_K = (w_K)^\bullet = (w^\bullet)_K$, ta có $p(f_{\varphi_K}) = p_K(f_K) = (w^\bullet)_K(f_K) = w^\bullet(f_{\varphi_K})$. Hai độ đo $p$ và $w^\bullet$ do đó bằng nhau nhờ công thức (2) và giả thiết 2) về $p$.

ĐPCM.

Vì độ đo cảm sinh $(w^\bullet)_K$ bằng $(w_K)^\bullet$, nên không có mơ hồ khi chỉ viết $w_K^\bullet$. Từ nay chúng tôi sẽ dùng ký hiệu này.

#### Hệ quả {#int-ix-s1-n2-cor-1 .statement}

— *Cho $v$ và $w$ là hai tiền độ đo dương trên $T$, sao cho $v^\bullet(L) = w^\bullet(L)$ với mọi tập compact $L$ của $T$; khi đó $v = w$. Nói riêng, quan hệ $v^\bullet = w^\bullet$ suy ra $v = w$.*

Vì, cho $K$ là một tập compact trong $T$; với mọi tập compact $L \subset K$, ta có quan hệ

$$
w_K(L) = w_K^\bullet(L) = w^\bullet(L) = v^\bullet(L) = v_K^\bullet(L) = v_K(L)
$$

theo Mệnh đề 2; do đó $w_K = v_K$ (Ch. IV, §4, No. 10, Hệ quả 3 của Mệnh đề 19), và cuối cùng $w = v$ theo định nghĩa của tiền độ đo.

#### Định nghĩa 5 {#int-ix-s1-def-5 .statement}

— *Cho $w$ là một tiền độ đo trên một không gian tôpô $T$. Người ta nói rằng $w$ là một độ đo (tương ứng, một độ đo bị chặn) nếu độ đo $|w|^\bullet$ là địa phương bị chặn (tương ứng, bị chặn) (xem No. 1, Định nghĩa 2)*.

Tập hợp các độ đo phức trên $T$ hiển nhiên là một không gian vectơ (*Nhận xét* 1), ký hiệu $\mathcal{M}(T; \mathbf{C})$. Không gian các độ đo thực sẽ được ký hiệu $\mathcal{M}(T; \mathbf{R})$ hoặc thường hơn là $\mathcal{M}(T)$, và nón các độ đo dương sẽ được ký hiệu $\mathcal{M}_+(T)$.

Nếu $w$ là một độ đo phức, thì phần thực và phần ảo của nó là các độ đo thực. Nếu $w$ là một độ đo thực, thì $w^+$ và $w^-$ là các độ đo dương. Mọi độ đo phức (tương ứng thực) do đó là một tổ hợp tuyến tính (tương ứng hiệu) của các độ đo dương.

#### Nhận xét 2 {#int-ix-s1-n2-rem-2 .statement}

Nếu $T$ là *địa phương compact*, thì mọi tiền độ đo $w$ trên $T$ đều là một độ đo. Thật vậy, mỗi $x \in T$ nhận được một lân cận compact $K$, và $|w|^*(K) = \|w_K\| < +\infty$, nên gánh nặng $|w|^*$ là bị chặn địa phương.

#### Nhận xét 3 {#int-ix-s1-n2-rem-3 .statement}

Với mọi tập con Borel $A$ của $T$ (đặc biệt với $A = T$) và mọi độ đo dương $\mu$ trên $T$, số $\mu^*(A)$ là cận trên đúng của các độ đo $\mu^*(K)$ với $K$ chạy trên các tập con compact của $A$. Thật vậy, với mọi tập con compact $K$ của $A$, ta có $\mu^*(K) \leq \mu^*(A)$; mặt khác, nếu $\mathfrak{K}$ là tập hợp các tập con compact của $T$, thì

$$
\mu^*(A) = \sup_{K \in \mathfrak{K}} \mu_K^*(A \cap K) = \sup_{K \in \mathfrak{K}} \sup_{L \in \mathfrak{K}, L \subset A \cap K} \mu_K^*(L) \leq \sup_{L \in \mathfrak{K}, L \subset A} \mu^*(L)
$$

theo Hệ quả 1 của ĐL. 4 của Ch. IV, §4, No. 6.

### 3. Các ví dụ về độ đo

#### Ví dụ 1 {#int-ix-s1-n3-exa-1 .statement}

— *Độ đo trên một không gian địa phương compact.*

Mệnh đề sau cho thấy lý thuyết của chương này bao hàm lý thuyết của Ch. IV. Trong phát biểu, từ 'measure' và ký hiệu $\mathcal{M}(T; \mathbf{C})$ được hiểu theo nghĩa của các chương trước.

#### Mệnh đề 3 {#int-ix-s1-prop-3 .statement}

*Cho $T$ là một không gian địa phương compact, và cho $\mu$ là một độ đo trên $T$. Kí hiệu $W(\mu)$ là ánh xạ gán cho mỗi tập con compact $K$ của $T$ độ đo cảm sinh $\mu_K$. Khi đó $W(\mu)$ là một tiền độ đo trên $T$, ta có $W(|\mu|) = |W(\mu)|$, và ánh xạ tuyến tính $W : \mu \mapsto W(\mu)$ là một song ánh từ không gian $\mathcal{M}(T; \mathbf{C})$ lên không gian $\mathcal{P}(T; \mathbf{C})$ của các tiền độ đo trên $T$. Hơn nữa, nếu $\mu$ dương thì $\mu^* = (W(\mu))^*$.*

Hiển nhiên rằng $W(\mu)$ là một tiền độ đo (Ch. V, §7, No. 2, Mệnh đề 4) và rằng ánh xạ $W$ là tuyến tính. Quan hệ $W(\mu) = 0$ có nghĩa là $\mu$ cảm sinh độ đo 0 trên mọi tập compact trong $T$; khi đó $\mu(f) = 0$ với $f \in \mathcal{H}(T; \mathbf{C})$, do đó $\mu = 0$, điều này chứng tỏ rằng $W$ là đơn ánh. Còn phải chứng minh rằng $W$ là toàn ánh. Vì mọi tiền độ đo đều là một tổ hợp tuyến tính của các tiền độ đo dương, nên chỉ cần xây dựng, cho mỗi *tiền độ đo dương* $w$, một độ đo dương $\mu$ sao cho $w = W(\mu)$. Cho $f \in \mathcal{H}(T)$ là một hàm cho trước, và cho $L$ là một tập compact chứa giá đỡ của $f$; số $w_L(f_L)$ không phụ thuộc vào lựa chọn của $L$, theo định nghĩa của các độ đo cảm sinh, nên có thể đặt $\mu(f) = w_L(f_L)$; khi đó $\mu$ là một dạng tuyến tính dương trên $\mathcal{H}(T)$, tức là một độ đo dương. Ta hãy kiểm tra rằng $w = W(\mu)$; trước hết, quan hệ $\mu^\bullet(f) = w_L^\bullet(f_L)$ mở rộng sang trường hợp $f$ là một hàm nửa liên tục trên hữu hạn, dương và bằng 0 ngoài $L$. Thật vậy, cho $M$ là một lân cận compact của $L$, và $\mathcal{H}$ là tập (có hướng giảm) các hàm liên tục trên $T$, có giá đỡ được chứa trong $M$, sao cho chúng $\geq f$. Khi đó (Ch. IV, §4, No. 4, Hệ quả 2 của Mệnh đề 5)

$$
\mu^\bullet(f) = \inf_{h \in \mathcal{H}} \mu(h) = \inf_{h \in \mathcal{H}} w_M(h_M) = w_M^\bullet(f_M),
$$

và mặt khác $w_M^\bullet(f_M) = w_L^\bullet(f_L)$ vì $f_M$ bằng 0 trên $M - L$ (Ch. V, §7, No. 1, Mệnh đề 1). Đặc biệt, nếu lấy $f$ là mở rộng bằng 0 của một phần tử của $\mathcal{H}_+(L)$, công thức này cho thấy $\mu_L = w_L$ theo định nghĩa của các độ đo cảm sinh, do đó thật vậy $W(\mu) = w$.

Nếu $\mu$ là dương, thì

$$
\mu^\bullet(f) = \sup_K \mu^\bullet(f \varphi_K) = \sup_K \mu_K^\bullet(f_K) = (W(\mu))^\bullet(f)
$$

với mọi $f \in \mathcal{F}_+(T)$ (Ch. V, §1, Định nghĩa 1 và §7, Mệnh đề 1). Quan hệ $|W(\mu)| = W(|\mu|)$ là hiển nhiên (Ch. IV, §5, No. 7, Bổ đề 3).

ĐPCM.

Khi $T$ là *compact địa phương*, từ nay về sau ta sẽ *đồng nhất* các không gian $\mathcal{M}(T; \mathbf{C})$ và $\mathcal{P}(T; \mathbf{C})$ bằng song ánh $W$.

#### Ví dụ 2 {#int-ix-s1-n3-exa-2 .statement}

— *Các độ đo có giá đỡ compact trên một không gian tôpô.*

#### Bổ đề 2 {#int-ix-s1-lem-2 .statement}

— *Cho $T$ là một không gian tôpô, $L$ là một tập con compact của $T$, và $\lambda$ là một độ đo dương trên $L$. Tồn tại duy nhất một độ đo dương $\mu$ trên $T$ sao cho, với mọi hàm $f \in \mathcal{F}_+(T)$,*

(2)
$$
\mu^\bullet(f) = \lambda^\bullet(f_L).
$$

Chúng ta đặt $p(f) = \lambda^\bullet(f_L)$ với mọi $f \in \mathcal{F}_+(T)$, và hãy chứng minh rằng các điều kiện 1) và 2) của Mệnh đề 2 *b*) được thỏa mãn. Điều kiện thứ hai hiển nhiên được thỏa mãn: thật vậy, $p(f) = p(f \varphi_K)$ nếu $K$ chứa $L$. Nếu $K \subset T$ là compact, và nếu $h \in \mathcal{F}_+(K)$, thì

$$
p_K(h) = p(h^0) = \lambda^\bullet(h^0|L).
$$

Nhưng $h^0|L$ là phép mở rộng bởi 0 của $h_{K \cap L}$ lên $L$: do đó biểu thức cuối cùng bằng $(\mu_K)^\bullet(h)$, trong đó $\mu_K$ là ảnh của $\lambda|K \cap L$ qua đơn ánh của $K \cap L$ vào $K$ (Ch. V, §6, No. 2, Mệnh đề 2 và §7, No. 1, Mệnh đề 1), và $p_K = (\mu_K)^\bullet$. Vì vậy điều kiện 1) của Mệnh đề 2 *b*) cũng được thỏa mãn, và sự tồn tại của $\mu$ suy ra ngay.

Q.E.D.

Ta sẽ nói rằng $\mu$ là độ đo trên T *được xác định* bởi $\lambda$. Đặc biệt, với mọi điểm $x$ của T, ta có thể định nghĩa độ đo $\varepsilon_x$; nó được đặc trưng bởi $(\varepsilon_x)^*(f) = f(x)$ với $f \in \mathcal{F}_+(T)$.

#### Nhận xét {#int-ix-s1-n3-rem-1 .statement}

— 1) Khi T là địa phương compact, $\mu$ là ảnh của $\lambda$ qua đơn ánh của L vào T. Chúng ta sẽ thấy ở §2, No. 3, *Ví dụ*, khi các độ đo ảnh đã được xét, rằng cách hiểu này vẫn đúng cho các không gian tùy ý.
2) Chúng ta cũng sẽ thấy rằng các độ đo được định nghĩa trong *Ví dụ* 2 là các độ đo dương trên T với giá đỡ compact (No. 6, *Nhận xét* 2)).

*Từ nay trở đi, trừ khi có lời nói rõ ràng ngược lại, chúng ta sẽ chỉ xét các độ đo dương. Trong phần còn lại của tiết này, T sẽ ký hiệu một không gian tôpô và $\mu$ một độ đo dương trên T.*

Nhiều kết quả trong các tiểu mục sau có thể được mở rộng cho các tiền độ dương. Phần mở rộng này để lại cho bạn đọc.

### 4. Các tập hợp và hàm không đáng kể địa phương

#### Định nghĩa 6 {#int-ix-s1-def-6 .statement}

*Một hàm* $f \in \mathcal{F}_+$ *(hoặc một tập con* A *của* T) *được gọi là không đáng kể địa phương đối với độ đo* $\mu$ *nếu* $\mu^*(f) = 0$ *(hoặc* $\mu^*(A) = 0$). *Người ta nói rằng* $\mu$ *tập trung trên một tập con* A *của* T *nếu* T − A *là không đáng kể theo* $\mu$ *ở địa phương*.

#### Nhận xét {#int-ix-s1-n4-rem-1 .statement}

— 1) Các khái niệm như trên, khi T là địa phương compact, trùng với các khái niệm thông thường.
2) Sau khi chúng ta đã định nghĩa các tập hợp *không đáng kể*, ta sẽ thấy rằng các tập hợp không đáng kể địa phương thật sự là những tập mà mầm của chúng, tại mọi điểm của T, là mầm của một tập không đáng kể (No. 9, Hệ quả 2 của Mệnh đề 14).
3) Cũng như trong Chs. IV và V, cụm từ 'hầu khắp nơi địa phương' sẽ đồng nghĩa với 'trừ trên một tập không đáng kể địa phương'.
4) Nếu $\theta$ là một độ đo phức, ta sẽ nói rằng một hàm (hoặc một tập con của T) là không đáng kể địa phương đối với $\theta$ nếu nó như vậy đối với độ đo dương $|\theta|$.

#### Ví dụ {#int-ix-s1-n4-exa-1 .statement}

— Cho L là một tập con compact của T, $\lambda$ là một độ đo trên L, và $\mu$ là độ đo trên T được xác định bởi $\lambda$ (No. 3, *Ví dụ* 2). Công thức (3) suy ra ngay rằng một hàm $f \in \mathcal{F}_+(T)$ là không đáng kể địa phương đối với $\mu$ nếu và chỉ nếu $f_L$ là không đáng kể đối với $\lambda$.

Suy ra ngay từ công thức (1) rằng một hàm $f \in \mathcal{F}_+(T)$ là không đáng kể địa phương đối với $\mu$ nếu và chỉ nếu $f_K$ là không đáng kể đối với $\mu_K$ với mọi tập con compact K của T. Do đó các tính chất của các tập hợp không đáng kể địa phương quy về ngay các tính chất của các tập không đáng kể trong các không gian compact, đã được xét trong Ch. IV. Sau đây là một số kết quả sẽ được dùng từ nay về sau mà không nhắc lại.

— Để một hàm $f \geqslant 0$ là không đáng kể địa phương, điều kiện cần và đủ là $f(t) = 0$ hầu khắp nơi địa phương (Ch. IV, §2, No. 3, Th. 1). Nếu $f$ là một hàm nhận giá trị trong một không gian Banach, thì do đó tương đương khi nói rằng $f = 0$ hầu khắp nơi địa phương hay rằng $\mu^*(|f|) = 0$; trong trường hợp này ta lại nói rằng $f$ là không đáng kể địa phương.

— Tổng và bao trên của một dãy các hàm không đáng kể địa phương $\geqslant 0$ là không đáng kể địa phương (*loc. cit.*, No. 1, Mệnh đề 2).

— Nếu $f$ và $g$ là hai hàm $\geqslant 0$ bằng nhau hầu khắp nơi địa phương, thì $\mu^\bullet(f) = \mu^\bullet(g)$ (*loc. cit.*, No. 3, Mệnh đề 6).

### 5. Các tập hợp và hàm đo được

#### Định nghĩa 7 {#int-ix-s1-def-7 .statement}

*Một hàm* $f$ *được xác định trên* $T$, *có giá trị trong một không gian tôpô* $F$ (*Hausdorff hay không*) *được gọi là đo được đối với độ đo* $\mu$ *(hoặc là* $\mu$*-đo được) nếu, với mọi tập con compact* $K$ *của* $T$, *hàm* $f_K$ *là* $\mu_K$*-đo được*.

Điều đó tương đương với việc nói rằng, với mọi tập compact $K$, tồn tại một phân hoạch của $K$ thành một tập $N$ không đáng kể theo $\mu_K$ và một dãy $(K_n)$ các tập compact, sao cho hạn chế của $f$ lên từng $K_n$ là liên tục. Vì việc nói rằng $N$ là không đáng kể theo $\mu_K$ hay rằng nó là không đáng kể theo $\mu$ địa phương (No. 4) là tương đương, ta thấy rằng $f$ là $\mu$-đo được khi và chỉ khi, với mọi tập compact $K$, tồn tại một phân hoạch của $K$ thành một tập $N$ không đáng kể theo $\mu$ địa phương và một dãy $(K_n)$ các tập compact sao cho $f_{K_n}$ liên tục với mọi $n$. Định nghĩa này trùng với Định nghĩa 1 của Ch. IV, §5, No. 1, và do đó ta thu lại khái niệm thông thường về hàm đo được khi $T$ là compact địa phương.

Một tập con $A$ của $T$ được gọi là đo được nếu hàm đặc trưng của nó là đo được. Khi $A$ là $\mu$-đo được và $\mu^\bullet(A) < +\infty$, số này chỉ được ký hiệu là $\mu(A)$ và được gọi là *độ đo* của $A$. Tương tự, ta viết $\mu(f)$ cho $\mu^\bullet(f)$ khi $f$ là $\geqslant 0$, $\mu$-đo được, và $\mu^\bullet(f) < +\infty$.

Nếu $\theta$ là một độ đo phức trên $T$, thì một hàm $f$ (resp. một tập con của $T$) được gọi là $\theta$-đo được nếu nó đo được đối với độ đo dương $|\theta|$. Các kết quả dưới đây có thể được mở rộng cho các độ đo phức.

#### Ví dụ {#int-ix-s1-n5-exa-1 .statement}

— Cho $L$ là một tập con compact của $T$, $\lambda$ là một độ đo trên $L$, và $\mu$ là độ đo trên $T$ được xác định bởi $\lambda$ (No. 3, *Ví dụ 2*). Một hàm $f$ xác định trên $T$ là $\mu$-đo được khi và chỉ khi $f_L$ là $\lambda$-đo được. Vì điều kiện này là hiển nhiên cần. Ngược lại, nếu điều kiện ấy được thỏa mãn, thì tồn tại một phân hoạch của $L$ thành một tập $\lambda$-không đáng kể $N$ và một dãy $(L_n)$ các tập compact, sao cho $f_{L_n}$ liên tục với mọi $n$. Nếu $K$ là một tập con compact của $T$, thì tập $K - \bigcup^n (K \cap L_n)$ có giao với $L$ là $\lambda$-không đáng kể, do đó tập này là $\mu$-không đáng kể theo công thức (3) của No. 3, và hạn chế của $f$ trên $K \cap L_n$ là liên tục với mọi $n$.

Định nghĩa 7 cho phép mở rộng, không cần một chứng minh mới, một số kết quả về các hàm đo được sang trường hợp các không gian không compact địa phương. Sau đây là một số kết quả trong đó, và ta sẽ dùng chúng về sau mà không viện dẫn thêm: các tập mở và các tập đóng của $T$ là $\mu$-đo được; các tập $\mu$-đo được lập thành một tribe (Ch. IV, §5, No. 4, Hệ quả 2 của ĐL. 2), chứa các tập Borel của T (loc. cit., Hệ quả 3), và các tập Souslin (Ch. IV, §5, No. 1, Hệ quả 2 của Mệnh đề 3)(1). Các phép đại số thông thường trên các hàm số bảo toàn tính đo được (Ch. IV, §5, No. 3), cũng như các phép lấy giới hạn đếm được (loc. cit., No. 4, ĐL. 2 và Hệ quả 1). Tính chất sau đây đáng được nêu rõ hơn:

#### Mệnh đề 4 {#int-ix-s1-prop-4 .statement}

— Cho $f$ là một hàm dương và $(g_n)_{n \geq 1}$ là một dãy các hàm dương $\mu$-đo được trên T. Đặt $g = \sum_{n \geq 1} g_n$, ta có

$$
\mu^\bullet(fg) = \sum_{n \geq 1} \mu^\bullet(fg_n).
$$

Đặt $h_n = \sum_{i=1}^n g_i$ với mọi $n \geq 1$. Với mọi tập con compact K của T,

$$
\mu_K^\bullet((fh_n)_K) = \sum_{i=1}^n \mu_K^\bullet((f g_i)_K)
$$

theo Mệnh đề 2 của Ch. V, §1, No. 1 áp dụng cho không gian compact K. Chuyển qua giới hạn đối với tập có hướng tăng các tập con compact của T, ta thu được

$$
\mu^\bullet(fh_n) = \sum_{i=1}^n \mu^\bullet(f g_i).
$$

Bây giờ, $fg$ là giới hạn của dãy tăng $(fh_n)_{n \geq 1}$, do đó $\mu^\bullet(fg) = \lim_{n \to \infty} \mu^\bullet(fh_n)$; công thức trên suy ra ngay (4).

#### Hệ quả {#int-ix-s1-n5-cor-1 .statement}

— Cho $(A_n)$ là một dãy các tập con đo được rời nhau từng đôi một, có hợp là A. Với mọi tập con B của T,

$$
\mu^\bullet(A \cap B) = \sum_n \mu^\bullet(A_n \cap B)
$$

và nói riêng

$$
\mu^\bullet(A) = \sum_n \mu^\bullet(A_n).
$$

Trong số các tính chất của các hàm đo được hoặc các tập đo được mà như trên còn mở rộng sang các không gian Hausdorff, ta cũng nêu Mệnh đề 12 của Ch. IV, §5, No. 8 (các họ tập compact $\mu$-trù mật). Do đó, một hàm $f$ nhận giá trị trong một không gian tôpô (Hausdorff hay không) là $\mu$-đo được khi và chỉ khi tập hợp các tập con compact K của T sao cho $f_K$ liên tục là $\mu$-trù mật (*loc. cit.*, No. 10, Mệnh đề 15).

### 6. Các họ có hướng; giá của một độ đo

**Mệnh đề 5. — a)** *Cho H là một tập có hướng tăng các hàm $\geqslant 0$ nửa liên tục dưới trên mọi tập con compact của T. Khi đó*

$$
\mu^\bullet \left( \sup_{h \in H} h \right) = \sup_{h \in H} \mu^\bullet(h).
$$

*b)* *Cho H là một tập có hướng giảm các hàm $\geqslant 0$ nửa liên tục trên trên mọi tập con compact của T. Nếu trong H tồn tại một hàm $h_0$ sao cho $\mu^\bullet(h_0) < +\infty$, thì*

$$
\mu^\bullet \left( \inf_{h \in H} h \right) = \inf_{h \in H} \mu^\bullet(h).
$$

Với mọi tập compact $K \subset T$, ta có trong trường hợp *a)*

$$
\mu^\bullet \left( sup_{h \in H} h \varphi_K \right) = \mu_K^\bullet \left( sup_{h \in H} h_K \right) = sup_{h \in H} \mu_K^\bullet(h_K) = sup_{h \in H} \mu^\bullet(h \varphi_K),
$$

và trong trường hợp *b)*

$$
\mu^\bullet \left( inf_{h \in H} h \varphi_K \right) = \mu_K^\bullet \left( inf_{h \in H} h_K \right) = inf_{h \in H} \mu_K^\bullet(h_K) = inf_{h \in H} \mu^\bullet(h \varphi_K),
$$

(1) Chứng minh của hệ quả này có giá trị không cần sửa đổi cho các tập Souslin trong một không gian compact địa phương không mêtric (GT, IX, §6, No. 9, ĐL. 5).

do Mệnh đề 2 của No. 2, và Mệnh đề 8 của Ch. V, §1, No. 2. Trường hợp *a*) theo ngay, bằng cách chuyển sang supremum theo K (No. 2, Mệnh đề 2). Để xét trường hợp *b*), ký hiệu $\varepsilon$ là một số $> 0$, và chọn một tập compact K sao cho $\mu^\bullet(h_0 \varphi_K) \geqslant \mu^\bullet(h_0) - \varepsilon$. Khi đó ta có (No. 5, Mệnh đề 4) $\mu^\bullet(h_0 \varphi_{C_K}) \leqslant \varepsilon$; do đó, với mọi hàm $h \in H$ sao cho $h \leqslant h_0$, ta có $\mu^\bullet(h \varphi_{C_K}) \leqslant \varepsilon$, và cuối cùng $\mu^\bullet(h \varphi_K) \geqslant \mu^\bullet(h) - \varepsilon$ theo Mệnh đề 4 của No. 5. Vì thế

$$
\mu^\bullet \left( \inf_{h \in H} h \right) \geqslant \mu^\bullet \left( \inf_{h \in H} h \varphi_K \right) = \inf_{h \in H, h \leqslant h_0} \mu^\bullet(h \varphi_K) \geqslant \inf_{h \in H, h \leqslant h_0} \mu^\bullet(h) - \varepsilon.
$$

Do đó vế trái của (6) $\geqslant$ vế phải; bất đẳng thức ngược lại là hiển nhiên, mệnh đề được chứng minh.

#### Hệ quả {#int-ix-s1-n6-cor-1 .statement}

— a) Cho $(U_\alpha)_{\alpha \in I}$ là một họ có hướng tăng các tập con mở của $T$, với hợp $U$. Khi đó $\mu^\bullet(U) = \sup_{\alpha \in I} \mu^\bullet(U_\alpha)$.

b) Cho $(F_\alpha)_{\alpha \in I}$ là một họ có hướng giảm các tập con đóng của $T$, với giao $F$. Nếu tồn tại một $\alpha \in I$ sao cho $\mu^\bullet(F_\alpha)$ là hữu hạn, thì $\mu^\bullet(F) = \inf_{\alpha \in I} \mu^\bullet(F_\alpha)$.

Theo hệ quả trên, tồn tại một tập mở không đáng kể địa phương lớn nhất; điều này biện minh cho định nghĩa sau:

#### Định nghĩa 8 {#int-ix-s1-def-8 .statement}

— *Giá của một số đo $\mu$ trên $T$ được định nghĩa là phần bù của tập mở lớn nhất không đáng kể địa phương theo $\mu$ trong $T$*.

Giá của $\mu$ được ký hiệu $\operatorname{Supp}(\mu)$.

#### Nhận xét 1 {#int-ix-s1-n6-rem-1 .statement}

Nếu $\mu$ là một số đo phức, giá của $\mu$ được định nghĩa là giá của số đo dương $|\mu|$; nó lại là phần bù của tập mở lớn nhất không đáng kể địa phương theo $\mu$.

#### Nhận xét 2 {#int-ix-s1-n6-rem-2 .statement}

Hãy chứng minh rằng các số đo được đưa vào trong *Ví dụ 2* của No. 3 là các số đo có giá compact trong $T$. Cho $\mu$ là một số đo dương trên $T$ có giá là một tập compact $K$, và cho $\nu$ là số đo được xác định bởi $\mu_K$ (theo nghĩa của No. 3). Cho $f \in \mathcal{F}_+(T)$; khi đó

$$
\nu^\bullet(f) = \mu_K^\bullet(f_K) \quad \text{(No. 3, công thức (3))}.
$$

Vì $\mu^\bullet$ tập trung trên $K$, ta cũng có

$$
\mu^\bullet(f) = \mu^\bullet(f \varphi_K) = \mu^\bullet((f_K)^0) = \mu_K^\bullet(f_K),
$$

do đó $\mu^\bullet = \nu^\bullet$, và cuối cùng $\mu = \nu$. Ngược lại, nếu $K$ là một tập compact trong $T$ và $\lambda$ là một số đo trên $K$, và nếu $\mu$ là số đo trên $T$ được xác định bởi $\lambda$, thì $\mu^\bullet(\mathbf{C}K) = 0$ (No. 3, công thức (3)); do đó, giá của $\mu$ được chứa trong $K$, suy ra compact.

### 7. Bao trên và tổng của các số đo

#### Mệnh đề 6 {#int-ix-s1-prop-6 .statement}

— *Cho $(\lambda_\alpha)_{\alpha \in A}$ là một họ tăng có hướng các độ đo trên $T$, và đặt $p = \sup_\alpha \lambda_\alpha^\bullet$. Để họ $(\lambda_\alpha)$ bị chặn trên trong $\mathcal{M}(T)$, điều kiện cần và đủ là bao $p$ địa phương bị chặn. Khi đó họ $(\lambda_\alpha)$ có một cận trên đúng $\lambda$ trong $\mathcal{M}(T)$, và $\lambda^\bullet = p$. Với mọi tập compact $K$, độ đo $\lambda_K$ là cận trên đúng của các độ đo $(\lambda_\alpha)_K$ trong $\mathcal{M}(K)$*.

Nếu họ $(\lambda_\alpha)$ bị chặn trên trong $\mathcal{M}(T)$, thì $p$ hiển nhiên địa phương bị chặn. Ngược lại, giả sử $p$ địa phương bị chặn, và hãy chứng minh rằng nó thỏa mãn các điều kiện 1) và 2) của Mệnh đề 2 b) của No. 2. Đối với 2), điều này suy ra từ các đẳng thức sau:

$$
p(f) = \sup_\alpha \lambda_\alpha^\bullet(f) = \sup_\alpha \sup_K \lambda_\alpha^\bullet(f \varphi_K) = \sup_K \sup_\alpha \lambda_\alpha^\bullet(f \varphi_K) = \sup_K p(f \varphi_K).
$$

Mặt khác, cho K là một tập compact; bao $p_K$ bằng với bao trên của các bao $(\lambda_\alpha^\bullet)_K$ và nó bị chặn vì $p$ địa phương bị chặn. Do đó các độ đo $(\lambda_\alpha)_K$ có một cận trên đúng $\lambda_K$ trong $\mathcal{M}(K)$, và $\lambda_K^\bullet = p_K$ (Ch. V, §1, No. 4, Mệnh đề 11). Vì vậy điều kiện 1) của Mệnh đề 2 b) của No. 2 được thỏa mãn, do đó tồn tại một độ đo $\lambda$ trên T sao cho $\lambda^\bullet = p$; rõ ràng $\lambda$ là cận trên đúng của các độ đo $\lambda_\alpha$.

#### Định nghĩa 9 {#int-ix-s1-def-9 .statement}

*Cho $(\mu_i)_{i \in I}$ là một họ các độ đo trên T. Cho A là tập các tập con hữu hạn của I; với mọi $\alpha \in A$ đặt $\lambda_\alpha = \sum_{i \in \alpha} \mu_i$. Nếu họ $(\lambda_\alpha)$ có một cận trên đúng $\mu$ trong $\mathcal{M}(T)$, thì họ $(\mu_i)$ được gọi là cộng được, $\mu$ được gọi là tổng của họ $(\mu_i)$, và ta viết $\mu = \sum_{i \in I} \mu_i$.*

Định nghĩa này mở rộng định nghĩa ở Ch. V, §2, No. 1.

#### Mệnh đề 7 {#int-ix-s1-prop-7 .statement}

*Để họ $(\mu_i)_{i \in I}$ cộng được, với tổng $\mu$, điều kiện cần và đủ là bao $p = \sum_{i \in I} \mu_i^\bullet$ địa phương bị chặn, trong trường hợp đó $p = \mu^\bullet$. Với mọi tập con compact K của T, họ $((\mu_i)_K)_{i \in I}$ khi đó cộng được trong $\mathcal{M}(K)$, và $\mu_K = \sum_{i \in I} (\mu_i)_K$.*

Với các ký hiệu như ở ĐN. 9, $\lambda_\alpha^\bullet = \sum_{i \in \alpha} \mu_i^\bullet$ với mọi tập con hữu hạn $\alpha$ của I (No. 2, *Nhận xét* 1). Mệnh đề này là hệ quả ngay lập tức của Mệnh đề 6.

Quan hệ $\mu_K = \sum_{i \in I} (\mu_i)_K$ và Mệnh đề 2 của Ch. V, §2, No. 2 suy ra kết quả sau:

#### Mệnh đề 8 {#int-ix-s1-prop-8 .statement}

*Cho $\mu$ là tổng của một họ cộng được $(\mu_i)_{i \in I}$ các độ đo trên T. Để một ánh xạ f từ T vào một không gian tôpô F (Hausdorff hay không) là $\mu$-đo được, điều kiện cần và đủ là f là $\mu_i$-đo được với mọi $i \in I$.*

### 8. Các phép nghiền

#### Định nghĩa 10 {#int-ix-s1-def-10 .statement}

*Người ta gọi một phép nghiền của T đối với $\mu$, hay một $\mu$-phép nghiền, bất kỳ họ đếm được địa phương $(K_\alpha)_{\alpha \in A}$ gồm các tập con compact rời nhau từng đôi một của T sao cho tập $N = T - \bigcup_{\alpha \in A} K_\alpha$ là địa phương $\mu$-không đáng kể.*

#### Mệnh đề 9 {#int-ix-s1-prop-9 .statement}

*a) Tồn tại một phân hoạch $(K_\alpha)_{\alpha \in A}$ của T đối với $\mu$.
b) Cho $(K_\alpha)_{\alpha \in A}$ là một phân hoạch của T đối với $\mu$. Nếu $\mu_\alpha$ là độ đo trên T được xác định bởi $\mu_{K_\alpha}$ (No. 3, Ví dụ 2), thì họ $(\mu_\alpha)_{\alpha \in A}$ là có thể cộng được,* tổng của nó bằng $\mu$, và, với mọi hàm $f \in \mathcal{F}_+(T)$,

$$
\mu^\bullet(f) = \sum_{\alpha \in A} \mu_\alpha^\bullet(f) = \sum_{\alpha \in A} \mu_{K_\alpha}^\bullet(f_{K_\alpha}) . \tag{1}
$$

Để một ánh xạ $g$ từ $T$ vào một không gian tôpô $G$ (Hausdorff hay không) là $\mu$-đo được, điều kiện cần và đủ là $g_{K_\alpha}$ là $\mu_{K_\alpha}$-đo được với mọi $\alpha \in A$.

A) *Sự tồn tại của một phân hoạch*:

Chứng minh là lặp lại chứng minh của Mệnh đề 14 của Ch. IV, §5, No. 9, với một vài sửa đổi nhỏ. Cho $\mathcal{K}$ là tập hợp các tập con compact $K$ của $T$ sao cho $\mathrm{Supp}(\mu_K) = K$, và cho $\mathcal{H}$ là tập hợp (được sắp thứ tự bởi bao hàm) các tập con $\mathcal{L}$ của $\mathcal{K}$ gồm các tập rời nhau từng đôi một. Trước hết, hãy chứng minh rằng mọi phần tử $\mathcal{L}$ của $\mathcal{H}$ đều là *địa phương đếm được*. Cho $x$ là một điểm của $T$, và $V$ là một lân cận mở của $x$ sao cho $\mu^\bullet(V) < +\infty$; cho $\mathcal{L}_V$ là tập hợp các $K \in \mathcal{L}$ cắt $V$. Nếu $(K_i)_{1 \leq i \leq n}$ là một dãy hữu hạn gồm các phần tử phân biệt của $\mathcal{L}_V$, ta có, theo Hệ quả của Mệnh đề 4,

$$
\sum_{i=1}^n \mu^\bullet(K_i \cap V) = \mu^\bullet\left(V \cap \left( \bigcup_{i=1}^n K_i \right) \right) \leq \mu^\bullet(V),
$$

vì các $K_i$ rời nhau từng đôi một. Do đó,

$$
\sum_{K \in \mathcal{L}_V} \mu^\bullet(K \cap V) < +\infty.
$$

$\mu^\bullet(K \cap V) = \mu_K^\bullet(K \cap V) > 0$ với mọi $K \in \mathcal{L}_V$, vì $K \cap V$ là khác rỗng, mở trong $K$, và giá đỡ của $\mu_K$ là toàn bộ $K$; do đó $\mathcal{L}_V$ là đếm được, và quả thật $\mathcal{L}$ là địa phương đếm được. Rõ ràng $\mathcal{H}$ là quy nạp, và không rỗng (ta có $\varnothing \in \mathcal{H}$). Vì thế, hãy để $\mathfrak{H}$ là một phần tử cực đại của $\mathcal{H}$. Ta sẽ chứng minh rằng tập $N = T - \bigcup_{K \in \mathfrak{H}} K$ là địa phương không đáng kể. Theo Mệnh đề 2, chỉ cần kiểm tra rằng $\mu^\bullet(N \cap L) = 0$ với mọi tập compact $L$, hay cũng có thể nói rằng $\mu_L^\bullet(N \cap L) = 0$. Ta sẽ lập luận bằng phản chứng. Vì thế, giả sử rằng $\mu_L^\bullet(N \cap L) > 0$. Vì tập các $K \in \mathfrak{H}$ cắt $L$ là đếm được, $N \cap L$ là $\mu_L$-khả đo; do đó tồn tại một tập compact $J$ được chứa trong $N \cap L$ sao cho $\mu_L^\bullet(J) > 0$. Hãy để $S$ là giá đỡ của độ đo khác không $(\mu_L)_J = \mu_J$; nó được chứa trong $N$, độ đo $\mu_S$ là khác không, và $\mathrm{Supp}(\mu_S) = S$ (Ch. IV, §5, No. 7, Bổ đề 2). Tập $\mathfrak{H} \cup \{S\}$ do đó thuộc $\mathcal{H}$, mâu thuẫn với tính cực đại của $\mathfrak{H}$. Điều này chứng minh sự tồn tại của một phép nén.

(1) Sau này ta sẽ thấy (§2, No. 2) rằng $\mu_\alpha$ là độ đo $\varphi_{K_\alpha} \cdot \mu$.

B) Chứng minh của (7):
Với mọi $\alpha \in A$, $\mu_\alpha^\bullet(f) = \mu_{K_\alpha}^\bullet(f_{K_\alpha}) = \mu^\bullet(f \varphi_{K_\alpha})$ theo công thức (3) của No. 3 và Mệnh đề 2 a) của No. 2; các công thức này cho thấy rằng gánh nặng $\sum_{\alpha \in A} \mu_\alpha^\bullet$ là $\leq \mu^\bullet$, do đó họ $(\mu_\alpha)_{\alpha \in A}$ là khả tổng (No. 7, Mệnh đề 7). Vậy chỉ cần chứng minh rằng $\mu = \sum_{\alpha \in A} \mu_\alpha$, tức là thiết lập công thức
$$
\mu_K^\bullet = \sum_{\alpha \in A} (\mu_\alpha)_K^\bullet
$$
với mọi tập con compact K của T. Bây giờ, K đã cố định, tập $A'$ gồm các $\alpha \in A$ sao cho $K_\alpha$ cắt K là đếm được. Hãy lấy $g \in \mathcal{F}_+(K)$; khi đó $g^0 = g^0 \varphi_N + \sum_{\alpha \in A} g^0 \varphi_{K_\alpha}$, và $g^0 \varphi_{K_\alpha} = 0$ với $\alpha \in A - A'$; theo Mệnh đề 4 của No. 5, suy ra $\mu^\bullet(g^0) = \sum_{\alpha \in A} \mu^\bullet(g^0 \varphi_{K_\alpha})$, do đó
$$
\mu_K^\bullet(g) = \mu^\bullet(g^0) = \sum_{\alpha \in A} \mu^\bullet(g^0 \varphi_{K_\alpha}) = \sum_{\alpha \in A} \mu_\alpha^\bullet(g^0) = \sum_{\alpha \in A} (\mu_\alpha)_K^\bullet(g);
$$
vậy (8) được thiết lập.

C) Tính khả đo:
Để một hàm $g$ xác định trên T là $\mu$-khả đo, điều kiện cần và đủ là nó $\mu_\alpha$-khả đo với mọi $\alpha \in A$ (No. 7, Mệnh đề 8); nhưng điều này tương đương với việc $g_{K_\alpha}$ là $\mu_{K_\alpha}$-khả đo với mọi $\alpha \in A$ (No. 5, Ví dụ). Q.E.D.

Như trong Mệnh đề 14 của Ch. IV, §5, No. 9, ta có thể yêu cầu các tập compact $K_\alpha$ thuộc về một tập hợp trù mật theo $\mu$ của các tập con compact của T, đã cho trước. Ta chỉ cần kết quả sau đây, và sẽ chứng minh trực tiếp:

#### Mệnh đề 10 {#int-ix-s1-prop-10 .statement}

— *Nếu g là một ánh xạ $\mu$-đo được nhận giá trị trong một không gian tôpô G (Hausdorff hay không), thì tồn tại một $\mu$-phân hoạch $(L_\beta)_{\beta \in B}$ của T sao cho các hạn chế $g_{L_\beta}$ đều liên tục với mọi $\beta \in B$.*

Xét một $\mu$-phân hoạch $(K_\alpha)_{\alpha \in A}$ của T. Vì ánh xạ $g$ là đo được, với mỗi $\alpha \in A$ tồn tại một phân hoạch của $K_\alpha$ thành một dãy $(K_{\alpha n})$ các tập compact và một tập không đáng kể địa phương $N_\alpha$, sao cho hạn chế của $g$ lên từng tập $K_{\alpha n}$ là liên tục. Khi đó họ $(K_{\alpha n})_{(\alpha, n) \in A \times \mathbf{N}}$ là phân hoạch cần tìm. Thật vậy, nó là địa phương đếm được, và tập $N' = N \cup (\bigcup_\alpha N_\alpha)$ là không đáng kể địa phương, vì một tập compact cắt nhiều nhất một vô hạn đếm được các tập $N_\alpha$.

#### Chú giải {#int-ix-s1-n8-sch-1 .statement}

— Cho $(K_\alpha)_{\alpha \in A}$ là một phân hoạch của T, và đặt $N = T - \bigcup_\alpha K_\alpha$. Ký hiệu $T'$ là không gian địa phương compact thu được bằng cách trang bị cho $T'$ tôpô tổng của các tôpô của các không gian con $K_\alpha$ và bất kỳ tôpô địa phương compact nào trên $N$ (trừ khi được nói rõ ngược lại, $N$ sẽ luôn được trang bị tôpô rời rạc). Với mỗi $\alpha \in A$, đặt $i_\alpha$ là đơn ánh chính tắc của $K_\alpha$ vào $T'$, và đặt $\mu'_\alpha$ là đo trên $T'$ là ảnh của $\mu_{K_\alpha}$ qua $i_\alpha$. Họ $(\mu'_\alpha)$ là khả tổng: vì, nếu $f$ là một hàm liên tục trên $T'$ có giá compact, thì $\operatorname{Supp}(f)$ chỉ cắt $K_\alpha$ đối với một số hữu hạn chỉ số $\alpha$. Đặt $\mu' = \sum_{\alpha \in A} \mu'_\alpha$. Tập $N$ là không đáng kể địa phương đối với $\mu'$, vì nó như thế đối với từng $\mu'_\alpha$ (Mệnh đề 9), nên họ $(K_\alpha)_{\alpha \in A}$ là một $\mu'$-phân hoạch của $T'$; nay, đo cảm sinh bởi $\mu'$ trên $K_\alpha$ hiển nhiên là $\mu_{K_\alpha}$ và công thức (7), áp dụng cho $\mu$ và cho $\mu'$, cho thấy rằng $\mu^\bullet = \mu'^\bullet$. Tương tự, khẳng định cuối cùng của mệnh đề của Mệnh đề 9, áp dụng cho $\mu$ và cho $\mu'$, cho thấy rằng *các ánh xạ đo được là như nhau đối với hai đo $\mu$ và $\mu'$*.

Hai tính chất này cho phép quy hầu như toàn bộ lý thuyết tích phân theo $\mu$ về lý thuyết được xây dựng cho các không gian địa phương compact. Các xét này sẽ được trình bày ở No. 10.

Sau đây là một ứng dụng khác của khái niệm phân hoạch:

#### Mệnh đề 11 {#int-ix-s1-prop-11 .statement}

*Cho $X$ là một tập con $\mu$-đo được của $T$. Tồn tại một họ địa phương đếm được $(L_\alpha)_{\alpha \in A}$ gồm các tập con compact của $X$, từng đôi một rời nhau, sao cho $X - \bigcup_{\alpha \in A} L_\alpha$ là địa phương $\mu$-không đáng kể. Nếu, ngoài ra, $X$ là hợp của một dãy $(X_n)$ các tập hợp đo được sao cho $\mu^\bullet(X_n) < +\infty$, thì tập $B$ các $\alpha \in A$ sao cho $\mu^\bullet(L_\alpha) \neq 0$ là đếm được, và $X - \bigcup_{\beta \in B} L_\beta$ là địa phương $\mu$-không đáng kể.*

Cho $f$ là hàm đặc trưng của $X$, và cho $(K_\alpha)_{\alpha \in A}$ là một phân hoạch của $T$ sao cho hạn chế của $f$ lên từng $K_\alpha$ là liên tục (Mệnh đề 10). Khi đó tập $L_\alpha = K_\alpha \cap X$ là compact với mọi $\alpha \in A$, và $(L_\alpha)_{\alpha \in A}$ là họ mong muốn. Xét sang mệnh đề thứ hai; các tập hợp đo được $X_n$ có thể rõ ràng được giả sử là rời nhau, và chỉ cần chứng minh mệnh đề đó cho từng tập trong số chúng. Nói cách khác, nếu cần đổi ký hiệu, ta có thể giả sử rằng $\mu^\bullet(X) < +\infty$. Tập $B$ các $\alpha \in A$ sao cho $\mu^\bullet(L_\alpha) > 0$ khi đó là đếm được, và chỉ còn phải chứng minh rằng tập $N = \bigcup_{\alpha \in A - B} L_\alpha$ là địa phương không đáng kể. Nhưng $K$ là một tập compact; vì họ $(L_\alpha)_{\alpha \in A}$ là địa phương đếm được, nên tập $K \cap N$ là hợp của một họ con *đếm được* của họ $(K \cap L_\alpha)_{\alpha \in A - B}$, và do đó tập này là địa phương không đáng kể. Khi đó điều tương tự cũng đúng với $N$ (No. 2, Mệnh đề 2) và mệnh đề được chứng minh.

### 9. Tích phân trên

#### Định nghĩa 11 {#int-ix-s1-def-11 .statement}

*Với mọi hàm $f \in \mathcal{F}_+(T)$, người ta định nghĩa tích phân trên của $f$ (đối với độ đo $\mu$) là số dương hữu hạn hoặc vô hạn*

$$
\mu^*(f) = \inf_g \mu^\bullet(g),
$$

*trong đó $g$ chạy qua tập các hàm nửa liên tục dưới mà $\geqslant f$.*

Các ký hiệu $\int^* f(t) d\mu(t)$ và $\int^* f d\mu$ cũng được dùng. Khi $T$ là địa phương compact, định nghĩa này trùng với định nghĩa thông thường (Ch. V, §1, No. 1, Mệnh đề 4). Rõ ràng $\mu^\bullet(f) \leqslant \mu^*(f)$, với đẳng thức khi $f$ nửa liên tục dưới. Nếu $A$ là một tập con của $T$, ta viết $\mu^*(A)$ thay cho $\mu^*(\varphi_A)$, và số này được gọi là *độ đo ngoài* của $A$. Các tập hợp đo được có độ đo ngoài hữu hạn được gọi là *các tập hợp khả tích*, như trong trường hợp các không gian địa phương compact.

Một hàm $f$ có giá trị trong một không gian Banach hoặc trong $\overline{\mathbf{R}}$ sao cho $\mu^*(|f|) = 0$ được gọi là *không đáng kể*; một tập $A \subset T$ được gọi là không đáng kể nếu $\varphi_A$ là không đáng kể, tức là nếu $\mu^*(A) = 0$. Cụm từ *hầu khắp nơi* được đưa vào như ở Ch. IV, §2, No. 3.

#### Mệnh đề 12 {#int-ix-s1-prop-12 .statement}

*Hàm $\mu^*$ là một gánh nặng trên $T$.*

Các tính chất $a), b), c)$ của Định nghĩa 1 của No. 1 là hiển nhiên. Chứng minh của tính chất $d)$ giống hệt chứng minh của Định lý 3 của Ch. IV, §1, No. 3, khi xét đến các Mệnh đề 4 và 5 *a)*.

#### Hệ quả {#int-ix-s1-n9-cor-1 .statement}

*Một hàm $f$, với giá trị trong một không gian Banach hoặc trong $\overline{\mathbf{R}}$, là không đáng kể khi và chỉ khi $f(t) = 0$ hầu khắp nơi.*

Ta ngay lập tức quy về trường hợp của một hàm dương. Chứng minh khi đó giống hệt chứng minh của Định lý 1 của Ch. IV, §2, No. 3.

#### Mệnh đề 13 {#int-ix-s1-prop-13 .statement}

*Với mọi tập con $A$ của $T$, $\mu^*(A)$ là cận dưới đúng của các độ đo ngoài của các tập mở chứa $A$.*

Chứng minh giống hệt chứng minh của Mệnh đề 19 của Ch. IV, §1, No. 4.

#### Định nghĩa 12 {#int-ix-s1-def-12 .statement}

*Cho $f$ là một hàm được định nghĩa trên $T$, với giá trị trong một không gian Banach hoặc trong $\overline{\mathbf{R}}$. Người ta nói rằng $f$ là điều độ đối với độ đo $\mu$, hay $\mu$-điều độ, nếu $f$ bằng không trên phần bù của một hợp đếm được các tập mở khả tích. Một tập con $A$ của $T$ được gọi là điều độ nếu hàm $\varphi_A$ là điều độ. Độ đo $\mu$ được gọi là điều độ nếu hàm $1$ là $\mu$-điều độ.*

Chẳng hạn, vì bao trùm $\mu^\bullet$ bị chặn địa phương, mọi tập con compact $K$ của $T$ đều được chứa trong một tập mở $V$ sao cho $\mu^\bullet(V) < +\infty$; do đó một hàm bằng không ở ngoài một tập compact là điều độ. Một hàm không đáng kể là điều độ. Các nhận xét theo sau Định nghĩa 2 của Ch. V, §1, No. 2 có thể ngay lập tức được mở rộng sang bối cảnh hiện tại. Đặc biệt, tổng của một dãy các hàm dương điều độ là điều độ.

#### Nhận xét 1 {#int-ix-s1-n9-rem-1 .statement}

Trên một không gian Lindelöf $T$ (TG, IX, Phụ lục I, Định nghĩa 1),¹ và đặc biệt trên một không gian Souslin (ở đó, hệ quả của Mệnh đề 1), mọi độ đo đều điều độ. Thật vậy, các tập mở có độ đo hữu hạn tạo thành một phủ của $T$, từ đó có thể trích ra một phủ đếm được của $T$.

#### Nhận xét 2 {#int-ix-s1-n9-rem-2 .statement}

Tuy nhiên, hãy lưu ý rằng sự tồn tại của một dãy các tập Borel có độ đo hữu hạn đối với $\mu$, có hợp là $T$, không nhất thiết suy ra sự tồn tại của một dãy các tập mở có độ đo hữu hạn có hợp là $T$ (nói cách khác, không suy ra rằng $\mu$ là điều độ). Xem Bài tập 8.

#### Mệnh đề 14 {#int-ix-s1-prop-14 .statement}

Cho $f \in \mathcal{F}_+(T)$. Nếu $f$ là $\mu$-điều độ, thì $\mu^*(f) = \mu^\bullet(f)$; nếu $f$ không $\mu$-điều độ, thì $\mu^*(f) = +\infty$.

Nếu $\mu^*(f) < +\infty$, tồn tại một hàm nửa liên tục dưới $g \geq f$ sao cho $\mu^\bullet(g) < +\infty$. Với mọi $n \in \mathbf{N}$, đặt $G_n$ là tập các $t \in T$ sao cho $g(t) > 1/n$; tập $G_n$ là mở, ta có $\mu^\bullet(G_n) \leq n \mu^\bullet(g) < +\infty$, và $f$ bằng không ở ngoài hợp của các $G_n$: do đó hàm $f$ là điều độ.

Tiếp theo, hãy chứng minh rằng $\mu^*$ và $\mu^\bullet$ có cùng giá trị đối với các hàm điều độ. Vì $\mu^*$ và $\mu^\bullet$ là các bao trùm, nên chỉ cần thiết lập quan hệ $\mu^*(f) = \mu^\bullet(f)$ khi $f$ là một hàm dương, bị chặn trên bởi một hằng số M, và bằng không ở ngoài một tập mở G có độ đo hữu hạn, điều mà ta sẽ làm ngay bây giờ.

Độ đo $\mu$ là cận trên đúng, trong $\mathcal{M}(T)$, của một họ tăng có hướng $(\mu_i)_{i \in I}$ các độ đo có giá compact: điều này suy ra ngay từ Mệnh đề 9 của No. 8. Cho $g$ là một hàm nửa liên tục dưới trên T, nằm giữa $f$ và hàm nửa liên tục dưới $M \varphi_G$. Đặt $\nu_i = \mu - \mu_i$; khi đó $\mu^\bullet = \mu_i^\bullet + \nu_i^\bullet$ (No. 2, Nhận xét 1), do đó
$$
\mu^\bullet(g) - \mu^\bullet(f) = (\mu_i^\bullet(g) - \mu_i^\bullet(f)) + (\nu_i^\bullet(g) - \nu_i^\bullet(f))
$$
$$
\leq (\mu_i^\bullet(g) - \mu_i^\bullet(f)) + \nu_i^\bullet(M \varphi_G).
$$
Ta có $\nu_i^\bullet(M \varphi_G) = \mu^\bullet(M \varphi_G) - \mu_i^\bullet(M \varphi_G)$ và $\mu^\bullet(M \varphi_G) = \sup \mu_i^\bullet(M \varphi_G)$ (No. 7, Mệnh đề 6); vì thế số $\nu_i^\bullet(M \varphi_G)$ có thể được làm tùy ý nhỏ bằng cách chọn $i$ thích hợp. Vậy mọi việc quy về việc chứng minh rằng, với mọi số $c > 0$ và mọi chỉ số $i \in I$, ta có thể tìm được một hàm nửa liên tục dưới $g$ nằm giữa $f$ và $M \varphi_G$, sao cho $\mu_i^\bullet(g) - \mu_i^\bullet(f) \leq c$. Bây giờ, cho L là giá compact của độ đo $\mu_i$, và cho $\lambda$ là độ đo $(\mu_i)_L$; vì $\mu_i$ tập trung trên L, ta có $\mu_i^\bullet(h) = \mu_i^\bullet(h \varphi_L) = \lambda^\bullet(h_L)$ đối với mọi hàm $h \in \mathcal{F}_+(T)$ (No. 1, Bổ đề 1 và No. 2, Mệnh đề 2); do đó
$$
\mu_i^\bullet(g) - \mu_i^\bullet(f) = \lambda^\bullet(g_L) - \lambda^\bullet(f_L).
$$

¹ Phụ lục được dẫn trong TG không xuất hiện trong GT (bản dịch một ấn bản trước của Ch. IX). Các không gian Lindelöf được định nghĩa trong GT, I, §9, Bài tập 14; bài tập này và định nghĩa của không gian Souslin (GT, IX, §6, No. 2, Định nghĩa 2) bao quát phần cần dùng ở đây.

Vì L là compact; do đó $\lambda^* = \lambda^*$, vì thế tồn tại một hàm nửa liên tục dưới $h$ xác định trên L, thỏa $\geq f_L$ và sao cho $\lambda^*(h) \leq \lambda^*(f_L) + c$. Vì tập L đóng trong T, hàm k bằng h trên L, và bằng $+\infty$ trên $T - L$, là nửa liên tục dưới trên T và thỏa $\geq f$, và $\lambda^*(k_L) = \lambda^*(h) \leq \lambda^*(f_L) + c$. Chỉ còn đặt $g = \inf(k, M \varphi_G)$: $g$ là nửa liên tục dưới, $g \geq f$ và

$$
\mu_i^*(g) \leq \mu_i^*(k) = \lambda^*(k_L) \leq \lambda^*(f_L) + c = \mu_i^*(f) + c.
$$

#### Hệ quả 1 {#int-ix-s1-prop-14-cor-1 .statement}

*Để một hàm không đáng kể, cần và đủ là nó địa phương không đáng kể và điều tiết.*

#### Hệ quả 2 {#int-ix-s1-prop-14-cor-2 .statement}

*Để một hàm $f$ địa phương không đáng kể, cần và đủ là mọi $x \in T$ đều có một lân cận V sao cho $f \varphi_V$ không đáng kể.*

Thật vậy, nếu tính chất này được thỏa mãn, thì $f \varphi_K$ không đáng kể đối với mọi tập compact K, và do đó $f$ là địa phương không đáng kể (No. 2, Mệnh đề 2). Ngược lại, giả sử $f$ là địa phương không đáng kể, và cho $x$ là một điểm của T; $x$ có một lân cận mở V có số đo hữu hạn. Khi ấy hàm $f \varphi_V$ là địa phương không đáng kể và điều tiết, nên không đáng kể.

#### Hệ quả 3 {#int-ix-s1-prop-14-cor-3 .statement}

*Cho $f$ là một hàm điều tiết xác định trên T. Tồn tại một dãy $(K_n)$ các tập compact từng đôi một rời nhau, và một tập H không đáng kể, sao cho $f = f \varphi_H + \sum_n f \varphi_{K_n}$.*

Thật vậy, cho G là một tập là hợp đếm được của các tập mở khả tích, sao cho $f$ bằng không ngoài G; khi đó G là hợp của một dãy $(K_n)$ các tập compact từng đôi một rời nhau và một tập H địa phương không đáng kể (No. 8, Mệnh đề 11); nhưng H là điều tiết, do đó không đáng kể.

#### Hệ quả 4 {#int-ix-s1-prop-14-cor-4 .statement}

*Nếu $\mu$ và $\nu$ là hai độ đo trên T sao cho $\mu^* = \nu^*$, thì $\mu = \nu$.*

Vì, đẳng thức $\mu^* = \nu^*$ suy ra rằng $\mu^*(f) = \nu^*(f)$ đối với mọi hàm dương $f$ được điều hòa đối với $\mu$ và $\nu$, do đó đối với mọi hàm dương có giá đỡ compact; suy ra $\mu^* = \nu^*$ (No. 2, Mệnh đề 2), rồi $\mu = \nu$ (No. 2, Hệ quả của Mệnh đề 2).

#### Hệ quả 5 {#int-ix-s1-prop-14-cor-5 .statement}

*Nếu $\mu$ là một độ đo được điều hòa trên T, thì tồn tại một dãy $(\mu_n)_{n \in \mathbf{N}}$ các độ đo có giá đỡ compact sao cho $\mu = \sum_{n \in \mathbf{N}} \mu_n$.*

Theo giả thiết, hàm hằng 1 là $\mu$-điều hòa. Hãy áp dụng Hệ quả 3 cho trường hợp $f = 1$; do đó, tồn tại một dãy $(K_n)_{n \in \mathbf{N}}$ các tập con compact từng đôi một rời nhau của T sao cho $1 = \sum_{n \in \mathbf{N}} \varphi_{K_n}$ $\mu$-hầu khắp mọi nơi. Gọi $\mu_n$ là độ đo trên T được xác định bởi độ đo $\mu_{K_n}$ trên $K_n$ (No. 3, Ví dụ 2). Ta biết (No. 6, Nhận xét 2) rằng $\mu_n$ có giá đỡ compact, và rằng $\mu_n^\bullet(f) = \mu^\bullet(f \varphi_{K_n})$ với $f \in \mathcal{F}_+(T)$. Bây giờ, $f$ bằng $\sum_{n \in \mathbf{N}} f \varphi_{K_n}$ $\mu$-hầu khắp mọi nơi, do đó

$$
\mu^\bullet(f) = \sum_{n \in \mathbf{N}} \mu^\bullet(f \varphi_{K_n}) = \sum_{n \in \mathbf{N}} \mu_n^\bullet(f).
$$

Suy ra $\mu = \sum_{n \in \mathbf{N}} \mu_n$ (No. 7, Mệnh đề 7).

### 10. Lý thuyết tích phân

#### Định nghĩa 13 {#int-ix-s1-def-13 .statement}

— *Cho* $p \in [1, +\infty[$; *người ta ký hiệu bởi* $\overline{\mathcal{L}}^p(T, \mu)$ *(tương ứng* $\overline{\mathcal{L}}_F^p(T, \mu)$ *nếu F là một không gian Banach) tập hợp các ánh xạ* $\mathbf{f}$ *từ T vào* $\overline{\mathbf{R}}$ *(tương ứng vào F) sao cho chúng đo được theo $\mu$ và thỏa mãn* $\mu^\bullet(|\mathbf{f}|^p) < +\infty$. *Người ta ký hiệu bởi* $\mathcal{L}^p(T, \mu)$ *(tương ứng* $\mathcal{L}_F^p(T, \mu)$*) tập hợp các phần tử được điều hòa theo $\mu$ của* $\overline{\mathcal{L}}^p(T, \mu)$ *(tương ứng* $\overline{\mathcal{L}}_F^p(T, \mu)$*).*

Ta sẽ viết $\overline{N}_p(\mathbf{f}) = \left( \mu^\bullet(|\mathbf{f}|^p) \right)^{1/p}$, $N_p(\mathbf{f}) = \left( \mu^*(|\mathbf{f}|^p) \right)^{1/p}$. Ta ký hiệu $\overline{N}_\infty(\mathbf{f})$ là cận dưới đúng của các số $k \geq 0$ sao cho $|\mathbf{f}| \leq k$ cục bộ $\mu$-hầu khắp mọi nơi; nếu $\overline{N}_\infty(\mathbf{f}) < +\infty$, thì $\mathbf{f}$ được gọi là hầu như bị chặn. Tập hợp các ánh xạ đo được và hầu như bị chặn từ T vào $\overline{\mathbf{R}}$ (tương ứng vào F) được ký hiệu là $\overline{\mathcal{L}}^\infty(T, \mu)$ (tương ứng $\overline{\mathcal{L}}_F^\infty(T, \mu)$). Các phần tử của $\overline{\mathcal{L}}_F^1(T, \mu)$ (tương ứng $\mathcal{L}_F^1(T, \mu)$) được gọi là các hàm khả tích theo nghĩa rộng (tương ứng các hàm khả tích) với giá trị trong F.

Nếu $\mu$ là một độ đo phức, ta đặt

$$
\overline{\mathcal{L}}_F^p(T, \mu) = \overline{\mathcal{L}}_F^p(T, |\mu|) \quad \text{và} \quad \mathcal{L}_F^p(T, \mu) = \mathcal{L}_F^p(T, |\mu|).
$$

Các ký hiệu trên thường được viết tắt thành $\overline{\mathcal{L}}_F^p(\mu)$, $\overline{\mathcal{L}}_F^p$ hoặc $\mathcal{L}^p(\mu)$, $\mathcal{L}^p$, nếu điều đó không dẫn đến nhầm lẫn.

Chúng ta đã thấy ở No. 8 (*Chú giải*) rằng có thể xây dựng một không gian địa phương compact T', có cùng tập nền với T và một tôpô mịn hơn tôpô của T, rồi trang bị cho T' một độ đo $\mu'$ sao cho các hàm đo được theo $\mu$ và các hàm đo được theo $\mu'$ là như nhau, và sao cho các nguyên trên cốt yếu của các hàm dương đối với $\mu$ và $\mu'$ bằng nhau. Suy ra rằng các tập $\overline{\mathcal{L}}_F^p(\mu)$ và $\overline{\mathcal{L}}_F^p(\mu')$ là đồng nhất với nhau đối với $1 \leq p \leq +\infty$ $^{(1)}$. Điều này cũng suy ra ngay không cần chứng minh mới rằng $\overline{\mathcal{L}}_F^p$ là một không gian vectơ, và hàm $\overline{N}_p$ là một bán chuẩn trên $\overline{\mathcal{L}}_F^p(\mu)$, với bán chuẩn đó không gian này đầy đủ.

Cho $\mathbf{f}$ là một phần tử của $\overline{\mathcal{L}}_F^p$ ($1 \leq p < +\infty$); vì ta có $\mu^\bullet(|\mathbf{f}|^p) = \mu'^\bullet(|\mathbf{f}|^p) < +\infty$, Mệnh đề 7 của Ch. V, §1, No. 2 suy ra rằng $\mathbf{f}$ bằng 0 ngoài

(1) Chú ý rằng không gian $\mathcal{L}_F^p(\mu)$ được chứa trong $\mathcal{L}_F^p(\mu')$, nhưng nói chung khác với nó.

hợp của một dãy các tập con compact của T' và một tập địa phương $\mu'$-không đáng kể; vì tập sau đó là địa phương $\mu$-không đáng kể, và mọi tập con compact của T' đều compact trong T, suy ra f địa phương bằng 0 hầu khắp nơi theo $\mu$ đối với một hàm $\mu$-điều độ. Ta ký hiệu $\overline{\mathcal{N}}_F$ (resp. $\mathcal{N}_F$) không gian các hàm địa phương $\mu$-không đáng kể (resp. $\mu$-không đáng kể); do đó ta có $\overline{\mathcal{L}}_F^p = \mathcal{L}_F^p + \overline{\mathcal{N}}_F$, và $\mathcal{N}_F = \mathcal{L}_F^p \cap \overline{\mathcal{N}}_F$ (No. 9, Hệ quả 1 của Mệnh đề 14). Vì vậy không gian $\overline{\mathcal{L}}_F^p / \overline{\mathcal{N}}_F$ có thể được đồng nhất một cách chính tắc với $\mathcal{L}_F^p / \mathcal{N}_F$, và ta kiểm tra ngay rằng sự đồng nhất này bảo toàn chuẩn; không gian thương này được ký hiệu là $L_F^p(\mu)$. Nó có thể được diễn giải như không gian có chuẩn liên kết với mỗi một trong các không gian bán chuẩn $\overline{\mathcal{L}}_F^p(\mu)$ và $\mathcal{L}_F^p(\mu)$; vì $\overline{\mathcal{L}}_F^p$ đầy đủ, điều tương tự đúng với $L_F^p$ và $\mathcal{L}_F^p$.

Tập các hàm f nhận giá trị trong F, liên tục trên T' với giá đỡ compact, trù mật trong $\overline{\mathcal{L}}_F^p(\mu') = \overline{\mathcal{L}}_F^p(\mu)$ (Ch. IV, §3, No. 4, Định nghĩa 2). Ta xét lại các ký hiệu của Chú giải ở No. 8. Vì một tập con compact của T' chỉ cắt một số hữu hạn các tập compact $K_\alpha$, nên mọi hàm liên tục f trên T' với giá đỡ compact đều có thể được viết thành một tổng
$$
f = \sum_{\alpha \in A} f_\alpha + g,
$$
trong đó $f_\alpha$ là, với mọi $\alpha$, phần mở rộng bởi 0 của một hàm liên tục trên $K_\alpha$, trong đó $f_\alpha = 0$ trừ một số hữu hạn chỉ số, và trong đó g là địa phương $\mu$-không đáng kể. Do đó ta có kết quả sau:

#### Mệnh đề 15 {#int-ix-s1-prop-15 .statement}

*Tập các hàm f nhận giá trị trong F, sao cho Supp(f) là compact và sao cho hạn chế của f lên Supp(f) là liên tục, trù mật trong $\overline{\mathcal{L}}_F^p(\mu)$ và trong $\mathcal{L}_F^p(\mu)$, với $1 \leq p < +\infty$.*

Chú ý rằng các hàm này *không phải là* các hàm liên tục *trên* T với giá đỡ compact.

Ta chuyển sang định nghĩa của nguyên.

#### Mệnh đề 16 {#int-ix-s1-prop-16 .statement}

*Tồn tại duy nhất một ánh xạ tuyến tính liên tục $f \mapsto \int f d\mu$, từ không gian $\overline{\mathcal{L}}_F^1(\mu)$ vào F, có tính chất sau:
Nếu f có dạng $t \mapsto g(t)a$, với $a \in F$, và g là một hàm dương, hữu hạn, $\mu$-đo được và thỏa mãn $\mu^*(g) < +\infty$, thì $\int f d\mu = \mu^*(g) \cdot a$.*

Vì thế, các không gian nửa chuẩn $\overline{\mathcal{L}}_F^1(\mu)$ và $\overline{\mathcal{L}}_F^1(\mu')$ là trùng nhau. Vì $\mu^* = \mu'^*$, ánh xạ $f \mapsto \int f d\mu'$ thỏa mãn các điều kiện của mệnh đề. Mặt khác, tập hợp các hàm có dạng $f = g \cdot a$ được xét trong mệnh đề là *toàn phần* trong $\overline{\mathcal{L}}_F^1(\mu')$ (Ch. IV, §3, No. 5, Mệnh đề 10), do đó có tính duy nhất.

Người ta nói rằng $\int f\, d\mu$ là nguyên của $f$ đối với $\mu$, và vectơ này cũng được ký hiệu là $\mu(f)$ hoặc $\int f(t)\, d\mu(t)$.

Vì $\int f\, d\mu = \int f\, d\mu'$ với mọi hàm khả tích cốt yếu nhận giá trị trong $F$, toàn bộ lý thuyết về nguyên cốt yếu được mở rộng sang các độ đo trên các không gian Hausdorff, mà không cần chứng minh mới; từ đó, ta suy ra các kết quả liên quan đến nguyên thông thường bằng cách chỉ xét các hàm điều độ. Đặc biệt, ta trích dẫn các kết quả sau:

— Định lý 3 của Ch. IV, §3, No. 4, phần mở rộng của nó sang $\overline{\mathcal{L}}_F^p$, và hai hệ quả của nó.
— Định lý 4 của Ch. IV, §3, No. 5 (hợp thành với một ánh xạ tuyến tính liên tục) và các hệ quả của nó; các Mệnh đề 9, 11 và 12 của cùng No.
— Tất cả các kết quả của Ch. IV, §3, No. 6, liên quan đến cấu trúc không gian vectơ có thứ tự của $L^p$.
— Tất cả các kết quả của Ch. IV, §3, No. 7, và đặc biệt là định lý Lebesgue.
— Tất cả các kết quả của Ch. IV, §3, No. 8, về các quan hệ giữa các không gian $L_F^p$.
— Định lý 2 của Ch. IV, §4, No. 3 (mệnh đề của định lý Lebesgue riêng cho $L_F^1$).
— Bất đẳng thức Hölder (Ch. IV, §6, No. 4, Định lý 2) và các hệ quả của nó.
— Các quan hệ giữa các không gian $L_F^p$ được thiết lập trong Ch. IV, §6, No. 5.
— Các kết quả về đối ngẫu của các không gian $L^p$ được thiết lập trong Ch. V, §5, No. 8.
— Định lý Dunford–Pettis (Ch. VI, §2, No. 5, Định lý 1), các Hệ quả 1 và 2 của nó, và Mệnh đề 10 của Ch. VI, §2, No. 6 (đối ngẫu của $L_F^1$).

### Bài tập {#int-ix-s1-exercises}

Xem [các bài tập cho § 1](exercises/s1/).
