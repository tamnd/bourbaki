---
book: evt
book_title: Topological Vector Spaces
chapter: II
chapter_title: CONVEX SETS AND LOCALLY CONVEX SPACES
section: 7
section_title: Extremal points and extremal generators
lang: vi
source: evt-i-v
book_pages: TVS II.54-TVS II.60, TVS II.87-TVS II.95
pdf_pages: 0091-0097, 0124-0132
extraction: ocr
subsections:
    - "no": 1
      title: Extremal points of compact convex sets
      page: 54
      pdf_page: 91
    - "no": 2
      title: Extremal generators of convex cones
      page: 57
      pdf_page: 94
    - "no": 3
      title: Convex cones with compact sole
      page: 59
      pdf_page: 96
statements: 25
exercises: 41
content_sha256: 60507908e102514ec0b9c54e87ae98a572e5242d6bb4f4d9c4521dbee84b74b1
translated_from: content/en/evt/II/07_s7_extremal_points_and_extremal_generators.md
source_content_sha256: bf23b70355aed84093184969e6c0730616120ed746f1eb87003a705d19e73634
translation_model: gpt-5-6, gpt-5-6-mini
translation_run: translate-vi-4bb1b7cf
glossary_version: 34
glossary_terms_sha256: 27fb439d820fcc96e1fcb953f29badd0182f4c9e2bd3fa9b9a61fcc3fa1ac8ca
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 7. CÁC ĐIỂM CỰC BIÊN VÀ CÁC PHẦN TỬ SINH CỰC BIÊN

### 1. Các điểm cực biên của các tập lồi compact

#### Định nghĩa 1 {#evt-ii-s7-def-1 .statement}

Cho $A$ là một tập lồi trong một không gian afin $E$. Khi đó ta nói rằng một điểm $x \in A$ là một điểm cực biên của $A$ nếu không tồn tại một đoạn mở nào được chứa trong $A$ và chứa $x$.

Nói cách khác, các quan hệ $x = \lambda y + (1 - \lambda)z,\ y \in A,\ z \in A,\ y \neq z$ và $0 \leq \lambda \leq 1$ kéo theo $\lambda = 0$ hoặc $\lambda = 1$ (do đó $x = y$ hoặc $x = z$). Điều này kéo theo rằng $x$ không thể là trọng tâm của một tập hợp gồm $n$ điểm $x_i$ của $A$ mang các khối lượng dương, trừ khi $x$ là một trong các $x_i$; vì đây chính là định nghĩa khi $n = 2$; với $n$ tùy ý, hãy lập luận bằng quy nạp theo $n$, vì $x$ là trọng tâm của $x_1$ và của trọng tâm $y_1$ của các $x_i$ với $2 \leq i \leq n$, do đó $x$ đồng nhất với $x_1$ hoặc $y_1$, và trong trường hợp thứ hai chỉ cần áp dụng giả thiết quy nạp.

Nói rằng $x$ là một điểm cực biên của $A$ cũng có nghĩa là $A - \{x\}$ là lồi.

#### Ví dụ 1 {#evt-ii-s7-n1-exa-1 .statement}

Trong không gian $\mathbf{R}^n$, mọi điểm của mặt cầu $S_{n-1}$ đều là các điểm cực biên của quả cầu đóng $B_n$. Thật vậy, nếu $\sum_i y_i^2 \leq 1,\ \sum_i z_i^2 \leq 1$ và $0 < \lambda < 1$, quan hệ
$$
\lambda^2 \sum_i y_i^2 + (1 - \lambda)^2 \sum_i z_i^2 + 2\lambda(1 - \lambda) \sum_i y_i z_i = 1 = (\lambda + (1 - \lambda))^2
$$
chỉ có thể xảy ra nếu
$$
\sum_i y_i^2 = \sum_i z_i^2 = \sum_i y_i z_i = 1.
$$
Nhưng điều này kéo theo $\sum_i (y_i - z_i)^2 = 0$, do đó $y_i = z_i$ với mọi $i$, điều này chứng minh mệnh đề của chúng ta.

#### Ví dụ 2 {#evt-ii-s7-n1-exa-2 .statement}

Trong không gian định chuẩn $\mathcal{B}(\mathbf{N})$ của các dãy bị chặn của các số thực (I, p. 4), các điểm cực biên của quả cầu đơn vị là các điểm $x = (\xi_n)$ sao cho $|\xi_n| = 1$ với mọi $n$. Thật vậy, giả sử ta có $|\xi_n| \leq 1$ với mọi $n$ và $|\xi_p| < 1$ đối với một chỉ số $p$. Khi đó ta có thể viết
$$
x = \frac{1 + \xi_p}{2} y + \frac{1 - \xi_p}{2} z
$$
trong đó $y$ (resp. $z$) là điểm mà tất cả các tọa độ của nó bằng tọa độ của $x$ có cùng chỉ số, trừ trường hợp chỉ số $p$ trong đó tọa độ bằng 1 (resp. $-1$). Điều này chứng tỏ rằng $x$ không là cực biên, vì ta có $\|y\| \leq 1$ và $\|z\| \leq 1$. Ngược lại, nếu $|\xi_n| = 1$ với mọi $n$, thì $x$ là cực biên, vì quan hệ $\xi_n = \lambda \eta_n + (1 - \lambda) \zeta_n$ với $|\eta_n| \leq 1,\ |\zeta_n| \leq 1$ và $0 < \lambda < 1$ kéo theo $\xi_n = \eta_n = \zeta_n$.

#### Ví dụ 3 {#evt-ii-s7-n1-exa-3 .statement}

Cho $u : E \to E'$ là một ánh xạ afin của một không gian afin $E$ vào một không gian afin $E'$; cho $C \subset E,\ C' \subset E'$ là hai tập lồi sao cho $u(C) \subset C'$. Nếu $x'$ là một điểm cực biên của $C'$ và $x$ là một điểm cực biên của $u^{-1}(x') \cap C$, thì $x$ là một điểm cực biên của $C$, như suy ra từ định nghĩa 1.

#### Mệnh đề 1 {#evt-ii-s7-prop-1 .statement}

Cho $B$ là tập hợp các điểm cực biên của $A$, một tập lồi compact không rỗng trong một không gian lồi địa phương Hausdorff $E$, và cho $f$ là một hàm lồi xác định trong $A$ và nửa liên tục trên. Khi đó $f$ đạt cận trên của nó trong $A$ tại ít nhất một điểm của $B$.

Dùng $\mathcal{F}$ để ký hiệu họ các tập con X của A là *không rỗng, đóng và sao cho mọi đoạn mở được chứa trong A và gặp X nhất thiết nằm trong X*. Họ này có các tính chất sau;
(i) A thuộc $\mathcal{F}$.
(ii) Một điểm $a \in A$ sao cho $\{a\} \in \mathcal{F}$, khi và chỉ khi, $a$ là một điểm cực biên của A.
(iii) Mọi giao không rỗng X của một họ $(X_\alpha)$ các tập hợp của $\mathcal{F}$ cũng thuộc $\mathcal{F}$.

Các tính chất (i), (ii) và (iii) suy ra ngay lập tức từ các định nghĩa.

(iv) Cho $X \in \mathcal{F}$, và cho $h$ là một hàm lồi và nửa liên tục trên trong A; khi đó tập hợp Y gồm các điểm của X tại đó hạn chế $h|X$ đạt cận trên của nó trong X có tính chất là Y thuộc $\mathcal{F}$.

Vì $h|X$ nửa liên tục trên trong X đạt cận trên của nó $\alpha$ trên X tại ít nhất một điểm của X (GT, IV, § 6.2, th. 3); do đó Y không rỗng, nó cũng đóng (GT, IV, § 6.2, mệnh đề 1). Mặt khác, cho $x, y$ là hai điểm phân biệt của A và cho $z = \lambda x + (1 - \lambda) y$ là một điểm của Y sao cho $0 < \lambda < 1$; vì $Y \subset X$ và $X \in \mathcal{F}$, ta có $x \in X$ và $y \in X$; mặt khác, vì $h$ là lồi, ta có

$$
h(z) \leq \lambda h(x) + (1 - \lambda) h(y)
$$

nhưng vì $h(x) \leq \alpha, h(y) \leq \alpha$ và $h(z) = \alpha$, tất yếu $h(x) = h(y) = \alpha$, tức là $x \in Y$ và $y \in Y$. Do đó $Y \in \mathcal{F}$.

Sau khi đã thiết lập các tính chất này, cho M là tập hợp các $x \in A$ tại đó $f$ đạt cận trên của nó trong A; theo (iv), $M \in \mathcal{F}$. Mặt khác, theo (iii) và sự kiện rằng các tập hợp của $\mathcal{F}$ là các tập con đóng của tập compact A, suy ra rằng $\mathcal{F}$ là *quy nạp* đối với quan hệ thứ tự $\supset$. Theo định lý 2 của S, III, § 2.4, M chứa một tập con N là một phần tử cực tiểu của $\mathcal{F}$. Ta sẽ chỉ ra rằng N gồm một điểm duy nhất và điều này sẽ hoàn tất chứng minh của mệnh đề. Vì E là một không gian lồi địa phương Hausdorff, chỉ cần chứng minh rằng mọi dạng tuyến tính liên tục $u$ trên E là hằng trong N (II, p. 38, hệ quả 1). Bây giờ từ (iv) suy ra rằng tập hợp $N'$ của các $x \in N$ tại đó $u|N$ đạt cận trên của nó trong N có tính chất là $N'$ thuộc về $\mathcal{F}$; vì N là cực tiểu trong $\mathcal{F}$ nên tất yếu ta có $N' = N$.

#### Hệ quả {#evt-ii-s7-n1-cor-1 .statement}

*Cho A là một tập compact lồi trong một không gian lồi địa phương Hausdorff E. Khi đó mọi siêu phẳng đỡ đóng H của A chứa ít nhất một điểm cực trị của A.*

Vì, nếu $f(x) = \alpha$ là một phương trình của H và $f(x) \leq \alpha$ trong A, chỉ cần áp dụng mệnh đề 1 cho $f$.

#### Định lý 1 (Krein-Milman) {#evt-ii-s7-thm-1 .statement}

— *Trong một không gian lồi địa phương Hausdorff E, mọi tập compact lồi A là bao lồi đóng của tập hợp các điểm cực trị của nó.*

Vì, cho C là bao lồi đóng của tập hợp các điểm cực trị của A; rõ ràng $C \subset A$. Để thấy rằng $A \subset C$, chỉ cần chứng minh rằng, nếu $u$ là một hàm tuyến tính affine, liên tục trong E và nếu $u(x) \geq 0$ trong C thì cũng $u(x) \geq 0$ trong A (II, p. 39, hệ quả 4); nhưng điều này suy ra từ mệnh đề 1 áp dụng cho $-u$.

#### Mệnh đề 2 {#evt-ii-s7-prop-2 .statement}

*Cho x là một điểm cực trị của một tập compact lồi A trong một không gian lồi địa phương Hausdorff* E. Khi đó với mọi lân cận mở V của x trong E, tồn tại một nửa không gian mở F trong E sao cho $x \in F \cap A \subset V \cap A$ (nói cách khác, các vết trên A của các nửa không gian mở chứa x tạo thành một hệ cơ sở các lân cận của x trong A).

Với mọi nửa không gian mở D của E chứa x, tập hợp $A \cap \overline{D}$ là một lân cận compact của x trong A, và giao của tất cả các lân cận này chính xác là điểm x (hai điểm phân biệt bất kỳ có thể được tách nghiêm ngặt bởi một siêu phẳng đóng (II, p. 38, mệnh đề 4). Theo mệnh đề 1 của GT, I, § 9.2, chỉ cần chứng minh rằng các tập hợp $A \cap \overline{D}$ tạo thành một cơ sở lọc. Bây giờ nếu ta viết $L_D = A \cap (E - D)$, tập hợp $L_D$ là lồi, compact và được chứa trong tập lồi $A - \{x\}$; nếu $D_1, D_2$ là hai nửa không gian mở của E chứa x, bao lồi B của $L_{D_1} \cup L_{D_2}$ do đó được chứa trong $A - \{x\}$; nhưng B là một tập compact (II, p. 14, mệnh đề 15), do đó tồn tại một siêu phẳng đóng H tách nghiêm ngặt x khỏi B (II, p. 38, mệnh đề 4) và nếu nửa không gian mở được xác định bởi H và chứa x là D, thì ta có $L_{D_1} \cup L_{D_2} \subset L_D$, do đó $A \cap \overline{D} \subset (A \cap \overline{D_1}) \cap (A \cap \overline{D_2})$.

#### Hệ quả {#evt-ii-s7-n1-cor-2 .statement}

— Trong một không gian lồi địa phương Hausdorff, cho K là một tập con compact của một tập compact lồi A. Khi đó các điều kiện sau là tương đương.

a) A là bao lồi đóng của K.

b) K giao với mọi tập là giao của A với một trong các siêu phẳng đỡ của nó.

c) K chứa tập hợp các điểm cực trị của A.

a) $\Rightarrow$ b). Giả sử tồn tại một siêu phẳng đỡ H của A có phương trình là $f(x) = \alpha$, sao cho $(H \cap A) \cap K = \varnothing$ và giả sử, chẳng hạn, rằng $f(x) \geq \alpha$ trong A. Vì $f(x) - \alpha > 0$ với mọi $x \in K$ theo giả thiết và vì K compact, ta có

$$
\beta = \inf_{x \in K} f(x) > \alpha ,
$$

và K do đó được chứa trong nửa không gian đóng $f(x) \geq \beta$; vì vậy điều tương tự cũng đúng đối với bao lồi đóng A của K và đây là một điều vô lý.

b) $\Rightarrow$ c). Giả sử một điểm cực biên x của A không thuộc K; có một lân cận V của x trong E sao cho $V \cap A \cap K = \varnothing$. Nhưng theo mệnh đề 2, ta có thể giả sử rằng V là một nửa không gian mở được xác định bởi một siêu phẳng H với phương trình $f(z) = \alpha$. Nếu chẳng hạn $f(x) > \alpha$, thì với mọi $y \in K$, ta có $f(y) \leq \alpha$, do đó K không gặp giao của A và siêu phẳng tựa $f(z) = \gamma > \alpha$ song song với H (II, p. 37, mệnh đề 2); điều này là vô lý.

c) $\Rightarrow$ a). Đây là một hệ quả hiển nhiên của định lý Krein-Milman.

#### Nhận xét 1 {#evt-ii-s7-n1-rem-1 .statement}

Ngay cả khi không gian vectơ E có chiều hữu hạn, tập hợp các điểm cực biên của một tập compact lồi không nhất thiết đóng (II, p. 89, bài tập. 11).

#### Nhận xét 2 {#evt-ii-s7-n1-rem-2 .statement}

Nếu K là một tập compact trong một không gian vectơ tôpô lồi địa phương Hausdorff không đầy đủ, và A, bao lồi đóng của K, không compact, thì có thể có những điểm cực biên của A không thuộc K (II, p. 87, bài tập. 2).

#### Nhận xét 3 {#evt-ii-s7-n1-rem-3 .statement}

Trong một không gian Banach E có chiều vô hạn, có thể xảy ra rằng quả cầu đóng tâm 0 và bán kính 1 không có bất kỳ điểm cực biên nào (II, p. 89, bài tập. 14).

#### Nhận xét 4 {#evt-ii-s7-n1-rem-4 .statement}

Nếu A là một tập compact lồi trong một không gian lồi địa phương Hausdorff, có thể xảy ra rằng một điểm cực biên của A không thuộc bất kỳ siêu phẳng tựa nào của A (II, p. 78, bài tập. 11). Chứng minh của định lý 1 (II, p. 56) chỉ ra rằng trong mọi trường hợp A là bao lồi đóng của tập hợp các điểm cực biên của A thuộc một siêu phẳng tựa.

### 2. Các phần tử sinh cực biên của các nón lồi

Cho C là một nón lồi có đỉnh 0 trong một không gian vectơ E; rõ ràng không có điểm nào khác của C ngoài đỉnh có thể là một điểm cực biên; đỉnh là một điểm cực biên của C khi và chỉ khi C là nhọn và thực sự.

#### Định nghĩa 2 {#evt-ii-s7-def-2 .statement}

Cho C là một nón lồi có đỉnh 0 trong một không gian vectơ E. Ta nói rằng một nửa đường thẳng D ⊂ C xuất phát từ 0 là một phần tử sinh cực biên của C, nếu mọi đoạn mở chứa trong C, không chứa 0 và gặp D, đều được chứa trong D.

Điều này tương đương với việc nói rằng với mọi x ∈ D sao cho x ≠ 0, nếu y ≠ 0, y' ≠ 0 là hai điểm của C sao cho x = y + y', thì tất yếu y ∈ D và y' ∈ D.

#### Nhận xét 1 {#evt-ii-s7-n2-rem-1 .statement}

Cho C là một nón lồi nhọn thực sự trong E, và xét trên E cấu trúc cấp mà theo đó C là tập hợp các phần tử ≥ 0 (II, p. 12, mệnh đề 13); để một phần tử của E, chẳng hạn x > 0, thuộc một phần tử sinh cực biên của C, thì cần và đủ là mọi phần tử y ≥ 0, bị chặn trên bởi x, có dạng λx với 0 ≤ λ ≤ 1 : thực vậy, nói rằng y bị chặn trên bởi x có nghĩa là x = y + y' trong đó y' ∈ C, do đó suy ra kết luận.

#### Mệnh đề 3 {#evt-ii-s7-prop-3 .statement}

Trong một không gian vectơ E, cho C là một nón lồi có đỉnh 0, và cho x₀ ≠ 0 là một điểm của C, và D là một nửa đường thẳng được chứa trong C, xuất phát từ 0 và chứa x₀. Cho H là một siêu phẳng chứa x₀ và không đi qua 0. Khi đó D là một phần tử sinh cực biên của C khi và chỉ khi x₀ là một điểm cực biên của H ∩ C.

Điều kiện này rõ ràng là cần thiết. Ngược lại, giả sử nó được thỏa mãn; giả sử rằng có một đường thẳng D' không chứa D, đi qua x₀ và sao cho D' ∩ C chứa một đoạn mở mà x₀ thuộc vào. Gọi y ≠ 0 là vectơ phương của D'; các giả thiết kéo theo rằng điểm (1 + λ)x₀ + μy thuộc C với |λ| và |μ| đủ nhỏ. Nhưng khi đó, trong mặt phẳng P được xác định bởi D và D' và mang tôpô chính tắc, x₀ là một điểm trong của P ∩ C, và do đó đường thẳng P ∩ H chứa một đoạn mở được chứa trong H ∩ C và chứa x₀. Điều này mâu thuẫn với giả thiết.

#### Định nghĩa 3 {#evt-ii-s7-def-3 .statement}

Cho C là một tập lồi trong một không gian vectơ tôpô Hausdorff E. Một tập compact lồi không rỗng A của C được gọi là một chỏm của C nếu phần bù C − A của A trong C là lồi.

Cho C là một nón lồi nhọn có đỉnh 0 trong E và cho A là một chỏm của C. Đặt B = C − A. Với mọi nửa đường thẳng đóng L ⊂ C xuất phát từ 0, các tập L ∩ A và L ∩ B là các tập lồi bù nhau trong L, có hợp là L, và sao cho L ∩ A là compact. Vì L ∩ A không rỗng đối với ít nhất một nửa đường thẳng L, ta thấy rằng 0 ∈ A, do đó L ∩ A là một đoạn đóng có một đầu mút tại 0. Nếu A tồn tại thì C là thực sự.

#### Mệnh đề 4 {#evt-ii-s7-prop-4 .statement}

— Cho C là một nón lồi nhọn có đỉnh 0 trong E, một không gian lồi địa phương Hausdorff.

a) Cho A là một chỏm của C. Cho p là hạn chế trên C của gauge của A (II, p. 20). Tập hợp các x ∈ C sao cho p(x) ≤ 1 là tập hợp A. Hàm p là nửa liên tục dưới và có các tính chất sau :
(i) Với mọi x, y trong C, ta có p(x + y) = p(x) + p(y).
(ii) Với mọi x ∈ C và λ ∈ R_+^*, ta có p(λx) = λp(x).
(iii) Nếu x ∈ C, quan hệ p(x) = 0 tương đương với x = 0.

b) Ngược lại, cho p là một hàm xác định trong C với các giá trị trong [0, +∞], thỏa mãn các điều kiện (i), (ii) của a). Cho A là tập hợp các x ∈ C sao cho p(x) ≤ 1. Khi đó A và C − A là lồi. A là một chỏm khi và chỉ khi A compact và không rỗng.

Mệnh đề b) là hiển nhiên. Các tính chất đã nêu trong a) là các hệ quả của các nhận xét trước mệnh đề 4 và của mệnh đề 22 của II, p. 20 và mệnh đề 23 của II, p. 20, ngoại trừ

$$
p(x + y) \geq p(x) + p(y).
$$

Chỉ cần chứng minh điều cuối cùng này khi x ≠ 0 và y ≠ 0; do đó ta có p(x) > 0, p(y) > 0. Cho μ, λ là hai số > 0 sao cho λ < p(x), μ < p(y), và ký hiệu phần bù của A trong C bởi B. Ta có x ∈ λB, y ∈ μB, do đó x + y ∈ λB + μB; do tính lồi của B, ta có λB + μB ⊂ (λ + μ)B, do đó p(x + y) > λ + μ, điều này kéo theo bất đẳng thức đã nêu ở trên.

#### Hệ quả 1 {#evt-ii-s7-prop-4-cor-1 .statement}

— Cho C là một nón lồi nhọn có đỉnh 0 trong E, một không gian lồi địa phương Hausdorff và cho p là hàm gauge của A, một mũ của C. Khi đó các điểm cực biên của A là điểm 0 và các điểm x trên các phần tử sinh cực biên của C sao cho p(x) = 1.

Hiển nhiên rằng 0 là một điểm cực biên của A. Cho x là một điểm trên L, một phần tử sinh cực biên của C và sao cho p(x) = 1. Cho y, z là hai điểm của A sao cho x = $\frac{1}{2}(y + z)$. Vì L là cực biên, ta có y = λx và z = μx, trong đó λ và μ là các số ≥ 0 sao cho $\frac{1}{2}(\lambda + \mu) = 1$, $\lambda = \lambda p(x) = p(y) \leq 1$ và $\mu = \mu p(x) = p(z) \leq 1$, từ đó $\lambda = \mu = 1$ và do đó y = z = x; vậy x là một điểm cực biên của A. Ngược lại, cho x ≠ 0 là một điểm cực biên của A. Hiển nhiên p(x) = 1. Cho y, y' là hai điểm của C sao cho x = y + y', và ta sẽ chứng minh rằng y, y' tỉ lệ với x. Không mất tính tổng quát, ta có thể giả sử rằng các số $\lambda = p(y)$ và $\lambda' = p(y')$ là hữu hạn và > 0. Khi đó $\lambda^{-1}y \in A, {\lambda'}^{-1}y' \in A, \lambda + \lambda' = 1$ theo mệnh đề 4, (i) và đẳng thức $x = \lambda(\lambda^{-1}y) + \lambda'({\lambda'}^{-1}y')$ kéo theo, theo giả thiết rằng

$$
x = \lambda^{-1}y = {\lambda'}^{-1}y'.
$$

#### Hệ quả 2 {#evt-ii-s7-prop-4-cor-2 .statement}

— Mọi điểm của C thuộc về một mũ của C cũng thuộc về bao lồi đóng của hợp các phần tử sinh cực biên của C.

Điều này suy ra ngay lập tức từ hệ quả 1 và định lý Krein-Milman (II, p. 55, th. 1).

\* Ví dụ. — Cho X là một không gian compact địa phương là σ-compact. Cho C là một nón lồi đóng có đỉnh 0 trong $\mathcal{M}_+(X)$ với tôpô yếu. Ta sẽ chứng minh rằng C là hợp các mũ của nó. Cho $(X_n)$ là một dãy tăng các tập mở, tương đối compact của X mà hợp của chúng là X. Cho μ là một phần tử $\neq 0$ của C. Tồn tại các $\alpha_n > 0$ sao cho $\sum_n \alpha_n \mu(X_n) = 1$.

Với mọi độ đo $v \in C$, đặt $p(v) = \sum_n \alpha_n v(X_n) \in [0, +\infty]$. Hàm p trên C thỏa mãn các điều kiện (i) và (ii) của mệnh đề 4. Nó nửa liên tục dưới đối với tôpô yếu (INT, IV, ấn bản lần thứ 2, § 1, No. 1, mệnh đề 4). Tập A gồm các $\gamma \in C$ sao cho $p(\gamma) \leq 1$ do đó là đóng và không rỗng. Mặt khác, mọi tập compact của X được chứa trong một trong các $X_n$, vì vậy A bị chặn yếu cũng là compact yếu (INT, III, ấn bản lần thứ 2, § 1, No. 9, mệnh đề 15). Do đó tập A là một mũ của C chứa μ. \*

#### Mệnh đề 5 {#evt-ii-s7-prop-5 .statement}

Cho C là một nón lồi thực sự có đỉnh 0 trong E, một không gian yếu Hausdorff; giả sử rằng C là đầy đủ đối với cấu trúc đều cảm sinh bởi cấu trúc của E, và rằng có một hệ cơ bản đếm được các lân cận của 0 trong C. Khi đó C là hợp các mũ của nó và là bao lồi đóng của hợp các phần tử sinh cực biên của nó.

Mệnh đề thứ hai suy ra từ mệnh đề thứ nhất và từ hệ quả 2 ở trên. Sử dụng mệnh đề 11 của II, p. 52 quy mệnh đề về trường hợp khi $E = \mathbf{R}^l$ và $C \subset \mathbf{R}_+^l$. Với mọi $\alpha \in I$, ký hiệu phép chiếu $pr_\alpha$ trong E bởi $f_\alpha$; khi đó $f_\alpha$ là một dạng tuyến tính liên tục. Mặt khác cho $(V_n)_{n \in \mathbf{N}}$ là một hệ cơ bản đếm được các lân cận của 0 trong C. Theo định nghĩa của tôpô của E, với mỗi $n \in \mathbf{N}$, tồn tại một tập con hữu hạn $J_n$ của I và một số $\varepsilon_n > 0$ sao cho $V_n$ chứa tập $W_n$ gồm các $x \in C$ sao cho $f_\alpha(x) \leq \varepsilon_n$ với mọi $\alpha \in J_n$; đặt $J = \bigcup_{n \in \mathbf{N}} J_n$. Cho $y \neq 0$ là một điểm của C, và p là hàm $\sum_{\alpha \in J} \lambda_\alpha (f_\alpha|C)$ trong đó các $\lambda_\alpha > 0$ được chọn sao cho $p(y) = 1$; điều này có thể thực hiện được, vì nếu $f_\alpha(y) = 0$ với mọi $\alpha \in J$, thì $y \in V_n$ với mọi $n$, điều này kéo theo $y = 0$, và điều này trái với giả thiết. Bây giờ ta nhận xét rằng với mọi $\alpha \in I$, hàm $f_\alpha|C$ liên tục tại điểm 0, do đó tồn tại một $n \in \mathbf{N}$ sao cho $f_\alpha$ bị chặn trong một $W_n$, do đó bị chặn trên trong C bởi một tổ hợp tuyến tính của một số hữu hạn các hàm $f_\beta|C$, trong đó $\beta \in J$. Suy ra rằng nếu A là tập các $x \in C$ sao cho $p(x) \leq 1$, thì $f_\alpha$ bị chặn trên A với mọi $\alpha \in I$. Vì p là nửa liên tục dưới trong C, suy ra A là đóng và không rỗng trong C và do đó là compact. Vì hiển nhiên p thỏa mãn các điều kiện (i) và (ii) của mệnh đề 4 của II, p. 58, ta thấy rằng A là một mũ trong C và chứa y.

#### Nhận xét 2 {#evt-ii-s7-n2-rem-2 .statement}

Tồn tại các nón lồi thực sự là đầy đủ yếu và không có phần tử sinh cực biên (II, p. 92, bài tập 31).

### 3. Các nón lồi có đáy compact

#### Mệnh đề 6 {#evt-ii-s7-prop-6 .statement}

Cho E là một không gian lồi địa phương Hausdorff và K là một tập compact lồi trong E không chứa 0. Khi đó nón có đỉnh 0 nhỏ nhất C chứa $K$ là một nón lồi thực sự trong $E$ và là một không gian con địa phương compact và đầy đủ của $E$; hơn nữa, tồn tại một siêu phẳng đóng $H$ trong $E$ không chứa 0 sao cho $H$ cắt mọi nửa đường thẳng xuất phát từ 0 được chứa trong $C$ và sao cho $H \cap C$ là compact. Hơn nữa, nếu $D$ là nửa không gian chứa 0 được xác định bởi $H$, một siêu phẳng đóng có các tính chất này, thì $C \cap D$ là một mũ của $C$ và $C$ là hợp của các $\lambda(C \cap D)$ với $\lambda > 0$.

Theo mệnh đề 4 của II, p. 38, tồn tại một siêu phẳng đóng $H$ tách biệt nghiêm ngặt 0 với $K$. Bây giờ, bao lồi $A$ của hợp của $\{0\}$ và $K$ là compact (II, p. 14, mệnh đề 15) và là hợp của các $\lambda K$ với $0 \leq \lambda \leq 1$. Vì 0 và $K$ nằm nghiêm ngặt ở hai phía đối nhau của $H$, với mọi $x \in K$ tồn tại $\lambda$ sao cho $0 < \lambda < 1$ và $\lambda x \in H$. Vì $C$ là hợp của các $\lambda A$ với $\lambda \geq 1$, ta thấy rằng $H$ gặp mọi nửa đường thẳng bắt nguồn từ 0 được chứa trong $C$ và $H \cap A = H \cap C$ là compact. Hơn nữa, $C$ cũng là hợp của các $\lambda(H \cap C)$ với $\lambda \geq 0$; đặt $C_n$ là hợp của các $\lambda(H \cap C)$ với $0 \leq \lambda \leq n$. Rõ ràng $C_n$ là bao lồi của hợp của $\{0\}$ và $n(H \cap C)$, do đó nó là compact. Ngoài ra, với mọi $x \in E$, tồn tại một lân cận đóng $V$ của $x$ trong $E$ và một số nguyên $n$ sao cho $V \cap C \subset C_n$; thực vậy, nếu $H$ được xác định bởi phương trình $f(z) = \alpha$, trong đó $\alpha > 0$, thì chỉ cần lấy $V$ là nửa không gian đóng được xác định bởi $nH$ và chứa 0, trong đó $n$ đủ lớn sao cho $n\alpha > f(x)$. Điều này cho thấy rằng $C$ là compact địa phương (lấy $x \in C$), và rằng nó đóng trong $E$. Ta cũng có thể xét $K$ như một tập con của không gian đầy đủ $\hat{E}$, do đó $C$ cũng đóng trong $\hat{E}$ và do đó đầy đủ.

Cho một nón $C$ và một siêu phẳng đóng $H$ trong một không gian vectơ tôpô Hausdorff $E$, sao cho $H$ không chứa đỉnh $s$ của $C$ và $C$ là nón nhỏ nhất có đỉnh $s$ chứa $H \cap C$, khi đó ta gọi giao $H \cap C$ là một « đế » của nón $C$. Mệnh đề 6 chỉ ra rằng trong một không gian lồi địa phương Hausdorff $E$, nón nhỏ nhất có đỉnh 0, chứa một tập lồi compact $K$ mà 0 không thuộc vào, là một nón có đế compact, và mọi nón lồi có một đế compact $S$, đều địa phương compact và đầy đủ.

#### Ví dụ 1 {#evt-ii-s7-n3-exa-1 .statement}

Mọi nón lồi đóng thực sự trong $E$, một không gian vectơ có số chiều hữu hạn, đều có một đế compact. Thật vậy, theo II, p. 52, mệnh đề 11 ta chỉ cần xét trường hợp $E = \mathbf{R}^n$ và $C = \mathbf{R}_+^n$. Nếu $(e_i)_{1 \leq i \leq n}$ là cơ sở chính tắc của $\mathbf{R}^n$, rõ ràng rằng tập lồi compact là bao lồi của các $e_i$ ($1 \leq i \leq n$) là một đế compact của $\mathbf{R}_+^n$.

#### Ví dụ 2 {#evt-ii-s7-n3-exa-2 .statement}

Nếu $X$ là một không gian compact, thì nón $\mathcal{M}_+(X)$ của các độ đo dương trên $X$, với tôpô mơ hồ, là một nón có một đế compact (INT, III, 2nd ed., § 1, No. 9, hệ quả 3 của mệnh đề 15). \*

### Bài tập {#evt-ii-s7-exercises}

Xem các [bài tập cho § 7](exercises/s7/).
