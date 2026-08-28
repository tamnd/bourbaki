---
book: top
book_title: General Topology
chapter: VII
chapter_title: The additive groups $\mathbf{R}^n$
section: 1
section_title: Subgroups and quotient groups of $\mathbf{R}^n$
lang: vi
source: top-v-x
pdf_pages: 0073-0084, 0093-0099
extraction: ocr
subsections:
    - "no": 1
      title: DISCRETE SUBGROUPS OF $\mathbf{R}^n$
      page: 0
      pdf_page: 74
    - "no": 2
      title: CLOSED SUBGROUPS OF $\mathbf{R}^n$
      page: 0
      pdf_page: 77
    - "no": 3
      title: ASSOCIATED SUBGROUPS
      page: 0
      pdf_page: 79
    - "no": 4
      title: HAUSDORFF QUOTIENT GROUPS OF $\mathbf{R}^n$
      page: 0
      pdf_page: 82
    - "no": 5
      title: SUBGROUPS AND QUOTIENT GROUPS OF $T^n$
      page: 0
      pdf_page: 83
    - "no": 6
      title: PERIODIC FUNCTIONS
      page: 0
      pdf_page: 84
statements: 19
exercises: 15
content_sha256: 2943f4e2c59b72d7dd7452b28ad8dcd58672c26264e99271ee1bae0d5ad50ed8
translated_from: content/en/top/VII/01_s1_subgroups_and_quotient_groups_of_mathbf.md
source_content_sha256: 3722fa7cbaf1b9d82abf2e8703d36456761eeefc481d2d26de9e167e71488cc2
translation_model: gpt-5.4-mini, gpt-5-6-mini
translation_run: translate-vi-2f74ccab
glossary_version: 34
glossary_terms_sha256: 0ca6f0e1a496e332979ec7f2438c5f715ee49345bad8890d67d16a73ee3d2d2a
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 1. NHÓM CON VÀ NHÓM THƯƠNG CỦA $\mathbf{R}^n$

Trước hết ta hãy đưa ra quy ước sau đây: nếu G là một nhóm tôpô, ta đã định nghĩa (chương III, § 2) nhóm tích $G^n$ gồm n thừa số đều bằng G, với mỗi số nguyên $n > 0$. Trong tiết diện này, ta sẽ mở rộng định nghĩa này sang trường hợp $n = 0$ theo quy ước rằng $G^0$ ký hiệu một nhóm chỉ gồm một phần tử. Nếu H là bất kỳ nhóm nào, ta sẽ đồng nhất $G^0 \times H$ với H.

Trên tập $\mathbf{R}^n$, ta sẽ phải xét, một mặt, cấu trúc nhóm tôpô (cộng tính) của nó và, mặt khác, cấu trúc không gian vectơ của nó trên trường $\mathbf{R}$ (chương VI, § 1, no. 3). Cho một tập con A của $\mathbf{R}^n$, ta có thể xét nhóm con của $\mathbf{R}^n$ sinh bởi A (tập tất cả các tổ hợp tuyến tính của các điểm của A, với hệ số nguyên) và cũng không gian con vectơ sinh bởi A (tập tất cả các tổ hợp tuyến tính của các điểm của A, với hệ số thực); hai khái niệm này phải được phân biệt cẩn thận. Phù hợp với các định nghĩa trong đại số, hạng của A là chiều của không gian con vectơ V của $\mathbf{R}^n$ sinh bởi A; nói rằng A có hạng $p$ vì thế tương đương với nói rằng có $p$ điểm $x_i \in A$ lập thành một hệ tự do đối với trường $\mathbf{R}$ (nói cách khác, quan hệ $\sum_i t_i x_i = 0$, trong đó các $t_i$ là các số thực, suy ra $t_i = 0$ với mỗi $i$) và lập thành một cơ sở của V (nghĩa là mọi điểm của V đều là một tổ hợp tuyến tính của các $x_i$ với hệ số thực).

Trong phần tiếp theo ta cũng sẽ phải dùng đến khái niệm một hệ các điểm của $\mathbf{R}^n$ tự do đối với trường $\mathbf{Q}$ của các số hữu tỉ; một hệ như vậy là một tập con hữu hạn $(x_i)$ của $\mathbf{R}^n$ sao cho quan hệ $\sum_i r_i x_i = 0$, trong đó các $r_i$ là các số hữu tỉ (hay các số nguyên — cũng như nhau), suy ra $r_i = 0$ với mỗi $i$. Khái niệm này phải được phân biệt cẩn thận với khái niệm hệ tự do đối với $\mathbf{R}$: mọi hệ tự do đối với $\mathbf{R}$ đều tự do đối với $\mathbf{Q}$, nhưng điều đảo lại là sai (ví dụ, các số 1 và $\sqrt{2}$ trong $\mathbf{R}$ lập thành một hệ tự do đối với $\mathbf{Q}$, nhưng không phải là một hệ tự do đối với $\mathbf{R}$). Mỗi khi nói đến một *hệ tự do* không nói rõ thêm, ta luôn hiểu là một hệ tự do *đối với* $\mathbf{R}$. Vì thế cần phân biệt trên $\mathbf{R}^n$ cấu trúc không gian vectơ *đối với* $\mathbf{R}$ với cấu trúc không gian vectơ *đối với* $\mathbf{Q}$; đặc biệt, không gian con vectơ *đối với* $\mathbf{Q}$ sinh bởi một tập con A của $\mathbf{R}^n$ là tập U gồm mọi tổ hợp tuyến tính của A với *hệ số hữu tỉ*; nó được chứa trong không gian con vectơ V (đối với $\mathbf{R}$) sinh bởi A, nhưng nói chung khác với V. Chiều của U (*đối với* $\mathbf{Q}$) được gọi là *hạng hữu tỉ* của A; nó *ít nhất bằng* *hạng* của A đã định nghĩa ở trên (chiều của V đối với $\mathbf{R}$); nó có thể *vô hạn* nếu A là một tập vô hạn, trong khi hạng của mọi tập con không rỗng của $\mathbf{R}^n$ luôn $\leq n$; đặc biệt, hạng hữu tỉ của mọi tập con *không đếm được* của $\mathbf{R}^n$ luôn vô hạn, vì mọi không gian vectơ hữu hạn chiều trên $\mathbf{Q}$ đều đếm được.

Trong tiết diện này ta sẽ trước hết xác định cấu trúc của các *nhóm con đóng* của nhóm cộng $\mathbf{R}^n$.

### 1. NHÓM CON RỜI RẠC CỦA $\mathbf{R}^n$

Ta đã thấy trong Chương V (\S 1, no. 1, Mệnh đề 1) rằng các nhóm con đóng duy nhất của $\mathbf{R}$, khác với chính $\mathbf{R}$, là các nhóm con *rời rạc*, được sinh bởi một *phần tử* duy nhất. Ta sẽ bắt đầu bằng việc xét các nhóm con *rời rạc* của $\mathbf{R}^n$.

Trước hết, nhóm con của $\mathbf{R}^n$ được sinh bởi $p$ vectơ ($p \leq n$) của cơ sở chính tắc (Chương VI, \S 1, no. 3) của $\mathbf{R}^n$ là một nhóm rời rạc đẳng cấu với tích $\mathbf{Z}^p$ của $p$ nhóm bằng $\mathbf{Z}$. Nói chung, xét nhóm con $G$ được sinh bởi $p$ điểm $a_i$ ($1 \leq i \leq p$) tạo thành một hệ tự do. Có một ánh xạ tuyến tính song ánh của $\mathbf{R}^n$ lên chính nó biến $a_i$ thành $e_i$ ($1 \leq i \leq p$); vì ánh xạ như vậy là một tự đẳng cấu của nhóm tôpô $\mathbf{R}^n$, $G$ đẳng cấu với tư cách là một nhóm tôpô với nhóm con được sinh bởi các $e_i$ ($1 \leq i \leq p$) và do đó là một nhóm con *rời rạc* hạng $p$ đẳng cấu với $\mathbf{Z}^p$.

Cấu trúc của nhóm $\mathbf{Z}^p$, và do đó của $G$, đã được nghiên cứu trong đại số. Ta nhắc lại các kết quả chính của nghiên cứu này. Các *cơ sở* của $G$ đối với vành $\mathbf{Z}$ là các hệ gồm $p$ điểm

$$
b_i = \sum_{j=1}^p r_{ij} a_j,
$$

trong đó các $r_{ij}$ là các số nguyên sao cho định thức $\det (r_{ij})$ bằng $+1$ hoặc $-1$. Mọi *nhóm con* $H$ của $G$ đều rời rạc và có hạng $q \leq p$; hơn nữa, nếu $H$ là một nhóm con đã cho có hạng $q$, thì tồn tại một hệ tự do gồm $p$ điểm $b_i$ ($1 \leq i \leq p$) sinh ra $G$, và một hệ gồm $q$ điểm $c_i$ ($1 \leq i \leq q$) sinh ra $H$, sao cho ta có $c_i = e_i b_i$ cho $1 \leq i \leq q$, trong đó các $e_i$ là các số nguyên (các thừa số bất biến của $H$ đối với $G$) sao cho
$$
e_{i+1} \equiv 0 \pmod{e_i} \quad \text{cho} \quad 1 \leq i \leq q - 1.
$$
Nhóm thương $G/H$ là một nhóm rời rạc đẳng cấu với $\mathbf{Z}^{p-q} \times F$, trong đó $F$ là một nhóm Abel hữu hạn, là tích trực tiếp của $q$ nhóm con chu kỳ có các cấp tương ứng $e_1, \ldots, e_q$.

Bây giờ ta sẽ chỉ ra rằng các nhóm con rời rạc của $\mathbf{R}^n$ mà ta vừa xét là những nhóm duy nhất tồn tại.

#### Mệnh đề 1 {#top-vii-s1-prop-1 .statement}

*Cho $G$ là một nhóm con rời rạc của $\mathbf{R}^n$ có hạng $p$, cho $(a_i)_{1 \leq i \leq p}$ là một hệ tự do gồm $p$ điểm của $G$, và cho $P$ là hình bình hành đóng với tâm $o$ và các vectơ cơ sở $a_i$ (Chương VI, § 1, no. 3). Khi đó tập hợp $G \cap P$ là hữu hạn và sinh ra $G$, và mọi điểm của $G$ là một tổ hợp tuyến tính của các $a_i$ với các hệ số hữu tỉ.*

$G \cap P$ là compact và rời rạc, do đó *hữu hạn*. Cho $x$ là một điểm bất kỳ của $G$; nó bằng một tổ hợp tuyến tính $\sum_{i=1}^p t_i a_i$ của các $a_i$ với các hệ số thực. Với mỗi số nguyên $m > 0$, xét điểm
$$
z_m = mx - \sum_{i=1}^p [mt_i] a_i = \sum_{i=1}^p (mt_i - [mt_i]) a_i \ (*) ;
$$
nó thuộc $G$, và vì $0 \leq mt_i - [mt_i] < 1$, nó nằm trong $P$. Do đó, thứ nhất, $x = z_1 + \sum_{i=1}^p [t_i] a_i$, suy ra $G$ được sinh bởi $G \cap P$; và thứ hai, vì $G \cap P$ là hữu hạn, tồn tại hai số nguyên phân biệt $h, k$ sao cho $z_h = z_k$, do đó $(h - k)t_i = [ht_i] - [kt_i]$ less ($1 \leq i \leq p$), và vì vậy các $t_i$ là các số hữu tỉ.

#### Hệ quả {#top-vii-s1-n1-cor-1 .statement}

*Cho $(a_i)_{1 \leq i \leq p}$ là một hệ tự do gồm $p$ điểm của $\mathbf{R}^n$ và cho*
$$
b = \sum_{i=1}^p t_i a_i
$$
*là một tổ hợp tuyến tính của các $a_i$, với các hệ số thực. Khi đó nhóm con $G$ của $\mathbf{R}^n$ sinh bởi $p + 1$ điểm $a_1, a_2, \ldots, a_p$ và $b$ là rời rạc khi và chỉ khi các số $t_i$ là hữu tỉ.*

(*) Ta nhắc lại (Chương IV, § 8, no. 2) rằng, với mỗi số thực $x, [x]$ là phần nguyên của $x$, nghĩa là số nguyên hữu tỉ lớn nhất $\leq x$.

Mệnh đề 1 chỉ ra rằng điều kiện là cần thiết. Nó cũng đủ, vì nếu điều kiện đó được thỏa mãn ta có thể viết $t_i = m_i/d$, trong đó $d$ và các $m_i$ là các số nguyên ($1 \leq i \leq p$); do đó $b$ là một tổ hợp tuyến tính, với các hệ số nguyên, của $p$ điểm $(1/d)a_i$; vì vậy $G$ là một nhóm con của nhóm rời rạc được sinh bởi $p$ điểm này, và do đó chính nó cũng rời rạc.

Kết quả của Mệnh đề 1 có thể được phát biểu như sau: nếu $q$ điểm $x_i$ ($1 \leq i \leq q$) của một nhóm con *rời rạc* $G$ của $\mathbf{R}^n$ tạo thành một hệ *phụ thuộc tuyến tính đối với* $\mathbf{R}$, thì chúng tạo thành một hệ *phụ thuộc tuyến tính đối với* $\mathbf{Q}$. Suy ra ngay rằng *hạng hữu tỉ* của một nhóm con rời rạc của $\mathbf{R}^n$ bằng *hạng* của nó.

Hệ quả của Mệnh đề 1, khi áp dụng cho trường hợp các $a_i$ là $n$ vectơ $e_i$ của cơ sở chính tắc của $\mathbf{R}^n$, cho ta mệnh đề sau:

**Mệnh đề 2 (Kronecker).** *Cho $\theta_1, \theta_2, \ldots, \theta_n$ là $n$ số thực. Để với mỗi $\varepsilon > 0$, tồn tại một số nguyên $q$ và $n$ số nguyên*
$$
p_i \quad (1 \leq i \leq n)
$$
*sao cho*
$$
|q\theta_i - p_i| \leq \varepsilon \quad (1 \leq i \leq n),
$$
*với vế trái của ít nhất một trong các bất đẳng thức này không bằng 0, thì điều kiện cần và đủ là ít nhất một trong các $\theta_i$ là vô tỉ.*

#### Định lý 1 {#top-vii-s1-thm-1 .statement}

*Mọi nhóm con rời rạc $G$ của $\mathbf{R}^n$, có hạng bằng $p$, đều được sinh bởi một hệ tự do gồm $p$ điểm.*

Nhờ các tính chất của những nhóm đẳng cấu với $\mathbf{Z}^p$ đã nhắc lại ở trên, chỉ cần chứng minh rằng $G$ là một *nhóm con* của một nhóm rời rạc được sinh bởi một hệ tự do gồm $p$ điểm. Nay vì $G$ có hạng $p$ nên tồn tại một hệ tự do gồm $p$ điểm $a_i$ ($1 \leq i \leq p$) của $G$ sao cho mọi $x \in G$ đều bằng một tổ hợp tuyến tính $\sum_{i=1}^p t_i a_i$ của các $a_i$ với hệ số thực; vì $G$ rời rạc, Mệnh đề 1 cho thấy các $t_i$ là *hữu tỉ*. Hơn nữa, Mệnh đề 1 cho thấy $G$ được sinh bởi một *số hữu hạn* các điểm; vì các điểm này là những tổ hợp tuyến tính của các $a_i$ với hệ số hữu tỉ, tồn tại một số nguyên $d$ sao cho chúng là những tổ hợp tuyến tính với *số nguyên* của $p$ điểm $(1/d)a_i = a'_i$. Suy ra $G$ là một nhóm con của nhóm được sinh bởi các $a'_i$.

Định lý 1 cũng có thể được chứng minh mà không cần viện đến lý thuyết các nhân tử bất biến (xem Bài tập 1).

Các nhóm con rời rạc của $\mathbf{R}^n$ có hạng $n$ còn được gọi là *mạng* trong $\mathbf{R}^n$.

### 2. CÁC NHÓM CON ĐÓNG CỦA $\mathbf{R}^n$

Ta đã biết hai loại nhóm con đóng của $\mathbf{R}^n$; một mặt, các *không gian con vectơ* của $\mathbf{R}^n$, đẳng cấu với các nhóm $\mathbf{R}^p$ ($p \leq n$) (Chương IV, § 1, no. 4, Mệnh đề 2); mặt khác, các nhóm con *rời rạc* (Chương III, § 2, no. 1, Mệnh đề 5), vốn đẳng cấu với các nhóm $\mathbf{Z}^q$ ($q \leq n$), như ta vừa thấy. Bây giờ ta sẽ xác định cấu trúc của một nhóm con đóng *tùy ý* của $\mathbf{R}^n$ bằng cách chứng minh rằng một nhóm con như vậy đẳng cấu với một *tích* có dạng

$$
\mathbf{R}^p \times \mathbf{Z}^q \quad \text{trong đó} \quad 0 \leq p + q \leq n.
$$

Chứng minh dựa trên mệnh đề sau:

#### Mệnh đề 3 {#top-vii-s1-prop-3 .statement}

*Mọi nhóm con đóng không rời rạc của* $\mathbf{R}^n$ *đều chứa một đường thẳng đi qua* $o$.

#### Định lý 2 {#top-vii-s1-thm-2 .statement}

Cho $(x_p)_{p \in \mathbf{N}}$ là một dãy vô hạn các điểm của $G$ sao cho $x_p \neq o$ và $\lim_{p \to \infty} x_p = o$; theo giả thiết, tồn tại một dãy như vậy. Cho $P$ là một khối lập phương mở có tâm $o$, chứa các $x_p$. Ký hiệu $k_p$ là số nguyên lớn nhất $h > 0$ sao cho $hx_p \in P$ (vì $P$ là một hộp bị chặn và $x_p \neq o$, sự tồn tại của $k_p$ suy ra từ tiên đề Archimedes). Các điểm $k_p x_p$ nằm trong một tập compact $\overline{P}$, do đó dãy $(k_p x_p)_{p \in \mathbf{N}}$ có một điểm tụ $a \in \overline{P}$. Nếu $\| (k_p + 1)x_p - a \| \leq \varepsilon$, ta có

$$
\| (k_p + 1)x_p - a \| \leq \varepsilon + \| x_p \|,
$$

và vì $\lim_{p \to \infty} x_p = o$, suy ra rằng $a$ cũng là một điểm tụ của dãy $((k_p + 1)x_p)$, mà các điểm của dãy này thuộc tập đóng $\mathbf{C}P$, theo định nghĩa của $k_p$; do đó $a \in \overline{P} \cap \mathbf{C}P$ (biên của $P$, Hình 5), suy ra $a \neq o$. Hơn nữa, vì $G$ là tập đóng, ta có $a \in G$. Cho $t$ là một số thực tùy ý; vì $|tk_p - [tk_p]| < 1$, quan hệ $\| k_p x_p - a \| \leq \varepsilon$ suy ra rằng $\| [tk_p]x_p - ta \| \leq |t| \varepsilon + \| x_p \|$; vì $\lim_{p \to \infty} x_p = o$, $ta$ là một điểm tụ của dãy ([tk_p]x_p); nhưng các điểm của dãy này thuộc $G$, và do đó ta ∈ G, vì $G$ đóng. Điều này kết thúc chứng minh.

![Hình 5](https://i.imgur.com/5z5z5z5.png)
Hình 5.

![Hình 6](https://i.imgur.com/6z6z6z6.png)
Hình 6.

Cho $G$ là một nhóm con đóng của $\mathbf{R}^n$, có hạng $r$ ($0 \leq r \leq n$). Khi đó tồn tại một không gian con vectơ lớn nhất $V$ được chứa trong $G$; với mọi không gian con vectơ $W$ bổ sung cho $V$, $W \cap G$ là rời rạc và $G$ là tổng trực tiếp của $V$ và $W \cap G$.

Trước hết ta chứng minh sự tồn tại của $V$ bằng cách chỉ ra rằng hợp của mọi đường thẳng đi qua $o$ và nằm trong $G$ là một không gian con vectơ: thật vậy, không gian con vectơ sinh bởi hợp các đường thẳng này cũng chính là nhóm con do chúng sinh ra. Nhóm $G$ là tổng trực tiếp của $V$ và $W \cap G$; vì nếu $x \in G$, ta có $x = y + z$ với $y \in V$ và $z \in W$; do $V \subset G$, $z = x - y \in G$ và do đó $z \in W \cap G$. Còn lại phải chứng minh rằng $W \cap G$ là rời rạc; điều này suy ra từ Mệnh đề 3, vì $W \cap G$ là một nhóm con đóng không chứa đường thẳng nào, theo định nghĩa của $V$.

Nếu $G \neq V$, ta có thể nói rằng $G$ là hợp của một vô hạn đếm được các đa tạp tuyến tính, song song với $V$ và đi qua các điểm của nhóm rời rạc $W \cap G$ (Hình 6).

Nếu $p$ là chiều của không gian con vectơ $V$, ta có $p \leq r$, và $W \cap G$ là một nhóm rời rạc có hạng $r - p$.

#### Hệ quả 1 {#top-vii-s1-thm-2-cor-1 .statement}

Có một cơ sở $(a_i)_{1 \leq i \leq n}$ của $\mathbf{R}^n$, sao cho
$$
a_i \in G \quad (1 \leq i \leq r), \qquad a_i \in V \quad (1 \leq i \leq p)
$$
và sao cho G là tập hợp các điểm $\sum_{i=1}^p t_i a_i + \sum_{j=p+1}^r n_j a_j$, trong đó các $t_i$ nhận mọi giá trị thực và các $n_j$ nhận mọi giá trị nguyên.

Điều này suy ra từ Định lý 2, và Định lý 1 của mục 1 được áp dụng cho nhóm rời rạc $W \cap G$.

#### Hệ quả 2 {#top-vii-s1-thm-2-cor-2 .statement}

Có một tự đẳng cấu của $\mathbf{R}^n$ ánh xạ G lên nhóm $G'$, đẳng cấu với $\mathbf{R}^p \times \mathbf{Z}^{r-p}$, là tổng trực tiếp của không gian con vectơ sinh bởi $e_1, e_2, \ldots, e_p$ và nhóm con cộng tính (rời rạc) sinh bởi $e_{p+1}, e_{p+2}, \ldots, e_r$.

Đây là một hệ quả ngay lập tức của Hệ quả 1. Hệ quả 2 của Định lý 2 cho thấy rằng một nhóm con đóng G của $\mathbf{R}^n$ được xác định hoàn toàn, tới đẳng cấu, bởi hai số nguyên $\geq 0$: hạng của nó, mà ta ký hiệu là $r(G)$, và chiều của không gian con vectơ lớn nhất được chứa trong G, mà ta gọi là chiều của G và ký hiệu là $d(G)$.

Các điều kiện duy nhất mà những số nguyên này phải thỏa mãn là các bất đẳng thức $0 \leq d(G) \leq r(G) \leq n$.

### 3. NHÓM CON LIÊN KẾT

Cho G là một nhóm con tùy ý (đóng hoặc không) của $\mathbf{R}^n$. Xét tập $G^*$ các điểm $u = (u_i) \in \mathbf{R}^n$ sao cho, với mọi $x = (x_i) \in G$, số $(u|x) = \sum_{i=1}^n u_i x_i$ là một số nguyên. Ta thấy ngay rằng $G^*$ là một nhóm con của $\mathbf{R}^n$; nó được gọi là nhóm con liên kết với G (*). Nếu G và H là hai nhóm con của $\mathbf{R}^n$ sao cho $H \subset G$, thì hiển nhiên $G^* \subset H^*$.

#### Mệnh đề 4 {#top-vii-s1-prop-4 .statement}

*Nhóm con $G^*$ liên kết với một nhóm con G của $\mathbf{R}^n$ là đóng, và ta có $(\overline{G})^* = G^*.$*

Với mỗi $x \in G$, ký hiệu $f_x(u)$ là $(u|x)$; $f_x$ là một dạng tuyến tính, do đó liên tục. Vì $G^*$ là giao của các tập $f_x^{-1}(z)$ khi $x$ chạy qua G, và vì mỗi tập ấy đều đóng, suy ra $G^*$ là đóng. Mặt khác, nếu $u \in G^*$, ta có $(u|x) \in \mathbf{Z}$ với mọi $x \in G$, và do đó, vì $\mathbf{Z}$ là đóng trong $\mathbf{R}$, $(u|y) \in \mathbf{Z}$ với mọi $y \in \overline{G}$; do đó $u \in (G)^*$. Nhưng ta có $(\overline{G})^* \subset G^*$ (vì $G \subset \overline{G}$), nên $(\overline{G})^* = G^*$.

Xét cấu trúc của $G^*$ khi $G$ là *đóng*. Theo Hệ quả 1 của Định lý 2 ở mục 2, tồn tại một cơ sở $(a_i)_{1 \leq i \leq n}$ của $\mathbf{R}^n$ sao cho G trùng với tập hợp các điểm

$$
x = \sum_{i=1}^p t_i a_i + \sum_{j=p+1}^{p+q} n_j a_j,
$$

trong đó các $t_i$ nhận mọi giá trị thực và các $n_j$ nhận mọi giá trị nguyên. Do đó $(u|x)$ là một số nguyên cho *mọi* điểm $x$ này khi và chỉ khi $(u|a_i) = 0$ đối với $1 \leq i \leq p$ và $(u|a_i)$ là một số nguyên đối với $p+1 \leq i \leq p+q$. Ta ký hiệu bởi $(a'_i)_{1 \leq i \leq n}$ cơ sở của $\mathbf{R}^n$ sao cho $(a'_i|a_j) = 0$ đối với $i \neq j$ và

$$
(a'_i|a_i) = 1 \quad \text{cho} \quad 1 \leq i \leq n
$$

(*) Khái niệm này là một trường hợp riêng, tương ứng với nhóm $\mathbf{R}^n$, của một khái niệm tổng quát trong lý thuyết *đối ngẫu* của các nhóm Abel compact địa phương (xem, chẳng hạn, A. Weil, "L'integration dans les groupes topologiques et ses applications", *Act. Sci. et Ind.* no. 869, Paris, Hermann, 1950, pp. 108-109). Người đọc sẽ nhận thấy sự tương tự gần gũi tồn tại giữa các tính chất của các nhóm con liên kết trong $\mathbf{R}^n$ và các tính chất của các không gian con vectơ *trực giao* của một không gian vectơ và không gian đối ngẫu của nó.

[cơ sở "đối ngẫu" với $(\mathbf{a}_i)$]; nếu ta đặt $u = \sum_{i=1}^n u_i a'_i$, thì rõ ràng các điểm $u \in G^*$ được đặc trưng bởi các điều kiện sau: $u_i = 0$ đối với $1 \leq i \leq p$, và $u_i \in \mathbf{Z}$ đối với
$$
p + 1 \leq i \leq p + q;
$$
do đó $G^*$ là tổng trực tiếp của một không gian con vectơ $W$ có một cơ sở gồm các $a'_i$ sao cho $p + q + 1 \leq i \leq n$, và một nhóm con rời rạc sinh bởi các $a'_i$ sao cho $p + 1 \leq i \leq p + q$. Nói cách khác:

#### Mệnh đề 5 {#top-vii-s1-prop-5 .statement}

*Đối với mọi nhóm con đóng* $G$ *của* $\mathbf{R}^n$,
$$
r(G^*) = n - d(G) \quad \text{và} \quad d(G^*) = n - r(G).
$$
Ta áp dụng cùng lập luận cho $G^*$. Nhận thấy rằng cơ sở đối ngẫu với $(a'_i)$ là $(a_i)$, ta thấy rằng:

#### Mệnh đề 6 {#top-vii-s1-prop-6 .statement}

*Đối với mọi nhóm con* $G$ *của* $\mathbf{R}^n$, *ta có* $(G^*)^* = \overline{G}$.

#### Hệ quả {#top-vii-s1-n3-cor-1 .statement}

*Một điểm* $x$ *nằm trong bao đóng của một nhóm con* $G$ *của* $\mathbf{R}^n$ *khi và chỉ khi* $(u|x)$ *là một số nguyên đối với mọi* $u \in \mathbf{R}^n$ *sao cho* $(u|y)$ *là một số nguyên đối với mọi* $y \in G$.

Ta áp dụng đặc trưng hóa này của các điểm nằm trong bao đóng của một nhóm con $G$ vào trường hợp nhóm con $G$ sinh bởi $n$ vectơ $e_j$ của cơ sở chính tắc $(1 \leq j \leq n)$ và bởi một số tùy ý $m$ điểm $a_i$ $(1 \leq i \leq m)$ của $\mathbf{R}^n$. Nói rằng $(u|e_j)$ là một số nguyên đối với $1 \leq j \leq n$ có nghĩa là $n$ tọa độ của $u$ là các số nguyên; do đó:

#### Mệnh đề 7 (Kronecker) {#top-vii-s1-prop-7 .statement}

*Cho* $a_i = (a_{ij})$ $(1 \leq i \leq m,\ 1 \leq j \leq n)$ *là* $m$ *điểm của* $\mathbf{R}^n$ *và cho* $b = (b_j)$ $(1 \leq j \leq n)$ *là một điểm của* $\mathbf{R}^n$. *Để, với mỗi* $\varepsilon > 0$, *tồn tại* $m$ *số nguyên* $g_i$ $(1 \leq i \leq m)$ *và* $n$ *số nguyên* $p_j$ $(1 \leq j \leq n)$ *sao cho*
$$
|q_1 a_{1j} + q_2 a_{2j} + \cdots + q_m a_{mj} - p_j - b_j| \leq \varepsilon \quad (1 \leq j \leq n)
$$
*thì điều kiện cần và đủ là, với mỗi dãy hữu hạn* $(r_j)$ $(1 \leq j \leq n)$ *gồm* $n$ *số nguyên sao cho* $m$ *số* $\sum_{j=1}^n a_{ij} r_j$ $(1 \leq i \leq m)$ *đều là số nguyên, thì số* $\sum_{j=1}^n b_j r_j$ *cũng phải là số nguyên*.

#### Hệ quả 1 {#top-vii-s1-prop-7-cor-1 .statement}

*Để, với mỗi* $x = (x_j)$ $(1 \leq j \leq n)$ *và mỗi* $\varepsilon > 0$, *tồn tại* $m$ *số nguyên* $q_i$ $(1 \leq i \leq m)$ *và* $n$ *số nguyên* $p_j$ ($1 \leq j \leq n$) *sao cho*

$$
|q_1 a_{1j} + q_2 a_{2j} + \cdots + q_m a_{mj} - p_j - x_j| \leq \varepsilon \quad (1 \leq j \leq n)
$$

*thì điều kiện cần và đủ là không tồn tại dãy hữu hạn* $(r_j)$ *gồm* $n$ *số nguyên, không phải tất cả đều bằng không, sao cho mỗi một trong* $m$ *số* $\sum_{j=1}^n a_{ij} r_j$ *là một số nguyên*.

Vì nếu $G$ *là trù mật trong* $\mathbf{R}^n$, *nghĩa là nếu* $\overline{G} = \mathbf{R}^n$, *thì* $G^* = \{0\}$, *và ngược lại*.

Đặc biệt $(m = 1)$:

#### Hệ quả 2 {#top-vii-s1-prop-7-cor-2 .statement}

*Cho* $\theta_1, \theta_2, \ldots, \theta_n$ *là* $n$ *số thực. Để, cho trước bất kỳ* $n$ *số thực* $x_1, x_2, \ldots, x_n$ *và một số thực* $\varepsilon > 0$, *tồn tại một số nguyên* $q$ *và* $n$ *số nguyên* $p_j$ *sao cho*

$$
|q \theta_j - p_j - x_j| \leq \varepsilon \quad (1 \leq j \leq n)
$$

*thì điều kiện cần và đủ là không tồn tại một quan hệ có dạng* $\sum_{j=1}^n r_j \theta_j = h$, *trong đó các* $r_j$ *là* $n$ *số nguyên không phải tất cả đều bằng không, và* $h$ *là một số nguyên* [điều này suy ra, đặc biệt, rằng các $\theta_j$ *và các tỉ số* $\theta_j / \theta_k$ ($j \neq k$) *phải là vô tỉ*].

Ta có thể hiểu kết quả này như sau: với mỗi số nguyên $q \in \mathbf{Z}$, đặt $x_q$ là điểm có tọa độ $q \theta_j - [q \theta_j]$ ($1 \leq j \leq n$); khi đó Hệ quả 2 cho một điều kiện cần và đủ để tập hợp các điểm $x_q$ là *trù mật* trong khối lập phương là tích của $n$ khoảng $[0, 1]$ trong các thừa số của $\mathbf{R}^n$.

#### Mệnh đề 8 {#top-vii-s1-prop-8 .statement}

*Nếu $G_1, G_2$ là hai nhóm con đóng bất kỳ của $\mathbf{R}^n$, ta có*

$$
(G_1 = G_2)^* + G_1^* \cap G_2^* \quad \text{và} \quad (G_1 \cap G_2)^* = G_1^* + G_2^*.
$$

Số thực $(u|x + y)$ là một số nguyên với mọi $x \in G_1$ và mọi $y \in G_2$ khi và chỉ khi $(u|x)$ là một số nguyên với mọi $x \in G_1$ và $(u|y)$ là một số nguyên với mọi $y \in G_2$, vì $(u|x + y) = (u|x) + (u|y)$; do đó

$$
(G_1 + G_2)^* = G_1^* \cap G_2^*
$$

cho mọi hai nhóm con $G_1, G_2$ của $\mathbf{R}^n$. Nếu bây giờ ta giả sử rằng $G_1$ và $G_2$ là đóng, ta có $(G_1^* + G_2^*)^* = G_1 \cap G_2$ theo Mệnh đề 6; do đó, lấy các nhóm con liên kết và áp dụng Mệnh đề 6 một lần nữa,

$$
(G_1 \cap G_2)^* = \overline{G_1^* + G_2^*}.
$$

#### Nhận xét {#top-vii-s1-n3-rem-1 .statement}

Cho $G_1, G_2$ là hai *mạng* trong $\mathbf{R}^n$ (no. 1) sao cho $G_2 \subset G_1$: khi đó (Mệnh đề 5) $G_1^*$ và $G_2^*$ là các *mạng* trong $\mathbf{R}^n$ sao cho $G_1^* \subset G_2^*$. Ta đã thấy ở no. 1 rằng tồn tại một số nguyên $m > 0$ sao cho $m G_1 \subset G_2$;

do đó với $x \in G_1$ và $u \in G_2^*$ ta có $m(u|x) \in \mathbf{Z}$ và vì vậy $(u|x) \in \mathbf{Q}$. Nếu $x \in G_2$ và $u \in G_2^*$, hoặc nếu $x \in G_1$ và $u \in G_1^*$, ta có $(u|x) \in \mathbf{Z}$ theo định nghĩa. Vì thế khi chuyển qua các thương, ánh xạ song tuyến tính trên $\mathbf{Z}$ $(x, u) \to (u|x)$ của $G_1 \times G_2^*$ vào $\mathbf{Q}$ xác định một ánh xạ song tuyến tính trên $\mathbf{Z}$ $B$ của $(G_1/G_2) \times (G_2^*/G_1^*)$ vào $\mathbf{Q}/\mathbf{Z}$. Hơn nữa, hiển nhiên rằng nếu $\bar{x}_0 \in G_1/G_2$ (resp. $\bar{u}_0 \in G_2^*/G_1^*$) sao cho, với *mỗi* $\bar{u} \in G_2^*/G_1^*$ (resp. với mỗi $\bar{x} \in G_1/G_2$) ta có

$$
B(\bar{x}_0, u) = 0 \quad [\text{resp. } B(\bar{x}, \bar{u}_0) = 0],
$$

then suy ra tất yếu $\bar{x}_0 = 0$ (tương ứng $\bar{u}_0 = 0$). Suy ra có một *song ánh* tuyến tính trên $\mathbf{Z}$ $h$ từ $G_2^*/G_1^*$ lên *đối ngẫu* của $G_1/G_2$, sao cho $\langle \bar{x}, h(\bar{u}) \rangle = B(\bar{x}, \bar{u})$ với $\bar{x} \in G_1/G_2$ và $\bar{u} \in G_2^*/G_1^*$; nói riêng, các nhóm hữu hạn $G_1/G_2$ và $G_2^*/G_1^*$ là *đẳng cấu*.

### 4. NHÓM THƯƠNG HAUSDORFF CỦA $\mathbf{R}^n$

Mọi nhóm thương Hausdorff của $\mathbf{R}^n$ đều có dạng $\mathbf{R}^n/H$, trong đó $H$ là một nhóm con đóng của $\mathbf{R}^n$ (Chương III, § 2, no. 6, Mệnh đề 18). Theo Hệ quả 2, Định lý 2 của no. 3, tồn tại một tự đẳng cấu $f$ của $\mathbf{R}^n$ biến $H$ thành một nhóm con $H'$, là tổng trực tiếp của một không gian con vectơ được sinh bởi $p$ trong các vectơ $e_i$ của cơ sở chính tắc và nhóm rời rạc được sinh bởi $g$ của $n - p$ vectơ còn lại

$$
e_i, \quad 0 \leq p + q \leq n.
$$

Chuyển qua các thương, $f$ cảm sinh một đẳng cấu từ $\mathbf{R}^n/H$ lên $\mathbf{R}^{n-p-q} \times T^q$ (Chương III, § 2, no. 8, Nhận xét 3); nay, $\mathbf{R}^n/H'$ đẳng cấu với $\mathbf{R}^{n-p-q} \times T^q$ (Chương III, § 2, no. 9, Hệ quả của Mệnh đề 26). Do đó:

#### Mệnh đề 9 {#top-vii-s1-prop-9 .statement}

*Mọi nhóm thương Hausdorff của* $\mathbf{R}^n$ *đều đẳng cấu với một nhóm tích* $\mathbf{R}^h \times T^k$ ($0 \leq h + k \leq n$).

Không gian tích $T^n$ (và, theo lối nói lạm dụng, nhóm tôpô $T^n$) được gọi là *xuyến n chiều*; theo Mệnh đề 4 của Chương V, § 1, no. 2, $T^n$ là compact, liên thông và liên thông địa phương.

Hơn nữa, nếu $C$ là một khối lập phương đóng cạnh 1 trong $\mathbf{R}^n$, thì $T^n$ đồng phôi với không gian thương của $C$ theo quan hệ tương đương " $x_i \equiv y_i \pmod{1}$ ($1 \leq i \leq n$)" giữa các điểm $x = (x_i)$ và $y = (y_i)$ của $C$. Như vậy $T^n$ được tạo thành từ khối lập phương $C$ bằng "sự đồng nhất các mặt đối diện".

#### Mệnh đề 10 {#top-vii-s1-prop-10 .statement}

*Nhóm tôpô* $T^n$ *là đẳng cấu địa phương với* $R^n$.

Vì $T^n = (R/Z)^n$ đẳng cấu với $R^n/Z^n$ (Chương III, § 2, no. 9, Hệ quả của Mệnh đề 26) và $Z^n$ là một nhóm con rời rạc của $R^n$ (Chương III, § 2, no. 6, Mệnh đề 19).

Suy ra các nhóm $R^p \times T^{n-p}$ đều đẳng cấu địa phương với $R^n$ ($0 \geq p \geq n$); trong § 2, no. 2, ta sẽ thấy rằng chúng là những nhóm *liên thông* duy nhất có tính chất này.

### 5. NHÓM CON VÀ NHÓM THƯƠNG CỦA $T^n$

Ta đồng nhất $T^n$ với $R^n/Z^n$, và đặt $\varphi$ là đồng cấu chính tắc của $R^n$ lên $R^n/Z^n$. Mọi nhóm con của $T^n$ đều có dạng $G = \varphi(H)$, trong đó $H$ là một nhóm con của $R^n$ chứa $Z^n$ và đẳng cấu với $H/Z^n$ (Chương III, § 2, no. 7, Mệnh đề 20); để $G$ *đóng* trong $T^n$ thì cần và đủ để $H$ *đóng* trong $R^n$ (Chương I, § 3, no. 4). Do đó để tìm các nhóm con *đóng* của $T^n$ ta phải xác định tất cả các nhóm con *đóng* $H$ của $R^n$ chứa $Z^n$; để làm điều này ta sẽ sử dụng Mệnh đề 6 của no. 3, và trước hết ta xác định nhóm con $H^*$ liên kết với $H$. Vì $Z^n$ liên kết với chính nó, ta có $H^* \subset Z^n$; do đó (no. 1) tồn tại một cơ sở $(a_i)_{1 \leq i \leq n}$ của $R^n$ sinh ra $Z^n$, và một cơ sở của $H^*$ (đối với vành $Z$) gồm $p$ điểm $b_i$ ($1 \leq i \leq p$) sao cho $b_i = e_i a_i$ ($1 \leq i \leq p$), trong đó các $e_i$ là các số nguyên thỏa mãn các đồng dư thức $e_{i+1} \equiv 0 \pmod{e_i}$ với $1 \leq i \leq p-1$. Cho $(a'_i)$ là cơ sở đối ngẫu với $(a_i)$; khi đó $u = \sum_{i=1}^n u_i a_i$ thuộc $(H^*)^* = H$ khi và chỉ khi $u_i e_i \in Z$ với $1 \leq i \leq p$; nói cách khác, $H$ là tổng trực tiếp của không gian con vectơ $V$ sinh bởi $a'_{p+1}, \ldots, a_n$, và nhóm con rời rạc $K$ sinh bởi $p$ điểm
$$
e_i^{-1} a'_i \quad (1 \leq i \leq p).
$$
Mặt khác, $Z^n$ là tổng trực tiếp của $V \cap Z^n$ và $K \cap Z^n$, vì các $a'_i$ ($1 \leq i \leq n$) sinh ra $Z^n$. Do đó nhóm thương $H/Z^n$ đẳng cấu với $(V/(V \cap Z^n)) \times (K/(K \cap Z^n))$ (Chương III, § 2, no. 9, Hệ quả của Mệnh đề 26); $V/(V \cap Z^n)$ đẳng cấu với $T^{n-p}$, và $K/(K \cap Z^n)$ là một nhóm hữu hạn, tổng trực tiếp của $p$ nhóm cyclic có cấp $e_i$, lần lượt ($1 \leq i \leq p$) (xem no. 1).

Với cùng ký hiệu, mọi nhóm thương Hausdorff của $T^n$ có dạng $T^n/\varphi(H)$ và đẳng cấu với $R^n/H$ (Chương III, § 2, No. 7, Hệ quả của Mệnh đề 22); nếu $W$ là không gian con vectơ được sinh bởi $K$, thì $R^n/H$ đẳng cấu với $W/K$ (Chương III, § 2, No. 9, Hệ quả của Mệnh đề 26), tức là, $T^p$. Tóm lại:

MỆNH ĐỀ II. *Mọi nhóm con đóng của* $\mathbf{T}^n$ *đều đẳng cấu với một nhóm có dạng* $\mathbf{T}^h \times F$ *(0 \leq h \leq n)* *trong đó* $F$ *là một nhóm Abel hữu hạn, sao cho số nhỏ nhất các nhóm con chu trình mà* $F$ *là một tổng trực tiếp của chúng là* $\leq n - h$. *Mọi nhóm thương Hausdorff của* $\mathbf{T}^n$ *đều đẳng cấu với một nhóm có dạng* $\mathbf{T}^h$ *(0 \leq h \leq n)*.

Đặc biệt ($n = 1$):

#### Hệ quả {#top-vii-s1-n5-cor-1 .statement}

*Mọi nhóm con đóng của* $\mathbf{T}$, *trừ chính* $\mathbf{T}$, *là một nhóm cyclic hữu hạn.* *Mọi nhóm thương Hausdorff của* $\mathbf{T}$, *trừ* $\{0\}$, *đẳng cấu với* $\mathbf{T}$.

### 6. HÀM TUẦN HOÀN

ĐỊNH NGHĨA I. *Một hàm* $f$, *xác định trên* $\mathbf{R}^n$, *với giá trị trong một tập hợp tùy ý* $E$, *được gọi là tuần hoàn nếu tồn tại một điểm* $a \neq 0$ *trong* $\mathbf{R}^n$ *sao cho*

$$
f(x + a) = f(x)
$$

*với mọi* $x \in \mathbf{R}^n$. *Nếu* $f$ *tuần hoàn, thì mọi điểm* $a \in \mathbf{R}^n$ *mà quan hệ* (1) *là một đẳng thức theo* $x$ *được gọi là một chu kỳ của* $f$.

Tập hợp $G$ gồm tất cả các chu kỳ của một hàm tuần hoàn $f$ rõ ràng là một *nhóm con* (theo giả thiết không chỉ gồm riêng $0$) của nhóm cộng $\mathbf{R}^n$. Nếu $f$ là một ánh xạ tuần hoàn *liên tục* từ $\mathbf{R}^n$ vào một không gian tôpô *Hausdorff* $E$, thì nhóm chu kỳ $G$ của nó là *đóng*. Thật vậy, nếu $G_x$ ký hiệu tập hợp mọi $a \in \mathbf{R}^n$ sao cho $f(x + a) = f(x)$ đối với một điểm cho trước $x \in \mathbf{R}^n$, thì $G$ là giao của các $G_x$ khi $x$ chạy qua $\mathbf{R}^n$, và mỗi $G$ đều là *đóng* (Chương I, § 8, no. 1, Mệnh đề 2). Cho $V$ là không gian vectơ lớn nhất *được chứa* trong $G$ (no. 2, Định lý 2); hàm $f$ là *hằng* trên mọi lớp kề mod $V$; nếu $W$ là một không gian vectơ bổ sung với $V$, thì $f$ được xác định bởi *hạn chế* của nó lên $W$. Nói cách khác ($W$ là một nhóm tôpô đẳng cấu với $\mathbf{R}^p$ đối với một $p$ nào đó), việc nghiên cứu các hàm tuần hoàn liên tục trên $\mathbf{R}^n$ được quy về việc nghiên cứu các hàm như vậy mà nhóm chu kỳ $G$ của chúng là *rời rạc*; nếu nhóm này có hạng $g$, thì hàm $f$ được gọi là *tuần hoàn q lớp*, và mọi hệ tự do gồm $q$ điểm sinh ra $G$ được gọi là một *hệ chu kỳ chính* của $f$.

Nếu $(a_i)$ và $(b_i)$ là hai hệ chu kỳ chính của $f$, ta đã thấy (no. 1) rằng mỗi hệ có thể thu được từ hệ kia bằng một phép biến đổi tuyến tính với các hệ số nguyên và định thức $\pm 1$.

Cho $\varphi$ là ánh xạ chính tắc của $\mathbf{R}^n$ lên $\mathbf{R}^n/G$; với mọi ánh xạ $g$ từ $\mathbf{R}^n/G$ vào một tập hợp $E$ tương ứng với hàm $\dot{g} = g \circ \varphi$, là một ánh xạ tuần hoàn của $\mathbf{R}^n$ vào $E$, có nhóm chu kỳ là

### Bài tập {#top-vii-s1-exercises}

Xem [các bài tập của § 1](exercises/s1/).
