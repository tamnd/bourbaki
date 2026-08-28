---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: VI
chapter_title: ROOT SYSTEMS
section: 4
section_title: Classification of root systems
lang: vi
source: lie-iv-vi
pdf_pages: 0214-0246, 0255-0261
extraction: ocr
subsections:
    - "no": 1
      title: FINITE COXETER GROUPS
      page: 0
      pdf_page: 214
    - "no": 2
      title: DYNKIN GRAPHS
      page: 0
      pdf_page: 220
    - "no": 3
      title: AFFINE WEYL GROUP AND COMPLETED DYNKIN GRAPH
      page: 0
      pdf_page: 223
    - "no": 4
      title: PRELIMINARIES TO THE CONSTRUCTION OF ROOT SYSTEMS
      page: 0
      pdf_page: 225
    - "no": 5
      title: SYSTEMS OF TYPE $B_l$ ($l \geq 2$)
      page: 0
      pdf_page: 227
    - "no": 6
      title: SYSTEMS OF TYPE $C_l$ ($l \geq 2$)
      page: 0
      pdf_page: 229
    - "no": 7
      title: SYSTEMS OF TYPE $A_l$ ($l \geq 1$)
      page: 0
      pdf_page: 230
    - "no": 8
      title: SYSTEMS OF TYPE $D_l$ ($l \geq 3$)
      page: 0
      pdf_page: 233
    - "no": 9
      title: SYSTEM OF TYPE $F_4$
      page: 0
      pdf_page: 236
    - "no": 10
      title: SYSTEM OF TYPE E_8
      page: 0
      pdf_page: 238
    - "no": 11
      title: SYSTEM OF TYPE E_7
      page: 0
      pdf_page: 240
    - "no": 12
      title: SYSTEM OF TYPE E_6
      page: 0
      pdf_page: 242
    - "no": 13
      title: SYSTEM OF TYPE G_2
      page: 0
      pdf_page: 244
    - "no": 14
      title: IRREDUCIBLE NON-REDUCED ROOT SYSTEMS
      page: 0
      pdf_page: 246
statements: 19
exercises: 16
content_sha256: bdc8fed3213ab3fd019c65a67d192da4679d94c9f8afbc50def989256d5022a5
translated_from: content/en/lie/VI/04_s4_classification_of_root_systems.md
source_content_sha256: 0c153ae39564b4d702d2c032dca1d31b01e6780eaeb4dcb9c8642c3524393f7c
translation_model: gpt-5-6-mini, gpt-5-mini, gpt-5.4-mini, gpt-5-6
translation_run: translate-vi-3374a7d1
glossary_version: 34
glossary_terms_sha256: 23d02e2bfb15e9c11e81d46736d03d57d674fc7e89f4882fd20601beecb5b06b
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 4. PHÂN LOẠI CÁC HỆ NGHIỆM

### 1. CÁC NHÓM COXETER HỮU HẠN

Trong tiết này, ta sẽ xác định, sai khác một đẳng cấu, tất cả các hệ nghiệm, và do đó tất cả các nhóm kết tinh (§ 2, no. 5). Tổng quát hơn, ta sẽ bắt đầu bằng việc xác định tất cả các nhóm hữu hạn được sinh bởi các phép phản xạ trong một không gian vectơ thực hữu hạn chiều: điều này tương đương (Chương V, § 4, no. 8) với việc xác định tất cả các nhóm Coxeter hữu hạn, hoặc (Chương V, § 4, no. 8, Định lý 2) với việc xác định tất cả các ma trận Coxeter cấp hữu hạn sao cho dạng song tuyến tính liên kết là dương và không suy biến.

Cho $M = (m_{ij})_{i,j \in I}$ là một ma trận Coxeter cấp hữu hạn $l$. Đặt

$$
q_{ij} = -\cos(\pi / m_{ij}).
$$

Nhắc lại rằng $q_{ii} = 1$ và rằng $q_{ij} = q_{ji}$ là không hoặc $\leq -1/2$ với $i \neq j$. Đặt $E = \mathbf{R}^l$ và cho $(e_i)_{i \in I}$ là cơ sở chính tắc của $E$. Ký hiệu $(x|y)$ là dạng song tuyến tính trên $E$ liên kết với $M$ (Chương V, § 4, no. 1) và $q$ là dạng toàn phương $x \mapsto (x|x)$ trên $E$. Với $x = \sum_{i \in I} \xi_i x_i$,

$$
\| x \| ^2 = q(x) = \sum_{i,j \in I} q_{ij} \xi_i \xi_j.
$$

Ký hiệu $(X, f)$ là đồ thị Coxeter của $M$ (Chương IV, § 1, no. 9). Nếu $a$ là một cạnh của $X$, $f(a)$ được gọi là cấp của $a$.

Trong phần còn lại của số này, nhóm Coxeter $W(M)$ xác định bởi $M$ (Chương V, § 4, no. 3) được giả thiết là hữu hạn, do đó $q$ là dương và không suy biến và $X$ là một rừng (Chương V, § 4, no. 8, Mệnh đề 8). Ta cũng giả thiết rằng $X$ là liên thông (nói cách khác là nhóm Coxeter $W(M)$ là bất khả quy), do đó $X$ là một cây.

Từ điều kiện rằng $q$ là dương và không suy biến, ta sẽ thu được các điều kiện trên các $m_{ij}$ cho phép ta liệt kê tất cả các khả năng của các đồ thị Coxeter tương ứng; sẽ chỉ còn phải chứng minh rằng các khả năng này thực sự đạt được, nói cách khác rằng các nhóm $W(M)$ tương ứng là hữu hạn.

#### Bổ đề 1 {#lie-vi-s4-lem-1 .statement}

Với mọi $i$, $\sum_{j \neq i} q_{ij}^2 < 1$.

Cho $J$ là tập hợp các $j \in I$ sao cho $q_{ij} \neq 0$, nói cách khác sao cho $\{i, j\}$ là một cạnh của $X$. Nếu $j, j' \in J$ và $j \neq j'$, $\{j, j'\}$ không là một cạnh (nếu không thì $i, j, j'$ sẽ tạo thành một chu trình), do đó $(e_j|e_{j'}) = 0$. Đặt $F = \sum_{j \in J} \mathbf{R} e_j$. Khi đó $(e_j)_{j \in J}$ là một cơ sở trực chuẩn của $F$. Khoảng cách $d$ từ $e_i$ đến $F$ được cho bởi $d^2 = 1 - \sum_{j \in J} (e_i|e_j)^2 = 1 - \sum_{j \in J} q_{ij}^2 = 1 - \sum_{j \neq i} q_{ij}^2$, do đó có bổ đề.

#### Bổ đề 2 {#lie-vi-s4-lem-2 .statement}

Mọi đỉnh của $X$ thuộc vào nhiều nhất 3 cạnh.

Thật vậy, nếu $i$ liên kết với $h$ đỉnh khác, các hệ thức $q_{ij}^2 \geq \frac{1}{4}$ đối với các đỉnh khác này suy ra rằng $\frac{h}{4} < 1$ theo Bổ đề 1, do đó $h \leq 3$.

#### Bổ đề 3 {#lie-vi-s4-lem-3 .statement}

*Nếu $i$ thuộc vào 3 cạnh, các cạnh này có cấp 3.*

Nếu không, theo quan hệ $\cos \frac{\pi}{4} = \frac{\sqrt{2}}{2}$, ta sẽ có

$$
\sum_{j \neq i} q_{ij}^2 \geq \frac{1}{4} + \frac{1}{4} + (\frac{\sqrt{2}}{2})^2 = 1
$$

điều này là không thể (Bổ đề 1).

#### Bổ đề 4 {#lie-vi-s4-lem-4 .statement}

*Nếu tồn tại một cạnh có cấp $\geq 6$, thì $l = 2$.*

Thật vậy, cho $\{i, j\}$ là một cạnh như vậy. Nếu $l > 2$, một trong các đỉnh $i, j$ (giả sử là $i$) sẽ được nối với một đỉnh thứ ba $j'$, vì $X$ là liên thông. Theo quan hệ $\cos \frac{\pi}{6} = \frac{\sqrt{3}}{2}$ ta sẽ có

$$
\sum_{k \neq i} q_{ik}^2 \geq \frac{1}{4} + (\frac{\sqrt{3}}{2})^2 = 1
$$

điều này là không thể (Bổ đề 1).

#### Bổ đề 5 {#lie-vi-s4-lem-5 .statement}

*Một đỉnh không thể thuộc về hai cạnh phân biệt có cấp $\geq 4$.*

Cho $i$ là một đỉnh như vậy. Ta sẽ có $\sum_{j \neq i} q_{ij}^2 \geq (\frac{\sqrt{2}}{2})^2 + (\frac{\sqrt{2}}{2})^2 = 1$, điều này là không thể (Bổ đề 1).

Cho $\{i, j\}$ là một cạnh của $X$. Ta sẽ định nghĩa một đồ thị Coxeter mới, nhận được từ đồ thị của $M$ *bằng cách đồng nhất* $i$ *và* $j$. Tập hợp $I'$ các đỉnh của nó là thương của $I$ thu được bằng cách đồng nhất $i$ và $j$. Đặt $p = \{i, j\}$, là một phần tử của $I'$, và đồng nhất các phần tử của $I$ phân biệt với $i$ và $j$ với các ảnh chính tắc của chúng trong $I'$. Cho $k, k'$ là hai phần tử phân biệt của $I'$. Khi đó, $\{k, k'\}$ là một cạnh của đồ thị mới trong các trường hợp sau:

1) $k$ và $k'$ phân biệt với $p$ và $\{k, k'\}$ là một cạnh của $X$: trong trường hợp này, cấp của cạnh này được định nghĩa là $m_{kk'}$:

2) $k = p$, và một trong các tập hợp $\{i, k'\}, \{j, k'\}$ là một cạnh của $X$; cấp của $\{p, k'\}$ được định nghĩa là $m_{ik'}$ nếu $\{i, k'\}$ là một cạnh của $X$, và là $m_{jk'}$ nếu $\{j, k'\}$ là một cạnh của $X$ (hai khả năng này loại trừ lẫn nhau vì $X$ là một cây).

Cho $M' = (m'_{ij})_{i,j \in I'}$ là ma trận Coxeter mới được định nghĩa như vậy, và đặt $q'_{ij} = -\cos \frac{\pi}{m'_{ij}}$. Khi đó, với $k \neq p$, $t'_{pk} = q_{ik} + q_{jk}$. Do đó, nếu $(\xi_i) \in \mathbf{R}^{I'}$,

$$
\sum_{k, k' \in I'} q'_{kk'} \xi_k \xi_{k'} = \sum_{k, k' \in I} q_{kk'} \xi_k \xi_{k'} + \xi_p^2 - \xi_i^2 - \xi_j^2 - 2q_{ij} \xi_i \xi_j \tag{1}
$$
$$
= \sum_{k, k' \in I} q_{kk'} \xi_k \xi_{k'} - (1 + 2q_{ij}) \xi_p^2.
$$

#### Bổ đề 6 {#lie-vi-s4-lem-6 .statement}

*Nếu $\{i, j\}$ có cấp 3, $W(M')$ là một nhóm Coxeter hữu hạn.*

Thật vậy, $q_{ij} = -\frac{1}{2}$, do đó (1) trở thành

$$
\sum_{k,k' \in I'} q'_{kk'} \xi_k \xi_{k'} = \sum_{k,k' \in I} q_{kk'} \xi_k \xi_{k'}
$$

và $(\xi_k)_{k \in I'} \mapsto \sum_{k,k' \in I'} q'_{kk'} \xi_k \xi_{k'}$ là một dạng toàn phương dương không suy biến.
Bây giờ chỉ cần áp dụng Định lý 2 của Chương V. § 4, no. 8.

#### Bổ đề 7 {#lie-vi-s4-lem-7 .statement}

Ta có một trong các trường hợp sau:

a) X có một điểm phân nhánh duy nhất (Chương IV, Phụ lục, no. 1). và tất cả các cạnh của X đều có cấp 3.
b) X là một dây chuyền và có nhiều nhất một cạnh có cấp $\geq 4$.

Ta lập luận bằng quy nạp theo l.

a) Giả sử rằng X có một điểm phân nhánh i. Khi đó i thuộc 3 cạnh có cấp 3. $\{i, k_1\}, \{i, k_2\}, \{i, k_3\}$ (Các Bổ đề 2 và 3). Nếu $l = 4$ thì bổ đề được chứng minh. Nếu không, thì chẳng hạn $k_1$ thuộc một cạnh phân biệt với các cạnh vừa được nhắc đến vì X liên thông. Đồng nhất i và $k_1$ trong đồ thị Coxeter của M. Điều này cho một đồ thị mới mà giả thiết quy nạp có thể được áp dụng, theo Bổ đề 6. Khi đó ảnh $p$ của i là một điểm phân nhánh của đồ thị mới $X'$. Do đó $X'$ không có điểm phân nhánh nào khác và tất cả các cạnh của nó đều có cấp 3. Vậy tất cả các cạnh của X đều có cấp 3, và i và $k_1$ là các điểm phân nhánh duy nhất có thể có của nó. Nhưng nếu $k_1$ là một điểm phân nhánh của X, thì $p$ sẽ thuộc ít nhất 4 cạnh trong $X'$, trái với Bổ đề 2.

b) Giả sử rằng X không có điểm phân nhánh. Khi đó X là một dây chuyền (Chương IV, Phụ lục, no. 3, Mệnh đề 3). Gọi $\{i, j\}$ là một cạnh có cấp $\geq 4$. Nếu $l = 2$, thì bổ đề là tầm thường. Nếu không, thì chẳng hạn i thuộc một cạnh $\{i, k\}$ với $k \neq j$ (vì X liên thông). Cạnh này có cấp 3 (Bổ đề 5). Đồng nhất i và k trong đồ thị Coxeter của M. Theo Bổ đề 6, giả thiết quy nạp có thể được áp dụng. Gọi $p$ là ảnh của i trong đồ thị mới $X'$. Trong $X'$, $\{p, j\}$ là một cạnh có cấp $\geq 4$, do đó $X'$ không có cạnh nào khác có cấp $\geq 4$, và vì vậy $\{i, j\}$ là cạnh duy nhất có cấp $\geq 4$ trong X.

#### Bổ đề 8 {#lie-vi-s4-lem-8 .statement}

Cho $i_1, i_2, \ldots, i_p$ là các đỉnh của X sao cho $\{i_1, i_2\}, \{i_2, i_3\}, \ldots, \{i_{p-1}, i_p\}$ là các cạnh có cấp 3. Khi đó $q(\sum_{r=1}^p r e_{i_r}) = \frac{1}{2} p(p+1)$.

Ta có $(e_{i_r}|e_{i_r}) = 1, (e_{i_r}|e_{i_{r+1}}) = -\frac{1}{2}, (e_{i_r}|e_{i_s}) = 0$ nếu $s > r + 1$. Do đó

$$
q(\sum_{r=1}^p r e_{i_r}) = \sum_{r=1}^p r^2 - 2 \sum_{r=1}^{p-1} \frac{1}{2} r(r+1) = p^2 - \sum_{r=1}^{p-1} r.
$$

Theo Lý thuyết tập hợp, Chương III. § 5, no. 8. Hệ quả của Mệnh đề 14, điều này bằng

$$
p^2 - \frac{1}{2} p(p-1) = \frac{1}{2} p(p+1).
$$

#### Bổ đề 9 {#lie-vi-s4-lem-9 .statement}

Giả sử rằng X là một dây chuyền với các đỉnh 1, 2, ..., l và các cạnh {1, 2}, {2, 3}, ..., {l - 1, l}.

(i) Nếu một trong các cạnh {2, 3}, {3, 4}, ..., {l - 2, l - 1} có cấp $\geq 4$, cạnh này có cấp 4 và đồ thị là như sau:

![Graph with 4 nodes connected in a chain](../images/chain_4.png)

(ii) Nếu cạnh {1, 2} có cấp 5, đồ thị là một trong các đồ thị sau:

![Graphs with 5 nodes connected in chains](../images/chains_5.png)

Ta có thể giả sử rằng $l > 2$ (Bổ đề 4). Giả sử rằng $\{i, i + 1\}$ có cấp $\geq 4$, với $1 \leq i \leq l - 1$. Đặt

$$
x = e_1 + 2e_2 + \cdots + ie_i,\ y = e_i + 2e_{l-1} + \cdots + (l - i)e_{i+1}, \text{ và } j = l - i.
$$

Theo Bổ đề 8, $\| x \| ^2 = \frac{1}{2} i(i + 1)$, $\| y \| ^2 = \frac{1}{2} j(j + 1)$. Mặt khác, $(x|y) = ij(e_i|e_{i+1}) = -ij \cos \frac{\pi}{m}$ với $m = 4$ hoặc 5 (Bổ đề 4). Bây giờ

$$
(x|y)^2 < \| x \| ^2 \| y \| ^2.
$$

suy ra

$$
\frac{1}{4} ij(i + 1)(j + 1) > i^2 j^2 \cos^2 \frac{\pi}{m}
$$

do đó

$$
(i + 1)(j + 1) > 4ij \cos^2 \frac{\pi}{m} \geq 2ij.
$$

Điều này trước hết cho $ij - i - j - 1 < 0$, hay $(i - 1)(j - 1) < 2$. Nếu

$$
1 < i < l - 1,
$$

thì $1 < j < l - 1$, vậy $i = j = 2$, và do đó $^1$

$$
9 > 16 \cos^2 \frac{\pi}{m}, \text{ do đó } \cos^2 \frac{\pi}{m} < \cos^2 \frac{\pi}{5}
$$

và do đó $m = 4$. Điều này chứng minh (i). Nếu $i = 1$ và $m = 5$, thì $2j + 2 > 4j \frac{3+\sqrt{5}}{8}$, hoặc $j \frac{\sqrt{5}-1}{2} < 2, j < \sqrt{5} + 1 < 4$, và do đó $l = j + 1 \leq 4$. Điều này chứng minh (ii).

$^1$ Các nghiệm bậc 5 của 1 phân biệt với 1 là các nghiệm của $z^4 + z^3 + z^2 + z + 1 = 0$. Đặt $x = \frac{1}{2}(z + \frac{1}{z})$, phương trình này trở thành $(2x)^2 - 2 + 2x + 1 = 0$, hay $4x^2 + 2x - 1 = 0$, do đó $x = \frac{-1 \pm \sqrt{5}}{4}$. Suy ra,

$$
2 \cos^2 \frac{\pi}{5} - 1 = \cos \frac{2\pi}{5} = \frac{\sqrt{5} - 1}{4}, \quad \cos^4 \frac{\pi}{5} = \frac{3 + \sqrt{5}}{8} > \frac{5}{8} > \frac{9}{16}, \quad \cos \frac{\pi}{5} = \frac{1 + \sqrt{5}}{4}.
$$

#### Bổ đề 10 {#lie-vi-s4-lem-10 .statement}

Nếu X có một điểm phân nhánh i, đồ thị con đầy đủ X - {i} là hợp của ba chuỗi, và nếu p - 1, q - 1, r - 1 là độ dài của các chuỗi này, thì bộ ba {p, q, r} bằng, sai khác một phép hoán vị, một trong các bộ ba {1, 2, 2}, {1, 2, 3}, {1, 2, 4}, {1, 1, m} (với một số m $\geq 1$).

Đỉnh i thuộc về 3 cạnh (Bổ đề 2), và không có điểm phân nhánh nào khác (Bổ đề 7), do đó đồ thị con đầy đủ X - {i} là tổng của 3 chuỗi X_1, X_2, X_3, mỗi chuỗi trong đó có một đỉnh tận cùng được nối với i trong X. Gọi {i_1, i_2}, {i_2, i_3}, ..., {i_{p-1}, i_p} là các cạnh của X_1, {j_1, j_2}, {j_2, j_3}, ..., {j_{q-1}, j_q} là các cạnh của X_2, và {k_1, k_2}, {k_2, k_3}, ..., {k_{r-1}, k_r} là các cạnh của X_3, với i_1, j_1, k_1 được nối với i trong X. Ta có thể giả sử rằng $p \geq q \geq r \geq 1$. Đặt

$$
x = e_{i_p} + 2e_{i_{p-1}} + \cdots + pe_{i_1}
$$
$$
y = e_{j_q} + 2e_{j_{q-1}} + \cdots + qe_{j_1}
$$
$$
z = e_{k_r} + 2e_{k_{r-1}} + \cdots + re_{k_1}.
$$

Vì tất cả các cạnh của X đều có cấp 3 (Bổ đề 7), Bổ đề 8 cho $\| x \| ^2 = \frac{1}{2} p(p+1)$, $\| y \| ^2 = \frac{1}{2} q(q+1)$, $\| z \| ^2 = \frac{1}{2} r(r+1)$. Mặt khác, $e_i$ vuông góc với $e_{i_2}, e_{i_3}, \ldots, e_{i_p}$, nên $(e_i | x) = p(e_i | e_{i_1}) = -\frac{1}{2} p$; tương tự $(e_i | y) = -\frac{1}{2} q$, $(e_i | z) = -\frac{1}{2} r$. Các vectơ đơn vị $\| x \|^{-1} x, \| y \|^{-1} y, \| z \|^{-1} z$ đôi một vuông góc, và $e_i$ không thuộc không gian con F mà chúng sinh ra; bình phương khoảng cách từ $e_i$ đến F là

$$
1 - (e_i | \frac{x}{\| x \|})^2 - (e_i | \frac{y}{\| y \|})^2 - (e_i | \frac{z}{\| z \|})^2
$$
$$
= 1 - \frac{1}{2} \frac{p}{p+1} - \frac{1}{2} \frac{q}{q+1} - \frac{1}{2} \frac{r}{r+1}
$$
$$
= 1 - \frac{1}{2} + \frac{1}{2} \frac{1}{p+1} - \frac{1}{2} + \frac{1}{2} \frac{1}{q+1} - \frac{1}{2} + \frac{1}{2} \frac{1}{r+1}.
$$

Vì đại lượng này > 0, ta có

$$
(p+1)^{-1} + (q+1)^{-1} + (r+1)^{-1} > 1.
$$ (4)

Suy ra $3(r+1)^{-1} > 1$, do đó $r < 2$ và cuối cùng $r = 1$. Khi đó (4) cho

$$
(p+1)^{-1} + (q+1)^{-1} > \frac{1}{2}
$$ (5)

suy ra $2(q+1)^{-1} > \frac{1}{2}$, do đó $q \leq 2$. Cuối cùng, nếu $q = 2$, (5) cho

$$
(p+1)^{-1} > \frac{1}{6}. \quad \text{do đó } p \leq 4.
$$

#### Định lý 1 {#lie-vi-s4-thm-1 .statement}

Đồ thị của mọi hệ Coxeter hữu hạn bất khả quy (W, S) là đẳng cấu với một trong các đồ thị sau:

A_l   (l \geq 1\ vertices)
B_l   (l \geq 2\ vertices)
D_l   (l \geq 4\ vertices)
E_6
E_7
E_8
F_4   4
G_2   6
H_3   5
H_4   5
I_2(p)   p (p = 5\ or\ p \geq 7).

Không có hai đồ thị nào trong số này là đẳng cấu.

Thật vậy, cho W = (m_{ij}) là ma trận Coxeter của (W, S), và cho l = Card(S). Nếu một trong các m_{ij} là $\geq 6$, thì l = 2 (Bổ đề 4) và đồ thị Coxeter của (W, S) là kiểu G_2 hoặc I_2(p) với p \geq 7. Bây giờ giả sử rằng mọi m_{ij} \leq 5.

a) Nếu các m_{ij} không phải tất cả đều bằng 3, đồ thị X của (W, S) là một chuỗi và đúng một trong các m_{ij} bằng 4 hoặc 5 (Bổ đề 7). Nếu một trong các m_{ij} bằng 5, Bổ đề 9 chỉ ra rằng ta có một trong các kiểu H_3, H_4 hoặc I_2(5). Nếu một trong các m_{ij} bằng 4, Bổ đề 9 chỉ ra rằng ta có một trong các kiểu B_l hoặc F_4.

b) Bây giờ giả sử rằng mọi m_{ij} đều bằng 3. Nếu X là một chuỗi, đồ thị Coxeter là kiểu A_l. Nếu không, Bổ đề 10 chỉ ra rằng nó là kiểu E_6, E_7, E_8 hoặc D_l.

Việc không có hai đồ thị Coxeter nào được liệt kê là đẳng cấu là hiển nhiên.

Ngược lại:

#### Định lý 2 {#lie-vi-s4-thm-2 .statement}

Các nhóm Coxeter được xác định bởi các đồ thị Coxeter A_l, B_l, ..., I_2(p) của Định lý 1 là hữu hạn.

Điều này hiển nhiên đối với I_2(p), nhóm tương ứng là nhóm nhị diện có cấp 2p (Chap. IV, § 1, no. 9). Đối với H_4 dạng toàn phương tương ứng là

$$
\xi_1^2 + \xi_2^2 + \xi_3^2 + \xi_4^2 - \xi_1 \xi_2 - \xi_2 \xi_3 - 2(\cos \frac{\pi}{5}) \xi_3 \xi_4
$$
$$
= \xi_1^2 + \xi_2^2 + \xi_3^2 + \xi_4^2 - \xi_1 \xi_2 - \xi_2 \xi_3 - \frac{1 + \sqrt{5}}{2} \xi_3 \xi_4
$$
$$
= (\xi_2 - \frac{\xi_1 + \xi_3}{2})^2 + (\xi_4 - \frac{1 + \sqrt{5}}{4} \xi_3)^2 + \frac{3}{4} (\xi_1 - \frac{1}{3} \xi_3)^2 + \frac{7 - 3 \sqrt{5}}{24} \xi_3^2.
$$

Vì $7 - 3 \sqrt{5}$ là $> 0$, dạng này là xác định dương không suy biến, và nhóm Coxeter tương ứng là hữu hạn. Điều tương tự cũng đúng đối với nhóm tương ứng với $H_3$, vì nó đẳng cấu với một nhóm con của nhóm trên (Chap. IV, § 1, no. 8).

Đối với các kiểu $A_l, B_l, \ldots, G_2$, ta sẽ xây dựng, trong Nos. 5 đến 13, các hệ nghiệm có các nhóm tương ứng làm các nhóm Weyl. Ta sẽ thấy rằng các nhóm này không chỉ hữu hạn, mà còn *tinh thể* (§ 2, no. 5).

### 2. ĐỒ THỊ DYNKIN

Do lạm dụng ngôn ngữ, ta sẽ gọi một *đồ thị chuẩn hóa* là một cặp $(\Gamma, f)$ có các tính chất sau:

1) $\Gamma$ là một đồ thị (được gọi là đồ thị *nền* của $(\Gamma, f)$).

2) Nếu $E$ chỉ tập hợp các cặp $(i, j)$ sao cho $\{i, j\}$ là một cạnh của $\Gamma$, thì $f$ là một ánh xạ từ $E$ vào $\mathbf{R}$ sao cho $f(i, j) f(j, i) = 1$ với mọi $(i, j) \in E$.

Có một khái niệm hiển nhiên về đẳng cấu của các đồ thị chuẩn hóa.

Cho $R$ là một hệ căn rút gọn trong một không gian vectơ thực $V$. Ta sẽ liên kết với nó một đồ thị có chuẩn $(X, f)$, được gọi là đồ thị *Dynkin* của $R$. Các đỉnh của $X$ sẽ là các phần tử của tập hợp $I$ gồm các quỹ đạo của $W(R)$ trong hợp của các tập hợp $\{B\} \times B$ (trong đó $B$ là tập hợp các cơ sở của $R$). Nếu $N = (n_{ij})_{i,j \in I}$ (tương ứng $M = (m_{ij})_{i,j \in I}$) là ma trận Cartan chính tắc (tương ứng ma trận Coxeter) của $R$ (§ 1, no. 5, *Nhận xét 7*), hai đỉnh $i$ và $j$ của $X$ được nối với nhau khi và chỉ khi $n_{ij} \neq 0$ và khi đó ta đặt
$$
f(i, j) = \frac{n_{ij}}{n_{ji}}.
$$
Vì $n_{ij} = 0$ kéo theo $n_{ji} = 0$, điều này xác định một đồ thị có chuẩn $(X, f)$.

Cho $(x|y)$ là một tích vô hướng trên $V$, bất biến dưới tác động của $W(R)$, và cho $B = (\alpha_i)_{i \in I}$ là một cơ sở của $R$, được đánh chỉ số một cách chính tắc. Các công thức (7) và (9) của § 1, no. 1 chỉ ra rằng các đỉnh $i$ và $j$ của đồ thị $X$ được nối với nhau khi và chỉ khi
$$
(\alpha_i|\alpha_j) \neq 0
$$
và rằng
$$
f(i, j) = \frac{(\alpha_i|\alpha_i)}{(\alpha_j|\alpha_j)}.
$$

Theo các kết quả của § 1, các số 3 và 5, các khả năng duy nhất là các khả năng sau đây, sai khác bởi việc đổi chỗ $i$ và $j$:

1) $i$ và $j$ không được nối; $n_{ij} = n_{ji} = 0; m_{ij} = 2;$
2) $f(i, j) = f(j, i) = 1; n_{ij} = n_{ji} = -1; m_{ij} = 3;$
3) $f(i, j) = 2, f(j, i) = 1/2; n_{ij} = -2, n_{ji} = -1; m_{ij} = 4;$
4) $f(i, j) = 3, f(j, i) = 1/3; n_{ij} = -3, n_{ji} = -1; m_{ij} = 6.$

Ta thấy từ điều này rằng đồ thị Dynkin $R$ xác định ma trận Cartan và ma trận Coxeter của $R$, và do đó xác định $R$ sai khác bởi một đẳng cấu. Chính xác hơn, Hệ quả của Mệnh đề 15 của § 1, no. 5 suy ra kết quả sau:

#### Mệnh đề 1 {#lie-vi-s4-prop-1 .statement}

*Cho $R_1$ và $R_2$ là hai hệ căn rút gọn trong các không gian vectơ $V_1$ và $V_2$. Cho $B_1 = (\alpha_i)_{i \in I_1}$ và $B_2 = (\alpha_i)_{i \in I_2}$ là các cơ sở của $R_1$ và $R_2$, được đánh chỉ số một cách chính tắc. Cho $\lambda$ là một đẳng cấu từ đồ thị Dynkin của $R_1$ đến đồ thị Dynkin của $R_2$. Khi đó, tồn tại một đẳng cấu duy nhất từ $V_1$ đến $V_2$ biến $R_1$ thành $R_2$ và $\alpha_i$ thành $\alpha_{\lambda(i)}$ với mọi $i \in I_1$.*

It is clear that một tự đẳng cấu của $R$ xác định một tự đẳng cấu của biểu đồ Dynkin của $R$, và do đó một đồng cấu $\varphi$ từ nhóm $A(R)$ đến nhóm các tự đẳng cấu của biểu đồ Dynkin của $R$.

#### Hệ quả {#lie-vi-s4-n2-cor-1 .statement}

*Đồng cấu $\varphi$ xác định, qua thương, một đẳng cấu từ nhóm $A(R)/W(R)$ đến nhóm các tự đẳng cấu của biểu đồ Dynkin của $R$.*

Rõ ràng, $\varphi(g) = \mathrm{Id}$ với mọi $g \in W(R)$. Mặt khác, Mệnh đề 1 cho thấy tồn tại một đẳng cấu $\psi$ từ nhóm các đẳng cấu của biểu đồ Dynkin của $R$ đến nhóm con $E$ gồm các phần tử của $A(R)$ giữ cố định một cơ sở $B$ đã cho của $R$, sao cho $\varphi \circ \psi = \mathrm{Id}$. Vì $A(R)$ là tích nửa trực tiếp của $E$ và $W(R)$ (\S 1, no. 5, Mệnh đề 16), hệ quả suy ra.

Trong thực hành, biểu đồ Dynkin $(X, f)$ được biểu diễn bởi một sơ đồ gồm các nút và các liên kết theo cách sau. Các nút tương ứng với các đỉnh của $X$; hai nút tương ứng với hai đỉnh phân biệt $i$ và $j$ được nối bởi 0, 1, 2 hoặc 3 liên kết trong các trường hợp 1), 2), 3) và 4) ở trên (xét đến việc đổi chỗ $i$ và $j$). Hơn nữa, trong các trường hợp 3) và 4), tức là khi $f(i, j) > 1$, hoặc khi các nghiệm $\alpha_i$ và $\alpha_j$ không trực giao và không cùng độ dài, dấu bất đẳng thức $>$ được đặt trên liên kết kép hoặc liên kết ba nối các nút tương ứng với $i$ và $j$, hướng về nút tương ứng với $j$ (tức là nghiệm ngắn nhất):

$$
\begin{array}{cc}
\circ \Longrightarrow \circ & \text{(với } f(i, j) = 2 \text{).} \\
\circ \Rrightarrow \circ & \text{(với } f(i, j) = 3 \text{).}
\end{array}
$$

Rõ ràng biểu đồ $(X, f)$ có thể được phục hồi từ sơ đồ này.

Ta nhận xét rằng sơ đồ gắn với biểu đồ Coxeter của $W(R)$ có thể thu được từ sơ đồ gắn với biểu đồ Dynkin của $R$ bằng cách giữ lại các nút và các liên kết đơn rồi thay các liên kết kép (tương ứng liên kết ba) bằng một liên kết có số 4 (tương ứng 6) ở trên. Ngược lại, cho biểu đồ Coxeter của W(R), sơ đồ gắn với biểu đồ Dynkin của R có thể được phục hồi bằng cách dùng phép ngược của thủ tục này, trừ các dấu bất đẳng thức trên các liên kết kép hoặc ba. Định lý 1 do đó cho ngay lập tức danh sách các biểu đồ Dynkin có thể có. Chính xác hơn:

#### Định lý 3 {#lie-vi-s4-thm-3 .statement}

*Nếu R là một hệ nghiệm rút gọn bất khả quy, biểu đồ Dynkin của nó đẳng cấu với một trong các biểu đồ được biểu diễn bởi các sơ đồ sau:*

$$
\begin{array}{ll}
A_l & \circ-\cdots-\circ \quad (l \geq 1 \text{ đỉnh }) \\
B_l & \circ-\cdots-\circ-\circ \quad (l \geq 2 \text{ đỉnh }) \\
C_l & \circ-\cdots-\circ-\circ \quad (l \geq 3 \text{ đỉnh }) \\
D_l & \circ-\cdots-\circ-\circ-\circ \quad (l \geq 4 \text{ đỉnh }) \\
E_6 & \circ-\cdots-\circ \\
E_7 & \circ-\cdots-\circ-\circ-\circ \\
E_8 & \circ-\cdots-\circ-\circ-\circ-\circ \\
F_4 & \circ-\circ-\circ-\circ \\
G_2 & \circ-\circ-\circ
\end{array}
$$

*Không có hai biểu đồ nào trong số này đẳng cấu với nhau và tồn tại các hệ nghiệm rút gọn bất khả quy có từng biểu đồ ấy làm biểu đồ Dynkin của chúng (xét đến đẳng cấu).*

Mệnh đề thứ nhất suy ra ngay từ Định lý 1, xét các nhận xét trên, thực tế là các nhóm Coxeter của các biểu đồ H_3, H_4 và I_2(p) (với p = 5 và p \geq 7) không kết tinh, và thực tế là hai khả năng có thể có cho dấu bất đẳng thức trên liên kết kép (tương ứng liên kết ba) của biểu đồ Dynkin gắn với biểu đồ Coxeter F_4 (tương ứng G_2) cho các biểu đồ Dynkin đẳng cấu. Mệnh đề thứ hai hiển nhiên và mệnh đề thứ ba sẽ suy ra từ phép dựng tường minh của một hệ nghiệm rút gọn bất khả quy cho mỗi kiểu, một phép dựng sẽ được thực hiện trong các số 5 đến 13.

#### Nhận xét 1 {#lie-vi-s4-n2-rem-1 .statement}

Biểu đồ A_1 rút gọn thành một nút duy nhất; ta cũng ký hiệu nó bằng B_1 hoặc C_1. Biểu đồ B_2 \circ-\circ-\circ-\circ cũng được ký hiệu bởi C_2. Biểu đồ A_3 \circ-\cdots-\circ cũng được ký hiệu bởi D_3. Cuối cùng, D_2 ký hiệu biểu đồ gồm hai nút không nối với nhau. (Các quy ước này suy ra từ các tính chất của các hệ nghiệm tương ứng, xem các số 5 đến 8.)

#### Nhận xét 2 {#lie-vi-s4-n2-rem-2 .statement}

Nếu (X, f) là biểu đồ Dynkin của một hệ nghiệm rút gọn R, biểu đồ Dynkin của hệ ngược có thể được đồng nhất với (X, f^{-1}). Nói cách khác, sơ đồ gắn với biểu đồ Dynkin của R^- có thể thu được từ sơ đồ gắn với biểu đồ Dynkin của R bằng cách đảo ngược các dấu bất đẳng thức. Nếu R bất khả quy, ta thấy R đẳng cấu với R^- trừ khi R thuộc kiểu B_l hoặc C_l, trong trường hợp ấy R^- thuộc kiểu C_l hoặc B_l.

### 3. NHÓM WEYL AFFINE VÀ BIỂU ĐỒ DYNKIN HOÀN CHỈNH

Cho R là một hệ nghiệm rút gọn bất khả quy và cho (X, f) là biểu đồ Dynkin của nó. Ta sẽ định nghĩa một biểu đồ có chuẩn khác (\tilde{X}, \tilde{f}) mà ta sẽ gọi là biểu đồ Dynkin hoàn chỉnh của R. Tập \tilde{I} các đỉnh của \tilde{X} gồm tập I các đỉnh của X và một đỉnh ký hiệu là 0, không thuộc I. Để định nghĩa \tilde{f}, chọn một cơ sở B = (\alpha_i)_{i \in I} của R và một tích vô hướng \langle x | y \rangle bất biến dưới W(R). Cho \alpha_0 là đối của nghiệm cao nhất theo thứ tự do B xác định. Hai đỉnh phân biệt i, j \in \tilde{I} được nối với nhau khi và chỉ khi \langle \alpha_i | \alpha_j \rangle \neq 0 và khi đó ta đặt

$$
\tilde{f}(i, j) = \frac{\langle \alpha_i | \alpha_i \rangle}{\langle \alpha_j | \alpha_j \rangle}.
$$

Rõ ràng biểu đồ \tilde{X} và ánh xạ \tilde{f} được định nghĩa như vậy không phụ thuộc vào lựa chọn B hay tích vô hướng.

Nếu hạng l của R bằng 1, thì $I = \{i\}$ và $\alpha_0 = -\alpha_1$; do đó $\tilde{f}(0, i) = 1$. Nếu $l \geq 2$, $\alpha_0$ không tỉ lệ với bất kỳ $\alpha_i$ nào và $\langle \alpha_0 | \alpha_i \rangle$ là $\leq 0$ (\S 1, no. 8, Prop. 25). Với mọi cặp $(i, j)$ gồm các phần tử phân biệt của $\tilde{I}$, các khả năng duy nhất là các khả năng được ký hiệu bởi 1), 2), 3), 4) trong số trước (đặt, chẳng hạn, $n_{0i} = n(\alpha_0, \alpha_i)$ và $m_{0i} = order of s_{\alpha_0} s_{\alpha_i}$ với mọi $i \in I$).

Trong trường hợp $l \geq 2$, biểu đồ Dynkin hoàn chỉnh được biểu diễn bởi một biểu đồ với cùng các quy ước như trong số trước, đôi khi chỉ ra bằng các đường chấm các liên kết nối đỉnh 0 với các đỉnh khác. Ta nhận xét rằng dấu bất đẳng thức > trên một liên kết như vậy, nếu tồn tại, luôn có hướng về phía đỉnh phân biệt với 0, vì $\alpha_0$ là một nghiệm dài nhất (\S 1, no. 8, Prop. 25). Đồ thị $(X, f)$ là đồ thị con thu được từ $(\tilde{X}, \tilde{f})$ bằng cách xóa đỉnh 0.

Tác động của $A(R)$ trên $(X, f)$ mở rộng thành một tác động trên $(\tilde{X}, \tilde{f})$, giữ cố định 0, và $W(R)$ tác động tầm thường trên $(\tilde{X}, \tilde{f})$.

Ta giữ lại các ký hiệu của \S 2, Prop. 5 của \S 2, no. 2, cùng với Th. 1 của Chap. V, \S 3, no. 2, cho thấy rằng đồ thị Coxeter $\Sigma$ của nhóm Weyl affine $W_a(R)$ có thể thu được từ $(\tilde{X}, \tilde{f})$ bởi cùng các quy tắc mà đồ thị Coxeter của $W(R)$ được thu được từ $(X, f)$. Mặt khác, cho $G$ là chuẩn hóa tử của $W_a(R)$ (\S 2, no. 3). Với mỗi $g \in G$ tương ứng một tự đẳng cấu $\varphi(g)$ của $\Sigma$ và $\varphi(g) = \mathrm{Id}$ nếu $g \in W_a(R)$. Ngược lại, cho một tự đẳng cấu $\lambda$ của $\Sigma$ thì có, theo Prop. 11 của Chap. V, \S 4, no. 9, một phần tử duy nhất $g = \psi(\lambda)$ bảo toàn một alcôvơ $C$ đã cho và sao cho $\varphi(g) = \lambda$. Vì $G$ là tích nửa trực tiếp của nhóm con $G_C$ gồm các phần tử bảo toàn $C$ và $W_a(R)$ (\S 2, no. 3), ta suy ra rằng $\varphi$ xác định qua phép chuyển sang thương một đẳng cấu từ $G/W_a$ (hoặc từ $G_C$) đến $\operatorname{Aut}(\Sigma)$. Hiển nhiên rằng hợp của đẳng cấu này với ánh xạ chính tắc từ $A(R)/W(R)$ đến $G/W_a$ trùng với đồng cấu từ $A(R)/W(R)$ đến $\operatorname{Aut}(\Sigma)$ cảm sinh bởi đồng cấu từ $A(R)/W(R)$ đến $\operatorname{Aut}(\tilde{X}, \tilde{f})$ được định nghĩa ở trên. Theo \S 2, no. 3, nhóm $\operatorname{Aut}(\Sigma)$ đẳng cấu với tích nửa trực tiếp của

$A(R)/W(R)$ bởi $P(R^*)/Q(R^*)$. và $P(R^*)/Q(R^*)$ đẳng cấu với nhóm $I_C = G_C \cap W'_a$ (với ký hiệu của § 2, no. 3): phần tử của $\operatorname{Aut}(\Sigma)$ tương ứng với phần tử $\gamma_i$ của $I_C$ biến đỉnh 0 thành đỉnh $i$ của $\Sigma$.

#### Nhận xét {#lie-vi-s4-n3-rem-1 .statement}

Có thể chứng minh rằng ánh xạ chính tắc
$$
\operatorname{Aut}(\tilde{X}, \tilde{f}) \to \operatorname{Aut}(\Sigma)
$$
là một đẳng cấu.

#### Định lý 4 {#lie-vi-s4-thm-4 .statement}

Cho $(W, S)$ là một hệ Coxeter bất khả quy với $S$ hữu hạn. Dạng toàn phương liên kết (Chap. V, § 4, no. 1) là dương và suy biến khi và chỉ khi đồ thị Coxeter của $(W, S)$ đẳng cấu với một trong các đồ thị sau:

$$
\begin{array}{ll}
\tilde{A}_1 & \circ \longrightarrow \infty \\
\tilde{A}_l \quad (l \geq 2) & \circ \longrightarrow \cdots \longrightarrow \circ \quad \text{(mạch với } l + 1 \text{ đỉnh)} \\
\tilde{B}_2 & \circ \longrightarrow 4 \longrightarrow \circ \\
\tilde{B}_l \quad (l \geq 3) & \circ \longrightarrow \cdots \longrightarrow \circ \longrightarrow 4 \quad \text{(l + 1 đỉnh)} \\
\tilde{C}_l \quad (l \geq 3) & \circ \longrightarrow 4 \longrightarrow \cdots \longrightarrow 4 \quad \text{(l + 1 đỉnh)} \\
\tilde{D}_l \quad (l \geq 4) & \circ \longrightarrow \cdots \longrightarrow \circ \quad \text{(l + 1 đỉnh)} \\
\tilde{E}_6 & \circ \longrightarrow \circ \longrightarrow \circ \longrightarrow \circ \\
\tilde{E}_7 & \circ \longrightarrow \circ \longrightarrow \circ \longrightarrow \circ \longrightarrow \circ \\
\tilde{E}_8 & \circ \longrightarrow \circ \longrightarrow \circ \longrightarrow \circ \longrightarrow \circ \longrightarrow \circ \\
\tilde{F}_4 & \circ \longrightarrow \circ \longrightarrow 4 \longrightarrow \circ \\
\tilde{G}_2 & \circ \longrightarrow 6 \longrightarrow \circ
\end{array}
$$

Không có hai đồ thị Coxeter nào trong số này đẳng cấu với nhau.

Theo Chap. V, § 4, no. 9 và Prop. 8 của § 2, no. 5, các hệ Coxeter có dạng toàn phương dương và suy biến là những hệ tương ứng với các nhóm Weyl affine của các hệ nghiệm bất khả quy thu gọn. Vì vậy định lý suy ra từ việc xác định các đồ thị Dynkin hoàn chỉnh được thực hiện trong các no. 5 đến 13 dưới đây.

### 4. CÁC CHUẨN BỊ CHO PHÉP DỰNG CÁC HỆ NGHIỆM

Cho V là một không gian vectơ thực có chiều $l \geq 1$ được trang bị một tích vô hướng $(x|y)$, L là một nhóm con rời rạc của V, $\Lambda$ là một tập hữu hạn các số > 0, và R là tập hợp các $\alpha \in L$ sao cho $(\alpha|\alpha) \in \Lambda$. Giả sử rằng R sinh ra V và rằng, với mọi cặp $(\alpha, \beta)$ các điểm của R, số $2 \frac{(\alpha|\beta)}{(\alpha|\alpha)}$ là một số nguyên. Khi đó, R *là một hệ nghiệm trong* V. Thật vậy, R rõ ràng thỏa mãn (RS_I). Cho $\alpha \in R$; gọi $s_{\alpha}$ là phép phản xạ trực giao $x \mapsto x - 2 \frac{(x|\alpha)}{(\alpha|\alpha)} \alpha$: khi đó, nếu $\beta \in R$, ta có $2 \frac{(\beta|\alpha)}{(\alpha|\alpha)} \in \mathbf{Z}$, do đó $s_{\alpha}(\beta) \in L$, và hơn nữa $\| s_{\alpha}(\beta) \| = \| \beta \|$, do đó $s_{\alpha}(\beta) \in R$; vậy R thỏa mãn (RS_{II}) và (RS_{III}), và là thu gọn nếu $\Lambda$ không chứa hai số có dạng $\lambda$ và $4\lambda$.

Bây giờ cho V là một không gian con của $E = \mathbf{R}^n$. Cho $(\varepsilon_1, \ldots, \varepsilon_n)$ là cơ sở chính tắc của E; ta trang bị cho E tích vô hướng sao cho cơ sở này là trực chuẩn và đồng nhất $E^*$ với E (resp. $V^*$ với V) nhờ tích vô hướng này. Ta định nghĩa các nhóm con $L_0, L_1, L_2, L_3$ của E như sau:

1) $L_0$ là $\mathbf{Z}$-môđun có cơ sở $(\varepsilon_i)$. Ta có $(\alpha|\beta) \in \mathbf{Z}$ với mọi $\alpha, \beta \in L_0$. Các vectơ $\alpha \in L_0$ sao cho $(\alpha|\alpha) = 1$ là các $\pm \varepsilon_i$ ($1 \leq i \leq n$); những vectơ sao cho $(\alpha|\alpha) = 2$ là các $\pm \varepsilon_i \pm \varepsilon_j$ với $i < j$ (hai dấu $\pm$, trong $\pm \varepsilon_i \pm \varepsilon_j$, được chọn độc lập với nhau; ta chấp nhận quy ước tương tự trong toàn bộ phần còn lại của mục này).

2) $L_1$ là $\mathbf{Z}$-môđun con của $L_0$ gồm các $x = \sum_{i=1}^n \xi_i \varepsilon_i \in L_0$ sao cho $\sum_{i=1}^n \xi_i$ là chẵn; vì $\xi_i$ và $\xi_i^2$ có cùng tính chẵn lẻ, điều này tương đương với việc yêu cầu rằng $(x|x)$ là chẵn. Gọi $L_1'$ là môđun con của $L_1$ sinh bởi các $\varepsilon_i \pm \varepsilon_j$; ta có $\sum_{i=1}^n \xi_i \varepsilon_i \equiv (\sum_{i=1}^n \xi_i) \varepsilon_n \pmod{L_1'}$, và vì $2\varepsilon_n = (\varepsilon_1 + \varepsilon_n) - (\varepsilon_1 - \varepsilon_n) \in L_1'$, suy ra rằng $L_1' = L_1$. Vì $L_0$ được sinh bởi $L_1$ và $\varepsilon_1$, $L_0/L_1$ đẳng cấu với $\mathbf{Z}/2\mathbf{Z}$.

3) $L_2 = L_0 + \mathbf{Z}(\frac{1}{2} \sum_{i=1}^n \varepsilon_i)$. Rõ ràng một phần tử $x = \sum_{i=1}^n \xi_i \varepsilon_i$ của V thuộc $L_2$ khi và chỉ khi
$$
2\xi_i \in \mathbf{Z}, \quad \xi_i - \xi_j \in \mathbf{Z} \text{ với mọi } i \text{ và } j.
$$
Vì $(\varepsilon_k | \frac{1}{2} \sum_{i=1}^n \varepsilon_i ) = \frac{1}{2}$ với mọi $k$, và vì $\| \frac{1}{2} \sum_{i=1}^n \varepsilon_i \| ^2 = \frac{n}{4}$, ta có $(\alpha|\beta) \in \frac{1}{2}\mathbf{Z}$ với $\alpha, \beta \in L_2$ nếu $n$ là chẵn. Nhóm $L_2/L_0$ đẳng cấu với $\mathbf{Z}/2\mathbf{Z}$.

4) $L_3 = L_1 + \mathbf{Z} (\frac{1}{2} \sum_{i=1}^n \varepsilon_i )$. Nếu $n$ là bội của 4, $L_3$ là tập hợp các $\sum_{i=1}^n \xi_i \varepsilon_i$ thỏa mãn (6) và điều kiện $\sum_{i=1}^n \xi_i \in 2\mathbf{Z}$: trong trường hợp này, $(\alpha|\beta) \in \mathbf{Z}$ với mọi $\alpha, \beta \in L_3$.

Rõ ràng ngay lập tức nhóm con của E liên kết với $L_0$ (tương ứng với $L_1, L_2$) là $L_0$ (tương ứng với $L_2, L_1$). Nhóm con của E liên kết với $L_3$ là tập hợp của

$$
x := \sum_{i=1}^n \xi_i \varepsilon_i \in L_2
$$

sao cho $(x| \frac{1}{2} \sum_{i=1}^n \varepsilon_i ) \in \mathbf{Z}$, nghĩa là, sao cho $\sum_{i=1}^n \xi_i \in 2\mathbf{Z}$: nếu $n \equiv 0 \pmod{4}$, nhóm con liên kết này do đó là $L_3$.

Nhóm Abel $L_2/L_1$ có cấp 4, và do đó đẳng cấu với $\mathbf{Z}/4\mathbf{Z}$ hoặc $\mathbf{Z}/2\mathbf{Z} \times \mathbf{Z}/2\mathbf{Z}$ (Đại số, Chương VII, § 4, no. 6, Định lý 3). Nếu $n$ là lẻ,

$$
p(\frac{1}{2} \sum_{i=1}^n \varepsilon_i ) \in L_1 \Leftrightarrow p \equiv 0 \pmod{4}
$$

nên $L_2/L_1$ là cyclic cấp 4. Nếu $n$ là chẵn,

$$
p(\frac{1}{2} \sum_{i=1}^n \varepsilon_i ) \in L_1 \Leftrightarrow p \equiv 0 \pmod{2}
$$

nên $L_2/L_1$, chứa hai phần tử phân biệt cấp 2, là đẳng cấu với $\mathbf{Z}/2\mathbf{Z} \times \mathbf{Z}/2\mathbf{Z}$.

Chúng ta sẽ dùng ký hiệu này trong suốt chín số tiếp theo và trong các bảng. Với mỗi kiểu đồ thị Dynkin trong Định lý 3, chúng ta sẽ mô tả tường minh:

(I) Một hệ nghiệm R và số nghiệm.
(II) Một cơ sở B của R, và các nghiệm dương tương ứng. Cơ sở B sẽ được đánh chỉ số bởi các số nguyên 1, ..., l.
(III) Số Coxeter h (§ 1, no. 11).
(IV) Nghiệm cao nhất $\tilde{\alpha}$ (đối với thứ tự được xác định bởi B) và đồ thị Dynkin hoàn chỉnh (no. 3). Chúng ta sẽ chỉ ra bên cạnh mỗi đỉnh nghiệm tương ứng của B.
(V) Hệ ngược $R^-$, dạng song tuyến tính chính tắc và hằng $\gamma(R)$ (§ 1, no. 12).
(VI) Các trọng số cơ bản đối với B (§ 1, no. 10).
(VII) Tổng các nghiệm dương.
(VIII) Các nhóm P(R), Q(R), P(R)/Q(R) và chỉ số liên kết (§ 1, no. 9).
(IX) Các số mũ của W(R) (Chương V, § 6, no. 2, Định nghĩa 2). Trong các trường hợp A_l, B_l, C_l và D_l chúng ta xác định các bất biến đối xứng.
(X) Cấp của W(R) (và trong một số trường hợp là cấu trúc của nó).

(XI) Nhóm $A(R)/W(R)$, tác động của nó trên đồ thị Dynkin, và phần tử $w_0$ của $W(R)$ biến đổi $B$ thành $-B$.

(XII) Tác động của $P(R^-)/Q(R^-)$ trên đồ thị Dynkin hoàn chỉnh và tác động của $A(R)/W(R)$ trên $P(R^-)/Q(R^-)$.

Đối với mỗi đồ thị Dynkin trong Định lý 3, các dữ liệu này sẽ được tập hợp trong các Bảng I đến IX, và được sắp xếp theo một cách thống nhất như trên. Chúng ta cũng cho:

(XIII) Ma trận Cartan, từ đó đồ thị Dynkin được dẫn xuất như đã mô tả trong no. 2.

### 5. CÁC HỆ KIỂU $B_l$ ($l \geq 2$)

(I) Ta xét nhóm $L_0$ trong $V = \mathbf{R}^l$ (no. 4). Gọi $R$ là tập hợp các $\alpha \in L_0$ sao cho $(\alpha|\alpha) = 1$ hoặc $(\alpha|\alpha) = 2$, nói cách khác là tập hợp các vectơ $\pm \varepsilon_i$ ($1 \leq i \leq l$) và $\pm \varepsilon_i \pm \varepsilon_j$ ($1 \leq i < j \leq l$). Rõ ràng rằng $R$ sinh ra $V$ và rằng $2(\alpha|\beta)/(\alpha|\alpha) \in \mathbf{Z}$ đối với mọi $\alpha, \beta \in R$. Vậy $R$ là một hệ nghiệm rút gọn trong $V$ (no. 4). Số nghiệm là $n = 2l + 4^{l(l-1)/2} = 2l^2$.

(II) Đặt

$$
\alpha_1 = \varepsilon_1 - \varepsilon_2,\ \alpha_2 = \varepsilon_2 - \varepsilon_3,\ldots,\alpha_{l-1} = \varepsilon_{l-1} - \varepsilon_1,\ \alpha_l = \varepsilon_l.
$$

Khi đó

$$
\varepsilon_i = \alpha_i + \alpha_{i+1} + \cdots + \alpha_l \quad (1 \leq i \leq l)
$$
$$
\varepsilon_i + \varepsilon_j = (\alpha_i + \alpha_{i+1} + \cdots + \alpha_l) + (\alpha_j + \alpha_{j+1} + \cdots + \alpha_l) \quad (1 \leq i < j \leq l)
$$
$$
\varepsilon_i - \varepsilon_j = \alpha_i + \alpha_{i+1} + \cdots + \alpha_{j-1} \quad (1 \leq i < j \leq l).
$$

Vì vậy $(\alpha_1, \alpha_2, \ldots, \alpha_l)$ là một cơ sở của $R$ (\S 1, no. 7, Hệ quả 3 của Mệnh đề 20). Hơn nữa, $\| \alpha_i \|^2 = 2$ với $i < l$, $\| \alpha_l \|^2 = 1$, $(\alpha_i|\alpha_{i+1}) = -1$ với $1 \leq i \leq l-1$, $(\alpha_i|\alpha_j) = 0$ với $j > i + 1$: đồ thị Dynkin của $R$ do đó có kiểu $B_l$, điều này chỉ ra rằng $R$ là bất khả quy. Các nghiệm dương là các $\varepsilon_i$ và các $\varepsilon_i \pm \varepsilon_j$ ($i < j$).

(III) Theo Định lý 1 (ii) của Chương V, \S 6, no. 2,

$$
h = n/l = 2l.
$$

(IV) Đặt $\tilde{\alpha} = \varepsilon_1 + \varepsilon_2 = \alpha_1 + 2\alpha_2 + 2\alpha_3 + \cdots + 2\alpha_l$, là một nghiệm. Tổng các tọa độ của nó đối với cơ sở $(\alpha_i)$ là $2l - 1 = h - 1$. Theo Mệnh đề 31 của \S 1, no. 11, $\tilde{\alpha}$ là nghiệm cao nhất của $R$. Ta có $(\tilde{\alpha}|\alpha_i) = 0$ với $i \neq 2$ và $(\tilde{\alpha}|\alpha_2) = 1$. Vì $\alpha_2$ có độ dài 1 (tương ứng $\sqrt{2}$) khi $l = 2$ (tương ứng $l \geq 3$), đồ thị Dynkin hoàn chỉnh của $R$ như sau:

với $l = 2$

$$
\begin{array}{c}
\alpha_2 \\
\alpha_1
\end{array}
$$

với $l \geq 3$

$$
\begin{array}{cccccc}
\alpha_1 & & & & & \\
& \alpha_2 & \alpha_3 & \cdots & \alpha_{l-1} & \alpha_l
\end{array}
$$

(V) Công thức $\alpha^- = \frac{2\alpha}{(\alpha|\alpha)}$ cho $R^-$ tập hợp các vectơ $\pm 2\varepsilon_i$ ($1 \leq i \leq l$), $\pm \varepsilon_i \pm \varepsilon_j$ ($1 \leq i < j \leq l$). Đồ thị Dynkin của $R^-$ thu được từ đồ thị của $R$ bằng quy trình được giải thích trong no. 2, và ta thấy rằng $R^-$ có kiểu $C_l$.

Có $4l - 2$ nghiệm không vuông góc với $\beta = \varepsilon_1$, cụ thể là $\pm \varepsilon_1$ và $\pm \varepsilon_1 \pm \varepsilon_j$ với $2 \leq j \leq l$; với mỗi nghiệm như vậy $\alpha$, $n(\alpha, \beta) = \pm 2$. Công thức (17) của § 1, no. 12 chỉ ra rằng, đối với $\Phi_R$, bình phương độ dài của $\beta$ là $(4l - 2)^{-1}$: do đó $\Phi_R(x, y) = (x|y)/(4l - 2)$. Áp dụng công thức (18) của § 1, no. 12 với $x = y = \beta$. Điều này cho
$$
2 + \frac{1}{4}(4l - 4) = \gamma(R) \frac{1}{4l - 2}
$$
và do đó $\gamma(R) = (l + 1)(4l - 2)$.

(VI) Các trọng số cơ bản $\omega_i$ ($1 \leq i \leq l$) sao cho $(\omega_i|\alpha_j) = \delta_{ij}$ được tính toán một cách dễ dàng, và ta tìm được rằng
$$
\begin{align*}
\omega_i &= \varepsilon_1 + \varepsilon_2 + \cdots + \varepsilon_i \\
&= \alpha_1 + 2\alpha_2 + \cdots + (i - 1)\alpha_{i-1} + i(\alpha_1 + \alpha_{i+1} + \cdots + \alpha_l) \quad (i < l) \\
\omega_l &= \frac{1}{2}(\varepsilon_1 + \varepsilon_2 + \cdots + \varepsilon_l) = \frac{1}{2}(\alpha_1 + 2\alpha_2 + \cdots + l\alpha_l).
\end{align*}
$$

(VII) Tổng của các nghiệm dương là
$$
\begin{align*}
2\rho &= (2l - 1)\varepsilon_1 + (2l - 3)\varepsilon_2 + \cdots + 3\varepsilon_{l-1} + \varepsilon_l \\
&= (2l - 1)\alpha_1 + 2(2l - 2)\alpha_2 + \cdots + i(2l - i)\alpha_i + \cdots + l^2\alpha_l.
\end{align*}
$$

(VIII) Ta có $Q(R) = L_0$ (no. 4), và $P(R)$ được sinh bởi $Q(R)$ và $\omega_l$, do đó bằng $L_2$ (no. 4). Vì vậy, $P(R)/Q(R)$ là đẳng cấu với $\mathbf{Z}/2\mathbf{Z}$, và chỉ số liên hệ bằng 2.

(IX) và (X) Trong $\mathbf{R}^l$, phép phản xạ trực giao $s_{\varepsilon_i, -\varepsilon_j}$ ($i \neq j$) hoán đổi $\varepsilon_i$ và $\varepsilon_j$ và giữ $\varepsilon_k$ bất biến khi chỉ số $k$ phân biệt với $i$ và $j$. Các $s_{\varepsilon_i, -\varepsilon_i}$ sinh ra một nhóm $G_1$ đẳng cấu với nhóm đối xứng $S_l$. Phép phản xạ trực giao $s_{\varepsilon_i}$ biến $\varepsilon_i$ thành $-\varepsilon_i$ và giữ bất biến các $\varepsilon_k$ khi chỉ số $k$ phân biệt với $i$. Các $s_{\varepsilon_i}$ sinh ra một nhóm $G_2$ đẳng cấu với $(\mathbf{Z}/2\mathbf{Z})^l$. Nhóm Weyl $W(R)$ được sinh bởi $G_1$ và $G_2$, và $G_2$ là chuẩn trong $W(R)$, do đó $W(R)$ đẳng cấu với tích nửa trực tiếp của $G_l$ bởi $(\mathbf{Z}/2\mathbf{Z})^l$. Cấp của nó do đó là $2^l.l!$.

Đại số đối xứng $S(\mathbf{R}^l)$ có thể được đồng nhất một cách chính tắc với đại số các hàm đa thức $P(\xi_1, \ldots, \xi_l)$ trên $\mathbf{R}^l$. Để một đa thức như vậy là bất biến dưới tác động của $W(R)$, trước hết cần thiết rằng
$$
P(\xi_1, \xi_2, \ldots, \xi_l) = P(\pm \xi_1, \pm \xi_2, \ldots, \pm \xi_l)
$$
với mọi cách chọn các dấu ở vế phải, sao cho
$$
P(\xi_1, \ldots, \xi_l) = Q(\xi_1^2, \ldots, \xi_l^2)
$$

trong đó Q là một đa thức, và thêm nữa Q là một đa thức đối xứng; và các điều kiện này là đủ. Do đó (Đại số. Chương V, Phụ lục I), $S(\mathbf{R}^l)^{W(R)}$ là đại số được sinh bởi các hàm đa thức thứ l

$$
t_i = \sum_{\tau \in S_l} \xi_{\tau(1)}^2 \xi_{\tau(2)}^2 \cdots \xi_{\tau(l)}^2 \quad (1 \leq i \leq l).
$$

Hơn nữa, bậc siêu việt trên $\mathbf{R}$ của trường các phân thức của $S(\mathbf{R}^l)^{W(R)}$ là l, do đó các $t_i$ độc lập đại số. Vì các $t_i$ có bậc 2, 4, ..., 2l, ta kết luận rằng các số mũ của W(R) (Chương V. § 6, no. 3, Mệnh đề 3) là:

$$ 1, 3, 5, \ldots, 2l - 1. $$

(XI) Tự đẳng cấu duy nhất của đồ thị Dynkin là phần tử đơn vị. Do đó, $A(R) = W(R)$ và $-1 \in W(R)$. Vì $-1$ biến B thành $-B$, ta kết luận rằng $w_0 = -1$.

(XII) Nhóm $P(R^-)/Q(R^-)$ là đối ngẫu với $P(R)/Q(R)$, và do đó đẳng cấu với $\mathbf{Z}/2\mathbf{Z}$. Phần tử không tầm thường của nó hoán vị các đỉnh tương ứng với $\alpha_0$ và $\alpha_1$ và giữ cố định các đỉnh còn lại.

### 6. CÁC HỆ KIỂU $C_l$ ($l \geq 2$)

(I) Sự tồn tại của các hệ nghiệm kiểu $C_l$ đã được chứng minh ở no. 5, vì ta đã thấy rằng hệ ngược của một hệ kiểu $B_l$ là kiểu $C_l$. Một hệ nghiệm kiểu $C_l$ do đó được thu được bằng cách lấy trong $\mathbf{R}'$ các vectơ $\pm 2\varepsilon_i$ ($1 \leq i \leq l$), và $\pm \varepsilon_i \pm \varepsilon_j$ ($1 \leq i < j \leq l$). Số nghiệm là $2l^2$.

(II) Một cơ sở của R có thể được thu được bằng cách lấy ảnh qua ánh xạ $\alpha \mapsto \frac{2\alpha}{(\alpha|\alpha)}$ của cơ sở của hệ xét ở no. 5. Ta thu được:

$$
\alpha_1 = \varepsilon_1 - \varepsilon_2, \quad \alpha_2 = \varepsilon_2 - \varepsilon_3, \ldots, \quad \alpha_{l-1} = \varepsilon_{l-1} - \varepsilon_l, \quad \alpha_l = 2\varepsilon_l.
$$

Các nghiệm dương là $2\varepsilon_i$ và $\varepsilon_i \pm \varepsilon_j$ ($i < j$).

(III) Số Coxeter là như đối với hệ ngược: $h = 2l$.

(IV) Cho $\tilde{\alpha} = 2\varepsilon_1 = 2\alpha_1 + 2\alpha_2 + \cdots + 2\alpha_{l-1} + \alpha_l$, là một nghiệm. Tổng các tọa độ của nó theo $(\alpha_i)$ là $2l - 1 = h - 1$. Vì thế, $\tilde{\alpha}$ là nghiệm cao nhất. Ta có $(\tilde{\alpha}|\alpha_i) = 0$ với $i \neq l$, $(\tilde{\alpha}|\alpha_l) = 2$. Do đó, đồ thị Dynkin mở rộng là

![Đồ thị Dynkin cho C_l](https://i.imgur.com/3Q5z5QG.png)

(V) Ta đã xác định $R^-$, vốn là kiểu $B_l$. Theo công thức (19) của § 1, no. 12 và theo no. 5 (V), bình phương độ dài của $2\varepsilon_i$ đối với $\Phi_R$ là

$$
((l+1)(4l-2))^{-1} ((4l-2)^{-1})^{-1} = (l+1)^{-1};
$$

do đó, $\Phi_R(x, y) = (x|y)/4(l+1)$.

Ta có $\gamma(R) = \gamma(R^-) = (l+1)(4l-2)$.

(VI) Các trọng số cơ bản dễ dàng tìm được:

$$
\omega_i = \varepsilon_1 + \varepsilon_2 + \cdots + \varepsilon_i
$$
$$
= \alpha_1 + 2\alpha_2 + \cdots + (i-1)\alpha_{i-1} + i(\alpha_i + \alpha_{i+1} + \cdots + \frac{1}{2}\alpha_l) \quad (i \leq l).
$$

(VII) Tổng các nghiệm dương là
$$
2\rho = 2l\varepsilon_1 + (2l-2)\varepsilon_2 + \cdots + 4\varepsilon_{l-1} + 2\varepsilon_l
$$
$$
= 2l\alpha_1 + 2(2l-1)\alpha_3 + \cdots + i(2l-i+1)\alpha_i + \cdots
$$
$$
\cdots + (l-1)(l+2)\alpha_{l-1} + \frac{1}{2}l(l+1)\alpha_l.
$$

(VIII) Theo no. 4 và no. 5 (VIII), $Q(R) = L_1, P(R) = L_0; P(R)/Q(R)$ đẳng cấu với $\mathbf{Z}/2\mathbf{Z}$, và chỉ số liên kết là 2.

(IX) và (X) Các dữ liệu này chỉ phụ thuộc vào $W(R)$, nên giống như đối với kiểu $B_l$.

(XI) Lập luận như ở no. 5 cho thấy $A(R) = W(R)$ và $w_0 = -1$.

(XII) Phần tử không phải phần tử đơn vị duy nhất của $P(R^-)/Q(R^-)$ xác định tự đẳng cấu không tầm thường duy nhất của đồ thị Dynkin mở rộng: nó hoán đổi các đỉnh tương ứng với $\alpha_j$ và $\alpha_{l-j}$ với $0 \leq j \leq l$.

### 7. CÁC HỆ KIỂU $A_l$ ($l \geq 1$)

(I) và (II) Cho $V$ là siêu phẳng trong $E = \mathbf{R}^{l+1}$ có phương trình $\sum\_{i=1}^{l+1} \xi\_i = 0$. Thay thế $l$ bởi $l+1$ trong no. 5, ta thu được một hệ $R'$ kiểu $B\_{l+1}$ trong $E$ với cơ sở
$$
\alpha\_1 = \varepsilon\_1 - \varepsilon\_2,\ \alpha\_2 = \varepsilon\_2 - \varepsilon\_3, \ldots, \alpha\_l = \varepsilon\_l - \varepsilon\_{l+1},\ \alpha\_{l+1} = \varepsilon\_{l+1}.
$$
Vì $\alpha\_1, \ldots, \alpha\_l$ sinh $V$, $R = R' \cap V$ là một hệ nghiệm trong $V$ với cơ sở $(\alpha\_1, \ldots, \alpha\_l)$ (\S 1, no. 7, Hệ quả 4 của Mệnh đề 20). Theo phép tính các tích vô hướng trong no. 5, ngay lập tức thấy rằng $R$ là kiểu $A\_l$. Các phần tử của $R$ là các $\varepsilon\_i - \varepsilon\_j$ ($i \neq j, 1 \leq i \leq l+1, 1 \leq j \leq l+1$). Có $n = l(l+1)$ nghiệm. Các nghiệm dương là các $\varepsilon\_i - \varepsilon\_j$ với $i < j$.

(III) Ta có $h = n/l = l+1$.

(IV) Đặt $\tilde{\alpha} = \varepsilon\_1 - \varepsilon\_{l+1} = \alpha\_1 + \alpha\_2 + \cdots + \alpha\_l$, đây là một nghiệm. Tổng các tọa độ của nó đối với $(\alpha\_i)$ là $l = h-1$. Do đó $\tilde{\alpha}$ là nghiệm cao nhất.
Với $l = 1$, $\tilde{\alpha} = \alpha\_1$ nên $(\tilde{\alpha}|\alpha\_1) = 2$; đồ thị Coxeter của nhóm $W\_a(R)$ là

$$
\begin{array}{c}
\infty \\\\
\alpha\_1
\end{array}
$$

Với $l \geq 2$. $(\tilde{\alpha}|\alpha\_i) = 0$ với $0 < i < l$ và $(\tilde{\alpha}|\alpha\_1) = (\tilde{\alpha}|\alpha\_l) = 1$. Do đó đồ thị Dynkin hoàn chỉnh là:

![Dynkin graph]$[https://i.imgur.com/3Q5z5QG.png](https://i.imgur.com/3Q5z5QG.png))

(V) Đồng nhất $V$ với đối ngẫu của nó bằng cách sử dụng tích vô hướng, ta có $\tilde{\alpha} = \frac{2\alpha}{(\alpha|\alpha)} = \alpha$ với mọi $\alpha \in \mathbf{R}$, do đó $R^\* = R$.

Đối với dạng $\Phi\_R$, độ dài của các nghiệm là $h^{-1/2} = (l+1)^{-1/2}$ (\S 1, no. 12); do đó $\Phi\_r(x, y) = (x|y)/2(l+1)$.

Ta có $\gamma(R) = (l+1)^2$ (\S 1, no. 12, công thức (20)).

(VI) Cho $(\omega\_i)\_{1 \leq i \leq l}$ là họ các trọng số cơ bản. Đặt

$$
\omega\_i = \sum\_{j=1}^{l+1} \xi\_{ij} \varepsilon\_j. \quad \text{với } \xi\_{ij} \in \mathbf{R}.
$$

Các điều kiện $(\omega\_i|\alpha\_j) = \delta\_{ij}$ và $\omega\_i \in V$ cho

$$
\xi\_{ii} - \xi\_{i,i+1} = 1, \quad \xi\_{ij} - \xi\_{i,j+1} = 0 \text{ với } j \neq i. \quad \sum\_{j=1}^{l+1} \xi\_{ij} = 0,
$$

dẫn dễ dàng đến

$$
\begin{align\*}
\omega\_i &= \varepsilon\_1 + \cdots + \varepsilon\_i - \frac{i}{l+1}(\varepsilon\_1 + \cdots + \varepsilon\_{l+1}) \\\\
&= \frac{1}{l+1}((l-i+1)(\alpha\_1 + 2\alpha\_2 + \cdots + (i-1)\alpha\_{i-1}) \\\\
&\qquad + i((l-i+1)\alpha\_i + (l-i)\alpha\_{i+1} + \cdots + \alpha\_l)).
\end{align\*}
$$

(VII) Tổng các nghiệm dương là

$$
\begin{align\*}
2\rho &= l\varepsilon\_1 + (l-2)\varepsilon\_2 + (l-4)\varepsilon\_3 + \cdots - (l-2)\varepsilon\_l - l\varepsilon\_{l+1} \\\\
&= l\alpha\_1 + 2(l-1)\alpha\_2 + \cdots + i(l-i+1)\alpha\_i + \cdots + l\alpha\_l.
\end{align\*}
$$

(VIII) Đưa vào $E = \mathbf{R}^{l+1}$ nhóm con $L\_0$ của no. 4. Gọi $p$ là phép chiếu trực giao của $E$ lên $V$. Theo \S 1, no. 10, Mệnh đề 28, ta có

$$
Q(R) = Q(R') \cap V \not\subset L\_0 \cap V, \quad \text{và} \quad P(R) = p(P(R'));
$$

do đó, vì trọng số cơ bản cuối cùng của $R'$ trực giao với $V$, ta có $P(R) = p(Q(R')) = p(L_0)$. Vì vậy, $P(R)$ là nhóm sinh bởi các $\varepsilon_i - \varepsilon_j$ và bởi $p(\varepsilon_1) = \varepsilon_1 - (l+1)^{-1} \sum_{i=1}^{l+1} \varepsilon_i$, nên

$$
P(R) = Q(R) + \mathbf{Z}(\varepsilon_1 - (l+1)^{-1} \sum_{i=1}^{l+1} \varepsilon_i).
$$

Bây giờ $l + 1$ là số nguyên nhỏ nhất $m > 0$ sao cho $mp(\varepsilon_1) \in Q(R)$. Do đó $P(R)/Q(R)$ đẳng cấu với $\mathbf{Z}/(l+1)\mathbf{Z}$ và chỉ số liên kết là $l + 1$.

(IX) và (X) Với mọi tự đẳng cấu $g$ của $V$, ký hiệu $\varphi(g)$ là tự đẳng cấu của $E$ mở rộng $g$ và giữ bất biến $\varepsilon_1 + \varepsilon_2 + \cdots + \varepsilon_l$. Nếu $g$ là phản xạ trực giao $s_{\varepsilon_i - \varepsilon_j}|V$, thì $\varphi(g)$ bằng $s_{\varepsilon_i - \varepsilon_j}$, tức là phép hoán vị $\varepsilon_i$ và $\varepsilon_j$ và giữ cố định các $\varepsilon_k$ với $k$ khác $i$ và $j$. Đặt

$$
X = \{\varepsilon_1, \varepsilon_2, \ldots, \varepsilon_{l+1}\}.
$$

Khi đó $g \mapsto \varphi(g)|X$ là một đẳng cấu từ $W(R)$ đến nhóm đối xứng của $X$. Vì vậy, $W(R)$ đẳng cấu với nhóm đối xứng $S_{l+1}$, nên có cấp $(l+1)!$.

Đại số đối xứng $S(E)$ có thể được đồng nhất một cách chính tắc với đại số các hàm đa thức $P(\xi_1, \xi_2, \ldots, \xi_{l+1})$ trên $E$. Đặt $G = \varphi(W(R))$. Theo đoạn trên, tập $S(E)^G$ gồm các phần tử của $S(E)$ bất biến dưới tác động của $G$ là tập các đa thức đối xứng (Đại số, Ch. V, App. I), và do đó (\emph{như trên}) là đại số sinh bởi các hàm

$$
s'_i = \sum_{\tau \in S_{l+1}} \xi_{\tau(1)} \xi_{\tau(2)} \cdots \xi_{\tau(i)} \quad (1 \leq i \leq l+1).
$$

Đại số $S(V)$ có thể được đồng nhất với các hạn chế lên $V$ của các hàm đa thức trên $E$. Nếu $P \in S(E)^G$, thì hạn chế của $P$ lên $V$ rõ ràng là bất biến dưới $W(R)$. Ngược lại, nếu $Q \in S(V)^{W(R)}$, tồn tại $P \in S(E)$ mở rộng $Q$; thay $P$ bởi $((l+1)!)^{-1} \sum_{g \in G} g(P)$, vốn có cùng hạn chế như $P$ lên $V$, ta có thể giả sử rằng $P \in S(E)^G$. Do đó, $S(V)^{W(R)}$ được sinh bởi các $s_i = s'_i|V$. Bây giờ $s_1 = 0$. Hơn nữa, bậc siêu việt trên $\mathbf{R}$ của trường phân thức của $S(V)^{W(R)}$ là $l$, nên các $s_i$ ($2 \leq i \leq l+1$) độc lập đại số. Vì các $s_i$ có bậc $2, 3, \ldots, l+1$, các số mũ của $W(R)$ là

$$
1, 2, 3, \ldots, l.
$$

(XI) Với $l = 1$, $A(R) = W(R) = \mathbf{Z}/2\mathbf{Z}$ và $w_0 = -1$.

Với $l \geq 2$, cho $\varepsilon \in A(R)$ là tự đẳng cấu biến $\alpha_i$ thành $\alpha_{l+1-i}$. Rõ ràng tự đẳng cấu cảm sinh bởi $\varepsilon$ là tự đẳng cấu không tầm thường duy nhất của đồ thị Dynkin. Nhóm $A(R)/W(R)$ đẳng cấu với $\mathbf{Z}/2\mathbf{Z}$. Vì $-1$ là một phần tử của $A(R)$ không thuộc $W(R)$ theo (IX) và (X), ta thấy rằng $A(R)$ đẳng cấu với $W(R) \times \mathbf{Z}/2\mathbf{Z}$. Ta có $w_0 = -\varepsilon$.

(XII) Nhóm $P(R^-)/Q(R^-)$ là nhóm cyclic cấp $l+1$ và tác động lên đồ thị Dynkin mở rộng bởi các hoán vị vòng tròn. Nếu $l \geq 2$, phần tử duy nhất khác phần tử đơn vị của $A(R)/W(R)$ tác động lên $P(R^-)/Q(R^-)$ bởi tự đẳng cấu $x \mapsto -x$.

### 8. HỆ THỐNG KIỂU $D_l$ ($l \geq 3$)

(I) Xét trong $V = \mathbf{R}'$ nhóm $L_0$ (no. 4). Tập hợp $R$ gồm các $\alpha \in L_0$ sao cho $(\alpha|\alpha) = 2$ là các vectơ $\pm \varepsilon_i \pm \varepsilon_j$ ($1 \leq i < j \leq l$). Rõ ràng $R$ sinh ra $V$ và $2(\alpha|\beta)/(\alpha|\alpha) \in \mathbf{Z}$ với mọi $\alpha, \beta \in R$. Do đó $R$ là một hệ căn rút gọn trong $V$ (no. 4). Số nghiệm là $n = 2l(l-1)$.

(II) Đặt

$$
\alpha_1 = \varepsilon_1 - \varepsilon_2,\ \alpha_2 = \varepsilon_2 - \varepsilon_3 \ldots \ldots \alpha_{l-1} = \varepsilon_{l-1} - \varepsilon_l,\ \alpha_l = \varepsilon_{l-1} + \varepsilon_l.
$$

Các công thức sau là hiển nhiên:

$$
\varepsilon_i - \varepsilon_j = \alpha_i + \alpha_{i+1} + \cdots + \alpha_{j-1}\quad (i < j)
$$
$$
\varepsilon_i + \varepsilon_j = \alpha_i + \alpha_{i+1} + \cdots + \alpha_{j-1} + 2\alpha_j + 2\alpha_{j+1} + \cdots
$$
$$
\cdots + 2\alpha_{l-2} + \alpha_{l-1} + \alpha_l\quad (i < j \leq l-2)
$$
$$
\varepsilon_i + \varepsilon_{l-1} = \alpha_i + \alpha_{i+1} + \cdots + \alpha_l\quad (i < l-1)
$$
$$
\varepsilon_i + \varepsilon_l = \alpha_i + \alpha_{i+1} + \cdots + \alpha_{l-2} + \alpha_l\quad (i < l-1)
$$
$$
\varepsilon_{l-1} + \varepsilon_l = \alpha_l.
$$

nên $(\alpha_1, \ldots, \alpha_l)$ là một cơ sở của $R$ (\S 1, no. 2, Hệ quả 3 của Mệnh đề 20). Hơn nữa, $\| \alpha_i \| ^2 = 2$ với mọi $i$. $(\alpha_i|\alpha_j) = 0$ với $i + 1 < j$ trừ trường hợp $i = l-2, j = l$ khi đó $(\alpha_{l-2}|\alpha_l) = -1$, $(\alpha_i|\alpha_{i+1}) = -1$ với $i \leq l-2$, và cuối cùng $(\alpha_{l-1}|\alpha_l) = -1$; do đó đồ thị Dynkin của $R$ là kiểu $D_l$. Các nghiệm dương là $\varepsilon_i \pm \varepsilon_j$ với $i < j$.

(III) Ta có $h = n/l = 2(l-1)$.

(IV) Cho $\tilde{\alpha} = \varepsilon_1 + \varepsilon_2 = \alpha_1 + 2\alpha_2 + \cdots + 2\alpha_{l-2} + \alpha_{l-1} + \alpha_l$, là một nghiệm. Tổng các tọa độ của nó theo $(\alpha_i)$ là

$$
2l-3 = h-1.
$$

Vậy $\tilde{\alpha}$ là nghiệm cao nhất.

Nếu $l = 3$, ta có

$$
(\tilde{\alpha}|\alpha_1) = 0,\quad (\tilde{\alpha}|\alpha_2) = (\tilde{\alpha}|\alpha_3) = 1.
$$

Nếu $l \geq 4$, ta có $(\tilde{\alpha}|\alpha_i) = 0$ với $i \neq 2$ và $(\tilde{\alpha}|\alpha_2) = 1$. Vì thế đồ thị Dynkin đầy đủ là:

![Dynkin graph for D_l](https://i.imgur.com/3Q5z5QG.png)

(V) Vì $(\alpha|\alpha) = 2$ với mọi $\alpha \notin R$, nên $R^- = R$.
Độ dài của các nghiệm của $\Phi_{L'}$ là $h^{-1/2} = (2l-2)^{-1/2}$. Do đó

$$
\Phi_R(x, y) = (x|y)/(4l-4)\quad \text{và}\quad \gamma(R) = 4(l-1)^2.
$$

(VI) Một phép tính tương tự như ở no. 7 cho các trọng số cơ bản:

$$
\omega_i = \varepsilon_1 + \varepsilon_2 + \cdots + \varepsilon_i \\
= \alpha_1 + 2\alpha_2 + \cdots + (i-1)\alpha_{i-1} + i(\alpha_i + \alpha_{i+1} + \cdots + \alpha_{l-2}) \\
\quad + \frac{1}{2}i(\alpha_{l-1} + \alpha_l)
$$

với $i < l - 1$,

$$
\omega_{l-1} = \frac{1}{2}(\varepsilon_1 + \varepsilon_2 + \cdots + \varepsilon_{l-2} + \varepsilon_{l-1} - \varepsilon_l) \\
= \frac{1}{2}(\alpha_1 + 2\alpha_2 + \cdots + (l-2)\alpha_{l-2} + \frac{1}{2}l\alpha_{l-1} + \frac{1}{2}(l-2)\alpha_l),
$$
$$
\omega_l = \frac{1}{2}(\varepsilon_1 + \varepsilon_2 + \cdots + \varepsilon_{l-2} + \varepsilon_{l-1} + \varepsilon_l) \\
= \frac{1}{2}(\alpha_1 + 2\alpha_2 + \cdots + (l-2)\alpha_{l-2} + \frac{1}{2}(l-2)\alpha_{l-1} + \frac{1}{2}l\alpha_l).
$$

(VII) Tổng các nghiệm dương là

$$
2\rho = 2(l-1)\varepsilon_1 + 2(l-2)\varepsilon_2 + \cdots + 2\varepsilon_{l-1} \\
= \sum_{i=1}^{l-2} 2(i(l-\frac{i(i+1)}{2}))\alpha_i + \frac{l(l-1)}{2}(\alpha_{l-1} + \alpha_l).
$$

(VIII) Các $\pm \varepsilon_i \pm \varepsilon_j$ sinh ra $L_1$ (no. 4), do đó $Q(R) = L_1$. Do đó $Q(R^*) = L_1$ và do đó $P(R) = L_2$ (no. 4). Theo no. 4, $P(R)/Q(R)$ đẳng cấu với $\mathbf{Z}/4\mathbf{Z}$ đối với $l$ lẻ, và với $\mathbf{Z}/2\mathbf{Z} \times \mathbf{Z}/2\mathbf{Z}$ đối với $l$ chẵn. Trong trường hợp thứ nhất, $P(R)/Q(R)$ được sinh bởi ảnh chính tắc của $\omega_l$ (và cũng bởi ảnh của $\omega_{l-1}$). Trong trường hợp thứ hai, $P(R)/Q(R)$ được sinh bởi các ảnh chính tắc của $\omega_{l-1}$ và $\omega_l$. Trong cả hai trường hợp chỉ số liên hệ là 4.

(IX) và (X) Trong $\mathbf{R}^l$, phép phản xạ trực giao $s_{\varepsilon_i, -\varepsilon_j}$ ($i \neq j$) hoán vị $\varepsilon_i$ và $\varepsilon_j$ và giữ bất biến các $\varepsilon_k$ với $k$ phân biệt với $i$ và $j$. Các $s_{\varepsilon_i, -\varepsilon_j}$ sinh ra một nhóm $G_1$ đẳng cấu với nhóm đối xứng $S_l$. Mặt khác, $s_{ij} = s_{\varepsilon_i, -\varepsilon_j} s_{\varepsilon_i, +\varepsilon_j}$ biến $\varepsilon_i$ thành $-\varepsilon_i$, $\varepsilon_j$ thành $-\varepsilon_j$ và giữ bất biến các $\varepsilon_k$ với $k$ phân biệt với $i$ và $j$. Các $s_{ij}$ sinh ra một nhóm $G_2$, là tập hợp các tự đẳng cấu $u$ của không gian vectơ $\mathbf{R}^l$ sao cho $u(\varepsilon_i) = (-1)^{\nu_i} \varepsilon_i$ với $\prod_{i=1}^l (-1)^{\nu_i} = 1$. Nhóm $G_2$ đẳng cấu với $(\mathbf{Z}/2\mathbf{Z})^{l-1}$, và $G_2$ là chuẩn tắc trong $W(R)$, nên $W(R)$ đẳng cấu với tích nửa trực tiếp của $S_l$ bởi $(\mathbf{Z}/2\mathbf{Z})^{l-1}$. Do đó, cấp của nó là $2^{l-1} l!$.

Các hàm đa thức $t_i$ của no. 5 là bất biến dưới $W(R)$, và $t = \xi_1 \xi_2 \ldots \xi_l$ cũng vậy; hơn nữa, $t_l = t^2$. Cho $P(\xi_1, \ldots, \xi_l)$ là một đa thức bất biến dưới $W(R)$. Cho $\xi_1^{\nu_1} \xi_2^{\nu_2} \ldots \xi_l^{\nu_l}$ là một đơn thức xuất hiện trong $P$ sao cho $\nu_i$ lẻ; khi đó $\nu_j$ là lẻ với mọi $j$ vì đơn thức $(-1)^{\nu_i + \nu_j} \xi_1^{\nu_1} \xi_2^{\nu_2} \ldots \xi_l^{\nu_l}$ xuất hiện trong $s_{ij}(P)$, nên $\nu_i + \nu_j \equiv 0 \pmod{2}$ và $\nu_j \equiv 1 \pmod{2}$. Do đó

P = P_1 + tP_2, trong đó mọi đơn thức xuất hiện trong P_1 và P_2 đều chỉ có số mũ chẵn. Vì P bất biến dưới các phép hoán vị của các $\xi_i$, nên P_1 và P_2 cũng có tính chất đó, và vì thế có thể viết dưới dạng các đa thức theo $t_1, t_2, \ldots, t_l$. Điều này chứng tỏ rằng đại số $S(\mathbf{R}^l)^{W(R)}$ được sinh bởi $t_1, t_2, \ldots, t_{l-1}, t$. Hơn nữa, bậc siêu việt của trường phân thức của $S(\mathbf{R}^l)^{W(R)}$ là l, nên $t_1, t_2, \ldots, t_{l-1}, t$ là độc lập đại số. Suy ra dãy số mũ, nếu sắp thứ tự thích hợp, là:

$$
1, 3, 5, \ldots, 2l - 5, 2l - 3, l - 1.
$$

Chú ý rằng $l - 1$ xuất hiện hai lần nếu $l$ chẵn, và một lần nếu $l$ lẻ.

(XI) Các tự đẳng cấu của đồ thị Dynkin chính là các tự đẳng cấu của đồ thị nền. Do đó:
1) Nếu $l = 3$, $A(R)/W(R)$ đẳng cấu với $\mathbf{Z}/2\mathbf{Z}$.
2) Nếu $l = 4$, mọi phép hoán vị của các đỉnh cuối xác định một tự đẳng cấu của đồ thị, nên $A(R)/W(R)$ đẳng cấu với $\mathfrak{S}_3$.
3) Nếu $l \geq 5$, các nhánh bắt đầu từ điểm phân nhánh có độ dài 1, 1, và $l - 3 \geq 2$. Tự đẳng cấu duy nhất của đồ thị khác với đồng nhất vì thế tương ứng với tự đẳng cấu $\varepsilon \in A(R)$, nó hoán đổi $\alpha_{l-1}$ và $\alpha_l$ và giữ cố định các $\alpha_i$ với $1 \leq i \leq l - 2$. Do đó $A(R)/W(R)$ đẳng cấu với $\mathbf{Z}/2\mathbf{Z}$; hơn nữa, $A(R)$ là tích nửa trực tiếp của nhóm $G_1 \cong \mathfrak{S}_l$ được xác định trong (IX) bởi nhóm $G_3$ gồm các tự đẳng cấu $u$ của $\mathbf{R}^l$ sao cho $u(\varepsilon_i) = \pm \varepsilon_i$ với mọi $i$.

Nếu $l$ chẵn, $-1 \in W(R)$, nên $w_0 = -1$. Nếu $l$ lẻ, $-1 \notin W(R)$, nên $A(R) = W(R) \times \{1, -1\}$ và $w_0 = -\varepsilon$.

(XII) Với $l$ chẵn, $P(R^-)/Q(R^-)$ có ba phần tử có cấp 2, cụ thể là $\omega_1, \omega_{l-1}$ và $\omega_l$. Vì $\omega_l$ (tương ứng $\omega_{l-1}$) hoán đổi các đỉnh tương ứng với $\alpha_0$ và $\alpha_l$ (tương ứng $\alpha_{l-1}$), nó hoán đổi các đỉnh tương ứng với $\alpha_1$ và $\alpha_{l-1}$ (tương ứng $\alpha_l$) và cũng hoán đổi các đỉnh tương ứng với $\alpha_j$ và $\alpha_{l-j}$ với

$$
2 \leq j \leq l - 2.
$$

Ta có $\omega_1 = \omega_l \omega_{l-1}$.

Với $l$ lẻ, $P(R^-)/Q(R^-)$ có hai phần tử có cấp 4, cụ thể là $\omega_{l-1}$ và $\omega_l$, và một phần tử có cấp 2, bằng $\omega_1$. Thật vậy, $\omega_1$ hoán đổi các đỉnh tương ứng với $\alpha_0$ và $\alpha_1$, nên nó giữ cố định các đỉnh tương ứng với $\alpha_j$ với $2 \leq j \leq l - 2$ và tất nhiên có cấp 2. Do đó $\omega_l$ có cấp 4 và biến đỉnh tương ứng với $\alpha_0$ (tương ứng $\alpha_l$, tương ứng $\alpha_1$, tương ứng $\alpha_{l-1}$) thành đỉnh tương ứng với $\alpha_l$ (tương ứng $\alpha_1$, tương ứng $\alpha_{l-1}$, tương ứng $\alpha_0$), và hoán đổi các đỉnh tương ứng với $\alpha_j$ và $\alpha_{l-j}$ với $2 \leq j \leq l - 2$. Ta có $\omega_1 = \omega_l^2$ và $\omega_{l-1} = \omega_l^3$.

Với $l \neq 4$, phần tử khác phần tử đơn vị của $A(R)/W(R)$ hoán đổi các đỉnh tương ứng với $\alpha_{l-1}$ và $\alpha_l$, và do đó hoán đổi các phần tử $\omega_{l-1}$ và $\omega_l$ của $P(R^-)/Q(R^-)$. Với $l$ lẻ, tự đẳng cấu của $P(R^-)/Q(R^-)$ thu được như vậy là ánh xạ $x \mapsto -x$.

Với $l = 4$, $A(R)/W(R)$ có thể được đồng nhất với nhóm các hoán vị của $\{1, 3, 4\}$ và tác động bằng các hoán vị của các chỉ số trên $\{\omega_1, \omega_3, \omega_4\}$.

### 9. HỆ THỐNG KIỂU $F_4$

(I) Xét nhóm $L_2$ (no. 4) trong $\mathbf{R}^4$. Cho $R$ là tập hợp các $\alpha \in L_2$ sao cho $(\alpha|\alpha) = 1$ hoặc $(\alpha|\alpha) = 2$; nó chứa các vectơ
$$
\pm \varepsilon_i,\quad \pm \varepsilon_i \pm \varepsilon_j\ (i < j),\quad \frac{1}{2}(\pm \varepsilon_1 \pm \varepsilon_2 \pm \varepsilon_3 \pm \varepsilon_4).
$$
Ngược lại, nếu $\alpha \in R$, các tọa độ của $\alpha$ chỉ có thể nhận các giá trị $0, \pm \frac{1}{2}, \pm 1$ (vì $(\frac{3}{2})^2 > 2$); hoặc các tọa độ này đều là số nguyên, cho các vectơ $\pm \varepsilon_i, \pm \varepsilon_i \pm \varepsilon_j$, hoặc chúng đều bằng $\pm \frac{1}{2}$, cho các vectơ $\frac{1}{2}(\pm \varepsilon_1 \pm \varepsilon_2 \pm \varepsilon_3 \pm \varepsilon_4)$.

Ta chứng minh rằng, với $\alpha, \beta \in R$, ta có $2(\alpha|\beta)/(|\alpha|\alpha) \in \mathbf{Z}$. Nếu $\alpha = \pm \varepsilon_i$ hoặc $\alpha = \frac{1}{2}(\pm \varepsilon_1 \pm \varepsilon_2 \pm \varepsilon_3 \pm \varepsilon_4)$, thì $(\alpha|\alpha) = 1$ và ta đã thấy ở no. 4 rằng $(\alpha|\beta) \in \frac{1}{2}\mathbf{Z}$ vì $\alpha, \beta \in L_2$. Nếu $\alpha = \pm \varepsilon_i \pm \varepsilon_j$, thì $(\alpha|\alpha) = 2$ và ta đã thấy ở no. 4 rằng $(\alpha|\beta) \in \mathbf{Z}$ vì $\alpha \in L_1$ và $\beta \in L_2$. Do đó, $R$ là một hệ căn rút gọn trong $\mathbf{R}^4$ (no. 4). Số các nghiệm là $n = 8 + \binom{4}{2} 4 + 2^4 = 48$.

(II) Hãy cho $\mathbf{R}^4$ thứ tự từ điển được xác định bởi cơ sở $(\varepsilon_1, \varepsilon_2, \varepsilon_3, \varepsilon_4)$ (§ 1, no. 7). Đặc biệt, ta có $\varepsilon_1 > \varepsilon_2 > \varepsilon_3 > \varepsilon_4$. Các nghiệm dương là
$$
\varepsilon_i,\quad \varepsilon_i \pm \varepsilon_j\ (i < j),\quad \frac{1}{2}(\varepsilon_1 \pm \varepsilon_2 \pm \varepsilon_3 \pm \varepsilon_4).
$$
Nghiệm nhỏ nhất là $\alpha_3 = \varepsilon_4$. Trong số các nghiệm thuộc $\mathbf{R}\varepsilon_3 + \mathbf{R}\varepsilon_4$ nhưng không thuộc $\mathbf{R}\varepsilon_4$, nghiệm nhỏ nhất là $\alpha_2 = \varepsilon_3 - \varepsilon_4$. Trong số các nghiệm dương thuộc $\mathbf{R}\varepsilon_2 + \mathbf{R}\varepsilon_3 + \mathbf{R}\varepsilon_4$ nhưng không thuộc $\mathbf{R}\varepsilon_3 + \mathbf{R}\varepsilon_4$, nghiệm nhỏ nhất là $\alpha_1 = \varepsilon_2 - \varepsilon_3$. Trong số các nghiệm dương không thuộc $\mathbf{R}\varepsilon_2 + \mathbf{R}\varepsilon_3 + \mathbf{R}\varepsilon_4$, nghiệm nhỏ nhất là $\alpha_4 = \frac{1}{2}(\varepsilon_1 - \varepsilon_2 - \varepsilon_3 - \varepsilon_4)$. Không một $\alpha_i$ nào là tổng của 2 nghiệm dương. Do đó, $(\alpha_1, \alpha_2, \alpha_3, \alpha_4)$ là một cơ sở của $R$ (§ 1, no. 6, Hệ quả 1 của Mệnh đề 19). Ta có $\| \alpha_1 \| = \| \alpha_2 \| = 2, \| \alpha_3 \| = \| \alpha_4 \| = 1, (\alpha_1|\alpha_2) = (\alpha_2|\alpha_3) = -1, (\alpha_3|\alpha_4) = -\frac{1}{2}, (\alpha_1|\alpha_3) = (\alpha_1|\alpha_4) = (\alpha_2|\alpha_4) = 0$. Ta thấy rằng đồ thị Dynkin của $R$ là kiểu $F_4$, và do đó là bất khả quy.

(III) Ta có $h = \frac{n}{l} = 12$.

(IV) Đặt $\tilde{\alpha} = \varepsilon_1 + \varepsilon_2 = 2\alpha_1 + 3\alpha_2 + 4\alpha_3 + 2\alpha_4$. Tổng các tọa độ của $\tilde{\alpha}$ theo $(\alpha_i)$ là $11 = h - 1$, nên $\tilde{\alpha}$ là nghiệm cao nhất. Ta có $(\tilde{\alpha}|\alpha_1) = 1, (\tilde{\alpha}|\alpha_2) = (\tilde{\alpha}|\alpha_3) = (\tilde{\alpha}|\alpha_4) = 0$.

Đồ thị Dynkin hoàn chỉnh là

![Dynkin graph of F_4](https://i.imgur.com/3Q5z5QG.png)

(V) Công thức $\alpha^* = \frac{2\alpha}{(\alpha|\alpha)}$ cho $R^-$ tập hợp các vectơ $\pm 2\varepsilon_i, \pm \varepsilon_i \pm \varepsilon_j, \pm \varepsilon_1 \pm \varepsilon_2 \pm \varepsilon_3 \pm \varepsilon_4$. Đồ thị Dynkin của $R^-$ thu được từ đồ thị của $R$ bằng thủ tục đã giải thích trong no. 2, và ta thấy rằng $R^-$ có kiểu $F_4$.

Các nghiệm không trực giao với $\beta = \varepsilon_1$ là $\pm \varepsilon_1, \pm \varepsilon_1 \pm \varepsilon_j \ (j \geq 2)$, và $\frac{1}{2}(\pm \varepsilon_1 \pm \varepsilon_2 \pm \varepsilon_3 \pm \varepsilon_4)$: số $n(\alpha|\beta) = 2(\alpha|\beta)$ bằng $\pm 2$ đối với 14 nghiệm đầu tiên trong các nghiệm này và bằng $\pm 1$ đối với 16 nghiệm cuối cùng; do đó, đối với $\Phi_R$, bình phương độ dài của $\beta$ là $4(14.4 + 16.1)^{-1} = \frac{1}{18}$; do đó

$$
\Phi_R(x, y) = \frac{(x|y)}{18}.
$$

Bây giờ ta áp dụng công thức (18) của § 1, no. 12, với $x = y = \beta$; điều này cho

$$
2 + 12.\frac{1}{4} + 16.\frac{1/4}{1} = \gamma(R).\frac{1}{18}
$$

suy ra

$$
\gamma(R) = 2.3^4.
$$

(VI) Việc tính các trọng số cơ bản cho

$$
\begin{align*}
\omega_1 &= \varepsilon_1 + \varepsilon_2 = 2\alpha_1 + 3\alpha_2 + 4\alpha_3 + 2\alpha_4 = \tilde{\alpha} \\
\omega_2 &= 2\varepsilon_1 + \varepsilon_2 + \varepsilon_3 = 3\alpha_1 + 6\alpha_2 + 8\alpha_3 + 4\alpha_4 \\
\omega_3 &= \frac{1}{2}(3\varepsilon_1 + \varepsilon_2 + \varepsilon_3 + \varepsilon_4) = 2\alpha_1 + 4\alpha_2 + 6\alpha_3 + 3\alpha_4 \\
\omega_4 &= \varepsilon_1 = \alpha_1 + 2\alpha_2 + 3\alpha_3 + 2\alpha_4.
\end{align*}
$$

(VII) Tổng các nghiệm dương là

$$
2\rho = 11\varepsilon_1 + 5\varepsilon_2 + 3\varepsilon_3 + \varepsilon_4 = 16\alpha_1 + 30\alpha_2 + 42\alpha_3 + 22\alpha_4.
$$

(VIII) Ta có $Q(R) = L_2$ (no. 4), và $P(R) = Q(R)$ theo (VI). Do đó, chỉ số liên kết bằng 1.

(IX) Họ các số mũ có 4 số hạng, và vì $h = 12$, nó phải chứa các số nguyên 1, 5, 7, 11, nguyên tố cùng nhau với 12 (\S 1, no. 11, Mệnh đề 30); do đó, đây là tất cả các số mũ của $W(R)$.

(X) và (XI) Tự đẳng cấu duy nhất của đồ thị Dynkin là tự đẳng cấu đồng nhất, do đó $A(R) = W(R)$ và $w_0 = -1$. Gọi $R'$ là tập hợp các phần tử dài nhất của $R$, tức là các $\pm \varepsilon_i \pm \varepsilon_j$; $R'$ là hệ nghiệm kiểu $D_4$ được xây dựng trong no. 8. Rõ ràng, mọi phần tử của $A(R)$ đều là một phần tử của $A(R')$. Ngược lại, một phần tử của $A(R')$ giữ $L_1$ ổn định (vì nó được sinh bởi $R'$), do đó cũng giữ $L_2$ liên kết của nó, và do đó cũng giữ $R$. Vậy $W(R) = A(R) = A(R')$. Theo no. 8, $W(R)$ là tích nửa trực tiếp của $S_3$ bởi $W(R')$, bản thân $W(R')$ là tích nửa trực tiếp của $S_4$ bởi $(\mathbf{Z}/2\mathbf{Z})^3$. Cấp của $W(R)$ là $3!4!2^3 = 2^7.3^2$.

### 10. HỆ KIỂU E_8

(I) Xét nhóm L_3 (no. 4) trong $\mathbf{R}^8$. Gọi R là tập hợp các $\alpha \in L_3$ sao cho $(\alpha|\alpha) = 2$; nó chứa các vectơ

$$
\pm \varepsilon_i \pm \varepsilon_j \quad (i < j), \quad \frac{1}{2} \sum_{i=1}^8 (-1)^{\nu(i)} \varepsilon_i \quad (\sum_{i=1}^8 \nu(i) \text{ chẵn}).
$$

Ngược lại, nếu một phần tử $\alpha \in L_3$ sao cho $(\alpha|\alpha) = 2$, các tọa độ của nó phải thuộc các giá trị $0, \pm \frac{1}{2}, \pm 1$: theo no. 4, hoặc các tọa độ này đều là số nguyên, cho các vectơ $\pm \varepsilon_i \pm \varepsilon_j$, hoặc chúng đều bằng $\pm \frac{1}{2}$ với một tổng nguyên, cho các vectơ

$$
\frac{1}{2} \sum_{i=1}^8 (-1)^{\nu(i)} \varepsilon_i
$$

với $\sum_{i=1}^8 \nu(i)$ chẵn.

Ta đã thấy (no. 4) rằng $(\alpha|\beta) \in \mathbf{Z}$ với mọi $\alpha, \beta \in L_3$. Do đó, R là một hệ căn rút gọn. Số các nghiệm là $n = \binom{8}{2} . 4 + 2^7 = 240$.

(II) Cho $\rho$ là vectơ $(0, 1, 2, 3, 4, 5, 6, 23)$ của $L_3$. Không có phần tử nào của R trực giao với $\rho$ (điều này hiển nhiên đối với các $\pm \varepsilon_i \pm \varepsilon_j$; nếu $\frac{1}{2} \sum_{i=1}^8 (-1)^{\nu(i)} \varepsilon_i$ trực giao với $\rho$, thì ta sẽ có $\sum_{i=1}^6 i(-1)^{\nu(i+1)} + 23(-1)^{\nu(8)} = 0$, điều này là không thể vì $\sum_{i=1}^6 i < 23$). Do đó (\S 1, no. 7, Hệ quả 2 của Mệnh đề 20) các $\alpha \in R$ sao cho $(\alpha|\rho) > 0$ là các nghiệm dương tương ứng với một chamber nào đó. Các nghiệm này là các $\pm \varepsilon_i + \varepsilon_j \ (i < j)$, và

$$
\frac{1}{2} (\varepsilon_8 + \sum_{i=1}^7 (-1)^{\nu(i)} \varepsilon_i)
$$

với $\sum_{i=1}^7 \nu(i)$ chẵn. Ta có $(\alpha|\rho) \in \mathbf{Z}$ với mọi $\alpha \in R$ (no. 4), và $(\alpha|\rho)$ bằng 1 đối với các nghiệm sau:

$$
\begin{align*}
\alpha_1 &= \frac{1}{2} (\varepsilon_1 + \varepsilon_8) - \frac{1}{2} (\varepsilon_2 + \varepsilon_3 + \varepsilon_4 + \varepsilon_5 + \varepsilon_6 + \varepsilon_7), \\
\alpha_2 &= \varepsilon_1 + \varepsilon_2, \ \alpha_3 = \varepsilon_2 - \varepsilon_1, \ \alpha_4 = \varepsilon_3 - \varepsilon_2, \ \alpha_5 = \varepsilon_4 - \varepsilon_3, \\
\alpha_6 &= \varepsilon_5 - \varepsilon_4, \ \alpha_7 = \varepsilon_6 - \varepsilon_5, \ \alpha_8 = \varepsilon_7 - \varepsilon_6.
\end{align*}
$$

và tám vectơ này tạo thành một cơ sở của $\mathbf{R}^8$. Theo \S 1, no. 6, Hệ quả 1 của Mệnh đề 19, $(\alpha_1, \alpha_2, \ldots, \alpha_8)$ là một cơ sở của R mà đối với đó các nghiệm dương là những nghiệm đã được định nghĩa ở trên. Ta có

$$
(\alpha_4|\alpha_5) = (\alpha_5|\alpha_6) = (\alpha_6|\alpha_7) = (\alpha_7|\alpha_8) = (\alpha_4|\alpha_2) = (\alpha_4|\alpha_3) = (\alpha_3|\alpha_1) = -1,
$$

và $(\alpha_i|\alpha_j) = 0$ với mọi cặp chỉ số khác. Do đó, đồ thị Dynkin của R thuộc kiểu E_8, và R là bất khả quy.

(III) Ta có $h = \frac{n}{8} = 30$.

(IV) Cho
$$
\tilde{\alpha} = \varepsilon_7 + \varepsilon_8 = 2\alpha_1 + 3\alpha_2 + 4\alpha_3 + 6\alpha_4 + 5\alpha_5 + 4\alpha_6 + 3\alpha_7 + 2\alpha_8,
$$
là một nghiệm. Tổng các tọa độ của nó theo $(\alpha_i)$ là $29 = h - 1$, nên $\tilde{\alpha}$ là nghiệm cao nhất. Nó trực giao với tất cả các $\alpha_i$ trừ $\alpha_8$, và $(\tilde{\alpha}|\alpha_8) = 1$. Do đó, đồ thị Dynkin hoàn chỉnh là:

![Đồ thị Dynkin của E_8](../images/dynkin_e8.png)

(V) Vì $(\alpha|\alpha) = 2$ với mọi $\alpha \in R$, ta có $R^- = R$.

Đối với $\Phi_R$, bình phương độ dài của các nghiệm là $\frac{1}{30}$ (\S 1, no. 12). Do đó, $\Phi_R(x, y) = (x|y)/60$ và $\gamma(R) = 900$ (\S 1. no. 12, công thức (20)).

(VI) Tính các trọng số cơ bản ta được
$$
\begin{align*}
\omega_1 &= 2\varepsilon_8 = 4\alpha_1 + 5\alpha_2 + 7\alpha_3 + 10\alpha_4 + 8\alpha_5 + 6\alpha_6 + 4\alpha_7 + 2\alpha_8 \\
\omega_2 &= \frac{1}{2}(\varepsilon_1 + \varepsilon_2 + \varepsilon_3 + \varepsilon_4 + \varepsilon_5 + \varepsilon_6 + \varepsilon_7 + 5\varepsilon_8) \\
&= 5\alpha_1 + 8\alpha_2 + 10\alpha_3 + 15\alpha_4 + 12\alpha_5 + 9\alpha_6 + 6\alpha_7 + 3\alpha_8 \\
\omega_3 &= \frac{1}{2}(-\varepsilon_1 + \varepsilon_2 + \varepsilon_3 + \varepsilon_4 + \varepsilon_5 + \varepsilon_6 + \varepsilon_7 + 7\varepsilon_8) \\
&= 7\alpha_1 + 10\alpha_2 + 14\alpha_3 + 20\alpha_4 + 16\alpha_5 + 12\alpha_6 + 8\alpha_7 + 4\alpha_8 \\
\omega_4 &= \varepsilon_3 + \varepsilon_4 + \varepsilon_5 + \varepsilon_6 + \varepsilon_7 + 5\varepsilon_8 \\
&= 10\alpha_1 + 15\alpha_2 + 20\alpha_3 + 30\alpha_4 + 24\alpha_5 + 18\alpha_6 + 12\alpha_7 + 6\alpha_8 \\
\omega_5 &= \varepsilon_4 + \varepsilon_5 + \varepsilon_6 + \varepsilon_7 + 4\varepsilon_8 \\
&= 8\alpha_1 + 12\alpha_2 + 16\alpha_3 + 24\alpha_4 + 20\alpha_5 + 15\alpha_6 + 10\alpha_7 + 5\alpha_8 \\
\omega_6 &= \varepsilon_5 + \varepsilon_6 + \varepsilon_7 + 3\varepsilon_8 \\
&= 6\alpha_1 + 9\alpha_2 + 12\alpha_3 + 18\alpha_4 + 15\alpha_5 + 12\alpha_6 + 8\alpha_7 + 4\alpha_8 \\
\omega_7 &= \varepsilon_6 + \varepsilon_7 + 2\varepsilon_8 \\
&= 4\alpha_1 + 6\alpha_2 + 8\alpha_3 + 2\alpha_4 + 10\alpha_5 + 8\alpha_6 + 6\alpha_7 + 3\alpha_8 \\
\omega_8 &= \varepsilon_7 + \varepsilon_8 \\
&= 5\alpha_1 + 8\alpha_2 + 10\alpha_3 + 15\alpha_4 + 12\alpha_5 + 9\alpha_6 + 6\alpha_7 + 3\alpha_8 = \tilde{\alpha}.
\end{align*}
$$

(VII) Nửa tổng các nghiệm dương bằng tổng các trọng số cơ bản (\S 1, no. 10, Mệnh đề 29); điều này cho
$$
\begin{align*}
\rho &= \varepsilon_2 + 2\varepsilon_3 + 3\varepsilon_4 + 4\varepsilon_5 + 5\varepsilon_6 + 6\varepsilon_7 + 23\varepsilon_8 \\
&= 46\alpha_1 + 68\alpha_2 + 91\alpha_3 + 135\alpha_4 + 110\alpha_5 + 84\alpha_6 + 57\alpha_7 + 29\alpha_8.
\end{align*}
$$

(VIII) Nhóm Q(R) được sinh bởi các $\varepsilon_i \pm \varepsilon_j$ và $\frac{1}{2} \sum_{i=1}^8 \varepsilon_i$, và bằng L_3 (no. 4). Do đó P(R), là nhóm liên kết với Q(R̄) = Q(R) = L_3, là L_3 (no. 4). Chỉ số liên kết là 1.

(IX) Họ các số mũ có 8 số hạng, và vì $h = 30$, các số nguyên 1, 7, 11, 13, 17, 19, 23, 29, nguyên tố cùng nhau với 30, phải có mặt trong họ này; do đó, đây là các số mũ của W(R).

(X) Từ (IX) và Chương V. § 6, no. 2, Hệ quả 1 của Mệnh đề 3, suy ra cấp của W(R) là

$$
2.8.12.14.18.20.24.30 = 2^{14}.3^5.5^2.7.
$$

(XI) Tự đẳng cấu duy nhất của đồ thị Dynkin là đồng nhất vì ba chuỗi xuất phát từ điểm phân nhánh có các độ dài phân biệt. Do đó, $A(R) = W(R)$ và $w_0 = -1$.

### 11. HỆ KIỂU E_7

(I) và (II) Cho $E = \mathbf{R}^8$, và cho R_8 là hệ nghiệm trong E được xây dựng ở no. 10. Cho V là siêu phẳng trong E được sinh bởi các nghiệm $\alpha_1, \ldots, \alpha_7$ của R_8; nó trực giao với trọng số cơ bản thứ tám $\omega = \varepsilon_7 + \varepsilon_8$ của R_8.

Cho $R = R\_8 \cap V$. Khi đó R là một hệ căn rút gọn với cơ sở $(\alpha\_1, \ldots, \alpha\_7)$, xem § 1, no. 7, Hệ quả 4 của Mệnh đề 20; do đó, hệ này có kiểu E\_7. Các phần tử của nó là:

$$
\pm \varepsilon\_i \pm \varepsilon\_j \quad (1 \leq i \leq j \leq 6), \quad \pm (\varepsilon\_7 - \varepsilon\_8),
$$
$$
\pm \frac{1}{2} (\varepsilon\_7 - \varepsilon\_8 + \sum\_{i=1}^8 (-1)^{\nu(i)} \varepsilon\_i) \quad \text{với } \sum\_{i=1}^8 \nu(i) \text{ lẻ}.
$$

Số các nghiệm là $n = 2 + \binom{6}{2}.4 + 2^6 = 126$. Các nghiệm dương là

$$
\pm \varepsilon\_i + \varepsilon\_j \quad (1 \leq i < j \leq 6), \quad -\varepsilon\_7 + \varepsilon\_8,
$$
$$
\frac{1}{2} (-\varepsilon\_7 + \varepsilon\_8 + \sum\_{i=1}^6 (-1)^{\nu(i)} \varepsilon\_i) \quad \text{với } \sum\_{i=1}^6 \nu(i) \text{ lẻ}.
$$

(III) Ta có $h = \frac{n}{l} = 18$.

(IV) Đặt $\tilde{\alpha} = \varepsilon\_8 - \varepsilon\_7 = 2\alpha\_1 + 2\alpha\_2 + 3\alpha\_3 + 4\alpha\_4 + 3\alpha\_5 + 2\alpha\_6 + \alpha\_7$, đó là một nghiệm. Tổng các tọa độ của nó đối với $(\alpha\_i)$ là 17 = $h - 1$. Vì vậy nó là nghiệm cao nhất. Nó trực giao với $\alpha\_i$ với $2 \leq i \leq 7$, và $(\tilde{\alpha}|\alpha\_1) = 1$. Đồ thị Dynkin hoàn chỉnh là

![Dynkin graph for E\_7]$[https://i.imgur.com/3Q5z5QG.png](https://i.imgur.com/3Q5z5QG.png)$

(V) Vì $(\alpha|\alpha) = 2$ với mọi $\alpha \in R$, ta có $R^- = R$.
Đối với $\Phi\_R$, bình phương độ dài của các nghiệm là $\frac{1}{18}$, nên
$$
\Phi\_R(x, y) = (x|y)/36, \quad \text{và} \quad \gamma(R) = 2^2 \cdot 3^4
$$
(§ 1. no. 12, công thức (20)).

(VI) Tính các trọng số cơ bản cho
$$
\begin{align\*}
\omega\_1 &= \varepsilon\_8 - \varepsilon\_7 = 2\alpha\_1 + 2\alpha\_2 + 3\alpha\_3 + 4\alpha\_4 + 3\alpha\_5 + 2\alpha\_6 + \alpha\_7 \\\\
\omega\_2 &= \frac{1}{2}(\varepsilon\_1 + \varepsilon\_2 + \varepsilon\_3 + \varepsilon\_4 + \varepsilon\_5 + \varepsilon\_6 - 2\varepsilon\_7 + 2\varepsilon\_8) \\\\
&= \frac{1}{2}(4\alpha\_1 + 7\alpha\_2 + 8\alpha\_3 + 12\alpha\_4 + 9\alpha\_5 + 8\alpha\_6 + 3\alpha\_7) \\\\
\omega\_3 &= \frac{1}{2}(-\varepsilon\_1 + \varepsilon\_2 + \varepsilon\_3 + \varepsilon\_4 + \varepsilon\_5 + \varepsilon\_6 - 3\varepsilon\_7 + 3\varepsilon\_8) \\\\
&= 3\alpha\_1 + 4\alpha\_2 + 6\alpha\_3 + 8\alpha\_4 + 6\alpha\_5 + 4\alpha\_6 + 2\alpha\_7 \\\\
\omega\_4 &= \varepsilon\_3 + \varepsilon\_4 + \varepsilon\_5 + \varepsilon\_6 + 2(\varepsilon\_8 - \varepsilon\_7) \\\\
&= 4\alpha\_1 + 6\alpha\_2 + 8\alpha\_3 + 12\alpha\_4 + 9\alpha\_5 + 6\alpha\_6 + 3\alpha\_7 \\\\
\omega\_5 &= \varepsilon\_4 + \varepsilon\_5 + \varepsilon\_6 + \frac{3}{2}(\varepsilon\_8 - \varepsilon\_7) \\\\
&= \frac{1}{2}(6\alpha\_1 + 9\alpha\_2 + 12\alpha\_3 + 18\alpha\_4 + 15\alpha\_5 + 10\alpha\_6 + 5\alpha\_7) \\\\
\omega\_6 &= \varepsilon\_5 + \varepsilon\_6 - \varepsilon\_7 + \varepsilon\_8 \\\\
&= 2\alpha\_1 + 3\alpha\_2 + 4\alpha\_3 + 6\alpha\_4 + 5\alpha\_5 + 4\alpha\_6 + 2\alpha\_7 \\\\
\omega\_7 &= \varepsilon\_6 + \frac{1}{2}(\varepsilon\_8 - \varepsilon\_7) \\\\
&= \frac{1}{2}(2\alpha\_1 + 3\alpha\_2 + 4\alpha\_3 + 6\alpha\_4 + 5\alpha\_5 + 4\alpha\_6 + 3\alpha\_7).
\end{align\*}
$$

### 12. HỆ KIỂU E_6

(I) và (II) Cho $E = \mathbf{R}^8$, và cho $R_8$ là hệ nghiệm trong $E$ được xây dựng ở no. 10. Cho $V$ là không gian con vectơ của $E$ sinh bởi các nghiệm $\alpha_1, \ldots, \alpha_6$ của $R_8$; đây là phần bù trực giao của mặt phẳng sinh bởi hai trọng số cơ bản cuối cùng $\omega = \varepsilon_7 + \varepsilon_8$ và $\pi = \varepsilon_6 + \varepsilon_7 + 2\varepsilon_8$ của $R_8$.

Đặt $R = R_8 \cap V$. Đây là một hệ căn rút gọn với cơ sở $(\alpha_1, \ldots, \alpha_6)$, và do đó có kiểu $E_6$. Các phần tử của nó là:

$$
\pm \varepsilon_i \pm \varepsilon_j \quad (1 \leq i < j \leq 5),
$$
$$
\pm \frac{1}{2} (\varepsilon_8 - \varepsilon_7 - \varepsilon_6 + \sum_{i=1}^5 (-1)^{\nu(i)} \varepsilon_i) \text{ với } \sum_{i=1}^5 \nu(i) \text{ chẵn}.
$$

Số các nghiệm là $n = \binom{5}{2}.4 + 2^5 = 72$. Các nghiệm dương là

$$
\pm \varepsilon_i + \varepsilon_j \quad (1 \leq i < j \leq 5),
$$
$$
\frac{1}{2} (\varepsilon_8 - \varepsilon_7 - \varepsilon_6 + \sum_{i=1}^5 (-1)^{\nu(i)} \varepsilon_i) \text{ với } \sum_{i=1}^5 \nu(i) \text{ chẵn}.
$$

(III) Ta có $h = \frac{n}{6} = 12$.

(IV) Đặt

$$
\tilde{\alpha} = \frac{1}{2} (\varepsilon_1 + \varepsilon_2 + \varepsilon_3 + \varepsilon_4 + \varepsilon_5 - \varepsilon_6 - \varepsilon_7 + \varepsilon_8)
$$
$$
= \alpha_1 + 2\alpha_2 + 2\alpha_3 + 3\alpha_4 + 2\alpha_5 + \alpha_6,
$$

là một nghiệm. Tổng các tọa độ của nó đối với $(\alpha_i)$ là $11 = h - 1$, do đó $\tilde{\alpha}$ là nghiệm cao nhất. Nó trực giao với $\alpha_1, \alpha_3, \alpha_4, \alpha_5, \alpha_6$, và $(\tilde{\alpha}|\alpha_2) = 1$. Đồ thị Dynkin hoàn chỉnh là

![Dynkin graph](../images/dynkin_graph.png)

(V) Vì $(\alpha|\alpha) = 2$ với mọi $\alpha \in R$, ta có $R' = R$. Đối với $\Phi_R$, bình phương độ dài của các nghiệm là $\frac{1}{12}$, nên
$$
\Phi_R(x, y) = (x|y)/24, \quad \text{và} \quad \gamma(R) = 144.
$$

(VI) Tính các trọng số cơ bản ta được:
$$
\begin{align*}
\omega_1 &= \frac{2}{3}(\varepsilon_8 - \varepsilon_7 - \varepsilon_6) = \frac{1}{3}(4\alpha_1 + 3\alpha_2 + 5\alpha_3 + 6\alpha_4 + 4\alpha_5 + 2\alpha_6) \\
\omega_2 &= \frac{1}{2}(\varepsilon_1 + \varepsilon_2 + \varepsilon_3 + \varepsilon_4 + \varepsilon_5 - \varepsilon_6 - \varepsilon_7 + \varepsilon_8) \\
&= \alpha_1 + 2\alpha_2 + 2\alpha_3 + 3\alpha_4 + 2\alpha_5 + \alpha_6 = \tilde{\alpha} \\
\omega_3 &= \frac{5}{6}(\varepsilon_8 - \varepsilon_7 - \varepsilon_6) + \frac{1}{2}(-\varepsilon_1 + \varepsilon_2 + \varepsilon_3 + \varepsilon_4 + \varepsilon_5) \\
&= \frac{1}{3}(5\alpha_1 + 6\alpha_2 + 10\alpha_3 + 12\alpha_4 + 8\alpha_5 + 4\alpha_6) \\
\omega_4 &= \varepsilon_3 + \varepsilon_4 + \varepsilon_5 - \varepsilon_6 - \varepsilon_7 + \varepsilon_8 \\
&= 2\alpha_1 + 3\alpha_2 + 4\alpha_3 + 6\alpha_4 + 4\alpha_5 + 2\alpha_6 \\
\omega_5 &= \frac{2}{3}(\varepsilon_8 - \varepsilon_7 - \varepsilon_6) + \varepsilon_4 + \varepsilon_5 \\
&= \frac{1}{3}(4\alpha_1 + 6\alpha_2 + 8\alpha_3 + 12\alpha_4 + 10\alpha_5 + 5\alpha_6) \\
\omega_6 &= \frac{1}{3}(\varepsilon_8 - \varepsilon_7 - \varepsilon_6) + \varepsilon_5 \\
&= \frac{1}{3}(2\alpha_1 + 3\alpha_2 + 4\alpha_3 + 6\alpha_4 + 5\alpha_5 + 4\alpha_6).
\end{align*}
$$

(VII) Nửa tổng các nghiệm dương là $\sum_{i=1}^6 \omega_i$, nên
$$
\begin{align*}
\rho &= \varepsilon_2 + 2\varepsilon_3 + 3\varepsilon_4 + 4\varepsilon_5 + 4(\varepsilon_8 - \varepsilon_7 - \varepsilon_6) \\
&= 8\alpha_1 + 11\alpha_2 + 15\alpha_3 + 21\alpha_4 + 15\alpha_5 + 8\alpha_6.
\end{align*}
$$

(VIII) Theo no. 10 (VIII) và § 4, no. 10, Mệnh đề 28,
$$
Q(R) = Q(R_8) \cap V = L_3 \cap V \quad \text{và} \quad P(R) = p(P(R_8)) = p(L_3),
$$

trong đó $p$ ký hiệu phép chiếu trực giao của $E$ lên $V$. Ta có
$$
p(\alpha_7) = \alpha_7 - \frac{2}{3}\pi + \omega, \quad p(\alpha_8) = \alpha_8 + \pi - 2\omega.
$$
Nhóm $Q(R)$ có cơ sở $(\alpha_1, \ldots, \alpha_6)$. Nhóm $P(R)$ được sinh bởi $Q(R)$ và $p(\alpha_7)$, vì $p(\alpha_8) \in P(R_8) \cap V = Q(R_8) \cap V = Q(R)$. Ta có $3p(\alpha_7) \in Q(R)$ và $p(\alpha_7) \notin Q(R)$. Do đó, nhóm $P(R)/Q(R)$ đẳng cấu với $\mathbf{Z}/3\mathbf{Z}$; nó được sinh, chẳng hạn, bởi ảnh của $\omega_6$.

Chỉ số liên kết là 3.

(IX) và (X) Theo § 2, no. 4, Mệnh đề 7, cấp của nhóm Weyl là $6!1.2.2.3.2.1.3 = 2^7.3^4.5$. Dãy các số mũ có 6 số hạng giữa 1 và 11, và chứa các số nguyên 1, 5, 7, 11 nguyên tố cùng nhau với 12. Các số mũ khác $m, m'$ là các số nguyên sao cho
$$
m + m' = 12,
$$
$$
(m + 1)(m' + 1)(1 + 1)(5 + 1)(7 + 1)(11 + 1) = 2^7.3^4.5,
$$
theo Chương V, § 6, no. 2, công thức (2) và Hệ quả 1 của Mệnh đề 3. Quan hệ thứ hai cho $(m + 1)(m' + 1) = 45$, và vì $m + m' + 2 = 14$, ta thu được $m = 4, m' = 8$. Do đó, dãy các số mũ là
$$
1, 4, 5, 7, 8, 11.
$$

(XI) và (XII) Vì tất cả các nghiệm đều có cùng độ dài, các tự đẳng cấu của đồ thị Dynkin là các tự đẳng cấu của đồ thị nền. Ngoài đồng nhất thức, chỉ có tự đẳng cấu $\varepsilon$ biến $\alpha_1, \alpha_3, \alpha_4, \alpha_5, \alpha_6, \alpha_2$ thành $\alpha_6, \alpha_5, \alpha_4, \alpha_3, \alpha_1, \alpha_2$, tương ứng. Do đó, $A(R)/W(R)$ đẳng cấu với $\mathbf{Z}/2\mathbf{Z}$; vì $-1 \in W(R)$ (Chương V, § 6, no. 2, Hệ quả 3 của Mệnh đề 3), $A(R)$ đẳng cấu với $W(R) \times \{1, -1\}$ và $w_0$ có thể được đồng nhất với $-\varepsilon$. Suy ra rằng phần tử khác đồng nhất của $A(R)/W(R)$ xác định tự đẳng cấu $x \mapsto -x$ của $P(R^-)/Q(R^-)$.

Hơn nữa, $P(R^-)/Q(R^-)$ có hai phần tử khác đồng nhất của cấp 3. Chúng xác định hai tự đẳng cấu cấp 3 của đồ thị Dynkin đã hoàn chỉnh.

### 13. HỆ KIỂU G_2

(I) Cho $E$ là siêu phẳng trong $\mathbf{R}^3$ có phương trình
$$
\xi_1 + \xi_2 + \xi_3 = 0.
$$
Cho $R$ là tập hợp các $\alpha \in L_0 \cap V$ sao cho $(\alpha|\alpha) = 2$ hoặc $(\alpha|\alpha) = 6$. Các phần tử của $R$ là
$$
\pm (\varepsilon_1 - \varepsilon_2), \quad \pm (\varepsilon_1 - \varepsilon_3), \quad \pm (\varepsilon_2 - \varepsilon_3), \quad \pm (2\varepsilon_1 - \varepsilon_2 - \varepsilon_3),
$$
$$
\pm (2\varepsilon_2 - \varepsilon_1 - \varepsilon_3), \quad \pm (2\varepsilon_3 - \varepsilon_1 - \varepsilon_2).
$$

Khi đó, R sinh ra V, và $\frac{2(\alpha|\beta)}{(\beta|\beta)} \in \mathbf{Z}$ với mọi $\alpha, \beta \in R$: điều này hiển nhiên nếu $\beta = \pm (\varepsilon_i - \varepsilon_j)$ với $i \neq j$; chẳng hạn nếu $\beta = 2\varepsilon_1 - \varepsilon_2 - \varepsilon_3$, ta có $(\alpha|\beta) \in 3\mathbf{Z}$, và một lần nữa mệnh đề của ta đúng. Do đó, R là một hệ căn rút gọn trong V. Số nghiệm là $n = 12$.

(II) Đặt $\alpha_1 = \varepsilon_1 - \varepsilon_2, \alpha_2 = -2\varepsilon_1 + \varepsilon_2 + \varepsilon_3$. Khi đó các nghiệm là

$$
\pm \alpha_1, \quad \pm (\alpha_1 + \alpha_2), \quad \pm (2\alpha_1 + \alpha_2), \quad \pm \alpha_2,
$$
$$
\pm (3\alpha_1 + \alpha_2), \quad \pm (3\alpha_1 + 2\alpha_2).
$$

Do đó, $(\alpha_1, \alpha_2)$ là một cơ sở của R. Ta có $\| \alpha_1 \| ^2 = 2, \| \alpha_2 \| ^2 = 6, (\alpha_1|\alpha_2) = -3$, nên R là một hệ kiểu G_2. Các nghiệm dương là $\alpha_1, \alpha_1 + \alpha_2, 2\alpha_1 + \alpha_2, 3\alpha_1 + \alpha_2, 3\alpha_1 + 2\alpha_2$.

(III) Ta có $h = \frac{n}{2} = 6$.

(IV) Nghiệm cao nhất là $\tilde{\alpha} = 3\alpha_1 + 2\alpha_2 = -\varepsilon_1 - \varepsilon_2 + 2\varepsilon_3$. Ta có $(\tilde{\alpha}|\alpha_1) = 0, (\tilde{\alpha}|\alpha_2) = 3$. Đồ thị Dynkin hoàn chỉnh là

![Dynkin graph](https://i.imgur.com/3Q5z5QG.png)

(V) Hệ ngược là tập các vectơ sau:

$$
\pm \alpha_1, \quad \pm (\alpha_1 + \alpha_2), \quad \pm (2\alpha_1 + \alpha_2), \quad \pm \frac{1}{3}\alpha_2,
$$
$$
\pm \frac{1}{3}(3\alpha_1 + \alpha_2), \quad \pm \frac{1}{3}(3\alpha_1 + 2\alpha_2).
$$

Có 10 nghiệm không trực giao với $\alpha_1$; ta có $n(\beta, \alpha_1) = \pm 1$ cho 4 nghiệm này, $n(\beta, \alpha_1) = \pm 3$ cho 4 nghiệm khác, và $n(\beta, \alpha_1) = \pm 2$ với $\beta = \pm \alpha_1$. Do đó, bình phương độ dài của $\alpha_1$ đối với $\Phi_R$ là $4(4.1 + 4.9 + 2.4)^{-1} = \frac{1}{12}$. Vì thế, $\Phi_R(x, y) = (x|y)/24$. Ta áp dụng công thức (18) của § 1, no. 12, với $x = y = \alpha_1$; điều này cho

$$
2 + 4.\frac{1}{4} + 4.\frac{1}{4} = \gamma(R).\frac{1}{12}
$$

nên $\gamma(R) = 48$.

(VI) và (VII) Nửa tổng của các nghiệm dương là

$$
\rho = 5\alpha_1 + 3\alpha_2.
$$

Các trọng số cơ bản $\omega_1$ và $\omega_2$ trực giao với $\alpha_2$ và $\alpha_1$, do đó tỷ lệ với $2\alpha_1 + \alpha_2$ và $3\alpha_1 + 2\alpha_2$. Ta có

$$
\omega_1 + \omega_2 = \rho = 5\alpha_1 + 3\alpha_2 = (2\alpha_1 + \alpha_2) + (3\alpha_1 + 2\alpha_2).
$$

Do đó,

$$
\omega_1 = 2\alpha_1 + \alpha_2, \quad \omega_2 = 3\alpha_1 + 2\alpha_2 = \tilde{\alpha}.
$$

(VIII) Q(R) được sinh bởi $\varepsilon_1 - \varepsilon_2$ và $\varepsilon_1 - \varepsilon_3$, chẳng hạn. Theo (VI) và (VII), P(R) = Q(R). Chỉ số liên kết là 1.

(IX) Họ các số mũ có 2 số hạng; vì 1 và $h - 1 = 5$ là các số mũ, nên chúng là những số duy nhất.

(X) Ta có $(\overline{\alpha_1, \alpha_2}) = \frac{5\pi}{6}$, do đó W(R) đẳng cấu với nhóm nhị diện cấp 12.

(XI) Tự đẳng cấu duy nhất của biểu đồ Dynkin là tự đẳng cấu đồng nhất, do đó $\Lambda(R) = W(R)$ và $w_0 = -1$.

### 14. HỆ NGHIỆM BẤT KHẢ QUY KHÔNG RÚT GỌN

Các hệ nghiệm bất khả quy, không rút gọn có thể thu được từ các hệ nghiệm rút gọn bất khả quy bằng cách sử dụng các Mệnh đề 13 và 14 của § 1. no. 4. Với mỗi số nguyên $l \geq 1$, tồn tại, sai khác một đẳng cấu, một hệ nghiệm bất khả quy, không rút gọn duy nhất có hạng $l$: cho R là một hệ nghiệm kiểu B_l, A là tập hợp các nghiệm ngắn nhất của R; lấy hợp của R và 2A. Với ký hiệu của no. 5, ta thu được các vectơ $2l(l+1)$

$$
\pm \varepsilon_i,\ \pm 2\varepsilon_i,\ \varepsilon_i \pm \varepsilon_j\ (i < j).
$$

### Bài tập {#lie-vi-s4-exercises}

Nếu R là một hệ nghiệm, ký hiệu bằng $W^+(R)$ tập hợp các phần tử của $W(R)$ có định thức bằng 1.

Xem [các bài tập của § 4](exercises/s4/).
