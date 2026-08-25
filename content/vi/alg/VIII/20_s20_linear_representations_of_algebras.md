---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Semisimple Modules and Rings
section: 20
section_title: Linear Representations of Algebras
lang: vi
source: alg-viii
source_edition: 2023, Springer Nature
book_pages: A VIII.373-A VIII.395
pdf_pages: 0390-0412
extraction: native+ocr
subsections:
    - "no": 1
      title: Linear Representations of Algebras
      page: 373
      pdf_page: 390
    - "no": 2
      title: Restricted Dual of an Algebra
      page: 375
      pdf_page: 392
    - "no": 3
      title: Coefficients of a Module
      page: 377
      pdf_page: 394
    - "no": 4
      title: Restricted Dual and Matrix Coefficients
      page: 379
      pdf_page: 396
    - "no": 5
      title: Dual of a Semisimple Algebra
      page: 380
      pdf_page: 397
    - "no": 6
      title: Character of a Representation
      page: 382
      pdf_page: 399
    - "no": 7
      title: Coefficients of a Set of Classes of Modules
      page: 387
      pdf_page: 404
    - "no": 8
      title: Cogebra Structure on the Restricted Dual
      page: 388
      pdf_page: 405
statements: 31
exercises: 6
content_sha256: a669321174a60acaefceaea117bb65e9bce597696ab34baa8e63065dd82ba2b1
translated_from: content/en/alg/VIII/20_s20_linear_representations_of_algebras.md
source_content_sha256: 5ff83d16e3a49fa515ef33dc4d59f5844d64a112e8716f6ee4b4cde01df7b682
translation_model: gpt-5.4-mini, gpt-5-6-mini
translation_run: translate-vi-78153639
glossary_version: 34
glossary_terms_sha256: e4f54ef6d06428be7b581d79b344c2399e5e147e7fe02a64bc281dbb4a8d39ee
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 20. BIỂU DIỄN TUYẾN TÍNH CỦA ĐẠI SỐ

Trong tiết này, K là một vành giao hoán, và A là một K-đại số. Từ No. 2 trở đi, ta giả sử rằng K là một trường, và ta ký hiệu bởi $A^*$ đối ngẫu của không gian vectơ A trên K. Trong tiết này, ký hiệu $A^*$ không bao giờ chỉ nhóm nhân của vành A.

### 1. Biểu diễn tuyến tính của đại số

#### Định nghĩa 1 {#alg-viii-s20-def-1 .statement tag=00MD}

Cho M là một K-môđun. Một biểu diễn tuyến tính của đại số A trong M là một đồng cấu K từ A vào đại số End$_K(M)$.

Ta cũng nói rằng cặp $(M, \pi )$ là một biểu diễn tuyến tính của đại số A. Khi M là một K-môđun tự do, chiều của M được gọi là bậc (hay chiều) của $\pi$.

Cho $\pi$ là một biểu diễn tuyến tính của A trong M. Luật cộng trên M và phép toán ngoài $(a, x)\mapsto \pi (a)(x)$ định nghĩa một cấu trúc A-môđun trái trên M, mà ta ký hiệu là $M_{\pi}$. Ta nói rằng $M_{\pi}$ là môđun của biểu diễn $\pi$. Cấu trúc K-môđun trên M được thu được từ cấu trúc A-môđun trên $M_{\pi}$ bằng hạn chế vô hướng.

Ngược lại, cho E là một A-môđun trái. Cho M là K-môđun suy ra từ E bằng hạn chế vô hướng từ A xuống K, và cho $\pi$ là đồng cấu $a\mapsto a_E$ từ A vào End$_K(M)$. Khi đó $\pi$ là một biểu diễn của A trong M, và ta có $E = M_{\pi}$. Ta nói rằng $\pi$ là biểu diễn tuyến tính liên kết với A-môđun E.

Việc nghiên cứu A-môđun hay biểu diễn tuyến tính của A là như nhau. Chúng tôi sẽ chuyển một số định nghĩa về môđun sang ngôn ngữ của biểu diễn tuyến tính.

Cho $\pi$ là một biểu diễn tuyến tính của A trong M. Hạt nhân của đồng cấu $\pi$ là một iđêan hai phía của A, và chính là linh hóa tử của A-môđun $M_{\pi}$. Đồng cấu $\pi$ là đơn ánh khi và chỉ khi A-môđun $M_{\pi}$ là trung thành; khi đó ta nói rằng $\pi$ là một biểu diễn trung thành của A.

Cho $(M, \pi )$ và $(M', \pi ')$ là các biểu diễn tuyến tính của A. Một ánh xạ A-tuyến tính từ $M_{\pi}$ đến $M'_{\pi'}$ là một ánh xạ K-tuyến tính $u: M\rightarrow M'$ thỏa mãn quan hệ

$$
\pi '(a)\circ u=u\circ \pi (a) \tag{1}
$$

với $a\in A$. Một đẳng cấu từ $M_{\pi}$ đến $M'_{\pi'}$ là một đẳng cấu của K-môđun $u: M\rightarrow M'$ thỏa mãn điều kiện

$$
\pi '(a) =u\circ \pi (a)\circ u^{-1} \tag{2}
$$

với $a\in A$. Ta nói rằng $\pi$ và $\pi '$ là đẳng cấu nếu các A-môđun $M_{\pi}$ và $M'_{\pi'}$ đẳng cấu. Ta nói rằng $\pi$ là một biểu diễn con (tương ứng, biểu diễn thương) của $\pi '$ nếu $M_{\pi}$ là một môđun con (tương ứng, môđun thương) của $M'_{\pi'}$.

Giả sử cho một họ $(M_i, \pi_i)$ các biểu diễn tuyến tính của A. Cho M là K-môđun là tổng trực tiếp của các $M_i$; với mọi $a\in A$, cho $\pi (a)$ là tự đồng cấu $(x_i)_{i\in I}\mapsto (\pi_i(a)(x_i))_{i\in I}$ của M. Khi đó $\pi$ là một biểu diễn tuyến tính của A trong M. A-môđun $M_{\pi}$ là tổng trực tiếp của các A-môđun $(M_i)_{\pi}(i\in I)$; ta nói rằng $\pi$ là tổng trực tiếp của các $\pi_i$, và viết $\pi =\bigoplus\pi_{i^i}$.

Ta nói rằng biểu diễn $\pi$ của A trong M là đơn hay bất khả quy nếu A-môđun $M_{\pi}$ là đơn; ta nói rằng biểu diễn $\pi$ của A trên M là nửa đơn hay khả quy hoàn toàn nếu A-môđun $M_{\pi}$ là nửa đơn.

### 2. Đối ngẫu hạn chế của một đại số

Giả sử từ đây về sau rằng K là một trường.

Với $a\in A$, ký hiệu $\boldsymbol{\gamma }(a)$ là ánh xạ $x\mapsto ax$ và $\boldsymbol{\delta }(a)$ là ánh xạ $x\mapsto xa$ từ A đến A. Khi đó $\boldsymbol{\gamma }$ là một biểu diễn tuyến tính của A trong A, gọi là biểu diễn chính quy trái; tương tự, $\boldsymbol{\delta }$ là một biểu diễn tuyến tính của $A^o$ trong A, gọi là (lạm dụng ngôn ngữ) biểu diễn chính quy phải của A. Bằng chuyển vị, từ $\boldsymbol{\delta }$ và $\boldsymbol{\gamma }$ ta suy ra các biểu diễn tuyến tính của các đại số A và $A^o$ trong không gian vectơ $A^*$, cho trên $A^*$ một cấu trúc A-môđun trái và một cấu trúc $A^o$-môđun trái. Hai cấu trúc này tương ứng với một cấu trúc $(A$, A)-song môđun trên $A^*$ với các phép toán ngoài được xác định bởi các công thức

$$
\langle af, b\rangle =\langle f, ba\rangle \tag{3}
$$

$$
\langle f a, b\rangle =\langle f, ab\rangle \tag{4}
$$

đối với $a, b,\in A$ và $f\in A^*$.

Nhắc lại (II, §2, No. 4, p. 234, Định nghĩa 4) rằng nếu E là một không gian con tuyến tính của A, thì không gian trực giao $E'$ của nó trong $A^*$ là tập hợp các dạng tuyến tính trên A có hạn chế lên E bằng không. Tương tự, không gian trực giao $F'$ trong A của một không gian con tuyến tính F của $A^*$ là giao của các hạt nhân của các dạng tuyến tính thuộc F.

Ta biết (II, §7, No. 5, p. 299, Định lý 7) rằng ánh xạ $\varphi : E\mapsto E'$ là một song ánh từ tập hợp các không gian con tuyến tính của A có đối chiều hữu hạn đến tập hợp các không gian con tuyến tính của $A^*$ có số chiều hữu hạn. Ánh xạ ngược $\varphi^{-1}$ gửi một không gian con hữu hạn chiều F của $A^*$ tới không gian trực giao $F'$ của nó trong A.

#### Mệnh đề 1 {#alg-viii-s20-prop-1 .statement tag=00ME}

a) Ánh xạ $\varphi$ cảm sinh một song ánh từ tập hợp các iđêan trái (tương ứng phải, hai phía) của A có đối chiều hữu hạn đến tập hợp các môđun con phải A (tương ứng các môđun con trái A, các song môđun con) của $A^*$ có số chiều hữu hạn trên K.

b) Mọi iđêan trái hoặc phải của A có đối chiều hữu hạn đều chứa một iđêan hai phía có đối chiều hữu hạn.

#### Mệnh đề 2 {#alg-viii-s20-def-2 .statement tag=00MF}

Đối ngẫu hạn chế

của đại số trên K A, được ký hiệu bởi Θ(A), là hợp trong $A^*$ của các trực giao của các iđêan hai phía của A có đối chiều hữu hạn.

Theo Mệnh đề 1, ta có thể đưa ra các mô tả tương đương sau của Θ(A):

– hợp của các trực giao của các iđêan trái của A có đối chiều hữu hạn

– hợp của các trực giao của các iđêan phải của A có đối chiều hữu hạn – hợp của các trực giao của các iđêan hai phía của A có đối chiều hữu hạn – hợp của các A-môđun con trái của $A^*$ hữu hạn chiều trên K

– hợp của các A-môđun con phải của $A^*$ hữu hạn chiều trên K

– hợp của các $(A$, A)-môđun con song của $A^*$ hữu hạn chiều trên K.

Ta có $\Theta (A) = \Theta (A^o)$, và $\Theta (A) = A^*$ nếu A có bậc hữu hạn trên K. Cho $f\in A^*$; khi đó $f$ thuộc Θ(A) nếu và chỉ nếu $Af$ (resp. $fA, AfA$) là một không gian con tuyến tính của $A^*$ có số chiều hữu hạn trên K.

Tổng của hai $(A$, A)-môđun con song của $A^*$ hữu hạn chiều trên K có số chiều hữu hạn trên K. Suy ra Θ(A) là một $(A$, A)-môđun con song của $A^*$.

### 3. Các hệ số của một môđun

Cho E là một A-môđun trái. Cho $E^*$ là đối ngẫu của không gian vectơ E trên K; ta trang bị cho nó cấu trúc A-môđun phải tự nhiên. Với các phần tử $x$ của E và $x^*$ của $E^*$, ta ký hiệu bởi $c_E(x, x^*)$ dạng tuyến tính

$$
c_E(x, x^*) :a\mapsto  \langle x^*, ax\rangle \tag{5}
$$

trên A. Các dạng tuyến tính này được gọi là các hệ số của E. Không gian con của $A^*$ được sinh bởi các hệ số của E được ký hiệu là $\Theta_E(A)$. Nó khác không nếu E khác không.

Nếu F là một A-môđun đẳng cấu với E, thì E và F có cùng các hệ số và ta có $\Theta_F(A) = \Theta_E(A)$. Xét $E^*$ như một A-môđun trái trên $A^o$; một hệ số của E là một hệ số của $E^*$, và $\Theta_E(A)\subset \Theta_{E^*}(A^o)$. Do đó, nếu E hữu hạn chiều trên K, thì E và $E^*$ có cùng các hệ số, và ta có $\Theta_E(A) = \Theta_{E^*}(A^o)$.

Cho $(M, \pi )$ là một biểu diễn tuyến tính của đại số A. Các hệ số của A-môđun $M_{\pi}$ cũng được gọi là các hệ số của biểu diễn $\pi$. Hệ số $c_{M_{\pi}}(x, x^*)$, với $x\in M$ và $x^*\in M^*$, cũng được ký hiệu bởi $c_{\pi}(x, x^*)$; không gian vectơ $\Theta_{M_{\pi}}(A)$ cũng được ký hiệu bởi $\Theta_{\pi}(A)$.

#### Nhận xét 1 {#alg-viii-s20-n3-rem-1 .statement tag=00MG}

Giả sử M hữu hạn chiều trên K. Cho $(e_1, . . . , e_n)$ là một cơ sở của V, và cho $(e^*_1, . . . , e^*_n)$ là cơ sở đối ngẫu của nó. Ký hiệu $(\pi_{ij}(a))$ là ma trận của $\pi (a)$ theo cơ sở $(e_1, . . . , e_n)$ của V; ta có $\pi_{ij}=$ $c_{\pi}(e_j, e^*_i)$. Ánh xạ $a\mapsto (\pi_{ij}(a))$ là một đồng cấu từ A vào $\mathbf{M}_n(K)$; một đồng cấu như thế đôi khi được gọi là một biểu diễn ma trận của đại số A.

#### Nhận xét 2 {#alg-viii-s20-n3-rem-2 .statement tag=00MH}

Cho E là một A-môđun, và cho $E'$ là một môđun con của E. Theo hệ quả của Định lý 5 của II, §7, No. 5, p. 299, ta có $\Theta_{E'}(A)\subset \Theta_E(A)$ và $\Theta_{E/E'}(A)\subset \Theta_E(A)$.

Cho $\gamma_E$ là ánh xạ K-tuyến tính duy nhất từ $E\otimes_KE^*$ đến $A^*$ biến $x\otimes x^*$ thành $c_E(x, x^*)$. Nó là song tuyến tính $(A$, A)-, và ảnh của nó là $\Theta_E(A)$. Ta suy ra từ nó các ánh xạ A-tuyến tính $c'_E: E\rightarrow$ Hom$_A(E^*,A^*)$ và $c''_E: E^*\rightarrow$ Hom$_A(E,A^*)$ sao cho

$$
c'_E(x)(x^*) =c_E(x, x^*) =c''_E(x^*)(x)
$$

Ký hiệu $\theta_E$ là ánh xạ K-tuyến tính $\theta_E: E\otimes E^*\rightarrow$ End$_K(E)$ được đặc trưng bởi quan hệ

$$
\theta_E(x\otimes x^*)(y) =\langle x^*, y\rangle x
$$

với $x, y\in E$ và $x^*\in E^*$. Ảnh của nó là tập hợp End$^f_K(E)$ gồm các tự đồng cấu của E có hạng hữu hạn (VIII, p. 463). Theo định nghĩa của vết (loc. cit.), ta có

Tr($\theta_E(x\otimes x^*)$) $=\langle x^*, x\rangle$

với $x\in E$ và $x^*\in E^*$; do đó ta có

$\langle \gamma_E(x\otimes x^*), a\rangle =\langle x^*, ax\rangle =$ Tr($\theta_E(ax\otimes x^*)$) $=$ Tr($\theta_E(x\otimes x^*)a$).

Điều này cho quan hệ

$\langle \gamma_E(h), a\rangle =$ Tr($\theta_E(h)\circ a_E$)

với $a\in A$ và $h\in E\otimes_KE^*$. Điều này chứng minh rằng $\Theta_E(A)$ là tập hợp các dạng tuyến tính $a\mapsto$ Tr($u\circ a_E$) trên A, trong đó $u$ chạy qua End$^f_K(E)$.

#### Bổ đề 1 {#alg-viii-s20-lem-1 .statement tag=00MI}

Ánh xạ $c''_E$ là song ánh. Nếu E hữu hạn chiều, thì $c'_E$ cũng vậy.

Khi F là một A-môđun phải và G là một không gian vectơ K, ta đã định nghĩa trong II, §4, No. 1, p. 268, Mệnh đề 1, a) một đẳng cấu $\gamma$ của các không gian vectơ K từ Hom$_K(F\otimes_AE,G)$ đến Hom$_A(E$, Hom$_K(F,G))$. Đẳng cấu này biến $\varphi : F\otimes_AE\rightarrow G$ thành đồng cấu $e\mapsto (f\mapsto \varphi (f\otimes e))$. Qua đẳng cấu chính tắc từ $A_d\otimes_AE$ đến E (II, §3, No. 4, p. $249$)$,\gamma$ có thể được đồng nhất với $c''_E$ khi $F = A_d$ và G = K.

==========

Tương tự, đẳng cấu $\beta$ được định nghĩa trong II, §4, No. 1, p. 268, Mệnh đề 1, b) chuyên biệt thành một đẳng cấu $\beta$ từ Hom$_K(E^*\otimes_AA_s,K)$ đến Hom$_A(E^*$, Hom$_K(A_s,K))$. Khi E hữu hạn chiều, E có thể được đồng nhất một cách chính tắc với Hom$_K(E^*,K)$ và $E^*$ với $E^*\otimes_AA_s$; khi đó đồng cấu $\beta$ được đồng nhất với $c'_E$.

#### Mệnh đề 2 {#alg-viii-s20-prop-2 .statement tag=00MJ}

Cho E là một A-môđun trái.

a) Tập hợp các hệ số của E là hợp của các ảnh của các ánh xạ A-tuyến tính từ E đến $A^*$.

b) Giả sử, hơn nữa, E có số chiều hữu hạn $n$ trên K. Khi đó A-môđun trái $\Theta_E(A)$ đẳng cấu với một thương của $E^n$, A-môđun E đẳng cấu với một môđun con của $\Theta_E(A)^n$, và mọi phần tử của $\Theta_E(A)$ đều là một hệ số của $E^n$.

Mệnh đề a) suy ra từ tính toàn ánh của $c''_E$.

Ta chứng minh b). Gọi $(e^*_1, . . . , e^*_n)$ là một cơ sở của $E^*$ trên K. Vì $\Theta_E(A)$ được sinh bởi các hệ số của E, nên ánh xạ A-tuyến tính

$$
(x_1, . . . , x_n)\mapsto \sum_{i=1}^nc_E(x_i, e^*_i)
$$

từ $E^n$ đến $\Theta_E(A)$ là toàn ánh. Theo a), mọi phần tử của $\Theta_E(A)$ đều là một hệ số của $E^n$. Hơn nữa, ánh xạ A-tuyến tính

$$
x\mapsto (c_E(x, e^*_1), . . . , c_E(x, e^*_n))
$$

từ E đến $\Theta_E(A)^n$ là đơn ánh; điều đó chứng minh b).

#### Nhận xét 3 {#alg-viii-s20-n3-rem-3 .statement tag=00MK}

Cho E là một A-môđun con trái của $A^*$. Gọi $\varepsilon$ là dạng tuyến tính $y\mapsto y(1)$ trên E. Với mọi $x$ trong E, ta có $x=c_E(x, \varepsilon )$, nên E là một A-môđun con của $\Theta_E(A)$.

### 4. Đối ngẫu hạn chế và các hệ số ma trận

#### Mệnh đề 3 {#alg-viii-s20-prop-3 .statement tag=00ML}

Cho $(V, \pi )$ là một biểu diễn tuyến tính hữu hạn chiều của đại số A. Hạt nhân $\mathfrak{a}$ của $\pi$ là một iđêan hai phía của A có đối chiều hữu hạn, và $\Theta_{\pi}(A)$ là trực giao của $\mathfrak{a}$ trong $A^*$. Chuyển vị của ánh xạ $\pi$ xác định một đẳng cấu từ đối ngẫu của không gian vectơ trên K $\pi (A)$ đến $\Theta_{\pi}(A)$.

Vì End$_K(V)$ hữu hạn chiều trên $K,\mathfrak{a}$ là một iđêan hai phía của A có đối chiều hữu hạn. Không gian vectơ $\Theta_{\pi}(A)$ là một không gian con hữu hạn chiều của $A^*$, và trực giao của nó trong A bằng $\mathfrak{a}$; theo Định lý 7 của II, §7, No. 5, p. 301, vì thế không gian $\Theta_{\pi}(A)$ là trực giao của $\mathfrak{a}$ trong $A^*$. Hơn nữa, vì $\mathfrak{a}$ là hạt nhân của $\pi$, chuyển vị của ánh xạ $\pi$ xác định một đẳng cấu từ đối ngẫu của $\pi (A)$ đến trực giao của $\mathfrak{a}$ trong $A^*$ (II, §7, No. 5, p. 299, Hệ quả của Định lý 5).

#### Hệ quả {#alg-viii-s20-n4-cor-1 .statement tag=00MM}

Đối ngẫu hạn chế Θ(A) của A là tập hợp các hệ số của các biểu diễn tuyến tính hữu hạn chiều của A.

==========

Theo định nghĩa, Θ(A) là hợp của các phần trực giao của các iđêan hai phía của A có đối chiều hữu hạn. Vì vậy ta có $\Theta_{\pi}(A)\subset \Theta (A)$ với mọi biểu diễn tuyến tính hữu hạn chiều $\pi$ của A. Ngược lại, cho $f$ là một phần tử của Θ(A), và cho $\mathfrak{a}$ là một iđêan hai phía có đối chiều hữu hạn, được chứa trong hạt nhân của $f$ (VIII, p. 376, Định nghĩa 2). Kí hiệu $\pi$ là biểu diễn tuyến tính của A trong $A/\mathfrak{a}$ suy ra từ biểu diễn chính quy trái trong A bằng cách chuyển qua thương. Cho $x$ là lớp của 1 (mod $\mathfrak{a}$), và cho $x^*$ là dạng tuyến tính trên $A/\mathfrak{a}$ suy ra từ $f$. Ta có $f=c_{\pi}(x, x^*)$, do đó $f$ là một hệ số của $\pi$.

Chú ý rằng nếu $(V, \pi )$ là một biểu diễn tuyến tính của A không hữu hạn chiều trên K, thì không nhất thiết không gian $\Theta_{\pi}(A)$ được chứa trong Θ(A).

### 5. Đối ngẫu của một đại số nửa đơn

Cho $\Theta^{ss}(A)$ là đế của A-môđun trái Θ(A), tức là, (VIII, p. 65) môđun con nửa đơn lớn nhất của Θ(A). Ta kí hiệu bằng $\mathscr{S}_K$ tập các lớp của các A-môđun đơn (trái) hữu hạn chiều trên K. Khi A là một đại số nửa đơn bậc hữu hạn trên K, ta có $A^*= \Theta (A) = \Theta^{ss}(A)$ vì mọi A-môđun trái đều nửa đơn (VIII, p. 138, Mệnh đề 4).

#### Định lý 1 {#alg-viii-s20-thm-1 .statement tag=00MN}

a) Tập $\Theta^{ss}(A)$ gồm các hệ số của các biểu diễn nửa đơn hữu hạn chiều của A. Nó là một $(A,A)$-môđun con song của $A^*$.

b) Với mọi $S\in \mathscr{S}_K$, thành phần đẳng kiểu của Θ(A) kiểu S bằng $\Theta_S(A)$. A-môđun trái $\Theta^{ss}(A)$ là tổng trực tiếp của các môđun con $\Theta_S(A)$, khi S chạy qua $\mathscr{S}_K$.

c) Với mọi S trong $\mathscr{S}_K$, A-môđun phải $S^*$ là đơn, và $\Theta_S(A)$ là thành phần đẳng kiểu kiểu $S^*$ của A-môđun phải Θ(A). Ánh xạ gửi S tới cl(S$^*$) là một song ánh từ $\mathscr{S}_K$ tới tập các lớp của các A$^o$-môđun đơn có số chiều hữu hạn trên K.

d) Xét như một A-môđun phải, Θ(A) có đế là $\Theta^{ss}(A)$.

Cho E là một A-môđun nửa đơn có số chiều hữu hạn trên K. Mọi hệ số của E đều thuộc ảnh của một ánh xạ A-tuyến tính từ E đến $A^*$ (VIII, p. 378, Mệnh đề 2) và do đó thuộc $\Theta^{ss}(A)$. Ngược lại, cho $f\in \Theta^{ss}(A)$. Khi đó A-môđun $Af$ có số chiều hữu hạn trên K và là nửa đơn. Theo nhận xét ở VIII, p. 367$,f$ là một hệ số của $Af$.

Với mọi S trong $\mathscr{S}_K$, thành phần đẳng kiểu của Θ(A) kiểu S được sinh bởi các ảnh của các ánh xạ A-tuyến tính từ S đến $A^*$; do đó nó bằng $\Theta_S(A)$ theo Mệnh đề 2, a) của VIII, p. 378. Mặt khác, nếu S là một A-môđun đơn không hữu hạn chiều trên K, thì thành phần đẳng kiểu của Θ(A) kiểu S bằng 0: thật vậy, mọi môđun con đơn của Θ(A) đều là đơn sinh và do đó hữu hạn chiều trên K. Vì đế của Θ(A) là tổng trực tiếp của các thành phần đẳng kiểu của nó (VIII, p. 65, Mệnh đề 4), điều này chứng minh b).

Cho S là một A-môđun đơn có số chiều hữu hạn trên K. Vì không gian vectơ trên K S không bị rút về 0, nên điều đó cũng đúng với $S^*$. Cho E là một môđun con của A-môđun phải $S^*$; phần trực giao $E'$ của nó trong S là một A-môđun con của S. Vì S đơn, ta có либо $E'= 0$, trong trường hợp đó $E = S^*$, hoặc $E'= S$, trong trường hợp đó E = 0. Do đó $S^*$ là một A-môđun phải đơn.

We have $\Theta (A^o) = \Theta (A)$ (VIII, p. 376); ta đồng nhất các A-môđun phải với các $A^o$-môđun trái. Vì mọi không gian vectơ có số chiều hữu hạn trên K đều đẳng cấu với song đối của nó, điều trên chứng minh rằng ánh xạ $S\mapsto$ cl(S$^*$) là một song ánh từ $\mathscr{S}_K$ lên tập hợp các lớp của các $A^o$-môđun đơn có số chiều hữu hạn trên K. Bây giờ, với S trong $\mathscr{S}_K$, thành phần đẳng kiểu của $\Theta (A^o)$ kiểu $S^*$ bằng $\Theta_{S^*}(A^o)$ theo mệnh đề b) áp dụng cho đại số $A^o$, và ta có $\Theta_{S^*}(A^o) = \Theta_S(A)$. Các mệnh đề c) và d) suy ra ngay lập tức.

#### Hệ quả 1 {#alg-viii-s20-thm-1-cor-1 .statement tag=00MO}

Mọi A-môđun đơn có số chiều hữu hạn trên K đều đẳng cấu với một A-môđun con của Θ(A).

Điều này suy ra từ Định lý 1, b) vì ta có $\Theta_E(A)\not= 0$ với mọi A-môđun khác không E.

#### Hệ quả 2 {#alg-viii-s20-thm-1-cor-2 .statement tag=00MP}

Nếu hai A-môđun đơn có số chiều hữu hạn trên K có một hệ số chung khác không, thì chúng đẳng cấu.

Cho $S_1$ và $S_2$ là các A-môđun đơn có số chiều hữu hạn trên K với một hệ số chung khác không. Khi đó ta có $\Theta_{S_1}(A)\cap \Theta_{S_2}(A)\not= 0$. Bây giờ, $\Theta_{S_1}(A)$ là đẳng kiểu kiểu $S_1$, và $\Theta_{S_2}(A)$ là đẳng kiểu kiểu $S_2$. Do đó $S_1$ đẳng cấu với $S_2$.

Theo Định lý 1, $\Theta^{ss}(A)$ là một $(A$, A)-môđun con song môđun của $A^*$, tổng trực tiếp của các $(A$, A)-môđun song môđun $\Theta_S(A)$ khi S chạy qua $\mathscr{S}_K$. Các song môđun này đôi một không đẳng cấu vì chúng đã không đẳng cấu với nhau với tư cách là các A-môđun trái.

Cố định một S trong $\mathscr{S}_K$. Ký hiệu D là trường đối của End$_A$(S), và xem S như một D-môđun phải và $S^*$ như một D-môđun trái. Với các quy ước này, S là một $(A$, D)-môđun song môđun, $S^*$ là một $(D$, A)-môđun song môđun, và $S\otimes_DS^*$ là một $(A$, A)-môđun song môđun.

#### Mệnh đề 4 {#alg-viii-s20-prop-4 .statement tag=00MQ}

a) Tồn tại một đồng cấu nhóm $\lambda_S$ từ $S\otimes_DS^*$ đến $\Theta_S(A)$, được đặc trưng bởi

$$
\lambda_S(x\otimes x^*) =c_S(x, x^*) \tag{6}
$$

với $x\in S$ và $x^*\in S^*$. Ánh xạ này là một đẳng cấu của các $(A,A)$-môđun song môđun.

b) $(A,A)$-môđun song môđun $\Theta_S(A)$ là đơn.

Ánh xạ $\gamma_S: S\otimes_KS^*\rightarrow \Theta_S(A)$ được đặc trưng bởi công thức $\gamma_S(x\otimes x^*) =c_S(x, x^*)$ là $(A$, A)-tuyến tính và toàn ánh và thỏa mãn $\gamma_S(xd\otimes x^*)$ $=\gamma_S(x\otimes dx^*)$ với $x\in S,x^*\in S^*$, và $d\in D$. Do đó nó xác định một ánh xạ $(A$, A)-tuyến tính toàn ánh $\lambda_S: S\otimes_DS^*\rightarrow \Theta_S(A)$ được đặc trưng bởi công thức (6).

Ta hãy chứng minh rằng $S\otimes_DS^*$ là một song môđun đơn $(A$, A)-bimodule. Theo Hệ quả 2 của VIII, p. 63, mọi $(A$, A)-sub-bimodule của $S\otimes_DS^*$ đều có dạng $S\otimes_DH$, trong đó H là một $(D$, A)-sub-bimodule của $S^*$. Vì $S^*$ là một A-môđun phải đơn (VIII, p. 380, Định lý 1, c)), ta có H = 0 hoặc $H = S^*$; suy ra mệnh đề.

Đồng cấu $\lambda_S$ là $(A$, A)-linear và khác không; vì $S\otimes_DS^*$ là một song môđun đơn, $\lambda_S$ là đơn ánh (VIII, p. 47, Mệnh đề 2, a)).

#### Nhận xét {#alg-viii-s20-n5-rem-1 .statement tag=00MR}

Khi trường K đóng đại số, ta có D = K theo Định lý 1 của VIII, p. 47, và $\lambda_S$ là một đẳng cấu của $(A$, A)-bimodules từ $S\otimes_KS^*$ đến $\Theta_S(A)$.

### 6. Đặc trưng của một biểu diễn

Cho E là một A-môđun trái có số chiều hữu hạn trên K. Đặc trưng của E hay vết của E, ký hiệu bởi Tr$_E$, là dạng tuyến tính $a\mapsto$ Tr($a_E$). Cho $(e_1, . . . , e_n)$ là một cơ sở của E và $(e^*_1, . . . , e^*_n)$ là cơ sở đối ngẫu của nó. Theo định nghĩa, ta có quan hệ

(7) Tr$_E=\sum_{i=1}^nc_E(e_i, e^*_i)$.

Dạng tuyến tính Tr$_E$ thuộc $\Theta_E(A)$. Ta có Tr$_E=$ Tr$_{E'}$ nếu E và $E'$ là hai A-môđun đẳng cấu. Do đó Tr$_E$ chỉ phụ thuộc vào lớp đẳng cấu của E.

Cho $\pi$ là một biểu diễn tuyến tính của A trong một không gian vectơ V có số chiều hữu hạn trên K. Vết của $\pi$, hay đôi khi đặc trưng của $\pi$, được định nghĩa là đặc trưng của A-môđun $V_{\pi}$. Ta ký hiệu nó bởi Tr$_{\pi}$. Nếu $(e_1, . . . , e_n)$ là một cơ sở của V trên K và nếu $(\pi_{ij}(a))$ là ma trận của $\pi (a)$ theo cơ sở này, thì ta có

(8) Tr$_{\pi}(a) =\sum_{i=1}^n\pi_{ii}(a)$.

Dạng tuyến tính Tr$_{\pi}$ thuộc $\Theta_{\pi}(A)$.

#### Mệnh đề 5 {#alg-viii-s20-prop-5 .statement tag=00MS}

Cho S là một A-môđun đơn có số chiều hữu hạn trên K, cho D là trường đối của hoán tập của S, và cho Z là tâm của D. Các tính chất sau là tương đương:

(i) Đặc trưng Tr$_S$ của S khác không.

(ii) Tồn tại một phần tử $d\in D$ sao cho Tr$_{D/K}(d)\not= 0$.

(iii) Mở rộng Z của K là tách được, và đặc số $p$ của K không chia hết cho bậc [D : Z].

Trong đó, không gian vectơ phải trên D S hữu hạn chiều. Cho $(e_1, . . . , e_n)$ là một cơ sở của S trên D, và cho $u$ là một phần tử của End$_D(S)$. Cho $(d_{ij})$ là ma trận của $u$ đối với cơ sở $(e_1, . . . , e_n)$. Ta có $u(e_j) =\sum^n_{i=1}e_id_{ij}$ với $j\in [1, n]$. Ký hiệu $u_K$ là ánh xạ $u$ được xem như một tự đồng cấu của không gian vectơ trên K S và $(u_{ij})$ là ma trận của $u_K$ đối với phân tích $(e_iD)$ của không gian vectơ trên K S thành một tổng trực tiếp (II, §10, No. 5, p. 346). Ta có Tr($u_K$) $=\sum_i$ Tr($u_{ii}$). Hơn nữa, $u_{ii}$ là tự đồng cấu của không gian vectơ trên K $e_iD$ được xác định bởi $u_{ii}(e_id) =e_id_{ii}d$ với $d\in D$, nên vết của nó bằng Tr$_{D/K}(d_{ii})$. Vậy ta đã chứng minh đẳng thức

(9) Tr($u_K$) $=$ Tr$_{D/K}(\sum_id_{ii})$.

Theo định lý Burnside (VIII, p. 83, Hệ quả 1 của Mệnh đề 4), ánh xạ $a\mapsto a_S$ từ A đến End$_D(S)$ là toàn ánh. Do đó, tính tương đương của các tính chất (i) và (ii) suy ra từ công thức (9).

Nếu mở rộng Z của K là tách được, thì tồn tại một phần tử $d\in Z$ sao cho Tr$_{Z/K}(d)\not= 0$ (V, §8, No. 2, p. 49, Hệ quả của Mệnh đề 1). Hơn nữa, ta có Tr$_{D/K}(d) = [D : Z]$ Tr$_{Z/K}(d)$ (III, §9, No. 4, p. 548, Hệ quả); do đó, nếu $p$ không chia hết [D : Z], thì ta có Tr$_{D/K}(d)\not=$ 0. Điều này chứng tỏ rằng (iii) suy ra (ii).

Nếu mở rộng Z của K không tách được, thì ta có Tr$_{Z/K}(x) = 0$ với mọi $x\in Z$, và do đó Tr$_{D/K}(d) =$ Tr$_{Z/K}$(Tr$_{D/Z}(d)$) $= 0$ với mọi $d\in D$.

Bây giờ giả sử rằng $p$ chia hết bậc [D : Z]. Khi đó nó chia hết bậc rút gọn của D trên Z. Với mọi $d\in D$, ta có Tr$_{D/Z}(d) = 0$ (VIII, p. 344, Nhận xét), và do đó Tr$_{D/K}(d) =$ Tr$_{Z/K}$(Tr$_{D/Z}(d)$) $= 0$. Điều này hoàn tất chứng minh của hàm ý (ii) $\Rightarrow$ (iii).

#### Hệ quả {#alg-viii-s20-n6-cor-1 .statement tag=00MT}

Nếu trường K hoàn hảo, thì các tính chất (i) đến (iii) đều đúng.

Vì trường là hoàn hảo, nên mở rộng Z của K là tách được (V, §15, No. 5, p. 125, Định lý 3). Khi đó tính chất (iii) suy ra từ Hệ quả 3 của VIII, p. 323.

#### Mệnh đề 6 {#alg-viii-s20-prop-6 .statement tag=00MU}

Cho $\mathscr{S}_0$ là tập hợp các lớp của các A-môđun đơn hữu hạn chiều trên K có vết khác không. Họ các dạng tuyến tính (Tr$_S$)$_{S\in\mathscr{S}_0}$ là tự do trên K.

Cho $F$ là một tập con hữu hạn của $\mathscr{S}_0$, và cho $S$ là một phần tử của $F$. Theo giả thiết, tồn tại một phần tử $a\in A$ sao cho Tr$_S(a)\not= 0$. Theo Hệ quả 1 của Mệnh đề 4 (VIII, p. 83), tồn tại một phần tử $b\in A$ sao cho $b_S=a_S$ và $b_T= 0$ với mọi $T\in F-\{S\}$. Ta có Tr$_S(b)\not= 0$ và Tr$_T(b) = 0$ với $T\in F-\{S\}$. Vì vậy họ (Tr$_S$)$_{S\in F}$ là độc lập tuyến tính. Suy ra Mệnh đề 6.

#### Nhận xét {#alg-viii-s20-n6-rem-1 .statement tag=00RR}

Cho $\mathscr{S}_K$ là tập các lớp của các A-môđun đơn có số chiều hữu hạn trên K. Mệnh đề 6 cũng suy ra từ तथ्य rằng tổng của các $\Theta_S$(A), với S chạy qua $\mathscr{S}_K$, là trực tiếp.

Cho

$$
0\longrightarrow E'\longrightarrow E\longrightarrow E''\longrightarrow 0
$$

là một dãy khớp của các A-môđun, tất cả đều hữu hạn chiều trên K. Theo Mệnh đề 1 của III, §9, No. 2, p. 543, ta có Tr$_E=$ Tr$_{E'}+$ Tr$_{E''}$. Theo định nghĩa của nhóm Grothendieck $R_K(A)$ (VIII, p. 194) và tính chất phổ quát của nó (VIII, p. 186, Mệnh đề 4), tồn tại một đồng cấu của các nhóm cộng $\theta$ từ $R_K(A)$ đến $A^*$ được đặc trưng bởi quan hệ $\theta ([E]) =$ Tr$_E$ với mọi A-môđun E có số chiều hữu hạn trên K. Đặc biệt, vết của một sự nửa đơn hóa của E bằng với vết của E. Từ $\theta$ ta suy ra một ánh xạ K-tuyến tính $\theta_K: K\otimes_{\mathbf{Z}}R_K(A)\rightarrow A^*$.

#### Hệ quả {#alg-viii-s20-n6-cor-2 .statement tag=00MV}

a) Giả sử trường K có đặc số 0. Các đồng cấu $\theta$ và $\theta_K$ là đơn ánh. Hai A-môđun nửa đơn có số chiều hữu hạn trên K là đẳng cấu khi và chỉ khi các ký tự của chúng bằng nhau.

b) Giả sử trường K là hoàn hảo và có đặc số khác không $p$. Khi đó đồng cấu $\theta_K$ là đơn ánh, và hạt nhân của $\theta$ là $pR_K(A)$. Cho E là một A-môđun nửa đơn có số chiều hữu hạn trên K. Dạng tuyến tính Tr$_E$ bằng không khi và chỉ khi tồn tại một A-môđun F sao cho E đẳng cấu với $F^p$.

Cho $\mathscr{S}_K$ là tập các lớp của các A-môđun đơn có số chiều hữu hạn trên K. Các phần tử [S], với S chạy qua $\mathscr{S}_K$, lập thành một cơ sở của $\mathbf{Z}$-môđun $R_K$(A), nên các phần tử $1\otimes [S]$ lập thành một cơ sở của không gian vectơ trên K $K\otimes_{\mathbf{Z}}R_K(A)$ (VIII, p. 195).

Giả sử trường K là hoàn hảo. Theo Mệnh đề 6 và hệ quả của VIII, p. 383, các phần tử $\theta ([S]) =\theta_K(1\otimes [S]) =$ Tr$_S$ của $A^*$ là độc lập tuyến tính trên K. Suy ra đồng cấu $\theta_K$ là đơn ánh và hạt nhân của đồng cấu $\theta$ gồm các phần tử $\sum_{S\in\mathscr{S}_K}n_S[S]$ của $R_K(A)$ sao cho $n_S\cdot 1_K= 0$ với mọi $S\in \mathscr{S}_K$. Vì vậy hạt nhân của $\theta$ bằng $pR_K$(A), trong đó $p$ là đặc số của K. Đặc biệt, nếu K có đặc số 0, thì đồng cấu $\theta$ là đơn ánh.

Khẳng định cuối cùng của a) suy ra từ hệ quả của VIII, p. 190.

Giả sử rằng các giả thiết của b) được thỏa mãn, và cho E là một A-môđun nửa đơn có số chiều hữu hạn trên K. Nếu tồn tại một A-môđun F sao cho E là tổng trực tiếp của $p$ môđun con đẳng cấu với F, thì môđun F là nửa đơn và có số chiều hữu hạn trên K và ta có Tr$_E=p$ Tr$_F= 0$. Ngược lại, giả sử Tr$_E= 0$. Ta có $[E]\in pR_K$(A), nên bội số của mọi môđun đơn $S\in \mathscr{S}_K$ trong E là một bội của $p$ (VIII, p. 190, Mệnh đề 7); ta có thể viết nó dưới dạng $p n_S$ với $n_S\in \mathbf{N}$. Họ $(n_S)$ có giá hữu hạn. Đặt $F =\oplus_{S\in\mathscr{S}_K}S^{n_S}$. Khi đó ta có $[E] = [F^p]$, do đó E và $F^p$ đẳng cấu (VIII, p. 190, Hệ quả).

Cho E là một A-môđun có số chiều hữu hạn trên K. Cho $a\in A$. Ký hiệu $\chi_E(a; T)$ là định thức của tự đồng cấu $1_E+ Ta_E$ của K[T]-môđun $E[T] = K[T]\otimes_KE$ (III, §8, No. 11, p. 541). Ta có quan hệ

(10) $\chi_E(a; T)\equiv 1 +$ Tr$_E(a)T$ (mod $T^2K[T]$)

(loc. cit., công thức (49)). Vì đa thức này có số hạng hằng bằng 1, nên nó là một chuỗi lũy thừa hình thức khả nghịch (IV, §4, No. 4, p. 30). Hơn nữa, nếu

$$
0\longrightarrow E'\longrightarrow E\longrightarrow E''\longrightarrow 0
$$

là một dãy khớp của các A-môđun, đều có số chiều hữu hạn trên K, thì ta có $\chi_E(a; T) =\chi_{E'}(a; T)\chi_{E''}(a,T)$ (III, §8, No. 7, p. 534, công thức (31)). Theo định nghĩa của nhóm Grothendieck $R_K(A)$ (VIII, p. 194) và tính chất phổ quát của nó (VIII, p. 186, Mệnh đề 4), tồn tại một đồng cấu duy nhất $\chi_a$ từ nhóm $R_K(A)$ đến nhóm nhân 1 + TK[[T]] sao cho $\chi_a([E]) =\chi_E(a; T)$ với mọi A-môđun E có số chiều hữu hạn trên K. Từ công thức (10) suy ra quan hệ

(11) $\chi_a(x)\equiv 1 +\theta (x)(a)T$ (mod $T^2K[[T]]$)

cho $x\in R_K(A)$ và $a\in A$.

Nếu E và $E'$ là hai A-môđun có số chiều hữu hạn trên K với các phần nửa đơn đẳng cấu, thì ta có $\chi_E(a; T) =\chi_{E'}(a; T)$.

#### Định lý 2 {#alg-viii-s20-thm-2 .statement tag=00MW}

Cho $\mathscr{A}$ là một tập con sinh của không gian vectơ trên K A. Đồng cấu $\chi_{\mathscr{A}}: R_K(A)\rightarrow$ (1 + TK[[T]])$^{\mathscr{A}}$ được xác định bởi quan hệ $\chi_{\mathscr{A}}(x) = (\chi_a(x))_{a\in\mathscr{A}}$ là đơn ánh.

Cho $x$ là một phần tử của $R_K(A)$ sao cho $\chi_{\mathscr{A}}(x) = 1$. Theo (11), ta có $\theta (x)(a) = 0$ với mọi $a\in \mathscr{A}$, và do đó $\theta (x) = 0$ vì $\theta (x)$ là một dạng tuyến tính K trên A và $\mathscr{A}$ sinh không gian vectơ trên K A. Nếu đặc số của K bằng không, thì điều này suy ra $x= 0$ (VIII, p. 384, Hệ quả của Mệnh đề 6), và do đó kết quả trong trường hợp này. Giả sử từ nay trở đi rằng đặc số $p$ của K khác không.

Trước hết xét trường hợp khi K đóng đại số. Theo trên và loc. cit., khi đó ta có $x\in pR_K(A)$. Cho $y\in R_K(A)$ sao cho $x=py$. Với mỗi phần tử $a$ của $\mathscr{A}$, ta có $\chi_a(y)^p=\chi_a(py) =\chi_a(x) = 1$. Do đó ta có $(\chi_a(y)-1)^p= 0$, và vì vậy $\chi_a(y) = 1$ vì vành K[[T]] là một miền nguyên. Vậy $ y $ thuộc hạt nhân của tự đồng cấu $ \chi_{\mathscr{A}} $. Suy ra bằng quy nạp rằng $ x $ thuộc $ p^n R_K(A) $ với mọi số nguyên $ n \geq 1 $. Vì $ R_K(A) $ là một $ \mathbf{Z} $-môđun tự do, điều này suy ra $ x = 0 $, và do đó $\chi_{\mathscr{A}}$ là đơn ánh trong trường hợp này.

Nếu không còn giả sử K đóng đại số nữa, thì ta chọn một bao đóng đại số $ \overline{K} $ của K và xét biểu đồ các nhóm và các đồng cấu nhóm

$$
\begin{array}{ccc}
R_K(A) & \xrightarrow{\chi_{\mathscr{A}}} & (1 + TK[[T]])^{\mathscr{A}} \\
|_u & & |_i \\
R_{\overline{K}}(A_{(\overline{K})}) & \xrightarrow{\overline{\chi}_{\mathscr{A}}} & (1 + T\overline{K}[[T]])^{\mathscr{A}},
\end{array}
$$

trong đó $ u $ là đồng cấu suy ra từ phép mở rộng vô hướng từ $ K $ đến $ \overline{K} $ (VIII, p. 195), $ i $ là đơn ánh chính tắc, và $ \overline{\chi}_{\mathscr{A}} $ là đồng cấu $ z \mapsto (\chi_{1 \otimes a}(z))_{a \in \mathscr{A}} $. Theo công thức (12) của III, §9, No. 1, p. 542, biểu đồ (12) giao hoán. Theo trên, đồng cấu $ \overline{\chi}_{\mathscr{A}} $ là đơn ánh. Vì $ u $ là đơn ánh (VIII, p. 195, Định lý 1), nên đồng cấu $ \chi_{\mathscr{A}} $ là đơn ánh.

#### Hệ quả 1 {#alg-viii-s20-thm-2-cor-1 .statement tag=00MX}

*Cho E và F là các A-môđun nửa đơn có chiều hữu hạn trên K, và cho $ \mathscr{A} $ là một tập con sinh của không gian vectơ trên K A. Giả sử rằng với mọi $ a \in \mathscr{A} $, các đa thức đặc trưng của các tự đồng cấu $ a_E $ và $ a_F $ của các không gian vectơ trên K E và F bằng nhau. Khi đó các A-môđun E và F đẳng cấu với nhau.*

Cho $ a $ là một phần tử của $ \mathscr{A} $. Các đa thức đặc trưng của $ a_E $ và $ a_F $ có cùng bậc, nên chiều của E bằng chiều của F; ta ký hiệu nó là $ n $. Ký hiệu $ \mathrm{Pc}_E(a; T) $ là đa thức đặc trưng của $ a_E $. Trong $ K(T) $, ta có các đẳng thức

$$
\chi_E(a; T) = \det(1 + a_E T) = (-T)^n \det \left( \frac{-1}{T} - a_E \right) = (-T)^n \mathrm{Pc}_E \left( a; \frac{-1}{T} \right),
$$

và $ \chi_F(a; T) $ được cho bởi một công thức tương tự. Do các giả thiết của chúng ta, ta có $ \chi_E(a; T) = \chi_F(a; T) $. Theo Định lý 2, ta có [E] = [F], điều đó suy ra E và F đẳng cấu (VIII, p. 190, Hệ quả của Mệnh đề 7).

#### Hệ quả 2 {#alg-viii-s20-thm-2-cor-2 .statement tag=00MY}

*Cho A là một đại số đơn tâm có bậc hữu hạn trên K. Cho B là một K-đại số nửa đơn, cho f và g là các đồng cấu đại số từ B đến A, và cho $ \mathscr{B} $ là một tập con sinh của không gian vectơ trên K B. Các tính chất sau là tương đương:

(i) Tồn tại một tự đẳng cấu trong $ \theta $ của A sao cho $ g = \theta \circ f $.
(ii) Với mọi $ b \in \mathscr{B} $, ta có $ \mathrm{Pc}_{A/K}(f(b); X) = \mathrm{Pc}_{A/K}(g(b); X) $.* Khi K có đặc số không, các tính chất này tương đương với điều sau:

(iii) Với mọi $b\in \mathscr{B}$, ta có Tr$_{A/K}(f(b)) =$ Tr$_{A/K}(g(b))$.

Ký hiệu M và N là các B-môđun trái thu được bằng cách trang bị cho nhóm cộng của A các luật ngoài $(b, a)\mapsto f(b)a$ và $(b, a)\mapsto g(b)a$, tương ứng. Theo Mệnh đề 1 của VIII, p. 257, tính chất (i) tương đương với việc các B-môđun M và N đẳng cấu. Theo cách dựng, phép vị tự $b_M$ liên kết với một phần tử $b$ của B là phép nhân trái bởi $f(b)$ trong A; do đó, ta có các đẳng thức

Pc$_M(b; X) =$ Pc$_{A/K}(f(b); X)$,

Tr$_M(b) =$ Tr$_{A/K}(f(b))$

và hai quan hệ tương tự trong đó thay M bằng N và $f$ bằng $g$. Chúng ta biết (VIII, p. 386, Hệ quả 1) rằng các B-môđun M và N đẳng cấu khi và chỉ khi ta có Pc$_M(b; X) =$ Pc$_N(b; X)$ với mọi $b\in \mathscr{B}$. Khi trường K có đặc số 0, quan hệ này cũng tương đương với Tr$_M(b) =$ Tr$_N(b)$ với mọi $b\in \mathscr{B}$ (VIII, p. 384, Hệ quả của Mệnh đề 6). Suy ra sự tương đương của các tính chất (i) và (ii), và cả của (i) và (iii) khi K có đặc số 0.

### 7. Các hệ số của một tập các lớp môđun

Cho $\mathscr{C}$ là một tập di truyền các lớp của A-môđun (VIII, p. 183, Định nghĩa 1). Giả sử rằng mọi A-môđun kiểu $\mathscr{C}$ đều hữu hạn chiều trên K và ký hiệu $\Theta_{\mathscr{C}}(A)$ là tập các hệ số của các A-môđun kiểu $\mathscr{C}$. Theo Mệnh đề 2 của VIII, p. 378, tập $\Theta_{\mathscr{C}}(A)$ cũng là hợp của các ảnh của các ánh xạ A-tuyến tính $u: E\rightarrow A^*$, trong đó E chạy qua $\mathscr{C}$; nó cũng là hợp của các không gian con $\Theta_E(A)$ của $A^*$, trong đó E chạy qua $\mathscr{C}$ (loc. cit.). Họ các (A, A)-môđun con song $(\Theta_E(A))_{E\in\mathscr{C}}$ của $A^*$ là có hướng, nên hợp của nó $\Theta_{\mathscr{C}}(A)$ là một (A, A)-môđun con song của $A^*$.

#### Mệnh đề 7 {#alg-viii-s20-prop-7 .statement tag=00MZ}

Một A-môđun con trái của $A^*$ có số chiều hữu hạn trên K được chứa trong $\Theta_{\mathscr{C}}(A)$ khi và chỉ khi nó có kiểu $\mathscr{C}$.

Cho V là một A-môđun con trái của $A^*$ có số chiều hữu hạn trên K. Ta đã thấy trong VIII, p. 379, Nhận xét 3 rằng ta có $V\subset \Theta_V(A)$. Nếu V có kiểu $\mathscr{C}$, thì ta có $\Theta_V(A)\subset \Theta_{\mathscr{C}}$ (A), nên V được chứa trong $\Theta_{\mathscr{C}}(A)$. Ngược lại, giả sử rằng V được chứa trong $\Theta_{\mathscr{C}}(A)$. Vì $\Theta_{\mathscr{C}}(A)$ là hợp của họ có hướng $(\Theta_E(A))_{E\in\mathscr{C}}$ và V có số chiều hữu hạn trên K, tồn tại một môđun E có kiểu $\mathscr{C}$ sao cho V được chứa trong $\Theta_E(A)$. Bây giờ, tồn tại một số tự nhiên $n$ sao cho $\Theta_E(A)$ đẳng cấu với một thương của $E^n$ (VIII, p. 378, Mệnh đề 2). Vì $\mathscr{C}$ là di truyền, V có kiểu $\mathscr{C}$.

#### Hệ quả {#alg-viii-s20-n7-cor-1 .statement tag=00N0}

Cho E là một A-môđun có số chiều hữu hạn trên K. Khi đó E có kiểu $\mathscr{C}$ khi và chỉ khi $\Theta_E(A)$ được chứa trong $\Theta_{\mathscr{C}}(A)$.

Điều kiện này hiển nhiên là cần.

Ngược lại, giả sử rằng $\Theta_{\mathscr{C}}(A)$ chứa $\Theta_E(A)$. A-môđun $\Theta_E(A)$ có số chiều hữu hạn trên K (VIII, p. 378, Mệnh đề 2), nên nó có kiểu $\mathscr{C}$ theo Mệnh đề 7. Bây giờ, tồn tại một số nguyên $n\geqslant 0$ sao cho E đẳng cấu với một A-môđun con của $\Theta_E(A)^n$ (VIII, p. 378, Mệnh đề 2). Vì $\mathscr{C}$ là di truyền, E có kiểu $\mathscr{C}$.

### 8. Cấu trúc cođại số trên đối ngẫu hạn chế

Đối với mọi $a$ trong A, ta ký hiệu $\eta (a)$ là dạng tuyến tính $f\mapsto f(a)$ trên Θ(A). Vậy ta định nghĩa một ánh xạ K-tuyến tính $\eta$ từ A đến đối ngẫu $\Theta (A)^*$ của không gian vectơ Θ(A). Đặt $\varepsilon =\eta (1)$.

#### Mệnh đề 8 {#alg-viii-s20-prop-8 .statement tag=00N1}

Trên không gian vectơ Θ(A), tồn tại một cấu trúc cođại số duy nhất (III, §11, No. 1, p. 574) sao cho ánh xạ $\eta : A\rightarrow \Theta (A)^*$ là một đồng cấu từ A đến đại số đối ngẫu (III, §11, No. 2, p. 579) của Θ(A). Cấu trúc cođại số Θ(A) là đồng kết hợp và nhận $\varepsilon$ làm một đồng đơn vị.

Với mọi số nguyên $n\geqslant 1$, xét ánh xạ K-tuyến tính $j_n$ từ $\Theta (A)^{\otimes n}$ đến đối ngẫu của $A^{\otimes n}$ được đặc trưng bởi công thức

$$
\langle j_n(f_1\otimes  \cdots  \otimes f_n), a_1\otimes  \cdots  \otimes a_n\rangle =\prod_{i=1}^n\langle f_i, a_i\rangle \tag{13}
$$

với $(a_i)$ trong $A^n$ và $(f_i)$ trong $\Theta (A)^n$. Theo Mệnh đề 16, (ii) của II, §7, No. 7, p. 308, ánh xạ $j_n$ là đơn ánh. Ký hiệu $m_K: K\otimes K\rightarrow K$ và $m_A: A\otimes A\rightarrow A$ là các ánh xạ suy ra từ phép nhân trong K và A, tương ứng. Với $f, g\in \Theta (A)$ và $a, b\in A$, ta có

$$
\langle j_2(f\otimes g), a\otimes b\rangle =m_K\circ (\eta (a)\otimes \eta (b))(f\otimes g)
$$

Do đó ta có

$$
\langle j_2(t), a\otimes b\rangle =m_K\circ (\eta (a)\otimes \eta (b))(t) \tag{14}
$$

với mọi $t\in \Theta (A)\otimes \Theta (A)$.

#### Bổ đề 2 {#alg-viii-s20-lem-2 .statement tag=00RS}

Cho $ c : \Theta(A) \to \Theta(A) \otimes \Theta(A) $ là một ánh xạ K-tuyến tính. Khi đó $ \eta $ là một đồng cấu từ $ A $ đến đại số đối ngẫu của cấu trúc cođại số $ (\Theta(A), c) $ khi và chỉ khi biểu đồ sau giao hoán:

$$
\begin{array}{ccc}
\Theta(A) & \xrightarrow{c} & \Theta(A) \otimes \Theta(A) \\
| & & | \\
A^* & \xrightarrow{t m_A} & (A \otimes A)^*
\end{array}
$$

Quả vậy, $ \eta $ là một đồng cấu từ $ A $ đến đại số đối ngẫu của cấu trúc cođại số $ (\Theta(A), c) $ khi và chỉ khi ta có $ \eta(ab) = m_K \circ (\eta(a) \otimes \eta(b)) \circ c $ với mọi $ a, b \in A $, tức là

$$
\eta(ab)(f) = m_K \circ (\eta(a) \otimes \eta(b))(c(f))
$$

với $ a, b \in A $ và $ f \in \Theta(A) $. Bây giờ, ta có

$$
\eta(ab)(f) = f(ab) = \langle t m_A(j_1(f)), a \otimes b \rangle
$$

và, theo (14),

$$
m_K \circ (\eta(a) \otimes \eta(b))(c(f)) = \langle j_2(c(f)), a \otimes b \rangle
$$

với mọi $ a, b \in A $ và mọi $ f \in \Theta(A) $. Bổ đề được suy ra.

Vì $ j_2 $ là đơn ánh, tồn tại nhiều nhất một ánh xạ tuyến tính $ c $ làm cho biểu đồ trên giao hoán. Để chứng minh sự tồn tại của nó, ta phải chứng minh rằng ảnh của $ t m \circ j_1 $ được chứa trong ảnh của $ j_2 $. Nói cách khác, ta phải chứng minh rằng, với mọi phần tử $ f $ của $ \Theta(A) $, tồn tại một số tự nhiên $ n $ và các phần tử $ f'_1, \ldots, f'_n, f''_1, \ldots, f''_n $ của $ \Theta(A) $ thỏa mãn các hệ thức

$$
f(ab) = \sum_{i=1}^n f'_i(a) f''_i(b)
$$

với $ a, b \in A $. Khi đó ta sẽ có

$$
c(f) = \sum_{i=1}^n f'_i \otimes f''_i.
$$

Theo hệ quả của VIII, p. 379, tồn tại một $ A $-môđun trái $ E $ có số chiều hữu hạn trên $ K $ với $ f $ là một hệ số. Cho $ (e_1, \ldots, e_n) $ là một cơ sở của $ E $, $ (e_1^*, \ldots, e_n^*) $ là cơ sở đối ngẫu, $ x $ là một phần tử của $ E $, và $ x^* $ là một phần tử của $ E^* $ sao cho $ f = c_E(x, x^*) $. Đặt $ f'_i = c_E(e_i, x^*) $ và $ f''_i = c_E(x, e_i^*) $ với $ i \in [1, n] $; với a, b trong A, ta có

$$
f(ab) = \langle x^*, abx \rangle = \langle x^* a, bx \rangle = \left\langle \sum_i \langle x^* a, e_i \rangle e_i^*, bx \right\rangle
$$
$$
= \sum_i \langle x^* a, e_i \rangle \langle e_i^*, bx \rangle = \sum_i \langle x^*, ae_i \rangle \langle e_i^*, bx \rangle = \sum_i f_i'(a) f_i''(b),
$$
và do đó (16).

Ta chứng minh tính đồng kết hợp của c. Với điều đó, xét các ánh xạ K-tuyến tính
$$
c' = (c \otimes 1_{\Theta(A)}) \circ c \quad \text{và} \quad c'' = (1_{\Theta(A)} \otimes c) \circ c
$$
từ $ \Theta(A) $ đến $ \Theta(A)^{\otimes 3} $. Ta có các quan hệ
$$
\langle j_3(f \otimes c(g)), a \otimes b \otimes c \rangle = \langle f, a \rangle \langle j_2 \circ c(g), b \otimes c \rangle
$$
$$
= \langle f, a \rangle \langle g, bc \rangle
$$
$$
= \langle j_2(f \otimes g), a \otimes bc \rangle
$$
$$
= \langle t(\mathrm{Id}_A \otimes m_A) \circ j_2(f \otimes g), a \otimes b \otimes c \rangle
$$
với $ f, g \in \Theta(A) $ và $ a, b, c \in A $. Từ đó, suy ra biểu đồ sau giao hoán:

$$
\begin{array}{ccc}
\Theta(A) \otimes \Theta(A) & \xrightarrow{\mathrm{Id}_{\Theta(A)} \otimes c} & \Theta(A) \otimes \Theta(A) \otimes \Theta(A) \\
\downarrow j_2 & & \downarrow j_3 \\
(A \otimes A)^* & \xrightarrow{t(\mathrm{Id}_A \otimes m_A)} & (A \otimes A \otimes A)^*.
\end{array}
$$

Nhờ tính giao hoán của biểu đồ này và của (15), với $ f \in \Theta(A) $ và $ a, a', a'' \in A $, ta có
$$
\langle j_3 \circ c'(f), a \otimes a' \otimes a'' \rangle = \langle f, (aa')a'' \rangle;
$$
ta cũng có thể chứng minh quan hệ
$$
\langle j_3 \circ c''(f), a \otimes a' \otimes a'' \rangle = \langle f, a(a'a'') \rangle
$$
tương tự. Vì phép nhân trong A là kết hợp, ta có $ j_3 \circ c' = j_3 \circ c'' $, và do đó $ c' = c'' $ vì $ j_3 $ là đơn ánh.

Cuối cùng, các công thức (16) và (17) suy ra rằng $ \Theta(A) $ nhận $ \varepsilon $ làm một đồng đơn vị.

#### Nhận xét 1 {#alg-viii-s20-n8-rem-1 .statement tag=00N2}

Cho $ (\mathbf{V}, \pi) $ là một biểu diễn tuyến tính hữu hạn chiều của đại số A. Hãy đưa vào một cơ sở $ (e_1, \ldots, e_n) $ của V và cơ sở đối ngẫu $ (e_1^*, \ldots, e_n^*) $ của $ \mathbf{V}^* $. Theo chứng minh của Bổ đề 2, ta có quan hệ
$$
c(c_\pi(x, x^*)) = \sum_{k=1}^n c_\pi(e_k, x^*) \otimes c_\pi(x, e_k^*)
$$

với $x\in V$ và $x^*\in V^*$. Với $1\leqslant i, j\leqslant n$, đặt $\pi_{ij}=c_{\pi}(e_j, e^*_i)$. Với mọi $a\in A$, ma trận của $\pi (a)$ theo cơ sở $(e_1, . . . , e_n)$ của V bằng $(\pi_{ij}(a))$. Với $1\leqslant i\leqslant n$ và $1\leqslant j\leqslant n$, khi đó ta có

$$
c(\pi_{ij}) =\sum_{k=1}^n\pi_{ik}\otimes \pi_{kj} \tag{20}
$$

#### Định nghĩa 3 {#alg-viii-s20-def-3 .statement tag=00N3}

Cho C là một đối đại số trên trường K và c là đồng tích của nó. Một đối đại số con của C là bất kỳ không gian con tuyến tính $C_1$ của C sao cho $c(C_1)$ được chứa trong ảnh chính tắc của $C_1\otimes_KC_1$ trong $C\otimes_KC$.

Cho $j$ là đơn ánh chính tắc của $C_1$ vào C. Theo định nghĩa này, tồn tại duy nhất một ánh xạ tuyến tính $c_1: C_1\rightarrow C_1\otimes_KC_1$ sao cho ta có

$$
c\circ j= (j\otimes j)\circ c_1 \tag{21}
$$

quan hệ này có nghĩa là $j$ là một cấu xạ của đối đại số từ $(C_1, c_1)$ đến $(C, c)$ (III, §11, No. 1, p. 574).

Nếu C đồng kết hợp, thì $C_1$ cũng đồng kết hợp. Nếu C đồng giao hoán, thì $C_1$ cũng vậy. Nếu C có một đồng đơn vị $\varepsilon$, thì hạn chế của $\varepsilon$ lên $C_1$ là một đồng đơn vị của $C_1$.

#### Mệnh đề 9 {#alg-viii-s20-prop-9 .statement tag=00N4}

Cho Θ là một không gian con tuyến tính của Θ(A). Các tính chất sau là tương đương:

(i) Θ là một $(A,A)$-sub-bimodule của Θ(A).

(ii) Θ là một đối đại số con của Θ(A).

(iii) Tồn tại một tập di truyền $\mathscr{C}$ các lớp của các A-môđun có số chiều hữu hạn trên K sao cho $\Theta  = \Theta_{\mathscr{C}}(A)$.

Khi các tính chất này đúng, tập $\mathscr{C}$ được nói đến trong (iii) được xác định duy nhất.

Khẳng định cuối cùng suy ra từ hệ quả của VIII, p. 388: tập $\mathscr{C}$ gồm các lớp của các A-môđun E có số chiều hữu hạn trên K sao cho $\Theta_E(A)$ được chứa trong Θ.

(iii) $\Rightarrow$ (ii): Cho $\mathscr{C}$ là một tập di truyền các lớp của các A-môđun có số chiều hữu hạn trên K. Khi đó $\Theta_{\mathscr{C}}(A)$ là hợp của họ có hướng $(\Theta_E(A))_{E\in\mathscr{C}}$. Vì $\Theta_E(A)$ là một đối đại số con của Θ(A) với mọi $E\in \mathscr{C}$ (VIII, p. 390, công thức (19)), nên điều tương tự đúng cho $\Theta_{\mathscr{C}}(A)$.

(ii) $\Rightarrow$ (i): Cho $f\in \Theta (A)$. Cho $f'_1, . . . , f'_n, f''_1, . . . , f''_n$ là các phần tử của Θ(A) thỏa mãn $c(f) =\sum f'_i\otimes f''_i$. Với $a,b$ trong A, ta có $f(ab) =\sum f'_i(a)f''_i(b)$, và do đó

$$
bf=\sum_{i=1}^nf''_i(b)f'_i,f a=\sum_{i=1}^nf'_i(a)f''_i
$$

(VIII, p. 375, các công thức (3) và (4)). Do đó, một đối đại số con của Θ(A) là một $(A$, A)-sub-bimodule.

(i) $\Rightarrow$ (iii): Giả sử Θ là một $(A$, A)-sub-bimodule của Θ(A); cho $\mathscr{C}$ là tập các lớp của các A-môđun E có số chiều hữu hạn trên K sao cho $\Theta_E(A)$ được chứa trong Θ. Tập $\mathscr{C}$ là di truyền (VIII, p. 377, Nhận xét 2), và theo phép dựng ta có $\Theta_{\mathscr{C}}(A)\subset \Theta$. Cho $f\in \Theta$ và $E = Af$. Khi đó E có số chiều hữu hạn trên K. Do đó, mọi dạng tuyến tính trên E đều có dạng $u_a:g\mapsto g(a)$ với $a$ trong A (II, §7, No. 5, p. 302, Hệ quả 2). Bây giờ, với $a, b, x\in A$, ta có

$$
c_E(af, u_b)(x) =\langle u_b, xaf\rangle =f(bxa) =af b(x)
$$

suy ra $c_E(af, u_b) =af b$. Vì thế ta có $\Theta_E(A)\subset \Theta$. Do đó, A-môđun E là kiểu $\mathscr{C}$, và $f$ là một trong các hệ số của nó. Vì thế ta có $\Theta \subset \Theta_{\mathscr{C}}(A)$ và, sau cùng, $\Theta  = \Theta_{\mathscr{C}}(A)$.

#### Nhận xét 2 {#alg-viii-s20-n8-rem-2 .statement tag=00N5}

Cho Θ là một đối đại số con của Θ(A). Ta trang bị cho K tôpô rời rạc và đại số A tôpô thô nhất sao cho các ánh xạ $f: A\rightarrow K$ với $f$ chạy qua Θ là liên tục (Gen. Top., I, §2, No. 2, p. 175). Tôpô này trang bị cho A cấu trúc của một K-môđun tôpô. Một iđêan hai phía $\mathfrak{a}$ của A là mở nếu và chỉ nếu nó có đối chiều hữu hạn và phần trực giao $\mathfrak{a}'$ của nó được chứa trong Θ. Theo Mệnh đề 3 của VIII, p. 379, các iđêan hai phía mở của A tạo thành một hệ cơ bản các lân cận của 0 trong A. Vì thế tôpô trên A tương thích với cấu trúc vành của nó.

Cho $\mathscr{C}$ là tập di truyền các lớp của các A-môđun có số chiều hữu hạn trên K sao cho $\Theta  = \Theta_{\mathscr{C}}$ (VIII, p. 391, Mệnh đề 9). Cho E là một A-môđun trái có số chiều hữu hạn trên K. Ta trang bị cho nó tôpô rời rạc. Các tính chất sau là tương đương:

(i) A-môđun E là kiểu $\mathscr{C}$.

(ii) Linh hóa tử của A-môđun E là mở trong A.

(iii) Ánh xạ $(a, x)\mapsto ax$ từ $A\times E$ đến E là liên tục.

Tính chất cuối cùng có nghĩa là E là một A-môđun tôpô.

Let $\Theta^*$ be the đại số đối ngẫu của đối đại số Θ. Ta trang bị cho $\Theta^*$ tôpô thô nhất sao cho các ánh xạ $\varphi \mapsto \varphi (u)$ từ $\Theta^*$ đến K, với $u$ chạy qua Θ, là liên tục. Tôpô trên đại số $\Theta^*$ tương thích với cấu trúc nhóm cộng trên $\Theta^*$. Các trực giao trong $\Theta^*$ của các tập hợp dạng $\Theta_E$(A), trong đó E là một A-môđun kiểu $\mathscr{C}$, lập thành một hệ cơ bản các lân cận của 0. Bây giờ, một tập như vậy là một đối đại số con của Θ, nên trực giao của nó là một iđêan của $\Theta^*$. Do đó tôpô trên $\Theta^*$ tương thích với cấu trúc vành của nó. Đồng cấu đại số chính tắc $\eta : A\rightarrow \Theta^*$ (đưa $a\in A$ tới dạng tuyến tính $f\mapsto f(a)$ trên Θ) định nghĩa một đẳng cấu từ không gian Hausdorff hoàn thành $\widehat{A}$ của A (Gen. Top., II, §3, No. 7, p. 191) tới $\Theta^*$.

### Bài tập {#alg-viii-s20-exercises}

Xem [các bài tập của § 20](exercises/s20/).
