---
book: int
book_title: Integration
chapter: VII
chapter_title: HAAR MEASURE
section: 3
section_title: Applications and examples
lang: vi
source: int-vii-ix
book_pages: INT VII.53-INT VII.73, INT VII.91-INT VII.94
pdf_pages: 0059-0079, 0097-0100
extraction: ocr
subsections:
    - "no": 1
      title: Compact groups of linear mappings
      page: 53
      pdf_page: 59
    - "no": 2
      title: Triviality of fibered spaces and of group extensions
      page: 55
      pdf_page: 61
    - "no": 3
      title: Examples
      page: 60
      pdf_page: 66
statements: 24
exercises: 12
content_sha256: 2040523dede8afee58e4a45c119ab669292c56dd9057a1e8cc61c8464b88b8b2
translated_from: content/en/int/VII/03_s3_applications_and_examples.md
source_content_sha256: be892f61702ef86e17887833e3b3fd6b0a97a2edac49c09d4edd4594b5071311
translation_model: gpt-5-6-mini, gpt-5-6
translation_run: translate-vi-cb2d1caa
glossary_version: 34
glossary_terms_sha256: 5d7a562a5e52273940f265b3b975f6cec051b937c288ebbc21170e85f1828d42
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 3. ỨNG DỤNG VÀ VÍ DỤ

### 1. Các nhóm compact của các ánh xạ tuyến tính

Cho $E$ là một không gian vectơ hữu hạn chiều trên $\mathbf{R}, \mathbf{C}$ hoặc $\mathbf{H}$. Khi đó $\mathrm{End}(E)$ là một đại số hữu hạn chiều trên $\mathbf{R}$, và tôpô chính tắc trên $\mathrm{End}(E)$ (\S 1, No. 10) là tôpô hội tụ compact. Nhóm $\mathrm{Aut}(E) = \mathbf{GL}(E)$ là một tập con mở của $\mathrm{End}(E)$, do đó là một nhóm địa phương compact. Cho $(e_1, e_2, \ldots, e_n)$ là một cơ sở của $E$ và, với mọi tự đồng cấu $u$ của $E$, cho $M(u) = (\alpha_{ij}(u))$ là ma trận của $u$ đối với cơ sở này; nói rằng một tập con $S$ của $\mathrm{End}(E)$ là tương đối compact trong $\mathrm{End}(E)$ tương đương với việc nói rằng các hàm $\alpha_{ij}(u)$ bị chặn trong $S$.

#### Mệnh đề 1 {#int-vii-s3-prop-1 .statement}

— *Cho G là một nhóm con của Aut(E)*. *Ba tính chất sau đây là tương đương*:

(i) *G là tương đối compact trong End(E)*;
(ii) *G là tương đối compact trong Aut(E)*;
(iii) *G bất biến một dạng Hermit dương không suy biến$^1$ trên E*.

(iii) $\Rightarrow$ (i): Giả sử rằng $G$ bất biến một dạng Hermit dương không suy biến $\Psi$. Cho $(e_1, \ldots, e_n)$ là một cơ sở trực chuẩn đối với $\Psi$ (*Alg.*, Ch. IX, \S 6, No. 1, Hệ quả 1 của Định lý 1). Với mọi $u \in G$, cho $(u_{ij})$ là ma trận của nó đối với $(e_i)$. Với mọi $j$, ta có $\sum_{i=1}^n |u_{ij}|^2 = 1$, do đó $|u_{ij}| \leq 1$ với mọi $i$ và $j$, điều này chứng minh (i).

(i) $\Rightarrow$ (ii): Điều này suy ra từ GT, X, \S 3, No. 5, Hệ quả của Định lý 4, có tính đến sự kiện rằng tôpô của $\mathrm{End}(E)$ là tôpô hội tụ compact.

(ii) $\Rightarrow$ (iii): Giả sử bao đóng $\overline{G}$ của $G$ trong $\mathrm{Aut}(E)$ là compact. Cho $\Phi$ là một dạng Hermit dương không suy biến trên $E$. Nếu trường vô hướng là $\mathbf{R}$ hoặc $\mathbf{C}$, việc cho $\Phi$ làm cho $E$ trở thành một không gian Hilbert hữu hạn chiều, và điều kiện (iii) sẽ suy ra từ bổ đề sau:

$^1$ Non dégénérée; trong EVT, thuật ngữ này được thay bằng séparante, sau đó được dịch là "phân tách" (TVS, V, \S 1, No. 1).

#### Bổ đề 1 {#int-vii-s3-lem-1 .statement}

Cho F là một không gian Hilbert, K là một nhóm compact, và $s \mapsto U(s)$ là một biểu diễn của K trong nhóm các phần tử khả nghịch của $\mathcal{L}(F; F)$, liên tục đối với tôpô hội tụ từng điểm. Tồn tại một dạng Hermit dương không suy biến $\varphi$ trên F sao cho

$$
\varphi(U(s)x, U(s)y) = \varphi(x, y)
$$

với mọi $s \in K, x \in F, y \in F$, và sao cho cấu trúc không gian vectơ tôpô của F được xác định bởi $\varphi$ (TVS, V, §1, No. 3) trùng với cấu trúc ban đầu của F.

Cho $\alpha$ là một độ đo Haar trên K. Với mọi $x, y$ trong F, ánh xạ $s \mapsto (U(s)x|U(s)y)$ là liên tục. Đặt

$$
\varphi(x, y) = \int (U(s)x|U(s)y)\, d\alpha(s).
$$

Điều này là hiển nhiên rằng $\varphi(x, y)$ là một dạng song tuyến tính Hermit trên F. Vì tập các tự đồng cấu $U(s)$ là compact trong $\mathcal{L}_s(F; F)$, tồn tại một hằng số M sao cho $\|U(s)\| \leq M$ với mọi $s \in K$. Với mọi $x \in F$, do đó ta có

$$
M^{-1}\|x\| \leq \|U(s)x\| \leq M\|x\|,
$$

do đó suy ra các bất đẳng thức

$$
M^{-2}\alpha(K)\|x\|^2 \leq \varphi(x, x) \leq M^2\alpha(K)\|x\|^2,
$$

điều này cho thấy rằng $\varphi$ là dương và không suy biến, và rằng chuẩn $\varphi(x, x)^{1/2}$ là tương đương với chuẩn $\|x\|$. Cuối cùng, với mọi $t \in K$,

$$
\begin{align*}
\varphi(U(t)x, U(t)y) &= \int (U(st)x|U(st)y)\, d\alpha(s) \\
&= \int (U(s)x|U(s)y)\, d\alpha(s) = \varphi(x, y).
\end{align*}
$$

Khi trường vô hướng là $\mathbf{H}$, ta lập luận hoàn toàn như trước bằng cách thay thế ở mọi nơi hàm $s \mapsto (U(s)x|U(s)y)$ bởi hàm $s \mapsto \Phi(sx, sy)$ xác định trên G, với các giá trị trong $\mathbf{H}$. Điều này hoàn thành chứng minh của mệnh đề.

#### Nhận xét {#int-vii-s3-n1-rem-1 .statement}

Cho $\Phi$ là một dạng Hermit dương không suy biến trên E. Nhóm unita $\mathbf{U}(\Phi)$ là đóng trong $\mathrm{Aut}(E)$, do đó là compact (Mệnh đề 1). Mệnh đề 1 cũng chỉ ra rằng mọi nhóm con compact của $\mathrm{Aut}(E)$ đều được chứa trong một nhóm con có dạng $\mathbf{U}(\Phi)$. Nếu bây giờ $\mathbf{U}(\Phi)$ được chứa trong một nhóm con compact K của $\mathrm{Aut}(E)$, ta thấy rằng tồn tại một dạng Hermit dương không suy biến $\Phi'$ trên E sao cho $\mathbf{U}(\Phi) \subset K \subset \mathbf{U}(\Phi')$, và dễ dàng suy ra

(Bài tập 1) rằng $\Phi$ và $\Phi'$ tỉ lệ, do đó $\mathbf{U}(\Phi) = K$. Như vậy các nhóm con compact cực đại của $\mathrm{Aut}(E)$ là các nhóm con có dạng $\mathbf{U}(\Phi)$.

### 2. Tính tầm thường của các không gian sợi và của các mở rộng nhóm

#### Mệnh đề 2 {#int-vii-s3-prop-2 .statement}

*Cho X là một không gian compact địa phương trong đó một nhóm compact địa phương H tác động bên phải, liên tục và đúng, bởi $(x, \xi) \mapsto x\xi$. Giả sử rằng X/H là paracompact. Cho g là một biểu diễn liên tục của H trong $\mathbf{R}^n$. Khi đó tồn tại một ánh xạ liên tục f của X vào $\mathbf{R}^n$ sao cho $f(x\xi) = f(x) + g(\xi)$ với mọi $x \in X$ và $\xi \in H$.*

Ta ngay lập tức quy về trường hợp $n = 1$. Vì nhóm cộng $\mathbf{R}$ đẳng cấu với nhóm nhân $\mathbf{R}_+^*$, mệnh đề khi đó là một hệ quả ngay lập tức của Mệnh đề 7 của §2, No. 4.

#### Hệ quả {#int-vii-s3-n2-cor-1 .statement}

*Cho X là một không gian compact địa phương trong đó một không gian vectơ thực hữu hạn chiều V tác động bên phải, liên tục và đúng, bởi $(x, v) \mapsto xv$. Cho $\pi$ là ánh xạ chính tắc của X lên $B = X/V$. Giả sử rằng B là paracompact.*

a) *Tồn tại một ánh xạ liên tục f của X vào V sao cho $f(xv) = f(x) + v$ với mọi $x \in X$ và $v \in V$.*

b) *Nếu f là một ánh xạ thỏa mãn các điều kiện của a), thì ánh xạ $x \mapsto (\pi(x), f(x))$ là một phép đồng phôi của X lên $B \times V$.*

Mệnh đề a) suy ra từ Mệnh đề 2 trong đó g được lấy là ánh xạ đồng nhất của V. Cho f là một ánh xạ thỏa mãn các điều kiện của a). Ánh xạ $x \mapsto x \cdot (-f(x))$ của X vào X là liên tục, và là hằng trên mỗi quỹ đạo, do đó có dạng $\varphi \circ \pi$, trong đó $\varphi$ là một ánh xạ liên tục của B vào X; với mọi $b \in B$, $\pi(\varphi(b)) = b$. Các ánh xạ $x \mapsto (\pi(x), f(x))$ của X vào $B \times V$ và $(b, v) \mapsto \varphi(b) \cdot v$ của $B \times V$ vào X là nghịch đảo của nhau, vì $\varphi(\pi(x)) \cdot f(x) = x \cdot (-f(x)) \cdot (f(x)) = x$, $\pi(\varphi(b) \cdot v) = \pi(\varphi(b)) = b$, và, nếu $b = \pi(y)$, thì

$$
f(\varphi(\pi(y)) \cdot v) = f(y \cdot (-f(y)) \cdot v) = f(y) - f(y) + v = v .
$$

Vì các ánh xạ này liên tục, chúng là các đồng phôi.

#### Nhận xét {#int-vii-s3-n2-rem-1 .statement}

— Cho E là một không gian affine thực hữu hạn chiều, T là một không gian compact, $\mu$ là một độ đo trên T có *khối lượng toàn phần* 1, và f là một ánh xạ liên tục từ T vào E. Nếu một gốc a trong E được chọn, E trở thành được trang bị một cấu trúc không gian vectơ, và tích phân $\int_T f(t) d\mu(t)$ do đó có nghĩa; nó biểu diễn điểm x của E sao cho

$$
x - a = \int_T (f(t) - a) d\mu(t) .
$$

Điểm này độc lập với lựa chọn $a$. Thật vậy, cho $a' \in \mathbf{E}$ và $x' \in \mathbf{E}$ sao cho $x' - a' = \int_{\mathbf{T}} (f(t) - a') d\mu(t)$. Khi đó

$$
x' - a = (x' - a') + (a' - a) = \int_{\mathbf{T}} (f(t) - a') d\mu(t) + \int_{\mathbf{T}} (a' - a) d\mu(t)
$$
$$
= \int_{\mathbf{T}} (f(t) - a) d\mu(t) = x - a,
$$

do đó $x' = x$. Vì vậy ta có thể dùng ký hiệu $\int_{\mathbf{T}} f(t) d\mu(t)$ mà không cần chỉ rõ lựa chọn gốc trong $\mathbf{E}$. Nếu $u$ là một ánh xạ affine từ $\mathbf{E}$ vào một không gian affine hữu hạn chiều khác $\mathbf{E}'$, thì

$$
u \left( \int_{\mathbf{T}} f(t) d\mu(t) \right) = \int_{\mathbf{T}} u(f(t)) d\mu(t).
$$

Thật vậy, $\mathbf{E}$ và $\mathbf{E}'$ có thể được đồng nhất với các không gian vectơ theo cách sao cho $u$ trở thành một ánh xạ tuyến tính, trong trường hợp đó công thức đã biết (Ch. III, §3, No. 2, Mệnh đề 2 và No. 3, Mệnh đề 7).

#### Bổ đề 2 {#int-vii-s3-lem-2 .statement}

*Cho $G$ là một nhóm compact, $\mu$ là độ đo Haar chuẩn hóa của $G$, $\mathbf{E}$ là một không gian affine thực hữu hạn chiều, $A$ là nhóm affine của $\mathbf{E}$, và $\rho$ là một đồng cấu từ $G$ vào $A$. Giả sử rằng, với mọi $x \in \mathbf{E}$, ánh xạ $s \mapsto \rho(s)x$ từ $G$ vào $\mathbf{E}$ là liên tục. Khi đó, với mọi $x \in \mathbf{E}$, điểm*

$$
x_0 = \int_G \rho(s)x\, d\mu(s) \in \mathbf{E}
$$

*là bất biến dưới tác động của $G$.*

Thật vậy, với mọi $t \in G$,

$$
\rho(t)x_0 = \int_G \rho(t)\rho(s)x\, d\mu(s) = \int_G \rho(ts)x\, d\mu(s) = \int_G \rho(s)x\, d\mu(s) = x_0.
$$

#### Mệnh đề 3 {#int-vii-s3-prop-3 .statement}

*Cho $G$ là một nhóm compact địa phương. Cho $H$ là một nhóm con chuẩn đóng của $G$, đẳng cấu với $\mathbf{R}^n$ và sao cho $G/H$ là compact.*

a) *Có một nhóm con đóng $L$ của $G$ sao cho $G$ là tích nửa trực tiếp tôpô của $L$ và $H$.*

b) *Nếu $M$ là một nhóm con compact của $G$, có một phần tử $x \in H$ sao cho $x^{-1}Mx \subset L$.*

c) *Mọi nhóm con compact của $G$ đều được chứa trong một nhóm con compact cực đại.*

d) *Các nhóm con compact cực đại của $G$ là các nhóm con là các ảnh của $L$ qua các tự đẳng cấu nội của $G$.*

Cho $\pi$ là đồng cấu chính tắc của $G$ lên $K = G/H$. Bằng phép chuyển qua thương, ánh xạ $(s, h) \mapsto shs^{-1}$ từ $G \times H$ vào $H$ xác định một ánh xạ liên tục $(\sigma, h) \mapsto \sigma \cdot h$ từ $K \times H$ vào $H$ sao cho $shs^{-1} = \pi(s) \cdot h$. Ta sẽ đồng nhất $H$ với $\mathbf{R}^n$ (và do đó sẽ sử dụng, tùy trường hợp, hoặc ký hiệu nhân hoặc ký hiệu cộng cho luật nhóm trong $H$). Theo Hệ quả của Mệnh đề 2, tồn tại một ánh xạ liên tục $f$ từ $G$ vào $H$ sao cho $f(xh) = f(x) + h$ với $x \in G, h \in H$. Với mọi $x \in G$, đặt $p(x) = x \cdot (-f(x))$, điều này chỉ phụ thuộc vào lớp kề của $x$ đối với $H$. Đặt

$$
\begin{align*}
(1) \quad F(x, y) &= p(xy)^{-1} p(x)p(y) = f(xy)y^{-1}x^{-1}x(-f(x))y(-f(y)) \\
&= f(xy)[y^{-1}(-f(x))y](-f(y)) \\
&= f(xy) - \pi(y)^{-1}f(x) - f(y).
\end{align*}
$$

Ta thấy rằng *nếu* $F(x, y) = 0$ *với mọi* $x, y$ *trong* $G$, thì $p(G) = L$ là một nhóm con của $G$ giao với mỗi lớp kề của $H$ tại một và chỉ một điểm. Vì $p$ liên tục, khi đó $G$ là tích nửa trực tiếp tôpô của $L$ và $H$ (GT, III, §2, No. 10).

Bây giờ, với mọi $h, h' \in H$,

$$
\begin{align*}
F'(xh, yh') &= f(xhyh') - \pi(y)^{-1}f(xh) - f(yh') \\
&= f(xhy) + h' - \pi(y)^{-1}f(x) - \pi(y)^{-1}h - f(y) - h' \\
&= f(xy(\pi(y)^{-1}h)) - \pi(y)^{-1}f(x) - f(y) - \pi(y)^{-1}h \\
&= f(xy) - \pi(y)^{-1}f(x) - f(y) = F(x, y).
\end{align*}
$$

Do đó $F$ xác định, bằng phép chuyển qua các thương, một ánh xạ liên tục $\varphi$ từ $K \times K$ vào $H$.

Mặt khác, với mọi $x, y, z$ trong $G$, ta có

$$
\begin{align*}
F(z, xy) + F(x, y) &= f(zxy) - \pi(xy)^{-1}f(z) - f(xy) + f(xy) \\
&\phantom{=} - \pi(y)^{-1}f(x) - f(y) \\
&= \pi(y)^{-1}f(zx) - \pi(xy)^{-1}f(z) - \pi(y)^{-1}f(x) + f(zxy) \\
&\phantom{=} - \pi(y)^{-1}f(zx) - f(y) \\
&= \pi(y)^{-1}F(z, x) + F(zx, y),
\end{align*}
$$

do đó, với mọi $x', y', z'$ trong $K$,

$$
-\varphi(x', y') = \varphi(z', x'y') - y'^{-1}\varphi(z', x') - \varphi(z'x', y').
$$

Ta hãy lấy tích phân theo $z'$ bằng độ đo Haar chuẩn hóa $\alpha$ của $K$. Đặt $\psi(x') = \int \varphi(z', x')\, d\alpha(z')$, $\psi$ là một hàm liên tục trên K, và (nhận thấy rằng các phép toán của K trong $\mathbf{R}^n$ tôn trọng cấu trúc không gian vectơ của $\mathbf{R}^n$ theo GT, VII, §2, No. 1, Mệnh đề 1), ta thu được

$$
-\varphi(x', y') = \psi(x'y') - y'^{-1}\psi(x') - \psi(y').
$$

Nói cách khác, đặt $k - \psi \circ \pi$, là một hàm liên tục trên $G$,

(2)
$$
-F(x, y) = k(xy) - \pi(y)^{-1}k(x) - k(y).
$$

So sánh (1) và (2), ta thấy rằng nếu thay $f$ bởi hàm liên tục $f + k$ (vẫn giữ nguyên tính chất $f(xh) = f(x) + h$), thì $F$ được thay bởi 0 và, như ta đã thấy trước đó, điều này hoàn tất chứng minh của a).

Với mọi $g \in G$, gọi $l_g$ (tương ứng $h_g$) là phần tử duy nhất của L (tương ứng H) sao cho $g = h_g l_g$. Nếu $h_1 \in H$ và $g \in G$, thì

$$
gh_1 = h_g l_g h_1 = h_g(l_g h_1 l_g^{-1})l_g,
$$

do đó $h_g h_1 = h_g + l_g h_1 l_g^{-1}$. Với mọi $g \in G$, gọi $\psi_g$ là ánh xạ của H vào chính nó được xác định bởi

$$
\psi_g(h_1) = h_g + l_g h_1 l_g^{-1}.
$$

Ta thấy rằng ánh xạ $(g, h_1) \mapsto \psi_g(h_1)$ của $G \times H$ vào H là liên tục và làm cho H thành một không gian thuần nhất đối với G, trong đó nhóm ổn định của gốc là L. Ngoài ra, ta nhận thấy rằng khi H được đồng nhất với $\mathbf{R}^n$, $\psi_g$ là một ánh xạ *afin* của H vào chính nó. Với điều này, cho M là một nhóm con compact của G; theo Bổ đề 2, tồn tại một $x \in H$ sao cho $\psi_m(x) = x$ với *mọi* $m \in M$. Với $y \in H$, $\psi_y$ là phép tịnh tiến với vectơ $y$; suy ra rằng với mọi $m \in M$, $\psi_{x^{-1}} \circ \psi_m \circ \psi_x$ biến gốc của H thành chính nó, do đó $x^{-1}mx \in L$. Điều này chứng minh rằng $x^{-1}Mx \subset L$, do đó b).

Cho $L'$ là một nhóm con đóng của G chứa L. Khi đó $L'$ là tích nửa trực tiếp tôpô của L và $L' \cap H$. Nếu $L'$ compact, thì $L' \cap H$ compact nên thu về một điểm (GT, IV, §2, No. 2, Hệ quả 1 của Định lý 2), do đó $L' = L$. Điều này chứng minh rằng L là một nhóm con compact cực đại của G; do đó điều tương tự cũng đúng với các nhóm con là các ảnh của L qua các tự đẳng cấu nội của G. Các khẳng định c) và d) của Mệnh đề 3 khi đó là các hệ quả ngay lập tức của b).

#### Mệnh đề 4 {#int-vii-s3-prop-4 .statement}

*Cho G là một nhóm compact địa phương và H là một nhóm con chuẩn đóng của G sao cho K = G/H là compact. Khi đó mọi biểu diễn liên tục u của H trong $\mathbf{R}$, sao cho $u(s\xi s^{-1}) = u(\xi)$ với mọi $\xi \in H$ và $s \in G$, có thể được mở rộng thành một biểu diễn liên tục của G trong $\mathbf{R}$.*

Đặt $L = G \times \mathbf{R}$ và gọi M là tập hợp các $(\xi, -u(\xi))$, trong đó $\xi$ chạy trên H. Hiển nhiên M là một nhóm con chuẩn đóng của L. Đặt $L' = L/M$ và gọi $\pi$ là ánh xạ chính tắc của L lên $L'$. Nhóm con của L sinh bởi M và R là H × R, do đó là đóng; vì vậy π(R) là một nhóm con đóng N của L'. Hạn chế ρ của π lên R là một biểu diễn song ánh liên tục của R lên N. Bổ đề 2 của Phụ lục 1 chứng minh rằng ρ là song liên tục. Ngoài ra, $L'/N$ đẳng cấu với $L/(H × R) = G/H$, nên là compact. Theo Mệnh đề 3, và xét đến sự kiện rằng N nằm trong tâm của L', L' là tích của N với một nhóm con khác. Do đó tồn tại một biểu diễn liên tục của L' lên N thu hẹp trên N thành ánh xạ đồng nhất. Vì vậy tồn tại một biểu diễn liên tục v của L vào R là tầm thường trên M và thu hẹp trên R thành ánh xạ đồng nhất. Với ξ ∈ H, ta có $v((\xi, 0)) = v((\xi, −u(\xi))(e, u(\xi))) = u(\xi)$, điều này hoàn tất chứng minh.

#### Bổ đề 3 {#int-vii-s3-lem-3 .statement}

Cho G là một nhóm tôpô được sinh bởi một lân cận compact của e. Cho H là một nhóm con đóng của G sao cho không gian thuần nhất G/H là compact. Khi đó H được sinh bởi một lân cận compact của e trong H.

Cho C là một tập compact sao cho G = CH. Nếu cần, phóng đại C, ta có thể giả sử rằng C sinh ra G và rằng G = ĈH. Khi đó C^2 là compact và được phủ bởi các Ĉs (s ∈ H), là các tập mở. Vì vậy tồn tại $s_1, ..., s_n$ trong H sao cho $C^2 \subset Ĉs_1 \cup ... \cup Ĉs_n$. Gọi Γ là nhóm con của H sinh bởi các $s_i$. Khi đó $C^2 \subset CΓ$. Bằng quy nạp, suy ra rằng $C^n \subset CΓ$ với mọi n, do đó $G = CΓ$. Mọi phần tử của H có thể được viết dưới dạng ab với a ∈ C, b ∈ Γ, do đó a ∈ H, do đó $a \in C \cap H$. Vì vậy H được sinh bởi $C \cap H$ và các $s_i$, tức là bởi một tập compact.

#### Bổ đề 4 {#int-vii-s3-lem-4 .statement}

Cho G là một nhóm tôpô liên thông, D là một nhóm con chuẩn rời rạc của G. Khi đó D được chứa trong tâm của G.

Thật vậy, cho d ∈ D. Ảnh của G qua ánh xạ liên tục $x \mapsto xdx^{-1}$ là một tập con liên thông của D, do đó thu về $\{d\}$, điều này chứng minh rằng xd = dx với mọi x ∈ G.

#### Mệnh đề 5 {#int-vii-s3-prop-5 .statement}

Cho G là một nhóm tôpô liên thông thừa nhận một nhóm con chuẩn rời rạc D sao cho K = G/D là compact, và sao cho nhóm con giao hoán tử của K là trù mật trong K. Khi đó D là hữu hạn và G là compact.

Nhóm G địa phương đẳng cấu với K (GT, III, §2, No. 6, Mệnh đề 19), do đó là compact địa phương; vì nó liên thông, nó được sinh bởi một lân cận compact của e. Theo các Bổ đề 3 và 4, D là một nhóm Abel sinh hữu hạn, do đó đẳng cấu với một nhóm $\mathbf{Z}^r \times D_1$ với D_1 hữu hạn (A, VII, §4, No. 7, Định lý 3). Giả sử rằng r > 0. Khi đó tồn tại một biểu diễn f của D lên $\mathbf{Z}$. Theo Mệnh đề 4, f có thể được mở rộng thành một biểu diễn liên tục g của G trong R. Qua phép chuyển sang thương, g xác định một biểu diễn liên tục $g'$ của $K$ trong $\mathbf{R}/\mathbf{Z}$; vì $\mathbf{R}/\mathbf{Z}$ là Abel, hạt nhân của $g'$ chứa nhóm con giao hoán tử của K, do đó $g'$ là tầm thường; nói cách khác, $g(G) \subset \mathbf{Z}$. Vì G liên thông, suy ra rằng $g(G) = \{0\}$, điều này là vô lý vì $f(D) = \mathbf{Z}$. Vậy $r = 0$ và D là hữu hạn. Do đó G là compact (GT, III, §4, No. 1, Hệ quả 2 của Mệnh đề 2).

### 3. Các ví dụ

Trong tiểu mục này (ngoại trừ các Ví dụ 7 và 8), $K$ ký hiệu một trường giao hoán compact địa phương không rời rạc; $dx$ ký hiệu một độ đo Haar trên nhóm cộng của $K$.

Nhắc lại rằng $\operatorname{mod} x = |x|$ khi $K = \mathbf{R}$, $\operatorname{mod} x = |x|^2$ khi $K = \mathbf{C}$, $\operatorname{mod} x = |x|_p$ khi $K = \mathbf{Q}_p$.

#### Ví dụ 1 {#int-vii-s3-n3-exa-1 .statement}

Nhóm tuyến tính tổng quát.

Cho $A$ là đại số $M_n(K)$. Nhóm $A^*$ gồm các phần tử khả nghịch của $A$ chính là nhóm tuyến tính tổng quát $\mathbf{GL}(n, K)$. Với mọi $X \in A$, chuẩn rút gọn $\operatorname{Nrd}_{A/K}(X)$ là $\det X$; do đó $N_{A/K}(X) = (\det X)^n$ (Alg., Ch. VIII, §12, No. 3, Mệnh đề 8; cf. A, III, §9, No. 3, Ví dụ 3). Vì $X \mapsto {}^t X$ là một đẳng cấu của $A$ lên đại số đối,

$$
N_{A^0/K}(X) = N_{A/K}({}^t X) = \det ({}^t X)^n = (\det X)^n.
$$

Khi đó, Mệnh đề 16 của §1, No. 11 chứng minh rằng độ đo

$$
\operatorname{mod}(\det X)^{-n} \cdot \bigotimes_{i,j} dx_{ij} \quad (X = (x_{ij}))
$$

là một độ đo Haar trái và phải trên $\mathbf{GL}(n, K)$.

Để xác định các độ đo bất biến tương đối trên $\mathbf{GL}(n, K)$, ta sẽ dựa vào bổ đề sau:

#### Bổ đề 5 {#int-vii-s3-lem-5 .statement}

Các biểu diễn liên tục của $\mathbf{GL}(n, K)$ trong $\mathbf{C}^*$ là các ánh xạ có dạng $X \mapsto \chi(\det X)$, trong đó $\chi$ là một biểu diễn liên tục của $K^*$ trong $\mathbf{C}^*$.

Một ánh xạ như vậy hiển nhiên là một biểu diễn liên tục của $\mathbf{GL}(n, K)$ trong $\mathbf{C}^*$. Ngược lại, giả sử rằng $\psi$ là một biểu diễn liên tục của $\mathbf{GL}(n, K)$ trong $\mathbf{C}^*$. Với $x \in K^*$, đặt

$$
\tilde{x} = \begin{pmatrix}
x & & \\
& 1 & 0 \\
& & 1 \\
0 & \cdots & 1
\end{pmatrix}
$$

và $\chi(x) = \psi(\widetilde{x})$. Khi đó, với mọi ma trận $X \in \mathbf{GL}(n, K)$, ta có $(\det X^{-1}) \sim \cdot X \in \mathbf{SL}(n, K)$. Vì $\mathbf{SL}(n, K)$ là nhóm giao hoán tử của $\mathbf{GL}(n, K)$ (A, III, §8, No. 9, Hệ quả của Mệnh đề 17), $\psi((\det X^{-1}) \sim \cdot X) = 1$, do đó
$$
\psi(X) = \psi((\det X) \sim) = \chi(\det X).
$$
Điều này đã được thiết lập, Hệ quả 1 của Mệnh đề 10 của §1, No. 8 chứng minh rằng các độ đo bất biến tương đối trên $\mathbf{GL}(n, K)$, sai khác một nhân tử hằng, là các độ đo có dạng
$$
(4) \quad \chi(\det X) \cdot \bigotimes_{ij} dx_{ij} \qquad (X = (x_{ij})),
$$
trong đó $\chi$ là một biểu diễn liên tục của $K^*$ trong $\mathbf{C}^*$.

**Ví dụ 2. — Nhóm affine.**
Với mọi $X \in \mathbf{GL}(n, K)$ và mọi $x \in K^n$, đặt $(X, x)$ là ánh xạ tuyến tính affine $\xi \mapsto X\xi + x$ trong $K^n$. Tập hợp các $(X, x)$ là nhóm affine $G$ của $K^n$ (A, II, §9, No. 4). Tập hợp $T$ các phép tịnh tiến là một nhóm con chuẩn đóng của $G$, đẳng cấu chính tắc với $K^n$; mặt khác, $\mathbf{GL}(n, K)$ là một nhóm con đóng của $G$, và $G$ là tích nửa trực tiếp của $\mathbf{GL}(n, K)$ và $T = K^n$. Trang bị cho $G$ tôpô (địa phương compact) sao cho $G$ là tích nửa trực tiếp tôpô của $\mathbf{GL}(n, K)$ và $T$ (GT, III, §2, No. 10). Ta có
$$
(X, x) = (1, x) \cdot (X, 0).
$$
Mặt khác, nếu $X \in \mathbf{GL}(n, K)$ và $x \in T$ thì, với mọi $\xi \in K^n$,
$$
(X, 0)(1, x)(X, 0)^{-1}\xi = X(X^{-1}\xi + x) = \xi + Xx = (1, Xx)\xi,
$$
do đó tự đẳng cấu $(1, x) \mapsto (X, 0)(1, x)(X, 0)^{-1}$ của $T$ có môđun $\mod(\det X)$ (§1, No. 10, Prop. 15). Theo Ví dụ 1 và §2, No. 9, *Nhận xét*, độ đo
$$
(5) \quad \mod(\det X)^{-n-1} \cdot \left( \bigotimes_{ij} dx_{ij} \right) \otimes \left( \bigotimes_i dx_i \right) \qquad (X = (x_{ij}), \ x = (x_i))
$$
là một độ đo Haar trái trên $G$. Mặt khác, theo Mệnh đề 14 của §2, No. 9,
$$
\Delta_G((X, x)) = \Delta_{\mathbf{GL}(n, K)}(X) \Delta_{K^n}(x) (\mod \det X)^{-1},
$$
hay
$$
(6) \quad \Delta_G((X, x)) = \mod(\det X^{-1}).
$$

Do đó, một độ đo Haar phải trên $G$ được cho bởi

$$
(\mod \det X)^{-n} \cdot \left( \bigotimes_{ij} dx_{ij} \right) \otimes \left( \bigotimes_i dx_i \right).
$$

**Ví dụ 3. — Nhóm tam giác ngặt.**

Cho $[1, n]$ là tập hợp các số nguyên $m$ sao cho $1 \leq m \leq n$. Cho $J$ là một tập con của $[1, n] \times [1, n]$ thỏa mãn các điều kiện sau:
1) nếu $(i, j) \in J$ thì $i < j$;
2) nếu $(i, j) \notin J$ thì, với mọi số nguyên $k$ sao cho $i < k < j$, ít nhất một trong hai cặp $(i, k)$ và $(k, j)$ không thuộc $J$.

Cho $T_J$ là tập hợp các ma trận $Z = (z_{ij})_{1 \leq i \leq n, 1 \leq j \leq n}$ với các phần tử trong $K$, sao cho $z_{ii} = 1$, và $z_{ij} = 0$ nếu $i \neq j$ và $(i, j) \notin J$. Đây là một tập con đóng của $\mathbf{GL}(n, K)$. Ánh xạ $Z \mapsto (z_{ij})_{(i, j) \in J}$ là một phép đồng phôi của $T_J$ lên $K^s$ (trong đó $s$ là số phần tử của $J$). Nếu $Z' = (z'_{ij}) \in T_J$, thì $Z'Z = (z''_{ij})$ với

$$
z''_{ij} = z_{ij} + z'_{ij} + \sum_{i < h < j} z'_{ih} z_{hj} \quad \text{với } i < j,
$$
$$
z''_{ij} = 0 \text{ với } i > j, \quad z''_{ii} = 1,
$$

do đó $Z'Z \in T_J$. Nếu $T_J$ được đồng nhất với $K^s$, thì ánh xạ $Z \mapsto Z'Z$ (với $Z'$ cố định) được đồng nhất với một ánh xạ affine, và định thức của nó là 1, như thấy được bằng cách sắp thứ tự các cặp $(i, j) \in J$ theo thứ tự từ điển và áp dụng bổ đề sau:

**Bổ đề 6. — Cho $L$ là một tập hợp hữu hạn được sắp thứ tự toàn phần. Với mỗi $\lambda \in L$, cho $V_\lambda$ là một môđun tự do có số chiều hữu hạn trên một vành giao hoán $k$; với $\lambda, \mu$ trong $L$ sao cho $\lambda \leq \mu$, cho $f_{\lambda \mu} \in \mathrm{Hom}_k(V_\mu, V_\lambda)$. Khi đó ánh xạ tuyến tính
$$
(v_\lambda)_{\lambda \in L} \mapsto \left( \sum_{\mu \geq \lambda} f_{\lambda \mu}(v_\mu) \right)_{\lambda \in L},
$$
từ $\prod_{\lambda \in L} V_\lambda$ vào $\prod_{\lambda \in L} V_\lambda$, có định thức $\prod_{\lambda \in L} \det f_{\lambda \lambda}$.

Ta quy ngay về trường hợp $L$ là một khoảng của các số nguyên, và khi đó bổ đề suy ra từ A, III, §8, No. 6, công thức (31).

Nếu $Z \in T_J$, khi đó ta thấy rằng tồn tại $Z' \in T_J$ sao cho $Z'Z = I_n$, do đó $Z' = Z^{-1}$. Vậy, $T_J$ là một nhóm con đóng của $\mathbf{GL}(n, K)$. Mặt khác, Mệnh đề 15 của §1, No. 10 cho thấy rằng độ đo

$$
\bigotimes_{(i, j) \in J} dz_{ij}
$$

là một độ đo Haar trái trên $T_J$. Bằng cách tính $ZZ'$ ta thấy theo cùng cách rằng độ đo này là một độ đo Haar phải trên $T_J$.

Có một kết quả tương tự nếu, trong định nghĩa của $T_J$, vai trò của các hàng và các cột được hoán đổi.

Khi $J$ là tập hợp các cặp $(i, j)$ sao cho $i < j$, nhóm $T_J$ được gọi là nhóm tam giác ngặt trên cấp $n$ trên $K$, và được ký hiệu là $T_1(n, K)$. Chuyển vị của nó được gọi là nhóm tam giác ngặt dưới.

#### Ví dụ 4 {#int-vii-s3-n3-exa-4 .statement}

— *Nhóm tam giác lớn.*

Cho $n_1, \ldots, n_r$ là các số nguyên $\geqslant 1$. Đặt $p_k = n_1 + \ldots + n_{k-1}$ và $n = p_{r+1} = n_1 + \cdots + n_r$. Gọi $I_k$ là tập hợp các số nguyên $j$ sao cho $p_k < j \leqslant p_{k+1}$, và $J$ là hợp của các $I_k \times I_l$ với $k < l$. Gọi $G$ là nhóm con đóng của $\mathbf{GL}(n, K)$ gồm các phần tử là các ma trận $(Z_{kl})_{1 \leqslant k \leqslant r, 1 \leqslant l \leqslant r}$ sao cho:
1) mỗi $Z_{kl}$ là một ma trận $(z_{ij})_{i \in I_k, j \in I_l}$ gồm các phần tử của $K$, với $n_k$ hàng và $n_l$ cột;
2) $Z_{kl} = 0$ với $k > l$;
3) $Z_{kk} \in \mathbf{GL}(n_k, K)$ với $1 \leqslant k \leqslant r$.

Công thức nhân khối

$$
\begin{pmatrix}
Z_{11} & 0 & \ldots & 0 \\
0 & Z_{22} & \ldots & 0 \\
\vdots & \vdots & \ddots & \vdots \\
0 & 0 & \ldots & Z_{rr}
\end{pmatrix}
\begin{pmatrix}
1 & Z_{12} & \ldots & Z_{1r} \\
0 & 1 & \ldots & Z_{2r} \\
\vdots & \vdots & \ddots & \vdots \\
0 & 0 & \ldots & 1
\end{pmatrix}
$$

$$
= \begin{pmatrix}
Z_{11} & Z_{11}Z_{12} & \ldots & Z_{11}Z_{1r} \\
0 & Z_{22} & \ldots & Z_{22}Z_{2r} \\
\vdots & \vdots & \ddots & \vdots \\
0 & 0 & \ldots & Z_{rr}
\end{pmatrix}
$$

chỉ ra rằng $G$ là tích nửa trực tiếp tôpô của nhóm con $D$ gồm các phần tử $(Z_{kl}) \in G$ sao cho $Z_{kl} = 0$ với $k \neq l$ và nhóm con $T_J$ của Ví dụ 3. Hơn nữa, $D$ đẳng cấu với tích trực tiếp của các nhóm $\mathbf{GL}(n_k, K)$ với $1 \leqslant k \leqslant r$.

Gọi $J'$ là tập hợp các cặp $(j, i)$ sao cho $(i, j) \in J$ và gọi $H$ là tập hợp các cặp $(i, j) \in [1, n] \times [1, n]$ không thuộc $J'$. Gọi $Z' = (z_{ij})_{1 \leqslant i \leqslant n, 1 \leqslant j \leqslant n}$ là một phần tử của $G$. Theo Mệnh đề 14 của §2, No. 9 và các Ví dụ 1 và 3 ở trên, ta thu được một độ đo Haar trái trên $G$ bằng cách lấy ảnh của độ đo

$$
\bigotimes_{k=1}^r ((\mathrm{mod}\ \det Z_{kk})^{-n_k} \cdot \bigotimes_{i,j \in I_k} dz_{ij}) \otimes \left( \bigotimes_{(i,j) \in J} dz_{ij} \right)
$$

qua ánh xạ

$$
((Z_{kk}), (Z_{kl})) \mapsto \begin{pmatrix}
Z_{11} & Z_{11}Z_{12} & \ldots & Z_{11}Z_{1r} \\
0 & Z_{22} & \ldots & Z_{22}Z_{2r} \\
\vdots & \vdots & \ddots & \vdots \\
0 & 0 & \ldots & Z_{rr}
\end{pmatrix}.
$$

Bây giờ, xét với $k < l$, không gian vectơ của các ma trận $Z_{kl} = (z_{ij})_{i \in I_k, j \in I_l}$. Nó là tổng trực tiếp của $n_l$ không gian con $M_j$ ($j \in I_l$) tạo bởi các ma trận sao cho $z_{ih} = 0$ với $h \neq j$. Mỗi không gian con này $M_j$ là ổn định đối với ánh xạ $Z_{kl} \mapsto Z_{kk}Z_{kl}$, và hạn chế của ánh xạ này trên $M_j$ có ma trận $Z_{kk}$. Do đó (\S 1, No. 10, Mệnh đề 15) ảnh của độ đo $\bigotimes_{i \in I_k, j \in I_l} dz_{ij}$ qua ánh xạ $Z_{kl} \mapsto Z_{kk}Z_{kl}$ là

$$
(\operatorname{mod} \det Z_{kk})^{-n_l} \cdot \bigotimes_{i \in I_k, j \in I_l} dz_{ij}.
$$

Một độ đo Haar trái trên $G$ do đó được cho bởi

$$
\prod_{k=1}^r (\operatorname{mod} \det Z_{kk})^{-q_k} \cdot \bigotimes_{(i,j) \in H} dz_{ij}
$$

với $q_k = \sum_{k \leq l \leq r} n_l = n - p_k$.

Ta hãy tính *môđun* của $G$, một lần nữa sử dụng Mệnh đề 14 của \S 2. Các nhóm $D$ và $T_J$ là đơn môđula; mặt khác:

$$
\begin{pmatrix}
Z_{11} & 0 & \ldots & 0 \\
0 & Z_{22} & \ldots & 0 \\
\vdots & \vdots & \ddots & \vdots \\
0 & 0 & \ldots & Z_{rr}
\end{pmatrix}
\begin{pmatrix}
1 & Z_{12} & \ldots & Z_{1r} \\
0 & 1 & \ldots & Z_{2r} \\
\vdots & \vdots & \ddots & \vdots \\
0 & 0 & \ldots & 1
\end{pmatrix}
\begin{pmatrix}
Z_{11} & 0 & \ldots & 0 \\
0 & Z_{22} & \ldots & 0 \\
\vdots & \vdots & \ddots & \vdots \\
0 & 0 & \ldots & Z_{rr}
\end{pmatrix}^{-1}
$$
$$
= \begin{pmatrix}
1 & Z'_{12} & \ldots & Z'_{1r} \\
0 & 1 & \ldots & Z'_{2r} \\
\vdots & \vdots & \ddots & \vdots \\
0 & 0 & \ldots & 1
\end{pmatrix},
$$

trong đó $Z'_{kl} = Z_{kk}Z_{kl}Z_{ll}^{-1}$. Tính đến Ví dụ 3, và Mệnh đề 15 của \S 1, No. 10, và lập luận như trên, ta thấy rằng nếu $X = \operatorname{diag}(Z_{11}, \ldots, Z_{rr}) \in D$ thì môđun của tự đẳng cấu $Z \mapsto X^{-1}ZX$ của $T_J$ là

$$
\prod_{k < l} (\operatorname{mod} \det Z_{kk})^{-n_l} (\operatorname{mod} \det Z_{ll})^{n_k},
$$

do đó

$$
\Delta_G(Z) = \prod_{k=1}^r (\operatorname{mod} \det Z_{kk})^{n+n_k-2q_k}.
$$

Nhóm chuyển vị $G'$ của $G$ được nghiên cứu theo cùng một cách. Đối với $G'$, ta tìm được độ đo Haar trái

$$
\prod_{k=1}^r (\operatorname{mod} \det Z_{kk})^{-p_{k+1}} \cdot \bigotimes_{(j,i) \in \mathbb{H}} dz_{ij},
$$

và môđun

$$
\prod_{k=1}^r (\operatorname{mod} \det Z_{kk})^{n+n_k-2p_{k+1}}.
$$

Nếu đặc biệt lấy $n_1 = \ldots = n_r = 1$, ta tìm được nhóm $G$ là nhóm $T(n, K)^*$ của các phần tử khả nghịch của đại số con của $M_n(K)$ tạo bởi các ma trận $X = (x_{ij})$ sao cho $x_{ij} = 0$ với $i > j$. Đại số này, mà ta sẽ ký hiệu là $T(n, K)$, được gọi là *đại số tam giác trên*, và nhóm $T(n, K)^*$ được gọi là *nhóm tam giác lớn trên* cấp $n$ trên $K$. Các công thức trước đó khi ấy có dạng sau: một độ đo Haar trái trên $T(n, K)^*$ là

$$(9\ bis)$$
$$
\prod_{i=1}^n (\operatorname{mod} z_{ii})^{i-n-1} \cdot \bigotimes_{i \leq j} dz_{ij} \quad (Z = (z_{ij}))
$$

và môđun của $T(n, K)^*$ là

$$(10\ bis)$$
$$
\Delta_{T(n,K)^*}(Z) = \prod_{i=1}^n (\operatorname{mod} z_{ii})^{2i-n-1} \quad (Z = (z_{ij})).
$$

Đối với chuyển vị của $T(n, K)^*$, hay *nhóm tam giác lớn dưới*, ta tìm được độ đo Haar trái

$$
\prod_{i=1}^n (\operatorname{mod} z_{ii})^{-i} \cdot \bigotimes_{i \geq j} dz_{ij},
$$

và môđun

$$
\prod_{i=1}^n (\operatorname{mod} z_{ii})^{n+1-2i}.
$$

#### Nhận xét {#int-vii-s3-n3-rem-1 .statement}

Nhóm $T(n, K)^*$ là một nhóm con đóng của $\mathbf{GL}(n, K)$, và $\Delta_{T(n, K)^*}((z_{ij})) = \prod_{i=1}^n (\operatorname{mod} z_{ii})^{2i-n-1}$. Ta đã thấy trong Ví dụ 1 rằng $\Delta_{\mathbf{GL}(n, K)} = 1$. Nếu $n > 1$, hàm
$$
\Delta_{T(n, K)^*}/\Delta_{\mathbf{GL}(n, K)}
$$
trên $T(n, K)^*$ không thể được mở rộng thành một biểu diễn liên tục của $\mathbf{GL}(n, K)$ trong $\mathbf{C}^*$ (bởi vì một biểu diễn như vậy sẽ bằng 1 trên $\mathbf{SL}(n, K)$ theo Bổ đề 5, trong khi $\operatorname{mod}(z_{11})^{1-n} \neq 1$ với $z_{11}$ được chọn thích hợp). Suy ra rằng không gian thuần nhất $\mathbf{GL}(n, K)/T(n, K)^*$ *không nhận độ đo bất biến tương đối* nếu $n > 1$ (\S 2, No. 6, Hệ quả 1 của Định lý 3).

Không gian thuần nhất này có thể được đồng nhất, với $n = 2$, với *đường xạ ảnh* trên $K$. Thật vậy, cho $(e_1, e_2)$ là cơ sở chính tắc của $K^2$. Nhóm $\mathbf{GL}(2, K)$ tác động bắc cầu trên tập hợp các đường của $K^2$ với 0 bị loại bỏ, và nhóm ổn định của $Ke_1 - \{0\}$ là $T(2, K)^*$.

#### Ví dụ 5 {#int-vii-s3-n3-exa-5 .statement}

— *Nhóm tam giác đặc biệt.*
Ta xét lại các ký hiệu ở đầu Ví dụ 4, và xét nhóm con $G_1 = G \cap \mathbf{SL}(n, K)$. Nhóm con này là tích nửa trực tiếp tôpô của nhóm $D_1 = D \cap \mathbf{SL}(n, K)$ với $T_J$. Nhóm $D_1$ có một nhóm con chuẩn $A$ đẳng cấu với $\mathbf{SL}(n_r, K)$, cụ thể là nhóm con gồm các phần tử $\operatorname{diag}(Z_{kk})$ với $Z_{kk} = 1$ khi $k < r$. Đồng cấu
$$
\varphi : \operatorname{diag}(Z_{11}, \ldots, Z_{rr}) \mapsto (Z_{11}, \ldots, Z_{r-1, r-1})
$$
của $D_1$ vào $\mathbf{GL}(n_1, K) \times \cdots \times \mathbf{GL}(n_{r-1}, K)$ là toàn ánh và có hạt nhân $A$. Mặt khác, $\varphi$ là liên tục. Theo Bổ đề 2 của Phụ lục I, $D_1/A$ có thể được đồng nhất với $\mathbf{GL}(n_1, K) \times \cdots \times \mathbf{GL}(n_{r-1}, K)$. Ta ký hiệu $\mu$ là độ đo Haar của $A$ (xem Ví dụ 6) và
$$
\alpha = \bigotimes_{k=1}^{r-1} \left( (\operatorname{mod} \det Z_{kk})^{-n_k} \cdot \bigotimes_{i,j \in I_k} dz_{ij} \right) \otimes' d\mu(Z_{rr})
$$
là độ đo Haar trên $D_1$ sao cho
$$
\alpha/\mu = \bigotimes_{k=1}^{r-1} \left( (\operatorname{mod} \det Z_{kk})^{-n_k} \cdot \bigotimes_{i,j \in I_k} dz_{ij} \right)
$$
(\S 2, No. 7, Mệnh đề 10). Khi đó, như trong Ví dụ 4, ta chỉ ra rằng một độ đo Haar trái trên $G_1$ được cho bởi
$$
\operatorname{mod} \left( \prod_{k=1}^{r-1} (\det Z_{kk})^{n_k-q_k} \right)
$$
$$
\cdot \left[ \bigotimes_{k=1}^{r-1} ((\operatorname{mod} \det Z_{kk})^{-n_k} \cdot \bigotimes_{i,j \in I_k} dz_{ij}) \otimes' d\mu(Z_{rr}) \right] \otimes \bigotimes_{(i,j) \in J} dz_{ij}.
$$

Vì $G_1$ là chuẩn trong $G$, *môđun* của $G_1$ là hạn chế của môđun của $G$ (\S 2, No. 7, Mệnh đề 10 b)).

Nếu $n_r = 1$, nhóm con $A$ thu gọn thành phần tử trung hòa, và một độ đo Haar trái trên $G$ là

$$
\operatorname{mod}\left( \prod_{k=1}^{r-1} (\det Z_{kk})^{-q_k} \right) \cdot \bigotimes_{k=1}^{r-1} \left( \bigotimes_{i,j \in I_k} dz_{ij} \right) \otimes \bigotimes_{(i,j) \in J} dz_{ij}.
$$

Nếu lấy $n_1 = n_2 = \ldots = n_r = 1$, nhóm $G_1$ thu được được gọi là *nhóm tam giác đặc biệt trên* và chuyển vị $G'_1$ của nó được gọi là *nhóm tam giác đặc biệt dưới*. Một độ đo Haar trái trên $G_1$ là

$$
\operatorname{mod} \left( \prod_{i=1}^{n-1} z_{ii}^{i-n-1} \right) \cdot \left( \bigotimes_{i=1}^{n-1} dz_{ii} \right) \otimes \left( \bigotimes_{1 \leq i < j \leq n} dz_{ij} \right)
$$
và môđun của $G_1$ là
$$
\operatorname{mod} \left( \prod_{i=1}^{n-1} z_{ii}^{2i-2n} \right).
$$
Đối với $G'_1$, ta tìm được tương tự độ đo Haar trái
$$
\operatorname{mod} \left( \prod_{i=1}^{n-1} z_{ii}^{n-i-1} \right) \cdot \left( \bigotimes_{i=1}^{n-1} dz_{ii} \right) \otimes \left( \bigotimes_{1 \leq j < i \leq n} dz_{ij} \right)
$$
và môđun
$$
\operatorname{mod} \left( \prod_{i=1}^{n-1} z_{ii}^{2n-2i} \right).
$$

#### Ví dụ 6 {#int-vii-s3-n3-exa-6 .statement}

— *Nhóm tuyến tính đặc biệt.*
Các nhóm con đóng $T_1(n, K)$ và ${}^t(T(n, K)^*)$ của $\mathbf{GL}(n, K)$ có giao $\{e\}$. Do đó ánh xạ $(M, N) \mapsto M \cdot N$ là một song ánh liên tục $\varphi$ của $T_1(n, K) \times {}^t(T(n, K)^*)$ lên một tập con $\Omega$ của $\mathbf{GL}(n, K)$.

#### Bổ đề 7 {#int-vii-s3-lem-7 .statement}

— a) *Cho $U = (u_{ij}) \in \mathbf{GL}(n, K)$. Để $U \in \Omega$, điều kiện cần và đủ là $\det(u_{ij})_{k \leq i, j \leq n} \neq 0$ với $k = 2, 3, \ldots, n$ là đúng.*
b) $\Omega$ *là một tập con mở của $\mathbf{GL}(n, K)$*.
c) *Ánh xạ $\varphi$ là một đồng phôi của $T_1(n, K) \times {}^t(T(n, K)^*)$ lên $\Omega$*.

Để $U \in \Omega$, điều kiện cần và đủ là tồn tại một $Z = (z_{ij}) \in T_1(n, K)$ sao cho $ZU \in {}^t(T(n, K))$ (khi đó tất nhiên

$ZU \in {}^t(T(n, K)^*)$ vì $U$ và $Z$ khả nghịch). Theo điều đã thấy trước đây, nếu $Z$ tồn tại thì nó là duy nhất. Do đó, để $U \in \Omega$, điều kiện cần và đủ là hệ tuyến tính

$$
\sum_{k=1}^n z_{ik} u_{kj} = 0 \qquad (1 \leq i < j \leq n)
$$

(với $(z_{ij}) \in T_1(n, K)$) có một nghiệm duy nhất. Bây giờ, hệ này có thể được viết

$$
(13) \qquad \sum_{k=i+1}^n z_{ik} u_{kj} = -u_{ij} \qquad (1 \leq i < j \leq n).
$$

Với $i$ cố định, ta có một hệ gồm $n-i$ phương trình với các ẩn $z_{i,i+1}, z_{i,i+2}, \ldots, z_{i,n}$; để các hệ này có nghiệm duy nhất, điều kiện cần và đủ là

$$
\det(u_{kj})_{i+1 \leq k \leq n,\ i+1 \leq j \leq n} \neq 0
$$

với $i = 1, 2, \ldots, n-1$. Điều này chứng minh a). Từ đó suy ra rằng $\Omega$ là mở trong $\mathbf{GL}(n, K)$. Mặt khác, khi giải hệ (13) bằng các công thức Cramer, ta thu được các $z_{ij}$ như những hàm hữu tỉ của các $u_{ij}$ với mẫu khác không trên $\Omega$, do đó $Z$ phụ thuộc liên tục vào $U$ trong $\Omega$, điều này chứng minh c).

Bây giờ cho $G'_1 \subset {}^t(T(n, K)^*)$ là nhóm tam giác đặc biệt dưới. Ánh xạ $(M, N) \mapsto M \cdot N$ là một song ánh liên tục $\psi$ của $T_1(n, K) \times G'_1$ lên một tập con $\Omega'$ của $\mathbf{SL}(n, K)$.

**Bổ đề 8. — a)** *Cho $U = (u_{ij}) \in \mathbf{SL}(n, K)$. Để $U \in \Omega'$, điều kiện cần và đủ là $\det(u_{ij})_{k \leq i, j \leq n} \neq 0$ với $k = 2, 3, \ldots, n$.*

b) $\Omega'$ *là một tập con mở của $\mathbf{SL}(n, K)$*.

c) *Ánh xạ $\psi$ là một đồng phôi của $T_1(n, K) \times G'_1$ lên $\Omega'$*.

Vì, cho $M \in T_1(n, K)$ và $N \in {}^t(T(n, K)^*)$. Để $M \cdot N \in \mathbf{SL}(n, K)$, điều kiện cần và đủ là $N \in G'_1$. Do đó $\Omega' = \mathbf{SL}(n, K) \cap \Omega$ và Bổ đề 8 suy ra ngay từ Bổ đề 7.

**Mệnh đề 6. — a)** *Nhóm $\mathbf{SL}(n, K)$ là đơn môđula.*

b) *Cho $\mu_1$ và $\mu_2$ lần lượt là các độ đo Haar trái trên nhóm tam giác ngặt trên $T_1(n, K)$ và nhóm tam giác đặc biệt dưới $G'_1$. Ảnh của $\mu_1 \otimes \mu_2$ qua đồng phôi $(M, N) \mapsto M \cdot N^{-1}$ của $T_1(n, K) \times G'_1$ lên $\Omega'$ là hạn chế trên $\Omega'$ của một độ đo Haar trên $\mathbf{SL}(n, K)$*.

c) *Phần bù của $\Omega'$ trong $\mathbf{SL}(n, K)$ là không đáng kể đối với độ đo Haar của $\mathbf{SL}(n, K)$*.

Nhóm $\mathbf{GL}(n, K)$ là đơn môđula (Ví dụ 1), và $\mathbf{SL}(n, K)$ là một nhóm con chuẩn tắc của $\mathbf{GL}(n, K)$, do đó là đơn môđula (\S 2, No. 7, Mệnh đề 10 b)). Mệnh đề b) suy ra từ a), Bổ đề 8, và Mệnh đề 13 của \S 2, No. 9. Ta chứng minh c). Theo Bổ đề 8 a), chỉ cần chứng minh điều sau: nếu $p((u_{ij})_{1 \leq i,j \leq n})$ là một đa thức, không đồng nhất bằng không trên $\mathbf{SL}(n, K)$, thì tập hợp E của các $U \in \mathbf{SL}(n, K)$ sao cho $p(U) = 0$ là không đáng kể đối với độ đo Haar. Xét \S 1, No. 10, Hệ quả của Mệnh đề 13, tôpô của $\mathbf{SL}(n, K)$ có một cơ sở đếm được. Vì vậy chỉ cần chứng minh rằng với mọi $U_0 \in E$, tồn tại một lân cận của $U_0$ trong $\mathbf{SL}(n, K)$ mà giao của nó với E là không đáng kể; hay tương đương là tồn tại một lân cận W của I trong $\mathbf{SL}(n, K)$ sao cho $U_0^{-1}E \cap W$ là không đáng kể. Ta lấy $W = \Omega'$. Theo b), mọi thứ quy về việc chỉ ra rằng tập hợp các cặp $(M, N) \in T_1(n, K) \times G'_1$ sao cho $p(U_0 MN) = 0$ là không đáng kể đối với $\mu_1 \otimes \mu_2$. Theo các biểu thức của $\mu_1$ và $\mu_2$ (được tính trong các Ví dụ 3 và 5), điều này suy ra từ bổ đề sau:

#### Bổ đề 9 {#int-vii-s3-lem-9 .statement}

*Cho $\psi$ là một đa thức $\neq 0$ của $K[X_1, \ldots, X_r]$. Trong không gian $K^r$, tập hợp N được xác định bởi $\psi(x_1, \ldots, x_r) = 0$ là không đáng kể đối với độ đo Haar.*

Ta lập luận bằng quy nạp theo $r$. Bổ đề là hiển nhiên đối với $r = 1$, vì khi đó N là một tập hợp hữu hạn. Nếu cần thiết, bằng cách thay đổi cách đánh số các biến, ta có thể giả sử rằng $\psi \notin K[X_1, \ldots, X_{r-1}]$; viết

$$
\psi(X_1, \ldots, X_r) = X_r^m \psi_0(X_1, \ldots, X_{r-1}) + \cdots + \psi_m(X_1, \ldots, X_{r-1})
$$

với $m > 0$ và $\psi_0 \neq 0$. Trong không gian $K^{r-1}$, gọi $N_0$ là tập hợp được xác định bởi $\psi_0(x_1, \ldots, x_{r-1}) = 0$, là không đáng kể theo giả thiết quy nạp. Với mọi $(x_1, \ldots, x_{r-1}) \notin N_0$, tập hợp các $x_r \in K$ sao cho $(x_1, \ldots, x_{r-1}, x_r) \in N$ là hữu hạn, do đó là không đáng kể. Vì $K^r$ là đếm được tại vô cực (\S 1, No. 10, Hệ quả của Mệnh đề 13), $N \cap [(K^{r-1} - N_0) \times K]$ là không đáng kể trong $K^r$ (Ch. V, \S 8, No. 2, Mệnh đề 4). Do đó N là không đáng kể.

#### Ví dụ 7 {#int-vii-s3-n3-exa-7 .statement}

*Phân tích Iwasawa của $\mathbf{GL}(n, K)$.*

Trong ví dụ này, K ký hiệu một trong các trường $\mathbf{R}, \mathbf{C}, \mathbf{H}$. Nếu $\lambda \in K$, $\overline{\lambda}$ được định nghĩa là bằng $\lambda$ nếu $K = \mathbf{R}$, và là liên hợp của $\lambda$ nếu $K = \mathbf{C}$ hoặc $\mathbf{H}$. Cho E là một không gian vectơ phải trên K có chiều $n$, và cho $\Phi$ là một dạng Hermit dương không suy biến trên E.

#### Bổ đề 10 {#int-vii-s3-lem-10 .statement}

*Cho $(f_1, f_2, \ldots, f_n)$ là một cơ sở của E.*
a) *Tồn tại duy nhất một cơ sở trực chuẩn $(e_1, e_2, \ldots, e_n)$ của E sao cho $f_i = e_1 \alpha_{i1} + e_2 \alpha_{i2} + \cdots + e_i \alpha_{ii}$ ($i = 1, 2, \ldots, n$) với $\alpha_{ii} > 0$ với mọi $i$.
b) *Với $\Phi$ cố định, các $e_i$ và $\alpha_{ij}$ phụ thuộc liên tục vào $(f_1, \ldots, f_n) \in E^n$.*

Cho $E_i = f_1 K + f_2 K + \cdots + f_i K$, có chiều $i$. Gọi $g_i$ là một phần tử khác không của $E_i$ trực giao với $E_{i-1}$ và sao cho $\Phi(g_i, g_i) = 1$. Theo quy nạp theo $i$, ta thấy rằng $(g_1, \ldots, g_i)$ là một cơ sở trực chuẩn của $E_i$. Đặc biệt, $(g_1, \ldots, g_n)$ là một cơ sở trực chuẩn của $E$. Đặt $\lambda_i = \Phi(f_i, g_i)$. Vì $f_i \notin E_{i-1}$, ta có $\lambda_i \neq 0$. Đặt $e_i = g_i |\lambda_i| \lambda_i^{-1}$. Khi đó

$$
\Phi(e_i, e_i) = |\lambda_i|^2 \overline{\lambda_i}^{-1} \Phi(g_i, g_i) \lambda_i^{-1} = 1,
$$

do đó $(e_1, \ldots, e_i)$ cũng là một cơ sở trực chuẩn của $E_i$; hơn nữa, $\Phi(e_i, f_i) = |\lambda_i| \overline{\lambda_i}^{-1} \Phi(g_i, f_i) = |\lambda_i| > 0$, do đó các $e_i$ có các tính chất của a). Gọi $(e'_1, \ldots, e'_n)$ là một cơ sở trực chuẩn khác của $E$ với cùng các tính chất. Theo quy nạp theo $i$, ta thấy rằng $(e'_1, \ldots, e'_i)$ phải là một cơ sở của $E_i$, do đó $e'_i = e_i \mu_i$ với một $\mu_i \in \mathbf{K}$. Khi đó

$$
1 = \Phi(e'_i, e'_i) = \overline{\mu_i} \Phi(e_i, e_i) \mu_i = \overline{\mu_i} \mu_i ,
$$

và $0 < \Phi(e'_i, f_i) = \overline{\mu_i} \Phi(e_i, f_i)$, do đó $\mu_i > 0$ và $\mu_i^2 = 1$, vậy $\mu_i = 1$, do đó a). Giả sử đã chứng minh rằng các $e_i$ và $\alpha_{ij}$ phụ thuộc liên tục vào $(f_1, \ldots, f_n)$ đối với $i < i_0$, và ta chứng minh rằng $e_{i_0}$ và các $\alpha_{i_0 j}$ phụ thuộc liên tục vào $(f_1, \ldots, f_n)$. Với $j < i_0$, $\overline{\alpha}_{i_0 j} = \Phi(f_{i_0}, e_j)$ phụ thuộc liên tục vào $(f_1, \ldots, f_n)$ theo giả thiết quy nạp. Mặt khác,

$$
\Phi(f_{i_0}, f_{i_0}) = |\alpha_{i_0 1}|^2 + |\alpha_{i_0 2}|^2 + \cdots + |\alpha_{i_0, i_0 - 1}|^2 + \alpha_{i_0 i_0}^2 ,
$$

do đó $\alpha_{i_0 i_0}$ phụ thuộc liên tục vào $(f_1, \ldots, f_n)$. Vì vậy

$$
e_{i_0} = (f_{i_0} - e_1 \alpha_{i_0 1} - \cdots - e_{i_0 - 1} \alpha_{i_0, i_0 - 1}) \alpha_{i_0 i_0}^{-1}
$$

phụ thuộc liên tục vào $(f_1, \ldots, f_n)$.

Kể từ đây, cho $E = K^n$ và lấy cho $\Phi$ dạng

$$
\overline{x}_1 y_1 + \cdots + \overline{x}_n y_n .
$$

Nhắc lại rằng $\mathbf{U}(n, \mathbf{K})$ ký hiệu nhóm unita tương ứng. Ngay cả khi $\mathbf{K}$ không giao hoán, ta vẫn ký hiệu bởi $\mathbf{T}_1(n, \mathbf{K})$ nhóm các ma trận tam giác trên của $\mathbf{M}_n(\mathbf{K})$ có tất cả các phần tử đường chéo bằng 1.

#### Mệnh đề 7 {#int-vii-s3-prop-7 .statement}

*Cho $D_+^*$ là nhóm các ma trận đường chéo có các phần tử đường chéo $> 0$. Ánh xạ $(U, D, T) \mapsto UDT$ là một phép đồng phôi từ $\mathbf{U}(n, \mathbf{K}) \times D_+^* \times \mathbf{T}_1(n, \mathbf{K})$ lên $\mathbf{GL}(n, \mathbf{K})$.*

Cho $(\varepsilon_1, \ldots, \varepsilon_n)$ là cơ sở chính tắc của $K^n$. Cho $X \in \mathbf{GL}(n, K)$. Khi đó các $X \cdot \varepsilon_i = f_i$ tạo thành một cơ sở của E. Với cơ sở $(f_i)$ này, ta có thể liên kết một cơ sở $(e_i)$ như trong Bổ đề 10. Gọi $U$ là ma trận của tự đẳng cấu unita của E biến $\varepsilon_i$ thành $e_i$. Khi đó

$$
U^{-1} \cdot f_i = \varepsilon_1 \alpha_{i1} + \varepsilon_2 \alpha_{i2} + \cdots + \varepsilon_i \alpha_{ii}
$$

với $\alpha_{ii} > 0$ đối với $i = 1, 2, \ldots, n$. Do đó $X = UC$, trong đó $C$ là ma trận

$$
\begin{pmatrix}
\alpha_{11} & \alpha_{21} & \cdots & \alpha_{n1} \\
0 & \alpha_{22} & \cdots & \alpha_{n2} \\
\vdots & \vdots & \ddots & \vdots \\
0 & 0 & \cdots & \alpha_{nn}
\end{pmatrix}.
$$

Hơn nữa, $U$ và $C$ phụ thuộc liên tục vào X theo Bổ đề 10. Mặt khác, công thức (8) chỉ ra rằng $C$ có thể được viết dưới dạng $DT$ với $D \in \mathbf{D}_+^*$, $T \in \mathbf{T}_1(n, K)$, $D$ và $T$ phụ thuộc liên tục vào $C$. Tính duy nhất của phân tích $X = UDT$ suy ra từ tính duy nhất trong Bổ đề 10.

Phép đồng phôi của Mệnh đề 7 được gọi là *phân tích Iwasawa* của $\mathbf{GL}(n, K)$.

Nhóm $G = \mathbf{D}_+^* \cdot \mathbf{T}_1(n, K)$ là tập hợp các ma trận tam giác trên trên K có các phần tử đường chéo $> 0$. Ta đồng nhất phần tử $(z_{ij})$ của nhóm này với phần tử

$$
((z_{ii})_{1 \leq i \leq n}, (z_{ij})_{1 \leq i < j \leq n}) \in (\mathbf{R}_+^*)^n \times K^{n(n-1)/2}.
$$

Lập luận đúng như trong Ví dụ 4, ta tìm được độ đo Haar phải trên nhóm này là độ đo (khi $K = \mathbf{R}$)

$$
\left( \prod_{i=1}^n z_{ii}^{-i} \right) \cdot \left( \bigotimes_{i=1}^n dz_{ii} \right) \otimes \left( \bigotimes_{i < j} dz_{ij} \right).
$$

Sau đó áp dụng Mệnh đề 13 của §2, No. 9, ta thấy rằng nếu $\mathbf{GL}(n, K)$ được đồng nhất với $\mathbf{U}(n, K) \times G$ bởi ánh xạ $(U, S) \mapsto US$, một độ đo Haar trên $\mathbf{GL}(n, K)$ được cho bởi (khi $K = \mathbf{R}$)

$$
\left( \prod_{i=1}^n z_{ii}^{-i} \right) \cdot \alpha \otimes \left( \bigotimes_{i=1}^n dz_{ii} \right) \otimes \left( \bigotimes_{i < n} dz_{ij} \right),
$$

trong đó $\alpha$ biểu thị một độ đo Haar trên $\mathbf{U}(n, K)$.

#### Ví dụ 8 {#int-vii-s3-n3-exa-8 .statement}

Không gian các dạng Hermit.

Trong ví dụ này, K luôn biểu thị một trong các trường $\mathbf{R}, \mathbf{C}, \mathbf{H}$. Ta viết $\delta = \dim_{\mathbf{R}} K$ (do đó $\delta = 1, 2$ hoặc 4). Một dạng Hermit $\Phi$ trên không gian vectơ phải $K^n$ có thể được viết

$$
\Phi(x, y) = \Phi(x_1, \ldots, x_n, y_1, \ldots, y_n) = \sum_{i,j=1}^n \overline{x_i} h_{ij} y_j
$$

với $h_{ij} = \overline{h_{ji}}$ với mọi $i$ và $j$. Ta ký hiệu bởi $\mathfrak{H}$ không gian vectơ trên $\mathbf{R}$ được tạo bởi các ma trận Hermit của $M_n(K)$. Ánh xạ $(h_{ij}) \mapsto \Phi$ là một đẳng cấu của $\mathfrak{H}$ lên không gian vectơ các dạng Hermit trên $K^n$, nhờ đó ta sẽ đồng nhất hai không gian này. Gọi $\mathfrak{H}_+^* \subset \mathfrak{H}$ là tập hợp các dạng Hermit dương không suy biến trên $K^n$. Tập hợp $\mathfrak{H}_+^*$ là *lồi* trong $\mathfrak{H}$; thật vậy, nếu $\Phi_1, \Phi_2$ thuộc $\mathfrak{H}_+^*$ và nếu $\lambda, \mu$ là hai số $> 0$ sao cho $\lambda + \mu = 1$, thì rõ ràng $\lambda \Phi_1 + \mu \Phi_2$ là một dạng Hermit dương; mặt khác, nếu $(\lambda \Phi_1 + \mu \Phi_2)(x, x) = 0$, thì $\Phi_1(x, x) = \Phi_2(x, x) = 0$, do đó $x = 0$, vì vậy $\lambda \Phi_1 + \mu \Phi_2$ là không suy biến. Bây giờ ta chứng minh rằng $\mathfrak{H}_+^*$ là một tập con *mở* của $\mathfrak{H}$. Gọi S là tập hợp các $x = (x_1, \ldots, x_n) \in K^n$ sao cho $x_1 \overline{x}_1 + \cdots + x_n \overline{x}_n = 1$; đây là một tập con compact của $K^n$; nếu $\Phi \in \mathfrak{H}_+^*$, hàm $x \mapsto \Phi(x, x)$ là liên tục và $> 0$ trên S, do đó cận dưới của nó là $> 0$; nếu $\Phi' \in \mathfrak{H}$ đủ gần $\Phi$, thì suy ra $\Phi'(x, x) > 0$ với mọi $x \in S$, do đó $\Phi'$ là dương và không suy biến.

Nhóm tuyến tính tổng quát $\mathbf{GL}(n, K)$ tác động liên tục bên phải trên $\mathfrak{H}$ bởi $(X, \Phi) \mapsto \Phi \circ X$, nghĩa là bởi $(X, H) \mapsto t \overline{X} \cdot H \cdot X$, trong đó $H$ ký hiệu ma trận Hermit tương ứng với $\Phi$. Rõ ràng rằng $\mathfrak{H}_+^*$ ổn định dưới tác động của $\mathbf{GL}(n, K)$. Chính xác hơn, theo *Alg.*, Ch. IX, §6, No. 1, Hệ quả 1 của Định lý 1,$^1$ $\mathfrak{H}_+^*$ là quỹ đạo dưới $\mathbf{GL}(n, K)$ của dạng $\sum_{i=1}^n \overline{x_i} y_i$ tương ứng với ma trận đơn vị $I_n$. Nhóm ổn định của dạng này là $\mathbf{U}(n, K)$. Theo Bổ đề 2 của Phụ lục I, $\mathfrak{H}_+^*$ có thể được đồng nhất, như một không gian thuần nhất tôpô, với $\mathbf{GL}(n, K)/\mathbf{U}(n, K)$.

Với mọi $X \in \mathbf{GL}(n, K)$, gọi $\widetilde{X}$ là tự đẳng cấu $H \mapsto t \overline{X} \cdot H \cdot X$ của không gian vectơ *thực* $\mathfrak{H}$. Nếu $\mu$ ký hiệu độ đo Haar của nhóm cộng $\mathfrak{H}$, ta có $\widetilde{X}^{-1}(\mu) = |\det \widetilde{X}| \cdot \mu$ (\S1, No. 10, Hệ quả 1 của Mệnh đề 15). Ta chứng minh rằng

$$
| \det \widetilde{X} | = | N(X) |^\lambda ,
$$

trong đó N ký hiệu chuẩn trong $M_n(K)$ *được xem như một* $\mathbf{R}\text{-đại số}$, và trong đó $\lambda = 1 - \frac{\delta - 2}{\delta n}$. Chỉ cần kiểm chứng (15) đối với $X$ chạy qua một hệ

\footnotetext{1Xem TVS, V, §2, No. 4, Hệ quả 1 của Định lý 2.}

sinh của $\mathbf{GL}(n, K)$, do đó (A, II, §10, No. 13, Hệ quả 2 của Mệnh đề 14) đối với $X$ thuộc các loại sau:

a) $X$ là ma trận của một ánh xạ có dạng
$$
(x_1, \ldots, x_n) \mapsto (x_{\sigma(1)}, \ldots, x_{\sigma(n)}),
$$
trong đó $\sigma \in \mathfrak{S}_n$. Trong trường hợp này, một lũy thừa của $X$ bằng 1, do đó $|\det \widetilde{X}| = |N(X)| = 1$.

b) $X$ là ma trận của một ánh xạ có dạng
$$
(x_1, \ldots, x_n) \mapsto (ax_1, x_2, \ldots, x_n).
$$
Khi đó, nếu $(h_{ij}) \in \mathfrak{H}$, ta có $\widetilde{X}((h_{ij})) = (h'_{ij})$ với $h'_{11} = \overline{a} h_{11} a = |a|^2 h_{11}$, $h'_{1i} = \overline{a} h_{1i}$ với $i > 1$, $h'_{ij} = h_{ij}$ với $i > 1, j > 1$; do đó
$$
|\det \widetilde{X}| = |a|^2 |a|^{\delta(n-1)} = |a|^{2+\delta(n-1)}.
$$
Mặt khác, nếu $Y = (y_{ij}) \in M_n(K)$, thì $XY = (y'_{ij})$ với $y'_{1j} = ay_{1j}$ và $y'_{ij} = y_{ij}$ với $i > 1$; do đó $|N(X)| = |a|^{\delta n}$. Công thức (15) lại được kiểm chứng.

c) $X$ là ma trận của một ánh xạ có dạng
$$
(x_1, \ldots, x_n) \mapsto (x_1 + bx_2, x_2, \ldots, x_n).
$$
Khi đó $\widetilde{X}((h_{ij})) = (h'_{ij})$ với $h'_{11} = h_{11}$, $h'_{12} = h_{12} + h_{11} b$, $h'_{1i} = h_{1i}$ với $i > 2$, $h'_{22} = h_{22} + \overline{b} h_{12} + \overline{h}_{12} b + \overline{b} h_{11} b$, $h'_{2i} = h_{2i} + \overline{b} h_{1i}$ với $i > 2$, $h'_{ij} = h_{ij}$ với $i > 2, j > 2$. Xét đến Bổ đề 6, ta thấy rằng $|\det \widetilde{X}| = 1$. Tương tự, ta kiểm chứng được rằng $|N(X)| = 1$, điều này hoàn tất chứng minh công thức (15).

Sau khi đã thiết lập điều này, độ đo $|N(H)|^{-\lambda/2} d\mu(H)$ trên $\mathfrak{H}$ là bất biến dưới $\mathbf{GL}(n, K)$, vì
$$
\widetilde{X}^{-1}(|N(H)|^{-\lambda/2} d\mu(H)) = |N(\widetilde{X}(H))|^{-\lambda/2} \cdot |\det \widetilde{X}| d\mu(H)
= |N(H)|^{-\lambda/2} |N(X)|^{-\lambda} |\det \widetilde{X}| d\mu(H) = |N(H)|^{-\lambda/2} d\mu(H).
$$

Nếu $H \in \mathfrak{H}_+^*$, thì $H = \widetilde{X}(I_n) = {}^t \overline{X} X$ với một $X \in \mathbf{GL}(n, K)$ nào đó, do đó $N(H) = \overline{N(X)} N(X) > 0$. Do đó, trên $\mathfrak{H}_+^*$, độ đo duy nhất (sai khác một nhân tử hằng) bất biến dưới $\mathbf{GL}(n, K)$ (xem §2, No. 6, Định lý 3) là độ đo
$$
d\gamma(H) = N(H)^{-\lambda/2} d\mu(H).
$$
Đặc biệt,
$$
d\gamma(H) = (\det H)^{-(n+1)/2} d\mu(H) \quad \text{khi } K = \mathbf{R},
$$
$$
d\gamma(H) = (\det H)^{-n} d\mu(H) \quad \text{khi } K = \mathbf{C}.
$$

### Bài tập {#int-vii-s3-exercises}

Xem các [bài tập của § 3](exercises/s3/).
