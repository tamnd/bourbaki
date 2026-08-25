---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: III
chapter_title: LIE GROUPS
section: 8
section_title: Lie groups over R or Qp
lang: vi
source: lie-i-iii
pdf_pages: 0355-0360, 0413-0415
extraction: ocr
subsections:
    - "no": 1
      title: CONTINUOUS MORPHISMS
      page: 0
      pdf_page: 355
    - "no": 2
      title: CLOSED SUBGROUPS
      page: 0
      pdf_page: 358
statements: 9
exercises: 7
content_sha256: 1238ff0028a17e7c53f08f7079b49c286422c183cf20715e6feb7a8c411b265c
translated_from: content/en/lie/III/08_s8_lie_groups_over_r_or_qp.md
source_content_sha256: 1721d86a3f42951517b0823bf79374dd686f85624f871d5d4ea8c5ee70882ad3
translation_model: gpt-5-6-mini, gpt-5-6
translation_run: translate-vi-600c1f3e
glossary_version: 34
glossary_terms_sha256: 004970d0b349727bc387dc1388034f5d42e8de5f40c14900f2f286734572c717
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 8. CÁC NHÓM LIE TRÊN $\mathbf{R}$ VÀ $\mathbf{Q}_p$

### 1. CÁC CẤU XẠ LIÊN TỤC

#### Định lý 1 {#lie-iii-s8-thm-1 .statement}

*Cho G và H là hai mầm nhóm Lie trên $\mathbf{R}$ hoặc $\mathbf{Q}_p$. Cho f là một cấu xạ liên tục từ G vào H. Khi đó f là giải tích.*

Ta trang bị $L(G)$ và $L(H)$ các chuẩn xác định tôpô của chúng và sao cho $\| [x, y] \| \leq \|x\| \|y\|$ với mọi $x, y$. Tồn tại một quả cầu mở V tâm 0 trong $L(G)$ và một ánh xạ mũ $\phi$ của G xác định trên V sao cho: (1) $\phi(V)$ là một lân cận mở của $e$ trong G; (2) $\phi$ là một đẳng cấu của đa tạp giải tích V lên đa tạp giải tích $\phi(V)$; (3) $\phi(nx) = \phi(x)^n$ với mọi $x \in V$ và mọi $n \in \mathbf{Z}$ sao cho $nx \in V$. Ta định nghĩa tương tự W và $\psi$ cho H. Bằng cách thu nhỏ V nếu cần, có thể giả sử rằng $f(\phi(V)) \subset \psi(W)$. Khi đó $g = \psi^{-1} \circ f \circ \phi$ là một ánh xạ liên tục từ V vào W.

Ta chứng minh rằng
$$
(x \in V, \lambda \in \mathbf{Q} \text{ và } \lambda x \in V) \Rightarrow g(\lambda x) = \lambda g(x).
$$
Có thể giả sử rằng $\lambda \neq 0$. Đặt $\lambda = \frac{r}{q}$ với $r, q$ trong $\mathbf{Z} - \{0\}$. Đặt $y = \frac{r}{q} x$.

Nếu $K = \mathbf{R}$, ta viết $z = \frac{x}{q} = \frac{y}{r} \in V$. Khi đó $x = qz, y = rz$, do đó
$$
g(x) = \psi^{-1}(f(\phi(qz))) = \psi^{-1}(f(\phi(z)^q)) = \psi^{-1}(f(\phi(z))^q).
$$
Ta chứng minh rằng $\psi^{-1}(f(\phi(z))^q) = q \psi^{-1}(f(\phi(z))) = qg(z)$. Chỉ cần kiểm tra rằng, nếu $u \in \psi(W)$ sao cho $u^q \in \psi(W)$, thì $\psi^{-1}(u^q) = q \psi^{-1}(u)$; nhưng nếu $u = \psi(v)$, $u^q = \psi(v^q)$, thì $v^1/q \in W$ và $(\psi(v^1/q))^q = u^q$, do đó $\psi(v^1/q) = u = \psi(v)$ và vì vậy $v^1 = qv$.

Tương tự, $g(y) = rg(z)$, do đó (1).

Nếu $K = \mathbf{Q}_p$, ta viết $z = rx = qy \in V$, do đó $g(z) = rg(x) = qg(y)$, do đó lại (1).

Vì $\mathbf{Q}$ trù mật trong $K$, (1) suy ra rằng
$$
(x \in V, \lambda \in K \text{ và } \lambda x \in V) \Rightarrow g(\lambda x) = \lambda g(x).
$$
Cho $x \in L(G)$ và $\lambda, \lambda'$ là các phần tử của $K^*$ sao cho $\lambda x \in V, \lambda' x \in V$. Khi đó
$$
g(\lambda' x) = g\left( \frac{\lambda'}{\lambda} \lambda x \right) = \frac{\lambda'}{\lambda} g(\lambda x)
$$
theo (2) và do đó $\frac{1}{\lambda} g(\lambda x) = \frac{1}{\lambda'} g(\lambda' x)$. Vì vậy một mở rộng $h$ của $g$ lên $L(G)$ được xác định bằng cách viết $h(x) = \frac{1}{\lambda} g(\lambda x)$ với mọi $\lambda$ sao cho $\lambda x \in V$. Rõ ràng $h$ liên tục. Ta chứng minh rằng
$$
(x \in L(G) \text{ và } \lambda \in K) \Rightarrow h(\lambda x) = \lambda h(x).
$$
Cho $\lambda' \in K^*$ sao cho $\lambda' x \in V$ và $\lambda' \lambda x \in V$. Khi đó
$$
h(\lambda x) = \frac{1}{\lambda'} g(\lambda' \lambda x) = \frac{1}{\lambda'} \lambda g(\lambda' x) = \lambda \frac{1}{\lambda'} g(\lambda' x) = \lambda h(x).
$$
Cho $x, y$ thuộc $L(G)$. Khi đó, theo Mệnh đề 4 của § 4, no. 3,
$$
\begin{align*}
h(x) + h(y) &= \lim_{\lambda \in K^*, \lambda \to 0} \lambda^{-1} \psi^{-1}(\psi(\lambda h(x)) \psi(\lambda h(y))) \\
&= \lim_{\lambda \in K^*, \lambda \to 0} \lambda^{-1} \psi^{-1}(\psi(h(\lambda x)) \psi(h(\lambda y))).
\end{align*}
$$
Với $|\lambda|$ đủ nhỏ, $\lambda x \in V$ và $\lambda y \in V$ và do đó biểu thức trên bằng
$$
\begin{align*}
&\lim_{\lambda \in K^*, \lambda \to 0} \lambda^{-1} \psi^{-1}(f(\phi(\lambda x)) f(\phi(\lambda y))) \\
&= \lim_{\lambda \in K^*, \lambda \to 0} \lambda^{-1} (\psi^{-1} \circ f)(\phi(\lambda x) \phi(\lambda y)) \\
&= \lim_{\lambda \in K^*, \lambda \to 0} \lambda^{-1} g(\phi^{-1}(\phi(\lambda x) \phi(\lambda y))) \\
&= \lim_{\lambda \in K^*, \lambda \to 0} h(\lambda^{-1} \phi^{-1}(\phi(\lambda x) \phi(\lambda y))) \\
&= h(\lim_{\lambda \in K^*, \lambda \to 0} \lambda^{-1} \phi^{-1}(\phi(\lambda x) \phi(\lambda y))) \\
&= h(x + y).
\end{align*}
$$
Vậy $h$ liên tục và tuyến tính, do đó $g = h|V$ là giải tích, do đó $f$ là giải tích trên $\phi(V)$ và do đó $f$ là giải tích (\S 1, no. 10).

#### Hệ quả 1 {#lie-iii-s8-thm-1-cor-1 .statement}

Cho $G$ là một nhóm tôpô. Trên $G$ tồn tại nhiều nhất một cấu trúc đa tạp giải tích trên $\mathbf{R}$ (tương ứng. $\mathbf{Q}_p$) tương thích với cấu trúc nhóm tôpô trên $G$.

Điều này suy ra ngay lập tức từ Định lý 1.

#### Định nghĩa 1 {#lie-iii-s8-def-1 .statement}

*Một nhóm tôpô G được gọi là một nhóm Lie thực (tương ứng. p-adic) nếu trên G tồn tại một cấu trúc nhóm Lie thực (tương ứng. p-adic) tương thích với tôpô của nó.*

Cấu trúc đó khi đó là duy nhất và ta có thể nói về *chiều* của một nhóm như vậy. Nếu G và H là hai nhóm như vậy, mọi cấu xạ liên tục từ G vào H đều là giải tích.

#### Hệ quả 2 {#lie-iii-s8-def-1-cor-2 .statement}

*Cho G là một nhóm tôpô và V là một lân cận mở của e. Giả sử rằng V có một cấu trúc đa tạp giải tích làm cho nó trở thành một mầm nhóm Lie thực (tương ứng. p-adic). Khi đó G là một nhóm Lie thực (tương ứng. p-adic).*

Cho $g \in G$. Tồn tại một lân cận mở $V'$ của $e$ trong G sao cho $V' \cup gV'g^{-1} \subset V$. Ánh xạ $v \mapsto gv g^{-1}$ từ $V'$ vào $V$ là một cấu xạ liên tục và do đó giải tích của mầm nhóm Lie $V'$ vào mầm nhóm Lie $V$. Khi đó chỉ cần áp dụng Mệnh đề 18 của § 1, no. 9.

#### Nhận xét {#lie-iii-s8-n1-rem-1 .statement}

(1) Định lý 1 và các hệ quả của nó không còn đúng nếu $\mathbf{R}$ (tương ứng. $\mathbf{Q}_p$) được thay bởi $\mathbf{C}$ (Bài tập 1).

(2) Cho G là một nhóm tôpô. Có thể chỉ ra† rằng các điều kiện sau là tương đương: (a) G là một nhóm Lie thực hữu hạn chiều; (b) G là compact địa phương và tồn tại một lân cận của $e$ chứa không nhóm con nào phân biệt với $\{e\}$; (c) tồn tại một lân cận mở của $e$ đồng phôi với một quả cầu mở của một không gian $\mathbf{R}^n$. (Đối với một kết quả ít khó hơn nhiều, xem Bài tập 6.)

#### Mệnh đề 1 {#lie-iii-s8-prop-1 .statement}

*Cho G, G' là các nhóm tôpô và f là một cấu xạ liên tục của G vào G'. Giả sử một trong ba trường hợp sau đây xảy ra:
(a) G là một nhóm Lie thực và G' là một nhóm Lie p-adic;
(b) G là một nhóm Lie p-adic và G' là một nhóm Lie thực;
(c) G là một nhóm Lie p-adic và G' là một nhóm Lie $p'$-adic với $p \neq p'$.
Khi đó f là hằng địa phương.*

Trường hợp (a). Gọi $G_0$ là thành phần đơn vị của G. Khi đó $f(G_0)$ là một nhóm con liên thông của $G'$ và do đó $f(G_0) = \{e\}$ và $G_0$ là mở trong G.

Trường hợp (b). Gọi $V'$ là một lân cận của $e$ trong $G'$ sao cho mọi nhóm con của $G'$ được chứa trong $V'$ đều thu gọn về $\{e\}$ (\S 4, no. 2, Hệ quả 1 của Định lý 2). Tồn tại một lân cận V của $e$ trong G sao cho $f(V) \subset V'$. Khi đó tồn tại một nhóm con mở $G_1$ của G sao cho $G_1 \subset V$ (\S 7, no. 1, Mệnh đề 1). Khi đó $f(G_1) = \{e\}$.

Trường hợp (c). Theo \S 7, Định lý 4 và Hệ quả của Mệnh đề 8, tồn tại một lân cận $V'$ của $e$ trong $G'$ sao cho, với mọi $x' \in V' - \{e\}$, $x'^{p^n}$ không hội tụ

† Xem chẳng hạn D. Montgomery và L. Zippin, *Topological transformation groups*, Interscience tracts in pure and applied mathematics, no. 1, Interscience publishers, New York 1955 (đặc biệt các trang 169 và 184).

tới $e$ khi $n$ tiến tới $+\infty$. Tồn tại một lân cận $V$ của $e$ trong G sao cho $f(V) \subset V'$. Theo § 7, Định lý 4 và Mệnh đề 9, tồn tại một nhóm con mở $G_1$ của $G$ sao cho $G_1 \subset V$ và sao cho, với mọi $x \in G_1$, $x^{p^n}$ hội tụ tới $e$ khi $n$ tiến tới $+\infty$. Khi đó $f(G_1) = \{e\}$.

### 2. NHÓM CON ĐÓNG

#### Định lý 2 {#lie-iii-s8-thm-2 .statement}

*Cho $G$ là một nhóm Lie hữu hạn chiều trên $\mathbf{R}$ hoặc $\mathbf{Q}_p$. Mọi nhóm con đóng của $G$ đều là một nhóm con Lie của $G$. Nói chung hơn, cho $U$ là một lân cận mở đối xứng của $e$ trong $G$ và $H$ là một không gian con đóng không rỗng của $U$ sao cho các điều kiện $x \in H$, $y \in H$ và $xy^{-1} \in U$ kéo theo $xy^{-1} \in H$. Khi đó $H$ là một mầm nhóm con Lie của $G$.*

Cho $\mathfrak{h}$ là đại số con Lie tiếp xúc với $H$ tại $e$ (\S 4, no. 5, Định nghĩa 2). Tồn tại một mầm nhóm con Lie $H_0$ của $G$ với đại số Lie $\mathfrak{h}$ và được chứa trong $H$. Ta chứng minh rằng $H_0$ là mở trong $H$ với tôpô cảm sinh bởi tôpô trên $G$. Điều này sẽ chứng minh rằng $H$ là một đa tạp con giải tích của $G$ và sẽ thiết lập định lý.

Tồn tại một không gian con vectơ $\mathfrak{k}$ phụ trợ cho $\mathfrak{h}$ trong $L(G)$, các lân cận mở đối xứng $V_1, V_2$ của không trong $\mathfrak{h}$ và $\mathfrak{k}$ tương ứng, và một ánh xạ mũ $\phi$ của $G$ được xác định trên $V_1 + V_2$ và có các tính chất sau:

(a) ánh xạ $(a_1, a_2) \mapsto \phi(a_1)\phi(a_2)$ là một đẳng cấu giải tích từ $V_1 \times V_2$ lên một tập con mở $V$ của $G$;
(b) $\phi(V_1) \subset H_0$;
(c) $V^2 \subset U$.

Ta sẽ chứng minh (và điều này sẽ hoàn tất chứng minh) rằng tồn tại một lân cận mở $V'_2$ của 0 trong $V_2$ sao cho $H \cap (\phi(V_1)\phi(V'_2)) = \phi(V_1)$.

Giả sử mệnh đề đó là sai. Khi đó ta có thể tìm được một dãy $(x_n)$ trong $V_1$ và một dãy $(y_n)$ trong $V_2 - \{0\}$ hội tụ về 0, sao cho $\phi(x_n)\phi(y_n) \in H$ với mọi $n$. Khi đó $\phi(y_n) \in H$ theo (c).

Nếu $K = \mathbf{Q}_p$, có thể giả sử rằng $V_2$ là một nhóm con cộng tính của $\mathfrak{k}$ và rằng $\phi(pa) = \phi(a)^p$ với mọi $a \in V_2$ và mọi $p \in \mathbf{Z}$. Khi đó $\phi(\lambda y_1) \in H$ với mọi $\lambda \in \mathbf{Z}$ và do tính liên tục với mọi $\lambda \in \mathbf{Z}_p$. Ánh xạ $f : \lambda \mapsto \phi(\lambda y_1)$ từ $\mathbf{Z}_p$ vào $G$ là giải tích và nhận các giá trị trong $H$ và $(T_0f)(1) = y_1$. Do đó $y_1 \in \mathfrak{h}$, điều này là vô lý. Vì vậy định lý được thiết lập trong trường hợp $\mathbf{Q}_p$.

Nếu $K = \mathbf{R}$, có thể giả sử rằng $V_2$ là liên thông và rằng $y_n$ thuộc $\frac{1}{2}V_2 - \{0\}$. Bằng cách lấy một dãy con của $(y_n)$ nếu cần, ta có thể tìm được một dãy $(\lambda_n)$ các vô hướng khác không sao cho $\lambda_n^{-1}y_n$ tiến tới một phần tử $y$ của $V_2 - \{0\}$. Dãy $(\lambda_n)$ tiến tới 0. Cho $\lambda \in \mathbf{R}$ sao cho $\lambda y \in \frac{1}{2}V_2$; ta chứng minh rằng $\exp(\lambda y) \in H$. Có thể giả sử rằng $\lambda \lambda_n^{-1}y_n \in \frac{1}{2}V_2$ với mọi $n$. Cho $k_n \in \mathbf{Z}$ sao cho $|\lambda - k_n \lambda_n|$ tiến tới 0. Với $n$ đủ lớn, $(\lambda - k_n \lambda_n)\lambda_n^{-1}y_n \in \frac{1}{2}V_2$ và do đó $k_n y_n \in \frac{1}{2}V_2$. Suy ra $\exp(h y_n) \in H$ với $h$ là một số nguyên và $0 \leq |h| \leq |k_n|$ (như thấy được bằng quy nạp theo $|h|$). Khi đó
$$
\exp(\lambda y) = \lim_{n \to \infty} \exp(\lambda \lambda_n^{-1}y_n) = \lim_{n \to \infty} (\exp((\lambda - k_n \lambda_n)\lambda_n^{-1}y_n) \exp(k_n y_n))
= \lim_{n \to \infty} \exp k_n y_n \in H.
$$

Do đó ánh xạ $f : \lambda \mapsto \exp \lambda y$, trong đó $\lambda y \in \frac{1}{4}V_2$, nhận các giá trị của nó trong $H$ và $(T_0f)(1) = y$. Suy ra $y \in \mathfrak{h}$, điều này là vô lý. Định lý được thiết lập như vậy trong trường hợp $\mathbf{R}$.

Định lý 2 không còn đúng nữa nếu không giả sử $G$ là hữu hạn chiều (Bài tập 12).

#### Hệ quả 1 {#lie-iii-s8-thm-2-cor-1 .statement}

*Cho $G'$ là một nhóm compact địa phương, $G$ là một nhóm Lie hữu hạn chiều trên $\mathbf{R}$ (tương ứng $\mathbf{Q}_p$) và $f$ là một cấu xạ liên tục từ $G'$ vào $G$. Nếu hạt nhân của $f$ là rời rạc, thì $G'$ là một nhóm Lie hữu hạn chiều thực (tương ứng $p$-adic).*

Có một lân cận compact $V$ của $e$ trong $G'$ sao cho $f|V$ là một phép đồng phôi từ $V$ lên một không gian con compact của $G$. Nếu $U$ là một lân cận mở đủ nhỏ của $e$ trong $G$, các giả thiết của Định lý 2 được thỏa mãn với $H = f(V) \cap U$. Do đó $H$ là một mầm nhóm con Lie của $G$. Gọi $W$ là ảnh ngược của $H$ theo $f|V$. Khi đó $W$ là một lân cận của $e$ trong $G'$. Trang bị cho $W$ cấu trúc đa tạp giải tích được vận chuyển từ cấu trúc trên $H$ bởi $(f|W)^{-1}$. Với mọi $z \in G'$, ánh xạ $x \mapsto f(z)x f(z)^{-1}$ từ $G$ vào $G$ là giải tích; do đó tồn tại một lân cận mở $W'$ của $e$ trong $W$ sao cho ánh xạ $x' \mapsto zx'z^{-1}$ từ $W'$ vào $W$ là giải tích. Theo Mệnh đề 18 của § 1, no. 9, tồn tại trên $G'$ một cấu trúc nhóm Lie cảm sinh trên một lân cận mở đủ nhỏ của $e$ cùng cấu trúc giải tích với $W$ và do đó cùng tôpô với tôpô ban đầu trên $G'$.

#### Hệ quả 2 {#lie-iii-s8-thm-2-cor-2 .statement}

*Cho $G$ là một nhóm Lie hữu hạn chiều trên $K$, $H$ là một nhóm con của $G$, $V$ là một lân cận mở của $e$ trong $G$ và $(M_i)_{i \in I}$ là một họ các đa tạp giải tích trên $K$; với mọi $i \in I$, gọi $f_i$ là một ánh xạ $K$-giải tích từ $V$ vào $M_i$ sao cho*

$$
H \cap V = \{ x \in V \mid f_i(x) = f_i(e) \text{ với mọi } i \in I \}.
$$

*(i) Nếu $K = \mathbf{C}$, $H$ là một nhóm con Lie của $G$.*
*(ii) Nếu $K$ là một mở rộng hữu hạn của $\mathbf{Q}_p$ và $I$ là hữu hạn, $H$ là một nhóm con Lie của $G$.*

(i) Giả sử $K = \mathbf{C}$. Ta xét $G$ như một nhóm Lie thực. Khi đó $H$ là một nhóm con Lie thực của $G$ (Định lý 2). Cho $a \in L(H)$. Có một lân cận mở liên thông $W$ của $0$ trong $\mathbf{C}$ sao cho $\exp \lambda a \in V$ với mọi $\lambda \in W$. Cho $i \in I$. Khi đó $f_i(\exp \lambda a) = f_i(e)$ nếu $\lambda \in \mathbf{R} \cap W$. Do đó $f_i(\exp \lambda a) = f_i(e)$ nếu $\lambda \in W$ nhờ phép tiếp tục giải tích. Vậy $\exp \lambda a \in H$ với $\lambda \in W$ và do đó $\mu a \in L(H)$ với mọi $\mu \in \mathbf{C}$. Suy ra $H$ là một nhóm con Lie của nhóm Lie phức $G$ (\S 4, no. 2, Mệnh đề 2).

(ii) Giả sử rằng $K$ là một mở rộng hữu hạn của $\mathbf{Q}_p$. Ta xét $G$ như một nhóm Lie trên $\mathbf{Q}_p$. Nó có số chiều hữu hạn và Định lý 2 suy ra rằng $H$ là một nhóm con Lie $p$-adic của $G$. Vì $I$ là hữu hạn, $\prod_{i \in I} M_i$ là một đa tạp và có thể giả sử rằng họ $(f_i)$ quy về một ánh xạ duy nhất $f$. Cho $a \in L(G)$. Gọi $\phi$ là một ánh xạ mũ của $G$. Khi đó $f(\phi(\lambda a)) = f(e)$ với $\lambda \in \mathbf{Q}_p$ và $|\lambda|$ đủ nhỏ. Vì $f$ là $K$-giải tích, suy ra $f(\phi(\lambda a)) = f(e)$ với $\lambda \in K$ và $|\lambda|$ đủ nhỏ. Do đó $\phi(\lambda a) \in H$ với $\lambda \in K$ và $|\lambda|$ đủ nhỏ, và vì vậy $\mu a \in L(H)$ với mọi $\mu \in K$. Chứng minh được hoàn thành như trong (i).

Hệ quả 2 (ii) không còn đúng nữa nếu ta bỏ giả thiết rằng $I$ là hữu hạn.

### Bài tập {#lie-iii-s8-exercises}

Xem các [bài tập của § 8](exercises/s8/).
