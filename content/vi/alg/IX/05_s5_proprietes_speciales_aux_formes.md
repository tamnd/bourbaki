---
book: alg
book_title: Algebra
chapter: IX
chapter_title: Formes sesquilinéaires et formes quadratiques
section: 5
section_title: Propriétés spéciales aux formes bilinéaires alternées
lang: vi
source: alg-ix-fr
pdf_pages: 0077-0087
extraction: ocr
subsections:
    - "no": 1
      title: Réduction des formes bilinéaires alternées.
      page: 0
      pdf_page: 77
    - "no": 2
      title: Pfaffien d'une matrice alternée.
      page: 0
      pdf_page: 80
    - "no": 3
      title: Groupe symplectique.
      page: 0
      pdf_page: 82
statements: 11
exercises: 0
content_sha256: bbf73dc3e18be88e948aa2a70bf4e4f40cad9b9970be960671cee6177009390d
translated_from: content/en-mt/alg/IX/05_s5_proprietes_speciales_aux_formes.md
source_lang: en-mt
translation_method: machine
source_content_sha256: 37eab0972d32d48c50fe1f46c6408db705441dc829547205d88946bff9026a86
translation_model: gpt-5.4
translation_run: translate-vi-5eb1c5d9
glossary_version: 34
glossary_terms_sha256: 459b7c6e5e1cc1613484906fedaca5d05223ac2650eb5aba500c69aeca41d989
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 5. Các tính chất đặc biệt của các dạng song tuyến tính phản xứng

### 1. Quy giản các dạng song tuyến tính phản xứng.

#### Định lý 1 {#alg-ix-s5-thm-1 .statement}

Cho $A$ là một vành chính (giao hoán), $E$ là một $A$-môđun tự do có số chiều hữu hạn $n$ và $\Phi$ là một dạng song tuyến tính phản xứng trên $E$. Khi đó tồn tại một cơ sở $(e_i)_{1 \leq i \leq n}$ của $E$ và một số nguyên chẵn $2r \leq n$, sao cho

$1^o$ $\Phi(e_1, e_2) = \alpha_1, \Phi(e_3, e_4) = \alpha_2, \ldots, \Phi(e_{2r-1}, e_{2r}) = \alpha_r$

trong đó các $\alpha_i$ là các phần tử $\neq 0$ của $A$, và trong đó $\alpha_i$ chia $\alpha_{i+1}$ với $i = 1, \ldots, r-1$.

$2^o$ Mọi giá trị khác $\Phi(e_i, e_j)$ với $i \leq j$ đều bằng không.

Các iđêan $A \alpha_i$ ($i = 1, \ldots, r$) được xác định duy nhất bởi các điều kiện trước. Môđun con $E^0$ của $E$ trực giao với $E$ được sinh bởi $e_{2r+1}, \ldots, e_n$.

Ta sẽ tiến hành bằng quy nạp theo chiều $n$ của $E$. Định lý là hiển nhiên đối với $n = 0$. Nếu $\Phi = 0$, định lý cũng hiển nhiên; do đó ta có thể giả sử $\Phi \neq 0$. Gọi $f$ là ánh xạ tuyến tính $d_\Phi$ từ $E$ vào $E^*$ liên kết bên phải với $\Phi$ ($§ 1$, no 1); khi đó $f(E)$ là một môđun con khác không của môđun $E^*$, là một môđun tự do chiều $n$. Gọi $A\alpha_1$ là nhân tử bất biến lớn nhất của $f(E)$ đối với $E^*$ (chap. VII, $§ 4$, no 2, th. 1); ta biết (*loc. cit.*) rằng tồn tại một cơ sở $(e'_1, a'_2, \ldots, a'_n)$ của $E^*$ và một phần tử $f(e_2) \in f(E)$ sao cho $f(e_2) = \alpha_1 e'_1$. Gọi $(e_1, a_2, \ldots, a_n)$ là cơ sở của $E$ (đồng nhất với song đối ngẫu $E^{**}$) đối ngẫu với $(e'_1, a'_2, \ldots, a'_n)$; ta có

$$
\Phi(e_1, e_2) = -\Phi(e_2, e_1) = \langle e_1, f(e_2) \rangle = \alpha_1.
$$

Cho $P$ là môđun con $Ae_1 + Ae_2$ của $E$. Ta sẽ thấy rằng $E$ là *tổng trực tiếp* của $Ae_1, Ae_2$ và môđun con trực giao $P^0$ của $P$. Để làm điều đó, chỉ cần chứng minh rằng, với mọi $x \in E$, tồn tại các phần tử $\xi_1, \xi_2$ của $A$, được xác định duy nhất, sao cho $x - \xi_1 e_1 - \xi_2 e_2 \in P^0$, nghĩa là sao cho

$$
\Phi(e_1, x - \xi_1 e_1 - \xi_2 e_2) = 0, \qquad \Phi(e_2, x - \xi_1 e_1 - \xi_2 e_2) = 0.
$$

Theo (1), các điều kiện này được viết thành

$$
\langle e_1, f(x) \rangle = \xi_2 \alpha_1, \langle e_2, f(x) \rangle = -\xi_1 \alpha_1.
$$

Nhưng ta biết (*loc. cit.*) rằng ảnh của $f(E)$ bởi mọi dạng tuyến tính trên $E^*$ đều được chứa trong iđêan $A\alpha_1$, nói cách khác mọi giá trị $\Phi(x, y) = \langle x, f(y) \rangle$ đều thuộc $A\alpha_1$; do đó có sự tồn tại và tính duy nhất của $\xi_1$ và $\xi_2$. Vậy $P^0$ là một môđun tự do hạng $n-2$; do đó tồn tại, trong $P^0$, theo giả thiết quy nạp, một cơ sở $(e_3, e_4, \ldots, e_n)$ thỏa mãn các điều kiện của mệnh đề. Để chứng minh rằng cơ sở $(e_1, \ldots, e_n)$ của $E$ thu được như vậy cũng thỏa mãn các điều kiện này, chỉ cần chứng minh rằng $\alpha_1$ chia $\alpha_2$; mà điều này suy ra từ việc mọi giá trị $\Phi(x, y)$ đều là bội của $\alpha_1$. Khi đó rõ ràng là $e_{2r+1}, \ldots, e_n$ sinh $E^0$. Sau cùng, nếu $(e'_i)$ là cơ sở đối ngẫu của $(e_i)$, ta có $f(e_{2j-1}) = -\alpha_j e'_{2j}$ và $f(e_{2j}) = \alpha_j e'_{2j}$ với $j = 1, \ldots, r$ và $f(e_k) = 0$ với $k = 2r+1, \ldots, n$; do đó các iđêan $A\alpha_1, A\alpha_1, A\alpha_2, A\alpha_2, \ldots, A\alpha_r, A\alpha_r$ là các nhân tử bất biến của $f(E)$ đối với $E^*$, điều này chứng minh tính duy nhất của chúng (Chương VII, $§ 4$, No. 2, Định lý 1).

#### Hệ quả 1 {#alg-ix-s5-thm-1-cor-1 .statement}

*Cho $A$ là một trường giao hoán, $E$ là một không gian vectơ hữu hạn chiều chiều $n$ trên $A$, và $\Phi$ là một dạng song tuyến tính phản xứng trên E. Khi đó tồn tại một cơ sở $(e_i)_{1 \leq i \leq n}$ của E và một số nguyên chẵn $2r \leq n$ sao cho

$$
\Phi\left( \sum_{i=1}^n \xi_i e_i, \sum_{i=1}^n \eta_i e_i \right) = \sum_{j=1}^r (\xi_{2j-1} \eta_{2j} - \xi_{2j} \eta_{2j-1}).
$$

Đặc biệt $\Phi$ có hạng chẵn $2r$.

Một cơ sở thỏa mãn (2) được gọi là một cơ sở symplectic của $\Phi$.

#### Nhận xét {#alg-ix-s5-n1-rem-1 .statement}

Cần chú ý rằng hệ quả này cũng là một hệ quả ngay lập tức của Mệnh đề 3 của § 4, No. 2 và của Hệ quả 1 của nó, bởi vì với ký hiệu của mệnh đề này, tất yếu có $H = \{0\}$ vì $\Phi$ là phản xứng.

#### Hệ quả 2 {#alg-ix-s5-thm-1-cor-2 .statement}

Cho A là một trường giao hoán, E là một không gian vectơ hữu hạn chiều chiều n trên A. Với mọi bivectơ $z \in \bigwedge^2 E$, tồn tại một cơ sở $(e_i)_{1 \leq i \leq n}$ của E sao cho

$$
z = e_1 \wedge e_2 + e_3 \wedge e_4 + \cdots + e_{2r-1} \wedge e_{2r} \quad (2r \leq n).
$$

Thật vậy, chỉ cần chú ý rằng z đồng nhất một cách chính tắc với một dạng song tuyến tính phản xứng trên $E^*$ (Chương III, § 8, No. 2), và áp dụng Hệ quả 1 cho dạng này.

Bằng cách dịch Hệ quả 1 sang ngôn ngữ ma trận, ta thu được:

#### Hệ quả 3 {#alg-ix-s5-thm-1-cor-3 .statement}

Cho $A$ là một trường giao hoán, $R$ là một ma trận vuông phản xứng trên $A$. Hạng của $R$ là một số chẵn $2r$, và tồn tại một ma trận khả nghịch $P$ trên $A$ sao cho

$$
{}^tP.R.P = \begin{pmatrix}
0 & I_r & 0 \\
-I_r & 0 & 0 \\
0 & 0 & 0
\end{pmatrix}.
$$

#### Nhận xét {#alg-ix-s5-n1-rem-2 .statement}

Nếu $A$ là một vành giao hoán bất kỳ và $R$ là một ma trận vuông phản xứng cấp lẻ n trên $A$, ta có det $R = 0$. Điều này suy ra từ Hệ quả 3 khi $A$ là một trường. Một chứng minh trực tiếp trong trường hợp $A$ là một trường có đặc số $\neq 2$ như sau: vì ${}^tR = -R$, ta có det $R = \det {}^tR = (-1)^n \det R$, do đó $2 \det {}^tR = 0$. Bây giờ, vì định thức của một ma trận phản xứng $(\alpha_{ij})$ là một đa thức với hệ số nguyên theo các $\alpha_{ij}$ sao cho $i < j$, nguyên lý mở rộng các đồng nhất thức đại số (Chương IV, § 2, No. 5, Chú giải) cho thấy khi đó mệnh đề của chúng ta đúng đối với một vành giao hoán tùy ý $A$.

### 2. Pfaffian của một ma trận phản xứng.

Cho $A$ là một trường giao hoán có đặc số 0, và $R = (\alpha_{ij})$ là một ma trận phản xứng bình phương cấp chẵn $2m$ trên $A$. Ký hiệu E là không gian vectơ $A^{2m}$, ký hiệu $(e_i)$ ($i = 1, \ldots, 2m$) là cơ sở chính tắc của nó, và ký hiệu e là phần tử $e_1 \wedge e_2 \wedge \ldots \wedge e_{2m}$ của $\wedge^2 E$. Lũy thừa ngoài thứ $m$ của bivectơ $u = \sum_{i < j} \alpha_{ij} e_i \wedge e_j \in \wedge^2 E$ có dạng $\alpha . e$, trong đó $\alpha$ là một phần tử của $A$ mà ta sẽ tính. Phần tử $\wedge^m u$ là một tổng của các số hạng có dạng
$$
\alpha_{h_1 k_1} \alpha_{h_2 k_2} \cdots \alpha_{h_m k_m} e_{h_1} \wedge e_{k_1} \wedge e_{h_2} \wedge e_{k_2} \wedge \ldots \wedge e_{h_m} \wedge e_{k_m}
$$
với $h_j < k_j$ đối với $j = 1, \ldots, m$. Một số hạng như thế bằng không nếu có hai $e_j$ bằng nhau xuất hiện trong nó, nghĩa là nếu tập hợp $\{ h_1, k_1, \ldots, h_m, k_m \}$ không đúng bằng $\{ 1, 2, \ldots, 2m \}$. Hơn nữa, nếu, trong (3), đồng thời đổi chỗ $e_{h_r}$ và $e_{h_{r+1}}$ một mặt, và $e_{k_r}$ và $e_{k_{r+1}}$ mặt khác, thì tích không thay đổi; do đó nó không thay đổi dưới bất kỳ phép hoán vị nào thực hiện trên các cặp $(h_1, k_1), \ldots, (h_m, k_m)$. Khi đó hãy xét các tập hợp (chứ không phải các dãy) $S = \{ (h_1, k_1), \ldots, (h_m, k_m) \}$ các cặp $(h_j, k_j)$ sao cho $1 \leq h_j < k_j \leq 2m$ đối với $j = 1, 2, \ldots, m$; gọi $\mathcal{S}$ là tập hợp của các cặp ấy. Với $S \in \mathcal{S}$, đặt
1°) $\varepsilon(S) = 0$ nếu $\{ h_1, k_1, \ldots, h_m, k_m \} \neq \{ 1, 2, \ldots, 2m \}$;
2°) trong trường hợp ngược lại, $\varepsilon(S) = 1$ hoặc $\varepsilon(S) = -1$ tùy theo phép hoán vị biến $h_j$ thành $2j-1$ và $k_j$ thành $2j$ ($j = 1, \ldots, m$) là chẵn hay lẻ.

Các nhận xét trên chứng minh rằng khi đó $\wedge^m u$ bằng
$$
m! \sum_{S \in \mathcal{S}} \varepsilon(S) (\prod_{(h, k) \in S} \alpha_{hk}) e.
$$

Khi đó đưa vào $m(2m-1)$ bất định $X_{hk}$ được đánh chỉ số bởi các cặp $(h, k)$ sao cho $1 \leq h < k \leq 2m$, và gọi P là đa thức trên $\mathbf{Z}$ theo các $X_{hk}$, được xác định bởi
$$
P((X_{hk})) = \sum_{S \in \mathcal{S}} \varepsilon(S) (\prod_{(h, k) \in S} X_{hk}).
$$

Do đó ta có

(6) $\bigwedge^m u = m! \mathrm{P}((\alpha_{hk})) . e.$

#### Định nghĩa 1 {#alg-ix-s5-def-1 .statement}

Cho một ma trận phản xứng $R = (\alpha_{ij})$ $(i, j = 1, \ldots, 2m)$ cấp chẵn $2m$ trên một vành giao hoán tùy ý $A$, pfaffian của $R$, ký hiệu là $\mathrm{Pf}(R)$, là phần tử $\mathrm{P}((\alpha_{hk}))$ của $A$, trong đó $1 \leq h < k \leq 2m$.

#### Ví dụ {#alg-ix-s5-n2-exa-1 .statement}

Giả sử:

$\alpha_{12} = -\alpha_{21} = \beta_1, \alpha_{34} = -\alpha_{43} = \beta_2, \ldots, \alpha_{2m-1, 2m} = -\alpha_{2m, 2m-1} = \beta_m,$

tất cả các $\alpha_{ij}$ khác đều bằng không (x. đl. 1). Khi đó pfaffian của $R = (\alpha_{ij})$ là $\beta_1 \beta_2 \ldots \beta_m$.

#### Mệnh đề 1 {#alg-ix-s5-prop-1 .statement}

Cho $R$ là một ma trận phản xứng cấp chẵn $2m$ trên một vành giao hoán $A$, và cho $P$ là một ma trận bình phương cấp $2m$ trên $A$. Ta có

(7) $\mathrm{Pf}({}^t P . R . P) = (\det P) \mathrm{Pf}(R).$

Thật vậy, trước hết giả sử rằng $A$ là một trường đặc số 0 và đặt $R = (\alpha_{ij}), P = (\beta_{st})$. Liên kết với $R$ bivectơ

$$ u = \sum_{i < j} \alpha_{ij} e_i \wedge e_j = \frac{1}{2} \sum_{1 \leq i, j \leq 2m} \alpha_{ij} e_i \wedge e_j $$

của $\bigwedge^2 \mathbf{A}^{2m}$, trong đó $(e_i)$ ký hiệu cơ sở chính tắc của $\mathbf{A}^{2m}$; coi ${}^t P$ là ma trận, đối với cơ sở $(e_i)$, của một tự đồng cấu $f$ của $\mathbf{A}^{2m}$. Khi đó bivectơ $(\bigwedge f)(u)$ liên kết với ma trận ${}^t P . R . P$ vì nó bằng $\frac{1}{2} \sum_{i, j, s, t} \beta_{is} \alpha_{ij} \beta_{jt} e_s \wedge e_t$. Vì phép mở rộng $\bigwedge f$ của $f$ lên đại số ngoài $\bigwedge \mathbf{A}^{2m}$ là một tự đồng cấu của đại số này (ch. III, § 5, số 9), ta có $\bigwedge ((\bigwedge f)(u)) = (\bigwedge f)(\bigwedge u)$; vì $\bigwedge f$ là phép vị tự với tỉ số $\det f$, do đó suy ra từ (6) và đn. 1 rằng ta có $m! \mathrm{Pf}({}^t P . R . P) = m! (\det P) \mathrm{Pf}(R)$, do đó có (7) trong trường hợp đang xét. Trường hợp tổng quát suy ra bằng cách nhận thấy rằng hai vế của (7) là những đa thức với hệ số nguyên theo các phần tử của các ma trận $R$ và $P$ (ch. IV, § 2, số 5, Chú giải).

#### Mệnh đề 2 {#alg-ix-s5-prop-2 .statement}

Với mọi ma trận phản xứng $R$ cấp chẵn $2m$ trên một vành giao hoán $A$, ta có
$$
\det R = (\mathrm{Pf}(R))^2.
$$
Thật vậy, vì hai vế của (8) là những đa thức với hệ số nguyên theo các phần tử của $R$, nguyên lý kéo dài các đồng nhất thức đại số (ch. IV, § 2, No. 5, Scholium) cho thấy rằng chỉ cần cho chứng minh trong trường hợp $A$ là một trường đặc số 0 và $\det R \neq 0$. Nếu $P$ là một ma trận bình phương khả nghịch cấp $2m$ trên $A$, ta có $\det (^tP . R . P) = (\det P)^2 (\det R)$ và $\mathrm{Pf} (^tP . R . P) = (\det P) \mathrm{Pf}(R)$ (mệnh đề 1), nên chỉ cần chứng minh (8) cho $^tP . R . P$ thay vì cho $R$. Theo hệ quả 1 của đl. 1, bằng một lựa chọn thích hợp của $P$, ta có thể giả sử rằng ma trận $^tP . R . P$ có dạng $(\alpha_{ij})$ trong đó
$$
\alpha_{12} = -\alpha_{21} = 1, \ldots, \alpha_{2m-1, 2m} = -\alpha_{2m, 2m-1} = 1,
$$
tất cả các $\alpha_{ij}$ khác đều bằng không (x. Ví dụ). Bây giờ định thức của ma trận này bằng 1, và Pfaffian của nó cũng vậy; điều này hoàn tất chứng minh.

### 3. Nhóm symplectic.

Giả sử vành $A$ là giao hoán. Nếu $\Phi$ là một dạng song tuyến tính phản xứng trên $E$, các tự đẳng cấu của môđun $E$ bảo toàn $\Phi$ được gọi là các *tự đẳng cấu symplectic* (hoặc *phép biến đổi symplectic*) đối với $\Phi$, và chúng tạo thành một nhóm được gọi là *nhóm symplectic* liên kết với $\Phi$; đôi khi nó được ký hiệu bởi $\mathbf{Sp}(\Phi)$.

Xét riêng, trên môđun $E = A^{2m}$, dạng song tuyến tính phản xứng $\Phi_0$ mà ma trận của nó đối với cơ sở chính tắc $(e_i)$ của $E$ là
$$
R_m = \begin{pmatrix} 0 & I_m \\ -I_m & 0 \end{pmatrix}.
$$
Các tự đẳng cấu symplectic và nhóm symplectic đối với $\Phi_0$ được gọi đơn giản là các tự đẳng cấu symplectic và nhóm symplectic *theo $2m$ biến* (trên $A$); nhóm này được ký hiệu bởi $\mathbf{Sp}(2m, A)$ hoặc $\mathbf{Sp}_{2m}(A)$. Mọi ma trận $A$ của một tự đẳng cấu symplectic đối với cơ sở chính tắc $(e)_i$ được gọi là một *ma trận symplectic*. Một ma trận như vậy là khả nghịch, và, theo công thức (48) của § 1, No. 10, thỏa mãn quan hệ

$$(9)$$
$$
{}^tA . R_m . A = R_m.
$$

Ngược lại, nếu một ma trận bình phương $A$ cấp $2m$ trên $A$ thỏa mãn (9), thì nó là symplectic: quả thật chỉ cần chứng minh rằng nó khả nghịch; mà (9) kéo theo $\mathrm{Pf}(R_m) = \mathrm{Pf}({}^tA . R_m . A) = (\det A) \mathrm{Pf}(R_m)$ theo mệnh đề 1 của No. 2, do đó $\det A = 1$. Đồng thời ta đã chứng minh mệnh đề sau:

#### Mệnh đề 3 {#alg-ix-s5-prop-3 .statement}

*Định thức của một ma trận symplectic bằng 1.*

Nếu $A$ là một trường giao hoán và $\Phi$ là một dạng song tuyến tính phản xứng không suy biến trên một không gian vectơ $E$ có chiều chẵn $2m$ trên $A$, thì nhóm symplectic liên kết với $\Phi$ là *đẳng cấu* với $\mathbf{Sp}(2m, A)$, theo hệ quả 1 của định lý 1.

*Bài tập.* — ¶ 1) Cho $A$ là một vành chính giao hoán, $E$ là một A-môđun tự do có số chiều hữu hạn $n$, $\Phi$ là một dạng song tuyến tính phản xứng trên $E$; các iđêan $A \alpha_i$ ($1 \leq i \leq r$) được xác định trong Định lý 1 của No. 1 được gọi là các *nhân tử bất biến* của $\Phi$.

a) Cho $F$ là một môđun con của $E$, và gọi $\Phi_F$ là hạn chế của $\Phi$ trên $F \times F$. Chứng minh rằng nếu $A \beta_i$ ($1 \leq i \leq s$) là các nhân tử bất biến của $\Phi_F$ (trong đó $\beta_i$ chia $\beta_{i+1}$), thì $s \leq r$ và $\beta_i$ là một bội của $\alpha_i$ với $1 \leq i \leq s$. (Rút gọn về trường hợp $r = s = n/2$, và dùng Bài tập 9 b) và 9 c) của Chương VII, § 4).

b) Cho $E_1$ là một $A$-môđun tự do thứ hai có số chiều hữu hạn, $\Phi_1$ là một dạng song tuyến tính phản xứng trên $E_1$, $A \gamma_1, \ldots, A \gamma_s$ là các ước số bất biến của nó ($\gamma_i$ chia $\gamma_{i+1}$). Để $\Phi_1$ là ảnh ngược của $\Phi$ bởi một ánh xạ tuyến tính từ $E_1$ vào $E$, điều kiện cần và đủ là $s \leq r$ và $\gamma_i$ là một bội của $\alpha_i$ với $1 \leq i \leq s$. (Dùng a) và Mệnh đề 4 của Chương VII, § 4, No. 5).

c) Cho $F, G$ là hai môđun con của $E$, sao cho $F^0$ (tương ứng $G^0$) bù cho $F$ (tương ứng $G$) trong $E$. Nếu các hạn chế của $\Phi$ lên $F$ và $G$ là tương đương, hãy chỉ ra rằng điều tương tự cũng đúng đối với các hạn chế của $\Phi$ lên $F^0$ và lên $G^0$, và rằng tồn tại một tự đẳng cấu của $E$ bảo toàn $\Phi$ và biến đổi $F$ thành $G$.

d) Hãy cho một ví dụ về hai môđun con $F, G$ của $E$, có chiều bằng 2, sao cho $F$ và $G$ thừa nhận các phần bù trong $E$ và sao cho các hạn chế $\Phi_F$ và $\Phi_G$ là tương đương, nhưng không tồn tại tự đẳng cấu nào của $E$ bảo toàn $\Phi$ và biến đổi $F$ thành $G$ (lấy $n = 4$).

2) Cho $\Phi$ là một dạng song tuyến tính phản xứng trên một không gian vectơ hữu hạn chiều $E$. Hãy chỉ ra rằng với mọi không gian con vectơ $M$ của $E$, hiệu dim M – dim (M ∩ M^0) là chẵn. (Trước hết hãy xét trường hợp $\Phi$ không suy biến).

¶ 3) Cho E là một không gian vectơ có chiều chẵn n = 2m trên một trường giao hoán A; cho $\Phi$ và $\Psi$ là hai dạng song tuyến tính phản xứng trên E; giả sử rằng $\Psi$ không suy biến. Cho u và v là các ánh xạ tuyến tính từ E vào E* liên kết bên phải tương ứng với $\Phi$ và $\Psi$; v là một đẳng cấu từ E lên E*; đặt $\omega = v^{-1} \circ u$, khi đó $\omega$ là một tự đồng cấu của E.

a) Đặt $M_0 = E$, và, xác định đệ quy, $M_{k+1} = \omega(M_k)$ với $k > 0$. Hãy chỉ ra rằng nếu $M'_k$ là không gian con trực giao với $M_k$ đối với $\Phi$, thì $M_{k+1}$ là không gian con trực giao với $M'_k$ đối với $\Psi$.

b) Gọi n_0 là chiều của M'_0; đặt m_0 = 0, và với k ≥ 1, ký hiệu bởi m_k chiều của M_k ∩ M'_0. Hãy chỉ ra rằng với k ≥ 1 chiều của M_k là n − n_0 − (m_1 + ... + m_{k−1}) và chiều của M'_k là n_0 + (m_1 + ... + m_k).

c) Hãy chỉ ra rằng, với mọi k ≥ 0, chiều của M_k ∩ M'_k là m_k + m_{k+1} + ... + m_{2k}, và chiều của M'_k ∩ M_{k+1} là m_{k+1} + m_{k+2} + ... + m_{2k+1} (áp dụng Bài tập 2 b) của § 3 để tính các chiều của M_h ∩ M'_{2k−h} và của M'_h ∩ M_{2k+1−h} bằng quy nạp theo h).

d) Suy ra từ c) rằng các số m_k là chẵn (dùng Bài tập 2).

e) Kết luận từ d) rằng số các ước số sơ cấp của tự đồng cấu ω, tương ứng với nghiệm đặc số λ = 0, và có một bậc cho trước, là chẵn (xem Chương VII, § 5, Bài tập 20).

4) Cho E là một không gian vectơ trên một trường giao hoán A, thừa nhận một cơ sở đếm được $(e_n)_{n≥1}$, và cho $\Phi$ là một dạng phản xứng không suy biến trên E. Hãy chỉ ra rằng tồn tại trong E một cơ sở $(a_n)$ sao cho Φ(a_{2n−1}, a_{2n}) = 1 với mọi n ≥ 1, và Φ(a_i, a_j) = 0 với mọi cặp chỉ số khác sao cho i < j (lập luận như trong Bài tập 13 của § 4).

5) Với mọi ma trận phản xứng X = (x_{ij}) có cấp chẵn n = 2m trên một vành giao hoán, và với mọi chỉ số i, hãy chỉ ra rằng ta có
$$
\mathrm{Pf}(X) = \sum_{j=1}^{n} (-1)^{i+j-1} \mathrm{Pf}(X_{ij}) x_{ij},
$$
trong đó X_{ij} là ma trận cấp n − 2 thu được bằng cách xóa khỏi X các hàng và các cột có chỉ số i và j.

6) Cho M là một ma trận vuông cấp m trên một vành giao hoán. Hãy chỉ ra rằng nếu đặt
$$
R = \begin{pmatrix}
0 & M \\
-^t M & 0
\end{pmatrix}
$$
thì ta có Pf(R) = det M (trước hết hãy chứng minh điều này khi M khả nghịch, dùng công thức (7)).

7) Cho A là một trường giao hoán, $\mathfrak{A}(A)$ tập hợp các ma trận phản xứng cấp 2m trên A; cho I là một ánh xạ từ $\mathfrak{A}(A)$ vào A sao cho với mọi ma trận R ∈ $\mathfrak{A}(A)$ và mọi ma trận P cấp 2m trên A, ta có I(^tPRP) = (det P)^h I(R), trong đó h là một số nguyên hữu tỉ. Hãy chỉ ra rằng I(R) = c(PfR)^h, trong đó c ∈ A (dùng công thức (7) và Định lý 1 của No. 1).

8) Cho P, Q là hai ma trận vuông phản xứng cấp chẵn 2m trên một vành giao hoán A. Đặt φ(X) = Pf(P − XQ); hãy chỉ ra rằng, nếu Q khả nghịch, thì ta có $\varphi(Q^{-1}P) = 0$. (Trước hết xét trường hợp A là một trường; sau đó suy ra từ Bài tập 3 rằng đa thức tối tiểu của ma trận $Q^{-1}P$ chia hết $\varphi(X)$, bằng cách chuyển qua một mở rộng đóng đại số của A, và nhận thấy rằng $\varphi^2$ là đa thức đặc trưng của $Q^{-1}P$ sai khác bởi một nhân tử vô hướng).

§ 9) Cho E là một không gian vectơ chiều $n$ trên một trường giao hoán A, $\Phi$ là một dạng song tuyến tính phản xứng trên E, $\Psi$ là một dạng nửa tuyến tính Hermit (đối với một tự đẳng cấu đối hợp của A) trên E, P và Q là các ma trận tương ứng của $\Phi$ và $\Psi$ đối với cùng một cơ sở của E.

a) Giả sử rằng $\Psi$ không suy biến. Hãy chỉ ra rằng số các ước sơ cấp của $Q^{-1}P$ tương ứng với nghiệm đặc trưng 0 và có cùng bậc chẵn là một số chẵn (phương pháp của Bài tập 3).

b) Giả sử rằng $\Phi$ không suy biến (điều đó kéo theo $n$ là chẵn). Hãy chỉ ra rằng số các ước sơ cấp của $P^{-1}Q$ tương ứng với nghiệm đặc trưng 0, và có cùng bậc lẻ, là một số chẵn (cùng phương pháp).

10) Cho $\omega_{2m}(\mathbf{F}_q)$ là cấp của nhóm đối xứng $\mathbf{Sp}(2m, \mathbf{F}_q)$ trên trường hữu hạn $\mathbf{F}_q$. Hãy chỉ ra rằng nếu $h_{2m}$ là số các cặp vectơ $(x, y)$ của $\mathbf{F}_q^{2m}$ sao cho $\Phi_0(x, y) = 1$ (các ký hiệu của No. 3), thì ta có $\omega_{2m}(\mathbf{F}_q) = h_{2m}\omega_{2m-2}(\mathbf{F}_q)$; suy ra

$$
\omega_{2m}(\mathbf{F}_q) = (q^{2m} - 1)q^{2m-1}(q^{2m-2} - 1)q^{2m-3} \ldots (q^2 - 1)q.
$$

11) Cho A là một trường giao hoán. Hãy chỉ ra rằng mọi phép biến đổi $u$ thuộc nhóm đối xứng $\mathbf{Sp}(2m, A)$ đều là một tích các phép chuyển vị thuộc nhóm này (gọi là các phép chuyển vị đối xứng; xem § 4, Bài tập 6). (Lập luận bằng quy nạp theo $m$, bằng cách chỉ ra rằng nếu $x, y$ là hai vectơ không trực giao của $E = A^{2m}$, thì tồn tại một tích $v$ các phép chuyển vị đối xứng sao cho $vu$ giữ bất biến $x$ và $y$.) Suy ra một chứng minh mới của Mệnh đề 3 của No. 3.

*12) Cho A là một trường giao hoán, E một không gian vectơ chiều chẵn $n = 2m$ trên A, $\Phi$ một dạng song tuyến tính phản xứng không suy biến trên E. Bây giờ chứng minh rằng, với mọi phép đồng dạng $u$ của dạng $\Phi$ ($§ 6$, no 5), với nhân tử $\alpha$, ta có $\det u = \alpha^m$ (dùng công thức (7)).*

§ 13) Ta giả sử rằng A là một trường giao hoán có đặc số 0, E là một không gian vectơ chiều $2m$ trên A, $\Phi$ là một dạng song tuyến tính phản xứng không suy biến trên E. Ta đồng nhất dạng nghịch đảo $\widehat{\Phi}$ của $\Phi$ với một song vectơ $\Gamma \in \bigwedge^2 E$, theo cách sao cho với mọi cơ sở đối xứng $(e_i)_{1 \leq i \leq 2m}$ của E (đối với $\Phi$), được đánh chỉ số sao cho $\Phi(e_i, e_j) = \Phi(e_{m+i}, e_{m+j}) = 0$, $\Phi(e_i, e_{m+j}) = \delta_{ij}$ ($1 \leq i \leq m, 1 \leq j \leq m$), ta có

$$
\Gamma = e_1 \wedge e_{m+1} + e_2 \wedge e_{m+2} + \cdots + e_m \wedge e_{2m}.
$$

Ta nói rằng một $p$-vectơ phân tích được và khác không $z \in \bigwedge^p E$ là đẳng hướng (tương ứng, hoàn toàn đẳng hướng) đối với $\Phi$, nếu không gian con vectơ tương ứng $V_z$ (chap. III, § 7, no 3) là đẳng hướng (tương ứng, hoàn toàn đẳng hướng).

a) Nếu $z$ là một $p$-vectơ phân tích được $\neq 0$, $2r$ là chiều của một phần bù của $V_z \cap V_z^0$ đối với $V_z$, bây giờ chứng minh rằng $m - p + r$ là số nguyên $h$ lớn nhất sao cho $z \wedge \Gamma^h \neq 0$, ký hiệu $\Gamma^h$ là lũy thừa thứ $h$ của $\Gamma$ trong đại số ngoài $\wedge E$ (dùng mệnh đề 2 của § 4, n° 2).

b) Bây giờ chứng minh rằng mọi lưỡng vectơ $x \in \overset{2}{\wedge} E$ đều có thể viết dưới dạng $\lambda \Gamma + x_1$, trong đó $\lambda$ là một vô hướng và $x_1$ là một tổ hợp tuyến tính của các lưỡng vectơ hoàn toàn đẳng hướng phân tích được. (Rút gọn về trường hợp $x$ là phân tích được, và nhận thấy rằng nếu $(e_i)$ là một cơ sở symplectic, thì $(e_1 + e_2) \wedge (e_{m+1} - e_{m+2})$ là hoàn toàn đẳng hướng).

c) Nếu $p \leq m$, bây giờ chứng minh rằng mọi $p$-vectơ $z \in \overset{p}{\wedge} E$ đều có thể viết thành $z = x \wedge \Gamma + z_1$, trong đó $x$ là một $(p-2)$-vectơ và $z_1$ là một tổ hợp tuyến tính của các $p$-vectơ hoàn toàn đẳng hướng phân tích được. (Rút gọn về trường hợp $z$ là phân tích được, và lập luận bằng quy nạp theo $p$. Như thế rút gọn về trường hợp mà, với $(e_i)$ là một cơ sở symplectic, ta có $z = e_1 \wedge e_2 \wedge \ldots \wedge e_{p-1} \wedge e_{m+p-1}$, và xét các lưỡng vectơ $(e_{p-1} + e_{p+i}) \wedge (e_{m+p-1} - e_{m+p+i})$ với $0 \leq i \leq m-p$.

d) Với $1 \leq p \leq m$, bây giờ chứng minh rằng mọi $(m+p)$-vectơ $z \in \overset{m+p}{\wedge} E$ đều có thể viết thành $z = y \wedge \Gamma^p$, trong đó $y$ là một $(m-p)$-vectơ. (Rút gọn về trường hợp $z$ là phân tích được; nếu $2r$ là chiều của một phần bù của $V_z \cap V_z^0$ đối với $V_z$, hãy phân biệt hai trường hợp tùy theo $r = p$ hay $r > p$; trong trường hợp thứ hai, lập luận bằng quy nạp theo $r$, theo cùng cách như trong c)). Suy ra rằng ánh xạ $y \to y \wedge \Gamma^p$ của $\overset{m+p}{\wedge} E$ vào $\overset{m+p}{\wedge} E$ là song ánh (nhận thấy rằng hai không gian có cùng chiều). Nếu $y$ là một $(m-p)$-vectơ phân tích được, hãy chỉ ra rằng $z = y \wedge \Gamma^p$ là phân tích được và rằng $V_z = V_y^0$.

e) Suy ra từ d) rằng, với $p \leq m$, không gian con $\overset{p}{\wedge} E$ là tổng trực tiếp của thành phần thuần nhất bậc $p$ của iđêan hai phía $c$ sinh bởi $\Gamma$ trong $\wedge E$, và của không gian con $R_p$ gồm các vectơ $p$ $z_1$ sao cho $z_1 \wedge \Gamma^{m-p+1} = 0$ (với $z \in \overset{p}{\wedge} E$, áp dụng d) cho vectơ $(2m-p+2)$ $z \wedge \Gamma^{m-p+1}$). Dùng c), chứng minh rằng $R_p$ được sinh bởi các vectơ $p$ phân tích được hoàn toàn đẳng hướng, và dùng d), hãy chỉ ra rằng ánh xạ $x \to x \wedge \Gamma$ từ $\overset{p-2}{\wedge} E$ vào $\overset{p}{\wedge} E$ là đơn ánh, và rằng $R_p$ có chiều $\binom{2m}{p} - \binom{2m}{p-2}$.

f) Bây giờ chứng minh rằng nếu $p \leq m$, một điều kiện cần và đủ để một vectơ $p$ $z$ có dạng $x \wedge \Gamma$ là với mọi vectơ $m$ phân tích được hoàn toàn đẳng hướng $u$, ta có $z \wedge u = 0$. (Bây giờ chứng minh rằng, nếu điều kiện này được thỏa mãn, và nếu $z \in R_p$, thì ta có $z \wedge y = 0$ với mọi vectơ $(2m-p)$ $y$; viết $y$ dưới dạng $x \wedge \Gamma^{m-p}$, trong đó $x$ là một vectơ $p$, rồi áp dụng c) cho $x$, và nhận thấy rằng, nếu $x_1$ là một vectơ $p$ phân tích được hoàn toàn đẳng hướng, thì $x_1 \wedge \Gamma^{m-p}$ là một vectơ $(2m-p)$ phân tích được, có thể viết thành $u_1 \wedge v_1$, trong đó $u_1$ là một vectơ $m$ phân tích được hoàn toàn đẳng hướng).

Gọi $\alpha$ là linh hóa tử của iđêan $c$ trong $\wedge E$; $\alpha$ là tổng trực tiếp của các không gian con $R_m, R_{m-1} \wedge \Gamma, \ldots, R_1 \wedge \Gamma^{m-1}$ và $K \Gamma^m$. Bây giờ chứng minh rằng linh hóa tử của $\alpha$ trong $\wedge E$ bằng $c$ (x. § 2, exerc. 4 b)).

g) Với mọi tự đẳng cấu symplectic $u$ của $E$ (đối với $\Phi$), gọi $\bar{u}$ là phép mở rộng chính tắc của $u$ thành một tự đẳng cấu của đại số $\wedge E$ (chương III, § 5, số 9). Bây giờ chứng minh rằng các phần tử duy nhất của $\wedge E$ bất biến dưới mọi tự đẳng cấu $\bar{u}$ là các tổ hợp tuyến tính của $1, \Gamma, \Gamma^2, \ldots, \Gamma^m$ với các hệ số trong $K$. (Nếu $(e_i)$ là một cơ sở symplectic, hãy viết rằng một phần tử của $\wedge E$ là bất biến dưới các phép đối xứng transvection symplectic (bài tập 11) tương ứng với các siêu phẳng trực giao với các $e_i$; rồi xét các phép biến đổi symplectic $u_{ij}$ được xác định bởi $u_{ij}(e_i) = e_j, u_{ij}(e_j) = e_i, u_{ij}(e_{m+i}) = e_{m+j}, u_{ij}(e_{m+j}) = e_{m+i}, u_{ij}(e_k) = e_k$ với mọi chỉ số khác $k$).

14) Cho $A$ là một trường giao hoán có đặc số 2, $E$ là không gian vectơ $A^{2m}$; ta đồng nhất nhóm symplectic $Sp(2m, A)$ với nhóm các ma trận symplectic $U$, do đó thỏa mãn quan hệ $^tU . R . U = R$, trong đó $R = \begin{pmatrix} 0 & I_m \\ I_m & 0 \end{pmatrix}$. Đặt $D = \begin{pmatrix} 0 & 0 \\ I_m & 0 \end{pmatrix}$; bây giờ chứng minh rằng mọi ma trận symplectic $U$ sao cho $I + U$ khả nghịch đều có thể viết được theo một và chỉ một cách dưới dạng $(^tD + S)^{-1}(D + S)$, trong đó $S$ là một ma trận đối xứng sao cho $D + S$ khả nghịch, và ngược lại (xem § 4, bài tập 11).

15) Cho $A$ là một trường giao hoán, $E$ là một không gian vectơ chiều $2m$ trên $A$, $\Phi$ là một dạng song tuyến tính phản xứng không suy biến trên $E$.
a) Mở rộng cho các nội tự đồng cấu $u$ của $E$ sao cho $u^*u = uu^*$ ($u^*$ là liên hợp của $u$ đối với $\Phi$) các kết quả của § 4, bài tập 12 a) và b).

b) Giả sử rằng $u^* = u$. Với các ký hiệu của bài tập 12 của § 4, hãy chỉ ra rằng nếu $M$ là một phần tử cực tiểu của tập hợp $\mathfrak{M}$ các không gian con không đẳng hướng được chứa trong $G(p, p)$ và ổn định dưới $u$, thì hoặc $M$ là một môđun con không phân tích được của $E_u$, hoặc nó là tổng trực tiếp của hai môđun con như thế đẳng cấu với nhau (lập luận như trong bài tập 12 c) của § 4). Hãy cho các ví dụ (với $p(X) = X - 1$) chỉ ra rằng cả hai trường hợp đều có thể xảy ra.

c) Giả sử $u^* = -u$, với $A$ không có đặc số 2. Với các ký hiệu như trên, gọi $p^h$ là đa thức tối tiểu của hạn chế của $u$ lên $M$, và gọi $d$ là bậc của $p$. Hãy chứng minh rằng nếu $d(h-1)$ là lẻ thì $M$ là một môđun con không phân tích được của $E_u$; trái lại, nếu $d(h-1)$ là chẵn thì $M$ hoặc là không phân tích được, hoặc là tổng trực tiếp của hai môđun con không phân tích được đẳng cấu.

d) Giả sử $u^*u = 1$ (nói cách khác, $u \in Sp(\Phi)$). Với các ký hiệu như trong c), nếu $p(X)$ không chia hết $X^{d(h-1)} - 1$, hoặc nếu $p(X) = X - 1$ và $(-1)^h \neq -1$, thì $M$ là một môđun con không phân tích được của $E_u$; nếu không, $M$ hoặc là không phân tích được, hoặc là tổng trực tiếp của hai môđun con không phân tích được đẳng cấu.
