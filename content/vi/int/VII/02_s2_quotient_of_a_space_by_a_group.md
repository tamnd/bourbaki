---
book: int
book_title: Integration
chapter: VII
chapter_title: HAAR MEASURE
section: 2
section_title: Quotient of a space by a group; homogeneous spaces
lang: vi
source: int-vii-ix
book_pages: INT VII.27-INT VII.53, INT VII.87-INT VII.91
pdf_pages: 0033-0059, 0093-0097
extraction: ocr
subsections:
    - "no": 1
      title: General results
      page: 27
      pdf_page: 33
    - "no": 2
      title: The case $\chi = 1$
      page: 29
      pdf_page: 35
    - "no": 3
      title: Another interpretation of $\lambda^\#$
      page: 32
      pdf_page: 38
    - "no": 4
      title: The case that $X/H$ is paracompact
      page: 36
      pdf_page: 42
    - "no": 5
      title: Quasi-invariant measures on a homogeneous space
      page: 38
      pdf_page: 44
    - "no": 6
      title: Relatively invariant measures on a homogeneous space
      page: 43
      pdf_page: 49
    - "no": 7
      title: Haar measure on a quotient group
      page: 44
      pdf_page: 50
    - "no": 8
      title: A transitivity property
      page: 45
      pdf_page: 51
    - "no": 9
      title: Construction of the Haar measure of a group from the Haar measures of certain subgroups
      page: 48
      pdf_page: 54
    - "no": 10
      title: Integration on a fundamental domain
      page: 50
      pdf_page: 56
statements: 53
exercises: 13
content_sha256: 607f4b7bb4a870f343671558ebbfab770d216680894e15869cd7af1dc4cfe26c
translated_from: content/en/int/VII/02_s2_quotient_of_a_space_by_a_group.md
source_content_sha256: 808d1febed5e98d1a4693836305c73d1f084d7d8ef2e3631777c1dd0a2f4de4b
translation_model: gpt-5.4-mini, gpt-5-6-mini
translation_run: translate-vi-bacf869e
glossary_version: 34
glossary_terms_sha256: 8dcb1f3f9ae2aa4d2e680ac2ec23a30554259021e4344aeef7ef4cd1db2c9a93
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 2. THƯƠNG CỦA MỘT KHÔNG GIAN THEO MỘT NHÓM; CÁC KHÔNG GIAN THUẦN NHẤT

### 1. KẾT QUẢ CHUNG

Cho X là một không gian compact địa phương mà một nhóm compact địa phương H tác động bên phải, liên tục và chính quy, bởi $(x, \xi) \mapsto x\xi$ ($x \in X, \xi \in H$). Quan hệ tương đương trong X do H xác định là mở (GT, III, §2, No. 4, Bổ đề 2) và X/H là Hausdorff (*loc. cit.*, §4, No. 2, Mệnh đề 3) do đó compact địa phương (GT, I, §10, No. 4, Mệnh đề 10). Kí hiệu $\pi$ là ánh xạ chính tắc của X lên X/H. Phần bão hòa của một tập con Y của X là $YH = \pi^{-1}(\pi(Y))$. Nếu K là một tập con compact của X, thì $\pi(K)$ là compact và phần bão hòa $\pi^{-1}(\pi(K))$ của K là đóng trong X. Mỗi tập con compact của X/H là ảnh của một tập con compact của X qua $\pi$ (GT, I, §10, No. 4, Mệnh đề 10). *Ta cố định một độ đo Haar trái $\beta$ trên H*.

Cho $\chi$ là một biểu diễn liên tục của H trong $\mathbf{R}_+^*$. Nếu một hàm g trên X thỏa mãn $g(x\xi) = \chi(\xi)g(x)$ với mọi $x \in X$ và $\xi \in H$, thì giá đỡ S của nó là bất biến dưới H nên có thể viết $\pi^{-1}(\pi(S))$. Ta sẽ kí hiệu $\mathcal{K}^\chi(X)$ là không gian Riesz tạo bởi các hàm liên tục nhận giá trị thực g trên X thỏa mãn $g(x\xi) = \chi(\xi)g(x)$ ($x \in X, \xi \in H$) và có giá đỡ là phần bão hòa của một tập con compact của X; ta kí hiệu $\mathcal{K}_+^\chi(X)$ là tập các phần tử $\geqslant 0$ của $\mathcal{K}^\chi(X)$. Đặc biệt, $\mathcal{K}^1(X)$ chẳng qua là tập hợp các hàm liên tục trên X, hằng trên các quỹ đạo, có giá đỡ là phần bão hòa của một tập con compact.

#### Mệnh đề 1 {#int-vii-s2-prop-1 .statement}

*Cho f là một hàm liên tục nhận giá trị thực trên X mà giá đỡ S của nó có giao compact với phần bão hòa của mọi tập con compact của X.*

a) *Với mọi $x \in X$, hàm $\xi \mapsto f(x\xi)$ trên H thuộc $\mathcal{K}(H)$; ta đặt*

$$
f^\chi(x) = \int_H f(x\xi)\chi(\xi)^{-1}\, d\beta(\xi).
$$

b) *Hàm $f^\chi$ là liên tục, bằng không ngoài SH, và thỏa mãn $f^\chi(x\xi) = \chi(\xi)f^\chi(x)$.*

c) *Nếu g là một hàm liên tục nhận giá trị thực trên X và thỏa mãn $g(x\xi) = \chi(\xi)g(x)$, thì $(fg)^\chi = f^1g$ ($f^1$ được cho bởi công thức (1) với $\chi$ được thay bởi biểu diễn $\xi \mapsto 1$ của H trong $\mathbf{R}_+^*$).*

d) *Nếu* $\eta \in \mathbf{H}$, *thì* $(\delta(\eta)f)^{\chi} = \chi(\eta)\Delta_{\mathbf{H}}(\eta)^{-1}f^{\chi}$.

Cho $x_0 \in X$ và cho $V$ là một lân cận compact của $x_0$ trong X. Tập hợp các $\xi \in \mathbf{H}$ sao cho $V\xi$ giao với S cũng chính là tập hợp các $\xi \in \mathbf{H}$ sao cho $V\xi$ giao với $S \cap VH$, do đó compact trong $\mathbf{H}$ vì $S \cap VH$ là compact và $\mathbf{H}$ tác động chính quy trong X (GT, III, §4, No. 5, Th. 1); khi đó Bổ đề 1 của §1, No. 1 chứng minh a) và tính liên tục của $f^{\chi}$. Phần còn lại của b) hiển nhiên. Cuối cùng, c) và d) suy ra từ các phép tính sau:

$$
(fg)^{\chi}(x) = \int_{\mathbf{H}} f(x\xi)g(x\xi)\chi(\xi)^{-1}\,d\beta(\xi) = \int_{\mathbf{H}} f(x\xi)g(x)\chi(\xi)\chi(\xi)^{-1}\,d\beta(\xi)
$$
$$
= g(x) \int_{\mathbf{H}} f(x\xi)\,d\beta(\xi) = g(x)f^{1}(x)
$$

$$
(\delta(\eta)f)^{\chi}(x) = \int_{\mathbf{H}} f(x\xi\eta)\chi(\xi)^{-1}\,d\beta(\xi)
$$
$$
= \Delta_{\mathbf{H}}(\eta)^{-1} \int_{\mathbf{H}} f(x\xi)\chi(\xi\eta^{-1})^{-1}\,d\beta(\xi)
$$
$$
= \chi(\eta)\Delta_{\mathbf{H}}(\eta)^{-1} \int_{\mathbf{H}} f(x\xi)\chi(\xi)^{-1}\,d\beta(\xi).
$$

#### Mệnh đề 2 {#int-vii-s2-prop-2 .statement}

*Ánh xạ* $f \mapsto f^{\chi}$ *từ* $\mathcal{K}(X)$ *vào* $\mathcal{K}^{\chi}(X)$ *là tuyến tính, và ảnh của* $\mathcal{K}(X)$ *(resp. $\mathcal{K}_{+}(X)$) là* $\mathcal{K}^{\chi}(X)$ *(resp. $\mathcal{K}_{+}^{\chi}(X)$).*

Tính tuyến tính là hiển nhiên. Rõ ràng là $f^{\chi} \geqslant 0$ nếu $f \geqslant 0$. Khi đó chỉ cần áp dụng bổ đề sau:

#### Bổ đề 1 {#int-vii-s2-lem-1 .statement}

— *Cho* $K$ *là một tập con compact của* $X$, *u là một hàm của* $\mathcal{K}_{+}(X)$ *với* $u(x) > 0$ *với* $x \in K$. *Cho* $g \in \mathcal{K}^{\chi}(X)$ *sao cho* $\operatorname{Supp} g \subset KH$.
a) *Ta có* $\inf_{x \in KH} u^{1}(x) > 0$.
b) *Hàm* $h$ *bằng* $g/u^{1}$ *trên* $KH$, *và bằng* $0$ *trên* $X - KH$, *thuộc* $\mathcal{K}^{\chi}(X)$.
c) $g = (uh)^{\chi}$.
Ta có $u^{1}(x) > 0$ với $x \in K$, do đó $\inf_{x \in KH} u^{1}(x) = \inf_{x \in K} u^{1}(x) > 0$.
Mệnh đề b) suy ra ngay từ đó. Cuối cùng, $(uh)^{\chi} = u^{1}h$ theo Mệnh đề 1 c), và hiển nhiên là $u^{1}h = g$.

Cho I là một dạng tuyến tính tương đối bị chặn (Ch. II, §2, No. 2) trên $\mathcal{K}^{\chi}(X)$. Khi đó $f \mapsto I(f^{\chi})$ là một dạng tuyến tính tương đối bị chặn trên $\mathcal{K}(X)$, tức là một *độ đo* $\mu_{I}$ trên $X$. Ánh xạ $I \mapsto \mu_{I}$ là đơn ánh theo Mệnh đề 2. Các độ đo $\mu_{I}$ trên $X$ thu được như vậy có thể đặc trưng như sau:

#### Mệnh đề 3 {#int-vii-s2-prop-3 .statement}

*Cho* $\mu$ *là một độ đo trên* $X$. *Các điều kiện sau là tương đương:*

a) Tồn tại một dạng tuyến tính tương đối bị chặn I trên $\mathcal{K}^\chi(X)$ sao cho $I(f^\chi) = \mu(f)$ với mọi $f \in \mathcal{K}(X)$.
b) $\delta(\xi)\mu = \chi(\xi)^{-1} \Delta_H(\xi)\mu$ với mọi $\xi \in H$.
c) Với mọi $f, g$ trong $\mathcal{K}(X)$,

(2)
$$
\mu(f \cdot g^1) = \mu(f^\chi \cdot g) .
$$

d) Nếu $f \in \mathcal{K}(X)$ sao cho $f^\chi = 0$, thì $\mu(f) = 0$.

a) $\Rightarrow$ b): Nếu $\mu(f) = I(f^\chi)$ thì, xét đến Mệnh đề 1 d),

$$
\langle \delta(\xi)\mu, f \rangle = \langle \mu, \delta(\xi^{-1})f \rangle = I\left( (\delta(\xi^{-1})f)^\chi \right)
= I(\chi(\xi)^{-1} \Delta_H(\xi)f^\chi)
= \chi(\xi)^{-1} \Delta_H(\xi) \langle \mu, f \rangle ,
$$

do đó $\delta(\xi)\mu = \chi(\xi)^{-1} \Delta_H(\xi)\mu$.

b) $\Rightarrow$ c): Giả sử giả thiết b) được thỏa mãn. Chú ý rằng các hàm $(x, \xi) \mapsto f(x)g(x\xi)$ và $(x, \xi) \mapsto f(x\xi)g(x)$ trên $X \times H$ là liên tục và có giá compact (vì $H$ tác động đúng trên $X$); điều này đã được thiết lập, Định lý 2 của Ch. III, §4, No. 1 cho phép ta viết:

$$
\int_X f(x) d\mu(x) \int_H g(x\xi) d\beta(\xi) = \int_H d\beta(\xi) \int_X f(x)g(x\xi) d\mu(x)
= \int_H d\beta(\xi) \int_X f(x\xi^{-1})g(x)\chi(\xi)\Delta_H(\xi)^{-1} d\mu(x)
= \int_X g(x) d\mu(x) \int_H f(x\xi^{-1})\chi(\xi)\Delta_H(\xi)^{-1} d\beta(\xi)
= \int_X g(x) d\mu(x) \int_H f(x\xi)\chi(\xi)^{-1} d\beta(\xi),
$$

điều này chứng minh c).

c) $\Rightarrow$ d): Nếu c) được kiểm chứng và nếu $f^\chi = 0$, thì $\mu(f \cdot g^1) = 0$ với mọi $g \in \mathcal{K}(X)$, do đó $\mu(f) = 0$ bằng cách chọn $g \in \mathcal{K}(X)$ sao cho $g^1 = 1$ trên $\mathrm{Supp}\, f$ (điều này có thể thực hiện được nhờ Mệnh đề 2 áp dụng với $\chi = 1$).

d) $\Rightarrow$ a): Nếu điều kiện d) được thỏa mãn, tồn tại một dạng tuyến tính I trên $\mathcal{K}^\chi(X)$ sao cho $\mu(f) = I(f^\chi)$ với $f \in \mathcal{K}(X)$, và dạng này bị chặn tương đối nhờ Mệnh đề 2.

### 2. Trường hợp $\chi = 1$

Nếu $f$ là một hàm trên $X/H$, thì $f \circ \pi$ là một hàm trên $X$ hằng trên các quỹ đạo, liên tục khi và chỉ khi $f$ liên tục. Ánh xạ $f \mapsto f \circ \pi$ xác định đặc biệt một song ánh từ $\mathcal{K}(X/H)$ lên $\mathcal{K}^1(X)$.

Khi đó, trong trường hợp $\chi = 1$, ta có thể phát biểu lại một số kết quả của No. 1 theo cách sau:

Cho $f$ là một hàm số liên tục trên $X$ có giá đỡ giao với phần bão hòa của mỗi tập con compact của $X$ là compact. Công thức

$$
f^b(\pi(x)) = \int_H f(x\xi)\, d\beta(\xi)
$$

xác định một hàm liên tục $f^b$ trên $X/H$. Nếu $g$ là một hàm liên tục trên $X/H$, thì

$$
(f \cdot g \circ \pi)^b = f^b \cdot g .
$$

Nếu $\eta \in H$, thì

$$
(\delta(\eta)f)^b = \Delta_H(\eta)^{-1} f^b .
$$

Không được quên rằng định nghĩa của $f^b$ phụ thuộc vào lựa chọn của $\beta$. Nếu $H$ compact và $\beta$ được chuẩn hóa, hàm $f^b$ đôi khi được gọi là *trung bình quỹ đạo* của $f$.

Nếu $f \in \mathcal{K}(X)$, thì $f^b \in \mathcal{K}(X/H)$. Ánh xạ $f \mapsto f^b$ từ $\mathcal{K}(X)$ vào $\mathcal{K}(X/H)$ là tuyến tính, và ảnh của $\mathcal{K}(X)$ (tương ứng $\mathcal{K}_+(X)$) là $\mathcal{K}(X/H)$ (tương ứng $\mathcal{K}_+(X/H)$).

#### Nhận xét 1 {#int-vii-s2-n2-rem-1 .statement}

— Ta sẽ chứng minh rằng ánh xạ $f \mapsto f^b$ là một *cấu xạ ngặt* (GT, III, §2, No. 8) từ $\mathcal{K}(X)$ lên $\mathcal{K}(X/H)$.

a) Ánh xạ là liên tục: chỉ cần chứng minh rằng, với mọi tập con compact $K$ của $X$, hạn chế của $f \mapsto f^b$ vào $\mathcal{K}(X, K)$ là một ánh xạ liên tục của $\mathcal{K}(X, K)$ vào $\mathcal{K}(X/H, \pi(K))$ (TVS, II, §4, No. 4, Mệnh đề 5); vì $H$ tác động đúng trong $X$, tập hợp $P$ của các $\xi \in H$ sao cho $K\xi$ giao với $K$ là compact; từ (3) suy ra $\sup_{x \in K} |f^b(\pi(x))| \leq \beta(P) \sup_{x \in K} |f(x)|$, và điều này chứng minh mệnh đề của chúng ta.

b) Cho $K'$ là một tập con compact của $X/H$. Hãy chọn một tập con compact $K$ của $X$ sao cho $\pi(K) = K'$, và hãy chứng minh rằng hạn chế của $f \mapsto f^b$ vào $\mathcal{K}(X, K)$ là một cấu xạ ngặt của $\mathcal{K}(X, K)$ lên $\mathcal{K}(X/H, K')$. Chỉ cần xây dựng một ánh xạ nghịch đảo phải cho hạn chế này (GT, III, §6, No. 2, Mệnh đề 3). Bây giờ, theo Bổ đề 1 của No. 1 (với các ký hiệu của bổ đề đó), ta thu được một ánh xạ nghịch đảo như vậy bằng cách hợp thành các ánh xạ sau:
$\alpha)$ ánh xạ $f' \mapsto f' \circ \pi$ của $\mathcal{K}(X/H, K')$ vào tập hợp $E$ các hàm của $\mathcal{K}^1(X)$ có giá được chứa trong $KH$;
$\beta)$ ánh xạ của $E$ vào $E$ mà, với mỗi $g \in E$, tương ứng hàm bằng $g/u^1$ trên $KH$, và bằng 0 trên $X - KH$;
$\gamma)$ ánh xạ của $E$ vào $\mathcal{K}(X)$ mà, với mỗi hàm $h \in E$, tương ứng $uh$.

c) Điều này đã được thiết lập, nếu $V$ là một lân cận lồi của 0 trong $\mathcal{K}(X)$, thì $V \cap \mathcal{K}(X, K)$ là một lân cận lồi của 0 trong $\mathcal{K}(X, K)$, do đó $V^b \cap \mathcal{K}(X/H, K')$ là một lân cận lồi của 0 trong $\mathcal{K}(X/H, K')$ theo b), do đó $V^b$ là một lân cận của 0 trong $\mathcal{K}(X/H)$ (TVS, II, §4, No. 4). Điều này hoàn tất chứng minh.

#### Mệnh đề 4 {#int-vii-s2-prop-4 .statement}

a) *Cho $\lambda$ là một độ đo trên $X/H$. Tồn tại một và chỉ một độ đo $\lambda^\#$ trên $X$ sao cho*
$$
\int_{X/H} f^b d\lambda = \int_X f d\lambda^\#
$$
*đối với mọi $f \in \mathcal{K}(X)$. Ta có $\delta(\xi)\lambda^\# = \Delta_H(\xi)\lambda^\#$ với mọi $\xi \in H$.*

b) *Ngược lại, cho $\mu$ là một độ đo trên $X$ sao cho $\delta(\xi)\mu = \Delta_H(\xi)\mu$ với mọi $\xi \in H$. Tồn tại duy nhất một độ đo $\lambda$ trên $X/H$ sao cho $\mu = \lambda^\#$.*

Đây là trường hợp riêng của No. 1, Mệnh đề 3.

#### Định nghĩa 1 {#int-vii-s2-def-1 .statement}

*Với các giả thiết và ký hiệu như trong Mệnh đề 4, $\lambda$ được gọi là thương của $\mu$ theo $\beta$ và được ký hiệu bởi $\frac{\mu}{\beta}$ hoặc $\mu/\beta$.*

Ánh xạ $\lambda \mapsto \lambda^\#$ của $\mathcal{M}(X/H)$ vào $\mathcal{M}(X)$ chính là phép chuyển vị của ánh xạ $f \mapsto f^b$ của $\mathcal{K}(X)$ vào $\mathcal{K}(X/H)$. Cho $\mathfrak{F}$ là một bộ lọc trên $\mathcal{M}(X/H)$; nói rằng $\lim_{\lambda,\mathfrak{F}} \lambda^\#(f) = 0$ với mọi $f \in \mathcal{K}(X)$ tương đương với nói rằng $\lim_{\lambda,\mathfrak{F}} \lambda(f') = 0$ với mọi $f' \in \mathcal{K}(X/H)$; do đó ánh xạ $\lambda \mapsto \lambda^\#$ là, đối với các tôpô mờ, một *đẳng cấu* của $\mathcal{M}(X/H)$ lên một không gian con tuyến tính của $\mathcal{M}(X)$. Không gian con này *đóng mờ*, vì nó là tập hợp các $\mu \in \mathcal{M}(X)$ sao cho $\delta(\xi)\mu = \Delta_H(\xi)\mu$ với mọi $\xi \in H$. Rõ ràng là các điều kiện $\lambda \geqslant 0$ và $\lambda^\# \geqslant 0$ là tương đương.

Công thức (6) có thể, theo phép tương tự với ký hiệu thông thường cho tích phân kép, được viết
$$
\int_X f(x) d\lambda^\#(x) = \int_{X/H} d\lambda(\dot{x}) \int_H f(x\xi) d\beta(\xi) \quad (\dot{x} = \pi(x)).
$$
Điều này bao hàm một sự lạm dụng ký hiệu, vì tích phân $\int_H f(x\xi) d\beta(\xi)$ được xem như một hàm của $\dot{x}$ chứ không phải của $x$; cách viết này sẽ được dùng thường xuyên về sau miễn là không thể xảy ra nhầm lẫn.

#### Nhận xét 2 {#int-vii-s2-n2-rem-2 .statement}

— Cho E là một không gian vectơ lồi địa phương và cho m là một độ đo vectơ trên $X/H$ với giá trị trong E. Khi đó ánh xạ $f \mapsto m(f^b)$ từ $\mathcal{K}(X)$ vào E là một độ đo vectơ trên X, với giá trị trong E, mà ta cũng sẽ ký hiệu là $m^\#$. Ánh xạ $m \mapsto m^\#$ lại là một *đẳng cấu* của $\mathcal{L}(\mathcal{K}(X/H); E)$ lên một không gian con tuyến tính A của $\mathcal{L}(\mathcal{K}(X); E)$ (khi các không gian này được trang bị tôpô hội tụ điểm). Hơn nữa, vì ánh xạ $f \mapsto f^b$ là một cấu xạ ngặt toàn ánh, nên không gian con A chính là tập hợp các độ đo vectơ n trên X mà bằng không trên hạt nhân N của ánh xạ $f \mapsto f^b$. Để $n \in A$, do đó cần và đủ rằng các độ đo vô hướng $z' \circ n$ bằng không trên N với mọi $z' \in E'$. Từ Mệnh đề 3 suy ra rằng $n \in A$ khi và chỉ khi $\delta(\xi)n = \Delta_H(\xi)n$ với mọi $\xi \in H$.

### 3. Một cách diễn giải khác của $\lambda^\#$

Đối với mọi $x \in X$, ánh xạ $\xi \mapsto x\xi$ từ H vào X là thực sự (GT, III, §4, No. 2, Prop. 4), do đó $\beta$ có một đo ảnh trên X dưới ánh xạ này, và ảnh đó tập trung trên quỹ đạo $xH$ (Ch. V, §6, No. 2, Cor. 3 of Prop. 2); vì $\beta$ bất biến trái, đo ảnh này chỉ phụ thuộc vào lớp $u = \pi(x)$ của $x$ trong $X/H$, và sẽ được ký hiệu là $\beta_u$. Theo định nghĩa, với $f \in \mathcal{K}(X)$,

$$
\int_X f(y)\, d\beta_u(y) = \int_H f(x\xi)\, d\beta(\xi) = f^\flat(u).
$$

Suy ra rằng

$$
(\varepsilon_u)^\# = \beta_u.
$$

#### Bổ đề 2 {#int-vii-s2-lem-2 .statement}

*Cho $f$ là một hàm trên X, nhận giá trị trong một không gian tôpô.*

a) *Nếu $f$ là một hàm số thực $\geq 0$ thì, với $x \in X$,*

$$
\int_X^* f(y)\, d\beta_{\dot{x}}(y) = \int_H^* f(x\xi)\, d\beta(\xi) \quad (\dot{x} = \pi(x)).
$$

b) *Để $f$ khả đo được theo $\beta_{\dot{x}}$, cần và đủ là hàm $\xi \mapsto f(x\xi)$ trên H khả đo được theo $\beta$.*

c) *Giả sử rằng $f$ là một hàm trên X, nhận giá trị trong một không gian Banach hoặc trong $\overline{\mathbf{R}}$; khi đó, để $f$ tích phân được theo $\beta_{\dot{x}}$ (tương ứng gần như tích phân được theo $\beta_{\dot{x}}$), cần và đủ là hàm $\xi \mapsto f(x\xi)$ trên H tích phân được theo $\beta$ (tương ứng gần như tích phân được theo $\beta$), trong trường hợp đó $\int_X f(y)\, d\beta_{\dot{x}}(y) = \int_H f(x\xi)\, d\beta(\xi)$.*

Điều này suy ra từ Ch. V, §4, Mệnh đề 2, Mệnh đề 3 và Định lý 2.

Vì $f^\flat \in \mathcal{K}(X/H)$ đối với $f \in \mathcal{K}(X)$, công thức (8) chứng minh rằng ánh xạ $u \mapsto \beta_u$ từ $X/H$ vào $\mathcal{M}(X)$ là liên tục yếu, rằng họ $(\beta_u)$ là $\lambda$-thích hợp$^1$ đối với mọi độ đo dương $\lambda$ trên $X/H$, và rằng

$$
\lambda^\# = \int_{X/H} \beta_u\, d\lambda(u),
$$

điều đó đem lại một cách diễn giải mới cho $\lambda^\#$.

$^1$ Theo nghĩa của lần xuất bản thứ nhất của Ch. V, do đó *a fortiori* theo nghĩa của lần thứ hai (cf. chú thích cho Ví dụ của Ch. VI, §1, No. 1).

#### Mệnh đề 5 {#int-vii-s2-prop-5 .statement}

— Cho $\lambda$ là một độ đo dương trên $X/H$.

a) *Cho $f$ là một hàm khả đo được theo $\lambda^\#$ trên $X$, nhận giá trị trong một không gian tôpô, hằng ngoài một hợp đếm được các tập hợp khả tích theo $\lambda^\#$. Khi đó, tập hợp các $\dot{x} \in X/H$ sao cho hàm $\xi \mapsto f(x\xi)$ không khả đo được theo $\beta$ là địa phương không đáng kể theo $\lambda$.*

b) *Cho $f$ là một hàm khả đo được theo $\lambda^\#$, $\geq 0$, trên X, bằng không ngoài một hợp đếm được các tập hợp khả tích theo $\lambda^\#$. Khi đó, hàm $\dot{x} \mapsto \int^* f(x\xi) d\beta(\xi)$ trên $X/H$ là khả đo được theo $\lambda$, và*

$$
\int_X^* f(x) d\lambda^\#(x) = \int_{X/H}^* d\lambda(\dot{x}) \int_H^* f(x\xi) d\beta(\xi) \quad (\dot{x} = \pi(x)).
$$

c) Cho $f$ là một hàm $\lambda^\#$-khả tích trên $X$, nhận giá trị trong một không gian Banach hoặc trong $\overline{\mathbf{R}}$. Khi đó, tập hợp các $\dot{x} \in X/H$ sao cho $\xi \mapsto f(x\xi)$ không $\beta$-khả tích là $\lambda$-bỏ qua được; hàm $f^b$ trên $X/H$ được xác định gần như mọi nơi bởi công thức

$$
f^b(\dot{x}) = \int_H f(x\xi) d\beta(\xi) \quad (\dot{x} = \pi(x))
$$

là $\lambda$-khả tích, và

$$
\int_{X/H} f^b d\lambda = \int_X f d\lambda^\#
$$

và

$$
\int_{X/H} |f^b| d\lambda \leq \int_X |f| d\lambda^\#.
$$

d) Cho $f$ là một hàm $\lambda^\#$-khả đo trên $X$, nhận giá trị trong một không gian Banach hoặc trong $\overline{\mathbf{R}}$, và bằng không ngoài một hợp đếm được các tập $\lambda^\#$-khả tích. Khi đó, để $f$ là $\lambda^\#$-khả tích, điều kiện cần và đủ là

$$
\int_{X/H}^* d\lambda(\dot{x}) \int_H^* |f(x\xi)| d\beta(\xi) < +\infty \quad (\dot{x} = \pi(x)).
$$

Xét đến Bổ đề 2, các khẳng định a), b) và c) suy ra từ Ch. V, §3, Mệnh đề 4, Mệnh đề 5 và Định lý 1 (trừ (13), điều này suy ra từ (12) vì hiển nhiên là $|f^b| \leq |f|^b$); d) suy ra từ b).

#### Mệnh đề 6 {#int-vii-s2-prop-6 .statement}

— Cho $\lambda$ là một độ đo dương trên $X/H$.

a) Cho $N$ là một tập con của $X/H$. Để $N$ là địa phương $\lambda$-bỏ qua được, điều kiện cần và đủ là $\pi^{-1}(N)$ là địa phương $\lambda^\#$-bỏ qua được.

b) Cho g là một hàm trên X/H, nhận giá trị trong một không gian tôpô. Để g là $\lambda$-khả đo, điều kiện cần và đủ là $g \circ \pi$ là $\lambda^\#$-khả đo.

c) Cho h là một hàm trên X/H, nhận giá trị trong một không gian Banach hoặc trong $\overline{\mathbf{R}}$. Để h là địa phương $\lambda$-khả tích, điều kiện cần và đủ là $h \circ \pi$ là địa phương $\lambda^\#$-khả tích, trong trường hợp đó $(h \cdot \lambda)^\# = (h \circ \pi) \cdot \lambda^\#$.

Giả sử $h \circ \pi$ là địa phương $\lambda^\#$-khả tích. Với mọi $f \in \mathcal{K}(X)$, $f \cdot (h \circ \pi)$ là $\lambda^\#$-khả tích, do đó (Mệnh đề 5) hàm $(f \cdot (h \circ \pi))^b = f^b \cdot h$ là $\lambda$-khả tích và

$$
\int_{X/H} f^b \cdot h \, d\lambda = \int_X f \cdot (h \circ \pi) \, d\lambda^\#.
$$

Vì $f \mapsto f^b$ là một ánh xạ toàn ánh từ $\mathcal{K}(X)$ lên $\mathcal{K}(X/H)$, điều này cho thấy rằng h là địa phương $\lambda$-khả tích và rằng

$$
(h \cdot \lambda)^\# = (h \circ \pi) \cdot \lambda^\#.
$$

Đặc biệt, nếu $\pi^{-1}(N)$ là địa phương $\lambda^\#$-không đáng kể, thì $\varphi_N \circ \pi$ là địa phương $\lambda^\#$-không đáng kể, do đó $(\varphi_N \cdot \lambda)^\# = (\varphi_N \circ \pi) \cdot \lambda^\# = 0$, suy ra $\varphi_N \cdot \lambda = 0$ và N là địa phương $\lambda$-không đáng kể. Giả sử bây giờ rằng $g \circ \pi$ là $\lambda^\#$-đo được. Cho K' là một tập con compact của X/H. Cho $f \in \mathcal{K}_+(X)$ sao cho $f^b = 1$ trên K' (No. 1, Mệnh đề 2), và đặt $K = \operatorname{Supp} f$; ta có $\pi(K) \supset K'$. Tồn tại một phân hoạch của K gồm một tập $\lambda^\#$-không đáng kể M và một dãy $(K_n)$ các tập compact sao cho $(g \circ \pi)|K_n$ liên tục với mọi n. Khi đó $g|_{\pi(K_n)}$ liên tục. Đặt P là tập các điểm của K' không thuộc $\pi(K_1) \cup \pi(K_2) \cup \ldots$; khi đó $\pi^{-1}(P) \cap K$ được chứa trong M, nên là $\lambda^\#$-không đáng kể; do đó $f \cdot \varphi_{\pi^{-1}(P)}$ là $\lambda^\#$-không đáng kể; suy ra (Mệnh đề 5)

$$
0 = \int_X f \cdot \varphi_{\pi^{-1}(P)} \, d\lambda^\# = \int_{X/H} f^b \cdot \varphi_P \, d\lambda \geq \int_{X/H}^* \varphi_P \, d\lambda,
$$

do đó P là $\lambda$-không đáng kể, và g là $\lambda$-đo được.

Nếu N là địa phương $\lambda$-không đáng kể, thì $\pi^{-1}(N)$ là địa phương $\lambda^\#$-không đáng kể (Chương V, §6, No. 6, Hệ quả 1 của Mệnh đề 10). Nếu g là $\lambda$-đo được, thì $g \circ \pi$ là $\lambda^\#$-đo được (*ibid.*). Cuối cùng, giả sử h là địa phương $\lambda$-khả tích. Khi đó ta đã biết rằng $h \circ \pi$ là $\lambda^\#$-đo được. Với mọi $f \in \mathcal{K}_+(X)$, theo Mệnh đề 5,

$$
\int_X^* f(x)|h|(\pi(x)) \, d\lambda^\#(x) = \int_{X/H}^* |h|(u)f^b(u) \, d\lambda(u) < +\infty,
$$

do đó $h \circ \pi$ là địa phương $\lambda^\#$-khả tích.

#### Hệ quả 1 {#int-vii-s2-prop-6-cor-1 .statement}

— Cho $\lambda, \lambda'$ là hai độ đo dương trên X/H. Để $\lambda'$ có cơ sở $\lambda$, cần và đủ rằng ${\lambda'}^\#$ có cơ sở $\lambda^\#$. Để $\lambda$ và $\lambda'$ tương đương, cần và đủ rằng $\lambda^\#$ và ${\lambda'}^\#$ tương đương.

Mệnh đề đầu suy ra từ Mệnh đề 6, a) và c). Mệnh đề thứ hai suy ra từ mệnh đề đầu.

#### Hệ quả 2 {#int-vii-s2-prop-6-cor-2 .statement}

— Cho $\lambda$ là một độ đo dương trên $X/H$, và $f$ là một hàm số trị số đo được theo $\lambda^\#$ trên $X$. Giả sử rằng, với mọi $\xi \in H$, $\delta(\xi)f = f$ địa phương $\lambda^\#$-hầu khắp nơi. Khi đó, tồn tại một hàm $\lambda$-đo được $g$ trên $X/H$ sao cho $f = g \circ \pi$ địa phương $\lambda^\#$-hầu khắp nơi.

Thay $f$ bằng $f/(1+|f|)$, ta quy về trường hợp $f$ bị chặn, do đó khả tích địa phương theo $\lambda^\#$. Đặt $\mu = f \cdot \lambda^\#$. Giả thiết về $f$ suy ra rằng $\delta(\xi)\mu = f \cdot \delta(\xi)\lambda^\# = \Delta_H(\xi)\mu$ với mọi $\xi \in H$. Khi đó tồn tại (Mệnh đề 4) một độ đo $\lambda'$ trên $X/H$ sao cho $\mu = {\lambda'}^\#$. Theo Hệ quả 1, tồn tại một hàm khả tích địa phương theo $\lambda$ $g$ trên $X/H$ sao cho $\lambda' = g \cdot \lambda$. Theo Mệnh đề 6, $f \cdot \lambda^\# = {\lambda'}^\# = (g \circ \pi) \cdot \lambda^\#$, do đó $f = g \circ \pi$ địa phương $\lambda^\#$-hầu khắp nơi.

#### Hệ quả 3 {#int-vii-s2-prop-6-cor-3 .statement}

— a) Cho $(\lambda_\iota)_{\iota \in I}$ là một họ các độ đo thực trên $X/H$. Để họ $(\lambda_\iota)$ bị chặn trên trong $\mathcal{M}(X/H)$, điều kiện cần và đủ là họ $(\lambda_\iota^\#)$ bị chặn trên trong $\mathcal{M}(X)$, trong trường hợp đó

$$
\sup(\lambda_\iota^\#) = (\sup \lambda_\iota)^\#.
$$

b) Cho $\lambda$ là một độ đo thực trên $X/H$. Khi đó $(\lambda^+)^\# = (\lambda^\#)^+$ và $(\lambda^-)^\# = (\lambda^\#)^-$.

c) Cho $\lambda$ là một độ đo phức trên $X/H$. Khi đó $|\lambda|^\# = |\lambda^\#|$.

Giả sử họ $(\lambda_\iota)$ bị chặn trên và đặt $\mu = \sup \lambda_\iota$. Vì $\lambda \geq 0$ suy ra $\lambda^\# \geq 0$, ta có $\mu^\# \geq \lambda_\iota^\#$ với mọi $\iota$, điều này cho thấy rằng họ $(\lambda_\iota^\#)$ bị chặn trên và rằng

$$
(\sup \lambda_\iota)^\# \geq \sup(\lambda_\iota^\#).
$$

Ngược lại, giả sử họ $(\lambda_\iota^\#)$ bị chặn trên và đặt $\nu = \sup(\lambda_\iota^\#)$. Vì $\delta(\xi)\lambda_\iota^\# = \Delta_H(\xi)\lambda_\iota^\#$ với mọi $\xi \in H$, hiển nhiên $\delta(\xi)\nu = \Delta_H(\xi)\nu$, do đó tồn tại một độ đo $\mu' \in \mathcal{M}(X/H)$ sao cho $\nu = {\mu'}^\#$. Vì $\lambda^\# \geq 0$ suy ra $\lambda \geq 0$, ta có $\mu' \geq \lambda_\iota$ với mọi $\iota$, điều này cho thấy họ $(\lambda_\iota)$ bị chặn trên và rằng $\nu = {\mu'}^\# \geq (\sup \lambda_\iota)^\#$, do đó

$$
\sup(\lambda_\iota^\#) \geq (\sup \lambda_\iota)^\#,
$$

điều đó hoàn tất chứng minh của a). Mệnh đề b) sau đó suy ra ngay vì, chẳng hạn, $\lambda^+$ chẳng qua là $\sup(\lambda, 0)$. Để chứng minh c), chỉ cần nhận xét rằng $|\lambda| = \sup \mathcal{R}(\alpha \lambda)$ trên các số phức $\alpha$ có giá trị tuyệt đối bằng 1, và mặt khác rằng $\mathcal{R}(\mu^\#) = (\mathcal{R}\mu)^\#$ với mọi $\mu \in \mathcal{M}(X/H)$.

#### Nhận xét 1 {#int-vii-s2-n3-rem-1 .statement}

Mệnh đề 6 a) có thể phát biểu bằng cách nói rằng $\lambda$ là một độ đo *ảnh giả* của $\lambda^\#$ theo $\pi$ (Ch. VI, §3, No. 2, Định nghĩa 1).

#### Nhận xét 2 {#int-vii-s2-n3-rem-2 .statement}

Giả sử $H$ là *compact* và $\beta$ được chuẩn hóa. Phần bão hòa của mọi tập con compact của $X$ là compact. Do đó, nếu $f \in \mathcal{K}(X/H)$ thì $f \circ \pi \in \mathcal{K}(X)$; và, với mọi độ đo dương $\lambda$ trên $X/H$, Mệnh đề 5 c) cho

$$
\int_X (f \circ \pi)(x)\, d\lambda^\#(x) = \int_{X/H} f(u)\, d\lambda(u).
$$

Nói cách khác, $\lambda$ là *ảnh* của $\lambda^\#$ theo $\pi$.

#### Nhận xét 3 {#int-vii-s2-n3-rem-3 .statement}

Hệ quả 3 c) của Mệnh đề 6 cho thấy ngay rằng các kết quả của tiểu mục này vẫn đúng trong trường hợp các độ đo phức (trừ những kết quả liên quan đến tích phân trên).

#### Nhận xét 4 {#int-vii-s2-n3-rem-4 .statement}

Cho $m$ là một độ đo vectơ trên $X/H$ nhận giá trị trong $E$, và cho $q$ là một nửa chuẩn nửa liên tục dưới trên $E$. Để $m$ là *q-trội được* (Ch. VI, §2, No. 3, Định nghĩa 3), điều kiện cần và đủ là $m^\#$ cũng như vậy, trong trường hợp đó $q(m^\#) = q(m)^\#$. Điều này suy ra ngay từ các định nghĩa và Hệ quả 3 a).

Mặt khác, cho $\mu$ là một độ đo dương trên $X/H$. Để $m$ là vô hướng có cơ sở $\mu$, điều kiện cần và đủ là $m^\#$ cũng là vô hướng có cơ sở $\mu^\#$: điều này suy ra từ Hệ quả 1.

Cuối cùng, nếu $m$ có cơ sở $\mu$, với mật độ $f$ đối với $\mu$ (Ch. VI, §2, No. 4, Định nghĩa 4), thì $m^\#$ có cơ sở $\mu^\#$, với mật độ $f \circ \pi$: điều này suy ra từ Mệnh đề 6 c).

### 4. Trường hợp $X/H$ là paracompact

Nếu $X/H$ là paracompact, trước hết ta sẽ thấy rằng các không gian vectơ $\mathcal{K}^\chi(X)$, với $\chi$ biến, đều *đẳng cấu* với nhau, và đặc biệt đẳng cấu với $\mathcal{K}^1(X)$.

#### Mệnh đề 7 {#int-vii-s2-prop-7 .statement}

*Giả sử $X/H$ paracompact. Cho $\chi$ là một biểu diễn liên tục của $H$ trong $\mathbf{R}_+^*$.*

a) *Trên $X$ tồn tại một hàm liên tục $r$, nhận các giá trị $> 0$, sao cho $r(x\xi) = \chi(\xi)r(x)$ với mọi $x \in X$ và $\xi \in H$.*

b) *Ánh xạ $g \mapsto g/r$ là một đẳng cấu của không gian vectơ $\mathcal{K}^\chi(X)$ lên không gian vectơ $\mathcal{K}^1(X)$.*

Ta áp dụng Mệnh đề 1 của No. 1 bằng cách lấy $f$ là một hàm $\geqslant 0$ không đồng nhất bằng không trên bất kỳ quỹ đạo nào (điều này có thể làm được nhờ Bổ đề 1 của Phụ lục 1); khi đó $r = f^\chi$ thỏa mãn các tính chất của a). Khẳng định b) hiển nhiên.

#### Mệnh đề 8 {#int-vii-s2-prop-8 .statement}

*Giả sử $X/H$ paracompact. Tồn tại trên $X$ một hàm liên tục $h \geqslant 0$, có hỗ trợ có giao compact với* bao hòa của mọi tập con compact của X, và sao cho $h^b = 1$. Với một hàm như vậy, ta có $g = (h \cdot (g \circ \pi))^b$ với mọi hàm liên tục $g$ trên $X/H$.

Ta áp dụng Mệnh đề 1 của No. 1, với $\chi = 1$, bằng cách lấy cho $f$ một hàm $\geqslant 0$ không đồng nhất bằng không trên bất kỳ quỹ đạo nào. Ta có $f^1(x) > 0$ tại mọi điểm $x$ của $X$. Đặt $h = f/f^1$. Khi đó $h^1 = f^1/f^1 = 1$, do đó $h^b = 1$. Suy ra rằng nếu $g$ là một hàm liên tục trên $X/H$, thì $(h \cdot (g \circ \pi))^b = h^b \cdot g = g$.

#### Nhận xét 1 {#int-vii-s2-n4-rem-1 .statement}

Đặc biệt, cho $X$ là một không gian địa phương compact trên đó một nhóm rời rạc $D$ tác động liên tục và đúng đắn bên phải; giả sử $X/D$ là paracompact. Khi đó, tồn tại một hàm liên tục $h \geqslant 0$ trên $X$ có hỗ trợ có giao compact với bao hòa của mọi tập con compact của $X$, và sao cho $\sum_{d \in D} h(xd) = 1$ với mọi $x \in X$ (mọi số hạng của tổng đều bằng không trừ hữu hạn số hạng).

#### Nhận xét 2 {#int-vii-s2-n4-rem-2 .statement}

Ta giữ các giả thiết và ký hiệu của Mệnh đề 8. Ánh xạ $g \mapsto h \cdot (g \circ \pi)$ là một ánh xạ liên tục của $\mathcal{K}(X/H)$ vào $\mathcal{K}(X)$, là một nghịch đảo phải của ánh xạ $f \mapsto f^b$. Do đó, mọi tập con bị chặn (tương ứng compact) của $\mathcal{K}(X/H)$ là ảnh của một tập con bị chặn (tương ứng compact) của $\mathcal{K}(X)$. Từ đó, suy ra ngay rằng ánh xạ $\lambda \mapsto \lambda^\#$ lại là một đẳng cấu của $\mathcal{M}(X/H)$ lên một không gian con tuyến tính đóng của $\mathcal{M}(X)$ khi các không gian này được trang bị tôpô hội tụ bị chặn (tương ứng compact).

#### Mệnh đề 9 {#int-vii-s2-prop-9 .statement}

— *Ta giữ các giả thiết và ký hiệu của Mệnh đề 8.* Cho $\lambda$ là một độ đo dương trên $X/H$.

a) *Cặp* $(\pi, h)$ *thích nghi với* $\lambda^\#$, *và* $\int_X h(x) \varepsilon_{\pi(x)} d\lambda^\#(x) = \lambda$.

b) *Ánh xạ* $\pi$ *thực sự đối với độ đo* $h \cdot \lambda^\#$, *và* $\pi(h \cdot \lambda^\#) = \lambda$.

c) *Cho* $k$ *là một hàm trên* $X/H$, *nhận giá trị trong một không gian Banach hoặc trong* $\overline{\mathbf{R}}$. *Để* $k$ *đo được (resp. khả tích địa phương, khả tích cốt yếu, khả tích) đối với* $\lambda$, *điều kiện cần và đủ là* $h \cdot (k \circ \pi)$ *cũng như thế đối với* $\lambda^\#$; *và, nếu* $k$ *khả tích cốt yếu đối với* $\lambda$, *thì*

$$
\int_{X/H} k \, d\lambda = \int_X h \cdot (k \circ \pi) \, d\lambda^\#.
$$

Cho $f \in \mathcal{K}(X/H)$. Khi đó $h \cdot (f \circ \pi) \in \mathcal{K}(X)$ và

$$
\int_X h(x) f(\pi(x)) d\lambda^\#(x) = \int_{X/H} f(\dot{x}) d\lambda(\dot{x}) \int_H h(x\xi) d\beta(\xi) = \int_{X/H} f(\dot{x}) d\lambda(\dot{x}),
$$

do đó a). Mệnh đề b) được chứng minh tương tự. Các mệnh đề của c) liên quan đến tính đo được, tính khả tích cốt yếu và công thức (14) sau đó có thể thu được bằng cách áp dụng các kết quả của Ch. V (§ 4, Mệnh đề 3, § 5, Định lý 1, § 4, Định lý 2). Nếu $k$ là $\lambda$-khả tích, thì $h \cdot (k \circ \pi)$ là $\lambda^\#$-khả tích (Ch. V, § 3, No. 3, Định lý 1). Nếu $h \cdot (k \circ \pi)$ là $\lambda^\#$-khả tích, Mệnh đề 5 chứng minh rằng $(h \cdot (k \circ \pi))^b = h^b \cdot k = k$ là $\lambda$-khả tích. Nếu $k$ là $\lambda$-khả tích địa phương, thì $h \cdot (k \circ \pi)$ là $\lambda^\#$-khả tích địa phương (Mệnh đề 6). Sau cùng, giả sử $h \cdot (k \circ \pi)$ khả tích địa phương theo $\lambda^\#$; với mọi $f \in \mathcal{H}(X/H)$, $h \cdot (k \circ \pi) \cdot (f \circ \pi)$ có giá compact, và
$$
|h \cdot (k \circ \pi) \cdot (f \circ \pi)| \leq M |h \cdot (k \circ \pi)|,
$$
trong đó $M = \sup |f|$; do đó $h \cdot ((kf) \circ \pi)$ là $\lambda^\#$-khả tích, suy ra $kf$ là $\lambda$-khả tích, theo điều đã chứng minh ở trên; điều này chứng tỏ rằng $k$ thật sự là $\lambda$-khả tích địa phương.

#### Hệ quả {#int-vii-s2-n4-cor-1 .statement}

— *Ánh xạ tuyến tính liên tục* $f \mapsto f^b$ *từ* $L^1(X, \lambda^\#)$ *vào* $L^1(X/H, \lambda)$ *được xác định bởi Mệnh đề 5 là toàn ánh*.

Trước hết giả sử $X/H$ là paracompact và cho $h$ là một hàm trên $X$ thỏa mãn các điều kiện của Mệnh đề 8. Nếu $k$ là một hàm số thực $\lambda$-khả tích trên $X/H$, thì $h \cdot (k \circ \pi)$ là $\lambda^\#$-khả tích và $(h \cdot (k \circ \pi))^b = k$ (Mệnh đề 9).

Trong trường hợp tổng quát, cho $u \in L^1(X/H, \lambda)$. Tồn tại một hàm $f \in \mathcal{L}^1(X/H, \lambda)$ có lớp $u$ và bằng không ngoài một hợp đếm được các tập compact $K_n$. Định nghĩa theo quy nạp một dãy các tập mở tương đối compact $U_n$ của $X/H$ sao cho $U_{n+1} \supset K_n \cup \overline{U}_n$, và cho $V$ là hợp của các $U_n$. Khi đó $V$ là một tập con mở của $X/H$, một hợp đếm được các tập con compact $\overline{U}_n$, do đó là paracompact (GT, I, § 9, No. 10, ĐL. 5). Đặt $Y = \overline{\pi}^{-1}(V)$ và ký hiệu $\lambda_V$ (resp. $\lambda_Y^\#$) là độ đo cảm sinh bởi $\lambda$ (resp. $\lambda^\#$) trên $V$ (resp. $Y$). Rõ ràng $Y/H$ có thể được đồng nhất với $V$ (GT, I, § 3, Mệnh đề 10) và rằng $\lambda_Y^\#$ có thể được đồng nhất với $(\lambda_V)^\#$. Hơn nữa, $f$ bằng không ngoài $V$ và thuộc $\mathcal{L}^1(V, \lambda_V)$. Do đó, tồn tại $g \in \mathcal{L}^1(Y, \lambda_Y^\#)$ sao cho $g^b = f$ hầu khắp nơi trên $V$. Mở rộng $g$ bằng 0 trên $X - Y$, ta thu được một hàm $g_1 \in \mathcal{L}^1(X, \lambda^\#)$, và rõ ràng lớp của $g_1^b$ trong $L^1(X/H, \lambda)$ không gì khác hơn là $u$.

#### Nhận xét 3 {#int-vii-s2-n4-rem-3 .statement}

— Giả sử $X/H$ paracompact, và ta giữ các ký hiệu của Mệnh đề 9. Khi đó ánh xạ $k \mapsto h \cdot (k \circ \pi)$ từ $L^1(X/H, \lambda)$ vào $L^1(X, \lambda^\#)$ là *đẳng cự* theo (14) và là một *nghịch đảo phải* của ánh xạ $f \mapsto f^b$ từ $L^1(X, \lambda^\#)$ lên $L^1(X/H, \lambda)$.

### 5. Các độ đo quasi-bất biến trên một không gian thuần nhất

#### Bổ đề 3 {#int-vii-s2-lem-3 .statement}

— *Cho G là một nhóm compact địa phương, $\mu$ là một độ đo Haar trái trên G, $\nu$ và $\nu'$ là hai độ đo quasi-bất biến khác không trên G. Nếu, với mọi $s \in G$, các mật độ của $\gamma(s)\nu$ đối với $\nu$ và của $\gamma(s)\nu'$* đối với $\nu'$ bằng nhau địa phương $\mu$-hầu khắp nơi, thì $\nu$ và $\nu'$ tỷ lệ với nhau.

Viết $\nu = \rho \cdot \mu$, $\nu' = \rho' \cdot \mu$, trong đó $\rho, \rho'$ là các hàm địa phương khả tích theo $\mu$ trên G và khác không ở mọi nơi ($§ 1$, No. 9, Mệnh đề 11). Với mọi $s \in G$,

$$
\gamma(s)\nu = (\gamma(s)\rho) \cdot \mu, \qquad \gamma(s)\nu' = (\gamma(s)\rho') \cdot \mu,
$$

và giả thiết suy ra rằng $\rho^{-1} \cdot \gamma(s)\rho = {\rho'}^{-1} \cdot \gamma(s)\rho'$ địa phương $\mu$-gần khắp nơi. Đặt $\sigma = \rho'/\rho$, là một hàm $\mu$-đo được trên $G$. Với mọi $s \in G$, $\gamma(s)\sigma = \sigma$ địa phương $\mu$-gần khắp nơi. Do đó $\sigma$ bằng một hằng số địa phương $\mu$-gần khắp nơi, theo Hệ quả 2 của Mệnh đề 6 áp dụng với $X = H = G$.

Cho $G$ là một nhóm địa phương compact, $H$ là một nhóm con đóng của $G$. Xét không gian thuần nhất $G/H$ của các lớp ghép trái theo $H$, trên đó $G$ tác động liên tục ở bên trái. Ta sẽ ցույց rằng tồn tại một và chỉ một lớp các độ đo khác không gần bất biến trên $G/H$.

Chú ý rằng $H$ tác động trên $G$ một cách liên tục và đúng đắn bởi các phép tịnh tiến phải; và không gian thương, chính là $G/H$, là paracompact (GT, III, $§ 4$, No. 6, Prop. 13). Vì thế ta có thể áp dụng các kết quả từ No. 1 đến 4, với $X = G$. Do đó ta có các ánh xạ $f \mapsto f^b$ từ $\mathcal{K}(G)$ lên $\mathcal{K}(G/H)$, và $\lambda \mapsto \lambda^\#$ từ $\mathcal{M}(G/H)$ vào $\mathcal{M}(G)$ (một khi đã cố định một độ đo Haar trái $\beta$ trên $H$). Việc $G$ tác động ở bên trái trên $G/H$ dẫn đến một tính chất bổ sung:

$$
\begin{align*}
(15) \qquad & \gamma_{G/H}(s) \cdot f^b = (\gamma_G(s) \cdot f)^b \qquad (s \in G,\ f \in \mathcal{K}(G)) \\
(16) \qquad & (\gamma_{G/H}(s) \cdot \lambda)^\# = \gamma_G(s) \cdot \lambda^\# \qquad (s \in G,\ \lambda \in \mathcal{M}(G/H)).
\end{align*}
$$

Thật vậy, với mọi $x \in G$,

$$
(\gamma_{G/H}(s) \cdot f^b)(\pi(x)) = f^b(s^{-1}\pi(x)) = f^b(\pi(s^{-1}x))
= \int_H f(s^{-1}x\xi)\, d\beta(\xi) = \int_H (\gamma_G(s)f)(x\xi)\, d\beta(\xi) = (\gamma_G(s)f)^b(\pi(x)),
$$

do đó có công thức (15), suy ra công thức (16).

#### Bổ đề 4 {#int-vii-s2-lem-4 .statement}

Cho $\lambda$ là một độ đo $\neq 0$ trên $G/H$, và $\mu$ là một độ đo Haar trái trên $G$. Các tính chất sau là tương đương:
a) $\lambda$ là gần bất biến dưới $G$;
b) để một tập con $A$ của $G/H$ là địa phương $\lambda$-không đáng kể, cần và đủ rằng $\overline{\pi}^{-1}(A)$ là địa phương $\mu$-không đáng kể;
c) độ đo $\lambda^\#$ tương đương với $\mu$.

Giả sử trường hợp này xảy ra và cho $\lambda^\# = \rho \cdot \mu$, trong đó $\rho$ là một hàm địa phương $\mu$-khả tích và khác không ở mọi nơi. Khi đó, với mọi $s \in G$, mật độ $\theta_s$ của $\gamma_{G/H}(s)\lambda$ đối với $\lambda$ thỏa mãn rằng

$$
\theta_s(\pi(x)) = \frac{\rho(s^{-1}x)}{\rho(x)}
$$

địa phương $\mu$-hầu khắp nơi trên $G$.

c) $\Rightarrow$ b): Điều này suy ra ngay từ Hệ quả 1 của Mệnh đề 6.

b) $\Rightarrow$ a): Nếu tính chất b) đúng, thì tập hợp các tập con địa phương $\lambda$-không đáng kể của $G/H$ là bất biến dưới tác động của $G$, do đó $\lambda$ là gần bất biến dưới tác động của $G$.

a) $\Rightarrow$ c): Giả sử $\lambda$ là gần bất biến dưới tác động của $G$; với mọi $s \in G$, $\lambda$ và $\gamma_{G/H}(s)\lambda$ là tương đương, vì thế $\lambda^\#$ và $\gamma_G(s) \cdot \lambda^\# = (\gamma_{G/H}(s) \cdot \lambda)^\#$ là tương đương (Hệ quả 1 của Mệnh đề 6); vì $\lambda^\# \neq 0$, $\lambda^\#$ tương đương với $\mu$ (§ 1, No. 9, Mệnh đề 11).

Hơn nữa, với mọi $s \in G$,

$$
(\theta_s \circ \pi) \cdot \lambda^\# = (\theta_s \cdot \lambda)^\# = (\gamma_{G/H}(s)\lambda)^\# = \gamma_G(s)\lambda^\#
$$
$$
= (\gamma_G(s)\rho) \cdot \mu = \frac{\gamma_G(s)\rho}{\rho} \cdot \lambda^\#,
$$

do đó (17).

Tính tương đương của a) và b) trước hết suy ra kết quả duy nhất đã nêu, và thậm chí một kết quả chính xác hơn:

#### Định lý 1 {#int-vii-s2-thm-1 .statement}

*Cho $G$ là một nhóm địa phương compact, $H$ là một nhóm con đóng của $G$.*

a) *Bất kỳ hai độ đo gần bất biến không bằng không nào trên $G/H$ đều tương đương; các tập con của $G/H$ địa phương không đáng kể đối với các độ đo này chính là những tập mà ảnh ngược của chúng trong $G$ là địa phương không đáng kể đối với một độ đo Haar.*

b) *Cho $\lambda, \lambda'$ là hai độ đo gần bất biến không bằng không trên $G/H$. Nếu, với mọi $s \in G$, các mật độ của $\gamma_{G/H}(s)\lambda$ đối với $\lambda$ và của $\gamma_{G/H}(s)\lambda'$ đối với $\lambda'$ bằng nhau hầu khắp nơi theo $\lambda$ (hoặc $\lambda'$), thì $\lambda$ và $\lambda'$ tỉ lệ với nhau.*

Mệnh đề a) suy ra ngay từ Bổ đề 4. Cho $\lambda$ và $\lambda'$ là hai độ đo gần bất biến không bằng không thỏa mãn điều kiện của b). Khi đó, với mọi $s \in G$, các mật độ của $\gamma_G(s)\lambda^\#$ đối với $\lambda^\#$ và của $\gamma_G(s){\lambda'}^\#$ đối với ${\lambda'}^\#$ bằng nhau địa phương $\mu$-hầu khắp nơi, do đó (Bổ đề 3) $\lambda^\#$ và ${\lambda'}^\#$ tỉ lệ với nhau, suy ra $\lambda$ và $\lambda'$ tỉ lệ với nhau.

Mặt khác, Bổ đề 4 rút việc tìm các độ đo gần bất biến không bằng không trên $G/H$ về việc tìm các độ đo trên $G$ tương đương với

độ đo Haar và có dạng $\lambda^\#$. Về chủ đề này, ta có bổ đề sau:

#### Bổ đề 5 {#int-vii-s2-lem-5 .statement}

*Cho $\mu$ là một độ đo Haar trái trên $G$, và $\rho$ là một hàm khả tích địa phương theo $\mu$. Để $\rho \cdot \mu$ có dạng $\lambda^\#$, điều kiện cần và đủ là, với mọi $\xi \in H$,*

$$
\rho(x\xi) = \frac{\Delta_H(\xi)}{\Delta_G(\xi)} \rho(x)
$$

*đúng $\mu$-gần khắp địa phương trên $G$.*

Nói rằng $\rho \cdot \mu$ có dạng $\lambda^\#$ tức là nói rằng, với mọi $\xi \in H$, $\delta(\xi)(\rho \cdot \mu) = \Delta_H(\xi)\rho \cdot \mu$ (Mệnh đề 4). Khi đó,

$$
\delta(\xi)(\rho \cdot \mu) = (\delta(\xi)\rho) \cdot (\delta(\xi)\mu) = \Delta_G(\xi)(\delta(\xi)\rho) \cdot \mu,
$$

suy ra bổ đề.

Ta có thể bây giờ thiết lập kết quả tồn tại đã nêu, và thậm chí còn một kết quả chính xác hơn:

#### Định lý 2 {#int-vii-s2-thm-2 .statement}

*Cho $G$ là một nhóm địa phương compact, $H$ là một nhóm con đóng của $G$, $\mu$ là một độ đo Haar trái trên $G$, và $\beta$ là một độ đo Haar trái trên $H$.

a) *Tồn tại các hàm $\rho$ liên tục và $> 0$ trên $G$, sao cho*

$$
\rho(x\xi) = \frac{\Delta_H(\xi)}{\Delta_G(\xi)} \rho(x)
$$

*với mọi* $x \in G$ *và* $\xi \in H$.

b) *Với một hàm $\rho$ như vậy, ta có thể tạo lập độ đo* $\lambda = (\rho \cdot \mu)/\beta$ *trên* $G/H$, *và* $\lambda$ *là một độ đo dương khác không gần bất biến đối với* $G$.

c) *Với* $s, x$ *trong* $G$, $\rho(sx)/\rho(x)$ *chỉ phụ thuộc vào* $s$ *và* $\pi(x)$, *do đó xác định một hàm* $\chi$ *liên tục và* > 0 *trên* $G \times (G/H)$ *sao cho*

$$
\chi(s, \pi(x)) = \frac{\rho(sx)}{\rho(x)}.
$$

*Khi đó*

$$
\gamma_{G/H}(s)\lambda = \chi(s^{-1}, .) \cdot \lambda \quad \text{for all } s \in G.
$$

a) suy ra từ Mệnh đề 7.
b) suy ra từ các Bổ đề 5 và 4.
c) suy ra từ (17).

#### Nhận xét 1 {#int-vii-s2-n5-rem-1 .statement}

Từ Nhận xét 1 của No. 3 suy ra rằng các độ đo gần bất biến khác không trên $G/H$ chẳng qua là các ảnh giả dưới $\pi$ của một độ đo Haar trên $G$.

#### Nhận xét 2 {#int-vii-s2-n5-rem-2 .statement}

Nếu $G$ là một nhóm Lie, ta sẽ thấy sau này rằng hàm $\rho$ của Định lý 2 có thể được chọn là khả vi vô hạn.*

Dưới các giả thiết của Định lý 2, một số kết quả của No. 3 và 4 có thể được đặc biệt hóa như sau (xét đến Ch. V, §4, Định lý 2 và Mệnh đề 2 để chuyển qua từ các tính chất đối với $\mu$ sang các tính chất đối với $\rho \cdot \mu$):

a) Cho $f$ là một hàm khả đo theo $\mu$ trên $G$, lấy giá trị trong một không gian tôpô, hằng ngoài một hợp đếm được các tập hợp khả tích theo $\mu$; khi đó, tập hợp các $\dot{x} \in G/H$ sao cho hàm $\xi \mapsto f(x\xi)$ không khả đo theo $\beta$ là địa phương $\lambda$-không đáng kể.

==========

b) Cho $f$ là một hàm $\mu$-đo được $\geqslant 0$ trên G, bằng không ở ngoài một hợp đếm được các tập hợp $\mu$-khả tích. Khi đó, hàm
$$
\dot{x} \mapsto \int_{H}^{*} f(x\xi) d\beta(\xi)
$$
trên $G/H$ là $\lambda$-đo được và
$$
\int_{G}^{*} f(x)\rho(x) d\mu(x) = \int_{G/H}^{*} d\lambda(\dot{x}) \int_{H}^{*} f(x\xi) d\beta(\xi) \quad (\dot{x} = \pi(x)).
$$

c) Cho $f$ là một hàm $\rho \cdot \mu$-khả tích trên G, với giá trị trong một không gian Banach hoặc trong $\overline{\mathbf{R}}$. Khi đó, tập hợp các $\dot{x} \in G/H$ sao cho $\xi \mapsto f(x\xi)$ không $\beta$-khả tích là $\lambda$-không đáng kể; hàm $\dot{x} \mapsto \int_{H} f(x\xi) d\beta(\xi)$ là $\lambda$-khả tích, và
$$
\int_{G} f(x)\rho(x) d\mu(x) = \int_{G/H} d\lambda(\dot{x}) \int_{H} f(x\xi) d\beta(\xi).
$$

d) Tồn tại một hàm liên tục $h \geqslant 0$ trên G, mà giá đỡ của nó có giao compact với bao hòa KH của mọi tập con compact K của G, và sao cho $\int_{H} h(x\xi) d\beta(\xi) = 1$ với mọi $x \in G$. Để một hàm g trên G/H là đo được (tương ứng địa phương khả tích, khả tích thiết yếu, khả tích) đối với $\lambda$, cần và đủ rằng $h \cdot (g \circ \pi)$ cũng như thế đối với $\rho \cdot \mu = \lambda^{\sharp}$; và, khi g khả tích thiết yếu đối với $\lambda$, ta có
$$
\int_{G/H} g(u) d\lambda(u) = \int_{G} h(x)g(\pi(x)) \rho(x) d\mu(x).
$$

### 6. Các độ đo bất biến tương đối trên một không gian thuần nhất

Cho G lại là một nhóm địa phương compact, H là một nhóm con đóng, $\beta$ là một độ đo Haar trái trên H.

#### Bổ đề 6 {#int-vii-s2-lem-6 .statement}

Cho $\lambda$ là một độ đo trên $G/H$, $\chi$ là một biểu diễn liên tục của G trong $\mathbf{C}^*$. Các tính chất sau là tương đương:
a) $\lambda$ là bất biến tương đối trên $G/H$ với nhân tử $\chi$;
b) $\lambda^\#$ là bất biến tương đối trên G với nhân tử trái $\chi$;
c) $\lambda^\#$ có dạng $a \chi \cdot \mu$ ($a \in \mathbf{C}$).

Điều kiện a) có nghĩa là, với mọi $s \in G$,

$$
\gamma_{G/H}(s)\lambda = \chi(s)^{-1}\lambda;
$$

điều này tương đương với $(\gamma_{G/H}(s)\lambda)^\# = \chi(s)^{-1}\lambda^\#$, tức là với

$$
\gamma_G(s)\lambda^\# = \chi(s)^{-1}\lambda^\#.
$$

Do đó a) tương đương với b). Sự tương đương của b) và c) suy ra từ §1, No. 8, Hệ quả 1 của Mệnh đề 10.

#### Định lý 3 {#int-vii-s2-thm-3 .statement}

Cho G là một nhóm địa phương compact, H là một nhóm con đóng của G, $\mu$ (tương ứng $\beta$) là một độ đo Haar trái trên G (tương ứng H), $\chi$ là một biểu diễn liên tục của G trong $\mathbf{C}^*$.

a) Để tồn tại trên $G/H$ một độ đo khác không bất biến tương đối dưới G và với nhân tử $\chi$, cần và đủ rằng $\chi(\xi) = \Delta_H(\xi)/\Delta_G(\xi)$ với mọi $\xi \in H$.

b) Khi đó độ đo này là duy nhất tới một thừa số hằng; chính xác hơn, nó tỉ lệ với $(\chi \cdot \mu)/\beta$.

Để tồn tại trên $G/H$ một độ đo khác không bất biến tương đối dưới G với nhân tử $\chi$, cần và đủ (Bổ đề 6) rằng $\chi \cdot \mu$ có dạng $\lambda^\#$, do đó (No. 2, Mệnh đề 4) rằng $\delta(\xi)(\chi \cdot \mu) = \Delta_H(\xi)(\chi \cdot \mu)$ với mọi $\xi \in H$. Điều kiện này cũng có thể viết là $\chi(\xi)\chi \cdot \Delta_G(\xi)\mu = \Delta_H(\xi)\chi \cdot \mu$, tức là,

$$
\chi(\xi) = \Delta_H(\xi)/\Delta_G(\xi)
$$

với mọi $\xi \in H$. Do đó a). Mệnh đề b) suy ra ngay từ Bổ đề 6 và thực tế là ánh xạ $\lambda \mapsto \lambda^\#$ là đơn ánh.

Ta sẽ thấy ở §3 (No. 3, Ví dụ 4) vài ví dụ rất đơn giản mà ở đó biểu diễn $\xi \mapsto \Delta_H(\xi)/\Delta_G(\xi)$ không thể được mở rộng thành một biểu diễn liên tục của G trong $\mathbf{C}^*$. Trong trường hợp này, do đó không tồn tại bất kỳ độ đo phức khác không nào trên $G/H$ bất biến tương đối dưới G.

#### Hệ quả 1 {#int-vii-s2-thm-3-cor-1 .statement}

Để trên $G/H$ tồn tại một độ đo dương khác không bất biến tương đối dưới G, điều kiện cần và đủ là tồn tại một biểu diễn liên tục của $G$ trong $\mathbf{R}_+^*$ mở rộng biểu diễn $\xi \mapsto \Delta_H(\xi)/\Delta_G(\xi)$.

Chú ý rằng điều kiện này được thỏa mãn khi $H$ đơn môđula.

#### Hệ quả 2 {#int-vii-s2-thm-3-cor-2 .statement}

— Để trên $G/H$ tồn tại một độ đo dương khác không bất biến dưới $G$, điều kiện cần và đủ là $\Delta_G$ trùng nhau với $\Delta_H$ trên $H$.

#### Hệ quả 3 {#int-vii-s2-thm-3-cor-3 .statement}

— Giả sử rằng $H$ đơn môđula và rằng trên $G/H$ tồn tại một độ đo dương bị chặn khác không $\nu$ bất biến tương đối dưới $G$. Khi đó $\nu$ bất biến, và $G$ đơn môđula.

Cho $\chi$ là nhân tử của $\nu$. Với mọi $s \in G$, $\nu$ và $\gamma(s)\nu$ có cùng khối lượng toàn phần hữu hạn (§ 1, No. 1, công thức (6)); vì $\gamma(s)\nu = \chi(s)^{-1}\nu$, ta có $\chi(s) = 1$. Vậy $\nu$ bất biến. Theo Hệ quả 2, $\Delta_G(s) = 1$ với mọi $s \in H$. Cho $G'$ là tập hợp các $t \in G$ sao cho $\Delta_G(t) = 1$. Đây là một nhóm con chuẩn đóng của $G$ chứa $H$. Cho $\pi$ là ánh xạ chính tắc của $G/H$ lên $G/G'$. Khi đó $\pi(\nu)$ là một độ đo dương khác không, bị chặn, bất biến dưới $G$. Do đó độ đo Haar trái của nhóm $G/G'$ là hữu hạn, suy ra $G/G'$ compact (§ 1, No. 2, Mệnh đề 2). Vì thế ảnh của $G$ qua $\Delta_G$ là một nhóm con compact của $\mathbf{R}_+^*$; nhóm con này thu gọn thành $\{1\}$, do đó $\Delta_G = 1$ trên toàn bộ $G$.

### 7. Độ đo Haar trên một nhóm thương

#### Mệnh đề 10 {#int-vii-s2-prop-10 .statement}

— Cho $G$ là một nhóm compact địa phương, $G'$ một nhóm con chuẩn đóng, $G''$ là nhóm $G/G'$, $\pi$ là ánh xạ chính tắc của $G$ lên $G/G'$, và $\alpha, \alpha', \alpha''$ là các độ đo Haar trái trên $G, G', G''$.

a) Nhân $\alpha$ với một thừa số hằng nếu cần, ta có thể giả sử rằng $\alpha'' = \alpha/\alpha'$. Đặc biệt, nếu $f \in \mathcal{K}(G)$ thì

$$
\int_G f(x)\,d\alpha(x) = \int_{G''} d\alpha''(\dot{x}) \int_{G'} f(x\xi)\,d\alpha'(\xi) \quad (\dot{x} = \pi(x)).
$$

b) Ta có $\Delta_G(\xi) = \Delta_{G'}(\xi)$ với mọi $\xi \in G'$; đặc biệt, nếu $G$ đơn môđula thì $G'$ cũng vậy.

c) Hạt nhân của biểu diễn $\Delta_G$ của $G$ trong $\mathbf{R}_+^*$ là nhóm con chuẩn đóng đơn môđula lớn nhất của $G$.

Áp dụng Định lý 3 của No. 6 với $\chi = 1$ (và biết rằng ở đây, tồn tại một độ đo trên $G/G'$ bất biến dưới $G$, tức là $\alpha''$), ta thu được a) và b); c) suy ra ngay từ b).

#### Mệnh đề 11 {#int-vii-s2-prop-11 .statement}

— Ta giữ các ký hiệu của Mệnh đề 10. Cho $u$ là một tự đẳng cấu của $G$ sao cho $u(G') = G'$. Ký hiệu $u'$ là hạn chế của $u$ lên $G'$, và $u''$ là tự đẳng cấu của $G''$ suy ra từ $u$ bằng cách đi qua các thương. Khi đó

$$
\operatorname{mod}_G(u) = \operatorname{mod}_{G'}(u') \operatorname{mod}_{G''}(u'').
$$

Vì, nếu $\alpha'' = \alpha/\alpha'$ thì $u''(\alpha'') = u(\alpha)/u'(\alpha')$, tức là
$$
\operatorname{mod}_{G''}(u'')^{-1}\alpha'' = \operatorname{mod}_G(u)^{-1}\alpha/\operatorname{mod}_{G'}(u')^{-1}\alpha'
$$
$$
= \frac{\operatorname{mod}_{G'}(u')}{\operatorname{mod}_G(u)} (\alpha/\alpha') = \frac{\operatorname{mod}_{G'}(u')}{\operatorname{mod}_G(u)} \alpha'',
$$
do đó mệnh đề.

#### Hệ quả {#int-vii-s2-n7-cor-1 .statement}

— *Với mọi* $x \in G$,
$$
\Delta_G(x) = \Delta_{G/G'}(\dot{x}) \operatorname{mod}(i_x),
$$
*trong đó* $\dot{x}$ *ký hiệu ảnh chính tắc của* $x$ *trong* $G/G'$, *và* $i_x$ *là tự đẳng cấu* $s \mapsto x^{-1}sx$ *của* $G'$.

Điều này suy ra từ Mệnh đề 11, và công thức (33) của §1, No. 4.

### 8. Một tính chất bắc cầu

Cho $X$ là một không gian địa phương compact mà một nhóm địa phương compact $H$ tác động lên bên phải, liên tục và *chính quy*, bởi $(x, \xi) \mapsto x\xi$ ($x \in X,\ \xi \in H$). Cho $H'$ là một nhóm con đóng của $H$; khi đó $H'$ tác động lên bên phải trên $X$, liên tục và *chính quy*. Ta sẽ ký hiệu $\pi, \pi', p$ là các ánh xạ chính tắc của $X$ lên $X/H$, của $X$ lên $X/H'$, và của $H$ lên $H/H'$.

Cho $\beta, \beta'$ là các độ đo Haar trái trên $H, H'$; giả sử rằng $\Delta_H$ và $\Delta_{H'}$ *trùng nhau trên* $H'$; khi đó ta có thể lập độ đo $\beta/\beta'$ trên $H/H'$, bất biến trái dưới tác động của $H$ (No. 6, Định lý 3). Mặt khác, cho $\mu$ là một độ đo dương trên $X$ sao cho
$$
\delta(\xi)\mu = \Delta_H(\xi)\mu
$$
với $\xi \in H$; khi đó ta có thể lập các độ đo $\mu/\beta$ trên $X/H$ và $\mu/\beta'$ trên $X/H'$ (No. 2, Mệnh đề 4). Ta sẽ viết $\mu/\beta'$ như là *tích phân*, theo $\mu/\beta$, của một họ các độ đo trên $X/H'$ được chỉ số hóa bởi các điểm của $X/H$. Khi $H' = \{e\}$, ta sẽ lại ở trong tình huống của No. 3.

Ánh xạ $(x, \xi) \mapsto \pi'(x\xi)$ của $X \times H$ vào $X/H'$ là *liên tục*; vì $\pi'(x\xi) = \pi'(x\xi\xi')$ với mọi $\xi' \in H'$ nên ánh xạ này xác định, khi qua thương, một ánh xạ *liên tục* của $X \times (H/H')$ vào $X/H'$; do đó, với mỗi $x$ cố định trong $X$, một ánh xạ bộ phận $\omega_x$ của $H/H'$ vào $X/H'$, suy ra khi qua thương từ ánh xạ $\psi_x : \xi \mapsto x\xi$ của H vào X. Chú ý rằng $\psi_{x\xi} = \psi_x \circ \gamma_H(\xi)$, do đó $\omega_{x\xi} = \omega_x \circ \gamma_{H/H'}(\xi)$ với mọi $\xi \in H$.

#### Bổ đề 7 {#int-vii-s2-lem-7 .statement}

*Cho K là một tập con compact của X/H', và L là một tập con compact của X. Khi đó $\bigcup_{x \in L} \omega_x^{-1}(K)$ là tương đối compact trong H/H'._

Cho $K_1$ là một tập con compact của X sao cho $\pi'(K_1) = K$. Cho $K_2$ là tập hợp các $\xi \in H$ sao cho $L\xi$ giao với $K_1$. Khi đó $K_2$ là compact (GT, III, §4, No. 5, Định lý 1). Cho $\xi \in H$ sao cho $p(\xi) \in \bigcup_{x \in L} \omega_x^{-1}(K)$. Do đó, tồn tại một $x \in L$ sao cho $\omega_x(p(\xi)) \in K$, hay nói cách khác là $\pi'(x\xi) \in K$. Vì $\pi'(K_1) = K$, tồn tại $\xi' \in H'$ sao cho $x\xi\xi' \in K_1$. Khi đó $\xi\xi' \in K_2$, do đó $p(\xi) = p(\xi\xi') \in p(K_2)$. Vậy ta đã chứng minh rằng $\bigcup_{x \in L} \omega_x^{-1}(K) \subset p(K_2)$.

This lemma shows first of all that the mapping $\omega_x$ is *thực sự*. One can therefore xác định độ đo $\omega_x(\beta/\beta')$ trên $X/H'$, which is concentrated on $\omega_x(H/H') = \pi'(\psi_x(H)) = \pi'(xH)$. If $f \in \mathcal{K}(X/H')$, Bổ đề 7 and §1, No. 1, Bổ đề 1 show that the function $x \mapsto \langle f, \omega_x(\beta/\beta') \rangle$ is continuous on X; moreover, $\langle f, \omega_x(\beta/\beta') \rangle$ is zero when Supp $f$ does not intersect $\pi'(xH)$, nói cách khác khi $\pi(x)$ không thuộc ảnh chính tắc của Supp $f$ trong $X/H$.

Moreover, if $x \in H$ then

$$
\omega_{x\xi}(\beta/\beta') = \omega_x(\gamma_{H/H'}(\xi)(\beta/\beta')) = \omega_x(\beta/\beta').
$$

The mapping $x \mapsto \omega_x(\beta/\beta')$ of X into $\mathcal{M}(X/H')$ therefore defines by passage to the quotient a mapping $u \mapsto (\beta/\beta')_u$ of $X/H$ into $\mathcal{M}(X/H')$. The foregoing shows that, for every $f \in \mathcal{K}(X/H')$, the mapping $u \mapsto \langle f, (\beta/\beta')_u \rangle$ is continuous with compact support. Consequently the mapping $u \mapsto (\beta/\beta')_u$ *là một họ độ đo liên tục yếu và* $(\mu/\beta)$*-thích hợp trên* $X/H'$, *với* $X/H$ *làm tập chỉ số*.

Let $x \in X$, and $u = \pi(x) \in X/H$. Let $f$ be a function on $X/H'$, with values in a Banach space or in $\overline{\mathbf{R}}$. By Ch. V, §4, Định lý 2, for $f$ to be $(\beta/\beta')_u$-integrable, it is necessary and sufficient that the function $p(\xi) \mapsto f(\omega_x(p(\xi))) = f(\pi'(x\xi))$ on $H/H'$ be $(\beta/\beta')$-integrable, in which case

$$
(21) \quad \int_{X/H'} f(u') d(\beta/\beta')_u(u') = \int_{H/H'} f(\pi'(x\xi)) d(\beta/\beta')(\dot{\xi}) \qquad (\dot{\xi} = p(\xi)).
$$

One has analogous properties for measurability, the upper integral and the essential integral.

#### Mệnh đề 12 {#int-vii-s2-prop-12 .statement}

— *Với các ký hiệu trên*,

$$
\int_{X/H} (\beta/\beta')_u d(\mu/\beta)(u) = \mu/\beta'.
$$

Let $f \in \mathcal{K}(X)$, and let $f^b \in \mathcal{K}(X/H')$, defined by

$$
f^b(\pi'(x)) = \int_{H'} f(x\xi') d\beta'(\xi').
$$

It suffices (cf. No. 2) to prove that $f^b$ has the same integral with respect to the two members of (22). Now, $\langle \mu/\beta', f^b \rangle = \langle \mu, f \rangle$. On the other hand,

$$
\left\langle \int_{X/H} (\beta/\beta')_u d(\mu/\beta)(u), f^b \right\rangle = \int_{X/H} \langle (\beta/\beta')_u, f^b \rangle d(\mu/\beta)(u).
$$

Now, let $x \in X$ and $u = \pi(x)$. We have

$$
\langle (\beta/\beta')_u, f^b \rangle = \langle \omega_x(\beta/\beta'), f^b \rangle = \int_{H/H'} f^b(\omega_x(\dot{\xi})) d(\beta/\beta')(\dot{\xi})
$$
$$
= \int_{H/H'} f^b(\pi'(x\xi)) d(\beta/\beta')(\dot{\xi})
$$
$$
= \int_{H/H'} d(\beta/\beta')(\dot{\xi}) \int_{H'} f(x\xi\xi') d\beta'(\xi')
$$
$$
= \int_H f(x\xi) d\beta(\xi).
$$

Therefore

$$
\left\langle \int_{X/H} (\beta/\beta')_u d(\mu/\beta)(u), f^b \right\rangle = \int_{X/H} d(\mu/\beta)(u) \int_H f(x\xi) d\beta(\xi) = \langle \mu, f \rangle,
$$

which proves the proposition.

#### Hệ quả 1 {#int-vii-s2-prop-12-cor-1 .statement}

— a) *Cho f là một hàm trên X/H', với giá trị trong một không gian Banach hoặc trong $\overline{\mathbf{R}}$, khả tích đối với $\mu/\beta'$. Tồn tại một tập con N không đáng kể theo $(\mu/\beta)$ của X/H có tính chất sau: nếu $x \in X$ sao cho $\pi(x) \notin N$, thì hàm $f \circ \omega_x$ trên H/H', tức là hàm $\dot{\xi} \mapsto f(\pi'(x\xi))$, khả tích đối với $\beta/\beta'$. Nguyên $\int_{H/H'} f(\pi'(x\xi)) d(\beta/\beta')(\dot{\xi})$ chỉ phụ thuộc vào $\dot{x} = \pi(x)$, và là một hàm khả tích theo $(\mu/\beta)$ của $\dot{x}$; và*

$$
\int_{X/H'} f d(\mu/\beta') = \int_{X/H} d(\mu/\beta)(\dot{x}) \int_{H/H'} f(\pi'(x\xi)) d(\beta/\beta')(\dot{\xi}).
$$

b) Cho $f$ là một hàm $\geq 0$ trên $X/H'$, đo được đối với $\mu/\beta'$ và bằng không ngoài một hợp đếm được các tập hợp khả tích theo $(\mu/\beta')$. Khi đó

$$
\pi(x) \mapsto \int_{H/H'}^* f(\pi'(x\xi)) d(\beta/\beta')(\dot{\xi})
$$

là $(\mu/\beta)$-đo được, và

$$
\int_{X/H'}^* f d(\mu/\beta') = \int_{X/H}^* d(\mu/\beta)(\dot{x}) \int_{H/H'}^* f(\pi'(x\xi)) d(\beta/\beta')(\dot{\xi}).
$$

c) Cho $f$ là một hàm trên X/H' với giá trị trong một không gian Banach hoặc trong $\overline{\mathbf{R}}$, đo được đối với $\mu/\beta'$ và bằng không ngoài một hợp đếm được các tập hợp khả tích theo $(\mu/\beta')$. Khi đó, để $f$ khả tích theo $(\mu/\beta')$, điều đủ là

$$
\int_{X/H}^* d(\mu/\beta)(\dot{x}) \int_{H/H'}^* |f(\pi'(x\xi))| d(\beta/\beta')(\dot{\xi}) < +\infty.
$$

#### Hệ quả 2 {#int-vii-s2-prop-12-cor-2 .statement}

— Cho $G$ là một nhóm compact địa phương, $A$ và $B$ là các nhóm con đóng của $G$ sao cho $A \supset B$. Giả sử rằng tồn tại, trên không gian thuần nhất $G/B$ của các lớp ghép trái theo $B$, một độ đo dương khác không $\alpha$ bất biến dưới $G$ và bị chặn.

a) Ảnh chính tắc của $\alpha$ trong $G/A$ là một độ đo dương khác không, bất biến dưới $G$, và bị chặn.

b) $\Delta_G$ trùng với $\Delta_A$ trên $A$ và với $\Delta_B$ trên $B$.

c) Tồn tại, trên không gian thuần nhất $A/B$ của các lớp ghép trái của $A$ theo $B$, một độ đo dương khác không bất biến dưới $A$ và bị chặn.

Mệnh đề a) là hiển nhiên. Mệnh đề b) suy ra từ a) và No. 6, Hệ quả 2 của Định lý 3. Theo b), $\Delta_A$ trùng với $\Delta_B$ trên $B$, và do đó có thể áp dụng các kết quả của tiểu mục hiện tại, với $X = G$, $H = A$, $H' = B$. Hàm 1 trên $G/B$ là $\alpha$-khả tích. Theo a) của Hệ quả 1, hàm 1 trên $A/B$ khả tích đối với $\beta/\beta'$, trong đó $\beta$ và $\beta'$ ký hiệu các độ đo Haar trái trên $A$ và $B$; do đó $\beta/\beta'$ bị chặn.

### 9. Phép dựng độ đo Haar của một nhóm từ các độ đo Haar của một số nhóm con

Cho $G$ là một nhóm compact địa phương, $X$ và $Y$ là hai nhóm con đóng của $G$ sao cho $\Omega = XY$ chứa một lân cận $U$ của $e$. Khi đó $\Omega$ mở trong $G$; vì, với mọi $x_0 \in X$ và $y_0 \in Y$, $XY = (x_0X)(Yy_0) \supset x_0Uy_0$, và $x_0 U y_0$ là một lân cận của $x_0 y_0$; do đó $\Omega$ là một lân cận của mỗi điểm của nó.

*Khi $G$ là một nhóm Lie với đại số Lie $g$, điều kiện đặt ra cho $X$ và $Y$ được thỏa mãn nếu các đại số con tương ứng với $X$ và $Y$ có tổng là $g$.*

Nhóm $X \times Y$ tác động liên tục lên $G$ bên trái, theo luật $(x, y) \cdot s = x s y^{-1}$ ($x \in X, y \in Y, s \in G$). Đặt $Z = X \cap Y$. Nhóm ổn định của $e$ trong $X \times Y$ là nhóm con $Z_0$ của $X \times Y$ gồm các cặp $(z, z)$, với $z \in Z$, một nhóm con đẳng cấu chính tắc với $Z$. Do đó tập $\Omega$ có thể được đồng nhất với không gian thuần nhất $(X \times Y)/Z_0$ của các lớp ghép trái; chính xác hơn, ánh xạ $(x, y) \mapsto xy^{-1}$ của $X \times Y$ lên $\Omega$ xác định, khi qua thương, một song ánh liên tục từ $(X \times Y)/Z_0$ lên $\Omega$. Ta sẽ giả sử rằng ánh xạ này *là một đồng phôi*. (Điều này đặc biệt đúng nếu $G$ đếm được tại vô cùng: xem Phụ lục I.)

#### Mệnh đề 13 {#int-vii-s2-prop-13 .statement}

— *Giả sử thêm rằng $Z$ là compact. Cho $\mu_G, \mu_X, \mu_Y$ là các độ đo Haar trái trên $G$, $X$, $Y$, và $\Lambda$ là sự hạn chế của $\Delta_G$ lên $Y$. Khi đó sự hạn chế $\mu$ của $\mu_G$ lên $\Omega$ là, đến một thừa số hằng, ảnh của $\mu_X \otimes (\Lambda^{-1} \cdot \mu_Y)$ qua ánh xạ $(x, y) \mapsto xy^{-1}$ của $X \times Y$ lên $\Omega$ (một ánh xạ thực sự).

Với $x \in X, y \in Y$,

$$
\gamma((x, y)) \mu = \delta(y) \gamma(x) \mu = \Delta_G(y) \mu .
$$

Nhận diện $\Omega$ với không gian thuần nhất $(X \times Y)/Z_0$ và chọn một độ đo Haar thích hợp trên $Z_0$, ta thấy rằng $\mu^\#$ là tích của độ đo Haar trái của $X \times Y$, tức là $\mu_X \otimes \mu_Y$, với hàm $(x, y) \mapsto \Delta_G(y)^{-1}$ (No. 6, Bổ đề 6). Mặt khác $\mu$ là, tới một nhân tử hằng, ảnh của $\mu^\#$ dưới ánh xạ chính tắc từ $X \times Y$ lên $\Omega$ (No. 3, Nhận xét 2).

#### Hệ quả {#int-vii-s2-n9-cor-1 .statement}

— *Cho f là một hàm xác định trên $\Omega$, nhận giá trị trong một không gian Banach hoặc trong $\overline{\mathbf{R}}$. Để f khả tích theo $\mu$, cần và đủ rằng hàm $(x, y) \mapsto f(xy) \Delta_G(y) \Delta_Y(y)^{-1}$ khả tích theo $(\mu_X \otimes \mu_Y)$; trong trường hợp đó*

$$
\int_\Omega f(\omega) d\mu(\omega) = a \iint_{X \times Y} f(xy) \Delta_G(y) \Delta_Y(y)^{-1} d\mu_X(x) d\mu_Y(y),
$$

trong đó $a$ là một hằng $> 0$ không phụ thuộc vào f.

Theo Mệnh đề 13, và Chương V, §4, No. 4, Định lý 2, để f khả tích theo $\mu$, cần và đủ rằng hàm $(x, y) \mapsto f(xy^{-1})$ khả tích đối với $\mu_X \otimes (\Lambda^{-1} \cdot \mu_Y)$, hoặc cũng vậy rằng hàm $(x, y) \mapsto f(xy^{-1}) \Delta_G(y)^{-1}$ khả tích đối với $\mu_X \otimes \mu_Y$, hoặc cũng vậy rằng hàm $(x, y) \mapsto f(xy) \Delta_G(y) \Delta_Y(y)^{-1}$ khả tích đối với $\mu_X \otimes \mu_Y$. Công thức (23) suy ra từ một lập luận tương tự.

#### Mệnh đề 14 {#int-vii-s2-prop-14 .statement}

— Giả sử các điều kiện của Mệnh đề 13 được thỏa mãn và, ngoài ra, Y là chuẩn tắc.

a) Hạn chế của $\mu_G$ trên $\Omega$ là, tới một nhân tử hằng, ảnh của $\mu_X \otimes \mu_Y$ dưới ánh xạ $(x, y) \mapsto xy$ của $X \times Y$ lên $\Omega$.

b) Với $x \in X$ và $y \in Y$,

$$
\Delta_G(xy) = \Delta_X(x)\Delta_Y(y) \operatorname{mod}(i_x),
$$

trong đó $i_x$ chỉ tự đẳng cấu $v \mapsto x^{-1}vx$ của Y.

Ta có $\Delta_G = \Delta_Y$ trên Y (Mệnh đề 10 b)), do đó a) suy ra từ (23). Cho $x_0 \in X,\ y_0 \in Y$. Kí hiệu $p$ là ánh xạ $(x, y) \mapsto xy$ của $X \times Y$ lên $\Omega$. Vì

$$
xy(x_0y_0)^{-1} = xx_0^{-1}(x_0yy_0^{-1}x_0^{-1}) = xx_0^{-1}i_{x_0^{-1}}(yy_0^{-1}),
$$

ta có

$$
\begin{align*}
\Delta_G(x_0y_0)p(\mu_X \otimes \mu_Y) &= \delta(x_0y_0)p(\mu_X \otimes \mu_Y) \\
&= p(\delta(x_0)\mu_X \otimes i_{x_0^{-1}}\delta(y_0)\mu_Y) \\
&= p(\Delta_X(x_0)\mu_X \otimes \Delta_Y(y_0)(\operatorname{mod}\ i_{x_0})\mu_Y) \\
&= \Delta_X(x_0)\Delta_Y(y_0)(\operatorname{mod}\ i_{x_0})p(\mu_X \otimes \mu_Y),
\end{align*}
$$

do đó b).

#### Nhận xét {#int-vii-s2-n9-rem-1 .statement}

Mệnh đề 14 áp dụng, đặc biệt, khi G là tích nửa trực tiếp tôpô của X bởi Y (GT, III, §2, No. 10). Trong trường hợp này, $Z = \{e\}$ và $\Omega = G$. Vì $yx = xi_x(y)$ với $x \in X,\ y \in Y$, độ đo $\mu_G$ cũng là, tới một nhân tử hằng, ảnh của $(\operatorname{mod}\ i_x)\mu_X \otimes \mu_Y$ dưới ánh xạ $(x, y) \mapsto yx$ của $X \times Y$ vào G.

### 10. Tích phân trên một miền cơ bản

Cho X là một không gian compact địa phương, H là một nhóm rời rạc tác động liên tục và đúng trên X ở phía phải. Cho $\pi$ là ánh xạ chính tắc của X lên $X/H$. Với mọi $x \in X$, ta ký hiệu $H_x$ là nhóm ổn định của $x$ trong H; đây là một nhóm con hữu hạn của H (GT, III, §4, No. 2, Mệnh đề 4); cấp của nó sẽ được ký hiệu là $n(x)$. Với mọi $s \in H,\ H_{xs} = s^{-1}H_x s$, do đó $n(xs) = n(x)$. Tồn tại một lân cận mở U của x sao cho $U \cap Us = \varnothing$ đối với $s \notin H_x$ (loc. cit., No. 4, chứng minh của Mệnh đề 8); với $y \in U$, ta có $H_y \subset H_x$; vì thế hàm $n$ trên X là nửa liên tục trên. Khi X đếm được ở vô cực, H là đếm được; thật vậy, cho $(K_1, K_2, \ldots)$ là một phủ của X bởi một dãy các tập con compact, và cho $x_0 \in X$; tập hợp các $s \in H$ sao cho $x_0 s \in K_i$ là hữu hạn (*loc. cit.*, No. 5, Định lý 1), do đó có mệnh đề của chúng tôi.

#### Định nghĩa 2 {#int-vii-s2-def-2 .statement}

*Cho $F \subset X$. Ta nói rằng $F$ là một miền cơ bản (cho $H$) nếu hạn chế của $\pi$ lên $F$ là một song ánh của $F$ lên $X/H$* (nói cách khác, $F$ là một *hệ đại diện* cho quan hệ tương đương do H xác định).

#### Bổ đề 8 {#int-vii-s2-lem-8 .statement}

— *Cho $F$ là một miền cơ bản. Với mọi $x \in X$,*
$$
\sum_{s \in H} \varphi_{Fs}(x) = n(x).
$$
(24)

Vì $\varphi_{Fs}(xt) = \varphi_{Fst^{-1}}(x)$ với mọi $s$ và $t$ trong H, hai vế của (24) vẫn bất biến khi thay $x$ bằng $xt$. Do đó ta có thể giả sử rằng $x \in F$. Khi đó ta có các tương đương
$$
\varphi_{Fs}(x) = 1 \iff x \in Fs \iff xs^{-1} \in F \iff xs^{-1} = x \iff s \in H_x,
$$
do đó (24).

#### Mệnh đề 15 {#int-vii-s2-prop-15 .statement}

*Giả sử rằng X đếm được ở vô cực. Cho $\mu$ là một độ đo $\geq 0$ trên X. Cho F là một miền cơ bản sao cho $Fs$ là $\mu$-đo được với mọi $s \in H$. Cho f là một hàm khả tích theo $\mu$ trên X, với giá trị trong một không gian Banach hoặc trong $\overline{\mathbf{R}}$. Khi đó họ của các*
$$
\int_{Fs} n(x)^{-1} f(x) d\mu(x) \qquad (s \in H)
$$
*là khả cộng, và*
$$
\int_X f(x) d\mu(x) = \sum_{s \in H} \int_{Fs} n(x)^{-1} f(x) d\mu(x).
$$

Nếu $A$ là một tập con hữu hạn của H, thì
$$
\left| \sum_{s \in A} n^{-1} f \varphi_{Fs} \right| \leq n^{-1} |f| \sum_{s \in A} \varphi_{Fs} \leq |f|
$$
theo Bổ đề 8. Bổ đề 8 cũng chứng minh rằng $\sum_{s \in A} n^{-1} f \varphi_{Fs}$ hội tụ điểm tới $f$ đối với tập có hướng tăng của các tập con hữu hạn của H. Mệnh đề 15 suy ra từ Ch. IV, §4, No. 3, Định lý 2.

#### Định lý 4 {#int-vii-s2-thm-4 .statement}

*Cho X là một không gian compact địa phương đếm được ở vô cực, H là một nhóm rời rạc tác động liên tục và đúng trên X ở phía phải, $\pi$ là ánh xạ chính tắc của X lên X/H, $\mu$ là một độ đo dương trên X bất biến dưới H, $\beta$ là độ đo Haar chuẩn hóa của H, và $\lambda = \mu/\beta$. Cho F là một miền cơ bản đo được theo $\mu$.

a) Cặp $(\pi, n^{-1}\varphi_F)$ là μ-thích nghi, và

$$
\int_X n(x)^{-1} \varphi_F(x) \varepsilon_{\pi(x)} \, d\mu(x) = \lambda.
$$

b) Ánh xạ π là thực sự đối với $n^{-1}\varphi_F \cdot \mu$, và $\pi(n^{-1}\varphi_F \cdot \mu) = \lambda$.

c) Cho k là một hàm trên X/H. Để k là λ-đo được (tương ứng λ-tích phân được), cần và đủ rằng $n^{-1}\varphi_F(k \circ \pi)$ là μ-đo được (tương ứng μ-tích phân được); và, nếu k là λ-tích phân được thì

$$
\int_{X/H} k \, d\lambda = \int_F n^{-1}(k \circ \pi) \, d\mu.
$$

Ta có $\mu = \lambda^\sharp$. Cho $f \in \mathcal{H}_+(X/H)$. Khi đó $n^{-1}\varphi_F(f \circ \pi)$ là μ-đo được và $\geq 0$, và theo Mệnh đề 5 b) của No. 3 ta có

$$
\int_X^* n(x)^{-1} \varphi_F(x) f(\pi(x)) d\mu(x) = \int_{X/H}^* f(\dot{x}) d\lambda(\dot{x}) \int_H^* n(x\xi)^{-1} \varphi_F(x\xi) d\beta(\xi)
$$

và $\int_H^* n(x\xi)^{-1} \varphi_F(x\xi) d\beta(\xi) = n(x)^{-1} \sum_{\xi \in H} \varphi_F(x\xi) = 1$ theo Bổ đề 8. Do đó $n^{-1}\varphi_F \cdot (f \circ \pi)$ là μ-tích phân được và

$$
\int_X n(x)^{-1} \varphi_F(x) f(\pi(x)) d\mu(x) = \int_{X/H} f(\dot{x}) d\lambda(\dot{x}).
$$

Điều đó chứng minh a). Mệnh đề b) được chứng minh tương tự. Mệnh đề c) có thể suy ra từ a) và từ Ch. V, §4, Mệnh đề 3 và Định lý 2.

#### Hệ quả {#int-vii-s2-n10-cor-1 .statement}

- Chúng ta giữ các giả thiết và ký hiệu của Định lý 4. Cho F' là một miền cơ sở thứ hai đo được theo μ. Cho u là một hàm trên X, nhận giá trị trong một không gian Banach hoặc trong $\overline{\mathbf{R}}$, bất biến theo H. Giả sử u khả tích theo μ trên F. Khi đó u khả tích theo μ trên F' và

$$
\int_F u(x) d\mu(x) = \int_{F'} u(x) d\mu(x).
$$

Vì u và n bất biến theo H, tồn tại một hàm v trên X/H sao cho v o π trùng với nu trên F và trên F'. Khi đó $n^{-1} \varphi_F(v \circ \pi) = \varphi_{F'} u, \quad n^{-1} \varphi_{F'}(v \circ \pi) = \varphi_{F'} u.$ Theo giả thiết, $n^{-1} \varphi_F(v \circ \pi)$ là $\mu$-tích phân được. Theo Định lý 4, $v$ là $\lambda$-tích phân được, $\varphi_{F'} \mu$ là $\mu$-tích phân được, và

$$
\int_F u d\mu = \int_{X/H} v d\lambda = \int_{F'} u d\mu.
$$

Về sự tồn tại của các miền cơ sở đo được theo $\mu$, xem Bài tập 12.

### Bài tập {#int-vii-s2-exercises}

Xem các [bài tập cho § 2](exercises/s2/).
