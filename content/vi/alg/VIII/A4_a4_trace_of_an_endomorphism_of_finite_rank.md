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
content_sha256: aa21a0273f1aa1ac001b2490bc605edb1fe4e75781c420107fe0470def9c603b
translated_from: content/en/alg/VIII/A4_a4_trace_of_an_endomorphism_of_finite_rank.md
source_content_sha256: ba92c145789444929ea958210e1292209334a911aa56a4290cdf547ce73f18e1
translation_model: gpt-5-6-mini, gpt-5-6
translation_run: translate-vi-12f53b8f
glossary_version: 5
glossary_terms_sha256: 73e63d7b34eac127857aee08b035061acdd46cbc40f0baceb0e5045fa18fe8d1
prompt_sha256: 7816e1600c72058e14ecd8b330e9a16e059e370f96fa366ad5fc8f147bcd8dd9
---

## PHỤ LỤC 4 VẾT CỦA MỘT TỰ ĐỒNG CẤU HẠNG HỮU HẠN

### 1. Ánh xạ tuyến tính hạng hữu hạn

Cho A là một vành, và cho E và F là các A-môđun. Ta ký hiệu Hom$^f_A(E,F)$ là tập hợp các ánh xạ tuyến tính từ E vào F mà ảnh được chứa trong một môđun con sinh hữu hạn của F. Nó là một nhóm con của Hom$_A(E,F)$. Khi A là một trường, đó là tập hợp các ánh xạ tuyến tính từ E vào F có hạng hữu hạn (II, §7, No. 4, p. 298, Định nghĩa 3). Đặt End$^f_A(E) =$ Hom$^f_A(E,E)$.

Cho $E,F,G$ là các A-môđun, và cho $u: E\rightarrow F$ và $v: F\rightarrow G$ là các ánh xạ a-tuyến tính. Nếu $u\in$ Hom$^f_A(E,F)$ hoặc $v\in$ Hom$^f_A(F,G)$, thì $v\circ u$ thuộc Hom$^f_A(E,G)$.

Ký hiệu $\theta$ là đồng cấu nhóm chính tắc từ $E^*\otimes_AF$ vào Hom$_A(E,F)$ (II, §4, No. 2, p. 271); nó biến một phần tử $x^*\otimes y$ của $E^*\otimes_AF$ thành ánh xạ $x\mapsto  \langle x, x^*\rangle y$ từ E vào F.

#### Bổ đề 1 {#alg-viii-a4-lem-1 .statement tag=00QO}

Giả sử A-môđun F là xạ ảnh. Đồng cấu nhóm $\theta$ là đơn ánh, và ảnh của nó là Hom$^f_A(E,F)$.

Theo chỗ đã dẫn, Hệ quả, đồng cấu $\theta$ là đơn ánh. Ảnh của nó được chứa trong Hom$^f_A(E,F)$. Cho $u\in$ Hom$^f_A(E,F)$; ta chứng minh rằng $u$ thuộc ảnh của $\theta$.

Trước hết, giả sử A-môđun F là tự do. Cho $(f_i)_{i\in I}$ là một cơ sở của F, và cho $(f_i^*)_{i\in I}$ là cơ sở của $F^*$ đối ngẫu với $(f_i)_{i\in I}$. Cho J là một tập con hữu hạn của I sao cho ảnh của $u$ được chứa trong môđun con của F sinh bởi các $f_j$ với $j\in J$. Ta có

$$
u(x) =\sum_{j\in J}\langle u(x), f_j^*\rangle f_j=\sum_{j\in J}\langle x,^tu(f_j^*)\rangle f_j \tag{1}
$$

với mọi $x\in E$, và do đó

$$
u=\theta \sum_{j\in J}^tu(f_j^*)\otimes f_j \tag{2}
$$

Trong trường hợp tổng quát, tồn tại một A-môđun tự do L và các đồng cấu $i: F\rightarrow L$ và $p: L\rightarrow F$ sao cho $p\circ i= 1_F$. Đồng cấu $i\circ u$ thuộc Hom$^f_A(E,L)$. Theo trên, tồn tại một tập hữu hạn J và, với mọi $j\in J$, các phần tử $x^*_j$ của $E^*$ và $y_j$ của L sao cho

$$
i(u(x)) =\sum_{j\in J}\langle x, x^*_j\rangle y_j
$$

với mọi $x\in E$. Khi đó ta có

$$
u(x) =p(i(u(x))) =\sum_{j\in J}\langle x, x^*_j\rangle p(y_j)
$$

với mọi $x\in E$, và do đó $u=\theta \sum_{j\in J}x^*_j\otimes p(y_j)$ .

### 2. Vết của một tự đồng cấu hạng hữu hạn

Trong tiểu mục này, A ký hiệu một vành giao hoán. Cho E là một A-môđun xạ ảnh. Khi đó End$^f_A(E)$ là một môđun con của End$_A$(E), và ánh xạ chính tắc $E^*\otimes_AE\rightarrow$ End$_A(E)$ xác định một đẳng cấu $\theta_E$ của các A-môđun từ $E^*\otimes_AE$ lên End$^f_A(E)$ (Bổ đề 1). Xét dạng tuyến tính chính tắc $\tau : E^*\otimes_AE\rightarrow A$ (II, §4, No. 3, p. 273) được đặc trưng bởi công thức $\tau (x^*\otimes x) =\langle x, x^*\rangle$. Hợp thành nó với đẳng cấu $\theta^-_E^1$, ta suy ra một dạng tuyến tính Tr : End$^f_A(E)\rightarrow A$, gọi là dạng vết. Khi A-môđun E sinh hữu hạn, ta thu lại định nghĩa trong II, §4, No. 3, p. 273.

#### Mệnh đề 1 {#alg-viii-a4-prop-1 .statement tag=00QP}

Cho E là một A-môđun tự do. Cho $(e_i)_{i\in I}$ là một cơ sở của E, và cho $(e^*_i)_{i\in I}$ là cơ sở đối ngẫu của nó. Cho $u\in$ End$^f_A(E)$. Họ $(\langle u(e_i), e^*_i\rangle )_{i\in I}$ có giá hữu hạn, và tổng của nó bằng Tr($u$).

Chỉ cần xét trường hợp $u$ có dạng $\theta_E(x^*\otimes x)$ với $x\in E$ và $x^*\in E^*$. Họ $(\langle x, e^*_i\rangle )_{i\in I}$ khi đó có giá hữu hạn, và ta có $x=\sum_{i\in I}\langle x, e^*_i\rangle e_i$. Do đó, họ $(\langle x, e^*_i\rangle \langle e_i, x^*\rangle )_{i\in I}$ cũng có giá hữu hạn, và ta có $\langle x, x^*\rangle =\sum_{i\in I}\langle x, e^*_i\rangle \langle e_i, x^*\rangle$. Bây giờ, ta có $\langle u(e_i), e^*_i\rangle =\langle x, e^*_i\rangle \langle e_i, x^*\rangle$ với mọi $i\in I$. Điều này chứng minh mệnh đề.

#### Mệnh đề 2 {#alg-viii-a4-prop-2 .statement tag=00QQ}

Cho E, F là các A-môđun xạ ảnh. Cho $u\in$ Hom$^f_A(E,F)$ và $v\in$ Hom$_A(F,E)$. Ta có quan hệ

(3) Tr($v\circ u$) $=$ Tr($u\circ v$).

Chỉ cần chứng minh mệnh đề khi $u$ có dạng $\theta (x^*\otimes y)$ với $x^*\in E^*$ và $y\in F$. Trong trường hợp này, ta có

$v\circ u=\theta_E(x^*\otimes v(y))$ và $u\circ v=\theta_F(^tv(x^*)\otimes y)$,

và do đó

Tr($v\circ u$) $=\langle v(y), x^*\rangle =\langle y,^tv(x^*)\rangle =$ Tr($u\circ v$).

#### Hệ quả {#alg-viii-a4-n2-cor-1 .statement tag=00QR}

Cho E là một A-môđun xạ ảnh, $u$ là một phần tử của End$^f_A(E)$, và F là một môđun con A-xạ ảnh của E chứa Im $u$. Ký hiệu $u_F$ là tự đồng cấu của F cảm sinh bởi $u$. Ta có

(4) Tr($u$) $=$ Tr($u_F$).

Ký hiệu $i$ là đơn ánh chính tắc của F vào E và $v: E\rightarrow F$ là đồng cấu suy ra từ $u$. Ta có $u_F=v\circ i$ và $u=i\circ v$. Hệ quả được suy ra.

Cho E là một A-môđun xạ ảnh và $u\in$ End$^f_A(E)$. Với mọi tự nhiên

số $p$, A-môđun $\wedge^pE$ là xạ ảnh (III, §7, No. 8, p. 519, Hệ quả 2), và tự đồng cấu $\wedge^pu$ thuộc End$^f_A(\wedge^pE)$ (III, §7, No. 3, p. 511,

Mệnh đề 6) và bằng không khi $p$ đủ lớn. Tập $1_E+$ End$^f_A(E)$ ổn định đối với phép hợp thành. Ta định nghĩa một ánh xạ định thức det từ $1_E+$ End$^f_A(E)$ vào A bằng cách đặt

det(1$_E+u) =\sum_{p\geqslant 0}$ Tr $\wedge^pu$

với $u\in$ End$^f_A(E)$.

Nếu E là tự do và hữu hạn chiều, thì định nghĩa này trùng với định nghĩa trong III, §8, No. 1, p. 522, theo hệ quả của III, §8, No. 5, p. 530.

#### Mệnh đề 3 {#alg-viii-a4-prop-3 .statement tag=00QS}

Cho E là một A-môđun xạ ảnh.

a) Cho $u\in$ End$^f_A(E)$. Cho F là một môđun con A xạ ảnh của E chứa Im $u$, và cho $u_F$ là tự đồng cấu của F cảm sinh bởi $u$. Ta có

(5) det(1$_E+u) =$ det(1$_F+u_F)$.

b) Cho $u$ và $v$ là hai phần tử của End$^f_A(E)$. Ta có

(6) det $(1_E+u)\circ (1_E+v)$ = det(1$_E+u)$ det(1$_E+v)$.

Hãy chứng minh a). Với mọi số nguyên $p\geqslant 0$, A-môđun xạ ảnh $\wedge^pF$ có thể được đồng nhất với một môđun con của $\wedge^pE$ (III, §7, No. 9, p. 520, Hệ quả). Ảnh của $\wedge^pu$ được chứa trong $\wedge^pF$, và tự đồng cấu của $\wedge^pF$ cảm sinh bởi $\wedge^pu$ bằng $\wedge^pu_F$. Do đó ta có Tr($\wedge^pu$) $=$ Tr($\wedge^pu_F$) theo

Hệ quả của Mệnh đề 2, và do đó a).

Chúng ta chứng minh b). Cho G là một A-môđun sao cho A-môđun $L = E\oplus G$ là tự do. Ký hiệu $u'$ và $v'$ là các tự đồng cấu $u\oplus 0_G$ và $v\oplus 0_G$ của L. Theo a), ta có các hệ thức det(1$_L+u') =$ det(1$_E+u)$, det(1$_L+v') =$ det(1$_E+v)$, và

det(1$_L+u'+v'+u'\circ v') =$ det(1$_E+u+v+u\circ v)$.

Do đó chỉ cần chứng minh mệnh đề b) khi A-môđun E là tự do. Khi đó tồn tại một môđun con F tự do sinh hữu hạn của E chứa ảnh của $u$ và ảnh của $v$. Đặt $w=u+v+u\circ v$. Ảnh của $w$ được chứa trong F, và ta có $w_F=u_F+v_F+u_F\circ v_F$. Do đó, theo (5), ta có det(1$_E+u) =$ det(1$_F+u_F)$, det(1$_E+v) =$ det(1$_F+v_F)$, và

det $(1_E+u)\circ (1_E+v)$

= det(1$_E+w) =$ det(1$_F+w_F) =$ det((1$_F+u_F)\circ (1_F+v_F))$.

Vì F là một A-môđun tự do sinh hữu hạn, ta có

det((1$_F+u_F)\circ (1_F+v_F)) =$ det(1$_F+u_F)$ det(1$_F+v_F) =$ det(1$_E+u)$ det(1$_E+v)$.

### Bài tập {#alg-viii-a4-exercises}

Xem [các bài tập cho Phụ lục 4](exercises/a4/).
