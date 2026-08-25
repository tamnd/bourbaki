---
book: fvr
book_title: Functions of a Real Variable
chapter: II
chapter_title: PRIMITIVES AND INTEGRALS
section: 1
section_title: PRIMITIVES AND INTEGRALS
lang: vi
source: fvr-i-vii
pdf_pages: 0066-0077, 0094-0099
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF PRIMITIVES
      page: 0
      pdf_page: 66
    - "no": 2
      title: EXISTENCE OF PRIMITIVES
      page: 0
      pdf_page: 67
    - "no": 3
      title: REGULATED FUNCTIONS
      page: 0
      pdf_page: 68
    - "no": 4
      title: INTEGRALS
      page: 0
      pdf_page: 71
    - "no": 5
      title: PROPERTIES OF INTEGRALS
      page: 0
      pdf_page: 74
    - "no": 6
      title: INTEGRAL FORMULA FOR THE REMAINDER IN TAYLOR'S FORMULA; PRIMITIVES OF HIGHER ORDER
      page: 0
      pdf_page: 77
statements: 28
exercises: 10
content_sha256: 4202119dd1551af6747cee9f733ef6b1c2e895cb0c930eb22978efb53183ea6a
translated_from: content/en/fvr/II/01_s1_primitives_and_integrals.md
source_content_sha256: ff30f9508044e05296fa35eac9891d983060ac6f9e5e128e409343cc51396165
translation_model: gpt-5-6, gpt-5-6-mini, gpt-5.4-mini
translation_run: translate-vi-e581a0ef
glossary_version: 34
glossary_terms_sha256: 9639dd7f8620cdc77587455cfd34d1d6ac660ca1766ce7d88921fd67001f6884
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 1. NGUYÊN THỦY HÀM VÀ TÍCH PHÂN

Trừ khi có nói rõ ngược lại, trong chương này chúng ta chỉ xét các hàm vectơ của một biến thực nhận giá trị trong một không gian định chuẩn đầy đủ trên $\mathbf{R}$. Khi đặc biệt xét các hàm nhận giá trị thực, luôn luôn hiểu rằng các hàm này là hữu hạn, trừ khi có nói ngược lại.

### 1. ĐỊNH NGHĨA NGUYÊN THỦY HÀM

Một hàm vectơ $f$ xác định trên một khoảng $I \subset \mathbf{R}$ không thể là đạo hàm tại mọi điểm của khoảng này của một hàm vectơ $g$ (được xác định và liên tục trên $I$), trừ khi nó thỏa mãn những điều kiện khá chặt chẽ: chẳng hạn, nếu $f$ có giới hạn phải và giới hạn trái tại một điểm $x_0$ nằm trong $I$ thì $f$ phải liên tục tại điểm $x_0$, như suy ra từ mệnh đề 6 của I, p. 18; do đó, nếu lấy khoảng $[ -1 , 1 ]$ làm $I$, và lấy $f$ là hàm thực bằng $-1$ trên $[ -1 , 0[$, và bằng $+1$ trên $[0 , 1]$, thì $f$ không phải là đạo hàm của bất kỳ hàm liên tục nào trên $I$; tuy vậy, hàm $|x|$ có $f(x)$ làm đạo hàm tại mọi điểm $\neq 0$; vì thế người ta đi đến định nghĩa sau đây:

#### Định nghĩa 1 {#fvr-ii-s1-def-1 .statement}

*Cho một hàm vectơ $f$ xác định trên một khoảng $I \subset \mathbf{R}$, ta nói rằng một hàm $g$ xác định trên $I$ là một nguyên thủy hàm của $f$ nếu $g$ liên tục trên $I$ và có đạo hàm bằng $f(x)$ tại mọi điểm $x$ thuộc phần bù (đối với $I$) của một tập con đếm được của $I$.*

Nếu thêm nữa $g$ có đạo hàm bằng $f(x)$ tại mọi điểm $x$ của $I$, thì ta nói rằng $g$ là một nguyên thủy hàm ngặt của $f$.

Với định nghĩa này, ta thấy rằng hàm thực $f$ đã xét ở trên có một nguyên thủy hàm bằng $|x|$.

Rõ ràng là nếu $f$ có một nguyên thủy hàm trên $I$ thì mọi nguyên thủy hàm của $f$ cũng là nguyên thủy hàm của mọi hàm bằng $f$ ngoại trừ tại các điểm của một tập con đếm được của $I$. Theo một cách nói lỏng, người ta nói đến một nguyên thủy hàm trên $I$ của một hàm $f_0$ chỉ được xác định trên phần bù (đối với $I$) của một tập con đếm được của $I$: đó sẽ là nguyên thủy hàm của mọi hàm $f$ xác định trên $I$ và bằng $f_0$ tại các điểm mà $f_0$ được xác định.

#### Mệnh đề 1 {#fvr-ii-s1-prop-1 .statement}

*Cho $f$ là một hàm vectơ được định nghĩa trên $I$ với các giá trị trong $E$; nếu $f$ nhận một nguyên hàm $g$ trên $I$ thì tập hợp các nguyên hàm của $f$ trên $I$ đồng nhất với tập hợp các hàm $g + a$, trong đó $a$ là một hàm hằng với các giá trị của nó trong $E$.*

Thật vậy, rõ ràng rằng $g + a$ là một nguyên hàm của $f$ với mọi $a \in E$; mặt khác, nếu $g_1$ là một nguyên hàm của $f$ thì $g_1 - g$ có một đạo hàm bằng 0 trừ tại các điểm của một tập con đếm được của $I$, và do đó là hằng (I, p. 17, hệ quả).

Người ta nói rằng các nguyên hàm của một hàm $f$ (khi chúng tồn tại) được định nghĩa “sai khác một hằng cộng tính”. Để định nghĩa một nguyên hàm của $f$ một cách không nhập nhằng, chỉ cần gán cho nó (tùy ý) một giá trị tại một điểm $x_0 \in I$; đặc biệt, tồn tại một và chỉ một nguyên hàm $g$ của $f$ sao cho $g(x_0) = 0$; với mọi nguyên hàm $h$ của $f$ ta có $g(x) = h(x) - h(x_0)$.

### 2. SỰ TỒN TẠI CỦA CÁC NGUYÊN HÀM

Cho $f$ là một hàm được định nghĩa trên một khoảng tùy ý $I \subset \mathbf{R}$; để một hàm $g$ được định nghĩa trên $I$ là một nguyên hàm của $f$, điều kiện cần và đủ là hạn chế của $g$ trên mọi khoảng compact $J \subset I$ là một nguyên hàm của hạn chế của $f$ trên $J$.

#### Định lý 1 {#fvr-ii-s1-thm-1 .statement}

*Cho $A$ là một tập hợp được lọc bởi một bộ lọc $\mathfrak{F}$, và $(f_\alpha)_{\alpha \in A}$ là một họ các hàm vectơ với các giá trị trong một không gian định chuẩn đầy đủ $E$ trên $\mathbf{R}$, được định nghĩa trên một khoảng $I \subset \mathbf{R}$: với mỗi $\alpha \in A$ cho $g_\alpha$ là một nguyên hàm của $f_\alpha$. Ta giả sử rằng:
1. đối với bộ lọc $\mathfrak{F}$ các hàm $f_\alpha$ hội tụ đều trên mọi tập con compact của $I$ đến một hàm $f$;
2. tồn tại một điểm $a \in I$ sao cho, đối với bộ lọc $\mathfrak{F}$, họ $(g_\alpha(a))$ có một giới hạn trong $E$.
Dưới các giả thiết này các hàm $g_\alpha$ hội tụ đều (đối với $\mathfrak{F}$) trên mọi tập con compact của $I$ đến một nguyên hàm $g$ của $f$.*

Theo nhận xét ở đầu tiểu mục này, ta có thể hạn chế vào trường hợp $I$ là một khoảng *compact*.

Trước hết hãy chứng minh rằng các $g_\alpha$ hội tụ đều trên $I$ đến một hàm liên tục $g$. Theo giả thiết, với mọi $\varepsilon > 0$ tồn tại một tập hợp $M \in \mathfrak{F}$ sao cho, với mọi hai chỉ số $\alpha, \beta$ thuộc $M$, ta có $\|f_\alpha(x) - f_\beta(x)\| \leq \varepsilon$ với mỗi $x \in I$; hệ quả là ta có (I, p. 15, đl. 2)

$$
\|g_\alpha(x) - g_\beta(x) - (g_\alpha(a) - g_\beta(a))\| \leq \varepsilon |x - a| \leq \varepsilon l
$$

trong đó $l$ ký hiệu độ dài của $I$; vì theo giả thiết $g_\alpha(a)$ tiến tới một giới hạn đối với $\mathfrak{F}$, nên từ tiêu chuẩn Cauchy suy ra rằng các $g_\alpha$ hội tụ đều trên $I$. Còn phải chứng minh rằng giới hạn $g$ của các $g_\alpha$ là một nguyên thủy của $f$.

Với mỗi số nguyên $n > 0$ lấy $\alpha_n$ là một chỉ số sao cho $\|f(x) - f_{\alpha_n}(x)\| \leq 1/n$ trên $I$; hiển nhiên dãy $(f_{\alpha_n})$ hội tụ đều đến $f$ và dãy $(g_{\alpha_n})$ hội tụ đều đến $g$ trên $I$. Gọi $H_n$ là tập con đếm được của $I$ tại đó $f_{\alpha_n}$ không phải là đạo hàm của $g_{\alpha_n}$, và gọi $H$ là hợp của các $H_n$, do đó cũng là một tập con đếm được của I; ta sẽ thấy rằng tại mọi điểm $x \in I$ không thuộc H thì hàm g có đạo hàm bằng $f(x)$. Thật vậy, như trên, ta thấy rằng với mọi $m \geq n$ và mọi $y \in I$ ta có

$$
\| g_{\alpha_m}(y) - g_{\alpha_m}(x) - (g_{\alpha_n}(y) - g_{\alpha_n}(x)) \| \leq \frac{2}{n} |y - x|.
$$

Cho $m$ tăng vô hạn, ta cũng có

$$
\| g(y) - g(x) - (g_{\alpha_n}(y) - g_{\alpha_n}(x)) \| \leq \frac{2}{n} |y - x|
$$

với mọi $y \in I$; bây giờ tồn tại một $h > 0$ sao cho, với $|y - x| \leq h$ và $y \in I$, ta có $\| g_\alpha(y) - g_{\alpha_n}(x) - f_{\alpha_n}(x)(y - x) \| \leq |y - x| / n$; mặt khác, ta có $\| f(x) - f_{\alpha_n}(x) \| \leq 1 / n$, nên cuối cùng thu được

$$
\| g(y) - g(x) - f(x)(y - x) \| \leq \frac{4}{n} |y - x|
$$

với $y \in I$ và $|y - x| \leq h$, điều này hoàn tất chứng minh.

#### Hệ quả 1 {#fvr-ii-s1-thm-1-cor-1 .statement}

*Tập hợp $\mathcal{H}$ các ánh xạ từ I vào E thừa nhận một nguyên thủy trên khoảng I là một không gian con vectơ đóng (và do đó đầy đủ) của không gian vectơ đầy đủ $\mathcal{F}_c(I; E)$ gồm các ánh xạ từ I vào E, được trang bị tôpô hội tụ đều trên mọi tập con compắc của I* (*Gen. Top.*, X, p. 277).

#### Hệ quả 2 {#fvr-ii-s1-thm-1-cor-2 .statement}

*Cho $x_0$ là một điểm của I, và với mỗi hàm $f \in \mathcal{H}$ gọi $P(f)$ là nguyên thủy của $f$ triệt tiêu tại điểm $x_0$; ánh xạ $f \mapsto P(f)$ từ $\mathcal{H}$ vào $\mathcal{F}_c(I; E)$ là một ánh xạ tuyến tính liên tục.*

Hệ quả 1 của Định lý 1 cho phép ta thiết lập sự tồn tại của các nguyên thủy đối với một số loại hàm bằng quy trình sau: nếu biết rằng các hàm thuộc một tập con $\mathcal{A}$ của $\mathcal{F}_c(I; E)$ nhận một nguyên thủy, thì các hàm thuộc *bao đóng* trong $\mathcal{F}_c(I; E)$ của không gian con vectơ sinh bởi $\mathcal{A}$ cũng sẽ nhận một nguyên thủy. Ta sẽ áp dụng phương pháp này trong tiểu mục tiếp theo.

### 3. CÁC HÀM ĐIỀU CHỈNH

#### Định nghĩa 2 {#fvr-ii-s1-def-2 .statement}

*Một ánh xạ $f$ của một khoảng $I \subset \mathbf{R}$ vào một tập hợp E được gọi là một hàm bậc thang nếu có một phân hoạch của I thành một số hữu hạn các khoảng $J_k$ sao cho $f$ là hằng trên mỗi $J_k$.*

Cho $(a_i)_{0 \leq i \leq n}$ là dãy tăng ngặt được tạo thành bởi các đầu mút phân biệt của các $J_k$; vì các $J_k$ rời nhau từng đôi một nên mỗi khoảng đó hoặc thu về một điểm đơn $a_i$ hoặc là một khoảng có hai điểm liên tiếp $a_i, a_{i+1}$ làm đầu mút; hơn nữa, vì I là hợp của các $J_k$, điểm $a_0$ là đầu mút trái, và $a_n$ là đầu mút phải của I. Do đó, mọi hàm bậc thang trên I có thể được đặc trưng như là một hàm hằng trên mỗi khoảng mở ]$a_i,\ a_{i+1}[\ (0 \leq i \leq n - 1)$, trong đó $(a_i)_{0 \leq i \leq n}$ là một dãy tăng ngặt các điểm của $I$ với $a_0$ là đầu mút trái và $a_n$ là đầu mút phải của $I$.

#### Mệnh đề 2 {#fvr-ii-s1-prop-2 .statement}

*Tập hợp các hàm bậc thang được xác định trên $I$, với các giá trị trong một không gian vectơ $E$ trên $\mathbf{R}$, là một không gian con vectơ $\mathcal{E}$ của không gian vectơ $\mathcal{F}(I; E)$ gồm tất cả các ánh xạ của $I$ vào $E$.*

Thật vậy, cho $f$ và $g$ là hai hàm bậc thang, và $(A_i)$ và $(B_j)$ là hai phân hoạch của $I$ thành một số hữu hạn các khoảng sao cho $f$ (tương ứng $g$) là hằng trên mỗi $A_i$ (tương ứng $B_j$); với mọi số thực $\lambda, \mu$, hiển nhiên rằng $\lambda f + \mu g$ là hằng trên mỗi khoảng khác rỗng $A_i \cap B_j$, và các khoảng này tạo thành một phân hoạch của $I$.

#### Hệ quả {#fvr-ii-s1-n3-cor-1 .statement}

*Không gian con vectơ $\mathcal{E}$ được sinh bởi các hàm đặc trưng của các khoảng.*

Bây giờ ta xét trường hợp $E$ là một không gian định chuẩn trên $\mathbf{R}$; khi đó ngay lập tức thấy rằng hàm đặc trưng của một khoảng $J$ có các đầu mút $a, b$ ($a < b$) nhận một nguyên thủy, cụ thể là hàm bằng $a$ với $x \leq a$, bằng $x$ với $a \leq x \leq b$, và bằng $b$ với $x \geq b$. Hệ quả của mệnh đề 2 do đó cho thấy rằng *mọi hàm bậc thang với các giá trị trong $E$ đều nhận một nguyên thủy*.

Bây giờ ta có thể áp dụng phương pháp được nêu trong số 2.

#### Định nghĩa 3 {#fvr-ii-s1-def-3 .statement}

*Một hàm vectơ, được xác định trên một khoảng $I$, với các giá trị trong một không gian định chuẩn đầy đủ $E$ trên $\mathbf{R}$, được gọi là một hàm điều chỉnh, nếu nó là giới hạn đều của các hàm bậc thang trên mọi tập con compact của $I$.*

Nói cách khác, các hàm điều hòa là các phần tử của bao đóng trong $\mathcal{F}_c(I; E)$ của không gian con $\mathcal{E}$ gồm các hàm bậc thang; $\overline{\mathcal{E}}$ là một không gian vectơ con của $\mathcal{F}_c(I; E)$ và vì $\mathcal{F}_c(I; E)$ đầy đủ nên $\overline{\mathcal{E}}$ cũng đầy đủ; nói cách khác, nếu một hàm là giới hạn đều của các hàm điều hòa trên mọi tập con compact của $I$, thì nó điều hòa trên $I$. Để $f$ điều hòa trên một khoảng $I$ thì điều kiện cần và đủ là hạn chế của nó trên mọi khoảng compact được chứa trong $I$ phải điều hòa.

Hệ quả I của II, p. 53 cho thấy:

#### Định lý 2 {#fvr-ii-s1-thm-2 .statement}

*Mọi hàm điều hòa trên một khoảng $I$ đều có một nguyên hàm trên $I$.*

Ta sẽ biến đổi định nghĩa 3 của II, p. 4 thành một định nghĩa tương đương khác:

#### Định lý 3 {#fvr-ii-s1-thm-3 .statement}

*Một hàm vectơ $f$ xác định trên một khoảng $I$, nhận giá trị trong một không gian định chuẩn đầy đủ $E$ trên $\mathbf{R}$, là điều hòa khi và chỉ khi nó có một giới hạn phải và một giới hạn trái tại mọi điểm trong của $I$, và một giới hạn phải tại đầu mút trái của $I$ và một giới hạn trái tại đầu mút phải của $I$, khi các điểm này thuộc $I$. Tập hợp các điểm gián đoạn của $f$ trong $I$ do đó là đếm được.*

Vì mọi khoảng là hợp đếm được của các khoảng compact, nên chỉ cần chứng minh định lý 3 khi $I$ compact, chẳng hạn $I = [a, b]$.

1 Điều kiện là cần. Giả sử $f$ điều hòa và $x$ là một điểm của $I$ khác $b$. Theo giả thiết, với mọi $\varepsilon > 0$ tồn tại một hàm bậc thang $g$ sao cho $\|f(z) - g(z)\| \leq \varepsilon$ với mọi $z \in I$; vì $g$ có giới hạn phải tại điểm $x$ nên tồn tại một $y$ sao cho $x < y \leq b$ và sao cho, với mọi cặp điểm $z, z'$ trong khoảng $]x, y]$, ta có $\|g(z) - g(z')\| \leq \varepsilon$, và do đó $\|f(z) - f(z')\| \leq 3\varepsilon$; điều này chứng minh (theo tiêu chuẩn Cauchy) rằng $f$ có giới hạn phải tại điểm $x$. Tương tự, ta chứng minh rằng $f$ có giới hạn trái tại mọi điểm của $I$ khác $a$.

2° Điều kiện là đủ. Giả sử điều kiện đó được thỏa mãn; với mỗi $x \in I$ tồn tại một khoảng mở $V_x = ]c_x, d_x[$ chứa $x$ và sao cho trên giao của $I$ với mỗi khoảng mở $]c_x, x[$, $]x, d_x[$ (khi giao không rỗng), dao động của $f$ $\leq \varepsilon$. Vì $I$ compact nên tồn tại hữu hạn điểm $x_i$ trong $I$ sao cho các $V_{x_i}$ tạo thành một phủ của $I$; gọi $(a_k)_{0 \leq k \leq n}$ là dãy thu được bằng cách sắp xếp theo thứ tự tăng các điểm của tập hữu hạn gồm các điểm $a, b$ và những điểm $x_i$, $c_{x_i}$ và $d_{x_i}$ thuộc $I$; mỗi khoảng $]a_k, a_{k+1}[$ $(0 \leq k \leq n - 1)$ được chứa trong một khoảng $]c_{x_i}, x_i[$ hoặc $]x_i, d_{x_i}[$, nên dao động của $f$ trên đó $\leq \varepsilon$; gọi $c_k$ là một trong các giá trị của $f$ trên $]a_k, a_{k+1}[$; đặt $g(a_k) = f(a_k)$ với $0 \leq k \leq n$, và $g(x) = c_k$ với mọi $x \in ]a_k, a_{k+1}[$ $(0 \leq k \leq n - 1)$, ta định nghĩa được một hàm bậc thang $g$ sao cho $\|f(z) - g(z)\| \leq \varepsilon$ trên $I$; vậy $f$ điều hòa trên $I$.

Cuối cùng, ta hãy chứng minh rằng nếu $f$ điều hòa trên $I$ thì tập hợp các điểm gián đoạn của nó là đếm được. Với mọi $n > 0$ tồn tại một hàm bậc thang $g_n$ sao cho $\|f(x) - g_n(x)\| \leq 1/n$ trên $I$; vì dãy $(g_n)$ hội tụ đều đến $f$ trên $I$, ta thấy rằng $f$ liên tục tại mọi điểm mà tất cả các $g_n$ đều liên tục (Gen. Top., X, p. 281, hệ quả 1); nhưng vì $g_n$ liên tục trừ tại các điểm của một tập hữu hạn $H_n$, suy ra $f$ liên tục tại các điểm thuộc phần bù của tập $H = \bigcup_{n} H_n$, tập này là đếm được.

#### Hệ quả 1 {#fvr-ii-s1-thm-3-cor-1 .statement}

Cho $f$ là một hàm điều hòa trên $I$; tại mọi điểm của $I$, ngoại trừ đầu mút phải (tương ứng, đầu mút trái) của $I$, mọi nguyên hàm của $f$ đều có đạo hàm phải bằng $f(x+)$ (tương ứng, đạo hàm trái bằng $f(x-)$); đặc biệt, tại mọi điểm $x$ mà $f$ liên tục, $f(x)$ là đạo hàm của một trong các nguyên hàm của nó.

Đây là một hệ quả ngay lập tức của định lý 3 của II, p. 54 và mệnh đề 6 của I, p. 18.

#### Hệ quả 2 {#fvr-ii-s1-thm-3-cor-2 .statement}

Cho $f_i$ $(1 \leq i \leq n)$ là $n$ hàm điều hòa trên một khoảng $I$, mỗi $f_i$ nhận các giá trị trong một không gian định chuẩn đầy đủ $E_i$ trên $\mathbf{R}$ $(1 \leq i \leq n)$. Nếu $g$ là một ánh xạ liên tục từ không gian con $\prod_{i=1}^{n} \overline{f_i(I)}$ của $\prod_{i=1}^{n} E_i$ vào một không gian định chuẩn đầy đủ $F$ trên $\mathbf{R}$, thì hàm hợp thành $x \mapsto g(f_1(x), f_2(x), \ldots, f_n(x))$ là điều hòa trên $I$.

Thật vậy, rõ ràng nó thỏa mãn các điều kiện của định lý 3 của II, p. 54.

Do đó ta thấy rằng nếu $f$ là một hàm vectơ điều hòa trên $I$, thì hàm thực $x \mapsto \|f(x)\|$ cũng điều hòa. Hơn nữa, các hàm thực điều hòa trên $I$ lập thành một vành;

hơn nữa, nếu $f$ và $g$ là hai hàm thực điều hòa, thì $\sup(f, g)$ và $\inf(f, g)$ là điều hòa.

#### Nhận xét 1 {#fvr-ii-s1-n3-rem-1 .statement}

Nếu $f$ là một hàm thực điều hòa trên $I$, và $g$ là một hàm vectơ điều hòa trên một khoảng chứa $f(I)$, thì hàm hợp thành $g \circ f$ không nhất thiết điều hòa ($cf.$ II, p. 79, bài tập 4).

Hai trường hợp riêng của định lý 3 của II, p. 54 đặc biệt quan trọng:

#### Mệnh đề 3 {#fvr-ii-s1-prop-3 .statement}

*Mọi hàm vectơ liên tục trên một khoảng $I \subset \mathbf{R}$ nhận các giá trị trong một không gian định chuẩn đầy đủ $E$ trên $\mathbf{R}$ đều điều hòa, và có một nguyên hàm trên $I$, mà tại mọi điểm nó là đạo hàm.*

#### Nhận xét 2 {#fvr-ii-s1-n3-rem-2 .statement}

Để chứng minh rằng một hàm liên tục có một nguyên hàm, ta có thể sử dụng sự kiện rằng mọi *hàm đa thức* của một biến thực (với các hệ số trong $E$) đều có một nguyên hàm; vì theo định lý Weierstrass (*Gen. Top.*, X, p. 313, prop. 3), mọi hàm liên tục đều là giới hạn đều của các đa thức trên mọi khoảng compáct, nên định lý 1 của II, p. 52 cho thấy rằng mọi hàm liên tục đều có một nguyên hàm.

#### Nhận xét 3 {#fvr-ii-s1-n3-rem-3 .statement}

Nguyên lý của nhận xét trước mở rộng được, không cần sửa đổi đáng kể, cho các hàm vectơ của một biến *phức* nhận giá trị trong một không gian định chuẩn đầy đủ trên $\mathbf{C}$. Nếu $U$ là một tập hợp mở trong $\mathbf{C}$, đồng phôi với $\mathbf{C}$, thì theo định nghĩa, một *nguyên hàm* của một hàm vectơ như vậy $f$ xác định trên $U$ là một hàm liên tục trên $U$, có đạo hàm bằng $f$ tại mọi điểm của $U$. Với định nghĩa này, định lý 1 của II, p. 52 mở rộng được mà không cần sửa đổi (người ta chứng minh, bằng cách sử dụng tính liên thông của $U$, rằng $(g_\alpha)$ hội tụ đều đối với $\mathcal{F}$ trên một lân cận của mỗi điểm của $U$, từ đó suy ra rằng $(g_\alpha)$ hội tụ đều đối với $\mathcal{F}$ trên mọi tập con compáct của $U$; chứng minh được hoàn tất bằng cách dùng mệnh đề 4 của I, p. 18). Do đó, mọi hàm là *giới hạn đều của các đa thức* trên mọi tập con compáct của $U$ đều có một nguyên hàm trên $U$; các hàm này không gì khác hơn là các hàm được gọi là *chỉnh hình* trên $U$, mà chúng ta sẽ nghiên cứu chi tiết hơn trong một Quyển sau.

#### Mệnh đề 4 {#fvr-ii-s1-prop-4 .statement}

*Mọi hàm thực đơn điệu $f$ trên một khoảng $I \subset \mathbf{R}$ đều là điều hòa được, và mọi nguyên hàm của $f$ đều lồi trên $I$.*

Thật vậy, $f$ thỏa mãn tiêu chuẩn của định lý 3 của *Gen. Top.*, IV, p. 350, prop. 4; phần thứ hai của mệnh đề suy ra từ hệ quả 1, từ II, p. 55, và từ mệnh đề 5 của I, p. 27.

#### Nhận xét 4 {#fvr-ii-s1-n3-rem-4 .statement}

Không nên nghĩ rằng các hàm điều hòa được trên một khoảng $I$ là những hàm duy nhất có một nguyên hàm trên $I$ ($cf.$ II, p. 80, bài tập 7 và 8).

### 4. TÍCH PHÂN

Chúng ta đã thu được (II, p. 54, định lý 2) một nguyên hàm của một hàm điều hòa được trên một khoảng $I$ như giới hạn đều của các nguyên hàm của các hàm bậc thang. Quy trình này có thể được diễn đạt theo một cách hơi khác: cho $x_0, x$ là hai điểm tùy ý của $I$ sao cho $x_0 < x$; ta gọi một *phân hoạch* của khoảng $[x_0, x]$ là bất kỳ dãy nào các khoảng $[x_i, x_{i+1}]$ có hợp bằng $[x_0, x]$, trong đó $(x_i)_{0 \leq i \leq n}$ là một dãy tăng ngặt các điểm của $[x_0, x]$ sao cho $x_n = x$. Ta sẽ gọi một *tổng Riemann*, tương ứng với một hàm vectơ $f$ xác định trên I và với phân hoạch tạo bởi các $[x_i,\ x_{i+1}]$, là mọi biểu thức có dạng
$$
\sum_{i=0}^{n-1} f(t_i)(x_{i+1} - x_i)
$$
trong đó các $t_i$ thuộc $[x_i,\ x_{i+1}]$ với $0 \leq i \leq n-1$. Khi đó ta có mệnh đề sau:

#### Mệnh đề 5 {#fvr-ii-s1-prop-5 .statement}

*Cho $f$ là một hàm điều hòa được trên một khoảng I, $g$ là một nguyên hàm của $f$ trên I, và $[x_0,\ x]$ là một khoảng compáct được chứa trong I. Với mọi $\varepsilon > 0$ tồn tại một số $\rho > 0$ sao cho đối với mọi phân hoạch của $[x_0,\ x]$ thành các khoảng có độ dài $\leq \rho$ ta có*
$$
\left| g(x) - g(x_0) - \sum_{i=0}^{n-1} f(t_i)(x_{i+1} - x_i) \right| \leq \varepsilon
$$
*(1)*
*đối với mọi tổng Riemann tương ứng với phân hoạch này.*

Thật vậy, cho $f_1$ là một hàm bậc thang sao cho $\|f(y) - f_1(y)\| \leq \varepsilon$ với mọi $y \in [x_0,\ x]$; ta có, ký hiệu một nguyên hàm của $f_1$ trên I là $g_1$,
$$
\|g(x) - g(x_0) - (g_1(x) - g_1(x_0))\| \leq \varepsilon(x - x_0)
$$
theo định lý giá trị trung bình, và mặt khác
$$
\left| \sum_{i=0}^{n-1} f(t_i)(x_{i+1} - x_i) - \sum_{i=0}^{n-1} f_1(t_i)(x_{i+1} - x_i) \right| \leq \varepsilon(x - x_0).
$$

Do đó chỉ cần chứng minh mệnh đề khi $f$ là một *hàm bậc thang*. Cho $(y_k)_{1 \leq k \leq m}$ là dãy hữu hạn tăng ngặt các điểm gián đoạn của $f$ trong $[x_0,\ x]$. Với mọi phân hoạch của $[x_0,\ x]$ thành các khoảng có độ dài $\leq \rho$, mỗi điểm $y_k$ thuộc nhiều nhất hai trong các khoảng này; do đó có không quá $2m$ khoảng trên đó $f$ không hằng; nhưng, trên một khoảng như thế $[x_i,\ x_{i+1}]$ ta có
$$
\|g(x_{i+1}) - g(x_i) - f(t_i)(x_{i+1} - x_i)\| \leq 2M (x_{i+1} - x_i)
$$
khi ký hiệu $M$ là cận trên nhỏ nhất của $\|f\|$ trên $[x_0,\ x]$; mặt khác, khi $f$ hằng trên $[x_i,\ x_{i+1}]$ thì ta có
$$
g(x_{i+1}) - g(x_i) - f(t_i)(x_{i+1} - x_i) = 0.
$$
Vì vậy thấy rằng hiệu
$$
\left| g(x) - g(x_0) - \sum_{i=0}^{n-1} f(t_i)(x_{i+1} - x_i) \right|
$$
không thể vượt quá $4Mm\rho$; do đó chỉ cần lấy $\rho \leq \varepsilon / 4Mm$ để thu được (1).

#### Nhận xét 1 {#fvr-ii-s1-n4-rem-1 .statement}

Khi $f$ là *liên tục* thì mệnh đề 5 có thể được chứng minh đơn giản hơn: vì $f$ liên tục đều trên $[x_0,\ x]$ nên tồn tại một $\rho > 0$ sao cho trên mọi khoảng có độ dài $\leq \rho$ được chứa trong $[x_0,\ x]$ độ dao động của $f$ là $\leq \frac{\varepsilon}{x - x_0}$; với mọi phân hoạch của $[x_0,\ x]$ thành các khoảng $[x_i,\ x_{i+1}]$ có độ dài $\leq \rho$ và mọi lựa chọn $t_i$ trong $[x_i,\ x_{i+1}]$ với $0 \leq i \leq n-1$, hàm bậc thang $f_1$ bằng $f(t_i)$ trên $[x_i,\ x_{i+1}]$ ($0 \leq i \leq n-1$), và bằng $f(x)$ tại điểm x, thỏa mãn $\| f(y) - f_1(y) \| \leq \frac{\varepsilon}{x - x_0}$ trên $[x_0, x]$; nếu $g_1$ là một nguyên hàm của $f_1$ thì ta có
$$
g_1(x) - g_1(x_0) = \sum_{i=0}^{n-1} f(t_i)(x_{i+1} - x_i),
$$
nên hệ thức (1) suy ra ngay từ định lý giá trị trung bình.

Trong phần còn lại của chương này, ta sẽ chỉ xét các nguyên hàm của các hàm *điều hòa* trên một khoảng I. Với một hàm như thế $f$, nhận giá trị trong E, một nguyên hàm $g$ của $f$, và với hai điểm tùy ý $x_0, x$ của I, phần tử $g(x) - g(x_0)$ của E (rõ ràng là như nhau, bất kể xét nguyên hàm $g$ nào của $f$) được gọi là *tích phân của hàm* $f$ *từ* $x_0$ *đến* $x$ (hay *trên khoảng đóng* $[x_0, x]$) và được ký hiệu bởi $\int_{x_0}^x f(t) dt$ hoặc $\int_{x_0}^x f$. Tên gọi và ký hiệu này có nguồn gốc từ mệnh đề 5 của II, p. 57, cho thấy rằng một tích phân có thể được xấp xỉ tùy ý gần bởi một tổng Riemann; cụ thể hơn, ta có thể viết, lấy các phân hoạch của $[x_0, x]$ thành các khoảng bằng nhau,

$$
\frac{1}{x - x_0} \int_{x_0}^x f(t) dt = \lim_{n \to \infty} \frac{1}{n} \sum_{k=0}^{n-1} f \left( x_0 + k \frac{x - x_0}{n} \right).
$$

Nói cách khác, phần tử $\frac{1}{x - x_0} \int_{x_0}^x f(t) dt$ là giới hạn của các *trung bình cộng* của các giá trị của $f$ tại các đầu mút bên trái của các khoảng trong một phép chia của $[x_0, x]$ thành các khoảng bằng nhau; người ta cũng gọi nó là *giá trị trung bình* (hoặc *trung bình*) của hàm $f$ trên khoảng $[x_0, x]$.

Theo định nghĩa, hàm $x \mapsto \int_{x_0}^x f(t) dt$ chẳng gì khác hơn là nguyên hàm của $f$ triệt tiêu tại điểm $x_0 \in I$; người ta cũng ký hiệu nó bởi $\int_{x_0}^x f(t) dt$ hay $\int_{x_0}^x f$.

#### Nhận xét 2 {#fvr-ii-s1-n4-rem-2 .statement}

Với một hàm tùy ý $h$ được định nghĩa trên I, nhận giá trị trong E, phần tử $h(x) - h(x_0)$ cũng được viết là $h(t)\Big|_{x_0}^x$; với ký hiệu này ta thấy rằng nếu $g$ là bất kỳ nguyên hàm nào của một hàm điều hòa $f$ trên I, thì ta có

$$
\int_{x_0}^x f(t) dt = g(t)\Big|_{x_0}^x.
$$

#### Nhận xét 3 {#fvr-ii-s1-n4-rem-3 .statement}

Các biểu thức $\int_{x_0}^x f(t) dt$ và $g(t)\Big|_{x_0}^x$ là những ký hiệu viết tắt biểu diễn các dãy ký hiệu trong đó các chữ $x, x_0, f, g$, nhưng *không phải* chữ $t$, xuất hiện (*xem Lý thuyết Tập hợp*, I, p. 15); người ta nói rằng trong số các ký hiệu này $t$ là một "*biến giả*": vì thế có thể thay $t$ bằng bất kỳ biến nào khác phân biệt với $x, x_0, f$ và $g$ (và với các biến có thể có đi vào chứng minh nơi các ký hiệu này xuất hiện) mà không làm thay đổi ý nghĩa của ký hiệu thu được (người đọc có thể so sánh các ký hiệu này với những ký hiệu như $\sum_{i=1}^n x_i$, hay $\bigcup X_i$, trong đó $i$ cũng là một biến giả).

#### Nhận xét 4 {#fvr-ii-s1-n4-rem-4 .statement}

Việc xấp xỉ một tích phân bằng các tổng Riemann có liên hệ chặt chẽ với một trong những nguồn gốc lịch sử của khái niệm tích phân, bài toán *đo* diện tích. Chúng ta sẽ trở lại điểm này trong Sách về Tích phân vốn dành cho các phép tổng quát hóa của khái niệm tích phân mà bài toán này dẫn tới; trong những phép tổng quát hóa ấy, các hàm "*được tích phân*" không nhất thiết được định nghĩa trên một tập con của $\mathbf{R}$; hơn nữa, ngay cả khi xét đến các hàm thực $f$ của một biến thực mà ta có thể định nghĩa một tích phân $\int_{x_0}^x f(t)\,dt$, thì hàm $x \mapsto \int_{x_0}^x f(t)\,dt$ không phải lúc nào cũng là một nguyên hàm của $f$, và tồn tại những hàm có nguyên hàm nhưng lại không "khả tích" theo nghĩa mà chúng tôi ám chỉ.

### 5. CÁC TÍNH CHẤT CỦA TÍCH PHÂN

Các tính chất của tích phân của các hàm điều hòa chỉ đơn thuần là bản dịch, theo ký hiệu thích hợp, của các tính chất của đạo hàm đã được chứng minh ở chương I.

Trước hết, công thức (3) cho thấy rằng bất kể các điểm $x,\ y,\ z$ của I là gì, ta có

$$
\int_x^x f(t)\,dt = 0 \tag{4}
$$

$$
\int_x^y f(t)\,dt + \int_y^x f(t)\,dt = 0 \tag{5}
$$

$$
\int_x^y f(t)\,dt + \int_y^z f(t)\,dt + \int_z^x f(t)\,dt = 0 \tag{6}
$$

Từ mệnh đề 1 của II, p. 52, ta có

$$
\int_{x_0}^x (f + g) = \int_{x_0}^x f + \int_{x_0}^x g \tag{7}
$$

và với mọi vô hướng $k$

$$
\int_{x_0}^x k f = k \int_{x_0}^x f. \tag{8}
$$

Cho E, F là hai không gian định chuẩn đầy đủ trên $\mathbf{R}$, và u là một ánh xạ tuyến tính liên tục từ E vào F. Nếu f là một hàm điều hòa trên I nhận giá trị trong E, thì $u \circ f$ là một hàm điều hòa trên I nhận giá trị trong F (II, p. 6, hệ quả 2), và với $a, b \in I$ (I, p. 13, mệnh đề 2) ta có

$$
\int_a^b u(f(t))\,dt = u \left( \int_a^b f(t)\,dt \right). \tag{9}
$$

Bây giờ cho E, F, G là ba không gian định chuẩn đầy đủ trên $\mathbf{R}$, và $(x, y) \mapsto |x.y|$ là một ánh xạ song tuyến tính liên tục của $E \times F$ vào G. Cho f và g là hai hàm vectơ được định nghĩa và liên tục trên I, nhận giá trị tương ứng trong E và F; hơn nữa giả sử f và g là hai nguyên hàm của các hàm *điều hòa*, mà chúng tôi lạm dụng ngôn ngữ mà ký hiệu là $f'$ và $g'$ (thực ra các hàm này không hề được bảo đảm bằng các đạo hàm của f và g tương ứng, trừ trên phần bù của một tập đếm được). Theo mệnh đề 3 của I, p. 6, hàm $h(x) = [f(x).g(x)]$ có, tại mỗi điểm thuộc phần bù của một tập con đếm được của I, một đạo hàm bằng $[f(x).g'(x)] + [f'(x).g(x)]$. Nay, nhờ tính liên tục của $[x.y]$ và hệ quả 2 của II, p. 55, mỗi hàm $[f.g']$ và $[f'.g]$ là một hàm điều hòa trên I; do đó ta có công thức

$$
\int_a^b [f'(t).g(t)]\,dt = [f(t).g(t)]\Big|_a^b - \int_a^b |f(t).g'(t)|\,dt \tag{10}
$$

được gọi là *công thức tích phân từng phần*, cho phép ta tính nhiều nguyên hàm.

Chẳng hạn, công thức tích phân từng phần cho ta công thức sau

$$
\int_{x_0}^{x} t f'(t) \, dt = t f(t) \Big|_{x_0}^{x} - \int_{x_0}^{x} f(t) \, dt
$$

như vậy quy việc tính nguyên hàm của một trong hai hàm $f(x)$ và $x f'(x)$ về hàm kia.

Tương tự, nếu $f$ và $g$ là khả vi $n$ lần trên một khoảng $I$, và nếu $f^{(n)}$ và $g^{(n)}$ là các hàm điều hòa trên $I$, thì công thức (5) của I, p. 21 tương đương với công thức sau:

$$
\int_a^b [f^{(n)}(t) \cdot g(t)] \, dt
$$
$$
= \left( \sum_{p=0}^{n-1} (-1)^p [f^{(n-p-1)}(t) \cdot g^{(p)}(t)] \right) \Bigg|_a^b + (-1)^n \int_a^b [f(t) \cdot g^{(n)}(t)] \, dt
$$
(11)

công thức này được gọi là *công thức tích phân từng phần cấp n*.

Giờ đây ta hãy dịch công thức lấy đạo hàm của hàm hợp (I, p. 9, Mệnh đề 5). Cho $f$ là một hàm thực được xác định và liên tục trên $I$, là nguyên hàm của một hàm *điều hòa* trên $I$ (mà ta lại viết là $f'$ theo lối nói quen dùng); hơn nữa, cho $g$ là một hàm vectơ *liên tục* (với giá trị trong một không gian định chuẩn đầy đủ) trên một khoảng mở $J$ chứa $f(I)$; nếu $h$ ký hiệu một nguyên hàm tùy ý của $g$ trên $J$, thì $h$ có một đạo hàm bằng $g$ tại mỗi điểm của $J$ (II, p. 56, Mệnh đề 3); do đó hàm hợp $h \circ f$ có một đạo hàm bằng $g(f(x)) f'(x)$ tại mọi điểm thuộc phần bù (so với $I$) của một tập con đếm được của $I$ (I, p. 9, Mệnh đề 5); vì hàm $g(f(x)) f'(x)$ là điều hòa (II, p. 55, Hệ quả 2), ta có thể viết công thức

$$
\int_a^b g(f(t)) f'(t) \, dt = \int_{f(a)}^{f(b)} g(u) \, du
$$
(12)

được gọi là *công thức đổi biến số*, công thức này cũng giúp việc tính nguyên hàm dễ dàng hơn.

Chẳng hạn, nếu lấy $f(x) = x^2$, ta thấy rằng công thức (12) quy việc tính nguyên hàm của các hàm $g(x)$ và $x g(x^2)$ về một công thức cho cái này và cái kia.

Để dịch định lý giá trị trung bình (I, p. 14, Định lý 1) đối với các nguyên hàm của các hàm thực điều hòa, trước hết ta nhận xét rằng một hàm thực điều hòa $f$ trên một khoảng đóng $I$ là bị chặn trên $I$; gọi $J$ là tập các điểm của $I$ tại đó $f$ là *liên tục*, và đặt $m = \inf_{x \in J} f(x)$, $M = \sup_{x \in J} f(x)$; ta biết (II, p. 54, Định lý 3) rằng $I \cap \mathbf{C}J$ là đếm được; hơn nữa, nếu $B$ là phần bù, trong $I$, của một tập con đếm được bất kỳ của $I$, và $m' = \inf_{x \in B} f(x)$, $M' = \sup_{x \in B} f(x)$, thì $m' \leq m \leq M \leq M'$: thật vậy, với mỗi điểm $x \in J$, có những điểm $y$ của B gần $x$ tùy ý, do đó $m' \leq f(y) \leq M'$; vì $f$ liên tục tại điểm $x$ nên khi cho $y$ tiến tới $x$ ($y$ vẫn thuộc B) ta thấy rằng $m' \leq f(x) \leq M'$, điều đó chứng minh mệnh đề trên. Vì thế, khi dịch định lý giá trị trung bình ta được mệnh đề sau:

#### Mệnh đề 6 (định lý giá trị trung bình) {#fvr-ii-s1-prop-6 .statement}

*Cho $f$ là một hàm chỉnh thực trên một khoảng compact $l = [a, b]$; nếu $J$ là tập các điểm của I tại đó $f$ liên tục, và $m = \inf_{x \in J} f(x)$, $M = \sup_{x \in J} f(x)$, thì*

$$
m < \frac{1}{b-a} \int_a^b f(t)\,dt < M
$$

*(13)*

*trừ khi $f$ là hằng trên J, trong trường hợp đó ba vế của (13) bằng nhau.*

Nói cách khác, *giá trị trung bình* của hàm chỉnh $f$ trong I nằm giữa các cận của $f$ trên tập con của I mà ở đó $f$ liên tục.

#### Hệ quả 1 {#fvr-ii-s1-prop-6-cor-1 .statement}

*Nếu một hàm chỉnh thực $f$ trên I sao cho $f(x) \geq 0$ tại các điểm mà $f$ liên tục, thì* $\frac{1}{b-a} \int_a^b f(t)\,dt > 0$ *trừ khi* $f(x) = 0$ *tại các điểm mà* $f$ *liên tục.*

#### Hệ quả 2 {#fvr-ii-s1-prop-6-cor-2 .statement}

*Cho $f$ và $g$ là hai hàm chỉnh thực trên I, sao cho $g(x) \geq 0$ *tại các điểm mà* $g$ *liên tục; nếu* $m$ *và* $M$ *là cận dưới lớn nhất và cận trên bé nhất của* $f$ *trên tập các điểm mà* $f$ *liên tục, thì*

$$
\frac{m}{b-a} \int_a^b g(t)\,dt \leq \frac{1}{b-a} \int_a^b f(t)g(t)\,dt \leq \frac{M}{b-a} \int_a^b g(t)\,dt.
$$

*(14)*

*Hai hạng đầu tiên (tương ứng, hai hạng cuối) không bằng nhau trừ khi* $g(x)(f(x) - m) = 0$ *(tương ứng, $g(x)(f(x) - M) = 0$) tại mọi điểm mà* $f$ *và* $g$ *đều liên tục.*

Đối với các hàm vectơ, định lý giá trị trung bình (I, p. 15, Định lý 2) suy ra mệnh đề sau:

#### Mệnh đề 7 {#fvr-ii-s1-prop-7 .statement}

*Cho* $\mathbf{f}$ *là một hàm vectơ chỉnh trên một khoảng compact* $I = [a, b]$, *nhận giá trị trong một không gian chuẩn đầy đủ* $E$, *và cho* $g$ *là một hàm chỉnh thực trên* $I$, *sao cho* $g(x) \geq 0$ *tại các điểm mà* $g$ *liên tục; trong trường hợp đó*

$$
\left\| \int_a^b \mathbf{f}(t)g(t)\,dt \right\| \leq \int_a^b \| \mathbf{f}(t) \| g(t)\,dt.
$$

*(15)*

*Đặc biệt,*

$$
\left\| \int_a^b \mathbf{f}(t)\,dt \right\| \leq \int_a^b \| \mathbf{f}(t) \| \,dt.
$$

*(16)*

### 6. CÔNG THỨC TÍCH PHÂN CHO SỐ DƯ TRONG CÔNG THỨC TAYLOR; CÁC NGUYÊN HÀM BẬC CAO HƠN

Công thức tích phân từng phần bậc $n$ (II, p. 60, công thức (11)) cho phép biểu diễn số dư $r_n(x)$ trong khai triển Taylor bậc $n$ của một hàm có đạo hàm chỉnh $(n+1)^{th}$ trên một khoảng I (I, p. 22) dưới dạng một tích phân; thật vậy, khi thay, trong (12), $f$ bằng $f'$, $b$ bằng $x$, và $g(t)$ bằng hàm $(t-x)^n/n!$, suy ra rằng

$$
f(x) = f(a) + f'(a) \frac{(x-a)}{1!} + f''(a) \frac{(x-a)^2}{2!} + \cdots \\
+ f^{(n)}(a) \frac{(x-a)^n}{n!} + \int_a^x f^{(n+1)}(t) \frac{(x-t)^n}{n!} \, dt
$$

nói cách khác

$$
r_n(x) = \int_a^x f^{(n+1)}(t) \frac{(x-t)^n}{n!} \, dt,
$$

công thức này thường cho phép thu được các cận đơn giản cho số dư.

Cho một hàm điều hòa $f$ trên một khoảng I, một nguyên thủy tùy ý $g$ của $f$, do liên tục trên I, lại có một nguyên thủy; một nguyên thủy tùy ý của một nguyên thủy tùy ý của $f$ được gọi là một *nguyên thủy thứ hai* của $f$. Nói chung, một nguyên thủy của một nguyên thủy cấp $n-1$ của $f$ được gọi là một *nguyên thủy cấp* $n$ của $f$. Ta thấy ngay lập tức, bằng quy nạp theo $n$, rằng hiệu của hai nguyên thủy cấp $n$ của $f$ là một *đa thức có bậc không vượt quá* $n-1$ (với các hệ số trong E). Một nguyên thủy cấp $n$ của $f$ được xác định hoàn toàn nếu ta cho giá trị của nó và các giá trị của $n-1$ đạo hàm đầu tiên của nó tại một điểm $a \in I$.

Đặc biệt, $\int_a^{(n)} f$ ký hiệu nguyên thủy cấp $n$ của $f$ triệt tiêu, cùng với $n-1$ đạo hàm đầu tiên của nó, tại điểm $a$. Công thức Taylor cấp $n-1$, áp dụng cho nguyên thủy này, cho thấy rằng nếu $g = \int_a^{(n)} f$, thì

$$
g(x) = \int_a^x f(t) \frac{(x-t)^{n-1}}{(n-1)!} \, dt
$$

do đó quy việc xác định một nguyên thủy cấp $n$ về một tích phân duy nhất.

### Bài tập {#fvr-ii-s1-exercises}

Xem [các bài tập của § 1](exercises/s1/).
