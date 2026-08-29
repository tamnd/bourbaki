---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: IX
chapter_title: COMPACT REAL LIE GROUPS
section: 3
section_title: Compact forms of complex semi-simple Lie algebras
lang: vi
source: lie-vii-ix
book_pages: 296-303, 394-396
pdf_pages: 0303-0310, 0401-0403
extraction: native+ocr
subsections:
    - "no": 1
      title: REAL FORMS
      page: 296
      pdf_page: 303
    - "no": 2
      title: REAL FORMS ASSOCIATED TO A CHEVALLEY SYSTEM
      page: 297
      pdf_page: 304
    - "no": 3
      title: CONJUGACY OF COMPACT FORMS
      page: 299
      pdf_page: 306
    - "no": 4
      title: 'EXAMPLE I: COMPACT ALGEBRAS OF TYPE A$_{\boldsymbol{n}}$'
      page: 300
      pdf_page: 307
    - "no": 5
      title: 'EXAMPLE II: COMPACT ALGEBRAS OF TYPE B$_{\boldsymbol{n}}\mathbf{A}\mathbf{N}\mathbf{D}$ $\mathbf{D}_{\boldsymbol{n}}$'
      page: 301
      pdf_page: 308
    - "no": 6
      title: COMPACT GROUPS OF RANK 1
      page: 302
      pdf_page: 309
statements: 17
exercises: 9
content_sha256: d8611ee0cd49856d4bcb9156cdaa925daa3be4539797ce805c36ee512e2d3953
translated_from: content/en/lie/IX/03_s3_compact_forms_of_complex_semi_simple.md
source_content_sha256: bf0ebd0cda151170c108a2f9b899a1c59ba20dd5f6195c4caf5f17e7cc05a3cd
translation_model: gpt-5.4
translation_run: translate-vi-ca8df590
glossary_version: 34
glossary_terms_sha256: 715d81c2d3519565ab2c83b9e18b8cc29494bde8b515e0425be3b42e1acf5dad
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 3. CÁC DẠNG COMPACT CỦA CÁC ĐẠI SỐ LIE NỬA ĐƠN PHỨC

### 1. CÁC DẠNG THỰC

Nếu $\mathfrak{a}$$ là một đại số Lie phức, ta ký hiệu bởi $\mathfrak{a}_{[\mathbf{R}]}$ (hoặc đôi khi bởi $\mathfrak{a}$) đại số Lie thực thu được bằng phép hạn chế vô hướng. Nếu $\mathfrak{g}$ là một đại số Lie thực, ta ký hiệu bởi $\mathfrak{g}_{(\mathbf{C})}$ (hoặc đôi khi bởi $\mathfrak{g}_{\mathbf{C}}$) đại số Lie phức $\mathbf{C}\otimes_{\mathbf{R}}\mathfrak{g}$ thu được bằng phép mở rộng vô hướng. Các đồng cấu của các đại số Lie thực $\mathfrak{g}\rightarrow \mathfrak{a}_{[\mathbf{R}]}$ tương ứng song ánh với các đồng cấu của các đại số Lie phức $\mathfrak{g}_{(\mathbf{C})}\rightarrow \mathfrak{a}:$ nếu $f:\mathfrak{g}\rightarrow \mathfrak{a}_{[\mathbf{R}]}$ và $g:\mathfrak{g}_{(\mathbf{C})}\rightarrow \mathfrak{a}$ tương ứng với nhau, ta có $f(x) =g(1\otimes x)$ và $g(\lambda \otimes x) =\lambda f(x)$ với $x\in \mathfrak{g}, \lambda \in \mathbf{C}$.

#### Định nghĩa 1 {#lie-ix-s3-def-1 .statement tag=01B1}

Cho $\mathfrak{a}$ là một đại số Lie phức. Một dạng thực của $\mathfrak{a}$ là một đại số con thực $\mathfrak{g}$ của $\mathfrak{a}$, là một cấu trúc $\mathbf{R}$ trên không gian vectơ $\mathbf{C}$ $\mathfrak{a}($Algebra, Chap. II, §8, no. 1, Định nghĩa 1).

Điều đó có nghĩa là đồng cấu của các đại số Lie phức $\mathfrak{g}_{(\mathbf{C})}\rightarrow \mathfrak{a}$ liên kết với đơn ánh chính tắc $\mathfrak{g}\rightarrow \mathfrak{a}_{[\mathbf{R}]}$ là song ánh. Do đó, một đại số con thực $\mathfrak{g}$ của $\mathfrak{a}$ là một dạng thực của $\mathfrak{a}$ khi và chỉ khi các không gian con $\mathfrak{g}$ và $i\mathfrak{g}$ của không gian vectơ thực $\mathfrak{a}$ bù nhau. Phép liên hợp của $\mathfrak{a}$ đối với dạng thực $\mathfrak{g}$ là ánh xạ $\sigma :\mathfrak{a}\rightarrow \mathfrak{a}$ sao cho

$$
\sigma (x+iy) =x-iy,x, y\in \mathfrak{g} \tag{1}
$$

#### Mệnh đề 1 {#lie-ix-s3-prop-1 .statement tag=01JF}

$a)$ Cho $\mathfrak{g}$ là một dạng thực của $\mathfrak{a}$ và $\sigma$ là phép liên hợp của $\mathfrak{a}$ đối với $\mathfrak{g}$. Khi đó:

$\sigma^2=$ Id$_{\mathfrak{a}}, \sigma (\lambda x+\mu y) = \overline{\lambda \sigma}(x) + \overline{\mu\sigma}(y),[\sigma (x), \sigma (y)] =\sigma [x, y]$ (2)

với $\lambda , \mu\in \mathbf{C},x, y\in \mathfrak{a}$. Một phần tử $x$ của $\mathfrak{a}$ thuộc $\mathfrak{g}$ khi và chỉ khi $\sigma (x) =x$.

b) Cho $\sigma :\mathfrak{a}\rightarrow \mathfrak{a}$ là một ánh xạ thỏa mãn (2). Khi đó tập hợp $\mathfrak{g}$ các điểm bất động của $\sigma$ là một dạng thực của $\mathfrak{a}$, và $\sigma$ là phép liên hợp của $\mathfrak{a}$ đối với $\mathfrak{g}$.

Chứng minh là ngay lập tức.

Chú ý rằng nếu B ký hiệu dạng Killing của $\mathfrak{a}$, và nếu $\mathfrak{g}$ là một dạng thực của $\mathfrak{a}$, thì hạn chế của B lên $\mathfrak{g}$ là dạng Killing của $\mathfrak{g}$; đặc biệt, B nhận giá trị thực trên $\mathfrak{g}\times \mathfrak{g}$. Giả sử rằng $\mathfrak{a}$ là khả quy; khi đó đại số Lie thực $\mathfrak{g}$ là compact nếu và chỉ nếu hạn chế của B lên $\mathfrak{g}$ là âm (§1, no. 3). Trong trường hợp đó ta nói rằng $\mathfrak{g}$ là một dạng thực compact của $\mathfrak{a}$.

### 2. CÁC DẠNG THỰC LIÊN KẾT VỚI MỘT HỆ CHEVALLEY

Trong số này, ta xét một đại số Lie nửa đơn tách $(\mathfrak{a},\mathfrak{h})$ trên trường $\mathbf{C}$ (Ch. VIII, §2, no. 1), với hệ nghiệm $R(\mathfrak{a},\mathfrak{h}) = R$, và một hệ Chevalley $(X_{\alpha})_{\alpha\in R}$ của $(\mathfrak{a},\mathfrak{h})$ (Ch. VIII, §2, no. 4, Định nghĩa 3).

Nhắc lại (loc. cit.) rằng ánh xạ tuyến tính $\theta :\mathfrak{a}\rightarrow \mathfrak{a}$ trùng với $-$Id$_{\mathfrak{h}}$ trên $\mathfrak{h}$ và biến $X_{\alpha}$ thành $X_{-\alpha}$ với mọi $\alpha \in R$ là một tự đẳng cấu của $\mathfrak{a}$. Hơn nữa (loc. cit., Mệnh đề 7), nếu $\alpha , \beta , \alpha +\beta$ là các nghiệm, thì

$$
[X_{\alpha}, X_{\beta}] = N_{\alpha ,\beta}X_{\alpha+\beta} \tag{3}
$$

với $N_{\alpha ,\beta}\in \mathbf{R}^*$ và

$$
N_{-\alpha ,-\beta}= N_{\alpha ,\beta} \tag{4}
$$

Ký hiệu bởi $\mathfrak{h}_0$ không gian con vectơ thực của $\mathfrak{h}$ gồm các $H\in \mathfrak{h}$ sao cho $\alpha (H)\in \mathbf{R}$ với mọi $\alpha \in R$. Khi đó $\mathfrak{h}_0$ là một $\mathbf{R}$-cấu trúc trên không gian vectơ phức $\mathfrak{h}$, ta có $[X_{\alpha}, X_{-\alpha}]\in \mathfrak{h}_0$ với mọi $\alpha \in R$, và hạn chế của dạng Killing B của $\mathfrak{a}$ lên $\mathfrak{h}_0$ là xác định dương (Ch. VIII, §2, no. 2, Nhận xét 2). Hơn nữa,

$B(H, X_{\alpha}) = 0,B(X_{\alpha}, X_{\beta}) = 0$ nếu $\alpha +\beta \not= 0,B(X_{\alpha}, X_{-\alpha})<0$ (5)

(Ch. VIII, §2, no. 2, Mệnh đề 1 và no. 4, Bổ đề 3).

#### Mệnh đề 2 {#lie-ix-s3-prop-2 .statement tag=01JG}

$a)$ Không gian con vectơ thực $\mathfrak{a}_0=\mathfrak{h}_0+\sum_{\alpha\in R}\mathbf{R}X_{\alpha}$ của $\mathfrak{a}$ là một dạng thực của $\mathfrak{a}$, trong đó $\mathfrak{h}_0$ là một đại số con Cartan. Cặp $(\mathfrak{a}_0,\mathfrak{h}_0)$ là một đại số Lie thực nửa đơn tách, trong đó $(X_{\alpha})$ là một hệ Chevalley.

b) Cho $\sigma$ là phép liên hợp của $\mathfrak{a}$ đối với $\mathfrak{a}_0$. Khi đó $\sigma \circ \theta =\theta \circ \sigma$. Tập các điểm bất động của $\sigma \circ \theta$ là một dạng thực compact $\mathfrak{a}_u$ của $\mathfrak{a}$, trong đó $i\mathfrak{h}_0$ là một đại số con Cartan.

Phần a) suy ra ngay lập tức từ điều trước đó. Ta chứng minh b). Vì $\sigma \circ \theta$ và $\theta \circ \sigma$ là hai ánh xạ nửa tuyến tính từ $\mathfrak{a}$ đến $\mathfrak{a}$ trùng nhau trên $\mathfrak{a}_0$, nên chúng trùng nhau. Bây giờ $\sigma \circ \theta$ thỏa mãn các điều kiện (2) của no. 1, do đó là phép liên hợp của $\mathfrak{a}$ đối với dạng thực $\mathfrak{a}_u$ gồm các $x\in \mathfrak{a}$ sao cho $\sigma \circ \theta (x) =x$ (Prop. 1). Với mọi $\alpha \in R$, đặt

$$
u_{\alpha}=X_{\alpha}+X_{-\alpha},v_{\alpha}=i(X_{\alpha}-X_{-\alpha}) \tag{6}
$$

Khi đó không gian vectơ $\mathbf{R}$ $\mathfrak{a}_u$ được sinh bởi $i\mathfrak{h}_0$, các $u_{\alpha}$ và các $v_{\alpha}$. Chính xác hơn, nếu ta chọn một buồng C của R, thì

$$
\mathfrak{a}_u=i\mathfrak{h}_0\oplus \bigoplus_{\alpha\in R_+(C)}(\mathbf{R}u_{\alpha}+\mathbf{R}v_{\alpha}) \tag{7}
$$

Hiển nhiên $i\mathfrak{h}_0$ là một đại số con Cartan của $\mathfrak{a}_u$, và còn phải chứng minh rằng hạn chế của B trên $\mathfrak{a}_u$ là âm. Bây giờ $i\mathfrak{h}_0$ và các không gian con khác nhau dạng $\mathbf{R}u_{\alpha}\oplus \mathbf{R}v_{\alpha}$ trực giao đối với B, theo (5); hạn chế của B trên $i\mathfrak{h}_0$ là âm và

$$
B(u_{\alpha}, u_{\alpha}) = B(v_{\alpha}, v_{\alpha}) = 2B(X_{\alpha}, X_{-\alpha})<0,B(u_{\alpha}, v_{\alpha}) = 0 \tag{8}
$$

do đó suy ra kết luận.

#### Nhận xét {#lie-ix-s3-n2-rem-1 .statement tag=01B2}

Với các ký hiệu trên, ta có các công thức sau:

$$
[h, u_{\alpha}] =-i\alpha (h)v_{\alpha},[h, v_{\alpha}] =i\alpha (h)u_{\alpha},[u_{\alpha}, v_{\alpha}] = 2iH_{\alpha},(h\in \mathfrak{h}) \tag{9}
$$

$$
[u_{\alpha}, u_{\beta}] = N_{\alpha ,\beta}u_{\alpha+\beta}+ N_{\alpha ,-\beta}u_{\alpha-\beta},\alpha \not=\pm \beta \tag{10}
$$

$$
[v_{\alpha}, v_{\beta}] =-N_{\alpha ,\beta}u_{\alpha+\beta}+ N_{\alpha ,-\beta}u_{\alpha-\beta},\alpha \not=\pm \beta \tag{11}
$$

$$
[u_{\alpha}, v_{\beta}] = N_{\alpha ,\beta}v_{\alpha+\beta}-N_{\alpha ,-\beta}v_{\alpha-\beta},\alpha \not=\pm \beta \tag{12}
$$

(trong ba công thức cuối, như thường lệ, hiểu rằng $N_{\gamma ,\delta}= 0$ nếu $\gamma +\delta$ không phải là một nghiệm).

Chú ý rằng $\sum\mathbf{R}u_{\alpha}$ là một đại số con thực của $\mathfrak{a}$, tức là $\mathfrak{a}_0\cap \mathfrak{a}_u$.

Gọi Q(R) là nhóm các trọng số căn của R (Chap. VI, §1, no. 9). Nhớ lại rằng với mọi đồng cấu $\gamma : Q(R)\rightarrow \mathbf{C}^*$ đều liên kết một tự đẳng cấu sơ cấp $f(\gamma )$ của $\mathfrak{a}$ sao cho $f(\gamma )(h) =h$ với mọi $h\in \mathfrak{h}$ và $f(\gamma )X_{\alpha}=$ $\gamma (\alpha )X_{\alpha}$ (Chap. VIII, §5, no. 2).

#### Mệnh đề 3 {#lie-ix-s3-prop-3 .statement tag=01B3}

Cho $\mathfrak{g}$ là một dạng thực compact của $\mathfrak{a}$ sao cho $\mathfrak{g}\cap \mathfrak{h}=i\mathfrak{h}_0$. Tồn tại một đồng cấu $\gamma : Q(R)\rightarrow \mathbf{R}^*_+$ sao cho $\mathfrak{g}=f(\gamma )(\mathfrak{a}_u)$.

Gọi $\tau$ là phép liên hợp của $\mathfrak{a}$ đối với $\mathfrak{g}$. Theo giả thiết $\tau (x) =x$ với $x\in i\mathfrak{h}_0$, nên $\tau (x) =-x$ với $x\in \mathfrak{h}_0$. Do đó, với mọi $\alpha \in R$ và mọi $h\in \mathfrak{h}_0$,

$$
[h, \tau (X_{\alpha})] = [-\tau (h), \tau (X_{\alpha})] =-\tau ([h, X_{\alpha}]) =-\tau (\alpha (h)X_{\alpha})
$$

suy ra rằng $[h, \tau (X_{\alpha})] =-\alpha (h)\tau (X_{\alpha})$ với mọi $h\in \mathfrak{h}_0$, do đó cũng với mọi $h\in \mathfrak{h}$. Vậy tồn tại $c_{\alpha}\in \mathbf{C}^*$ sao cho $\tau (X_{\alpha}) =c_{\alpha}X_{-\alpha}$. Vì $[X_{\alpha}, X_{-\alpha}]\in \mathfrak{h}_0$, ta có $[\tau (X_{\alpha}), \tau (X_{-\alpha})] =-[X_{\alpha}, X_{-\alpha}]$, nên $c_{\alpha}c_{-\alpha}$ = 1; tương tự, các công thức (3) và (4) cho $c_{\alpha+\beta}=c_{\alpha}c_{\beta}$ nếu $\alpha , \beta , \alpha +\beta$ là các gốc. Theo Ch. VI, §1, no. 6, Hệ quả 2 của Mệnh đề 19, tồn tại một đồng cấu $\delta : Q(R)\rightarrow \mathbf{C}^*$ sao cho $\delta (\alpha ) =c_{\alpha}$ với mọi $\alpha \in R$.

Bây giờ ta sẽ chỉ ra rằng mỗi $c_{\alpha}$ đều dương ngặt. Thật vậy, $c_{\alpha}B(X_{\alpha}, X_{-\alpha}) =$ $B(X_{\alpha}, \tau (X_{\alpha}))$, và vì $B(X_{\alpha}, X_{-\alpha})$ là âm, chỉ cần chỉ ra rằng $B(z, \tau (z))<0$ với mọi phần tử khác không $z$ của $\mathfrak{a}$; nhưng mọi phần tử của $\mathfrak{a}$ đều có thể viết dưới dạng $x+iy$, với $x$ và $y$ thuộc $\mathfrak{g}$, và

$$
B(x+iy, \tau (x+iy)) = B(x+iy, x-iy) = B(x, x) + B(y, y)
$$

do đó suy ra mệnh đề đã nêu, hạn chế của B lên $\mathfrak{g}$ là âm và phân ly theo giả thiết.

Suy ra đồng cấu $\delta$ nhận giá trị trong $\mathbf{R}^*_+$; do đó tồn tại một đồng cấu $\gamma : Q(R)\rightarrow \mathbf{R}^*_+$ sao cho $\delta =\gamma^{-2}$. Khi đó $f(\gamma )^{-1}(\mathfrak{g})$ là một dạng thực của $\mathfrak{a}$; phép liên hợp tương ứng là $\tau '=f(\gamma )^{-1}\circ \tau \circ f(\gamma )$. Với mọi $\alpha \in R$, ta có

$$
\tau '(X_{\alpha}) =f(\gamma )^{-1}(\tau (c^{-1/2}_{\alpha}X_{\alpha})) =f(\gamma )^{-1}(c^{1/2}_{\alpha}X_{-\alpha}) =X_{-\alpha}
$$

và $\tau '(h) =\tau (h) =h$ với $h\in i\mathfrak{h}_0$; suy ra $\tau '$ là phép liên hợp đối với $\mathfrak{a}_u$, và do đó $f(\gamma )^{-1}(\mathfrak{g}) =\mathfrak{a}_u$.

### 3. TÍNH LIÊN HỢP CỦA CÁC DẠNG COMPACT

#### Định lý 1 {#lie-ix-s3-thm-1 .statement tag=01B4}

Cho $\mathfrak{a}$ là một đại số Lie nửa đơn phức.

a$)\mathfrak{a}$ có các dạng thực compact (tương ứng, phân rã được).

b) Nhóm Int($\mathfrak{a}$) tác động bắc cầu trên tập hợp các dạng thực compact (tương ứng, phân rã được) của $\mathfrak{a}$.

Cho $\mathfrak{h}$ là một đại số con Cartan của $\mathfrak{a}$. Khi đó $(\mathfrak{a},\mathfrak{h})$ là tách (Chương VIII, §2, no. 1, Nhận xét 2), và có một hệ Chevalley $(X_{\alpha})$ (Chương VIII, §4, no. 4, Hệ quả của Mệnh đề 5). Phần a) bây giờ suy ra từ Mệnh đề 2. Cho $\mathfrak{g}$ là một dạng thực compact của $\mathfrak{a}$; ta sẽ chỉ ra rằng tồn tại $v\in$ Int($\mathfrak{a}$) sao cho $v(\mathfrak{a}_u) =\mathfrak{g}$. Cho $\mathfrak{t}$ là một đại số con Cartan của $\mathfrak{g}$; khi đó $\mathfrak{t}_{(\mathbf{C})}$ là một đại số con Cartan của $\mathfrak{a}$; vì Int($\mathfrak{a}$) tác động bắc cầu trên tập hợp các đại số con Cartan của $\mathfrak{a}$ (Chương VII, §3, no. 2, Định lý 1), nên ta được đưa về trường hợp $\mathfrak{t}_{(\mathbf{C})}=\mathfrak{h}$. Vì $\mathfrak{g}$ là một dạng compact, các trị riêng của các nội tự đồng cấu ad $h$, với $h\in \mathfrak{t}$, là thuần ảo (§1, no. 3, Mệnh đề 1), nên các căn $\alpha \in R$ ánh xạ $\mathfrak{t}$ vào $i\mathbf{R}$; điều này kéo theo $\mathfrak{t}=i\mathfrak{h}_0$. Khi đó, theo Mệnh đề 3 (no. 2), tồn tại $v\in$ Int($\mathfrak{a}$) sao cho $v(\mathfrak{a}_u) =\mathfrak{g}$, do đó suy ra b) trong trường hợp các dạng compact. Cuối cùng, cho $\mathfrak{m}_1$ và $\mathfrak{m}_2$ là hai dạng thực tách được của $\mathfrak{a}$. Tồn tại các khung $(\mathfrak{m}_1,\mathfrak{h}_1,B_1,(X_{\alpha}^1))$ và $(\mathfrak{m}_2,\mathfrak{h}_2,B_2,(X_{\alpha}^2))$ (Chương VIII, §4, no. 1). Chúng mở rộng một cách hiển nhiên thành các cơ sở $e_1$ và $e_2$ của $\mathfrak{a}$. Một tự đẳng cấu của $\mathfrak{a}$ ánh xạ $e_1$ lên $e_2$ thì ánh xạ $\mathfrak{m}_1$ lên $\mathfrak{m}_2$; như vậy, chỉ cần áp dụng Mệnh đề 5 của Chương VIII, §5, no. 3, để thu được sự tồn tại của một phần tử $u$ của Aut$_0(\mathfrak{a}) =$ Int($\mathfrak{a}$) sao cho $u(\mathfrak{m}_1) =\mathfrak{m}_2$.

#### Nhận xét {#lie-ix-s3-n3-rem-1 .statement tag=01B5}

Mãi về sau ta sẽ thấy một phân loại tổng quát các dạng thực của một đại số Lie nửa đơn phức.

#### Hệ quả 1 {#lie-ix-s3-thm-1-cor-1 .statement tag=01B6}

Cho $\mathfrak{g}$ và $\mathfrak{g}'$ là hai đại số Lie thực compact. Khi đó $\mathfrak{g}$ và $\mathfrak{g}'$ đẳng cấu nếu và chỉ nếu các đại số Lie phức $\mathfrak{g}_{(\mathbf{C})}$ và $\mathfrak{g}'_{(\mathbf{C})}$ đẳng cấu.

Điều kiện này rõ ràng là cần thiết. Ngược lại, giả sử rằng $\mathfrak{g}_{(\mathbf{C})}$ và $\mathfrak{g}'_{(\mathbf{C})}$ đẳng cấu. Gọi $\mathfrak{c}$ (resp. $\mathfrak{c}'$) là tâm của $\mathfrak{g}$ (resp. $\mathfrak{g}'$) và $\mathfrak{s}$ (resp. $\mathfrak{s}'$) là đại số dẫn xuất của $\mathfrak{g}$ (resp. $\mathfrak{g}'$). Khi đó $\mathfrak{c}_{(\mathbf{C})}$ và $\mathfrak{c}'_{(\mathbf{C})}$ lần lượt là các tâm của $\mathfrak{g}_{(\mathbf{C})}$ và $\mathfrak{g}'_{(\mathbf{C})}$, nên chúng đẳng cấu; suy ra các đại số giao hoán $\mathfrak{c}$ và $\mathfrak{c}'$ đẳng cấu. Tương tự, $\mathfrak{s}_{(\mathbf{C})}$ và $\mathfrak{s}'_{(\mathbf{C})}$ đẳng cấu, do đó $\mathfrak{s}$ và $\mathfrak{s}'$, là các dạng thực compact của hai đại số Lie nửa đơn phức đẳng cấu, đẳng cấu theo Đl. $1b)$.

#### Hệ quả 2 {#lie-ix-s3-thm-1-cor-2 .statement tag=01B7}

Cho $\mathfrak{a}$ là một đại số Lie phức. Các điều kiện sau là tương đương:

(i) $\mathfrak{a}$ là khả quy.

(ii) Tồn tại một đại số Lie thực compact $\mathfrak{g}$ sao cho $\mathfrak{a}$ đẳng cấu với $\mathfrak{g}_{(\mathbf{C})}$.

(iii) Tồn tại một nhóm Lie compact G sao cho $\mathfrak{a}$ đẳng cấu với $L(G)_{(\mathbf{C})}$.

Theo Định nghĩa 1 của §1, no. 3, các điều kiện (ii) và (iii) là tương đương và kéo theo (i). Nếu $\mathfrak{a}$ là khả quy, thì nó là tích trực tiếp của một đại số giao hoán, rõ ràng có một dạng thực compact, và một đại số nửa đơn mà có một dạng như vậy theo Đl. $1a)$, do đó (i) kéo theo (ii).

#### Hệ quả 3 {#lie-ix-s3-thm-1-cor-3 .statement tag=01B8}

Cho $\mathfrak{a}_1$ và $\mathfrak{a}_2$ là hai đại số Lie nửa đơn phức. Các dạng thực compact của $\mathfrak{a}_1\times \mathfrak{a}_2$ là các tích $\mathfrak{g}_1\times \mathfrak{g}_2$, trong đó, với $i= 1,2,\mathfrak{g}_i$ là một dạng thực compact của $\mathfrak{a}_i$.

Thật vậy, tồn tại một dạng thực compact $\mathfrak{g}_1$ (resp. $\mathfrak{g}_2$) của $\mathfrak{a}_1$ (resp. $\mathfrak{a}_2$); khi đó $\mathfrak{g}_1\times \mathfrak{g}_2$ là một dạng thực compact của $\mathfrak{a}_1\times \mathfrak{a}_2$. Hệ quả khi đó suy ra từ Đl. $1b)$, áp dụng cho $\mathfrak{a}_1,\mathfrak{a}_2$ và $\mathfrak{a}_1\times \mathfrak{a}_2$.

Chú ý rằng từ Hệ quả 3 trên suy ra rằng một đại số Lie thực compact $\mathfrak{g}$ là đơn khi và chỉ khi đại số Lie phức $\mathfrak{g}_{(\mathbf{C})}$ là đơn. Ta nói rằng $\mathfrak{g}$ thuộc kiểu $A_n$, hoặc $B_n,. .$., nếu $\mathfrak{g}_{(\mathbf{C})}$ thuộc kiểu $A_n$, hoặc $B_n,. .$. (Chương VIII, §2, no. 2). Theo Hệ quả 1 trên, hai đại số Lie thực compact đơn là đẳng cấu khi và chỉ khi chúng cùng một kiểu.

Cho G là một nhóm Lie compact liên thông gần đơn (Chương III, §9, no. 8, Định nghĩa 3). Ta nói rằng G thuộc kiểu $A_n$, hoặc $B_n,. .$., nếu đại số Lie của nó thuộc kiểu $A_n$, hoặc $B_n,. .$.. Hai nhóm Lie compact gần đơn đơn liên thông là đẳng cấu khi và chỉ khi chúng cùng một kiểu.

### 4. VÍ DỤ I: ĐẠI SỐ COMPAC KIỂU A$_{\boldsymbol{n}}$

Cho V là một không gian vectơ phức hữu hạn chiều và $\Phi$ là một dạng Hermit dương phân ly trên V. Nhóm unita liên kết với $\Phi$ (xem Algebra, Chap. IX) là nhóm con $\mathbf{U}(\Phi )$ của $\mathbf{G}\mathbf{L}(V)$ gồm các tự đẳng cấu của không gian Hilbert phức $(V, \Phi )$; đó là một nhóm con Lie (thực) của nhóm $\mathbf{G}\mathbf{L}$(V), có đại số Lie là đại số con $\mathfrak{u}(\Phi )$ của đại số Lie thực $\mathfrak{g}\mathfrak{l}(V)$ gồm các nội cấu xạ $x$ của V sao cho $x^*=-x$ (Chap. III, §3, no. 10, Cor. 2 of Prop. 37), trong đó $x^*$ ký hiệu liên hợp của $x$ đối với $\Phi$. Vì nhóm $\mathbf{U}(\Phi )$ là compact (§1, no. $1$)$,\mathfrak{u}(\Phi )$ là một đại số Lie thực compact. Tương tự, nhóm unita đặc biệt $\mathbf{S}\mathbf{U}(\Phi ) =\mathbf{U}(\Phi )\cap \mathbf{S}\mathbf{L}(V)$ là một nhóm con Lie compact của $\mathbf{S}\mathbf{L}$(V), có đại số Lie là $\mathfrak{s}\mathfrak{u}(\Phi ) =\mathfrak{u}(\Phi )\cap \mathfrak{s}\mathfrak{l}(V)$.

Khi $V =\mathbf{C}^n$ và $\Phi$ là dạng Hermit thông thường (mà đối với nó cơ sở chính tắc của $\mathbf{C}^n$ là trực chuẩn), ta viết $\mathbf{U}(n,\mathbf{C}),\mathbf{S}\mathbf{U}(n,\mathbf{C}),\mathfrak{u}(n,\mathbf{C}),\mathfrak{s}\mathfrak{u}(n,\mathbf{C})$ thay cho $\mathbf{U}(\Phi ),\mathbf{S}\mathbf{U}(\Phi ),\mathfrak{u}(\Phi ),\mathfrak{s}\mathfrak{u}(\Phi )$. Các phần tử của $\mathbf{U}(n,\mathbf{C})$ (resp. $\mathfrak{u}(n,\mathbf{C})$) là các ma trận $A\in M_n(\mathbf{C})$ sao cho $A.^t\overline{A}=I_n$ (resp. $A=-^t\overline{A}$), và được gọi là unita (resp. phản Hermit).

#### Mệnh đề 4 {#lie-ix-s3-prop-4 .statement tag=01B9}

a) Các dạng thực compact của đại số Lie phức $\mathfrak{s}\mathfrak{l}(V)$ là các đại số $\mathfrak{s}\mathfrak{u}(\Phi )$, trong đó $\Phi$ thuộc tập hợp các dạng Hermit dương phân ly trên không gian vectơ phức V.

b) Các đại số $\mathfrak{u}(\Phi )$ là các dạng thực compact của $\mathfrak{g}\mathfrak{l}(V)$.

Cho $\Phi$ là một dạng Hermit dương phân ly trên V. Với mọi $x\in \mathfrak{g}\mathfrak{l}$(V), đặt $\sigma (x) =-x^*$ (trong đó $x^*$ là liên hợp của $x$ đối với $\Phi$ ). Khi đó $\sigma$ thỏa mãn các điều kiện (2) của Mệnh đề 1 ở no. 1, nên tập hợp $\mathfrak{u}(\Phi )$ (resp. $\mathfrak{s}\mathfrak{u}(\Phi )$) các điểm bất động của $\sigma$ trên $\mathfrak{g}\mathfrak{l}(V)$ (resp. $\mathfrak{s}\mathfrak{l}(V)$) là một dạng thực compact của $\mathfrak{g}\mathfrak{l}(V)$ (resp. $\mathfrak{s}\mathfrak{l}(V)$). Vì $\mathbf{G}\mathbf{L}(V)$ tác động bắc cầu trên tập hợp các dạng Hermit dương phân ly trên V (Algebra, Chap. IX) và trên tập hợp các dạng thực compact của $\mathfrak{s}\mathfrak{l}(V)$ (no. 3, Th. 1 and Chap. VIII, §13, no. 1 (VII)), Mệnh đề 4 được chứng minh.

#### Hệ quả {#lie-ix-s3-n4-cor-1 .statement tag=01BA}

Mọi đại số Lie thực đơn compact kiểu $A_n(n\geq 1)$ đều đẳng cấu với $\mathfrak{s}\mathfrak{u}(n+ 1,\mathbf{C})$.

Thật vậy, mọi đại số Lie phức kiểu $A_n$ đều đẳng cấu với $\mathfrak{s}\mathfrak{l}(n+ 1,\mathbf{C})$ (Chap. VIII, §13, no. 1).

#### Nhận xét 1 {#lie-ix-s3-n4-rem-1 .statement tag=01BB}

Ta có $\mathfrak{g}\mathfrak{l}(V) =\mathfrak{s}\mathfrak{l}(V)\times \mathbf{C}.1_V,\mathfrak{u}(\Phi ) =\mathfrak{s}\mathfrak{u}(\Phi )\times \mathbf{R}.i1_V$; các dạng thực compact của $\mathfrak{g}\mathfrak{l}(V)$ là các $\mathfrak{s}\mathfrak{u}(\Phi )\times \mathbf{R}.\alpha 1_V,\alpha \in \mathbf{C}^*$.

#### Nhận xét 2 {#lie-ix-s3-n4-rem-2 .statement tag=01BC}

Nếu đại số Lie phức $\mathfrak{a}=\mathfrak{s}\mathfrak{l}(n,\mathbf{C})$ được trang bị hệ tách và hệ Chevalley được đưa vào trong Chap. VIII, §13, no. 1 (IX), thì, với các ký hiệu ở no. 2,

$$
\mathfrak{a}_u=\mathfrak{s}\mathfrak{u}(n,\mathbf{C}),\mathfrak{a}_0=\mathfrak{s}\mathfrak{l}(n,\mathbf{R}),\mathfrak{a}_u\cap \mathfrak{a}_0=\mathfrak{o}(n,\mathbf{R})
$$

### 5. VÍ DỤ II: ĐẠI SỐ COMPACT KIỂU B$_{\boldsymbol{n}}\mathbf{A}\mathbf{N}\mathbf{D}$ $\mathbf{D}_{\boldsymbol{n}}$

Cho V là một không gian vectơ thực hữu hạn chiều và Q là một dạng toàn phương dương xác định trên V. Nhóm trực giao liên kết với Q (Đại số, Chương IX) là nhóm con $\mathbf{O}(Q)$ của $\mathbf{G}\mathbf{L}(V)$ gồm các tự đẳng cấu của không gian Hilbert thực $(V,Q)$; đó là một nhóm con Lie của $\mathbf{G}\mathbf{L}$(V), mà đại số Lie của nó là đại số con $\mathfrak{o}(Q)$ của $\mathfrak{g}\mathfrak{l}(V)$ gồm các nội tự đồng cấu $x$ của V sao cho $x^*=-x$ (Chương III, §3, no. 10, Hệ quả 2 của Mệnh đề $37$)$,x^*$ ký hiệu liên hợp của $x$ đối với Q. Vì nhóm $\mathbf{O}(Q)$ là compact, nên $\mathfrak{o}(Q)$ do đó là một đại số Lie thực compact. Đặt $\mathbf{S}\mathbf{O}(Q) =\mathbf{O}(Q)\cap \mathbf{S}\mathbf{L}(V)$; đó là một nhóm con đóng có chỉ số hữu hạn của $\mathbf{O}(Q)$ (chỉ số bằng 2 nếu dim $V\not= 0$), nên cũng có đại số Lie là $\mathfrak{o}(Q)$.

Khi $V =\mathbf{R}^n$ và Q là dạng toàn phương thông thường (đối với dạng này cơ sở chính tắc của $\mathbf{R}^n$ là trực chuẩn), ta viết $\mathbf{O}(n,\mathbf{R}),\mathbf{S}\mathbf{O}(n,\mathbf{R}),\mathfrak{o}(n,\mathbf{R})$ thay cho $\mathbf{O}(Q),\mathbf{S}\mathbf{O}(Q),\mathfrak{o}(Q)$. Các phần tử của $\mathbf{O}(n,\mathbf{R})$ (tương ứng, $\mathfrak{o}(n,\mathbf{R})$) là các ma trận $A\in M_n(\mathbf{R})$ sao cho $A.^tA=I_n$ (tương ứng, $A=-^tA$), và được gọi là trực giao (tương ứng, phản đối xứng).

Cho $V_{(\mathbf{C})}$ là không gian vectơ phức liên kết với V và cho $Q_{(\mathbf{C})}$ là dạng toàn phương trên $V_{(\mathbf{C})}$ liên kết với Q. Đồng nhất $\mathfrak{g}\mathfrak{l}(V)_{(\mathbf{C})}$ với $\mathfrak{g}\mathfrak{l}(V_{(\mathbf{C})})$; khi đó $\mathfrak{o}(Q)_{(\mathbf{C})}$ được đồng nhất với $\mathfrak{o}(Q_{(\mathbf{C})}):$ điều này hiển nhiên vì ánh xạ $x \rightarrow x^*+x$ từ $\mathfrak{g}\mathfrak{l}(V_{(\mathbf{C})})$ vào chính nó là $\mathbf{C}$-tuyến tính. Vì $\mathfrak{o}(Q_{(\mathbf{C})})$ thuộc kiểu $B_n$ nếu dim $V = 2n+ 1$, $n\geq 1$, và thuộc kiểu $D_n$ nếu dim $V = 2n,n\geq 3$ (Chương VIII, §13, số 2 và 4), ta suy ra:

#### Mệnh đề 5 {#lie-ix-s3-prop-5 .statement tag=01BD}

Mọi đại số Lie thực đơn compact kiểu $B_n,n\geq 1$ (tương ứng, kiểu $D_n,n\geq 3$) đều đẳng cấu với $\mathfrak{o}(2n+ 1,\mathbf{R})$ (tương ứng, $\mathfrak{o}(2n,\mathbf{R})$).

### 6. CÁC NHÓM COMPACT HẠNG 1

Theo Tôpô đại cương, Chương VIII, §1, no. 4, Mệnh đề 3, Mệnh đề 4 và Nhận xét 4, nhóm tôpô $\mathbf{S}\mathbf{U}(2,\mathbf{C})$ đẳng cấu với nhóm tôpô $\mathbf{S}_3$ các quaternion có chuẩn 1, và thương của $\mathbf{S}\mathbf{U}(2,\mathbf{C})$ bởi nhóm con Z gồm các ma trận $I_2$ và $-I_2$ đẳng cấu với nhóm tôpô $\mathbf{S}\mathbf{O}(3,\mathbf{R})$. Chú ý rằng Z là tâm của $\mathbf{S}\mathbf{U}(2,\mathbf{C}):$ thật vậy, vì $\mathbf{H}=\mathbf{R}.\mathbf{S}_3$, mọi phần tử của tâm của nhóm $\mathbf{S}_3$ đều nằm trong tâm $\mathbf{R}$ của đại số $\mathbf{H}$ và do đó thuộc nhóm có hai phần tử $\mathbf{S}_3\cap \mathbf{R}=\{-1,1\}$.

#### Mệnh đề 6 {#lie-ix-s3-prop-6 .statement tag=01BE}

Mọi đại số Lie thực nửa đơn compact hạng 1 đều đẳng cấu với $\mathfrak{s}\mathfrak{u}(2,\mathbf{C})$ và với $\mathfrak{o}(3,\mathbf{R})$. Mọi nhóm Lie compact liên thông nửa đơn hạng 1 đều đẳng cấu với $\mathbf{S}\mathbf{U}(2,\mathbf{C})$ nếu nó đơn liên, và với $\mathbf{S}\mathbf{O}(3,\mathbf{R})$ nếu không.

Mệnh đề thứ nhất suy ra từ Hệ quả của Mệnh đề 4 và Mệnh đề 5. Vì $\mathbf{S}\mathbf{U}(2,\mathbf{C})$ đồng phôi với $\mathbf{S}_3($Topologie générale, Chap. VIII, §1, no. 4, Nhận xét 4), nên đơn liên (Topologie générale, Chap. XI, sẽ xuất bản), mọi nhóm Lie compact nửa đơn đơn liên hạng 1 đều đẳng cấu với $\mathbf{S}\mathbf{U}(2,\mathbf{C})$; mọi nhóm Lie compact liên thông nửa đơn hạng 1 không đơn liên đều đẳng cấu với một thương của $\mathbf{S}\mathbf{U}(2,\mathbf{C})$ bởi một nhóm con của Z không rút gọn về phần tử đơn vị, do đó đẳng cấu với $\mathbf{S}\mathbf{O}(3,\mathbf{R})$.

#### Nhận xét {#lie-ix-s3-n6-rem-1 .statement tag=01BF}

Ta đã thấy ở trên rằng $\mathbf{S}\mathbf{U}(2,\mathbf{C})$ là đơn liên và $\pi_1(\mathbf{S}\mathbf{O}(3,\mathbf{R}))$ có cấp 2. Ta sẽ thấy muộn hơn nhiều rằng các kết quả này lần lượt được tổng quát hóa cho $\mathbf{S}\mathbf{U}(n,\mathbf{C}) (n\geq 1)$ và $\mathbf{S}\mathbf{O}(n,\mathbf{R}) (n\geq 3)$ (xem thêm §3, Bài tập 4 và 5).

Nhắc lại (Chap. VIII, §1, no. 1) rằng cơ sở chính tắc của $\mathfrak{s}\mathfrak{l}(2,\mathbf{C})$ là cơ sở $(X_+, X_-, H)$, trong đó

$(01)(00)(1$ 0 $)$

$X_+=$ 0 0 $, X_-=-1$ 0 $, H=$ 0 $-1$.

Do đó ta thu được một cơ sở $(U,V,iH)$ của $\mathfrak{su}(2,\mathbf C)$, cũng gọi là chính tắc, bằng cách đặt
$$
U=X_++X_-=
\begin{pmatrix}
0&1\\
-1&0
\end{pmatrix},
\qquad
V=i(X_+-X_-)=
\begin{pmatrix}
0&i\\
i&0
\end{pmatrix},
$$
$$
iH=
\begin{pmatrix}
i&0\\
0&-i
\end{pmatrix}.
$$

Ta có
$$
[iH,U]=2V,\qquad [iH,V]=-2U,\qquad [U,V]=2iH.
\tag{13}
$$

Nếu B ký hiệu dạng Killing của $\mathfrak{su}(2,\mathbf C)$ thì một phép tính ngay lập tức cho
$$
\mathrm{B}(aU+bV+ciH,a'U+b'V+c'iH)=-8(aa'+bb'+cc'),
\tag{14}
$$
nên, nếu ta đồng nhất $\mathfrak{su}(2,\mathbf C)$ với $\mathbf R^3$ bằng cơ sở chính tắc, thì biểu diễn liên hợp của $\mathbf{SU}(2,\mathbf C)$ xác định một đồng cấu $\mathbf{SU}(2,\mathbf C)\to\mathbf{SO}(3,\mathbf R)$ (xem ở trên).

Hơn nữa, chú ý rằng $\mathbf RiH$ là một đại số con Cartan của $\mathfrak{su}(2,\mathbf C)$, rằng xuyến cực đại T của $\mathbf{SU}(2,\mathbf C)$ tương ứng với nó gồm các ma trận đường chéo
$$
\begin{pmatrix}
a&0\\
0&\bar a
\end{pmatrix},
$$
trong đó $a\bar a=1$, và rằng ánh xạ mũ
$$
\exp:\mathbf RiH\longrightarrow T
$$
ánh xạ $xH$, với $x\in\mathbf Ri$, lên ma trận
$$
\begin{pmatrix}
\exp(x)&0\\
0&\exp(-x)
\end{pmatrix},
$$
và do đó có hạt nhân $\mathbf Z.K$, trong đó K là phần tử của $\mathfrak{su}(2,\mathbf C)$ được xác định bởi
$$
K=2\pi iH=
\begin{pmatrix}
2\pi i&0\\
0&-2\pi i
\end{pmatrix}.
\tag{15}
$$

Hơn nữa, tâm của $\mathbf{SU}(2,\mathbf C)$ gồm phần tử đơn vị và $\exp(K/2)$.

Đặt
$$
\theta=
\begin{pmatrix}
0&-1\\
1&0
\end{pmatrix}
\in\mathbf{SU}(2,\mathbf C).
\tag{16}
$$

Theo Chap. VIII, §1, no. 5,
$$
\theta^2=
\begin{pmatrix}
-1&0\\
0&-1
\end{pmatrix},
\qquad
(\mathrm{Int}\,\theta)t=t^{-1},\quad t\in T,
\tag{17}
$$
$$
(\mathrm{Ad}\,\theta)X_+=X_-,
\qquad
(\mathrm{Ad}\,\theta)X_-=X_+,
\qquad
(\mathrm{Ad}\,\theta)U=U,
\qquad
(\mathrm{Ad}\,\theta)V=-V.
\tag{18}
$$

Sau cùng, với $t=
\begin{pmatrix}
a&0\\
0&\bar a
\end{pmatrix}
\in T$, ta có
$$
(\mathrm{Ad}\,t)X_+=a^2X_+,
\qquad
(\mathrm{Ad}\,t)X_-=a^{-2}X_-,
\qquad
(\mathrm{Ad}\,t)H=H,
\tag{19}
$$
$$
(\mathrm{Ad}\,t)U=\mathscr{R}(a^2)U+\mathscr{I}(a^2)V,
\qquad
(\mathrm{Ad}\,t)V=-\mathscr{I}(a^2)U+\mathscr{R}(a^2)V.
\tag{20}
$$

### Bài tập {#lie-ix-s3-exercises}

Xem [các bài tập cho § 3](exercises/s3/).
