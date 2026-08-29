---
book: alg
book_title: Algebra
chapter: IX
chapter_title: Formes sesquilinéaires et formes quadratiques
section: 1
section_title: Formes sesquilinéaires
lang: vi
source: alg-ix-fr
pdf_pages: 0005-0038
extraction: ocr
subsections:
    - "no": 1
      title: Applications bilinéaires.
      page: 0
      pdf_page: 5
    - "no": 2
      title: Applications sesquilinéaires.
      page: 0
      pdf_page: 8
    - "no": 3
      title: Orthogonalité. Sommes directes d’applications bilinéaires ou sesquilinéaires.
      page: 0
      pdf_page: 10
    - "no": 4
      title: Changement d’anneaux de base.
      page: 0
      pdf_page: 11
    - "no": 5
      title: Quelques identités.
      page: 0
      pdf_page: 16
    - "no": 6
      title: Formes bilinéaires et sesquilinéaires. Rang.
      page: 0
      pdf_page: 16
    - "no": 7
      title: Forme inverse d’une forme bilinéaire ou sesquilinéaire.
      page: 0
      pdf_page: 21
    - "no": 8
      title: Adjoint d’un homomorphisme.
      page: 0
      pdf_page: 23
    - "no": 9
      title: Produits tensoriels et puissances extérieures de formes sesquilinéaires.
      page: 0
      pdf_page: 25
    - "no": 10
      title: Calculs matriciels.
      page: 0
      pdf_page: 30
statements: 45
exercises: 0
content_sha256: f82552c03564e4cf2063db2814d2e113bf00894e5f0df883ad43298c0629d10a
translated_from: content/en-mt/alg/IX/01_s1_formes_sesquilineaires.md
source_lang: en-mt
translation_method: machine
source_content_sha256: a788ed40848999c0d18ff945a803189841c5bd0cc9a81227b38d5b0ae7369e0a
translation_model: gpt-5-6, gpt-5-mini, gpt-5-6-mini
translation_run: translate-vi-8df81c1a
glossary_version: 34
glossary_terms_sha256: 555771022196f2ccdc24875de7acab72ca54ac285b39af6631e6bf0fb08d81f0
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 1. Dạng toàn phương sesqui

### 1. Ánh xạ song tuyến tính.

Trong No. này $A$ và $B$ ký hiệu hai vành, $E$ một $A$-môđun trái, $F$ một $B$-môđun phải, và $G$ một $(A, B)$-song môđun, nghĩa là một nhóm giao hoán được trang bị một cấu trúc $A$-môđun trái và một cấu trúc $B$-môđun phải sao cho $(ag)b = a(gb)$ với mọi $a \in A$, $b \in B$, $g \in G$.

#### Định nghĩa 1 {#alg-ix-s1-def-1 .statement}

Một ánh xạ $\Phi$ của tích $E \times F$ vào $G$ được gọi là song tuyến tính nếu nó thỏa mãn các điều kiện sau:

(1) $\Phi(x + x', y) = \Phi(x, y) + \Phi(x', y)$
    với mọi $x \in E$, $x' \in E$, $y \in F$ ;
(2) $\Phi(x, y + y') = \Phi(x, y) + \Phi(x, y')$
    với mọi $x \in E$, $y \in F$, $y' \in F$ ;
(3) $\Phi(ax, y) = a\Phi(x, y)$ với mọi $a \in A$, $x \in E$, $y \in F$ ;
(4) $\Phi(x, yb) = \Phi(x, y)b$ với mọi $x \in E$, $y \in F$, $b \in B$.

Tích tenxơ $E \otimes_{\mathbf{Z}} F$ được trang bị một cách chính tắc một cấu trúc của $(A, B)$-song môđun được đặc trưng bởi $a(x \otimes y)b = ax \otimes yb$ (Chương III, 2e éd., Phụ lục II, n° 3), và việc cho một ánh xạ song tuyến tính $\Phi$ của $E \times F$ vào $G$ tương đương với việc cho một ánh xạ $\Psi$ của $E \otimes_{\mathbf{Z}} F$ vào $G$ là một đồng cấu đối với các cấu trúc $(A, B)$-song môđun và thỏa mãn $\Psi(x \otimes y) = \Phi(x, y)$ với mọi $x \in E$ và $y \in F$.

Các điều kiện áp đặt lên $\Phi$ bởi Định nghĩa 1 có nghĩa là các ánh xạ từng phần $d_\Phi(y) : x \to \Phi(x, y)$ và $s_\Phi(x) : y \to \Phi(x, y)$ lần lượt là một ánh xạ A-tuyến tính từ $E$ vào $G$ và một ánh xạ B-tuyến tính từ $F$ vào $G$. Ta trang bị cho nhóm giao hoán $\mathcal{L}_A(E, G)$ (resp. $\mathcal{L}_B(F, G)$) cấu trúc của B-môđun phải (resp. A-môđun trái) được xác định bởi $ub(x) = u(x) . b$ ($u \in \mathcal{L}_A(E, G)$, $x \in E$, $b \in B$) (resp. $a \nu(y) = a . \nu(y)$ ($a \in A$, $\nu \in \mathcal{L}_B(F, G)$, $y \in F$)). Khi đó các điều kiện (1) đến (4) lần lượt tương đương với:

$$
\begin{align*}
(1') & \quad s_\Phi(x + x') = s_\Phi(x) + s_\Phi(x') \\
(2') & \quad d_\Phi(y + y') = d_\Phi(y) + d_\Phi(y') \\
(3') & \quad s_\Phi(ax) = a.s_\Phi(x) \\
(4') & \quad d_\Phi(yb) = d_\Phi(y).b,
\end{align*}
$$

với mọi $x, x'$ trong $E$, $y, y'$ trong $F$, $a \in A$, $b \in B$; nói cách khác, ánh xạ $d_\Phi$ từ $F$ vào $\mathcal{L}_A(E, G)$ là B-tuyến tính, và ánh xạ $s_\Phi$ từ $E$ vào $\mathcal{L}_B(F, G)$ là A-tuyến tính. Theo định nghĩa, ta có

$$(5) \quad \Phi(x, y) = d_\Phi(y)(x) = s_\Phi(x)(y) \text{ với mọi } x \in E, y \in F.$$

#### Định nghĩa 2 {#alg-ix-s1-def-2 .statement}

Cho một ánh xạ song tuyến tính $\Phi$ từ $E \times F$ vào $G$, ánh xạ $d_\Phi$ từ $F$ vào $\mathcal{L}_A(E, G)$ (resp. ánh xạ $s_\Phi$ từ $E$ vào $\mathcal{L}_B(F, G)$) được đặc trưng bởi (5) được gọi là ánh xạ tuyến tính liên kết bên phải (resp. bên trái) với $\Phi$.

Ngược lại, dữ liệu của một ánh xạ B-tuyến tính $d$ từ $F$ vào $\mathcal{L}_A(E, G)$ (resp. của một ánh xạ A-tuyến tính $s$ từ $E$ vào $\mathcal{L}_B(F, G)$) xác định duy nhất, bởi công thức

$$
\Phi(x, y) = d(y)(x) \quad \text{(resp. } \Phi(x, y) = s(x)(y))
$$

một ánh xạ song tuyến tính $\Phi$ từ $E \times F$ vào $G$, mà $d$ (resp. $s$) là ánh xạ tuyến tính liên kết bên phải (resp. bên trái).

#### Định nghĩa 3 {#alg-ix-s1-def-3 .statement}

Một ánh xạ song tuyến tính $\Phi$ của $E \times F$ vào $G$ được gọi là suy biến bên phải (tương ứng bên trái) nếu tồn tại một phần tử khác không $y_0$ của $F$ (tương ứng $x_0$ của $E$) sao cho $\Phi(x, y_0) = 0$ với mọi $x \in E$ (tương ứng $\Phi(x_0, y) = 0$ với mọi $y \in F$). Ta nói rằng $\Phi$ là suy biến nếu nó suy biến bên phải hoặc nếu nó suy biến bên trái.

Để $\Phi$ không suy biến bên phải (tương ứng bên trái), điều kiện cần và đủ là ánh xạ tuyến tính liên kết bên phải (tương ứng bên trái) với $\Phi$ là đơn ánh; nói rằng $\Phi$ không suy biến do đó có nghĩa là các ánh xạ tuyến tính liên kết $d_\Phi$ và $s_\Phi$ đều là đơn ánh.

Cho $(e_i)_{i \in I}$ và $(f_k)_{k \in K}$ là hai họ các phần tử của $E$ và $F$, và cho $(a_i)_{i \in I}$ và $(b_k)_{k \in K}$ là hai họ các phần tử của $A$ và $B$, tất cả trừ một số hữu hạn phần tử trong đó là không. Suy ra từ các đẳng thức (1) đến (4), bằng quy nạp theo số các hệ số khác không, rằng ta có

$$
\Phi(\sum_i a_i e_i, \sum_k f_k b_k) = \sum_{i,k} a_i \Phi(e_i, f_k) b_k.
$$

Nếu $(e_i)$ và $(f_k)$ là các hệ sinh của các môđun $E$ và $F$, thì $\Phi$ được xác định hoàn toàn bởi các phần tử $g_{ik} = \Phi(e_i, f_k)$. Nếu $(e_i)$ và $(f_k)$ là các cơ sở của $E$ và $F$ và nếu các phần tử $g_{ik}$ của $G$ ($i \in I, k \in K$) được cho, thì công thức

$$
\Phi(\sum_i a_i e_i, \sum_k f_k b_k) = \sum_{i,k} a_i g_{ik} b_k
$$

xác định một ánh xạ của $E \times F$ vào $G$, ánh xạ này là song tuyến tính và thỏa mãn $\Phi(e_i, f_k) = g_{ik}$. Khi $(e_i)$ và $(f_k)$ là các cơ sở hữu hạn, ta gọi $(\Phi(e_i, f_k))$ là ma trận của $\Phi$ đối với các cơ sở này.

Các ánh xạ song tuyến tính của $E \times F$ vào $G$ hiển nhiên tạo thành một nhóm con của nhóm cộng các ánh xạ của $E \times F$ vào $G$. Mặt khác, cho $a$ (tương ứng $b$) là một phần tử của tâm của $A$ (tương ứng $B$); khi đó ánh xạ $a \Phi b$ của $E \times F$ vào $G$ được xác định bởi $(a \Phi b)(x, y) = a . \Phi(x, y) . b$ là song tuyến tính. Tập hợp các ánh xạ song tuyến tính của $E \times F$ vào $G$ do đó được trang bị một cấu trúc song môđun trên các tâm của $A$ và $B$.

Cho E' (tương ứng F') là một A-môđun trái (tương ứng một B-môđun phải), u (tương ứng v) là một đồng cấu của E vào E' (tương ứng của F vào F') và $\Phi'$ là một ánh xạ song tuyến tính của $E' \times F'$ vào G. *Ảnh ngược* của $\Phi'$ (đối với u và v) được gọi là ánh xạ song tuyến tính $\Phi$ của $E \times F$ vào G được xác định bởi
$$
\Phi(x, y) = \Phi'(u(x), v(y)) \qquad (x \in E,\ y \in F).
$$
Ta dễ dàng kiểm tra rằng
$$
d_{\Phi}(y) = d_{\Phi'}(v(y)) \circ u \qquad \text{và} \qquad s_{\Phi}(x) = s_{\Phi'}(u(x)) \circ v
$$
với mọi $x \in E,\ y \in F$.

Cho $\Phi$ là một ánh xạ song tuyến tính của $E \times F$ vào G, và h là một đồng cấu (đối với các cấu trúc của các song môđun (A, B)) của G vào một song môđun (A, B) khác $G'$. Khi đó $h \circ \Phi$ là một ánh xạ song tuyến tính của $E \times F$ vào $G'$.

### 2. Các ánh xạ nửa song tuyến tính.

Trong No. này, trừ khi được nói rõ khác đi, A và B là hai vành, E là một A-môđun trái và F là một B-môđun *trái*; $b \to b^J$ ($b \in B$) là một *phản tự đẳng cấu* của B, nghĩa là một song ánh của B lên chính nó thỏa mãn $(b + c)^J = b^J + c^J$ và $(bc)^J = c^J b^J$ với mọi $b,\ c$ trong B; ta sẽ viết $J'$ thay cho $J^{-1}$. G là một song môđun (A, B) (No. 1).

#### Định nghĩa 4 {#alg-ix-s1-def-4 .statement}

*Ta nói rằng một ánh xạ $\Phi$ của $E \times F$ vào G là nửa song tuyến tính phải đối với J nếu nó thỏa mãn các điều kiện (1), (2), (3) (đn. 1, No. 1) cũng như*
(7) $\Phi(x, by) = \Phi(x, y) \cdot b^J$ với mọi $x \in E,\ y \in F$ và $b \in B$.

Nếu J là đồng nhất (điều này đòi hỏi B phải *giao hoán*), ta thu được khái niệm một ánh xạ song tuyến tính.

Cho $(e_i)_{i \in I}$ và $(f_k)_{k \in K}$ là hai họ các phần tử của E và F, và cho $(a_i)_{i \in I}$ và $(b_k)_{k \in K}$ là các phần tử của A và B bằng không trừ một số hữu hạn trong chúng. Khi đó
$$
\Phi(\sum_i a_i e_i, \sum_k b_k f_k) = \sum_{i,k} a_i \Phi(e_i, f_k) b_k^J.
$$

Như trong trường hợp của một ánh xạ song tuyến tính, các phần tử $\Phi(e_i, f_k)$ xác định duy nhất $\Phi$ khi $(e_i)$ và $(f_k)$ là các hệ sinh, và có thể được chọn tùy ý khi $(e_i)$ và $(f_k)$ là các cơ sở của E và F; khi $(e_i)$ và $(f_k)$ là các cơ sở hữu hạn, $(\Phi(e_i, f_k))$ được gọi là ma trận của $\Phi$ đối với các cơ sở này.

Đối với các ánh xạ song tuyến tính, người ta định nghĩa trên tập hợp các ánh xạ nửa song tuyến tính phải (đối với $J$) từ $E \times F$ vào $G$ một cấu trúc song môđun trên các tâm của $A$ và $B$. Người ta định nghĩa khái niệm ảnh ngược của một ánh xạ nửa song tuyến tính bằng cùng một công thức như đối với một ánh xạ song tuyến tính. Hơn nữa, ta sẽ thấy rằng việc nghiên cứu các ánh xạ nửa song tuyến tính có thể quy về việc nghiên cứu các ánh xạ song tuyến tính.

#### Định nghĩa 5 {#alg-ix-s1-def-5 .statement}

Cho $B$ là một vành, $F$ là một $B$-môđun trái (tương ứng phải) và $J$ là một phản tự đẳng cấu của $B$. Ta ký hiệu $F^J$ là $B$-môđun phải (tương ứng trái) có cùng nhóm cộng nền với $F$ và trong đó luật hợp thành ngoài là $(b, y) \to b^{J'}y$ (tương ứng $(b, y) \to yb^{J'}$) $(b \in B,\ y \in F,\ J' = J^{-1})$.

Với các ký hiệu của Định nghĩa 5, một ánh xạ tuyến tính từ $F^J$ vào một $B$-môđun phải (tương ứng trái) $H$ do đó được đồng nhất với một ánh xạ $\mathbf{Z}$-tuyến tính $u$ từ $F$ vào $H$ thỏa mãn
$$
u(by) = u(y)b^J \quad \text{(tương ứng } u(yb) = b^Ju(y)) \quad (b \in B,\ y \in F).
$$

Ánh xạ $u$ từ $F$ vào $H$ là một ánh xạ nửa tuyến tính từ $F$ vào $H$ đối với $J$ (chương II, Phụ lục I, số 1), nếu ta xét $J$ như một đẳng cấu của vành $B^0$ đối của $B$ lên $B$, và $F$ như một $B^0$-môđun phải (tương ứng trái).

Tương tự, một ánh xạ nửa song tuyến tính phải $\Phi$ (đối với $J$) từ $E \times F$ vào $G$, trong đó $F$ là một $B$-môđun trái, được đồng nhất với một ánh xạ song tuyến tính từ $E \times F^J$ vào $G$; nếu ánh xạ sau suy biến phải (tương ứng suy biến trái, không suy biến), người ta nói rằng $\Phi$ suy biến phải (tương ứng suy biến trái, không suy biến).

#### Nhận xét {#alg-ix-s1-n2-rem-1 .statement}

Cho $A$ và $B$ là hai vành, $J_1$ là một phản tự đẳng cấu của $A$, $M$ là một $A$-môđun phải, $N$ là một $B$-môđun phải và G là một (A, B)-song môđun. Người ta nói rằng một ánh xạ $\Phi$ từ $M \times N$ vào G là *nửa song tuyến tính trái đối với $J_1$* nếu nó là $\mathbf{Z}$-song tuyến tính và nếu nó thỏa mãn

$$
\Phi(xa, yb) = a^{J_1} \Phi(x, y)b \quad (x \in M, y \in N, a \in A, b \in B).
$$

Một ánh xạ như vậy được đồng nhất với một ánh xạ song tuyến tính từ $M^{J_1} \times N$ vào G. Ta thường để cho độc giả nhiệm vụ chuyển sang các ánh xạ nửa song tuyến tính trái các định nghĩa và tính chất đã cho đối với các ánh xạ nửa song tuyến tính phải; khi ta nói đến một ánh xạ nửa song tuyến tính (không có chỉ rõ thêm), nó sẽ là một ánh xạ nửa song tuyến tính phải.

### 3. Trực giao. Các tổng trực tiếp của các ánh xạ song tuyến tính hoặc nửa song tuyến tính.

Trong Số này, A và B ký hiệu các vành, E là một A-môđun trái, F là một B-môđun phải (resp. một B-môđun trái), G là một song môđun (A, B), và $\Phi$ là một ánh xạ song tuyến tính (resp. ánh xạ sesquilinear đối với một tự đẳng cấu phản J đã cho của B) từ $E \times F$ vào G.

#### Định nghĩa 6 {#alg-ix-s1-def-6 .statement}

*Hai phần tử $x \in E$ và $y \in F$ được gọi là trực giao đối với $\Phi$ nếu $\Phi(x, y) = 0$. Hai tập con $E' \subset E$ và $F' \subset F$ được gọi là trực giao nếu, với mọi $x \in E'$ và $y \in F'$, $x$ và $y$ là trực giao. Tập hợp các phần tử của $E$ (resp. F) trực giao với một môđun con N đã cho của F (resp. M của E) là một môđun con của E (resp. F), được gọi là môđun con trực giao toàn phần (hoặc đơn giản là môđun con trực giao) với N (resp. M), và được ký hiệu bởi $N^0$ (resp. $M^0$).*

Cho H và $H'$ là hai môđun con của E hoặc F. Ta có $H \subset (H^0)^0$ (được ký hiệu bởi $H^{00}$); nếu $H \subset H'$, ta có ${H'}^0 \supset H^0$. Suy ra ta có $H^0 \supset (H^{00})^0$ và $H^0 \subset (H^0)^{00}$; khi đặt

$$
H^{000} = (H^{00})^0 = (H^0)^{00} = ((H^0)^0)^0,
$$

do đó ta có $H^0 = H^{000}$.

Để ánh xạ $\Phi$ là suy biến (No. 1, Def. 3), điều kiện cần và đủ là ít nhất một trong hai môđun con $E^0, F^0$ phải $\neq \{0\}$. Rõ ràng rằng $\Phi(x, y)$ không thay đổi khi một phần tử của $F^0$ (resp. $E^0$) được thêm vào $x$ (resp. $y$), và do đó $\Phi$ xác định, bằng cách chuyển qua thương, một ánh xạ song tuyến tính (hoặc ánh xạ sesquilinear) trên $(E/F^0) \times (F/E^0)$; ánh xạ này hiển nhiên không suy biến; nó được gọi là ánh xạ song tuyến tính (hoặc ánh xạ sesquilinear) không suy biến liên kết với $\Phi$.

Cho $(E_i)_{i \in I}$ là một họ các A-môđun trái, $(F_i)_{i \in I}$ là một họ các B-môđun phải (tương ứng, các B-môđun trái), và $\Phi_i$ là một ánh xạ song tuyến tính (tương ứng, song J-nửa tuyến tính phải) từ $E_i \times F_i$ vào G. Gọi $E$ (tương ứng, $F$) là môđun tổng trực tiếp của các $E_i$ (tương ứng, $F_i$). Ta thấy ngay lập tức rằng ánh xạ $\Phi$ từ $E \times F$ vào G được xác định bởi
$$
\Phi((x_i), (y_i)) = \sum_i \Phi_i(x_i, y_i) \quad (x_i \in E_i, y_i \in F_i)
$$
(tổng này có nghĩa vì mọi số hạng của nó, trừ một số hữu hạn, đều bằng không) là song tuyến tính (tương ứng, song J-nửa tuyến tính phải). Nó được gọi là tổng trực tiếp của các ánh xạ $\Phi_i$. Rõ ràng rằng $E_i$ trực giao với $F_j$ đối với $\Phi$ khi $i \neq j$. Ngược lại, cho $\Phi$ là một ánh xạ song tuyến tính hoặc nửa tuyến tính từ $E \times F$ vào G, và giả sử rằng E là tổng trực tiếp của các môđun con $(E_i)_{i \in I}$ và F là tổng trực tiếp của các môđun con $(F_i)_{i \in I}$ sao cho $E_i$ trực giao với $F_j$ khi $i \neq j$; khi đó $\Phi$ là tổng trực tiếp của các hạn chế của nó lên các tích $E_i \times F_i$ ($i \in I$).

Để $\Phi$ không suy biến, điều kiện cần và đủ là mỗi $\Phi_i$ đều như vậy; dưới các điều kiện này, môđun con trực giao với $E_i$ là $\sum_{j \neq i} F_j$.

### 4. Thay đổi vành cơ sở.

Trong mục này, cho A, B, A', B' là bốn vành, $h$ và $h'$ là các đồng cấu của A vào A' và của B vào B' tương ứng, G là một song môđun (A, B), G' là một song môđun (A', B'), và $u$ là một đồng cấu của nhóm Abel nền của G vào nhóm Abel nền của G', thỏa mãn
$$
u(agb) = h(a)u(g)h'(b) \quad (a \in A, g \in G, b \in B).
$$

Cho E (tương ứng, F) là một A-môđun trái (tương ứng, B-môđun phải). Nhắc lại (Chap. III, 2e éd., App. II, no 10) rằng, nếu $A'$ (tương ứng, $B'$) được xem như một A-môđun phải (tương ứng, B-môđun trái), tích tenxơ $E' = A' \otimes_A E$ (tương ứng, $F' = F \otimes_B B'$) được trang bị một cấu trúc của A'-môđun trái (tương ứng, B'-môđun phải) được xác định bởi

$$
a'_1(a' \otimes x) = (a'_1 a') \otimes x \quad (a', a'_1 \in A', x \in E)
$$
(tương ứng, $(y \otimes b') b'_1 = y \otimes (b' b'_1)$ $(b', b'_1 \in B', y \in F)$).

#### Mệnh đề 1 {#alg-ix-s1-prop-1 .statement}

*Cho $E$ là một A-môđun trái và $F$ là một B-môđun phải; đặt $E' = A' \otimes_A E$ và $F' = F \otimes_B B'$. Với mọi ánh xạ song tuyến tính $\Phi$ từ $E \times F$ vào $G$, tồn tại duy nhất một ánh xạ song tuyến tính $\Phi'$ từ $E' \times F'$ vào $G'$ sao cho*

$$
\Phi'(a' \otimes x, y \otimes b') = a'.u(\Phi(x, y)).b'
$$

bất kỳ $a' \in A'$, $b' \in B'$, $x \in E$, $y \in F$.

Tính duy nhất của $\Phi'$ suy ra từ sự kiện rằng các phần tử $a' \otimes x$ và $y \otimes b'$ sinh ra $E'$ và $F'$ tương ứng. Để chứng minh sự tồn tại của nó, xét ánh xạ

$$
m : (a', x, y, b') \to a'.u(\Phi(x, y)).b'
$$

từ $A' \times E \times F \times B'$ vào $G$; nó hiển nhiên là $\mathbf{Z}$-đa tuyến tính, và nó thỏa mãn

$$
m(a', ax, y, b') = m(a'h(a), x, y, b')
$$
và
$$
m(a', x, yb, b') = m(a', x, y, h'(b)b')
$$
$(a \in A, b \in B, a' \in A', b' \in B', x \in E, y \in F)$.

Do đó tồn tại một ánh xạ song tuyến tính trên $\mathbf{Z}$ $\Phi'$ từ $E' \times F'$ vào $G'$ thỏa mãn (13) (Chap. III, 2nd ed., App. II, No. 1, prop. 2). Quan hệ này và định nghĩa các cấu trúc môđun của $E'$ và $F'$ bởi (12) cho thấy rằng $\Phi'$ là song tuyến tính, điều này hoàn thành chứng minh.

Các giả thiết và ký hiệu là những cái của Mệnh đề 1, bây giờ ta hãy nghiên cứu các *ánh xạ tuyến tính liên kết* của $\Phi$ và $\Phi'$ (No. 1, def. 2). Vì mục đích này trước hết ta sẽ định nghĩa một đồng cấu chính tắc từ $\mathcal{L}_A(E, G)$ vào $\mathcal{L}_{A'}(E', G')$. Với mọi $\nu \in \mathcal{L}_A(E, G)$, ánh xạ $(a', x) \to a'.u(\nu(x))$ từ $A' \times E$ vào $G'$ là song tuyến tính trên $\mathbf{Z}$, và, được xem như (11), biến $(a'h(a), x)$ và $(a', ax)$ $(a \in A)$ thành cùng một phần tử của $G'$; do đó nó định nghĩa (Chap. III, 2nd ed.,

App. II, Nos. 1 và 10) một ánh xạ $k(\nu)$ từ $E' = A' \otimes_A E$ vào $G'$ sao cho $k(\nu)(a' \otimes x) = a'.u(\nu(x))$, và ánh xạ này, được xem như (12), là $A'$-tuyến tính. Hơn nữa, ta ngay lập tức suy ra từ (12) rằng ánh xạ $\nu \to k(\nu)$ từ $\mathcal{L}_A(E, G)$ vào $\mathcal{L}_{A'}(E', G')$ thỏa mãn $k(\nu b) = k(\nu)h'(b)$ với mọi $b \in B$. Gọi $i$ là ánh xạ chính tắc $y \to y \otimes 1$ từ $F$ vào $F'$. Khi đó biểu đồ

$$
\begin{array}{ccc}
F & \xrightarrow{d_\Phi} & \mathcal{L}_A(E, G) \\
|_i & & |_k \\
F' & \xrightarrow{d_{\Phi'}} & \mathcal{L}_{A'}(E', G')
\end{array}
$$

(trong đó $d_\Phi$ và $d_{\Phi'}$ ký hiệu các ánh xạ tuyến tính liên kết phải của $\Phi$ và $\Phi'$) là *giao hoán*. Thật vậy, với $x \in E, y \in F$ và $a' \in A'$, ta có $d_{\Phi'}(i(y))(a' \otimes x) = \Phi'(a' \otimes x, y \otimes 1) = a'.u(\Phi(x, y)) = a'.u(d_\Phi(y)(x))$, nghĩa là, $d_{\Phi'}(i(y))(a' \otimes x) = k(d_\Phi(y))(a' \otimes x)$. Có một quan hệ giao hoán tương tự cho các ánh xạ tuyến tính liên kết trái $s_\Phi$ và $s_{\Phi'}$ của $\Phi$ và $\Phi'$.

#### Mệnh đề 2 {#alg-ix-s1-prop-2 .statement}

*Giả sử rằng B và B' được trang bị các phản tự đẳng cấu J và I sao cho*

$$(15)$$
$$ h'(b^J) = h'(b)^I \quad \text{cho mọi } b \in B. $$

*Cho E là một A-môđun trái và F là một B-môđun trái; đặt $E' = A' \otimes_A E$ và $F' = B' \otimes_B F$. Với mọi ánh xạ nửa song tuyến tính (đối với J) $\Phi$ của $E \times F$ vào $G$, tồn tại một và chỉ một ánh xạ nửa song tuyến tính (đối với I) $\Phi'$ của $E' \times F'$ vào $G'$ sao cho*

$$(16)$$
$$ \Phi'(a' \otimes x, b' \otimes y) = a'.u(\Phi(x, y)).{b'}^I $$

*đối với mọi $a' \in A'$, $b' \in B'$, $x \in E$, $y \in F$.*

Tính duy nhất của $\Phi'$ suy ra từ sự kiện rằng các tích tenxơ $a' \otimes x$ và $b' \otimes y$ sinh ra $E'$ và $F'$ tương ứng. Để thiết lập sự tồn tại của nó, xét ánh xạ

$$ m : (a, x, b', y) \to a'.u(\Phi(x, y)).{b'}^I $$

từ $A' \times E \times B' \times F$ vào $G'$. Ánh xạ này hiển nhiên là $\mathbf{Z}$-đa tuyến tính, và, theo (11) và (15), thỏa mãn $m(a', ax, b', y) = m(a'h(a), x, b', y)$ và $m(a', x, b', by) = a'.u(\Phi(x, y)).h'(b^J){b'}^I = m(a', x, b'h'(b), y)$ ($a \in A, b \in B, a' \in A', b' \in B', x \in E, y \in F$). Do đó tồn tại một ánh xạ $\mathbf{Z}$-song tuyến tính $\Phi'$ của $E' \times F'$ vào $G'$ thỏa mãn (16) (chương III, 2e éd., Phụ lục II, số 1, mệnh đề 2). Quan hệ này, cùng với định nghĩa các cấu trúc môđun của E' và F' bởi (12), cho thấy, theo (15), rằng $\Phi'$ là nửa song tuyến tính đối với I, điều này hoàn thành chứng minh.

Các ví dụ quan trọng nhất của các song môđun $(A', B')$ G', được trang bị các ánh xạ tuyến tính $\mathbf{Z}$ $u$ từ G vào G' thỏa mãn (11), là các ví dụ sau:

1) Ta lấy tích tenxơ $G'$ là $A' \otimes_A G \otimes_B B'$ (chương III, ấn bản lần thứ 2, Phụ lục II, No. 9) và lấy $u$ là ánh xạ
$$
g \to 1 \otimes g \otimes 1 \qquad (g \in G)
$$
từ G vào G'. Cặp $(G', u)$ được xác định như vậy rõ ràng là *phổ quát* theo nghĩa sau: đối với mọi song môđun $(A', B')$ $G'_1$ và mọi ánh xạ tuyến tính trên $\mathbf{Z}$ $u_1$ của G vào $G'_1$ thỏa mãn điều tương tự của (11), tồn tại duy nhất một ánh xạ tuyến tính trên $\mathbf{Z}$ $f$ của G' vào $G'_1$ sao cho $f(a'g'b') = a'f(g')b'$ ($a' \in A'$, $g' \in G'$, $b' \in B'$; nói cách khác $f$ là một đồng cấu đối với các cấu trúc song môđun của G' và $G'_1$) và sao cho $u_1 = f \circ u$.

2) Khi $A = B = G$ (cấu trúc song môđun $(A, A)$ của A được xác định bởi các phép vị tự trái và phải), $A' = B'$, và $h = h'$ thì ta có thể lấy G' là vành $A'$ và lấy $u$ là đồng cấu $h$ của A vào $A'$.

3) Giả sử rằng $A = B$, $A' = B'$, $h = h'$, rằng các vành A và A' là *giao hoán*, và rằng cấu trúc A-môđun trái của G trùng với cấu trúc A-môđun phải của nó. Khi đó ta có thể lấy G' là tích tenxơ $A' \otimes_A G$ (cấu trúc A'-môđun phải của G' trùng với cấu trúc A'-môđun trái của nó) và lấy $u$ là ánh xạ $g \to 1 \otimes g$ ($g \in G$) từ G vào G'. Khi đó ta sẽ nói rằng ánh xạ song tuyến tính (tương ứng ánh xạ nửa song tuyến tính) $\Phi'$ được xác định bởi mệnh đề 1 (tương ứng mệnh đề 2) thu được từ $\Phi$ *bằng mở rộng vành cơ sở*, hay *bằng mở rộng vô hướng*.

Điều sau đây đúng như nhau đối với các ánh xạ song tuyến tính và các ánh xạ nửa song tuyến tính; các giả thiết và ký hiệu là những điều của mệnh đề 1 (tương ứng mệnh đề 2). Cho một môđun con M của E hoặc F, ta ký hiệu bởi M' môđun con của E' hoặc F' sinh bởi ảnh chính tắc của M.

#### Mệnh đề 3 {#alg-ix-s1-prop-3 .statement}

Các giả thiết và ký hiệu là những điều của mệnh đề 1 (tương ứng mệnh đề 2), giả sử thêm rằng A, B, A', B' là các trường và rằng các ánh xạ α và β của $A' \otimes_A G$ và $G \otimes_B B'$ vào G' được đặc trưng bởi $\alpha(a' \otimes g) = a'u(g)$ và $\beta(g \otimes b') = u(g)b'$ ($a' \in A'$, $b' \in B'$, $g \in G$) là đơn ánh. Cho M là một không gian con của E và N là một không gian con của F. Khi đó không gian con $(M')^0$ của F' trực giao với M' đối với $\Phi'$ bằng $(M^0)'$, và tương tự, ta có $(N')^0 = (N^0)'$.

Thật vậy, các bao hàm $(M^0)' \subset (M')^0$ và $(N^0)' \subset (N')^0$ là hiển nhiên (và hơn nữa còn đúng mà không cần các giả thiết về A, B, A', B', $\alpha$ hoặc $\beta$). Ta sẽ chứng minh bao hàm $(M')^0 \subset (M^0)'$; ta để lại cho độc giả việc kiểm tra bao hàm $(N')^0 \subset (N^0)'$, điều này hoàn toàn tương tự. Cho $y'$ là một phần tử của $(M')^0$. Ta có thể viết

$$
y' = \sum_{i=1}^s y_i \otimes b'_i \quad \text{(resp. } y' = \sum_{i=1}^s b'_i \otimes y_i)
$$

trong đó $y_i \in F$ ($1 \leq i \leq s$), và trong đó các $b'_i$ là các phần tử của B' độc lập tuyến tính trên B đối với cấu trúc B-môđun trái (tương ứng B-môđun phải) của B'. Cho $x \in M$ và $x' = 1 \otimes x \in M'$. Ta có

$$
0 = \Phi'(x', y') = \sum_i u(\Phi(x, y_i)) b'_i = \beta(\sum_i \Phi(x, y_i) \otimes b'_i)
$$
(tương ứng $0 = \Phi'(x', y') = \sum_i u(\Phi(x, y_i)) {b'}^I_i = \beta(\sum_i \Phi(x, y_i) \otimes {b'}^I_i)$).

Vì $\beta$ là đơn ánh và các $b'_i$ (tương ứng các ${b'}^I_i$, có tính đến (15)) độc lập tuyến tính trên B đối với cấu trúc B-môđun trái của B', điều này suy ra $\Phi(x, y_i) = 0$ với $i = 1, \ldots, s$. Vì quan hệ cuối cùng này đúng với mọi $x \in M$, ta có $y_i \in M^0$ với $i = 1, \ldots, s$, do đó $y' \in (M^0)'$. QED.

#### Hệ quả {#alg-ix-s1-n4-cor-1 .statement}

Các giả thiết và ký hiệu là những cái của Mệnh đề 3, để $\Phi'$ không suy biến, điều kiện cần và đủ là $\Phi$ không suy biến.

Thật vậy, theo Mệnh đề 3, ta có $(F')^0 = (F^0)'$ và $(E')^0 = (E^0)'$. Mặt khác, để $\Phi$ (tương ứng $\Phi'$) không suy biến, điều kiện cần và đủ là phải có $F^0 = E^0 = \{0\}$ (tương ứng $(F')^0 = (E')^0 = \{0\}$).

#### Nhận xét {#alg-ix-s1-n4-rem-1 .statement}

Giả sử rằng A, B, A' và B' là các trường. Khi đó, đối với các song môđun G' được định nghĩa trong ba ví dụ trên, các ánh xạ $\alpha$ và $\beta$ là đơn ánh, như suy ra ngay lập tức từ Chap. III, 2nd ed., App. II, No. 6.

### 5. Một số đẳng thức.

Trong No. này, cho A là một vành được trang bị một tự phản đẳng cấu J, E một A-môđun trái, G một (A, A)-song môđun, và $\Phi$ một ánh xạ sesquilinear (phải) đối với J từ $E \times E$ vào G. Đặt $Q(x) = \Phi(x, x)$ ($x \in E$). Hiển nhiên ta có

$$
\begin{align*}
(17) \quad & Q(x + y) = Q(x) + \Phi(x, y) + \Phi(y, x) + Q(y) \\
(18) \quad & Q(x - y) = Q(x) - \Phi(x, y) - \Phi(y, x) + Q(y)
\end{align*}
$$

với mọi $x, y$ trong E. Do đó, bằng phép trừ,

$$
(19) \quad 2(\Phi(x, y) + \Phi(y, x)) = Q(x + y) - Q(x - y).
$$

Cho $a$ là một phần tử của A; thay $y$ bởi $ay$ trong (19), ta thu được

$$
(20) \quad 2(\Phi(x, y)a^j + a\Phi(y, x)) = Q(x + ay) - Q(x - ay).
$$

Ta suy ra từ (19) và (20), bằng cách nhân (19) với $a$ (bên trái) và trừ:

$$
\begin{align*}
(21) \quad & 2(a\Phi(x, y) - \Phi(x, y)a^j) \\
& \quad = aQ(x + y) - aQ(x - y) - Q(x + ay) + Q(x - ay).
\end{align*}
$$

Đặc biệt, giả sử rằng A là một mở rộng bậc hai $K(i)$ của một vành giao hoán K, với $i^2 = -1$ (Chap. II, § 7, No. 7), rằng J là tự đẳng cấu K $u + iv \to u - iv$ ($u, v$ trong K) của A, và rằng các cấu trúc A-môđun trái và A-môđun phải của G trùng nhau. Lấy $a = i$ trong (21), ta thu được

$$
(22) \quad 4\Phi(x, y) = Q(x + y) - Q(x - y) + iQ(x + iy) - iQ(x - iy).
$$

### 6. Các dạng song tuyến tính và sesquilinear. Hạng.

Trong No. này, cho A là một vành (tương ứng một vành được trang bị một tự phản đẳng cấu J), E một A-môđun trái, và F một A-môđun phải (tương ứng A-môđun trái). Ta trang bị cho A cấu trúc của (A, A)-song môđun được xác định bởi các phép vị tự trái và các phép vị tự phải. Trong trường hợp này một ánh xạ song tuyến tính (tương ứng ánh xạ sesquilinear phải đối với J) từ E × F vào song môđun A được gọi là một dạng song tuyến tính (tương ứng dạng sesquilinear phải đối với J) trên E × F.

Khi E = F (điều này kéo theo rằng nó là một dạng sesquilinear), người ta thường nói rằng một dạng sesquilinear trên E × F là một dạng sesquilinear trên E.

Cho hai A-môđun trái E và E′, và hai dạng sesquilinear $\Phi$ và $\Phi′$ đối với J trên E và E′ tương ứng, ta nói rằng $\Phi$ và $\Phi′$ là tương đương nếu tồn tại một đẳng cấu u của A-môđun E lên A-môđun E′ sao cho $\Phi′(u(x), u(y)) = \Phi(x, y)$ với mọi $x, y$ trong E; khi đó $\Phi$ là ảnh ngược của $\Phi′$ đối với u và u, và $\Phi′$ là ảnh ngược của $\Phi$ đối với $u^{-1}$ và $u^{-1}$ (No. 2).

Cho $\Phi$ là một dạng song tuyến tính trên E × F (F là một A-môđun phải). Các ánh xạ tuyến tính $s_{Φ}$ và $d_{Φ}$ liên kết với $\Phi$ (No. 1, Định nghĩa 2) khi đó là các ánh xạ từ E vào đối ngẫu F* của F, và từ F vào đối ngẫu E* của E.

Theo định nghĩa do đó

$$
\Phi(x, y) = \langle x, d_{Φ}(y) \rangle = \langle y, s_{Φ}(x) \rangle.
$$

Bây giờ ta sẽ định nghĩa các ánh xạ tuyến tính liên kết với một dạng sesquilinear. Cho J là một tự phản đẳng cấu của A và $\Phi$ là một dạng sesquilinear (bên phải) đối với J trên E × F (F là một A-môđun trái); đặt J′ = J^{-1}. Ánh xạ $\Phi′$ từ F × E vào A được định nghĩa bởi

$$
Φ′(y, x) = Φ(x, y)^{J′} \quad (x ∈ E, y ∈ F)
$$

là, như ta dễ dàng thấy, một dạng sesquilinear (bên phải) đối với J′ trên F × E. Theo No. 2 (Định nghĩa 5) các dạng sesquilinear $\Phi$ và $\Phi′$ lần lượt được đồng nhất với các dạng song tuyến tính trên E × F^{J′} và trên F × E^{J′}. Các ánh xạ $d_{Φ}$ và $d_{Φ′}$ liên kết với các dạng sau được gọi là các ánh xạ liên kết phải và trái với dạng sesquilinear $\Phi$, và được ký hiệu bởi $d_\Phi$ và $s_\Phi$. Do đó ta có, theo định nghĩa:

$$
(24)\quad \Phi(x, y) = \langle x, d_\Phi(y) \rangle = \langle y, s_\Phi(x) \rangle^J \qquad (x \in E,\ y \in F).
$$

Do đó $d_\Phi$ (tương ứng $s_\Phi$) là một ánh xạ tuyến tính từ $F^J$ vào $E^*$ (tương ứng từ $E^{J'}$ vào $F^*$), hoặc lại là một ánh xạ nửa tuyến tính từ $F$ vào $E^*$ (tương ứng từ $E$ vào $F^*$) đối với $J$ (tương ứng $J'$) nếu $J$ (tương ứng $J'$) được xem như một đẳng cấu của vành $A^0$ (đối của $A$) lên $A$, và $F$ (tương ứng $E$) như một môđun phải trên $A^0$.

Công thức (24) và Định nghĩa 6 của No. 3 ngay lập tức suy ra rằng với mọi môđun con $N$ của $F$ (tương ứng $M$ của $E$), ta có

$$
(25)\quad N^0 = s_\Phi^{-1}(N') \qquad (\text{resp. } M^0 = d_\Phi^{-1}(M'))
$$

trong đó $N'$ (tương ứng $M'$) là môđun con của đối ngẫu $F^*$ của $F$ (tương ứng của đối ngẫu $E^*$ của $E$) vuông góc với $N$ (tương ứng $M$) (Chương II, § 4, No. 2).

#### Mệnh đề 4 {#alg-ix-s1-prop-4 .statement}

*Giả sử rằng $A$ là một trường, và cho $\Phi$ là một dạng song tuyến tính (tương ứng dạng nửa song tuyến tính đối với $J$) trên $E \times F$; để $E/F^0$ có số chiều hữu hạn, điều kiện cần và đủ là $F/E^0$ có số chiều hữu hạn, và khi đó các số chiều này bằng nhau.*

Thật vậy, gọi $\Phi_1$ là dạng không suy biến liên kết với $\Phi$, trên $(E/F^0) \times (F/E^0)$ (No. 3). Giả sử rằng $E/F^0$ có số chiều hữu hạn $n$; vì ánh xạ tuyến tính $d_{\Phi_1}$ từ $F/E^0$ (tương ứng $(F/E^0)^J$) vào $(E/F^0)^*$ là đơn ánh, $F/E^0$ có số chiều hữu hạn $n' \leq n$; xét $s_{\Phi_1}$, ta thấy tương tự rằng $n \leq n'$.

#### Hệ quả 1 {#alg-ix-s1-prop-4-cor-1 .statement}

*Giả sử rằng $A$ là một trường và rằng $\Phi$ không suy biến. Để một không gian con $M$ của $E$ có số chiều hữu hạn, điều kiện cần và đủ là $M^0$ có đối chiều hữu hạn trong $F$, và khi đó ta có $\operatorname{codim} M^0 = \dim M$, và $M^{00} = M$.*

Vì $F^0 = \{0\}$, hai mệnh đề đầu tiên suy ra từ mệnh đề 4 áp dụng cho hạn chế của $\Phi$ lên $M \times F$. Hơn nữa, $M^0$ là trực giao của $M^{00}$, do đó $M^{00}$ có số chiều hữu hạn bằng $\operatorname{codim} M^0 = \dim M$; nhưng vì $M^{00} \supset M$, ta có $M^{00} = M$.

#### Hệ quả 2 {#alg-ix-s1-prop-4-cor-2 .statement}

*Các giả thiết là các giả thiết của hệ quả 1, cho $M, N$ là hai không gian con của $E$; khi đó ta có $(M + N)^0 = M^0 \cap N^0$; nếu hơn nữa $M$ và $N$ có số chiều hữu hạn, ta có $(M \cap N)^0 = M^0 + N^0$.*

Mệnh đề đầu tiên là tầm thường. Giả sử rằng M và N có số chiều hữu hạn, và đặt G = M^0 + N^0; ta có G^0 = M^{00} \cap N^{00} = M \cap N theo hệ quả 1; mệnh đề 4 áp dụng cho hạn chế của $\Phi$ lên $M \times G$ khi đó chỉ ra (vì $M^0 \subset G$ và $G^0 \subset M$) rằng ta có $\dim M/(M \cap N) = \dim G/M^0 = \operatorname{codim} M^0 - \operatorname{codim} G$, và vì $\operatorname{codim} M^0 = \dim M$, ta suy ra $\dim (M \cap N) = \operatorname{codim} G$. Nhưng ta cũng có $\dim (M \cap N) = \operatorname{codim} (M \cap N)^0$ theo hệ quả 1, và vì $G \subset G^{00} = (M \cap N)^0$ ta có $G = (M \cap N)^0$.

Mệnh đề 4 cho phép ta đưa ra định nghĩa sau:

#### Định nghĩa 7 {#alg-ix-s1-def-7 .statement}

Cho A là một trường (tương ứng, một trường được trang bị một phản tự đẳng cấu J), E là một không gian vectơ trái trên A, F là một không gian vectơ phải (tương ứng, trái) trên A, và $\Phi$ là một dạng song tuyến tính (tương ứng, sesquilinear đối với J) trên $E \times F$. Giả sử rằng $E/F^0$ và $F/E^0$ có số chiều hữu hạn trên A. Hạng của $\Phi$ được gọi là số chiều chung (hữu hạn) của các không gian vectơ $E/F^0$ và $F/E^0$.

Khi $E/F^0$ và $F/E^0$ có số chiều vô hạn, ta nói rằng $\Phi$ có hạng vô hạn.

#### Mệnh đề 5 {#alg-ix-s1-prop-5 .statement}

Các giả thiết và ký hiệu là các giả thiết và ký hiệu của định nghĩa 7, các ánh xạ tuyến tính $s_\Phi$ và $d_\Phi$ liên kết với $\Phi$ có cùng hạng, và hạng này bằng hạng của dạng $\Phi$.

Thật vậy, hạt nhân của ánh xạ $d_\Phi$ từ F vào $E^*$ hiển nhiên là $E^0$, do đó hạng của nó bằng chiều của $F/E^0$. Tương tự, hạng của $s_\Phi$ bằng chiều của $E/F^0$.

#### Mệnh đề 6 {#alg-ix-s1-prop-6 .statement}

Các giả thiết và ký hiệu là các giả thiết và ký hiệu của định nghĩa 7, giả sử thêm rằng E và F có cùng số chiều hữu hạn. Khi đó các điều kiện sau là tương đương:
a) $d_\Phi$ là đơn ánh ;
b) $d_\Phi$ là toàn ánh ;
c) $s_\Phi$ là đơn ánh ;
d) $s_\Phi$ là toàn ánh ;
e) $\Phi$ là không suy biến.

Thật vậy, vì E, F, $E^*$ và $F^*$ có cùng số chiều hữu hạn,

a) và b) là tương đương, cũng như c) và d) (chương II, § 3, số 4). Vì $s_\Phi$ và $d_\Phi$ có cùng hạng (mệnh đề 5), a) và c) là tương đương. Vì e) tương đương với quan hệ $E^0 = F^0 = \{0\}$, nó tương đương với phép hội của a) và c), do đó có sự tương đương của các điều kiện đã nêu.

#### Hệ quả {#alg-ix-s1-n6-cor-1 .statement}

Các giả thiết và ký hiệu là những giả thiết và ký hiệu của Định nghĩa 7, ta giả sử thêm rằng E có số chiều hữu hạn và $\Phi$ không suy biến. Khi đó ta có $\dim E = \dim F$ và, với mọi cơ sở $(e_i)$ ($1 \leq i \leq \dim E$) của E, tồn tại một cơ sở $(f_i)$ của F sao cho $\Phi(e_i, f_k) = \delta_{ik}$ ($i, k = 1, ..., \dim E$).

Thật vậy, vì $\Phi$ không suy biến, ta có $E^0 = F^0 = \{0\}$, do đó $\dim E = \dim F$ (mệnh đề 4). Suy ra (mệnh đề 6) rằng $d_\Phi$ là một đẳng cấu của F (tương ứng $F^j$) lên $E^*$; do đó, nếu $(e_i^*)$ là cơ sở đối ngẫu của $(e_i)$, các phần tử $f_i = d_\Phi^{-1}(e_i^*)$ lập thành một cơ sở của F mà, theo công thức (23) (tương ứng công thức (24)), thỏa mãn $\Phi(e_i, f_k) = \delta_{ik}$.

Ngay lập tức thấy rằng, trong hệ quả này, ta có thể hoán đổi vai trò của E và F, thay thế $d_\Phi$ bởi $s_\Phi$ trong chứng minh.

#### Nhận xét {#alg-ix-s1-n6-rem-1 .statement}

Cho A là một vành được trang bị một tự đẳng cấu ngược J, M và N là các A-môđun phải, và $\Phi$ là một dạng nửa song tuyến tính trái đối với J trên $M \times N$ (No. 2, Nhận xét); do đó nó thỏa mãn đẳng thức

$$
\Phi(xa, xa') = a^j \Phi(x, y)a' \quad (a, a' \in A, x \in M, y \in N).
$$

Ánh xạ $\Phi'$ từ $N \times M$ vào A được xác định bởi $\Phi'(y, x) = \Phi(x, y)^{J'}$ (trong đó $J' = J^{-1}$) là một dạng nửa song tuyến tính trái đối với $J'$, và $\Phi$ và $\Phi'$ đồng nhất với các dạng song tuyến tính trên $M^{J'} \times N$ và $N^{J'} \times M$ tương ứng. Các ánh xạ $s_\Phi$ và $s_{\Phi'}$ liên kết với các dạng song tuyến tính này được gọi là các ánh xạ liên kết trái và phải của dạng nửa song tuyến tính $\Phi$, và được ký hiệu bởi $s_\Phi$ và $d_\Phi$. Như vậy, theo định nghĩa

$$(26)$$
$$
\Phi(x, y) = \langle y, s_\Phi(x) \rangle = \langle x, d_\Phi(y) \rangle^j \quad (x \in M, y \in N),
$$

và $s_\Phi$ (tương ứng $d_\Phi$) là một ánh xạ tuyến tính từ $M^{J'}$ vào $N^*$ (tương ứng

từ $N'$ vào $M^*$). Ta dễ dàng phát biểu và chứng minh các tương tự, cho trường hợp đang xét ở đây, của Định nghĩa 7 và các mệnh đề 4, 5, 6.

### 7. Dạng nghịch đảo của một dạng song tuyến tính hoặc nửa song tuyến tính.

Cho $A$ là một vành, $E$ là một $A$-môđun trái, $F$ là một $A$-môđun phải và $\Phi$ là một dạng song tuyến tính trên $E \times F$. Ở đây ta giả sử rằng các ánh xạ liên kết với $\Phi$, được ký hiệu bởi $s$ và $d$, là *song ánh*. Khi đó ánh xạ tích $(s, d)$ là một song ánh của $E \times F$ lên $F^* \times E^*$, và xác định, bởi phép chuyển cấu trúc, một dạng song tuyến tính $\hat{\Phi}$ trên $F^* \times E^*$. Do đó dạng sau thỏa mãn

$$
(27)\quad \hat{\Phi}(y', x') = \Phi(s^{-1}(y'), d^{-1}(x')) \\
= \langle s^{-1}(y'), x' \rangle = \langle d^{-1}(x'), y' \rangle \qquad (x' \in E^*, y' \in F^*).
$$

#### Định nghĩa 8 {#alg-ix-s1-def-8 .statement}

*Cho $\Phi$ là một dạng song tuyến tính trên $E \times F$ mà các ánh xạ liên kết $s$ và $d$ là song ánh. Dạng song tuyến tính $\hat{\Phi}$ trên $F^* \times E^*$ được định nghĩa bởi (27) được gọi là dạng nghịch đảo của $\Phi$.*

Bây giờ, gọi $\hat{s}$ và $\hat{d}$ là các ánh xạ tuyến tính từ $F^*$ vào $E^{**}$ và từ $E^*$ vào $F^{**}$ liên kết ở bên trái và bên phải với $\hat{\Phi}$. Vì, với $x' \in E^*$ và $y' \in F^*$, theo định nghĩa ta có

$$
\hat{\Phi}(y', x') = \langle y', \hat{d}(x') \rangle = \langle x', \hat{s}(y') \rangle
$$

nên, bằng cách so sánh với (27), ta thấy rằng dạng tuyến tính $\hat{d}(x')$ trên $F^*$ bằng với dạng được xác định bởi phần tử $d^{-1}(x')$ của $F$. Suy ra rằng ánh xạ hợp thành $\hat{d} \circ d$ là ánh xạ chính tắc của $F$ vào đối ngẫu kép $F^{**}$ của nó, và ánh xạ này là *song ánh* vì $d$ và $\hat{d}$ (ánh xạ sau nhờ phép chuyển cấu trúc) là song ánh; do đó, nếu ta đồng nhất một cách chính tắc $F$ với $F^{**}$, ta có $\hat{d} = d^{-1}$. Tương tự $E$ được đồng nhất một cách chính tắc với $E^{**}$, ánh xạ chính tắc của $E$ vào $E^{**}$ là $\hat{s} \circ s$, và ta có $\hat{s} = s^{-1}$. Từ đó suy ra rằng dạng nghịch đảo của $\hat{\Phi}$ là $\Phi$.

Xét bây giờ một vành $A$ được trang bị một phản tự đẳng cấu $J$, hai $A$-môđun trái $E$ và $F$, và một dạng nửa song tuyến tính phải $\Phi$ đối với $J$ trên $E \times F$ sao cho các ánh xạ liên kết với $\Phi$, sẽ được ký hiệu là $s$ và $d$, là *song ánh*. Định nghĩa một ánh xạ $\widehat{\Phi}$ từ $F^* \times E^*$ vào $A$ bởi phương trình thứ nhất (27). Ánh xạ này thỏa mãn, theo (24) (No. 6), quan hệ

$$
(28)\quad \widehat{\Phi}(y', x') = \langle s^{-1}(y'), x' \rangle = \langle d^{-1}(x'), y' \rangle^J \qquad (x' \in E^*,\ y' \in F^*).
$$

Ánh xạ $\widehat{\Phi}$ hiển nhiên là $\mathbf{Z}$-song tuyến tính; hơn nữa, với $a,\ b$ trong $A$, $x' \in E^*$ và $y' \in F^*$, và theo các định nghĩa của $s$ và $d$,

$$
\widehat{\Phi}(y'a,\ x'b) = \Phi(a^j s^{-1}(y'),\ b^{j'} d^{-1}(x')) = a^j \widehat{\Phi}(y',\ x') b;
$$

do đó $\widehat{\Phi}$ là một *dạng sesquilinear trái* đối với $J$ trên $F^* \times E^*$ (No. 2).

#### Định nghĩa 9 {#alg-ix-s1-def-9 .statement}

*Cho $\Phi$ là một dạng sesquilinear phải đối với $J$ trên $E \times F$, có các ánh xạ liên kết $s$ và $d$ là song ánh. Dạng sesquilinear trái $\widehat{\Phi}$ đối với $J$ trên $F^* \times E^*$ được gọi là dạng nghịch đảo của $\Phi$.*

Ta để cho người đọc định nghĩa và nghiên cứu dạng nghịch đảo của một dạng sesquilinear trái. Dạng nghịch đảo này là một dạng sesquilinear phải.

Gọi $\widehat{s}$ và $\widehat{d}$ là các ánh xạ liên kết với $\widehat{\Phi}$; theo (26) (No. 6) ta có

$$
(29)\quad \widehat{\Phi}(y', x') = \langle y',\ \widehat{d}(x') \rangle^J = \langle x',\ \widehat{s}(y') \rangle.
$$

Vì $s$ là song ánh, và từ đẳng thức $\langle s^{-1}(y'),\ x' \rangle = \langle y',\ \widehat{d}(x') \rangle^J$ suy ra từ (28) và (29), ta suy ra rằng $\widehat{d}$ là song ánh; do đó $\widehat{d} \circ d$ là song ánh. Bây giờ đẳng thức $\langle d^{-1}(x'),\ y' \rangle = \langle y',\ \widehat{d}(x') \rangle$, suy ra từ (28) và (29), cho thấy rằng $\widehat{d} \circ d$ là ánh xạ chính tắc từ $F$ vào song đối ngẫu của nó $F^{**}$. Một cách tương tự, ta thấy rằng $\widehat{s}$ là song ánh và rằng $\widehat{s} \circ s$ là ánh xạ chính tắc từ $E$ vào $E^{**}$. Do đó, nếu đồng nhất $E^{**}$ với $E$ và $F^{**}$ với $F$ nhờ các ánh xạ chính tắc này, ta có $\widehat{s} = s^{-1},\ \widehat{d} = d^{-1}$, và $\Phi$ là dạng nghịch đảo của $\widehat{\Phi}$.

Với cùng ký hiệu và giả thiết, cho $a$ là một phần tử khả nghịch của tâm của $A$. Khi đó các ánh xạ liên kết của dạng $a\Phi$ là, theo (23) (tương ứng (24)), bằng $a.d$ và $a.s$ (tương ứng $a^{J'}.s$), và do đó là song ánh. Vì vậy, từ (27) suy ra rằng dạng nghịch đảo của $a\Phi$ là $a^{-1}\widehat{\Phi}$ (tương ứng $(a^{J'})^{-1}\widehat{\Phi}$).

### 8. Dạng phụ hợp của một đồng cấu.

Trong Số này, $A$ ký hiệu một vành (tương ứng, một vành được trang bị một phản tự đẳng cấu $J$), $E$ và $E'$ là hai $A$-môđun trái, $F$ và $F'$ là hai $A$-môđun phải (tương ứng, trái), và $\Phi$ và $\Phi'$ là hai dạng song tuyến tính (tương ứng, dạng sesquilinear đối với $J$) trên $E \times F$ và $E' \times F'$ tương ứng. Giả sử rằng $\Phi$ là không suy biến, nói cách khác (No. 1) rằng các ánh xạ tuyến tính $d_{\Phi}$ và $s_{\Phi}$ liên kết với $\Phi$ là đơn ánh.

Cho một đồng cấu $u$ từ E vào E’, xét tập hợp $F'_1$ gồm các phần tử $y'$ của $F'$ sao cho tồn tại $y \in F$ mà ta có $d_{\Phi'}(y') \circ u = d_{\Phi}(y)$, nghĩa là $\Phi'(u(x), y') = \Phi(x, y)$ với mọi $x \in E$. Rõ ràng rằng $F'_1$ là một môđun con của $F'$. Vì $d_{\Phi}$ là đơn ánh, nên với mỗi $y' \in F'_1$, tồn tại duy nhất một phần tử $y$ của F sao cho $\Phi'(u(x), y') = \Phi(x, y)$. Ánh xạ $y' \to y$ từ $F'_1$ vào F được xác định như vậy là A-tuyến tính; ký hiệu nó là $u^*$, ta có, với mọi $x \in E$ và mọi $y \in F'_1$

$$
\Phi'(u(x), y') = \Phi(x, u^*(y')).
$$

#### Định nghĩa 10 {#alg-ix-s1-def-10 .statement}

Với các giả thiết và ký hiệu như trước, ta nói rằng đồng cấu $u^*$ từ $F'_1$ vào F thỏa mãn (30) là liên hợp trái của $u$, và rằng $F'_1$ là môđun con xác định của $u^*$.

Liên hợp phải của một đồng cấu $\varphi$ từ F vào $F'$ được định nghĩa tương tự bởi công thức

$$
\Phi'(x', \varphi(y)) = \Phi(\varphi^*(x'), y) \quad (x' \in E'_1, y \in F),
$$

trong đó $E'_1$ ký hiệu môđun con của $E'$ được định nghĩa tương tự như $F'_1$.

#### Nhận xét {#alg-ix-s1-n8-rem-1 .statement}

Nếu liên hợp trái $u^*$ của $u : E \to E'$ được xác định khắp nơi, và nếu $s_{\Phi'}$ và $d_{\Phi'}$ là đơn ánh, công thức (30) chỉ ra rằng $u$ là liên hợp phải của $u^*$.

Suy ra từ (30) rằng, nếu $u_1$ và $u_2$ là hai đồng cấu từ $E$ vào $E'$ có các liên hợp được xác định khắp nơi, và nếu $c$ là một phần tử của tâm của $A$, ta có

$$
\begin{cases}
(u_1 + u_2)^* = u_1^* + u_2^* ; 1^* = 1 ; \\
(cu_1)^* = c . u_1^* \text{ khi } \Phi \text{ và } \Phi' \text{ là song tuyến tính ;} \\
(cu_1)^* = c^{j'} . u_1^* \text{ khi } \Phi \text{ và } \Phi' \text{ là nửa song tuyến tính.}
\end{cases}
$$

Hơn nữa, nếu $E''$ là một A-môđun trái thứ ba, $F''$ là một A-môđun phải thứ ba (tương ứng môđun trái), $\Phi''$ là một dạng song tuyến tính (tương ứng nửa song tuyến tính đối với $J$) trên $E'' \times F''$, và nếu $u'$ là một đồng cấu từ $E'$ vào $E''$ thừa nhận một tự đồng cấu liên hợp trái xác định khắp nơi, thì ta có

$$(u' \circ u)^* = u^* \circ {u'}^*.$$

Đặc biệt, nếu $u$ là một *đẳng cấu* của $E$ lên $E'$, và nếu các ánh xạ liên hợp $u^*$ và $(u^{-1})^*$ đều xác định khắp nơi, thì $u^*$ là một đẳng cấu của $F'$ lên $F$, và ta có $(u^*)^{-1} = (u^{-1})^*$. Các tính chất tương tự đối với các ánh xạ liên hợp phải.

#### Mệnh đề 7 {#alg-ix-s1-prop-7 .statement}

Với cùng các ký hiệu như trước, giả sử rằng $d_{\Phi}$ là song ánh. Khi đó mọi đồng cấu $u$ của $E$ vào $E'$ đều thừa nhận một ánh xạ liên hợp trái xác định khắp nơi, và ta có $u^* = (d_{\Phi})^{-1} \circ {}^t u \circ d_{\Phi'}$.

Thật vậy, vì $d_{\Phi}$ là song ánh, ta có, với các ký hiệu ở đầu No., $F'_1 = F'$, và do đó $u^*$ xác định khắp nơi. Mặt khác (30) tương đương với

$$\langle u(x), d_{\Phi'}(y') \rangle = \langle x, (d_{\Phi} \circ u^*)(y') \rangle \quad (x \in E, y' \in F');$$

bây giờ $\langle d_{\Phi'}(y'), u(x) \rangle = \langle {}^t u(d_{\Phi'}(y')), x \rangle$; do đó ta có ${}^t u(d_{\Phi'}(y')) = d_{\Phi}(u^*(y'))$ với mọi $y' \in F'$, do đó ${}^t u \circ d_{\Phi'} = d_{\Phi} \circ u^*$, và do đó biểu thức đã công bố của $u^*$. Q.E.D.

#### Nhận xét {#alg-ix-s1-n8-rem-2 .statement}

Khi $s_{\Phi}$ là song ánh, mọi đồng cấu $\nu$ của $F$ vào $F'$ đều thừa nhận một ánh xạ liên hợp phải xác định khắp nơi, và ta có

$$(34)$$
$$\nu^* = (s_{\Phi})^{-1} \circ {}^t \nu \circ s_{\Phi'}.$$

#### Mệnh đề 8 {#alg-ix-s1-prop-8 .statement}

Với cùng các ký hiệu như trước, giả sử rằng $s_{\Phi}$ và $d_{\Phi}$ là song ánh. Cho $u$ và $\nu$ lần lượt là các đẳng cấu của E lên E' và của F lên F'. Khi đó, để Φ là ảnh ngược của Φ' đối với u và v (nghĩa là ta có Φ(x, y) = Φ'(u(x), v(y)) với mọi x ∈ E, y ∈ F), điều kiện cần và đủ là ta có u^{-1} = v^* và v^{-1} = u^*.

Thật vậy Φ'(u(x), v(y)) = Φ(x, y) cũng có thể được viết là Φ (x, u^*(v(y))) = Φ(x, y). Nếu điều này đúng với mọi x ∈ E và y ∈ F, ta có u^* ∘ v = 1 vì Φ là không suy biến. Do đó ta cũng có v^* ∘ u = 1 theo (33). Điều đảo lại là ngay lập tức.

#### Hệ quả {#alg-ix-s1-n8-cor-1 .statement}

Cho A là một vành được trang bị một tự đẳng cấu phản $J$, E là một A-môđun trái, Φ là một dạng nửa song tuyến tính đối với $J$ trên E × E mà các ánh xạ liên kết của nó là song ánh, và u là một tự đẳng cấu của A-môđun E. Để u giữ bất biến Φ (nghĩa là ta có Φ(u(x), u(y)) = Φ(x, y) với mọi x, y trong E), điều kiện cần và đủ là hai ánh xạ liên hợp của u bằng nhau và ta có u^* = u^{-1}.

Điều này suy ra ngay lập tức từ mệnh đề 8.

#### Nhận xét {#alg-ix-s1-n8-rem-3 .statement}

Dưới các giả thiết của hệ quả của mệnh đề 8, giả sử thêm rằng A là một trường và E có số chiều hữu hạn trên A. Cho ω là một tự đồng cấu của E, ω_1 và ω_2 là các ánh xạ liên hợp phải và trái của nó. Mỗi điều kiện ωω_1 = 1, ωω_2 = 1, ω_1ω = 1, ω_2ω = 1 kéo theo rằng ω là một tự đẳng cấu của E giữ Φ bất biến, và rằng ω_1 = ω_2.

### 9. Các tích tenxơ và lũy thừa ngoài của các dạng nửa song tuyến tính.

Trong No. này, A sẽ chỉ một vành giao hoán. Một dạng song tuyến tính trên tích của hai A-môđun do đó là một trường hợp riêng của một dạng nửa song tuyến tính. Ta sẽ ký hiệu J là một tự đẳng cấu của A, và J' là nghịch đảo của nó.

Cho E_i (i = 1, ..., m) là các A-môđun. Ánh xạ

$$(x_1, ..., x_m) \to x_1 \otimes \cdots \otimes x_m$$

của $\prod_{i=1}^m E_i^J$ vào $(\bigotimes_{i=1}^m E_i)^J$ (x_i \in E_i^J) (xem định. 5, n° 2) hiển nhiên là A-đa tuyến tính; do đó nó xác định (chương III, § 1, n° 7) một ánh xạ A-tuyến tính $f$ của $\bigotimes_i E_i^j$ vào $(\bigotimes_i E_i)^j$; ánh xạ này biến $x_1 \otimes \cdots \otimes x_m$ (trong đó các dấu $\otimes$ chỉ các tích tenxơ trong $\bigotimes_i E_i^j$) thành $x_1 \otimes \cdots \otimes x_m$ (trong đó các dấu $\otimes$ chỉ các tích tenxơ trong $(\bigotimes_i E_i)^j$). Như vậy $f$ là một đẳng cấu của $\bigotimes_i E_i^j$ lên $(\bigotimes_i E_i)^j$. Ta sẽ đồng nhất hai môđun này bằng đẳng cấu này.

Tương tự, cho $E$ là một A-môđun. Ánh xạ
$$
(x_1, \ldots, x_m) \to x_1 \wedge \ldots \wedge x_m
$$
từ $(E^j)^m$ vào $(\wedge^m E)^j$ hiển nhiên là A-đa tuyến tính và phản xứng. Do đó nó xác định một ánh xạ A-tuyến tính $f$ từ $\wedge^m E^j$ vào $(\wedge^m E)^j$, ánh xạ này hiển nhiên là một đẳng cấu. Ta sẽ đồng nhất $\wedge^m E^j$ và $(\wedge^m E)^j$ bằng đẳng cấu này.

Cho $x'$ là một phần tử của đối ngẫu $E^*$ của $E$. Ánh xạ $x \to \langle x, x' \rangle^j$ ($x \in E$) là một phần tử ${x'}^j$ của $(E^j)^*$, và hiển nhiên $x' \to {x'}^j$ là một song ánh $g$ từ $E^*$ lên $(E^j)^*$ thỏa mãn $g(ax') = a^j g(x')$ với mọi $a \in A$. Do đó ánh xạ hợp thành của $g$ và ánh xạ đồng nhất của $(E^*)^j$ lên $E^*$ là một đẳng cấu của $(E^*)^j$ lên $(E^j)^*$. Ta sẽ đồng nhất các môđun này bằng đẳng cấu này, và sẽ ký hiệu chúng bởi $E_j^*$.

Cho $E_i, F_i \ (i = 1, \ldots, m)$ là các A-môđun, và $\Phi_i \ (i = 1, \ldots, m)$ là một dạng nửa song tuyến tính đối với $J$ trên $E_i \times F_i$. Ánh xạ
$$
(x_1, \ldots, x_m, y_1, \ldots, y_m) \to \Phi_1(x_1, y_1) \Phi_2(x_2, y_2) \ldots \Phi_m(x_m, y_m)
$$
$(x_i \in E_i, y_i \in F_i, i = 1, \ldots, m)$ là một ánh xạ A-đa tuyến tính từ $E_1 \times \cdots \times E_m \times F_1^j \times \cdots \times F_m^j$ vào $A$, và do đó xác định một dạng song tuyến tính trên $(\bigotimes_i E_i) \times (\bigotimes_i F_i^j)$ (Chap. III, § 1, No. 7). Vì nhân tử thứ hai đã được đồng nhất với $(\bigotimes_i F_i)^j$, nên ta đã xác định một dạng nửa song tuyến tính $\Phi$ đối với $J$ trên $(\bigotimes_i E_i) \times (\bigotimes_i F_i)$. Dạng này được đặc trưng bởi
$$
\Phi(x_1 \otimes \cdots \otimes x_m, y_1 \otimes \cdots \otimes y_m) = \prod_{i=1}^m \Phi_i(x_i, y_i) \quad (x_i \in E_i, y_i \in F_i).
$$

#### Định nghĩa 11 {#alg-ix-s1-def-11 .statement}

Cho các A-môđun $E_i, F_i (i = 1, \ldots, m)$ và, với mỗi $i$, một dạng nửa song tuyến tính $\Phi_i$ đối với $J$ trên $E_i \times F_i$, dạng nửa song tuyến tính $\Phi$ đối với $J$ trên $(\bigotimes_i E_i) \times (\bigotimes_i F_i)$ được đặc trưng bởi (35) được gọi là tích tenxơ của các dạng nửa song tuyến tính $\Phi_i$.

Trong trường hợp các $E_i$ và các $F_i$ đều bằng cùng một môđun $E$, và các $\Phi_i$ đều bằng cùng một dạng $\Psi$, ta nói rằng $\Phi$ là sự mở rộng của $\Psi$ lên $\bigotimes^m E$.

Với các ký hiệu của Định nghĩa 11, ta hãy nghiên cứu các ánh xạ liên kết với $\Phi$. Từ công thức (24) (No. 6) và từ (35) ta thu được quan hệ

$$
\Phi(x_1 \otimes \cdots \otimes x_m, y_1 \otimes \cdots \otimes y_m) = \prod_{i=1}^m \langle x_i, d_{\Phi_i}(y_i) \rangle = \prod_{i=1}^m \langle y_i, s_{\Phi_i}(x_i) \rangle^J.
$$

Do đó ta có:

(36) $s_\Phi = j_s \circ (s_{\Phi_1} \otimes \cdots \otimes s_{\Phi_m}), \quad d_\Phi = j_d \circ (d_{\Phi_1} \otimes \cdots \otimes d_{\Phi_m})$

trong đó $j_s$ (tương ứng $j_d$) là ánh xạ chính tắc của $\bigotimes_i F_i^*$ vào $(\bigotimes_i F_i)^*$ (tương ứng của $\bigotimes_i E_i^*$ vào $(\bigotimes_i E_i)^*$) (Chương III, § 1, Số 4 và 7).

#### Mệnh đề 9 {#alg-ix-s1-prop-9 .statement}

Cho $A$ là một trường giao hoán được trang bị một tự đẳng cấu $J$, $E_i, F_i$ là các không gian vectơ hữu hạn chiều trên $A$, và $\Phi_i$ là một dạng sesquilinear đối với $J$ trên $E_i \times F_i$ ($1 \leqslant i \leqslant m$). Nếu các dạng $\Phi_i$ không suy biến, thì điều tương tự cũng đúng đối với tích tenxơ $\Phi$ của chúng. Trong trường hợp này dạng nghịch đảo $\widehat{\Phi}$ của $\Phi$ là tích tenxơ của các dạng nghịch đảo $\widehat{\Phi}_i$.

Thật vậy, vì $A$ là một trường, suy ra từ các mệnh đề 6 và 7 của chương III, § 1, no. 3 rằng tích tenxơ của các ánh xạ tuyến tính đơn ánh (tương ứng toàn ánh) của các $A$-môđun là một ánh xạ tuyến tính đơn ánh (tương ứng toàn ánh). Vì các $s_{\Phi_i}$ là song ánh theo giả thiết (mệnh đề 6, no. 6), nên điều tương tự cũng đúng đối với tích tenxơ của chúng. Mặt khác ánh xạ chính tắc $j_s$ của $\bigotimes_i F_i^*$ vào $(\bigotimes_i F_i)^*$ là song ánh (chương III, § 1, no. 5, mệnh đề 11). Do đó, theo (36), $s_\Phi$ là song ánh, và điều này chứng minh mệnh đề đầu tiên của chúng ta (mệnh đề 6, no. 6). Tương tự $d_\Phi$ là song ánh.

Trong mệnh đề thứ hai, ta đã ngầm đồng nhất $\bigotimes_i F_i^*$ với $(\bigotimes_i F_i)^*$ và $\bigotimes_i E_i^*$ với $(\bigotimes_i E_i)^*$ bằng các ánh xạ $j_s$ và $j_d$, vốn ở đây là các đẳng cấu. Các dạng nghịch đảo trong mệnh đề tồn tại vì các $s_{\Phi_i}$, các $d_{\Phi_i}$, $s_\Phi$ và $d_\Phi$ là các song ánh (no. 7). Khi đó đặt $x' = x'_1 \otimes \cdots \otimes x'_m$, $y' = y'_1 \otimes \cdots \otimes y'_m$ ($x'_i \in E_i^*$, $y'_i \in F_i^*$, $i = 1, \ldots, m$). Theo định nghĩa của các dạng nghịch đảo, và xét (36), ta có

$$
\widehat{\Phi}(j_s(y'), j_d(x')) = \Phi(s_{\Phi_1}^{-1}(y'_1) \otimes \cdots \otimes s_{\Phi_m}^{-1}(y'_m), d_{\Phi_1}^{-1}(x'_1) \otimes \cdots \otimes d_{\Phi_m}^{-1}(x'_m))
$$
$$
= \prod_{i=1}^m \Phi_i(s_{\Phi_i}^{-1}(y'_i), d_{\Phi_i}^{-1}(x'_i)) = \prod_{i=1}^m \widehat{\Phi}_i(y'_i, x'_i),
$$

do đó có mệnh đề thứ hai của chúng ta.

C. Q. F. D.

Cho E và F là hai môđun trên vành giao hoán A, và $\Phi$ là một dạng sesquilinear đối với $J$ trên $E \times F$. Ánh xạ
$$
(x_1, \ldots, x_m, y_1, \ldots, y_m) \to \det(\Phi(x_i, y_k)) \quad (x_i \in E, y_i \in F, i = 1, \ldots, m)
$$
của $E^m \times (F^j)^m$ vào A là A-song tuyến tính. Do đó nó xác định một dạng song tuyến tính $\Phi'$ trên $(\bigotimes^m E) \times (\bigotimes^m F^j)$ được đặc trưng bởi
$$
\Phi'(x_1 \otimes \cdots \otimes x_m, y_1 \otimes \cdots \otimes y_m) = \det(\Phi(x_i, y_k)).
$$
Vì phần tử thứ nhất bằng không khi $x_i = x_k$ hoặc khi $y_i = y_k$ ($i \neq k$), $\Phi'$ xác định, bằng cách chuyển qua các thương, một dạng song tuyến tính trên $(\wedge^m E) \times (\wedge^m F^j)$, hay một lần nữa, vì $\wedge^m F^j$ được đồng nhất với $(\wedge^m F)^j$, một dạng sesquilinear $\Phi_{(m)}$ đối với J trên $(\wedge^m E) \times (\wedge^m F)$. Dạng này được đặc trưng bởi
$$
\left\{
\begin{array}{l}
\Phi_{(m)}(x_1 \wedge \ldots \wedge x_m, y_1 \wedge \ldots \wedge y_m) = \det(\Phi(x_i, y_k)) \\
(x_i \in E, y_i \in F, i = 1, \ldots, m).
\end{array}
\right.
$$
(37)

#### Định nghĩa 12 {#alg-ix-s1-def-12 .statement}

Cho hai A-môđun E, F và một dạng $\Phi$ sesquilinear đối với J trên $E \times F$, dạng $\Phi_{(m)}$ sesquilinear đối với J trên $(\wedge^m E) \times (\wedge^m F)$ được đặc trưng bởi (37) được gọi là mở rộng của $\Phi$ tới các lũy thừa ngoài bậc m.

Với các ký hiệu là những ký hiệu của Định nghĩa 12, ta hãy nghiên cứu các ánh xạ liên kết với $\Phi_{(m)}$. Từ công thức (24) (No. 6) và (37) ta thu được các hệ thức

$$
\Phi_{(m)}(x_1 \wedge \ldots \wedge x_m, y_1 \wedge \ldots \wedge y_m) = \det(\langle x_i, d_\Phi(y_k) \rangle)
= \det(\langle y_i, s_\Phi(x_k) \rangle^j).
$$

Do đó ta có

$$
s_{\Phi(m)} = k_s \circ (\wedge^m s_\Phi), \quad d_{\Phi m} = k_d \circ (\wedge^m d_\Phi),
$$

trong đó $k_s$ (tương ứng $k_d$) ký hiệu ánh xạ chính tắc của $\wedge^m F^*$ vào $(\wedge^m F)^*$ (tương ứng của $\wedge^m E^*$ vào $(\wedge^m E)^*$) (xem Chương III, § 8, No. 2).

#### Mệnh đề 10 {#alg-ix-s1-prop-10 .statement}

*Cho A là một trường giao hoán được trang bị một tự đẳng cấu J, E và F là hai không gian vectơ hữu hạn chiều trên A, và $\Phi$ là một dạng sesquilinear đối với J trên $E \times F$. Nếu $\Phi$ không suy biến, thì mở rộng $\Phi_{(m)}$ của nó tới các lũy thừa ngoài bậc m là không suy biến, và dạng nghịch đảo của $\Phi_{(m)}$ là mở rộng tới các lũy thừa ngoài bậc m của dạng nghịch đảo $\widehat{\Phi}$ của $\Phi$.*

Thật vậy, vì $s_\Phi$ và $d_\Phi$ là song ánh theo giả thiết (Mệnh đề 6, No. 6), điều tương tự cũng đúng đối với các lũy thừa ngoài của chúng (Chương III, § 5, No. 7). Mặt khác các ánh xạ chính tắc $k_s$ và $k_d$ là song ánh (Chương III, § 8, No. 2, Định lý 1). Do đó, theo (38), $s_{\Phi(m)}$ và $d_{\Phi(m)}$ là song ánh, điều này chứng minh rằng $\Phi_{(m)}$ là không suy biến (Mệnh đề 6, No. 6). Trong mệnh đề thứ hai ta đã ngầm đồng nhất $\wedge^m F^*$ với $(\wedge^m F)^*$ và $\wedge^m E^*$ với $(\wedge^m E)^*$ bằng các ánh xạ $k_s$ và $k_d$, vốn ở đây là các đẳng cấu (*loc. cit.*). Các dạng nghịch đảo được xét trong mệnh đề tồn tại vì $s_\Phi, d_\Phi, s_{\Phi(m)}, d_{\Phi(m)}$ là các song ánh (No. 7). Khi đó đặt $x' = x'_1 \wedge \ldots \wedge x'_m$ và $y' = y'_1 \wedge \ldots \wedge y'_m$ ($x'_i \in E^*, y'_i \in F^*, i = 1, \ldots, m$). Theo định nghĩa của các dạng nghịch đảo (No. 7) và theo (38), ta có

$$
\widehat{\Phi}_{(m)}(k_s(y'), k_d(x')) = \Phi_{(m)}(s^{-1}_\Phi(y'_1) \wedge \ldots \wedge s^{-1}_\Phi(y'_m), d^{-1}_\Phi(x'_1) \wedge \ldots \wedge d^{-1}_\Phi(x'_m))
= \det(\Phi(s^{-1}_\Phi(y'_i), d^{-1}_\Phi(x'_k))) = \det(\widehat{\Phi}(y'_i, x'_k))
$$

do đó có khẳng định thứ hai.

#### Nhận xét {#alg-ix-s1-n9-rem-1 .statement}

Cho E là một A-môđun tự do, và cho θ là đẳng cấu chính tắc của $\bigwedge^m E$ lên môđun con gồm các tenxơ phản đối xứng hóa cấp m (Chương III, § 5, No. 6, Mệnh đề 6). Cho $\Phi$ là một dạng sesquilinear trên E, $\Phi_{(m)}$ là mở rộng của $\Phi$ lên $\bigwedge^m E$, và $\Theta$ là dạng sesquilinear trên $\bigwedge^m E$ là ảnh ngược bởi $\theta$ của mở rộng của $\Phi$ lên $\bigotimes^m E$. Từ định nghĩa của $\theta$ và của tenxơ phản đối xứng hóa, và từ (35), ta có

$$
\Theta(x_1 \wedge \ldots \wedge x_m, y_1 \wedge \ldots \wedge y_m) = \sum_{\sigma, \tau} \varepsilon_\sigma \varepsilon_\tau \Phi(x_{\sigma(1)}, y_{\tau(1)}) \ldots \Phi(x_{\sigma(m)}, y_{\tau(m)})
$$

trong đó $\sigma$ và $\tau$ chạy qua nhóm đối xứng $S_m$. Từ công thức tính các định thức và công thức (37), biểu thức này có thể được viết

$$
\sum_{\tau \in S_m} \varepsilon_\tau \det(\Phi(x_i, y_{\tau(k)})) = m! \det(\Phi(x_i, y_k));
$$

nói cách khác, ta có $\Theta = m! \Phi_{(m)}$.

### 10. Các phép tính ma trận.

Trong No. hiện tại, ta đề xuất làm cho phép tính ma trận được đưa vào trong Chương II, § 6, linh hoạt hơn, và áp dụng nó để chuyển dịch một số kết quả đã được chứng minh trong đoạn này.

I. — Cho I và K là hai tập hợp hữu hạn các chỉ số, H là một tập hợp khác rỗng, và $M = (m_{ik})_{(i,k) \in I \times K}$ là một ma trận trên H (Chương II, § 6, No. 1, Định nghĩa 1).

Ma trận chuyển vị của $M$ được gọi là, và ký hiệu bởi ${}^tM$, ma trận $(m'_{ki})_{(k,i) \in K \times I}$ thỏa mãn $m'_{ki} = m_{ik} \ ((i, k) \in I \times K)$. Hiển nhiên ta có

$$(39)$$
$$
{}^t({}^tM) = M.
$$

Điều này tổng quát hóa khái niệm được đưa vào trong Chương II, § 6, No. 6.

Giả sử rằng H là một nhóm giao hoán (được viết cộng tính). Tập hợp các ma trận trên H có I và K làm các tập hợp chỉ số có một cấu trúc nhóm giao hoán, vì nó là tập hợp các ánh xạ từ $I \times K$ vào H. Nhóm này được viết cộng tính.

Cho $H', H''$ là hai tập hợp khác rỗng, $H$ là một nhóm giao hoán (được viết cộng tính) và $f : (h', h'') \to h'h''$ là một ánh xạ từ $\mathbf{H}' \times \mathbf{H}''$ vào $\mathbf{H}$. Cho hai ma trận
$$
M' = (m_{ik}')_{(i,k) \in I \times K}, \qquad M'' = (m_{kl}'')_{(k,l) \in K \times L}
$$
trên $\mathbf{H}'$ và $\mathbf{H}''$ tương ứng, sao cho tập hợp $K$ các chỉ số của các cột của $M'$ bằng tập hợp các chỉ số của các hàng của $M''$, người ta gọi *tích* của $M'$ và $M''$ (theo $f$) và ký hiệu bởi $M'M''$ ma trận
$$
M'.M'' = (\sum_{k \in K} m_{ik}' m_{kl}'' )_{(i,l) \in I \times L}
$$
trên $\mathbf{H}$. Điều này tổng quát hóa khái niệm được đưa vào trong Chương II, § 6, No. 4.
Nếu $\mathbf{H}' = \mathbf{H}'' = \mathbf{H}$ và nếu $\mathbf{H}$ là một vành, tích $M'M''$ sẽ, trừ khi có nói rõ khác đi, được tính “trong $\mathbf{H}$”, nghĩa là theo ánh xạ $(x, y) \to xy$. Khi $\mathbf{H}'$ và $\mathbf{H}''$ là các nhóm giao hoán (được viết cộng tính) và $f$ là song tuyến tính, ta có
$$
\left\{
\begin{array}{l}
(M' + M'_1)M'' = M'M'' + M'_1M'', \\
M'(M'' + M''_1) = M'M'' + M'M''_1,
\end{array}
\right.
$$
trong đó $M', M'_1$ là các ma trận trên $\mathbf{H}'$, $M'', M''_1$ là các ma trận trên $\mathbf{H}''$, và trong đó các tổng và tích được viết được giả sử là đã được xác định. Cho $M', M''$ là các ma trận trên các tập hợp $\mathbf{H}', \mathbf{H}''$, và $f^0$ là ánh xạ từ $\mathbf{H}'' \times \mathbf{H}'$ vào $\mathbf{H}$ được xác định bởi $(h'', h') \to h'h''$; khi đó ta có
$$
t(M'M'') = tM'' . tM'
$$
trong đó tích ở vế thứ nhất (tương ứng thứ hai) được tính theo $f$ (tương ứng $f^0$).

Trong trường hợp $\mathbf{H}' = \mathbf{H}'' = \mathbf{H}$ là một vành, ta thu lại công thức (12) của Chương II, § 6, No. 6.

Cho $A$ là một vành, $J$ là một phản tự đẳng cấu của $A$. Với mọi ma trận $M = (m_{ik})$ trên $A$, ta sẽ ký hiệu bởi $M^J$ ma trận $(m_{ik}^J)$. Cho $M_1, M_2$ là hai ma trận trên $A$ sao cho $M_1M_2$ được xác định. Vì $J$ là một đẳng cấu của $A$ lên vành đối $A^0$, ta có $(M_1M_2)^J = M_1^J . M_2^J$ trong đó vế thứ nhất (tương ứng thứ hai) được tính trong $A$ (tương ứng $A^0$). Xét (42) và (39), điều này cho
$$
(M_1M_2)^J = t(tM_2^J . tM_1^J)
$$
trong đó *hai* vế được tính trong $A$.

Bourbaki XXIV.

Cho $H_1, H_2, H_3, H_{12}, H_{23}$ và $H$ là các nhóm giao hoán (được ký hiệu cộng tính), $f_{12} : H_1 \times H_2 \to H_{12}$, $f_{23} : H_2 \times H_3 \to H_{23}$, $f_3 : H_{12} \times H_3 \to H$, $f_1 : H_1 \times H_{23} \to H$ là các ánh xạ, và cho $M_1, M_2, M_3$ là các ma trận trên $H_1, H_2, H_3$ tương ứng. Nếu $f_3(f_{12}(x_1, x_2), x_3) = f_1(x_1, f_{23}(x_2, x_3))$ với mọi $x_i \in H_i$ ($i = 1, 2, 3$), thì các tích $(M_1 M_2) M_3$ và $M_1 (M_2 M_3)$ (được tính theo $f_{12}, f_3, f_{23}$ và $f_1$), nếu được xác định, là bằng nhau; ta sẽ ký hiệu chúng là $M_1 M_2 M_3$. Khi $H_1 = H_2 = H_3 = H_{12} = H_{23} = H$, $H$ là một vành, và $f_{12}, f_{23}, f_3, f_1$ đều bằng ánh xạ $(x, y) \to xy$, điều kiện trước biểu thị tính kết hợp của ánh xạ sau, và do đó được thỏa mãn. Ta sẽ dùng các quy ước tương tự cho các tích của nhiều hơn ba thừa số.

Cho $A, B$ là hai vành, $M = (m_{ik})_{(i,k) \in I \times K}$ và $M' = (m'_{ik})_{(i,k) \in I \times K}$ là hai ma trận trên một song môđun $(A, B)$- $G$ (No. 1). Nếu, với mọi ma trận một hàng $L = (a_i)_{i \in I}$ có các phần tử trong $A$ và mọi ma trận một cột $C = (b_k)_{k \in K}$ có các phần tử trong $B$, ta có $L . M . C = L . M' . C$ (các tích được tính theo các ánh xạ xác định cấu trúc song môđun $(A, B)$ của $G$), thì các ma trận $M$ và $M'$ bằng nhau. Thật vậy, nếu lấy $a_i = 1, a_s = 0$ với $s \neq i$, $b_k = 1, b_t = 0$ với $t \neq k$, thì các ma trận $L . M . C$ và $L . M' . C$, là các ma trận vô hướng, lần lượt bằng $m_{ik}$ và $m'_{ik}$.

II. — Xét một vành $A$ và một $A$-môđun (phải hoặc trái) $E$, có một cơ sở hữu hạn $(e_i)_{i \in I}$. Với mọi phần tử $x$ của $E$, ta gọi ma trận của $x$ đối với cơ sở $(e_i)$, và ký hiệu là $M(x)$ hoặc $x$, là ma trận một cột tạo bởi các thành phần $x_i$ ($i \in I$) của $x$ đối với $(e_i)$ (xem Chương II, § 6, No. 4); trong các phép tính, để nhắc lại rằng chỉ số $i$ là một chỉ số hàng, sẽ thuận tiện khi gắn thêm cho nó một chỉ số cột chỉ có thể nhận một giá trị, và viết $(x_{i0})$ là ma trận $M(x)$.

Xét hai $A$-môđun (trái hoặc phải) $E$ và $F$, có các cơ sở hữu hạn lần lượt là $(e_i)_{i \in I}$ và $(f_k)_{k \in K}$; gọi $(f_k^*)$ là cơ sở đối ngẫu của $F^*$ đối với $(f_k)$. Ta sẽ định nghĩa ma trận, đối với các cơ sở này, của một ánh xạ $u$ từ $E$ vào $F$ trong bốn trường hợp sau:

(D) $E$ và $F$ là các môđun phải, $u$ là $A$-tuyến tính ;

(G) E và F là các môđun trái, u là A-tuyến tính ;
(GD) E là một môđun trái, F là một môđun phải, A được trang bị một phản tự đẳng cấu J, u là $\mathbf{Z}$-tuyến tính và thỏa mãn $u(ax) = u(x)a^J$ ($a \in A,\ x \in E$) (nói cách khác u là một ánh xạ A-tuyến tính từ $E^J$ vào F (no 2, định nghĩa 5)).
(DG) E là một A-môđun phải, F là một A-môđun trái, A được trang bị một tự đẳng cấu J, u là $\mathbf{Z}$-tuyến tính và thỏa mãn $u(xa) = a^Ju(x)$ ($x \in E,\ a \in A$) (nói cách khác u là một ánh xạ A-tuyến tính từ $E^J$ vào F).
Trong mỗi trường hợp trong bốn trường hợp này, ma trận của ánh xạ u, theo định nghĩa, là ma trận $(u_{ki})_{(k,i) \in \mathbb{K} \times I}$ sao cho
$$
u_{ki} = \langle u(e_i), f_k^* \rangle.
$$
Định nghĩa này trùng với, trong trường hợp (D), định nghĩa đã cho trong chap. II, § 6, no 3. Với các điều kiện này, ma trận $M(u(x))$ của ảnh của một phần tử x của E được cho bởi các công thức sau:
$$
\begin{align*}
(45\ D)\quad &M(u(x)) = M(u) \cdot M(x) \\
(45\ G)\quad &{}^tM(u(x)) = {}^tM(x) \cdot {}^tM(u) \\
(45\ GD)\quad &M(u(x)) = M(u) \cdot M(x)^J \\
(45\ DG)\quad &{}^tM(u(x)) = {}^tM(x)^J \cdot {}^tM(u).
\end{align*}
$$
Ta hãy kiểm tra, chẳng hạn (45 DG), các kiểm tra khác là tương tự và dễ hơn một chút. Đặt $x = \sum e_ix_{io}$, $u(x) = \sum y_{ko}f_k$; ta có $u(x) = u(\sum e_ix_{io}) = \sum x_{io}^ju(e_i) = \sum x_{io}^ju_{ki}/k$; do đó $y_{ko} = \sum x_{io}^ju_{ki}$; để đặt hai chỉ số i cạnh nhau, xét các ma trận chuyển vị ${}^tM(x) = (x'_{oi})$ trong đó $x'_{oi} = x_{io}$, và ${}^tM(u) = (u'_{ik})$ trong đó $u'_{ik} = u_{ki}$; khi đó ta có $y_{ko} = \sum x'_{oi}u'_{ik}$; vì vế thứ hai là phần tử có chỉ số k của ma trận một hàng ${}^tM(x)^J \cdot {}^tM(u)$, công thức (45 DG) được kiểm tra.

#### Nhận xét 1 {#alg-ix-s1-n10-rem-1 .statement}

Khi A là giao hoán, (45 G) thu gọn về (45 D), và (45 DG) về (45 GD), nhờ công thức ${}^t(M'M'') = {}^tM'' \cdot {}^tM'$ (xem (42)), trong đó hai vế ở đây được tính trong A.
2) Cho E, F, G là ba môđun trái có các cơ sở hữu hạn, và $u : E \to F,\ v : F \to G$ là các ánh xạ A-tuyến tính. Từ (45 G) suy ra rằng ta có
$$
{}^tM(v \circ u) = {}^tM(u) \cdot {}^tM(v).
$$

Thật vậy, với mọi $x \in E$,

$$
{}^t M(x) \cdot {}^t M(\varphi \circ u) = {}^t M(\varphi(u(x))) = {}^t M(u(x)) \cdot {}^t M(\varphi)
= {}^t M(x) \cdot {}^t M(u) \cdot {}^t M(\varphi),
$$

do đó (46).

Nhắc lại rằng, trong trường hợp các môđun phải, ta có

$$
M(\varphi \circ u) = M(\varphi) M(u).
$$

III. — Từ nay về sau ta sẽ ký hiệu A là một vành, B là một vành (tương ứng một vành được trang bị một phản tự đẳng cấu J, với ký hiệu $J' = J^{-1}$), E là một A-môđun trái có cơ sở hữu hạn $(e_i)_{i \in I}$, và F là một B-môđun phải (tương ứng trái) có cơ sở hữu hạn $(f_k)_{k \in K}$. Ta ký hiệu $(e_i^*)$ và $(f_k^*)$ là các cơ sở đối ngẫu của E* và F*. Trừ khi có chỉ dẫn rõ ràng ngược lại, các ma trận được xét được lấy đối với các cơ sở này.

Cho G là một song môđun (A, B) (no 1), Φ là một ánh xạ song tuyến tính (tương ứng một ánh xạ nửa song tuyến tính phải đối với J) từ $E \times F$ vào G, và $R = (\Phi(e_i, f_k))$ là ma trận của Φ. Khi đó, với $x \in E$ và $y \in F$, công thức (6) của no 1 (tương ứng (8) của no 2), được viết, với các quy ước trên,

(47) $\Phi(x, y) = {}^t M(x) \cdot R \cdot M(y)$ (tương ứng $\Phi(x, y) = {}^t M(x) \cdot R \cdot M(y)^J$),

trong đó các tích được tính theo các ánh xạ xác định cấu trúc của song môđun (A, B) của G ; đặc biệt, nếu $A = B = G$ (trong trường hợp đó Φ là một dạng), các tích được tính trong A.

Cho $E’$ là một A-môđun trái có một cơ sở hữu hạn $(e'_s)_{s \in S}$, $F’$ là một A-môđun phải (tương ứng trái) có một cơ sở hữu hạn $(f'_t)_{t \in T}$, $u : E \to E'$ và $\varphi : F \to F'$ là các ánh xạ A-tuyến tính, và $\Phi'$ là một ánh xạ song tuyến tính (tương ứng song nửa tuyến tính phải đối với $J$) từ $E' \times F'$ vào $G$. Gọi $\Phi$ là ảnh ngược của $\Phi'$ (đối với $u$ và $\varphi$), $U, V, R, R'$ là các ma trận của $u, \varphi, \Phi, \Phi'$ đối với các cơ sở đang xét. Khi đó ta có

(48) $R = {}^t U \cdot R' \cdot V$ (tương ứng $R = {}^t U \cdot R' \cdot V^J$),

các tích được tính như trong (47). Thật vậy, với mọi $x \in E$ và $y \in F$, theo định nghĩa ta có $\Phi(x, y) = \Phi'(u(x), v(y))$, do đó, theo (47),

$$
'M(x).R.M(y) = 'M(u(x)).R'.M(v(y))
$$
(tương ứng $'M(x).R.M(y)^J = 'M(u(x)).R'.M(v(y))^J$);

theo (45 G) và (45 D) (tương ứng (45 G)) và (43) ta suy ra

$$
'M(x).R.M(y) = 'M(x).'U.R'.V.M(y)
$$
(tương ứng $'M(x).R.M(y)^J = 'M(x).'U.R'.('M(y).'V)^J$
$= 'M(x).'U.R'.V^J.M(y)^J$);

điều này chứng minh mệnh đề của ta.

IV. — Ở đây ta giả sử rằng các vành $A$ và $B$ bằng nhau, và ta ký hiệu bởi $\Phi$ một dạng song tuyến tính (tương ứng song nửa tuyến tính phải đối với $J$) trên $E \times F$, và bởi $R$ ma trận của nó. Ta hãy tính các ma trận của các ánh xạ $s_\Phi$ và $d_\Phi$ liên kết với $\Phi$, mà để đơn giản ta sẽ ký hiệu bởi $s$ và $d$. Vì ta có $\Phi(x, y) = \langle y, s(x) \rangle = \langle x, d(y) \rangle$ theo (23), No. 6 (tương ứng $\Phi(x, y) = \langle x, d(y) \rangle = \langle y, s(x) \rangle^J$ theo (24), No. 6), ta có $\Phi(e_i, f_k) = \langle f_k, s(e_i) \rangle = \langle e_i, d(f_k) \rangle$ (tương ứng $\Phi(e_i, f_k) = \langle e_i, d(f_k) \rangle = \langle f_k, s(e_i) \rangle^J$), do đó, theo (44) và vì $(e_i)$ là cơ sở đối ngẫu của $(e_i^*)$ và $(f_k)$ là cơ sở đối ngẫu của $(f_k^*)$:

(49) $M(d) = R, \ M(s) = 'R$   (tương ứng $M(d) = R, \ M(s) = 'R^{J'}$).

#### Nhận xét 2 {#alg-ix-s1-n10-rem-2 .statement}

Khi $A$ là một trường, các ánh xạ tuyến tính $s$ và $d$ có cùng hạng. Ta thấy ở đây rằng các ma trận $M(s)$ và $M(d)$ của chúng có cùng hạng; thật vậy, một ma trận trên $A$ và ma trận chuyển vị của nó có cùng hạng (chương II, § 6, No. 7, mệnh đề 3) và, khi $\Phi$ là sesqui tuyến tính, đẳng thức các hạng của $R$ trên $A$ và của $'R$ trên $A^0$ (nt.) cùng với sự kiện rằng $J'$ là một đẳng cấu của $A^0$ lên $A$, kéo theo đẳng thức các hạng của $R$ và của $'R^J$ trên $A$.

#### Nhận xét 3 {#alg-ix-s1-n10-rem-3 .statement}

Nếu $M$ và $N$ là các môđun phải $A$ có các cơ sở hữu hạn $(m_i)$ và $(n_k)$, $\Phi$ là một dạng sesqui tuyến tính trái đối với $J$ trên $M \times N$ (No. 6, Nhận xét), $s$ và $d$ là các ánh xạ liên kết của nó, và $R = (\Phi(m_i, n_k))$ là ma trận của nó, các công thức (26) của No. 6 cho thấy rằng ta có

$$
M(d) = R^{J'}, \quad M(s) = 'R.
$$

Giả sử bây giờ rằng các ánh xạ $s$ và $d$ liên kết với $\Phi$ là song ánh và tính ma trận $\hat{R}$ của dạng nghịch đảo của $\Phi$ (No. 7). Khi $\Phi$ là song tuyến tính, $\Phi$ là ảnh ngược của $\hat{\Phi}$ đối với các ánh xạ tuyến tính $s : E \to F^*$ và $d : F \to E^*$; do đó, nhờ (48) và (49), ta có $R = R . \hat{R} . R$, do đó, vì $R$ khả nghịch ($d$ là song ánh), $\hat{R} = R^{-1}$. Công thức này mở rộng đến trường hợp $\Phi$ là sesqui tuyến tính, bởi vì, nếu ta xét $\Phi$ như một dạng song tuyến tính trên $E \times F^J$, và nếu ta đồng nhất $(F^J)^*$ với $(F^*)^J$ (xem No. 9), dạng nghịch đảo của dạng song tuyến tính này trùng với $\hat{\Phi}$ được xét như một dạng song tuyến tính trên $(F^*)^J \times E^*$. Trong cả hai trường hợp *ma trận của dạng nghịch đảo của $\Phi$ là nghịch đảo của ma trận của $\Phi$*.

Cuối cùng, cho $E'$ là một A-môđun trái, $F'$ là một A-môđun phải (tương ứng là A-môđun trái), cả hai đều thừa nhận các cơ sở hữu hạn $(e'_s)$ và $(f'_t)$; cho $\Phi'$ là một dạng song tuyến tính (tương ứng là dạng nửa song tuyến tính đối với J) trên $E' \times F'$, và cho $R'$ là ma trận của nó. Giả sử $s_\Phi$ và $d_\Phi$ là song ánh. Cho $u : E \to E'$ và $\nu : F \to F'$ là các ánh xạ tuyến tính, $u^* : F' \to F$ và $\nu^* : E' \to E$ là các *ánh xạ liên hợp* của chúng (No. 8, mệnh đề 7); ký hiệu bởi $U, V, U^*, V^*$ các ma trận của $u, \nu, u^*, \nu^*$ đối với các cơ sở đã cho. Khi đó ta có

$$
U^* = R^{-1} . {}^t U . R', \quad {}^t V^* = R'. V . R^{-1}
$$
(tương ứng $U^{*J} = R^{-1} . {}^t U . R', \ {}^t V^* = R'. V^J . R^{-1}$).

Thật vậy, với mọi $x \in E$ và $y \in F'$, ta có $\Phi'(u(x), y) = \Phi(x, u^*(y))$ (No. 8, định nghĩa 10). Do đó, khi $\Phi$ là song tuyến tính, theo (47), ${}^t M(u(x)) . R' . M(y) = {}^t M(x) . R . M(u^*(y))$; điều này cho, theo (45 G) và (45 D), ${}^t M(x) . {}^t U . R' . M(y) = {}^t M(x) . R . U^* . M(y)$, do đó ${}^t U . R' = R . U^*$ và công thức đầu tiên đã công bố, vì $d$ là song ánh nên $R$ khả nghịch. Khi $\Phi$ là nửa song tuyến tính, (47) và (45 G) cho ${}^t M(x) . {}^t U . R' . M(y)^J = {}^t M(x) . R . {}^t ({}^t M(y) . {}^t U^*)^J$; giờ đây, theo (43), ta có $({}^t M(y) . {}^t U^*)^J = {}^t ({}^t U^{*J} . {}^t M(y)^J)$, do đó ${}^t ({}^t M(y) . {}^t U^*)^J = U^{*J} . M(y)^J$; vì vậy suy ra ${}^t M(x) . {}^t U . R' . M(y)^J = {}^t M(x) . R . U^{*J} . M(y)^J$, do đó ${}^t U . R' = R . U^{*J}$, và $U^{*J} = R^{-1} . {}^t U . R'$. Việc kiểm chứng các công thức đối với $V^*$ là tương tự.

*Bài tập.* — 1) Cho A là một trường giao hoán, E là một không gian vectơ trên A thừa nhận một cơ sở đếm được vô hạn $(e_n)_{n \geqslant 1}$. Một dạng song tuyến tính $\Phi$ được xác định trên E bằng cách đặt $\Phi(e_{i+1}, e_i) = 1$ với $i \geqslant 1$, $\Phi(e_k, e_j) = 0$ với $k \neq j + 1$ và $j \geqslant 1$. Chứng minh rằng ánh xạ tuyến tính $d_\Phi$ liên kết ở bên phải với $\Phi$ là đơn ánh, nhưng ánh xạ tuyến tính $s_\Phi$ liên kết ở bên trái với $\Phi$ không đơn ánh.

2) Cho E là tổng trực tiếp các môđun $\mathbf{Z}$ và $\mathbf{Z}/(2)$ trên $\mathbf{Z}$, và cho $E^*$ là môđun đối ngẫu của nó (đẳng cấu với $\mathbf{Z}$). Chứng minh rằng dạng song tuyến tính $(x, x') \to \langle x, x' \rangle$ trên $E \times E^*$ có tính chất rằng ánh xạ tuyến tính liên kết ở bên phải là đơn ánh, nhưng ánh xạ tuyến tính liên kết ở bên trái không đơn ánh.

#### Nhận xét 4 {#alg-ix-s1-n10-rem-4 .statement}

Cho một ví dụ về một dạng song tuyến tính $\Phi$ xác định trên một tích $E \times F$ của hai không gian vectơ, sao cho $d_\Phi$ là song ánh, $s_\Phi$ đơn ánh nhưng không song ánh (lấy $E$ có chiều vô hạn và $F$ bằng không gian đối ngẫu $E^*$ của $E$; xem Chương. II, § 5, bài tập. 3).

#### Nhận xét 5 {#alg-ix-s1-n10-rem-5 .statement}

Cho $A$ là một vành được trang bị một phản tự đẳng cấu $J$, $E$ là một $A$-môđun trái, $G$ là một $(A, A)$-song môđun và $\Phi$ là một ánh xạ từ $E \times E$ vào $G$, nửa song tuyến phải đối với $J$. Chứng minh đẳng thức (trong đó $Q(x) = \Phi(x, x)$) :

$$
2\Phi(x, y)\ (\mu^J\lambda^J - \lambda^J\mu^J) = Q(x - \mu\lambda y) - Q(x + \mu\lambda y) + \mu Q(x + \lambda y)
- \mu Q(x - \lambda y) + Q(x + \mu y)\lambda^J - Q(x - \mu y)\lambda^J + \mu Q(x - y)\lambda^J - \mu Q(x + y)\lambda^J.
$$

#### Nhận xét 6 {#alg-ix-s1-n10-rem-6 .statement}

Cho $K$ là một trường giao hoán có đặc số 2, $A$ là một mở rộng bậc hai tách được của $K$; ta có $A = K(\theta)$, trong đó $\theta$ là nghiệm của một đa thức bất khả quy $X^2 + X + \beta$ của $K[X]$ và tự đẳng cấu $K$-tự đẳng cấu $J$ của $A$, khác với tự đẳng cấu đồng nhất, sao cho $\theta^J = \theta + 1$ (Chương V, § 11, Bài tập 8). Bây giờ chứng minh rằng nếu $E$ và $G$ là các không gian vectơ trên $A$, $\Phi$ là một ánh xạ nửa song tuyến (đối với $J$) từ $E \times E$ vào $G$, thì, đặt $Q(x) = \Phi(x, x)$, ta có

$$
\Phi(x, y) = Q(\theta x + y) - \beta Q(x) - Q(y) - (\theta + 1)(Q(x + y) - Q(x) - Q(y)).
$$

#### Nhận xét 7 {#alg-ix-s1-n10-rem-7 .statement}

Cho $A$ là một trường, $E$ là một không gian vectơ trên $A$, $\Phi$ là một dạng nửa song tuyến trên $E$, $u$ là một tự đồng cấu của $E$.

a) Để tồn tại duy nhất một tự đồng cấu $u^*$ của $E$ sao cho $\Phi(u(x), y) = \Phi(x, u^*(y))$ với $x, y$ thuộc $E$, điều kiện cần và đủ là $d_\Phi$ đơn ánh và $u(d_\Phi(E)) \subset d_\Phi(E)$.

b) Cho một ví dụ trong đó $E$ có chiều vô hạn và $d_\Phi$ là đơn ánh, nhưng $u(d_\Phi(E))$ không được chứa trong $d_\Phi(E)$.

#### Nhận xét 8 {#alg-ix-s1-n10-rem-8 .statement}

Cho $E, E_1$ là hai $A$-môđun, $\Phi$ (tương ứng $\Phi_1$) là một dạng sesquilinear trên $E$ (tương ứng $E_1$). Giả sử rằng $\Phi_1$ không suy biến và tồn tại một phần tử $\alpha \in A$ cùng một song ánh $u$ của $E$ lên $E_1$ sao cho $\Phi_1(u(x), u(y)) = \Phi(x, y)\alpha$ với mọi $x, y$ trong $E$. Chứng minh rằng: 1° $\Phi$ không suy biến ; 2° $u$ tuyến tính ; 3° nếu $E_1$ là một $A$-môđun trung thành, thì điều đó cũng đúng với $E$, và $\alpha$ không là một ước phải của 0 trong $A$ ; 4° nếu $\Phi_1$ nhận các giá trị trong $A$ không phải là các ước trái của 0, thì điều đó cũng đúng với $\Phi$.

#### Nhận xét 9 {#alg-ix-s1-n10-rem-9 .statement}

Cho $A$ là một trường, $E_1, E_2$ là hai không gian vectơ khác 0 trên $A$, $\Phi_1$ (tương ứng $\Phi_2$) là một dạng sesquilinear không suy biến trên $E_1$ (tương ứng $E_2$) đối với một phản tự đẳng cấu $J_1$ (tương ứng $J_2$) của $A$. Cho $u$ là một ánh xạ tuyến tính của $E_1$ lên $E_2$ sao cho quan hệ $\Phi_1(x, y) = 0$ kéo theo $\Phi_2(u(x), u(y)) = 0$.

a) Chứng minh rằng $u$ là một song ánh của $E_1$ lên $E_2$. (Nếu $u(0)$ không suy biến thành 0, chứng minh rằng tồn tại trong $E_1$ hai vectơ $a, b$ sao cho $u(a) \neq 0, u(b) = 0$ và $\Phi_1(a, b) \neq 0$; nếu $H$ là siêu phẳng của các $x \in E_1$ sao cho $\Phi_1(a, x) = 0$, nhận xét rằng khi đó ta sẽ có $u(H) = E_2$.

b) Chứng minh rằng nếu dim $E_1 \geqslant 2$, tồn tại $\alpha \in A$ sao cho ta có $\Phi_2(u(x), u(y)) = \Phi_1(x, y)\alpha$ với mọi $x, y$ thuộc $E_1$. (Với mọi $y \in E_1$, chứng minh rằng tồn tại một phần tử $m(y) \in A$ sao cho $\Phi_2(u(x), u(y)) = \Phi_1(x, y)m(y)$ với mọi $x \in E_1$, và rằng nếu $y$ và $y'$ độc lập tuyến tính trong $E_1$, thì có $m(y + y') = m(y) = m(y')$).

#### Nhận xét 10 {#alg-ix-s1-n10-rem-10 .statement}

Cho $A$ là một trường, $E, F$ là hai không gian vectơ trái trên $A$, $\Phi$ là một dạng sesquilinear không suy biến trên $E \times F$ đối với một tự đẳng cấu phản của $A$.

a) Cho $M$ là một không gian con của $E$, $N$ là một không gian con của $F$ sao cho $N \supset M^0$ và $M \supset N^0$. Chứng minh rằng nếu một trong hai không gian $N/M^0, M/N^0$ có số chiều hữu hạn, thì điều đó cũng đúng với không gian kia, và số chiều của hai không gian này bằng nhau.

b) Cho $M, M'$ là hai không gian con của $E$ sao cho $M^{00} = M$ và $M'$ có số chiều hữu hạn; chứng minh rằng ta có $(M \cap M')^0 = M^0 + {M'}^0$ và $(M + M')^{00} = M + M'$. (Áp dụng $a$) cho các không gian con $M'$ và $M^0 + {M'}^0$, chứng minh rằng $\dim(M \cap M') = \operatorname{codim}(M^0 + {M'}^0)$; áp dụng $a$ cho các không gian con $M + M'$ và $M^0$, chứng minh rằng
$$
\dim((M + M')^{00}/M) = \dim((M + M')/M)).
$$

c) Nếu $E = F$ và nếu $M$ là một không gian con của $E$ sao cho $E = M^0 + M^{00}$, chứng minh rằng $E$ là tổng trực tiếp của $M^0$ và $M^{00}$.

d) Cho $E$ là một không gian vectơ trên một trường giao hoán $A$ thừa nhận một cơ sở đếm được vô hạn $(e_n)_{n \geqslant 0}$, và cho $\Phi$ là dạng song tuyến tính đối xứng trên $E$ sao cho $\Phi(e_n, e_n) = 1$ với mọi $n$, $\Phi(e_i, e_j) = 0$ với $i \geqslant 1, j \geqslant 1$ và $i \neq j$, và $\Phi(e_0, e_n) = 1$ với mọi $n \geqslant 1$. Bây giờ chứng minh rằng $\Phi$ là không suy biến. Cho $M$ (tương ứng $N$) là không gian con của $E$ sinh bởi các $e_{2k}$ (tương ứng $e_{2k-1}$) với $k \geqslant 1$, và cho $H = M + N$, là một siêuphẳng trong $E$. Bây giờ chứng minh rằng ta có $M^0 = N, N^0 = M, H^{00} = E \neq H, (M \cap N)^0 \neq M^0 + N^0$ và $(M + N)^{00} \neq M + N$, mặc dù $M^{00} = M, N^{00} = N$; nếu $L$ là không gian con có số chiều hữu hạn 2 sinh bởi $e_0$ và $e_1$, thì có $(L \cap H)^0 \neq L^0 + H^0$.

#### Nhận xét 11 {#alg-ix-s1-n10-rem-11 .statement}

Cho $E, E'$ là hai không gian vectơ trái trên các trường $A, A'$ tương ứng, có chiều $\geqslant 3$; cho $\mathfrak{F}(E)$ (tương ứng $\mathfrak{F}(E')$ là tập hợp có thứ tự dàn (theo quan hệ bao hàm) tạo bởi các không gian con hữu hạn chiều của $E$ (tương ứng $E'$).

a) Cho $p$ là một ánh xạ từ $\mathfrak{F}(E)$ vào $\mathfrak{F}(E')$ sao cho với mọi $M \in \mathfrak{F}(E)$, $\dim p(M) = \dim M$, và sao cho với mọi cặp $(M, N)$ các phần tử của $\mathfrak{F}(E)$, $p(M + N) = p(M) + p(N)$. Bây giờ chứng minh rằng $p$ là đơn ánh; nếu $p$ là song ánh, tồn tại một ánh xạ nửa tuyến tính song ánh $u$ từ $E$ vào $E'$ sao cho ta có $u(M) = p(M)$ với mọi $M \in \mathfrak{F}(E)$ (sử dụng Bài tập 10 của Chương II, ấn bản thứ 2, Phụ lục III).

(b) Hãy cho một ví dụ trong đó $A' = A$ là giao hoán, $E' = E$ có số chiều hữu hạn, và tồn tại một ánh xạ $p$ từ $\mathfrak{F}(E)$ vào chính nó, sao cho $\dim p(M) = \dim M, p(M + N) = p(M) + p(N), p(M \cap N) = p(M) \cap p(N)$, nhưng không tồn tại bất kỳ ánh xạ nửa tuyến tính đơn ánh $u$ nào từ $E$ vào chính nó sao cho $u(M) = p(M)$ đối với $M \in \mathfrak{F}(E)$. (Xét trường hợp tồn tại một siêu trường $A''$ của $A$ có bậc hữu hạn và đẳng cấu với $A$,
