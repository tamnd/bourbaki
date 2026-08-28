---
book: top
book_title: General Topology
chapter: I
chapter_title: Topological Structures
section: 10
section_title: Proper mappings
lang: vi
source: top-i-iv
pdf_pages: 0103-0113, 0156-0161
extraction: ocr
subsections:
    - "no": 1
      title: PROPER MAPPINGS
      page: 0
      pdf_page: 103
    - "no": 2
      title: CHARACTERIZATION OF PROPER MAPPINGS BY COMPACTNESS PROPERTIES
      page: 0
      pdf_page: 107
    - "no": 3
      title: PROPER MAPPINGS INTO LOCALLY COMPACT SPACES
      page: 0
      pdf_page: 110
    - "no": 4
      title: QUOTIENT SPACES OF COMPACT SPACES AND LOCALLY COMPACT SPACES
      page: 0
      pdf_page: 111
statements: 30
exercises: 20
content_sha256: d022289888d8f07e9399efd680fa81eef58ccfeecfdfcf09cdd0f6f79b2eabe3
translated_from: content/en/top/I/10_s10_proper_mappings.md
source_content_sha256: 4090cf2d28c3566332e20a1f373d65f57c9a4a96f1defbe488f43340f5366b01
translation_model: gpt-5-6-mini, gpt-5-6
translation_run: translate-vi-ad2f2242
glossary_version: 34
glossary_terms_sha256: 7e9fcbaaaa277b8e2319816361192488f950ee59298e5de4e6ad988037900f5e
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 10. ÁNH XẠ THỰC SỰ

*Trong tiết này ta ký hiệu bằng $\iota_X$ ánh xạ đồng nhất của một tập hợp $X$ lên chính nó.*

### 1. ÁNH XẠ THỰC SỰ

Nếu $f : X \to Y$ và $f' : X' \to Y'$ là hai ánh xạ *liên tục đóng*, thì tích $f \times f' : X \times X' \to Y \times Y'$ không nhất thiết là một ánh xạ đóng, ngay cả khi $f$ có dạng $\iota_X$.

#### Ví dụ {#top-i-s10-n1-exa-1 .statement}

Mọi ánh xạ hằng vào một không gian Hausdorff đều đóng. Nhưng nếu $f$ là ánh xạ hằng $Q \to 0$, thì $f \times \iota_Q$ là ánh xạ $(x, y) \to (0, y)$ của $Q^2$ vào $Q^2$, do đó nó là phép chiếu thứ hai và không đóng (§ 4, no. 2, Nhận xét 1).

#### Định nghĩa 1 {#top-i-s10-def-1 .statement}

*Cho $f$ là một ánh xạ của một không gian tôpô $X$ vào một không gian tôpô $Y$. Ta nói $f$ là thực sự nếu $f$ liên tục và nếu ánh xạ $f \times \iota_Z : X \times Z \to Y \times Z$ là đóng, với mọi không gian tôpô $Z$.*

Ta sẽ đưa ra các đặc trưng khác của các ánh xạ thực sự trong no. 2 và 3.

Nếu trong Định nghĩa 1 ta lấy không gian $Z$ gồm một điểm duy nhất, ta thấy rằng:

#### Mệnh đề 1 {#top-i-s10-prop-1 .statement}

*Mọi ánh xạ thực sự đều đóng.*

#### Mệnh đề 2 {#top-i-s10-prop-2 .statement}

*Cho $f : X \to Y$ là một đơn ánh liên tục. Khi đó ba mệnh đề sau là tương đương:*
a) $f$ là thực sự.
b) $f$ là đóng.
c) $f$ là một đồng phôi của $X$ lên một tập con đóng của $Y$.

Ta vừa thấy rằng a) suy ra b). Vì quan hệ tương đương $f(x) = f(x')$ là quan hệ đẳng thức, không gian thương của $X$ đối với quan hệ này có thể được đồng nhất với $X$; do đó b) suy ra c) theo § 5, no. 2, Mệnh đề 3. Cuối cùng, nếu c) được thỏa mãn thì $f \times \iota_Z$ là một đồng phôi của $X \times Z$ lên một không gian con đóng của $Y \times Z$ và do đó là một ánh xạ đóng; vì vậy c) suy ra a).

#### Mệnh đề 3 {#top-i-s10-prop-3 .statement}

*Cho $f : X \to Y$ là một ánh xạ liên tục. Nếu $T$ là một tập con bất kỳ của $Y$, gọi $f_T$ là ánh xạ $\overline{f}^{-1}(T) \to T$ trùng với $f$ trên $\overline{f}^{-1}(T)$.*

a) *Nếu $f$ là thực sự thì $f_T$ cũng thực sự.*
b) *Cho $(T(i))_{i \in I}$ là một họ các tập con của $Y$ mà các phần trong của chúng phủ $Y$, hoặc là một phủ đóng hữu hạn địa phương của $Y$; khi đó nếu mỗi ánh xạ $f_{T(i)}$ là thực sự thì $f$ cũng thực sự.*

Cho $Z$ là một không gian tôpô. Nếu $T$ là một tập con bất kỳ của $Y$, ta có
$$
f_T \times \iota_Z = (f \times \iota_Z)_{T \times Z};
$$
nếu $f$ là thực sự, thì $f \times \iota_Z$ là đóng, do đó $(f \times \iota_Z)_{T \times Z}$ cũng vậy [§ 5, no. 1, Mệnh đề 2 a)], do đó a) được chứng minh. Nếu bây giờ $(T(i))_{i \in I}$ thỏa mãn một trong hai điều kiện đã nêu trong b), thì phủ $(T(i) \times Z)_{i \in I}$ của $Y \times Z$ có cùng tính chất đó; nếu $f_{T(i)}$ là thực sự thì các ánh xạ
$$
(f \times \iota_Z)_{T(i) \times Z}
$$
là đóng, do đó $f \times \iota_Z$ là đóng [§ 5, no. 1, Mệnh đề 2 b)]. Điều này hoàn thành chứng minh.

#### Mệnh đề 4 {#top-i-s10-prop-4 .statement}

*Cho $I$ là một tập hợp hữu hạn và với mỗi $i \in I$ cho $f_i : X_i \to Y_i$ là một ánh xạ liên tục. Cho $X = \prod_{i \in I} X_i, \ Y = \prod_{i \in I} Y_i,$ và cho $f : X \to Y$* là ánh xạ tích $(x_i) \to (f_i(x_i))$. Khi đó:
a) *Nếu mỗi $f_i$ là thực sự, thì $f$ là thực sự.*
b) *Nếu $f$ là thực sự và nếu các $X_i$ là không rỗng, thì mỗi $f_i$ là thực sự.*

(Trong no. 2, Định lý 1, Hệ quả 3, ta sẽ thấy rằng mệnh đề này mở rộng đến các tích vô hạn.)

Bằng quy nạp, chỉ cần xét trường hợp $I = \{1, 2\}$.
a) Giả sử rằng $f_1, f_2$ là thực sự, và cho $Z$ là một không gian tôpô; $f_1 \times f_2 \times \iota_Z$ là hợp thành của $\iota_{Y_1} \times f_2 \times \iota_Z$ và
$$
f_1 \times \iota_{X_2} \times \iota_Z;
$$
hai ánh xạ này là đóng theo giả thiết, do đó $f_1 \times f_2 \times \iota_Z$ cũng là đóng [§ 5, no. 1, Mệnh đề 1 a)], do đó $f_1 \times f_2$ là thực sự.

b) Bây giờ giả sử $f$ là thực sự. Cho $F$ là một tập con đóng của $X_2 \times Z$ và cho $G$ là ảnh của $F$ trong $Y_2 \times Z$ theo ánh xạ $f_2 \times \iota_Z$. Khi đó ảnh của $X_1 \times F$ trong $Y_1 \times Y_2 \times Z$ theo $f_1 \times f_2 \times \iota_Z$ là $f_1(X_1) \times G$. Theo giả thiết, tập này là đóng trong $Y_1 \times Y_2 \times Z$; nếu $X_1 \neq \emptyset$, thì $f_1(X_1)$ không rỗng, điều này suy ra rằng $G$ là đóng trong $Y_2 \times Z$ (§ 4, no. 3, Hệ quả của Mệnh đề 7); do đó $f_2$ là thực sự. Tương tự $f_1$ là thực sự nếu $X_2 \neq \emptyset$.

#### Mệnh đề 5 {#top-i-s10-prop-5 .statement}

*Cho $f : X \to X'$ và $g : X' \to X''$ là hai ánh xạ liên tục.*
a) *Nếu $f$ và $g$ là thực sự, thì $g \circ f$ là thực sự.*
b) *Nếu $g \circ f$ là thực sự và $f$ là toàn ánh, thì $g$ là thực sự.*
c) *Nếu $g \circ f$ là thực sự và $g$ là đơn ánh, thì $f$ là thực sự.*
d) *Nếu $g \circ f$ là thực sự và $X'$ là Hausdorff, thì $f$ là thực sự.*

Cho $Z$ là một không gian tôpô. Ta có
$$
(g \circ f) \times \iota_Z = (g \times \iota_Z) \circ (f \times \iota_Z);
$$
nếu $f$ và $g$ là thực sự, thì $f \times \iota_Z$ và $g \times \iota_Z$ là đóng; do đó [§ 5, no. 1, Mệnh đề 1 a)] $(g \circ f) \times \iota_Z$ là đóng; điều này chứng minh a). Chứng minh của b) [tương ứng c)] được tiến hành theo cùng các bước, sử dụng phần b) [tương ứng c)] của Mệnh đề 1 của § 5, no. 1, và nhận xét rằng nếu $f$ là toàn ánh (tương ứng nếu $g$ là đơn ánh) thì $f \times \iota_Z$ là toàn ánh (tương ứng $g \times \iota_Z$ là đơn ánh). Cuối cùng, để chứng minh d), xét biểu đồ giao hoán

$$
\begin{array}{ccc}
X & \overset{\varphi}{\to} & X \times X' \\
f \downarrow & & \downarrow (g \circ f) \times \iota_{X'} \\
X' & \underset{\psi}{\to} & X'' \times X'
\end{array}
$$

trong đó $\varphi(x) = (x, f(x))$ và $\psi(x') = (g(x'), x')$. Ánh xạ $\varphi$ (tương ứng $\psi$) là một đồng phôi của $X$ (tương ứng $X'$) lên đồ thị của $f$ (tương ứng ảnh phản xạ của đồ thị của $g$) (§ 4, no. 1, Mệnh đề 1, Hệ quả 2). Hơn nữa, vì $X'$ là Hausdorff, đồ thị $\varphi(X)$ của $f$ là đóng trong $X \times X'$ (§ 8, no. 1, Mệnh đề 2, Hệ quả 2). Do đó (Mệnh đề 2) $\varphi$ là thực sự; mặt khác Mệnh đề 4 chỉ ra rằng $(g \circ f) \times i_{X'}$ là thực sự. Theo a) ở trên và tính giao hoán của biểu đồ (1), $\psi \circ f$ là thực sự; nhưng $\psi$ là đơn ánh và do đó $f$ là thực sự theo c) ở trên.

#### Nhận xét {#top-i-s10-n1-rem-1 .statement}

Nếu $X'$ không là Hausdorff thì có thể xảy ra rằng $g \circ f$ là thực sự còn $f$ thì không; chẳng hạn, lấy $X$ và $X''$ gồm một điểm và $X'$ gồm hai điểm, với tôpô thô nhất.

#### Hệ quả 1 {#top-i-s10-prop-5-cor-1 .statement}

*Nếu $f : X \to Y$ là một ánh xạ thực sự, thì hạn chế của $f$ lên một tập con đóng $F$ của $X$ là một ánh xạ thực sự của $F$ vào $Y$.*

Vì hạn chế này là hợp thành $f \circ j$, trong đó $j : F \to X$ là đơn ánh chính tắc, và là thực sự theo Mệnh đề 2.

#### Hệ quả 2 {#top-i-s10-prop-5-cor-2 .statement}

*Cho $f : X \to Y$ là một ánh xạ thực sự, trong đó $X$ là Hausdorff. Khi đó không gian con $f(X)$ của $Y$ là Hausdorff.*

Theo Mệnh đề 5 c), ta chỉ cần xét trường hợp $f(X) = Y$. Khi đó đường chéo của $Y \times Y$ là ảnh qua $f \times f$ của đường chéo của $X$, vốn đóng (§ 8, no. 1, Mệnh đề 1); $f \times f$ là thực sự (Mệnh đề 4); do đó đường chéo của $Y \times Y$ là đóng (Mệnh đề 1) và vì vậy $Y$ là Hausdorff (§ 8, no. 1, Mệnh đề 1).

#### Hệ quả 3 {#top-i-s10-prop-5-cor-3 .statement}

*Cho $I$ là một tập hợp hữu hạn và với mỗi $i \in I$, cho $f_i : X \to Y_i$ là một ánh xạ thực sự. Nếu $X$ là Hausdorff, thì ánh xạ $x \mapsto (f_i(x))$ của $X$ vào $\prod_{i \in I} Y_i$ là thực sự.*

Ánh xạ này là hợp thành của ánh xạ tích $(x_i) \mapsto (f_i(x_i))$ của $X^I$ vào $\prod_i Y_i$ và ánh xạ đường chéo của $X$ vào $X^I$; vì ánh xạ sau là thực sự (theo Mệnh đề 2 và § 8, no. 1, Mệnh đề 1) nên kết luận suy ra từ Mệnh đề 4 và Mệnh đề 5 a).

#### Hệ quả 4 {#top-i-s10-prop-5-cor-4 .statement}

*Cho $X$ và $Y$ là hai không gian tôpô, $f : X \to Y$ là một ánh xạ liên tục, $R$ là quan hệ tương đương $f(x) = f(y)$ trên $X$, và*
$$
X \xrightarrow{p} X/R \xrightarrow{h} f(X) \xrightarrow{i} Y
$$
*là phân tích chính tắc của $f$.* *Khi đó để $f$ là thực sự thì cần và đủ rằng $p$ là thực sự, $h$ là một phép đồng phôi và $f(X)$ là một tập con đóng của $Y$.*

Các điều kiện là đủ theo Mệnh đề 5 a) và Mệnh đề 2. Ngược lại, nếu $f$ là thực sự, thì $f$ là đóng; do đó $f(X)$ là đóng trong $Y$ và $h$ là một phép đồng phôi ($§ 5$, no. 2, Mệnh đề 3); đồng thời $h \circ p$ là thực sự theo Mệnh đề 5 c); do đó $p = h^{-1} \circ (h \circ p)$ là thực sự theo Mệnh đề 5 a).

### 2. ĐẶC TRƯNG HÓA CÁC ÁNH XẠ THỰC SỰ BẰNG CÁC TÍNH CHẤT COMPACT

Trong tiểu mục này ta sẽ ký hiệu bởi $P$ một không gian gồm một điểm duy nhất, với tôpô duy nhất của nó.

#### Bổ đề 1 {#top-i-s10-lem-1 .statement}

*Cho $X$ là một không gian tôpô sao cho ánh xạ hằng $X \to P$ là thực sự. Khi đó $X$ là quasi-compact.*

(Ta sẽ thấy sau đây một chút (Định lý 1, Hệ quả 1) rằng tính chất này đặc trưng hóa các không gian quasi-compact.)

Chúng ta có thể tự hạn chế vào trường hợp $X$ không rỗng. Cho $\mathcal{F}$ là một lọc trên $X$, và $X' = X \cup \{ \omega \}$ là không gian tôpô liên kết với $\mathcal{F}$ ($§ 6$, no. 5, Ví dụ). Gọi $\Delta$ là tập con của $X \times X'$ gồm tất cả các $(x, x)$ trong đó $x \in X$, và gọi $F = \overline{\Delta}$ là bao đóng của $\Delta$ trong $X \times X'$. Theo giả thiết về $X$, ảnh của $F$ qua phép chiếu $X \times X' \to X'$ là đóng trong $X'$; ảnh này chứa $X$ và do đó chứa $\omega$, là điểm thuộc bao đóng của $X$; nói cách khác, tồn tại một điểm $x \in X$ sao cho $(x, \omega) \in F$. Theo định nghĩa của tôpô của $X \times X'$, điều này có nghĩa là, với mỗi lân cận $V$ của $x$ trong $X$ và mỗi $M \in \mathcal{F}$, ta có $(V \times M) \cap \Delta \neq \emptyset$, tức là $V \cap M \neq \emptyset$, do đó $x$ là một điểm tụ của lọc $\mathcal{F}$, và vì vậy $X$ là quasi-compact.

Q.E.D.

#### Định lý 1 {#top-i-s10-thm-1 .statement}

*Cho $f : X \to Y$ là một ánh xạ liên tục. Bốn mệnh đề sau là tương đương:

a) $f$ là thực sự.
b) $f$ là đóng và $\overline{f}^{-1}(y)$ là quasi-compact với mỗi $y \in Y$.
c) *Nếu $\mathcal{F}$ là một lọc trên $X$ và nếu $y \in Y$ là một điểm tụ của $f(\mathcal{F})$ thì tồn tại một điểm tụ $x$ của $\mathcal{F}$ sao cho $f(x) = y$.*
d) *Nếu $\mathcal{U}$ là một siêu lọc trên $X$ và nếu $y \in Y$ là một điểm giới hạn của cơ sở lọc $f(\mathcal{U})$, thì tồn tại một điểm giới hạn $x$ của $\mathcal{U}$ sao cho $f(x) = y$.*

a) $\Longrightarrow$ b): Nếu $f$ là thực sự thì $f$ là đóng (no. 1, Mệnh đề 1) và với mỗi $y \in Y$ ánh xạ $f_{|y|} : \overline{f}^{-1}(y) \to \{ y \}$ là thực sự [no. 1, Mệnh đề 3a)]. Theo Bổ đề 1, điều này suy ra rằng $\overline{f}^{-1}(y)$ là quasi-compact.

b) $\Longrightarrow$ c): Giả sử $\mathfrak{F}$ và $y$ thỏa mãn các giả thiết của c). Gọi $\mathcal{B}$ là cơ sở lọc trên $X$ được tạo bởi các bao đóng của các tập hợp thuộc $\mathfrak{F}$. Vì $f$ là đóng, ta có $f(\overline{M}) = f(M)$ với mỗi $M \in \mathfrak{F}$ (§ 5, no. 4, Mệnh đề 9). Điều này cho thấy các tập hợp $\overline{M} \cap \overline{f}^{-1}(y)$ là không rỗng với mọi $M \in \mathfrak{F}$, và do đó tạo thành một cơ sở lọc trên $\overline{f}^{-1}(y)$ mà các phần tử của nó là các tập con đóng của $\overline{f}^{-1}(y)$. Vì $\overline{f}^{-1}(y)$ là quasi-compact, tồn tại một điểm $x \in \overline{f}^{-1}(y)$ thuộc tất cả các tập hợp $M$ khi $M$ chạy qua $\mathfrak{F}$. Do đó $f(x) = y$ và $x$ là một điểm tụ của $\mathfrak{F}$.

c) $\Longrightarrow$ d): Tầm thường.

d) $\Longrightarrow$ a): Trước hết, ta chứng minh rằng nếu d) được thỏa mãn thì $f$ là một ánh xạ đóng. Cho $A$ là một tập con đóng khác rỗng của $X$ và cho $\mathfrak{F}$ là bộ lọc gồm các tập con của $X$ chứa $A$. Khi đó $A$ là tập hợp các điểm tụ của $\mathfrak{F}$. Cho $B$ là tập hợp các điểm tụ của cơ sở lọc $f(\mathfrak{F})$ trên $Y$; $B$ là đóng và rõ ràng chứa $f(A)$; ta sẽ chứng minh rằng $B = f(A)$. Cho $y \in B$ và cho $\mathcal{B}$ là bộ lọc lân cận của $y$ trong $Y$; theo giả thiết, mọi tập hợp của $\mathfrak{W} = \overline{f}^{-1}(\mathcal{B})$ đều gặp mọi tập hợp của $\mathfrak{F}$; do đó $\mathfrak{W}$ là một cơ sở lọc trên $X$ và tồn tại một siêu lọc $U$ trên $X$ mịn hơn cả $\mathfrak{F}$ lẫn bộ lọc có cơ sở là $\mathfrak{W}$ (§ 6, no. 2, Mệnh đề 1, Hệ quả 1 và no. 4, Định lý 1). Siêu lọc có cơ sở là $f(U)$ mịn hơn $\mathcal{B}$ và do đó hội tụ về $y$. Theo d), tồn tại một điểm $x \in X$ sao cho $f(x) = y$ và $U$ hội tụ về $x$; vì $U$ mịn hơn $\mathfrak{F}$, $x$ là một điểm tụ của $\mathfrak{F}$; do đó $x \in A$. Điều này chứng tỏ rằng $B = f(A)$ và do đó $f$ là đóng.

Để hoàn tất chứng minh, ta phải chỉ ra rằng $f \times \iota_Z$ là đóng với mọi không gian tôpô $Z$. Từ những gì đã chứng minh, chỉ cần chỉ ra rằng nếu $f$ thỏa mãn điều kiện d), thì $f \times \iota_Z$ cũng vậy. Đây là một hệ quả của bổ đề tổng quát sau:

#### Bổ đề 2 {#top-i-s10-lem-2 .statement}

*Nếu* $(f_i)_{i \in I}$ *là một họ các ánh xạ liên tục* $f_i : X_i \to Y_i$, *mỗi ánh xạ đều thỏa mãn điều kiện d)* của Định lý 1, *thì ánh xạ tích*
$$
f : (x_i) \to (f_i(x_i))
$$
*cũng thỏa mãn* d).

Cho $U$ là một siêu lọc trên $X = \prod_i X_i$, và cho $y = (y_i)$ là một điểm của $Y = \prod_i Y_i$ sao cho $f(U)$ hội tụ về $y$. Điều này có nghĩa là mỗi cơ sở siêu lọc $\operatorname{pr}_i(f(U)) = f_i(\operatorname{pr}_i(U))$ đều hội tụ về $y_i$ (§ 7, no. 6, Mệnh đề 10, Hệ quả 1). Theo điều kiện d), với mỗi $i \in I$ tồn tại $x_i \in X_i$ sao cho $f_i(x_i) = y_i$ và $\operatorname{pr}_i(U)$ hội tụ về $x_i$; nhưng khi đó $U$ hội tụ về $x = (x_i)$ (_chỗ đã dẫn_) và ta có $f(x) = y$. Điều này hoàn tất chứng minh Bổ đề 2 và do đó cả Định lý 1.

#### Hệ quả 1 {#top-i-s10-lem-2-cor-1 .statement}

_Một không gian tôpô_ $X$ _là gần compact khi và chỉ khi ánh xạ_ $X \to P$ _là thực sự_.

Áp dụng a) $\iff$ b) cho $X \to P$.

#### Hệ quả 2 {#top-i-s10-lem-2-cor-2 .statement}

_Mọi ánh xạ liên tục_ $f$ _của một không gian gần compact_ $X$ _vào một không gian Hausdorff_ $Y$ _đều là thực sự_.

Hợp thành $X \xrightarrow{f} Y \to P$ là thực sự theo Hệ quả 1; do đó $f$ là thực sự theo no. 1, Mệnh đề 5 d). Ngoài ra, ta có thể áp dụng tiêu chuẩn b) của Định lý 1, sử dụng § 9, no. 4, Định lý 2, Hệ quả 2.

#### Hệ quả 3 {#top-i-s10-lem-2-cor-3 .statement}

_Nếu_ $(f_i)$ _là một họ các ánh xạ thực sự, thì ánh xạ tích_ $(x_i) \to (f_i(x_i))$ _là thực sự_.

Theo Định lý 1, đây chính là Bổ đề 2 ở trên.

Nếu áp dụng hệ quả này cho họ các ánh xạ $X_i \to P$ và sử dụng Hệ quả 1, ta được định lý Tychonoff (§ 9, no 5, Định lý 3).

#### Hệ quả 4 {#top-i-s10-lem-2-cor-4 .statement}

_Cho_ $X$ _là một không gian Hausdorff, và cho_ $f_i : X \to Y_i$ _là một họ các ánh xạ thực sự. Khi đó ánh xạ_ $f : x \to (f_i(x))$ _từ_ $X$ _vào_ $\prod_i Y_i$ _là thực sự_.

Chứng minh giống như trong trường hợp một họ hữu hạn (no. 1, Mệnh đề 5, Hệ quả 3), sử dụng Hệ quả 3 ở trên và sự kiện đường chéo của $X^1$ là đóng (§ 8, no. 1, Mệnh đề 1).

#### Hệ quả 5 {#top-i-s10-lem-2-cor-5 .statement}

_Nếu_ $X$ _là một không gian gần compact bất kỳ và_ $Y$ _là một không gian tôpô bất kỳ, thì phép chiếu_ $\mathrm{pr}_2 : X \times Y \to Y$ _là thực sự_.

Vì ta có thể đồng nhất $Y$ với $P \times Y$ và $\mathrm{pr}_2$ với tích của $X \to P$ và $\iota_Y$, cả hai đều là các ánh xạ thực sự.

#### Ví dụ {#top-i-s10-n2-exa-1 .statement}

Cho $X$ là một tập hợp, và cho $f : X \to X'$ là một ánh xạ từ $X$ lên một không gian tôpô $X'$; trang bị cho $X$ tôpô là ảnh ngược qua $f$ của tôpô của $X'$. Khi đó $f$ là _thực sự_, vì $f$ là đóng (§ 5, no. 1, Ví dụ 3) và ảnh ngược của một điểm của $X'$ là một không gian con của $X$ có tôpô là tôpô thô nhất và do đó là gần compact.

#### Nhận xét {#top-i-s10-n2-rem-1 .statement}

Khi $Y$ là _Hausdorff_, điều kiện d) của Định lý 1 tương đương với điều kiện sau:

d') _Nếu_ $\mathcal{U}$ _là một siêu lọc trên_ $X$ _sao cho_ $f(\mathcal{U})$ _là một cơ sở lọc hội tụ, thì_ $\mathcal{U}$ _là hội tụ_.

Vì nếu $\mathcal{U}$ hội tụ đến $x$ và $f(\mathcal{U})$ hội tụ đến $y$, thì tính duy nhất của giới hạn trong $Y$ và tính liên tục của $f$ cho thấy ta phải có $y = f(x)$. Tương tự, vì Y là Hausdorff, điều kiện c) của Định lý 1 tương đương với:

c') *Nếu $\mathfrak{F}$ là một bộ lọc trên X sao cho $f(\mathfrak{F})$ có một điểm tụ, thì $\mathfrak{F}$ có một điểm tụ.*

Vì c) $\Longrightarrow$ c') $\Longrightarrow$ d') $\Longrightarrow$ d) $\Longrightarrow$ c).

Mặt khác, nếu Y không là Hausdorff, thì d') không còn suy ra d); chẳng hạn, lấy X gồm một điểm và Y gồm hai điểm, với tôpô thô nhất.

#### Mệnh đề 6 {#top-i-s10-prop-6 .statement}

*Cho $f : X \to Y$ là một ánh xạ thực sự, và K là một tập con quasi-compact của Y. Khi đó $\overline{f}^{-1}(K)$ là quasi-compact.*

Theo Mệnh đề 3 của no. 1, ánh xạ $f_K : \overline{f}^{-1}(K) \to K$ là thực sự. Vì $K \to P$ là một ánh xạ thực sự (Định lý 1, Hệ quả 1), theo no. 1, Mệnh đề 5 a), suy ra hợp thành $\overline{f}^{-1}(K) \xrightarrow{f_K} K \to P$ là thực sự, do đó $\overline{f}^{-1}(K)$ là quasi-compact theo Định lý 1, Hệ quả 1.

### 3. ÁNH XẠ THỰC SỰ VÀO CÁC KHÔNG GIAN ĐỊA PHƯƠNG COMPACT

#### Mệnh đề 7 {#top-i-s10-prop-7 .statement}

*Cho f là một ánh xạ liên tục từ một không gian Hausdorff X vào một không gian địa phương compact Y. Khi đó f là thực sự khi và chỉ khi ảnh ngược qua f của mọi tập con compact của Y là compact. Hơn nữa, nếu f là thực sự thì X là địa phương compact.*

Nếu f là thực sự và K là một tập con compact của Y, thì $\overline{f}^{-1}(K)$ là compact theo Mệnh đề 6 của no. 2. Ngược lại, nếu điều kiện này được thỏa mãn, cho $(\mathbf{U}_\alpha)$ là một phủ của Y bởi các tập mở tương đối compact. Khi đó các tập $\overline{f}^{-1}(\overline{\mathbf{U}}_\alpha)$ là compact trong X và phần trong của chúng phủ X; vì X là Hausdorff, điều này cho thấy X là địa phương compact. Hơn nữa, mỗi ánh xạ $f_{\overline{\mathbf{U}}_\alpha} : \overline{f}^{-1}(\alpha \overline{\mathbf{U}}) \to \overline{\mathbf{U}}_\alpha$ là thực sự (no. 2, Định lý 1, Hệ quả 2) và do đó f là thực sự theo Mệnh đề 3 b) của no. 1.

#### Hệ quả {#top-i-s10-n3-cor-1 .statement}

*Cho X, X' là hai không gian địa phương compact, và cho Y (t.ư. Y') là không gian compact thu được bằng cách thêm một điểm ở vô cực $\omega$ (t.ư. $\omega'$) vào X (t.ư. X') (§ 9, no. 8). Khi đó một ánh xạ liên tục $f : X \to X'$ là thực sự khi và chỉ khi mở rộng của nó $\overline{f} : Y \to Y'$, sao cho $\overline{f}(\omega) = \omega'$, là liên tục.*

Theo Mệnh đề 7, f là thực sự khi và chỉ khi, với mỗi tập con compact K' của X', $\overline{f}^{-1}(X' - K') = X - \overline{f}^{-1}(K')$ là phần bù của một tập con compact của X; theo định nghĩa các lân cận của $\omega$ (t.ư. $\omega'$) trong Y (t.ư. Y') điều này xảy ra khi và chỉ khi $\overline{f}$ liên tục tại $\omega$.

### 4. KHÔNG GIAN THƯƠNG CỦA CÁC KHÔNG GIAN COMPACT VÀ CÁC KHÔNG GIAN ĐỊA PHƯƠNG COMPACT

#### Mệnh đề 8 {#top-i-s10-prop-8 .statement}

Cho $X$ là một không gian compact, $R$ một quan hệ tương đương trên $X$, $C$ là đồ thị của $R$ trong $X \times X$, $f$ là ánh xạ chính tắc $X \to X/R$. Khi đó các điều kiện sau là tương đương:

a) $C$ là đóng trong $X \times X$.

b) $R$ là đóng.

c) $f$ là thực sự.

d) $X/R$ là Hausdorff.

$R$ đóng khi và chỉ khi $f$ đóng; do đó b) suy ra c) theo Định lý 1b) của no. 2. Việc c) suy ra d) là một trường hợp riêng của no. 1, Mệnh đề 5, Hệ quả 2. d) suy ra a) đối với mọi không gian tôpô $X$ ($\S$ 8, no. 3, Mệnh đề 8). Còn phải chứng minh rằng a) suy ra b). Nếu $F$ là một tập con đóng của $X$ thì bão hòa của nó (đối với $R$) là $\mathrm{pr}_2(C \cap (F \times X))$; theo giả thiết, $C \cap (F \times X)$ là một tập con đóng của không gian compact $X \times X$, và do đó là compact ($\S$ 9, no. 3, Mệnh đề 3); kết quả nay suy ra từ tính liên tục của $\mathrm{pr}_2$ ($\S$ 9, no. 4, Định lý 2, Hệ quả 2).

Cuối cùng, hiển nhiên rằng nếu $X/R$ là Hausdorff thì nó là compact ($\S$ 9, no. 4, Định lý 2).

#### Mệnh đề 9 {#top-i-s10-prop-9 .statement}

Cho $X$ là một không gian địa phương compact, $R$ là một quan hệ tương đương trên $X$, $C$ là đồ thị của $R$ trong $X \times X$, $f$ là ánh xạ chính tắc $X \to X/R$; cho $X'$ là không gian compact thu được bằng cách ghép thêm một điểm ở vô cực $\omega$ vào $X$, và cho $R'$ là quan hệ tương đương trên $X'$ có đồ thị là $C' = C \cup \{(\omega, \omega)\}$. Khi đó các điều kiện sau là tương đương:

a) $f$ là thực sự.

b) Bão hòa của mỗi tập con compact của $X$ đối với $R$ là compact.

c) $R'$ đóng.

d) Hạn chế của $\mathrm{pr}_2$ lên $C$ là thực sự.

e) $R$ đóng và các lớp tương đương đối với $R$ là compact.

Hơn nữa, nếu các điều kiện này được thỏa mãn thì $X/R$ là địa phương compact.

a) $\Longrightarrow$ b): Vì $X/R = f(X)$ và $f$ là thực sự, nên $X/R$ là Hausdorff (no. 1, Mệnh đề 5, Hệ quả 2); do đó ảnh qua $f$ của mọi tập con compact $K$ của $X$ là compact ($\S$ 9, no. 4, Định lý 2, Hệ quả 1).

Bão hòa của $K$ đối với $R$ là $\overline{f}^{-1}(f(K))$ và do đó là compact theo no. 2, Mệnh đề 6.

b) $\Longrightarrow$ c) : Nếu $F'$ đóng trong $X'$ và không chứa $\omega$, thì $F'$ là một tập con compact của $X$; do đó, bao hòa của nó đối với $R'$, cũng chính là bao hòa của nó đối với $R$, là compact và *a fortiori* đóng trong $X'$. Nếu $\omega \in F'$ và $F = F' \cap X = F' - \{ \omega \}$, thì bao hòa của $F'$ đối với $R'$ là hợp của $\{ \omega \}$ và bao hòa $H$ của $F$ đối với $R$; do đó chỉ cần chứng minh rằng $H$ *đóng* trong $X$ (tức là $R$ là một quan hệ *đóng*). Để làm điều này, chỉ cần chứng minh rằng nếu $K$ là một tập con compact bất kỳ của $X$ thì $H \cap K$ là compact ($§ 9$, no. 7, Mệnh đề 11). Theo giả thiết, bao hòa $L$ của $K$ đối với $R$ là compact, và $H \cap L$ là bao hòa của $F \cap L$, cũng compact; *a fortiori* $H \cap K = (H \cap L) \cap K$ là compact.

c) $\Longrightarrow$ d) : Vì $X'$ là chính quy ($§ 9$, no. 2, Hệ quả của Mệnh đề 1), $C'$ *đóng* trong $X' \times X'$ ($§ 8$, no. 6, Mệnh đề 14) và do đó compact. Suy ra $C'$ là compact hóa một điểm của $C$ ($§ 9$, no. 8, Định lý 4). Vì hạn chế trên $C'$ của $pr_2 : X' \times X' \to X'$ liên tục tại $\omega$, kết quả suy ra từ no. 3, Hệ quả của Mệnh đề 7.

d) $\Longrightarrow$ e) : Nếu $F$ là một tập con đóng bất kỳ của $X$, thì $C \cap (F \times X)$ đóng trong $C$, do đó bao hòa của $F$ đối với $R$, bằng $pr_2(C \cap (F \times X))$, là đóng trong $X$ (no. 1, Mệnh đề 1). Ngoài ra, lớp tương đương của $x \in X$ mod $R$ đồng phôi với ảnh ngược của $\{ x \}$ qua hạn chế của $pr_2$ lên $C$ và do đó compact [no. 2, Định lý 1 b)].

e) $\Longrightarrow$ a) : Nếu $R$ đóng, thì theo định nghĩa $f$ đóng, và với mỗi $z \in X/R$, $f^{-1}(z)$ là một lớp tương đương mod $R$ và do đó compact; suy ra $f$ là thực sự theo Định lý 1 b) của no. 2.

Cuối cùng ta phải chứng minh rằng $X/R$ là compact địa phương. $X'/R'$ là compact theo c) và Mệnh đề 8; quan hệ $R$ là quan hệ cảm sinh trên $X$ bởi $R'$; $X$ là mở trong $X'$ và bão hòa đối với $R'$; do đó $X/R$ đẳng cấu tôpô với ảnh $f'(X)$ của $X$ qua ánh xạ chính tắc $f' : X' \to X'/R'$ ($§ 3$, no. 6, Mệnh đề 10, Hệ quả 1). Khi đó $f'(X)$ là mở trong $X'/R'$, và do đó là một không gian con compact địa phương của $X'/R'$.

Q.E.D.

#### Hệ quả {#top-i-s10-n4-cor-1 .statement}

*Một không gian Hausdorff $X$, một không gian tôpô $Y$, và một ánh xạ thực sự $f : X \to Y$. Khi đó $X$ compact (resp. compact địa phương) khi và chỉ khi $f(X)$ compact (resp. compact địa phương), và điều kiện $Y$ compact (resp. compact địa phương) là đủ.*

#### Nhận xét {#top-i-s10-n4-rem-1 .statement}

Nếu X compact địa phương nhưng không compact, thì một quan hệ tương đương đóng R trên X không nhất thiết Hausdorff (Chương IX, § 4, Bài tập 14); và ngay cả khi R Hausdorff, X/R không nhất thiết compact địa phương (Bài tập 17). Tuy nhiên, ta có tiêu chuẩn sau:

#### Mệnh đề 10 {#top-i-s10-prop-10 .statement}

Cho X là một không gian compact địa phương, R là một quan hệ tương đương mở Hausdorff trên X, và cho f : X \to X/R là ánh xạ chính tắc. Khi đó X/R compact địa phương, và nếu K' là một tập con compact bất kỳ của X/R thì tồn tại một tập con compact K của X sao cho f(K) = K'.

Mệnh đề đầu tiên là hệ quả của các sự kiện rằng mỗi x \in X có một lân cận compact V và f(V) là một lân cận compact của f(x) (§ 5, no. 3, Mệnh đề 5 và § 9, no. 4, Định lý 2, Hệ quả 1). Với mỗi y \in K' gọi V(y) là một lân cận compact của một điểm nào đó của f^{-1}(y) trong X, sao cho f(V(y)) là một lân cận compact của y. Có hữu hạn điểm y_i \in K' sao cho các f(V(y_i)) phủ K'. Gọi K_1 là tập compact $\bigcup_i V(y_i)$ trong X; ta có K' \subset f(K_1); do đó K = K_1 \cap f^{-1}(K') là compact (vì nó đóng trong K_1) và f(K) = K'.

### Bài tập {#top-i-s10-exercises}

Xem [các bài tập cho § 10](exercises/s10/).
