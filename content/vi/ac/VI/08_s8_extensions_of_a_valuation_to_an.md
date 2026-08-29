---
book: ac
book_title: Commutative Algebra
chapter: VI
chapter_title: VALUATIONS
section: 8
section_title: Extensions of a valuation to an algebraic extension
lang: vi
source: ac-i-vii
book_pages: 416-431, 461-469
pdf_pages: 0434-0449, 0479-0487
extraction: ocr
subsections:
    - "no": 1
      title: RAMIFICATION INDEX. RESIDUE CLASS DEGREE
      page: 416
      pdf_page: 434
    - "no": 2
      title: EXTENSION OF A VALUATION AND COMPLETION
      page: 418
      pdf_page: 436
    - "no": 3
      title: THE RELATION $\sum_i e_i f_i \leq n$
      page: 420
      pdf_page: 438
    - "no": 4
      title: INITIAL RAMIFICATION INDEX
      page: 422
      pdf_page: 440
    - "no": 5
      title: THE RELATION $\sum_i e_i f_i = n$
      page: 423
      pdf_page: 441
    - "no": 6
      title: VALUATION RINGS IN AN ALGEBRAIC EXTENSION
      page: 427
      pdf_page: 445
    - "no": 7
      title: THE EXTENSION OF ABSOLUTE VALUES
      page: 428
      pdf_page: 446
statements: 36
exercises: 21
content_sha256: 8a7d1b3cf1bdce48f437788590efec6c8a0d820242a8200c14c02c6d45501ef1
translated_from: content/en/ac/VI/08_s8_extensions_of_a_valuation_to_an.md
source_content_sha256: 1740a7e6d3aaa11959ee2ba6e65707eab0efe09ef5333a215378d18f32bd6007
translation_model: gpt-5-6-mini, gpt-5.4
translation_run: translate-vi-568d1a67
glossary_version: 34
glossary_terms_sha256: f7fba7538678c4e3fcf9a812021913e49958a01f5d3e6e210dea4646fcfe0348
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 8. MỞ RỘNG CỦA MỘT ĐỊNH GIÁ ĐẾN MỘT MỞ RỘNG ĐẠI SỐ

### 1. CHỈ SỐ PHÂN NHÁNH. BẬC LỚP THẶNG DƯ

Cho $\mathbf{K}$ là một trường, $\mathbf{L}$ một mở rộng của $\mathbf{K}$ và $\mathbf{A}'$ một vành định giá của $\mathbf{L}$. Như đã thấy trong § 1, no. 4, vành $\mathbf{A} = \mathbf{K} \cap \mathbf{A}'$ là một vành định giá của $\mathbf{K}$ và
$$
m(\mathbf{A}) = m(\mathbf{A}') \cap \mathbf{K}.
$$
Nếu $v'$ là một định giá liên kết với $\mathbf{A}'$, hạn chế $v$ của $v'$ trên $\mathbf{K}$ là một định giá trên $\mathbf{K}$ liên kết với $\mathbf{A}$; nhóm cấp $\Gamma_v$ của $v$ là một nhóm con của nhóm cấp $\Gamma_{v'}$ của $v'$.

#### Định nghĩa 1 {#ac-vi-s8-def-1 .statement}

*Chỉ số* $[\mathfrak{p}_v : \Gamma_{v'}]$ *được gọi là chỉ số phân nhánh của* $v'$ *trên* $v$ *(hoặc trên* $\mathbf{K}$*) và được ký hiệu là* $e(v'/v)$ *(hoặc* $e(A'/A)$, *hoặc đôi khi* $e(L/K)$*).

Chỉ số này là một số tự nhiên hoặc $+\infty$. Nếu $v'_0$ là một định giá *tương đương* với $v'$, $e(v'/v)$ cũng được gọi là chỉ số phân nhánh của $v'_0$ *trên* $v$. Nếu $e(v'/v) = 1$, $v'$ được gọi là *không phân nhánh* trên $v$.

Mặt khác, trường thặng dư $\kappa(\mathbf{A})$ của $v$ được đồng nhất với một trường con của trường thặng dư $\kappa(\mathbf{A}')$ của $v'$.

#### Định nghĩa 2 {#ac-vi-s8-def-2 .statement}

*Bậc* $[\kappa(\mathbf{A}') : \kappa(\mathbf{A})]$ *được gọi là bậc lớp thặng dư của* $v'$ *trên* $v$ *(hoặc trên* $\mathbf{K}$*) và được ký hiệu là* $f(v'/v)$ *(hoặc* $f(A'/A)$, *hoặc đôi khi* $f(L/K)$*).

Bậc này là một số tự nhiên hoặc $+\infty$.

#### Bổ đề 1 {#ac-vi-s8-lem-1 .statement}

*Cho* $\mathbf{K}, \mathbf{K}', \mathbf{K}''$ *là ba trường sao cho* $K \subset K' \subset K''$, $v''$ *là một định giá trên* $K''$ *và* $v$ *và* $v'$ *là các hạn chế của nó trên* $\mathbf{K}$ *và* $\mathbf{K}'$. *Khi đó có các hệ thức:*
$$(1)\quad e(v''/v) = e(v''/v') e(v'/v), \qquad f(v''/v) = f(v''/v') f(v'/v).$$

Điều này là hiển nhiên.

#### Bổ đề 2 {#ac-vi-s8-lem-2 .statement}

Cho $K$ là một trường, $L$ là một mở rộng hữu hạn của $K$ có bậc $n$, $v'$ là một định giá trên $L$ và $v$ là hạn chế của nó lên $K$. Khi đó bất đẳng thức

$$
e(v'/v) f(v'/v) \leq n
$$

đúng; đặc biệt $e(v'/v)$ và $f(v'/v)$ là hữu hạn.

Ta lấy các số tự nhiên $r$ và $s$ lần lượt không lớn hơn $e(v'/v)$ và $f(v'/v)$. Chỉ cần chứng minh rằng $rs \leq n$. Theo định nghĩa của $r$, tồn tại các phần tử $x_i$ của $L$ ($1 \leq i \leq r$) sao cho $v'(x_i) \not\equiv v'(x_j)$ (mod. $\Gamma_v$) với $i \neq j$. Theo định nghĩa của $s$, tồn tại các phần tử $y_k$ ($1 \leq k \leq s$) của vành $A'$ của $v'$ mà các ảnh chính tắc $\bar{y}_k$ của chúng trong $\kappa(A')$ là độc lập tuyến tính trên $\kappa(A)$; hiển nhiên $v'(y_k) = 0$ với mọi $k$. Ta sẽ chứng minh rằng $rs$ phần tử $x_i y_k$ là độc lập tuyến tính trên $K$, điều này chắc chắn thiết lập bất đẳng thức $rs \leq n$.

Giả sử khi đó tồn tại một quan hệ tuyến tính không tầm thường có dạng

$$
\sum_{i,k} a_{ik} x_i y_k = 0 \quad (a_{ik} \in K).
$$

Ta chọn các chỉ số $j, m$ sao cho

$$
v'(a_{jm} x_j y_m) \leq v'(a_{ik} x_i y_k)
$$

với mọi cặp có thứ tự $(i, k)$; khi đó $a_{jm} \neq 0$. Nếu $i \neq j$, thì $v'(a_{ik} x_i y_k) = v'(a_{jm} x_j y_m)$ là không thể xảy ra vì điều này sẽ suy ra

$$
v'(x_i) - v'(x_j) = v'(a_{jm}) - v'(a_{ik}) \in \Gamma_v,
$$

mâu thuẫn với lựa chọn các $x_i$. Nhân (3) với $(a_{jm} x_j)^{-1}$, ta thu được một quan hệ có dạng

$$
\sum_k b_k y_k + z = 0, \text{ trong đó } b_k = \frac{a_{jk} x_j}{a_{jm} x_j} \in A', \quad z \in A'
$$

và $v'(b_k) \geq 0, v'(z) > 0$. Do đó, trong $\kappa(A')$, một quan hệ có dạng $\sum_k \bar{b}_k \bar{y}_k = 0$. Vì $b_m = 1$, điều này mâu thuẫn với giả thiết đặt ra trên $y_k$.

#### Mệnh đề 1 {#ac-vi-s8-prop-1 .statement}

Cho $K$ là một trường, $L$ là một mở rộng đại số của $K$, $v'$ là một định giá trên $L$, $v$ là hạn chế của nó trên $K$ và $A$ và $A'$ là các vành của $v$ và $v'$. Khi đó $\Gamma_{v'}/\Gamma_v$ là một nhóm xoắn và $\kappa(A')$ là một mở rộng đại số của $\kappa(A)$.

Cho $(L_\alpha)$ là họ các mở rộng con hữu hạn của $L$; ta viết $\Gamma_\alpha = v'(L_\alpha^*)$. Nhóm $\Gamma_{v'}$ là hợp của họ có hướng phải gồm các $\Gamma_\alpha$; vì các nhóm $\Gamma_\alpha/\Gamma_v$ là hữu hạn (Bổ đề 2), $\Gamma_{v'}/\Gamma_v$ là một nhóm xoắn. Lập luận tương tự để chứng minh rằng $\kappa(A')$ là một mở rộng đại số của $\kappa(A)$.

#### Hệ quả 1 {#ac-vi-s8-prop-1-cor-1 .statement}

*Chiều cao của $v'$ bằng chiều cao của $v$.*

Điều này suy ra từ Mệnh đề 1 và bổ đề sau:

#### Bổ đề 3 {#ac-vi-s8-lem-3 .statement}

*Cho $G'$ là một nhóm được sắp thứ tự toàn phần, $G$ là một nhóm con của $G$ và $\mathcal{G}'$ (resp. $\mathcal{G}$) là tập hợp các nhóm con cô lập của $G'$ (resp. $G$). Ánh xạ $H' \mapsto H' \cap G$ ánh xạ $\mathcal{G}'$ lên $\mathcal{G}$. Ánh xạ này là song ánh nếu $G'/G$ là một nhóm xoắn.*

Rõ ràng $H' \in \mathcal{G}'$ kéo theo $H' \cap G \in \mathcal{G}$. Bây giờ cho $H \in \mathcal{G}$; gọi $H'$ là tập hợp các $x' \in G'$ sao cho tồn tại $h \in H$ thỏa mãn $-h \leq x' \leq h$; ta kiểm tra ngay lập tức rằng $H'$ là một nhóm con cô lập của $G'$; khi đó $H' \cap G = H$ vì $H$ là cô lập; do đó ánh xạ $H' \mapsto H' \cap G$ là toàn ánh. Cuối cùng giả sử rằng $G'/G$ là một nhóm xoắn; cho $H'_1$ và $H'_2$ là hai nhóm con cô lập của $G'$ sao cho $H'_1 \cap G = H'_2 \cap G$; khi đó, chẳng hạn, $H'_1 \supset H'_2$ (xem § 4, no. 4); khi đó $H'_1/H'_2$ là một nhóm được sắp thứ tự toàn phần và đẳng cấu với một nhóm thương của $H'_1/(H'_1 \cap G)$ mà bản thân nó được đồng nhất với một nhóm con của $G'/G$; do đó $H'_1/H'_2$ là một nhóm xoắn và vì thế rút gọn về 0.

#### Hệ quả 2 {#ac-vi-s8-lem-3-cor-2 .statement}

*Để $v'$ là không đúng (resp. có chiều cao 1), điều kiện cần và đủ là $v$ là không đúng (resp. có chiều cao 1).*

#### Hệ quả 3 {#ac-vi-s8-lem-3-cor-3 .statement}

*Giả sử rằng $L$ là một mở rộng hữu hạn của $K$. Để $v'$ là rời rạc, điều kiện cần và đủ là $v$ rời rạc.*
Nếu $v'$ là rời rạc, $\Gamma_{v'}$ đẳng cấu với một nhóm con khác không của $\mathbf{Z}$ (Hệ quả 2) và do đó đẳng cấu với $\mathbf{Z}$. Ngược lại, nếu $v$ là rời rạc, $\Gamma_v$ đẳng cấu với $\mathbf{Z}$ và $\Gamma_{v'}/\Gamma_v$ là một nhóm hữu hạn (Bổ đề 2); do đó $\Gamma_{v'}$ là một nhóm giao hoán sinh hữu hạn có hạng 1 và không xoắn; do đó nó đẳng cấu với $\mathbf{Z}$.

### 2. MỞ RỘNG MỘT ĐỊNH GIÁ VÀ HOÀN THIỆN

#### Định nghĩa 3 {#ac-vi-s8-def-3 .statement}

*Cho $K$ là một trường, $v$ là một định giá trên $K$ và $L$ là một mở rộng của $K$. Một họ $(v'_i)_{i \in I}$ các định giá trên $L$ mở rộng $v$ và sao cho mọi định giá trên $L$ mở rộng $v$ là tương đương với duy nhất một $v'_i$ được gọi là một hệ đầy đủ các mở rộng của $v$ lên $L$.*

#### Mệnh đề 2 {#ac-vi-s8-prop-2 .statement}

*Cho $K$ là một trường, $v$ là một định giá trên $K$, $\hat{K}$ là sự hoàn thiện của $K$ đối với $v$, $\hat{v}$ là mở rộng liên tục của $v$ lên $\hat{K}$ và $L$ là một mở rộng hữu hạn của $K$ có bậc $n$.
(a) Cho $v'$ là một định giá trên $L$ mở rộng $v$; ký hiệu $\hat{L}_{v'}$ là sự hoàn thiện của $L$ đối với $v'$ và $8'$ là mở rộng liên tục của $v'$ lên $\hat{L}_{v'}$; đồng nhất $\hat{K}$ với bao đóng của $K$ trong $\hat{L}_{v'}$,
$$
e(\hat{v}'|\hat{v}) = e(v'|v), \quad f(\hat{v}'|\hat{v}) = f(v'|v),
$$
$$
[\hat{L}_{v'} : \hat{K}] \leq n,
$$
$$
e(v'|v)f(v'|v) \preceq [\hat{L}_{v'} : \hat{K}].
$$
(b) *Mọi tập hợp các định giá từng đôi một độc lập trên $L$ mở rộng một định giá không tầm thường $v$ đều là hữu hạn. Gọi $v'_1, \ldots, v'_s$ là các định giá từng đôi một độc lập trên $L$ mở rộng* v sao cho mọi định giá trên L mở rộng v đều phụ thuộc vào một trong các v_i'; gọi L_i là trường L với tôpô được xác định bởi v_i' và $\hat{L}_i$ là sự hoàn thiện của nó; ta viết $n_i = [\hat{L}_i : \hat{K}]$. Khi đó ánh xạ chính tắc

$$
\phi : \hat{K} \otimes_K L \to \prod_{i=1}^s \hat{L}_i
$$

(mở rộng bằng liên tục ánh xạ đường chéo $L \to \prod_{i=1}^s L_i$) là toàn ánh, hạt nhân của nó là căn Jacobson của $\hat{K} \otimes_K L$ và

$$
\sum_{i=1}^s n_i \leq n.
$$

Trước hết, hãy chứng minh (a). Giả sử rằng v không tầm thường. Vì v và $\hat{v}$ (tương ứng $v'$ và $\hat{v}'$) có cùng nhóm cấp và cùng trường thặng dư (§ 5, no. 3, Mệnh đề 5 (b) và (f)), nên (4) đúng. Từ đó, bằng Bổ đề 2, suy ra (6). Sau cùng, không gian vectơ con trên $\hat{K}$ của $\hat{L}_{v'}$ được sinh bởi L là đóng (§ 5, no. 2, Hệ quả của Mệnh đề 4) và trù mật khắp nơi, do đó bằng $\hat{L}_{v'}$; điều này chứng tỏ (5).

Bây giờ ta chuyển sang (b). Ta vẫn có thể giả sử rằng v không tầm thường. Cho $(v_1', \ldots, v_r')$ là một họ hữu hạn bất kỳ gồm các định giá từng đôi một độc lập trên L mở rộng v. Ảnh của L trong $\prod_{i=1}^r L_i$, dưới ánh xạ đường chéo, là trù mật khắp nơi (§ 7, no. 2, Định lý 1) và $\prod_{i=1}^r L_i$ là trù mật trong $\prod_{i=1}^r \hat{L}_i$. Do đó ảnh chính tắc của $\hat{K} \otimes_K L$ trong $\prod_{i=1}^r \hat{L}_i$ là trù mật khắp nơi. Mặt khác ảnh này là một không gian vectơ con trên $\hat{K}$ của $\prod_{i=1}^r \hat{L}_i$; vì $\prod_{i=1}^r \hat{L}_i$ có số chiều hữu hạn trên $\hat{K}$ theo (5), ảnh của $\hat{K} \otimes_K L$ là đóng (§ 5, no. 2, Hệ quả của Mệnh đề 4) và do đó bằng $\prod_{i=1}^r \hat{L}_i$. Vì chiều của $\hat{K} \otimes_K L$ trên K là n, nên $\sum_{i=1}^r n_i \leq n$. Điều này đặc biệt cho thấy số nguyên r bị chặn trên bởi n và chứng tỏ mệnh đề thứ nhất của (b).

Bây giờ ta lấy $(v_1', \ldots, v_s')$ như trong mệnh đề. Việc

$$
\phi : \hat{K} \otimes_K L \to \prod_{i=1}^s \hat{L}_i
$$

là toàn ánh và quan hệ (7) đã được chứng minh. Còn phải kiểm tra rằng hạt nhân n của $\phi$ là căn Jacobson $t$ của $\hat{K} \otimes_K L$. Vì $\prod_{i=1}^s \hat{L}_i$ là nửa đơn, nên $t \subset n$. Mặt khác, với mọi iđêan cực đại m của $\hat{K} \otimes_K L$, trường thương $L(m) = (\hat{K} \otimes_K L)/m$ là một mở rộng hợp thành của $\hat{K}$ và L trên K (*Algebra*,

Chương VIII, § 8, Mệnh đề 1). Tồn tại một định giá w trên L(m) mở rộng $\vartheta$ (§ 3, no. 3, Mệnh đề 5); hạn chế $v'$ của w lên L mở rộng $v$. Vì $[L(m): \hat{K}]$ là hữu hạn, $L(m)$ là đầy đủ đối với w ($§ 5$, no. 2, Mệnh đề 4). Khi đó bao đóng của L trong $L(m)$ là một trường chứa $\mathbf{K}$ và L, nên bằng $L(m)$. Do đó $L(m)$ được đồng nhất với hoàn thành $\hat{L}_{v'}$ và m là hạt nhân của ánh xạ chính tắc từ $\hat{K} \otimes_K L$ lên $\hat{L}_{v'}$. Theo giả thiết, tồn tại một chỉ số $i$ sao cho $v'$ và $v'_i$ phụ thuộc; do đó $L_{v'} = L_i$ ($§ 7$, no. 2, Mệnh đề 3). Vậy $n \subset m$, điều này chứng minh rằng $n \subset r$ và hoàn tất chứng minh.

#### Hệ quả 1 {#ac-vi-s8-prop-2-cor-1 .statement}

*Nếu K đầy đủ đối với v và v không tầm thường, thì hai định giá trên L mở rộng v là phụ thuộc.*

Điều này suy ra vì $\hat{K} \otimes_K L = L$.

#### Hệ quả 2 {#ac-vi-s8-prop-2-cor-2 .statement}

*Nếu $\hat{K}$ hoặc L tách được trên K, thì ánh xạ chính tắc*

$$
\phi : \hat{K} \otimes_K L \to \prod_{i=1}^s \hat{L}_i
$$

*là một đẳng cấu*.

Khi đó căn Jacobson của $\hat{K} \otimes_K L$ bằng không (*Algebra*, Chương VIII, § 7, no. 3, Định lý 1).

#### Nhận xét {#ac-vi-s8-n2-rem-1 .statement}

Mệnh đề 2 (b) cho thấy rằng mọi mở rộng hợp thành của $\hat{K}$ và L trên K (*Algebra*, Chương VIII, § 8) đều đẳng cấu với một trong các hoàn thành $\hat{L}_i$ và rằng đó là các mở rộng hợp thành mà không có hai mở rộng nào đẳng cấu với nhau.

### 3. QUAN HỆ $\sum_i e_i f_i \leq n$

Cho K là một trường, $v$ là một định giá trên K và L là một mở rộng hữu hạn của K bậc $n$. Cho $(v'_1, \ldots, v'_r)$ là các định giá trên L mở rộng $v$ *không có hai định giá nào tương đương; nếu* chúng *độc lập* (điều này luôn đúng nếu $v$ có chiều cao 1), thì

$$
\sum_{i \in I} e(v'_i|v) f(v'_i|v) \leq n
$$

theo Mệnh đề 2 (các công thức (6) và (7)). Ta sẽ thấy rằng kết quả này đúng trong trường hợp tổng quát. Nói chính xác hơn:

#### Định lý 1 {#ac-vi-s8-thm-1 .statement}

*Cho K là một trường, v là một định giá trên K và L là một mở rộng hữu hạn của K bậc n. Khi đó:*

(a) *Mọi hệ đầy đủ $(v'_i)_{i \in I}$ các mở rộng của v lên L đều là hữu hạn.*

(b) $\sum_{i \in I} e(v'_i|v) f(v'_i|v) \leq n$ và a fortiori $\operatorname{Card}(I) \leq n$

(c) *Không có hai nào trong các vành của các $v'_i$ là so sánh được đối với quan hệ bao hàm.*

Vì định lý là tầm thường nếu $v$ là định giá không chính thực, ta sẽ giả sử rằng $v$ không không chính thực. Cho $(v'_1, \ldots, v'_s)$ là một họ hữu hạn bất kỳ các định giá trên L mở rộng $v$, không có

QUAN HỆ $\sum_i e_i f_i \leq n$

hai định giá nào tương đương. Trước hết ta sẽ chứng minh rằng $\sum_{i=1}^s e(v'_i/v)f(v'_i/v) \leq n$. Điều này sẽ chứng minh (a) và (b).

Ta lập luận bằng quy nạp theo s và do đó giả sử rằng bất đẳng thức đã được thiết lập trong trường hợp có 0, 1, ..., s - 1 định giá. Ta phân biệt hai trường hợp.

(1) Giả sử có ít nhất hai định giá $v'_i$ độc lập. Khi đó tồn tại (§ 7, no. 2, Nhận xét 1) một phân hoạch $[1, s] = I_1 \cup \ldots \cup I_t$ của $[1, s]$ sao cho:
(i) để $v'_i$ và $v'_j$ phụ thuộc, điều kiện cần và đủ là $i$ và $j$ thuộc cùng một $I_k$;
(ii) Card$(I_k) < s$ với mọi $k$.

Ta chọn trong mỗi $I_k$ một chỉ số $i(k)$. Ký hiệu $\hat{L}_{i(k)}$ là đầy đủ hóa của $L$ đối với $v'_{i(k)}$ và đặt $n(k) = [\hat{L}_{i(k)} : \hat{K}]$. Với mọi $i \in I_k$, $v'_i$ xác định trên $L$ cùng một tôpô như $v'_{i(k)}$ (§ 7, no. 2, Mệnh đề 3) và do đó có thể mở rộng thành một định giá $\bar{v}'_i$ trên $\hat{L}_{i(k)}$ mà hạn chế của nó lên $\hat{K}$ là 0. Vì không có hai nào trong các $v'_i$ với $i \in I$, là tương đương, điều tương tự cũng đúng đối với các $\bar{v}'_i$. Giả thiết quy nạp áp dụng cho cặp có thứ tự $(\hat{K}, \hat{L}_{i(k)})$ cho thấy, nhờ Mệnh đề 2 (a), công thức (4), rằng $\sum_{i \in I_k} e(v'_i/v)f(v'_i/v) \leq n(k)$. Vì $\sum_{k=1}^t n(k) \leq n$ (Mệnh đề 2 (b), công thức (7)), chắc chắn $\sum_{i=1}^s e(v'_i/v)f(v'_i/v) \leq n$.

(2) Bây giờ ta chuyển sang trường hợp trong đó hai bất kỳ của các $v'_i$ đều phụ thuộc. Gọi $A'_i$ là vành của $v'_i$ ($1 \leq i \leq s$); ký hiệu $A$ là vành của $v$, ta có $A'_i \cap K = A$ với mọi $i$. Gọi $B'$ là vành con của $L$ sinh bởi $A'_1, \ldots, A'_s$; đặt $B = B' \cap K$; khi đó $B \supseteq A$. Khi ấy $B$ là vành của một định giá $w$ trên $K$ và $B'$ là vành của một định giá $w'$ không tầm thường và mở rộng $w$ (§ 7, no. 2, Mệnh đề 4); trường $\kappa(B')$ là một mở rộng của $\kappa(B)$ bậc $f(w'/w)$. Xét các ảnh chính tắc $\bar{A}'_i, \bar{A}$ của $A'_i$ và $A$ trong $\kappa(B')$; khi đó $\bar{A}$ là vành của một định giá $\bar{v}$ trên $\kappa(B)$ và các $\bar{A}'_i$ là các vành của những định giá $\bar{v}'_i$ trên $\kappa(B')$ mở rộng $\bar{v}$. Vì các $A'_i$ sinh ra $B'$, các $\bar{A}'_i$ sinh ra $\kappa(B')$ và do đó các $\bar{v}'_i$ không phải tất cả đều phụ thuộc (§ 7, no. 2, Mệnh đề 4). Từ phần đầu của chứng minh,

$$
\sum_{i=1}^s e(\bar{v}'_i/\bar{v})f(\bar{v}'_i/\bar{v}) \leq [\kappa(B') : \kappa(B)] = f(w'/w)
$$

và do đó

$$
\sum_{i=1}^s e(w'/w)e(\bar{v}'_i/\bar{v})f(\bar{v}'_i/\bar{v}) \leq e(w'/w)f(w'/w) \leq n \quad \text{(no. 1, Bổ đề 1).}
$$

Vậy nên chứng minh của (a) và (b) sẽ hoàn tất nếu ta chứng minh rằng

$$
f(\bar{v}'_i/\bar{v}) = f(\bar{v}'_i/v), \quad e(w'/w)e(\bar{v}'_i/\bar{v}) = e(v'_i/v).
$$

Để làm điều đó, ta lưu ý rằng $v$ và $\bar{v}$ (tương ứng $v'_i$ và $\bar{v}'_i$) có cùng trường thặng dư (§ 4, no. 1, Hệ quả của Mệnh đề 2); điều này chứng minh đẳng thức thứ nhất. Đối với đẳng thức thứ hai, theo Nhận xét ở §4, no. 3, ta có biểu đồ giao hoán sau đây, trong đó các hàng là các dãy khớp và các mũi tên thẳng đứng biểu thị các đơn ánh chính tắc:

$$
\begin{array}{ccccccccc}
0 & \to & \Gamma_{\bar{v}} & \to & \Gamma_v & \to & \Gamma_w & \to & 0 \\
& & \downarrow & & \downarrow & & \downarrow & & \\
0 & \to & \Gamma_{\bar{v}_i'} & \to & \Gamma_{v_i'} & \to & \Gamma_{w'} & \to & 0
\end{array}
$$

Ta suy ra rằng có một dãy khớp

$$
0 \to \Gamma_{\bar{v}_i'}/\Gamma_{\bar{v}} \to \Gamma_{v_i'}/\Gamma_v \to \Gamma_{w'}/\Gamma_w \to 0
$$

theo Chương I, § 1, no. 4, Mệnh đề 2, điều này chứng minh công thức thứ hai (8).

Để hoàn tất chứng minh của Định lý 1, còn phải chứng minh (c). Nếu vành của $v_i'$ chứa vành của $v_j'$, thì $\Gamma_{v_i'}$ được đồng nhất với một nhóm thương $\Gamma_{v_j'}/H$, trong đó $H$ là một nhóm con cô lập (§ 4, no. 3). Vì ánh xạ chính tắc hợp thành

$$
\Gamma_v \to \Gamma_{v_j} \to \Gamma_{v_j'}/H = \Gamma_{v_i'}
$$

là đơn ánh, ta có $H \cap \Gamma_v = \{0\}$, do đó $H = \{0\}$ (Bổ đề 3, no. 1). Khi đó $v_i'$ và $v_j'$ là tương đương, do đó $i = j$.

#### Nhận xét {#ac-vi-s8-n3-rem-1 .statement}

Giao của các vành $A_i'$ của các định giá $v_i'$ ($i \in I$) là bao đóng nguyên của $A$ trong L (§ 1, no. 3, Hệ quả 3 của Định lý 3); hơn nữa, từ (c) và § 7, no. 1, các Mệnh đề 1 và 2 suy ra rằng C là một vành nửa địa phương, rằng các iđêan cực đại của nó là các giao $m_i = C \cap m(A_i')$ và rằng $A_i' = C$, với mọi $i \in I$.

### 4. CHỈ SỐ PHÂN NHÁNH BAN ĐẦU

#### Định nghĩa 4 {#ac-vi-s8-def-4 .statement}

Cho G là một nhóm giao hoán được sắp thứ tự toàn phần và H là một nhóm con của G có chỉ số hữu hạn. Số các tập con lớn của G gồm các phần tử dương ngặt và chứa tất cả các phần tử > O của H được gọi là chỉ số ban đầu của H trong G và được ký hiệu bởi $\varepsilon(G, H)$.

Chỉ số ban đầu này là một số tự nhiên theo mệnh đề sau:

#### Mệnh đề 3 {#ac-vi-s8-prop-3 .statement}

Dưới các giả thiết của Định nghĩa 4, nếu tập hợp các phần tử dương ngặt của G không có phần tử nhỏ nhất, thì $\varepsilon(G, H) = 1$ với mọi H. Nếu tồn tại một phần tử nhỏ nhất > O của G và $G'$ ký hiệu nhóm con do nó sinh ra, thì

$$
\varepsilon(G, H) = (G : (G \cap H)).
$$

Trong trường hợp thứ nhất, cho x là một phần tử > 0 trong G. Tập hợp các $y \in G$ sao cho $0 < y < x$ là vô hạn và do đó tồn tại hai phần tử của tập hợp này phân biệt và đồng dư modulo H; hiệu của chúng là một phần tử z của H sao cho $0 < z < x$. Vì vậy mọi tập con lớn chứa tất cả các phần tử dương ngặt của H đều chứa x và do đó chứa tất cả các phần tử > 0 của G.

Trong trường hợp thứ hai, cho $x$ là phần tử nhỏ nhất >0 của G và cho $n$ là số nguyên nhỏ nhất >0 sao cho $nx \in H$. Rõ ràng $n = (G : (G \cap H))$. Mặt khác, viết $M(y)$ cho tập hợp các $z \in G$ sao cho $y \leq z \ (y \in G)$, ta thấy ngay rằng các tập lớn của Định nghĩa 4 chính là $M(x), M(2x), \ldots, M(nx)$.

#### Hệ quả {#ac-vi-s8-n4-cor-1 .statement}

*Chỉ số ban đầu $\varepsilon(G, H)$ chia chỉ số* $(G : H)$ *và bằng nó nếu* $G$ *đẳng cấu với* $\mathbf{Z}$.

Đặc biệt, $\varepsilon(G, H) \leq (G : H)$.

#### Định nghĩa 5 {#ac-vi-s8-def-5 .statement}

*Cho* $K$ *là một trường, L là một mở rộng hữu hạn của* $K$, $w$ *là một định giá trên* $L$, $v$ *là hạn chế của nó lên* $K$ *và* $\Gamma_w$ *và* $\Gamma_v$ *là các nhóm cấp của chúng. Chỉ số ban đầu của* $\Gamma_v$ *trong* $\Gamma_w$ *được gọi là chỉ số phân nhánh ban đầu của* $w$ *đối với* $v$ *(hoặc đối với* $K$*) và được ký hiệu bởi* $\varepsilon(w/v)$.

Từ hệ quả trên, $\varepsilon(w/v)$ chia $e(w/v)$ với đẳng thức xảy ra trong trường hợp một định giá rời rạc.

#### Mệnh đề 4 {#ac-vi-s8-prop-4 .statement}

*Dưới các giả thiết của Định nghĩa 5, cho* $A$ *và* $m$ *(tương ứng.* $A'$ *và* $m'$*) *là vành và iđêan của định giá* $v$ *(tương ứng.* $w$*). *Khi đó*

$$
[A'/mA': A/m] = \varepsilon(w/v) f(w/v).
$$

Các iđêan của $A'$ chứa $mA'$ và phân biệt với $A'$ tương ứng với các tập con chính của $\Gamma_w$ gồm các phần tử >0 và chứa các phần tử >0 của $\Gamma_v$ (§ 3, no. 5, Hệ quả của Mệnh đề 7). Do đó chúng có số lượng bằng $\varepsilon(w/v)$ và, vì chúng tạo thành một tập hợp được sắp thứ tự toàn phần theo quan hệ bao hàm, số này bằng độ dài của vành thương $A'/mA'$. Mặt khác, một môđun có độ dài 1 trên $A'$ là một không gian vectơ 1 chiều trên $A'/m'$ và vì thế là một môđun có độ dài $f(w/v)$ trên $A$; do đó, vì $A'/mA'$ có độ dài $\varepsilon(w/v)$ trên $A'$, nó có độ dài $\varepsilon(w/v) f(w/v)$ trên $A$, tức là trên $A/m$.

### 5. QUAN HỆ $\sum_i e_i f_i = n$

#### Mệnh đề 5 {#ac-vi-s8-prop-5 .statement}

*Cho* $K$ *là một trường, v là một định giá trên* $K$, $A$ *là vành của nó, m là iđêan của nó, L là một mở rộng hữu hạn của* $K$ *bậc* $n$, $B$ *là bao đóng nguyên của* $A$ *trong* $L$ *và* $(v'_i)_{1 \leq i \leq s}$ *là một hệ đầy đủ các mở rộng của* $v$ *tới* $L$. *Khi đó*

$$
[B/mB : A/m] = \sum_{i=1}^s \varepsilon(v'_i/v) f(v'_i/v).
$$

Gọi $A_i$ là vành của $v'_i$; khi đó $A_i = B_{m_i}$ trong đó $m_i$ chạy qua họ các iđêan cực đại của $B$ (no. 3, Nhận xét). Gọi $q_i$ là bão hòa của $mB$ đối với $m_i$ (Chương II, § 2, no. 4). Theo Chương V, Hệ quả 3 của Mệnh đề 1, no. 1, § 2, đồng cấu chính tắc $B/mB \to \prod_{i=1}^s B/q_i$ là một đẳng cấu và $m_i$ là iđêan cực đại duy nhất của B chứa $q_i$. Do đó $B/q_i$ đẳng cấu chính tắc với $(B/q_i)_{m_i}$ (Chương II, § 3, no. 3, Mệnh đề 8), tức là với
$$
B_{m_i}/mB_{m_i} = A_i/mA_i.
$$
Vì vậy có một đẳng cấu chính tắc $B/mB \to \prod_{i=1}^s A_i/mA_i$, do đó kết quả suy ra nhờ Mệnh đề 4 của no. 4.

#### Hệ quả {#ac-vi-s8-n5-cor-1 .statement}

*Với cùng các giả thiết và ký hiệu,
$$
[B/mB : A/m] = \sum_{i=1}^s \varepsilon(v'_i/v) f(v'_i/v) \leq \sum_{i=1}^s \varepsilon(v'_i/v) f(v'_i/v) \leq n.
$$
Ta biết rằng $\varepsilon(v'_i/v) \leq \varepsilon(v'_i/v)$ (no. 4, Hệ quả của Mệnh đề 3) và $\sum_{i=1}^s \varepsilon(v'_i/v) f(v'_i/v) \leq n$ (no. 3, Định lý 1).

#### Định lý 2 {#ac-vi-s8-thm-2 .statement}

*Với các giả thiết và ký hiệu của Mệnh đề 5, các điều kiện sau là tương đương :
(a) B là một A-môđun hữu hạn sinh;
(b) B là một A-môđun tự do;
(c) $[B/mB : A/m] = n;$
(d) $\sum_{i=1}^n \varepsilon(v'_i/v) f(v'_i/v) = n$ và $\varepsilon(v'_i/v) = \varepsilon(v'_i/v)$ với mọi i.

Sự tương đương của (a) và (b) suy ra từ Bổ đề 1, § 3, no. 6. Rõ ràng (b) kéo theo (c) (*Algebra*, Chương 11, § 1, no. 5, công thức (19)). Sự tương đương của (c) và (d) suy ra từ Hệ quả của Mệnh đề 5. Còn lại phải chứng minh rằng (c) kéo theo (b).

Nói chung, nếu M là một A-môđun, ta sẽ ký hiệu không gian vectơ $M/mM$ trên $A/m$ bởi V(M). Giả thiết (c) có nghĩa là $\dim(V(B)) = n$. Cho $x_1, \ldots, x_n$ là các phần tử của B mà các ảnh chính tắc của chúng trong V(B) lập thành một cơ sở của V(B) và cho L $\subset B$ là A-môđun con do chúng sinh ra. Vì L là không xoắn và sinh hữu hạn, nó là tự do (§ 3, no. 6, Bổ đề 1). Ta sẽ thấy rằng $B = L$. Cho $y \in B$; ta viết $M = L + Ay$; đây cũng là một A-môđun tự do. Các phép nhúng chính tắc $L \to M \to B$ cho các đồng cấu chính tắc $V(L) \to V(M) \to V(B)$. Vì các hạng của L và M là $\leq n$, nên các chiều của V(L) và V(M) cũng vậy. Bây giờ, theo giả thiết, $V(L) \to V(B)$ là toàn ánh và $V(B)$ có chiều n, do đó $V(L)$ và $V(M)$ có chiều n và $V(L) \to V(M)$ là toàn ánh. Vì M sinh hữu hạn, $L \to M$ là toàn ánh (Chương II, § 3, no. 2, Hệ quả 1 của Mệnh đề 4), do đó $L = M, y \in L$ và $B = L$. Suy ra B là tự do.

*Nhận xét (1)* Nếu v là *rời rạc*, $\varepsilon(v'_i/v) = \varepsilon(v'_i/v)$ (no. 4) và điều kiện (d) rút gọn thành $\sum_{i=1}^s \varepsilon(v'_i/v) f(v'_i/v) = n.$

#### Hệ quả 1 {#ac-vi-s8-thm-2-cor-1 .statement}

*Với cùng các giả thiết và ký hiệu, giả sử thêm rằng v là rời rạc và L tách được. Khi đó*

$$
\sum_{i=1}^{s} e(v_i'/v) f(v_i'/v) = n.
$$

Bao đóng nguyên B của A khi đó là một A-môđun tự do có hạng $n$, vì A là một miền iđêan chính (Chương V, § 1, no. 6, Hệ quả 2 của Mệnh đề 18).

#### Hệ quả 2 {#ac-vi-s8-thm-2-cor-2 .statement}

*Cho K là một trường, v là một định giá rời rạc trên K mà theo đó K là đầy đủ và L là một mở rộng hữu hạn của K có bậc n. Khi đó v thừa nhận một mở rộng duy nhất (tới tương đương) $v'$ tới L, vành A' của $v'$ là một môđun tự do sinh hữu hạn trên vành A của v và $e(v'/v) f(v'/v) = n$.*

tôpô adic (trong đó $m = m(A)$); vành A là đầy đủ, vì nó đóng trong K. Ta kết luận rằng, vì $A'/mA'$ là một không gian vectơ hữu hạn chiều ($A/m$)-không gian (no. 4, Mệnh đề 4), A' là một A-môđun sinh hữu hạn (Chương III, § 2, no. 9, Hệ quả 3 của Mệnh đề 12). Do đó nó là tự do và $e(v'/v) f(v'/v) = n$ theo

$$
\phi : \hat{K} \otimes_K L \to \prod_{i=1}^s \hat{L}_i
$$

(no. 2, Mệnh đề 2). *là song ánh. Với mọi $x \in L$, đa thức đặc trưng $P_{C_{L/K}}(x; X)$ bằng tích của các đa thức đặc trưng $P_{C_{\hat{L}_i/\bar{K}}}(x; X)$ ($1 \leq i \leq s$); đặc biệt,

$$
\begin{cases}
\operatorname{Tr}_{L/K}(x) = \sum_{i=1}^s \operatorname{Tr}_{\hat{L}_i/\bar{K}}(x) \\
N_{L/K}(x) = \prod_{i=1}^s N_{\hat{L}_i/\bar{K}}(x) \\
v(N_{L/K}(x)) = \sum_{i=1}^s n_i v_i'(x).
\end{cases}
$$

(Quan hệ cuối cùng trong (9) có ý nghĩa, vì ta có thể hiển nhiên giả sử rằng các $v_i'$, vốn có hạng 1 theo Hệ quả 2 của Mệnh đề 1 trong no. 1, nhận các giá trị của chúng, cũng như v, trong một nhóm con của $\mathbf{R}$.)

Vì không có hai nào trong các $v'_i$ là tương đương và chúng có chiều cao 1, nên chúng độc lập và Mệnh đề 2 của no. 2 do đó cho thấy rằng $e(v'_i/v) f(v'_i/v) \leq n_i$ với mọi $i$ và $\sum_{i=1}^s n_i \leq n$. Mệnh đề thứ nhất do đó suy ra từ các bất đẳng thức này và quan hệ $\sum_{i=1}^s e(v'_i/v) f(v'_i/v) = n$. Dưới đẳng cấu $\phi$ tự đồng cấu $z \mapsto z(1 \otimes x)$ của $\hat{K} \otimes_K L$ (với $x \in L$) được chuyển thành tự đồng cấu của $\prod_{i=1}^s \hat{L}_i$ bảo toàn mỗi nhân tử và trên mỗi nhân tử thu về phép nhân bởi $x$ ($L$ được nhúng một cách chính tắc vào bổ sung của nó $\hat{L}_i$); do đó suy ra mệnh đề liên quan đến đa thức đặc trưng của $x$ và hai công thức đầu của (9). Cuối cùng, cho E là một mở rộng quasi-Galois hữu hạn của $\hat{K}$, chứa $\hat{L}_i$; vì $\hat{K}$ là đầy đủ và $\hat{\nu}$ có chiều cao 1, chỉ tồn tại một định giá duy nhất (tới tương đương) $w$ trên E kéo dài $\hat{\nu}$ (no. 2, Hệ quả 1 của Mệnh đề 2); khi đó, với mọi tự đẳng cấu $\hat{K}$ $\sigma$ của E, $w(\sigma(x)) = v'_i(x)$. Do đó
$$
\vartheta(N_{\hat{L}_i/\hat{K}}(x)) = n_i v'_i(x)
$$
(Đại số, Chương VIII, § 12, no. 2, công thức (15)), điều này chứng minh công thức của (9).

#### Hệ quả 4 {#ac-vi-s8-thm-2-cor-4 .statement}

*Nếu dưới các giả thiết của Hệ quả 3, L là một mở rộng tách được của K, thì mỗi $\hat{L}_i$ là một mở rộng tách được của $\hat{K}$. Nếu hơn nữa L là một mở rộng Galois của K với nhóm Galois $\mathcal{G}$ và $\mathcal{G}_i$ ký hiệu nhóm phân tích của iđêan của $v'_i$ trong B (Chương V, § 2, no. 2, Định nghĩa 2), thì $\hat{L}_i$ là một mở rộng Galois của $\hat{K}$ mà nhóm Galois đẳng cấu với $\mathcal{G}_i$.*

Rõ ràng $\hat{L}_i = \hat{K}(L)$; do đó, nếu L tách được trên K, thì $\hat{L}_i$ tách được trên $\hat{K}$ (Đại số, Chương V, § 7, no. 6, Mệnh đề 10). Bây giờ giả sử rằng L là Galois. Mọi tự đẳng cấu $\sigma \in \mathcal{G}_i$ đều liên tục trên L đối với tôpô được xác định bởi $v'_i$, sự kiện rằng không có hai iđêan nào của các $v'_i$ là so sánh được đối với quan hệ bao hàm (§ 7, no. 2, Hệ quả 1 của Định lý 1) tất yếu kéo theo rằng $v'_i = v'_i \circ \sigma$ theo định nghĩa của $\mathcal{G}_i$; do đó $\sigma$ có thể được kéo dài nhờ tính liên tục thành một tự đẳng cấu $\hat{K}$ $\hat{\sigma}$ của $\hat{L}_i$. Điều này chứng minh rằng số các tự đẳng cấu $\hat{K}$ của off,, ít nhất bằng $\mathrm{Card}(\mathcal{G}_i)$. Nhưng vì các định giá $v'_i$ liên hợp từng đôi một dưới $\mathcal{G}$ (Chương V, § 2, no. 3, Mệnh đề 6), $s = (\mathcal{G}_i)$, do đó
$$
\mathrm{Card}(\mathcal{G}_i) = n/s \leq n.
$$
và mặt khác $n = sn$, theo Hệ quả 3; điều này chứng minh rằng $\hat{L}_i$ là một mở rộng Galois của $\hat{K}$ và rằng các phép kéo dài nhờ tính liên tục của các tự đẳng cấu $\sigma \in \mathcal{G}_i$ là các tự đẳng cấu $\hat{K}$ duy nhất của $\hat{L}_i$.

*Nhận xét (2)*. Một phần của các kết quả trên mở rộng được cho trường hợp các định giá trên một trường K *không nhất thiết giao hoán* (x. § 3, no. 1). Cho L là một trường mở rộng của K và cho $v'$ là một định giá trên L, $v$ là hạn chế của nó lên K, còn A' và A là các vành tương ứng của các định giá $v'$ và $v$; khi đó chỉ số phân nhánh $e(v'/v)$ được xác định như ở no. 1; mặt khác, $\kappa(A)$ được đồng nhất với một trường con của $\kappa(A')$ và hạng thặng dư (trái) của $v'$ đối với $v$ được định nghĩa là số $f(v'/v)$ bằng chiều của không gian vectơ trái trên $\kappa(A)$ là $\kappa(A')$, nếu chiều này là hữu hạn, và bằng $+\infty$ trong trường hợp đối. Khi đó, nếu L là một không gian vectơ trái trên K có số chiều hữu hạn $n$, thì Bổ đề 2 của no. 1 và chứng minh của nó được chuyển sang mà không thay đổi. Hơn nữa, nếu K là đầy đủ đối với $v$, thì các mệnh đề của Hệ quả 2 của Định lý 2 ở no. 5 (ngoài sự tồn tại của $u'$) cũng còn đúng ($n$ ký hiệu chiều của L như một không gian vectơ trái trên K) với chứng minh sau đây:

Trước hết, tôpô do $v'$ xác định trên L là Hausdorff và tương thích với cấu trúc không gian vectơ trái trên K của nó, và do đó hai mở rộng của $v$ lên L cho cùng một tôpô trên L ($§ 5$, no. 2, Mệnh đề 4), điều này chứng minh rằng các mở rộng ấy là như nhau tới tương đương ($§ 6$, no. 2). Tiếp theo ta chỉ ra rằng, nếu $m = m(A)$, thì $A'/mA'$ là một không gian vectơ trái trên $(A/m)$ có chiều $e(v'/v) f(v'/v)$. Viết $e = e(v'/v)$, ta có thể giả sử rằng $v(K^*) = Z$ và $v'(L^*) = e^{-1}Z$; cho $u'$ là một phần tử của L sao cho $v'(u') = e^{-1}$ và $u$ là một phần tử của K sao cho $v(u) = 1$; do đó $u = z{u'}^e$, trong đó $z \in L$ sao cho $v'(z) = 0$. Vì m được sinh bởi $u$ (như một iđêan trái hay phải của A), nên $mA' = {u'}^eA' = A'{u'}^e$ và chỉ cần chứng minh rằng, với $0 \leq k \leq e - 1$, $A'{u'}^k/A'{u'}^{k+1}$ là một không gian vectơ trái trên $(A/m)$ có chiều $f(v'/v)$. Nhưng $t \mapsto t{u'}^k$ là một đẳng cấu từ A-môđun trái A lên A-môđun trái $A'{u'}^k$ biến $A'u'$ thành $A'{u'}^{k+1}$, và vì thế bằng cách lấy thương cho một $(A/m)$-đẳng cấu từ $A'/A'u'$ lên $A'{u'}^k/A'{u'}^{k+1}$, do đó theo định nghĩa của $f(v'/v)$ ta được mệnh đề cần chứng minh, vì $u'$ sinh iđêan cực đại của $A'$. Chứng minh được hoàn tất như khi K và L giao hoán (việc một A-môđun không xoắn sinh hữu hạn thì tự do được chứng minh như trong $§ 3$, no. 6, Bổ đề 1).

### 6. CÁC VÀNH ĐỊNH GIÁ TRONG MỘT MỞ RỘNG ĐẠI SỐ

#### Mệnh đề 6 {#ac-vi-s8-prop-6 .statement}

Cho K là một trường, $v$ một định giá trên K, A là vành của nó, L là một mở rộng đại số của K và $A'$ là bao đóng nguyên của A trong L. Cho 23 là tập hợp các vành định giá trên L mở rộng $v$ và $\mathfrak{M}'$ là tập hợp các iđêan cực đại của $A'$. Khi đó ánh xạ $V \mapsto m(V) \cap A'$ là một song ánh từ 23 lên $\mathfrak{M}'$ và $m' \mapsto A'_{m'}$ là song ánh ngược.

Mọi iđêan cực đại $m'$ của $A'$ đều có tính chất là $m' \cap A$ là iđêan cực đại của A (Chương V, § 2, no. 1, Mệnh đề 1) và $A'_{m'}$ bị một vành định giá V của L chi phối (do đó V là vành của một định giá trên L mở rộng $v$) ($§ 1$, no. 2, Hệ quả của Định lý 2). Trường L là hợp của một họ có hướng các mở rộng con $K_\alpha$ của L, hữu hạn trên K, và để thấy rằng $V = A'_{m'}$, chỉ cần chứng minh rằng $V \cap K_\alpha = A'_{m'} \cap K_\alpha$, với mọi $\alpha$. Bây giờ, nếu viết $A'_\alpha = A' \cap K_\alpha$, thì $A'_\alpha$ là bao đóng nguyên của A trong K, và do đó là giao của các vành của các định giá trên K mở rộng $v$; các vành này $V_{i\alpha}$ là hữu hạn về số lượng và là các vành địa phương $(A'_\alpha)_{m'_{i\alpha}}$ của $A'_\alpha$ ($1 \leq i \leq n$), trong đó các $m'_{i\alpha}$ là các iđêan cực đại phân biệt của $A'_\alpha$ (no. 3, Nhận xét); nhưng $m' \cap A'_\alpha$ là một trong các $m'_{i\alpha}$ và vì thế $V \cap K_\alpha$ bằng vành địa phương tương ứng $(A'_\alpha)_{m'_{i\alpha}} \subset A'_{m'}$, điều này hoàn tất chứng minh rằng $V = A'_{m'}$. Ngược lại, nếu $V \in \mathfrak{V}$, thì $A' \subset V$ (§ 3, no. 3, Mệnh đề 6) và, nếu $m' = m(V) \cap A'$, thì $m' \cap A = m$, do đó $m'$ là một iđêan cực đại của $A'$ (Chương V, § 2, no. 1, Mệnh đề 1) và lập luận trên cho thấy rằng $V = A'_{m'}$.

#### Mệnh đề 7 {#ac-vi-s8-prop-7 .statement}

*Cho K là một trường, L là một mở rộng quasi-Galois của K và f và $f'$ là các phép đặt chỗ của L nhận giá trị trong cùng một trường F. Giả sử rằng các hạn chế của f và $f'$ lên K trùng nhau. Khi đó tồn tại một K-tự đẳng cấu s của L sao cho $f' = f \circ s$.*

Cho A là vành của phép đặt chỗ của K là hạn chế chung của f và $f'$. Các vành của f và $f'$ chứa bao đóng nguyên $A'$ của A trong L (§ 1, no. 3, Hệ quả 3 của Định lý 3) và do đó (Chương V, § 2, no. 3, Hệ quả 1 của Mệnh đề 6) tồn tại một K-tự đẳng cấu s của L sao cho các hạn chế của $f'$ và $f \circ s$ lên $A'$ bằng nhau; nếu $m'$ là hạt nhân chung của các hạn chế này, thì $m' \cap A$ là iđêan cực đại của A, do đó $m'$ là một iđêan cực đại của $A'$ và các phép đặt chỗ $f'$ và $f \circ s$ trùng nhau trên vành $A'_{m'}$; nhưng theo Mệnh đề 6, vành định giá duy nhất của L chi phối $A'_{m'}$ là chính vành $A'_{m'}$ và do đó các vành của các phép đặt chỗ $f'$ và $f \circ s$ là như nhau.

#### Hệ quả 1 {#ac-vi-s8-prop-7-cor-1 .statement}

*Cho K là một trường, v là một định giá trên K, L là một mở rộng quasi-Galois của K và $v'$ và $v''$ là hai mở rộng của v lên L. Khi đó tồn tại một K-tự đẳng cấu s của L sao cho $v''$ tương đương với $v' \circ s$.*

Cho $f'$ và $f''$ là các phép đặt chỗ của K liên kết với $v'$ và $v''$; bằng cách thay thế chúng, nếu cần, bởi các phép đặt chỗ tương đương, có thể giả sử rằng cả hai đều nhận giá trị trong bao đóng đại số của trường thặng dư của v (no. 1, Mệnh đề 1). Khi đó tồn tại một K-tự đẳng cấu s của L sao cho $f'' = f' \circ s$ (Mệnh đề 7); do đó $v''$ tương đương với $v' \circ s$ theo sự tương ứng giữa các phép đặt chỗ và các định giá (§ 3, no. 3).

#### Hệ quả 2 {#ac-vi-s8-prop-7-cor-2 .statement}

*Cho K là một trường, f là một phép đặt chỗ của K (tương ứng v là một định giá trên K) và L là một mở rộng radicial của K. Khi đó mọi mở rộng của f (tương ứng của v) lên L đều tương đương.*

L là một mở rộng quasi-Galois và tự đẳng cấu duy nhất của nó là đồng nhất. Do đó Hệ quả 2 suy ra từ Mệnh đề 7 (tương ứng Hệ quả 1).

#### Mệnh đề 8 {#ac-vi-s8-prop-8 .statement}

*Cho K là một trường, v một định giá trên K, L một mở rộng quasi-Galois hữu hạn của K bậc n và $(v'_i)_{1 \leq i \leq g}$ một hệ đầy đủ các mở rộng của v lên L. Khi đó $e(v'_i/v)$ và $f(v'_i/v)$ có các giá trị e và $\mathfrak{f}$ độc lập với i. Khi đó $ef g \leq n$. Nếu bao đóng nguyên trong L của vành A của v là một A-môđun hữu hạn sinh, thì $ef g = n$.*

Điều này suy ra ngay lập tức từ các Định lý 1 (no. 3) và 2 (no. 5).

### 7. SỰ MỞ RỘNG CỦA CÁC GIÁ TRỊ TUYỆT ĐỐI

#### Mệnh đề 9 {#ac-vi-s8-prop-9 .statement}

*Cho K là một trường, L một mở rộng đại số của K và $\mathfrak{f}$ một giá trị tuyệt đối trên K. Khi đó $\mathfrak{f}$ có thể được mở rộng thành một giá trị tuyệt đối trên L.*

Trước hết giả sử rằng tồn tại một định giá $v$ trên $K$ với các giá trị thực sao cho $f(x) = e^{-v(x)}$. Tồn tại một định giá $v'$ trên $L$ mà hạn chế của nó lên $K$ tương đương với $v$ ($§ 3$, no. 3, Mệnh đề 5). Khi đó $v'$ có chiều cao 0 hoặc 1 (no. 1, Hệ quả 2 của Mệnh đề 1) và do đó có thể giả thiết là có các giá trị thực. Hạn chế của ánh xạ $x \mapsto e^{-v'(x)}$ lên $K$ là một giá trị tuyệt đối tương đương với $f$ và vì thế có dạng $f^s$ với $s > 0$ (*Tôpô đại cương*, Chương IX, $§ 3$, no. 2, Mệnh đề 5). Ta kết luận rằng

$$
x \mapsto e^{-v'(x)/s}
$$

là một giá trị tuyệt đối trên $L$ mở rộng $f$.

Bây giờ giả sử rằng $f$ không siêu mêtric. Khi đó $K$ được đồng nhất với một trường con của $\mathbf{C}$ sao cho $f(x) = |x|^s$ với $0 \leq s \leq 1$ ($§ 6$, no. 4, Định lý 2). Vì $\mathbf{C}$ đóng đại số, nên $L$ được đồng nhất với một trường con của $\mathbf{C}$ và giá trị tuyệt đối $x \mapsto |x|^s$ mở rộng $f$.

#### Mệnh đề 10 {#ac-vi-s8-prop-10 .statement}

*Cho $K$ là một trường, $f$ một giá trị tuyệt đối trên $K$ sao cho $K$ đầy đủ và không rời rạc đối với $f$ và $L$ một mở rộng đại số của $K$. Khi đó $f$ có thể được mở rộng một cách duy nhất thành một giá trị tuyệt đối $f'$ trên $L$ và, nếu $L$ có bậc hữu hạn $n$, thì*

$$
f'(x) = (f(N_{L/K}(x)))^{1/n}
$$

*đối với mọi* $x \in L$.

Sự tồn tại của $f'$ suy ra từ Mệnh đề 9 và tính duy nhất của nó (trên mọi mở rộng con hữu hạn của $L$ và do đó trên toàn thể $L$) suy ra từ Bổ đề 2 của $§ 6$, no. 4. Gọi $f'$ là mở rộng duy nhất của $f$ lên bao đóng đại số của $K$ và giả sử $L$ có bậc hữu hạn $n$. Ta biết rằng $N_{L/K}(x) = \prod_{i=1}^n x_i$, trong đó mỗi $x_i$ là một liên hợp của $x$ trên $K$ (*Algebra*, Chapter VIII, $§ 12$, no. 2, Proposition 4). Xét theo tính duy nhất của $f'$, ta có $f'(x_i) = f'(x)$ với mọi $i$, do đó suy ra công thức đã nêu.

#### Mệnh đề 11 {#ac-vi-s8-prop-11 .statement}

*Cho $K$ là một trường, $f$ là một giá trị tuyệt đối không siêu Acsimet trên $K$, $\hat{K}$ là phép hoàn thành của $K$ đối với $f$, $\hat{f}$ là mở rộng liên tục của $f$ lên $\hat{K}$ và $L$ là một mở rộng hữu hạn của $K$ bậc $n$.

(a) *Cho $f'$ là một giá trị tuyệt đối trên $L$ mở rộng $f$; gọi $\hat{L}_{f'}$ là phép hoàn thành của $L$ đối với $f'$ và đồng nhất $\hat{K}$ với bao đóng của $K$ trong $\hat{L}_{f'}$; khi đó* $[\hat{L}_{f'} : K] \leq n$.

(b) *Các giá trị tuyệt đối trên $L$ mở rộng $f$ có số lượng hữu hạn. Nếu ký hiệu chúng là* $f'_1, \ldots, f'_s$ *và ký hiệu phép hoàn thành của $L$ đối với* $f'_i$ *là* $\hat{L}_i$, *thì ánh xạ chính tắc*

$$
\hat{K} \otimes_K L \to \prod_{i=1}^s \hat{L}_i
$$

*là một đẳng cấu và*

$$
\sum_{i=1}^s [\hat{L}_i : \hat{K}] = n.
$$

(10)

Chứng minh cũng giống như đối với các mệnh đề tương tự trong Mệnh đề 2 (no. 2). Các dẫn chiếu

§ 7, no. 2, Theorem 1; § 5, no. 2, Corollary to Proposition 4 phải được thay bằng các dẫn chiếu sau

§ 7, no. 3, Theorem 2; Topological Vector Spaces, Chapter I,
§ 2, no. 3, Corollary 1 to Theorem 2.

Hãy nhận xét rằng hai mở rộng của $f$ lên L xác định cùng một tôpô thì bằng nhau (General Topology, Chapter IX, § 3, no. 2, Proposition 5). Cuối cùng, vì $f$ không siêu Acsimet, K có đặc số 0 và do đó căn Jacobson của $\hat{K} \otimes_K L$ bằng không.

Nhận xét
(1) Mệnh đề 11 (b) cho thấy rằng mọi mở rộng hợp thành của $\hat{K}$ và L trên K đều đẳng cấu với một trong các bổ sung $\hat{L}_i$ và rằng đó là các mở rộng hợp thành đôi một không đẳng cấu.
(2) Ta biết rằng các bổ sung $\hat{K}$ và $\hat{L}_i$ đẳng cấu với $\mathbf{R}$ hoặc $\mathbf{C}$ ($§ 6$, no. 4, Định lý 2). Nếu $\hat{K}$ đẳng cấu với $\mathbf{C}$, thì $\hat{L}_i$ cũng vậy với mọi $i$ và (10) cho thấy rằng số các mở rộng $f_i'$ là *bằng n*. Nếu $\hat{K}$ đẳng cấu với $\mathbf{R}$ (chẳng hạn nếu $K = \mathbf{Q}$), gọi $r_1$ (resp. $r_2$) là số các chỉ số $i$ sao cho $\hat{L}_i$ đẳng cấu với $\mathbf{R}$ (resp. $\mathbf{C}$); khi đó (10) có thể viết thành:

$$
r_1 + 2r_2 = n.
$$

#### Mệnh đề 12 {#ac-vi-s8-prop-12 .statement}

*Cho K là một trường, f là một giá trị tuyệt đối trên K, L là một mở rộng giả Galois của K và $f'$ và $f''$ là hai mở rộng của f lên L. Khi đó tồn tại một K-tự đẳng cấu s của L sao cho $f'' = f' \circ s$.*

Nếu $f$ là siêu mêtric, Hệ quả 1 của Mệnh đề 7 (no. 6) cho thấy rằng tồn tại một K-tự đẳng cấu s của L sao cho $f''$ và $f' \circ s$ là các giá trị tuyệt đối tương đương; khi đó tồn tại một số thực $a > 0$ sao cho $f''(x) = (f'(s(x)))^a$ với mọi $x \in L$. Nếu $f$ không tầm thường, lấy $x \in K^*$ sao cho $f(x) \neq 1$, điều này cho thấy rằng $a = 1$. Nếu $f$ là tầm thường, thì $f'$ và $f''$ cũng vậy (Hệ quả 2 của Mệnh đề 1, no. 1) và có thể lấy s là tự đẳng cấu đồng nhất.

Nếu $f$ không phải là siêu mêtric, tồn tại các Q-đẳng cấu $u', u''$ của L lên các trường con của $\mathbf{C}$ và các số mũ thực $a' > 0, a'' > 0$ sao cho $f'(x) = |u'(x)|^{a'}$ và

$$
f''(x) = |u''(x)|^{a''}
$$

với mọi $x \in L$ ($§ 6$, no. 4, Định lý 2). Lấy $x = 2$, ta thấy rằng $a' = a''$. Các hạn chế của $u'$ và $u''$ trên K được mở rộng bởi tính liên tục thành các đẳng cấu $u_1$ và $u_2$ của $\hat{K}$ lên $\mathbf{R}$ (tương ứng, $\mathbf{C}$). Khi đó $u_2 \circ \bar{u}_1^{-1}$ là một tự đẳng cấu của trường *được định giá* $\mathbf{R}$ (tương ứng, $\mathbf{C}$) và do đó là đồng nhất (tương ứng, đồng nhất hoặc tự đẳng cấu $c : \zeta \to \bar{\zeta}$). Nếu cần, thay thế $u'$ bằng $c \circ u'$, ta thấy rằng có thể giả sử các hạn chế của $u'$ và $u''$ trên K trùng nhau. Đồng nhất hóa K với một trường con của $\mathbf{C}$ bằng hạn chế chung này, $u'$ và $u''$ là các K-đẳng cấu của L lên các trường con của $\mathbf{C}$. Vì L là một mở rộng giả Galois của K, tồn tại một K-tự đẳng cấu s của L sao cho $u'' = u' \circ s$; do $a' = a''$, ta suy ra ngay lập tức rằng $f'' = f' \circ s$.

Nhận xét (3). Nếu $\hat{K}$ đẳng cấu với $\mathbf{R}$, Mệnh đề 12 cho thấy rằng mọi hoàn thành $\hat{L}_t$ của $L$ (theo ký hiệu của Mệnh đề 11) đều đẳng cấu với nhau. Do đó, với ký hiệu của Nhận xét 2 ở trên, hoặc $r_1 = n$ và $r_2 = 0$, hoặc $r_1 = 0$ và $2r_2 = n$.

### Bài tập {#ac-vi-s8-exercises}

Xem [các bài tập của § 8](exercises/s8/).
