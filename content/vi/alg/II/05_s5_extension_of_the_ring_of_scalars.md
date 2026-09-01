---
book: alg
book_title: Algebra
chapter: II
chapter_title: LINEAR ALGEBRA
section: 5
section_title: Extension of the ring of scalars
lang: vi
source: alg-i-iii
source_edition: 1998, Springer
book_pages: 277-284, 398-399
pdf_pages: 0301-0308, 0422-0423
extraction: ocr
subsections:
    - "no": 1
      title: EXTENSION OF THE RING OF SCALARS OF A MODULE
      page: 277
      pdf_page: 301
    - "no": 2
      title: RELATIONS BETWEEN RESTRICTION AND EXTENSION OF THE RING OF SCALARS
      page: 280
      pdf_page: 304
    - "no": 3
      title: EXTENSION OF THE RING OF OPERATORS OF A HOMOMORPHISM MODULE
      page: 282
      pdf_page: 306
    - "no": 4
      title: DUAL OF A MODULE OBTAINED BY EXTENSION OF SCALARS
      page: 283
      pdf_page: 307
    - "no": 5
      title: A CRITERION FOR FINITENESS
      page: 284
      pdf_page: 308
statements: 13
exercises: 7
content_sha256: affc07e603b807d5587a6c10602c9cb3a6beda320720a4c14db60fc1f11f4679
translated_from: content/en/alg/II/05_s5_extension_of_the_ring_of_scalars.md
source_content_sha256: febcd34cae06506edd112484e71c36d0c4e9ea06b4c8287244a60b89d1e7d7bd
translation_model: gpt-5.4
translation_run: translate-vi-6f13837c
glossary_version: 34
glossary_terms_sha256: ee23966408c4a4daa17f318bc70ae01e7ce9585ffd0b5ab2fc281d3be1241340
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 5. MỞ RỘNG VÀNH VÔ HƯỚNG

### 1. MỞ RỘNG VÀNH VÔ HƯỚNG CỦA MỘT MÔĐUN

Cho $A, B$ là hai vành và $\rho : A \to B$ là một đồng cấu vành; ta xét A-môđun phải $\rho^*(B_d)$ được định nghĩa bởi đồng cấu này ($§ 1$, no. 13); A-môđun này cũng có một cấu trúc B-môđun trái, cụ thể là cấu trúc của $B_s$ và, vì $b'(b\rho(a)) = (b'b)\rho(a)$ với $a \in A, b, b'$ trong $B$, hai cấu trúc môđun này trên $B$ là tương thích ($§ 1$, no. 14). Điều này cho phép ta, với mọi A-môđun trái $E$, định nghĩa một cấu trúc B-môđun trái trên tích tenxơ $\rho_*(B_d) \otimes_A E$ sao cho $\beta'(\beta \otimes x) = (\beta'\beta) \otimes x$ với $\beta, \beta'$ trong $B$ và $x \in E$ ($§ 3$, no. 3). B-môđun trái này được gọi là *dẫn xuất từ $E$ bằng cách mở rộng vành vô hướng lên $B$ bằng $\rho$* và được ký hiệu là $\rho^*(E)$ hoặc $E_{(B)}$ nếu không có sự lẫn lộn.

#### Mệnh đề 1 {#alg-ii-s5-prop-1 .statement}

*Với mọi A-môđun trái $E$, ánh xạ $\phi : x \mapsto 1 \otimes x$ từ $E$ vào A-môđun $\rho_*(\rho^*(E))$ là tuyến tính trên $A$ và tập hợp $\phi(E)$ sinh ra B-môđun $\rho^*(E)$. Hơn nữa, với mọi B-môđun trái $F$ và mọi ánh xạ tuyến tính trên $A$ $f$ từ $E$ vào A-môđun $\rho_*(F)$, tồn tại một và chỉ một ánh xạ tuyến tính trên $B$ $\bar{f}$ từ $\rho^*(E)$ vào $F$ sao cho $\bar{f}(1 \otimes x) = f(x)$ với mọi $x \in E$.*

$B$ có thể được xem như một song môđun $(B, A)$ bằng $\rho$; khi đó có một đẳng cấu chính tắc của $\mathbf{Z}$-môđun

(1)
$$
\operatorname{Hom}_B(B \otimes_A E, F) \to \operatorname{Hom}_A(E, \operatorname{Hom}_B(B_s, F))
$$
như đã thấy trong $§ 4$, no. 1, Mệnh đề 1. Nhưng A-môđun trái $\operatorname{Hom}_B(B_s, F)$ được đồng nhất một cách chính tắc với $\rho^*(F)$: thật vậy, theo định nghĩa ($§ 1$, no. 14), ứng với một phần tử $y \in F$ là đồng cấu $\theta(y) : B_s \to F$ sao cho $(\theta(y))(1) = y$; với mọi $\lambda \in A$, do đó ứng với $\rho(\lambda)y \in F$ là đồng cấu $\mu \mapsto \mu \rho(\lambda)y$ từ $B_s$ vào $F$, mà chính là $\lambda \theta(y)$ đối với cấu trúc A-môđun trái trên $\operatorname{Hom}_B(B_s, F)$ ($§ 1$, no. 14). Dùng sự đồng nhất này, do đó ta thu được một *đẳng cấu* $\mathbf{Z}$-môđun *chính tắc*, nghịch đảo của (1)

(2)
$$
\delta : \operatorname{Hom}_A(E, \rho_*(F)) \to \operatorname{Hom}_B(\rho^*(E), F)
$$
và từ các định nghĩa suy ra ngay lập tức rằng nếu $\delta(f) = \bar{f}$ thì $\bar{f}(1 \otimes x) = f(x)$ với mọi $x \in E$. Đặc biệt, ánh xạ $\phi_E : x \mapsto 1 \otimes x$ chính là
(3)
$$
\phi_E = \delta^{-1}(1_{\rho^*(E)}).
$$

Vậy Mệnh đề 1 được chứng minh. Ánh xạ $\phi_E : E \to \rho_*(\rho^*(E))$ được gọi là *chính tắc*.

#### Nhận xét {#alg-ii-s5-n1-rem-1 .statement}

(1) Mệnh đề 1 cho thấy rằng cặp có thứ tự gồm $E_{(B)}$ và $\phi_E$ là một nghiệm của bài toán ánh xạ phổ quát (Lý thuyết tập hợp, IV, § 3, no. 1), trong đó $\Sigma$ là loài các cấu trúc B-môđun trái (các cấu là các ánh xạ B-tuyến tính) và các ánh xạ $\alpha$ là các ánh xạ A-tuyến tính từ E vào một B-môđun.

(2) Nếu E là một đa môđun $(A, (C'_i); (D'_j))$ và F là một đa môđun $(B, (C''_h); (D''_k))$, thì đẳng cấu (2) là tuyến tính đối với các cấu trúc đa môđun $((D'_j, (C''_h); (C'_i), (D''_k))$ của hai vế ($§ 1$, no. 14 và $§ 3$, no. 4).

(3) Cho E là một A-môđun trái, $a$ là một iđêan hai phía của A và $\rho : A \to A/a$ là đồng cấu chính tắc. Theo ký hiệu của $§ 3$, no. 6, Hệ quả 2 của Mệnh đề 6, A-môđun $E/aE$ bị triệt tiêu bởi $a$ và do đó có một cách chính tắc một cấu trúc $(A/a)$-môđun trái ($§ 1$, no. 12); ngay lập tức thấy rằng ánh xạ chính tắc $\pi : \rho^*(E) \to E/aE$ được định nghĩa trong $§ 3$, no. 6, Hệ quả 2 của Mệnh đề 6 là một đẳng cấu đối với các cấu trúc $(A/a)$-môđun.

#### Hệ quả {#alg-ii-s5-n1-cor-1 .statement}

*Cho E, E' là hai A-môđun trái; với mọi ánh xạ A-tuyến tính $u : E \to E'$, $v = l_B \otimes u$ là ánh xạ B-tuyến tính duy nhất làm cho biểu đồ*

$$
\begin{array}{ccc}
E & \xrightarrow{\phi_E} & E_{(B)} \\
| & & | \\
u \downarrow & & v \downarrow \\
E' & \xrightarrow{\phi_{E'}} & E'_{(B)}
\end{array}
$$

*giao hoán, trong đó $\phi_E$ và $\phi_{E'}$ là các ánh xạ chính tắc.*

Chỉ cần áp dụng Mệnh đề 1 cho đồng cấu A $\phi_{E'} \circ u : E \to E'_{(B)}$.

Ánh xạ $v$ được định nghĩa trong hệ quả trên được ký hiệu là $\rho^*(u)$ hoặc $u_{(B)}$.

Nếu $E''$ là một A-môđun trái thứ ba và $v : E' \to E''$ là một ánh xạ A-tuyến tính, thì ngay lập tức có

$$
(v \circ u)_{(B)} = v_{(B)} \circ u_{(B)}.
$$

Mở rộng vành các toán tử của một môđun là một phép toán *bắc cầu*; nói chính xác hơn:

#### Mệnh đề 2 {#alg-ii-s5-prop-2 .statement}

*Cho $\rho : A \to B,\ \sigma : B \to C$ là các đồng cấu vành. Với mọi A-môđun trái E, tồn tại một và chỉ một C-đồng cấu*

$$(4)$$
$$
\sigma^*(\rho^*(E)) \to (\sigma \circ \rho)^*(E)
$$
*ánh xạ $1 \otimes (1 \otimes x)$ tới $1 \otimes x$ với mọi $x \in E$ và đồng cấu này là song ánh.*

Các $\mathbf{Z}$-môđun nền của $\sigma^*(\rho^*(E))$ và $(\sigma \circ \rho)^*(E)$ tương ứng là $C \otimes_B (B \otimes_A E)$ và $C \otimes_A E$. Tồn tại một $\mathbf{Z}$-đẳng cấu chính tắc $C \otimes_B (B \otimes_A E) \to (C \otimes_B B) \otimes_A E$ ($§ 3$, no. 8, Mệnh đề 8), đẳng cấu này cũng là một C-đẳng cấu đối với các cấu trúc C-môđun trái ở hai vế. Hơn nữa, C-môđun $C \otimes_B B$ được đồng nhất một cách chính tắc với C-môđun $C_s$ dưới đẳng cấu ánh xạ $\gamma \otimes \beta$ tới $\gamma \sigma(\beta)$ (§ 3, no. 4, Mệnh đề 4) và đẳng cấu này cũng là một đẳng cấu đối với cấu trúc A-môđun phải trên $C \otimes_B B$ được xác định bởi $\rho$ và cấu trúc A-môđun phải trên C được xác định bởi $\sigma \circ \rho$. Do đó thu được một đẳng cấu chính tắc

$$
(C \otimes_B B) \otimes_A E \to C \otimes_A E
$$

và, hợp thành nó với đẳng cấu

$$
C \otimes_B (B \otimes_A E) \to (C \otimes_B B) \otimes_A E
$$

đã được xác định ở trên, ta thu được đẳng cấu chính tắc cần tìm.

Nếu $\phi, \phi'$ và $\phi''$ ký hiệu các ánh xạ chính tắc $E \to \rho^*(E), \rho^*(E \to) \sigma^*(\rho^*(E))$ và $E \to (\sigma \circ \rho)^*(E)$, thì $\phi' \circ \phi$ được đồng nhất với $\phi''$ dưới đẳng cấu chính tắc của Mệnh đề 2.

#### Mệnh đề 3 {#alg-ii-s5-prop-3 .statement}

*Cho A, B là hai vành giao hoán, $\rho : A \to B$ là một đồng cấu vành và E, E' là hai A-môđun. Tồn tại một và chỉ một B-đồng cấu*

$$
E_{(B)} \otimes_B E'_{(B)} \to (E \otimes_A E')_{(B)}
$$

*ánh xạ* $(1 \otimes x) \otimes (1 \otimes x')$ *tới* $1 \otimes (x \otimes x')$ *với* $x \in E, x' \in E'$, *và đồng cấu này là song ánh*.

Vế trái của (5) có thể được viết là $(B \otimes_A E) \otimes_B (B \otimes_A E')$ và được đồng nhất với $(E \otimes_A B) \otimes_B (B \otimes_A E')$ vì A và B là giao hoán; tích sau lần lượt được đồng nhất với $E \otimes_A (B \otimes_B B) \otimes_A E'$, $E \otimes_A (B \otimes_A E')$, $E \otimes_A (E' \otimes_A B)$, và cuối cùng với $(E \otimes_A E') \otimes_A B$, bằng cách dùng tính kết hợp của tích tenxơ (§ 3, no. 8, Mệnh đề 8), Mệnh đề 4, § 3, no. 4, và tính giao hoán của A và B. Đẳng cấu cần tìm là hợp thành của các đẳng cấu chính tắc liên tiếp đó.

Rõ ràng nếu S là một hệ sinh của E, thì ảnh của S dưới ánh xạ chính tắc $E \to E_{(B)}$ là một hệ sinh của $E_{(B)}$; đặc biệt, nếu E là một A-môđun hữu hạn sinh, thì $E_{(B)}$ là một B-môđun hữu hạn sinh.

#### Mệnh đề 4 {#alg-ii-s5-prop-4 .statement}

*Cho E là một A-môđun có một cơ sở* $(a_\lambda)_{\lambda \in L}$; *nếu* $\phi : x \mapsto 1 \otimes x$ *là ánh xạ chính tắc của E vào* $\rho^*(E)$, *thì* $(\phi(a_\lambda))_{\lambda \in L}$ *là một cơ sở của* $\rho^*(E)$. *Nếu* $\rho$ *là đơn ánh, thì* $\phi$ *cũng vậy*.

Mệnh đề thứ nhất suy ra ngay lập tức từ § 3, no. 7, Hệ quả 1 của Mệnh đề 7. Hơn nữa, với mọi họ $(\xi_\lambda)_{\lambda \in L}$ các phần tử của A có giá hữu hạn,

$$
\phi \left( \sum_{\lambda \in L} \xi_\lambda a_\lambda \right) = \sum_{\lambda \in L} \rho(\xi_\lambda) \phi(a_\lambda)
$$

và do đó quan hệ $\phi \left( \sum_{\lambda \in L} \xi_\lambda a_\lambda \right) = 0$ tương đương với $\rho(\xi_\lambda) = 0$ với mọi $\lambda \in L$, do đó suy ra mệnh đề thứ hai.

#### Hệ quả {#alg-ii-s5-n1-cor-2 .statement}

*Với mọi A-môđun xạ ảnh E, B-môđun* $\rho^*(E)$ *là xạ ảnh. Nếu hơn nữa* $\rho$ *là đơn ánh, thì ánh xạ chính tắc của E vào* $\rho^*(E)$ *là đơn ánh.*

Theo giả thiết tồn tại một A-môđun tự do M chứa E và trong đó E thừa nhận một phần bù F. Theo § 3, no. 7, Mệnh đề 7, ngay lập tức suy ra rằng $M_{(B)}$ được đồng nhất với tổng trực tiếp của $E_{(B)}$ và $F_{(B)}$ và nếu $\phi$ và $\psi$ là các ánh xạ chính tắc $E \to E_{(B)}$ và $F \to F_{(B)}$, thì ánh xạ chính tắc $M \to M_{(B)}$ đơn giản là $x + y \mapsto \phi(x) + \psi(y)$. Hệ quả suy ra ngay lập tức từ Mệnh đề 4 áp dụng cho A-môđun M.

Khi E là một A-môđun phải, ta viết tương tự $\rho^*(E) = E \otimes_A \rho_*(B_s)$, lần này B được xét như một song môđun (A, B) và cấu trúc B-môđun phải trên $\rho^*(E)$ sao cho $(x \otimes \beta)\beta' = x \otimes (\beta\beta')$ với $\beta \in B' \ \beta' \in B$ và $x \in E$. Chúng tôi để cho người đọc phát biểu đối với các môđun phải những kết quả tương ứng với các kết quả của no. này và no. tiếp theo.

Nhận xét (4). Xét A-môđun trái $\rho_*(B_s)$ được định nghĩa bởi $\rho$ và với mọi A-môđun trái E, xét $\mathbf{Z}$-môđun
$$
\tilde{\rho}(E) = \operatorname{Hom}_A(\rho_*(B_s), E).
$$
Vì $\rho_*(B_s)$ có một cấu trúc B-môđun phải, nên một cấu trúc B-môđun trái được dẫn xuất trên $\tilde{\rho}(E)$ (§ 1, no. 14) sao cho, nếu $u \in \tilde{\rho}(E)$ và $b' \in B$, thì $b'u$ là đồng cấu $b \mapsto u(bb')$ từ $\rho_*(B_s)$ vào E. Ta còn định nghĩa một ánh xạ A-tuyến tính, gọi là chính tắc,
$$
\eta : \rho_*(\tilde{\rho}(E)) \to E
$$
ứng với mỗi đồng cấu $u \in \tilde{\rho}(E)$ phần tử $u(1)$ của E. Vì B có thể được xét như một song môđun (A, B) nhờ $\rho$, nên với mọi B-môđun trái F, có một đẳng cấu $\mathbf{Z}$-môđun chính tắc
$$
\operatorname{Hom}_A(\rho_*(B_s) \otimes_B F, E) \to \operatorname{Hom}_B(F, \operatorname{Hom}_A(\rho_*(B_s), E))
$$
(§ 1, no. 1, Mệnh đề 1). Vì A-môđun trái $\rho^*(B_s) \otimes_B F$ được đồng nhất một cách chính tắc với $\rho_*(F)$ theo § 3, no. 4, Mệnh đề 4, nên ta thu được một đẳng cấu $\mathbf{Z}$-môđun chính tắc, nghịch đảo của đẳng cấu trên,
$$
\operatorname{Hom}_B(F, \tilde{\rho}(E)) \to \operatorname{Hom}_A(\rho_*(F), E)
$$
đẳng cấu này ứng với mỗi ánh xạ B-tuyến tính g từ F vào $\tilde{\rho}(E)$ ánh xạ hợp thành $\eta \circ g$, được xét như một ánh xạ A-tuyến tính từ $\rho_*(F)$ vào E. Đặc biệt, dưới các giả thiết của Mệnh đề 2, nếu thay F bằng $\sigma_*(C_s)$, ta thu được một C-đẳng cấu chính tắc
$$
\tilde{\sigma}(\tilde{\rho}(E)) \to (\sigma \circ \rho)^*(E).
$$

### 2. CÁC QUAN HỆ GIỮA SỰ HẠN CHẾ VÀ MỞ RỘNG VÀNH VÔ HƯỚNG

Cho $\rho : A \to B$ là một đồng cấu vành. Với mọi A-môđun trái E, một ánh xạ A-tuyến tính chính tắc
$$
\phi_E : E \to \rho_*(\rho^*(E))
$$
đã được định nghĩa trong no. 1 sao cho $\phi_E(x) = 1 \otimes x$. Bây giờ ta xét một B-môđun trái F và áp dụng Mệnh đề 1 (no. 1) cho đồng cấu A $l_{\rho_*(F)} : \rho_*(F) \to \rho_*(F)$: ta thu được một ánh xạ B-tuyến tính

$$
\psi_F : \rho^*(\rho_*(F)) \to F
$$

bằng $\delta(l_{\rho_*(F)})$ và do đó sao cho, với mọi $y \in F$ và mọi $\beta \in B$,
$\psi_F(\beta \otimes y) = \beta y$.

#### Mệnh đề 5 {#alg-ii-s5-prop-5 .statement}

*Cho E là một A-môđun trái và F là một B-môđun trái; các ánh xạ hợp thành*

$$
\rho^*(E) \xrightarrow{\rho^*(\phi_E)} \rho^*(\rho_*(\rho^*(E))) \xrightarrow{\psi_{\rho^*(E)}} \rho^*(E)
$$
$$
\rho_*(E) \xrightarrow{\phi_{\rho_*(F)}} \rho_*(\rho^*(\rho_*(F))) \xrightarrow{\rho_*(\psi_F)} \rho_*(F)
$$

*lần lượt bằng các ánh xạ đồng nhất của $\rho^*(E)$ và $\rho_*(F)$.*

Ta cho chứng minh, chẳng hạn, cho (12); với mọi $x \in E$, ánh xạ $\rho^*(\phi_E)$ biến $1 \otimes x$ thành phần tử $1 \otimes (1 \otimes x)$ và ánh xạ $\psi_{\rho^*(E)}$ biến $1 \otimes (1 \otimes x)$ thành phần tử $1 \otimes x$; kết luận suy ra từ thực tế là các phần tử dạng $1 \otimes x$ sinh B-môđun $\rho^*(E)$; chứng minh cho (13) còn đơn giản hơn nữa.

#### Hệ quả {#alg-ii-s5-n2-cor-1 .statement}

*Các ánh xạ $\rho^*(\phi_E)$ và $\phi_{\rho_*(F)}^*$ là đơn ánh và lần lượt đồng nhất $\rho^*(E)$ với một nhân tử trực tiếp của $\rho^*(\rho_*(\rho^*(E)))$ và $\rho_*(F)$ với một nhân tử trực tiếp của $\rho_*(\rho^*(\rho_*(F)))$.*

Đây là một hệ quả của Mệnh đề 5 và § 1, no. 9, Hệ quả 2 của Mệnh đề 15.

#### Mệnh đề 6 {#alg-ii-s5-prop-6 .statement}

*Cho E là một A-môđun trái và F là một B-môđun phải. Tồn tại một và chỉ một $\mathbf{Z}$-đồng cấu*

$$
\rho_*(F) \otimes_A E \to F \otimes_B \rho^*(E)
$$

*biến $y \otimes x$ thành $y \otimes (1 \otimes x)$ với mọi $x \in E$ và mọi $y \in F$, và đồng cấu này là song ánh.*

Theo định nghĩa, vế phải của (14) là $F \otimes_B (B \otimes_A E)$, trong đó B được xét như một song môđun (B, A), và có một $\mathbf{Z}$-đẳng cấu chính tắc $(F \otimes_B B) \otimes_A E \to F \otimes_B (B \otimes_A E)$ được định nghĩa ở § 3, no. 8, Mệnh đề 8; mặt khác, đẳng cấu chính tắc $F \to F \otimes_B B$ của § 3, no. 4, Mệnh đề 4 là một đẳng cấu đối với các cấu trúc A-môđun phải ở hai vế, được xác định bởi $\rho$. Do đó có đẳng cấu cần tìm.

Khi A và B là *giao hoán*, đẳng cấu (14) là một đẳng cấu *A-môđun*

$$
\rho_*(F) \otimes_A E \to \rho_*(F \otimes_B \rho^*(E)).
$$

### 3. MỞ RỘNG VÀNH CÁC TOÁN TỬ CỦA MỘT MÔĐUN ĐỒNG CẤU

Cho $A$ là một vành *giao hoán*, $B$ là một vành, $\rho : A \to B$ là một đồng cấu vành và $E, F$ là hai $A$-môđun; vì $B$ là một song môđun $(A, A)$ (thông qua $\rho$) và $F$ có thể được xét như một song môđun $(A, A)$, nên trên $\mathbf{Z}$-môđun $B \otimes_A F$ có *hai* cấu trúc $A$-môđun, trong đó lần lượt $a(b \otimes y) = (\rho(a)b) \otimes y$ và $a(b \otimes y) = b \otimes (ay)$ với $a \in A,\ b \in B,\ y \in F$. Ta sẽ ký hiệu hai $A$-môđun được xác định như vậy bởi $G'$ và $G''$; hơn nữa $G'$ chính là A-môđun $\rho_*(\rho^*(F))$.

Vì thế, trong định nghĩa của đồng cấu chính tắc ở § 4, no. 2, công thức (7), ta thay $B$ bởi $A$, $B$-môđun $F$ bởi vành $B$ được xét như một $A$-môđun qua $\rho$ và $G$ bởi $F$ được xét như một $(A, A)$-song môđun; vì $A$ là giao hoán, ta có thể viết *đồng cấu* $\mathbf{Z}$-*chính tắc* thu được là

$$
(15) \quad B \otimes_A \operatorname{Hom}_A(E, F) \to \operatorname{Hom}_A(E, G'').
$$

Mặt khác (no. 1, công thức (2)), có một *đẳng cấu* $\mathbf{Z}$-*chính tắc*

$$
(16) \quad \operatorname{Hom}_A(E, G') = \operatorname{Hom}_A(E, \rho_*(\rho^*(F))) \to \operatorname{Hom}_B(\rho^*(E), \rho^*(F)).
$$

Bây giờ giả sử rằng $\rho(A)$ được chứa trong *tâm* của $B$, khi đó $\rho$ cũng được gọi là một đồng cấu *trung tâm* *(hoặc nói rằng $\rho$ xác định một cấu trúc $A$*-đại số* trên $B$, xem III, § 1, no. 3)*. Khi đó các cấu trúc $A$-môđun của $G'$ và $G''$ là *đồng nhất* và bằng cách hợp thành các đồng cấu (16) và (15) do đó ta thu được một *đồng cấu* $\mathbf{Z}$-*chính tắc*

$$
(17) \quad \omega : B \otimes_A \operatorname{Hom}_A(E, F) \to \operatorname{Hom}_B(E_{(B)}, F_{(B)})
$$

được đặc trưng bởi tính chất là, với mọi $u \in \operatorname{Hom}_A(E, F)$ và mọi $b \in B$

$$
(18) \quad \omega(b \otimes u) = r_b \otimes u,
$$

trong đó $r_b$ ký hiệu phép nhân bên phải bởi $b$ trong $B$.

Hơn nữa, giả thiết rằng $\omega$ là một đồng cấu *trung tâm* kéo theo rằng $(bb')\rho(a) = b\rho(a))b'$ với $b,\ b'$ trong $B$ và $a \in A$; nói cách khác cấu trúc $B$-môđun *phải* của $B_d$ là *tương thích* với cấu trúc $A$-môđun của nó; do đó nó xác định trên $B \otimes_A \operatorname{Hom}_A(E, F)$ một cấu trúc $B$-*môđun* *phải* (§ 3, no. 4) và cũng trên $F_{(B)} = B \otimes_A F$, và sau cùng, vì các cấu trúc $B$-môđun trái và phải trên $F_{(B)}$ là *tương thích*, ta cũng thu được một cấu trúc $B$-*môđun* *phải* trên $\operatorname{Hom}_B(E_{(B)}, F_{(B)})$ (§ 1, no. 14). Khi đó kiểm tra ngay lập tức được rằng (17) là một *đồng cấu* $B$-*môđun* *phải* đối với các cấu trúc ấy.

#### Proposition 7 {#alg-ii-s5-prop-7 .statement}

*Cho $A$ là một vành giao hoán, $B$ là một vành, $\rho : A \to B$ là một đồng cấu trung tâm và $E, F$ là hai $A$-môđun.*

(i) *Nếu B là một A-môđun xạ ảnh* (resp. *xạ ảnh sinh hữu hạn*), đồng cấu (17) là *đơn ánh* (resp. *song ánh*).

(ii) *Nếu E là một A-môđun xạ ảnh sinh hữu hạn, đồng cấu* (17) *là song ánh*.

Vì (16) là song ánh, mệnh đề suy ra từ § 4, no. 2. Mệnh đề 2, áp dụng cho đồng cấu chính tắc (15).

### 4. ĐỐI NGẪU CỦA MỘT MÔĐUN THU ĐƯỢC BẰNG MỞ RỘNG VÔ HƯỚNG

Cho A, B là hai vành, $\rho : A \to B$ là một đồng cấu vành, E là một A-môđun trái và E* là đối ngẫu của nó. Ta sẽ định nghĩa một ánh xạ B-*tuyến tính* chính tắc

$$
v_E : (E^*)_{(B)} \to (E_{(B)})^*.
$$

Vế trái của (19) có thể được viết là $\mathrm{Hom}_A(E, A) \otimes_A \rho_* (B_s)$, trong đó, trong $\mathrm{Hom}_A(E, A)$, A được xét như một (A, A)-song môđun. Khi đó có một đồng cấu $\mathbf{Z}$ chính tắc ($§ 4$, no. 2, công thức (7))

$$
v : \mathrm{Hom}_A(E, A) \otimes_A \rho_* (B_s) \to \mathrm{Hom}_A(E, A \otimes_A \rho_* (B_s)) = \mathrm{Hom}_A(E, \rho_* (B_s))
$$

với sự đồng nhất được cho bởi đẳng cấu chính tắc của $§ 3$, no. 4, Mệnh đề 4. Mặt khác, vế phải của (19) có thể được viết là $\mathrm{Hom}_B(\rho_* (B_d) \otimes_A E, B_s)$; vì B là một song môđun (B, A), nên có một $\mathbf{Z}$-đẳng cấu chính tắc ($§ 4$, no. 1, Mệnh đề 1)

$$
\beta : \mathrm{Hom}_B(\rho_* (B_d) \otimes_A E, B_s) \to \mathrm{Hom}_A(E, \mathrm{Hom}_B(B_s, B_s))
$$

và $\mathrm{Hom}_B(B_s, B_s)$ được đồng nhất một cách chính tắc, như một A-môđun, với $\rho_* (B_s)$ (xem chứng minh của no. 1, Mệnh đề 1). Tính đến các sự đồng nhất này, ta thu được đồng cấu $v_E$; dễ dàng kiểm chứng rằng đồng cấu này được đặc trưng bởi đẳng thức

$$
\langle \xi \otimes x, v_E(x^* \otimes \eta) \rangle = \xi_p (\langle x, x^* \rangle) \eta,
$$

với $x \in E, x^* \in E^*, \xi, \eta$ trong B, điều này cho thấy ngay lập tức rằng $v_E$ là B-*tuyến tính*. Hơn nữa, với mọi ánh xạ A-tuyến tính $u : E \to F$ biểu đồ

$$
\begin{array}{ccc}
(F^*)_{(B)} & \xrightarrow{v_F} & (F_{(B)})^* \\
(tu)_{(B)} \downarrow & & \downarrow t(u_{(B)}) \\
(E^*)_{(B)} & \xrightarrow{v_E} & (E_{(B)})^*
\end{array}
$$

là giao hoán.

#### Mệnh đề 8 {#alg-ii-s5-prop-8 .statement}

*Nếu một trong các A-môđun* E, $\rho_* (B_s)$ *là xạ ảnh và hữu hạn sinh, thì đồng cấu* $v_E$ *là song ánh*.

Điều này suy ra từ điều trên và § 4, no. 2, Mệnh đề 2.

Giả sử đặc biệt rằng E là một A-môđun tự do sinh hữu hạn và gọi $(e_i)_{1 \leq i \leq n}$ là một cơ sở của E và $(e_i^*)$ là cơ sở đối ngẫu; khi đó đẳng cấu chính tắc (19) ánh xạ cơ sở $(e_i^* \otimes 1)$ của $(E^*)_{(B)}$ lên cơ sở đối ngẫu của cơ sở $(1 \otimes e_i)$ của $E_{(B)}$.

### 5. MỘT TIÊU CHUẨN VỀ TÍNH HỮU HẠN

#### Mệnh đề 9 {#alg-ii-s5-prop-9 .statement}

Cho B là một vành, A là một vành con của B và P là một A-môđun trái xạ ảnh. Khi đó, nếu $P_{(B)}$ là một B-môđun sinh hữu hạn, thì P tự nó là một A-môđun sinh hữu hạn.

Ta biết (§ 2, no. 6, Mệnh đề 12) rằng tồn tại một họ $(a_\lambda)_{\lambda \in L}$ các phần tử của P và một họ $(a_\lambda^*)_{\lambda \in L}$ các phần tử của đối ngẫu P* sao cho, với mọi $x \in P$, họ $\langle x, a_\lambda^* \rangle$ có giá hữu hạn và $x = \sum_\lambda \langle x, a_\lambda^* \rangle a_\lambda$. Vì $P_{(B)}$ là sinh hữu hạn, tồn tại một họ hữu hạn $(y_i)_{i \in I}$ các phần tử của P sao cho $P_{(B)}$ được sinh bởi các phần tử $1 \otimes y_i$. Với mỗi chỉ số i, họ $\langle y_i, a_\lambda^* \rangle$ có giá hữu hạn. Do đó tồn tại một tập con hữu hạn H của L sao cho $\langle y_i, a_\lambda^* \rangle = 0$ với $i \in I$ và $\lambda \notin H$. Vì
$$
\langle 1 \otimes y_i, 1 d_B \otimes a_\lambda^* \rangle = \langle y_i, a_\lambda^* \rangle,
$$
nên suy ra rằng $1 d_B \otimes a_\lambda^* = 0$ với $\lambda \notin H$. Do đó, với mọi $x \in P$,
$$
\langle x, a_\lambda^* \rangle = \langle 1 \otimes x, 1_B \otimes a_\lambda^* \rangle = 0
$$
với $\lambda \notin H$. Điều này cho thấy A-môđun P được sinh bởi các $a_\lambda$ sao cho $\lambda \in H$.

### Bài tập {#alg-ii-s5-exercises}

Xem [các bài tập của § 5](exercises/s5/).
