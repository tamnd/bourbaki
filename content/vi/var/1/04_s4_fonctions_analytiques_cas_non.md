---
book: var
book_title: Variétés différentielles et analytiques
chapter: "1"
chapter_title: VARIÉTÉS DIFFÉRENTIELLES ET ANALYTIQUES, FASCICULE DE RÉSULTATS
section: 4
section_title: Fonctions analytiques (cas non archimédien)
lang: vi
source: var-fr
pdf_pages: 0029-0032
extraction: ocr
subsections:
    - "no": 1
      title: Séries convergentes
      page: 0
      pdf_page: 29
    - "no": 2
      title: Fonctions analytiques
      page: 0
      pdf_page: 31
    - "no": 3
      title: Quelques inégalités
      page: 0
      pdf_page: 32
statements: 0
exercises: 0
content_sha256: 47ef3c81955fc3407200505f234933c542a220eb5aa6087cc0890124040cb0e1
translated_from: content/en-mt/var/1/04_s4_fonctions_analytiques_cas_non.md
source_lang: en-mt
translation_method: machine
source_content_sha256: 80985f908999f00f998e02079336ec6d5e99b09bf471da981e8d65cac53291cf
translation_model: gpt-5.4
translation_run: translate-vi-7b2a232f
glossary_version: 34
glossary_terms_sha256: cc274e34975f6bee7ca35859d0238006247e7a439484cd9fbdc49ad983b1d30a
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 4. Hàm giải tích (trường hợp siêu mêtric)

Trong số này, giả thiết rằng giá trị tuyệt đối của K là siêu mêtric. Ta ký hiệu bởi $(E_i)_{1 \leq i \leq n}$ một họ hữu hạn các không gian định chuẩn trên K, và bởi E không gian tích của các $E_i$, được trang bị chuẩn:

$$
\|x\| = \sup \|x_i\| \quad \text{nếu } x = (x_i).
$$

Ta ký hiệu bởi F một không gian đa định chuẩn tách trên K.

### 4.1. Chuỗi hội tụ

4.1.1. Cho $f = \sum_a f_a$ là một chuỗi hình thức thuộc $\hat{P}(E_1, \ldots, E_n; F)$, (x. Phụ lục). Nếu $\gamma$ là một nửa chuẩn liên tục trên F, và $R = (R_i)$ là một hệ gồm $n$ số thực $> 0$, ta đặt

$$
\|f\|_{\gamma, R} = \sup_a \|f_a\|_\gamma R^\alpha.
$$

Các định nghĩa và kết quả của No. 3.1.1 (đoạn thứ hai) và No. 3.1.2 áp dụng không thay đổi; đặc biệt, ta định nghĩa các không gian

$$
\mathcal{H}_R(E_1, \ldots, E_n; F) \quad \text{và} \quad \mathcal{H}(E_1, \ldots, E_n; F).
$$

4.1.2. Đẳng cấu chính tắc $j$ của $\hat{P}(E; F)$ lên $\hat{P}(E_1, \ldots, E_n; F)$, bằng hạn chế, cho một đẳng cấu của các không gian vectơ tôpô từ $\mathcal{H}_R(E; F)$ lên $\mathcal{H}_{(R, \ldots, R)}(E_1, \ldots, E_n; F)$ với mọi $R \in \mathbf{R}_+^*$; nó cũng cho một đẳng cấu từ $\mathcal{H}(E; F)$ lên $\mathcal{H}(E_1, \ldots, E_n; F)$. Chính xác hơn, nếu $f = \sum_m f_m \in \hat{P}(E; F)$ và nếu $j(f) = \sum_a f_a$, thì với mọi nửa chuẩn liên tục $\gamma$ trên F, ta có:

$$
\|f_m\|_\gamma = \sup_{|\alpha|=m} \|f_\alpha\|_\gamma
$$
$$
\|f\|_{\gamma, R} = \|j(f)\|_{\gamma, (R, \ldots, R)}.
$$

4.1.3. Cho $f = \sum_a f_a$ là một phần tử của $\mathcal{H}(E_1, \ldots, E_n; F)$; gọi $I(f)$ là tập hợp các $R \in (\mathbf{R}_+^*)^n$ sao cho, với mọi nửa chuẩn liên tục $\gamma$ trên F, tích $\|f_\alpha\|_\gamma R^\alpha$ tiến tới không khi $|\alpha|$ tiến tới vô hạn. Tập hợp $I(f)$ là khác rỗng; nó được gọi là chỉ dấu hội tụ ngặt của $f$. Tập hợp $\Omega(f)$ của các điểm

$$(\log R_1, \ldots, \log R_n) \quad \text{với } R \in I(f)$$

là một tập con lồi của $\mathbf{R}^n$.

Khi $n = 1$, tập hợp $I(f)$ là một khoảng của $\mathbf{R}$, mở bên trái và mở hoặc đóng bên phải; cận trên của nó (hữu hạn hoặc $+\infty$) được ký hiệu bởi $\rho(f)$ và được gọi là *bán kính hội tụ ngặt* của $f$.

Với ký hiệu của 4.1.2, ta có $R \in I(f)$ khi và chỉ khi
$$
(R, \ldots, R) \in I(j(f)).
$$
Tập hợp các điểm $x = (x_i)$ sao cho tồn tại $R = (R_i) \in I(f)$ với $\|x_i\| \leq R_i$ đối với $1 \leq i \leq n$ được gọi là *miền hội tụ ngặt* của $f$ và được ký hiệu bởi $C(f)$. Nó là một tập con mở của $E$, hợp của các đa cầu
$$
B(R) = \{ x \in E \mid \|x_i\| \leq R_i \text{ với } 1 \leq i \leq n \},
$$
với $R \in I(f)$.

4.1.4. Các kết quả của 3.1.7 và 3.1.8 vẫn còn khớp, nếu thay thế ở mọi chỗ $\tilde{C}(f)$ bởi $C(f)$ và $\tilde{\mathcal{H}}_R$ bởi $\mathcal{H}_R$.

4.1.5. Cho $F_1, \ldots, F_m$ là các không gian chuẩn đầy đủ và giả sử rằng $F$ là giả đầy đủ. Cho $f = (f_i)_{1 \leq i \leq m}$, với $f_i \in \mathcal{H}(E_1, \ldots, E_n; F_i)$ và cho $g \in \mathcal{H}(F_1, \ldots, F_m; F)$, sao cho điểm $(f_i(0))_{1 \leq i \leq m}$ của $E$ thuộc miền hội tụ ngặt của $g$. Khi đó, với mọi $\alpha \in \mathbf{N}^m$, chuỗi hình thức $g_\alpha \circ f$ thuộc $\mathcal{H}(E_1, \ldots, E_n; F)$ và họ các $g_\alpha \circ f$ là khả tổng trong $\mathcal{H}(E_1, \ldots, E_n; F)$ (do đó *a fortiori* trong $\hat{P}(E_1, \ldots, E_n; F)$). Tổng của nó sẽ được ký hiệu là $g \circ f$.

Chính xác hơn, tồn tại $R \in \bigcap_i I(f_i)$ và $R' \in I(g)$ sao cho
$$
\sup_{|\alpha| > 0} \|f_{i,\alpha}\| R^\alpha < R'_i \quad (\text{với } 1 \leq i \leq m).
$$
Dưới các điều kiện này, các chuỗi hình thức $g_\alpha \circ f$ thuộc $\mathcal{H}_R(E_1, \ldots, E_n; F)$ và họ các $g_\alpha \circ f$ là khả tổng trong $\mathcal{H}_R(E_1, \ldots, E_n; F)$. Cuối cùng, nếu $x \in B(R)$, thì $f(x) = (f_i(x))$ thuộc $C(g)$ và ta có:
$$
g(f(x)) = (g \circ f)(x).
$$

Giả sử hơn nữa rằng, với mỗi $i$, tồn tại một họ $(e_j^i)$ các phần tử của $E_i$ sao cho mọi phần tử $x$ của $E_i$ là tổng của một họ khả tổng $(\lambda_j e_j^i)$ (với $\lambda_j \in K$) sao cho $\|x\| = \sup_j |\lambda_j|$. Khi đó trong đoạn trước có thể thay thế điều kiện $\sup_{|\alpha| > 0} \|f_{i,\alpha}\| R^\alpha < R'_i$ bằng điều kiện $\|f_i\|_R \leq R'_i$.

4.1.6. Giả sử rằng $E_i = K$ với $1 \leq i \leq n$. Khi đó không gian $\hat{P}(K^n; F)$ được đồng nhất với không gian các chuỗi hình thức theo $n$ bất định $X_1, \ldots, X_n$ với hệ số trong $F$ và một phần tử $f$ của $\hat{P}(K^n; F)$ được viết:
$$
f = \sum_a X^a c_a \quad \text{với } c_a \in F.
$$
Nếu $R \in (\mathbf{R}_+^*)^n$ và nếu $\gamma$ là một nửa chuẩn liên tục trên $F$, ta có:
$$
\|f\|_{\gamma, R} = \sup \|c_a\|_\gamma \cdot R^\alpha.
$$

Đoạn cuối của 3.1.10 vẫn còn đúng, cũng như 3.1.11.

4.1.7. Giả sử rằng K là một trường con đóng của một trường định giá đầy đủ (tất yếu siêu mêtric) L. Với $y \in E_i \otimes_K L$, đặt:

$$
\|y\| = \inf_k (\sup |a_k| \cdot \|x_k\|)
$$

cận dưới lớn nhất được lấy trên mọi họ hữu hạn các cặp $(x_k, a_k) \in E_i \times L$ sao cho $y = \sum_k x_k \otimes a_k$. Như vậy ta thu được một chuẩn trên không gian vectơ L $E_i \otimes_K L$, chuẩn này cảm sinh trên $E_i$ chuẩn đã cho. Phần bù đầy đủ của $E_i \otimes_K L$ đối với chuẩn này được ký hiệu là $E_i^L$.

Bây giờ cho F là một không gian vectơ trên L đa chuẩn tách biệt đầy đủ. Với mọi đa thức K-liên tục $f_\alpha$, thuần nhất bậc đa chỉ số $\alpha$, trên $E_1 \times \cdots \times E_n$, nhận giá trị trong không gian vectơ trên K đa chuẩn nền $F_K$ của F, tồn tại duy nhất một đa thức L-liên tục $\tilde{f}_\alpha$, thuần nhất cùng bậc đa chỉ số, trên $E_1^L \times \cdots \times E_n^L$, nhận giá trị trong F, mở rộng $f_\alpha$. Với mọi nửa chuẩn liên tục trên không gian vectơ trên L F, ta có

$$
\|\tilde{f}_\alpha\|_i = \|f_\alpha\|_i.
$$

Nếu $f = \sum f_\alpha \in \mathcal{H}(E_1, \ldots, E_n; F_K)$, thì $\tilde{f} = \sum \tilde{f}_\alpha \in \mathcal{H}(E_1^L, \ldots, E_n^L; F)$.

Chuỗi $f$ và $\tilde{f}$ có cùng chỉ báo hội tụ ngặt (và cùng bán kính hội tụ ngặt khi $n = 1$).

Ngược lại, cho L là một trường con đóng không rời rạc của K và cho $E_i^0$ và $F^0$ là các không gian trên L thu được bằng cách hạn chế các vô hướng từ các $E_i$ và F. Nếu $f = \sum f_\alpha \in \mathcal{H}(E_1, \ldots, E_n; F)$, thì $f_\alpha \in P_\alpha(E_1^0, \ldots, E_n^0; F^0)$; nếu đặt $f^0 = \sum \tilde{f}_\alpha \in \hat{P}(E_1^0, \ldots, E_n^0; F^0)$, thì $f^0 \in \mathcal{H}(E_1^0, \ldots, E_n^0; F^0)$.

Ta có $C(f) \subset C(f^0)$ và $f(x) = f^0(x)$ với mọi $x \in C(f)$.

### 4.2. Các hàm giải tích

4.2.1. Các định nghĩa và kết quả của 3.2.1 và 3.2.2 vẫn đúng không thay đổi.

4.2.2. Với các ký hiệu của 3.2.2, chỉ báo hội tụ ngặt của khai triển chuỗi lũy thừa của $\Delta^a f$ tại một điểm $a$ của U chứa chỉ báo hội tụ ngặt của khai triển chuỗi lũy thừa của $f$ tại $a$.

4.2.3. Các kết quả của 3.2.4, 3.2.5, 3.2.7, 3.2.8 và 3.2.11 vẫn còn nguyên vẹn. Kết quả của 3.2.6 cũng vậy, với điều kiện thêm rằng K được giả thiết có đặc số không.

4.2.4. Giả sử F là gần đầy đủ và cho $f \in \mathcal{H}(E_1, \ldots, E_n; F)$. Ánh xạ $x \mapsto f(x)$ là giải tích trên $C(f)$. Với mọi $a \in C(f)$, chỉ báo hội tụ của khai triển chuỗi lũy thừa của $f$ tại $a$ bằng chỉ báo hội tụ của $f$.

### 4.3. Một vài bất đẳng thức

4.3.1. Giả thiết rằng K thỏa mãn ít nhất một trong các điều kiện sau:
(a) trường thặng dư của K là vô hạn ;
(b) ảnh của K bởi ánh xạ $a \mapsto |a|$ là trù mật trong $\mathbf{R}_+$. (Nói cách khác, giả thiết rằng K không địa phương compact).
Cho $f = \sum_\alpha f_\alpha \in \mathcal{H}(E_1, \ldots, E_n; F)$ và cho $R \in I(f)$. Ta có:
$$
\sup_{x \in B(R)} \|f(x)\|_y = \sup_\alpha \sup_{x \in B(R)} \|f_\alpha(x)\|_y
$$
với mọi nửa chuẩn liên tục $\gamma$ trên F (“các bất đẳng thức Cauchy”).

4.3.2. Tồn tại một hằng số $a > 0$ sao cho với mọi đa thức thuần nhất liên tục $f_\alpha \in P_\alpha(E_1, \ldots, E_n; F)$ và mọi $R \in (\mathbf{R}_+^*)^n$, ta có:
$$
a^{|\alpha|} R^{\alpha} |\alpha|! \|f_\alpha\|_y \leq \sup_{x \in B(R)} \|f_\alpha(x)\|_y \leq \|f_\alpha\|_y R^\alpha
$$
với mọi nửa chuẩn liên tục $\gamma$ trên F. Nếu K thỏa mãn điều kiện (b) của 4.3.1 hoặc nếu ảnh của $E_i$ bởi ánh xạ $x \mapsto \|x\|$ được chứa trong ảnh của K bởi ánh xạ $a \mapsto |a|$ và chứa $R_i$ (với $1 \leq i \leq n$), thì có thể lấy $a = 1$.

4.3.3. Nếu K có đặc số không, chuỗi hình thức $f = \sum_\alpha f_\alpha$ thuộc $\mathcal{H}(E_1, \ldots, E_n; F)$ khi và chỉ khi tồn tại $R \in (\mathbf{R}_+^*)^n$ sao cho
$$
\sup_\alpha \sup_{x \in B(R)} \|f_\alpha(x)\|_y < +\infty
$$
với mọi nửa chuẩn liên tục $\gamma$ trên F.
