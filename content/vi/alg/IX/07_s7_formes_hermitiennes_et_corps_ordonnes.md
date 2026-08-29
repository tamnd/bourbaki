---
book: alg
book_title: Algebra
chapter: IX
chapter_title: Formes sesquilinéaires et formes quadratiques
section: 7
section_title: Formes hermitiennes et corps ordonnés
lang: vi
source: alg-ix-fr
pdf_pages: 0112-0130
extraction: ocr
subsections:
    - "no": 1
      title: Formes hermitiennes positives.
      page: 0
      pdf_page: 113
    - "no": 2
      title: La loi d’inertie.
      page: 0
      pdf_page: 115
    - "no": 3
      title: Réduction d’une forme par rapport à une forme hermitienne positive.
      page: 0
      pdf_page: 116
statements: 42
exercises: 0
content_sha256: 121108f22228a6f45994ce132cdcbe4b41f089fb78e8df61a906a163c1ae1fe7
translated_from: content/en-mt/alg/IX/07_s7_formes_hermitiennes_et_corps_ordonnes.md
source_lang: en-mt
translation_method: machine
source_content_sha256: 4f0c80812b75ece3f8fe3269f0264a75cbbe436bedea3cd029330b3a85055bd4
translation_model: gpt-5-6, gpt-5-6-mini, gpt-5-mini
translation_run: translate-vi-99a2622d
glossary_version: 34
glossary_terms_sha256: fc9e08a1fc07a12b0cf2e6cdb9dc821f466770490711b97344d860bb4060e636
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 7. Các dạng Hermit và các trường có thứ tự

Trong toàn bộ đoạn này, ký hiệu K một trường có thứ tự cực đại (do đó giao hoán và có đặc số không; xem chương VI, § 2), và giả sử rằng ta ở một trong ba trường hợp sau:

1°) A = K, J là đồng nhất;
2°) A là trường K(i), nhận được bằng phép nối vào K một nghiệm i của căn bậc hai của −1, và, với mọi λ ∈ A, $\overline{\lambda}$ là liên hợp của λ (chương II, § 7, số 7).
3°) A là trường quaternion trên K tương ứng với cặp (−1, −1) (hay, như ta sẽ nói ngắn gọn, trường quaternion trên K), và, với mọi λ ∈ A, $\overline{\lambda}$ là liên hợp của λ (xem chương II, § 7, số 8 và chương VIII, § 11, số 2).

Nếu Φ là một dạng Hermit trên E, do đó trong mọi trường hợp ta có $\Phi(x, x) \in K$ với mọi $x \in E$, vì $\Phi(x, x) = \overline{\Phi(x, x)}$.

### 1. Các dạng Hermit dương.

#### Định nghĩa 1 {#alg-ix-s7-def-1 .statement}

Một dạng Hermit $\Phi$ trên $E$ được gọi là dương (tương ứng âm) nếu $\Phi(x, x) \geqslant 0$ (tương ứng $\Phi(x, x) \leqslant 0$) với mọi $x \in E$.

Khi $A = K$, người ta cũng nói rằng dạng toàn phương
$$
Q(x) = \frac{1}{2} \Phi(x, x)
$$
liên kết với $\Phi$ là dương (tương ứng âm).

Giả sử $E$ là hữu hạn chiều trên $A$, và $(e_i)$ ($i = 1, \ldots, n$) là một cơ sở trực giao của $E$ ($§ 6$, số 1, định lý 1). Để một dạng Hermit $\Phi$ trên $E$ là dương, điều kiện cần và đủ là $\Phi(e_i, e_i) \geqslant 0$ với $i = 1, \ldots, n$. Cho $\Phi$ là một dạng Hermit dương không suy biến trên $E$; vì mọi phần tử dương của $K$ là một bình phương, do đó có dạng $\rho \overline{\rho}$ ($\rho \in A$), nên tồn tại các cơ sở trực chuẩn đối với $\Phi$ trong $E$ ($§ 6$, số 1, hệ quả 1 của định lý 1).

#### Mệnh đề 1 {#alg-ix-s7-prop-1 .statement}

Giả sử $E$ là hữu hạn chiều, và $A = K$ hoặc $A = K(i)$. Nếu $\Phi$ là một dạng Hermit dương không suy biến trên $E$, thì các mở rộng của $\Phi$ lên $\bigotimes^p E$ và $\wedge^p E$ ($p > 0$), cũng như dạng nghịch đảo của $\Phi$, là các dạng Hermit dương không suy biến.

Điều này suy ra ngay từ sự tồn tại của một cơ sở trực chuẩn của $E$, và từ mệnh đề 2, $§ 6$, số 1.

Mệnh đề 1 vẫn đúng nếu « dương không suy biến » được thay thế ở mọi nơi bởi « dương ».

#### Mệnh đề 2 {#alg-ix-s7-prop-2 .statement}

Cho $\Phi$ là một dạng Hermit dương trên $E$. Với $x, y$ thuộc $E$, ta có
$$
\Phi(x, y) \overline{\Phi(x, y)} \leqslant \Phi(x, x) \Phi(y, y).
$$

Bất đẳng thức quả thực là ngay lập tức khi các vectơ $x$ và $y$ tỉ lệ. Do đó ta có thể giả sử rằng $x$ và $y$ độc lập tuyến tính. Gọi $A'$ là trường con (giao hoán) $K(\Phi(x, y))$ của $A$, $F$ là mặt phẳng vectơ trên $A'$ sinh bởi $x$ và $y$, và $\Phi_F$ là hạn chế của $\Phi$ vào $F$; dạng sau nhận các giá trị của nó trong $A'$. Theo Mệnh đề 1, biệt thức của $\Phi_F$ đối với cơ sở $(x, y)$ là $\geqslant 0$. Bây giờ biệt thức này là $\Phi(x, x)\Phi(y, y) - \Phi(x, y)\overline{\Phi(x, y)}$. Q.E.D.

#### Hệ quả {#alg-ix-s7-n1-cor-1 .statement}

*Tập hợp các vectơ đẳng hướng của E là không gian con trực giao $E^0$ của E đối với $\Phi$. Để $\Phi$ không suy biến, điều kiện cần và đủ là $\Phi(x, x) > 0$ với mọi $x \neq 0$.

#### Mệnh đề 3 {#alg-ix-s7-prop-3 .statement}

*Giả sử E hữu hạn chiều và A giao hoán ($\mathbf{A} = \mathbf{K}$ hoặc $\mathbf{A} = \mathbf{K}(i)$). Gọi $\Phi$ là một dạng Hermit trên E, X là ma trận của nó đối với một cơ sở $(x_j)$ ($j = 1, \ldots, n$) của E; với mọi tập hợp con H của $\{1, n\}$, ký hiệu $X_{H, H}$ là phần con của X thu được bằng cách xóa các hàng và các cột có chỉ số $j \notin H$ (Chương III, § 6, No. 3).

a) *Nếu $\Phi$ là dương không suy biến, thì $X_{H, H} > 0$ với mọi tập hợp con H của $\{1, n\}$.

b) *Ngược lại, nếu, bằng cách đặt $H_j = \{1, j\}$, ta có $X_{H_j, H_j} > 0$ với $j = 1, \ldots, n$, thì $\Phi$ là dương không suy biến.

Trước hết giả sử rằng $\Phi$ là dương không suy biến. Các phần tử $(x_j)$ ($j \in H$) tạo thành một cơ sở của một không gian con F của E, và phần con $X_{H, H}$ là biệt thức của hạn chế $\Phi_F$ của $\Phi$ vào F đối với cơ sở này; bây giờ, vì $\Phi_F(x, x) > 0$ với mọi $x \neq 0$ trong F, $\Phi_F$ là dương không suy biến (Hệ quả của Mệnh đề 2); do đó $X_{H, H} > 0$ (Mệnh đề 1). Để chứng minh b), ta hãy chú ý rằng, với ký hiệu của Mệnh đề 1, § 6, No. 1, phần con $X_{H_j, H_j}$ bằng $D_{j+1, j+1}$; do đó tồn tại (Mệnh đề 1, § 6, No. 1) một cơ sở trực giao $(e_j)$ ($j = 1, \ldots, n$) của E sao cho $\Phi(e_j, e_j) > 0$ với $j = 1, \ldots, n$; do đó $\Phi$ là dương không suy biến.

#### Nhận xét {#alg-ix-s7-n1-rem-1 .statement}

Từ sự tồn tại của các cơ sở trực chuẩn suy ra rằng hai dạng Hermit dương không suy biến trên hai không gian vectơ có cùng số chiều hữu hạn là *tương đương* (§ 1, no 6). Khi đó, cho L là một không gian Hermit hữu hạn chiều trên A, có dạng metric dương không suy biến, và cho $V_1$ và $V_2$ là hai đa tạp tuyến tính có *cùng chiều* trong L (§ 6, no 6); vì các hạn chế của dạng metric lên các phương của $T_1$ và $T_2$ của $V_1$ và $V_2$ một mặt, và lên các không gian con trực giao $T_1^0$ và $T_2^0$ mặt khác, là tương đương, nên tồn tại một tự đẳng cấu unita $u$ của không gian $T$ các phép tịnh tiến của $L$ sao cho $u(T_1) = T_2$ và $u(T_1^0) = T_2^0$; do đó tồn tại một phép dời hình $v$ của $L$ sao cho $v(V_1) = V_2$. Cho $(a, b), (a', b')$ là hai cặp điểm của $L$; để tồn tại một phép dời hình $v$ của $L$ sao cho $v(a) = a'$ và $v(b) = b'$, thì cần và đủ (với ký hiệu của § 6, no 6) là ta có $e(a, b) = e(a', b')$; phần tử $\sqrt{e(a, b)}$ của $A$ (chap. VI, § 2, no 4) được gọi là khoảng cách giữa $a$ và $b$ trong không gian Hermit $L$.

### 2. Luật quán tính.

#### Định lý 1 (« luật quán tính ») {#alg-ix-s7-thm-1 .statement}

Giả sử rằng $A$ thỏa mãn các giả thiết ở đầu đoạn này, và rằng $E$ có số chiều hữu hạn $n$. Cho $\Phi$ là một dạng Hermit trên $E$. Khi đó:

a) Tồn tại một phân tích của $E$ thành tổng trực tiếp của không gian con $E^0$ trực giao với $E$, và của hai không gian con $E^+$ và $E^-$ sao cho hạn chế của $\Phi$ lên $E^+$ (resp. $E^-$) là dương (resp. âm) và không suy biến.

b) Tồn tại một cơ sở trực giao $(e_i)_{1 \leq i \leq n}$ của $E$ sao cho

$$
\Phi\left( \sum_{i=1}^n \xi_i e_i, \sum_{i=1}^n \eta_i e_i \right) = \sum_{i=1}^s \xi_i \overline{\eta_i} - \sum_{i=s+1}^{s+t} \xi_i \overline{\eta_i}.
$$

c) Các số chiều $s$ của $E^+$ và $t$ của $E^-$ là như nhau đối với mọi phân tích thành tổng trực tiếp thỏa mãn các điều kiện đã nêu trong a) ; số nguyên $s$ (resp. $t$) là giá trị lớn nhất của các số chiều của các không gian con $F$ của $E$ sao cho hạn chế của $\Phi$ lên $F$ là dương (resp. âm) và không suy biến.

d) Hạng của $\Phi$ là $s + t$.

e) Nếu $\Phi$ không suy biến, chỉ số của nó bằng $\inf(s, t)$ (§ 4, no 2, def. 2).

Thật vậy, cho $(x_i)$ ($i = 1, \ldots, n$) là một cơ sở trực giao của $E$ (§ 6, No. 1, Định lý 1); nhắc lại rằng $\Phi(x, x) \in K$ với mọi $x \in E$. Ta có thể giả sử rằng $\Phi(x_i, x_i) > 0$ với $i = 1, \ldots, s$, $\Phi(x_i, x_i) < 0$ với $i = s + 1, \ldots, s + t$ và $\Phi(x_i, x_i) = 0$ với $i = s + t + 1, \ldots, n$. Điều này chứng minh a), vì ta lấy $E^+$ (tương ứng $E^-$) là không gian con sinh bởi $x_1, \ldots, x_s$ (tương ứng bởi $x_{s+1}, \ldots, x_{s+t}$), và $E^0$ khi đó được sinh bởi $x_{s+t+1}, \ldots, x_n$. Ta suy ra b) từ điều này bằng cách nhận thấy rằng $\Phi(x_i, x_i)$ có dạng $\rho \overline{\rho}$ (tương ứng

- $\rho \bar{\rho} )\ (\rho \in A^*)$ với $i = 1, \ldots, s$ (tương ứng $i = s + 1, \ldots, s + t$). Để chứng minh c), xét một không gian con P của E sao cho hạn chế của $\Phi$ trên P là dương và không suy biến; khi đó ta có $P \cap (E^- + E^0) = \{0\}$, và tổng $P + E^- + E^0$ do đó là trực tiếp; ta kết luận rằng $\dim P \leq \dim E^+ = s$, và điều này chứng minh c). Mệnh đề d) suy ra ngay từ a).

Cuối cùng giả sử rằng $\Phi$ là không suy biến, đặt $q = \inf (s, t)$, và chứng minh rằng q là chỉ số của $\Phi$. Với các ký hiệu của b), các vectơ $e_i + e_{s+i}$ (tương ứng $e_i - e_{s+i}$) ($i = 1, \ldots, q$) sinh một không gian con đẳng hướng toàn phần F (tương ứng $F'$). Vì K có đặc số 0, $F + F'$ được sinh bởi $e_1, \ldots, e_q, e_{s+1}, \ldots, e_{s+q}$ và do đó là không đẳng hướng. Hạn chế của $\Phi$ trên không gian con $H = (F + F')^0$ khi đó là dương (hoặc âm) và không suy biến, và H do đó không chứa vectơ đẳng hướng $\neq 0$. Vì $F^0$ chứa F và H, và vì $\dim(F + H) = \operatorname{codim} F' = \operatorname{codim} F$, ta có $F^0 = F + H$. Vậy một vectơ đẳng hướng z trực giao với F tất yếu thuộc F, bởi vì, trong tổng trực tiếp $F + H$, thành phần của z trong H là đẳng hướng. Do đó F là một không gian con đẳng hướng toàn phần cực đại, và điều này chứng minh e).

#### Định nghĩa 2 {#alg-ix-s7-def-2 .statement}

Với các ký hiệu của Định lý 1, cặp $(s, t)$ được gọi là chữ ký của $\Phi$.

### 3. Rút gọn một dạng đối với một dạng Hermit dương.

Trong Số này ta sẽ giả sử rằng E có số chiều hữu hạn $n$ trên $A$, và ta sẽ ký hiệu $\Phi$ là một dạng Hermit dương không suy biến trên E.

Vì các ánh xạ tuyến tính từ E vào $E^*$ liên kết với $\Phi$ là song ánh, với mọi các phần tử $x, y, z$ của E với $y \neq 0$, tồn tại một và chỉ một phần tử $t$ của E sao cho $\Phi(x, z) = \overline{\Phi(t, y)}$. Đặc biệt, nếu $A = K$ hoặc $A = K(i)$ và nếu $u$ là một ánh xạ nửa tuyến tính đối với J từ E vào chính nó (chương II, Phụ lục I, No. 1), thì với mỗi $x \in E$, tồn tại một và chỉ một phần tử $u^*(x)$ sao cho với mỗi $y \in E$, $\Phi(x, u(y)) = \overline{\Phi(u^*(x), y)}$. Người ta thấy ngay lập tức rằng $u^*$ là một ánh xạ nửa tuyến tính đối với J từ E vào chính nó; nó được gọi là tự đồng cấu liên hợp của $u$.

#### Nhận xét 1 {#alg-ix-s7-n3-rem-1 .statement}

Khi J là ánh xạ đồng nhất, ta thu được lại khái niệm tự đồng cấu liên hợp của một đồng cấu được định nghĩa trong § 1, No. 8.

#### Nhận xét 2 {#alg-ix-s7-n3-rem-2 .statement}

Giả sử vẫn rằng $A = K$ hoặc $A = K(i)$. Gọi $E^J$ là A-môđun phải được định nghĩa trong § 1, No. 2, Định nghĩa 5. Dạng $\Phi$ là một dạng song tuyến tính trên $E \times E^J$, $\Phi^J$ là một dạng song tuyến tính trên $E^J \times E$, và $u$ là một ánh xạ A-tuyến tính từ E vào $E^J$. Tự đồng cấu liên hợp của đồng cấu này, theo nghĩa của § 1, No. 8, là một ánh xạ A-tuyến tính từ E vào $E^J$; người ta thấy ngay lập tức rằng nó trùng với ánh xạ $u^*$ được định nghĩa ở trên.

Một tự đồng cấu $u$ của E được gọi là chuẩn (đối với $\Phi$) nếu $uu^* = u^*u$.

Các ví dụ về các tự đồng cấu chuẩn:
1) các tự đẳng cấu unita đối với $\Phi$ ($\S$ 6, No. 2), được đặc trưng bởi quan hệ $u^{-1} = u^*$ ($\S$ 1, No. 8, hệ quả của mệnh đề 8);
2) các tự đồng cấu $u$ sao cho $u^* = u$; các tự đồng cấu này được gọi là các tự đồng cấu Hermit.

Với mỗi tự đồng cấu Hermit $u$ của E, đặt $\Phi_u(x, y) = \Phi(u(x), y)$; ta có
$$
\Phi_u(y, x) = \Phi(u(y), x) = \Phi(y, u(x)) = \overline{\Phi(u(x), y)} = \overline{\Phi_u(x, y)}.
$$
điều này chỉ ra rằng $\Phi_u$ là một dạng Hermit trên E. Ngược lại, cho $\Psi$ là một dạng Hermit trên E; vì ánh xạ $s_\Phi$ từ E vào $E^*$ liên kết với $\Phi$ là song ánh, nên với mỗi $x \in E$, tồn tại một và chỉ một phần tử $u(x)$ của E sao cho $\Psi(x, y) = \Phi(u(x), y)$; dễ dàng kiểm tra được rằng $u$ là một tự đồng cấu Hermit của E. Do đó $u \to \Phi_u$ là một song ánh chính tắc từ tập hợp các tự đồng cấu Hermit của E lên tập hợp các dạng Hermit trên E.

Giả sử rằng $A = K$ hoặc $A = K(i)$; cho một dạng song tuyến tính $\Psi$ trên E, với mỗi $x \in E$, tồn tại một và chỉ một phần tử $u(x)$ của E sao cho $\Psi(x, y) = \overline{\Phi(u(x), y)}$; người ta thấy ngay lập tức rằng $u$ là một ánh xạ nửa tuyến tính (đối với J) từ E vào chính nó. Vì $\Phi(u(x), y) = \Phi(y, u(x)) = \overline{\Phi(u^*(y), x)}$, ta thấy rằng, để $\Psi$ là đối xứng (tương ứng, phản xứng), điều kiện cần và đủ là $u^* = u$ (tương ứng, $u^* = -u$).

#### Định lý 2 {#alg-ix-s7-thm-2 .statement}

Cho S là một tập hợp các tự đồng cấu của E (tương ứng, các ánh xạ nửa tuyến tính từ E vào E khi $A = K$ hoặc $A = K(i)$) ổn định đối với ánh xạ u → u*. Khi đó, nếu V là một không gian con của E ổn định đối với S, thì trực giao của nó V⁰ ổn định đối với S. Mặt khác E là tổng trực tiếp của các không gian con ổn định đối với S, cực tiểu trong tập hợp các không gian con ≠ {0} và ổn định đối với S, và trực giao từng đôi một.

Thật vậy, cho V là một không gian con của E ổn định dưới S; với mọi $x \in V⁰$, $y \in V$ và $u \in S$, ta có $u*(y) \in V$, do đó $\Phi(y, u(x)) = \Phi(u*(y), x) = 0$ (tương ứng $\Phi(y, u(x)) = \overline{\Phi(u^*(y), x)} = 0$), và do đó $u(x) \in V⁰$; vậy V⁰ ổn định dưới S, điều này chứng minh mệnh đề đầu tiên của ta. Đối với mệnh đề thứ hai, ta sẽ tiến hành quy nạp theo chiều n của E, trường hợp n = 0 là tầm thường. Với n ≠ 0 tồn tại một không gian con V ≠ {0} của E ổn định dưới S và cực tiểu, chẳng hạn một không gian con ổn định ≠ {0} có chiều cực tiểu. Khi đó chỉ cần áp dụng giả thiết quy nạp cho V⁰, vì tự đồng cấu phụ hợp của hạn chế của u trên V⁰ (đối với hạn chế của $\Phi$) trùng với hạn chế trên V⁰ của tự đồng cấu phụ hợp của u.

#### Hệ quả 1 {#alg-ix-s7-thm-2-cor-1 .statement}

Giả sử rằng A = K hoặc rằng A = K(i). Cho B là một đại số con của $\mathcal{L}_A(E)$, ổn định dưới ánh xạ u → u*. Khi đó E là một B-môđun nửa đơn, và là tổng trực tiếp của các môđun con đơn trực giao từng đôi một. Đại số B là nửa đơn.

Thật vậy, vì mọi B-môđun con V của E đều có một phần bù, chẳng hạn V⁰, nên B-môđun V là nửa đơn (chương VIII, § 3, No. 3, mệnh đề 7). Vì mọi B-môđun con ≠ {0} và cực tiểu trong E đều đơn, nên E là tổng trực tiếp của các môđun con đơn trực giao từng đôi một. Cuối cùng B là một đại số nửa đơn, vì nó có một môđun nửa đơn và trung thành E mà đối môđun của nó có kiểu hữu hạn (chương VIII, § 5, No. 1, mệnh đề 3).

#### Hệ quả 2 {#alg-ix-s7-thm-2-cor-2 .statement}

Các giả thiết và ký hiệu là những thứ của hệ quả 1, giả sử thêm rằng đại số B là giao hoán. Khi đó mọi phần tử của nó là các tự đồng cấu nửa đơn (chuẩn) của E. Khi A = K (tương ứng A = K(i)), E là tổng trực tiếp của các B-môđun con đơn trực giao từng đôi một, là các không gian vectơ có chiều 1 hoặc 2 (tương ứng 1) trên A.

Mệnh đề đầu tiên suy ra từ chương VIII, § 9, No. 1, mệnh đề 2, vì B là nửa đơn. Mặt khác mọi B-môđun đơn đều đẳng cấu với một B-môđun có dạng B/m, trong đó m là một iđêan cực đại của B, do đó đẳng cấu với một trường giao hoán L có bậc hữu hạn trên A; khi A = K (tương ứng A = K(i)), trường L nhất thiết đẳng cấu với K hoặc K(i) (tương ứng K(i)), vì K(i) là đóng đại số (chương VI, § 2, No. 6, định lý 3).

#### Mệnh đề 4 {#alg-ix-s7-prop-4 .statement}

Cho u là một tự đồng cấu chuẩn của E. Khi A bằng K(i) hoặc trường quaternion trên K, tồn tại một cơ sở trực chuẩn (đối với Φ) của E được tạo bởi các vectơ riêng của u. Khi A = K, u là nửa đơn và E là tổng trực tiếp của các không gian con ổn định đối với u, trực giao từng đôi một, và có chiều 1 hoặc 2.

Trước hết xét trường hợp A là giao hoán (A = K hoặc A = K(i)). Khi đó đại số con B = A[u, u*] của $\mathcal{L}_A(E)$ là giao hoán vì u là chuẩn; nó ổn định dưới ánh xạ $\varphi \to \varphi^*$ nhờ các công thức (32) và (33) của § 1, No. 8. Mệnh đề liên quan đến trường hợp A = K khi đó suy ra ngay lập tức từ hệ quả 2 của định lý 2. Khi A = K(i), hệ quả này cũng chỉ ra rằng E là tổng trực tiếp của các không gian con vectơ $Ax_i$ ($i = 1, \ldots, n$) có chiều 1, trực giao từng đôi một và ổn định đối với u; nếu đặt $e_i = (\Phi(x_i, x_i))^{-1/2} x_i$, $(e_i)$ là cơ sở trực chuẩn cần tìm.

Khi A là trường quaternion trên K, tương tự chỉ cần chứng minh, nhờ định lý 2, rằng mọi phần tử cực tiểu của tập hợp các không gian con $\neq \{0\}$ của E ổn định đối với u và $u^*$ đều có chiều 1. Nhưng một không gian con V như vậy nhất thiết chứa một vectơ riêng $x \neq 0$ của u (*), như nhận thấy được bằng cách quan sát rằng trường quaternion A chứa K(i) như một trường con đóng đại số, và bằng cách hạn chế trường

(*) Nếu E là một không gian vectơ trái trên một trường không giao hoán A, và u là một tự đồng cấu của E, người ta vẫn nói rằng một vectơ $x \neq 0$ của E là một vectơ riêng đối với u nếu tồn tại $a \in A$ sao cho $u(x) = ax$; vô hướng a khi đó được gọi là một trị riêng của u. Ta chú ý rằng, với mọi $b \neq 0$ trong A, vectơ $bx$ là một vectơ riêng đối với u, và trị riêng tương ứng là $bab^{-1}$.

các vô hướng của V vào K(i). Vì vậy chỉ còn phải chứng minh rằng vectơ riêng x của u cũng là một vectơ riêng của u*. Đặt $u(x) = ax$ ($a \in A$); khi đó ta có $\Phi(u(x), x) = a\Phi(x, x) = \Phi(x, x)a = \Phi(x, \overline{a}x)$ vì $\Phi(x, x)$ thuộc tâm của A, và mặt khác $\Phi(u(x), x) = \Phi(x, u^*(x))$; suy ra rằng ta có $\Phi(x, u^*(x) - \overline{a}x) = 0$, và do đó có thể viết $u^*(x) = \overline{a}x + z$, trong đó z là một vectơ trực giao với x. Khi đó ta có

$$
\Phi(u^*(x), u^*(x)) = \overline{a}a\Phi(x, x) + \Phi(z, z) = \Phi(u(x), u(x)) + \Phi(z, z).
$$

Bây giờ, vì u là chuẩn, ta có

$$
\begin{align*}
\Phi(u(x), u(x)) &= \Phi(x, u^*u(x)) = \Phi(x, uu^*(x)) \\
&= \Phi(uu^*(x), x) = \Phi(u^*(x), u^*(x)).
\end{align*}
$$

Do đó ta có $\Phi(z, z) = 0$, điều này, theo giả thiết, kéo theo $z = 0$ và $u^*(x) = \overline{a}x$. QED.

#### Nhận xét {#alg-ix-s7-n3-rem-28 .statement}

Suy ra từ định lý 2 rằng các không gian riêng tương ứng với hai trị riêng phân biệt của u là trực giao.

#### Mệnh đề 5 {#alg-ix-s7-prop-5 .statement}

Cho u là một tự đồng cấu Hermit của E. Các trị riêng của u thuộc K, và tồn tại một cơ sở trực chuẩn của E được tạo bởi các vectơ riêng của u.

Khi A bằng K(i) hoặc trường quaternion trên K, nhờ mệnh đề 4 chỉ cần chứng minh mệnh đề đầu tiên; bây giờ, nếu x là một vectơ riêng $\neq 0$ của u và a là trị riêng tương ứng, thì nhờ giả thiết $u = u^*$, ta có

$$
a\Phi(x, x) = \Phi(u(x), x) = \Phi(x, u(x)) = \Phi(x, x)\overline{a} ;
$$

vì $\Phi(x, x)$ là một phần tử khác không của tâm của A, suy ra $a = \overline{a}$, do đó $a \in K$. Do đó một ma trận Hermit có tất cả các trị riêng của nó trong K. Bây giờ giả sử rằng A bằng K. Ma trận M của u đối với một cơ sở trực chuẩn của E khi đó là đối xứng; do đó nó là một ma trận Hermit nếu ta xét nó như một ma trận trên K(i). Phần đầu của chứng minh khi đó chỉ ra rằng ma trận này có tất cả các trị riêng của nó trong K, và do đó, nếu $E \neq \{0\}$, có các vectơ riêng khác không trong E. Suy ra rằng mọi không gian con ổn định đối với u và cực tiểu nhất thiết có chiều 1, và kết luận suy ra ngay lập tức, như trong mệnh đề 4.

#### Mệnh đề 6 {#alg-ix-s7-prop-6 .statement}

a) Cho $\Psi$ là một dạng Hermit (tương ứng, dạng song tuyến tính đối xứng nếu $\mathbf{A} = \mathbf{K}$ hoặc $\mathbf{A} = \mathbf{K}(i)$) trên $E$. Tồn tại một cơ sở của $E$ trực chuẩn đối với $\Phi$ và trực giao đối với $\Psi$.

b) Giả sử $\mathbf{A} = \mathbf{K}$ hoặc $\mathbf{A} = \mathbf{K}(i)$, và cho $\Psi$ là một dạng song tuyến tính phản xứng trên $E$. Tồn tại một cơ sở của $E$ trực chuẩn đối với $\Phi$ và sao cho đối với cơ sở đó ma trận của $\Psi$ có dạng

$$
\begin{pmatrix}
0 & a_1 & 0 & 0 \ldots 0 \\
-a_1 & 0 & 0 & 0 \ldots 0 \\
0 & 0 & 0 & a_2 \ldots 0 \\
0 & 0 & -a_2 & 0 \ldots 0 \\
\cdots & \cdots & \cdots & \cdots
\end{pmatrix}.
$$

trong đó các $a_i$ là $\geqslant 0$ trong K.

Khi $\Psi$ là Hermit, mệnh đề của chúng ta suy ra ngay lập tức từ Mệnh đề 5 và sự tương ứng chính tắc giữa các dạng Hermit trên $E$ và các tự đồng cấu Hermit đối với $\Phi$. Trong hai trường hợp kia, cho $u$ là ánh xạ nửa tuyến tính từ $E$ vào chính nó được xác định ở đầu No. này bởi công thức $\Psi(x, y) = \overline{\Phi(u(x), y)}$. Khi đó $u^2$ là một ánh xạ tuyến tính đối với $\mathbf{A}$; khi $\Psi$ là đối xứng (tương ứng, phản xứng), ta có $u = u^*$ (tương ứng, $u = -u^*$), do đó $u^2$ là Hermit; do đó cũng có

$$
\Phi(u^2(x), x) = \overline{\Phi(x, u^2(x))} = \Phi(u^*(x), u(x)) = \Phi(u(x), u(x))
$$
(tương ứng, $-\Phi(u(x), u(x))$);

điều này chỉ ra rằng dạng Hermit $(x, y) \to \Phi(u^2(x), y)$ là dương (tương ứng, âm). Áp dụng Định lý 2, và cho $V$ là một phần tử cực tiểu của họ các không gian con $\neq \{0\}$ của $E$ ổn định đối với $u$ và đối với $u^*$. Vì $u^2$ là một tự đồng cấu Hermit, $V$ chứa một vectơ thực sự $x \neq 0$ của $u^2$; đặt $u^2(x) = ax$, trong đó $a \in \mathbf{K}$ (Mệnh đề 5).

Khi $\Psi$ là đối xứng, bất đẳng thức $\Phi(u^2(x), x) \geqslant 0$ chỉ ra rằng ta có $a \geqslant 0$. Đặt $y = a^{1/2}x + u(x)$; ta có $u(y) = a^{1/2}u(x) + ax = a^{1/2}y$, và $Ay$ là ổn định đối với $u$ và $u^* = u$. Nếu $y = 0$, $Ax$ là ổn định đối với $u$ và $u^*$; trong mọi trường hợp, $V$ là một không gian con có chiều 1, và kết luận của chúng ta suy ra ngay lập tức từ Định lý 2.

Khi $\Psi$ là phản xứng, ta có $a \leqslant 0$; đặt

$$
y = (-a)^{1/2}x + u(x), \quad z = (-a)^{1/2}x - u(x).
$$

Ta có $u(y) = -(-a)^{1/2}z, \ u(z) = (-a)^{1/2}y$ và
$$
\Phi(y, z) = -a\Phi(x, x) - \Phi(u(x), u(x)) = -\Phi(ax, x) + \Phi(u^2(x), x) = 0.
$$

Nếu $y = z = 0$, ta có $a = 0$ và $u(x) = 0$, do đó $Ax$ ổn định dưới tác dụng của $u$ và $u^*$, $V$ có chiều 1, và ma trận của hạn chế của $\Psi$ lên $V$ là không vì $\Psi$ là phản xứng. Ngược lại, $y$ và $z$ đều $\neq 0$, chúng sinh $V$, và vì chúng trực giao, $V$ có chiều 2 và ma trận của hạn chế của $\Psi$ lên $V$ có dạng $\begin{pmatrix} 0 & b \\ -b & 0 \end{pmatrix}$. Cuối cùng, nhờ công thức $\Psi'(x', y') = \overline{\Phi(u(x'), y')}$, ta có $\Psi'(x', y') = 0$ khi $x'$ và $y'$ thuộc hai không gian con ổn định dưới tác dụng của $u$ và trực giao đối với $\Phi$. Điều này chứng minh sự tồn tại của một cơ sở trực chuẩn của $E$ (đối với $\Phi$) sao cho ma trận của $\Psi$ đối với nó có dạng đã chỉ ra. Q.E.D.

Bài tập. — 1) Giả sử rằng các giả thiết ở đầu § 7 được thỏa mãn; cho $\Phi$ là một dạng Hermit dương trên $E$.

a) Để có $\Phi(x, x)\Phi(y, y) = \Phi(x, y)\overline{\Phi(x, y)}$, điều kiện cần và đủ là $x$ và $y$ phụ thuộc tuyến tính hoặc mặt phẳng sinh bởi $x$ và $y$ là đẳng hướng.

b) Giả sử rằng, với mọi $x \in E$, $\Phi(x, x)$ là một bình phương trong $K$. Bây giờ chứng minh rằng với mọi hai vectơ $x, y$ của $E$, ta có
$$
\sqrt{\Phi(x + y, x + y)} \leq \sqrt{\Phi(x, x)} + \sqrt{\Phi(y, y)}.
$$

Nếu $\Phi$ không suy biến, hai vế của bất đẳng thức này chỉ có thể bằng nhau khi $\alpha x + \beta y = 0$, trong đó $\alpha$ và $\beta$ là hai phần tử của $K$, không đồng thời bằng không và sao cho $\alpha \beta \leq 0$.

2) Giả sử $A = K$ hoặc $A = K(i)$. Cho $X$ là một ma trận vuông Hermit cấp $n$ trên $A$, sao cho với mọi tập con khác rỗng $H$ của $\{1, n\}$, ta có $X_{H, H} \geq 0$ (các ký hiệu của Mệnh đề 3 của No. 1).

a) Cho $\lambda$ là một phần tử $> 0$ của $K$; bây giờ chứng minh rằng ma trận $X + \lambda I$ là dương không suy biến (sử dụng Mệnh đề 3 của No. 1, lập luận bằng quy nạp theo $n$).

b) Suy ra rằng ma trận Hermit $X$ là dương.

#### Nhận xét 3 {#alg-ix-s7-n3-rem-3 .statement}

Giả sử rằng $A = K$ hoặc $A = K(i)$ và rằng $E$ là hữu hạn chiều. Cho $\Phi_1, \Phi_2$ là hai dạng Hermit dương trên $E$, và cho $V = (\alpha_{ij}), W = (\beta_{ij})$ là các ma trận của các dạng này đối với cùng một cơ sở $(e_i)$ của $E$. Chứng minh rằng dạng Hermit $\Phi$ có ma trận $(\gamma_{ij})$ đối với $(e_i)$ sao cho $\gamma_{ij} = \alpha_{ij}\beta_{ij}$ với mọi cặp chỉ số, là dương; hơn nữa, nếu $\Phi_1$ và $\Phi_2$ không suy biến, điều tương tự cũng đúng với $\Phi$. (Trong phép tính của $\Phi(x, x)$, biểu diễn các $\alpha_{ij}$ theo các giá trị $\Phi_1(c_i, c_i)$ đối với một cơ sở trực giao $(c_i)$ của $E$ đối với $\Phi_1$.)

#### Nhận xét 4 {#alg-ix-s7-n3-rem-4 .statement}

Giả sử rằng $A = K$ hoặc $A = K(i)$. Cho $R$ là một ma trận Hermit cấp $n$ trên $A$; người ta nói rằng $R$ có chữ ký $(s, t)$ nếu dạng Hermit trên $A^n$ có $R$ làm ma trận đối với cơ sở chính tắc, có chữ ký $(s, t)$. Gọi $\Delta_k$ là phần tử con chính của $R$ thu được bằng cách xóa trong $R$ các hàng và cột có chỉ số $> k$; giả sử rằng $\Delta_{s+t} \neq 0$ và rằng, với không một chỉ số $k < s + t$ nào, $\Delta_k$ và $\Delta_{k+1}$ đồng thời bằng không (xem § 6, bài tập 1 b)). Chứng minh rằng nếu $\Delta_k = 0$ với một $k < s + t$ nào đó, $\Delta_{k-1}$ và $\Delta_{k+1}$ có dấu đối nhau (phương pháp của bài tập 1 a) của § 6) và rằng số $s - t$ bằng

$$
\operatorname{sgn} \Delta_1 + \operatorname{sgn} (\Delta_1 \Delta_2) + \cdots + \operatorname{sgn} (\Delta_{s+t-1} \Delta_{s+t})
$$

(sử dụng bài tập 2 của § 6).

#### Nhận xét 5 {#alg-ix-s7-n3-rem-5 .statement}

Giả sử rằng $A = K$ hoặc $A = K(i)$; cho $R, S$ là hai ma trận Hermit trên $A$, có các chữ ký $(s, t)$ và $(s', t')$ tương ứng (bài tập 4); chứng minh rằng ma trận $R \otimes S$ là một ma trận Hermit có chữ ký $(ss' + tt', st' + s't)$.

#### Nhận xét 6 {#alg-ix-s7-n3-rem-6 .statement}

Cho $K$ là một trường có thứ tự cực đại, $L$ là một đại số đơn có hạng hữu hạn trên $K$. Nếu $(s, t)$ là chỉ số của dạng song tuyến tính đối xứng $(x, y) \to \operatorname{Tr}_{L/K}(xy)$ trên $L$, bây giờ chứng minh rằng ta có:
$s - t = m$ nếu $L$ đẳng cấu với một đại số ma trận cấp $m$ trên $K$;
$s - t = 0$ nếu $L$ đẳng cấu với một đại số ma trận trên trường $K(i)$;
$s - t = -2m$ nếu $L$ đẳng cấu với một đại số ma trận cấp $m$ trên trường quaternion trên $K$.

#### Nhận xét 7 {#alg-ix-s7-n3-rem-7 .statement}

Ta giả sử rằng $A$ thỏa mãn các điều kiện ở đầu § 7 và rằng $E$ có số chiều hữu hạn $n$. Gọi $\Phi$ là một dạng Hermit không suy biến dương trên $E$.
a) Bây giờ chứng minh rằng mọi phép đồng dạng đối với $\Phi$ có thể được viết theo một và chỉ một cách như là tích của một phép vị tự có tỉ số $\geqslant 0$ trong $K$, và một phép biến đổi unita.
b) Với mọi cơ sở $(a_i)_{1 \leq i \leq n}$ của $E$, hãy chứng minh rằng tồn tại một và chỉ một cơ sở trực chuẩn $(e_i)_{1 \leq i \leq n}$ của $E$ thỏa mãn các điều kiện sau: 1° với mọi $m$ sao cho $1 \leq m \leq n$, không gian con sinh bởi $a_1, \ldots, a_m$ là đồng nhất với không gian con sinh bởi $e_1, \ldots, e_m$; 2° ta có $\Phi(a_i, e_i) \geq 0$ trong $K$, với mọi chỉ số $i$ (xem § 6, no 1, prop. 1).
c) Suy ra từ b) rằng với mọi ma trận bình phương khả nghịch $M$ cấp $n$ trên $A$, tồn tại một và chỉ một cặp ma trận $(L, U)$ cấp $n$, sao cho $U$ là một ma trận unita, sao cho $L = (\lambda_{ij})$ chỉ có các số không bên dưới đường chéo của nó và các phần tử đường chéo $\lambda_{ii}$ thuộc $K$ và $> 0$, và cuối cùng $M = LU$.

#### Nhận xét 8 {#alg-ix-s7-n3-rem-8 .statement}

Ta giả sử $A = K$; cho $L$ là một không gian Hermit hữu hạn chiều trên $A$, có dạng mêtric dương không suy biến. Cho $M, N$ là hai phần của $L$, $u$ là một song ánh từ $M$ lên $N$ sao cho $e(u(a), u(b)) = e(a, b)$ với mọi điểm $a, b$ của $M$. Chứng minh rằng tồn tại một phép dời hình mà hạn chế của nó trên $M$ bằng $u$ (lập luận bằng quy nạp theo chiều của đa tạp tuyến tính affine sinh bởi $M$, như trong quá trình trực giao hóa Gram-Schmidt). Mệnh đề có còn đúng trong trường hợp $A$ bằng $K(i)$ hoặc trường quaternion trên $K$ không?

#### Nhận xét 9 {#alg-ix-s7-n3-rem-9 .statement}

Giả sử các điều kiện của n° 3 được thỏa mãn, và thêm vào đó $A$ là trường quaternion trên $K$. Cho $u$ là một tự đồng cấu chuẩn của $E$. Chứng minh rằng $E$ là tổng trực tiếp của các không gian con $F_k$ (1 \leq k \leq r), đôi một trực giao, sao cho trong mỗi $F_k$ tồn tại một cơ sở trực chuẩn $(e_{ik})$ (1 \leq i \leq n_k) và ta có $u(e_{ik}) = \lambda_k e_{ik}$ với $1 \leq i \leq n_k$, hai $\lambda_k$ có chỉ số khác nhau không biến đổi thành nhau bởi một tự đẳng cấu trong của $A$. Ngoài ra, nếu $(F'_k)$ là một phân tích thứ hai của $E$ có cùng các tính chất, với một hệ $(\lambda'_k)$ các giá trị riêng, thì có $F'_k = F_k$ (sai khác một phép hoán vị các chỉ số) và $\lambda'_k = \alpha_k \lambda_k \alpha_k^{-1}$; tập hợp các vectơ riêng của $u$ ứng với giá trị riêng $\lambda_k$ là không gian con trên hoán tập $A_k$ của $\lambda_k$ trong $A$, sinh bởi các $e_{ik}$ (1 \leq i \leq n_k).

#### Nhận xét 10 {#alg-ix-s7-n3-rem-10 .statement}

Giả sử các điều kiện của n° 3 được thỏa mãn, và thêm vào đó $A$ bằng $K(i)$ hoặc trường quaternion trên $K$. Cho $u$ là một tự đồng cấu chuẩn của $E$.

a) Chứng minh rằng để một không gian con vectơ $F$ của $E$ có tính chất $u(F) \subset F$, điều kiện cần và đủ là $F$ được sinh bởi các vectơ riêng của $u$; khi đó ta có $u(F^0) \subset F^0$ và $u^*(F) \subset F$.

b) Để $u$ là unita (tương ứng, để $u^* = u, u^* = -u$), điều kiện cần và đủ là với mọi giá trị riêng $\lambda$ của $u$, ta có $\lambda \overline{\lambda} = 1$ (tương ứng, $\overline{\lambda} = \lambda, \overline{\lambda} = -\lambda$).

c) Ta nói rằng một tự đồng cấu Hermit $u$ của $E$ là dương (tương ứng, dương và không suy biến) nếu dạng Hermit $(x, y) \to \Phi(u(x), y)$ tương ứng chính tắc với nó là dương (tương ứng, dương và không suy biến); điều kiện cần và đủ cho điều này là mọi giá trị riêng của $u$ đều thỏa mãn $\geq 0$ (tương ứng, $> 0$).

d) Chứng minh rằng với mọi số nguyên $m > 0$, tồn tại một tự đồng cấu chuẩn $v$ của $E$ sao cho $v^m = u$. Nếu $u$ là Hermit dương, tồn tại duy nhất một tự đồng cấu Hermit dương $v$ sao cho $v^m = u$, và tồn tại một đa thức $f \in K[X]$ sao cho $v = f(u)$ ; kết quả sau cùng này cũng đúng khi $A = K$.

#### Nhận xét 11 {#alg-ix-s7-n3-rem-11 .statement}

Giả sử các điều kiện của n° 3 được thỏa mãn, và thêm vào đó $A = K$. Cho $u$ là một tự đồng cấu chuẩn của $E$.

a) Cho $V$ là một phần tử cực tiểu của tập hợp các không gian con của $E$ khác $0$, ổn định đối với $u$ và $u^*$; chứng minh rằng nếu $V$ có chiều 2, thì hạn chế của $u$ trên $V$ là một phép đồng dạng trực tiếp với hệ số nhân $> 0$.

b) Chứng minh rằng mọi không gian con của $E$ ổn định đối với $u$ cũng ổn định đối với $u^*$. (Cho $E_0$ là không gian vectơ thu được từ $E$ bằng mở rộng trường các vô hướng đến $K(i)$; $\Phi$ là hạn chế của một dạng Hermit dương không suy biến trên $E_0$ vào $E$ và $u$ là hạn chế của một tự đồng cấu chuẩn $u_0$ của $E_0$ vào $E$ (đối với dạng này); ngoài ra $E$ là tập hợp các $x \in E_0$ bất biến bởi một song ánh nửa tuyến tính đối hợp $j$ của $E_0$, và ta có $u_0j = ju_0$. Áp dụng khi đó bài tập 10 a.).

#### Nhận xét 12 {#alg-ix-s7-n3-rem-12 .statement}

Giả sử các điều kiện của n° 3 được thỏa mãn, và thêm vào đó $A$ bằng $K(i)$ hoặc trường quaternion trên $K$. Chứng minh rằng với mọi tự đồng cấu $u$ của $E$, tồn tại một cơ sở trực chuẩn của $E$ đối với nó ma trận của $u$ chỉ có các số không bên dưới đường chéo. (Tiến hành bằng quy nạp theo chiều của $E$, bằng cách xét một vectơ riêng của $u$.)

#### Nhận xét 13 {#alg-ix-s7-n3-rem-13 .statement}

Cho $A$ là một trường thỏa mãn các điều kiện ở đầu § 7, $E, F$ là hai không gian vectơ hữu hạn chiều trên $A$, $\Phi$ (tương ứng $\Psi$) là một dạng Hermit dương không suy biến trên $E$ (tương ứng $F$). Chứng minh rằng, với mọi ánh xạ tuyến tính $u$ từ $E$ vào $F$, tự đồng cấu liên hợp $u^*$ của $u$ (đối với $\Phi$ và $\Psi$; cf. § 1, no 8) có tính chất $u^*u$ và $uu^*$ là các tự đồng cấu Hermit dương (bài tập 10 c)) của $E$ và $F$ tương ứng.

#### Nhận xét 14 {#alg-ix-s7-n3-rem-14 .statement}

Giả sử các điều kiện của no 3 được thỏa mãn. Cho $u$ là một tự đồng cấu của $E$, $h_1, h_2$ là hai tự đồng cấu Hermit dương của $E$, sao cho $h_1^2 = u^*u, h_2^2 = uu^*$ (bài tập 13 và 10 d)).

a) Chứng minh rằng tồn tại một tự đồng cấu unita $\nu$ sao cho $u = \nu h_1 = h_2 \nu$ và đặc biệt $h_1$ và $h_2$ đồng dạng (nhận xét rằng $u(0) = \overline{h_1}(0)$ và rằng nếu $V$ là không gian con trực giao với $\overline{u}(0)$, ta có $\Phi(u(x), u(x)) = \Phi(h_1(x), h_1(x))$ với mọi $x \in V$. Để $\nu$ được xác định duy nhất, điều kiện cần và đủ là $u$ song ánh. Để có thể chọn $\nu$ hoán tập được với $h_1$, điều kiện cần và đủ là $u$ chuẩn.

b) Suy ra từ a) rằng mọi ma trận bình phương $M$ cấp $n$ trên $A$ có thể được viết $UDV$, trong đó $U$ và $V$ là các ma trận unita và $D$ là một ma trận đường chéo mà các phần tử của nó là $\geqslant 0$, và các bình phương của chúng là các trị riêng của $MM^*$.

#### Nhận xét 15 {#alg-ix-s7-n3-rem-15 .statement}

Giả sử các điều kiện của No. 3 được thỏa mãn. Chứng minh rằng mọi ma trận Hermit dương $H$ trên $A$ có thể được viết dưới dạng $LL^*$, trong đó $L = (\lambda_{ij})$ chỉ có các số 0 bên dưới đường chéo của nó và các phần tử đường chéo thuộc $K$ và $\geqslant 0$; hơn nữa $L$ được xác định duy nhất bởi các điều kiện này khi $H$ khả nghịch (xem Bài tập 10 d) và 7 c)).

#### Nhận xét 16 {#alg-ix-s7-n3-rem-16 .statement}

Giả sử các điều kiện của No. 3 được thỏa mãn và thêm vào đó $A = K(i)$. Cho $u$ là một tự đồng cấu của $E$.

a) Tập hợp các trị riêng của $u$ được chứa trong tập hợp $U$ gồm các giá trị của $\Phi(x, u(x))$ khi $x$ chạy qua tập hợp các phần tử của $E$ sao cho $\Phi(x, x) = 1$.

b) Một tập con $C$ của $A = K(i)$ được gọi là lồi nếu, với mọi cặp phần tử $(\xi, \eta) \in C^2$ và mọi $\tau \in K$ sao cho $0 \leqslant \tau \leqslant 1$ ta có $\tau \xi + (1-\tau)\eta \in C$. Chứng minh rằng tập hợp $U$ là lồi. (Rút gọn về trường hợp $n = 2$; bằng cách viết $u$ dưới dạng $\nu + i\omega$, trong đó $\nu$ và $\omega$ là Hermit, và bằng cách thay thế nếu cần $u$ bởi $\lambda u$, trong đó $\lambda \in A$ và $\lambda \overline{\lambda} = 1$, chứng minh rằng mọi thứ quy về việc chứng minh tính chất sau. Cho $f(\xi_1, \xi_2) = \xi_1 \overline{\xi}_1 + \xi_2 \overline{\xi}_2$, $g(\xi_1, \xi_2) = a \xi_1 \overline{\xi}_1 + b \xi_2 \overline{\xi}_2$ ($a \in K, b \in K$), $h(\xi_1, \xi_2) = \alpha \xi_1 \overline{\xi}_1 + \beta \xi_1 \overline{\xi}_2 + \beta \xi_2 \overline{\xi}_1 + \gamma \xi_2 \overline{\xi}_2$ ($\alpha \in K, \gamma \in K, \beta \in A$); cho $(\eta_1, \eta_2) \in A^2, (\zeta_1, \zeta_2) \in A^2$ sao cho $f(\eta_1, \eta_2) = f(\zeta_1, \zeta_2) = 1$, $g(\eta_1, \eta_2) = g(\zeta_1, \zeta_2) = 1$, $h(\eta_1, \eta_2) > 0$, $h(\zeta_1, \zeta_2) < 0$; khi đó tồn tại $(theta_1, theta_2) \in A^2$ sao cho $f(\theta_1, \theta_2) = 1$, $g(\theta_1, \theta_2) = 1$ và $h(\theta_1, \theta_2) = 0$. Trước hết sẽ nhận thấy rằng với mọi cặp $(\xi_1, \xi_2)$, tồn tại $\mu \in A$ sao cho $\mu \overline{\mu} = 1$ và $\beta \mu \xi_1 \overline{\xi}_2 + \beta \mu \xi_2 \overline{\xi}_1 = 0$, điều này sẽ cho phép rút gọn về trường hợp $\beta = 0$; dùng Mệnh đề 5 của Chương VI, § 2, No. 5.)

c) Chứng minh rằng nếu $u$ là chuẩn tắc, $U$ là tập hợp lồi nhỏ nhất chứa tất cả các trị riêng của $u$. Cho một ví dụ trong đó $u$ không chuẩn tắc nhưng $U$ vẫn có tính chất trước đó. (Lấy làm các trị riêng của $u$ các phần tử $\pm 1 \pm i$ như các trị riêng đơn, và 0 như một trị riêng kép.)

#### Nhận xét 17 {#alg-ix-s7-n3-rem-17 .statement}

Giả sử các điều kiện của No. 3 được thỏa mãn; với mọi $\xi \in A$, ký hiệu $|\xi|$ là phần tử $\rho \geqslant 0$ của K sao cho $\rho^2 = \xi \overline{\xi}$ (giá trị tuyệt đối của $\xi$). Với mọi ma trận vuông $M = (\alpha_{ij})$ trên A, đặt $f(M) = \max_i |\alpha_{ii}|$, $g(M) = \max_{i,j} |\alpha_{ij}|$, và ký hiệu $\varphi(M)$ là giá trị tuyệt đối lớn nhất của các trị riêng của $M$ (người ta sẽ chứng minh rằng định nghĩa này có ý nghĩa khi A là trường quaternion trên K).

a) Cho $A, B, D$ là ba ma trận vuông cấp $n$ trên A. Chứng minh rằng nếu $D$ là đường chéo, ta có

$$
g^2(ADB^*) \leq f^2(D)f(AA^*)f(BB^*)
$$
(sử dụng bất đẳng thức (1) của No. 1). Suy ra rằng
$$
g(ABB^*A^*) \leq f(AA^*)\varphi(BB^*)
$$
(áp dụng Mệnh đề 5 cho ma trận Hermit $BB^*$). Suy ra rằng, với $m$ ma trận vuông tùy ý $A_i$ ($1 \leq i \leq m$) trên A, ta có
$$
g^2(A_1A_2\ldots A_m) \leq f(A_1A_1^*)\varphi(A_2A_2^*)\ldots\varphi(A_{m-1}A_{m-1}^*)f(A_m^*A_m)
$$
$$
\varphi^2(A_1A_2\ldots A_m) \leq \varphi(A_1A_1^*)\varphi(A_2A_2^*)\ldots\varphi(A_mA_m^*)
$$
$$
g^2(A_1A_2\ldots A_m) \leq \varphi(A_1A_1^*)\ldots\varphi(A_mA_m^*).
$$
(Đối với (3), lập luận bằng quy nạp từ (2). Đối với (4), dùng Bài tập 12; cuối cùng suy ra (5) từ (3).)

Chứng minh rằng bất đẳng thức (3) không còn nhất thiết đúng khi $A_m^*A_m$ được thay thế ở đó bởi $A_mA_m^*$ (nhận xét rằng có thể có $f(A^*A) \neq f(AA^*)$), hoặc khi $\varphi(A_iA_i^*)$ được thay thế bởi $f(A_iA_i^*)$ với $2 \leq i \leq m-1$ (lấy tất cả các $A_i$ bằng ma trận vuông mà mọi phần tử đều bằng 1).

b) Cho $u$ là một tự đồng cấu chuẩn của E; nếu $\lambda$ là một trị riêng của $u$ (phần tử của $K(i)$ khi $A = K$), $\overline{\lambda}$ là một trị riêng của $u^*u$. Với mọi ma trận chuẩn $M$ (ma trận của một tự đồng cấu chuẩn của E đối với một cơ sở trực chuẩn), do đó ta có $\varphi^2(M) = \varphi(MM^*)$. Suy ra rằng ta cũng có $g(M) \leq \varphi(M)$, và tổng quát hơn, nếu $M_1, \ldots, M_m$ là chuẩn,
$$
g(M_1\ldots M_m) \leq \varphi(M_1)\ldots\varphi(M_m)
$$
$$
\varphi(M_1\ldots M_m) \leq \varphi(M_1)\ldots\varphi(M_m)
$$
(dùng (4) và (5)).

c) Chứng minh rằng nếu $H$ là một ma trận Hermit dương trên A, ta có $f(H) = g(H) \leq \varphi(H)$ (dùng (3) và b), bằng cách viết $H = AA^*$.

#### Nhận xét 18 {#alg-ix-s7-n3-rem-18 .statement}

Các điều kiện của No. 3 được giả sử thỏa mãn.

a) Với mọi tự đồng cấu $u$ của $E$, cho $(e_i)$ là một cơ sở trực chuẩn của $E$ được tạo thành bởi các vectơ riêng của $u^*u$, và cho $\rho_i$ là trị riêng của $u^*u$ tương ứng với vectơ $e_i$; đặt $s(u) = (\sum_{i=1}^n \rho_i)^{1/2}$ (căn bình phương của $\operatorname{Tr}(u^*u)$ khi $A$ giao hoán); ta có $s(u^*) = s(u)$. Nếu $u, v$ là hai tự đồng cấu của $E$, $U, V$ là các ma trận của chúng đối với cùng một cơ sở trực chuẩn của $E$, chứng minh rằng đối với ma trận $UV^* + VU^*$, với các phần tử trong $K$, ta có $(\operatorname{Tr}(UV^* + VU^*))^2 \leq 4s(u)s(v)$ (nhận xét rằng $(u^* + \lambda v^*)(u + \lambda v)$ là Hermit dương với mọi $\lambda \in K$); suy ra rằng $s(u + v) \leq s(u) + s(v)$. Nếu ngoài ra $A$ giao hoán, ta có

$$
|\operatorname{Tr}(uv)|^2 \leq s(u)s(v) \quad \text{và} \quad |\operatorname{Tr}(u)| \leq \sqrt{n}s(u)
$$

(viết $u$ thành một tích bằng cách dùng Bài tập 14 b)).

b) Giả sử thêm rằng $A$ là giao hoán (do đó bằng $K$ hoặc $K(i)$). Nếu $H_1, H_2$ là hai ma trận vuông Hermit dương, bây giờ chứng minh rằng ta có $\operatorname{Tr}(H_1H_2) \geq 0$ (rút gọn về trường hợp $H_2$ là một ma trận đường chéo). Suy ra rằng ta có (các ký hiệu của Bài tập 17)

$$
|\operatorname{Tr}(H_1H_2)| \leq \varphi(H_1)\operatorname{Tr}(H_2) \leq \operatorname{Tr}(H_1)\operatorname{Tr}(H_2).
$$

Kết luận từ các bất đẳng thức này rằng đối với hai tự đồng cấu tùy ý $u, v$ của $E$, khi đó ta có $s(uv) \leq s(u)s(v)$.

c) Vẫn giả sử rằng $A$ là giao hoán, cho $\prod_{i=1}^n (x - \lambda_i)$ là phân tích thành các nhân tử tuyến tính của đa thức đặc trưng của một tự đồng cấu tùy ý $u$ của $E$; bây giờ chứng minh rằng ta có $\sum_{i=1}^n |\lambda_i|^2 \leq (s(u))^2$ và rằng, để hai vế của bất đẳng thức này bằng nhau, điều kiện cần và đủ là $u$ là chuẩn (dùng Bài tập 12).

#### Nhận xét 19 {#alg-ix-s7-n3-rem-19 .statement}

Giả sử các điều kiện của No. 3 được thỏa mãn. Cho $M$ là một ma trận vuông cấp $n$ trên $A$; bây giờ chứng minh rằng đối với mọi ma trận con vuông $N$ của $M$ (thu được bằng cách xóa trong $M$ một số hàng và các cột có cùng các chỉ số với các hàng đó), ta có (các ký hiệu của Bài tập 17) $\varphi^2(N) \leq \varphi(MM^*)$ (áp dụng thích hợp công thức (4) của Bài tập 17). Nếu đặc biệt $M$ là một ma trận chuẩn, $\varphi(N) \leq \varphi(M)$ (xem Bài tập 17 b)).

#### Nhận xét 20 {#alg-ix-s7-n3-rem-20 .statement}

Giả sử các điều kiện của No. 3 được thỏa mãn và thêm vào đó $A$ bằng $K$ hoặc $K(i)$. Áp dụng các kết quả của các Bài tập 17 đến 19 cho mở rộng của $\Phi$ tới các lũy thừa ngoài thứ $p$ (§ 1, No. 9) và cho các lũy thừa ngoài thứ $p$ của các tự đồng cấu hoặc các ma trận được xét. Đặc biệt, bây giờ chứng minh rằng, nếu $\prod_{i=1}^n (X - \lambda_i)$ và $\prod_{i=1}^n (X - \rho_i^2)$ là các phân tích thành các nhân tử tuyến tính của các đa thức đặc trưng của một tự đồng cấu $u$ của $E$ và của tự đồng cấu $u^*u$, và nếu giả sử $|\lambda_i| \geqslant |\lambda_{i+1}|$ và $\rho_i \geqslant \rho_{i+1} \geqslant 0$ với $1 \leqslant i \leqslant n-1$, thì ta có
$$
|\lambda_1 \lambda_2 \ldots \lambda_h| \leqslant \rho_1 \rho_2 \ldots \rho_h
$$
với $1 \leqslant h \leqslant n-1$ và $|\lambda_1 \lambda_2 \ldots \lambda_n| = \rho_1 \rho_2 \ldots \rho_n$.

#### Nhận xét 21 {#alg-ix-s7-n3-rem-21 .statement}

Giả sử các điều kiện của No. 3 được thỏa mãn. Cho $u$ là một tự đồng cấu Hermit của $E$ và cho $\prod_{i=1}^n (X-\lambda_i)$ là phân tích thành các nhân tử tuyến tính của đa thức đặc trưng của nó; giả sử $\lambda_i \geqslant \lambda_{i+1}$ với $1 \leqslant i \leqslant n-1$.

a) Bây giờ chứng minh rằng giá trị lớn nhất (tương ứng, giá trị nhỏ nhất) của các trị riêng $\lambda_i$ trong $K$ bằng giá trị lớn nhất (tương ứng, giá trị nhỏ nhất) của các giá trị của $\Phi(u(x), x)$ khi $x$ chạy trên tập hợp các $x \in E$ sao cho $\Phi(x, x) = 1$. (Lập luận trực tiếp, hoặc áp dụng Bài tập 16 c) bằng cách rút gọn về trường hợp $A = K(i)$ ($§ 3$, Bài tập 4).)

b) Gọi $\Psi_v$ là hạn chế của dạng Hermit $\Psi'$ liên kết với $u$ lên không gian con vectơ $V$ của $E$, và gọi $u_v$ là tự đồng cấu Hermit của $V$ liên kết với $\Psi_v$. Bây giờ chứng minh rằng $\lambda_k$ là nhỏ nhất trong các trị riêng lớn nhất của các $u_v$, khi $V$ chạy qua tập hợp các không gian con vectơ của $E$ có chiều $n-k+1$ (dùng Mệnh đề 5).

#### Nhận xét 22 {#alg-ix-s7-n3-rem-22 .statement}

Giả sử các điều kiện của No. 3 được thỏa mãn, và ngoài ra $A$ bằng $K(i)$ hoặc bằng trường các quaternion trên $K$. Cho $u, v$ là hai tự đồng cấu chuẩn của $E$; gọi $(E_i)_{1 \leqslant i \leqslant r}$ (resp. $(F_j)_{1 \leqslant j \leqslant s}$) là phân tích của $E$ thành tổng trực tiếp của các không gian con trực giao từng đôi một, sao cho trong $E_i$ (resp. $F_j$) có một cơ sở trực chuẩn được tạo thành bởi các vectơ riêng của $u$ (resp. $v$) ứng với cùng trị riêng $\lambda_i$ (resp. $\mu_j$), và $\lambda_h$ và $\lambda_i$ (resp. $\mu_j$ và $\mu_k$) không được biến đổi thành nhau bởi một tự đẳng cấu trong của $A$ nếu $h \neq i$ (resp. $j \neq k$) (xem Mệnh đề 4 và Bài tập 9). Để một tự đồng cấu $w$ của $E$ sao cho $uw = vw$, điều kiện cần và đủ là với mọi $j$ ($1 \leqslant j \leqslant s$), $w(F_j)$ được chứa trong một trong các $E_i$ và ảnh bởi $w$ của mọi vectơ riêng của $v$ tương ứng với trị riêng $\mu_j$ là một vectơ riêng của $u$ tương ứng với trị riêng $\mu_j$ (điều này đặc biệt suy ra rằng $\mu_j$ và $\lambda_i$ được biến đổi thành nhau bởi một tự đẳng cấu trong của $A$). Suy ra rằng nếu điều này xảy ra, thì $u^*w = wv^*$.

#### Nhận xét 23 {#alg-ix-s7-n3-rem-23 .statement}

Giả sử các điều kiện của No. 3 được thỏa mãn. Cho $u$ và $v$ là hai tự đồng cấu của $E$.

a) Giả sử rằng $u$ và $uv$ là chuẩn. Để $vu$ là chuẩn, điều kiện cần và đủ là $v$ và $u^*u$ giao hoán. (Để thấy rằng điều kiện là cần, dùng quan hệ $u(vu) = (uv)u$ và Bài tập 22; để thấy rằng điều kiện là đủ, dùng Bài tập 14 a) và 10 d).)

b) Giả sử rằng $u, v$ và $uv$ là chuẩn; gọi $\beta$ là trị riêng lớn nhất của $uu^*$, và gọi $F$ là không gian con của $E$ tạo bởi các vectơ riêng của $uu^*$ tương ứng với trị riêng $\beta$. Bây giờ chứng minh rằng $v(F) \subset F$. (Nhận xét rằng đối với mọi tự đồng cấu chuẩn $u$ và mọi $x \in E$, ta có
$$
\Phi(u(x), u(x)) = \Phi(u^*(x), u^*(x)).
$$)

Rút gọn về trường hợp A bằng K(i) hoặc trường quaternion trên K; khi đó F có một cơ sở tạo bởi các vectơ riêng của u (và u*); nhận xét rằng đối với một vectơ z như vậy, ta có $\Phi(u^*u v(z), v(z)) = \beta \Phi(v(z), v(z))$. Suy ra rằng νu là chuẩn (lý luận bằng quy nạp theo số các trị riêng phân biệt của $u^*u$). Nếu h (tương ứng $h'$) là tự đồng cấu Hermit dương sao cho $h^2 = uu^*$ (tương ứng ${h'}^2 = \nu \nu^*$) và nếu đặt $u = hu_1, \nu = h'\nu_1$, trong đó $u_1$ và $\nu_1$ là unita, h hoán vị được với $u_1$ và $h'$ với $\nu_1$ (Bài tập 14 a)), chứng minh rằng các cặp $(h, h'), (h, \nu_1)$ và $(h', u_1)$ là hoán vị được; đảo lại. Suy ra rằng $u^m \nu^n, \nu^n u^m, u \nu^*$ và $\nu^* u$ khi đó là chuẩn ($m$ và $n$ là các số nguyên tùy ý $> 0$).

#### Nhận xét 24 {#alg-ix-s7-n3-rem-24 .statement}

Giả sử rằng các điều kiện của No. 3 được thỏa mãn. Cho $\Gamma$ là một nhóm các tự đẳng cấu của E sao cho mọi $u \in \Gamma$ đều là chuẩn. Bây giờ chứng minh rằng tồn tại một phân tích của E thành tổng trực tiếp các không gian con $E_k$ ($1 \leq k \leq r$) trực giao từng đôi một, sao cho hạn chế trên $E_k$ của mọi $u \in \Gamma$ có dạng $\lambda_k \nu_k$, trong đó $\lambda_k$ là một phần tử $> 0$ của K và trong đó $\nu_k$ là một tự đồng cấu unita của $E_k$ (phân tích mỗi $u \in \Gamma$ dưới dạng $h \nu$, trong đó $\nu$ là unita, h Hermit dương và $h^2 = uu^*$ (Bài tập 14 a)); dùng Bài tập 23 b) và áp dụng hệ quả 2 của định lý 2 cho đại số sinh bởi các tự đồng cấu Hermit h tương ứng với các $u \in \Gamma$. Suy ra rằng nếu $\Gamma$ là hữu hạn, các phần tử $u \in \Gamma$ là unita.

#### Nhận xét 25 {#alg-ix-s7-n3-rem-25 .statement}

Giả sử rằng $A = K$ (trường có thứ tự cực đại). Cho L là một không gian Euclid có chiều $n$ trên A, có dạng mêtric dương không suy biến.

Cho S là một mặt bậc hai affine không suy biến trong L (§ 6, Bài tập 25). Nếu S có một tâm $a$ và nếu lấy $a$ làm gốc trong L, bây giờ chứng minh rằng tồn tại một cơ sở trực chuẩn $(e_i)$ của L sao cho, đối với cơ sở này, S có phương trình $\lambda_1 \xi_1^2 + \cdots + \lambda_n \xi_n^2 = 1$. Hơn nữa, nếu hai cơ sở trực chuẩn có tính chất này, các phần tử $\lambda_i \in K$ tương ứng với chúng là như nhau sai khác một hoán vị.

Nếu S không có tâm, hãy chứng minh rằng tồn tại một điểm $b$ của S và (lấy $b$ làm gốc) một cơ sở trực chuẩn của L sao cho, đối với cơ sở này, S có phương trình $\lambda_1 \xi_1^2 + \cdots + \lambda_{n-1} \xi_{n-1}^2 + \xi_n = 0$. (Nếu $\overline{S}$ là mặt bậc hai xạ ảnh sao cho $S = L \cap \overline{S}$, hãy xác định $b$ bởi điều kiện rằng đường thẳng đi qua $b$ và $c$ vuông góc với siêu phẳng tiếp xúc với S tại điểm $b$, trong đó c là cực (tại vô cực) đối với $\overline{S}$ của siêu phẳng tại vô cực $H_0$).

#### Nhận xét 26 {#alg-ix-s7-n3-rem-26 .statement}

a) Cho K là một trường giao hoán, S là một tập con của K sao cho K là một trường có thứ tự cực đại S (chương VI, § 2, bài tập 8). Cho $f$ là một đa thức của $K[X]$, L là trường các nghiệm của nó. Hãy chứng minh rằng nếu, đối với mọi cấu trúc cấp (toàn phần) trên K tương thích với cấu trúc vành của nó, L nhận một cấu trúc của một mở rộng có thứ tự của K, thì tất yếu $L = K$. (Lập luận bằng phản chứng: tiến hành như trong bài tập 8 e) của chương VI, § 2, rút gọn về trường hợp ta có $[L : K] = 2$. Kết luận bằng cách nhận thấy rằng nếu $b \in K$ không là một bình phương, thì tồn tại một cấu trúc cấp toàn phần trên K, tương thích với cấu trúc vành của nó, mà đối với nó $b < 0$ (xem chương VI, § 2, no. 3, bổ đề của định lý 1)).

b) Hãy mở rộng các kết quả của no. 3 (ngoại trừ mệnh đề 6) về trường hợp K là một trường có thứ tự cực đại S (*). (Bắt đầu bằng cách chứng minh tương tự của mệnh đề 5, sử dụng a). Tiếp theo hãy thiết lập tương tự của hệ quả 2 của định lý 2 cho trường hợp đại số giao hoán B gồm các tự đồng cấu Hermit, sử dụng mệnh đề 10 của chương VIII, § 9, no. 4. Chuyển qua trường hợp của một tự đồng cấu chuẩn tắc u đối với A = K(i), bằng cách nhận thấy rằng khi đó có thể viết $u = v + i w$, trong đó v và w là Hermit và hoán vị được. Cuối cùng, nếu A là trường quaternion trên K, E_0 là không gian E được xét như một không gian vectơ chiều 2n trên K(i), và nếu đặt $\Phi(x, y) = \Phi_1(x, y) + \Phi_2(x, y)i$, trong đó $\Phi_1$ và $\Phi_2$ nhận giá trị trong K(i), hãy nhận thấy rằng nếu u là chuẩn tắc đối với $\Phi$, thì nó cũng là chuẩn tắc đối với $\Phi_1$.)

#### Nhận xét 27 {#alg-ix-s7-n3-rem-27 .statement}

Cho K là một trường có thứ tự cực đại, E là một không gian vectơ chiều n trên K, $\Phi$ là một dạng song tuyến tính đối xứng không suy biến trên E, có chỉ số $(s, t)$ phân biệt với $(n, 0)$ và với $(0, n)$. Cho $(e_i)$ là một cơ sở trực giao đối với $\Phi$, sao cho $\Phi(e_i, e_i) = 1$ với $1 \leq i \leq s$, $\Phi(e_i, e_i) = -1$ với $s+1 \leq i \leq n$. Đối với mọi biến đổi trực giao $u \in \mathbf{U}(\Phi)$, đặt

$$
U = \begin{pmatrix} M & N \\ P & Q \end{pmatrix}
$$

là ma trận của u đối với $(e_i)$, được viết dưới dạng một bảng vuông của các ma trận tương ứng với phân hoạch của $(1, n)$ thành $(1, s)$ và $(s+1, n)$.

a) Chứng minh các hệ thức

$$
\begin{align*}
{}^tM \cdot M - {}^tP \cdot P &= I_s \\
{}^tQ \cdot Q - {}^tN \cdot N &= I_t \\
{}^tM \cdot N - {}^tP \cdot Q &= 0.
\end{align*}
$$

b) Cho R là một ma trận trên K có t hàng và s cột, sao cho $I_s - {}^tR \cdot R$ là ma trận của một dạng Hermit dương không suy biến (trên $K^s$). Hãy chứng minh rằng $\det(M + \lambda NR)$ không đổi dấu đối với $-1 \leq \lambda \leq 1$ trong K (hãy chứng minh, sử dụng a), rằng ${}^t(M + \lambda NR)(M + \lambda NR)$ là ma trận của một dạng đối xứng dương không suy biến).

c) Đặt $\sigma(u) = \sigma(U) = \operatorname{sgn}(\det M)$; hãy chứng minh rằng, đối với hai phần tử bất kỳ u, v của nhóm trực giao $\mathbf{U}(\Phi)$, ta có $\sigma(uv) = \sigma(u)\sigma(v)$ (sử dụng a) và b)). Suy ra rằng nhóm giao hoán tử của nhóm trực giao đặc biệt $\mathbf{SU}(\Phi)$ là phân biệt với $\mathbf{SU}(\Phi)$ (xem § 10, bài tập 9).
