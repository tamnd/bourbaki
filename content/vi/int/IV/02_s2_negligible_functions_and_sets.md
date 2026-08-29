---
book: int
book_title: Integration
chapter: IV
chapter_title: EXTENSION OF A MEASURE. LP SPACES
section: 2
section_title: Negligible functions and sets
lang: vi
source: int-i-vi
book_pages: INT IV.11-INT IV.17
pdf_pages: 0118-0124
extraction: ocr
subsections:
    - "no": 1
      title: Negligible positive functions
      page: 11
      pdf_page: 118
    - "no": 2
      title: Negligible sets
      page: 12
      pdf_page: 119
    - "no": 3
      title: Properties true almost everywhere
      page: 12
      pdf_page: 119
    - "no": 4
      title: Classes of equivalent functions
      page: 13
      pdf_page: 120
    - "no": 5
      title: Functions defined almost everywhere
      page: 15
      pdf_page: 122
    - "no": 6
      title: Equivalence classes of functions with values in $\overline{\mathbf{R}}$
      page: 16
      pdf_page: 123
statements: 15
exercises: 0
content_sha256: 56eed24fea44908e22ade4d7a360464fb05ec94f8609e473f96e479bbe5872d1
translated_from: content/en/int/IV/02_s2_negligible_functions_and_sets.md
source_content_sha256: 8ed4876b66e4b93e4252c89f40e59e5df51207d878e7a01e38c48f580a5ec1d0
translation_model: gpt-5-6-mini, gpt-5.4-mini
translation_run: translate-vi-12513e78
glossary_version: 34
glossary_terms_sha256: 4a042e3857ee534862bd268b19e5759cc83a251765b132f0d411211c54fbba20
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 2. CÁC HÀM VÀ TẬP HỢP KHÔNG ĐÁNG KỂ

### 1. Các hàm dương không đáng kể

#### Định nghĩa 1 {#int-iv-s2-def-1 .statement}

— *Cho một độ đo $\mu$ trên một không gian địa phương compact X*, *một hàm số* $f \geq 0$ (*hữu hạn hoặc không*) *xác định trên X được gọi là không đáng kể đối với độ đo $\mu$ nếu* $|\mu|^*(f) = 0$.

Khi đó ta cũng nói rằng $f$ là *$\mu$-không đáng kể*, hoặc đơn giản là *không đáng kể* nếu không thể xảy ra sự nhầm lẫn.

#### Mệnh đề 1 {#int-iv-s2-prop-1 .statement}

— *Nếu* $f$ *là một hàm không đáng kể* $\geq 0$, *thì mọi hàm số* $g$ *sao cho* $0 \leq g \leq \alpha f$ ($\alpha$ *là một vô hướng* $> 0$) *đều là không đáng kể*. Thật vậy, $0 \leq |\mu|^*(g) \leq \alpha |\mu|^*(f) = 0$.

#### Mệnh đề 2 {#int-iv-s2-prop-2 .statement}

— *Tổng và bao trên của một dãy* $(f_n)$ *các hàm không đáng kể* $\geq 0$ *là không đáng kể*.

Thật vậy, $|\mu|^*(\sum_n f_n) \leq \sum_n |\mu|^*(f_n) = 0$ (§ 1, No. 3, Mệnh đề 13) và $\sup_n f_n \leq \sum_n f_n$.

#### Mệnh đề 3 {#int-iv-s2-prop-3 .statement}

*Đối với một hàm nửa liên tục dưới $f \geq 0$ trên $X$, để là không đáng kể, điều kiện cần và đủ là $f$ bằng không trên giá của $\mu$.*

Nếu $|\mu|^*(f) = 0$ thì $|\mu|(g) = 0$ đối với mọi hàm $g \in \mathcal{K}_+$ sao cho $g \leq f$; suy ra (Ch. III, § 2, No. 3, Mệnh đề 9) rằng $g$ bằng không trên giá $S$ của $\mu$; vì $f$ là bao trên của các hàm $g \in \mathcal{K}_+$ sao cho $g \leq f$ (§ 1, No. 1, Bổ đề), nên $f(x) = 0$ trên $S$. Ngược lại, nếu $f(x) = 0$ trên $S$ thì $g(x) = 0$ trên $S$ đối với mọi hàm $g \in \mathcal{K}_+$ sao cho $g \leq f$, do đó (Ch. III, § 2, No. 3, Mệnh đề 8) $|\mu|(g) = 0$, điều này, theo định nghĩa, kéo theo $|\mu|^*(f) = 0$.

### 2. Các tập hợp không đáng kể

#### Định nghĩa 2 {#int-iv-s2-def-2 .statement}

*Cho một độ đo $\mu$ trên một không gian địa phương compact $X$, một tập con $A$ của $X$ được gọi là không đáng kể đối với độ đo $\mu$ nếu $|\mu|^*(A) = 0$.*

Ta cũng nói rằng $A$ là $\mu$-không đáng kể, hoặc đơn giản là không đáng kể nếu không thể xảy ra sự nhầm lẫn. Điều này tương đương với việc nói rằng hàm đặc trưng $\varphi_A$ là không đáng kể.

#### Mệnh đề 4 {#int-iv-s2-prop-4 .statement}

*Mọi tập con của một tập hợp không đáng kể đều không đáng kể; mọi hợp đếm được của các tập hợp không đáng kể đều không đáng kể.*

Đây là một hệ quả ngay lập tức của các Mệnh đề 1 và 2.

#### Ví dụ {#int-iv-s2-n2-exa-1 .statement}

— Cho $\mu$ là độ đo Lebesgue trên $\mathbf{R}$. Mọi tập hợp $\{x_0\}$ thu gọn thành một điểm đều không đáng kể (xem § 1, No. 3, *Nhận xét* 1). Suy ra rằng *mọi tập con đếm được của $\mathbf{R}$ đều không đáng kể đối với độ đo Lebesgue*. Đảo lại của mệnh đề này không đúng (§ 4, Bài tập 4 b)).

#### Mệnh đề 5 {#int-iv-s2-prop-5 .statement}

*Phần bù của giá $S$ của $\mu$ là tập hợp mở không đáng kể lớn nhất trong $X$.*

Thật vậy, theo Mệnh đề 3, để một tập mở $G$ là không đáng kể, điều kiện cần và đủ là $G \cap S = \varnothing$, tức là $G \subset \mathbf{C}S$.

### 3. Các tính chất đúng hầu khắp nơi

Cho $X$ là một không gian compact địa phương, $\mu$ là một độ đo trên $X$. Nếu $P\{x\}$ là một tính chất, tính chất « $P\{x\}$ hầu khắp nơi (đối với $\mu$) » theo định nghĩa tương đương với tính chất « *tập hợp các x sao cho* $(x \in X \text{ và không } P\{x\})$ *là $\mu$*-tập không đáng kể ».

#### Định lý 1 {#int-iv-s2-thm-1 .statement}

— Để một hàm số (hữu hạn hoặc không) $f \geqslant 0$ xác định trên $X$ là không đáng kể, điều kiện cần và đủ là $f(x) = 0$ hầu khắp nơi.

Điều kiện là cần. Thật vậy, giả sử $f$ là không đáng kể, và gọi $N$ là tập hợp các $x \in X$ sao cho $f(x) \neq 0$; khi đó $\varphi_N \leqslant \sup_n (n f)$, do đó $\varphi_N$ là không đáng kể (No. 1, Props. 1 và 2).

Điều kiện là đủ. Giả sử rằng tập hợp $N$ các điểm mà tại đó $f(x) \neq 0$ là không đáng kể; khi đó $f \leqslant \sup_n n \varphi_N$, do đó $f$ là không đáng kể (No. 1, Props. 1 và 2).

#### Mệnh đề 6 {#int-iv-s2-prop-6 .statement}

— Nếu $f$ và $g$ là hai hàm $\geqslant 0$ (hữu hạn hoặc không) xác định trên $X$ sao cho $f(x) = g(x)$ hầu khắp nơi, thì $|\mu|^*(f) = |\mu|^*(g)$.

Gọi $N$ là tập không đáng kể các điểm $x \in X$ sao cho $f(x) \neq g(x)$. Các hàm $\inf(f, g)$ và $\sup(f, g)$ bằng nhau ngoại trừ tại các điểm của $N$, do đó chỉ cần chứng minh mệnh đề trong trường hợp giả sử $f \leqslant g$. Gọi $h$ là hàm bằng $+\infty$ tại các điểm của $N$, và bằng 0 trên $CN$; khi đó $f \leqslant g \leqslant f + h$, do đó

$$
|\mu|^*(f) \leqslant |\mu|^*(g) \leqslant |\mu|^*(f + h) \leqslant |\mu|^*(f) + |\mu|^*(h) = |\mu|^*(f)
$$

(vì $h$ là không đáng kể), do đó có mệnh đề.

#### Mệnh đề 7 {#int-iv-s2-prop-7 .statement}

— Nếu $f$ là một hàm $\geqslant 0$ xác định trên $X$ sao cho $|\mu|^*(f) < +\infty$, thì $f(x)$ là hữu hạn hầu khắp nơi.

Thật vậy, gọi $N$ là tập hợp các điểm $x \in X$ sao cho $f(x) = +\infty$; với mọi số nguyên $n$, $n \varphi_N \leqslant f$, do đó $n |\mu|^*(\varphi_N) \leqslant |\mu|^*(f)$; vì $n$ tùy ý lớn, $|\mu|^*(N) = 0$.

Tuy nhiên, ngay cả khi $X$ là compact, một hàm $f \geqslant 0$ xác định trên $X$ và hữu hạn mọi nơi vẫn có thể có tích phân trên vô hạn, như được chỉ ra bởi ví dụ $X = [0, 1]$, $f(x) = 1/x$ với $x > 0$ và $f(0) = 0$, $\mu$ là độ đo Lebesgue trên $X$.

### 4. Các lớp của các hàm tương đương

Cho $\mu$ là một độ đo trên một không gian địa phương compact $X$. Với một tập hợp $F$ cho trước, hai ánh xạ $f, g$ từ $X$ vào $F$ được gọi là *tương đương đối với* $\mu$ (hay *μ-tương đương*, hay đơn giản *tương đương* nếu không thể có nhầm lẫn) nếu $f(x) = g(x)$ *hầu khắp nơi* trong $X$. Vì hợp của hai tập không đáng kể vẫn là không đáng kể, ta thật sự định nghĩa theo cách này một quan hệ tương đương trên tập $F^X$ của mọi ánh xạ từ $X$ vào $F$; khi nói đến *lớp tương đương* của một hàm $f$ như vậy (không nói rõ thêm) thì sẽ hiểu là lớp của mọi hàm bằng $f$ hầu khắp nơi; trong chương này và các chương sau, ta sẽ ký hiệu lớp này bằng ký hiệu $\tilde{f}$.

#### Mệnh đề 8 {#int-iv-s2-prop-8 .statement}

*Cho* $(F_n)$ *là một họ đếm được (hữu hạn hoặc vô hạn) các tập hợp. Với mọi chỉ số n, cho* $f_n, g_n$ *là hai ánh xạ tương đương của X vào* $F_n$; *khi đó, tồn tại một tập không đáng kể H sao cho, với mọi* $x \notin H$, $f_n(x) = g_n(x)$ *với mọi n*.

Thật vậy, tập $H_n$ gồm các $x \in X$ sao cho $f_n(x) \neq g_n(x)$ là không đáng kể, do đó hợp của chúng là $H$ cũng vậy (No. 2, Mệnh đề 4), và tập này thỏa mãn các yêu cầu.

#### Hệ quả {#int-iv-s2-n4-cor-1 .statement}

*Nếu* $\varphi$ *là một ánh xạ của* $\prod_n F_n$ *vào một tập G, thì các ánh xạ* $\varphi((f_n))$ *và* $\varphi((g_n))$ *của X vào G là tương đương*.

Ta ký hiệu bằng $\varphi((\tilde{f}_n))$ lớp tương đương của mọi hàm $\varphi((f_n))$, trong đó $f_n$ là một hàm tùy ý trong lớp $\tilde{f}_n$.

Đặc biệt, nếu F là một *không gian vectơ* trên $\mathbf{R}$, ta định nghĩa $\tilde{f} + \tilde{g}$ và $\alpha \tilde{f}$ là các lớp tương đương của $f + g$ và $\alpha f$, tương ứng ($f$ và $g$ là các ánh xạ của X vào F, và $\alpha$ là một vô hướng); theo cách này, trên tập các lớp tương đương của các ánh xạ của X vào F, ta thu được một cấu trúc *không gian vectơ*: hơn nữa, đó là cấu trúc *không gian thương* của cấu trúc của $F^X$ theo không gian con tuyến tính của các ánh xạ $f$ sao cho $\tilde{f} = \tilde{0}$ (các hàm bằng không hầu khắp nơi), mà ta cũng gọi là các hàm *không đáng kể* (với giá trị trong F). Tương tự, ta định nghĩa tích $\tilde{g} \tilde{f}$, trong đó $\tilde{f}$ là một lớp tương đương của các ánh xạ của X vào F, và $\tilde{g}$ là một lớp tương đương của các hàm số giá trị hữu hạn xác định trên X: do đó, tập các lớp tương đương của các ánh xạ của X vào F được trang bị cấu trúc một *môđun* trên tập các lớp tương đương của các hàm số giá trị hữu hạn xác định trên X (chính tập này lại được trang bị một cấu trúc *vành*). Nếu F là một *đại số* trên $\mathbf{R}$, ta cũng định nghĩa tương tự một cấu trúc đại số trên tập các lớp tương đương của các ánh xạ của X vào F.

Cho F là một không gian tôpô *mêtric hóa*, và xét một cấu trúc đều trên F tương thích với tôpô của nó và được xác định bởi một họ *đếm được* các giả khoảng cách $\rho_n$ (GT, IX, §§1 và 2); để hai ánh xạ $f, g$ từ X vào F tương đương, điều kiện cần và đủ là các hàm số $\rho_n(f, g)$ *không đáng kể*; vì điều này tương đương với việc tồn tại một tập không đáng kể H trong X sao cho, với mọi $x \notin H$, $\rho_n(f(x), g(x)) = 0$ với mọi n, nghĩa là $f(x) = g(x)$. Đặc biệt, nếu F là một không gian lồi địa phương mêtric hóa, và $(q_n)$ là một họ đếm được các nửa chuẩn xác định tôpô của F (TVS, II, §4, No. 1), để hai ánh xạ $f, g$ từ X vào F tương đương thì điều kiện cần và đủ là mọi hàm số thực $q_n(f(x) - g(x))$ đều không đáng kể.

#### Mệnh đề 9 {#int-iv-s2-prop-9 .statement}

— Cho $f$ và $g$ là hai ánh xạ liên tục từ $X$ vào một không gian tôpô Hausdorff $F$; để $f$ và $g$ tương đương, điều kiện cần và đủ là $f(x) = g(x)$ tại mọi điểm của giá đỡ của $\mu$.

Vì, tập các $x \in X$ sao cho $f(x) \neq g(x)$ là một tập mở (GT, I, §8, No. 1); để nó không đáng kể, điều kiện cần và đủ là nó không giao với giá đỡ của $\mu$ (No. 2, Mệnh đề 5).

#### Mệnh đề 10 {#int-iv-s2-prop-10 .statement}

— Cho $F$ là một không gian lồi địa phương Hausdorff trên $\mathbf{R}$ sao cho trong không gian đối ngẫu $F'$ của $F$ tồn tại một dãy $(a'_n)$ trù mật đối với tôpô yếu $\sigma(F', F)$ (TVS, II, §6, No. 2). Để hai ánh xạ $f, g$ từ $X$ vào $F$ tương đương, điều kiện cần và đủ là, với mọi n, các hàm số $\langle f(x), a'_n \rangle$ và $\langle g(x), a'_n \rangle$ tương đương.

Điều kiện này hiển nhiên là cần. Ngược lại, nếu điều kiện ấy được thỏa mãn, tồn tại một tập không đáng kể $H$ sao cho, với mỗi $x \notin H$, $\langle f(x), a'_n \rangle$ = $\langle g(x), a'_n \rangle$ với mọi n; điều này có nghĩa là các dạng tuyến tính liên tục yếu $z' \mapsto \langle f(x), z' \rangle$ và $z' \mapsto \langle g(x), z' \rangle$ trên $F'$ bằng nhau tại từng điểm $a'_n$, do đó trùng nhau nhờ giả thiết, điều đó chứng tỏ rằng $f(x) = g(x)$ với mọi $x \notin H$.

Chú ý rằng giả thiết của Mệnh đề 10 áp dụng đặc biệt khi $F$ là một không gian lồi địa phương mêtric hóa và tách được¹ (TVS, III, §3, No. 4, Hệ quả 2 của Mệnh đề 6).

### 5. Hàm được xác định hầu khắp nơi

Theo đúng định nghĩa ở No. 3, một ánh xạ $f$ của một tập con $A$ của $X$ vào một tập hợp $F$ được gọi là được xác định hầu khắp nơi nếu phần bù của tập $A$ trên đó nó được xác định là một tập không đáng kể. Ta lại gọi lớp tương đương của $f$, và ký hiệu là $\tilde{f}$, là lớp tương đương của mọi hàm được xác định trên toàn bộ $X$ và bằng $f(x)$ tại các điểm $x \in X$ nơi $f$ được xác định; hiển nhiên lớp này chỉ phụ thuộc vào $f$. Hai hàm được xác định hầu khắp nơi $f, g$ lại được gọi là tương đương nếu $\tilde{f} = \tilde{g}$: điều đó có nghĩa là, do đó, tập các điểm mà $f(x)$ và $g(x)$ đều được xác định và bằng nhau có phần bù không đáng kể.

Suy ra ngay rằng Mệnh đề 8 của No. 4 và hệ quả của nó có thể được tổng quát hóa sang trường hợp mà trong phát biểu của chúng chỉ giả thiết rằng mỗi hàm $f_n, g_n$ đều được xác định hầu khắp nơi; khi đó các hàm $\varphi((f_n))$

¹ Nguyên văn là de type dénombrable, cũng được dịch là 'kiểu đếm được' (GT, IX, §2, No. 8, Định nghĩa 4) hoặc 'có cơ sở đếm được', hoặc 'thỏa mãn tiên đề đếm được thứ hai'. Trong hệ quả được dẫn ở đây từ TVS, thuật ngữ 'thỏa mãn tiên đề đếm được thứ nhất' nên được thay bằng một trong các thuật ngữ nói trên.

và $\varphi((g_n))$ bản thân chúng cũng được xác định hầu khắp nơi; lớp tương đương của $\varphi((f_n))$ lại là $\varphi((\tilde{f}_n))$.

Một hàm được xác định hầu khắp nơi, nhận giá trị trong một không gian vectơ F, cũng được gọi là *không đáng kể* nếu nó tương đương với 0. Nếu f là một hàm không đáng kể nhận giá trị trong F, và u là một ánh xạ tuyến tính của F vào một không gian vectơ G, thì hàm hợp $u \circ f$ (được xác định hầu khắp nơi) là không đáng kể; tương tự, với mọi hàm số (hữu hạn) g, được xác định hầu khắp nơi, hàm $gf$ (được xác định hầu khắp nơi) là không đáng kể.

Cần chú ý rằng, trong tập các hàm nhận giá trị trong F và được xác định hầu khắp nơi, luật hợp thành nội bộ $(f, g) \mapsto f + g$ *không phải là một luật nhóm*, vì, tuy hàm 0 quả thực là một phần tử trung hòa đối với luật này, nhưng nếu f không được xác định mọi nơi thì không tồn tại hàm g sao cho $f + g = 0$. Đó là lý do đưa vào các lớp tương đương $\tilde{f}$, và chúng thực sự tạo thành một không gian vectơ.

Cho $(f_n)$ là một dãy các ánh xạ vào một *không gian tôpô* F, mỗi ánh xạ đều được xác định hầu khắp nơi trong X. Ta nói rằng dãy $(f_n)$ *hội tụ (theo điểm) hầu khắp nơi đến f trong* X nếu tập các điểm $x \in X$ mà tại đó mọi $f_n(x)$ đều được xác định và dãy $(f_n(x))$ có giới hạn bằng $f(x)$, có phần bù không đáng kể. Rõ ràng rằng nếu, với mỗi n, hàm $g_n$ (được xác định hầu khắp nơi) tương đương với $f_n$, thì dãy $(g_n)$ hội tụ hầu khắp nơi đến f.

Nếu F là một *không gian vectơ tôpô*, ta định nghĩa tương tự một *chuỗi hội tụ hầu khắp nơi*, mà số hạng tổng quát là một hàm $f_n$ được xác định hầu khắp nơi trong X với giá trị trong F; tổng của chuỗi này là một hàm được xác định tại các điểm mà các tổng riêng $\sum_{k=1}^n f_k(x)$ được xác định và có giới hạn, và lớp của nó chỉ phụ thuộc vào các lớp $\tilde{f}_n$.

### 6. Các lớp tương đương của các hàm với giá trị trong $\overline{\mathbf{R}}$

Phù hợp với định nghĩa ở No. 3, ta nói rằng một hàm $f$, được xác định hầu khắp nơi trong X và nhận giá trị trong $\overline{\mathbf{R}}$, là *hữu hạn hầu khắp nơi* nếu tập các $x \in X$ sao cho $f(x)$ được xác định và hữu hạn có phần bù không đáng kể. Một hàm hữu hạn hầu khắp nơi tương đương với một hàm *hữu hạn mọi nơi*; vì thế ta có thể đồng nhất lớp $\tilde{f}$ của nó với một lớp các hàm số *hữu hạn* được xác định trên X (hoặc hầu khắp nơi trên X). Đặc biệt, tổng và tích của hai lớp các hàm hữu hạn hầu khắp nơi được xác định, và tập các lớp đó là một *đại số* trên $\mathbf{R}$. Nếu $(f_n)$ là một dãy các hàm với giá trị trong $\overline{\mathbf{R}}$, được xác định và hữu hạn hầu khắp nơi, thì các tổng riêng $\sum_{k=1}^n f_k(x)$ được xác định hầu khắp nơi; nếu, với hầu mọi $x \in X$, chúng có giới hạn $f(x)$ trong $\overline{\mathbf{R}}$, ta lại nói rằng chuỗi có số hạng tổng quát $f_n$ hội tụ hầu khắp nơi và rằng $f$ là tổng của chuỗi đó (lưu ý rằng $f$ không nhất thiết hữu hạn hầu khắp nơi).

Nếu $f$ và $g$ là hai hàm số được xác định và hữu hạn hầu khắp nơi trong $X$, thì $\tilde{f} + \tilde{g}$ (tương ứng $\tilde{f} \tilde{g}$) là lớp của mọi hàm bằng $f(x) + g(x)$ (tương ứng $f(x)g(x)$) tại các điểm $x \in X$ nơi biểu thức này có nghĩa. Lưu ý rằng f và g đều có thể *được xác định mọi nơi* mà không nhất thiết $f(x) + g(x)$ (tương ứng $f(x)g(x)$) được xác định với mọi $x$ (GT, IV, §4, No. 3); theo định nghĩa, $f + g$ (tương ứng $fg$) khi đó là hàm bằng $f(x) + g(x)$ (tương ứng $f(x)g(x)$) tại các điểm mà biểu thức này được xác định; vì vậy nó chỉ được xác định hầu khắp nơi.

Cho $f$ và $g$ là hai hàm số (hữu hạn hay không) được xác định hầu khắp nơi trên $X$ và sao cho $f(x) \leq g(x)$ hầu khắp nơi; nếu $f_1$ tương đương với $f$, và $g_1$ tương đương với $g$, thì hiển nhiên cũng có $f_1(x) \leq g_1(x)$ hầu khắp nơi. Do đó quan hệ đang xét chỉ phụ thuộc vào các lớp của $f$ và $g$; ta viết $\tilde{f} \leq \tilde{g}$, và người ta kiểm tra ngay rằng quan hệ này là một *quan hệ thứ tự* trên tập hợp các lớp tương đương của các hàm số nhận giá trị trong $\overline{\mathbf{R}}$. Nếu $(\tilde{f}_n)$ là một họ đếm được (hữu hạn hay vô hạn) của các lớp như vậy và nếu, với mọi $n$, $f_n$ và $g_n$ là hai hàm số được xác định hầu khắp nơi và thuộc lớp $\tilde{f}_n$, thì theo Mệnh đề 8 của No. 4, các hàm số $\sup_n f_n$ và $\sup_n g_n$, được xác định hầu khắp nơi, là tương đương; do đó lớp của chúng chỉ phụ thuộc vào các lớp $\tilde{f}_n$, và ta kiểm tra ngay rằng đó là *cận trên đúng* $\sup_n \tilde{f}_n$ của các lớp này trong tập hợp các lớp của các hàm số nhận giá trị trong $\overline{\mathbf{R}}$, được sắp thứ tự theo cách vừa mô tả (một tập hợp vì thế, nói riêng, *có thứ tự dàn*). Người ta cũng chứng minh tương tự sự tồn tại của cận dưới đúng $\inf_n \tilde{f}_n$, và ta có $\inf_n \tilde{f}_n = -\sup_n (-\tilde{f}_n)$. Suy ra rằng $\limsup_{n \to \infty} f_n$ và $\limsup_{n \to \infty} g_n$ cũng tương đương, và lớp của chúng, được ký hiệu $\limsup_{n \to \infty} \tilde{f}_n$, bằng $\inf_n (\sup_{p \geq 0} \tilde{f}_{n+p})$; $\liminf_{n \to \infty} \tilde{f}_n$ được định nghĩa tương tự.

Một hàm số $f$ (hữu hạn hay không) được gọi là *không đáng kể* nếu nó tương đương với 0; định nghĩa này tương đương với Định nghĩa 1 đối với các hàm số dương và được xác định ở mọi nơi, nhờ Định lý 1. Để $f$ là không đáng kể, điều kiện cần và đủ là $|f|$ không đáng kể (hay là cả $f^+$ và $f^-$ đều không đáng kể).
