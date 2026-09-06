---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: VII
chapter_title: CARTAN SUBALGEBRAS AND REGULAR ELEMENTS
section: 3
section_title: Conjugacy theorems
lang: vi
source: lie-vii-ix
book_pages: 20-27, 57-62
pdf_pages: 0030-0037, 0066-0071
extraction: native
subsections:
    - "no": 1
      title: ELEMENTARY AUTOMORPHISMS
      page: 20
      pdf_page: 30
    - "no": 2
      title: CONJUGACY OF CARTAN SUBALGEBRAS
      page: 22
      pdf_page: 32
    - "no": 3
      title: APPLICATIONS OF CONJUGACY
      page: 24
      pdf_page: 34
    - "no": 4
      title: CONJUGACY OF CARTAN SUBALGEBRAS OF SOLVABLE LIE ALGEBRAS
      page: 25
      pdf_page: 35
    - "no": 5
      title: LIE GROUP CASE
      page: 26
      pdf_page: 36
statements: 17
exercises: 18
content_sha256: 7954d9b116c2b536ab847e56bcbbc599fadec8e28f4f1efcad7cf73e04330bd3
translated_from: content/en/lie/VII/03_s3_conjugacy_theorems.md
source_content_sha256: 101d1c917bccf9d451ef36bc325751d7276a14c534bc85fbe7012cad2e06164a
translation_model: gpt-5-6-mini
translation_run: translate-vi-67073b9f
glossary_version: 34
glossary_terms_sha256: d276d52c73fb14438fbbf062c28254a02e546e62375ee51c069220aad4069db7
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 3. CÁC ĐỊNH LÝ LIÊN HỢP

Trong đoạn này, trường cơ sở $k$ có đặc số 0.

### 1. CÁC TỰ ĐẲNG CẤU SƠ CẤP

Cho $\mathfrak{g}$ là một đại số Lie. Ký hiệu nhóm các tự đẳng cấu của nó là Aut($\mathfrak{g}$). Nếu $x\in \mathfrak{g}$ và ad $x$ là lũy linh, thì $e^{adx}\in$ Aut($\mathfrak{g}$) (Chap. I, §6, no. 8).

#### Định nghĩa 1 {#lie-vii-s3-def-1 .statement tag=00V0}

Một tích hữu hạn các tự đẳng cấu của $\mathfrak{g}$ có dạng $e^{adx}$ với ad $x$ lũy linh được gọi là một tự đẳng cấu sơ cấp của $\mathfrak{g}$. Nhóm các tự đẳng cấu sơ cấp của $\mathfrak{g}$ được ký hiệu bởi Aut$_e(\mathfrak{g})$.

Nếu $u\in$ Aut($\mathfrak{g}$)$,ue^{adx}u^{-1}=e^{adu(x)}$. Suy ra rằng Aut$_e(\mathfrak{g})$ là một nhóm con chuẩn của Aut($\mathfrak{g}$). Nếu $k=\mathbf{R}$ hoặc $\mathbf{C}$, Aut$_e(\mathfrak{g})$ được chứa trong nhóm Int($\mathfrak{g}$) các tự đẳng cấu nội của $\mathfrak{g}$ (Chap. III, §6, no. 2, Định. 2).

$^*$ Trong trường hợp tổng quát, Aut$_e(\mathfrak{g})$ được chứa trong thành phần đơn vị của nhóm đại số Aut($\mathfrak{g}$)$._*$

#### Bổ đề 1 {#lie-vii-s3-lem-1 .statement tag=00V1}

Cho V là một không gian vectơ hữu hạn chiều, $\mathfrak{n}$ là một đại số con Lie của $\mathfrak{a}=\mathfrak{g}\mathfrak{l}(V)$ gồm các phần tử lũy linh.

(i) Ánh xạ $x \rightarrow$ exp $x$ là một song ánh từ $\mathfrak{n}$ lên một nhóm con N của $\mathbf{G}\mathbf{L}(V)$ gồm các phần tử lũy đơn (Chap. II, §6, no. 1, Nhận xét 4). Ta có $\mathfrak{n}=$ log(exp$\mathfrak{n}$). Ánh xạ $f \rightarrow f\circ$ log là một đẳng cấu từ đại số các hàm đa thức trên $\mathfrak{n}$ vào đại số các hạn chế lên N của các hàm đa thức trên End(V).

(ii) Nếu $x\in \mathfrak{n}$ và $a\in \mathfrak{a}$,

(exp ad$_{\mathfrak{a}}x$)$.a=$ (exp $x$)$a$(exp($-x$)).

(iii) Cho $V'$ là một không gian vectơ hữu hạn chiều, $\mathfrak{n}'$ là một đại số con Lie của $\mathfrak{g}\mathfrak{l}(V')$ gồm các phần tử lũy linh, $\rho$ là một đồng cấu từ $\mathfrak{n}$ đến $\mathfrak{n}'$. Cho $\pi$ là ánh xạ exp $x \rightarrow$ exp $\rho (x)$ từ exp$\mathfrak{n}$ đến exp$\mathfrak{n}'$. Khi đó $\pi$ là một đồng cấu nhóm.

Theo định lý Engel, ta có thể đồng nhất V với $k^n$ theo cách sao cho $\mathfrak{n}$ là một đại số con của $\mathfrak{n}(n, k)$ (đại số con Lie của $\mathbf{M}_n(k)$ gồm các ma trận tam giác dưới với các số không trên đường chéo). Với $s\geq 0$, gọi $\mathfrak{n}_s(n, k)$ là tập hợp của $(x_{ij})_{1\leq i,j\leq n}\in \mathbf{M}_n(k)$ sao cho $x_{ij}= 0$ với $i-j < s$. Khi đó

$$
[\mathfrak{n}_s(n, k),\mathfrak{n}_{s'}(n, k)]\subset \mathfrak{n}_{s+s'}(n, k)
$$

(Chương II, §4, no. 6, Nhận xét), và chuỗi Hausdorff xác định một ánh xạ đa thức $(a, b) \rightarrow H(a, b)$ từ $\mathfrak{n}(n, k)\times \mathfrak{n}(n, k)$ vào $\mathfrak{n}(n, k)$ (Chương II, §6, no. 5, Nhận xét 3); ánh xạ này biến $\mathfrak{n}(n, k)$ thành một nhóm (Chương II, §6, no. 5, Mệnh đề 4). Theo Chương II, §6, no. 1, Nhận xét 4, các ánh xạ $x \rightarrow$ exp $x$ từ $\mathfrak{n}(n, k)$ vào $1 +\mathfrak{n}(n, k)$ và $y \rightarrow$ log $y$ từ $1 +\mathfrak{n}(n, k)$ vào $\mathfrak{n}(n, k)$ là các song ánh nghịch đảo và là đa thức; theo Chương II, §6, no. 5, Mệnh đề 3, các ánh xạ này là các đẳng cấu nhóm nếu $\mathfrak{n}(n, k)$ được trang bị luật nhóm $(a, b) \rightarrow H(a, b)$ và nếu $1 +\mathfrak{n}(n, k)$ được xem như một nhóm con của $\mathbf{G}\mathbf{L}_n(k)$. Các khẳng định (i) và (iii) của bổ đề suy ra ngay. Cho $x\in \mathfrak{n}$. Ký hiệu $L_x,R_x$ là các ánh xạ $u \rightarrow xu, u \rightarrow ux$ từ $\mathfrak{a}$ vào $\mathfrak{a}$, giao hoán với nhau và lũy linh. Ta có ad$_{\mathfrak{a}}x= L_x-R_x$, do đó, với mọi $a\in \mathfrak{a}$,

(exp ad$_{\mathfrak{a}}x$)$a=$ (exp(L$_x-R_x$))$a=$ (exp $L_x$)(exp $R_{-x}$)$a$ (1)

$=\sum Li^{ix}$! $Rj\overset{j-x}{!}a=$ (exp $x$)$a$(exp($-x$)).

$i,j\geq 0$

Với ký hiệu trong Bổ đề $1,\pi$ được gọi là biểu diễn tuyến tính của exp $\mathfrak{n}$ tương thích với biểu diễn đã cho $\rho$ của $\mathfrak{n}$ trên $V'$. Khi $k$ là $\mathbf{R}$, $\mathbf{C}$, hoặc một trường ultrametric đầy đủ không rời rạc, $\rho = L(\pi )$ theo các tính chất của các ánh xạ mũ (Chương III, §4, no. 4, Hệ quả 2 của Mệnh đề 8).

#### Mệnh đề 1 {#lie-vii-s3-prop-1 .statement tag=00V2}

Cho $\mathfrak{g}$ là một đại số Lie, $\mathfrak{n}$ là một đại số con của $\mathfrak{g}$ sao cho ad$_{\mathfrak{g}}x$ là lũy linh với mọi $x\in \mathfrak{n}$. Khi đó $e^{ad_{\mathfrak{g}}\mathfrak{n}}$ là một nhóm con của Aut$_e(\mathfrak{g})$.

Điều này suy ra ngay lập tức từ Bổ đề 1 (i).

Đặc biệt, nếu $\mathfrak{n}$ là căn lũy linh của $\mathfrak{g},e^{ad_{\mathfrak{g}}\mathfrak{n}}$ là nhóm các tự đẳng cấu đặc biệt của $\mathfrak{g}$ (Chap. I, §6, no. 8, Định. 6).

#### Nhận xét 1 {#lie-vii-s3-n1-rem-1 .statement tag=00V3}

Cho V là một không gian vectơ hữu hạn chiều, $\mathfrak{g}$ là một đại số con Lie của $\mathfrak{a}=\mathfrak{g}\mathfrak{l}$(V), $x$ là một phần tử của $\mathfrak{g}$ sao cho ad$_{\mathfrak{g}}x$ là lũy linh. Khi đó tồn tại một phần tử lũy linh $n$ của $\mathfrak{a}$ sao cho ad$_{\mathfrak{a}}n$ mở rộng ad$_{\mathfrak{g}}x$. Thật vậy, gọi $s, n$ là các thành phần nửa đơn và lũy linh của $x$; khi đó ad$_{\mathfrak{a}}s$ và ad$_{\mathfrak{a}}n$ là các thành phần nửa đơn và lũy linh của ad$_{\mathfrak{a}}x$ (Chap. I, §5, no. 4, Bổ đề 2), do đó ad$_{\mathfrak{a}}s$ và ad$_{\mathfrak{a}}n$ giữ $\mathfrak{g}$ ổn định, và ad$_{\mathfrak{a}}s|\mathfrak{g}$ và ad$_{\mathfrak{a}}n|\mathfrak{g}$ là các thành phần nửa đơn và lũy linh của ad$_{\mathfrak{g}}x$; do đó, ad$_{\mathfrak{g}}x=$ ad$_{\mathfrak{a}}n|\mathfrak{g}$, điều này chứng minh mệnh đề của chúng ta. Theo Bổ đề 1 (ii), mọi tự đẳng cấu sơ cấp của $\mathfrak{g}$ mở rộng thành một tự đẳng cấu của $\mathfrak{a}$ có dạng $u \rightarrow mum^{-1}$ trong đó $m\in \mathbf{G}\mathbf{L}(V)$.

#### Nhận xét 2 {#lie-vii-s3-n1-rem-2 .statement tag=00V4}

Cho V là một không gian vectơ hữu hạn chiều. Với mọi $g\in \mathbf{S}\mathbf{L}$(V), gọi $\varphi (g)$ là tự đẳng cấu $x \rightarrow gxg^{-1}$ của $\mathfrak{g}\mathfrak{l}(V)$. Khi đó

Aut$_e(\mathfrak{g}\mathfrak{l}(V)) =\varphi (\mathbf{S}\mathbf{L}(V))$.

Thật vậy, theo (1), Aut$_e(\mathfrak{g}\mathfrak{l}(V))$ được chứa trong $\varphi (\mathbf{S}\mathbf{L}$(V)), và bao hàm ngược lại suy ra từ Đại số, Chap. III, §8, no. 9, Mệnh đề 17 và (1). Một lập luận tương tự chỉ ra rằng Aut$_e(\mathfrak{s}\mathfrak{l}(V))$ là tập hợp các hạn chế của các phần tử của $\varphi (\mathbf{S}\mathbf{L}(V))$ lên $\mathfrak{s}\mathfrak{l}(V)$.

### 2. SỰ LIÊN HỢP CỦA CÁC ĐẠI SỐ CON CARTAN

Cho $\mathfrak{g}$ là một đại số Lie, $\mathfrak{h}$ là một đại số con lũy linh của $\mathfrak{g}$ và R là tập hợp các trọng khác không của $\mathfrak{h}$ trong $\mathfrak{g}$, nói cách khác là tập hợp các dạng tuyến tính $\lambda \not= 0$ trên $\mathfrak{h}$ sao cho $\mathfrak{g}^{\lambda}(\mathfrak{h})\not= 0$, cf. §1, no. 3, Mệnh đề 9 (iii). Giả sử rằng

$$
\mathfrak{g}=\mathfrak{g}^0(\mathfrak{h})\oplus \sum_{\lambda\in R}\mathfrak{g}^{\lambda}(\mathfrak{h})
$$

trong trường hợp đó nếu $k$ đóng đại số (§1, no. 3, Mệnh đề 9 (i)). Với $\lambda \in R$ và $x\in \mathfrak{g}^{\lambda}(\mathfrak{h})$, ad $x$ là lũy linh (§1, no. 3, Mệnh đề 10 (iv)). Ký hiệu $E(\mathfrak{h})$ là nhóm con của Aut$_e(\mathfrak{g})$ sinh bởi các $e^{adx}$ trong đó $x$ có dạng trên. Nếu $u\in$ Aut($\mathfrak{g}$), ta thấy ngay lập tức rằng $uE(\mathfrak{h})u^{-1}= E(u(\mathfrak{h}))$.

#### Bổ đề 2 {#lie-vii-s3-lem-2 .statement tag=00V5}

(i) Gọi $\mathfrak{h}_r$ là tập hợp các $x\in \mathfrak{h}$ sao cho $\mathfrak{g}^0(x) =\mathfrak{g}^0(\mathfrak{h})$; đây là tập hợp các $x\in \mathfrak{h}$ sao cho $\lambda (x)\not= 0$ với mọi $\lambda \in R$, và $\mathfrak{h}_r$ là mở và trù mật trong $\mathfrak{h}$ đối với tôpô Zariski.

(ii) Đặt $R =\{\lambda_1, \lambda_2, . . . , \lambda_p\}$ trong đó các $\lambda_i$ đôi một phân biệt. Gọi F là ánh xạ từ $\mathfrak{g}^0(\mathfrak{h})\times \mathfrak{g}^{\lambda_1}(\mathfrak{h})\times  \cdots  \times \mathfrak{g}^{\lambda_p}(\mathfrak{h})$ vào $\mathfrak{g}$ được xác định bởi công thức

$$
F(h, x_1, . . . , x_p) =e^{adx_1}. . . e^{adx_p}h
$$

Khi đó F là một ánh xạ đa thức trội (Phụ lục I).

Khẳng định (i) là rõ ràng. Ta chứng minh (ii). Đặt $n=$ dim $\mathfrak{g}$. Nếu $\lambda \in R$ và $x\in \mathfrak{g}^{\lambda}(\mathfrak{h})$, ta có (ad $x$)$^n= 0$. Suy ra rằng $(y, x) \rightarrow e^{adx}y$ là một ánh xạ đa thức từ $\mathfrak{g}\times \mathfrak{g}^{\lambda}(\mathfrak{h})$ vào $\mathfrak{g}$; bằng quy nạp suy ra rằng F là đa thức. Cho $h_0\in \mathfrak{h}_r$ và gọi DF là ánh xạ tuyến tính tiếp xúc của F tại $(h_0,0, . . . ,0)$; ta chứng minh rằng DF là toàn ánh. Với $h\in \mathfrak{g}^0(\mathfrak{h}), F(h_0+h,0, . . . ,0) =h_0+h$, do đó DF($h,0, . . . ,0$) $=h$ và Im(DF) $\supset \mathfrak{g}^0(\mathfrak{h})$. Mặt khác, với $x\in \mathfrak{g}^{\lambda_1}(\mathfrak{h})$,

$F(h_0, x,0, . . . ,0) =e^{adx}h_0=h_0+$ (ad $x$)$.h_0+$ (ad2!$x$)$^2h_0+\cdots$

do đó DF(0$, x,0, . . . ,0$) $=$ (ad $x$)$.h_0=-$(ad $h_0$)$x$; vì ad $h_0$ sinh ra một tự đẳng cấu của $\mathfrak{g}^{\lambda_1}(\mathfrak{h})$, Im(DF) $\supset \mathfrak{g}^{\lambda_1}(\mathfrak{h})$. Tương tự,

Im(DF) $\supset \mathfrak{g}^{\lambda_i}(\mathfrak{h})$

với mọi $i$, do đó DF là toàn ánh. Mệnh đề 4 của Phụ lục I bây giờ cho thấy rằng F là trội.

#### Mệnh đề 2 {#lie-vii-s3-prop-2 .statement tag=00V6}

Giả sử $k$ đóng đại số. Cho $\mathfrak{g}$ là một đại số Lie, $\mathfrak{h}$ và $\mathfrak{h}'$ là các đại số con Cartan của $\mathfrak{g}$. Tồn tại $u\in E(\mathfrak{h})$ và $u'\in E(\mathfrak{h}')$ sao cho $u(\mathfrak{h}) =u'(\mathfrak{h}')$.

Ta giữ lại ký hiệu của Bổ đề 2. Từ sự kiện rằng $\mathfrak{h}$ và $\mathfrak{h}'$ là các đại số con Cartan, suy ra $\mathfrak{g}^0(\mathfrak{h}) =\mathfrak{h}$ và $\mathfrak{g}^0(\mathfrak{h}') =\mathfrak{h}'$. Theo Bổ đề 2 và Mệnh đề 3 của Phụ lục $I, E(\mathfrak{h})\mathfrak{h}_r$ và $E(\mathfrak{h}')\mathfrak{h}'_r$ chứa các tập hợp mở trù mật của $\mathfrak{g}$ trong tôpô Zariski. Do đó $E(\mathfrak{h})\mathfrak{h}_r\cap E(\mathfrak{h}')\mathfrak{h}'_r\not=\emptyset$. Nói cách khác, tồn tại $u\in E(\mathfrak{h}), u'\in E(\mathfrak{h}'), h\in \mathfrak{h}_r, h'\in \mathfrak{h}'_r$ sao cho $u(h) =u'(h')$; khi đó

$$
u(\mathfrak{h}) =u(\mathfrak{g}^0(\mathfrak{h})) =\mathfrak{g}^0(u(h)) =\mathfrak{g}^0(u'(h')) =u'(\mathfrak{h}')
$$

#### Hệ quả {#lie-vii-s3-n2-cor-1 .statement tag=00V7}

$E(\mathfrak{h}) = E(\mathfrak{h}')$.

Cho $u, u'$ như trong Mệnh đề 2. Khi đó

$$
E(\mathfrak{h}) =uE(\mathfrak{h})u^{-1}= E(u(\mathfrak{h})) = E(u'(\mathfrak{h}')) =u'E(\mathfrak{h}')u^{'-1}= E(\mathfrak{h}')
$$

suy ra hệ quả.

Do kết quả này, nếu $k$ đóng đại số, ta sẽ ký hiệu đơn giản bởi E nhóm $E(\mathfrak{h})$, trong đó $\mathfrak{h}$ là một đại số con Cartan của $\mathfrak{g}$.

Nói chung, Aut$_e(\mathfrak{g})\not= E$ (ví dụ, nếu $\mathfrak{g}$ lũy linh, E thu gọn thành phần tử đơn vị, mặc dù các tự đẳng cấu sơ cấp không tầm thường tồn tại với điều kiện $\mathfrak{g}$ không giao hoán). Tuy nhiên, có thể chứng minh được (Chương VIII, §10, Bài tập 5) rằng Aut$_e(\mathfrak{g}) = E$ đối với $\mathfrak{g}$ nửa đơn.

#### Định lý 1 {#lie-vii-s3-thm-1 .statement tag=00V8}

Giả sử rằng $k$ đóng đại số. Cho $\mathfrak{g}$ là một đại số Lie. Nhóm E là chuẩn tắc trong Aut($\mathfrak{g}$) và tác động bắc cầu trên tập hợp các đại số con Cartan của $\mathfrak{g}$.

Cho $\mathfrak{h}$ là một đại số con Cartan của $\mathfrak{g}$, và $v\in$ Aut($\mathfrak{g}$). Khi đó

$$
vE(\mathfrak{h})v^{-1}= E(v(\mathfrak{h})) = E(\mathfrak{h})
$$

do đó $E(\mathfrak{h}) = E$ là chuẩn tắc trong Aut($\mathfrak{g}$). Nếu $\mathfrak{h}'$ là một đại số con Cartan khác của $\mathfrak{g}$, thì, theo ký hiệu của Mệnh đề $2,u^{'-1}u(\mathfrak{h}) =\mathfrak{h}'$, và $u^{'-1}u\in E$.

### 3. CÁC ỨNG DỤNG CỦA SỰ LIÊN HỢP

#### Định lý 2 {#lie-vii-s3-thm-2 .statement tag=00V9}

Cho $\mathfrak{g}$ là một đại số Lie.

(i) Các đại số con Cartan của $\mathfrak{g}$ đều có cùng chiều, cụ thể là rk($\mathfrak{g}$), và cùng lớp lũy linh.

(ii) Một phần tử $x\in \mathfrak{g}$ là chính quy khi và chỉ khi $\mathfrak{g}^0(x)$ là một đại số con Cartan của $\mathfrak{g}$; mọi đại số con Cartan đều thu được theo cách này.

Để chứng minh (i), ta có thể giả sử rằng $k$ đóng đại số (xem §2, Mệnh đề 3 và Mệnh đề 6), trong trường hợp đó điều này suy ra từ Định lý 1 của no. 2. Mệnh đề (ii) suy ra từ (i) và §2, Định lý 1 (i) và (iv).

#### Mệnh đề 3 {#lie-vii-s3-prop-3 .statement tag=00VA}

Cho $\mathfrak{g}$ là một đại số Lie, $\mathfrak{g}'$ là một đại số con của $\mathfrak{g}$. Các điều kiện sau là tương đương:

(i) $\mathfrak{g}'$ chứa một phần tử chính quy của $\mathfrak{g}$, và rk($\mathfrak{g}$) $=$ rk($\mathfrak{g}'$);

(ii) $\mathfrak{g}'$ chứa một đại số con Cartan của $\mathfrak{g}$;

(iii) mọi đại số con Cartan của $\mathfrak{g}'$ đều là một đại số con Cartan của $\mathfrak{g}$.

(i) $=\Rightarrow$ (ii): Giả sử rằng rk($\mathfrak{g}$) $=$ rk($\mathfrak{g}'$), và tồn tại $x\in \mathfrak{g}'$ chính quy trong $\mathfrak{g}$. Đặt $\mathfrak{h}=\mathfrak{g}^0(x),\mathfrak{h}'={\mathfrak{g}'}^0(x) =\mathfrak{h}\cap \mathfrak{g}'$. Khi đó

rk($\mathfrak{g}'$)$\leq$ dim$\mathfrak{h}'\leq$ dim$\mathfrak{h}=$ rk($\mathfrak{g}$) $=$ rk($\mathfrak{g}'$)

suy ra $\mathfrak{h}=\mathfrak{h}'\subset \mathfrak{g}'$. Điều này chứng minh (ii).

(ii) $=\Rightarrow$ (iii): Giả sử rằng $\mathfrak{g}'$ chứa một đại số con Cartan $\mathfrak{h}$ của $\mathfrak{g}$, và gọi $\mathfrak{h}_1$ là một đại số con Cartan của $\mathfrak{g}'$. Để chứng minh rằng $\mathfrak{h}_1$ là một đại số con Cartan của $\mathfrak{g}$, ta có thể giả sử rằng $k$ là đóng đại số. Gọi $E(\mathfrak{h})$ và $E'(\mathfrak{h})$ là các nhóm tự đẳng cấu của $\mathfrak{g}$ và $\mathfrak{g}'$ liên kết với $\mathfrak{h}$ (no. 2). Theo Định lý 1, tồn tại $f\in E'(\mathfrak{h})$ sao cho $f(\mathfrak{h}) =\mathfrak{h}_1$. Bây giờ mọi phần tử của $E'(\mathfrak{h})$ đều được cảm sinh bởi một phần tử của $E(\mathfrak{h})$; thật vậy, chỉ cần kiểm tra điều này đối với $e^{adx}$, với $x\in {\mathfrak{g}'}^{\lambda}(\mathfrak{h}),\lambda \not= 0$, trong trường hợp này điều đó suy ra từ phép bao hàm ${\mathfrak{g}'}^{\lambda}(\mathfrak{h})\subset \mathfrak{g}^{\lambda}(\mathfrak{h})$. Do đó $\mathfrak{h}_1$ là một đại số con Cartan của $\mathfrak{g}$.

(iii) $=\Rightarrow$ (i): Giả sử rằng điều kiện (iii) được thỏa mãn. Gọi $\mathfrak{h}$ là một đại số con Cartan của $\mathfrak{g}'$. Vì đây là một đại số con Cartan của $\mathfrak{g}$, nó chứa một phần tử chính quy của $\mathfrak{g}$ (Định lý 2 (ii)), và mặt khác rk($\mathfrak{g}$) $=$ dim($\mathfrak{h}$) $=$ rk($\mathfrak{g}'$).

#### Hệ quả {#lie-vii-s3-n3-cor-1 .statement tag=00VB}

Cho $\mathfrak{h}$ là một đại số con lũy linh của $\mathfrak{g}$. Đại số con $\mathfrak{g}^0(\mathfrak{h})$ có các tính chất (i), (ii), (iii) trong Mệnh đề 3.

Thật vậy, Mệnh đề 11 của §2, no. 3, chỉ ra rằng $\mathfrak{g}^0(\mathfrak{h})$ có tính chất (ii).

#### Mệnh đề 4 {#lie-vii-s3-prop-4 .statement tag=00VC}

Cho $\mathfrak{g}$ là một đại số Lie, $l$ là hạng của $\mathfrak{g},c$ là lớp lũy linh của các đại số con Cartan của $\mathfrak{g}$, và $x\in \mathfrak{g}$. Tồn tại một đại số con $l$-chiều của $\mathfrak{g}$ có lớp lũy linh $\leq c$ và chứa $x$.

Cho T là một phần tử bất định. Đặt $k'=k(T)$ và $\mathfrak{g}'=\mathfrak{g}\otimes_kk'$. Nếu $\mathfrak{h}$ là một đại số con Cartan của $\mathfrak{g},\mathfrak{h}\otimes_kk'$ là một đại số con Cartan của $\mathfrak{g}'$, do đó hạng của $\mathfrak{g}'$ là $l$ và lớp lũy linh của các đại số con Cartan của $\mathfrak{g}'$ là $c$.

Chọn một phần tử chính quy $y$ của $\mathfrak{g}$. Với các ký hiệu của §2, no. 2, ta có $a_l(y)\not= 0$. Ký hiệu cũng bởi $a_l$ hàm đa thức trên $\mathfrak{g}'$ mở rộng $a_l$. Khi đó phần tử $a_l(x+ Ty)$ của $k[T]$ có hệ số trội $a_l(y)$. Đặc biệt, $x+ Ty$ là chính quy trong $\mathfrak{g}'$. Gọi $\mathfrak{h}'$ là không gian linh của ad($x+ Ty$) trong $\mathfrak{g}'$. Khi đó chiều $\mathfrak{h}'=l$ và lớp lũy linh của $\mathfrak{h}'$ là $c$. Đặt $\mathfrak{k}=\mathfrak{h}'\cap (\mathfrak{g}\otimes_kk[T])$; khi đó $\mathfrak{k}\otimes_{k[T]}k(T) =\mathfrak{h}'$.

Cho $\varphi$ là đồng cấu từ $k[T]$ đến $k$ sao cho $\varphi (T) = 0$, và cho $\psi$ là đồng cấu $1\otimes \varphi$ từ $\mathfrak{g}\otimes_kk[T]$ đến $\mathfrak{g}$. Khi đó $\psi (\mathfrak{k})$ là một đại số con của $\mathfrak{g}$ có lớp lũy linh $\leq c$ và chứa $\psi (x+ Ty) =x$.

Trong môđun $k$[T]-tự do $\mathfrak{g}\otimes_kk[T],\mathfrak{k}$ là một môđun con có hạng $l$, và $(\mathfrak{g}\otimes_kk[T])/\mathfrak{k}$ là xoắn tự do, do đó môđun con $\mathfrak{k}$ là một tổng hạng trực tiếp của $\mathfrak{g}\otimes_kk[T] ($Đại số, Chap. VII, §4, no. 2, Th. 1). Vì vậy chiều$_k\psi (\mathfrak{k}) =l$, điều này hoàn tất chứng minh.

### 4. Sự liên hợp của các đại số con Cartan của các đại số Lie giải được

Cho $\mathfrak{g}$ là một đại số Lie giải được. Ký hiệu $\mathscr{C}^{\infty}(\mathfrak{g})$ là giao của các số hạng của chuỗi trung tâm giảm dần của $\mathfrak{g}$ (Chương I, §1, no. 5). Đây là một iđêan đặc số của $\mathfrak{g}$, và là iđêan nhỏ nhất $\mathfrak{m}$ của $\mathfrak{g}$ sao cho $\mathfrak{g}/\mathfrak{m}$ là lũy linh. Vì $\mathscr{C}^{\infty}(\mathfrak{g})\subset [\mathfrak{g},\mathfrak{g}],\mathscr{C}^{\infty}(\mathfrak{g})$ là một iđêan lũy linh của $\mathfrak{g}$ (Chương I, §5, no. 3, Hệ quả 5 của Định lý 1). Theo Mệnh đề 1 của no. 1, tập hợp của $e^{adx}$, với $x\in \mathscr{C}^{\infty}(\mathfrak{g})$, là một nhóm con của Aut($\mathfrak{g}$) được chứa trong nhóm các tự đẳng cấu đặc biệt (Chương I, §6, no. 8, Định nghĩa 6).

#### Định lý 3 {#lie-vii-s3-thm-3 .statement tag=00VD}

Cho $\mathfrak{g}$ là một đại số Lie giải được, và cho $\mathfrak{h},\mathfrak{h}'$ là các đại số con Cartan của $\mathfrak{g}$. Tồn tại $x\in \mathscr{C}^{\infty}(\mathfrak{g})$ sao cho $e^{adx}\mathfrak{h}=\mathfrak{h}'$.

Ta lập luận bằng quy nạp theo dim$\mathfrak{g}$, trường hợp $\mathfrak{g}= 0$ là tầm thường. Cho $\mathfrak{n}$ là một iđêan giao hoán cực tiểu khác không của $\mathfrak{g}$. Cho $\varphi :\mathfrak{g}\rightarrow \mathfrak{g}/\mathfrak{n}$ là cấu xạ chính tắc. Khi đó $\varphi (\mathscr{C}^{\infty}\mathfrak{g}) =\mathscr{C}^{\infty}(\mathfrak{g}/\mathfrak{n})$ (Chương I, §1, no. 5, Mệnh đề 4). Vì $\varphi (\mathfrak{h})$ và $\varphi (\mathfrak{h}')$ là các đại số con Cartan của $\mathfrak{g}/\mathfrak{n}($§2, no. 1, Hệ quả 2 của Mệnh đề 4), nên tồn tại, theo giả thiết quy nạp, một $x\in \mathscr{C}^{\infty}(\mathfrak{g})$ sao cho $e^{ad\varphi(x)}\varphi (\mathfrak{h}) =\varphi (\mathfrak{h}')$. Thay thế $\mathfrak{h}$ bởi $e^{adx}\mathfrak{h}$, ta có thể giả sử rằng $\varphi (\mathfrak{h}) =\varphi (\mathfrak{h}')$, nói cách khác rằng

$$
\mathfrak{h}+\mathfrak{n}=\mathfrak{h}'+\mathfrak{n}
$$

Khi đó $\mathfrak{h}$ và $\mathfrak{h}'$ là các đại số con Cartan của $\mathfrak{h}+\mathfrak{n}$. Nếu $\mathfrak{h}+\mathfrak{n}\not=\mathfrak{g}$, mệnh đề cần chứng minh suy ra từ giả thiết quy nạp. Từ nay giả sử rằng $\mathfrak{h}+\mathfrak{n}=\mathfrak{h}'+\mathfrak{n}=\mathfrak{g}$.

Do tính cực tiểu của $\mathfrak{n}, [\mathfrak{g},\mathfrak{n}] =\{0\}$ hoặc $[\mathfrak{g},\mathfrak{n}] =\mathfrak{n}$. Nếu $[\mathfrak{g},\mathfrak{n}] =\{0\}$, thì $\mathfrak{n}\subset \mathfrak{h}$ và $\mathfrak{n}\subset \mathfrak{h}'($§2, no. 1, Mệnh đề 5), do đó $\mathfrak{h}=\mathfrak{h}+\mathfrak{n}=\mathfrak{h}'+\mathfrak{n}=\mathfrak{h}'$. Còn lại cần xét trường hợp $[\mathfrak{g},\mathfrak{n}] =\mathfrak{n}$, do đó $\mathfrak{n}\subset \mathscr{C}^{\infty}(\mathfrak{g})$. Iđêan $\mathfrak{n}$ là một $\mathfrak{g}$-môđun đơn; vì $\mathfrak{g}=\mathfrak{h}+\mathfrak{n}$, và vì $[\mathfrak{n},\mathfrak{n}] =\{0\}$, suy ra rằng $\mathfrak{n}$ là một $\mathfrak{h}$-môđun đơn. Nếu $\mathfrak{h}\cap \mathfrak{n}\not=\{0\}$, thì $\mathfrak{n}\subset \mathfrak{h}$, do đó $\mathfrak{g}=\mathfrak{h}$ và $\mathfrak{h}'=\mathfrak{h}$. Bây giờ giả sử rằng $\mathfrak{h}\cap \mathfrak{n}=\{0\}$. Khi đó $\mathfrak{g}=\mathfrak{h}\oplus \mathfrak{n}$ và do đó $\mathfrak{g}=\mathfrak{h}'\oplus \mathfrak{n}$, vì $\mathfrak{h}$ và $\mathfrak{h}'$ có cùng chiều.

Với mọi $x\in \mathfrak{h}$, gọi $f(x)$ là phần tử duy nhất của $\mathfrak{n}$ sao cho $x-f(x)\in \mathfrak{h}'$; nếu $x, y\in \mathfrak{h}$,

$$
[x, y]-[x, f(y)]-[f(x), y] = [x-f(x), y-f(y)]\in \mathfrak{h}'
$$

do đó $f([x, y]) = [x, f(y)] + [f(x), y]$. Theo §1, no. 3, Hệ quả của Mệnh đề 9, tồn tại $a\in \mathfrak{n}$ sao cho $f(x) = [x, a]$ với mọi $x\in \mathfrak{h}$. Ta có (ad $a$)$^2(\mathfrak{g})\subset$ (ad $a$)$(\mathfrak{n}) = 0$, do đó, với mọi $x\in \mathfrak{h}$,

$$
e^{ada}x=x+ [a, x] =x-f(x)
$$

Suy ra $e^{ada}(\mathfrak{h}) =\mathfrak{h}'$. Vì $a\in \mathscr{C}^{\infty}(\mathfrak{g})$, điều này hoàn tất chứng minh.

#### Bổ đề 3 {#lie-vii-s3-lem-3 .statement tag=00VE}

Cho $\mathfrak{g}$ là một đại số Lie, $\mathfrak{r}$ là căn của nó, $\varphi$ là đồng cấu chính tắc từ $\mathfrak{g}$ đến $\mathfrak{g}/\mathfrak{r},v$ là một tự đẳng cấu sơ cấp của $\mathfrak{g}/\mathfrak{r}$. Tồn tại một tự đẳng cấu sơ cấp $u$ của $\mathfrak{g}$ sao cho $\varphi \circ u=v\circ \varphi$.

Ta có thể giả sử rằng $v$ có dạng $e^{adb}$, trong đó $b\in \mathfrak{g}/\mathfrak{r}$ và ad $b$ là lũy linh. Gọi $\mathfrak{s}$ là một đại số con Levi của $\mathfrak{g}$ (Chap. I, §6, no. 8, Định nghĩa 7) và gọi $a$ là phần tử của $\mathfrak{s}$ sao cho $\varphi (a) =b$. Vì ad$_{\mathfrak{s}}a$ là lũy linh, ad$_{\mathfrak{g}}a$ là lũy linh (Chap. I, §6, no. 3, Hệ quả của Mệnh đề 3), và $u=e^{ad_{\mathfrak{g}}a}$ là một tự đẳng cấu sơ cấp của $\mathfrak{g}$ sao cho $\varphi \circ u=v\circ \varphi$.

#### Mệnh đề 5 {#lie-vii-s3-prop-5 .statement tag=00VF}

Cho $\mathfrak{g}$ là một đại số Lie, $\mathfrak{r}$ là căn của nó, $\mathfrak{h}$ và $\mathfrak{h}'$ là các đại số con Cartan của $\mathfrak{g}$, và $\varphi$ là đồng cấu chính tắc từ $\mathfrak{g}$ đến $\mathfrak{g}/\mathfrak{r}$. Các điều kiện sau là tương đương:

(i) $\mathfrak{h}$ và $\mathfrak{h}'$ liên hợp bởi một tự đẳng cấu sơ cấp của $\mathfrak{g}$;

(ii) $\varphi (\mathfrak{h})$ và $\varphi (\mathfrak{h}')$ liên hợp bởi một tự đẳng cấu sơ cấp của $\mathfrak{g}/\mathfrak{r}$.

(i) $=\Rightarrow$ (ii): Điều này là hiển nhiên.

(ii) $=\Rightarrow$ (i): Ta giả sử rằng điều kiện (ii) được thỏa mãn và chứng minh (i). Theo Bổ đề 3, ta quy về trường hợp $\varphi (\mathfrak{h}) =\varphi (\mathfrak{h}')$. Đặt $\mathfrak{k}=$ $\mathfrak{h}+\mathfrak{r}=\mathfrak{h}'+\mathfrak{r}$, là một đại số con giải được của $\mathfrak{g}$. Khi đó $\mathfrak{h}$ và $\mathfrak{h}'$ là các đại số con Cartan của $\mathfrak{k}$, do đó tồn tại $x\in \mathscr{C}^{\infty}(\mathfrak{k})$ sao cho $e^{ad_{\mathfrak{k}}x}\mathfrak{h}=\mathfrak{h}'$ (Đl. 3). Vì $\mathfrak{k}/\mathfrak{r}$ là lũy linh, $\mathscr{C}^{\infty}(\mathfrak{k})\subset \mathfrak{r}$; mặt khác, $\mathscr{C}^{\infty}(\mathfrak{k})\subset [\mathfrak{k},\mathfrak{k}]\subset [\mathfrak{g},\mathfrak{g}]$, nên $x\in \mathfrak{r}\cap [\mathfrak{g},\mathfrak{g}]$; theo Chương I, §5, số. 3, Đl. 1, ad$_{\mathfrak{g}}x$ là lũy linh, do đó $e^{ad_{\mathfrak{g}}x}$ là một tự đẳng cấu sơ cấp của $\mathfrak{g}$ biến $\mathfrak{h}$ thành $\mathfrak{h}'$.

### 5. TRƯỜNG HỢP NHÓM LIE

#### Mệnh đề 6 {#lie-vii-s3-prop-6 .statement tag=00VG}

Giả sử rằng $k$ là $\mathbf{R},\mathbf{C}$ hoặc một trường ultrametric đầy đủ rời rạc có đặc số 0. Cho $G$ là một nhóm Lie hữu hạn chiều trên $k,e$ là phần tử đơn vị của nó, $\mathfrak{g}$ là đại số Lie của nó, $\mathfrak{h}$ là một đại số con Cartan của $\mathfrak{g},\mathfrak{h}_r$ là tập hợp các phần tử chính quy của $\mathfrak{g}$ thuộc $\mathfrak{h}$.

(i) Cho $\mathfrak{s}$ là một không gian vectơ bù của $\mathfrak{h}$ trong $\mathfrak{g},\mathfrak{s}_0$ là một lân cận của 0 trong $\mathfrak{s}$ trên đó một ánh xạ mũ được xác định, và $h_0\in \mathfrak{h}_r$. Ánh xạ $(s, h) \rightarrow F(s, h) =$ (exp ad $s$).$h$ từ $\mathfrak{s}_0\times \mathfrak{h}$ đến $\mathfrak{g}$ là étale tại $(0, h_0)$.

(ii) Ánh xạ $(g, h) \rightarrow F'(g, h) =$ (Ad $g$).$h$ từ $G\times \mathfrak{h}_r$ đến $\mathfrak{g}$ là một ánh xạ hạ chìm. Đặc biệt, ảnh của nó $\Omega$ là mở. Với mọi $x\in \Omega ,\mathfrak{g}^0(x)$ là một đại số con Cartan của $\mathfrak{g}$ liên hợp với $\mathfrak{h}$ dưới Ad(G).

(iii) Cho $h_0\in \mathfrak{h}_r$. Với mọi lân cận U của $e$ trong G, tập hợp $\bigcup_{a\in U}$(Ad $a$)$(\mathfrak{h}_r)$

là một lân cận của $h_0$ trong $\mathfrak{g}$.

Cho $h_0$ và $\mathfrak{s}$ như trong (i). Gọi T là ánh xạ tuyến tính tiếp xúc của F tại $(0, h_0)$. Khi đó $F(0, h) =h$ với mọi $h\in \mathfrak{h}$, do đó $T(0, h) =h$ với mọi $h\in \mathfrak{h}$. Mặt khác, với $\mathfrak{s}_0$ đủ nhỏ, ánh xạ tuyến tính tiếp xúc tại 0 của ánh xạ $s \rightarrow$ exp ad $s$ từ $\mathfrak{s}_0$ vào End($\mathfrak{g}$) là ánh xạ $s \rightarrow$ ad $s$ từ $\mathfrak{s}$ vào End($\mathfrak{g}$). Vì vậy $T(s,0) = [s, h_0]$ với mọi $s\in \mathfrak{s}$. Bây giờ ánh xạ từ $\mathfrak{g}/\mathfrak{h}$ vào $\mathfrak{g}/\mathfrak{h}$ cảm sinh bởi ad $h_0$ qua phép lấy thương là song ánh. Suy ra T là song ánh, do đó (i). Vì exp ad $s=$ Ad exp $s$ với mọi $s\in \mathfrak{s}$ đủ gần 0, nên (iii) và mệnh đề đầu tiên của (ii) suy ra. Mọi $x\in \Omega$ đều có dạng (Ad $a$)$(h)$ với $a\in G$ và $h\in \mathfrak{h}_r$, nên $\mathfrak{g}^0(x) =$ (Ad $a$)$(\mathfrak{g}^0(h)) =$ (Ad $a$)$(\mathfrak{h})$ là một đại số con của $\mathfrak{g}$ liên hợp với $\mathfrak{h}$ dưới Ad(G).

### Bài tập {#lie-vii-s3-exercises}

Xem các [bài tập của § 3](exercises/s3/).
