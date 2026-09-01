---
book: ac
book_title: Commutative Algebra
chapter: VI
chapter_title: VALUATIONS
section: 9
section_title: 'Application: locally compact fields'
lang: vi
source: ac-i-vii
book_pages: 431-434, 470-471
pdf_pages: 0449-0452, 0488-0489
extraction: ocr
subsections:
    - "no": 1
      title: THE MODULUS FUNCTION ON A LOCALLY COMPACT FIELD
      page: 431
      pdf_page: 449
    - "no": 2
      title: EXISTENCE OF REPRESENTATIVES
      page: 432
      pdf_page: 450
    - "no": 3
      title: STRUCTURE OF LOCALLY COMPACT FIELDS
      page: 433
      pdf_page: 451
statements: 10
exercises: 5
content_sha256: 14e6aa974dd0c40970a4f76a75323502866a2a9c718c8cfaf25f2fbd04a47d68
translated_from: content/en/ac/VI/09_s9_application_locally_compact_fields.md
source_content_sha256: d266a1348cad0959a68f948795d45c8123c34ab55ddc0962987616e825a8a361
translation_model: gpt-5.4
translation_run: translate-vi-e899e013
glossary_version: 34
glossary_terms_sha256: c8f9c0d50292cb5150f42033a06c03cc92c8cc527b30fe826b4ceeee386ff190
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 9. ỨNG DỤNG: CÁC TRƯỜNG COMPACT ĐỊA PHƯƠNG

### 1. HÀM MÔĐUN TRÊN MỘT TRƯỜNG COMPACT ĐỊA PHƯƠNG

Cho $K$ là một trường compact địa phương (không nhất thiết giao hoán). Nhắc lại rằng hàm mod (hay mod,) đã được định nghĩa (Tích phân, Chương VII, § 1, no. 10, Định nghĩa 6) trên $K$ như sau: $\operatorname{mod}_K(0) = 0$ và với $x \neq 0$ trong $K$, số $\operatorname{mod}_K(x)$ là môđun của tự đẳng cấu $y \mapsto xy$ của nhóm cộng của $K$.

#### Mệnh đề 1 {#ac-vi-s9-prop-1 .statement}

*Nếu $K$ là một trường compact địa phương, hàm mod, thuộc $\mathcal{V}(K)$ (§ 6, no. 1). Hơn nữa:*
(i) *Nếu $s > 0$ sao cho $(\operatorname{mod}_K)^s = g$ là một giá trị tuyệt đối, thì $g$ xác định tôpô trên $K$.*
(ii) *Nếu $K$ không rời rạc và mod, là một giá trị tuyệt đối siêu mêtric, thì tồn tại một định giá rời rạc chuẩn hóa $v$ trên $K$ mà vành của nó là compact và trường thặng dư của nó là hữu hạn với $q$ phần tử, sao cho $\operatorname{mod}, = q^{-v}$. Tôpô trên $K$ được xác định bởi $v$.*

Điều này suy ra từ § 6, no. 1, Mệnh đề 1, § 5, no. 1, Mệnh đề 2 và Tích phân, Chương VII, § 1, no. 10, các Mệnh đề 12 và 13.

#### Mệnh đề 2 {#ac-vi-s9-prop-2 .statement}

*Cho $K, K'$ là hai trường compact địa phương (không nhất thiết giao hoán) sao cho $K$ là một trường con tôpô của $K'$ và $K$ không rời rạc. Khi đó:*
(i) *$K'$ là một không gian vectơ trái (ứng với phải) hữu hạn chiều trên $K$.*
(ii) *Nếu $K$ được chứa trong tâm của $K'$, thì, với mọi $x \in K'$.*
(1)
$$
\operatorname{mod}_{K'}(x) = \operatorname{mod}_K(N_{K'/K}(x)).
$$
Vì $K$ là một trường định giá đầy đủ không rời rạc, mệnh đề (i) suy ra từ Không gian vectơ tôpô, Chương I, § 2, no. 4, Định lý 3; mệnh đề (ii) chính là Tích phân, Chương VII, § 1, no. 11, Mệnh đề 17.

#### Hệ quả 1 {#ac-vi-s9-prop-2-cor-1 .statement}

*Mọi trường compact địa phương có tâm không rời rạc đều có hạng hữu hạn trên tâm của nó.*

Tâm $Z$ của một trường compact địa phương $K$ là đóng trong $K$ và do đó compact địa phương.

#### Hệ quả 2 {#ac-vi-s9-prop-2-cor-2 .statement}

*Cho $K'$ là một trường compact địa phương và $K$ là một trường con đóng của $K'$ (không trường nào nhất thiết giao hoán). Nếu $K'$ là một không gian vectơ trái (ứng với phải) số chiều hữu hạn $n$ trên $K$, thì*
(2)
$$
\operatorname{mod}_{K'}(x) = (\operatorname{mod}_K(x))^n \quad \text{với mọi } x \in K.
$$

Nói chung người ta biết rằng trong một không gian vectơ (trái hoặc phải) số chiều hữu hạn $n$ trên $K$, phép vị tự với tỷ số $x \in K$ có môđun bằng $(\mathrm{mod}_K(x))^n$; chỉ cần áp dụng điều này cho $K'$.

### 2. SỰ TỒN TẠI CỦA CÁC ĐẠI DIỆN

#### Mệnh đề 3 {#ac-vi-s9-prop-3 .statement}

*Cho $K$ là một trường compact địa phương (không nhất thiết giao hoán) không rời rạc và có tôpô được xác định bởi một định giá rời rạc $v$; gọi $A$ là vành và $m$ là iđêan của $v$ và đặt $\mathrm{Card}(A/m) = q = p^f$ ($p$ nguyên tố). Khi đó, tồn tại một hệ đại diện $S$ của $A/m$ trong $A$ và một phần tử đều hóa $u$ đối với $v$ sao cho $O \in S$, $S^* = S \cap K^*$ là một nhóm con cyclic của $K^*$ và $u^{-1} Su = S$. Hơn nữa, mọi phần tử của $A$ đều có thể viết duy nhất dưới dạng $\sum_{i=0}^\infty s_i u^i$, trong đó $s_i \in S$.*

Ta sẽ dùng bổ đề sau:

#### Bổ đề 1 {#ac-vi-s9-lem-1 .statement}

*Cho $x, y$ là hai phần tử của $A$ giao hoán với nhau sao cho $x - y \in m^j \ (j \geq 1)$; khi đó $x^{p^n} - y^{p^n} \in m^{j+n}$ với mọi số nguyên $n \geq 0$.*

Quy nạp theo $n$, ta quy về việc chứng minh bổ đề cho $n = 1$. Khi đó

$$
x^p - y^p = (x - y)(x^{p-1} + x^{p-2}y + \ldots + y^{p-1});
$$

nhân tử thứ hai là một tổng gồm $p$ số hạng đồng dư với nhau mod. $m$ và, vì $A/m$ có đặc số $p$, ta có $p \cdot 1 \in m$ trong $A$ và do đó

$$
x^{p-1} + x^{p-2}y + \ldots + y^{p-1} \in m;
$$

do đó $x^p - y^p \in m^{j+1}$.

Ta biết rằng nhóm nhân $(A/m)^*$ là một nhóm cyclic có $q - 1$ phần tử (*Algebra*, Chương V, § 11, no. 1, Định lý 1); lấy $x$ là một đại diện trong $A$ của một phần tử sinh của nhóm này; khi đó $x^q - x \in m$, do đó, theo Bổ đề 1, $x^{q^{n+1}} - x^{q^n} \in m^{1+fn}$, vì $x^q$ và $x$ giao hoán với nhau. Điều này chứng minh rằng $(x^{q^n})_{n \geq 0}$ là một dãy Cauchy trong $A$; vì $A$ compact và do đó đầy đủ, dãy này có một giới hạn trong $A$; giới hạn đó hiển nhiên thỏa mãn $s \equiv x \pmod{m}$ và $s^q = s$. Vì $s \neq 0$, ta có $s^{q-1} = 1$; chính xác hơn, $s$ là một *primitive* $(q-1)$*-th root of unity* trong $A$. Rõ ràng tập hợp $S$ gồm $0$ và các lũy thừa $s^j \ (0 \leq j \leq q-2)$ là một *hệ đại diện* của các lớp của $A$ mod. $m$ và là *bất biến* đối với phép nhân trong $A$.

Bây giờ lấy $a$ là một phần tử sinh cho $v$ và xét tự đẳng cấu trong $y \mapsto a^{-1}ya$ của $K$; nó biến $A$ thành chính nó, $m$ thành chính nó và do đó, lấy thương, nó xác định một tự đẳng cấu của trường $A/m$; người ta biết (*Algebra*, Chương V, § 11, no. 4, Mệnh đề 5) rằng một tự đẳng cấu như vậy có dạng $z \mapsto z^{p^r}$, trong đó $0 \leq r \leq f-1$. Khi đó $a^{-1}s^j a \equiv s^{jp^r} \pmod{m}$ với $0 \leq j \leq q-2$; vì $a \in m$ và $s \notin m$, điều này suy ra $s^{-j}as^{jp^r} \equiv a \pmod{m^2}$.

Ta viết

$$
u = \sum_{i=0}^{q-2} s^{-1} a s^i p^r.
$$

Khi đó $u \equiv (q - l) a \equiv -a (\text{mod. } m^2)$ vì $p . 1 \in m$; ta kết luận rằng $u$ cũng là một phần tử sinh cho $v$; hơn nữa
(3)
$$
s^{-1} u s^{p^r} = u
$$
do đó ta suy ra rằng $u^{-1} S u = S$.

Cuối cùng, với mọi $x \in A$ tồn tại một dãy duy nhất $(s_i)$ ($i \in \mathbf{N}$) sao cho $s_i \in S$ với mọi $i$ và $x \equiv \sum s_i u^i$ (mod. $m^{n+1}$) với mọi $n \geq 0$: điều này ngay lập tức có được bằng quy nạp theo $n$, mọi phần tử $t$ của $m^{n+1}$ thỏa mãn một quan hệ dạng $t \equiv t' u^{n+1}$ (mod. $m^{n+2}$), trong đó $t'$ là một phần tử của $S$ được xác định duy nhất. Khi đó $x = \sum_{i=0}^{\infty} s_i u^i$ và họ $(s_i)$ thỏa mãn quan hệ này và sao cho $s_i \in S$ với mọi $i$ được xác định duy nhất.

### 3. CẤU TRÚC CỦA CÁC TRƯỜNG COMPACT ĐỊA PHƯƠNG

Các bổ sung đầy đủ $\mathbf{R}$ và $\mathbf{Q}_p$ của trường $\mathbf{Q}$ đối với các giá trị tuyệt đối không không chính quy trên $\mathbf{Q}$ ($p$ là một số nguyên tố bất kỳ) là compact địa phương. Mặt khác, với mọi lũy thừa $q = p^f$ của một số nguyên tố $p$, trường $\mathbf{F}_q((T))$ các chuỗi lũy thừa hình thức trên trường hữu hạn $F$, với định giá được xác định ở § 3, no. 4, Ví dụ 3 là *compact địa phương*: vì iđêan cực đại của vành định giá $\mathbf{F}_q[[T]]$ được sinh bởi $T$; ta biết rằng vành này là đầy đủ đối với tôpô (T)-adic (Chương III, § 2, no. 6, Mệnh đề 6) và, vì trường thặng dư $\mathbf{F}_q$ là hữu hạn, Mệnh đề 2 của § 5, no. 1 chứng minh mệnh đề của chúng ta. Ngược lại:

#### Định lý 1 {#ac-vi-s9-thm-1 .statement}

*Cho K là một trường compact địa phương (không nhất thiết giao hoán) mà không rời rạc.*

(i) *Nếu K có đặc số 0 và mod, không phải là một giá trị tuyệt đối siêu mêtric thì K đẳng cấu với một trong các trường $\mathbf{R}, \mathbf{C}$ hoặc $\mathbf{H}$.*

(ii) *Nếu K có đặc số 0 và mod, là một giá trị tuyệt đối siêu mêtric, thì K là một đại số hạng hữu hạn trên một trường p-adic $\mathbf{Q}_p$.*

(iii) *Nếu K có đặc số $p \neq 0$, thì nó đẳng cấu với một trường có tâm là một trường các chuỗi lũy thừa hình thức $\mathbf{F}_q((T))$ (trong đó $q$ là một lũy thừa của $p$) và có hạng hữu hạn trên tâm của nó.*

(i) Suy ra từ Định lý Ostrowski (§ 6, no. 4, Định lý 2) rằng K là một trường tôpô đẳng cấu với một trường con trù mật khắp nơi của $\mathbf{R}, \mathbf{C}$ hoặc $\mathbf{H}$ và, vì K là đầy đủ, nó đẳng cấu với $\mathbf{R}, \mathbf{C}$ hoặc $\mathbf{H}$.

(ii) Gọi A là vành của giá trị tuyệt đối mod, và m là iđêan cực đại của nó. Ta biết rằng A/m là một trường hữu hạn (§ 5, no. 1, Mệnh đề 2) và do đó giá trị tuyệt đối cảm sinh bởi mod, trên $\mathbf{Q}$ có một trường thặng dư hữu hạn, điều này chỉ có thể xảy ra nếu nó tương đương với một giá trị tuyệt đối $p$-adic ($§ 6$, no. 3, Mệnh đề 4); bao đóng của $\mathbf{Q}$ trong $K$ vì vậy đẳng cấu với $\mathbf{Q}_p$ và được chứa trong tâm của $K$ vì tâm này đóng trong $K$; ta kết luận bằng cách sử dụng Mệnh đề 2 của no. 1.

(iii) Mệnh đề thứ hai suy ra từ mệnh đề thứ nhất và Hệ quả của Mệnh đề 2 của no. 2. Để chứng minh mệnh đề thứ nhất, chú ý rằng mod, tất yếu là một giá trị tuyệt đối siêu mêtric ($§ 6$, no. 2, Hệ quả của Mệnh đề 3); theo ký hiệu của chứng minh Mệnh đề 3 của no. 2, tâm $Z$ của $K$ gồm các phần tử giao hoán với cả $s$ lẫn $u$; nhưng nhờ (3),

$$
u^{-q} s u^q = s^{q p^r} = s,
$$

nên $u^q \in Z$ và ta kết luận rằng $Z$ không rời rạc. Vì $Z$ là compact địa phương, ta có thể tự giới hạn vào trường hợp K là giao hoán. Đại số con trên $\mathbf{F}_p$ là $\mathbf{F}_p[s]$ trong $K$ khi đó là một trường hữu hạn vì $s^{q-1} = 1$ và hiển nhiên $y^q = y$ với mọi phần tử của trường này, do đó nó đồng nhất với $S$ và đẳng cấu với $\mathbf{F}_q$ vì $S \subset \mathbf{F}_p[s]$ có $q$ phần tử. Vì tổng của hai phần tử của $S$ nằm trong $S$, ánh xạ biến mỗi chuỗi lũy thừa hình thức $\sum_{i=0}^\infty s_i T^i \in \mathbf{F}_q[[T]]$ thành phần tử $\sum_{i=0}^\infty s_i u^i$ là một đồng cấu song ánh từ vành $\mathbf{F}_q[[T]]$ lên vành $A$, do đó ngay lập tức có kết luận.

#### Hệ quả 1 {#ac-vi-s9-thm-1-cor-1 .statement}

*Mọi trường compact địa phương* mà *không rời rạc* *đều có hạng hữu hạn* trên tâm của nó.

#### Hệ quả 2 {#ac-vi-s9-thm-1-cor-2 .statement}

Mọi *trường compact địa phương* đều liên thông *hoặc* hoàn toàn không liên thông; *nếu* nó liên thông, thì nó *đẳng cấu* với $\mathbf{R}, \mathbf{C}$ *hoặc* $\mathbf{H}$.

Nếu tôpô trên một trường $K$ được xác định bởi một giá trị tuyệt đối siêu mêtric, thì $K$ hoàn toàn không liên thông đối với tôpô này.

#### Nhận xét {#ac-vi-s9-n3-rem-1 .statement}

Cho $s$ là một số nguyên $> 0$; trường con $\mathbf{F}_q((T^s)) = L$ của $K = \mathbf{F}_q((T))$ là đóng trong $K$ và $e(K/L) = s$ và $f(K/L) = 1$. Vì vậy thấy rằng có những trường con đóng $L$ của $K$ không rời rạc và sao cho $e(K/L)$ (và *a fortiori* bậc $[K:L]$) lớn tùy ý (trái với điều xảy ra đối với các trường compact địa phương có đặc số 0, ở đó mọi trường con compact địa phương $L$ của một trường như vậy $K$ tất yếu chứa $\mathbf{R}$ hoặc $\mathbf{Q}_p$ và do đó $[K:L]$ bị chặn).

### Bài tập {#ac-vi-s9-exercises}

22. (a) Nếu tồn tại một định giá rời rạc trên một trường K, hãy chứng minh rằng bao đóng đại số của K là vô hạn trên K.

(b) Cho K là một mở rộng sinh hữu hạn của trường $K_0$. Chứng minh rằng, nếu K không đại số trên $K_0$, thì tồn tại một định giá rời rạc $v$ trên K sao cho $v(x) = 0$ trên $K_0$.

39

Xem [các bài tập của § 9](exercises/s9/).
