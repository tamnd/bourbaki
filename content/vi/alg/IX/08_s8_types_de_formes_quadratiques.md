---
book: alg
book_title: Algebra
chapter: IX
chapter_title: Formes sesquilinéaires et formes quadratiques
section: 8
section_title: Types de formes quadratiques
lang: vi
source: alg-ix-fr
pdf_pages: 0130-0137
extraction: ocr
subsections:
    - "no": 1
      title: Types de formes quadratiques.
      page: 0
      pdf_page: 130
    - "no": 2
      title: Groupe des types de formes quadratiques.
      page: 0
      pdf_page: 132
    - "no": 3
      title: Anneau des types de formes quadratiques.
      page: 0
      pdf_page: 135
statements: 10
exercises: 0
content_sha256: 4a532ebbdbf3a782a16b8e446b4c69c73548dbae4fbccbcd27dfc725af66c921
translated_from: content/en-mt/alg/IX/08_s8_types_de_formes_quadratiques.md
source_lang: en-mt
translation_method: machine
source_content_sha256: 9597d70ccc4f2287399276b7482c92a23e2147cbca1b5400cff671a619b25517
translation_model: gpt-5-mini, gpt-5-6-mini
translation_run: translate-vi-65edabea
glossary_version: 34
glossary_terms_sha256: 5169aeb7c3c1697f310f43bb7ef3ebbbc9fce6b8f5d1fb17e7d118887de23ed5
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 8. Các kiểu của dạng toàn phương

Trong đoạn này ta giả sử rằng A là một trường giao hoán.

### 1. Các kiểu của dạng toàn phương.

Cho một dạng toàn phương Q ($§ 3, n° 4$) trên một không gian vectơ E trên A, ta sẽ nói rằng E là không gian định nghĩa-

(*) Các kết quả này (chưa công bố) đã được I. Kaplansky truyền đạt cho chúng tôi.

của Q và rằng dim(E) là chiều của Q. Cho hai dạng toàn phương Q, Q' trên các không gian vectơ E, E' trên A, ta sẽ ký hiệu tổng trực tiếp của chúng là Q ⊕ Q' (§ 3, no 4). Nhắc lại rằng tổng trực tiếp của hai dạng trung hòa là trung hòa (§ 4, no 2).

Ta đưa vào quan hệ sau:

« Q và Q' là các dạng toàn phương không suy biến có số chiều hữu hạn trên A, và tồn tại các dạng toàn phương trung hòa N, N' sao cho Q ⊕ N tương đương với Q' ⊕ N' ».

Quan hệ này, mà ta sẽ ký hiệu là Q ~ Q', hiển nhiên là phản xạ và đối xứng. Nó cũng là bắc cầu: thật vậy, nếu Q, Q', Q'' là các dạng toàn phương sao cho Q ~ Q' và Q' ~ Q'', thì tồn tại các dạng toàn phương trung hòa M, M', N, N' sao cho Q ⊕ M tương đương với Q' ⊕ M' và Q' ⊕ N với Q'' ⊕ N' ; khi đó Q ⊕ (M ⊕ N) tương đương với (Q ⊕ M) ⊕ N, do đó tương đương với (Q' ⊕ M') ⊕ N, và cũng tương đương với (Q' ⊕ N) ⊕ M', do đó lại tương đương với (Q'' ⊕ N') ⊕ M' và với Q'' ⊕ (N' ⊕ M') ; vì M ⊕ N và N' ⊕ M' là trung hòa, ta thực sự có Q ~ Q''. Quan hệ Q ~ Q' vì thế là một quan hệ tương đương giữa Q và Q'. Hiển nhiên rằng, nếu Q và Q' là hai dạng toàn phương không suy biến có số chiều hữu hạn và tương đương, thì ta có Q ~ Q'.

Đối với mọi dạng toàn phương Q trên A, không suy biến và có số chiều hữu hạn, ta đặt

(1)
$$
\theta(Q) = \tau_x(X \sim Q),
$$
và ta sẽ nói rằng $\theta(Q)$ là kiểu của Q. Nếu Q và Q' là hai dạng toàn phương trên A, không suy biến và có số chiều hữu hạn, thì các quan hệ Q ~ Q' và $\theta(Q) = \theta(Q')$ là tương đương.

#### Mệnh đề 1 {#alg-ix-s8-prop-1 .statement}

Cho Q và Q' là hai dạng toàn phương trên A, không suy biến và có số chiều hữu hạn. Để Q và Q' tương đương, điều kiện cần và đủ là chúng có cùng số chiều và cùng kiểu.

Điều kiện hiển nhiên là cần. Giả sử nó được thỏa mãn. Khi đó tồn tại các dạng trung hòa N, N' sao cho Q ⊕ N và Q' ⊕ N' tương đương. Vì hai dạng này có cùng số chiều, điều tương tự cũng đúng đối với N và N', do đó chúng tương đương (§ 4, no 2, hệ quả 2 của mệnh đề 2). Suy ra Q và Q' tương đương theo định lý Witt (§ 4, no 3, hệ quả 1 của định lý 1).

#### Mệnh đề 2 {#alg-ix-s8-prop-2 .statement}

Quan hệ « tồn tại một dạng toàn phương Q trên A, không suy biến và có số chiều hữu hạn, sao cho X = θ(Q) » là xác định tập trong X (Ens., chap. II, § 1, n° 4).

Thật vậy, cho V là một không gian vectơ vô hạn chiều trên A, $\mathfrak{S}$ là tập hợp các dạng toàn phương không suy biến được xác định trên các không gian con hữu hạn chiều của V, và $\mathfrak{W}$ là tập hợp các $\theta(Q)$ đối với $Q \in \mathfrak{S}$. Hiển nhiên rằng mọi dạng toàn phương không suy biến $Q'$ có số chiều hữu hạn trên A đều tương đương với ít nhất một phần tử của $\mathfrak{S}$; do đó $\theta(Q') \in \mathfrak{W}$, điều này chứng minh mệnh đề của chúng ta.

### 2. Nhóm các kiểu của dạng toàn phương.

Ta sẽ trang bị cho tập $\mathfrak{W}$ các kiểu của các dạng toàn phương không suy biến có số chiều hữu hạn trên A một cấu trúc nhóm giao hoán. Ta sẽ định nghĩa một phép cộng trong $\mathfrak{W}$ bằng công thức

$$
T + T' = \theta(T \tau T') \tag{2}
$$

Phép cộng này là giao hoán vì $T' \tau T$ tương đương với $T \tau T'$. Nó là kết hợp vì, nếu $T, T'$ và $T''$ là các phần tử của $\mathfrak{W}$, ta có

$$
(T + T') + T'' \sim (T + T') \tau T'' \sim (T \tau T') \tau T''
$$
$$
\sim T \tau (T' \tau T'') \sim T \tau (T' + T'') \sim T + (T' + T''),
$$
do đó $(T + T') + T'' = T + (T' + T'')$ vì hai phần tử của $\mathfrak{W}$ có cùng kiểu thì bằng nhau. Hơn nữa phép cộng mà ta vừa định nghĩa có một phần tử đơn vị: thật vậy, hiển nhiên rằng mọi dạng trung hòa đều có cùng kiểu $T_0$, cụ thể là kiểu của dạng không của số chiều không; ta thấy ngay rằng $T_0$ là phần tử đơn vị cần tìm. Cuối cùng sự tồn tại, với mọi $T \in \mathfrak{W}$, của một phần tử đối với T suy ra ngay từ mệnh đề sau:

#### Mệnh đề 3 {#alg-ix-s8-prop-3 .statement}

Cho Q là một dạng toàn phương không suy biến có số chiều hữu hạn trên một không gian vectơ V trên A. Gọi – Q là dạng toàn phương trên V được xác định bởi $(-Q)(x) = -Q(x)$ ($x \in V$). Khi đó dạng $Q \tau (-Q)$ là trung hòa.

Thật vậy, hạn chế của $Q \tau (-Q)$ trên đường chéo D của $V \times V$ là không. Chỉ số của dạng này do đó là $\geqslant \frac{1}{2} \dim (V \times V)$ (§ 4, no 2, định nghĩa 2), và do đó bằng $\frac{1}{2} \dim (V \times V)$ (*ibid.*, công thức (4)). Suy ra rằng $Q \tau (-Q)$ là trung hòa (*ibid.*).

Điều này cho phép ta đưa ra định nghĩa sau:

#### Định nghĩa 1 {#alg-ix-s8-def-1 .statement}

*Tập hợp các kiểu của các dạng toàn phương không suy biến có số chiều hữu hạn trên $A$, được trang bị phép cộng được định nghĩa bởi (2), được gọi là nhóm các kiểu của các dạng toàn phương, hay nhóm Witt, của $A$.*

*Nhận xét. —* 1) Mọi dạng toàn phương không suy biến $Q$ có số chiều hữu hạn mà kiểu là không (nghĩa là sao cho $\theta(Q) = T_0$ với ký hiệu trên) là một dạng trung hòa. Thật vậy tồn tại các dạng trung hòa $N, N'$ sao cho $Q \tau N$ tương đương với $N'$. Điều này chỉ ra rằng $Q$ có số chiều chẵn, và do đó tồn tại một dạng trung hòa $N_1$ có cùng số chiều với $Q$. Vì $Q$ và $N_1$ có cùng kiểu, suy ra từ mệnh đề 1 rằng chúng tương đương, và do đó rằng $Q$ là trung hòa.

2) Với mọi dạng toàn phương hữu hạn chiều $Q$ trên $A$, ký hiệu $\delta(Q)$ là lớp modulo 2 của chiều của $Q$. Ta có
$$
\delta(Q \tau Q') = \delta(Q) + \delta(Q').
$$
Vì mọi dạng trung hoà $N$ đều có chiều chẵn, ta có $\delta(N) = 0$; quan hệ $Q \sim Q'$ do đó kéo theo $\delta(Q) = \delta(Q')$. Vậy hạn chế của $\delta$ vào nhóm $\mathfrak{W}$ các kiểu của các dạng toàn phương trên $A$ là một đồng cấu từ $\mathfrak{W}$ vào nhóm $\mathbf{Z}/(2)$. Đồng cấu này là toàn ánh khi $A$ có đặc số $\neq 2$, nhưng không phải như vậy nếu $A$ có đặc số 2, vì khi đó một dạng toàn phương có chiều lẻ là suy biến, dạng song tuyến tính liên kết của nó là phản xứng (xem § 5).

3) Cho $a$ là một phần tử $\neq 0$ của $A$. Nếu $N$ là một dạng trung hoà, thì $aN$ cũng vậy. Suy ra quan hệ $Q \sim Q'$ kéo theo $aQ \sim aQ'$. Với mọi phần tử $T$ của nhóm $\mathfrak{W}$, ta đặt
$$
a.T = \theta(aT).
$$
Như vậy ta thu được một luật hợp thành ngoài giữa nhóm $A^*$ các phần tử khác không của $A$ và nhóm $\mathfrak{W}$. Các công thức sau đây suy ra ngay lập tức từ định nghĩa:
$$
a.(T + T') = a.T + a.T', \quad ab.T = a.(b.T)
$$
$$
(a, b \text{ trong } A^*, \quad T, T' \text{ trong } \mathfrak{W}).
$$

Mặt khác, nếu $a, b$ và $a + b$ thuộc $A^*$, nói chung ta không có $(a + b).T = a.T + b.T$ ($T \in \mathfrak{W}$).

#### Mệnh đề 4 {#alg-ix-s8-prop-4 .statement}

*Cho Q là một dạng toàn phương không suy biến trên một không gian vectơ hữu hạn chiều E trên A. Giả sử rằng A có đặc số $\neq 2$, và cho $(x_1, \ldots, x_n)$ là một cơ sở trực giao của V. Cho $T_1$ là kiểu của dạng toàn phương $Q_1$ xác định trên không gian vectơ A và sao cho $Q_1(1) = 1$. Khi đó kiểu của Q là $\sum_{i=1}^n Q(x_i) \cdot T_1$.

Thật vậy dạng Q tương đương với
$$(Q(x_1)Q_1) \tau \ldots \tau (Q(x_n)Q_1)$$

#### Hệ quả {#alg-ix-s8-n2-cor-1 .statement}

*Các giả thiết và ký hiệu là những giả thiết và ký hiệu của mệnh đề 3, các phần tử $a.T_1$ ($a \in A^*$) tạo thành một tập hợp các phần tử sinh của nhóm các kiểu của các dạng toàn phương trên A.*

Tìm cấu trúc của nhóm các kiểu của các dạng toàn phương trên A do đó là tìm các quan hệ $\mathbf{Z}$-tuyến tính tồn tại giữa các phần tử dạng $a.T_1$. Nếu $b \in A^*$, dạng $Q_1$ xác định trong mệnh đề 4 hiển nhiên tương đương với $b^2Q_1$; do đó $a.T_1 = ab^2.T_1$, điều này cho thấy rằng $a.T_1$ chỉ phụ thuộc vào lớp của $a$ modulo nhóm con $(A^*)^2$ các bình phương của các phần tử của $A^*$. Hơn nữa, từ mệnh đề 3 suy ra rằng ta có $(-a).T_1 = -a.T_1$. Tuy nhiên, nói chung có những quan hệ $\mathbf{Z}$-tuyến tính khác giữa các $a.T_1$ ngoài những quan hệ suy ra từ các quan hệ mà ta vừa chỉ ra.

#### Mệnh đề 5 {#alg-ix-s8-prop-5 .statement}

*Ta giả sử rằng A là một trường có thứ tự cực đại. Cho Q là một dạng toàn phương không suy biến có số chiều hữu hạn trên A, và $(s, t)$ là dấu của nó ($§ 7$, no 2, def. 2). Khi đó kiểu của Q là $(s - t).T_1$, và nhóm $\mathfrak{W}$ các kiểu của các dạng toàn phương trên A là một nhóm cyclic vô hạn sinh bởi $T_1$.

Thật vậy, vì $A^*/(A^*)^2$ có cấp 2 và $(-1).T_1 = -T_1$, $\mathfrak{W}$ được sinh bởi $T_1$ và do đó là cyclic. Với mọi $n > 0$, $n.T_1$ là kiểu của các dạng toàn phương dương không suy biến có chiều $n$; vì các dạng này không trung hòa, ta có $n.T_1 \neq 0$, điều này chứng tỏ rằng $\mathfrak{W}$ là vô hạn. Cuối cùng, một dạng có dấu $(s, t)$ là đẳng cấu, với ký hiệu của mệnh đề 4, với tổng trực tiếp của $s$ dạng $Q_1$ và của $t$ dạng $- Q_1$ (§ 7, n° 2, th. 1); suy ra kiểu của nó là $(s - t). T_1$.

### 3. Vành các kiểu của các dạng toàn phương.

Trong số này, ta giả sử rằng $A$ là một trường có đặc số $\neq 2$.

Cho hai dạng toàn phương $Q, Q'$ trên các không gian vectơ $V, V'$ trên $A$, ta gọi tích tenxơ của $Q$ và $Q'$ là, và ký hiệu bởi $Q \otimes Q'$ dạng toàn phương trên $V \otimes V'$ mà dạng song tuyến tính liên kết của nó là tích tenxơ (§ 1, n° 9, def. 11) của các dạng song tuyến tính liên kết với $Q$ và $Q'$. Dễ thấy rằng $Q \otimes Q'$ thỏa mãn quan hệ

$$(5)$$
$$(Q \otimes Q')(x \otimes x') = Q(x)Q'(x') \quad (x \in V, x' \in V').$$

Nếu $Q$ và $Q'$ không suy biến và có các chiều hữu hạn, điều tương tự cũng đúng đối với $Q \otimes Q'$ (§ 1, n° 9, prop. 9).

Cho $Q, Q', Q''$ là các dạng toàn phương trên các không gian vectơ $V, V', V''$. Sử dụng đẳng cấu chính tắc của $V \otimes V'$ lên $V' \otimes V$ (tương ứng của $(V \otimes V') \otimes V''$ lên $V \otimes (V' \otimes V'')$), của $(V \times V') \otimes V''$ lên $(V \otimes V'') \times (V' \otimes V'')$), ta thấy ngay rằng $Q \otimes Q'$ tương đương với $Q' \otimes Q$ (tương ứng $(Q \otimes Q') \otimes Q''$ với $Q \otimes (Q' \otimes Q'')$, $(Q \tau Q') \otimes Q''$ với $(Q \otimes Q'') \tau (Q' \otimes Q'')$).

Cho $Q$ và $Q'$ là hai dạng toàn phương không suy biến có chiều hữu hạn. Nếu $Q$ là trung hòa thì $Q \otimes Q'$ cũng vậy. Thật vậy, cho $V, V'$ là các không gian trên đó $Q, Q'$ được xác định, $2n$ và $n'$ là các chiều của chúng, và cho $W$ là một không gian con kỳ dị toàn phần có chiều $n$ của $V$ (§ 4, No. 2); khi đó, $W \otimes V'$ là một không gian con kỳ dị toàn phần, và chiều của nó bằng một nửa chiều của $V \otimes V'$; suy ra, như trong Mệnh đề 3, rằng $Q \otimes Q'$ là trung hòa. Tương tự $Q \otimes Q'$ là trung hòa bất cứ khi nào $Q'$ là trung hòa.

Suy ra từ điều này rằng, nếu $Q, Q', Q_1, Q'_1$ là các dạng toàn phương không suy biến có chiều hữu hạn trên $A$, và nếu giả sử rằng $\theta(Q_1) = \theta(Q)$ và $\theta(Q'_1) = \theta(Q')$, thì $\theta(Q_1 \otimes Q'_1) = \theta(Q \otimes Q')$. Thực ra chỉ cần kiểm tra điều này trong trường hợp $Q_1 = Q \tau N$ và $Q'_1 = Q' \tau N'$, $N$ và $N'$ là các dạng trung hòa; trong trường hợp này $Q_1 \otimes Q'_1$ tương đương với

$$
(Q \otimes Q') \tau (Q \otimes N' \tau Q' \otimes N \tau N \otimes N')
$$

và dấu ngoặc thứ hai chỉ một dạng trung hòa; điều này chứng minh mệnh đề của chúng ta.

Bây giờ cho $\mathfrak{B}$ là nhóm các kiểu của các dạng toàn phương trên $A$. Định nghĩa, trên tập hợp $\mathfrak{B}$, một luật hợp thành thứ hai, được ký hiệu theo phép nhân, bởi công thức

(6)
$$
TT' = \theta(T \otimes T') \qquad (T, T' \text{ trong } \mathfrak{B}).
$$

Suy ra ngay từ những gì vừa thấy rằng luật hợp thành này là giao hoán, kết hợp và phân phối đối với phép cộng. Nó có một phần tử đơn vị, đó là kiểu $T_1$ của dạng toàn phương $Q_1$ được xác định trên không gian vectơ $A$ và sao cho $Q_1(1) = 1$: thật vậy, theo (5), $Q_1 \otimes Q = Q$ đối với mọi dạng toàn phương $Q$. Nhóm cộng $\mathfrak{B}$, được trang bị phép nhân mà ta vừa định nghĩa, do đó là một vành giao hoán có phần tử đơn vị; nó được gọi là *vành các kiểu của các dạng toàn phương* của $A$ (hay *vành Witt* của $A$, khi không có nguy cơ nhầm lẫn).

#### Nhận xét 1 {#alg-ix-s8-n3-rem-1 .statement}

Hiển nhiên rằng, nếu $a$ là một phần tử của $A^*$, thì ta có

(7)
$$
a . (TT') = (a . T)T' = T(a . T')
$$

với mọi phần tử $T, T'$ của $\mathfrak{B}$. Hơn nữa, nhận thấy rằng ta có $a . T = T_a T$, ký hiệu $T_a$ là kiểu của dạng toàn phương $aQ_1$ trên $A$.

#### Nhận xét 2 {#alg-ix-s8-n3-rem-2 .statement}

Vì $A$ có đặc số $\neq 2$, mọi phần tử $T$ của $\mathfrak{B}$ có thể được viết dưới dạng $\sum_{i=1}^n a_i . T_1$ trong đó $a_i \in A^*$ (No. 2, Mệnh đề 4). Ta có

(8)
$$
(\sum_{i=1}^n a_i . T_1)(\sum_{j=1}^q b_j . T_1) = \sum_{i,j} a_i b_j . T_1 \qquad (a_i, b_j \text{ trong } A^*).
$$

#### Nhận xét 3 {#alg-ix-s8-n3-rem-3 .statement}

Giả sử rằng $A$ là một *trường có thứ tự cực đại*. Khi đó vành $\mathfrak{B}$ đẳng cấu với $\mathbf{Z}$ (Mệnh đề 5), số nguyên tương ứng với kiểu của một dạng có dấu $(s,\ t)$ là $s - t$ (*ibid.*). Vì tích tenxơ của hai dạng $Q$, $Q'$ có dấu $(s,\ t)$, $(s',\ t')$ là một dạng có chiều $(s + t)\,(s' + t')$, nên bằng một phép tính sơ cấp, suy ra rằng dấu của $Q \otimes Q'$ là $(ss' + tt',\ st' + ts')$.
