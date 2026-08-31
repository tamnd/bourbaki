---
book: ts
book_title: Théories spectrales
chapter: IV
chapter_title: THÉORIE SPECTRALE HILBERTIENNE
section: 1
section_title: Opérateurs compacts sur un espace hilbertien
lang: vi
source: ts-iii-v-fr
book_pages: TS IV.146-TS IV.179, TS IV.313-TS IV.319
pdf_pages: 0159-0192, 0326-0332
extraction: native
subsections:
    - "no": 1
      title: Endomorphismes diagonaux
      page: 146
      pdf_page: 159
    - "no": 2
      title: Diagonalisation des endomorphismes compacts
      page: 149
      pdf_page: 162
    - "no": 3
      title: Suite décroissante des valeurs propres
      page: 151
      pdf_page: 164
    - "no": 4
      title: Caractérisations variationnelles des valeurs propres
      page: 153
      pdf_page: 166
    - "no": 5
      title: Applications de la caractérisation variationnelle des valeurs propres
      page: 155
      pdf_page: 168
    - "no": 6
      title: Inégalités de Weyl
      page: 157
      pdf_page: 170
    - "no": 7
      title: Endomorphismes de trace finie
      page: 164
      pdf_page: 177
    - "no": 8
      title: Applications nucléaires
      page: 167
      pdf_page: 180
    - "no": 9
      title: Opérateurs intégraux de Hilbert–Schmidt
      page: 172
      pdf_page: 185
    - "no": 10
      title: Trace des opérateurs intégraux à noyau continu
      page: 174
      pdf_page: 187
statements: 66
exercises: 22
content_sha256: 505d3c28f058b1ba9435ac6e7d510b596f0d663b3fa668163c6cc7228496ac78
translated_from: content/en-mt/ts/IV/01_s1_operateurs_compacts_sur_un_espace.md
source_lang: en-mt
translation_method: machine
source_content_sha256: cff347a68f44a4f3da567c33474a6b11ca1254d89cd96fd15d27da328da51b68
translation_model: gpt-5.4
translation_run: translate-vi-10328def
glossary_version: 34
glossary_terms_sha256: 69448f71f264cabc7d1e6fc36482151a630033e624dafc57043b816976d83034
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 1. TOÁN TỬ COMPACT TRÊN MỘT KHÔNG GIAN HILBERT

Trong đoạn này, K là một trường bằng $\mathbf{R}$ hoặc $\mathbf{C}$ và E ký hiệu một không gian Hilbert trên trường K.

### 1. Các tự đồng cấu đường chéo

#### Định nghĩa 1 {#ts-iv-s1-def-1 .statement tag=02W8}

Cho $B = (e_i)_{i\in I}$ là một cơ sở trực chuẩn của E. Một tự đồng cấu $u$ được gọi là đường chéo trong cơ sở B hoặc đường chéo đối với B nếu tồn tại một họ $\lambda = (\lambda_i)_{i\in I}$ các phần tử của K sao cho $u(e_i) =\lambda_ie_i$ với mọi $i\in I$.

Cho $B = (e_i)_{i\in I}$ là một cơ sở trực chuẩn của E. Ta ký hiệu bởi $\mathscr{D}_B(E)$ tập hợp các tự đồng cấu của E là đường chéo đối với B. Đó là một đại số con đóng, giao hoán, có đơn vị của $\mathscr{L}(E)$. Cho $u\in \mathscr{D}_B(E)$. Họ $\lambda = (\lambda_i)_{i\in I}$ sao cho $u(e_i) =\lambda_ie_i$ được xác định duy nhất bởi $u$ và bởi cơ sở B, và người ta nói rằng đó là họ các trị riêng của $u$ đối với B.

Giả sử rằng $K =\mathbf{R}$ và đồng nhất E với một không gian con của $E_{(\mathbf{C})}$. Cho $B = (e_i)_{i\in I}$ là một cơ sở trực chuẩn của E. Ký hiệu bởi $B_{(\mathbf{C})}$ cơ sở trực chuẩn $(1\otimes e_i)_{i\in I}$ của $E_{(\mathbf{C})}($xem EVT, V, p. 29, hệ quả 1). Ánh xạ $u\mapsto u_{(\mathbf{C})}$ cảm sinh một cấu xạ đại số đơn ánh từ $\mathscr{D}_B(E)$ vào $\mathscr{D}_{B_{(\mathbf{C})}}(E_{(\mathbf{C})})$; ảnh của nó là tập hợp các $u\in \mathscr{D}_{B_{(\mathbf{C})}}(E_{(\mathbf{C})})$ sao cho $u(E)\subset E$, nói cách khác là tập hợp các $u$ đường chéo trong cơ sở $B_{(\mathbf{C})}$ mà các trị riêng là thực.

Với mọi $i\in I$, ta ký hiệu bởi $p_i$ phép chiếu trực giao của E có ảnh là $Ke_i$. Ta có $\|p_i\|= 1$ với mọi $i\in I$. Tự đồng cấu $p_i$ là đường chéo trong cơ sở B, họ các trị riêng của nó là họ $(\delta_{ij})_{j\in I}$ (ký hiệu Kronecker, xem A, II, p. 24).

Cho $B'= (f_i)_{i\in I}$ là một cơ sở trực chuẩn của E và $u: E\rightarrow E$ là đẳng cấu đẳng cự sao cho $u(f_i) =e_i$. Khi đó $\mathscr{D}_{B'}(E) =u^{-1}\mathscr{D}_B(E)u$.

Ta trang bị cho I tôpô rời rạc và ký hiệu bởi $\mathscr{B}(I) =\mathscr{C}_b(I; K)$ đại số Banach có đơn vị của các hàm bị chặn trên I với giá trị trong K (ví dụ 2 của I, p. 17) ; nếu $K =\mathbf{C}$, đó là một đại số sao (ví dụ 2 của I, p. 102).

#### Bổ đề 1 {#ts-iv-s1-lem-1 .statement tag=02W9}

Cho $u\in \mathscr{D}_B(E)$ và $\lambda = (\lambda_i)_{i\in I}$ là họ các trị riêng của nó. Họ $\lambda$ bị chặn và ta có sup$_i|\lambda_i|=\|u\|$.

Ta có $|\lambda_i|\leqslant \|u\|$ với mọi $i$, do đó sup$_{i\in I}|\lambda_i|\leqslant \|u\|$. Hơn nữa, vì

$\|u(x)\|^2=\sum_{i\in I}|\lambda_i|^2|\langle e_i|x\rangle |^2\leqslant ($sup$_{i\in I}|\lambda_i|^2)\|x\|^2$

với mọi $x\in E$ (EVT, V, p. 22, mệnh đề 5), suy ra $\|u\|=$ sup$|\lambda_i|$.

#### Mệnh đề 1 {#ts-iv-s1-prop-1 .statement tag=02WA}

a) Ánh xạ $\alpha$ từ $\mathscr{D}_B(E)$ vào $\mathscr{B}(I)$ gán cho một tự đồng cấu đường chéo $u$ họ các trị riêng của $u$ là một đẳng cấu đẳng cự của các đại số Banach trên K. Nếu $K =\mathbf{C}$, đó là một cấu xạ của các đại số có phép đối hợp ;

b) Với mọi họ bị chặn $\lambda = (\lambda_i)_{i\in I}$, họ $(\lambda_ip_i)_{i\in I}$ là khả tổng trong không gian $\mathscr{L}(E)$ được trang bị tôpô hội tụ đơn giản, và tổng của họ này là ánh xạ duy nhất $u\in \mathscr{D}_B(E)$ sao cho $\alpha (u) =\lambda$;

c) Cho $u\in \mathscr{D}_B(E)$ và gọi $\lambda$ là họ các giá trị riêng của nó đối với B. Phổ của $u$ là bao đóng trong K của tập hợp các giá trị của $\lambda$;

d) Nếu K = $\mathbf{C}$, thì ánh xạ của phép tính phiếm hàm liên tục từ $\mathscr{C}$ (Sp($u$)) vào $\mathscr{L}(E)$ gắn với một hàm liên tục $f\in \mathscr{C}$ (Sp($u$)) tự đồng cấu $\alpha (f\circ \lambda )$ trong $\mathscr{D}_B(E)$.

Theo Bổ đề 1, họ các giá trị riêng của một tự đồng cấu chéo theo B là bị chặn và do đó ánh xạ từ $\mathscr{D}_B(E)$ vào $\mathscr{B}(I)$ được xác định như vậy là một cấu xạ đẳng cự liên tục của các đại số Banach có đơn vị.

Cho $i\in I$. Với mọi $j\in I$, ta có $\langle u^*(e_i)|e_j\rangle =\lambda_j\langle e_i|e_j\rangle =\langle \overline{\lambda_j}e_i|e_j\rangle$. Suy ra $u^*(e_i) =\overline{\lambda}_ie_i$. Do đó liên hợp của $u$ là tự đồng cấu chéo theo cơ sở B mà họ các giá trị riêng là $(\lambda_i)_{i\in I}$. Khẳng định a) được suy ra.

Cho $\lambda = (\lambda_i)_{i\in I}\in \mathscr{B}(I)$. Với mọi $x\in E$, họ $(|\langle e_i|x\rangle |^2)_{i\in I}$ là khả tổng, với tổng bằng $\|x\|^2$ (EVT, V, p. 22, mệnh đề 5), do đó, với mọi tập con hữu hạn J của I:

$\|\sum_{i\in J}\lambda_ip_i(x)\|^2=\sum_{i\in J}|\lambda_i|^2|\langle e_i|x\rangle |^2\leqslant ($sup$_{i\in I}|\lambda_i|^2)(\sum_{j\in J}|\langle e_i|x\rangle |^2$

$\leqslant ($sup$_{i\in I}|\lambda_i|)^2\|x\|^2$.

Do đó, họ $(\lambda_ip_i)$ là khả tổng trong $\mathscr{L}(E)$ được trang bị tôpô hội tụ đơn giản. Tổng của nó $u_{\lambda}$ thỏa mãn $u_{\lambda}(e_i) =\lambda_ie_i$; vì vậy nó là một tự đồng cấu chéo theo cơ sở B, với các giá trị riêng là $\lambda$. Khẳng định b) được suy ra.

Các khẳng định cuối cùng suy ra từ a), từ Ví dụ 3 của I, p. 17 và từ Ví dụ 4 của I, p. 111.

#### Nhận xét {#ts-iv-s1-n1-rem-1 .statement tag=02WB}

Đại số Banach $\mathscr{D}_B(E)$ là một đại số con đóng giao hoán cực đại của $\mathscr{L}(E)$. Thật vậy, cho $u$ là một tự đồng cấu của E giao hoán với $\mathscr{D}_B(E)$. Cho $i\in I$. Vì phép chiếu trực giao $p_i$ là chéo theo cơ sở B, ta có $p_i(u(e_i)) =u(p_i(e_i)) =u(e_i)$, điều đó suy ra rằng $u(e_i)$ tỉ lệ với $e_i$. Vậy $u$ là chéo theo cơ sở B.

Nếu E có chiều vô hạn, tồn tại các đại số con có phép đối involutive giao hoán cực đại của $\mathscr{L}(E)$ không đẳng cấu với $\mathscr{D}_B(E)$ (bài tập 5 của IV, p. 314).

#### Mệnh đề 2 {#ts-iv-s1-prop-2 .statement tag=02WC}

Cho $u\in \mathscr{D}_B(E)$ và $\lambda = (\lambda_i)_{i\in I}$ là họ các giá trị riêng của nó.

a) Các điều kiện sau là tương đương:

(i) Ta có $\lambda \in \mathscr{C}_0(I; K)$;

(ii) Tự đồng cấu $u$ là compact ;

(iii) Họ $(\lambda_ip_i)_{i\in I}$ là khả tổng trong không gian Banach

$\mathscr{L}(E)$. Khi đó tổng của nó bằng $u$.

b) Giả sử rằng $u$ là compact và ký hiệu bởi Λ tập hợp các giá trị của $\lambda$. Tập hợp các $i\in I$ sao cho $\lambda_i\not = 0$ là đếm được. Nếu E có chiều vô hạn, ta có Sp$_s(u) = \Lambda -\{0\}$ và Sp($u$) $= \Lambda \cup  \{0\}$. Nếu E có số chiều hữu hạn, thì Sp$_s(u) =$ Sp($u$) $= \Lambda$.

Theo Bổ đề 1, ta có $\|\sum_{j\in J}\lambda_jp_j\|=$ sup$_{j\in J}|\lambda_j|$ với mọi tập con hữu hạn J của I. Từ đó suy ra, theo tiêu chuẩn Cauchy, rằng họ $(\lambda_ip_i)$ là khả tổng trong $\mathscr{L}(E)$ khi và chỉ khi họ $\lambda$ tiến tới 0 ở vô cực, điều này kéo theo rằng các điều kiện (i) và (iii) là tương đương.

Điều kiện (iii) kéo theo rằng $u$ là compact (hệ quả của Mệnh đề 2 của III, p. 4). Ngược lại, giả sử rằng tự đồng cấu $u$ là compact. Vì họ B bị chặn trong E, ảnh của nó bởi $u$ trong E là tương đối compact trong E (III, p. 2), và do đó tiền compact. Cho $\varepsilon  >0$ và J là một tập con hữu hạn của I sao cho ảnh của B bởi $u$ được chứa trong hợp của các quả cầu bán kính $\varepsilon$ và tâm $u(e_j)$ với $j\in J$. Cho $i\in I$ - J. Tồn tại $j\in J$ sao cho $\|u(e_i)-u(e_j)\|\leqslant \varepsilon$, do đó

$$
|\lambda_i|^2\leqslant |\lambda_i|^2+|\lambda_j|^2=\|u(e_i)-u(e_j)\|^2\leqslant \varepsilon^2
$$

Do đó, ta có $\lambda \in \mathscr{C}_0(I; K)$$, nghĩa là, điều kiện (i).

Sau cùng, phổ của $u$ và phổ nhạy của nó được tính như những hàm của $\lambda$ bằng cách dùng mệnh đề 1, c) và Mệnh đề 5 của III, p. 90.

#### Nhận xét {#ts-iv-s1-n1-rem-2 .statement tag=02WD}

Khi I là vô hạn, điều kiện $\lambda \in \mathscr{C}_0(I; K)$ cũng có thể được phát biểu như sau: “họ $\lambda$ tiến tới 0 theo bộ lọc các phần bù của các tập con hữu hạn của I.”

### 2. Chéo hóa các tự đồng cấu compact

#### Định lý 1 {#ts-iv-s1-thm-1 .statement tag=02WE}

Giả sử $K =\mathbf{C}$. Cho $u$ là một tự đồng cấu compact và chuẩn tắc của E. Tồn tại một cơ sở trực chuẩn B của E sao cho $u$ là đường chéo trong cơ sở B.

Tập hợp Sp$_s(u)$ là đếm được, và nó không chứa 0 nếu E có chiều vô hạn (III, p. 90, prop. 5, b)). Với mọi phần tử $\lambda \in$ Sp$_s(u)$, ký hiệu bởi $N_{\lambda}$ không gian-không của $u-\lambda 1_E$. Nó có số chiều hữu hạn (loc. cit.) và, vì $u$ là chuẩn tắc, nó trùng với không gian riêng của $u$ ứng với $\lambda$ (EVT, V, p. 43, hệ quả của mệnh đề 8). Các không gian $N_{\lambda}$ trực giao từng đôi một (I, p. 132, n$^o5$).

Cho F là không gian con của E là tổng Hilbert của các không gian $N_{\lambda}$ với $\lambda \in$ Sp$_s(u)-\{0\}$. Đó là một không gian kiểu đếm được, ổn định dưới $u$ vì mỗi không gian con $N_{\lambda}$ đều ổn định dưới $u$. Vì $N_{\lambda}$ cũng là không gian riêng của $u^*$ tương ứng với $\overline{\lambda}$ (EVT, V, loc. cit.), tự đồng cấu $u$ cảm sinh một tự đồng cấu $\widetilde{u}$ của $F^{\circ}$ bằng cách chuyển qua các không gian con. Tự đồng cấu $\widetilde{u}$ là compact (Mệnh đề 3 của III, p. 5) và chuẩn tắc (Bổ đề 4 của I, p. 135). Theo phép dựng, phổ điểm của $\widetilde{u}$ được chứa trong $\{0\}$ (thật vậy, mọi vectơ riêng của $\widetilde{u}$ cũng sẽ là vectơ riêng của $u$, do đó sẽ thuộc một trong các không gian $N_{\lambda}$ nếu trị riêng tương ứng khác không). Vì vậy bán kính phổ của $\widetilde{u}$ bằng không, do đó $\widetilde{u}= 0$ vì $\widetilde{u}$ là chuẩn tắc (Hệ quả 1 của I, p. 108). Suy ra $F^{\circ}\subset$ Ker($u$).

Với mọi $\lambda \in$ Sp$_s(u)$, gọi $B_{\lambda}$ là một cơ sở trực chuẩn của $N_{\lambda}$ và gọi $(e_j)_{j\in J}$ là họ hợp của các $B_{\lambda}$; đó là một cơ sở trực chuẩn của F. Gọi B là hợp của $(e_j)_{j\in J}$ với một cơ sở trực chuẩn của $F^{\circ}$. Đó là một cơ sở trực chuẩn của E và $u$ là đường chéo trong cơ sở B.

#### Hệ quả 1 {#ts-iv-s1-thm-1-cor-1 .statement tag=02WF}

Cho $u$ là một tự đồng cấu Hermit compact của E. Tồn tại một cơ sở trực chuẩn B của E sao cho $u$ là đường chéo trong cơ sở B và các trị riêng của nó là thực.

Nếu $K =\mathbf{C}$, điều này suy ra ngay từ định lý. Giả sử $K =\mathbf{R}$. Không gian E là một $\mathbf{R}$-cấu trúc trên $E_{(\mathbf{C})}($x. A, II, p. 119). Tự đồng cấu $u_{(\mathbf{C})}$ của $E_{(\mathbf{C})}$ là compact (Nhận xét 4 của III, p. 2) và Hermit. Gọi $B = (e_j)_{j\in J}$ là một cơ sở trực chuẩn của $E_{(\mathbf{C})}$ sao cho $u_{(\mathbf{C})}\in \mathscr{D}_B(E_{(\mathbf{C})})$ và $\lambda$ là họ các trị riêng của $u_{(\mathbf{C})}$ (Định lý 1). Ta có $\lambda \in \mathbf{R}^J($I, p. 106, Mệnh đề 4) ; vì ánh xạ tuyến tính $u_{(\mathbf{C})}$ là $\mathbf{R}$-hữu tỉ, không gian riêng của $u_{(\mathbf{C})}$ tương ứng với $\lambda_j$ là $\mathbf{R}$-hữu tỉ với mọi $j\in J ($x. A, V, p. 60, Mệnh đề 6). Do đó tồn tại một cơ sở của nó thuộc E, và a fortiori, tồn tại một cơ sở trực chuẩn của nó trong E. Hợp của các cơ sở này là một cơ sở trực chuẩn $B_{\mathbf{R}}$ của E sao cho $u\in \mathscr{D}_{B_{\mathbf{R}}}(E)$.

#### Hệ quả 2 {#ts-iv-s1-thm-1-cor-2 .statement tag=02WG}

Cho F là một không gian Hilbert và cho $u$ là một ánh xạ tuyến tính liên tục compact từ E vào F. Tồn tại một tập đếm được I, một cơ sở trực chuẩn $(e_i)_{i\in I}$ của không gian ban đầu Ker($u$)$^{\circ}$ của $u$, một họ trực chuẩn $(f_i)_{i\in I}$ của F và một họ $(\alpha_i)_{i\in I}\in (\mathbf{R}^*_+)^I$ sao cho $u(e_i) =\alpha_if_i$ với mọi $i\in I$.

Đặt $v=u^*\circ u$. Đó là một tự đồng cấu compact (III, p. 5, Prop. 3) và dương, do đó Hermit, của E. Theo Hệ quả 1, tồn tại một cơ sở trực chuẩn $(e_j)_{j\in J}$ của E sao cho $v$ là chéo trong cơ sở này. Họ $(\lambda_j)_{j\in J}$ các trị riêng của nó được chứa trong $\mathbf{R}_+^J$. Đặt $\alpha_j=\surd\overline{\lambda_j}$ với mọi $j\in J$. Gọi I là tập các $j\in J$ sao cho $\alpha_j\not = 0$. Đó là một tập đếm được vì $v$ là compact. Họ $(e_i)_{i\in I}$ là một cơ sở trực chuẩn của không gian ban đầu của $v$, tức là không gian ban đầu Ker($u$)$^{\circ}$ của $u$ (EVT, V, p. 43, Prop. 8). Đặt $f_i=\frac{1}{\alpha_i}u(e_i)$ với $i\in I$. Với mọi $i$ và $j$ thuộc I, ta có

$$
\langle f_i|f_j\rangle =\frac{1}{\alpha_i\alpha_j}\langle u(e_i)|u(e_j)\rangle =\frac{1}{\alpha_i\alpha_j}\langle v(e_i)|e_j\rangle =\frac{\lambda_i}{\alpha_i\alpha_j}\langle e_i|e_j\rangle
$$

do đó suy ra rằng họ $(f_i)_{i\in I}$ là trực chuẩn trong F. Hệ quả được suy ra, vì $u(e_i) =\alpha_if_i$ với mọi $i\in I$.

#### Định nghĩa 2 {#ts-iv-s1-def-2 .statement tag=02WH}

Với các ký hiệu của hệ quả, họ $(\alpha_i)_{i\in I}$ là họ các giá trị kỳ dị của $u$, đối với cơ sở trực chuẩn $(e_i)_{i\in I}$ của không gian ban đầu của $u$.

#### Nhận xét 1 {#ts-iv-s1-n2-rem-1 .statement tag=02WI}

Hệ quả này tổng quát hóa Định lý 2 của EVT, V, p. 54, tương ứng với các ánh xạ Hilbert–Schmidt.

#### Nhận xét 2 {#ts-iv-s1-n2-rem-2 .statement tag=02WJ}

Với các ký hiệu của hệ quả, ta có công thức

$$
u(x) =\sum_{i\in I}\alpha_i\langle e_i|x\rangle f_i \tag{1}
$$

với mọi $x\in E$.

#### Nhận xét 3 {#ts-iv-s1-n2-rem-3 .statement tag=02WK}

Cho $u$ là một tự đồng cấu compact dương của E. Gọi $B = (f_i)_{i\in I}$ là một cơ sở trực chuẩn của E sao cho $u$ là chéo trong cơ sở B (Định lý 1), và gọi $(\lambda_i)_{i\in I}$ là họ các trị riêng của $u$ trong cơ sở này. Gọi J là tập các $i\in I$ sao cho $\lambda_i>0$; họ $(e_i)_{i\in J}$ là một cơ sở trực chuẩn của không gian Ker($u$)$^{\circ}$. Với mọi $i\in J$, đặt $e_i=f_i$ và $\alpha_i=\lambda_i$. Suy ra rằng $u(e_i) =\alpha_if_i:$ họ $(\alpha_i)_{i\in J}$ là họ các giá trị kỳ dị của $u$ đối với cơ sở $(e_i)_{i\in J}$.

### 3. Dãy giảm của các trị riêng

Trong số này, giả thiết rằng $K =\mathbf{C}$.

Ta ký hiệu $\overline{\mathbf{N}}=\mathbf{N}\cup  \{+\infty \} \subset \overline{\mathbf{R}}$. Trong số này, ta sẽ nói rằng một không gian vectơ E có chiều $+\infty  \in \overline{\mathbf{N}}$ nếu E không có số chiều hữu hạn.

Cho $I_E\subset \mathbf{N}$ là tập hợp các chiều của các không gian con hữu hạn chiều F của E sao cho $F\not = E$. Ta có $I_E=\mathbf{N}$ nếu E có chiều vô hạn, và ngược lại $I_E=\{0, . . .$, dim(E) $-1\}$. Ta sẽ viết $I = I_E$ khi không thể có nhầm lẫn vì điều này.

Cho $u$ là một tự đồng cấu compắc và dương (đặc biệt là Hermit) của E. Phổ điểm của $u$ là tập hợp các giá trị của một dãy giảm nghiêm ngặt $(\nu_k)_{0\leqslant k<Card(Sp_s(u))}$ gồm các số thực dương (x. mệnh đề 5 của III, p. 90). Với mọi số nguyên $k$ sao cho $0\leqslant k <$ Card(Sp$_s(u)$), ta ký hiệu bởi $n_k\geqslant 1$ bội số phổ của $\nu_k$. Cho $M\in \overline{\mathbf{N}}$ là tổng của các bội số phổ $n_k$; đó là chiều của ảnh của $u$. Ta có $M\leqslant$ Card(I).

Với $0\leqslant n <M$, ta định nghĩa $\lambda_n(u) =\nu_k$, trong đó $k\geqslant 0$ là số nguyên duy nhất sao cho

$$
n_0+\cdots +n_{k-1}\leqslant n < n_0+\cdots +n_k
$$

Ta đặt $\lambda_n(u) = 0$ nếu $n\in I$ thỏa mãn $n\geqslant M$. Trường hợp này chỉ có thể xảy ra nếu $I =\mathbf{N}$ và nếu Sp$_s(u)$ là hữu hạn (hay, điều này cũng tương đương, nếu E có chiều vô hạn và $u$ có hạng hữu hạn).

Dãy $(\lambda_n(u))_{n\in I}$ là giảm; với mọi $\lambda \in$ Sp$_s(u)$, số các số nguyên $n$ sao cho $\lambda_n(u) =\lambda$ bằng bội số phổ của trị riêng $\lambda$ của $u$.

Do lạm dụng ngôn ngữ, người ta nói rằng $(\lambda_n(u))_{n\in J}$ là dãy giảm của các trị riêng của $u$ được lặp lại theo bội số của chúng.

#### Mệnh đề 3 {#ts-iv-s1-prop-3 .statement tag=02WL}

Cho $u$ là một tự đồng cấu dương compắc của E. Tồn tại một họ trực chuẩn $(e_n)_{n\in I}$ trong E sao cho, với mọi $x\in E$, ta có

$$
u(x) =\sum_{n\in I}\lambda_n(u)\langle e_n|x\rangle e_n,\langle x|u(x)\rangle =\sum_{n\in I}\lambda_n(u)|\langle e_n|x\rangle |^2
$$

Cho $B = (f_j)_{j\in J}$ là một cơ sở trực chuẩn của E trong đó $u$ là đường chéo (hệ quả 1 của IV, p. 150) và $(\lambda_j)_{j\in J}$ là họ các trị riêng của $u$ trong cơ sở B. Cho $J'$ là tập hợp các $j\in J$ sao cho $\lambda_j$ thuộc phổ điểm của $u$.

Với mỗi $\lambda \in$ Sp$_s(u)$, tồn tại một song ánh giữa các số nguyên $n$ sao cho $0\leqslant n <M$ và $\lambda_n(u) =\lambda$ và các $j\in J'$ sao cho $\lambda_j=\lambda$, vì hai tập hợp này có lực lượng bằng bội số phổ của $\lambda$. Một lựa chọn các song ánh như vậy cho mỗi $\lambda$ xác định một song ánh $\iota$ từ tập hợp các số nguyên sao cho $0\leqslant n <M$ lên tập $J'$. Ta xác định dãy $(e_n)_{0\leqslant n<M}$ trong E bằng cách đặt $e_n=f_{\iota(n)}$ với $0\leqslant n <M$. Đó là một họ trực chuẩn trong E.

Trong trường hợp M $<$ Card(I) $= +\infty$, không gian F sinh bởi $\{e_0, . . . , e_{M-1}\}$ có số chiều hữu hạn và phần bù trực giao $F^{\circ}$ của nó có số chiều vô hạn; ta chọn cho $(e_n)_{n\geqslant M}$ một họ trực chuẩn trong $F^{\circ}$.

Với mọi $x\in E$, ta có

$$
u(x) =\sum_{j\in J'}\lambda_j\langle f_j|x\rangle f_j=\sum_{0\leqslant n<M}\lambda_n(u)\langle e_n|x\rangle e_n
$$

vì $u(f_j) = 0$ khi $j\in J$ - $J'$. Nếu $n\in I$ thỏa mãn $n\geqslant M$, ta có $\lambda_n(u) = 0$, và thu được công thức thứ nhất của mệnh đề. Công thức thứ hai suy ra từ đó.

#### Mệnh đề 4 {#ts-iv-s1-prop-4 .statement tag=02WM}

Cho $u$ là một tự đồng cấu compắc dương của E. Cho $f\in \mathscr{C}(\mathbf{R}_+)$ là một ánh xạ tăng liên tục sao cho $f(0) = 0$.

Tự đồng cấu $f(u)$ là compắc và dương và, với mọi $n\in I_E$, ta có $\lambda_n(f(u)) =f(\lambda_n(u))$.

Tự đồng cấu $f(u)$ là compắc và dương theo mệnh đề 6, b) của III, p. 91 và mệnh đề 15, a) của I, p. 117. Phổ của $f(u)$ là ảnh qua $f$ của phổ của $u$ (hệ quả 2 của I, p. 111). Nếu $\lambda \in$ Sp$_s(f(u))$, bội số phổ của $\lambda$ là tổng các bội số phổ của những $\mu\in$ Sp($u$) sao cho $f(\mu) =\lambda$ (hệ quả 2 của III, p. 84). Vì $f$ tăng, dãy $(f(\lambda_n(u)))_{n\in I_E}$ là giảm. Mệnh đề khi đó suy ra từ định nghĩa của dãy $(\lambda_n(f(u)))_{n\in I_E}$.

### 4. Các đặc trưng biến phân của các giá trị riêng

Trong số này, giả sử rằng $K =\mathbf{C}$.

Cho $u$ là một tự đồng cấu compắc dương của E và $(\lambda_n(u))_{n\in I_E}$ dãy giảm các giá trị riêng của $u$. Ta đặt $I = I_E$.

Với mọi không gian con đóng F của E, ta ký hiệu

$r_F(u) =$ inf $\frac{\langle x|u(x)\rangle}{2},R_F(u) =$ sup $\frac{\langle x|u(x)\rangle}{2}$,

$$
_{x\in F-\{0\}}\|x\|x_{\in F^{\circ-}\{0\}}\|x\|
$$

trong đó cận dưới lớn nhất (tương ứng cận trên nhỏ nhất) được lấy trong $[0,+\infty ]$.

Với mọi $n\in \mathbf{N}$, ký hiệu $\mathscr{F}_n$ là tập hợp các không gian con vectơ $F\subset E$ có chiều $n$. Ta nói rằng một không gian con $F\in \mathscr{F}_n$ là thích nghi với $u$ nếu nó có một cơ sở trực chuẩn $(f_i)_{0\leqslant i\leqslant n-1}$ sao cho $u(f_i) =\lambda_i(u)f_i$ với $0\leqslant i\leqslant n-1$.

#### Mệnh đề 5 {#ts-iv-s1-prop-5 .statement tag=02WN}

Cho $n\in I$.

a) Với mọi không gian con $F\in \mathscr{F}_{n+1}$ thích nghi với $u$, ta có $\lambda_n(u) =r_F(u)$;

b) Với mọi không gian con $F\in \mathscr{F}_n$ thích nghi với $u$, ta có $\lambda_n(u) = R_F(u)$.

Cho $F\in \mathscr{F}_{n+1}$ là một không gian con thích nghi với $u$, và $(f_i)_{0\leqslant i\leqslant n}$ là một cơ sở trực chuẩn của F sao cho $u(f_i) =\lambda_i(u)f_i$ với mọi $i$. Với mọi $x$ trong F, ta có

$$
\langle x|u(x)\rangle =\sum_{0\leqslant i\leqslant n}\lambda_i(u)|\langle f_i|x\rangle |^2\geqslant \lambda_n(u)\sum_{0\leqslant i\leqslant n}|\langle f_i|x\rangle |^2=\lambda_n(u)\|x\|^2
$$

với đẳng thức xảy ra nếu $x=f_n$. Điều này suy ra $r_F(u) =\lambda_n(u)$, do đó mệnh đề a).

Cho $F\in \mathscr{F}_n$ là một không gian con thích nghi với $u$. Không gian con đóng $F^{\circ}$ là khác không (vì $n=$ dim(F) $<$ dim(E)) và ổn định dưới $u$; tự đồng cấu $\widetilde{u}$ của $F^{\circ}$ suy ra từ $u$ bằng cách chuyển qua các không gian con là compact và dương.

Ta có Sp($\widetilde{u}$)$\subset$ Sp($u$). Hơn nữa, ta có Sp($\widetilde{u}$)$\subset [0, \lambda_n(u)]$. Thật vậy, chỉ cần kiểm tra rằng $\lambda \leqslant \lambda_n(u)$ với mọi $\lambda \in$ Sp$_s(\widetilde{u})$. Khi đó số $\lambda$ là một trị riêng của $u$, nên tồn tại $j\in I$ sao cho $\lambda =\lambda_j(u)$. Do đó không gian riêng của $u$ ứng với $\lambda_j(u)$ không được chứa trong F, điều này suy ra $\lambda_j(u)\leqslant \lambda_n(u)$.

Giả sử $\lambda_n(u)>0$. Khi đó không gian riêng của $u$ ứng với $\lambda_n(u)$ không được chứa trong F, và do đó $\lambda_n(u)$ thuộc phổ điểm của $\widetilde{u}$. Suy ra sup(Sp($\widetilde{u}$)) $=\lambda_n(u)$. Nếu $\lambda_n(u) = 0$, ta cũng có cùng kết quả vì khi đó phổ của $\widetilde{u}$ thu về $\{0\}$.

Hơn nữa, theo định nghĩa ta có $R_F(u) = R_{\{0\}}(\widetilde{u})$, và cuối cùng $R_{\{0\}}(\widetilde{u}) =$ sup(Sp($\widetilde{u}$)) theo Mệnh đề 9 của I, p. 139, a). Mệnh đề b) được chứng minh.

#### Mệnh đề 6 {#ts-iv-s1-prop-6 .statement tag=02WO}

Với mọi $n\in I$, ta có

$\lambda_n(u) =$ sup$_{F\in\mathscr{F}_{n+1}}r_F(u) =$ inf$_{F\in\mathscr{F}_n}R_F(u)$.

Cho $(e_n)_{n\in I}$ là một họ trực chuẩn có tính chất của Mệnh đề 3 của IV, p. 152. Với mọi số nguyên sao cho $1\leqslant n <M + 1$, gọi $F_n\in \mathscr{F}_n$ là không gian con chiều $n$ của E sinh bởi $(e_0, . . . , e_{n-1})$; theo phép dựng, không gian $F_n$ là thích nghi với $u$. Theo Mệnh đề 5, do đó ta có

$$
\lambda_n(u) =r_{F_{n+1}}(u) = R_{F_n}(u) \tag{2}
$$

Cho $n\in I$. Cho $F\in \mathscr{F}_{n+1}$. Hạn chế lên F của phép chiếu trực giao lên $F_n$ không đơn ánh, do đó tồn tại $x\not = 0$ trong F trực giao với $F_n$. Vì $x\in F^{\circ}_n$, khi đó ta có (Mệnh đề 3 của IV, p. 152)

$$
\langle x|u(x)\rangle =\sum_{m\in I}\lambda_m(u)|\langle e_m|x\rangle |^2
$$

$m\geqslant n$

$$
\leqslant \lambda_n(u)\sum_{mm\geqslant\in nI}|\langle e_m|x\rangle |^2=\lambda_n(u)\|x\|^2
$$

Điều này chứng minh rằng $r_F(u)\leqslant \lambda_n(u)$, do đó đặc biệt có bất đẳng thức

(3) Fsup$_{\in\mathscr{F}_{n+1}}r_F(u)\leqslant \lambda_n(u)$.

Cho $F\in \mathscr{F}_n$. Hạn chế lên $F_{n+1}$ của phép chiếu trực giao lên F không đơn ánh, do đó tồn tại một vectơ $x\not = 0$ trong $F_{n+1}$ trực giao với F. Vì $x\in F_{n+1}$, ta có (loc. cit.)

$$
\langle x|u(x)\rangle =\sum_{0\leqslant m\leqslant n}\lambda_m(u)|\langle e_m|x\rangle |^2
$$

$$
\geqslant \lambda_n(u)\sum_{0\leqslant m\leqslant n}|\langle e_m|x\rangle |^2=\lambda_n(u)\|x\|^2
$$

và do đó $R_F(u)\geqslant \lambda_n(u)$. Đặc biệt, ta thu được

(4) Finf$_{\in\mathscr{F}_n}R_F(u)\geqslant \lambda_n(u)$.

Xét các công thức (2), (3) và (4), mệnh đề được chứng minh.

### 5. Các ứng dụng của đặc trưng hóa biến phân của các trị riêng

Trong số này, các không gian Hilbert trên $\mathbf{C}$ được xét.

#### Mệnh đề 7 {#ts-iv-s1-prop-7 .statement tag=02WP}

Cho $u$ và $v$ là các tự đồng cấu compact dương của E.

a) Ta có $|\lambda_n(u)-\lambda_n(v)|\leqslant \|u-v\|$ với mọi $n\in I$;

b) Nếu $u\leqslant v$, thì $\lambda_n(u)\leqslant \lambda_n(v)$ với mọi $n\in I$.

Cho $n\in I$ và cho F là một không gian con vectơ chiều $n$ của E. Với mọi $x\in F$, ta có

$$
|\langle x|v(x)\rangle  - \langle x|u(x)\rangle |\leqslant \|u-v\| \|x\|^2
$$

do đó có các bất đẳng thức

$$
R_F(v)- \|u-v\|\leqslant R_F(u)\leqslant R_F(v) +\|u-v\|
$$

Mệnh đề a) suy ra từ đây bởi Mệnh đề 6 của IV, p. 154.

Nếu $u\leqslant v$, ta có $\langle x|u(x)\rangle \leqslant \langle x|v(x)\rangle$ với mọi $x\in E$. Với mọi $n\in I$ và mọi không gian con F chiều $n$, do đó ta có $R_F(u)\leqslant R_F(v)$, do đó $\lambda_n(u)\leqslant \lambda_n(v) ($loc. cit.).

#### Mệnh đề 8 {#ts-iv-s1-prop-8 .statement tag=02WQ}

Cho $u$ là một tự đồng cấu compact dương của E. Cho H là một không gian con đóng của E và $i_H: H\rightarrow E$ là đơn ánh chính tắc. Ký hiệu $u_H$ là tự đồng cấu $i^*_Hui_H$ của H. Nó compact và dương.

a) Ta có $I_H\subset I_E$ và $\lambda_n(u_H)\leqslant \lambda_n(u)$ với mọi $n\in I_H$;

b) Nếu H có đối chiều hữu hạn $k\in \mathbf{N}$ trong E, thì ta có $I_H+k\subset I_E$ và $\lambda_{n+k}(u)\leqslant \lambda_n(u_H)$ với mọi $n\in I_H$.

Tự đồng cấu $u_H$ là compact (mệnh đề 3 của III, p. 5). Nó dương vì $\langle x|u_H(x)\rangle =\langle i_H(x)|u(i_H(x))\rangle \geqslant 0$ với mọi $x\in H$.

Lấy $n\in I_H\subset I_E$. Gọi F là một không gian con chiều $n+ 1$ của H thích nghi với $u_H$. Do đó $\lambda_n(u_H) =r_F(u_H)$ (mệnh đề 5 của IV, p. 153, a)), và hơn nữa vì $r_F(u_H) =r_F(u)\leqslant \lambda_n(u)$ (mệnh đề 6 của IV, p. 154), ta thu được mệnh đề a).

Giả sử rằng H có đối chiều $k\in \mathbf{N}$ trong E và rằng $n\in I_H$. Gọi F là một không gian con của H có chiều $n$ thích nghi với $u_H$. Trực giao bù của nó trong H bằng $H\cap F^{\circ}$, và đó là trực giao bù trong E của không gian con $F + H^{\circ}$ có chiều $n+k$. Do đó $n+k\in I_E$ và (mệnh đề 5 của IV, p. 153, b))

$\lambda_n(u_H) =$ sup $\frac{\langle x|u_H(x)\rangle}{2}= R_{F+H^{\circ}}(u)$

$$
_{x\in H\cap F^{\circ}}\|x\|
$$

$x\not =0$

do đó $\lambda_n(u_H)\leqslant \lambda_{n+k}(u)$ (mệnh đề 6 của IV, p. 154).

#### Định nghĩa 3 {#ts-iv-s1-def-3 .statement tag=02WR}

Cho F là một không gian Hilbert và $u$ là một ánh xạ tuyến tính compact từ E vào F.

Với mọi số nguyên $n\in I_E$ người ta ký hiệu $\alpha_n(u) =\lambda_n(u^*\circ u)$. Gọi J là tập hợp các $n\in I_E$ sao cho $\alpha_n(u)>0$. Họ $(\alpha_n(u))_{n\in J}$ được gọi là dãy các giá trị kỳ dị của $u$ lặp lại theo bội số.

Người ta nói rằng dãy $(\alpha_n(u))_{n\in I_E}$ là dãy mở rộng các giá trị kỳ dị của $u$.

Dãy $(\alpha_n(u))_{n\in I_E}$ được xác định tốt vì tự đồng cấu $u^*\circ u$ của E là compact (III, p. 5, mệnh đề 3); đó là một họ giảm các số thực dương vì $u^*\circ u$ là dương.

#### Mệnh đề 9 {#ts-iv-s1-prop-9 .statement tag=02WS}

Cho F là một không gian Hilbert và $u$ là một ánh xạ tuyến tính compact từ E vào F.

a) Với $n\in I_E$, ta có

$\alpha_n(u) =$ sup$_{F\in\mathscr{F}_{n+1}}$ inf$_{x\in F-\{0\}}\frac{\|u(x)\|}{\|x\|}=$ inf$_{F\in\mathscr{F}_n}$ sup$_{x\in F^{\circ-}\{0\}}\frac{\|u(x)\|}{\|x\|}$.

b) Gọi J là tập hợp các $n\in I_E$ sao cho $\alpha_n(u)\not = 0$. Tồn tại các họ trực chuẩn $(e_n)_{n\in J}$ trong E và $(f_n)_{n\in J}$ trong F sao cho với mọi $x\in E$, ta có

$$
u(x) =\sum_{n\in J}\alpha_n(u)\langle e_n|x\rangle f_n
$$

Vì $\langle x|u^*u(x)\rangle =\|u(x)\|^2$ với mọi $x\in E$, các định nghĩa và mệnh đề 6 của IV, p. 154, a), suy ra đẳng thức của mệnh đề thứ nhất.

Gọi $(e_n)_{n\in I_E}$ là một họ trực chuẩn của E thỏa mãn các kết luận của mệnh đề 3 của IV, p. 152 áp dụng cho tự đồng cấu dương compact $u^*\circ u$ của E. Đặt $f_n=\alpha^{-1}_nu(e_n)$ với $n\in J$. Bằng lập luận như trong chứng minh của hệ quả 2 của IV, p. 150, ta thu được mệnh đề c).

#### Hệ quả {#ts-iv-s1-n5-cor-1 .statement tag=02WT}

Cho F là một không gian Hilbert và $u$ một ánh xạ tuyến tính compact từ E vào F. Cho $w\in \mathscr{L}(E)$ và $v\in \mathscr{L}(F)$. Với mọi $n\in I_E$, ta có $\alpha_n(w\circ u\circ v)\leqslant \|v\| \|w\|\alpha_n(u)$.

Đây là một hệ quả của mệnh đề a) của mệnh đề trước.

#### Nhận xét 1 {#ts-iv-s1-n5-rem-1 .statement tag=02WU}

Vì dãy $(\alpha_n(u))_{n\in I_E}$ là giảm, tập hợp J hoặc bằng $I_E$, hoặc bằng một đoạn $\{0, . . . , m\}$ trong $I_E$ với $m\in \mathbf{N}$. Trường hợp sau này xảy ra khi và chỉ khi $u$ có hạng hữu hạn.

#### Nhận xét 2 {#ts-iv-s1-n5-rem-2 .statement tag=02WV}

Vì $\|u(x)\|=\||u|(x)\|$ với mọi $x\in E ($I, p. 139, mệnh đề 10), ta có $\alpha_n(u) =\alpha_n(|u|)$ với mọi $n\in I_E$.

#### Nhận xét 3 {#ts-iv-s1-n5-rem-3 .statement tag=02WW}

Nếu $u$ là dương, thì $\alpha_n(u) =\lambda_n(u)$ với mọi $n\in I_E$ (thật vậy, khi đó ta có $\alpha_n(u)^2=\lambda_n(u^*u) =\lambda_n(u^2) =\lambda_n(u)^2$ theo Mệnh đề 4 của IV, p. 153).

#### Nhận xét 4 {#ts-iv-s1-n5-rem-4 .statement tag=02WX}

Có thể xảy ra việc $\alpha_n(v\circ u\circ w) = 0$ ngay cả khi $\alpha_n(u)$ khác không; trong trường hợp này, $\alpha_n(v\circ u\circ w)$ không phải là một giá trị riêng suy biến của $v\circ u\circ w$.

### 6. Bất đẳng thức Weyl

Trong số này, ta xét các không gian Hilbert trên $K =\mathbf{C}$.

Cho E là một không gian Hilbert. Với mọi $n\in \mathbf{N}$, nhắc lại rằng lũy thừa ngoài Hilbert $\widehat{\wedge}^nE$ đã được định nghĩa trong EVT, V, p. 34. Với mọi không gian Hilbert F và với $u\in \mathscr{L}(E; F)$, ánh xạ tuyến tính $\widehat{\wedge}^nu\in \mathscr{L}(\widehat{\wedge}^nE;\widehat{\wedge}^nF) $ cũng đã được định nghĩa (loc. cit.). Các phép dựng này là hàm tử: với mọi không gian Hilbert G và với mọi ánh xạ tuyến tính $v\in \mathscr{L}(F; G)$, công thức

$$
\widehat{\wedge}^nv\circ \widehat{\wedge}^nu=\widehat{\wedge}^n(v\circ u)
$$

đúng (loc. cit., công thức (28)).

Cho H là một không gian con đóng của E và $i_H$ là đơn ánh chính tắc của H vào E. Với mọi tự đồng cấu $u$ của E, ta ký hiệu bởi $u_H$ tự đồng cấu $i^*_Hui_H$ của H.

#### Bổ đề 2 {#ts-iv-s1-lem-2 .statement tag=02WY}

Cho $n\in \mathbf{N}$. Ánh xạ $\widehat{\wedge}^ni_H$ là một ánh xạ tuyến tính đẳng cự từ $\widehat{\wedge}^nH$ vào $\widehat{\wedge}^nE$.

Cho $(e_j)_{j\in J}$ là một cơ sở trực chuẩn của H và $(e_j)_{j\in J'}$ là một cơ sở trực chuẩn của E, với $J\subset J'$. Trang bị cho $J'$ một thứ tự toàn phần. Các phần tử $e_{j_1}\wedge  \cdots  \wedge e_{j_n}$ với $j_1<\cdots < j_n$ trong $J'$ (tương ứng, trong J) tạo thành một cơ sở trực chuẩn của $\widehat{\wedge}^nE$ (tương ứng, của $\widehat{\wedge}^nH$) theo Mệnh đề 5 của EVT, V, p. 34, mệnh đề 5. Bổ đề được suy ra.

Trong phần sau, ta sẽ đồng nhất $\widehat{\wedge}^nH$ với một không gian con đóng của $\widehat{\wedge}^nE$ посредством ánh xạ $\widehat{\wedge}^ni_H$.

#### Bổ đề 3 {#ts-iv-s1-lem-3 .statement tag=02WZ}

Cho F là một không gian Hilbert và $u\in \mathscr{L}(E; F)$. Cho $n\in \mathbf{N}$.

a) Ta có $(\widehat{\wedge}^nu)^*=\widehat{\wedge}^n(u^*)$;

b) Nếu F = E và $u$ là Hermit (tương ứng, dương, chuẩn tắc, unita), thì $\widehat{\wedge}^nu$ là Hermit (tương ứng, dương, chuẩn tắc, unita) ;

c) Ta có $|\widehat{\wedge}^nu|=\widehat{\wedge}^n|u|$;

d) Cho H là một không gian con đóng của E. Hạn chế $(\widehat{\wedge}^nu)|\widehat{\wedge}^nH$ của $\widehat{\wedge}^nu$ lên $\widehat{\wedge}^nH$ bằng $\widehat{\wedge}^n(u|H) ($đẳng thức trong $\mathscr{L}(\widehat{\wedge}^nH;\widehat{\wedge}^nF))$;

e) Giả sử F = E. Cho H là một không gian con đóng của E. Ta có $(\widehat{\wedge}^nu)_{\widehat{\wedge}^nH}=\widehat{\wedge}^n(u_H)$ trong $\mathscr{L}(\widehat{\wedge}^nH)$.

Mệnh đề a) suy ra từ EVT, V, p. 39, công thức (13). Nó kéo theo ngay rằng $\widehat{\wedge}^nu$ là Hermit (tương ứng, unitary) khi $u$ là Hermit (tương ứng, unitary). Nếu $u$ là dương, thì $u^{1/2}$ là Hermit, do đó $\widehat{\wedge}^n(u^{1/2})$ cũng vậy; quan hệ $\widehat{\wedge}^nu=(\widehat{\wedge}^nu^{1/2})^2$ kéo theo rằng $\widehat{\wedge}^nu$ là dương (I, p. 138, mệnh đề 8). Điều này chứng minh b).

Điều ở trên cho phép tính được rằng

$$
(\widehat{\wedge}^n|u|)^2=\widehat{\wedge}^n(|u|^2) =\widehat{\wedge}^n(u^*u)
$$

$$
=\widehat{\wedge}^nu^*\widehat{\wedge}^nu=(\widehat{\wedge}^nu)^*(\widehat{\wedge}^nu) =|\widehat{\wedge}^nu|^2
$$

Vì $\widehat{\wedge}^n|u|$ là dương theo b), từ mệnh đề 16 của I, p. 118 suy ra $\widehat{\wedge}^n|u|=|\widehat{\wedge}^nu|$, do đó c).

Cho $i_H$ là đơn ánh chính tắc của H vào E. Không gian $\widehat{\wedge}^nH$ được đồng nhất với một không gian con đóng của $\widehat{\wedge}^nE$ bởi ánh xạ $\widehat{\wedge}^ni_H$, do đó

$$
(\widehat{\wedge}^nu)|\widehat{\wedge}^nH =\widehat{\wedge}^nu\circ \widehat{\wedge}^ni_H=\widehat{\wedge}^n(u\circ i_H) =\widehat{\wedge}^n(u|H)
$$

và

$$
(\widehat{\wedge}^nu)_{\widehat{\wedge}^nH}= (\widehat{\wedge}^ni_H)^*\circ \widehat{\wedge}^nu\circ \widehat{\wedge}^ni_H=\widehat{\wedge}^n(i^*_Hui_H) =\widehat{\wedge}^n(u_H)
$$

điều này chứng minh d) và e).

Cho F là một không gian Hilbert, và cho $u\in \mathscr{L}^c(E; F)$. Như trong IV, p. 151, ta ký hiệu bởi $I_E$ tập hợp các chiều của các không gian con hữu hạn chiều F của E sao cho $F\not = E$. Nhắc lại rằng $(\alpha_n(u))_{n\in I_E}$ ký hiệu dãy mở rộng các giá trị kỳ dị của $u$ (định nghĩa 3 của IV, p. 156).

#### Mệnh đề 10 {#ts-iv-s1-prop-10 .statement tag=02X0}

Ta có đẳng thức

$$
\prod_{i=0}^n\alpha_i(u) =\|\wedge^{n+1}u\|
$$

với mọi $n\in I_E$.

Bổ đề 3, c) chứng minh rằng $\|\widehat{\wedge}^{n+1}u\|=\|\widehat{\wedge}^{n+1}|u|\|$; hơn nữa, vì $\alpha_i(u) =\alpha_i(|u|)$ với mọi $i\in I_E$ (nhận xét 5 của IV, p. 157, (2)), chỉ cần chứng minh mệnh đề cho $|u|$. Điều này cho phép giả sử rằng F = E và $u$ là dương.

Khi đó, cho $B = (e_j)_{j\in J}$ là một cơ sở trực chuẩn của E sao cho $u$ chéo hóa được trong cơ sở B (định lý 1 của IV, p. 149), và cho $(\lambda_j)_{j\in J}$ là họ các giá trị riêng của $u$ trong cơ sở B. Trang bị cho J một thứ tự toàn phần, và ký hiệu bởi $J_n$ tập hợp các họ tăng ngặt $(j_0, . . . , j_n)\in J^{n+1}$ gồm các phần tử của J. Các vectơ

$$
e_{\iota}=e_{j_0}\wedge  \cdots  \wedge e_{j_n}
$$

với $\iota = (j_0, . . . , j_n)\in J_n$ tạo thành một cơ sở trực chuẩn $B_n$ của $\widehat{\wedge}^{n+1}E$ (EVT, V, p. 34, mệnh đề 5). Với mọi $\iota = (j_0, . . . , j_n)\in J_n$, đặt

$$
\lambda_{\iota}=\prod_{j=0}^n\lambda_{i_j}
$$

Khi đó $(\widehat{\wedge}^{n+1}u)e_{\iota}=\lambda_{\iota}e_{\iota}$, nên $\widehat{\wedge}^{n+1}u$ là đường chéo trong cơ sở $B_n$. Do đó, ta có

$\|\widehat{\wedge}^{n+1}u\|=$ sup$_{\iota\in I_n}\lambda_{\iota}$

(bổ đề 1 của IV, p. 147), bằng với tích $\lambda_0(u)\cdots \lambda_n(u)$ của $n+ 1$ giá trị riêng lớn nhất của $u$. Công thức phải chứng minh suy ra, vì $\lambda_i(u) =\alpha_i(u)$ với mọi $i\in I_E$ khi $u$ là dương (nhận xét 5 của IV, p. 157, (3)).

Đặc biệt, nếu $\alpha_1(u)< \alpha_0(u) =\|u\|$, ta thấy rằng bất đẳng thức $\|\widehat{\wedge}^n(u)\|\leqslant \|u\|^n$ (EVT, V, p. 34, công thức (29)) nói chung không phải là một đẳng thức nếu $n\geqslant 2$.

#### Hệ quả {#ts-iv-s1-n6-cor-1 .statement tag=02X1}

Cho G là một không gian Hilbert và $v\in \mathscr{L}^c(F; G)$. Khi đó

$$
\prod_{i=0}^n\alpha_i(v\circ u)\leqslant \prod_{i=0}^n\alpha_i(u)\alpha_i(v)
$$

với mọi $n\in I_E$.

Chỉ cần nhận xét rằng

$$
\|\widehat{\wedge}^{n+1}(vu)\|=\|\widehat{\wedge}^{n+1}v\circ \widehat{\wedge}^{n+1}u\|\leqslant \|\widehat{\wedge}^{n+1}v\| \|\widehat{\wedge}^{n+1}u\|
$$

và áp dụng mệnh đề 10.

#### Bổ đề 4 {#ts-iv-s1-lem-4 .statement tag=02X2}

Cho A là một vành. Cho $n\in \mathbf{N}$ và cho $(a_i)_{0\leqslant i\leqslant n}$ và $(b_i)_{0\leqslant i\leqslant n}$ là các họ phần tử của A. Với $0\leqslant j\leqslant n$, đặt

$$
A_j=\sum_{i=0}^ja_i
$$

Khi đó

$$
\sum_{i=0}^na_ib_i= A_nb_n-\sum^{n-1}_{i=0}A_i(b_{i+1}-b_i)
$$

Đặt $A_{-1}= 0$. Ta có $a_i= A_i-A_{i-1}$ với $0\leqslant i\leqslant n$, do đó

$$
\sum_{i=0}^na_ib_i=\sum_{i=0}^n(A_i-A_{i-1})b_i=\sum^{n-1}_{i=0}A_i(b_i-b_{i+1}) + A_nb_n
$$

như đã muốn chứng minh.

Cho I là một khoảng của $\overline{\mathbf{R}}$ không chứa $+\infty$. Nhắc lại (FVR, I, p. 38, nhận xét) rằng một hàm liên tục $f: I\rightarrow [-\infty ,+\infty [$ được gọi là lồi nếu hạn chế của nó lên phần trong của I là một hàm lồi nhận giá trị trong $\mathbf{R}$; khi đó nó có một giới hạn (hữu hạn hoặc vô hạn) bên phải tại inf I. Trong các mệnh đề dưới đây, tích của 0 với một phần tử của $\{-\infty ,+\infty \}$ được quy ước là bằng 0.

#### Bổ đề 5 {#ts-iv-s1-lem-5 .statement tag=02X3}

Cho $I\subset \overline{\mathbf{R}}$ là một khoảng không chứa $+\infty$, và cho $f$ là một hàm lồi tăng từ I vào $[-\infty ,+\infty [$.

Cho $n$ là một số tự nhiên, và cho

$$
a_0\geqslant a_1\geqslant \cdots \geqslant a_n,b_0\geqslant b_1\geqslant \cdots \geqslant b_n
$$

là các phần tử của I.

Cho $\varrho_0\geqslant \varrho_1\geqslant \cdots \geqslant \varrho_n$ là các số thực dương. Giả sử rằng

$$
\sum_{i=0}^ja_i\leqslant \sum_{i=0}^jb_i \tag{5}
$$

với mọi số nguyên $j$ sao cho $0\leqslant j\leqslant n$. Khi đó

$$
\sum_{i=0}^n\varrho_if(a_i)\leqslant \sum_{i=0}^n\varrho_if(b_i) \tag{6}
$$

Trước hết giả sử rằng $a_i\in \mathring{I}$, và do đó $f(a_i)\in \mathbf{R}$, với mọi $i$. Cho $i$ sao cho $0\leqslant i\leqslant n$, và cho $(\alpha_i, \beta_i)$ là các số thực sao cho đường thẳng có phương trình $y=\alpha_ix+\beta_i$ là một đường tựa của đồ thị của $f$ tại điểm $(a_i, f(a_i))$ (FVR, I, p. 37). Do đó ta có $f(a_i) =\alpha_ia_i+\beta_i$ và $f(b_i)\geqslant \alpha_ib_i+\beta_i$ vì đồ thị của $f$ nằm phía trên đường tựa, do đó

$$
f(b_i)-f(a_i)\geqslant \alpha_i(b_i-a_i) \tag{7}
$$

Hơn nữa, nếu $i < n$, ta có

$$
\alpha_i\geqslant f'_g(a_i)\geqslant f'_d(a_{i+1})\geqslant \alpha_{i+1}
$$

(loc. cit. và FVR, I, p. 36, hệ quả 1); hơn nữa $\alpha_i\geqslant 0$ vì $f$ tăng (FVR, I, p. 22, hệ quả), do đó $\varrho_i\alpha_i\geqslant \varrho_{i+1}\alpha_{i+1}\geqslant 0$ với $0\leqslant i < n$.

Cho $j$ là một số nguyên sao cho $0\leqslant j\leqslant n$. Đặt

$$
A_j=\sum_{i=0}^j(b_i-a_i)
$$

để cho $A_j\geqslant 0$ theo giả thiết (5). Áp dụng bất đẳng thức (7) rồi đến bổ đề 4, ta suy ra rằng

$$
\sum_{i=0}^n\varrho_i(f(b_i)-f(a_i))\geqslant \sum_{i=0}^n\varrho_i\alpha_i(b_i-a_i)
$$

$$
=\varrho_n\alpha_nA_n+\sum^{n-1}_{j=0}(\varrho_j\alpha_j-\varrho_{j+1}\alpha_{j+1})A_j\geqslant 0
$$

Xét trường hợp tổng quát, và lập luận bằng quy nạp theo $n$. Nếu một trong các $a_i$ không thuộc nội bộ của I, tất yếu ta có $a_0=$ sup I hoặc $a_n=$ inf I.

Trước hết giả sử $a_n$ = inf I. Khi đó ta có $a_n\leqslant b_n$ và vì vậy $\varrho_nf(a_n)\leqslant \varrho_nf(b_n)$. Giả thiết quy nạp, áp dụng cho các họ $(a_0, . . . , a_{n-1}), (b_0, . . . , b_{n-1})$ và $(\varrho_0, . . . , \varrho_{n-1})$, suy ra

$$
\sum^{n-1}_{i=0}\varrho_if(a_i)\leqslant \sum^{n-1}_{i=0}\varrho_if(b_i)
$$

do đó thu được bất đẳng thức cần chứng minh, bằng cách thêm $\varrho_nf(a_n)$. Trường hợp $a_0=$ sup I được xử lý tương tự.

#### Mệnh đề 11 (Các bất đẳng thức Weyl) {#ts-iv-s1-prop-11 .statement tag=02X4}

Cho G là một không gian Hilbert và $v\in \mathscr{L}^c(F; G)$. Cho $g:\mathbf{R}_+\rightarrow [-\infty ,+\infty [$ là một hàm tăng sao cho hàm $g\circ$ exp là lồi. Ta có

$$
\sum_{i=0}^ng(\alpha_i(v\circ u))\leqslant \sum_{i=0}^ng(\alpha_i(v)\alpha_i(u))
$$

với mọi $n\in I_E\cap I_F$.

Đặt $I = [-\infty ,+\infty [$ và $f=g\circ$ exp. Ta có thể áp dụng Bổ đề 5 với

$a_i=$ log($\alpha_i(v\circ u)$)$\in I,b_i=$ log($\alpha_i(v)\alpha_i(u)$)$\in I$

và $\varrho_i= 1$ với $0\leqslant i\leqslant n$, vì

$\sum_{i=0}^ja_i=$ log$(\prod_{i=0}^j\alpha_i(v\circ u))\leqslant$ log$(\prod_{i=0}^j\alpha_i(v)\alpha_i(u))=\sum_{i=0}^jb_i$

với $0\leqslant j\leqslant n$ theo hệ quả của Mệnh đề 10. Khi đó bất đẳng thức (6) chính là kết luận cần chứng minh.

#### Bổ đề 6 {#ts-iv-s1-lem-6 .statement tag=02X5}

Cho $g$ và $h$ là các hàm lồi xác định trên các khoảng I và J của $\mathbf{R}$, tương ứng. Nếu $g$ tăng và xác định trên ảnh của $h$, thì hàm $g\circ h$ là lồi trên J.

Thật vậy, với $t\in [0,1]$ và $(x, y)\in J\times J$, ta có

$$
g(h(tx+ (1-t)y))\leqslant g(th(x) + (1-t)h(y))
$$

$$
\leqslant tg(h(x)) + (1-t)g(h(y))
$$

#### Hệ quả {#ts-iv-s1-n6-cor-2 .statement tag=02X6}

Cho G là một không gian Hilbert và $v\in \mathscr{L}^c(F; G)$. Cho $n\in I_E\cap I_F$.

a) Cho $r\in \mathbf{R}^*_+$. Ta có

$$
\sum_{i=0}^n\alpha_i(v\circ u)^r\leqslant \sum_{i=0}^n\alpha_i(v)^r\alpha_i(u)^r
$$

b) Cho $p, q, r\in \mathbf{R}_+^*$ sao cho $\frac{1}{p}+\frac{1}{q}=\frac{1}{r}$. Khi đó

$$
(\sum_{i=0}^n\alpha_i(v\circ u)^r)^{1/r}\leqslant (\sum_{i=0}^n\alpha_i(v)^p)^{1/p}(\sum_{i=0}^n\alpha_i(u)^q)^{1/q}
$$

c) Giả sử F = E. Với mọi số nguyên $m\geqslant 2$, ta có

$$
\sum_{i=0}^n\alpha_i(u^m)\leqslant (\sum_{i=0}^n\alpha_i(u)^2)^{m/2}
$$

Cho $r\in \mathbf{R}^*_+$ và cho $g$ là hàm xác định trên $\mathbf{R}_+$ bởi $g(x) =x^r$. Hàm $g\circ$ exp là lồi (Bổ đề 6), và vì vậy mệnh đề a) suy ra từ Mệnh đề 11 áp dụng cho hàm $g$.

Mệnh đề b) suy ra từ a) và bất đẳng thức Hölder (INT, I, Mệnh đề 4).

Cho $m\geqslant 2$ là một số nguyên. Áp dụng b) với $r= 1,p=q= 2$ và $v=u^{m-1}$. Ta được

$$
\sum_{i=0}^n\alpha_i(u^m)\leqslant (\sum_{i=0}^n\alpha_i(u^{m-1})^2)^{1/2}(\sum_{i=0}^n\alpha_i(u)^2)^{1/2}
$$

Ta chứng minh c) bằng quy nạp theo $m\geqslant 2$. Bất đẳng thức trước chứng minh mệnh đề khi $m= 2$. Giả sử rằng $m\geqslant 3$ và mệnh đề là đúng với $m-1$; vì ta có

$$
\sum_{i=0}^n\alpha_i(u^{m-1})^2\leqslant (\sum_{i=0}^m\alpha_i(u^{m-1}))^2
$$

nên bất đẳng thức trên kéo theo

$$
\sum_{i=0}^n\alpha_i(u^m)\leqslant (\sum_{i=0}^n\alpha_i(u^{m-1}))^{1/2}(\sum_{i=0}^n\alpha_i(u)^2)^{1/2}\leqslant (\sum_{i=0}^n\alpha_i(u)^2)^{m/2}
$$

áp dụng giả thiết quy nạp.

### 7. Các Tự Đồng Cấu Có Vết Hữu Hạn

Nhắc lại rằng một tự đồng cấu dương $u$ của E có vết hữu hạn khi và chỉ khi tồn tại một cơ sở trực chuẩn $(e_i)_{i\in I}$ của E sao cho

$$
\sum_{i\in I}\langle e_i|u(e_i)\rangle <+\infty
$$

(EVT, V, p. 48, lemma 3 và p. 49, def. 7). Nếu $K =\mathbf{C}$, không gian $\mathscr{L}_1(E)$ các tự đồng cấu có vết hữu hạn của E là không gian vectơ sinh bởi tập hợp các tự đồng cấu dương có vết hữu hạn (EVT, V, p. 50, def. 8); nếu $K =\mathbf{R}$, không gian $\mathscr{L}_1(E)$ được định nghĩa là giao $\mathscr{L}(E)\cap \mathscr{L}_1(E_{(\mathbf{C})})$ (EVT, V, p. 50).

Nếu $u\in \mathscr{L}_1$(E), thì chuỗi

$$
\sum_{i\in I}\langle e_i|u(e_i)\rangle
$$

hội tụ đối với mọi cơ sở trực chuẩn $(e_i)_{i\in I}$ của E và tổng của nó độc lập với cơ sở trực chuẩn; ta nói rằng đó là vết Tr($u$) của $u$ (EVT, V, p. 50). Nếu $K =\mathbf{R}$, ta có Tr($u$) $=$ Tr($u_{(\mathbf{C})}$).

Cho $u\in \mathscr{L}_1(E)$. Ta có $u^*\in \mathscr{L}_1(E)$ và Tr($u^*$) $=$ Tr($u$) $($loc. cit.).

#### Mệnh đề 12 {#ts-iv-s1-prop-12 .statement tag=02X7}

Cho $B = (e_i)_{i\in I}$ là một cơ sở trực chuẩn của E. Cho $u\in \mathscr{D}_B(E)$ và ký hiệu bởi $\lambda = (\lambda_i)_{i\in I}$ họ các giá trị riêng của nó. Tự đồng cấu $u$ có vết hữu hạn khi và chỉ khi họ $\lambda$ là khả tổng trong K. Khi đó ta có Tr($u$) $=\sum\lambda_i$.

Nếu cần, thay thế $u$ bởi $u_{(\mathbf{C})}$, ta có thể giả sử rằng $K =\mathbf{C}$.

Trước hết giả sử rằng $u$ có vết hữu hạn. Theo EVT, V, p. 50 và p. 49, công thức (25), họ $(\langle e_i|u(e_i)\rangle )_{i\in I}= (\lambda_i)_{i\in I}$ là khả tổng.

Ngược lại, giả sử rằng họ $\lambda$ là khả tổng.

Khi đó, mỗi họ trong các họ $(\mathscr{R}(\lambda_i)^+), (\mathscr{R}(\lambda_i)^-), (\mathscr{I}(\lambda_i)^+), (\mathscr{I}(\lambda_i)^-)$ đều là khả tổng. Tự đồng cấu $u$ là một tổ hợp tuyến tính của các phần tử của $\mathscr{D}_B(E)$ có các họ ấy làm các giá trị riêng. Các phần tử này của $\mathscr{D}_B(E)$ là dương. Vì, theo định nghĩa, không gian các tự đồng cấu có vết hữu hạn được sinh bởi các tự đồng cấu dương có vết hữu hạn, do đó ta có thể giả sử rằng $\lambda_i\geqslant 0$ với mọi $i$. Vì $\langle e_i|u(e_i)\rangle =\lambda_i$, họ $(\langle e_i|u(e_i)\rangle )_{i\in I}$ là khả tổng, vậy nên $u$ có vết hữu hạn (EVT, V, p. 48, lemma 3).

Sau cùng, nếu $u$ có vết hữu hạn, thì theo EVT, V, p. 50, ta có

Tr($u$) $=\sum_{i\in I}\langle e_i|u(e_i)\rangle =\sum_{i\in I}\lambda_i$.

#### Hệ quả 1 {#ts-iv-s1-prop-12-cor-1 .statement tag=02X8}

Cho $u$ là một tự đồng cấu có vết hữu hạn của E.

a) Tự đồng cấu $u$ là compact;

b) Cho $B = (e_i)_{i\in I}$ là một cơ sở trực chuẩn của không gian ban đầu Ker($u$)$^{\circ}$ của $u$, $C = (f_i)_{i\in I}$ là một họ trực chuẩn trong E, và $(\alpha_i)_{i\in I}$ là một họ trong $(\mathbf{R}^*_+)^I$ sao cho $u(e_i) =\alpha_if_i$ với mọi $i\in I$ (hệ quả 2 của IV, p. 150). Ta có

Tr($u$) $=\sum_{i\in I}\alpha_i\langle e_i|f_i\rangle$.

Để chứng minh a), có thể giả sử rằng $K =\mathbf{C}$ (EVT, V, p. 50 và nhận xét 4 của III, p. 2) và rằng $u$ là dương (EVT, V, p. 50, định nghĩa 8).

Theo EVT, V, p. 56, hệ quả 1, tồn tại một cơ sở trực chuẩn $B = (e_i)_{i\in I}$ của E sao cho $u$ là đường chéo trong cơ sở B và hơn nữa họ $\lambda$ các trị riêng của $u$ thuộc $\mathbf{R}^I_+$ và khả tổng. Do đó họ $\lambda$ thuộc $\mathscr{C}_0(I; K)$ (TG, III, p. 38, mệnh đề 1), và do đó tự đồng cấu $u$ là compact (mệnh đề 2 của IV, p. 148).

Ta hãy chứng minh b). Cho $(e_i)_{i\in J}$ là một cơ sở trực chuẩn của E mở rộng họ B, sao cho $u(e_i) = 0$ nếu $i\in J$ - I. Khi đó

Tr($u$) $=\sum_{i\in J}\langle e_i|u(e_i)\rangle =\sum_{i\in I}\langle e_i|u(e_i)\rangle =\sum_{i\in I}\alpha_i\langle e_i|f_i\rangle$.

#### Hệ quả 2 {#ts-iv-s1-prop-12-cor-2 .statement tag=02X9}

Cho F là một không gian Hilbert. Cho $u\in \mathscr{L}(E; F)$ là một ánh xạ Hilbert-Schmidt. Khi đó $u$ là một ánh xạ tuyến tính compact.

Cho $(j,|u|)$ là phân tích cực của $u($I, p. 140, định nghĩa 4). Theo định nghĩa (EVT, V, p. 50, định nghĩa 9) tự đồng cấu $u^*u$ có vết hữu hạn,$\surd$ nên là compact (hệ quả 1, a)); điều tương tự cũng đúng với $|u|=u^*u$ (mệnh đề 6 của III, p. 91, b)) và với $u=j|u|$ (mệnh đề 3 của III, p. 5).

#### Hệ quả 3 {#ts-iv-s1-prop-12-cor-3 .statement tag=02XA}

Giả sử rằng $K =\mathbf{C}$. Cho $u$ là một tự đồng cấu compact dương của E. Tự đồng cấu $u$ có vết hữu hạn nếu và chỉ nếu họ giảm các trị riêng của nó $(\lambda_n(u))_{n\in I_E}$ là khả tổng; khi đó vết của $u$ là tổng của họ này.

Theo định lý 1 của IV, p. 149, điều này suy ra từ mệnh đề trên và từ định nghĩa của dãy $(\lambda_n(u))_{n\in I_E}$ (No$^o3$ của IV, p. 151), có kể đến công thức (28) của EVT, V, p. 49.

#### Hệ quả 4 {#ts-iv-s1-prop-12-cor-4 .statement tag=02XB}

Cho F là một không gian Hilbert. Cho $u\in \mathscr{L}(E; F)$ là một ánh xạ tuyến tính compact. Cho $B = (e_i)_{i\in I}$ là một cơ sở trực chuẩn của không gian ban đầu Ker($u$)$^{\circ}$ của $u$, $C = (f_i)_{i\in I}$ là một họ trực chuẩn trong F, và $(\alpha_i)_{i\in I}$ là một họ trong $(\mathbf{R}^*_+)^I$ sao cho $u(e_i) =\alpha_if_i$ với mọi $i\in I$ (hệ quả 2 của IV, p. 150).

Tự đồng cấu $|u|$ của E có vết hữu hạn nếu và chỉ nếu họ $(\alpha_i)_{i\in I}$ là khả tổng. Khi đó ta có $u\in \mathscr{L}_2(E; F)$ và

(8) Tr($|u|$) $=\sum_{i\in I}\alpha_i,\|u\|^2_2=$ Tr($u^*u$) $=\sum_{i\in I}\alpha^2_i$,

và đặc biệt $\|u\|_2\leqslant$ Tr($|u|$).

Họ các trị riêng khác không của $|u|$ là $(\alpha_i)_{i\in I}$, do đó $|u|$ có vết hữu hạn nếu và chỉ nếu họ $(\alpha_i)_{i\in I}$ là cộng được (Mệnh đề 12). Nếu đúng như vậy, thì họ $(\alpha^2_i)$ các trị riêng khác không của $u^*u=|u|^2$ là cộng được, và các công thức (8) suy ra từ nơi đã dẫn.

#### Bổ đề 7 {#ts-iv-s1-lem-7 .statement tag=02XC}

Cho $\lambda = (\lambda_i)_{i\in I}$ là một họ các số phức. Với mỗi $t\in \mathbf{C}^*$, gọi $n_t$ là lực lượng của tập hợp các $i\in I$ sao cho $\lambda_i=t$. Họ $(\lambda_i)_{i\in I}$ là cộng được nếu và chỉ nếu $n_t$ là hữu hạn với mỗi $t\in \mathbf{C}^*$ và họ $(n_tt)_{t\in\mathbf{C}^*}$ là cộng được. Trong trường hợp đó, tổng của hai họ này bằng nhau.

Giả sử họ $(\lambda_i)_{i\in I}$ là cộng được. Với mỗi $t\in \mathbf{C}$, gọi $I_t$ là tập hợp các $i\in I$ sao cho $\lambda_i=t$. Theo TG, III, p. 39, Định lý 2, áp dụng cho phân hoạch của I bởi các tập hợp $I_t$, tập hợp $I_t$ là hữu hạn với mỗi $t\in \mathbf{C}^*$, và hơn nữa họ $(n_tt)_{t\in\mathbf{C}^*}$ là cộng được, với tổng bằng tổng của họ $(\lambda_i)_{i\in I}$.

Ngược lại, giả sử $n_t$ là hữu hạn với mỗi $t\in \mathbf{C}^*$ và họ $(n_tt)_{t\in\mathbf{C}^*}$ là cộng được. Gọi J là một tập con hữu hạn của I và Λ là tập hợp các $\lambda_i$ với $i\in J$. Ta có

$$
|\sum_{i\in J}\lambda_i|\leqslant \sum_{t\in\Lambda-\{0\}}n_t|t|\leqslant \sum_{t\in\mathbf{C}^*}n_t|t|
$$

do đó họ $(\lambda_i)_{i\in I}$ là cộng được (TG, VII, p. 17, hệ quả).

#### Mệnh đề 13 {#ts-iv-s1-prop-13 .statement tag=02XD}

Giả sử $K =\mathbf{C}$. Cho $u$ là một tự đồng cấu chuẩn compắc của E. Với $t\in$ Sp$_s(u)$, gọi $n_t\geqslant 1$ là bội số phổ của trị riêng $t$ của $u$. Để $u$ có vết hữu hạn, điều kiện cần và đủ là họ $(n_tt)_{t\in Sp_s(u)}$ là cộng được. Khi đó vết của $u$ là tổng của họ này.

Cho $B = (e_i)_{i\in I}$ là một cơ sở trực chuẩn của E sao cho $u$ chéo trong cơ sở B (Định lý 1 của IV, p. 149), và gọi $\lambda = (\lambda_i)_{i\in I}$ là họ các trị riêng của nó. Vì, với $t\in$ Sp$_s(u)$, bội số $n_t$ bằng số phần tử $i\in I$ sao cho $\lambda_i=t$, và vì các phần tử khác không của $\lambda$ thuộc Sp$_s(u)$, nên mệnh đề suy ra từ Mệnh đề 12 và bổ đề trước đó.

### 8. Ánh xạ hạt nhân

Trong số này, F ký hiệu một không gian Hilbert trên K. Khi $K =\mathbf{C}$, nhắc lại rằng (I, p. $139\surd$, Định nghĩa 3), với $u\in \mathscr{L}(E; F)$, $|u|$ ký hiệu tự đồng cấu dương $u^*\circ u$ của E. Khi $K =\mathbf{R}$, phần tử $|u_{(\mathbf{C})}|$ của $\mathscr{L}(E_{(\mathbf{C})})$ có dạng $v_{(\mathbf{C})}$ đối với một tự đồng cấu duy nhất $v\in \mathscr{L}$ (E), và tự đồng cấu này lại được ký hiệu bởi $|u|($xem I, p. 87).

Ta ký hiệu bởi $(u, v)\mapsto  \langle u|v\rangle =$ Tr($u^*v$) tích vô hướng trong không gian Hilbert $\mathscr{L}_2(E; F)$ (EVT, V, p. 53, Nhận xét 1 và 2).

Với mọi $u\in \mathscr{L}(E; F)$, đặt $\|u\|_1=$ Tr($|u|$) nếu $|u|$ có vết hữu hạn và $\|u\|_1= +\infty$ nếu không phải như vậy. Do đó $\|u\|_1\in \mathbf{R}_+\cup \{+\infty \}$. Vì $\|u\|=\| |u| \|$ (Mệnh đề 10, a) của I, p. 139) và nếu $v$ là dương và có vết hữu hạn thì Tr($v$)$\geqslant \|v\|$ (EVT, V, p. 49, công thức (24bis) và p. 44, Mệnh đề 9), suy ra rằng

$$
\|u\|\leqslant \|u\|_1 \tag{9}
$$

Nếu $\|u\|_1$ là hữu hạn, thì $u$ là một ánh xạ Hilbert-Schmidt và $\|u\|_2\leqslant \|u\|_1$ (Hệ quả 4 của IV, p. 165).

#### Mệnh đề 14 {#ts-iv-s1-prop-14 .statement tag=02XE}

Cho $u\in \mathscr{L}_2(E; F)$. Khi đó

$\|u\|_1=$ sup$_{v\in\mathscr{L}_2(E;F)}|\langle v|u\rangle |$,

$\|v\|\leqslant 1$

ở đó cận trên bé nhất được lấy trong $\mathbf{R}_+\cup  \{+\infty \}$.

Cho $B = (e_i)_{i\in I}$ là một cơ sở trực chuẩn của không gian ban đầu Ker($u$)$^{\circ}$ của $u$, $C = (f_i)_{i\in I}$ là một họ trực chuẩn trong F và $(\alpha_i)_{i\in I}$ là một họ trong $(\mathbf{R}^*_+)^I$ sao cho $u(e_i) =\alpha_if_i$ với mọi $i\in I$ (Hệ quả 2 của IV, p. 150). Họ $(\alpha_i)_{i\in I}$ là bình phương-khả tổng vì $u$ thuộc $\mathscr{L}_2(E; F)$ (Hệ quả 4 của IV, p. 165). Cho $(e_j)_{j\in J}$ là một cơ sở trực chuẩn của E mở rộng $(e_i)_{i\in I}$.

Cho L là một tập con hữu hạn của I. Gọi $v_L$ là ánh xạ tuyến tính liên tục hữu hạn hạng từ E vào F được xác định bởi

$$
v_L(x) =\sum_{i\in L}\langle e_i|x\rangle f_i
$$

với mọi $x$ trong E. Ta có $\|v_L\|\leqslant 1$ và $v_L\in \mathscr{L}_2(E; F)$. Hơn nữa, với mọi $j\in J$, ta có $v_L(e_j) = 0$ nếu $j \notin L$ và $v_L(e_j) =f_j$ nếu $j\in L$. Do đó

$|\langle v_L|u\rangle |=|$Tr($v^*_Lu$)$|=|\sum_{j\in J}\langle v_L(e_j)|u(e_j)\rangle |=\sum_{j\in L}\alpha_j$.

Từ nơi dẫn trên, ta suy ra rằng

(10) $\|u\|_1=$ sup$_L\sum_{j\in L}\alpha_j\leqslant$ sup$_{v\in\|\mathscr{L}v^2\|(E;F)\leqslant 1}|\langle v|u\rangle |$

trong $\mathbf{R}_+\cup  \{+\infty \}$.

Điều này suy ra đẳng thức của mệnh đề khi $\|u\|_1= +\infty$.

Giả sử rằng $\|u\|_1$ là hữu hạn. Với mọi $i\in I$, gọi $p_i$ là ánh xạ tuyến tính từ E vào F sao cho $p_i(e_i) =f_i$ và $p_i(x) = 0$ với mọi $x\in e^{\circ}_i$. Với mọi $j$ và $k$ trong I, ta có

$\langle p_j|p_k\rangle =$ Tr($p^*_jp_k$) $=\sum_{i\in J}\langle p_j(e_i)|p_k(e_i)\rangle$,

biểu thức này bằng không trừ khi $j=k$, và trong trường hợp đó đại lượng này là $\|f_k\|^2= 1$. Do đó họ $(p_i)_{i\in I}$ là trực chuẩn trong $\mathscr{L}_2(E; F)$. Do đó, họ $(\alpha_ip_i)_{i\in I}$ là khả tổng trong $\mathscr{L}_2(E; F)$; tổng của nó bằng $u$ vì hai ánh xạ tuyến tính liên tục này trùng nhau trên các phần tử $e_i$ với mọi $i\in J$.

Gọi $v\in \mathscr{L}_2(E; F)$. Với mọi $i\in I$, ta có

$\langle v|p_i\rangle =$ Tr($v^*p_i$) $=\sum_{j\in J}\langle v(e_j)|p_i(e_j)\rangle =\langle v(e_i)|f_i\rangle$.

Nếu $\|v\|\leqslant 1$, khi đó ta thu được ước lượng

$$
|\langle v|u\rangle |=|\langle v|\sum_{i\in I}\alpha_ip_i\rangle |\leqslant \sum_{i\in I}\alpha_i|\langle v|p_i\rangle |
$$

$=\sum_{i\in I}\alpha_i|\langle v(e_i)|f_i\rangle |\leqslant \sum_{i\in I}\alpha_i=$ Tr($|u|$),

do đó bất đẳng thức

sup$_{v\in\|\mathscr{L}v^2\|(E;F)\leqslant 1}|\langle v|u\rangle |\leqslant \|u\|_1$,

bất đẳng thức này, kết hợp với công thức (10), hoàn tất chứng minh mệnh đề.

Từ mệnh đề này suy ra rằng tập hợp $\mathscr{L}_1(E; F)$ các ánh xạ tuyến tính liên tục $u$ từ E vào F sao cho $\|u\|_1$ là hữu hạn là một không gian con vectơ của $\mathscr{L}_2(E; F)$ và ánh xạ $u\mapsto  \|u\|_1$ là một nửa chuẩn trên $\mathscr{L}_1(E; F)$; bất đẳng thức (9) cho thấy đó là một chuẩn.

#### Định nghĩa 4 {#ts-iv-s1-def-4 .statement tag=02XF}

Người ta gọi không gian vectơ $\mathscr{L}_1(E; F)$ được trang bị chuẩn $u\mapsto  \|u\|_1$ là không gian các ánh xạ hạt nhân từ E vào F. Nếu $u\in \mathscr{L}_1(E; F)$, người ta nói rằng $u$ là hạt nhân.

#### Nhận xét 1 {#ts-iv-s1-n8-rem-1 .statement tag=02XG}

Giả sử rằng $K =\mathbf{R}$. Gọi $u\in \mathscr{L}(E; F)$. Ta có $u\in \mathscr{L}_1(E; F)$ khi và chỉ khi $u_{(\mathbf{C})}\in \mathscr{L}_1(E_{(\mathbf{C})}; F_{(\mathbf{C})})$; trong trường hợp đó, ta có $\|u\|_1=\|u_{(\mathbf{C})}\|_1$.

#### Nhận xét 2 {#ts-iv-s1-n8-rem-2 .statement tag=02XH}

Gọi $u$ là một ánh xạ hạt nhân từ E vào F. Vì ánh xạ $u$ thuộc kiểu Hilbert–Schmidt, nó là compact (hệ quả 2 của IV, p. 165). Hơn nữa, Mệnh đề 14 suy ra rằng với mọi $v\in \mathscr{L}_2(E; F)$, ta có

$$
|\langle v|u\rangle |\leqslant \|v\| \|u\|_1 \tag{11}
$$

#### Nhận xét 3 {#ts-iv-s1-n8-rem-3 .statement tag=02XI}

Giả sử rằng $K =\mathbf{C}$. Gọi $u\in \mathscr{L}_1(E; E)$ sao cho $u$ là dương. Chuẩn $\|u\|_1$ của $u$ là tổng của dãy $(\lambda_n(u))_{n\in I_E}$ (hệ quả 3 của IV, p. 165).

#### Nhận xét 4 {#ts-iv-s1-n8-rem-4 .statement tag=02XJ}

Phép nhúng chính tắc của $\mathscr{L}_1(E; F)$ vào $\mathscr{L}(E; F)$ có chuẩn $\leqslant 1$ (bất đẳng thức (9), p. 167).

#### Mệnh đề 15 {#ts-iv-s1-prop-15 .statement tag=02XK}

Cho G là một không gian Hilbert trên K. Ánh xạ $(u, v)\mapsto v\circ u$ từ $\mathscr{L}(E; F)\times \mathscr{L}(F; G)$ vào $\mathscr{L}(E; G)$ xác định, khi chuyển qua các không gian con, một ánh xạ song tuyến tính liên tục có chuẩn $\leqslant 1$ từ $\mathscr{L}_2(E; F)\times \mathscr{L}_2(F; G)$ vào $\mathscr{L}_1(E; G)$.

Cho $u\in \mathscr{L}_2(E; F)$ và $v\in \mathscr{L}_2(F; G)$. Cho $w\in \mathscr{L}_2(E; G)$. Ta có $\langle uv|w\rangle =$ Tr($v^*u^*w$) $=\langle v|u^*w\rangle$ do đó

$$
|\langle uv|w\rangle |\leqslant \|v\|_2\|u^*w\|_2\leqslant \|v\|_2\|u\|_2\|w\|
$$

theo bất đẳng thức Cauchy–Schwarz và công thức (37) của EVT, V, p 52. Kết quả vì thế suy ra từ Mệnh đề 14.

#### Bổ đề 8 {#ts-iv-s1-lem-8 .statement tag=02XL}

Ánh xạ $u\mapsto u^*$ từ $\mathscr{L}(E; F)$ vào $\mathscr{L}(F; E)$ xác định, khi chuyển qua các không gian con, một ánh xạ tuyến tính đẳng cự của $\mathscr{L}_1(E; F)$ vào $\mathscr{L}_1(F; E)$.

Cho $u\in \mathscr{L}_1(E; F)$. Vì $u$ là một ánh xạ Hilbert–Schmidt, điều đó cũng đúng với $u^*$ (EVT, V, p. 54). Ánh xạ $v\mapsto v^*$ là một song ánh từ tập hợp các $v\in \mathscr{L}_2(E; F)$ sao cho $\|v\|\leqslant 1$ lên tập hợp các $w\in \mathscr{L}_2(F; E)$ sao cho $\|w\|\leqslant 1$; với mọi $v\in \mathscr{L}_2(E; F)$ thỏa $\|v\|\leqslant 1$, ta có $\langle v|u\rangle =\langle u^*|v^*\rangle$ (EVT, V, p. 54, công thức (42)), do đó kết quả suy ra từ Mệnh đề 14.

#### Mệnh đề 16 {#ts-iv-s1-prop-16 .statement tag=02XM}

Cho $E_1$ và $F_1$ là các không gian Hilbert. Cho $u$ thuộc $\mathscr{L}_1(E; F),v$ thuộc $\mathscr{L}(E_1; E)$ và $v_2$ thuộc $\mathscr{L}(F; F_1)$. Khi đó $v_2uv_1\in \mathscr{L}_1(E_1; F_1)$ và $\|v_2uv_1\|_1\leqslant \|v_2\| \|v_1\| \|u\|_1$.

Cho $w\in \mathscr{L}_2(E; F_1)$ sao cho $\|w\|\leqslant 1$. Ta có $v_2u\in \mathscr{L}_2(E; F_1)$ (EVT, V, p. 52, công thức (36)). Vì $v^*_2w\in \mathscr{L}_2(E; F) ($loc. cit.), suy ra rằng

$$
|\langle w|v_2u\rangle |=|\langle v^*_2w|u\rangle |\leqslant \|v_2\| \|u\|_1
$$

(công thức (11)), do đó $v_2u\in \mathscr{L}_1(E; F_1)$ và $\|v_2u\|_1\leqslant \|v_2\|\|u\|_1$ (Mệnh đề 14).

Cho $v_1\in \mathscr{L}(E_1; E)$; vì $uv_1= (v^*_1u^*)^*$, ta có $uv_1\in \mathscr{L}_1(E_1; F)$ và $\|uv_1\|_1\leqslant \|v^*_1\| \|u^*\|_1=\|v_1\| \|u\|_1$ (Bổ đề 8).

Mệnh đề được suy ra ngay từ các bất đẳng thức này.

#### Mệnh đề 17 {#ts-iv-s1-prop-17 .statement tag=02XN}

Không gian $\mathscr{L}_1(E; E)$ trùng với không gian $\mathscr{L}_1(E)$ của các tự đồng cấu có vết hữu hạn của E, và ta có $|$Tr($u$)$|\leqslant \|u\|_1$ với mọi tự đồng cấu $u$ của E có vết hữu hạn.

Ta có thể giả sử rằng $K =\mathbf{C}$. Theo định nghĩa, không gian $\mathscr{L}_1(E; E)$ chứa tập hợp các tự đồng cấu dương có vết hữu hạn, và do đó $\mathscr{L}_1(E)\subset \mathscr{L}_1(E; E)$ (EVT, p. 50, định nghĩa 8). Ngược lại, hãy chứng minh rằng $\mathscr{L}_1(E; E)$ được chứa trong $\mathscr{L}_1(E)$.

Cho $u\in \mathscr{L}_1(E; E)$. Ta có $u^*\in \mathscr{L}_1(E; E)$ (bổ đề 8); vì vậy chỉ cần chứng minh rằng các phần tử Hermit của $\mathscr{L}_1(E; E)$ có vết hữu hạn (bổ đề 2 của I, p. 96).

Cho $u$ là một tự đồng cấu như vậy. Nó là compact (nhận xét 2, p. 169). Gọi B là một cơ sở trực chuẩn của E sao cho $u$ là đường chéo trong cơ sở B (Định lý 1 của IV, p. 149), và gọi $\lambda$ là họ các trị riêng của $u$ đối với B. Tự đồng cấu $|u|$ chéo hóa được trong cơ sở B và họ các trị riêng của nó là $|\lambda |$ (mệnh đề 1, d) của IV, p. 147). Vì $|u|$ có vết hữu hạn, họ sau là khả tổng (mệnh đề 12 của IV, p. 164), nên họ $\lambda$ là khả tổng. Do đó, $u$ có vết hữu hạn (loc. cit.), và ta có $|$Tr($u$)$|\leqslant$ Tr($|u|$) $=\|u\|_1$.

Do đó, không gian $\mathscr{L}_1(E)$ là một iđêan hai phía tự liên hợp của *-đại số $\mathscr{L}(E)$. Nếu E có chiều vô hạn, iđêan này không đóng trong $\mathscr{L}(E)$.

Các mệnh đề 17 và 16 chứng minh rằng dạng song tuyến tính $b$ trên $\mathscr{L}_1(E; F)\times \mathscr{L}(F; E)$ với giá trị trong $\mathbf{C}$ được xác định bởi $b(u, v) =$ Tr($vu$) là một dạng song tuyến tính liên tục đặt các không gian $\mathscr{L}_1(E; F)$ và $\mathscr{L}(F; E)$ vào thế đối ngẫu.

#### Bổ đề 9 {#ts-iv-s1-lem-9 .statement tag=02XO}

Cho $u\in \mathscr{L}_1(E; F)$. Ta có

$\|u\|_1=$ sup$_{v\in\mathscr{L}_c(F;E)}|b(u, v)|$.

$\|v\|\leqslant 1$

Vì mọi ánh xạ Hilbert-Schmidt đều compact (hệ quả 2 của IV, p. 165), ta có

$\|u\|_1\leqslant$ sup$_{v\in\|\mathscr{L}v\|^c(E;F)\leqslant 1}|$Tr($vu$)$|=$ sup$_{v\in\mathscr{L}\|v^c\|(F;E)\leqslant 1}|b(u, v)|$

theo mệnh đề 14.

Cho $v\in \mathscr{L}^c(E; F)$ có chuẩn $\leqslant$ 1. Vì $\mathscr{L}_2(E; F)$ trù mật trong $\mathscr{L}^c(E; F)$, tồn tại một dãy $(v_n)_{n\in\mathbf{N}}$ trong $\mathscr{L}_2(E; F)$ hội tụ tới $v$ trong $\mathscr{L}(E; F)$. Dãy $(b(u, v_n))_{n\in\mathbf{N}}$ hội tụ tới $b(u, v)$; vì $|b(u, v_n)|$ = $|$Tr($v_nu$)$|$ = $|\langle v_n^*|u\rangle |\leqslant \|u\|_1$ (mệnh đề 14) với mọi $n\in \mathbf{N}$, suy ra $|b(u, v)|\leqslant \|u\|_1$.

Ta ký hiệu bởi $\theta$ ánh xạ tuyến tính liên tục

$$
\theta :\mathscr{L}_1(E; F)\rightarrow \mathscr{L}^c(F; E)'
$$

sao cho $\theta (u)(v) =b(u, v)$.

#### Mệnh đề 18 {#ts-iv-s1-prop-18 .statement tag=02XP}

Ánh xạ $\theta$ là một đẳng cấu đẳng cự.

Theo bổ đề 9, ánh xạ $\theta$ là đẳng cự, và chỉ cần chứng minh rằng $\theta$ là toàn ánh.

Lấy $\lambda \in \mathscr{L}^c(F; E)'$. Vì $\|v\|\leqslant \|v\|_2$ với mọi $v\in \mathscr{L}_2(F; E)$ (EVT, V, p. 52, công thức (33)), hạn chế của $\lambda$ lên không gian con $\mathscr{L}_2(F; E)$ là một dạng tuyến tính liên tục trên không gian Hilbert $\mathscr{L}_2(F; E)$. Do đó tồn tại một phần tử $u$ của $\mathscr{L}_2(F; E)$ sao cho $\lambda (v) =\langle u|v\rangle$ với mọi $v\in \mathscr{L}_2(F; E)$ (EVT, V, p. 15, th. 3).

Với mọi $w\in \mathscr{L}_2(E; F)$ có chuẩn $\leqslant 1$, ta có $|\langle w|u\rangle |=|\lambda (w)|\leqslant \|\lambda \|$. Do đó, $u$ là một ánh xạ hạt nhân từ E vào F (mệnh đề 14).

Các dạng tuyến tính liên tục $\lambda$ và $\theta (u)$ bằng nhau trên không gian con trù mật $\mathscr{L}_2(F,E)$ của $\mathscr{L}^c(F; E)$. Suy ra $\lambda =\theta (u)$, điều này kết thúc chứng minh.

#### Hệ quả {#ts-iv-s1-n8-cor-1 .statement tag=02XQ}

Không gian định chuẩn $\mathscr{L}_1(E; F)$ là một không gian Banach.

Mệnh đề suy ra từ mệnh đề trên và từ EVT, III, p. 24, hệ quả 2 vì không gian $\mathscr{L}^c(F; E)$ là một không gian định chuẩn.

### 9. Toán tử tích phân Hilbert-Schmidt

Trong số này, X và Y là các không gian tôpô compact địa phương. Lấy $\mu$ là một độ đo dương trên X và $\nu$ là một độ đo dương trên Y. Ta ký hiệu bởi $L^2$(X), $L^2(Y)$ và $L^2(X\times Y)$ các không gian $L^2(X, \mu), L^2(Y, \nu )$ và $L^2(X\times Y, \mu\otimes \nu )$ tương ứng, và tương tự đối với $\mathscr{L}^2$(X), $\mathscr{L}^2(Y)$ và $\mathscr{L}^2(X\times Y)$.

Ta nhắc lại (xem số $^o4$ của III, p. 26) rằng với mọi $N\in \mathscr{L}^2(X\times Y)$, tồn tại duy nhất một ánh xạ tuyến tính liên tục $u_N$ từ $L^2(X)$ vào $L^2(Y)$ sao cho

$$
\langle g|u_N(f)\rangle =\int_{X\times Y}g(y)N(x, y)f(x)d(\mu\otimes \nu )(x, y) \tag{12}
$$

với mọi $f\in L^2(X)$ và mọi $g\in L^2(Y)$. Ánh xạ $u_N$ là compact (hệ quả 1 của III, p. 33). Ánh xạ $N\mapsto u_N$ cảm sinh, bằng cách chuyển qua các thương, một ánh xạ tuyến tính liên tục đơn ánh từ $L^2(X\times Y)$ vào $\mathscr{L}(L^2(X); L^2(Y))$ (mệnh đề 5 của III, p. 30).

Ta ký hiệu bởi $\theta$ ánh xạ tuyến tính duy nhất từ $\mathscr{L}^2(X)\otimes \mathscr{L}^2(Y)$ vào $\mathscr{L}^2(X\times Y)$ mà với mọi $f\in \mathscr{L}^2(X)$ và mọi $g\in \mathscr{L}^2(Y)$ gán hàm được xác định bởi $(x, y)\mapsto f(x)g(y)$.

#### Bổ đề 10 {#ts-iv-s1-lem-10 .statement tag=02XR}

Ánh xạ $\theta$ xác định, bằng cách chuyển qua các thương, một ánh xạ tuyến tính $\widetilde{\theta}$ từ $L^2(X)\otimes L^2(Y)$ vào $L^2(X\times Y)$, và tồn tại duy nhất một đẳng cấu đẳng cự từ $L^2(X)\widehat{\otimes}_2L^2(Y)$ lên $L^2(X\times Y)$ trùng với ánh xạ này trên $L^2(X)\otimes L^2(Y)$.

Mệnh đề thứ nhất là hiển nhiên. Ta hãy chứng minh mệnh đề thứ hai.

Cho $(f_i)_{i\in I}$ và $(g_j)_{j\in J}$ lần lượt là các cơ sở trực chuẩn của $L^2(X)$ và $L^2$(Y). Họ $(f_i\otimes g_j)_{(i,j)\in I\times J}$ là một cơ sở trực chuẩn của $L^2(X)\widehat{\otimes}_2L^2(Y)$ (EVT, V, p. 29, hệ quả 1) và họ $(\widetilde{\theta}(\overline{f}_i\otimes g_j))_{(i,j)\in I\times J}$ là trực chuẩn trong $L^2(X\times Y)$ (INT, V, p. 95, § 8, n$^o3$, hệ quả 2). Do đó ánh xạ $\widetilde{\theta}$ mở rộng bằng liên tục thành một ánh xạ tuyến tính đẳng cự từ $L^2(X)\widehat{\otimes}_2L^2(Y)$ vào $L^2(X\times Y)$. Còn phải chứng minh rằng phép mở rộng này là toàn ánh.

Để làm việc này, chỉ cần chứng minh rằng ảnh của $\widetilde{\theta}$ là trù mật trong $L^2(X\times Y)$. Cho N là một phần tử của $L^2(X\times Y)$ trực giao với ảnh của $\widetilde{\theta}$. Với mọi $i\in I$ và $j\in J$, ta có $\langle g_j|u_N(f_i)\rangle =\langle \widetilde{\theta}(\overline{f}_i\otimes g_j)|N\rangle = 0$ (công thức (12)), do đó $u_N= 0$, và vì thế N = 0.

Bổ đề trước thiết lập mệnh đề được phát biểu trong EVT, V, p. 29, ví dụ 2.

Từ nay về sau ta sẽ đồng nhất $L^2(X)\widehat{\otimes}_2L^2(Y)$ và $L^2(X\times Y)$ bằng đẳng cấu đẳng cự của Bổ đề 10.

#### Mệnh đề 19 {#ts-iv-s1-prop-19 .statement tag=02XS}

Ánh xạ $N\mapsto u_N$ là một đẳng cấu đẳng cự từ $L^2(X\times Y)$ lên không gian $\mathscr{L}_2(L^2(X); L^2(Y))$ các ánh xạ

of Hilbert–Schmidt deThe ánh xạ tuyến tính of L$L^2(X)_2$into$(Y)\otimes L\overset{2}{L}(Y)_2(X)$ into. $\mathscr{L}_2(L^2(X); L^2(Y))$ mà gán cho $g\otimes f$ ánh xạ Hilbert–Schmidt $h\mapsto  \langle f|h\rangle g$ mở rộng thành một đẳng cấu đẳng cự $\theta_1$ từ $L^2(Y)\widehat{\otimes}_2L^2(X)$ lên $\mathscr{L}_2(L^2(X); L^2(Y))$ (EVT, V, p. 52, định lý 1).

Hơn nữa, ký hiệu bởi $\theta_2$ đẳng cấu đẳng cự từ $L^2(X)\widehat{\otimes}_2L^2(Y)$ lên $L^2(Y)\widehat{\otimes}_2L^2(X)$ mà với mọi $f\in L^2(X)$ và mọi $g\in L^2(Y)$ gán cho $f\otimes g$ phần tử $g\otimes \overline{f}$.

Ánh xạ tuyến tính $\theta_3=\theta_1\circ \theta_2$ được đồng nhất với một đẳng cấu đẳng cự từ $L^2(X\times Y)$ lên $\mathscr{L}_2(L^2(X); L^2(Y))$.

Cho $f\in L^2(X)$ và $g\in L^2$(Y), và cho N là phần tử của $L^2(X\times Y)$ được đồng nhất với $f\otimes g$. Từ INT, V, p. 95, § 8, n$^o3$, hệ quả 2 và công thức (12) ta có

$$
\langle g_1|u_N(f_1)\rangle =\langle \overline{f}|f_1\rangle  \langle g_1|g\rangle
$$

với mọi $f_1\in L^2(X)$ và $g_1\in L^2(Y)$. Ánh xạ $u=\theta_3(N)$ là ánh xạ tuyến tính $\theta_1(g\otimes f)$; do đó nó thỏa mãn $u(h) =\langle f|h\rangle g$ với mọi $h\in L^2(X)$. Do đó, với mọi $f_1\in L^2(X)$ và $g_1\in L^2$(Y), ta có

$$
\langle g_1|u(h_1)\rangle =\langle \overline{f}|h_1\rangle  \langle g_1|g\rangle =\langle g_1|u_N(h_1)\rangle
$$

do đó $\theta_3(N) =u_N$. Vì $\theta_3$ và $N\mapsto u_N$ là liên tục, suy ra $\theta_3(N) =u_N$ với mọi $N\in L^2(X\times Y)$, điều này hoàn tất chứng minh.

#### Hệ quả {#ts-iv-s1-n9-cor-1 .statement tag=02XT}

Với mọi $N\in L^2(X\times Y)$, ánh xạ tuyến tính $u_N$ là một ánh xạ Hilbert–Schmidt và ta có Tr($u^*_Nu_N$) $=\|N\|^2$.

Thực vậy, ta có $\|u\|_2=\surd$Tr($u^*u$) với mọi $u\in \mathscr{L}_2(L^2(X); L^2(Y))$.

#### Nhận xét {#ts-iv-s1-n9-rem-1 .statement tag=02XU}

Cho $N\in L^2(X\times Y)$. Theo hệ quả 2 của IV, p. 150, tồn tại một tập hợp đếm được I, các họ trực chuẩn $(f_i)_{i\in I}$ trong $L^2(X)$ và $(g_i)_{i\in I}$ trong $L^2$(Y), cũng như một họ $(\alpha_i)_{i\in I}$ trong $\mathbf{R}^*_+$, sao cho

$$
u_N(f) =\sum_{i\in I}\alpha_i\langle f_i|f\rangle g_i
$$

với mọi $f\in L^2$(X), trong đó chuỗi hội tụ trong $L^2(Y)$. Theo hệ quả 4 của IV, p. 165 và hệ quả trên, ta có

$\sum_{i\in I}\alpha^2_i=$ Tr($u^*_Nu_N$) $=\|u_N\|^2_2=\int_{X\times Y}|N(x, y)|^2d(\mu\otimes \nu )(x, y)$.

Đặt thêm $h_{i,j}=\overline{f}_i\otimes g_j\in L^2(X\times Y)$ với mọi $(i, j)\in I\times I$. Khi đó ta có

$$
N =\sum_{i\in I}\alpha_ih_{i,i}
$$

trong $L^2(X\times Y)$.

Thực vậy, cho $(f_j)_{j\in J}$ và $(g_k)_{k\in K}$ là các cơ sở trực chuẩn của $L^2(X)$ và $L^2$(Y), tương ứng, mở rộng các họ $(f_i)_{i\in I}$ và $(g_i)_{i\in I}$. Đặt $h_{j,k}=\overline{f}_j\otimes g_k$ với mọi $(j, k)\in J\times K$. Theo bổ đề 10, họ $(h_{j,k})_{(j,k)\in J\times K}$ là một cơ sở trực chuẩn của $L^2(X\times Y)$. Ta có $\langle h_{j,k}|N\rangle =\langle g_k|u_N(f_j)\rangle$ với mọi $(j, k)\in J\times K$. Nếu $j \notin I$, đại lượng này bằng không. Nếu $j\in I$, nó bằng $\alpha_j\langle g_k|g_j\rangle$, do đó bằng không trừ khi $k=j$, trong trường hợp đó $\langle h_{j,j}|N\rangle =\alpha_j$. Do đó

$$
N =\sum_{(j,k)\in J\times K}\langle h_{j,k}|N\rangle h_{j,k}=\sum_{i\in I}\alpha_ih_{i,i}
$$

### 10. Vết của các toán tử tích phân với hạt nhân liên tục

Trong số này, các quy ước của số trước vẫn được giữ lại với Y = X và $\nu =\mu$. Giả thiết rằng X là một không gian tôpô compact địa phương đếm được ở vô cùng (TG, I, p. 68, Định nghĩa 5).

Đặc biệt, ta đồng nhất các không gian $L^2(X\times X)$ và $L^2(X)\widehat{\otimes}_2L^2(X)$ (bổ đề 10 của IV, p. 172). Ta sẽ ký hiệu bởi $\widetilde{f}$ lớp trong $L^2(X)$ (tương ứng trong $L^2(X\times X)$) của một hàm $f\in \mathscr{L}^2(X)$ (tương ứng trong $\mathscr{L}^2(X\times X)$).

#### Mệnh đề 20 {#ts-iv-s1-prop-20 .statement tag=02XV}

Cho $(f_n)_{n\in\mathbf{N}}$ là một dãy các ánh xạ đo được từ X vào một không gian mêtric hóa được F. Giả sử rằng giới hạn của $f_n(x)$ tồn tại trên phần bù của một tập con không đáng kể đối với $\mu$ của X. Tồn tại một dãy $(C_m)_{m\in\mathbf{N}}$ các tập con compact của X mà hợp $\widetilde{X}$ của chúng thỏa mãn $|\mu|(X-\widetilde{X}) = 0$, sao cho các hàm $f_n$ liên tục trên $C_m$ với mọi $n\in \mathbf{N}$ và mọi $m\in \mathbf{N}$, và dãy $(f_n)_{n\in\mathbf{N}}$ hội tụ đều đến $f$ trên $C_m$ với mọi $m\in \mathbf{N}$.

Suy ra từ định lý 2 của INT, IV, p. 175, § 5, n$^o4$ và mệnh đề 12, b) của INT, IV, p. 188, § 5, n$^o8$, rằng tập hợp các tập con compact C của X sao cho các hàm $f_n$ liên tục trên C với mọi $n$, và sao cho $(f_n)$ hội tụ đều đến $f$ trên C, là $\mu$-trù mật trong X (INT, IV, p. 189, § 5, n$^o8$, định nghĩa 6). Khi đó mệnh đề được suy ra từ nhận xét trong INT, IV, p. 189, §5, n$^o8$.

Cho N là một hàm thuộc $\mathscr{L}^2(X\times X)$ và cho $u_N$ là ánh xạ Hilbert-Schmidt từ $L^2(X)$ vào $L^2(X)$ có hạt nhân N (mệnh đề 19 của IV, p. 173). Vì ánh xạ $u_N$ là compact, nên theo mệnh đề 9 của IV, p. 156, tồn tại một phần tử M của $\mathbf{N}$ và, ký hiệu bởi I tập hợp các số nguyên $n\in \mathbf{N}$ sao cho $n\leqslant M$, các họ trực chuẩn $(f_i)_{i\in I}$ và $(g_i)_{i\in I}$ trong $\mathscr{L}^2(X)$ và một họ $(\alpha_i)_{i\in I}$ trong $\mathbf{R}^*_+$ sao cho

$$
u_N(f) =\sum_{i\in I}\alpha_i\langle \widetilde{f}_i|f\rangle \widetilde{g}_i \tag{13}
$$

với mọi $f\in L^2$(X), trong đó chuỗi hội tụ trong $L^2(X)$.

Với mỗi $i\in I$, cho $h_i\in \mathscr{L}^2(X\times X)$ ký hiệu hàm được xác định bởi $h_i(x, y) =f_i(x)g_i(y)$, do đó $\widetilde{h}_i$ là lớp của $f_i\otimes g_i$. Theo nhận xét 9 của IV, p. 173, chuỗi có số hạng tổng quát $\alpha_ih_i$ hội tụ đến N trong $L^2(X\times X)$.

Trong phần còn lại của số này, ta giả sử rằng N là một hàm liên tục.

#### Mệnh đề 21 {#ts-iv-s1-prop-21 .statement tag=02XW}

Giả sử rằng $u_N$ có vết hữu hạn. Khi đó tồn tại một tập hợp $\widetilde{X}\subset X$ mà phần bù X $-\widetilde{X}$ của nó là $\mu$-không đáng kể và một hàm $H\in \mathscr{L}^2(X\times X)$ thỏa mãn các điều kiện sau :

(i) Với mọi $(x, y)\in \widetilde{X}\times \widetilde{X}$, họ $(\alpha_if_i(x)g_i(y))_{i\in I}$ là khả tổng trong $\mathbf{C}$ và tổng của nó là $N(x, y)$;

(ii) Với mọi tập con hữu hạn J của I và mọi $(x, y)\in \widetilde{X}\times \widetilde{X}$, ta có

$$
|\sum_{i\in J}\alpha_ih_i(x, y)|\leqslant H(x, y) \tag{14}
$$

(iii) Hàm $x\mapsto H(x, x)$ thuộc $\mathscr{L}^1(X)$.

Vì $u_N$ có vết hữu hạn, họ $(\alpha_i)$ là hội được (hệ quả 4 của IV, p. 165). Do đó các chuỗi

$$
\sum_{i\in I}\alpha_i|f_i|^2,\sum_{i\in I}\alpha_i|g_i|^2
$$

hội tụ trong $\mathscr{L}^1(X)$ và do đó $\mu$-hầu khắp nơi (INT, IV, p. 128, § 3, n$^o3$, mệnh đề 6). Ký hiệu F và G, tương ứng, là các hàm được xác định $\mu$-hầu khắp nơi bởi tổng của các chuỗi này, đặt $F(x) = 0$ và $G(x) = 0$ với mọi $x$ sao cho chuỗi tương ứng không hội tụ. Vì F và G thuộc $\mathscr{L}^1$(X), hàm H xác định bởi $H(x, y) =\surd F(x)G(y)$ thuộc $\mathscr{L}^2(X\times X)$ (INT, V, p. 95, § 8, n$^o3$, hệ quả 2).

Áp dụng mệnh đề 20 cho không gian X, cho $F =\mathbf{C}^2$, và cho các ánh xạ đo được

$$
s_n:x\mapsto (\sum_{i\in I}\alpha_i|f_i(x)|^2,\sum_{i\in I}\alpha_i|g_i(x)|^2)
$$

$i\leqslant ni\leqslant n$

được xác định trên X. Do đó tồn tại một dãy $(C_m)_{m\in\mathbf{N}}$ các tập con compact của X thỏa mãn các điều kiện sau:

(1) hợp $\widetilde{X}$ thỏa mãn $\mu(X-\widetilde{X}) = 0$;

(2) với mọi $m\in \mathbf{N}$ và mọi $n\in \mathbf{N}$, các hàm $s_n$ liên tục trên $C_m$;

(3) với mọi $m\in \mathbf{N}$, các chuỗi $\sum\alpha_i|f_i|^2$ và $\sum\alpha_i|g_i|^2$ hội tụ đều trên $C_m$ lần lượt đến F và G;

(4) giá của độ đo cảm sinh bởi $\mu$ trên $C_m$ bằng $C_m$ (thay thế $C_m$ bởi giá của độ đo này nếu cần).

Ta sẽ chứng minh rằng tập hợp $\widetilde{X}$ và hàm H thỏa mãn các điều kiện (i), (ii), và (iii).

Lấy $(x, y)\in \widetilde{X}\times \widetilde{X}$. Với mọi tập con hữu hạn $J\subset I$, ta có

$$
|\sum_{i\in J}\alpha_i\overline{f_i(x)}g_i(y)|\leqslant (\sum_{i\in J}\alpha_i|f_i(x)|^2)^{1/2}(\sum_{i\in J}\alpha_i|g_i(y)|^2)^{1/2} \tag{15}
$$

do đó cũng có

$$
|\sum_{i\in J}\alpha_i\overline{f_i(x)}g_i(y)|\leqslant H(x, y) \tag{16}
$$

điều này đã thiết lập tính chất (ii).

Theo bất đẳng thức (15), chuỗi $\sum_i\alpha_ih_i$ hội tụ đều trên $K_m\times K_n$ với mọi $(m, n)\in \mathbf{N}^2$. Ký hiệu $\widetilde{N}$ là hàm trên $X\times X$ được xác định bởi

$$
\widetilde{N}(x, y) =\sum_{i\in I}\alpha_ih_i(x, y) =\sum_{i\in I}\alpha_i\overline{f_i(x)}g_i(y)
$$

với mọi $(x, y)\in \widetilde{X}\times \widetilde{X}$ và bởi $\widetilde{N}(x, y) = 0$ trong trường hợp ngược lại. Hàm $\widetilde{N}$ là đo được (INT, IV, p. 175, § 5, n$^o4$, định lý 2), và nó liên tục trên $K_m\times K_n$ với mọi $(m, n)\in \mathbf{N}^2$.

Từ (16), ta có $|\widetilde{N}(x, y)|\leqslant H(x, y)$ với mọi $(x, y)\in X\times X$, và đặc biệt $\widetilde{N}$ thuộc $\mathscr{L}^2(X\times X)$ (INT, IV, p. 84, § 5, n$^o6$, định lý 5).

Ta sẽ chứng minh rằng $N =\widetilde{N}$ trên $\widetilde{X}\times \widetilde{X}$, điều này sẽ thiết lập tính chất (i). Cho $f$ và $g$ là các phần tử của $\mathscr{L}^2(X)$. Ta có

$$
\langle g|u_{\widetilde{N}}(f)\rangle =\int_{X\times X}\widetilde{N}(x, y)f(x)\overline{g(y)}d(\mu\otimes \mu)(x, y)
$$

(công thức (12) của IV, p. 172). Với mọi $(x, y)\in \widetilde{X}\times \widetilde{X}$ và mọi tập con hữu hạn J của I, ta có

$$
|\sum_{i\in J}\alpha_i\overline{f_i(x)}g_i(y)f(x)\overline{g(y)}|\leqslant |f(x)g(y)|H(x, y)
$$

theo công thức (16). Vì vế phải của bất đẳng thức này khả tích trên $X\times X$ (INT, V, p. 95, § 8, n$^o3$, hệ quả 2), ta có thể áp dụng định lý Lebesgue (INT, IV, p. 137, § 3, n$^o7$, định lý 6) và công thức (13), và suy ra rằng

$$
\langle g|u_{\widetilde{N}}(f)\rangle =\sum_{i\in I}\alpha_i\int_{X\times X}\overline{f_i(x)}g_i(y)f(x)\overline{g(y)}d(\mu\otimes \mu)(x, y)
$$

$$
=\sum_{i\in I}\alpha_i\langle f_i|f\rangle \langle g|g_i\rangle =\langle g|u_N(f)\rangle
$$

Do đó, ta được $u_{\widetilde{N}}=u_N$, và vì thế $N =\widetilde{N}$ trong $L^2(X\times X)$ (mệnh đề 3 của III, p. 28, b)).

Với mọi $(m, n)\in \mathbf{N}^2$, các hàm N và $\widetilde{N}$ liên tục trên $K_m\times K_n$ và do đó bằng nhau trên $K_m\times K_n$ (mệnh đề 9 của INT, III, p. 69, § 2, n$^o2$), vì giá của độ đo cảm sinh bởi $\mu\otimes \mu$ trên $K_m\times K_n$ bằng $K_m\times K_n$. Vậy N trùng với $\widetilde{N}$ trên $\widetilde{X}\times \widetilde{X}$.

$$
\surd
$$

Sau cùng, ước lượng FG $\leqslant (F + G)/2$ kéo theo rằng hàm $x\mapsto \surd F(x)G(x) = H(x, x)$ khả tích trên X, do đó có tính chất (iii).

Trong phần còn lại của số này, ta giữ ký hiệu của mệnh đề.

#### Định lý 2 {#ts-iv-s1-thm-2 .statement tag=02XX}

Giả sử rằng $u_N$ có vết hữu hạn. Khi đó hàm $x\mapsto N(x, x)$ thuộc $\mathscr{L}^1(X)$ và ta có

Tr($u_N$) $=\int_XN(x, x)d\mu(x)$.

Từ các điều kiện (i) và (ii), ta có $|N(x, x)|\leqslant H(x, x)$ với $x\in \widetilde{X}$, do đó hàm $x\mapsto N(x, x)$ thuộc $\mathscr{L}^1(X)$ theo điều kiện (iii).

Điều kiện (i) thiết lập đẳng thức

$$
N(x, x) =\sum_{i\in I}\alpha_i\overline{f_i(x)}g_i(x)
$$

với mọi $x\in \widetilde{X}$. Từ các điều kiện (ii) và (iii), ta có thể áp dụng định lý Lebesgue (INT, IV, p. 137, § 3, n$^o7$, định lý 6), từ đó suy ra rằng

$$
\int_XN(x, x)d\mu(x) =\sum_{i\in I}\alpha_i\int_X\overline{f_i(x)}g_i(x)d\mu(x)
$$

$=\sum_{i\in I}\alpha_i\langle f_i|g_i\rangle =$ Tr($u_N$),

đẳng thức cuối cùng thu được từ hệ quả của mệnh đề 17 của IV, p. 170.

#### Bổ đề 11 {#ts-iv-s1-lem-11 .statement tag=02XY}

Nếu tự đồng cấu $u_N$ của $L^2(X)$ là dương, thì $N(x, x)\geqslant 0$ với mọi $x$ trong giá của $\mu$.

Vì $u_N$ là dương, các họ $(f_i)$ và $(g_i)$ có thể được chọn sao cho $f_i=g_i$ với mọi $i\in I$ (nhận xét 3 của IV, p. 151). Khi đó, với mọi $x\in \widetilde{X}$, ta có

$$
N(x, x) =\sum_{i\in I}\alpha_i|f_i(x)|^2\geqslant 0
$$

Vì N liên tục, và $\mu(X-\widetilde{X}) = 0$, nên hàm N là dương trên giá của $\mu$.

#### Nhận xét {#ts-iv-s1-n10-rem-1 .statement tag=02XZ}

Mệnh đề đảo lại của bổ đề không đúng (bài tập 14 của IV, p. 316).

#### Mệnh đề 22 {#ts-iv-s1-prop-22 .statement tag=02Y0}

Giả sử rằng $u_N$ là một tự đồng cấu dương của $L^2(X)$. Khi đó tự đồng cấu $u_N$ có vết hữu hạn khi và chỉ khi hàm $x\mapsto N(x, x)$ là $\mu$-khả tích. Trong trường hợp đó, ta có

Tr($u_N$) $=\int_XN(x, x)d\mu(x)$.

Nếu $u_N$ có vết hữu hạn, Định lý 2 kéo theo rằng $x\mapsto N(x, x)$ khả tích trên X và tích phân của nó là vết của $u_N$.

Ngược lại, giả sử rằng hàm $x\mapsto N(x, x)$ khả tích. Vì $u_N$ dương, các họ trực chuẩn $(f_i)_{i\in I}$ và $(g_i)_{i\in I}$ có thể được chọn sao cho $f_i=g_i$ với mọi $i\in I$ (nhận xét 3 của IV, p. 151). Với mọi $x\in \widetilde{X}$, ta có

$$
N(x, x) =\sum_{i\in I}\alpha_i|f_i(x)|^2
$$

do đó, với mọi tập con hữu hạn J của I, suy ra

$$
\sum_{i\in J}\alpha_i=\sum_{i\in J}\alpha_i\int_X|f_i(x)|^2d\mu(x)
$$

$$
=\int_X\sum_{i\in J}\alpha_i|f_i(x)|^2d\mu(x)\leqslant \int_XN(x, x)d\mu(x)
$$

Vì thế họ $(\alpha_i)_{i\in I}$ là khả tổng, điều này kéo theo rằng tự đồng cấu $u_N$ có vết hữu hạn (mệnh đề 12 của IV, p. 164).

#### Nhận xét {#ts-iv-s1-n10-rem-2 .statement tag=02Y1}

Ngay cả khi X compact và N liên tục, tự đồng cấu $u_N$ của $L^2(X)$ cũng không phải lúc nào cũng có vết hữu hạn (xem bài tập 8 của IV, p. 314).

## BÀI TẬP {#ts-iv-s1-exercises}

Xem [các bài tập cho § 1](exercises/s1/).
