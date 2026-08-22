---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Semisimple Modules and Rings
section: 21
section_title: Linear Representations of Finite Groups
lang: vi
source: alg-viii
source_edition: 2023, Springer Nature
book_pages: A VIII.397-A VIII.434
pdf_pages: 0414-0451
extraction: native
subsections:
    - "no": 1
      title: Linear Representations
      page: 397
      pdf_page: 414
    - "no": 2
      title: Maschke’s Theorem
      page: 401
      pdf_page: 418
    - "no": 3
      title: Induced and Coinduced Representations
      page: 402
      pdf_page: 419
    - "no": 4
      title: Representations and the Grothendieck Group
      page: 404
      pdf_page: 421
    - "no": 5
      title: Fourier Inversion Formula
      page: 406
      pdf_page: 423
    - "no": 6
      title: Schur Orthogonality Relations
      page: 409
      pdf_page: 426
    - "no": 7
      title: Orthogonality Relation for Characters
      page: 410
      pdf_page: 427
    - "no": 8
      title: Central Functions on a Finite Group
      page: 411
      pdf_page: 428
    - "no": 9
      title: The Case of Abelian Groups
      page: 414
      pdf_page: 431
    - "no": 10
      title: Characters and Grothendieck Groups
      page: 415
      pdf_page: 432
    - "no": 11
      title: Dimension of Simple Representations
      page: 415
      pdf_page: 432
    - "no": 12
      title: Change of Base Field
      page: 416
      pdf_page: 433
    - "no": 13
      title: Complex Linear Representations
      page: 421
      pdf_page: 438
statements: 36
exercises: 30
content_sha256: 8751c9ed3358250a77bf5b9204859e13d5b4ffce10bb9174d000f54edddf1d67
translated_from: content/en/alg/VIII/21_s21_linear_representations_of_finite_groups.md
source_content_sha256: 57b93c57e726f0b46672458d4233fb8efa77dd7ed1544adad7750b082adfbad3
translation_model: gpt-5.4, gpt-5.4-mini, copied
translation_run: translate-vi-ecba1889
glossary_version: 34
glossary_terms_sha256: 80d0c8a6f3be053ea3c044df421c0630f8e8e0bcac385018620a32bdfef35267
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 21. BIỂU DIỄN TUYẾN TÍNH CỦA NHÓM HỮU HẠN

Trong tiết này, G là một nhóm, và K là một vành giao hoán. Nếu G là một nhóm hữu hạn, thì ta ký hiệu bởi $|G|$ phần tử Card(G)$\cdot 1$ của K. Từ No. 5 trở đi, ta giả thiết rằng nhóm G là hữu hạn, rằng vành K là một trường đóng đại số, và rằng $|G|$ khác không.

### 1. Biểu Diễn Tuyến Tính

#### Định nghĩa 1 {#alg-viii-s21-def-1 .statement tag=00NC}

Cho M là một K-môđun. Một biểu diễn tuyến tính của G trong M là một đồng cấu nhóm từ G vào nhóm tuyến tính $\mathbf{G}\mathbf{L}(M)$ (II, §1, No. 2, p. 195).

Cho $\pi$ là một biểu diễn tuyến tính của G trong một K-môđun M. Ta cũng nói rằng cặp $(M, \pi )$ là một biểu diễn tuyến tính của G. Khi K khác không và M là một K-môđun tự do, chiều của M được gọi là bậc (hoặc chiều) của biểu diễn $\pi$.

Nhớ rằng ánh xạ chính tắc $g\mapsto e_g$ từ G vào đại số K[G] của nhóm G là một cơ sở của K-môđun K[G]. Theo lối nói lạm dụng ký hiệu, ta cũng ký hiệu phần tử $e_g$ của K[G] bởi $g$. Với một biểu diễn tuyến tính $\pi : G\rightarrow \mathbf{G}\mathbf{L}(M)$ của G, tồn tại một đồng cấu duy nhất của các K-đại số từ K[G] vào End$_K(M)$ mở rộng $\pi$ (III, §2, No. 6, p. 447, Ví dụ); ta cũng ký hiệu mở rộng này bởi $\pi$. Đó là một biểu diễn của đại số K[G] trong M (VIII, p. 373, Định nghĩa 1), nên M là một K[G]-môđun. Ngược lại, mọi biểu diễn tuyến tính $\rho$ của đại số K[G] trong M xác định một biểu diễn tuyến tính của G trong M cho bởi $g\mapsto \rho (g)$.

Ta sẽ tự do áp dụng thuật ngữ liên quan đến cấu trúc K[G]-môđun cho các biểu diễn tuyến tính của nhóm G. Chẳng hạn, ta nói đến một biểu diễn con, một biểu diễn đơn, một tổng trực tiếp các biểu diễn, v.v. Cho $(M, \pi )$ và $(M', \pi ')$ là các biểu diễn tuyến tính của G; ta ký hiệu bởi Hom$_G(\pi , \pi ')$ K-môđun Hom$_{K[G]}(M,M')$ gồm các đồng cấu của các K[G]-môđun từ M đến $M'$.[^1]

Một ánh xạ $f$ từ G vào K được gọi là một hàm trung tâm nếu ta có $f(gg') =$ $f(g'g)$ với mọi cặp $(g, g')$ các phần tử của G; tương đương, ta có $f(ghg^{-1}) =$ $f(h)$ với mọi cặp phần tử $g, h$ của G. Do đó các hàm trung tâm là các hàm trên G mà hạn chế của chúng trên mỗi lớp liên hợp là hằng. Chúng tạo thành một môđun con của không gian các ánh xạ từ G vào K, được ký hiệu bởi $\mathscr{Z}_K(G)$. Khi G hữu hạn, K-đại số $\mathscr{Z}_K(G)$ là một K-môđun tự do có chiều bằng số các lớp liên hợp của G. Tâm Z(K[G]) của đại số K[G] gồm các phần tử $a=\sum a_gg$ của K[G] sao cho $hah^{-1}=a$ với mọi $h\in G$. Bây giờ, ta có

$$
hah^{-1}=\sum_{g\in G}a_{h^{-1}gh}g
$$

do đó, khi G hữu hạn, tâm Z(K[G]) của đại số K[G] gồm các hàm trung tâm.

Cho $(M, \pi )$ là một biểu diễn tuyến tính của G. Giả sử rằng M là một K-môđun tự do hữu hạn chiều. Vết của $\pi$ là vết của biểu diễn của K[G] liên kết với $\pi$, nghĩa là (VIII, p. 382), dạng tuyến tính $a\mapsto$ Tr($\pi (a)$) trên K[G]. Dạng tuyến tính này được xác định bởi ánh xạ $g\mapsto$ Tr($\pi (g)$) từ G vào K, mà ta gọi là đặc trưng của biểu diễn $\pi$ và ký hiệu là $\chi_{\pi}$. Đặc trưng của một biểu diễn là một hàm trung tâm (II, §4, No. 3, p. 273, Mệnh đề 3).

Cho M và $M'$ là các K-môđun tự do hữu hạn chiều. Cho $\pi$ và $\pi '$ lần lượt là các biểu diễn tuyến tính của G trong M và $M'$. Khi đó $M\oplus M'$ là một K-môđun tự do hữu hạn chiều, và, theo Mệnh đề 1 của III, §9, No. 2, p. 543, ta có

$$
\chi_{\pi\oplus\pi'}=\chi_{\pi}+\chi_{\pi'}
$$

Nói chung, cho

$$
0\longrightarrow M'\longrightarrow M\longrightarrow M''\longrightarrow 0
$$

là một dãy khớp các K[G]-môđun, và gọi $\pi ,\pi '$, và $\pi ''$ lần lượt là các biểu diễn tuyến tính của G liên kết với $M, M'$, và $M''$. Giả sử rằng các K-môđun $M'$ và $M''$ là tự do và hữu hạn chiều. Khi đó M cũng vậy (II, §1, No. 11, p. 218, Mệnh đề 21), và ta có

$$
\chi_{\pi}=\chi_{\pi'}+\chi_{\pi''} \tag{1}
$$

#### Mệnh đề 1 {#alg-viii-s21-prop-1 .statement tag=00ND}

Giả sử rằng K là một trường giao hoán. Cho $\pi$ và $\pi '$ là các biểu diễn K-tuyến tính nửa đơn hữu hạn chiều của G.

a) Nếu các đa thức đặc trưng của $\pi (g)$ và $\pi '(g)$ là như nhau với mọi $g\in G$, thì các biểu diễn $\pi$ và $\pi '$ là đẳng cấu.

b) Giả sử thêm rằng K có đặc số 0. Nếu các đặc trưng $\chi_{\pi}$ và $\chi_{\pi'}$ bằng nhau, thì các biểu diễn $\pi$ và $\pi '$ là đẳng cấu.

Mệnh đề a) suy ra từ Hệ quả 1 của VIII, p. 386; mệnh đề b) suy ra từ phần a) của hệ quả ở VIII, p. 384.

#### Ví dụ 1 {#alg-viii-s21-n1-exa-1 .statement tag=00NE}

Biểu diễn đơn vị hay tầm thường của G là biểu diễn $(K, \varepsilon )$, trong đó $\varepsilon (g) =$ Id$_K$ với mọi $g\in G$. Đặc trưng của nó là hàm hằng có giá trị 1.

#### Ví dụ 2 {#alg-viii-s21-n1-exa-2 .statement tag=00NF}

Biểu diễn chính quy (trái) của G là biểu diễn $\boldsymbol{\gamma }$ của G trong K[G] được xác định bởi $\boldsymbol{\gamma }(g)(x) =gx$ với $g\in G$ và $x\in K[G]$. Nó tương ứng với biểu diễn chính quy trái của đại số K[G] (VIII, p. 375). Giả sử nhóm G là hữu hạn. Khi đó biểu diễn chính quy có bậc hữu hạn. Với mọi phần tử $g$ của G khác phần tử đơn vị, ma trận của phép nhân trái bởi $g$ trong K[G] đối với cơ sở chính tắc là ma trận của một phép hoán vị không có điểm bất động. Do đó ta có

$|G|$ nếu $g$ là phần tử đơn vị,

$$
\chi_{\boldsymbol{\gamma }}(g) = \tag{2}
$$

0 trong các trường hợp khác.

Ta cũng định nghĩa tương tự biểu diễn chính quy phải của G. Biểu diễn song chính quy của G là biểu diễn $\rho$ của $G\times G$ trong K[G] được định nghĩa bởi quan hệ $\rho (g, g')(x) =gxg^{'-1}$ với $(g, g')\in G\times G$ và $x\in K[G]$.

#### Ví dụ 3 {#alg-viii-s21-n1-exa-3 .statement tag=00NG}

Cho một biểu diễn tuyến tính $(M, \pi )$ của G, biểu diễn phản biến hay đối ngẫu $\pi^{\vee}$ của $\pi$ là biểu diễn của G trong K-môđun đối ngẫu của M được định nghĩa bởi quan hệ $\pi^{\vee}(g) =^t\pi (g^{-1})$ với mọi $g\in G$ (xem II, §2, No. 5, p. 234). Nếu M là một K-môđun tự do hữu hạn chiều, thì đối ngẫu của nó cũng vậy, và ta có $\chi_{\pi^{\vee}}(g) =\chi_{\pi}(g^{-1})$ với mọi $g\in G$.

#### Ví dụ 4 {#alg-viii-s21-n1-exa-4 .statement tag=00NH}

Cho $(M, \pi )$ và $(M', \pi ')$ là các biểu diễn tuyến tính của G. Trong Ví dụ 1 của VIII, p. 198, ta đã xác định một cấu trúc K[G]-môđun trên $M\otimes_KM'$. Biểu diễn tuyến tính tương ứng được gọi là tích tenxơ của $\pi$ và $\pi '$ và được ký hiệu bởi $\pi \otimes \pi '$. Với $g\in G,x\in M$, và $x'\in M'$, ta có $((\pi \otimes \pi ')(g))(x\otimes x') =\pi (g)x\otimes \pi '(g)x'$.

Nếu M và $M'$ là các K-môđun tự do hữu hạn chiều, thì theo Mệnh đề 2 của III, §9, No. 2, p. 543, ta có

$$
\chi_{\pi\otimes\pi'}=\chi_{\pi}\chi_{\pi'} \tag{3}
$$

#### Ví dụ 5 {#alg-viii-s21-n1-exa-5 .statement tag=00NI}

Giả sử G là tích $G'\times G''$ của hai nhóm. Ánh xạ K-tuyến tính từ $K[G']\otimes_KK[G'']$ đến K[G] biến $g'\otimes g''$ thành $(g', g'')$ với $g'\in G'$ và $g''\in G''$ là một đẳng cấu đại số. Gọi $(M', \pi ')$ là một biểu diễn tuyến tính của $G'$ và $(M'', \pi '')$ là một biểu diễn tuyến tính của $G''$. Tích tenxơ ngoài của $\pi '$ và $\pi ''$, ký hiệu là $\pi '\pi ''$, là biểu diễn của $G'\times G''$ trong không gian vectơ $M'\otimes M''$ được xác định bởi $(\pi '\pi '')(g', g'') =\pi '(g')\otimes \pi ''(g'')$ với $(g', g'')\in G'\times G''$. Nếu $M'$ và $M''$ là các K-môđun tự do hữu hạn chiều, thì $M'\otimes_KM''$ là một K-môđun tự do hữu hạn chiều và đặc trưng của biểu diễn $\pi '\pi ''$ được cho bởi công thức

$$
\chi_{\pi'\pi''}(g', g'') =\chi_{\pi'}(g')\chi_{\pi''}(g'')
$$

với $g'\in G'$ và $g''\in G''$ (Mệnh đề 2 của III, §9, No. 2, p. 542).

#### Ví dụ 6 {#alg-viii-s21-n1-exa-6 .statement tag=00NJ}

Cho $(V, \pi )$ là một biểu diễn tuyến tính của G sao cho V là một K-môđun tự do hữu hạn chiều. Ta định nghĩa một biểu diễn $\rho$ của $G\times G$ trong End$_K(V)$ bởi công thức

$$
\rho (g, g')(u) =\pi (g')\circ u\circ \pi (g^{-1})
$$

Đẳng cấu K-môđun $\theta_V: V^*\otimes_KV\rightarrow$ End$_K(V)$ của II, §4, No. 2, p. 271 là một đẳng cấu của các biểu diễn từ tích tenxơ ngoài $\pi^{\vee}\pi$ tới $\rho$. Ánh xạ $g\mapsto \rho (1, g)$ (resp. $g\mapsto \rho (g,1)$) là một biểu diễn của G đẳng cấu với $\pi^{dim_KV}$ (resp. $(\pi^{\vee})^{dim_KV}$).

Cho L là một đại số giao hoán trên K, và cho $(M, \pi )$ là một biểu diễn tuyến tính của nhóm G. Đồng cấu nhóm $\pi_{(L)}: G\rightarrow \mathbf{G}\mathbf{L}(M_{(L)})$ được xác định bởi $g\mapsto$ Id$_L\otimes \pi (g)$ là một biểu diễn tuyến tính của G trong L-môđun $M_{(L)}$, được gọi là biểu diễn tuyến tính của G suy ra từ biểu diễn $\pi$ bằng phép mở rộng vành vô hướng từ K thành L.

Giả sử K là một trường và L là một K-đại số giao hoán khác không. Cho $(M, \pi )$ và $(M', \pi ')$ là các biểu diễn tuyến tính của G. Các biểu diễn $\pi$ và $\pi '$ là đẳng cấu khi và chỉ khi $\pi_{(L)}$ và $\pi '_{(L)}$ là đẳng cấu (VIII, p. 37, Định lý 3).

Giả sử thêm rằng đại số L là một mở rộng của K. Xét các vành $R_K(G)$ và $R_L(G)$ được định nghĩa trong Ví dụ 1 của VIII, p. 198. Mở rộng vô hướng xác định một đồng cấu vành

$$
u: R_K(G)\longrightarrow R_L(G)
$$

Đồng cấu này là đơn ánh, và một phần tử $\xi \in R_K(G)$ là hiệu dụng khi và chỉ khi $u(\xi )$ là hiệu dụng (VIII, p. 195, Định lý 1).

### 2. Định lý Maschke

#### Định lý 1 {#alg-viii-s21-thm-1 .statement tag=00NK}

Giả sử nhóm G là hữu hạn. Cho M là một K[G]-môđun, và N là một môđun con K[G] của M. Giả sử N là một nhân tử trực tiếp của K-môđun M và $|G|$ khả nghịch trong K. Khi đó N là một nhân tử trực tiếp của K[G]-môđun M.

Cho $p$ là một phép chiếu K-tuyến tính trên M có ảnh là N. Ta định nghĩa một tự đồng cấu $q$ của K-môđun M bằng cách đặt

$$
q(x) =|G|^{-1}\sum_{g\in G}g p(g^{-1}x)
$$

với mọi $x\in M$. Vì N ổn định dưới tác động của G và $p$ cảm sinh đồng nhất trên N, nên ta thấy rằng $q$ gửi M vào N và cảm sinh đồng nhất trên N.

Do đó K-môđun M là tổng trực tiếp của ảnh N của $q$ và hạt nhân của $q$. Ta có $g q(x) =q(gx)$ với mọi $x\in M$ và $g\in G$, nên hạt nhân của $q$ là một K[G]-môđun con của M. Điều này chứng minh rằng N là một nhân tử trực tiếp của K[G]-môđun M.

#### Hệ quả 1 (Maschke) {#alg-viii-s21-thm-1-cor-1 .statement tag=00SC}

Giả sử rằng nhóm G là hữu hạn và K là một trường giao hoán. Đại số K[G] là nửa đơn khi và chỉ khi phần tử $|G|$ của trường K khác không.

Giả sử $|G| \not= 0$. Theo Định lý 1, mọi K[G]-môđun con của $K[G]_s$ đều là một nhân tử trực tiếp. Do đó K[G] là nửa đơn.

Đảo lại, giả sử rằng $|G|$ bằng không, và ký hiệu bởi $\varepsilon$ phần tử $\sum_{g\in G}g$ của tâm của K[G]. Ta có $\varepsilon \not= 0$ nhưng $\varepsilon^2=|G|\varepsilon = 0$, do đó K[G] không nửa đơn (VIII, p. 153, Mệnh đề 3, a) và VIII, p. 157, Nhận xét 1).

#### Hệ quả 2 {#alg-viii-s21-thm-1-cor-2 .statement tag=00NL}

Giả sử rằng nhóm G là hữu hạn và rằng $|G|$ khả nghịch trong K. Một dãy khớp các K[G]-môđun tách được khi và chỉ khi nó tách được như một dãy khớp các K-môđun.

Cho một dãy khớp các K[G]-môđun

0 // ${M'}^f$ // M // $M''$ // $0$,

chỉ cần áp dụng Định lý 1 cho ảnh của cấu xạ $f$.

#### Hệ quả 3 {#alg-viii-s21-thm-1-cor-3 .statement tag=00NM}

Giả sử rằng nhóm G là hữu hạn và rằng $|G|$ khả nghịch trong K. Một K[G]-môđun là xạ ảnh khi và chỉ khi nó xạ ảnh như một K-môđun.

Cho P là một K[G]-môđun. Nếu P là một nhân tử trực tiếp của một K[G]-môđun tự do M, thì a fortiori nó là một nhân tử trực tiếp của K-môđun tự do M. Chiều đảo lại suy ra từ Hệ quả 2, theo II, §2, No. 2, p. 231, Mệnh đề 4, d).

#### Hệ quả 4 {#alg-viii-s21-thm-1-cor-4 .statement tag=00NN}

a) Giả sử rằng nhóm G là hữu hạn và rằng K là một trường giao hoán có đặc số 0. Hai biểu diễn tuyến tính hữu hạn chiều của G là đẳng cấu khi và chỉ khi chúng có cùng đặc trưng.

b) Giả sử rằng K là một trường hoàn hảo có đặc số là một số nguyên tố $p$ và rằng nhóm G là hữu hạn, có lực lượng nguyên tố cùng nhau với $p$. Đặc trưng của một biểu diễn tuyến tính hữu hạn chiều của G bằng không khi và chỉ khi biểu diễn này đẳng cấu với tổng trực tiếp của $p$ biểu diễn từng đôi một đẳng cấu.

Dưới các giả thiết của hệ quả, mọi biểu diễn tuyến tính hữu hạn chiều của G đều nửa đơn. Khi đó hệ quả suy ra từ hệ quả ở VIII, p. 384.

#### Hệ quả 5 {#alg-viii-s21-thm-1-cor-5 .statement tag=00NO}

Giả sử nhóm G là hữu hạn và K là một trường giao hoán trong đó $|G| \not= 0$. Cho $\pi$ và $\pi '$ là các biểu diễn tuyến tính hữu hạn chiều của G. Khi đó $\pi$ và $\pi '$ là đẳng cấu nếu và chỉ nếu với mọi $g$ trong G, các nội cấu $\pi (g)$ và $\pi '(g)$ có cùng đa thức đặc trưng.

Điều này suy ra từ Hệ quả 1 của VIII, p. 386.

### 3. Các Biểu diễn Cảm sinh và Đối cảm sinh

Cho H là một nhóm con của nhóm G.

Nếu $(V, \pi )$ là một biểu diễn tuyến tính của G, thì hạn chế của $\pi$ lên H là một biểu diễn tuyến tính của H trong V; ta ký hiệu nó bởi Res$^G_H(\pi )$. K[H]-môđun liên kết với Res$^G_H(\pi )$ đơn giản là môđun suy ra từ K[G]-môđun V bằng hạn chế vô hướng (II, §1, No. 13, p. 221). Nếu V là một K-môđun tự do hữu hạn chiều, thì đặc trưng của Res$^G_H(\pi )$ là hạn chế của đặc trưng của $\pi$ lên H.

Cho $(M, \sigma )$ là một biểu diễn của H.

Ta xem K[G] là một $(K[G]$, K[H])-song môđun và M là một K[H]-môđun. K[G]-môđun $\mathscr{T}(M) = K[G]\otimes_{K[H]}M$ (VIII, p. 58) xác định một biểu diễn tuyến tính của G, được ký hiệu bởi Ind$^G_H(\sigma )$ và được gọi là biểu diễn của G cảm sinh bởi $\sigma$. Nếu $(V, \pi )$ là một biểu diễn tuyến tính của G, thì K[H]-môđun $\mathscr{H}(V) =$ Hom$_{K[G]}(K[G],V)$ có thể được đồng nhất với K[H]-môđun tương ứng với biểu diễn Res$^G_H(\pi )$. Do đó, cấu xạ phép nối (VIII, p. 59) cho một đẳng cấu K-môđun, được gọi là chính tắc, từ Hom$_H(\sigma$, Res$^G_H(\pi ))$ đến Hom$_G$(Ind$^G_H(\sigma ), \pi$ ) (“tương hỗ Frobenius”).

Ta xem K[G] như một $(K[H]$, K[G])-song môđun. K[G]-môđun $\mathscr{H}(M) =$ Hom$_{K[H]}(K[G],M)$ xác định một biểu diễn của G, ký hiệu là Coind$^G_H(\sigma )$ và được gọi là biểu diễn của G đối cảm sinh bởi $\sigma$. Nếu $(V, \pi )$ là một biểu diễn tuyến tính của G, thì K[H]-môđun $\mathscr{T}(V) = K[G]\otimes_{K[G]}V$ có thể được đồng nhất với K[H]-môđun tương ứng với biểu diễn Res$^G_H(\pi )$. Do đó, cấu xạ phép nối (loc. cit.) cho một đẳng cấu K-môđun, được gọi là chính tắc, từ Hom$_H$(Res$^G_H(\pi ), \sigma$ ) đến Hom$_G(\pi$, Coind$^G_H(\sigma ))$.

Cho $\varepsilon : K[G]\rightarrow K[H]$ là đồng cấu K-môđun được đặc trưng bởi các quan hệ $\varepsilon (h) =h$ nếu $h\in$ H và $\varepsilon (g) = 0$ nếu $g\in G$ - H. Ánh xạ $\varepsilon$ là một đồng cấu của các song môđun $(K[H]$, K[H]). Cho $(M, \sigma )$ là một biểu diễn tuyến tính của H. Ánh xạ $v\mapsto v\circ \varepsilon$ từ Hom$_{K[H]}(K[H],M)$ vào Hom$_{K[H]}(K[G],M)$ là một đồng cấu của các K[H]-môđun. Bằng cách đồng nhất M với Hom$_{K[H]}(K[H],M)$, ta thu được một đồng cấu của các K[H]-môđun từ M vào Res$^G_H$(Coind$^G_H(\sigma )$). Luật tương hỗ Frobenius gửi nó thành một đồng cấu $\iota$ của các K[G]-môđun từ Ind$^G_H(\sigma )$ vào Coind$^G_H(\sigma )$ được đặc trưng bởi quan hệ

$$
\iota (g\otimes m)(g') =\varepsilon (g'g)m
$$

với $g, g'\in G$ và $m\in M$. Đồng cấu này được gọi là đồng cấu chính tắc.

#### Mệnh đề 2 {#alg-viii-s21-prop-2 .statement tag=00NP}

Cho H là một nhóm con của G, và cho $(M, \sigma )$ là một biểu diễn tuyến tính của H. Đồng cấu chính tắc $\iota :$ Ind$^G_H(\sigma )\rightarrow$ Coind$^G_H(\sigma )$ là đơn ánh. Nếu nhóm con H có chỉ số hữu hạn trong G, thì $\iota$ là một đẳng cấu K[G]-môđun.

Cho $S\subset G$ là một hệ các đại diện của $G/H$. Họ $(s)_{s\in S}$ là một cơ sở của K[H]-môđun phải K[G]. Suy ra ánh xạ $M^{(S)}\rightarrow$ Ind$^G_H(\sigma )$ được xác định bởi $(m_s)_{s\in S}\mapsto \sum_{s\in S}s\otimes m_s$ là một đẳng cấu của các K-môđun. Với mọi $s, s'\in S$ và mọi $m\in M$, ta có các hệ thức

$$
\iota (s'\otimes m)(s^{-1}) =\begin{cases} m & \text{nếu } s=s',\\ 0 & \text{nếu không.}\end{cases}
$$

Suy ra $\iota '$ là đơn ánh.

Giả sử rằng H có chỉ số hữu hạn trong G. Khi đó tập hợp S là hữu hạn; gọi $\rho$ là ánh xạ từ Coind$^G_H(\sigma )$ đến Ind$^G_H(\sigma )$ được cho bởi $u\mapsto \sum_{s\in S}s\otimes u(s^{-1})$. Nó thỏa mãn $(\iota \circ \rho (u))(s^{-1}) =u(s^{-1})$ với $u\in$ Coind$^G_H(\sigma )$ và $s\in S$. Vì họ $(s^{-1})_{s\in S}$ là một cơ sở của K[H]-môđun trái K[G], ánh xạ $\iota \circ \rho$ là ánh xạ đồng nhất. Do đó, $\iota$ là song ánh với song ánh ngược $\rho$.

Cho H là một nhóm con của G có chỉ số hữu hạn. Cho $u$ là một hàm trung tâm trên H; ký hiệu $u^0$ là hàm trên G kéo dài $u$ và bằng không tại mọi điểm của G - H. Cho S là một hệ đại diện của $G/H$. Với $g\in G$, đặt

(4) Ind$^G_H(u)(g) =\sum_{s\in S}u^0(s^{-1}gs)$.

Chú ý rằng với mọi $x, g\in G$ và mọi $h\in H$, ta có $u^0((xh)^{-1}gxh) =$ $u^0(x^{-1}gx)$. Suy ra Ind$^G_H(u)$ là một hàm trung tâm trên G không phụ thuộc vào lựa chọn S. Do đó ta định nghĩa một ánh xạ K-tuyến tính Ind$^G_H$ từ $\mathscr{Z}_K(H)$ vào $\mathscr{Z}_K(G)$.

#### Mệnh đề 3 {#alg-viii-s21-prop-3 .statement tag=00NQ}

Cho H là một nhóm con của G với chỉ số hữu hạn. Cho $(M, \sigma )$ là một biểu diễn tuyến tính của H. Giả sử rằng M là một K-môđun tự do hữu hạn chiều. Ký hiệu bởi $(V, \pi )$ biểu diễn của G được cảm sinh bởi $\sigma$. Khi đó K-môđun V là tự do và hữu hạn chiều, và

(5) $\chi_{\pi}=$ Ind$^G_H(\chi_{\sigma})$.

Cho S là một hệ đại diện của $G/H$. Như đã thấy ở trên, ánh xạ tuyến tính $M^S\rightarrow$ Ind$^G_H(M)$ xác định bởi $(m_s)_{s\in S}\mapsto \sum_{s\in S}s\otimes m_s$ là một đẳng cấu K-môđun. Đặc biệt, V là một K-môđun tự do hữu hạn chiều. Với mọi $g\in G$, ký hiệu $M_g$ là ảnh của M bởi ánh xạ $m\mapsto g\otimes m$. Với mọi $g, g'\in G$, ta có $M_g= M_{g'}$ khi và chỉ khi $gH =g'H$, và V là tổng trực tiếp của các môđun con $M_s$ với $s\in S$. Với mọi $g, g'\in G$, ta cũng có $\pi (g)M_{g'}= M_{gg'}$. Với mọi $g\in G$, ký hiệu $S_g$ là tập hợp các phần tử $s$ của S sao cho $s^{-1}gs\in H$. Với mọi $g, g'\in G$ sao cho $g^{'-1}gg'\in H$, tự đẳng cấu $\pi (g)$ của V cảm sinh một tự đẳng cấu $\pi (g)_{g'}$ của $M_{g'}$, và ta có

Tr($\pi (g)$) $=\sum_{s\in S_g}$ Tr($\pi (g)_s$) $=\sum_{s\in S_g}$ Tr($\sigma (s^{-1}gs)$).

Khẳng định cuối cùng của mệnh đề suy ra được.

### 4. Các biểu diễn và nhóm Grothendieck

Trong tiểu mục này, ta giả sử rằng K là một trường giao hoán. Với một biểu diễn tuyến tính hữu hạn chiều $(M, \pi )$ của G, ta ký hiệu bởi $[\pi ]$ lớp của K[G]-môđun M trong vành Grothendieck $R_K(G)$ (VIII, p. 198, Ví dụ 1).

Theo định nghĩa các luật hợp thành trên vành $R_K$(G), nếu $\pi$ và $\pi '$ là các biểu diễn tuyến tính hữu hạn chiều của G, thì ta có

$$
[\pi \oplus \pi '] = [\pi ] + [\pi '],[\pi \otimes \pi '] = [\pi ] [\pi ']
$$

Phần tử đơn vị của vành $R_K(G)$ là lớp của biểu diễn đơn vị của G (VIII, p. 399, Ví dụ 1).

Vành $R_K(G)$ là một $\mathbf{Z}$-môđun tự do có cơ sở là tập hợp các lớp của các K[G]-môđun đơn có số chiều hữu hạn trên K. Khi $|G|$ khả nghịch trong K, hai biểu diễn hữu hạn chiều là đẳng cấu khi và chỉ khi chúng có cùng lớp trong $R_K(G)$ (VIII, p. 190, Hệ quả và p. 401, Hệ quả 1).

Với mọi biểu diễn tuyến tính hữu hạn chiều $(M, \pi )$ của G, biểu diễn đối ngẫu $\pi^{\vee}$ cũng là hữu hạn chiều. Các biểu diễn $\pi$ và $(\pi^{\vee})^{\vee}$ là đẳng cấu. Nếu $\pi '$ cũng là một biểu diễn tuyến tính hữu hạn chiều của G, thì các biểu diễn $(\pi \otimes \pi ')^{\vee}$ và $\pi^{\vee}\otimes \pi^{'\vee}$ là đẳng cấu. Nếu

$$
0\longrightarrow M'\longrightarrow M\longrightarrow M''\longrightarrow 0
$$

là một dãy khớp các K[G]-môđun có số chiều hữu hạn trên K, thì các biểu diễn đối ngẫu cho một dãy khớp các K[G]-môđun

$$
0\longrightarrow M^{''\vee}\longrightarrow M^{\vee}\longrightarrow M^{'\vee}\longrightarrow 0
$$

(II, §7, No. 5, p. 299, Hệ quả của Định lý 5). Theo tính chất phổ quát của các nhóm Grothendieck (VIII, p. 186, Mệnh đề 4), tồn tại một tự đẳng cấu $c\mapsto c^{\vee}$ của vành $R_K(G)$ được đặc trưng bởi $[\pi ]^{\vee}= [\pi^{\vee}]$ với mọi biểu diễn tuyến tính hữu hạn chiều $\pi$ của G; ta có $(c^{\vee})^{\vee}=c$ với mọi phần tử $c$ của $R_K(G)$.

Cho H là một nhóm con của G. Hạn chế bảo toàn các dãy khớp. Theo tính chất phổ quát của các nhóm Grothendieck (loc. cit.), do đó tồn tại một đồng cấu nhóm, ký hiệu là Res$^G_H$, từ $R_K(G)$ đến $R_K(H)$ được đặc trưng bởi quan hệ

(6) Res$^G_H[\pi ] =$ [Res$^G_H(\pi )]$

đối với mọi biểu diễn tuyến tính hữu hạn chiều $\pi$ của G; đó là một đồng cấu vành. Nếu H có chỉ số hữu hạn trong G, thì theo Mệnh đề 14 của II, §7, No. 7, p. 306, ta có thể định nghĩa, tương tự, một đồng cấu nhóm Ind$^G_H$ từ $R_K(H)$ vào $R_K(G)$ được đặc trưng bởi quan hệ

(7) Ind$^G_H[\sigma ] =$ [Ind$^G_H(\sigma )]$

đối với mọi biểu diễn tuyến tính hữu hạn chiều $\sigma$ của H.

Theo các quan hệ (1) của VIII, p. 399 và (3) của VIII, p. 400 và tính chất phổ quát của các nhóm Grothendieck đã nhắc đến ở trên, tồn tại một đồng cấu vành $\Theta_G$ từ $R_K(G)$ vào đại số $\mathscr{Z}_K(G)$ các hàm trung tâm trên G, được đặc trưng bởi $\Theta_G([\pi ]) =\chi_{\pi}$ đối với mọi biểu diễn hữu hạn chiều $\pi$ của G.

Nếu H là một nhóm con của G, thì các đồng cấu $\Theta_G$ và $\Theta_H$ liên kết với các nhóm G và H tương thích với các phép toán Res$^G_H$ và Ind$^G_H$ (VIII, p. 402 và VIII, p. 404, Mệnh đề 3).

Giả sử rằng G là tích $G'\times G''$ của hai nhóm. Theo VIII, p. 213, Nhận xét 2, tồn tại một ánh xạ tuyến tính trên $\mathbf{Z}$ $\kappa$ từ $R_K(G')\otimes_{\mathbf{Z}}R_K(G'')$ đến nhóm $R_K(G'\times G'')$ được đặc trưng bởi quan hệ $\kappa ([\pi ']\otimes [\pi '']) = [\pi '\pi '']$ với $\pi '$ (resp. $\pi ''$) là một biểu diễn hữu hạn chiều của $G'$ (resp. $G''$) và $\pi '\pi ''$ là tích tenxơ ngoài (VIII, p. 400, Ví dụ 5). Nó là một đồng cấu vành. Nếu trường K đóng đại số, thì ánh xạ $\kappa$ là một đẳng cấu (VIII, p. 213, Nhận xét 2).

Giả sử rằng G là tích $G'\times G''$ của hai nhóm. Kí hiệu bởi $\psi$ đồng cấu từ $\mathscr{Z}_K(G')\otimes_K\mathscr{Z}_K(G'')$ tới $\mathscr{Z}_K(G)$ biến $f'\otimes f''$ thành hàm $(g', g'')\mapsto f'(g')f''(g'')$. Biểu đồ sau là giao hoán:

$R_K(G')\otimes_{\mathbf{Z}}R_K(G'')^{\kappa}$ // $R_K(G)$

$\Theta_{G'}\otimes \Theta_{G''}\Theta_G$

$\mathscr{Z}_K(G')\otimes_K\mathscr{Z}_K(G'')^{\psi}$ /$/\mathscr{Z}_K(G)$.

### 5. Công thức đảo Fourier

Trong phần còn lại của tiết này, ta giả sử rằng nhóm G là hữu hạn và K là một trường đóng đại số mà đặc số không chia hết cấp của G, do đó phần tử $|G|$ của K khác không.

Đại số K[G] là nửa đơn (định lý Maschke) và hữu hạn chiều. Ký hiệu $\widehat{G}$ là tập hợp các lớp của các K[G]-môđun đơn. Với mọi $\lambda \in \widehat{G}$, chọn một biểu diễn tuyến tính $(V_{\lambda}, \pi_{\lambda})$ của G sao cho K[G]-môđun liên kết thuộc lớp $\lambda$. Tập hợp $\widehat{G}$ là hữu hạn, và các không gian vectơ $V_{\lambda}$ là hữu hạn chiều (VIII, p. 141, Ví dụ). Với mọi $\lambda \in \widehat{G}$, ký hiệu $d_{\lambda}$ là bậc của biểu diễn $\pi_{\lambda}$, tức là chiều của không gian vectơ trên K $V_{\lambda}$, và ký hiệu đặc trưng của nó là $\chi_{\lambda}$.

Ký hiệu $F(\widehat{G})$ là đại số tích $\prod_{\lambda\in\widehat{G}}$ End$_K(V_{\lambda})$ và $\overline{\mathscr{F}}$ là ánh xạ từ K[G] vào $F(\widehat{G})$ được xác định bởi $\overline{\mathscr{F}}(a) = (\pi_{\lambda}(a))_{\lambda\in\widehat{G}}$. Vì trường K đóng đại số, ánh xạ $\overline{\mathscr{F}}$ là một đẳng cấu đại số (loc. cit.).

Với mọi $\lambda \in \widehat{G}$, chiều của đại số End$_K(V_{\lambda})$ là $d^2_{\lambda}$; chiều của đại số K[G] là Card(G). Do đó ta có quan hệ

(8) Card(G) $=\sum_{\lambda\in\widehat{G}}d^2_{\lambda}$.

Ký hiệu $\tau$ là vết trong đại số K[G]; theo định nghĩa, vết $\tau (a)$ của một phần tử $a$ của K[G] là vết của tự đồng cấu $x\mapsto ax$ của K[G] (III, §7, No. 7, p. 515). Cho $a=\sum_{g\in G}a_gg$ là một phần tử của K[G]; theo công thức (2), ta có $\tau (ag^{-1}) =|G|a_g$ với mọi $g\in G$, và do đó có quan hệ

$$
a=|G|^{-1}\sum_{g\in G}\tau (ag^{-1})g \tag{9}
$$

Ký hiệu $\widehat{\tau}$ là vết trong đại số $F(\widehat{G})$. Cho $A = (A_{\lambda})_{\lambda\in\widehat{G}}$ là một phần tử của $F(\widehat{G})$; ta có (xem III, §9, No. 3, p. 545, Ví dụ 3)

(10) $\widehat{\tau}(A) =\sum_{\lambda\in\widehat{G}}d_{\lambda}$ Tr(A$_{\lambda}$).

Vì ánh xạ $\overline{\mathscr{F}}$ là một đẳng cấu đại số trên K, ta có $\widehat{\tau}\circ \overline{\mathscr{F}}=\tau$, và do đó

$\tau (a) =\widehat{\tau}(\overline{\mathscr{F}}(a)) =\widehat{\tau}((\pi_{\lambda}(a))_{\lambda\in\widehat{G}})=\sum_{\lambda\in\widehat{G}}d_{\lambda}$ Tr($\pi_{\lambda}(a)$) $=\sum_{\lambda\in\widehat{G}}d_{\lambda}$ Tr$_{\lambda}(a)$

với mọi $a\in K[G]$, tức là

(11) $\tau =\sum_{\lambda\in\widehat{G}}d_{\lambda}$ Tr$_{\lambda}$.

Do đó, theo (2) của VIII, p. 399, với $g\in G$, ta có

$|G|$ nếu $g$ là phần tử đơn vị,

$$
\sum d_{\lambda}\chi_{\lambda}(g) = \tag{12}
$$

0 trong các trường hợp khác.

Với $a\in K[G]$, quan hệ $(^{\lambda\in\widehat{G}}$ 9) có dạng sau:

(13) $a=|G|^{-1}\sum_{g\in G}\sum_{\lambda\in\widehat{G}}d_{\lambda}$ Tr($\pi_{\lambda}(a)\pi_{\lambda}(g^{-1})$)$g$;

suy ra rằng đối với mọi phần tử $A = (A_{\lambda})_{\lambda\in\widehat{G}}$ của $F(\widehat{G})$, ta có

(14) $\overline{\mathscr{F}}^{-1}(A) =|G|^{-1}\sum_{g\in G}\sum_{\lambda\in\widehat{G}}d_{\lambda}$ Tr(A$_{\lambda}\pi_{\lambda}(g^{-1})$)$g$ (“công thức đảo Fourier”).

Với $\mu\in \widehat{G}$, ký hiệu bởi $j_\mu:$ End$_K(V_\mu)\longrightarrow \prod_{\lambda\in\widehat{G}}$ End$_K(V_{\lambda})$ ánh xạ sao cho $j_\mu(u) = (v_{\lambda})$, trong đó $v_{\lambda}= 0$ nếu $\lambda \not=\mu$ và $v_\mu=u$. Theo công thức (14), ta có

(15) $\overline{\mathscr{F}}^{-1}(j_\mu(u)) =|G|^{-1}d_\mu\sum_{g\in G}$ Tr($u\pi_\mu(g^{-1})$)$g$.

Tâm của đại số $F(\widehat{G}) =\prod_{\lambda\in\widehat{G}}$ End$_K(V_{\lambda})$ gồm các họ $(a_{\lambda}1_{V_{\lambda}})_{\lambda\in\widehat{G}}$, trong đó $(a_{\lambda})$ là một họ các phần tử của K. Nó là ảnh bởi $\overline{\mathscr{F}}$ của tâm của đại số K[G]. Vậy tâm đó có một cơ sở $(e_{\lambda})_{\lambda\in\widehat{G}}$ được đặc trưng bởi quan hệ

$$
\pi_{\lambda}(e_\mu) =\delta_{\lambda \mu}1_{V_{\lambda}} \tag{16}
$$

với $\lambda , \mu\in \widehat{G}$, trong đó $\delta_{\lambda \mu}$ là hàm delta Kronecker. Theo công thức (15), ta có, với mọi $\mu\in \widehat{G}$,

$$
e_\mu=|G|^{-1}d_\mu\sum_{g\in G}\chi_\mu(g^{-1})g \tag{17}
$$

Các phần tử này thỏa mãn các quan hệ

(18) $\sum_{\lambda\in\widehat{G}}e_{\lambda}= 1,e^2_\mu=e_\mu$, and $e_\mu e_{\nu}= 0$

với mọi $\mu, \nu \in \widehat{G}$ sao cho $\mu\not=\nu$; chúng là các lũy đẳng không phân tích được của Z(K[G]) (VIII, p. 147, Mệnh đề 15)

#### Nhận xét {#alg-viii-s21-n5-rem-1 .statement tag=00NR}

Cho $(V, \pi )$ là một biểu diễn tuyến tính của G. Theo Định lý Maschke, K[G]-môđun V là nửa đơn. Với mọi $\lambda \in \widehat{G}$, ký hiệu $V^{\lambda}$ là thành phần đẳng kiểu kiểu $\lambda$ của K[G]-môđun V; ta có $V =\bigoplus_{\lambda\in\widehat{G}}V^{\lambda}$. Theo Mệnh đề 15 của VIII, p. 147 và công thức (17), phép chiếu của V có ảnh $V^{\lambda}$ liên kết với phân tích này của V thì bằng

$$
\pi (e_{\lambda}) =|G|^{-1}d_{\lambda}\sum_{g\in G}\chi_{\lambda}(g^{-1})\pi (g) \tag{19}
$$

Áp dụng công thức này cho $\pi =\pi_{\lambda}$, ta thu được rằng phần tử $d_{\lambda}\cdot 1$ của K là khác không. Ta sẽ thấy về sau (VIII, p. 420, Hệ quả 2) rằng $d_\mu$ chia lực lượng của G.

Cho $\lambda$ là một phần tử của $\widehat{G}$. Ánh xạ $\pi_{\lambda}$ từ K[G] tới End$_K(V_{\lambda})$ gây ra một đẳng cấu các $(K[G]$, K[G])-song môđun từ $e_{\lambda}K[G]$ lên End$_K(V_{\lambda})$. Theo Mệnh đề 15 của VIII, p. 147, K[G]-môđun con $e_{\lambda}K[G]$ là thành phần đẳng kiểu của K[G] thuộc kiểu $\lambda$. Nó cũng là thành phần đẳng kiểu thuộc kiểu $\lambda^{\vee}$ đối với biểu diễn chính quy phải của G (VIII, p. 143, Mệnh đề 11), cũng như thành phần đẳng kiểu thuộc kiểu $\lambda \times \lambda^{\vee}$ đối với biểu diễn hai phía (VIII, p. 381, Mệnh đề 4).

### 6. Các hệ thức trực giao Schur

Ta giữ ký hiệu của tiểu mục trước. Cho $\lambda$ là một phần tử của $\widehat{G}$, và cho $u$ và $v$ là các phần tử của End$_K(V_{\lambda})$; theo công thức (10), ta có

$\widehat{\tau}(j_{\lambda}(u)j_{\lambda}(v)) =d_{\lambda}$ Tr($uv$). Vì $\tau =\widehat{\tau}\circ \mathscr{F}$, ta suy ra từ các công thức (2) và (15) quan hệ

$d^2_{\lambda}|G|^{-1}\sum_{g\in G}$ Tr($u\pi_{\lambda}(g)$) Tr($v\pi_{\lambda}(g^{-1})$) $=d_{\lambda}$ Tr($uv$).

Trước đây ta đã nhận thấy rằng $d_{\lambda}.1\not= 0$ trong trường K; suy ra (20) $|G|^{-1}\sum_{g\in G}$ Tr($u\pi_{\lambda}(g)$) Tr($v\pi_{\lambda}(g^{-1})$) $=d^{-1}_{\lambda}$ Tr($uv$).

Hãy áp dụng quan hệ này cho trường hợp $u$ và $v$ có hạng $\leqslant 1$; ta được (21) $|G|^{-1}\sum_{g\in G}\langle x^*, \pi_{\lambda}(g)x\rangle  \langle y^*, \pi_{\lambda}(g^{-1})y\rangle =d^{-1}_{\lambda}\langle x^*, y\rangle \langle y^*, x\rangle$

với $x,y$ trong $V_{\lambda}$ và $x^*, y^*$ trong đối ngẫu $V^*_{\lambda}$ của $V_{\lambda}$.

Với mọi $\lambda \in \widehat{G}$, cho $(e_{\lambda ,j})_{1\leqslant j\leqslant d_{\lambda}}$ là một cơ sở của $V_{\lambda}$; ký hiệu bởi $(\pi^{\lambda}_{ij}(g))$ ma trận của tự đồng cấu $\pi_{\lambda}(g)$ của $V_{\lambda}$ đối với cơ sở này. Nếu ta ký hiệu bởi $(e^*_{\lambda ,i})_{1\leqslant i\leqslant d_{\lambda}}$ cơ sở của $V^*_{\lambda}$ đối ngẫu với $(e_{\lambda ,j})$, thì ta có $\pi^{\lambda}_{ij}(g) =\langle e^*_{\lambda ,i}, \pi_{\lambda}(g)e_{\lambda ,j}\rangle$, và do đó (22) $|G|^{-1}\sum_{g\in G}\pi_{ij}^{\lambda}(g)\pi^{\lambda}_{k\ell}(g^{-1}) =d^{-1}_{\lambda}\delta_{i\ell}\delta_{jk}$.

Bây giờ cho $\lambda$ và $\mu$ là hai phần tử phân biệt của $\widehat{G}$, và cho $u\in$ End$_K(V_{\lambda})$ và $v\in$ End$_K(V_\mu)$. Lại theo quan hệ (15), ta có (23) $\sum_{g\in G}$ Tr($u\pi_{\lambda}(g)$) Tr($v\pi_\mu(g^{-1})$) $= 0$.

Như trên, ta suy ra rằng (24) $\sum_{g\in G}\langle x^*, \pi_{\lambda}(g)x\rangle  \langle y^*, \pi_\mu(g^{-1})y\rangle = 0$

đối với $x\in V_{\lambda},x^*\in V^*_{\lambda},y\in V_\mu$, và $y^*\in V^*_\mu$. Ta cũng có (25) $\sum_{g\in G}\pi^{\lambda}_{ij}(g)\pi^\mu_{k\ell}(g^{-1}) = 0$ với $i, j$ trong $[1, d_{\lambda}]$ và $k, \ell$ trong $[1, d_\mu]$.

Các hệ thức từ (20) đến (25) được gọi là các hệ thức trực giao Schur.

#### Nhận xét {#alg-viii-s21-n6-rem-1 .statement tag=00NS}

Ta đồng nhất đại số End$_K(V_{\lambda})$ với đại số ma trận $\mathbf{M}_{d_{\lambda}}(K)$ thông qua cơ sở $(e_{\lambda ,j})$ của $V_{\lambda}$. Ánh xạ $\mathscr{F}^{-1}$ là một đẳng cấu từ đại số $\prod_{\lambda}\mathbf{M}_{d_{\lambda}}(K)$ tới đại số K[G]. Với $\mu\in \widehat{G}$, ký hiệu bởi $E^\mu_{ij}$ phần tử của $\prod_{\lambda}\mathbf{M}_{d_{\lambda}}(K)$ mà thành phần có chỉ số $\mu$ là đơn vị ma trận $E_{ij}$ của $\mathbf{M}_{d_\mu}(K)$ (II, §10, No. 3, p. 341) và các thành phần khác của nó là không; đặt $u^\mu_{ij}=\mathscr{F}^{-1}(E^\mu_{ij})$. Họ các phần tử $u^{\lambda}_{ij}$, với $\lambda \in \widehat{G}, 1\leqslant i\leqslant d_{\lambda}$, $1\leqslant j\leqslant d_{\lambda}$, là một cơ sở của đại số K[G]; bảng phép nhân là

$$
u^{\lambda}_{ij}u^\mu_{k\ell}=\delta_{\lambda \mu}\delta_{jk}u^{\lambda}_{i\ell} \tag{26}
$$

Hơn nữa, theo công thức (15), ta có

$$
u^{\lambda}_{ij}=|G|^{-1}d_{\lambda g}\sum_{\in G}\pi^{\lambda}_{ji}(g^{-1})g \tag{27}
$$

### 7. Quan Hệ Trực Giao Cho Các Đặc Trưng

Ta giữ ký hiệu của các Tiểu mục 5 và 6. Nhắc lại rằng Z(K[G]) gồm các hàm trung tâm.

Ta định nghĩa một ánh xạ song tuyến tính đối xứng từ $K[G]\times K[G]$ vào K bởi công thức

$$
\langle f, f'\rangle_G=|G|^{-1}\sum_{g\in G}f_gf'_{g^{-1}} \tag{28}
$$

với mọi $f=\sum f_gg$ và $f'=\sum f_g'g$ thuộc K[G]. Ta có $\langle f, f'\rangle_G=$ $|G|^{-2}\tau (f f')$.

#### Mệnh đề 4 (Quan hệ trực giao cho các đặc trưng) {#alg-viii-s21-prop-4 .statement tag=00SG}

Với $\lambda$ và $\mu$ trong $\widehat{G}$, ta có $\langle \chi_{\lambda}, \chi_\mu\rangle_G=\delta_{\lambda \mu}$.

Đây là trường hợp riêng của các hệ thức (20) và (23) khi các nội cấu $u$ và $v$ được lấy là đồng nhất.

#### Hệ quả {#alg-viii-s21-n7-cor-1 .statement tag=00NT}

Cho $\pi$ và $\pi '$ là các biểu diễn tuyến tính hữu hạn chiều của G. Trong trường K, ta có

(29) $\langle \chi_{\pi}, \chi_{\pi'}\rangle_G=$ (dim$_K$ Hom$_G(\pi , \pi ')$)$\cdot 1$.

Trước hết giả sử rằng $\pi$ và $\pi '$ là các biểu diễn đơn. Không gian vectơ Hom$_G(\pi , \pi ')$ có chiều bằng 1 hoặc 0 tùy theo $\pi$ và $\pi '$ có đẳng cấu với nhau hay không (Bổ đề Schur, VIII, p. 47, Mệnh đề 2). Trong trường hợp này, công thức (29) suy ra từ Mệnh đề 4.

Trong trường hợp tổng quát, biểu diễn $\pi$ (resp. $\pi '$) là tổng trực tiếp của các biểu diễn đơn $\pi_1, . . . , \pi_m$ (resp. $\pi '_1, . . . , \pi '_n$). Không gian Hom$_G(\pi , \pi ')$ đẳng cấu với tổng trực tiếp của các không gian Hom$_G(\pi_i, \pi '_j)$ với $1\leqslant i\leqslant m$, $1\leqslant j\leqslant n$, và ta có

$$
\chi_{\pi}=\chi_{\pi_1}+\cdots +\chi_{\pi_m},\chi_{\pi'}=\chi_{\pi'_1}+\cdots +\chi_{\pi'_n}
$$

Do tính tuyến tính, việc chứng minh công thức (29) được quy về trường hợp các biểu diễn đơn.

### 8. Các Hàm Trung Tâm trên một Nhóm Hữu Hạn

#### Mệnh đề 5 {#alg-viii-s21-prop-5 .statement tag=00NU}

Họ $(\chi_{\lambda})_{\lambda\in\widehat{G}}$ là một cơ sở của không gian vectơ các hàm trung tâm. Số các lớp biểu diễn tuyến tính đơn của G bằng số các lớp liên hợp của G.

Với $a=\sum_{g\in G}a_gg\in K[G]$, viết $a^{\vee}=\sum_{g\in G}a_{g^{-1}}g$; ánh xạ $a\mapsto a^{\vee}$ là một phản tự đẳng cấu đối hợp của đại số K[G]. Theo công thức (17), ta có $e_{\lambda}=|G|^{-1}d_{\lambda}\chi^{\vee}_{\lambda}$ với mọi $\lambda \in \widehat{G}$. Khi đó mệnh đề suy ra từ sự kiện rằng họ $(e_{\lambda})_{\lambda\in\widehat{G}}$ là một cơ sở của tâm của K[G].

Ký hiệu bởi $\mathscr{C}$ tập hợp các lớp liên hợp của G. Cho C là một phần tử của $\mathscr{C}$; ảnh $C^{-1}$ của C qua ánh xạ $g\mapsto g^{-1}$ là một lớp liên hợp. Các chuẩn hóa tử của các phần tử của C là những nhóm con đôi một liên hợp của G; lực lượng của chúng $d(C)$ thỏa mãn

(30) Card(G) = Card(C) $d(C)$.

Đặc biệt, ta có $d(C)\cdot 1\not= 0$ trong trường K.

Cho $f$ là một hàm trung tâm trên G. Với mỗi lớp liên hợp C, ký hiệu bởi $f(C)$ giá trị chung của các $f(x)$ với $x\in C$. Với ký hiệu này, quan hệ trực giao của các đặc trưng (VIII, p. 410, Mệnh đề 4) có thể được viết thành

$$
\sum_{C\in\mathscr{C}}\chi_{\lambda}(C^{-1})\chi_\mu(C)d(C)^{-1}=\delta_{\lambda \mu} \tag{31}
$$

đối với $\lambda$ và $\mu$ trong $\widehat{G}$.

Ký hiệu bởi A ma trận kiểu $\widehat{G}\times \mathscr{C}$ có các phần tử là $\chi_{\lambda}(C)$ và bởi B ma trận kiểu $\mathscr{C}\times \widehat{G}$ có các phần tử là $\chi_{\lambda}(C^{-1})d(C)^{-1}$. Các tập hợp $\widehat{G}$ và $\mathscr{C}$ có cùng lực lượng (Mệnh đề 5); quan hệ (31) biểu thị rằng tích ma trận AB là đơn vị ma trận kiểu $\widehat{G}\times \widehat{G}$. Theo Mệnh đề 11 của II, §10, No. 12, p. 360, tích ma trận BA là đơn vị ma trận kiểu $\mathscr{C}\times \mathscr{C}$; nói cách khác, ta có quan hệ

$$
\sum_{\lambda\in\widehat{G}}\chi_{\lambda}(C^{-1})\chi_{\lambda}(C') =d(C)\delta_{CC'} \tag{32}
$$

với C và $C'$ trong $\mathscr{C}$ (đôi khi được gọi là “quan hệ trực giao thứ hai đối với các đặc trưng”).

Cho H là một nhóm con của G. Chú ý rằng số nguyên Card(H) chia Card(G) và rằng $|G|$ không bằng không trong K; do đó ta có $|H| \not= 0$ trong K.

Ký hiệu bởi Res$^G_H$ ánh xạ tuyến tính từ Z(K[G]) vào Z(K[H]) biến một hàm trung tâm trên G thành hạn chế của nó lên H. Ta đã thấy rằng nếu $\chi_{\pi}$ là đặc trưng của một biểu diễn hữu hạn chiều $\pi$ của G, thì Res$^G_H(\chi_{\pi})$ là đặc trưng của biểu diễn Res$^G_H(\pi )$ của H.

#### Mệnh đề 6 {#alg-viii-s21-prop-6 .statement tag=00NV}

Cho $f$ là một hàm trung tâm trên G và $u$ là một hàm trung tâm trên H. Ta có

(33) $\langle$Ind$^G_H(u), f\rangle_G=\langle u$, Res$^G_H(f)\rangle_H$.

Các đặc trưng của các biểu diễn đơn của G tạo thành một cơ sở của Z(K[G]) (VIII, p. 411, Mệnh đề 5), và điều tương tự cũng đúng với H. Do đó chỉ cần thiết lập (33) trong trường hợp $f$ là đặc trưng $\chi_{\pi}$ của một biểu diễn đơn $\pi$ của G và $u$ là đặc trưng $\chi_{\sigma}$ của một biểu diễn đơn $\sigma$ của H. Trong trường hợp này, Ind$^G_H(u)$ là đặc trưng của biểu diễn Ind$^G_H(\sigma )$ của G, và, theo VIII, p. 410, Hệ quả, ta có

$\langle$Ind$^G_H(u), f\rangle_G=$ (dim$_K$ Hom$_G$(Ind$^G_H(\sigma ), \pi$ ))$\cdot 1$.

Ta chứng minh quan hệ

$\langle u$, Res$^G_H(f)\rangle_H=$ (dim$_K$ Hom$_H(\sigma$, Res$^G_H(\pi )$))$\cdot 1$

tương tự, và đẳng thức (33) suy ra từ tương hỗ Frobenius.

#### Mệnh đề 7 {#alg-viii-s21-prop-7 .statement tag=00NW}

Cho $f$ là một ánh xạ từ G vào K. Các mệnh đề sau là tương đương:

(i) Tồn tại một phần tử $\lambda$ của $\widehat{G}$ và một phần tử $a$ của K sao cho $f=a\chi_{\lambda}$.

(ii) Với mọi cặp $(g, g')$ các phần tử của G, ta có

$$
f(g)f(g') =|G|^{-1}f(1)\sum_{h\in G}f(hgh^{-1}g') \tag{34}
$$

Cho $\lambda$ là một phần tử của $\widehat{G}$; với mọi tự đồng cấu $u$ của $V_{\lambda}$, đặt

$$
u^{\natural}=|G|^{-1}\sum_{h\in G}\pi_{\lambda}(h)u \pi_{\lambda}(h^{-1}) \tag{35}
$$

Tự đồng cấu $u^{\natural}$ của $V_{\lambda}$ là K[G]-tuyến tính. Theo bổ đề Schur (VIII, p. 47, Định lý 1)$,u^{\natural}$ là một phép vị tự. Vì $u$ và $u^{\natural}$ có cùng vết, do đó ta có

$u^{\natural}=d^{-1}_{\lambda}$ Tr($u$) $1_{V_{\lambda}}$.

Cho $u$ và $v$ là các nội cấu của $V_{\lambda}$; suy ra rằng

(36) Tr($u$) Tr($v$) $=d_{\lambda}$ Tr($u^{\natural}v$) $=d_{\lambda}|G|^{-1}\sum_{h\in G}$ Tr($\pi_{\lambda}(h)u \pi_{\lambda}(h^{-1})v$).

Lấy $u=\pi_{\lambda}(g)$ và $v=\pi_{\lambda}(g')$ trong công thức (36); quan hệ (34) đối với $f=\chi_{\lambda}$ suy ra được.

Ngược lại, giả sử rằng mệnh đề (ii) đúng. Nếu ta có $f(1) = 0$, thì suy ra $f(g)f(g') = 0$ với mọi cặp $(g, g')$ các phần tử của G, và do đó $f= 0$. Vì vậy ta có thể giả sử $f(1)\not= 0$. Lấy $g'= 1$ trong (34), ta thu được quan hệ

$$
f(g) =|G|^{-1}\sum_{h\in G}f(hgh^{-1})
$$

với mọi $g\in G$, điều này kéo theo rằng $f$ là một hàm trung tâm. Theo Mệnh đề 5, tồn tại một họ $(a_{\lambda})$ các phần tử của K sao cho $f=\sum_{\lambda\in\widehat{G}}a_{\lambda}\chi_{\lambda}$. Hãy thay thế $f$ bằng biểu thức này trong công thức (34); chú ý rằng mỗi ký số $\chi_{\lambda}$ cũng thỏa mãn quan hệ này, ta được

$$
\sum_{\lambda ,\mu\in\widehat{G}}a_{\lambda}a_\mu\chi_{\lambda}(g)\chi_\mu(g') =\sum_{\lambda\in\widehat{G}}a_{\lambda}d^{-1}_{\lambda}f(1)\chi_{\lambda}(g)\chi_{\lambda}(g') \tag{37}
$$

với $g, g'\in G$. Quan hệ này cũng có thể được viết thành

$$
\sum_{\lambda ,\mu}(a_{\lambda}a_\mu-\delta_{\lambda \mu}a_{\lambda}d^{-1}_{\lambda}f(1))\chi_{\lambda}(g)\chi_\mu(g') = 0 \tag{38}
$$

với $g, g'\in G$. Bây giờ, các hàm $\chi_{\lambda}$, với $\lambda \in \widehat{G}$, là độc lập tuyến tính (Mệnh đề 5 của VIII, p. 411); suy ra rằng

$$
a_{\lambda}a_\mu=\delta_{\lambda \mu}a_{\lambda}d^{-1}_{\lambda}f(1)
$$

với $\lambda , \mu\in \widehat{G}$. Đặc biệt, $a_{\lambda}a_\mu= 0$ mỗi khi $\lambda \not=\mu$. Do đó, tồn tại nhiều nhất một phần tử $\lambda$ của $\widehat{G}$ sao cho $a_{\lambda}\not= 0$, và ta có $f=a_{\lambda}\chi_{\lambda}$, và vì thế (i).

### 9. Trường hợp các nhóm Abel

Trong tiểu mục này, ta giả thiết rằng nhóm G là Abel.

Theo Bổ đề Schur (VIII, p. 48, Hệ quả 1), mọi biểu diễn đơn của G đều có chiều 1. Cho $(M, \pi )$ là một biểu diễn như vậy và $\chi$ là đặc trưng của nó; với mọi $g\in G$ và $x\in M$, ta có $\pi (g)(x) =\chi (g)x$. Do đó, đặc trưng $\chi$ là một đồng cấu từ G vào nhóm nhân $K^*$ của K. Ngược lại, mọi đồng cấu từ G vào $K^*$ đều là đặc trưng của một biểu diễn của G bậc 1. Vậy tập hợp $\widehat{G}$ các lớp các K[G]-môđun đơn có thể được đồng nhất với tập hợp Hom(G$,K^*$) các đồng cấu từ G vào $K^*$. Từ đó suy ra trên $\widehat{G}$ một cấu trúc nhóm Abel; tích trong $\widehat{G}$ tương ứng với tích tenxơ của các biểu diễn. Các nhóm G và $\widehat{G}$ có cùng lực lượng theo Mệnh đề 5 của VIII, p. 411. Mọi hàm trên G đều là trung tâm, và $\widehat{G}$ là một cơ sở của không gian vectơ các ánh xạ từ G vào K (loc. cit.). Do quan hệ trực giao đối với các đặc trưng, một ánh xạ như vậy $f$ có phân tích duy nhất sau đây theo cơ sở $\widehat{G}:$

$$
f=\sum_{\chi\in\widehat{G}}\langle \chi , f\rangle_G\chi \tag{39}
$$

Đối với các ánh xạ $f$ và $f'$ từ G đến K, ta có quan hệ

$$
\langle f, f'\rangle_G=\sum_{\chi\in\widehat{G}}\langle \chi , f\rangle_G\langle \chi , f'\rangle_G \tag{40}
$$

Cho $(V, \pi )$ là một biểu diễn tuyến tính của G. Với mọi $\chi \in \widehat{G}$, ký hiệu bởi $V^{\chi}$ không gian con của V gồm các vectơ $v$ sao cho $\pi (g)(v) =\chi (g)v$ với mọi $g\in G$. Không gian $V^{\chi}$ là thành phần đẳng kiểu kiểu $\chi$ của K[G]-môđun V. Không gian V là tổng trực tiếp của họ $(V^{\chi})_{\chi\in\widehat{G}}$, và phép chiếu $p_{\chi}$ của V có ảnh là $V^{\chi}$ liên kết với phép phân tích này được cho bởi

$$
p_{\chi}=|G|^{-1}\sum_{g\in G}\chi (g^{-1})\pi (g) \tag{41}
$$

do quan hệ (19).

#### Nhận xét {#alg-viii-s21-n9-rem-1 .statement tag=00NX}

Cho $n$ là lực lượng của nhóm G, và gọi $\mu_n(K)$ là nhóm các căn bậc $n$ của đơn vị trong K. Với mọi $g\in G$, ta có $g^n= 1$; do đó, $\widehat{G}$ có thể được đồng nhất với nhóm Hom(G$, \mu_n(K)$). Nhóm $\mu_n(K)$ là cyclic cấp $n$ (V, §11, No. 2, p. 78, Định lý 1). Vì vậy nhóm $\widehat{G}$ đẳng cấu với nhóm D(G) = Hom(G$,\mathbf{Q}/\mathbf{Z}$). Theo VII, §4, No. 9, p. 26, Mệnh đề 10, nhóm $\widehat{G}$ đẳng cấu với nhóm G, và ánh xạ gửi một phần tử $g$ của G tới đồng cấu $\chi \mapsto \chi (g)$ từ $\widehat{G}$ tới $K^*$ là một đẳng cấu từ G tới $\widehat{\widehat{G}}$.

### 10. Các đặc trưng và các nhóm Grothendieck

Ký hiệu bởi $\theta_G$ đồng cấu đại số trên K từ $K\otimes_{\mathbf{Z}}R_K(G)$ vào $\mathscr{Z}_K(G)$ biến $1\otimes [\pi ]$ thành $\chi_{\pi}$ với mọi biểu diễn hữu hạn chiều $\pi$.

#### Mệnh đề 8 {#alg-viii-s21-prop-8 .statement tag=00NY}

a) Đồng cấu $\theta_G$ là một đẳng cấu từ $K\otimes_{\mathbf{Z}}R_K(G)$ lên $\mathscr{Z}_K(G)$.

b) Giả sử rằng K có đặc số 0. Khi đó $\theta_G$ xác định một đẳng cấu từ $R_K(G)$ lên vành con của $\mathscr{Z}_K(G)$ gồm các tổ hợp tuyến tính của các đặc trưng $\chi_{\lambda}$, với $\lambda$ trong $\widehat{G}$, có hệ số nguyên.

Họ $([\lambda ])_{\lambda\in\widehat{G}}$ là một cơ sở của $\mathbf{Z}$-môđun $R_K$(G), và họ $(\chi_{\lambda})_{\lambda\in\widehat{G}}$ là một cơ sở của không gian vectơ trên K $\mathscr{Z}_K(G)$. Các khẳng định a) và b) suy ra từ đó (VIII, p. 411, Mệnh đề 5).

### 11. Chiều của các biểu diễn đơn

Ký hiệu lực lượng của nhóm G là $n$. Cho $\pi$ là một biểu diễn tuyến tính của G trong một không gian vectơ trên K hữu hạn chiều M. Với mọi $g\in G$, ta có $\pi (g)^n= 1_M$, nên đa thức tối tiểu của $\pi (g)$ chia hết $T^n-1$. Vì $n\cdot 1\not= 0$ trong K, đa thức tối tiểu này là tách được (V, §11, No. 2, p. 78), và vì trường K là đóng đại số, tự đồng cấu $\pi (g)$ của M là chéo hóa được (VII, §5, No. 7, p. 40, Mệnh đề 12). Các trị riêng của $\pi (g)$ là các nghiệm bậc $n$ của đơn vị, và với mọi $\alpha \in K$, bội số hình học của $\alpha$ như một trị riêng của $\pi (g)$ (VII, §5, No. 2, p. 30, Định nghĩa 1) bằng bội số của $\alpha$ như một nghiệm của đa thức đặc trưng của $\pi (g)$. Ký hiệu bởi $\mathscr{O}_n$ nhóm con của K sinh bởi tập hợp $\mu_n(K)$ các nghiệm bậc $n$ của đơn vị; đó là một $\mathbf{Z}$-môđun sinh hữu hạn và một vành con của K. Đặc trưng của $\pi$ nhận các giá trị trong $\mathscr{O}_n$.

#### Mệnh đề 9 {#alg-viii-s21-prop-9 .statement tag=00NZ}

Giả sử trường K có đặc số không. Khi đó bậc của mọi biểu diễn đơn của G là ước của lực lượng của G.

Cho $(V, \pi )$ là một biểu diễn đơn của G và $\chi$ là đặc trưng của nó. Với mọi phần tử $a$ của Z(K[G]), tự đồng cấu $\pi (a)$ của V là một phép vị tự (VIII, p. 47, Định lý 1); ký hiệu bởi $\varphi (a)$ vô hướng sao cho $\pi (a) =\varphi (a)_V$. Ánh xạ thu được $\varphi$ từ Z(K[G]) vào K là một đồng cấu đại số. Lấy $a=\sum_{g\in G}\chi (g^{-1})g$; theo nhận xét ở VIII, p. 408, ta có $\varphi (a) =$ (dim $V$)$^{-1}|G|$. Mặt khác, $a$ thuộc vành con $\mathscr{O}_n[G]\cap Z(K[G])$ của K[G], là một $\mathbf{Z}$-môđun sinh hữu hạn (VII, §3, p. 15, Hệ quả). Vậy phần tử $\varphi (a) =$ (dim $V$)$^{-1}|G|$ của K thuộc một vành con của K là một $\mathbf{Z}$-môđun sinh hữu hạn. Ta kết luận bằng cách sử dụng bổ đề sau.

#### Bổ đề {#alg-viii-s21-n11-lem-1 .statement tag=00O0}

Cho L là một mở rộng của $\mathbf{Q}$. Cho A là một vành con của L. Giả sử rằng A là một $\mathbf{Z}$-môđun sinh hữu hạn. Ta có $A\cap \mathbf{Q}=\mathbf{Z}$.

Vì $\mathbf{Z}$-môđun $A\cap \mathbf{Q}$ sinh hữu hạn, nên tồn tại một số nguyên dương ngặt N sao cho $A\cap \mathbf{Q}$ được chứa trong $\frac{1}{N}\mathbf{Z}$. Cho $x$ là một phần tử của $\mathbf{Q}-\mathbf{Z}$; ta viết nó dưới dạng $x=\frac{p}{q}$, trong đó $p$ và $q$ là các số nguyên nguyên tố cùng nhau và $q\geqslant 2$. Ta có $q^N\geqslant 2^N>N ($Lý thuyết tập hợp, III, §3, No. 6, p. 165, Định lý 2), các số nguyên $p^N$ và $q^N$ là nguyên tố cùng nhau, và do đó $x^N\notin\frac{1}{N}\mathbf{Z}$. Suy ra $x$ không thuộc A. Điều này kết thúc chứng minh của bổ đề.

Trong tiểu mục tiếp theo, chúng tôi mở rộng Mệnh đề 9 cho trường hợp chỉ giả thiết rằng đặc số của K không chia hết cấp của G.

### 12. Đổi trường cơ sở

Ta giữ ký hiệu của tiểu mục trước. Cho $K'$ là một trường đóng đại số sao cho phần tử $n\cdot 1$ của $K'$ khác không. Các nhóm $\mu_n(K)$ và $\mu_n(K')$ là các nhóm cyclic cấp $n$ (V, §11, No. 2, p. 78, Định lý 1). Chọn một đẳng cấu $\varphi$ từ $\mu_n(K)$ lên $\mu_n(K')$. Cho $\pi$ là một biểu diễn tuyến tính của G trong một không gian vectơ hữu hạn chiều trên K, và cho $\pi '$ là một biểu diễn tuyến tính của G trong một không gian vectơ hữu hạn chiều trên $K'$ . Ta nói rằng $\pi$ và $\pi '$ là liên quan (thông qua $\varphi$ ) nếu với mọi $g\in G$ và $\omega \in \mu_n$(K), bội số của $\omega$ như một trị riêng của $\pi (g)$ bằng bội số của $\varphi (\omega )$ như một trị riêng của $\pi '(g)$. Khi đó, $\pi$ và $\pi '$ có cùng chiều, như thấy được khi lấy $g= 1$.

Cho $\pi_1$ và $\pi_2$ (resp. $\pi '_1$ và $\pi '_2$) là các biểu diễn tuyến tính của G trong các không gian vectơ hữu hạn chiều trên K (resp. $K'$). Ta có các tính chất sau:

a) Nếu $\pi_1$ liên quan với $\pi '_1$ và $\pi '_2$, thì $\pi '_1$ và $\pi '_2$ đẳng cấu.

b) Nếu $\pi_1$ liên quan với $\pi '_1$ và $\pi_2$ liên quan với $\pi '_2$, thì $\pi_1\oplus \pi_2$ liên quan với $\pi '_1\oplus \pi '_2$ và $\pi_1\otimes \pi_2$ liên quan với $\pi '_1\otimes \pi '_2$.

Mệnh đề a) suy ra từ Hệ quả 5 của VIII, p. 402, và mệnh đề b) là hiển nhiên.

Ở đây, ta ký hiệu bởi $\mathscr{S}_K(G)$ tập hợp các lớp của các K[G]-môđun đơn, trước đây được ký hiệu bởi $\widehat{G}$, và ta cũng định nghĩa $\mathscr{S}_{K'}(G)$ tương tự. Các tập hợp $\mathscr{S}_K(G)$ và $\mathscr{S}_{K'}(G)$ đều hữu hạn, với lực lượng bằng số các lớp liên hợp (VIII, p. 411, Mệnh đề 5).

#### Mệnh đề 10 {#alg-viii-s21-prop-10 .statement tag=00O1}

Tồn tại một ánh xạ duy nhất $\varphi_G$ từ $\mathscr{S}_K(G)$ vào $\mathscr{S}_{K'}(G)$ sao cho $\lambda$ và $\varphi_G(\lambda )$ liên quan với nhau qua $\varphi$ đối với mọi $\lambda$ trong $\mathscr{S}_K(G)$. Hơn nữa, $\varphi_G$ là song ánh.

Tính duy nhất của $\varphi_G$ suy ra từ tính chất a) ở trên.

A) Giả sử trường K có đặc số 0.

Nhóm $\mu_n(K)$ là cyclic (V, §11, No. 2, p. 78, Định lý 1); chọn một phần tử sinh $\zeta$ của nhóm này. Xét đồng cấu vành $\rho :\mathbf{Z}[X]\rightarrow \mathscr{O}_n$ gửi X tới $\zeta$. Nó là toàn ánh. Đa thức cyclotomic $\Phi_n(X)$ là bất khả quy trong $\mathbf{Q}[X]$ (V, §11, No. 5, p. 84, Định lý 2); do đó nó là đa thức tối tiểu của $\zeta$ trên $\mathbf{Q}$. Đa thức $\Phi_n$ có hệ số đầu bằng 1 và các hệ số nguyên (V, §11, No. 4, p. 81). Cho $P\in \mathbf{Z}[X]$ là một đa thức sao cho $P(\zeta ) = 0$; nhờ phép chia Euclid của các đa thức (IV, §1, No. 6, p. 10), tồn tại hai đa thức Q và R trong $\mathbf{Z}[X]$ sao cho P = QΦ$_n+ R$ và deg(R) $<$ deg(Φ$_n$). Ta có $R(\zeta ) = 0$, và do đó R = 0 vì $\Phi_n$ là đa thức tối tiểu của $\zeta$. Do đó, hạt nhân của $\rho$ là iđêan $\Phi_n\mathbf{Z}[X]$ của $\mathbf{Z}[X]$, và $\rho$ cảm sinh một đẳng cấu vành từ $\mathbf{Z}[X]/\Phi_n\mathbf{Z}[X]$ đến $\mathscr{O}_n$.

Đặt $\zeta '=\varphi (\zeta )$; đó là một nghiệm nguyên thủy bậc $n$ của đơn vị trong $K'$, và do đó ta có $\Phi_n(\zeta ') = 0$ (V, §11, No. 5, p. 83, Bổ đề 3). Do đó, tồn tại một đồng cấu $\varphi_0$ từ vành $\mathscr{O}_n$ đến trường $K'$ đưa $\zeta$ thành $\zeta '$; nó mở rộng ánh xạ $\varphi$ từ $\mu_n(K)$ đến $\mu_n(K')$. Cho $\mathscr{O}$ là vành con của K gồm các phần tử $\frac{a}{n^r}$ với $a\in \mathscr{O}_n$ và $r\in \mathbf{N}$. Vì $n\cdot 1$ khả nghịch trong $K'$, đồng cấu $\varphi_0$ mở rộng thành một đồng cấu $\varphi_1$ từ $\mathscr{O}$ đến $K'$.

Đồng nhất đại số $\mathscr{O}[G]$ của nhóm G trên $\mathscr{O}$ với một vành con của đại số K[G] và định nghĩa một đồng cấu vành Φ từ $\mathscr{O}[G]$ đến $K'[G]$ bởi công thức

$$
\Phi (\sum_{g\in G}a_gg)=\sum_{g\in G}\varphi_1(a_g)g \tag{42}
$$

Đặt $\mathscr{C}$ là tập hợp các lớp liên hợp của G. Với C thuộc $\mathscr{C}$, đặt $u_C$ là phần tử $\sum_{g\in C}g$ của $\mathscr{O}[G]$; họ $(u_C)_{C\in\mathscr{C}}$ là một cơ sở trên $\mathscr{O}$ của tâm $Z(\mathscr{O}[G])$ của đại số $\mathscr{O}[G]$ (VIII, p. 398). Với mọi phần tử $\lambda$ của $\mathscr{S}_K$(G), ký hiệu $\chi_{\lambda}$ là đặc trưng của nó, $d_{\lambda}$ là chiều của nó, và $e_{\lambda}$ là phần tử của K[G] được xác định bởi

$$
e_{\lambda}=|G|^{-1}d_{\lambda}\sum_{g\in G}\chi_{\lambda}(g^{-1})g \tag{43}
$$

Họ $(e_{\lambda})$ là một cơ sở trên K của tâm Z(K[G]) của vành K[G] (VIII, p. 408). Ta có

$$
e_{\lambda}=\sum_{C\in\mathscr{C}}\alpha_{\lambda ,C}u_C \tag{44}
$$

với

$$
\alpha_{\lambda ,C}=|G|^{-1}d_{\lambda}\chi_{\lambda}(C^{-1}) \tag{45}
$$

Với $C\in \mathscr{C}$ và $\lambda \in \mathscr{S}_K$(G), đặt $\beta_{C,\lambda}=|G|d^{-1}_{\lambda}d(C)^{-1}\chi_{\lambda}(C)$. Các phần tử của ma trận $(\alpha_{\lambda ,C})$ đều thuộc $\mathscr{O}$, và từ công thức (31) của VIII, p. 411 suy ra rằng ma trận nghịch đảo của nó là ma trận $(\beta_{C,\lambda})$, mà các phần tử cũng đều thuộc $\mathscr{O}$ theo Mệnh đề 9 của VIII, p. 415. Do đó, họ $(e_{\lambda})$ là một cơ sở của $\mathscr{O}$-môđun $Z(\mathscr{O}[G])$.

Các phần tử $\Phi (u_C) =\sum_{g\in C}g$ của $K'[G]$ tạo thành một cơ sở trên $K'$ của tâm $Z(K'[G])$ của vành $K'[G]$. Ta có

$$
\Phi (e_{\lambda}) =\sum_{C\in\mathscr{C}}\varphi_1(\alpha_{\lambda ,C}) \Phi (u_C) \tag{46}
$$

và ma trận có các phần tử $\varphi_1(\alpha_{\lambda ,C})$ là khả nghịch. Do đó, họ các $\Phi (e_{\lambda})$ là một cơ sở của $Z(K'[G])$. Họ $(e_{\lambda})$ là một phân hoạch của lũy đẳng 1 trong Z(K[G]) (VIII, p. 146 và p. 408); nói cách khác, ta có

$\sum_{\lambda}e_{\lambda}= 1,e^2_{\lambda}=e_{\lambda},e_{\lambda}e_\mu= 0$ nếu $\lambda \not=\mu$.

Suy ra rằng họ các $\Phi (e_{\lambda})$ là một phân hoạch của lũy đẳng 1 trong $Z(K'[G])$; vì họ này là một cơ sở của $Z(K'[G])$ trên $K'$, nên các phần tử của nó là các lũy đẳng không phân tích được trong $Z(K'[G])$ (VIII, p. 148, Nhận xét 4).

Với $\lambda '$ trong $\mathscr{S}_{K'}$(G), định nghĩa $\chi_{\lambda'},d_{\lambda'}$, và $e_{\lambda'}$ như trên. Theo VIII, p. 408, các phần tử $e_{\lambda'}$ là các phần tử lũy đẳng không phân tích được trong $Z(K'[G])$. Do đó tồn tại một song ánh $\varphi_G$ từ $\mathscr{S}_K(G)$ đến $\mathscr{S}_{K'}(G)$ sao cho $\Phi (e_{\lambda}) =e_{\varphi_G(\lambda)}$ với mọi $\lambda$ trong $\mathscr{S}_K(G)$.

Cho $\lambda$ trong $\mathscr{S}_K(G)$; đặt $\lambda '=\varphi_G(\lambda )$. Cho $(V_{\lambda}, \pi_{\lambda})$ (tương ứng $(V_{\lambda'}, \pi_{\lambda'})$) là một biểu diễn tuyến tính của G mà K[G]-môđun liên kết (tương ứng $K'$[G]-môđun) có lớp $\lambda$ (tương ứng $\lambda '$). Ta chứng minh rằng $\lambda$ và $\lambda '$ có liên quan. Cho $g$ là một phần tử của G. Cho $\delta (T)$ là định thức của tự đồng cấu $1 + T\pi_{\lambda}(g)$ của K[T]-môđun $K[T]\otimes_KV_{\lambda}$. Cho $\omega_1, . . . , \omega_{d_{\lambda}}$ là các giá trị riêng của $\pi_{\lambda}(g)$; ta có

$$
\delta (T) = (1 + T\omega_1)\cdots (1 + T\omega_{d_{\lambda}})
$$

Ta cũng định nghĩa $\delta '(T)$ như vậy, và ký hiệu các giá trị riêng của $\pi_{\lambda'}(g)$ là $\omega '_1, . . . , \omega '_{d_{\lambda'}}$. Môđun $\mathscr{O}$ $\mathscr{O}[G]$ là tự do với cơ sở G, và không gian vectơ trên K K[G] có cơ sở G. Ký hiệu Δ(T) là định thức của phép nhân với $1 +e_{\lambda}gT$ trong $\mathscr{O}$[T]-môđun $\mathscr{O}[T]\otimes_{\mathscr{O}}\mathscr{O}[G]$. Nó cũng là định thức của phép nhân với $1 +e_{\lambda}gT$ trong K[T]-môđun $K[T]\otimes_KK[G]$. Cho $\overline{\varphi}_1$ là đồng cấu từ $\mathscr{O}[T]$ vào $K'[T]$ mở rộng $\varphi_1$ và gửi T thành T. Vì G là một cơ sở của không gian vectơ trên $K'$ $K'[G]$, đa thức $\overline{\varphi}_1(\Delta (T))$ bằng định thức $\Delta '(T)$ của phép nhân với $1 +e_{\lambda'}gT$ trong không gian vectơ trên $K'$ $K'[G]$.

Đại số K[G] là tổng trực tiếp của các thành phần đơn $e_\mu K[G]$ với $\mu$ chạy qua $\mathscr{S}_K(G)$. Với $\mu$ khác $\lambda$, phần tử $e_{\lambda}g$ triệt tiêu $e_\mu K[G]$. Hơn nữa, phép nhân với $e_{\lambda}g$ trùng với phép nhân với $g$ trong $e_{\lambda}K[G]$. Theo VIII, p. 409 và Ví dụ 6 của VIII, p. 400, biểu diễn của G trong $e_{\lambda}K[G]$ là tổng trực tiếp của $d_{\lambda}$ biểu diễn của lớp $\lambda$. Do đó ta có $\Delta (T) =\delta (T)^{d_{\lambda}}$.

Tương tự, ta có $\Delta '(T) =\delta '(T)^{d_{\lambda'}}$.

Từ quan hệ $\Delta '(T) =\overline{\varphi}_1$(Δ(T)), trước hết suy ra $d^2_{\lambda}=d^2_{\lambda'}$, và do đó $d_{\lambda}=d_{\lambda'}$, rồi tiếp theo dãy $\varphi (\omega_1), . . . , \varphi (\omega_{d_{\lambda}})$ có thể được suy ra từ dãy $(\omega '_1, . . . , \omega '_{d'_{\lambda'}})$ bằng một phép hoán vị của tập hợp các chỉ số.

Vì điều này đúng với mọi phần tử $g$ của G, nên các biểu diễn $\lambda$ và $\lambda '$ có liên quan. Vậy chúng ta đã chứng minh xong Mệnh đề 10 khi trường K có đặc số 0.

B) Trường hợp tổng quát.

Cho L là một trường đóng đại số có đặc số 0 (chẳng hạn, một bao đóng đại số của $\mathbf{Q}$). Ký hiệu $\mathscr{S}_L(G)$ là tập hợp các lớp của các L[G]-môđun đơn. Chọn một đẳng cấu $\eta$ từ nhóm $\mu_n(L)$ sang nhóm $\mu_n$(K), và đặt $\eta '=\varphi \circ \eta$. Theo phần A) của chứng minh, tồn tại các song ánh

$$
\eta_G:\mathscr{S}_L(G)\rightarrow \mathscr{S}_K(G),\eta '_G:\mathscr{S}_L(G)\rightarrow \mathscr{S}_{K'}(G)
$$

với tính chất sau: với mọi $\lambda$ trong $\mathscr{S}_L$(G), các biểu diễn $\lambda$ và $\eta_G(\lambda )$ liên quan qua $\eta$, và các biểu diễn $\lambda$ và $\eta '_G(\lambda )$ liên quan qua $\eta '$. Song ánh $\varphi_G=\eta '_G\circ \eta_G^{-1}$ có các tính chất mong muốn.

Song ánh $\varphi_G$ từ $\mathscr{S}_K(G)$ đến $\mathscr{S}_{K'}(G)$ được mở rộng thành một đẳng cấu, cũng ký hiệu bởi $\varphi_G$, từ nhóm Grothendieck $R_K(G)$ đến nhóm $R_{K'}(G)$.

#### Nhận xét 1 {#alg-viii-s21-n12-rem-1 .statement tag=00O2}

Giả sử rằng $K'$ là một mở rộng của K và đẳng cấu $\varphi$ là ánh xạ $\xi \mapsto \xi \cdot 1$; khi đó ánh xạ $\varphi_G$ được cho bởi phép mở rộng vô hướng từ K đến $K'$.

#### Hệ quả 1 {#alg-viii-s21-prop-10-cor-1 .statement tag=00O3}

Ánh xạ $\varphi_G$ là một đẳng cấu vành từ $R_K(G)$ đến $R_{K'}(G)$. Với mọi biểu diễn hữu hạn chiều $\pi$ của G trong một không gian vectơ trên K, ta có $\varphi_G([\pi ]) = [\pi ']$, trong đó $\pi '$ là một biểu diễn liên quan đến $\pi$ qua $\varphi$.

Điều này suy ra từ tính chất nửa đơn của các biểu diễn của G và tính chất b) của VIII, p. 416.

#### Hệ quả 2 {#alg-viii-s21-prop-10-cor-2 .statement tag=00O4}

Chiều của mỗi biểu diễn đơn của G chia hết cho cấp của G.

Điều này suy ra từ Mệnh đề 10 và Mệnh đề 9 của VIII, p. 415.

#### Nhận xét 2 {#alg-viii-s21-n12-rem-2 .statement tag=00O5}

Giả sử nhóm G là Abel. Ta đã thấy trong nhận xét của VIII, p. 414 rằng $\mathscr{S}_K(G)$ có thể được đồng nhất với tập Hom(G$, \mu_n(K)$). Tương tự, $\mathscr{S}_{K'}(G)$ có thể được đồng nhất với Hom(G$, \mu_n(K')$). Với các đồng nhất này, song ánh $\varphi_G$ chỉ là ánh xạ $\chi \mapsto \varphi \circ \chi$.

#### Nhận xét 3 {#alg-viii-s21-n12-rem-3 .statement tag=00O6}

Cho $\pi_1$ và $\pi_2$ là các biểu diễn tuyến tính của G trong các không gian vectơ hữu hạn chiều trên K. Với $i= 1,2$, gọi $\pi '_i$ là một biểu diễn liên quan với $\pi_i$ qua $\varphi$. Ta có

(47) dim$_K$ Hom$_K(\pi_1, \pi_2) =$ dim$_{K'}$ Hom$_{K'}(\pi '_1, \pi '_2)$.

Chứng minh theo chứng minh của Hệ quả VIII, p. 410, bằng cách quy về trường hợp khi các $\pi_i$ (và do đó các $\pi '_i$) là đơn.

#### Nhận xét 4 {#alg-viii-s21-n12-rem-4 .statement tag=00O7}

Cho H là một nhóm con của G có lực lượng $m$. Đẳng cấu $\varphi$ hạn chế thành một đẳng cấu từ $\mu_m(K)$ đến $\mu_m(K')$ và, do đó, một đẳng cấu vành $\varphi_H$ từ $R_K(H)$ đến $R_{K'}(H)$. Các sơ đồ sau giao hoán:

$R_K(G)^{Res^G_H}$ // $R_K(H)R_K(H)^{Ind^G_H}$ // $R_K(G)$

$\varphi_G\varphi_H\varphi_H\varphi_G$

$R_{K'}(G)^{Res^G_H}/$/ $R_{K'}(H),R_{K'}(H)^{Ind^G_H}/$/ $R_{K'}(G)$.

Tính giao hoán của biểu đồ thứ nhất là hiển nhiên, và tính giao hoán của biểu đồ thứ hai suy ra từ đó nhờ luật tương hỗ Frobenius và công thức (47).

#### Nhận xét 5 {#alg-viii-s21-n12-rem-5 .statement tag=00O8}

Giả sử G là tích $G'\times G''$ của hai nhóm hữu hạn. Ta định nghĩa các đẳng cấu $\varphi_{G'}$ và $\varphi_{G''}$ như trong ví dụ trước.

Ta có một biểu đồ giao hoán

$R_K(G')\otimes_{\mathbf{Z}}R_K(G'')^{\kappa}$ // $R_K(G)$

$\varphi_{G'}\otimes \varphi_{G''}\varphi_G$

$R_{K'}(G')\otimes_{\mathbf{Z}}R_{K'}(G'')^{\kappa'}$ // $R_{K'}(G)$.

nơi các đẳng cấu $\kappa$ và $\kappa '$ là những đẳng cấu được xác định trong VIII, p. 406.

### \*13. Biểu diễn tuyến tính phức

Trong tiểu mục này, ta giả sử rằng K là trường $\mathbf{C}$ của các số phức.

Cho $(M, \pi )$ là một biểu diễn tuyến tính của G. Ta nói rằng một dạng Hermit Φ trên M là bất biến dưới G nếu ta có

$$
\Phi (\pi (g)x, \pi (g)x') = \Phi (x, x') \tag{48}
$$

với mọi $x, x'\in M$ và mọi $g\in G$. Điều này cũng có nghĩa là với mọi $g\in G$, tự đẳng cấu $\pi (g)$ của M là đơn vị đối với Φ.

#### Mệnh đề 11 {#alg-viii-s21-prop-11 .statement tag=00O9}

Cho $(M, \pi )$ là một biểu diễn tuyến tính hữu hạn chiều của G.

a) Trên M tồn tại một dạng Hermit vừa dương, vừa phân biệt, vừa bất biến dưới G.

b) Giả sử rằng biểu diễn $\pi$ là đơn. Nếu Φ và Ψ là các dạng Hermit khác không trên M bất biến dưới G, thì tồn tại một số thực $a$ sao cho $\Psi  =a\Phi$.

Chọn một dạng Hermit dương phân biệt trên không gian vectơ M, và ký hiệu nó là $\Phi_0$. Ta định nghĩa một dạng Hermit dương phân biệt Φ bất biến dưới G bằng cách đặt

$$
\Phi (x, x') =\sum_{g\in G}\Phi_0(\pi (g)x, \pi (g)x') \tag{49}
$$

for $x, x'\in M$.

Cho Ψ là một dạng Hermit trên M; tồn tại duy nhất một tự đồng cấu A của M sao cho $\Psi (x, x') = \Phi (x,Ax')$ với $x, x'$ trong M. Nếu, hơn nữa, Ψ là bất biến dưới G, thì tự đồng cấu A giao hoán với tự đẳng cấu $\pi (g)$ với $g\in G$. Nếu biểu diễn $\pi$ là đơn, thì theo Bổ đề Schur (VIII, p. 47, Định lý 1), A là một phép vị tự và do đó tồn tại một số phức $a$ sao cho $\Psi  =a\Phi$. Vì Φ và Ψ là Hermit và Φ khác không, $a$ là một số thực. Mệnh đề theo sau.

Ta trang bị cho không gian vectơ $\mathbf{C}[G]$ của các hàm phức trên G cấu trúc không gian Hilbert có tích vô hướng được cho bởi

$$
\langle f|f'\rangle_G=|G|^{-1}\sum_{g\in G}\overline{f(g)}f'(g) \tag{50}
$$

Với mỗi hàm $f\in \mathbf{C}[G]$, ta ký hiệu $f^*$ là hàm được xác định bởi

$$
f^*(g) =\overline{f(g^{-1})} \tag{51}
$$

với $g\in G$; ánh xạ $f\mapsto f^*$ là một đối hợp nửa tuyến tính của $\mathbf{C}[G]$. Chúng ta cũng có

$$
\langle f|f'\rangle_G=\langle f^*, f'\rangle_G \tag{52}
$$

với $f, f'\in \mathbf{C}[G]$, theo ký hiệu của công thức (28) của VIII, p. 410. Do đó ta có

$$
\langle f|f'\rangle_G=|G|^{-2}\tau (f^*f') \tag{53}
$$

Cho $(M, \pi )$ là một biểu diễn tuyến tính hữu hạn chiều của G. Ta trang bị cho không gian vectơ M cấu trúc của một không gian Hilbert sao cho các tự đồng cấu $\pi (g)$ là đơn vị (Mệnh đề 11). Nếu ký hiệu $A^*$ là tự đồng cấu liên hợp của một tự đồng cấu A của M đối với cấu trúc này, thì ta có Tr(A$^*$) $=$ Tr(A). Với mọi $g\in G$, ta có $\pi (g^{-1}) =\pi (g)^*$, và do đó $\chi_{\pi}(g^{-1}) =\chi_{\pi}(g)$; nói cách khác, ta có $\chi_{\pi}=\chi^*_{\pi}$. Quan hệ trực giao của các ký tự (VIII, p. 410, Mệnh đề 4) khi đó có dạng

$$
\langle \chi_{\lambda}|\chi_\mu\rangle_G=\delta_{\lambda \mu} \tag{54}
$$

với $\lambda , \mu\in \widehat{G}$. Nó diễn tả rằng họ các ký hiệu đặc trưng $(\chi_{\lambda})_{\lambda\in\widehat{G}}$ của các biểu diễn đơn của G là một cơ sở trực chuẩn của không gian Hilbert $Z(\mathbf{C}[G])$ của các hàm trung tâm.

Cho $\pi$ và $\pi '$ là các biểu diễn tuyến tính hữu hạn chiều của G. Ta có quan hệ $\langle \chi_{\pi}|\chi_{\pi'}\rangle_G=$ dim$_{\mathbf{C}}$ Hom$_G(\pi , \pi ')$ (VIII, p. 410, Hệ quả). Biểu diễn $\pi$ là bất khả quy khi và chỉ khi $\langle \chi_{\pi}|\chi_{\pi}\rangle_G= 1$.

Với mọi phần tử $\lambda$ của $\widehat{G}$, ta trang bị cho không gian vectơ $V_{\lambda}$ cấu trúc của một không gian Hilbert sao cho các tự đẳng cấu $\pi_{\lambda}(g)$ là đơn vị. Ta ký hiệu $\langle v|v'\rangle_{\lambda}$ là tích vô hướng của hai phần tử $v, v'$ của $V_{\lambda}$ và $u^*$ là toán tử liên hợp của một tự đồng cấu $u$ của $V_{\lambda}$. Cho $A = (A_{\lambda})_{\lambda\in\widehat{G}}$ và $A'= (A'_{\lambda})_{\lambda\in\widehat{G}}$ là các phần tử của $F(\widehat{G})$. Ta viết $A^*= (A^*_{\lambda})_{\lambda\in\widehat{G}}$. Ta có $\mathscr{F}(a^*) = (\mathscr{F}(a))^*$ với mọi phần tử $a$ của $\mathbf{C}[G]$. Đặt (55) $\langle A|A'\rangle_{\widehat{G}}=|G|^{-2}\widehat{\tau}(A^*A')$. Theo công thức (10) của VIII, p. 407, ta có

(56) $\langle A|A'\rangle_{\widehat{G}}=\frac{1}{|G|^2}\sum_{\lambda\in\widehat{G}}d_{\lambda}$ Tr(A$^*_{\lambda}$A$'_{\lambda}$).

Vì $\widehat{\tau}\circ \mathscr{F}=\tau$, các công thức (53) và (55) suy ra rằng ánh xạ $\mathscr{F}$ là một đẳng cấu của các không gian Hilbert từ $\mathbf{C}[G]$ đến $F(\widehat{G})$.

Các hệ thức trực giao Schur (VIII, p. 410) có thể được phát biểu lại bằng các tích nội Hilbert. Khi đó các hệ thức (21) và (24) cho các khẳng định sau đây. Với $\lambda \in \widehat{G}$ và $x, x', y, y'$ trong $V_{\lambda}$, ta có (57) $|G|^{-1}\sum_{g\in G}\overline{\langle x|\pi_{\lambda}(g)x'\rangle}_{\lambda}\langle y|\pi_{\lambda}(g)y'\rangle_{\lambda}=d^{-1}_{\lambda}\overline{\langle x|y\rangle}_{\lambda}\langle x'|y'\rangle_{\lambda}$.

Nếu $\lambda$ và $\mu$ là hai phần tử phân biệt của $\widehat{G}$, thì với $x, x'$ trong $V_{\lambda}$ và $y, y'$ trong $V_\mu$, ta có (58) $\sum_{g\in G}\overline{\langle x|\pi_{\lambda}(g)x'\rangle}_{\lambda}\langle y|\pi_\mu(g)y'\rangle_\mu= 0$.

Với mọi $\lambda \in \widehat{G}$, ta chọn một cơ sở trực chuẩn $(e_{\lambda ,i})_{1\leqslant i\leqslant d_{\lambda}}$ của $V_{\lambda}$. Với mọi $g\in G$, ta ký hiệu bởi $(\pi^{\lambda}_{ij}(g))$ ma trận của tự đồng cấu $\pi_{\lambda}(g)$ của $V_{\lambda}$ đối với cơ sở này; ta có (59) $\pi^{\lambda}_{ij}(g) =\langle e_{\lambda ,i}|\pi_{\lambda}(g)e_{\lambda ,j}\rangle_{\lambda}$.

Vì tự đồng cấu $\pi_{\lambda}(g)$ là đơn vị, nên nghịch đảo của nó bằng $\pi_{\lambda}(g)^*$, do đó (60) $\overline{\pi^{\lambda}_{ij}(g)}=\pi^{\lambda}_{ji}(g^{-1})$. Từ các công thức (22) của VIII, p. 409 và (25), p. 409 suy ra rằng các hàm $(d_{\lambda})^{1/2}\pi_{ij}^{\lambda}$, với $\lambda \in \widehat{G},1\leqslant i\leqslant d_{\lambda},1\leqslant j\leqslant d_{\lambda}$, tạo thành một cơ sở trực chuẩn của không gian Hilbert $\mathbf{C}[G].*$

### Bài tập {#alg-viii-s21-exercises}

Xem [các bài tập cho § 21](exercises/s21/).

[^1]: Các phần tử của Hom$_G(\pi , \pi ')$ đôi khi được gọi là các toán tử xen kẽ của $\pi$ và $\pi '$.
