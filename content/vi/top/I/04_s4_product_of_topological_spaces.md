---
book: top
book_title: General Topology
chapter: I
chapter_title: Topological Structures
section: 4
section_title: Product of topological spaces
lang: vi
source: top-i-iv
pdf_pages: 0049-0056, 0131-0133
extraction: ocr
subsections:
    - "no": 1
      title: PRODUCT SPACES
      page: 0
      pdf_page: 49
    - "no": 2
      title: SECTION OF AN OPEN SET; SECTION OF A CLOSED SET; PROJECTION OF AN OPEN SET. PARTIAL CONTINUITY
      page: 0
      pdf_page: 52
    - "no": 3
      title: CLOSURE IN A PRODUCT
      page: 0
      pdf_page: 53
    - "no": 4
      title: INVERSE LIMITS OF TOPOLOGICAL SPACES
      page: 0
      pdf_page: 54
statements: 21
exercises: 10
content_sha256: 1e5cf77ba2c7d50d4daff69feaa3e63475086501a77a253162e3aad8db19bc30
translated_from: content/en/top/I/04_s4_product_of_topological_spaces.md
source_content_sha256: 1a13adb7bc7e4153dcc789210ec0e3032ec6e298f64eb440003ae30e35867a10
translation_model: gpt-5.4
translation_run: translate-vi-40a2834b
glossary_version: 34
glossary_terms_sha256: 366ce2f1f04fa09773e31d6ffdef2a3e1036246bd0df3eec893172b4238c81d6
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 4. TÍCH CỦA CÁC KHÔNG GIAN TÔPÔ

### 1. CÁC KHÔNG GIAN TÍCH

#### Định nghĩa 1 {#top-i-s4-def-1 .statement}

*Cho một họ $(X_i)_{i \in I}$ các không gian tôpô, không gian tích của họ này là tập hợp tích $X = \prod_{i \in I} X_i$ được trang bị tôpô là tích của các tôpô của các $X_i$ (\S 2, no. 3, Ví dụ 3). Các không gian $X_i (i \in I)$ được gọi là các nhân tử của X.*

Theo § 2, no. 3, Mệnh đề 4, tôpô tích trên $X$ có một cơ sở là tập hợp $\mathcal{B}$ gồm các giao hữu hạn của các tập hợp có dạng $\overline{\mathrm{pr}}_i^{-1}(U_i)$, trong đó $U_i$ là mở trong $X_i$; các tập hợp này là các tích $\prod_{i \in I} A_i$, trong đó $A_i$ là mở trong $X_i$ với mỗi $i \in I$ và $A_i = X_i$ trừ ra đối với một số hữu hạn chỉ số. Các tập hợp này sẽ được gọi là các tập hợp sơ cấp.

Nếu $\mathcal{B}_i$ là một cơ sở của tôpô của $X_i$ (với mỗi $i \in I$), thì hiển nhiên là các tập hợp sơ cấp $\prod_{i \in I} A_i$ sao cho $A_i \in \mathcal{B}_i$ với mỗi chỉ số $i$ mà $A_i \neq X_i$ tạo thành một cơ sở khác của tôpô tích. Do đó, các tập hợp sơ cấp thuộc kiểu này chứa một điểm đã cho $x \in X$ tạo thành một hệ cơ bản các lân cận của $x$ ($\S 1$, no. 3, Mệnh đề 3).

Nếu $I$ là một tập hợp hữu hạn, phép dựng tôpô tích từ các tôpô của các thừa số $X_i$ là đơn giản hơn: các tập hợp sơ cấp chỉ đơn giản là các tích $\prod_{i \in I} A_i$, trong đó $A_i$ là một tập con mở bất kỳ của $X_i$, với mỗi $i \in I$ (x. Bài tập 9).

#### Ví dụ {#top-i-s4-n1-exa-1 .statement}

\* Tích $\mathbf{R}^n$ của $n$ không gian đồng nhất với đường thẳng thực $\mathbf{R}$ được gọi là không gian số thực $n$ chiều; $\mathbf{R}^2$ cũng được gọi là mặt phẳng thực (x. Chương VI, § 1). Tương tự, xuất phát từ đường thẳng hữu tỉ $\mathbf{Q}$, ta định nghĩa không gian số hữu tỉ $n$ chiều $\mathbf{Q}^n$ (mặt phẳng hữu tỉ khi $n = 2$).

Tôpô của không gian $\mathbf{R}^n$ có một cơ sở là tập hợp mọi tích của $n$ khoảng mở trong $\mathbf{R}$, được gọi là các hộp mở $n$ chiều. Các hộp mở chứa một điểm $x \in \mathbf{R}^n$ lập thành một hệ cơ bản các lân cận của điểm này. Tương tự, các tích của $n$ khoảng đóng trong $\mathbf{R}$ được gọi là các hộp đóng $n$ chiều. Các hộp đóng mà $x$ là điểm trong của chúng cũng lập thành một hệ cơ bản các lân cận của $x$. Có các kết quả tương tự đối với $\mathbf{Q}^n$. \*

#### Mệnh đề 1 {#top-i-s4-prop-1 .statement}

Cho $f = (f_i)$ là một ánh xạ từ một không gian tôpô $Y$ vào một không gian tích $X = \prod_{i \in I} X_i$. Khi đó $f$ liên tục tại một điểm $a \in Y$ nếu và chỉ nếu $f_i$ liên tục tại $a$ với mọi $i \in I$.

Vì $f_i = \mathrm{pr}_i \circ f$, đây chỉ là một trường hợp riêng của Mệnh đề 4 của § 2, no. 3.

#### Hệ quả 1 {#top-i-s4-prop-1-cor-1 .statement}

Cho $(X_i)_{i \in I}, (Y_i)_{i \in I}$ là hai họ không gian tôpô có cùng tập chỉ số. Với mỗi $i \in I$, cho $f_i$ là một ánh xạ từ $X_i$ vào $Y_i$. Để ánh xạ tích $f : (x_i) \to (f_i(x_i))$ từ
$$
\prod_{i \in I} X_i \text{ vào } \prod_{i \in I} Y_i
$$
liên tục tại một điểm $a = (a_i)$ thì điều kiện cần và đủ là $f_i$ liên tục tại $a_i$ với mọi $i \in I$.

f có thể được viết thành $x \to (f_i(\mathrm{pr}_i(x)))$, nên theo Mệnh đề 1 điều kiện là đủ. Ngược lại, với mỗi $x \in I$ đặt $g_x$ là ánh xạ từ $X_x$ vào $\prod_{i \in I} X_i$ sao cho $\mathrm{pr}_x(g_x(x_x)) = x_x$ và $\mathrm{pr}_i(g_x(x_x)) = a_i$ mỗi khi $i \neq x$; khi đó $g_x$ liên tục tại điểm $a_x$, theo Mệnh đề 1. Vì $f_x = \mathrm{pr}_x \circ f \circ g_x$ nên suy ra rằng nếu $f$ liên tục tại $a$, thì $f_x$ liên tục tại $a_x$.

#### Hệ quả 2 {#top-i-s4-prop-1-cor-2 .statement}

*Cho $X, Y$ là hai không gian tôpô. Để một ánh xạ $f : X \to Y$ là liên tục, điều kiện cần và đủ là ánh xạ $g : x \to (x, f(x))$ là một đồng phôi của $X$ lên đồ thị $G$ của $f$ (được xét như một không gian con của không gian tích $X \times Y$).*

Vì $f = \mathrm{pr}_2 \circ g$, điều kiện là đủ. Nó cũng là cần, vì nếu $f$ liên tục, thì $g$ là song ánh và liên tục (Mệnh đề 1) và nghịch đảo của $g$ là hạn chế của $\mathrm{pr}_1$ lên $G$, ánh xạ này là liên tục (xem *Lý thuyết tập hợp*, Chương IV, § 2, no. 4, tiêu chuẩn CST 17).

#### Mệnh đề 2 (Tính kết hợp của các tích tôpô) {#top-i-s4-prop-2 .statement}

*Cho $(X_i)_{i \in I}$ là một họ các không gian tôpô, $(J_x)_{x \in K}$ là một phân hoạch của tập hợp $I$, và với mỗi $x \in K$ đặt $X'_x = \prod_{i \in J_x} X_i$ là tích của các không gian $X_i$ với $i \in J_K$. Khi đó ánh xạ chính tắc của không gian tích*
$$
\prod_{i \in I} X_i \text{ lên không gian tích } \prod_{x \in K} X'_x
$$
*là một đồng phôi.*

Đây là một trường hợp riêng của tính bắc cầu của các tôpô ban đầu ($\S$ 2, no. 3, Mệnh đề 5; xem *Lý thuyết tập hợp*, Chương IV, § 2, no. 4, tiêu chuẩn CST 13).

Nói chung ta *đồng nhất* các không gian tích $\prod_{i \in I} X_i$ và $\prod_{x \in K} X'_x$ bằng ánh xạ chính tắc.

#### Hệ quả {#top-i-s4-n1-cor-1 .statement}

*Cho $\sigma$ là một phép hoán vị của tập hợp $I$. Khi đó ánh xạ $(x_i) \to (x_{\sigma(i)})$ là một đồng phôi của*
$$
\prod_{i \in I} X_i \text{ lên } \prod_{i \in I} X_{\sigma(i)}.
$$

Lấy $K = I$ và $J_i = \{ \sigma(i) \}$ với mỗi $i \in I$ trong Mệnh đề 2.

#### Mệnh đề 3 {#top-i-s4-prop-3 .statement}

*Cho $X$ là một tập hợp, $(Y_i)_{i \in I}$ là một họ các không gian tôpô, và với mỗi $i \in I$ cho $f_i$ là một ánh xạ từ $X$ vào $Y_i$. Gọi $f$ là ánh xạ $x \to (f_i(x))$ từ $X$ vào $Y = \prod_{i \in I} Y_i$, và gọi $\mathcal{T}$ là tôpô thô nhất trên $X$ sao cho các ánh xạ $f_i$ là liên tục. Khi đó $\mathcal{T}$ là ảnh ngược theo $f$ của tôpô cảm sinh trên $f(X)$ bởi tôpô tích trên $Y$.*

Đây là một trường hợp riêng khác của tính bắc cầu của các tôpô ban đầu (\S\ 2, no. 3, Mệnh đề 5; xem thêm Lý thuyết tập hợp, Chương IV, \S\ 2, no. 4, tiêu chuẩn CST 15).

#### Hệ quả {#top-i-s4-n1-cor-2 .statement}

*Với mỗi $i \in I$ gọi $A_i$ là một không gian con của $Y_i$. Khi đó tôpô cảm sinh trên $A = \prod_{i \in I} A_i$ bởi tôpô tích trên $\prod_{i \in I} Y_i$ là tích của các tôpô của các không gian con $A_i$.*

Gọi $j_i$ là đơn ánh chính tắc $A_i \to Y_i$, và áp dụng Mệnh đề 3 cho các ánh xạ $f_i = j_i \circ \mathrm{pr}_i$ (xem thêm Lý thuyết tập hợp, Chương IV, \S\ 2, no. 4, tiêu chuẩn CST 14).

### 2. TIẾT DIỆN CỦA MỘT TẬP HỢP MỞ; TIẾT DIỆN CỦA MỘT TẬP HỢP ĐÓNG; PHÉP CHIẾU CỦA MỘT TẬP HỢP MỞ. TÍNH LIÊN TỤC BỘ PHẬN

#### Mệnh đề 4 {#top-i-s4-prop-4 .statement}

*Cho $X_1, X_2$ là hai không gian tôpô; khi đó với mỗi $a_1 \in X_1$, ánh xạ $x_2 \to (a_1, x_2)$ là một đồng phôi của $X_2$ lên không gian con $\{a_1\} \times X_2$ của $X_1 \times X_2$.*

Đây là một trường hợp riêng của Hệ quả 1 của Mệnh đề 1 của no. 1 áp dụng cho hàm hằng $x_2 \to a_1$.

Ánh xạ $x_2 \to (a_1, x_2)$ là một *tiết diện liên tục* (\S\ 3, no. 5) đối với quan hệ tương đương $\mathrm{pr}_2 z = \mathrm{pr}_2 z'$ trên $X_1 \times X_2$; do đó không gian thương của $X_1 \times X_2$ theo quan hệ tương đương này đồng phôi với $X_2$.

#### Hệ quả {#top-i-s4-n2-cor-1 .statement}

*Tiết diện $A(x_1)$ của một tập hợp mở (tương ứng, đóng) $A$ của tích $X_1 \times X_2$ tại một điểm tùy ý $x_1 \in X_1 (*)$ là mở (tương ứng, đóng) trong $X_2$.*

#### Mệnh đề 5 {#top-i-s4-prop-5 .statement}

*Phép chiếu của một tập hợp mở $U$ của tích $X_1 \times X_2$ lên một trong hai nhân tử là một tập hợp mở.*

Chẳng hạn, ta có $\mathrm{pr}_2 U = \bigcup_{x_1 \in X_1} U(x_1)$, và mệnh đề suy ra từ Hệ quả của Mệnh đề 4 và tiên đề (O_1).

#### Nhận xét 1 {#top-i-s4-n2-rem-1 .statement}

Phép chiếu của một tập con *đóng* của $X_1 \times X_2$ lên một nhân tử *không nhất thiết là đóng*. Chẳng hạn, trong mặt phẳng hữu tỉ $\mathbf{Q}^2$, hyperbol có phương trình là $x_1 x_2 = 1$ là một tập hợp đóng, nhưng cả hai phép chiếu của nó đều bằng phần bù của điểm 0 trong $\mathbf{Q}$, và đây không phải là một tập hợp đóng.

(*) *Tiết diện* $A(x_1)$ của $A$ tại $x_1$ được hiểu là tập hợp tất cả các $x_2 \in X_2$ sao cho $(x_1, x_2) \in A$ (xem Lý thuyết tập hợp R, \S\ 3, no. 7).

#### Mệnh đề 6 {#top-i-s4-prop-6 .statement}

Cho $X_1, X_2, Y$ là ba không gian tôpô, $f$ là một ánh xạ từ không gian tích $X_1 \times X_2$ vào $Y$. Nếu $f$ liên tục tại điểm $(a_1, a_2)$ thì ánh xạ bộ phận $x_2 \to f(a_1, x_2)$ từ $X_2$ vào $Y$ liên tục tại điểm $a_2$.

Thật vậy, ánh xạ này là hợp thành của $f$ và ánh xạ $x_2 \to (a_1, x_2)$; do đó kết quả suy ra từ Mệnh đề 4.

Mệnh đề 6 thường được phát biểu bằng cách nói rằng một hàm liên tục của hai biến là liên tục đối với từng biến một.

#### Nhận xét 2 {#top-i-s4-n2-rem-2 .statement}

Có thể xảy ra trường hợp mọi ánh xạ riêng phần được xác định bởi một ánh xạ $f : X_1 \times X_2 \to Y$ đều liên tục mà $f$ không liên tục trên $X_1 \times X_2$ (xem Chương IX, § 5, Bài tập 23). \* Ví dụ nếu $f$ là ánh xạ từ mặt phẳng thực $\mathbf{R}^2$ vào $\mathbf{R}$ được xác định bởi
$$
f(x, y) = xy/(x^2 + y^2) \quad \text{nếu} \quad (x, y) \neq (0, 0)
$$
và $f(0, 0) = 0$, thì mọi ánh xạ riêng phần đều liên tục; nhưng $f$ không liên tục tại $(0, 0)$, vì $f(x, x) = 1/2$ nếu $x \neq 0$.

Nếu $g$ là một ánh xạ từ $X_1$ vào $Y$, liên tục tại một điểm $a_1$, thì ánh xạ $(x_1, x_2) \to g(x_1)$ từ $X_1 \times X_1 \to Y$ là liên tục tại mọi điểm $(a_1, x_2)$, vì nó là hợp thành của $g$ và phép chiếu lên $X_1$.

Các kết quả của tiểu mục này dễ dàng được mở rộng cho một tích tùy ý $\prod_{i \in I} X_i$ của các không gian tôpô bằng cách nhận thấy rằng tích này đồng phôi với tích $\left( \prod_{i \in J} X_i \right) \times \left( \prod_{i \in K} X_i \right)$ đối với mọi phân hoạch $(J, K)$ của $I$ (no. 1, Mệnh đề 2).

### 3. BAO ĐÓNG TRONG MỘT TÍCH

#### Mệnh đề 7 {#top-i-s4-prop-7 .statement}

Trong một không gian tích $\prod_{i \in I} X_i$, bao đóng của một tích các tập hợp $\prod_{i \in I} A_i$ cũng chính là tích $\prod_{i \in I} \overline{A}_i$ của các bao đóng của chúng.

Giả sử rằng $a = (a_i)$ thuộc bao đóng của $\prod_{i \in I} A_i$; khi đó với mỗi $x \in I$, $a_x = \operatorname{pr}_x a$ thuộc bao đóng của $A_x$ do tính liên tục của $\operatorname{pr}_x$ (\S 2, no. 1, Định lý 1) và vì thế $a \in \prod_{i \in I} \overline{A}_i$. Ngược lại, cho $b = (b_i) \in \prod_{i \in I} \overline{A}_i$, và cho $\prod_{i \in I} V_i$ là một tập hợp sơ cấp bất kỳ chứa $b$; với mỗi $i \in I$, $V_i$ chứa một điểm $x_i \in A_i$; do đó $\prod_{i \in I} V_i$ chứa điểm $(x_i) \in \prod_{i \in I} A_i$ và vì thế $b$ thuộc bao đóng của $\prod_{i \in I} A_i$.

#### Hệ quả {#top-i-s4-n3-cor-1 .statement}

*Một tích* $\prod_{i \in I} A_i$ *của các tập hợp không rỗng là đóng trong không gian tích* $\prod_{i \in I} X_i$ *khi và chỉ khi* $A_i$ *là đóng trong* $X_i$ *với mỗi* $i \in I$.

Nếu $I$ là *hữu hạn*, thì một tích $\prod_{i \in I} A_i$ là mở với điều kiện $A_i$ là mở trong $X_i$ với mỗi $i \in I$; nhưng điều này không còn đúng nữa nếu $I$ là vô hạn.

#### Mệnh đề 8 {#top-i-s4-prop-8 .statement}

*Cho* $a = (a_i)$ *là một điểm bất kỳ của một không gian tích* $X = \prod_{i \in I} X_i$; *khi đó tập hợp* $D$ *các điểm* $x \in X$ *sao cho* $\mathrm{pr}_i x = a_i$ *trừ ra với một số hữu hạn chỉ số* $i$ *là trù mật trong* $X$.

Với mỗi $x \in X$ và mỗi tập sơ cấp $V = \prod_{i \in I} U_i$ chứa $x$, ta có $U_i = X_i$ trừ ra đối với các chỉ số $i$ thuộc một tập con hữu hạn $J$ của $I$; nếu ta lấy $y_i = x_i$ với $i \in J$ và $y_i = a_i$ với $i \notin J$, thì hiển nhiên là
$$
y = (y_i) \in D \quad \text{và} \quad y \in V;
$$
do đó có kết quả.

### 4. GIỚI HẠN NGHỊCH ĐẢO CỦA CÁC KHÔNG GIAN TÔPÔ

Cho $I$ là một tập hợp được sắp thứ tự bộ phận (nhưng không nhất thiết có hướng) (*), trong đó quan hệ thứ tự được viết là $\alpha \leq \beta$. Với mỗi $\alpha \in I$, cho $X_\alpha$ là một không gian tôpô, và với mỗi cặp $(\alpha, \beta)$ sao cho $\alpha \leq \beta$ cho $f_{\alpha \beta}$ là một ánh xạ từ $X_\beta$ vào $X_\alpha$. Ta nói rằng $(X_\alpha, f_{\alpha \beta})$ là một *hệ ngược các không gian tôpô* nếu: 1) $(X_\alpha, f_{\alpha \beta})$ là một *hệ ngược các tập hợp*; 2) $f_{\alpha \beta}$ là một ánh xạ *liên tục* mỗi khi $\alpha \leq \beta$. Ký hiệu $X$ là tập hợp $\varprojlim X_\alpha$, và với mỗi $\alpha \in I$ cho $f_\alpha$ là ánh xạ chính tắc $X \to X_\alpha$; khi đó tôpô *thô nhất* trên $X$ mà đối với nó các $f_\alpha$ đều liên tục được gọi là *giới hạn ngược* (đối với các $f_{\alpha \beta}$) của các tôpô của $X_\alpha$, và tập hợp $X$ với tôpô này được gọi là *giới hạn ngược của hệ ngược các không gian tôpô* $(X_\alpha, f_{\alpha \beta})$. Mỗi khi ta nói đến $\varprojlim X_\alpha$ như một không gian tôpô, luôn luôn phải hiểu rằng tôpô của không gian này là giới hạn ngược của các tôpô của $X_\alpha$, trừ khi điều ngược lại được nói rõ ràng.

Tập hợp $X$ là tập con của tích $\prod_{\alpha \in I} X_\alpha$ gồm những điểm $x$ sao cho
$$(1)$$
$$
\mathrm{pr}_\alpha(x) = f_{\alpha \beta}(\mathrm{pr}_\beta(x))
$$
mỗi khi $\alpha \leq \beta$. Theo Mệnh đề 3 của no. 1 suy ra rằng giới hạn ngược của các tôpô của các $X_\alpha$ cũng chính là tôpô *cảm sinh* trên $X$ bởi tôpô của không gian tích $\prod_{\alpha \in I} X_\alpha$. Nếu, với mỗi $\alpha \in I$, $Y_\alpha$ là

(*) Nghĩa là, một tập hợp được trang bị một quan hệ phản xạ và bắc cầu (*Lý thuyết tập hợp* R, § 6, no. 1).

Cho $(X'_\alpha, f'_{\alpha\beta})$ là một hệ ngược khác của các không gian tôpô được đánh chỉ số bởi cùng tập hợp $I$, và với mỗi $\alpha \in I$ cho $u_\alpha : X_\alpha \to X'_\alpha$ là một ánh xạ *liên tục* sao cho $(u_\alpha)$ là một *hệ ngược các ánh xạ*; khi đó $u = \varprojlim u_\alpha$ là một ánh xạ liên tục từ $X = \varprojlim X_\alpha$ vào $X' = \varprojlim X'_\alpha$. Thật vậy, nếu $f'_\alpha$ là ánh xạ chính tắc $X' \to X'_\alpha$, ta có $f'_\alpha \circ u = u_\alpha \circ f_\alpha$, do đó $f'_\alpha \circ u$ là liên tục với mọi $\alpha \in I$, và mệnh đề suy ra từ Mệnh đề 4 của § 2, no. 3.

Cuối cùng, giả sử $I$ là một tập hợp *có hướng*, và cho $J$ là một tập con *đồng tận* của $I$; gọi $Z$ là giới hạn ngược của hệ ngược các không gian tôpô $(X_\alpha, f_{\alpha\beta})_{\alpha \in J, \beta \in J}$. Khi đó song ánh chính tắc $g : X \to Z$ (*Lý thuyết tập hợp*, Chương III, § 7, no. 2, mệnh đề 3) là một *đồng phôi*. Thật vậy, ta có $\mathrm{pr}_\lambda(g(x)) = \mathrm{pr}_\lambda(x)$ với mọi $\lambda \in J$; do đó $g$ liên tục (no. 1, Mệnh đề 1); và nếu $h$ là ánh xạ nghịch đảo của $g$, thì với mọi $\alpha \in I$ tồn tại $\lambda \in J$ sao cho $\alpha \leq \lambda$, và vì thế $\mathrm{pr}_\alpha(h(z)) = f_{\alpha\lambda}(\mathrm{pr}_\lambda(z))$, điều này cho thấy $h$ liên tục (no. 1, Mệnh đề 1), vì các $f_{\alpha\lambda}$ là liên tục.

#### Mệnh đề 9 {#top-i-s4-prop-9 .statement}

*Cho $I$ là một tập có hướng và $J$ là một tập con đồng cuối của $I$. Cho $(X_\alpha, f_{\alpha\beta})$ là một hệ ngược các không gian tôpô được đánh chỉ số bởi $I$; đặt $X = \varprojlim X_\alpha$ và gọi $f_\alpha : X \to X_\alpha$ là ánh xạ chính tắc. Khi đó họ các tập hợp $f^{-1}_\alpha(U_\alpha)$, trong đó $\alpha$ chạy qua $J$ và $U_\alpha$ chạy qua một cơ sở $\mathcal{B}_\alpha$ của tôpô của $X_\alpha$ với mỗi $\alpha \in J$, là một cơ sở của tôpô của $X$.*

Từ § 2, no. 3 ta biết rằng các *giao hữu hạn* của các tập hợp dạng $f^{-1}_\alpha(U_\alpha)$ ($\alpha \in I, U_\alpha$ mở trong $X_\alpha$) tạo thành một cơ sở của tôpô của $X$. Nếu $(\alpha_i)_{1 \leq i \leq n}$ là một họ hữu hạn các chỉ số của $I$, thì tồn tại $\gamma \in J$ sao cho $\alpha_i \leq \gamma$ với $1 \leq i \leq n$; do đó $f_{\alpha_i} = f_{\alpha_i\gamma} \circ f_\gamma$; nếu đặt

$$
V_\gamma = \bigcap_i f^{-1}_{\alpha_i\gamma}(U_{\alpha_i}),
$$

thì ta có

$$
f^{-1}_\gamma(V_\gamma) = \bigcap_i f^{-1}_{\alpha_i}(U_{\alpha_i});
$$

nhưng $V_\gamma$ là mở và vì vậy là một hợp của các tập hợp thuộc $\mathcal{B}_\gamma$. Suy ra kết quả.

#### Hệ quả {#top-i-s4-n4-cor-1 .statement}

*Cho $A$ là một tập con của $X$ và gọi $A_\alpha$ là $f_\alpha(A)$ với mỗi $\alpha \in I$. Khi đó:*

(i) *Các $A_\alpha$ (tương ứng, các $\overline{A}_\alpha$) tạo thành một hệ ngược các tập con của các $X_\alpha$, và*

$$
\overline{A} = \bigcap_\alpha f^{-1}_\alpha(\overline{A}_\alpha) = \varprojlim \overline{A}_\alpha.
$$

(ii) *Nếu $A$ đóng trong $X$, thì $A = \varprojlim A_\alpha = \varprojlim \overline{A}_\alpha$.*

Mệnh đề thứ nhất của (i) suy ra từ các hệ thức $f_\alpha = f_{\alpha\beta} \circ f_\beta$ với $\alpha \leq \beta$ và từ tính liên tục của các $f_{\alpha\beta}$ (\S 2, no. 1, Định lý 1). Ký hiệu $A'$ là
$$
\bigcap_\alpha \overline{f}_\alpha(\overline{A}_\alpha);
$$
khi đó hiển nhiên $A'$ là đóng và chứa $A$, nên $\overline{A} \subset A'$. Ngược lại, giả sử $x \in A'$; ta phải chứng minh rằng $x$ thuộc bao đóng của $A$. Theo Mệnh đề 9, chỉ cần chứng minh rằng mọi lân cận của $x$ có dạng $\overline{f}_\alpha(U_\alpha)$, với $\alpha \in I$ và $U_\alpha$ mở trong $X_\alpha$, đều giao với $A$. Thật vậy, theo giả thiết, $f_\alpha(x) \in U_\alpha$, và vì $f_\alpha(x) \in \overline{A}$ nên ta có $U_\alpha \cap A_\alpha \neq \varnothing$, điều đó có nghĩa là $A \cap \overline{f}_\alpha(U_\alpha)$ không rỗng.

Để thiết lập (ii), chỉ cần nhận xét rằng, không có bất kỳ hạn chế nào trên $A$, ta có $A \subset \lim A_\alpha \subset \lim \overline{A}_\alpha$; bây giờ nếu $A$ là đóng, thì theo (i)
$$
A = \lim \overline{A}_\alpha
$$
và (ii) suy ra.

#### Ví dụ {#top-i-s4-n4-exa-1 .statement}

Cho $I$ là một tập có hướng và $(X_\alpha)_{\alpha \in I}$ là một họ các tập con của một tập hợp $Y$, sao cho $X_\alpha \supset X_\beta$ mỗi khi $\alpha \leq \beta$. Với mỗi $\alpha \in I$ cho $\mathcal{T}_\alpha$ là một tôpô trên $X_\alpha$ sao cho $\mathcal{T}_\beta$ mịn hơn tôpô cảm sinh trên $X_\beta$ bởi $\mathcal{T}_\alpha$ mỗi khi $\alpha \leq \beta$. Nếu lấy $f_{\alpha\beta}$ là đơn ánh chính tắc $X_\beta \to X_\alpha$ đối với $\alpha \leq \beta$, thì $\lim X_\alpha$ có thể được đồng nhất một cách chính tắc với *giao* $X$ của các $X_\alpha$, được trang bị tôpô là *cận trên bé nhất* (\S 2, no. 3, Ví dụ 2) của các tôpô cảm sinh trên $X$ bởi các $\mathcal{T}_\alpha$.

### Bài tập {#top-i-s4-exercises}

Xem [các bài tập của § 4](exercises/s4/).
