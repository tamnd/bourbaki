---
book: int
book_title: Integration
chapter: VI
chapter_title: VECTORIAL INTEGRATION
section: 1
section_title: Integration of vector-valued functions
lang: vi
source: int-i-vi
pdf_pages: 0392-0409, 0447-0453
extraction: ocr
subsections:
    - "no": 1
      title: Scalarly essentially integrable functions
      page: 2
      pdf_page: 393
    - "no": 2
      title: Properties of the integral of a scalarly essentially integrable function
      page: 5
      pdf_page: 396
    - "no": 3
      title: Integrals of operators
      page: 7
      pdf_page: 398
    - "no": 4
      title: The property (GDF)
      page: 9
      pdf_page: 400
    - "no": 5
      title: Measurable mappings and scalarly measurable mappings
      page: 12
      pdf_page: 403
    - "no": 6
      title: 'Applications: I. Extension of a continuous function to a space of measures'
      page: 13
      pdf_page: 404
    - "no": 7
      title: 'Applications: II. Extension, to a space of measures, of a continuous function with values in a space of operators'
      page: 15
      pdf_page: 406
statements: 34
exercises: 27
content_sha256: 22b3ba1b78f67ee8eb2a7350f57ab1a78ce5ff438856797947f57797006e91ff
translated_from: content/en/int/VI/01_s1_integration_of_vector_valued_functions.md
source_content_sha256: 0b2c492b6e4f982a6b14689c7015f7e4bafa51b9eb3f437d2d4cdf8f4278da11
translation_model: gpt-5.4-mini
translation_run: translate-vi-e8985126
glossary_version: 34
glossary_terms_sha256: c57531ffad6aa436fb95f3cb45efdc386feb8da73177dd88db0c542f5089f5e1
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 1. TÍCH PHÂN CỦA CÁC HÀM NHẬN GIÁ TRỊ VECTƠ

Trong suốt tiết diện này, $\mu$ ký hiệu một độ đo dương trên T, và F một không gian vectơ Hausdorff lồi địa phương trên $\mathbf{R}$. Với mọi ánh xạ f từ T vào F, và mọi phần tử $z'$ của đối ngẫu $F'$ của F, ta ký hiệu bằng $\langle f, z' \rangle$ hoặc $\langle z', f \rangle$ hàm vô hướng $z' \circ f$ trên T. Ta sẽ nói rằng f có tính chất P *theo vô hướng* nếu, với mọi $z' \in F'$, $\langle z', f \rangle$ có tính chất P. Chẳng hạn, ta sẽ nói rằng $f$ là *khả tích gần như khắp nơi theo $\mu$ theo vô hướng* nếu, với mọi $z' \in F'$, $\langle z', f \rangle$ là khả tích gần như khắp nơi theo $\mu$.\footnote{Trường hợp đặc biệt $F = \mathcal{M}(X)$ ($X$ là một không gian compact địa phương), được trang bị tôpô mờ $\sigma(\mathcal{M}(X), \mathcal{K}(X))$, cho khái niệm 'khả tích gần như khắp nơi theo $\mu$ theo vô hướng', đối với một ánh xạ $f : T \to \mathcal{M}_+(X)$, được định nghĩa trong Ch. V, §3, No. 1.}

Chú ý rằng trong định nghĩa này, tôpô của F chỉ can thiệp thông qua trung gian của đối ngẫu $F'$ của F. Nếu một hàm f có tính chất P theo vô hướng, thì nó lại có tính chất P theo vô hướng khi tôpô của F được thay bởi bất kỳ tôpô lồi địa phương Hausdorff nào tương thích với tính đối ngẫu giữa F và $F'$.

### 1. Các hàm khả tích gần như khắp nơi theo vô hướng

Nếu f là một ánh xạ khả tích gần như khắp nơi theo $\mu$ theo vô hướng từ T vào F, thì ánh xạ $z' \mapsto \int \langle f(t), z' \rangle d\mu(t)$ là một dạng tuyến tính trên $F'$, nghĩa là một phần tử của đối ngẫu đại số $F'^*$.

#### Định nghĩa 1 {#int-vi-s1-def-1 .statement}

*Người ta gọi* tích phân của f theo $\mu$, *và ký hiệu bởi* $\int f d\mu$ *hoặc* $\int f(t) d\mu(t)$, *phần tử của* $F'^*$ *được xác định bởi*
$$
\left\langle z', \int f d\mu \right\rangle = \int \langle z', f \rangle d\mu
$$
*với mọi* $z' \in F'$.

Nếu f liên tục với giá compact, thì nó khả tích theo vô hướng và Định nghĩa 1 trùng với định nghĩa về tích phân của f đã cho trong Ch. III, §3, No. 1. Mặt khác, nếu F là một không gian Banach và f là khả tích gần như khắp nơi, thì f là khả tích gần như khắp nơi theo vô hướng và Định nghĩa 1 trùng với định nghĩa về tích phân của f đã cho trong chương V (Ch. V, §1, No. 3 và Ch. IV, §4, No. 2, Hệ quả 1 của Định lý 1).

#### Ví dụ {#int-vi-s1-n1-exa-1 .statement}

Cho $X$ là một không gian compact địa phương, $t \mapsto \lambda_t$ là một ánh xạ của $T$ vào không gian $\mathcal{M}(X)$ của các độ đo trên $X$. Nói rằng họ $t \mapsto \lambda_t$ là $\mu$-adequate có nghĩa là nó gồm các độ đo dương và rằng ánh xạ $t \mapsto \lambda_t$ khả tích gần như khắp nơi theo vô hướng đối với $\mu$ và $\mu$-đo được đối với tôpô $\sigma(\mathcal{M}(X), \mathcal{K}(X))$.\footnote{Đây là định nghĩa của 'µ-adequate' trong ấn bản thứ nhất của Chương 5 (Ch. V, 1st edn., §3, No. 1, Def. 1). Trong ấn bản thứ hai, mà chương trước là một bản dịch, thuật ngữ 'µ-adequate' định nghĩa một khái niệm yếu hơn (tổng quát hơn) (Ch. V, §3, No. 1, Def. 1); chính xác hơn, một họ khả tích gần như khắp nơi theo vô hướng đối với $\mu$ $t \mapsto \lambda_t$ các độ đo dương là $\mu$-adequate theo nghĩa của ấn bản thứ nhất của Chương V khi và chỉ khi nó là $\mu$-adequate theo nghĩa của ấn bản thứ hai và là mơ hồ $\mu$-đo được, tức là $\mu$-đo được đối với $\sigma(\mathcal{M}(X), \mathcal{K}(X))$ (Ch. V, §3, No. 1, Prop 2 b)). Hai định nghĩa là tương đương mỗi khi tôpô của $X$ có một cơ sở đếm được (*ibid*. Prop. 2 c)), điều này là trường hợp trong các áp dụng ở Chương VI (§3); do đó, về phần còn lại của chương, không phân biệt giữa hai cách hiểu của 'µ-adequate', và các tham chiếu đến ấn bản thứ nhất của Ch. V đã được thay bằng tương đương gần nhất của chúng trong ấn bản thứ hai.}

Tích phân theo $\mu$ là độ đo đã được ký hiệu $\int \lambda_t\, d\mu(t)$ trong Ch. V, §3, No. 1.

#### Nhận xét 1 {#int-vi-s1-n1-rem-1 .statement}

Nếu $F$ hữu hạn chiều, thì mọi ánh xạ từ $T$ vào $F$ khả tích gần như khắp nơi theo vô hướng đều khả tích (Ch. V, §1, No. 3). Tuy nhiên, trong trường hợp tổng quát, một hàm vô hướng không đáng kể trên một không gian compact $T$ thậm chí có thể không $\mu$-đo được (Exer. 12).

#### Nhận xét 2 {#int-vi-s1-n1-rem-2 .statement}

Rõ ràng là tích phân của $f$ chỉ phụ thuộc vào lớp của $f$ modulo không gian các ánh xạ của $T$ vào $F$ mà theo vô hướng là địa phương $\mu$-không đáng kể. Chú ý rằng một hàm $g$ vô hướng địa phương không đáng kể không nhất thiết bằng không hầu khắp nơi (Exer. 12). Tuy nhiên, điều này quả thật đúng khi trong $F'$ tồn tại một dãy $(\mathbf{z}'_n)$ trù mật đối với tôpô $\sigma(F', F)$: vì nếu $H_n$ là tập hợp không đáng kể địa phương của các điểm $t \in T$ sao cho $\langle g(t), \mathbf{z}'_n \rangle \neq 0$, thì hợp $H$ của các $H_n$ là không đáng kể địa phương và, với mọi $t \notin H$, ta có $\langle g(t), \mathbf{z}'_n \rangle = 0$ với mọi $n$, do đó $g(t) = 0$.

Cho $u$ là một ánh xạ tuyến tính liên tục của $F$ vào một không gian lồi địa phương Hausdorff $G$; chuyển vị $^t u$ của nó là một ánh xạ tuyến tính của $G'$ vào $F'$, và chuyển vị (đại số) $^t(^t u)$ là một ánh xạ tuyến tính của $F'^*$ vào $G'^*$, mở rộng $u$, mà ta cũng sẽ ký hiệu là $u$. Với quy ước này:

#### Mệnh đề 1 {#int-vi-s1-prop-1 .statement}

— *Nếu $f$ là một ánh xạ của $T$ vào $F$ mà khả tích gần như khắp nơi theo vô hướng đối với $\mu$, thì ánh xạ $u \circ f$ cũng khả tích gần như khắp nơi theo vô hướng đối với $\mu$ và*
$$
\int (u \circ f)\, d\mu = u \left( \int f\, d\mu \right).
$$
Với mọi $\mathbf{z}' \in G'$, $\langle \mathbf{z}', u \circ f \rangle = \langle ^t u(\mathbf{z}'), f \rangle$, do đó có khẳng định thứ nhất; khẳng định thứ hai suy ra từ công thức
$$
\left\langle \mathbf{z}', \int (u \circ f)\, d\mu \right\rangle = \int \langle \mathbf{z}', u \circ f \rangle\, d\mu = \left\langle ^t u(\mathbf{z}'), \int f\, d\mu \right\rangle = \left\langle \mathbf{z}', u \left( \int f\, d\mu \right) \right\rangle.
$$

Đặc biệt, nếu $f$ khả tích gần như khắp nơi theo vô hướng đối với $\mu$, thì nó vẫn khả tích gần như khắp nơi theo vô hướng đối với $\mu$ khi tôpô của $F$ được thay bằng một tôpô thô hơn.

#### Mệnh đề 2 {#int-vi-s1-prop-2 .statement}

— *Cho $f$ là một ánh xạ của $T$ vào $F$ mà khả tích gần như khắp nơi theo vô hướng đối với $\mu$. Với mọi hàm số vô hướng $g \geqslant 0$ là $\mu$-đo được và bị chặn, ánh xạ $t \mapsto g(t)f(t)$ (được ký hiệu $gf$ hoặc $fg$) của $T$ vào $F$ khả tích gần như khắp nơi theo vô hướng, $f$ khả tích gần như khắp nơi theo vô hướng đối với $(g \cdot \mu)$, và*
$$
\int f\, d(g \cdot \mu) = \int fg\, d\mu.
$$

Điều này là hệ quả trực tiếp của công thức $\langle \mathbf{z}', gf \rangle = g \langle \mathbf{z}', f \rangle$, với mọi $\mathbf{z}' \in F'$, và công thức $\int h d(g \cdot \mu) = \int hg d\mu$ đối với mọi hàm số vô hướng khả tích gần như khắp nơi đối với $\mu$ $h$ (Ch. V, §5, No. 3, Th. 1).

Rất nhiều mệnh đề về các hàm số vô hướng khả tích gần như khắp nơi có thể được chuyển nguyên văn thành các mệnh đề về các ánh xạ nhận giá trị vectơ khả tích gần như khắp nơi theo vô hướng. Trong số những điều quan trọng hơn, ta lưu ý đến các điều kiện để một hàm số khả tích gần như khắp nơi đối với một độ đo được xác định bởi một mật độ (Ch. V, §5, No. 3, Th. 1), hoặc đối với ảnh của một độ đo (Ch. V, §6, No. 2, Th. 1), hoặc đối với một độ đo cảm sinh (Ch. V, §7, No. 1, Th. 1), hoặc đối với tổng của một họ khả tổng các độ đo dương (Ch. V, §2, No. 2, Props. 1 and 3 and Cor. 3 of Prop. 1). Những phép chuyển này để lại cho bạn đọc.

Tuy nhiên, để thu được các mệnh đề tương ứng với các định lý về “tích phân kép” (Ch. V, §3, No. 3, Th. 1 và §8, No. 4, Th. 1 (định lý Lebesgue–Fubini)), cần tăng cường các giả thiết (xem Exer. 1); khi áp dụng các định lý đã dẫn ở trên cho từng hàm $\langle \mathbf{z}', f \rangle$, với $\mathbf{z}' \in F'$, ta thu được các mệnh đề sau:

#### Mệnh đề 3 {#int-vi-s1-prop-3 .statement}

— Cho $X$ là một không gian compact địa phương, $t \mapsto \lambda_t$ là một họ $\mu$-adequate$^3$ (Ch. V, §3, No. 1, Def. 1) các độ đo dương trên $X$, và đặt $\nu = \int \lambda_t d\mu(t)$. Cho $f$ là một ánh xạ từ $X$ vào $F$; giả sử rằng $1^\circ$ $f$ khả tích theo từng vô hướng đối với $\nu$; $2^\circ$ tồn tại một tập hợp không đáng kể địa phương $N \subset T$ sao cho, với mọi $t \notin N$, $f$ khả tích theo từng vô hướng đối với $\lambda_t$ và $\int f d\lambda_t \in F$. Khi đó, hàm $t \mapsto \int f d\lambda_t$, được xác định với $t \notin N$, là gần khắp khả tích theo từng vô hướng đối với $\mu$, và$^4$

$$
\int f(x) d\nu(x) = \int d\mu(t) \int f(x) d\lambda_t(x) .
$$

#### Mệnh đề 4 {#int-vi-s1-prop-4 .statement}

— Cho $T$ và $T'$ là hai không gian compact địa phương, $\mu$ (tương ứng $\mu'$) là một độ đo dương trên $T$ (tương ứng $T'$), $\nu = \mu \otimes \mu'$ là độ đo tích trên $X = T \times T'$. Cho $f$ là một ánh xạ của $X$ vào $F$. Giả sử rằng: $1^\circ$ $f$ khả tích theo từng vô hướng đối với $\nu$; $2^\circ$ tồn tại một tập hợp không đáng kể địa phương $N \subset T$ sao cho, với mọi $t \notin N$, ánh xạ $t' \mapsto f(t, t')$ khả tích theo từng vô hướng đối với $\mu'$, và $\int f(t, t') d\mu'(t') \in F$. Khi đó, hàm $t \mapsto \int f(t, t') d\mu'(t')$, được xác định với $t \notin N$, là gần khắp khả tích theo từng vô hướng đối với $\mu$ và$^4$

$$
\iint f(t, t') d\mu(t) d\mu'(t') = \int d\mu(t) \int f(t, t') d\mu'(t') .
$$

$^3$Chỉ cần giả sử rằng họ này gần khắp khả tích theo từng vô hướng đối với $\mu$, do đó mệnh đề đúng theo một trong hai cách hiểu của ' $\mu$-adequate'.
$^4$Đẳng thức như các phần tử của $F'^*$.

### 2. Các tính chất của nguyên của một hàm gần khắp khả tích theo từng vô hướng

#### Mệnh đề 5 {#int-vi-s1-prop-5 .statement}

— Cho $\mu$ là một độ đo dương bị chặn trên $T$, $S$ là một tập $\mu$-đo được mang $\mu$ (Ch. V, §5, No. 7, Định nghĩa 4), $f$ là một hàm khả tích theo từng giá trị vô hướng (*) với giá trị trong $F$. Cho $D$ là bao lồi đóng của $f(S)$ trong không gian $F'$* được trang bị tôpô $\sigma(F', F')$. Khi đó $\int f\, d\mu \in \mu(T)D$.

Vì $D$ là giao của các nửa không gian đóng chứa $f(S)$ (TVS, II, §5, No. 3, Hệ quả 1 của Mệnh đề 4), đủ để chứng minh rằng quan hệ $\langle f(t), z' \rangle \leq a$ với mọi $t \in S$ (với $z' \in F', a \in \mathbf{R}$) suy ra $\langle z', \int f\, d\mu \rangle \leq a \cdot \mu(T)$; nhưng vì $\int f\, d\mu = \int_S f\, d\mu$, điều này suy ra từ Ch. IV, §4, No. 2, Hệ quả 1 của Định lý 1.

#### Hệ quả {#int-vi-s1-n2-cor-1 .statement}

— Cho $\mu$ là một độ đo dương bị chặn trên $T$, $S$ là một tập $\mu$-đo được mang $\mu$, và $f$ là một ánh xạ của $T$ vào $F$, khả đo vô hướng theo $\mu$ và sao cho $f(S)$ được chứa trong một tập con lồi compact yếu $A$ của $F$. Khi đó $f$ khả tích vô hướng theo $\mu$, và $\int f\, d\mu \in \mu(T)A \subset F$.

Với mọi $z' \in F'$, $\langle z', f \rangle$ là $\mu$-đo được và bị chặn trên $S$, do đó khả tích, điều này chứng tỏ rằng $f$ khả tích vô hướng. Hơn nữa, vì $A$ compact trong $F_\sigma$, nên nó đóng trong $F'$*, và bao lồi đóng của $f(S)$ trong $F'$* được chứa trong $A$, do đó có hệ quả.

#### Mệnh đề 6 {#int-vi-s1-prop-6 .statement}

— Cho $f$ là một hàm khả tích gần như theo $\mu$ theo từng giá trị vô hướng với giá trị trong $F$, sao cho $\int f\, d\mu \in F$. Với mọi nửa chuẩn nửa liên tục dưới $q$ trên $F$,

$$
q\left( \int f\, d\mu \right) \leq \int^\bullet (q \circ f)\, d\mu .
$$

Cho $D$ là tập hợp các $z \in F$ sao cho $q(z) \leq 1$; $D$ là một tập đóng, lồi và chứa $0$, do đó $D = D^{oo}$ (TVS, II, §6, No. 3, Hệ quả 3 của Định lý 1). Do đó chỉ cần chứng minh rằng với mọi $z' \in D^\circ$, ta có $|\langle z', \int f\, d\mu \rangle| \leq \int^\bullet (q \circ f)\, d\mu$; nhưng điều này suy ra ngay từ thực tế rằng $|\langle z', f(t) \rangle| \leq q(f(t))$ với mọi $t \in T$.

Chú ý rằng hàm số $q \circ f$ có thể không đo được theo $\mu$ (Bài tập 12).

#### Mệnh đề 7 {#int-vi-s1-prop-7 .statement}

— Cho $f$ là một ánh xạ của $T$ vào $F$, khả tích vô hướng theo nghĩa cốt yếu đối với $\mu$, sao cho với mọi tập con compact $K$ của $T$, $f(K)$ được chứa

(*) Nhắc lại rằng, với một độ đo dương *bị chặn* $\mu$, các khái niệm hàm khả tích theo $\mu$ và hàm khả tích theo nghĩa cốt yếu đối với $\mu$ là như nhau (Ch. V, §1, No. 3, Hệ quả của Mệnh đề 9).

5 Ký hiệu ban đầu cho tích phân cốt yếu trên là $\overline{\int^*}$, được đổi thành $\int^\bullet$ trong ấn bản thứ hai của Ch. V.

trong một tập con compact yếu, cân bằng, lồi của F. Khi đó $\int f d\mu$ thuộc đối ngẫu kép $F''$ của F.

Với mọi tập con compact $K$ của $T$,

$$
\int f \varphi_K d\mu = \int (f \varphi_K) d(\varphi_K \cdot \mu);
$$

Hệ quả của Mệnh đề 5 có thể được áp dụng cho độ đo bị chặn $\varphi_K \cdot \mu$ và hàm $f \varphi_K$, do đó $\int f \varphi_K d\mu \in F$. Với mọi $z' \in F'$, $\langle z', f \rangle$ là khả tích theo $\mu$ theo nghĩa cốt yếu, do đó (Ch. V, §1, No. 3, Mệnh đề 10)

$$
\int \langle z', f \rangle d\mu = \lim_K \int \langle z', f \rangle \varphi_K d\mu,
$$

giới hạn được lấy theo tập có hướng tăng của các tập con compact của T. Suy ra rằng, đối với tập có hướng này, $\int f \varphi_K d\mu$ hội tụ đến $\int f d\mu$ theo tôpô $\sigma(F'^*, F')$. Bây giờ,

$$
\left| \left\langle z', \int f \varphi_K d\mu \right\rangle \right| = \left| \int \langle z', f \rangle \varphi_K d\mu \right| \leq \int |\langle z', f \rangle| d\mu,
$$

điều này chứng tỏ rằng tập các phần tử $\int f \varphi_K d\mu$ là một *tập con bị chặn* của $F_\sigma$, do đó cũng của F (TVS, IV, §1, No. 1, Mệnh đề 1). Mệnh đề 7 do đó là một hệ quả của bổ đề sau:

#### Bổ đề 1 {#int-vi-s1-lem-1 .statement}

*Bao đóng trong $F'^*$ (với tôpô $\sigma(F'^*, F')$) của mọi tập con bị chặn của F đều được chứa trong đối ngẫu kép $F''$.*

Vì, một tập con bị chặn của F được chứa trong tập đối cực (trong $F''$) của một lân cận của 0 trong đối ngẫu mạnh $F'$ của F, do đó tương đối compact trong $F''$ đối với $\sigma(F'', F')$ (TVS, III, §3, No. 5, Mệnh đề 7 và No. 4, Hệ quả 2 của Mệnh đề 4); vì $\sigma(F'', F')$ được cảm sinh bởi $\sigma(F'^*, F')$, nên bổ đề được chứng minh.

#### Hệ quả {#int-vi-s1-n2-cor-2 .statement}

*Giả sử F là nửa phản xạ, và cho f là một ánh xạ khả tích vô hướng theo nghĩa cốt yếu của T vào F sao cho, với mọi tập con compact K của T, $f(K)$ bị chặn. Khi đó $\int f d\mu$ thuộc F.*

Vì, mọi tập con bị chặn của F đều tương đối compact yếu (TVS, IV, §2, No. 2, Định lý 1), và $F = F''$.

#### Mệnh đề 8 {#int-vi-s1-prop-8 .statement}

*Cho $\mu$ là một độ đo dương bị chặn trên T, S là một tập đo được theo $\mu$ mang $\mu$, f là một ánh xạ đo được theo $\mu$ của T vào F, sao cho $f(S)$ được chứa trong một tập con đầy đủ, bị chặn, cân bằng lồi B của F. Khi đó, f khả tích vô hướng theo $\mu$ và $\int f d\mu \in \mu(T)B \subset F$.*

Vì $S$ là $\mu$-khả tích, tồn tại một phân hoạch của $S$ gồm một tập $\mu$-không đáng kể $N$ và một dãy $(K_n)$ các tập con compact sao cho hạn chế của $f$ trên từng $K_n$ là liên tục (Ch. IV, §4, No. 6, Hệ quả 3 của Định lý 4 và §5, No. 1, Định nghĩa 1); do đó $f(K_n)$ là một tập con compact của $F$. Bao lồi cân bằng đóng $B_n$ của $f(K_n)$ khi đó là tiền compact (TVS, II, §4, No. 1, Mệnh đề 3) và được chứa trong tập con đầy đủ $B$ của $F$, do đó nó compact, và *a fortiori* compact yếu. Do đó (Hệ quả của Mệnh đề 5) $f \varphi_{K_n}$ là $\mu$-khả tích theo vô hướng, và

$$
z_n = \int f \varphi_{K_n} d\mu \in \mu(K_n)B_n \subset \mu(K_n)B .
$$

Với mọi nửa chuẩn liên tục $p$ trên $F$, suy ra rằng

$$
p(z_n) \leq \mu(K_n) \cdot \sup_{x \in B} p(x) ;
$$

vì $B$ bị chặn và vì chuỗi có số hạng tổng quát $\mu(K_n)$ hội tụ và có tổng $\mu(T)$, ta thấy rằng dãy có số hạng tổng quát $s_n = z_1 + z_2 + \cdots + z_n$ là một dãy Cauchy trong tập con đầy đủ $\mu(T)B$ của $F$. Dãy này do đó hội tụ đến một phần tử $s$ của $\mu(T)B$; vì có thể giả sử rằng $f(t) = 0$ trên $T - S$, định lý Lebesgue áp dụng cho từng các hàm $\langle z', f \rangle$ ($z' \in F'$) chứng minh rằng $s = \int f d\mu$.

### 3. Tích phân của các toán tử

Cho $G$ và $H$ là hai không gian lồi địa phương Hausdorff trên $\mathbf{R}$, và bây giờ giả sử rằng $F$ là không gian $\mathcal{L}(G; H)$ của các ánh xạ tuyến tính liên tục từ $G$ vào $H$, được trang bị tôpô hội tụ *từng điểm*. Mọi dạng tuyến tính liên tục trên $F$ đều có thể được mở rộng thành một dạng tuyến tính liên tục trên không gian tích $H^G$ (TVS, II, §4, No. 1, Mệnh đề 2), do đó có thể viết $u \mapsto \sum_{i=1}^n \langle u(a_i), b'_i \rangle$, trong đó các $a_i$ (tương ứng các $b'_i$) là các phần tử của $G$ (tương ứng của đối ngẫu $H'$ của $H$). Nói rằng một ánh xạ $U$ của $T$ vào $F$ là khả tích một cách bản chất theo vô hướng nghĩa là, với mọi $a \in G$ và mọi $b \in H'$, hàm số vô hướng $t \mapsto \langle U(t) \cdot a, b' \rangle$ là khả tích một cách bản chất theo $\mu$.

#### Mệnh đề 9 {#int-vi-s1-prop-9 .statement}

*Cho $U$ là một ánh xạ khả tích một cách bản chất theo vô hướng của $T$ vào $F = \mathcal{L}_s(G; H)$. Để $\int U d\mu \in F$, cần và đủ rằng hai điều kiện sau được thỏa mãn:*

a) *Với mọi $x \in G$, $\int (U(t) \cdot x) d\mu(t) \in H$.*

b) *Với mọi tập con đều liên tục $B'$ của $H'$, tập các dạng tuyến tính $u_{y'} : x \mapsto \int \langle U(t) \cdot x, y' \rangle d\mu(t)$, trong đó $y'$ chạy trên $B'$, là đều liên tục.*

Các điều kiện a) và b) là cần thiết. Thật vậy, vì với mọi $x \in G$, ánh xạ $\tilde{x} : V \mapsto V \cdot x$ của $\mathcal{L}_s(G; H)$ vào $H$ là tuyến tính, nên thấy được (No. 1,

Mệnh đề 1) rằng $\widetilde{\mathbf{x}} \circ U : t \mapsto U(t) \cdot \mathbf{x}$ là khả tích theo nghĩa vô hướng và $\mu$-hầu khắp nơi, và rằng

$$
(1) \quad S \cdot \mathbf{x} = \int (U(t) \cdot \mathbf{x})\, d\mu(t),
$$

trong đó $S = \int U\, d\mu \in \mathcal{L}_s(G; H)$. Điều này chứng tỏ a). Hơn nữa, (1) cũng có thể viết

$$
(2) \quad \langle S \cdot \mathbf{x}, \mathbf{y}' \rangle = \int \langle U(t) \cdot \mathbf{x}, \mathbf{y}' \rangle\, d\mu(t) = \langle \mathbf{x}, u_{\mathbf{y}'} \rangle,
$$

nói cách khác ${}^t S \cdot \mathbf{y}' = u_{\mathbf{y}'}$. Vì $S$ liên tục, ${}^t S$ biến mỗi tập con đều liên tục của $H'$ thành một tập con đều liên tục của $G'$, do đó b).

Ngược lại, giả sử a) và b) đã được xác minh. Nhờ a), công thức (1) xác định một ánh xạ tuyến tính $S$ của $G$ vào $H$, và, với mọi $\mathbf{y}' \in H'$, ánh xạ này thỏa mãn (2) (No. 1, Mệnh đề 1); nhưng khi đó, điều kiện (b) cho biết rằng $S$ liên tục (TVS, II, §6, No. 4, Mệnh đề 5 và 6, và III, §3, No. 5, Mệnh đề 7), do đó $S \in \mathcal{L}_s(G; H)$. Cuối cùng, công thức (2) chứng tỏ rằng $S = \int U\, d\mu$.

#### Hệ quả {#int-vi-s1-n3-cor-1 .statement}

— *Điều kiện b) của Mệnh đề 9 được thỏa mãn trong mỗi một trong hai trường hợp sau*:

$1^\circ$ *Độ đo $\mu$ bị chặn, và nếu $S$ là giá đỡ của nó, thì $U(S)$ là một tập con đều liên tục của $\mathcal{L}(G; H)$*.

$2^\circ$ *Điều kiện a) của Mệnh đề 9 được thỏa mãn, không gian $G$ là barreled, và, với mọi tập con compact $K$ của $T$, $U(K)$ là một tập con bị chặn của $\mathcal{L}_s(G; H)$*.

Trước hết, ta đặt mình vào trường hợp $1^\circ$. Ta có thể tự hạn chế vào trường hợp $S = T$ (Ch. V, §7, No. 1, ĐL. 1). Khi đó, với mọi tập con đều liên tục $B'$ của $H'$, tồn tại một tập con đều liên tục, lồi, cân bằng và đóng yếu $A' \subset G'$ sao cho ${}^t U(t) \cdot \mathbf{y}' \in A'$ với mọi $\mathbf{y}' \in B'$ và mọi $t \in T$ (TVS, II, §6, No. 4, Mệnh đề 6). Vì $U$ khả tích theo nghĩa vô hướng đối với $\mu$, ánh xạ $t \mapsto {}^t U(t) \cdot \mathbf{y}'$ của $T$ vào không gian đối ngẫu $G'$ của $G$ được trang bị $\sigma(G', G)$, là khả tích theo nghĩa vô hướng đối với $\mu$, và ta có thể viết

$$
u_{\mathbf{y}'} = \int ({}^t U(t) \cdot \mathbf{y}')\, d\mu(t).
$$

Vì $A'$ là lồi và compact đối với $\sigma(G', G)$, Hệ quả của Mệnh đề 5 của No. 2 cho thấy $u_{\mathbf{y}'} \in \mu(T)A'$ với mọi $\mathbf{y}' \in B'$, điều đó chứng tỏ mệnh đề của ta.

Bây giờ ta đặt mình vào trường hợp $2^\circ$. Với mọi $\mathbf{y}' \in H'$ và mọi tập con compact $K$ của $T$, đặt

$$
u_{K, \mathbf{y}'} = \int \varphi_K(t) ({}^t U(t) \cdot \mathbf{y}')\, d\mu(t),
$$

một phần tử của đối ngẫu đại số $G^*$ của $G$. Vì $G$ là barreled, mọi tập con bị chặn của $\mathcal{L}_s(G; H)$ đều là đều liên tục (TVS, III, §4, No. 2, Th. 1); phần đầu của lập luận, áp dụng cho hàm $\varphi_K U$ và độ đo bị chặn $\varphi_K \cdot \mu$, cho thấy $u_{K, y'} \in G'$. Hơn nữa, đối với tôpô $\sigma(G^*, G)$, ta có $u_{y'} = \lim_{K} = u_{K, y'}$, trong đó giới hạn được lấy theo tập có hướng tăng của các tập con compact của $T$ (Ch. V, §1, No. 3, Prop. 10). Để kiểm tra điều kiện b) của Prop. 9, theo Prop. 9, chỉ cần chứng minh rằng ánh xạ tuyến tính $S$ của $G$ vào $H$ được định nghĩa bởi (1) là liên tục; hơn nữa, $G$ là barreled, do đó chỉ cần chứng minh rằng $S$ liên tục khi $G$ và $H$ được trang bị các tôpô suy yếu của chúng (TVS, IV, §1, No. 3, Prop. 7); cuối cùng, nhờ (2), ta quy về việc chứng minh rằng $u_{y'} \in G'$ với mọi $y' \in H'$. Vì $u_{y'}$ nằm trong bao đóng, đối với $\sigma(G^*, G)$, của tập $M'$ gồm các $u_{K, y'}$, trong đó $K$ chạy qua tập các tập con compact của $T$, chỉ cần chứng minh rằng $M'$ là đều liên tục (TVS, III, §3, No. 4, Prop. 4); và vì $G$ là barreled, điều đó tương đương với việc nói rằng với mọi $x \in G$, tập các $\langle x, u_{K, y'} \rangle$ là bị chặn (TVS, III, §4, No. 2, Th. 1). Nhưng điều này suy ra ngay từ các hệ thức

$$
|\langle x, u_{K, y'} \rangle| = \left| \int \varphi_K(t) \langle U(t) \cdot x, y' \rangle d\mu(t) \right| \leq \int |\langle U(t) \cdot x, y' \rangle| d\mu(t).
$$

#### Mệnh đề 10 {#int-vi-s1-prop-10 .statement}

— *Cho $U$ là một ánh xạ của $T$ vào $F = \mathcal{L}_s(G; H)$. Trong mỗi một trong ba trường hợp sau, $U$ khả tích theo vô hướng một cách hầu khắp theo $\mu$ và $\int U d\mu \in \mathcal{L}_s(G; H)$:*

a) $H$ là gần đầy đủ, $\mu$ bị chặn và, nếu $S$ là giá đỡ của nó, $U$ đo được theo $\mu$ và $U(S)$ là đều liên tục.

b) $H$ là nửa phản xạ, $\mu$ bị chặn và, nếu $S$ là giá đỡ của nó, $U$ đo được theo vô hướng theo $\mu$ và $U(S)$ là đều liên tục.

c) $H$ là nửa phản xạ, $G$ là barreled, $U$ khả tích theo vô hướng một cách hầu khắp theo $\mu$, và, với mọi tập con compact $K$ của $T$, $U(K)$ bị chặn.

Việc $U$ là khả tích thiết yếu theo vô hướng là hiển nhiên trong cả ba trường hợp; nhờ Mệnh đề 9 và hệ quả của nó, trong mỗi trường hợp chỉ cần kiểm tra điều kiện a) của Mệnh đề 9. Bây giờ, điều kiện này suy ra từ Mệnh đề 8 của Mục 2 trong trường hợp thứ nhất, và từ Hệ quả của Mệnh đề 7 của Mục 2 trong hai trường hợp còn lại.

### 4. Tính chất (GDF)

Trong mục này, ta sẽ xét các không gian lồi địa phương $F$ có tính chất sau đây (được gọi là tính chất “đồ thị đóng đếm được”):⁶

⁶ *Graphe dénombrablement fermé*, do đó có các chữ cái đầu (GDF).

(GDF) *Nếu u là một ánh xạ tuyến tính từ F vào một không gian Banach B sao cho, trong không gian tích F × B, mọi giới hạn của mọi dãy hội tụ các điểm của đồ thị Γ của u lại thuộc Γ, thì u liên tục.*

Mọi không gian Fréchet đều có tính chất (GDF) (TVS, I, §3, No. 3, Hệ quả 5 của Định lý 1). Trong Phụ lục, ta sẽ thấy các ví dụ khác về các không gian có tính chất (GDF).

#### Mệnh đề 11 {#int-vi-s1-prop-11 .statement}

*Mọi không gian lồi địa phương Hausdorff F có tính chất (GDF) đều là barreled.*

Cho V là một thùng trong F, q là hàm gauge, tức là một phiếm chuẩn trên F; gọi H là không gian Hausdorff liên kết với không gian F được trang bị tôpô do phiếm chuẩn duy nhất này xác định. Sự hoàn thiện $\widehat{H}$ của H là một không gian Banach; gọi $\pi$ là ánh xạ chính tắc của F vào $\widehat{H}$; ta sẽ chứng minh rằng $\pi$ là *liên tục* (đối với tôpô ban đầu trên F); điều này sẽ chứng minh mệnh đề, vì V, ảnh ngược qua $\pi$ của hình cầu đơn vị của $\widehat{H}$, khi đó sẽ là một lân cận của 0 trong F. Để chứng minh tính liên tục của $\pi$, nhờ (GDF), chỉ cần chứng minh rằng đồ thị của $\pi$ là *đóng* trong $F \times \widehat{H}$; nói cách khác, ta phải thấy rằng nếu $\mathcal{F}$ là một bộ lọc trên F, hội tụ tới $x \in F$, và ảnh của nó $\pi(\mathcal{F})$ hội tụ tới $y \in \widehat{H}$, thì $y = \pi(x)$. Bây giờ, mọi phần tử $x'$ của đối ngẫu $V^\circ$ của V trong $F'$ đều chỉ có thể được kéo dài theo đúng một cách thành một dạng tuyến tính liên tục trên $\widehat{H}$ (cũng ký hiệu là $x'$), và tập hợp các dạng này là hình cầu đơn vị của đối ngẫu của $\widehat{H}$; do đó chỉ cần chứng minh rằng $\langle y, x' \rangle = \langle \pi(x), x' \rangle$ với mọi $x' \in V^\circ$. Nhưng điều này suy ra từ các hệ thức

$$
\langle y, x' \rangle = \lim_{\mathcal{F}} \langle \pi(z), x' \rangle = \lim_{\mathcal{F}} \langle z, x' \rangle = \langle x, x' \rangle = \langle \pi(x), x' \rangle .
$$

#### Định lý 1 {#int-vi-s1-thm-1 .statement}

(Gelfand–Dunford)—*Cho F là một không gian lồi địa phương Hausdorff có tính chất (GDF), $F'_s$ là đối ngẫu yếu của nó. Với mọi ánh xạ f của T vào $F'_s$ sao cho f khả tích thiết yếu theo vô hướng $\mu$, tích phân $\int f d\mu$ thuộc $F'$. \*

Nhắc lại rằng đối ngẫu của $F'_s$ là F (TVS, II, §6, No. 2, Mệnh đề 3). Với mọi $z \in F$, hàm số thực $\langle z, f \rangle$ do đó là khả tích thiết yếu theo $\mu$; hãy gọi $\theta(z)$ là lớp của nó trong $L^1(\mu)$. Để chứng minh rằng $\int f d\mu \in F'$, cần thiết lập rằng dạng tuyến tính $z \mapsto \langle z, \int f d\mu \rangle$ là liên tục trên F; thật ra, ta sẽ chứng minh kết quả mạnh hơn sau đây:

#### Bổ đề 2 {#int-vi-s1-lem-2 .statement}

*Cho f là một ánh xạ của T vào $F'_s$, sao cho với mọi $z \in F$, hàm số thực $\langle z, f \rangle$ thuộc $\overline{\mathcal{L}}^p(\mu)$ ($1 \leq p \leq +\infty$); hãy gọi $\theta(z)$ là lớp của hàm này trong $L^p(\mu)$. Khi đó $z \mapsto \theta(z)$ là một ánh xạ tuyến tính liên tục của F vào $L^p(\mu)$.*

Nhờ tính chất (GDF), chỉ cần chứng minh rằng với mọi dãy $(z_n)$ gồm các phần tử của F hội tụ đến $z$, sao cho $(\theta(z_n))$ hội tụ đến $u \in L^p(\mu)$, ta có $u = \theta(z)$. Nếu cần, thay dãy $(z_n)$ bởi một dãy con, ta có thể giả sử rằng dãy các hàm $\langle z_n, f \rangle$ hội tụ địa phương hầu khắp nơi đến một hàm $h \in \overline{\mathcal{L}}^p(\mu)$, với lớp $u$ trong $L^p(\mu)$ (Ch. IV, §3, No. 4, Th. 3 và Ch. V, §1, No. 3). Vì, theo giả thiết, với mọi $t \in T$ dãy $(\langle z_n, f(t) \rangle)$ hội tụ đến $\langle z, f(t) \rangle$, nên ta có $h(t) = \langle z, f(t) \rangle$ địa phương hầu khắp nơi, do đó $u = \theta(z)$.

#### Hệ quả 1 {#int-vi-s1-lem-2-cor-1 .statement}

*Cho $G_i$ ($1 \leq i \leq n$) là $n$ không gian lồi địa phương Hausdorff có tính chất (GDF), và cho $F$ là không gian các dạng đa tuyến tính liên tục riêng rẽ trên $\prod_{i=1}^n G_i$, được trang bị tôpô hội tụ điểm. Với mọi ánh xạ $f$ của $T$ vào $F$ mà khả tích theo vô hướng một cách hầu khắp đối với $\mu$, ta có $\int f d\mu \in F$.*

Không gian $F$ ở trong đối ngẫu với tích tenxơ $\bigotimes_{i=1}^n G_i$, và tôpô hội tụ điểm trên $F$ chẳng qua là tôpô $\sigma(F, \bigotimes_{i=1}^n G_i)$. Do đó đối ngẫu đại số $F'^*$ là không gian của mọi dạng đa tuyến tính trên $\prod_{i=1}^n G_i$. Cho $z = (z_1, \ldots, z_n)$ là một phần tử của $\prod_{i=1}^n G_i$; với mọi dạng đa tuyến tính $u \in F'^*$, ánh xạ $x \mapsto u(z_1, \ldots, z_{i-1}, x, z_{i+1}, \ldots, z_n)$ là một dạng tuyến tính trên $G_i$, mà ta sẽ ký hiệu bởi $\lambda_i(z)(u)$; do đó ta thu được một ánh xạ tuyến tính $\lambda_i(z)$ của $F'^*$ vào đối ngẫu đại số $G_i^*$ của $G_i$, liên tục đối với các tôpô $\sigma(F'^*, \bigotimes_{i=1}^n G_i)$ và $\sigma(G_i^*, G_i)$. Nói rằng $u \in F$ có nghĩa là với mọi chỉ số $i$ và mọi $z \in \prod_{i=1}^n G_i$, ta có $\lambda_i(z)(u) \in G_i'$. Bây giờ, nhờ Mệnh đề 1 của No. 1, ánh xạ $\lambda_i(z)$ của $F$ là một ánh xạ khả tích theo vô hướng một cách hầu khắp đối với $\mu$ từ $T$ vào $G_i'$ được trang bị tôpô $\sigma(G_i', G_i)$, và
$$
\int (\lambda_i(z) \circ f) d\mu = \lambda_i(z) \left( \int f d\mu \right).
$$
Nhờ Định lý 1, $\int (\lambda_i(z) \circ f) d\mu \in G_i'$ với $1 \leq i \leq n$, do đó $\int f d\mu \in F$.

#### Hệ quả 2 {#int-vi-s1-lem-2-cor-2 .statement}

*Cho $G$ là một không gian tôpô lồi Hausdorff có tính chất (GDF), và $H$ là một không gian nửa phản xạ sao cho đối ngẫu mạnh $H_b'$ có tính chất (GDF) (xem App., No. 2, Mệnh đề 3). Cho $F$ là không gian $\mathcal{L}_s(G; H)$; với mọi ánh xạ $U$ của $T$ vào $F$ mà gần như khả tích theo vô hướng đối với $\mu$, tích phân $\int U d\mu$ thuộc $F$.

Vì $G$ là barreled (Mệnh đề 11), $\mathcal{L}(G; H) = \mathcal{L}(G_\sigma; H_\sigma)$ (TVS, IV, §1, No. 3, Mệnh đề 7); hơn nữa, có thể thay $F = \mathcal{L}_s(G; H)$ bằng không gian $\mathcal{L}_s(G_\sigma; H_\sigma)$, vì hai không gian có cùng đối ngẫu $G \otimes H'$ (TVS, II, §6, No. 2, Mệnh đề 3, và đoạn đầu tiên của No. 3 ở trên). Nếu, với mọi $u \in \mathcal{L}(G; H) = \mathcal{L}(G_\sigma; H_\sigma)$, ta đặt $\tilde{u}(x, y') = \langle u(x, y') \rangle$ (với $x \in G$, y' \in H' ), thì ánh xạ tuyến tính $u \mapsto \tilde{u}$ là một song ánh của F lên không gian $F_1$ các dạng song tuyến tính liên tục riêng rẽ trên $G_\sigma \times H'_s$, trong đó $H'_s$ ký hiệu đối ngẫu $H'$ được trang bị tôpô yếu $\sigma(H', H)$ (App., No. 1); hơn nữa, ánh xạ này là một đẳng cấu của $\mathcal{L}_s(G_\sigma; H_\sigma)$ lên $F_1$ được trang bị tôpô hội tụ từng điểm (*loc. cit.*). Nhưng vì theo giả thiết H là đối ngẫu của $H'_b$, $F_1$ cũng là không gian các dạng song tuyến tính liên tục riêng rẽ trên $G \times H'_b$. Do đó Hệ quả 2 suy ra từ Hệ quả 1.

Chú ý rằng Hệ quả 2 áp dụng đặc biệt khi G là *không gian Banach* và H là *không gian Banach phản xạ*.

### 5. Các ánh xạ đo được và các ánh xạ đo được theo vô hướng

Nếu một ánh xạ f của T vào một không gian tôpô lồi Hausdorff F là đo được theo vô hướng đối với $\mu$, thì nói chung không suy ra rằng f là $\mu$-đo được (Bài tập 12). Tuy nhiên:

#### Mệnh đề 12 {#int-vi-s1-prop-12 .statement}

*Nếu F là một không gian tôpô lồi địa phương tách được, metrizable, thì mọi ánh xạ f đo được theo vô hướng đối với $\mu$ của T vào F đều là $\mu$-đo được.*

Vì, F có thể được xem như một không gian con của một tích đếm được $\prod_n E_n$ các không gian Banach (TVS, II, §1, No. 3, Mệnh đề 3), và có thể giả sử rằng $\mathrm{pr}_n(F)$ trù mật trong $E_n$, do đó $E_n$ là tách được. Với mọi n, ánh xạ $\mathrm{pr}_n \circ f$ là đo được theo vô hướng đối với $\mu$, do đó $\mu$-đo được (Ch. IV, §5, No. 5, Hệ quả 2 của Mệnh đề 10), suy ra f là $\mu$-đo được (Ch. IV, §5, No. 3, Định lý 1).

#### Mệnh đề 13 {#int-vi-s1-prop-13 .statement}

*Cho F là một không gian tôpô lồi địa phương là giới hạn trực tiếp của một dãy các không gian tôpô lồi địa phương tách được, metrizable $F_n$, F là hợp của các $F_n$. Cho $F'$ là đối ngẫu của F, được trang bị tôpô $\sigma(F', F)$. Khi đó, mọi ánh xạ f đo được theo vô hướng đối với $\mu$ của T vào $F'$ đều là $\mu$-đo được.*

Giả sử trước hết rằng $F$ khả metric và separable, và cho $D$ là một tập đếm được trù mật trong $F$. Cho $(V_n)$ là một dãy nền giảm của các lân cận mở cân bằng, lồi của $0$ trong $F$; các tập đối cực $V_n^\circ$ là đều liên tục và hợp của chúng là toàn bộ $F'$. Đặt $T_n = f(V_n^\circ)$; dãy $(T_n)$ là tăng và $T = \bigcup T_n$; ta hãy chứng minh rằng mỗi $T_n$ đều là *đo được* theo $\mu$. Thật vậy, $D \cap V_n^n$ trù mật trong $V_n$; với mọi $y \in D \cap V_n$, cho $S_y$ là tập các $t \in T$ sao cho $|\langle y, f(t) \rangle| \leq 1$; giả thiết suy ra rằng mỗi $S_y$ đều đo được, và $T_n$ là giao của họ đếm được các $S_y$ ($y \in D \cap V_n$). Vì thế, với mọi tập con hữu hạn compact K của T và mọi $\varepsilon > 0$, tồn tại một số nguyên n sao cho $\mu(K - (K \cap T_n)) \leq \frac{\varepsilon}{4}$, rồi một tập con hữu hạn compact $K_1$ của $K \cap T_n$ sao cho $\mu((K \cap T_n) - K_1) \leq \frac{\varepsilon}{4}$; cuối cùng, tồn tại một tập con hữu hạn compact $K_2$ của $K_1$ sao cho $\mu(K_1 - K_2) \leq \frac{\varepsilon}{2}$ và sao cho các hạn chế lên $K_2$ của mọi hàm $\langle y, f \rangle$, với $y \in D$, đều liên tục (Ch. IV, §5, No. 1, Prop. 2). Vì tập $f(K_2) \subset f(T_n) \subset V_n^\circ$ là đều liên tục, tôpô cảm sinh bởi $\sigma(F', F)$ trên $f(K_2)$ trùng với tôpô hội tụ điểm trên $D$ (GT, X, §2, No. 4, Th. 1); do đó, hạn chế của $f$ lên $K_2$ là liên tục, suy ra mệnh đề của ta trong trường hợp thứ nhất.

Ta chuyển sang trường hợp tổng quát. Nếu $z'$ là một dạng tuyến tính liên tục trên $F$, thì hạn chế $z'_n$ của nó trên $F_n$ là liên tục; vì $F = \bigcup_n F_n$, không gian đối ngẫu $F'$ của $F$ có thể được đồng nhất (theo nghĩa đại số) với một không gian con tuyến tính của tích $\prod_n F'_n$, và $\operatorname{pr}_n z' = z'_n$. Hơn nữa, vì mọi tập con hữu hạn của $F$ đều được chứa trong một trong các $F_n$, tôpô $\sigma(F', F)$ chẳng qua là tôpô cảm sinh bởi tôpô tích của các tôpô $\sigma(F'_n, F_n)$. Vì thế, nếu $f$ là đo được vô hướng theo $\mu$ thì $\operatorname{pr}_n \circ f$ cũng đo được vô hướng theo $\mu$, vì với mọi $t \in T$, $\operatorname{pr}_n(f(t))$ là hạn chế của $f(t)$ trên $F_n$. Phần thứ nhất của chứng minh cho thấy rằng $\operatorname{pr}_n \circ f$ là đo được theo $\mu$ với mọi $n$, do đó $f$ cũng vậy (Ch. IV, §5, No. 3, Th. 1).

### 6. Ứng dụng: I. Mở rộng một hàm liên tục tới một không gian các độ đo

Cho $T$ là một không gian compact địa phương, $F$ là một không gian lồi địa phương Hausdorff gần đầy đủ, và $f$ là một ánh xạ liên tục của $T$ vào $F$; nếu $\mu$ là một độ đo dương trên $T$, với giá compact $S$, thì $f(S)$ là compact; bao lồi đóng của $f(S)$ khi đó cũng compact (TVS, III, §1, No. 6), do đó $f$ là khả tích theo vô hướng đối với $\mu$ và $\int f \, d\mu \in F$ (No. 2, Hệ quả của Mệnh đề 5). Nếu bây giờ $\lambda$ là một độ đo thực bất kỳ có giá compact, thì $\lambda^+$ và $\lambda^-$ là các độ đo dương có giá compact; đặt $\int f \, d\lambda = \int f \, d\lambda^+ - \int f \, d\lambda^-$, ta kiểm tra ngay lập tức (dùng quan hệ $(\lambda + \mu)^+ + \lambda^- + \mu^- = \lambda^+ + \mu^+ + (\lambda + \mu)^-$) rằng $\lambda \mapsto \int f \, d\lambda$ là một ánh xạ tuyến tính của không gian $\mathcal{C}'(T)$ gồm các độ đo trên $T$ có giá compact, vào không gian lồi địa phương $F$.

Ta hãy nhận xét rằng không gian $\mathcal{C}'(T)$ có thể được đồng nhất với đối ngẫu của không gian $\mathcal{C}(T)$ gồm các hàm số thực liên tục trên $T$ (do đó có ký hiệu ấy), khi $\mathcal{C}(T)$ được trang bị tôpô hội tụ đều trên các tập compact (điều mà ta sẽ luôn giả sử trong No. này và No. sau): vì, một mặt, người ta biết rằng (Ch. IV, §4, No. 8, Mệnh đề 14) các độ đo trên $T$ có thể được mở rộng thành các dạng tuyến tính liên tục trên $\mathcal{C}(T)$ chính là các độ đo có giá compact, và ngược lại, hạn chế lên $\mathcal{K}(T)$ của một dạng tuyến tính liên tục trên $\mathcal{C}(T)$ là một độ đo (vì tôpô của $\mathcal{K}(T)$ mịn hơn tôpô cảm sinh bởi tôpô của $\mathcal{C}(T)$).

#### Mệnh đề 14 {#int-vi-s1-prop-14 .statement}

*Cho $T$ là một không gian compact địa phương, $F$ là một không gian lồi địa phương Hausdorff gần đầy đủ, và $f$ là một ánh xạ liên tục của $T$ vào $F$. Nếu không gian $\mathcal{C}'(T)$ gồm các độ đo trên $T$ có giá compact được trang bị tôpô hội tụ đều trên các tập compact của $\mathcal{C}(T)$, thì ánh xạ $\lambda \mapsto \int f d\lambda$ là ánh xạ tuyến tính liên tục duy nhất $\tilde{f}$ từ $\mathcal{C}'(T)$ vào $F$ sao cho $\tilde{f}(\varepsilon_t) = f(t)$ với mọi $t \in T$.*

Để xác lập tính duy nhất của sự mở rộng, chỉ cần thấy rằng các độ đo tại điểm $\varepsilon_t$ tạo thành một tập đầy đủ trong $\mathcal{C}'(T)$; vì đối ngẫu của $\mathcal{C}'(T)$ là $\mathcal{C}(T)$ (TVS, IV, §1, No. 1, Định lý 1), chỉ cần nhận xét rằng mọi hàm $g \in \mathcal{C}(T)$ trực giao với tất cả các độ đo $\varepsilon_t$ đều bằng 0 theo định nghĩa (TVS, IV, §1, No. 2, Mệnh đề 2).

Giờ ta hãy chứng minh rằng $\lambda \mapsto \int f d\lambda$ là liên tục. Cho V là một lân cận đóng, cân bằng, lồi của 0 trong F; chỉ cần chứng minh rằng tồn tại một tập con tương đối compact L của $\mathcal{C}(T)$ sao cho các quan hệ $\lambda \in L^\circ$ và $z' \in V^\circ$ suy ra $|\langle \int f d\lambda, z' \rangle| \leq 1$, hay cũng vậy $|\int \langle f, z' \rangle d\lambda| \leq 1$. Để làm điều này, ta sẽ chứng minh rằng khi $z'$ chạy qua $V^\circ$, tập L các hàm số số trị $\langle f, z' \rangle$ là tương đối compact trong $\mathcal{C}(T)$. Vì $V^\circ$ bị chặn đối với $\sigma(F', F)$, cận trên của các số $|\langle f(t), z' \rangle|$, với $t \in T$ cố định và $z'$ chạy qua $V^\circ$, là hữu hạn; nhờ định lý Ascoli (GT, X, §2, No. 5, Hệ quả 2 của Định lý 2), do đó chỉ cần chứng minh rằng tập các $\langle f, z' \rangle$ ($z' \in V^\circ$) là *liên đều*. Nhưng, với mọi $t_0 \in T$ và mọi $\delta > 0$, theo giả thiết tồn tại một lân cận W của $t_0$ trong T sao cho $f(t) - f(t_0) \in \delta V$ đối với mọi $t \in W$; suy ra $|\langle f(t), z' \rangle - \langle f(t_0), z' \rangle| \leq \delta$ đối với mọi $t \in W$ và mọi $z' \in V^\circ$, điều này hoàn tất chứng minh.

#### Nhận xét {#int-vi-s1-n6-rem-1 .statement}

— 1) Ánh xạ $t \mapsto \varepsilon_t$ là một *đồng phôi* của T vào không gian $\mathcal{C}'(T)$; thật vậy, nếu L là một tập con compact của $\mathcal{C}(T)$, và $t_0 \in T$, tồn tại (GT, X, §2, No. 5, Hệ quả 3 của Định lý 2) một lân cận W của $t_0$ sao cho $|g(t) - g(t_0)| \leq 1$ với mọi $t \in W$ và mọi hàm số $g \in L$, do đó $\varepsilon_t - \varepsilon_{t_0} \in L^\circ$ với $t \in W$, điều này chứng minh tính liên tục của $t \mapsto \varepsilon_t$ (cf. Ch. IV, §4, No. 8, Mệnh đề 15); ngoài ra người ta còn biết rằng ánh xạ nghịch đảo đã liên tục đối với tôpô mơ hồ (Ch. III, §1, No. 9, Mệnh đề 13), nên *a fortiori* đối với tôpô hội tụ đều trên tập con compact của $\mathcal{C}(T)$. Nếu rồi đồng nhất T với ảnh của nó trong $\mathcal{C}'(T)$ qua $t \mapsto \varepsilon_t$, ta có thể nói rằng $\lambda \mapsto \int f d\lambda$ là phần *mở rộng liên tục* duy nhất của f thành một ánh xạ *tuyến tính*.

2) Chú ý rằng trong chứng minh tính liên tục của $\lambda \mapsto \int f d\lambda$, ta đã không dùng giả thiết F là gần đầy đủ. Do đó kết luận của Mệnh đề 14 vẫn đúng mà không cần giả thiết này, với điều kiện còn biết thêm rằng $\int f d\mu \in F$ đối với mọi độ đo dương $\mu$ có giá compact.

Giả sử bây giờ rằng $f(T)$ là một tập con *bị chặn* của F. Khi đó, đối với mọi độ đo dương *bị chặn* $\mu$ trên T, f là khả tích theo vô hướng đối với $\mu$ và $\int f d\mu \in F$

(No. 2, Mệnh đề 8). Nếu $\lambda$ là bất kỳ độ đo thực bị chặn nào trên T, thì $\lambda^+$ và $\lambda^-$ đều bị chặn, và ta thấy ngay rằng $\lambda \mapsto \int f\, d\lambda$, được định nghĩa như trên, là một ánh xạ *tuyến tính* của không gian $\mathcal{M}^1(T)$ các độ đo *bị chặn* trên T, vào không gian lồi địa phương F, ánh xạ này hiển nhiên mở rộng ánh xạ $\lambda \mapsto \int f\, d\lambda$ của $\mathcal{C}'(T)$ vào F.

#### Mệnh đề 15 {#int-vi-s1-prop-15 .statement}

*Cho $T$ là một không gian compact địa phương, $F$ là một không gian lồi địa phương Hausdorff đầy đủ từng phần, và $f$ là một ánh xạ liên tục của $T$ vào $F$ sao cho $f(T)$ bị chặn. Nếu $\mathcal{M}^1(T)$ được trang bị tôpô không gian Banach của nó, thì ánh xạ tuyến tính $\lambda \mapsto \int f\, d\lambda$ từ $\mathcal{M}^1(T)$ vào $F$ là liên tục.*

Với mọi lân cận đóng, cân bằng, lồi $V$ của $0$ trong $F$, tồn tại một $\rho > 0$ sao cho $f(T) \subset \rho V$; do đó bao đóng, cân bằng, lồi $B$ của $f(T)$ được chứa trong $\rho V$, và nó đầy đủ theo giả thiết. Nếu khi đó $\| \lambda \| \leq 1/\rho$, thì suy ra từ No. 2, Mệnh đề 8, và quan hệ $\| \lambda \| = \lambda^+(T) + \lambda^-(T)$, rằng $\int f\, d\lambda \in B/\rho \subset V$.

### 7. Ứng dụng: II. Mở rộng, sang một không gian các độ đo, của một hàm liên tục nhận giá trị trong một không gian các toán tử

Cho $G$ là một không gian lồi địa phương Hausdorff, $H$ là một không gian lồi địa phương Hausdorff và gần đầy đủ, và ký hiệu $F$ là không gian $\mathcal{L}(G; H)$ của các ánh xạ tuyến tính liên tục từ $G$ vào $H$, được trang bị tôpô *hội tụ compact*. Không gian $F$ không nhất thiết gần đầy đủ, và nếu $t \mapsto U(t)$ là một ánh xạ liên tục của $T$ vào $F$, và $\mu$ là một độ đo dương trên $T$ với giá đỡ compact, thì không nhất thiết có $\int U\, d\mu \in F$ (Bài tập 27). Tuy nhiên, nếu, với mọi tập con compact $K$ của $T$, $U(K)$ đều liên tục đều, thì bao lồi cân bằng của nó trong $F$ cũng liên tục đều (TVS, III, §3, No. 4), và vì $H$ là gần đầy đủ, bao đóng của bao lồi cân bằng này sẽ là một tập con đầy đủ của $F$ (TVS, III, §3, No. 8, Mệnh đề 11); khi đó quả thật sẽ có $\int U\, d\mu \in F$ (No. 2, Mệnh đề 8).

Điều kiện bổ sung đặt lên $U$ có thể phát biểu theo cách khác:

#### Bổ đề 3 {#int-vi-s1-lem-3 .statement}

*Cho $G, H$ là hai không gian lồi địa phương, $U$ là một ánh xạ của một không gian compact địa phương $T$ vào $\mathcal{L}(G; H)$. Các điều kiện sau là tương đương:
a) Ánh xạ $(t, x) \mapsto U(t) \cdot x$ từ $T \times G$ vào $H$ là liên tục.
b) Với mọi tập con compact $K$ của $T$, $U(K)$ đều liên tục đều, và tồn tại một tập toàn phần $D \subset G$ sao cho với mọi $x \in D$, ánh xạ $t \mapsto U(t) \cdot x$ là liên tục trên $T$.*

Hơn nữa, khi $U$ thỏa các điều kiện này, $U$ là một ánh xạ liên tục của $T$ vào $\mathcal{L}(G; H)$ được trang bị tôpô hội tụ trên compact.

Để thấy rằng a) suy ra b), ta nhận thấy rằng với mọi lân cận $V$ của $0$ trong $H$ và mọi $t \in K$, theo giả thiết tồn tại một lân cận $L_t$ của $t$ trong $T$ và một lân cận $W_t$ của $0$ trong $G$ sao cho các quan hệ $t' \in L_t$ và $x \in W_t$ suy ra $U(t') \cdot x \in V$. Chỉ cần phủ $K$ bởi một số hữu hạn các lân cận $L_{t_i}$ và lấy $W = \bigcap_i W_{t_i}$ để có $U(t) \cdot x \in V$ bất cứ khi nào $t \in K$ và $x \in W$, điều này chứng minh tính đều liên tục của $U(K)$.

Ngược lại, giả sử b) đã được xác nhận; chỉ cần chứng minh rằng với mọi tập hợp con $K$ compact của $T$, ánh xạ $(t, x) \mapsto U(t) \cdot x$ là liên tục trên $K \times G$. Đặt $M = U(K)$; vì $M$ là đều liên tục, suy ra trên $M$, tôpô hội tụ điểm trong $G$ trùng với tôpô hội tụ điểm trong $D$ (GT, X, §2, No. 4, Định lý 1); do đó giả thiết b) suy ra rằng $t \mapsto U(t)$ là một ánh xạ liên tục của $K$ vào $\mathcal{L}(G; H)$ khi $\mathcal{L}(G; H)$ được trang bị tôpô hội tụ điểm. Mặt khác, $(A, x) \mapsto A \cdot x$ là một ánh xạ liên tục của $M \times G$ vào $H$ khi $M$ được trang bị tôpô hội tụ điểm (GT, X, §2, No. 1, Hệ quả 4 của Mệnh đề 1). Vì ánh xạ $(t, x) \mapsto U(t) \cdot x$ có thể phân tích thành $(t, x) \mapsto (U(t), x) \mapsto U(t) \cdot x$, ta kết luận rằng nó là liên tục.

Cuối cùng, khẳng định cuối cùng của bổ đề suy ra từ sự kiện rằng, trên $M$, tôpô của sự hội tụ compact trùng với tôpô của sự hội tụ điểm (GT, X, §2, No. 4, Định lý 1).

Vì thế, giả sử rằng $U$ thỏa các điều kiện của Bổ đề 3; khi đó (nếu $H$ là gần đầy đủ) ta định nghĩa, như trong No. 6, một ánh xạ tuyến tính $\lambda \mapsto \int U d\lambda$ của $\mathcal{C}'(T)$ vào $F = \mathcal{L}(G; H)$. Ta đặt $U(\lambda) = \int U d\lambda$.

#### Mệnh đề 16 {#int-vi-s1-prop-16 .statement}

— Cho $G, H$ là hai không gian lồi địa phương Hausdorff, với $H$ được giả sử là gần đầy đủ. Cho $U$ là một ánh xạ của $T$ vào $\mathcal{L}(G; H)$ sao cho $(t, x) \mapsto U(t) \cdot x$ là một ánh xạ liên tục của $T \times G$ vào $H$. Khi đó ánh xạ song tuyến tính $(\lambda, x) \mapsto U(\lambda) \cdot x$ của $\mathcal{C}'(T) \times G$ vào $H$ là nửa liên tục tương ứng với các tập hợp đều liên tục của $\mathcal{C}'(T)$ và các tập hợp compact của $G$ (điều này kéo theo rằng ánh xạ tuyến tính $\lambda \mapsto U(\lambda)$ của $\mathcal{C}'(T)$ vào $F$ là liên tục).

Sự liên tục của $\lambda \mapsto U(t)$ như một ánh xạ của $\mathcal{C}'(T)$ vào $F$ suy ra từ Bổ đề 3 và Nhận xét 2 sau Mệnh đề 14 của No. 6. Do đó, vẫn còn phải chứng minh rằng với mọi lân cận đóng, cân bằng, lồi $V$ của 0 trong $H$ và với mọi tập con đều liên tục $N$ của $\mathcal{C}'(T)$, tồn tại một lân cận $W$ của 0 trong $G$ sao cho các điều kiện $x \in W, \lambda \in N$ suy ra rằng $U(\lambda) \cdot x \in V$. Có thể giả sử rằng $N = S^\circ$, trong đó $S$ là một lân cận của 0 trong $\mathcal{C}(T)$, do đó có thể giả sử rằng $S$ là tập các hàm $g \in \mathcal{C}(T)$ sao cho $|g(t)| \leq 1$ trên một tập con compact $K$ của $T$. Chỉ cần chứng minh rằng

|⟨U(λ) · x, x′⟩| ≤ 1 với x ∈ W, x′ ∈ V° và λ ∈ S°. Bây giờ, vì $U(K)$ là đều liên tục, tồn tại một lân cận $W$ của 0 trong $G$ sao cho các điều kiện $t ∈ K, x ∈ W$ suy ra $U(t) · x ∈ V$; các điều kiện $x ∈ W, x′ ∈ V°$ do đó suy ra rằng hàm $t ↦ ⟨U(t) · x, x′⟩$ thuộc $S$, suy ra rằng $|⟨U(t) · x, x′⟩| = |∫⟨U(t) · x, x′⟩ dλ(t)| ≤ 1$ theo định nghĩa của $S°$.

Bây giờ ta giả sử rằng $U$ là một ánh xạ liên tục của $T$ vào $F$ và, hơn nữa, $U(T)$ là đều liên tục. Khi đó, cùng một lập luận như trên cho thấy (vì $H$ là gần đầy đủ) rằng với mọi độ đo dương bị chặn $\mu$ trên $T$, $\int U d\mu \in F$. Do đó có thể định nghĩa, như trên, một ánh xạ tuyến tính $\lambda \mapsto \int U d\lambda = U(\lambda)$ của $M^1(T)$ vào $F$ mở rộng ánh xạ tương tự của $\mathcal{C}'(T)$ vào $F$. Hơn nữa, với mọi lân cận đóng, cân bằng, lồi $V$ của 0 trong $H$, theo giả thiết tồn tại một lân cận $W$ của 0 trong $G$ sao cho với mọi $x \in W$ và mọi $t \in T$, ta có $U(t) · x ∈ V$, do đó (vì $V$ là đóng yếu) $\int (U(t) · x)d\lambda(t) ∈ ||\lambda|| · V$ (No. 2, Mệnh đề 5). Nói cách khác:

#### Mệnh đề 17 {#int-vi-s1-prop-17 .statement}

— Cho $G, H$ là hai không gian lồi địa phương Hausdorff, với $H$ được giả sử là gần đầy đủ. Cho $U$ là một ánh xạ của $T$ vào $L(G; H)$ sao cho $(t, x) ↦ U(t) · x$ liên tục trên $T × G$, và $U(T)$ là đều liên tục. Khi đó, nếu $M^1(T)$ được trang bị tôpô không gian Banach của nó, thì ánh xạ song tuyến tính $(\lambda, x) ↦ U(\lambda) · x$ của $M^1(T) × G$ vào $H$ là liên tục (điều này kéo theo, đặc biệt, rằng ánh xạ tuyến tính $\lambda \mapsto U(\lambda)$ của $M^1(T)$ vào $L(G; H)$ là liên tục khi $L(G; H)$ được trang bị tôpô hội tụ bị chặn).

#### Mệnh đề 18 {#int-vi-s1-prop-18 .statement}

— Cho $G_1, G_2, H_1, H_2$ là bốn không gian lồi địa phương Hausdorff, với $H_1$ và $H_2$ được giả sử là gần đầy đủ. Cho $A : G_1 \to G_2$ và $B : H_1 \to H_2$ là hai ánh xạ tuyến tính liên tục. Cho $U_1 : T \to L(G_1; H_1), U_2 : T \to L(G_2; H_2)$ là hai ánh xạ thỏa mãn các điều kiện của Mệnh đề 16 (resp. Mệnh đề 17), và giả sử rằng với mọi $t ∈ T$, $B \circ U_1(t) = U_2(t) \circ A$. Khi đó, với mọi độ đo có giá đỡ compact (resp. mọi độ đo bị chặn) $\lambda$ trên $T$, $B \circ U_1(\lambda) = U_2(\lambda) \circ A$.

Thật vậy, với mọi $x ∈ G_1$, ta có (No. 1, Mệnh đề 1)

$$
(B \circ U_1(\lambda)) \cdot x = \int \left( (B \circ U_1(t)) \cdot x \right) d\lambda(t)
$$
$$
= \int \left( (U_2(t) \circ A) \cdot x \right) d\lambda(t) = U_2(\lambda) \cdot (A \cdot x).
$$

#### Nhận xét 1 {#int-vi-s1-n7-rem-1 .statement}

Giả sử rằng $G$ và $H$ là các không gian Banach, và cho $U$ là một ánh xạ của $T$ vào $L(G; H)$ sao cho $(t, x) ↦ U(t) · x$ liên tục trên $T × G$. Lưu ý rằng điều này kéo theo rằng hàm hữu hạn $t ↦ \|U(t)\|$ bị chặn trên mọi tập con compact của $T$ và nửa liên tục dưới trên $T$, vì nó là bao trên của các hàm liên tục $t \mapsto |U(t) \cdot x|$ khi $x$ chạy trên quả cầu $|x| \leq 1$ trong $G$. Đặt $h(t) = \| U(t) \|$. Khi đó, với mọi độ đo dương $\mu$ trên $T$ sao cho $h$ là khả tích theo $\mu$, ta lại có $\int U d\mu \in \mathcal{L}(G; H)$. Thật vậy, độ đo $\nu = h \cdot \mu$ bị chặn theo giả thiết; do đó tồn tại một phân hoạch của $T$ gồm một tập $N$ không đáng kể theo $\nu$ và một dãy $(K_n)$ các tập con compact. Lập luận ở đầu số này, áp dụng cho độ đo $\varphi_{K_n} \cdot \mu$, cho thấy rằng

$$
A_n = \int \varphi_{K_n} U \, d\mu \in F = \mathcal{L}(G; H),
$$

và hơn nữa (No. 2, Mệnh đề 6), $\| A_n \| \leq \int \varphi_{K_n} \| U \| \, d\mu \leq \nu(K_n)$. Do đó chuỗi với số hạng tổng quát $A_n$ hội tụ tuyệt đối trong không gian Banach $\mathcal{L}(G; H)$, và ngay lập tức suy ra rằng tổng của nó là $\int U \, d\mu$ và rằng $\| \int U \, d\mu \| \leq \int \| U \| \, d\mu$.

#### Nhận xét 2 {#int-vi-s1-n7-rem-2 .statement}

Giả sử rằng $G = H$ là gần đầy đủ và rằng $U$ thỏa mãn các giả thiết của Mệnh đề 16. Cho $M$ là một tập con trù mật của không gian $\mathcal{C}'(T)$, đối với tôpô yếu $\sigma(\mathcal{C}'(T), \mathcal{C}(T))$, và cho $X$ là một không gian con tuyến tính đóng của $H$ sao cho $U(\lambda)(X) \subset X$ với mọi độ đo $\lambda \in M$. Khi đó cũng có $U(t)(X) \subset X$ với mọi $t \in T$: thật vậy, với mọi $x \in X$ và mọi $x' \in H'$ trực giao với $X$, theo giả thiết $\langle U(\lambda) \cdot x, x' \rangle = 0$ với mọi $\lambda \in M$, điều này có thể viết là $\int \langle U(t) · x, x' \rangle \, d\mu(t) = 0$. Hàm liên tục $t \mapsto \langle U(t) \cdot x, x' \rangle$, vì trực giao với $M$, do đó bằng 0, điều này suy ra $\langle U(t) \cdot x, x' \rangle = 0$ với mọi $x' \in X^\circ$, do đó $U(t) \cdot x \in X$ với mọi $t \in T$ và $x \in X$, và điều đó chứng minh mệnh đề của chúng ta.

### Bài tập {#int-vi-s1-exercises}

Xem các [bài tập của § 1](exercises/s1/).
