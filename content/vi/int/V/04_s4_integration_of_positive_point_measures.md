---
book: int
book_title: Integration
chapter: V
chapter_title: INTEGRATION OF MEASURES
section: 4
section_title: Integration of positive point measures
lang: vi
source: int-i-vi
book_pages: INT V.31-INT V.38, INT V.99
pdf_pages: 0286-0293, 0354-0354
extraction: ocr
subsections:
    - "no": 1
      title: Families of point measures
      page: 31
      pdf_page: 286
    - "no": 2
      title: Upper integrals of positive functions with respect to an integral of point measures
      page: 33
      pdf_page: 288
    - "no": 3
      title: Measurability with respect to an integral of point measures
      page: 35
      pdf_page: 290
    - "no": 4
      title: Integration of functions with values in a Banach space, with respect to an integral of point measures
      page: 37
      pdf_page: 292
statements: 10
exercises: 2
content_sha256: 4ee53feccd3bd1c6b2b33713a994e7e740942e223aa765da3c696f4791178f66
translated_from: content/en/int/V/04_s4_integration_of_positive_point_measures.md
source_content_sha256: 3c0c4299b63b198ba8be5789099b080c2d5176490f2fda987ee1745f2a1fbb81
translation_model: gpt-5-6, gpt-5-6-mini, gpt-5.4-mini
translation_run: translate-vi-596d3df3
glossary_version: 34
glossary_terms_sha256: 846956af7f931d2f45763dbba664d26ab7e9eb1973128fd232d8a240d2cc30f2
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 4. TÍCH PHÂN CÁC PHÉP ĐO ĐIỂM DƯƠNG

### 1. Các họ phép đo điểm

Cho X và T là hai không gian địa phương compact, $\pi$ là một ánh xạ từ T vào X, và $g$ là một hàm số hữu hạn $\geqslant 0$ xác định trên T; hai hàm này xác định một ánh xạ $t \mapsto \lambda_t = g(t)\varepsilon_{\pi(t)}$ từ T vào không gian $\mathcal{M}(X)$ của các phép đo trên X, sao cho với mọi $t \in T$, $\lambda_t$ hoặc là một phép đo điểm (Ch. III, §2, No. 4) hoặc bằng 0. Nếu $f$ là một hàm số $\geqslant 0$ xác định trên X, thì $\int^* f(x) d\lambda_t(x) = \int^\bullet f(x) d\lambda_t(x) = f(\pi(t))g(t)$ (nhắc lại quy ước của ta là lấy tích này bằng 0 khi $g(t) = 0$ và $f(\pi(t)) = +\infty$). Mọi hàm (có giá trị trong một không gian tôpô) xác định trên X đều là $\lambda_t$-đo được với mọi $t \in T$. Mọi ánh xạ $f$ từ X vào một không gian Banach F đều là $\lambda_t$-khả tích phân với mọi $t \in T$, và $\int f(x) d\lambda_t(x) = f(\pi(t))g(t)$. Cuối cùng, nếu $f$ là một hàm số tùy ý xác định trên X, để $f$ là $\lambda_t$-khả tích phân thì điều kiện cần và đủ là $f(\pi(t))g(t)$ là hữu hạn, trong trường hợp đó $\int f(x) d\lambda_t(x) = f(\pi(t))g(t)$.

#### Định nghĩa 1 {#int-v-s4-def-1 .statement}

Cho $\mu$ là một phép đo dương trên T. Cặp $(\pi, g)$ được gọi là $\mu$-thích nghi nếu các điều kiện sau được thỏa mãn:
1° Các hàm $\pi$ và $g$ là $\mu$-đo được.
2° Với mọi hàm $f \in \mathcal{K}(X)$, ánh xạ $t \mapsto f(\pi(t))g(t)$ là $\mu$-khả tích phân một cách bản chất.

#### Mệnh đề 1 {#int-v-s4-prop-1 .statement}

Nếu cặp $(\pi, g)$ là $\mu$-thích nghi, thì ánh xạ $\Lambda : t \mapsto \lambda_t = g(t)\varepsilon_{\pi(t)}$ từ T vào $\mathcal{M}_+(X)$ là $\mu$-khả tích phân một cách bản chất theo vô hướng, $\mu$-đo được theo nghĩa mơ hồ và $\mu$-thích đáng. Ngược lại, nếu $\Lambda$ là $\mu$-khả tích phân một cách bản chất theo vô hướng và $\mu$-đo được theo nghĩa mơ hồ, thì hàm $g$ là $\mu$-đo được và hạn chế của $\pi$ lên tập hợp $S$ của $t \in T$ sao cho $g(t) \neq 0$ là $\mu$-đo được.

Giả sử rằng cặp $(\pi, g)$ là $\mu$-thích nghi; với mọi hàm $f \in \mathcal{K}(X)$, hàm $t \mapsto \langle f, \lambda_t \rangle = f(\pi(t))g(t)$ khi đó là khả tích $\mu$-một cách cốt yếu. Ta hãy chỉ ra rằng $t \mapsto \lambda_t$ là đo được $\mu$-theo nghĩa mơ hồ. Thật vậy, trước hết ta chú ý rằng nếu $\pi$ và $g$ liên tục, thì ánh xạ $t \mapsto \lambda_t$ liên tục theo nghĩa mơ hồ. Trong trường hợp tổng quát, tập hợp các tập con compact $K$ của $T$ sao cho các hạn chế của $\pi$ và $g$ lên $K$ là liên tục là $\mu$-trù mật (Ch. IV, §5, No. 10, Prop. 15); nếu $K$ là một tập như vậy, thì hạn chế của $t \mapsto \lambda_t$ lên $K$ là liên tục theo nghĩa mơ hồ, do đó có mệnh đề đầu tiên của mệnh đề. Prop. 2 của §3, No. 1 chỉ ra rằng $\Lambda$ là $\mu$-thích hợp.

Ngược lại, giả sử rằng $\Lambda$ là khả tích $\mu$-một cách cốt yếu theo vô hướng và đo được $\mu$-theo nghĩa mơ hồ; khi đó nó là $\mu$-thích hợp (§3, No. 1, Prop. 2). Vì hàm 1 là nửa liên tục dưới trên $X$, hàm $t \mapsto \lambda_t(1) = g(t)$ là đo được $\mu$ (§3, Def. 1). Do đó tập hợp $S$ là đo được (Ch. IV, §5, No. 5, Prop. 7). Tập hợp $\mathfrak{K}$ gồm các tập hợp compact $K \subset S$ sao cho $g|K$ liên tục và $\Lambda|K$ liên tục theo nghĩa mơ hồ là $\mu$-trù mật trong $S$ (Ch. IV, §5, No. 10, Prop. 15); nếu $K \in \mathfrak{K}$, thì hạn chế lên $K$ của ánh xạ $t \mapsto \varepsilon_{\pi(t)} = \frac{1}{g(t)} \lambda_t$ do đó là liên tục theo nghĩa mơ hồ, và điều này kéo theo tính liên tục của $\pi|K$ (Ch. III, §1, No. 9, Prop. 13). Vì $\mathfrak{K}$ là $\mu$-trù mật trong $S$, hạn chế của $\pi$ lên $S$ là đo được $\mu$.

Ta sẽ sử dụng bổ đề sau:

#### Bổ đề {#int-v-s4-n1-lem-1 .statement}

*Cho $T$ và $X$ là hai không gian tôpô, $\pi$ là một ánh xạ liên tục thực sự (GT, I, §10, No. 1, Def. 1) từ $T$ vào $X$. Cho $g$ là một hàm số nửa liên tục dưới xác định trên $T$. Với mọi $x \in X$, gọi $f(x)$ là cận dưới đúng của hàm $g(t)$ trong tập hợp $\overline{\pi}^{-1}(x)$ (cận dưới đúng bằng $+\infty$ nếu $\overline{\pi}^{-1}(x) = \varnothing$; cf. S, III, §1, No. 9). Khi đó $f$ là nửa liên tục dưới trên $X$.*

### 2. Tích phân trên của các hàm dương đối với một tích phân của các độ đo điểm

Ta sẽ thấy rằng, khi $(\pi, g)$ là một cặp thích nghi với $\mu$, ta có thể cải thiện các kết quả thu được bằng cách áp dụng các mệnh đề của $§ 3$ cho họ $t \mapsto \lambda_t = g(t)\varepsilon_{\pi(t)},$ họ này là thích hợp với $\mu$ theo Mệnh đề 1.

#### Định lý 1 {#int-v-s4-thm-1 .statement}

*Cho* $(\pi, g)$ *là một cặp thích nghi với $\mu$, và cho*
$$
\nu = \int g(t)\varepsilon_{\pi(t)}\, d\mu(t).
$$
*Với mọi hàm số thực* $f \geq 0$ *xác định trên X,* (1)
$$
\int^\bullet f(x)\, d\nu(x) = \int^\bullet f(\pi(t))g(t)\, d\mu(t).
$$

A) Trước hết giả sử độ đo $\mu$ có giá compact K và các hạn chế của các hàm $g$ và $\pi$ trên K đều liên tục. Theo công thức (4) của $§ 3$, No. 1, $\nu^\bullet(1) = \int_K g(t)\, d\mu(t) < +\infty,$ nên mọi độ đo xuất hiện trong công thức (1) đều bị chặn. Vì vậy ta có thể thay $\int^\bullet$ bằng $\int^*$ ở vế thứ nhất. Xét công thức (6) của $§ 3$, No. 2, thì rút cục chỉ còn phải chứng minh rằng (2)
$$
\int^* f(x)\, d\nu(x) \leq \int^\bullet f(\pi(t))g(t)\, d\mu(t),
$$
trong đó ký hiệu $\int^\bullet$ ở vế thứ hai lại có thể thay bằng $\int^*$. Theo định nghĩa tích phân trên, chỉ cần kiểm tra bất đẳng thức (3)
$$
\int^* f(x)\, d\nu(x) \leq \int^* h(t)\, d\mu(t)
$$
với mọi hàm nửa liên tục dưới $h$ trên T sao cho $h \geq$ hàm số $t \mapsto f(\pi(t))g(t)$. Bây giờ, cho $\varepsilon$ là một số $> 0$ và cho $u$ là hàm $(h + \varepsilon)/g,$ hàm này nửa liên tục dưới trên K. Nếu $t \in \pi^{-1}(\{x\}) \cap K,$ thì $u(t) \geq f(x):$ điều này hiển nhiên nếu $g(t) = 0,$ vì khi đó $u(t) = +\infty;$ nếu $g(t) > 0,$ thì
$$
u(t)g(t) = h(t) + \varepsilon \geq f(\pi(t))g(t) = f(x)g(t),
$$

do đó bất đẳng thức đã được khẳng định. Với các điều kiện này, với mọi $x \in X$ hãy đặt $v(x)$ là infimum của $u(t)$ với $t \in \pi^{-1}(\{x\}) \cap K$. Hàm $v$ là $\geq f$ theo điều đã nêu ở trên, nó nửa liên tục dưới trên $X$ theo Bổ đề (áp dụng cho hạn chế của $\pi$ lên $K$), và $v(\pi(t))g(t) \leq h(t) + \varepsilon$ với mọi $t \in K$ (nhắc lại rằng vế thứ nhất bằng không theo quy ước nếu $g(t) = 0$). Khi đó hãy áp dụng cho $v$ công thức (4) của §3, No. 1. Ta thu được:

$$
\int^* f(x)\, d\nu(x) \leq \int^* v(x)\, d\nu(x)
$$
$$
= \int^* v(\pi(t))g(t)\, d\mu(t) \leq \int_K^* (h(t) + \varepsilon)\, d\mu(t)
$$
$$
= \int_K^* h(t)\, d\mu(t) + \varepsilon \mu(1).
$$

Vì độ đo $\mu$ bị chặn và $\varepsilon$ là tùy ý, bất đẳng thức (3) suy ra.

B) Bây giờ ta chuyển sang trường hợp tổng quát. Vì ánh xạ $t \mapsto (\pi(t), g(t))$ từ $T$ vào $X \times \mathbf{R}_+$ là $\mu$-đo được (Ch. IV, §5, No. 3, Đl. 1), tập hợp $\mathcal{K}$ gồm các tập con compact $K$ của $T$ sao cho các hạn chế của $\pi$ và $g$ lên $K$ là liên tục là $\mu$-trù mật (Ch. IV, §5, No. 10, Mđ. 15). Theo Mđ. 4 của §2, No. 3, $\mu$ là tổng của một họ cộng được $(\mu_\alpha)_{\alpha \in A}$ các độ đo mà giá của chúng là các phần tử của $\mathcal{K}$; cặp $(\pi, g)$ là $\mu_\alpha$-thích nghi với mọi $\alpha \in A$, hãy đặt $\nu_\alpha$ là độ đo $\int g(t) \varepsilon_{\pi(t)}\, d\mu_\alpha(t)$. Khi đó theo A),

$$
\int^* f(x)\, d\nu_\alpha(x) = \int^* f(\pi(t))g(t)\, d\mu_\alpha(t).
$$

Nhưng các $\nu_\alpha$ tạo thành một họ cộng được có tổng bằng $\nu$ (§3, No. 1, Hệ quả của Mđ. 1). Do đó, theo Mđ. 1 của §2, No. 2,

$$
\int^* f(x)\, d\nu(x) = \sum_{\alpha \in A} \int^* f(x)\, d\nu_\alpha(x).
$$

Ta có một quan hệ tương tự đối với vế thứ hai của (5), và (1) do đó suy ra từ (5) bằng cách lấy tổng theo $\alpha$.

#### Hệ quả {#int-v-s4-n2-cor-1 .statement}

— *Để một tập con N của X là không đáng kể địa phương đối với $\nu$, điều kiện cần và đủ là giao của $\pi^{-1}(N)$ với tập hợp các điểm $t \in T$ sao cho $g(t) > 0$ là không đáng kể địa phương đối với $\mu$.*

#### Mệnh đề 2 {#int-v-s4-prop-2 .statement}

— *Cho $\pi$ là một ánh xạ liên tục thực sự (GT, I, §10, No. 1) từ T vào X, và cho g là một hàm số liên tục, hữu hạn trên T sao cho $g(t) > 0$ với mọi $t \in T$. Khi đó cặp $(\pi, g)$ là $\mu$-thích nghi, và nếu đặt*
$$
\nu = \int g(t) \varepsilon_{\pi(t)}\, d\mu(t),
$$

thì, với mọi hàm số $f \geq 0$ trên $X$,

$$
\int^* f(x)\, d\nu(x) = \int^* f(\pi(t))g(t)\, d\mu(t).
$$

Hiển nhiên rằng $\pi$ và $g$ là $\mu$-đo được; hơn nữa, đối với mọi hàm $\psi \in \mathcal{K}(X)$, $\psi \circ \pi$ là liên tục với giá đỡ compact, vì $\pi$ là thực sự; do đó cặp $(\pi, g)$ là $\mu$-thích nghi và hơn nữa, ánh xạ $t \mapsto g(t)\varepsilon_{\pi(t)}$ là liên tục theo nghĩa yếu.

Cho $h$ là một hàm nửa liên tục dưới trên $T$ sao cho

$$
f(\pi(t))g(t) \leq h(t) \quad \text{với mọi } t \in T.
$$

Ta sẽ chứng minh rằng

$$
\int^* f(x)\, d\nu(x) \leq \int^* h(t)\, d\mu(t).
$$

Theo định nghĩa của tích phân trên, điều này sẽ kéo theo bất đẳng thức

$$
\int^* f(x)\, d\nu(x) \leq \int^* f(\pi(t))g(t)\, d\mu(t),
$$

mà khi kết hợp với bất đẳng thức (7) của §3, No. 2, sẽ chứng minh (7).

Để chứng minh (8), ta định nghĩa một hàm $\overline{f}$ trên $X$ theo cách sau: $\overline{f}(x)$ là cận dưới lớn nhất của $h(t)/g(t)$ trong tập $\overline{\pi}^{-1}(x)$ (cận dưới lớn nhất bằng $+\infty$ nếu $\overline{\pi}^{-1}(x) = \varnothing$). Hàm $\overline{f}$ có các tính chất sau:

$1^\circ$ $\overline{f}(x) \geq f(x)$ với mọi $x \in X$ (vì $g(t) > 0$ với mọi $t \in T$).

$2^\circ$ $\overline{f}(\pi(t))g(t) \leq h(t)$ với mọi $t \in T$.

$3^\circ$ Hàm $\overline{f}$ là nửa liên tục dưới theo Bổ đề, vì hàm $h/g$ là nửa liên tục dưới trên $T$.

Do đó, theo Mệnh đề 2a) của §3, No. 1:

$$
\int^* f(x)\, d\nu(x) \leq \int^* \overline{f}(x)\, d\nu(x) = \int^* \overline{f}(\pi(t))g(t)\, d\mu(t) \leq \int^* h(t)\, d\mu(t),
$$

điều này thiết lập (8), và hoàn tất chứng minh.

### 3. Tính đo được đối với một tích phân của các độ đo điểm

#### Mệnh đề 3 {#int-v-s4-prop-3 .statement}

— Cho $(\pi, g)$ là một cặp $\mu$-thích nghi, và cho

$$
\nu = \int g(t)\varepsilon_{\pi(t)}\, d\mu(t).
$$

Cho $f$ là một ánh xạ từ $X$ vào một không gian tôpô $G$, và cho $S$ là tập hợp ($\mu$-đo được) các điểm $t \in T$ sao cho $g(t) > 0$. Để $f$ là $\nu$-đo được, điều kiện cần và đủ là hạn chế của $f \circ \pi$ lên $S$ là $\mu$-đo được.

Giả sử trước hết rằng $f$ là $\nu$-khả đo. Theo giả thiết, tập hợp $\mathcal{K}$ của các tập compact $K$ của $S$, sao cho hạn chế của $\pi$ lên $K$ là liên tục, là $\mu$-trù mật trong $S$ (Ch. IV, §5, No. 10, Mệnh đề 15). Để chứng minh rằng hạn chế của $f \circ \pi$ lên $S$ là $\mu$-khả đo, do đó chỉ cần chứng minh rằng với mọi $K \in \mathcal{K}$, tập hợp các tập compact $H$ của $K$, sao cho hạn chế của $f \circ \pi$ lên $H$ là liên tục, là $\mu$-trù mật trong $K$ (Ch. IV, §5, No. 8, Mệnh đề 13). Nhưng theo giả thiết, tồn tại một phân hoạch của tập compact $\pi(K)$ gồm một tập hợp $\nu$-không đáng kể $N$ và một dãy các tập compact $(C_n)$ sao cho hạn chế của $f$ lên từng $C_n$ là liên tục. Trong các điều kiện này, $K \cap \overline{\pi}(N)$ và các tập $K \cap \overline{\pi}(C_n)$ tạo thành một phân hoạch của $K$; nhưng $K \cap \overline{\pi}(N)$ là $\mu$-không đáng kể nhờ Hệ quả của Định lý 1 của No. 2, các tập $K \cap \overline{\pi}(C_n)$ là compact, và hạn chế của $f \circ \pi$ lên từng tập sau là liên tục, điều đó chứng tỏ rằng hạn chế của $f \circ \pi$ lên $S$ là $\mu$-khả đo.

Ngược lại, giả sử điều đó đúng; để chứng minh rằng $f$ là $\nu$-đo được, chỉ cần chứng minh rằng tập $\mathcal{L}$ gồm các tập con compact $L$ của $X$, sao cho hạn chế của $f$ lên $L$ là liên tục, là $\nu$-trù mật (Ch. IV, §5, No. 10, Mệnh đề 15). Cho $N$ là một tập con của $X$ sao cho $N \cap L$ là $\nu$-không đáng kể với mọi $L \in \mathcal{L}$, và ta hãy chứng minh rằng $N$ là địa phương $\nu$-không đáng kể. Để làm điều này, ta phải chứng minh rằng $\overline{\pi}(N) \cap S$ là địa phương $\mu$-không đáng kể (Hệ quả của Định lý 1 của No. 2). Bây giờ, tập $\mathcal{H}$ gồm các tập con compact $H$ của $S$, sao cho các hạn chế lên $H$ của $\pi$ và $f \circ \pi$ là liên tục, theo giả thiết là $\mu$-trù mật trong $S$ (Ch. IV, §5, No. 10, Mệnh đề 15). Do đó chỉ cần chứng minh rằng $\overline{\pi}(N) \cap H$ là $\mu$-không đáng kể với mọi $H \in \mathcal{H}$. Bây giờ, $\pi(H)$ là compact và có thể đồng nhất với không gian thương của $H$ theo quan hệ tương đương $\pi(t) = \pi(t')$, trong đó $\pi$ được đồng nhất với ánh xạ chính tắc của $H$ lên không gian thương này (GT, I, §5, No. 2, Mệnh đề 3). Vì hạn chế của $f \circ \pi$ lên $H$ là liên tục, nên hạn chế của $f$ lên $\pi(H)$ cũng liên tục, nói cách khác $\pi(H) \in \mathcal{L}$, do đó $N \cap \pi(H)$ là $\nu$-không đáng kể. Theo Hệ quả của Định lý 1 của No. 2, $\overline{\pi}(N \cap \pi(H)) \cap S$ là địa phương $\mu$-không đáng kể; vì thế tập

$$
H \cap \overline{\pi}(N) \subset \overline{\pi}(N \cap \pi(H)) \cap S;
$$

cũng là địa phương $\mu$-không đáng kể; nhưng vì $H$ là compact, $H \cap \overline{\pi}(N)$ là $\mu$-không đáng kể, và điều đó hoàn tất chứng minh.

#### Nhận xét {#int-v-s4-n3-rem-1 .statement}

Nếu $f$ là một ánh xạ từ $X$ vào một không gian Banach $F$, thì cũng như nói rằng hạn chế của $f \circ \pi$ lên $S$ là $\mu$-đo được hoặc nói rằng hàm $(f \circ \pi)g$ (được xác định trên $T$) là $\mu$-đo được, vì $g$ là $\mu$-đo được, không triệt tiêu trên $S$, và bằng không trên $T - S$ (Ch. IV, §5, No. 10, Mệnh đề 15).

### 4. Tích phân các hàm nhận giá trị trong một không gian Banach, đối với một tích phân của các độ đo điểm

#### Định lý 2 {#int-v-s4-thm-2 .statement}

*Cho* $(\pi, g)$ *là một cặp $\mu$-thích nghi, và đặt*
$$
\nu = \int g(t) \varepsilon_{\pi(t)} \, d\mu(t).
$$
*Cho* $f$ *là một hàm xác định trên* $X$, *nhận giá trị trong một không gian Banach* $F$ *hoặc trong* $\overline{\mathbf{R}}$. *Để* $f$ *khả tích theo nghĩa rộng đối với* $\nu$, *cần và đủ là* $t \mapsto f(\pi(t))g(t)$ *khả tích theo nghĩa rộng đối với* $\mu$, *trong trường hợp đó*
$$
\int f(x) \, d\nu(x) = \int f(\pi(t))g(t) \, d\mu(t).
$$
*Giả sử thêm rằng* $\pi$ *liên tục và proper, và rằng* $g$ *liên tục và sao cho* $g(t) > 0$ *với mọi* $t \in T$. *Khi đó, để* $f$ *khả tích đối với* $\nu$, *cần và đủ là* t $\mapsto f(\pi(t))g(t)$ *khả tích đối với* $\mu$.

A) Trước hết xét trường hợp độ đo $\mu$ có giá compact $K$, trên đó $g$ bị chặn. Khi đó các độ đo $\mu$ và $\nu$ đều hữu hạn, và có thể thay 'khả tích theo nghĩa rộng' trong mệnh đề bằng 'khả tích'. Giả sử rằng $f$ là $\nu$-khả tích: khi đó hàm $f(\pi(t))g(t)$ là $\mu$-khả tích, và hệ thức (9) được thỏa mãn, theo Định lý 1 của §3, No. 3. Ngược lại, giả sử rằng $f(\pi(t))g(t)$ là $\mu$-khả tích: khi đó $f$ là $\nu$-đo được (No. 3, Mệnh đề 3 và *Nhận xét*), và
$$
\int^\bullet |f(x)| \, d\nu(x) = \int^\bullet |f(\pi(t))|g(t) \, d\mu(t) < +\infty
$$
(No. 2, Định lý 1); do đó $f$ khả tích theo nghĩa rộng đối với $\nu$ (§1, No. 3, Mệnh đề 9), suy ra $f$ khả tích đối với $\nu$. Định lý 1 của §3, No. 3 khi đó suy ra (9).

B) Xét trường hợp tổng quát. Cho $\mathcal{K}$ là tập hợp các tập con compact $K$ của $T$ sao cho $g|K$ liên tục: $\mathcal{K}$ trù mật theo $\mu$ (Ch. IV, §5, No. 10, Mệnh đề 15), do đó độ đo $\mu$ là tổng của một họ $(\mu_\alpha)_{\alpha \in A}$ các độ đo có giá là các phần tử của $\mathcal{K}$ (§2, No. 3, Mệnh đề 4). Cặp $(g, \pi)$ hiển nhiên là $\mu_\alpha$-thích nghi với mọi $\alpha \in A$, và độ đo $\nu$ là tổng của họ các độ đo $\nu_\alpha = \int \varepsilon_{\pi(t)}g(t) \, d\mu_\alpha(t)$ (§3, No. 1, Hệ quả của Mệnh đề 1). Vì lập luận của A) có thể áp dụng cho các độ đo $\mu_\alpha, \nu_\alpha$, nên phần thứ nhất của mệnh đề suy ra từ Mệnh đề 3 của §2, No. 2.

Để hàm $f$ (resp. $t \mapsto f(\pi(t))g(t)$) khả tích đối với $\nu$ (resp. đối với $\mu$), cần và đủ là nó khả tích theo nghĩa rộng và rằng

$$
\int^* |f(x)| d\nu(x) < +\infty \quad (\text{resp. } \int^* |f(\pi(t))|g(t)\,d\mu(t) < +\infty ).
$$

Do đó phần thứ hai của mệnh đề suy ra từ phần thứ nhất và Mệnh đề 2.

#### Nhận xét {#int-v-s4-n4-rem-1 .statement}

— Cho $(\pi, g)$ là một cặp $\mu$-thích nghi, $\pi'$ là một ánh xạ từ T vào X, và $g'$ là một hàm số hữu hạn $\geq 0$ xác định trên T, sao cho $\pi'$ (tương ứng $g'$) bằng $\pi$ (tương ứng $g$) địa phương hầu khắp nơi đối với $\mu$. Khi đó cặp $(\pi', g')$ là $\mu$-thích nghi, các độ đo $\lambda_t = g(t)\varepsilon_{\pi(t)}$ và $\lambda'_t = g'(t)\varepsilon_{\pi'(t)}$ bằng nhau địa phương hầu khắp nơi, và $\int g(t)\varepsilon_{\pi(t)}\,d\mu(t) = \int g'(t)\varepsilon_{\pi'(t)}\,d\mu(t)$. Nếu bây giờ $\pi'$ và $g'$ chỉ được xác định địa phương hầu khắp nơi (theo $\mu$) và nếu tồn tại một cặp $\mu$-thích nghi $(\pi, g)$ sao cho $\pi'$ (tương ứng $g'$) bằng $\pi$ (tương ứng $g$) địa phương hầu khắp nơi, thì lại nói rằng cặp $(\pi', g')$ là $\mu$-thích nghi và ta đặt

$$
\int g'(t)\varepsilon_{\pi'(t)}\,d\mu(t) = \int g(t)\varepsilon_{\pi(t)}\,d\mu(t)
$$

(xem §3, No. 3, *Nhận xét*). Các mệnh đề của ĐL 1 và 2 và của Mệnh đề 3 vẫn đúng khi chỉ giả thiết rằng $\pi$ và $g$ được xác định địa phương hầu khắp nơi.

### Bài tập {#int-v-s4-exercises}

Xem [các bài tập cho § 4](exercises/s4/).
