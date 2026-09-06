---
book: ts
book_title: Théories spectrales
chapter: III
chapter_title: APPLICATIONS LINÉAIRES COMPACTES ET PERTURBATIONS
section: 2
section_title: Exemples d’applications linéaires compactes
lang: vi
source: ts-iii-v-fr
book_pages: TS III.23-TS III.39, TS III.118-TS III.120
pdf_pages: 0037-0053, 0132-0134
extraction: native
subsections:
    - "no": 1
      title: Endomorphismes de trace finie, de Hilbert–Schmidt et de puissance $p^{\mathbf{e}}$ nucléaire
      page: 23
      pdf_page: 37
    - "no": 2
      title: Opérateurs diagonaux dans des espaces de suites
      page: 23
      pdf_page: 37
    - "no": 3
      title: Applications linéaires à valeurs dans un espace de fonctions continues définies par un noyau
      page: 25
      pdf_page: 39
    - "no": 4
      title: Applications linéaires entre espaces de Lebesgue définies par un noyau
      page: 26
      pdf_page: 40
    - "no": 5
      title: Restriction d’applications différentiables
      page: 34
      pdf_page: 48
    - "no": 6
      title: Restriction de sections différentiables d’un fibré vectoriel
      page: 35
      pdf_page: 49
    - "no": 7
      title: Restriction de sections analytiques d’un fibré vectoriel
      page: 37
      pdf_page: 51
statements: 26
exercises: 4
content_sha256: 5a995f82984a5c56aa9709453f8d68ea9b28bc839c1f9935136996a9f2017036
translated_from: content/en-mt/ts/III/02_s2_exemples_d_applications_lineaires.md
source_lang: en-mt
translation_method: machine
source_content_sha256: 4e5b73807c51c43f4658e3d4c0aa12802558831c80f1a39336cae718bffa14c0
translation_model: gpt-5.4
translation_run: translate-vi-4e5cd7c9
glossary_version: 34
glossary_terms_sha256: c29d52b43b886b439fd6faaa8dc33a9a53d9e7e348204a05e674161b558a8a91
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 2. VÍ DỤ VỀ CÁC ÁNH XẠ TUYẾN TÍNH COMPACT

### 1. Các tự đồng cấu có vết hữu hạn, thuộc lớp Hilbert–Schmidt, và có lũy thừa hạt nhân $p^{\mathbf{e}}$

*Cho E và F là các không gian Hilbert. Mọi tự đồng cấu của E có vết hữu hạn (EVT, V, p. 49, Def. 7 và p. 50, Def. 8) đều compact (IV, p. 165, hệ quả 1); mọi ánh xạ Hilbert–Schmidt từ E vào F (EVT, V, p. 51, Def. 9) đều compact (IV, p. 165, hệ quả 2).

Với mọi số thực $p\geqslant 1$, không gian vectơ $\mathscr{L}_p(E; F)$ của các ánh xạ tuyến tính từ E vào F có lũy thừa hạt nhân $p^e$ được chứa trong $\mathscr{L}^c(E; F) ($x. IV, p. 169, Nhận xét 2 khi $p= 1).*$

### 2. Các toán tử đường chéo trong các không gian dãy

Cho I là một tập hợp khác rỗng. Nhắc lại rằng (EVT, I, p. 4 và p. 5) không gian vectơ của các họ bị chặn $x= (x_i)_{i\in I}$ gồm các phần tử của $\mathbf{C}$, được trang bị chuẩn $\|x\|=$ sup$_i|x_i|$, là một không gian Banach được ký hiệu bởi $\ell^{\infty}_{\mathbf{C}}(I)$.

Cho $p$ là một phần tử của $[1,+\infty [$. Không gian $\ell^p_{\mathbf{C}}(I)$ của các họ $x= (x_i)_{i\in I}$ gồm các phần tử của $\mathbf{C}$ sao cho họ $(|x_i|^p)$ là khả tổng là một không gian vectơ trên đó ánh xạ $x\mapsto  \|x\|= (\sum_i|x_i|^p)^{1/p}$ là một chuẩn biến nó thành một không gian Banach. Nếu người ta trang bị cho không gian I tôpô rời rạc và độ đo sao cho $\mu(\{x\}) = 1$ với mọi $x\in I$, thì không gian này không gì khác hơn là không gian Banach $L^p_{\mathbf{C}}(I, \mu)$. Khi $p= 1$ hoặc $p= 2$, ký hiệu này do đó trùng với ký hiệu của EVT, I, p. 4 và EVT, V, p. 18 (x. INT, IV, p. 141, §4, No.$^o1$, ví dụ).

Với các họ $x= (x_i)_{i\in I}$ và $y= (y_i)_{i\in I}$ các số phức, người ta ký hiệu bởi $xy$ họ $(x_iy_i)_{i\in I}$.

#### Mệnh đề 1 {#ts-iii-s2-prop-1 .statement tag=02QK}

Cho $\lambda = (\lambda_i)_{i\in I}$ là một họ bị chặn gồm các phần tử của $\mathbf{C}$. Cho $p$ là một phần tử của $[1,+\infty ]$. Cho E là không gian Banach $\ell^p_{\mathbf{C}}(I)$.

a) Với mọi $x\in E$, ta có $\lambda x\in E$ và ánh xạ $u:x\mapsto \lambda x$ là một tự đồng cấu liên tục của E, có phổ trong đại số Banach $\mathscr{L}(E)$ bằng bao đóng trong $\mathbf{C}$ của tập các $\lambda_i$, và có chuẩn bằng sup$_i|\lambda_i|$;

b) Tự đồng cấu $u$ là compact nếu và chỉ nếu với mọi số thực $\varepsilon  >0$, tập hợp các phần tử $i\in I$ sao cho $|\lambda_i|\geqslant \varepsilon$ là hữu hạn.

Với ký hiệu của mệnh đề, tự đồng cấu $x\mapsto \lambda x$ được gọi là một tự đồng cấu đường chéo của $\ell^p_{\mathbf{C}}(I)$.

Hãy chứng minh mệnh đề. Đặt C = sup$_i|\lambda_i|$. Cho $x\in E$. Ta có các bất đẳng thức

$\sum_{i\in I}|\lambda_ix_i|^p\leqslant C^p\|x\|^p$, nếu $p\not = +\infty$

sup$_{i\in I}|\lambda_ix_i|\leqslant C\|x\|$, nếu $p= +\infty$.

Điều đó chứng tỏ rằng $\lambda x\in E$. Do đó ánh xạ $x\mapsto \lambda x$ là một tự đồng cấu của E, và các bất đẳng thức này chứng tỏ rằng nó có chuẩn $\leqslant C$.

Với $j\in I$, ký hiệu bởi $e_j$ phần tử $(x_i)_{i\in I}$ của $\ell^p_{\mathbf{C}}(I)$ sao cho $x_j= 1$ và $x_i= 0$ nếu $i\not =j$. Khi đó ta có $u(e_j) =\lambda_je_j$ với mọi $j\in I$, điều này cho thấy rằng $\lambda_j$ thuộc phổ của $u$. Vì phổ của $u$ là đóng, bao đóng trong $\mathbf{C}$ của tập các $\lambda_i$ được chứa trong phổ của $u$. Vì phổ của $u$ được chứa trong đĩa tâm 0 và bán kính $\|u\|($I, p. 24, Định lý 1 và công thức (3) của I, p. 21), ta suy ra bất đẳng thức $C\leqslant \|u\|$, do đó $\|u\|= C$.

Đảo lại, nếu $\lambda \in \mathbf{C}$ không là điểm dính của tập các $\lambda_i$, thì họ $((\lambda_i-\lambda )^{-1})_{i\in I}$ bị chặn. Điều đi trước vì vậy cho thấy rằng ánh xạ tuyến tính $x\mapsto ((\lambda -\lambda_i)^{-1}x_i)_{i\in I}$ là một tự đồng cấu của E. Nó là nghịch đảo của $u-\lambda 1_E$, và do đó $\lambda$ không thuộc phổ của $u$. Điều này chứng minh a).

Bây giờ chứng minh b). Giả sử rằng tự đồng cấu $u$ là compact. Cho $\varepsilon  >0$. Ký hiệu bởi J tập các $i\in I$ sao cho $|\lambda_i|\geqslant \varepsilon$. Tập các phần tử $e_i$ với $i\in J$ là bị chặn trong E. Ảnh của nó bởi $u$, gồm các phần tử $\lambda_ie_i$ với $i\in J$, vì vậy là tương đối compact trong E (Nhận xét 1 của III, p. 2). Vì $\|\lambda_ie_i-\lambda_je_j\|\geqslant \varepsilon$ với mọi cặp phần tử $i\not =j$ trong J, điều này chỉ có thể xảy ra nếu tập J là hữu hạn.

Ta chứng minh mệnh đề đảo lại. Cho J là một tập con hữu hạn của I và ký hiệu bởi $z_J= (z_{J,i})_{i\in I}$, trong đó $z_{J,i}=\lambda_i$ với $i\in J$ và $z_{J,i}= 0$ với $i\in I$- J ; họ $z_J$ xác định một tự đồng cấu hạng hữu hạn $u_J:x\mapsto z_Jx$ của E. Theo điều đi trước, chuẩn của ánh xạ tuyến tính $u-u_J$ bị chặn trên bởi cận trên trong $\mathbf{R}_+$ của họ $(|\lambda_i|)_{i\in I-J}$. Giả thiết kéo theo rằng với mọi $\varepsilon  >0$, tồn tại một tập con hữu hạn $J\subset I$ sao cho cận trên này là $\leqslant \varepsilon$. Suy ra ánh xạ $u$ là điểm dính của $\mathscr{L}^f$(E), và do đó nó là compact (III, p. 4, hệ quả của Mệnh đề 2).

#### Nhận xét 1 {#ts-iii-s2-n2-rem-1 .statement tag=02QL}

Giả thiết của mệnh đề b) luôn đúng nếu I là hữu hạn. Khi tập I là vô hạn, điều đó có nghĩa là họ $(\lambda_i)_{i\in I}$ hội tụ tới 0 theo bộ lọc các phần bù của các tập con hữu hạn của I; đặc biệt, tập các $i\in I$ sao cho $\lambda_i\not = 0$ khi đó là đếm được.

#### Nhận xét 2 {#ts-iii-s2-n2-rem-2 .statement tag=02QM}

*Về sau sẽ thấy (xem IV, p. 149, định lý 1) rằng khi $p= 2$, mọi tự đồng cấu compact chuẩn tắc của không gian Hilbert $\ell^2_{\mathbf{C}}(I)$ đều có dạng $u=w\circ v\circ w^{-1}$, trong đó $v$ là một tự đồng cấu compact đường chéo và $w$ là một tự đồng cấu unita (EVT, V, p. 40) của không gian Hilbert $\ell^2_{\mathbf{C}}(I).*$

### 3. Các ánh xạ tuyến tính nhận giá trị trong một không gian các hàm liên tục được định nghĩa bởi một hạt nhân

Ở đây ta lấy $K =\mathbf{C}$. Cho X và Y là các không gian tôpô compact địa phương. Cho $\mu$ là một độ đo phức trên X và $k$ là một ánh xạ từ $X\times Y$ vào $\mathbf{C}$ có hai tính chất sau:

(i) Với mọi $y\in Y$, hàm $k_y:x\mapsto k(x, y)$ từ X vào $\mathbf{C}$ là $\mu$-khả tích;

(ii) Ánh xạ $y\mapsto k_y$ từ Y vào $\mathscr{L}_{\mathbf{C}}^1(X, \mu)$ là liên tục.

Trang bị cho không gian $\mathscr{C}(Y)$ các hàm liên tục trên Y nhận giá trị phức tôpô hội tụ compact. Với $f$ trong $\mathscr{L}_{\mathbf{C}}^{\infty}(X, \mu)$, định nghĩa $\widetilde{k}(f) : Y\rightarrow \mathbf{C}$ bởi

$$
\widetilde{k}(f)(y) =\int_Xk(x, y)f(x)d\mu(x) =\int_Xk_yf d\mu \tag{1}
$$

Ánh xạ $h\mapsto \int_Xhf d\mu$ là một dạng tuyến tính liên tục trên $\mathscr{L}_{\mathbf{C}}^1(X, \mu)$, nên điều kiện (ii) cho thấy rằng hàm $\widetilde{k}(f)$ là liên tục.

#### Mệnh đề 2 {#ts-iii-s2-prop-2 .statement tag=02QN}

Ánh xạ $\widetilde{k}$ từ $\mathscr{L}_{\mathbf{C}}^{\infty}(X, \mu)$ vào $\mathscr{C}(Y)$ là compact.

Với mọi $y$ và $y'$ trong Y, ta có

$$
|\widetilde{k}(f)(y)|\leqslant \|k_y\|_1\|f\|_{\infty},|\widetilde{k}(f)(y)-\widetilde{k}(f)(y')|\leqslant \|k_y-k_{y'}\|_1\|f\|_{\infty}
$$

Theo định lý Ascoli (TG, X, p. 18, hệ quả 2), suy ra ảnh qua $\widetilde{k}$ của quả cầu đơn vị của $\mathscr{L}_{\mathbf{C}}^{\infty}(X;\mu)$ là compact tương đối trong $\mathscr{C}(Y)$.

#### Hệ quả {#ts-iii-s2-n3-cor-1 .statement tag=02QO}

Cho X là một không gian tôpô compact, Y là một không gian tôpô compact địa phương, $\mu$ là một độ đo phức trên X, và $k$ là một ánh xạ liên tục từ $X\times Y$ vào $\mathbf{C}$. Khi đó công thức (1) xác định một ánh xạ tuyến tính compact, vẫn ký hiệu là $\widetilde{k}$, từ $\mathscr{C}(X)$ được trang bị tôpô hội tụ đều vào $\mathscr{C}(Y)$ được trang bị tôpô hội tụ compact.

Hãy kiểm tra các điều kiện (i) và (ii) đối với $k$. Với mọi $y\in Y$, ánh xạ $k_y$ liên tục trên không gian compact X, do đó là $\mu$-khả tích. Hơn nữa, ánh xạ $y\mapsto k_y$ là liên tục từ Y vào $\mathscr{C}(X)$ vì X compact (TG, X, p. 28, định lý 3). Vì $\|k_y-k_{y'}\|_1\leqslant \|\mu\| \|k_y-k_{y'}\|$ với mọi $(y, y')\in Y^2$, ánh xạ này từ Y vào $\mathscr{L}_{\mathbf{C}}^1(X, \mu)$ là liên tục. Theo mệnh đề 2, ánh xạ $\widetilde{k}$ từ $\mathscr{L}_{\mathbf{C}}^{\infty}(X, \mu)$ vào $\mathscr{C}(Y)$ là compact. Hợp thành với ánh xạ chính tắc $\mathscr{C}(X)\rightarrow \mathscr{L}_{\mathbf{C}}^{\infty}(X, \mu)$, ta thu được một ánh xạ tuyến tính compact từ $\mathscr{C}(X)$ vào $\mathscr{C}(Y)$.

### 4. Các ánh xạ tuyến tính giữa các không gian Lebesgue được định nghĩa bởi một hạt nhân

Ở đây ta lấy $K =\mathbf{C}$. Cho X là một không gian tôpô compact địa phương được trang bị một độ đo dương $\mu$. Với mọi $r\in [1,+\infty ]$, ta viết $\mathscr{L}^r(X) =\mathscr{L}_{\mathbf{C}}^r(X, \mu)$ và $L^r(X) = L^r_{\mathbf{C}}(X, \mu)$. Khi $r\in [1,+\infty [$, ta đồng nhất đối ngẫu của $L^r(X)$ với $L^{r'}(X)$, trong đó $r'$ là số mũ liên hợp của $r$, sao cho $1/r+ 1/r'= 1$ (INT, V, p. 61, § 5, n$^o8$, th. 4). Ta viết $\|f\|_r$ để chỉ chuẩn (hoặc nửa chuẩn) của $f\in L^r(X)$ (hoặc $f\in \mathscr{L}^r(X)$).

Ta nhắc lại rằng một tập con A của X được gọi là $\mu$-vừa phải (INT, V, p. 4, § 1, n$^o2$) nếu nó được chứa trong hợp của một dãy các tập hợp $\mu$-khả tích, và rằng một hàm $f$ xác định trên X với giá trị trong một không gian vectơ hoặc trong $\overline{\mathbf{R}}$ là $\mu$-vừa phải nếu nó bằng không trên phần bù của một tập con $\mu$-vừa phải của X. Nếu 1 $\leqslant p <+\infty$ và $f\in \mathscr{L}^p$(X), thì $f$ là vừa phải (INT, V, p. 9, § 1, n$^o3$, cor.). Nếu $f$ là $\mu$-vừa phải, thì $f g$ là $\mu$-vừa phải với mọi hàm $g$.

Cho $p$ và $q$ là các phần tử của$]1,+\infty [$. Cho X và Y là các không gian tôpô compact địa phương, lần lượt được trang bị các độ đo dương $\mu$ và $\nu$. Ta trang bị cho không gian $X\times Y$ (tương ứng $Y\times X$) độ đo tích $\mu\otimes \nu$ (tương ứng $\nu \otimes \mu$).

Ta viết $\mathscr{N}^{p,q}(X\times Y, \mu\otimes \nu )$, hoặc đơn giản là $\mathscr{N}^{p,q}(X\times Y)$, để chỉ tập hợp các ánh xạ $(\mu\otimes \nu$)-đo được $k$ từ $X\times Y$ vào $\mathbf{C}$ sao cho tồn tại một số thực $C\geqslant 0$ thỏa mãn

$$
\int_{X\times Y}^*|k(x, y)f(x)g(y)|d(\mu\otimes \nu )(x, y)\leqslant C\|f\|_p\|g\|_q \tag{2}
$$

với mọi hàm $f\in \mathscr{L}^p(X)$ và $g\in \mathscr{L}^q(Y)$. Khi đó ta viết $\|k\|_{p,q}$ để chỉ cận dưới lớn nhất của tập hợp các số thực C có tính chất này.

#### Nhận xét {#ts-iii-s2-n4-rem-1 .statement tag=02QP}

Cho $f\in \mathscr{L}^p(X)$ và $g\in \mathscr{L}^q(Y)$. Vì $p <+\infty$ và $q <+\infty$, các hàm $f$ và $g$ là vừa phải, và hàm xác định bởi $(x, y)\mapsto f(x)g(y)$ là $(\mu\otimes \nu$)-vừa phải (x. INT, V, p. 92, § 8, n$^o3$, Hệ quả 2). Do đó, hàm $(x, y)\mapsto k(x, y)f(x)g(y)$ là $(\mu\otimes \nu$)-vừa phải, và đặc biệt tích phân trên của giá trị tuyệt đối của nó trùng với tích phân trên cốt yếu (INT, V, p. 6, § 1, n$^o3$, Mệnh đề 7).

Tập hợp $\mathscr{N}^{p,q}(X\times Y)$ là một không gian con vectơ của không gian các hàm từ $X\times Y$ vào $\mathbf{C}$ và ánh xạ xác định bởi $k\mapsto  \|k\|_{p,q}$ là một nửa chuẩn trên $\mathscr{N}^{p,q}(X\times Y)$.

#### Bổ đề 1 {#ts-iii-s2-lem-1 .statement tag=02QQ}

Cho $k\in \mathscr{N}^{p,q}(X\times Y)$. Hàm $k$ khả tích địa phương đối với $(\mu\otimes \nu )$.

Ánh xạ $k$ là $(\mu\otimes \nu$)-đo được theo giả thiết. Cho A là một tập con compact của $X\times Y$. Tồn tại các tập con compact $B\subset X$ và $C\subset Y$ sao cho $A\subset B\times C$. Áp dụng (2) cho các hàm đặc trưng $\varphi_B$ của B và $\varphi_C$ của C, ta được

$$
\int_{X\times Y}^*|k(x, y)|\varphi_A(x, y)d(\mu\otimes \nu )(x, y)
$$

$$
\leqslant \int_{X\times Y}^*|k(x, y)|\varphi_B(x)\varphi_C(y)d(\mu\otimes \nu )(x, y)<+\infty
$$

do đó suy ra kết quả (INT, V, p. 41, §5, n$^o1$, Mệnh đề 1 và Định nghĩa 1).

#### Mệnh đề 3 {#ts-iii-s2-prop-3 .statement tag=02QR}

a) Cho $k\in \mathscr{N}^{p,q}(X\times Y)$. Với $f\in \mathscr{L}^p(X)$ và $g\in \mathscr{L}^q(Y)$, hàm

$$
(x, y)\mapsto k(x, y)f(x)g(y)
$$

là $(\mu\otimes \nu )$-khả tích và tồn tại một ánh xạ duy nhất $u_k$ từ $L^p(X)$ vào $L^{q'}(Y)$ sao cho

$$
\langle g, u_k(f)\rangle =\int_{X\times Y}k(x, y)f(x)g(y)d(\mu\otimes \nu )(x, y)
$$

với mọi $f\in L^p(X)$ và $g\in L^q(Y)$. Ánh xạ $u_k$ là tuyến tính và liên tục, và chuẩn của nó là $\leqslant \|k\|_{p,q}$;

b) Cho $k\in \mathscr{N}^{p,q}(X\times Y)$. Ta có $u_k= 0$ khi và chỉ khi $k$ là không đáng kể địa phương đối với $(\mu\otimes \nu )$;

c) Ánh xạ liên kết $u_k$ với $k$ là một ánh xạ tuyến tính liên tục từ không gian nửa chuẩn $\mathscr{N}^{p,q}(X\times Y)$ vào không gian Banach $\mathscr{L}(L^p(X); L^{q'}(Y))$, sao cho $\|u_k\|\leqslant \|k\|_{p,q}$ với mọi $k\in \mathscr{N}^{p,q}(X\times Y)$.

Cho $k\in \mathscr{N}^{p,q}(X\times X)$. Theo định nghĩa, hàm từ $X\times Y$ vào $\mathbf{C}$ được xác định bởi $(x, y)\mapsto k(x, y)f(x)g(y)$ là khả tích đối với $(\mu\otimes \nu$) khi $f\in \mathscr{L}^p(X)$ và $g\in \mathscr{L}^q$(Y), và ánh xạ

$$
b_k: (f, g)\mapsto \int_{X\times Y}k(x, y)f(x)g(y)d(\mu\otimes \nu )(x, y)
$$

là một ánh xạ song tuyến tính liên tục từ $L^p(X)\times L^q(Y)$ vào $\mathbf{C}$. Do đó, với mọi $f\in L^p$(X), tồn tại duy nhất $h\in L^{q'}(Y)$ sao cho $b_k(f, g) =$ $\langle g, h\rangle$ với mọi $g\in L^q(Y)$; ta viết $u_k(f) =h$. Theo (2), ta có $\|u_k(f)\|_{q'}\leqslant \|k\|_{p,q}\|f\|_p$; ánh xạ $u_k$ là tuyến tính và liên tục, có chuẩn $\leqslant \|k\|_{p,q}$. Hơn nữa, ánh xạ $k\mapsto u_k$ là tuyến tính, và các khẳng định a) và c) suy ra từ điều này.

Ta chứng minh b). Giả sử rằng $k$ là địa phương không đáng kể đối với $(\mu\otimes \nu$). Cho $f\in \mathscr{L}^p(X)$ và $g\in \mathscr{L}^q(Y)$; hàm xác định trên $X\times Y$ bởi $(x, y)\mapsto k(x, y)f(x)g(y)$ là vừa phải đối với $(\mu\otimes \nu$). Vì nó là địa phương không đáng kể đối với $(\mu\otimes \nu$), nên nó là không đáng kể (INT, V, p. 7, § 1, No.$^o2$, Hệ quả 1). Do đó, ta có $\langle u_k(f), g\rangle =b_k(f, g) = 0$. Suy ra $u_k= 0$.

Ngược lại, cho $k\in \mathscr{N}^{p,q}(X\times Y)$ sao cho $u_k= 0$. Hàm $k$ là địa phương khả tích đối với $(\mu\otimes \nu$) (Bổ đề 1). Với mọi hàm $f\in \mathscr{K}(X)$ và $g\in \mathscr{K}$ (Y), ta có

$$
\langle g, u_k(f)\rangle =\int_{X\times Y}f(x)g(y)k(x, y)d(\mu\otimes \nu )(x, y)
$$

do đó độ đo $k\cdot (\mu\otimes \nu )$ trên $X\times Y$ bằng không (xem INT, III, p. 82, § 4, No.$^o1$, Định lý 1). Điều đó có nghĩa là $k$ là địa phương không đáng kể đối với $(\mu\otimes \nu$) (INT, V, p. 46, §5, No.$^o3$, Hệ quả 2).

#### Định nghĩa 1 {#ts-iii-s2-def-1 .statement tag=02QS}

Cho $k\in \mathscr{N}^{p,q}(X\times Y)$. Ta nói rằng ánh xạ $u_k$ là toán tử tích phân với hạt nhân $k$ từ $L^p(X)$ vào $L^{q'}(Y)$.

Với $k\in \mathscr{N}^{p,q}(X\times Y)$ và $f\in \mathscr{L}^p$(X), đôi khi người ta cũng ký hiệu bởi $u_k(f)$ ảnh qua $u_k$ của lớp của $f$ trong $L^p(X)$.

#### Mệnh đề 4 {#ts-iii-s2-prop-4 .statement tag=02QT}

Cho $k\in \mathscr{N}^{p,q}(X\times Y)$ và $f\in \mathscr{L}^p(X)$. Ánh xạ xác định trên X bởi $x\mapsto k(x, y)f(x)$ là $\mu$-khả tích với mọi $y$ ở ngoài một tập địa phương $\nu$-không đáng kể, và $u_k(f)$ trùng với lớp của hàm

$$
y\mapsto \int_Xk(x, y)f(x)d\mu(x)
$$

được xác định địa phương $\nu$-hầu khắp nơi.

Ký hiệu $Y'$ là tập hợp các $y\in Y$ sao cho ánh xạ $x\mapsto k(x, y)f(x)$ không $\mu$-khả tích. Lấy $y\in Y$ và lấy C là một lân cận compact của $y$, có hàm đặc số được ký hiệu bởi $\varphi$. Theo điều kiện (2) áp dụng cho $f$ và $\varphi$, hàm $(x, y)\mapsto k(x, y)f(x)\varphi (y)$ là khả tích trên $X\times Y$ đối với độ đo $\mu\otimes \nu$. Theo định lý Lebesgue-Fubini (INT, V, p. 96, § 8, No.$^o4$, Định lý 1, a)), hàm $x\mapsto k(x, y)f(x)\varphi (y)$ là $\mu$-khả tích với $y$ ở ngoài một tập $\nu$-không đáng kể $Y_C$. Vì $Y'\cap C\subset Y_C$, suy ra $Y'$ là địa phương $\nu$-không đáng kể trong Y (INT, IV, p. 172, § 5, No.$^o2$, Định nghĩa 3).

Ký hiệu $h$ là ánh xạ được xác định địa phương $\nu$-hầu khắp nơi trên Y bởi $y\mapsto \int k(x, y)f(x)d\mu$. Nó địa phương $\nu$-khả tích (INT, V, loc. cit.). Lấy $g\in \mathscr{K}(Y)$. Ta có

$$
\langle g, u_k(f)\rangle =\int_{X\times Y}k(x, y)f(x)g(y)d(\mu\otimes \nu )(x, y)
$$

$$
=\int_Y\int_Xk(x, y)f(x)g(y)d\mu(x)d\nu (y)
$$

$$
=\int_Yg(y)h(y)d\nu (y)
$$

(INT, V, loc. cit.). Do đó $u_k(f) =h$ địa phương $\nu$-hầu khắp nơi (x. INT, V, p. 46, § 5, No.$^o3$, Hệ quả 2).

#### Mệnh đề 5 {#ts-iii-s2-prop-5 .statement tag=02QU}

Không gian $\mathscr{L}^{p'}(X\times Y)$ được chứa trong $\mathscr{N}^{p,p}(X\times Y)$. Ánh xạ tuyến tính từ $\mathscr{L}^{p'}(X\times Y)$ vào $\mathscr{L}(L^p(X); L^{p'}(Y))$ xác định bởi $k\mapsto u_k$ gây ra, sau khi chuyển qua thương, một ánh xạ tuyến tính liên tục đơn ánh từ $L^{p'}(X\times Y)$ vào $\mathscr{L}(L^p(X); L^{p'}(Y))$.

Lấy $k\in \mathscr{L}^{p'}(X\times Y)$. Ánh xạ $k$ là đo được (INT, IV, p. 84, § 5, No.$^o6$, định lý 5). Lấy $f\in \mathscr{L}^p(X)$ và $g\in \mathscr{L}^p(Y)$. Hàm $h: (x, y)\mapsto f(x)g(y)$ thuộc $\mathscr{L}^p(X\times Y)$ và $\|h\|_p=\|f\|_p\|g\|_p$ (INT, V, p. 95, § 8, No.$^o3$, Hệ quả 2). Do đó hàm $hk$ là khả tích trên $X\times Y$ và ta có

$$
(\mu\otimes \nu )^*(|hk|)\leqslant \|k\|_{p'}\|h\|_p=\|k\|_{p'}\|f\|_p\|g\|_p
$$

theo bất đẳng thức Hölder (INT, IV, p. 208, § 6, No.$^o4$, Định lý 2), điều này chứng minh rằng $k\in \mathscr{N}^{p,p}(X\times Y)$ với $\|k\|_{p,p}\leqslant \|k\|_{p'}$.

Vì $p'\not = +\infty$, mọi hàm $k\in \mathscr{L}^{p'}(X\times Y)$ đều ôn hòa (INT, V, p. 9, § 1, No.$^o3$, Hệ quả), và khẳng định cuối cùng khi đó suy ra từ Mệnh đề 3, b) và c).

Với mọi hàm $k: X\times Y\rightarrow \mathbf{C}$ và mọi $y\in Y$, ta ký hiệu bởi $k_y$ ánh xạ từ X vào $\mathbf{C}$ được xác định bởi $k_y(x) =k(x, y)$, và ta ký hiệu bởi $k_{\circ}$ ánh xạ từ Y vào $\mathscr{F}(X;\mathbf{C})$ được xác định bởi $y\mapsto k_y$. Tương tự, ta cũng sẽ ký hiệu bởi cùng một ký hiệu ánh xạ từ Y vào không gian các hàm được xác định $\mu$-hầu khắp nơi trên X mà gán cho $y$ lớp của $k_y$.

Với mọi hàm $k$ từ $X\times Y$ vào $\mathbf{C}$, ta đặt

$$
N_{p',q'}(k)=\left(\int_Y^\bullet N_{p'}(k_y)^{q'}d\nu(y)\right)^{1/q'}.
$$

Đó là một phần tử của $[0,+\infty ]$.

#### Bổ đề 2 {#ts-iii-s2-lem-2 .statement tag=02QV}

Với mọi $k\in \mathscr{L}^{p'}(X\times Y)$, ta có $N_{p', p'}(k) =\|k\|_{p'}$.

Cho $k\in \mathscr{L}^{p'}(X\times Y)$. Theo INT, V, p. 96, § 8, No.$^o4$, Định lý 1, a), tập hợp $Y'$ gồm các phần tử $y\in Y$ sao cho hàm $|k_y|^{p'}$ không $\mu$-khả tích là $\nu$-không đáng kể; hơn nữa, hàm được xác định bởi $y\mapsto \mu(|k_y|^{p'})$ trên Y - $Y'$ và bằng không trên $Y'$ là $\nu$-khả tích và thỏa mãn

$$
\|k\|^{p'}_{p'}=\int_{X\times Y}|k(x, y)|^{p'}d(\mu\otimes \nu )(x, y) =\int_Y\mu(|k_y|^{p'})d\nu = N_{p', p'}(k)^{p'}
$$

Ta ký hiệu bởi $\mathscr{L}^{p',q'}(X,Y, \mu, \nu )$, hoặc đơn giản bởi $\mathscr{L}^{p',q'}(X,Y)$, không gian vectơ phức của các hàm $k$ từ $X\times Y$ vào $\mathbf{C}$, đo được đối với $(\mu\otimes \nu$), sao cho, với $\nu$-hầu mọi $y\in Y$, ánh xạ $k_y$ thuộc $\mathscr{L}^{p'}$(X), và sao cho ánh xạ $k_{\circ}$ thuộc $\mathscr{L}_{L^{p'}(X)}^{q'}(Y, \nu )$ (INT, IV, p. 129, § 3, No.$^o4$, Định nghĩa 2). Ta trang bị cho $\mathscr{L}^{p',q'}(X,Y)$ nửa chuẩn $k\mapsto N_{p',q'}(k)$; chú ý rằng khi đó ta có $N_{p',q'}(k) =\|k_{\circ}\|_{q'}$, trong đó $k_{\circ}$ được xem như một ánh xạ nhận giá trị trong không gian Banach $L^{p'}(X)$.

#### Mệnh đề 6 {#ts-iii-s2-prop-6 .statement tag=02QW}

a) Không gian $\mathscr{L}^{p'}(X\times Y)$ được chứa trong $\mathscr{L}^{p',p'}(X,Y)$, và với $k\in \mathscr{L}^{p'}(X\times Y)$, ta có $N_{p', p'}(k) =\|k\|_{p'}$;

b) Không gian $\mathscr{L}^{p',q'}(X,Y)$ được chứa trong $\mathscr{N}^{p,q}(X\times Y)$ và với $k\in \mathscr{L}^{p',q'}(X,Y)$, ta có $\|k\|_{p,q}\leqslant N_{p',q'}(k)$.

Ta chứng minh mệnh đề a). Cho $k\in \mathscr{L}^{p'}(X\times Y)$. Theo INT, V, p. 96, § 8, n$^o4$, th. 1, a), hàm $k_y$ thuộc $\mathscr{L}^{p'}(X)$ với $\nu$-hầu khắp mọi $y\in Y$.

Cho $\varepsilon  >0$. Tồn tại $h\in \mathscr{K}(X\times Y)$ sao cho $\|k-h\|_{p'}< \varepsilon$. Hàm $h_{\circ}$ là một hàm liên tục có giá compact từ Y vào $L^{p'}(X)$ thỏa mãn

$$
\|k_{\circ}-h_{\circ}\|_{p'}= N_{p',p'}(k-h) =\|k-h\|_{p'}< \varepsilon
$$

theo Bổ đề 2. Suy ra $k_{\circ}$ thuộc $\mathscr{L}_{L^{p'}(X)}^{p'}(Y, \nu )$, nghĩa là $k$ thuộc $\mathscr{L}^{p',p}(X,Y)$. Khi đó Bổ đề 2 chứng minh rằng $N_{p', p'}(k) =\|k\|_{p'}$.

Ta chứng minh mệnh đề b). Cho $k\in \mathscr{L}^{p',q'}(X,Y)$ và cho $f\in \mathscr{L}^p(X)$. Với mọi $y\in Y$, bất đẳng thức Hölder (INT, IV, p. 208, § 6, n$^o4$, th. 2) áp dụng cho $k_y$ suy ra

$$
\int_X^*|k(x, y)f(x)|d\mu(x)\leqslant \|k_y\|_{p'}\|f\|_p
$$

Cho $g\in \mathscr{L}^{q'}(Y)$. Các ánh xạ $f$ và $g$ là vừa phải, vì $p$ và $q'$ là hữu hạn. Do đó, ánh xạ $(x, y)\mapsto f(x)g(y)$ là vừa phải đối với $(\mu\otimes \nu )$ (xem INT, V, p. 92, § 8, n$^o3$, cor. 2), và vì thế ánh xạ $(x, y)\mapsto k(x, y)f(x)g(y)$ là vừa phải đối với $(\mu\otimes \nu$). Theo INT, V, p. 93, § 8, n$^o3$, prop. 7, a), suy ra rằng

$$
\int_{X\times Y}^*|k(x, y)f(x)g(y)|d(\mu\otimes \nu )
$$

$$
=\int_Y^*|g(y)|(\int_X^*|k(x, y)f(x)|d\mu(x))d\nu (y)
$$

$$
\leqslant \|f\|_p\int_Y^*\|k_y\|_{p'}|g(y)|d\nu (y)\leqslant N_{p',q'}(k)\|f\|_p\|g\|_q
$$

lại dùng bất đẳng thức Hölder. Điều này kết thúc chứng minh.

#### Mệnh đề 7 {#ts-iii-s2-prop-7 .statement tag=02QX}

Cho $k\in \mathscr{L}^{p',q'}(X,Y)$. Ánh xạ tuyến tính $u_k$ từ $L^p(X)$ vào $L^{q'}(Y)$ là compact.

Trước hết giả sử rằng $k$ sao cho $k_{\circ}\in \mathscr{K}(Y;\mathscr{L}^{p'}$(X)), và ký hiệu A là giá của $k_{\circ}$. Gọi F là không gian con của $\mathscr{K}(Y,A;\mathscr{L}^{p'}(X, \mu))$ được sinh bởi các hàm $y\mapsto f_2(y)f_1$, trong đó $f_2\in \mathscr{K}(Y,A)$ và $f_1\in \mathscr{L}^{p'}(X)$. Khi $m\in \mathscr{K}(Y;\mathscr{L}^{p'}(X))$ thỏa mãn $m_{\circ}\in F$, ánh xạ tuyến tính $u_m$ có hạng hữu hạn, do đó compact. Hơn nữa, với $m_1$ và $m_2$ trong $\mathscr{K}(Y,A;\mathscr{L}^{p'}$(X)), ta có

$\int'1/q'$

$$
\|u_{m_1}-u_{m_2}\|\leqslant \|m_1-m_2\|_{p',q'}=(_Y\|m_{1,y}-m_{2,y}\|^q_{p'}d\nu (y))
$$

$\leqslant \nu (A)^{1/q'}$ sup$_{y\in Y}N_{p'}(m_{1,y}-m_{2,y})$.

Vì không gian F là trù mật trong $\mathscr{K}(Y,A; L^{p'}(X))$ đối với tôpô hội tụ đều trên A (INT, III, p. 41, § 1, n$^o1$, mệnh đề 1 và INT, III, p. 46, § 1, n$^o2$, mệnh đề 5), suy ra ánh xạ tuyến tính $u_k$ là giới hạn của một dãy các ánh xạ tuyến tính hạng hữu hạn. Do đó nó là compact (hệ quả 1 của III, p. 4).

Xét trường hợp tổng quát. Cho $k\in \mathscr{L}^{p',q'}(X,Y)$. Với mọi $\varepsilon  >0$, tồn tại một ánh xạ $k_{\varepsilon ,\circ}\in \mathscr{K}(Y;\mathscr{L}^{p'}(X))$ sao cho

$$
\|k_{\circ}-k_{\varepsilon ,\circ}\|_{q'}< \varepsilon
$$

Khi đó hàm tương ứng $k_{\varepsilon}: X\times Y\rightarrow \mathbf{C}$ thỏa mãn

$$
\|u_k-u_{k_{\varepsilon}}\|\leqslant \|k-k_{\varepsilon}\|_{p,q}\leqslant N_{p',q'}(k-k_{\varepsilon}) =\|k_{\circ}-k_{\varepsilon ,\circ}\|_{q'}< \varepsilon
$$

Vì $u_{k_{\varepsilon}}$ là compact theo điều đã đi trước, ánh xạ $u_k$ cũng vậy là compact (mệnh đề 2 của III, p. 4).

Đặt $p= 1$ và giả sử $q >1$. Có thể tồn tại các ánh xạ $k: X\times Y\rightarrow \mathbf{C}$ sao cho $k_y\in \mathscr{L}^{\infty}(X)$ với mọi $y\in Y$, và sao cho tích phân

$$
\int_Y^*\|k_y\|^{q'}_{\infty}d\nu (y)
$$

là hữu hạn (đặc biệt, điều kiện (2) của III, p. 27 được thỏa mãn), nhưng sao cho ánh xạ tuyến tính $u_k$ từ $L^1(X)$ vào $L^{q'}(X)$ không compact (bài tập 2 của III, p. 119).

Đặc biệt, từ mệnh đề ta suy ra hệ quả sau:

#### Hệ quả 1 (Hilbert–Schmidt) {#ts-iii-s2-prop-7-cor-1 .statement tag=02QY}

Cho $k\in \mathscr{L}^2(X\times Y)$. Ánh xạ tuyến tính $u_k$ là compact từ $L^2(X)$ vào $L^2(Y)$.

Theo mệnh đề 5, ta có $k\in \mathscr{N}^{2,2}(X\times Y)$, do đó ánh xạ tuyến tính $u_k$ được xác định (mệnh đề 3). Ta có $k\in \mathscr{L}^{2,2}(X\times Y)$ (mệnh đề 6, a)), do đó $u_k$ là compact (mệnh đề 7).

#### Nhận xét {#ts-iii-s2-n4-rem-2 .statement tag=02QZ}

Trong trường hợp $p=q= 2$, nói chung sẽ thuận tiện hơn khi phát biểu đặc trưng hóa của toán tử tích phân $u_k$ bằng tích vô hướng: đó là ánh xạ duy nhất từ $L^2(X)$ vào $L^2(Y)$ sao cho

$$
\langle g|u_k(f)\rangle =\int_{X\times Y}k(x, y)f(x)\overline{g(y)}d(\mu\otimes \nu )(x, y)
$$

với mọi $f\in L^2(X)$ và $g\in L^2(Y)$. Hơn nữa, liên hợp của $u_k$ là ánh xạ tuyến tính $u_{k^*}$, trong đó $k^*\in L^2(Y\times X)$ thỏa mãn $k^*(y, x) =k(x, y)$ với hầu khắp mọi $(y, x)\in Y\times X$. Thật vậy, với mọi $f\in L^2(X)$ và $g\in L^2$(Y), ta có

$$
\langle g|u_k(f)\rangle =\int_{X\times Y}k(x, y)\overline{g(y)}f(x)d(\mu\otimes \nu )(x, y) =\langle u_{k^*}(g)|f\rangle
$$

#### Hệ quả 2 {#ts-iii-s2-prop-7-cor-2 .statement tag=02R0}

Cho G là một nhóm tôpô compact được trang bị một độ đo Haar $\mu$. Cho $p$ là một số thực sao cho $1< p <+\infty$ và $q$ là số mũ liên hợp của $p$. Cho $f\in \mathscr{L}^q(G)$. Đặt $k(x, y) =f(x^{-1}y)$ với mọi $(x, y)\in G\times G$.

a) Ta có $k\in \mathscr{L}^{q,p}(G,G)$;

b) Với $\varphi \in L^p(G)$, tích chập $\varphi *f$ thuộc $L^p(G)$ và ánh xạ tuyến tính $v_f:\varphi \mapsto \varphi *f$ của $L^p(G)$ vào chính nó là liên tục. Nó trùng với tự đồng cấu $u_k$. Đặc biệt, ánh xạ tuyến tính $v_f$ là compắc.

Vì G compắc, hàm $f$ thuộc $\mathscr{L}^1(G)$. Do đó ánh xạ tuyến tính $v_f$ được xác định và liên tục theo INT, VIII, p. 167, § 4, No.$^o5$, Mệnh đề 13.

Ánh xạ $k$ là $(\mu\otimes \mu$)-đo được, và ta có $\|k_y\|_q=\|f\|_q$ với mọi $y\in G$. Vì độ đo $\mu$ bị chặn, suy ra

$$
\int_G\|k_y\|^p_qd\mu(y) =\mu(G)\|f\|^p_q
$$

do đó $k\in \mathscr{L}^{q,p}(G,G)$. Vì vậy ánh xạ tuyến tính $u_k$ là một ánh xạ tuyến tính compắc của $L^p(G)$ vào $L^p(G)$ (Mệnh đề 7).

Cho $\varphi \in \mathscr{K}(G)$. Theo INT, VIII, p. 166, § 4, No.$^o5$, Mệnh đề 11 và Mệnh đề 4 của III, p. 29, khi đó ta có

$$
v_f(\varphi )(y) =\int_G\varphi (x)f(x^{-1}y)d\mu(x)
$$

$$
=\int_G\varphi (x)k(x, y)d\mu(x) =u_k(\varphi )(y)
$$

với hầu khắp mọi $y\in G$. Điều này suy ra $v_f=u_k$.

### 5. Hạn chế của các ánh xạ khả vi

Cho $n$ và $r$ là các số nguyên dương, U là một tập con mở của $\mathbf{R}^n$ và F là một không gian Banach. Ký hiệu $\mathscr{C}^r(U; F)$ là không gian vectơ các ánh xạ lớp $C^r$ từ U vào F, được trang bị tôpô của sự hội tụ compắc $C^r$. Xin nhắc lại rằng đó là cận trên của các tôpô của sự hội tụ đều $C^r$ trên K (VAR, R2, 12.3.10, p. 56), khi K chạy qua tập hợp các tập con compắc của U. Không gian $\mathscr{C}^0(U; F)$ không gì khác hơn là không gian $\mathscr{C}(U; F)$ các ánh xạ liên tục từ U vào F, được trang bị tôpô của sự hội tụ compắc.

#### Bổ đề 3 {#ts-iii-s2-lem-3 .statement tag=02R1}

Cho A là tập hợp các đa chỉ số $\alpha \in \mathbf{N}^n$ sao cho $|\alpha |\leqslant r$ và gọi $u$ là ánh xạ tuyến tính $f\mapsto (\partial^{\alpha}f)_{\alpha\in A}$ từ $\mathscr{C}^r(U; F)$ vào $\mathscr{C}(U; F)^A$.

a) Ánh xạ $u$ là đơn ánh, liên tục, ngặt, và ảnh của nó là đóng.

b) Không gian vectơ tôpô $\mathscr{C}^r(U; F)$ là đầy đủ.

Ánh xạ $u$ là tuyến tính và đơn ánh. Nó liên tục và ngặt theo định nghĩa của tôpô của $\mathscr{C}^r(U; F)$.

Cho $(g_{\alpha})_{\alpha\in A}$ là một điểm của $\mathscr{C}(U; F)^A$ thuộc bao đóng của ảnh của $u$. Tồn tại một bộ lọc $\mathfrak{F}$ trên $\mathscr{C}^r(U; F)$ sao cho ta có $g_{\alpha}=$ lim$_{f,\mathscr{F}}\partial^{\alpha}f$ trong $\mathscr{C}(U; F)$ với mọi $\alpha \in A$. Cho $m$ là một số nguyên sao cho $0\leqslant m\leqslant r$. Lập luận quy nạp theo $m$, suy ra từ Định lý 1 của FVR, II, p. 2, rằng ánh xạ $g_0$ thuộc lớp $C^m$ và ta có $g_{\alpha}=\partial^{\alpha}g_0$ với mọi $\alpha \in \mathbf{N}^n$ sao cho $|\alpha |\leqslant m$. Do đó $g_0$ thuộc không gian $\mathscr{C}^r(U; F)$ và ảnh của nó dưới $u$ là $(g_{\alpha})_{\alpha\in A}$. Điều này chứng minh rằng ảnh của $u$ là đóng, và do đó thiết lập mệnh đề a).

Mệnh đề a) kéo theo rằng không gian $\mathscr{C}^r(U; F)$ đẳng cấu với ảnh của nó trong $\mathscr{C}(U; F)^A$; vì ảnh này là đóng và không gian $\mathscr{C}(U; F)^A$ là đầy đủ (TG, X, p. 9, Hệ quả 3 của Định lý 2 và TG, II, p. 17, Mệnh đề 10), nên không gian $\mathscr{C}^r(U; F)$ là đầy đủ.

#### Mệnh đề 8 {#ts-iii-s2-prop-8 .statement tag=02R2}

Giả sử rằng F là hữu hạn chiều. Cho $s$ là một số nguyên sao cho $0\leqslant s < r$ và V là một tập con mở tương đối compắc của U. Ánh xạ tuyến tính $f\mapsto f|V$ từ $\mathscr{C}^r(U; F)$ vào $\mathscr{C}^s(V; F)$ là compact.

Gọi W là tập hợp các hàm $f\in \mathscr{C}^r(U; F)$ mà các đạo hàm riêng cấp $\leqslant r$ nhận tại mọi điểm của V một giá trị có chuẩn nhỏ hơn 1. Tập W là một lân cận của 0 trong không gian $\mathscr{C}^r(U; F)$. Cho $\alpha$ là một đa chỉ số sao cho $|\alpha |\leqslant s$. Xét tập H gồm các hàm có dạng $(\partial^{\alpha}f)|V$ với $f$ thuộc W. Tập H là một tập con đồng liên tục của $\mathscr{C}(V; F)$ (TG, X, p. 10) theo định lý giá trị trung bình (VAR, R, 2.2.3). Hơn nữa, với mọi $x\in V$, ảnh của H dưới ánh xạ $g\mapsto g(x)$ là một tập con bị chặn, do đó là một tập con tương đối compắc, của F. Theo định lý Ascoli (TG, X, p. 18, Hệ quả 2), tập H là tương đối compắc trong $\mathscr{C}(V; F)$. Điều này chứng minh rằng ánh xạ tuyến tính $f\mapsto (\partial^{\alpha}f)|V$ từ $\mathscr{C}^r(U; F)$ vào $\mathscr{C}(V; F)$ là compact. Khi đó mệnh đề suy ra từ Bổ đề 3 và các Nhận xét 5 và 6 của III, p. 3.

### 6. Hạn chế của các tiết diện khả vi của một bó vectơ

Cho $r$ là một số nguyên dương, X là một đa tạp khả vi thuộc lớp $C^r$ địa phương hữu hạn chiều và E là một bó vectơ (thực hoặc phức) với cơ sở là X và thuộc lớp $C^r$. Với mọi tập con mở U của X, ký hiệu bởi $\mathscr{S}^r(U; E)$ không gian vectơ (được ký hiệu bởi $\mathscr{S}_E^r(U)$ trong VAR, R1, 7.4, p. 74) các tiết diện thuộc lớp $C^r$ của E trên U, được trang bị tôpô của sự hội tụ $C^r$ compắc.

#### Bổ đề 4 {#ts-iii-s2-lem-4 .statement tag=02R3}

Cho $\mathscr{U}$ là một phủ mở của X. Ánh xạ $u:f\mapsto (f|U)_{U\in\mathscr{U}}$ từ $\mathscr{S}^r(X; E)$ vào $\prod_{U\in\mathscr{U}}\mathscr{S}^r(U; E)$ là tuyến tính, đơn ánh, liên tục và ngặt. Ảnh của nó là đóng.

Ánh xạ $u$ là tuyến tính, đơn ánh và liên tục. Theo TG, IX, p. 43, prop. 1 và p. 48, cor. 1, mọi tập con compact của X đều có một phủ hữu hạn $(C_i)_{i\in I}$ trong đó, với mỗi $i\in I$, tập hợp $C_i$ là một tập con compact của một trong các tập hợp mở của phủ $\mathscr{U}$. Suy ra ánh xạ tuyến tính $u$ là ngặt. Cuối cùng, ảnh của nó là đóng, vì nó gồm các họ $(f_U)_{U\in\mathscr{U}}$ sao cho $f_U$ và $f_V$ trùng nhau trên $U\cap V$ với mọi U và V trong $\mathscr{U}$.

#### Mệnh đề 9 {#ts-iii-s2-prop-9 .statement tag=02R4}

Không gian $\mathscr{S}^r(X; E)$ là đầy đủ.

Trước hết giả sử rằng tồn tại một số nguyên $n\geqslant 0$ và một không gian Banach F sao cho X là một tập hợp mở của $\mathbf{R}^n$ và E là bó vectơ tầm thường $X\times F$ với cơ sở X và thớ F. Trong trường hợp này, không gian vectơ tôpô $\mathscr{S}^r(X; E)$ đẳng cấu với $\mathscr{C}^r(X; F)$, và kết quả suy ra từ bổ đề 3 của III, p. 34.

Trong trường hợp tổng quát, lấy $\mathscr{U}$ là một phủ mở của X bởi các miền bản đồ sao cho với mọi $U\in \mathscr{U}$, hạn chế của E lên U là khả tầm thường hóa. Theo bổ đề trên, không gian $\mathscr{S}^r(X; E)$ đẳng cấu với ảnh của ánh xạ tuyến tính $f\mapsto (f|U)_{U\in\mathscr{U}}$, ảnh này là đóng trong tích của các không gian $\mathscr{S}^r(U; E)$ với U thuộc $\mathscr{U}$. Theo trường hợp trước, mỗi không gian $\mathscr{S}^r(U; E)$ đều đầy đủ, nên tích của chúng là đầy đủ (TG, II, p. 17, prop. 10). Do đó $\mathscr{S}^r(X; E)$ là đầy đủ.

#### Nhận xét {#ts-iii-s2-n6-rem-1 .statement tag=02R5}

Lấy $\mathscr{U}$ là một phủ mở của X bởi các miền bản đồ $c_U= (U, \varphi_U,\mathbf{R}^{n_U})$ sao cho với mọi $U\in \mathscr{U}$, hạn chế của E lên U là khả tầm thường hóa kiểu $F_U$, trong đó $F_U$ là một không gian Banach. Với mọi $U\in \mathscr{U}$, một tiết diện $f$ của E trên U được đồng nhất với một ánh xạ $f_U$ từ $\varphi_U(U)$ vào $F_U$. Từ chứng minh của prop. 9 suy ra rằng tôpô của không gian $\mathscr{S}^r(X; E)$ được xác định bởi họ các nửa chuẩn $p_{U,C,\alpha}$ sao cho

$p_{U,C,\alpha}(f) =$ sup$_{x\in C}\|(\partial^{\alpha}f_U)(x)\|$, trong đó U chạy qua $\mathscr{U}, C$ chạy qua tập hợp các tập con compact của $\varphi_U(U)$ và $\alpha \in \mathbf{N}^{n_U}$ chạy qua tập hợp các đa chỉ số sao cho $|\alpha |\leqslant r$.

#### Mệnh đề 10 {#ts-iii-s2-prop-10 .statement tag=02R6}

Giả sử rằng bó vectơ E địa phương có hạng hữu hạn. Cho $s$ là một số nguyên sao cho $0\leqslant s < r$ và Y là một tập hợp mở compact tương đối của X. Ánh xạ tuyến tính $f\mapsto f|Y$ từ $\mathscr{S}^r(X; E)$ vào $\mathscr{S}^s(Y; E)$ là compact.

Trước hết giả sử rằng tồn tại một số nguyên $n\geqslant 0$ và một không gian Banach hữu hạn chiều F sao cho X là một tập hợp mở của $\mathbf{R}^n$ và E là bó vectơ tầm thường $X\times F$ với cơ sở X và thớ F. Trong trường hợp này, các không gian vectơ tôpô $\mathscr{S}^r(X; E)$ và $\mathscr{S}^s(Y; E)$ lần lượt đẳng cấu với $\mathscr{C}^r(X; F)$ và $\mathscr{C}^s(Y; F)$, và prop. 10 là một hệ quả của prop. 8.

Ta hãy chuyển sang trường hợp tổng quát. Cho C là một tập con compắc của X chứa Y. Với mọi điểm $x$ của C, chọn một lân cận mở $U(x)$ của $x$ trong X là một miền tọa độ mà trên đó bó vectơ E là tầm thường hóa được. Hơn nữa, chọn một lân cận mở tương đối compắc $V(x)$ của $x$ trong $U(x)$. Vì tập hợp C là compắc, nó được phủ bởi một họ hữu hạn $(V(x_1), . . . ,V(x_m))$ các tập mở như vậy. Với mọi $i$, đặt $U_i= U(x_i)$ và $Y_i= V(x_i)\cap Y$. Khi đó $Y_i$ là một tập con mở tương đối compắc của $U_i$ và ta có $Y = Y_1\cup  \cdots  \cup Y_m$. Các ánh xạ tuyến tính $f\mapsto f|U_i$ từ $\mathscr{S}^r(X; E)$ vào $\mathscr{S}^r(U_i; E)$ là liên tục và các ánh xạ tuyến tính $g\mapsto g|Y_i$ từ $\mathscr{S}^r(U_i; E)$ vào $\mathscr{S}^s(Y_i; E)$ là compắc theo phần thứ nhất của chứng minh. Do đó các ánh xạ tuyến tính $f\mapsto f|Y_i$ từ $\mathscr{S}^r(X; E)$ vào $\mathscr{S}^s(Y_i; E)$ là compắc (mệnh đề 3 của III, p. 5). Có tính đến bổ đề 4, áp dụng cho phủ của Y bởi các tập mở $Y_i$, và các nhận xét 5 và 6 của III, p. 3, ánh xạ tuyến tính $f\mapsto f|Y$ từ $\mathscr{S}^r(X; E)$ vào $\mathscr{S}^s(Y; E)$ là compắc, điều này hoàn tất chứng minh.

### 7. Hạn chế của các tiết diện giải tích của một bó vectơ

Cho X là một đa tạp giải tích phức địa phương có số chiều hữu hạn và E là một bó vectơ giải tích với cơ sở X (VAR, p. 35 và VAR, p. 70). Ký hiệu bởi $\mathscr{S}^{\omega}(X; E)$ không gian vectơ các tiết diện giải tích của E trên X, được trang bị tôpô của sự hội tụ compắc.

#### Bổ đề 5 {#ts-iii-s2-lem-5 .statement tag=02R7}

Cho $X_0$ là đa tạp giải tích thực nền của X và $E_0$ là bó vectơ phức trên $X_0$ nền của E.

a) Không gian con vectơ $\mathscr{S}^{\omega}(X; E)$ của $\mathscr{S}^0(X_0; E_0)$ là đóng, và đơn ánh của $\mathscr{S}^{\omega}(X; E)$ vào $\mathscr{S}^0(X_0; E_0)$ là liên tục và ngặt ;

b) Đơn ánh chính tắc của $\mathscr{S}^{\omega}(X; E)$ vào $\mathscr{S}^1(X_0; E_0)$ là liên tục.

Trước hết giả sử rằng tồn tại một số nguyên $n\geqslant 0$ và một không gian Banach F sao cho X là một tập con mở của $\mathbf{C}^n$ và E là bó vectơ tầm thường $X\times F$. Trong trường hợp này, các không gian vectơ tôpô $\mathscr{S}^{\omega}(X; E)$, $\mathscr{S}^0(X_0; E_0)$ và $\mathscr{S}^1(X_0; E_0)$ lần lượt đẳng cấu với $\mathscr{C}^{\omega}(X; F),\mathscr{C}^0(X_0; F)$ và $\mathscr{C}^1(X_0; F)$, và không gian vectơ $\mathscr{S}^0(X_0; E_0)$ là mêtric hóa được (TG, X, p. 20, hệ quả của mệnh đề 1). Khi đó bổ đề suy ra từ VAR, 3.3.2, p. 28.

Ta hãy chuyển sang trường hợp tổng quát. Cho $\mathfrak{F}$ là một bộ lọc trên $\mathscr{S}^{\omega}(X; E)$ hội tụ trong không gian $\mathscr{S}^0(X_0; E_0)$ tới một giới hạn $f$. Vấn đề là chứng minh rằng $f$ thuộc $\mathscr{S}^{\omega}(X; E)$ và rằng bộ lọc $\mathfrak{F}$ hội tụ tới $f$ trong không gian $\mathscr{S}^1(X_0; E_0)$. Mệnh đề này có tính chất địa phương, và do đó suy ra từ phần thứ nhất của chứng minh.

#### Mệnh đề 11 {#ts-iii-s2-prop-11 .statement tag=02R8}

Giả sử rằng bó vectơ E địa phương có hạng hữu hạn. Cho Y là một tập con mở tương đối compắc của X. Ánh xạ hạn chế $f\mapsto f|Y$ từ $\mathscr{S}^{\omega}(X; E)$ vào $\mathscr{S}^{\omega}(Y; E)$ là compắc.

Với các ký hiệu của bổ đề 5, ta có một biểu đồ giao hoán

$$
\mathscr{S}^{\omega}(X; E)\leftarrow_i\rightarrow \mathscr{S}^1(X_0; E_0)
$$

$$
\rightarrow \leftarrow_u\rightarrow \leftarrow_v \tag{3}
$$

$$
\mathscr{S}^{\omega}(Y; E)\leftarrow_j\rightarrow \mathscr{S}^0(Y_0; E_0)
$$

trong đó $i$ và $j$ là các đơn ánh chính tắc và $u,v$ là các ánh xạ hạn chế. Ánh xạ $i$ là liên tục (Bổ đề 5, b)), và ánh xạ $u$ là compắc (Mệnh đề 10). Vì đơn ánh chính tắc $j$ là liên tục, ngặt, và có ảnh đóng (Bổ đề 5, a)), ánh xạ $u$ là compắc (Nhận xét 5 của III, p. 3).

#### Hệ quả {#ts-iii-s2-n7-cor-1 .statement tag=02R9}

Cho X là một đa tạp giải tích phức compắc và E là một bó vectơ giải tích trên X, địa phương có hạng hữu hạn. Không gian vectơ $\mathscr{S}^{\omega}(X; E)$ là hữu hạn chiều.

Vì nó compắc, đa tạp giải tích X là hữu hạn chiều địa phương. Theo Mệnh đề 11, ánh xạ đồng nhất của $\mathscr{S}^{\omega}(X; E)$ là một ánh xạ tuyến tính compắc. Điều này kéo theo không gian $\mathscr{S}^{\omega}(X; E)$ là hữu hạn chiều (Nhận xét 3 của III, p. 2).

## BÀI TẬP {#ts-iii-s2-exercises}

Xem [các bài tập cho § 2](exercises/s2/).
