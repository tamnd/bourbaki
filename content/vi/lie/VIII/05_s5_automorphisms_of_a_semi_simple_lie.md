---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: VIII
chapter_title: SPLIT SEMI-SIMPLE LIE ALGEBRAS
section: 5
section_title: Automorphisms of a semi-simple Lie algebra
lang: vi
source: lie-vii-ix
book_pages: 106-115, 233-237
pdf_pages: 0114-0123, 0241-0245
extraction: native+ocr
subsections:
    - "no": 1
      title: AUTOMORPHISMS OF A FRAMED SEMI-SIMPLE LIE ALGEBRA
      page: 106
      pdf_page: 114
    - "no": 2
      title: AUTOMORPHISMS OF A SPLIT SEMI-SIMPLE LIE ALGEBRA
      page: 107
      pdf_page: 115
    - "no": 3
      title: AUTOMORPHISMS OF A SPLITTABLE SEMI-SIMPLE LIE ALGEBRA
      page: 111
      pdf_page: 119
    - "no": 4
      title: ZARISKI TOPOLOGY ON Aut($\mathfrak{g}$)
      page: 113
      pdf_page: 121
    - "no": 5
      title: LIE GROUP CASE
      page: 115
      pdf_page: 123
statements: 25
exercises: 13
errata:
    - says: Chap. VII, §13, no. 1
      read: Chap. VIII, §13, no. 1
      why: Chapter VII has five sections and no section 13. The sentence says that the groups Aut$_0(\mathfrak{g})$ and Aut$_e(\mathfrak{g})$ can be distinct, and the place that shows it is no. 1 of section 13 of this chapter, on the algebras of type $A_l$, which computes Aut$_0(\mathfrak{g}) =\varphi (\mathbf{G}\mathbf{L}(l+ 1, k))$, identifies the quotient Aut$_0(\mathfrak{g})/$Aut$_e(\mathfrak{g})$ with $\mathbf{P}\mathbf{G}\mathbf{L}(l+ 1, k)/\mathbf{P}\mathbf{S}\mathbf{L}(l+ 1, k)$, and over the reals finds it isomorphic to $\mathbf{Z}/2\mathbf{Z}$ when $l+1$ is even. Chapter VII names neither group anywhere.
content_sha256: ad88b1b3239bfb3964472405b46e2701b09f0cd7980ced7a476855f6837c5c42
translated_from: content/en/lie/VIII/05_s5_automorphisms_of_a_semi_simple_lie.md
source_content_sha256: 80823ac5024f35186150a7d683b4b02c82a9670ba20df80f2f6ba46b412253ae
translation_model: gpt-5.4
translation_run: translate-vi-e27281d2
glossary_version: 34
glossary_terms_sha256: f1ed006cb5659c0f470b3fae277865b316e297ad8b3798beea2f70c336e82f86
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 5. CÁC TỰ ĐẲNG CẤU CỦA MỘT ĐẠI SỐ LIE NỬA ĐƠN

Trong mục này, $\mathfrak{g}$ ký hiệu một đại số Lie nửa đơn.

### 1. CÁC TỰ ĐẲNG CẤU CỦA MỘT ĐẠI SỐ LIE NỬA ĐƠN CÓ KHUNG

Nhắc lại (Chương VII, §3, no. 1) rằng Aut($\mathfrak{g}$) ký hiệu nhóm các tự đẳng cấu của $\mathfrak{g}$. Nếu $\mathfrak{h}$ là một đại số con Cartan của $\mathfrak{g}$, ta ký hiệu bởi Aut($\mathfrak{g},\mathfrak{h}$) nhóm các tự đẳng cấu của $\mathfrak{g}$ làm cho $\mathfrak{h}$ ổn định. Giả sử rằng $\mathfrak{h}$ là tách, và gọi R là hệ nghiệm của $(\mathfrak{g},\mathfrak{h})$. Nếu $s\in$ Aut($\mathfrak{g},\mathfrak{h}$), ánh xạ phản biến của $s|\mathfrak{h}$ là một phần tử của A(R) (nhóm các tự đẳng cấu của R), mà trong mục này chúng tôi sẽ ký hiệu bởi $\varepsilon (s)$. Do đó

$\varepsilon :$ Aut($\mathfrak{g},\mathfrak{h}$)$\rightarrow A(R)$

là một đồng cấu nhóm.

Với mọi hệ nghiệm R và mọi cơ sở B của R, ta ký hiệu bởi Aut(R$,B$) nhóm các tự đẳng cấu của R làm cho B ổn định. Nhắc lại rằng (Chương VI, §1, no. 5, Mệnh đề 16 và §4, no. 2, Hệ quả của Mệnh đề 1) A(R) là tích nửa trực tiếp của Aut(R$,B$) và W(R), và $A(R)/W(R)$ đẳng cấu một cách chính tắc với nhóm các tự đẳng cấu của đồ thị Dynkin của R.

#### Mệnh đề 1 {#lie-viii-s5-prop-1 .statement tag=011N}

Cho $(\mathfrak{g},\mathfrak{h},B,(X_{\alpha})_{\alpha\in B})$ là một đại số Lie nửa đơn có khung, và R là hệ nghiệm của $(\mathfrak{g},\mathfrak{h})$. Gọi G là tập hợp các $s\in$ Aut($\mathfrak{g},\mathfrak{h}$) làm cho B ổn định, và sao cho $s(X_{\alpha}) =X_{\varepsilon(s)\alpha}$ với mọi $\alpha \in B ($nói cách khác, tập hợp các tự đẳng cấu của $(\mathfrak{g},\mathfrak{h},B,(X_{\alpha})_{\alpha\in B}))$. Khi đó hạn chế của $\varepsilon$ lên G là một đẳng cấu từ G lên Aut(R$,B$).

Nếu $s\in G$, hiển nhiên là $\varepsilon (s)\in$ Aut(R$,B$). Mặt khác, ánh xạ

$\varepsilon |G : G\rightarrow$ Aut(R$,B$)

là song ánh theo Định lý 2 của §4, no. 4.

### 2. TỰ ĐẲNG CẤU CỦA MỘT ĐẠI SỐ LIE NỬA ĐƠN TÁCH

Cho E là một nhóm giao hoán, và $A =\bigoplus_{\gamma\in E}A^{\gamma}$ là một đại số phân bậc theo E. Với mọi đồng cấu $\varphi$ từ nhóm E vào nhóm nhân $k^*$, gọi $f(\varphi )$ là ánh xạ $k$-tuyến tính từ A vào A mà hạn chế của nó trên mỗi $A^{\gamma}$ là phép vị tự có tỷ số $\varphi (\gamma )$; hiển nhiên $f(\varphi )$ là một tự đẳng cấu của đại số phân bậc A, và $f$ là một đồng cấu từ nhóm Hom(E$, k^*$) vào nhóm các tự đẳng cấu của đại số phân bậc A.

Cho $\mathfrak{h}$ là một đại số con Cartan tách của $\mathfrak{g}$, và R là hệ nghiệm của $(\mathfrak{g},\mathfrak{h})$. Nhắc lại rằng P(R) (resp. Q(R)) ký hiệu nhóm các trọng số (resp. các trọng số căn) của R. Đặt

$T_P=$ Hom(P(R)$, k^*$)$T_Q=$ Hom(Q(R)$, k^*$).

Ta có thể xem $\mathfrak{g}=\mathfrak{g}^0+\sum_{\alpha\in R}\mathfrak{g}^{\alpha}$ như một đại số phân bậc theo Q(R). Các nhận xét trên xác định một đồng cấu chính tắc từ $T_Q$ vào Aut($\mathfrak{g},\mathfrak{h}$), sẽ được ký hiệu là $f$ trong đoạn này. Mặt khác, đơn ánh chính tắc từ Q(R) vào P(R) xác định một đồng cấu từ $T_P$ vào $T_Q$, sẽ được ký hiệu là $q:$

$T_P\longrightarrow^qT_Q\longrightarrow^f$ Aut($\mathfrak{g},\mathfrak{h}$).

Nếu $s\in$ Aut($\mathfrak{g},\mathfrak{h}$), gọi $s^*$ là hạn chế của $^t(s|\mathfrak{h})^{-1}$ trên Q(R). Khi đó, với mọi $\varphi \in T_Q$,

$$
f(\varphi \circ s^*) =s^{-1}\circ f(\varphi )\circ s \tag{1}
$$

Thật vậy, cho $\gamma \in Q(R)$ và $x\in \mathfrak{g}^{\gamma}$; khi đó $sx\in \mathfrak{g}^{s^*\gamma}$ và

$$
f(\varphi \circ s^*)x= (\varphi \circ s^*)(\gamma ).x=s^{-1}(\varphi (s^*\gamma )sx) = (s^{-1}\circ f(\varphi )\circ s)(x)
$$

#### Mệnh đề 2 {#lie-viii-s5-prop-2 .statement tag=011O}

Dãy các đồng cấu

1 $\longrightarrow T_Q\longrightarrow^f$ Aut($\mathfrak{g},\mathfrak{h}$)$\longrightarrow^{\varepsilon}$ A(R) $\longrightarrow$ 1

là khớp.

a) Cho $\varphi \in$ Ker $f$. Khi đó $\varphi (\alpha ) = 1$ với mọi $\alpha \in R$. Vì R sinh nhóm $Q(R),\varphi$ là phần tử đơn vị của $T_Q$.

b) Cho $\varphi \in T_Q$. Hạn chế của $f(\varphi )$ trên $\mathfrak{h}=\mathfrak{g}^0$ là đồng nhất, do đó

Im $f\subset$ Ker$\varepsilon$.

c) Cho $s\in$ Ker$\varepsilon$. Khi đó $s|\mathfrak{h}=$ Id$_{\mathfrak{h}}$. Với mọi $\alpha \in R$, ta có $s(\mathfrak{g}^{\alpha}) =\mathfrak{g}^{\alpha}$, và tồn tại một $t_{\alpha}\in k^*$ sao cho $sx=t_{\alpha}x$ với mọi $x\in \mathfrak{g}^{\alpha}$. Viết điều kiện để $s\in$ Aut($\mathfrak{g}$), ta thu được các hệ thức

$t_{\alpha}t_{-\alpha}= 1$ với mọi $\alpha \in R$

$t_{\alpha}t_{\beta}=t_{\alpha+\beta}$ khi $\alpha , \beta , \alpha +\beta \in R$.

Trong các điều kiện này, tồn tại $\varphi \in T_Q$ sao cho $\varphi (\alpha ) =t_{\alpha}$ với mọi $\alpha \in R$ (Chương VI, §1, no. 6, Hệ quả 2 của Mệnh đề 19). Khi đó $s=f(\varphi )$. Do đó, Ker $\varepsilon \subset$ Im $f$.

d) Ảnh của Aut($\mathfrak{g},\mathfrak{h}$) qua $\varepsilon$ chứa W(R) theo §2, no. 2, Hệ quả của Định lý 2, và chứa Aut(R$,B$) theo Mệnh đề 1. Do đó ảnh này bằng A(R).

#### Hệ quả 1 {#lie-viii-s5-prop-2-cor-1 .statement tag=011P}

Cho $(B,(X_{\alpha})_{\alpha\in B})$ là một cơ sở của $(\mathfrak{g},\mathfrak{h})$. Gọi G là tập hợp các $s\in$ Aut($\mathfrak{g},\mathfrak{h}$) bảo toàn cơ sở đó. Khi đó Aut($\mathfrak{g},\mathfrak{h}$) là tích nửa trực tiếp của G và $\varepsilon^{-1}(W(R))$.

Thật vậy, $G\cap \varepsilon^{-1}(W(R)) =\{1\}$ theo Mệnh đề 1, và

Aut($\mathfrak{g},\mathfrak{h}$) $= G.\varepsilon^{-1}(W(R))$

vì $\varepsilon$ là toàn ánh (Mệnh đề 2).

#### Hệ quả 2 {#lie-viii-s5-prop-2-cor-2 .statement tag=011Q}

Nhóm $\varepsilon^{-1}(W(R))$ tác động đơn bắc cầu trên tập hợp các cơ sở của $(\mathfrak{g},\mathfrak{h})$.

Thật vậy, Aut($\mathfrak{g},\mathfrak{h}$) tác động bắc cầu trên tập hợp các cơ sở của $(\mathfrak{g},\mathfrak{h})$ theo §4, no. 4, Định lý 2. Hệ quả 2 bây giờ suy ra từ Hệ quả 1.

#### Hệ quả 3 {#lie-viii-s5-prop-2-cor-3 .statement tag=011R}

Cho B là một cơ sở của R. Nhóm Ker $\varepsilon =f(T_Q)$ tác động đơn bắc cầu trên tập hợp các khung của $(\mathfrak{g},\mathfrak{h})$ có dạng $(B,(X_{\alpha})_{\alpha\in B})$.

Điều này suy ra ngay lập tức từ Mệnh đề 2.

Cho $\alpha \in R,X_{\alpha}\in \mathfrak{g}^{\alpha},X_{-\alpha}\in \mathfrak{g}^{-\alpha}$ sao cho $[X_{\alpha}, X_{-\alpha}] =-H_{\alpha}$. Ta đã thấy (§2, no. 2, Định lý 2) rằng, với mọi $t\in k^*$, hạn chế của tự đẳng cấu sơ cấp

$$
\theta_{\alpha}(t) =e^{adtX_{\alpha}}e^{adt^{-1}X_{-\alpha}}e^{adtX_{\alpha}}
$$

vào $\mathfrak{h}$ là chuyển vị của $s_{\alpha}$; do đó $\varepsilon (\theta_{\alpha}(t)) =s_{\alpha}$ và hệ quả là $\theta_{\alpha}(t)\theta_{\alpha}(-1)\in$ Ker $\varepsilon$.

#### Bổ đề 1 {#lie-viii-s5-lem-1 .statement tag=011S}

Cho $\alpha \in R$ và $t\in k^*$. Gọi $\varphi$ là đồng cấu $\lambda  \rightarrow t^{\lambda(H_{\alpha})}$ từ Q(R) vào $k^*$. Khi đó $f(\varphi ) =\theta_{\alpha}(t)\theta_{\alpha}(-1)$.

Cho $\rho$ là biểu diễn của $\mathfrak{s}\mathfrak{l}(2, k)$ trên $\mathfrak{g}$ liên kết với $X_{\alpha}$. Cho $\pi$ là biểu diễn của $\mathbf{S}\mathbf{L}(2, k)$ tương thích với $\rho$. Đặt các ký hiệu $\theta (t), h(t)$ của §1, no. 5. Vì $\rho (H) =$ ad $H_{\alpha}$, các phần tử của $\mathfrak{g}^{\lambda}$ có trọng số $\lambda (H_{\alpha})$ đối với $\rho$. Theo §2, số $2,\theta_{\alpha}(t)\theta_{\alpha}(-1) =\pi (\theta (t)\theta (-1)) =\pi (h(t))$. Do đó hạn chế của $\theta_{\alpha}(t)\theta_{\alpha}(-1)$ lên $\mathfrak{g}^{\lambda}$ là phép vị tự có tỷ số $t^{\lambda(H_{\alpha})}($§1, no. 5, Mệnh đề 6), suy ra bổ đề.

#### Mệnh đề 3 {#lie-viii-s5-prop-3 .statement tag=011T}

Ảnh của đồng cấu hợp thành

$T_P\longrightarrow^qT_Q\longrightarrow^f$ Aut($\mathfrak{g},\mathfrak{h}$)

được chứa trong Aut$_e(\mathfrak{g})$.

Cho B là một cơ sở của R. Khi đó $(H_{\alpha})_{\alpha\in B}$ là một cơ sở của $R^{\vee}$, và cơ sở đối ngẫu của $(H_{\alpha})_{\alpha\in B}$ trong $\mathfrak{h}^*$ là một cơ sở của nhóm P(R). Do đó nhóm $T_P$ được sinh bởi các đồng cấu $\lambda  \rightarrow t^{\lambda(H_{\alpha})}(t\in k^*, \alpha \in B)$. Nếu $\varphi$ là hạn chế của một đồng cấu như vậy lên Q(R), thì Bổ đề 1 chứng minh rằng $f(\varphi )\in$ Aut$_e(\mathfrak{g})$, do đó suy ra mệnh đề.

Cho $\overline{k}$ là một bao đóng đại số của $k$. Ánh xạ liên kết với mỗi tự đẳng cấu $s$ của $\mathfrak{g}$ tự đẳng cấu $s\otimes 1$ của $\mathfrak{g}\otimes_k\overline{k}$ là một đơn cấu từ Aut($\mathfrak{g}$) vào Aut($\mathfrak{g}\otimes_k\overline{k}$). Ta ký hiệu bởi Aut$_0(\mathfrak{g})$ nhóm con chuẩn tắc của Aut($\mathfrak{g}$) là ảnh ngược của Aut$_e(\mathfrak{g}\otimes_k\overline{k})$ qua đồng cấu này; đó là tập hợp các tự đẳng cấu của $\mathfrak{g}$ trở thành sơ cấp khi mở rộng trường cơ sở từ $k$ lên $\overline{k}$. Hiển nhiên Aut$_e(\mathfrak{g})$ độc lập với lựa chọn $\overline{k}$, và Aut$_e(\mathfrak{g})\subset$ Aut$_0(\mathfrak{g})$. Các nhóm Aut$_0(\mathfrak{g})$ và Aut$_e(\mathfrak{g})$ có thể phân biệt (Chương VII, §13, no. 1). Nếu $\mathfrak{h}$ là một đại số con Cartan của $\mathfrak{g}$, đặt

Aut$_e(\mathfrak{g},\mathfrak{h}) =$ Aut$_e(\mathfrak{g})\cap$ Aut($\mathfrak{g},\mathfrak{h}$), Aut$_0(\mathfrak{g},\mathfrak{h}) =$ Aut$_0(\mathfrak{g})\cap$ Aut($\mathfrak{g},\mathfrak{h}$).

#### Bổ đề 2 {#lie-viii-s5-lem-2 .statement tag=011U}

Cho $\mathfrak{h}$ là một đại số con Cartan tách của $\mathfrak{g}$, và $s\in$ Aut$_0(\mathfrak{g},\mathfrak{h})$. Giả sử rằng hạn chế của $s$ lên $\sum_{\alpha\in R}\mathfrak{g}^{\alpha}$ không có 1 là một trị riêng.

Khi đó $\varepsilon (s) = 1$.

Bằng cách mở rộng $k$, ta quy về trường hợp $s\in$ Aut$_e(\mathfrak{g},\mathfrak{h})$. Chiều của không gian lũy linh của $s-1$ ít nhất bằng dim $\mathfrak{h}$ (Chương VII, §4, no. 4, Mệnh đề 9). Do đó, $(s-1)|\mathfrak{h}$ là lũy linh. Vì $s|\mathfrak{h}\in A(R^{\vee}),s|\mathfrak{h}$ có cấp hữu hạn, nên nửa đơn (Chương V, Phụ lục, Mệnh đề 2). Do đó, $(s-1)|\mathfrak{h}= 0$, điều này chứng tỏ rằng $\varepsilon (s) = 1$.

#### Bổ đề 3 {#lie-viii-s5-lem-3 .statement tag=011V}

(i) Cho $m= (P(R) : Q(R))$. Nếu $\varphi$ là lũy thừa bậc $m$ của một phần tử của $T_Q$, thì $\varphi \in q(T_P)$.

(ii) Nếu $k$ đóng đại số, $q(T_P) = T_Q$.

Tồn tại một cơ sở $(\lambda_1, . . . , \lambda_l)$ của P(R) và các số nguyên $n_1\geq 1, . . . , n_l\geq 1$ sao cho $(n_1\lambda_1, . . . , n_l\lambda_l)$ là một cơ sở của Q(R). Ta có $m=n_1. . . n_l$. Lấy $\psi \in T_Q$ và đặt $\psi (n_1\lambda_1) =t_1, . . . , \psi (n_l\lambda_l) =t_l$. Với $i= 1, . . . , l$, đặt $m_i=$ $\prod_{j\not=i}n_j$. Cho $\chi$ là phần tử của $T_P$ sao cho $\chi (\lambda_1) =t^{m_1}_1, . . . , \chi (\lambda_l) =t^{m_l}_l$. Khi đó

$$
\chi (n_i\lambda_i) =t^{m_in_i}_i=t^m_i= (\psi^m)(n_i\lambda_i)
$$

nên $\chi |Q(R) =\psi^m$. Điều này chứng minh (i). Nếu $k$ đóng đại số, mọi phần tử của $k^*$ đều là lũy thừa bậc $m$ của một phần tử của $k^*$, nên mọi phần tử của $T_Q$ đều là lũy thừa bậc $m$ của một phần tử của $T_Q$; do đó (ii) suy ra từ (i).

#### Mệnh đề 4 {#lie-viii-s5-prop-4 .statement tag=011W}

Ta có $f(T_Q)\subset$Aut$_0(\mathfrak{g},\mathfrak{h})$ và $\varepsilon^{-1}(W(R)) =$ Aut$_0(\mathfrak{g},\mathfrak{h})$.

a) Cho $\varphi \in T_Q$ và cho $\overline{k}$ là một bao đóng đại số của $k$. Theo Bổ đề $3,\varphi$ kéo dài thành một phần tử của Hom(P(R)$, k^*$). Theo Mệnh đề 3,

$f(\varphi )\otimes 1\in$ Aut$_e(\mathfrak{g}\otimes_k\overline{k},\mathfrak{h}\otimes_k\overline{k})$.

Do đó $f(\varphi )\in$ Aut$_0(\mathfrak{g},\mathfrak{h})$, và Ker $\varepsilon \subset$ Aut$_0(\mathfrak{g},\mathfrak{h})$.

b) Ảnh của Aut$_e(\mathfrak{g},\mathfrak{h})$ dưới $\varepsilon$ chứa W(R) (§2, no. 2, Hệ quả của Định lý 2). Theo a), ta thấy rằng $\varepsilon^{-1}(W(R))\subset$ Aut$_0(\mathfrak{g},\mathfrak{h})$.

c) Còn phải chứng minh rằng Aut$_0(\mathfrak{g},\mathfrak{h})\subset \varepsilon^{-1}(W(R))$. Theo b), chỉ cần chứng minh rằng $\varepsilon$(Aut$_0(\mathfrak{g},\mathfrak{h})$)$\cap$ Aut(R$,B$), trong đó B chỉ một cơ sở của R, rút gọn thành $\{1\}$.

Cho $s\in$ Aut$_0(\mathfrak{g},\mathfrak{h})$ sao cho $\varepsilon (s)\in$ Aut(R$,B$). Nhóm con của A(R) được sinh bởi $\varepsilon (s)$ có một số hữu hạn quỹ đạo trên R. Cho U là một quỹ đạo như vậy, có lực lượng $r$, và $\mathfrak{g}^U=\sum_{\beta\in U}\mathfrak{g}^{\beta}$. Lấy $\beta_1\in U$, và đặt $\beta_i=\varepsilon (s)^{i-1}\beta_1$ với

$1\leq i\leq r$, sao cho $U =\{\beta_1, . . . , \beta_r\}$. Gọi $X_{\beta_1}$ là một phần tử khác không của $\mathfrak{g}^{\beta_1}$, và đặt $X_{\beta_i}=s^{i-1}X_{\beta_1}$ với $1\leq i\leq r$. Tồn tại $c_U\in k^*$ sao cho $s^rX_{\beta_1}=$ $c_UX_{\beta_1}$, do đó $s^rX_{\beta_i}=c_UX_{\beta_i}$ với mọi $i$, và do đó $s^r|\mathfrak{g}^U=c_U.1$. Gọi $\varphi \in T_Q$, và $s'=s\circ f(\varphi )$, theo a) thì đó là một phần tử của Aut$_0(\mathfrak{g},\mathfrak{h})$. Ta có ${s'}^r|\mathfrak{g}^U=c'_U.1$, trong đó

$$
c'_U=c_U\prod_{i=1}^r\varphi (\beta_i) =c_U\varphi (\sum_{i=1}^r\beta_i)
$$

Đặt $B =\{\alpha_1, . . . , \alpha_l\}$ và $\sum_{i=1}^r\beta_i=\sum_{j=1}^lm^U_j\alpha_j$. Vì $\varepsilon (s)\in$ Aut(R$,B$), các

$m^U_j$ là những số nguyên cùng dấu và không phải tất cả đều bằng không. Ta có

$$
c'_U=c_U\prod_{j=1}^l\varphi (\alpha_j)^{m^U_j}
$$

Bây giờ có thể chọn $\varphi$ sao cho $c'_U\not= 1$ với mọi quỹ đạo U; thật vậy, điều này quy về việc chọn các phần tử $\varphi (\alpha_1) =t_1, . . . , \varphi (\alpha_l) =t_l$ của $k^*$ không bị triệt tiêu bởi một số hữu hạn đa thức theo $t_1, . . . , t_l$, không đồng nhất bằng không. Với một lựa chọn như vậy của $\varphi ,\varepsilon (s') = 1$ theo Bổ đề 2, nên

$$
\varepsilon(s)=\varepsilon(s')\varepsilon(f(\varphi))^{-1}=1.
$$

#### Hệ quả {#lie-viii-s5-n2-cor-1 .statement tag=01J0}

— Cho $B$ là một cơ sở của $R$. Nhóm $\operatorname{Aut}(\mathfrak g,\mathfrak h)$ đẳng cấu với tích nửa trực tiếp của các nhóm $\operatorname{Aut}(R,B)$ và $\operatorname{Aut}_0(\mathfrak g,\mathfrak h)$.

Điều này suy ra từ Mệnh đề 1, Hệ quả 1 của Mệnh đề 2, và Mệnh đề 4.

#### Nhận xét {#lie-viii-s5-n2-rem-1 .statement tag=011X}

Cho $\varepsilon',\varepsilon''$ là các hạn chế của $\varepsilon$ lên $\operatorname{Aut}_0(\mathfrak g,\mathfrak h)$, $\operatorname{Aut}_e(\mathfrak g,\mathfrak h)$. Cho $f'$ là đồng cấu từ $T_P$ đến $\operatorname{Aut}_e(\mathfrak g,\mathfrak h)$ được cảm sinh bởi $f$ qua đơn ánh chính tắc từ $Q(R)$ vào $P(R)$. Trong phần trước chúng ta đã thiết lập biểu đồ giao hoán sau:
$$
\begin{array}{ccccccccc}
1&\longrightarrow&T_Q&\xrightarrow{\ f\ }&\operatorname{Aut}(\mathfrak g,\mathfrak h)&\xrightarrow{\ \varepsilon\ }&A(\mathbf R)&\longrightarrow&1\\
&&\uparrow&&\uparrow&&\uparrow&&\\
1&\longrightarrow&T_Q&\xrightarrow{\ f\ }&\operatorname{Aut}_0(\mathfrak g,\mathfrak h)&\xrightarrow{\ \varepsilon'\ }&W(\mathbf R)&\longrightarrow&1\\
&&\uparrow^{q}&&\uparrow&&\uparrow&&\\
&&T_P&\xrightarrow{\ f'\ }&\operatorname{Aut}_e(\mathfrak g,\mathfrak h)&\xrightarrow{\ \varepsilon''\ }&W(\mathbf R)&\longrightarrow&1
\end{array}
$$
trong đó các mũi tên thẳng đứng khác $q$ biểu thị các đơn ánh chính tắc. Ta đã thấy (Mệnh đề 2 và 4) rằng hai hàng đầu là khớp. Trong hàng thứ ba, đồng cấu $\varepsilon''$ là toàn ánh (§2, no. 2, Hệ quả của Định lý 2); có thể chứng minh được rằng hạt nhân của nó là $f'(T_P)$ (§7, Bài tập 26 d)).

### 3. CÁC TỰ ĐỒNG CẤU CỦA MỘT ĐẠI SỐ LIE NỬA ĐƠN PHÂN RÃ ĐƯỢC

#### Mệnh đề 5 {#lie-viii-s5-prop-5 .statement tag=01J1}

— Giả sử rằng $\mathfrak g$ là tách được. Nhóm $\operatorname{Aut}_0(\mathfrak g)$ tác động đơn bắc cầu trên tập hợp các khung của $\mathfrak g$.

Cho $e_1=(\mathfrak g,\mathfrak h_1,B_1,(X^1_\alpha)_{\alpha\in B_1})$, $e_2=(\mathfrak g,\mathfrak h_2,B_2,(X^2_\alpha)_{\alpha\in B_2})$ là hai khung của $\mathfrak g$. Tồn tại ít nhất một phần tử của $\operatorname{Aut}_0(\mathfrak g)$ biến $e_1$ thành $e_2$ (Mệnh đề 1 và Mệnh đề 4). Cho $\overline{k}$ là một bao đóng đại số của $k$. Tồn tại một phần tử của $\operatorname{Aut}_e(\mathfrak g\otimes_k\overline{k})$ biến $\mathfrak h_1\otimes_k\overline{k}$ thành $\mathfrak h_2\otimes_k\overline{k}$ (Chương VII, §3, no. 2, Định lý 1). Do đó, theo Mệnh đề 4 và Hệ quả 2 của Mệnh đề 2, tồn tại một phần tử $\varphi$ của $\operatorname{Aut}_e(\mathfrak g\otimes_k\overline{k})$ biến khung $(\mathfrak g\otimes_k\overline{k},\mathfrak h_1\otimes_k\overline{k},B_1,(X^1_\alpha)_{\alpha\in B_1})$ của $\mathfrak g\otimes_k\overline{k}$ thành khung $(\mathfrak g\otimes_k\overline{k},\mathfrak h_2\otimes_k\overline{k},B_2,(X^2_\alpha)_{\alpha\in B_2})$. Vì $\mathfrak h_1$ và các $X^1_\alpha$ (tương ứng $\mathfrak h_2$ và các $X^2_\alpha$) sinh ra $\mathfrak g_1$ (tương ứng $\mathfrak g_2$), ta có $\varphi(\mathfrak g_1)=\mathfrak g_2$, nên $\varphi$ có dạng $\psi\otimes 1$ với $\psi\in\operatorname{Aut}_0(\mathfrak g)$, và $\psi$ biến $e_1$ thành $e_2$.

#### Hệ quả 1 {#lie-viii-s5-prop-5-cor-1 .statement tag=01J2}

— Cho $(\mathfrak g,\mathfrak h,B,(X_\alpha)_{\alpha\in B})$ là một sự định khung của $\mathfrak g$, và $G$ là nhóm (đẳng cấu với $\operatorname{Aut}(R,B)$) các tự đẳng cấu của $\mathfrak g$ để sự định khung này bất biến. Khi đó $\operatorname{Aut}(\mathfrak g)$ là tích nửa trực tiếp của $G$ và $\operatorname{Aut}_0(\mathfrak g)$.

Thật vậy, mọi phần tử của $\operatorname{Aut}(\mathfrak g)$ biến $(\mathfrak g,\mathfrak h,B,(X_\alpha)_{\alpha\in B})$ thành một sự định khung của $\mathfrak g$. Theo Mệnh đề 5, mỗi lớp kề của $\operatorname{Aut}(\mathfrak g)$ theo môđun $\operatorname{Aut}_0(\mathfrak g)$ cắt $G$ đúng tại một điểm.

Q.E.D.

Từ Hệ quả 1 suy ra rằng nhóm Aut($\mathfrak{g}$)$/$Aut$_0(\mathfrak{g})$ có thể được đồng nhất với Aut(R$,B$), và đẳng cấu với nhóm các tự đẳng cấu của đồ thị Dynkin của R.

#### Hệ quả 2 {#lie-viii-s5-prop-5-cor-2 .statement tag=01J3}

Aut($\mathfrak{g}$) $=$ Aut$_0(\mathfrak{g})$ khi $\mathfrak{g}$ là một đại số Lie đơn phân rã được thuộc kiểu $A_1,B_n(n\geq 2)$, $C_n(n\geq 2)$, $E_7,E_8,F_4,G_2$. Thương Aut($\mathfrak{g}$)$/$Aut$_0(\mathfrak{g})$ có cấp 2 khi $\mathfrak{g}$ thuộc kiểu $A_n(n\geq 2)$, $D_n(n\geq 5)$, $E_6$; nó đẳng cấu với $\mathfrak{S}_3$ khi $\mathfrak{g}$ thuộc kiểu $D_4$.

Điều này suy ra từ Hệ quả 1 và Chương VI, Các bảng I đến IX.

#### Nhận xét 1 {#lie-viii-s5-n3-rem-1 .statement tag=011Z}

Cho $e_1= (\mathfrak{g},\mathfrak{h}_1,B_1,(X_{\alpha}^1)_{\alpha\in B_1}),e_2= (\mathfrak{g},\mathfrak{h}_2,B_2,(X_{\alpha}^2)_{\alpha\in B_2})$, $e'_2= (\mathfrak{g},\mathfrak{h}_2,B_2,(Y_{\alpha}^2)_{\alpha\in B_2})$ là các khung của $\mathfrak{g}$, và $s$ (resp. $s'$) là một phần tử của Aut$_0(\mathfrak{g})$ biến đổi $e_1$ thành $e_2$ (resp. $e'_2$). Khi đó $s|\mathfrak{h}_1=s'|\mathfrak{h}_1$. Thật vậy, $s^{'-1}s\in$ Aut$_0(\mathfrak{g},\mathfrak{h}_1)$ và $s^{'-1}s(B_1) = B_1$, nên $\varepsilon (s^{'-1}s) = 1$.

#### Nhận xét 2 {#lie-viii-s5-n3-rem-2 .statement tag=0120}

Cho X là tập hợp các cặp $(\mathfrak{h},B)$ trong đó $\mathfrak{h}$ là một đại số con Cartan tách của $\mathfrak{g}$ và B là một cơ sở của hệ nghiệm của $(\mathfrak{g},\mathfrak{h})$. Nếu $x= (\mathfrak{h},B)$ và $x'= (\mathfrak{h}',B')$ là hai phần tử của X, thì tồn tại $s\in$ Aut$_0(\mathfrak{g})$ biến đổi $x$ thành $x'$ (Mệnh đề 5), và hạn chế $s_{x',x}$ của $s$ trên $\mathfrak{h}$ không phụ thuộc vào lựa chọn $s$ (Nhận xét 1). Đặc biệt, $s_{x'',x'}\circ s_{x',x}=s_{x'',x}$ nếu $x, x', x''\in X$, và $s_{x,x}= 1$. Tập hợp các họ $(h_x)_{x\in X}$ thỏa mãn các điều kiện

$a)h_x\in \mathfrak{h}$ nếu $x= (\mathfrak{h},B)$

$b)s_{x',x}(h_x) =h_{x'}$ nếu $x, x'\in X$

là, một cách tự nhiên, một không gian vectơ $\mathfrak{h}(\mathfrak{g})$ mà đôi khi chúng tôi gọi là đại số con Cartan chính tắc của $\mathfrak{g}$. Với $x= (\mathfrak{h},B)$ và $x'= (\mathfrak{h}',B'),s_{x',x}$ biến B thành $B'$, và do đó biến hệ nghiệm của $(\mathfrak{g},\mathfrak{h})$ thành hệ nghiệm của $(\mathfrak{g},\mathfrak{h}')$; suy ra đối ngẫu $\mathfrak{h}(\mathfrak{g})^*$ của $\mathfrak{h}(\mathfrak{g})$ được trang bị một cách tự nhiên một hệ nghiệm $R(\mathfrak{g})$ và một cơ sở $B(\mathfrak{g})$ của $R(\mathfrak{g})$. Đôi khi chúng tôi nói rằng $R(\mathfrak{g})$ là hệ nghiệm chính tắc của $\mathfrak{g}$ và $B(\mathfrak{g})$ là cơ sở chính tắc của nó. Nhóm Aut($\mathfrak{g}$) tác động lên $\mathfrak{h}(\mathfrak{g})$ và để $R(\mathfrak{g})$ cùng $B(\mathfrak{g})$ ổn định; các phần tử của Aut($\mathfrak{g}$) tác động tầm thường trên $\mathfrak{h}(\mathfrak{g})$ là các phần tử của Aut$_0(\mathfrak{g})$.

#### Mệnh đề 6 {#lie-viii-s5-prop-6 .statement tag=0121}

Cho $\mathfrak{h}$ là một đại số con Cartan tách của $\mathfrak{g}$. Ta có, với các ký hiệu ở no. 1, Aut$_0(\mathfrak{g}) =$ Aut$_e(\mathfrak{g})$.Ker $\varepsilon =$ Aut$_e(\mathfrak{g}).f(T_Q)$.

Theo §3, no. 3, Hệ quả của Mệnh đề 10, Aut$_0(\mathfrak{g}) =$ Aut$_e(\mathfrak{g})$.Aut$_0(\mathfrak{g},\mathfrak{h})$. Mặt khác, $\varepsilon$(Aut$_e(\mathfrak{g},\mathfrak{h})$)$\supset W(R)$ theo §2, no. 2, Hệ quả của Định lý 2, do đó Aut$_0(\mathfrak{g},\mathfrak{h}) =$ Aut$_e(\mathfrak{g},\mathfrak{h})$.Ker$\varepsilon$.

#### Nhận xét 3 {#lie-viii-s5-n3-rem-3 .statement tag=0122}

Mệnh đề 6 cho thấy rằng đồng cấu chính tắc

$\iota : T_Q/$Im(T$_P$)$\rightarrow$ Aut$_0(\mathfrak{g})/$Aut$_e(\mathfrak{g})$,

được cảm sinh bởi biểu đồ ở no. 2, là toàn ánh. Đặc biệt, Aut$_e(\mathfrak{g})$ chứa nhóm dẫn xuất của Aut$_0(\mathfrak{g})$; ta sẽ thấy (§11, no. 2, Mệnh đề 3) rằng thực ra chúng bằng nhau. Hơn nữa, có thể chứng minh rằng $\iota$ là đơn ánh, nói cách khác rằng $f(T_Q)\cap$ Aut$_e(\mathfrak{g}) =f'(T_P)$,

(xem §7, Bài tập $26d$)$)$.

#### Mệnh đề 7 {#lie-viii-s5-prop-7 .statement tag=0123}

Cho $\mathfrak{g}$ là một đại số Lie nửa đơn tách được, $\mathfrak{b}$ là một đại số con Borel của $\mathfrak{g}$, và $\mathfrak{p}_1$ và $\mathfrak{p}_2$ là hai đại số con parabolic phân biệt của $\mathfrak{g}$ chứa $\mathfrak{b}$. Khi đó $\mathfrak{p}_1$ và $\mathfrak{p}_2$ không liên hợp dưới Aut$_0(\mathfrak{g})$.

Ta có thể giả thiết rằng $k$ đóng đại số. Cho $s\in$ Aut$_0(\mathfrak{g})$ sao cho $s(\mathfrak{p}_1) =\mathfrak{p}_2$. Gọi $\mathfrak{h}$ là một đại số con Cartan của $\mathfrak{g}$ được chứa trong $\mathfrak{b}\cap s(\mathfrak{b}) ($§3, no. 3, Prop. 10). Vì $\mathfrak{h}$ và $s(\mathfrak{h})$ là các đại số con Cartan của $s(\mathfrak{b})$, tồn tại $u\in [\mathfrak{b},\mathfrak{b}]$ sao cho $e^{adu}(\mathfrak{h}) =s(\mathfrak{h})$ (Chap. VII, §3, no. 4, Th. 3). Thay thế $s$ bởi $e^{-adu}s$, ta được quy về trường hợp $s(\mathfrak{h}) =\mathfrak{h}$, và khi đó $s$ cảm sinh trên $\mathfrak{h}$ một phần tử $\sigma$ của nhóm Weyl W của $(\mathfrak{g},\mathfrak{h})$ (Prop. 4). Gọi C là buồng Weyl tương ứng với $\mathfrak{b}$. Khi đó $\mathfrak{p}_1$ và $\mathfrak{p}_2$ tương ứng với các mặt $F_1$ và $F_2$ của $\mathfrak{h}_{\mathbf{R}}$ được chứa trong bao đóng của C. Ta có $\sigma (F_1) = F_2$. Vì $\sigma \in W$, điều này suy ra $F_1= F_2$ (Chap. V, §3, no. 3, Th. 2) nên $\mathfrak{p}_1=\mathfrak{p}_2$.

#### Nhận xét 4 {#lie-viii-s5-n3-rem-4 .statement tag=0124}

Cho $\mathfrak{g}$ là một đại số Lie nửa đơn phân rã được, $\mathscr{P}$ tập hợp các đại số con parabolic của $\mathfrak{g}$, một tập hợp mà trên đó Aut$_0(\mathfrak{g})$ tác động. Giữ các ký hiệu của Nhận xét 2. Cho $\Sigma$ là một tập con của $B(\mathfrak{g})$. Cho $\Sigma$ tương đương với việc cho, với mỗi $x= (\mathfrak{h},B)\in X$, một tập con $\Sigma_x$ của B, sao cho $s_{x',x}$ biến $\Sigma_x$ thành $\Sigma_{x'}$ với mọi $x, x'\in X$. Gọi $\mathfrak{p}_x$ là đại số con parabolic của $\mathfrak{g}$ tương ứng với $\Sigma_x$ (§3, no. 4, Nhận xét). Quỹ đạo của $\mathfrak{p}_x$ dưới tác động của Aut$_0(\mathfrak{g})$ là tập hợp các $\mathfrak{p}_{x'}$ với $x'\in X$. Điều này xác định một ánh xạ từ $\mathfrak{P}(B(\mathfrak{g}))$ tới $\mathscr{P}/$Aut$_0(\mathfrak{g})$. Ánh xạ này là toàn ánh theo Nhận xét của §3, no. 4, và đơn ánh theo Mệnh đề 7.

### 4. TÔPÔ ZARISKI TRÊN Aut($\mathfrak{g}$)

#### Mệnh đề 8 {#lie-viii-s5-prop-8 .statement tag=0125}

Gọi V là tập hợp các nội cấu của không gian vectơ $\mathfrak{g}$. Khi đó Aut($\mathfrak{g}$) là đóng trong V đối với tôpô Zariski (Chương VII, Phụ lục I).

Gọi K là dạng Killing của $\mathfrak{g}$. Nếu $s\in$ Aut($\mathfrak{g}$),

$$
[sx, sy] = [x, y] \tag{2}
$$

$$
K(sx, sy) = K(x, y) \tag{3}
$$

với mọi $x, y\in \mathfrak{g}$. Ngược lại, giả sử $s$ là một phần tử của V thỏa mãn (2) và (3) với mọi $x, y\in \mathfrak{g}$. Khi đó Ker($s$) $= 0$, nên $s$ là song ánh và $s\in$ Aut($\mathfrak{g}$). Nhưng, với mọi $x, y\in \mathfrak{g}$, các ánh xạ $s \rightarrow [sx, sy]$ và $s \rightarrow K(sx, sy)$ từ V tới $\mathfrak{g}$ và $k$ là đa thức.

#### Mệnh đề 9 {#lie-viii-s5-prop-9 .statement tag=0126}

Cho $\mathfrak{h}$ là một đại số con Cartan tách của $\mathfrak{g}$.

(i) Nhóm $f(T_Q)$ là đóng trong Aut($\mathfrak{g}$) đối với tôpô Zariski.

(ii) Nhóm $f(q(T_P))$ là trù mật trong $f(T_Q)$ đối với tôpô Zariski.

Mệnh đề (i) suy ra từ đẳng thức $f(T_Q) =$ Aut($\mathfrak{g},\mathfrak{h}$)$\cap$Ker$\varepsilon$ (Prop. 2). Đặt $m= (P(R) : Q(R))$. Cho F là một hàm đa thức trên V; ta giả sử rằng F triệt tiêu trên lũy thừa bậc $m$ của mọi phần tử của $f(T_Q)$, và chứng minh rằng $F|f(T_Q) = 0$; theo Bổ đề 3, điều này sẽ chứng minh (ii).

Tập hợp $V'$ các phần tử của V cảm sinh đồng nhất trên $\mathfrak{h}$ và để mỗi $\mathfrak{g}^{\alpha}$ ổn định có thể được đồng nhất với $k^R$. Gọi $F'$ là hạn chế của F lên $V'=k^R$; đó là một hàm đa thức. Ta có $f(T_Q)\subset V'$. Gọi $B = (\alpha_1, . . . , \alpha_l)$ là một cơ sở của R. Với mọi $t= (t_1, . . . , t_l)\in k^{*B}$, gọi $\varphi (t)$ là đồng cấu từ Q(R) vào nhóm $k^*$ kéo dài $t$. Khi đó $F'(f(\varphi (t)))$ có thể được viết thành một tổng hữu hạn

$$
\sum_{n_1,...,n_l\in\mathbf{Z}}c_{n_1,...,n_l}t^{n_1}_1. . . t^{n_l}_l= H(t_1, . . . , t_l)
$$

Theo giả thiết,

$$
0 = H(t^m_1, . . . , t^m_l) =\sum_{n_1,...,n_l\in\mathbf{Z}}c_{n_1,...,n_l}t^{mn_1}_1. . . t^{mn_l}_l
$$

với mọi $t_1, . . . , t_l\in k^*$. Do đó các $c_{n_1,...,n_l}$ là các hệ số của một đa thức theo $l$ biến triệt tiêu trên $k^{*l}$; vì thế chúng đều bằng không.

#### Mệnh đề 10 {#lie-viii-s5-prop-10 .statement tag=0127}

Giả sử rằng $\mathfrak{g}$ là khả phân.

(i) Nhóm Aut$_e(\mathfrak{g})$ trù mật trong Aut$_0(\mathfrak{g})$ theo tôpô Zariski.

(ii) Các nhóm Aut$_e(\mathfrak{g})$ và Aut$_0(\mathfrak{g})$ là liên thông theo tôpô Zariski.

Theo Mệnh đề $3,f(q(T_P))\subset$ Aut$_e(\mathfrak{g})$. Với mọi $s\in$ Aut$_e(\mathfrak{g})$, bao đóng của $s.f(q(T_P))$ trong tôpô Zariski chứa $s.f(T_Q)$ theo Mệnh đề 9. Do đó bao đóng của Aut$_e(\mathfrak{g})$ chứa Aut$_e(\mathfrak{g}).f(T_Q) =$ Aut$_0(\mathfrak{g})$ (Mệnh đề 6). Điều này chứng minh (i).

Cho Aut$_e(\mathfrak{g}) =\Omega \cup \Omega '$ là một phân hoạch của Aut$_e(\mathfrak{g})$ được tạo bởi các tập con mở tương đối trong tôpô Zariski, với $\Omega \not=\emptyset$. Nếu $\omega \in \Omega$ và nếu $x$ là một phần tử lũy linh của $\mathfrak{g}$, ánh xạ $\tau :t \rightarrow \omega$ exp($t$ ad $x$) từ $k$ vào Aut$_e(\mathfrak{g})$ là đa thức, nên liên tục trong tôpô Zariski; do đó, $\tau (k)$ là liên thông; vì $\omega \in \tau (k)$, ta có $\tau (k)\subset \Omega$. Do đó, $\Omega$.(exp ad $kx$)$\subset \Omega$, nên $\Omega$.Aut$_e(\mathfrak{g})\subset \Omega$ và $\Omega =$ Aut$_e(\mathfrak{g})$. Điều này chứng minh rằng Aut$_e(\mathfrak{g})$ là liên thông. Theo (i) suy ra rằng Aut$_0(\mathfrak{g})$ là liên thông. Q.E.D.

Ta sẽ thấy (§8, no. 4, Hệ quả của Mệnh đề 6) rằng Aut$_0(\mathfrak{g})$ đóng trong V đối với tôpô Zariski, và rằng nó là thành phần liên thông của phần tử đơn vị của Aut($\mathfrak{g}$). Mặt khác, Aut$_e(\mathfrak{g})$ nói chung không đóng đối với tôpô Zariski.

$^*$Giả sử rằng $(\mathfrak{g},\mathfrak{h})$ là tách. Nhóm Aut$_0(\mathfrak{g})$ là nhóm $G(k)$ của các $k$-điểm của một nhóm đại số nửa đơn liên thông G có tâm tầm thường (nhóm adjoint). Nhóm $f(T_Q)$ bằng $H(k)$, trong đó H là nhóm Cartan của G có đại số Lie $\mathfrak{h}$. Ảnh ngược $\widetilde{H}$ của H trong phủ phổ quát $\widetilde{G}$ của G (theo nghĩa đại số) có $T_P$ là nhóm các $k$-điểm của nó. Ảnh của $\widetilde{G}(k)$ trong $G(k) =$ Aut$_0(\mathfrak{g})$ là nhóm Aut$_e(\mathfrak{g})._*$

### 5. TRƯỜNG HỢP NHÓM Lie

#### Mệnh đề 11 {#lie-viii-s5-prop-11 .statement tag=0128}

Giả sử rằng $k$ là $\mathbf{R},\mathbf{C}$ hoặc một trường ultrametric đầy đủ không rời rạc. Cho $\mathfrak{h}$ là một đại số con Cartan tách của $\mathfrak{g}$.

(i) Aut($\mathfrak{g},\mathfrak{h}$) là một nhóm con Lie của Aut($\mathfrak{g}$) với đại số Lie ad$\mathfrak{h}$.

(ii) $f(T_Q)$ và $(q\circ f)(T_P)$ là các nhóm con mở của Aut($\mathfrak{g},\mathfrak{h}$).

(iii) Aut$_e(\mathfrak{g})$ là một nhóm con mở của Aut($\mathfrak{g}$).

(iv) Nếu $k=\mathbf{R}$ hoặc $\mathbf{C}$, Aut$_e(\mathfrak{g})$ là thành phần liên thông của đơn vị của Aut($\mathfrak{g}$), nói cách khác là Int($\mathfrak{g}$).

Theo Chương III, §3, no. 8, Hệ quả 2 của Mệnh đề 29, và no. 10, Mệnh đề 36, Aut($\mathfrak{g},\mathfrak{h}$) là một nhóm con Lie của Aut($\mathfrak{g}$) mà đại số Lie là tập hợp các ad $x(x\in \mathfrak{g})$ sao cho (ad $x$)$\mathfrak{h}\subset \mathfrak{h}$, nói cách khác là ad$\mathfrak{h}$.

Cho $H\in \mathfrak{h}$. Tồn tại $\varepsilon  >0$ có các tính chất sau đây: với $t\in k$ và $|t|< \varepsilon$, exp($t\gamma (H)$) được xác định với mọi $\gamma \in P(R)$, và ánh xạ $\gamma  \rightarrow$ exp($t\gamma (H)$) là một đồng cấu $\sigma_t$ từ P(R) vào $k^*$. Với $|t|< \varepsilon$, exp($t$ ad H) được xác định, cảm sinh đồng nhất trên $\mathfrak{h}$ và cảm sinh trên $\mathfrak{g}^{\alpha}$ phép vị tự có tỉ số $\sigma_t(\alpha )$; do đó exp $t$ ad $H\in (q\circ f)(T_P)$. Điều này chứng tỏ, theo (i), rằng $(q\circ f)(T_P)$ chứa một lân cận của 1 trong Aut($\mathfrak{g},\mathfrak{h}$), và do đó là một nhóm con mở của Aut($\mathfrak{g},\mathfrak{h}$). A fortiori$,f(T_Q)$ là một nhóm con mở của Aut($\mathfrak{g},\mathfrak{h}$).

Với mọi $\alpha \in R$, exp ad $\mathfrak{g}^{\alpha}\subset$ Aut$_e(\mathfrak{g})$. Theo (ii), Aut$_e(\mathfrak{g})$ chứa một lân cận của 1 trong Aut($\mathfrak{g}$), điều này chứng minh (iii).

Giả sử rằng $k=\mathbf{R}$ hoặc $\mathbf{C}$. Khi đó Aut$_e(\mathfrak{g})$ được chứa trong thành phần chứa đơn vị C của Aut($\mathfrak{g}$) (Chap. VII, §3, no. 1), và là mở trong Aut($\mathfrak{g}$) theo (iii). Do đó Aut$_e(\mathfrak{g}) = C$. Cuối cùng, C = Int($\mathfrak{g}$) theo Chap. III, §9, no. 8, Prop. 30 (i).

### Bài tập {#lie-viii-s5-exercises}

Xem [các bài tập của § 5](exercises/s5/).
