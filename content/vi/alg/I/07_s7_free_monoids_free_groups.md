---
book: alg
book_title: Algebra
chapter: I
chapter_title: ALGEBRAIC STRUCTURES
section: 7
section_title: Free monoids, free groups
lang: vi
source: alg-i-iii
source_edition: 1998, Springer
pdf_pages: 0105-0120, 0183-0195
extraction: ocr
subsections:
    - "no": 1
      title: FREE MAGMAS
      page: 0
      pdf_page: 105
    - "no": 2
      title: FREE MONOIDS
      page: 0
      pdf_page: 106
    - "no": 3
      title: AMALGAMATED SUM OF MONOIDS
      page: 0
      pdf_page: 108
    - "no": 4
      title: APPLICATION TO FREE MONOIDS
      page: 0
      pdf_page: 112
    - "no": 5
      title: FREE GROUPS
      page: 0
      pdf_page: 113
    - "no": 6
      title: PRESENTATIONS OF A GROUP
      page: 0
      pdf_page: 114
    - "no": 7
      title: FREE COMMUTATIVE GROUPS AND MONOIDS
      page: 0
      pdf_page: 116
    - "no": 8
      title: EXPONENTIAL NOTATION
      page: 0
      pdf_page: 118
    - "no": 9
      title: RELATIONS BETWEEN THE VARIOUS FREE OBJECTS
      page: 0
      pdf_page: 119
statements: 17
exercises: 3
content_sha256: a3f5c7595d5fff92ea2a59376e70b8ac487b5508e5b65e5f161b7b9fa9fccee9
translated_from: content/en/alg/I/07_s7_free_monoids_free_groups.md
source_content_sha256: d6c7fd2882a44296a4e9b83c268872b327ceb30194985c94a03a463dd6e566f0
translation_model: gpt-5-6, gpt-5-6-mini, gpt-5.4-mini
translation_run: translate-vi-ca7cd7e4
glossary_version: 34
glossary_terms_sha256: 60b8db012b8fdd34f92b203d73bc7b075ec2bb9d498685fa4a9cb3e3ee2261ae
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 7. CÁC NỬA NHÓM TỰ DO, CÁC NHÓM TỰ DO

Trong đoạn này X sẽ ký hiệu một tập hợp. Trừ khi có nói khác đi, phần tử đơn vị của một nửa nhóm sẽ được ký hiệu bởi e.

### 1. CÁC MAGMA TỰ DO

Một dãy các tập hợp $M_n(X)$ được định nghĩa bằng quy nạp theo số nguyên $n \geqslant 1$ như sau: viết $M_1(X) = X$, với $n \geqslant 2$, $M_n(X)$ là tập hợp là tổng của các tập hợp $M_p(X) \times M_{n-p}(X)$ với $1 \leqslant p \leqslant n-1$. Tập hợp là tổng của họ $(M_n(X))_{n \geqslant 1}$ được ký hiệu bởi $M(X)$; mỗi tập hợp $M_n(X)$ được đồng nhất với ảnh chính tắc của nó trong $M(X)$. Với mọi phần tử $w$ của $M(X)$ tồn tại một số nguyên duy nhất $n$ sao cho $w \in M_n(X)$; nó được gọi là độ dài của $w$ và được ký hiệu bởi $l(w)$. Tập hợp X gồm các phần tử trong $M(X)$ có độ dài 1.

Cho $w$ và $w'$ thuộc $M(X)$; viết $p = l(w)$ và $q = l(w')$. Ảnh của $(w, w')$ qua đơn ánh chính tắc của $M_p(X) \times M_q(X)$ vào tập hợp tổng $M_{p+q}(X)$ được gọi là hợp thành của $w$ và $w'$ và được ký hiệu bởi $ww'$ hoặc $w.w'$. Khi đó $l(w.w') = l(w) + l(w')$ và mọi phần tử của $M(X)$ có độ dài $\geqslant 2$ có thể được viết duy nhất dưới dạng $w'w''$ với $w', w''$ thuộc $M(X)$.

Tập hợp $M(X)$ với luật hợp thành $(w, w') \mapsto w.w'$ được gọi là magma tự do được xây dựng trên X (\$ 1, no. 1, Định nghĩa 1).

#### Mệnh đề 1 {#alg-i-s7-prop-1 .statement}

Cho M là một magma. Mọi ánh xạ f từ X vào M có thể được mở rộng theo một cách duy nhất thành một cấu xạ từ $M(X)$ vào M.

Bằng quy nạp trên $n \geqslant$, các ánh xạ $f_n : M_n(X) \to M$ được định nghĩa như sau: cho f_1 = f; với n \geq 2, ánh xạ f_n được định nghĩa bởi $f_n(w.w') = f_p(w).f_{n-p}(w')$ với $p = 1, 2, \ldots, n-1$ và $(w, w')$ thuộc $M_p(X) \times M_{n-p}(X)$. Cho $g$ là ánh xạ từ $M(X)$ vào $M$ cảm sinh các $f_n$ trên $M_n(X)$ với mọi số nguyên $n \geq 1$. Rõ ràng $g$ là cấu xạ duy nhất từ $M(X)$ vào $M$ mở rộng $f$.

Cho $u$ là một ánh xạ của $X$ vào một tập hợp $Y$. Theo Mệnh đề 1, tồn tại một và chỉ một đồng cấu của $M(X)$ vào $M(Y)$ trùng với $u$ trên $X$. Nó sẽ được ký hiệu là $M(u)$. Nếu $v$ là một ánh xạ của $Y$ vào một tập hợp $Z$, đồng cấu $M(v) \circ M(u)$ của $M(X)$ vào $M(Z)$ trùng với $v \circ u$ trên $X$, do đó

$$
M(v) \circ M(u) = M(v \circ u).
$$

#### Mệnh đề 2 {#alg-i-s7-prop-2 .statement}

*Cho $u : X \to Y$ là một ánh xạ. Nếu $u$ là đơn ánh (tương ứng toàn ánh, song ánh), thì $M(u)$ cũng vậy.*

Giả sử $u$ là đơn ánh. Khi $X$ là rỗng, $M(X)$ là rỗng, do đó $M(u)$ là đơn ánh. Nếu $X$ không rỗng, tồn tại một ánh xạ $v$ của $Y$ vào $X$ sao cho $v \circ u$ là ánh xạ đồng nhất của $X$ (*Lý thuyết tập hợp*, II, § 3, no. 8, Mệnh đề 8); ánh xạ $M(v) \circ M(u) = M(v \circ u)$ là ánh xạ đồng nhất của $M(X)$ và do đó $M(u)$ là đơn ánh.

Khi $u$ là toàn ánh, tồn tại một ánh xạ $w$ của $Y$ vào $X$ sao cho $u \circ w$ là ánh xạ đồng nhất của $Y$ (*Lý thuyết tập hợp*, II, § 3, no. 8, Mệnh đề 8). Khi đó $M(u) \circ M(w) = M(u \circ w)$ là ánh xạ đồng nhất của $M(Y)$ và do đó $M(u)$ là toàn ánh.

Cuối cùng, nếu $u$ là song ánh, nó là đơn ánh và toàn ánh, và do đó $M(u)$ có cùng các tính chất.

Cho $S$ là một tập con của $X$. Theo Mệnh đề 2, đơn ánh của $S$ vào $X$ có thể được mở rộng thành một đẳng cấu của $M(S)$ lên một dưới magma $M'(S)$ của $M(X)$. Các magma $M(S)$ và $M'(S)$ được đồng nhất nhờ đẳng cấu này. Khi đó $M(S)$ là dưới magma của $M(X)$ sinh bởi $S$.

Cho $X$ là một tập hợp và $(u_\alpha, v_\alpha)_{\alpha \in I}$ là một họ các cặp có thứ tự của các phần tử của $M(X)$. Cho $R$ là quan hệ tương đương trên $M(X)$ tương thích với luật của $M(X)$ và sinh bởi các $(u_\alpha, v_\alpha)$ (\S 1, no. 6). Magma $M(X)/R$ được gọi là *magma được xác định bởi $X$ và các phần tử xác định* $(u_\alpha, v_\alpha)_{\alpha \in I}$. Cho $h$ là cấu xạ chính tắc của $M(X)$ lên $M(X)/R$. Khi đó $M(X)/R$ được sinh bởi $h(X)$.

Cho $N$ là một magma và $(n_x)_{x \in X}$ là một họ các phần tử của $N$. Cho $k$ là cấu xạ từ $M(X)$ đến $N$ sao cho $k(x) = n_x$ với mọi $x \in X$ (Mệnh đề 1). Nếu $k(u_\alpha) = k(v_\alpha)$ với mọi $\alpha \in I$, tồn tại một và chỉ một cấu xạ $f : M(X)/R \to N$ sao cho $f(h(x)) = n_x$ với mọi $x \in X$ (\S 1, no. 6, Mệnh đề 9).

### 2. MONÔID TỰ DO

Mọi dãy hữu hạn $w = (x_i)_{1 \leq i \leq n}$ của các phần tử của $X$ được đánh chỉ số bởi một khoảng $[1, n]$ của $\mathbf{N}$ (có thể rỗng) được gọi là một *từ* được dựng trên $X$. Số nguyên $n$ được gọi là *độ dài* của từ $w$ và được ký hiệu bởi $l(w)$. Có duy nhất một từ có độ dài 0, đó là dãy rỗng $e$. $\mathbf{X}$ sẽ được đồng nhất với tập hợp các từ có độ dài 1.

Cho $w = (x_i)_{1 \leq i \leq m}$ và $w' = (x'_j)_{1 \leq j \leq n}$ là hai từ. Hợp thành của $w$ và $w'$ là từ $u = (y_k)_{1 \leq k \leq m+n}$ được xác định bởi

$$
y_k = \begin{cases}
x_k & \text{cho } 1 \leq k \leq m \\
x'_{k-m} & \text{cho } m+1 \leq k \leq m+n.
\end{cases}
$$

Nói cách khác, dãy $w''$ được thu được bằng cách trước hết viết các phần tử của dãy $w$ rồi sau đó viết các phần tử của $w'$. Hợp thành của $w$ và $w'$ nói chung được ký hiệu bởi $ww'$ hoặc $w.w'$; đôi khi người ta nói rằng nó được thu được bằng phép ghép $w$ và $w'$. Khi đó theo phép dựng $l(w.w') = l(w) + l(w')$.

Quan hệ $we = ew = w$ được thiết lập ngay lập tức đối với mọi từ $w$. Cho $w = (x_i)_{1 \leq i \leq m}$, $w' = (x'_j)_{1 \leq j \leq n}$ và $w'' = (x''_k)_{1 \leq k \leq p}$ là ba từ; rõ ràng các từ $w(w'w'')$ và $(ww')w''$ đều bằng từ $(y_l)_{1 \leq l \leq m+n+p}$ được xác định bởi

$$
y_l = \begin{cases}
x_l & \text{nếu } 1 \leq l \leq m \\
x_{l-m} & \text{nếu } m+1 \leq l \leq m+n \\
x''_{l-m-n} & \text{nếu } m+n+1 \leq l \leq m+n+p.
\end{cases}
$$

Điều trên chỉ ra rằng tập hợp các từ được xây dựng trên $\mathbf{X}$ với luật hợp thành $(w, w') \mapsto w.w'$ là một monoid với phần tử đơn vị $e$. Nó được ký hiệu bởi $\mathrm{Mo}(\mathbf{X})$ và được gọi là *monoid tự do được xây dựng trên* $\mathbf{X}$. Từ định nghĩa tích của các từ suy ra ngay lập tức rằng mọi từ $w = (x_i)_{1 \leq i \leq n}$ bằng tích $\prod_{i=1}^n x_i$. Do đó, một từ có thể được viết dưới dạng $x_1 \ldots x_n$.

#### Mệnh đề 3 {#alg-i-s7-prop-3 .statement}

*Cho M là một monoid. Mọi ánh xạ f từ X vào M mở rộng duy nhất thành một đồng cấu từ Mo(X) vào M.*

Cho $g$ là một đồng cấu từ $\mathrm{Mo}(\mathbf{X})$ vào $M$ mở rộng $f$. Nếu $w = (x_i)_{1 \leq i \leq n}$ là một từ, thì $w = \prod_{i=1}^n x_i$ trong monoid $\mathrm{Mo}(\mathbf{X})$, do đó

$$
g(w) = \prod_{i=1}^n g(x_i) = \prod_{i=1}^n f(x_i)
$$

trong monoid $M$ (\S 1, no. 2, công thức (2)). Điều này chứng minh tính duy nhất của $g$.

Đặt $h(w) = \prod_{i=1}^n f(x_i)$ đối với mọi từ $w = (x_i)_{1 \leq i \leq n}$. Định lý tính kết hợp (\S 1, no. 3, Định lý 1) và định nghĩa tích trong $\mathrm{Mo}(\mathbf{X})$ kéo theo $h(ww') = h(w)h(w')$. Theo quy ước, tích rỗng $h(e)$ là phần tử đơn vị của $M$ và $h(x) = f(x)$ với $x \in \mathbf{X}$. Vì thế $h$ là một đồng cấu từ $\mathrm{Mo}(x)$ vào $M$ mở rộng $f$.

Cho $u : \mathbf{X} \to \mathbf{Y}$ là một ánh xạ. Theo Mệnh đề 3, tồn tại một và chỉ một đồng cấu từ Mo(X) vào Mo(Y) trùng với u trên X; nó được ký hiệu là Mo(u). Nó biến một từ $(x_i)_{1 \leq i \leq n}$ thành từ $(u(x_i))_{1 \leq i \leq n}$. Như trong trường hợp của các magma (no. 1), phương trình Mo(v \circ u) = Mo(v) \circ Mo(u) được thiết lập đối với mọi ánh xạ $v : Y \to Z$ và có thể chứng minh rằng Mo(u) là đơn ánh (tương ứng toàn ánh, song ánh) nếu u là như vậy. Đối với mọi tập con S của X, Mo(S) được đồng nhất với monoid con của Mo(X) sinh bởi S.

Cho X là một tập hợp và $(u_\alpha, v_\alpha)_{\alpha \in I}$ là một họ các cặp có thứ tự của các phần tử của Mo(X). Cho R là quan hệ tương đương trên Mo(X) tương thích với luật trên Mo(X) và được sinh bởi các $(u_\alpha, v_\alpha)$ (\S 1, no. 6). Monoid Mo(X)/R được gọi là *monoid được xác định bởi X và các quan hệ xác định* $(u_\alpha, v_\alpha)_{\alpha \in I}$. Cho h là cấu xạ chính tắc từ Mo(X) lên Mo(X)/R. Khi đó Mo(X) được sinh bởi h(X).

Cho N là một monoid và $(n_x)_{x \in X}$ là một họ các phần tử của N. Cho k là cấu xạ từ Mo(X) vào N sao cho $k(x) = n_x$ với mọi $x \in X$ (Mệnh đề 3). Nếu $k(u_\alpha) = k(v_\alpha)$ với mọi $\alpha \in I$, tồn tại một và chỉ một cấu xạ magma $f : Mo(X)/R \to N$ sao cho $f(h(x)) = n_x$ với mọi $x \in X$ (\S 1, no. 6, Mệnh đề 9); vì k có đơn vị, f là một cấu xạ monoid.

### 3. TỔNG DÍNH CỦA CÁC MONOID

*Cho $(M_i)_{i \in I}$ là một họ các monoid và $e_i$ là phần tử đơn vị của $M_i$. Ta cho một monoid A và một họ các đồng cấu $h_i : A \to M_i$ (đối với $i \in I$).*

Tập hợp S mà tổng của họ $(M_i)_{i \in I}$ có các phần tử là các cặp có thứ tự $(i, x)$ với $i \in I$ và $x \in M_i$. Với mọi bộ ba $\alpha = (i, x, x')$ với $i \in I$, $x, x'$ trong $M_i$, viết $u_\alpha = (i, xx')$ và $v_\alpha = (i, x).(i, x')$; với mọi bộ ba $\lambda = (i, j, a)$ trong $I \times I \times A$, viết $p_\lambda = (i, h_i(a))$ và $q_\lambda = (j, h_j(a))$; với mọi $i \in I$, viết $\varepsilon_i = (i, e_i)$. Vị nhóm M được xác định bởi S và các hệ thức $(u_\alpha, v_\alpha)$, $(p_\lambda, q_\lambda)$ và $(\varepsilon_i, e)$ được gọi là *tổng của họ* $(M_i)_{i \in I}$ *thác triển theo* A. Ký hiệu $\phi$ là đồng cấu chính tắc của Mo(S) lên M và viết $\phi_i(x) = \phi(i, x)$ với $(i, x) \in S$. Ta nói rằng $\phi_i$ là *ánh xạ chính tắc* của $M_i$ vào M. Với mọi $a \in A$, phần tử $\phi(i, h_i(a))$ độc lập với i và được ký hiệu là $h(a)$.\footnote{Khi I rỗng, $M = \{e\}$ và $h(a) = e$ với mọi $a \in A$.}

Tính chất phổ quát của các vị nhóm được xác định bởi các phần tử sinh và các hệ thức (no. 2) kéo theo kết quả sau:

#### Mệnh đề 4 {#alg-i-s7-prop-4 .statement}

(a) *Với mọi $i \in I$, ánh xạ $\phi_i$ là một đồng cấu của $M_i$ vào M và $\phi_i \circ h_i = h$ với mọi $i \in I$. Hơn nữa, M được sinh bởi $\bigcup_{i \in I} \phi_i(M_i)$.*

(b) *Cho $M'$ là một vị nhóm và $f' : M_i \to M'$ (với $i \in I$) là các đồng cấu sao cho $f_i \circ h_i$ độc lập với $i \in I$. Tồn tại duy nhất một đồng cấu $f : M \to M'$ sao cho $f_i = f \circ \phi_i$ với mọi $i \in I$.*

Sau đây ta sẽ đưa ra giả thiết sau:

(A) *Với mọi $i \in I$, tồn tại một tập con $P_i$ của $M_i$ chứa $e_i$ sao cho ánh xạ $(a, p) \mapsto h_i(a).p$ của $A \times P_i$ vào $M_i$ là song ánh.*

Điều này kéo theo các đồng cấu $h_i$ là đơn ánh. Cho $x \in M$; mọi dãy hữu hạn $\sigma = (a; i_1, \ldots, i_n; p_1, \ldots, p_n)$ với $a \in A, i_\alpha \in I$ và $p_\alpha \in P_{i_\alpha}$ với $1 \leq \alpha \leq n$, thỏa mãn

$$
x = h(a) \cdot \prod_{\alpha=1}^n \phi_{i_\alpha}(p_\alpha)
$$

được gọi là một phân tích của $x$. Số nguyên $n \geq 0$ được gọi là độ dài của phân tích $\sigma$ và được ký hiệu bởi $l(\sigma)$; dãy $(e)$ là một phân tích có độ dài 0 của phần tử đơn vị của $M$. Phân tích $\sigma$ được gọi là rút gọn nếu $i_\alpha \neq i_{\alpha+1}$ với $1 \leq \alpha < n$ và $p_\alpha \neq e_{i_\alpha}$ với $1 \leq \alpha \leq n$.

#### Mệnh đề 5 {#alg-i-s7-prop-5 .statement}

Theo giả thiết (A), mọi phần tử $x$ của $M$ đều thừa nhận một phân tích rút gọn duy nhất $\sigma$. Mọi phân tích $\sigma' \neq \sigma$ của $x$ đều thỏa mãn $l(\sigma') > l(\sigma)$.

(A) Tính duy nhất của một phân tích rút gọn:

Gọi $\Sigma$ là tập hợp các dãy $\sigma = (a; i_1, \ldots, i_n; p_1, \ldots, p_n)$ với $n \geq 0$, $a \in A, i_\alpha \in I$ và $p_\alpha \in P_{i_\alpha} - \{e_{i_\alpha}\}$ với $1 \leq \alpha \leq n$, sao cho $i_\alpha \neq i_{\alpha+1}$ với $1 \leq \alpha < n$. Gọi $\Phi$ là ánh xạ của $\Sigma$ vào $M$ được xác định bởi

$$
\Phi(a; i_1, \ldots, i_n; p_1, \ldots, p_n) = h(a) \cdot \prod_{\alpha=1}^n \phi_{i_\alpha}(p_\alpha).
$$

Một phân tích rút gọn của $x \in M$ là một phần tử $\sigma$ của $\Sigma$ sao cho $\Phi(\sigma) = x$.

Với mọi $i \in I$, gọi $\Sigma_i$ là tập con của $\Sigma$ gồm các dãy $(e; i_1, \ldots, i_n; p_1, \ldots, p_n)$ với $i \neq i_1$ khi $n > 0$. Gọi

$$
\sigma = (e; i_1, \ldots, i_n; p_1, \ldots, p_n)
$$

là một phần tử của $\Sigma_i$ và $\xi$ thuộc $M_i$; giả sử $\xi = h_i(a) \cdot p$ với $a \in A$ và $p \in P_i$, và

$$
\Psi_i(\xi, \sigma) = \begin{cases}
(a; i_1, \ldots, i_n; p_1, \ldots, p_n) & \text{nếu } p = e_i \\
(a; i, i_1, \ldots, i_n; p, p_1, \ldots, p_n) & \text{nếu } p \neq e_i.
\end{cases}
$$

Hiển nhiên rằng $\Psi_i$ là một song ánh từ $M_i \times \Sigma_i$ lên $\Sigma$.

Cho $i \in I$ và $x \in M_i$; vì $\Psi_i$ là một song ánh, một ánh xạ $f_{i,x}$ của $\Sigma$ vào chính nó được xác định bởi

$$
f_{i,x}(\Psi_i(\xi, \sigma)) = \Psi_i(x\xi, \sigma) \quad (\xi \in M_i, \sigma \in \Sigma_i).
$$

Ngoài ra, với $a \in A, f_a$ ký hiệu ánh xạ của $\Sigma$ vào chính nó được xác định bởi

$$
f_a(a'; i_1, \ldots, i_n; p_1, \ldots, p_n) = (aa'; i_1, \ldots, i_n; p_1, \ldots, p_n).
$$

Rõ ràng $f_{i,e_i}$ là ánh xạ đồng nhất của $\Sigma$ và $f_{i,xx'} = f_{i,x} \circ f_{i,x'}$ đối với $x, x'$ trong $M_i$ và $f_{i,h_i(a)} = f_a$ đối với $a \in A$ và $i \in I$.

Khi đó Mệnh đề 4 có thể được áp dụng vào trường hợp $M'$ là nửa nhóm các ánh xạ của $\Sigma$ vào chính nó với luật hợp thành $(f,f') \mapsto f \circ f'$ và trong đó f_i là đồng cấu $x \mapsto f_{i,x}$ của $M_i$ vào $M'$; khi đó tồn tại một đồng cấu $f$ của $M$ vào $M'$ sao cho $f_{i,x} = f(\phi_i(x))$ đối với $i \in I$ và $x \in M_i$. Cho
$$
\sigma = (a; i_1, \ldots, i_n; p_1, \ldots, p_n)
$$
thuộc $\Sigma$. Các công thức (5) đến (7) suy ra bằng quy nạp theo $n$ quan hệ
$$
\begin{align*}
\sigma &= (f_a \circ f_{i_1, p_1} \circ \cdots \circ f_{i_n, p_n})(e) \\
&= f(h(a)\phi_{i_1}(p_1) \ldots \phi_{i_n}(p_n))(e),
\end{align*}
$$
nghĩa là $\sigma = f(\Phi(\sigma))(e)$. Điều này chứng minh rằng $\Phi$ là đơn ánh.

(B) *Sự tồn tại của một phân tích*:

Cho $D$ là tập hợp các phần tử của $M$ thừa nhận một phân tích. Khi đó $e \in D$ và $M$ được sinh bởi $\bigcup_{i \in I} \phi_i(M_i)$ và do đó bởi $h(A) \cup \bigcup_{i \in I} \phi_i(P_i)$. Khi đó $D.\phi_i(P_i) \subset D$ với mọi $i \in I$; để chứng minh rằng $D = M$, do đó chỉ cần chứng minh quan hệ $D.h(A) \subset D$. Điều này suy ra từ bổ đề chính xác hơn sau đây:

#### Bổ đề 1 {#alg-i-s7-lem-1 .statement}

*Cho $i_1, \ldots, i_n$ thuộc $I$ và $p_\alpha$ thuộc $P_{i_\alpha}$ với $1 \leq \alpha \leq n$. Với mọi $a \in A$ tồn tại $a' \in A$ và một dãy $(p'_\alpha)_{1 \leq \alpha \leq n}$ với $p'_\alpha \in P_{i_\alpha}$ sao cho*
$$
\phi_{i_1}(p_1) \ldots \phi_{i_n}(p_n)h(a) = h(a')\phi_{i_1}(p'_1) \ldots \phi_{i_n}(p'_n).
$$
$h(a) = \phi_{i_n}(h_{i_n}(a))$ và tồn tại $a_n \in A$ và $p'_n \in P_{i_n}$ sao cho
$$
p_n \cdot h_{i_n}(a) = h_{i_n}(a_n) \cdot p'_n.
$$
Suy ra rằng $\phi_{i_n}(p_n)h(a) = h(a_n)\phi_{i_n}(p'_n)$, do đó
$$
\phi_{i_1}(p_1) \ldots \phi_{i_{n-1}}(p_{n-1})\phi_{i_n}(p_n)h(a) = \phi_{i_1}(p_1) \ldots \phi_{i_{n-1}}(p_{n-1})h(a_n)\phi_{i_n}(p'_n);
$$
bổ đề suy ra từ điều này bằng quy nạp theo $n$.

(C) *Kết thúc chứng minh*:

Cho $x \in M$ và $n$ là độ dài nhỏ nhất của các phân tích của $x$. Ta sẽ chứng minh rằng mọi phân tích $\sigma$ của $x$ có độ dài $n$ đều là thu gọn. Điều này sẽ thiết lập sự tồn tại của một phân tích thu gọn của $x$; tính duy nhất của phân tích thu gọn sau đó suy ra $l(\sigma') > l(\sigma)$ đối với mọi phân tích $\sigma' \neq \sigma$ của $x$.

Trường hợp $n = 0$ là tầm thường, giả sử $n > 0$. Cho
$$
\sigma = (a; i_1, \ldots, i_n; p_1, \ldots, p_n)
$$
là một phân tích của $x$ có độ dài $n$. Nếu tồn tại một số nguyên $\alpha$ với $1 \leq \alpha \leq n$ và $p_\alpha = e_{i_\alpha}$, dãy
$$
(a; i_1, \ldots, i_{\alpha-1}, i_{\alpha+1}, \ldots, i_n; p_1, \ldots, p_{\alpha-1}, p_{\alpha+1}, \ldots, p_n)
$$

sẽ là một phân tích của $x$ có độ dài $n - 1$, điều này bị loại trừ. Giả sử tồn tại một số nguyên $\alpha$ với $1 \leq \alpha < n$ và $i_{\alpha} = i_{\alpha + 1}$ và cho
$$
p_{\alpha} p_{\alpha + 1} = h_{i_{\alpha}}(a') \cdot p'_{\alpha}
$$
với $a' \in \mathbf{A}$ và $p'_{\alpha} \in P_{i_{\alpha}}$; theo Bổ đề 1 tồn tại các phần tử $a'' \in \mathbf{A}$,
$$
p'_{1} \in P_{i_{1}}, \ldots, p'_{\alpha - 1} \in P_{i_{\alpha - 1}}
$$
sao cho
$$
\phi_{i_{1}}(p_{1}) \cdots \phi_{i_{\alpha - 1}}(p_{\alpha - 1}) h(a') = h(a'') \phi_{i_{1}}(p'_{1}) \cdots \phi_{i_{\alpha - 1}}(p'_{\alpha - 1})
$$
và dãy
$$
(aa''; i_{1}, \ldots, i_{\alpha - 1}, i_{\alpha}, i_{\alpha + 2}, \ldots, i_{n}; p'_{1}, \ldots, p'_{\alpha - 1}, p'_{\alpha}, p_{\alpha + 2}, \ldots, p_{n})
$$
là một phân tích của $x$ có độ dài $n - 1$, điều này mâu thuẫn.

Như vậy ta đã chứng minh rằng $\sigma$ là thu gọn.

#### Hệ quả {#alg-i-s7-n3-cor-1 .statement}

*Dưới giả thiết (A) các đồng cấu $\phi_{i}$ và $h$ là đơn ánh. Với $i \neq j$ trong $I$, $\phi_{i}(M_{i}) \cap \phi_{j}(M_{j}) = h(\mathbf{A})$.*

Trước hết $h$ là đơn ánh: nếu $h(a) = h(a')$, thì $(a)$ và $(a')$ là hai phân tích thu gọn của cùng một phần tử của $M$, do đó $a = a'$. Cho $i \in I$; khi đó $h(\mathbf{A}) = \phi_{i}(h_{i}(\mathbf{A})) \subset \phi_{i}(M_{i})$; tính duy nhất của các phân tích thu gọn suy ra
$$
h(\mathbf{A}) \cap \phi_{i}(M_{i} - h_{i}(\mathbf{A})) = \varnothing,
$$
do đó $\phi_{i}(M_{i} - h_{i}(\mathbf{A})) = \phi_{i}(M_{i}) - h(\mathbf{A})$.

Tính đơn ánh của các đồng cấu $\phi_{i}$ và quan hệ
$$
\phi_{i}(M_{i}) \cap \phi_{j}(M_{j}) \subset h(\mathbf{A})
$$
với $i \neq j$ khi đó là các hệ quả của sự kiện sau: với $i, j$ thuộc $I$, $x$ thuộc $M_{i} - h_{i}(\mathbf{A})$ và $y$ thuộc $M_{j} - h_{j}(\mathbf{A})$, quan hệ $\phi_{i}(x) = \phi_{j}(y)$ kéo theo $i = j$ và $x = y$. Cho $x = h_{i}(a) \cdot p$ và $y = h_{j}(b) \cdot q$ với $a, b$ thuộc $\mathbf{A}$, $p$ thuộc $P_{i} - \{e_{i}\}$ và $y$ thuộc $P_{j} - \{e_{j}\}$. Khi đó $\phi_{i}(x) = h(a)\phi_{i}(p)$ và $\phi_{j}(y) = h(b)\phi_{j}(q)$ và do đó $(a; i; p)$ và $(b; j; q)$ là hai phân tích rút gọn của cùng một phần tử của $M$. Suy ra $i = j, a = b$ và $p = q$, do đó $x = h_{i}(a)p = h_{j}(b)q = y$.

Khi giả thiết (A) được thỏa mãn, ta sẽ đồng nhất mỗi monoid $M_{i}$ với một monoid con của $M$ thông qua $\phi_{i}$; tương tự, ta sẽ đồng nhất $\mathbf{A}$ với một monoid con của $M$ bởi $h$. Khi đó $M$ được sinh bởi $\bigcup_{i \in I} M_{i}$ và $M_{i} \cap M_{j} = \mathbf{A}$ với $i \neq j$.

Mỗi phần tử của $M$ có thể được viết duy nhất dưới dạng $a \prod_{\alpha = 1}^{n} p_{\alpha}$ với $a \in \mathbf{A}, p_{1} \in P_{i_{1}} - \{e\}, \ldots, p_{n} \in P_{i_{n}} - \{e\}$ và $i_{\alpha} \neq i_{\alpha + 1}$ với $1 \leq \alpha < n$. Cuối cùng, nếu $M'$ là một monoid và $(f_{i}: M_{i} \to M')$ (với $i \in I$) là một họ các đồng cấu mà các hạn chế của chúng lên $\mathbf{A}$ là cùng một đồng cấu của $\mathbf{A}$ vào $M'$, thì tồn tại duy nhất một đồng cấu $f: M \to M'$ cảm sinh $f_{i}$ trên $M_{i}$ với mọi $i \in I$.

Giả thiết (A) được thỏa mãn trong hai trường hợp quan trọng:

(a) $A = \{e\}$. Trong trường hợp này, có một họ $(M_i)_{i \in I}$ các monoid và $M$ được gọi là tổng monoid của họ này. Mỗi $M_i$ được đồng nhất với một monoid con của $M$ và $M$ được sinh bởi $\bigcup_{i \in I} M_i$; hơn nữa, $M_i \cap M_j = \{e\}$ với $i \neq j$. Mọi phần tử của $M$ có thể được viết duy nhất dưới dạng $x_1 \ldots x_n$ với
$$
x_1 \in M_{i_1} - \{e\}, \ldots, x_n \in M_{i_n} - \{e\}
$$
và $i_\alpha \neq i_{\alpha+1}$ với $1 \leq \alpha \leq n$. Cuối cùng, với mọi họ các đồng cấu $(f_i : M_i \to M')$, tồn tại một đồng cấu duy nhất $f : M \to M'$ mà hạn chế của nó trên $M_i$ là $f_i$ với mọi $i \in I$.

(b) Có một họ các nhóm $(G_i)_{i \in I}$ chứa cùng nhóm $A$ như nhóm con và $h_i$ là đơn ánh của $A$ vào $G_i$. Tổng của họ $(G_i)_{i \in I}$ ghép lại bởi $A$ khi đó là một *nhóm* $G$ : monoid $G$ được sinh bởi $\bigcup_{i \in I} \phi_i(G_i)$ và mọi phần tử của $\bigcup_{i \in I} \phi_i(G_i)$ đều nhận một phần tử nghịch đảo trong $G$ (xem § 2, no. 3, Hệ quả 1 của Mệnh đề 4); nó được ký hiệu bởi $*_A G_i$ hoặc $G_1 *_A G_2$ khi $I = \{1, 2\}$. Khi $A$ gồm phần tử đơn vị, người ta cũng nói rằng $G$ là *tích tự do của họ* $(G_i)_{i \in I}$ các nhóm và nó được ký hiệu bởi $* G_i$ (hoặc $G_1 * G_2$ nếu $I = \{1, 2\}$).†

### 4. ỨNG DỤNG VÀO CÁC MONOID TỰ DO

#### Bổ đề 2 {#alg-i-s7-lem-2 .statement}

*Cho $M$ là tổng monoid của họ $(M_x)_{x \in X}$ được xác định bởi $M_x = \mathbf{N}$ với mọi $x \in X$ và cho $\phi_x$ ký hiệu đồng cấu chính tắc của $M_x$ vào $M$. Ánh xạ $x \mapsto \phi_x(1)$ của $X$ vào $M$ mở rộng thành một đẳng cấu $h$ của $\mathrm{Mo}(X)$ lên $M$.*

Cho $h$ là đồng cấu của $\mathrm{Mo}(X)$ vào $M$ được xác định bởi $h(x) = \phi_x(1)$. Với mọi số nguyên $n \geq 0$, $\phi_x(n) = \phi_x(1)^n = h(x)^n$ và vì $M$ được sinh bởi $\bigcup_{x \in X} \phi_x(\mathbf{N})$, nó cũng được sinh bởi $h(X)$. Do đó $h$ là *toàn ánh*. Hơn nữa, với mọi $x$ trong $X$, ánh xạ $n \mapsto x^n$ là một đồng cấu của $\mathbf{N} = M_x$ vào $\mathrm{Mo}(X)$; do đó tồn tại (no. 3, Mệnh đề 4) một đồng cấu $h'$ của $M$ vào $\mathrm{Mo}(X)$ sao cho $h'(\phi_x(n)) = x^n$ với $x \in X$ và $n \in \mathbf{N}$; đặc biệt, $h'(h(x)) = x$ với $x \in X$ và do đó $h' \circ h$ là đồng cấu đồng nhất của $\mathrm{Mo}(X)$. Vì vậy $h$ là *đơn ánh*. Do đó đã chứng minh được rằng $h$ là song ánh.

#### Mệnh đề 6 {#alg-i-s7-prop-6 .statement}

*Cho $w$ là một phần tử của $\mathrm{Mo}(X)$.
(a) Tồn tại một số nguyên $n \geq 0$, các phần tử $x_\alpha$ của $X$ và các số nguyên $m(\alpha) > 0$ (với

† Chú ý rằng $G_1 * G_2$ không phải là "tích" của $G_1$ và $G_2$ theo nghĩa của *Lý thuyết tập hợp*, IV, § 2, no. 4 (cũng không theo nghĩa của "lý thuyết phạm trù"; trong ngữ cảnh của lý thuyết này, $G_1 * G_2$ là "tổng" của $G_1$ và $G_2$).

$1 \leq \alpha \leq n$ sao cho $x_\alpha \neq x_{\alpha+1}$ với $1 \leq \alpha < n$ và $w = \prod_{\alpha=1}^n x_\alpha^{m(\alpha)}$. Dãy $(x_\alpha, m(\alpha))_{1 \leq \alpha \leq n}$ được xác định duy nhất bởi các điều kiện này.

(b) Cho $p$ là một số nguyên dương, $x'_\beta$ trong $X$ và $m'(\beta)$ trong $\mathbf{N}$ với $1 \leq \beta \leq p$ sao cho $w = \prod_{\beta=1}^p {x'}^{m'(\beta)}$. Khi đó $p \geq n$. Nếu $p = n$, thì $x'_\beta = x_\beta$ và $m'(\beta) = m(\beta)$ với $1 \leq \beta \leq p$.

Theo ký hiệu của Bổ đề 2, $h^{-1}(\phi_x(n)) = x^n$ với $x \in X$ và $n \in \mathbf{N}$. Mệnh đề 6 khi đó suy ra từ no. 3, Mệnh đề 5.

### 5. NHÓM TỰ DO

Cho $G_x = \mathbf{Z}$ với mọi $x \in X$. Tích tự do của họ $(G_x)_{x \in X}$ được gọi là *nhóm tự do được xây dựng trên* $X$ và được ký hiệu bởi $F(X)$. Gọi $\phi_x$ là đồng cấu chính tắc của $G_x = \mathbf{Z}$ vào $F(X)$. Theo no. 3, Hệ quả của Mệnh đề 5, ánh xạ $x \mapsto \phi_x(1)$ của $X$ vào $F(X)$ là đơn ánh; ta sẽ đồng nhất $X$ với ảnh của nó trong $F(X)$ qua ánh xạ này. Khi đó $X$ sinh $F(X)$ và $e \notin X$.

Áp dụng no. 3, Mệnh đề 5, ta thu được kết quả sau:

#### Mệnh đề 7 {#alg-i-s7-prop-7 .statement}

*Cho g là một phần tử của nhóm tự do* $F(X)$. *Tồn tại một số nguyên* $n \geq 0$ *và một dãy* $(x_\alpha, m(\alpha))_{1 \leq \alpha \leq n}$ *được xác định duy nhất bởi các hệ thức* $x_\alpha \in X$, $x_\alpha \neq x_{\alpha+1}$ *với* $1 \leq \alpha < n$, $m(\alpha) \in \mathbf{Z}$, $m(\alpha) \neq 0$ *với* $1 \leq \alpha \leq n$, *và* $g = \prod_{\alpha=1}^n x_\alpha^{m(\alpha)}$.

Nhóm tự do $F(X)$ có tính chất phổ quát sau:

#### Mệnh đề 8 {#alg-i-s7-prop-8 .statement}

*Cho G là một nhóm và f là một ánh xạ của* $X$ *vào G. Tồn tại một và chỉ một đồng cấu* $\bar{f}$ *của* $F(X)$ *vào G mở rộng f*.

Tính duy nhất của $\bar{f}$ suy ra từ sự kiện rằng nhóm $F(X)$ được sinh bởi $X$. Với mọi $x$ trong $X$, gọi $f_x$ là đồng cấu $n \mapsto f(x)^n$ của $\mathbf{Z}$ vào $G$. Theo no. 3, Mệnh đề 4, tồn tại một đồng cấu $\bar{f}$ của $F(X)$ vào $G$ sao cho $\bar{f}(x^n) = f_x(n)$ với $x \in X$ và $n \in \mathbf{Z}$; đặc biệt, $\bar{f}(x) = f_x(1) = f(x)$ với mọi $x \in X$ và do đó $\bar{f}$ mở rộng $f$.

Cho $u : X \to Y$ là một ánh xạ. Theo Mệnh đề 8, tồn tại một và chỉ một đồng cấu của $F(X)$ vào $F(Y)$ trùng với $u$ trên $X$; nó được ký hiệu bởi $F(u)$. Như trong trường hợp của các magma (no. 1), công thức

$$
F(v \circ u) = F(v) \circ F(u)
$$

được thiết lập cho mọi ánh xạ $v : Y \to Z$ và ta chứng minh rằng $F(u)$ là đơn ánh (tương ứng toàn ánh, song ánh) nếu $u$ là đơn ánh (tương ứng toàn ánh, song ánh). Với mọi tập con $S$ của $X$, $F(S)$ sẽ được đồng nhất với nhóm con của $F(X)$ sinh bởi $S$.

Cho I là một tập hợp. Trong một số trường hợp, người ta quan tâm đến việc không đồng nhất $i$ trong I với ảnh chính tắc $\phi_i(1)$ của nó trong nhóm tự do $F(I)$; phần tử sau sẽ được ký hiệu là $T_i$ (hoặc $T'_i, X_i, \ldots$ tùy trường hợp) và được gọi là *bất định* có chỉ số $i$. Khi đó nhóm tự do $F(I)$ được ký hiệu là $F((T_i)_{i \in I})$ hoặc $F(T_1, \ldots, T_n)$ nếu $I = \{1, 2, \ldots, n\}$.

Cho $G$ là một nhóm và $t = (t_i)_{i \in I}$ là một họ các phần tử của $G$. Theo Mệnh đề 8 tồn tại một đồng cấu $f_t$ của $F((T_i)_{i \in I})$ vào $G$ được đặc trưng bởi $f_t(T_i) = t_i$ với mọi $i \in I$. Ảnh của một phần tử $w$ của $F((T_i)_{i \in I})$ qua $f_t$ sẽ được ký hiệu là $w(t)$ hoặc $w(t_1, \ldots, t_n)$ nếu $I = \{1, 2, \ldots, n\}$; $w(t)$ được nói là thu được từ *phép thế* $T_i \mapsto t_i$ trong $w$. Đặc biệt, nếu ta lấy $G = F((T_i)_{i \in I})$ và $(t_i) = (T_i) = T, f_T$ là đồng cấu đồng nhất của $G$, do đó $w(T) = w$; với $I = \{1, 2, \ldots, n\}$, khi đó $w(T_1, \ldots, T_n) = w$.

Cho $G$ và $G'$ là hai nhóm, $u$ là một đồng cấu của $G$ vào $G'$ và $t = (t_1, \ldots, t_n)$ là một dãy hữu hạn các phần tử của $G$. Đặt $t' = (u(t_1), \ldots, u(t_n))$; đồng cấu $u \circ f_t$ của $F(T_1, \ldots, T_n)$ vào $G'$ ánh xạ $T_i$ thành $u(t_i)$ với $1 \leq i \leq n$ và do đó bằng $f_{t'}$; với $w$ trong $F(T_1, \ldots, T_n)$, khi đó

$$
u(w(t_1, \ldots, t_n)) = w(u(t_1), \ldots, u(t_n)).
$$

Cho $w$ là một phần tử đã cho trong $F(T_1, \ldots, T_n)$ và $v_1, \ldots, v_n$ là các phần tử của nhóm tự do $F(T'_1, \ldots, T'_m)$. Phép thế $T_i \mapsto v_i$ xác định một phần tử $w' = w(v_1, \ldots, v_n)$ của $F(T'_1, \ldots, T'_m)$. Cho $G$ là một nhóm, $t_1, \ldots, t_m$ là các phần tử của $G$ và $u$ là đồng cấu từ $F(T'_1, \ldots, T'_m)$ vào $G$ được đặc trưng bởi $u(T'_j) = t_j$ với $1 \leq j \leq m$. Khi đó $u(v_i) = v_i(t_1, \ldots, t_m)$ và $u(w') = w(t_1, \ldots, t_m)$; do đó công thức (8) suy ra

$$
w'(t_1, \ldots, t_m) = w(v_1(t_1, \ldots, t_m), \ldots, v_n(t_1, \ldots, t_m)).
$$

Điều này giải thích "ký hiệu phiếm hàm" $w(t_1, \ldots, t_n)$. Người đọc được yêu cầu mở rộng các công thức (8) và (9) sang trường hợp các tập chỉ số tùy ý.

### 6. CÁC TRÌNH BÀY CỦA MỘT NHÓM

Cho $G$ là một nhóm và $t = (t_i)_{i \in I}$ là một họ các phần tử của $G$. Cho $f_t$ là đồng cấu duy nhất từ nhóm tự do $F(I)$ vào $G$ biến $i$ thành $t_i$. Ảnh của $f_t$ là nhóm con sinh bởi các phần tử $t_i$ của $G$. Các phần tử của hạt nhân của $f_t$ được gọi là *các từ quan hệ* của họ $t$. $t$ được gọi là *sinh* (tương ứng *tự do*, *cơ sở*) nếu $f_t$ là toàn ánh (tương ứng đơn ánh, song ánh).

Cho $G$ là một nhóm. Một *trình bày* của $G$ là một cặp có thứ tự $(\mathbf{t}, \mathbf{r})$ gồm một họ sinh $\mathbf{t} = (t_i)_{i \in I}$ và một họ $\mathbf{r} = (r_j)_{j \in J}$ các từ quan hệ sao cho hạt nhân $N_t$ của $f_t$ được sinh bởi các phần tử $gr_jg^{-1}$ với $g \in F(I)$ và $j \in J$. Nói cách khác, điều này tương đương với việc nói rằng $N_t$ là nhóm con chuẩn tắc của $F(I)$ sinh bởi các $r_j$ với $j \in J$ (nói cách khác, nhóm con chuẩn tắc nhỏ nhất của $F(I)$ chứa các phần tử $r_j$ ($j \in J$), xem § 4, no. 4). Theo một cách dùng ngôn ngữ hơi lạm dụng, các phần tử sinh $t_i$ và các quan hệ $r_j(\mathbf{t}) = e$ được nói là lập thành một *trình bày* của nhóm $G$.

Cho I là một tập hợp và $r = (r_j)_{j \in J}$ là một họ các phần tử của nhóm tự do $F(I)$. Gọi $N(r)$ là nhóm con chuẩn của $F(I)$ sinh bởi các $r_j$ với $j \in J$. Đặt $F(I, r) = F(I)/N(r)$ và ký hiệu $\tau_i$ là lớp của $i$ modulo $N(r)$. Cặp có thứ tự $(\tau, r)$ với $\tau = (\tau_i)_{i \in I}$ là một phép trình bày của nhóm $F(I, r)$; nếu $G$ là một nhóm và $(t, r)$ là một phép trình bày của $G$ với $t = (t_i)_{i \in I}$, tồn tại một đẳng cấu duy nhất $u$ của $F(I, r)$ lên $G$ sao cho $u(\tau_i) = t_i$ với mọi $i \in I$. Nhóm $F(I, r)$ được gọi là được xác định bởi các phần tử sinh $\tau_i$ và các hệ thức $r_j$, hoặc bằng một sự lạm dụng ngôn ngữ, là *được xác định bởi các phần tử sinh $\tau_i$ và các quan hệ* $r_j(\tau) = e$. Khi $I = \{1, n\}$ và $J = \{1, m\}$, ta nói rằng $F(I, r)$ được xác định bởi phép trình bày

$$
\langle \tau_1, \ldots, \tau_n; r_1, \ldots, r_m \rangle.
$$

Nếu $r_j = u_j^{-1} v_j$ với $u_j$ và $v_j$ thuộc $F(I)$, phép trình bày này cũng được ký hiệu bằng ký hiệu

$$
\langle \tau_1, \ldots, \tau_n; u_1 = v_1, \ldots, u_m = v_m \rangle.
$$

#### Ví dụ {#alg-i-s7-n6-exa-1 .statement}

(1) Nhóm được xác định bởi phép trình bày $\langle \tau; \tau^q = e \rangle$ là xyclic có cấp $q$.

(2) Nhóm được xác định bởi phép trình bày $\langle x, y; xy = yx \rangle$ là đẳng cấu với $\mathbf{Z} \times \mathbf{Z}$.

#### Mệnh đề 9 {#alg-i-s7-prop-9 .statement}

*Cho $G$ là một nhóm, $t = (t_i)_{i \in I}$ là một họ sinh của $G$ và $r = (r_j)_{j \in J}$ là một họ các hệ thức của $t$. Các điều kiện sau là tương đương:*

(a) *Cặp có thứ tự* $(t, r)$ *là một phép trình bày của* $G$.

(b) *Cho* $G'$ *là một nhóm và* $t' = (t'_i)_{i \in I}$ *là một họ các phần tử của* $G'$. *Nếu* $r_j(t') = e$ *với mọi* $j \in J$, *tồn tại một đồng cấu* $u$ *của* $G$ *vào* $G'$ *sao cho* $u(t_i) = t'_i$ *với mọi* $i \in I$.

(c) *Cho* $\overline{G}$ *là một nhóm và* $\bar{t} = (\bar{t}_i)_{i \in I}$ *là một họ sinh của* $\overline{G}$ *sao cho* $r_j(\bar{t}) = e$ *với mọi* $j \in J$. *Mọi đồng cấu của* $\overline{G}$ *vào* $G$ *ánh xạ* $\bar{t}_i$ *thành* $t_i$ *với mọi* $i \in I$ *đều là một đẳng cấu*.

Ký hiệu $f$ là đồng cấu của $F(I)$ vào $G$ ánh xạ $i$ thành $t_i$ với mọi $i \in I$ và $N$ là hạt nhân của $f$.

(a) $\Rightarrow$ (b): Giả sử rằng $(t, r)$ là một biểu diễn của $G$ và $t' = (t'_i)_{i \in I}$ là một họ các phần tử của một nhóm $G'$ sao cho $r_j(t') = e$ với mọi $j \in J$. Gọi $f'$ là đồng cấu của $F(I)$ vào $G'$ được xác định bởi $f'(i) = t'_i$ với mọi $i \in I$. Theo giả thiết, $f'(r_j) = e$ với mọi $j \in J$ và, vì $N$ được sinh bởi các phần tử $gr_jg^{-1}$ với $j \in J$ và $g \in F(I), f'(N) = \{e\}$. Vì đồng cấu $f \colon F(I) \to G$ là toàn ánh với hạt nhân $N$, tồn tại một đồng cấu $u \colon G \to G'$ sao cho $f' = u \circ f$. Khi đó $u(t_i) = u(f(i)) = f'(i) = t'_i$.

(b) $\Rightarrow$ (c): Giả sử điều kiện (b) đúng. Cho $t = (t_i)_{i \in I}$ là một họ sinh của một nhóm $G$ sao cho $r_j(t) = e$ với mọi $j \in J$ và cho $v$ là một đồng cấu từ $\overline{G}$ vào $G$ sao cho $v(\bar{t}_i) = t_i$ với mọi $i \in I$. Vì họ $(t_i)_{i \in I}$ sinh ra $G$, đồng cấu $v$ là *toàn ánh*. Theo tính chất (b) tồn tại một đồng cấu $u \colon G \to \overline{G}$ sao cho $u(t_i) = \bar{t}_i$ với mọi $i \in I$. Khi đó $u(v(\bar{t}_i)) = \bar{t}_i$ với mọi $i \in I$ và do đó $u \circ v$ là đồng nhất trên $\overline{G}$, điều này chứng minh rằng $v$ là đơn ánh. Vì vậy $v$ là một đẳng cấu và điều kiện (c) đúng.

(c) $\Rightarrow$ (a): Giả sử điều kiện (c) đúng. Cho $t'_i$ là ảnh chính tắc của $i$ trong $F(I, r)$ và $t' = (t'_i)_{i \in I}$; khi đó $r_j(t') = e$ với mọi $j \in J$. Vì $r_j(t) = e$ với mọi $j \in J$, tồn tại duy nhất một đồng cấu $v$ từ $F(I, r)$ vào $G$ sao cho $v(t_i) = t_i$ với mọi $i \in I$. Theo (c), $v$ là một đẳng cấu từ $F(I, r)$ lên $G$ biến cách trình bày $(t', r)$ của $F(I, r)$ thành một cách trình bày $(t, r)$ của $G$.

### 7. CÁC NHÓM GIAO HOÁN TỰ DO VÀ CÁC VỊ NHÓM

Tập hợp $\mathbf{Z}^X$ gồm tất cả các ánh xạ từ $X$ vào $\mathbf{Z}$ là một nhóm giao hoán theo luật xác định bởi $(\alpha + \beta)(x) = \alpha(x) + \beta(x)$ ($\alpha, \beta \in \mathbf{Z}^X, x \in X$); các phần tử của $\mathbf{Z}^X$ đôi khi được gọi là đa chỉ số. Phần tử đơn vị, ký hiệu bởi 0, là ánh xạ hằng có giá trị 0. Với $\alpha \in \mathbf{Z}^X$, tập hợp $S_\alpha$ gồm các $x \in X$ sao cho $\alpha(x) \neq 0$ được gọi là giá của $\alpha$; khi đó $S_0 = \varnothing$ và $S_{\alpha+\beta} \subset S_\alpha \cup S_\beta$ đối với $\alpha, \beta$ trong $\mathbf{Z}^X$. Do đó tập hợp $\mathbf{Z}^{(X)}$ gồm các ánh xạ $\alpha : X \to \mathbf{Z}$ có giá hữu hạn là một nhóm con của $\mathbf{Z}^X$ được gọi là nhóm giao hoán tự do được xây dựng trên $X$.

Với mọi $x \in X$, ký hiệu $\delta_x$ là phần tử của $\mathbf{Z}^{(X)}$ được xác định bởi

$$
\delta_x(y) = \begin{cases}
1 & \text{nếu } y = x \\
0 & \text{nếu } y \neq x.
\end{cases}
$$

Ngoài ra, với $\alpha \in \mathbf{Z}^{(X)}$, số nguyên $|\alpha|$, độ dài của $\alpha$ được định nghĩa bởi công thức

$$
|\alpha| = \sum_{x \in X} \alpha(x).
$$

Các quan hệ sau được thiết lập ngay lập tức:

$$
\alpha = \sum_{x \in X} \alpha(x) \cdot \delta_x
$$
$$
|\delta_x| = 1, \quad |0| = 0
$$
$$
|\alpha + \beta| = |\alpha| + |\beta|
$$

với $\alpha, \beta$ trong $\mathbf{Z}^{(X)}$ và $x$ trong $X$.

Quan hệ thứ tự $\alpha \leq \beta$ được định nghĩa trong $\mathbf{Z}^{(X)}$ bởi $\alpha(x) \leq \beta(x)$ với mọi $x \in X$. Các quan hệ $\alpha \leq \beta$ và $\alpha' \leq \beta'$ kéo theo $\alpha + \alpha' \leq \beta + \beta'$, $|\alpha| \leq |\beta|$ và $-\alpha \geq -\beta$; hơn nữa, quan hệ $\alpha \leq \beta$ tương đương với $\beta - \alpha \geq 0$. Tập hợp các phần tử $\alpha \geq 0$ trong $\mathbf{Z}^{(X)}$ được ký hiệu là $\mathbf{N}^{(X)}$; đó là tập hợp các ánh xạ từ $X$ vào $\mathbf{N}$ có giá hữu hạn và là một monoid con của $\mathbf{Z}^{(X)}$ được gọi là monoid giao hoán tự do được xây dựng trên $X$. Các phần tử có độ dài 1 là các phần tử cực tiểu trong $\mathbf{N}^{(X)} - \{0\}$ và lập thành tập hợp các $\delta_x$ ($x \in X$).

Monoid $\mathbf{N}^{(X)}$ và nhóm $\mathbf{Z}^{(X)}$ có tính chất phổ quát sau đây.

#### Mệnh đề 10 {#alg-i-s7-prop-10 .statement}

*Cho M là một nửa nhóm giao hoán (tương ứng nhóm) và f là một ánh xạ từ X vào M. Tồn tại một và chỉ một đồng cấu từ $\mathbf{N}^{(X)}$ (tương ứng $\mathbf{Z}^{(X)}$) vào M sao* cho $g(\delta_x) = f(x)$ với mọi $x \in X$. *Nếu M được viết theo phép cộng, thì* $g(\alpha) = \sum_{x \in X} \alpha(x) \cdot f(x)$ với mọi $\alpha$ trong $\mathbf{N}^{(X)}$ (tương ứng $\mathbf{Z}^{(X)}$).

Cho $g$ là một đồng cấu từ $\mathbf{N}^{(X)}$ (tương ứng $\mathbf{Z}^{(X)}$) vào M sao cho $g(\delta_x) = f(x)$ với mọi $x \in X$. Với mọi $\alpha$ trong $\mathbf{N}^{(X)}$ (tương ứng $\mathbf{Z}^{(X)}$), từ (12) suy ra rằng
$$
g(\alpha) = \sum_{x \in X} \alpha(x) \cdot g(\delta_x) = \sum_{x \in X} \alpha(x) \cdot f(x),
$$
do đó tính duy nhất của $g$.

Với mọi $\alpha$ trong $\mathbf{N}^{(X)}$ (tương ứng $\mathbf{Z}^{(X)}$) ta viết $g(\alpha) = \sum_{x \in X} \alpha(x) \cdot f(x)$. Khi đó hiển nhiên $g(0) = 0$; với $\alpha, \beta$ trong $\mathbf{N}^{(X)}$ (tương ứng $\mathbf{Z}^{(X)}$),
$$
\begin{align*}
g(\alpha + \beta) &= \sum_{x \in X} (\alpha(x) + \beta(x)) \cdot f(x) \\
&= \sum_{x \in X} [\alpha(x) \cdot f(x) + \beta(x) \cdot f(x)] \\
&= \sum_{x \in X} \alpha(x) \cdot f(x) + \sum_{x \in X} \beta(x) \cdot f(x) \\
&= g(\alpha) + g(\beta)
\end{align*}
$$
và do đó $g$ là một đồng cấu từ $\mathbf{N}^{(X)}$ (tương ứng $\mathbf{Z}^{(X)}$) vào M. Ngoài ra, với $y$ trong $X$,
$$
g(\delta_y) = \sum_{x \in X} \delta_y(x) \cdot f(x);
$$
bây giờ $\delta_y(x) \cdot f(x) = 0$ với $x \neq y$ và $\delta_y(y) \cdot f(y) = f(y)$, do đó $g(\delta_y) = f(y)$.

Cho $u : X \to Y$ là một ánh xạ. Theo Mệnh đề 10 tồn tại một và chỉ một đồng cấu từ $\mathbf{Z}^{(X)}$ vào $\mathbf{Z}^{(Y)}$ ánh xạ $\delta_x$ thành $\delta_{u(x)}$ với mọi $x \in X$. Nó được ký hiệu là $\mathbf{Z}^{(u)}$; thấy ngay rằng nó ánh xạ $\alpha \in \mathbf{Z}^{(X)}$ thành phần tử $\beta \in \mathbf{Z}^{(Y)}$ được xác định bởi
$$
\beta(y) = \sum_{x \in u^{-1}(y)} \alpha(x).
$$
Như trong trường hợp của các magma (no. 1), công thức $\mathbf{Z}^{(v \circ u)} = \mathbf{Z}^{(v)} \circ \mathbf{Z}^{(y)}$ được thiết lập với mọi ánh xạ $v : Y \to Z$; cũng chứng minh được rằng $\mathbf{Z}^{(u)}$ là đơn ánh (tương ứng toàn ánh, song ánh) nếu $u$ là như vậy.

Cho S là một tập con của X; nếu i là đơn ánh từ S vào X, ánh xạ $f = \mathbf{Z}^{(i)}$ là một đẳng cấu từ $\mathbf{Z}^{(S)}$ lên nhóm con H của $\mathbf{Z}^{(X)}$ sinh bởi các phần tử $\delta_s$ với $s \in S$. Theo (15),
$$
(f(\alpha))(x) = \begin{cases}
\alpha(x) & \text{nếu } x \in S \\
0 & \text{nếu } x \in X - S
\end{cases}
$$

và do đó $H$ là tập hợp các phần tử của $\mathbf{Z}^{(X)}$ có giá chứa trong $S$. Kể từ đây $\mathbf{Z}^{(S)}$ sẽ được đồng nhất với $H$ nhờ vào $f$.

Công thức (15) chỉ ra rằng hạn chế của $\mathbf{Z}^{(u)}$ lên $\mathbf{N}^{(X)}$ cảm sinh một đồng cấu $\mathbf{N}^{(u)}$ của $\mathbf{N}^{(X)}$ vào $\mathbf{N}^{(Y)}$. Khi đó $\mathbf{N}^{(v \circ u)} = \mathbf{N}^{(v)} \circ \mathbf{N}^{(u)}$ với mọi ánh xạ $v : Y \to Z$; hơn nữa, $\mathbf{N}^{(u)}$ là đơn ánh (tương ứng toàn ánh, song ánh) nếu $u$ là như vậy. Nếu $S$ là một tập con của $X$,

$$
\mathbf{N}^{(S)} = \mathbf{Z}^{(S)} \cap \mathbf{N}^{(X)}.
$$

#### Nhận xét {#alg-i-s7-n7-rem-1 .statement}

Cho $M$ là monoid nhân của các số nguyên dương ngặt và cho $\mathfrak{P}$ là tập hợp các số nguyên tố (\S 4, no. 10, Định nghĩa 15). Theo Mệnh đề 10 tồn tại một đồng cấu $u$ của $\mathbf{N}^{(\mathfrak{P})}$ vào $M$ được đặc trưng bởi $u(\delta_p) = p$ với mọi số nguyên tố $p$. Khi đó $u(\alpha) = \prod_{p \in \mathfrak{P}} p^{\alpha(p)}$ với $\alpha$ trong $\mathbf{N}^{(\mathfrak{P})}$ và Định lý 7 của \S 4, no. 10 chỉ ra rằng $u$ là một đẳng cấu của $\mathbf{N}^{(\mathfrak{P})}$ lên $H$.

### 8. KÝ HIỆU LŨY THỪA

Cho $M$ là một monoid, được viết theo phép nhân, và $u = (u_x)_{x \in X}$ là một họ các phần tử của $M$, giao hoán từng đôi một. Cho $\alpha$ thuộc $\mathbf{N}^{(X)}$; các phần tử $u_x^{\alpha(x)}$ và $u_y^{\alpha(y)}$ của $M$ giao hoán với $x, y$ thuộc $X$ và tồn tại một tập con hữu hạn $S$ của $X$ sao cho $u_x^{\alpha(x)} = 1$ với $x$ thuộc $X - S$. Do đó ta có thể viết:

$$
u^\alpha = \prod_{x \in X} u_x^{\alpha(x)}.
$$

Cho $M'$ là monoid con của $M$ sinh bởi họ $(u_x)_{x \in X}$; nó là giao hoán (\S 1, no. 5, Hệ quả 2 của Mệnh đề 4). Vì vậy tồn tại (no. 7, Mệnh đề 10) một đồng cấu duy nhất $f$ của $\mathbf{N}^{(X)}$ vào $M'$ sao cho $f(\delta_x) = u_x$ với mọi $x \in X$ và $f(\alpha) = u^\alpha$ với mọi $\alpha$ trong $\mathbf{N}^{(X)}$. Ta suy ra các công thức sau đây

$$
u^{\alpha + \beta} = u^\alpha . u^\beta
$$
$$
u^0 = 1
$$
$$
u^{\delta_x} = u_x
$$

với $\alpha, \beta$ trong $\mathbf{N}^{(X)}$ và $x$ trong $X$.

Cho $v = (v_x)_{x \in X}$ là một họ khác gồm các phần tử của $M$; giả sử rằng $v_x v_y = v_y v_x$ và $u_x v_y = v_y u_x$ với $x, y$ trong $X$. Khi đó tồn tại (\S 1, no. 5, Hệ quả 2 của Mệnh đề 4) một monoid con giao hoán $L$ của $M$ sao cho $u_x \in L$ và $v_x \in L$ với mọi $x \in X$. Ánh xạ $\alpha \mapsto u^\alpha . v^\alpha$ từ $\mathbf{N}^{(X)}$ vào $L$ khi đó là một đồng cấu (\S 1, no. 5, Mệnh đề 5) gửi $\delta_x$ đến $u_x . v_x$. Do đó ta có công thức

$$
u^\alpha . v^\alpha = (u . v)^\alpha,
$$

trong đó $u . v$ là họ $(u_x . v_x)_{x \in X}$.

Khi M giao hoán, $u^\alpha$ có thể được định nghĩa cho mọi họ $u$ các phần tử của M và các công thức (15) đến (20) đúng không bị hạn chế.

### 9. CÁC MỐI LIÊN HỆ GIỮA CÁC ĐỐI TƯỢNG TỰ DO KHÁC NHAU

Vì monoid tự do Mo(X) là một magma, Mệnh đề 1 của no. 1 cho thấy tồn tại một đồng cấu $\lambda : M(X) \to Mo(X)$ có hạn chế trên X là ánh xạ đồng nhất. Tương tự, vì nhóm tự do F(X) là một monoid, ánh xạ đồng nhất của X mở rộng thành một đồng cấu $\mu : Mo(X) \to F(X)$ (no. 2, Mệnh đề 3). Theo no. 4, Mệnh đề 6 và no. 5, Mệnh đề 7, $\mu$ là đơn ánh. Tương tự, Mệnh đề 10 của no. 7 và Mệnh đề 8 của no. 5 cho thấy tồn tại các đồng cấu $\nu : Mo(X) \to N^{(X)}$ và $\pi : F(X) \to Z^{(X)}$ được đặc trưng bởi $\nu(x) = \delta_x$ và $\pi(x) = \delta_x$ với mọi $x \in X$. Nếu $i$ là phép đơn ánh từ $N^{(X)}$ vào $Z^{(X)}$, thì hai đồng cấu $i \circ \nu$ và $\pi \circ \mu$ của Mo(X) vào $Z^{(X)}$ trùng nhau trên X, do đó $i \circ \nu = \pi \circ \mu$. Tình hình có thể được tóm tắt bởi biểu đồ giao hoán sau:

$$
\begin{array}{ccc}
M(X) & \xrightarrow{\lambda} & Mo(X) \\
& & \downarrow \mu \\
& & F(X) \xrightarrow{\pi} Z^{(X)}
\end{array}
$$

Các đồng cấu $\lambda, \mu, \nu$ và $\pi$ sẽ được gọi là chính tắc.

Cho w thuộc M(X); dễ dàng chứng minh bằng quy nạp theo $l(w)$ rằng độ dài của từ $\lambda(w)$ bằng độ dài của w. Hơn nữa

$$
\nu(x_1 \ldots x_n) = \sum_{i=1}^n \delta_{x_i}
$$
với $x_1, \ldots, x_n$ trong X, do đó $|\nu(x_1 \ldots x_n)| = n$ theo (13) và (14). Nói cách khác,

$$
|\nu(u)| = l(u) \quad (u \in Mo(X)).
$$

#### Mệnh đề 11 {#alg-i-s7-prop-11 .statement}

*Đồng cấu chính tắc $\nu$ của Mo(X) vào $N^{(X)}$ là toàn ánh.* Cho $w = x_1 \ldots x_n$ và $w' = x'_1 \ldots x'_m$ là hai phần tử của Mo(X); để $\nu(w) = \nu(w')$, điều kiện cần và đủ là $m = n$ và tồn tại một phép hoán vị $\sigma \in S_n$ sao cho $x'_i = x_{\sigma(i)}$ với $1 \leq i \leq n$.

Ảnh của $\nu$ là một monoid con I của $N^{(X)}$ chứa các phần tử $\delta_x$ (với $x \in X$). Công thức (12) (no. 7) cho thấy rằng $N^{(X)}$ được sinh bởi họ $(\delta_x)_{x \in X}$, trong đó $I = N^{(X)}$. Do đó $\nu$ là toàn ánh.

Nếu $m = n$ và $x'_i = x_{\sigma(i)}$ với $1 \leq i \leq n$, thì

$$
\nu(w') = \sum_{i=1}^n \delta_{x'_i} = \sum_{i=1}^n \delta_{x_{\sigma(i)}} = \sum_{i=1}^n \delta_{x_i} = \nu(w)
$$

theo công thức (21) và định lý giao hoán (§ 1, no. 5, Định lý 2).

Ngược lại, giả sử rằng $v(w)$ và $v(w')$ đều bằng cùng một phần tử $\alpha$ của $\mathbf{N}^{(X)}$; theo công thức (22), $n = |\alpha| = m$. Với mọi $x \in X$, cho $I_x$ (k. $I'_x$) là tập hợp các số nguyên $i$ sao cho $1 \leq i \leq n$ và $x_i = x$ (k. $x'_i = x$). Khi đó $(I_x)_{x \in X}$ và $(I'_x)_{x \in X}$ là các phân hoạch của khoảng $[1, n]$ của $\mathbf{N}$; hơn nữa, công thức
$$
\alpha = \sum_{i=1}^n \delta_{x_i}
$$
cho thấy rằng $\alpha(x)$ là lực lượng của $I_x$; tương tự, công thức
$$
\alpha = \sum_{i=1}^n \delta_{x'_i}
$$
cho thấy rằng $\alpha(x)$ là lực lượng của $I'_x$. Do đó tồn tại một phép hoán vị $\sigma$ của $[1, n]$ sao cho $\sigma(I'_x) = I_x$ với mọi $x \in X$, tức là $x'_i = x_{\sigma(i)}$ với $i = 1, \ldots, n$.

#### Nhận xét {#alg-i-s7-n9-rem-1 .statement}

Cho $S$ là một tập con của $X$. Nhắc lại rằng ta đã đồng nhất $M(S)$ với một submagma của $M(X)$, $Mo(S)$ với một submonoid của $Mo(X)$ và $N^{(S)}$ với một submonoid của $N^{(X)}$. Khi đó
$$
M(S) = \lambda^{-1}(Mo(S)).
$$
Rõ ràng $\lambda(M(S)) \subset Mo(S)$. Cho $w \in \lambda^{-1}(Mo(S))$; ta chứng minh bằng quy nạp theo $l(w)$ rằng $w \in M(S)$. Hiển nhiên nếu $l(w) = 1$. Nếu $l(w) > 1$, ta có thể viết $w = w_1 w_2$ với $w_1, w_2 \in M(X)$, $l(w_1) < l(w)$, $l(w_2) < l(w)$. Khi đó $\lambda(w_1) \lambda(w_2) \in Mo(S)$, suy ra $\lambda(w_1) \in Mo(S)$ và $\lambda(w_2) \in Mo(S)$, do đó $w_1 \in M(S)$ và $w_2 \in M(S)$ theo giả thiết quy nạp và cuối cùng $w \in M(S)$.

Cũng vậy
$$
Mo(S) = v^{-1}(N^{(S)}).
$$
Điều này suy ra ngay lập tức từ công thức (21).

Hơn nữa, $N^{(S)}$ là tập hợp các phần tử của $N^{(X)}$ có giá đỡ được chứa trong $S$; nếu $(S_i)_{i \in I}$ là một họ các tập con của $X$ có giao là $S$, thì $N^{(S)} = \bigcap_{i \in I} N^{(S_i)}$ và các công thức (23) và (24) suy ra
$$
M(S) = \bigcap_{i \in I} M(S_i), \quad Mo(S) = \bigcap_{i \in I} Mo(S_i).
$$

### Bài tập {#alg-i-s7-exercises}

Xem [các bài tập cho § 7](exercises/s7/).
