---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Semisimple Modules and Rings
section: 4
section_title: Trace of an Endomorphism of Finite Rank
appendix: true
lang: vi
source: alg-viii
source_edition: 2023, Springer Nature
book_pages: A VIII.463-A VIII.467
pdf_pages: 0480-0484
extraction: native
subsections:
    - "no": 1
      title: Linear Mappings of Finite Rank
      page: 463
      pdf_page: 480
    - "no": 2
      title: Trace of an Endomorphism of Finite Rank
      page: 464
      pdf_page: 481
statements: 5
exercises: 2
content_sha256: 762b1563ef2f43c28aaca2c81d1f4f9779bb4b6e49aaeb8a07d3522e6d1c6e40
translated_from: content/en/alg/VIII/A4_a4_trace_of_an_endomorphism_of_finite_rank.md
source_content_sha256: b21c8fa64810e183438c648b465f555368181eb6b34b8b9afdc829259a3d239d
translation_model: nemotron-3-ultra-free, laguna-s-2.1-free, hy3-free, nemotron-3.5-lightning-free
translation_run: translate-vi-ce069b8d
glossary_version: 30
glossary_terms_sha256: f6a58f22c1b06bcd4acb7571a13a4f5eb2c57ee57182ca4d838d0b77c1f23528
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## PHỤ LỤC 4 DẤU CỦA MỘT TỰ ĐỘNG CẤU HẠNG HỮU HẠN

### 1. Ánh xạ tuyến tính của hạng hữu hạn

Cho A là một vành, và cho E và F là các A-môđun. Ta ký hiệu bởi Hom$^f_A(E,F)$ tập hợp các ánh xạ tuyến tính từ E vào F có ảnh được chứa trong một môđun con sinh hữu hạn của F. Nó là một nhóm con của Hom$_A(E,F)$. Khi A là một trường, nó là tập hợp các ánh xạ tuyến tính từ E vào F có hạng hữu hạn (II, §7, No. 4, p. 298, Định nghĩa 3). Đặt End$^f_A(E) =$ Hom$^f_A(E,E)$.

Cho $E,F,G$ là các A-môđun, và cho $u: E\rightarrow F$ và $v: F\rightarrow G$ là các ánh xạ A-tuyến tính. Nếu $u\in$ Hom$^f_A(E,F)$ hoặc $v\in$ Hom$^f_A(F,G)$, thì $v\circ u$ thuộc Hom$^f_A(E,G)$.

Ký hiệu bằng $\theta$ là đồng cấu nhóm chính tắc từ $E^*\otimes_AF$ sang Hom$_A(E,F)$ (II, §4, No. 2, p. 271); nó gửi một phần tử $x^*\otimes y$ của $E^*\otimes_AF$ đến ánh xạ $x\mapsto  \langle x, x^*\rangle y$ từ E đến F.

#### Bổ đề 1 {#alg-viii-a4-lem-1 .statement tag=00QO}

Giả sử A-môđun F là xạ ảnh. Đồng cấu nhóm $\theta$ là đơn ánh, và ảnh của nó là Hom$^f_A(E,F)$.

Theo loc. cit., Hệ quả, đồng cấu $\theta$ là đơn ánh. Ảnh của nó được chứa trong Hom$^f_A(E,F)$. Đối với $u\in$ Hom$^f_A(E,F)$; chúng ta hãy chứng minh rằng $u$ thuộc ảnh của $\theta$.

Trước hết, giả sử rằng F là một A-môđun tự do. Cho $(f_i)_{i\in I}$ là một cơ sở của F, và cho $(f_i^*)_{i\in I}$ là cơ sở của $F^*$ đối ngẫu với $(f_i)_{i\in I}$. Cho J là một tập con hữu hạn của I sao cho ảnh của $u$ được chứa trong môđun con của F sinh bởi các $f_j$ với $j\in J$. Ta có

$$
u(x) =\sum_{j\in J}\langle u(x), f_j^*\rangle f_j=\sum_{j\in J}\langle x,^tu(f_j^*)\rangle f_j \tag{1}
$$

với mọi $x\in E$, và do đó

$$
u=\theta (\sum_{j\in J}^tu(f_j^*)\otimes f_j) \tag{2}
$$

Trong trường hợp tổng quát, tồn tại một A-môđun tự do L và các đồng cấu $i: F\rightarrow L$ và $p: L\rightarrow F$ sao cho $p\circ i= 1_F$. Đồng cấu $i\circ u$ thuộc Hom$^f_A(E,L)$. Theo trên, tồn tại một tập hợp hữu hạn J và, với mọi $j\in J$, các phần tử $x^*_j$ của $E^*$ và $y_j$ của L sao cho ta có

$$
i(u(x)) =\sum_{j\in J}\langle x, x^*_j\rangle y_j
$$

với mọi $x\in E$. Khi đó ta có

$$
u(x) =p(i(u(x))) =\sum_{j\in J}\langle x, x^*_j\rangle p(y_j)
$$

với mọi $x\in E$, và do đó $u=\theta (\sum_{j\in J}x^*_j\otimes p(y_j))$.

### 2. Dấu của một Tự Đồng Cấu Hạng Hữu Hạn

Trong tiểu mục này, A biểu thị một vành giao hoán. Cho E là một A-môđun xạ ảnh. Khi đó End$^f_A(E)$ là một A-môđun con của End$_A$(E), và ánh xạ chính tắc $E^*\otimes_AE\rightarrow$ End$_A(E)$ xác định một đẳng cấu $\theta_E$ của A-môđun từ $E^*\otimes_AE$ vào End$^f_A(E)$ (Bổ đề 1). Xét dạng tuyến tính chính tắc $\tau : E^*\otimes_AE\rightarrow A$ (II, §4, No. 3, p. 273) được đặc trưng bởi công thức $\tau (x^*\otimes x) =\langle x, x^*\rangle$. Bằng cách hợp nó với đẳng cấu $\theta^{-1}_E$, ta suy ra một dạng tuyến tính Tr : End$^f_A(E)\rightarrow A$, gọi là dạng vết. Khi A-môđun E là sinh hữu hạn, ta tìm lại định nghĩa của II, §4, No. 3, p. 273.

#### Mệnh đề 1 {#alg-viii-a4-prop-1 .statement tag=00QP}

Cho E là một A-môđun tự do. Cho $(e_i)_{i\in I}$ là một cơ sở của E, và cho $(e^*_i)_{i\in I}$ là cơ sở đối ngẫu của nó. Cho $u\in$ End$^f_A(E)$. Họ $(\langle u(e_i), e^*_i\rangle )_{i\in I}$ có giá hữu hạn, và tổng của nó bằng Tr($u$).

Đủ để xét trường hợp khi $u$ có dạng $\theta_E(x^*\otimes x)$ với $x\in E$ và $x^*\in E^*$. Khi đó họ $(\langle x, e^*_i\rangle )_{i\in I}$ có giá hữu hạn, và ta có $x=\sum_{i\in I}\langle x, e^*_i\rangle e_i$. Do đó, họ $(\langle x, e^*_i\rangle \langle e_i, x^*\rangle )_{i\in I}$ cũng có giá hữu hạn, và ta có $\langle x, x^*\rangle =\sum_{i\in I}\langle x, e^*_i\rangle \langle e_i, x^*\rangle$. Bây giờ, ta có $\langle u(e_i), e^*_i\rangle =\langle x, e^*_i\rangle \langle e_i, x^*\rangle$ với mọi $i\in I$. Điều này chứng minh mệnh đề.

#### Mệnh đề 2 {#alg-viii-a4-prop-2 .statement tag=00QQ}

Cho E, F là các A-môđun xạ ảnh. Cho $u\in$ Hom$^f_A(E,F)$ và $v\in$ Hom$_A(F,E)$. Ta có quan hệ

(3) Tr($v\circ u$) $=$ Tr($u\circ v$).

Ta chỉ cần chứng minh mệnh đề khi $u$ có dạng $\theta (x^*\otimes y)$ với $x^*\in E^*$ và $y\in F$. Trong trường hợp này, ta có

$v\circ u=\theta_E(x^*\otimes v(y))$ và $u\circ v=\theta_F(^tv(x^*)\otimes y)$,

và do đó

Tr($v\circ u$) $=\langle v(y), x^*\rangle =\langle y,^tv(x^*)\rangle =$ Tr($u\circ v$).

#### Hệ quả {#alg-viii-a4-n2-cor-1 .statement tag=00QR}

Cho E là một A-môđun xạ ảnh, $u$ là một phần tử của End$^f_A(E)$, và F là một A-môđun con xạ ảnh của E chứa Im $u$. Gọi $u_F$ là tự đồng cấu của F cảm sinh bởi $u$. Ta có

(4) Tr($u$) $=$ Tr($u_F$).

Gọi $i$ là đơn ánh chính tắc của F vào E và gọi $v: E\rightarrow F$ là đồng cấu suy ra từ $u$. Ta có $u_F=v\circ i$ và $u=i\circ v$. Hệ quả suy ra.

Cho E là một A-môđun xạ ảnh và $u\in$ End$^f_A(E)$. Với mọi số tự nhiên $p$, A-môđun $\wedge^pE$ là xạ ảnh (III, §7, No. 8, p. 519, Hệ quả 2), và tự đồng cấu $\wedge^pu$ thuộc End$^f_A(\wedge^pE)$ (III, §7, No. 3, p. 511, Mệnh đề 6) và bằng không với $p$ đủ lớn. Tập hợp $1_E+$ End$^f_A(E)$ là ổn định dưới hợp thành. Ta định nghĩa một ánh xạ det từ $1_E+$ End$^f_A(E)$ đến A bằng cách đặt

det(1$_E+u$) $=\sum_{p\geqslant 0}$ Tr $\wedge^pu$

với $u\in$ End$^f_A(E)$.

Nếu E là tự do và hữu hạn chiều, thì định nghĩa này phù hợp với định nghĩa của III, §8, No. 1, p. 522, theo hệ quả của III, §8, No. 5, p. 530.

#### Mệnh đề 3 {#alg-viii-a4-prop-3 .statement tag=00QS}

Cho E là một A-môđun xạ ảnh.

a) Cho $u\in$ End$^f_A(E)$. Cho F là một xạ ảnh A-môđun con của E chứa Im $u$, và cho $u_F$ là tự đồng cấu của F cảm sinh bởi $u$. Ta có

(5) det(1$_E+u$) $=$ det(1$_F+u_F$).

b) Cho $u$ và $v$ là hai phần tử của End$^f_A(E)$. Ta có

(6) det $(1_E+u)\circ (1_E+v)$ = det(1$_E+u$) det(1$_E+v$).

Chứng minh a). Với mọi số nguyên $p\geqslant 0$, môđun A xạảnh $\wedge^pF$ được xác định là một môđun con của $\wedge^pE$ (III, §7, No. 9, p. 520, Hệ qua). Hình ảnh của $\wedge^pu$ được chứa trong $\wedge^pF$, và tự đồng cấu của $\wedge^pF$ do $\wedge^pu$ bằng $\wedge^pu_F$. Do đó ta có Tr($\wedge^pu$) $=$ Tr($\wedge^pu_F$) bằng Hệ quả của Mệnh đề 2, và vì vậy a).

Ta chứng minh b). Cho G là một A-môđun sao cho A-môđun $L = E\oplus G$ là tự do. Ký hiệu $u'$ và $v'$ là các tự đồng cấu $u\oplus 0_G$ và $v\oplus 0_G$ của L. Theo a), ta có các hệ thức det(1$_L+u'$) $=$ det(1$_E+u$), det(1$_L+v'$) $=$ det(1$_E+v$), và

det(1$_L+u'+v'+u'\circ v'$) $=$ det(1$_E+u+v+u\circ v$).

Do đó, đủ để chứng minh mệnh đề b) khi A-môđun E là tự do. Khi đó tồn tại một môđun con tự do sinh hữu hạn F của E chứa ảnh của $u$ và ảnh của $v$. Đặt $w=u+v+u\circ v$. Ảnh của $w$ được chứa trong F, và ta có $w_F=u_F+v_F+u_F\circ v_F$. Do đó, theo (5), ta có det(1$_E+u$) $=$ det(1$_F+u_F$), det(1$_E+v$) $=$ det(1$_F+v_F$), và

det$((1_E+u)\circ (1_E+v))$

= det(1$_E+w$) $=$ det(1$_F+w_F$) $=$ det((1$_F+u_F$)$\circ (1_F+v_F)$).

Vì F là một A-môđun tự do sinh hữu hạn, ta có

det((1$_F+u_F$)$\circ (1_F+v_F)$) $=$ det(1$_F+u_F$) det(1$_F+v_F$) $=$ det(1$_E+u$) det(1$_E+v$).

### Bài tập {#alg-viii-a4-exercises}

Xem [bài tập cho phụ lục 4](exercises/a4/).
