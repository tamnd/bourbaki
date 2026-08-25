---
book: top
book_title: General Topology
chapter: III
chapter_title: Topological Groups
section: 3
section_title: Uniform structures on groups
lang: vi
source: top-i-iv
pdf_pages: 0248-0256, 0312-0313
extraction: ocr
subsections:
    - "no": 1
      title: THE RIGHT AND LEFT UNIFORMITIES ON A TOPOLOGICAL GROUP
      page: 0
      pdf_page: 248
    - "no": 2
      title: UNIFORMITIES ON SUBGROUPS, QUOTIENT GROUPS AND PRODUCT GROUPS
      page: 0
      pdf_page: 250
    - "no": 3
      title: COMPLETE GROUPS
      page: 0
      pdf_page: 251
    - "no": 4
      title: COMPLETION OF A TOPOLOGICAL GROUP
      page: 0
      pdf_page: 252
    - "no": 5
      title: UNIFORMITY AND COMPLETION OF A COMMUTATIVE TOPOLOGICAL GROUP
      page: 0
      pdf_page: 254
statements: 18
exercises: 12
content_sha256: 35563344e390f05fef7e65877244f32bb41b931c2239286d5d5fbd05f7779add
translated_from: content/en/top/III/03_s3_uniform_structures_on_groups.md
source_content_sha256: 4b4be51d0c9bcd3de9ff17b7a6c044b6d925fe61a3cd120addca4da3673e750a
translation_model: gpt-5.4
translation_run: translate-vi-cf854575
glossary_version: 34
glossary_terms_sha256: 01b0236b4d1a500f26692d0d82693fe07305fed31b0e5de34518fe46c819ff52
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 3. CÁC CẤU TRÚC ĐỀU TRÊN CÁC NHÓM

### 1. CÁC CẤU TRÚC ĐỀU PHẢI VÀ TRÁI TRÊN MỘT NHÓM TÔPÔ

Trong một nhóm tôpô G, ta có thể nhận thấy khả năng xác định một khái niệm về "các điểm đủ gần nhau" và do đó một cấu trúc đều, bằng cách làm như sau: nếu x và y là hai điểm bất kỳ của G, ta áp dụng cho cả hai điểm phép tịnh tiến đưa một trong hai điểm ấy, chẳng hạn x, về phần tử đơn vị e; khi đó "độ gần nhau" của x và y được đánh giá theo một nghĩa nào đó bởi lân cận V của e mà vào đó y được chuyển tới. Phép tịnh tiến này, gồm việc nhân cả x lẫn y với $x^{-1}$, có thể được thực hiện ở phải hoặc ở trái, và ta sẽ thấy rằng trong cả hai trường hợp ta thực sự thu được một cấu trúc đều trên G tương thích với tôpô của G. Hãy xét trường hợp trong đó các phép tịnh tiến được thực hiện ở phải; khi đó với mỗi lân cận V của e tương ứng tập hợp $V_d$ gồm các cặp $(x, y) \in G \times G$ sao cho $yx^{-1} \in V$. Gọi $\mathcal{G}_d$ là họ các tập hợp $V_d$, khi V chạy qua bộ lọc lân cận $\mathfrak{B}$ của e. Khi đó $\mathcal{G}_d$ là một hệ cơ sở của các entourage (Chương II, § 1, no. 1). Thật vậy, vì $e \in V$, đường chéo $\Delta$ của $G \times G$ được chứa trong $V_d$ với mọi $V \in \mathfrak{B}$, do đó $\mathcal{G}_d$ là một cơ sở bộ lọc và thỏa mãn tiên đề $(U'_1)$; vì các quan hệ $yx^{-1} \in V$ và $xy^{-1} \in V^{-1}$ là tương đương, ta có $\overline{V}_d^1 = (V^{-1})_d$, do đó $\overline{V}_d^1 \in \mathcal{G}_d$ theo (GV$_{\text{II}}$), nên (U'$_{\text{II}}$) được thỏa mãn; và sau cùng, các quan hệ $zx^{-1} \in V$ và $yz^{-1} \in V$ kéo theo $yx^{-1} \in V.V$; do đó $V_d \circ V_d$ được chứa trong (V.V)$_d$, và (GV$_{\text{I}}$) cho thấy rằng $\mathcal{G}_d$ thỏa mãn (U'$_{\text{III}}$).

Cấu trúc đều được xác định bởi $\mathcal{G}_d$ là tương thích với tôpô của G, vì các quan hệ $y \in V_d(x)$ và $y \in V.x$ theo định nghĩa là tương đương; nói cách khác $V_d(x) = V.x$.

Lập luận là tương tự khi các phép tịnh tiến ở bên trái, và do đó ta có thể đưa ra định nghĩa sau:

#### Định nghĩa 1 {#top-iii-s3-def-1 .statement}

*Cấu trúc đều phải (tương ứng, trái) trên một nhóm tôpô G là cấu trúc đều mà một hệ cơ bản các entourage của nó thu được bằng cách làm tương ứng với mỗi lân cận V của phần tử đơn vị e, tập hợp V$_d$ (tương ứng, V$_s$) các cặp $(x, y)$ sao cho $yx^{-1} \in V$ (tương ứng, $x^{-1}y \in V$).*

Khi V chạy qua một hệ cơ bản các lân cận của e, các tập hợp V$_d$ (tương ứng, V$_s$) tạo thành một hệ cơ bản các entourage của cấu trúc đều phải (tương ứng, trái).

Với mỗi mệnh đề về tôpô của một không gian đều thì tương ứng có một mệnh đề về tôpô của một nhóm; phép chuyển dịch được thực hiện theo Định nghĩa 1 và các công thức $V_d(x) = V.x,\ V_d(A) = V.A,\ V_s(x) = x.V,\ V_s(A) = A.V,$ là những hệ quả ngay lập tức của định nghĩa. Chẳng hạn, nếu A là một tập con không rỗng bất kỳ của G thì ta có (Chương II, § 1, no. 2, Hệ quả 1 của Mệnh đề 2)

$$
\overline{A} = \bigcap_{V \in \mathcal{B}} V.A = \bigcap_{V \in \mathcal{B}} A.V.
$$

Lại nữa (Chương II, § 1, no. 2, Hệ quả 3 của Mệnh đề 2), *mọi nhóm Hausdorff đều chính quy*.

Cấu trúc đều phải và cấu trúc đều trái trên một nhóm tôpô nói chung là phân biệt (xem Bài tập 4). Hiển nhiên chúng trùng nhau nếu nhóm là *giao hoán*, vì khi đó $V_d = V_s$; chúng cũng trùng nhau nếu nhóm là *compact* (Chương II, § 4, no. 1, Định lý 1).

Nói chung, ta sẽ ký hiệu bởi $G_s$ (tương ứng là $G_d$) *không gian đều* thu được bằng cách trang bị cho tập hợp G cấu trúc đều trái (tương ứng là phải).

#### Mệnh đề 1 {#top-iii-s3-prop-1 .statement}

*Các phép tịnh tiến trái và phải là những đẳng cấu của cấu trúc đều phải lên chính nó.*

Đối với các phép tịnh tiến phải, kết quả là hiển nhiên, vì quan hệ $yx^{-1} \in V$ là tương đương với $(ya)(xa)^{-1} \in V$ [nói cách khác, ánh xạ $(x, y) \to (xa, ya)$ để $V_d$ bất biến]. Đối với các phép tịnh tiến trái, kết quả suy ra từ $(GV_{\text{III}})$; thật vậy, $yx^{-1} \in V$ khi và chỉ khi $(ay)(ax)^{-1} \in aV a^{-1}$; do đó $x \to ax$ là liên tục đều trên $G_d$.

Tương tự, các phép tịnh tiến phải và trái là những đẳng cấu của cấu trúc đều trái lên chính nó.

Mọi *tự đẳng cấu trong* $x \to axa^{-1}$ của $G$ do đó là một tự đẳng cấu đối với cấu trúc nhóm của $G$, đối với tôpô của $G$, và đối với cả hai cấu trúc đều của $G$.

#### Mệnh đề 2 {#top-iii-s3-prop-2 .statement}

*Phép đối xứng* $x \to x^{-1}$ *là một đẳng cấu của cấu trúc đều phải lên cấu trúc đều trái.*

Đây là một hệ quả ngay lập tức của Định nghĩa 1.

Người đọc cần thận trọng đừng cho rằng ánh xạ $(x, y) \to xy$ từ không gian đều $G_d \times G_d$ vào không gian đều $G_d$ nói chung là liên tục đều. Tương tự, phép đối xứng $x \to x^{-1}$, khi được xét như một ánh xạ từ $G_d$ lên $G_d$, nói chung không liên tục đều (xem Bài tập 3 và 4).

#### Mệnh đề 3 {#top-iii-s3-prop-3 .statement}

*Mọi đồng cấu liên tục* $f$ *từ một nhóm tôpô* $G$ *vào một nhóm tôpô* $G'$ *đều liên tục đều khi được xét như một ánh xạ từ* $G_d$ *vào* $G'_d$ *(hoặc từ* $G_s$ *vào* $G'_s$).

Thật vậy, nếu $V'$ là một lân cận của phần tử đơn vị trong $G'$, và $V = \overline{f}^{-1}(V')$, thì quan hệ $yx^{-1} \in V$ kéo theo
$$
f(y)(f(x))^{-1} = f(yx^{-1}) \in V'.
$$

### 2. CÁC CẤU TRÚC ĐỀU TRÊN NHÓM CON, NHÓM THƯƠNG VÀ NHÓM TÍCH

Nếu $H$ là một nhóm con của một nhóm tôpô $G$, thì cấu trúc đều cảm sinh trên $H$ bởi cấu trúc đều phải của $G$ chính là cấu trúc đều phải của nhóm tôpô $H$.

Nếu $H$ là một nhóm con chuẩn tắc của $G$, và nếu $\varphi$ là ánh xạ chính tắc từ $G$ lên $G/H$, ta thu được một hệ cơ bản các lân cận của cấu trúc đều phải của nhóm thương $G/H$ bằng cách gán cho mỗi lân cận $V$ của phần tử đơn vị trong $G$ tập hợp tất cả các cặp $(\dot{x}, \dot{y})$ của $G/H$ sao cho $\dot{x}\dot{y}^{-1} \in \varphi(V)$ (\S 2, no. 6, Mệnh đề 17). Điều kiện này có nghĩa là tồn tại ít nhất một điểm $x \in \dot{x}$ và ít nhất một điểm $y \in \dot{y}$ sao cho $yx^{-1} \in V$ [tức là sao cho $(x, y) \in V_d$]. Đặc biệt, nếu $N$ là bao đóng của tập con $\{e\}$ của $G$, thì cấu trúc đều phải trên $G/N$ đẳng cấu với cấu trúc đều Hausdorff *liên kết* với cấu trúc đều phải trên $G$ (xem Chương II, \S 3, no. 8).

Có những kết quả tương tự đối với cấu trúc đều trái.

Các cấu trúc đều trái và phải trên nhóm tích $\prod_{i \in I} G_i$ là đồng nhất khi và chỉ khi các cấu trúc đều trái và phải trên mỗi nhân tử $G_i$ trùng nhau. Điều này luôn luôn đúng nếu một số $G_i$ là giao hoán và những nhóm còn lại là compact.

### 3. NHÓM ĐẦY ĐỦ

#### Định nghĩa 2 {#top-iii-s3-def-2 .statement}

*Một nhóm tôpô được gọi là đầy đủ nếu các cấu trúc đều trái và phải của nó là các cấu trúc của những không gian đầy đủ.*

Theo Mệnh đề 2 của no. 1, để một nhóm là đầy đủ thì chỉ cần *một* trong các cấu trúc đều của nó là một cấu trúc của không gian đầy đủ. $G$ đầy đủ khi và chỉ khi nhóm Hausdorff liên kết của nó ($§\ 2$, no. 6) đầy đủ.

Mọi nhóm con *đóng* của một nhóm đầy đủ đều đầy đủ (Chương II, § 3, no. 4, Mệnh đề 8). Mọi tích của các nhóm đầy đủ đều đầy đủ (Chương II, § 3, no. 5, Mệnh đề 10).

Mặt khác, nếu $G$ là một nhóm đầy đủ và $H$ là một nhóm con chuẩn đóng của $G$, thì nhóm thương $G/H$ không nhất thiết đầy đủ (tuy nhiên, xem Chương IX, § 3, no. 1, Mệnh đề 4).

#### Mệnh đề 4 {#top-iii-s3-prop-4 .statement}

*Nếu trong một nhóm tôpô $G$ có một lân cận $V$ của $e$ đầy đủ đối với cấu trúc đều phải hoặc cấu trúc đều trái, thì $G$ đầy đủ.*

Giả sử chẳng hạn $V$ là đầy đủ đối với cấu trúc đều phải, và $\mathfrak{F}$ là một bộ lọc Cauchy trên $G_d$; khi đó $\mathfrak{F}$ chứa một tập $V_d$-nhỏ $M$, và nếu $x_1 \in M$ thì do đó ta có $M \subset Vx_1$. Vậy nên vết của $\mathfrak{F}$ trên không gian con đầy đủ $Vx_1$ của $G_d$ là một bộ lọc Cauchy, hội tụ đến một điểm $x_0$; vì $x_0$ là một điểm tụ của $\mathfrak{F}$, nên nó là một giới hạn của $\mathfrak{F}$ (Chương II, § 3, no. 2, Hệ quả 2 của Mệnh đề 5).

#### Hệ quả 1 {#top-iii-s3-prop-4-cor-1 .statement}

*Một nhóm địa phương compact là đầy đủ.*

Vì mọi không gian compact đều đầy đủ đối với cấu trúc đều duy nhất của nó (Chương II, § 4, no. 1, Định lý 1).

#### Hệ quả 2 {#top-iii-s3-prop-4-cor-2 .statement}

*Mọi nhóm con compact địa phương của một nhóm tôpô Hausdorff $G$ đều đóng trong $G$.*

#### Mệnh đề 5 {#top-iii-s3-prop-5 .statement}

Cho $G_1$ là một nhóm tôpô, cho $G_2$ là một nhóm tôpô Hausdorff đầy đủ, và cho $H_1$ (tương ứng $H_2$) là một nhóm con trù mật của $G_1$ (tương ứng của $G_2$). Khi đó mọi đồng cấu liên tục $u$ từ $H_1$ vào $H_2$ đều có thể được mở rộng một cách duy nhất thành một đồng cấu liên tục $\bar{u}$ từ $G_1$ vào $G_2$. Hơn nữa, nếu $G_1$ Hausdorff và đầy đủ, và nếu $u$ là một đẳng cấu từ $H_1$ lên $H_2$, thì $\bar{u}$ là một đẳng cấu từ $G_1$ lên $G_2$.

$\bar{u}$ liên tục đều đối với các cấu trúc đều phải của $H_1$ và $H_2$ (no. 1, Mệnh đề 3), do đó có một mở rộng duy nhất thành một ánh xạ $\bar{u}$ từ $G_1$ vào $G_2$ liên tục đều đối với các cấu trúc đều phải của các nhóm này (Chương II, § 3, no. 6, Định lý 2). Hơn nữa, theo nguyên lý mở rộng các đồng nhất thức (Chương I, § 8, no. 1, Hệ quả 1 của Mệnh đề 2), $\bar{u}$ là một đồng cấu từ $G_1$ vào $G_2$, do đó có mệnh đề thứ nhất của Mệnh đề. Để chứng minh mệnh đề thứ hai, chỉ cần xét đẳng cấu $v$ của $H_2$ lên $H_1$, là nghịch đảo của $u$, và mở rộng của nó $\bar{v}$ thành một đồng cấu liên tục từ $G_2$ vào $G_1$; do tính duy nhất của phép mở rộng, $\bar{v} \circ \bar{u}$ và $\bar{u} \circ \bar{v}$ là các ánh xạ đồng nhất của $G_1$ và $G_2$ tương ứng, và vì vậy (Lý thuyết tập hợp, R, § 2, no. 12) $\bar{u}$ là song ánh.

#### Nhận xét {#top-iii-s3-n3-rem-1 .statement}

Nếu đồng cấu liên tục $u$ là song ánh, thì nói chung không suy ra rằng $\bar{u}$ là đơn ánh hoặc toàn ánh (x. Bài tập 12); nhưng xem no. 5, Mệnh đề 9.

### 4. HOÀN THÀNH CỦA MỘT NHÓM TÔPÔ

Cho $G$ là một nhóm tôpô Hausdorff. Không gian đều $G_d$ có thể được xem như một không gian con trù mật của bổ sung của nó $\hat{G}_d$. Ta sẽ khảo sát xem liệu $G$ có thể được xem như một nhóm con trù mật của một nhóm Hausdorff đầy đủ $G'$ hay không. Nếu được như vậy, thì không gian đều $G'_d$ phải đẳng cấu với $\hat{G}_d$ (Chương II, § 3, no. 6, Hệ quả của Định lý 2), và do đó ta phải có thể định nghĩa trên $\hat{G}_d$ một cấu trúc nhóm tôpô cảm sinh cấu trúc nhóm tôpô đã cho trên $G$. Do đó ta phải xét: 1) liệu ta có thể mở rộng bằng tính liên tục các hàm $xy$ và $x^{-1}$ lần lượt lên $\hat{G}_d \times \hat{G}_d$ và $\hat{G}_d$ hay không; 2) liệu các hàm được mở rộng như vậy có thực sự định nghĩa một cấu trúc nhóm trên $\hat{G}_d$ hay không (khi đó tất yếu chúng sẽ định nghĩa một cấu trúc nhóm tôpô trên $\hat{G}_d$ cảm sinh cấu trúc đã cho trên $G$). Tiếp theo ta phải thiết lập rằng 3) khi các phép toán trước đó là có thể, thì nhóm tôpô mà chúng định nghĩa là đầy đủ. Sau hết, ta sẽ thấy rằng 4) nếu có một nhóm đầy đủ thỏa mãn các điều kiện đã cho, thì nó là duy nhất đến đẳng cấu.

1) Mở rộng của $xy$ và $x^{-1}$ bằng tính liên tục. Vì các hàm $xy$ và $x^{-1}$ nói chung không liên tục đều, nên ta không thể áp dụng định lý về mở rộng các hàm liên tục đều (Chương II, § 3, no. 6, Định lý 2). Tuy nhiên, ta có thể mở rộng $xy$, nhờ Mệnh đề 11 của Chương II, § 3, no. 6 và Mệnh đề sau đây:

#### Mệnh đề 6 {#top-iii-s3-prop-6 .statement}

Cho $\mathfrak{F}$ và $\mathfrak{G}$ là hai bộ lọc Cauchy trên $G_d$. Khi đó ảnh của bộ lọc $\mathfrak{F} \times \mathfrak{G}$ qua ánh xạ $(x, y) \to xy$ là một cơ sở bộ lọc Cauchy trên $G_d$.

Hãy đánh giá "độ gần nhau" của $xy$ và $x'y'$ trong $G_d$; nói cách khác, hãy lập tích $(x'y')(xy)^{-1} = x'y'y^{-1}x^{-1}$. Với mỗi $a \in G$, ta cũng có thể viết $(x'y')(xy)^{-1} = (x'a^{-1})(ay'y^{-1}a^{-1})(ax^{-1})$. Ta sẽ thấy rằng, bằng một lựa chọn thích hợp của $a$, mỗi thừa số trong ba thừa số của tích này đều rất nhỏ mỗi khi các cặp $(x, y)$ và $(x', y')$ thuộc một tập đủ nhỏ của $\mathfrak{F} \times \mathfrak{G}$. Cho $V$ là một lân cận bất kỳ của $e$ trong $G$; khi đó tồn tại một tập $V_d$-nhỏ $A \in \mathfrak{F}$. Chọn $a$ trong $A$, khi đó nếu $x$ và $x'$ là hai điểm bất kỳ của $A$, ta có $x'a^{-1} \in V$ và $ax^{-1} \in V$. Mặt khác, quan hệ $ay'y^{-1}a^{-1} \in V$ tương đương với
$$
y'y^{-1} \in a^{-1}Va = W,
$$
và vì $W$ là một lân cận của $e$, tồn tại một tập $W_d$-nhỏ $B \in \mathfrak{G}$. Do đó với mọi $(x, y)$ và $(x', y')$ trong $A \times B$, ta có $(x'y')(xy)^{-1} \in V^3$, và điều này hoàn tất chứng minh.

Để $x^{-1}$ có thể được mở rộng bằng liên tục lên $\hat{G}_d$ thì điều kiện cần và đủ là *ảnh, qua phép đối xứng* $x \to x^{-1}$, *của một bộ lọc Cauchy trên $G_d$ là một bộ lọc Cauchy trên $G_d$* (Chương II, § 3, no. 6, Mệnh đề 11). Có những ví dụ về các nhóm tôpô trong đó điều kiện này không được thỏa mãn (xem Chương X, § 3, Bài tập 16); trong phần còn lại của chứng minh này, ta sẽ giả thiết rằng điều kiện ấy được thỏa mãn.

2) *Các hàm được mở rộng* $xy$ và $x^{-1}$ *xác định một cấu trúc nhóm trên* $\hat{G}_d$. Thật vậy, nếu ta áp dụng nguyên lý mở rộng các đồng nhất thức (Chương I, § 8, no. 1, Mệnh đề 2, Hệ quả 1) cho các hàm $x(yz)$ và $(xy)z$, được định nghĩa trên $\hat{G}_d \times \hat{G}_d \times \hat{G}_d$ và bằng nhau trên không gian con trù mật $G_d \times G_d \times G_d$, thì ta thấy rằng luật hợp thành $(x, y) \to xy$ là *kết hợp* trên $\hat{G}_d$. Vì cùng lý do đó, các hàm $x, ex, xe$ là đồng nhất trên $\hat{G}_d$, và các hàm $e, xx^{-1}, x^{-1}x$ là đồng nhất trên $\hat{G}_d$.

3) *Nhóm tôpô* $\hat{G}_d$ *là đầy đủ*. Gọi $\mathcal{U}_d$ là *cấu trúc đều phải* của nó, và gọi $\mathcal{U}$ là cấu trúc đều trên $\hat{G}_d$ thu được bằng cách *làm đầy đủ* cấu trúc đều phải của $G$. Khi đó $\mathcal{U}$ và $\mathcal{U}_d$ cảm sinh *cùng một* cấu trúc đều trên $G$, và do đó mọi cơ sở bộ lọc Cauchy $\mathcal{B}$ *trên* $G$ *đối với* $\mathcal{U}_d$ *cũng là một cơ sở bộ lọc Cauchy đối với* $\mathcal{U}$. Bây giờ $\mathcal{B}$ hội tụ trong $\hat{G}_d$,

4) *Tính duy nhất.* Điều này suy ra từ Mệnh đề 5 của no. 3.

Tóm lại, chúng ta đã chứng minh định lý sau đây:

#### Định lý 1 {#top-iii-s3-thm-1 .statement}

*Một nhóm tôpô Hausdorff $G$ đẳng cấu với một nhóm con trù mật của một nhóm đầy đủ $\hat{G}$ khi và chỉ khi ảnh, dưới đối xứng $x \to x^{-1}$, của một bộ lọc Cauchy đối với cấu trúc đều phải của $G$ là một bộ lọc Cauchy đối với cấu trúc đều này. Nhóm đầy đủ $\hat{G}$ (được gọi là phép hoàn thành của $G$) khi đó là duy nhất (sai khác bởi đẳng cấu).*

#### Mệnh đề 7 {#top-iii-s3-prop-7 .statement}

*Cho $G$ là một nhóm tôpô Hausdorff có một phép hoàn thành $\hat{G}$. Khi đó các bao đóng trong $\hat{G}$ của các lân cận của phần tử đơn vị trong $G$ tạo thành một hệ cơ bản các lân cận của phần tử đơn vị trong $\hat{G}$.*

Vì $\hat{G}$ là chính quy, mọi lân cận của phần tử đơn vị trong $\hat{G}$ đều chứa bao đóng $V$ của một lân cận mở $U$ của $e$ trong $\hat{G}$, và $V$ cũng là bao đóng của vết của $U$ trên $G$.

Cho $G$ là một nhóm không nhất thiết Hausdorff; đặt $N = \overline{\{e\}}$, và gọi $G' = G/N$ là nhóm Hausdorff liên kết với $G$ (\S 2, no. 6). Nếu $G'$ có một hoàn thành $\hat{G}'$, thì hoàn thành này được gọi là *hoàn thành Hausdorff* của $G$ và được ký hiệu là $\hat{G}$; khi đó $\hat{G}'_d$ (resp. $\hat{G}'_s$) là *hoàn thành Hausdorff* (Chương II, § 3, no. 7) của không gian đều $G_d$ (resp. $G_s$).

#### Mệnh đề 8 {#top-iii-s3-prop-8 .statement}

*Cho $G$ là một nhóm tôpô có một hoàn thành Hausdorff $\hat{G}'$. Khi đó mọi đồng cấu liên tục $u$ của $G$ vào một nhóm Hausdorff đầy đủ $H$ đều có thể được phân tích duy nhất thành $u = v \circ \varphi$, trong đó $v$ là một đồng cấu liên tục của $\hat{G}'$ vào $H$ và $\varphi$ là ánh xạ chính tắc của $G$ vào $\hat{G}'$ (hợp thành của đơn ánh chính tắc của $G'$ vào $\hat{G}'$ và đồng cấu chính tắc $\psi$ của $G$ lên $G/N = G'$).*

Vì hạt nhân của $u$ là đóng và chứa $e$, nên nó chứa $N$, và do đó $u$ có thể được viết thành $u = w \circ \psi$, trong đó $w$ là một đồng cấu liên tục từ $G'$ vào $H$; bây giờ áp dụng Mệnh đề 5 của no. 3 cho $w$.

### 5. CẤU TRÚC ĐỀU VÀ PHÉP HOÀN THÀNH CỦA MỘT NHÓM TÔPÔ GIAO HOÁN

Ta đã nhận xét rằng các cấu trúc đều trái và phải trùng nhau trên một nhóm tôpô giao hoán $G$; mỗi khi ta nói đến *cấu trúc đều* của $G$, thì đó là cấu trúc đều duy nhất này mà ta muốn nói đến.

#### Định lý 2 {#top-iii-s3-thm-2 .statement}

Cho $G$ là một nhóm tôpô giao hoán. Khi đó các ánh xạ $x^{-1}$ và $xy$ lần lượt liên tục đều trên $G$ và $G \times G$. Hơn nữa $G$ có một hoàn chỉnh Hausdorff $\hat{G}$, và $\hat{G}$ là giao hoán.

Tính liên tục đều của $x^{-1}$ suy ra từ Mệnh đề 2 của no. 1, và tính liên tục đều của $xy$ suy ra từ Mệnh đề 3 của no. 1, vì $(x, y) \to xy$ là một đồng cấu liên tục từ $G \times G$ vào $G$. Nếu $G$ là Hausdorff, thì nó thỏa mãn điều kiện của Định lý 1 ở no. 4 (cũng như mọi nhóm Hausdorff mà các cấu trúc đều trái và phải của nó trùng nhau); hơn nữa các hàm $xy$ và $yx$ bằng nhau trên $\hat{G} \times \hat{G}$ theo nguyên lý mở rộng các đồng nhất thức; do đó suy ra phần thứ hai của định lý, bằng cách xét trong trường hợp tổng quát nhóm Hausdorff liên kết với $G$.

Đặc biệt, từ định lý này suy ra rằng nếu $f$ và $g$ là hai ánh xạ liên tục đều của một không gian đều $X$ vào một nhóm giao hoán $G$, viết theo lối cộng, thì các hàm $-f$ và $f + g$ là liên tục đều.

#### Mệnh đề 9 {#top-iii-s3-prop-9 .statement}

Cho $G$ là một nhóm giao hoán, và $\mathcal{T}_1, \mathcal{T}_2$ là hai tôpô Hausdorff tương thích với cấu trúc nhóm của $G$. Giả sử rằng $\mathcal{T}_1$ mịn hơn $\mathcal{T}_2$ và tồn tại một hệ cơ bản các lân cận của $o$ đối với $\mathcal{T}_1$ mà đều đóng đối với $\mathcal{T}_2$. Gọi $G_1, G_2$ lần lượt là các bổ sung của $G$ đối với các tôpô $\mathcal{T}_1, \mathcal{T}_2$, và gọi $f : G_1 \to G_2$ là đồng cấu liên tục kéo dài ánh xạ đồng nhất của $G$ (no. 3, Mệnh đề 5). Khi đó $f$ là đơn ánh.

Giả sử rằng $G$ được viết theo phép cộng. Gọi $\mathcal{U}_1$ là cấu trúc đều trên $G$ tương ứng (no. 1) với tôpô $\mathcal{T}_1$: chỉ cần chứng minh rằng nếu $\mathfrak{F}$ và $\mathfrak{F}'$ là hai bộ lọc Cauchy cực tiểu (Chương II, § 3, no. 2) đối với $\mathcal{U}_1$, cùng hội tụ trong $G_2$ đến một điểm $a$, thì $\mathfrak{F} = \mathfrak{F}'$ (Chương II, § 3, no. 7). Để làm điều đó, chỉ cần chứng minh rằng $\mathfrak{F} \cap \mathfrak{F}'$ là một bộ lọc Cauchy đối với $\mathcal{U}_1$. Cho $V$ là một lân cận của $o$ trong $G$ đối với $\mathcal{T}_1$, sao cho $V$ đóng trong $\mathcal{T}_2$, và cho $W$ là một lân cận đối xứng của $o$ trong $G$ đối với $\mathcal{T}_1$, sao cho $W + W \subset V$. Theo giả thiết, có một tập $W_d$-nhỏ $M$ (resp. $M'$) trong $\mathfrak{F}$ (resp. $\mathfrak{F}'$); nếu $x \in M$ và $y \in M$ thì ta có $y - x \in W$, tức là $y \in x + W$. Nếu $\overline{W}$ và $\overline{V}$ là các bao đóng của $W$ và $V$ trong $G_2$, suy ra $y \in x + \overline{W}$, và do đó, vì $a$ thuộc bao đóng của $M$, nên $a \in x + \overline{W}$ với mọi $x \in M$. Tương tự, $a \in x' + \overline{W}$ với mọi $x' \in M'$, và vì thế $x - x' \in \overline{W} + \overline{W}$; nhưng vì $(x, y) \to x + y$ là một ánh xạ liên tục từ $G_2 \times G_2$ vào $G_2$, nên ta có $\overline{W} + \overline{W} \subset \overline{W} + \overline{W} \subset \overline{V}$. Suy ra rằng nếu $x \in M$ và $x' \in M'$, thì $x - x' \in \overline{V} \cap G = V$, vì $V$ đóng trong $\mathcal{T}_2$; và điều này hoàn thành chứng minh.

#### Hệ quả 1 {#top-iii-s3-prop-9-cor-1 .statement}

Dưới các giả thiết của Mệnh đề 9, nếu $A$ là một tập con của $G$ là một không gian con đầy đủ đối với cấu trúc đều $U_2$ tương ứng với $\mathcal{T}_2$, thì $A$ cũng là một không gian con đầy đủ đối với cấu trúc đều $U_1$ tương ứng với $\mathcal{T}_1$.

Nếu $A_1$ là bao đóng của $A$ trong $G_1$, thì $f(A_1)$ được chứa trong bao đóng của $A$ trong $G_2$, mà theo giả thiết thì bằng $A$. Vì $f(A) = A$ theo định nghĩa và $f$ là đơn ánh, ta có $A_1 = A$.

#### Hệ quả 2 {#top-iii-s3-prop-9-cor-2 .statement}

Cho $G$ là một nhóm giao hoán và cho $\mathcal{T}_1, \mathcal{T}_2$ là hai tôpô tương thích với cấu trúc nhóm của $G$. Giả sử rằng $\mathcal{T}_1$ mịn hơn $\mathcal{T}_2$ và rằng tồn tại một hệ cơ bản $\mathcal{B}$ các lân cận của $O$ đối với $\mathcal{T}_1$ mà đầy đủ đối với cấu trúc đều $U_2$ tương ứng với $\mathcal{T}_2$. Khi đó $G$ là đầy đủ đối với cấu trúc đều $U_1$ tương ứng với $\mathcal{T}_1$.

Các tập hợp của $\mathcal{B}$ là đóng trong tôpô $\mathcal{T}_2$, do đó đầy đủ đối với cấu trúc đều $U_1$ theo Hệ quả 1; vì thế kết quả suy ra từ Mệnh đề 4 của no. 3.

### Bài tập {#top-iii-s3-exercises}

Xem [các bài tập cho § 3](exercises/s3/).
