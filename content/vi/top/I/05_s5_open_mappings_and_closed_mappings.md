---
book: top
book_title: General Topology
chapter: I
chapter_title: Topological Structures
section: 5
section_title: Open mappings and closed mappings
lang: vi
source: top-i-iv
pdf_pages: 0056-0063, 0133-0134
extraction: ocr
subsections:
    - "no": 1
      title: OPEN MAPPINGS AND CLOSED MAPPINGS
      page: 0
      pdf_page: 56
    - "no": 2
      title: OPEN EQUIVALENCE RELATIONS AND CLOSED EQUIVALENCE RELATIONS
      page: 0
      pdf_page: 58
    - "no": 3
      title: PROPERTIES PECULIAR TO OPEN MAPPINGS
      page: 0
      pdf_page: 60
    - "no": 4
      title: PROPERTIES PECULIAR TO CLOSED MAPPINGS
      page: 0
      pdf_page: 62
statements: 19
exercises: 7
content_sha256: 20a04c3c76a8fb7649c034520a683c784ed58c75bb56494f41b988a65fffbafd
translated_from: content/en/top/I/05_s5_open_mappings_and_closed_mappings.md
source_content_sha256: 11521c20fdafc2a28ae1fe99f2ad238394f02d44313e71c97ba6893b7ec4f268
translation_model: gpt-5.4
translation_run: translate-vi-c488f15b
glossary_version: 34
glossary_terms_sha256: 8c95bbccd81eb87e1098d654e444055d841d4437394990df02bc06b0b33a241e
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 5. ÁNH XẠ MỞ VÀ ÁNH XẠ ĐÓNG

### 1. ÁNH XẠ MỞ VÀ ÁNH XẠ ĐÓNG

#### Định nghĩa 1 {#top-i-s5-def-1 .statement}

*Cho $X, X'$ là hai không gian tôpô. Một ánh xạ $f : X \to X'$ được gọi là mở (tương ứng, đóng) nếu ảnh qua $f$ của mỗi tập mở (tương ứng, đóng) của $X$ là mở (tương ứng, đóng) trong $X'$.*

Đặc biệt, khi đó $f(X)$ là một tập con mở (tương ứng, đóng) của $X'$.

#### Ví dụ 1 {#top-i-s5-n1-exa-1 .statement}

Cho $A$ là một không gian con của một không gian tôpô $X$. Khi đó đơn ánh chính tắc $j : A \to X$ là mở (tương ứng, đóng) nếu và chỉ nếu $A$ là mở (tương ứng, đóng) trong $X$ (\S 3, no. 1).
2) Để một song ánh $f$ từ một không gian tôpô $X$ lên một không gian tôpô $X'$ là một *đồng phôi* thì điều kiện cần và đủ là $f$ *liên tục và mở*, hoặc *liên tục và đóng*.

3) Cho $f$ là một toàn ánh từ một tập hợp $X$ lên một không gian tôpô $X'$; nếu ta trang bị cho $X$ tôpô là ảnh ngược theo $f$ của tôpô của $X'$ (\$ 2, no. 3, Ví dụ 1), thì $f$ là liên tục, mở và đóng.

4) Trong một không gian tích
$$
X = \prod_{i \in I} X_i,
$$
mỗi phép chiếu $\mathrm{pr}_i : X \to X_i$ là một ánh xạ liên tục và mở, nhưng không nhất thiết là đóng (\$ 4, no. 2, Mệnh đề 5).

\* 5) Một hàm chỉnh hình trên một tập con mở $A$ của $C$ là một ánh xạ mở từ $A$ vào $C$. \*
6) Cho $X, X'$ là hai không gian tôpô và $f$ là một song ánh liên tục, nhưng không song liên tục, từ $X$ lên $X'$. Khi đó song ánh ngược $g : X' \to X$ là một ánh xạ mở và đóng từ $X'$ lên $X$, nhưng không liên tục.

#### Mệnh đề 1 {#top-i-s5-prop-1 .statement}

*Cho $X, X', X''$ là ba không gian tôpô, và cho $f : X \to X', \ g : X' \to X''$ là hai ánh xạ. Khi đó:*

a) *Nếu $f$ và $g$ là mở (tương ứng, đóng), thì $g \circ f$ cũng vậy.*

b) *Nếu $g \circ f$ là mở (tương ứng, đóng) và nếu $f$ liên tục và toàn ánh, thì $g$ là mở (tương ứng, đóng).*

c) *Nếu $g \circ f$ là mở (tương ứng, đóng) và nếu $g$ liên tục và đơn ánh, thì $f$ là mở (tương ứng, đóng).*

Từ Định nghĩa 1, a) suy ra ngay lập tức. Để chứng minh b), chỉ cần nhận xét rằng mọi tập con mở (tương ứng đóng) $A'$ của $X'$ đều có thể viết dưới dạng $f(A)$, trong đó $A = f^{-1}(A')$ là mở (tương ứng đóng) trong $X$ (\$ 2, no. 1, Định lý 1); do đó $g(A') = g(f(A))$ là mở (tương ứng đóng) trong $X''$. Sau hết, để chứng minh c), ta nhận xét rằng $f(A) = g^{-1}(g(f(A)))$ với mọi tập con $A$ của $X$; theo giả thiết, nếu $A$ là mở (tương ứng đóng) trong $X$, thì $g(f(A))$ là mở (tương ứng đóng) trong $X''$, do đó $f(A)$ là mở (tương ứng đóng) trong $X'$ theo \$ 2, no. 1, Định lý 1.

#### Mệnh đề 2 {#top-i-s5-prop-2 .statement}

*Cho $X, Y$ là hai không gian tôpô, $f$ là một ánh xạ từ $X$ vào $Y$. Với mỗi tập con $T$ của $Y$, ký hiệu $f_T$ là ánh xạ từ $f^{-1}(T)$ vào $T$ trùng với $f$ trên $f^{-1}(T)$.*

a) *Nếu $f$ là mở (resp. đóng), thì $f_T$ là mở (resp. đóng).*

b) *Cho $(T(i))_{i \in I}$ là một họ các tập con của $Y$ mà các phần trong của chúng phủ $Y$, hoặc là một phủ đóng hữu hạn địa phương của $Y$; nếu mọi $f_{T(i)}$ đều mở (tương ứng, đóng), thì $f$ là mở (tương ứng, đóng).*

a) Nếu $A$ là một tập con mở (tương ứng, đóng) của $f^{-1}(T)$, thì tồn tại một tập con mở (tương ứng, đóng) $B$ của $X$ sao cho $A = B \cap f^{-1}(T)$, và do đó f_T(A) = f(B) \cap T; theo giả thiết, $f(B)$ là mở (tương ứng, đóng), nên $f_T(A)$ là mở (tương ứng, đóng) trong $T$.

b) Cho $B$ là một tập con mở (tương ứng, đóng) của $X$, và ký hiệu $B_i$ là $B \cap f^{-1}(T(i))$; khi đó $f(B) \cap T(i) = f_{T(i)}(B_i)$. Vì $f_{T(i)}(B_i)$ là mở (tương ứng, đóng) trong $T(i)$ theo giả thiết, suy ra $f(B)$ là mở (tương ứng, đóng) trong $Y$, theo Mệnh đề 3 của § 3, no. 1.

#### Hệ quả {#top-i-s5-n1-cor-1 .statement}

*Nếu $(T(i))_{i \in I}$ là một họ các tập con của $Y$ mà các phần trong của chúng phủ $Y$, hoặc là một phủ đóng hữu hạn địa phương của $Y$, nếu $f : X \to Y$ liên tục và nếu mỗi ánh xạ $f_{T(i)}$ là một đồng phôi từ $f^{-1}(T(i))$ lên $T(i)$, thì $f$ là một đồng phôi từ $X$ lên $Y$.*

Thật vậy, $f$ rõ ràng là song ánh, và là ánh xạ mở theo Mệnh đề 2.

### 2. CÁC QUAN HỆ TƯƠNG ĐƯƠNG MỞ VÀ CÁC QUAN HỆ TƯƠNG ĐƯƠNG ĐÓNG

#### Định nghĩa 2 {#top-i-s5-def-2 .statement}

*Một quan hệ tương đương $R$ trên một không gian tôpô $X$ được gọi là mở (tương ứng, đóng) nếu ánh xạ chính tắc của $X$ lên $X/R$ là mở (tương ứng, đóng).*

Nói như vậy cũng tương đương với việc nói rằng *bão hòa* của mỗi tập con mở (tương ứng, đóng) của $X$ đối với $R$ là mở (tương ứng, đóng) trong $X$ (\S 3, no. 4).

#### Ví dụ 1 {#top-i-s5-n2-exa-1 .statement}

Cho $X$ là một không gian tôpô, $\Gamma$ là một *nhóm các phép đồng phôi* của $X$ lên chính nó, và gọi $R$ là quan hệ tương đương

"tồn tại $\sigma \in \Gamma$ sao cho $y = \sigma(x)$"

giữa $x$ và $y$ (do đó $R$ là quan hệ tương đương mà các lớp của nó là các *quỹ đạo* của $\Gamma$ trong $X$. Quan hệ $R$ là *mở*, vì sự bão hòa của một tập con $A$ của $X$ đối với $R$ là mở thì mỗi $\sigma(A)$ cũng mở và do đó hợp của chúng cũng vậy.

\* Trên đường thẳng thực $\mathbf{R}$ quan hệ tương đương $x \equiv y \pmod{1}$ là mở, vì nó được dẫn xuất như trên từ nhóm các phép tịnh tiến

$$
x \to x + n \qquad (n \in \mathbf{Z})
$$

(xem Chương III, § 2, no. 4). \*

#### Ví dụ 2 {#top-i-s5-n2-exa-2 .statement}

Cho $X$ là tổng của một họ $(X_i)$ các không gian con của $X$, và gọi $X/R$ là không gian thu được bằng cách *dán lại* các $X_i$ dọc theo các tập con *mở* $A_{ix}$ nhờ các song ánh $h_{ix}$ (\S 2, no. 5); và giả sử rằng $h_{ix}$ là một *đồng phôi* từ $A_{ix}$ lên $A_{x'}$ với mọi cặp chỉ số $(i, x)$.

Khi đó quan hệ R là mở. Thật vậy, nếu U mở trong X, thì bão hòa của U là hợp của các $h_{x!}(U \cap A_{ix})$; vì $U \cap A_{ix}$ mở trong $A_{ix}$, nên $h_{x!}(U \cap A_{ix})$ mở trong $A_{ix}$ và do đó trong X.

#### Ví dụ 3 {#top-i-s5-n2-exa-3 .statement}

Với ký hiệu của Ví dụ 2, bây giờ giả sử rằng các $A_{ix}$ là đóng và các $h_{x!}$ là các đồng phôi; hơn nữa giả sử rằng với mỗi chỉ số i chỉ có một số hữu hạn chỉ số x sao cho $A_{ix} \neq \varnothing$ (tức là mỗi $X_i$ chỉ được "gắn" với một số hữu hạn $X_x$). Khi đó quan hệ R là đóng. Thật vậy, nếu F là một tập con đóng bất kỳ của X, thì bão hòa của F là hợp của các tập $h_{x!}(F \cap A_{ix}) \subset A_{ix}$; các giả thiết đã nêu suy ra rằng họ này là hữu hạn địa phương, và $h_{x!}(F \cap A_{ix})$ là đóng trong $A_{ix}$ và do đó trong X. Vậy kết quả suy ra từ Mệnh đề 4 của § 1, no. 5.

#### Mệnh đề 3 {#top-i-s5-prop-3 .statement}

Cho X, Y là hai không gian tôpô, cho $f : X \to Y$ là một ánh xạ liên tục, cho R là quan hệ tương đương $f(x) = f(y)$ trên X, và cho $X \xrightarrow{p} X/R \xrightarrow{h} f(X) \xrightarrow{i} Y$ là phân tích chính tắc của f. Khi đó ba mệnh đề sau là tương đương:

a) f là một ánh xạ mở.

b) Ba ánh xạ p, h, i đều mở.

c) Quan hệ tương đương R là mở, h là một đồng phôi, và $f(X)$ là một tập con mở của Y.

Ngoài ra mệnh đề trước đó vẫn đúng nếu thay khắp nơi "mở" bằng "đóng".

Vì đơn ánh i là liên tục, suy ra từ Mệnh đề 1 c) của no. 1 rằng nếu f mở thì $h \circ p$ cũng mở; vì p là toàn ánh và liên tục, Mệnh đề 1 b) cho thấy h mở; trong mọi trường hợp h là một song ánh liên tục; do đó h là một đồng phôi, và vì thế, theo Mệnh đề 1 a) của no. 1, $p = \overline{h}^{-1} \circ (h \circ p)$ là một ánh xạ mở. Hơn nữa [no. 1, Mệnh đề 1 b)] $i \circ h$ là mở; do đó [no. 1, Mệnh đề 1 a)] $i = (i \circ h) \circ \overline{h}^{-1}$ cũng mở. Điều này chứng minh rằng a) suy ra b). Ngược lại, Mệnh đề 1 a) của no. 1 cho thấy b) suy ra a). Cuối cùng, sự tương đương của b) và c) theo ngay lập tức từ các định nghĩa.

Chứng minh trong trường hợp các ánh xạ đóng là tương tự, mutatis mutandis.

#### Mệnh đề 4 {#top-i-s5-prop-4 .statement}

Cho R là một quan hệ tương đương mở (resp. đóng) trên một không gian tôpô X, và f là ánh xạ chính tắc $X \to X/R$. Cho A là một tập con của X và giả sử rằng một trong hai điều kiện sau được thỏa mãn:

a) A mở (resp. đóng) trong X.

b) A là bão hòa đối với R.

Khi đó quan hệ $R_A$ cảm sinh trên A là mở (resp. đóng) và ánh xạ chính tắc của $A/R_A$ lên $f(A)$ là một đồng phôi.

Xét biểu đồ giao hoán (i) của § 3, no. 6, cho phân tích chính tắc của $f \circ j$. Theo điều kiện a), $j$ là mở (tương ứng, đóng) và $f$ cũng vậy theo giả thiết; do đó $f \circ j$ là mở (tương ứng, đóng) [no. 1, Mệnh đề 1 a)], và kết quả suy ra từ Mệnh đề 3. Theo điều kiện b) ta có
$$
A = \overline{f}^{-1}(f(A)),
$$
và $h \circ \varphi$ là ánh xạ từ $A$ vào $f(A)$ trùng với $f$ trên $A$; chiếu theo Mệnh đề 2 a) của no. 1, $h \circ \varphi$ là mở (tương ứng, đóng), và kết quả lại suy ra từ Mệnh đề 3, áp dụng cho $h \circ \varphi$.

### 3. TÍNH CHẤT RIÊNG CỦA CÁC ÁNH XẠ MỞ

#### Mệnh đề 5 {#top-i-s5-prop-5 .statement}

*Cho $X, Y$ là hai không gian tôpô, $f$ là một ánh xạ từ $X$ vào $Y, \mathcal{B}$ là một cơ sở của tôpô trên $X$. Khi đó các mệnh đề sau là tương đương*:

a) *$f$ là một ánh xạ mở*.

b) *Với mỗi $U \in \mathcal{B}$, $f(U)$ là mở trong $Y$*.

c) *Với mỗi $x \in X$ và mỗi lân cận $V$ của $x$ trong $X$, $f(V)$ là một lân cận của $f(x)$ trong $Y$*.

Tính tương đương của a) và b) suy ra ngay lập tức từ các định nghĩa và từ $(O_1)$; tính tương đương của a) và c) là hệ quả của Mệnh đề 1 của § 1, no. 2.

#### Mệnh đề 6 {#top-i-s5-prop-6 .statement}

*Cho $R$ là một quan hệ tương đương trên một không gian tôpô $X$; khi đó ba điều kiện sau là tương đương*:

a) *Quan hệ $R$ là mở*.

b) *Phần trong của mỗi tập con bão hòa đối với $R$ là bão hòa đối với $R$*.

c) *Bao đóng của mỗi tập con bão hòa đối với $R$ là bão hòa đối với $R$*.

Lấy phần bù ($§ 1$, no. 6, công thức (2)) ta thấy rằng b) và c) là tương đương. Ta hãy chỉ ra rằng b) suy ra a): giả sử điều kiện b) được thỏa mãn và gọi $U$ là một tập con mở của $X$, $V$ là bão hòa của nó đối với $R$; khi đó $\dot{V} \supset U$, và vì theo giả thiết $\dot{V}$ là bão hòa, suy ra $\dot{V} = V$, và do đó bão hòa của $U$ là mở. Ngược lại, giả sử điều kiện a) được thỏa mãn, và gọi $A$ là một tập bão hòa; nếu $B$ là bão hòa của $\dot{A}$, thì $\dot{A} \subset B \subset A$, và vì $B$ là mở theo giả thiết nên suy ra $B = \dot{A}$.

#### Mệnh đề 7 {#top-i-s5-prop-7 .statement}

Cho $R$ là một quan hệ tương đương mở trên một không gian tôpô $X$, và gọi $\varphi : X \to X/R$ là ánh xạ chính tắc. Nếu $A$ là một tập con bất kỳ của $X$ bão hòa đối với $R$, thì bao đóng (tương ứng, phần trong) của $\varphi(A)$ trong $X/R$ là $\varphi(\overline{A})$ (tương ứng, $\varphi(\overset{\circ}{A})$).

Mỗi một trong hai mệnh đề khẳng định của mệnh đề đều có thể suy ra từ mệnh đề kia bằng cách lấy phần bù và dùng công thức (2) của § 1, no. 6 cùng với sự kiện là nếu $B$ là một tập con bão hòa của $X$ thì $\varphi(\complement B) = \complement_{\varphi}(B)$. Theo Mệnh đề 6, $\overline{A}$ là bão hòa; do đó $\varphi(\overline{A})$ là đóng trong $X/R$, và vì $A \subset \overline{A}$ nên ta có $\varphi(A) \subset \varphi(\overline{A})$, bởi vậy $\varphi(A) \subset \varphi(\overline{A})$. Nhưng vì $\varphi$ liên tục, nên $\varphi(\overline{A}) \subset \varphi(A)$ (\S 2, no. 1, Định lý 1), và kết quả suy ra.

#### Mệnh đề 8 {#top-i-s5-prop-8 .statement}

Cho $(X_i)_{i \in I}, (Y_i)_{i \in I}$ là hai họ không gian tôpô được đánh chỉ số bởi cùng một tập hợp $I$. Với mỗi $i \in I$ cho $f_i$ là một ánh xạ mở từ $X_i$ vào $Y_i$, và giả sử rằng $f_i$ là toàn ánh với mọi chỉ số trừ ra một số hữu hạn chỉ số. Khi đó ánh xạ tích $f : (x_i) \to (f_i(x_i))$ từ $\prod_{i \in I} X_i$ vào $\prod_{i \in I} Y_i$ là mở.

Theo Mệnh đề 5, ta chỉ cần chứng minh rằng ảnh qua $f$ của mọi tập hợp sơ cấp $\prod_{i \in I} A_i$ trong $\prod_{i \in I} X_i$ là mở trong $\prod_{i \in I} Y_i$. Nhưng ảnh này là $\prod_{i \in I} f_i(A_i)$, và các giả thiết kéo theo rằng $f_i(A_i)$ là mở trong $Y_i$ với mỗi $i \in I$, và rằng $f_i(A_i) = Y_i$ với mọi chỉ số trừ ra một số hữu hạn chỉ số; do đó suy ra kết quả.

#### Hệ quả {#top-i-s5-n3-cor-1 .statement}

Cho $(X_i)_{i \in I}$ là một họ các không gian tôpô, và với mỗi $i \in I$ cho $R_i$ là một quan hệ tương đương trên $X_i$, và cho $f_i$ là ánh xạ chính tắc $X_i \to X_i/R_i$. Cho $R$ là quan hệ tương đương trong $X = \prod_{i \in I} X_i$

"với mọi $i \in I$, $\operatorname{pr}_i(x) = \operatorname{pr}_i(y)$ (mod $R_i$)"

giữa $x$ và $y$, và cho $f$ là ánh xạ tích $(x_i) \to (f_i(x_i))$ của $X$ vào $\prod_{i \in I} (X_i/R_i)$. Nếu mỗi quan hệ $R_i$ là mở, thì quan hệ $R$ là mở, và song ánh liên kết với $f$ là một đồng phôi của $X/R$ lên $\prod_{i \in I} (X_i/R_i)$.

$R$ là quan hệ $f(x) = f(y)$. Vì $f$ là liên tục và mở theo Mệnh đề 8 ở trên và § 4, no. 1, Hệ quả 1 của Mệnh đề 1, kết quả suy ra từ Mệnh đề 3 của no. 2.

Đặc biệt, nếu $R$ (resp. $S$) là một quan hệ tương đương mở trên một không gian tôpô $X$ (resp. $Y$), thì song ánh chính tắc từ

$$
(X \times Y)/(R \times S) \quad \text{lên} \quad (X/R) \times (Y/S)
$$

là một đồng phôi. Nếu không giả thiết R và S là mở, song ánh này là liên tục nhưng không nhất thiết là một đồng phôi, ngay cả khi một trong hai quan hệ R, S là quan hệ đẳng thức (Bài tập 6).

### 4. CÁC TÍNH CHẤT ĐẶC THÙ CỦA ÁNH XẠ ĐÓNG

#### Mệnh đề 9 {#top-i-s5-prop-9 .statement}

Cho X, X' là hai không gian tôpô. Điều kiện cần và đủ để một ánh xạ f : X → X' là liên tục và đóng là f(Ā) = f(A) với mọi tập con A của X.

Điều kiện này là đủ, vì nó hiển nhiên kéo theo rằng f là đóng, và nó cũng kéo theo rằng f là liên tục theo § 2, no. 1, Định lý 1. Ngược lại, nếu f là liên tục và đóng, ta có f(A) ⊂ f(Ā) ⊂ f(A) theo § 2, no. 1, Định lý 1; hơn nữa f(Ā) là đóng trong X' theo giả thiết; do đó f(Ā) = f(A).

#### Mệnh đề 10 {#top-i-s5-prop-10 .statement}

Cho R là một quan hệ tương đương trên một không gian tôpô X. Khi đó R là đóng nếu và chỉ nếu mỗi lớp tương đương M mod R có một hệ cơ bản các lân cận bão hòa đối với R.

Giả sử R là đóng, và cho U là một lân cận mở tùy ý của M; vì F = ĈU là đóng trong X, nên bão hòa S của F đối với R là đóng trong X. Vì M bão hòa đối với R, ta có M ∩ S = ∅, và do đó V = ĈS là một lân cận mở của M, bão hòa đối với R và được chứa trong U.

Để chứng minh đảo lại, cho F là một tập con đóng bất kỳ của X. Gọi T là bão hòa của F đối với R, cho x là một điểm của ĈT, và gọi M là lớp tương đương của x; khi đó M ∩ T = ∅ và a fortiori M ∩ F = ∅, nên U = ĈF là một lân cận của M. Vậy tồn tại một lân cận V ⊂ U của M sao cho V bão hòa đối với R; V không giao với F, nên cũng không giao với T, do đó ĈT là một lân cận của M và vì vậy của x. Điều này chứng tỏ rằng ĈT là mở (§ 1, no. 2, Mệnh đề 1), tức là T là đóng.

#### Nhận xét {#top-i-s5-n4-rem-1 .statement}

Mệnh đề 10 kéo theo điều sau đây: nếu R là đóng và nếu φ ký hiệu ánh xạ chính tắc X → X/R, thì với mỗi x ∈ X và mỗi lân cận U của lớp tương đương của x trong X, φ(U) là một lân cận của φ(x) trong X/R. Cần chú ý kỹ rằng mệnh đề này hoàn toàn không hàm ý rằng với mọi lân cận V của x, φ(V) là một lân cận của φ(x); nói cách khác (no. 3, Mệnh đề 5) một quan hệ tương đương đóng không nhất thiết là mở (Bài tập 2). Ngược lại, một quan hệ tương đương mở không nhất thiết là đóng (no. 1, Ví dụ 4);

vì nếu $U$ là một lân cận trong $X$ của một lớp tương đương $M$, thì với mỗi $x \in M$ và mỗi lân cận $V \subset U$ của $x$, bão hòa của $V$ chắc chắn là một lân cận của $M$ trong $X$, nhưng lân cận này *không nhất thiết được chứa trong* $U$.

Cuối cùng, có những quan hệ tương đương khác với đẳng thức mà vừa mở vừa đóng (Bài tập 3) và những quan hệ tương đương không mở cũng không đóng ($\S 8$, Bài tập 10).

### Bài tập {#top-i-s5-exercises}

Xem [các bài tập của § 5](exercises/s5/).
