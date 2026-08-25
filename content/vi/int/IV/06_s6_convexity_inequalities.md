---
book: int
book_title: Integration
chapter: IV
chapter_title: EXTENSION OF A MEASURE. LP SPACES
section: 6
section_title: Convexity inequalities
lang: vi
source: int-i-vi
book_pages: INT IV.89-INT IV.100, INT IV.134-INT IV.142
pdf_pages: 0196-0207, 0241-0249
extraction: ocr
subsections:
    - "no": 1
      title: The convexity theorem
      page: 89
      pdf_page: 196
    - "no": 2
      title: Inequality of the mean
      page: 90
      pdf_page: 197
    - "no": 3
      title: The spaces $L^\infty_F$
      page: 91
      pdf_page: 198
    - "no": 4
      title: Hölder’s inequality
      page: 93
      pdf_page: 200
    - "no": 5
      title: 'Application: relations between the spaces $L^p_F$ ($1 \leq p \leq +\infty$)'
      page: 98
      pdf_page: 205
statements: 22
exercises: 20
content_sha256: bf23ed8277c91c875d13c0de1a1b2822dcc981f46d28f9ac4b6d4ba94e4d820f
translated_from: content/en/int/IV/06_s6_convexity_inequalities.md
source_content_sha256: 1943305609b50f182ebf680418cbb9b81a0c09ae593113d7d4c5e7b050ac7f2f
translation_model: gpt-5-6-mini, gpt-5-6
translation_run: translate-vi-d38441a8
glossary_version: 34
glossary_terms_sha256: a5e37bf3e7a24e69df3cc9d7fe343f2487bc52aade6a3724a77303a8d5c00392
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 6. CÁC BẤT ĐẲNG THỨC LỒI

### 1. Định lý lồi

#### Định lý 1 {#int-iv-s6-thm-1 .statement}

— Cho $X$ là một không gian compact địa phương, $\mu$ là một độ đo dương trên $X$, $F$ là một không gian Banach thực, $D$ là một tập lồi đóng trong $F$, và $f$ là một hàm trên $X$ sao cho $f(X) \subset D$. Với mọi hàm số số học khả tích không đáng kể $g \geqslant 0$ sao cho $fg$ khả tích, điểm $\frac{\int fg\, d\mu}{\int g\, d\mu}$ thuộc $D$.

Thật vậy, đặt $F'$ là đối ngẫu của $F$ và xét quan hệ $\langle z, a' \rangle \leqslant \alpha$ ($a' \in F', \alpha \in \mathbf{R}$) xác định một nửa không gian đóng chứa $D$. Vì $fg$ khả tích, nên hàm số số học $\langle fg, a' \rangle = \langle f, a' \rangle g$ cũng khả tích, và

$$
\int \langle fg, a' \rangle\, d\mu = \left\langle \int fg\, d\mu, a' \right\rangle
$$

(\S 4, No. 2, Hệ quả 1 của Định lý 1); nhưng, theo giả thiết, $\langle f(x), a' \rangle \leqslant \alpha$ với mọi $x \in X$, do đó $\langle f(x)g(x), a' \rangle \leqslant \alpha g(x)$; khi lấy tích phân, ta có

$$
\left\langle \int fg\, d\mu, a' \right\rangle \leqslant \alpha \int g\, d\mu .
$$

Điều này chứng minh rằng điểm $\frac{\int fg\, d\mu}{\int g\, d\mu}$ thuộc mọi nửa không gian đóng chứa $D$; nhưng, theo định lý Hahn–Banach, $D$ là giao của các nửa không gian đóng chứa nó (TVS, II, §5, No. 3, Hệ quả 1 của Mệnh đề 4), do đó suy ra định lý.

#### Hệ quả {#int-iv-s6-n1-cor-1 .statement}

— *Nếu độ đo dương $\mu$ có khối lượng toàn phần bằng 1 và nếu $f$ khả tích, thì $\int f\, d\mu$ thuộc bao lồi đóng của $f(X)$ trong $F$*.

Chỉ cần lấy cho $g$ hàm hằng 1.

### 2. Bất đẳng thức của trung bình

Ta sẽ làm sắc bén hơn Định lý 1 đối với các hàm số số học đo được (hữu hạn hoặc không).

#### Định nghĩa 1 {#int-iv-s6-def-1 .statement}

— Cho X là một không gian compact địa phương, $\mu$ là một độ đo trên X. Cho một hàm số số học f (hữu hạn hoặc không), được xác định địa phương hầu khắp nơi trong X, ta gọi là cực đại theo độ đo, hay cực đại $\mu$ (tương ứng là cực tiểu theo độ đo, hay cực tiểu $\mu$) của hàm f, và ký hiệu là $M_\infty(f)$ (tương ứng là $m_\infty(f)$), cận dưới đúng (tương ứng là cận trên đúng) của tập hợp các số $\alpha$ sao cho $f(x) \leq \alpha$ (tương ứng là $f(x) \geq \alpha$) địa phương hầu khắp nơi (đối với $\mu$).

Từ định nghĩa suy ra ngay rằng $m_\infty(f) = -M_\infty(-f)$, do đó từ mọi tính chất của cực đại theo độ đo ta suy ra một tính chất tương ứng của cực tiểu theo độ đo.

Với mọi $\alpha > M_\infty(f)$, tập hợp các $x \in X$ sao cho $f(x) > \alpha$ là không đáng kể địa phương; khi đó, tập hợp các $x \in X$ sao cho $f(x) > M_\infty(f)$ là hợp của các tập hợp mà trên đó $f(x) > r_n$, với $r_n$ chạy qua tập hợp các số hữu tỉ $> M_\infty(f)$; do đó $f(x) \leq M_\infty(f)$ địa phương hầu khắp nơi (\S 5, No. 2). Tương tự $f(x) \geq m_\infty(f)$ địa phương hầu khắp nơi; suy ra $m_\infty(f) \leq M_\infty(f)$ nếu độ đo $\mu$ khác không; hơn nữa, quan hệ $m_\infty(f) = M_\infty(f)$ tương đương với việc nói rằng $f$ bằng một hằng địa phương hầu khắp nơi. Rõ ràng rằng nếu độ đo $\mu$ khác không, thì

$$
\inf_{x \in X} f(x) \leq m_\infty(f) \leq M_\infty(f) \leq \sup_{x \in X} f(x).
$$

Nếu hai hàm $f, g$ bằng nhau địa phương hầu khắp nơi, thì $m_\infty(f) = m_\infty(g)$ và $M_\infty(f) = M_\infty(g)$.

Cuối cùng, nếu $f$ và $g$ là hai hàm sao cho $f + g$ được xác định địa phương hầu khắp nơi, thì

(1)
$$
M_\infty(f + g) \leq M_\infty(f) + M_\infty(g)
$$
với điều kiện vế thứ hai được xác định, như suy ra ngay lập tức từ Định nghĩa 1; tương tự, nếu $f$ và $g$ đều $\geq 0$ và sao cho $fg$ được xác định địa phương hầu khắp nơi, thì

(2)
$$
M_\infty(fg) \leq M_\infty(f) M_\infty(g)
$$
với điều kiện vế thứ hai được xác định.

Nếu $M_\infty(f) < +\infty$, thì $f(x) < +\infty$ địa phương hầu khắp nơi, nhưng không nhất thiết hầu khắp nơi. Một hàm số thực $f$ được gọi là bị chặn theo độ đo (đối với độ đo $\mu$) nếu nó được xác định và hữu hạn hầu khắp nơi, và hơn nữa, các số $m_\infty(f)$ và $M_\infty(f)$ đều hữu hạn (điều kiện sau tương đương với việc nói rằng $M_\infty(|f|) < +\infty$).

#### Mệnh đề 1 (Bất đẳng thức của giá trị trung bình) {#int-iv-s6-prop-1 .statement}

— *Cho f là một hàm số thực đo được bị chặn theo độ đo. Với mọi hàm số thực khả tích $g \geqslant 0$, hàm $fg$ (được xác định hầu khắp nơi) là khả tích và*

$$
m_\infty(f) \int g d|\mu| \leqslant \int fg d|\mu| \leqslant M_\infty(f) \int g d|\mu|.
$$

Hơn nữa, *hai trong ba thành phần của bất đẳng thức (3) không thể bằng nhau trừ khi, trong tập hợp các $x \in X$ sao cho $g(x) \neq 0$, f bằng $M_\infty(f)$ hầu khắp nơi hoặc bằng $m_\infty(f)$ hầu khắp nơi*.

Thật vậy, $fg$ là đo được (\S 5, No. 3, Hệ quả 5 của Định lý 1); hơn nữa, bất đẳng thức $m_\infty(f)g(x) \leqslant f(x)g(x) \leqslant M_\infty(f)g(x)$ đúng, không chỉ địa phương hầu khắp nơi, mà thậm chí hầu khắp nơi, bởi vì tập hợp các điểm $x \in X$ nơi $g(x) \neq 0$ là một hợp đếm được của các tập hợp khả tích (\S 5, No. 6, Bổ đề 1). Suy ra rằng $fg$ là khả tích (\S 5, No. 6, Định lý 5) và bất đẳng thức (3) đúng. Mặt khác, hàm $M_\infty(f)g - fg$ được xác định hầu khắp nơi và bằng $(M_\infty(f) - f)g$; do đó nó $\geqslant 0$ hầu khắp nơi trong $X$; vì quan hệ $M_\infty(f) \int g d|\mu| = \int fg d|\mu|$ tương đương với $\int (M_\infty(f) - f)g d|\mu| = 0$, nó chỉ có thể đúng nếu hàm $(M_\infty(f) - f)g$ là không đáng kể, điều này hoàn tất chứng minh.

Bỏ qua trường hợp tầm thường $\int g d|\mu| = 0$, bất đẳng thức (3) có thể được suy ra từ Định lý 1 của No. 1 áp dụng cho khoảng $D = [m_\infty(f), M_\infty(f)]$. Người ta có thể đưa vào Định lý 1 của No. 1 các phần bù tương tự như những phần bù của Mệnh đề 1, xác định trường hợp trong đó điểm $(\int fg d\mu)/(\int g d\mu)$ thuộc biên của D (Bài tập 2).

### 3. Các không gian $L^\infty_F$

#### Định nghĩa 2 {#int-iv-s6-def-2 .statement}

*Với mọi ánh xạ $f$ của $X$ vào một không gian Banach $F$, đặt $N_\infty(f) = M_\infty(|f|)$; $f$ được gọi là bị chặn theo độ đo (đối với độ đo $\mu$) nếu $N_\infty(f)$ là hữu hạn. Tập hợp các ánh xạ của $X$ vào $F$ đo được và bị chặn theo độ đo được ký hiệu là $\mathcal{L}_F^\infty(X, \mu)$ (hoặc $\mathcal{L}_F^\infty(\mu)$, hoặc đơn giản là $\mathcal{L}_F^\infty$).*

Một hàm $f$ trong $\mathcal{L}_F^\infty$ do đó có thể được đặc trưng bởi việc tồn tại một hàm *bị chặn đo được* bằng $f$ địa phương hầu khắp nơi.

Suy ra ngay lập tức từ (1) rằng

$$
N_\infty(f + g) \leqslant N_\infty(f) + N_\infty(g);
$$

mặt khác, $N_\infty(\alpha f) = |\alpha| N_\infty(f)$ với mọi vô hướng $\alpha$. Tập hợp $\mathcal{L}_F^\infty$ do đó là một *không gian con tuyến tính* của không gian tất cả các ánh xạ từ $X$ vào $F$, và $N_\infty(f)$ là một nửa chuẩn trên không gian vectơ này. Cho $(f_n)$ là một dãy các hàm thuộc $\mathcal{L}_F^\infty$ hội tụ đến $f \in \mathcal{L}_F^\infty$ theo tôpô xác định bởi nửa chuẩn $N_\infty(f)$; với mọi số nguyên $m$, tồn tại một tập hợp không đáng kể địa phương $H_m$ và một số nguyên $n_0$ sao cho $|f(x) - f_n(x)| \leq 1/m$ với mọi số nguyên $n \geq n_0$ và mọi $x \notin H_m$ (mọi hợp đếm được của các tập hợp không đáng kể địa phương đều không đáng kể địa phương); hợp $H$ của các $H_m$ là không đáng kể địa phương, và ta thấy rằng $f_n(x)$ hội tụ *đều* đến $f(x)$ trên phần bù của tập hợp không đáng kể địa phương $H$; đảo lại là ngay lập tức.

Rõ ràng rằng mọi hàm bằng địa phương hầu khắp nơi với một hàm thuộc $\mathcal{L}_F^\infty$ đều thuộc $\mathcal{L}_F^\infty$. Đặc biệt, các hàm *không đáng kể địa phương* xác định trên $X$ với giá trị trong $F$ tạo thành một không gian con tuyến tính $\mathcal{N}_F^\infty$ của $\mathcal{L}_F^\infty$, được đặc trưng bởi quan hệ $N_\infty(f) = 0$ (bao đóng của 0 đối với tôpô xác định bởi $N_\infty(f)$). Không gian Hausdorff liên kết với $\mathcal{L}_F^\infty$, nghĩa là không gian thương $\mathcal{L}_F^\infty / \mathcal{N}_F^\infty$, được ký hiệu là $L_F^\infty(X, \mu)$ (hoặc $L_F^\infty(\mu)$ hoặc $L_F^\infty$); tôpô của nó được xác định bởi chuẩn suy ra từ $N_\infty$ bằng phép chuyển qua thương; chuẩn của một lớp $\dot{f} \in L_F^\infty$ được ký hiệu là $N_\infty(\dot{f})$, hoặc cũng là $\| \dot{f} \|_\infty$. Khi $F = \mathbf{R}$ (tương ứng $\mathbf{C}$), ta viết $\mathcal{L}^\infty$ và $L^\infty$ thay cho $\mathcal{L}_\mathbf{R}^\infty$ và $L_\mathbf{R}^\infty$ (tương ứng $\mathcal{L}_\mathbf{C}^\infty$ và $L_\mathbf{C}^\infty$) nếu điều này không gây nhầm lẫn.

#### Mệnh đề 2 {#int-iv-s6-prop-2 .statement}

*Không gian* $\mathcal{L}_F^\infty$ *là đầy đủ; không gian* $L_F^\infty$ *là một không gian Banach*.

Vì, xét $(f_n)$ là một dãy Cauchy trong $\mathcal{L}_F^\infty$; với mỗi số nguyên $n$, tồn tại một số nguyên $k_n$ sao cho $N_\infty(f_r - f_s) \leq 1/n$ với $r \geq k_n$ và $s \geq k_n$; do đó, tồn tại một tập hợp không đáng kể địa phương $A_{rs}$ sao cho $|f_r(x) - f_s(x)| \leq 1/n$ với mọi $x \notin A_{rs}$. Nếu $A_n$ là hợp của các tập hợp $A_{rs}$ (với $r \geq k_n$ và $s \geq k_n$), thì $A_n$ là không đáng kể địa phương và, với mọi $x \notin A_n$, $|f_r(x) - f_s(x)| \leq 1/n$ với mọi chỉ số $r \geq k_n, s \geq k_n$. Gọi $A$ là tập hợp không đáng kể địa phương được tạo thành bởi hợp của các $A_n$, và đặt $g_n(x) = f_n(x)$ với $x \notin A$, $g_n(x) = 0$ với $x \in A$; khi đó $g_n$ thuộc $\mathcal{L}_F^\infty$ và, theo định nghĩa của $A$, dãy $(g_n)$ hội tụ *đều* trên $X$ tới một hàm $g$. Suy ra rằng hàm $g$ là đo được (\S 5, No. 4, Th. 2); hơn nữa, $g$ bị chặn trên tập hợp các $x \in X$ mà $|g_{k_1}(x)| \leq N_\infty(g_{k_1})$ và, vì phần bù của tập hợp này là không đáng kể địa phương, $g$ thuộc $\mathcal{L}_F^\infty$. Hiển nhiên rằng trong $\mathcal{L}_F^\infty$, dãy $(g_n)$ có giới hạn $g$, và do đó điều tương tự cũng đúng với dãy $(f_n)$, vì $N_\infty(f_n - g_n) = 0$ với mọi $n$. Phần thứ hai của mệnh đề được suy ra ngay lập tức từ điều này.

#### Nhận xét {#int-iv-s6-n3-rem-1 .statement}

— 1) Mọi hàm *liên tục bị chặn* $f$ trên $X$ với các giá trị trong $F$ đều thuộc $\mathcal{L}_F^\infty$, và

$$
N_\infty(f) \leq \| f \| = \sup_{x \in X} |f(x)| .
$$

Để $N_\infty(f) = \|f\|$ đối với mọi hàm liên tục bị chặn $f$, điều kiện cần và đủ là giá của độ đo $\mu$ bằng $X$. Thật vậy, nếu tồn tại một hàm liên tục $f$ có giá compact không đáng kể và không đồng nhất bằng không, thì $N_\infty(f) = 0$ và $\|f\| > 0$. Ngược lại, nếu giá của $\mu$ bằng $X$ thì, đối với mọi hàm liên tục bị chặn $f$ và mọi số $\alpha < \|f\|$, tập hợp các $x \in X$ sao cho $|f(x)| > \alpha$ là mở và khác rỗng, do đó có độ đo ngoài $> 0$, điều này chứng tỏ rằng $N_\infty(f) = \|f\|$.

Khi giá của $\mu$ bằng $X$, do đó ta có thể đồng nhất không gian định chuẩn $C^b(X; F)$, gồm các hàm liên tục bị chặn trên $X$ với giá trị trong $F$, với một không gian con của không gian $L_F^\infty$. Vì $L_F^\infty$ nói chung không Hausdorff, không gian con $C^b(X; F)$ nói chung không đóng trong $L_F^\infty$, nhưng ảnh chính tắc của nó trong $L_F^\infty$ là một không gian con đóng của $L_F^\infty$ (hơn nữa có thể đồng nhất với $C^b(X; F)$ trong trường hợp đang xét). Nói chung, $C^b(X; F)$ khác với $L_F^\infty$, nghĩa là, đối với một hàm đo được bị chặn tùy ý $f$, nói chung không tồn tại một hàm liên tục $g$ bằng $f$ địa phương hầu khắp nơi (\S 5, Bài tập 12). Điều này suy ra rằng không gian $\mathcal{H}(X; F)$ gồm các ánh xạ từ $X$ vào $F$, liên tục với giá compact, nói chung không trù mật trong $L_F^\infty$, trong khi nó trù mật trong mỗi không gian $L_F^p$ với $1 \leq p < +\infty$ (\S 3, No. 4. Định nghĩa 2).

2) Hiển nhiên rằng tôpô xác định bởi bán chuẩn $N_\infty$ mịn hơn tôpô cảm sinh trên $L_F^\infty$ bởi tôpô của sự hội tụ theo độ đo (\S 5, No. 11).

### 4. Bất đẳng thức Hölder

Trong No. này, $p$ và $q$ sẽ ký hiệu hai số thực sao cho $1 \leq p \leq +\infty$, $1 \leq q \leq +\infty$, liên hệ bởi quan hệ $1/p + 1/q = 1$; do đó $q = p/(p-1)$ nếu $1 < p < +\infty$, $q = +\infty$ nếu $p = 1$, và $q = 1$ nếu $p = +\infty$; $p$ và $q$ sẽ được gọi là các số mũ liên hợp. Chú ý rằng quan hệ $1 \leq p \leq 2$ tương đương với $2 \leq q \leq +\infty$; $p = q$ chỉ khi $p$ và $q$ đều bằng 2.

#### Định lý 2 (Bất đẳng thức Hölder) {#int-iv-s6-thm-2 .statement}

— Cho $f$ và $g$ là hai hàm số có giá trị số hữu hạn hầu khắp nơi và sao cho $f$ bằng hầu khắp nơi một hàm thuộc $L^p$ và $g$ bằng hầu khắp nơi một hàm thuộc $L^q$. Khi đó, hàm $fg$ (được xác định hầu khắp nơi) là khả tích, và

$$
N_1(fg) \leq N_p(f) N_q(g).
$$

Gọi $f_1$ (tương ứng $g_1$) là một hàm trong $L^p$ (tương ứng $L^q$) mà $f$ (tương ứng $g$) bằng hầu khắp nơi; $fg$ bằng hầu khắp nơi hàm $f_1 g_1$, hàm này được xác định khắp nơi và hữu hạn, và đo được, vì là tích của hai hàm đo được (\S 5, No. 3, Hệ quả 5 của Định lý 1). Nếu $1 < p < +\infty$, bất đẳng thức Hölder đối với tích phân trên (Ch. I, No. 3, Mệnh đề 4) cho bất đẳng thức (4), và quan hệ $N_1(fg) < +\infty$ khi đó chỉ ra rằng $fg$ là khả tích (\S 5, No. 6, Định lý 5). Nếu $p = 1$, $q = +\infty$, bất đẳng thức (4) và sự kiện $fg$ là khả tích là những hệ quả ngay lập tức của bất đẳng thức trung bình (No. 2, Mệnh đề 1); do đó định lý được chứng minh trong mọi trường hợp.

#### Hệ quả 1 {#int-iv-s6-thm-2-cor-1 .statement}

— Cho $F, G, H$ là ba không gian Banach, và cho $(u, v) \mapsto \Phi(u, v)$ là một ánh xạ song tuyến tính liên tục của $F \times G$ vào $H$ sao cho $|\Phi(u, v)| \leq |u| \cdot |v|$. Nếu $f \in \mathcal{L}_F^p$ và $g \in \mathcal{L}_G^q$, thì hàm $\Phi(f, g)$ là khả tích và

$$
\left| \int \Phi(f, g)\, d\mu \right| \leq \int |\Phi(f, g)|\, d|\mu| \leq N_p(f) N_q(g).
$$

Vì, $\Phi(f, g)$ là đo được (\S 5, No. 3, Hệ quả 5 của Định lý 1); do $|\Phi(f, g)| \leq |f| \cdot |g|$, hệ quả suy ra từ Định lý 2 và tiêu chuẩn khả tích của \S 5, No. 6, Định lý 5.

Hai trường hợp đặc biệt của Hệ quả 1 có tầm quan trọng trong các ứng dụng:

#### Hệ quả 2 {#int-iv-s6-thm-2-cor-2 .statement}

— Cho $F$ là một không gian Banach thực (tương ứng phức), $F'$ là đối ngẫu mạnh của nó (TVS, III, \S 3, No. 1), và cho $(z, z') \mapsto \langle z, z' \rangle$ là dạng song tuyến tính chính tắc trên $F \times F'$. Nếu $f \in \mathcal{L}_F^p$ và $g \in \mathcal{L}_{F'}^q$, thì hàm thực (tương ứng phức) $\langle f, g \rangle$ là khả tích và

$$
\left| \int \langle f, g \rangle\, d\mu \right| \leq \int |\langle f, g \rangle|\, d|\mu| \leq N_p(f) N_q(g).
$$

Vì, $|\langle z, z' \rangle| \leq |z| \cdot |z'|$.

Khi $F$ là một không gian Hilbert thực hoặc phức, ta biết rằng nó có thể được đồng nhất một cách chính tắc với đối ngẫu $F'$ của nó (TVS, V, \S 1, No. 7). Vì không gian $L_F^2$ là đầy đủ, ta có kết quả sau:

#### Hệ quả 3 {#int-iv-s6-thm-2-cor-3 .statement}

— Cho $\mu$ là một độ đo dương trên $X$, $F$ là một không gian Hilbert thực (tương ứng phức). Trên không gian $L_F^2$, dạng đối xứng (tương ứng Hermit)

$$
(\widetilde{f}, \widetilde{g}) \mapsto \int \langle f, g \rangle\, d\mu
$$

xác định một cấu trúc không gian Hilbert, mà đối với nó chuẩn bằng $\| \widetilde{f} \|_2$.

#### Hệ quả 4 {#int-iv-s6-thm-2-cor-4 .statement}

— Cho $F$ là một không gian Banach, $f$ là một hàm trong $\mathcal{L}_F^p$, và $g$ là một hàm số thuộc $\mathcal{L}^q$; khi đó, hàm $fg$ là khả tích và

$$
\left| \int fg\, d\mu \right| \leq \int |fg|\, d|\mu| \leq N_p(f) N_q(g).
$$

#### Hệ quả 5 {#int-iv-s6-thm-2-cor-5 .statement}

— Cho $f_1, f_2, \ldots, f_n$ là n hàm khả tích dương, và cho $\alpha_1, \alpha_2, \ldots, \alpha_n$ là n số $> 0$ sao cho $\sum_{i=1}^n \alpha_i = 1$; dưới các điều kiện này, hàm $f_1^{\alpha_1} f_2^{\alpha_2} \cdots f_n^{\alpha_n}$ là khả tích và

$$
\int f_1^{\alpha_1} f_2^{\alpha_2} \cdots f_n^{\alpha_n} d|\mu| \leqslant
\left( \int f_1 d|\mu| \right)^{\alpha_1} \left( \int f_2 d|\mu| \right)^{\alpha_2} \cdots \left( \int f_n d|\mu| \right)^{\alpha_n}.
$$

Vì, tích $f_1^{\alpha_1} f_2^{\alpha_2} \cdots f_n^{\alpha_n}$ là đo được, vì nó là tích của các hàm đo được (\S 5, No. 3, Th. 1 và Hệ quả 5 của nó); do bất đẳng thức (8) đúng đối với các tích phân trên (Ch. I, No. 2, Hệ quả của Mệnh đề 2), hàm $f_1^{\alpha_1} f_2^{\alpha_2} \cdots f_n^{\alpha_n}$ là khả tích (\S 5, No. 6, Th. 5), do đó có hệ quả.

Hệ quả 2 của Th. 2 được làm sắc hơn bởi mệnh đề sau:

#### Mệnh đề 3 {#int-iv-s6-prop-3 .statement}

— Cho $\mu$ là một độ đo dương trên X, F là một không gian Banach thực hoặc phức, F' là đối ngẫu mạnh của nó, và $(z, z') \mapsto \langle z, z' \rangle$ là dạng song tuyến tính chính tắc trên $F \times F'$.

1° Với mọi hàm $f \in \mathcal{L}_F^p$ ($1 \leq p \leq +\infty$),

$$
N_p(f) = \sup \left| \int \langle f, g \rangle \, d\mu \right|
$$

khi g chạy qua tập hợp các hàm trong $\mathcal{L}_{F'}^q$, sao cho $N_q(g) \leq 1$.

2° Với mọi hàm $g \in \mathcal{L}_{F'}^q$ ($1 \leq q \leq +\infty$),

$$
N_q(g) = \sup \left| \int \langle f, g \rangle \, d\mu \right|
$$

khi f chạy qua tập hợp các hàm trong $\mathcal{L}_F^p$ sao cho $N_p(f) \leq 1$.

Trước hết ta chứng minh quan hệ (9); ta phân biệt hai trường hợp.

(i) $1 \leq p < +\infty$. Quan hệ (9) là tầm thường khi $N_p(f) = 0$ (vì khi đó f và $\langle f, g \rangle$ là không đáng kể), nên ta luôn có thể giả sử, bằng cách nhân f với một vô hướng, rằng $N_p(f) = 1$. Trước hết giả sử rằng f là một hàm bậc thang khả tích, $f = \sum_{k=1}^n a_k \varphi_{A_k}$, trong đó các $A_k$ rời nhau từng đôi một (\S 4, No. 9, Bổ đề). Do đó $\sum_{k=1}^n |a_k|^p \mu(A_k) = 1$ theo giả thiết. Với mọi $\varepsilon > 0$, tồn tại (với mỗi chỉ số k) một vectơ $a'_k \in F'$ sao cho $|a'_k|^q = |a_k|^p$ nếu $p > 1$ (tương ứng $|a'_k| = 1$ nếu $p = 1$) và $\langle a_k, a'_k \rangle \geq (1 - \varepsilon)|a_k| \cdot |a'_k|$ (TVS, IV,

§1, No. 3, Mệnh đề 8). Đặt $g = \sum_{k=1}^n a_k' \varphi_{A_k}$, ta có $\sum_{k=1}^n |a_k'|^q \mu(A_k) = 1$ nếu $p > 1$ (tương ứng $\sup_{1 \leq k \leq n} |a_k'| = 1$ nếu $p = 1$), do đó $N_q(g) = 1$; mặt khác,

$$
\int \langle f, g \rangle d\mu = \sum_{k=1}^n \langle a_k, a_k' \rangle \mu(A_k) \geq (1 - \varepsilon) \sum_{k=1}^n |a_k| \cdot |a_k'| \mu(A_k)
$$

và, vì $|a_k'| = |a_k|^{p/q} = |a_k|^{p-1}$ nếu $p > 1$ (tương ứng $|a_k'| = 1$ nếu $p = 1$), ta có

$$
\int \langle f, g \rangle d\mu \geq (1 - \varepsilon) \sum_{k=1}^n |a_k|^p \mu(A_k) = (1 - \varepsilon) N_p(f) = 1 - \varepsilon,
$$

điều này chứng minh quan hệ (9) trong trường hợp này.

Ta chuyển sang trường hợp f là một phần tử bất kỳ của $\mathcal{L}_F^p$ sao cho $N_p(f) = 1$. Với mọi $\varepsilon > 0$, tồn tại một hàm bậc thang $f_1 \in \mathcal{L}_F^p$ sao cho $N_p(f - f_1) \leq \varepsilon$ (\S 4, No. 10, Hệ quả 1 của Mệnh đề 19). Theo điều vừa thấy, tồn tại một hàm $g \in \mathcal{L}_F^q$, sao cho $N_q(g) = 1$ và

$$
\int \langle f_1, g \rangle d\mu \geq N_p(f_1) - \varepsilon \geq 1 - 2\varepsilon.
$$

Bây giờ,

$$
\int \langle f, g \rangle d\mu = \int \langle f_1, g \rangle d\mu + \int \langle f - f_1, g \rangle d\mu
$$

và, theo (6),

$$
\left| \int \langle f - f_1, g \rangle d\mu \right| \leq N_p(f - f_1) N_q(g),
$$

do đó

$$
\left| \int \langle f, g \rangle d\mu \right| \geq 1 - 3\varepsilon,
$$

điều này chứng minh (9).

(ii) $p = +\infty$. Ta lại có thể tự hạn chế vào trường hợp $N_\infty(f) > 0$. Cho $\alpha$ là một số tùy ý sao cho $0 < \alpha < N_\infty(f)$; theo giả thiết, tập hợp các $x \in X$ sao cho $|f(x)| > \alpha$ là đo được và không địa phương không đáng kể, do đó nó chứa một tập compact $K$ có độ đo $> 0$. Vì $f$ là đo được, tồn tại một tập compact $K_1 \subset K$ có độ đo $> 0$, sao cho hạn chế của $f$ lên $K_1$ là liên tục. Suy ra rằng, với mọi $\varepsilon > 0$, tồn tại một phân hoạch của $K_1$ thành một số hữu hạn các tập hợp khả tích, trong mỗi tập hợp đó dao động của $f$ là $\leq \varepsilon$; ít nhất một trong các tập hợp này $A$ có độ đo > 0. Gọi $a$ là một trong các giá trị của $f$ trong $A$; khi đó $|a| > \alpha$ và $|f(x) - a| \leq \varepsilon$ với mọi $x \in A$. Tồn tại một vectơ $a' \in F'$ sao cho $|a'| = 1$ và $|\langle a, a' \rangle| \geq |a| - \varepsilon$; hàm $g = \varphi_A \cdot a'/\mu(A)$ là khả tích và $N_1(g) = 1$; mặt khác,

$$
\int \langle f, g \rangle d\mu = \frac{1}{\mu(A)} \int \langle f, a' \rangle \varphi_A d\mu.
$$

Bây giờ, ta có thể viết

$$
\int \langle f, a' \rangle \varphi_A d\mu = \langle a, a' \rangle \mu(A) + \int \langle f - a, a' \rangle \varphi_A d\mu,
$$

và vì

$$
|\langle f - a, a' \rangle \varphi_A| \leq \varepsilon \varphi_A,
$$

ta thấy rằng

$$
\left| \int \langle f, g \rangle d\mu \right| \geq |\langle a, a' \rangle| - \varepsilon \geq |a| - 2\varepsilon > \alpha - 2\varepsilon;
$$

vì $\varepsilon$ là tùy ý và $\alpha$ là bất kỳ số nào < $N_\infty(f)$, quan hệ (9) cũng được kiểm chứng trong trường hợp này.

Ta lập luận hoàn toàn theo cùng một cách để chứng minh quan hệ (10), bằng cách xét riêng trường hợp $1 \leq q < +\infty$ và trường hợp $q = +\infty$, và sử dụng sự kiện rằng với mọi $z' \in F'$, $|z'| = \sup_{|z| \leq 1} |\langle z, z' \rangle|$ theo định nghĩa của chuẩn trong $F'$.

#### Nhận xét {#int-iv-s6-n4-rem-1 .statement}

— 1) Cho $\mathcal{E}$ là một không gian con tuyến tính trù mật của $\mathcal{L}_{F'}^q$; khi đó công thức (9) đúng khi $g$ chạy trên giao của $\mathcal{E}$ với tập hợp $B$ gồm các hàm trong $\mathcal{L}_{F'}^q$ sao cho $N_q(g) \leq 1$. Thật vậy, chỉ cần nhận xét rằng phần trong $\overset{\circ}{B}$ của $B$ là trù mật trong $B$ và rằng $\overset{\circ}{B} \cap \mathcal{E}$ là trù mật trong $\overset{\circ}{B}$, vì $\overset{\circ}{B}$ là mở. Nhận xét này áp dụng riêng cho tập hợp $\mathcal{E} = \mathcal{K}(X; F')$ gồm các hàm liên tục có giá compact (với các giá trị trong $F'$) khi $1 \leq q < +\infty$, nghĩa là, $1 < p \leq +\infty$. Nhưng trong trường hợp này, công thức (9) đúng khi $g$ chạy trên $B \cap \mathcal{K}(X; F')$, ngay cả với $p = 1$. Thật vậy, như trên, ta có thể hạn chế về trường hợp $f$ là một hàm bậc thang. Khi đó ta đã thấy rằng nếu $N_1(f) = 1$, thì với mọi $\varepsilon > 0$ tồn tại một hàm bậc thang $g \in \mathcal{L}_{F'}^\infty$ sao cho $|g(x)| \leq 1$ với mọi $x \in X$ và $|\int \langle f, g \rangle d\mu| \geq 1 - \varepsilon$. Tồn tại một số hữu hạn các tập hợp compact rời nhau từng đôi một $K_i$ sao cho $g$ có giá trị hằng $a'_i$ trên mỗi $K_i$ và sao cho, nếu $K$ là hợp của các $K_i$, thì $\int |f| \varphi_{\mathcal{C}_K} d\mu \leq \varepsilon$. Gọi $U_i$ là một lân cận của $K_i$ sao cho các tập hợp $U_i$ rời nhau từng đôi một, và gọi $h_i$ là một ánh xạ liên tục từ $X$ vào $[0, 1]$ có giá được chứa trong $U_i$ và bằng 1 trên $K_i$. Đặt $h = \sum a'_i h_i$, ta có $h(x) = g(x)$ trên $K$ và $|h(x)| \leq 1$ trên $X$, do đó

$$
\int |\langle f, h \rangle| \varphi_{\mathcal{C}_K} d\mu \leq \varepsilon
$$

và do đó $|\int \langle f, h \rangle d\mu| \geq 1 - 3\varepsilon$, điều này chứng minh mệnh đề của chúng ta. Các nhận xét tương tự có thể được đưa ra cho công thức (10).

2) Cho $\mu$ là một độ đo dương trên $X$, $f$ là một hàm đo được $\geq 0$ (hữu hạn hoặc không) có giá được chứa trong một hợp đếm được của các tập hợp compact $K_n$. Khi đó, với mọi $p$ sao cho $1 \leq p \leq +\infty$,

$$
(11) \quad N_p(f) = \sup \int^* |fg| d\mu,
$$

khi $g$ chạy qua tập hợp các hàm trong $\mathcal{H}(X; \mathbf{R})$ sao cho $N_q(g) \leq 1$. Thật vậy, công thức (11) là một trường hợp đặc biệt của (9) khi $N_p(f) < +\infty$, vì khi đó $f$ tương đương với một hàm trong $\mathcal{L}^p$ (\S 5, No. 6, Định lý 5). Nếu $N_p(f) = +\infty$, với mọi số nguyên $n > 0$ đặt $f_n = \inf(n, f \varphi_{K_n})$. Khi đó

$$
N_p(f_n) = \sup \int^* |f_n g| d\mu \leq \sup \int^* |f g| d\mu,
$$

do đó, khi chuyển qua giới hạn (giả sử, như ta có thể, rằng dãy $(K_n)$ là tăng), ta có $\sup \int^* |f g| d\mu = +\infty$ (\S 1, No. 3, Định lý 3).

#### Hệ quả {#int-iv-s6-n4-cor-1 .statement}

— *Cho $\mu$ là một độ đo dương trên $X$, $F$ là một không gian Banach, $F'$ là đối ngẫu mạnh của nó, và $g$ là một hàm bất kỳ trong $\mathcal{L}^q_{F'}$. Khi đó, dạng tuyến tính trên $L^p_F$, suy ra từ dạng tuyến tính $f \mapsto \int \langle f, g \rangle d\mu$ trên $\mathcal{L}^p_F$ bằng cách chuyển qua thương, là liên tục và có chuẩn $N_q(g)$.*

### 5. Ứng dụng: các quan hệ giữa các không gian $L^p_F$ ($1 \leq p \leq +\infty$)

#### Mệnh đề 4 {#int-iv-s6-prop-4 .statement}

— *Cho $f$ là một hàm đo được với các giá trị trong một không gian Banach $F$; tập hợp $I$ các số $p$, sao cho $1 \leq p \leq +\infty$ và $N_p(f)$ là hữu hạn, hoặc là rỗng hoặc là một khoảng của $\overline{\mathbf{R}}$. Nếu $I$ khác rỗng, hạn chế vào $I$ của ánh xạ $p \mapsto N_p(f)$ là liên tục; hơn nữa, nếu $f$ không đáng kể, $\log N_p(f)$ là một hàm lồi của $1/p$ trên $\bar{I}$.

Ta đã biết (Ch. I, No. 3, Mệnh đề 5) rằng tập hợp $J$ các số *hữu hạn* $p \geq 1$ sao cho $N_p(f) < +\infty$ hoặc là rỗng hoặc là một khoảng, và rằng $\log N_p(f)$ là một hàm lồi của $1/p$ trên $J$ (khi $f$ không đáng kể); điều này dĩ nhiên suy ra tính liên tục của $p \mapsto N_p(f)$ trên $J$.

Nếu $J$ rỗng thì hoặc là $I = \varnothing$ hoặc là $I = \{+\infty\}$, và mệnh đề là hiển nhiên trong trường hợp này; từ nay giả sử rằng $J$ khác rỗng. Mệnh đề cũng hiển nhiên nếu $f$ đáng kể; từ nay giả sử rằng $f$ không đáng kể. Nếu $s \in J$ thì, với mọi số hữu hạn $p > s$, $|f|^p = |f|^s |f|^{p-s}$, và bất đẳng thức của trung bình cho thấy rằng

$$
(12) \quad N_p(f) \leq (N_s(f))^{s/p} (N_\infty(f))^{(p-s)/p}.
$$

Cho $p$ tiến tới $+\infty$, suy ra rằng

$$
\limsup_{p \to +\infty} N_p(f) \leq N_\infty(f).
$$

Điều này chứng minh rằng nếu $+\infty \in I$ thì $J$ chứa các số lớn tùy ý; do đó $I$ thực sự là một khoảng của $\overline{\mathbf{R}}$, và $\overline{I} = \overline{J}$. Mệnh đề sẽ được chứng minh nếu ta chỉ ra rằng $p \mapsto N_p(f)$ là liên tục trên $\overline{J}$, và chỉ cần thiết lập tính liên tục tại các đầu mút của $J$. Hơn nữa, ta có thể giả sử rằng $J$ không rút gọn thành một điểm. Gọi $r$ và $s$ là các đầu mút trái và phải của $J$ ($r < s \leq +\infty$). Gọi $A$ là tập hợp (đo được) các $x \in X$ sao cho $|f(x)| \geq 1$; khi đó

$$
\int |f|^p d|\mu| = \int |f|^p \varphi_A d|\mu| + \int |f|^p \varphi_{C_A} d|\mu|.
$$

Khi $p \in J$ tiến tới $r$, $|f|^p \varphi_A$ tiến tới $|f|^r \varphi_A$ trong khi giảm, và $|f|^p \varphi_{C_A}$ tiến tới $|f|^r \varphi_{C_A}$ trong khi tăng. Do đó $\int |f|^p \varphi_{C_A} d|\mu|$ tiến tới $\int^* |f|^r \varphi_{C_A} d|\mu|$ (\S1, No. 3, Th. 3). Mặt khác, $|f|^p \varphi_A$ khả tích đối với $p \in J$, và $\int |f|^p \varphi_A d|\mu|$ tiến tới $\int |f|^r \varphi_A d|\mu|$ (\S4, No. 3, Prop. 4). Vì vậy $\int |f|^p d|\mu|$ tiến tới $\int^* |f|^r d|\mu|$, điều này chứng minh tính liên tục của $p \mapsto N_p(f)$ tại $r$.

Có thể áp dụng cùng một lập luận tại điểm $s$ nếu $s < +\infty$. Cuối cùng, giả sử rằng $s = +\infty$. Theo (13), chỉ cần chứng minh rằng

$$
\liminf_{p \to +\infty} N_p(f) \geq N_\infty(f).
$$

Bây giờ, cho $a$ là một số sao cho $0 < a < N_\infty(f)$. Vì theo giả thiết, tồn tại các giá trị hữu hạn của $p$ sao cho $N_p(f) < +\infty$, tập hợp $A$ gồm các $x \in X$ sao cho $|f(x)| \geq a$, là đo được và không có độ đo bằng không, là khả tích nhờ bất đẳng thức $\varphi_A \leq (|f|/a)^p$; hơn nữa, từ bất đẳng thức này ta suy ra rằng $N_p(f) \geq a \cdot (|\mu|(A))^{1/p}$; cho $p$ tiến tới $+\infty$, suy ra rằng $\liminf_{p \to +\infty} N_p(f) \geq a$, điều này hoàn tất chứng minh.

Lập luận tương tự cũng được áp dụng tại điểm $s$ nếu $s < +\infty$. Cuối cùng, giả sử rằng $s = +\infty$. Theo (13), chỉ cần chứng minh rằng

$$
\liminf_{p \to +\infty} N_p(f) \geq N_\infty(f).
$$

Bây giờ, cho $a$ là một số sao cho $0 < a < N_\infty(f)$. Vì theo giả thiết, tồn tại các giá trị hữu hạn của $p$ sao cho $N_p(f) < +\infty$, tập hợp $A$ gồm các $x \in X$ sao cho $|f(x)| \geq a$, là đo được và không có độ đo bằng không, là khả tích nhờ bất đẳng thức $\varphi_A \leq (|f|/a)^p$; hơn nữa, từ bất đẳng thức này ta suy ra rằng $N_p(f) \geq a \cdot (|\mu|(A))^{1/p}$; cho $p$ tiến tới $+\infty$, suy ra rằng $\liminf_{p \to +\infty} N_p(f) \geq a$, điều này hoàn tất chứng minh.

#### Hệ quả {#int-iv-s6-n5-cor-1 .statement}

— *Nếu* $r, s, p$ *là ba số sao cho*

$$
1 \leq r < p < s \leq +\infty,
$$

*thì giao* $\mathcal{L}_F^r \cap \mathcal{L}_F^s$ *được chứa trong* $\mathcal{L}_F^p$.

Nhận xét rằng nói chung các tôpô cảm sinh trên giao $\mathcal{L}_F^r \cap \mathcal{L}_F^s$ bởi các tôpô của các $\mathcal{L}_F^p$ ($r < p < s$) là *phân biệt*. Nếu không đặt thêm giả thiết nào về $\mu$, các tôpô cảm sinh trên $\mathcal{L}_F^r \cap \mathcal{L}_F^s$ bởi các tôpô của $\mathcal{L}_F^r$ và $\mathcal{L}_F^s$ nói chung không so sánh được (nói cách khác, tỉ số $N_r(f)/N_s(f)$ có thể nhận các giá trị lớn tùy ý và các giá trị nhỏ tùy ý trong $\mathcal{L}_F^r \cap \mathcal{L}_F^s$; cf. Exer. 8).

Mệnh đề 4 có thể được làm sắc hơn khi $\mu$ là một độ đo bị chặn:

#### Mệnh đề 5 {#int-iv-s6-prop-5 .statement}

— Cho $\mu$ là một độ đo bị chặn, và cho $f$ là một hàm $\mu$-đo được với các giá trị trong một không gian Banach $F$. Tập hợp I các số $p$ sao cho $1 \leq p \leq +\infty$ và $N_p(f)$ là hữu hạn, hoặc là rỗng hoặc là một khoảng với điểm đầu bên trái $p = 1$ và chứa điểm này; hơn nữa, $(|\mu|(X))^{-1/p} N_p(f)$ là một hàm tăng của $p$ trên I.

Đây là một hệ quả ngay lập tức của Mệnh đề 4 ở trên và của Hệ quả của Mệnh đề 4 trong Ch. I, No. 3.

#### Hệ quả {#int-iv-s6-n5-cor-2 .statement}

— Nếu độ đo $\mu$ bị chặn, quan hệ $r < s$ kéo theo $\mathcal{L}_F^s \subset \mathcal{L}_F^r$; hơn nữa, tôpô của sự hội tụ theo trung bình cấp $s$ mịn hơn tôpô của sự hội tụ theo trung bình cấp $r$ (trên $\mathcal{L}_F^s$).

Có thể chỉ ra rằng nói chung tôpô của sự hội tụ theo trung bình cấp $s$ thực sự mịn hơn tôpô của sự hội tụ theo trung bình cấp $r$ (Exer. 8).

#### Mệnh đề 6 {#int-iv-s6-prop-6 .statement}

— Cho $X$ là một không gian rời rạc, $\mu$ là độ đo trên $X$ được xác định bằng cách đặt khối lượng $+1$ tại mỗi điểm của $X$. Nếu $f$ là một ánh xạ từ $X$ vào không gian Banach $F$, tập hợp I các số $p$ sao cho $1 \leq p \leq +\infty$ và $N_p(f)$ là hữu hạn, hoặc là rỗng hoặc là một khoảng với điểm đầu bên phải $+\infty$ và chứa điểm này; hơn nữa, $N_p(f)$ là một hàm giảm của $p$ trên I.

Vì, $\mu^*(|f|) = \sum_{x \in X} |f(x)|$ đối với mọi hàm $f$ (\S 1, No. 1, Ví dụ), và $N_\infty(f) = \|f\| = \sup_{x \in X} |f(x)|$; nếu tồn tại một số $\alpha > 0$ sao cho $|f(x)| \geq \alpha$ đối với vô hạn giá trị của $x \in X$, thì $N_p(f) = +\infty$ đối với mọi $p$ hữu hạn; trong trường hợp ngược lại, tồn tại một $x_0 \in X$ sao cho $|f(x_0)| = \|f\|$, do đó

$$
N_\infty(f) = |f(x_0)| \leq N_p(f)
$$

đối với mọi $p$ hữu hạn. Vì hàm $\log N_p(f)$ là lồi đối với $1/p$ và nhận giá trị nhỏ nhất của nó tại điểm $+\infty$, nên nó tất yếu là một hàm giảm của $p$ trên I (FRV, I, \S 4, No. 3, Mệnh đề 5), điều này hoàn thành chứng minh.

#### Hệ quả {#int-iv-s6-n5-cor-3 .statement}

— Nếu $X$ là rời rạc và độ đo $\mu$ được xác định bởi một khối lượng $+1$ tại mỗi điểm của $X$, thì quan hệ $r < s$ kéo theo $\mathcal{L}_F^r \subset \mathcal{L}_F^s$; hơn nữa, tôpô của sự hội tụ theo trung bình cấp $r$ mịn hơn tôpô của sự hội tụ theo trung bình cấp $s$ (trên $\mathcal{L}_F^r$).

### Bài tập {#int-iv-s6-exercises}

Xem [các bài tập cho § 6](exercises/s6/).
