---
book: ac
book_title: Commutative Algebra
chapter: VI
chapter_title: VALUATIONS
section: 2
section_title: Places
lang: vi
source: ac-i-vii
book_pages: 381-385, 444-446
pdf_pages: 0399-0403, 0462-0464
extraction: ocr
subsections:
    - "no": 1
      title: THE NOTION OF MORPHISM FOR LAWS OF COMPOSITION NOT EVERYWHERE DEFINED
      page: 381
      pdf_page: 399
    - "no": 2
      title: PLACES
      page: 381
      pdf_page: 399
    - "no": 3
      title: PLACES AND VALUATION RINGS
      page: 383
      pdf_page: 401
    - "no": 4
      title: EXTENSION OF PLACES
      page: 384
      pdf_page: 402
    - "no": 5
      title: CHARACTERIZATION OF INTEGRAL ELEMENTS BY MEANS OF PLACES
      page: 385
      pdf_page: 403
statements: 9
exercises: 3
content_sha256: 539f8a9893125fe545b5e78ad46cddf42f6b4d8151132f9e53dc586a84bc8474
translated_from: content/en/ac/VI/02_s2_places.md
source_content_sha256: 77317d3d786c749ffbfb7d9d7477860a00cdaffa086276cdf73ac7a545e3297d
translation_model: gpt-5-6-mini, gpt-5-6
translation_run: translate-vi-ae5239b0
glossary_version: 34
glossary_terms_sha256: 3e249044d53fdf6b6866580418faeecb036325b0fec753c456d43acdf0dbeb58
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 2. CÁC VỊ TRÍ

### 1. KHÁI NIỆM CẤU XẠ ĐỐI VỚI CÁC LUẬT HỢP THÀNH KHÔNG ĐƯỢC XÁC ĐỊNH KHẮP NƠI

#### Định nghĩa 1 {#ac-vi-s2-def-1 .statement}

*Cho E và E' là hai tập hợp, mỗi tập hợp có một luật hợp thành trong được ký hiệu bởi $(x, y) \mapsto x * y$, không nhất thiết được xác định khắp nơi. Một ánh xạ $f : E \to E'$ là một cấu xạ nếu, với mọi $x, y$ trong E sao cho $f(x) * f(y)$ được xác định, hợp thành $x * y$ cũng được xác định và:*

(1)
$$
f(x * y) = f(x) * f(y).
$$
Nói ngắn gọn hơn, ta có thể nói rằng công thức (1) phải đúng mỗi khi vế phải có nghĩa.

Khái niệm cấu xạ phân biệt với khái niệm biểu diễn (*Đại số*, Chương I, § 1, no. 1), trong đó yêu cầu rằng phương trình (1) đúng bất cứ khi nào vế trái có nghĩa. Dĩ nhiên, hai khái niệm trùng nhau đối với các luật hợp thành được xác định khắp nơi.

#### Định nghĩa 2 {#ac-vi-s2-def-2 .statement}

*Cho E và E' là hai tập hợp, mỗi tập hợp có một họ các luật hợp thành trong $(x, y) \mapsto x *_{\alpha} y, \alpha \in I$. Một ánh xạ $f : E \to E'$ là một cấu xạ nếu nó là một cấu xạ đối với mỗi luật hợp thành $(x, y) \mapsto x *_{\alpha} y$.*

Cũng như các biểu diễn, các cấu xạ thỏa mãn các tiên đề (MO_I), (MO_{II}), (MO_{III}) của *Lý thuyết tập hợp*, Chương IV, § 2. Nếu: $E \to E'$ là một cấu xạ, thì $f(E)$ là một tập con ổn định của $\mathbf{R}'$.

### 2. CÁC VỊ TRÍ

Nếu K là một trường, nhắc lại rằng $\mathbf{K}$ ký hiệu tập hợp là tổng của K và một phần tử được ký hiệu bởi $\infty$ (*Đại số*, Chương 11, § 9, no. 9); các luật hợp thành của K mở rộng tới $\mathbf{K}$ bằng cách đặt (*loc. cit.*)

(2)
$$
a + \infty = \infty \quad \text{với } a \in \mathbf{K}, \quad a \neq \infty,
$$
(3)
$$
\infty . a = a . \infty = \infty \quad \text{với } a \in \tilde{\mathbf{K}}, \quad a \neq 0.
$$

Các hợp thành duy nhất không được xác định do đó là các hợp thành của $+ \infty$, $\infty . 0$ và $0 . \infty$. Mặt khác, các ánh xạ $x \mapsto -x$ và $x \mapsto x^{-1}$ mở rộng tương tự tới $\tilde{K}$ bằng cách đặt $-\infty = \infty, 0^{-1} = \infty, \infty^{-1} = 0$. Ta cũng sẽ viết $x + (-y) = x - y$.

Tập hợp $\tilde{K}$, được gọi là *trường xạ ảnh* liên kết với $K$, có thể được đồng nhất với *đường thẳng xạ ảnh* $P_1(K)$ (*loc. cit.*).

#### Định nghĩa 3 {#ac-vi-s2-def-3 .statement}

*Cho $K$ và $L$ là hai trường. Mọi cấu xạ* $f$ *của* $K$ *vào* $\tilde{L}$ *(đối với phép cộng và phép nhân)* *sao cho* $f(1) = 1$ *được gọi là một vị trí của* $K$ *với các giá trị trong* $L$.

Nói cách khác, nếu $x$ và $y$ là các phần tử của $K$ và $f(x) + f(y)$ (resp. $f(x)f(y)$) được xác định, thì $x + y$ (resp. $xy$) được xác định và

$$
f(x + y) = f(x) + f(y)
$$
$$
f(xy) = f(x)f(y).
$$

Vì $\infty + \infty$ không được xác định, nên $f(\infty) + f(\infty)$ cũng không được xác định, điều này chỉ ra rằng
$$
f(\infty) = \infty.
$$

Tương tự, vì $0 \cdot \infty$ không được xác định, nên $f(0)f(\infty)$ cũng không được xác định, điều này, nhờ vào (6), suy ra
$$
f(0) = 0.
$$

Mặt khác
$$
f(a^{-1}) = f(a)^{-1} \quad \text{với mọi } a \in \tilde{K}.
$$

Nếu $f(a)f(a^{-1})$ được xác định, $aa^{-1}$ được xác định và do đó bằng 1; khi đó $f(a)f(a^{-1}) = f(1) = 1$, điều này chứng minh (8) trong trường hợp này. Nếu $f(a)f(a)^{-1}$ không được xác định, thì hoặc là $f(a) = 0$ và $f(a^{-1}) = \infty$ hoặc là $f(a) = \infty$ và $f(a^{-1}) = 0$ và (8) vẫn đúng.

Tương tự có thể chỉ ra rằng
$$
f(-a) = -f(a) \quad \text{với mọi } a \in K.
$$

Từ các công thức (8) và (9) suy ra rằng $f$ cũng là một cấu xạ đối với các luật hợp thành $(x, y) \mapsto x - y$ và $(x, y) \mapsto xy^{-1}$.

Đối với $x \in \tilde{K}$, $f$ được gọi là hữu hạn tại $x$ nếu $f(x) \neq \infty$; điều này kéo theo $x \in K$ theo (6).

Nếu $f : K \to \tilde{L}$ là một nơi, $f(K)$ là một tập con của $\tilde{L}$ ổn định đối với các luật hợp thành $(x, y) \mapsto x + y, (x, y) \mapsto x - y, (x, y) \mapsto xy$ và $(x, y) \mapsto xy^{-1}$ và chứa 1. Nếu E là tập hợp các phần tử hữu hạn của $f(\tilde{K})$, E là một trường con của L và $f(\tilde{K}) = \tilde{E}$. Do lạm dụng ngôn ngữ, E được gọi là *trường giá trị* của f.

Ánh xạ *hợp thành* của hai nơi là một nơi.

Cho F là một đẳng cấu của một trường K lên một trường con của một trường L; ta mở rộng $f$ tới $K$ bằng cách đặt $f(\infty) = \infty$. Như vậy ta thu được một nơi của K với các giá trị trong L được gọi là *tầm thường* và thường được đồng nhất với đẳng cấu $f$.

### 3. CÁC NƠI VÀ CÁC VÀNH ĐỊNH GIÁ

#### Mệnh đề 1 {#ac-vi-s2-prop-1 .statement}

Cho K là một trường, $\mathbf{A}$ là một vành định giá của K và $\kappa(\mathbf{A})$ là trường thặng dư của $\mathbf{A}$. Ta mở rộng ánh xạ chính tắc của $\mathbf{A}$ lên $\kappa(\mathbf{A})$ thành một ánh xạ $h_{\mathbf{A}} : \tilde{K} \to (\kappa(\mathbf{A}))$ bởi công thức $h_{\mathbf{A}}(x) = \infty$ nếu $x \notin \mathbf{A}$. Ánh xạ $h_{\mathbf{A}}$ được xác định như vậy là một nơi của K mà trường giá trị của nó là $\kappa(\mathbf{A})$.

Rõ ràng $h_{\mathbf{A}}(1) = 1$.

Ta chứng minh rằng $h_{\mathbf{A}}$ là một cấu xạ đối với phép cộng. Cho $x, y$ là hai phần tử của $\tilde{K}$ sao cho $h_{\mathbf{A}}(x) + h_{\mathbf{A}}(y)$ được xác định. Khi đó một trong hai phần tử $x, y$ thuộc về $\mathbf{A}$ và do đó $x + y$ được xác định. Nếu $x \in \mathbf{A}$ và $y \in \mathbf{A}$, rõ ràng

$$
h_{\mathbf{A}}(x) + h_{\mathbf{A}}(y) = h_{\mathbf{A}}(x + y)
$$

đúng. Nếu $x \in \mathbf{A}$ và $y \notin \mathbf{A}$, thì $x + y \notin \mathbf{A}$ và hai vế của công thức trên đều bằng $\infty$.

Cuối cùng ta chứng minh rằng $h_{\mathbf{A}}$ là một cấu xạ đối với phép nhân. Cho $x \in K, y \in K$ sao cho $h_{\mathbf{A}}(x)h_{\mathbf{A}}(y)$ được xác định. Nếu $x \in \mathbf{A}$ và $y \in \mathbf{A}$, rõ ràng $xy$ được xác định và $h_{\mathbf{A}}(x)h_{\mathbf{A}}(y) = h_{\mathbf{A}}(xy)$. Bây giờ giả sử rằng một trong các phần tử $x, y$, chẳng hạn $y$, không thuộc $\mathbf{A}$; vì $h_{\mathbf{A}}(y) = \infty$, $h_{\mathbf{A}}(x) \neq 0$, nghĩa là $x \notin m(\mathbf{A})$, do đó $x^{-1} \in \mathbf{A}$; suy ra $xy$ được xác định và $xy \notin \mathbf{A}$, do đó

$$
h_{\mathbf{A}}(xy) = \infty = h_{\mathbf{A}}(x)h_{\mathbf{A}}(y).
$$

Điều này chứng minh Mệnh đề 1.

Nếu $j$ là một đẳng cấu của $\kappa(\mathbf{A})$ lên một trường con của một trường L, $j \circ h_{\mathbf{A}} : \tilde{K} \to \tilde{L}$ là một nơi của K với các giá trị trong L. Quá trình trên thực sự cung cấp tất cả các nơi trên K. Nói chính xác hơn:

#### Mệnh đề 2 {#ac-vi-s2-prop-2 .statement}

Cho K và L là hai trường và f là một nơi của K với các giá trị trong L. Khi đó tồn tại một vành định giá $\mathbf{A}$ của K và một đẳng cấu $j$ của $\kappa(\mathbf{A})$ lên một trường con của L sao cho $f = j \circ h_{\mathbf{A}}$; các điều kiện này xác định $\mathbf{A}$ và $j$ một cách duy nhất. Vành $\mathbf{A}$ là tập hợp các $x \in K$ sao cho $f(x) \neq \infty$ và $m(\mathbf{A})$ là tập hợp các $x \in K$ sao cho $f(x) = 0$.

Nếu $f = j \circ h_{\mathbf{A}}$, điều kiện $f(x) \neq \infty$ (tương ứng. $f(x) = 0$) tương đương với điều kiện $h_{\mathbf{A}}(x) \neq \infty$ (tương ứng. $h_{\mathbf{A}}(x) = 0$) và do đó với điều kiện $x \in \mathbf{A}$ (tương ứng. $x \in m(\mathbf{A})$). Do đó $\mathbf{A}$ được xác định duy nhất và, vì $h_{\mathbf{A}}$ là toàn ánh, $j$ cũng là duy nhất.

Bây giờ cho $f$ là một place bất kỳ của K có các giá trị trong L; ký hiệu $\mathbf{A}$ là tập hợp các $x \in K$ sao cho $f(x) \neq \infty$. Nếu $x \in \mathbf{A}$ và $y \in \mathbf{A}$, các hợp thành $f(x) - f(y)$ và $f(x)f(y)$ được xác định và $\neq \infty$, điều này cho thấy rằng $x - y \in \mathbf{A}$ và $xy \in \mathbf{A}$; do đó $\mathbf{A}$ là một vành con của K. Nếu $x \notin \mathbf{A}$, thì $f(x) = \infty$, do đó $f(x^{-1}) = 0$ và $x^{-1}$ thuộc hạt nhân $m$ của đồng cấu $f'$ thu được bằng cách hạn chế $f$ vào $\mathbf{A}$. Ngược lại nếu $y \in m$, thì $y^{-1} \notin \mathbf{A}$. Điều này cho thấy rằng $\mathbf{A}$ là một vành định giá của K và rằng $m$ là iđêan cực đại của nó. Gọi $j$ là đơn cấu từ $\kappa(\mathbf{A})$ vào L dẫn xuất từ f' bằng cách chuyển qua thương. Khi đó $f(x) = j(h_A(x))$ với mọi $x \in A$ và đẳng thức này vẫn đúng với $x \notin A$, khi đó hai vế đều bằng $\infty$.

Phân tích $f = j \circ h_A$ được gọi là phân tích chính tắc của placef. $A$ được gọi là vành của f, $m(A)$ là iđêan của $f$ và $\kappa(A)$ là trường thặng dư của f. Để hai place $f : \mathbf{K} \to \mathbf{L}$ và $f' : \mathbf{K} \to \mathbf{L}'$ có cùng một vành, điều kiện cần và đủ là tồn tại một đẳng cấu của trường giá trị của f lên trường giá trị của f' sao cho $f' = s \circ f$; khi đó $f$ và $f'$ được gọi là tương đương. Ta thấy rằng mọi kết quả về các vành định giá có thể được chuyển thành một kết quả về các place và ngược lại; đó là điều chúng ta sẽ thực hiện trong các số tiếp theo.

Các ví dụ về các điểm
(1) Cho $K$ là một trường. Ánh xạ đồng nhất trên $K$ là một điểm tầm thường với vành $K$ và iđêan $(0)$.
(2) Cho $k$ là một trường. Với mọi $u \in k((T))^\sim$, ta viết $f(u) = \infty$ nếu $u \notin k[[T]]$ và định nghĩa $f(u)$ là số hạng hằng của $u$ nếu $u \in k[[T]]$. Khi đó $f$ là một điểm của $k((T))$, với trường thặng dư $k$ và vành $k[[T]]$. Vì $k[[T]]$ là một vành định giá của $k((T))$ (\S 1, no. 4, Ví dụ 3 ) và hạn chế của $f$ trên $k[[T]]$ được đồng nhất với đồng cấu chính tắc của $k[[T]]$ lên trường thặng dư của nó.
(3) Cho $k$ là một trường, $a$ là một phần tử của $k$ và $A$ là tập hợp các $u \in k(X)$ sao cho $a$ có thể thế vào $u$ (Đại số, Chương IV, \S 3, no. 2). Nếu $p$ ký hiệu iđêan nguyên tố $(X - a)$ của $k[X]$, thì $A = k[X]_p$, do đó $A$ là một vành định giá của $k(X)$ (\S 1, no. 4, Mệnh đề 2). Với mọi $u \in k(X)^\sim$, ta viết $f(u) = \infty$ nếu $u \notin A$ và $f(u) = u(a)$ nếu $u \in A$. Khi đó $f$ là một điểm của $k(X)$ với trường thặng dư $k$ và vành $A$; vì hạn chế của f trên $A$ là một đồng cấu từ $A$ lên $k$ (Đại số, Chương IV, \S 3, Mệnh đề 2) có hạt nhân $pA = m(A)$. Phần tử $f(u) \in k$ được gọi là thu được bằng cách đặt $X = a$ trong $u$.
\* (4) Cho $S$ là một đa tạp giải tích phức liên thông có chiều 1 và $K$ là trường các hàm phân hình trên $S$. Với mọi $z_0 \in S$, ánh xạ $f \mapsto f(z_0)$ từ $K$ đến $\mathbf{C}$ là một điểm của $K$, có vành là tập hợp các $f \in K$ giải tích tại $z_0$ và có iđêan là tập hợp các $f \in K$ bằng không tại $z_0$. Chính ví dụ này và các ví dụ tương tự khác là nguồn gốc của thuật ngữ "điểm".*

### 4. MỞ RỘNG CỦA CÁC VỊ TRÍ

#### Mệnh đề 3 {#ac-vi-s2-prop-3 .statement}

Cho $K$ là một trường, $S$ là một vành con của $K$ và $f$ là một đồng cấu từ $S$ vào một trường đóng đại số $L$. Khi đó tồn tại một vị trí của $K$ với giá trị trong $L$ mở rộng $f$.

Xét đến Mệnh đề 1, đây là bản dịch của Định lý 2 của \S 1, no. 2.

#### Mệnh đề 4 {#ac-vi-s2-prop-4 .statement}

Cho $K$ là một trường, $f$ là một vị trí của $K$ với giá trị trong một trường $L$ và $K'$ là một mở rộng của $K$. Khi đó tồn tại một mở rộng $L'$ của $L$ và một vị trí $f'$ của $K'$ với giá trị trong $L'$ mở rộng $f$. Nếu $x_1, \ldots, x_n$ là các phần tử của $K$ độc lập đại số trên $K$ và $a,, \ldots, a,,$ là các phần tử bất kỳ $\in L, f'$ có thể được chọn sao cho $f(x_i) = a,$ với $1 \leq i \leq n.$

Gọi $V$ là vành off, $g$ là hạn chế của f lên $V$ và $g'$ là mở rộng của $g$ lên $V[x_1, \ldots, x_n]$ sao cho $g'(x_i) = a,$ với $1 \leq i \leq n.$ Chỉ cần lấy $L'$ là một bao đóng đại số của $L$ và áp dụng Mệnh đề 3 cho $g'$ và $L'$: ta thu được một vị tríf': $K' \to \tilde{L}'$ mở rộng $g'$; nếu $x \in K - V,$ thì $x^{-1} \in m(V),$ do đó $f(x^{-1}) = g(x^{-1}) = 0$ và $f'(x) = \infty = f(x);$ do đóf' mở rộngf.

### 5. ĐẶC TRƯNG HÓA CÁC PHẦN TỬ NGUYÊN BẰNG CÁC VỊ TRÍ

#### Mệnh đề 5 {#ac-vi-s2-prop-5 .statement}

Cho $K$ là một trường, $S$ là một vành con của $K, h$ là một đồng cấu từ $S$ vào một trường và $p$ là hạt nhân của $h.$ Để một phần tử $x$ của $K$ là nguyên trên vành địa phương $S,$ điều kiện cần và đủ là mọi vị trí của $K$ mở rộng $h$ đều hữu hạn tại $x.$

Nếu $f$ là một vị trí của $K$ mở rộng $h, f$ hữu hạn trên $S_p$ và không trên $pS_p$ và do đó vành của vị trí $f$ trội $S_p.$ Ngược lại, nếu $V$ là một vành định giá của $K$ trội $S_p,$ $V$ là vành của một vị tríf mà hạn chế của nó trên $S$ là một đồng cấu có cùng hạt nhân như $h;$ thay thế $f$ bởi một vị trí tương đương, ta thấy rằng $V$ là vành của một vị trí của $K$ mở rộng $h.$ Nói rằng mọi vị trí của $K$ mở rộng $h$ đều hữu hạn tại $x$ tương đương với nói rằng $x$ thuộc mọi vành định giá của $K$ trội $S_p.$ Mệnh đề khi đó suy ra từ Định lý 3 của § 1, no. 3.

#### Mệnh đề 6 {#ac-vi-s2-prop-6 .statement}

Cho $K$ là một trường và $S$ là một vành con của $K.$ Để một phần tử $x \in K$ là nguyên trên $S,$ điều kiện cần và đủ là mọi vị trí của $K$ hữu hạn trên $S$ đều hữu hạn tại $x.$

Đây cũng là một hệ quả của Định lý 3 của § 1, no. 3.

### Bài tập {#ac-vi-s2-exercises}

Xem các [bài tập cho § 2](exercises/s2/).
