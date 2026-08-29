---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: VIII
chapter_title: SPLIT SEMI-SIMPLE LIE ALGEBRAS
section: 4
section_title: Split semi-simple Lie algebra defined by a reduced root system
lang: vi
source: lie-vii-ix
book_pages: 95-106, 231-233
pdf_pages: 0103-0114, 0239-0241
extraction: native
subsections:
    - "no": 1
      title: FRAMED SEMI-SIMPLE LIE ALGEBRAS
      page: 95
      pdf_page: 103
    - "no": 2
      title: A PRELIMINARY CONSTRUCTION
      page: 96
      pdf_page: 104
    - "no": 3
      title: EXISTENCE THEOREM
      page: 100
      pdf_page: 108
    - "no": 4
      title: UNIQUENESS THEOREM
      page: 104
      pdf_page: 112
statements: 23
exercises: 7
content_sha256: 0ac6fbf3e9c5df76219acbbbb2499ad9d8f01210fd047669e0bbd6bd3651193d
translated_from: content/en/lie/VIII/04_s4_split_semi_simple_lie_algebra_defined.md
source_content_sha256: d31efd9ddbb6c9db525488b6ea28a82ed909217def1e86239e848957a5f5eb01
translation_model: gpt-5-6-mini, gpt-5-mini
translation_run: translate-vi-b0344878
glossary_version: 34
glossary_terms_sha256: 627582a4e04db93dc2a7a00679aa2fcae017e9c3897464c92331d5ed51a3b514
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 4. ĐẠI SỐ LIE NỬA ĐƠN TÁCH ĐƯỢC XÁC ĐỊNH BỞI MỘT HỆ NGHIỆM RÚT GỌN

### 1. CÁC ĐẠI SỐ LIE NỬA ĐƠN ĐƯỢC ĐÓNG KHUNG

#### Mệnh đề 1 {#lie-viii-s4-prop-1 .statement tag=010T}

Cho $(\mathfrak{g},\mathfrak{h})$ là một đại số Lie nửa đơn tách được, R là hệ nghiệm của nó, B là một cơ sở của R, và $(n(\alpha , \beta ))_{\alpha ,\beta\in B}$ là ma trận Cartan tương ứng. Với mọi $\alpha \in B$, cho $X_{\alpha}\in \mathfrak{g}^{\alpha}, X_{-\alpha}\in \mathfrak{g}^{-\alpha}$. Khi đó, với $\alpha , \beta \in B$,

$$
[H_{\alpha}, H_{\beta}] = 0 \tag{1}
$$

$$
[H_{\alpha}, X_{\beta}] =n(\beta , \alpha )X_{\beta} \tag{2}
$$

$$
[H_{\alpha}, X_{-\beta}] =-n(\beta , \alpha )X_{-\beta} \tag{3}
$$

$[X_{-\alpha}, X_{\beta}] = 0$ nếu $\alpha \not=\beta$ (4)

(ad $X_{\alpha}$)$^{1-n(\beta ,\alpha)}X_{\beta}= 0$ nếu $\alpha \not=\beta$ (5)

(ad $X_{-\alpha}$)$^{1-n(\beta ,\alpha)}X_{-\beta}= 0$ nếu $\alpha \not=\beta$. (6)

Họ $(H_{\alpha})_{\alpha\in B}$ là một cơ sở của $\mathfrak{h}$. Nếu $X_{\alpha}\not= 0$ và $X_{-\alpha}\not= 0$ với mọi $\alpha \in B$, đại số Lie $\mathfrak{g}$ được sinh bởi các $X_{\alpha}$ và các $X_{-\alpha}(\alpha \in B)$.

(Nhắc lại rằng, nếu $\alpha , \beta \in B$ và $\alpha \not=\beta ,n(\beta , \alpha )$ là một số nguyên $\leq 0$, do đó các công thức (5) và (6) có nghĩa.)

Các công thức (1), (2) và (3) là rõ ràng. Nếu $\alpha \not=\beta ,\beta -\alpha$ không phải là một nghiệm vì mọi phần tử của R là một tổ hợp tuyến tính của các phần tử của B với các hệ số nguyên tất cả cùng dấu (Chương VI, §1, no. 6, Định lý 3). Điều này chứng minh (4). Theo Chương VI, §1, no. 3, Mệnh đề 9, điều này cũng chứng minh rằng dãy $\alpha$ được xác định bởi $\beta$ là

$$
\{\beta , \beta +\alpha , . . . , \beta -n(\beta , \alpha )\alpha \}
$$

do đó $\beta +(1-n(\beta , \alpha ))\alpha  \notin R$, điều này chứng minh (5). Đẳng thức (6) được thiết lập theo cách tương tự. Họ $(H_{\alpha})_{\alpha\in B}$ là một cơ sở của $R^{\vee}$, và do đó của $\mathfrak{h}$. Nếu $X_{\alpha}\not= 0$ và $X_{-\alpha}\not= 0$ với mọi $\alpha \in B$, thì $[X_{\alpha}, X_{-\alpha}] =\lambda_{\alpha}H_{\alpha}$ với $\lambda_{\alpha}\not= 0$, do đó khẳng định cuối cùng suy ra từ §3, no. 3, Mệnh đề 9 (iii).

#### Định nghĩa 1 {#lie-viii-s4-def-1 .statement tag=010U}

Cho $(\mathfrak{g},\mathfrak{h})$ là một đại số Lie nửa đơn tách được, R là hệ nghiệm của nó. Một sự đóng khung của $(\mathfrak{g},\mathfrak{h})$ là một cặp $(B,(X_{\alpha})_{\alpha\in B})$, trong đó B là một cơ sở của R, và trong đó, với mọi $\alpha \in B,X_{\alpha}$ là một phần tử khác không của $\mathfrak{g}^{\alpha}$. Một đại số Lie nửa đơn được đóng khung là một dãy $(\mathfrak{g},\mathfrak{h},B,(X_{\alpha})_{\alpha\in B})$ trong đó $(\mathfrak{g},\mathfrak{h})$ là một đại số Lie nửa đơn tách được, và trong đó $(B,(X_{\alpha})_{\alpha\in B})$ là một sự đóng khung của $(\mathfrak{g},\mathfrak{h})$.

Một sự đóng khung của $\mathfrak{g}$ là một sự đóng khung của $(\mathfrak{g},\mathfrak{h})$, trong đó $\mathfrak{h}$ là một đại số con Cartan tách của $\mathfrak{g}$.

Cho $a_1= (\mathfrak{g}_1,\mathfrak{h}_1,B_1,(X_{\alpha}^1)_{\alpha\in B_1})$ và $a_2= (\mathfrak{g}_2,\mathfrak{h}_2,B_2,(X_{\alpha}^2)_{\alpha\in B_2})$ là các đại số Lie nửa đơn có khung. Một đẳng cấu từ $a_1$ đến $a_2$ là một đẳng cấu $\varphi$ từ $\mathfrak{g}_1$ đến $\mathfrak{g}_2$ biến $\mathfrak{h}_1$ thành $\mathfrak{h}_2, B_1$ thành $B_2$, và $X_{\alpha}^1$ thành $X_{\psi \alpha}^2$ với mọi $\alpha \in B_1$ (trong đó $\psi$ là ánh xạ đối ngẫu của $\varphi |\mathfrak{h}_1$). Trong trường hợp này, $\varphi$ được nói là biến đổi khung $(B_1,(X_{\alpha}^1)_{\alpha\in B_1})$ thành khung $(B_2,(X_{\alpha}^2)_{\alpha\in B_2})$.

Nếu $(B,(X_{\alpha})_{\alpha\in B})$ là một khung của $(\mathfrak{g},\mathfrak{h})$, thì với mọi $\alpha \in B$, tồn tại một phần tử duy nhất $X_{-\alpha}$ của $\mathfrak{g}^{-\alpha}$ sao cho $[X_{\alpha}, X_{-\alpha}] =-H_{\alpha}($§2, no. 2, Đl. 1 (iv)). Họ $(X_{\alpha})_{\alpha\in B\cup(-B)}$ được gọi là họ sinh được xác định bởi khung (xem Mđ.1). Đây cũng là họ sinh được xác định bởi khung $(-B,(X_{\alpha})_{\alpha\in -B})$. Với mọi $\alpha \in B\cup (-B)$, lấy $t_{\alpha}\in k^*$, và giả sử rằng $t_{\alpha}t_{-\alpha}= 1$ với mọi $\alpha \in B$. Khi đó $(t_{\alpha}X_{\alpha})_{\alpha\in B\cup(-B)}$ là họ sinh được xác định bởi khung $(B,(t_{\alpha}X_{\alpha})_{\alpha\in B})$.

### 2. MỘT XÂY DỰNG SƠ BỘ

Trong số này và số tiếp theo, ta ký hiệu bởi R một hệ nghiệm rút gọn trong một không gian vectơ V và bởi B một cơ sở của R. Ta ký hiệu bởi $(n(\alpha , \beta ))_{\alpha ,\beta\in B}$ ma trận Cartan tương ứng với B. Nhắc lại rằng $n(\alpha , \beta ) =\langle \alpha , \beta^{\vee}\rangle$. Ta sẽ chứng minh rằng R là hệ nghiệm của một đại số Lie nửa đơn tách, duy nhất sai khác một đẳng cấu. Phần lớn ta sẽ xét đại số Lie được xác định bởi các quan hệ trong Mđ. 1.

Phép dựng trong số này áp dụng cho mọi ma trận bình phương $(n(\alpha , \beta ))_{\alpha ,\beta\in B}$ trên $k$ có định thức khác không và sao cho $n(\alpha , \alpha ) = 2$ với mọi $\alpha \in B$ (xem Ch. VI, §1, no. 10, công thức (14)).

Gọi E là đại số kết hợp tự do của tập hợp B trên $k$. Nhắc lại rằng E là $\mathbf{N}$-phân bậc (Đại số, Ch. III, §3, no. 1, Ví dụ 3). Ta sẽ gán cho mỗi $\alpha \in B$ các tự đồng cấu $X_{-\alpha}^0, H_{\alpha}^0, X_{\alpha}^0$ của không gian vectơ E, có bậc lần lượt là $1,0,-1$. Với mọi từ $(\alpha_1, . . . , \alpha_n)$ gồm các phần tử của B, đặt

$$
X_{-\alpha}^0(\alpha_1, . . . , \alpha_n) = (\alpha , \alpha_1, . . . , \alpha_n) \tag{7}
$$

$$
H_{\alpha}^0(\alpha_1, . . . , \alpha_n) =(-\sum_{i=1}^nn(\alpha_i, \alpha ))(\alpha_1, . . . , \alpha_n) \tag{8}
$$

Mặt khác, $X_{\alpha}^0(\alpha_1, . . . , \alpha_n)$ được xác định bằng quy nạp theo $n$ sử dụng công thức

$$
X_{\alpha}^0(\alpha_1, . . . , \alpha_n) = (X_{-\alpha_1}^0X_{\alpha}^0-\delta_{\alpha ,\alpha_1}H_{\alpha}^0)(\alpha_2, . . . , \alpha_n) \tag{9}
$$

trong đó $\delta_{\alpha ,\alpha_1}$ là ký hiệu Kronecker; hiểu rằng $X_{\alpha}^0(\alpha_1, . . . , \alpha_n)$ bằng không nếu $(\alpha_1, . . . , \alpha_n)$ là từ rỗng.

#### Bổ đề 1 {#lie-viii-s4-lem-1 .statement tag=010V}

Với mọi $\alpha , \beta \in B$, ta có

$$
[X_{\alpha}^0, X_{-\alpha}^0] =-H_{\alpha}^0 \tag{10}
$$

$$
[H_{\alpha}^0, H_{\beta}^0] = 0 \tag{11}
$$

$$
[H_{\alpha}^0, X_{\beta}^0] =n(\beta , \alpha )X_{\beta}^0 \tag{12}
$$

$$
[H_{\alpha}^0, X_{-\beta}^0] =-n(\beta , \alpha )X_{-\beta}^0 \tag{13}
$$

$[X_{\alpha}^0, X_{-\beta}^0] = 0$ nếu $\alpha \not=\beta$. (14)

Thật vậy, quan hệ (9) có thể viết thành

$$
(X_{\alpha}^0X_{-\alpha_1}^0)(\alpha_2, . . . , \alpha_n) = (X_{-\alpha_1}^0X_{\alpha}^0)(\alpha_2, . . . , \alpha_n)-\delta_{\alpha ,\alpha_1}H_{\alpha}^0(\alpha_2, . . . , \alpha_n)
$$

điều này chứng minh (10) và (14). Quan hệ (11) là hiển nhiên. Tiếp theo

$$
[H_{\alpha}^0, X_{-\beta}^0](\alpha_1, . . . , \alpha_n) =H_{\alpha}^0(\beta , \alpha_1, . . . , \alpha_n)+(\sum_{i=1}^nn(\alpha_i, \alpha ))(\beta , \alpha_1, . . . , \alpha_n)
$$

$$
=-n(\beta , \alpha )(\beta , \alpha_1, . . . , \alpha_n)
$$

$$
=-n(\beta , \alpha )X_{-\beta}^0(\alpha_1, . . . , \alpha_n)
$$

suy ra (13). Cuối cùng,

$0 = [H_{\alpha}^0,[X_{\beta}^0, X_{-\gamma}^0]]$ theo $(10),(11),(14)$ (15)

$$
= [[H_{\alpha}^0, X_{\beta}^0], X_{-\gamma}^0] + [X_{\beta}^0,[H_{\alpha}^0, X_{-\gamma}^0]]
$$

$= [[H_{\alpha}^0, X_{\beta}^0]-n(\gamma , \alpha )X_{\beta}^0, X_{-\gamma}^0]$ theo (13)

$= [[H_{\alpha}^0, X_{\beta}^0]-n(\beta , \alpha )X_{\beta}^0, X_{-\gamma}^0]$ theo (14);

bây giờ, xét từ rỗng ngay lập tức cho

$$
([H_{\alpha}^0, X_{\beta}^0]-n(\beta , \alpha )X_{\beta}^0)(\emptyset ) = 0
$$

do đó (15) suy ra rằng

$$
([H_{\alpha}^0, X_{\beta}^0]-n(\beta , \alpha )X_{\beta}^0)X_{-\gamma_1}^0X_{-\gamma_2}^0. . . X_{-\gamma_n}^0(\emptyset ) = 0
$$

với mọi $\gamma_1, . . . , \gamma_n\in B$; điều này chứng minh (12).

#### Bổ đề 2 {#lie-viii-s4-lem-2 .statement tag=010W}

Các tự đồng cấu $X_{\alpha}^0,H_{\beta}^0,X_{-\gamma}^0$, trong đó $\alpha , \beta , \gamma \in B$, độc lập tuyến tính.

Vì $X_{-\alpha}^0(\emptyset ) =\alpha$, rõ ràng rằng các $X_{-\alpha}^0$ độc lập tuyến tính.

Giả sử rằng $\sum_{\alpha}a_{\alpha}H_{\alpha}^0= 0$; khi đó, với mọi $\beta \in B$,

$$
0 =[\sum_{\alpha}a_{\alpha}H_{\alpha}^0, X_{-\beta}^0]=-\sum_{\alpha}a_{\alpha}n(\beta , \alpha )X_{-\beta}^0
$$

vì det($n(\beta , \alpha )$)$\not= 0$, suy ra rằng $a_{\alpha}$ = 0 với mọi $\alpha$. Giả sử rằng $\sum_{\alpha}a_{\alpha}X_{\alpha}^0= 0$. Theo các công thức (7), (8), (9),

$$
X_{\alpha}^0(\beta ) = 0
$$

$$
X_{\alpha}^0(\beta , \beta ) = 2\delta_{\alpha \beta}\beta
$$

với mọi $\beta \in B$. Suy ra rằng $a_{\beta}= 0$ với mọi $\beta$. Vì $X_{\alpha}^0, H_{\alpha}^0, X_{-\alpha}^0$ lần lượt có bậc $-1,0,1$, bổ đề suy ra từ những gì đã được chứng minh trước đó.

Cho I là tập hợp $B\times  \{-1,0,1\}$. Đặt $x_{\alpha}= (\alpha ,-1),h_{\alpha}= (\alpha ,0)$, và $x_{-\alpha}= (\alpha ,1)$. Gọi $\mathfrak{a}$ là đại số Lie được xác định bởi họ sinh I và tập hợp sau $\mathscr{R}$ gồm các quan hệ:

$$
[h_{\alpha}, h_{\beta}]
$$

$$
[h_{\alpha}, x_{\beta}]-n(\beta , \alpha )x_{\beta}
$$

$$
[h_{\alpha}, x_{-\beta}] +n(\beta , \alpha )x_{-\beta}
$$

$$
[x_{\alpha}, x_{-\alpha}] +h_{\alpha}
$$

$[x_{\alpha}, x_{-\beta}]$ nếu $\alpha \not=\beta$

(xem Chương II, §2, no. 3). Theo Bổ đề 1, tồn tại một biểu diễn tuyến tính duy nhất $\rho$ của $\mathfrak{a}$ trên E sao cho

$$
\rho (x_{\alpha}) =X_{\alpha}^0, \rho (h_{\alpha}) =H_{\alpha}^0, \rho (x_{-\alpha}) =X_{-\alpha}^0
$$

Theo Bổ đề 2, điều này chứng minh kết quả sau:

#### Bổ đề 3 {#lie-viii-s4-lem-3 .statement tag=010X}

Các ảnh chính tắc trong $\mathfrak{a}$ của các phần tử $x_{\alpha}, h_{\beta}, x_{-\gamma}$, trong đó $\alpha , \beta , \gamma \in B$, là độc lập tuyến tính.

Trong phần sau, ta đồng nhất $x_{\alpha}, h_{\alpha}, x_{-\alpha}$ với các ảnh chính tắc của chúng trong $\mathfrak{a}$.

#### Bổ đề 4 {#lie-viii-s4-lem-4 .statement tag=010Y}

Tồn tại một tự đẳng cấu đối hợp duy nhất $\theta$ của $\mathfrak{a}$ sao cho

$$
\theta (x_{\alpha}) =x_{-\alpha}, \theta (x_{-\alpha}) =x_{\alpha}, \theta (h_{\alpha}) =-h_{\alpha}
$$

với mọi $\alpha \in B$.

Thật vậy, tồn tại một tự đẳng cấu đối hợp của đại số Lie tự do L(I) thỏa mãn các điều kiện này. Nó giữ $\mathscr{R}\cup (-\mathscr{R})$ ổn định, và do đó xác định qua phép chuyển sang thương một tự đẳng cấu đối hợp của $\mathfrak{a}$ thỏa mãn các điều kiện của bổ đề. Tính duy nhất suy ra từ sự kiện rằng $\mathfrak{a}$ được sinh bởi các phần tử $x_{\alpha}, h_{\alpha}, x_{-\alpha}(\alpha \in B)$.

Tự đẳng cấu này được gọi là tự đẳng cấu đối hợp chính tắc của $\mathfrak{a}$.

Cho Q là tập hợp các trọng số căn của R; đây là một $\mathbf{Z}$-môđun tự do với cơ sở B (Ch. VI, §1, no. 9). Tồn tại một phân hoạch kiểu Q trên đại số Lie tự do L(I) sao cho $x_{\alpha}, h_{\alpha}, x_{-\alpha}$ có các bậc lần lượt là $\alpha ,0,-\alpha$ (Ch. II, §2, no. 6). Khi đó các phần tử của $\mathscr{R}$ là thuần nhất. Do đó tồn tại một phân hoạch duy nhất kiểu Q trên $\mathfrak{a}$ tương thích với cấu trúc đại số Lie của $\mathfrak{a}$ và sao cho $x_{\alpha}, h_{\alpha}, x_{-\alpha}$ có các bậc lần lượt là $\alpha ,0,-\alpha$. Với mọi $\mu\in Q$, ký hiệu $\mathfrak{a}^\mu$ là tập hợp các phần tử của $\mathfrak{a}$ thuần nhất có bậc $\mu$.

#### Bổ đề 5 {#lie-viii-s4-lem-5 .statement tag=010Z}

Cho $z\in \mathfrak{a}$. Khi đó $z\in \mathfrak{a}^\mu$ khi và chỉ khi $[h_{\alpha}, z] =\langle \mu, \alpha^{\vee}\rangle z$ với mọi $\alpha \in B$.

Với $\mu\in Q$, gọi $\mathfrak{a}^{(\mu)}$ là tập hợp các $x\in \mathfrak{a}$ sao cho $[h_{\alpha}, x] =\langle \mu, \alpha^{\vee}\rangle x$ với mọi $\alpha \in B$. Tổng của các $\mathfrak{a}^{(\mu)}$ là trực tiếp. Để chứng minh bổ đề, do đó chỉ cần chỉ ra rằng $\mathfrak{a}^\mu\subset \mathfrak{a}^{(\mu)}$. Cho $\alpha \in B$. Tự đồng cấu $u$ của không gian vectơ $\mathfrak{a}$ sao cho $u|\mathfrak{a}^\mu=\langle \mu, \alpha^{\vee}\rangle .1$ là một đạo hàm của $\mathfrak{a}$ sao cho $ux=$ (ad $h_{\alpha}$)$.x$ đối với $x=x_{\beta}, x=h_{\beta}, x=x_{-\beta}$; do đó $u=$ ad $h_{\alpha}$, điều này chứng minh mệnh đề của ta.

#### Nhận xét {#lie-viii-s4-n2-rem-1 .statement tag=0110}

Suy ra từ Bổ đề 5 rằng mọi iđêan của $\mathfrak{a}$ đều thuần nhất, vì nó ổn định dưới ad $h_{\alpha}$.

Ký hiệu $Q_+$ (tương ứng $Q_-$) là tập hợp các tổ hợp tuyến tính của các phần tử của B với các hệ số nguyên dương (tương ứng âm), không phải tất cả đều bằng không. Đặt $\mathfrak{a}_+=$ $\sum_{\mu\in Q_+}a^\mu$ và $\mathfrak{a}_-=\sum_{\mu\in Q_-}\mathfrak{a}^\mu$. Vì $Q_++ Q_+\subset Q_+$ và $Q_-+ Q_-\subset Q_-,\mathfrak{a}_+$

và $\mathfrak{a}_-$ là các đại số Lie con của $\mathfrak{a}$.

#### Mệnh đề 2 {#lie-viii-s4-prop-2 .statement tag=0111}

(i) Đại số Lie $\mathfrak{a}_+$ được sinh bởi họ $(x_{\alpha})_{\alpha\in B}$.

(ii) Đại số Lie $\mathfrak{a}_-$ được sinh bởi họ $(x_{-\alpha})_{\alpha\in B}$.

(iii) Họ $(h_{\alpha})_{\alpha\in B}$ là một cơ sở của không gian vectơ $\mathfrak{a}^0$.

(iv) Không gian vectơ $\mathfrak{a}$ là tổng trực tiếp của $\mathfrak{a}_+,\mathfrak{a}^0,\mathfrak{a}_-$.

Cho $\mathfrak{r}$ (tương ứng $\mathfrak{n}$) là đại số con Lie của $\mathfrak{a}$ sinh bởi $(x_{\alpha})_{\alpha\in B}$ (tương ứng $(x_{-\alpha})_{\alpha\in B}$), và $\mathfrak{h}$ là không gian con vectơ của $\mathfrak{a}$ sinh bởi $(h_{\alpha})_{\alpha\in B}$. Vì các $x_{\alpha}$ là các phần tử thuần nhất của $\mathfrak{a}_+,\mathfrak{r}$ là một đại số con phân bậc của $\mathfrak{a}_+$; do đó, $[\mathfrak{h},\mathfrak{r}]\subset \mathfrak{r}$, nên $\mathfrak{h}+\mathfrak{r}$ là một đại số con của $\mathfrak{a}$; vì

$$
[x_{-\alpha}, x_{\beta}] =\delta_{\alpha \beta}h_{\alpha}
$$

$[x_{-\alpha},\mathfrak{r}]\subset \mathfrak{h}+\mathfrak{r}$ với mọi $\alpha \in B$. Tương tự, $\mathfrak{n}$ là một đại số con phân bậc của $\mathfrak{a}_-$, ta có $[\mathfrak{h},\mathfrak{n}]\subset \mathfrak{n},\mathfrak{h}+\mathfrak{n}$ là một đại số con của $\mathfrak{n}$, và $[x_{\alpha},\mathfrak{n}]\subset \mathfrak{h}+\mathfrak{n}$ với mọi $\alpha \in B$. Đặt $\mathfrak{a}'=\mathfrak{r}+\mathfrak{h}+\mathfrak{n}$. Điều trên cho thấy rằng $\mathfrak{a}'$ ổn định đối với ad $x_{\alpha}$, ad $h_{\alpha}$ và ad $x_{-\alpha}$ với mọi $\alpha \in B$, và do đó là một iđêan của $\mathfrak{a}$. Vì $\mathfrak{a}'$ chứa $x_{\alpha}, h_{\alpha}, x_{-\alpha}$ với mọi $\alpha \in B,\mathfrak{a}'=\mathfrak{a}$. Từ đó suy ra rằng các bao hàm $\mathfrak{r}\subset \mathfrak{a}_+,\mathfrak{h}\subset \mathfrak{a}^0$, $\mathfrak{n}\subset \mathfrak{a}_-$ là các đẳng thức, điều này chứng minh mệnh đề.

#### Mệnh đề 3 {#lie-viii-s4-prop-3 .statement tag=0112}

Đại số Lie $\mathfrak{a}_+$ (tương ứng $\mathfrak{a}_-$) là một đại số Lie tự do với họ cơ bản $(x_{\alpha})_{\alpha\in B}$ (tương ứng $(x_{-\alpha})_{\alpha\in B}$) (xem Chương II, §2, no. 3).

Gọi L là đại số con Lie của E sinh bởi B. Theo Chương II, §3, Đl. 1, L có thể được đồng nhất với đại số Lie tự do sinh bởi B. Biểu diễn chính quy trái của E trên chính nó là đơn ánh một cách rõ ràng, và bằng cách hạn chế vào L nó xác định một biểu diễn đơn ánh $\rho '$ của đại số Lie L trên E. Gọi $\varphi$ là đồng cấu duy nhất từ L đến $\mathfrak{a}_-$ nhận $\alpha$ thành $x_{-\alpha}$ với mọi $\alpha \in B$. Khi đó, với mọi $\alpha \in B,\rho (\varphi (\alpha ))$ là tự đồng cấu của phép nhân trái bởi $\alpha$ trên E, do đó $\rho \circ \varphi =\rho '$, điều này chứng minh rằng $\varphi$ là đơn ánh. Vậy, $(x_{-\alpha})_{\alpha\in B}$ là một họ cơ bản của $\mathfrak{a}_-$. Vì $\theta (x_{-\alpha}) =x_{\alpha}$ với mọi $\alpha$ (xem Bổ đề $4$)$, (x_{\alpha})_{\alpha\in B}$ là một họ cơ bản của $\mathfrak{a}_+$.

### 3. ĐỊNH LÝ TỒN TẠI

Ta giữ các giả thiết và ký hiệu của số trước. Nhắc lại rằng nếu $\alpha , \beta \in B$ và nếu $\alpha \not=\beta$, thì $n(\beta , \alpha )\leq 0$; hơn nữa, nếu $n(\beta , \alpha ) = 0$, thì $n(\alpha , \beta ) = 0$ (Chap. VI, §1, no. 1, công thức (8)). Với mọi cặp $(\alpha , \beta )$ các phần tử phân biệt của B, đặt

$x_{\alpha \beta}=$ (ad $x_{\alpha}$)$^{1-n(\beta ,\alpha)}x_{\beta}y_{\alpha \beta}=$ (ad $x_{-\alpha}$)$^{1-n(\beta ,\alpha)}x_{-\beta}$.

Khi đó $x_{\alpha \beta}\in \mathfrak{a}_+, y_{\alpha \beta}\in \mathfrak{a}_-$. Nếu $\theta$ là tự đẳng cấu chính tắc của $\mathfrak{a}$, thì $\theta (x_{\alpha \beta}) =y_{\alpha \beta}$.

#### Bổ đề 6 {#lie-viii-s4-lem-6 .statement tag=0113}

Cho $\alpha , \beta \in B$ với $\alpha \not=\beta$. Khi đó

$$
[\mathfrak{a}_+, y_{\alpha \beta}] = 0[\mathfrak{a}_-, x_{\alpha \beta}] = 0
$$

Công thức thứ hai suy ra từ công thức thứ nhất bằng cách dùng tự đẳng cấu $\theta$. Để chứng minh công thức thứ nhất, chỉ cần chỉ ra rằng $[x_{\gamma}, y_{\alpha \beta}] = 0$ với mọi $\gamma \in B$. Ta phân biệt ba trường hợp.

Trường hợp 1$:\gamma \not=\alpha$ và $\gamma \not=\beta$. Trong trường hợp này, $x_{\gamma}$ giao hoán với $x_{-\alpha}$ và $x_{-\beta}$, do đó giao hoán với $y_{\alpha \beta}$.

Trường hợp 2$:\gamma =\beta$. Trong trường hợp này, $x_{\gamma}$ giao hoán với $x_{-\alpha}$, nên

$[x_{\gamma}, y_{\alpha \beta}] =$ (ad $x_{-\alpha}$)$^{1-n(\beta ,\alpha)}[x_{\gamma}, x_{-\beta}]$

$=-$(ad $x_{-\alpha}$)$^{1-n(\beta ,\alpha)}h_{\beta}=-n(\alpha , \beta$)(ad $x_{-\alpha}$)$^{-n(\beta ,\alpha)}x_{-\alpha}$.

Nếu $n(\beta , \alpha )<0$, biểu thức này bằng không vì (ad $x_{-\alpha}$)$.x_{-\alpha}= 0$. Nếu $n(\beta , \alpha ) = 0$, thì $n(\alpha , \beta ) = 0$. Trong cả hai trường hợp, $[x_{\gamma}, y_{\alpha \beta}] = 0$.

Trường hợp 3$:\gamma =\alpha$. Trong đại số các tự đồng cấu của $\mathfrak{a}$, $[$-ad $h_{\alpha}$, ad $x_{-\alpha}] = 2$ ad $x_{-\alpha}$

và [ad $x_{\alpha}$, ad $x_{-\alpha}] =$-ad $h_{\alpha}$; do đó, theo §1, Bổ đề 1,

[ad $x_{\alpha}$, (ad $x_{-\alpha}$)$^{1-n(\beta ,\alpha)}] = (1-n(\beta , \alpha$))(ad $x_{-\alpha}$)$^{-n(\beta ,\alpha)}($-ad $h_{\alpha}-n(\beta , \alpha ))$.

Do đó,

$[x_{\gamma}, y_{\alpha \beta}] =$ [ad $x_{\alpha}$, (ad $x_{-\alpha}$)$^{1-n(\beta ,\alpha)}]x_{-\beta}+$ (ad $x_{-\alpha}$)$^{1-n(\beta ,\alpha)}$(ad $x_{\alpha}$)$x_{-\beta}$

$=-(1-n(\beta , \alpha$))(ad $x_{-\alpha}$)$^{-n(\beta ,\alpha)}$(ad $h_{\alpha}+n(\beta , \alpha )$)$x_{-\beta}$

+ (ad $x_{-\alpha}$)$^{1-n(\beta ,\alpha)}$(ad $x_{\alpha}$)$x_{-\beta}$.

Bây giờ $[h_{\alpha}, x_{-\beta}] +n(\beta , \alpha )x_{-\beta}= 0$ và $[x_{\alpha}, x_{-\beta}] = 0$, do đó $[x_{\gamma}, y_{\alpha \beta}] = 0$.

#### Bổ đề 7 {#lie-viii-s4-lem-7 .statement tag=0114}

Iđêan $\mathfrak{n}$ của $\mathfrak{a}_+$ sinh bởi các $x_{\alpha \beta}(\alpha , \beta \in B, \alpha \not=\beta )$ là một iđêan của $\mathfrak{a}$. Iđêan của $\mathfrak{a}_-$ sinh bởi các $y_{\alpha \beta}(\alpha , \beta \in B, \alpha \not=\beta )$ là một iđêan của $\mathfrak{a}$ và bằng $\theta (\mathfrak{n})$.

Đặt $\mathfrak{n}'=\sum_{\alpha ,\beta\in B,\alpha\not=\beta}kx_{\alpha \beta}$. Vì mỗi $x_{\alpha \beta}$ là thuần nhất trong $\mathfrak{a}, [\mathfrak{a}^0,\mathfrak{n}']\subset \mathfrak{n}'$

(Bổ đề 5 và Mệnh đề 2). Gọi U (tương ứng V) là đại số bao của $\mathfrak{a}$ (tương ứng $\mathfrak{a}_+$), và $\sigma$ là biểu diễn của U trên $\mathfrak{a}$ xác định bởi biểu diễn phụ hợp của $\mathfrak{a}$. Iđêan của $\mathfrak{a}$ sinh bởi $\mathfrak{n}'$ là $\sigma (U)\mathfrak{n}'$. Bây giờ $\mathfrak{a}=\mathfrak{a}_++\mathfrak{a}^0+\mathfrak{a}_-$ (Mệnh đề $2$)$,\sigma (\mathfrak{a}_-)\mathfrak{n}'= 0$ (Bổ đề 6), và $\sigma (\mathfrak{a}^0)\mathfrak{n}'\subset \mathfrak{n}'$ theo điều đã nêu trước đó. Theo định lý Poincaré-Birkhoff-Witt, $\sigma (U)\mathfrak{n}'=\sigma (V)\mathfrak{n}'$, điều này chứng minh mệnh đề đầu tiên của bổ đề. Suy ra rằng iđêan của $\theta (\mathfrak{a}_+) =\mathfrak{a}_-$ sinh bởi các $\theta (x_{\alpha \beta}) =y_{\alpha \beta}(\alpha , \beta \in B, \alpha \not=\beta )$ là iđêan $\theta (\mathfrak{n})$ của $\mathfrak{a}$. Q.E.D.

Ideal $\mathfrak{n}+\theta (\mathfrak{n})$ của $\mathfrak{a}$ được phân bậc vì nó được sinh bởi các phần tử thuần nhất. Do đó, đại số Lie $\mathfrak{a}/(\mathfrak{n}+\theta (\mathfrak{n}))$ là một đại số Lie phân bậc Q; trong phần còn lại của đoạn này, nó được ký hiệu là $\mathfrak{g}_B$, hoặc đơn giản là $\mathfrak{g}$. Theo Mệnh đề 2, nếu $\mathfrak{g}^\mu\not= 0$ thì $\mu\in Q_+$, hoặc $\mu\in Q_-$, hoặc $\mu= 0$. Ký hiệu $X_{\alpha}$ (resp. $H_{\alpha}, X_{-\alpha}$) là ảnh chính tắc của $x_{\alpha}$ (resp. $h_{\alpha}, x_{-\alpha}$) trong $\mathfrak{g}$. Theo định nghĩa của $\mathfrak{a},\mathfrak{n}$ và $\theta (\mathfrak{n})$, suy ra rằng $\mathfrak{g}$ là đại số Lie được xác định bởi họ sinh $((X_{\alpha}, H_{\alpha}, X_{-\alpha}))_{\alpha\in B}$ và các hệ thức

$$
[H_{\alpha}, H_{\beta}] = 0 \tag{16}
$$

$$
[H_{\alpha}, X_{\beta}]-n(\beta , \alpha )X_{\beta}= 0 \tag{17}
$$

$$
[H_{\alpha}, X_{-\beta}] +n(\beta , \alpha )X_{-\beta}= 0 \tag{18}
$$

$$
[X_{\alpha}, X_{-\alpha}] +H_{\alpha}= 0 \tag{19}
$$

$$
[X_{\alpha}, X_{-\beta}] = 0(\alpha \not=\beta ) \tag{20}
$$

(ad $X_{\alpha}$)$^{1-n(\beta ,\alpha)}X_{\beta}= 0(\alpha \not=\beta )$ (21)

(ad $X_{-\alpha}$)$^{1-n(\beta ,\alpha)}X_{-\beta}= 0(\alpha \not=\beta )$. (22)

Cho $z\in \mathfrak{g}$ và $\mu\in Q$. Khi đó $z\in \mathfrak{g}^\mu$ khi và chỉ khi $[H_{\alpha}, z] =\langle \mu, \alpha^{\vee}\rangle z$ với mọi $\alpha \in B$. Điều này suy ra từ Bổ đề 5.

Vì $\mathfrak{a}^0\cap (\mathfrak{n}+\theta (\mathfrak{n})) = 0$, ánh xạ chính tắc từ $\mathfrak{a}^0$ vào $\mathfrak{g}^0$ là một đẳng cấu. Do đó, $(H_{\alpha})_{\alpha\in B}$ là một cơ sở của không gian vectơ $\mathfrak{g}^0$. Đại số con giao hoán $\mathfrak{g}^0$ của $\mathfrak{g}_B$ sẽ được ký hiệu là $\mathfrak{h}_B$ hoặc đơn giản là $\mathfrak{h}$. Tồn tại một đẳng cấu duy nhất $\mu \rightarrow \mu_B$ từ V vào $\mathfrak{h}^*$ sao cho $\langle \mu_B, H_{\alpha}\rangle =\langle \mu, \alpha^{\vee}\rangle$ với mọi $\mu\in V$ và mọi $\alpha \in B$.

Tự đẳng cấu đối hợp $\theta$ của $\mathfrak{a}$ xác định, qua phép chuyển sang thương, một tự đẳng cấu đối hợp của $\mathfrak{g}$ cũng được ký hiệu là $\theta$. Ta có $\theta (X_{\alpha}) =X_{-\alpha}$ với $\alpha \in B\cup (-B)$, và $\theta (H_{\alpha}) =-H_{\alpha}$.

#### Định lý 1 {#lie-viii-s4-thm-1 .statement tag=0115}

Cho R là một hệ nghiệm rút gọn, B là một cơ sở của R. Cho $\mathfrak{g}$ là đại số Lie được xác định bởi họ sinh $((X_{\alpha}, H_{\alpha}, X_{-\alpha}))_{\alpha\in B}$ và các quan hệ (16) đến (22). Cho $\mathfrak{h}=\sum_{\alpha\in B}kH_{\alpha}$. Khi đó $(\mathfrak{g},\mathfrak{h})$ là một đại số Lie nửa đơn tách. Đẳng cấu $\mu \rightarrow \mu_B$ từ V đến $\mathfrak{h}^*$ biến R thành hệ nghiệm của $(\mathfrak{g},\mathfrak{h})$. Với mọi $\mu\in R,\mathfrak{g}^\mu$ là không gian riêng tương ứng với nghiệm $\mu$.

Chứng minh theo chứng minh của các Bổ đề 8, 9, 10, 11.

#### Bổ đề 8 {#lie-viii-s4-lem-8 .statement tag=0116}

Cho $\alpha \in B\cup (-B)$. Khi đó ad $X_{\alpha}$ là lũy linh địa phương.$^1$

Giả sử rằng $\alpha \in B$. Cho $\mathfrak{g}'$ là tập hợp các $z\in \mathfrak{g}$ sao cho (ad $X_{\alpha}$)$^pz= 0$ với $p$ đủ lớn. Vì ad $X_{\alpha}$ là một đạo hàm của $\mathfrak{g},\mathfrak{g}'$ là một đại số con của $\mathfrak{g}$. Theo (21), $X_{\beta}\in \mathfrak{g}'$ với mọi $\beta \in B$. Theo (17), (19), (20), $H_{\beta}\in \mathfrak{g}'$ và $X_{-\beta}\in \mathfrak{g}'$ với mọi $\beta \in B$. Do đó $\mathfrak{g}'=\mathfrak{g}$ và ad $X_{\alpha}$ là lũy linh địa phương. Vì ad $X_{-\alpha}=\theta$(ad $X_{\alpha}$)$\theta^{-1}$, ta thấy rằng ad $X_{-\alpha}$ là lũy linh địa phương.

Ta sẽ thấy rằng $\mathfrak{g}$ là hữu hạn chiều, do đó ad $X_{\alpha}$ thực sự là lũy linh.

#### Bổ đề 9 {#lie-viii-s4-lem-9 .statement tag=0117}

Cho $\mu, \nu \in Q$ và $w\in W(R)$ sao cho $w\mu=\nu$. Tồn tại một tự đẳng cấu của $\mathfrak{g}$ biến $\mathfrak{g}^\mu$ thành $\mathfrak{g}^{\nu}$.

Với mọi $\alpha \in B$, cho $s_{\alpha}$ là phép đối xứng trong V được xác định bởi $\alpha$. Vì W(R) được sinh bởi các $s_{\alpha}$ (Chương VI, §1, no. 5, Nhận xét 1), chỉ cần chứng minh bổ đề khi $w=s_{\alpha}$. Theo Bổ đề 8, ta có thể định nghĩa

$$
\theta_{\alpha}=e^{adX_{\alpha}}e^{adX_{-\alpha}}e^{adX_{\alpha}}
$$

Ta kiểm tra được như trong Chương I, §6, no. 8, rằng $\theta_{\alpha}$ là một tự đẳng cấu của $\mathfrak{g}$. Ta có

$^1$ Một tự đồng cấu $u$ của một không gian vectơ V được gọi là lũy linh địa phương (hoặc gần

lũy linh) nếu, với mọi $v\in V$, tồn tại một số nguyên dương $n$ sao cho $u^n(v) = 0$

(xem Đại số giao hoán, Chương IV, §1, no. 4, Định nghĩa 2). Khi đó exp($u$), hay $e^u$, được

định nghĩa bởi công thức $e^u(v) =\sum_{n\geq 0}(1/n$!)$u^n(v)$ với mọi $v\in V$. $\theta_{\alpha}(H_{\alpha}) =e^{adX_{\alpha}}e^{adX_{-\alpha}}(H_{\beta}-n(\alpha , \beta )X_{\alpha})$

$$
=e^{adX_{\alpha}}(H_{\beta}-n(\alpha , \beta )X_{\alpha}+n(\alpha , \beta )X_{-\alpha}-n(\alpha , \beta )H_{\alpha}-\frac{n(\alpha , \beta)}{2}2X_{-\alpha})
$$

$$
=e^{adX_{\alpha}}(H_{\beta}-n(\alpha , \beta )H_{\alpha}-n(\alpha , \beta )X_{\alpha})
$$

$$
=H_{\beta}-n(\alpha , \beta )H_{\alpha}-n(\alpha , \beta )X_{\alpha}-n(\alpha , \beta )X_{\alpha}-n(\alpha , \beta )(-2X_{\alpha})
$$

$$
=H_{\beta}-n(\alpha , \beta )H_{\alpha}
$$

Nếu $z\in \mathfrak{g}^\mu$,

$$
[H_{\beta}, \theta_{\alpha}^{-1}z] =\theta_{\alpha}^{-1}[H_{\beta}-n(\alpha , \beta )H_{\alpha}, z]
$$

$$
=\theta_{\alpha}^{-1}(\langle \mu, \beta^{\vee}\rangle z-n(\alpha , \beta )\langle \mu, \alpha^{\vee}\rangle z)
$$

$$
=\langle \mu- \langle \alpha^{\vee}, \mu\rangle \alpha , \beta^{\vee}\rangle \theta^{-1}_{\alpha}z=\langle s_{\alpha}\mu, \beta^{\vee}\rangle \theta^{-1}_{\alpha}z
$$

do đó $\theta_{\alpha}^{-1}z\in \mathfrak{g}^{s_{\alpha}\mu}$. Điều này cho thấy rằng $\theta^{-1}_{\alpha}\mathfrak{g}^\mu\subset \mathfrak{g}^{s_{\alpha}\mu}$. Vì $\theta_{\alpha}$ là một tự đẳng cấu và vì bao hàm này đúng với mọi $\mu\in Q$, ta thấy rằng $\theta_{\alpha}^{-1}\mathfrak{g}^\mu=\mathfrak{g}^{s_{\alpha}\mu}$, điều này chứng minh bổ đề.

#### Bổ đề 10 {#lie-viii-s4-lem-10 .statement tag=0118}

Cho $\mu\in Q$, và giả sử rằng $\mu$ không là bội của một nghiệm. Tồn tại $w\in W(R)$ sao cho một số tọa độ của $w\mu$ đối với cơ sở B là $>0$ và một số tọa độ khác là $<0$.

Gọi $V_{\mathbf{R}}$ là không gian vectơ $Q\otimes_{\mathbf{Z}}\mathbf{R}$, trong đó R là một hệ nghiệm. Theo giả thiết, tồn tại $f\in V^*_{\mathbf{R}}$ sao cho $\langle f, \alpha \rangle  \not= 0$ với mọi $\alpha \in R$, và $\langle f, \mu\rangle = 0$. Tồn tại một phòng C của $R^{\vee}$ sao cho $f\in C$. Theo Chương VI, §1, no. 5, Định lý 2 (i), tồn tại $w\in W(R)$ sao cho $wf$ thuộc phòng liên kết với B, nói cách khác sao cho $\langle wf, \alpha \rangle >0$ với mọi $\alpha \in B$. Viết $w\mu=\sum_{\alpha\in B}t_{\alpha}\alpha$. Khi đó

$$
0 =\langle f, \mu\rangle =\langle wf, w\mu\rangle =\sum_{\alpha\in B}t_{\alpha}\langle wf, \alpha \rangle
$$

điều này chứng minh rằng một số $t_{\alpha}$ là $>0$ và các số khác là $<0$.

#### Bổ đề 11 {#lie-viii-s4-lem-11 .statement tag=0119}

Cho $\mu\in Q$. Nếu $\mu \notin R\cup \{0\}$, thì $\mathfrak{g}^\mu= 0$. Nếu $\mu\in R$, thì dim$\mathfrak{g}^\mu= 1$.

1) Nếu $\mu$ không là bội của một phần tử của R, tồn tại $w\in W$ sao cho $w\mu \notin Q_+\cup Q_-$ (Bổ đề 10), do đó $\mathfrak{a}^{w\mu}= 0,\mathfrak{g}^{w\mu}= 0$, và vì vậy $\mathfrak{g}^\mu= 0$ (Bổ đề 9).

2) Cho $\alpha \in B$ và cho $m$ là một số nguyên. Vì $\mathfrak{a}_+$ là một đại số Lie tự do với họ cơ bản $(x_{\alpha})_{\alpha\in B}$, ta có dim$\mathfrak{a}^{\alpha}= 1$ và $\mathfrak{a}^{m\alpha}= 0$ với $m >1$ (Chương II, §2, no. 6, Mệnh đề 4). Do đó dim$\mathfrak{g}^{\alpha}\leq 1$ và $\mathfrak{g}^{m\alpha}= 0$ với $m >1$. Ta không thể có $\mathfrak{g}^{\alpha}= 0$, vì điều này sẽ kéo theo $x_{\alpha}\in \mathfrak{n}+\theta \mathfrak{n}$, và do đó $\mathfrak{n}+\theta \mathfrak{n}$ chứa $h_{\alpha}=-[x_{\alpha}, x_{-\alpha}]$, trong khi $\mathfrak{a}^0\cap (\mathfrak{n}+\theta \mathfrak{n}) = 0$. Do đó, dim$\mathfrak{g}^{\alpha}= 1$.

3) Nếu $\mu\in R$, tồn tại $w\in W(R)$ sao cho $w(\mu)\in B$ (Chương VI, §1, no. 5, Mệnh đề 15), do đó dim $\mathfrak{g}^\mu=$ dim $\mathfrak{g}^{w\mu}= 1$. Hơn nữa, nếu $n$ là một số nguyên $>1$ thì $\mathfrak{g}^{nw(\mu)}= 0$ và do đó $\mathfrak{g}^{n\mu}= 0$.

Chứng minh Định lý 1.

Vì dim$\mathfrak{g}^0=$ Card B, suy ra từ Bổ đề 11 rằng $\mathfrak{g}$ có số chiều hữu hạn bằng Card B + Card R. Ta chứng minh rằng $\mathfrak{g}$ là nửa đơn. Cho $\mathfrak{k}$ là một iđêan giao hoán của $\mathfrak{g}$. Vì $\mathfrak{k}$ ổn định dưới ad($\mathfrak{h}$)$,\mathfrak{k}= (\mathfrak{k}\cap \mathfrak{h}) +\sum_{\mu\in R}(\mathfrak{k}\cap \mathfrak{g}^\mu)$.

Rõ ràng là, với mọi $\alpha \in B,\mathfrak{g}^{\alpha}+\mathfrak{g}^{-\alpha}+kH_{\alpha}$ đẳng cấu với $\mathfrak{s}\mathfrak{l}(2, k)$. Theo Bổ đề 9, với mọi $\mu\in R,\mathfrak{g}^\mu$ được chứa trong một đại số con của $\mathfrak{g}$ đẳng cấu với $\mathfrak{s}\mathfrak{l}(2, k)$; do đó, $\mathfrak{k}\cap \mathfrak{g}^\mu= 0$, suy ra $\mathfrak{k}\subset \mathfrak{h}$; vì thế

$$
[\mathfrak{k},\mathfrak{g}^\mu]\subset \mathfrak{k}\cap \mathfrak{g}^\mu= 0
$$

nên $\mu_B(\mathfrak{k}) = 0$ với mọi $\mu\in R$. Suy ra $\mathfrak{k}= 0$, điều này chứng minh rằng $\mathfrak{g}$ là nửa đơn.

Cho $\mu\in R$. Tồn tại $\alpha \in B$ sao cho $\langle \mu, \alpha^{\vee}\rangle  \not= 0$, và (ad $H_{\alpha}$)$|\mathfrak{g}^\mu$ khi đó là một phép vị tự khác không. Do đó, $\mathfrak{h}$ bằng chuẩn hóa tử của chính nó trong $\mathfrak{g}$, và vì thế là một đại số con Cartan của $\mathfrak{g}$. Với mọi $u\in \mathfrak{h}$, ad $u$ chéo hóa được, do đó $(\mathfrak{g},\mathfrak{h})$ là một đại số Lie nửa đơn tách.

Đối với mọi $\mu\in R$, rõ ràng rằng $\mu_B$ là một nghiệm của $(\mathfrak{g},\mathfrak{h})$ và rằng $\mathfrak{g}^\mu$ là không gian riêng tương ứng. Số các nghiệm của $(\mathfrak{g},\mathfrak{h})$ là dim$\mathfrak{g}-$ dim $\mathfrak{h}=$ Card R. Do đó, ánh xạ $\mu \rightarrow \mu_B$ từ V vào $\mathfrak{h}^*$ ánh xạ R vào hệ nghiệm của $(\mathfrak{g},\mathfrak{h})$.

### ĐỊNH LÝ DUY NHẤT

#### Mệnh đề 4 {#lie-viii-s4-prop-4 .statement tag=011A}

Cho $(\mathfrak{g},\mathfrak{h},B,(X_{\alpha})_{\alpha\in B})$ là một đại số Lie nửa đơn có khung. Cho $(n(\alpha , \beta ))_{\alpha ,\beta\in B}$ và $(X_{\alpha})_{\alpha\in B\cup(-B)}$ lần lượt là ma trận Cartan và họ sinh tương ứng.

(i) Họ $((X_{\alpha}, H_{\alpha}, X_{-\alpha}))_{\alpha\in B}$ và các quan hệ (16) đến (22) của no. 3 tạo thành một trình bày của $\mathfrak{g}$.

(ii) Họ $(X_{\alpha})_{\alpha\in B}$ và các quan hệ (21) của no. 3 tạo thành một trình bày của đại số con của $\mathfrak{g}$ sinh bởi $(X_{\alpha})_{\alpha\in B}$.

Cho R là hệ nghiệm của $(\mathfrak{g},\mathfrak{h})$. Áp dụng cho R và B các phép xây dựng của nos. 2 và 3, ta thu được các đối tượng mà ta sẽ ký hiệu bởi $\mathfrak{a}',\mathfrak{g}', X'_{\alpha}, H'_{\alpha}, . .$. thay vì $\mathfrak{a},\mathfrak{g}, X_{\alpha}, H_{\alpha}, . .$..

Có một đồng cấu $\varphi$ từ đại số Lie $\mathfrak{g}'$ vào đại số Lie $\mathfrak{g}$ sao cho $\varphi (X'_{\alpha}) =X_{\alpha},\varphi (H'_{\alpha}) =H_{\alpha},\varphi (X'_{-\alpha}) =X_{-\alpha}$ với mọi $\alpha \in B$ (Mệnh đề 1). Vì dim $\mathfrak{g}'$ = Card R + Card B = dim$\mathfrak{g},\varphi$ là song ánh. Điều này chứng minh (i).

Đại số con của $\mathfrak{g}'=\mathfrak{a}'/(\mathfrak{n}'\oplus \theta '\mathfrak{n}') = (\mathfrak{a}'_+\oplus {\mathfrak{a}'}^0\oplus \mathfrak{a}'_-)/(\mathfrak{n}'\oplus \theta '\mathfrak{n}')$ sinh bởi $(X'_{\alpha})_{\alpha\in B}$ có thể được đồng nhất với $\mathfrak{a}'_+/\mathfrak{n}'$. Theo Mệnh đề 3 và định nghĩa của $\mathfrak{n}'$, điều này chứng minh (ii).

#### Hệ quả {#lie-viii-s4-n4-cor-1 .statement tag=011B}

Mọi đại số Lie nửa đơn có khung đều thu được từ một đại số Lie nửa đơn $\mathbf{Q}$ có khung bằng phép mở rộng vô hướng từ $\mathbf{Q}$ đến $k$.

Điều này suy ra ngay lập tức từ mệnh đề.

#### Định lý 2 {#lie-viii-s4-thm-2 .statement tag=011C}

Cho $(\mathfrak{g},\mathfrak{h},B,(X_{\alpha})_{\alpha\in B})$ và $(\mathfrak{g}',\mathfrak{h}',B',(X'_{\alpha})_{\alpha\in B'})$ là các đại số Lie nửa đơn có khung, cho R và $R'$ là các hệ nghiệm của $(\mathfrak{g},\mathfrak{h})$ và $(\mathfrak{g}',\mathfrak{h}')$, cho $(n(\alpha , \beta ))_{\alpha ,\beta\in B}$ (tương ứng $(n'(\alpha , \beta ))_{\alpha ,\beta\in B'}$) là ma trận Cartan của R (tương ứng $R'$) đối với B (tương ứng $B'$), và cho $\Delta$ (tương ứng $\Delta '$) là đồ thị Dynkin của R (tương ứng $R'$) đối với B (tương ứng $B'$).

(i) Nếu $\varphi$ là một đẳng cấu từ $\mathfrak{h}^*$ đến $\mathfrak{h}^{'*}$ sao cho $\varphi (R) = R'$ và $\varphi (B) = B'$, thì tồn tại một đẳng cấu duy nhất $\psi$ từ $(\mathfrak{g},\mathfrak{h},B,(X_{\alpha})_{\alpha\in B})$ đến $(\mathfrak{g}',\mathfrak{h}',B',(X'_{\alpha})_{\alpha\in B'})$ sao cho $\psi |\mathfrak{h}=^t\varphi^{-1}$.

(ii) Nếu $f$ là một song ánh từ B đến $B'$ sao cho $n'(f(\alpha ), f(\beta )) =n(\alpha , \beta )$ với mọi $\alpha , \beta \in$ B, tồn tại một đẳng cấu từ $(\mathfrak{g},\mathfrak{h},B,(X_{\alpha})_{\alpha\in B})$ đến $(\mathfrak{g}',\mathfrak{h}',B',(X'_{\alpha})_{\alpha\in B'})$.

(iii) Nếu tồn tại một đẳng cấu từ $\Delta$ đến $\Delta '$, tồn tại một đẳng cấu từ $(\mathfrak{g},\mathfrak{h},B,(X_{\alpha})_{\alpha\in B})$ đến $(\mathfrak{g}',\mathfrak{h}',B',(X'_{\alpha})_{\alpha\in B'})$.

Điều này suy ra ngay lập tức từ Mệnh đề 4 (i) (sử dụng Chương VI, §4, no. 2, Mệnh đề 1 cho phần (iii)).

#### Chú giải {#lie-viii-s4-n4-sch-1 .statement tag=011D}

Với mỗi đại số Lie nửa đơn tách được $\mathfrak{g}$, liên kết với nó là một đồ thị Dynkin, đồ thị này xác định $\mathfrak{g}$ sai khác một đẳng cấu (Định lý 2 (iii)). Đồ thị này rỗng và liên thông khi và chỉ khi $\mathfrak{g}$ là đơn (§3, no. 2, Hệ quả 1 của Mệnh đề 6). Theo Định lý 1 của no. 3, và Chương VI, §4, no. 2, Định lý 3, các đại số Lie đơn tách được là các đại số kiểu $A_l(l\geq 1), B_l(l\geq 2), C_l(l\geq 3), D_l(l\geq 4)$, $E_6, E_7, E_8, F_4, G_2$. Không có hai đại số nào trong danh sách này là đẳng cấu.

#### Mệnh đề 5 {#lie-viii-s4-prop-5 .statement tag=011E}

Cho $(\mathfrak{g},\mathfrak{h},B,(X_{\alpha})_{\alpha\in B})$ là một đại số Lie nửa đơn có khung, và $(X_{\alpha})_{\alpha\in B\cup(-B)}$ là họ sinh tương ứng. Tồn tại một tự đẳng cấu duy nhất $\theta$ của $\mathfrak{g}$ sao cho $\theta (X_{\alpha}) =X_{-\alpha}$ với mọi $\alpha \in B\cup (-B)$. Ta có $\theta^2=$ Id$_{\mathfrak{g}}$, và $\theta (h) =-h$ với mọi $h\in \mathfrak{h}$.

Tính duy nhất là rõ ràng vì $(X_{\alpha})_{\alpha\in B\cup(-B)}$ sinh đại số Lie $\mathfrak{g}$. Theo Mệnh đề 4, sự tồn tại của $\theta$ suy ra từ điều đã nói trong no. 3 trước Định lý 1.

#### Hệ quả {#lie-viii-s4-n4-cor-2 .statement tag=011F}

Cho $(\mathfrak{g},\mathfrak{h})$ là một đại số Lie nửa đơn tách. Khi đó $(\mathfrak{g},\mathfrak{h})$ có một hệ Chevalley (§2, no. 4, Định nghĩa 3).

Cho R là hệ nghiệm của $(\mathfrak{g},\mathfrak{h})$. Với mọi $\alpha \in R$, cho $X_{\alpha}$ là một phần tử khác không của $\mathfrak{g}^{\alpha}$. Giả sử rằng các $X_{\alpha}$ được chọn sao cho $[X_{\alpha}, X_{-\alpha}] =-H_{\alpha}$ với mọi $\alpha \in R ($§2, no. 4, Bổ đề 2). Cho B là một cơ sở của R và $\theta$ là tự đẳng cấu của $\mathfrak{g}$ sao cho $\theta (X_{\alpha}) =X_{-\alpha}$ với mọi $\alpha \in B\cup (-B)$. Ta có $\theta |\mathfrak{h}=-$Id$_{\mathfrak{h}}$. Do đó, với mọi $\alpha \in R$ tồn tại $t_{\alpha}\in k^*$ sao cho $\theta X_{\alpha}=t_{\alpha}X_{-\alpha}$. Ta có

$$
t_{\alpha}t_{-\alpha}H_{\alpha}= [t_{\alpha}X_{-\alpha}, t_{-\alpha}X_{\alpha}] = [\theta X_{\alpha}, \theta X_{-\alpha}] =\theta ([X_{\alpha}, X_{-\alpha}])
$$

$$
=\theta (-H_{\alpha}) =H_{\alpha}
$$

vì vậy $t_{\alpha}t_{-\alpha}= 1$ với mọi $\alpha \in R$. Đưa vào các $N_{\alpha \beta}$ như trong §2, no. 4. Nếu $\alpha , \beta , \alpha +\beta \in R$,

$$
N_{-\alpha ,-\beta}t_{\alpha}t_{\beta}X_{-\alpha-\beta}=t_{\alpha}t_{\beta}[X_{-\alpha}, X_{-\beta}] = [\theta X_{\alpha}, \theta X_{\beta}] =\theta ([X_{\alpha}, X_{\beta}])
$$

$$
= N_{\alpha \beta}\theta X_{\alpha+\beta}= N_{\alpha \beta}t_{\alpha+\beta}X_{-\alpha-\beta}
$$

do đó, theo §2, no. 4, Bổ đề 4,

$$
(q+ 1)^2t_{\alpha}t_{\beta}= N^2_{\alpha \beta}t_{\alpha+\beta}
$$

trong đó $q$ là một số nguyên. Suy ra rằng nếu $t_{\alpha}$ và $t_{\beta}$ là các bình phương trong $k^*$, thì $t_{\alpha+\beta}$ cũng vậy. Vì $t_{\alpha}= 1$ với mọi $\alpha \in B$, Mệnh đề 19 của Chương VI, §1, no. 6, chứng minh rằng $t_{\alpha}$ là một bình phương với mọi $\alpha \in R$. Chọn, với mọi $\alpha \in R$, một $u_{\alpha}\in k$ sao cho $u^2_{\alpha}=t_{\alpha}$. Lựa chọn này có thể được thực hiện sao cho $u_{\alpha}u_{-\alpha}= 1$ với mọi $\alpha \in R$. Đặt $X'_{\alpha}=u^{-1}_{\alpha}X_{\alpha}$. Khi đó, với mọi $\alpha \in R$,

$$
X'_{\alpha}\in \mathfrak{g}^{\alpha},[X'_{\alpha}, X'_{-\alpha}] = [X_{\alpha}, X_{-\alpha}] =-H_{\alpha}
$$

và $\theta (X'_{\alpha}) =\theta (u^{-1}_{\alpha}X_{\alpha}) =u^{-1}_{\alpha}t_{\alpha}X_{-\alpha}=u_{\alpha}X_{-\alpha}=u_{\alpha}u_{-\alpha}X'_{-\alpha}=X'_{-\alpha}$, do đó $(X'_{\alpha})_{\alpha\in R}$ là một hệ Chevalley của $(\mathfrak{g},\mathfrak{h})$.

### Bài tập {#lie-viii-s4-exercises}

Các đại số Lie được xét trong đoạn này không nhất thiết là hữu hạn chiều.

Xem các [bài tập cho § 4](exercises/s4/).
