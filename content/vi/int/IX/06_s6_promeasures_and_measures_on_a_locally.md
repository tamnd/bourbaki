---
book: int
book_title: Integration
chapter: IX
chapter_title: MEASURES ON HAUSDORFF TOPOLOGICAL SPACES
section: 6
section_title: Promeasures and measures on a locally convex space
lang: vi
source: int-vii-ix
book_pages: INT IX.72-INT IX.101, INT IX.117
pdf_pages: 0254-0283, 0299-0299
extraction: ocr
subsections:
    - "no": 1
      title: Promeasures on a locally convex space
      page: 72
      pdf_page: 254
    - "no": 2
      title: Image of a promeasure
      page: 74
      pdf_page: 256
    - "no": 3
      title: Fourier transform of a promeasure
      page: 75
      pdf_page: 257
    - "no": 4
      title: Calculation of Gaussian integrals
      page: 77
      pdf_page: 259
    - "no": 5
      title: Gaussian promeasures and measures
      page: 78
      pdf_page: 260
    - "no": 6
      title: Examples of Gaussian promeasures
      page: 82
      pdf_page: 264
    - "no": 7
      title: Wiener measure
      page: 85
      pdf_page: 267
    - "no": 8
      title: Continuity of the Fourier transform
      page: 92
      pdf_page: 274
    - "no": 9
      title: Minlos’s lemma
      page: 93
      pdf_page: 275
    - "no": 10
      title: Measures on the dual of a nuclear space
      page: 96
      pdf_page: 278
    - "no": 11
      title: Measures on a Hilbert space
      page: 97
      pdf_page: 279
statements: 33
exercises: 1
content_sha256: e0d0e01292f1757196d93ff07df77c5294d37b88558319f6118506292c65c707
translated_from: content/en/int/IX/06_s6_promeasures_and_measures_on_a_locally.md
source_content_sha256: f5af6278d6bcac9db62099468624d04d8e4f8c4d55064bcd03a2261c3d9724ac
translation_model: gpt-5.4-mini, gpt-5-6-mini
translation_run: translate-vi-9d47048b
glossary_version: 34
glossary_terms_sha256: f0a5a2fc8c5cd3b6ef7201d06523aef5de50d1e2707eb58f94f181805a8069a1
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 6. TIỀN ĐỘ ĐO VÀ ĐỘ ĐO TRÊN MỘT KHÔNG GIAN LỒI ĐỊA PHƯƠNG

Trong suốt tiết này, chỉ xét các không gian vectơ trên trường số thực. Một không gian lồi địa phương là một không gian vectơ tôpô trên $\mathbf{R}$, Hausdorff và lồi địa phương. Đối ngẫu tôpô của một không gian lồi địa phương E sẽ được ký hiệu là $E'$; với $x \in E$ và $x' \in E'$, ta viết $\langle x, x' \rangle = x'(x)$.

### 1. Tiền độ đo trên một không gian lồi địa phương

Cho E là một không gian lồi địa phương. Ta ký hiệu $\mathcal{F}(E)$ là tập hợp các không gian con tuyến tính đóng của E có đối chiều hữu hạn, được sắp thứ tự bởi quan hệ $\supset$. Với mọi $V \in \mathcal{F}(E)$, $p_V$ ký hiệu ánh xạ chính tắc của E lên $E/V$. Cho V và W là hai phần tử của $\mathcal{F}(E)$ sao cho $V \supset W$; ta ký hiệu $p_{VW}$ là ánh xạ từ $E/W$ vào $E/V$ suy ra từ ánh xạ đồng nhất của E khi chuyển sang các thương. Họ $\mathcal{Q}(E) = (E/V, p_{VW})$ là một hệ ngược các không gian lồi địa phương, được chỉ số hóa bởi $\mathcal{F}(E)$. Nó được gọi là *hệ ngược các thương hữu hạn chiều của E*.

Có thể chứng minh rằng giới hạn ngược của hệ ngược $\mathcal{Q}(E)$ đẳng cấu chính tắc với đối ngẫu đại số $E'{}^*$ của $E'$, được trang bị tôpô yếu $\sigma(E'{}^*, E')$.

#### Định nghĩa 1 {#int-ix-s6-def-1 .statement}

*Cho $E$ là một không gian lồi địa phương. Người ta gọi tiền độ đo trên $E$ là mọi hệ ngược$^{(1)}$ các độ đo (\S 4, No. 2, Định nghĩa 1) trên hệ ngược các thương hữu hạn chiều của $E$.*

Nói cách khác, một tiền độ đo $\mu$ trên $E$ là một họ $(\mu_V)_{V \in \mathscr{F}(E)}$, trong đó $\mu_V$ là một độ đo bị chặn (dương) trên không gian hữu hạn chiều $E/V$, và trong đó $\mu_V = p_{VW}(\mu_W)$ khi $V \supset W$. Tất cả các độ đo $\mu_V$ đều có cùng tổng khối lượng, gọi là *tổng khối lượng* của tiền độ đo $\mu$.

Để một không gian con $V$ của $E$ thuộc $\mathscr{F}(E)$, điều kiện cần và đủ là tồn tại một số hữu hạn phần tử $x'_1, \ldots, x'_n$ của $E'$ sao cho $V$ gồm các $x \in E$ thỏa mãn $\langle x, x'_i \rangle = 0$ với $1 \leq i \leq n$ (TVS, II, \S 6, No. 3, Hệ quả 2 của Định lý 1 và No. 5, Hệ quả 2 của Mệnh đề 7). Hơn nữa, trên một không gian vectơ hữu hạn chiều chỉ tồn tại một và chỉ một tôpô không gian vectơ Hausdorff (TVS, I, \S 2, No. 3, Định lý 2). Do đó, khái niệm tiền độ đo trên $E$ chỉ phụ thuộc vào đối ngẫu $E'$ của $E$.

Cho $\lambda$ là một độ đo bị chặn trên $E$. Với mọi $V \in \mathscr{F}(E)$, ta ký hiệu bởi $\widetilde{\lambda}_V$ ảnh của $\lambda$ qua ánh xạ chính tắc $p_V$ của $E$ lên $E/V$. Ta có $p_V = p_{VW} \circ p_W$ đối với hai phần tử bất kỳ $V$ và $W$ của $\mathscr{F}(E)$ sao cho $V \supset W$; do đó, họ $\widetilde{\lambda} = (\widetilde{\lambda}_V)_{V \in \mathscr{F}(E)}$ là một độ đo tiền trên $E$. Ta sẽ nói rằng $\widetilde{\lambda}$ là độ đo tiền *liên kết* với độ đo $\lambda$. Ta thấy ngay lập tức rằng $\lambda$ và $\widetilde{\lambda}$ có cùng khối lượng toàn phần.

#### Mệnh đề 1 {#int-ix-s6-prop-1 .statement}

*Cho $E$ là một không gian lồi địa phương. Ánh xạ $\lambda \mapsto \widetilde{\lambda}$ là một song ánh từ tập hợp các độ đo bị chặn trên $E$ lên tập hợp các độ đo tiền $(\mu_V)_{V \in \mathscr{F}(E)}$ trên $E$ thỏa mãn điều kiện sau:

Với mọi $\varepsilon > 0$, tồn tại một tập con compact $K$ của $E$ sao cho $\mu_V(E/V - p_V(K)) \leq \varepsilon$ với mọi $V \in \mathscr{F}(E)$.*

Người ta biết rằng giao của các hạt nhân của các dạng tuyến tính liên tục trên $E$ bằng 0 (TVS, II, \S 4, No. 1, Cor. 1 of Prop. 2); do đó $\bigcap_{V \in \mathscr{F}(E)} V = \{0\}$ và họ $(p_V)_{V \in \mathscr{F}(E)}$ là nhất quán và phân tách. Mệnh đề khi đó suy ra từ Th. 1 của \S 4, No. 2.

Đặc biệt, ánh xạ $\lambda \mapsto \widetilde{\lambda}$ là đơn ánh. Nếu $\mu$ là một độ đo tiền trên $E$, và nếu tồn tại một độ đo bị chặn $\lambda$ trên $E$ sao cho $\mu = \widetilde{\lambda}$, ta sẽ nói, bằng một sự lạm dụng ngôn ngữ, rằng $\mu$ là một độ đo. Nếu $E$ là hữu hạn chiều, mọi độ đo tiền $\mu = (\mu_V)_{V \in \mathscr{F}(E)}$ đều là một độ đo: vì, $\{0\} \in \mathscr{F}(E)$, $E/\{0\} = E$ và $p_{V,\{0\}} = p_V$, do đó $\mu_V = p_V(\mu_{\{0\}})$ với mọi $V \in \mathscr{F}(E)$; nói cách khác, $\mu = \widetilde{\lambda}$ với $\lambda = \mu_{\{0\}}$.

(1) Còn được gọi là một 'hệ xạ ảnh'.

#### Mệnh đề 2 {#int-ix-s6-prop-2 .statement}

— Cho T là một tập hợp đếm được, và E là không gian vectơ của các hàm thực trên T, được trang bị bởi tôpô của sự hội tụ điểm. Mọi độ đo tiền trên E đều là một độ đo.

### 2. Ảnh của một tiền độ đo

Với mọi $t \in T$, hãy ký hiệu $\varepsilon_t$ là dạng tuyến tính $f \mapsto f(t)$ trên E. Ta biết (TVS, II, §6, No. 6, Cor. 2 of Prop. 8) rằng họ $(\varepsilon_t)_{t \in T}$ là một cơ sở của không gian vectơ $E'$. Ký hiệu $\Phi$ là tập các tập con hữu hạn của 'T', và với mọi $J \in \Phi$ hãy đặt $E_J$ là tập hợp các hàm trên T bằng 0 tại mọi điểm của J. Cho $F \in \mathcal{F}(E)$; vì phần trực giao $F^\circ$ của F là một không gian con hữu hạn chiều của $E'$, tồn tại $J \in \Phi$ sao cho $F^\circ$ được chứa trong không gian con tuyến tính G của $E'$ được sinh bởi các $\varepsilon_t$ với $t \in J$. Vì $F^\circ \subset G$, ta có $E_J = G^\circ \subset F^{\circ\circ} = F$ và họ đếm được $(E_J)_{J \in \Phi}$ là đồng cuối trong $\mathcal{F}(E)$. Mệnh đề suy ra từ Định lý 2 của §4, No. 3.

Cho E và $E_1$ là hai không gian lồi địa phương, và $u$ là một ánh xạ tuyến tính liên tục của E vào $E_1$. Với mọi $V_1 \in \mathcal{F}(E_1)$, không gian con $V = \overline{u}^{-1}(V_1)$ của E thuộc $\mathcal{F}(E)$, và $u$ xác định, bằng cách qua các thương, một ánh xạ tuyến tính $u_{V_1}$ của $E/V$ vào $E_1/V_1$. Cho $V_1$ và $W_1$ trong $\mathcal{F}(E_1)$ sao cho $V_1 \supset W_1$; đặt $V = \overline{u}^{-1}(V_1)$ và $W = \overline{u}^{-1}(W_1)$. Ta có $V \supset W$, và một biểu đồ giao hoán

$$
\begin{array}{ccc}
E & \xrightarrow{pw} & E/W & \xrightarrow{pvw} & E/V \\
\downarrow u & & \downarrow u_{W_1} & & \downarrow u_{V_1} \\
E_1 & \xrightarrow{pw_1} & E_1/W_1 & \xrightarrow{pv_{1W_1}} & E_1/V_1
\end{array}
$$

Bây giờ cho $\mu = (\mu_V)_{V \in \mathcal{F}(E)}$ là một tiền độ đo trên E. Với mọi $V_1 \in \mathcal{F}(E_1)$, đặt

(1)
$$
\nu_{V_1} = u_{V_1}(\mu_{u^{-1}(V_1)}).
$$

Tính giao hoán của biểu đồ trên cho thấy họ $\nu = (\nu_{V_1})_{V_1 \in \mathcal{F}(E_1)}$ là một tiền độ đo trên $E_1$. Ta nói rằng $\nu$ là ảnh của $\mu$ qua $u$, và ký hiệu nó là $u(\mu)$.

Cho $\lambda$ là một độ đo bị chặn trên E, và $u(\lambda)$ là độ đo trên $E_1$ là ảnh của $\lambda$ qua $u$. Nếu tiền độ đo $\mu$ liên kết với $\lambda$, thì tiền độ đo $u(\mu)$ liên kết với $u(\lambda)$. Điều này suy ra từ tính giao hoán của biểu đồ trên.

Cho $V \in \mathcal{F}(E)$. Ngay lập tức thấy rằng ảnh của tiền độ đo trên $E/V$ của tiền độ đo $\mu$ theo ánh xạ chính tắc $p_V : E \to E/V$ liên kết với độ đo $\mu_V$.

Cho $u_1$ là một ánh xạ tuyến tính liên tục của $E_1$ vào một không gian lồi địa phương $E_2$. Ta thiết lập không khó khăn quan hệ

$$
(u_1 \circ u)(\mu) = u_1(u(\mu))
$$

*(tính bắc cầu của các ảnh của các tiền độ đo)*.

### 3. Biến đổi Fourier của một tiền độ đo

Cho $E$ là một không gian lồi địa phương và $\mu = (\mu_V)_{V \in \mathcal{F}(E)}$ là một tiền độ đo trên $E$. Với mọi dạng tuyến tính liên tục $x'$ trên $E$, ta ký hiệu $\mu_{x'}$ là độ đo trên $\mathbf{R}$ là ảnh theo $x'$ của tiền độ đo $\mu$ trên $E$. Biến đổi Fourier của $\mu$ là hàm $\mathcal{F}\mu$ trên $E'$ được xác định bởi

$$
(\mathcal{F}\mu)(x') = \int_{\mathbf{R}} e^{it} d\mu_{x'}(t).
$$

Cho $\lambda$ là một độ đo bị chặn trên $E$. Biến đổi Fourier của $\lambda$ là hàm trên $E'$ được xác định bởi

$$
(\mathcal{F}\lambda)(x') = \int_E e^{i\langle x, x' \rangle} d\lambda(x).
$$

Cho $\mu$ là tiền độ đo liên kết với $\lambda$. Với mọi $x' \in E'$, độ đo $\mu_{x'}$ trên $\mathbf{R}$ là ảnh theo $x' : E \to \mathbf{R}$ của độ đo $\lambda$ trên $E$; từ các công thức (2) và (3), ta ngay lập tức suy ra $\mathcal{F}\mu = \mathcal{F}\lambda$.

Cho $\mu$ là một tiền độ đo bất kỳ trên $E$, và $u$ là một ánh xạ tuyến tính liên tục của $E$ vào một không gian lồi địa phương $E_1$. Ký hiệu $^t u$ là ánh xạ tuyến tính của $E'_1$ vào $E'$ là chuyển vị của $u$, và ký hiệu $\nu$ là tiền độ đo $u(\mu)$ trên $E_1$. Với mọi $x'_1 \in E'_1$, ta có $^t u(x'_1) = x'_1 \circ u$, do đó

$$
\nu_{x'_1} = x'_1(\nu) = x'_1(u(\mu)) = (x'_1 \circ u)(\mu) = \mu_{^t u(x'_1)}.
$$

Do đó,

$$
\mathcal{F}(u(\mu)) = (\mathcal{F}\mu) \circ {}^t u.
$$

Đặc biệt, ta lấy $u$ là ánh xạ chính tắc $p_V$ của $E$ lên $E/V$ (với $V \in \mathcal{F}(E)$). Độ đo tiền $p_V(\mu)$ trên $E/V$ liên kết với độ đo $\mu_V$, và $^t p_V$ là một đẳng cấu từ đối ngẫu của $E/V$ lên không gian con $V^\circ$ của $E'$ vuông góc với $V$. Nếu $(E/V)'$ được đồng nhất với $V^\circ$ bằng $^t p_V$, thì

$$
(\mathcal{F}\mu)(x') = \int_{E'/V} e^{i\langle x, x' \rangle} d\mu_V(x)
$$

với mọi $x' \in V^\circ$. Ta có $E' = \bigcup_{V \in \mathscr{F}(E)} V^\circ$, do đó công thức trước đó đặc trưng hàm $\mathcal{F}\mu$ trên $E'$. Cuối cùng, nếu đặt $x' = 0$ trong (5), ta thấy khối lượng toàn phần của $\mu$ bằng $(\mathcal{F}\mu)(0)$.

#### Mệnh đề 3 {#int-ix-s6-prop-3 .statement}

*Cho $E$ là một không gian lồi địa phương. Ánh xạ $\mu \mapsto \mathcal{F}\mu$ từ tập hợp các độ đo tiền trên $E$ vào tập hợp các hàm trên $E'$ là đơn ánh.*

Công thức (5) cho phép quy về trường hợp $E$ là hữu hạn chiều; vì mọi không gian hữu hạn chiều đều đẳng cấu với một không gian $\mathbf{R}^n$, ta thậm chí có thể giả sử tồn tại một số nguyên $n \geqslant 0$ sao cho $E = \mathbf{R}^n$. Do đó ta phải chứng minh rằng nếu $\mu$ là một độ đo bị chặn (không nhất thiết dương) trên $\mathbf{R}^n$ và nếu

$$
\int_{\mathbf{R}^n} e^{i\langle x, y \rangle} d\mu(x) = 0
$$

với mọi dạng tuyến tính $y$ trên $\mathbf{R}^n$, thì $\mu = 0$.

Với mọi số nguyên $m \geqslant 0$, gọi $G_m$ là nhóm con $m \cdot \mathbf{Z}^n$ của $\mathbf{R}^n$. Ký hiệu $\mathscr{C}_m$ là không gian vectơ các hàm liên tục $f$ trên $\mathbf{R}^n$ sao cho $f(x + a) = f(x)$ với $x \in \mathbf{R}^n$ và $a \in G_m$. Theo Mệnh đề 8 của GT, X, §4, No. 4, mọi hàm trong $\mathscr{C}_m$ là giới hạn đều của các tổ hợp tuyến tính hữu hạn của các hàm kiểu $x \mapsto e^{2\pi i \langle x, q \rangle}$ với $q \in m^{-1} \cdot \mathbf{Z}^n$. Do đó $\mu(f) = 0$ với mọi hàm $f \in \mathscr{C}_m$.

Let $f$ be a continuous function on $\mathbf{R}^n$ with compact support. Với mọi số nguyên $m \geqslant 0$, đặt $f_m(x) = \sum_{q \in G_m} f(x + q)$. Hiển nhiên rằng với mọi $x \in \mathbf{R}^n$, chuỗi trước có chỉ hữu hạn nhiều số hạng, và $f_m$ thuộc $\mathscr{C}_m$. Hơn nữa, dễ thấy rằng dãy $(f_m)$ tiến tới $f$ đều trên mọi tập compact, và rằng tồn tại một hằng số $C \geqslant 0$ sao cho $|f_m| \leqslant C$ với mọi $m$. Do đó, $\mu(f) = \lim_{m \to \infty} \mu(f_m)$ theo Mệnh đề 12 của §5, No. 6. Vì $f_m \in \mathscr{C}_m$, ta có $\mu(f_m) = 0$, do đó cuối cùng $\mu(f) = 0$. Vậy $\mu = 0$.

#### Nhận xét {#int-ix-s6-n3-rem-1 .statement}

— Khi $E$ có số chiều hữu hạn, mọi đặc trưng của $E$ đều có dạng $x \mapsto e^{i\langle x, x' \rangle}$ với $x' \in E'$ (*Théor. spect.*, Ch. II, §1, No. 9, Hệ quả 3 của Mệnh đề 12). Trong trường hợp này, Mệnh đề 3 suy ra từ định lý duy nhất cho phép biến đổi Fourier (*loc. cit.*, §1, No. 6, Hệ quả của Mệnh đề 6).*

### 4. Tính các tích phân Gaussian

#### Bổ đề 1 {#int-ix-s6-lem-1 .statement}

Với mọi số nguyên $n \geqslant 0$,

$$
\int_{\mathbf{R}} |x|^n e^{-x^2/2} dx = 2^{n+1 \over 2} \Gamma \left( {n+1 \over 2} \right)
$$
(6)

$$
\int_{\mathbf{R}} x^{2n} e^{-x^2/2} dx = (2\pi)^{1/2} \frac{(2n)!}{2^n n!}
$$
(7)

$$
\int_{\mathbf{R}} x^{2n+1} e^{-x^2/2} dx = 0.
$$
(8)

Nhắc lại công thức

$$
\Gamma(s) = \int_0^\infty u^{s-1} e^{-u} du
$$
(9)

đúng với mọi số thực $s > 0$ (FRV, VII, §1, No. 3, Mệnh đề 3). Khi thực hiện đổi biến $x = (2u)^{1/2}$, từ (9) suy ra rằng

$$
\int_0^\infty x^n e^{-x^2/2} dx = \int_0^\infty (2u)^{n/2} e^{-u} {1 \over 2} 2^{1/2} u^{-1/2} du = 2^{n-1 \over 2} \Gamma \left( {n+1 \over 2} \right),
$$

do đó có công thức (6) vì

$$
\int_{\mathbf{R}} |x|^n e^{-x^2/2} dx = 2 \int_0^\infty x^n e^{-x^2/2} dx.
$$

Công thức (7) suy ra từ (6) và quan hệ

$$
\Gamma \left( n + \frac{1}{2} \right) = \pi^{1/2} \frac{(2n)!}{2^{2n} n!}.
$$
(10)

Với $n = 0$, quan hệ này rút gọn thành $\Gamma(\frac{1}{2}) = \pi^{1/2}$, tức là công thức (21) của FRV, VII, §1, No. 3. Trường hợp tổng quát sau đó suy ra bằng quy nạp theo $n$, khi xét đến quan hệ $\Gamma(x+1) = x \cdot \Gamma(x)$ (loc. cit., §1, No. 1).

Cuối cùng, công thức (8) suy ra từ thực tế rằng hàm $x \mapsto x^{2n+1} e^{-x^2/2}$ là lẻ.

#### Bổ đề 2 {#int-ix-s6-lem-2 .statement}

Với mọi số phức $y$,

$$
(2\pi)^{-1/2} \int_{\mathbf{R}} e^{-x^2/2} e^{ixy} dx = e^{-y^2/2}.
$$
(11)

Đặc biệt,

$$
(2\pi)^{-1/2} \int_{\mathbf{R}} e^{-x^2/2} dx = 1.
$$

Đổi biến $x \mapsto -x$ cho

$$
(2\pi)^{-1/2} \int_{\mathbf{R}} e^{-x^2/2} e^{i xy} dx = (2\pi)^{-1/2} \int_{\mathbf{R}} e^{-x^2/2} e^{-ixy} dx;
$$

vì $\cos u = \frac{e^{iu} + e^{-iu}}{2}$ với mọi số phức $u$, suy ra rằng

$$
(12) \quad (2\pi)^{-1/2} \int_{\mathbf{R}} e^{-x^2/2} e^{i xy} dx = (2\pi)^{-1/2} \int_{\mathbf{R}} e^{-x^2/2} \cos xy \, dx .
$$

Với mọi số nguyên $n \geqslant 0$, đặt

$$
g_n(x) = (-1)^n (2\pi)^{-1/2} \frac{(xy)^{2n}}{(2n)!} e^{-x^2/2}.
$$

Theo (7),

$$
(13) \quad \int_{\mathbf{R}} |g_n(x)| \, dx = \frac{1}{n!} \left( \frac{|y|^2}{2} \right)^n
$$
$$
(14) \quad \int_{\mathbf{R}} g_n(x) \, dx = \frac{1}{n!} \left( -\frac{y^2}{2} \right)^n,
$$

do đó

$$
\sum_{n=0}^{\infty} \int_{\mathbf{R}} |g_n(x)| \, dx = e^{|y|^2/2} < +\infty.
$$

Vì hơn nữa,

$$
(2\pi)^{-1/2} e^{-x^2/2} \cos xy = \sum_{n=0}^{\infty} g_n(x),
$$

đẳng thức này có thể được tích phân từng hạng, do đó

$$
(2\pi)^{-1/2} \int_{\mathbf{R}} e^{-x^2/2} \cos xy \, dx = \sum_{n=0}^{\infty} \int_{\mathbf{R}} g_n(x) \, dx = e^{-y^2/2}
$$

theo (14). Công thức (11) khi đó suy ra từ (12).

### 5. Tiền đo Gaussian và các độ đo

#### Mệnh đề 4 {#int-ix-s6-prop-4 .statement}

*Cho E là một không gian lồi địa phương. Với mọi dạng toàn phương dương Q trên E', tồn tại duy nhất một tiền đo $\Gamma_Q$ trên E sao cho $\mathcal{F} \Gamma_Q = e^{-Q/2}$. Khối lượng toàn phần của $\Gamma_Q$ bằng 1.*

Tính duy nhất của $\Gamma_Q$ suy ra từ Mệnh đề 3 của No. 3. Khối lượng toàn phần của $\Gamma_Q$ bằng $(\mathcal{F}\Gamma_Q)(0) = e^{-Q(0)/2} = 1$. Ta sẽ chứng minh sự tồn tại theo từng bước.

A) E có số chiều hữu hạn n, và Q không suy biến.

Theo Bổ đề 2 của No. 4, độ đo $\gamma_1$ trên $\mathbf{R}$ có mật độ $t \mapsto (2\pi)^{-1/2}e^{-t^2/2}$ là bị chặn, có tổng khối lượng bằng 1. Đặt $\gamma = \gamma_1 \otimes \cdots \otimes \gamma_1$ ($n$ thừa số). Từ Bổ đề 2 của No. 4, suy ra

$$
\int_{\mathbf{R}^n} e^{i(a_1 t_1 + \cdots + a_n t_n)} d\gamma(t_1, \ldots, t_n) = \prod_{j=1}^n \int_{\mathbf{R}} e^{ia_j t} d\gamma_1(t)
$$
$$
= \prod_{j=1}^n (2\pi)^{-1/2} \int_{\mathbf{R}} e^{ia_j t} e^{-t^2/2} dt
$$
$$
= \prod_{j=1}^n e^{-a_j^2/2}
$$
$$
= \exp \left( -\frac{1}{2}(a_1^2 + \cdots + a_n^2) \right).
$$

Vì Q dương và không suy biến, tồn tại một cơ sở $(e'_1, \ldots, e'_n)$ của E' trực chuẩn đối với Q (Alg., Ch. IX, §7, No. 1). Ký hiệu f là đẳng cấu $x \mapsto (e'_1(x), \ldots, e'_n(x))$ của E lên $\mathbf{R}^n$, và ký hiệu $\Gamma_Q$ là độ đo $f^{-1}(\gamma)$ trên E. Cho $x' = a_1 e'_1 + \cdots + a_n e'_n$ thuộc E'; khi đó $x'(f^{-1}(t_1, \ldots, t_n)) = \sum_{j=1}^n t_j a_j$ với $t_1, \ldots, t_n$ thực, do đó

$$
\int_E e^{i\langle x, x' \rangle} d\Gamma_Q(x) = \int_{\mathbf{R}^n} e^{i(a_1 t_1 + \cdots + a_n t_n)} d\gamma(t_1, \ldots, t_n)
$$
$$
= \exp \left( -\frac{1}{2}(a_1^2 + \cdots + a_n^2) \right) = \exp \left( -\frac{1}{2}Q(x') \right).
$$

Do đó, $\mathcal{F}\Gamma_Q = e^{-Q/2}$.

B) E hữu hạn chiều.

Cho N là không gian con tuyến tính của E' gồm các $x'$ sao cho $Q(x') = 0$. Ký hiệu M là phần trực giao của N trong E, và j là đơn ánh chính tắc của M vào E. Ánh xạ tuyến tính ${}^t j : E' \to M'$ là toàn ánh, với hạt nhân N, do đó tồn tại trên $M'$ một dạng toàn phương dương không suy biến q sao cho $Q = q \circ {}^t j$. Theo trên, tồn tại một độ đo bị chặn $\Gamma$ trên M sao cho $\mathcal{F}\Gamma = e^{-q/2}$. Đặt $\Gamma_Q = j(\Gamma)$, ta có

$$
\mathcal{F}\Gamma_Q = (\mathcal{F}\Gamma) \circ {}^t j = \exp(-q \circ {}^t j/2) = e^{-Q/2}
$$

theo công thức (4) của No. 3.

C) *Trường hợp tổng quát.*
Cho $V \in \mathcal{F}(E)$. Ký hiệu $p_V$ là ánh xạ chính tắc của $E$ lên $E/V$, và $Q_V$ là dạng toàn phương dương $Q \circ {}^t p_V$ trên $(E/V)'$; sau cùng, gọi $\mu_V$ là độ đo trên $E/V$ có biến đổi Fourier $e^{-Q_V/2}$ (xem B)). Nếu $W \in \mathcal{F}(E)$ được chứa trong $V$, thì $p_V = p_{VW} \circ p_W$, do đó $Q_V = Q_W \circ {}^t p_{VW}$; theo công thức (4) của No. 3, độ đo $p_{VW}(\mu_W)$ có biến đổi Fourier là hàm $(e^{-Q_W/2}) \circ {}^t p_{VW} = e^{-Q_V/2}$, nên bằng $\mu_V$. Vì vậy họ $(\mu_V)_{V \in \mathcal{F}(E)}$ là một tiền độ đo $\mu$ trên E. Công thức (5) của No. 3 cho thấy rằng $\mathcal{F}\mu$ bằng $e^{-Q/2}$.

#### Định nghĩa 2 {#int-ix-s6-def-2 .statement}

*Cho $E$ là một không gian vectơ tôpô lồi. Với mọi dạng bậc hai dương $Q$ trên $E'$, tiền đo trên $E$ có biến đổi Fourier bằng $e^{-Q/2}$ được gọi là tiền đo Gauss trên $E$ với phương sai $Q$, và được ký hiệu $\Gamma_Q$. Một tiền đo $\mu$ trên $E$ được gọi là Gauss nếu tồn tại một dạng bậc hai dương $Q$ trên $E'$ sao cho $\mu = \Gamma_Q$.*

Theo lối nói mở rộng, một độ đo bị chặn $\mu$ trên $E$ sẽ được gọi là Gauss với phương sai $Q$ nếu tiền đo liên kết $\widetilde{\mu}$ bằng $\Gamma_Q$.

#### Nhận xét {#int-ix-s6-n5-rem-1 .statement}

— 1) Cho $E$ là một không gian vectơ hữu hạn chiều, và cho $\mu$ là một độ đo dương trên $E$ có khối lượng 1, sao cho mọi dạng tuyến tính trên $E$ đều thuộc $\mathcal{L}^2(E, \mu)$. Người ta xác định một phần tử $m$ của $E$ và một dạng bậc hai dương $V$ trên $E'$ bởi các công thức
$$
\langle m, x' \rangle = \int_E \langle x, x' \rangle d\mu(x), \quad V(x') = \int_E \langle x - m, x' \rangle^2 d\mu(x).
$$
Theo thuật ngữ truyền thống của Lý thuyết Xác suất, $m$ được gọi là *trung bình* và $V$ là *phương sai* của $\mu$; $\mu$ được gọi là *có tâm* nếu $m = 0$.

Bây giờ cho $a$ là một phần tử của $E$ và $Q$ là một dạng bậc hai dương trên $E'$. Ký hiệu $\Gamma_{a,Q}$ là ảnh của độ đo $\Gamma_Q$ qua phép tịnh tiến $x \mapsto x + a$. Dễ thấy rằng $\Gamma_{a,Q}$ là một độ đo dương trên $E$ có khối lượng 1, với biến đổi Fourier $x' \mapsto e^{i\langle a, x' \rangle - \frac{1}{2} Q(x')}$ và trung bình là $a$. Hơn nữa, Mệnh đề 6 dưới đây suy ra rằng $Q$ là phương sai của $\Gamma_{a,Q}$. Theo truyền thống, người ta nói rằng $\Gamma_{a,Q}$ là độ đo Gauss có trung bình $a$ và phương sai $Q$, và rằng $\Gamma_Q = \Gamma_{0,Q}$ là độ đo Gauss *có tâm* với phương sai $Q$. Vì chúng ta sẽ chỉ xét các độ đo Gauss *có tâm*, nên ta sẽ bỏ qua định ngữ này.

2) Cho $Q$ là một dạng toàn phương trên đối ngẫu $E'$ của một không gian lồi địa phương $E$. Nếu tồn tại một tiền độ đo trên $E$ có biến đổi Fourier là $e^{-Q/2}$, thì dạng toàn phương $Q$ tất yếu là dương: vì hàm $e^{-Q/2}$ bị chặn trên $E'$; do đó, với mọi $x' \in E'$, hàm $t \mapsto e^{-t^2 Q(x')/2} = e^{-Q(tx')/2}$ trên $\mathbf{R}$ bị chặn, suy ra $Q(x') \geq 0$.

3) Đối ngẫu của $\mathbf{R}$ đẳng cấu chính tắc với $\mathbf{R}$ và các dạng toàn phương dương trên $\mathbf{R}$ là các hàm có dạng $t \mapsto at^2$ với $a \geq 0$. Vì vậy, với mọi $a \geq 0$ tồn tại duy nhất một độ đo bị chặn $\gamma_a$ trên $\mathbf{R}$ có biến đổi Fourier bằng hàm $t \mapsto e^{-at^2/2}$; theo lối nói lỏng, $\gamma_a$ được gọi là *độ đo Gaussian trên $\mathbf{R}$ với phương sai $a$*.

Biến đổi Fourier của $\gamma_0$ là hằng 1, suy ra $\gamma_0 = \varepsilon_0$ (khối lượng đơn vị tại gốc của $\mathbf{R}$). Giả sử $a > 0$ và ký hiệu $u_a$ là ánh xạ tuyến tính $x \mapsto a^{1/2} x$; khi đó $\mathcal{F}\gamma_a = \mathcal{F}\gamma_1 \circ {}^t u_a$, suy ra $\gamma_a = u_a(\gamma_1)$. Bổ đề 2 cho thấy $\gamma_1$ là độ đo có mật độ $x \mapsto (2\pi)^{-1/2} e^{-x^2/2}$ đối với độ đo Lebesgue; từ đó, ta dễ dàng suy ra

$$
(15) \quad d\gamma_a(x) = (2\pi a)^{-1/2} e^{-x^2/2a} dx .
$$

Ảnh của một tiền độ đo Gaussian dưới một ánh xạ tuyến tính liên tục là một tiền độ đo Gaussian. Chính xác hơn, ta có kết quả sau:

#### Mệnh đề 5 {#int-ix-s6-prop-5 .statement}

*Cho E và E₁ là hai không gian lồi địa phương, và u là một ánh xạ tuyến tính liên tục từ E vào E₁. Cho Q là một dạng toàn phương dương trên E', và Q₁ là dạng toàn phương dương Q $\circ {}^t u$ trên E'₁. Khi đó $u(\Gamma_Q) = \Gamma_{Q_1}$.*

Đặt $\mu = u(\Gamma_Q)$. Theo công thức (4) của No. 3,

$$
\mathcal{F}\mu = (\mathcal{F}\Gamma_Q) \circ {}^t u = e^{-Q/2} \circ {}^t u = e^{-Q_1/2} = \mathcal{F}\Gamma_{Q_1} ,
$$

suy ra $\mu = \Gamma_{Q_1}$ theo Mệnh đề 3 của No. 3.

#### Hệ quả {#int-ix-s6-n5-cor-1 .statement}

*Cho E là một không gian lồi địa phương và Q là một dạng toàn phương dương trên E'. Với mọi $x' \in E'$, ảnh của $\Gamma_Q$ qua $x'$ là độ đo Gaussian trên $\mathbf{R}$ với phương sai $Q(x')$.*

#### Mệnh đề 6 {#int-ix-s6-prop-6 .statement}

*Cho E là một không gian lồi địa phương, và $\mu$ là một độ đo Gaussian trên E, với phương sai Q. Với mọi số nguyên $n \geq 0$ và mọi $x' \in E'$, ta có các hệ thức*

$$
\begin{align*}
(16) & \quad \int_E |\langle x, x' \rangle|^n d\mu(x) = \pi^{-1/2} 2^{n/2} \Gamma\left( \frac{n+1}{2} \right) Q(x')^{n/2} \\
(17) & \quad \int_E \langle x, x' \rangle^{2n} d\mu(x) = \frac{(2n)!}{2^n n!} Q(x')^n \\
(18) & \quad \int_E \langle x, x' \rangle^{2n+1} d\mu(x) = 0 .
\end{align*}
$$

*Đặc biệt,*

$$
(19) \quad \int_E \langle x, x' \rangle^2 d\mu(x) = Q(x') \qquad (x' \in E') .
$$

Nếu các công thức này đúng với một phần tử $x'$ của E', thì chúng cũng đúng với mọi bội $t \cdot x'$ của nó (với $t$ thực). Vì vậy, ta chỉ cần chứng minh chúng trong trường hợp $Q(x')$ bằng 0 hoặc 1.

a) Giả sử $Q(x') = 0$. Độ đo $x'(\mu)$ bằng $\gamma_0 = \varepsilon_0$, do đó $x'$ bằng không $\mu$-hầu khắp nơi; các công thức (16) đến (19) khi đó hiển nhiên.

b) Giả sử $Q(x') = 1$, do đó $x'(\mu) = \gamma_1$. Khi đó
$$
\int_E |\langle x, x' \rangle|^n d\mu(x) = \int_{\mathbf{R}} |t|^n d\gamma_1(t) = (2\pi)^{-1/2} \int_{\mathbf{R}} |t|^n e^{-t^2/2} dt
$$
và (16) suy ra ngay lập tức từ (6) (No 4, Bổ đề 1). Tương tự, các công thức (17) và (18) suy ra từ (7) và (8). Cuối cùng, (19) thu được bằng cách đặt $n = 1$ trong (17).

Bây giờ ta có thể chứng minh một mệnh đề đảo của Hệ quả của Mệnh đề 5.

#### Mệnh đề 7 {#int-ix-s6-prop-7 .statement}

*Cho E là một không gian lồi địa phương và $\mu$ là một promeasure trên E. Giả sử rằng $x'(\mu)$ là một độ đo Gaussian trên $\mathbf{R}$ với mọi $x' \in E'$. Khi đó $\mu$ là một promeasure Gaussian trên E.*

Với mọi $x' \in E'$, ký hiệu $Q(x')$ là phương sai của độ đo Gaussian $x'(\mu)$ trên $\mathbf{R}$. Ta có $x'(\mu) = \gamma_{Q(x')}$, do đó
$$
(\mathcal{F}\mu)(x') = \int_{\mathbf{R}} e^{it \cdot 1} d\gamma_{Q(x')}(t) = e^{-Q(x') \cdot 1^2 / 2}
$$
theo định nghĩa của $\mathcal{F}\mu$ (No. 3, công thức (2)). Nói cách khác, $\mathcal{F}\mu = e^{-Q/2}$, và còn lại phải chứng minh rằng $Q$ là một dạng toàn phương dương trên $E'$.

Với mỗi không gian con tuyến tính đóng V của E có đối chiều hữu hạn, ký hiệu $p_V$ là ánh xạ chính tắc của E lên $E/V$, ký hiệu $\mu_V$ là độ đo $p_V(\mu)$ trên $E/V$, và đặt $Q_V = Q \circ {}^t p_V$. Vì $E' = \bigcup_{V \in \mathcal{F}(E)} \operatorname{Im}({}^t p_V)$ và ${}^t p_V$ đơn ánh, chỉ cần chứng minh rằng $Q_V$ là một dạng toàn phương dương trên $(E/V)'$. Cho $u \in (E/V)'$ và $x' = {}^t p_V(u)$. Ta có
$$
u(\mu_V) = u(p_V(\mu)) = x'(\mu) = \gamma_{Q(x')} ;
$$
Mệnh đề 6 suy ra
$$
Q_V(u) = Q(x') = \int_{\mathbf{R}} t^2 d\gamma_{Q(x')}(t) = \int_{E/V} u(x)^2 d\mu_V(x),
$$
do đó $Q_V$ là một dạng toàn phương dương trên $(E/V)'$.

### 6. Các ví dụ về các promeasure Gaussian

1) Cho E là một không gian Hilbert thực. Ánh xạ $x' \mapsto \|x'\|^2$ là một dạng toàn phương dương trên $E'$. Promeasure Gaussian tương ứng được gọi là *promeasure Gaussian chính tắc* trên E. Có thể chứng minh rằng promeasure này không phải là một độ đo nếu E vô hạn chiều.

Cho $A$ là một toán tử tuyến tính liên tục trên E. Ánh xạ $x' \mapsto \|{}^tA \cdot x'\|^2$ là một dạng toàn phương dương trên $E'$. Promeasure tương ứng $\mu_A$ trên E là một độ đo khi và chỉ khi $A$ là một toán tử Hilbert–Schmidt (xem No. 11, Hệ quả 2 của ĐL 3).

2) *Nhân của kiểu dương.* Cho $T$ là một tập hợp và $E = \mathbf{R}^T$ là không gian vectơ các hàm thực trên $T$, được trang bị tôpô hội tụ điểm. Với mỗi $t \in T$, ký hiệu $\varepsilon_t$ là dạng tuyến tính $f \mapsto f(t)$ trên E. Họ $(\varepsilon_t)_{t \in T}$ là một cơ sở của $E'$ (TVS, II, §6, No. 6, Hệ quả 2 của Mệnh đề 8).

Người ta gọi hạt nhân (thực) kiểu dương trên $T$ là mọi hàm nhận giá trị thực $K$ trên $T \times T$ thỏa mãn các hệ thức

$$
\text{(20)} \qquad K(t, t') = K(t', t) \quad \text{với } t, t' \text{ trong } T,
$$
$$
\text{(21)} \qquad \sum_{i,j=1}^p c_i c_j K(t_i, t_j) \geqslant 0
$$

với mọi số nguyên dương $p$, các phần tử $t_1, \ldots, t_p$ của $T$, và các số thực $c_1, \ldots, c_p$. Nếu vậy, công thức

$$
\text{(22)} \qquad q\left( \sum_{t \in T} c_t \varepsilon_t \right) = \sum_{t,t' \in T} c_t c_{t'} K(t, t')
$$

xác định một dạng toàn phương dương trên $E'$. Ngược lại, nếu $q$ là một dạng toàn phương dương trên $E'$, thì công thức

$$
\text{(23)} \qquad K(t, t') = \frac{1}{2} [q(\varepsilon_t + \varepsilon_{t'}) - q(\varepsilon_t) - q(\varepsilon_{t'})]
$$

xác định một hạt nhân $K$ kiểu dương trên $T$. Như vậy ta thu được hai song ánh ngược nhau giữa tập hợp các hạt nhân kiểu dương trên $T$, và tập hợp các dạng toàn phương dương trên $E'$.

Cho $K$ là một hạt nhân kiểu dương trên $T$, và $q$ là dạng toàn phương liên kết trên $E'$. Tiền độ đo Gauss trên $E$ với phương sai $q$ cũng còn được gọi là *tiền độ đo Gauss trên $E$ với hiệp phương sai* $K$. Nếu $T$ đếm được, Mệnh đề 2 của No. 1 suy ra tiền độ đo này là một độ đo.

3) Cho $T$ là một tập hợp đếm được. Một hạt nhân $\delta$ trên $T$ kiểu dương được định nghĩa bằng cách đặt

$$
\text{(24)} \qquad \delta(t, t') = \begin{cases}
1 & \text{nếu } t = t' \\
0 & \text{nếu } t \neq t'.
\end{cases}
$$

Dạng toàn phương tương ứng được cho bởi $q\left( \sum_{t \in T} c_t \varepsilon_t \right) = \sum_{t \in T} c_t^2$. Với mọi $t \in T$, ký hiệu $\mu_t$ là độ đo Gauss trên $\mathbf{R}$ có phương sai 1;

ta dễ dàng thấy rằng độ đo Gauss trên $\mathbf{R}^T$ với hiệp phương sai $\delta$ bằng $\bigotimes_{t \in T} \mu_t$.

4) Cho $n \geq 1$ là một số nguyên. Một ma trận vuông $C = (c_{ij})$ cấp $n$ được gọi là *đối xứng dương* nếu nó đối xứng và $\sum_{i,j=1}^n c_{ij} x_i x_j \geq 0$ với mọi $x_1, \ldots, x_n$ thực; điều đó cũng tương đương với việc nói rằng ánh xạ $(i, j) \mapsto c_{ij}$ là một hạt nhân kiểu dương trên tập hợp $\{1, 2, \ldots, n\}$. Vì vậy ta có thể nói về độ đo Gauss $\gamma_C$ trên $\mathbf{R}^n$, với hiệp phương sai $C$; nó được đặc trưng bởi công thức

$$
(25) \quad \int_{\mathbf{R}^n} e^{i(x_1 t_1 + \cdots + x_n t_n)} d\gamma_C(t_1, \ldots, t_n) = \exp \left( - \frac{1}{2} \sum_{j,k=1}^n c_{jk} x_j x_k \right),
$$

với $x_1, \ldots, x_n$ thực. Từ Mệnh đề 6 của No. 5 (công thức (19)), suy ra

$$
(26) \quad \int_{\mathbf{R}^n} t_j t_k d\gamma_C(t_1, \ldots, t_n) = c_{jk} \quad (1 \leq j, k \leq n).
$$

Từ Mệnh đề 5 của No. 5, suy ra công thức

$$
(27) \quad u(\gamma_C) = \gamma_{UC^t U},
$$

trong đó $u$ là một ánh xạ tuyến tính từ $\mathbf{R}^n$ vào $\mathbf{R}^m$ có ma trận $U$. Hơn nữa, ta dễ dàng thấy (xem phần đầu của chứng minh Mệnh đề 4 của No. 5) rằng nếu $I_n$ là ma trận đơn vị cấp $n$, thì độ đo $\gamma_{I_n}$ có mật độ

$$
(2\pi)^{-n/2} \exp \left( - \frac{1}{2}(t_1^2 + \cdots + t_n^2) \right)
$$

đối với độ đo Lebesgue $\lambda_n$ trên $\mathbf{R}^n$.

Ta sẽ chứng minh rằng nếu ma trận $C$ khả nghịch, với nghịch đảo $D = (d_{jk})$, thì

$$
(28) \quad d\gamma_C(t_1, \ldots, t_n) =
(2\pi)^{-n/2} (\det D)^{1/2} \left( \exp \left( - \frac{1}{2} \sum_{j,k=1}^n d_{jk} t_j t_k \right) \right) dt_1 \cdots dt_n.
$$

Thật vậy, nếu $C$ khả nghịch, thì dạng toàn phương $q$ trên $\mathbf{R}^n$ được xác định bởi

$$
q(x_1, \ldots, x_n) = \sum_{j,k=1}^n c_{jk} x_j x_k
$$

là không suy biến. Dùng sự tồn tại của một cơ sở của $\mathbf{R}^n$ trực chuẩn đối với $q$, ta chứng minh được sự tồn tại của một ma trận vuông $U$ cấp $n$ sao cho $C = U \cdot {}^tU$, do đó $\gamma_C = u(\gamma_{I_n})$ theo (27) (trong đó $u$ ký hiệu tự đẳng cấu của $\mathbf{R}^n$ có ma trận $U$). Ký hiệu $Q$ là dạng toàn phương trên $\mathbf{R}^n$ được xác định bởi
$$
Q(t_1, \ldots, t_n) = t_1^2 + \cdots + t_n^2;
$$
khi đó
$$
\gamma_{I_n} = (2\pi)^{-n/2} e^{-Q/2} \cdot \lambda_n,
$$
do đó
$$
u(\gamma_{I_n}) = (2\pi)^{-n/2} e^{-(Qou^{-1})/2} \cdot u(\lambda_n).
$$
Hiển nhiên rằng dạng toàn phương $Q \circ u^{-1}$ trên $\mathbf{R}^n$ nhận giá trị $\sum_{j,k=1}^n d_{jk} t_j t_k$ tại điểm $(t_1, \ldots, t_n)$, và Mệnh đề 15 của Ch. VII, §1, No. 10 cho thấy rằng
$$
u(\lambda_n) = (\det U)^{-1} \cdot \lambda_n = (\det D)^{1/2} \cdot \lambda_n.
$$
Công thức (28) suy ra từ đây.

### 7. Độ đo Wiener

Trong mục này, ta ký hiệu $T$ là khoảng $]0, 1]$ của $\mathbf{R}$ và $\mathcal{H}$ là không gian Hilbert của các hàm thực trên $T$ khả tích bình phương đối với độ đo Lebesgue, trong đó tích vô hướng được ký hiệu bởi $(f|g)$. Ta cũng ký hiệu $\mathcal{C}$ là không gian các hàm thực liên tục trên $T$ tiến tới 0 tại điểm 0; ta trang bị cho $\mathcal{C}$ chuẩn $\|f\| = \sup_{t \in T} |f(t)|$. Khoảng compact $[0, 1] = T \cup \{0\}$ là compact hóa Alexandroff của khoảng địa phương compact nhưng không compact $T$; do đó, tập các hàm liên tục trên $T$ có giá compact là trù mật trong $\mathcal{C}$, và đối ngẫu của $\mathcal{C}$ có thể được đồng nhất với không gian $\mathcal{M}^1$ gồm các độ đo bị chặn (không nhất thiết dương) trên $T$ (Ch. III, §1, No. 8, Def. 3).

Với mỗi hàm $f \in \mathcal{H}$, ta định nghĩa một hàm $Pf$ trên $T$ bởi
$$
(Pf)(t) = \int_0^t f(x) \, dx = (f|I_t),
$$
trong đó $I_t$ là hàm đặc trưng của khoảng $]0, t]$. Bất đẳng thức Cauchy–Schwarz suy ra các bất đẳng thức
$$
|(Pf)(t)| \leq \|f\|_2 \cdot t^{1/2}
$$
$$
|(Pf)(t) - (Pf)(t')| \leq \|f\|_2 \cdot |t - t'|^{1/2};
$$

do đó, $Pf$ thuộc $\mathcal{C}$, và ánh xạ tuyến tính $P$ của $\mathcal{H}$ vào $\mathcal{C}$ là liên tục với chuẩn $\leqslant 1$.

Chúng ta đồng nhất không gian Hilbert $\mathcal{H}$ với đối ngẫu của nó (TVS, V, §1, No. 7, Th. 3), và ký hiệu $\Pi : \mathcal{M}^1 \to \mathcal{H}$ là chuyển vị của $P : \mathcal{H} \to \mathcal{C}$. Với mọi độ đo $\mu \in \mathcal{M}^1$ và mọi hàm $f \in \mathcal{H}$, ta có

$$
(\Pi \mu | f) = \mu(Pf) = \int_{\mathbf{T}} d\mu(t) \int_{\mathbf{T}} I_t(x) f(x) \, dx
$$
$$
= \int_{\mathbf{T}} f(x) \, dx \int_{\mathbf{T}} I_t(x) \, d\mu(t)
$$

theo định lý Lebesgue–Fubini. Bây giờ,

$$
I_t(x) = \begin{cases}
1 & \text{nếu } 0 < x \leq t \leq 1 \\
0 & \text{khác},
\end{cases}
$$

do đó cuối cùng

(34) $$ (\Pi \mu)(x) = \mu([x, 1]) \quad \text{với } x \in \mathbf{T}. $$

Cho $\mu, \nu$ thuộc $\mathcal{M}^1$. Khi đó

$$
(\Pi \mu | \Pi \nu) = \int_{\mathbf{T}} \Pi \mu(x) \Pi \nu(x) \, dx = \int_{\mathbf{T}} dx \int_{\mathbf{T}} I_t(x) \, d\mu(t) \int_{\mathbf{T}} I_{t'}(x) \, d\nu(t')
$$
$$
= \int_{\mathbf{T}} \int_{\mathbf{T}} d\mu(t) \, d\nu(t') \int_{\mathbf{T}} I_t(x) I_{t'}(x) \, dx.
$$

Bây giờ, $I_t \cdot I_{t'}$ là hàm đặc trưng của khoảng $]0, t] \cap ]0, t']$, do đó ngay lập tức

(35) $$ \int_{\mathbf{T}} I_t(x) I_{t'}(x) \, dx = \inf(t, t'). $$

Suy ra rằng

(36) $$ (\Pi \mu | \Pi \nu) = \int_{\mathbf{T}} \int_{\mathbf{T}} \inf(t, t') \, d\mu(t) \, d\nu(t'). $$

Theo kết quả trên, ta định nghĩa một dạng toàn phương dương $W$ trên $\mathcal{M}^1$ bằng công thức

(37) $$ W(\mu) = \int_{\mathbf{T}} \int_{\mathbf{T}} \inf(t, t') \, d\mu(t) \, d\mu(t') = \| \Pi \mu \|_2^2. $$

Đặc biệt, nếu $t_1, \ldots, t_n$ là các phần tử của T, và $c_1, \ldots, c_n$ là các số thực, thì
$$
W \left( \sum_{j=1}^n c_j \varepsilon_{t_j} \right) = \sum_{j,k=1}^n c_j c_k \inf(t_j, t_k)
$$
và vì W là dương, hàm $(t, t') \mapsto \inf(t, t')$ là một hạt nhân kiểu dương trên T.

**ĐỊNH LÝ 1 (Wiener).** — *Cho w là ảnh dưới $P : \mathcal{H} \to \mathcal{C}$ của tiền độ đo Gaussian chính tắc trên không gian Hilbert $\mathcal{H}$. Khi đó w là một độ đo Gaussian trên $\mathcal{C}$ với phương sai W.*

Theo phép dựng, $W(\mu) = \|^tP(\mu)\|_2^2$; Mệnh đề 5 của No. 5 cho thấy w là một tiền độ đo Gaussian với phương sai W. Còn lại phải chứng minh rằng w là một độ đo trên $\mathcal{C}$.

A) *Phép dựng một không gian có độ đo phụ trợ*^{(2)} $(\Omega, m)$:
Với mọi số nguyên $n \geqslant 0$, ký hiệu $D_n$ là tập hợp các số có dạng $k/2^n$ với $k = 1, 2, 3, \ldots, 2^n$. Đặt $D = \bigcup_{n \geqslant 0} D_n$ (tập hợp các số dyadic được chứa trong T) và $\Omega = \mathbf{R}^D$. Với mọi $t \in D$, ký hiệu $X(t)$ là dạng tuyến tính $f \mapsto f(t)$ trên $\Omega$.

Với $t, t'$ trong D, đặt $M(t, t') = \inf(t, t')$; ta đã thấy rằng M là một hạt nhân kiểu dương trên D. Vì tập D là đếm được, người ta có thể định nghĩa độ đo Gaussian *m* trên $\Omega$ với hiệp phương sai M (No. 6, *Ví dụ 2*).

#### Bổ đề 3 {#int-ix-s6-lem-3 .statement}

*Với mọi $t, t'$ trong D,
$$
\int_\Omega \left| X\left( \frac{t + t'}{2} \right) - \frac{X(t) + X(t')}{2} \right|^3 dm = \frac{1}{(8\pi)^{1/2}} |t - t'|^{3/2}.
$$
Chú ý rằng $\frac{t + t'}{2}$ thuộc D. Ta biết (No. 6, *Ví dụ 2*) rằng họ $(X(t))_{t \in D}$ là một cơ sở của đối ngẫu tôpô $\Omega'$ của $\Omega$; do đó tồn tại một dạng song tuyến tính đối xứng $\widehat{M}$ trên $\Omega' \times \Omega'$ được đặc trưng bởi $\widehat{M}(X(t), X(t')) = \inf(t, t')$. Theo phép dựng, phương sai của độ đo Gaussian m trên $\Omega$ là dạng toàn phương $\xi \mapsto \widehat{M}(\xi, \xi)$ trên $\Omega'$. Đặt, cụ thể,
$$
\xi = X\left( \frac{t + t'}{2} \right) - \frac{X(t) + X(t')}{2};
$$
một phép tính dễ dàng cho ta
$$
\widehat{M}(\xi, \xi) = \frac{|t - t'|}{4}.
$$

(2) *Espace mesuré*: một không gian compact địa phương được trang bị một độ đo (Ch. III, 1st edn., §2, No. 2, p. 52).

Theo Mệnh đề 6 của No. 5 (công thức (16)),

$$
\int_{\Omega} |\xi|^3 \, dm = \pi^{-1/2} 2^{3/2} \Gamma(2) \widehat{M}(\xi, \xi)^{3/2};
$$

bổ đề suy ra ngay lập tức từ các công thức (40) và (41).

B) *Phép dựng một ánh xạ u từ $\Omega$ vào $\mathcal{C}$:*
Với mọi số nguyên $n \geqslant 0$, ký hiệu $E_n$ là không gian con của $\mathcal{C}$ gồm các hàm afin trên từng khoảng $\left[ \frac{k-1}{2^n}, \frac{k}{2^n} \right]$ với $1 \leqslant k \leqslant 2^n$. Một hàm afin trên một khoảng compact I của $\mathbf{R}$ đạt các cận của nó tại các đầu mút của I; do đó,

$$
\|f\| = \sup_{1 \leqslant k \leqslant 2^n} \left| f\left( \frac{k}{2^n} \right) \right|
$$

với $f \in E_n$.

Với mọi hàm $g \in \Omega$ và mọi số nguyên $n \geqslant 0$, tồn tại một và chỉ một hàm $u_n(g)$ thuộc $E_n$ và trùng với $g$ tại mọi điểm của $D_n$; ta sẽ viết $T_n g = u_{n+1}(g) - u_n(g)$. Vì $D_n$ hữu hạn, ánh xạ $T_n$ của $\Omega$ vào $\mathcal{C}$ liên tục, do đó $m$-đo được.

#### Bổ đề 4 {#int-ix-s6-lem-4 .statement}

— *Với mọi số nguyên $n \geqslant 0$,*

$$
\int_{\Omega} \|T_n g\|^3 \, dm(g) \leqslant \frac{1}{(8\pi)^{1/2}} 2^{-n/2}.
$$

Cho $g \in \Omega$ và $n \in \mathbf{N}$. Ta có $E_n \subset E_{n+1}$; do đó, hàm $T_n g$ thuộc $E_{n+1}$ và bằng không tại mọi điểm của $D_n$; vì vậy, theo (42),

$$
\|T_n g\|^3 = \sup_{1 \leqslant k \leqslant 2^n} \left| T_n g\left( \frac{2k-1}{2^{n+1}} \right) \right|^3 \leqslant \sum_{k=1}^{2^n} \left| T_n g\left( \frac{2k-1}{2^{n+1}} \right) \right|^3.
$$

Quy ước $g(0) = 0$. Phép nội suy tuyến tính của $g$ để dựng $u_n(g)$ cho ta các hệ thức

$$
T_n g\left( \frac{2k-1}{2^{n+1}} \right) = g\left( \frac{2k-1}{2^{n+1}} \right) - \frac{1}{2} \left( g\left( \frac{k-1}{2^n} \right) + g\left( \frac{k}{2^n} \right) \right)
$$

với $1 \leqslant k \leqslant 2^n$. Từ đó, bằng phép tích phân, suy ra

$$
\int_{\Omega} \left| T_n g\left( \frac{2k-1}{2^{n+1}} \right) \right|^3 \, dm(g) = \int_{\Omega} \left| X\left( \frac{2k-1}{2^{n+1}} \right) - \frac{1}{2} \left( X\left( \frac{k-1}{2^n} \right) + X\left( \frac{k}{2^n} \right) \right) \right|^3 \, dm;
$$

![Hình 1](../images/figure_1.png)

HÌNH 1

khi đó có thể áp dụng Bổ đề 3 với $t = \frac{k-1}{2^n}$, $t' = \frac{k}{2^n}$, suy ra

$$
\int_{\Omega} \left| T_n g \left( \frac{2k-1}{2^{n+1}} \right) \right|^3 dm(g) = \frac{1}{(8\pi)^{1/2}} 2^{-\frac{3n}{2}} .
$$

Từ (44), ta có

$$
\int_{\Omega} \| T_n g \|^3 dm(g) \leq \sum_{k=1}^{2^n} \int_{\Omega} \left| T_n g \left( \frac{2k-1}{2^{n+1}} \right) \right|^3 dm(g) = \frac{1}{(8\pi)^{1/2}} 2^n \cdot 2^{-\frac{3n}{2}} ,
$$

suy ra bổ đề.

Theo Bổ đề 4, ánh xạ $T_n$ của $\Omega$ vào không gian Banach $\mathcal{C}$ thuộc $L^3_{\mathcal{C}}(\Omega, m)$ và $N_3(T_n) \leq \frac{1}{(8\pi)^{1/6}} (2^{-1/6})^n$, do đó $\sum_{n=0}^{\infty} N_3(T_n) < +\infty$. Theo Mệnh đề 6 của Ch. IV, §3, No. 3, tồn tại một tập $\Omega_0 \subset \Omega$ sao cho $\Omega - \Omega_0$ là $m$-không đáng kể và sao cho chuỗi $\sum_{n=0}^{\infty} T_n(g)$ hội tụ tuyệt đối trong $\mathcal{C}$ với mọi $g \in \Omega_0$. Khi đó ta định nghĩa một ánh xạ $m$-đo được $u$ từ $\Omega$ vào $\mathcal{C}$ bởi

$$
u(g) = \begin{cases}
\sum_{n=0}^{\infty} T_n g = \lim_{n \to \infty} u_n(g) & \text{nếu } g \in \Omega_0 \\
0 & \text{nếu } g \in \Omega - \Omega_0 .
\end{cases}
$$

Vì $u_n(g)$ và $g$ trùng nhau trên $D_m \subset D_n$ với $0 \leq m \leq n$, nên ngay lập tức suy ra rằng hạn chế của $u(g)$ lên $D$ bằng $g$ với mọi $g \in \Omega_0$.

C) Phép dựng một độ đo Gaussian trên $\mathcal{C}$:
Cho $w'$ là độ đo bị chặn trên $\mathcal{C}$ là ảnh của $m$ qua ánh xạ $m$-đo được $u : \Omega \to \mathcal{C}$. Ta sẽ chứng minh rằng $w'$ là một độ đo Gaussian trên $\mathcal{C}$, với phương sai $W$, do đó $w = w'$. Kí hiệu $\mathcal{D}$ là không gian con tuyến tính của $\mathcal{M}^1$ sinh bởi các độ đo $\varepsilon_t$ khi $t$ chạy qua $D$.

#### Bổ đề 5 {#int-ix-s6-lem-5 .statement}

Với mọi độ đo $\mu \in \mathcal{D}$,

$$
\int_{\mathcal{C}} e^{i \langle f, \mu \rangle} \, dw'(f) = e^{-W(\mu)/2}.
$$

Đặt $\mu = c_1 \varepsilon_{t_1} + c_2 \varepsilon_{t_2} + \cdots + c_n \varepsilon_{t_n}$ với $t_1, \ldots, t_n$ trong $D$ và $c_1, \ldots, c_n$ trong $\mathbf{R}$. Với mọi $g \in \Omega_0$, hàm $u(g)$ trùng với $g$ trên $D$; do đó

$$
\langle u(g), \mu \rangle = \sum_{j=1}^n c_j g(t_j) \qquad (g \in \Omega_0).
$$

Mặt khác,

$$
W(\mu) = \sum_{j,k=1}^n c_j c_k \inf(t_j, t_k),
$$

và, vì $m$ là độ đo Gaussian trên $\Omega$ với hiệp phương sai $M$, và $\Omega - \Omega_0$ là $m$-không đáng kể, ta có

$$
\int_{\Omega_0} e^{i \sum_{j=1}^n c_j g(t_j)} \, dm(g) = \exp \left( - \frac{1}{2} \sum_{j,k=1}^n c_j c_k \inf(t_j, t_k) \right).
$$

Bây giờ, $\Omega - \Omega_0$ là $m$-không đáng kể và $w' = u(m)$; suy ra rằng

$$
\int_{\mathcal{C}} e^{i \langle f, \mu \rangle} \, dw'(f) = \int_{\Omega_0} e^{i \langle u(g), \mu \rangle} \, dm(g).
$$

Công thức (48) suy ra ngay lập tức từ các công thức (49) đến (52).

#### Bổ đề 6 {#int-ix-s6-lem-6 .statement}

Cho $\mu \in \mathcal{M}^1$. Tồn tại một dãy các độ đo $\mu_n \in \mathcal{D}$ sao cho $\mu(f) = \lim_{n \to \infty} \mu_n(f)$ với mọi $f \in \mathcal{C}$ và $W(\mu) = \lim_{n \to \infty} W(\mu_n)$.

Đặt $I = [0, 1]$. Không gian $\mathcal{M}^1$ của các độ đo bị chặn trên $T = ]0, 1[$ sẽ được đồng nhất với không gian con của $\mathcal{M}(I)$ gồm các độ đo không đặt trọng số tại $0$. (3) Ta trang bị cho $\mathcal{M}(I)$ tôpô mơ hồ. Ánh xạ

(3) Tức là, các độ đo trên $I$ tập trung trên $T = I - \{0\}$.

Ánh xạ $t \mapsto \varepsilon_t$ từ $I$ vào $\mathcal{M}(I)$ là liên tục (Ch. III, §1, No. 9, Mệnh đề 13); vì D trù mật trong I, bao đóng $\overline{\mathcal{D}}$ của $\mathcal{D}$ chứa tất cả các độ đo điểm. Đặt A là tập các độ đo $\nu \in \mathcal{D}$ sao cho $\| \nu \| \leq \| \mu \|$; độ đo $\mu$ nằm trong bao đóng của A (Ch. III, §2, No. 4, Hệ quả 1 của Định lý 1). Tập A tương đối compact trong $\mathcal{M}(I)$ (Ch. III, §1, No. 9, Mệnh đề 15) và các tập con compact của $\mathcal{M}(I)$ đều khả metric (TVS, III, §3, No. 4, Hệ quả 2 của Mệnh đề 6,(4) và GT, X, §3, No. 3, Định lý 1). Vì thế tồn tại một dãy độ đo $\mu_n \in A$ hội tụ đến $\mu$ trong $\mathcal{M}(I)$. Vì $\mathcal{C}$ được đồng nhất với không gian con các hàm liên tục trên I bằng không tại gốc, ta có $\mu(f) = \lim_{n \to \infty} \mu_n(f)$ với mọi $f \in \mathcal{C}$. Hơn nữa, vì $\mathcal{C}(I) \otimes \mathcal{C}(I)$ trù mật trong không gian chuẩn $\mathcal{C}(I \times I)$ (Ch. III, §4, No. 1, Bổ đề 1), các quan hệ $\lim_{n \to \infty} \mu_n = \mu$ và $\| \mu_n \| \leq \| \mu \|$ suy ra $\lim_{n \to \infty} (\mu_n \otimes \mu_n) = \mu \otimes \mu$ (Ch. III, §1, No. 10, Mệnh đề 17); vì các độ đo $\mu_n$ và $\mu$ không đặt trọng số tại 0, ta có

$$
W(\mu_n) = \int_I \int_I \inf(t, t') d\mu_n(t) d\mu_n(t'),
$$
$$
W(\mu) = \int_I \int_I \inf(t, t') d\mu(t) d\mu(t'),
$$

do đó $\lim_{n \to \infty} W(\mu_n) = W(\mu)$.

Còn phải chứng minh rằng biến đổi Fourier của $w'$ bằng $e^{-W/2}$. Cho $\mu \in \mathcal{M}^1$; chọn các độ đo $\mu_n \in \mathcal{D}$ như trong Bổ đề 6. Độ đo $w'$ bị chặn, và $|e^{i \langle f, \mu_n \rangle}| = 1$ với mọi $n$; Bổ đề 5 và định lý hội tụ của Lebesgue (Ch. IV, §4, No. 3, Định lý 2) suy ra

$$
\int_{\mathcal{C}} e^{i \langle f, \mu \rangle} dw'(f) = \lim_{n \to \infty} \int_{\mathcal{C}} e^{i \langle f, \mu_n \rangle} dw'(f)
= \lim_{n \to \infty} e^{-W(\mu_n)/2} = e^{-W(\mu)/2}.
$$

Q.E.D.

Độ đo $w$ trên $\mathcal{C}$ có biến đổi Fourier bằng $e^{-W/2}$ được gọi là *độ đo Wiener trên $\mathcal{C}$*.

#### Nhận xét {#int-ix-s6-n7-rem-1 .statement}

— Với mọi khoảng nửa mở $J = ]a, b]$ được chứa trong T, ta đặt $l(J) = b - a$ (độ dài của J) và ký hiệu $A_J$ là dạng tuyến tính $f \mapsto f(b) - f(a)$ trên $\mathcal{C}$. Có thể chứng minh rằng độ đo Wiener được đặc trưng bởi tính chất sau:

*Cho $J_1, \ldots, J_n$ là các khoảng nửa mở được chứa trong T và rời nhau từng đôi một. Ảnh của độ đo w qua ánh xạ tuyến tính $f \mapsto (A_{J_1}(f), \ldots, A_{J_n}(f))$ từ $\mathcal{C}$ vào $\mathbf{R}^n$ bằng $\gamma_{a_1} \otimes \cdots \otimes \gamma_{a_n}$ với $a_i = l(J_i)^{1/2}$ cho $1 \leq i \leq n$.*

### 8. Tính liên tục của biến đổi Fourier

#### Mệnh đề 8 {#int-ix-s6-prop-8 .statement}

— Cho E là một không gian lồi địa phương, $\mu$ là một tiền độ đo trên E, và $\Phi$ là biến đổi Fourier của $\mu$. Ta có các bất đẳng thức

$$
|\Phi(x')| \leq \Phi(0)
$$
$$
|\Phi(x') - \Phi(y')|^2 \leq 2\Phi(0)\left(\Phi(0) - \Re \Phi(x' - y')\right)
$$

với $x', y'$ trong $E'$.

Công thức (5) của No. 3 cho phép rút về trường hợp E hữu hạn chiều và $\mu$ là một độ đo. Khi đó

$$
|\Phi(x')| = \left| \int_E e^{i\langle x, x' \rangle} d\mu(x) \right| \leq \int_E |e^{i\langle x, x' \rangle}| d\mu(x) = \int_E d\mu(x) = \Phi(0),
$$

do đó (53). Hơn nữa, nếu $a$ và $b$ là các số thực, thì

$$
|e^{ia} - e^{ib}|^2 = |e^{ib}|^2|e^{i(a-b)} - 1|^2 = (e^{i(a-b)} - 1)(e^{-i(a-b)} - 1) = 2 - 2\cos(a - b);
$$

theo bất đẳng thức Cauchy–Schwarz, ta có

$$
|\Phi(x') - \Phi(y')|^2 = \left| \int_E (e^{i\langle x, x' \rangle} - e^{i\langle x, y' \rangle}) d\mu(x) \right|^2
$$
$$
\leq \int_E |e^{i\langle x, x' \rangle} - e^{i\langle x, y' \rangle}|^2 d\mu(x) \int_E 1^2 d\mu(x)
$$
$$
= \int_E (2 - 2\cos\langle x, x' - y' \rangle)) d\mu(x) \cdot \Phi(0)
$$
$$
= 2\Phi(0)\left(\Phi(0) - \Re \Phi(x' - y')\right),
$$

do đó (54).

#### Hệ quả {#int-ix-s6-n8-cor-1 .statement}

— Trang bị cho $E'$ một tôpô tương thích với cấu trúc không gian vectơ của nó. Để $\Phi$ liên tục, điều kiện cần và đủ là phần thực $\Re \Phi$ của nó liên tục tại gốc, khi đó $\Phi$ liên tục đều.

Điều này suy ra từ bất đẳng thức (54).

Cho F là một không gian lồi địa phương. Ta trang bị cho đối ngẫu $F'$ của F một tôpô tương thích với tính đối ngẫu giữa F và $F'$, và đồng nhất F với đối ngẫu của $F'$. Do đó, biến đổi Fourier của một độ đo bị chặn $\mu$ trên $F'$ là hàm $\mathcal{F}\mu$ trên F được xác định bởi

$$
(\mathcal{F}\mu)(x) = \int_{F'} e^{i\langle x, x' \rangle} d\mu(x').
$$

#### Mệnh đề 9 {#int-ix-s6-prop-9 .statement}

— *Nếu F là barreled, thì biến đổi Fourier của mọi độ đo bị chặn trên F' là một hàm liên tục đều trên F*.

Cho $\mu$ là một độ đo bị chặn trên $F'$ và $\Phi$ là biến đổi Fourier của nó. Cho $\varepsilon > 0$. Tồn tại một tập con compact K của $F'$ sao cho $\mu(F' - K) \leq \varepsilon$. Bây giờ, K là compact đối với tôpô yếu $\sigma(F', F)$, do đó là đều liên tục vì F là barreled (TVS, III, §4, No. 2, Định lý 1). Vì thế tồn tại một lân cận đối xứng U của 0 trong F sao cho cực $U^\circ$ chứa K. Lấy x thuộc $\varepsilon U$; khi đó

$$
\Phi(0) - \Re \Phi(x) = \int_{F'} (1 - \cos \langle x, x' \rangle) d\mu(x').
$$

Khi đó, $0 \leq 1 - \cos \langle x, x' \rangle \leq 2$ với mọi $x' \in F' - K$, và

$$
1 - \cos \langle x, x' \rangle \leq \frac{1}{2} \langle x, x' \rangle^2 \leq \frac{\varepsilon^2}{2}
$$

với $x' \in K \subset U^\circ$; suy ra rằng

$$
0 \leq \Phi(0) - \Re \Phi(x) \leq 2 \mu(F' - K) + \frac{\varepsilon^2}{2} \mu(K) \leq 2\varepsilon + \frac{\varepsilon^2}{2} \mu(F').
$$

Vế thứ hai của bất đẳng thức này tiến tới 0 khi $\varepsilon$ tiến tới 0; do đó $\Re \Phi$ liên tục tại 0 và mệnh đề suy ra từ Hệ quả của Mệnh đề 8.

### 9. Bổ đề Minlos

Cho T là một không gian vectơ hữu hạn chiều và $\mu$ là một độ đo bị chặn trên $T'$; ta sẽ đồng nhất T với đối ngẫu của $T'$, sao cho biến đổi Fourier $\Phi$ của $\mu$ là một hàm trên T. Giả sử cho trước hai dạng toàn phương dương h và q trên T và một số $\varepsilon > 0$. Với mọi số thực $r > 0$, ta ký hiệu $C_r$ là tập hợp các $x' \in T'$ sao cho $\langle x, x' \rangle^2 \leq r^2 h(x)$ với mọi $x \in T$.

#### Mệnh đề 10 {#int-ix-s6-prop-10 .statement}

— *Dưới giả thiết $\Phi(0) - \Re \Phi \leq \varepsilon + q$, ta có*

$$
\mu(T' - C_r) \leq 3 (\varepsilon + r^{-2} \operatorname{Tr}(q/h))
$$

*với mọi* $r > 0$.

Ta viết $\operatorname{Tr}(q/h)$ để chỉ vết của q theo h (xem Phụ lục, No. 1). Công thức (55) là tầm thường khi $\operatorname{Tr}(q/h)$ vô hạn. Từ đây trở đi, ta giả sử rằng $\operatorname{Tr}(q/h)$ là hữu hạn, do đó $h(x) = 0$ kéo theo $q(x) = 0$ với $x \in T$.

Cho $a_1, \ldots, a_n$ là các phần tử của $T$, và $D$ là tập hợp các $x' \in T'$ sao cho $\sum_{j=1}^n \langle a_j, x' \rangle^2 > 1$. Với mọi số thực $t \geq 0$ ta có $3(1 - e^{-t/2}) \geq 0$, và thậm chí ta có

$$
3(1 - e^{-t/2}) \geq 3(1 - e^{-1/2}) \geq 3\left(1 - \left(\frac{9}{4}\right)^{-1/2}\right) = 1
$$

với $t > 1$, vì $e > \frac{9}{4}$. Áp dụng các bất đẳng thức này cho $t = \sum_{j=1}^n \langle a_j, x' \rangle^2$, ta thu được

$$
\mu(D) \leq 3 \int_{T'} \left(1 - \exp \left(-\frac{1}{2} \sum_{j=1}^n \langle a_j, x' \rangle^2\right)\right) d\mu(x').
$$

Đặt $\gamma$ là độ đo trên $\mathbf{R}$ có mật độ $t \mapsto (2\pi)^{-1/2} e^{-t^2/2}$ đối với độ đo Lebesgue. Theo Bổ đề 2 của No. 4,

$$
\int_{\mathbf{R}} e^{iut} d\gamma(t) = e^{-u^2/2}
$$

với mọi số thực $u$. Do đó,

$$
\begin{align*}
1 - \exp \left(-\frac{1}{2} \sum_{j=1}^n \langle a_j, x' \rangle^2\right) \\
&= \int \cdots \int \left(1 - e^{i \sum_{j=1}^n \langle a_j, x' \rangle t_j}\right) d\gamma(t_1) \cdots d\gamma(t_n)
\end{align*}
$$

với mọi $x' \in T'$. Hàm theo $x', t_1, \ldots, t_n$ được lấy tích phân ở vế thứ hai là liên tục và bị chặn về trị tuyệt đối bởi 2, và các độ đo $\mu$ và $\gamma$ đều bị chặn; do đó có thể lấy tích phân hai vế của (57) theo $d\mu(x')$ và hoán đổi các phép lấy tích phân theo $\mu$ và $\gamma$; ta thu được

$$
\begin{align*}
\int_{T'} \left(1 - \exp \left(-\frac{1}{2} \sum_{j=1}^n \langle a_j, x' \rangle^2\right)\right) d\mu(x') \\
&= \int \cdots \int \left(\Phi(0) - \Phi\left(\sum_{j=1}^n t_j a_j\right)\right) d\gamma(t_1) \cdots d\gamma(t_n).
\end{align*}
$$

Vì $q$ là một dạng toàn phương trên $T$, tồn tại các số thực $q_{jk}$ sao cho
$$
q \left( \sum_{j=1}^n t_j a_j \right) = \sum_{j,k} q_{jk} t_j t_k
$$
với $t_1, \ldots, t_n$ thực; đặc biệt, $q_{jj} = q(a_j)$ với $1 \leq j \leq n$. Hơn nữa, tích phân $\int_{\mathbf{R}} t^n d\gamma(t)$ nhận các giá trị 1, 0, 1 cho $n = 0, 1, 2$, tương ứng (No. 4, Bổ đề 1). Từ đó, suy ra ngay lập tức
$$
\int \cdots \int \left( \varepsilon + q \left( \sum_{j=1}^n t_j a_j \right) \right) d\gamma(t_1) \ldots d\gamma(t_n) = \varepsilon + \sum_{j=1}^n q(a_j).
$$
Bây giờ, vế thứ nhất của (58) và $\Phi(0)$ là các số thực; do đó có thể thay $\Phi$ bằng $\Re \Phi$ ở vế thứ hai của (58). Bất đẳng thức $\Phi(0) - \Re \Phi \leq \varepsilon + q$ và các công thức (56), (58) và (59) khi đó suy ra
$$
\mu(D) \leq 3 \left( \varepsilon + \sum_{j=1}^n q(a_j) \right).
$$
Cố định số $r > 0$. Vì dạng toàn phương $h$ là dương, tồn tại một cơ sở $(e_1, \ldots, e_n)$ của $T$ và một số nguyên m giữa 0 và n sao cho
$$
h \left( \sum_{j=1}^n t_j e_j \right) = \sum_{j=1}^m t_j^2
$$
với $t_1, \ldots, t_n$ thực (Phụ lục, No. 1, Mệnh đề 2). Khi đó ngay lập tức $C_r$ gồm các $x' \in T'$ sao cho
$$
\sum_{j=1}^m \langle e_j, x' \rangle^2 \leq r^2, \qquad \sum_{j=m+1}^n \langle e_j, x' \rangle^2 = 0.
$$
Với mỗi số nguyên $l \geq 1$, đặt $D_l$ là tập hợp các $x' \in T'$ thỏa mãn bất đẳng thức
$$
\sum_{j=1}^m \langle r^{-1} e_j, x' \rangle^2 + \sum_{j=m+1}^n \langle l e_j, x' \rangle^2 > 1.
$$
Dễ dàng thấy rằng dãy $(D_l)_{l \geq 1}$ là tăng với hợp $T' - C_r$, do đó
$$
\mu(T' - C_r) = \lim_{l \to \infty} \mu(D_l).
$$

Nhưng theo (60),

$$
\mu(D_l) \leq 3 \left( \varepsilon + \sum_{j=1}^m r^{-2} q(e_j) + \sum_{j=m+1}^n l^2 q(e_j) \right);
$$

for $j = m+1, \ldots, n$ we have $h(e_j) = 0$, do đó $q(e_j) = 0$. Hơn nữa, $\operatorname{Tr}(q/h) = \sum_{j=1}^m q(e_j)$ (Phụ lục, No. 1, Mệnh đề 2). Quan hệ (55) khi đó suy ra từ (61) và (62).

Q.E.D.

### 10. Các độ đo trên đối ngẫu của một không gian hạt nhân

Cho F là một không gian lồi địa phương. Cho $\mathcal{T}_s$ là tôpô yếu $\sigma(F', F)$ trên $F'$, và $\mathcal{T}_c$ là tôpô của sự hội tụ đều trên các tập con lồi compact của F. Theo định lý của Mackey (TVS, IV, §1, No. 1, Định lý 1) các tôpô $\mathcal{T}_s$ và $\mathcal{T}_c$ trên $F'$ tương thích với đối ngẫu giữa F và $F'$; do đó điều đó cũng đúng với mọi tôpô lồi địa phương $\mathcal{T}$ trên $F'$ trung gian giữa $\mathcal{T}_s$ và $\mathcal{T}_c$. Nếu $\mathcal{T}$ là một tôpô như thế, và $F'_{\mathcal{T}}$ ký hiệu không gian $F'$ được trang bị $\mathcal{T}$, ta sẽ đồng nhất F với không gian đối ngẫu của $F'_{\mathcal{T}}$. Vì thế các tiền độ đo trên $F'$ là như nhau đối với mọi tôpô $\mathcal{T}$ thuộc kiểu nói trên, và nếu $\mu$ là một tiền độ đo như thế thì biến đổi Fourier của nó là một hàm trên F.

Ta gọi tôpô của Sazonov trên F là tôpô lồi địa phương $\mathcal{S}$ được xác định bởi các nửa chuẩn liên tục N thỏa mãn điều kiện sau: $N^2$ là một dạng toàn phương dương trên F và tồn tại một dạng toàn phương dương liên tục H trên F sao cho $\operatorname{Tr}(N^2/H) < +\infty$. Tôpô $\mathcal{S}$ thô hơn tôpô đã cho trên F; nếu hai tôpô này đồng nhất, F được gọi là một không gian hạt nhân. Lớp các không gian này sẽ được khảo sát chi tiết về sau.

#### Định lý 2 (Minlos) {#int-ix-s6-thm-2 .statement}

— *Cho F là một không gian lồi địa phương, $\mathcal{T}$ là một tôpô lồi địa phương trên $F'$ trung gian giữa $\mathcal{T}_s$ và $\mathcal{T}_c$, và $\mu$ là một tiền độ đo trên $F'_{\mathcal{T}}$. Giả sử rằng biến đổi Fourier $\Phi$ của $\mu$ liên tục trên F đối với tôpô của Sazonov. Khi đó $\mu$ là một độ đo trên $F'_{\mathcal{T}}$.*

Cho $\varepsilon > 0$. Vì $\Phi$ liên tục đối với tôpô của Sazonov trên F, nên tồn tại hai dạng toàn phương dương liên tục Q và H trên F sao cho $\operatorname{Tr}(Q/H) < +\infty$ và

$$
\Phi(0) - \mathcal{R}\Phi(x) \leq \varepsilon/6
$$

với mọi $x \in F$ sao cho $Q(x) \leq 1$. Theo Mệnh đề 8 của No. 8, $|\mathcal{R}\Phi(x)| \leq \Phi(0)$ với mọi $x \in F$, do đó

$$
\Phi(0) - \mathcal{R}\Phi(x) \leq \varepsilon/6 + 2\Phi(0)Q(x)
$$

với mọi $x \in F$.

Đặt $r = (12\Phi(0)\operatorname{Tr}(Q/H)\varepsilon^{-1})^{1/2}$ và ký hiệu K là tập hợp các $x' \in F'_\mathcal{T}$ sao cho $\langle x, x' \rangle^2 \leq r^2 H(x)$ với mọi $x \in F$. Vì $H^{1/2}$ là một nửa chuẩn liên tục trên $F$, nên tập hợp K là đều liên tục và đóng trong $F'_\mathcal{T}$; do đó nó compact trong $F'_\mathcal{T}$ theo định lý Ascoli (GT, X, §2, No. 5, Hệ quả 1 của Định lý 2).

Cho V là một không gian con tuyến tính đóng của $F'_\mathcal{T}$ với đối chiều hữu hạn; khi đó, V là phần trực giao của một không gian con tuyến tính hữu hạn chiều T của F. Cho $\mu_V$ là độ đo trên $T'$ là ảnh của tiền độ đo $\mu$ trên $F'_\mathcal{T}$ qua ánh xạ $p_V$ là chuyển vị của đơn ánh chính tắc của T vào F; biến đổi Fourier của nó là sự hạn chế của $\Phi$ lên T. Cuối cùng, theo định lý Hahn–Banach (TVS, II, §3, No. 2, Hệ quả 1 của Định lý 1), $p_V(K)$ bằng tập hợp $C_r$ của các $x' \in T'$ sao cho $\langle x, x' \rangle^2 \leq r^2 H(x)$ với mọi $x \in T$. Theo bất đẳng thức (63), ta có thể áp dụng Mệnh đề 10 của No. 9 cho độ đo $\mu_V$ trên $T'$, khi lấy q là sự hạn chế của $2\Phi(0)Q$ lên T và h là của H. Khi đó, $\operatorname{Tr}(q/h) \leq 2\Phi(0)\operatorname{Tr}Q/H)$, do đó

$$
\mu_V(T' - C_r) \leq 3 \left( \frac{\varepsilon}{6} + 2\Phi(0)\operatorname{Tr}(Q/H)\,r^{-2} \right) = \varepsilon.
$$

Vì $p_V$, qua phép đi qua thương, xác định một đẳng cấu của $F'_\mathcal{T}/V$ lên $T'$, Mệnh đề 1 của No. 1 suy ra rằng $\mu$ là một độ đo trên $F'_\mathcal{T}$.

Q.E.D.

#### Hệ quả {#int-ix-s6-n10-cor-1 .statement}

— *Cho F là một không gian barreled hạt nhân, $\mathcal{T}$ là một tôpô lồi địa phương trên $F'$ trung gian giữa $\mathcal{T}_s$ và $\mathcal{T}_c$, $\mu$ là một tiền độ đo trên $F'_\mathcal{T}$, và $\Phi$ là biến đổi Fourier của $\mu$. Để $\mu$ là một độ đo, điều kiện cần và đủ là $\Phi$ liên tục trên F.*

Điều kiện cần suy ra từ Mệnh đề 9 của No. 8 và điều kiện đủ từ Định lý 2.

#### Nhận xét {#int-ix-s6-n10-rem-1 .statement}

— Cho F là một không gian barreled và $\mathcal{T}$ là một tôpô lồi địa phương trên $F'$ trung gian giữa $\mathcal{T}_s$ và $\mathcal{T}_c$. Mọi tập con của $F'$ compact đối với $\mathcal{T}$ đều compact đối với tôpô yếu hơn $\mathcal{T}_s$. Ngược lại, cho K là một tập con của $F'$ compact đối với $\mathcal{T}_s$. Vì F là barreled, K là đều liên tục (TVS, III, §4, No. 2, Định lý 1); nhưng theo định lý Ascoli, mọi tập con đều liên tục của $F'$ đều tương đối compact đối với $\mathcal{T}_c$ và *a fortiori* đối với $\mathcal{T}$, do đó K được chứa trong một tập con của $F'$ compact đối với $\mathcal{T}$. Không khó suy ra từ đó rằng ánh xạ đồng nhất của $F'_\mathcal{T}$ lên $F'_{\mathcal{T}_s}$ xác định một song ánh giữa các tập hợp các độ đo trên hai không gian này.

### 11. Các độ đo trên một không gian Hilbert

Cho E là một không gian Hilbert thực, trong đó tích vô hướng được ký hiệu bởi $(x|y)$. Tồn tại một đẳng cấu j của E lên đối ngẫu $E'$, được đặc trưng bởi công thức $\langle x, j(y) \rangle = (x|y)$ với $x, y$ trong E (TVS, V, §1, No. 7, Định lý 3). Ta sẽ đồng nhất E và $E'$ nhờ j. Vì thế biến đổi Fourier của một tiền độ đo $\mu$ trên E là một hàm $\mathscr{F}\mu$ trên E; khi $\mu$ là một độ đo, ta có

$$(64)$$
$$(\mathcal{F}\mu)(x) = \int_{E} e^{i(x|y)} d\mu(y) \quad (x \in E).$$

**Định lý 3** (Prokhorov–Sazonov) — *Cho E là một không gian Hilbert và Es là không gian E được trang bị tôpô yếu hơn. Cho μ là một tiền độ đo trên E, và Φ là biến đổi Fourier của nó. Các điều kiện sau là tương đương*:

a) *Hàm Φ liên tục trên E theo tôpô Sazonov*.

b) *Với mọi ε > 0, tồn tại một dạng toàn phương dương hạt nhân Q trên E sao cho Φ(0) − $\Re \Phi$ ≤ ε + Q*.

c) *Tiền độ đo μ là một độ đo trên Es*.

$b) \Rightarrow a)$: Điều này suy ra từ Mệnh đề 8 của No. 8 (xem bất đẳng thức (54)).

$a) \Rightarrow c)$: Điều này suy ra từ Định lý 2 của No. 10.

$c) \Rightarrow b)$: Giả sử rằng μ là một độ đo trên Es. Cho ε > 0. Với mọi số nguyên $n \geq 1$, tập $B_n$ của các $x \in E$ có chuẩn $\leq n$ là một tập con đóng của $E_s$, và $E = \bigcup_{n \geq 1} B_n$. Do đó tồn tại một số nguyên $n \geq 1$ sao cho $\mu(E - B_n) < \frac{\varepsilon}{2}$. Công thức

$$(65)$$
$$ Q(x) = \frac{1}{2} \int_{B_n} (x|y)^2 d\mu(y) $$

định nghĩa một dạng toàn phương dương Q trên E. Đặt $C = \frac{n^2}{2} \mu(B_n)$. Nếu $(e_1, \ldots, e_p)$ là một dãy trực chuẩn hữu hạn trong E, thì

$$
\sum_{j=1}^p (e_j|y)^2 \leq \|y\|^2 \leq n^2
$$

với mọi $y \in B_n$ theo bất đẳng thức Bessel. Suy ra bằng cách lấy tích phân rằng

$$
\sum_{j=1}^p Q(e_j) = \frac{1}{2} \int_{B_n} \sum_{j=1}^p (e_j|y)^2 d\mu(y) \leq \frac{n^2}{2} \mu(B_n) = C,
$$

do đó Q là hạt nhân.

Hơn nữa, $1 - \cos t \leq \inf \left( 2, \frac{t^2}{2} \right)$ với mọi số thực t, do đó

$$
\Phi(0) - \Re \Phi(x) = \int_{E} (1 - \cos(x|y)) d\mu(y)
$$
$$
\leq \int_{B_n} \frac{1}{2}(x|y)^2 d\mu(y) + \int_{E - B_n} 2 \cdot d\mu(y)
$$
$$
< Q(x) + \varepsilon
$$

với mọi $x \in E$. Vậy b) được xác minh.

Q.E.D.

#### Hệ quả 1 {#int-ix-s6-thm-2-cor-1 .statement}

— *Cho $E_1$ và $E_2$ là hai không gian Hilbert, $u$ là một ánh xạ Hilbert–Schmidt của $E_1$ vào $E_2$, và $\mu$ là một tiền độ đo trên $E_1$. Giả sử rằng biến đổi Fourier $\Phi$ của $\mu$ liên tục trên $E_1$. Khi đó tiền độ đo $\nu = u(\mu)$ là một độ đo trên $E_2$ được trang bị tôpô yếu.*

Với các đồng nhất hóa của $E_1$ và $E_2$ với các đối ngẫu của chúng đã được đưa vào trong mục này, biến đổi Fourier của $\nu$ bằng $\Phi \circ u^*$, trong đó u^* là toán tử liên hợp của u. Mà, $u^*$ là một ánh xạ Hilbert–Schmidt của $E_2$ vào $E_1$ (Phụ lục, No. 2), và do đó dạng toàn phương $y \mapsto \|u^*(y)\|^2$ trên $E_2$ là hạt nhân. Nếu $(E_2)_\mathscr{S}$ ký hiệu $E_2$ được trang bị tôpô Sazonov, thì do đó $u^*$ là một ánh xạ tuyến tính liên tục từ $(E_2)_\mathscr{S}$ vào $E_1$, và $\mathcal{F}_V = \Phi \circ u^*$ liên tục trên $(E_2)_\mathscr{S}$; Định lý 3 suy ra rằng \nu là một độ đo trên không gian $E_2$ được trang bị tôpô yếu.

#### Hệ quả 2 {#int-ix-s6-thm-2-cor-2 .statement}

— *Cho $Q$ là một dạng toàn phương dương hạt nhân trên không gian Hilbert $E$. Tiền độ đo Gauss $\Gamma_Q$ trên $E$ với phương sai $Q$ là một độ đo trên $E_s$.*

Biến đổi Fourier $\Phi$ của $\Gamma_Q$ bằng $e^{-Q/2}$. Mặt khác, $e^t \geq 1 + t$ với mọi số thực $t$, do đó $\Phi(0) - \Re \Phi \leq Q/2$. Vì vậy điều kiện b) của Định lý 3 được thỏa mãn và $\Gamma_Q$ là một độ đo trên $E_s$.

#### Nhận xét {#int-ix-s6-n11-rem-1 .statement}

— 1) Cho $E$ là một không gian Hilbert, $E_s$ là không gian $E$ được trang bị tôpô yếu, và $j$ là ánh xạ đồng nhất của $E$ vào $E_s$. Ta biết rằng $j$ xác định một song ánh của tập hợp các tiền độ đo trên $E$ lên tập hợp tương ứng cho $E_s$. Hơn nữa, nếu $E$ tách được thì $E$ là một không gian Polish và $j$ xác định một song ánh của tập hợp các độ đo bị chặn trên $E$ lên tập hợp các độ đo bị chặn trên $E_s$ (\S 3, No. 3, *Nhận xét*); có thể chứng minh (định lý của Phillips) rằng định lý này vẫn đúng nếu $E$ không tách được. Do đó, Định lý 3 cung cấp các tiêu chuẩn để một tiền độ đo trên $E$ là một độ đo.

2) Có thể chứng minh (Phụ lục, Bài tập 7) rằng tôpô Sazonov trên một không gian Hilbert $E$ được xác định bởi các nửa chuẩn kiểu $Q^{1/2}$ trong đó $Q$ là một dạng toàn phương dương *hạt nhân* trên $E$.

*12. Liên hệ với các hàm có kiểu dương*

#### Định nghĩa 3 {#int-ix-s6-def-3 .statement}

— *Cho $G$ là một nhóm. Một hàm giá trị phức $\Phi$ trên $G$ được gọi là có kiểu dương nếu bất đẳng thức*

$$
\sum_{j,k=1}^p c_j \overline{c_k} \Phi(x_j x_k^{-1}) \geq 0
$$

*đúng với mọi* $x_1, \ldots, x_p$ *trong* $G$ *và mọi số phức* $c_1, \ldots, c_p$.

Khái niệm này sẽ được khảo sát chi tiết về sau.

#### Mệnh đề 11 {#int-ix-s6-prop-11 .statement}

— Cho $E$ là một không gian vectơ hữu hạn chiều, $\mu$ là một độ đo bị chặn (dương) trên $E$, và $\Phi$ là biến đổi Fourier của $\mu$. Hàm $\Phi$ liên tục và có kiểu dương trên $E'$.

Tính liên tục của $\Phi$ suy ra từ Mệnh đề 9 của No. 8.

Hãy chứng minh rằng $\Phi$ có kiểu dương. Cho $x'_1, \ldots, x'_p$ thuộc $E'$ và $c_1, \ldots, c_p$ là các số phức. Khi đó

$$
\sum_{j,k} c_j \overline{c_k} \Phi(x'_j - x'_k) = \int_E \sum_{j,k} c_j \overline{c_k} e^{i \langle x, x'_j - x'_k \rangle} \, d\mu(x)
$$
$$
= \int_E \left| \sum_{j=1}^p c_j e^{i \langle x, x'_j \rangle} \right|^2 \, d\mu(x) \geq 0.
$$

ĐPCM.

Có thể chứng minh một đảo lại được gọi là *định lý Bochner*: mọi hàm liên tục trên $E'$ có kiểu dương đều là biến đổi Fourier của một độ đo bị chặn (dương). (*) Chúng ta sẽ giả sử kết quả này trong phần còn lại của No. 12.

#### Định lý 4 {#int-ix-s6-thm-4 .statement}

— Cho $E$ là một không gian lồi địa phương. Biến đổi Fourier là một song ánh của tập hợp các tiền độ đo trên $E$ lên tập hợp các hàm có kiểu dương trên $E'$ mà hạn chế của nó lên mọi không gian con hữu hạn chiều là liên tục.

Ta biết (No. 3, Mệnh đề 3) rằng biến đổi Fourier là đơn ánh. Cho $\mu = (\mu_V)_{V \in \mathcal{F}(E)}$ là một tiền đo trên E và $\Phi$ là biến đổi Fourier của nó. Cho T là một không gian con hữu hạn chiều của $E'$ và cho V là trực giao của T trong E. Có thể đồng nhất T với đối ngẫu của $E/V$; hạn chế $\Phi_T$ của $\Phi$ lên T là biến đổi Fourier của độ đo bị chặn $\mu_V$ trên $E/V$. Theo Mệnh đề 11, $\Phi_T$ liên tục và có kiểu dương trên T. Vì T là tùy ý, rõ ràng $\Phi$ có kiểu dương trên $E'$.

Ngược lại, cho $\Phi$ là một hàm có kiểu dương trên $E'$ mà hạn chế của nó lên mọi không gian con hữu hạn chiều của $E'$ đều liên tục. Với mọi $V \in \mathcal{F}(E)$, ta đồng nhất đối ngẫu của $E/V$ với trực giao $V^\circ$ của V trong $E'$; hạn chế $\Phi_V$ của $\Phi$ lên $V^\circ$ là liên tục và có kiểu dương và do đó, theo định lý Bochner, tồn tại một độ đo bị chặn (dương) $\mu_V$ trên $E/V$ mà biến đổi Fourier của nó là $\Phi_V$. Cho V và W trong $\mathcal{F}(E)$ sao cho $W \subset V$, và cho $p_{VW}$ là ánh xạ chính tắc của $E/W$ lên $E/V$; với các đồng nhất đó, ${}^t p_{VW}$ là đơn ánh từ $V^\circ$ vào $W^\circ$. Theo công thức (4) của No. 3, ta có

$$
\mathcal{F}(p_{VW}(\mu_W)) = (\mathcal{F}\mu_W) \circ {}^t p_{VW} = \Phi_W \circ {}^t p_{VW} = \Phi_V = \mathcal{F}\mu_V,
$$

(*) Câu hỏi này sẽ được nghiên cứu trong một chương sắp tới của cuốn sách *Théories spectrales*. Độc giả có thể tham khảo về chủ đề này cuốn sách của L.H. LOOMIS, *Abstract harmonic analysis*, Van Nostrand, New York, 1953.

do đó $pvw(\mu_w) = \mu_v$ theo Mệnh đề 3 của No. 3. Do đó, họ $\mu = (\mu_v)_{v \in \mathscr{F}(E)}$ là một tiền đo trên E; rõ ràng $\Phi$ là biến đổi Fourier của $\mu$.

#### Hệ quả {#int-ix-s6-n11-cor-1 .statement}

— *Cho F là một không gian hạt nhân có lô-gic barreled; trang bị cho F' một tôpô tuyến tính địa phương trung gian giữa tôpô yếu $\sigma(F', F)$ và tôpô hội tụ đều trên các tập con lồi compact của F. Biến đổi Fourier là một song ánh của tập hợp các độ đo bị chặn (dương) trên F' lên tập hợp các hàm liên tục có kiểu dương trên F.*

Điều này suy ra ngay lập tức từ Định lý 4 và Hệ quả của Định lý 2 của No. 10.*

### Bài tập {#int-ix-s6-exercises}

Xem [các bài tập cho § 6](exercises/s6/).
