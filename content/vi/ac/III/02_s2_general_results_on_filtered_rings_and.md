---
book: ac
book_title: Commutative Algebra
chapter: III
chapter_title: GRADUATIONS. FILTRATIONS AND TOPOLOGIES
section: 2
section_title: General results on filtered rings and modules
lang: vi
source: ac-i-vii
book_pages: 162-195, 233-245
pdf_pages: 0182-0215, 0253-0265
extraction: ocr
subsections:
    - "no": 1
      title: FILTERED RINGS AND MODULES
      page: 162
      pdf_page: 182
    - "no": 2
      title: THE ORDER FUNCTION
      page: 165
      pdf_page: 185
    - "no": 3
      title: THE GRADED MODULE ASSOCIATED WITH A FILTERED MODULE
      page: 165
      pdf_page: 185
    - "no": 4
      title: HOMOMORPHISMS COMPATIBLE WITH FILTRATIONS
      page: 169
      pdf_page: 189
    - "no": 5
      title: THE TOPOLOGY DEFINED BY A FILTRATION
      page: 170
      pdf_page: 190
    - "no": 6
      title: COMPLETE FILTERED MODULES
      page: 173
      pdf_page: 193
    - "no": 7
      title: LINEAR COMPACTNESS PROPERTIES OF COMPLETE FILTERED MODULES
      page: 176
      pdf_page: 196
    - "no": 8
      title: THE LIFT OF HOMOMORPHISMS OF ASSOCIATED GRADED MODULES
      page: 177
      pdf_page: 197
    - "no": 9
      title: THE LIFT OF FAMILIES OF ELEMENTS OF AN ASSOCIATED GRADED MODULE
      page: 179
      pdf_page: 199
    - "no": 10
      title: 'APPLICATION: EXAMPLES OF NOETHERIAN RINGS'
      page: 183
      pdf_page: 203
    - "no": 11
      title: COMPLETE m-ADIC RINGS AND INVERSE LIMITS
      page: 185
      pdf_page: 205
    - "no": 12
      title: THE HAUSDORFF COMPLETION OF A FILTERED MODULE
      page: 187
      pdf_page: 207
    - "no": 13
      title: THE HAUSDORFF COMPLETION OF A SEMI-LOCAL RING
      page: 192
      pdf_page: 212
statements: 57
exercises: 13
content_sha256: 91252eda42cd43c67b0cf362d2d386d7140a09875316d4da9f51fdc92636851f
translated_from: content/en/ac/III/02_s2_general_results_on_filtered_rings_and.md
source_content_sha256: 8ef1e1745e256756c336640ea25cd38dd8a13bd1f46cf491dee2874345913e91
translation_model: gpt-5-6-mini, gpt-5.4
translation_run: translate-vi-61e6febe
glossary_version: 34
glossary_terms_sha256: f9b3d6461e2f1f2e801b4cb796a1632fe0d0c1c2839acb54f8505f14ac6d06f8
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 2. CÁC KẾT QUẢ CHUNG VỀ CÁC VÀNH VÀ MÔĐUN LỌC

### 1. CÁC VÀNH VÀ MÔĐUN LỌC

#### Định nghĩa 1 {#ac-iii-s2-def-1 .statement}

Một dãy tăng (tương ứng, giảm) $(G_n)_{n \in \mathbf{Z}}$ của các nhóm con của một nhóm $G$ được gọi là một lọc tăng (tương ứng, lọc giảm) trên $G$.
Một nhóm cùng với một lọc được gọi là một nhóm lọc.

Nếu $(G_n)_{n \in \mathbf{Z}}$ là một lọc tăng (tương ứng, giảm) trên một nhóm $G$ và ta viết $G'_n = G_{-n}$, rõ ràng $(G'_n)_{n \in \mathbf{Z}}$ là một lọc giảm (tương ứng, tăng) trên $G$. Do đó ta có thể hạn chế việc nghiên cứu của mình vào các lọc giảm và từ nay trở đi khi ta nói đến một lọc, ta sẽ hiểu đó là một lọc giảm, trừ khi có nói khác.

Cho một lọc giảm $(G_n)_{n \in \mathbf{Z}}$ trên một nhóm $G$, rõ ràng $\bigcap_{n \in \mathbf{Z}} G_n$ và $\bigcup_{n \in \mathbf{Z}} G_n$ là các nhóm con của $G$; lọc này được gọi là tách được nếu $\bigcup_{n \in \mathbf{Z}} G_n$ được thu gọn về phần tử đơn vị và đầy đủ nếu $\bigcup_{n \in \mathbf{Z}} G_n = G$.

#### Định nghĩa 2 {#ac-iii-s2-def-2 .statement}

Cho một vành $A$, một lọc $(A_n)_{n \in \mathbf{Z}}$ trên nhóm cộng $A$ được gọi là tương thích với cấu trúc vành trên $A$ nếu

(1)
$$
A_m A_n \subset A_{m+n} \quad \text{với} \quad m \in \mathbf{Z}, \quad n \in \mathbf{Z}
$$

(2)
$$
1 \in A_0.
$$
Vành $A$ với lọc này khi đó được gọi là một vành lọc.

Các điều kiện (1) và (2) chỉ ra rằng $A_n$ là một vành con của $A$ và các $A_n$ là các $A_0$-môđun (trái và phải). Tập hợp $B = \bigcup_{n \in \mathbf{Z}} A_n$ là một vành con của $A$ và tập hợp $n = \bigcap_{n \in \mathbf{Z}} A_n$, một iđêan hai phía của $B$; vì nếu $x \in n$ và $a \in A_k$ với mọi $k \in \mathbf{Z}$, $x \in A_{k-p}$, do đó $ax \in A$, và $xa \in A$, theo (1); vì vậy $ax \in n$ và $xa \in n$.

Một trường hợp riêng quan trọng là trường hợp trong đó $A_n = A$; khi đó $A_n = A$ với $n \leq 0$ và tất cả các $A_n$ đều là các iđêan hai phía của $A$.

#### Định nghĩa 3 {#ac-iii-s2-def-3 .statement}

Cho $A$ là một vành lọc, $(A_n)_{n \in \mathbf{Z}}$ là lọc của nó và $E$ là một $A$-môđun. Một lọc $(E_n)_{n \in \mathbf{Z}}$ trên $E$ được gọi là tương thích với cấu trúc môđun của nó trên vành lọc $A$ nếu
$$
A_m E_n \subset E_{m+n} \quad \text{với} \quad m \in \mathbf{Z}, \quad n \in \mathbf{Z}.
$$
$A$-môđun $E$ với lọc này được gọi là một môđun lọc.

Các $E_n$ đều là các $A_n$-môđun; nếu $B = \bigcup_{n \in \mathbf{Z}} A_n$, rõ ràng $\bigcup_{n \in \mathbf{Z}} E_n$ là một $B$-môđun và $\bigcap_{n \in \mathbf{Z}} E_n$ cũng vậy theo cùng lập luận như trên đối với $\bigcap_{n \in \mathbf{Z}} A_n$. Nếu $A_n = A$, tất cả các $E_n$ là các môđun con của $E$.

Ví dụ

(1) Cho $A$ là một vành phân bậc kiểu $\mathbf{Z}$; với mọi $i \in \mathbf{Z}$, cho $A_{(i)}$ là nhóm con các phần tử thuần nhất bậc $i$ trong $A$. Ta viết $A_n = \sum_{i \geq n} A_{(i)}$; khi đó ngay lập tức thấy rằng $(A_n)$ là một lọc giảm đầy đủ và tách được, tương thích với cấu trúc vành trên $A$; lọc này được gọi là liên kết với phép phân bậc $(A_{(i)})_{i \in \mathbf{Z}}$ và vành lọc $A$ được gọi là liên kết với vành phân bậc đã cho $A$.

Bây giờ cho $E$ là một môđun phân bậc kiểu $\mathbf{Z}$ trên vành phân bậc $A$ và với mọi $i \in \mathbf{Z}$ cho $E_{(i)}$ là nhóm con các phần tử thuần nhất bậc $i$ của $E$. Ta viết $E_n = \sum_{i \geq n} E_{(i)}$; khi đó $(E_n)$ là một lọc giảm đầy đủ và tách được, tương thích với cấu trúc môđun trên $E$ trên vành lọc $A$; lọc này được gọi là liên kết với phép phân bậc $(E_{(i)})_{i \in \mathbf{Z}}$ và môđun lọc $E$ được gọi là liên kết với môđun phân bậc đã cho $E$.

(2) Cho $A$ là một vành lọc, $(A_n)_{n \in \mathbf{Z}}$ là lọc của nó và $E$ là một $A$-môđun. Ta viết $E_n = A_n E$; từ (1) suy ra rằng
$$
A_m E_n = A_m A_n E \subset A_{m+n} E = E_{m+n},
$$
và từ (2) suy ra rằng $E_0 = E$; khi đó $(E_n)$ là một lọc đầy đủ tương thích với cấu trúc $A$-môđun trên $E$. Lọc này được gọi là dẫn xuất từ lọc đã cho $(A_n)$ trên $A$; chú ý rằng nó không nhất thiết phải tách được,

(3) Cho $A$ là một vành và $m$ là một iđêan hai phía của $A$. Ta viết $A_n = m^n$ với $n \geq 0$, $A_n = A$ với $n < 0$; ngay lập tức thấy rằng $(A_n)$ là một lọc đầy đủ trên $A$, được gọi là lọc $m$-adic. Cho $E$ là một $A$-môđun; lọc $(E_n)$ dẫn xuất từ lọc $m$-adic trên $A$ được gọi là lọc $m$-adic trên $E$; nói cách khác, $E_n = m^n E$ với $n \geq 0$ và $E_n = E$ với $n < 0$.

Nếu $A$ là giao hoán và $B$ là một $A$-đại số, $n = mB$ là một iđêan hai phía của $B$ và, với mọi $B$-môđun $F$, $n^k F = m^k F$ và do đó lọc $n$-adic trên $F$ trùng với lọc $m$-adic (nếu $F$ được xem như một $A$-môđun).

(4) Nếu $A$ là một vành có lọc và $(A_n)$ là lọc của nó, $A$-môđun trái $A_n$ là một $A$-môđun có lọc với lọc $(A_n)$. Mặt khác, rõ ràng $(A_n)$ là một lọc tương thích với cấu trúc vành trên vành đối $A^0$ và $A_n$ là một $A^0$-môđun (trái) có lọc với lọc $(A_n)$.

(5) Trên một vành $A$, các tập hợp $A_n$ sao cho $A_n = 0$ với $n > 0$, $A_n = A$ với $n \leq 0$ tạo thành cái được gọi là một lọc tầm thường liên kết (Ví dụ 1) với phân bậc tầm thường trên $A$; trên một $A$-môđun $E$, mọi lọc $(E_n)$ gồm các môđun con-$A$ khi đó đều tương thích với cấu trúc môđun trên $E$ trên vành có lọc $A$. Khi đó có thể nói rằng mọi nhóm giao hoán có lọc $G$ là một $\mathbf{Z}$-môđun có lọc, nếu $\mathbf{Z}$ được cho lọc tầm thường.

Cho $G$ là một nhóm có lọc và $(G_n)_{n \in \mathbf{Z}}$ là lọc của nó; rõ ràng, với mọi nhóm con $H$ của $G$, $(H \cap G_n)_{n \in \mathbf{Z}}$ là một lọc được gọi là cảm sinh bởi lọc trên $G$; nó là đầy đủ (tương ứng, tách biệt) nếu lọc trên $G$ là như vậy. Tương tự, nếu $H$ là một nhóm con chuẩn của $G$, họ $((H.G_n)/H)_{n \in \mathbf{Z}}$ là một lọc trên nhóm $G/H$, được gọi là lọc thương dưới $H$ của lọc trên $G$; nó là đầy đủ nếu $(G_n)$ là như vậy. Nếu $G'$ là một nhóm có lọc khác và $(G'_n)_{n \in \mathbf{Z}}$ là lọc của nó, $(G_n \times G'_n)$ là một lọc trên $G \times G'$ được gọi là tích của các lọc trên $G$ và $G'$, nó là đầy đủ (tương ứng, tách biệt) nếu $(G_n)$ và $(G'_n)$ là như vậy.

Bây giờ cho $A$ là một vành có lọc và $(A_n)$ là lọc của nó; trên mọi vành con $B$ của $A$, rõ ràng lọc cảm sinh bởi lọc trên $A$ là tương thích với cấu trúc vành trên $B$. Nếu $b$ là một iđêan hai phía của $A$, lọc thương trên $A/b$ của lọc trên $A$ là tương thích với cấu trúc của vành này, vì
$$
(A_n + b)(A_m + b) \subset A_{n+m} + b.
$$
Nếu $A'$ là một vành có lọc khác, lọc tích trên $A \times A'$ là tương thích với cấu trúc của vành này.

Cuối cùng, cho $E$ là một A-môđun được lọc và $(E_n)$ là lọc của nó; trên mọi môđun con $F$ của $E$, lọc cảm sinh bởi lọc của $E$ là tương thích với cấu trúc A-môđun trên $F$ và, trên môđun thương $E/F$, lọc thương của lọc của $E$ là tương thích với cấu trúc A-môđun, vì
$$
A_n(F + E_m) \subset F + A_n E_m \subset F + E_{m+n}.
$$

Nếu E' là một A-môđun được lọc khác, thì lọc tích trên E × E' là tương thích với cấu trúc A-môđun của nó. Nếu các lọc trên E và E' được dẫn xuất từ lọc trên A (Ví dụ 2), thì lọc tích của chúng cũng vậy.

### 2. HÀM CẤP

Cho A là một vành được lọc, E là một A-môđun được lọc và $(E_n)$ là lọc của E. Với mọi x ∈ E, ký hiệu v(x) là cận trên *nhỏ nhất* trong R của tập các số nguyên n ∈ Z sao cho x ∈ E_n. Khi đó các tương đương sau đúng:

$$
\begin{cases}
v(x) = -∞ \Leftrightarrow x \notin \bigcup_{n \in \mathbf{Z}} E_n \\
v(x) = p \Leftrightarrow x \in E_p \text{ và } x \notin E_{p+1} \\
v(x) = +∞ \Leftrightarrow x \in \bigcap_{n \in \mathbf{Z}} E_n
\end{cases}
$$

Ánh xạ v : E → \overline{\mathbf{R}} được gọi là hàm cấp của môđun được lọc E. Nếu biết v thì cũng biết các E_n, vì E_n là tập các x ∈ E sao cho v(x) ≥ n; việc các E_n là những nhóm con cộng tính của E kéo theo quan hệ

$$
v(x - y) \geq \inf(v(x), v(y)).
$$

Định nghĩa trên áp dụng đặc biệt cho A-môđun được lọc A; gọi w là hàm cấp của nó. Từ công thức (3) của no. 1 suy ra rằng với a ∈ A và x ∈ E,

$$
v(ax) \geq w(a) + v(x)
$$
mỗi khi vế phải được xác định; đặc biệt, với a ∈ A và b ∈ A,

$$
w(ab) \geq w(a) + w(b)
$$
mỗi khi vế phải được xác định.

*Hàm cấp* được định nghĩa tương tự trên một nhóm được lọc G không nhất thiết giao hoán; khi đó quan hệ tương ứng với (5) được viết là

$$
v(yx^{-1}) = v(xy^{-1}) \geq \inf(v(x), v(y)).
$$

### 3. MÔĐUN PHÂN BẬC LIÊN KẾT VỚI MỘT MÔĐUN ĐƯỢC LỌC

Cho G là một nhóm giao hoán (viết theo lối cộng tính) và (G_n) là một lọc trên G. Ta viết

$$
\begin{align*}
\operatorname{gr}_n(G) &= G_n / G_{n+1} \quad \text{với } n \in \mathbf{Z} \\
\operatorname{gr}(G) &= \bigoplus_{n \in \mathbf{Z}} \operatorname{gr}_n(G).
\end{align*}
$$

Khi đó nhóm giao hoán gr(G) là một nhóm phân bậc kiểu $\mathbf{Z}$, được gọi là *nhóm phân bậc liên kết* với nhóm được lọc G, các phần tử thuần nhất bậc $n$ của gr(G) là các phần tử của $\mathrm{gr}_n(G)$.

Bây giờ cho A là một vành được lọc, (A,) là lọc của nó, E là một A-môđun được lọc và $(E_n)$ là lọc của nó. Với mọi $p \in \mathbf{Z}$, $q \in \mathbf{Z}$, một ánh xạ

$$
\mathrm{gr}_p(A) \times \mathrm{gr}_q(E) \to \mathrm{gr}_{p+q}(E)
$$

được định nghĩa như sau: cho $a \in \mathrm{gr}_p(A)$, $\xi \in \mathrm{gr}_q(E)$, hai đại diện $a, a'$ của $a$ và hai đại diện $x, x'$ của $\xi$, ta có $ax \in E_{p+q}$, $a'x' \in E_{p+q}$ và $ax \equiv a'x'$ (mod. $E_{p+q+1}$), vì

$$
ax - a'x' = (a - a')x + a'(x - x')
$$

và $a - a' \in A_{p+1}$ và $x - x' \in E_{q+1}$ và do đó mệnh đề của chúng ta suy ra từ công thức (3) của no. 1. Vậy ta có thể ký hiệu bởi $\alpha\xi$ lớp trong

$$
E_{p+1}/E_{p+q+1} = \mathrm{gr}_{p+q}(E)
$$

của tích $ax$ của một đại diện bất kỳ $a \in a$ và một đại diện bất kỳ $x \in \xi$. Ngay lập tức thấy rằng ánh xạ (9) là *song tuyến tính trên Z*; bằng tính tuyến tính, ta dẫn xuất được một ánh xạ song tuyến tính trên $\mathbf{Z}$

$$
\mathrm{gr}(A) \times \mathrm{gr}(E) \to \mathrm{gr}(E).
$$

Nếu trước hết áp dụng định nghĩa này cho trường hợp $E = A_0$, thì ánh xạ (10) là một luật hợp thành trong trên $\mathrm{gr}(A)$, và ngay lập tức kiểm tra được rằng nó là *kết hợp* và có một phần tử đơn vị là ảnh chính tắc trong $\mathrm{gr}_0(A)$ của phần tử đơn vị của A; do đó nó xác định trên $\mathrm{gr}(A)$ một cấu trúc vành và theo định nghĩa, phân bậc $(\mathrm{gr}_n(A))_{n \in \mathbf{Z}}$ là tương thích với cấu trúc này. Vành phân bậc $\mathrm{gr}(A)$ (kiểu $\mathbf{Z}$) được xác định như vậy được gọi là *vành phân bậc liên kết* với vành được lọc A; hiển nhiên nó giao hoán nếu A giao hoán; $\mathrm{gr}_0(A)$ là một vành con của $\mathrm{gr}(A)$. Mặt khác, ánh xạ (10) là một phép toán ngoài môđun trên $\mathrm{gr}(A)$ trên $\mathrm{gr}(E)$, các tiên đề môđun được thỏa mãn một cách tầm thường, và phân bậc $(\mathrm{gr}_n(E))_{n \in \mathbf{Z}}$ trên $\mathrm{gr}(E)$ hiển nhiên là tương thích với cấu trúc môđun này. Môđun phân bậc $\mathrm{gr}(A)$-môđun $\mathrm{gr}(E)$ (kiểu $\mathbf{Z}$) được xác định như vậy được gọi là *môđun phân bậc liên kết* với A-môđun được lọc E.

*Ví dụ*

#### Ví dụ 1 {#ac-iii-s2-n3-exa-1 .statement}

Cho A là một vành giao hoán và $t$ là một phần tử của A không phải là ước của 0. Hãy trang bị cho A *lọc* *adic theo (t)* (no. 1, *Ví dụ 3*). Khi đó vành phân bậc liên kết $\mathrm{gr}(A)$ đẳng cấu chính tắc với *vành đa thức* $(A/(t))[X]$. Thật vậy, $\mathrm{gr}_n(A) = 0$ với $n < 0$ và theo định nghĩa vành $\mathrm{gr}_0(A)$ là vành $A/(t)$. Bây giờ ta chú ý rằng, do giả thiết đặt trên $t$, quan hệ $at^n \equiv 0$ (mod. $t^{n+1}$) tương đương với $a \equiv 0$ (mod. $t$); nếu $\tau$ là ảnh chính tắc của $t$ trong $\mathrm{gr}_1(A)$, thì mọi phần tử của $\mathrm{gr}_n(A)$ khi đó có thể được viết duy nhất dưới dạng $\alpha \tau^n$ với $\alpha \in \mathrm{gr}_0(A)$; do đó có mệnh đề của ta.

#### Ví dụ 2 {#ac-iii-s2-n3-exa-2 .statement}

Cho $K$ là một vành giao hoán, $A$ là vành các chuỗi lũy thừa hình thức

$$
K[[X_1,\ldots,X_r]]
$$

(*Đại số, Chương IV, § 5*) và $m$ là iđêan của $A$ mà các phần tử là các chuỗi lũy thừa hình thức không có số hạng hằng. Hãy trang bị cho $A$ *lọc* adic theo $m$ (no. 1, *Ví dụ 3*); nếu $M_1,\ldots,M_s$ là các đơn thức phân biệt theo $X_1,\ldots,X_r$ có bậc toàn phần bằng $n-1$, thì rõ ràng mọi chuỗi lũy thừa hình thức $u$ có cấp toàn phần $\omega(u)\geq n$

*(loc. cit., no. 2)* đều có thể được viết thành $\displaystyle\sum_{k=1}^{s}u_kM_k$, trong đó các $u_k$ thuộc $m$; ta **thấy** rằng $m^n$ là tập hợp các chuỗi lũy thừa hình thức $u$ sao cho $\omega(u)\geq n$, điều này cho thấy rằng $\omega$ là *hàm cấp* của lọc adic theo $m$. Khi đó rõ ràng, với mọi chuỗi lũy thừa hình thức $u\in m^n$, tồn tại duy nhất một *đa thức thuần nhất* bậc $n$ theo các $X_i$ đồng dư với $u$ mod. $m^{n+1}$, cụ thể là tổng các số hạng bậc $n$ của $u$; ta kết luận rằng $\operatorname{gr}(A)$ đẳng cấu chính tắc với *vành đa thức* $K[X_1,\ldots,X_r]$.

#### Ví dụ 3 {#ac-iii-s2-n3-exa-3 .statement}

Nói chung hơn, cho $A$ là một vành giao hoán, $b$ một iđêan của $A$ và $A$ được trang bị lọc $b$-adic. Nếu viết $B=\operatorname{gr}_0(A)$, $F=\operatorname{gr}_1(A)=b/b^2$, ta biết (*Đại số, Chương III*) rằng ánh xạ đồng nhất của $B$-môđun $F$ lên chính nó có thể được mở rộng duy nhất thành một đồng cấu $u$ từ *đại số đối xứng* $S(F)$ của $F$ đến $B$-đại số $\operatorname{gr}(A)$; suy ra từ định nghĩa của $\operatorname{gr}(A)$ rằng $u$ là một *đồng cấu toàn ánh của các đại số phân bậc*; với $n\geq1$, mọi phần tử của $\operatorname{gr}_n(A)$ là một tổng của các lớp mod $b^{n+1}$ của các phần tử có dạng $y=x_1x_2\cdots x_n$, trong đó $x_i\in b$ $(1\leq i\leq n)$; nếu $\xi_i$ là lớp của $x_i$ mod. $b^2$, rõ ràng lớp của $y$ mod. $b^{n+1}$ là phần tử $u(\xi_1)\cdots u(\xi_n)$, do đó có mệnh đề của chúng ta. Đặc biệt, mọi hệ sinh của $B$-môđun $F$ là một hệ sinh của $B$-đại số $\operatorname{gr}(A)$.

Nếu bây giờ $E$ là một $A$-môđun và $E$ được trang bị lọc $b$-adic, ta thấy tương tự rằng $\operatorname{gr}(A)$-môđun phân bậc $\operatorname{gr}(E)$ được *sinh* bởi $\operatorname{gr}_0(E)=E/bE$. Cụ thể hơn, hạn chế $\phi$ trên $\operatorname{gr}(A)\times\operatorname{gr}_0(E)$ của luật ngoài trên $\operatorname{gr}(A)$-môđun $\operatorname{gr}(E)$ là một ánh xạ song tuyến tính $\mathbf{Z}$ từ $\operatorname{gr}(A)\times\operatorname{gr}_0(E)$ vào $\operatorname{gr}(E)$; hơn nữa $\operatorname{gr}(A)$ là một $(\operatorname{gr}_0(A),\operatorname{gr}_0(A))$-song môđun và $\operatorname{gr}_0(E)$ là một $\operatorname{gr}_0(A)$-môđun; ta kiểm tra ngay lập tức rằng, với $a\in\operatorname{gr}(A)$, $\alpha_0\in\operatorname{gr}_0(A)$, $\xi\in\operatorname{gr}_0(E)$,

$$
\phi(a\alpha_0,\xi)=\phi(a,\alpha_0\xi)
$$

và do đó $\phi$ xác định một ánh xạ tuyến tính toàn ánh *chính tắc* $\operatorname{gr}_1(A)$

(11)

$$
\gamma_E:\operatorname{gr}(A)\otimes_{\operatorname{gr}_0(A)}\operatorname{gr}_0(E)\longrightarrow\operatorname{gr}(E)
$$

được gọi là *chính tắc*.

#### Ví dụ 4 {#ac-iii-s2-n3-exa-4 .statement}

Cho $K$ là một vành giao hoán, $\mathfrak g$ là một đại số Lie trên $K$ và $U$ là đại số bao phủ của $\mathfrak g$. Một *lọc tăng* $(U_n)_{n\in\mathbf{Z}}$ được xác định trên $U$ bằng cách lấy $U_n=\{0\}$ đối với $n<0$ và ký hiệu bởi $U_n$, với $n\geq0$, tập hợp các phần tử của $U$ có thể được biểu diễn thành một tổng các tích của nhiều nhất $n$ phần tử của $\mathfrak g$, khi đó

U_0 = K và gr(U) là một đại số giao hoán trên K (Các nhóm Lie và các đại số Lie, Chương I, § 2, no. 6). Ánh xạ chính tắc của g vào gr_1(U) = U_1/U_0 có thể được mở rộng duy nhất thành một đồng cấu h của đại số đối xứng $S(g)$ của K-môđun g vào đại số trên K gr(U); đồng cấu h là toàn ánh và, nếu K-môđun g là tự do, h là song ánh (sđd., no. 7, Định lý 1).

#### Ví dụ 5 {#ac-iii-s2-n3-exa-5 .statement}

Cho A là một vành phân bậc kiểu $\mathbf{Z}$ và E là một A-môđun phân bậc kiểu $\mathbf{Z}$; ký hiệu $A_{(i)}$ (tương ứng $E_{(i)}$) là nhóm con của các phần tử thuần nhất bậc i của A (tương ứng E). Cho A và E các lọc liên kết với các phân bậc của chúng (no. 1, Ví dụ 1) và ký hiệu A' và E' là vành có lọc và A-môđun có lọc thu được như vậy. Khi đó ngay lập tức thấy rằng ánh xạ tuyến tính trên Z $A \to \mathrm{gr}(A')$ biến một phần tử của $A_{(n)}$ thành ảnh chính tắc của nó trong
$$
\mathrm{gr}_n(A) = \left( \bigoplus_{i \geq n} A_{(i)} \right) / \left( \bigoplus_{i \geq n+1} A_{(i)} \right)
$$
là một đẳng cấu vành phân bậc. Một đẳng cấu A-môđun phân bậc chính tắc $E \to \mathrm{gr}(E')$ được xác định tương tự.

#### Mệnh đề 1 {#ac-iii-s2-prop-1 .statement}

Cho A là một vành có lọc, $(A_n)_{n \in \mathbf{Z}}$ là lọc của nó và v là hàm bậc của nó. Giả sử rằng $\mathrm{gr}(A)$ là một vành không có ước của không. Khi đó, với mọi cặp có thứ tự của các phần tử a, b của vành $B = \bigcup_{n \in \mathbf{Z}} A_n$, $v(ab) = v(a) + v(b)$.

Vì $n = \bigcap_{n \in \mathbf{Z}} A_n$ là một iđêan hai phía của vành B, công thức đúng nếu $v(a)$ hoặc $v(b)$ bằng $+\infty$. Nếu không, $v(a) = r$ và $v(b) = s$ là các số nguyên; các lớp $\alpha$ của a mod. A, +, và $\beta$ của b mod. A, +_1 là $\neq 0$ theo định nghĩa, do đó theo giả thiết $\alpha \beta \neq 0$ trong $\mathrm{gr}(A)$ và vì vậy $ab \notin A_{r+s+1}$, vì $ab \in A_{r+s}$,
$$
v(ab) = v(a) + v(b).
$$

#### Hệ quả {#ac-iii-s2-n3-cor-1 .statement}

Cho A là một vành có lọc và $(A_n)_{n \in \mathbf{Z}}$ là lọc của nó; đặt $B = \bigcup_{n \in \mathbf{Z}} A_n$, $n = \bigcap_{n \in \mathbf{Z}} A_n$. Nếu vành $\mathrm{gr}(A)$ không có các ước của không, thì vành $B/n$ cũng không có các ước của không.
Nếu a và b là các phần tử của B không thuộc n, thì $v(a) \neq +\infty$ và $v(b) \neq +\infty$, do đó $v(ab) \neq +\infty$ và vì vậy $ab \notin n$.

Chú ý rằng vành A có thể là một miền nguyên và lọc (A,,) đầy đủ và tách mà không có $\mathrm{gr}(A)$ là một miền nguyên (Bài tập 2).

#### Nhận xét {#ac-iii-s2-n3-rem-1 .statement}

Cho G là một nhóm không nhất thiết giao hoán với một lọc $(G_n)_{n \in \mathbf{Z}}$ sao cho $G_{n+1}$ là chuẩn trong G, với mọi $n \in \mathbf{Z}$; lại đặt $\mathrm{gr}_n(G) = G_n/G_{n+1}$. Tích hạn chế của họ $(\mathrm{gr}_n(G))_{n \in \mathbf{Z}}$, nghĩa là nhóm con của tích $\prod_{n \in \mathbf{Z}} \mathrm{gr}_n(G)$ gồm các phần tử $(\xi_n)$ mà tất cả các thành phần của chúng, trừ nhiều nhất một số hữu hạn, đều bằng phần tử đơn vị, cũng được gọi là nhóm phân bậc liên kết với G và được ký hiệu bởi $\mathrm{gr}(G)$.

### 4. CÁC ĐỒNG CẤU TƯƠNG THÍCH VỚI CÁC LỌC

Cho G, G' là hai nhóm giao hoán (viết theo phép cộng), (G,) là một lọc trên G và (G'_n) là một lọc trên G'; một đồng cấu h : G → G' được gọi là tương thích với các lọc trên G và G' nếu h(G_n) ⊂ G'_n với mọi n ∈ Z. Đồng cấu hợp thành G, $\xrightarrow{h} G'_n \longrightarrow G'_n/G'_{n+1}$ là không trên G_{n+1} và do đó xác định bằng cách lấy thương một đồng cấu h, : G_n/G_{n+1} → G'_n/G'_{n+1}; vì vậy tồn tại duy nhất một đồng cấu nhóm cộng tính gr(h) : gr(G) → gr(G') sao cho, với mọi n ∈ Z, gr(h) trùng với h, trên gr_n(G) = G_n/G_{n+1}. gr(h) được gọi là đồng cấu nhóm phân bậc liên kết với h. Nếu G'' là một nhóm có lọc thứ ba và h' : G' → G'' là một đồng cấu tương thích với các lọc, h' ∘ h là một đồng cấu tương thích với các lọc và

(12)
$$
\operatorname{gr}(h' \circ h) = \operatorname{gr}(h') \circ \operatorname{gr}(h)
$$

#### Mệnh đề 2 {#ac-iii-s2-prop-2 .statement}

Cho G là một nhóm giao hoán có lọc và H là một nhóm con của G; cho H cấu trúc lọc cảm sinh và G/H cấu trúc lọc thương. Nếu j : H → G là đơn ánh chính tắc và p : G → G/H là toàn cấu chính tắc, thì j và p tương thích với các cấu trúc lọc và dãy

(13)
$$
0 \longrightarrow \operatorname{gr}(H) \xrightarrow{\operatorname{gr}(j)} \operatorname{gr}(G) \xrightarrow{\operatorname{gr}(p)} \operatorname{gr}(G/H) \longrightarrow 0
$$
là khớp.

Mệnh đề đầu tiên là hiển nhiên; nếu (G,,) là cấu trúc lọc trên G, thì
$$
(H \cap G_n) \cap G_{n+1} = H \cap G_{n+1}
$$
và do đó gr(j) là đơn ánh; hơn nữa ánh xạ chính tắc
$$
G_n \to (H + G_n)/H
$$
là toàn ánh, do đó gr(p) cũng là toàn ánh và gr(p) ∘ gr(j) = 0 theo (12). Cuối cùng, cho $\xi \in G_n/G_{n+1}$ thuộc hạt nhân của gr(p); khi đó tồn tại x ∈ ξ sao cho x ∈ H + G_{n+1}; nhưng vì G_{n+1} ⊂ G,
$$
G_n \cap (H + G_{n+1}) = (H \cap G_n) + G_{n+1}
$$
và do đó x = y + z trong đó y ∈ H ∩ G, và z ∈ G, +_1; điều này chứng minh rằng ξ là lớp mod. G, +_1 của j(y), nói cách khác nó thuộc ảnh của gr(H) qua gr(j).

Chú ý rằng, với một dãy khớp 0 → G' \xrightarrow{u} G \xrightarrow{v} G'' → 0 của các nhóm giao hoán có lọc, trong đó u và v tương thích với các cấu trúc lọc, dãy 0 \longrightarrow \operatorname{gr}(G') \xrightarrow{\operatorname{gr}(u)} \operatorname{gr}(G) \xrightarrow{\operatorname{gr}(v)} \operatorname{gr}(G'') \longrightarrow 0 không nhất thiết là khớp (Bài tập 4).

Nếu bây giờ A và B là hai vành có lọc và h: A → B là một đồng cấu vành tương thích với các cấu trúc lọc, thì kiểm tra ngay lập tức rằng đồng cấu nhóm phân bậc gr(h): gr(A) → gr(B) cũng là một đồng cấu vành. Đặc biệt, nếu A' là một vành con của A với cấu trúc lọc cảm sinh, thì gr(A') được đồng nhất một cách chính tắc với một vành con phân bậc của gr(A) (Mệnh đề 2); nếu b là một iđêan hai phía của A và A/b được cho cấu trúc lọc thương, thì gr(A/b) được đồng nhất một cách chính tắc với vành phân bậc thương gr(A)/gr(b) (Mệnh đề 2).

Cuối cùng, cho A là một vành có lọc, E, F là hai A-môđun có lọc và u : E → F là một đồng cấu tương thích với các cấu trúc lọc. Khi đó hiển nhiên rằng gr(u) : gr(E) → gr(F) là một ánh xạ gr(A)-tuyến tính và do đó là một đồng cấu thuần nhất bậc 0 của các gr(A)-môđun phân bậc. Hơn nữa, nếu u' : E → F là một A-đồng cấu khác tương thích với các cấu trúc lọc, thì u + u' cũng vậy và

$$
\operatorname{gr}(u + u') = \operatorname{gr}(u) + \operatorname{gr}(u').
$$

Nhận xét

(1) Rõ ràng các đồng cấu vành có lọc (tương ứng các đồng cấu của các môđun có lọc trên một vành có lọc A đã cho) tương thích với các cấu trúc lọc có thể được lấy làm các cấu xạ cho cấu trúc vành có lọc (tương ứng cấu trúc A-môđun có lọc) (Lý thuyết tập hợp, Chương IV, § 2, no. 1).

(2) Cho E và F là hai môđun trên một vành có lọc A và cho chúng các cấu trúc lọc dẫn xuất từ cấu trúc lọc (A_n) trên A (no. 1, Ví dụ 2). Khi đó mọi ánh xạ A-tuyến tính u : E → F đều tương thích với các cấu trúc lọc, vì

$$
u(A_nE) = A_nu(E) \subset A_nF.
$$

(3) Chú ý rằng một đồng cấu môđun A có lọc u : E → F tương thích với các cấu trúc lọc có thể thỏa mãn gr(u) = 0 mà không bằng không; ví dụ điều này đúng với tự đồng cấu x ↦ nx của nhóm cộng $\mathbf{Z}$ với cấu trúc lọc (n)-adic (với mọi số nguyên n > 1). Quan hệ gr(u) = gr(v) đối với hai đồng cấu u, v từ E đến F, tương thích với các cấu trúc lọc, do đó không suy ra nhất thiết u = u.

(4) Các định nghĩa ở đầu số này mở rộng ngay lập tức cho hai nhóm G, G', không nhất thiết giao hoán và được lọc bởi các nhóm con $G_n, G'_n$ sao cho $G_{n+1}$ (tương ứng. $G'_{n+1}$) là chuẩn trong G, (tương ứng. $G'_n$). Mệnh đề 2 cũng đúng với cùng các giả thiết trên G, và giả sử rằng H là bất biến trong G, chứng minh vẫn không thay đổi ngoại trừ ký hiệu.

### 5. TÔPÔ ĐƯỢC XÁC ĐỊNH BỞI MỘT CẤU TRÚC LỌC

Cho G là một nhóm được lọc bởi một họ $(G_n)_{n \in \mathbf{Z}}$ các nhóm con chuẩn của G. Tồn tại một tôpô duy nhất trên G tương thích với cấu trúc nhóm và sao cho các G, tạo thành một hệ lân cận cơ bản của phần tử đơn vị e của G (Tôpô đại cương, Chương III, § 1, no. 2, Ví dụ); nó được gọi là tôpô trên G được xác định bởi cấu trúc lọc (G,). Khi ta sử dụng các khái niệm tôpô liên quan đến một nhóm có lọc, ta sẽ hiểu, trừ khi có nói khác, với tôpô được xác định bởi cấu trúc lọc. Chú ý rằng các G,, là các nhóm con của G, đều mở và đóng (Tôpô đại cương, Chương III, § 2, no. 1, Hệ quả của Mệnh đề 4).

Vì mỗi G, là chuẩn trong G, các lân cận của các đồng đều trái và phải trên G trùng nhau; ta suy ra rằng G thừa nhận một nhóm hoàn thiện Hausdorff $\hat{G}$ (Tôpô đại cương, Chương III, § 3, no. 4, Định lý 1 và no. 1, Mệnh đề 2).

Với mọi tập con M của G, bao đóng của M trong G bằng

$$
\bigcap_{n \in \mathbf{Z}} (M . G_n) = \bigcap_{n \in \mathbf{Z}} (G_n . M)
$$

(Tôpô đại cương, Chương III, § 3, no. 1, công thức (1)); đặc biệt $\bigcap_{n \in \mathbf{Z}} G$, là bao đóng của $\{e\}$; do đó thấy rằng để tôpô trên G là Hausdorff thì cần và đủ rằng cấu trúc lọc (G,) là tách. Để tôpô trên G là rời rạc, cần và đủ rằng tồn tại $n \in \mathbf{Z}$ sao cho $G_+ = \{e\}$ (trong trường hợp đó $G_m = \{e\}$ với $m \geq n$); khi đó cấu trúc lọc (G,) được gọi là rời rạc.

Vì nhóm Hausdorff liên kết với G là $H = G / \left( \bigcap_{n \in \mathbf{Z}} G_n \right)$, các nhóm phân bậc liên kết gr(G) và gr(H) (nếu H được cho cấu trúc lọc thương) được đồng nhất một cách chính tắc.

Bây giờ, cho G' là một nhóm lọc khác và $u : G \to G'$ là một đồng cấu tương thích với các lọc; định nghĩa của các tôpô trên G và G' cho thấy ngay lập tức rằng $u$ liên tục (*). Nếu H là một nhóm con (tương ứng, nhóm con chuẩn tắc) của G, thì tôpô cảm sinh trên H bởi tôpô của G (tương ứng, tôpô thương theo H của tôpô đó) là tôpô trên H (tương ứng, G/H) được xác định bởi lọc cảm sinh từ lọc của G (tương ứng, tôpô thương của lọc đó). Tôpô tích của các tôpô trên G và G' là tôpô được xác định bởi tích của các lọc trên G và G'.

Cho v là hàm cấp (no. 2) trên G. Giả thiết về G suy ra rằng $v(xy x^{-1}) = v(y)$ và do đó $v(xy^{-1}) = v(yx^{-1}) = v(x^{-1}y) = v(y^{-1}x)$ với mọi x, y trong G. Cho $\rho$ là một số thực sao cho $0 < \rho < 1$ (chẳng hạn lấy

(*) Trong toàn bộ chương này chúng tôi sẽ dùng các từ "continuous homomorphism" theo nghĩa của điều được gọi là "continuous representation" trong *General Topology*, Chapter III, § 2, no. 8; từ "homomorphism" sẽ không bao giờ được dùng theo nghĩa của *General Topology*, Chapter III, § 2, no. 8, Definition 1; đối với khái niệm này chúng tôi sẽ luôn dùng thuật ngữ "strict morphism" để tránh mọi sự nhầm lẫn.

$\rho = 1/e$ và đặt $d(x, y) = \rho^{v(xy^{-1})}$ với mọi $x, y$ trong G. Khi đó $d(x, x) = 0, d(x, y) = d(y, x)$ và bất đẳng thức (5') của no. 2 cho

$$
(15) \quad d(x, y) \leq \sup(d(x, z), d(y, z))
$$

với mọi $x, y, z$ trong G, điều này suy ra bất đẳng thức tam giác

$$
d(x, y) \leq d(x, z) + d(y, z).
$$

Vì vậy $d$ là một *giả khoảng cách* trên G, bất biến qua các phép tịnh tiến trái và phải, và G, là tập các $x \in G$ sao cho $d(e, x) < \rho^n$; cấu trúc đều được xác định bởi $d$ khi đó là cấu trúc đều trên nhóm tôpô G. Nếu G Hausdorff, thì G là một không gian tôpô mêtric *không chiều* (*General Topology*, Chapter IX, § 6, no. 4); $d$ là một *khoảng cách* trên G nếu thêm nữa lọc (G,) là phủ hết.

Cho một vành tôpô A, nhắc lại rằng một *A-môđun tôpô trái* là một A-môđun E được trang bị một tôpô tương thích với cấu trúc nhóm cộng của nó và sao cho ánh xạ $(a, x) \mapsto ax$ từ $A \times E$ vào E là liên tục (*General Topology*, Chapter III, § 6, no. 6).

#### Mệnh đề 3 {#ac-iii-s2-prop-3 .statement}

*Cho A là một vành lọc, (A,) là lọc của nó, B là vành con $\bigcup_{n \in \mathbf{Z}} A_n$ của A, E là một B-môđun lọc, (E_n) là lọc của nó, và F là B-môđun con $\bigcup_{n \in \mathbf{Z}} E_n$ của E. Khi đó ánh xạ $(a, x) \mapsto ax$ từ $B \times F$ vào F là liên tục.*

Cho $a, \in B, x_0 \in F$; theo giả thiết tồn tại các số nguyên $r, s$ sao cho $a_0 \in A_r$ và $x_0 \in E_s$. Quan hệ

$$
ax - a_0x_0 = (a - a_0)x_0 + a_0(x - x_0) + (a - a_0)(x - x_0)
$$

cho thấy rằng nếu $a - a_0 \in A_i$ và $x - x_0 \in E_j$, thì $ax - a_0x_0$ thuộc

$$
E_{i+s} + E_{j+r} + E_{i+j}.
$$

Vậy, với một số nguyên $n$ cho trước, ta có $ax - a_0x_0 \in E_n$ miễn là $i \geq n - s, j \geq n - r$ và $i + j \geq n$, tức là miễn là $i$ và $j$ đủ lớn.

#### Hệ quả {#ac-iii-s2-n5-cor-1 .statement}

*B là một vành tôpô và B-môđun F là một B-môđun tôpô.*

Khẳng định thứ nhất thu được bằng cách áp dụng Mệnh đề 3 cho $F = B$.

Đặc biệt, ta thấy rằng một vành lọc A mà lọc của nó là *phủ hết* là một vành tôpô; nếu đúng như vậy thì mọi A-môđun lọc mà lọc của nó là *phủ hết* đều là một A-môđun tôpô.

#### Mệnh đề 4 {#ac-iii-s2-prop-4 .statement}

*Cho A là một vành giao hoán được lọc bởi một lọc phủ hết (A,) và p là một iđêan của A. Giả sử rằng iđêan $\operatorname{gr}(p) = \bigoplus_{n \in \mathbf{Z}} (p \cap A_n)/(p \cap A_{n+1})$ của vành $\operatorname{gr}(A)$ là nguyên tố. Khi đó bao đóng của p trong A là một iđêan nguyên tố.*

Ta biết rằng gr(A/p) đẳng cấu với gr(A)/gr(p) (no. 4, Proposition 2) và do đó là một miền nguyên; ta kết luận rằng $A / \bigcap_{n \in \mathbf{Z}} (p + A_n)$ là một miền nguyên (no. 3, Corollary to Proposition 1). Vậy bao đóng $\bigcap_{n \in \mathbf{Z}} (p + A_n)$ của $p$ là một iđêan nguyên tố.

Cho $A$ là một vành và $m$ là một iđêan hai phía của $A$; tôpô được xác định trên $A$ bởi lọc $m$-adic (no. 1, Example 3) được gọi là *tôpô m-adic*; vì lọc *m*-adic là phủ hết, $A$ là một vành tôpô đối với tôpô này (Corollary to Proposition 3). Tương tự, với mọi $A$-môđun $E$, tôpô được xác định bởi lọc $m$-adic được gọi là *tôpô m-adic* trên $E$; $E$ là một $A$-môđun tôpô đối với tôpô này.

Cho $m'$ là một iđêan hai phía khác của $A$; để tôpô $m'$-adic trên $A$ mịn hơn tôpô $m$-adic, điều kiện cần và đủ là tồn tại một số nguyên $n > 0$ sao cho ${m'}^n \subset m$; điều kiện này là cần và, nếu nó được thỏa mãn, thì ${m'}^{hn} \subset m^h$ với mọi $h > 0$ và do đó điều kiện này là đủ. Nếu $A$ là một *vành Noether giao hoán*, thì điều đó tương đương với việc nói rằng $V(m) \subset V(m')$ trong phổ nguyên tố của $A$ (Chương II, § 4, no. 3, Hệ quả 2 của Mệnh đề 11 và § 2, no. 6, Mệnh đề 15).

### 6. MÔĐUN LỌC ĐẦY ĐỦ

#### Mệnh đề 5 {#ac-iii-s2-prop-5 .statement}

*Cho $G$ là một nhóm được lọc mà phép lọc $(G,)$ gồm các nhóm con bất biến của $G$. Các điều kiện sau là tương đương:*

(a) $G$ là một nhóm tôpô đầy đủ.

(b) *Nhóm Hausdorff liên kết* $G' = G / (\bigcap_{n \in \mathbf{Z}} G_n)$ *là đầy đủ*.

(c) *Mọi dãy Cauchy trong $G$ đều hội tụ*.

*Nếu $G$ giao hoán và được viết theo phép cộng, thì các điều kiện này cũng tương đương với điều kiện sau:*

(d) *Mọi họ* $(x_\lambda)_{\lambda \in L}$ *các phần tử của $G'$ hội tụ về 0 đối với lọc $\mathcal{F}$ gồm các phần bù của các tập con hữu hạn của $L$ thì đều khả tổng trong $G'$*.

Để một lọc trên $G$ là một lọc Cauchy (tương ứng, một lọc hội tụ), điều kiện cần và đủ là ảnh của nó qua ánh xạ chính tắc $G \to G'$ là một lọc Cauchy (tương ứng, một lọc hội tụ) (*Tôpô Đại cương*, Chương II, § 3, no. 1, Mệnh đề 4); do đó trước hết suy ra sự tương đương của (a) và (b); mặt khác, vì $G'$ là mêtric hóa được, sự tương đương của (b) và (c) suy ra từ Mệnh đề 9 của *Tôpô Đại cương*, Chương IX, § 2, no. 6.

Bây giờ giả sử rằng $G$ giao hoán. Giả sử rằng $G'$ đầy đủ và $(x_\lambda)_{\lambda \in L}$ là một họ các phần tử của $G'$ hội tụ về 0 đối với $\mathcal{F}$. Với mọi lân cận $V'$ của 0 trong $G$ là một nhóm con của $G'$, tồn tại một tập con hữu hạn $J$ của $L$ sao cho điều kiện $\lambda \in L - J$ kéo theo $x_\lambda \in V'$; khi đó $\sum_{\lambda \in H} x_\lambda \in V'$ với mọi tập con hữu hạn $H$ của $L$ không giao với $J$, điều này chỉ ra rằng họ $(x_\lambda)_{\lambda \in L}$ là khả tổng (*Tôpô Đại cương*, Chương III, § 5, no. 2, Định lý 1).

Ngược lại, giả sử điều kiện (d) đúng và $(x_n)$ là một dãy Cauchy trên $G'$; khi đó họ $(x_{n+1} - x_n)$ là khả tổng và đặc biệt chuỗi có số hạng tổng quát $x_{n+1} - x_n$ là hội tụ và do đó dãy $(x_n)$ là hội tụ.

Cho $G$ là một nhóm lọc mà bộ lọc $(G_r)$ gồm các nhóm con chuẩn tắc của $G$; các nhóm thương $G/G_n$ là *rời rạc* và do đó đầy đủ, vì các $G_r$ là mở trong $G$. Gọi $f_n$ là ánh xạ chính tắc $G \to G/G_n$ và với $m \leq n$ gọi $f_{mn}$ là ánh xạ chính tắc $G/G_n \to G/G_m$; $(G/G_n, f_{mn})$ là một hệ ngược các nhóm rời rạc với $\mathbf{Z}$ làm tập hợp chỉ số (*General Topology*, Chapter III, § 7, no. 3). Gọi $\tilde{G}$ là nhóm tôpô là giới hạn ngược của hệ ngược này và với mọi $n$ gọi $g_n : \tilde{G} \to G/G_n$ là ánh xạ chính tắc; gọi $f : G \to \tilde{G}$ là giới hạn ngược của hệ ngược các ánh xạ $(f_n)$ sao cho $f_n = g_n \circ f$ với mọi $n$; sau cùng, gọi $j$ là ánh xạ chính tắc của $G$ vào hoàn thành Hausdorff $\hat{G}$ của nó; vì các $G/G_n$ là đầy đủ, tồn tại một đẳng cấu nhóm tôpô duy nhất $i : \hat{G} \to \tilde{G}$ sao cho $f = i \circ j$ (*loc. cit.*, Hệ quả 1 của Mệnh đề 2); ta sẽ gọi nó là đẳng cấu *chính tắc* từ $\hat{G}$ lên $\tilde{G}$.

Cho $H$ là một nhóm lọc khác mà bộ lọc $(H_r)$ gồm các nhóm con chuẩn tắc của $H$ và gọi $u : G \to H$ là một đồng cấu tương thích với các bộ lọc (no. 4). Đặt $\tilde{H} = \lim H/H_n$; với mọi $n$, $u$ xác định bằng cách chuyển sang thương một đồng cấu $u_n : G/G_n \to H/H_n$ và hiển nhiên các $u_n$ tạo thành một hệ ngược các ánh xạ; đặt $\tilde{u} = \lim u_n$. Hơn nữa, gọi $\hat{H}$ là hoàn thành Hausdorff của $H$ và $ti : \hat{G} \to H$ là đồng cấu dẫn xuất từ $u$ bằng cách chuyển qua các hoàn thành Hausdorff (*General Topology*, Chapter II, § 3, no. 7, Proposition 15). Từ các định nghĩa suy ra ngay lập tức rằng nếu đồng nhất $\hat{G}$ với $\tilde{G}$ và $\hat{H}$ với $\tilde{H}$ bằng các đẳng cấu chính tắc, thì $ti$ được đồng nhất với $\tilde{u}$. Đặc biệt, ta kết luận rằng nếu, với mọi $n$, $u_n$ là một đẳng cấu, thì $ti$ là một đẳng cấu các nhóm tôpô.

*Các ví dụ về nhóm lọc và vành lọc đầy đủ*

#### Ví dụ 1 {#ac-iii-s2-n6-exa-1 .statement}

Cho $G$ là một nhóm lọc đầy đủ. Mọi nhóm con *đóng* của $G$, với bộ lọc cảm sinh, đều đầy đủ (*General Topology*, Chapter II, § 3, no. 4, Proposition 8). Mọi nhóm thương của $G$, với bộ lọc thương, đều đầy đủ (*General Topology*, Chapter IX, § 3, no. 1, *Remark* 1).

#### Ví dụ 2 {#ac-iii-s2-n6-exa-2 .statement}

Cho $A$ là một vành giao hoán được lọc mà bộ lọc của nó được ký hiệu bởi $(a_n)_{n \in \mathbf{Z}}$; gọi $A'$ là vành các chuỗi lũy thừa hình thức $A[[X_1, \ldots, X_s]]$. Với mọi $e = (e_1, \ldots, e_s) \in \mathbf{N}^s$, ta đặt $|e| = \sum_{i=1}^s e_i$, $X^e = \prod_{i=1}^s X_i^{e_i}$ sao cho mọi phần tử $P \in A'$ đều có thể được viết một cách duy nhất dưới dạng $P = \sum_{e \in \mathbf{N}^s} \alpha_{e,P} X^e$ trong đó $\alpha_{e,P} \in A$. Với mọi $n \in \mathbf{Z}$, gọi $a'_n$ là tập hợp các $P \in A'$ sao cho $\alpha_{e,P} \in a_{n-|e|}$ với mọi $e \in \mathbf{N}^s$; ta chứng minh rằng $a'_n$ là một *iđêan* của $A'$. Rõ ràng $a'_n$ là một nhóm con cộng tính của $A'$; mặt khác, nếu $P \in a'_n$ và $Q \in A'$, thì, với mọi $e \in \mathbf{N}^s$, $\alpha_{e,PQ} = \sum_{e'+e''=e} \alpha_{e',Q}\alpha_{e'',P}$; vì quan hệ $e' + e'' = e$ kéo theo $|e''| \leq |e|$, suy ra $PQ \in a'_n$. Hơn nữa, nếu $Q \in a'_m$, thì, với $e' + e'' = e$, $\alpha_{e',Q}\alpha_{e'',P} \in a_{m-|e'|}a_{n-|e''|} \subset a_{m+n-|e|}$, điều đó chứng tỏ rằng $(a'_n)_{n \in \mathbf{Z}}$ là một *bộ lọc* tương thích với cấu trúc vành trên $A'$ (vì hiển nhiên $1 \in a'_0$). Về sau, khi nói đến $A'$ như một vành được lọc, ta sẽ hiểu, trừ khi có nói rõ ngược lại, là với bộ lọc (ah). Rõ ràng $\bigcap_{n \in \mathbf{Z}} a'_n$ là tập hợp các chuỗi lũy thừa hình thức mà mọi hệ số của chúng đều thuộc $\bigcap_{n \in \mathbf{Z}} a_n$; do đó, nếu $A$ là Hausdorff thì $A'$ cũng vậy. Nếu $a_0 = A$, thì $a'_0 = A'$.

#### Mệnh đề 6 {#ac-iii-s2-prop-6 .statement}

*Với các ký hiệu trên, giả sử rằng $a_0 = A$ và gọi $h$ là ánh xạ $P \mapsto (\alpha_{e,P})_{e \in \mathbf{N}^s}$. Khi đó $h$ là một đẳng cấu của nhóm tôpô cộng tính $A$ lên nhóm tôpô cộng tính $A^{\mathbf{N}^s}$. Vành đa thức $A[X_1, \ldots, X_s]$ là trù mật trong $A'$; nếu $A$ là đầy đủ, thì $A'$ cũng vậy.*

Rõ ràng $h$ là song ánh; $V_n = h(a'_n)$ là tập hợp các $(a_e) \in A^{\mathbf{N}^s}$ sao cho $a_e \in a_{n-|e|}$ với mọi $e \in \mathbf{N}^s$ sao cho $|e| \leq n$; vì các phần tử $e$ này có số lượng hữu hạn, $V_n$ là một lân cận của 0 trong $A^{\mathbf{N}^s}$. Ngược lại, nếu $V$ là một lân cận của 0 trong $A^{\mathbf{N}^s}$, thì tồn tại một tập con hữu hạn $E$ của $\mathbf{N}^s$ và một số nguyên $v$ sao cho các điều kiện $a_e \in a_v$ với mọi $e \in E$ kéo theo $(a_e) \in V$; khi đó nếu $n$ là lớn nhất trong các số nguyên $v + |e|$ với $e \in E$, thì $h(a'_n) \subset V$, điều này chứng minh khẳng định đầu tiên của Mệnh đề 6.

Hơn nữa, với $n$ và $E$ được xác định như trên, $h(P - \sum_{e \in E} \alpha_{e,P}X^e) \in V$ với mọi $P \in A'$, điều này chỉ ra rằng $A[X_1, \ldots, X_s]$ là trù mật trong $A'$. Khẳng định cuối cùng suy ra từ khẳng định đầu tiên và sự kiện rằng một tích của các không gian đầy đủ là đầy đủ.

Cho $m$ là một iđêan của $A$ và giả sử rằng $(a_i)$ là lọc $m$-adic; khi đó, nếu $n$ là iđêan của $A'$ sinh bởi $m$ và các $X_i$ ($1 \leq i \leq s$), thì lọc $(a_i)$ là lọc $n$-adic. Vì rõ ràng, với mọi $k \geq 0$, $n^k$ được sinh bởi các phần tử $aX^e$ sao cho $a \in m^{k-|e|}$ với mọi $e \in \mathbf{N}^s$ sao cho $|e| \leq k$, do đó $n^k \subset a \&$. Ta hãy chứng minh ngược lại rằng $a'_k \subset n^k$. Với mọi $P \in a'_k$, $P = P' + P''$, trong đó $P' = \sum_{|e| < k} \alpha_{e,P}X^e$, $P'' = \sum_{|e| \geq k} \alpha_{e,P}X^e$. Rõ ràng có thể viết $P'' = \sum_{|e|=k} X^e Q_e$, trong đó các $Q_e$ là các phần tử của $A'$, do đó $P'' \in n^k$; mặt khác, rõ ràng $\alpha_{e,P}X^e \in n^k$ với mọi $e \in \mathbf{N}^s$, do đó $P' \in n^k$. Vậy $n^k = a'_k$.

#### Hệ quả {#ac-iii-s2-n6-cor-1 .statement}

*Cho $A$ là một vành giao hoán,

$$
A' = A[[X_1, \ldots, X_s]]
$$

*vành chuỗi lũy thừa hình thức theo $s$ phần tử bất định trên $A$ và $n$ là iđêan của $A'$ gồm các chuỗi lũy thừa hình thức không có số hạng hằng. Vành $A'$ là Hausdorff và đầy đủ* với tôpô n-adic và vành đa thức $A[X_1, \ldots, X_s]$ là trù mật khắp nơi trong $A'$.

Chỉ cần áp dụng điều vừa nói cho trường hợp $m = \{0\}$.

### 7. CÁC TÍNH CHẤT GỌN TUYẾN TÍNH CỦA CÁC MÔĐUN LỌC ĐẦY ĐỦ

Nhắc lại rằng, nếu E là một A-môđun, một tập con afin (hay một đa tạp tuyến tính afin) của E là bất kỳ tập con F nào rỗng hoặc có dạng $a + M$, trong đó $a \in E$ và M là một môđun con của E được gọi là phương của F (Đại số, Chương II, § 9, số 1 và 3).

#### Mệnh đề 7 {#ac-iii-s2-prop-7 .statement}

Cho A là một vành được lọc, E là một A-môđun được lọc và $(E_n)$ là phép lọc của E; giả sử rằng $E_0 = E$, rằng các $E_n$ là các môđun con của E, rằng các A-môđun $E/E_n$ là Artin và cuối cùng rằng nhóm tôpô E là Hausdorff và đầy đủ. Khi đó giao của một dãy giảm các tập con afin đóng khác rỗng của E là khác rỗng.

Ta đã thấy ở no. 6 rằng, vì E là Hausdorff và đầy đủ, nó được đồng nhất với $\tilde{E} = \lim_{\leftarrow} E/E_n$. Cho $(W_p)$ là một dãy giảm các tập con afin đóng khác rỗng của E và, với mọi $n \geq 0$, cho $W_{p,n}$ là ảnh chính tắc của $W_p$ trong $E/E_n$; ta sẽ xây dựng một dãy $x = (x_n) \in \tilde{E}$ sao cho $x_n \in W_{p,n}$ với mọi $p$ và mọi $n$; do đó $x \in W_p + E_n$ với mọi $p$ và mọi $n$ và, vì các $W_p$ là đóng, $x \in W_p$ với mọi $p$ (no. 5), điều này sẽ chứng minh mệnh đề.

Vì $E/E_0 = 0$, ta sẽ lấy $x_0 = 0$. Giả sử rằng các $x_i$ đã được xác định với $0 \leq i \leq n - 1$ và cho $W'_{p,n}$ là tập hợp các phần tử của $W_{p,n}$ mà ảnh chính tắc của chúng trong $E/E_{n-1}$ là $x_{n-1}$; vì $x_{n-1} \in W_{p,n-1}$ và $W_{p,n-1}$ là ảnh chính tắc của $W_{p,n}$, $W'_{p,n}$ là khác rỗng và hiển nhiên là một tập con afin của $E/E_n$; hơn nữa dãy $(W'_{p,n})_{p \in \mathbf{N}}$ là giảm. Vì $E/E_n$ là Artin, dãy này là dừng (nếu không thì dãy các môđun con của $E/E_n$ là các phương của các $W'_{p,n}$ sẽ giảm nghiêm ngặt, điều này là vô lý). Khi đó chỉ cần lấy $x_n$ là một phần tử của $\bigcap_{p \in \mathbf{N}} W'_{p,n}$ và phép dựng của $(x_n)$ khi đó có thể được thực hiện bằng quy nạp.

#### Mệnh đề 8 {#ac-iii-s2-prop-8 .statement}

Giả sử rằng A và E thỏa mãn các giả thiết của Mệnh đề 7. Cho $(F_p)$ là một dãy giảm các môđun con đóng của E sao cho $\bigcap F_p = 0$. Khi đó, với mọi lân cận V của 0 trong E, tồn tại $p$ sao cho $F_p \subset V$ (nói cách khác, cơ sở của bộ lọc $(F_p)$ hội tụ về 0).

Ta có thể giả sử rằng V là một trong các $E_n$, khi đó $E/V$ là Artin. Hãy viết $F'_p = (F_p + V)/V$; vì các $F'_p$ tạo thành một dãy giảm các môđun con của $E/V$, nên tồn tại một số nguyên $j$ sao cho $F'_p = F'_j$ với mọi $p > j$. Ta sẽ thấy rằng $F'_j = \{0\}$, điều này sẽ hoàn tất chứng minh. Lấy $x \in F'_j$ và gọi W, là tập hợp các phần tử của F, mà ảnh của chúng trong $E/V$ là $x$ ($p \geq j$); theo định nghĩa của j, các W, là những tập con afin đóng không rỗng của E và hiển nhiên $W_{p+1} \subset W$;

khi đó suy ra từ Mệnh đề 7 rằng tồn tại một phần tử y thuộc tất cả các W,. Vì W, $\subset F,$ và $\bigcap_{p \in \mathbf{N}} F_p = \{0\}, y = 0$; do x là ảnh chính tắc của y trong E/V, nên $x = 0$ (xem Bài tập 15 đến 21).

### 8. SỰ NÂNG CỦA CÁC ĐỒNG CẤU CỦA CÁC MÔĐUN PHÂN BẬC LIÊN KẾT

#### Định lý 1 {#ac-iii-s2-thm-1 .statement}

Cho X, Y là hai nhóm lọc mà các lọc của chúng $(X_n), (Y_n)$ gồm các nhóm con chuẩn tắc; gọi $u : X \to Y$ là một đồng cấu tương thích với các lọc.

(i) Giả sử rằng lọc $(X_n)$ là đầy đủ. Để $\mathrm{gr}(u)$ là đơn ánh, điều kiện cần và đủ là $\bar{u}^{-1}(Y_n) = X_n$ với mọi $n \in \mathbf{Z}$.

(ii) Giả sử rằng một trong các giả thiết sau được thỏa mãn: (α) X đầy đủ và Y Hausdorff; (β) Y rời rạc. Khi đó, để $\mathrm{gr}(u)$ là toàn ánh, điều kiện cần và đủ là $Y_n = u(X_n)$ với mọi $n \in \mathbf{Z}$.

(i) Nói rằng ánh xạ $\mathrm{gr}_n(u)$ là đơn ánh có nghĩa là
$$
X_n \cap \bar{u}^{-1}(Y_{n+1}) \subset X_{n+1}.
$$
Điều này hiển nhiên đúng nếu $(Y_{n+1}) = X_{n+1}$. Ngược lại, nếu
$$
X_n \cap \bar{u}^{-1}(Y_{n+1}) \subset X_{n+1}
$$
với mọi $n$, ta suy ra bằng quy nạp theo $k$ rằng $X_{n-k} \cap \bar{u}^{-1}(Y_{n+1}) \subset X_{n+1}$ với mọi $n \in \mathbf{Z}$ và mọi $k \geq 0$. Vì lọc $(X_n)$ là đầy đủ, ta thấy rằng, với mọi $n$, $X_n$ là hợp của các $X_{n-k}$ ($k \geq 0$), do đó $\bar{u}^{-1}(Y_{n+1}) \subset X_{n+1}$ với mọi $n$ và vì thế $X_{n+1} \subset \bar{u}^{-1}(Y_{n+1})$, điều này hoàn tất chứng minh.

(ii) Nói rằng ánh xạ $\mathrm{gr}_n(u)$ là toàn ánh có nghĩa là
$$
Y_n = u(X_n)Y_{n+1}.
$$
Điều này hiển nhiên đúng nếu $Y_n = u(X_n)Y_{n+1}$ với mọi $n \in \mathbf{Z}$. Cho $n$ là một số nguyên và $y$ là một phần tử của $Y_n$; ta sẽ định nghĩa một dãy $(x_k)_{k \geq 0}$ các phần tử của $X_n$ sao cho $x_k \in X_n$, $x_{k+1} \equiv x_k \pmod{X_{n+k}}$ và $u(x_k) \equiv y \pmod{Y_{n+k}}$ với mọi $k \geq 0$. Ta lấy $x_0$ bằng phần tử đơn vị của X, điều này chắc chắn cho $u(x_0) \equiv y \pmod{Y_n}$. Giả sử đã xây dựng được một $x_k \in X_n$ sao cho $u(x_k) \equiv y \pmod{Y_{n+k}}$; khi đó $(u(x_k))^{-1}y \in Y_{n+k}$; giả thiết kéo theo rằng tồn tại $t \in X_{n+k}$ sao cho $u(t) \equiv (u(x_k))^{-1}y \pmod{Y_{n+k+1}}$ và do đó $u(x_k t) \equiv y \pmod{Y_{n+k+1}}$; chỉ cần lấy $x_{k+1} = x_k t$ để thực hiện bước quy nạp. Như vậy, nếu Y là rời rạc, thì tồn tại $k \geq 0$ sao cho $Y_{n+k} = \{e'\}$ (phần tử đơn vị của Y), do đó $u(x_k) = y$ và vì thế trong trường hợp này đã chứng minh được rằng $u(X_n) = Y$, với mọi $n$. Bây giờ giả sử X là đầy đủ và Y Hausdorff. Vì $x_h^{-1} x_k \in X_{n+k}$ với $h \geq k \geq 0$, $(x_k)$ là một dãy Cauchy trong $X_n$; vì

$X_n$ đóng trong X và do đó đầy đủ, dãy này có ít nhất một giới hạn x trong $X_n$. Nhờ tính liên tục của u, $u(x)$ là giới hạn duy nhất của dãy (u(x_k)) trong Y, vì Y là Hausdorff. Nhưng các hệ thức u(x_k) \equiv y (\text{mod. } Y_{n+k+1}) cho thấy rằng y cũng là một giới hạn của dãy này, do đó $u(x) = y$ và cũng đã chứng minh được rằng $u(X_n) = Y_n$.

#### Hệ quả 1 {#ac-iii-s2-thm-1-cor-1 .statement}

*Giả sử rằng X là Hausdorff và bộ lọc của nó là vét cạn. Khi đó, nếu gr(u) là đơn ánh, thì u là đơn ánh.*

Gọi e, e' lần lượt là các phần tử đơn vị của X và Y. Khi đó
$$
\bar{u}^{-1}(e') \subset \bigcap_n \bar{u}^{-1}(Y_n) = \bigcap_n X_n = \{e\}
$$
theo giả thiết, do đó hệ quả được chứng minh.

#### Hệ quả 2 {#ac-iii-s2-thm-1-cor-2 .statement}

*Giả sử rằng một trong các giả thiết sau được thỏa mãn :*
$(\alpha)$ *X là đầy đủ, Y là Hausdorff và bộ lọc của nó là vét cạn;*
$(\beta)$ *Y là rời rạc và bộ lọc của nó là vét cạn.*
*Khi đó, nếu gr(u) là toàn ánh, thì u là toàn ánh.*

Trong trường hợp này $Y = \bigcup_n Y_n = \bigcup_n u(X_n) \subset u(X)$.

#### Hệ quả 3 {#ac-iii-s2-thm-1-cor-3 .statement}

*Giả sử rằng X và Y là Hausdorff, các bộ lọc của X và Y đều vét cạn và X đầy đủ. Khi đó, nếu gr(u) là song ánh, thì u là song ánh.*

Cho A là một vành địa phương, m iđêan cực đại của nó và M một A-môđun; trang bị cho A và M các bộ lọc *m-adic* và gọi gr(A) và gr(M) là vành phân bậc và gr(A)-môđun phân bậc liên kết với A và M. Ta đã thấy (no. 3, Ví dụ 3) rằng ánh xạ chính tắc (11) luôn luôn *toàn ánh*; ta sẽ xét tính chất sau của M:
*(GR)* *Ánh xạ chính tắc*
$$
\gamma_M : \operatorname{gr}(A) \otimes_{\operatorname{gr}_0(A)} \operatorname{gr}_0(M) \to \operatorname{gr}(M)
$$
*là song ánh*.

#### Mệnh đề 9 {#ac-iii-s2-prop-9 .statement}

*Cho A là một vành địa phương, m iđêan cực đại của nó, M, N là hai A-môđun và u : N \to M một A-đồng cấu. Trang bị cho M và N các bộ lọc m-adic và giả sử rằng: (1) M thỏa mãn tính chất (GR); (2) \operatorname{gr}_0(u) : \operatorname{gr}_0(N) \to \operatorname{gr}_0(M) là đơn ánh. Khi đó \operatorname{gr}(u) : \operatorname{gr}(N) \to \operatorname{gr}(M) là đơn ánh, N và P = \operatorname{Coker}(u) thỏa mãn tính chất (GR) và $m^n N = \bar{u}^{-1}(m^n M)$ với mọi số nguyên $n > 0$.*

Ngay lập tức kiểm tra được rằng biểu đồ
$$
\begin{array}{ccc}
\operatorname{gr}(A) \otimes_{\operatorname{gr}_0(A)} \operatorname{gr}_0(N) & \xrightarrow{1 \otimes \operatorname{gr}_0(u)} & \operatorname{gr}(A) \otimes_{\operatorname{gr}_0(A)} \operatorname{gr}_0(M) \\
\downarrow \gamma_N & & \downarrow \gamma_M \\
\operatorname{gr}(N) & \xrightarrow{\operatorname{gr}(u)} & \operatorname{gr}(M)
\end{array}
$$

là giao hoán. Vì $\mathrm{gr}_0(A) = A/m$ là một trường, giả thiết kéo theo rằng $1 \otimes \mathrm{gr}_0(u)$ là đơn ánh; vì theo giả thiết $\gamma_M$ là đơn ánh, nên $\gamma_M \circ (1 \otimes \mathrm{gr}_0(u))$ cũng vậy. Trước hết điều này kéo theo rằng $\gamma_N$ là đơn ánh và do đó là song ánh và vì thế $\mathrm{gr}(u)$ là đơn ánh. Công thức $\tilde{u}^1(m^nM) = m^nN$ khi đó là một hệ quả của Định lý 1 (i).

Mặt khác, đặt $N' = u(N)$ và gọi $j : N' \to M$ là đơn ánh chính tắc. Nếu $p : M \to P = M/N'$ là đồng cấu chính tắc, thì trong biểu đồ giao hoán

$$
\begin{array}{ccccccccc}
\mathrm{gr}(A) \otimes \mathrm{gr}_0(N') & \xrightarrow{1 \otimes \mathrm{gr}_0(j)} & \mathrm{gr}(A) \otimes \mathrm{gr}_0(M) & \xrightarrow{1 \otimes \mathrm{gr}_0(p)} & \mathrm{gr}(A) \otimes \mathrm{gr}_0(P) & \to & 0 \\
\downarrow \gamma_{N'} & & \downarrow \gamma_M & & \downarrow \gamma_P & & \\
\mathrm{gr}(N') & \xrightarrow{\mathrm{gr}(j)} & \mathrm{gr}(M) & \xrightarrow{\mathrm{gr}(p)} & \mathrm{gr}(P) & \to & 0
\end{array}
$$

hàng dưới là khớp (no. 4, Mệnh đề 2) và hàng trên cũng vậy theo Mệnh đề 2 của no. 4 và thực tế rằng $\mathrm{gr}_0(A)$ là một trường. Hơn nữa, $\mathrm{gr}(j)$ là đơn ánh (no. 4, Mệnh đề 2) và do đó $\mathrm{gr}_0(j)$ là đơn ánh. Phần đầu của lập luận áp dụng cho $j$ cho thấy rằng $\gamma_{N'}$ là song ánh; vì $\gamma_M$ cũng song ánh theo giả thiết, ta kết luận rằng $\gamma_P$ là song ánh (Chương I, § 1, no. 4, Hệ quả 2 của Mệnh đề 2).

#### Hệ quả {#ac-iii-s2-n8-cor-1 .statement}

Dưới các giả thiết của Mệnh đề 9, nếu ta còn giả sử rằng $N$ là Hausdorff đối với lọc $m$-adic, thì $u$ là đơn ánh.

Điều này suy ra từ việc $\mathrm{gr}(u)$ là đơn ánh (Hệ quả 1 của Định lý 1).

\* Nhận xét. Giả sử rằng các giả thiết của Mệnh đề 9 được thỏa mãn và thêm nữa có một trong các điều kiện sau:
(1) $m$ là lũy linh;
(2) $A$ là Noether và $P$ là Hausdorff iđêan (x. § 5, no. 1);
khi đó $P$ là một $A$-môđun phẳng. Điều này suy ra từ việc $\gamma_P$ là song ánh và § 5, no. 2, Định lý 1 (iv), vì $A/m$ là một trường. \*

### 9. PHÉP NÂNG CÁC HỌ PHẦN TỬ CỦA MỘT MÔĐUN PHÂN BẬC LIÊN KẾT

Cho $A$ là một vành giao hoán có lọc, $(A_n)_{n \in \mathbf{Z}}$ là lọc của nó và $C$ là một vành con của $A$, sao cho $C \cap A_1 = \{0\}$. Hạn chế lên $C$ của ánh xạ chính tắc $A_0 \to A_0/A_1 = \mathrm{gr}_0(A)$ khi đó là đơn ánh, điều này cho phép ta đồng nhất $C$ với một môđun con của $\mathrm{gr}_0(A)$; đây là điều mà ta thường sẽ làm trong các trường hợp tương tự. Nếu $A_1 \neq A$, và $K$ là một trường con bất kỳ của $A$, thì $K \cap A_1 = (0)$ vì $K \cap A_1$ là một iđêan của $K$ không chứa 1; khi đó $K$ có thể được đồng nhất với một trường con của $\mathrm{gr}_0(A)$.

#### Mệnh đề 10 {#ac-iii-s2-prop-10 .statement}

Cho $A$ là một vành giao hoán có lọc và $(A_n)$ là lọc của nó; giả sử rằng tồn tại một vành con $C$ của $A_0$ sao cho $C \cap A_n = \{0\}$ và $C$ được đồng nhất với một vành con của $\mathrm{gr}_0(A)$. Cho $(x_i)_{1 \leq i \leq q}$ là một họ hữu hạn các phần tử của $A$; giả sử rằng $x_i \in A_n$, với $1 \leq i \leq q$ và gọi $\xi_i$ là lớp của $x_i$ trong $\mathrm{gr}_{n_i}(A)$ với $1 \leq i \leq q$.

(i) Nếu họ $(\xi_i)$ các phần tử của $\mathrm{gr}(A)$ là đại số tự do trên $C$, thì họ $(x_i)$ là đại số tự do trên $C$.

(ii) Nếu lọc trên $A$ là đầy đủ và rời rạc và $(\xi_i)$ là một hệ sinh của $C$-đại số $\mathrm{gr}(A)$, thì $(x_i)$ là một hệ sinh của $C$-đại số $A$.

Cho $A'$ là đại số đa thức $\mathbf{C}[X_1, \ldots, X_q]$ trên $\mathbf{C}$; cho $A'$ được trang bị phân bậc $(A'_n)$ kiểu $\mathbf{Z}$ trong đó $A_n$ là tập hợp các tổ hợp tuyến tính trên $\mathbf{C}$ của các đơn thức $X_1^{s(1)} \ldots X_q^{s(q)}$ sao cho $\sum_{i=1}^q n_i s(i) = n$. Gọi $u$ là đồng cấu $f \mapsto f(x_1, \ldots, x_q)$ từ $\mathbf{C}$-đại số $A'$ vào $\mathbf{C}$-đại số $A$; theo định nghĩa, $u(A'_n) \subset A_n$ với mọi $n \in \mathbf{Z}$ và do đó $u$ tương thích với các bộ lọc khi $(A')$ được trang bị cấu trúc vành lọc liên kết với cấu trúc vành phân bậc của nó, x. no. 1, Ví dụ 1). Do đó, giả thiết của (i) có nghĩa là

$$
\mathrm{gr}(u): A' = \mathrm{gr}(A') \to \mathrm{gr}(A)
$$

là đơn ánh; vì bộ lọc trên $A'$ là đầy đủ và tách biệt, có thể áp dụng Hệ quả 1 của Định lý 1 ở no. 8 và $u$ là đơn ánh, điều đó chứng minh kết luận của (i). Tương tự, giả thiết (ii) trên (\&) có nghĩa là $\mathrm{gr}(u)$ là toàn ánh; vì $A$ là rời rạc và bộ lọc của nó là đầy đủ, có thể áp dụng Hệ quả 2 của Định lý 1 ở no. 8 và $u$ là toàn ánh, điều đó chứng minh kết luận của (ii).

#### Mệnh đề 11 {#ac-iii-s2-prop-11 .statement}

Cho $A$ là một vành giao hoán lọc đầy đủ Hausdorff, $C$ một vành con của $A_0$ sao cho $C \cap A_n = 0$ và $(x_i)_{1 \leq i \leq q}$ một họ hữu hạn các phần tử của $A$ sao cho $x_i \in A_{n_i}$ với $n_i > 0$ đối với $1 \leq i \leq q$; gọi $\xi_i$ là lớp của $x_i$ trong $\mathrm{gr}_{n_i}(A)$ đối với $1 \leq i \leq q$.

(i) Tồn tại một $C$-đồng cấu duy nhất $v$ từ đại số chuỗi lũy thừa hình thức $A'' = \mathbf{C}[[X_1, \ldots, X_q]]$ vào $A$ sao cho $v(X_i) = x_i$ đối với $1 \leq i \leq q$.

(ii) Nếu họ $(\xi_i)$ tự do đại số trên $C$, đồng cấu $v$ là đơn ánh.

(iii) Nếu bộ lọc trên $A$ là đầy đủ và họ $(\xi_i)$ là một hệ sinh của $C$-đại số $\mathrm{gr}(A)$, đồng cấu $v$ là toàn ánh.

Vì $n_i \geq 1$ với mọi $i$, nên $\sum_{i=1}^q n_i s(i) \geq \sum_{i=1}^q s(i)$ đối với mọi đơn thức $X_1^{s(1)} \ldots X_q^{s(q)}$, và mặt khác $\sum_{i=1}^q n_i s(i) \leq r \cdot \sum_{i=1}^q s(i)$ nếu $r$ là số lớn nhất trong các $n_i$. Nếu $A''_n$ ký hiệu tập hợp các chuỗi lũy thừa hình thức mà các hạng khác không $a_s X_1^{s(1)} \ldots X_q^{s(q)}$ của chúng thỏa mãn $\sum_{i=1}^q n_i s(i) \geq n$, thì từ no. 6, Hệ quả của Mệnh đề 6, suy ra rằng $A''$ là Hausdorff và đầy đủ đối với lọc cạn $(A''_n)$, và rằng

$$
A' = \mathbf{C}[X_1, \ldots, X_q]
$$

là trù mật trong $A''$; hơn nữa, đồng cấu $u$ được xác định trong chứng minh của Mệnh đề 10 là liên tục trên $A'$ và có thể được mở rộng duy nhất thành một đồng cấu liên tục $v : A \to A$, vì $A$ là Hausdorff và đầy đủ (General Topology, Chapter III, § 3, no. 3, Proposition 5), điều này chứng minh (i); đồng thời, $\mathrm{gr}(A'') = \mathrm{gr}(A')$ và $\mathrm{gr}(v) = \mathrm{gr}(u)$; khi đó (ii) và (iii) suy ra tương ứng từ các Hệ quả 1 và 2 của Định lý 1 ở no. 8, theo các giả thiết trên $A$.

Kết luận của (ii) (tương ứng, của (iii)) của mệnh đề đôi khi được diễn đạt bằng cách nói rằng họ $(x_i)$ là tự do hình thức trên $C$ (tương ứng, một hệ sinh hình thức của $A$).

#### Mệnh đề 12 {#ac-iii-s2-prop-12 .statement}

Cho $A$ là một vành được lọc, $E$ một $A$-môđun được lọc, và $(A_n)$ và $(E_n)$ là các lọc tương ứng trên $A$ và $E$. Giả sử rằng $A$ là đầy đủ và lọc $(E_n)$ là cạn và phân ly. Cho $(x_i)_{i \in I}$ là một họ hữu hạn các phần tử của $E$, và với mỗi $i \in I$ cho $n(i)$ là một số nguyên sao cho $x_i \in E_{n(i)}$; sau cùng, cho $\xi_i$ là lớp của $x_i$ trong $\mathrm{gr}_{n(i)}(E)$. Khi đó, nếu $(\xi_i)$ là một hệ sinh của $\mathrm{gr}(A)$-môđun $\mathrm{gr}(E)$, thì $(x_i)$ là một hệ sinh của $A$-môđun $E$.

Trong $A$-môđun $L = A'$, ký hiệu $L_0$ là tập hợp các $(a_i)$ sao cho $a_i \in A_{n - n(i)}$ với mọi $i \in I$; nếu $p$ và $q$ là giá trị nhỏ nhất và lớn nhất của các $n(i)$, thì $A^I_{n-q} \supset L_0 \supset A^I_{n-p}$ và tôpô xác định trên $L$ bởi định nghĩa $(L_n)$ là cùng một tôpô với tôpô tích; do đó $L$ là một $A$-môđun lọc đầy đủ. Vì $L$ là tự do, tồn tại một ánh xạ $A$-tuyến tính $u : L \to E$ sao cho $u((a_i)) = \sum_{i \in I} a_i x_i$ và hiển nhiên nó tương thích với các lọc; phải chứng minh rằng $u$ là toàn ánh và để làm việc đó, theo Hệ quả 2 của Định lý 1, no. 8, chỉ cần chỉ ra rằng

$$
\mathrm{gr}(u) : \mathrm{gr}(L) \to \mathrm{gr}(E)
$$

là toàn ánh, hay cũng có nghĩa là, với mọi $x \in E_n$, tồn tại một họ $(a_i)$ sao cho $a_i \in A_{n-n(i)}$ với mọi $i \in I$ và $x \equiv \sum_{i \in I} a_i x_i \pmod{E_{n+1}}$. Gọi $\xi$ là lớp của $x$ trong $\mathrm{gr}_n(E)$; vì các $\xi_i$ sinh $\mathrm{gr}(A)$-môđun $\mathrm{gr}(E)$, tồn tại các $\alpha_i \in \mathrm{gr}(A)$ sao cho $\xi = \sum_{i \in I} \alpha_i \xi_i$ và ta có thể giả sử rằng $\alpha_i \in \mathrm{gr}_{n-n(i)}(A)$ bằng cách thay thế, nếu cần, $\alpha_i$ bởi thành phần thuần nhất bậc $n - n(i)$ của nó. Khi đó $\alpha_i$ là ảnh của một phần tử $a_i \in A_{n-n(i)}$ và họ $(a_i)$ có tính chất cần thiết.

#### Hệ quả 1 {#ac-iii-s2-prop-12-cor-1 .statement}

Cho $A$ là một vành lọc đầy đủ và $E$ là một $A$-môđun lọc mà lọc của nó là vét cạn và phân cách. Nếu $\mathrm{gr}(E)$ là một $\mathrm{gr}(A)$-môđun sinh hữu hạn (tương ứng Noether), thì $E$ là một $A$-môđun sinh hữu hạn (tương ứng Noether).

Nếu $\mathrm{gr}(E)$ sinh hữu hạn, thì có một hệ hữu hạn các phần tử sinh thuần nhất và Mệnh đề 12 cho thấy rằng $E$ sinh hữu hạn. Bây giờ giả sử rằng $\mathrm{gr}(E)$ là Noether và gọi $F$ là một môđun con của $E$; lọc cảm sinh trên $F$ bởi lọc của $E$ là vét cạn và phân cách, và $\mathrm{gr}(F)$ được đồng nhất với một môđun con gr(A) của gr(E) (no. 4, Mệnh đề 2), do đó theo giả thiết nó sinh hữu hạn; ta kết luận rằng F là một A-môđun hữu hạn sinh và vì thế E là Noether.

#### Hệ quả 2 {#ac-iii-s2-prop-12-cor-2 .statement}

Cho A là một vành lọc Hausdorff đầy đủ mà lọc của nó là vét cạn. Nếu gr(A) là một vành Noether trái, thì A cũng vậy.

Chỉ cần áp dụng Hệ quả 1 với E = A.

#### Hệ quả 3 {#ac-iii-s2-prop-12-cor-3 .statement}

Cho A là một vành lọc đầy đủ, (A,) là lọc của nó, E là một A-môđun lọc Hausdorff, (E_n) là lọc của nó và F là một môđun con sinh hữu hạn của E; giả sử rằng A_∞ = A và E_0 = E.

(i) Nếu, với mọi k ≥ 0, E_k = E_{k+1} + A_k F, thì F = E.
(ii) Nếu giả sử thêm rằng lọc trên E được dẫn xuất từ lọc trên A (no. 1, Ví dụ 2), thì quan hệ E = E_1 + F kéo theo F = E.

Gọi ξ_i (1 ≤ i ≤ n) là các lớp mod. E_1 của một hệ hữu hạn các phần tử sinh của F. Từ giả thiết đã cho suy ra rằng với mọi k ≥ 0, mọi phần tử của gr_k(E) đều có thể viết dưới dạng $\sum_{i=1}^n \alpha_i \xi_i$ trong đó $\alpha_i \in \mathrm{gr}(A)$; do đó các $\xi_i$ sinh gr(A)-môđun gr(E), điều này chứng minh (i) theo Mệnh đề 12. Nếu lọc trên E được dẫn xuất từ lọc trên A, thì quan hệ E = E_1 + F kéo theo

$$
E_k = A_k E = A_k E_1 + A_k F = A_k A_1 E + A_k F \subset A_{k+1} E + A_k F \\
= E_{k+1} + A_k F \subset E_k,
$$

do đó (ii).

#### Mệnh đề 13 {#ac-iii-s2-prop-13 .statement}

Cho A là một vành, m là một iđêan hai phía của A được chứa trong căn Jacobson của A và E là một A-môđun. Cho A và E các lọc m-adic (no. 1, Ví dụ 3). Giả sử rằng một trong các điều kiện sau được thỏa mãn:
(a) E là một A-môđun hữu hạn sinh và A là Hausdorff;
(b) m là lũy linh.

Để E là một A-môđun tự do, điều kiện cần và đủ là E/mE là một (A/m)-môđun tự do và E thỏa mãn tính chất (GR) (no. 8).

Nếu E là một A-môđun tự do và $(e_\lambda)$ là một cơ sở của E, thì $m^k E$ là tổng trực tiếp của các môđun con $m^k e_\lambda$ của E với mọi $k > 0$ (Đại số, Chương II, § 3, no. 7, Nhận xét); khi đó $m^k E / m^{k+1} E$ được đồng nhất với tổng trực tiếp của các $m^k e_\lambda / m^{k+1} e_\lambda$ (Đại số, Chương 11, § 1, no. 6, Mệnh đề 7). Trước hết ta suy ra (với $k = 0$) rằng các lớp $1 \otimes e_\lambda$ của các $e_\lambda$ trong $E / mE = (A / m) \otimes_A E$ lập thành một cơ sở của (A/m)-môđun $E / mE$, vì ánh xạ chính tắc

$$
(m^k / m^{k+1}) \otimes_A (E / mE) \to m^k E / m^{k+1} E
$$

là song ánh với mọi $k \geq 0$; do đó $\gamma_E$ là song ánh. Chú ý rằng phần này của chứng minh không dùng điều kiện (a) cũng không dùng điều kiện (b).

Ngược lại, giả sử các điều kiện của mệnh đề được thỏa mãn và gọi $(x_i)_{i \in I}$ là một họ phần tử của E mà các lớp của chúng mod. $mE$ lập thành một cơ sở của $(A/m)$-môđun $E/mE$; gọi L là A-môđun tự do $A_s^{(I)}$, $(f_i)_{i \in I}$ là cơ sở chính tắc của nó và $u : L \to E$ là ánh xạ A-tuyến tính sao cho $u(f_i) = x_i$ với mọi $i \in I$. Các giả thiết đã kéo theo rằng $u$ là toàn ánh (Chương II, § 3, no. 2, Hệ quả 1 của Mệnh đề 4) và còn lại phải chứng minh rằng $u$ là đơn ánh. Bây giờ, mỗi giả thiết (a) và (b) đều kéo theo rằng A là Hausdorff và vì thế L cũng vậy đối với lọc m-adic, vì $m^kL = (m^k)^{(I)}$ (Đại số, Chương II, § 3, no. 7, Nhận xét) và $\operatorname{gr}(L)$ được đồng nhất với $\operatorname{gr}(A) \otimes_{A/m} (L/mL)$ từ phần đầu của chứng minh; đồng cấu $u$ tương thích với các lọc và có thể viết $\operatorname{gr}(u) = \gamma_E \circ v$ trong đó $v$ là song ánh từ $\operatorname{gr}(L)$ lên
$$
\operatorname{gr}(A) \otimes_{A/m} (E/mE)
$$
ánh xạ lớp off, mod. mM lên $1 \otimes \bar{x}_i$, trong đó $\bar{x}_i$ là lớp của $x_i$ mod. $mE$. Khi đó giả thiết kéo theo rằng $\operatorname{gr}(u)$ là đơn ánh và kết luận suy ra nhờ Hệ quả 1 của Định lý 1, no. 8.

### 10. ÁP DỤNG: CÁC VÍ DỤ VỀ VÀNH NOETHER

#### Bổ đề 1 {#ac-iii-s2-lem-1 .statement}

Cho A là một vành phân bậc kiểu $\mathbf{Z}$, với phân bậc $(A_n)$ sao cho $A_n = 0$ với mọi $n < 0$ hoặc $A_n = 0$ với mọi $n > 0$. Cho M là một A-môđun phân bậc kiểu $\mathbf{Z}$. Để M là một A-môđun Noether, điều kiện cần và đủ là mọi môđun con phân bậc của M đều sinh hữu hạn.

Vì $n \mapsto -n$ là một tự đẳng cấu của nhóm $\mathbf{Z}$, ta có thể chỉ xét trường hợp $A_n = 0$ với mọi $n > 0$. Gọi A' và M' là vành A và môđun M được trang bị các lọc liên kết với các phân bậc tương ứng của chúng (no. 1, Ví dụ 1), các lọc này là đầy đủ và tách biệt; giả thiết trên A kéo theo rằng A' là rời rạc và do đó đầy đủ. Nếu E là một môđun con-A của M, thì A'-môđun có lọc E' nhận được bằng cách trang bị cho E lọc cảm sinh là Hausdorff và lọc của nó là đầy đủ; hơn nữa $\operatorname{gr}(E')$ được đồng nhất với một môđun con phân bậc-A của $M = \operatorname{gr}(M')$ và do đó sinh hữu hạn theo giả thiết. Khi đó kết luận suy ra từ Hệ quả 1 của Mệnh đề 12 ở no. 9.

#### Định lý 2 {#ac-iii-s2-thm-2 .statement}

Cho A là một vành phân bậc kiểu $\mathbf{N}$, M là một A-môđun phân bậc kiểu $\mathbf{N}$ và $(A_n)$ và $(M_n)$ là các phân bậc tương ứng của chúng. Giả sử tồn tại một phần tử $a \in A_0$ sao cho $A_n = A_0 a^n$ và $M_n = a^n M_0$ với mọi $n > 0$. Khi đó, nếu M, là một $A_0$-môđun Noether, thì M là một A-môđun Noether.

Do Bổ đề 1, chỉ cần chứng minh rằng mọi môđun con phân bậc N của M đều sinh hữu hạn. Với mọi $r \geq 0$, đặt $N_r = N \cap M_r$ và gọi $L_r$ là tập các $m \in M_0$ sao cho $a^r m \in N_r$. Vì
$$
a^r A_0 \subset A_r = A_0 a^r, \quad a^r A_0 L_r \subset A_0 a^r L_r \subset A_0 N_r \subset N_r
$$

nên các $L_r$ là các môđun con A_0 của M_0; hơn nữa,

$$
aN_r \subset N \cap aM_r = N \cap M_{r+1} = N_{r+1}
$$

và do đó dãy $(L_r)_{r \geq 0}$ là tăng. Giả thiết cho thấy tồn tại một số nguyên $n \geq 0$ sao cho $L_r = L_n$ với $r \geq n$. Với mỗi $r \leq n$, gọi $(m_{r,s})_{1 \leq s \leq k_r}$ là một hệ sinh của A_0-môđun $L_r$. Ta sẽ chỉ ra rằng các phần tử $a^r m_{r,s}$ với $1 \leq s \leq k_r$, $0 \leq r \leq n$ tạo thành một hệ sinh của A-môđun N. Vì $M_r = a^r M_0$ với mọi $r$, theo định nghĩa của $L_r$ ta có $N_r = a^r L_r$ với mọi $r$. Khi đó, với $r \leq n$,

$$
N_r = a^r L_r = \sum_{s=1}^{k_r} a^r A_0 m_{r,s} \subset \sum_{s=1}^{k_r} A_0 a^r m_{rs},
$$

và, với $r > n$,

$$
N_r = a^r L_n = \sum_{s=1}^{k_n} a^r A_0 m_{n,s} \subset \sum_{s=1}^{k_n} A_0 a^r m_{n,s} \subset \sum_{s=1}^{k_n} A_0 a^{r-n} \cdot (a^n m_{n,s})
$$

điều này hoàn tất chứng minh (x. Bài tập 10).

#### Hệ quả 1 (Định lý Hilbert) {#ac-iii-s2-thm-2-cor-1 .statement}

*Với mọi vành giao hoán Noether C, vành đa thức C[X] là Noether* (x. Bài tập 10).

#### Hệ quả 2 {#ac-iii-s2-thm-2-cor-2 .statement}

*Với mọi vành giao hoán Noether C và mọi số nguyên $n > 0$, vành đa thức C[X_1, ..., X_n] là Noether.*

Điều này suy ra từ Hệ quả 1 bằng quy nạp theo $n$.

#### Hệ quả 3 {#ac-iii-s2-thm-2-cor-3 .statement}

*Nếu C là một vành giao hoán Noether thì mọi C-đại số giao hoán sinh hữu hạn đều là một vành Noether.*

Một đại số như vậy đẳng cấu với một thương của đại số đa thức C[X_1, ..., X_n] (§ 1, no. 1).

#### Hệ quả 4 {#ac-iii-s2-thm-2-cor-4 .statement}

*Cho A là một vành giao hoán phân bậc kiểu $\mathbf{N}$ và gọi $(A_n)$ là phân bậc của nó. Để A là Noether, điều kiện cần và đủ là $A_n$ là Noether và A là một A,-đại số sinh hữu hạn.*

Điều kiện này là đủ theo Hệ quả 3. Ngược lại, giả sử A là Noether; khi đó $m = \sum_{n \geq 1} A_n$, là một iđêan của A, sinh hữu hạn; suy ra A là một A,-đại số sinh hữu hạn (§ 1, no. 2, Hệ quả của Mệnh đề 1); mặt khác $A_n$, đẳng cấu với $A/m$, là một vành Noether.

#### Hệ quả 5 {#ac-iii-s2-thm-2-cor-5 .statement}

*Cho A là một vành giao hoán và m một iđêan của A sao cho $A/m$ là Noether, $m/m^2$ là một $(A/m)$-môđun sinh hữu hạn và A là Hausdorff và đầy đủ đối với tôpô m-adic. Khi đó gr(A) và A là Noether.*

gr(A) là một $(A/m)$-môđun sinh bởi $m/m^2$ (no. 3, Ví dụ 3) và do đó vành gr(A) là Noether theo Hệ quả 3. Từ đó suy ra chính A cũng là Noether (no. 9, Hệ quả 2 của Mệnh đề 12).

#### Hệ quả 6 {#ac-iii-s2-thm-2-cor-6 .statement}

Với mọi vành giao hoán Noether C và mọi số nguyên n > 0, vành các chuỗi lũy thừa hình thức $\mathbf{C}[[X_1, \ldots, X_n]]$ là Noether.

Điều này suy ra từ Hệ quả 5 và no. 6, Hệ quả của Mệnh đề 6, vì nếu m là iđêan của $A = \mathbf{C}[[X_1, \ldots, X_n]]$ gồm các chuỗi lũy thừa hình thức không có số hạng hằng, thì $A/m$ đẳng cấu với C và $m/m^2$ đẳng cấu với C-môđun $\mathbf{C}"$.

Nhận xét

(1) Các Hệ quả 2, 3 và 6 áp dụng đặc biệt khi C là một trường giao hoán.

\* (2) Cho g là một đại số Lie trên một vành giao hoán Noether C và giả sử rằng g là một C-môđun sinh hữu hạn. Gọi đại số bao U của g được trang bị bộ lọc tăng $(U_n)$ được định nghĩa ở no. 3, Ví dụ 4. Với tôpô tương ứng, U là rời rạc và do đó Hausdorff và đầy đủ; vành phân bậc liên kết gr(U) là một C-đại số sinh hữu hạn, vì nó là một thương của đại số đối xứng $\mathcal{S}(g)$, nên gr(U) là một vành Noether (Hệ quả 3) và suy ra U là một vành Noether trái và phải (no. 9, Hệ quả 2 của Mệnh đề 12). \*

### 11. VÀNH m-ADIC ĐẦY ĐỦ VÀ GIỚI HẠN NGƯỢC

Ta đã thấy ở no. 6 rằng, nếu A là một vành giao hoán và m là một iđêan của A sao cho A là Hausdorf và đầy đủ đối với tôpô m-adic, thì vành tôpô $A$ được đồng nhất một cách chính tắc với giới hạn ngược của các vành rời rạc $A_i = A/m^{i+1} \ (i \in \mathbf{N})$ đối với các ánh xạ chính tắc

$$
h_{ij}: A/m^{j+1} \to A/m^{i+1} \quad (i \leq j);
$$

chú ý rằng $h_{ij}$ là toàn ánh và rằng, nếu $n_{ij}$ là hạt nhân của nó, thì

$$
n_{ij} = m^{i+1}/m^{j+1} = (m/m^{j+1})^{i+1} =
$$

đặc biệt là $(n_{0j})^{j+1} = 0$. Ngược lại:

#### Mệnh đề 14 {#ac-iii-s2-prop-14 .statement}

Cho $(A,, h_{ij})$ là một hệ ngược các vành giao hoán rời rạc, có tập chỉ số là $\mathbf{N}$, và gọi $(M_i, u_{ij})$ là một hệ ngược các môđun trên hệ ngược các vành $(A_i, h_{ij})$. Gọi $n_j$ là hạt nhân của $h_{0j}: A \to A$, và đặt $A = \lim A_i$, $M = \lim M_i$. Giả sử rằng

(a) với mọi $i \in \mathbf{N}$, $h_{ii}$ là ánh xạ đồng nhất trên A, và, với $i \leq j$, $h_{ij}$ và $u_{ij}$ là toàn ánh;
(b) với $i \leq j$, các hạt nhân của $h_{ij}$ và $u_{ij}$ lần lượt là $n_j^{i+1}$ và $n_j^{i+1} M_j$.

Khi đó:
(i) $A$ là một vành tôpô Hausdorff đầy đủ, $M$ là một A-môđun tôpô Hausdorff đầy đủ và các ánh xạ chính tắc $h,: A \to A,, u_i: M \to M_i$ là toàn ánh.
(ii) Nếu $M_0$ là một $A_0$-môđun hữu hạn sinh, thì $M$ là một A-môđun hữu hạn sinh;

nói chính xác hơn, mọi tập con hữu hạn S của M sao cho $u_0(S)$ sinh ra M, đều là một hệ sinh của M.

Các khẳng định trong (i) suy ra từ Tôpô đại cương, Chương II, § 3, no. 5, Hệ quả của Mệnh đề 10 và Hệ quả 1 của Định lý 1.

Với mọi $i \in \mathbf{N}$, đặt $m_{i+1} = \mathrm{Ker}(h_i), N_{i+1} = \mathrm{Ker}(u_i)$; khi đó

$$
m_{i+1} = \lim_{k \geq 0} h_{i,t+k}^{-1}(0) = \lim_{\leftarrow} n_{i+1}^{t+k}
$$

và $N_{i+1} = \lim_{\leftarrow} n_{i+k}^{t+1} M_{i+k}$; vì $h_{i+k}$ và $u_{i+k}$ là toàn ánh,

$$
h_{i+k}(m_{i+1}) = n_{i+k}^{t+1}, \quad u_{i+k}(N_{i+1}) = n_{i+k}^{t+1} M_{i+k}.
$$

Hãy chứng minh rằng $m_i N_j \subset N_{i+j}$ với $i \geq 1$ và $j \geq 1$, điều này quy về việc chứng minh rằng $u_{i+j-1}(m_i N_j) = 0$; thật vậy

$$
u_{i+j-1}(m_i N_j) = h_{i+j-1}(m_i) u_{i+j-1}(N_j)
$$

bằng $n_{i+j-1}^{t'}(n_{i+j-1}^{t'} M_{i+j-1}) = 0$, vì, với mọi $k \geq 0$, $n_k^{k+1}$, là hạt nhân của $h_{kk}$, bằng 0. Tương tự ta thấy rằng $m_i m_j \subset m_{i+j}$. Nếu với $i \leq 0$ ta đặt $m_i = A$ và $N_i = M$, thì $(m_i)_{i \in \mathbf{Z}}$ là một filtration của A và $(N_i)_{i \in \mathbf{Z}}$ là một filtration của M tương thích với filtration trên A; các tôpô trên A và M hiển nhiên là những tôpô được xác định bởi các filtration ấy. Khi đó, gọi $a$ là một iđêan của A sao cho $h_1(a) = n_1$ và $M'$ là môđun con của M sinh bởi S; ta sẽ chứng minh rằng

$$
N_i = a^i M' + N_{i+1} \quad \text{với } i \geq 0.
$$

Đặt $a_i = h_i(a), M'_i = u_i(M')$; chỉ cần chứng minh rằng

$$
u_i(N_i) = a_i^i M'_i.
$$

Điều này đúng nếu $i = 0$, vì $N_0 = M$ và $M'_0 = M$, theo giả thiết. Nếu $i \geq 1$, thì $u_i(N_i) = n_i^i M_i$ theo (16). Vì $h_{1i}$ là toàn ánh và $h_{0i} = h_{01} \circ h_{1i}$, $h_{1i}$ biến hạt nhân $n_i$ của $h_i$, thành hạt nhân $n_1$ của $h_1$, và $n_i = h_{1i}(n_1)$; khi đó

$$
h_{1i}(a_i) = h_1(a) = n_1 = h_{1i}(n_i)
$$

và, vì hạt nhân của $h_{1i}$ là $n_i^2$, ta có $n_i \subset a_i + n_i^2$ và $a_i \subset n_i$, do đó $n_i = a_i + n_i^2$. Hơn nữa $u_{0i}(M'_i) = u_0(M') = M, = u_{0i}(M_i)$ và, vì $\mathrm{Ker}(u_{0i}) = n_i M_i$, $M_i = M'_i + n_i M_i$; do đó

$$
n_i^i M_i = (a_i + n_i^2)^i (M'_i + n_i M_i).
$$

Bây giờ, $a_i^k n_i^{i+1-k} \subset n_i^{i+1} = 0$ với $0 \leq k \leq i$; khi đó chắc chắn suy ra rằng $u_i(N_i) = n_i M_i = a_i^i M'_i$, điều này chứng minh (17).

Hơn nữa $m_1 = h_1(n_1)$, do đó $a \subset m_1$ và vì thế $a^i \subset m_1^i \subset m_i$, suy ra

$N_i \subset m_i M' + N_{i+1}$; mặt khác hiển nhiên $m_i M \subset N_i$ và do đó $N_i = m_i M' + N_{i+1}$ với mọi $i \geq 0$; khi đó từ Hệ quả 3 của Mệnh đề 12 ở no. 9 suy ra $M' = M$, điều này kết thúc chứng minh.

#### Hệ quả 1 {#ac-iii-s2-prop-14-cor-1 .statement}

*Với ký hiệu và các giả thiết của Mệnh đề 14, giả sử thêm rằng $M_0$ là một $A$-môđun sinh hữu hạn và iđêan $n_1$ của $A$, là sinh hữu hạn. Gọi $m_1$ là hạt nhân của $h_1$; khi đó các tôpô trên $A$ và $M$ lần lượt là các tôpô $m_1$-adic trên vành này và môđun này; chính xác hơn, với mọi $i \geq 0$, các hạt nhân của $h_i$ và $u_i$ lần lượt là $m_1^{i+1}$ và $m_1^{i+1} M$; hơn nữa $m_1 / m_1^2$ là một $A$-môđun sinh hữu hạn.*

Ta giữ ký hiệu của chứng minh Mệnh đề 14; các giả thiết ở đây cho phép ta giả sử rằng iđêan $a$ là sinh hữu hạn. Gọi $i \geq 0$ là một số nguyên bất kỳ; với mọi $j \geq 0$, theo (17), $N_{i+j} = a^j(a^i M) + N_{i+j+1} \subset m_j(a^i M) + N_{i+j+1}$; ngược lại, $m_j(a^i M) \subset m_j m_i M \subset m_{i+j} M \subset N_{i+j}$, do đó

$$
N_{i+j} = m_j(a^i M) + N_{i+j+1}.
$$

Vì $a$ và $M$ là các $A$-môđun sinh hữu hạn, nên $a^i M$ cũng vậy. Áp dụng Hệ quả 3 của Mệnh đề 12 ở no. 9 cho môđun $N_i$ với bộ lọc $(N_{ij})_{j \in \mathbf{Z}}$ xác định bởi $N_{ij} = N_i$, nếu $j < 0$, $N_{ij} = N_{i+j}$ nếu $j \geq 0$, ta thu được $N_i = a^i M$, do đó $N_i \subset m_1^i M$. Nhưng cũng có $m_1^i M \subset m_i M \subset N_i$, do đó $N_i = m_1^i M$. Áp dụng điều này cho trường hợp $M = A$, $u_{ij} = h_{ij}$, ta được $m_i = m_1^i$. Hơn nữa, $m_1 = a + m_1^2$ theo (17), điều này chứng minh khẳng định cuối cùng của hệ quả.

#### Hệ quả 2 {#ac-iii-s2-prop-14-cor-2 .statement}

*Dưới các giả thiết của Hệ quả 1, để $A$ là Noether, điều kiện cần và đủ là $A$, cũng vậy.*

Điều kiện này là cần thiết vì $A$, đẳng cấu với một thương của $A$; nó là đủ theo no. 10, Hệ quả 5 của Định lý 2.

### 12. BỔ SUNG HAUSDORFF CỦA MỘT MÔĐUN ĐƯỢC LỌC

Cho $G$ là một nhóm được lọc mà bộ lọc $(G,)$ của nó gồm các nhóm con chuẩn tắc của $G$; ta đã nhắc lại (no. 6) rằng *bổ sung Hausdorff* $\hat{G}$ của nhóm tôpô $G$ được đồng nhất một cách chính tắc với giới hạn ngược $\lim \leftarrow G/G_n$ của các nhóm *rời rạc* $G/G_n$, đồng cấu chính tắc $i : G \to \hat{G}$ có ảnh là nhóm Hausdorff liên kết với $G$ (trù mật khắp nơi trong $\hat{G}$) và hạt nhân là bao đóng $\bigcap G$, của $\{0\}$ trong $G$. Bổ sung Hausdorff $\hat{G}_n$ của nhóm con $G$, của $G$ được đồng nhất với bao đóng của $i(G_n)$ trong $\hat{G}$ (*Topologie Générale*, Chương II, § 3, no. 9, Hệ quả 1 của Mệnh đề 18) và, vì $G$, là đóng trong $\hat{G}$,

$$
G, = i^{-1}(\hat{G}_n) = i^{-1}(\hat{G}_n \cap i(G)).
$$

Hơn nữa, các $\hat{G}_n$ tạo thành một hệ cơ bản các lân cận của 0 trong $\hat{G}$ (*Topologie Générale*, Chương 111, § 3, no. 4, Mệnh đề 7) và do đó là các nhóm con mở chuẩn tắc của $\hat{G}$ (Topologie Générale, Chương 111, § 2, no. 3, Mệnh đề 8); tôpô trên $\hat{G}$ được xác định bởi bộ lọc $(\hat{G}_n)$, theo định nghĩa luôn tách biệt. Vì $i(G)$ trù mật trong $\hat{G}$ và $\hat{G}_n$ là mở,

$$
\hat{G} = i(G) \cdot \hat{G}_n
$$

và tương tự,

$$
= i(G_{n-1}) \cdot \hat{G}_n.
$$

Ta suy ra từ (18) và (19) rằng bộ lọc $(\hat{G}_n)$ là phủ hết khi và chỉ khi $(G,)$ là như vậy.

Định lý đẳng cấu thứ hai (Đại số, Chương I, § 6, no. 13, Định lý 6 (d)) và các đẳng thức (18), (19) và (20) cho thấy rằng các đồng cấu chính tắc

$$
G_{n-1}/G_n \to \hat{G}_{n-1}/\hat{G}_n, \quad G/G_n \to \hat{G}/\hat{G}_n,
$$

là song ánh và do đó đồng cấu chính tắc sau cũng vậy

$$
\operatorname{gr}(G) \to \operatorname{gr}(\hat{G}).
$$

Bây giờ cho $A$ là một vành được lọc, $E$ là một $A$-môđun được lọc và $(A_n)$ và $(E_n)$ là các bộ lọc tương ứng của $A$ và $E$; ta sẽ giả thiết rằng các bộ lọc này là phủ hết để đối với các tôpô tương ứng, $A$ là một vành tôpô và $E$ là một $A$-môđun tôpô (no. 5, Mệnh đề 3). Khi đó ta đã định nghĩa (*Topologie Générale*, Chương 111, §6, nos. 5 và 6) $\hat{A}$ như một vành tôpô và $\hat{E}$ như một $\hat{A}$-môđun tôpô. Nếu $i : A \to \hat{A}$ là đồng cấu chính tắc, thì $i(A_m)i(A_n) \subset i(A_{m+n})$, do đó bởi tính liên tục của phép nhân trong $A$,

$$
\hat{A}_m \hat{A}_n \subset \hat{A}_{m+n}
$$

vì $A_n$ là bao đóng của $i(A_n)$ trong $\hat{A}$. Tương tự, có thể chỉ ra rằng

$$
\hat{A}_m \hat{E}_n \subset \hat{E}_{m+n};
$$

nói cách khác:

#### Mệnh đề 15 {#ac-iii-s2-prop-15 .statement}

Cho $A$ là một vành lọc và $E$ một $A$-môđun lọc, các lọc tương ứng $(A_n), (E_n)$ của $A$ và $E$ là vét cạn. Khi đó $(\hat{A}_n)$ là một lọc tương thích với cấu trúc vành trên $\hat{A}$ và $(\hat{E}_n)$ là một lọc tương thích với cấu trúc môđun trên $\hat{E}$ đối với vành lọc $\hat{A}$; hơn nữa các lọc này là vét cạn và lần lượt định nghĩa các tôpô trên $\hat{A}$ và $\hat{E}$. Sau cùng, các ánh xạ chính tắc $\operatorname{gr}(A) \to \operatorname{gr}(\hat{A})$ và $\operatorname{gr}(E) \to \operatorname{gr}(\hat{E})$ của các $\mathbf{Z}$-môđun phân bậc lần lượt là một đẳng cấu vành phân bậc và một đẳng cấu $\operatorname{gr}(A)$-môđun phân bậc.

Trong phần sau, với mọi không gian đều $X$, $j_X$ sẽ ký hiệu ánh xạ chính tắc từ $X$ vào hoàn bị Hausdorff $\hat{X}$ của nó và $X_0 = j_X(X)$ là không gian con đều của $\hat{X}$, vốn là không gian Hausdorff liên kết với $X$. Nhắc lại rằng tôpô trên $X$ là ảnh ngược qua $j_X$ của tôpô trên $X_0$ (Topologie générale,

Chương II, § 3, no. 7, Mệnh đề 12). Cũng nhắc lại rằng, với mọi ánh xạ liên tục đều $f : X \to Y$, $\hat{f}$ ký hiệu ánh xạ liên tục đều từ $\hat{X}$ vào $\hat{Y}$ sao cho $\hat{f} \circ j_X = j_Y \circ f$ (loc. cit., Mệnh đề 15); nếu $X$ là một không gian con đều của $Y$ và $\mathcal{E}$ là đơn ánh chính tắc, thì $\hat{X}$ được đồng nhất với một không gian con đều của $\hat{Y}$ và $\hat{f}$ là đơn ánh chính tắc của $X$ vào $\hat{Y}$ (loc. cit., no. 9. Hệ quả 1 của Mệnh đề 18).

#### Bổ đề 2 {#ac-iii-s2-lem-2 .statement}

*Cho $X \xrightarrow{f} Y \xrightarrow{g} Z$ là một dãy khớp các cấu xạ ngặt của các nhóm tôpô (Đại số, Chương II, § 1, no. 4, Nhận xét). Giả sử rằng $X, Y, Z$ thừa nhận các nhóm hoàn bị Hausdorff và các phần tử đơn vị $\mathcal{E} X, Y, Z$ thừa nhận các hệ cơ bản đếm được của lân cận. Khi đó $\hat{X} \xrightarrow{\hat{f}} \hat{Y} \xrightarrow{\hat{g}} \hat{Z}$ là một dãy khớp các cấu xạ ngặt.*

Gọi $N_1, N_g$ là các hạt nhân tương ứng của f và $g$; ta viết

$$
f = f_3 \circ f_2 \circ f_1
$$

trong đó $f_1$ là ánh xạ chính tắc $X \to X/N_f$, $f_2$ là một đẳng cấu từ $X/N_f$ lên $N$, và $f_3$ là đơn ánh chính tắc $N \to Y$. Ta đã biết rằng $f_2$ là một đẳng cấu từ $(X/N_f)^*$ lên $\hat{N}_g$ và ta vừa nhắc lại rằng $f_1$ là một cấu xạ ngặt đơn ánh từ $N$ vào $\hat{Y}$; nếu ta chứng minh được rằng $\hat{f}_1$ là một cấu xạ ngặt toàn ánh, thì suy ra $\hat{f}$ là một cấu xạ ngặt (Tôpô đại cương, Chương III, § 2, no. 8, Nhận xét 2). Gọi $g_1$ là ánh xạ chính tắc $Y \to Y/N_g$; nếu ta chứng minh được rằng $\hat{g}_1$ là một cấu xạ ngặt toàn ánh của hạt nhân $\hat{N}_g$, thì như trên ta sẽ thấy rằng $\hat{g}$ là một cấu xạ ngặt và dãy $\hat{X} \xrightarrow{\hat{f}} \hat{Y} \xrightarrow{\hat{g}} \hat{Z}$ sẽ khớp. Như vậy ta đã quy bài toán về việc chứng minh rằng, nếu $Y = X/N$ (trong đó $N$ là một nhóm con chuẩn tắc của $X$) và $f : X \to Y$ là ánh xạ chính tắc, thì $\hat{f}$ là một *cấu xạ ngặt toàn ánh với hạt nhân* $\hat{N}$.

Gọi $f_0 : X_0 \to Y_0$ là ánh xạ trùng với $f$ trên $X_0$; vì $j_X$ (tương ứng $j_Y$) là một cấu xạ ngặt toàn ánh từ $X$ lên $X$, (tương ứng từ $Y$ lên $Y_0$), nên $f_0$ là một cấu xạ ngặt toàn ánh (Tôpô đại cương, Chương III, § 2, no. 8, Nhận xét 3). Bây giờ $X_0$ và $Y_0$ là khả mêtric hóa được (Tôpô đại cương, Chương IX, § 3, no. 1, Mệnh đề 1); khi đó từ Tôpô đại cương, Chương IX, § 3, no. 1, Hệ quả 1 của Mệnh đề 4 và Bổ đề 1, suy ra rằng $\hat{f}_0 = \hat{f}$ là một cấu xạ ngặt toàn ánh và có hạt nhân là bao đóng $\hat{N}_0'$ *trong* $X$ của hạt nhân $N_0'$ của $f_0$. Vậy chỉ cần chứng minh rằng $\hat{N}_0' = \hat{N}$. Bây giờ $N_0'$ hiển nhiên chứa $N_0 = j_X(N)$; chỉ cần chứng minh rằng $N_0'$ được chứa trong bao đóng $\overline{N}_0$ của $N_0$ *trong* $X$. Bây giờ,

$$
u = j_X^{-1}(X_0 - \overline{N}_0) = X - j_X^{-1}(\overline{N}_0)
$$

là một tập mở trong $X$ không giao với $N$; vì $f$ là một cấu xạ ngặt toàn ánh, $V = f(U)$ là một tập mở trong $Y$ không chứa phần tử đơn vị $e'$ của $Y$ và do đó không giao với bao đóng của $e'$; khi đó $j_Y(V)$ không chứa phần tử đơn vị của $Y_0$. Nhưng $j_Y(V) = f_0(X_0 - \overline{N}_0)$ và do đó $N'_0 \subset \overline{N}_0$, điều này hoàn thành chứng minh của Bổ đề 2.

#### Mệnh đề 16 {#ac-iii-s2-prop-16 .statement}

*Cho $A$ là một vành lọc, ($A,$) bộ lọc của nó, $E$ một $A$-môđun và ($E_n$) bộ lọc trên $E$ dẫn xuất từ bộ lọc trên $A$ gồm các $E_n = A_n E$. Giả sử rằng bộ lọc ($A,$) là đầy đủ và môđun $E$ là sinh hữu hạn. Nếu $i : E \to \hat{E}$ là ánh xạ chính tắc, thì, với mọi $n \in \mathbf{Z}$,*
$$
8_n = \hat{A}_n \hat{E} = \hat{A}_n i(E) \quad \text{và} \quad \hat{E} = \hat{A}.i(E).
$$
*Đặc biệt $\hat{E}$ là một $\hat{A}$-môđun sinh hữu hạn.*

Đẳng thức $A_n E = E_n$ kéo theo, do tính liên tục của phép toán ngoài trên $A$-môđun $8, \hat{A}_n \hat{E} \subset 8$, và hiển nhiên $\hat{A}_n \hat{E} \supset \hat{A}_n i(E)$. Theo giả thiết tồn tại một đồng cấu toàn ánh $u : L \to E$, với $L = A_s^I$, trong đó $I$ là một tập hợp hữu hạn; trang bị cho $L$ bộ lọc tích, gồm các $L_n = A_n^I$, xác định trên $L$ tôpô tích; khi đó $\hat{L} = \hat{A}_s^I$ và $\hat{L}_n = \hat{A}_n^I$ (*General Topology*, Chương II, § 3, no. 9, Hệ quả 2 của Mệnh đề 18). Gọi $j : L \to \hat{L}$ là ánh xạ chính tắc và $(e_i)_{i \in I}$ là cơ sở chính tắc của $L$; để một phần tử $\sum_{i \in I} a_{ij}(e_i)$ (trong đó $a_i \in \hat{A}$ với mọi $i \in I$) thuộc $\hat{L}_n$, điều kiện cần và đủ là $a_i \in \hat{A}_n$ với mọi $i$; do đó $\hat{L}_n = \hat{A}_n . j(L)$. Như vậy, theo định nghĩa $u(\hat{L}_n) = A_n E = E_n$ và vì thế $u$ là một *cấu xạ ngặt* từ $L$ lên $E$ (*General Topology*, Chương III, § 2, no. 8, Mệnh đề 24). Khi đó Bổ đề 2 cho thấy rằng $\hat{u} : \hat{L} \to \hat{E}$ là một *cấu xạ ngặt toàn ánh*. Vì $\hat{L}_n$ là một nhóm con mở của $\hat{L}$, nên $\hat{u}(\hat{L}_n)$ là một nhóm con mở (và do đó đóng) của $\hat{E}$; nhưng $\hat{u}(\hat{L}_n) = \hat{A}_n \hat{u}(j(L)) = \hat{A}_n i(E)$ và, vì $i(E_n) \subset A_n i(E) \subset \hat{A}_n i(E)$, cuối cùng $\hat{E}_n \subset \hat{A}_n i(E) \subset \hat{A}_n \hat{E} \subset \hat{E}_n$ và do đó $\hat{E}_n = \hat{A}_n \hat{E} = \hat{A}_n i(E)$; đặt $n = 0$, ta thu được công thức thứ hai của (25).

#### Hệ quả 1 {#ac-iii-s2-prop-16-cor-1 .statement}

*Trong các điều kiện của Mệnh đề 16, nếu $A$ đầy đủ thì $E$ cũng vậy.*

Vì khi đó ánh xạ chính tắc $A \to \hat{A}$ là toàn ánh (no. 6, Mệnh đề 5), nên $\hat{E} = i(E)$ theo (25), và kết luận suy ra từ Mệnh đề 5 của no. 6.

#### Hệ quả 2 {#ac-iii-s2-prop-16-cor-2 .statement}

*Cho $A$ là một vành giao hoán, $m$ là một iđêan sinh hữu hạn của $A$ và $\hat{A}$ là bổ sung Hausdorff của $A$ đối với tôpô $m$-adic. Khi đó $\hat{m}^n = (\hat{m})^n = m^n . \hat{A}$ với mọi số nguyên $n > 0$ và tôpô trên $\hat{A}$ là tôpô $\hat{m}$-adic.*

Ta viết $A_n = m^n$, là một iđêan sinh hữu hạn của $A$. Công thức $m^p A_n = m^{n+p}$ cho thấy rằng tôpô cảm sinh trên $A$, bởi tôpô $m$-adic, trùng với tôpô $m$-adic trên $A$-môđun $A_n$ (no. 1, *Ví dụ 3*).

Theo Mệnh đề 16 áp dụng cho $E = A_n$, $\hat{A}_n = \hat{A}.A_n$, nói cách khác $\hat{m}^n = m^n . \hat{A}$. Đặc biệt $m = m . \hat{A}$, do đó
$$
(\hat{m})^n = m^n . \hat{A} = \hat{A}.A_n
$$
(xem Bài tập 12).

Các ví dụ về phép hoàn thành Hausdorff của các vành lọc

(1) Cho $A$ là một vành phân bậc kiểu $\mathbf{N}$ và $(A_n)_{n \geq 0}$ là phân bậc của nó; trang bị cho nó lọc liên kết, lọc này tách được và vét cạn (no. 1, Ví dụ 1). Nhóm cộng $A$ được đồng nhất một cách chính tắc với một nhóm con của $B = \prod_{n \in \mathbf{N}} A_n$; nếu $B$ được trang bị tôpô là tích của các tôpô rời rạc, thì tôpô cảm sinh trên $A$ là tôpô được định nghĩa bởi lọc trên $A$; hơn nữa $B$ là một nhóm tôpô đầy đủ và $A$ trù mật trong $B$ (Tôpô đại cương, Chương III, §2, no. 9, Mệnh đề 25). Khi đó nhóm tôpô cộng tính $B$ được đồng nhất với phép hoàn thành $\hat{A}$ của nhóm cộng Hausdorff $A$ và từ Mệnh đề 15 suy ra rằng nó có một cấu trúc vành duy nhất khiến nó là phép hoàn thành của vành tôpô $A$. Để định nghĩa phép nhân trong vành này, chú ý rằng, nếu ta viết $A'_n = \sum_{i > n} A_i$, thì bao đóng trong $B$ của iđêan hai phía $A'_n$ là tập hợp $B$, gồm các $x = (x_i) \in B$ sao cho $x_i = 0$ với $i \leq n$. Bây giờ cho $x = (x_i), y = (y_i)$ là hai phần tử của $B$ và $z = (z_i)$ là tích của chúng. Khi đó, với mọi $n > 0$, $x \equiv x'_n$ (mod. $B_n$), $y \equiv y'_n$ (mod. $B_n$), trong đó $x'_n = (x_i)_{0 \leq i \leq n}$, $y'_n = (y_i)_{0 \leq i \leq n}$, do đó $z \equiv x'_n y'_n$ (mod. $B_n$). Nhưng $x'_n$ và $y'_n$ thuộc $A$ và vì thế ta thấy rằng, với mọi $n \in \mathbf{N}$,

$$
z_n = \sum_{j=0}^n x_j y_{n-j}.
$$

Đặc biệt, ta lại thu được Hệ quả của Mệnh đề 6 của no. 6: nếu $C$ là một vành giao hoán, thì phép hoàn thành của vành đa thức $C[X_1, \ldots, X_r]$, với lọc liên kết với phân bậc thông thường của nó (theo tổng bậc), được đồng nhất một cách chính tắc với vành chuỗi lũy thừa hình thức $C[[X_1, \ldots, X_r]]$ (xem Đại số, Chương IV, §5, no. 10).

*(2) Cho $K$ là một trường giao hoán đầy đủ với một định giá. Phép hoàn thành của vành các chuỗi hội tụ theo $r$ biến trên $K$ được đồng nhất một cách chính tắc với vành chuỗi lũy thừa hình thức $K[[X_1, \ldots, X_r]]$. \*

(3) Cho $a$ là một phần tử khác không và không khả nghịch của một miền iđêan chính; tôpô (a)-adic trên $A$ cũng được gọi là tôpô $a$-adic; nó là Hausdorff, vì giao của các iđêan $(a^n)$ thu về 0 (Đại số, Chương VII, §1, no. 3). Chú ý rằng bổ sung của $A$ đối với tôpô này không nhất thiết là một miền nguyên (xem no. 13, Nhận xét 3). Vành phân bậc liên kết $\mathrm{gr}(A) = \mathrm{gr}(\hat{A})$ đẳng cấu một cách chính tắc với $(A/a)[X]$ (no. 3, Ví dụ 1). Nếu $A = \mathbf{Z}$, bổ sung của $\mathbf{Z}$ đối với tôpô n-adic ($n > 1$) được ký hiệu bởi $\mathbf{Z}_n$ và các phần tử của nó được gọi là các số nguyên $n$-adic.

Mọi phần tử của $\mathbf{Z}/n^k \mathbf{Z}$ đều có một đại diện duy nhất dạng $\sum_{i=0}^{k-1} a_i n^i$ trong đó $0 \leq a_i \leq n - 1$ với mọi $i$; hơn nữa, ảnh chính tắc của nó trong $\mathbf{Z}/n^{k-1} \mathbf{Z}$ là lớp của $\sum_{i=0}^{k-2} a_i n^i$. Những nhận xét này và việc $Z$, được đồng nhất một cách chính tắc với giới hạn ngược $\lim_{\leftarrow} \mathbf{Z}/n^k \mathbf{Z}$ chỉ ra ngay lập tức rằng mọi phần tử của $Z$, đều có thể được viết duy nhất dưới dạng $\sum_{i=0}^{\infty} a_i n^i$ trong đó $0 \leq a_i < n$ và ngược lại rằng một chuỗi như vậy là hội tụ trong $\mathbf{Z}$.

### 13. BỔ SUNG HAUSDORFF CỦA MỘT VÀNH NỬA ĐỊA PHƯƠNG

#### Mệnh đề 17 {#ac-iii-s2-prop-17 .statement}

Cho $A$ là một vành giao hoán và $(m_{\lambda})_{\lambda \in L}$ là một họ các iđêan của $A$, khác $A$, sao cho $m_{\lambda}$ và $m_{\mu}$ nguyên tố cùng nhau với $\lambda \neq \mu$. Với mọi họ $s = (s(\lambda))_{\lambda \in L}$ các số nguyên $\geq 0$, có giá hữu hạn, đặt $a_s = \bigcap_{\lambda \in L} m_{\lambda}^{s(\lambda)}$ (bằng tích của các $m_{\lambda}^{s(\lambda)}$ ứng với những $\lambda$ sao cho $s(\lambda) \neq 0$; xem Chương 11, § 1, no. 2, các Mệnh đề 3 và 5); các $a_s$ tạo thành một hệ cơ bản các lân cận của 0 đối với một tôpô $\mathcal{T}$ tương thích với cấu trúc vành trên $A$; gọi $\hat{A}$ là bổ sung Hausdorff của $A$ đối với tôpô này. Mặt khác, với mọi $\lambda \in L$, gọi $A_{\lambda}$ là vành $A$ với tôpô $m_{\lambda}$-adic và gọi $\hat{A}_{\lambda}$ là bổ sung Hausdorff của nó. Nếu $u : A \to \prod_{\lambda \in L} A_{\lambda}$ ký hiệu đồng cấu đường chéo, thì $u$ liên tục và đồng cấu tương ứng $\hat{u} :$

$$
\hat{A} \to \left( \prod_{\lambda \in L} A_{\lambda} \right)^{\hat{}} = \prod_{\lambda \in L} \hat{A}_{\lambda}
$$

(Topo đại cương, Chương III, § 6, no. 5 và Chương II, § 3, no. 9, Hệ quả 2 của Mệnh đề 18) là một đẳng cấu tôpô của vành.

Mệnh đề thứ nhất suy ra từ Tôpô đại cương, Chương III, § 6, no. 3, Ví dụ 3. Đặt $B = \prod_{\lambda \in L} A_{\lambda}$; vì tôpô trên $A$ mịn hơn từng tôpô $m_{\lambda}$-adic, các ánh xạ $\mathrm{pr}_{\lambda} \circ u$ là liên tục và do đó $u$ là liên tục. Mặt khác, $u(a_s)$ là giao của đường chéo $A$ của $B$ với tập mở $\bigcap_{\lambda \in L} \mathrm{pr}_{\lambda}^{-1}(m_{\lambda}^{s(\lambda)})$ của $B$; suy ra $u$ là một cấu xạ ngặt từ nhóm cộng $A$ vào $B$ có ảnh là $A$. Bây giờ $\Delta$ là trù mật trong $B$. Thật vậy, cho $b = (a_{\lambda})_{\lambda \in L}$ là một phần tử của $B$; mọi lân cận của $b$ trong $B$ đều chứa một tập có dạng $b + V$, trong đó $V = \bigcap_{\lambda \in L} \mathrm{pr}_{\lambda}^{-1}(m_{\lambda}^{s(\lambda)})$ đối với một họ $s = (s(\lambda))_{\lambda \in L}$ có giá hữu hạn gồm các số nguyên $\geq 0$. Vì các $m_{\lambda}^{s(\lambda)}$ đôi một nguyên tố cùng nhau (Chương II, § 1, no. 2, Mệnh đề 3), tồn tại $x \in A$ sao cho $x \equiv a_{\lambda} \pmod{m_{\lambda}^{s(\lambda)}}$ với mọi $\lambda$ (loc. cit., Mệnh đề 5), và do đó $(b + V) \cap A \neq \varnothing$. Khi đó bổ sung Hausdorff của nhóm $B/\Delta$ là $\{0\}$; áp dụng Bổ đề 2 của no. 12 cho các dãy khớp $0 \to A \xrightarrow{u} B, A \xrightarrow{u} B \to B/\Delta$, ta thấy rằng $\hat{u}$ là một đẳng cấu từ $\hat{A}$ lên $\hat{B}$.

#### Hệ quả {#ac-iii-s2-n13-cor-1 .statement}

Cho $A$ là một miền iđêan chính và $P$ là một hệ đại diện các phần tử cực biên của $A$ (Đại số, Chương VII, § 1, no. 3). Tôpô trên $A$ mà đối với nó các iđêan $\neq 0$ của $\mathbf{A}$ tạo thành một hệ cơ bản các lân cận của 0, tương thích với cấu trúc vành trên $\mathbf{A}$, là Hausdorff và bổ sung của $\mathbf{A}$ theo tôpô này đẳng cấu chính tắc với tích các bổ sung của $\mathbf{A}$ đối với các tôpô $x$-adic, khi $x$ chạy qua $P$.

Các iđêan chính $(x)$ với $\pi \in P$ là cực đại và phân biệt, do đó nguyên tố cùng nhau; ta đã thấy (no. 12, Ví dụ 3) rằng các tôpô $x$-adic là Hausdorff và do đó tôpô được xác định trong mệnh đề của Mệnh đề 17, mịn hơn từng tôpô $x$-adic, cũng là Hausdorff.

Nếu áp dụng Hệ quả của Mệnh đề 17 khi $\mathbf{A} = \mathbf{Z}$, ta ký hiệu bởi $\hat{\mathbf{Z}}$ bổ sung của $\mathbf{Z}$ đối với tôpô mà theo đó mọi iđêan $\neq 0$ của $\mathbf{Z}$ tạo thành một hệ cơ bản các lân cận của 0, vành đẳng cấu với tích $\prod_{p \in P} \mathbf{Z}_p$ của các vành số nguyên $p$-adic ($P$ là tập hợp các số nguyên tố).

Nhận xét

(1) Rõ ràng, dưới các điều kiện của Mệnh đề 17, tôpô $\mathcal{T}$ là cận trên bé nhất của các tôpô $m_\lambda$-adic trên $\mathbf{A}$.

(2) Mọi iđêan đóng $a$ của $\prod_{\lambda \in L} \hat{A}_\lambda$ đồng nhất với tích của các hình chiếu của nó $a_\lambda = \mathrm{pr}_\lambda(a)$, là các iđêan đóng trong các $A_\lambda$; vì $\hat{A}_\lambda$ được đồng nhất một cách chính tắc với một iđêan đóng $A'_\lambda$ của $\prod_{\lambda} \hat{A}_\lambda$ và $a_\lambda$ với $a \cap A'_\lambda$ (Đại số, Chương I, §8, no. 10, Mệnh đề 6), tổng của các $a_\lambda$ là trù mật trong tích $\prod_\lambda a_\lambda$ (Tôpô đại cương, Chương III, §2, no. 9, Mệnh đề 25) và tích sau là đóng trong $\prod_\lambda \hat{A}_\lambda$, do đó có mệnh đề của chúng ta.

#### Mệnh đề 18 {#ac-iii-s2-prop-18 .statement}

Cho $\mathbf{A}$ là một vành giao hoán, $(m_i)_{1 \leq i \leq q}$ là một họ hữu hạn các iđêan cực đại phân biệt của $\mathbf{A}$, t là iđêan tích $m_1 m_2 \ldots m_q = m_1 \cap m_2 \cap \ldots \cap m_q$ và $S$ là tập con nhân $\bigcap_{i=1}^q (\mathbf{A} - m_i)$. Trang bị cho $\mathbf{A}$ tôpô $r$-adic, cho vành $B = S^{-1} \mathbf{A}$ tôpô $rB$-adic và cho mỗi vành địa phương $A_n$ tôpô $(m_i A_{m_i})$-adic. Cho $u : \mathbf{A} \to B$, $v_i : B \to A_{m_i}$ là đồng cấu chính tắc (Chương II, §2, no.1, Hệ quả 2 của Mệnh đề 2) và $v$ là đồng cấu $(v_i) : B \to \prod_{i=1}^q A_n$. Các đồng cấu $u$ và $v$ là liên tục và các đồng cấu tương ứng $\hat{u} : \hat{\mathbf{A}} \to$ và $\hat{v} : \hat{B} \to \prod_{n} (A_n)^*$ là các đẳng cấu tôpô của vành.

$m_i \cap S = \varnothing$ với $1 \leq i \leq q$, do đó iđêan $m'_i = m_i B$ của $B$ là cực đại (Chương II, §2, no. 5, Mệnh đề 11) và
$$
rB = m'_1 \cap m'_2 \cap \cdots \cap m'_q
$$

(Chương II, § 2, no. 4); sau cùng, $B_{m'_i} = A_i$, sai khác bởi một đẳng cấu chính tắc (Chương 11, § 2, no. 5, Mệnh đề 11). Vì $\bar{u}^1(rB) = r$ và $\bar{v}_i^1(m_iA_{m_i}) \supset rB$, $u$ và $v$ là liên tục. Khi đó, chỉ cần chứng minh rằng,

$$
w = v \circ u : A \to \prod_{i=1}^4 A_{m_i},
$$

$\hat{w}$ là một đẳng cấu từ $\hat{A}$ lên $\prod_{i=1}^q \hat{A}_{m_i}$; vì kết quả này áp dụng cho $B$ và các $m'_i$ sẽ cho thấy rằng $\hat{v}$ là một đẳng cấu và do đó $\hat{u}$ cũng vậy. Chú ý rằng mọi tích của các lũy thừa của các $m_i$ đều chứa một lũy thừa của $c$ và vì thế tôpô $r$-adic là cận trên bé nhất của các tôpô $m_i$-adic; hơn nữa, nếu $A_i$ ký hiệu vành $A$ được trang bị tôpô $m_i$-adic và $\phi : A \to \prod_{i=1}^q A$, ánh xạ đường chéo, thì $\hat{\phi} : \hat{A} \to \prod_{i=1}^4 \hat{A}_i$ là một đẳng cấu (Mệnh đề 17). Khi đó mọi việc quy về chứng minh rằng, nếu $u_i : A_i \to A_{m_i}$ là ánh xạ chính tắc, thì $\hat{u}_i : \hat{A}_i \to \hat{A}_{m_i}$ là một đẳng cấu. Bây giờ, với mọi $n$, ánh xạ

$$
u_{i,n} : A/m_i^n \to A_{m_i}/m_i^n A_{m_i}
$$

suy ra từ $u_i$ bằng cách lấy thương là một đẳng cấu (Chương II, §3, no. 3, Mệnh đề 9); mệnh đề của chúng ta suy ra từ sự kiện rằng $\hat{A}_i$ (tương ứng $\hat{A}_{m_i}$) là giới hạn ngược của các vành rời rạc $A/m_i^n$ (tương ứng $A_{m_i}/m_i^n A_{m_i}$) (x. no. 6).

Nhận xét (3). Ta thấy rằng một miền nguyên $A$ có thể có tính chất là hoàn thành Hausdorff $\hat{A}$ của nó thừa nhận các ước của không khác không.

#### Mệnh đề 19 {#ac-iii-s2-prop-19 .statement}

Cho $A$ là một vành giao hoán và $m$ là một iđêan cực đại của $A$. Hoàn thành Hausdorff $\hat{A}$ của $A$ đối với tôpô $m$-adic là một vành địa phương mà iđêan cực đại là $m$.

Nếu $a = \bigcap_{k \geq 1} m^k$, thì $\hat{A}$ là hoàn thành của vành Hausdorff $A/a$ liên kết với $A$ và, vì $m/a$ là cực đại trong $A/a$, ta có thể giả sử rằng $A$ là Hausdorff đối với tôpô $m$-adic. Vì $A/m$ và $\hat{A}/\hat{m}$ là các vành đẳng cấu (no. 12, công thức (21)), nên $m$ là cực đại trong $\hat{A}$. Vì tôpô trên $\hat{A}$ được xác định bởi bộ lọc $(m^n)^*$ (no. 12), mệnh đề sẽ là một hệ quả của bổ đề sau:

#### Bổ đề 3 {#ac-iii-s2-lem-3 .statement}

Cho $A$ là một vành tôpô Hausdorff đầy đủ, trong đó tồn tại một hệ cơ bản $\mathcal{G}$ các lân cận của 0 gồm các nhóm con cộng tính của $A$.
(i) Với mọi $x \in A$ sao cho $\lim_{n \to m} x^n = 0$, $1 - x$ là khả nghịch trong $A$ và nghịch đảo của nó bằng $\sum_{n=0}^\infty x^n$.
(ii) Cho $a$ là một iđêan hai phía của $A$ sao cho $\lim_{n \to \infty} x^n = 0$ với mọi $x \in a$. Để một phần tử y của $\mathbf{A}$ là khả nghịch, điều kiện cần và đủ là lớp của nó mod. a khả nghịch trong $\mathbf{A}/a$; đặc biệt a được chứa trong căn Jacobson của $\mathbf{A}$.

(i) Vì

$$
(1 - x)(1 + x + \cdots + x^n) = (1 + x + \cdots + x^n)(1 - x) = 1 - x^{n+1},
$$

tất cả quy về việc chứng minh rằng chuỗi có số hạng tổng quát $x^n$ là hội tụ trong $\mathbf{A}$; mà, theo giả thiết, với mọi lân cận $V \in \mathfrak{S}$ của 0 trong $\mathbf{A}$, tồn tại một số nguyên $p > 0$ sao cho $x^n \in V$ với mọi $n \geq p$. Ta kết luận rằng

$$
x^p + x^{p+1} + \ldots + x^q \in V
$$

với mọi $q \geq p$ và khi đó mệnh đề của ta suy ra từ tiêu chuẩn Cauchy (*Tôpô đại cương*, Chương III, § 5, no. 2, Định lý 1).

(ii) Giả sử tồn tại $y' \in \mathbf{A}$ sao cho $yy' \equiv 1$ (mod. a) và $y'y \equiv 1$ (mod. a). Giả thiết về a kéo theo, theo (i), rằng $yy'$ và $y'y$ là khả nghịch trong $\mathbf{A}$ và do đó $y$ khả nghịch trong $\mathbf{A}$. Đặc biệt, mọi $x \in a$ đều có tính chất là $1 - x$ khả nghịch trong $\mathbf{A}$ và, vì a là một iđêan hai phía của $\mathbf{A}$, nên nó được chứa trong căn Jacobson của $\mathbf{A}$ (*Đại số*, Chương VIII, § 6, no. 3, Định lý 1).

Sau khi thiết lập bổ đề này, chỉ cần áp dụng nó cho vành tôpô $\hat{\mathbf{A}}$ và iđêan $\hat{\mathfrak{m}}$, vì, với mọi $x \in \hat{\mathfrak{m}}$, $x^n \in (\hat{\mathfrak{m}})^n \subset (\mathfrak{m}^n)^{\wedge}$ và do đó dãy $(x^n)$ tiến tới 0.

Nếu ta lấy $\mathbf{A} = \mathbf{Z}$, mọi iđêan cực đại của $\mathbf{Z}$ đều có dạng $p\mathbf{Z}$ trong đó $p$ là nguyên tố. Khi đó vành các số $p$-adic $\mathbf{Z}_p$ là một vành địa phương mà iđêan cực đại là $p\mathbf{Z}_p$ (Hệ quả 2 của Mệnh đề 16) và trường thặng dư của nó đẳng cấu với $\mathbf{Z}/p\mathbf{Z} = \mathbf{F}_p$, còn $\mathbf{Z}_{(p)}$ với tôpô $p\mathbf{Z}_{(p)}$-adic được đồng nhất với một vành con tôpô của $\mathbf{Z}$, chứa $\mathbf{Z}$.

#### Hệ quả {#ac-iii-s2-n13-cor-2 .statement}

Cho $\mathbf{A}$ là một vành nửa địa phương (Chương II, § 3, no. 5), $m_i$ là các iđêan cực đại phân biệt của nó $(1 \leq i \leq q)$ và

$$
r = m_1 \cap m_2 \cap \cdots \cap m_q
$$

căn Jacobson của nó. Bổ sung Hausdorff $\hat{\mathbf{A}}$ của $\mathbf{A}$ đối với tôpô r-adic là một vành nửa địa phương, đẳng cấu chính tắc với tích $\prod_{i=1}^q \hat{\mathbf{A}}_{m_i}$, trong đó $\hat{\mathbf{A}}_{m_i}$ là vành bổ sung Hausdorff của vành địa phương $\mathbf{A}_{m_i}$ đối với tôpô $(m_i \mathbf{A}_{m_i})$-adic.

### Bài tập {#ac-iii-s2-exercises}

Xem [bài tập cho § 2](exercises/s2/).
