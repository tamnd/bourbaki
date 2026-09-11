---
book: ts
book_title: Théories spectrales
chapter: IV
chapter_title: THÉORIE SPECTRALE HILBERTIENNE
section: 3
section_title: Distributions et distributions tempérées
lang: vi
source: ts-iii-v-fr
book_pages: TS IV.196-TS IV.223, TS IV.330-TS IV.344
pdf_pages: 0209-0236, 0343-0357
extraction: native
subsections:
    - "no": 1
      title: Dérivation sous le signe somme
      page: 197
      pdf_page: 210
    - "no": 2
      title: Critères d’intégrabilité dans R$^n$ et Z$^n$
      page: 199
      pdf_page: 212
    - "no": 3
      title: Fonctions test
      page: 200
      pdf_page: 213
    - "no": 4
      title: Distributions
      page: 203
      pdf_page: 216
    - "no": 5
      title: Interprétation de fonctions comme distributions
      page: 206
      pdf_page: 219
    - "no": 6
      title: Dérivation des distributions
      page: 208
      pdf_page: 221
    - "no": 7
      title: Fonctions de Schwartz
      page: 209
      pdf_page: 222
    - "no": 8
      title: Inclusions d’espaces fonctionnels dans l’espace des fonctions de Schwartz
      page: 212
      pdf_page: 225
    - "no": 9
      title: Fonctions à croissance polynomiale
      page: 214
      pdf_page: 227
    - "no": 10
      title: Distributions tempérées
      page: 214
      pdf_page: 227
    - "no": 11
      title: Interprétation de fonctions comme distributions tempérées
      page: 216
      pdf_page: 229
    - "no": 12
      title: Transformation de Fourier des distributions tempérées
      page: 217
      pdf_page: 230
    - "no": 13
      title: Distributions et distributions tempérées sur un espace vectoriel
      page: 221
      pdf_page: 234
    - "no": 14
      title: Espaces de Sobolev
      page: 221
      pdf_page: 234
statements: 46
exercises: 33
content_sha256: 805ac956a27110771f8647319e68a618430ba2ff8a3d10aa0716fbffa1dac3fd
translated_from: content/en-mt/ts/IV/03_s3_distributions_et_distributions_temperees.md
source_lang: en-mt
translation_method: machine
source_content_sha256: 83403e096a36131af4fc93cdae5fe789686d4fc6631978a38c0948a981a7d65d
translation_model: gpt-5.4
translation_run: translate-vi-44ca7555
glossary_version: 34
glossary_terms_sha256: 44cc380b4163badd91380a30b5d6a8f3db04722c9da0182208cddae00ec6f3ac
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 3. PHÂN BỐ VÀ PHÂN BỐ ÔN HÒA

Trong đoạn này, $n$ chỉ một số tự nhiên. Chúng tôi sẽ ký hiệu bởi $\mu$ độ đo Lebesgue trên $\mathbf{R}^n$, cũng như hạn chế của nó trên mọi tập compact địa phương của $\mathbf{R}^n$.

Chúng tôi ký hiệu

$$
x\cdot y=\sum_{i=1}^nx_iy_i
$$

tích vô hướng trên không gian Euclid $\mathbf{R}^n$; chuẩn Euclid được ký hiệu bởi $x\mapsto  \|x\|$ (TG, VI, p. 7). Ta nhắc lại rằng nhóm $\mathbf{R}^n$ đối ngẫu với chính nó đối với ánh xạ $(x, y)\mapsto$ exp(2$i\pi  x\cdot y$) và khi đó độ đo đối ngẫu của độ đo Lebesgue được đồng nhất với độ đo Lebesgue (hệ quả 3 của II, p. 236). Chúng tôi ký hiệu bởi $\mathscr{F}$ (tương ứng $\overline{\mathscr{F}}$) biến đổi Fourier (tương ứng phản biến đổi Fourier) của $\mathbf{R}^n$ (cf. n$^o9$ của II, p. 237).

Với mọi $\alpha = (\alpha_i)_{1\leqslant i\leqslant n}\in \mathbf{N}^n$, chúng tôi sẽ ký hiệu bởi $X^{\alpha}$ hàm từ $\mathbf{R}^n$

vào $\mathbf{R}$ được xác định bởi $x= (x_i)_{1\leqslant i\leqslant n}\mapsto x^{\alpha}=\prod_{i=1}^nx^{\alpha_i}_i$.

Cho $\alpha$ và $\beta$ là các phần tử của $\mathbf{N}^n$. Chúng tôi ký hiệu

$$
^n(\alpha )^n(\alpha_i)
$$

$$
|\alpha |=\sum\alpha_i,=\prod
$$

$$
\beta \beta_i
$$

$i=1i=1$

#### Bổ đề 1 {#ts-iv-s3-lem-1 .statement tag=030C}

Cho U là một tập mở của $\mathbf{R}^n$.

a) Cho K là một tập con compact của U và V là một lân cận mở của K trong U. Tồn tại một hàm $\varphi \in \mathscr{C}^{\infty}(U)$ có giá compact được chứa trong V sao cho $0\leqslant \varphi \leqslant 1$ và sao cho $\varphi (x) = 1$ với mọi $x\in K$;

b) Với mọi phủ mở hữu hạn địa phương của U, tồn tại một phân hoạch đơn vị gồm các hàm thuộc lớp $C^{\infty}$ phụ thuộc vào nó.

Điều này suy ra từ VAR, R1, p. 40, 5.3.6.

#### Mệnh đề 1 {#ts-iv-s3-prop-1 .statement tag=030D}

Cho U là một tập mở của $\mathbf{R}^n$ và $k\in \mathbf{N}$. Cho E, F và G là các không gian vectơ tôpô và cho $b: E\times F\rightarrow G$ là một ánh xạ song tuyến tính liên tục. Cho $f$ và $g$ là các hàm thuộc lớp $C^k$ từ U vào E và F tương ứng. Khi đó ánh xạ $h:x\mapsto b(f(x), g(x))$ thuộc lớp $C^k$ trên U; hơn nữa, với mọi $\alpha \in \mathbf{N}^n$ sao cho $|\alpha |\leqslant k$ và với mọi $x\in U$, ta có

$$
\alpha (\alpha )\beta \alpha -\beta
$$

$$
\partial h(x) =\sum b(\partial f(x), \partial g(x))
$$

$$
_{\beta\in\mathbf{N}^n}\beta
$$

$\beta \leqslant \alpha$

Ánh xạ $h$ là hợp thành của ánh xạ $(f, g) : U\rightarrow E\times F$, thuộc lớp $C^k$, và của ánh xạ $b: E\times F\rightarrow G$ thuộc lớp $C^{\infty}$. Do đó nó thuộc lớp $C^k$. Biểu thức các đạo hàm riêng của nó suy ra từ công thức Leibniz (FVR, I, p. 28, mệnh đề 2, cf. A, III, p. 122, hệ quả).

Ta nhắc lại rằng một không gian vectơ tôpô lồi địa phương tách được là một không gian Montel nếu nó bị chặn-thùng và nếu mọi tập bị chặn đều compact tương đối (EVT, IV, p. 18, đn. 4).

Ta cũng nhắc lại rằng nếu E và F là các không gian lồi địa phương, và nếu E là bornological (EVT, III, p. 12, đn. 1), thì một ánh xạ tuyến tính $u: E\rightarrow F$ là liên tục khi và chỉ khi ảnh qua $u$ của mọi tập con bị chặn của E đều bị chặn trong F (EVT, III, p. 11, mệnh đề 1, (iiibis), khi F là nửa chuẩn, trường hợp tổng quát suy ra hình thức từ điều này, cf. EVT, II, p. 7, mệnh đề 5, b)).

### 1. Đạo hàm dưới dấu tổng

Cho X là một không gian tôpô compact địa phương và $\nu$ một độ đo trên X. Cho E là một không gian Banach.

#### Mệnh đề 2 {#ts-iv-s3-prop-2 .statement tag=030E}

Cho I là một khoảng của $\mathbf{R}$ và $f$ một ánh xạ từ $X\times I$ vào E sao cho

(i) Với mọi $t\in I$, ánh xạ $x\mapsto f(x, t)$ từ X vào E là $\nu$-khả tích;

(ii) Với mọi $x\in X$, ánh xạ $t\mapsto f(x, t)$ từ I vào E có đạo hàm, được ký hiệu bởi $t\mapsto f'(x, t)$;

(iii) Tồn tại một hàm dương $\nu$-khả tích $g$ trên X sao cho $\|f'(x, t)\|\leqslant g(x)$ với mọi $(x, t)\in X\times I$.

Khi đó ánh xạ F từ I vào E được xác định bởi

$$
F(t) =\int_Xf(x, t)d\nu (x)
$$

là khả vi trên I, và với mọi $t\in I$, ta có

$$
F'(t) =\int_Xf'(x, t)d\nu (x)
$$

Cho $t_0\in I$ và gọi J là một khoảng của $\mathbf{R}$ được chứa trong I và là một lân cận của $t_0$ trong I. Gọi $h: X\times J\rightarrow E$ là ánh xạ được xác định bởi $(x, t)\mapsto (f(x, t)-f(x, t_0))/(t-t_0)$ với $(x, t)\in X\times (J-\{t_0\})$ và $(x, t_0)\mapsto f'(x, t_0)$ với $x\in X$. Cho $x\in X$. Ta có $\|h(x, t_0)\|\leqslant g(x)$ và, với mọi $t\not =t_0$, ta có $\|h(x, t)\|\leqslant g(x)$ theo FVR, I, p. 23, định lý 2. Theo định nghĩa của đạo hàm, mệnh đề suy ra từ hệ quả 1 của INT, IV, p. 144, § 4, n$^o3$, áp dụng cho ánh xạ $h$.

Ta lấy lại ký hiệu của VAR, R1, 2.4, p. 19 liên quan đến các đạo hàm riêng.

#### Hệ quả 1 {#ts-iv-s3-prop-2-cor-1 .statement tag=030F}

Cho U là một tập mở của $\mathbf{R}^n$. Cho $k\in \mathbf{N}$ và $f$ là một ánh xạ từ $X\times U$ vào E thỏa mãn các điều kiện sau:

(i) Với mọi $t\in U$, ánh xạ $x\mapsto f(x, t)$ từ X vào E là $\nu$-khả tích;

(ii) Với mọi $x\in X$, ánh xạ $t\mapsto f(x, t)$ từ U vào E thuộc lớp $C^k$, với các đạo hàm riêng được ký hiệu bởi $\partial^{\alpha}f(x, t)$ với mọi $\alpha \in \mathbf{N}^n$ sao cho $|\alpha |\leqslant k$;

(iii) Tồn tại một hàm $\nu$-khả tích $g$ trên X sao cho với mọi $\alpha \in \mathbf{N}^n$ thỏa mãn $|\alpha |\leqslant k$ và với mọi $(x, t)\in X\times U$, ta có $\|\partial^{\alpha}f(x, t)\|\leqslant g(x)$.

Khi đó ánh xạ F từ U vào E được xác định bởi

$$
F(t) =\int_Xf(x, t)d\nu (x)
$$

thuộc lớp $C^k$ trên U, và với mọi $\alpha \in \mathbf{N}^n$ thỏa mãn $|\alpha |\leqslant k$ và mọi $t\in U$, ta có

$$
\partial^{\alpha}F(t) =\int_X\partial^{\alpha}f(x, t)d\nu (x)
$$

Điều này suy ra từ mệnh đề bằng quy nạp theo $k$.

#### Hệ quả 2 {#ts-iv-s3-prop-2-cor-2 .statement tag=030G}

Cho $k$ là một số tự nhiên. Cho $f\in \mathscr{L}^1(\mathbf{R}^n, \mu)$ và $g\in \mathscr{C}^k(\mathbf{R}^n)$. Giả sử rằng với mọi $\alpha \in \mathbf{N}^n$ sao cho $|\alpha |\leqslant k$, hàm $\partial^{\alpha}g$ bị chặn. Khi đó tích chập $f*g$ thuộc $\mathscr{C}^k(\mathbf{R}^n)$ và với mọi $\alpha$ sao cho $|\alpha |\leqslant k$, ta có $\partial^{\alpha}(f*g) =f*\partial^{\alpha}g$.

Có thể áp dụng hệ quả 1 cho không gian $X =\mathbf{R}^n$, cho độ đo Lebesgue và cho ánh xạ $h$ được xác định bởi $(x, t)\mapsto f(x)g(t-x)$ từ $\mathbf{R}^n\times \mathbf{R}^n$ vào $\mathbf{C}$; thật vậy, với mọi $\alpha \in \mathbf{N}^n$ sao cho $|\alpha |\leqslant k$, ta có bất đẳng thức

$|\partial^{\alpha}h(x, t)|\leqslant ($sup$_{|\beta|\leqslant k}$ sup$_{y\in\mathbf{R}^n}|\partial^{\beta}g(y)|)|f(x)|$

mà vế phải là một hàm khả tích trên $\mathbf{R}^n$.

### 2. Các Tiêu Chuẩn Khả Tích trong R$^n$ và Z$^n$

#### Mệnh đề 3 {#ts-iv-s3-prop-3 .statement tag=030H}

Cho N là một chuẩn trên $\mathbf{R}^n,r$ là một số thực và $p\in [1,+\infty [$.

a) Hàm $(1 + N)^r$ thuộc $\mathscr{L}^p(\mathbf{R}^n, \mu)$ khi và chỉ khi $rp <-n$;

a$')$ Hạn chế lên $\mathbf{Z}^n$ của hàm $(1 + N)^r$ thuộc $\ell^p(\mathbf{Z}^n)$ khi và chỉ khi $rp <-n$;

b) Cho V là một lân cận đo được bị chặn của 0 trong $\mathbf{R}^n$. Hàm $N^r$ thuộc $\mathscr{L}^p(\mathbf{R}^n-V, \mu)$ khi và chỉ khi $rp <-n$.

Do tính tương đương của các chuẩn trên $\mathbf{R}^n$ (EVT I, p. 14, định lý 2 và TG, IX, p. 32, mệnh đề 8), ta có thể giả sử rằng chuẩn N được cho bởi $N(x) =$ sup$|x_i|$ với $x= (x_i)\in \mathbf{R}^n$. Ký hiệu B là quả cầu đơn vị của $\mathbf{R}^n$ đối với chuẩn này.

Cho V là một lân cận đo được bị chặn của 0 trong $\mathbf{R}^n$. Hàm $N^r$ liên tục và bị chặn trên (B- $V$)$\cup (V$- B), điều này cho thấy mệnh đề b) đúng khi và chỉ khi nó đúng với V = B, điều mà từ nay ta sẽ giả sử. Vì hàm $(1 + N)^r$ liên tục và bị chặn trên B, và thỏa mãn các bất đẳng thức $N^r\leqslant (1 + N)^r\leqslant 2^rN^r$ trên $\mathbf{R}^n-$ B, ta thấy rằng các mệnh đề a) và b) là tương đương.

Hãy chứng minh b) khi V = B. Ta có thể giả sử rằng $p= 1$. Vì trường hợp $r >0$ là sơ cấp, giả sử rằng $r\leqslant 0$. Với mọi số nguyên $j\geqslant 1$, tập hợp

$$
C_j=\{x\in \mathbf{R}^n|2^{j-1}\leqslant N(x)<2^j\}
$$

có độ đo bằng $2^{nj}(2^n-1)$. Các tập hợp $(C_j)_{j\geqslant 1}$ tạo thành một phân hoạch của $\mathbf{R}^n-$ B. Theo INT, V, p. 4, § 1, No.$^o1$, hệ quả, do đó ta có

$$
\int^*N^rd\mu=\sum\int^*N^rd\mu
$$

$\mathbf{R}^{n-}Bj\geqslant 1C_j$

$\leqslant \sum_{j\geqslant 1}2^{n+nj}2^{r(j-1)}= 2^{n-r}\sum_{j\geqslant 1}2^{(n+r)j}$ là hữu hạn nếu $r <-n$. Mặt khác, ta có (loc. cit.)

$$
\int^*N^rd\mu\geqslant \sum 2^{rj}2^{nj}(2^n-1) = (2^n-1)\sum 2^{(r+n)j}
$$

$\mathbf{R}^{n-}Bj\geqslant 1j\geqslant 1$

là vô hạn nếu $r\geqslant -n$.

Ta chứng minh a$')$ tương tự bằng cách xét các tập hợp $C_j\cap \mathbf{Z}^n$ phủ $\mathbf{Z}^n-\{0\}$ và thỏa mãn

Card(C$_j\cap \mathbf{Z}^n$) $= (2^{j+1}-1)^n-(2^j-1)^n$,

thuộc khoảng $[(1-2^{-n})(2^{j+1}-1)^n,2^{n(j+1)}]$.

### 3. Hàm thử

Trong số này, U chỉ một tập con mở của $\mathbf{R}^n$. Với $p\in [1,+\infty ]$, ta sẽ viết $\mathscr{L}^p(U)$ và $L^p(U)$ thay vì $\mathscr{L}^p(U, \mu)$ và $L^p(U, \mu)$. Ta đồng nhất các hàm liên tục thuộc $\mathscr{L}^p(U)$ với ảnh của chúng trong $L^p(U)$.

Hãy trang bị cho không gian $\mathscr{C}^{\infty}(U)$ các hàm phức khả vi vô hạn lần trên U tôpô được xác định bởi họ các nửa chuẩn $p_{\alpha ,K}$ xác định với $\alpha \in \mathbf{N}^n$ và $K\subset U$ bởi

$p_{\alpha ,K}(\varphi ) =$ sup$_{x\in K}|\partial^{\alpha}\varphi (x)|$.

Không gian này là đầy đủ (xem EVT, III, p. 9, ví dụ b)).

Với mọi tập con compắc K của U, ta ký hiệu bởi $\mathscr{C}_K^{\infty}(U)$ không gian con của $\mathscr{C}^{\infty}(U)$ tạo bởi các hàm có giá trong K. Không gian $\mathscr{C}_K^{\infty}(U)$ được trang bị tôpô cảm sinh bởi tôpô của $\mathscr{C}^{\infty}(U)$. Nó là một không gian Fréchet, một họ đếm được các nửa chuẩn xác định tôpô của nó là họ $(p_{\alpha ,K})_{\alpha\in\mathbf{N}^n}$. Đặc biệt, nó là một không gian bornological (EVT, III, p. 12, prop. 2).

Ta ký hiệu bởi $\mathscr{D}(U)$ không gian vectơ $\mathscr{K}(U)\cap \mathscr{C}^{\infty}(U)$ của các hàm lớp $C^{\infty}$ có giá compắc trong U. Ta nói rằng $\mathscr{D}(U)$ là không gian các hàm thử trên U. Không gian $\mathscr{D}(U)$ là giới hạn quy nạp của các không gian $\mathscr{C}_K^{\infty}(U)$ và được trang bị tôpô lồi địa phương giới hạn quy nạp tương ứng (EVT, II, p. 31).

Không gian này được ký hiệu bởi $\mathscr{C}_{\circ}^{\infty}(U)$ trong EVT, III, p. 9.

Cho $(K_m)$ là một dãy tăng các tập con compắc của U mà các phần trong của chúng tạo thành một phủ của U. Khi đó không gian $\mathscr{D}(U)$ là giới hạn quy nạp ngặt của các không gian $\mathscr{C}_{K_m}^{\infty}(U)$ (EVT, III, p. 9). Vì vậy nó là một không gian đầy đủ (EVT, II, p. 35, prop. 9). Mọi tập con bị chặn của $\mathscr{D}(U)$ đều được chứa trong một trong các không gian con $\mathscr{C}_{K_m}^{\infty}(U)$ (EVT, III, p. 5, prop. 6). Điều này có nghĩa là $B\subset \mathscr{D}(U)$ bị chặn nếu và chỉ nếu tồn tại một tập con compắc K của U và một họ $(M_{\alpha})_{\alpha\in\mathbf{N}^n}$ trong $\mathbf{R}_+$ sao cho B được chứa trong tập hợp các hàm $\varphi \in \mathscr{C}_K^{\infty}(U)$ thỏa mãn

$$
p_{\alpha ,K}(\varphi )\leqslant M_{\alpha}
$$

với mọi $\alpha \in \mathbf{N}^n$.

Không gian $\mathscr{D}(U)$ là một không gian bornological (EVT, III, p. 12, ví dụ 3) và một không gian Montel (EVT, IV, p. 18, ví dụ 4).

Cho V là một tập con mở của $\mathbf{R}^n$ được chứa trong U. Nếu $K\subset V$ là compắc, thì hạn chế các hàm lên V xác định một ánh xạ tuyến tính liên tục toàn ánh từ $\mathscr{C}_K^{\infty}(U)$ lên $\mathscr{C}_K^{\infty}(V)$. Mở rộng bởi không ngoài một hàm xác định trên V cảm sinh một ánh xạ tuyến tính liên tục đơn ánh, gọi là chính tắc, từ $\mathscr{D}(V)$ vào $\mathscr{D}(U)$.

#### Nhận xét {#ts-iv-s3-n3-rem-1 .statement tag=030I}

Người ta định nghĩa tương tự không gian $\mathscr{D}_{\mathbf{R}}(U)$ các hàm thử thực trị trên U. Ánh xạ tuyến tính sao cho $z\otimes \varphi \mapsto z\varphi$ với mọi $z\in \mathbf{C}$ và mọi $\varphi \in \mathscr{D}_{\mathbf{R}}(U)$ là một đẳng cấu của $\mathbf{C}\otimes \mathscr{D}_{\mathbf{R}}(U)$ lên $\mathscr{D}(U)$.

#### Bổ đề 2 {#ts-iv-s3-lem-2 .statement tag=030J}

Cho $\mathscr{U}$ là một phủ mở của U. Tồn tại một phủ mở hữu hạn địa phương của U mịn hơn $\mathscr{U}$ và được tạo thành từ các tập hợp tương đối compact.

Vì U là compact địa phương, tồn tại một phủ $\mathscr{V}$ của U mịn hơn $\mathscr{U}$ gồm các tập mở tương đối compact trong U. Vì U là paracompact (TG, IX, p. 51, đl. 4), tồn tại một phủ mở hữu hạn địa phương $\mathscr{W}$ mịn hơn $\mathscr{V}$. Khi đó $\mathscr{W}$ mịn hơn $\mathscr{U}$ và gồm các tập mở tương đối compact.

#### Bổ đề 3 {#ts-iv-s3-lem-3 .statement tag=030K}

Cho $f\in \mathscr{K}(\mathbf{R}^n)$ và cho V là một lân cận mở của giá K của $f$. Tồn tại một số nguyên $m_0\geqslant 1$ sao cho, với mọi $x\in K$, tập hợp V chứa quả cầu bán kính $m^{-1}_0$ có tâm tại $x$. Với mỗi số nguyên $m > m_0$, ký hiệu $V_m$ là quả cầu đóng bán kính $m^{-1}$ có tâm tại 0 trong $\mathbf{R}^n$ và ký hiệu $\varphi_m$ là một hàm thử có giá trong $V_m$, dương và có tích phân bằng 1. Đặt $f_m=\varphi_m*f$.

a) Ta có $f_m\in \mathscr{D}(\mathbf{R}^n)$ và giá của $f_m$ được chứa trong V ;

b) Cho $p\in [1,+\infty ]$. Dãy $(f_m)_{m>m_0}$ hội tụ tới $f$ trong $L^p(\mathbf{R}^n)$.

Theo TG, IX, p. 14, nhận xét, ta có $d(K,\mathbf{R}^n-V)>0$. Lấy một số nguyên $m_0\geqslant 1$ sao cho $m^{-1}_0< d(K,\mathbf{R}^n-$ V) ; nó thỏa mãn điều kiện cần có. Với mọi $m > m_0$, hàm $f_m$ liên tục (INT, VIII, p. 166, § 4, n$^o5$, mệnh đề 11) và có giá được chứa trong $K + V_m$ (INT, VIII, p. 126, § 1, n$^o4$, mệnh đề 5), do đó trong V. Theo Hệ quả 2 của IV, p. 198, ta có $f_m\in \mathscr{D}(\mathbf{R}^n)$. Nếu $p\not = +\infty$, thì dãy $(f_m)$ hội tụ tới $f$ trong $L^p(\mathbf{R}^n)$ (INT, VIII, p. 172, § 4, n$^o7$, mệnh đề 20).[^1]

Giả sử rằng $p= +\infty$. Cho $\varepsilon  >0$. Hàm $f$ liên tục đều trên $\mathbf{R}^n$, do đó tồn tại một số nguyên $m_1> m_0$ sao cho, với mọi $m\geqslant m_1$ và mọi $x\in \mathbf{R}^n$ và $y\in V_m$, ta có $|f(x)-f(x-y)|< \varepsilon$.

Với mọi $m\geqslant m_1$, hàm $\varphi_m$ triệt tiêu ở ngoài $V_m$, dương và có tích phân bằng 1. Do đó suy ra bất đẳng thức

$$
|f(x)-f_m(x)|=|\int_{\mathbf{R}^n}(f(x)-f(x-y))\varphi_m(y)d\mu(y)|\leqslant \varepsilon
$$

với mọi $x\in \mathbf{R}^n$, do đó suy ra kết quả.

#### Mệnh đề 4 {#ts-iv-s3-prop-4 .statement tag=030L}

a) Đơn ánh chính tắc của $\mathscr{D}(U)$ vào $\mathscr{K}(U)$ là liên tục và $\mathscr{D}(U)$ trù mật trong $\mathscr{K}(U)$;

b) Với mọi $p\in [1,+\infty [$, đơn ánh chính tắc của $\mathscr{D}(U)$ vào $\mathscr{L}^p(U)$ là liên tục và $\mathscr{D}(U)$ trù mật trong $L^p(U)$.

Mọi nửa chuẩn liên tục trên $\mathscr{K}(U)$ đều liên tục trên $\mathscr{D}$(U), do đó đơn ánh chính tắc của $\mathscr{D}(U)$ vào $\mathscr{K}(U)$ là liên tục.

Cho $f\in \mathscr{K}(U)$. Tồn tại một dãy $(f_m)_{m\in\mathbf{N}}$ trong $\mathscr{D}(U)$ hội tụ đều đến $f$ trên U và sao cho các giá của $f_m$ được chứa trong một lân cận tương đối compắc cố định của giá của $f$ (Bổ đề 3). Do đó dãy $(f_m)$ hội tụ đến $f$ trong $\mathscr{K}(U)$. Điều này kết thúc chứng minh của a).

Cho $p\in [1,+\infty [$. Cho $f\in \mathscr{D}(U)$ và K là giá của $f$. Khi đó ta có bất đẳng thức $N_p(f)\leqslant \mu(K)^{1/p}$ sup$_{x\in K}|f(x)|$, do đó đơn ánh chính tắc của $\mathscr{D}(U)$ vào $\mathscr{L}^p(U)$ là liên tục. Phần cuối của mệnh đề b) khi đó suy ra từ a).

Vì tích của hai hàm thử vẫn lại là một hàm thử, công thức Leibniz (FVR, I, p. 28, prop. 2) cho thấy rằng không gian $\mathscr{D}(U)$ là một đại số tôpô.

Nói chung hơn, cho $f\in \mathscr{C}^{\infty}(U)$. Khi đó ánh xạ tuyến tính $\varphi \mapsto f \varphi$ của $\mathscr{D}(U)$ vào $\mathscr{D}(U)$ là liên tục. Thật vậy, với mọi tập con compắc K của U và mọi $\alpha \in \mathbf{N}^n$, ta có

$$
(\alpha )
$$

$$
p_{\alpha ,K}(f \varphi )\leqslant \sum p_{\beta ,K}(f)p_{\alpha-\beta ,K}(\varphi )
$$

$$
\beta
$$

$0\leqslant \beta \leqslant \alpha$

(xem chỗ đã dẫn).

### 4. Phân phối

Ta giữ lại ký hiệu của số trước; do đó U chỉ một tập mở của $\mathbf{R}^n$.

#### Định nghĩa 1 {#ts-iv-s3-def-1 .statement tag=030M}

Không gian đối ngẫu của $\mathscr{D}(U)$, được trang bị tôpô của sự hội tụ bị chặn, được gọi là không gian các phân phối trên U. Nó được ký hiệu bởi $\mathscr{D}'(U)$.

Do đó, một phân phối trên U là một dạng tuyến tính liên tục trên $\mathscr{D}(U)$.

Nếu $f$ là một dạng tuyến tính trên $\mathscr{D}(U)$ (và đặc biệt nếu $f$ là một phân phối) và nếu $\varphi$ thuộc $\mathscr{D}$(U), thì ta sẽ ký hiệu bởi $\langle f, \varphi \rangle$ giá trị của $f$ tại $\varphi$.

Vì $\mathscr{D}(U)$ là bornological, không gian $\mathscr{D}'(U)$ là đầy đủ (EVT, III, p. 24, cor. 1). Vì $\mathscr{D}(U)$ là một không gian Montel, điều tương tự cũng đúng cho $\mathscr{D}'(U)$ (EVT, IV, p. 19, prop. 9). Đặc biệt, không gian $\mathscr{D}'(U)$ là phản xạ (EVT, IV, p. 16, th. 2).

#### Bổ đề 4 {#ts-iv-s3-lem-4 .statement tag=030N}

Cho $f$ là một ánh xạ tuyến tính từ $\mathscr{D}(U)$ vào $\mathbf{C}$. Khi đó $f$ là một phân phối nếu và chỉ nếu, với mọi tập con compắc K của U và mọi họ $(M_{\alpha})_{\alpha\in\mathbf{N}^n}$ trong $\mathbf{R}_+$, dạng tuyến tính $f$ bị chặn trên tập hợp các hàm $\varphi \in \mathscr{C}_K^{\infty}(U)$ sao cho, với mọi $\alpha \in \mathbf{N}^n$, ta có

sup$_{x\in K}|\partial^{\alpha}\varphi (x)|\leqslant M_{\alpha}$.

Thật vậy, không gian $\mathscr{D}(U)$ là bornological và mọi tập con bị chặn của $\mathscr{D}(U)$ đều được chứa trong một trong các tập bị chặn được mô tả trong mệnh đề.

#### Bổ đề 5 {#ts-iv-s3-lem-5 .statement tag=030O}

Cho $\mathfrak{F}$ là một bộ lọc trên $\mathscr{D}'(U)$ có một cơ sở đếm được hoặc chứa một tập hợp bị chặn đơn. Khi đó $\mathfrak{F}$ hội tụ đến một phân phối nếu và chỉ nếu $\langle f, \varphi \rangle$ hội tụ theo $\mathfrak{F}$ với mọi hàm thử $\varphi$ trên U.

Đặc biệt, một dãy $(f_m)_{m\in\mathbf{N}}$ các phân phối hội tụ đến một phân phối $f$ nếu và chỉ nếu, với mọi $\varphi \in \mathscr{D}(U)$, dãy $(\langle f_m, \varphi \rangle )_{m\in\mathbf{N}}$ hội tụ đến $\langle f, \varphi \rangle$.

Vì $\mathscr{D}'(U)$ là một không gian Montel, do đó là barrelled, điều này suy ra từ định lý Banach-Steinhaus (EVT, III, p. 26, cor. 3 of th. 1).

Cho V là một tập mở được chứa trong U. Chuyển vị của ánh xạ tuyến tính chính tắc từ $\mathscr{D}(V)$ vào $\mathscr{D}(U)$ là một ánh xạ tuyến tính liên tục từ $\mathscr{D}'(U)$ vào $\mathscr{D}'$(V), được gọi là hạn chế của các phân phối từ U xuống V và được ký hiệu bởi $r_{VU}$, hoặc đôi khi $r_{V,U}$.

Ta có $r_{VV}= 1_{\mathscr{D}'(V)}$. Nếu $W\subset V\subset U$ là các tập mở trong U, thì ta có $r_{WV}\circ r_{VU}=r_{WU}$. Nói cách khác, nếu $\mathscr{T}$ ký hiệu tôpô trên U, thì hệ xạ ảnh $\mathscr{D}'(U) = ((\mathscr{D}'(V))_{V\in\mathscr{T}},(r_{WV}))$ là một tiền bó trên U với giá trị trong Loài cấu trúc của các không gian vectơ tôpô lồi địa phương (TA, I, p. 42, def. 1 and p. 66, §10).

#### Mệnh đề 5 {#ts-iv-s3-prop-5 .statement tag=030P}

Tiền bó $\mathscr{D}'(U)$ là một bó.

Nhắc lại (TA, I, p. 43, def. 2) rằng điều đó có nghĩa là với mọi tập con mở V của U và mọi phủ mở $(V_i)_{i\in I}$ của V, các điều kiện sau được thỏa mãn:

(i) Ánh xạ $(r_{V_iV})_{i\in I}:\mathscr{D}'(V)\rightarrow \prod_{i\in I}\mathscr{D}'(V_i)$ là đơn ánh;

(ii) Với mọi họ $(f_i)\in \prod_{i\in I}\mathscr{D}'(V_i)$ sao cho

$$
r_{(V_i\cap V_{i'})V_i}(f_i) =r_{(V_i\cap V_{i'})V_{i'}}(f_{i'})
$$

với mọi cặp $(i, i')\in I\times I$, tồn tại một phân phối $f\in \mathscr{D}'(V)$ sao cho với mọi $i\in I$, ta có $r_{V_iV}(f) =f_i$.

Cho V là một tập mở của U và $\mathscr{V}= (V_i)_{i\in I}$ một phủ mở của V. Cho $(W_j)_{j\in J}$ là một phủ mở hữu hạn địa phương của V, mịn hơn $\mathscr{V}$ và gồm các tập con tương đối compắc (bổ đề 2 của IV, p. 201). Cố định một phân hoạch đơn vị $(\varphi_j)_{j\in J}$ phụ thuộc vào phủ $(W_j)_{j\in J}$ sao cho giá của $\varphi_j$ được chứa trong $W_j$ với mọi $j\in J$ (bổ đề 1 của IV, p. 196).

Cho $\varphi \in \mathscr{D}(V)$. Vì tập hợp các $j\in J$ sao cho $W_j$ giao với giá của $\varphi$ là hữu hạn (TG, I, §9, n$^o1$, p. 59), ta có

$$
\varphi =\sum_{j\in J}\varphi \varphi_j
$$

trong đó tổng chỉ gồm một số hữu hạn số hạng khác không.

Ta chứng minh (i). Giả sử rằng $f\in \mathscr{D}'(V)$ thỏa mãn $r_{V_iV}(f) = 0$ với mọi $i\in I$. Điều đó có nghĩa là $\langle f, \varphi \rangle = 0$ với mọi hàm thử $\varphi$ mà giá của nó được chứa trong một trong các tập mở $V_i$. Điều này a fortiori cũng đúng nếu giá của $\varphi$ được chứa trong một trong các tập mở $W_j$. Nhưng khi đó, với mọi $\varphi \in \mathscr{D}$(V), ta có

$$
\langle f, \varphi \rangle =\langle f,\sum_{j\in J}\varphi \varphi_j\rangle =\sum_{j\in J}\langle f, \varphi \varphi_j\rangle = 0
$$

do đó $f= 0$.

Ta chứng minh (ii). Cho $(f_i)_{i\in I}$ là một họ sao cho $f_i\in \mathscr{D}'(V_i)$ với mọi $i\in I$ và $r_{V_i\cap V_{i'},V_i}(f_i) =r_{V_i\cap V_{i'},V_{i'}}(f_{i'})$ với mọi $i$ và $i'$ trong I. Cho $\iota : J\rightarrow I$ là một ánh xạ sao cho $W_j\subset V_{\iota(j)}$ với mọi $j\in J$. Với mọi $j\in J$, đặt $\widetilde{f}_j=r_{W_j,V_{\iota(j)}}(f_{\iota(j)})$. Khi đó ta có

$$
r_{W_j\cap W_{j'},W_j}(\widetilde{f}_j) =r_{W_j\cap W_{j'},W_j}(r_{W_j,V_{\iota(j)}}(f_{\iota(j)}))
$$

$$
=r_{W_j\cap W_{j'},V_{\iota(j)}}(f_{\iota(j)})
$$

$$
=r_{W_j\cap W_{j'},V_{\iota(j)}\cap V_{\iota(j')}}\circ r_{V_{\iota(j)}\cap V_{\iota(j')},V_{\iota(j)}}(f_{\iota(j)})
$$

Đổi vai trò của $j$ và $j'$ và nhận thấy rằng

$$
r_{V_{\iota(j)}\cap V_{\iota(j')},V_{\iota(j)}}(f_{\iota(j)}) =r_{V_{\iota(j)}\cap V_{\iota(j')},V_{\iota(j')}}(f_{\iota(j')})
$$

theo giả thiết, ta suy ra rằng

$$
r_{W_j\cap W_{j'},W_j}(\widetilde{f}_j) =r_{W_j\cap W_{j'},W_j}(\widetilde{f}_{j'}) \tag{1}
$$

với mọi $(j, j')\in J^2$.

Với $\varphi \in \mathscr{D}$(V), đặt

$$
\lambda (\varphi ) =\sum_{j\in J}\langle \widetilde{f}_j, \varphi \varphi_j|W_j\rangle
$$

trong đó tổng là hữu hạn vì chỉ có một số hữu hạn số hạng có thể khác không.

Ánh xạ $\lambda$ là một dạng tuyến tính trên $\mathscr{D}(V)$. Ta chứng minh rằng nó là một phân phối. Cho B là một tập con bị chặn của $\mathscr{D}(V)$ và cho K là một tập compact của V sao cho $B\subset \mathscr{C}_K^{\infty}(V)$. Theo TG, I, §9, n$^o1$, p. 59, tồn tại một tập con hữu hạn $J'$ của J sao cho

$$
\lambda (\varphi ) =\sum_{j\in J'}\langle \widetilde{f}_j, \varphi \varphi_j|W_j\rangle
$$

với mọi $\varphi \in B$. Vì $\widetilde{f}_j$ là một phân phối với mọi $j\in J'$ và $\mathscr{D}(V)$ là một đại số tôpô, ta suy ra rằng $\lambda$ bị chặn trên B, do đó có kết quả (bổ đề 4).

Cho $j\in J$ và cho $\varphi \in \mathscr{D}(V)$ mà giá của nó được chứa trong $W_j$. Khi đó ta có

$$
\langle \lambda , \varphi \rangle =\sum_{j'\in J}\langle \widetilde{f}_{j'}, \varphi \varphi_{j'}|W_j\rangle =\sum_{j'\in J}\langle \widetilde{f}_j, \varphi \varphi_{j'}|W_j\rangle
$$

theo (1), vì $\varphi \varphi_{j'}$ có giá được chứa trong $W_j\cap W_{j'}$. Do đó

$$
\langle \lambda , \varphi \rangle =\langle \widetilde{f}_j,\sum_{j'\in J}\varphi \varphi_{j'}|W_j\rangle =\langle \widetilde{f}_j, \varphi |W_j\rangle
$$

do đó $r_{W_jV}(\lambda ) =\widetilde{f}_j$ với mọi $j\in J$.

Cho $i\in I$. Cuối cùng, ta hãy chỉ ra rằng hạn chế của $\lambda$ lên $V_i$ trùng với $f_i$. Theo điều kiện (i), áp dụng cho phủ của $V_i$ bởi các tập mở $W_j$, chỉ cần kiểm tra rằng với mọi $j\in J$, hạn chế của $\lambda$ lên $V_i\cap W_j$ trùng với hạn chế của $f_i$. Theo điều đã đi trước, vấn đề là kiểm tra rằng hạn chế của $f_i$ lên $V_i\cap W_j$ là hạn chế của $\widetilde{f}_j$. Bây giờ ta có

$$
r_{V_i\cap W_j,V_i}(f_i) =r_{V_i\cap W_j,V_i\cap V_{\iota(j)}}(r_{V_i\cap V_{\iota(j)},V_i}(f_i))
$$

$$
=r_{V_i\cap W_j,V_i\cap V_{\iota(j)}}(r_{V_i\cap V_{\iota(j)},V_{\iota(j)}}(f_{\iota(j)}) =r_{V_i\cap W_j,V_{\iota(j)}}(f_{\iota(j)})
$$

trong đó ta đã dùng giả thiết liên quan đến họ $(f_i)$. Nhưng khi đó

$$
r_{V_i\cap W_j,V_{\iota(j)}}(f_{\iota(j)}) =r_{V_i\cap W_j,W_j}(r_{W_j,V_{\iota(j)}}(f_{\iota(j)})) =r_{V_i\cap W_j,W_j}(\widetilde{f}_j)
$$

điều này cho phép ta kết luận.

### 5. Giải thích các hàm như các phân phối

#### Mệnh đề 6 {#ts-iv-s3-prop-6 .statement tag=030Q}

Cho $\nu$ là một độ đo trên U. Hạn chế của $\nu$ lên $\mathscr{D}(U)$ là một phân phối, và nó bằng không khi và chỉ khi độ đo $\nu$ bằng không.

Cho K là một tập con compact của U. Với mọi hàm $\varphi \in \mathscr{C}_K^{\infty}$(U), ta có $|\langle \nu , \varphi \rangle |\leqslant p_{0,K}(\varphi )|\nu |$(K), do đó hạn chế của $\nu$ lên $\mathscr{D}(U)$ là liên tục. Vì $\mathscr{D}(U)$ trù mật trong $\mathscr{K}(U)$ (mệnh đề 4, a) của IV, p. 202), nên hạn chế của $\nu$ lên $\mathscr{D}(U)$ bằng không khi và chỉ khi $\nu$ bằng không.

Ta sẽ đồng nhất không gian $\mathscr{M}(U;\mathbf{C})$ các độ đo phức trên U với một không gian con của $\mathscr{D}'(U)$. Ta cũng sẽ đồng nhất không gian $L^1_{loc}(U)$ với một không gian con của $\mathscr{D}'(U)$ bởi ánh xạ suy ra bằng cách chuyển qua các thương từ ánh xạ gán cho $f\in \mathscr{L}_{loc}^1(U)$ độ đo $f\cdot \mu$ (INT, V, p. 44, § 5, No.$^o2$, định nghĩa 2). Nói cách khác, với $f\in L^1_{loc}(U)$ và $\varphi \in \mathscr{D}$(U), ta có

$$
\langle f, \varphi \rangle =\int_Uf \varphi  d\mu
$$

Đặc biệt, với $p\in [1,+\infty ]$, điều này cho phép đồng nhất không gian $L^p(U)$ với một không gian con của $\mathscr{D}'(U) ($x. INT, V, p. 43, § 5, No.$^o1)$.

#### Mệnh đề 7 {#ts-iv-s3-prop-7 .statement tag=030R}

Cho $p\in [1,+\infty ]$. Đơn ánh từ $L^p(U)$ vào $\mathscr{D}'(U)$ là liên tục.

Cho $f\in L^p(U)$. Cho K là một tập con compact của U, và ký hiệu bởi $\varphi_K$ hàm đặc số của nó. Với mọi hàm thử $\varphi$ có giá chứa trong K, bất đẳng thức Hölder suy ra

$$
|\langle f, \varphi \rangle |=|\int_Uf \varphi  d\mu|\leqslant N_p(f)N_q(\varphi )\leqslant N_p(f)N_q(\varphi_K)p_{0,K}(\varphi )
$$

trong đó $q$ là số mũ liên hợp của $p$.

Đặc biệt ta có thể đồng nhất $\mathscr{D}(U)$ với một không gian con của $\mathscr{D}'(U)$.

#### Mệnh đề 8 {#ts-iv-s3-prop-8 .statement tag=030S}

Không gian $\mathscr{D}(U)$ trù mật trong $\mathscr{D}'(U)$.

Cho $\lambda$ là một dạng tuyến tính trên $\mathscr{D}'(U)$ triệt tiêu trên $\mathscr{D}(U)$. Vì $\mathscr{D}(U)$ là phản xạ, tồn tại một hàm thử $\varphi \in \mathscr{D}(U)$ sao cho $\lambda (f) =\langle f, \varphi \rangle$ với mọi $f\in \mathscr{D}'(U)$. Do đó

$$
0 =\lambda (\overline{\varphi}) =\langle \varphi , \varphi \rangle =\int_U|\varphi |^2d\mu
$$

suy ra $\varphi = 0$. Mệnh đề do đó suy ra từ định lý Hahn–Banach (EVT, II, p. 49, hệ quả 3 (ii)).

Với $h\in \mathscr{C}^{\infty}$(U), ánh xạ chuyển vị của ánh xạ tuyến tính liên tục $\varphi \mapsto h\varphi$ từ $\mathscr{D}(U)$ vào chính nó là một ánh xạ tuyến tính liên tục của $\mathscr{D}'(U)$ vào chính nó, được ký hiệu là $f\mapsto hf$. Định nghĩa này là xác đáng vì nếu $f$ là phân phối liên kết với một độ đo $\nu$ trên U, thì $hf$ liên kết với độ đo $h\cdot \nu$. Thật vậy, với mọi hàm thử $\varphi \in \mathscr{D}$(U), ta tính được

$$
\langle hf, \varphi \rangle =\langle f, h\varphi \rangle =\int_Uh\varphi d\nu =\int_U\varphi  d(h\cdot \nu )
$$

### 6. Đạo hàm của các phân phối

Cho $\alpha \in \mathbf{N}^n$. Ánh xạ tuyến tính $\varphi \mapsto \partial^{\alpha}\varphi$ là liên tục từ $\mathscr{D}(U)$ vào $\mathscr{D}(U)$. Ánh xạ chuyển vị của nó $^t\partial^{\alpha}$ là một ánh xạ tuyến tính liên tục của $\mathscr{D}'(U)$ vào $\mathscr{D}'(U)$ (EVT, IV, p. 6, cor., b)).

Ánh xạ tuyến tính liên tục $(-1)^{|\alpha|t}\partial^{\alpha}$ của $\mathscr{D}'(U)$ vào chính nó được ký hiệu là $\partial^{\alpha}$.

#### Định nghĩa 2 {#ts-iv-s3-def-2 .statement tag=030T}

Nếu $f\in \mathscr{D}'(U)$ là một phân phối, thì $\partial^{\alpha}f$ được gọi là đạo hàm riêng lặp cấp $\alpha$ của $f$.

Do đó, theo định nghĩa,

$$
\langle \partial^{\alpha}f, \varphi \rangle = (-1)^{|\alpha|}\langle f, \partial^{\alpha}\varphi \rangle
$$

với mọi hàm $\varphi \in \mathscr{D}(U)$. Ta có $\partial^{\alpha+\beta}=\partial^{\alpha}\circ \partial^{\beta}$ với mọi $\alpha$ và $\beta$ trong $\mathbf{N}^n$.

Nếu $n= 1$, đạo hàm của một phân phối $f\in \mathscr{D}'(U)$ cũng sẽ được ký hiệu là $f'$.

Định nghĩa này được biện minh bởi bổ đề sau.

#### Bổ đề 6 {#ts-iv-s3-lem-6 .statement tag=030U}

Cho $k$ là một số tự nhiên. Cho $f\in \mathscr{C}^k(U)$ và cho $\lambda$ là phân phối liên kết với $f$. Với mọi $\beta \in \mathbf{N}^n$ sao cho $|\beta |\leqslant k$, phân phối $\partial^{\beta}\lambda$ là phân phối liên kết với hàm $\partial^{\beta}f$.

Bằng quy nạp theo $k$, chỉ cần chứng minh tính chất này khi $\beta$ thỏa mãn $|\beta |= 1$, và thậm chí có thể giả sử rằng $\beta = (0, . . . ,0,1)$. Vì các phân phối xác định một bó (mệnh đề 5 của IV, p. 204), chỉ cần kiểm tra mệnh đề này khi tồn tại một tập hợp mở $V\subset \mathbf{R}^{n-1}$ và một khoảng mở $I\subset \mathbf{R}$ sao cho $U = V\times I$.

Với mọi hàm thử $\varphi \in \mathscr{D}$(U), theo định nghĩa ta có

$$
\langle \partial^{\beta}\lambda , \varphi \rangle =-\int_Uf(x)\partial^{\beta}\varphi (x)dx=-\int_V(\int_If(y, t)\partial^{\beta}\varphi (y, t)dt)dy
$$

từ định lý Lebesgue–Fubini (INT, V, p. 96, § 8, n$^o4$, th. 1). Bằng phép tích phân từng phần (FVR, II, p. 10), ta có

$$
-\int_If(y, t)\partial^{\beta}\varphi (y, t)dt=\int_I\partial^{\beta}f(y, t)\varphi (y, t)dt
$$

vì $t\mapsto \varphi (y, t)$ có giá compact trong I. Do đó suy ra

$$
\langle \partial^{\beta}\lambda , \varphi \rangle =\int_V(\int_I\partial^{\beta}f(y, t)\varphi (y, t)dt)dy=\langle \partial^{\beta}f, \varphi \rangle
$$

#### Mệnh đề 9 (Công thức Leibniz) {#ts-iv-s3-prop-9 .statement tag=030V}

Cho $f$ là một phân phối trên U và $g$ là một hàm khả vi vô hạn trên U. Cho $\alpha \in \mathbf{N}^n$. Ta có quan hệ

$$
\alpha (\alpha )\beta \alpha -\beta
$$

$$
\partial (f g) =\sum\partial f \partial g
$$

$$
\beta
$$

$\beta \leqslant \alpha$

Tiến hành bằng quy nạp theo $|\alpha |$ như trong chứng minh của FVR, I, p. 28, prop. 2, chỉ cần xét trường hợp $|\alpha |= 1$. Khi đó kết quả suy ra từ phép tính

$$
\langle \partial^{\alpha}(f g), \varphi \rangle =\langle f g,-\partial^{\alpha}\varphi \rangle =\langle f,-g\partial^{\alpha}\varphi \rangle
$$

$$
=\langle f,-\partial^{\alpha}(g\varphi ) +\varphi \partial^{\alpha}g\rangle =\langle g\partial^{\alpha}f+f \partial^{\alpha}g, \varphi \rangle
$$

đúng với mọi $\varphi \in \mathscr{D}(U)$.

### 7. Các hàm Schwartz

Ta ký hiệu bởi $\mathscr{S}(\mathbf{R}^n)$ không gian các hàm khả vi vô hạn $\varphi$ trên $\mathbf{R}^n$, nhận giá trị phức, sao cho, với mọi $\alpha$ và $\beta$ trong $\mathbf{N}^n$, hàm $X^{\beta}\partial^{\alpha}\varphi$ bị chặn trên $\mathbf{R}^n$. Người ta trang bị cho $\mathscr{S}(\mathbf{R}^n)$ tôpô lồi địa phương được xác định bởi họ đếm được các nửa chuẩn $(q_{\alpha ,\beta})_{(\alpha ,\beta)\in\mathbf{N}^n\times\mathbf{N}^n}$, trong đó $q_{\alpha ,\beta}$ được xác định bởi

$q_{\alpha ,\beta}(\varphi ) =$ sup$_{x\in\mathbf{R}^n}|x^{\beta}\partial^{\alpha}\varphi (x)|=\|X^{\beta}\partial^{\alpha}\varphi \|_{\infty}$

đối với $\varphi \in \mathscr{S}(\mathbf{R}^n)$. Tôpô này là tách được. Nó cũng được xác định bởi các nửa chuẩn $\widetilde{q}_{\alpha ,k}$ xác định bởi

$\widetilde{q}_{\alpha ,k}(\varphi ) =$ sup$_{x\in\mathbf{R}^n}\|x\|^k|(\partial^{\alpha}\varphi )(x)|$.

đối với mọi $\varphi \in \mathscr{S}(\mathbf{R}^n)$, trong đó $k\in \mathbf{N}$ và $\alpha \in \mathbf{N}^n$.

Người ta nói rằng $\mathscr{S}(\mathbf{R}^n)$ là không gian Schwartz hay không gian các hàm Schwartz trên $\mathbf{R}^n$.

#### Nhận xét {#ts-iv-s3-n7-rem-1 .statement tag=030W}

Cho $\varphi \in \mathscr{S}(\mathbf{R}^n)$. Với mọi $k\in \mathbf{N}$, ta có

lim$_{\|x\|\rightarrow+\infty}\|x\|^k\varphi (x) = 0$,

vì hàm $x\mapsto  \|x\|^{k+1}\varphi (x)$ bị chặn.

#### Ví dụ {#ts-iv-s3-n7-exa-1 .statement tag=030X}

Hàm $\gamma_n$ xác định trên $\mathbf{R}^n$ bởi $\gamma_n(x) =$ exp($-\|x\|^2$) thuộc $\mathscr{S}(\mathbf{R}^n)$. Thật vậy, người ta chứng minh bằng quy nạp theo $k$ rằng, với mọi số nguyên $k\in \mathbf{N}$, tồn tại một đa thức $P_k\in \mathbf{R}[X]$ sao cho $\partial_k\gamma_1= P_k\gamma_1$.

Với mọi $\alpha = (\alpha_i)\in \mathbf{N}^n$ và $\beta = (\beta_i)\in \mathbf{N}^n$, và mọi $x= (x_i)\in \mathbf{R}^n$, khi đó ta có

$$
|(X^{\beta}\partial^{\alpha}\gamma_n)(x)|=\prod_{i=1}^n|x_i|^{\beta_i}|P_{\alpha_i}(x_i)|\gamma_1(x_i)
$$

đó là một lượng bị chặn khi $x$ biến thiên trong $\mathbf{R}^n$.

Cho $\alpha \in \mathbf{N}^n$ và $\beta \in \mathbf{N}^n$. Nếu $\varphi \in \mathscr{S}(\mathbf{R}^n)$, thì $X^{\beta}\partial^{\alpha}(\varphi )$ lại là một hàm Schwartz; ánh xạ thu được $\varphi \mapsto X^{\beta}\partial^{\alpha}\varphi$ của $\mathscr{S}(\mathbf{R}^n)$ vào chính nó là liên tục.

Không gian $\mathscr{S}(\mathbf{R}^n)$ là một đại số tôpô. Chính xác hơn, nếu $\varphi_1$ và $\varphi_2$ thuộc $\mathscr{S}(\mathbf{R}^n)$, thì $\varphi_1\varphi_2$ là một hàm Schwartz sao cho

$$
(\alpha )
$$

$$
q_{\alpha ,\beta}(\varphi_1\varphi_2)\leqslant \sum q_{\gamma ,\beta}(\varphi_1)q_{\alpha-\gamma ,0}(\varphi_2) \tag{2}
$$

$$
\gamma
$$

$0\leqslant \gamma \leqslant \alpha$

với mọi $\alpha$ và $\beta \in \mathbf{N}^n$ (mệnh đề 1 của IV, p. 196).

Phép bao hàm chính tắc của $\mathscr{S}(\mathbf{R}^n)$ vào không gian $\mathscr{C}^{\infty}(\mathbf{R}^n)$, được trang bị tôpô được mô tả trong Số$^o3$ của IV, p. 200, là liên tục, vì

sup$_{x\in K}|\partial^{\alpha}\varphi (x)|\leqslant q_{\alpha ,0}(\varphi )$

đối với mọi tập con compắc K của $\mathbf{R}^n$, mọi $\alpha \in \mathbf{N}^n$ và mọi hàm Schwartz $\varphi$.

#### Bổ đề 7 {#ts-iv-s3-lem-7 .statement tag=030Y}

Cho $k\in \mathbf{N}$ và $\alpha \in \mathbf{N}^n$. Với mọi hàm $\varphi \in \mathscr{S}(\mathbf{R}^n)$ và mọi số thực $T>0$, ta có

$_k\alpha$ 1

(3) $\widetilde{q}_{\alpha ,k}(\varphi )\leqslant T$ sup $|\partial \varphi (x)|+\widetilde{q}_{\alpha ,k+1}(\varphi )$.

$\|x\|\leqslant T$ T

Thật vậy, ta có

$\widetilde{q}_{\alpha ,k}(\varphi )\leqslant$ sup$_{\|x\|\leqslant T}\|x\|^k|\partial^{\alpha}\varphi (x)|+$ sup$_{\|x\|>T}\|x\|^k|\partial^{\alpha}\varphi (x)|$

$\leqslant T^k$ sup$_{\|x\|\leqslant T}|\partial^{\alpha}\varphi (x)|+\frac{1}{T}$ sup$_{\|x\|>T}\|x\|^{k+1}|\partial^{\alpha}\varphi (x)|$.

#### Mệnh đề 10 {#ts-iv-s3-prop-10 .statement tag=030Z}

Cho B là một tập con bị chặn của $\mathscr{S}(\mathbf{R}^n)$. Tôpô cảm sinh trên B bởi $\mathscr{S}(\mathbf{R}^n)$ trùng với tôpô cảm sinh bởi $\mathscr{C}^{\infty}(\mathbf{R}^n)$.

Vì phép bao hàm của $\mathscr{S}(\mathbf{R}^n)$ vào $\mathscr{C}^{\infty}(\mathbf{R}^n)$ là liên tục, chỉ cần chứng minh rằng, với mọi tập con mở V của $\mathscr{S}(\mathbf{R}^n)$, giao $V\cap B$ là mở trong B đối với tôpô cảm sinh bởi $\mathscr{C}^{\infty}(\mathbf{R}^n)$.

Cho V là một tập con mở của $\mathscr{S}(\mathbf{R}^n)$. Cho $\varphi_0\in V\cap B$. Tồn tại một tập hợp hữu hạn I, một họ $(\alpha_i, k_i)_{i\in I}\in (\mathbf{N}^n\times \mathbf{N})^I$ và một số thực $\varepsilon  >0$ sao cho V chứa tập hợp các $\varphi \in \mathscr{S}(\mathbf{R}^n)$ thỏa mãn

sup$_{i\in I}\widetilde{q}_{\alpha_i,k_i}(\varphi -\varphi_0)\leqslant \varepsilon$.

Vì B bị chặn trong $\mathscr{S}(\mathbf{R}^n)$, tồn tại $M>0$ sao cho các nửa chuẩn $\widetilde{q}_{\alpha_i,k_i+1}$ với $i\in I$ bị chặn bởi M trên B. Cho $\delta  >0$ và $T>0$ là các số thực. Theo bất đẳng thức (3), ngay khi $\varphi \in B$ thỏa mãn điều kiện chặn

(4) sup$_{i\in I}$ sup$_{\|x\|\leqslant T}|\partial^{\alpha_i}(\varphi -\varphi_0)|\leqslant \delta$,

ta có

$_k$ 2M

sup $\widetilde{q}_{\alpha_i,k_i}(\varphi -\varphi_0)\leqslant \delta T$ +.

$_{i\in I}$ T

Đặt $T =\frac{4M}{\varepsilon}$, khi đó $\delta =\frac{\varepsilon}{2T^k}$. Ta thấy rằng $V\cap B$ chứa lân cận của $\varphi_0$ trong B đối với tôpô cảm sinh của $\mathscr{C}^{\infty}(\mathbf{R}^n)$ được xác định bởi (4). Điều này hoàn tất chứng minh.

#### Hệ quả {#ts-iv-s3-n7-cor-1 .statement tag=0310}

Cho $(\varphi_m)_{m\in\mathbf{N}}$ là một dãy bị chặn trong $\mathscr{S}(\mathbf{R}^n)$. Với mọi hàm $\varphi \in \mathscr{S}(\mathbf{R}^n)$, các mệnh đề sau là tương đương:

a) Dãy $(\varphi_m)$ hội tụ tới $\varphi$ trong $\mathscr{S}(\mathbf{R}^n)$;

b) Dãy $(\varphi_m)$ hội tụ tới $\varphi$ trong $\mathscr{C}^{\infty}(\mathbf{R}^n)$.

#### Nhận xét {#ts-iv-s3-n7-rem-2 .statement tag=0311}

Một dãy $(\varphi_m)$ trong $\mathscr{C}^{\infty}(\mathbf{R}^n)$ hội tụ khi và chỉ khi, với mọi $\alpha \in \mathbf{N}^n$, dãy $(\partial^{\alpha}\varphi_m)$ hội tụ tới một hàm $\varphi^{(\alpha)}$ trong $\mathscr{C}(\mathbf{R}^n)$ được trang bị tôpô hội tụ compact. Khi đó ta có $\varphi^{(\alpha)}=\partial^{\alpha}\varphi$ và $(\varphi_m)$ hội tụ tới $\varphi^{(0)}$.

Thật vậy, điều kiện ấy là cần thiết. Ngược lại, nếu các dãy $(\partial^{\alpha}\varphi_m)$ hội tụ tới các hàm $\varphi^{(\alpha)}$ với mọi $\alpha \in \mathbf{N}^n$, thì theo FVR, II, p. 2, th. 1, suy ra rằng $\varphi^{(\alpha)}=\partial^{\alpha}\varphi^{(0)}$, điều đó có nghĩa là dãy $(\varphi_m)$ hội tụ tới $\varphi^{(0)}$ trong $\mathscr{C}^{\infty}(\mathbf{R}^n)$.

#### Mệnh đề 11 {#ts-iv-s3-prop-11 .statement tag=0312}

Không gian $\mathscr{S}(\mathbf{R}^n)$ là một không gian Fréchet và một không gian Montel.

Vì không gian $\mathscr{C}^{\infty}(\mathbf{R}^n)$ là đầy đủ (EVT, III, p. 9, ví dụ b)), hệ quả của mệnh đề 10 suy ra rằng mọi dãy Cauchy trong $\mathscr{S}(\mathbf{R}^n)$ đều hội tụ trong $\mathscr{S}(\mathbf{R}^n)$ vì nó bị chặn và hội tụ trong $\mathscr{C}^{\infty}(\mathbf{R}^n)$.

Do đó $\mathscr{S}(\mathbf{R}^n)$ là một không gian Fréchet; đặc biệt, nó là một không gian thùng (EVT, III, p. 25, hệ quả của mệnh đề 2). Cho B là một tập con bị chặn của $\mathscr{S}(\mathbf{R}^n)$ và $(\varphi_m)_{m\in\mathbf{N}}$ là một dãy nhận giá trị trong B. Vì $\mathscr{C}^{\infty}(\mathbf{R}^n)$ là một không gian Montel (EVT, IV, p. 18, ví dụ (4)), tồn tại một dãy con của $(\varphi_m)_{m\in\mathbf{N}}$ hội tụ trong $\mathscr{C}^{\infty}(\mathbf{R}^n)$, do đó trong $\mathscr{S}(\mathbf{R}^n)$ (mệnh đề 10). Vậy B là tương đối compact trong $\mathscr{S}(\mathbf{R}^n)$. Suy ra rằng $\mathscr{S}(\mathbf{R}^n)$ là một không gian Montel.

### 8. Các bao hàm của các không gian hàm trong không gian các hàm Schwartz

#### Mệnh đề 12 {#ts-iv-s3-prop-12 .statement tag=0313}

Không gian $\mathscr{D}(\mathbf{R}^n)$ được chứa trong $\mathscr{S}(\mathbf{R}^n)$, và phép nhúng của $\mathscr{D}(\mathbf{R}^n)$ vào $\mathscr{S}(\mathbf{R}^n)$ là liên tục và có ảnh trù mật.

Cho $B\subset \mathscr{D}(\mathbf{R}^n)$ là một tập con bị chặn, và cho K là một tập con compact của $\mathbf{R}^n$ sao cho $B\subset \mathscr{C}_K^{\infty}(\mathbf{R}^n)$. Cho $\alpha \in \mathbf{N}^n$ và $k\in \mathbf{N}$. Với mọi hàm $\varphi \in B$, ta có

$\widetilde{q}_{\alpha ,k}(\varphi )\leqslant ($sup$_{x\in K}\|x\|^k)p_{\alpha ,K}(\varphi )$,

do đó B bị chặn trong $\mathscr{S}(\mathbf{R}^n)$. Tính liên tục của phép bao hàm khi đó suy ra từ việc các không gian $\mathscr{S}(\mathbf{R}^n)$ và $\mathscr{D}(\mathbf{R}^n)$ là bornological.

Hãy chứng minh rằng $\mathscr{D}(\mathbf{R}^n)$ trù mật trong $\mathscr{S}(\mathbf{R}^n)$. Gọi B là quả cầu đơn vị của $\mathbf{R}^n$ và cho $\eta \in \mathscr{D}(\mathbf{R}^n)$ là một hàm thử có giá được chứa trong 2B sao cho $0\leqslant \eta \leqslant 1$ và $\eta (x) = 1$ với mọi $x\in B$ (bổ đề 1, a) của IV, p. 196).

Cho $\varphi \in \mathscr{S}(\mathbf{R}^n)$. Với mọi số nguyên $m\geqslant 1$ và mọi $x\in \mathbf{R}^n$, đặt $\eta_m(x) =\eta (x/m)$. Cuối cùng định nghĩa $\varphi_m=\eta_m\varphi$; ta có $\varphi_m\in \mathscr{D}(\mathbf{R}^n)$. Vì $\partial^{\alpha}\eta_m=m^{-|\alpha|}(\partial^{\alpha}\eta )(x/m)$ với mọi $\alpha \in \mathbf{N}^n$ và $x\in \mathbf{R}^n$, suy ra từ công thức (2) của IV, p. 210 rằng dãy $(\varphi_m)$ bị chặn trong $\mathscr{S}(\mathbf{R}^n)$.

Cho C là một tập con compắc của $\mathbf{R}^n$. Dãy $(\varphi_m)_{m\geqslant 1}$ hội tụ tới $\varphi$ trong $\mathscr{C}_K^{\infty}(\mathbf{R}^n)$ vì $\varphi_m$ trùng với $\varphi$ trên C với mọi m đủ lớn. Vậy dãy $(\varphi_m)$ hội tụ tới $\varphi$ trong $\mathscr{C}^{\infty}(\mathbf{R}^n)$, và hệ quả của mệnh đề 10 của IV, p. 211 cho phép kết luận rằng dãy $(\varphi_m)$ hội tụ tới $\varphi$ trong $\mathscr{S}(\mathbf{R}^n)$.

#### Bổ đề 8 {#ts-iv-s3-lem-8 .statement tag=0314}

Cho B là một tập con bị chặn của $\mathscr{D}(\mathbf{R}^n)$. Tôpô cảm sinh trên B bởi tôpô của $\mathscr{S}(\mathbf{R}^n)$ trùng với tôpô cảm sinh bởi $\mathscr{D}(\mathbf{R}^n)$.

Vì phép bao hàm của $\mathscr{D}(\mathbf{R}^n)$ vào $\mathscr{S}(\mathbf{R}^n)$ là liên tục, tôpô trên B cảm sinh bởi $\mathscr{D}(\mathbf{R}^n)$ mịn hơn tôpô cảm sinh bởi $\mathscr{S}(\mathbf{R}^n)$. Mặt khác, tồn tại một tập con compắc K của $\mathbf{R}^n$ sao cho $B\subset \mathscr{C}_K^{\infty}(\mathbf{R}^n)$. Với mọi $\alpha \in \mathbf{N}^n$, khi đó ta có $p_{\alpha ,K}(\varphi )\leqslant \widetilde{q}_{\alpha ,0}(\varphi )$, điều này kéo theo rằng tôpô cảm sinh bởi $\mathscr{S}(\mathbf{R}^n)$ mịn hơn tôpô cảm sinh bởi $\mathscr{D}(\mathbf{R}^n)$.

#### Mệnh đề 13 {#ts-iv-s3-prop-13 .statement tag=0315}

Cho $p\in [1,+\infty ]$. Không gian $\mathscr{S}(\mathbf{R}^n)$ được chứa trong $\mathscr{L}^p(\mathbf{R}^n)$ và đơn ánh chính tắc của $\mathscr{S}(\mathbf{R}^n)$ vào $\mathscr{L}^p(\mathbf{R}^n)$ là liên tục. Ảnh của $\mathscr{S}(\mathbf{R}^n)$ trong $L^p(\mathbf{R}^n)$ là trù mật nếu $p\not = +\infty$.

Mệnh đề thứ nhất là ngay lập tức đối với $p= +\infty$. Từ đây về sau giả sử rằng $p\in [1,+\infty [$. Gọi $m$ là một số nguyên sao cho $n+ 1< mp$. Với mọi $\varphi \in \mathscr{S}(\mathbf{R}^n)$ và $x\in \mathbf{R}^n$, ta có

$$
\|x\|^{n+1}|\varphi (x)|^p\leqslant \widetilde{q}_{0,m}(\varphi )^p
$$

do đó $\varphi \in \mathscr{L}^p(\mathbf{R}^n)$ theo Mệnh đề 3 của IV, p. 199. Hơn nữa, ta thu được

$$
N_p(\varphi )\leqslant a^{1/p}_n\widetilde{q}_{0,0}(\varphi ) +b_n\widetilde{q}_{0,m}(\varphi )
$$

trong đó

$$
a_n=\int d\mu(x),b_n=\int 1_{n+1}d\mu(x)
$$

$$
_{\|x\|\leqslant 1}\|_{x\|\geqslant 1}\|x\|
$$

do đó đơn ánh của $\mathscr{S}(\mathbf{R}^n)$ vào $\mathscr{L}^p(\mathbf{R}^n)$ là liên tục.

Vì không gian $\mathscr{D}(\mathbf{R}^n)$ được chứa trong $\mathscr{S}(\mathbf{R}^n)$, Mệnh đề 4 của IV, p. 202 suy ra rằng $\mathscr{S}(\mathbf{R}^n)$ là trù mật trong $L^p(\mathbf{R}^n)$ nếu $p\not = +\infty$.

### 9. Các hàm có tăng trưởng đa thức

#### Định nghĩa 3 {#ts-iv-s3-def-3 .statement tag=0316}

Một hàm $f:\mathbf{R}^n\rightarrow \mathbf{C}$ có tăng trưởng đa thức nếu tồn tại một số nguyên $k\geqslant 1$ sao cho ánh xạ xác định bởi $x\mapsto (1 +\|x\|)^{-k}f(x)$ bị chặn trên $\mathbf{R}^n$.

Mọi hàm có tăng trưởng đa thức đều bị chặn địa phương. Mọi hàm đa thức trên $\mathbf{R}^n$ đều có tăng trưởng đa thức.

#### Mệnh đề 14 {#ts-iv-s3-prop-14 .statement tag=0317}

Cho $f\in \mathscr{C}^{\infty}(\mathbf{R}^n)$. Giả sử rằng với mọi $\alpha$ trong $\mathbf{N}^n$, hàm $\partial^{\alpha}f$ có tăng trưởng đa thức. Ánh xạ tuyến tính của không gian $\mathscr{S}(\mathbf{R}^n)$ vào chính nó xác định bởi $\varphi \mapsto f \varphi$ là liên tục.

Với mọi $\varphi$ trong $\mathscr{S}(\mathbf{R}^n)$, hàm $f \varphi$ thuộc $\mathscr{C}^{\infty}(\mathbf{R}^n)$. Theo giả thiết, với mọi $\alpha \in \mathbf{N}^n$, tồn tại một số nguyên $k_{\alpha}\geqslant 0$ và một số thực $C_{\alpha}$ sao cho $|\partial^{\alpha}f(x)|\leqslant C_{\alpha}(1 +\|x\|)^{k_{\alpha}}$ với mọi $x$ trong $\mathbf{R}^n$. Gọi $\varphi \in \mathscr{S}(\mathbf{R}^n)$. Gọi $\alpha \in \mathbf{N}^n$ và $k\in \mathbf{N}$. Theo Mệnh đề 1 của IV, p. 196, suy ra

$$
(\alpha )k\beta \alpha -\beta
$$

$\widetilde{q}_{\alpha ,k}(f \varphi )\leqslant \sum$ sup $\|x\||\partial f(x)\partial \varphi (x)|$

$$
\beta_{x\in\mathbf{R}^n}
$$

$0\leqslant \beta \leqslant \alpha$

$$
(\alpha )kk\alpha -\beta
$$

$\leqslant \sum C_{\beta}$ sup $\|x\|(1 +\|x\|)^{^{\beta}}|\partial \varphi (x)|$.

$$
\beta_{x\in\mathbf{R}^n}
$$

$0\leqslant \beta \leqslant \alpha$

Gọi $\beta \in \mathbf{N}^n$ sao cho $0\leqslant \beta \leqslant \alpha$. Với mọi $x\in \mathbf{R}^n$, ta có

$\|x\|^k(1 +\|x\|)^{k_{\beta}}|\partial^{\alpha-\beta}\varphi (x)|\leqslant$ sup$_{\|x\|\leqslant 1}2^{k_{\beta}}|\partial^{\alpha-\beta}\varphi (x)|$

+ sup$_{x\in\mathbf{R}^n}2^{k_{\beta}}\|x\|^{k+k_{\beta}}|\partial^{\alpha-\beta}\varphi (x)|$ do đó cuối cùng

$$
(\alpha )_k()
$$

$$
\widetilde{q}_{\alpha ,k}(f \varphi )\leqslant \sum 2^{^{\beta}}C_{\beta}\widetilde{q}_{\alpha-\beta ,0}(\varphi ) +\widetilde{q}_{\alpha-\beta ,k+k_{\beta}}(\varphi )
$$

$$
\beta
$$

$0\leqslant \beta \leqslant \alpha$

điều này suy ra mệnh đề.

### 10. Các phân phối ôn hòa

#### Định nghĩa 4 {#ts-iv-s3-def-4 .statement tag=0318}

Không gian đối ngẫu của $\mathscr{S}(\mathbf{R})$ được trang bị tôpô của sự hội tụ bị chặn được gọi là không gian các phân phối ôn hòa trên $\mathbf{R}^n$. Nó được ký hiệu bởi $\mathscr{S}'(\mathbf{R}^n)$.

Vì $\mathscr{S}(\mathbf{R}^n)$ là sinh bởi bị chặn, không gian $\mathscr{S}'(\mathbf{R}^n)$ là đầy đủ (EVT, III, p. 24, hệ quả 1). Vì $\mathscr{S}(\mathbf{R}^n)$ là một không gian Montel, điều tương tự cũng đúng với $\mathscr{S}'(\mathbf{R}^n)$ (EVT, IV, p. 19, mệnh đề 9). Do đó không gian $\mathscr{S}'(\mathbf{R}^n)$ là phản xạ (EVT, IV, p. 16, định lý 2).

#### Bổ đề 9 {#ts-iv-s3-lem-9 .statement tag=0319}

Một ánh xạ tuyến tính $f$ từ $\mathscr{S}(\mathbf{R}^n)$ vào $\mathbf{C}$ là một phân phối ôn hòa khi và chỉ khi với mọi họ $(M_{\alpha ,k})_{(\alpha ,k)\in\mathbf{N}^n\times\mathbf{N}}$ trong $\mathbf{R}_+$, dạng tuyến tính $f$ bị chặn trên tập hợp các hàm $\varphi \in \mathscr{S}(\mathbf{R}^n)$ sao cho $\widetilde{q}_{\alpha ,k}(\varphi )\leqslant M_{\alpha ,k}$ với mọi $(\alpha , k)\in \mathbf{N}^n\times \mathbf{N}$.

Thật vậy, không gian $\mathscr{S}(\mathbf{R}^n)$ là sinh bởi bị chặn (EVT, III, p. 12, mệnh đề 2), và mọi tập con bị chặn của $\mathscr{S}(\mathbf{R}^n)$ đều được chứa trong một trong các tập bị chặn được mô tả trong mệnh đề.

#### Bổ đề 10 {#ts-iv-s3-lem-10 .statement tag=031A}

Cho $\mathfrak{F}$ là một bộ lọc trên $\mathscr{S}'(\mathbf{R}^n)$ có một cơ sở đếm được hoặc chứa một tập hợp bị chặn đơn. Khi đó $\mathfrak{F}$ hội tụ tới một phân phối ôn hòa khi và chỉ khi $\langle f, \varphi \rangle$ hội tụ theo $\mathfrak{F}$ với mọi hàm Schwartz $\varphi$.

Đặc biệt, một dãy $(f_m)_{m\in\mathbf{N}}$ các phân phối ôn hòa hội tụ tới một phân phối ôn hòa $f$ khi và chỉ khi ta có $\langle f_m, \varphi \rangle  \rightarrow  \langle f, \varphi \rangle$ với mọi $\varphi \in \mathscr{S}(\mathbf{R}^n)$.

Vì $\mathscr{S}'(\mathbf{R}^n)$ là một không gian Fréchet, do đó là thùng, (EVT, III, p. 25, hệ quả của mệnh đề 2) bổ đề suy ra từ định lý Banach-Steinhaus (EVT, III, p. 26, hệ quả 3 của định lý 1).

Đơn ánh chính tắc $j$ của $\mathscr{D}(\mathbf{R}^n)$ vào $\mathscr{S}(\mathbf{R}^n)$ là liên tục, và ảnh của nó là trù mật (bổ đề 12 của IV, p. 212); do đó chuyển vị của $j$, là ánh xạ hạn chế các phân phối ôn hòa lên không gian con $\mathscr{D}(\mathbf{R}^n)$, là một ánh xạ tuyến tính liên tục đơn ánh của $\mathscr{S}'(\mathbf{R}^n)$ vào $\mathscr{D}'(\mathbf{R}^n)$. Ta sẽ đồng nhất $\mathscr{S}'(\mathbf{R}^n)$ với một không gian con của $\mathscr{D}'(\mathbf{R}^n)$ nhờ ánh xạ này.

Cho $\alpha \in \mathbf{N}^n$. Ánh xạ tuyến tính $\varphi \mapsto \partial^{\alpha}\varphi$ của $\mathscr{S}(\mathbf{R}^n)$ vào $\mathscr{S}(\mathbf{R}^n)$ là liên tục. Do đó chuyển vị của nó là một ánh xạ tuyến tính liên tục của $\mathscr{S}'(\mathbf{R}^n)$ vào $\mathscr{S}'(\mathbf{R}^n)$ (EVT, IV, p. 6, hệ quả, b)). Ánh xạ tuyến tính liên tục $(-1)^{|\alpha|t}\partial^{\alpha}$ của $\mathscr{S}'(\mathbf{R}^n)$ vào $\mathscr{S}'(\mathbf{R}^n)$ được ký hiệu bởi $\partial^{\alpha}$. Định nghĩa này tương thích với Định nghĩa 2 của IV, p. 208 đối với các phân phối.

Cho $h\in \mathscr{C}^{\infty}(\mathbf{R}^n)$ là một hàm sao cho $\partial^{\alpha}h$ có tăng trưởng đa thức với mọi $\alpha \in \mathbf{N}^n$. Chuyển vị của ánh xạ tuyến tính liên tục $\varphi \mapsto h\varphi$ (mệnh đề 14 của IV, p. 214) là một ánh xạ tuyến tính liên tục trên $\mathscr{S}'(\mathbf{R}^n)$, được ký hiệu bởi $f\mapsto hf$.

### 11. Giải thích các hàm như các phân phối ôn hòa

#### Định nghĩa 5 {#ts-iv-s3-def-5 .statement tag=031B}

Một độ đo $\nu$ trên $\mathbf{R}^n$ được gọi là tăng ôn nếu tồn tại một số nguyên $r\in \mathbf{N}$ sao cho ánh xạ liên tục $x\mapsto (1 +\|x\|)^{-r}$ là $\nu$-khả tích trên $\mathbf{R}^n$.

Nói cách khác, một độ đo $\nu$ là tăng ôn nếu tồn tại $r\in \mathbf{N}$ sao cho hàm được xác định bởi $x\mapsto  \|x\|^{-r}$ là $\nu$-khả tích trên phần bù của quả cầu đơn vị trong $\mathbf{R}^n$. Đặc biệt, mọi độ đo bị chặn trên $\mathbf{R}^n$ đều tăng ôn. Nói chung hơn, nếu $f$ là một hàm $\mu$-đo được tăng đa thức và nếu $\nu$ là tăng ôn, thì độ đo $f\cdot \nu$ là tăng ôn.

Tập hợp $\mathscr{M}^t(\mathbf{R}^n)$ các độ đo tăng ôn trên $\mathbf{R}^n$ là một không gian con của không gian vectơ $\mathscr{M}(\mathbf{R}^n;\mathbf{C})$ các độ đo phức trên $\mathbf{R}^n$.

#### Mệnh đề 15 {#ts-iv-s3-prop-15 .statement tag=031C}

Cho $\nu$ là một độ đo tăng ôn trên $\mathbf{R}^n$. Hạn chế của $\nu$ lên $\mathscr{S}(\mathbf{R}^n)$ là một phân phối tăng ôn. Nó bằng không khi và chỉ khi độ đo $\nu$ bằng không.

Vì $\nu$ là tăng ôn, nên tồn tại một số nguyên dương $k$ sao cho ánh xạ $x\mapsto  \|x\|^{-k}$ là $\nu$-khả tích trên phần bù của quả cầu đơn vị trong $\mathbf{R}^n$. Với mọi hàm Schwartz $\varphi \in \mathscr{S}(\mathbf{R}^n)$, ta có

$$
|\langle \nu , \varphi \rangle |\leqslant (\int_{\|x\|\leqslant 1}d\nu )\widetilde{q}_{0,0}(\varphi ) +(\int_{\|x\|>1}\|x\|^{-k}d\nu )\widetilde{q}_{0,k}(\varphi )
$$

do đó hạn chế của $\nu$ lên $\mathscr{S}(\mathbf{R}^n)$ là một phân phối tăng ôn.

Khẳng định cuối cùng suy ra từ Mệnh đề 6 của IV, p. 206 vì $\mathscr{D}(\mathbf{R}^n)$ được chứa trong $\mathscr{S}(\mathbf{R}^n)$.

Ta sẽ đồng nhất không gian $\mathscr{M}^t(\mathbf{R}^n)$ với một không gian con của $\mathscr{S}'(\mathbf{R}^n)$.

#### Mệnh đề 16 {#ts-iv-s3-prop-16 .statement tag=031D}

Cho $p\in [1,+\infty ]$ và $f\in \mathscr{L}^p(\mathbf{R}^n)$. Khi đó độ đo $f\cdot \mu$ có mật độ $f$ đối với độ đo Lebesgue là tăng ôn. Ánh xạ thu được $f\mapsto f\cdot \mu$ từ $L^p(\mathbf{R}^n)$ vào $\mathscr{S}'(\mathbf{R}^n)$ là liên tục.

Cho $q$ là số mũ liên hợp của $p$ và cho $r\geqslant 0$ sao cho $rq > n$. Với mọi $x\in \mathbf{R}^n$, ta viết $g(x) = (1 +\|x\|)^{-r}$. Hàm $g$ thuộc $\mathscr{L}^q(\mathbf{R}^n)$ theo Mệnh đề 3 của IV, p. 199. Theo bất đẳng thức Hölder, ta có

$$
\int_{\mathbf{R}^n}^*(1 +\|x\|)^{-r}|f(x)|d\mu(x)\leqslant N_q(g)N_p(f)<+\infty
$$

do đó độ đo $f\cdot \mu$ là tăng ôn.

Cho $f\in L^p(\mathbf{R}^n)$ và $\varphi \in \mathscr{S}(\mathbf{R}^n)$. Bất đẳng thức Hölder suy ra

$$
|\langle f\cdot \mu, \varphi \rangle |=|\int_{\mathbf{R}^n}f(x)\varphi (x)d\mu(x)|\leqslant \|f\|_p\|\varphi \|_q
$$

và khi đó tính liên tục của ánh xạ $f\mapsto f\cdot \mu$ suy ra từ Mệnh đề 13 của IV, p. 213.

Với mọi $p\in [1,+\infty ]$, ta sẽ đồng nhất $L^p(\mathbf{R}^n)$ với một không gian con của $\mathscr{S}'(\mathbf{R}^n)$ bởi ánh xạ tuyến tính $f\mapsto f\cdot \mu$.

#### Mệnh đề 17 {#ts-iv-s3-prop-17 .statement tag=031E}

Các không gian $\mathscr{D}(\mathbf{R}^n)$ và $\mathscr{S}(\mathbf{R}^n)$ trù mật trong $\mathscr{S}'(\mathbf{R}^n)$.

Chỉ cần chứng minh rằng $\mathscr{D}(\mathbf{R}^n)$ trù mật trong $\mathscr{S}'(\mathbf{R}^n)$. Cho $\lambda$ là một dạng tuyến tính liên tục trên $\mathscr{S}'(\mathbf{R}^n)$ bằng không trên $\mathscr{D}(\mathbf{R}^n)$. Vì không gian $\mathscr{S}(\mathbf{R}^n)$ là phản xạ, tồn tại một hàm $\varphi \in \mathscr{S}(\mathbf{R}^n)$ sao cho $\lambda (f) =\langle f, \varphi \rangle$ với mọi $f\in \mathscr{S}'(\mathbf{R}^n)$. Do đó

$$
0 =\lambda (\psi ) =\langle \psi , \varphi \rangle =\int_{\mathbf{R}^n}\psi \varphi  d\mu
$$

với mọi $\psi \in \mathscr{D}(\mathbf{R}^n)$. Vậy độ đo $\varphi \cdot \mu$ trên $\mathbf{R}^n$ bằng không (mệnh đề 6 của IV, p. 206), do đó $\varphi = 0$. Mệnh đề khi ấy suy ra từ định lý Hahn–Banach (EVT, II, p. 46, hệ quả 1).

### 12. Biến đổi Fourier của các phân phối ôn hòa

Vì mọi hàm Schwartz $\varphi$ đều khả tích trên $\mathbf{R}^n$ (mệnh đề 13 của IV, p. 213), nó có một biến đổi Fourier $\mathscr{F}(\varphi )$ (tương ứng, một đối biến đổi Fourier $\overline{\mathscr{F}}(\varphi )$) được đồng nhất với hàm liên tục bị chặn trên $\mathbf{R}^n$ xác định bởi

$y\mapsto \int\varphi (x)$ exp($-2i\pi  x\cdot y$)$d\mu(x)$

(tương ứng, với hàm $y\mapsto \int^{\mathbf{R}^n}_{\mathbf{R}^n}\varphi (x)$ exp(2$i\pi  x\cdot y$)$d\mu(x)$).

#### Bổ đề 11 {#ts-iv-s3-lem-11 .statement tag=031F}

Cho $\varphi \in \mathscr{S}(\mathbf{R}^n)$. Hàm $\mathscr{F}(\varphi )$ khả vi vô hạn lần trên $\mathbf{R}^n$ và ta có

$$
\mathscr{F}(X^{\alpha}\varphi ) = (-2i\pi )^{-|\alpha|}\partial^{\alpha}(\mathscr{F}(\varphi ))
$$

$$
\mathscr{F}(\partial^{\alpha}\varphi ) = (2i\pi )^{|\alpha|}X^{\alpha}\mathscr{F}(\varphi )
$$

với mọi $\alpha$ trong $\mathbf{N}^n$.

Có thể giả thiết rằng $n\geqslant 1$. Cho $\varphi \in \mathscr{S}(\mathbf{R}^n)$. Hàm xác định bởi $(x, y)\mapsto \varphi (x)$ exp(2$i\pi x\cdot y$) từ $\mathbf{R}^n\times \mathbf{R}^n$ vào $\mathbf{C}$ thỏa các giả thiết của Hệ quả 1 của IV, p. 198 với mọi số nguyên $k$. Vậy biến đổi Fourier của $\varphi$ khả vi vô hạn lần và thỏa

$\partial^{\alpha}(\mathscr{F}\varphi )(y) = (-2i\pi )^{|\alpha|}\int_{\mathbf{R}^n}x^{\alpha}\varphi (x)$ exp($-2i\pi x\cdot y$)$d\mu(x)$

với mọi $y\in \mathbf{R}^n$, điều này kéo theo công thức thứ nhất.

Hãy chứng minh công thức thứ hai. Bằng quy nạp theo $|\alpha |$, chỉ cần làm điều đó khi $|\alpha |= 1$, và ta dễ dàng quy về trường hợp $\alpha = (1,0, . . . ,0)$. Viết mọi $x\in \mathbf{R}^n$ dưới dạng $x= (x_1, x')$ với $x'\in \mathbf{R}^{n-1}$, và ký hiệu bởi $\mu_1$ (resp. $\mu'$) độ đo Lebesgue trên $\mathbf{R}^{n-1}$ (resp. $\mathbf{R}$). Theo định lý Lebesgue-Fubini (INT, V, p. 96, § 8, n$^o4$, th. 1), với mọi $y= (y_1, y')\in \mathbf{R}\times \mathbf{R}^{n-1}$, ta được

$\mathscr{F}(\partial_1\varphi )(y) =\int$ exp($-2i\pi  x'\cdot y'$)

$\times^{\mathbf{R}^n}(\int^{^{-1}}_{\mathbf{R}}(\partial_1\varphi )(x_1, x')$ exp($-2i\pi  x_1y_1$)$d\mu_1(x_1))d\mu'(x')$.

Với mọi khoảng compact $[a, b]$ trong $\mathbf{R}$ và mọi $x'\in \mathbf{R}^{n-1}$, ta có

$\int_a^b(\partial_1\varphi )(x_1, x')$ exp($-2i\pi  x_1y_1$)$d\mu_1(x_1) =$

$[\varphi (x_1, x')$ exp($-2i\pi  x_1y_1$)$]^b_a$

$+ 2i\pi y_1\int_a^b\varphi (x_1, x')$ exp($-2i\pi x_1y_1$)$d\mu_1(x_1)$ theo phép lấy tích phân từng phần (FVR, II, p. 10, công thức (10)). Khi $a$ tiến tới $-\infty$ và $b$ tiến tới $+\infty$, số hạng thứ nhất của vế thứ hai hội tụ về 0 vì $\varphi \in \mathscr{S}(\mathbf{R}^n)$. Số hạng thứ hai hội tụ, theo định lý Lebesgue (INT, IV, p. 137, § 3, n$^o7$, th. 6), tới

$2i\pi y_1\int_{\mathbf{R}}\varphi (x_1, x')$ exp($-2i\pi x_1y_1$)$d\mu_1(x_1)$,

vì ánh xạ $x_1\mapsto \varphi (x_1, x')$ khả tích trên $\mathbf{R}$. Vì $x_1\mapsto \partial_1\varphi (x_1, x')$ cũng khả tích trên $\mathbf{R}$, ta suy ra rằng

$\int_{\mathbf{R}}\partial_1\varphi (x_1, x')$ exp($-2i\pi x_1y_1$)$d\mu_1(x_1)$

$= 2i\pi y_1\int_{\mathbf{R}}\varphi (x_1, x')$ exp($-2i\pi x_1y_1$)$d\mu_1(x_1)$ và cuối cùng, áp dụng lại định lý Lebesgue-Fubini, ta kết luận rằng

$\mathscr{F}(\partial_1\varphi )(y) = 2i\pi y_1\int_{\mathbf{R}^n}\varphi (x)$ exp($-2i\pi  x\cdot y$)$d\mu(x)$,

đúng như cần phải chứng minh.

#### Mệnh đề 18 {#ts-iv-s3-prop-18 .statement tag=031G}

Hạn chế của biến đổi Fourier trên $\mathscr{S}(\mathbf{R}^n)$ là một tự đẳng cấu của các không gian vectơ tôpô mà nghịch đảo là hạn chế của đối biến đổi Fourier.

Cho $\varphi \in \mathscr{S}(\mathbf{R}^n)$. Theo bổ đề trước, biến đổi Fourier của $\varphi$ thuộc $\mathscr{C}^{\infty}(\mathbf{R}^n)$. Hơn nữa, với $\alpha \in \mathbf{N}^n$ và $\beta \in \mathbf{N}^n$, ta có

$$
X^{\beta}\partial^{\alpha}(\mathscr{F}(\varphi )) = (-2i\pi )^{|\alpha|}X^{\beta}\mathscr{F}(X^{\alpha}\varphi )
$$

$$
= (-1)^{|\alpha|}(2i\pi )^{|\alpha|-|\beta|}\mathscr{F}(\partial^{\beta}(X^{\alpha}\varphi ))
$$

Đặc biệt, hàm $X^{\beta}\partial^{\alpha}(\mathscr{F}(\varphi ))$ bị chặn. Vì $\alpha$ và $\beta$ là tùy ý trong $\mathbf{N}^n$, điều đó có nghĩa là $\mathscr{F}(\varphi )$ thuộc $\mathscr{S}(\mathbf{R}^n)$. Hơn nữa, phép tính này kéo theo

$$
q_{\alpha ,\beta}(\mathscr{F}(\varphi ))\leqslant (2\pi )^{|\alpha|-|\beta|}\|\partial^{\beta}(X^{\alpha}\varphi )\|_1
$$

với $(\alpha , \beta )\in \mathbf{N}^n\times \mathbf{N}^n$ và $\varphi \in \mathscr{S}(\mathbf{R}^n)$.

Vì phép bao hàm của không gian $\mathscr{S}(\mathbf{R}^n)$ vào $L^1(\mathbf{R}^n)$ là liên tục (mệnh đề 13 của IV, p. 213), ánh xạ $q_{\alpha ,\beta}\circ \mathscr{F}$ từ $\mathscr{S}(\mathbf{R}^n)$ vào $\mathbf{R}$ là liên tục. Suy ra rằng biến đổi Fourier là liên tục từ không gian $\mathscr{S}(\mathbf{R}^n)$ vào chính nó (x. EVT, II, p. 7, mệnh đề 5, c)). Tương tự, người ta kiểm tra được rằng đối biến đổi Fourier là liên tục từ không gian $\mathscr{S}(\mathbf{R}^n)$ vào chính nó. Theo công thức đảo Fourier (định lý 3 của II, p. 222), biến đổi Fourier và đối biến đổi Fourier là các đẳng cấu nghịch đảo của nhau.

#### Định nghĩa 6 {#ts-iv-s3-def-6 .statement tag=031H}

Chuyển vị của biến đổi Fourier trên $\mathscr{S}(\mathbf{R}^n)$ (tương ứng, của đối biến đổi Fourier) được gọi là biến đổi Fourier (tương ứng, đối biến đổi Fourier) trên $\mathscr{S}'(\mathbf{R}^n)$.

Ký hiệu $\mathscr{F}$ (tương ứng $\overline{\mathscr{F}}$) lại được dùng cho biến đổi Fourier (tương ứng đối biến đổi Fourier) trên $\mathscr{S}'(\mathbf{R}^n)$. Do đó, biến đổi Fourier trên $\mathscr{S}'(\mathbf{R}^n)$ là một tự đẳng cấu của các không gian vectơ tôpô mà nghịch đảo của nó là đối biến đổi Fourier. Với mọi $f\in \mathscr{S}'(\mathbf{R}^n)$, phân phối ôn hòa $\mathscr{F}(f)$ (tương ứng $\overline{\mathscr{F}}(f)$) được xác định bởi công thức

$\langle \mathscr{F}(f), \varphi \rangle =\langle f,\mathscr{F}(\varphi )\rangle ($tương ứng $\langle \overline{\mathscr{F}}(f), \varphi \rangle =\langle f,\overline{\mathscr{F}}(\varphi )\rangle )$

với mọi $\varphi \in \mathscr{S}(\mathbf{R}^n)$.

#### Mệnh đề 19 {#ts-iv-s3-prop-19 .statement tag=031I}

Cho $f$ là một phân phối ôn hòa liên kết với một độ đo bị chặn $\nu \in \mathscr{M}^1(\mathbf{R}^n) ($tương ứng, với $g\in L^2(\mathbf{R}^n))$. Biến đổi Fourier của $f$ trong $\mathscr{S}'(\mathbf{R}^n)$ là phân phối ôn hòa liên kết với biến đổi Fourier của độ đo $\nu ($tương ứng, với biến đổi Fourier của g).

Cho $\nu$ là một độ đo bị chặn trên $\mathbf{R}^n$ và $f$ là phân phối ôn hòa liên kết với $\nu$. Biến đổi Fourier $\mathscr{F}(\nu )$ là một hàm liên tục và bị chặn trên $\mathbf{R}^n$ (mệnh đề 3 của II, p. 207). Phân phối ôn hòa liên kết với hàm này thỏa mãn

$$
\langle \mathscr{F}(\nu ), \varphi \rangle =\int_{\mathbf{R}^n}\mathscr{F}(\nu )\varphi  d\mu=\int_{\mathbf{R}^n}\mathscr{F}(\varphi )d\nu =\langle f,\mathscr{F}(\varphi )\rangle =\langle \mathscr{F}(f), \varphi \rangle
$$

với mọi $\varphi \in \mathscr{S}(\mathbf{R}^n)$, trong đó đẳng thức thứ hai là mệnh đề 13 của II, p. 221, áp dụng được ở đây vì độ đo $\varphi \cdot \mu$ bị chặn. Vậy phân phối ôn hòa liên kết với $\mathscr{F}(\nu )$ là $\mathscr{F}(f)$.

Khi $f$ là phân phối ôn hòa liên kết với $g\in L^2(\mathbf{R}^n)$, người ta làm hoàn toàn tương tự bằng cách dùng công thức (29) của II, p. 221.

Một mệnh đề tương tự cũng đúng đối với đối biến đổi Fourier.

#### Nhận xét {#ts-iv-s3-n12-rem-1 .statement tag=031J}

Các công thức sơ cấp liên quan đến biến đổi Fourier của các độ đo vẫn còn đúng đối với biến đổi Fourier của các phân phối ôn hòa. Chẳng hạn, với $f\in \mathscr{S}'(\mathbf{R}^n)$ và $\alpha \in \mathbf{N}^n$, ta có

$$
\mathscr{F}(\partial^{\alpha}f) = (2i\pi )^{|\alpha|}X^{\alpha}\mathscr{F}(f)
$$

$$
\mathscr{F}(X^{\alpha}f) = (-2i\pi )^{-|\alpha|}\partial^{\alpha}(\mathscr{F}(f))
$$

theo bổ đề 11.

### 13. Phân phối và phân phối ôn hòa trên một không gian vectơ

Cho $u$ là một ánh xạ tuyến tính song ánh của $\mathbf{R}^n$ vào $\mathbf{R}^n$. Ánh xạ $\varphi \mapsto \varphi \circ u$ là một tự đẳng cấu của $\mathscr{S}(\mathbf{R}^n)$ (tương ứng của $\mathscr{D}(\mathbf{R}^n)$); chuyển vị của nó là một tự đẳng cấu của $\mathscr{S}'(\mathbf{R}^n)$ (tương ứng của $\mathscr{D}'(\mathbf{R}^n)$).

Cho E là một không gian vectơ thực hữu hạn chiều, có chiều $n$. Cho $v:\mathbf{R}^n\rightarrow E$ là một đẳng cấu của các không gian vectơ. Ta ký hiệu bởi $\mathscr{S}(E)$ (tương ứng $\mathscr{D}(E)$) tập hợp các ánh xạ $\varphi : E\rightarrow \mathbf{C}$ sao cho $\varphi \circ v\in \mathscr{S}(\mathbf{R}^n)$ (tương ứng sao cho $\varphi \circ v\in \mathscr{D}(\mathbf{R}^n)$). Theo nhận xét trước đó, không gian này không phụ thuộc vào lựa chọn $v$; nó đẳng cấu với $\mathscr{S}(\mathbf{R}^n)$ (tương ứng $\mathscr{D}(\mathbf{R}^n)$). Ta ký hiệu bởi $\mathscr{S}'(E)$ (tương ứng $\mathscr{D}'(E)$) đối ngẫu của $\mathscr{S}(E)$ (tương ứng của $\mathscr{D}(E)$) được trang bị tôpô hội tụ bị chặn. Đây là một không gian vectơ tôpô đẳng cấu với $\mathscr{S}'(\mathbf{R}^n)$ (tương ứng với $\mathscr{D}'(\mathbf{R}^n)$).

Cho E và F là các không gian vectơ thực có chiều $n$, đối ngẫu với nhau đối với một dạng song tuyến tính $b: E\times F\rightarrow \mathbf{R}$. Nhóm giao hoán địa phương compact E đối ngẫu với F đối với ánh xạ

$(x, y)\mapsto$ exp(2$i\pi b(x, y)$)

từ $E\times F$ vào $\mathbf{U}($xem hệ quả 1 của II, p. 235). Ta trang bị cho E và F các độ đo Haar đối ngẫu với nhau đối với ánh xạ này.

Không gian $\mathscr{S}(E)$ được chứa trong $L^1(E)$; biến đổi Fourier của E gây ra, bằng cách chuyển qua các không gian con và bằng đối ngẫu, một đẳng cấu của các không gian vectơ tôpô từ $\mathscr{S}(E)$ lên $\mathscr{S}$ (F), mà ánh xạ chuyển vị của nó là một đẳng cấu của các không gian vectơ tôpô từ $\mathscr{S}'(F)$ lên $\mathscr{S}'(E)$.

### 14. Các Không Gian Sobolev

Cho U là một tập mở của $\mathbf{R}^n$. Cho $p$ là một số thực $\geqslant 1$ và $k$ là một số tự nhiên. Ta ký hiệu bởi $W^{k,p}(U)$ không gian các phân phối $f\in \mathscr{D}'(U)$ sao cho, với mọi $\alpha \in \mathbf{N}^n$ thỏa $|\alpha |\leqslant k$, phân phối $\partial^{\alpha}f$ liên kết với một phần tử của $L^p(U)$.

Đặc biệt, với $U =\mathbf{R}^n$, các phần tử của $W^{k,p}(U)$ là các phân phối ôn hòa.

Ánh xạ từ $W^{k,p}(u)$ vào $\mathbf{R}_+$ gán cho $f\in W^{k,p}(U)$

$$
\|f\|_{k,p}=((\sum_{|\alpha|\leqslant k}\|\partial^{\alpha}f\|^p_p)^{1/p}
$$

là một chuẩn trên $W^{k,p}(U)$. Không gian $W^{k,p}(U)$ sẽ luôn được trang bị chuẩn này; không gian định chuẩn này được gọi là không gian Sobolev có chỉ số $k$ và số mũ $p$.

Không gian $\mathscr{D}(U)$ được chứa trong $W^{k,p}(U)$. Ta ký hiệu bởi $W^{k,p}_0$ (U) bao đóng của $\mathscr{D}(U)$ trong $W^{k,p}(U)$. Nó là một không gian con đóng của $W^{k,p}(U)$.

Ta có $W^{k,p}_0(\mathbf{R}^n) = W^{k,p}(\mathbf{R}^n)$, nhưng nói chung các không gian $W^{k,p}(U)$ và $W^{k,p}_0$ (U) là phân biệt (xem các Bài tập 12 của IV, p. 334 và 14 của IV, p. 334).

Ta cũng ký hiệu $H^k(U) = W^{k,2}(U)$ và $H^k_0(U) = W^{k,2}_0(U)$.

Chuẩn của $H^k(U)$ là một chuẩn tiền Hilbert, liên kết với dạng Hermit dương trên $H^k(U)$ được xác định bởi

$$
(f_1, f_2)\mapsto \sum_{|\alpha|\leqslant}\int_{kU}\overline{\partial^{\alpha}f_1}\partial^{\alpha}f_2d\mu
$$

Không gian Hilbert $H^k(U)$ trùng với không gian được ký hiệu bởi $\mathscr{H}^k$ trong EVT, V, p. 6, ví dụ (3).

Theo định nghĩa, ta có $W^{0,p}(U) = L^p(U)$ và $H^0(U) = L^2(U)$; hơn nữa $W^{0,p}_0(U) = L^p(U)$ theo Mệnh đề 4, b) của IV, p. 202.

#### Mệnh đề 20 {#ts-iv-s3-prop-20 .statement tag=031K}

Các không gian Sobolev $W^{k,p}(U)$ và $W^{k,p}_0$ (U) là các không gian Banach kiểu đếm được. Đặc biệt, các không gian $H^k(U)$ và $H^k_0(U)$ là các không gian Hilbert kiểu đếm được.

Chỉ cần chứng minh các khẳng định liên quan đến $W^{k,p}(U)$.

Gọi I là tập hợp các $\alpha \in \mathbf{N}^n$ sao cho $|\alpha |\leqslant k$. Ánh xạ tuyến tính $u$ từ $W^{k,p}(U)$ vào $L^p(U)^I$ liên kết với $f$ họ $(\partial^{\alpha}f)_{\alpha\in I}$ là đơn ánh; nó liên tục và ngặt theo định nghĩa của chuẩn trên $W^{k,p}(U)$. Để chứng minh rằng $W^{k,p}(U)$ là đầy đủ, chỉ cần chứng minh rằng ảnh của nó qua $u$ là đóng. Bây giờ, gọi $(f_n)_{n\in\mathbf{N}}$ là một dãy trong $W^{k,p}(U)$ sao cho $(u(f_n))_{n\in\mathbf{N}}$ hội tụ. Gọi $(g_{\alpha})_{\alpha\in I}\in L^p(U)^I$ là giới hạn của nó. Với $\alpha \in I$, dãy $(\partial^{\alpha}f_n)_{n\in\mathbf{N}}$ hội tụ trong $L^p(U)$ đến $g_{\alpha}$. a fortiori, sự hội tụ diễn ra trong $\mathscr{D}'(U)$. Đặt $f=g_0$. Với mọi $\varphi \in \mathscr{D}$(U), ta có

$$
\langle \partial^{\alpha}f, \varphi \rangle = (-1)^{|\alpha|}\langle f, \partial^{\alpha}\varphi \rangle
$$

= lim$_{n\rightarrow+\infty}(-1)^{|\alpha|}\langle f_n, \partial^{\alpha}\varphi \rangle =$ lim$_{n\rightarrow+\infty}\langle \partial^{\alpha}f_n, \varphi \rangle =\langle g_{\alpha}, \varphi \rangle$.

Điều này chứng tỏ rằng $g_{\alpha}=\partial^{\alpha}f$ với mọi $\alpha \in I$, do đó $(g_{\alpha})_{\alpha\in I}=u(f)$ thuộc ảnh của $u$.

Không gian $W^{k,p}(U)$ được đồng nhất bởi $u$ với một không gian con của không gian $L^p(U)^I$; không gian sau là kiểu đếm được (Mệnh đề 2 của IV, p. 180 và TG, IX, p. 19, Hệ quả, (ii))), do đó điều tương tự cũng đúng với $W^{k,p}(U) ($loc. cit., (i)).

#### Mệnh đề 21 {#ts-iv-s3-prop-21 .statement tag=031L}

Gọi N là chuẩn Euclid trên $\mathbf{R}^n$. Gọi $k$ là một số nguyên $\geqslant 0$. Không gian Sobolev $H^k(\mathbf{R}^n)$ là không gian các $f\in \mathscr{S}'(\mathbf{R}^n)$ sao cho $(1 + N^k)\mathscr{F}(f)$ thuộc $L^2(\mathbf{R}^n)$.

Ta tiến hành bằng quy nạp theo $k$. Khi $k= 0$, kết quả là một hệ quả của định lý Plancherel (II, p. 215, th. 1). Giả sử rằng $k= 1$. Với $f\in \mathscr{S}'(\mathbf{R}^n)$, ta có $(1 + N)\mathscr{F}f\in L^2(\mathbf{R}^n)$ khi và chỉ khi $f\in L^2(\mathbf{R}^n)$ và $N\mathscr{F}f\in L^2(\mathbf{R}^n)$. Hơn nữa, $N\mathscr{F}\in L^2(\mathbf{R}^n)$ khi và chỉ khi, với mọi $\alpha \in \mathbf{N}^n$ sao cho $|\alpha |= 1$, ta có $X^{\alpha}\mathscr{F}f\in L^2(\mathbf{R}^n)$. Vì ta có $\mathscr{F}(\partial^{\alpha}f) = 2i\pi X^{\alpha}\mathscr{F}f$, điều kiện này có nghĩa là $\mathscr{F}(\partial^{\alpha}f)\in L^2(\mathbf{R}^n)$ với mọi $\alpha$ sao cho $|\alpha |= 1$, nghĩa là, $\partial^{\alpha}f\in L^2(\mathbf{R}^n)$ với mọi $\alpha$ sao cho $|\alpha |= 1$. Suy ra mệnh đề là đúng với $k= 1$.

Bây giờ giả sử rằng $k\geqslant$ 2 và mệnh đề liên quan đến $H^{\ell}(\mathbf{R}^n)$ là đúng với mọi số nguyên dương $\ell \leqslant k-1$. Cho $f\in \mathscr{S}'(\mathbf{R}^n)$. Theo định nghĩa, ta có $f\in H^k(\mathbf{R}^n)$ khi và chỉ khi $f\in L^2(\mathbf{R}^n)$ và, với mọi $\beta \in \mathbf{N}^n$ sao cho $|\beta |\leqslant 1$, phân phối $\partial^{\beta}f$ thuộc $H^{k-1}(\mathbf{R}^n)$. Điều này tương đương, theo giả thiết quy nạp, với việc $f\in L^2(\mathbf{R}^n)$ và $(1 + N^{k-1})\mathscr{F}(\partial^{\beta}f)\in L^2(\mathbf{R}^n)$ với mọi $\beta \in \mathbf{N}^n$ sao cho $|\beta |\leqslant 1$. Vì $\mathscr{F}(\partial^{\beta}f) = (2i\pi X)^{|\beta|}\mathscr{F}(f)$, điều kiện $f\in H^k(\mathbf{R}^n)$ tương đương với việc nói rằng $\mathscr{F}f\in L^2(\mathbf{R}^n)$ và $(1 + N^{k-1})X^{\beta}\mathscr{F}f\in L^2(\mathbf{R}^n)$ với $\beta \in \mathbf{N}^n$ sao cho $|\beta |\leqslant 1$.

Các bất đẳng thức

$$
1 + N^k\leqslant 1 + N^{k-1}\sum_{\beta|\beta\in|\mathbf{N}\leqslant 1^n}|X^{\beta}|\leqslant 1 +n^{1/2}N^k\leqslant (1 +n^{1/2})(1 + N^k)
$$

khi đó suy ra rằng $f\in H^k(\mathbf{R}^n)$ khi và chỉ khi $(1+N^k)\mathscr{F}\in L^2(\mathbf{R}^n)$.

## BÀI TẬP {#ts-iv-s3-exercises}

Xem [bài tập cho § 3](exercises/s3/).

[^1]: Chú ý rằng chính do một sai lầm mà phát biểu của mệnh đề này bao gồm trường hợp $p= +\infty$.
