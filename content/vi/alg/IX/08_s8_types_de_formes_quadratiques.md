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
content_sha256: af3b297f693ac6c318cc2fedc1f479c640a2824228ebf643bfe0fbea8ad134de
translated_from: content/en-mt/alg/IX/08_s8_types_de_formes_quadratiques.md
source_lang: en-mt
translation_method: machine
source_content_sha256: 9597d70ccc4f2287399276b7482c92a23e2147cbca1b5400cff671a619b25517
translation_model: gpt-5.4
translation_run: translate-vi-65edabea
glossary_version: 34
glossary_terms_sha256: 5169aeb7c3c1697f310f43bb7ef3ebbbc9fce6b8f5d1fb17e7d118887de23ed5
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 8. Các kiểu của dạng toàn phương

Trong tiết này ta giả sử rằng A là một trường giao hoán.

### 1. Các kiểu của dạng toàn phương.

Cho một dạng toàn phương Q ($§ 3, n° 4$) trên một không gian vectơ E trên A, ta sẽ nói rằng E là không gian xác-

(*) Các kết quả này (chưa công bố) đã được I. Kaplansky thông báo cho chúng tôi.

định của Q và rằng dim(E) là chiều của Q. Cho hai dạng toàn phương Q, Q' trên các không gian vectơ E, E' trên A, ta sẽ ký hiệu bởi Q ⊕ Q' tổng trực tiếp của chúng (§ 3, no 4). Nhắc lại rằng tổng trực tiếp của hai dạng trung hòa là trung hòa (§ 4, no 2).

Ta đưa vào quan hệ sau:

« Q và Q' là các dạng toàn phương không suy biến, hữu hạn chiều trên A, và tồn tại các dạng toàn phương trung hòa N, N' sao cho Q ⊕ N tương đương với Q' ⊕ N' ».

Quan hệ này, mà ta sẽ ký hiệu là Q ~ Q', hiển nhiên là phản xạ và đối xứng. Nó cũng bắc cầu: thật vậy, nếu Q, Q', Q'' là các dạng toàn phương sao cho Q ~ Q' và Q' ~ Q'', thì tồn tại các dạng toàn phương trung hòa M, M', N, N' sao cho Q ⊕ M tương đương với Q' ⊕ M' và Q' ⊕ N tương đương với Q'' ⊕ N' ; khi đó Q ⊕ (M ⊕ N) tương đương với (Q ⊕ M) ⊕ N, do đó với (Q' ⊕ M') ⊕ N, và cũng tương đương với (Q' ⊕ N) ⊕ M', do đó lại tương đương với (Q'' ⊕ N') ⊕ M' và với Q'' ⊕ (N' ⊕ M') ; vì M ⊕ N và N' ⊕ M' là trung hòa, nên quả thật ta có Q ~ Q''. Vậy quan hệ Q ~ Q' là một quan hệ tương đương giữa Q và Q'. Rõ ràng là, nếu Q và Q' là hai dạng toàn phương không suy biến, hữu hạn chiều và tương đương, thì ta có Q ~ Q'.

Với mọi dạng toàn phương Q trên A, không suy biến và hữu hạn chiều, ta đặt

(1)
$$
\theta(Q) = \tau_x(X \sim Q),
$$
và ta sẽ nói rằng $\theta(Q)$ là kiểu của Q. Nếu Q và Q' là hai dạng toàn phương trên A, không suy biến và hữu hạn chiều, thì các quan hệ Q ~ Q' và $\theta(Q) = \theta(Q')$ là tương đương.

#### Mệnh đề 1 {#alg-ix-s8-prop-1 .statement}

Cho Q và Q' là hai dạng toàn phương trên A, không suy biến và hữu hạn chiều. Để Q và Q' tương đương, điều kiện cần và đủ là chúng có cùng chiều và cùng kiểu.

Điều kiện ấy hiển nhiên là cần. Giả sử nó được thỏa mãn. Khi đó tồn tại các dạng trung hòa N, N' sao cho Q ⊕ N và Q' ⊕ N' là tương đương. Vì hai dạng này có cùng chiều, N và N' cũng vậy, do đó chúng tương đương (§ 4, no 2, cor. 2 of prop. 2). Suy ra Q và Q' tương đương theo định lý của Witt (§ 4, no 3, cor. 1 of th. 1).

#### Mệnh đề 2 {#alg-ix-s8-prop-2 .statement}

Quan hệ « tồn tại một dạng toàn phương Q trên A, không suy biến và hữu hạn chiều, sao cho X = θ(Q) » là xác định tập theo X (Ens., chap. II, § 1, n° 4).

Thật vậy, cho V là một không gian vectơ vô hạn chiều trên A, $\mathfrak{S}$ là tập hợp các dạng toàn phương không suy biến xác định trên các không gian con hữu hạn chiều của V, và $\mathfrak{W}$ là tập hợp các $\theta(Q)$ với $Q \in \mathfrak{S}$. Rõ ràng mọi dạng toàn phương không suy biến $Q'$ hữu hạn chiều trên A đều tương đương với ít nhất một phần tử của $\mathfrak{S}$; do đó $\theta(Q') \in \mathfrak{W}$, điều này chứng minh mệnh đề của chúng ta.

### 2. Nhóm các kiểu của dạng toàn phương.

Ta sẽ trang bị cho tập hợp $\mathfrak{W}$ các kiểu của các dạng toàn phương không suy biến, hữu hạn chiều trên A một cấu trúc nhóm giao hoán. Ta sẽ định nghĩa một phép cộng trên $\mathfrak{W}$ bởi công thức

$$
T + T' = \theta(T \tau T') \tag{2}
$$

Phép cộng này là giao hoán vì $T' \tau T$ tương đương với $T \tau T'$. Nó là kết hợp vì, nếu $T, T'$ và $T''$ là các phần tử của $\mathfrak{W}$, thì ta có

$$
(T + T') + T'' \sim (T + T') \tau T'' \sim (T \tau T') \tau T''
$$
$$
\sim T \tau (T' \tau T'') \sim T \tau (T' + T'') \sim T + (T' + T''),
$$
do đó $(T + T') + T'' = T + (T' + T'')$ vì hai phần tử của $\mathfrak{W}$ có cùng kiểu thì bằng nhau. Hơn nữa phép cộng mà ta vừa định nghĩa có một phần tử đơn vị: quả thật hiển nhiên là mọi dạng trung hòa đều có cùng một kiểu $T_0$, cụ thể là kiểu của dạng không có chiều bằng không; ta thấy ngay rằng $T_0$ là phần tử đơn vị cần tìm. Sau hết, sự tồn tại, với mọi $T \in \mathfrak{W}$, của một phần tử đối của T là hệ quả trực tiếp của mệnh đề sau:

#### Mệnh đề 3 {#alg-ix-s8-prop-3 .statement}

Cho Q là một dạng toàn phương không suy biến, hữu hạn chiều trên một không gian vectơ V trên A. Ký hiệu bởi – Q dạng toàn phương trên V được xác định bởi $(-Q)(x) = -Q(x)$ ($x \in V$). Khi đó dạng $Q \tau (-Q)$ là trung hòa.

Thật vậy, hạn chế của $Q \tau (-Q)$ lên đường chéo D của $V \times V$ là không. Vậy chỉ số của dạng này là $\geqslant \frac{1}{2} \dim (V \times V)$ (§ 4, no 2, déf. 2), và do đó bằng $\frac{1}{2} \dim (V \times V)$ (*ibid.*, formula (4)). Suy ra $Q \tau (-Q)$ là trung hòa (*ibid.*).

Điều này cho phép ta đưa ra định nghĩa sau:

#### Định nghĩa 1 {#alg-ix-s8-def-1 .statement}

*Tập hợp các kiểu của các dạng toàn phương không suy biến, hữu hạn chiều trên $A$, được trang bị phép cộng định nghĩa bởi (2), được gọi là nhóm các kiểu của dạng toàn phương, hay nhóm Witt, của $A$.*

*Nhận xét. —* 1) Mọi dạng toàn phương không suy biến $Q$ hữu hạn chiều có kiểu bằng không (nghĩa là sao cho $\theta(Q) = T_0$ theo ký hiệu trên) là một dạng trung hòa. Thật vậy, tồn tại các dạng trung hòa $N, N'$ sao cho $Q \tau N$ tương đương với $N'$. Điều này cho thấy rằng $Q$ có chiều chẵn, và do đó tồn tại một dạng trung hòa $N_1$ có cùng chiều với $Q$. Vì $Q$ và $N_1$ có cùng kiểu, theo mệnh đề 1 suy ra chúng tương đương, và vì thế $Q$ là trung hòa.

2) Với mọi dạng toàn phương hữu hạn chiều $Q$ trên $A$, ký hiệu $\delta(Q)$ là lớp modulo 2 của chiều của $Q$. Ta có
$$
\delta(Q \tau Q') = \delta(Q) + \delta(Q').
$$
Vì mọi dạng trung hòa $N$ đều có chiều chẵn, nên $\delta(N) = 0$; do đó quan hệ $Q \sim Q'$ kéo theo $\delta(Q) = \delta(Q')$. Như vậy, sự hạn chế của $\delta$ lên nhóm $\mathfrak{W}$ các kiểu của các dạng toàn phương trên $A$ là một đồng cấu từ $\mathfrak{W}$ vào nhóm $\mathbf{Z}/(2)$. Đồng cấu này là toàn ánh khi $A$ có đặc số $\neq 2$, nhưng không như vậy nếu $A$ có đặc số 2, vì khi đó một dạng toàn phương có chiều lẻ là suy biến, dạng song tuyến tính liên kết của nó là phản xứng (x. § 5).

3) Cho $a$ là một phần tử $\neq 0$ của $A$. Nếu $N$ là một dạng trung hòa thì $aN$ cũng vậy. Suy ra rằng quan hệ $Q \sim Q'$ kéo theo $aQ \sim aQ'$. Với mọi phần tử $T$ của nhóm $\mathfrak{W}$, ta đặt
$$
a.T = \theta(aT).
$$
Như vậy ta thu được một luật hợp thành ngoài giữa nhóm $A^*$ các phần tử khác không của $A$ và nhóm $\mathfrak{W}$. Các công thức sau suy ra ngay lập tức từ định nghĩa:
$$
a.(T + T') = a.T + a.T', \quad ab.T = a.(b.T)
$$
$$
(a, b \text{ trong } A^*, \quad T, T' \text{ trong } \mathfrak{W}).
$$

Mặt khác, nếu $a, b$ và $a + b$ thuộc $A^*$, thì nói chung không có $(a + b).T = a.T + b.T$ ($T \in \mathfrak{W}$).

#### Mệnh đề 4 {#alg-ix-s8-prop-4 .statement}

*Cho Q là một dạng toàn phương không suy biến trên một không gian vectơ hữu hạn chiều E trên A. Giả sử rằng A có đặc số $\neq 2$, và cho $(x_1, \ldots, x_n)$ là một cơ sở trực giao của V. Gọi $T_1$ là kiểu của dạng toàn phương $Q_1$ được xác định trên không gian vectơ A và thỏa mãn $Q_1(1) = 1$. Khi đó kiểu của Q là $\sum_{i=1}^n Q(x_i) \cdot T_1$.

Thật vậy, dạng Q tương đương với
$$(Q(x_1)Q_1) \tau \ldots \tau (Q(x_n)Q_1)$$

#### Hệ quả {#alg-ix-s8-n2-cor-1 .statement}

*Với các giả thiết và ký hiệu như trong mệnh đề 3, các phần tử $a.T_1$ ($a \in A^*$) tạo thành một hệ sinh của nhóm các kiểu của các dạng toàn phương trên A.*

Do đó, tìm cấu trúc của nhóm các kiểu của các dạng toàn phương trên A tức là tìm các quan hệ $\mathbf{Z}$-tuyến tính tồn tại giữa các phần tử dạng $a.T_1$. Nếu $b \in A^*$, thì dạng $Q_1$ được xác định trong mệnh đề 4 hiển nhiên tương đương với $b^2Q_1$; do đó $a.T_1 = ab^2.T_1$, điều này cho thấy rằng $a.T_1$ chỉ phụ thuộc vào lớp của $a$ modulo nhóm con $(A^*)^2$ gồm các bình phương của các phần tử của $A^*$. Hơn nữa, từ mệnh đề 3 suy ra rằng ta có $(-a).T_1 = -a.T_1$. Tuy nhiên, nói chung còn có những quan hệ $\mathbf{Z}$-tuyến tính khác giữa các $a.T_1$ ngoài những quan hệ suy ra từ các quan hệ mà ta vừa chỉ ra.

#### Mệnh đề 5 {#alg-ix-s8-prop-5 .statement}

*Ta giả sử rằng A là một trường có thứ tự cực đại. Cho Q là một dạng toàn phương không suy biến có số chiều hữu hạn trên A, và $(s, t)$ là dấu hiệu của nó ($§ 7$, no 2, đn. 2). Khi đó kiểu của Q là $(s - t).T_1$, và nhóm $\mathfrak{W}$ các kiểu của các dạng toàn phương trên A là một nhóm đơn sinh vô hạn được sinh bởi $T_1$.

Thật vậy, vì $A^*/(A^*)^2$ có cấp 2 và $(-1).T_1 = -T_1$, nên $\mathfrak{W}$ được sinh bởi $T_1$ và do đó là đơn sinh. Với mọi $n > 0$, $n.T_1$ là kiểu của các dạng toàn phương dương không suy biến có chiều $n$; vì các dạng này không trung hòa, nên ta có $n.T_1 \neq 0$, điều đó chứng tỏ rằng $\mathfrak{W}$ là vô hạn. Sau hết, một dạng có dấu hiệu $(s, t)$ là đẳng cấu, theo ký hiệu của mệnh đề 4, với tổng trực tiếp của $s$ dạng $Q_1$ và của $t$ dạng $- Q_1$ (§ 7, n° 2, đl. 1); suy ra kiểu của nó là $(s - t). T_1$.*

### 3. Vành các kiểu của các dạng toàn phương.

Trong số này, ta sẽ giả sử rằng $A$ là một trường có đặc số $\neq 2$.

Cho hai dạng toàn phương $Q, Q'$ trên các không gian vectơ $V, V'$ trên $A$, ta sẽ gọi tích tenxơ của $Q$ và $Q'$, và ký hiệu bởi $Q \otimes Q'$ dạng toàn phương trên $V \otimes V'$ mà dạng song tuyến tính liên kết là tích tenxơ (§ 1, n° 9, đn. 11) của các dạng song tuyến tính liên kết với $Q$ và $Q'$. Dễ thấy rằng $Q \otimes Q'$ thỏa mãn quan hệ

$$(5)$$
$$(Q \otimes Q')(x \otimes x') = Q(x)Q'(x') \quad (x \in V, x' \in V').$$

Nếu $Q$ và $Q'$ không suy biến và có số chiều hữu hạn, thì điều đó cũng đúng cho $Q \otimes Q'$ (§ 1, n° 9, mệnh đề 9).

Cho $Q, Q', Q''$ là các dạng toàn phương trên các không gian vectơ $V, V', V''$. Dùng đẳng cấu chính tắc từ $V \otimes V'$ lên $V' \otimes V$ (tương ứng từ $(V \otimes V') \otimes V''$ lên $V \otimes (V' \otimes V'')$), từ $(V \times V') \otimes V''$ lên $(V \otimes V'') \times (V' \otimes V'')$), ta thấy ngay rằng $Q \otimes Q'$ tương đương với $Q' \otimes Q$ (tương ứng $(Q \otimes Q') \otimes Q''$ với $Q \otimes (Q' \otimes Q'')$, $(Q \tau Q') \otimes Q''$ với $(Q \otimes Q'') \tau (Q' \otimes Q'')$).

Cho $Q$ và $Q'$ là hai dạng toàn phương không suy biến có chiều hữu hạn. Nếu $Q$ là trung hòa thì $Q \otimes Q'$ cũng vậy. Thật vậy, cho $V, V'$ là các không gian trên đó $Q, Q'$ được định nghĩa, $2n$ và $n'$ là các chiều của chúng, và cho $W$ là một không gian con hoàn toàn kỳ dị chiều $n$ của $V$ (§ 4, No. 2); khi đó $W \otimes V'$ là một không gian con hoàn toàn kỳ dị, và chiều của nó bằng một nửa chiều của $V \otimes V'$; suy ra, như trong mệnh đề 3, rằng $Q \otimes Q'$ là trung hòa. Tương tự $Q \otimes Q'$ là trung hòa mỗi khi $Q'$ là trung hòa.

Suy ra từ đó rằng, nếu $Q, Q', Q_1, Q'_1$ là các dạng toàn phương không suy biến có chiều hữu hạn trên $A$, và nếu giả sử rằng $\theta(Q_1) = \theta(Q)$ và $\theta(Q'_1) = \theta(Q')$, thì $\theta(Q_1 \otimes Q'_1) = \theta(Q \otimes Q')$. Thực ra chỉ cần kiểm tra điều này trong trường hợp $Q_1 = Q \tau N$ và $Q'_1 = Q' \tau N'$, với $N$ và $N'$ là các dạng trung hòa; trong trường hợp đó $Q_1 \otimes Q'_1$ tương đương với

$$
(Q \otimes Q') \tau (Q \otimes N' \tau Q' \otimes N \tau N \otimes N')
$$

và ngoặc thứ hai biểu thị một dạng trung hòa; điều này chứng minh mệnh đề của ta.

Xét bây giờ $\mathfrak{B}$ là nhóm các kiểu của các dạng toàn phương trên $A$. Định nghĩa, trên tập hợp $\mathfrak{B}$, một luật hợp thành thứ hai, được ký hiệu theo lối nhân, bởi công thức

(6)
$$
TT' = \theta(T \otimes T') \qquad (T, T' \text{ trong } \mathfrak{B}).
$$

Suy ra ngay từ những gì ta vừa thấy rằng luật hợp thành này là giao hoán, kết hợp và phân phối đối với phép cộng. Nó có một phần tử đơn vị, cụ thể là kiểu $T_1$ của dạng toàn phương $Q_1$ được định nghĩa trên không gian vectơ $A$ và thỏa mãn $Q_1(1) = 1$: thật vậy, theo (5), $Q_1 \otimes Q = Q$ với mọi dạng toàn phương $Q$. Nhóm cộng $\mathfrak{B}$, được trang bị phép nhân mà ta vừa định nghĩa, vì thế là một vành giao hoán có phần tử đơn vị; nó được gọi là *vành các kiểu của các dạng toàn phương* của $A$ (hoặc là *vành Witt* của $A$, khi không có nguy cơ nhầm lẫn).

#### Nhận xét 1 {#alg-ix-s8-n3-rem-1 .statement}

Rõ ràng là, nếu $a$ là một phần tử của $A^*$, ta có

(7)
$$
a . (TT') = (a . T)T' = T(a . T')
$$

với mọi phần tử $T, T'$ của $\mathfrak{B}$. Ngoài ra nhận thấy rằng ta có $a . T = T_a T$, ký hiệu $T_a$ là kiểu của dạng toàn phương $aQ_1$ trên $A$.

#### Nhận xét 2 {#alg-ix-s8-n3-rem-2 .statement}

Vì $A$ có đặc số $\neq 2$, mọi phần tử $T$ của $\mathfrak{B}$ đều có thể viết dưới dạng $\sum_{i=1}^n a_i . T_1$ với $a_i \in A^*$ (No. 2, mệnh đề 4). Ta có

(8)
$$
(\sum_{i=1}^n a_i . T_1)(\sum_{j=1}^q b_j . T_1) = \sum_{i,j} a_i b_j . T_1 \qquad (a_i, b_j \text{ trong } A^*).
$$

#### Nhận xét 3 {#alg-ix-s8-n3-rem-3 .statement}

Giả sử rằng $A$ là một *trường có thứ tự cực đại*. Khi đó vành $\mathfrak{B}$ đẳng cấu với $\mathbf{Z}$ (mệnh đề 5), số nguyên tương ứng với kiểu của một dạng có chữ ký $(s,\ t)$ là $s - t$ (*ibid.*). Vì tích tenxơ của hai dạng $Q$, $Q'$ có các chữ ký $(s,\ t)$, $(s',\ t')$ là một dạng có chiều $(s + t)\,(s' + t')$, suy ra, bằng một phép tính sơ cấp, chữ ký của $Q \otimes Q'$ là $(ss' + tt',\ st' + ts')$.
