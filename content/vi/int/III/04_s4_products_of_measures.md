---
book: int
book_title: Integration
chapter: III
chapter_title: MEASURES ON LOCALLY COMPACT SPACES
section: 4
section_title: Products of measures
lang: vi
source: int-i-vi
book_pages: INT III.60-INT III.62
pdf_pages: 0085-0100, 0105-0107
extraction: ocr
subsections:
    - "no": 1
      title: The product of two measures
      page: 40
      pdf_page: 85
    - "no": 2
      title: Properties of product measures
      page: 44
      pdf_page: 89
    - "no": 3
      title: Continuity of product measures
      page: 47
      pdf_page: 92
    - "no": 4
      title: Product of a finite number of measures
      page: 48
      pdf_page: 93
    - "no": 5
      title: Inverse limits of measures
      page: 50
      pdf_page: 95
    - "no": 6
      title: Infinite products of measures
      page: 53
      pdf_page: 98
statements: 22
exercises: 8
content_sha256: 5f00f400b352cc21e3e7c0a1ad529ad752dbfa2526a30a1bbe6c9a60f17bacea
translated_from: content/en/int/III/04_s4_products_of_measures.md
source_content_sha256: 6cce27b93cc8eb2432ea6f68fe801fc213586fdca8c9bffffb15f6d695b84b75
translation_model: gpt-5.4
translation_run: translate-vi-74c3c443
glossary_version: 34
glossary_terms_sha256: bf6930fd70164cce46867e061f2280e36ea9d8cedab5eafd4b442da99f30cffb
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 4. TÍCH CỦA CÁC ĐỘ ĐO

### 1. Tích của hai độ đo

#### Định lý 1 {#int-iii-s4-thm-1 .statement}

— *Cho X và Y là hai không gian địa phương compact, $\lambda$ là một độ đo trên X, $\mu$ là một độ đo trên Y; tồn tại một và chỉ một độ đo $\nu$ trên $X \times Y$ sao cho, với mọi hàm* $g \in \mathcal{K}(X; \mathbf{C})$ *và mọi hàm* $h \in \mathcal{K}(Y; \mathbf{C})$,

$$
\int g(x)h(y)\, d\nu(x, y) = \left( \int g(x)\, d\lambda(x) \right) \left( \int h(y)\, d\mu(y) \right).
$$

#### Bổ đề {#int-iii-s4-n1-lem-1 .statement}

1— *Cho X và Y là hai không gian địa phương compact, K (tương ứng L) là một tập con compact của X (tương ứng của Y).*

(i) *Hạn chế lên* $\mathcal{K}(X \times Y, K \times L; \mathbf{C})$ *của song ánh chính tắc*

$$
\omega : \mathcal{F}(X \times Y; \mathbf{C}) \to \mathcal{F}(X; \mathcal{F}(Y; \mathbf{C}))
$$

(S, R, §4, No. 14) *là một đẳng cự của không gian Banach* $\mathcal{K}(X \times Y, K \times L; \mathbf{C})$ *lên không gian Banach* $\mathcal{K}(X, K; \mathcal{K}(Y, L; \mathbf{C}))$.

(ii) *Không gian vectơ* $\mathcal{K}(X, K; \mathbf{C}) \otimes_{\mathbf{C}} \mathcal{K}(Y, L; \mathbf{C})$, *được đồng nhất một cách chính tắc với một không gian con của* $\mathcal{K}(X \times Y, K \times L; \mathbf{C})$ *(A, II, §7, No. 7, các chú thích sau Hệ quả của Mệnh đề 15), là trù mật trong không gian Banach này*.

Ngay lập tức thấy rằng ảnh qua $\omega$ của $\mathcal{K}(X \times Y, K \times L; \mathbf{C})$ được chứa trong $\mathcal{K}(X, K; \mathcal{K}(Y, L; \mathbf{C}))$. Ngược lại, nếu $u$ là một ánh xạ liên tục từ $X$ vào $\mathcal{K}(Y, L; \mathbf{C})$, có giá đỡ được chứa trong $K$, thì ánh xạ $(x, y) \mapsto u(x)(y)$ từ $X \times Y$ vào $\mathbf{C}$ là liên tục và có giá đỡ được chứa trong $K \times L$, do đó hạn chế của $\omega$ lên $\mathcal{K}(X \times Y, K \times L; \mathbf{C})$ là một song ánh của không gian này lên $\mathcal{K}(X, K; \mathcal{K}(Y, L; \mathbf{C}))$; việc hạn chế này là một đẳng cự của không gian Banach suy ra từ quan hệ

$$
\sup_{(x, y) \in K \times L} |f(x, y)| = \sup_{x \in K} \left( \sup_{y \in L} |f(x, y)| \right).
$$

Điều này chứng minh (i); mặt khác, ảnh qua $\omega$ của

$$
\mathcal{K}(X, K; \mathbf{C}) \otimes_{\mathbf{C}} \mathcal{K}(Y, L; \mathbf{C})
$$

được đồng nhất với một không gian con của $\mathcal{K}(X \times Y, K \times L; \mathbf{C})$, lại chính là không gian $\mathcal{K}(X, K; \mathbf{C}) \otimes_{\mathbf{C}} \mathcal{K}(Y, L; \mathbf{C})$ nhưng lần này được đồng nhất một cách chính tắc với một không gian các ánh xạ từ $X$ vào $\mathcal{K}(Y, L; \mathbf{C})$ (A, II, §7, No. 7, Hệ quả của Mệnh đề 15); nhưng không gian con này của $\mathcal{K}(X, K; \mathcal{K}(Y, L; \mathbf{C}))$ được biết là *trù mật* trong không gian sau (§ 1, No. 2, Prop. 5), vì vậy kết luận của (ii) suy ra từ việc hạn chế của $\omega$ là một đẳng cấu tôpô.

Sau khi đã chứng minh bổ đề, bây giờ ta nhận thấy rằng mọi tập con compact của $X \times Y$ đều được chứa trong một tích $K \times L$, trong đó $K$ (tương ứng $L$) là một tập con compact của $X$ (tương ứng của $Y$). Vì vậy từ Bổ đề 1, (ii) suy ra rằng không gian con $\mathcal{K}(X; \mathbf{C}) \otimes_{\mathbf{C}} \mathcal{K}(Y; \mathbf{C})$ là *trù mật* trong $\mathcal{K}(X \times Y; \mathbf{C})$; vì quan hệ (1) cũng có thể viết là $\nu(g \otimes h) = \lambda(g)\mu(h)$ với $g \in \mathcal{K}(X; \mathbf{C})$, $h \in \mathcal{K}(Y; \mathbf{C})$, nên *tính duy nhất* của $\nu$ suy ra ngay lập tức. Để chứng minh sự tồn tại của $\nu$, ta sẽ dùng bổ đề sau:

#### Bổ đề 2 {#int-iii-s4-lem-2 .statement}

*Với các ký hiệu như trong Bổ đề 1, với mọi hàm* $f \in \mathcal{K}(X \times Y, K \times L; \mathbf{C})$ *hàm*

$$
y \mapsto h(y) = \int f(x, y) \, d\lambda(x)
$$

*thuộc* $\mathcal{K}(Y, L; \mathbf{C})$.

Với mọi hàm $u \in \mathcal{K}(X; \mathcal{K}(Y, L; \mathbf{C}))$, tích phân $\int u(x) d\lambda(x)$ thuộc $\mathcal{K}(Y, L; \mathbf{C})$ vì không gian sau là một không gian Banach (§ 3, No. 3, Cor. 1 of Prop. 7); nhưng với $u = \omega(f)$ và với mọi $y \in Y$,

$$
\left\langle \int u(x) d\lambda(x), \varepsilon_y \right\rangle = \int u(x)(y) d\lambda(x) = \int f(x, y) d\lambda(x),
$$

do đó suy ra bổ đề.

Xét, khi đó, với mọi hàm $f \in \mathcal{K}(X \times Y; \mathbf{C})$, số $\nu(f) = \mu(\int f(x, y) d\lambda(x))$ (mà ta cũng sẽ viết là $\int d\mu(y) \int f(x, y) d\lambda(x)$ do lạm dụng ký hiệu); nếu K (resp. L) là một tập con compact của X (resp. Y), thì tồn tại một số $a_K$ (resp. $b_L$) sao cho, với mọi hàm $g \in \mathcal{K}(X, K; \mathbf{C})$ (resp. $h \in \mathcal{K}(Y, L; \mathbf{C})$), ta có $|\lambda(g)| \leq a_K \|g\|$ (resp. $|\mu(h)| \leq b_L \|h\|$). Suy ra rằng với mọi hàm $f \in \mathcal{K}(X \times Y, K \times L; \mathbf{C})$,

$$
\left| \int f(x, y) d\lambda(x) \right| \leq a_K \|f\|
$$

với mọi $y \in Y$, do đó $|\nu(f)| \leq a_K b_L \|f\|$. Dạng tuyến tính $\nu$ trên $\mathcal{K}(X \times Y; \mathbf{C})$ vì thế là một độ đo trên $X \times Y$ hiển nhiên thỏa mãn (1), điều này hoàn tất chứng minh của Định lý 1.

#### Định nghĩa 1 {#int-iii-s4-def-1 .statement}

*Cho hai độ đo $\lambda, \mu$ được định nghĩa, tương ứng, trên hai không gian compact địa phương $X, Y$, tích độ đo của $\lambda$ với $\mu$ được định nghĩa là độ đo duy nhất $\nu$ trên $X \times Y$ thỏa mãn quan hệ (1) với mọi hàm $g \in \mathcal{K}(X; \mathbf{C})$ và mọi hàm $h \in \mathcal{K}(Y; \mathbf{C})$.*

Trong chứng minh của Định lý 1, vai trò của các không gian X và Y có thể hoán đổi cho nhau; đồng nhất một cách chính tắc $Y \times X$ với $X \times Y$, do đó ta định nghĩa trên $X \times Y$ một độ đo

$$
f \mapsto \int d\lambda(x) \int f(x, y) d\mu(y)
$$

mà lại thỏa mãn điều kiện (1). Như vậy ta đã chứng minh định lý sau đây:

#### Định lý 2 {#int-iii-s4-thm-2 .statement}

*Cho $\lambda, \mu$ là hai độ đo được định nghĩa, tương ứng, trên hai không gian compact địa phương $X, Y$. Với mọi hàm $f$ trong $\mathcal{K}(X \times Y; \mathbf{C})$, tích phân của $f$ đối với tích độ đo $\nu$ của $\lambda$ với $\mu$ có giá trị*

$$
\int f(x, y) d\nu(x, y) = \int d\lambda(x) \int f(x, y) d\mu(y)
$$
$$(3)$$
$$
= \int d\mu(y) \int f(x, y) d\lambda(x).
$$

Do công thức cuối cùng, tích phân của $f$ đối với tích độ đo $\nu$ thường được ký hiệu là $\iint f\, d\lambda\, d\mu$, hoặc $\iint f\, d\mu\, d\lambda$, hoặc $\iint f\, \lambda\mu$, hoặc $\iint f\, \mu\lambda$, hoặc $\iint f(x, y)\, d\lambda(x)\, d\mu(y)$, hoặc $\iint f(x, y)\, d\mu(y)\, d\lambda(x)$, hoặc $\iint f(x, y)\, \lambda(x)\mu(y)$, hoặc $\iint f(x, y)\, \mu(y)\lambda(x)$; nó được gọi là tích phân kép của $f$ đối với $\lambda$ và $\mu$. Với ký hiệu này, công thức (3) có thể được viết

$$
\iint f(x, y)\, d\lambda(x)\, d\mu(y) = \int d\lambda(x) \int f(x, y)\, d\mu(y)
$$
$$
= \int d\mu(y) \int f(x, y)\, d\lambda(x).
$$

Công thức (3) cho thấy rằng nếu $\lambda$ và $\mu$ là các độ đo thực (resp. dương), thì tích độ đo $\nu$ là thực (resp. dương).

#### Ví dụ 1 {#int-iii-s4-n1-exa-1 .statement}

Độ đo tích của các độ đo Dirac $\varepsilon_x$ ($x \in X$) và $\varepsilon_y$ ($y \in Y$) là độ đo Dirac $\varepsilon_{(x, y)}$.

#### Ví dụ 2 {#int-iii-s4-n1-exa-2 .statement}

Lấy $X = Y = \mathbf{R}$, và $\lambda$ và $\mu$ là *độ đo Lebesgue* trên $\mathbf{R}$ (§1, No. 3); tích của chúng được gọi là *độ đo Lebesgue* trên $\mathbf{R}^2$; tích phân của một hàm $f \in \mathcal{K}(\mathbf{R}^2; \mathbf{C})$ đối với độ đo này được ký hiệu là $\iint f(x, y)\, dx\, dy$ hoặc $\iint f(x, y)\, dy\, dx$; công thức (4), đối với một hàm bằng không ở ngoài một hình chữ nhật compắc $[a, b] \times [c, d]$, cho công thức

$$
\int_c^d dy \int_a^b f(x, y)\, dx = \int_a^b dx \int_c^d f(x, y)\, dy
$$

được chứng minh trong FRV, II, §3, No. 6.

Vì độ đo Lebesgue trên $\mathbf{R}$ là bất biến dưới mọi phép tịnh tiến (§1, No. 3), do đó suy ra ngay rằng độ đo Lebesgue trên $\mathbf{R}^2$ là *bất biến dưới mọi phép tịnh tiến của $\mathbf{R}^2$*.

#### Nhận xét {#int-iii-s4-n1-rem-1 .statement}

Cho $E$ là một không gian lồi địa phương Hausdorff, và cho $f$ là một ánh xạ thuộc $\mathcal{K}(X \times Y; E)$ sao cho $f(X \times Y)$ được chứa trong một tập con *lồi đầy đủ* $C$ của $E$. Khi đó, với mọi $y \in Y$, tích phân $h(y) = \int f(x, y)\, d\lambda(x)$ thuộc $E$ (§3, No. 3, Prop. 7); hơn nữa, hàm $h$ thuộc $\widetilde{\mathcal{K}}(Y; E)$: thật vậy, với mọi $z' \in E'$ ta có

$$
\langle h(y), z' \rangle = \int \langle f(x, y), z' \rangle\, d\lambda(x),
$$

vì thế $y \mapsto \langle h(y), z' \rangle$ thuộc $\mathcal{K}(Y; C)$ theo Bổ đề 2. Do đó tích phân $\int h\, d\mu$ được xác định (và *tiên nghiệm* thuộc ${E'}^*$); hãy chỉ ra rằng

$$
\iint f(x, y)\, d\lambda(x)\, d\mu(y) = \int d\mu(y) \int f(x, y)\, d\lambda(x)
$$
$$
= \int d\lambda(x) \int f(x, y)\, d\mu(y),
$$

như vậy tổng quát hóa công thức (4). Thật vậy, với mọi $z' \in E'$ ta có
$$
\left\langle \int \int f d\lambda d\mu, z' \right\rangle = \int \int \langle f, z' \rangle d\lambda d\mu = \int d\mu \int \langle f, z' \rangle d\lambda \\
= \int \left\langle \int f d\lambda, z' \right\rangle d\mu = \left\langle \int d\mu \int f d\lambda, z' \right\rangle
$$
theo (4), do đó có (5).

### 2. Tính chất của các độ đo tích

Nếu $\lambda$ (resp. $\mu$) là một độ đo trên X (resp. Y) và $\nu$ là độ đo tích của $\lambda$ với $\mu$, thì hạn chế của $\nu$ lên $\mathcal{K}(X; \mathbf{C}) \otimes_{\mathbf{C}} \mathcal{K}(Y; \mathbf{C})$ không gì khác hơn là *tích tenxơ* $\lambda \otimes \mu$ của hai dạng tuyến tính $\lambda$ và $\mu$ (A, II, §3, No. 2), bởi vì quan hệ (1) của No. 1 có thể được viết
$$
\langle g \otimes h, \nu \rangle = \langle g, \lambda \rangle \langle h, \mu \rangle = \langle g \otimes h, \lambda \otimes \mu \rangle
$$
với mọi $g \in \mathcal{K}(X; \mathbf{C})$ và $h \in \mathcal{K}(Y; \mathbf{C})$. Do lạm dụng ký hiệu, chúng tôi cũng sẽ ký hiệu bởi $\lambda \otimes \mu$ độ đo tích $\nu$ (chứ không chỉ hạn chế của nó lên không gian con trù mật $\mathcal{K}(X; \mathbf{C}) \otimes_{\mathbf{C}} \mathcal{K}(Y; \mathbf{C})$ của $\mathcal{K}(X \times Y; \mathbf{C})$).

Ánh xạ $(\lambda, \mu) \mapsto \lambda \otimes \mu$ từ $\mathcal{M}(X; \mathbf{C}) \times \mathcal{M}(Y; \mathbf{C})$ vào $\mathcal{M}(X \times Y; \mathbf{C})$ hiển nhiên là *song tuyến tính*, theo công thức (3) của No. 1.

#### Mệnh đề 1 {#int-iii-s4-prop-1 .statement}

*Cho $\lambda$ là một độ đo trên X, $\mu$ là một độ đo trên Y; nếu $g \in \mathcal{C}(X; \mathbf{C}),\ h \in \mathcal{C}(Y; \mathbf{C}),$ thì*
$$
(g \cdot \lambda) \otimes (h \cdot \mu) = (g \otimes h) \cdot (\lambda \otimes \mu).
$$

Với mọi hàm $f \in \mathcal{K}(X \times Y; \mathbf{C})$, theo công thức (3) của No. 1, ta có
$$
\langle f, (g \otimes h) \cdot (\lambda \otimes \mu) \rangle = \int d\lambda(x) \int f(x, y) g(x) h(y) d\mu(y) \\
= \int g(x) d\lambda(x) \int f(x, y) h(y) d\mu(y),
$$
điều này chứng minh công thức (6).

#### Mệnh đề 2 {#int-iii-s4-prop-2 .statement}

*Giá của tích $\lambda \otimes \mu$ bằng tích của giá của $\lambda$ và giá của $\mu$.*

Trước hết ta nhận thấy rằng quan hệ $\lambda \otimes \mu = 0$ kéo theo một trong hai độ đo $\lambda, \mu$ là không (A, II, §7, No. 7, Prop. 16, (ii)). Mặt khác, nếu U (tương ứng V) là một tập mở trong X (tương ứng trong Y), thì hạn chế của $\lambda \otimes \mu$ lên tích $U \times V$ là tích của các hạn chế của $\lambda$ lên U và của $\mu$ lên V, như suy ra từ Th. 1 của No. 1 và định nghĩa của hạn chế của một độ đo lên một tập mở (§ 2, No. 1). Do đó suy ra rằng để hạn chế của $\lambda \otimes \mu$ lên $U \times V$ là không thì điều kiện cần và đủ là hoặc hạn chế của $\lambda$ lên U hoặc hạn chế của $\mu$ lên V là không; điều này chứng minh mệnh đề, có tính đến định nghĩa của giá của một độ đo (§ 2, No. 2).

#### Mệnh đề 3 {#int-iii-s4-prop-3 .statement}

*Cho $\lambda \in \mathcal{M}(X; \mathbf{C}),\ \mu \in \mathcal{M}(Y; \mathbf{C})$. Khi đó*

$$
|\lambda \otimes \mu| = |\lambda| \otimes |\mu|.
$$

Cho $f \in \mathcal{K}_+(X \times Y),\ g \in \mathcal{K}(X \times Y; \mathbf{C})$ sao cho $|g| \leq f$; ta có (§ 1, No. 6, công thức (13))

$$
\begin{align*}
|\langle g, \lambda \otimes \mu \rangle| &= \left| \int d\lambda(x) \int g(x, y) d\mu(y) \right| \\
&\leq \int d|\lambda|(x) \int |g(x, y)|\ d|\mu|(y) \\
&= \langle |g|, |\lambda| \otimes |\mu| \rangle \leq \langle f, |\lambda| \otimes |\mu| \rangle.
\end{align*}
$$

Suy ra $\langle f, |\lambda \otimes \mu| \rangle \leq \langle f, |\lambda| \otimes |\mu| \rangle$, và do đó

$$
|\lambda \otimes \mu| \leq |\lambda| \otimes |\mu|.
$$

Mặt khác, cho $u \in \mathcal{K}_+(X),\ v \in \mathcal{K}_+(Y)$. Với mọi $\varepsilon > 0$, tồn tại $u_1 \in \mathcal{K}(X; \mathbf{C}),\ v_1 \in \mathcal{K}(Y; \mathbf{C})$ sao cho $|u_1| \leq u,\ |v_1| \leq v$ và

$$
|\langle u_1, \lambda \rangle| \geq \langle u, |\lambda| \rangle - \varepsilon,\quad |\langle v_1, \mu \rangle| \geq \langle v, |\mu| \rangle - \varepsilon
$$
(§ 1, No. 6). Suy ra $|u_1 \otimes v_1| \leq u \otimes v$ và

$$
\begin{align*}
\langle u \otimes v, |\lambda \otimes \mu| \rangle &\geq |\langle u_1 \otimes v_1, \lambda \otimes \mu \rangle| = |\langle u_1, \lambda \rangle \langle v_1, \mu \rangle| \\
&\geq ((\langle u, |\lambda| \rangle - \varepsilon)(\langle v, |\mu| \rangle - \varepsilon)).
\end{align*}
$$

Vì $\varepsilon$ là tùy ý, ta suy ra rằng

$$
\langle u \otimes v, |\lambda \otimes \mu| \rangle \geq \langle u, |\lambda| \rangle \langle v, |\mu| \rangle = \langle u \otimes v, |\lambda| \otimes |\mu| \rangle.
$$

Có tính đến (8), ta thấy rằng

$$
\langle u \otimes v, |\lambda \otimes \mu| \rangle = \langle u \otimes v, |\lambda| \otimes |\mu| \rangle.
$$

Vì mọi hàm trong $\mathcal{K}(X; \mathbf{C})$ (tương ứng $\mathcal{K}(Y; \mathbf{C})$) đều là một tổ hợp tuyến tính của các hàm trong $\mathcal{K}_+(X)$ (tương ứng $\mathcal{K}_+(Y)$), công thức trước vẫn đúng cho $u \in \mathcal{K}(X; \mathbf{C})$ và $v \in \mathcal{K}(Y; \mathbf{C})$; do đó mệnh đề suy ra từ việc $\mathcal{K}(X; \mathbf{C}) \otimes_{\mathbf{C}} \mathcal{K}(Y; \mathbf{C})$ trù mật trong $\mathcal{K}(X \times Y; \mathbf{C})$.

#### Hệ quả {#int-iii-s4-n2-cor-1 .statement}

— *Cho* $\lambda \in \mathcal{M}(X; \mathbf{R}), \ \mu \in \mathcal{M}(Y; \mathbf{R})$. *Khi đó*

$$
\begin{cases}
(\lambda \otimes \mu)^+ = \lambda^+ \otimes \mu^+ + \lambda^- \otimes \mu^- , \\
(\lambda \otimes \mu)^- = \lambda^+ \otimes \mu^- + \lambda^- \otimes \mu^+ .
\end{cases}
$$

Thật vậy, theo Prop. 3,

$$
\begin{align*}
(\lambda \otimes \mu)^+ &= \frac{1}{2} (\lambda \otimes \mu + |\lambda| \otimes |\mu|) \\
&= \frac{1}{2} ((\lambda^+ - \lambda^-) \otimes (\mu^+ - \mu^-) + (\lambda^+ + \lambda^-) \otimes (\mu^+ + \mu^-)) \\
&= \lambda^+ \otimes \mu^+ + \lambda^- \otimes \mu^- .
\end{align*}
$$

Lập luận đối với $(\lambda \otimes \mu)^-$ là tương tự.

#### Mệnh đề 4 {#int-iii-s4-prop-4 .statement}

— *Cho* $\lambda \in \mathcal{M}(X; \mathbf{C}), \ \mu \in \mathcal{M}(Y; \mathbf{C})$. *Khi đó*

$$
\|\lambda \otimes \mu\| = \|\lambda\| \cdot \|\mu\|,
$$

*với quy ước rằng vế thứ hai được thay bằng 0 mỗi khi một trong các thừa số là 0 và thừa số kia là $+\infty$*. *Đặc biệt, nếu* $\lambda$ *và* $\mu$ *bị chặn thì* $\lambda \otimes \mu$ *bị chặn*.

Theo Mệnh đề 3 ở trên, và §1, No. 8, Hệ quả 1 của Mệnh đề 10, ta có thể chỉ xét trường hợp $\lambda$ và $\mu$ là các độ đo dương. Nếu $\lambda = 0$ hoặc $\mu = 0$ thì kết quả là tầm thường; do đó giả sử $\lambda \neq 0$ và $\mu \neq 0$. Trước hết hãy chứng minh rằng $\|\lambda \otimes \mu\| \leq \|\lambda\| \cdot \|\mu\|$. Ta có thể giả sử $\lambda$ và $\mu$ bị chặn. Với mọi $f \in \mathcal{K}_+(X \times Y)$,

$$
\langle f, \lambda \otimes \mu \rangle = \int d\lambda(x) \int f(x, y) d\mu(y)
$$

và

$$
\int f(x, y) d\mu(y) \leq \|f\| \cdot \|\mu\|
$$

với mọi $x \in X$, vậy nên

$$
\langle f, \lambda \otimes \mu \rangle \leq \|f\| \cdot \|\lambda\| \cdot \|\mu\|,
$$

điều này chứng minh mệnh đề của ta. Mặt khác, cho

$$
\alpha < \| \lambda \| , \quad \beta < \| \mu \|
$$

là hai số thực $\geqslant 0$. Tồn tại $g \in \mathcal{K}_+(X) , \ h \in \mathcal{K}_+(Y)$ sao cho

$$
\| g \| \leqslant 1 , \ \| h \| \leqslant 1 , \quad \lambda(g) \geqslant \alpha , \ \mu(h) \geqslant \beta .
$$

Khi đó $g \otimes h \in \mathcal{K}_+(X \times Y) , \ \| g \otimes h \| \leqslant 1$ và $\langle g \otimes h , \lambda \otimes \mu \rangle \geqslant \alpha \beta ;$ do đó $\| \lambda \otimes \mu \| \geqslant \alpha \beta$ và cuối cùng $\| \lambda \otimes \mu \| \geqslant \| \lambda \| \cdot \| \mu \|$, điều này hoàn tất chứng minh.

### 3. Tính liên tục của các độ đo tích

#### Mệnh đề 5 {#int-iii-s4-prop-5 .statement}

*Với mọi độ đo* $\lambda_0 \in \mathcal{M}(X; \mathbf{C})$, *ánh xạ* $\mu \mapsto \lambda_0 \otimes \mu$ *từ* $\mathcal{M}(Y; \mathbf{C})$ *vào* $\mathcal{M}(X \times Y; \mathbf{C})$ *là liên tục mơ hồ*.

Với mọi hàm $f \in \mathcal{K}(X \times Y; \mathbf{C})$, ta biết rằng hàm $h(y) = \int f(x, y) d\lambda_0(x)$ thuộc $\mathcal{K}(Y; \mathbf{C})$ (No. 1, Bổ đề 2), và $\langle f , \lambda_0 \otimes \mu \rangle = \langle h , \mu \rangle$, do đó suy ra mệnh đề.

#### Mệnh đề 6 {#int-iii-s4-prop-6 .statement}

*Nếu* $\mathcal{M}(X; \mathbf{C}) , \ \mathcal{M}(Y; \mathbf{C})$ *và* $\mathcal{M}(X \times Y; \mathbf{C})$ *được trang bị tôpô hội tụ chặt trên compáct* (§ 1, No. 10), *thì ánh xạ song tuyến tính* $(\lambda, \mu) \mapsto \lambda \otimes \mu$ *từ* $\mathcal{M}(X; \mathbf{C}) \times \mathcal{M}(Y; \mathbf{C})$ *vào* $\mathcal{M}(X \times Y; \mathbf{C})$ *là hypocontinuous đối với tập hợp các tập con bị chặn mơ hồ của* $\mathcal{M}(X; \mathbf{C})$ *và* $\mathcal{M}(Y; \mathbf{C})$ *(TVS, III, § 5, No. 3)*.

Cho $K \subset X , \ L \subset Y$ là hai tập compact, $A$ là một tập con compact của $\mathcal{K}(X \times Y, K \times L; \mathbf{C})$, và $B$ là một tập con bị chặn mơ hồ và đóng của $\mathcal{M}(X; \mathbf{C})$; ta biết rằng $B$ là compact mơ hồ (§ 1, No. 9, Mệnh đề 15), nên cũng compact đối với tôpô hội tụ compact chặt (§ 1, No. 10, Mệnh đề 17). Mặt khác, không gian Banach $\mathcal{K}(X \times Y, K \times L; \mathbf{C})$ đẳng cự với $\mathcal{K}(X, K; \mathcal{K}(Y, L; \mathbf{C}))$ (No. 1, Bổ đề 1); ánh xạ $\varphi$ từ $\mathcal{K}(X, K; \mathcal{K}(Y, L; \mathbf{C})) \times \mathcal{M}(X; \mathbf{C})$ vào $\mathcal{K}(Y, L; \mathbf{C})$, sao cho $\varphi(g, \lambda)$ là hàm $h$ xác định bởi $h(y) = \int g(x, y) d\lambda(x)$, là *liên tục riêng* theo § 3, No. 4, Mệnh đề 8 và 9. Vì $\mathcal{K}(X, K; \mathcal{K}(Y, L; \mathbf{C}))$ là thùng, suy ra ánh xạ $\varphi$ là *hypoliên tục* đối với các tập con bị chặn mơ hồ của $\mathcal{M}(X; \mathbf{C})$ (TVS, III, § 5, No. 3, Mệnh đề 6); do đó hạn chế của ánh xạ này lên $A \times B$ là *liên tục* (*loc. cit.*, Mệnh đề 4). Ảnh $C$ của $A \times B$ qua ánh xạ này do đó là một tập con compact của không gian Banach $\mathcal{K}(Y, L; \mathbf{C})$. Bây giờ, $C$ không là gì khác ngoài tập các hàm $h(y) = \int f(x, y) d\lambda(x)$ khi $f$ chạy qua $A$ và $\lambda$ chạy qua $B$; theo công thức (3) của No. 1, các điều kiện $\lambda \in B$ và $\mu \in C^\circ$ do đó kéo theo $\lambda \otimes \mu \in A^\circ$. Xét định nghĩa của tôpô hội tụ compact chặt, điều này chứng minh mệnh đề (TVS, III, § 5, No. 3, Định nghĩa 2).

Kết luận của Mệnh đề 6 không còn đúng nữa khi tôpô hội tụ compact chặt được thay bằng tôpô mơ hồ (Bài tập 2 c)). Tuy nhiên, nếu B (tương ứng C) là một tập con bị chặn mơ hồ của $\mathcal{M}(X; \mathbf{C})$ (tương ứng $\mathcal{M}(Y; \mathbf{C})$), thì ảnh của $B \times C$ qua ánh xạ $(\lambda, \mu) \mapsto \lambda \otimes \mu$ là bị chặn mơ hồ trong $\mathcal{M}(X \times Y; \mathbf{C})$ và do đó hạn chế của ánh xạ này lên $B \times C$ là liên tục mơ hồ, theo Mệnh đề 6, §1, No. 10, Mệnh đề 17, và Mệnh đề 4 của TVS, III, §5, No. 3 (x. Bài tập 3).

### 4. Tích của một số hữu hạn các độ đo

Cho $X_i$ ($1 \leq i \leq n$) là $n$ không gian compact địa phương, $X = \prod_{i=1}^n X_i$ là tích của chúng. Tập các tổ hợp tuyến tính của các hàm phức có dạng
$$
(x_1, x_2, \ldots, x_n) \mapsto f_1(x_1)f_2(x_2)\cdots f_n(x_n),
$$
trong đó $f_i \in \mathcal{K}(X_i; \mathbf{C})$ ($1 \leq i \leq n$), có thể được đồng nhất một cách chính tắc với tích tenxơ $\bigotimes_{i=1}^n \mathcal{K}(X_i; \mathbf{C})$, và suy ra từ Bổ đề 1 của No. 1, bằng quy nạp theo $n$, rằng tích tenxơ này *trù mật* trong $\mathcal{K}(X; \mathbf{C})$.

Bây giờ cho $\mu_i$ là một độ đo trên $X_i$ ($1 \leq i \leq n$); tồn tại trên $X$ một và chỉ một độ đo $\nu$ sao cho, với $f_i \in \mathcal{K}(X_i; \mathbf{C})$ ($1 \leq i \leq n$),
$$
\langle f_1 \otimes f_2 \otimes \cdots \otimes f_n, \nu \rangle = \prod_{i=1}^n \langle f_i, \mu_i \rangle.
$$
Thật vậy, nếu độ đo này tồn tại thì theo điều đã nói trên, nó là duy nhất. Mặt khác, cho $\nu = \mu_1 \otimes \mu_2 \otimes \cdots \otimes \mu_n$ là độ đo trên $X$ được xác định bởi quan hệ quy nạp
$$
\mu_1 \otimes \mu_2 \otimes \cdots \otimes \mu_n = (\mu_1 \otimes \mu_2 \otimes \cdots \otimes \mu_{n-1}) \otimes \mu_n.
$$
Suy ra từ No. 1, công thức (1) và định nghĩa này (bằng quy nạp theo $n$) rằng $\nu$ thỏa mãn (11); người ta gọi nó là *độ đo tích* của các độ đo $\mu_i$ ($1 \leq i \leq n$) và lại ký hiệu nó bởi $\bigotimes_{i=1}^n \mu_i$. Quan hệ (11) cũng có thể viết thành
$$
\langle f_1 \otimes f_2 \otimes \cdots \otimes f_n, \mu_1 \otimes \mu_2 \otimes \cdots \otimes \mu_n \rangle = \prod_{i=1}^n \langle f_i, \mu_i \rangle.
$$

#### Mệnh đề 7 ('tính kết hợp của tích các độ đo') {#int-iii-s4-prop-7 .statement}

—
*Cho* $(I_k)_{1 \leq k \leq r}$ *là một phân hoạch của khoảng* $[1, n]$ *của* $\mathbf{N}$; *khi đó*
$$
\bigotimes_{k=1}^r \left( \bigotimes_{i \in I_k} \mu_i \right) = \bigotimes_{i=1}^n \mu_i
$$

Thật vậy, hai độ đo này trùng nhau, theo (12), trên mọi hàm thuộc $\bigotimes_{i=1}^n \mathcal{K}(X_i; \mathbf{C})$.

Tích phân của một hàm $f \in \mathcal{K}(X; \mathbf{C})$ đối với độ đo tích được ký hiệu là
$$
\int f d\mu_1 d\mu_2 \ldots d\mu_n,
$$
hoặc
$$
\iiint \ldots \int f d\mu_1 d\mu_2 \ldots d\mu_n
$$
hoặc
$$
\int f(\mu_1 \otimes \cdots \otimes \mu_n)
$$
hoặc cũng
$$
\iiint \ldots \int f(x_1, x_2, \ldots, x_n) d\mu_1(x_1) d\mu_2(x_2) \ldots d\mu_n(x_n)
$$
hoặc
$$
\iiint \ldots \int f(x_1, x_2, \ldots, x_n) \mu_1(x_1) \mu_2(x_2) \ldots \mu_n(x_n)
$$
với $n$ dấu $\int$; người ta gọi đó là một *tích phân bội cấp* $n$, hoặc một *tích phân $n$ lần*. Do tính kết hợp của tích các độ đo và định lý về việc đảo thứ tự lấy tích phân (No. 1, Định lý 2), ta có, với mọi phép hoán vị $\sigma$ của $[1, n]$,
$$
\iiint \ldots \int f d\mu_1 d\mu_2 \ldots d\mu_n = \int d\mu_{\sigma(1)} \int d\mu_{\sigma(2)} \ldots \int fd\mu_{\sigma(n)}.
$$
(14)

Ký hiệu tích phân và công thức (14) có thể được mở rộng một cách hiển nhiên cho các hàm $f \in \mathcal{K}(X; E)$ nhận giá trị trong một không gian lồi địa phương Hausdorff $E$, sao cho $f(X)$ được chứa trong một tập con lồi đầy đủ của $E$. Chúng tôi để bạn đọc tự tổng quát hóa cho tích của một số hữu hạn bất kỳ các độ đo các kết quả của Nos. 2 và 3 liên quan đến tích của hai độ đo.

Đặc biệt, người ta gọi *độ đo Lebesgue* trên $\mathbf{R}^n$ là tích của $n$ độ đo đồng nhất với độ đo Lebesgue trên $\mathbf{R}$; tích phân của một hàm $f \in \mathcal{K}(\mathbf{R}^n; E)$, thỏa mãn điều kiện trước đó, được ký hiệu là
$$
\iiint \ldots \int f(x_1, x_2, \ldots, x_n) dx_1 dx_2 \ldots dx_n
$$
và bằng
$$
\int_{-\infty}^{+\infty} dx_1 \int_{-\infty}^{+\infty} dx_2 \ldots \int_{-\infty}^{+\infty} f(x_1, x_2, \ldots, x_n) dx_n.
$$
Độ đo Lebesgue trên $\mathbf{R}^n$ là *bất biến dưới mọi phép tịnh tiến*.

### 5. Giới hạn nghịch của các độ đo

Cho $X, Y$ là hai không gian compact, $p : X \to Y$ là một ánh xạ liên tục; khi đó $f \mapsto f \circ p$ là một ánh xạ tuyến tính liên tục từ $\mathcal{C}(Y; \mathbf{C})$ vào $\mathcal{C}(X; \mathbf{C})$, vì $\|f \circ p\| \leq \|f\|$ với mọi hàm $f \in \mathcal{C}(Y; \mathbf{C})$; ta ký hiệu ánh xạ này bởi $p'$. Do đó chuyển vị của nó ${}^t p' : \mathcal{M}(X; \mathbf{C}) \to \mathcal{M}(Y; \mathbf{C})$ là sao cho, với mọi độ đo $\mu$ trên $X$, ${}^t p'(\mu)$ là độ đo trên $Y$ sao cho

$$
\langle {}^t p'(\mu), f \rangle = \langle \mu, f \circ p \rangle
$$

với mọi hàm $f \in \mathcal{C}(Y; \mathbf{C})$. Chú ý rằng với mọi $x \in X$, ${}^t p'(\varepsilon_x) = \varepsilon_{p(x)}$; vì lý do đó, chúng ta sẽ ký hiệu bởi $p_*(\mu)$ độ đo ${}^t p'(\mu)$, do đó mở rộng $p$ khi $X$ (ứng. $Y$) được nhúng một cách chính tắc vào $\mathcal{M}(X; \mathbf{C})$ (ứng. $\mathcal{M}(Y; \mathbf{C})$) (§ 1, No. 9, Mệnh đề 13); với mọi độ đo $\mu$ trên $X$, $p_*(\mu)$ là một trường hợp riêng của khái niệm tổng quát về *ảnh của một độ đo*, mà chúng ta sẽ nghiên cứu ở Ch. V, §6. Vì, như đã thấy ở trên, $\|p'\| \leq 1$, ta cũng có $\|{}^t p'\| \leq 1$ và do đó

$$
\|p_*(\mu)\| \leq \|\mu\|
$$

với mọi độ đo $\mu \in \mathcal{M}(X; \mathbf{C})$.

Bây giờ ta xét một tập tiền thứ tự có hướng $I$, và một *hệ ngược* (hay 'hệ xạ ảnh') $(X_\alpha, p_{\alpha\beta})$ gồm các không gian *compact* $X_\alpha$ (GT, I, §4, No. 4) nhận $I$ làm tập chỉ số; không gian *giới hạn ngược* $X = \lim_{\leftarrow} X_\alpha$ được biết là compact (GT, I, §9, No. 6, Mệnh đề 8); ta sẽ ký hiệu bởi $p_\alpha$ ánh xạ chính tắc từ $X$ vào $X_\alpha$.

Hiển nhiên $(\mathcal{M}(X_\alpha; \mathbf{C}), (p_{\alpha\beta})_* )$ là một *hệ ngược* các không gian vectơ, và $((p_\alpha)_*)$ là một *hệ ngược* các ánh xạ tuyến tính, điều này biện minh cho định nghĩa sau:

#### Định nghĩa 2 {#int-iii-s4-def-2 .statement}

*Một họ* $(\mu_\alpha)_{\alpha \in I}$, *trong đó, với mọi* $\alpha \in I$, $\mu_\alpha$ *là một độ đo trên* $X_\alpha$, *được gọi là một hệ ngược các độ đo nếu, mỗi khi* $\alpha \leq \beta$, $\mu_\alpha = (p_{\alpha\beta})_*(\mu_\beta)$. *Một độ đo* $\mu$ *trên* $X = \lim_{\leftarrow} X_\alpha$ *được gọi là một giới hạn ngược của hệ ngược* $(\mu_\alpha)$ *nếu* $\mu_\alpha = (p_\alpha)_*(\mu)$ *với mọi* $\alpha \in I$.

#### Mệnh đề 8 {#int-iii-s4-prop-8 .statement}

(i) *Nếu một hệ ngược* $(\mu_\alpha)$ *các độ đo trên các* $X_\alpha$ *có một giới hạn ngược, thì giới hạn đó là duy nhất.*
(ii) *Nếu một hệ ngược* $(\mu_\alpha)$ *có một giới hạn ngược, thì họ các chuẩn* $(\|\mu_\alpha\|)$ *bị chặn.*
(iii) *Nếu các* $p_{\alpha\beta}$ *là toàn ánh và họ* $(\|\mu_\alpha\|)$ *bị chặn, thì hệ ngược các độ đo* $(\mu_\alpha)$ *có một giới hạn ngược.*

(iv) *Nếu các $p_{\alpha \beta}$ là toàn ánh, thì mọi hệ ngược $(\mu_\alpha)$ của các độ đo dương đều có một giới hạn ngược $\mu$, là một độ đo dương trên $X$, và $\| \mu \| = \| \mu_\alpha \|$ với mọi $\alpha$.

(i) Trước hết ta chứng minh bổ đề sau:

#### Bổ đề 3 {#int-iii-s4-lem-3 .statement}

— *Cho F là tập các hàm $f \in \mathcal{C}(X; \mathbf{C})$ có tính chất sau: tồn tại một $\alpha \in I$ và một hàm $f_\alpha \in \mathcal{C}(X_\alpha; \mathbf{C})$ sao cho $f = f_\alpha \circ p_\alpha$. Khi đó F là một không gian con tuyến tính trù mật của $\mathcal{C}(X; \mathbf{C})$.*

Trước hết ta chú ý rằng nếu $g = g_\beta \circ p_\beta$ và $h = h_\gamma \circ p_\gamma$, trong đó $g_\beta \in \mathcal{C}(X_\beta; \mathbf{C})$ và $h_\gamma \in \mathcal{C}(X_\gamma; \mathbf{C})$, thì tồn tại một $\alpha \in I$ sao cho $\alpha \geq \beta$ và $\alpha \geq \gamma$, và do đó $p_\beta = p_{\beta \alpha} \circ p_\alpha$, $p_\gamma = p_{\gamma \alpha} \circ p_\alpha$, điều này cho thấy rằng
$$
g + h = (g_\beta \circ p_{\beta \alpha} + h_\gamma \circ p_{\gamma \alpha}) \circ p_\alpha
$$
thuộc F; tương tự, ta cũng thấy rằng $gh \in F$; do đó F là một đại số con *C* của $\mathcal{C}(X; \mathbf{C})$, chứa các hằng số và có tính chất là quan hệ $f \in F$ kéo theo $\overline{f} \in F$. Cuối cùng, nếu $x \neq y$ là hai điểm của X, thì tồn tại một $\alpha \in I$ sao cho $p_\alpha(x) \neq p_\alpha(y)$, do đó có một hàm $f_\alpha \in \mathcal{C}(X_\alpha; \mathbf{C})$ sao cho $f_\alpha(p_\alpha(x)) \neq f_\alpha(p_\alpha(y))$. Vậy kết luận suy ra từ định lý Stone–Weierstrass (GT, X, §4, No. 4, Prop. 7).

Bổ đề đã được thiết lập, cho $\mu, \mu'$ là hai độ đo trên X sao cho $(p_\alpha)_*(\mu) = (p_\alpha)_*(\mu')$ với mọi $\alpha \in I$; điều này có nghĩa là, với mọi $\alpha \in I$ và mọi hàm $f_\alpha \in \mathcal{C}(X_\alpha; \mathbf{C})$, ta có
$$
\langle f_\alpha, (p_\alpha)_*(\mu) \rangle = \langle f_\alpha, (p_\alpha)_*(\mu') \rangle,
$$
nghĩa là, $\langle f_\alpha \circ p_\alpha, \mu \rangle = \langle f_\alpha \circ p_\alpha, \mu' \rangle$; nói cách khác, $\mu$ và $\mu'$ trùng nhau trên không gian con F của $\mathcal{C}(X; \mathbf{C})$, không gian này là trù mật theo Bổ đề 3, do đó $\mu = \mu'$, điều này chứng minh (i).

(ii) Quan hệ (15) áp dụng cho $p_\alpha$ cho thấy rằng nếu $\mu$ là giới hạn ngược của hệ ngược $(\mu_\alpha)$, thì tất yếu
$$
\| \mu \| \geq \| \mu_\alpha \|
$$
với mọi $\alpha \in I$.

(iii) Giả sử các $p_{\alpha \beta}$ là toàn ánh; khi đó người ta biết rằng các $p_\alpha$ cũng có tính chất ấy (GT, I, §9, No. 6, Prop. 8). Xét một hệ ngược các độ đo $(\mu_\alpha)$ và trước hết ta sẽ chứng minh rằng tồn tại một dạng tuyến tính $\lambda$ *trên* F (theo các ký hiệu của Bổ đề 3) sao cho, với mọi $\alpha \in I$ và mọi $f_\alpha \in \mathcal{C}(X_\alpha; \mathbf{C})$, $\lambda(f_\alpha \circ p_\alpha) = \mu_\alpha(f_\alpha)$. Muốn vậy, cho $\beta, \gamma$ là hai chỉ số trong I, và $f_\beta \in \mathcal{C}(X_\beta; \mathbf{C})$, $f_\gamma \in \mathcal{C}(X_\gamma; \mathbf{C})$ là hai hàm sao cho $f_\beta \circ p_\beta = f_\gamma \circ p_\gamma$; khi đó tồn tại một chỉ số $\alpha \in I$ sao cho $\alpha \geq \beta$ và $\alpha \geq \gamma$, do đó
$$
p_\beta = p_{\beta \alpha} \circ p_\alpha ,\ p_\gamma = p_{\gamma \alpha} \circ p_\alpha \quad \text{and} \quad (f_\beta \circ p_{\beta \alpha}) \circ p_\alpha = (f_\gamma \circ p_{\gamma \alpha}) \circ p_\alpha ;
$$

vì $p_\alpha$ là toàn ánh, điều này kéo theo $f_\beta \circ p_{\beta \alpha} = f_\gamma \circ p_{\gamma \alpha}$, do đó

$$
\mu_\alpha(f_\beta \circ p_{\beta \alpha}) = \mu_\alpha(f_\gamma \circ p_{\gamma \alpha});
$$

nhưng theo định nghĩa quan hệ cuối cùng cũng có thể viết là $\mu_\beta(f_\beta) = \mu_\gamma(f_\gamma)$, do đó có mệnh đề của ta.

Điều này đã có, giả sử rằng tồn tại một số hữu hạn $a > 0$ sao cho $\| \mu_\alpha \| \leq a$ với mọi $\alpha \in I$; khi đó, với mọi hàm $f_\alpha \in \mathcal{C}(X_\alpha; \mathbf{C})$,

$$
|\lambda(f_\alpha \circ p_\alpha)| = |\mu_\alpha(f_\alpha)| \leq a \| f_\alpha \| = a \| f_\alpha \circ p_\alpha \|
$$

vì $p_\alpha$ là toàn ánh. Điều này cho thấy dạng tuyến tính $\lambda$ là liên tục trên $F$, và từ Bổ đề 3 suy ra rằng $\lambda$ có thể được mở rộng thành một độ đo $\mu$ trên $X$ sao cho $(p_\alpha)_*(\mu) = \mu_\alpha$ với mọi $\alpha \in I$, điều đó chứng minh (iii).

(iv) Để chứng minh sự tồn tại của $\mu$ thì theo (iii), chỉ cần kiểm tra rằng họ các chuẩn $(\| \mu_\alpha \|)$ bị chặn. Nhưng $\| \mu_\alpha \| = \mu_\alpha(1)$ và, khi $\alpha \leq \beta$, quan hệ $\mu_\alpha = (p_{\alpha \beta})_*(\mu_\beta)$ kéo theo $\mu_\alpha(1) = \mu_\beta(1)$; vì $I$ có hướng, nên các khối lượng toàn phần của mọi độ đo $\mu_\alpha$ do đó đều bằng nhau, do đó có mệnh đề của chúng ta. Hơn nữa, không gian con $F$ hiển nhiên thỏa mãn tính chất (P) của §1, No. 7, Mệnh đề 9, vì vậy độ đo giới hạn ngược $\mu$ của $(\mu_\alpha)$ là dương. Cuối cùng, quan hệ $\mu_\alpha = (p_\alpha)_*(\mu)$ cho thấy như trên rằng $\mu(1) = \mu_\alpha(1)$.

#### Ví dụ {#int-iii-s4-n5-exa-1 .statement}

— Cho $(X_\lambda)_{\lambda \in L}$ là một họ các không gian compact; đặt $X = \prod_{\lambda \in L} X_\lambda$ và, với mọi tập con hữu hạn $J$ của $L$, đặt $X_J = \prod_{\lambda \in J} X_\lambda$; ký hiệu bởi $\mathrm{pr}_J : X \to X_J$ và $\mathrm{pr}_{J, K} : X_K \to X_J$ (với $J \subset K$) các phép chiếu chính tắc. Ta biết rằng $(X_J, \mathrm{pr}_{JK})$ là một hệ ngược các không gian compact, và rằng giới hạn ngược của hệ các ánh xạ liên tục $(\mathrm{pr}_J)$ là một *đồng cấu* từ $X$ lên không gian giới hạn ngược $\lim_{\leftarrow} X_J$, cho phép đồng nhất hai không gian này (GT, I, §4, No. 4 và S, III, §7, No. 2, *Nhận xét* 3). Vì các phép chiếu $\mathrm{pr}_{J, K}$ là toàn ánh, từ Mệnh đề 8 suy ra rằng tập hợp $\mathcal{M}(X; \mathbf{C})$ (ứng với $\mathcal{M}_+(X)$) có thể được đồng nhất với tập hợp các hệ ngược $(\mu_J)$ sao cho họ các chuẩn $(\| \mu_J \|)$ bị chặn (ứng với sao cho các $\mu_J$ đều dương, và tất yếu có cùng khối lượng toàn phần).

Hãy xét riêng trường hợp mà, với mỗi $\lambda \in L$, một độ đo $\mu_\lambda$ được cho trên $X_\lambda$ và đặt $\mu_J = \bigotimes_{\lambda \in J} \mu_\lambda$. Nếu $J \subset K$ là hai tập con hữu hạn của $I$ thì, với mọi hàm $f_J \in \mathcal{C}(X_J; \mathbf{C})$ ta có, theo công thức (14) của No. 4,

$$
\mu_K(f_J \circ \mathrm{pr}_{J, K}) = \mu_J(f_J) \cdot \prod_{\lambda \in K - J} \mu_\lambda(1).
$$

Để $(\mu_J)$ là một hệ ngược các độ đo, do đó điều kiện cần và đủ là hoặc $\mu_\lambda = 0$ với mọi $\lambda \in L$ hoặc $\mu_\lambda(1) = 1$ với mọi $\lambda \in L$.

### 6. Tích vô hạn của các độ đo

Cho $(X_\lambda)_{\lambda \in L}$ là một họ các không gian compact, và với mỗi $\lambda \in L$ cho một độ đo $\mu_\lambda$ trên $X_\lambda$. Ta giữ lại các ký hiệu của Ví dụ ở No. 5, để đặc biệt có $\mu_J = \bigotimes_{\lambda \in J} \mu_\lambda$ với mọi tập con hữu hạn $J$ của $L$.

#### Mệnh đề 9 {#int-iii-s4-prop-9 .statement}

*Giả sử rằng tất cả các độ đo $\mu_\lambda$ đều dương và rằng họ $(\mu_\lambda(1))_{\lambda \in L}$ là khả nhân trong $\mathbf{R}_+$ (với tích có thể bằng 0). Khi đó tồn tại một và chỉ một độ đo $\mu$ trên $X$ sao cho, với mọi tập con hữu hạn $J$ của $L$ và mọi hàm $f_J \in \mathcal{C}(X_J; \mathbf{C})$,*

$$
\mu(f_J \circ \mathrm{pr}_J) = \mu_J(f_J) \prod_{\lambda \in L - J} \mu_\lambda(1).
$$

Hơn nữa, độ đo $\mu$ là dương và khối lượng toàn phần của nó được cho bởi

$$
\mu(1) = \prod_{\lambda \in L} \mu_\lambda(1).
$$

Gọi $F$ là không gian vectơ gồm các hàm trên $X$ có dạng $f_J \circ \mathrm{pr}_J$, trong đó $J$ chạy qua tập có hướng các tập con hữu hạn của $L$, và $f_J \in \mathcal{C}(X_J; \mathbf{C})$; ta lại nói rằng $F$ là không gian các hàm liên tục trên $X$ *chỉ phụ thuộc vào một số hữu hạn biến*. Bổ đề 3 của No. 5 cho thấy rằng $F$ trù mật trong $\mathcal{C}(X; \mathbf{C})$, điều đó chứng minh mệnh đề về tính duy nhất. Nếu $\mu_{\lambda_0} = 0$ với một $\lambda_0 \in L$ nào đó thì độ đo $\mu = 0$ thỏa mãn các điều kiện yêu cầu, vì trong vế thứ hai của (18) ta có $\mu_J(f_J) = 0$ nếu $\lambda_0 \in J$ và $\prod_{\lambda \in L - J} \mu_\lambda(1) = 0$ nếu $\lambda_0 \notin J$. Do đó ta có thể giả sử rằng $\mu_\lambda \neq 0$ với mọi $\lambda \in J$ và, vì các độ đo $\mu_\lambda$ là dương, điều này kéo theo $\mu_\lambda(1) \neq 0$ với mọi $\lambda \in L$. Khi đó đặt $\mu'_\lambda = \mu_\lambda / \mu_\lambda(1)$ với mọi $\lambda \in L$, để $\mu'_\lambda$ là một độ đo dương trên $X_\lambda$ sao cho $\mu'_\lambda(1) = 1$. Khi đó theo Mệnh đề 8 của No. 5 suy ra tồn tại một độ đo dương $\mu'$ trên $X$ có khối lượng toàn phần bằng 1, sao cho $\mu'(f_J \circ \mathrm{pr}_J) = \mu'_J(f_J)$ với mọi tập con hữu hạn $J$ của $L$ và mọi hàm $f_J \in \mathcal{C}(X_J; \mathbf{C})$. Độ đo dương

$$
\mu = \left( \prod_{\lambda \in L} \mu_\lambda(1) \right) \mu'
$$

khi đó thỏa mãn các điều kiện yêu cầu, vì

$$
\mu_J(f_J) = \mu'_J(f_J) \cdot \prod_{\lambda \in J} \mu_\lambda(1),
$$
$$
\prod_{\lambda \in L} \mu_\lambda(1) = \prod_{\lambda \in J} \mu_\lambda(1) \cdot \prod_{\lambda \in L - J} \mu_\lambda(1).
$$

Độ đo $\mu$ được xác định trong Mệnh đề 9 được gọi là *độ đo tích* của họ các độ đo dương $(\mu_\lambda)_{\lambda \in L}$ và được ký hiệu là $\bigotimes_{\lambda \in L} \mu_\lambda$.

#### Hệ quả {#int-iii-s4-n6-cor-1 .statement}

*Giả sử rằng các điều kiện của Mệnh đề 9 được thỏa mãn, và gọi $(L_\rho)_{\rho \in R}$ là một phân hoạch của $L$. Khi đó mỗi họ độ đo $(\mu_\lambda)_{\lambda \in L_\rho}$ đều thừa nhận một độ đo tích, họ các độ đo tích $\left( \bigotimes_{\lambda \in L_\rho} \mu_\lambda \right)_{\rho \in R}$ thừa nhận một độ đo tích, và*

$$
\bigotimes_{\rho \in R} \left( \bigotimes_{\lambda \in L_\rho} \mu_\lambda \right) = \bigotimes_{\lambda \in L} \mu_\lambda.
$$

Điều này suy ra ngay từ các công thức (18) và (19) và tính kết hợp của tích đối với các họ khả nhân trong $\mathbf{R}_+$ (GT, IV, §7, No. 5, *Nhận xét*).

Bài tập

### Bài tập {#int-iii-s4-exercises}

Xem [bài tập cho § 4](exercises/s4/).
