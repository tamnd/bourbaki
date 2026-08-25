---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: VI
chapter_title: ROOT SYSTEMS
section: 3
section_title: Exponential invariants
lang: vi
source: lie-iv-vi
pdf_pages: 0207-0213, 0254-0254
extraction: ocr
subsections:
    - "no": 1
      title: GROUP ALGEBRA OF A FREE ABELIAN GROUP
      page: 0
      pdf_page: 207
    - "no": 2
      title: CASE OF THE GROUP OF WEIGHTS; MAXIMAL TERMS
      page: 0
      pdf_page: 208
    - "no": 3
      title: ANTI-INvariant ELEMENTS
      page: 0
      pdf_page: 209
    - "no": 4
      title: INVARIANT ELEMENTS
      page: 0
      pdf_page: 212
statements: 12
exercises: 2
content_sha256: 4f47126adadf3898a093b80782466a29a62247ea4558a4b17e703ea30e42e05e
translated_from: content/en/lie/VI/03_s3_exponential_invariants.md
source_content_sha256: a1d623b664a3e6aeb9850e9dddd38396c5fe9526ee78a042d5bd1805375ab6bf
translation_model: gpt-5.4
translation_run: translate-vi-f41c29d2
glossary_version: 34
glossary_terms_sha256: f0107f875bbdaba3c79f4b97210e11d8cd468072e1ce40a679578794c11a6fcf
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 3. BẤT BIẾN MŨ

Trong tiết này, chữ A chỉ một vành giao hoán, có phần tử đơn vị, và khác 0.

### 1. ĐẠI SỐ NHÓM CỦA MỘT NHÓM ABEL TỰ DO

Cho P là một $\mathbf{Z}$-môđun tự do hạng hữu hạn $l$. Ta ký hiệu bởi $A[P]$ đại số nhóm của nhóm cộng của P trên A (*Đại số*, Chương III, § 2, no. 6). Với mọi $p \in P$, ký hiệu bởi $e^p$ phần tử tương ứng của $A[P]$. Khi đó $(e^p)_{p \in P}$ là một *cơ sở* của A-môđun $A[P]$, và, với mọi $p, p' \in P$, ta có
$$
e^p e^{p'} = e^{p + p'}, \quad (e^p)^{-1} = e^{-p}, \quad e^0 = 1.
$$

#### Bổ đề 1 {#lie-vi-s3-lem-1 .statement}

*Giả sử rằng A là một vành factorial* (*Đại số giao hoán*, Chương VII, § 3, no. 1, Định nghĩa 1).
(i) *Vành $A[P]$ là factorial.*
(ii) *Nếu $u, v$ là các phần tử không tỷ lệ của P, thì các phần tử $1 - e^u, 1 - e^v$ của $A[P]$ nguyên tố cùng nhau.*

Cho $(p_1, p_2, \ldots, p_l)$ là một cơ sở của P, và $X_1, X_2, \ldots, X_l$ là các bất định. Ánh xạ A-tuyến tính từ $A[X_1, \ldots, X_l, X_1^{-1}, \ldots, X_l^{-1}]$ vào $A[P]$ biến $X_1^{n_1} X_2^{n_2} \ldots X_l^{n_l}$ (trong đó $n_1, n_2, \ldots, n_l \in \mathbf{Z}$) thành $e^{n_1 p_1 + \cdots + n_l p_l}$ là một đẳng cấu vành. Bây giờ $A[X_1, \ldots, X_l]$ là một vành giai thừa (*Đại số giao hoán*, Chap. VII, § 3, no. 5), và $A[X_1, \ldots, X_l, X_1^{-1}, \ldots, X_l^{-1}]$ là vành các phân thức của $A[X_1, \ldots, X_l]$, do đó nó cũng là giai thừa.

Cho $P'$ (ứng với $P''$) là tập hợp các phần tử của P mà một bội nào đó của chúng thuộc $\mathbf{Z}u + \mathbf{Z}v$ (ứng với $\mathbf{Z}u$). Khi đó các nhóm $P/P'$ và $P'/P''$ là không xoắn, nên tồn tại một phần bù của $P''$ trong $P'$ và một phần bù của $P'$ trong P. Do đó, tồn tại một cơ sở $(z_1, z_2, \ldots, z_l)$ của $\mathbf{Z}$-môđun P và các số nguyên hữu tỉ $j, m, n$ sao cho $u = jz_1, v = mz_1 + nz_2, j > 0, n > 0$. Đặt $X_i = e^{z_i}$ với $1 \leq i \leq l$, khi đó ta có $1 - e^u = 1 - X_1^j, 1 - e^v = 1 - X_1^m X_2^n$. Cho K là một bao đóng đại số của trường phân thức của A, để $A[P]$ có thể được đồng nhất với một vành con của vành $B = K[X_1, \ldots, X_l, X_1^{-1}, \ldots, X_l^{-1}]$. Với mọi nghiệm bậc $j$ của đơn vị $z$, $1 - zX_1$ là cực biên trong
$$
K[X_1, \ldots, X_l];
$$
hơn nữa, iđêan sinh bởi $1 - zX_1$ không chứa đơn thức nào theo các $X_i$. Ta kết luận rằng iđêan $(1 - zX_1)B$ của B là một iđêan nguyên tố chiều cao 1

(Đại số giao hoán, Chương VII, § 1, no. 6), do đó $1 - zX_1$ là cực biên trong B. Vì thế các thừa số cực biên của $1 - X_1^j$ trong B có dạng $1 - zX_1$. Bây giờ không một thừa số nào trong các thừa số đó chia hết $1 - X_1^m X_2^n$ trong B (vì đồng cấu $f$ từ B vào B sao cho $f(X_1) = z^{-1}, f(X_i) = X_i$ với $i \geq 2$, thỏa mãn

$$
f(1 - zX_1) = 0 \quad \text{và} \quad f(1 - X_1^m X_2^n) = 1 - z^{-m} X_2^n \neq 0).
$$

Do đó, $1 - X_1^j$ và $1 - X_1^m X_2^n$ là nguyên tố cùng nhau trong B. Do đó, mọi ước chung của $1 - X_1^j$ và $1 - X_1^m X_2^n$ trong $A[P]$ đều khả nghịch trong B và vì thế, sai khác bởi phép nhân với một phần tử có dạng $X_1^{k_1} X_2^{k_2} \ldots X_l^{k_l}$, đều bằng một phần tử $a$ của A; nói cách khác, $a$ chia hết 1 trong A, nên khả nghịch trong A. Vậy, sau cùng, $1 - X_1^j$ và $1 - X_1^m X_2^n$ là nguyên tố cùng nhau trong $A[P]$.

### 2. TRƯỜNG HỢP CỦA NHÓM TRỌNG SỐ; CÁC HẠNG TỬ CỰC ĐẠI

Ta giữ lại các ký hiệu của số trước và cho R là một hệ căn rút gọn trong một không gian vectơ thực V. Trong phần còn lại của tiết diện này, ta lấy P là nhóm trọng số của R (\S 1, no. 9). Nhóm $W = W(R)$ tác động trên P, do đó cũng tác động trên đại số $A[P]$; ta có $w(e^p) = e^{w(p)}$ với $w \in W$ và $p \in P$.

Cho C là một buồng của R (\S 1, no. 5) và cho $B = (\alpha_i)_{1 \leq i \leq l}$ là cơ sở tương ứng của R. Ta trang bị cho V (và do đó cũng cho P) cấu trúc thứ tự được xác định bởi C. Nếu $p, p' \in P, p \geq p'$ khi và chỉ khi $p - p'$ là một tổ hợp tuyến tính của các $\alpha_i$ với các hệ số dương.

#### Định nghĩa 1 {#lie-vi-s3-def-1 .statement}

Cho $x = \sum_{p \in P} x_p e^p$ là một phần tử của $A[P]$. Tập hợp S các $p \in P$ sao cho $x_p \neq 0$ được gọi là giá của x và tập hợp X các phần tử cực đại của S được gọi là giá cực đại của x. Khi đó một số hạng $x_p e^p$ với $p \in X$ được gọi là một số hạng cực đại của x.

#### Bổ đề 2 {#lie-vi-s3-lem-2 .statement}

Cho $x \in A[P]$ và gọi $(x_p e^p)_{p \in X}$ là họ các số hạng cực đại của x. Cho $q \in P$ và cho $y \in A[P]$ sao cho $e^q$ là số hạng cực đại duy nhất của y. Khi đó, họ các số hạng cực đại của $xy$ là $(x_p e^{p+q})_{p \in X}$.

Đặt $x = \sum_p x_p e^p, y = \sum_r y_r e^r$ và $xy = \sum_t z_t e^t$. Khi đó $r \leq q$ với mọi $r \in P$ sao cho $y_r \neq 0$ và $z_t = \sum_{p+r=t} x_p y_r$.

Nếu $t = p + q = p' + r$ với $p \in X$ và $x_{p'} y_r \neq 0$, thì $r \leq q$, nên $p' \geq p$ và do đó $p' = p$. Vì thế $z_{p+q} = x_p y_q = x_p \neq 0$. Điều này cho thấy rằng $X + q$ được chứa trong giá đỡ của tích $xy$.

Mặt khác, nếu $t = p' + r$ với $x_{p'} y_r \neq 0$, thì tồn tại $p \in X$ sao cho $p' \leq p$ và ta có $t \leq p + q$. Vậy giá của $xy$ là cực đại được chứa trong $X + q$. Vì không có hai phần tử nào của $X + q$ là so sánh được với nhau, suy ra $X + q$ chính xác là giá cực đại của $xy$ và ở trên ta đã thấy rằng $z_{p+q} = x_p$ với $p \in X$, điều này hoàn thành chứng minh của bổ đề.

#### Nhận xét {#lie-vi-s3-n2-rem-1 .statement}

Vì $x \neq 0$ có nghĩa là giá cực đại của $x$ là không rỗng, Bổ đề 2 cho thấy rằng $x \neq 0$ kéo theo $xy \neq 0$ bất cứ khi nào $y$ có một số hạng cực đại duy nhất có dạng $e^q$.

### 3. CÁC PHẦN TỬ PHẢN-BẤT BIẾN

Ta giữ lại các ký hiệu của số trước. Ký hiệu bởi $\varepsilon(w)$ định thức của phần tử $w \in W$. Khi đó
$$
\varepsilon(w) = (-1)^{l(w)},
$$
trong đó độ dài $l(w)$ được lấy đối với họ các phép đối xứng $s_{\alpha_i}$.

#### Định nghĩa 2 {#lie-vi-s3-def-2 .statement}

*Một phần tử* $x \in A[P]$ *được gọi là phản-bất biến dưới* $W$ *nếu*
$$
w(x) = (-1)^{l(w)}.x
$$
*với mọi* $w \in W$.

Các phần tử phản bất biến của $A[P]$ tạo thành một môđun con trên $A$ của $A[P]$. Với mọi $x \in A[P]$, đặt
$$
J(x) = \sum_{w \in W} \varepsilon(w).w(x).
$$
(1)

Với $x \in A[P]$ và $w \in W$, ta có
$$
w(J(x)) = \sum_{v \in W} \varepsilon(v).wv(x) = \varepsilon(w) \sum_{v \in W} \varepsilon(v).v(x) = \varepsilon(w).J(x)
$$
và $J(x)$ là phản bất biến. Mặt khác, đặt $q = \mathrm{Card}(W)$. Với mọi phần tử phản bất biến $x$ của $A[P]$, ta có $J(x) = q.x$. Suy ra rằng, nếu $q$ khả nghịch trong $A$, thì ánh xạ $q^{-1}J$ là một *phép chiếu* từ $A[P]$ lên môđun con các phần tử phản bất biến.

Gọi $\overline{\omega}_1, \ldots, \overline{\omega}_l$ là các trọng cơ bản tương ứng với buồng $C$. Các phần tử của $P \cap \overline{C}$ (resp. $P \cap C$) là các trọng có dạng $n_1 \overline{\omega}_1 + \cdots + n_l \overline{\omega}_l$ với $n_i \geq 0$ (resp. $n_i > 0$) với $1 \leq i \leq l$ (\S 1, no. 10). Mặt khác,
$$
\rho = \overline{\omega}_1 + \cdots + \overline{\omega}_l
$$
là nửa tổng của các căn dương (*loc. cit.*) nên các phần tử của $P \cap C$ là các trọng có dạng $\rho + p$ với $p \in P \cap \overline{C}$. Cuối cùng, nếu $p \in P \cap C$, thì $w(p) < p$ với mọi $w \neq 1$ (\S 1, no. 6, Hệ quả của Mệnh đề 18) và do đó $e^p$ là số hạng cực đại duy nhất của $J(e^p)$.

#### Mệnh đề 1 {#lie-vi-s3-prop-1 .statement}

*Nếu* 2 *không phải là một ước của không trong* $A$, *thì các phần tử* $J(e^p)$ *với* $p \in P \cap C$ *lập thành một cơ sở của môđun các phần tử phản bất biến của* $A[P]$.

Các trọng số $w(p)$ với $w \in W$ và $p \in P \cap C$ là từng đôi một phân biệt. Suy ra các $J(e^p)$ với $p \in P \cap C$ là độc lập tuyến tính.

Mặt khác, cho $x = \sum_p x_p e^p$ là một phần tử phản bất biến của $A[P]$. Nếu $p_0$ thuộc một tường, thì nó bất biến dưới một phép đối xứng $s \in W$ và
$$
x = \sum_p x_p e^p = -s(x) = -\sum_p x_p e^{s(p)}.
$$
Suy ra $2x_{p_0} = 0$, nên $x_{p_0} = 0$. Vì mọi phần tử không thuộc bất kỳ tường nào đều có thể được viết duy nhất dưới dạng $w(p)$ với $w \in W$ và $p \in P \cap C$, do đó ta có
$$
x = \sum_{p \in P \cap C} \sum_{w \in W} x_{w(p)} e^{w(p)}. \tag{2}
$$
Vì $w(x) = \sum_p x_p e^{w(p)} = \varepsilon(w) \sum_p x_p e^p$, nên $x_{w(p)} = \varepsilon(w)x_p$ và ta suy ra từ (2) rằng
$$
x = \sum_{p \in P \cap C} x_p J(e^p),
$$
điều này hoàn tất chứng minh.

Bây giờ xét phần tử $d$ của đại số $A[\frac{1}{2}P]$ được định nghĩa bởi
$$
d = \prod_{\alpha \in R, \alpha > 0} (e^{\alpha/2} - e^{-\alpha/2}) \\
= e^{\rho} \cdot \prod_{\alpha \in R, \alpha > 0} (1 - e^{-\alpha}) \\
= e^{-\rho} \cdot \prod_{\alpha \in R, \alpha > 0} (e^{\alpha} - 1).
$$
Vì $\rho \in P$, nên $d \in A[P]$.

#### Mệnh đề 2 {#lie-vi-s3-prop-2 .statement}

(i) *Phần tử d được xác định bởi (3) là một phần tử phản bất biến của A[P]; số hạng cực đại duy nhất của nó* (no. 2, Định nghĩa 1) *là* $e^{\rho}$ *và* $d = J(e^{\rho})$.
(ii) *Với mọi* $p \in P$, *phần tử* $J(e^p)$ *chia được duy nhất cho* $d$ *và thương* $J(e^p)/d$ *là một phần tử của* $A[P]$ *bất biến dưới* $W$.
(iii) *Nếu 2 không phải là một ước của không trong* $A$, *phép nhân bởi* $d$ *là một song ánh từ tập hợp các phần tử của* $A[P]$ *bất biến dưới* $W$ *lên tập hợp các phần tử phản bất biến của* $A[P]$.

Ta biết rằng, với $1 \leq i \leq l$, phép phản xạ $s_i = s_{\alpha_i}$ giữ ổn định tập các căn dương khác $\alpha_i$ và rằng $s_i(\alpha_i) = -\alpha_i$ (\S 1, no. 6, Hệ quả 1 của Mệnh đề 17). Do đó,
$$
s_i(d) = (e^{-\alpha_i/2} - e^{\alpha_i/2}) \prod_{\alpha \in R, \alpha > 0, \alpha \neq \alpha_i} (e^{\alpha/2} - e^{-\alpha/2}) \\
= -d = \varepsilon(s_i).d.
$$
Vì các $s_i$ sinh ra $W$, điều này chứng minh mệnh đề thứ nhất trong (i). Mệnh đề thứ hai trong (i) suy ra ngay lập tức từ (3) và Bổ đề 2, khi lưu ý rằng 1 là số hạng cực đại duy nhất của $1 - e^{-\alpha}$ đối với $\alpha \in R, \alpha > 0$.

Bây giờ giả sử rằng $A = \mathbf{Z}$. Theo Mệnh đề 1,

$$
d = \prod_{p \in P \cap C} c_p J(e^p) \quad \text{với} \quad c_p \in \mathbf{Z}.
$$

Mặt khác, hiển nhiên là

$$
d = e^\rho + \sum_{q < \rho} c'_q e^q.
$$

Nếu $p \in P \cap C$ với $p \neq \rho$, thì $p > \rho$ và hệ số của $e^p$ trong $d$ bằng không theo (5). Do đó, $c_p = 0$. Hơn nữa, việc so sánh các hệ số của $e^\rho$ trong (4) và (5) cho thấy $c_\rho = 1$ và vì thế $d = J(e^\rho)$.

Ta tiếp tục giả sử rằng $A = \mathbf{Z}$. Cho $p \in P, \alpha \in \mathbf{R}$ và $M$ là một hệ các đại diện của các lớp kề phải của $W$ đối với nhóm con $\{1, s_\alpha\}$. Khi đó,

$$
J(e^p) = \sum_{w \in M} \varepsilon(w) e^{w(p)} + \sum_{w \in M} \varepsilon(s_\alpha w) e^{s_\alpha w(p)}.
$$

Bây giờ $s_\alpha w(p) = w(p) - \langle \alpha^*, w(p) \rangle \alpha = w(p) + n_w \alpha$, với $n_w \in \mathbf{Z}$. Do đó,

$$
J(e^p) = \sum_{w \in M} \varepsilon(w) e^{w(p)} (1 - e^{n_w \alpha}).
$$

Nếu $n_w \geq 0$, hiển nhiên là $1 - e^{n_w \alpha}$ chia được cho $1 - e^\alpha$ và điều này cũng đúng khi $n_w < 0$ vì $1 - e^{n_w \alpha} = -e^{n_w \alpha}(1 - e^{-n_w \alpha})$. Vậy $J(e^p)$ chia được cho $1 - e^\alpha$ trong $\mathbf{Z}[P]$.

Theo Bổ đề 1, $\mathbf{Z}[P]$ là một vành phân tích duy nhất và các phần tử $1 - e^\alpha$ với $\alpha \in \mathbf{R}$ và $\alpha > 0$ là đôi một nguyên tố cùng nhau. Suy ra $J(e^p)$ chia được trong $\mathbf{Z}[P]$ cho tích $\prod_{\alpha > 0} (1 - e^\alpha)$, và do đó cũng chia được cho $d = e^{-\rho} \prod_{\alpha > 0} (1 - e^\alpha)$.

Trở lại trường hợp tổng quát, bằng phép mở rộng các vô hướng từ $\mathbf{Z}$ sang $A$, ta suy ra từ trên rằng $d = J(e^\rho)$ và mọi phần tử $J(e^p)$ đều chia được cho $d$. Vì $e^\rho$ là số hạng cực đại duy nhất của $d$, Nhận xét của no. 2 cho thấy rằng tồn tại một phần tử duy nhất $y \in A[P]$ sao cho $J(e^p) = dy$ và ngay lập tức suy ra rằng $y$ là bất biến dưới $W$, và do đó $d$ và $J(e^p)$ là phản bất biến. Điều này chứng minh (i) và (ii).

Cuối cùng, nếu 2 không là một ước của không trong $A$, thì Nhận xét của no. 2 và Mệnh đề 1 suy ra (iii).

#### Nhận xét 1 {#lie-vi-s3-n3-rem-1 .statement}

Nếu 2 không phải là một ước của không trong $A$, thì dễ kiểm tra rằng $d$ là phần tử phản bất biến duy nhất của $A[P]$ có $e^\rho$ là số hạng cực đại của nó.

#### Nhận xét 2 {#lie-vi-s3-n3-rem-2 .statement}

Bổ đề 2 của no. 2 cho thấy rằng số hạng cực đại duy nhất của thương $J(e^p)/d$ (với $p \in P \cap C$) là $e^{p-\rho}$.

### 4. CÁC PHẦN TỬ BẤT BIẾN

Cho $A[P]^W$ là đại số con của $A[P]$ gồm các phần tử bất biến dưới $W$. Với $p \in P$, ký hiệu bởi $W.p$ quỹ đạo của $p$ dưới $W$, và đặt $S(e^p) = \sum_{q \in W.p} e^q$ là tổng các biến đổi bởi $W$ của $e^p$; đây là một phần tử bất biến dưới $W$.

Nếu $p \in P \cap \overline{C}$, thì $w(p) \leq p$ với mọi $w \in W$ ($\S$ 1, no. 6, Mệnh đề 18) và $e^p$ là số hạng cực đại duy nhất của $S(e^p)$.

Cho $x = \sum_p x_p e^p \in A[P]^W$; khi đó $x_{w(p)} = x_p$ với mọi $p \in P$ và mọi $w \in W$.

Mặt khác, mọi quỹ đạo của $W$ trong $P$ cắt $P \cap \overline{C}$ tại đúng một điểm ($\S$ 1, no. 5, Định lý 2). Do đó,

$$
x = \sum_{P \cap \overline{C}} x_p S(e^p).
$$

Ta suy ra:

#### Bổ đề 3 {#lie-vi-s3-lem-3 .statement}

*Các $S(e^p)$ với $p \in P \cap \overline{C}$ tạo thành một cơ sở của $A$-môđun $A[P]^W$.*

$$
e_{i_0} = x_{i_0} - \sum_{j < i_0} a_{i_0 j} e_j,
$$
từ đó suy ra (b). Do đó $J' \in \mathfrak{S}$, mâu thuẫn. Vậy $J = I$ và bổ đề được chứng minh.

Bây giờ chúng ta chứng minh Mệnh đề 3. Ta áp dụng Bổ đề 4 với $I = P \cap \overline{C}$. Cho $q \in I$, và gọi $I_q$ là tập hợp các $p \in I$ sao cho $p \leq q$. Nếu $p \in I_q$, các hệ thức
$$
q - p \geq 0,\quad p \in \overline{C},\quad q \in \overline{C}
$$
suy ra rằng
$$
(q - p|p) \geq 0 \quad \text{và} \quad (q - p|q) \geq 0,
$$
và do đó
$$
(p|p) \leq (p|q) \leq (q|q).
$$
Vậy tập hợp $I_q$ là *bị chặn*. Vì $I$ là rời rạc, suy ra $I_q$ là *hữu hạn*, và hiển nhiên là $I$ thỏa mãn điều kiện (MIN). Mặt khác, với mọi $p \in I$,
$$
x_p = e^p + \sum_{q < p} c_{pq} e^q
$$
nên theo (6).
$$
x_p = S(e^p) + \sum_{q < p, q \in I} c_{pq} S(e^q).
$$
Mệnh đề bây giờ suy ra từ các Bổ đề 3 và 4.

#### Định lý 1 {#lie-vi-s3-thm-1 .statement}

*Cho $\overline{\omega}_1, \ldots, \overline{\omega}_l$ là các trọng số cơ bản tương ứng với buồng $C$, và, với $1 \leq i \leq l$, cho $x_i$ là một phần tử của $A[P]^W$ có $e^{\overline{\omega}_i}$ là số hạng cực đại duy nhất. Cho*
$$
\varphi : \Lambda[X_1, \ldots, X_l] \to A[P]^W
$$
*là đồng cấu từ đại số đa thức $\Lambda[X_1, \ldots, X_l]$ vào $A[P]^W$ biến $X_i$ thành $x_i$. Khi đó, ánh xạ $\varphi$ là một đẳng cấu.*

Bổ đề 2 kéo theo rằng ảnh qua $\varphi$ của đơn thức $X_1^{n_1} \ldots X_l^{n_l}$ là một phần tử có số hạng cực đại duy nhất $e^{n_1 \overline{\omega}_1 + \cdots + n_l \overline{\omega}_l}$. Vì mọi phần tử của $P \cap \overline{C}$ đều có thể viết một cách duy nhất dưới dạng $n_1 \overline{\omega}_1 + \cdots + n_l \overline{\omega}_l$, Mệnh đề 3 cho thấy rằng các ảnh qua $\varphi$ của các đơn thức $X_1^{n_1} \ldots X_l^{n_l}$ tạo thành một cơ sở của $A[P]^W$, do đó suy ra định lý.

#### Ví dụ 1 {#lie-vi-s3-n4-exa-1 .statement}

Ta có thể lấy $x_i = S(e^{\overline{\omega}_i})$.
2) Theo *Nhận xét* 2 của no. 3, ta có thể lấy $x_i = J(e^{\rho + \overline{\omega}_i})/d$ (với ký hiệu ở no. 3).

### Bài tập {#lie-vi-s3-exercises}

Các ký hiệu và giả thiết là các ký hiệu và giả thiết của các số 2, 3, 4.

Xem [bài tập cho § 3](exercises/s3/).
