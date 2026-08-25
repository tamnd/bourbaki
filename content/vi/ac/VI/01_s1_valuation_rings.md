---
book: ac
book_title: Commutative Algebra
chapter: VI
chapter_title: VALUATIONS
section: 1
section_title: Valuation rings
lang: vi
source: ac-i-vii
book_pages: 375-381, 441-444
pdf_pages: 0393-0399, 0459-0462
extraction: ocr
subsections:
    - "no": 1
      title: THE RELATION OF DOMINATION BETWEEN LOCAL RINGS
      page: 375
      pdf_page: 393
    - "no": 2
      title: VALUATION RINGS
      page: 376
      pdf_page: 394
    - "no": 3
      title: CHARACTERIZATION OF INTEGRAL ELEMENTS
      page: 378
      pdf_page: 396
    - "no": 4
      title: EXAMPLES OF VALUATION RINGS
      page: 379
      pdf_page: 397
statements: 15
exercises: 7
content_sha256: cf8d86aa11d3334a6802fd6c3689089314013cf55ff1487cce1de28d9746c585
translated_from: content/en/ac/VI/01_s1_valuation_rings.md
source_content_sha256: a947fe432911be13d4aa196ac570607e0088749f8ccb41825c16db8646985cc3
translation_model: gpt-5-6, gpt-5-6-mini
translation_run: translate-vi-6a818b3d
glossary_version: 34
glossary_terms_sha256: e4d48bbd436b76eca1ae1bba7c1f1e9c43364841bcc9a3272a29393009b2e7a2
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 1. CÁC VÀNH ĐỊNH GIÁ

### 1. QUAN HỆ TRỘI GIỮA CÁC VÀNH ĐỊA PHƯƠNG

#### Định nghĩa 1 {#ac-vi-s1-def-1 .statement}

Cho $A$ và $B$ là hai vành địa phương. Ta nói rằng $B$ trội $A$ nếu $A$ là một vành con của $B$ và $m(A) = A \cap m(B)$.

#### Mệnh đề 1 {#ac-vi-s1-prop-1 .statement}

Cho $A$ và $B$ là các vành địa phương sao cho $A$ là một vành con của $B$. Các điều kiện sau là tương đương:
(a) $m(A) \subset m(B)$;
(b) $B$ trội $A$;
(c) iđêan $Bm(A)$ sinh bởi $m(A)$ trong $B$ không chứa 1.

Nếu $m(A) \subset m(B)$, $m(B) \cap A$ là một iđêan của $A$ không chứa 1 và chứa iđêan cực đại $m(A)$; do đó nó bằng iđêan này và (a) suy ra (b). Nếu $B$ trội $A$, iđêan $Bm(A)$ được chứa trong $m(B)$ và do đó không chứa 1; vì vậy (b) suy ra (c). Nếu (c) đúng, $Bm(A)$ được chứa trong iđêan cực đại duy nhất $m(B)$ của $B$, do đó (a).

Chú ý rằng, nếu $K$ là một vành, quan hệ "B trội A" là một quan hệ thứ tự trên tập hợp các vành con địa phương của $K$.

Cho $A$ và $B$ là hai vành địa phương sao cho $B$ trội $A$. Đơn ánh chính tắc $A \to B$ xác định, bằng cách lấy thương, một đẳng cấu của trường $\kappa(A)$ lên một trường con của $\kappa(B)$; đẳng cấu này cho phép ta đồng nhất $\kappa(A)$ với một trường con của $\kappa(B)$.

Ví dụ
(1) Cho $A$ là một vành địa phương Noether và $\hat{A}$ là phần hoàn thiện của nó; vành địa phương $\hat{A}$ khi đó trội $A$ (Chương 111, § 3, no. 5, Mệnh đề 9).
(2) Cho $B$ là một miền nguyên, $A$ một vành con của $B$, $p'$ một iđêan nguyên tố của $B$ và $p = A \cap p'$. Khi đó $pA_p \subset p'B_{p'}$, sao cho $B_{p'}$ trội $A_p$.

### 2. CÁC VÀNH ĐỊNH GIÁ

#### Định lý 1 {#ac-vi-s1-thm-1 .statement}

*Cho K là một trường và V là một vành con của K. Các điều kiện sau là tương đương*:
(a) *V là một phần tử cực đại của tập hợp các vành con địa phương của K, tập hợp này được sắp thứ tự bởi quan hệ "B trội A" giữa A và B.*
(b) *Tồn tại một trường đóng đại số L và một đồng cấu h từ V vào L cực đại trong tập hợp các đồng cấu từ các vành con của K vào L, được sắp thứ tự bởi quan hệ "g là một mở rộng của f" giữa f và g.*
(c) *Nếu $x \in K - V$, thì $x^{-1} \in V$.*
(d) *Trường phân thức của V là K và tập hợp các iđêan chính của V được sắp thứ tự toàn phần bởi quan hệ bao hàm.*
(e) *Trường phân thức của V là K và tập hợp các iđêan của V được sắp thứ tự toàn phần bởi quan hệ bao hàm.*

Ta sẽ chứng minh định lý bằng cách chứng minh các kéo theo sau

$$(a) \Rightarrow (b) \Rightarrow (c) \Rightarrow (d) \Rightarrow (e) \Rightarrow (a).$$

Giả sử (a) đúng. Khi đó $V$ là một vành địa phương. Gọi $L$ là một bao đóng đại số của trường thặng dư $\kappa(V)$ và $h$ là đồng cấu chính tắc từ $V$ đến $L$. Gọi $V'$ là một vành con của $K$ chứa $V$ và $h'$ là một đồng cấu từ $V'$ đến $L$ mở rộng $h$. Nếu $p'$ là hạt nhân của $h'$, thì $p' \cap V = m(V)$; do đó (no. 1, Ví dụ 2) $V'_{p'}$ trội $V$, điều này suy ra $V'_{p'} = V$ và $V' = V$. Vậy (b) đúng.

Giả sử (b) đúng. Gọi $L$ là một trường đóng đại số và $h$ là một đồng cấu từ $V$ đến $L$; giả sử rằng $h$ là cực đại trong tập hợp các đồng cấu từ các vành con của $K$ đến $L$; gọi $p$ là hạt nhân của $h$. Các phần tử của $h(V - p)$ là khả nghịch trong $L$, nên $h$ có thể được mở rộng thành một đồng cấu từ $V_p$ đến $L$ (Chương II, § 2, no. 1, Mệnh đề 1); do đó $V = V_p$, điều này cho thấy rằng $V$ là một vành địa phương và $p$ là iđêan cực đại của nó. Gọi $x$ là một phần tử khác không của $K$; ta phải chứng minh rằng ít nhất một trong các phần tử $x, x^{-1}$ thuộc về $V$, nghĩa là, nhờ đặc trưng cực đại của $h$, rằng $h$ có thể được mở rộng đến $V[x]$ hoặc $V[x^{-1}]$. Nếu $x$ nguyên trên $V$, điều này suy ra từ Chương V, § 2, no. 1, Hệ quả 4 của Định lý 1. Nếu $x$ không nguyên trên $V$, ta sẽ sử dụng bổ đề sau:

#### Bổ đề 1 {#ac-vi-s1-lem-1 .statement}

Cho $A$ là một vành con của một vành $B$ và $x$ là một phần tử của $B$ không nguyên trên $A$; khi đó vành phân thức $B$, (Chương II, § 5, no. 1) *không rút gọn về O* và tồn tại trong vành con $A[1/x]$ của $B$, các iđêan cực đại chứa $1/x$; hơn nữa, nếu $\mathfrak{M}$ là một trong các iđêan cực đại này, ảnh ngược của $\mathfrak{M}$ trong $A$ *là* một iđêan cực đại.

Vì $x$ không nguyên trên $A$, nó không lũy linh và do đó $B, \neq 0$; hơn nữa, $x/1 \notin A[1/x]$, nếu không thì sẽ có một quan hệ có dạng

$$
x/1 = a_0/1 + a_1/x + \cdots + a_n/x^n
$$

với một $n \geq 0$ nào đó (trong đó $a_i \in A$ với $0 \leq i \leq n$), tương đương với

$$
x^{n+h} - a\ x^{n+h-1} - a_1 x^{n+h-2} - \cdots - a_n x^{h-1} = 0
$$

với một $h \geq 1$ thích hợp nào đó; nhưng một quan hệ như vậy sẽ suy ra rằng $x$ là nguyên trên $A$, trái với giả thiết. Sự tồn tại của một iđêan cực đại của $A[1/x]$ chứa $1/x$ do đó suy ra từ sự kiện rằng $1/x$ không khả nghịch trong $A[1/x]$ (*Đại số*, Chương I, § 8, no. 7, Định lý 2).

Khi đó cho $\mathfrak{M}$ là một iđêan cực đại của $A[1/x]$ chứa $1/x$; cho $\phi : A \to A[1/x]$, $p : A[1/x] \to A[1/x]/\mathfrak{M}$ là các đồng cấu chính tắc; khi đó

$$
p(A[1/x]) = p(\phi(A))[p(1/x)] = p(\phi(A))
$$

vì $p(1/x) = 0$; điều này chứng minh rằng $p(\phi(A))$ là một trường và do đó ảnh ngược $\phi^{-1}(\mathfrak{M})$ là một iđêan cực đại của $A$.

Áp dụng bổ đề này với $A = V$ và $B = K$; khi đó có một iđêan cực đại $\mathfrak{m}$ của $V[x^{-1}]$ chứa $x^{-1}$ và $\mathfrak{m} \cap V$ là một iđêan cực đại của $V$, khi đó $\mathfrak{m} \cap V = p$ vì $V$ là địa phương; ký hiệu $f$ là đồng cấu chính tắc của $V[x^{-1}]$ lên $V[x^{-1}]/\mathfrak{m}$, $f(x^{-1}) = 0$, do đó $V/p = f(V) = f(V[x^{-1}])$; vì $h$ xác định bằng cách lấy thương một đơn cấu $\bar{h}$ từ $V/p$ vào $L$, $\bar{h}$ *của* là một đồng cấu từ $V[x^{-1}]$ vào $L$ mở rộng $h$. Do đó (c) đúng.

Giả sử bây giờ (c) được thỏa mãn. Rõ ràng $K$ là trường các phân thức của $V$. Cho $a$ và $b$ là các phần tử của $V$ sao cho $Va \notin Vb$; ta chứng minh rằng $Vb \subset Va$. Điều này đúng nếu $b = 0$; nếu không thì quan hệ $a \notin Vb$ kéo theo $b^{-1}a \notin V$, do đó theo (c) $a^{-1}b \in V$ và vì vậy $Vb \subset Va$. Do đó (d) được thỏa mãn.

Giả sử (d) được thỏa mãn. Cho $a$ và $b$ là các iđêan của $V$ sao cho $a \notin b$. Tồn tại $a \in a$ sao cho $a \notin b$. Với mọi $b \in b$, $a \notin Vb$, do đó $Va \notin Vb$ và vì vậy $Vb \subset Va \subset a$ (theo (c)) và $b \in a$. Khi đó $b \subset a$, điều này chứng tỏ rằng điều kiện (e) *được* thỏa mãn.

Cuối cùng giả sử rằng (e) được thỏa mãn. Vì $V$ có một iđêan cực đại, nó chỉ có một iđêan cực đại và do đó là một vành địa phương. Cho $V'$ là một vành con địa phương của $K$ trội hơn $V$ và cho $x$ là một phần tử khác không của $V'$, ta viết $x = ab^{-1}$ trong đó $a \in V, b \in V$. Một trong các iđêan $Va, Vb$ được chứa trong iđêan kia. *Nếu Va \subset Vb*, thì $x \in V$. *Nếu Vb \subset Va*, thì $x^{-1} \in V$; vì iđêan $V' m(V)$ không chứa 1 (số. 1, Mệnh đề 1), $x^{-1} \notin m(V)$, do đó lại có $x \in V$ vì $V$ là địa phương. Mọi phần tử của $V'$ vì vậy đều thuộc về $V$; ta kết luận rằng (a) được thỏa mãn.

#### Định nghĩa 2 {#ac-vi-s1-def-2 .statement}

*Theo ký hiệu của Định lý 1, $V$ được gọi là một vành định giá đối với trường $K$ nếu các điều kiện tương đương (a), (b), (c), (d), (e) được thỏa mãn. Một vành được gọi là một vành định giá nếu nó là một miền nguyên và nó là một vành định giá đối với trường các phân thức của nó.*

#### Định lý 2 {#ac-vi-s1-thm-2 .statement}

*Cho $K$ là một trường và $h$ là một đồng cấu từ một vành con $A$ của $K$ đến một trường đóng đại số $L$. Khi đó tồn tại một vành định giá $V$ đối với $K$ và một đồng cấu $h'$ từ $V$ đến $L$ sao cho $V$ chứa $A$, $h'$ mở rộng $h$ và $h'^{-1}(O) = m(V)$.*

Cho $\mathfrak{S}$ là tập hợp các đồng cấu của các vành con của $K$ vào $L$, được sắp thứ tự bởi quan hệ mở rộng. Tập hợp này là quy nạp; vì nếu $(h_\alpha)_{\alpha \in I}$ là một họ không rỗng có thứ tự toàn phần của các phần tử của $\mathfrak{S}$ và $B$, là vành xác định của $h_\alpha$, thì các $B_\alpha$ tạo thành một họ có thứ tự toàn phần của các vành con của $K$ và hợp của chúng $B$ do đó là một vành con của $K$; do đó tồn tại một ánh xạ duy nhất $\bar{h}$ từ $B$ vào $L$ mở rộng các $h_\alpha$ (*Set Theory*, Chương II, § 4, no. 6, Mệnh đề 7) và người ta thấy ngay lập tức rằng $\bar{h}$ là một đồng cấu từ $B$ vào $L$. Bổ đề Zorn khi đó chỉ ra rằng tồn tại một phần tử cực đại $h'$ của $\mathfrak{S}$ mở rộng $h$. Vành xác định $V$ của $h'$ là một vành định giá của $K$ (Định lý 1); nếu $p$ là hạt nhân của $h'$, $h'$ có thể được mở rộng thành một đồng cấu từ $V_p$ vào $L$ (Chương II, § 2, no. 1, Mệnh đề 1), do đó $V_p = V$ và $p = m(V)$.

#### Hệ quả {#ac-vi-s1-n2-cor-1 .statement}

*Mọi vành con địa phương $A$ của một trường $K$ đều bị trội bởi ít nhất một vành định giá của $K$.*

Áp dụng Định lý 2 cho đồng cấu chính tắc $h$ từ $A$ vào một bao đóng đại số $L$ của $A/m(A)$.

### 3. ĐẶC TRƯNG HÓA CÁC PHẦN TỬ NGUYÊN

#### Định lý 3 {#ac-vi-s1-thm-3 .statement}

*Cho $A$ là một vành con của một trường $K$. Bao đóng nguyên $A'$ của $A$ trong $K$ là giao của các vành định giá của $K$ chứa $A$; nếu $A$ là địa phương, $A'$ là giao của các vành định giá của $K$ trội $A$.*

Cho $x$ là một phần tử của $A'$ và $V$ là một vành định giá của $K$ chứa $A$; vì $x$ là nguyên trên $V$, tồn tại một iđêan nguyên tố $p'$ của $V[x]$ sao cho $p' \cap V = m(V)$ (Chương V, § 2, no. 1, Định lý 1); rõ ràng khi đó vành địa phương $(V[x])_{p'}$ trội hơn $V$ và do đó bằng nó; do đó $x \in V$. Ngược lại, cho $y$ là một phần tử của $K$ không nguyên trên $A$; khi đó tồn tại một iđêan cực đại 2.2 của $A[y^{-1}]$ chứa $y^{-1}$ (no. 2, Bổ đề 1); cũng tồn tại một vành định giá $V$ của $K$ trội hơn $(A[y^{-1}])_m$ (no. 2, Hệ quả của Định lý 2); vì $y^{-1} \in m(V)$, $y \notin V$. Hơn nữa $2.2 \cap A$ là một iđêan cực đại của $A$ (no. 2, Bổ đề 1); do đó, nếu $A$ là địa phương, $2.2 \cap A = m(A)$ và $V$ trội hơn $A$.

#### Hệ quả 1 {#ac-vi-s1-thm-3-cor-1 .statement}

Mọi vành định giá đều đóng nguyên.

#### Hệ quả 2 {#ac-vi-s1-thm-3-cor-2 .statement}

Để một miền nguyên là đóng nguyên, điều kiện cần và đủ là nó là giao của một họ các vành định giá của trường phân thức của nó.

Trong trường hợp một vành Noether, Hệ quả 2 có thể được làm chính xác hơn (Chương VII, § 1, no. 3, Hệ quả của Định lý 1).

#### Hệ quả 3 {#ac-vi-s1-thm-3-cor-3 .statement}

Cho K là một trường, K' là một mở rộng của K và A là một vành định giá của K. Bao đóng nguyên của A trong K' là giao của các vành định giá V' của K sao cho V' $\cap K = A$.

Định lý 1 (c) cho thấy rằng, nếu V' là một vành định giá của K', V' $\cap K$ là một vành định giá của K và V' trội hơn V' $\cap K$. Để V' trội hơn A, điều kiện cần và đủ là V' $\cap K$ trội hơn A và do đó bằng nó.

### 4. CÁC VÍ DỤ VỀ VÀNH ĐỊNH GIÁ

(1) Mọi trường đều là một vành định giá.

(2) Nếu V' là một vành định giá của một trường K' và K là một trường con của K', V' $\cap K$ là, theo no. 2, Định lý 1 (c), một vành định giá của K.

(3) Mệnh đề sau cung cấp nhiều ví dụ về các vành định giá:

#### Mệnh đề 2 {#ac-vi-s1-prop-2 .statement}

Cho A là một vành địa phương có iđêan cực đại là một iđêan chính Ap. Nếu $\bigcap_{n=1}^{\infty} Ap^n = (0)$ (chẳng hạn nếu A là Noether, xem Chương III, § 3, no. 2, Hệ quả của Mệnh đề 5), các iđêan duy nhất của A là (0) và các Ap^n; khi đó hoặc p là lũy linh hoặc A là một vành định giá.

Cho A được lọc bởi các Ap^n và cho v là hàm cấp tương ứng (Chương III, § 2, no. 2). Vì

$$
\bigcap_{n=1}^{w} Ap^n = (0),
$$

quan hệ $v(x) = +\infty$ kéo theo $x = 0$. Cho a là một iđêan $\neq (0)$ của A và a là một phần tử của a tại đó v nhận giá trị nhỏ nhất của nó; ta viết $v(a) = s$ ($s \neq +\infty$). Khi đó $a \subset Ap^s$. Đặc biệt, tồn tại $u \in A$ sao cho $a = up^s$; vì $a \notin Ap^{s+1}$, $u \notin Ap$; do đó u là khả nghịch và $p^s \in A$ $a \subset a$. Suy ra rằng $a = Ap^s$, do đó mệnh đề đầu tiên của chúng ta. Cũng thấy rằng mọi phần tử $a \neq 0$ của A có thể được viết dưới dạng $a = up^{v(a)}$ trong đó u là khả nghịch. Nếu $a' = u'p^{v(a')}$ ($u'$ khả nghịch) là một phần tử khác không khác của A, thì $aa' = uu'p^{v(a)+v(a')}$; do đó, nếu p không lũy linh, $aa' \neq 0$ và A là một miền nguyên. Khi đó, vì tập hợp các iđêan của A được sắp thứ tự toàn phần theo quan hệ bao hàm, ta kết luận rằng A là một vành định giá (Định lý I (e)).

Ví dụ, nếu $p$ là một số nguyên tố, vành địa phương $\mathbf{Z}_{(p)}$ là một vành định giá. Cho $B = K[X_1, \ldots, X_n]$ là vành đa thức với $n$ phần tử bất định trên một trường $K$; iđêan $BX_1$ là nguyên tố, vì $B/BX_1$ là đẳng cấu với $K[X_2, \ldots, X_n]$; do đó $B_{BX_1}$ là một vành định giá; nó gồm các hàm hữu tỉ $PQ^{-1}$, trong đó $P$ và $Q$ là các đa thức và $Q(0, X,, \ldots, X,) \neq 0$.

Nói chung hơn, ta sẽ thấy rằng, nếu $F$ là một phần tử cực biên của

$$
B = K[X_1, \ldots, X_n],
$$

$B_{BF}$ là một vành định giá (xem Chương VII, § 3, no. 5). \*

Vành các chuỗi lũy thừa hình thức $K[[T]]$ với một phần tử bất định trên một trường $K$ là một miền nguyên địa phương Noether có iđêan cực đại là chính; do đó nó là một vành định giá. Mặt khác, vành $K[[T_1, T_2]]$ các chuỗi lũy thừa hình thức với hai phần tử bất định, là một miền nguyên địa phương Noether, không phải là một vành định giá, vì không phần tử nào trong hai phần tử $T_1, T_2$ là bội của phần tử kia.

#### Mệnh đề 3 {#ac-vi-s1-prop-3 .statement}

*Cho $A$ là một miền iđêan chính và $K$ là trường các phân thức của nó. Các vành định giá của $K$ chứa $A$ và phân biệt với $K$ là các vành có dạng $A_{Ap}$, trong đó $p$ là một phần tử cực biên của $A$.

Rõ ràng $A_{Ap}$ ($p$ cực biên) là một vành định giá chứa $A$ và phân biệt với $K$ (Mệnh đề 2). Ngược lại, cho $V$ là một vành định giá phân biệt với $K$ và chứa $A$. Vì $V \neq K$, $m(V)$ chứa một phần tử $x \neq 0$; viết $x = a/b$ trong đó $a \in A$ và $b \in A$, ta thấy rằng $A \cap m(V)$ chứa phần tử khác không $a$. Vì $A \cap m(V)$ là nguyên tố, nó có dạng $Ap$ trong đó $p$ là cực biên trong $A$. Khi đó $A_{Ap} \subset V, pA_{Ap} \subset m(V)$, do đó $V$ trội $A_{Ap}$; vì $A_{Ap}$ là một vành định giá của $K$ (Mệnh đề 2), $V = A_{Ap}$.

#### Hệ quả 1 {#ac-vi-s1-prop-3-cor-1 .statement}

*Mọi vành định giá của trường $\mathbf{Q}$ và phân biệt với $\mathbf{Q}$ đều có dạng $\mathbf{Z}_{(p)}$ trong đó $p$ là một số nguyên tố.

Mọi vành con của $\mathbf{Q}$ đều chứa $\mathbf{Z}$.

#### Hệ quả 2 {#ac-vi-s1-prop-3-cor-2 .statement}

*Cho $K$ là một trường, $K(X)$ là trường các hàm hữu tỉ theo một bất định trên $K$ và $V$ là một vành định giá của $K(X)$ chứa $K$ và phân biệt với $K(X)$. Nếu $X \in V$, tồn tại một đa thức bất khả quy $P \in K[X]$ sao cho $V = (K[X])_{(P)}$; nếu không thì $V$ là vành địa phương của $K[X^{-1}]$ tại iđêan nguyên tố $X^{-1}K[X^{-1}]$ (nói cách khác $V$ được tạo thành bởi các phân thức $A/B$, trong đó $A \in K[X]$ và $B \in K[X]$, sao cho $\deg(A) \leq \deg(B)$).

Nếu $X \in V$, khi đó $K[X] \subset V$ và mệnh đề đã nêu suy ra từ Mệnh đề 3. Nếu $X \notin V$, khi đó $X^{-1} \in V$, do đó $K[X^{-1}] \subset V$; khi đó $V$ là vành địa phương của $K[X^{-1}]$ tại một iđêan nguyên tố $p$ (Mệnh đề 3) và iđêan này chứa $X^{-1}$ vì $X^{-1}$ không khả nghịch trong V; khi đó $p = X^{-1}K[X^{-1}]$ vì iđêan sau cùng là cực đại. Cuối cùng ta xét một hàm hữu tỉ $A(X)/B(X)$, trong đó A và B là các đa thức có bậc tương ứng là $a$ và $b$; khi đó $A(X) = X^a A'(X^{-1})$ và $B(X) = X^b B'(X^{-1})$, trong đó $A'$ và $B'$ là các đa thức sao cho $A'(0) \neq 0$ và $B'(0) \neq 0$; do đó, để $A(X)/B(X)$ thuộc vành địa phương của $K[X^{-1}]$ tại $X^{-1}K[X^{-1}]$, điều kiện cần và đủ là $a \leq b$.

### Bài tập {#ac-vi-s1-exercises}

Xem [các bài tập cho § 1](exercises/s1/).
