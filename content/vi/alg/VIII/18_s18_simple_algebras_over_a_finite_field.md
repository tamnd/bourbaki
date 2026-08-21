---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Semisimple Modules and Rings
section: 18
section_title: Simple Algebras over a Finite Field
lang: vi
source: alg-viii
source_edition: 2023, Springer Nature
book_pages: A VIII.355-A VIII.360
pdf_pages: 0372-0377
extraction: native
subsections:
    - "no": 1
      title: Polynomials over a Finite Field
      page: 355
      pdf_page: 372
    - "no": 2
      title: Simple Algebras over Finite Fields
      page: 357
      pdf_page: 374
statements: 10
exercises: 7
content_sha256: d247b5e5825cd5cd407b4c953f1781acd2ae274bb01d96d1efb5cc14a684e550
translated_from: content/en/alg/VIII/18_s18_simple_algebras_over_a_finite_field.md
source_content_sha256: 2e54129261e2cf9cc0935b1e6d5d3d389efce06f1bc5f48edb1e9227a40ce254
translation_model: gpt-5.4
translation_run: translate-vi-74c08a00
glossary_version: 34
glossary_terms_sha256: 320974a7c223d0597926f2b2a86d1849a2adfd5725a5804dda4858d081e6e2a9
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 18. ĐẠI SỐ ĐƠN TRÊN MỘT TRƯỜNG HỮU HẠN

### 1. Các đa thức trên một trường hữu hạn

#### Định lý 1 (Chevalley–Warning) {#alg-viii-s18-thm-1 .statement tag=00SA}

Cho K là một trường giao hoán hữu hạn có đặc số $p$. Cho $n$ là một số nguyên $\geqslant 1$ và $(f_i)_{i\in I}$ là một họ hữu hạn các phần tử khác không của $K[X_1, . . . ,X_n]$. Ký hiệu Z là tập hợp các phần tử $\mathbf{x}$ của $K^n$ sao cho ta có $f_i(\mathbf{x}) = 0$ với mọi $i\in I$. Nếu ta có $n >\sum_{i\in I}$ deg($f_i$), thì lực lượng của Z chia được cho $p$.

#### Bổ đề 1 {#alg-viii-s18-lem-1 .statement tag=00LB}

Cho L là một trường, G là một nhóm hữu hạn, và $\chi$ là một đồng cấu không tầm thường từ G vào nhóm nhân $L^*$. Ta có $\sum_{x\in G}\chi (x) = 0$.

Theo giả thiết, tồn tại một phần tử $a$ của G sao cho $\chi (a)\not= 1$; vì phép nhân bởi $a$ là một phép hoán vị của G, ta có

$$
\sum_{x\in G}\chi (x) =\sum_{x\in G}\chi (ax) =\chi (a)\sum_{x\in G}\chi (x)
$$

điều này cho Bổ đề 1.

#### Bổ đề 2 {#alg-viii-s18-lem-2 .statement tag=00LC}

Gọi $q$ là lực lượng của K. Với mọi số nguyên $m\geqslant 0$, đặt $S_m=$ $\sum_{x\in K}x^m$. Ta có $S_m=-1$ nếu $m$ là một bội khác không của $q-1$ và $S_m= 0$ trong mọi trường hợp khác.

Nhớ rằng $0^0= 1$ (I, §2, No. 1, p. 14). Giả sử rằng $m$ là một bội của $q-1$. Vì nhóm Abel $K^*$ có cấp $q-1$, ta có $x^m= 1$ với mọi $x\in K^*$ và $S_m= 0^m+ (q-1)\cdot 1$, điều này cho mệnh đề trong trường hợp này.

Giả sử rằng $m$ không phải là một bội của $q-1$. Đặt $\chi (x) =x^m$ với $x\in K^*$. Vì nhóm nhân $K^*$ là cyclic cấp $q-1$ (V, §12, No. 1, p. 93, Mệnh đề 1), nên tồn tại một phần tử $a$ của $K^*$ sao cho $\chi (a)\not= 1$. Theo Bổ đề 1 áp dụng cho $G = K^*$, ta có

$$
S_m= 0^m+\sum_{x\in K^*}\chi (x) = 0
$$

điều này cho Bổ đề 2.

Bây giờ chúng ta chứng minh Định lý 1. Cho $\mathbf{x}= (x_1, . . . , x_n)$ là một phần tử của $K^n$. Ta có $1-f_i(\mathbf{x})^{q-1}= 0$ nếu $f_i(\mathbf{x})\not= 0$ và $1-f_i(\mathbf{x})^{q-1}= 1$ nếu $f_i(\mathbf{x}) = 0$. Đặt $P =\prod^r_{i=1}(1-f_i^{q-1})$. Ta có

1 nếu $\mathbf{x}\in Z$,

$$
P(\mathbf{x}) = \tag{1}
$$

0 nếu $\mathbf{x}\notin Z$.

Khai triển đa thức P thành $\sum_{\alpha\in\mathbf{N}^n}c_{\alpha}X^{\alpha}$; theo giả thiết, nó có bậc $<(q-1)n$. Gọi $\alpha$ là một phần tử của $\mathbf{N}^n$ sao cho $c_{\alpha}$ khác không. Vì ta có $\alpha_1+\cdots +\alpha_n<(q-1)n$, nên tồn tại một số nguyên $\ell$ sao cho $1\leqslant \ell \leqslant n$ và $0\leqslant \alpha_{\ell}< q-1$. Theo Bổ đề 2, khi đó ta có $\sum_{x\in K}x^{\alpha_{\ell}}= 0$, và do đó

$$
\sum_{\mathbf{x}\in K^n}\mathbf{x}^{\alpha}=\prod_{j=1}^n((\sum_{x\in K}x^{\alpha_j})= 0
$$

Do đó ta có

$$
\sum_{\mathbf{x}\in K^n}P(\mathbf{x}) =\sum_{\alpha\in\mathbf{N}^n}c_{\alpha}((\sum_{\mathbf{x}\in K^n}\mathbf{x}^{\alpha})= 0
$$

Bây giờ, theo công thức (1), ta có $\sum_{\mathbf{x}\in K^n}P(\mathbf{x}) =$ Card(Z) $\cdot 1$, và do đó Card(Z) $\cdot 1 = 0$, điều đó có nghĩa là Card(Z) chia hết cho $p$.

#### Hệ quả {#alg-viii-s18-n1-cor-1 .statement tag=00LD}

Cho V là một không gian vectơ có số chiều hữu hạn $n$ trên K và I là một tập hợp hữu hạn, và với mỗi $i\in I$, cho $F_i: V\rightarrow K$ là một ánh xạ đa thức thuần nhất bậc $d_i>0$. Nếu ta có $\sum_{i\in I}d_i< n$, thì tồn tại một phần tử khác không $x$ của V sao cho $F_i(x) = 0$ với mọi $i\in I$.

Cho $(e_1, . . . , e_n)$ là một cơ sở của V trên K. Theo định nghĩa của các ánh xạ đa thức thuần nhất (IV, §5, No. 9, p. 55, Định nghĩa 3), với mọi $i\in I$, tồn tại một đa thức thuần nhất $f_i$ trong $K[X_1, . . . ,X_n]$ bậc $d_i$ sao cho ta có $F_i(\xi_1e_1, . . . , \xi_ne_n) =f_i(\xi_1, . . . , \xi_n)$. Gọi Z là tập hợp các phần tử $x$ của V sao cho $F_i(x) = 0$ với mọi $i\in I$. Theo Định lý 1, lực lượng của Z chia hết cho $p$, và vì 0 thuộc S, ta có Card(Z) $\geqslant p >1$.

### 2. Đại số đơn trên trường hữu hạn

#### Định lý 2 (Wedderburn) {#alg-viii-s18-thm-2 .statement tag=00SB}

Mọi trường hữu hạn đều giao hoán.

Cho D là một trường hữu hạn, và gọi K là tâm của nó. K-đại số D là đơn tâm bậc $m^2$, trong đó $m$ là một số nguyên dương ngặt. Chuẩn rút gọn là một ánh xạ đa thức thuần nhất Nrd$: D\rightarrow K$ bậc $m$ (VIII, p. 345, Mệnh đề 6), và ta có Nrd($a$)$\not= 0$ với mọi $a\not= 0$ trong D (VIII, p. 340, Mệnh đề 3). Hệ quả trên suy ra rằng $m\geqslant m^2$, và do đó $m= 1$. Vậy ta có D = K.

#### Hệ quả 1 {#alg-viii-s18-thm-2-cor-1 .statement tag=00LE}

Mọi vành đơn hữu hạn đều đẳng cấu với một vành ma trận $\mathbf{M}_n(L)$, trong đó $n$ là một số nguyên dương ngặt và L là một trường giao hoán hữu hạn.

Điều này suy ra từ Định lý 2 và định lý cấu trúc của các vành đơn (VIII, p. 120, Định lý 1).

#### Hệ quả 2 {#alg-viii-s18-thm-2-cor-2 .statement tag=00LF}

Cho K là một trường giao hoán hữu hạn. Mọi đại số đơn tâm trên K đều đẳng cấu với một đại số ma trận $\mathbf{M}_n(K)$, trong đó $n$ là một số nguyên dương ngặt.

Điều này suy ra từ Định lý 2 và định lý cấu trúc của các đại số đơn tâm (VIII, p. 252, Định lý 1).

#### Nhận xét 1 {#alg-viii-s18-n2-rem-1 .statement tag=00LG}

Đây là một chứng minh khác của Định lý 2. Cho D là một trường hữu hạn, K là tâm của nó, và L là một trường con giao hoán cực đại của D. Cho $x$ là một phần tử của $D^*$. Nó thuộc về một trường con giao hoán cực đại $L_1$ của D. Ta có đẳng thức

$$
[D : K] = [L : K]^2= [L_1: K]^2
$$

theo Hệ quả 2 của VIII, p. 265, và do đó $[L : K] = [L_1: K]$. Theo Mệnh đề 3 của V, §12, No. 2, p. 94, các mở rộng L và $L_1$ của K là đẳng cấu. Theo VIII, p. 263, Hệ quả, tồn tại một phần tử $a$ của $D^*$ sao cho $aLa^{-1}= L_1$, nên $a^{-1}xa$ thuộc về L. Khi đó ta có $(ay)^{-1}x(ay) =a^{-1}xa$ với mọi $y\in L^*$. Do đó, nếu S là một tập hợp các đại biểu của các lớp kề trái của $D^*$ theo modulo $L^*$, thì mọi phần tử của $D^*-\{1\}$ đều có thể viết dưới dạng $sxs^{-1}$ với $s\in S$ và $x\in L^*-\{1\}$. Ta ký hiệu cấp của $D^*$ là $d$ và cấp của $L^*$ là $\ell$. Vì lực lượng của S bằng $d/\ell$, ta có $d-1\leqslant (d/\ell )(\ell -1) =d-d/\ell$. Suy ra $\ell =d$, và do đó L = D, điều này chứng minh rằng trường D là giao hoán.

#### Nhận xét 2 {#alg-viii-s18-n2-rem-2 .statement tag=00LH}

Cho L là một trường giao hoán có tính chất sau: $(C_1)$ Cho V là một không gian vectơ có số chiều hữu hạn $n$ trên trường L, và cho $d$ sao cho $0< d < n$. Với mọi ánh xạ đa thức thuần nhất $F : V\rightarrow L$ bậc $d$, tồn tại một phần tử khác không $x$ của V sao cho $F(x) = 0$.

Chứng minh của Định lý 2 cho thấy rằng mọi trường bậc hữu hạn trên L có tâm L đều bằng L.

Theo hệ quả ở VIII, p. 356, mọi trường hữu hạn đều có tính chất $(C_1)$. Có thể chứng minh (VIII, p. 360, Bài tập 7) rằng các trường sau đây có tính chất $(C_1):$

– mọi mở rộng đại số của một trường hữu hạn

– mọi trường phân thức hữu tỉ theo một biến với hệ số trong một trường đóng đại số (định lý Tsen).

– $*$mọi trường được trang bị một định giá rời rạc mà đối với nó trường đó là đầy đủ và

trường thặng dư của nó là đóng đại số (VIII, p. 332, Bài tập 17)$.*$

#### Nhận xét 3 {#alg-viii-s18-n2-rem-3 .statement tag=00LI}

Giả sử rằng trường K thỏa mãn điều kiện sau:

– Nếu L là một mở rộng của K bậc hữu hạn, thì nó là cyclic và ánh xạ chuẩn $N : L^*\rightarrow K^*$ là toàn ánh.

Điều kiện này được thỏa mãn, đặc biệt, khi trường K là hữu hạn (V, §12, No. 2, p. 95, Mệnh đề 4). Khi đó có thể chứng minh rằng mọi trường bậc hữu hạn trên K có tâm K đều bằng K (Bài tập 10 của VIII, p. 329).

### Bài tập {#alg-viii-s18-exercises}

Xem [các bài tập của § 18](exercises/s18/).
