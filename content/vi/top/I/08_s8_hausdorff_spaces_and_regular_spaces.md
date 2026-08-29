---
book: top
book_title: General Topology
chapter: I
chapter_title: Topological Structures
section: 8
section_title: Hausdorff spaces and regular spaces
lang: vi
source: top-i-iv
pdf_pages: 0081-0089, 0140-0147
extraction: ocr
subsections:
    - "no": 1
      title: HAUSDORFF SPACES
      page: 0
      pdf_page: 81
    - "no": 2
      title: SUBSPACES AND PRODUCTS OF HAUSDORFF SPACES
      page: 0
      pdf_page: 83
    - "no": 3
      title: HAUSDORFF QUOTIENT SPACES
      page: 0
      pdf_page: 84
    - "no": 4
      title: REGULAR SPACES
      page: 0
      pdf_page: 86
    - "no": 5
      title: EXTENSION BY CONTINUITY; DOUBLE LIMIT
      page: 0
      pdf_page: 87
    - "no": 6
      title: EQUIVALENCE RELATIONS ON A REGULAR SPACE
      page: 0
      pdf_page: 88
statements: 28
exercises: 24
content_sha256: 31e89de76d209caece3ce19f9bba9230689e420ea2de27cd580a919cf9279395
translated_from: content/en/top/I/08_s8_hausdorff_spaces_and_regular_spaces.md
source_content_sha256: f1786c8e71990c5b477a3226adfcfe52fdd3cc7520408bdd42e9767c604fb35d
translation_model: gpt-5.4
translation_run: translate-vi-d9a27e24
glossary_version: 34
glossary_terms_sha256: 508fdead34cc61fe7fe1b3cb497a9bc9dbbfc5742cf6cb6b8f243d672f524331
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 8. KHÔNG GIAN HAUSDORFF VÀ KHÔNG GIAN CHÍNH QUY

### 1. KHÔNG GIAN HAUSDORFF

#### Mệnh đề 1 {#top-i-s8-prop-1 .statement}

Cho $X$ là một không gian tôpô. Khi đó các mệnh đề sau là tương đương:

(H) Hai điểm phân biệt bất kỳ của $X$ có các lân cận rời nhau.
(Hi) Giao của các lân cận đóng của một điểm bất kỳ của $X$ chỉ gồm riêng điểm đó.
(Hii) Đường chéo của không gian tích $X \times X$ là một tập hợp đóng.
(Hiii) Với mọi tập hợp $I$, đường chéo của không gian tích $Y = X^I$ là đóng trong $Y$.
(Hiv) Không có bộ lọc nào trên $X$ có nhiều hơn một điểm giới hạn.
(Hv) Nếu một bộ lọc $\mathfrak{F}$ trên $X$ hội tụ đến $x$, thì $x$ là điểm bám duy nhất của $\mathfrak{F}$.

Ta sẽ chứng minh các hệ kéo theo

$$
\begin{array}{cccccc}
(H) & \Longrightarrow & (Hi) & \Longrightarrow & (Hv) & \Longrightarrow (Hiv) \Longrightarrow (H)
\\
(H) & \Longrightarrow & (Hiii) & \Longrightarrow & (Hii) & \Longrightarrow (H).
\end{array}
$$

và

(H) $\Longrightarrow$ (Hi): Nếu $x \neq y$ thì tồn tại một lân cận mở $U$ của $x$ và một lân cận mở $V$ của $y$ sao cho $U \cap V = \varnothing$; do đó $y \notin \overline{U}$.

(Hi) $\Longrightarrow$ (Hv): Giả sử $y \neq x$; khi đó tồn tại một lân cận đóng $V$ của $x$ sao cho $y \notin V$, và theo giả thiết tồn tại $M \in \mathfrak{F}$ sao cho $M \subset V$; do đó $M \cap C_V = \varnothing$. Nhưng $C_V$ là một lân cận của $y$; vì thế $y$ không phải là một điểm tụ của $\mathfrak{F}$.

(Hv) $\Longrightarrow$ (Hiv): Hiển nhiên, vì mọi điểm giới hạn của một bộ lọc cũng là một điểm tụ.

(Hiv) $\Longrightarrow$ (H): Giả sử $x \neq y$ và mọi lân cận $V$ của $x$ đều gặp mọi lân cận $W$ của $y$. Khi đó các tập hợp $V \cap W$ tạo thành một cơ sở của một bộ lọc mà cả $x$ lẫn $y$ đều là các điểm giới hạn, điều này trái với giả thiết.

(H) $\Longrightarrow$ (Hiii): Cho $(x) = (x_i)$ là một điểm của $X^I$ không thuộc đường chéo $\Delta$. Khi đó tồn tại ít nhất hai chỉ số $\lambda, \mu$ sao cho $x_\lambda \neq x_\mu$. Gọi $V_\lambda$ (resp. $V_\mu$) là một lân cận của $x_\lambda$ (resp. $x_\mu$) trong $X$, sao cho $V_\lambda \cap V_\mu = \varnothing$; khi đó tập hợp $W = V_\lambda \times V_\mu \times \prod_{i \neq \lambda, \mu} X_i$ (trong đó $X_i = X$ nếu $i \neq \lambda, \mu$) là một lân cận của $x$ trong $X^I$ (§ 4, no. 1) không giao với $\Delta$. Do đó $\Delta$ là đóng trong $X^I$.

(Hiii) $\Longrightarrow$ (Hii): Hiển nhiên.

(Hii) $\Longrightarrow$ (H): Nếu $x \neq y$ thì $(x, y) \in X \times X$ không thuộc đường chéo $\Delta$, do đó (§ 4, no. 1) tồn tại một lân cận $V$ của $x$ và một lân cận $W$ của $y$ trong $X$ sao cho $(V \times W) \cap \Delta = \varnothing$, điều đó có nghĩa là
$$
V \cap W = \varnothing.
$$

#### Định nghĩa 1 {#top-i-s8-def-1 .statement}

*Một không gian tôpô thỏa mãn các điều kiện của Mệnh đề 1 được gọi là một không gian Hausdorff hay tách biệt; tôpô của một không gian như vậy được gọi là một tôpô Hausdorff.*

Tiên đề (H) là *tiên đề Hausdorff*.

#### Ví dụ {#top-i-s8-n1-exa-1 .statement}

Mọi không gian rời rạc đều là Hausdorff. Đường thẳng hữu tỉ $Q$ là Hausdorff, vì nếu $x, y$ là hai số hữu tỉ sao cho $x < y$ thì tồn tại một số hữu tỉ $z$ sao cho $x < z < y$, và các lân cận ]$\leftarrow, z[$ của $x$ và ]$z, \rightarrow[$ của $y$ không giao nhau.

Một tập hợp $X$ có ít nhất hai điểm và được trang bị tôpô thô nhất (§ 2, no. 2) không phải là một không gian Hausdorff.

Cho $f : X \to Y$ là một ánh xạ từ một tập hợp $X$ vào một không gian *Hausdorff* $Y$; khi đó suy ra ngay lập tức từ Mệnh đề 1 rằng $f$ có thể có *nhiều nhất một giới hạn* đối với một bộ lọc $\mathfrak{F}$ trên $X$, và nếu $f$ có $y$ là một giới hạn đối với $\mathfrak{F}$, thì $y$ là *điểm tụ duy nhất* của $f$ đối với $\mathfrak{F}$.

#### Mệnh đề 2 {#top-i-s8-prop-2 .statement}

*Cho $f, g$ là hai ánh xạ liên tục từ một không gian tôpô $X$ vào một không gian Hausdorff $Y$; khi đó tập hợp tất cả các $x \in X$ sao cho $f(x) = g(x)$ là đóng trong $X$.*

Vì tập hợp này là ảnh ngược của đường chéo của $Y \times Y$ dưới ánh xạ $x \mapsto (f(x), g(x))$, ánh xạ này liên tục (§ 4, no. 1, Mệnh đề 1). Do đó kết quả suy ra từ (Hii) và § 2, no. 1, Định lý 1.

#### Hệ quả 1 (Nguyên lý mở rộng các đồng nhất thức) {#top-i-s8-prop-2-cor-1 .statement}

*Cho $f, g$ là hai ánh xạ liên tục từ một không gian tôpô $X$ vào một không gian Hausdorff $Y$. Nếu $f(x) = g(x)$ tại mọi điểm của một tập con trù mật của $X$, thì $f = g$.*

Nói cách khác, một ánh xạ liên tục từ $X$ vào $Y$ (Hausdorff) được xác định duy nhất bởi các giá trị của nó tại mọi điểm của một tập con trù mật của $X$.

#### Hệ quả 2 {#top-i-s8-prop-2-cor-2 .statement}

*Nếu $f$ là một ánh xạ liên tục từ một không gian tôpô $X$ vào một không gian Hausdorff $Y$, thì đồ thị của $f$ là đóng trong $X \times Y$.*

Thật vậy, đồ thị này là tập hợp mọi $(x, y) \in X \times Y$ sao cho $f(x) = y$, và hai ánh xạ $(x, y) \to y$ và $(x, y) \to f(x)$ là liên tục.

#### Mệnh đề 3 {#top-i-s8-prop-3 .statement}

*Cho $(x_i)_{1 \leq i \leq n}$ là một họ hữu hạn các điểm phân biệt của một không gian Hausdorff $X$; khi đó mỗi $x_i$ có một lân cận $V_i$ trong $X$ sao cho các $V_i$ ($1 \leq i \leq n$) đôi một rời nhau.*

Chứng minh bằng quy nạp theo $n$: trường hợp $n = 2$ chính là tiên đề (H). Khi đó, giả sử $W_i$ ($1 \leq i \leq n - 1$) là một lân cận của $x_i$ sao cho các $W_i$ đôi một rời nhau. Mặt khác, với $1 \leq i \leq n - 1$ tồn tại một lân cận $T_i$ của $x_i$ và một lân cận $U_i$ của $x_n$ không giao nhau. Nếu ta lấy $V_i$ là $W_i \cap T_i$ với $1 \leq i \leq n - 1$ và
$$
V_n = \bigcap_{i=1}^{n-1} U_i,
$$
thì các điều kiện của mệnh đề được thỏa mãn.

#### Hệ quả {#top-i-s8-n1-cor-1 .statement}

*Mọi không gian Hausdorff hữu hạn đều rời rạc.*

#### Mệnh đề 4 {#top-i-s8-prop-4 .statement}

*Mọi tập con hữu hạn của một không gian Hausdorff đều đóng.*

Vì mọi tập con gồm một điểm đều đóng theo tiên đề (H\textsuperscript{i}).

#### Mệnh đề 5 {#top-i-s8-prop-5 .statement}

*Cho $X$ là một không gian tôpô và giả sử rằng với mỗi cặp điểm phân biệt $x, y$ của $X$ đều có một ánh xạ liên tục $f$ từ $X$ vào một không gian Hausdorff $X'$ sao cho $f(x) \neq f(y)$. Khi đó $X$ là Hausdorff.*

Cho $V'$ và $W'$ lần lượt là các lân cận rời nhau của $f(x)$ và $f(y)$ trong $X'$; khi đó $\overline{f}^{-1}(V')$ và $\overline{f}^{-1}(W')$ là các lân cận rời nhau lần lượt của $x$ và $y$ trong $X$.

#### Hệ quả {#top-i-s8-n1-cor-2 .statement}

*Mọi tôpô mịn hơn một tôpô Hausdorff đều là Hausdorff.*

### 2. KHÔNG GIAN CON VÀ TÍCH CỦA CÁC KHÔNG GIAN HAUSDORFF

*Một không gian con $A$ của một không gian Hausdorff $X$ là Hausdorff*, như ta thấy khi áp dụng Mệnh đề 5 của no. 1 cho đơn ánh chính tắc $A \to X$. Ngược lại, ta có

#### Mệnh đề 6 {#top-i-s8-prop-6 .statement}

*Một không gian tôpô $X$ là Hausdorff nếu mỗi điểm của $X$ có một lân cận đóng là một không gian con Hausdorff của $X$.*

Cho $x \in X$ và cho $V$ là một lân cận đóng của $x$ trong $X$ sao cho không gian con $V$ là Hausdorff. Khi đó các lân cận đóng của $x$ trong $V$ có giao là $\{x\}$ (tiên đề (H\textsuperscript{'})); nhưng chúng cũng là các lân cận đóng của $x$ trong $X$ (§ 3, no. 1) và do đó $X$ thỏa mãn (H\textsuperscript{i}).

Tồn tại các không gian *không Hausdorff* mà trong đó mỗi điểm đều có một lân cận Hausdorff (Bài tập 7).

#### Mệnh đề 7 {#top-i-s8-prop-7 .statement}

*Mọi tích của các không gian Hausdorff đều là Hausdorff. Ngược lại, nếu một tích của các không gian khác rỗng là Hausdorff, thì mỗi nhân tử là một không gian Hausdorff.*

Cho $X = \prod_{i \in I} X_i$ là một tích các không gian tôpô. Khi đó nếu $x, y$ là hai điểm phân biệt của $X$, ta có $\operatorname{pr}_i x \neq \operatorname{pr}_i y$ đối với một chỉ số $i$, và Mệnh đề 5 của no. 1 cho thấy rằng $X$ là Hausdorff nếu các $X_i$ là Hausdorff. Ngược lại, nếu $X$ là Hausdorff và các $X_i$ là không rỗng, thì mỗi $X_i$ đẳng cấu đồng phôi với một không gian con của $X$ (§ 4, no. 2, Mệnh đề 4) và do đó là Hausdorff.

#### Hệ quả 1 {#top-i-s8-prop-7-cor-1 .statement}

*Cho $X$ là một tập hợp, cho $(Y_i)_{i \in I}$ là một họ các không gian tôpô Hausdorff, và với mỗi $i \in I$ cho $f_i$ là một ánh xạ từ $X$ vào $Y_i$. Trang bị cho $X$ tôpô thô nhất $\mathcal{T}$ sao cho các $f_i$ đều liên tục. Khi đó, điều kiện cần và đủ để $X$ là Hausdorff là với mỗi cặp điểm phân biệt $x, y$ của $X$ ta có $f_i(x) \neq f_i(y)$ đối với một chỉ số $i \in I$ nào đó.*

Điều kiện là đủ do Mệnh đề 5 của no. 1. Ngược lại, giả sử $X$ là Hausdorff; đặt $Y = \prod_{i \in I} Y_i$ và $f = (f_i)_{i \in I}$ là ánh xạ $x \to (f_i(x))$. Theo Mệnh đề 7 ở trên, $Y$ là Hausdorff, và theo Mệnh đề 3 của § 4, no. 1, $\mathcal{T}$ là ảnh ngược theo $f$ của tôpô của $Y$. Nếu $f(x) = f(y)$ với hai điểm phân biệt $x, y$ của $X$ thì hiển nhiên mọi tập mở (trong tôpô $\mathcal{T}$) chứa $x$ cũng chứa $y$, trái với giả thiết rằng $X$ là Hausdorff.

#### Hệ quả 2 {#top-i-s8-prop-7-cor-2 .statement}

*Cho $(X_\alpha, f_{\alpha \beta})$ là một hệ ngược các không gian tôpô. Nếu các $X_\alpha$ là Hausdorff, thì $X = \varprojlim X_\alpha$ là Hausdorff và là một không gian con đóng của $\prod_\alpha X_\alpha$.

Mệnh đề thứ nhất suy ra từ sự kiện rằng $X$ là một không gian con của không gian Hausdorff $\prod_\alpha X_\alpha$ (Mệnh đề 7). Để chỉ ra rằng $X$ là đóng trong không gian tích, gọi $F_{\alpha \beta}$ ($\alpha \leq \beta$) là tập con của $\prod_\alpha X_\alpha$ gồm các điểm $x$ sao cho $\operatorname{pr}_\alpha x = f_{\alpha \beta}(\operatorname{pr}_\beta x)$; các $F_{\alpha \beta}$ là đóng trong $\prod_\alpha X_\alpha$ (no. 1, Mệnh đề 2), do đó giao của chúng là $X$ cũng đóng.

Hiển nhiên, mọi *tổng* của các không gian Hausdorff (§ 2, no. 4, Ví dụ 3) đều là một không gian Hausdorff.

### 3. CÁC KHÔNG GIAN THƯƠNG HAUSDORFF

Hãy tìm các điều kiện để một không gian thương $X/R$ là *Hausdorff* (trong trường hợp đó, quan hệ tương đương $R$ được gọi là *Hausdorff*). Trước hết, nếu $X/R$ là Hausdorff, thì các tập con của $X/R$ gồm một điểm duy nhất là *đóng* (no. 1, Mệnh đề 4), và do đó *mỗi lớp tương đương* theo mod $R$ *đều đóng trong* $X$. Nhưng điều kiện cần này không đủ.

Định nghĩa của các tập mở trong $X/R$ dẫn đến điều kiện cần và đủ sau đây: $X/R$ là Hausdorff khi và chỉ khi mọi cặp lớp tương đương phân biệt trong $X$ đều được chứa trong các tập mở bão hòa rời nhau của $X$. Chúng tôi sẽ đưa ra những điều kiện khác dùng được thuận tiện hơn.

#### Mệnh đề 8 {#top-i-s8-prop-8 .statement}

*Điều kiện cần để không gian thương $X/R$ là Hausdorff là đồ thị $C$ của $R$ đóng trong $X \times X$. Nếu quan hệ tương đương $R$ là mở, thì điều kiện này cũng đủ.*

Cho $\varphi : X \to X/R$ là ánh xạ chính tắc; khi đó $C$ là ảnh ngược theo $\varphi \times \varphi : X \times X \to (X/R) \times (X/R)$ của đường chéo $\Delta$ của $(X/R) \times (X/R)$. Phần thứ nhất của mệnh đề do đó suy ra từ tính liên tục của $\varphi \times \varphi$ [Tiên đề (Hii) và Định lý 1 của § 2, no. 1]. Nếu $R$ là mở thì $(X/R) \times (X/R)$ có thể được đồng nhất với không gian thương $(X \times X)/(R \times R)$ ($§ 5$, no. 3, hệ quả của Mệnh đề 8), và khi đó $\Delta$ được đồng nhất với ảnh chính tắc trong $(X \times X)/(R \times R)$ của tập hợp $C$, tập hợp này bão hòa đối với $R \times R$. Vậy $\Delta$ là đóng trong $X \times X$ và do đó $X$ là Hausdorff.

Nếu $R$ không mở, thì có những ví dụ trong đó $C$ là đóng nhưng $R$ không Hausdorff (Bài tập 10 và 28).

Để chứng tỏ rằng $X/R$ là Hausdorff ta cũng có thể áp dụng Mệnh đề 5 của no. 1: $M$ và $N$ là hai lớp tương đương phân biệt của $R$ thì điều kiện đủ là tồn tại một ánh xạ liên tục $f$ từ một tập con mở $A$ của $X$, bão hòa đối với $R$ và chứa $M$ và $N$, vào một không gian Hausdorff $X'$, sao cho 1) $f$ là hằng trên mỗi lớp tương đương mod $R$ được chứa trong $A$, 2) $f$ nhận các giá trị phân biệt trên $M$ và $N$. Thật vậy, vì $A/R_A$ có thể được đồng nhất với một tập con mở của $X/R$ ($§ 3$, no. 6, Mệnh đề 10, Hệ quả 1), ta có thể áp dụng Mệnh đề 5 của no. 1 cho ánh xạ $g : A/R_A \to X'$ được cảm sinh bởi $f$, vì $g$ liên tục ($§ 3$, no. 4, Mệnh đề 6).

Đặc biệt:

#### Mệnh đề 9 {#top-i-s8-prop-9 .statement}

*Nếu $f$ là một ánh xạ liên tục từ một không gian tôpô $X$ vào một không gian Hausdorff $X'$, và nếu $R$ là quan hệ tương đương $f(x) = f(y)$, thì không gian thương $X/R$ là Hausdorff.*

#### Mệnh đề 10 {#top-i-s8-prop-10 .statement}

*Nếu $X$ là một không gian Hausdorff, và nếu $X$ có một tiết diện liên tục $s$ đối với quan hệ tương đương $R$, thì $X/R$ là Hausdorff và $s(X/R)$ đóng trong $X$.*

Theo ($§ 3$, no. 5), $X/R$ đồng phôi với không gian con $s(X/R)$ của $X$, không gian này là Hausdorff. Hơn nữa $s(X/R)$ là tập hợp tất cả các $x \in X$ sao cho $s(\varphi(x)) = x$, trong đó $\varphi : X \to X/R$ là ánh xạ chính tắc; do đó mệnh đề thứ hai suy ra từ no. 1, Mệnh đề 2.

### 4. KHÔNG GIAN CHÍNH QUY

#### Mệnh đề 11 {#top-i-s8-prop-11 .statement}

Các tính chất sau của một không gian tôpô $X$ là tương đương:

(O_{III}) Tập hợp các lân cận đóng của mỗi điểm của $X$ là một hệ cơ bản các lân cận của điểm đó.

(O'_{III}) Với mọi tập con đóng $F$ của $X$ và mọi điểm $x \notin F$ đều tồn tại một lân cận của $x$ và một lân cận của $F$ không giao nhau.

(O_{III}) \Longrightarrow (O'_{III}): Nếu $F$ là đóng và $x \notin F$, thì tồn tại một lân cận đóng $V$ của $x$ được chứa trong lân cận $C_F$ của $x$; $V$ và $C_V$ lần lượt là các lân cận của $x$ và $F$, và không có điểm chung nào.

(O'_{III}) \Longrightarrow (O_{III}): Nếu $W$ là một lân cận mở của $x \in X$, thì tồn tại một lân cận $U$ của $x$ và một lân cận $V$ của $C_W$ rời nhau, và do đó $\overline{U} \subset W$.

#### Định nghĩa 2 {#top-i-s8-def-2 .statement}

Một không gian tôpô được gọi là chính quy nếu nó là Hausdorff và thỏa mãn tiên đề (O_{III}); khi đó tôpô của nó được gọi là chính quy.

Một không gian rời rạc là chính quy. \* Ta sẽ thấy ở § 9 rằng mọi không gian compact địa phương (đặc biệt đường thẳng thực $\mathbf{R}$) đều chính quy. \*

#### Mệnh đề 12 {#top-i-s8-prop-12 .statement}

Mọi không gian con của một không gian chính quy đều chính quy.

Cho $A$ là một không gian con của một không gian chính quy $X$. Vì $X$ là Hausdorff, nên $A$ cũng vậy (no. 2); mặt khác, mọi lân cận của một điểm $x \in A$ đối với $A$ đều có dạng $V \cap A$, trong đó $V$ là một lân cận của $x$ trong $X$. Vì $X$ là chính quy nên tồn tại một lân cận $W$ của $x$ trong $X$ vừa đóng trong $X$ vừa được chứa trong $V$; khi đó $W \cap A$ là một lân cận của $x$ trong $A$, đóng trong $A$ và được chứa trong $V \cap A$. Do đó suy ra kết quả. Ngược lại:

#### Mệnh đề 13 {#top-i-s8-prop-13 .statement}

Nếu mọi điểm $x$ của một không gian tôpô $X$ đều có một lân cận đóng là một không gian con chính quy của $X$, thì $X$ là chính quy.

$X$ là Hausdorff theo Mệnh đề 6 của no. 2. Cho $x$ là một điểm bất kỳ của $X$ và cho $V$ là một lân cận đóng chính quy của $x$. Nếu $U$ là một lân cận bất kỳ của $x$ được chứa trong $V$, thì $U$ là một lân cận của $x$ tương đối đối với $V$; do đó theo giả thiết tồn tại một lân cận $W$ của $x$ trong $V$ vừa đóng trong $V$ vừa được chứa trong $U$. Nhưng $W$ là một lân cận của $x$ trong $X$ vì $V$ là một lân cận của $x$ trong $X$, và $W$ đóng trong $X$ vì $V$ đóng trong $X$.

#### Nhận xét 1 {#top-i-s8-n4-rem-1 .statement}

Có những ví dụ về các không gian không Hausdorff trong đó mọi điểm đều có một lân cận chính quy (Bài tập 7).
2) Có những không gian Hausdorff nhưng không chính quy (Bài tập 20).
3) Một tôpô mịn hơn một tôpô chính quy không nhất thiết là chính quy (Bài tập 20).

### 5. MỞ RỘNG BẰNG TÍNH LIÊN TỤC; GIỚI HẠN KÉP

#### Định lý 1 {#top-i-s8-thm-1 .statement}

Cho X là một không gian tôpô, A là một tập con trù mật của X, f : A → Y là một ánh xạ từ A vào một không gian chính quy Y. Điều kiện cần và đủ để f mở rộng thành một ánh xạ liên tục $\overline{f} : X \to Y$ là, với mỗi $x \in X$, $f(y)$ tiến tới một giới hạn trong Y khi y tiến tới x mà vẫn thuộc A. Khi đó, mở rộng liên tục $\overline{f}$ của f lên X là duy nhất.

Tính duy nhất của $\overline{f}$ suy ra từ nguyên lý mở rộng các đồng nhất thức (no. 1, Mệnh đề 2, Hệ quả 1). Rõ ràng điều kiện ấy là cần thiết, vì nếu $\overline{f}$ liên tục trên X, thì với mỗi $x \in X$ ta có
$$
\overline{f}(x) = \lim_{y \to x, y \in A} \overline{f}(y) = \lim_{y \to x, y \in A} f(y)
$$
(§ 7, no. 5). Ngược lại, giả sử điều kiện ấy được thỏa mãn và định nghĩa
$$
\overline{f}(x) = \lim_{y \to x, y \in A} f(y)
$$
với mỗi $x \in X$; $\overline{f}(x)$ là một phần tử xác định tốt của Y, vì Y là Hausdorff. Ta phải chứng minh rằng $\overline{f}$ liên tục tại mỗi điểm $x \in X$. Khi đó, gọi V' là một lân cận đóng của $\overline{f}(x)$ trong Y; khi ấy theo giả thiết tồn tại một lân cận mở V của x trong X sao cho $f(V \cap A) \subset V'$. Vì V là một lân cận của mỗi điểm của nó, ta có
$$
\overline{f}(z) = \lim_{y \to z, y \in V \cap A} f(y)
$$
với mỗi $z \in V$, và từ đó suy ra $\overline{f}(z) \in \overline{f}(V \cap A) \subset V'$, vì V' đóng. Kết quả bây giờ suy ra từ sự kiện rằng các lân cận đóng của $f(x)$ tạo thành một hệ lân cận cơ bản của $f(x)$ trong Y.

Ánh xạ $\overline{f}$ được gọi là thu được bằng cách mở rộng liên tục f lên X.

Trong mệnh đề của Định lý 1, giả thiết rằng Y là chính quy không thể được làm yếu đi nếu không đặt thêm những điều kiện hạn chế đối với X, A hoặc f (Bài tập 19).

#### Hệ quả {#top-i-s8-n5-cor-1 .statement}

Cho $\mathfrak{F}_1$ là một bộ lọc trên một tập hợp $X_1$, và $\mathfrak{F}_2$ là một bộ lọc trên một tập hợp $X_2$; cho $\mathfrak{F}_1 \times \mathfrak{F}_2$ là bộ lọc tích (§ 6, no. 7) trên $X = X_1 \times X_2$, và cho f là một ánh xạ từ X vào một không gian chính quy Y. Giả sử rằng
a) $\lim_{\mathfrak{F}_1 \times \mathfrak{F}_2} f$ tồn tại.

b) $\lim_{x_2, \mathfrak{F}_2} f(x_1, x_2) = g(x_1)$ tồn tại với mọi $x_1 \in X_1$.

Khi đó $\lim_{x_1, \mathfrak{F}_1} g(x_1)$ tồn tại và bằng $\lim_{\mathfrak{F}_1 \times \mathfrak{F}_2} f$.

Cho $X'_1 = X_1 \cup \{\omega_1\}$ (tương ứng $X'_2 = X_2 \cup \{\omega_2\}$) là không gian tôpô *liên kết với bộ lọc* $\mathfrak{F}_1$ (tương ứng $\mathfrak{F}_2$) (§ 6, no. 5, Ví dụ). Trong không gian tích $X' = X'_1 \times X'_2$ gọi $X''$ là hợp của các không gian con $X_1 \times X'_2$ và $\{(\omega_1, \omega_2)\}$. $X$ rõ ràng là một không gian con trù mật của $X''$, và các giả thiết kéo theo rằng $f(y_1, y_2)$ tiến tới một giới hạn khi $(y_1, y_2)$ tiến tới bất kỳ điểm nào $(x_1, x_2)$ của $X''$ trong khi vẫn nằm trong $X$. Khi đó sự tồn tại của mở rộng của $f$ bằng tính liên tục lên $X''$ suy ra từ Định lý 1. Vì $(\omega_1, \omega_2)$ cũng nằm trong bao đóng của $X_1 \times \{\omega_2\}$ tương đối đối với $X''$, kết quả suy ra ngay lập tức (§ 7, no. 5).

### 6. QUAN HỆ TƯƠNG ĐƯƠNG TRÊN MỘT KHÔNG GIAN CHÍNH QUY

#### Mệnh đề 14 {#top-i-s8-prop-14 .statement}

*Cho* $X$ *là một không gian chính quy*, $R$ *là một quan hệ tương đương đóng trên* $X$. *Khi đó đồ thị* $C$ *của* $R$ *trong* $X \times X$ *là đóng*.

Cho $(a, b)$ là một điểm của $X \times X$ thuộc phần đóng của $C$, và cho $V$ (tương ứng, $W$) là một lân cận *đóng* của $a$ (tương ứng, một lân cận của $b$) trong $X$; khi đó tồn tại một điểm $(x, y) \in C \cap (V \times W)$. Vì $x \in V$, nên $y$ thuộc bão hòa $S$ của $V$ đối với $R$; do đó mỗi lân cận $W$ của $b$ đều giao với $S$. Theo giả thiết, $S$ là *đóng*, và vì vậy $b \in S$. Bây giờ cho $B$ là bão hòa của $\{b\}$ đối với $R$, khi đó mỗi lân cận đóng $V$ của $a$ đều giao với $B$; vì theo giả thiết $B$ là *đóng* và $X$ là *chính quy*, suy ra $a \in B$ và do đó $(a, b) \in C$. Điều này kết thúc chứng minh.

#### Hệ quả {#top-i-s8-n6-cor-1 .statement}

*Trên một không gian chính quy, mọi quan hệ tương đương vừa mở vừa đóng đều là Hausdorff*.

Điều này suy ra từ Mệnh đề 14 và Mệnh đề 8 của no. 3.

#### Mệnh đề 15 {#top-i-s8-prop-15 .statement}

*Cho* $X$ *là một không gian chính quy*, $F$ *một tập con đóng của* $X$, $R$ *là quan hệ tương đương trên* $X$ *thu được bằng cách đồng nhất tất cả các điểm của* $F$ *[nói cách khác, quan hệ tương đương mà các lớp tương đương của nó là* $F$ *(nếu* $F \neq \emptyset$*) và các tập* $\{x\}$ *với* $x \in CF$*]. Khi đó không gian thương* $X/R$ *là Hausdorff*.

Cho $M$ và $N$ là hai lớp tương đương phân biệt trong $X$. Nếu mỗi lớp trong chúng chỉ gồm một điểm duy nhất trong phần bù của $F$, thì tồn tại hai lân cận mở rời nhau của $M$ và $N$ trong không gian con Hausdorff $CF$; đó là các lân cận của $M$ và $N$ trong $X$ và bão hòa đối với $R$. Nếu $M = F$ (do đó $F \neq \emptyset$) và $N = \{ b \}$ với $b \notin F$, thì vì $X$ là chính quy nên có một lân cận mở của $b$ và một lân cận mở của $F$ không giao nhau; các lân cận này bão hòa đối với $R$, và mệnh đề được chứng minh.

Chú ý rằng không gian thương $X/R$ không nhất thiết là chính quy (Chương IX, § 4, Bài tập 14).

### Bài tập {#top-i-s8-exercises}

Xem [các bài tập của § 8](exercises/s8/).
