---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Semisimple Modules and Rings
section: 5
section_title: Commutation
lang: vi
source: alg-viii
source_edition: 2023, Springer Nature
book_pages: A VIII.77-A VIII.94
pdf_pages: 0094-0111
extraction: native
subsections:
    - "no": 1
      title: The Commutant and Bicommutant of a Module
      page: 77
      pdf_page: 94
    - "no": 2
      title: Generating Modules
      page: 79
      pdf_page: 96
    - "no": 3
      title: The Bicommutant of a Generating Module
      page: 82
      pdf_page: 99
    - "no": 4
      title: The Countermodule of a Semisimple Module
      page: 84
      pdf_page: 101
    - "no": 5
      title: Density Theorem
      page: 88
      pdf_page: 105
    - "no": 6
      title: Application to Field Theory
      page: 89
      pdf_page: 106
statements: 37
exercises: 19
content_sha256: ce0628b82d6db685ba49146591784edd42d163dfe579ad0f90e2afc4061515f0
translated_from: content/en/alg/VIII/05_s5_commutation.md
source_content_sha256: 92146afa3071a759dfd60b0a1909d5b82cb570c6ed50a098e57fa1acd8ea9c00
translation_model: gpt-5.4
translation_run: translate-vi-fd029d78
glossary_version: 34
glossary_terms_sha256: ccbcb285b25da3f8a4a834b0cfcc78cbdd1f6d6f6d55001841ae0d5f6d22c0a0
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 5. GIAO HOÁN

### 1. Hoán tập và đối giao hoán tử kép của một môđun

Cho E là một vành và B là một tập con của E. Hoán tập (hay tập trung tâm hóa) của B trong E là vành con $B'$ của E gồm các phần tử giao hoán với mọi phần tử của B. Hoán tập $B''$ của $B'$ được gọi là đối giao hoán tử kép (hay đối tập trung tâm hóa) của B. Ta có $B\subset B''$, và $B'$ trùng với đối giao hoán tử kép của nó (III, §1, No. 2, p. 429). Tâm của một vành con B của E là $B\cap B'$; tâm chung của $B'$ và $B''$ là $B'\cap B''$. Nếu B là một vành con giao hoán của E, thì ta có $B\subset B'$, và $B''$ là tâm của $B'$ (III, §1, No. 2, p. 430).

Cho A là một vành và M là một A-môđun trái (tương ứng, phải). Hãy áp dụng các định nghĩa này cho trường hợp trong đó E là vành tự đồng cấu của nhóm cộng của M và B là vành các vị tự $A_M$ của M. Hoán tập $A'_M$ của $A_M$ trong E được gọi là hoán tập của M; đó là vành tự đồng cấu của A-môđun M. Đối giao hoán tử kép $A''_M$ của $A_M$ trong E được gọi là đối giao hoán tử kép của M; đó là vành tự đồng cấu của môđun đối của M (VIII, p. 8, Định nghĩa 3). Ta có $A_M\subset A''_M$, vành $A_M\cap A'_M$ là tâm của $A_M$, và $A'_M\cap A''_M$ là tâm chung của $A'_M$ và $A''_M$.

#### Định nghĩa 1 {#alg-viii-s5-def-1 .statement tag=005E}

A-môđun M là cân bằng nếu ta có $A_M= A''_M$.

Nếu A-môđun M là cân bằng, thì các vành $A_M$ và $A'_M$ có cùng tâm $A_M\cap A'_M$. Môđun M là một A-môđun cân bằng khi và chỉ khi nó là một $A_M$-môđun cân bằng. Môđun đối của một A-môđun M là trung thành và cân bằng.

Khi vành A giao hoán, đối giao hoán tử kép $A''_M$ của M là tâm của $A'_M=$ End$_A(M)$; việc M là cân bằng có nghĩa là tâm của End$_A(M)$ thu về các phép vị tự.

Với mọi phần tử $a$ của A, ký hiệu bởi $\boldsymbol{\delta }_a$ phép vị tự phải $x\mapsto xa$ từ A vào A và bởi $\boldsymbol{\gamma }_a$ phép vị tự trái $x\mapsto ax$ (I, §8, No. 1, p. 97). Ánh xạ $a\mapsto \boldsymbol{\delta }_a$ là một đẳng cấu vành từ $A^o$ lên hoán tập của A-môđun trái $A_s$ (xem II, §10, No. 7, p. 349, áp dụng cho $I =\{1\}$). Ánh xạ $a\mapsto \boldsymbol{\gamma }_a$ là một đẳng cấu vành từ A lên hoán tập của A-môđun phải $A_d$ (loc. cit.). Nếu ta đồng nhất A với hoán tập của $A_d$ qua ánh xạ này, thì môđun đối của $A_d$ được đồng nhất với $A_s$; do đó, A-môđun $A_d$ là cân bằng. Tương tự, A-môđun $A_s$ là cân bằng.

Cho $n$ là một số nguyên $\geqslant 1$. Ta xem $A^n$ như một $\mathbf{M}_n$(A)-môđun trái (nơi đã dẫn). Ánh xạ gửi $m\in \mathbf{M}_n(A)$ tới tự đồng cấu $x\mapsto mx$ của A-môđun $A^n_d$ là một đẳng cấu vành từ $\mathbf{M}_n(A)$ lên hoán tập của A-môđun phải $A^n_d$ (nơi đã dẫn).

#### Mệnh đề 1 {#alg-viii-s5-prop-1 .statement tag=005F}

Cho $(A_i)_{i\in I}$ là một họ các vành, và với mọi $i\in I$, cho $M_i$ là một $A_i$-môđun. Đặt $A =\prod A_i,M =\prod M_i$, và $N =\bigoplus M_i$. Trang bị cho M cấu trúc của một A-môđun với luật tác động $((a_i),(x_i))\mapsto (a_ix_i)$. Tập hợp N là một A-môđun con của M.

a) Ánh xạ $(u_i)\mapsto \prod u_i$ từ $\prod$ End$_{\mathbf{Z}}(M_i)$ vào End$_{\mathbf{Z}}(M)$ (II, §1, No. 5, p. 200) hạn chế thành các đẳng cấu vành từ $\prod(A_i)_{M_i},\prod(A_i)'_{M_i}$, và $\prod(A_i)''_{M_i}$ lên $A_M,A'_M$, và $A''_M$, tương ứng.

b) Ánh xạ $(u_i)\mapsto \bigoplus u_i$ từ $\prod$ End$_{\mathbf{Z}}(M_i)$ tới End$_{\mathbf{Z}}(N)$ (II, §1, No. 6, p. 203) hạn chế thành các đẳng cấu vành từ $\prod(A_i)_{M_i},\prod(A_i)'_{M_i}$, và $\prod(A_i)''_{M_i}$ lên $A_N,A'_N$, và $A''_N$, tương ứng.

Các đẳng cấu vành được xác định trong Mệnh đề 1 được gọi là chính tắc. Tích $\prod(A_i)_{M_i}$ thường được đồng nhất với $A_M$, và $\prod(A_i)'_{M_i}$ với $A'_M$, v.v., thông qua các đẳng cấu này.

Ánh xạ $\varphi : (u_i)\mapsto \prod u_i$ từ $\prod$ End$_{\mathbf{Z}}(M_i)$ vào End$_{\mathbf{Z}}(M)$ là một đồng cấu vành đơn ánh. Theo định nghĩa của cấu trúc A-môđun trên M, ta có $\varphi (\prod(A_i)_{M_i}) = A_M$. Lấy $u\in A'_M$. Với mọi $i\in I$, ký hiệu bởi $h_i$ phần tử của A mà mọi thành phần đều bằng 1 trừ thành phần có chỉ số $i$, thành phần này bằng 0. Nếu $x$ là một phần tử của M có thành phần chỉ số $i$ bằng 0, thì ta có $x=h_ix$, và do đó pr$_i(u(x)) =$ pr$_i(u(h_ix)) =$ pr$_i(h_iu(x)) = 0$. Do đó, tồn tại một đồng cấu nhóm duy nhất $u_i: M_i\mapsto M_i$ sao cho pr$_i(u(y)) =u_i$(pr$_i(y)$) với mọi $y\in M$. Ta có $u=\prod u_i$. Vì ánh xạ $u$ là A-tuyến tính, nên ánh xạ $u_i$ là $A_i$-tuyến tính với mọi $i\in I$. Điều này chứng tỏ rằng ảnh của $\prod(A_i)'_{M_i}$ dưới $\varphi$ chứa $A'_M$; bao hàm ngược lại là hiển nhiên. Áp dụng điều này cho môđun đối của M, ta suy ra rằng $\varphi$ cảm sinh một đẳng cấu từ $A''_M$ lên $\prod_i(A_i)''_{M_i}$. Điều này chứng minh mệnh đề a).

Chứng minh của b) cũng giống như chứng minh của a), mutatis mutandis.

#### Mệnh đề 2 {#alg-viii-s5-prop-2 .statement tag=005G}

Cho A là một vành, và M là một A-môđun. Cho I là một tập hợp. Khi đó đối giao hoán tử kép của A-môđun $M^{(I)}$ trùng với vành các vị tự của $A''_M$-môđun $M^{(I)}$.

Với $i\in I$, ta ký hiệu phép chiếu đồng cấu từ $M^{(I)}$ lên M bởi $\pi_i: (x_j)_{j\in I}\mapsto x_i$ và đơn ánh chính tắc tương ứng (I, §4, No. 9, p. 47) bởi $\iota_i: M\rightarrow M^{(I)}$.

Cho $u$ là một phần tử của End$_A(M^{(I)})$. Với mọi $i, j\in I$, hợp thành $u_{i,j}=\pi_j\circ u\circ \iota_i$ thuộc hoán tập $A'_M$ của M. Với mọi phần tử $b$ của $A''_M$ và mọi $(x_i)\in M^{(I)}$, ta có các hệ thức

$$
bu((x_i)_{i\in I})=b(\sum_{i\in I}u_{i,j}(x_i))_{j\in I}=(\sum_{i\in I}u_{i,j}(bx_i))_{j\in I}=u(b(x_i)_{i\in I})
$$

Vì vậy phép vị tự $b_{M^{(I)}}$ thuộc đối giao hoán tử kép của A-môđun $M^{(I)}$.

Ngược lại, cho $b$ là một phần tử của đối giao hoán tử kép của $M^{(I)}$. Với $i, j\in I$, đặt $b_{i,j}=\pi_j\circ b\circ \iota_i$. Lấy $i, j\in I$ với $i\not=j$. Vì $\iota_j\circ \pi_j$ thuộc hoán tập của A-môđun $M^{(I)}$, ta có

$$
b_{i,j}=\pi_j\circ \iota_j\circ \pi_j\circ b\circ \iota_i=\pi_j\circ b\circ \iota_j\circ \pi_j\circ \iota_i= 0
$$

Tương tự, ta có

$$
b_{j,j}=\pi_j\circ b\circ \iota_j=\pi_i\circ \iota_i\circ \pi_j\circ b\circ \iota_j=\pi_i\circ b\circ \iota_i\circ \pi_j\circ \iota_j=b_{i,i}
$$

Hơn nữa, $b_{i,i}$ thuộc $A''_M$. Suy ra $b$ trùng với một phép vị tự của $A''_M$-môđun $M^{(I)}$.

### 2. Môđun Sinh

Cho A là một vành.

#### Định nghĩa 2 {#alg-viii-s5-def-2 .statement tag=005H}

Một A-môđun M được gọi là sinh nếu mọi A-môđun N đều được sinh bởi các ảnh của các ánh xạ A-tuyến tính từ M vào N.

Cho M là một A-môđun trái. Ta ký hiệu đối ngẫu của M bởi $M^*$ và dạng song tuyến tính chính tắc trên $M\times M^*$ (II, §2, No. 3, p. 233) bởi

$$
(x, x^*)\mapsto  \langle x, x^*\rangle =x^*(x)
$$

Ta ký hiệu bởi $\tau (M)$ tập hợp các phần tử của A có dạng $\sum^n_{i=1}\langle x_i, x^*_i\rangle$, trong đó $x_1, . . . , x_n$ là các phần tử của M và $x^*_1, . . . , x^*_n$ là các phần tử của $M^*$. Đó là một iđêan hai phía của A, được gọi là iđêan vết của M. Iđêan vết của A-môđun $A_s$ là A. Nếu một môđun là tổng trực tiếp của một họ $(M_i)_{i\in I}$ các A-môđun, thì iđêan vết của nó là iđêan $\sum_{i\in I}\tau (M_i)$. Nếu M là một A-môđun xạ ảnh, thì từ Mệnh đề 12 của II, §2, No. 6, p. 238, suy ra rằng ta có $M =\tau (M)M$.

#### Định lý 1 {#alg-viii-s5-thm-1 .statement tag=005I}

Cho M là một A-môđun trái. Các tính chất sau là tương đương:

(i) A-môđun M là sinh.

(ii) Với mọi A-môđun N, tồn tại một tập hợp I và một ánh xạ A-tuyến tính toàn ánh từ $M^{(I)}$ đến N.

(iii) Tồn tại một số nguyên $n\geqslant 0$ và một ánh xạ A-tuyến tính toàn ánh từ $M^n$ đến $A_s$.

(iv) Tồn tại một số nguyên $n\geqslant 0$ sao cho $A_s$ đẳng cấu với một môđun con hạng tử trực tiếp của $M^n$.

(v) Iđêan vết $\tau (M)$ bằng A.

(vi) Tồn tại một số nguyên $n\geqslant 0$, các phần tử $x_1, . . . , x_n$ của M, và các phần tử $x^*_1, . . . , x^*_n$ của $M^*$ thỏa mãn $\sum^n_{i=1}\langle x_i, x^*_i\rangle = 1$.

(i) $\Rightarrow$ (ii): Giả sử rằng M là sinh, và cho N là một A-môđun trái. Tồn tại một họ $(u_i)_{i\in I}$ các ánh xạ A-tuyến tính từ M vào N sao cho ta có $N =\sum_{i\in I}u_i(M)$. Ánh xạ $(x_i)\mapsto \sum_{i\in I}u_i(x_i)$ từ $M^{(I)}$ vào N là A-tuyến tính và toàn ánh.

(ii) $\Rightarrow$ (iii): Giả sử rằng tính chất (ii) đúng, và lấy $N = A_s$. Khi đó ta có một tập hợp I và một ánh xạ tuyến tính toàn ánh $u: M^{(I)}\rightarrow A_s$. Vì $A_s$ được sinh bởi phần tử 1, tồn tại một tập con hữu hạn J của I sao cho $u(M^{(J)}) = A_s$, do đó có (iii).

(iii) $\Rightarrow$ (iv): Điều này suy ra từ Mệnh đề 21 của II, §1, No. 12, p. 218.

(iv) $\Rightarrow$ (v): Cho $n\geqslant 1$ là một số nguyên sao cho $A_s$ đẳng cấu với một môđun con hạng tử trực tiếp của M. Ta có $A =\tau (A_s)\subset \tau (M^n) =\tau (M)$ và vì thế $\tau (M) = A$.

(v) $\Rightarrow$ (vi): Điều này là hiển nhiên.

(vi) $\Rightarrow$ (i): Cho $n$ là một số nguyên $\geqslant 0,x_1, . . . , x_n$ là các phần tử của M, và $x^*_1, . . . , x^*_n$ là các phần tử của $M^*$ thỏa mãn $\sum^n_{i=1}\langle x_i, x^*_i\rangle = 1$. Cho N là một A-môđun trái và $y$ là một phần tử của N. Các ánh xạ $u_i:x\mapsto  \langle x, x^*_i\rangle y$ từ M vào N là A-tuyến tính, và ta có $y=\sum^n_{i=1}u_i(x_i)$. Điều này chứng tỏ M là một A-môđun sinh.

#### Hệ quả {#alg-viii-s5-n2-cor-1 .statement tag=00R1}

Một A-môđun sinh là trung thành.

Cho $a\in A$ thỏa mãn $aM = 0$. Dùng hệ quả (i) $\Rightarrow$ (iv) của Định lý 1, ta được $aA_s= 0$, và do đó $a= 0$. Hệ quả được suy ra (II, §1, No. 12, p. 219).

#### Ví dụ 1 {#alg-viii-s5-n2-exa-1 .statement tag=005J}

A-môđun $A_s$ là sinh.

#### Ví dụ 2 {#alg-viii-s5-n2-exa-2 .statement tag=005K}

Mọi A-môđun tự do khác không đều là sinh. Nói chung, mọi môđun có một thương sinh thì bản thân nó cũng là sinh.

#### Ví dụ 3 {#alg-viii-s5-n2-exa-3 .statement tag=005L}

Cho M là một A-môđun nửa đơn mà môđun đối của nó sinh hữu hạn. Khi đó M là một $A_M$-môđun sinh. Thật vậy, theo Bổ đề 4 của VIII, p. 8, tồn tại một số tự nhiên $m$ sao cho $(A_M)_s$ đẳng cấu với một môđun con của $M^m$. Vì $M^m$ là một $A_M$-môđun nửa đơn, $(A_M)_s$ đẳng cấu với một môđun con hạng tử trực tiếp của $M^m$ và M là một $A_M$-môđun sinh (Định lý 1).

#### Ví dụ 4 {#alg-viii-s5-n2-exa-4 .statement tag=005M}

Cho A là một miền iđêan chính, và cho P là một A-môđun hữu hạn sinh. Tồn tại một số nguyên $n\geqslant 1$ và một dãy tăng các iđêan $(\mathfrak{a}_i)_{1\leqslant i\leqslant n}$ của A sao cho P đẳng cấu với tổng trực tiếp của các $A/\mathfrak{a}_i$ (VII, §4, No. 4, p. 19, Định lý 2); linh hóa tử $\mathfrak{a}$ của P bằng $\mathfrak{a}_1$. Khi đó P là một môđun sinh trên vành $A/\mathfrak{a}$. Nếu P không phải là một môđun xoắn, thì ta có $\mathfrak{a}= 0$ và P là một A-môđun sinh.

#### Bổ đề 1 {#alg-viii-s5-lem-1 .statement tag=005N}

Cho A là một vành giao hoán, M một A-môđun hữu hạn sinh, và Ann(M) là linh hóa tử của nó. Cho $\mathfrak{a}$ là một iđêan của A. Các tính chất sau là tương đương:

(i) $\mathfrak{a}M = M$.

(ii) Ann(M) $+\mathfrak{a}= A$.

(iii) Tồn tại một phần tử $a$ của $\mathfrak{a}$ sao cho $am=m$ với mọi $m\in M$.

(i) $\Rightarrow$ (ii): Cho $(x_1, . . . , x_n)$ là một họ sinh của A-môđun M. Nếu $\mathfrak{a}M = M$, thì mỗi $x_i$ có thể được viết dưới dạng $\sum^n_{j=1}c_{ij}x_j$, trong đó các $c_{ij}$ thuộc $\mathfrak{a}$. Ký hiệu ma trận $(c_{ij})$ bởi C và ma trận cột có các phần tử $x_1, . . . , x_n$ bởi X. Ta có ($I_n-C$)X = 0. Gọi $d$ là định thức và V là ma trận các phần bù đại số của ma trận $I_n-C$. Theo công thức (26) của III, §8, No. 6, p. 532, ta có $dX=^tV$($I_n-C$)X = 0, nên $d\in$ Ann(M). Mặt khác, vì các $c_{ij}$ thuộc $\mathfrak{a}$, ta có $d\equiv$ 1(mod $\mathfrak{a}$) (III, §8, No. 5, p. 529, (18)), và do đó $1\in$ Ann(M) $+\mathfrak{a}$.

(ii) $\Rightarrow$ (iii): Giả sử rằng (ii) đúng, tồn tại $a\in \mathfrak{a}$ và $b\in$ Ann(M) sao cho $a+b= 1$. Khi đó ta có $am=m$ với mọi $m\in M$.

(iii) $\Rightarrow$ (i): Điều này là hiển nhiên.

#### Mệnh đề 3 {#alg-viii-s5-prop-3 .statement tag=00R2}

Cho A là một vành giao hoán. Mọi A-môđun xạ ảnh sinh hữu hạn và trung thành đều là sinh. Nói chung hơn, một A-môđun xạ ảnh sinh hữu hạn P là một $A_P$-môđun sinh.

Cho P là một A-môđun xạ ảnh sinh hữu hạn. Ta có $\tau (P)P = P$ (VIII, p. 80).

Nếu A-môđun P là trung thành, thì iđêan $\tau (P)$ bằng A (Bổ đề 1) và A-môđun P là sinh (Định lý 1); điều này dẫn đến mệnh đề thứ nhất. Mệnh đề thứ hai suy ra từ Bổ đề 2 dưới đây.

#### Bổ đề 2 {#alg-viii-s5-lem-2 .statement tag=005O}

Cho A là một vành và M là một A-môđun xạ ảnh. $A_M$-môđun M là xạ ảnh.

Cho $(x_i)_{i\in I}$ là một họ sinh của A-môđun M. Tồn tại một họ $(x^*_i)_{i\in I}$ các dạng tuyến tính trên A-môđun M sao cho với mọi $x\in M$, họ $(\langle x, x^*_i\rangle )_{i\in I}$ có giá hữu hạn và $x=\sum_{i\in I}\langle x, x^*_i\rangle x_i$ (II, §2, No. 6, p. 238, Mệnh đề 12). Với mọi $i\in I$, ánh xạ $x\mapsto  \langle x, x^*_i\rangle_M$ là một dạng tuyến tính trên $A_M$-môđun M, và ta có $x=\sum_{i\in I}\langle x, x^*_i\rangle_Mx_i$ với mọi $x\in M$. Theo loc. cit., M là một $A_M$-môđun xạ ảnh.

### 3. Đối giao hoán tử kép của một môđun sinh

#### Định lý 2 {#alg-viii-s5-thm-2 .statement tag=005P}

Một môđun sinh là cân bằng.

Cho A là một vành, và cho M là một A-môđun sinh; theo định nghĩa, tồn tại một số nguyên $n\geqslant 0$, các phần tử $x_1, . . . , x_n$ của M, và các phần tử $x^*_1, . . . , x^*_n$ của đối ngẫu $M^*$ của M thỏa mãn $\sum^n_{i=1}\langle x_i, x^*_i\rangle = 1$. Nhắc lại (II, §4, No. 2, p. 271) rằng ta định nghĩa một đồng cấu nhóm $\theta : M^*\otimes_AM\rightarrow$ End$_A(M)$ bởi công thức $\theta (x^*\otimes y)(x) =\langle x, x^*\rangle y$. Nếu $u$ là một phần tử của đối giao hoán tử kép của M, thì nó giao hoán với End$_A(M)$; do đó, với mọi $y\in M$, ta có

$$
u(y) =u(\sum_{i=1}^n\langle x_i, x^*_i\rangle y)=\sum_{i=1}^nu(\theta (x^*_i\otimes y)(x_i))
$$

$$
=\sum_{i=1}^n\theta (x^*_i\otimes y)(u(x_i)) =(\sum_{i=1}^n\langle u(x_i), x^*_i\rangle )y
$$

Do đó, $u$ thuộc $A_M$, và M là cân bằng.

#### Hệ quả 1 {#alg-viii-s5-thm-2-cor-1 .statement tag=005Q}

Một môđun tự do là cân bằng.

Điều này là hiển nhiên nếu môđun bằng không, và một môđun tự do khác không là sinh (VIII, p. 81, Ví dụ 2).

#### Hệ quả 2 {#alg-viii-s5-thm-2-cor-2 .statement tag=00R3}

Cho A là một vành, và cho $n$ là một số nguyên $\geqslant 0$. Tâm của $\mathbf{M}_n(A)$ gồm các ma trận vô hướng có các phần tử thuộc tâm của A. Ta xem $A^n$ như một $\mathbf{M}_n(A)$-môđun trái (II, §10, No. 7, p. 349). Các tự đồng cấu của môđun này là các ánh xạ $x\mapsto xa$, trong đó $a$ chạy qua A.

Cho M là A-môđun phải $A^n_d$. Nó là cân bằng theo Hệ quả 1. Do đó, các tâm của $A_M, A'_M$ và $A''_M$ trùng nhau. Khi đó Hệ quả 2 suy ra từ việc $A_M$ được đồng nhất với A và $A'_M$ với $\mathbf{M}_n(A)$.

#### Nhận xét {#alg-viii-s5-n3-rem-1 .statement tag=005R}

Cho M là một A-môđun. Nếu $A_M$-môđun M là sinh, thì ta có $A_M= A''_M$ theo Định lý 2 áp dụng cho $A_M$-môđun M, do đó M là một A-môđun cân bằng.

#### Hệ quả 3 {#alg-viii-s5-thm-2-cor-3 .statement tag=005S}

Mọi môđun xạ ảnh hữu hạn sinh trên một vành giao hoán đều cân bằng.

Thật vậy, một môđun xạ ảnh hữu hạn sinh M là một $A_M$-môđun sinh theo Mệnh đề 3 của VIII, p. 82. Vậy hệ quả suy ra từ nhận xét trên.

#### Hệ quả 4 {#alg-viii-s5-thm-2-cor-4 .statement tag=005T}

Mọi môđun hữu hạn sinh trên một miền iđêan chính đều cân bằng.

Thật vậy, một môđun hữu hạn sinh M trên một miền iđêan chính A là một $A_M$-môđun sinh (VIII, p. 81, Ví dụ 4).

#### Hệ quả 5 {#alg-viii-s5-thm-2-cor-5 .statement tag=005U}

Cho K là một trường giao hoán, V là một không gian vectơ hữu hạn chiều trên K, và $u$ và $v$ là các tự đồng cấu của V. Các tính chất sau là tương đương:

(i) Tồn tại một đa thức P trong K[X] sao cho $v= P(u)$.

(ii) Tự đồng cấu $v$ giao hoán với mọi tự đồng cấu của V giao hoán với $u$.

Lấy A là vành K[X] và M là K[X]-môđun suy ra từ V và $u$ (VII, §5, No. 1, p. 28). Mệnh đề (i) có nghĩa là $v\in K[X]_M$ và (ii) có nghĩa là $v\in K[X]''_M$. Vậy Hệ quả 5 là một trường hợp riêng của Hệ quả 4.

#### Mệnh đề 4 {#alg-viii-s5-prop-4 .statement tag=005V}

Một môđun nửa đơn có môđun đối hữu hạn sinh thì cân bằng.

Điều này suy ra từ Ví dụ 3 của VIII, p. 81 và nhận xét.

#### Hệ quả 1 {#alg-viii-s5-prop-4-cor-1 .statement tag=005W}

Cho $(S_i)_{i\in I}$ là một họ hữu hạn các A-môđun đơn đôi một không đẳng cấu. Với $i\in I$, ký hiệu $D_i$ là vành đối của trường các nội cấu của $S_i$. Giả sử rằng với mọi $i\in I$, không gian vectơ $D_i$ $S_i$ là hữu hạn chiều. Khi đó ánh xạ $a\mapsto (a_{S_i})_{i\in I}$ từ A vào $\prod_{i\in I}$ End$_{D_i}(S_i)$ là toàn ánh.

Xét A-môđun $M =\prod_{i\in I}S_i$. Vì I hữu hạn, ta cũng có $M =\bigoplus_{i\in I}S_i$, và ảnh của $S_i$ trong M là thành phần đẳng kiểu của M kiểu $S_i$. Do đó, các nội cấu của A-môđun M là các ánh xạ $(s_i)\mapsto (s_id_i)$, trong đó $(d_i)_{i\in I}$ chạy qua $\prod_{i\in I}D_i$ (VIII, p. 66, Mệnh đề 5). Vì I hữu hạn và với mọi $i\in I$, không gian vectơ phải trên $D_i$ là $S_i$ hữu hạn chiều, nên môđun đối của M là sinh hữu hạn. Theo Mệnh đề 4, A-môđun M là cân bằng. Bây giờ, đối giao hoán tử kép của A-môđun M gồm các phần tử của End$_{\mathbf{Z}}(M)$ có dạng $\prod_{i\in I}u_i$, trong đó $(u_i)\in \prod_{i\in I}$ End$_{D_i}(S_i)$ (VIII, p. 78, Mệnh đề 1) vì End$_{D_i}(S_i)$ là đối giao hoán tử kép của $S_i$. Hệ quả suy ra từ đó.

Hệ quả này áp dụng được, đặc biệt, khi A là một đại số trên một trường giao hoán K và mỗi $S_i$ là một A-môđun đơn hữu hạn chiều như một không gian vectơ trên K: thật vậy, khi đó $D_i$ chứa các phép vị tự $\alpha_{S_i}$, với $\alpha$ chạy qua K, và $S_i$ là hữu hạn chiều trên $D_i$ vì nó hữu hạn chiều trên K.

#### Hệ quả 2 (định lý Burnside) {#alg-viii-s5-prop-4-cor-2 .statement tag=00S0}

Cho A là một đại số trên một trường giao hoán đóng đại số K, và S là một A-môđun đơn hữu hạn chiều như một không gian vectơ trên K. Khi đó ánh xạ $a\mapsto a_S$ từ A vào End$_K(S)$ là toàn ánh.

Thật vậy, trường các nội cấu của A-môđun S chỉ gồm các phép vị tự $\alpha_S$ với $\alpha \in K$ (VIII, p. 47, Định lý 1). Khi đó áp dụng Hệ quả 1 cho A-môđun đơn S.

### 4. Môđun Đối của một Môđun Nửa Đơn

Cho A là một vành. Ký hiệu tập hợp các lớp của các A-môđun đơn bởi $\mathscr{S}$. Với mọi $\lambda \in \mathscr{S}$, chọn một A-môđun đơn $S_{\lambda}$ thuộc lớp $\lambda$, và ký hiệu vành đối của trường các tự đồng cấu của $S_{\lambda}$ bởi $D_{\lambda}$. Ta xem $S_{\lambda}$ như một $(A,D_{\lambda}$)-song môđun.

Cho M là một A-môđun nửa đơn, và cho B là vành tự đồng cấu của M. Ký hiệu đối giao hoán tử kép của M bởi C. Với mọi $\lambda \in \mathscr{S}$, ký hiệu song môđun trái $(D_{\lambda}$, B)-Hom$_A(S_{\lambda},M)$ bởi $V_{\lambda}$. Cuối cùng, ký hiệu giá đỡ của A-môđun M bởi $\mathscr{S}_M$ (VIII, p. 66); đó cũng là tập hợp các phần tử $\lambda$ của $\mathscr{S}$ sao cho $V_{\lambda}$ khác không.

#### Nhận xét 1 {#alg-viii-s5-n4-rem-1 .statement tag=00R4}

Mô tả chính tắc $\alpha_M$ của A-môđun M là một đẳng cấu của các song môđun trái $(A$, B). Theo hệ quả của Mệnh đề 9, VIII, p. 71, ánh xạ $f\mapsto ($Hom(1$_{S_{\lambda}}, f$))$_{\lambda\in\mathscr{S}_M}$ từ B vào $\prod_{\lambda\in\mathscr{S}_M}$ End$_{D_{\lambda}}(V_{\lambda})$ là một đẳng cấu vành.

#### Mệnh đề 5 {#alg-viii-s5-prop-5 .statement tag=005X}

a) Môđun đối của M là nửa đơn.

b) Với mọi $\lambda \in \mathscr{S}_M$, B-môđun $V_{\lambda}$ là đơn, và hoán tập của nó bằng $(D_{\lambda})_{V_{\lambda}}$.

c) Ánh xạ $\lambda \mapsto$ cl(V$_{\lambda}$) là một song ánh từ giá của A-môđun M lên giá của môđun đối của nó.

d) Với mọi $\lambda \in \mathscr{S}_M$, B-môđun con $M_{\lambda}$ là thành phần đẳng kiểu thuộc kiểu $V_{\lambda}$ của B-môđun M, và bội số của $V_{\lambda}$ trong M bằng dim$_{D_{\lambda}}(S_{\lambda})$.

e) Với $s\in S$, ký hiệu ánh xạ $\varphi \mapsto \varphi (s)$ từ $V_{\lambda}=$ Hom$_A(S_{\lambda},M)$ vào M bởi $\widetilde{s}$. Nó là B-tuyến tính. Ánh xạ thu được $s\mapsto \widetilde{s}$ từ $S_{\lambda}$ vào Hom$_B(V_{\lambda},M)$ là một đẳng cấu của các $(A,D_{\lambda})$-song môđun.

Cho $\lambda \in \mathscr{S}_M$. Ký hiệu vành End$_{D_{\lambda}}(V_{\lambda})$ bởi $E_{\lambda}$; vì $V_{\lambda}$ là một không gian vectơ $D_{\lambda}$ khác không, nên nó là một $E_{\lambda}$-môđun đơn, (VIII, p. 45, Ví dụ 3), và hoán tập của nó bằng $(D_{\lambda})_{V_{\lambda}}$ (VIII, p. 82, Hệ quả 1 của Định lý 2). Vì $E_{\lambda}$ là vành các phép vị tự của B-môđun $V_{\lambda}$ (VIII, p. 71, Hệ quả của Mệnh đề 9), điều này chứng minh b).

Mô tả chính tắc $\alpha_M$ của M xác định một đẳng cấu $\alpha_{\lambda}$ từ $V_{\lambda}\otimes_{D^o_{\lambda}}S_{\lambda}$ đến $M_{\lambda}$. Vì $V_{\lambda}$ là một B-môđun đơn, B-môđun $V_{\lambda}\otimes_{D^o_{\lambda}}S_{\lambda}$ là đẳng kiểu kiểu $V_{\lambda}$ (VIII, p. 61, Mệnh đề 1); do đó điều tương tự cũng đúng đối với B-môđun $M_{\lambda}$, điều này chứng minh a).

Theo Nhận xét 1 ở trên, tồn tại các phần tử $e_{\lambda}$ của B, với $\lambda$ chạy qua $\mathscr{S}_M$, sao cho $(e_{\lambda})_{V_{\lambda}}= 1_{V_{\lambda}}$ và $(e_{\lambda})_{V_\mu}$ = 0 với $\mu\in \mathscr{S}_M$ và $\mu\not=\lambda$. Do đó các B-môđun đơn $V_{\lambda}$ đôi một không đẳng cấu, điều này chứng minh c) và mệnh đề thứ nhất của d). B-môđun $M_{\lambda}$ đẳng cấu với $V_{\lambda}\otimes_{D^o_{\lambda}}S_{\lambda}$, nên dim$_{D_{\lambda}}(S_{\lambda})$ là bội số của $V_{\lambda}$ trong M (II, §3, No. 7, p. 255, Hệ quả 1).

Ánh xạ $\sum_{\lambda\in\mathscr{S}_M}\alpha_{\lambda}$ từ $\bigoplus_{\lambda\in\mathscr{S}_M}V_{\lambda}\otimes_{D^o_{\lambda}}S_{\lambda}$ đến M cung cấp một mô tả (VIII, p. 69, Định nghĩa 5) của B-môđun nửa đơn M. Theo VIII, p. 70, Mệnh đề 8, b), với mọi $\lambda \in \mathscr{S}_M$, ánh xạ từ $S_{\lambda}$ đến Hom$_B(V_{\lambda},M)$ được mô tả trong e) là song ánh và $D_{\lambda}$-tuyến tính. Vì nó hiển nhiên là A-tuyến tính, điều này chứng minh e).

#### Nhận xét 2 {#alg-viii-s5-n4-rem-2 .statement tag=00R5}

Suy ra từ chứng minh rằng ánh xạ

$$
\sum_{\lambda\in\mathscr{S}_M}V_{\lambda}\otimes_{D^o_{\lambda}}S_{\lambda}\longrightarrow M
$$

được cảm sinh bởi mô tả chính tắc của M là một mô tả của môđun đối của M.

#### Mệnh đề 6 {#alg-viii-s5-prop-6 .statement tag=005Y}

a) Khi được xem như một song môđun $(A,B^o)$, M là nửa đơn.

b) Với mọi $\lambda \in \mathscr{S}_M,M_{\lambda}$ là một môđun con song $(A,B^o)$ đơn của M.

c) Với mọi môđun con song $(A,B^o)$ N của M, tồn tại một tập con Λ duy nhất của $\mathscr{S}_M$ sao cho N bằng $\oplus_{\lambda\in\Lambda}M_{\lambda}$.

Cho $\lambda$ thuộc $\mathscr{S}_M$. A-môđun trái $S_{\lambda}$ và B-môđun phải $V_{\lambda}$ là đơn, và $D_{\lambda}$ là vành đối của trường các tự đồng cấu của $S_{\lambda}$. Theo Hệ quả 2 của VIII, p. 63, $(A,B^o$)-song môđun $S_{\lambda}\otimes_{D_{\lambda}}V_{\lambda}$ là đơn, và điều tương tự cũng đúng với $M_{\lambda}$, là môđun đẳng cấu với nó. Điều này chứng minh b), và a) suy ra.

Nếu $\lambda$ và $\mu$ phân biệt trong $\mathscr{S}_M$, thì $M_{\lambda}$ và $M_\mu$ không đẳng cấu như các A-môđun, và do đó a fortiori cũng không đẳng cấu như các $(A,B^o$)-song môđun. Mệnh đề c) suy ra từ Hệ quả 2 của VIII, p. 68.

#### Mệnh đề 7 {#alg-viii-s5-prop-7 .statement tag=005Z}

a) Với mọi phần tử $c$ của đối giao hoán tử kép C của M và mọi $\lambda \in \mathscr{S}_M$, tồn tại một phần tử duy nhất $c_{\lambda}$ của End$_{D_{\lambda}}(S_{\lambda})$ sao cho với mọi $\varphi \in$ Hom$_A(S_{\lambda},M)$ và mọi $s\in S_{\lambda}$, ta có $c\varphi (s) =\varphi (c_{\lambda}s)$.

b) Trang bị cho các $S_{\lambda}$, với $\lambda$ chạy qua $\mathscr{S}_M$, cấu trúc C-môđun được xác định bởi a). Khi đó ánh xạ chính tắc $\alpha_M$ từ $\bigoplus_{\lambda\in\mathscr{S}_M}S_{\lambda}\otimes_{D_{\lambda}}V_{\lambda}$ tới M là một đẳng cấu của các $(C,B^o)$-song môđun.

c) Ánh xạ $c\mapsto (c_{\lambda})_{\lambda\in\mathscr{S}_M}$ là một đẳng cấu từ C lên $\prod_{\lambda\in\mathscr{S}_M}$ End$_{D_{\lambda}}(S_{\lambda})$.

Các khẳng định a) và c) suy ra từ VIII, p. 71, Mệnh đề 9 vì ánh xạ chính tắc $\alpha_M$ từ $\bigoplus_{\lambda\in\mathscr{S}}(S_{\lambda}\otimes_{D_{\lambda}}W_{\lambda})$ lên M cho một mô tả của B-môđun M (Nhận xét 2). Hơn nữa, $\alpha_M$ là $(C,B^o$)-tuyến tính, điều này chứng minh b).

#### Nhận xét 3 {#alg-viii-s5-n4-rem-3 .statement tag=0060}

Trang bị cho $S_{\lambda}$, với $\lambda \in \mathscr{S}_M$, cấu trúc C-môđun được cho bởi Mệnh đề 7, a). Nếu ta thay thế A bằng B và B bằng C trong Mệnh đề 5 (VIII, p. 85), thì ta thấy rằng với mọi $\lambda \in \mathscr{S}_M$, C-môđun trái $S_{\lambda}$ là đơn, với hoán tập là $D_{\lambda}$, rằng thành phần đẳng kiểu kiểu $S_{\lambda}$ của C-môđun M bằng $M_{\lambda}$, và rằng ánh xạ $\lambda \mapsto$ cl$_C(S_{\lambda})$ là một song ánh từ giá của A-môđun M lên giá của C-môđun M. Sau cùng, nhận thấy rằng các ánh xạ A-tuyến tính và các ánh xạ C-tuyến tính từ $S_{\lambda}$ đến M là trùng nhau, cũng như các A-môđun con và các C-môđun con của M, và rằng các vành End$_A(M)$ và End$_C(M)$ là bằng nhau.

Cho M là một A-môđun nửa đơn. Ký hiệu bởi Z tâm của đối giao hoán tử kép C của A-môđun M; đó cũng là tâm của hoán tập B của M. Trang bị cho M và các $S_{\lambda}$, với $\lambda \in \mathscr{S}_M$, các cấu trúc Z-môđun suy ra bằng hạn chế vô hướng từ các cấu trúc C-môđun. Với mọi $\lambda \in \mathscr{S}_M$, ký hiệu tâm của trường $D_{\lambda}$ bởi $Z_{\lambda}$.

#### Mệnh đề 8 {#alg-viii-s5-prop-8 .statement tag=0061}

a) Ánh xạ $z\mapsto (z_{S_{\lambda}})_{\lambda\in\mathscr{S}_M}$ là một đẳng cấu từ Z lên tích của các trường $Z_{\lambda}$.

b) A-môđun M là đẳng kiểu và khác không khi và chỉ khi Z là một trường.

c) Cho Λ là một tập con của $\mathscr{S}_M$. Ký hiệu bởi $e_{\Lambda}$ phần tử duy nhất của Z sao cho $(e_{\Lambda})_{S_{\lambda}}= 1_{S_{\lambda}}$ với $\lambda \in \Lambda$ và $(e_{\Lambda})_{S_{\lambda}}= 0$ với $\lambda \in \mathscr{S}_M-\Lambda$. Ta có $(e_{\Lambda})_{M_{\lambda}}= 1_{M_{\lambda}}$ với $\lambda \in \Lambda$ và $(e_{\Lambda})_{M_{\lambda}}= 0$ với $\lambda \in \mathscr{S}_M-\Lambda$.

d) Nếu giá $\mathscr{S}_M$ của M là hữu hạn, thì ánh xạ $\Lambda \mapsto e_{\Lambda}Z$ là một song ánh từ tập hợp các tập con của $\mathscr{S}_M$ lên tập hợp các iđêan của Z, và ánh xạ $\mathfrak{a}\mapsto \mathfrak{a}M$ là một song ánh từ tập hợp các iđêan của Z lên tập hợp các môđun con song $(A,B^o)$ của M. Các song ánh này là các đẳng cấu của các tập hợp có thứ tự. Song ánh ngược gửi một môđun con song $(A,B^o)$ N của M tới iđêan gồm các phần tử $z$ của Z mà gửi N vào M.

Với $\lambda \in \mathscr{S}_M, Z_{\lambda}$ là tâm chung của hoán tập $D_{\lambda}$ và đối giao hoán tử kép $C_{\lambda}$ của A-môđun $S_{\lambda}$. Theo Mệnh đề 7, c) ở trên, ánh xạ $c\mapsto (c_{\lambda})_{\lambda\in\mathscr{S}_M}$ là một đẳng cấu từ C lên $\prod_{\lambda\in\mathscr{S}_M}C_{\lambda}$. Bằng cách hạn chế vào các tâm, ta thu được đẳng cấu $z\mapsto (z_{S_{\lambda}})_{\lambda\in\mathscr{S}_M}$ từ Z lên $\prod_{\lambda\in\mathscr{S}_M}Z_{\lambda}$, do đó a).

Vành $\prod_{\lambda\in\mathscr{S}_M}Z_{\lambda}$ là một trường khi và chỉ khi tập hợp $\mathscr{S}_M$ chỉ có một phần tử, do đó b).

Mệnh đề c) suy ra từ Mệnh đề 7, a). Giả sử rằng $\mathscr{S}_M$ là hữu hạn. Từ a) và Mệnh đề 8 của I, §8, No. 10, p. 109, suy ra rằng ánh xạ $\Lambda \mapsto e_{\Lambda}Z$ là một đẳng cấu của các tập hợp có thứ tự từ $\mathfrak{P}(\mathscr{S}_M)$ lên tập hợp các iđêan của Z. Cho Λ là một tập con của $\mathscr{S}_M$. Theo c), ta có quan hệ $e_{\Lambda}$ZM $=e_{\Lambda}M =$ $\bigoplus_{\lambda\in\Lambda}M_{\lambda}$; do Mệnh đề 6, c) của VIII, p. 86, còn lại là mô tả song ánh ngược. Nhưng $z\in Z$ biến M vào $\bigoplus_{\lambda\in\Lambda}M_{\lambda}$ khi và chỉ khi $z=e_{\Lambda}z$, tức là, $z\in e_{\Lambda}Z$.

#### Hệ quả {#alg-viii-s5-n4-cor-1 .statement tag=0062}

Giả sử A là một đại số trên một trường giao hoán đóng đại số K và M là một A-môđun nửa đơn hữu hạn chiều như một không gian vectơ trên K. Với mọi $\lambda$ trong $\mathscr{S}_M$, ký hiệu bởi $e_{\lambda}$ phép chiếu của M có ảnh là $M_{\lambda}$ và hạt nhân là $\oplus_{\lambda\not=\mu}M_\mu$. Khi đó $(e_{\lambda})_{\lambda\in\mathscr{S}_M}$ là một cơ sở của không gian vectơ Z trên K.

Vì M là một không gian vectơ hữu hạn chiều trên K đồng thời là tổng trực tiếp của họ các môđun con khác không $(M_{\lambda})_{\lambda\in\mathscr{S}_M}$, tập hợp $\mathscr{S}_M$ là hữu hạn, và mỗi không gian $S_{\lambda}$, với $\lambda \in \mathscr{S}_M$, đều hữu hạn chiều trên K. Vì trường K là đóng đại số, ta có $D_{\lambda}= Z_{\lambda}= K$ (VIII, p. 47, Định lý 1), và ánh xạ $z\mapsto (z_{S_{\lambda}})_{\lambda\in\mathscr{S}_M}$ là một đẳng cấu từ Z lên $K^{\mathscr{S}_M}$ (Mệnh đề 8, a)). Khi đó hệ quả suy ra từ phần c) của Mệnh đề 8.

### 5. Định lý mật độ

#### Định lý 3 (Jacobson) {#alg-viii-s5-thm-3 .statement tag=00S1}

Cho M là một A-môđun nửa đơn, và cho $c$ là một tự đồng cấu của nhóm cộng M. Khi đó $c$ thuộc đối giao hoán tử kép $A''_M$ của M khi và chỉ khi nó thỏa mãn điều kiện sau:

(D) Với mọi tập con hữu hạn F của M, tồn tại một phần tử $a$ của A sao cho $c$ trùng với $a_M$ trên F.

Trước hết, giả sử rằng $c$ thỏa mãn điều kiện (D). Cho $u$ là một phần tử của $A'_M$. Cho $x$ là một phần tử của M, và áp dụng điều kiện (D) cho tập con $F =\{x, u(x)\}$. Tồn tại một phần tử $a$ của A sao cho $c(x) =ax$ và $c(u(x)) =au(x)$, do đó $u(c(x)) =u(ax) =au(x) =c(u(x))$. Vì $x$ là tùy ý, ta có $cu=uc$; do điều này đúng với mọi $u$, suy ra $c\in A''_M$.

Để chứng minh đảo lại, ta dùng bổ đề sau.

#### Bổ đề 3 {#alg-viii-s5-lem-3 .statement tag=0063}

Cho M là một A-môđun nửa đơn. Cho B là đối giao hoán tử kép của A-môđun M. Khi đó mọi A-môđun con của M đều là một B-môđun con của M.

Cho N là một A-môđun con của M. Theo Hệ quả 2 của VIII, p. 56, tồn tại một phép chiếu $p$ của A-môđun M có ảnh là N; nó thuộc về $A'_M$. Vì ta có quan hệ $pb=bp$ với mọi $b\in B$, suy ra N là một B-môđun con của M.

Hãy kết luận chứng minh của Định lý 3. Giả sử rằng $c$ thuộc $A''_M$, và đặt F = $\{x_1, . . . , x_n\}$ là một tập con hữu hạn của M. Ký hiệu phần tử $(x_1, . . . , x_n)$ của $M^n$ bởi $x$. A-môđun $M^n$ là nửa đơn và, theo Mệnh đề 2 của VIII, p. 79, đối giao hoán tử kép của nó trùng với các phép vị tự của $A''_M$-môđun $M^n$. Theo Bổ đề 3, A-môđun con $Ax$ của $M^n$ là một $A''_M$-môđun con của $M^n$. Lấy $a\in A$ sao cho $(cx_1, . . . , cx_n)$ bằng $ax$. Khi đó $c$ trùng với $a_M$ trên $\{x_1, . . . , x_n\}$, điều này kéo theo điều kiện (D).

#### Nhận xét {#alg-viii-s5-n5-rem-1 .statement tag=0064}

Ký hiệu vành các tự đồng cấu của nhóm cộng của M bởi E. Trang bị cho M tôpô rời rạc; vành E gồm các ánh xạ từ M vào M, và ta có thể trang bị cho nó tôpô cảm sinh bởi tôpô tích trên $M^M$ (“tôpô của hội tụ đơn giản trên M”, Gen. Top., I, §2, No. 3, p. 31). Tôpô trên E là Hausdorff và tương thích với cấu trúc nhóm cộng trên E. Với mọi $f$ trong E, các ánh xạ $g\mapsto f\circ g$ và $g\mapsto g\circ f$ từ E vào E là liên tục. Do đó, hoán tập của mọi tập con của E là đóng trong E. Vì thế Định lý 3 suy ra rằng $A''_M$ là bao đóng của $A_M$ trong E.

### 6. Ứng dụng vào Lý thuyết trường

#### Mệnh đề 9 {#alg-viii-s5-prop-9 .statement tag=0065}

Cho L là một trường và E là một vành con của End$_{\mathbf{Z}}(L)$ chứa ánh xạ $\boldsymbol{\gamma }_a:x\mapsto ax$ với mọi $a\in L$. Ký hiệu bởi K tập hợp các phần tử $a$ của L sao cho $u(xa) =u(x)a$ với mọi $x$ trong L và mọi $u$ trong E; đó là một trường con của L.

Cho V là một không gian con tuyến tính hữu hạn chiều của không gian vectơ phải trên K L, và $h$ là một ánh xạ K-tuyến tính từ V vào L. Tồn tại một phần tử của E trùng với $h$ trên V.

Ta xem L như một E-môđun trái. Vì E chứa các phép nhân trái $\boldsymbol{\gamma }_a$, mọi E-môđun con của L đều là một iđêan trái của trường L; do đó E-môđun L là đơn. Mọi tự đồng cấu của nhóm cộng của L giao hoán với các $\boldsymbol{\gamma }_a$ đều có dạng $\boldsymbol{\delta }_b:x\mapsto xb$ với $b$ thuộc L. Do đó, $b\mapsto \boldsymbol{\delta }_b$ là một đẳng cấu từ K lên vành đối của End$_E$(L), vành này là một trường.

Do đó đối giao hoán tử kép $E''$ của E-môđun L gồm các tự đồng cấu của không gian vectơ phải trên K L. Cho $v$ là một tự đồng cấu của không gian vectơ trên K L mà hạn chế của nó trên V trùng với $h$; nó là một phần tử của $E''$. Cho $(x_i)_{i\in I}$ là một cơ sở của V trên K; theo Định lý 3 (VIII, p. 88), tồn tại một phần tử $u$ của E sao cho $u(x_i) =v(x_i) =h(x_i)$ với $i\in I$. Theo tính tuyến tính, suy ra $u(x) =h(x)$ với mọi $x$ trong V.

#### Hệ quả {#alg-viii-s5-n6-cor-1 .statement tag=0066}

Cho L là một trường. Cho Γ là một nhóm con của nhóm tự đẳng cấu của trường L, và cho K là trường các bất biến của Γ. Cho V là một không gian con K-tuyến tính phải của L có số chiều hữu hạn $n$ trên K. Khi đó tồn tại các phần tử $\sigma_1, . . . , \sigma_n$ của Γ có tính chất sau: với mọi ánh xạ K-tuyến tính $u$ từ V vào L, tồn tại các phần tử $a_1, . . . , a_n$ của L sao cho ta có $u(x) =\sum_{i=1}^na_i\sigma_i(x)$ với mọi $x$ trong V.

Ký hiệu bởi E tập hợp các ánh xạ từ L vào L có dạng $x\mapsto$ $\sum_{\sigma\in\Gamma}a_{\sigma}\sigma (x)$, trong đó $(a_{\sigma})_{\sigma\in\Gamma}$ là một họ các phần tử của L có giá hữu hạn. Ta có $\boldsymbol{\gamma }_a\in E$ với mọi $a$ trong L, và E là một vành con của vành tự đồng cấu của nhóm cộng của L. Hơn nữa, trường K gồm các phần tử $a$ của L sao cho $u(xa) =u(x)a$ với mọi $x$ trong L và mọi $u$ trong E.

Cho H là không gian vectơ trái trên L Hom$_K(V,L)$; nó có chiều $n$. Theo Mệnh đề 9, nó được sinh bởi các phép hạn chế lên V của các phần tử của Γ. Tồn tại $n$ phần tử $\sigma_1, . . . , \sigma_n$ của Γ mà các phép hạn chế của chúng lên V tạo thành một cơ sở của H trên L. Hệ quả suy ra từ điều này.

#### Nhận xét {#alg-viii-s5-n6-rem-1 .statement tag=0067}

Khi trường L giao hoán, hệ quả này quy về định lý của Artin (V, §10, No. 6, p. 65).

### Bài tập {#alg-viii-s5-exercises}

Xem [các bài tập của § 5](exercises/s5/).
