---
book: ac
book_title: Commutative Algebra
chapter: VI
chapter_title: VALUATIONS
section: 4
section_title: The height of a valuation
lang: vi
source: ac-i-vii
book_pages: 393-399, 449-453
pdf_pages: 0411-0417, 0467-0471
extraction: ocr
subsections:
    - "no": 1
      title: INCLUSION OF VALUATION RINGS OF THE SAME FIELD
      page: 393
      pdf_page: 411
    - "no": 2
      title: ISOLATED SUBGROUPS OF AN ORDERED GROUP
      page: 394
      pdf_page: 412
    - "no": 3
      title: COMPARISON OF VALUATIONS
      page: 395
      pdf_page: 413
    - "no": 4
      title: THE HEIGHT OF A VALUATION
      page: 396
      pdf_page: 414
    - "no": 5
      title: VALUATIONS OF HEIGHT 1
      page: 397
      pdf_page: 415
statements: 18
exercises: 11
content_sha256: e7f53bb102fc4b160f2307504586a98cd5b23e33383e687bf2c226e70fad9f72
translated_from: content/en/ac/VI/04_s4_the_height_of_a_valuation.md
source_content_sha256: 241b523bbe6a35c37704c2aac29a38f7afcc9e1e0df9204c949f3665e008f232
translation_model: gpt-5-6-mini
translation_run: translate-vi-f7c6e7e4
glossary_version: 34
glossary_terms_sha256: 1dfad9986d5cde590915a2c04e7340e0e89b13fdb80d60e8065ec4f63cdc2022
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 4. CHIỀU CAO CỦA MỘT ĐỊNH GIÁ

### 1. SỰ BAO HÀM CỦA CÁC VÀNH ĐỊNH GIÁ CỦA CÙNG MỘT TRƯỜNG

#### Mệnh đề 1 {#ac-vi-s4-prop-1 .statement}

*Cho $K$ là một trường và $A$ là một vành định giá của $K$. Khi đó:*
(a) *Mọi vành $B$ sao cho $A \subset B \subset K$ đều là một vành định giá của $K$;
(b) *Iđêan cực đại $m(B)$ của một vành như vậy được chứa trong $A$ và nó là một iđêan nguyên tố của $A$;
(c) *Ánh xạ $\mathfrak{p} \mapsto A$, là một song ánh giảm của tập hợp các iđêan nguyên tố của $A$ lên tập hợp các vành $B$ sao cho $A \subset B \subset K$; song ánh ngược của nó là ánh xạ $B \mapsto m(B)$.

Nếu $B$ là một vành sao cho $A \subset B \subset K$ và $x \in K - B$, thì $x \in K - A$, do đó $x^{-1} \in m(A) \subset B$, điều này chứng minh cả rằng $B$ là một vành định giá của $K$ và rằng $m(B) \subset m(A)$; vì $m(B) = m(B) \cap A$ là một iđêan nguyên tố của $A$, ta đã chứng minh (a) và (b). Hơn nữa, $A_{m(B)} \subset B$; ngược lại, nếu $x \in B - A$, thì $x^{-1} \in A$ và $x^{-1} \notin m(B)$ và do đó $x \in A_{m(B)}$; vậy $A_{m(B)} = B$. Cuối cùng cho $\mathfrak{p}$ là một iđêan nguyên tố của $A$; ta viết $B = A_{\mathfrak{p}}$; khi đó $m(B) \cap A = \mathfrak{p}$. (Chương II, § 2, no. 5, Mệnh đề 11) và $m(B) \subset A$ theo (b); do đó $m(B) = \mathfrak{p}$, điều này cho thấy các ánh xạ $\mathfrak{p} \mapsto A$, và $B \mapsto m(B)$ của mệnh đề là các song ánh ngược.

#### Hệ quả {#ac-vi-s4-n1-cor-1 .statement}

*Tập hợp & các vành con của K chứa A được sắp thứ tự toàn phần bởi quan hệ bao hàm.*

Tập hợp các iđêan nguyên tố của $A$ được sắp thứ tự toàn phần bởi quan hệ bao hàm ($\S$ 1, no. 2, Định lý 1 (e)) và ánh xạ $\mathfrak{p} \mapsto A_{\mathfrak{p}}$ đảo ngược các quan hệ bao hàm.

#### Mệnh đề 2 {#ac-vi-s4-prop-2 .statement}

*Cho K là một trường, B là một vành định giá của K và h, là nơi & K liên kết với B (với các giá trị trong $\kappa(B)$). Khi đó ánh xạ $A \mapsto h_B(A)$ xác định một song ánh của tập hợp $\mathcal{A}$ các vành định giá của K được chứa trong B lên tập hợp $\mathcal{A}'$ các vành định giá của $\kappa(B)$.

Nếu $A \in \mathcal{A}$, thì $h_B(A) \in \mathcal{A}'$: thật vậy nếu $x' = h_B(x)$ (trong đó $x \in B$) là một phần tử của $\kappa(B) - h_B(A)$, thì $x \notin A$, do đó $x^{-1} \in A$ và $h_B(x)^{-1} \in h_B(A)$. Mặt khác, với $A \in \mathcal{A}$, $A \supset m(B)$ (Mệnh đề 1 (b)) và do đó ánh xạ,

$A \mapsto h_B(A)$ là đơn ánh. Cuối cùng, cho $A' \in \mathcal{A}'$ và $A = h_B(A') \subset B$; ta sẽ chứng minh, điều này sẽ hoàn tất chứng minh, rằng $A \in \mathcal{A}$; nếu $x \in K - A$, thì hoặc $x \notin B$, hoặc $x \in B$; nếu $x \notin B$, thì $x^{-1} \in m(B) \subset A$; nếu $x \in B$, thì $h_B(x) \in \kappa(B)$ và $h_B(x) \notin A$, do đó $h_B(x^{-1}) \in A$ và ta lại kết luận rằng $x^{-1} \in A$; do đó $A \in \mathcal{A}$.

#### Hệ quả {#ac-vi-s4-n1-cor-2 .statement}

*Cho A và B là hai vành định giá của K, trong đó $A \subset B$; đặt $A' = h_B(A)$, đây là một vành định giá của $\kappa(B)$. Trường thặng dư $\kappa(A')$ của $A'$ đẳng cấu chính tắc với trường thặng dư $\kappa(A)$ của A và nơi $h_A$ liên kết với A là hợp thành $h_{A'} \circ h_B$ của các nơi liên kết với A và B.*

Vì vành địa phương $A'$ là một thương của vành địa phương $A$, nên các trường thặng dư của chúng đẳng cấu chính tắc và phương trình $h_A(x) = h_{A'}(h_B(x))$ đúng với $x \in A$. Mặt khác, nếu $x \in B - A$, thì $h_B(x) \notin A'$ và hai vế của phương trình bằng $\infty$; điều tương tự đúng nếu $x \in K - B$.

#### Nhận xét {#ac-vi-s4-n1-rem-1 .statement}

Ngược lại, cho $f$ là một nơi của K với các giá trị trong $K'$ và $f'$ là một nơi của $K'$ với các giá trị trong $K''$. Khi đó $f' \circ f$ là một nơi của K có vành được chứa trong vành của nơi $f$.

### 2. CÁC NHÓM CON CÔ LẬP CỦA MỘT NHÓM CÓ THỨ TỰ

Để nghiên cứu tình huống ở no. 1 dưới quan điểm của các định giá, ta sẽ cần Định nghĩa 1 và Mệnh đề 3 dưới đây.

#### Định nghĩa 1 {#ac-vi-s4-def-1 .statement}

*Một nhóm con H của một nhóm có thứ tự G được gọi là cô lập nếu các quan hệ $0 \leq y \leq x$ và $x \in H$ kéo theo $y \in H$.*

Ví dụ (1) Cho $A$ và $B$ là hai nhóm có thứ tự; trang bị cho $A \times B$ thứ tự từ điển (nghĩa là "$(a, b) \leq (a', b')$" tương đương với "$(a < a') \text{ or } (a = a' \text{ and } b \leq b')$"). Nhân tử thứ hai $B$ của $A \times B$ khi đó, như thấy ngay lập tức, là một nhóm con cô lập của $A \times B$.

#### Mệnh đề 3 {#ac-vi-s4-prop-3 .statement}

Cho $G$ là một nhóm có thứ tự và $P$ là tập hợp các phần tử dương của nó.

(a) *Hạt nhân của một đồng cấu tăng từ $G$ vào một nhóm có thứ tự là một nhóm con cô lập của $G$.*

(b) *Ngược lại, cho $H$ là một nhóm con cô lập của $G$ và $g$ là đồng cấu chính tắc của $G$ lên $G/H$. Khi đó $g(P)$ là tập hợp các phần tử dương của một cấu trúc nhóm có thứ tự trên $G/H$. Hơn nữa, nếu $G$ được sắp thứ tự toàn phần, thì $G/H$ cũng vậy.*

(a) Cho $f$ là một đồng cấu tăng từ $G$ vào một nhóm có thứ tự; gọi $H$ là hạt nhân của f. Nếu $0 \leq y \leq x$ và $x \in H$, thì $0 \leq f(y) \leq f(x) = 0$, do đó $f(y) = 0$, nghĩa là $y \in H$. Suy ra $H$ là cô lập.

(b) Cho $H$ là một nhóm con cô lập của $G$ và $g : G \to G/H$. Đặt $P' = g(P)$. Rõ ràng $P' + P' \subset P'$. Ngoài ra

$$
P' \cap (-P') = \{0\},
$$

vì, *nếu* $x$ và $y$ là các phần tử của $P$ sao cho $g(x) = -g(y)$, thì $x + y \in H$, do đó $x \in H$ và $y \in H$ vì $H$ là cô lập; suy ra $g(x) = g(y) = 0$. Vậy $P'$ là tập hợp các phần tử dương của một cấu trúc nhóm có thứ tự trên $G/H$ (*Đại số*, Chương VI, § 1, no. 3, Mệnh đề 3). Cuối cùng, nếu $G$ được sắp thứ tự toàn phần, thì $P \cap (-P) = G$, do đó $P' \cup (-P') = G/H$ và vì thế $G/H$ được sắp thứ tự toàn phần (*loc. cit.*).

Ví dụ (2) Nếu xét lại ví dụ trong đó $G$ là một tích từ điển $A \times B$ và $H = B$, thì nhóm có thứ tự $G/H$ được đồng nhất một cách chính tắc với $A$.

### 3. SO SÁNH CÁC GIÁ TRỊ

Cho $K$ là một trường và $A$ là một vành định giá của $K$. Với mọi vành con $B$ của $K$ chứa $A$, $U(A) \subset U(B)$. Khi đó tồn tại một đồng cấu chính tắc $\lambda$ của $\Gamma_A = K^*/U(A)$ lên $\Gamma_B = K^*/U(B)$, có hạt nhân là $U(B)/U(A)$. Khi đó, ký hiệu $v_A$ và $v_B$ là các định giá chính tắc trên $K$ được xác định bởi $A$ và $B$ (§ 3, no. 2),

(1)

$$
v_B = \lambda \circ v_A.
$$

Vì $A \subset B$, $\lambda$ ánh xạ các phần tử dương của $\Gamma_A$ vào các phần tử dương của $\Gamma_B$ và do đó là tăng. Vì vậy (Mệnh đề 3) hạt nhân $H$, của $\lambda$ là một nhóm con cô lập của $\Gamma_A$ và $\lambda$ phân tích thành $\Gamma_A \to \Gamma_A/H_B \xrightarrow{\mu} \Gamma_B$, trong đó $\mu$ là một đồng cấu song ánh tăng và do đó là một *đẳng cấu* của các nhóm có thứ tự toàn phần; do đó $\Gamma_B$ được đồng nhất với nhóm thương có thứ tự toàn phần $\Gamma_A/H_B$.

#### Mệnh đề 4 {#ac-vi-s4-prop-4 .statement}

*Ánh xạ* $B \mapsto H_B$ *là một song ánh tăng từ tập hợp các vành con của* $K$ *chứa* $A$ *lên tập hợp các nhóm con cô lập của* $\Gamma_A$.

Cho $H$, $v_B$ được xác định tới tương đương và do đó $B$ được xác định duy nhất. Mặt khác, cho $H$ là một nhóm con cô lập của $\Gamma_A$; xét $\Gamma_A / H$ như một nhóm có thứ tự toàn phần (Mệnh đề 3), ánh xạ hợp thành

$$
K^* \xrightarrow{v_A} \Gamma_A \longrightarrow \Gamma_A / H
$$

là một định giá trên $K$ có vành chứa $A$.

#### Nhận xét {#ac-vi-s4-n3-rem-1 .statement}

Dưới các giả thiết trên, cho $f$ là đồng cấu chính tắc của $B$ lên $\kappa(B)$ và $A' = f(A)$; nó là một vành định giá của $\kappa(B)$ (Mệnh đề 2, no. 1). Khi đó $f^{-1}(\kappa(B)^*) = U(B), f^{-1}(A') = A, f^{-1}(m(A')) = m(A)$, do đó

$$
f^{-1}(U(A')) = U(A).
$$

Khi đó có một đẳng cấu chính tắc của $U(B)/U(A)$ lên $\kappa(B)^*/U(A') = \Gamma_{A'}$. Dãy khớp

$$
0 \to U(B)/U(A) \to \Gamma_A \to \Gamma_B \to 0
$$

khi đó cho một dãy khớp

$$
0 \to \Gamma_{A'} \to \Gamma_A \to \Gamma_B \to 0.
$$

#### Ví dụ {#ac-vi-s4-n3-exa-1 .statement}

Cho $k$ là một trường,

$$
E = k(X) \quad \text{và} \quad K = k(X, Y) = E(Y)
$$

$(X, Y$ các bất định). Cho $B = E[Y]_{(Y)}$ là vành định giá của $K$ được xác định bởi phần tử cực trị $Y$ của miền iđêan chính $E[Y]$ (\S 1, no. 4, Mệnh đề 3). Trường thặng dư $\kappa(B)$ được đồng nhất một cách chính tắc với $E[Y]/(Y) = E$. Tương tự, cho $A' = k[X]_{(X)}$ là vành định giá của $E = k(X)$ được xác định bởi phần tử cực trị $X$ của $k[X]$. Ký hiệu $h$, place của $E$ liên kết với $B$ và viết $A = h_B^{-1}(A')$, ta xác định được một vành định giá $A$ của $K$ được chứa trong $B$ và $\kappa(A) = \kappa(A') = k$. Place chính tắc $h$: $K \to k$ có thể được mô tả như sau: nếu $(X, Y)$ là một phần tử của $K$, thì trước hết ta đặt $Y = 0$ inf (điều này cho một phần tử của $\tilde{E} = k(X)^*$), rồi đặt $X = 0$ trong kết quả thu được. Các nhóm $\Gamma_{A'}$ và $\Gamma_B$ đẳng cấu một cách chính tắc với $\mathbf{Z}$ (\S 3, no. 4, Ví dụ 4). *Không khó để chỉ ra (xem \S 10, no. 2, Bổ đề 2) rằng nhóm $\Gamma_A$ đẳng cấu với tích từ điển $\mathbf{Z} \times \mathbf{Z}$ và rằng định giá $v_A$ tương đương với định giá được xác định trong \S 3, no. 4, cuối Ví dụ 6.*

### 4. CHIỀU CAO CỦA MỘT ĐỊNH GIÁ

Cho $G$ là một nhóm có thứ tự toàn phần. Cho hai nhóm con cô lập $H$ và $H'$ của $G$, một trong hai nhóm được chứa trong nhóm kia theo thứ tự: thật vậy, nếu không thì sẽ tồn tại một phần tử dương $x$ của $H$ không thuộc $H'$ và một phần tử dương $x'$ của $H'$ không thuộc H; giả sử chẳng hạn $x \geq x'$; vì H là cô lập, nên $x' \in H$, đó là một mâu thuẫn.

Điều này cũng suy ra từ Mệnh đề 4 của no. 3 và Hệ quả của Mệnh đề 1 của no. 1, xét đến sự kiện rằng mọi nhóm có thứ tự toàn phần đều là nhóm thứ tự của một định giá (\$ 3, no. 4, Ví dụ 6).

#### Định nghĩa 2 {#ac-vi-s4-def-2 .statement}

*Cho G là một nhóm có thứ tự toàn phần. Nếu số các nhóm con cô lập của G phân biệt với G là hữu hạn và bằng n, thì G được gọi là có chiều cao n. Nếu số này là vô hạn, thì G được gọi là có chiều cao vô hạn.*

Ví dụ
(1) Chiều cao của nhóm $G = \{0\}$ là 0.
(2) Các nhóm $\mathbf{Z}$ và $\mathbf{R}$ có chiều cao 1.
(3) Cho $G$ là một nhóm có thứ tự toàn phần và $H$ là một nhóm con cô lập của $G$. Nếu $h(H)$ và $h(G/H)$ lần lượt chỉ các chiều cao của các nhóm có thứ tự toàn phần $H$ và $G/H$, thì
$$
h(G) = h(H) + h(G/H),
$$
vì tập hợp các nhóm con cô lập của $G$ được sắp thứ tự toàn phần bởi quan hệ bao hàm. Đặc biệt, nếu $G$ là tích từ điển của hai nhóm có thứ tự toàn phần $H$ và $H'$, thì
$$
h(G) = h(H) + h(H')
$$
(xem no. 2, Ví dụ 2); do đó tích từ điển $\mathbf{Z} \times \mathbf{Z}$ có chiều cao 2.

Mặt khác, cấp của $\mathbf{Z} \times \mathbf{Z}$ được sắp thứ tự bởi phép nhúng vào $\mathbf{R}$ (xem § 3, no. 4, cuối Ví dụ 6) bằng 1 (xem Mệnh đề 8 dưới đây).

#### Định nghĩa 3 {#ac-vi-s4-def-3 .statement}

*Cấp của nhóm thứ tự của một định giá được gọi là cấp của định giá đó.*

Chẳng hạn một định giá rời rạc có cấp 1. Chỉ các định giá không đúng mới có cấp 0. Các Mệnh đề 1 và 4 kéo theo:

#### Mệnh đề 5 {#ac-vi-s4-prop-5 .statement}

*Cấp của một định giá bằng số các iđêan nguyên tố khác không trong vành của nó.*

### 5. CÁC ĐỊNH GIÁ CẤP 1

#### Mệnh đề 6 {#ac-vi-s4-prop-6 .statement}

*Cho $\mathbf{K}$ là một trường và $A$ là một vành con của $\mathbf{K}$. Giả sử rằng $A$ không là một trường. Khi đó các điều kiện sau là tương đương:*
(a) $A$ là vành của một định giá cấp 1 trên $\mathbf{K}$;
(b) $A$ là một vành định giá của $\mathbf{K}$ và không có iđêan nguyên tố nào khác ngoài $(O)$ và $m(A)$;
(c) $A$ là cực đại trong các vành con của $\mathbf{K}$ phân biệt với $\mathbf{K}$.

Mệnh đề 5 của no. 4 chỉ ra rằng (a) kéo theo (b) và Mệnh đề 1 của no. 1 chỉ ra rằng (b) kéo theo (c). Còn phải chứng minh rằng (c) kéo theo (a). Giả sử A là cực đại trong các vành con của K phân biệt với K. Gọi m là một iđêan cực đại của A và V là một vành định giá của K trội hơn A,, (§ 1, no. 2, Hệ quả của Định lý 2); vì m(V) ∩ A = m và m ≠ (0) (vì A không là một trường), V ≠ K, do đó V = A, điều này chứng tỏ rằng A không phải là vành của một định giá v trên K. Như vậy, v có cấp 1 theo các Mệnh đề 1 (no. 1) và 5 (no. 4).

#### Mệnh đề 7 {#ac-vi-s4-prop-7 .statement}

Để một định giá trên một trường có cấp 1, điều kiện cần và đủ là nhóm cấp của nó đẳng cấu với một nhóm con có thứ tự khác không của $\mathbf{R}$.

Điều này thực ra suy ra từ mệnh đề sau:

#### Mệnh đề 8 {#ac-vi-s4-prop-8 .statement}

Cho G là một nhóm được sắp thứ tự toàn phần không rút gọn về O. Các điều kiện sau là tương đương:
(a) G có cấp 1;
(b) với mọi x > 0 và y ≥ 0 trong G, tồn tại một số nguyên n ≥ 0 sao cho y ≤ nx;
(c) G đẳng cấu với một nhóm con của nhóm cộng có thứ tự $\mathbf{R}$ không rút gọn về O.

Cho x là một phần tử dương của G và gọi H, là tập hợp các y ∈ G sao cho tồn tại một số nguyên n ≥ 0 thỏa mãn |y| ≤ nx. Dễ dàng kiểm tra rằng H, là một nhóm con cô lập của G và mọi nhóm con cô lập của G chứa x đều chứa H,. Do đó điều kiện (a) tương đương với “H, = G với mọi x > 0”, nghĩa là với điều kiện (b).

Rõ ràng (c) kéo theo (b). Ngược lại, giả sử điều kiện (b) đúng và gọi Q là tập hợp các phần tử >0 của G. Trước hết giả sử Q có một phần tử nhỏ nhất x; với mọi y ∈ Q, gọi n là số nguyên nhỏ nhất sao cho y ≤ nx; nếu y < nx, thì cũng có nx − y ≥ x, do đó y ≤ (n − 1)x trái với lựa chọn n; vậy y = nx, điều này chỉ ra rằng G = \mathbf{Z}x đẳng cấu với \mathbf{Z} ⊂ \mathbf{R}. Bây giờ giả sử Q không có phần tử nhỏ nhất; ta áp dụng cho tập hợp có thứ tự P = Q ∪ (0) Mệnh đề 1 của Tôpô đại cương, Chương V, § 2 (điều này có thể thực hiện được, vì điều kiện (b) chính là “tiên đề Archimedes”); ta thấy rằng tồn tại một ánh xạ tăng ngặt f của P vào \mathbf{R}_+ sao cho

$$
f(x + y) = f(x) + f(y)
$$

với x ∈ P và y ∈ P; theo tính tuyến tính f có thể được mở rộng thành một đẳng cấu của G lên một nhóm con của $\mathbf{R}$, điều này chứng minh rằng (b) kéo theo (c).

#### Mệnh đề 9 {#ac-vi-s4-prop-9 .statement}

Cho K là một trường, v là một định giá không đúng trên K và A là vành của v. Để A đóng toàn nguyên (Chương V, § 1, no. 4, Định nghĩa 5), điều kiện cần và đủ là v có cấp 1.

Giả sử v có cấp 1. Cho x ∈ K sao cho các x^n (n ≥ 0) đều được chứa trong một môđun con-A sinh hữu hạn của K. Tồn tại d ∈ A − {0} sao cho dx^n ∈ A với mọi n ≥ 0. Khi đó v(d) + nv(x) ≥ 0, nghĩa là n(−v(x)) ≤ v(d) với mọi $n \geqslant 0$, do đó $-v(x) \leqslant 0$ (Mệnh đề 8 (b)) và $x \in A$. Vậy A đóng toàn nguyên.

Bây giờ giả sử v không có cấp 1. Khi đó tồn tại $y \in m(A)$ và $t \in A$ sao cho $nv(y) < v(t)$ với mọi $n \geqslant 0$ (Mệnh đề 8 (b)). Khi đó $ty^{-n} \in A$ với mọi $n \geqslant 0$, nhưng $y^{-1} \notin A$. Do đó A không đóng toàn nguyên.

#### Hệ quả {#ac-vi-s4-n5-cor-1 .statement}

*Cho K là một trường, $(v_\alpha)_{\alpha \in I}$ là một họ các định giá cấp 1 trên K và A là giao của các vành của các v.* Khi đó A là một miền đóng toàn nguyên.

Một miền đóng toàn nguyên không phải lúc nào cũng là một giao của các vành định giá cấp 1 (Bài tập 6).

### Bài tập {#ac-vi-s4-exercises}

Xem các [bài tập cho § 4](exercises/s4/).
