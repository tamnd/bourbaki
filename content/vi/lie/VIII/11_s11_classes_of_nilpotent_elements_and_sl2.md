---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: VIII
chapter_title: SPLIT SEMI-SIMPLE LIE ALGEBRAS
section: 11
section_title: Classes of nilpotent elements and sl2 -triplets
lang: vi
source: lie-vii-ix
book_pages: 163-173, 261-266
pdf_pages: 0171-0181, 0269-0274
extraction: native+ocr
subsections:
    - "no": 1
      title: DEFINITION OF $\mathfrak{s}\mathfrak{l}_{2}$-TRIPLETS
      page: 163
      pdf_page: 171
    - "no": 2
      title: $\mathfrak{s}\mathfrak{l}_{2}$-TRIPLETS IN SEMI-SIMPLE LIE ALGEBRAS
      page: 165
      pdf_page: 173
    - "no": 3
      title: SIMPLE ELEMENTS
      page: 167
      pdf_page: 175
    - "no": 4
      title: PRINCIPAL ELEMENTS
      page: 170
      pdf_page: 178
statements: 29
exercises: 17
content_sha256: 2d1655b50e3ffca496fba47f2e3af587ad4c6af0fe887d6620c70d075c6aa12e
translated_from: content/en/lie/VIII/11_s11_classes_of_nilpotent_elements_and_sl2.md
source_content_sha256: 9fa596e246cac621b5b9e0b269c472085fd46db9e470656f32a0223db1df02b5
translation_model: gpt-5.4
translation_run: translate-vi-7ef3e28e
glossary_version: 34
glossary_terms_sha256: ae1b318548eb87c2bf54b111e901e40124c8df2d182bfaac1333c2e4b046b8c6
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 11. CÁC LỚP PHẦN TỬ LŨY LINH VÀ CÁC BỘ BA $\mathfrak{s}\mathfrak{l}_{2}$

Trong đoạn này, $\mathfrak{g}$ kí hiệu một đại số Lie hữu hạn chiều.

### 1. ĐỊNH NGHĨA CÁC BỘ BA $\mathfrak{s}\mathfrak{l}_{2}$

#### Định nghĩa 1 {#lie-viii-s11-def-1 .statement tag=0170}

Một bộ ba $\mathfrak{s}\mathfrak{l}_2$ trong $\mathfrak{g}$ là một dãy $(x, h, y)$ các phần tử của $\mathfrak{g}$, phân biệt với $(0,0,0)$, sao cho

$$
[h, x] = 2x,[h, y] =-2y,[x, y] =-h
$$

Cho $(x, h, y)$ là một bộ ba $\mathfrak{s}\mathfrak{l}_2$ trong $\mathfrak{g}$. Ánh xạ tuyến tính $\tau$ từ $\mathfrak{s}\mathfrak{l}(2, k)$ vào $\mathfrak{g}$ sao cho $\tau (X_+) =x, \tau (H) =h, \tau (X_-) =y$ là một đồng cấu khác không và do đó đơn ánh (vì $\mathfrak{s}\mathfrak{l}(2, k)$ là đơn), và có ảnh là $kx+kh+ky$. Như vậy ta thu được một song ánh chính tắc từ tập hợp các bộ ba $\mathfrak{s}\mathfrak{l}_2$ trong $\mathfrak{g}$ lên tập hợp các đồng cấu đơn ánh từ $\mathfrak{s}\mathfrak{l}(2, k)$ vào $\mathfrak{g}$. Nếu $\mathfrak{g}$ là nửa đơn và nếu $(x, h, y)$ là một bộ ba $\mathfrak{s}\mathfrak{l}_2$ trong $\mathfrak{g}$, thì $x$ và $y$ là các phần tử lũy linh của $\mathfrak{g}$ và $h$ là một phần tử nửa đơn của $\mathfrak{g}$ (Chap. I, §6, no. 3, Prop. 4).

#### Bổ đề 1 {#lie-viii-s11-lem-1 .statement tag=0171}

Cho $x, h, y, y'\in \mathfrak{g}$. Nếu $(x, h, y)$ và $(x, h, y')$ là các bộ ba $\mathfrak{s}\mathfrak{l}_2$ trong $\mathfrak{g}$, thì $y=y'$.

Thật vậy, $y-y'\in$ Ker(ad$_{\mathfrak{g}}x$) và (ad$_{\mathfrak{g}}h$)$(y-y') =-2(y-y')$. Nhưng ad$_{\mathfrak{g}}x$ là đơn ánh trên Ker($p+$ ad$_{\mathfrak{g}}h$) với mọi số nguyên $p >0 ($§1, no. 2, Hệ quả của Mệnh đề 2).

#### Bổ đề 2 {#lie-viii-s11-lem-2 .statement tag=0172}

Cho $\mathfrak{n}$ là một đại số con của $\mathfrak{g}$ sao cho, với mọi $n\in \mathfrak{n}$, ad$_{\mathfrak{g}}(n)$ là lũy linh. Cho $h\in \mathfrak{g}$ sao cho $[h,\mathfrak{n}] =\mathfrak{n}$. Khi đó $e^{ad_{\mathfrak{g}}\mathfrak{n}}.h=h+\mathfrak{n}$.

Rõ ràng là $e^{ad_{\mathfrak{g}}(\mathfrak{n})}.h\subset h+\mathfrak{n}$. Ta sẽ chứng minh rằng, nếu $v\in \mathfrak{n}$, thì $h+v\in e^{ad_{\mathfrak{g}}(\mathfrak{n})}.h$. Chỉ cần chứng minh rằng $h+v\in e^{ad_{\mathfrak{g}}(\mathfrak{n})}.h+\mathscr{C}0\mathfrak{n}$ với mọi $p\geq 1$ (vì $\mathscr{C}^p\mathfrak{n}= 0$ với $p$ đủ lớn). Điều này là rõ đối với $p= 1$ vì $\mathscr{C}^1\mathfrak{n}=\mathfrak{n}$. Bây giờ giả sử rằng ta đã chứng minh được sự tồn tại của $y_p\in \mathfrak{n}$ và $z_p\in \mathscr{C}^p\mathfrak{n}$ sao cho $h+v=e^{ad_{\mathfrak{g}}y_p}.h+z_p$. Vì (ad$_{\mathfrak{g}}h$)$(\mathfrak{n}) =\mathfrak{n}$, nên (ad$_{\mathfrak{g}}h$)$|\mathfrak{n}$ là một song ánh từ $\mathfrak{n}$ lên $\mathfrak{n}$, do đó hạn chế của nó lên $\mathscr{C}^p\mathfrak{n}$, vốn để $\mathscr{C}^p\mathfrak{n}$ ổn định, cũng là song ánh; do đó, tồn tại $z\in \mathscr{C}^p\mathfrak{n}$ sao cho $z_p= [z, h]$. Khi đó

$$
e^{ad_{\mathfrak{g}}(y_p+z)}h-e^{ad_{\mathfrak{g}}y_p}h\in [z, h] +\mathscr{C}^{p+1}\mathfrak{n}
$$

nên

$$
e^{ad_{\mathfrak{g}}(y_p+z)}h\in h+v-z_p+ [z, h] +\mathscr{C}^{p+1}\mathfrak{n}=h+v+\mathscr{C}^{p+1}\mathfrak{n}
$$

điều này thiết lập mệnh đề của chúng ta bằng quy nạp theo $p$.

#### Bổ đề 3 {#lie-viii-s11-lem-3 .statement tag=0173}

Cho $x\in \mathfrak{g},\mathfrak{p}=$ Ker(ad $x$)$,\mathfrak{q}=$ Im(ad $x$). Khi đó $[\mathfrak{p},\mathfrak{q}]\subset \mathfrak{q}$, và $\mathfrak{p}\cap \mathfrak{q}$ là một đại số con của $\mathfrak{g}$.

Nếu $u\in \mathfrak{p}$ và $v\in \mathfrak{q}$, thì tồn tại $w\in \mathfrak{g}$ sao cho $v= [x, w]$, nên

$$
[u, v] = [u,[x, w]] = [x,[u, w]]-[[x, u], w] = [x,[u, w]]\in \mathfrak{q}
$$

Mặt khác, $\mathfrak{p}$ là một đại số con của $\mathfrak{g}$, nên $[\mathfrak{p}\cap \mathfrak{q},\mathfrak{p}\cap \mathfrak{q}]\subset \mathfrak{p}\cap \mathfrak{q}$.

#### Bổ đề 4 {#lie-viii-s11-lem-4 .statement tag=0174}

Cho $(x, h, y)$ và $(x, h', y')$ là các bộ ba $\mathfrak{s}\mathfrak{l}_2$ trong $\mathfrak{g}$. Tồn tại $z\in \mathfrak{g}$ sao cho ad$_{\mathfrak{g}}z$ là lũy linh và sao cho

$$
e^{ad_{\mathfrak{g}}z}x=x,e^{ad_{\mathfrak{g}}z}h=h',e^{ad_{\mathfrak{g}}z}y=y'
$$

Đặt $\mathfrak{n}=$ Ker(ad $x$)$\cap$ Im(ad $x$). Với mọi $p\in \mathbf{Z}$, đặt $\mathfrak{g}_p=$ Ker(ad $h-p$). Theo §1, no. 3 (áp dụng cho biểu diễn liên hợp của $kx+ky+kh$ trên $\mathfrak{g}$), ta có $\mathfrak{n}\subset \sum_{p>0}\mathfrak{g}_p$, nên ad$_{\mathfrak{g}}n$ là lũy linh với mọi $n\in \mathfrak{n}$, và $[h,\mathfrak{n}] =\mathfrak{n}$. Ta có $[x, h'-h] = 0$ và $[x, y-y'] =h'-h$, nên $h'-h\in \mathfrak{n}$. Theo Bổ đề 2 và 3, tồn tại $z\in \mathfrak{n}$ sao cho $e^{ad_{\mathfrak{g}}z}h=h'$. Vì $z\in$ Ker ad$_{\mathfrak{g}}x$, ta có $e^{ad_{\mathfrak{g}}z}x=x$. Bổ đề 1 khi đó chứng minh rằng $e^{ad_{\mathfrak{g}}z}y=y'$. Q.E.D.

Cho G là một nhóm các tự đẳng cấu của $\mathfrak{g}$. Khi đó, hai bộ ba $\mathfrak{s}\mathfrak{l}_2$ $(x, h, y)$, $(x', h', y')$ được gọi là liên hợp dưới G nếu tồn tại $g\in G$ sao cho $gx=x'$, $gh=h', gy=y'$.

#### Mệnh đề 1 {#lie-viii-s11-prop-1 .statement tag=0175}

Cho G là một nhóm các tự đẳng cấu của $\mathfrak{g}$ chứa Aut$_e(\mathfrak{g})$. Cho $(x, h, y)$ và $(x', h', y')$ là các bộ ba $\mathfrak{s}\mathfrak{l}_2$ trong $\mathfrak{g}$. Đặt

$$
\mathfrak{t}=kx+kh+ky,\mathfrak{t}'=kx'+kh'+ky'
$$

Xét các điều kiện sau:

(i) $x$ và $x'$ liên hợp theo G;

(ii) $(x, h, y)$ và $(x', h', y')$ liên hợp theo G;

(iii) $\mathfrak{t}$ và $\mathfrak{t}'$ liên hợp theo G.

Ta có (i) $\Leftarrow \Rightarrow$ (ii) $=\Rightarrow$ (iii). Nếu $k$ đóng đại số, ba điều kiện là tương đương.

(i) $\Leftarrow \Rightarrow$ (ii): Điều này suy ra từ Bổ đề 4.

(ii) $=\Rightarrow$ (iii): Điều này là hiển nhiên.

Ta giả sử rằng $k$ đóng đại số và chứng minh rằng (iii) $=\Rightarrow$ (i). Trước hết ta xét trường hợp $\mathfrak{t}=\mathfrak{t}'=\mathfrak{g}=\mathfrak{s}\mathfrak{l}(2, k)$. Vì ad$_{\mathfrak{g}}x$ là lũy linh, tự đồng cấu $x$ của $k^2$ là lũy linh (Chương I, §6, Định lý 3), nên tồn tại một ma trận $A\in \mathbf{G}\mathbf{L}(2, k)$ sao cho $AxA^{-1}=X$, và do đó một tự đẳng cấu $\alpha$ của $\mathfrak{s}\mathfrak{l}(2, k)$ sao cho $\alpha (x) =x'$; bây giờ $\alpha \in$ Aut$_e(\mathfrak{g}) ($§5, no. 3, Hệ quả 2 của Mệnh đề 5). Bây giờ ta chuyển sang trường hợp tổng quát; ta giả sử rằng $\mathfrak{t}$ và $\mathfrak{t}'$ liên hợp dưới G và chứng minh rằng $x$ và $x'$ liên hợp dưới G. Ta có thể giả sử rằng $\mathfrak{t}=\mathfrak{t}'$. Theo điều nói trên, tồn tại $\beta \in$ Aut$_e(\mathfrak{t})$ sao cho $\beta x=x'$. Bây giờ, nếu $t\in \mathfrak{t}$ sao cho ad$_{\mathfrak{t}}t$ là lũy linh, thì ad$_{\mathfrak{g}}t$ là lũy linh; do đó $\beta$ mở rộng thành một phần tử của Aut$_e(\mathfrak{g})$.

#### Nhận xét {#lie-viii-s11-n1-rem-1 .statement tag=0176}

Ba điều kiện của Mệnh đề 1 là tương đương nếu ta chỉ giả sử rằng $k=k^2$ (x. Bài tập 1).

### 2. CÁC BỘ BA $\mathfrak{s}\mathfrak{l}_{2}$ TRONG CÁC ĐẠI SỐ LIE NỬA ĐƠN

#### Bổ đề 5 {#lie-viii-s11-lem-5 .statement tag=0177}

Cho V là một không gian vectơ hữu hạn chiều, A và B là các nội tự đồng cấu của V. Giả sử rằng A lũy linh và rằng $[A,[A,B]] = 0$. Khi đó AB lũy linh.

Đặt $C = [A,B]$. Vì $[A,C] = 0$,

$[A$, BC$^p] = [A,B]C^p= C^{p+1}$

với mọi số nguyên $p\geq 0$. Do đó, Tr(C$^p$) $= 0$ với $p\geq 1$, điều này chứng tỏ rằng C là lũy linh (Đại số, Chương VII, §3, no. 5, Hệ quả 4 của Mệnh đề 13). Bây giờ, cho $\overline{k}$ là một bao đóng đại số của $k$, và cho $\lambda \in \overline{k},x\in V\otimes_k\overline{k}$ sao cho AB$x=\lambda x$, $x\not= 0$. Quan hệ $[[B,A],A] = 0$ cho thấy rằng $[B,A^p] =p[B,A]A^{p-1}$ với mọi số nguyên $p\geq 0$. Gọi $r$ là số nguyên nhỏ nhất sao cho $A^rx= 0$. Khi đó

$\lambda A^{r-1}x= A^{r-1}$AB$x= A^rBx=$ BA$^rx-[B,A^r]x=-r[B,A]A^{r-1}x$.

Vì $[B,A]$ là lũy linh và vì $A^{r-1}x\not= 0$, điều này chứng tỏ rằng $\lambda = 0$. Do đó, mọi trị riêng của AB đều bằng không, suy ra bổ đề.

#### Bổ đề 6 {#lie-viii-s11-lem-6 .statement tag=0178}

Cho $h, x\in \mathfrak{g}$ sao cho $[h, x] = 2x$ và $h\in$ (ad $x$)$(\mathfrak{g})$. Khi đó tồn tại $y\in \mathfrak{g}$ sao cho $(x, h, y)$ hoặc là $(0,0,0)$ hoặc là một bộ ba $\mathfrak{s}\mathfrak{l}_2$.

Cho $\mathfrak{g}'$ là đại số Lie giải được $kh+kx$. Vì $x\in [\mathfrak{g}',\mathfrak{g}']$, ad$_{\mathfrak{g}}x$ là lũy linh (Chương I, §5, no. 3, Định lý 1); gọi $\mathfrak{n}$ là hạt nhân của nó. Vì [ad $h$, ad $x] =$ 2 ad $x$, ta có (ad $h$)$\mathfrak{n}\subset \mathfrak{n}$. Lấy $z\in \mathfrak{g}$ sao cho $h=-[x, z]$. Với mọi số nguyên $n\geq 0$, đặt $M_n=$ (ad $x$)$^n\mathfrak{g}$. Nếu $n >0$, ta có (§1, no. 1, Bổ đề 1)

[ad $z$,(ad $x$)$^n] =n$((ad $h$)$-n+$ 1)(ad $x$)$^{n-1}$

do đó, nếu $u\in M_{n-1}$,

$n$((ad $h$)$-n+ 1$)$u\in$ (ad $z$)(ad $x$)$u+ M_n$.

Vì (ad $h$)$\mathfrak{n}\subset \mathfrak{n}$, suy ra

((ad $h$)$-n+ 1$)$(\mathfrak{n}\cap M_{n-1})\subset \mathfrak{n}\cap M_n$.

Vì ad $x$ là lũy linh, nên $M_n= 0$ với $n$ đủ lớn. Do đó, các trị riêng của ad $h|\mathfrak{n}$ là các số nguyên $\geq 0$. Vậy hạn chế của ad $h+ 2$ lên $\mathfrak{n}$ là khả nghịch.

Bây giờ $[h, z] + 2z\in \mathfrak{n}$ vì

$$
[x,[h, z] + 2z] = [[x, h], z] + [h,[x, z]] + 2[x, z]
$$

$$
= [-2x, z] + [h,-h] + 2[x, z] = 0
$$

Do đó tồn tại $z'\in \mathfrak{n}$ sao cho $[h, z'] + 2z'= [h, z] + 2z$, tức là $[h, y] =-2y$, khi đặt $y=z-z'$. Vì $[x, y] = [x, z] =-h$, điều này hoàn tất chứng minh.

#### Mệnh đề 2 (Jacobson-Morozov) {#lie-viii-s11-prop-2 .statement tag=0179}

Giả sử rằng $\mathfrak{g}$ là nửa đơn. Cho $x$ là một phần tử lũy linh khác không của $\mathfrak{g}$. Tồn tại $h, y\in \mathfrak{g}$ sao cho $(x, h, y)$ là một bộ ba $\mathfrak{s}\mathfrak{l}_2$.

Đặt $\mathfrak{n}=$ Ker(ad $x$)$^2$. Nếu $z\in \mathfrak{n}$, thì [ad $x$,[ad $x$, ad $z]] =$ ad([$x,[x, z]]$) $= 0$. Theo Bổ đề 5, ad $x\circ$ ad $z$ là lũy linh, nên Tr(ad $x\circ$ ad $z$) $= 0$. Điều này cho thấy $x$ trực giao với $\mathfrak{n}$ đối với dạng Killing $\Phi$ của $\mathfrak{g}$. Vì

$\Phi$((ad $x$)$^2y, y'$) $=\Phi (y$, (ad $x$)$^2y')$

với mọi $y, y'\in \mathfrak{g}$, và vì $\Phi$ không suy biến nên phần bù trực giao của $\mathfrak{n}$ là ảnh của (ad $x$)$^2$. Do đó tồn tại $y'\in \mathfrak{g}$ sao cho $x=$ (ad $x$)$^2y'$. Đặt

$$
h=-2[x, y']
$$

ta có $[h, x] = 2x$ và $h\in$ (ad $x$)$(\mathfrak{g})$. Bây giờ chỉ còn áp dụng Bổ đề 6.

#### Hệ quả {#lie-viii-s11-n2-cor-1 .statement tag=017A}

Giả sử rằng $\mathfrak{g}$ là nửa đơn. Cho G là một nhóm các tự đẳng cấu của $\mathfrak{g}$ chứa Aut$_e(\mathfrak{g})$. Ánh xạ gán cho mỗi bộ ba $\mathfrak{s}\mathfrak{l}_2$ $(x, h, y)$ trong $\mathfrak{g}$ phần tử lũy linh $x$ xác định, bằng cách chuyển xuống thương, một song ánh từ tập hợp các lớp liên hợp theo G của các bộ ba $\mathfrak{s}\mathfrak{l}_2$ lên tập hợp các lớp liên hợp theo G của các phần tử lũy linh khác không.

Điều này suy ra từ Mệnh đề 1 và 2.

#### Bổ đề 7 {#lie-viii-s11-lem-7 .statement tag=017B}

Cho K là một trường giao hoán có ít nhất 4 phần tử. Gọi G là nhóm các ma trận $(\alpha 0\alpha \beta_{-1})$ trong đó $\alpha \in K^*,\beta \in K$. Gọi $G'$ là nhóm

gồm các ma trận như vậy sao cho $\alpha = 1$. Khi đó $G'= (G,G)$.

Nếu $\alpha , \alpha '\in K^*$ và $\beta , \beta '\in K$,

$$
(\alpha \beta )((\alpha '\beta ')((\alpha \beta )^{-1}(\alpha '\beta ')^{-1}
$$

0 $\alpha^{-1}$ 0 $\alpha^{'-1}$ 0 $\alpha^{-1}$ 0 $\alpha^{'-1}$

$$
=(1-\alpha '\beta '-{\alpha \beta \alpha '}^2+\alpha^2\alpha '\beta '+\alpha \beta )
$$

0 1

Đặc biệt,

$(1\beta )((\alpha '$ 0 $)((1\beta )^{-1}(\alpha '$ 0 $)^{-1}=(1\beta (1-{\alpha '}^2))$.

0 1 0 $\alpha^{'-1}$ 0 1 0 $\alpha^{'-1}$ 0 1

Nhưng tồn tại $\alpha '_0\in K^*$ sao cho $\alpha '_0\not= 1$ và $\alpha '_0\not=-1$, và khi đó $k.(1-{\alpha '_0}^2)$ $=k$, do đó bổ đề được chứng minh.

#### Mệnh đề 3 {#lie-viii-s11-prop-3 .statement tag=017C}

Giả sử rằng $\mathfrak{g}$ là nửa đơn. Nhóm Aut$_e(\mathfrak{g})$ bằng nhóm dẫn xuất của nó. Nếu $\mathfrak{g}$ phân rã được, Aut$_e(\mathfrak{g})$ là nhóm dẫn xuất của Aut$_0(\mathfrak{g})$.

Cho $x$ là một phần tử lũy linh khác không của $\mathfrak{g}$. Chọn $h, y\in \mathfrak{g}$ sao cho $(x, h, y)$ là một bộ ba $\mathfrak{s}\mathfrak{l}_2$ (Mệnh đề 2). Đại số con $\mathfrak{s}$ của $\mathfrak{g}$ sinh bởi $(x, h, y)$ có thể được đồng nhất với $\mathfrak{s}\mathfrak{l}(2, k)$. Gọi $\rho$ là biểu diễn $z \rightarrow$ ad$_{\mathfrak{g}}z$ của $\mathfrak{s}=\mathfrak{s}\mathfrak{l}(2, k)$ trên $\mathfrak{g}$, và gọi $\pi$ là biểu diễn của $\mathbf{S}\mathbf{L}(2, k)$ tương thích với $\rho ($§1, no. 4). Ảnh của $\pi$ được sinh bởi các exp($t$ ad$_{\mathfrak{g}}x$) và các exp($t$ ad$_{\mathfrak{g}}y$) với $t\in k($Đại số, Chap. III, §8, no. 9, Mệnh đề 17), do đó được chứa trong Aut$_e(\mathfrak{g})$. Vì $\mathbf{S}\mathbf{L}(2, k)$ bằng với nhóm dẫn xuất của nó (Bổ đề 7 và loc. cit.), exp(ad$_{\mathfrak{g}}x$) thuộc nhóm dẫn xuất G của Aut$_e(\mathfrak{g})$. Do đó Aut$_e(\mathfrak{g})$ bằng G. Bây giờ giả sử rằng $\mathfrak{g}$ là phân rã được. Vì Aut$_0(\mathfrak{g})/$Aut$_e(\mathfrak{g})$ là giao hoán (§5, no. 3, Nhận xét 3), điều vừa đi trước chứng minh rằng nhóm dẫn xuất của Aut$_0(\mathfrak{g})$ là Aut$_e(\mathfrak{g})$.

### 3. CÁC PHẦN TỬ ĐƠN

#### Định nghĩa 2 {#lie-viii-s11-def-2 .statement tag=017D}

Một phần tử $h$ của $\mathfrak{g}$ được gọi là đơn nếu tồn tại $x, y\in \mathfrak{g}$ sao cho $(x, h, y)$ là một bộ ba $\mathfrak{s}\mathfrak{l}_2$ trong $\mathfrak{g}$.

Ta cũng nói rằng $h$ là phần tử đơn của bộ ba $\mathfrak{s}\mathfrak{l}_2$ $(x, h, y)$.

#### Mệnh đề 4 {#lie-viii-s11-prop-4 .statement tag=017E}

Cho $h$ là một phần tử khác không của $\mathfrak{g}$. Khi đó $h$ là đơn khi và chỉ khi tồn tại $x\in \mathfrak{g}$ sao cho $[h, x] = 2x$ và $h\in$ (ad $x$)$(\mathfrak{g})$.

Điều kiện ấy rõ ràng là cần. Nó là đủ theo Bổ đề 6.

#### Mệnh đề 5 {#lie-viii-s11-prop-5 .statement tag=017F}

Giả sử rằng $\mathfrak{g}$ là nửa đơn tách được. Lấy $\mathfrak{h}$ là một đại số con Cartan tách của $\mathfrak{g}$, R là tập hợp các căn của $(\mathfrak{g},\mathfrak{h})$, và B là một cơ sở của R. Lấy $h$ là một phần tử đơn của $\mathfrak{g}$ thuộc $\mathfrak{h}$. Khi đó $h$ liên hợp dưới Aut$_e(\mathfrak{g},\mathfrak{h})$ với một phần tử $h'$ của $\mathfrak{h}$ sao cho $\alpha (h')\in  \{0,1,2\}$ với mọi $\alpha \in B$.

Các trị riêng của ad$_{\mathfrak{g}}h$ thuộc $\mathbf{Z}($§1, no. 2, Hệ quả của Mệnh đề 2). Do đó $h\in \mathfrak{h}_{\mathbf{Q}}$. Tồn tại một phần tử $w$ của nhóm Weyl của $(\mathfrak{g},\mathfrak{h})$ sao cho $\alpha (wh)\geq 0$ với mọi $\alpha \in B$ (Chap. VI, §1, no. 5, Định lý 2 (i)). Theo §2, no. 2, Hệ quả của Định lý 2, ta được quy về trường hợp trong đó $\alpha (h)\in \mathbf{N}$ với mọi $\alpha \in B$. Ký hiệu $R_+$ là tập hợp các căn dương đối với B, và $R_-=-R_+$. Tồn tại một bộ ba $\mathfrak{s}\mathfrak{l}_2$ trong $\mathfrak{g}$ có dạng $(x, h, y)$. Gọi T là tập hợp các căn $\beta$ sao cho $\beta (h) =-2$. Khi đó $T\subset R_-$ và $y\in \sum_{\beta\in T}\mathfrak{g}^{\beta}$. Giả sử rằng có

tồn tại $\alpha \in B$ sao cho $\alpha (h)>2$. Với mọi $\beta \in T$, ta có $(\alpha +\beta )(h)>0$, nên $\alpha +\beta  \notin R_-$ và $\alpha +\beta \not= 0$; mặt khác, vì $\beta \in R_-$ và $\alpha \in B$, ta có $\alpha +\beta  \notin R_+$; do đó $\alpha +\beta  \notin R\cup  \{0\}$, nên $[\mathfrak{g}^{\alpha},\mathfrak{g}^{\beta}] = 0$. Vì thế, $[y,\mathfrak{g}^{\alpha}] = 0$. Nhưng ad$_{\mathfrak{g}}y|\mathfrak{g}^{\alpha}$ là đơn ánh vì $\alpha (h)>0 ($§1, no. 2, Hệ quả của Mệnh đề 2). Mâu thuẫn này chứng tỏ rằng $\alpha (h)\leq 2$ với mọi $\alpha \in B$.

#### Hệ quả {#lie-viii-s11-n3-cor-1 .statement tag=017G}

Nếu $k$ đóng đại số và nếu $\mathfrak{g}$ là nửa đơn, hạng $l$, thì số các lớp liên hợp của các phần tử đơn của $\mathfrak{g}$, đối với Aut$_e(\mathfrak{g})$, không vượt quá $3^l$.

Thật vậy, mọi phần tử nửa đơn của $\mathfrak{g}$ đều liên hợp dưới Aut$_e(\mathfrak{g})$ với một phần tử của $\mathfrak{h}$.

#### Bổ đề 8 {#lie-viii-s11-lem-8 .statement tag=017H}

Giả sử rằng $k$ đóng đại số và $\mathfrak{g}$ nửa đơn. Gọi $h$ là một phần tử nửa đơn của $\mathfrak{g}$ sao cho các giá trị riêng của ad $h$ là hữu tỉ. Đặt $\mathfrak{g}^0=$ Ker(ad $h$)$,\mathfrak{g}^2=$ Ker(ad $h-2$). Gọi $G_h$ là tập hợp các tự đẳng cấu sơ cấp của $\mathfrak{g}$ cố định $h$. Gọi $x\in \mathfrak{g}^2$ sao cho $[x,\mathfrak{g}^0] =\mathfrak{g}^2$. Khi đó $G_hx$ chứa một tập con của $\mathfrak{g}^2$ vừa trù mật vừa mở đối với tôpô Zariski.

Cho $\mathfrak{h}$ là một đại số con Cartan của $\mathfrak{g}^0$. Khi đó đây là một đại số con Cartan của $\mathfrak{g}$ chứa $h$ (Chap. VII, §2, no. 3, Prop. 10). Ta có $h\in \mathfrak{h}_{\mathbf{Q}}$. Gọi R là hệ nghiệm của $(\mathfrak{g},\mathfrak{h}), Q$ là nhóm các trọng số căn. Tồn tại một cơ sở B của R sao cho $\alpha (h)\geq 0$ với mọi $\alpha \in B$.

Cho U là tập hợp các $z\in \mathfrak{h}$ sao cho $\alpha (z)\not= 0$ với mọi $\alpha \in B$. Gọi $(H'_{\alpha})_{\alpha\in B}$ là cơ sở của $\mathfrak{h}$ đối ngẫu với B. Nếu $z\in U$, tồn tại một đồng cấu từ Q vào $k^*$ biến mọi $\gamma \in Q$ thành $\prod_{\alpha\in B}\alpha (z)^{\gamma(H'_{\alpha})}$. Theo §5, Mệnh đề 2 và 4, tự

đồng cấu $\varphi (z)$ của không gian vectơ $\mathfrak{g}$ mà cảm sinh trên $\mathfrak{g}^{\gamma}$ phép vị tự có tỷ số $\prod_{\alpha\in B}\alpha (z)^{\gamma(H'_{\alpha})}$ là một tự đẳng cấu sơ cấp của $\mathfrak{g}$, rõ ràng

thuộc $G_h$.

Cho $s\in \mathfrak{h}$. Nếu $\gamma \in R$ sao cho $\mathfrak{g}^{\gamma}\cap \mathfrak{g}^2\not= 0$,

$$
2 =\gamma (h) =\gamma (\sum_{\alpha\in B}\alpha (h)H'_{\alpha})=\sum_{\alpha\in B}\alpha (h)\gamma (H'_{\alpha})
$$

vì $\alpha (h)\geq 0$ với mọi $\alpha \in B$, và vì các $\gamma (H'_{\alpha})$ là các số nguyên hoặc đều $\geq 0$ hoặc đều $\leq 0$, nên ta có $\gamma (H'_{\alpha})\in \mathbf{N}$ với mọi $\alpha \in B$. Do đó, ta có thể xét (với $z\in \mathfrak{h}$) tự đồng cấu $\psi (z)$ của không gian vectơ $\mathfrak{g}^2$ cảm sinh trên $\mathfrak{g}^{\gamma}\cap \mathfrak{g}^2$ phép vị tự có tỷ số $\prod_{\alpha\in B}\alpha (z)^{\gamma(H'_{\alpha})}$. Ánh xạ $z \rightarrow \psi (z)$ từ $\mathfrak{h}$ vào End($\mathfrak{g}^2$) là đa thức. Với $z\in U$, ta có $\psi (z) =\varphi (z)|\mathfrak{g}^2$.

Cho $\gamma_1, . . . , \gamma_r$ là các nghiệm phân biệt của $(\mathfrak{g},\mathfrak{h})$ triệt tiêu trên $h$. Nếu $y_1\in \mathfrak{g}^{\gamma_1}, . . .$, $y_r\in \mathfrak{g}^{\gamma_r}$, ta có $e^{ady_1}. . . e^{ady_r}\in G_h$. Do đó ta có thể định nghĩa một ánh xạ $\rho$ từ $\mathfrak{h}\times \mathfrak{g}^{\gamma_1}\times  \cdots  \times \mathfrak{g}^{\gamma_r}$ vào $\mathfrak{g}^2$ bằng cách đặt

$$
\rho (z, y_1, . . . , y_r) =\psi (z)e^{ady_1}. . . e^{ady_r}x
$$

với $z\in \mathfrak{h}, y_1\in \mathfrak{g}^{\gamma_1}, . . . , y_r\in \mathfrak{g}^{\gamma_r}$. Ánh xạ này là đa thức, và $\rho (U,\mathfrak{g}^{\gamma_1}, . . . ,\mathfrak{g}^{\gamma_r})$ $\subset G_hx$. Theo Chap. VII, App. I, Prop. 3 và 4, chỉ cần chứng minh rằng ánh xạ tuyến tính tiếp xúc của $\rho$ là toàn ánh tại một điểm nào đó.

Bây giờ, cho T là ánh xạ tuyến tính tiếp xúc của $z \rightarrow \psi (z)$ tại $h_0=\sum_{\alpha\in B}H'_{\alpha}$. Khi đó $T(z)$ là tự đồng cấu của $\mathfrak{g}^2$ cảm sinh trên $\mathfrak{g}^{\gamma}\cap \mathfrak{g}^2$ phép vị tự với tỷ số

$$
\sum_{\alpha\in B}\gamma (H'_{\alpha})\alpha (h_0)^{\gamma(H'_{\alpha})-1}\alpha (z)\prod_{\beta\in B,\beta\not=\alpha}\beta (h_0)^{\gamma(H'_{\alpha})}=\sum_{\alpha\in B}\gamma (H'_{\alpha})\alpha (z) =\gamma (z)
$$

Do đó, ánh xạ tuyến tính tiếp xúc của $z \rightarrow \rho (z,0, . . . ,0)$ tại $h_0$ là ánh xạ $z \rightarrow [z, x]$; ảnh của nó là $[x,\mathfrak{h}]$. Ánh xạ tuyến tính tiếp xúc tại 0 của ánh xạ $y_1 \rightarrow \rho (h_0, y_1,0, . . . ,0)$ là ánh xạ $y_1 \rightarrow \psi (h_0)[y_1, x]$; ánh xạ sau cùng này có ảnh là $\psi (h_0)[x,\mathfrak{g}^{\gamma_1}] = [x,\mathfrak{g}^{\gamma_1}]$. Tương tự, ánh xạ tuyến tính tiếp xúc tại 0 của ánh xạ $y_i \rightarrow \rho (h_0,0, . . . ,0, y_i,0, . . . ,0)$ có ảnh là $[x,\mathfrak{g}^{\gamma_i}]$. Cuối cùng, ánh xạ tuyến tính tiếp xúc của $\rho$ tại $(h_0,0, . . . ,0)$ có ảnh là

$$
[x,\mathfrak{h}+\mathfrak{g}^{\gamma_1}+\cdots +\mathfrak{g}^{\gamma_r}] = [x,\mathfrak{g}^0] =\mathfrak{g}^2.Q.E.D
$$

$^*$Nhóm $G_h$ là một nhóm đại số với đại số Lie ad $\mathfrak{g}^0._*$

#### Mệnh đề 6 {#lie-viii-s11-prop-6 .statement tag=017I}

Giả sử rằng $k$ đóng đại số và $\mathfrak{g}$ là nửa đơn. Cho G là một nhóm các tự đẳng cấu của $\mathfrak{g}$ chứa Aut$_e(\mathfrak{g})$. Cho $(x, h, y)$ và $(x', h', y')$ là các bộ ba $\mathfrak{s}\mathfrak{l}_2$ trong $\mathfrak{g}$. Các điều kiện sau là tương đương:

(i) $h$ và $h'$ liên hợp dưới G;

(ii) $(x, h, y)$ và $(x', h', y')$ liên hợp dưới G.

Ta chỉ còn phải chứng minh kéo theo (i) $=\Rightarrow$ (ii), và ngay lập tức quy về trường hợp $h=h'$. Đưa vào $\mathfrak{g}^2$ và $G_h$ như trong Bổ đề 8. Ta có $x\in \mathfrak{g}^2$, và $[x,\mathfrak{g}^0] =\mathfrak{g}^2$ theo §1, no. 2, Hệ quả của Mệnh đề 2. Do đó $G_hx$ chứa một tập con của $\mathfrak{g}^2$ vừa trù mật vừa mở trong tôpô Zariski, và $G_hx'$ cũng vậy. Vậy tồn tại $a\in G_h$ sao cho $a(x) =x'$. Ta có $a(h) =h$, và do đó $a(y) =y'$ (no. 1, Bổ đề 1).

#### Hệ quả 1 {#lie-viii-s11-prop-6-cor-1 .statement tag=017J}

Ánh xạ liên kết với mọi bộ ba $\mathfrak{s}\mathfrak{l}_2$ phần tử đơn của nó xác định, bằng cách chuyển sang các thương, một song ánh từ tập hợp các lớp liên hợp theo G của các bộ ba $\mathfrak{s}\mathfrak{l}_2$ đến tập hợp các lớp liên hợp theo G của các phần tử đơn.

#### Hệ quả 2 {#lie-viii-s11-prop-6-cor-2 .statement tag=017K}

Nếu rk($\mathfrak{g}$) $=l$, số các lớp liên hợp, đối với Aut$_e(\mathfrak{g})$, của các phần tử lũy linh khác không của $\mathfrak{g}$ nhiều nhất là $3^l$.

Điều này suy ra từ Hệ quả 1, Hệ quả của Mệnh đề 2, và Hệ quả của Mệnh đề 5.

#### Hệ quả 3 {#lie-viii-s11-prop-6-cor-3 .statement tag=017L}

Nếu rk($\mathfrak{g}$) $=l$, số các lớp liên hợp, đối với Aut$_e(\mathfrak{g})$, của các đại số con của $\mathfrak{g}$ đẳng cấu với $\mathfrak{s}\mathfrak{l}(2, k)$ nhiều nhất là $3^l$.

Điều này suy ra từ Hệ quả 1, Mệnh đề 1, và Hệ quả của Mệnh đề 5.

### 4. CÁC PHẦN TỬ CHÍNH

#### Định nghĩa 3 {#lie-viii-s11-def-3 .statement tag=017M}

Giả sử rằng $\mathfrak{g}$ là nửa đơn.

(i) Một phần tử lũy linh $x$ của $\mathfrak{g}$ được gọi là chính nếu chiều của Ker ad $x$ là hạng của $\mathfrak{g}$.

(ii) Một phần tử đơn $h$ của $\mathfrak{g}$ được gọi là chính nếu $h$ là chính quy và các giá trị riêng của ad $h$ trong một bao đóng đại số của $k$ thuộc $2\mathbf{Z}$.

(iii) Một bộ ba $\mathfrak{s}\mathfrak{l}_2$ $(x, h, y)$ của $\mathfrak{g}$ được gọi là chính nếu độ dài của $\mathfrak{g}$, được xét như một môđun trên $kx+kh+ky$, bằng với hạng của $\mathfrak{g}$.

#### Mệnh đề 7 {#lie-viii-s11-prop-7 .statement tag=017N}

Giả sử rằng $\mathfrak{g}$ là nửa đơn. Cho $(x, h, y)$ là một bộ ba $\mathfrak{s}\mathfrak{l}_2$ trong $\mathfrak{g}$. Các điều kiện sau là tương đương:

(i) $x$ là chính;

(ii) $h$ là chính;

(iii) $(x, h, y)$ là chính.

Với $p\in \mathbf{Z}$, đặt $\mathfrak{g}^p=$ Ker(ad $h-p$). Đặt $\mathfrak{g}'=\sum_{p\in\mathbf{Z}}\mathfrak{g}^{2p}$. Nếu coi $\mathfrak{g}$ như

một môđun trên $\mathfrak{a}=kx+kh+ky,\mathfrak{g}'$ là tổng của các môđun con đơn có chiều lẻ (§1, no. 2, Hệ quả của Mệnh đề 2). Gọi $l$ (resp. $l'$) là độ dài của $\mathfrak{g}$ (resp. $\mathfrak{g}'$) khi coi như một $\mathfrak{a}$-môđun. Theo §1, no. 2,

dim(Ker ad $x$) $=l\geq l'=$ dim(Ker ad $h$)$\geq$ rk($\mathfrak{g}$).

Sự tương đương của (i) và (iii) suy ra ngay lập tức. Mặt khác, điều kiện (ii) có nghĩa là dim(Ker ad $h$) $=$ rk($\mathfrak{g}$) và $\mathfrak{g}'=\mathfrak{g}$, nói cách khác là

dim(Ker ad $h$) $=$ rk($\mathfrak{g}$) và $l=l'$. Sự tương đương của (ii) với các điều kiện khác suy ra.

#### Mệnh đề 8 {#lie-viii-s11-prop-8 .statement tag=017O}

Giả sử rằng $\mathfrak{g}$ là nửa đơn và $\not= 0$. Gọi $\mathfrak{h}$ là một đại số con Cartan tách của $\mathfrak{g}$, R là hệ nghiệm của $(\mathfrak{g},\mathfrak{h})$, B là một cơ sở của R$,h^0$ là phần tử của $\mathfrak{h}$ sao cho $\alpha (h^0) = 2$ với mọi $\alpha \in B$.

(i) Phần tử $h^0$ là đơn và chính.

(ii) Các phần tử $x$ của $\mathfrak{g}$ sao cho tồn tại một bộ ba $\mathfrak{s}\mathfrak{l}_2$ có dạng $(x, h^0, y)$ là các phần tử của $\sum_{\alpha\in B}\mathfrak{g}^{\alpha}$ có thành phần khác không trong mỗi $\mathfrak{g}^{\alpha}$.

Phần tử $h^0$ là phần tử đã xét ở §7, no. 5, Bổ đề 2 (xem loc. cit., công thức (1)). Từ bổ đề này suy ra rằng $h^0$ là chính đơn và rằng, nếu $x\in \sum_{\alpha\in B}\mathfrak{g}^{\alpha}$ có thành phần khác không trong mỗi $\mathfrak{g}^{\alpha}$, thì tồn tại một bộ ba $\mathfrak{s}\mathfrak{l}_2$ có dạng $(x, h^0, y)$. Ngược lại, cho $(x, h^0, y)$ là một bộ ba $\mathfrak{s}\mathfrak{l}_2$. Ta có $[h^0, x] = 2x$, nên $x\in \sum_{\gamma\in R,\gamma(h^0)=2}\mathfrak{g}^{\gamma}=\sum_{\alpha\in B}\mathfrak{g}^{\alpha}$. Tương tự, $y\in \sum_{\alpha\in B}\mathfrak{g}^{-\alpha}$. Viết

$h^0=\sum_{\alpha\in B}a_{\alpha}H_{\alpha}$ trong đó $a_{\alpha}>0$ với mọi $\alpha \in B$,

$x=\sum_{\alpha\in B}X_{\alpha}$ trong đó $X_{\alpha}\in \mathfrak{g}^{\alpha}$ với mọi $\alpha \in B$,

$y=\sum_{\alpha\in B}X_{-\alpha}$ trong đó $X_{-\alpha}\in \mathfrak{g}^{-\alpha}$ với mọi $\alpha \in B$.

Khi đó

$$
\sum_{\alpha\in B}a_{\alpha}H_{\alpha}=h^0= [y, x] =\sum_{\alpha ,\beta\in B}[X_{-\beta}, X_{\alpha}] =\sum_{\alpha\in B}[X_{-\alpha}, X_{\alpha}]
$$

nên $[X_{-\alpha}, X_{\alpha}]\not= 0$ với mọi $\alpha \in B$.

#### Hệ quả {#lie-viii-s11-n4-cor-1 .statement tag=017P}

Trong một đại số Lie nửa đơn phân rã được, tồn tại các phần tử lũy linh chính.

Trong một đại số Lie nửa đơn không phân rã được, 0 có thể là phần tử lũy linh duy nhất.

#### Mệnh đề 9 {#lie-viii-s11-prop-9 .statement tag=017Q}

Giả sử rằng $k$ là đóng đại số và $\mathfrak{g}$ là nửa đơn. Mọi phần tử đơn chính (tương ứng, lũy linh) của $\mathfrak{g}$ đều liên hợp dưới Aut$_e(\mathfrak{g})$.

Ta giữ các ký hiệu của Mệnh đề 8. Cho $h$ là một phần tử đơn chính. Nó liên hợp dưới Aut$_e(\mathfrak{g})$ với một $h'\in \mathfrak{h}$ sao cho $\alpha (h')\in  \{0,1,2\}$ với mọi $\alpha \in B$ (no. 3, Mệnh đề 5). Vì $h'$ là đơn chính, nên $\alpha (h')\not= 0$ và $\alpha (h')\in 2\mathbf{Z}$ với mọi $\alpha \in B$, do đó $\alpha (h') = 2$ với mọi $\alpha \in B$, và vì thế $h'=h^0$. Điều này chứng minh mệnh đề đối với các phần tử đơn chính.

Cho $x, x'$ là các phần tử lũy linh chính. Tồn tại các bộ ba $\mathfrak{s}\mathfrak{l}_2$ $(x, h, y)$, $(x', h', y')$. Theo Mệnh đề $7,h$ và $h'$ là đơn chính, nên liên hợp dưới Aut$_e(\mathfrak{g})$ theo điều vừa nêu trên. Vậy $x$ và $x'$ liên hợp dưới Aut$_e(\mathfrak{g})$ (Mệnh đề 6).

#### Bổ đề 9 {#lie-viii-s11-lem-9 .statement tag=017R}

Với các ký hiệu của Mệnh đề 8, đặt $\mathfrak{g}^p=$ Ker(ad $h^0-p$) với $p\in \mathbf{Z}$. Gọi $\mathfrak{g}^2_*$ là tập hợp các phần tử của $\mathfrak{g}^2=\sum_{\alpha\in B}\mathfrak{g}^{\alpha}$ có một thành phần khác không

trong mỗi $\mathfrak{g}^{\alpha}$. Gọi $R_+$ là tập hợp các nghiệm dương đối với B$,\mathfrak{n}_+=\sum_{\alpha\in R_+}\mathfrak{g}^{\alpha}$, và $x\in \mathfrak{g}^2_*$. Khi đó $e^{ad\mathfrak{n}_+}.x=x+ [\mathfrak{n}_+,\mathfrak{n}_+]$.

Hiển nhiên là $e^{ad\mathfrak{n}_+}.x\subset x+ [\mathfrak{n}_+,\mathfrak{n}_+]$. Ta chứng minh rằng, nếu $v\in [\mathfrak{n}_+,\mathfrak{n}_+]$, thì $x+v\in e^{ad\mathfrak{n}_+}.x$. Đặt $\mathfrak{n}^{(p)}=\sum_{r\geq p}\mathfrak{g}^{2r}$; chỉ cần chứng minh rằng

$$
x+v\in e^{ad\mathfrak{n}_+}.x+\mathfrak{n}^{(p)}
$$

với mọi $p\geq 2$. Điều này là hiển nhiên khi $p= 2$ vì $\mathfrak{n}^{(2)}$ $= [\mathfrak{n}_+,\mathfrak{n}_+] ($§3, no. 3, Mệnh đề 9 (iii)). Giả sử ta đã tìm được $z\in \mathfrak{n}_+$ sao cho $v+x-e^{adz}.x\in$ $\mathfrak{n}^{(p)}$. Vì tồn tại một bộ ba $\mathfrak{s}\mathfrak{l}_2$ có dạng $(x, h^0, y)$ (Mệnh đề 8), §1, no. 2, Hệ quả của Mệnh đề 2 chứng minh rằng $[x,\mathfrak{g}^{2p-2}] =\mathfrak{g}^{2p}$; do đó tồn tại $z'\in \mathfrak{g}^{2p-2}\subset \mathfrak{n}_+$ sao cho

$$
v+x-e^{adz}.x\in [z', x] +\mathfrak{n}^{(p+1)}
$$

Vậy $v+x\in e^{ad(z+z')}.x+\mathfrak{n}^{(p+1)}$, và mệnh đề của chúng ta được thiết lập bằng quy nạp.

#### Mệnh đề 10 {#lie-viii-s11-prop-10 .statement tag=017S}

Giả sử rằng $\mathfrak{g}$ là nửa đơn. Cho $\mathfrak{h}$ là một đại số con Cartan tách của $\mathfrak{g}$, R là hệ nghiệm của $(\mathfrak{g},\mathfrak{h})$, B là một cơ sở của R, $R_+$ là tập hợp các nghiệm dương đối với B, và $\mathfrak{n}_+=\sum_{\alpha\in R_+}\mathfrak{g}^{\alpha}$. Các phần tử lũy linh chính thuộc $\mathfrak{n}_+$ là các phần tử của $\mathfrak{n}_+$ có một thành phần khác không trong $\mathfrak{g}^{\alpha}$ với mọi $\alpha \in B$.

Mệnh đề 8 và Bổ đề 9 chứng minh rằng các phần tử như thế là các phần tử lũy linh chính. Ta chứng minh mệnh đề đảo lại. Hiển nhiên ta có thể giả sử rằng $\mathfrak{g}$ là đơn. Gọi $h^0$ và $\mathfrak{g}^p$ như trong Mệnh đề 8 và Bổ đề 9. Gọi $\omega$ là nghiệm cao nhất, và đặt $\omega (h^0) = 2q$; ta có $q=h-1$, trong đó $h$ là số Coxeter của R, xem Chương VI, §1, no. 11, Mệnh đề 31. Khi đó $\mathfrak{g}^{2q}=\mathfrak{g}^{\omega},\mathfrak{g}^{-2q}=\mathfrak{g}^{-\omega}$, và $\mathfrak{g}^{2k}= 0$ với $|k|> q$. Tồn tại một bộ ba $\mathfrak{s}\mathfrak{l}_2$ chính $(x^0, h^0, y^0)$. Theo §1, no. 2, Hệ quả của Mệnh đề 2, (ad $x^0$)$^{2q}(\mathfrak{g}^{-\omega}) =\mathfrak{g}^{\omega}$, nên (ad $x^0$)$^{2q}\not= 0$. Gọi $x$ là một phần tử lũy linh chính của $\mathfrak{g}$ thuộc $\mathfrak{n}_+$. Nếu $\overline{k}$ là một bao đóng đại số của $k,x\otimes 1$ và $x^0\otimes 1$ liên hợp dưới một tự đẳng cấu của $\mathfrak{g}\otimes_k\overline{k}$ (Mệnh đề 9), nên (ad $x$)$^{2q}\not= 0$. Tồn tại $\lambda \in R$ sao cho (ad $x$)$^{2q}\mathfrak{g}^{\lambda}\not= 0$. Đặt $x=\sum_{n\geq 1}x_n$, trong đó $x_n\in \mathfrak{g}^{2n}$.

Khi đó

(ad $x$)$^{2q}\mathfrak{g}^{\lambda}\subset$ (ad $x_1$)$^{2q}\mathfrak{g}^{\lambda}+\sum_{k>4q+\lambda(h^0)}\mathfrak{g}^k=$ (ad $x_1$)$^{2q}\mathfrak{g}^{\lambda}$, vì $4q+\lambda (h^0)\geq 4q-2q= 2q$. Bây giờ (ad $x_1$)$^{2q}\mathfrak{g}^{\lambda}\subset \mathfrak{g}^{4q+\lambda(h^0)}$, trong đó $\lambda =-\omega$. Do đó, (ad $x_1$)$^{2q}\mathfrak{g}^{-\omega}=\mathfrak{g}^{\omega}$. Ta có $\omega =\sum_{\alpha\in B}n_{\alpha}\alpha$ với $n_{\alpha}>0$ với mọi $\alpha \in$ B (Chương VI, §1, no. 8, Nhận xét). Nếu tồn tại $\alpha_0\in B$ sao cho $x_1\in$

$\sum\mathfrak{g}^{\alpha}$, quan hệ

$\alpha \in B,\alpha \not=\alpha_0$

$$
\omega  \notin  -\omega +\sum_{\alpha\in B,\alpha\not=\alpha_0}k\alpha
$$

hàm ý rằng $\mathfrak{g}^{\omega}\not\subset$ (ad $x_1$)$^p\mathfrak{g}^{-\omega}$ với mọi $p$; điều này phi lý, vậy nên thành phần của $x_1$ trong $\mathfrak{g}^{\alpha}$ là khác không với mọi $\alpha \in B$.

### Bài tập {#lie-viii-s11-exercises}

Xem [bài tập của § 11](exercises/s11/).
