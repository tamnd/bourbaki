---
book: int
book_title: Integration
chapter: IX
chapter_title: MEASURES ON HAUSDORFF TOPOLOGICAL SPACES
section: 0
section_title: Complements on Hilbert spaces
appendix: true
lang: vi
source: int-vii-ix
book_pages: INT IX.118-INT IX.119
pdf_pages: 0284-0288, 0300-0301
extraction: ocr
subsections:
    - "no": 1
      title: Trace of a quadratic form with respect to another$^{(1)}$
      page: 0
      pdf_page: 284
    - "no": 2
      title: Hilbert–Schmidt mappings$^{(2)}$
      page: 104
      pdf_page: 286
statements: 5
exercises: 9
content_sha256: 79d346d07e4b44beac09b854f0dd0cec6f0f697832af931483086d08ec6bc392
translated_from: content/en/int/IX/A_a_complements_on_hilbert_spaces.md
source_content_sha256: aa78d7417dc812e3fe49b768fcc72481a0fc960e63e09218c2f7ad67767169c0
translation_model: gpt-5.4, gpt-5-6
translation_run: translate-vi-df96e5cb
glossary_version: 34
glossary_terms_sha256: fd3b0fc18b155bc9032ed1d0ddf3f16ffdba57f9a5764d0139240ea313392faf
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## PHỤ LỤC

# Bổ sung về các không gian Hilbert

### 1. Vết của một dạng toàn phương đối với một dạng khác$^{(1)}$

Trong No. này, ta ký hiệu bởi $E$ một không gian vectơ thực và bởi $Q, H$ hai dạng toàn phương dương trên $E$. Tồn tại hai dạng song tuyến tính đối xứng $(x, y) \mapsto (x|y)_Q$ và $(x, y) \mapsto (x|y)_H$ được đặc trưng bởi
$$
Q(x) = (x|x)_Q , \quad H(x) = (x|x)_H
$$
với mọi $x \in E$.

Ta gọi là *vết của Q đối với H* và ký hiệu bởi $\operatorname{Tr}(Q/H)$ số thực dương, hữu hạn hoặc không, được xác định như sau:

a) Nếu tồn tại một $x \in E$ sao cho $H(x) = 0$ và $Q(x) \neq 0$, ta đặt $\operatorname{Tr}(Q/H) = +\infty$.

b) Trong trường hợp ngược lại, $\operatorname{Tr}(Q/H)$ là cận trên đúng của tập hợp các số có dạng $\sum_{i=1}^p Q(e_i)$, trong đó $(e_1, \ldots, e_p)$ chạy qua tập hợp các dãy hữu hạn các phần tử của $E$ trực chuẩn đối với $H$.

Cho $E$ là một không gian Hilbert thực và $Q$ là một dạng toàn phương dương trên $E$. Đặt $H(x) = \|x\|^2$ với mọi $x \in E$; khi đó $H$ là một dạng toàn phương dương trên $E$. Người ta nói rằng $Q$ là *hạt nhân* nếu $\operatorname{Tr}(Q/H)$ là hữu hạn. Với mọi $x \in E$ có chuẩn bằng 1, ta có $Q(x) \leq \operatorname{Tr}(Q/H)$, do đó $Q \leq \operatorname{Tr}(Q/H) \cdot H$; đặc biệt, mọi dạng hạt nhân $Q$ đều liên tục.

#### Nhận xét {#int-ix-a0-n1-rem-1 .statement}

— 1) Với mọi không gian con $F$ của $E$, ký hiệu $Q_F$ là hạn chế của $Q$ trên $F$, và $H_F$ là hạn chế của $H$. Khi đó $\operatorname{Tr}(Q_F/H_F) \leq \operatorname{Tr}(Q/H)$ và $\operatorname{Tr}(Q/H)$ là cận trên đúng của các số $\operatorname{Tr}(Q_F/H_F)$ với $F \subset E$ hữu hạn chiều.

2) Cho $E_1$ là một không gian vectơ thực, $Q_1$ và $H_1$ là hai dạng toàn phương dương trên $E_1$, và $\pi : E \to E_1$ là một ánh xạ tuyến tính toàn ánh. Nếu $Q = Q_1 \circ \pi$ và $H = H_1 \circ \pi$, thì chứng minh rằng $\operatorname{Tr}(Q/H) = \operatorname{Tr}(Q_1/H_1)$.

(1) Xem TVS, V, §4, No. 9.

#### Mệnh đề 1 {#int-ix-a0-prop-1 .statement}

— *Giả sử rằng E hữu hạn chiều và H không suy biến.*

a) *Tồn tại một tự đồng cấu u của E được đặc trưng bởi* $(x|y)_Q = (u(x)|y)_H$ *với x, y thuộc E*.

b) $\operatorname{Tr}(Q/H) = \operatorname{Tr}(u)$.

c) $\operatorname{Tr}(Q/H) = \sum_{i=1}^m Q(e_i)$ *đối với mọi cơ sở* $(e_1, \ldots, e_m)$ *của E trực chuẩn đối với H*.

*a)* suy ra từ việc dạng song tuyến tính $(x, y) \mapsto (x|y)_H$ là không suy biến. Mọi dãy trong E trực chuẩn đối với H đều có thể được bổ sung thành một cơ sở của E trực chuẩn đối với H. Do đó, $\operatorname{Tr}(Q/H)$ là cận trên đúng của tập hợp các số có dạng $\sum_{i=1}^m Q(e_i)$ khi $(e_1, \ldots, e_m)$ chạy qua mọi cơ sở của E trực chuẩn đối với H. Để chứng minh *b)* và *c)*, chỉ cần chỉ ra rằng $\sum_{i=1}^m Q(e_i) = \operatorname{Tr}(u)$ đối với mọi cơ sở như thế. Đặt $a_{ij} = (u(e_i)|e_j)_H = (e_i|e_j)_Q$ với $1 \leq i, j \leq m$; khi đó $u(e_i) = \sum_{j=1}^m a_{ij} e_j$ với $1 \leq i \leq m$, do đó

$$
\operatorname{Tr}(u) = \sum_{i=1}^m a_{ii} = \sum_{i=1}^m (e_i|e_i)_Q = \sum_{i=1}^m Q(e_i).
$$

Đ.P.C.M.

#### Mệnh đề 2 {#int-ix-a0-prop-2 .statement}

— *Giả sử rằng E là hữu hạn chiều. Tồn tại một cơ sở* $(e_1, \ldots, e_n)$ *của E và một số nguyên m với* $0 \leq m \leq n$ *sao cho*

$$
\operatorname{H}\left( \sum_{i=1}^n t_i e_i \right) = \sum_{i=1}^m t_i^2
$$

*với* $t_1, \ldots, t_n$ *thực. Nếu hơn nữa, quan hệ* $\operatorname{H}(x) = 0$ *kéo theo* $Q(x) = 0$ *đối với* $x \in E$, *thì* $\operatorname{Tr}(Q/H) = \sum_{i=1}^m Q(e_i)$.

Tồn tại một cơ sở $(e'_1, \ldots, e'_n)$ của E trực giao đối với H. Có thể giả sử cơ sở được đánh chỉ số sao cho $\operatorname{H}(e'_i) > 0$ với $1 \leq i \leq m$ và $\operatorname{H}(e'_i) = 0$ với $m < i \leq n$. Khi đó đặt $e_i = e'_i / \operatorname{H}(e'_i)^{1/2}$ với $1 \leq i \leq m$ và $e_i = e'_i$ với $m < i \leq n$; quan hệ (1) được thỏa mãn.

Cho F là không gian con của E sinh bởi $e'_{m+1}, \ldots, e'_n$; đó là tập hợp các $x \in E$ sao cho $\operatorname{H}(x) = 0$. Ký hiệu $\pi$ là ánh xạ chính tắc từ E lên $E_1 = E/F$. Vì Q và H bằng không trên F, tồn tại hai dạng toàn phương dương $Q_1$ và $H_1$ trên $E_1$ sao cho $Q = Q_1 \circ \pi$ và $H = H_1 \circ \pi$. Hơn nữa, $(\pi(e_1), \ldots, \pi(e_m))$ là một cơ sở của $E_1$ trực chuẩn đối với $H_1$, và do đó $H_1$ là không suy biến.

Theo Mệnh đề 1 và *Nhận xét 2*,

$$
\operatorname{Tr}(Q/H) = \operatorname{Tr}(Q_1/H_1) = \sum_{i=1}^m Q_1(\pi(e_i)) = \sum_{i=1}^m Q(e_i).
$$

Phải chứng minh điều đó.

#### Nhận xét 3 {#int-ix-a0-n1-rem-3 .statement}

— Giả sử E hữu hạn chiều và H không suy biến. Cho $(e_1, \ldots, e_n)$ là một cơ sở của E. Đặt $q = ((e_i|e_j)_Q)_{1 \leq i,j \leq n}$ và $h = ((e_i|e_j)_H)_{1 \leq i,j \leq n}$. Với các ký hiệu như trong Mệnh đề 1, ma trận của $u$ đối với cơ sở $(e_1, \ldots, e_n)$ của E bằng $h^{-1}q$, do đó

(2)
$$
\operatorname{Tr}(Q/H) = \operatorname{Tr}(h^{-1}q) = \operatorname{Tr}(qh^{-1}).
$$

### 2. Ánh xạ Hilbert–Schmidt$^{(2)}$

Cho E là một không gian Hilbert thực, trong đó tích vô hướng được ký hiệu bởi $(x|y)$. Tồn tại một đẳng cự $j_E$ của E lên đối ngẫu của nó, được đặc trưng bởi công thức

(3)
$$
(x|y) = \langle x, j_E(y) \rangle \quad \text{với } x, y \text{ trong E}
$$
(TVS, V, §1, No. 7, Định lý 3).

Cho $E_1$ và $E_2$ là hai không gian Hilbert thực và $u$ là một ánh xạ tuyến tính liên tục từ $E_1$ vào $E_2$. Người ta gọi *liên hợp của u* là ánh xạ tuyến tính liên tục $u^* = j_{E_1}^{-1} \circ {}^t u \circ j_{E_2}$ từ $E_2$ vào $E_1$. Ánh xạ $u^*$ được đặc trưng bởi quan hệ

(4)
$$
(u(x_1)|x_2) = (x_1|u^*(x_2)) \quad \text{với } x_1 \in E_1,\ x_2 \in E_2.
$$

Nếu $v$ là một ánh xạ tuyến tính liên tục từ $E_2$ vào một không gian Hilbert $E_3$, thì ta có $(v \circ u)^* = u^* \circ v^*$.

Cho $E_1$ và $E_2$ là hai không gian Hilbert thực và $u$ là một ánh xạ tuyến tính từ $E_1$ vào $E_2$. Người ta định nghĩa hai dạng toàn phương dương H và Q trên $E_1$ bởi các công thức

$$
H(x) = \|x\|^2,\quad Q(x) = \|u(x)\|^2 \quad (x \in E_1).
$$

#### Mệnh đề 3 {#int-ix-a0-prop-3 .statement}

*Giả sử u liên tục. Cho $(e_i)_{i \in I}$ là một cơ sở trực chuẩn của $E_1$ và $(f_j)_{j \in J}$ là một cơ sở trực chuẩn của $E_2$. Khi đó*

$$
\operatorname{Tr}(Q|H) = \sum_{i \in I} \|u(e_i)\|^2 = \sum_{j \in J} \|u^*(f_j)\|^2 = \sum_{i \in I} \sum_{j \in J} (u(e_i)|f_j)^2.
$$

(2) Xem TVS, V, §4, No. 7.

Với mọi $x \in E_1$, ta có $\|x\|^2 = \sum_{i \in I} (x|e_i)^2$, và tương tự $\|y\|^2 = \sum_{j \in J} (y|f_j)^2$ với mọi $y \in E_2$. Do đó,

$$
\sum_{i \in I} \|u(e_i)\|^2 = \sum_{i \in I} \sum_{j \in J} (u(e_i)|f_j)^2 \\
= \sum_{j \in J} \sum_{i \in I} (e_i|u^*(f_j))^2 \\
= \sum_{j \in J} \|u^*(f_j)\|^2 .
$$

Đặc biệt, số $\sum_{i \in I} \|u(e_i)\|^2$ độc lập với cơ sở trực chuẩn $(e_i)_{i \in I}$ của $E_1$.

Đặt $t = \operatorname{Tr}(Q|H)$. Với mọi tập con hữu hạn $I'$ của $I$, theo định nghĩa

$$
\sum_{i \in I'} \|u(e_i)\|^2 = \sum_{i \in I'} Q(e_i) \leq t ,
$$

do đó $\sum_{i \in I} \|u(e_i)\|^2 \leq t$. Cho $(e'_1, \ldots, e'_p)$ là một dãy trực chuẩn hữu hạn trong $E$. Dãy này có thể được bổ sung thành một cơ sở trực chuẩn $(e'_\alpha)_{\alpha \in A}$ của $E_1$. Khi đó

$$
\sum_{\alpha=1}^p \|u(e'_\alpha)\|^2 \leq \sum_{\alpha \in A} \|u(e'_\alpha)\|^2 = \sum_{i \in I} \|u(e_i)\|^2
$$

và, chuyển qua cận trên đúng trên mọi $(e'_1, \ldots, e'_p)$, ta thu được bất đẳng thức $t \leq \sum_{i \in I} \|u(e_i)\|^2$. Như vậy ta đã thiết lập được đẳng thức $t = \sum_{i \in I} \|u(e_i)\|^2$.

Điều phải chứng minh.

Người ta nói rằng $u$ là một *ánh xạ Hilbert–Schmidt* từ $E_1$ vào $E_2$ nếu dạng toàn phương dương $Q : x \mapsto \|u(x)\|^2$ trên $E_1$ là hạch. Khi điều đó đúng, ta có $Q \leq \operatorname{Tr}(Q/H) \cdot H$, do đó $u$ liên tục và

$$
\|u\| \leq \operatorname{Tr}(Q/H)^{1/2} .
$$

Cho $u : E_1 \to E_2$ là một ánh xạ tuyến tính liên tục. Theo Mệnh đề 3, $u$ là một ánh xạ Hilbert–Schmidt khi và chỉ khi tồn tại một cơ sở trực chuẩn $(e_i)_{i \in I}$ của $E_1$ sao cho $\sum_{i \in I} \|u(e_i)\|^2 < +\infty$. Khi điều này đúng, mọi cơ sở trực chuẩn của $E_1$ đều có cùng tính chất đó. Hơn nữa, nếu $u$ là một ánh xạ Hilbert–Schmidt, thì liên hợp $u^*$ của nó cũng vậy nhờ công thức $\sum_{i \in I} \|u(e_i)\|^2 = \sum_{j \in J} \|u^*(f_j)\|^2$ (Mệnh đề 3).

Bài tập

### Bài tập {#int-ix-a0-exercises}

Xem [các bài tập cho phụ lục 0](exercises/a0/).
