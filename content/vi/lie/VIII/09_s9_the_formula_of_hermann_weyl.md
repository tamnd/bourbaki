---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: VIII
chapter_title: SPLIT SEMI-SIMPLE LIE ALGEBRAS
section: 9
section_title: The formula of Hermann Weyl
lang: vi
source: lie-vii-ix
book_pages: 152-159, 253-260
pdf_pages: 0160-0167, 0261-0268
extraction: native
subsections:
    - "no": 1
      title: CHARACTERS OF FINITE DIMENSIONAL $\mathfrak{g}$-MODULES
      page: 152
      pdf_page: 160
    - "no": 2
      title: DIMENSIONS OF SIMPLE $\mathfrak{g}$-MODULES
      page: 154
      pdf_page: 162
    - "no": 3
      title: MULTIPLICITIES OF WEIGHTS OF SIMPLE $\mathfrak{g}$-MODULES
      page: 156
      pdf_page: 164
    - "no": 4
      title: DECOMPOSITION OF TENSOR PRODUCTS OF SIMPLE $\mathfrak{g}$-MODULES
      page: 157
      pdf_page: 165
statements: 12
exercises: 16
content_sha256: f30042d9dbd75a4886a17d4763e34141582b2bbb7f71025613c7ce0facf6d63a
translated_from: content/en/lie/VIII/09_s9_the_formula_of_hermann_weyl.md
source_content_sha256: 16e58934b12a0ac3234fd1dee9446b6558b2edb33a94c1d55bbd2fbd906273b2
translation_model: gpt-5.4
translation_run: translate-vi-34a50c5a
glossary_version: 34
glossary_terms_sha256: f6ed1ec52b177873e1a1d1b599d1f1d8484ab2447646ed87ae97dc86622f4da9
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 9. CÔNG THỨC CỦA HERMANN WEYL

Trong tiết này, ta giữ các ký hiệu tổng quát của §6 và §7.

### 1. CÁC ĐẶC TRƯNG CỦA CÁC $\mathfrak{g}$-MÔĐUN HỮU HẠN CHIỀU

Cho $(e^{\lambda})_{\lambda\in\mathfrak{h}^*}$ là cơ sở chính tắc của vành $\mathbf{Z}[\mathfrak{h}^*]$. Trang bị cho không gian $\mathbf{Z}^{\mathfrak{h}^*}$ của mọi ánh xạ từ $\mathfrak{h}^*$ vào $\mathbf{Z}$ tôpô tích của các tôpô rời rạc trên các thừa số. Nếu $\varphi \in \mathbf{Z}^{\mathfrak{h}^*}$, họ $(\varphi (\nu )e^{\nu})_{\nu\in\mathfrak{h}^*}$ là khả tổng, và

$$
\varphi =\sum_{\nu\in\mathfrak{h}^*}\varphi (\nu )e^{\nu}
$$

Gọi $\mathbf{Z}\langle P\rangle$ là tập hợp các $\varphi \in \mathbf{Z}^{\mathfrak{h}^*}$ mà giá của chúng được chứa trong một hợp hữu hạn các tập hợp có dạng $\nu -P_+$, trong đó $\nu \in \mathfrak{h}^*$. Khi đó $\mathbf{Z}[P]\subset \mathbf{Z}\langle P\rangle  \subset \mathbf{Z}^{\mathfrak{h}^*}$. Định nghĩa trên $\mathbf{Z}\langle P\rangle$ một cấu trúc vành mở rộng cấu trúc của $\mathbf{Z}[P]$ bằng cách đặt, với $\varphi , \psi \in \mathbf{Z}\langle P\rangle$ và $\nu \in \mathfrak{h}^*$,

$$
(\varphi \psi )(\nu ) =\sum_{\mu\in\mathfrak{h}^*}\varphi (\mu)\psi (\nu -\mu)
$$

(họ $(\varphi (\mu)\psi (\nu -\mu))_{\mu\in\mathfrak{h}^*}$ có giá hữu hạn, xét theo điều kiện được thỏa bởi các giá của $\varphi$ và $\psi$). Nếu $\varphi =\sum_{\nu}x_{\nu}e^{\nu}$ và $\psi =\sum_{\nu}y_{\nu}e^{\nu}$, thì $\varphi \psi =\sum_{\nu ,\mu}x_{\nu}y_\mu e^{\nu+\mu}$.

Cho $\nu \in \mathfrak{h}^*$. Một phân hoạch của $\nu$ thành các nghiệm dương là một họ $(n_{\alpha})_{\alpha\in R_+}$, trong đó các $n_{\alpha}$ là các số nguyên $\geq 0$ sao cho $\nu =\sum_{\alpha\in R_+}n_{\alpha}\alpha$. Ta ký hiệu bởi $\mathfrak{P}(\nu )$ số các phân hoạch của $\nu$ thành các nghiệm dương. Ta có

$$
\mathfrak{P}(\nu )>0\Leftarrow \Rightarrow \nu \in Q_+
$$

Trong đoạn này, chúng tôi ký hiệu bởi K phần tử sau của $\mathbf{Z}\langle P\rangle :$

$$
K =\sum_{\gamma\in Q_+}\mathfrak{P}(\gamma )e^{-\gamma}
$$

Bây giờ nhắc lại rằng (Ch. VI, §3, no. 3, Mệnh đề 2)

$$
d=\prod_{\alpha\in R_+}(e^{\alpha /2}-e^{-\alpha /2}) =\sum_{w\in W}\varepsilon (w)e^{w\rho}
$$

là một phần tử phản bất biến của $\mathbf{Z}[P]$.

#### Bổ đề 1 {#lie-viii-s9-lem-1 .statement tag=015T}

Trong vành $\mathbf{Z}\langle P\rangle$, ta có $K.\prod_{\alpha\in R_+}(1-e^{-\alpha}) = Ke^{-\rho}d= 1$.

Thật vậy,

$$
K =\prod_{\alpha\in R_+}(e^0+e^{-\alpha}+e^{-2\alpha}+\cdots )
$$

nên

$$
Ke^{-\rho}d=\prod_{\alpha\in R_+}(1 +e^{-\alpha}+e^{-2\alpha}+\cdots )\prod_{\alpha\in R_+}(1-e^{-\alpha}) = 1
$$

#### Bổ đề 2 {#lie-viii-s9-lem-2 .statement tag=015U}

Cho $\lambda \in \mathfrak{h}^*$. Môđun $Z(\lambda ) ($§6, no. 3) thừa nhận một đặc trưng là một phần tử của $\mathbf{Z}\langle P\rangle$, và ta có $d$. ch $Z(\lambda ) =e^{\lambda+\rho}$.

Cho $\alpha_1, . . . , \alpha_q$ là các phần tử phân biệt của $R_+$. Các $X_{-\alpha_1}^{n_1}X_{-\alpha_2}^{n_2}. . . X_{-\alpha_q}^{n_q}\otimes 1$ tạo thành một cơ sở của $Z(\lambda ) ($§6, Prop. 6 (iii)). Với $h\in \mathfrak{h}$, ta có

$$
h.(X_{-\alpha_1}^{n_1}X_{-\alpha_2}^{n_2}. . .X_{-\alpha_q}^{n_q}\otimes 1)
$$

$$
= [h, X_{-\alpha_1}^{n_1}. . . X_{-\alpha_q}^{n_q}]\otimes 1 + (X_{-\alpha_1}^{n_1}. . . X_{-\alpha_q}^{n_q})\otimes h.1
$$

$$
= (\lambda -n_1\alpha_1- \cdots  -n_q\alpha_q)(h)(X_{-\alpha_1}^{n_1}. . . X_{-\alpha_q}^{n_q}\otimes 1)
$$

Vậy chiều của $Z(\lambda )^{\lambda-\mu}$ là $\mathfrak{P}(\mu)$. Điều này chứng minh rằng ch $Z(\lambda )$ được xác định, là một phần tử của $\mathbf{Z}\langle P\rangle$, và rằng

ch $Z(\lambda ) =\sum_\mu\mathfrak{P}(\mu)e^{\lambda-\mu}= Ke^{\lambda}$.

Bây giờ chỉ còn cần áp dụng Bổ đề 1.

#### Bổ đề 3 {#lie-viii-s9-lem-3 .statement tag=015V}

Cho M là một $\mathfrak{g}$-môđun thừa nhận một đặc trưng ch(M) mà giá đỡ của nó được chứa trong một hợp hữu hạn của các tập hợp $\mu-P_+$. Gọi U là đại số bao của $\mathfrak{g}$, Z là tâm của U$,\lambda_0\in \mathfrak{h}^*$, và $\chi_{\lambda_0}$ là đồng cấu tương ứng từ Z tới $k($§8, Hệ quả 1 của Định lý 2). Giả sử rằng, với mọi $z\in Z,z_M$ là phép vị tự với tỉ số $\chi_{\lambda_0}(z)$. Gọi $D_M$ là tập hợp các $\lambda \in W(\lambda_0+\rho )-\rho$ sao cho $\lambda + Q_+$ cắt Supp(ch M). Khi đó ch(M) là một tổ hợp tuyến tính trên $\mathbf{Z}$ của các ch $Z(\lambda )$ với $\lambda \in D_M$.

Nếu Supp(ch M) là rỗng, bổ đề là hiển nhiên. Giả sử rằng Supp(ch $M$)$\not=\emptyset$. Cho $\lambda$ là một phần tử cực đại của giá này, và đặt dim $M^{\lambda}=m$. Tồn tại một $\mathfrak{g}$-đồng cấu $\varphi$ từ $(Z(\lambda ))^m$ đến M ánh xạ $(Z(\lambda )^{\lambda})^m$ song ánh lên $M^{\lambda}($§6, no. 3, Mệnh đề 6 (i)). Do đó, đặc trưng trung tâm của $Z(\lambda )$ là $\chi_{\lambda_0}$, nên $\lambda \in W(\lambda_0+\rho )-\rho ($§8, no. 5, Hệ quả 1 của Định lý 2). Điều này chứng minh rằng $D_M\not=\emptyset$, và cho phép ta lập luận bằng quy nạp theo Card $D_M$. Gọi L và N là hạt nhân và đối hạt nhân của $\varphi$. Khi đó ta có một dãy khớp các $\mathfrak{g}$-đồng cấu:

$$
0\rightarrow L\rightarrow (Z(\lambda ))^m\rightarrow M\rightarrow N\rightarrow 0
$$

do đó

ch(M) $=-$ch(L) $+m$ ch $Z(\lambda ) +$ ch(N)

(§7, no. 7, công thức (6)). Các tập Supp(ch L) và Supp(ch N) được chứa trong một hợp hữu hạn các tập $\mu-P_+$. Với $z\in Z,z_L$ và $z_N$ là các phép vị tự có tỉ số $\chi_{\lambda_0}(z)$. Rõ ràng, $D_N\subset D_M$. Mặt khác, $(\lambda + Q_+)\cap$Supp(ch $M$) $=\{\lambda \}$, và $\lambda  \notin$ Supp(ch N), nên $\lambda  \notin D_N$ và

Số lượng $D_N<$ số lượng $D_M$.

Mặt khác, L là một môđun con của $(Z(\lambda ))^m$; nếu $\lambda '\in D_L$, thì $\lambda '+ Q_+$ cắt Supp(ch $L$)$\subset$ Supp ch $Z(\lambda )$, nên $\lambda \in \lambda '+ Q_+($§6, no. 1, Prop. 1 (ii)); do đó suy ra $D_L\subset D_M$. Vì $L\cap (Z(\lambda )^{\lambda})^m= 0$, ta có $\lambda  \notin D_L$, nên

Số lượng $D_L<$ số lượng $D_M$.

Bây giờ chỉ còn đủ để áp dụng giả thiết quy nạp.

#### Định lý 1 (Công thức đặc trưng của H. Weyl) {#lie-viii-s9-thm-1 .statement tag=015W}

Cho M là một $\mathfrak{g}$-môđun đơn hữu hạn chiều, và $\lambda$ là trọng số cao nhất của nó. Khi đó

$(\sum_{w\in W}\varepsilon (w)e^{w\rho})$.ch $M =\sum_{w\in W}\varepsilon (w)e^{w(\lambda+\rho)}$.

Với các ký hiệu của Bổ đề 3, đặc trưng trung tâm của M là $\chi_{\lambda}($§6, no. 4, Mệnh đề 7). Do đó, theo các Bổ đề 2 và $3,d$.ch M là một tổ hợp tuyến tính trên $\mathbf{Z}$ của các $e^{\mu+\rho}$ sao cho

$$
\mu+\rho \in W(\lambda +\rho )
$$

Mặt khác, theo §7, no. 7, Bổ đề $7,d$.ch M là phản bất biến, và số hạng cực đại duy nhất của nó là $e^{\lambda+\rho}$, do đó suy ra định lý.

#### Ví dụ {#lie-viii-s9-n1-exa-1 .statement tag=015X}

Lấy $\mathfrak{g}=\mathfrak{s}\mathfrak{l}(2, k),\mathfrak{h}=kH$. Gọi $\alpha$ là nghiệm của $(\mathfrak{g},\mathfrak{h})$ sao cho $\alpha (H) = 2$. $\mathfrak{g}$-môđun $V(m)$ có trọng số cao nhất $(m/2)\alpha$. Do đó

ch(V($m$)) $= (e^{(m/2)\alpha+^1_2\alpha}-e^{-(m/2)\alpha-^1_2\alpha})/(e^{^1_2\alpha}-e^{-^1_2\alpha})$

$$
=e^{-(m/2)\alpha}.(e^{(m+1)\alpha}-1)/(e^{\alpha}-1)
$$

$$
=e^{-(m/2)\alpha}(e^{m\alpha}+e^{(m-1)\alpha}+\cdots + 1)
$$

$$
=e^{(m/2)\alpha}+e^{(m-2)\alpha /2}+\cdots +e^{-(m/2)\alpha}
$$

điều này cũng dễ dàng suy ra từ §1, no. 2, Mệnh đề 2.

### 2. Số chiều của các $\mathfrak{g}$-môđun đơn

Nếu $\mu\in \mathfrak{h}^*$, đặt $J(e^\mu) =\sum_{w\in W}\varepsilon (w)e^{w\mu}$, xem Chương VI, §3, no. 3.

#### Định lý 2 {#lie-viii-s9-thm-2 .statement tag=015Y}

Cho E là một $\mathfrak{g}$-môđun đơn hữu hạn chiều, $\lambda$ là trọng số cao nhất của nó và $(\cdot  | \cdot )$ là một dạng song tuyến tính đối xứng dương, không suy biến, bất biến dưới W trên $\mathfrak{h}^*$. Khi đó:

$$
\prod\langle \lambda +\rho , H_{\alpha}\rangle \prod((\lambda |\alpha ))
$$

dim E = = 1 +.

$$
_{\alpha\in R_+}\langle \rho , H_{\alpha}\rangle_{\alpha\in R_+}\overline{(\rho|\alpha)}
$$

Cho T là một ẩn. Với mọi $\nu \in P$, ký hiệu $f_{\nu}$ là đồng cấu từ $\mathbf{Z}[P]$ vào $\mathbf{R}[[T]]$ biến $e^\mu$ thành $e^{(\nu|\mu)T}$ với mọi $\mu\in P$. Khi đó dim E là số hạng hằng của chuỗi $f_{\nu}$(ch E).

Với mọi $\mu, \nu \in P$, ta có

$$
f_{\nu}(J(e^\mu)) =\sum_{w\in W}\varepsilon (w)e^{(\nu|w\mu)T}
$$

$$
=\sum_{w\in W}\varepsilon (w)e^{(w^{-1}\nu|\mu)T}=f_\mu(J(e^{\nu}))
$$

Đặc biệt, theo Chap. VI, §3, no. 3, công thức (3),

$$
f_{\rho}(J(e^\mu)) =f_\mu(J(e^{\rho})) =e^{(\mu|\rho)T}\prod_{\alpha\in R_+}(1-e^{-(\mu|\alpha)T})
$$

Do đó, đặt Card(R$_+$) $= N$,

$f_{\rho}(J(e^\mu))\equiv T^N\prod_{\alpha\in R}(\mu|\alpha )$ (mod $T^{N+1}\mathbf{R}[[T]]$).

Vì vậy đẳng thức $J(e^{\lambda+\rho}) =$ ch(E)$.J(e^{\rho})$ (Định lý 1) suy ra rằng

$T^N\prod_{\alpha\in R_+}(\lambda +\rho |\alpha )\equiv f_{\rho}$(ch $E$)$.T^N\prod_{\alpha\in R_+}(\rho |\alpha )$ (mod $T^{N+1}\mathbf{R}[[T]]$)

nên

dim $E =((\prod_{\alpha\in R_+}(\lambda +\rho |\alpha ))/((\prod_{\alpha\in R_+}(\rho |\alpha ))=\prod_{\alpha\in R_+}(1 +\frac{(\lambda|\alpha)}{(\rho|\alpha)})$.

Bây giờ, nếu $\alpha \in R_+,\alpha$ được đồng nhất với một phần tử của $\mathfrak{h}_{\mathbf{R}}$ tỉ lệ với $H_{\alpha}$, nên

$$
(\lambda +\rho |\alpha )/(\rho |\alpha ) =\langle \lambda +\rho , H_{\alpha}\rangle /\langle \rho , H_{\alpha}\rangle
$$

#### Ví dụ 1 {#lie-viii-s9-n2-exa-1 .statement tag=015Z}

Trong Ví dụ của no. 1, ta thấy rằng

số chiều $V(m) =(\frac{m}{2}\alpha +\frac{\alpha}{2})(H_{\alpha})/\frac{\alpha}{2}(H_{\alpha}) =m+ 1$,

điều mà ta đã biết ở §1.

#### Ví dụ 2 {#lie-viii-s9-n2-exa-2 .statement tag=0160}

Lấy $\mathfrak{g}$ là đại số Lie đơn phân rã được kiểu $G_2$ và dùng các ký hiệu của Chương VI, Bảng IX. Trang bị cho $\mathfrak{h}^*_{\mathbf{R}}$ dạng đối xứng dương bất biến dưới W $(\cdot  | \cdot )$ sao cho $(\alpha_1|\alpha_1) = 1$. Khi đó $\rho =\varpi_1+\varpi_2$ và

$$
(\varpi_1|\alpha_1) =\frac{1}{2},(\varpi_1|\alpha_2) = 0,(\varpi_1|\alpha_2+\alpha_1) =\frac{1}{2}
$$

$$
(\varpi_1|\alpha_2+ 2\alpha_1) = 1,(\varpi_1|\alpha_2+ 3\alpha_1) =\frac{3}{2},(\varpi_1|2\alpha_2+ 3\alpha_1) =\frac{3}{2}
$$

$$
(\varpi_2|\alpha_1) = 0,(\varpi_2|\alpha_2) =\frac{3}{2},(\varpi_2|\alpha_2+\alpha_1) =\frac{3}{2}
$$

$$
(\varpi_2|\alpha_2+ 2\alpha_1) =\frac{3}{2},(\varpi_2|\alpha_2+ 3\alpha_1) =\frac{3}{2},(\varpi_2|2\alpha_2+ 3\alpha_1) = 3
$$

Do đó, nếu $n_1, n_2$ là các số nguyên $\geq 0$, thì chiều của biểu diễn đơn có trọng số cao nhất $n_1\varpi_1+n_2\varpi_2$ là

$$
(1 +\frac{n_1/2}{1\overline{2}})((1 +\frac{3n_2/2}{3\overline{2}})((1 +\frac{n_1/2 + 3n_2/2}{_{1\overline{2}} + \frac{3}{2}})((1 +\frac{n_1 + 3n_2/2}{1 +^{3\overline{2}}})
$$

$$
\times (1 +\frac{3n_1/2 + 3n_2/2}{_{3\overline{2}} + \frac{3}{2}})((1 +3n_1\frac{/_3}{2}2 + 3+ 3n_2)
$$

$$
= (1 +n_1)(1 +n_2)(1 +\frac{n_1 + 3n_2}{4})((1 +\frac{2n_1 + 3n_2}{5})((1 +\frac{n_1 + n_2}{2})
$$

$$
\times (1 +\frac{n_1 + 2n_2}{3})
$$

$$
(1+n_1)(1+n_2)(2+n_1+n_2)(3+n_1+2n_2)(4+n_1+3n_2)(5+2n_1+3n_2)
$$

=.

5!

Đặc biệt, biểu diễn cơ bản có trọng số cao nhất $\varpi_1$ (tương ứng $\varpi_2$) có chiều bằng 7 (tương ứng 14).

### 3. BỘI SỐ CỦA CÁC TRỌNG SỐ CỦA CÁC $\mathfrak{g}$-MÔĐUN ĐƠN

#### Mệnh đề 1 {#lie-viii-s9-prop-1 .statement tag=0161}

Cho $\omega \in P_{++}$. Với mọi $\lambda \in P$, bội số của $\lambda$ trong $E(\omega )$ là

$$
m_{\lambda}=\sum_{w\in W}\varepsilon (w)\mathfrak{P}(w(\omega +\rho )-(\lambda +\rho ))
$$

Theo Định lý 1 và Bổ đề 1,

ch $E(\omega ) = Ke^{-\rho}d$ ch $E(\omega ) = Ke^{-\rho}\sum_{w\in W}\varepsilon (w)e^{w(\omega+\rho)}$

nên

ch $E(\omega ) =\sum_{w\in W,\gamma\in Q_+}\varepsilon (w)\mathfrak{P}(\gamma )e^{-\rho+w(\omega+\rho)-\gamma}$

và

$$
m_{\lambda}=\sum\varepsilon (w)\mathfrak{P}(\gamma )
$$

$w\in W,\gamma \in Q_+,\gamma =-\lambda -\rho +w(\omega +\rho )$

#### Hệ quả {#lie-viii-s9-n3-cor-1 .statement tag=0162}

Nếu $\lambda$ là một trọng số của $E(\omega )$ phân biệt với $\omega$,

$$
m_{\lambda}=-\sum_{w\in W,w\not=1}\varepsilon (w)m_{\lambda+\rho-w\rho}
$$

Áp dụng Mệnh đề 1 với $\omega = 0$. Nếu $\mu\in P$**--** $\{0\}$, ta thấy rằng

$$
0 =\sum_{w\in W}\varepsilon (w)\mathfrak{P}(w\rho +\mu-\rho )
$$

do đó

$$
\mathfrak{P}(\mu) =-\sum_{w\in W,w\not=1}\varepsilon (w)\mathfrak{P}(\mu+w\rho -\rho ) \tag{1}
$$

Mệnh đề 1 cũng cho

$$
m_{\lambda}=-\sum_{w\in W}\varepsilon (w)\sum_{w'\in W,w'\not=1}\varepsilon (w')\mathfrak{P}(w(\omega +\rho )-(\lambda +\rho ) +w'\rho -\rho )
$$

vì $w(\omega +\rho )\not=\lambda +\rho$ với mọi $w\in W ($§7, Mệnh đề 5 (iii)). Do đó,

$$
m_{\lambda}=-\sum_{w'\in W,w'\not=1}\varepsilon (w')\sum_{w\in W}\varepsilon (w)\mathfrak{P}(w(\omega +\rho )-(\lambda +\rho -w'\rho +\rho ))
$$

$=-\sum_{w'\in W,w'\not=1}\varepsilon (w')m_{\lambda+\rho-w'\rho}$ (Mệnh đề$.1$).

### 4. PHÂN TÍCH CỦA CÁC TÍCH TENXƠ CỦA CÁC $\mathfrak{g}$-MÔĐUN ĐƠN

#### Mệnh đề 2 {#lie-viii-s9-prop-2 .statement tag=0163}

Cho $\lambda , \mu\in P_{++}$. Trong $\mathscr{R}(\mathfrak{g})$, ta có

$$
[\lambda ].[\mu] =\sum_{\nu\in P_{++}}m(\lambda , \mu, \nu )[\nu ]
$$

với

$$
m(\lambda , \mu, \nu ) =\sum_{w,w'\in W}\varepsilon (ww')\mathfrak{P}(w(\lambda +\rho ) +w'(\mu+\rho )-(\nu + 2\rho ))
$$

Cho $E,F$ là các $\mathfrak{g}$-môđun đơn hữu hạn chiều có các trọng số cao nhất $\lambda , \mu$. Gọi $l_{\nu}$ là độ dài của thành phần đẳng kiểu của $E\otimes F$ có trọng số cao nhất $\nu$. Chỉ cần chứng minh rằng

$$
l_{\nu}=\sum_{w,w'\in W}\varepsilon (ww')\mathfrak{P}(w(\lambda +\rho ) +w'(\mu+\rho )-(\nu + 2\rho )) \tag{2}
$$

Đặt $c_1=$ ch(E) $=\sum_{\sigma\in P}m_{\sigma}e^{\sigma},c_2=$ ch(F), và $d= J(e^{\rho})$, trong đó J được định nghĩa như ở no. 2. Ta có $\sum_{\xi\in P_{++}}l_{\xi}$ch[$\xi ] =$ ch(E $\otimes F$) $=c_1c_2$

nên, sau khi nhân với $d$ và dùng Định lý 1,

$$
\sum_{\xi\in P_{++}}l_{\xi}J(e^{\xi+\rho}) =c_1J(e^{\mu+\rho}) =(\sum_{\sigma\in P}m_{\sigma}e^{\sigma})((\sum_{w\in W}\varepsilon (w)e^{w(\mu+\rho)}) \tag{3}
$$

$$
=\sum_{\tau\in P}(\sum_{w\in W}\varepsilon (w)m_{\tau+\rho-w(\mu+\rho)})e^{\tau+\rho}
$$

Bây giờ, nếu $\xi \in P_{++},\xi +\rho$ thuộc buồng được xác định bởi B (Chương VI, §1, no. 10); do đó, với mọi $w\in W$ phân biệt với 1, ta có $w(\xi +\rho )\notin P_{++}$. Do đó, hệ số của $e^{\nu+\rho}$ trong $\sum_{\xi\in P_{++}}l_{\xi}J(e^{\xi+\rho})$ bằng $l_{\nu}$. Xét (3), ta thu được

$$
l_{\nu}=\sum_{w\in W}\varepsilon (w)m_{\nu+\rho-w(\mu+\rho)}
$$

nghĩa là, theo Mệnh đề 1,

$$
l_{\nu}=\sum_{w,w'\in W}\varepsilon (w)\varepsilon (w')\mathfrak{P}(w'(\lambda +\rho )-(\nu +\rho -w(\mu+\rho ) +\rho ))
$$

điều này chứng minh (2).

#### Ví dụ {#lie-viii-s9-n4-exa-1 .statement tag=0164}

Ta trở lại Ví dụ ở no. 1. Cho $\lambda = (n/2)\alpha , \mu= (p/2)\alpha$, $\nu = (q/2)\alpha$ với $n\geq p$. Ta có

$$
m(\lambda , \mu, \nu ) =\mathfrak{P}(\frac{n}{2}\alpha +\frac{\alpha}{2}+\frac{p}{2}\alpha +\frac{\alpha}{2}-\frac{q}{2}\alpha -\alpha )
$$

$$
-\mathfrak{P}(\frac{n}{2}\alpha +\frac{\alpha}{2}-\frac{p}{2}\alpha -\frac{\alpha}{2}-\frac{q}{2}\alpha -\alpha )
$$

$$
-\mathfrak{P}(-\frac{n}{2}\alpha -\frac{\alpha}{2}+\frac{p}{2}\alpha +\frac{\alpha}{2}-\frac{q}{2}\alpha -\alpha )
$$

$$
+\mathfrak{P}(-\frac{n}{2}\alpha -\frac{\alpha}{2}-\frac{p}{2}\alpha -\frac{\alpha}{2}-\frac{q}{2}\alpha -\alpha )
$$

$$
=\mathfrak{P}(\frac{n + p-q}{2}\alpha )-\mathfrak{P}(\frac{n-p-q- 2}{2}\alpha )
$$

Biểu thức này bằng không nếu $n+p+q$ không chia được cho 2, hoặc nếu $q\geq n+p$. Nếu

$$
q=n+p-2r
$$

với $r$ là một số nguyên $\geq 0$, ta có

$$
m(\lambda , \mu, \nu ) =\mathfrak{P}(r\alpha )-\mathfrak{P}((r-p-1)\alpha )
$$

do đó $m(\lambda , \mu, \nu ) = 1$ nếu $r\leq p$ và $m(\lambda , \mu, \nu ) = 0$ nếu $r > p$. Cuối cùng, $\mathfrak{g}$-môđun $V(n)\otimes V(p)$ đẳng cấu với

$$
V(n+p)\oplus V(n+p-2)\oplus V(n+p-4)\oplus  \cdots  \oplus V(n-p)
$$

(công thức Clebsch-Gordan).

### Bài tập {#lie-viii-s9-exercises}

Mọi $\mathfrak{g}$-môđun được xét đều được giả thiết là hữu hạn chiều.

Xem [các bài tập của § 9](exercises/s9/).
