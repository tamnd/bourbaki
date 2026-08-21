---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Semisimple Modules and Rings
section: 2
section_title: Determinants over a Noncommutative Field
appendix: true
lang: vi
source: alg-viii
source_edition: 2023, Springer Nature
book_pages: A VIII.447-A VIII.460
pdf_pages: 0464-0477
extraction: native
subsections:
    - "no": 1
      title: A Generalization of Alternating Multilinear Forms
      page: 447
      pdf_page: 464
    - "no": 2
      title: A Uniqueness Theorem
      page: 448
      pdf_page: 465
    - "no": 3
      title: Determinant of an Automorphism
      page: 452
      pdf_page: 469
    - "no": 4
      title: Determinant of a Square Matrix
      page: 452
      pdf_page: 469
    - "no": 5
      title: The Unimodular Group
      page: 455
      pdf_page: 472
statements: 18
exercises: 4
content_sha256: d99e90ac0e691a6ff282b9fb540da55f46faf15f3a4a0c9a57c0fe94d569e6cb
translated_from: content/en/alg/VIII/A2_a2_determinants_over_a_noncommutative_field.md
source_content_sha256: a1a346c55a436d2ed8247c3e3a5bc5302eaac2c7930a98ff5617acbf65dc1b0e
translation_model: gpt-5-6, gpt-5-6-mini, gpt-5.4
translation_run: translate-vi-74c08a00
glossary_version: 34
glossary_terms_sha256: fac8e3f8e51a49ee7354f36800f1ebd6cda2f7907e3795e8dc0413508ead6d81
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## PHỤ LỤC 2 ĐỊNH THỨC TRÊN MỘT TRƯỜNG KHÔNG GIAO HOÁN

Trong phụ lục này, D là một trường, và $D^*_{ab}$ là thương của nhóm nhân $D^*$ của D theo nhóm dẫn xuất của nó (I, §6, No. 2, p. 70). Nhóm $D^*_{ab}$ là giao hoán, và $D^*_{ab}$ có thể được đồng nhất với $D^*$ nếu trường D là giao hoán. Ta ký hiệu đồng cấu chính tắc từ $D^*$ đến $D^*_{ab}$ bởi $\pi$.

### 1. Phép tổng quát hóa các dạng đa tuyến tính thay phiên

Cho V là một không gian vectơ phải trên trường D, có số chiều hữu hạn $n\geqslant 0$. Ta ký hiệu B(V) là tập hợp các cơ sở của V và Ω(V) là tập hợp các ánh xạ $\omega$ từ B(V) vào $D^*_{ab}$ thỏa mãn hai điều kiện sau:

a) Nếu $\lambda_1, . . . , \lambda_n$ là các phần tử của $D^*$, thì ta có

$$
\omega (v_1\lambda_1, . . . , v_n\lambda_n) =\pi (\lambda_1\cdots \lambda_n)\omega (v_1, . . . , v_n) \tag{1}
$$

với mọi cơ sở $(v_1, . . . , v_n)$ của V.

b) Nếu $i$ và $j$ là hai số nguyên phân biệt trong khoảng $[1, n]$, thì ta có

$$
\omega (v_1, . . . , v_{i-1}, v_i+v_j, v_{i+1}, . . . , v_n) =\omega (v_1, . . . , v_n) \tag{2}
$$

với mọi cơ sở $(v_1, . . . , v_n)$ của V.

Cho $\omega$ là một phần tử của Ω(V). Cho $(v_1, . . . , v_n)$ là một cơ sở của V và $i$ là một số nguyên trong khoảng $[1, n-1]$; theo tính chất b), ta có

$$
\omega (v_1, . . . , v_i, v_{i+1}, . . . , v_n) =\omega (v_1, . . . , v_i+v_{i+1}, v_{i+1}, . . . , v_n)
$$

$$
=\omega (v_1, . . . , v_i+v_{i+1}, v_{i+1}-(v_i+v_{i+1}), . . . , v_n)
$$

$$
=\omega (v_1, . . . , v_i+v_{i+1},-v_i, . . . , v_n)
$$

$$
=\omega (v_1, . . . ,(v_i+v_{i+1})-v_i,-v_i, . . . , v_n)
$$

và do đó

$$
\omega (v_1, . . . , v_i, v_{i+1}, . . . , v_n) =\pi (-1)\omega (v_1, . . . , v_{i+1}, v_i, . . . , v_n) \tag{3}
$$

Vì nhóm đối xứng $\mathfrak{S}_n$ được sinh bởi các phép chuyển chỗ của hai phần tử liên tiếp của khoảng $[1, n]$ (I, §5, No. 7, p. 63, Mệnh đề 9), công thức (3) được tổng quát hóa thành

$$
\omega (v_{\sigma(1)}, . . . , v_{\sigma(n)}) =\pi (\varepsilon (\sigma ))\omega (v_1, . . . , v_n) \tag{4}
$$

trong đó $\sigma$ thuộc $\mathfrak{S}_n$ và $\varepsilon (\sigma )$ là chữ ký của nó (I, §5, No. 7, p. 64).

Công thức (2) được tổng quát hóa như sau. Trước hết, với mọi $\lambda$ trong $D^*$, ta có

$$
\omega (v_1, . . . , v_n) =\pi (\lambda )\omega (v_1, . . . , v_i\lambda^{-1}, . . . , v_n)
$$

$$
=\pi (\lambda )\omega (v_1, . . . , v_i\lambda^{-1}+v_j, . . . , v_n)
$$

$$
=\omega (v_1, . . . ,(v_i\lambda^{-1}+v_j)\lambda , . . . , v_n)
$$

nghĩa là,

$$
\omega (v_1, . . . , v_n) =\omega (v_1, . . . , v_i+v_j\lambda , . . . , v_n) \tag{5}
$$

Bằng quy nạp ngay lập tức, ta suy ra

$$
\omega (v_1, . . . , v_n) =\omega (v_1, . . . , v_i+w, . . . , v_n) \tag{6}
$$

đối với mọi tổ hợp tuyến tính $w=\sum_{j\not=i}v_j\lambda_j$ của các vectơ $v_j$ với $j$ khác $i$ trong khoảng $[1, n]$.

### 2. Một Định lý về tính duy nhất

Trong tiểu mục này, với mọi số nguyên dương ngặt $m$, mọi số nguyên $i$ trong khoảng $[1, m]$, và mọi dãy $(v_1, . . . , v_m)$ trong $V^m$, ta ký hiệu $(v_1, . . . ,\widehat{v}_i, . . . , v_m)$ là dãy $(v_1, . . . , v_{i-1}, v_{i+1}, . . . , v_m)$ trong $V^{m-1}$.

#### Mệnh đề 1 {#alg-viii-a2-prop-1 .statement tag=00Q1}

Cho W là một siêu phẳng trong V và $e$ là một vectơ trong V- W. Cho $\varphi$ là một phần tử của Ω(W). Tồn tại một phần tử duy nhất $\omega$ của Ω(V) sao cho

$$
\omega (w_1, . . . , w_{n-1}, e) =\varphi (w_1, . . . , w_{n-1}) \tag{7}
$$

với mọi cơ sở $(w_1, . . . , w_{n-1})$ của W.

A) Tính duy nhất của $\omega :$ Cho $\omega$ là một phần tử của Ω(V). Cho $(v_1, . . . , v_n)$ là một cơ sở của V, và gọi $\mu_1, . . . , \mu_n$ là các tọa độ của $e$ trong cơ sở này. Ký hiệu bởi I tập hợp các số nguyên từ 1 đến $n$ (kể cả hai đầu mút) sao cho $\mu_i\not= 0$; tập hợp này không rỗng. Cho $i$ là một phần tử của I. Dãy $(v_1, . . . ,\widehat{v}_i, . . . , v_n, e)$ là một cơ sở của V, và vì $e-v_i\mu_i$ là một tổ hợp tuyến tính của dãy $(v_1, . . . ,\widehat{v}_i, . . . , v_n)$, công thức (6) suy ra

$$
\omega (v_1, . . . ,\widehat{v}_i, . . . , v_n, v_i\mu_i) =\omega (v_1, . . . ,\widehat{v}_i, . . . , v_n, e) \tag{8}
$$

Suy ra từ các công thức (1) và (3) rằng vế trái của đẳng thức này bằng $\pi (-1)^{n-i}\pi (\mu_i)\omega (v_1, . . . , v_n)$. Ký hiệu bởi $p$ phép chiếu của V có ảnh W và hạt nhân $eD$. Các vectơ $v_j-p(v_j)$ tỉ lệ với $e$, và việc áp dụng lặp đi lặp lại công thức (6) cho thấy rằng vế phải của công thức (8) bằng $\omega (p(v_1), . . . ,\widehat{p}(v_i), . . . , p(v_n), e)$.

Từ đó suy ra rằng nếu $\omega$ thỏa mãn quan hệ (7), thì ta có

$$
\omega (v_1, . . . , v_n) =\pi (-1)^{n-i}\pi (\mu_i)^{-1}\varphi (p(v_1), . . . ,\widehat{p}(v_i), . . . , p(v_n)) \tag{9}
$$

với mọi $i$ trong I, điều này chứng minh tính duy nhất của $\omega$.

B) Phép dựng của $\omega :$ Cho $(v_1, . . . , v_n)$ là một cơ sở của V; ta định nghĩa $\mu_1, . . . , \mu_n$ và I như trên. Với mọi $i$ trong I, giả thiết $\mu_i\not= 0$ suy ra rằng dãy $(v_1, . . . ,\widehat{v}_i, . . . , v_n, e)$ sinh ra không gian V, nên dãy $(p(v_1), . . . ,\widehat{p}(v_i), . . . , p(v_n))$ sinh ra không gian $W =p(V)$. Nói cách khác, dãy sau cùng này là một cơ sở của W, và

$$
t_i=\pi (-1)^{n-i}\pi (\mu_i)^{-1}\varphi (p(v_1), . . . ,\widehat{p}(v_i), . . . , p(v_n)) \tag{10}
$$

xác định một phần tử của $D^*_{ab}$.

Cho $i$ và $j$ là hai phần tử của I sao cho $i < j$; hãy chứng minh đẳng thức $t_i=t_j$. Theo định nghĩa, vectơ $v_i\mu_i+v_j\mu_j-e$ là một tổ hợp tuyến tính của các vectơ $p(v_k)$ với $k$ khác $i$ và $j$. Do đó, $p(v_i)\mu_i+p(v_j)\mu_j$ là một tổ hợp tuyến tính của các vectơ $p(v_k)$ với $k$ khác $i$ và $j$. Theo công thức (6), vì thế ta có

$$
\varphi (p(v_1), . . . ,p(\widehat{v}_i), . . . ,p(\widehat{v}_j), . . . , p(v_n), p(v_i)\mu_i)
$$

$$
=\varphi (p(v_1), . . . ,p(\widehat{v}_i), . . . ,p(\widehat{v}_j), . . . , p(v_n),-p(v_j)\mu_j)
$$

Bằng cách áp dụng các công thức (1) và (3), ta suy ra

$$
\varphi (p(v_1), . . . ,p(\widehat{v}_j), . . . , p(v_n))\pi (\mu_i)\pi (-1)^{n-i-1}
$$

$$
=\varphi (p(v_1), . . . ,\widehat{p}(v_i), . . . , p(v_n))\pi (-\mu_j)\pi (-1)^{n-j}
$$

và do đó $t_i=t_j$.

Sau khi đã chứng minh điều này, ta định nghĩa $\omega (v_1, . . . , v_n)$ là giá trị chung của các $t_i$ với $i$ thuộc I. Như vậy ta đã xây dựng được một ánh xạ $\omega$ từ B(V) vào $D^*_{ab}$ thỏa mãn quan hệ (9). Cho $(w_1, . . . , w_{n-1})$ là một cơ sở của W; nếu đặt $v_i=w_i$ với $1\leqslant i\leqslant n-1$ và $v_n=e$, thì ta có $I =\{n\}$ và $\mu_n= 1$. Hơn nữa ta có $p(v_i) =w_i$ với $1\leqslant i\leqslant n-1$, và công thức $\omega (w_1, . . . , w_{n-1}, e) =\varphi (w_1, . . . , w_{n-1})$ là một trường hợp riêng của (9).

Bây giờ ta phải chứng minh rằng $\omega$ thuộc Ω(V).

C) Chứng minh công thức (1): Cho $\lambda_1, . . . , \lambda_n$ là các phần tử của $D^*$ và $(v_1, . . . , v_n)$ là một cơ sở của V. Ta định nghĩa $\mu_1, . . . , \mu_n$ và I như trên. Chọn một $i$ trong I. Vì ta có $e=\sum^n_{j=1}(v_j\lambda_j)(\lambda^{-1}_j\mu_j)$, công thức (9) suy ra

$$
\omega (v_1\lambda_1, . . . , v_n\lambda_n) \tag{11}
$$

$$
=\pi (-1)^{n-i}\pi (\lambda^{-1}_i\mu_i)^{-1}\varphi (p(v_1)\lambda_1, . . . ,\widehat{p(v_i)\lambda_i}, . . . , p(v_n)\lambda_n)
$$

Nhưng ta có $\pi (\lambda^{-1}_i\mu_i)^{-1}=\pi (\mu_i)^{-1}\pi (\lambda_i)$ và

$$
\varphi (p(v_1)\lambda_1, . . . ,\widehat{p(v_i)\lambda_i}, . . . , p(v_n)\lambda_n)
$$

$$
=\varphi (p(v_1), . . . ,\widehat{p(v_i)}, . . . , p(v_n))\pi (\lambda_1. . .\widehat{\lambda}_i. . . \lambda_n)
$$

So sánh các công thức (9) và (11) dẫn đến quan hệ cần tìm

$$
\omega (v_1\lambda_1, . . . , v_n\lambda_n) =\omega (v_1, . . . , v_n)\pi (\lambda_1. . . \lambda_n)
$$

D) Chứng minh công thức (2): Cho $(v_1, . . . , v_n)$ là một cơ sở của V và $i, j$ là hai số nguyên phân biệt trong khoảng $[1, n]$; ta định nghĩa $\mu_1, . . . , \mu_n$ như trước. Xét cơ sở $(v'_1, . . . , v'_n)$ của V được xác định bởi $v'_i=v_i+v_j$ và $v'_k=v_k$ với $k\not=i$, và đưa vào các tọa độ $\mu'_1, . . . , \mu'_n$ của $e$ đối với cơ sở này; chúng thỏa mãn $\mu'_j=\mu_j-\mu_i$ và $\mu'_k=\mu_k$ với $k\not=j$. Đặt $t=\omega (v_1, . . . , v_n)$ và $t'=\omega (v'_1, . . . , v'_n)$. Ta phải chứng minh rằng $t$ và $t'$ bằng nhau.

Trước hết, chú ý rằng, theo định nghĩa của $\omega$, ta có

$$
t=\pi (-1)^{n-k}\pi (\mu_k)^{-1}\varphi (p(v_1), . . . ,\widehat{p(v_k)}, . . . , p(v_n)) \tag{12}
$$

$$
t'=\pi (-1)^{n-k}\pi (\mu'_k)^{-1}\varphi (p(v'_1), . . . ,\widehat{p(v'_k)}, . . . , p(v'_n)) \tag{13}
$$

với mọi $k$ sao cho $\mu_k$ và $\mu'_k$ là khác không.

a) Nếu $\mu_i\not=0$, thì các dãy $(p(v_1), . . . ,\widehat{p(v_k)}, . . . , p(v_n))$ và $(p(v'_1), . . . ,\widehat{p(v'_k)}, . . . , p(v'_n))$ là bằng nhau, và ta có $\mu_i$ = $\mu'_i$, do đó $t=t'$.

b) Nếu tồn tại một chỉ số $k$ khác $i$ và $j$ sao cho $\mu_k\not= 0$, thì ta có $p(v'_l) =p(v_l)$ với $l\not=i$ và $p(v'_i) =p(v_i) +p(v_j)$. Các phần tử $p(v_i)$ và $p(v_j)$ đều thuộc dãy $(p(v_1), . . . ,p(\widehat{v}_k), . . . , p(v_n))$. Vì $\varphi$ thuộc Ω(W), công thức (2) của VIII, p. 447 được áp dụng; nó cho

$$
\varphi (p(v_1), . . . ,p(\widehat{v}_k), . . . , p(v_n)) =\varphi (p(v'_1), . . . ,p(\widehat{v}'_k), . . . , p(v'_n))
$$

Nhưng ta cũng có $\mu_k=\mu'_k$, và do đó $t=t'$.

c) Còn phải xét trường hợp mà chỉ số duy nhất $k$ sao cho $\mu_k\not= 0$ là $j$. Khi đó ta có $\mu'_j=\mu_j,e=v_j\mu_j$, và $p(v_j) = 0$. Đặt $k=j$ trong các công thức (12) và (13). Vì các dãy $(p(v_1), . . . ,p(\widehat{v}_j), . . . , p(v_n))$ và $(p(v'_1), . . . ,p(\widehat{v}'_j), . . . , p(v'_n))$ bằng nhau, ta có $t=t'$.

#### Hệ quả 1 {#alg-viii-a2-prop-1-cor-1 .statement tag=00Q2}

Cho $(e_1, . . . , e_n)$ là một cơ sở của V và $t$ là một phần tử của $D^*_{ab}$. Tồn tại một phần tử duy nhất $\omega$ của Ω(V) sao cho $\omega (e_1, . . . , e_n) =t$.

Hãy chứng minh hệ quả bằng quy nạp theo $n$. Nếu $n= 0$, thì cơ sở duy nhất của V là cơ sở rỗng, nên mệnh đề là đúng. Bây giờ giả sử $n\geqslant 1$; ký hiệu W là không gian con của V sinh bởi $e_1, . . . , e_{n-1}$. Theo Mệnh đề 1, tồn tại một song ánh Λ từ Ω(V) tới Ω(W) thỏa mãn

$$
(\Lambda (\omega ))(w_1, . . . , w_{n-1}) =\omega (w_1, . . . , w_{n-1}, e_n)
$$

với mọi cơ sở $(w_1, . . . , w_{n-1})$ của W và mọi $\omega$ trong Ω(V). Theo giả thiết quy nạp, tồn tại một phần tử duy nhất $\varphi$ của Ω(W) sao cho $\varphi (e_1, . . . , e_{n-1}) =t$. Quan hệ $\omega (e_1, . . . , e_n) =t$, với $\omega$ trong Ω(V), là tương đương với $\Lambda (\omega ) =\varphi$. Hệ quả 1 được suy ra.

#### Hệ quả 2 {#alg-viii-a2-prop-1-cor-2 .statement tag=00Q3}

Cho $\omega$ và $\omega '$ là hai phần tử của Ω(V). Tồn tại một phần tử duy nhất $t$ của $D^*_{ab}$ sao cho $\omega '=t\omega$.

#### Nhận xét {#alg-viii-a2-n2-rem-1 .statement tag=00Q4}

Giả sử rằng trường D là giao hoán. Theo định nghĩa, B(V) là một tập con của $V^n$. Hiển nhiên là hạn chế lên B(V) của một dạng $n$-tuyến tính phản xứng khác không $f: V^n\rightarrow D$ thuộc Ω(V). Hơn nữa, nếu $(e_1, . . . , e_n)$ là một cơ sở của V và $t$ là một phần tử khác không của D, thì tồn tại một dạng $n$-tuyến tính phản xứng duy nhất $f$ sao cho $f(e_1, . . . , e_n) =t$ (III, §7, No. 4, p. 511 and III, §7, No. 8, p. 518). Theo Hệ quả 1, tập hợp Ω(V) gồm các hạn chế lên B(V) của các dạng $n$-tuyến tính phản xứng khác không.

### 3. Định thức của một tự đẳng cấu

Trước hết ta giả sử rằng trường D là giao hoán. Theo nhận xét ở trên, định thức của một tự đẳng cấu $u$ của V là phần tử duy nhất det $u$ của $D^*$ sao cho ta có

(14) $\omega (u(v_1), . . . , u(v_n)) =$ (det $u$)$\omega (v_1, . . . , v_n)$

đối với mọi cơ sở $(v_1, . . . , v_n)$ của V và mọi phần tử $\omega$ của Ω(V).

Bây giờ ta trở lại trường hợp trong đó D không còn được giả sử là giao hoán nữa.

#### Mệnh đề 2 {#alg-viii-a2-prop-2 .statement tag=00Q5}

a) Cho $u$ là một tự đẳng cấu của V. Tồn tại một phần tử duy nhất của $D^*_{ab}$, được ký hiệu là det $u$ và được gọi là định thức của $u$, sao cho ta có

(15) $\omega (u(v_1), . . . , u(v_n)) =$ (det $u$)$\omega (v_1, . . . , v_n)$

đối với mọi cơ sở $(v_1, . . . , v_n)$ của V và mọi $\omega$ thuộc Ω(V).

b) Ánh xạ $u\mapsto$ det $u$ từ $\mathbf{G}\mathbf{L}(V)$ vào $D^*_{ab}$ là một đồng cấu nhóm.

Cho $\omega_0$ là một phần tử của Ω(V). Ánh xạ $(v_1, . . . , v_n)\mapsto$ $\omega_0(u(v_1), . . . , u(v_n))$ từ B(V) vào $D^*_{ab}$ thuộc Ω(V). Theo Hệ quả 2 của VIII, p. 451, tồn tại một phần tử duy nhất $t$ của $D^*_{ab}$ sao cho ta có

$$
\omega_0(u(v_1), . . . , u(v_n)) =t\omega_0(v_1, . . . , v_n)
$$

đối với $(v_1, . . . , v_n)$ trong B(V). Nếu $\omega$ là một phần tử khác của Ω(V), thì tồn tại một phần tử $s$ của $D^*_{ab}$ sao cho

$$
\omega (v_1, . . . , v_n) =s\omega_0(v_1, . . . , v_n)
$$

đối với mọi cơ sở $(v_1, . . . , v_n)$ của V (loc. cit.). Ta ngay lập tức suy ra quan hệ

$$
\omega (u(v_1), . . . , u(v_n)) =t\omega (v_1, . . . , v_n)
$$

Điều này chứng minh a); mệnh đề b) là một hệ quả ngay lập tức của a).

### 4. Định thức của một Ma trận Bình phương

Cho $n$ là một số nguyên dương. Hãy áp dụng điều trên cho không gian vectơ phải $D^n_d$ trên trường D; các phần tử của $D^n_d$ được xem như các ma trận có $n$ hàng và một cột. Gọi $(\varepsilon_1, . . . , \varepsilon_n)$ là cơ sở chính tắc của $D^n_d$. Theo Hệ quả 2 của VIII, p. 451, tồn tại một phần tử duy nhất $\omega_0$ của $\Omega (D^n_d)$ sao cho $\omega_0(\varepsilon_1, . . . , \varepsilon_n) = 1$. Nếu A là một phần tử của $\mathbf{G}\mathbf{L}_n$(D), thì các cột của nó $a_1, . . . , a_n$ lập thành một cơ sở của $D^n_d$; phần tử $\omega_0(a_1, . . . , a_n)$ của $D^*_{ab}$ được gọi là định thức của A và được ký hiệu bởi det(A). Vì ta có $a_i=A\varepsilon_i$ với $1\leqslant i\leqslant n$, định thức của A đơn giản là định thức của tự đẳng cấu $x\mapsto Ax$ của $D^n_d$. Đặc biệt, nếu trường D là giao hoán, thì định thức của A trùng với định thức đã được định nghĩa trong III, §8, No. 3, p. 524.

Cho V là một không gian vectơ phải có số chiều hữu hạn $n$ trên trường D, và gọi $(e_1, . . . , e_n)$ là một cơ sở của V. Nếu $u$ là một tự đẳng cấu của V và A là ma trận của $u$ đối với cơ sở $(e_1, . . . , e_n)$, thì ta có det($u$) $=$ det(A).

Ta ký hiệu bởi ($E_{ij}$) họ các đơn vị ma trận của $\mathbf{M}_n(D)$ (II, §10, No. 3, p. 341). Với mỗi phần tử $\lambda$ của D và mỗi cặp $(i, j)$ gồm các số nguyên phân biệt trong $[1, n]$, ta đặt (II, §10, No. 13, p. 361)

$$
B_{ij}(\lambda ) =I_n+\lambda E_{ij}
$$

nó là một phần tử của $\mathbf{G}\mathbf{L}_n(D)$. Nếu $\lambda_1, . . . , \lambda_n$ là các phần tử của $D^*$, thì ma trận đường chéo diag($\lambda_1, . . . , \lambda_n$) cũng thuộc $\mathbf{G}\mathbf{L}_n(D)$.

#### Mệnh đề 3 {#alg-viii-a2-prop-3 .statement tag=00Q6}

Ánh xạ det là đồng cấu duy nhất từ $\mathbf{G}\mathbf{L}_n(D)$ vào $D^*_{ab}$ thỏa mãn các hệ thức

(16) det($B_{ij}(1)$) $= 1$

với $i\not=j$ và

(17) det(diag($\lambda_1, . . . , \lambda_n$)) $=\pi (\lambda_1\cdots \lambda_n)$,

với $\lambda_1, . . . , \lambda_n\in D^*$

Cho A là một phần tử của $\mathbf{G}\mathbf{L}_n(D)$ và $a_1, . . . , a_n$ là các cột của nó. Ta có

det(A) $=\omega_0(a_1, . . . , a_n)$.

Bây giờ, các cột của ma trận A diag($\lambda_1, . . . , \lambda_n$) là $a_1\lambda_1, . . . , a_n\lambda_n$, và do đó các cột của ma trận AB$_{ij}(1)$ là $a_1, . . . , a_j+a_i, a_{j+1}, . . . , a_n$. Vì $\omega_0$ là phần tử duy nhất của $\Omega (D^n_d)$ sao cho $\omega_0(\varepsilon_1, . . . , \varepsilon_n) = 1$, ta thấy rằng định thức là ánh xạ duy nhất $\varphi :\mathbf{G}\mathbf{L}_n(D)\rightarrow D^*_{ab}$ thỏa mãn các hệ thức

(18) $\varphi ($A diag($\lambda_1, . . . , \lambda_n$)) $=\varphi ($A$)\pi (\lambda_1\cdots \lambda_n)$,

(19) $\varphi ($AB$_{ij}(1)) =\varphi ($A) với $i\not=j$,

$$
\varphi (I_n) = 1 \tag{20}
$$

Điều này trước hết chứng minh rằng ánh xạ định thức thỏa mãn các hệ thức (16) và (17). Ta đã biết rằng ánh xạ này là một đồng cấu từ $\mathbf{G}\mathbf{L}_n(D)$ đến $D^*_{ab}$. Ngược lại, nếu $\varphi$ là một đồng cấu từ $\mathbf{G}\mathbf{L}_n(D)$ đến $D^*_{ab}$ sao cho $\varphi (B_{ij}(1)) = 1$ với $i\not=j$ và $\varphi$(diag($\lambda_1, . . . , \lambda_n$)) $=\pi (\lambda_1\cdots \lambda_n)$, thì $\varphi$ thỏa mãn các hệ thức từ (18) đến (20) và do đó bằng det.

#### Ví dụ 1 {#alg-viii-a2-n4-exa-1 .statement tag=00Q7}

Các cột của ma trận $B_{ij}(\lambda )$ là $\varepsilon_1, . . . , \varepsilon_j$ + $\varepsilon_i\lambda , \varepsilon_{i+1}, . . . , \varepsilon_n$. Theo công thức (5) của VIII, p. 448, ta có

(21) det($B_{ij}(\lambda )$) $= 1$.

#### Ví dụ 2 {#alg-viii-a2-n4-exa-2 .statement tag=00Q8}

Cho $\sigma$ là một phép hoán vị của khoảng $[1, n]$ trong $\mathbf{N}$, có dấu $\varepsilon (\sigma )$. Gọi M$(\sigma )$ là ma trận của phép hoán vị $\sigma$ (II, §10, No. 7, p. 351). Các cột của ma trận M$(\sigma )$ là $\varepsilon_{\sigma(1)}, . . . , \varepsilon_{\sigma(n)}$. Áp dụng công thức (4) của VIII, p. 448, do đó ta có

(22) det(M$(\sigma )$) $=\pi (\varepsilon (\sigma ))$.

#### Ví dụ 3 {#alg-viii-a2-n4-exa-3 .statement tag=00Q9}

Giả sử $n\geqslant 1$. Với mọi ma trận đường chéo khả nghịch có dạng Δ = diag($d_1, . . . , d_n$), ta có Δ$B_{ij}(\lambda$)Δ$^{-1}=B_{ij}(d_i\lambda d^{-1}_j)$. Cho A là một phần tử của $\mathbf{G}\mathbf{L}_n(D)$. Theo Hệ quả 1 của II, §10, No. 13, p. 362 và công thức trước, tồn tại các ma trận P và Δ trong $\mathbf{G}\mathbf{L}_n(D)$ sao cho A = PΔ, P là tích của các ma trận dạng $B_{ij}(\lambda )$, và Δ là một ma trận đường chéo có dạng diag(1$, . . . ,1, d$). Theo Ví dụ 1, ta có det(P) = 1, và do đó det(A) = det(Δ) $=\pi (d)$ theo Mệnh đề 3.

#### Ví dụ 4 {#alg-viii-a2-n4-exa-4 .statement tag=00QA}

Cho $D'$ là một trường, và cho $u$ là một đồng cấu từ D đến $D'$. Khi chuyển qua các thương, $u$ xác định một đồng cấu nhóm $u_{ab}$ từ $D^*_{ab}$ đến $D^{'*}_{ab}$. Gọi $u_n$ là đồng cấu từ $\mathbf{G}\mathbf{L}_n(D)$ đến $\mathbf{G}\mathbf{L}_n(D')$ biến đổi một ma trận A $= (a_{ij})$ thành ma trận $(u(a_{ij}))$. Công thức

(23) det($u_n($A)) $=u_{ab}$(det(A))

đối với $A\in \mathbf{G}\mathbf{L}_n(D)$ suy ra ngay lập tức từ Ví dụ 3.

#### Ví dụ 5 {#alg-viii-a2-n4-exa-5 .statement tag=00QB}

Ta có $\mathbf{G}\mathbf{L}_1(D) = D^*$, và Mệnh đề 3 cho thấy rằng ta có det($a$) $=\pi (a)$ với $a$ trong $\mathbf{G}\mathbf{L}_1(D)$.

#### Ví dụ 6 {#alg-viii-a2-n4-exa-6 .statement tag=00QC}

Giả sử $n= 2$. Cho $A = \begin{pmatrix} a & b \\ c & d \end{pmatrix}$ là một phần tử của $\mathbf{G}\mathbf{L}_2(D)$. Hai phần tử $a$ và $c$ của D không đồng thời bằng không. Chúng ta sẽ cho định thức của A một cách tường minh.

Nếu $a$ khác không, thì ta có

(24) $A = \begin{pmatrix} 1 & 0 \\ ca^{-1} & 1 \end{pmatrix}\begin{pmatrix} a & 0 \\ 0 & d-ca^{-1}b \end{pmatrix}\begin{pmatrix} 1 & a^{-1}b \\ 0 & 1 \end{pmatrix}$.

Do đó, $ad-aca^{-1}b\not= 0$ và

(25) det(A) $=\pi (ad-aca^{-1}b)$.

b) Nếu $a$ bằng không, thì ta có $c\not= 0$ và

(26) $A = \begin{pmatrix} 0 & b \\ c & d \end{pmatrix} = \begin{pmatrix} 0 & 1 \\ 1 & 0 \end{pmatrix}\begin{pmatrix} c & d \\ 0 & b \end{pmatrix}$.

Do đó, theo a) và Ví dụ 2, ta có $cb\not= 0$ và

(27) det(A) $=\pi (-cb)$.

#### Ví dụ 7 {#alg-viii-a2-n4-exa-7 .statement tag=00QD}

Cho $D^o$ là trường đối của D. Ánh xạ $A\mapsto^tA$ từ $\mathbf{M}_n(D)$ vào $\mathbf{M}_n(D^o)$ thỏa mãn $^t($AB$) =^tB^tA$. Do đó, với mọi ma trận A trong $\mathbf{G}\mathbf{L}_n$(D), ma trận chuyển vị $^tA$ là khả nghịch trong $\mathbf{M}_n(D^o)$, nhưng không nhất thiết khả nghịch trong $\mathbf{M}_n(D)$. Suy ra từ Ví dụ 3 rằng nếu A thuộc $\mathbf{G}\mathbf{L}_n$(D), thì các phần tử A của $\mathbf{G}\mathbf{L}_n(D)$ và $^tA$ của $\mathbf{G}\mathbf{L}_n(D^o)$ có cùng định thức. Mặt khác, ngay cả khi ma trận $^tA$ thuộc $\mathbf{G}\mathbf{L}_n$(D), định thức của nó trong GL$_n(D)$ không nhất thiết bằng định thức của A (xem Ví dụ 6).

#### Nhận xét 1 {#alg-viii-a2-n4-rem-1 .statement tag=00QE}

Cho V là một không gian vectơ phải trên trường D, có số chiều hữu hạn $n$. Ta xem không gian đối ngẫu $V^*=$ Hom$_D(V,D)$ như một không gian vectơ phải trên trường đối $D^o$ của D. Cho $u$ là một tự đẳng cấu của V, và cho $^tu$ là tự đẳng cấu của $V^*$ là chuyển vị của $u$. Nếu $u$ được biểu diễn bởi một ma trận A trong $\mathbf{M}_n(D)$ đối với một cơ sở $(e_1, . . . , e_n)$ của V, thì tự đẳng cấu $^tu$ được biểu diễn bởi ma trận $^tA$ trong $\mathbf{M}_n(D^o)$ đối với cơ sở $(e^*_1, . . . , e^*_n)$ của $V^*$ đối ngẫu với $(e_1, . . . , e_n)$ (II, §10, No. 4, p. 344, Mệnh đề 3). Theo Ví dụ 7, định thức của $^tu$ bằng định thức của $u$.

#### Nhận xét 2 {#alg-viii-a2-n4-rem-2 .statement tag=00QF}

Các kết quả của các Tiểu mục 1 đến 4 khái quát hóa được cho trường hợp D là một vành địa phương (VIII, p. 459, Bài tập 2).

### 5. Nhóm đơn môđula

Cho $n$ là một số nguyên dương. Ta ký hiệu bởi $\mathbf{S}\mathbf{L}_n(D)$ hạt nhân của đồng cấu nhóm det$:\mathbf{G}\mathbf{L}_n(D)\rightarrow D^*_{ab}$, và gọi nó là nhóm đơn môđula hoặc nhóm tuyến tính đặc biệt (xem III, §8, No. 9, p. 537 khi trường D là giao hoán).

#### Định lý 1 {#alg-viii-a2-thm-1 .statement tag=00QG}

Giả sử $n\geqslant 2$.

a) Nhóm con $\mathbf{S}\mathbf{L}_n(D)$ của $\mathbf{G}\mathbf{L}_n(D)$ được sinh bởi các ma trận $B_{ij}(\lambda )$, trong đó $i$ và $j$ là các số nguyên phân biệt trong khoảng $[1, n]$ và $\lambda$ chạy qua D.

b) Giả sử $n\geqslant 3$ hoặc Card(D) $\geqslant 3$. Nhóm dẫn xuất của $\mathbf{G}\mathbf{L}_n(D)$ bằng $\mathbf{S}\mathbf{L}_n(D)$.

c) Giả sử $n\geqslant 3$ hoặc Card(D) $\geqslant 4$. Nhóm dẫn xuất của $\mathbf{S}\mathbf{L}_n(D)$ bằng $\mathbf{S}\mathbf{L}_n(D)$.

A) Ký hiệu bởi T nhóm con của $\mathbf{G}\mathbf{L}_n(D)$ sinh bởi các ma trận $B_{ij}(\lambda )$. Theo Ví dụ 1 của VIII, p. 454, ta có det($B_{ij}(\lambda )$) $= 1$, và do đó $T\subset \mathbf{S}\mathbf{L}_n(D)$. Để chứng minh rằng hai nhóm này bằng nhau, khi đó chỉ cần, theo Ví dụ 3 của loc. cit., chứng minh rằng mọi ma trận có dạng diag(1$, . . . ,1, d$) với $\pi (d) = 1$ đều thuộc T. Ma trận diag(1$, . . . ,1, d$) thuộc ảnh của đồng cấu $U\mapsto \begin{pmatrix} I_{n-2} & 0 \\ 0 & U \end{pmatrix}$ từ $\mathbf{G}\mathbf{L}_2(D)$ vào $\mathbf{G}\mathbf{L}_n(D)$; vì vậy chỉ cần xét trường hợp $n= 2$. Vì hạt nhân của $\pi$ là nhóm dẫn xuất của $D^*$, ta có thể giả sử $d=uvu^{-1}v^{-1}$ với $u, v$ trong $D^*$. Mệnh đề của ta khi đó suy ra từ các đẳng thức

(28) $\begin{pmatrix} 1 & 0 \\ 0 & d \end{pmatrix} = \begin{pmatrix} u^{-1} & 0 \\ 0 & u \end{pmatrix}\begin{pmatrix} v^{-1} & 0 \\ 0 & v \end{pmatrix}\begin{pmatrix} vu & 0 \\ 0 & u^{-1}v^{-1} \end{pmatrix}$

và

(29) $\begin{pmatrix} s & 0 \\ 0 & s^{-1} \end{pmatrix} = \begin{pmatrix} 1 & s \\ 0 & 1 \end{pmatrix}\begin{pmatrix} 1 & 0 \\ 1-s^{-1} & 1 \end{pmatrix}\begin{pmatrix} 1 & -1 \\ 0 & 1 \end{pmatrix}\begin{pmatrix} 1 & 0 \\ 1-s & 1 \end{pmatrix}$

với $s\in D^*$.

B) Theo phép dựng, $\mathbf{S}\mathbf{L}_n(D)$ là hạt nhân của một đồng cấu từ $\mathbf{G}\mathbf{L}_n(D)$ đến một nhóm giao hoán, nên nó chứa nhóm dẫn xuất $(\mathbf{G}\mathbf{L}_n(D),\mathbf{G}\mathbf{L}_n(D))$ của $\mathbf{G}\mathbf{L}_n(D)$. Theo điều trên, ta có

$$
\mathbf{S}\mathbf{L}_n(D)\supset (\mathbf{G}\mathbf{L}_n(D),\mathbf{G}\mathbf{L}_n(D))\supset (\mathbf{S}\mathbf{L}_n(D),\mathbf{S}\mathbf{L}_n(D))
$$

Để chứng minh c), chỉ cần chứng minh rằng các ma trận $B_{ij}(\lambda )$ là các giao hoán tử trong $\mathbf{S}\mathbf{L}_n(D)$.

Giả sử $n\geqslant 3$. Nếu $i,j,k$ là các số nguyên phân biệt trong khoảng $[1, n]$ và $\mu, \nu$ là các phần tử của D, thì ta có

$$
B_{ij}(\mu\nu ) =B_{ik}(\mu)^{-1}B_{kj}(\nu )^{-1}B_{ik}(\mu)B_{kj}(\nu ) \tag{30}
$$

Lấy $\mu= 1$ và $\nu =\lambda$, ta thấy rằng ma trận $B_{ij}(\lambda )$ là một giao hoán tử của các phần tử của $\mathbf{S}\mathbf{L}_n(D)$.

Bây giờ giả sử $n= 2$. Cho $u$ và $v$ là các phần tử của D với $u\not= 0$. Ta có các hệ thức

(31) $\begin{pmatrix} 1 & v-uvu \\ 0 & 1 \end{pmatrix} = \begin{pmatrix} u & 0 \\ 0 & u^{-1} \end{pmatrix}\begin{pmatrix} 1 & -v \\ 0 & 1 \end{pmatrix}\begin{pmatrix} u^{-1} & 0 \\ 0 & u \end{pmatrix}\begin{pmatrix} 1 & v \\ 0 & 1 \end{pmatrix}$ và

(32) $\begin{pmatrix} 1 & 0 \\ v-uvu & 1 \end{pmatrix} = \begin{pmatrix} u^{-1} & 0 \\ 0 & u \end{pmatrix}\begin{pmatrix} 1 & 0 \\ -v & 1 \end{pmatrix}\begin{pmatrix} u & 0 \\ 0 & u^{-1} \end{pmatrix}\begin{pmatrix} 1 & 0 \\ v & 1 \end{pmatrix}$.

Ta có det $\begin{pmatrix} u & 0 \\ 0 & u^{-1} \end{pmatrix}$ = 1, do đó các ma trận $B_{12}(v-uvu)$ và $B_{21}(v-uvu)$ là các giao hoán tử của các phần tử của $\mathbf{S}\mathbf{L}_n(D)$.

Giả sử trường D có ít nhất bốn phần tử. Cho $\lambda$ là một phần tử của D. Nếu $\lambda$ bằng 0, 1, hoặc $-1$, chọn một phần tử tùy ý $u$ trong $D-\{0,1,-1\}$; nếu không, đặt $u=\lambda$. Trong cả hai trường hợp, $u$ là một phần tử khác không của D, nó giao hoán với $\lambda$, và ta có $u^2\not= 1$. Đặt $v=\lambda (1-u^2)^{-1}$. Ta có $uv=vu$ và do đó $v-uvu=v(1-u^2) =\lambda$. Khi đó suy ra từ các hệ thức (31) và (32) rằng các ma trận $B_{12}(\lambda )$ và $B_{21}(\lambda )$ là các giao hoán tử trong $\mathbf{S}\mathbf{L}_n(D)$. Điều này hoàn tất chứng minh của c).

C) Còn phải chứng minh rằng $\mathbf{S}\mathbf{L}_2(D)$ là nhóm dẫn xuất của $\mathbf{G}\mathbf{L}_2(D)$ khi D có ba phần tử. Theo A), nhóm $\mathbf{S}\mathbf{L}_2(D)$ được sinh bởi các ma trận $B_{12}(1) = \begin{pmatrix} 1 & 1 \\ 0 & 1 \end{pmatrix}$ và $B_{21}(1) = \begin{pmatrix} 1 & 0 \\ 1 & 1 \end{pmatrix}$, và các ma trận này là các giao hoán tử của những phần tử của $\mathbf{G}\mathbf{L}_2(D)$ vì ta có $B_{21}(1) =^tB_{12}(1)$ và

(33) $\begin{pmatrix} 1 & 1 \\ 0 & 1 \end{pmatrix} = \begin{pmatrix} -1 & 0 \\ 0 & 1 \end{pmatrix}\begin{pmatrix} 1 & 1 \\ 0 & 1 \end{pmatrix}\begin{pmatrix} -1 & 0 \\ 0 & 1 \end{pmatrix}^{-1}\begin{pmatrix} 1 & 1 \\ 0 & 1 \end{pmatrix}^{-1}$.

#### Nhận xét {#alg-viii-a2-n5-rem-1 .statement tag=00QH}

Nếu D là một trường có hai phần tử, thì $\mathbf{G}\mathbf{L}_2(D)$ bằng $\mathbf{S}\mathbf{L}_2$(D), và đó là một nhóm có cấp 6 mà nhóm dẫn xuất của nó có cấp 3. Nếu D là một trường có ba phần tử, thì nhóm $\mathbf{S}\mathbf{L}_2(D)$ có cấp 24, và nhóm dẫn xuất của nó có cấp 8. Giả sử $n\geqslant 2$; trừ hai trường hợp trước, mọi nhóm con chuẩn tắc của $\mathbf{S}\mathbf{L}_n(D)$ phân biệt với $\mathbf{S}\mathbf{L}_n(D)$ đều được chứa trong tâm $Z(\mathbf{S}\mathbf{L}_n(D))$ của $\mathbf{S}\mathbf{L}_n(D)$ (II, §10, p. 421, Bài tập 13 and 14). Khi đó nhóm $\mathbf{S}\mathbf{L}_n(D)/Z(\mathbf{S}\mathbf{L}_n(D))$ là đơn.

Cho V là một không gian vectơ phải trên trường D, có số chiều hữu hạn $n$. Ta ký hiệu bởi SL(V), và gọi là nhóm đơn môđula của V, hạt nhân của đồng cấu det$:\mathbf{G}\mathbf{L}(V)\rightarrow D^*_{ab}$. Việc chọn một cơ sở của V cho phép đồng nhất nhóm này với $\mathbf{S}\mathbf{L}_n(D)$.

Ta nói rằng một tự đẳng cấu $u$ của V là một phép vị tự nếu tồn tại một vectơ $v$ của V và một dạng tuyến tính $\varphi$ trên V sao cho $\varphi (v) = 0$ và $u(x) =x+v\varphi (x)$ với mọi $x$ trong V. Khi $n\geqslant 2,u$ là một phép vị tự nếu và chỉ nếu tồn tại một cơ sở của V mà đối với cơ sở đó ma trận của $u$ có dạng $B_{ij}(\lambda )$. Định lý 1 suy ra hệ quả sau đây.

#### Hệ quả {#alg-viii-a2-n5-cor-1 .statement tag=00RU}

Cho V là một không gian vectơ phải trên trường D, có số chiều hữu hạn $n\geqslant 2$.

a) Nhóm con $\mathbf{S}\mathbf{L}(V)$ của $\mathbf{G}\mathbf{L}(V)$ được sinh bởi các phép vị tự.

b) Nhóm con $\mathbf{S}\mathbf{L}(V)$ là nhóm dẫn xuất của $\mathbf{G}\mathbf{L}(V)$ trừ khi ta có $n= 2$ và D có hai phần tử.

c) Nhóm $\mathbf{S}\mathbf{L}(V)$ bằng nhóm dẫn xuất của nó trừ khi ta có $n= 2$ và D có hai hoặc ba phần tử.

### Bài tập {#alg-viii-a2-exercises}

Xem [các bài tập của phụ lục 2](exercises/a2/).
