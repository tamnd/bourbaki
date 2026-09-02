---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: I
chapter_title: Lie Algebras
section: 7
section_title: Ado’s Theorem
lang: vi
source: lie-i-iii
pdf_pages: 0086-0090, 0127-0128
extraction: ocr
subsections:
    - "no": 1
      title: COEFFICIENTS OF A REPRESENTATION
      page: 0
      pdf_page: 87
    - "no": 2
      title: THE EXTENSION THEOREM
      page: 0
      pdf_page: 87
    - "no": 3
      title: ADO'S THEOREM
      page: 0
      pdf_page: 89
statements: 6
exercises: 5
content_sha256: 171efc4b707890c8545675e5949c9fa0c52aa22c4aff998479bf8acf06ccda8c
translated_from: content/en/lie/I/07_s7_ado_s_theorem.md
source_content_sha256: 88c99569fd7f93541de8470999a923ed72c5b349486bddb4207865298e2f0c53
translation_model: gpt-5.4, copied
translation_run: translate-vi-eb57ee92
glossary_version: 34
glossary_terms_sha256: 04d7c9bbab54999d87f6ccab444eb129376483f64767e87526a6d057f6a7d62c
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 7. ĐỊNH LÝ ADO

*Nhắc lại rằng $K$ ký hiệu một trường có đặc số 0 và mọi đại số Lie đều được giả thiết là hữu hạn chiều trên $K$.*

### 1. CÁC HỆ SỐ CỦA MỘT BIỂU DIỄN

Cho U là một đại số kết hợp có phần tử đơn vị trên K, U* là đối ngẫu của không gian vectơ U và $\rho$ là một biểu diễn của U trên một không gian vectơ E. Với $e \in E$ và $e' \in E^*$, gọi $\theta(e, e') \in U^*$ là hệ số tương ứng của $\rho$ (Đại số, Chương VIII, § 13, no. 3). Nhắc lại rằng $\theta(e, e')(x) = \langle \rho(x)e, e' \rangle$ và rằng ánh xạ $e \mapsto \theta(e, e')$ với $e'$ cố định là một đồng cấu của U-môđun E vào U-môđun U* của biểu diễn đối chính quy của U (loc. cit., Mệnh đề 1); do đó không gian con vectơ của U* sinh bởi các hệ số của $\rho$ (một không gian con mà trong đoạn này chúng ta sẽ ký hiệu là $C(\rho)$) là một dưới-U-môđun của U*. Nếu $(e'_i)_{i \in I}$ là một họ các phần tử sinh ra E* trên K, thì ánh xạ $e \mapsto (\theta(e, e'_i))$ là một U-đồng cấu đơn ánh của E vào $C(\rho)^I$; vì $\theta(e, e'_i) = 0$ với mọi $i$ suy ra $\langle e, e'_i \rangle = \langle \rho(1)e, e'_i \rangle = \theta(e, e'_i)(1) = 0$ với mọi $i$ và do đó $e = 0$.

Đặc biệt, nếu U là đại số bao của một đại số Lie g và $\rho$ là một biểu diễn của g (đồng nhất với một biểu diễn của U) trên một không gian vectơ E chiều n, thì g-môđun E đẳng cấu với một g-môđun con của $(C(\rho))^n$.

### 2. ĐỊNH LÝ MỞ RỘNG

Cho $g = h + g'$ là một đại số Lie là tổng trực tiếp của một iđêan $g'$ và một đại số con $h$, U là đại số bao của g và $U' \subset U$ là đại số bao của $g'$. Tồn tại một và chỉ một cấu trúc môđun trên $U'$ sao cho: (α) với $x \in g'$ và $u \in U'$, $x_{U'}u = -ux$; (β) với $x \in h$ và $u \in U'$, $x_{U'}u = xu - ux$ (phần tử sau này chắc chắn thuộc $U'$ vì đạo hàm nội của U được định nghĩa bởi x giữ ổn định $g'$ và do đó giữ ổn định $U'$). Các điều kiện (α) và (β) xác định duy nhất một ánh xạ tuyến tính $x \mapsto x_{U'}$ từ g vào $\mathcal{L}_K(U')$. Do đó chỉ cần kiểm tra rằng $[x, y]_{U'} = [x_{U'}, y_{U'}]$; chỉ cần xét các trường hợp sau:

(1) $x \in g', y \in g'$: khi đó
$$
[x, y]_{U'}u = -u(xy - yx) = (x_{U'}y_{U'} - y_{U'}x_{U'})u;
$$

(2) $x \in h, y \in g'$: khi đó
$$
[x, y]_{U'}u = -u(xy - yx) = x(-uy) - (-uy)x + (xu - ux)y \\
= (x_{U'}y_{U'} - y_{U'}x_{U'})u;
$$

(3) $x \in h, y \in h$: khi đó $[x, y]_{U'}$ và $[x_{U'}, y_{U'}]$ là hai đạo hàm của $U'$ mà các hạn chế của chúng lên $g'$ trùng nhau với các hạn chế của $\mathrm{ad}_g[x, y]$ và $[\mathrm{ad}_g x, \mathrm{ad}_g y]$; do đó các đạo hàm này bằng nhau.

Ta cũng sẽ xét biểu diễn đối ngẫu $x \mapsto {}^t x_{U'}$ của g trên ${U'}^*$. Với $x \in g'$, ${}^t x_{U'}$ là chuyển vị của phép nhân phải bởi x trong $U'$; do đó biểu diễn tương ứng của $U'$ là biểu diễn đối chính quy của $U'$.

#### Định nghĩa 1 {#lie-i-s7-def-1 .statement}

Cho $g$ là một đại số Lie, $g'$ là một đại số con của $g$ và $\rho'$ là một biểu diễn của $g'$ trên $V'$. Một biểu diễn $\rho$ của $g$ trên $V$ được gọi là một mở rộng của $\rho'$ lên $g$ nếu tồn tại một đồng cấu đơn cấu của $g'$-môđun vào $g'$-môđun $V$. Ta cũng nói rằng $g$-môđun $V$ là một mở rộng của $g'$-môđun $V'$.

Nếu $\rho'$ là hữu hạn chiều và $g'$ là một iđêan giải được của $g$, thì điều kiện cần để tồn tại một mở rộng hữu hạn chiều là $[g, g']$ được chứa trong iđêan lũy linh lớn nhất của $\rho'$ (§ 5, no. 3, Định lý 1).

#### Định lý 1 (Zassenhaus) {#lie-i-s7-thm-1 .statement}

Cho $g = g' + h$ là một đại số Lie là tổng trực tiếp của một iđêan $g'$ và một đại số con $h$, và $\rho'$ là một biểu diễn hữu hạn chiều của $g'$ mà iđêan lũy linh lớn nhất của nó chứa $[h, g']$.

(a) Tồn tại một mở rộng hữu hạn chiều $\rho$ của $\rho'$ lên $g$ mà iđêan lũy linh lớn nhất của nó chứa iđêan lũy linh lớn nhất của $\rho'$.

(b) Nếu với mọi $x \in h$ thì hạn chế lên $g'$ của $\operatorname{ad}_gx$ là lũy linh, có thể chọn $\rho$ sao cho hơn nữa iđêan lũy linh lớn nhất của $\rho$ chứa $h$.

Cho $U'$ là đại số bao của $g'$. Giả sử $U'$ và ${U'}^*$ có các cấu trúc $g$-môđun được xác định ở đầu no này.

$$
\begin{array}{ll}
{U'}^* & \text{Cho } I \subset U' \text{ là hạt nhân của } \rho' \text{ (đồng nhất với một biểu diễn của } U'). \text{ Nó là một iđêan hai phía của } U' \text{ có đối chiều hữu hạn. Không gian con } C(\rho') \text{ của } {U'}^* \text{ (x. no. 1) trực giao với } I. \text{ Cho } S \text{ là môđun con-} g \text{ của } {U'}^* \text{ được sinh bởi } C(\rho'). \\
C(\rho')
\end{array}
$$

Bây giờ ta chỉ ra rằng $S$ là hữu hạn chiều trên $K$. Gọi $V'$ là không gian mà trên đó $\rho'$ tác động và $V' = V'_0 \supset V'_1 \supset \cdots \supset V'_d = \{0\}$ là một chuỗi Jordan-Hölder của $g'$-môđun $V'$. Gọi $\rho'_i$ là biểu diễn của $g'$ trên $V'_{i-1}/V'_i$ dẫn xuất từ $\rho'$ ($1 \leq i \leq d$). Gọi $I' \subset U'$ là giao của các hạt nhân của các $\rho'_i$ (được đồng nhất với các biểu diễn của $U'$). Khi đó

$$
{I'}^d \subset I \subset I'
$$

và $I' \cap g'$ là iđêan lũy linh lớn nhất của $\rho'$. Theo § 2, no. 6, Hệ quả của Mệnh đề 6, ${I'}^d$ có đối chiều hữu hạn trong $U'$. Nếu $x \in h$, đạo hàm $u \mapsto xu - ux$ của $U'$ ánh xạ $g'$ vào $[h, g'] \subset I'$, do đó ánh xạ $U'$ vào $I'$ và vì thế ánh xạ ${I'}^d$ vào ${I'}^d$. Mặt khác, rõ ràng ${I'}^d$ là một dưới-$g'$-môđun của $U'$. Vậy ${I'}^d$ là một dưới-$g$-môđun của $U'$. Phần trực giao của ${I'}^d$ trong ${U'}^*$ là một dưới-$g$-môđun hữu hạn chiều chứa $C(\rho')$ và do đó chứa $S$. Điều này chứng tỏ rằng $S$ là hữu hạn chiều trên $K$. Với $x \in I' \cap g'$, $x^d$ hiển nhiên được chứa trong linh hóa tử của $g$-môđun $U'/{I'}^d$ và do đó cũng được chứa trong linh hóa tử của $g$-môđun $S$.

Ta đã thấy ở no. 1 rằng $g'$-môđun $V'$ đẳng cấu với một môđun con-$g'$ của một tích $(C(\rho'))^n$. Do đó, $g$-môđun $S^n$ cho một mở rộng hữu hạn chiều $\rho$ của $\rho'$ lên $g$. Hơn nữa, $\rho(x)$ là lũy linh với $x \in I' \cap g'$; vì $I' \cap g'$ là một iđêan của $g$ (do nó chứa $[h, g']$ theo giả thiết), ta thấy rằng $I' \cap g'$ được chứa trong iđêan lũy linh lớn nhất của $\rho$. Vậy (a) được chứng minh.

Giả sử sau cùng rằng với mọi $x \in h$ phép hạn chế lên $g'$ của $\mathrm{ad}_{\psi}x$ là lũy linh. Vì các phần tử của $h$ tác động lên $U'$ bởi các phép dẫn xuất, nên với mọi $u \in U'$ và mọi $x \in h$ tồn tại một số nguyên $e$ sao cho $(x_{U'})^e.u = 0$; do đó các nội cấu dẫn xuất từ $x_{U'}$ trên $U'/{I'}^d$ và trên $S$ (là các không gian hữu hạn chiều) đều lũy linh. Vậy $\rho(x)$ là lũy linh với mọi $x \in h$. Ta đã thấy trước đó rằng điều này cũng đúng với $x \in I' \cap g'$. Vì $I' \cap g'$ là một iđêan của $g'$ chứa $[h, g']$, nên tổng $h + (I' \cap g')$ cũng là một iđêan của $g$. Mệnh đề (b) của Định lý 1 khi đó suy ra từ bổ đề sau:

#### Bổ đề 1 {#lie-i-s7-lem-1 .statement}

*Cho $g = g' + h$ là một đại số Lie là tổng của một iđêan $g'$ và một đại số con $h$. Cho $\sigma$ là một biểu diễn hữu hạn chiều của $g$. Giả sử rằng $\sigma(x)$ là lũy linh với mọi $x \in g'$ và mọi $x \in h$. Khi đó $\sigma(x)$ là lũy linh với mọi $x \in g$.*

Chuyển qua thương theo hạt nhân của $\sigma$, có thể giả sử $\sigma$ là trung thành. Khi đó $g'$ và $h$ là lũy linh và do đó $g$, là một mở rộng của một thương của $h$ bởi $g'$, là giải được. Khi đó $h$ và $g'$ được chứa trong iđêan lũy linh lớn nhất của $\sigma$ (§ 5, no. 3, Hệ quả 6 của Định lý 1).

Để có một cải tiến của Định lý 1, xem Bài tập 4.

### 3. ĐỊNH LÝ ADO

#### Mệnh đề 1 {#lie-i-s7-prop-1 .statement}

*Cho $g$ là một đại số Lie, $n$ là iđêan lũy linh lớn nhất của nó, $a$ là một iđêan lũy linh của $g$ và $\rho$ là một biểu diễn hữu hạn chiều của $a$ sao cho mọi phần tử của $\rho(a)$ đều lũy linh. Khi đó $\rho$ có một mở rộng hữu hạn chiều $\sigma$ lên $g$ sao cho mọi phần tử của $\sigma(n)$ đều lũy linh.*

Cho $a = n_0 \subset n_1 \subset \cdots \subset n_p = n$ là một dãy các đại số con của $n$ sao cho $n_{i-1}$ là một iđêan của $n_i$ có đối chiều 1 với $1 \leq i \leq p$ (§ 4, no. 1, Mệnh đề 1 (e)). Do đó đại số $n_i$ là tổng trực tiếp của $n_{i-1}$ và một đại số con 1-chiều. Vì $\mathrm{ad}_{n}x$ là lũy linh với mọi $x \in n$, nên có thể tìm được lần lượt các mở rộng hữu hạn chiều $\rho_1, \rho_2, \ldots, \rho_p = \rho'$ của $\rho$ lên $n_1, n_2, \ldots, n_p = n$ sao cho mọi phần tử của $\rho'(n)$ đều lũy linh.

Gọi $r$ là căn của $g$ và gọi $n = r_0 \subset r_1 \subset \cdots \subset r_q = r$ là một dãy các đại số con của $r$ sao cho $r_{i-1}$ là một iđêan của $r_i$ có đối chiều 1 với $1 \leq i \leq q$ (§ 5, no. 1, Mệnh đề 2 (d)). Do đó đại số $r_i$ là tổng trực tiếp của $r_{i-1}$ và một đại số con một chiều. Vì $[r, r] \subset n$, nên có thể (Định lý 1) tìm lần lượt các mở rộng hữu hạn chiều $\rho'_1, \rho'_2, \ldots, \rho'_q = \rho''$ của $\rho'$ lên $r_1, r_2, \ldots, r_q = r$ sao cho mọi phần tử của $\rho''(n)$ đều lũy linh.

Cuối cùng $g$ là tổng trực tiếp của $r$ và một đại số con $s$ (§ 6, no. 8, Định lý 5). Vì $[s, r] \subset n$, nên có thể (Định lý 1) tìm được một mở rộng hữu hạn chiều $\sigma$ của $\rho''$ lên $g$ sao cho mọi phần tử của $\sigma(n)$ đều lũy linh.

#### Định lý 2 {#lie-i-s7-thm-2 .statement}

*Mọi đại số Lie đều có một biểu diễn tuyến tính trung thành hữu hạn chiều.*

Chính xác hơn:

#### Định lý 3 (Ado) {#lie-i-s7-thm-3 .statement}

*Cho $g$ là một đại số Lie và $n$ là iđêan lũy linh lớn nhất của nó. Tồn tại một biểu diễn trung thành hữu hạn chiều $\varphi$ của $g$ sao cho mọi phần tử của $\varphi(n)$ đều lũy linh.*

Đại số Lie hữu hạn chiều $K$ chấp nhận các biểu diễn trung thành hữu hạn chiều $\tau$ sao cho mọi phần tử của $\tau(K)$ đều lũy linh, ví dụ biểu diễn
$$
\lambda \mapsto \begin{pmatrix} 0 & 0 \\ \lambda & 0 \end{pmatrix}.
$$

Dễ dàng suy ra rằng tâm $c$ của $g$, là một tích của các đại số 1-chiều, có một biểu diễn trung thành hữu hạn chiều $\sigma$ sao cho mọi phần tử của $\sigma(c)$ đều lũy linh. Cho $\sigma_1$ là một mở rộng hữu hạn chiều của $\sigma$ lên $g$ sao cho mọi phần tử của $\sigma_1(n)$ đều lũy linh (Mệnh đề 1); nếu $k$ ký hiệu hạt nhân của $\sigma_1$, thì $k \cap c = \{0\}$. Mặt khác, cho $\sigma_2$ là biểu diễn kề của $g$, có hạt nhân là $c$; mọi phần tử của $\sigma_2(n)$ đều lũy linh. Tổng trực tiếp $\rho$ của $\sigma_1$ và $\sigma_2$ là hữu hạn chiều; mọi phần tử của $\rho(n)$ đều lũy linh; và hạt nhân của $\rho$, được chứa trong $k$ và trong $c$, là không, do đó $\rho$ là trung thành.

### Bài tập {#lie-i-s7-exercises}

Các quy ước của § 7 vẫn còn hiệu lực trừ khi có nói khác.

Xem [các bài tập của § 7](exercises/s7/).
