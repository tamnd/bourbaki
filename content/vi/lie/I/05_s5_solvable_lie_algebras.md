---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: I
chapter_title: Lie Algebras
section: 5
section_title: Solvable Lie algebras
lang: vi
source: lie-i-iii
book_pages: 43-50, 99-101
pdf_pages: 0061-0068, 0117-0119
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF SOLVABLE LIE ALGEBRAS
      page: 43
      pdf_page: 61
    - "no": 2
      title: RADICAL OF A LIE ALGEBRA
      page: 44
      pdf_page: 62
    - "no": 3
      title: NILPOTENT RADICAL OF A LIE ALGEBRA
      page: 44
      pdf_page: 62
    - "no": 4
      title: A CRITERION FOR SOLVABILITY
      page: 47
      pdf_page: 65
    - "no": 5
      title: FURTHER PROPERTIES OF THE RADICAL
      page: 48
      pdf_page: 66
    - "no": 6
      title: EXTENSION OF THE BASE FIELD
      page: 49
      pdf_page: 67
statements: 27
exercises: 17
content_sha256: ef6542df1d646219d4df97c8b9c498674f6c1f73a4ea49d6c088ebad1a551fd1
translated_from: content/en/lie/I/05_s5_solvable_lie_algebras.md
source_content_sha256: bc96d56afc3255aae8af0a123337b972ece4e127279103def5f9db7ba948b944
translation_model: gpt-5.4
translation_run: translate-vi-f47a882b
glossary_version: 34
glossary_terms_sha256: a13ee3c7dbb7af6584e14b346317574b35ec853a8b50bf0a283c3890b06bf6ba
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 5. ĐẠI SỐ LIE GIẢI ĐƯỢC

Nhắc lại rằng từ nay $K$ ký hiệu một trường có đặc số 0 và mọi đại số Lie đều được giả thiết là hữu hạn chiều trên $K$.†

### 1. ĐỊNH NGHĨA ĐẠI SỐ LIE GIẢI ĐƯỢC

#### Định nghĩa 1 {#lie-i-s5-def-1 .statement}

*Một đại số Lie $g$ được gọi là giải được nếu đại số dẫn xuất bậc $k$ của nó $D^k g$ bằng không với $k$ đủ lớn.*

Một đại số Lie lũy linh là giải được.

#### Mệnh đề 1 {#lie-i-s5-prop-1 .statement}

*Các đại số con và các đại số thương của một đại số Lie giải được đều giải được. Mọi mở rộng của một đại số giải được bởi một đại số giải được đều giải được. Mọi tích hữu hạn của các đại số giải được đều giải được.*

Cho $g$ là một đại số Lie, $g'$ một đại số con, $h$ một iđêan của $g$, $t = g/h$ và $\phi$ là ánh xạ chính tắc của $g$ lên $t$. Nếu $g$ giải được thì $D^k g = \{0\}$ với một số nguyên $k$, do đó $D^k g' \subset D^k g = \{0\}$, $D^k t = \phi(D^k g) = \{0\}$ và vì thế $g'$ và $t$ giải được. Nếu $h$ và $t$ giải được thì tồn tại các số nguyên $s, t$ sao cho

$$
D^s h = D^t t = \{0\};
$$

khi đó $D^t g \subset h$, do đó $D^{s+t} g = D^s(D^t g) \subset D^s h = \{0\}$ và $g$ giải được. Khẳng định cuối cùng suy ra từ khẳng định thứ hai bằng quy nạp theo số các thừa số.

#### Mệnh đề 2 {#lie-i-s5-prop-2 .statement}

*Cho $g$ là một đại số Lie. Các điều kiện sau là tương đương:*

(a) $g$ giải được;
(b) *tồn tại một dãy giảm $g = g_0 \supset g_1 \supset \cdots \supset g_n = \{0\}$ các iđêan của $g$ sao cho các đại số $g_i/g_{i+1}$ là giao hoán ($i = 0, 1, \ldots, n-1$);*
(c) *tồn tại một dãy giảm $g = g'_0 \supset g'_1 \supset \cdots \supset g'_p = \{0\}$ các đại số con của $g$ sao cho $g'_{i+1}$ là một iđêan của $g'_i$ và $g'_i/g'_{i+1}$ là giao hoán ($i = 0, 1, \ldots, p-1$);*
(d) *tồn tại một dãy giảm $g = g''_0 \supset g''_1 \supset \cdots \supset g''_q = \{0\}$ các đại số con của $g$ sao cho $g''_{i+1}$ là một iđêan của $g''_i$ có đối chiều 1 ($i = 0, 1, \ldots, q-1$).*

(a) $\Rightarrow$ (b): chỉ cần xét dãy các iđêan dẫn xuất của $g$.
(b) $\Rightarrow$ (c): điều này hiển nhiên.
(c) $\Rightarrow$ (d): giả sử điều kiện (c) được thỏa mãn; mọi không gian con vectơ của $g'_i$ chứa $g'_{i+1}$ đều là một iđêan của $g'_i$, do đó ngay lập tức suy ra (d).
(d) $\Rightarrow$ (a): điều này suy ra ngay lập tức từ việc một mở rộng của một đại số giải được bởi một đại số giải được là giải được.

† Người đọc sẽ chú ý rằng giả thiết về đặc số của $K$ không được dùng trong số 1 và 2 của đoạn này.

Các ví dụ về đại số Lie giải được

I. Cho $g$ là một không gian vectơ 2 chiều trên $K$ và $(e_1, e_2)$ là một cơ sở của $g$. Tồn tại một và chỉ một phép nhân song tuyến tính phản xứng $(x, y) \mapsto [x, y]$ trên $g$ sao cho $[e_1, e_2] = e_2$. Dễ dàng kiểm tra rằng như vậy $g$ được trang bị một cấu trúc đại số Lie giải được. Bây giờ, cho $h$ là một đại số Lie không giao hoán chiều 2 trên $K$. Ta chỉ ra rằng $h$ đẳng cấu với $g$. Cho $(f_1, f_2)$ là một cơ sở của $h$. Phần tử $[f_1, f_2]$ khác không (nếu không thì $h$ sẽ giao hoán) và do đó nó sinh ra một không gian con 1 chiều $t$ của $h$. Khi đó $[h, h] = t$. Cho $(e'_1, e'_2)$ là một cơ sở của $h$ sao cho $e'_2 \in t$. Khi đó $[e'_1, e'_2] = \lambda e'_2$ với $\lambda \neq 0$. Thay $e'_1$ bằng $\lambda^{-1} e_1$, ta có thể giả sử rằng $\lambda = 1$, do đó có mệnh đề của ta.

II. Các công thức (5) của § 1 chứng minh rằng $\mathcal{D}t(n, K) = n(n, K)$. Vì $n(n, K)$ lũy linh và do đó giải được, nên $t(n, K)$ giải được. Vậy $st(n, K)$ giải được. Đặc biệt, $st(2, K)$ đẳng cấu với đại số của Ví dụ I.

### 2. CĂN CỦA MỘT ĐẠI SỐ LIE

Cho $a, b$ là hai iđêan giải được của một đại số Lie $g$. Đại số $(a + b)/b$ đẳng cấu với $a/(a \cap b)$ và do đó giải được, còn $a + b$, là một mở rộng của $(a + b)/b$ bởi $b$, cũng giải được (Mệnh đề 1). Suy ra rằng một iđêan giải được cực đại của $g$ chứa mọi iđêan giải được của $g$ và do đó $g$ có một iđêan giải được lớn nhất. Điều này cho phép ta đưa ra định nghĩa sau đây:

#### Định nghĩa 2 {#lie-i-s5-def-2 .statement}

*Can của một đại số Lie là iđêan giải được lớn nhất của nó.*

#### Mệnh đề 3 {#lie-i-s5-prop-3 .statement}

*Can $r$ của một đại số Lie $g$ là iđêan nhỏ nhất của $g$ sao cho $g/r$ có căn là $\{0\}$.*

Cho $a$ là một iđêan của $g$ và $\phi$ là ánh xạ chính tắc từ $g$ lên $g/a$. Nếu căn của $g/a$ bằng không, thì $\phi(r)$, là một iđêan giải được của $g/a$, bằng không; do đó $r \subset a$.

Mặt khác, ảnh ngược $\phi^{-1}(r')$ của căn $r'$ của $g/r$ là một iđêan của $g$ giải được theo Mệnh đề 1 và do đó bằng $r$; vì thế $r' = \{0\}$.

#### Mệnh đề 4 {#lie-i-s5-prop-4 .statement}

*Cho $g_1, \ldots, g_n$ là các đại số Lie. Căn $r$ của tích của các $g_i$ là tích của các căn $r_i$ của các $g_i$.*

Tích $r'$ của các $r_i$ là một iđêan giải được (Mệnh đề 1) và do đó $r' \subset r$. Ảnh chính tắc của $r$ trong $g_i$ là một iđêan giải được của $g_i$ và vì thế được chứa trong $r_i$; do đó $r \subset r'$.

### 3. CĂN LŨY LINH CỦA MỘT ĐẠI SỐ LIE

#### Định nghĩa 3 {#lie-i-s5-def-3 .statement}

*Cho $g$ là một đại số Lie. Căn lũy linh của $g$ là giao của các hạt nhân của các biểu diễn đơn hữu hạn chiều của $g$.*

#### Nhận xét {#lie-i-s5-n3-rem-1 .statement}

(1) Cho $s$ là căn lũy linh của $g$. Vì mọi dãy giảm các không gian vectơ con của $g$ đều dừng, tồn tại một số hữu hạn các biểu diễn đơn hữu hạn chiều của $g$ mà các hạt nhân của chúng có giao bằng $s$.

Tổng trực tiếp của các biểu diễn này là nửa đơn và có hạt nhân là s. Suy ra tập hợp các hạt nhân của các biểu diễn nửa đơn hữu hạn chiều của g có một phần tử nhỏ nhất, cụ thể là s.

(2) Theo Mệnh đề 4 (c) của § 4, no. 3, s cũng là giao của các iđêan lũy linh lớn nhất của các biểu diễn hữu hạn chiều của g. Đặc biệt, s được chứa trong iđêan lũy linh lớn nhất của g và vì thế là một iđêan lũy linh của g.

(3) Mọi dạng tuyến tính $\lambda$ trên g bằng không trên $\mathcal{D}g$ là một biểu diễn đơn (với không gian K) của g, do đó $\lambda(s) = \{0\}$. Suy ra $s \subset \mathcal{D}g$. Mặt khác, s được chứa trong căn r của g theo Nhận xét 2. Ta sẽ chứng minh rằng $s = r \cap \mathcal{D}g$.

#### Bổ đề 1 {#lie-i-s5-lem-1 .statement}

Cho V là một không gian vectơ hữu hạn chiều trên K, g là một đại số con của gl(V) sao cho V là một g-môđun đơn và a là một iđêan giao hoán của g. Khi đó $a \cap \mathcal{D}g = \{0\}$. Cho S là đại số con của $\mathcal{L}(V)$ sinh bởi 1 và a.

Nếu b là một iđêan của g được chứa trong a sao cho $\operatorname{Tr} bs = 0$ với mọi $b \in b$ và mọi $s \in S$, thì đặc biệt, theo định nghĩa của S, $\operatorname{Tr}(b^n) = 0$ với mọi số nguyên $n > 0$ và do đó b là lũy linh (Đại số, Chương VII, § 5, no. 5, Hệ quả 4 của Mệnh đề 13); vì mọi phần tử của b đều lũy linh, $b = \{0\}$ (§ 4, no. 3, Bổ đề 2). Trước hết ta áp dụng điều này cho iđêan $[g, a]$ của g. Nếu $x \in g, a \in a, s \in S$, thì $\operatorname{Tr}[x, a]s = \operatorname{Tr}(xas - axs) = \operatorname{Tr} x(as - sa) = 0$ vì $as = sa$; do đó $[g, a] = \{0\}$. Vậy các phần tử của g giao hoán với các phần tử của a và do đó cũng giao hoán với các phần tử của S. Nếu $x, y$ thuộc g và $s \in S$, thì

$$
\operatorname{Tr}[x, y]s = \operatorname{Tr}(xys - yxs) = \operatorname{Tr} x(ys - sy) = 0
$$

vì $ys = sy$; khi đó lấy b là iđêan $\mathcal{D}g \cap a$, suy ra $\mathcal{D}g \cap a = \{0\}$.

#### Định lý 1 {#lie-i-s5-thm-1 .statement}

Cho g là một đại số Lie, r là căn của nó và s là căn lũy linh của nó. Khi đó $s = \mathcal{D}g \cap r$.

Ta đã biết rằng $s \subset \mathcal{D}g \cap r$. Vì thế, chỉ cần chứng minh rằng nếu $\rho$ là một biểu diễn đơn hữu hạn chiều của g thì $\rho(\mathcal{D}g \cap r) = \{0\}$. Gọi k là số nguyên nhỏ nhất $\geq 0$ sao cho $\rho(\mathcal{D}^{k+1}r) = \{0\}$; đặt $g' = \rho(g)$, $a' = \rho(D^k r)$; vì $\mathcal{D}^k r$ là một iđêan của g nên $a'$ là một iđêan của $g'$; iđêan này là giao hoán vì $\rho(\mathcal{D}^{k+1}r) = \{0\}$. Nếu V là không gian của $\rho$, thì $g' \subset \operatorname{gl}(V)$ và V là một $g'$-môđun đơn. Khi đó $\rho(\mathcal{D}g \cap \mathcal{D}^k r) \subset \mathcal{D}g' \cap a' = \{0\}$. Nếu $k > 0$, thì $\mathcal{D}^k r \subset \mathcal{D}g$ và $\rho(\mathcal{D}^k r) = \{0\}$, trái với định nghĩa của k. Vậy $k = 0$, nghĩa là

$$
\rho(\mathcal{D}g \cap r) = \{0\}.
$$

#### Hệ quả 1 {#lie-i-s5-thm-1-cor-1 .statement}

Cho g là một đại số Lie giải được. Căn lũy linh của g là $\mathcal{D}g$. Nếu $\rho$ là một biểu diễn đơn hữu hạn chiều của g thì $\rho(g)$ là giao hoán và đại số kết hợp L sinh bởi 1 và $\rho(g)$ là một trường bậc hữu hạn trên K.

Ở đây $r = g$, do đó $s = \mathcal{D}g$. Vì thế $\varphi(\mathcal{D}g) = \{0\}$, điều đó chứng tỏ rằng $g' = \rho(g)$ là giao hoán. Mọi phần tử $\neq 0$ của $L$ đều khả nghịch theo Bổ đề Schur; vậy $L$ là một trường.

**Hệ quả 2 (Định lý Lie).** *Cho $g$ là một đại số Lie giải được; giả sử rằng $K$ đóng đại số. Cho $M$ là một $g$-môđun có số chiều hữu hạn trên $K$ và cho $(M_i)_{0 \leq i \leq r}$ là một chuỗi Jordan-Hölder của $M$. Khi đó $M_{i-1}/M_i$ có chiều bằng 1 trên $K$ với $1 \leq i \leq r$ và, với mọi $x \in g$, $x_{M_{i-1}/M_i} = \lambda_i(x) \cdot 1$, trong đó $\lambda_i$ là một dạng tuyến tính trên $g$ triệt tiêu trên $\mathcal{D}g$. Đặc biệt, mọi $g$-môđun đơn có chiều hữu hạn trên $K$ thực ra đều có chiều bằng 1.*

Gọi $\rho_i$ là biểu diễn của $g$ trên $M_{i-1}/M_i$. Đại số kết hợp $L_i$ sinh bởi 1 và $\rho_i(g)$ là một trường, một mở rộng hữu hạn của $K$ và do đó bằng $K$; và $M_{i-1}/M_i$ là một $L_i$-môđun đơn, do đó $\dim M_{i-1}/M_i = 1$. Phần còn lại của hệ quả là hiển nhiên.

#### Nhận xét {#lie-i-s5-n3-rem-2 .statement}

(1) Nếu $(M_i)_{0 \leq i \leq r}$ được thay bằng một chuỗi Jordan-Hölder khác của $M$, thì dãy $(\lambda_1, \ldots, \lambda_r)$ được thay bằng một dãy có dạng $(\lambda_{\pi(1)}, \ldots, \lambda_{\pi(r)})$, trong đó $\pi$ là một phép hoán vị của $\{1, \ldots, r\}$, như suy ra từ Định lý Jordan-Hölder.

(2) Cho $(e_1, \ldots, e_r)$ là một cơ sở của $M$ sao cho $e_i \in M_{i-1}, e_i \notin M_i$ ($1 \leq i \leq r$). Nếu $x \in g$ thì tự đồng cấu của $M$ tương ứng với $x$ được biểu diễn đối với cơ sở này bởi một ma trận tam giác mà các hệ số đường chéo là

$$
\lambda_1(x), \ldots, \lambda_r(x).
$$

#### Hệ quả 3 {#lie-i-s5-thm-1-cor-3 .statement}

*Giả sử rằng $K$ đóng đại số. Nếu $g$ là một đại số Lie giải được $r$-chiều, thì mọi iđêan của $g$ là một số hạng của một dãy giảm các iđêan có các chiều $r, r-1, \ldots, 0$.*

Mọi iđêan đều là một phần của một chuỗi Jordan-Hölder của $g$, được xét như không gian của biểu diễn phụ hợp (*Đại số*, Chương I, § 6, no. 14, Hệ quả của Định lý 8); khi đó chỉ cần áp dụng Hệ quả 2.

#### Hệ quả 4 {#lie-i-s5-thm-1-cor-4 .statement}

*Giả sử rằng $K = \mathbf{R}$. Cho $g$ là một đại số Lie giải được. Mọi biểu diễn đơn của $g$ đều có chiều $\leq 2$. Mọi iđêan của $g$ là một số hạng của một dãy giảm $(g_i)_{0 \leq i \leq m}$ các iđêan sao cho $g_0 = g, g_m = \{0\}, \dim g_{i-1}/g_i \leq 2$ ($1 \leq i \leq m$).

Điều này được chứng minh theo cách tương tự như đối với các Hệ quả 2 và 3, dùng sự kiện rằng mọi mở rộng đại số của $\mathbf{R}$ đều có bậc $\leq 2$.*

#### Hệ quả 5 {#lie-i-s5-thm-1-cor-5 .statement}

*Để một đại số Lie $g$ là giải được, điều kiện cần và đủ là $\mathcal{D}g$ lũy linh.*

Điều kiện đó là cần theo Hệ quả 1. Nó là đủ vì $g/\mathcal{D}g$ là giao hoán.

#### Hệ quả 6 {#lie-i-s5-thm-1-cor-6 .statement}

*Cho $\varphi$ là một biểu diễn hữu hạn chiều của một đại số Lie $g$. Cho* r là căn của g. Mọi phần tử $x \in r$ sao cho $\rho(x)$ lũy linh đều thuộc iđêan lũy linh lớn nhất $n$ của $\rho$.

Cho V là không gian của $\rho$; cho $(V_i)_{0 \leq i \leq r}$ là một chuỗi Jordan-Hölder đối với cấu trúc r-môđun trên V và cho $\rho_i$ là biểu diễn của r có không gian $V_i / V_{i-1}$ ($1 \leq i \leq r$). Nếu $\rho(x)$ lũy linh, thì $\rho_i(x)$ cũng vậy; vì với mọi $i$, đại số sinh bởi $\rho_i(x)$ là một trường, nên $\rho_i(x) = 0$. Ngược lại, nếu $\rho_i(x) = 0$ với mọi $i$, thì $\rho(x) = 0$. Điều này cho thấy rằng tập $a$ các $x \in r$ sao cho $\rho(x)$ lũy linh là một iđêan của r. Mặt khác, $[g, a] \subset \mathcal{D}g \cap r \subset n \cap r \subset a$ và do đó $a$ là một iđêan của g. Điều này chứng minh rằng $a \subset n$.

#### Hệ quả 7 {#lie-i-s5-thm-1-cor-7 .statement}

Cho g là một đại số Lie và r là căn của nó. Bốn tập hợp sau đây trùng nhau: (a) iđêan lũy linh lớn nhất của g; (b) iđêan lũy linh lớn nhất của r; (c) tập hợp các $x \in r$ sao cho $\mathrm{ad}_g x$ là lũy linh; (d) tập hợp các $x \in r$ sao cho $\mathrm{ad}_r x$ là lũy linh.

Ký hiệu các tập hợp này bởi $a, b, c, d$. Các bao hàm $a \subset b \subset d \subset c$ là hiển nhiên. $c \subset a$ theo Hệ quả 6 áp dụng cho biểu diễn liên hợp của g.

### 4. MỘT TIÊU CHUẨN CHO TÍNH GIẢI ĐƯỢC

#### Bổ đề 2 {#lie-i-s5-lem-2 .statement}

Cho $x$ là một tự đồng cấu của một không gian vectơ hữu hạn chiều V và s (tương ứng n) là thành phần nửa đơn (tương ứng lũy linh) của nó (xem Đại số, Chương VIII, § 9, no. 4, Định nghĩa 4). Cho $\mathrm{ad}\, x, \mathrm{ad}\, s, \mathrm{ad}\, n$ là các ảnh tương ứng của $x, s, n$ trong biểu diễn liên hợp của $\mathfrak{gl}(V)$. Khi đó $\mathrm{ad}\, s$ (tương ứng $\mathrm{ad}\, n$) là thành phần nửa đơn (tương ứng lũy linh) của $\mathrm{ad}\, x$ và bằng một đa thức theo $\mathrm{ad}\, x$ với các hệ số trong K và không có số hạng hằng.

Ta biết rằng $\mathrm{ad}\, x = \mathrm{ad}\, s + \mathrm{ad}\, n, [\mathrm{ad}\, s, \mathrm{ad}\, n] = 0$ và $\mathrm{ad}\, n$ là lũy linh ($§ 4$, Bổ đề 1). Ta sẽ chỉ ra rằng $\mathrm{ad}\, s$ là nửa đơn. Chỉ cần làm điều này khi K đóng đại số (xem Đại số, Chương VIII, § 9, no. 2, Mệnh đề 3). Khi đó, lấy $(e_i)_{1 \leq i \leq n}$ là một cơ sở của V sao cho $s(e_i) = \lambda_i e_i$ ($\lambda_i \in K$). Cho $(E_{ij})$ là cơ sở chính tắc của $M_n(K) = \mathfrak{gl}(V)$. Theo các công thức (5) của $§ 1$,

$$
(\mathrm{ad}\, s)\cdot E_{ij} = (\lambda_i - \lambda_j)E_{ij}
$$

và do đó $\mathrm{ad}\, s$ là nửa đơn. Khẳng định cuối cùng của bổ đề suy ra từ Đại số, Chương VIII, § 9, no. 4, Mệnh đề 8.

#### Bổ đề 3 {#lie-i-s5-lem-3 .statement}

Cho M là một không gian vectơ hữu hạn chiều, A và B là hai không gian vectơ con của $\mathfrak{gl}(M)$ sao cho $B \subset A$ và T là tập hợp các $t \in \mathfrak{gl}(M)$ sao cho $[t, A] \subset B$. Nếu $z \in T$ sao cho $\mathrm{Tr}(zu) = 0$ với mọi $u \in T$, thì $z$ là lũy linh.

Chỉ cần chứng minh điều này khi K đóng đại số, và từ đây về sau ta sẽ giả thiết như vậy. Cho s và n là các thành phần nửa đơn và lũy linh của z và cho $(e_i)$ là một cơ sở của M sao cho $s(e_i) = \lambda_i e_i$ ($\lambda_i \in K$). Cho $V \subset K$ là không gian vectơ trên $\mathbf{Q}$ sinh bởi các $\lambda_i$. Ta cần chứng minh rằng $V = \{0\}$. Cho f là một dạng tuyến tính $\mathbf{Q}$-tuyến tính trên V và cho t là tự đồng cấu của M sao cho

$te_i = f(\lambda_i)e_i$. Nếu $(E_{ij})$ là cơ sở chính tắc của $\mathfrak{gl}(M)$ được xác định bởi $E_{ij}e_k = \delta_{jk}e_i$, thì
$$
\begin{align*}
(\mathrm{ad}\ s)E_{ij} &= (\lambda_i - \lambda_j)E_{ij} \\
(\mathrm{ad}\ t)E_{ij} &= (f(\lambda_i) - f(\lambda_j))E_{ij}.
\end{align*}
$$

Tồn tại một đa thức P không có số hạng hằng và có các hệ số trong K sao cho $P(\lambda_i - \lambda_j) = f(\lambda_i) - f(\lambda_j)$ với mọi i và j (thật vậy, nếu $\lambda_i - \lambda_j = \lambda_h - \lambda_k$, thì $f(\lambda_i) - f(\lambda_j) = f(\lambda_h) - f(\lambda_k)$ và, nếu $\lambda_i - \lambda_j = 0$, thì $f(\lambda_i) - f(\lambda_j) = 0$). Khi đó $\mathrm{ad}\ t = P(\mathrm{ad}\ s)$. Mặt khác, $\mathrm{ad}\ s$ là một đa thức không có số hạng hằng theo $\mathrm{ad}\ z$. Bây giờ $(\mathrm{ad}\ z)(A) \subset B$, do đó cũng có $(\mathrm{ad}\ t)(A) \subset B$. Theo giả thiết $0 = \mathrm{Tr}(zt) = \sum \lambda_i f(\lambda_i)$, do đó $0 = f(\mathrm{Tr}(zt)) = \sum f(\lambda_i)^2$. Vì các $f(\lambda_i)$ là những số hữu tỉ, suy ra $f = 0$, điều này hoàn tất chứng minh.

#### Định lý 2 (tiêu chuẩn của Cartan) {#lie-i-s5-thm-2 .statement}

*Cho g là một đại số Lie, M là một không gian vectơ hữu hạn chiều, ρ là một biểu diễn của g trên M và β là dạng song tuyến tính trên g liên kết với ρ. Khi đó ρ(g) là giải được khi và chỉ khi 𝒟g trực giao với g đối với β.*

Hiển nhiên có thể quy về trường hợp g là một đại số con Lie của $\mathfrak{gl}(M)$ và ρ là ánh xạ đồng nhất. Nếu g giải được, 𝒟g được chứa trong iđêan lũy linh lớn nhất của biểu diễn đồng nhất của g (Định lý 1) và vì thế trực giao với g đối với β (§ 4, Mệnh đề 4 (d)). Giả sử rằng 𝒟g trực giao với g đối với β. Ta chứng minh rằng g giải được. Gọi T là tập hợp các $t \in \mathfrak{gl}(M)$ sao cho $[t, g] \subset \mathscr{D}g$. Nếu $t \in T$ và x, y thuộc g, thì $[t, x] \in \mathscr{D}g$ và do đó
$$
\mathrm{Tr}(t[x, y]) = \beta([t, x], y) = 0
$$
do đó theo tính tuyến tính $\mathrm{Tr}(tu) = 0$ với mọi $u \in \mathscr{D}g$. Ngoài ra, rõ ràng $\mathscr{D}g \subset T$. Vậy nên (Bổ đề 3) mọi phần tử của 𝒟g đều lũy linh. Suy ra 𝒟g là lũy linh (§ 4, Hệ quả 3 của Định lý 1) và vì thế g là giải được (no. 3, Hệ quả 5 của Định lý 1).

### 5. CÁC TÍNH CHẤT BỔ SUNG CỦA CĂN

#### Mệnh đề 5 {#lie-i-s5-prop-5 .statement}

*Cho g là một đại số Lie và r là căn của nó.*
(a) *Nếu ρ là một biểu diễn hữu hạn chiều của g và β là dạng song tuyến tính liên kết, thì r và 𝒟g trực giao đối với β.*
(b) *r là trực giao của 𝒟g đối với dạng Killing.*
Cho x, y thuộc g, $z \in r$. Khi đó $[y, z] \in \mathscr{D}g \cap r$ và do đó
$$
\beta([x, y], z) = \beta(x, [y, z]) = 0
$$
(Định lý 1). Suy ra (a).
Gọi r' là trực giao của 𝒟g đối với dạng Killing. Nó là một iđêan của g (§ 3, no. 6, Mệnh đề 7 (a)) chứa r theo điều trên. Mặt khác, ảnh s của r' dưới biểu diễn kề của g là giải được (Định lý 2) và vì thế r' là giải được vì là một mở rộng trung tâm của s. Suy ra r' ⊂ r.

#### Hệ quả 1 {#lie-i-s5-prop-5-cor-1 .statement}

Cho g là một đại số Lie. Khi đó g giải được khi và chỉ khi $\mathcal{D}g$ trực giao với g đối với dạng Killing.

Đây là một hệ quả ngay lập tức của Mệnh đề 5 (b).

#### Hệ quả 2 {#lie-i-s5-prop-5-cor-2 .statement}

Căn r của một đại số Lie g là một iđêan đặc trưng.

$\mathcal{D}g$ là một iđêan đặc trưng và dạng Killing là hoàn toàn bất biến (§ 3, no. 6, Mệnh đề 10). Do đó trực giao của $\mathcal{D}g$ đối với dạng Killing là một iđêan đặc trưng (§ 3, no. 6, Mệnh đề 7 (b)).

#### Hệ quả 3 {#lie-i-s5-prop-5-cor-3 .statement}

Cho g là một đại số Lie, r là căn của nó và a là một iđêan của g. Khi đó căn của a bằng $r \cap a$.

r ∩ a là một iđêan giải được của a và do đó được chứa trong căn r' của a. Ngược lại, r' là một iđêan của g (Hệ quả 2 và § 1, no. 4, Mệnh đề 2) và do đó r' ⊂ r.

Hệ quả 2 có thể được làm chính xác hơn như sau:

#### Mệnh đề 6 {#lie-i-s5-prop-6 .statement}

Cho g là một đại số Lie, r là căn của nó và n là iđêan lũy linh lớn nhất của nó. Mọi đạo hàm của g đều ánh xạ r vào n.

Cho D là một đạo hàm của g. Gọi g' = g + Kx_0 là một đại số Lie trong đó g là một iđêan đồng chiều 1 sao cho Dx = [x_0, x] với mọi x ∈ g (§ 1, no. 8, Ví dụ 1). Theo Hệ quả 3 của Mệnh đề 5, r được chứa trong căn r' của g'. Khi đó D(r) = [x_0, r] ⊂ [g', g'] ∩ r' = s'. Với mọi x ∈ s', ad_{g'} x là lũy linh (Định lý 1). Do đó, với mọi x ∈ s' ∩ g, ad_g x là lũy linh. Vậy D(r) được chứa trong iđêan lũy linh s' ∩ g của g.

#### Hệ quả {#lie-i-s5-n5-cor-1 .statement}

Iđêan lũy linh lớn nhất của một đại số Lie là một iđêan đặc trưng.

#### Nhận xét {#lie-i-s5-n5-rem-1 .statement}

Để tóm tắt một số kết quả trên đây, chú ý rằng, nếu r, n, s, t lần lượt ký hiệu căn của g, iđêan lũy linh lớn nhất của g, căn lũy linh của g và trực giao của g đối với dạng Killing, thì

$$
r \supset t \supset n \supset s.
$$

Bao hàm thức r ⊃ t suy ra từ Mệnh đề 5 (b). Bao hàm thức t ⊃ n suy ra từ § 4, no. 4, Mệnh đề 6 (b). Bao hàm thức n ⊃ s đã được chỉ ra trong Nhận xét 2 của no. 3.

### 6. MỞ RỘNG TRƯỜNG CƠ SỞ

Cho g là một đại số Lie trên K và K_1 là một mở rộng của K. Rõ ràng g_{(K_1)} là giải được khi và chỉ khi g giải được, vì $\mathcal{D}^n(g_{(K_1)}) = (\mathcal{D}^n g)_{(K_1)}$.

Cho r là căn của g. Khi đó $r_{(K_1)}$ *là căn của* $g_{(K_1)}$. Thật vậy, gọi $\beta$ là dạng Killing của g. Vì r là trực giao của $\mathcal{D}g$ đối với $\beta$ (Mệnh đề 5 (b)), $r_{(K_1)}$ là trực giao của $(\mathcal{D}g)_{(K_1)} = \mathcal{D}(g_{(K_1)})$ đối với dạng suy ra từ $\beta$ bằng cách mở rộng từ K lên $K_1$, tức là dạng Killing của $g_{(K_1)}$ (§ 3, no. 8). Khi đó mệnh đề của chúng ta suy ra từ một lần áp dụng nữa của Mệnh đề 5 (b).

### Bài tập {#lie-i-s5-exercises}

Các quy ước của § 5 vẫn còn hiệu lực trừ khi có nói khác.

Xem [các bài tập cho § 5](exercises/s5/).
