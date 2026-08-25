---
book: top
book_title: General Topology
chapter: X
chapter_title: Function spaces
section: 2
section_title: Equicontinuous sets
lang: vi
source: top-v-x
pdf_pages: 0289-0299, 0327-0333
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION AND GENERAL CRITERIA
      page: 0
      pdf_page: 289
    - "no": 2
      title: SPECIAL CRITERIA FOR EQUICONTINUITY
      page: 0
      pdf_page: 293
    - "no": 3
      title: CLOSURE OF AN EQUICONTINUOUS SET
      page: 0
      pdf_page: 295
    - "no": 4
      title: POINTWISE CONVERGENCE AND COMPACT CONVERGENCE ON EQUICONTINUOUS SETS
      page: 0
      pdf_page: 295
    - "no": 5
      title: COMPACT SETS OF CONTINUOUS MAPPINGS
      page: 0
      pdf_page: 296
statements: 24
exercises: 16
content_sha256: eef5e35b8ba01a80d9a4e01fc2f4d2bfeba77b69e76420c5e0ca8b0c333e0ab9
translated_from: content/en/top/X/02_s2_equicontinuous_sets.md
source_content_sha256: 955831a757822ebbfc21d4e0b552cc9058dc588efa14540061dfee0a4c9bf02b
translation_model: gpt-5.4-mini, gpt-5-6-mini
translation_run: translate-vi-82a58eef
glossary_version: 34
glossary_terms_sha256: fb7b8e24918abd89b23caeac4d43efbdb7cdf83f7df27069ff7d4c85e42762de
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 2. CÁC TẬP ĐỀU LIÊN TỤC

### 1. ĐỊNH NGHĨA VÀ CÁC TIÊU CHUẨN CHUNG

#### Định nghĩa 1 {#top-x-s2-def-1 .statement}

*Cho $X$ là một không gian tôpô và $Y$ là một không gian đều. Một tập con $H$ của $\mathcal{F}(X; Y)$ được gọi là đều liên tục tại một điểm $x_0 \in X$ nếu, với mỗi lân cận $V$ của $Y$, tồn tại một lân cận $U$ của $x_0$ trong $X$ sao cho* (f(x_0), f(x)) \in V \text{ với mọi } x \in U \text{ và mọi } f \in H. \text{ H được gọi là đều liên tục nếu nó đều liên tục tại mọi điểm của } X.*

#### Định nghĩa 2 {#top-x-s2-def-2 .statement}

Cho X và Y là hai không gian đều. Một tập con H của $\mathcal{F}(X; Y)$ được gọi là đều liên tục đều nếu, với mỗi lân cận V của Y, tồn tại một lân cận U của X sao cho ta có $(f(x), f(x')) \in V$ bất cứ khi nào $(x, x') \in U$ và $f \in H$.

Một họ $(f_i)_{i \in I}$ các ánh xạ của X vào Y được gọi là đều liên tục tại một điểm $x_0$ (tương ứng, đều liên tục, đều liên tục đều) nếu tập hợp các $f_i$ là đều liên tục tại $x_0$ (tương ứng, đều liên tục, đều liên tục đều).

Hiển nhiên là nếu $H \subset \mathcal{F}(X; Y)$ đều liên tục tại $x_0$, thì mỗi $f \in H$ đều liên tục tại $x_0$; nếu H đều liên tục, thì mỗi $f \in H$ đều liên tục trên X, tức là $H \subset C(X; Y)$. Tương tự, nếu H đều liên tục đều (X là một không gian đều), thì mọi $f \in H$ đều liên tục đều trên X. Cũng hiển nhiên rằng một tập các ánh xạ đều liên tục đều thì đều liên tục; nhưng một tập các ánh xạ liên tục đều có thể đều liên tục mà không đều liên tục đều (xem Bài tập 1; Hệ quả 2 của Mệnh đề 1; và no. 2, Mệnh đề 4).

#### Ví dụ 1 {#top-x-s2-n1-exa-1 .statement}

Cho X là một không gian tôpô (tương ứng, một không gian đều) và Y là một không gian đều. Mọi tập hữu hạn các ánh xạ liên tục (tương ứng, liên tục đều) từ X vào Y đều đều liên tục (tương ứng, đều liên tục đều).

#### Ví dụ 2 {#top-x-s2-n1-exa-2 .statement}

Cho X, Y là hai không gian mêtric, d (tương ứng, $d'$) là mêtric trên X (tương ứng, trên Y), và cho k, $\alpha$ là hai số thực > 0. Khi đó tập tất cả các ánh xạ $f : X \to Y$ sao cho
$$
d'(f(x), f(x')) \leq k(d(x, x'))^\alpha
$$
với mỗi cặp điểm $x, x'$ của X, là đều liên tục đều. Chẳng hạn, tập tất cả các đẳng cự (Chương IX, § 2, no. 2) của X lên một tập con của Y đều liên tục đều.

\* Cho H là một tập các hàm nhận giá trị thực được xác định trên một khoảng $I \subset \mathbf{R}$, khả vi trên I và thỏa mãn $|f'(x)| \leq k$ với mọi $x \in I$ và mọi $f \in H$. Khi đó H đều liên tục đều, vì nếu $x_1, x_2$ là bất kỳ hai điểm của I thì ta có $|f(x_1) - f(x_2)| \leq k|x_1 - x_2|$ với mỗi $f \in H$ theo định lý giá trị trung bình. \*

#### Ví dụ 3 {#top-x-s2-n1-exa-3 .statement}

Cho G là một nhóm tôpô, cho Y là một không gian đều và cho $f : G \to Y$ là một ánh xạ liên tục đều [G được trang bị tính đều trái của nó (Chương III, § 3, no. 1)]. Với mỗi $s \in G$, cho $f_s$ là ánh xạ $x \to f(sx)$ của G vào Y. Khi đó tập các ánh xạ $f_s$ ($s \in G$) là đều liên tục đều, vì quan hệ $x^{-1}x' \in V$ tương đương với $(sx)^{-1}(sx') \in V$.

#### Mệnh đề 1 {#top-x-s2-prop-1 .statement}

Cho T là một tập, cho $\mathcal{S}$ là một tập các tập con của T, cho Y là một không gian đều, X một không gian tôpô (tương ứng, đều), và cho f là một ánh xạ của $T \times X$ vào $Y$. Với mỗi $A \in \mathcal{S}$, cho $H_A \subset \mathcal{F}(X; Y)$ là tập tất cả các ánh xạ $x \to f(t, x)$ khi $t$ chạy qua $A$. Khi đó ánh xạ $x \to f(., x)$ của X vào $\mathcal{F}_\mathcal{S}(T; Y)$ liên tục tại một điểm $x_0 \in X$ (tương ứng, liên tục đều) khi và chỉ khi tập $H_A$ đều liên tục tại $x_0$ (tương ứng, đều liên tục đều) với mọi $A \in \mathcal{S}$.

Trước hết xét trường hợp riêng khi $\mathcal{S} = \{ T \}$, tức là $\mathcal{F}_\mathcal{S}(T; Y) = \mathcal{F}_u(T; Y)$. Với mỗi lân cận $V$ của $Y$, điều kiện $(f(., x), f(., x')) \in W(V)$ có nghĩa là $(f(t, x), f(t, x')) \in V$ với mọi $t \in T$. Nói rằng $x \to f(., x)$ là liên tục tại $x_0$ (tương ứng là liên tục đều) do đó tương đương với việc nói rằng, với mỗi lân cận $V$ của $Y$, tồn tại một lân cận $U$ của $x_0$ trong $X$ (tương ứng một lân cận $M$ của $X$) sao cho quan hệ $x \in U$ [tương ứng $(x, x') \in M$] kéo theo $(f(t, x), f(t, x_0)) \in V$ [tương ứng $(f(t, x), f(t, x')) \in V$] với mọi $t \in T$, và mệnh đề suy ra từ các Định nghĩa 1 và 2. Trong trường hợp tổng quát, ta phải biểu diễn rằng, với mỗi $A \in \mathcal{S}$, ánh xạ $x \to f(., x)|A$ của $X$ vào $\mathcal{F}_u(A; Y)$ là liên tục tại $x_0$ (tương ứng liên tục đều), theo § 1, no. 2; từ những điều đã nói, điều này tương đương với việc nói rằng, với mỗi $A \in \mathcal{S}$, $H_A$ là liên tục đều tại $x_0$ (tương ứng liên tục đều đồng nhất).

Mệnh đề 1 cho phép ta chuyển các Định nghĩa 1 và 2 thành những dạng đôi khi hữu ích, bằng cách áp dụng nó vào trường hợp $T = H$ và $f$ là ánh xạ $(h, x) \to h(x)$ của $H \times X$ vào $Y$; vì $f(., x)$ là ánh xạ $h \to h(x)$ của $H$ vào $Y$, ta thấy rằng:

#### Hệ quả 1 {#top-x-s2-prop-1-cor-1 .statement}

Cho $X$ là một không gian tôpô (tương ứng không gian đều), $Y$ là một không gian đều và $H$ là một tập con của $\mathcal{F}(X; Y)$. Với mỗi $x \in X$, ký hiệu $\tilde{x}$ là ánh xạ $h \to h(x)$ của $H$ vào $Y$. Khi đó $H$ là liên tục đều tại $x_0$ (tương ứng liên tục đều đồng nhất) khi và chỉ khi ánh xạ $x \to \tilde{x}$ của $X$ vào không gian đều $\mathcal{F}_u(H; Y)$ là liên tục tại $x_0$ (tương ứng liên tục đều).

Đặc biệt, nếu $X$ là compact, mọi ánh xạ liên tục của $X$ vào $\mathcal{F}_u(H; Y)$ đều là liên tục đều (Chương II, § 4, no. 1, Định lý 2). Do đó:

#### Hệ quả 2 {#top-x-s2-prop-1-cor-2 .statement}

Cho $X$ là một không gian compact, $Y$ là một không gian đều. Khi đó mọi tập con liên tục đều của $\mathcal{F}(X; Y)$ đều là liên tục đều đồng nhất.

Giả sử bây giờ ta có một tập hợp $T$, một không gian tôpô $X$, một không gian đều $Y$ và một ánh xạ $f : T \times X \to Y$. Ký hiệu $\tilde{f}$ là ánh xạ $x \to f(., x)$ của $X$ vào $\mathcal{F}_u(T; Y)$, và xét ánh xạ chính tắc $\theta : (t, g) \to g(t)$ của $T \times \mathcal{F}_u(T; Y)$ vào $Y$. Rõ ràng biểu đồ

$$
\begin{array}{ccc}
T \times X & \xrightarrow{f} & Y \\
\downarrow_{\iota_T \times \tilde{f}} & & \uparrow \theta \\
T \times \mathcal{F}_u(T; Y)
\end{array}
$$

(trong đó $i_T$ là ánh xạ đồng nhất của T) là giao hoán. Giả sử bây giờ T được trang bị một tôpô và rằng, với mỗi $x \in X$, ánh xạ $f(., x) : t \to f(t., x)$ là liên tục; khi đó ta có thể thay $\mathcal{F}_u(T; Y)$ bằng $\mathcal{C}_u(T; Y)$ trong biểu đồ trên. Nhưng ta biết rằng $\theta$ là liên tục theo § 1, no. 6, Mệnh đề 9; do đó nếu $\tilde{f}$ liên tục thì suy ra $f$ liên tục. Vì tính liên tục của $\tilde{f}$ có thể được diễn đạt nhờ Mệnh đề 1, ta thu được kết quả sau:

#### Hệ quả 3 {#top-x-s2-prop-1-cor-3 .statement}

*Cho T, X là các không gian tôpô, cho Y là một không gian đều và cho f là một ánh xạ của T × X vào Y. Khi đó f liên tục, miễn là các điều kiện sau được thỏa mãn:*

1) *Với mỗi $x \in X$, ánh xạ riêng phần $t \to f(t, x)$ là liên tục.*

2) *Khi t chạy qua T, các ánh xạ riêng phần $x \to f(t, x)$ tạo thành một tập con đẳng liên tục của $\mathcal{F}(X; Y)$. \*

Cụ thể hơn, lấy T là một tập con H của $\mathcal{F}(X; Y)$ và lấy f là ánh xạ chính tắc $(h, x) \to h(x)$ của $H \times X$ vào Y; điều kiện 1) của Hệ quả 3 có nghĩa là H được trang bị một tôpô mịn hơn tôpô hội tụ từng điểm, và điều kiện 2) có nghĩa là H đẳng liên tục. Do đó:

#### Hệ quả 4 {#top-x-s2-prop-1-cor-4 .statement}

*Cho X là một không gian tôpô, Y là một không gian đều, H là một tập đẳng liên tục các ánh xạ của X vào Y. Nếu H được trang bị tôpô hội tụ từng điểm, thì ánh xạ $(h, x) \to h(x)$ của $H \times X$ vào Y là liên tục.*

Một cách trực quan hơn, điều này diễn đạt rằng nếu $h \in H$ hội tụ *từng điểm* đến $h_0 \in H$ và nếu $x \in X$ hội tụ đến $x_0$, thì $h(x)$ hội tụ đến $h_0(x_0)$.

#### Hệ quả 5 {#top-x-s2-prop-1-cor-5 .statement}

*Cho X là một không gian tôpô, cho Y, Z là hai không gian đều và cho H là một tập đẳng liên tục các ánh xạ của Y vào Z. Nếu H, $\mathcal{C}(X; Y)$ và $\mathcal{C}(X; Z)$ được trang bị tôpô hội tụ từng điểm, thì ánh xạ $(u, v) \to u \circ v$ của $H \times \mathcal{C}(X; Y)$ vào $\mathcal{C}(X; Z)$ là liên tục.*

Ta phải chứng minh rằng, với mỗi $x \in X$, ánh xạ $(u, v) \to u(v(x))$ của $H \times \mathcal{C}(X; Y)$ vào Z là liên tục. Bây giờ $v \to v(x)$ là liên tục trên H (\S 1, no. 2, Nhận xét 6), và từ Hệ quả 4 suy ra rằng $(u, y) \to u(y)$ là một ánh xạ liên tục của $H \times Y$ vào Z; vì $(u, v) \to u(v(x))$ là hợp thành của $(u, y) \to u(y)$ và $(u, v) \to (u, v(x))$, nên kết quả được chứng minh.

Mệnh đề sau và hệ quả của nó là các bản tương ứng của Hệ quả 3 và 4 của Mệnh đề 1 đối với các tập đẳng liên tục đều các ánh xạ:

#### Mệnh đề 2 {#top-x-s2-prop-2 .statement}

Cho T, X, Y là các không gian đều và cho f là một ánh xạ của T × X vào Y. Khi đó f liên tục đều khi và chỉ khi hai điều kiện sau được thỏa mãn:

1) Các ánh xạ x → f(t, x) (t ∈ T) tạo thành một tập con đẳng liên tục đều của $\mathcal{F}(X; Y)$.

2) Các ánh xạ t → f(t, x) (x ∈ X) tạo thành một tập con đẳng liên tục đều của $\mathcal{F}(T; Y)$.

Dễ thấy rằng các điều kiện là cần thiết. Chiều ngược lại, giả sử chúng được thỏa mãn. Cho W là một lân cận chéo của Y; khi đó tồn tại một lân cận chéo U của T và một lân cận chéo V của X sao cho:

1) $(t', t'') \in U$ suy ra rằng, với mỗi $x \in X$,
$$
(f(t', x), f(t'', x)) \in W.
$$

2) $(x', x'') \in V$ suy ra rằng, với mỗi $t \in T$,
$$
(f(t, x'), f(t, x'')) \in W.
$$

Bây giờ rõ ràng là quan hệ "$(t', t'') \in U$ và $(x', x'') \in V$" suy ra rằng $(f(t', x'), f(t'', x'')) \in \hat{W}$, do đó có kết quả.

Đặc biệt, cho T là một tập con H của $\mathcal{F}(X; Y)$, được trang bị tính đều của sự hội tụ đều, và cho f là ánh xạ chính tắc $(h, x) \to h(x)$; khi đó điều kiện 2) của Mệnh đề 2 được thỏa mãn một cách hiển nhiên vì, với mỗi bao lân cận W của Y, tập các cặp $(h', h'')$ sao cho $(h'(x), h''(x)) \in W$ với mọi $x \in X$ theo định nghĩa là một bao lân cận của cấu trúc đều của H. Do đó chỉ còn phải phát biểu điều kiện 1); nói cách khác:

#### Hệ quả {#top-x-s2-n1-cor-1 .statement}

Cho X, Y là hai không gian đều và cho H là một tập con của $\mathcal{F}(X; Y)$. Khi đó H là đều liên tục đều khi và chỉ khi ánh xạ $(h, x) \to h(x)$ của $H \times X$ vào Y là đồng đều liên tục, với H được trang bị tính đều của sự hội tụ đều.

### 2. CÁC TIÊU CHUẨN ĐẶC BIỆT CHO TÍNH ĐỀU LIÊN TỤC

Rõ ràng rằng mọi tập con của một tập đều liên tục (resp. đều liên tục đều) đều là đều liên tục (resp. đều liên tục đều). Hơn nữa, nếu X là một không gian tôpô (resp. không gian đều) và Y là một không gian đều, thì mọi hợp hữu hạn của các tập con đều liên tục (resp. đều liên tục đều) của $\mathcal{F}(X; Y)$ đều liên tục (resp. đều liên tục đều).

Cho X, X' là hai không gian tôpô (resp. không gian đều), cho Y, Y' là hai không gian đều, cho $f : X \to X'$ là một ánh xạ liên tục (resp. đồng đều liên tục) và cho $g : Y \to Y'$ là một ánh xạ đồng đều liên tục.

Suy ra ngay lập tức từ các định nghĩa rằng ánh xạ $u \to g \circ u \circ f$ của $\mathcal{F}(X; Y)$ vào $\mathcal{F}(X'; Y')$ biến các tập đều liên tục (resp. đều liên tục đều) thành các tập đều liên tục (resp. đều liên tục đều).

#### Mệnh đề 3 {#top-x-s2-prop-3 .statement}

*Cho $X$ là một không gian tôpô (resp. không gian đều), cho $(Y_i)_{i \in I}$ là một họ các không gian đều, cho $Y$ là một tập hợp, và với mỗi $i \in I$, cho $f_i$ là một ánh xạ từ $Y$ vào $Y_i$. Cho $Y$ được trang bị tính đều thô nhất sao cho mọi $f_i$ đều là đồng đều liên tục. Để một tập con $H$ của $\mathcal{F}(X; Y)$ là đều liên tục (resp. đều liên tục đều) thì cần và đủ rằng, với mỗi $i \in I$, ảnh của $H$ qua ánh xạ $u \to f_i \circ u$ là một tập con đều liên tục (resp. đều liên tục đều) của $\mathcal{F}(X; Y_i)$. \*

Đây là hệ quả ngay lập tức của Định nghĩa 1 và 2 và của định nghĩa các bao lân cận của Y.

#### Mệnh đề 4 {#top-x-s2-prop-4 .statement}

*Cho $X, Y$ là hai không gian đều và cho H là một tập các ánh xạ đồng đều liên tục từ $X$ vào $Y$. Cho $\hat{X}, \hat{Y}$ là các hoàn thiện Hausdorff tương ứng của $X, Y$, và ký hiệu $\tilde{H}$ là tập các ánh xạ $\hat{u} : \hat{X} \to \hat{Y}$ khi u chạy qua H (Chương II, § 3, no. 7, Mệnh đề 15). Khi đó H đều liên tục đều khi và chỉ khi $\tilde{H}$ đều liên tục đều.*

Ta nhắc lại rằng biểu đồ

$$
\begin{array}{ccc}
X & \xrightarrow{u} & Y \\
i \downarrow & & j \downarrow \\
\hat{X} & \xrightarrow{\hat{u}} & \hat{Y}
\end{array}
$$

là giao hoán, trong đó $i$ và $j$ là các ánh xạ chính tắc; hơn nữa, cấu trúc đều của $X$ (resp. $Y$) là ảnh ngược bởi $i$ (resp. $j$) của cấu trúc đều của $\hat{X}$ (resp. $\hat{Y}$). Suy ra $H$ đều liên tục đều khi và chỉ khi ảnh của nó qua ánh xạ $u \to j \circ u$ đều liên tục đều (Mệnh đề 3), và ta có thể ngay từ đầu chỉ xét trường hợp $Y$ là Hausdorff và đầy đủ; hơn nữa, nếu $\tilde{H}$ đều liên tục đều thì $H$ cũng vậy, vì nó là ảnh của $\tilde{H}$ qua ánh xạ $\hat{u} \to \hat{u} \circ i$; do đó còn lại phải chứng minh chiều đảo lại khi $Y = \hat{Y}$. Cho $V$ là một lân cận đóng của $Y$; theo giả thiết, có một lân cận $U$ của $X$ sao cho các điều kiện $(x, x') \in U$ và $u \in H$ kéo theo $(u(x), u(x')) \in V$. Bây giờ, nếu $U'$ là ảnh của $U$ qua $i \times i$, thì bao đóng $\overline{U'}$ của $U'$ trong $\hat{X} \times \hat{X}$ là một lân cận của $\hat{X}$ (Chương II, § 3, no. 7, Mệnh đề 12); giả thiết suy ra rằng, mỗi khi $(z, z') \in U'$ và $u \in H$, ta có $(\hat{u}(z), \hat{u}(z')) \in V$. Vì $V$ đóng và $\hat{u}$ liên tục, ta cũng có $(\hat{u}(t), \hat{u}(t')) \in V$ với mọi $(t, t') \in \overline{U'}$ và mọi $u \in H$; điều đó hoàn tất chứng minh.

#### Mệnh đề 5 {#top-x-s2-prop-5 .statement}

Cho $G, G'$ là hai nhóm tôpô được trang bị các cấu trúc đều trái của chúng, và cho $H$ là một tập các đồng cấu từ $G$ vào $G'$. Khi đó các điều kiện sau là tương đương:
a) $H$ đều liên tục tại phần tử đơn vị $e$ của $G$,
b) $H$ đều liên tục,
c) $H$ đều liên tục đều.

Chỉ cần chứng minh a) suy ra c). Cho $V'$ là một lân cận của phần tử đơn vị $e'$ của $G'$; khi đó, theo giả thiết, có một lân cận $V$ của $e$ trong $G$ sao cho $u(V) \subset V'$ với mọi $u \in H$; vì các phần tử của $H$ là các đồng cấu, điều kiện $x^{-1} y \in V$ suy ra rằng ta có
$$
(u(x))^{-1} u(y) = u(x^{-1} y) \in V'.
$$
Xét theo định nghĩa các lân cận của các cấu trúc đều trái của $G$ và $G'$ (Chương III, § 3, no. 1), kết quả suy ra.

### 3. BAO ĐÓNG CỦA MỘT TẬP ĐỀU LIÊN TỤC

#### Mệnh đề 6 {#top-x-s2-prop-6 .statement}

Cho $X$ là một không gian tôpô (resp. không gian đều), cho $Y$ là một không gian đều và cho $H$ là một tập con của $\mathcal{F}(X; Y)$. Khi đó $H$ là đồng liên tục tại một điểm $x_0 \in X$ (resp. đồng liên tục đều) khi và chỉ khi bao đóng $\overline{H}$ của $H$ trong $\mathcal{F}_s(X; Y)$ là đồng liên tục tại $x_0$ (resp. đồng liên tục đều).

Điều kiện đó hiển nhiên là đủ. Để chứng minh rằng nó là cần thiết, xét một lân cận $V$ của $Y$ đóng trong $Y \times Y$; theo giả thiết, có một lân cận $U$ của $x_0$ trong $X$ (resp. một lân cận $M$ của $X$) sao cho quan hệ $x \in U$ (resp. $(x', x'') \in M$) suy ra $(h(x_0), h(x)) \in V$ [resp. $(h(x'), h(x'')) \in V$] với mọi $h \in H$. Vì $V$ đóng, các ánh xạ $h \in \mathcal{F}(X; Y)$ thỏa mãn quan hệ $(h(x_0), h(x)) \in V$ với mọi $x \in U$ [resp. quan hệ $(h(x'), h(x'')) \in V$ với mọi $(x', x'') \in M$] tạo thành một tập con đóng của $\mathcal{F}_s(X; Y)$ (\S 1, no. 2, Nhận xét 6); vì tập con đóng này chứa $H$, nó chứa $\overline{H}$. Do đó được kết quả, vì các lân cận đóng của $Y$ tạo thành một hệ cơ bản của các lân cận (Chương II, § 1, no. 2, Mệnh đề 2, Hệ quả 2).

### 4. HỘI TỤ ĐIỂM VÀ HỘI TỤ COMPACT TRÊN CÁC TẬP ĐỒNG LIÊN TỤ

#### Định lý 1 {#top-x-s2-thm-1 .statement}

Cho $X$ là một không gian tôpô (resp. không gian đều), cho $Y$ là một không gian đều và cho $H$ là một tập con đồng liên tục (resp. đồng liên tục đều) của $\mathcal{C}(X; Y)$. Khi đó các cấu trúc đều sau trên $H$ là như nhau: cấu trúc đều của hội tụ compact (resp. tiền compact), cấu trúc đều của hội tụ điểm và cấu trúc đều của hội tụ điểm trên một tập con trù mật $D$ của $X$.

Chỉ cần chứng minh rằng cấu trúc đều cuối cùng trên $H$ mịn hơn cấu trúc thứ nhất; nói cách khác, cho một lân cận $V$ của $Y$ và một tập con compact (resp. tiền compact) $A$ của $X$, tồn tại một lân cận $W$ của $Y$ và một tập con hữu hạn $F$ của $D$ sao cho quan hệ

$$
(2)\quad u \in H,\ v \in H\ \text{và}\ (u(x), v(x)) \in W\ \text{với mọi}\ x \in F
$$

suy ra

$$
(3)\quad (u(x),\ v(x)) \in V\ \text{với mọi}\ x \in A
$$

#### Hệ quả {#top-x-s2-n4-cor-1 .statement}

*Theo các giả thiết của Định lý 1, bao đóng $\overline{H}$ của $H$ trong $\mathcal{F}(X; Y)$ đối với tôpô hội tụ từng điểm cũng chính là bao đóng của $H$ trong $\mathcal{C}(X; Y)$ đối với tôpô hội tụ compact (tương ứng tiền compact).*

Vì tập $\overline{H}$ là đẳng liên tục (tương ứng đẳng liên tục đều) theo Mệnh đề 6 của no. 3, và do đó được chứa trong $\mathcal{C}(X; Y)$; kết quả suy ra ngay từ thực tế là, trên $\overline{H}$, hai tôpô đang xét là như nhau, nhờ Định lý 1.

### 5. CÁC TẬP COMPACT CỦA CÁC ÁNH XẠ LIÊN TỤC

#### Định lý 2 (Ascoli) {#top-x-s2-thm-2 .statement}

*Cho $X$ là một không gian tôpô (tương ứng không gian đều), cho $\mathcal{S}$ là một phủ của $X$, cho $Y$ là một không gian đều và $H$ là một tập các ánh xạ của $X$ vào $Y$ sao cho, với mỗi $A \in \mathcal{S}$ và mỗi $u \in H$, hạn chế của $u$ lên $A$ là liên tục (tương ứng liên tục đều). Khi đó, để $H$ là tiền compact đối với tính đều của hội tụ theo $\mathcal{S}$, thì trong mọi trường hợp là cần và cũng đủ nếu các tập $A \in \mathcal{S}$ là compact (tương ứng tiền compact) rằng các điều kiện sau phải được thỏa mãn:*

a) Với mỗi $A \in \mathcal{S}$, tập $H|A \subset \mathcal{F}(A; Y)$ gồm các hạn chế lên $A$ của các hàm thuộc $H$ là đẳng liên tục (tương ứng, đều đẳng liên tục).

b) Với mỗi $x \in X$, tập $H(x) \subset Y$ gồm các điểm $u(x)$ ($u \in H$) là tiền compact.

1) Trước hết, ta chứng minh rằng các điều kiện a) và b) là cần thiết. Ta biết (\S 1, no. 2, Nhận xét 6) rằng ánh xạ $u \to u(x)$ của $\mathcal{F}_{\mathcal{S}}(X; Y)$ vào $Y$ là liên tục đều; do đó, nếu $H$ là tiền compact thì $H(x)$ cũng vậy (Chương II, \S 4, no. 2, Mệnh đề 2), điều này chứng minh b). Để chứng minh a), xét một tập $A \in \mathcal{S}$, một điểm $x_0 \in A$ và một bao lân cận $V$ của $Y$; vì $H$ là tiền compact nên nó có thể được phủ bởi hữu hạn tập $W(A, V)$-nhỏ; nói cách khác, tồn tại một dãy hữu hạn $(u_i)$ gồm các phần tử của $H$ sao cho, với mỗi $u \in H$, ta có

$$
(u(x),\ u_i(x)) \in V \quad \text{với mọi } x \in A
$$

cho ít nhất một chỉ số $i$.

Vì mỗi $u_i|A$ đều liên tục tại $x_0$ (tương ứng, liên tục đều) nên tồn tại một lân cận $U_i$ của $x_0$ trong $A$ (tương ứng, một bao lân cận $M_i$ của $A$) sao cho

$$
x \in U_i \implies (u_i(x), u_i(x_0)) \in V,
$$

(tương ứng, sao cho

$$
(x', x'') \in M_i \implies (u_i(x'), u_i(x'')) \in V.)
$$

Gọi $U$ (tương ứng, $M$) là giao của các $U_i$ (tương ứng, các $M_i$); đó là một lân cận của $x_0$ trong $A$ (tương ứng, một bao lân cận của $A$). Với mỗi $u \in H$ có một chỉ số $i$ sao cho (4) đúng; viết điều kiện (4) cho $x_0$ và cho $x$ (tương ứng, cho $x'$ và $x''$) và xét thêm (5) [tương ứng, (6)], ta thấy ngay lập tức rằng quan hệ $x \in U$ [tương ứng, $(x', x'') \in M$] suy ra $(u(x),\ u(x_0)) \in \overset{\circ}{V}$ [tương ứng, $(u(x'),\ u(x'')) \in \overset{\circ}{V}$], với mỗi $u \in H$; và điều này thiết lập a).

2) Bây giờ ta chứng minh rằng các điều kiện a) và b) là đủ nếu các tập $A \in \mathcal{S}$ là compact (tương ứng, tiền compact). Điều kiện b) suy ra rằng $H$ là tiền compact đối với cấu trúc đều của hội tụ điểm (Chương II, \S 4, no. 2, Mệnh đề 3). Nhưng từ điều kiện a) và Định lý 1 của no. 4 suy ra rằng trên $H|A$, cấu trúc đều của hội tụ điểm trong $A$ trùng với cấu trúc đều của hội tụ đều trong $A$; do đó $H|A$ là tiền compact trong $\mathcal{F}_u(A; Y)$, điều này suy ra rằng $H$ là tiền compact đối với cấu trúc đều của $\mathcal{S}$-hội tụ (\S 1, no. 2).

Lưu ý rằng điều kiện b) của Định lý 2 tự động được thỏa mãn nếu $Y$ là một không gian tiền compact.

#### Hệ quả 1 {#top-x-s2-thm-2-cor-1 .statement}

Cho $X$ là một không gian tôpô (tương ứng, không gian đều), cho $Y$ là một không gian đều Hausdorff và cho $H$ là một tập con đều liên tục (tương ứng, đều liên tục đồng đều) của $C(X; Y)$. Giả sử rằng $H(x)$ là tương đối compact trong $Y$ với mỗi $x \in X$. Khi đó $H$ là tương đối compact trong $C(X; Y)$ đối với tôpô hội tụ compact (tương ứng, tiền compact).

Cho $\overline{H}$ là bao đóng của $H$ trong $\mathcal{F}_s(X; Y)$. $\overline{H}$ là đều liên tục (tương ứng, đều liên tục đồng đều) (no. 3, Mệnh đề 6). Hơn nữa, ta có $\overline{H}(x) \subset \overline{H(x)}$ (\S 1, no. 2, Nhận xét 6) và do đó $\overline{H}(x)$ cũng tương đối compact; suy ra Định lý 2 cho thấy rằng $\overline{H}$ là tiền compact đối với $\mathcal{S}$-hội tụ, trong đó $\mathcal{S}$ ký hiệu tập tất cả các tập con compact (tương ứng, tiền compact) của $X$. Hơn nữa, vì $\overline{H(x)}$ là compact, và do đó đầy đủ, nên $\overline{H}$ là đầy đủ đối với tính đều của hội tụ điểm (Chương II, \S 3, no. 5, Mệnh đề 10 và no. 4, Mệnh đề 8) và do đó cũng đối với tính đều của $\mathcal{S}$-hội tụ (\S 1, no. 5, Mệnh đề 5, Hệ quả 2); vì thế $\overline{H}$ là compact, vì nó tiền compact, đầy đủ và Hausdorff (\S 1, no. 2, Mệnh đề 1).

#### Hệ quả 2 {#top-x-s2-thm-2-cor-2 .statement}

Cho $X$ là một không gian tôpô (tương ứng, không gian đều), cho $Y$ là một không gian đều Hausdorff đầy đủ và cho $H$ là một tập con đều liên tục (tương ứng, đều liên tục đồng đều) của $C(X; Y)$. Giả sử rằng $H(x)$ là tương đối compact trong $Y$ với mọi $x \in D$, trong đó $D$ là một tập con trù mật của $X$. Khi đó $H$ là tương đối compact trong $C(X; Y)$ đối với tôpô hội tụ compact (tương ứng, tiền compact).

Chỉ cần chứng minh rằng $H(x)$ là tương đối compact với mọi $x \in X$, vì khi đó ta có thể áp dụng Hệ quả 1. Vì $Y$ đầy đủ, chỉ cần chứng minh rằng $H(x)$ là tiền compact với mọi $x \in X$. Bây giờ nếu $V$ là một lân cận đối xứng bất kỳ của $Y$, thì tồn tại một lân cận $U$ của $x$ sao cho $(u(x), u(x')) \in V$ với mọi $x' \in U$ và mọi $u \in H$. Theo giả thiết tồn tại $x' \in U \cap D$, và vì $H(x')$ tương đối compact trong $Y$, nên tồn tại một số hữu hạn các điểm $y_k \in Y$ sao cho $H(x')$ được chứa trong hợp của các tập $V(y_k)$; do đó $H(x)$ được chứa trong hợp của các tập $V(y_k)$, và chứng minh hoàn tất.

#### Hệ quả 3 {#top-x-s2-thm-2-cor-3 .statement}

Cho $X$ là một không gian địa phương compact, $Y$ là một không gian đều Hausdorff, $H$ là một tập hợp con của $C(X; Y)$. Khi đó $H$ là tương đối compact trong $C_c(X; Y)$ khi và chỉ khi $H$ đều liên tục và $H(x)$ tương đối compact trong $Y$ với mọi $x \in X$.

Xét theo Hệ quả 1, chỉ cần chứng minh rằng, nếu $H$ tương đối compact trong $C_c(X; Y)$, thì $H$ đều liên tục. Bây giờ mỗi điểm $x \in X$ có một lân cận compact $A$, và từ Định lý 2 suy ra rằng $H/A$ đều liên tục; điều này kéo theo rằng $H$ đều liên tục tại $x$, và kết quả được chứng minh.

#### Nhận xét {#top-x-s2-n5-rem-1 .statement}

Cho $X$ là một không gian tôpô, $Y$ là một không gian đều và $\mathcal{S}$ là một tập hợp các tập con của $X$. Khi đó trên mọi tập hợp con *tiền compact* $H$ của $\mathcal{F}_{\mathcal{S}}(X; Y)$, tính đều của sự hội tụ $\mathcal{S}$ trùng với tính đều của sự hội tụ từng điểm trong $B = \bigcup_{A \in \mathcal{S}} A$. Ta có thể rút gọn về trường hợp $B = X$ và $Y$ là Hausdorff và đầy đủ; vì nếu $j$ là đơn ánh chính tắc $B \to X$ và $i$ là ánh xạ chính tắc $Y \to \hat{Y}$, thì tính đều của sự hội tụ $\mathcal{S}$ trên $\mathcal{F}(X; Y)$ là ảnh ngược của tính đều của sự hội tụ $\mathcal{S}$ trên $\mathcal{F}(B; \hat{Y})$ qua ánh xạ $\theta : u \to i \circ u \circ j$ (\S 1, no. 4, Mệnh đề 4), và $H$ là tiền compact khi và chỉ khi $\theta(H)$ là như vậy (Chương II, \S 4, no. 2, Mệnh đề 3). Vì thế, nếu $B = X$ và $Y$ là Hausdorff và đầy đủ, $\mathcal{F}_{\mathcal{S}}(X; Y)$ là Hausdorff và đầy đủ (\S 1, no. 2, Mệnh đề 1 và no. 5, Định lý 1); do đó bao đóng $\overline{H}$ của $H$ trong không gian này là *compact*. Trên $\overline{H}$, tôpô hội tụ từng điểm là Hausdorff (\S 1, no. 2, Mệnh đề 1) và thô hơn tôpô của sự hội tụ $\mathcal{S}$; do đó hai tôpô này trùng nhau (Chương I, \S 9, no. 4, Định lý 2, Hệ quả 3) và do đó các tính đều của sự hội tụ $\mathcal{S}$ và sự hội tụ từng điểm cũng trùng nhau (Chương II, \S 4, no. 1, Định lý 1).

### Bài tập {#top-x-s2-exercises}

Xem [các bài tập cho § 2](exercises/s2/).
