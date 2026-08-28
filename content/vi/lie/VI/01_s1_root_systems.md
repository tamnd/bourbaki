---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: VI
chapter_title: ROOT SYSTEMS
section: 1
section_title: Root systems
lang: vi
source: lie-iv-vi
pdf_pages: 0168-0198, 0248-0253
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF A ROOT SYSTEM
      page: 0
      pdf_page: 168
    - "no": 2
      title: DIRECT SUM OF ROOT SYSTEMS
      page: 0
      pdf_page: 172
    - "no": 3
      title: RELATION BETWEEN TWO ROOTS
      page: 0
      pdf_page: 173
    - "no": 4
      title: REDUCED ROOT SYSTEMS
      page: 0
      pdf_page: 177
    - "no": 5
      title: CHAMBERS AND BASES OF ROOT SYSTEMS
      page: 0
      pdf_page: 178
    - "no": 6
      title: POSITIVE ROOTS
      page: 0
      pdf_page: 181
    - "no": 7
      title: CLOSED SETS OF ROOTS
      page: 0
      pdf_page: 186
    - "no": 8
      title: HIGHEST ROOT
      page: 0
      pdf_page: 191
    - "no": 9
      title: WEIGHTS, RADICAL WEIGHTS
      page: 0
      pdf_page: 192
    - "no": 10
      title: FUNDAMENTAL WEIGHTS, DOMINANT WEIGHTS
      page: 0
      pdf_page: 193
    - "no": 11
      title: COXETER TRANSFORMATION
      page: 0
      pdf_page: 195
    - "no": 12
      title: CANONICAL BILINEAR FORM
      page: 0
      pdf_page: 197
statements: 79
exercises: 24
content_sha256: ee5ffad14726cfe539e95b9a51c53d83d508ac694a4ddad4e23c02fd493dea9e
translated_from: content/en/lie/VI/01_s1_root_systems.md
source_content_sha256: 63306735a7f6d780a7b9820aded9cbd9eaac6a612cf204aee1470da429e156f4
translation_model: gpt-5-6-mini, gpt-5-6, gpt-5-mini
translation_run: translate-vi-078c10e9
glossary_version: 34
glossary_terms_sha256: 0457923eb54a37f952d0a721ce7180681ff6288d847e254d76e01d0cae691dd3
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 1. HỆ NGHIỆM

Trong đoạn này, $k$ ký hiệu một trường có đặc số không. Từ no. 3 trở đi, ta giả sử rằng $k = \mathbf{R}$.

### 1. ĐỊNH NGHĨA CỦA MỘT HỆ NGHIỆM

#### Bổ đề 1 {#lie-vi-s1-lem-1 .statement}

Cho $V$ là một không gian vectơ trên $k$, $R$ là một tập con hữu hạn của $V$ sinh ra $V$. Với mọi $\alpha \in R$ sao cho $\alpha \neq 0$, tồn tại nhiều nhất một phép phản xạ $s$ của $V$ sao cho $s(\alpha) = -\alpha$ và $s(R) = R$.

Cho $G$ là nhóm các tự đẳng cấu của $V$ giữ $R$ ổn định. Vì $R$ sinh ra $V$, $G$ đẳng cấu với một nhóm con của nhóm đối xứng của $R$, và do đó là hữu hạn. Cho $s, s'$ là các phép phản xạ của $V$ sao cho $s(\alpha) = s'(\alpha) = -\alpha$, $s(R) = R$, $s'(R) = R$. Khi đó $t = ss'$ thuộc $G$, và do đó có cấp hữu hạn $m$. Mặt khác,

$$
t(\alpha) = \alpha \quad \text{và} \quad t(x) \equiv x \mod. k\alpha \quad \text{với mọi } x \in V.
$$

Suy ra tồn tại một dạng tuyến tính $f$ trên $V$ sao cho

$$
t(x) = x + f(x)\alpha \quad \text{với mọi } x \in V
$$

và $f(\alpha) = 0$. Theo quy nạp trên $n$, suy ra rằng

$$
t^n(x) = x + nf(x)\alpha \text{ với mọi } x \in V.
$$

Lấy $n$ bằng $m$, ta thấy rằng $mf(x) = 0$ với mọi $x \in V$, do đó $f = 0$, $t = 1$ và $s = s'$.

#### Định nghĩa 1 {#lie-vi-s1-def-1 .statement}

Cho $V$ là một không gian vectơ trên $k$, và $R$ là một tập con của $V$. Khi đó $R$ được gọi là một hệ nghiệm trong $V$ nếu các điều kiện sau được thỏa mãn:

(RS_I) $R$ là hữu hạn, không chứa 0, và sinh ra $V$.
(RS_{II}) Với mọi $\alpha \in R$, tồn tại một phần tử $\alpha^\vee$ của đối ngẫu $V^*$ của $V$ sao cho $\langle \alpha, \alpha^\vee \rangle = 2$ và phép phản xạ $s_{\alpha, \alpha^\vee}$ (xem Chương V, § 2) giữ $R$ ổn định.

(RS_{\text{III}}) Với mọi $\alpha \in \mathbf{R}$, $\alpha^{\sim}(R) \subseteq \mathbf{Z}$.

Theo Bổ đề 1, phép đối xứng $s_{\alpha,\alpha^{\sim}}$ (và do đó cả dạng tuyến tính $\alpha^{\sim}$) được xác định duy nhất bởi $\alpha$, nên (RS_{\text{III}}) có nghĩa. Ta đặt $s_{\alpha,\alpha^{\sim}} = s_{\alpha}$. Khi đó $s_{\alpha}(x) = x - \langle \alpha^{\sim}, x \rangle \alpha$ với mọi $x \in V$.

Các phần tử của R được gọi là các nghiệm (của hệ đang xét). Chiều của V được gọi là hạng của hệ.

Các tự đẳng cấu của V giữ R ổn định được gọi là các tự đẳng cấu của R. Chúng tạo thành một nhóm hữu hạn ký hiệu là A(R). Nhóm con của A(R) sinh bởi các $s_{\alpha}$ được gọi là nhóm Weyl của R và được ký hiệu bởi W(R), hoặc đơn giản là W.

#### Nhận xét 1 {#lie-vi-s1-n1-rem-1 .statement}

Cho $k'$ là một mở rộng của $k$. Đồng nhất một cách chính tắc V với một tập con của $V \otimes k'$ và $V^*$ với một tập con của $V^* \otimes k' = (V \otimes k')^*$. Khi đó, R là một hệ nghiệm trong $V \otimes k'$, và các $\alpha^{\sim}$ cũng giống như trước.

#### Bổ đề 2 {#lie-vi-s1-lem-2 .statement}

Cho R là một hệ nghiệm trong V. Cho $(x|y)$ là một dạng song tuyến tính đối xứng trên V, không suy biến và bất biến dưới W(R). Đồng nhất V với $V^*$ nhờ dạng này. Nếu $\alpha \in R$, thì $\alpha$ là không đẳng hướng và

$$
\alpha^{\sim} = \frac{2\alpha}{(\alpha|\alpha)}.
$$

Điều này suy ra từ công thức (4) của Chương V, § 2, no. 3.

#### Mệnh đề 1 {#lie-vi-s1-prop-1 .statement}

Cho $V_Q$ (tương ứng $V_Q^*$) là không gian con Q-vectơ của V (tương ứng $V^*$) sinh bởi các $\alpha$ (tương ứng các $\alpha^{\sim}$). Khi đó $V_Q$ (tương ứng $V_Q^*$) là một cấu trúc Q trên V (tương ứng $V^*$) (Đại số, Chương II, § 8, no. 1). Hạn chế của dạng song tuyến tính chính tắc trên $V_Q \times V_Q^*$ của $V \times V^*$ cho một sự đồng nhất mỗi không gian $V_Q, V_Q^*$ với đối ngẫu của không gian kia. Tập hợp R là một hệ nghiệm trong $V_Q$.

Nếu $k = \mathbf{R}$, tồn tại một tích vô hướng trên V bất biến dưới tác dụng của W(R) (Integration, Chap. VII, § 3, no. 1, Prop. 1); Bổ đề 2 chỉ ra rằng các $\alpha^{\sim}$ sinh $V^*$. Theo Nhận xét 1, các $\alpha^{\sim}$ lại sinh $V^*$ nếu $k = \mathbf{Q}$. Bây giờ ta xét trường hợp tổng quát. Đặt E = $V_Q$. Theo (RS_{\text{III}}), mỗi $\alpha^{\sim}$ ánh xạ E vào $\mathbf{Q}$, và do đó xác định một phần tử $\tilde{\alpha}$ của $E^*$. Điều này là ngay lập tức rằng R là một hệ nghiệm trong E, và rằng phần tử tương ứng với $\alpha$ trong $E^*$ là $\tilde{\alpha}$. Theo điều đã nói ở trên, các $\tilde{\alpha}$ sinh không gian vectơ $E^*$. Xét đồng cấu chính tắc $i : E \otimes_Q k \to V$, và chuyển vị của nó $^t i : V^* \to E^* \otimes_Q k$. Vì R sinh V, $^t i$ là đơn ánh; nhưng ảnh của $^t i$ chứa các $\tilde{\alpha}$, nên $^t i$ là toàn ánh. Từ đó ta kết luận cuối cùng rằng i và $^t i$ là các đẳng cấu. Do đó ta có thể đồng nhất V với $E \otimes k$, $V^*$ với $E^* \otimes k$, $\alpha^{\sim}$ với $\tilde{\alpha}$, và $V_Q^*$ với $E^*$. Như vậy, $V_Q$ (resp. $V_Q^*$) là một cấu trúc Q trên V (resp. $V^*$). Hạn chế xuống $V_Q \times V_Q^*$ của dạng song tuyến tính chính tắc trên $V \times V^*$ có thể được đồng nhất với dạng song tuyến tính chính tắc trên $E \times E^*$, do đó ta có mệnh đề.

#### Nhận xét 2 {#lie-vi-s1-n1-rem-2 .statement}

Mệnh đề 1 quy việc nghiên cứu các hệ nghiệm về trường hợp $k = \mathbf{Q}$. Nhận xét 1 quy tiếp nó về việc nghiên cứu các hệ nghiệm trong không gian vectơ thực $V_{\mathbf{R}} = V_{\mathbf{Q}} \otimes_{\mathbf{Q}} \mathbf{R}$. Các nhóm Weyl liên kết với các hệ khác nhau này được đồng nhất một cách chính tắc.

#### Nhận xét 3 {#lie-vi-s1-n1-rem-3 .statement}

Vì các $\alpha \tilde{}$ sinh $V^*$, nhóm $W(R)$, được xem như một nhóm con của $\mathbf{GL}(V_{\mathbf{R}})$, là cốt yếu (Chap. V, § 3, no. 7). Hơn nữa, Hệ quả của Định lý 1 của Chap. V, § 3, no. 2 chỉ ra rằng các phép phản xạ duy nhất thuộc $W(R)$ là các $s_{\alpha}$.

#### Mệnh đề 2 {#lie-vi-s1-prop-2 .statement}

*Các $\alpha \tilde{}$ tạo thành một hệ nghiệm trong $V^*$, và $\alpha \tilde{} = \alpha$ với mọi $\alpha \in R$.*

Các $\alpha \tilde{}$ thỏa mãn (RS_I) theo Mệnh đề 1. Vì $s_{\alpha, \alpha \tilde{}}$ là một tự đẳng cấu của không gian vectơ $V$ được trang bị tập con $R$, ${}^t(s_{\alpha, \alpha \tilde{}})^{-1}$ giữ ổn định tập hợp $R \tilde{}$ của các $\alpha \tilde{}$; nhưng ${}^t(s_{\alpha, \alpha \tilde{}})^{-1} = s_{\alpha \tilde{}, \alpha}$, điều này chứng minh rằng $R \tilde{}$ thỏa mãn (RS_{II}) và rằng $\alpha \tilde{} = \alpha$. Cuối cùng, $\langle \alpha \tilde{}, \beta \rangle \in \mathbf{Z}$ với mọi $\alpha \tilde{} \in R \tilde{}$ và $\beta \in R$, do đó $R \tilde{}$ thỏa mãn (RS_{III}).

Tập hợp $R \tilde{}$ được gọi là *hệ nghiệm nghịch đảo của* $R$. Ánh xạ $\alpha \mapsto \alpha \tilde{}$ là một song ánh từ $R$ đến $R \tilde{}$, được gọi là *song ánh chính tắc từ* $R$ *đến* $R \tilde{}$. Chú ý rằng, nếu $\alpha, \beta$ là các phần tử của $R$ sao cho $\alpha + \beta \in R$, thì nói chung $(\alpha + \beta) \tilde{} \neq \alpha \tilde{} + \beta \tilde{}$.

Vì $s_{\alpha}(\alpha) = -\alpha$, tiên đề (RS_{II}) cho thấy rằng $-R = R$. Hiển nhiên $(-\alpha) \tilde{} = -\alpha \tilde{}$ và $-1 \in A(R)$ (nhưng không phải lúc nào cũng đúng rằng $-1 \in W(R)$).

Đẳng thức ${}^t(s_{\alpha, \alpha \tilde{}})^{-1} = s_{\alpha \tilde{}, \alpha}$ cho thấy rằng ánh xạ $u \mapsto {}^t u^{-1}$ là một đẳng cấu từ nhóm $W(R)$ đến nhóm $W(R \tilde{})$. Ta đồng nhất hai nhóm này bằng đẳng cấu này; nói cách khác, ta xét $W(R)$ như tác động đồng thời trong $V$ và trong $V^*$. Tương tự đối với $A(R)$.

#### Mệnh đề 3 {#lie-vi-s1-prop-3 .statement}

*Với $x, y \in V$, đặt*
$$
(x|y) = \sum_{\alpha \in R} \langle \alpha \tilde{}, x \rangle \langle \alpha \tilde{}, y \rangle.
$$
*Khi đó* $(x|y)$ *là một dạng song tuyến tính đối xứng không suy biến trên* $V$, *bất biến dưới tác động của* $A(R)$. *Với* $x, y \in V_{\mathbf{Q}}$ *ta có* $(x|y) \in \mathbf{Q}$. *Mở rộng chính tắc của* $(x|y)$ *đến*
$$
V_{\mathbf{R}} = V_{\mathbf{Q}} \otimes_{\mathbf{Q}} \mathbf{R}
$$
*là không suy biến và dương*.

Hiển nhiên $(x|y)$ là một dạng song tuyến tính đối xứng trên $V$. Nếu $g \in A(R)$,
$$
(g(x)|g(y)) = \sum_{\alpha \in R} \langle {}^t g(\alpha \tilde{}), x \rangle \langle {}^t g(\alpha \tilde{}), y \rangle = (x|y)
$$
vì ${}^t g)(R \tilde{}) = R \tilde{}$. Nếu $x, y \in V_{\mathbf{Q}}$, thì $(x|y) \in \mathbf{Q}$ theo (RS_{III}). Nếu $z \in V_{\mathbf{R}}$, thì $(z|z) = \sum_{\alpha \in R} \langle \alpha \tilde{}, z \rangle^2 \geq 0$, và $(z|z) > 0$ nếu $z \neq 0$ theo Mệnh đề 1, do đó mở rộng chính tắc của $(x|y)$ lên $V_{\mathbf{R}}$ là dương và không suy biến. Hạn chế của $(x|y)$ trên $V_{\mathbf{Q}}$ do đó là không suy biến, và vì thế dạng $(x|y)$ trên $V$ là không suy biến.

#### Mệnh đề 4 {#lie-vi-s1-prop-4 .statement}

(i) *Cho $X$ là một tập con của $\mathbf{R}$, cho $V_X$ là không gian con vectơ của $V$ sinh bởi $X$, và cho $V'_X$ là không gian con vectơ của $V^*$ sinh bởi các $\alpha^-$, với $\alpha \in X$. Khi đó $V$ là tổng trực tiếp của $V_X$ và phần bù trực giao của $V'_X$; $V^*$ là tổng trực tiếp của $V'_X$ và phần bù trực giao của $V_X$, và $V'_X$ được đồng nhất với đối ngẫu của $V_X$.

(ii) $R \cap V_X$ là một hệ nghiệm trong $V_X$, và song ánh chính tắc từ $R \cap V_X$ đến hệ nghiệm nghịch đảo của nó được đồng nhất với hạn chế của ánh xạ $\alpha \mapsto \alpha^-$ trên $R \cap V_X$.

Theo *Nhận xét 2*, ta có thể giả sử rằng $k = \mathbf{R}$. Đồng nhất $V$ với $V^*$ bằng dạng song tuyến tính đối xứng của Mệnh đề 3. Ta có $\alpha^- = \frac{2\alpha}{(\alpha|\alpha)}$ với mọi $\alpha \in R$ (Bổ đề 2). Mọi không gian con vectơ của $V$ đều không đẳng hướng, và mệnh đề bây giờ là hiển nhiên.

#### Hệ quả {#lie-vi-s1-n1-cor-1 .statement}

*Cho $V_1$ là một không gian con vectơ của $V$, và cho $V_2$ là không gian con vectơ sinh bởi $R \cap V_1$. Khi đó $R \cap V_1$ là một hệ nghiệm trong $V_2$.

Điều này suy ra từ (ii) áp dụng cho $X = R \cap V_1$.

Với $\alpha, \beta \in R$, đặt
$$
\langle \alpha, \beta^- \rangle = n(\alpha, \beta).
$$
(1)

Khi đó
$$
n(\alpha, \alpha) = 2
$$
(2)
$$
n(-\alpha, \beta) = n(\alpha, -\beta) = -n(\alpha, \beta).
$$
(3)

Theo (RSIII),
$$
n(\alpha, \beta) \in \mathbf{Z}.
$$
(4)

Theo định nghĩa của $n(\alpha, \beta)$,
$$
s_\beta(\alpha) = \alpha - n(\alpha, \beta)\beta.
$$
(5)

Công thức (1) và Mệnh đề 2 suy ra rằng
$$
n(\alpha, \beta) = n(\beta^-, \alpha^-).
$$
(6)

Cho $(x|y)$ là một dạng song tuyến tính đối xứng trên $V$, không suy biến và bất biến dưới $W(R)$ (Mệnh đề 3). Theo Bổ đề 2,
$$
n(\alpha, \beta) = \frac{2(\alpha|\beta)}{(\beta|\beta)}.
$$
(7)

Suy ra rằng
$$
n(\alpha, \beta) = 0 \iff n(\beta, \alpha) = 0 \iff (\alpha|\beta) = 0 \iff s_\alpha \text{ và } s_\beta \text{ giao hoán.}
$$
(8)

Nếu $(\alpha|\beta) \neq 0$, thì
$$
\frac{n(\beta, \alpha)}{n(\alpha, \beta)} = \frac{(\beta|\beta)}{(\alpha|\alpha)}.
$$
(9)

### 2. TỔNG TRỰC TIẾP CỦA CÁC HỆ NGHIỆM

Cho V là một không gian vectơ trên $k$ là tổng trực tiếp của một họ $(V_i)_{1 \leq i \leq r}$ các không gian vectơ. Đồng nhất $V^*$ với tổng trực tiếp của các $V_i^*$. Với mọi $i$, cho $R_i$ là một hệ nghiệm trong $V_i$. Khi đó $R = \bigcup_i R_i$ là một hệ nghiệm trong V có hệ ngược là $R^- = \bigcup_i R_i^-$; song ánh chính tắc từ R đến $R^-$ mở rộng, với mọi $i$, song ánh chính tắc từ $R_i$ đến $R_i^-$. Tập hợp R được gọi là *tổng trực tiếp của các hệ nghiệm* $R_i$. Cho $\alpha \in R_i$. Nếu $j \neq i$, hạt nhân của $\alpha^-$ chứa $V_j$, do đó $s_\alpha$ cảm sinh ánh xạ đồng nhất trên $V_j$; mặt khác, $k\alpha \subseteq V_i$, nên $s_\alpha$ giữ $V_i$ ổn định. Các nhận xét này chỉ ra rằng $W(R)$ *có thể được đồng nhất với* $\prod_{i=1}^r W(R_i)$.

Một hệ nghiệm R được gọi là *bất khả quy* nếu $R \neq \varnothing$ và nếu R không là tổng trực tiếp của hai hệ nghiệm khác rỗng.

#### Mệnh đề 5 {#lie-vi-s1-prop-5 .statement}

*Cho V là một không gian vectơ trên k là tổng trực tiếp của các không gian vectơ* $V_1, \ldots, V_r$. *Cho R là một hệ nghiệm trong V. Đặt* $R_i = R \cap V_i$. *Ba điều kiện sau là tương đương*:

(i) *các* $V_i$ *ổn định dưới* $W(R)$;
(ii) $R \subseteq V_1 \cup V_2 \cup \cdots \cup V_r$;
(iii) *với mọi* $i$, $R_i$ *là một hệ nghiệm trong* $V_i$, *và R là tổng trực tiếp của các* $R_i$.
(iii) $\Longrightarrow$ (i): điều này suy ra từ điều đã nói ở đầu số này.

(i) $\Longrightarrow$ (ii): giả sử rằng các $V_i$ ổn định dưới $W(R)$. Cho $\alpha \in R$ và cho H là hạt nhân của $\alpha^-$. Theo Mệnh đề 3 của Chương V, § 2, no. 2, mỗi $V_i$ là tổng của một không gian con của H và một không gian con của $k\alpha$. Do đó một trong các $V_i$ chứa $k\alpha$, vậy $\alpha \in V_1 \cup V_2 \cup \cdots \cup V_r$.

(ii) $\Longrightarrow$ (iii): nếu điều kiện (ii) được thỏa mãn, $R_i$ sinh ra $V_i$ với mọi $i$, do đó $R_i$ là một hệ nghiệm trong $V_i$ (Mệnh đề 4). Rõ ràng rằng R là tổng trực tiếp của các $R_i$.

#### Hệ quả {#lie-vi-s1-n2-cor-1 .statement}

*Cho R là một hệ nghiệm trong V. Các điều kiện sau là tương đương*:
(i) *R là bất khả quy*;
(ii) *V là* $W(R)$*-môđun đơn*;
(iii) *V là* $W(R)$*-môđun đơn tuyệt đối*.
(ii) $\Longleftrightarrow$ (i): điều này suy ra từ Mệnh đề 5 và Định lý Maschke (Chương V, Phụ lục, Mệnh đề 2).
(iii) $\Longleftrightarrow$ (ii): điều này suy ra từ Mệnh đề 1 của Chương V, § 2, no. 1.

#### Mệnh đề 6 {#lie-vi-s1-prop-6 .statement}

*Mọi hệ nghiệm* R *trong* V *là tổng trực tiếp của một họ* $(R_i)_{i \in I}$ *các hệ nghiệm bất khả quy và duy nhất sai khác một song ánh của tập chỉ số*.

Sự tồn tại của các $R_i$ được chứng minh bằng quy nạp theo Card R: nếu R không rỗng và không bất khả quy, R là tổng trực tiếp của hai hệ nghiệm $R', R''$ sao cho Card $R' <$ Card $R$, Card $R'' <$ Card $R$, và giả thiết quy nạp áp dụng cho $R'$ và $R''$. Để chứng minh tính duy nhất, chỉ cần chứng minh rằng, nếu $R$ là tổng trực tiếp của $R'$ và $R''$, mọi $R_i$ nhất thiết được chứa trong $R'$ hoặc trong $R''$. Cho $V', V'', V'_i, V''_i$ là các không gian con vectơ của $V$ được sinh bởi $R', R'', R' \cap R_i, R'' \cap R_i$. Vì tổng $V' + V''$ là trực tiếp, tổng $V'_i + V''_i$ là trực tiếp. Vì $R_i \subseteq R' \cup R''$, $R_i$ là tổng trực tiếp của các hệ nghiệm $R' \cap R_i$ và $R'' \cap R_i$; do đó hoặc $R' \cap R_i = \varnothing$ hoặc $R'' \cap R_i = \varnothing$, điều này chứng minh mệnh đề.

Các $R_i$ được gọi là *các thành phần bất khả quy* của $R$. Với mọi vô hướng khác không $\lambda_i$, hợp của các $\lambda_i R_i$ là một hệ nghiệm trong $V$, có hệ ngược là hợp của các $\lambda_i^{-1} R_i$, và có nhóm Weyl là $W(R)$.

#### Mệnh đề 7 {#lie-vi-s1-prop-7 .statement}

*Cho $R$ là một hệ nghiệm trong $V$, $(R_i)$ là họ các thành phần bất khả quy của nó, $V_i$ là không gian con vectơ của $V$ được sinh bởi $R_i$, $B$ là dạng song tuyến tính đối xứng bất biến trên $V$ được xác định trong Mệnh đề 3, và $B'$ là một dạng song tuyến tính đối xứng trên $V$ bất biến dưới tác động của $W(R)$. Khi đó các $V_i$ trực giao từng đôi một đối với $B'$, và, với mọi $i$, các hạn chế của $B$ và $B'$ lên $V_i$ tỉ lệ với nhau.*

Nếu $v_i \in V_i, v_j \in V_j, i \neq j$, và nếu $w \in W(R_j)$, thì
$$
B'(v_i, w(v_j)) = B'(v_i, v_j),
$$
điều này cho thấy rằng $w(v_j) - v_j$ trực giao với $v_i$ đối với $B'$. Vì $V_j$ là bất khả quy đối với $W(R_j)$, nó được sinh bởi các $w(v_j) - v_j$, và do đó nó trực giao với $V_i$.

Sự kiện rằng các hạn chế của $B$ và $B'$ lên mỗi $V_i$ là tỉ lệ với nhau suy ra từ Mệnh đề 1 của Chương V, § 2, no. 1.

#### Nhận xét {#lie-vi-s1-n2-rem-1 .statement}

Chọn một tích vô hướng trên $V_R$ bất biến dưới $W(R)$. Khi đó có thể nói về *độ dài* của một nghiệm và *góc* giữa hai nghiệm. Mệnh đề 7 cho thấy rằng góc này độc lập với lựa chọn tích vô hướng, cũng như tỉ số độ dài của hai nghiệm, với điều kiện chúng thuộc cùng một *thành phần* bất khả quy của $R$.

### 3. QUAN HỆ GIỮA HAI NGHIỆM

Nhắc lại rằng *từ nay về sau ta giả sử rằng* $k = \mathbf{R}$. (Ta để cho độc giả nhiệm vụ mở rộng các định nghĩa và kết quả sang trường hợp tổng quát, bằng cách sử dụng phương pháp được chỉ ra trong *Nhận xét 2* của no. 1.)

*Trong toàn bộ phần sau, $R$ ký hiệu một hệ nghiệm trong một không gian vectơ $V$; và $V$ được trang bị một tích vô hướng $(x, y) \mapsto (x|y)$ bất biến dưới $W(R)$, cf. Mệnh đề 3.*

Cho $\alpha, \beta \in R$. Theo công thức (7) của no. 1,
$$
n(\alpha, \beta)n(\beta, \alpha) = 4 \cos^2 (\widehat{\alpha, \beta}) \leq 4.
$$

Do đó, số nguyên $n(\alpha, \beta)n(\beta, \alpha)$ phải nhận một trong các giá trị 0, 1, 2, 3, 4. Theo Chương V, § 2, no. 5, Hệ quả của Mệnh đề 6, và chú thích cuối trang ở trang của Chương V, § 4, no. 8, ta thấy rằng các khả năng duy nhất là sau đây, sai khác bởi đổi chỗ $\alpha$ và $\beta$:

1) $n(\alpha, \beta) = n(\beta, \alpha) = 0;$
   $$
   (\overline{\alpha, \beta}) = \frac{\pi}{2}; \quad s_{\alpha}s_{\beta} \text{ có cấp } 2;
   $$
2) $n(\alpha, \beta) = n(\beta, \alpha) = 1;$
   $$
   (\overline{\alpha, \beta}) = \frac{\pi}{3}; \quad s_{\alpha}s_{\beta} \text{ có cấp } 3;
   $$
   $$
   \| \alpha \| = \| \beta \|;
   $$
3) $n(\alpha, \beta) = n(\beta, \alpha) = -1;$
   $$
   (\overline{\alpha, \beta}) = \frac{2\pi}{3}; \quad s_{\alpha}s_{\beta} \text{ có cấp } 3;
   $$
   $$
   \| \alpha \| = \| \beta \|;
   $$
4) $n(\alpha, \beta) = 1,\ n(\beta, \alpha) = 2;$
   $$
   (\overline{\alpha, \beta}) = \frac{\pi}{4}; \quad s_{\alpha}s_{\beta} \text{ có cấp } 4;
   $$
   $$
   \| \beta \| = \sqrt{2}\ \| \alpha \|;
   $$
5) $n(\alpha, \beta) = -1,\ n(\beta, \alpha) = -2;$
   $$
   (\overline{\alpha, \beta}) = \frac{3\pi}{4}; \quad s_{\alpha}s_{\beta} \text{ có cấp } 4;
   $$
   $$
   \| \beta \| = \sqrt{2}\ \| \alpha \|;
   $$
6) $n(\alpha, \beta) = 1,\ n(\beta, \alpha) = 3;$
   $$
   (\overline{\alpha, \beta}) = \frac{\pi}{6}; \quad s_{\alpha}s_{\beta} \text{ có cấp } 6;
   $$
   $$
   \| \beta \| = \sqrt{3}\ \| \alpha \|;
   $$
7) $n(\alpha, \beta) = -1,\ n(\beta, \alpha) = -3;$
   $$
   (\overline{\alpha, \beta}) = \frac{5\pi}{6}; \quad s_{\alpha}s_{\beta} \text{ có cấp } 6;
   $$
   $$
   \| \beta \| = \sqrt{3}\ \| \alpha \|;
   $$
8) $n(\alpha, \beta) = n(\beta, \alpha) = 2;$
   $$
   \alpha = \beta;
   $$
9) $n(\alpha, \beta) = n(\beta, \alpha) = -2;$
   $$
   \alpha = -\beta;
   $$
10) $n(\alpha, \beta) = 1,\ n(\beta, \alpha) = 4;$
    $$
    \beta = 2\alpha;
    $$
11) $n(\alpha, \beta) = -1,\ n(\beta, \alpha) = -4;$
    $$
    \beta = -2\alpha.
    $$

Đặc biệt:

#### Mệnh đề 8 {#lie-vi-s1-prop-8 .statement}

(i) *Nếu hai nghiệm tỉ lệ với nhau, nhân tử tỉ lệ chỉ có thể là $\pm 1, \pm \frac{1}{2}, \pm 2$.*

(ii) *Nếu $\alpha$ và $\beta$ là hai nghiệm không tỉ lệ, và nếu $\| \alpha \| \leq \| \beta \|$, thì $n(\alpha, \beta)$ nhận một trong các giá trị 0, 1, -1.*

Nếu một nghiệm $\alpha \in \mathbf{R}$ sao cho $\frac{1}{2}\alpha \notin \mathbf{R}$, thì $\alpha$ được gọi là một nghiệm *không thể phân chia*.

#### Định lý 1 {#lie-vi-s1-thm-1 .statement}

*Cho $\alpha, \beta$ là hai nghiệm.*

(i) *Nếu $n(\alpha, \beta) > 0$, $\alpha - \beta$ là một nghiệm trừ khi $\alpha = \beta$.*
(ii) *Nếu $n(\alpha, \beta) < 0$, $\alpha + \beta$ là một nghiệm trừ khi $\alpha = -\beta$.*

Nếu $n(\alpha, \beta) > 0$, các khả năng, theo danh sách ở trên, là các khả năng sau:

1) $n(\alpha, \beta) = 1$; khi đó $\alpha - \beta - s_{\beta}(\alpha) \in \mathbf{R}$;
2) $n(\beta, \alpha) = 1$; khi đó $\beta - \alpha = s_{\alpha}(\beta) \in \mathbf{R}$, do đó $\alpha - \beta \in \mathbf{R}$;
3) $\beta = \alpha$.

Điều này chứng minh (i), và (ii) suy ra bằng cách thay $\beta$ bởi $-\beta$.

#### Hệ quả {#lie-vi-s1-n3-cor-1 .statement}

Cho $\alpha$ và $\beta$ là hai nghiệm.

(i) *Nếu* $(\alpha|\beta) > 0$, $\alpha - \beta$ là một nghiệm trừ khi $\alpha = \beta$.
(ii) *Nếu* $(\alpha|\beta) < 0$, $\alpha + \beta$ là một nghiệm trừ khi $\alpha = -\beta$.
(iii) *Nếu* $\alpha - \beta \notin \mathbf{R} \cup \{0\}$ và $\alpha + \beta \notin \mathbf{R} \cup \{0\}$, *thì* $(\alpha|\beta) = 0$.

Các mệnh đề (i) và (ii) suy ra từ Đ.lý 1 và công thức (7) của no. 1. Mệnh đề (iii) suy ra từ (i) và (ii).

Có thể xảy ra $\alpha + \beta \in \mathbf{R}$, $(\alpha|\beta) = 0$ (xem Plate X, Hệ B_2). Khi $\alpha - \beta \notin \mathbf{R} \cup \{0\}$ và $\alpha + \beta \notin \mathbf{R} \cup \{0\}$, $\alpha$ và $\beta$ được gọi là *trực giao mạnh*.

#### Mệnh đề 9 {#lie-vi-s1-prop-9 .statement}

Cho $\alpha$ và $\beta$ là hai nghiệm không tỷ lệ.

(i) *Tập hợp* I *của các số nguyên* j *sao cho* $\beta + j\alpha$ *là một nghiệm là một khoảng* $[ -q, p ]$ *trong* $\mathbf{Z}$ *chứa* 0.
(ii) *Cho* S *là tập hợp của* $\beta + j\alpha$ *với* $j \in \mathrm{I}$. *Khi đó*,
$$
s_{\alpha}(S) = S \quad \text{và} \quad s_{\alpha}(\beta + p\alpha) = \beta - q\alpha.
$$
(iii) $p - q = -n(\beta, \alpha)$.

Rõ ràng, $0 \in \mathrm{I}$. Gọi $p$ (tương ứng $-q$) là phần tử lớn nhất (tương ứng nhỏ nhất) của I. Nếu không phải tất cả các số nguyên trong $[ -q, p ]$ đều thuộc I, tồn tại hai số nguyên $r, s$ trong $[ -q, p ]$ có các tính chất sau: $s > r + 1, s \in \mathrm{I}, r \in \mathrm{I}, r + k \notin \mathrm{I}$ với $1 \leq k \leq s - r - 1$. Với ký hiệu của Hệ quả của Đ.lý 1, $(\alpha|\beta + s\alpha) \leq 0, (\alpha|\beta + r\alpha) \geq 0$, điều này là vô lý vì
$$
(\alpha|\beta + s\alpha) \leq 0 > (\alpha|\beta + r\alpha).
$$
Điều này chứng minh (i).

Ta có $s_{\alpha}(\beta + j\alpha) = \beta - n(\beta, \alpha)\alpha - j\alpha = \beta + j'\alpha$ với $j' = -j - n(\beta, \alpha)$. Do đó $s_{\alpha}(S) \subseteq S$ và hệ quả là $s_{\alpha}(S) = S$. Bây giờ $j \mapsto -j - n(\beta, \alpha)$ là một song ánh giảm từ I vào I. Suy ra rằng, $j' = -q$ khi $j = p$, do đó $-q = -p - n(\beta, \alpha)$. Điều này chứng minh (ii) và (iii).

Tập hợp S được gọi là chuỗi nghiệm $\alpha$ xác định bởi $\beta$, $\beta - q\alpha$ là gốc của nó, $\beta + p\alpha$ là đầu của nó, và $p + q$ là độ dài của nó.

#### Hệ quả {#lie-vi-s1-n3-cor-2 .statement}

Cho S là một chuỗi nghiệm $\alpha$, và $\gamma$ là gốc của S. Độ dài của S là $-n(\gamma, \alpha)$; nó bằng 0, 1, 2 hoặc 3.

Mệnh đề đầu tiên suy ra từ Mđ. 9, (iii), được áp dụng cho $\beta = \gamma$, và sử dụng sự kiện rằng $q = 0$.

Mặt khác, vì $\gamma$ không tỷ lệ với $\alpha$, danh sách được cho ở đầu số này cho thấy rằng $|n(\gamma, \alpha)| \leq 3$, do đó có hệ quả.

#### Nhận xét {#lie-vi-s1-n3-rem-1 .statement}

Ta giữ lại ký hiệu ở trên. Khi đó:

1) Nếu độ dài của S bằng 0, thì $(\alpha|\gamma) = 0$.

2) Nếu độ dài của S bằng 1, thì $n(\gamma, \alpha) = -1$, và có ba trường hợp:

$$
n(\alpha, \gamma) = -1, \quad (\alpha|\alpha) = (\gamma|\gamma), \quad (\alpha|\gamma) = -\frac{1}{2}(\alpha|\alpha), \quad (\overline{\alpha, \gamma}) = \frac{2\pi}{3}
$$
$$
n(\alpha, \gamma) = -2, \quad (\alpha|\alpha) = 2(\gamma|\gamma), \quad (\alpha|\gamma) = -\frac{1}{2}(\alpha|\alpha), \quad (\overline{\alpha, \gamma}) = \frac{3\pi}{4}
$$
$$
n(\alpha, \gamma) = -3, \quad (\alpha|\alpha) = 3(\gamma|\gamma), \quad (\alpha|\gamma) = -\frac{1}{2}(\alpha|\alpha), \quad (\overline{\alpha, \gamma}) = \frac{5\pi}{6}
$$

![Three diagrams showing root systems with angles labeled π/3, π/4, 2π/3, and vectors γ + α, γ, γ + 2α](../images/root_systems_1.png)

3) Nếu độ dài của S bằng 2, thì $n(\gamma, \alpha) = -2$, do đó

$$
n(\alpha, \gamma) = -1, \quad (\alpha|\alpha) = \frac{1}{2}(\gamma|\gamma), \quad (\alpha|\gamma) = -(\alpha|\alpha), \quad (\overline{\alpha, \gamma}) = \frac{3\pi}{4}.
$$

![Diagram showing root system with angles π/4, π/4, and vectors γ, γ + α, γ + 2α](../images/root_systems_2.png)

4) Nếu độ dài của S bằng 3, thì $n(\gamma, \alpha) = -3$, do đó

$$
n(\alpha, \gamma) = -1, \quad (\alpha|\alpha) = \frac{1}{3}(\gamma|\gamma), \quad (\alpha|\gamma) = -\frac{3}{2}(\alpha|\alpha), \quad (\overline{\alpha, \gamma}) = \frac{5\pi}{6}.
$$

![Diagram showing root system with angles π/6, π/3, π/6, and vectors γ, γ + α, γ + 2α, γ + 3α](../images/root_systems_3.png)

Ta sẽ thấy (Bản X, các hệ A₂, B₂, G₂) rằng tất cả các trường hợp này thực sự đều xảy ra.

#### Mệnh đề 10 {#lie-vi-s1-prop-10 .statement}

*Cho $\alpha, \beta$ là hai nghiệm không tỷ lệ với nhau sao cho $\beta + \alpha$ là một nghiệm. Cho $p, q$ là các số nguyên trong Mệnh đề 9. Khi đó*

$$
\frac{(\beta + \alpha|\beta + \alpha)}{(\beta|\beta)} = \frac{q + 1}{p}.
$$

Cho S là chuỗi nghiệm $\alpha$ xác định bởi $\beta$, $\gamma$ là gốc của nó; độ dài $l$ của nó là $\geq 1$ vì $\beta + \alpha$ là một nghiệm. Các trường hợp sau đây có thể xảy ra:

1) $l = 1$; khi đó $\beta = \gamma, q = 0, p = 1, (\beta + \alpha|\beta + \alpha) = (\beta|\beta)$.
2) $l = 2, \beta = \gamma$; khi đó $q = 0, p = 2, (\beta + \alpha|\beta + \alpha) = \frac{1}{2}(\beta|\beta)$.
3) $l = 2, \beta = \gamma + \alpha$; khi đó $q = 1, p = 1, (\beta + \alpha|\beta + \alpha) = 2(\beta|\beta)$.

4) $l = 3, \beta = \gamma$; khi đó $q = 0, p = 3, (\beta + \alpha|\beta + \alpha) = \frac{1}{3}(\beta|\beta)$.
5) $l = 3, \beta = \gamma + \alpha$; khi đó $q = 1, p = 2, (\beta + \alpha|\beta + \alpha) = (\beta|\beta)$.
6) $l = 3, \beta = \gamma + 2\alpha$; khi đó $q = 2, p = 1, (\beta + \alpha|\beta + \alpha) = 3(\beta|\beta)$.

Trong mỗi trường hợp, công thức cần chứng minh đều được thỏa mãn.

#### Mệnh đề 11 {#lie-vi-s1-prop-11 .statement}

*Giả sử rằng R là bất khả quy. Cho $\alpha$ và $\beta$ là hai nghiệm sao cho $\| \alpha \| = \| \beta \|$. Tồn tại $g \in W(R)$ sao cho $g(\alpha) = \beta$.*

Các ảnh của $\alpha$ qua $W(R)$ sinh V (no. 2, Hệ quả của Mệnh đề 5). Do đó tồn tại $g \in W(R)$ sao cho $(g(\alpha)|\beta) \neq 0$. Từ nay ta giả sử rằng $(\alpha|\beta) \neq 0$. Theo công thức (9) của no. 1, $n(\alpha, \beta) = n(\beta, \alpha)$. Thay thế $\beta$ nếu cần thiết bởi $s_\beta(\beta) = -\beta$, ta có thể giả sử rằng $n(\alpha, \beta) > 0$. Khi đó, theo danh sách ở đầu no. 3, hoặc là $\alpha = \beta$ (trong trường hợp đó mệnh đề là hiển nhiên), hoặc là $n(\alpha, \beta) = n(\beta, \alpha) = 1$; trong trường hợp đó

$$
s_\alpha s_\beta s_\alpha(\beta) = s_\alpha s_\beta(\beta - \alpha) = s_\alpha(-\beta - \alpha + \beta) = \alpha.
$$

### 4. HỆ NGHIỆM RÚT GỌN

Một hệ nghiệm được gọi là *rút gọn* nếu mọi nghiệm của hệ là không phân chia được (no. 3).

#### Mệnh đề 12 {#lie-vi-s1-prop-12 .statement}

*Giả sử rằng R là bất khả quy và rút gọn.*

(i) *Tỉ số $\frac{(\beta|\beta)}{(\alpha|\alpha)}$ với $\alpha \in R, \beta \in R$ phải nhận một trong các giá trị 1, 2, $\frac{1}{2}$, 3, $\frac{1}{3}$.*

(ii) *Tập hợp các $(\alpha|\alpha)$ với $\alpha \in R$ có nhiều nhất hai phần tử.*

Vì R là bất khả quy, các ảnh của một nghiệm qua $W(R)$ sinh V (no. 2, Hệ quả của Mệnh đề 5). Do đó, với mọi nghiệm $\alpha, \beta$, tồn tại một nghiệm $\beta'$ sao cho $(\alpha|\beta') \neq 0$ và $(\beta'|\beta') = (\beta|\beta)$. Theo công thức (9) của no. 1 và danh sách của no. 3, $\frac{(\beta'|\beta')}{(\alpha|\alpha)}$ nhận một trong các giá trị 1, 2, $\frac{1}{2}$, 3, $\frac{1}{3}$ (nhớ rằng hệ được giả sử là rút gọn). Bằng cách nhân $(x|y)$ với một vô hướng thích hợp, ta có thể giả sử rằng $(\alpha|\alpha) = 1$ đối với một số nghiệm và các giá trị có thể khác của $(\beta|\beta)$ đối với $\beta \in R$ là 2 và 3. Các giá trị 2 và 3 không thể đồng thời đạt được, vì trong trường hợp đó sẽ tồn tại $\beta \in R, \gamma \in R$ sao cho $\frac{(\gamma|\gamma)}{(\beta|\beta)} = \frac{3}{2}$, trái với điều ta đã thấy ở trên.

#### Mệnh đề 13 {#lie-vi-s1-prop-13 .statement}

*Giả sử rằng R là bất khả quy, không rút gọn và có hạng $\geq 2$.*

(i) *Tập hợp $R_0$ các nghiệm không phân chia được là một hệ nghiệm trong V; hệ này là bất khả quy và rút gọn; và $W(R_0) = W(R)$.*

(ii) *Gọi A là tập hợp các nghiệm $\alpha$ mà $(\alpha|\alpha)$ nhận giá trị nhỏ nhất $\lambda$. Khi đó mọi hai phần tử không tỉ lệ với nhau của A là trực giao.*

(iii) *Gọi B là tập hợp các $\beta \in R$ sao cho $(\beta|\beta) = 2\lambda$. Khi đó $B \neq \varnothing$, $R_0 = A \cup B$, $R = A \cup B \cup 2A$.*

Nếu $\alpha \in R - R_0$, thì $\frac{1}{2} \alpha \in R$, nhưng $\frac{1}{2} (\frac{1}{2} \alpha) \notin R$ (Mệnh đề 8), do đó $\frac{1}{2} \alpha \in R_0$. Điều này chứng minh rằng $R_0$ thỏa mãn (RS$_1$). Hiển nhiên rằng, với mọi $\alpha \in R$, $s_{\alpha, \alpha^-}(R_0) = R_0$, do đó $R_0$ thỏa mãn (RS$_{II}$) và (RS$_{III}$). Vì $\alpha \in R - R_0$ kéo theo $\frac{1}{2} \alpha \in R_0$ và vì $s_\alpha = s_{\alpha/2}$, ta có $W(R) = W(R_0)$. Do đó $R_0$ là bất khả quy (Hệ quả của Mệnh đề 5), và hiển nhiên nó là rút gọn.

Vì $R$ không rút gọn, tồn tại $\alpha \in R_0$ sao cho $2\alpha \in R$. Vì $R_0$ là bất khả quy và $\dim V \geq 2$, $\alpha$ không thể tỉ lệ hoặc vuông góc với mọi nghiệm. Cho $\beta \in R_0$ sao cho $n(\beta, \alpha) \neq 0$ và $\beta$ không tỉ lệ với $\alpha$. Nếu cần thì thay $\beta$ bởi $-\beta$, ta có thể giả sử rằng $n(\beta, \alpha) > 0$. Khi đó $\frac{1}{2} n(\beta, \alpha) = n(\beta, 2\alpha) \in \mathbf{Z}$, do đó $n(\beta, \alpha) \in 2\mathbf{Z}$. Từ danh sách trong no. 3, $n(\beta, \alpha) = 2$, $(\beta|\beta) = 2(\alpha|\alpha)$. Vì $R_0$ rút gọn, Mệnh đề 12 cho thấy rằng, với mọi $\gamma \in R_0$, hoặc $(\gamma|\gamma) = (\alpha|\alpha)$ hoặc $(\gamma|\gamma) = 2(\alpha|\alpha)$. Ngoài ra, điều trên cho thấy rằng, với mọi $\gamma \in R - R_0$, vectơ $\frac{1}{2} \gamma$ là một phần tử của $R_0$ sao cho $(\frac{1}{2} \gamma|\frac{1}{2} \gamma) = (\alpha|\alpha)$. Như vậy, $\lambda = (\alpha|\alpha)$, $B \neq \varnothing$, $R_0 = A \cup B$, và $R \subseteq A \cup B \cup 2A$; mặt khác, nếu $\gamma \in A$, tồn tại $g \in W(R)$ sao cho $\gamma = g(\alpha)$ (Mệnh đề 11), do đó $2\gamma = g(2\alpha) \in R$; vậy $2A \subseteq R$ và $R = A \cup B \cup 2A$. Cuối cùng, cho $\gamma, \gamma'$ là hai phần tử không tỉ lệ của $A$. Khi đó

$$
n(2\gamma, \gamma') = 2n(\gamma, \gamma') = 4n(\gamma, 2\gamma') \in 4\mathbf{Z}, \quad \text{và} \quad |n(\gamma, \gamma')| \leq 1
$$

vì $\gamma$ và $\gamma'$ có cùng độ dài, do đó $n(\gamma, \gamma') = 0$ và $(\gamma|\gamma') = 0$.

#### Mệnh đề 14 {#lie-vi-s1-prop-14 .statement}

*Giả sử rằng $R$ là bất khả quy và rút gọn, và rằng $(\alpha|\alpha)$ nhận các giá trị $\lambda$ và $2\lambda$ với $\alpha \in R$. Gọi $A$ là tập hợp các nghiệm $\alpha$ sao cho $(\alpha|\alpha) = \lambda$. Giả sử rằng mọi hai phần tử không tỉ lệ của $A$ đều vuông góc. Khi đó $R_1 = R \cup 2A$ là một hệ nghiệm bất khả quy không rút gọn và $R$ là tập hợp các nghiệm không chia hết của $R_1$.*

Hiển nhiên rằng $R_1$ thỏa mãn (RS$_1$) và (RS$_{III}$). Ta chứng minh rằng, nếu $\alpha, \beta \in R_1$, thì $\langle \alpha^-, \beta \rangle \in \mathbf{Z}$. Điều này hiển nhiên nếu $\alpha \in R$. Vì $(2\alpha)^- = \frac{1}{2} \alpha^-$ với $\alpha \in A$, điều này cũng ngay lập tức đúng nếu $\alpha, \beta \in 2A$. Cuối cùng, giả sử rằng $\beta \in R$ và $\alpha = 2\gamma$ với $\gamma \in A$.

1) Nếu $\gamma = \pm \beta$, thì $\langle \alpha^-, \beta \rangle = \pm \frac{1}{2} \langle \gamma^-, \gamma \rangle = \pm 1$.
2) Nếu $\gamma$ không tỷ lệ với $\beta$ và nếu $\beta \in A$, giả thiết về $A$ suy ra rằng $\langle \gamma^-, \beta \rangle = 0$, do đó $\langle \alpha^-, \beta \rangle = 0$.
3) Nếu $\beta \in R - A$, thì $(\beta|\beta) = 2\lambda = 2(\gamma|\gamma)$, do đó $\langle \beta, \gamma^- \rangle$ bằng 0, 2 hoặc -2 theo danh sách trong no. 3. Vì vậy $\langle \beta, \alpha^- \rangle = \frac{1}{2} \langle \beta, \gamma^- \rangle \in \mathbf{Z}$.

Vậy $R_1$ là một hệ nghiệm trong $V$, và các khẳng định khác là hiển nhiên.

### 5. CÁC PHÒNG VÀ CƠ SỞ CỦA CÁC HỆ NGHIỆM

Với mọi $\alpha \in R$, cho $L_\alpha$ là siêu phẳng của $V$ gồm các điểm bất biến dưới $s_\alpha$. Các phòng trong $V$ được xác định bởi tập hợp các $L_\alpha$ (Chương V, § 1, no. 3) được gọi là các *phòng* của $R$. Song ánh $V \to V^*$ được xác định bởi tích vô hướng $(x|y)$ đưa $\alpha$ thành $\frac{2\alpha^-}{(\alpha^-|\alpha^-)}$ với $\alpha \in R$, do đó đưa $L_\alpha$ thành $L_{\alpha^-}$, và do đó đưa các phòng của $R$ thành các phòng của $R^-$. Nếu $C$ là một phòng của $R$, thì phòng tương ứng của $R^-$ được ký hiệu là $C^-$. Theo Mệnh đề 7 của no. 2, $C^-$ chỉ phụ thuộc vào $C$ chứ không phụ thuộc vào lựa chọn của $(x|y)$.

#### Định lý 2 {#lie-vi-s1-thm-2 .statement}

(i) *Nhóm* $W(R)$ *tác động đơn bắc cầu lên tập hợp các phòng*.

(ii) *Cho* $C$ *là một phòng. Khi đó* $\overline{C}$ *là một miền cơ bản đối với* $W(R)$.

(iii) $C$ *là một nón đơn hình mở* (Chương V, § 1, no. 6).

(iv) *Gọi* $L_1, L_2, \ldots, L_l$ *là các tường của* $C$. *Với mọi* $i$, *tồn tại duy nhất một nghiệm bất khả quy* $\alpha_i$ *sao cho* $L_i = L_{\alpha_i}$ *và sao cho* $\alpha_i$ *nằm cùng phía của* $L_i$ *với* $C$.

(v) *Tập hợp* $B(C) = \{ \alpha_1, \ldots, \alpha_l \}$ *là một cơ sở của* $V$.

(vi) $C$ *là tập hợp các* $x \in V$ *sao cho* $\langle \alpha_i, x \rangle > 0$ *với mọi* $i$ *(hay, tương đương, là tập hợp các* $x \in V$ *sao cho* $(x|\alpha_i) > 0$ *với mọi* $i$).

(vii) *Gọi* $S$ *là tập hợp các* $s_{\alpha_i}$. *Cặp* $(W(R), S)$ *là một hệ Coxeter* (Chương IV, § 1, no. 3).

Các mệnh đề (i) và (vii) suy ra từ Chương V, § 3, no. 2, Định lý 1. Mệnh đề (ii) suy ra từ Chương V, § 3, no. 3, Định lý 2. Mệnh đề (iv) là hiển nhiên. Nghiệm $\alpha_i$ vuông góc với $L_i$, và $\alpha_i^-$ được đồng nhất với $2\alpha_i / (\alpha_i|\alpha_i)$. Vì $W(R)$ là cốt yếu (no. 1, *Nhận xét 3*), các mệnh đề (iii), (v) và (vi) suy ra từ Chương V, § 3, no. 9, Mệnh đề 7.

#### Nhận xét 1 {#lie-vi-s1-n5-rem-1 .statement}

Mệnh đề (vii) chỉ ra đặc biệt rằng $W(R)$ được *sinh* bởi các phép đối xứng $s_{\alpha_i}$.

#### Nhận xét 2 {#lie-vi-s1-n5-rem-2 .statement}

Nếu $x, y \in C$, thì $(x|y) > 0$ (Chương V, § 3, no. 5, Bổ đề 6), nói cách khác góc $(x, y)$ là *nhọn*.

#### Nhận xét 3 {#lie-vi-s1-n5-rem-3 .statement}

Gọi $m(\alpha, \beta)$ là cấp của $s_{\alpha} s_{\beta}$ ($\alpha, \beta \in B(C)$). Ma trận $(m(\alpha, \beta))$ được đồng nhất với *ma trận Coxeter* (Chương IV, § 1, no. 9) của $(W, S)$. Nếu $\alpha \neq \beta$, Mệnh đề 3 của Chương V, § 3, no. 4 chỉ ra rằng góc $(\alpha, \beta)$ bằng $\pi - \frac{\pi}{m(\alpha, \beta)}$; đặc biệt, góc này hoặc tù hoặc bằng $\pi$, và $(\alpha|\beta) \leq 0$. Bằng cách sử dụng danh sách trong no. 3, suy ra rằng $m(\alpha, \beta)$ *bằng* 2, 3, 4 *hoặc* 6.

#### Định nghĩa 2 {#lie-vi-s1-def-2 .statement}

*Một tập con* $B$ *của* $R$ *được gọi là một cơ sở của* $R$ *nếu tồn tại một phòng* $C$ *của* $R$ *sao cho* $B = B(C)$. *Nếu* $C$ *là một phòng*, $B(C)$ *được gọi là cơ sở của* $R$ *được xác định bởi* $C$.

#### Nhận xét 4 {#lie-vi-s1-n5-rem-4 .statement}

Mệnh đề (vi) của Định lý 2 chỉ ra rằng ánh xạ $C \mapsto B(C)$ là một *song ánh* từ tập hợp các phòng đến tập hợp các cơ sở. Do đó, $W(R)$ tác động *đơn bắc cầu* trên tập hợp các cơ sở.

#### Nhận xét 5 {#lie-vi-s1-n5-rem-5 .statement}

Cho $C$ là một buồng của $R$, và cho $B$ là cơ sở tương ứng. Nếu $\alpha \in B$, đặt $\varphi(\alpha) = \alpha^-$ nếu $2\alpha \notin R$ và $\varphi(\alpha) = \frac{1}{2}\alpha^-$ nếu $2\alpha \in R$. Khi đó $\varphi(B)$ *là cơ sở của* $R^-$ *được định nghĩa bởi* $C^-$; điều này suy ra từ sự kiện rằng các siêu phẳng của $C^-$ là các $L_{\alpha^-}$, với $\alpha \in B$.

#### Định nghĩa 3 {#lie-vi-s1-def-3 .statement}

Cho B là một cơ sở của R. Ma trận Cartan của R (đối với B) là ma trận $(n(\alpha, \beta))_{\alpha, \beta \in B}$.

Với mọi $\alpha \in B$, $n(\alpha, \alpha) = 2$. Với $\alpha, \beta \in B$,

$$
n(\alpha, \beta) = 2 \frac{(\alpha|\beta)}{(\beta|\beta)} = -2 \frac{\|\alpha\|}{\|\beta\|} \cos \frac{\pi}{m(\alpha, \beta)},
$$

trong đó $m(\alpha, \beta)$ chỉ cấp của $s_\alpha s_\beta$ như trên. Nếu $\alpha \neq \beta$, $n(\alpha, \beta) = 0, -1, -2$ hoặc $-3$ (xem no. 3).

#### Nhận xét 6 {#lie-vi-s1-n5-rem-6 .statement}

Ma trận Cartan $(n(\alpha, \beta))$ không nên bị nhầm lẫn với ma trận Coxeter $(m(\alpha, \beta))$. Đặc biệt chú ý rằng ma trận Cartan không nhất thiết đối xứng.

#### Nhận xét 7 {#lie-vi-s1-n5-rem-7 .statement}

Đánh chỉ số chính tắc. Nếu B và $B'$ là hai cơ sở của R, tồn tại một phần tử duy nhất $w \in W$ sao cho $w(B) = B'$. Ta có

$$
n(w(\alpha), w(\beta)) = n(\alpha, \beta) \quad \text{và} \quad m(w(\alpha), w(\beta)) = m(\alpha, \beta)
$$

với $\alpha, \beta \in B$. Do đó, các ma trận Cartan và Coxeter liên kết với B có thể nhận được từ các ma trận liên kết với $B'$ bằng cách hợp thành với song ánh

$$
\alpha \mapsto w(\alpha)
$$

từ B đến $B'$.

Các ma trận Cartan và Coxeter thực ra có thể được định nghĩa một cách chính tắc theo cách sau. Gọi X là tập hợp các cặp $(B, \alpha)$, trong đó B là một cơ sở của R và $\alpha \in B$. Nhóm W tác động một cách hiển nhiên lên X và mỗi quỹ đạo của W trên X gặp mỗi tập hợp $\{B\} \times B$ tại đúng một điểm. Nếu I là tập hợp các quỹ đạo này, mỗi cơ sở B thừa nhận một cách đánh chỉ số chính tắc $(\alpha_i)_{i \in I}$. Hơn nữa, tồn tại một ma trận duy nhất $N = (n_{ij})$ (tương ứng $M = (m_{ij})$), kiểu $I \times I$, sao cho với mọi cơ sở B, ma trận Cartan (tương ứng Coxeter) liên kết với B có thể nhận được từ N (tương ứng M) bằng cách hợp thành với phép đánh chỉ số chính tắc của B; nó được gọi là ma trận Cartan chính tắc (tương ứng ma trận Coxeter chính tắc) của R.

#### Mệnh đề 15 {#lie-vi-s1-prop-15 .statement}

Cho B là một cơ sở của R và $\alpha$ là một nghiệm không phân chia. Tồn tại $\beta \in B$ và $w \in W(R)$ sao cho $\alpha = w(\beta)$.

Cho C là buồng sao cho $B = B(C)$. Siêu phẳng $L_\alpha$ là một tường của một buồng $C'$ của R, và tồn tại một phần tử của $W(R)$ biến $C'$ thành C. Do đó ta quy về trường hợp $L_\alpha$ là một tường của C. Khi đó $\alpha$ tỉ lệ với một phần tử $\beta$ của R. Vì $\alpha$ và $\beta$ không phân chia, $\alpha = \pm \beta$. Nếu $\alpha = -\beta$, thì $\alpha = s_\beta(\beta)$, do đó có mệnh đề.

#### Hệ quả {#lie-vi-s1-n5-cor-1 .statement}

Cho $R_1$ và $R_2$ là hai hệ nghiệm rút gọn trong các không gian vectơ $V_1$ và $V_2$, và cho $B_1$ và $B_2$ là các cơ sở của $R_1$ và $R_2$. Cho $f : B_1 \to B_2$ là một song ánh biến ma trận Cartan của $R_1$ thành ma trận Cartan của $R_2$. Khi đó tồn tại một đẳng cấu $F : V_1 \to V_2$ biến $R_1$ thành $R_2$ và $\alpha$ thành $f(\alpha)$ với mọi $\alpha \in B_1$.

Cho $F$ là đẳng cấu từ $V_1$ đến $V_2$ lấy $\alpha$ thành $f(\alpha)$ với mọi $\alpha \in B_1$. Khi đó $F$ biến $s_\alpha$ thành $s_{f(\alpha)}$, do đó $W(R_1)$ thành $W(R_2)$ (Đl. 2), và do đó $R_1$ thành $R_2$ (Mđ. 15).

#### Mệnh đề 16 {#lie-vi-s1-prop-16 .statement}

Cho $B$ là một cơ sở của $R$, và $G$ là nhóm con của $A(R)$ gồm các phần tử giữ $B$ ổn định. Khi đó $W(R)$ là một nhóm con chuẩn của $A(R)$ và $A(R)$ là tích nửa trực tiếp của $G$ và $W(R)$.

Nếu $\alpha \in R$ và $t \in A(R)$, thì $ts_\alpha t^{-1} = s_{t(\alpha)}$; vì $W(R)$ được sinh bởi các $s_\alpha$, ta thấy rằng $W(R)$ là một nhóm con chuẩn của $A(R)$. Bằng phép chuyển cấu trúc, $A(R)$ biến một cơ sở của $R$ thành một cơ sở của $R$. Vì $W(R)$ tác động bắc cầu đơn giản trên tập hợp các cơ sở, mỗi phần tử của $A(R)$ có thể được viết duy nhất dưới dạng $g_1 g_2$, trong đó $g_1 \in W(R)$ và $g_2 \in G$.

#### Nhận xét 8 {#lie-vi-s1-n5-rem-8 .statement}

Cho $R_1, \ldots, R_p$ là các hệ nghiệm trong các không gian vectơ $V_1, \ldots, V_p$, $R$ là tổng trực tiếp của các $R_i$ trong $V = \prod_i V_i$, $C_i$ là một buồng của $R_i$, và $B_i = B(C_i)$. Ngay lập tức ta thấy rằng $C = \prod_i C_i$ là một buồng của $R$ và rằng $B(C) = \bigcup_i B_i$. Từ Đl. 2 suy ra rằng tất cả các buồng và cơ sở của $R$ đều thu được theo cách này.

### 6. CÁC NGHIỆM DƯƠNG

Cho $C$ là một buồng của $R$, và cho $B(C) = \{ \alpha_1, \ldots, \alpha_l \}$ là cơ sở tương ứng của $R$. Quan hệ thứ tự trên $V$ (tương ứng $V^*$) được xác định bởi $C$ là quan hệ thứ tự tương thích với cấu trúc không gian vectơ của $V$ (tương ứng $V^*$), trong đó các phần tử $\geq 0$ là các tổ hợp tuyến tính của các $\alpha_i$ (tương ứng các $\alpha_i^*$) với các hệ số $\geq 0$. Một phần tử dương đối với một trong các quan hệ này được gọi là dương đối với $C$, hay dương đối với cơ sở $B(C)$. Các quan hệ thứ tự này cũng được xác định bởi $C^*$, như thấy được bằng cách đồng nhất $V$ với $V^*$ nhờ sử dụng một tích vô hướng bất biến dưới $W(R)$. Theo Đl. 2, no. 5, một phần tử của $V^*$ là $\geq 0$ khi và chỉ khi các giá trị của nó trên $C$ là $\geq 0$. Một phần tử $x$ của $V$ là $\geq 0$ khi và chỉ khi các giá trị của nó trên $C^*$ là $\geq 0$, hay, tương đương, nếu $(x|y) \geq 0$ với mọi $y \in C$.

Các phần tử của $\overline{C}$ là $\geq 0$ đối với $C$ theo Bổ đề 6 của Ch. V, § 3, no. 5. Nhưng tập hợp các phần tử $\geq 0$ đối với $C$ nói chung là phân biệt với $\overline{C}$ (xem Plate X, các hệ $A_2, B_2, G_2$).

#### Định lý 3 {#lie-vi-s1-thm-3 .statement}

Mọi nghiệm đều là một tổ hợp tuyến tính với các hệ số nguyên cùng dấu của các phần tử của $B(C)$. Đặc biệt, mọi nghiệm đều hoặc dương hoặc âm đối với $C$.

Nếu $\alpha \in R$, hạt nhân $L_\alpha$ của $\alpha$ không gặp $C^*$, do đó $\alpha$ hoặc là $> 0$ trên toàn bộ $C^*$ hoặc là $< 0$ trên toàn bộ $C^*$, suy ra mệnh đề thứ hai. Còn lại phải chứng minh rằng $\alpha$ được chứa trong nhóm con $P$ của $V$ sinh bởi $B(C)$; ta có thể giả sử rằng $\alpha$ không phân chia được. Khi đó nhóm $P$ rõ ràng ổn định dưới các $s_{\gamma}$, với $\gamma \in B(C)$, do đó cũng ổn định dưới $W(R)$ theo Đl. 2. Vì $\alpha$ có dạng $w(\beta)$, với $w \in W(R)$ và $\beta \in B(C)$ (xem Mđ. 15), ta có $\alpha \in P$. Đpcm.

Ký hiệu $R_+(C)$ là tập hợp các nghiệm dương đối với $C$. Khi đó,
$$
R = R_+(C) \cup (-R_+(C))
$$
là một phân hoạch của $R$.

#### Hệ quả {#lie-vi-s1-n6-cor-1 .statement}

*Cho $\gamma$ là một tổ hợp tuyến tính của các nghiệm với các hệ số nguyên, và $\alpha$ là một nghiệm không phân chia được. Nếu $\gamma$ tỉ lệ với $\alpha$, thì $\gamma \in \mathbf{Z}\alpha$.*

Theo Mđ. 15 của no. 5, có thể chọn $C$ sao cho $\alpha \in B(C)$. Theo Đl. 3,
$$
\gamma = \sum_{\beta \in B(C)} n_{\beta} \beta \quad \text{với} \quad n_{\beta} \in \mathbf{Z}.
$$
Do đó, nếu $\gamma$ tỉ lệ với $\alpha$, thì $\gamma = n_{\alpha} \alpha$, điều này chứng minh hệ quả.

Bây giờ cho $S$ là tập hợp các phép phản xạ $s_{\alpha}$ với $\alpha \in B(C)$ và cho $T$ là hợp của các liên hợp của $S$ theo $W$. Với $\alpha \in B(C)$ và $w \in W$, phần tử $t = ws_{\alpha}w^{-1}$ của $T$ là phép phản xạ trực giao $s_{\beta}$ liên kết với nghiệm $\beta = w(\alpha)$; ngược lại, với mọi nghiệm không phân chia được $\beta$, tồn tại một phần tử $w \in W$ sao cho $\alpha = w^{-1}(\beta) \in B(C)$ (Mệnh đề 15) và $s_{\beta} = ws_{\alpha}w^{-1} \in T$. Suy ra rằng một *song ánh* $\psi$ từ tập hợp các nghiệm không phân chia được đến $\{\pm 1\} \times T$ được thu được bằng cách liên kết với một nghiệm không phân chia được $\beta$ cặp $(\varepsilon, s_{\beta})$, trong đó $\varepsilon = +1$ nếu $\beta$ là dương và $\varepsilon = -1$ nếu $\beta$ là âm.

Mặt khác, $(W, S)$ là một hệ Coxeter (Định lý 2) và các kết quả của Chương IV, § 1, no. 4 có thể được áp dụng. Ta đã thấy rằng, nếu $w$ là một phần tử của $W$ có độ dài (đối với $S$) bằng $q$, tồn tại một tập con $T_w$ của $T$, với $q$ phần tử, sao cho, nếu $w = s_1 \ldots s_q$ với $s_i \in S$ và nếu
$$
t_i = s_1 \ldots s_{i-1} s_i s_{i-1} \ldots s_1
$$
(với $1 \leq i \leq q$), thì $T_w = \{t_1, \ldots, t_q\}$. Nhắc lại rằng ta cũng đã định nghĩa trong no. 4 của § 1 một số $\eta(w, t)$ (với $w \in W$ và $t \in T$) bằng $+1$ nếu $t \notin T_w$ và bằng $-1$ nếu $t \in T_w$. Cuối cùng, nhắc lại rằng, nếu ta định nghĩa một ánh xạ $U_w$ từ tập hợp $\{\pm 1\} \times T$ vào chính nó bởi công thức
$$
U_w(\varepsilon, t) = (\varepsilon \eta(w^{-1}, t), wt w^{-1}),
$$
ánh xạ $w \mapsto U_w$ là một *đồng cấu* từ $W$ đến nhóm các phép hoán vị của tập hợp $\{\pm 1\} \times T$ (Chương IV, § 1, no. 4, Bổ đề 1).

#### Mệnh đề 17 {#lie-vi-s1-prop-17 .statement}

*Giả sử rằng $R$ là thu gọn và cho $w \in W$ và $\alpha \in R$.*

(i) *Ta có $\psi(w(\alpha)) = U_w(\psi(\alpha))$.*
(ii) *Giả sử rằng $\alpha$ là dương. Nghiệm $w(\alpha)$ là âm khi và chỉ khi*
$$
\eta(w^{-1}, s_{\alpha}) = -1,
$$
*hay nói cách khác nếu* $s_{\alpha} \in T_{w^{-1}}$.

(iii) Ta có $\eta(w, s_\alpha) = -1$ khi và chỉ khi các phòng C và $w(C)$ nằm ở hai phía đối nhau của siêu phẳng $L_\alpha$. Nói cách khác, tập hợp $T_w$ gồm các phép đối xứng qua các tường ngăn cách C và $w(C)$.

Cho $\beta \in B(C)$ và đặt $s = s_\beta$. Rõ ràng $T_s = \{ s \}$ và do đó

$$
U_s(\varepsilon, t) = \begin{cases}
(\varepsilon, st s^{-1}) & \text{nếu } t \neq s \\
(-\varepsilon, s) & \text{nếu } t = s.
\end{cases}
$$

Mặt khác, cho $\rho = \sum_{\gamma \in B(C)} n_\gamma(\rho) \gamma$ là một nghiệm dương. Đặt

$$
s(\rho) = \sum_{\gamma \in B(C)} n_\gamma(s(\rho)) \gamma.
$$

Nếu $\rho \neq \beta$, tồn tại một phần tử $\gamma \in B(C)$ với $\gamma \neq \beta$, sao cho $n_\gamma(\rho) > 0$, và ta có $n_\gamma(s(\rho)) = n_\gamma(\rho) > 0$ (no. 1, công thức (5)). Do đó $s(\rho)$ là dương. Ta suy ra ngay lập tức rằng

$$
\psi(s(\varepsilon, \rho)) = \begin{cases}
(\varepsilon, ss_\rho s^{-1}) & \text{nếu } \rho \neq \beta \\
(-\varepsilon, s) & \text{nếu } \rho = \beta.
\end{cases}
$$

So sánh (12) và (13) cho thấy rằng $U_s(\psi(\gamma)) = \psi(s(\gamma))$ với mọi nghiệm $\gamma$ và mọi $s \in S$. Vì S sinh ra W, suy ra (i).

Mặt khác, nói rằng $w(\alpha)$ là âm tương đương với nói rằng

$$
\psi(w(\alpha)) = (-1, ws_\alpha w^{-1}),
$$

hoặc, theo (i), rằng $U_w(\psi(\alpha)) = (-1, ws_\alpha w^{-1})$. Nếu thêm rằng $\alpha$ là dương, thì $\psi(\alpha) = (+1, s_\alpha)$ và $U_w(\psi(\alpha)) = (\eta(w^{-1}, s_\alpha), ws_\alpha w^{-1})$, do đó (ii).

Cuối cùng, theo (ii), $\eta(w, s_\alpha) = -1$ khi và chỉ khi một trong các nghiệm $\alpha$ và $w^{-1}(\alpha)$ là dương còn nghiệm kia là âm. Điều này tương đương với nói rằng $(\alpha|x).(w^{-1}(\alpha)|x) = (\alpha|x).(w|x) < 0$ với mọi $x \in C$, do đó có mệnh đề đầu tiên trong (iii). Mệnh đề thứ hai trong (iii) suy ra ngay lập tức.

#### Hệ quả 1 {#lie-vi-s1-prop-17-cor-1 .statement}

Cho $\beta \in B(C)$. Phép đối xứng $s_\beta$ hoán vị các nghiệm dương không tỉ lệ với $\beta$.

Ta rút gọn ngay lập tức về trường hợp R là rút gọn. Trong trường hợp đó, mệnh đề của ta suy ra từ (ii) và sự kiện rằng $T_{s_\beta} = s_\beta$.

#### Hệ quả 2 {#lie-vi-s1-prop-17-cor-2 .statement}

Giả sử rằng R là rút gọn. Cho $w \in W$, gọi q là độ dài của $w$ đối với S (Chap. IV, § 1, no. 1), và cho $w = s_1 \ldots s_q$ là một phân tích rút gọn của $w$. Cho $\alpha_1, \ldots, \alpha_q$ là các phần tử của $B(C)$ tương ứng với $s_1, \ldots, s_q$. Đặt

$$
\theta_i = s_q s_{q-1} \ldots s_{i+1}(\alpha_i), \quad i = 1, \ldots, q.
$$

Các nghiệm $\theta_i$ là $> 0$, từng đôi một phân biệt, $w(\theta_i) < 0$, và mọi nghiệm $\alpha > 0$ sao cho $w(\alpha) < 0$ đều bằng một trong các $\theta_i$.

Gọi X là tập hợp các $\alpha > 0$ sao cho $w(\alpha) < 0$. Theo (ii),

$$
\operatorname{Card}(X) = \operatorname{Card}(T_{w^{-1}}) = l(w^{-1}) = l(w) = q.
$$

Mặt khác, nếu $\alpha \in X$ thì rõ ràng tồn tại $i \in \{1, q\}$ sao cho

$$
s_{i+1} \ldots s_q(\alpha) > 0 \quad \text{và} \quad s_i s_{i+1} \ldots s_q(\alpha) < 0.
$$

Theo Hệ quả 1, điều này suy ra rằng $s_{i+1} \ldots s_q(\alpha) = \alpha_i$ và do đó $\alpha = \theta_i$. Vì vậy tập hợp X được chứa trong tập hợp các $\theta_i$. Vì $\operatorname{Card}(X) = q$, điều này chỉ có thể xảy ra nếu X bằng tập hợp các $\theta_i$ và các phần tử này từng đôi một phân biệt. Do đó có hệ quả.

#### Hệ quả 3 {#lie-vi-s1-prop-17-cor-3 .statement}

*Giả sử rằng R là rút gọn. Tồn tại một phần tử dài nhất duy nhất $w_0$ trong W. Độ dài của nó bằng số các nghiệm dương và $w_0$ biến phòng C thành $-C$. Ta có $w_0^2 = 1$ và $l(ww_0) = l(w_0) - l(w)$ với mọi $w \in W$.*

Hiển nhiên rằng $-C$ là một phòng. Do đó tồn tại một phần tử $w_0$ của W biến C thành $-C$. Khi đó $w_0(\alpha) < 0$ với mọi nghiệm dương $\alpha$ và hai khẳng định đầu tiên của Hệ quả 3 là các hệ quả ngay lập tức của Hệ quả 2. Ta có $w_0^2(C) = C$, nên $w_0^2 = 1$. Cuối cùng, nếu $w \in W$, độ dài $l(w)$ (tương ứng $l(ww_0)$) bằng, theo Mệnh đề 17 (iii), số các tường ngăn cách C và $w(C)$ (tương ứng $ww_0(C) = -w(C)$). Vì $w(C)$ và $-w(C)$ nằm ở hai phía đối của mỗi tường, tổng $l(w) + l(w_0)$ bằng tổng số các tường, tức là bằng $l(w_0)$.

#### Mệnh đề 18 {#lie-vi-s1-prop-18 .statement}

*Cho $x \in V$. Ba tính chất sau là tương đương:

(i) $x \in \overline{C}$;
(ii) $x \geq s_\alpha(x)$ với mọi $\alpha \in B(C)$ (theo quan hệ thứ tự được xác định bởi C);
(iii) $x \geq w(x)$ với mọi $w \in W$.*

Vì $s_\alpha(x) = x - \langle x, \alpha^\vee \rangle \alpha$ và vì $\overline{C}$ là tập hợp các phần tử $x \in V$ sao cho $\langle x, \alpha^\vee \rangle \geq 0$ với mọi $\alpha \in B(C)$, sự tương đương của (i) và (ii) là hiển nhiên. Mặt khác, rõ ràng là (iii) $\Longrightarrow$ (ii). Ta chứng minh rằng (i) $\Longrightarrow$ (iii). Cho $x \in \overline{C}$, và cho $w \in W$. Ta lập luận bằng quy nạp theo độ dài $l(w)$ của $w$. Trường hợp $l(w) = 0$ là tầm thường. Nếu $l(w) \geq 1$, $w$ có thể được viết dưới dạng $w = w' s_\alpha$, với $\alpha \in B(C)$ và $l(w') = l(w) - 1$. Khi đó

$$
x - w(x) = x - w'(x) + w'(x - s_\alpha(x)).
$$

Giả thiết quy nạp chỉ ra rằng $x - w'(x)$ là dương. Mặt khác,

$$
w'(x - s_\alpha(x)) = w(s_\alpha(x) - x) = -\langle x, \alpha^\vee \rangle w(\alpha).
$$

Bây giờ $s_\alpha \in T_{w^{-1}}$, và Mệnh đề 17 (ii) chỉ ra rằng $w(\alpha) < 0$. Do đó có kết quả.

#### Hệ quả {#lie-vi-s1-n6-cor-2 .statement}

Một phần tử $x \in C$ khi và chỉ khi $x > w(x)$ với mọi $w \in W$ sao cho $w \neq 1$.

#### Mệnh đề 19 {#lie-vi-s1-prop-19 .statement}

Cho $(\beta_i)_{1 \leq i \leq n}$ là một dãy các nghiệm dương đối với phòng $C$ sao cho $\beta_1 + \beta_2 + \cdots + \beta_n$ là một nghiệm. Khi đó tồn tại một phép hoán vị $\pi \in S_n$ sao cho, với mọi $i \in \{1, 2, \ldots, n\}$, $\beta_{\pi(1)} + \beta_{\pi(2)} + \cdots + \beta_{\pi(i)}$ là một nghiệm.

Ta lập luận bằng quy nạp theo $n$, mệnh đề hiển nhiên đối với $n \leq 2$. Đặt $\beta = \beta_1 + \cdots + \beta_n$. Khi đó $\sum_{i=1}^n (\beta|\beta_i) = (\beta|\beta) > 0$, do đó tồn tại một chỉ số $k$ sao cho $(\beta|\beta_k) > 0$. Nếu $\beta = \beta_k$, thì $n = 1$ vì $\beta_i > 0$ với mọi $i$. Ngược lại $\beta - \beta_k$ là một nghiệm (no. 3, Hệ quả của Định lý 1); khi đó chỉ cần áp dụng giả thiết quy nạp cho $\beta - \beta_k = \sum_{i \neq k} \beta_i$.

#### Hệ quả 1 {#lie-vi-s1-prop-19-cor-1 .statement}

Cho $\alpha \in R_+(C)$. Khi đó $\alpha \in B(C)$ khi và chỉ khi $\alpha$ là tổng của hai nghiệm dương.

Nếu $\alpha$ là tổng của hai nghiệm dương, Định lý 3 cho thấy rằng $\alpha \in B(C)$. Nếu $\alpha \notin B(C)$, Định lý 3 cho thấy rằng $\alpha = \sum_{k=1}^n \beta_k$ với $\beta_k \in B(C)$ với mọi $k$ và $n \geq 2$.

Hoán vị các $\beta_k$ nếu cần, ta có thể giả sử rằng $\sum_{k=1}^{n-1}$ là một nghiệm (Mệnh đề 19), và do đó $\alpha$ là tổng của các nghiệm dương $\sum_{k=1}^{n-1} \beta_k$ và $\beta_n$.

#### Hệ quả 2 {#lie-vi-s1-prop-19-cor-2 .statement}

Cho $\varphi$ là một ánh xạ từ $R$ vào một nhóm Abel $\Gamma$ có các tính chất sau:

1) $\varphi(-\alpha) = -\varphi(\alpha)$ với $\alpha \in R$;
2) nếu $\alpha \in R, \beta \in R$ là sao cho $\alpha + \beta \in R$, thì $\varphi(\alpha + \beta) = \varphi(\alpha) + \varphi(\beta)$.

Gọi $Q$ là nhóm con của $V$ sinh bởi $R$. Khi đó $\varphi$ mở rộng thành một đồng cấu từ $Q$ đến $\Gamma$.

Cho $B$ là một cơ sở của $R$. Cho $\psi$ là đồng cấu duy nhất từ $Q$ đến $\Gamma$ trùng với $\varphi$ trên $B$. Chỉ cần chứng minh rằng $\psi(\alpha) = \varphi(\alpha)$ khi $\alpha$ là một nghiệm dương đối với $B$. Ta có $\alpha = \beta_1 + \cdots + \beta_m$ với $\beta_i \in B$ với mọi $i$, và $\beta_1 + \cdots + \beta_h \in R$ với mọi $h$ (Mệnh đề 19). Ta chứng minh rằng $\psi(\alpha) = \varphi(\alpha)$ bằng quy nạp theo $m$. Điều này là hiển nhiên nếu $m = 1$. Giả thiết quy nạp cho

$$
\psi(\beta_1 + \cdots + \beta_{m-1}) = \varphi(\beta_1 + \cdots + \beta_{m-1}),
$$

và ta có $\psi(\beta_m) = \varphi(\beta_m)$, do đó $\psi(\alpha) = \varphi(\alpha)$, điều này chứng minh hệ quả.

Với mọi nghiệm $\alpha = \sum_{\beta \in B(C)} n_\beta \beta$ trong $R$, ký hiệu $Y(\alpha)$ là tập hợp các $\beta \in B(C)$ sao cho $n_\beta \neq 0$. Hơn nữa, nhận xét rằng $B(C)$ có thể được đồng nhất với tập hợp các đỉnh của đồ thị của hệ Coxeter được tạo bởi $W(R)$ và các $s_{\alpha_i}$ (xem Ch. IV, § 1, no. 9 và Ch. V, § 3, no. 2).

#### Hệ quả 3 {#lie-vi-s1-prop-19-cor-3 .statement}

a) Cho $\alpha \in \mathbf{R}$. Khi đó $Y(\alpha)$ là một tập con liên thông của $B(C)$ (Ch. IV, Phụ lục).

b) Cho $Y$ là một tập con liên thông khác rỗng của $B(C)$. Khi đó $\sum_{\beta \in Y} \beta$ thuộc về $\mathbf{R}$.

Để chứng minh a), ta có thể giả sử rằng $\alpha$ là dương. Ta lập luận bằng quy nạp theo $\mathrm{Card}(Y(\alpha))$, với mệnh đề là tầm thường nếu $\mathrm{Card}(Y(\alpha)) = 1$. Theo Mệnh đề 19, tồn tại $\beta \in B(C)$ sao cho $\alpha - \beta \in \mathbf{R}$. Gọi $p$ là số nguyên lớn nhất $\geqslant 0$ sao cho $\gamma = \alpha - p\beta \in \mathbf{R}$. Vì $\gamma - \beta \notin \mathbf{R}$ và $\gamma + p\beta \in \mathbf{R}$, nên $(\gamma|\beta) \neq 0$ (Mệnh đề 9); do đó $\beta$ được nối với ít nhất một phần tử của $Y(\gamma)$. Nhưng $Y(\alpha) = Y(\gamma) \cup \{\beta\}$, và $Y(\gamma)$ là liên thông theo giả thiết quy nạp. Vậy $Y(\alpha)$ là liên thông, điều này chứng minh a).

Bây giờ lấy $Y$ là một tập con liên thông không rỗng của $B(C)$; ta chứng minh bằng quy nạp theo $\mathrm{Card}(Y)$ rằng $\sum_{\beta \in Y} \beta$ là một nghiệm. Trường hợp $\mathrm{Card}(Y) \leqslant 1$ là tầm thường. Giả sử rằng $\mathrm{Card}(Y) \geqslant 2$. Vì $X$ là một rừng (Chương V, § 4, no. 8, Mệnh đề 8), $Y$ là một cây và có một đỉnh tận cùng $\beta$ (Chương IV, Phụ lục). Tập hợp $Y - \{\beta\}$ là liên thông, và một trong các phần tử của nó được nối với $\beta$. Theo giả thiết quy nạp, $\alpha = \sum_{\gamma \in Y - \{\beta\}} \gamma \in \mathbf{R}$, và vì $(\alpha|\beta) < 0$, suy ra rằng $\alpha + \beta \in \mathbf{R}$ (Định lý 1). Đpcm.

### 7. CÁC TẬP HỢP ĐÓNG CỦA CÁC NGHIỆM

#### Định nghĩa 4 {#lie-vi-s1-def-4 .statement}

Cho $P$ là một tập con của $\mathbf{R}$.

(i) $P$ được gọi là đóng nếu các điều kiện $\alpha \in P, \beta \in P, \alpha + \beta \in \mathbf{R}$ kéo theo $\alpha + \beta \in P$.

(ii) $P$ được gọi là parabol nếu $P$ là đóng và nếu $P \cup (-P) = \mathbf{R}$.

(iii) $P$ được gọi là đối xứng nếu $P = -P$.

#### Bổ đề 3 {#lie-vi-s1-lem-3 .statement}

Cho $C$ là một phòng của $\mathbf{R}$ và $P$ là một tập con đóng của $\mathbf{R}$ chứa $R_+(C)$ (theo ký hiệu của no. 6). Đặt $\Sigma = B(C) \cap (-P)$, và gọi $Q$ là tập hợp các nghiệm là các tổ hợp tuyến tính của các phần tử của $\Sigma$ với hệ số nguyên không dương. Khi đó, $P = R_+(C) \cup Q$.

Chỉ cần chứng minh rằng $P \cap (-R_+(C)) = Q$. Cho $-\alpha \in Q$. Khi đó $\alpha$ là tổng của $n$ phần tử của $\Sigma$. Ta chứng minh, bằng quy nạp theo $n$, rằng $-\alpha \in P$. Điều này hiển nhiên nếu $n = 1$. Nếu $n > 1$, thì theo Mệnh đề 19 của no. 6 ta có thể viết $\alpha = \beta + \gamma$ với $\gamma \in \Sigma$ và $\beta$ là tổng của $n - 1$ phần tử của $\Sigma$. Theo giả thiết quy nạp, $-\beta \in P$; vì $-\gamma \in P$ và vì $P$ là đóng, nên $-\alpha \in P$. Do đó, $Q \subseteq P \cap (-R_+(C))$. Ngược lại, cho $-\alpha \in P \cap (-R_+(C))$. Khi đó $\alpha$ là tổng của $p$ phần tử của $B(C)$. Ta chứng minh, bằng quy nạp theo $p$, rằng $-\alpha \in Q$. Điều này hiển nhiên nếu $p = 1$. Nếu $p > 1$, thì theo Mệnh đề 19, ta có thể viết $\alpha = \beta + \gamma$ với $\gamma \in B(C)$ và $\beta$ là một nghiệm là tổng của $p - 1$ phần tử của $B(C)$. Vì $-\gamma = \beta + (-\alpha)$ và vì $P$ là đóng, nên $-\gamma \in P$, do đó $\gamma \in \Sigma$. Hơn nữa, $-\beta = \gamma + (-\alpha)$ nên $-\beta \in P$ vì $P$ là đóng. Theo giả thiết quy nạp, $-\beta \in Q$, do đó $-\alpha = -\beta - \gamma \in Q$. Do đó, $P \cap (-R_+(C)) \subseteq Q$.

#### Mệnh đề 20 {#lie-vi-s1-prop-20 .statement}

*Cho $P$ là một tập con của $R$. Các điều kiện sau là tương đương*:

(i) $P$ *là parabolic*;
(ii) $P$ *là đóng và tồn tại một phòng $C$ của $R$ sao cho $P \supseteq R_+(C)$*;
(iii) *tồn tại một phòng $C$ của $R$ và một tập con $\Sigma$ của $B(C)$ sao cho $P$ là hợp của $R_+(C)$ và tập hợp $Q$ gồm các nghiệm là các tổ hợp tuyến tính của các phần tử của $\Sigma$ với các hệ số nguyên không dương*.

(ii) $\Longrightarrow$ (iii): điều này suy ra từ Bổ đề 3.

(iii) $\Longrightarrow$ (i): ta áp dụng các giả thiết và ký hiệu của (iii). Rõ ràng là $P \cup (-P) = R$. Ta chứng minh rằng, nếu $\alpha, \beta \in P$ sao cho $\alpha + \beta \in R$, thì $\alpha + \beta \in P$. Điều này là hiển nhiên nếu nghiệm $\alpha + \beta$ là dương. Giả sử rằng $\alpha + \beta$ là âm. Khi đó $\alpha + \beta = \sum_{\gamma \in B(C)} n_\gamma \gamma$, với $n_\gamma \leq 0$. Nhưng hệ số của mọi phần tử $\gamma$ của $B(C) - \Sigma$ trong $\alpha$ hoặc $\beta$ là $\geq 0$; do đó $n_\gamma = 0$ nếu $\gamma \in B(C) - \Sigma$, vậy $\alpha + \beta \in Q \subseteq P$.

(i) $\Longrightarrow$ (ii): giả sử rằng $P$ là parabol. Cho $C$ là một phòng sao cho $\mathrm{Card}(P \cap R_+(C))$ là lớn nhất có thể. Cho $\alpha \in B(C)$ và giả sử rằng $\alpha \in P$, sao cho $-\alpha \in P$. Với mọi $\beta \in P \cap R_+(C)$, $\beta$ không tỷ lệ với $\alpha$ (vì giả thiết $\beta = 2\alpha$ sẽ kéo theo $\alpha = 2\alpha + (-\alpha) \in P$ do $P$ đóng). Do đó $s_\alpha(\beta) \in R_+(C)$ (no. 6, Hệ quả 1 của Mệnh đề 17). Nếu đặt $C' = s_\alpha(C)$, thì $\beta = s_\alpha(s_\alpha(\beta)) \in s_\alpha(R_+(C)) = R_+(C)$, vậy $-\alpha \in P \cap R_+(C')$ và do đó $\mathrm{Card}(P \cap R_+(C')) > \mathrm{Card}(P \cap R_+(C))$. Điều này là vô lý, vì $\alpha \in P$. Do đó $B(C) \subseteq P$, và do đó $R_+(C) \subseteq P$ theo Mệnh đề 19 và do $P$ đóng.

#### Hệ quả 1 {#lie-vi-s1-prop-20-cor-1 .statement}

*Cho $P$ là một tập con của $R$. Các điều kiện sau là tương đương*:

(i) *tồn tại một phòng $C$ sao cho $P = R_+(C)$*;
(ii) *$P$ đóng và $\{P, -P\}$ là một phân hoạch của $R$*.

*Phòng $C$ sao cho $P = R_+(C)$ khi đó là duy nhất*.

Nếu $P = R_+(C)$, $C$ là tập hợp các $x^* \in V^*$ sao cho $\langle x^*, x \rangle > 0$ với mọi $x \in P$, do đó $C$ có tính duy nhất.

#### Hệ quả 2 {#lie-vi-s1-prop-20-cor-2 .statement}

*Giả sử rằng $V$ được trang bị cấu trúc của một không gian vectơ có thứ tự sao cho, đối với cấu trúc này, mọi nghiệm của $R$ đều là dương hoặc âm. Cho $P$ là tập hợp các nghiệm dương đối với cấu trúc này. Khi đó tồn tại duy nhất một phòng $C$ của $R$ sao cho $P = R_+(C)$*.

Quả thực, $P$ thỏa mãn điều kiện (ii) của Hệ quả 1.

Hệ quả này đặc biệt áp dụng khi cấp đang được xét là toàn phần, khi đó điều kiện trên $R$ được thỏa mãn một cách tự động. Nhắc lại rằng một cấp như vậy có thể thu được, chẳng hạn, bằng cách chọn một cơ sở $(e_i)_{1 \leq i \leq n}$ của $V$ và lấy cấp từ điển trên $V$, sao cho $x = \sum_i \xi_i e_i$ là $\geq 0$ nếu tất cả các $\xi_i$ đều là 0, hoặc nếu $\xi_i > 0$ với chỉ số nhỏ nhất $i$ sao cho $\xi_i \neq 0$.

#### Hệ quả 3 {#lie-vi-s1-prop-20-cor-3 .statement}

*Một tập con B của R là một cơ sở của R khi và chỉ khi các điều kiện sau được thỏa mãn:*

(i) *các phần tử của B độc lập tuyến tính;*
(ii) *mọi nghiệm của R là một tổ hợp tuyến tính của các phần tử của B trong đó các hệ số hoặc đều dương hoặc đều âm;*
(iii) *mọi nghiệm của B là không phân chia được.*

Ta đã biết rằng các điều kiện là cần thiết (no. 5, Định lý 2, và no. 6, Định lý 3). Giả sử rằng các điều kiện (i), (ii), (iii) được thỏa mãn. Gọi P là tập hợp các nghiệm là các tổ hợp tuyến tính của các phần tử của B với các hệ số $\geq 0$. Vì P thỏa mãn điều kiện (ii) của Hệ quả 1, tồn tại một phòng C sao cho $P = R_+(C)$; đặt $B' = B(C)$, và gọi X và $X'$ là các nón lồi sinh bởi B và $B'$. Khi đó

$$
B \subseteq P \subseteq X \quad \text{và} \quad B' \subseteq P \subseteq X',
$$

điều này cho thấy X và $X'$ đều được sinh bởi P, và do đó trùng nhau. Nhưng các nửa đường thẳng sinh bởi các phần tử của B (tương ứng bởi $B'$) là các phần tử sinh cực biên của X (tương ứng của $X'$); vì một nửa đường thẳng như vậy chỉ chứa một nghiệm không phân chia được, nên $B = B'$.

#### Hệ quả 4 {#lie-vi-s1-prop-20-cor-4 .statement}

*Cho B là một cơ sở của R, $B'$ là một tập con của B, $V'$ là không gian con vectơ của V sinh bởi $B'$, và $R' = R \cap V'$. Khi đó $B'$ là một cơ sở của hệ nghiệm $B'$.*

Điều này suy ra ngay lập tức từ Hệ quả 3 và Hệ quả của Mệnh đề 4.

Ta gọi $R'$ là hệ nghiệm *sinh* bởi $B'$.

#### Hệ quả 5 {#lie-vi-s1-prop-20-cor-5 .statement}

*Cho B là một cơ sở của R, $A_1, A_2, \ldots, A_r$ là các tập con của B trực giao từng đôi một, và $A = A_1 \cup A_2 \cup \cdots \cup A_r$. Khi đó mọi nghiệm $\alpha$ là một tổ hợp tuyến tính của các phần tử của A thực sự là một tổ hợp tuyến tính của các phần tử của một trong các $A_i$. Đặc biệt, nếu R là bất khả quy, không có phân hoạch nào của B thành các tập con trực giao từng đôi một.*

Gọi $E_1, \ldots, E_r, E$ là các không gian con vectơ của V lần lượt sinh bởi $A_1, \ldots, A_r, A$. Theo Hệ quả 4, ta có thể giả sử rằng $E = V$. Khi đó, theo Định lý 2 (vii) của no. 5, các $E_i$ ổn định dưới tác động của $W(R)$, do đó R là hợp của các $R \cap E_i$ (no. 2, Mệnh đề 5).

#### Hệ quả 6 {#lie-vi-s1-prop-20-cor-6 .statement}

*Ta chấp nhận các giả thiết và ký hiệu của Mệnh đề 20. Gọi $V_1$ là không gian con vectơ của V sinh bởi $\Sigma$. Khi đó $P \cap (-P) = Q \cup (-Q) = V_1 \cap R$ là một hệ nghiệm trong $V_1$ với cơ sở $\Sigma$.*

Ta có $P \cap (-P) = (R_+(C) \cup Q) \cap ((-R_+(C)) \cup (-Q)) = Q \cup (-Q)$. Định lý 3 chứng minh rằng $Q \cup (-Q) = V_1 \cap R$. Cuối cùng, $\Sigma$ là một cơ sở của hệ nghiệm $V_1 \cap R$ theo Hệ quả 4.

#### Mệnh đề 21 {#lie-vi-s1-prop-21 .statement}

*Cho C (tương ứng $C'$) là một buồng của R, $\Sigma$ (tương ứng $\Sigma'$) là một tập con của $B(C)$ (tương ứng $B(C')$), Q (tương ứng $Q'$) là tập hợp các tổ hợp tuyến tính của các phần tử của $\Sigma$ (tương ứng $\Sigma'$) với các hệ số nguyên âm, và $P = Q \cup R_+(C)$ (tương ứng $P' = Q' \cup R_+(C')$). Nếu tồn tại một phần tử của nhóm Weyl biến đổi P thành $P'$, thì tồn tại một phần tử của nhóm Weyl biến đổi C thành $C'$ và $\Sigma$ thành $\Sigma'$.

Ta rút gọn ngay lập tức về trường hợp $P = P'$. Cho $V_1$ là không gian con vectơ của V sinh bởi $P \cap (-P)$. Khi đó $\Sigma$ và $\Sigma'$ là các cơ sở của hệ nghiệm $R_1 = P \cap (-P)$ trong $V_1$ (Hệ quả 6 của Mệnh đề 20). Do đó tồn tại $g_1 \in W(R_1)$ sao cho $g_1(\Sigma) = \Sigma'$. Rõ ràng $g_1$ được cảm sinh bởi một phần tử $g$ của $W(R)$ là tích của các phép đối xứng $s_\sigma$ với $\sigma \in \Sigma$. Cho $\gamma = \sum_{\beta \in B(C)} c_\beta \beta$ là một phần tử của $P - R_1$. Khi đó $c_\beta > 0$ với ít nhất một $\beta \in B(C) - \Sigma$. Hơn nữa, nếu $\sigma \in \Sigma$, thì $s_\sigma(\gamma) - \gamma \in V_1$, do đó $s_\sigma(\gamma)$ có ít nhất một tọa độ $> 0$ đối với $B(C)$ (no. 1, công thức (5)), suy ra $s_\sigma(\gamma) \in R_+(C)$ và cuối cùng $s_\sigma(\gamma) \in P - R_1$. Suy ra $P - R_1$ ổn định dưới các $s_\sigma, \sigma \in \Sigma$, và do đó dưới g, nên $g(P) = P$. Vì vậy ta quy về việc chứng minh mệnh đề trong trường hợp $P = P'$ và $\Sigma = \Sigma'$. Trong trường hợp này, $Q = Q'$, do đó $R_+(C) = P - Q = P - Q' = R_+(C')$, và vì thế $C = C'$ (Hệ quả 1 của Mệnh đề 20).

#### Hệ quả {#lie-vi-s1-n7-cor-1 .statement}

*Cho P, $P'$ là hai tập con parabolic của R được biến đổi thành nhau bởi một phần tử của nhóm Weyl. Nếu tồn tại một buồng C của R sao cho $R_+(C) \subseteq P$ và $R_+(C) \subseteq P'$, thì $P = P'$.

Điều này suy ra từ Bổ đề 3 và Mệnh đề 21 vì phần tử duy nhất của $W(R)$ biến đổi C thành C là 1, xem no. 5, Định lý 2.

#### Mệnh đề 22 {#lie-vi-s1-prop-22 .statement}

*Cho P là một tập hợp đóng của R sao cho $P \cap (-P) = \varnothing$. Khi đó tồn tại một buồng C của R sao cho $P \subseteq R_+(C)$.

1) Theo Hệ quả của Định lý 1, no. 3, các giả thiết $\alpha \in P, \beta \in P, (\alpha|\beta) < 0$ kéo theo $\alpha + \beta \in P$.

2) Ta chứng minh rằng không có tổng nào $\alpha_1 + \cdots + \alpha_q$ ($q \geqslant 1$) của các phần tử của P là không. Ta tiến hành bằng quy nạp theo $q$. Mệnh đề hiển nhiên đối với $q = 1$, giả sử rằng $q \geqslant 2$. Nếu $\alpha_1 + \cdots + \alpha_q = 0$, thì

$$
-\alpha_1 = \alpha_2 + \cdots + \alpha_q,
$$

do đó $(-\alpha_1|\alpha_2 + \cdots + \alpha_q) > 0$, suy ra tồn tại $j \in \{2, q\}$ sao cho $(\alpha_1|\alpha_j) < 0$. Theo phần 1) của chứng minh, $\alpha_1 + \alpha_j \in P$, và quan hệ $(\alpha_1 + \alpha_j) + \sum_{i \neq 1, j} \alpha_i = 0$ mâu thuẫn với giả thiết quy nạp.

3) Ta chứng minh rằng tồn tại một phần tử khác không $\gamma$ trong $V$ sao cho $(\gamma|\alpha) \geqslant 0$ với mọi $\alpha \in P$. Nếu không, kết quả của 1) sẽ cho thấy rằng có thể tìm được một dãy vô hạn $\alpha_1, \alpha_2, \ldots$ các phần tử của $P$ sao cho
$$
\beta_i = \alpha_1 + \cdots + \alpha_i \in P
$$
với mọi $i$; sẽ tồn tại hai số nguyên phân biệt $i, j$ sao cho $\beta_i = \beta_j$, điều này sẽ mâu thuẫn với kết quả của 2).

4) Để chứng minh mệnh đề, chỉ cần (Hệ quả 2 của Mệnh đề 20) chỉ ra rằng tồn tại một cơ sở $(\alpha_k)_{1 \leq k \leq l}$ của $V$ sao cho, đối với thứ tự từ điển được xác định bởi cơ sở này, mọi phần tử của $P$ đều $> 0$. Ta tiến hành bằng quy nạp theo $l = \dim V$, và giả sử rằng mệnh đề đã được thiết lập cho mọi số chiều $< l$. Cho $\gamma \in V$ là sao cho $\gamma \neq 0$ và $(\gamma|\alpha) \geqslant 0$ với mọi $\alpha \in P$ (xem 3)). Gọi $L$ là siêu phẳng trực giao với $\gamma$, và $V'$ là không gian con của $L$ sinh bởi $R \cap L$. Khi đó $R \cap L$ là một hệ nghiệm trong $V'$ và $P \cap L$ là đóng trong $R \cap L$. Theo giả thiết quy nạp, tồn tại một cơ sở $(\beta_1, \ldots, \beta_{l'})$ của $V'$ sao cho các phần tử của $P \cap L$ là $> 0$ đối với thứ tự từ điển được xác định bởi cơ sở này. Khi đó mọi cơ sở của $V$ mà $l' + 1$ phần tử đầu tiên là $\gamma, \beta_1, \ldots, \beta_{l'}$ và các phần tử còn lại thuộc $L$ đều có tính chất cần có.

#### Mệnh đề 23 {#lie-vi-s1-prop-23 .statement}

*Cho $P$ là một tập con của $R$ và $V_1$ (tương ứng $\Gamma$) là không gian con vectơ (tương ứng nhóm con) của $V$ sinh bởi $P$. Các điều kiện sau là tương đương:*

(i) *P là đóng và đối xứng;*
(ii) *P là đóng, và P là một hệ nghiệm trong $V_1$;*
(iii) $\Gamma \cap R = P$.

*Giả sử rằng các điều kiện này được thỏa mãn. Với mọi $\alpha \in P$, gọi $\alpha_1 \tilde{}$ là hạn chế của $\alpha \tilde{}$ lên $V_1$. Khi đó ánh xạ $\alpha \mapsto \alpha_1 \tilde{}$ là song ánh chính tắc từ hệ nghiệm $P$ đến $P \tilde{}$.*

(iii) $\Longrightarrow$ (i): hiển nhiên.

(i) $\Longrightarrow$ (ii): giả sử rằng $P$ đóng và đối xứng. Trước hết, $P$ thỏa mãn (RS_I) trong $V_1$. Ta chứng minh rằng, nếu $\alpha, \beta \in P$, thì $s_\alpha(\beta) \in P$. Điều này hiển nhiên nếu $\alpha$ và $\beta$ tỉ lệ. Nếu không, $s_\alpha(\beta) = \beta - n(\beta, \alpha)\alpha$ và $\beta - p\alpha \in R$ với mọi số nguyên hữu tỉ $p$ nằm giữa 0 và $n(\beta, \alpha)$ (Mệnh đề 9, no. 3), do đó
$$
\beta - n(\beta, \alpha)\alpha \in P
$$
vì $P$ đóng và đối xứng. Vậy, $s_{\alpha, \alpha_1}(P) = P$, và $P$ thỏa mãn (RS_{II}). Hiển nhiên rằng $P$ thỏa mãn (RS_{III}). Vậy, $P$ thỏa mãn (ii), và đồng thời ta đã chứng minh khẳng định cuối cùng của mệnh đề.

(ii) $\Longrightarrow$ (iii): ta chứng minh rằng, nếu điều kiện (ii) được thỏa mãn, thì $\Gamma \cap R = P$. Hiển nhiên rằng $P \subseteq \Gamma \cap R$. Cho $\beta \in \Gamma \cap R$. Vì $\beta \in \Gamma$ và $P = -P$, ta có $\beta = \alpha_1 + \alpha_2 + \cdots + \alpha_k$ với $\alpha_1, \ldots, \alpha_k \in P$. Ta sẽ chứng minh rằng $\beta \in P$. Điều này hiển nhiên nếu $k = 1$. Ta lập luận bằng quy nạp theo $k$. Ta có

$$
0 < (\beta|\beta) = \sum_{i=1}^{k} (\beta|\alpha_i),
$$
nên $(\beta|\alpha_i) > 0$ với một chỉ số $i$ nào đó. Nếu $\beta = \alpha_i$, thì $\beta \in P$. Nếu không, $\beta - \alpha_i \in R$ (Hệ quả của Định lý 1, no. 3), do đó $\beta - \alpha_i \in P$ theo giả thiết quy nạp, suy ra $\beta \in P$ vì $P$ đóng.

Các điều kiện của Mệnh đề 23 có thể được thực hiện với $V_1 = V$ nhưng vẫn có $P \neq R$. Ví dụ, đây là trường hợp khi $R$ là một hệ kiểu $G_2$ và $P$ là một hệ kiểu $A_2$; cf. Bản X.

#### Mệnh đề 24 {#lie-vi-s1-prop-24 .statement}

*Cho $R'$ là giao của $R$ với một không gian con vectơ của $V$, sao cho $R'$ là một hệ nghiệm trong không gian con vectơ $V'$ mà nó sinh ra (cf. Hệ quả của Mệnh đề 4, no. 1). Cho $B'$ là một cơ sở của $R'$.*

(i) *Tồn tại một cơ sở của $R$ chứa $B'$.*
(ii) *$R'$ là tập hợp các phần tử của $R$ là các tổ hợp tuyến tính của các phần tử của $B'$.*

Mệnh đề (ii) là rõ ràng. Ta chứng minh (i). Cho $(\varepsilon_1, \varepsilon_2, \ldots, \varepsilon_l)$ là một cơ sở của $V$ sao cho $B' = (\varepsilon_{p+1}, \varepsilon_{p+2}, \ldots, \varepsilon_l)$. Thứ tự từ điển trên $V$ tương ứng với cơ sở này xác định một buồng $C$ của $R$. Rõ ràng rằng mọi phần tử của $B'$ đều là cực tiểu trong $R_+(C)$. Do đó $B' \subseteq B(C)$.

### 8. NGHIỆM CAO NHẤT

#### Mệnh đề 25 {#lie-vi-s1-prop-25 .statement}

*Giả sử rằng $R$ là bất khả quy. Cho $C$ là một buồng của $R$, và cho $B(C) = \{\alpha_1, \ldots, \alpha_l\}$ là cơ sở tương ứng.*

(i) *Tồn tại một nghiệm $\tilde{\alpha} = \sum_{i=1}^{l} n_i \alpha_i$ sao cho, với mọi nghiệm $\sum_{i=1}^{l} p_i \alpha_i$, ta có $n_1 \geq p_1, n_2 \geq p_2, \ldots, n_l \geq p_l$. Nói cách khác, $R$ có một phần tử lớn nhất đối với quan hệ thứ tự được xác định bởi $C$.*
(ii) *Ta có $\tilde{\alpha} \in \overline{C}$.*
(iii) *Ta có $(\tilde{\alpha}|\tilde{\alpha}) \geq (\alpha|\alpha)$ với mọi nghiệm $\alpha$.*
(iv) *Với mọi nghiệm dương $\alpha'$ không tỉ lệ với $\tilde{\alpha}$, ta có $n(\alpha', \tilde{\alpha}) = 0$ hoặc $1$.*

1) Cho $\alpha = \sum_{i=1}^{l} n_i \alpha_i$, $\beta = \sum_{i=1}^{l} p_i \alpha_i$ là hai nghiệm lớn nhất đối với quan hệ thứ tự được xác định bởi $C$. Ta sẽ chứng minh rằng $\alpha = \beta$, điều này sẽ thiết lập (i).

2) Nếu $(\alpha|\alpha_i) < 0$ với một chỉ số $i$ nào đó, suy ra rằng hoặc $\alpha + \alpha_i \in R$ hoặc $\alpha = -\alpha_i$ (Hệ quả của Định lý 1, no. 3), và cả hai khả năng đều vô lý do tính lớn nhất của $\alpha$. Vì vậy $(\alpha|\alpha_i) \geq 0$ với mọi $i$.

3) Nếu $\alpha < 0$, thì $\alpha < -\alpha$, điều này là vô lý. Do đó $n_i \geq 0$ với mọi $i$. Gọi $J$ là tập hợp các $i$ sao cho $n_i > 0$, và $J'$ là phần bù của $J$ trong $\{1, 2, \ldots, l\}$. Khi đó $J \neq \varnothing$. Nếu $J'$ không rỗng, tồn tại một $i \in J$ và một $i' \in J'$ sao cho $(\alpha_i|\alpha_{i'}) < 0$ (Hệ quả 5 của Mệnh đề 20, no. 7); khi đó ta có

$$(\alpha | \alpha_{i'}) = \sum_{i \in I} n_i (\alpha_i | \alpha_{i'}) < 0$$

vì $(\alpha_j | \alpha_k) \leq 0$ với mọi $j$ và $k$ phân biệt, điều này sẽ mâu thuẫn với 2). Do đó $J' = \varnothing$ và $n_i > 0$ với mọi $i$.

4) Ta có $(\beta | \alpha_i) \geq 0$ với mọi $i$ theo 2). Ta không thể có $(\beta | \alpha_i) = 0$ với mọi $i$ vì $\beta \neq 0$. Từ 3) ta suy ra rằng

$$(\beta | \alpha) = \sum_i n_i (\beta | \alpha_i) > 0.$$

Nếu $\gamma = \alpha - \beta \in \mathbf{R}$, thì hoặc $\alpha > \beta$ hoặc $\beta > \alpha$ (Đl. 3, no. 6), điều này mâu thuẫn với tính cực đại của $\alpha$ và $\beta$. Do đó $\alpha = \beta$ (Hệ quả của Đl. 1, no. 3).

5) Theo 2), $\tilde{\alpha} \in \overline{C}$. Ta sẽ chứng minh rằng $(\alpha' | \alpha') \leq (\tilde{\alpha} | \tilde{\alpha})$ với mọi $\alpha' \in \mathbf{R}$. Vì $\overline{C}$ là một miền cơ bản của $W(\mathbf{R})$, ta có thể giả sử rằng $\alpha' \in \overline{C}$. Ta có $\tilde{\alpha} - \alpha' \geq 0$, do đó $(\tilde{\alpha} - \alpha' | x) \geq 0$ với mọi $x \in \overline{C}$. Đặc biệt $(\tilde{\alpha} - \alpha' | \tilde{\alpha}) \geq 0$ và $(\tilde{\alpha} - \alpha' | \alpha') \geq 0$, suy ra $(\tilde{\alpha} | \tilde{\alpha}) \geq (\alpha' | \tilde{\alpha}) \geq (\alpha' | \alpha')$. Như vậy $n(\alpha', \tilde{\alpha})$ phải bằng 0, 1 hoặc -1 nếu $\alpha'$ không tỉ lệ với $\tilde{\alpha}$. Nếu $\alpha' \geq 0$, thì $(\tilde{\alpha} | \alpha') \geq 0$ theo 2), do đó $n(\alpha', \tilde{\alpha}) \geq 0$ và $n(\alpha', \tilde{\alpha})$ phải bằng 0 hoặc 1. Q.E.D.

#### Nhận xét {#lie-vi-s1-n8-rem-1 .statement}

Nghiệm

$$\tilde{\alpha} = \sum_i n_i \alpha_i$$

trong (i) được gọi là nghiệm cao nhất của $\mathbf{R}$ (đối với $C$). Chú ý rằng, theo (i), ta có $n_i \geq 1$ với mọi $i$.

### 9. CÁC TRỌNG LƯỢNG, CÁC TRỌNG LƯỢNG CĂN

Cho $l = \dim V$. Ký hiệu $Q(\mathbf{R})$ là nhóm con của $V$ sinh bởi $\mathbf{R}$; các phần tử của $Q(\mathbf{R})$ được gọi là các trọng lượng căn của $\mathbf{R}$. Theo Đl. 3 của no. 6, $Q(\mathbf{R})$ là một nhóm con rời rạc của $V$ có hạng $l$, và mọi cơ sở của $\mathbf{R}$ là một cơ sở của $Q(\mathbf{R})$.

Tương tự, nhóm $Q(\mathbf{R}^*)$ là một nhóm con rời rạc của $V^*$ có hạng $l$.

#### Mệnh đề 26 {#lie-vi-s1-prop-26 .statement}

*Tập hợp các $x \in V$ sao cho $\langle x, y^* \rangle \in \mathbf{Z}$ với mọi $y^* \in Q(\mathbf{R}^*)$ (hay, tương đương, với mọi $y^* \in \mathbf{R}^*$) là một nhóm con rời rạc $G$ của $V$ chứa $Q(\mathbf{R})$. Nếu $B'$ là một cơ sở của $\mathbf{R}^*$, thì cơ sở của $V$ đối ngẫu với $B'$ là một cơ sở của $G$*.

Cho $x \in V$. Ba tính chất sau là tương đương:

(i) $\langle x, y^* \rangle \in \mathbf{Z}$ với mọi $y^* \in Q(\mathbf{R}^*)$;
(ii) $\langle x, y^* \rangle \in \mathbf{Z}$ với mọi $y^* \in B'$;
(iii) các tọa độ của $x$ đối với cơ sở đối ngẫu của $B'$ thuộc $\mathbf{Z}$.

Từ đó suy ra rằng cơ sở đối ngẫu với $B'$ là một cơ sở của $G$. Mặt khác, (RSIII) chứng minh rằng $\mathbf{R} \subseteq G$, do đó $Q(\mathbf{R}) \subseteq G$.

Nhóm $G$ của Mệnh đề 26 được ký hiệu là $P(\mathbf{R})$, và các phần tử của nó được gọi là các trọng số của $\mathbf{R}$. Ta cũng có thể xét nhóm $P(\mathbf{R}^*)$ gồm các trọng số của $\mathbf{R}^*$.

$$
P(R)/Q(R), \quad P(\tilde{R})/Q(\tilde{R})
$$

là các nhóm hữu hạn đối ngẫu trên $\mathbf{Q}/\mathbf{Z}$, và do đó là đẳng cấu. Cấp chung của hai nhóm này được gọi là *chỉ số liên kết* của R (hoặc của $\tilde{R}$).

Nếu R là một tổng trực tiếp của các hệ nghiệm $R_i$, nhóm Q(R) (tương ứng P(R)) được đồng nhất một cách chính tắc với tổng trực tiếp của Q($R_i$) (tương ứng P($R_i$)).

#### Mệnh đề 27 {#lie-vi-s1-prop-27 .statement}

*Cho $R_1$ là một tập con của R, $Q_1$ là nhóm con của Q(R) được sinh bởi $R_1$, và $W_1$ là nhóm con của W(R) được sinh bởi các $s_\alpha$ ($\alpha \in R_1$). Nếu $p \in P(R)$ và $w \in W_1$, thì $p - w(p) \in Q_1$.*

Nếu $w = s_\alpha$ với $\alpha \in R_1$, thì

$$
p - w(p) = \langle p, \alpha^\vee \rangle \alpha \in \mathbf{Z}\alpha \subseteq Q_1.
$$

Nếu $w = s_{\alpha_1} s_{\alpha_2} \ldots s_{\alpha_r}$, với $\alpha_1, \ldots, \alpha_r \in R_1$, thì vẫn đúng rằng $p - w(p) \in Q_1$, như ta thấy bằng quy nạp theo r.

Nhóm A(R) giữ bất biến P(R) và Q(R), và do đó tác động trên nhóm thương P(R)/Q(R). Theo Mệnh đề 27, nhóm W(R) tác động tầm thường trên P(R)/Q(R). Chuyển qua nhóm thương, ta thấy rằng *nhóm thương* A(R)/W(R) (xem Mệnh đề 16, no. 5) *tác động một cách chính tắc trên* P(R)/Q(R).

### 10. CÁC TRỌNG SỐ CƠ BẢN, CÁC TRỌNG SỐ TRỘI

Giả sử rằng R là *rút gọn*. Cho C là một phòng của R, và cho B là cơ sở tương ứng của R. Vì R là rút gọn, $B^\vee = \{ \alpha^\vee \}_{\alpha \in B}$ là một cơ sở của $R^\vee$. Cơ sở *đối ngẫu* $(\overline{\omega}_\alpha)_{\alpha \in B}$ của $B^\vee$ do đó là một cơ sở của nhóm các trọng số; các phần tử của nó được gọi là các *trọng số cơ bản* (đối với B, hoặc đối với C); nếu các phần tử của B được ký hiệu bởi $(\alpha_1, \ldots, \alpha_l)$, thì các trọng số cơ bản tương ứng được ký hiệu bởi $(\overline{\omega}_1, \ldots, \overline{\omega}_l)$.

Cho $x \in V$. Khi đó, $x \in C$ khi và chỉ khi $\langle x, \alpha^\vee \rangle > 0$ với mọi $\alpha \in B$. Suy ra rằng C là tập hợp các tổ hợp tuyến tính của các $\overline{\omega}_\alpha$ với các hệ số $\geq 0$.

Các phần tử $n(\alpha, \beta) = \langle \alpha, \beta^\vee \rangle$ của ma trận Cartan là, với $\alpha$ cố định, các tọa độ của $\alpha$ đối với cơ sở $(\overline{\omega}_\beta)_{\beta \in B}$:

$$
\alpha = \sum_{\beta \in B} n(\alpha, \beta) \overline{\omega}_\beta.
$$

Do đó, ma trận Cartan là ma trận chuyển vị của ma trận của đơn ánh chính tắc

$$
Q(R) \to P(R)
$$

đối với các cơ sở B và $(\overline{\omega}_\alpha)_{\alpha \in B}$ của các $\mathbf{Z}$-môđun Q(R) và P(R).

Một trọng số $\overline{\omega}$ được gọi là *trội* nếu nó thuộc $\overline{C}$, nói cách khác nếu các tọa độ của nó đối với $(\overline{\omega}_\alpha)_{\alpha \in B}$ là các số nguyên $\geq 0$, hoặc tương đương nếu $g(\overline{\omega}) \leq \overline{\omega}$ với mọi $g \in W(R)$ (no. 6, Mệnh đề 18). Vì $\overline{C}$ là một miền cơ bản đối với $W(R)$ (Định lý 2), tồn tại, với mọi trọng số $\overline{\omega}$, một trọng số duy nhất $\overline{\omega}'$ sao cho $\overline{\omega}'$ là một biến đổi của $\overline{\omega}$ bởi $W(R)$.

Ta có
$$
\langle \overline{\omega}_\alpha, \beta^\vee \rangle = (\overline{\omega}_\alpha | \frac{2\beta}{(\beta|\beta)}) = \delta_{\alpha\beta}
$$
với $\alpha, \beta \in B$ ($\delta_{\alpha\beta}$ ký hiệu Kronecker), do đó
$$
s_\beta(\overline{\omega}_\alpha) = \overline{\omega}_\alpha - \delta_{\alpha\beta}\beta \quad \text{và} \quad (\overline{\omega}_\alpha |\beta) = \frac{1}{2}(\beta|\beta)\delta_{\alpha\beta}.
$$
Nói cách khác, $\overline{\omega}_\alpha$ *vuông góc với* $\beta$ *đối với* $\beta \neq \alpha$, *và phép chiếu vuông góc của nó lên* $R\alpha$ *là* $\frac{1}{2}\alpha$. Vì $\overline{\omega}_\alpha \in \overline{C}$, $(\overline{\omega}_\alpha |\overline{\omega}_\beta) \geqslant 0$ với $\alpha, \beta \in B$, nghĩa là góc $(\overline{\omega}_\alpha, \overline{\omega}_\beta)$ là nhọn hoặc là góc vuông. Các trọng số trội là các $\overline{\omega} \in V$ sao cho $2(\overline{\omega}|\alpha)/(|\alpha|\alpha)$ là một số nguyên $\geqslant 0$ với mọi $\alpha \in B$.

#### Mệnh đề 28 {#lie-vi-s1-prop-28 .statement}

*Cho* $B$ *là một cơ sở của* $R$, $B'$ *một tập con của* $B$, $V'$ *không gian con vectơ của* $V$ *sinh bởi* $B'$, $R' = R \cap V'$ *(là một hệ nghiệm trong* $V'$*),* $R'\tilde{}$ *hệ nghiệm nghịch đảo (được đồng nhất với ảnh chính tắc của* $R'$ *trong* $R'\tilde{}$), $V_1$ *phần bù trực giao của* $R'\tilde{}$ *trong* $V$, *và* $p$ *phép chiếu của* $V$ *lên* $V'$ *song song với* $V_1$. *Khi đó,* $Q(R') = Q(R) \cap V'$, $P(R') = p(P(R))$. *Tập hợp các trọng số trội của* $R'$ *là ảnh qua* $p$ *của tập hợp các trọng số trội của* $R$.

Thật vậy, $Q(R)$ là nhóm con của $V$ có cơ sở $B$, $Q(R')$ là nhóm con của $V'$ có cơ sở $B'$ (no. 7, Hệ quả 4 của Mệnh đề 20), từ đó $Q(R') = Q(R) \cap V'$ là ngay lập tức. Nếu $\overline{\omega} \in P(R)$ và $\alpha \in R'$, $\langle p(\overline{\omega}), \alpha^\vee \rangle = \langle \overline{\omega}, \alpha^\vee \rangle \in \mathbf{Z}$, nên $p(\overline{\omega}) \in P(R')$, và do đó $p(P(R)) \subseteq P(R')$. Nếu $\overline{\omega}' \in P(R')$, $\overline{\omega}'$ mở rộng thành một dạng tuyến tính $\overline{\omega}$ trên $V^*$ triệt tiêu trên $(B - B')\tilde{}$; ta có $\langle \overline{\omega}, \alpha^\vee \rangle \in \mathbf{Z}$ với mọi $\alpha \in B$, nên $\overline{\omega} \in P(R)$, và $\overline{\omega}' = p(\overline{\omega})$; do đó $P(R') \subseteq p(P(R))$. Vậy $P(R') = p(P(R))$, và mệnh đề về các trọng số trội được chứng minh theo cùng cách.

#### Mệnh đề 29 {#lie-vi-s1-prop-29 .statement}

*Cho* $\rho$ *là một nửa tổng của các nghiệm* $> 0$.

(i) $\rho = \sum_{\alpha \in B} \overline{\omega}_\alpha$; *đây là một phần tử của* $C$.
(ii) $s_\alpha(\rho) = \rho - \alpha$ *với mọi* $\alpha \in B$.
(iii) $(2\rho|\alpha) = (\alpha|\alpha)$ *với mọi* $\alpha \in B$.

Vì $R$ là rút gọn, ta có $s_\alpha(R_+(C) - \{\alpha\}) = R_+(C) - \{\alpha\}$ và $s_\alpha(\alpha) = -\alpha$ với $\alpha \in B$ (no. 6, Hệ quả 1 của Mệnh đề 17), do đó $s_\alpha(2\rho) = 2\rho - 2\alpha$. Vì $s_\alpha(\rho) = \rho - \langle \rho, \alpha^\vee \rangle$, ta thấy rằng
$$
\langle \rho, \alpha^\vee \rangle = 1 = \langle \sum_{\beta \in B} \overline{\omega}_\beta, \alpha^\vee \rangle.
$$
Suy ra, $\rho = \sum_{\beta} \overline{\omega}_\beta$, và do đó $\rho \in C$. Cuối cùng, (iii) tương đương với $\langle \rho, \alpha^\vee \rangle = 1$.

#### Hệ quả {#lie-vi-s1-n10-cor-1 .statement}

Gọi $\sigma$ là một nửa tổng của các phần tử $> 0$ của $R^-$ (đối với $B^-$). Với mọi $\alpha \in V$, tổng các tọa độ của $\alpha$ đối với cơ sở $B$ là $\langle \alpha, \sigma \rangle$. Nếu $\alpha \in R$, tổng này bằng $\frac{1}{2} \sum_{\beta \in R_+ (\mathbf{C})} n(\alpha, \beta)$.

Đổi chỗ vai trò của $R$ và $R^-$ ở trên, ta có $\langle \alpha, \sigma \rangle = 1$ với mọi $\alpha \in B$, do đó suy ra hệ quả.

### 11. PHÉP BIẾN ĐỔI COXETER

Cho $C$ là một ngăn của $R$, cho $\{ \alpha_1, \ldots, \alpha_l \}$ là cơ sở tương ứng của $R$, và đặt $c = s_{\alpha_1} \cdots s_{\alpha_l}$. Phần tử $c$ của $W$ được gọi là *phép biến đổi Coxeter* của $W$ xác định bởi $C$ và song ánh $i \mapsto \alpha_i$ (Ch. V, § 6, no. 1). Cấp $h$ của nó được gọi là *số Coxeter* của $W$ (hoặc của $R$).

#### Mệnh đề 30 {#lie-vi-s1-prop-30 .statement}

*Giả sử rằng $R$ là bất khả quy. Cho $m$ là một số nguyên giữa 1 và $h - 1$ và nguyên tố cùng nhau với $h$. Khi đó $\exp(\frac{2i\pi m}{h})$ là một trị riêng của $c$ có bội số 1.*

Đặc biệt, $m$ là một *số mũ* của $W$, xem Ch. V, § 6, no. 2.

Trước hết ta chứng minh một bổ đề:

#### Bổ đề 4 {#lie-vi-s1-lem-4 .statement}

*Với mọi $w \in W$, đa thức đặc trưng của $w$ có các hệ số nguyên.*

Ta biết (no. 6, Định lý 3) rằng $\{ \alpha_1, \ldots, \alpha_l \}$ là một cơ sở của nhóm con $Q(R)$ của $V$ được sinh bởi $R$. Vì $w$ giữ ổn định $Q(R)$, ma trận của nó đối với $\{ \alpha_1, \ldots, \alpha_l \}$ có các phần tử nguyên; do đó đa thức đặc trưng của nó có các hệ số nguyên.

Cho $P$ là đa thức đặc trưng của $c$. Bổ đề trên cho thấy các hệ số của $P$ là các số nguyên. Theo Chap. V, § 6, no. 2, Hệ quả 2 của Mệnh đề 3, nghiệm nguyên thủy thứ $h$ của đơn vị $z = \exp(\frac{2i\pi}{h})$ là một nghiệm đơn của $P$. Do đó, mọi *liên hợp* của $z$ trên $\mathbf{Q}$ cũng là một nghiệm đơn của $P$. Nhưng ta biết (*Đại số*, Chap. V) rằng các nghiệm nguyên thủy thứ $h$ của đơn vị là liên hợp trên $\mathbf{Q}$. Vậy tất cả chúng đều là các nghiệm đơn của $P$, điều này chứng minh mệnh đề.

#### Mệnh đề 31 {#lie-vi-s1-prop-31 .statement}

*Giả sử $R$ là bất khả quy và thu gọn, và đặt $\beta = n_1 \alpha_1 + \cdots + n_l \alpha_l$ là nghiệm cao nhất của $R$ (xem no. 8). Khi đó $n_1 + \cdots + n_l = h - 1$.*

Cho $R_+$ là tập hợp các nghiệm dương tương ứng với $C$. Khi đó (no. 10, Hệ quả của Mệnh đề 29):

$$
n_1 + \cdots + n_l = \frac{1}{2} \sum_{\alpha \in R_+} n(\beta, \alpha)
$$
$$
= 1 + \frac{1}{2} \sum_{\alpha \in R_+, \alpha \neq \beta} n(\beta, \alpha) = 1 + \sum_{\alpha \in R_+, \alpha \neq \beta} \frac{(\alpha | \beta)}{(\alpha | \alpha)}
$$

Theo no. 8, Mệnh đề 25 (iv), với mọi $\alpha \in R_+$ và $\alpha \neq \beta$, $n(\alpha, \beta) = 0$ hoặc 1, do đó $n(\alpha, \beta)^2 = n(\alpha, \beta)$, tức là $\frac{4(\alpha | \beta)^2}{(\beta | \beta)^2} = \frac{2(\alpha | \beta)}{(\beta | \beta)}$. Suy ra:

$$
n_1 + \cdots + n_l + 1 = 2 + 2 \sum_{\alpha \in R_+, \alpha \neq \beta} \frac{(\alpha | \beta)^2}{(\alpha | \alpha)(\beta | \beta)}
= 2 \sum_{\alpha \in R_+} \frac{(\alpha | \beta)^2}{(\alpha | \alpha)(\beta | \beta)} = (\beta | \beta)^{-1} \sum_{\alpha \in R} \left( \frac{\alpha}{\| \alpha \|} | \beta \right)^2.
$$

Theo Chap. V, § 6, no. 2, Hệ quả của Định lý 1,

$$
\sum_{\alpha \in R} \left( \frac{\alpha}{\| \alpha \|} | \beta \right)^2 = h(\beta | \beta)
$$

nên $n_1 + \cdots + n_l + 1 = h$.

#### Mệnh đề 32 {#lie-vi-s1-prop-32 .statement}

*Giả sử $R$ là bất khả quy, và mọi nghiệm đều có cùng độ dài. Cho $\alpha \in R$. Số phần tử của $R$ không trực giao với $\alpha$ là $4h - 6$.*

Cho $R'$ là tập hợp các nghiệm không tỉ lệ với và không trực giao với $\alpha$.
Theo Chap. V, § 6, no. 2, Hệ quả của Định lý 1,

$$
(\alpha | \alpha)^2 + (\alpha | -\alpha)^2 + \sum_{\beta \in R'} (\alpha | \beta)^2 = h(\alpha | \alpha)^2,
$$

tức là

$$
\sum_{\beta \in R'} (\alpha | \beta)^2 = (h - 2)(\alpha | \alpha)^2.
$$

Nếu $\beta \in R'$, thì $(\alpha | \beta) = \pm \frac{1}{2} (\alpha | \alpha)$ theo danh sách trong no. 3. Do đó

$$
\frac{1}{4} \operatorname{Card} R' = h - 2, \quad \operatorname{Card} R' = 4h - 8,
$$

và số nghiệm không trực giao với $\alpha$ là $\operatorname{Card} R' + 2 = 4h - 6$.

#### Mệnh đề 33 {#lie-vi-s1-prop-33 .statement}

*Giả sử $R$ là bất khả quy và thu gọn. Đặt $s_{\alpha_i} = s_i$, và cho $\Gamma$ là nhóm con của $W$ sinh bởi $c = s_1 \ldots s_l$.*

(i) *Cho $\theta_i = s_l s_{l-1} \ldots s_{i+1} (\alpha_i)$ ($i = 1, \ldots, l$). Khi đó, $\theta_i > 0, c(\theta_i) < 0$.*
(ii) *Nếu $\alpha$ là một nghiệm $> 0$ sao cho $c(\alpha) < 0$, thì $\alpha$ bằng một trong các $\theta_i$.*
(iii) *Họ $(\theta_i)_{1 \leq i \leq l}$ là một cơ sở của Q(R).*
(iv) *Cho $\Omega_i$ là quỹ đạo của $\theta_i$ dưới tác động của $\Gamma$. Các tập hợp $\Omega_i$ rời nhau từng đôi một, chúng là tất cả các quỹ đạo của $\Gamma$ trên $R$, và mỗi tập có $h$ phần tử.*

Trước hết, lưu ý rằng $(s_1, \ldots, s_l)$ là một *phân tích thu gọn* của $c$ (Chap. IV, § 1, no. 1) đối với tập hợp S của các $s_i$. Thật vậy, nếu không, sẽ tồn tại một tập con $X = S - \{ j \}$ gồm $l - 1$ phần tử của S sao cho $c \in W_X$, điều này mâu thuẫn với Hệ quả 2 của Mệnh đề 7 của Chap. IV, § 1, no. 8.

Áp dụng Hệ quả 2 của Mệnh đề 17 của no. 6 cho $c$ ta được các khẳng định (i) và (ii).

Gọi $Q_i$ là nhóm con của Q(R) được sinh bởi các $\alpha_j, j > i$. Ngay lập tức thấy rằng $Q_i$ ổn định dưới các $s_j, j > i$, và rằng $s_j (\alpha_i) = \alpha_i$ mod. $Q_i$ với $j > i$.
Do đó:

$$
\theta_i = s_l \ldots s_{i+1} (\alpha_i) = \alpha_i \text{ mod. } Q_i.
$$

Nói cách khác, tồn tại các số nguyên $c_{ij}$ sao cho
$$
\theta_i = \alpha_i + \sum_{j > i} c_{ij} \alpha_j.
$$
Phần (iii) suy ra ngay lập tức.

Cuối cùng, cho $\alpha$ là một nghiệm. Phần tử $\sum_{k=0}^{h-1} c^k(\alpha)$ là bất biến dưới $c$, và do đó bằng không (Chap. V, § 6, no. 2). Vì vậy các $c^k(\alpha)$ không thể đều có cùng dấu, và tồn tại một $k$ sao cho $c^k(\alpha) > 0$ và $c^{k+1}(\alpha) < 0$. Theo (ii), $c^k(\alpha)$ là một trong các $\theta_i$. Do đó mọi quỹ đạo của $\Gamma$ trên R đều là một trong các $\Omega_i$. Mở rộng $(x|y)$ thành một dạng Hermit trên $V \otimes \mathbf{C}$. Mỗi quỹ đạo của $\Gamma$ trong R có nhiều nhất $h$ phần tử, và theo các nhận xét trên, có nhiều nhất $l$ quỹ đạo phân biệt. Bây giờ (Chap. V, § 6, no. 2, Định lý 2, ii)), lực lượng của $R$ bằng $hl$, điều này ngay lập tức suy ra (iv).

### 12. DẠNG SONG TUYẾN TÍNH CHÍNH TẮC

Ta đã thấy (no. 1, Mệnh đề 3) rằng dạng song tuyến tính đối xứng
$$
(x, y) \mapsto B_R(x, y) = \sum_{\alpha \in R} \langle \alpha^*, x \rangle \langle \alpha^*, y \rangle
$$
trên $V$ là không suy biến và bất biến dưới $A(R)$. Đổi chỗ vai trò của $R$ và $R^*$, suy ra rằng dạng song tuyến tính đối xứng $(x^*, y^*) \mapsto B_{R^*}(x^*, y^*) = \sum_{\alpha \in R} \langle \alpha, x^* \rangle \langle \alpha, y^* \rangle$ trên $V^*$ là không suy biến và bất biến dưới $A(R)$.

Dạng nghịch đảo của $B_{R^*}$ (tương ứng $B_R$) trên $V$ (tương ứng $V^*$) sẽ được gọi là *dạng song tuyến tính chính tắc* trên $V$ (tương ứng $V^*$) và được ký hiệu bởi $\Phi_R$ (tương ứng $\Phi_{R^*}$). Nó không suy biến và bất biến dưới $A(R)$. Gọi $\sigma$ là đẳng cấu từ $V$ đến $V^*$ được xác định bởi $B_{R^*}$. Khi đó, với $x \in V$ và $y \in V$:
$$
\Phi_R(x, y) = B_{R^*}(\sigma(x), \sigma(y)) = \sum_{\alpha \in R} \langle \alpha, \sigma(x) \rangle \langle \alpha, \sigma(y) \rangle.
$$
Nhưng $\langle \alpha, \sigma(x) \rangle = B_{R^*}(\sigma(\alpha), \sigma(x)) = \Phi_R(\alpha, x)$. Do đó,
$$
\Phi_R(x, y) = \sum_{\alpha \in R} \Phi_R(\alpha, x) \Phi(\alpha, y).
$$
(16)
Theo Mệnh đề 7 của no. 2, $\Phi_R$ là dạng song tuyến tính đối xứng khác không duy nhất bất biến dưới $W(R)$ thỏa mãn đồng nhất thức (16).

Với $\beta \in R$, (16) cho
$$
\Phi_R(\beta, \beta) = \sum_{\alpha \in R} \Phi_R(\alpha, \beta)^2 = \frac{1}{4} \Phi_R(\beta, \beta)^2 \sum_{\alpha \in R} n(\alpha, \beta)^2,
$$
suy ra
$$
4 \Phi_R(\beta, \beta)^{-1} = \sum_{\alpha \in R} n(\alpha, \beta)^2.
$$
Hơn nữa, theo Bổ đề 2 của no. 1, ta có, với $x, y \in V$:

$$
B_R(x, y) = \sum_{\alpha \in R} \Phi_R \left( \frac{2\alpha}{\Phi_R(\alpha, \alpha)}, x \right) \left( \frac{2\alpha}{\Phi_R(\alpha, \alpha)}, y \right)
= 4 \sum_{\alpha \in R} \Phi_R(\alpha, x) \Phi_R(\alpha, y) \Phi_R(\alpha, \alpha)^{-2}.
$$

Suy ra rằng, nếu $R$ là *bất khả quy*, tồn tại một hằng $\gamma(R) > 0$ sao cho

$$
\sum_{\alpha \in R} \Phi_R(\alpha, x) \Phi_R(\alpha, y) \Phi_R(\alpha, \alpha)^{-2} = \gamma(R) \Phi_R(x, y).
$$ (18)

Theo định nghĩa của $\gamma(R)$, ta có $B_R(x, y) = 4\gamma(R) \Phi_R(x, y)$, do đó

$$
\Phi_{R^{\sim}}(x^*, y^*) = (4\gamma(R))^{-1} B_{R^{\sim}}(x^*, y^*)
$$

với $x^*, y^* \in V^*$. Điều này chứng minh rằng $\gamma(R) = \gamma(R^{\sim})$. Mặt khác, với $\beta \in R$,

$$
\Phi_{R^{\sim}}(\beta^{\sim}, \beta^{\sim}) = (4\gamma(R))^{-1} \sum_{\alpha \in R} \langle \beta^{\sim}, \alpha \rangle^2
= \gamma(R)^{-1} \sum_{\alpha \in R} \frac{\Phi_R(\alpha, \beta)^2}{\Phi_R(\beta, \beta)^2}
$$

do đó, theo (16),

$$
\Phi_{R^{\sim}}(\beta^{\sim}, \beta^{\sim}) = \gamma(R)^{-1} \Phi_R(\beta, \beta)^{-2} \Phi_R(\beta, \beta)
$$

hay cuối cùng

$$
\Phi_R(\beta, \beta) \Phi_{R^{\sim}}(\beta^{\sim}, \beta^{\sim}) = \gamma(R)^{-1}.
$$ (19)

Hơn nữa, nếu tất cả các nghiệm của $R$ có cùng độ dài $\lambda$ đối với $\Phi_R$, (16) và (18) cho thấy rằng

$$
\gamma(R) = \lambda^{-4}.
$$ (20)

Ngoài ra, nếu $h$ là số Coxeter của $W$, Hệ quả của Định lý 1 của Chương V, § 6, no. 2 cho thấy rằng:

$$
h \Phi_R(x, x) = \sum_{\alpha \in R} \left( x, \frac{\alpha}{\lambda} \right)^2 \text{ với mọi } x \in V.
$$

So sánh với (16), ta suy ra rằng

$$
\lambda = h^{-1/2} \quad \text{hoặc} \quad \gamma(R) = h^2.
$$ (21)

Cuối cùng, công thức (19) cho thấy rằng các nghiệm của $R^{\sim}$ có độ dài $\lambda$ đối với $\Phi_{R^{\sim}}$.

### Bài tập {#lie-vi-s1-exercises}

Tất cả các hệ nghiệm được xét dưới đây đều là tương đối với các không gian vectơ thực. Ta ký hiệu bởi $(x|y)$ một tích vô hướng bất biến dưới nhóm Weyl (xem no. 3).

Xem [các bài tập của § 1](exercises/s1/).
