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
content_sha256: dd514ac646f579a88647d96820bd42640f985d0b8a6994a7bea0a61e22c8cc13
translated_from: content/en/ac/VI/08_s8_extensions_of_a_valuation_to_an.md
source_content_sha256: e49f6fbfa95ed268d0719b34c59a38becfcce0b552ca780ea3e2dc144c85d20e
translation_model: gpt-5-6-mini, gpt-5-6
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

(kéo dài bằng tính liên tục ánh xạ đường chéo $L \to \prod_{i=1}^s L_i$) là toàn ánh, hạt nhân của nó là căn Jacobson của $\hat{K} \otimes_K L$ và

$$
\sum_{i=1}^s n_i \leq n.
$$

Trước hết ta chứng minh (a). Giả sử rằng v không là không thích hợp. Vì v và $\hat{v}$ (tương ứng $v'$ và $\hat{v}'$) có cùng nhóm cấp và cùng trường thặng dư (\S 5, no. 3, Mệnh đề 5 (b) và (f)), nên (4) đúng. Ta suy ra (6) từ đó bằng Bổ đề 2. Cuối cùng, không gian con-vectơ $\hat{K}$ của $\hat{L}_{v'}$ sinh bởi L là đóng (\S 5, no. 2, Hệ quả của Mệnh đề 4) và trù mật khắp nơi, do đó bằng $\hat{L}_{v'}$; điều này chứng minh (5).

Bây giờ ta chuyển sang (b). Ta vẫn có thể giả sử rằng v không là không thích hợp. Cho $(v_1', \ldots, v_r')$ là một họ hữu hạn các định giá từng đôi một độc lập trên L mở rộng v. Ảnh của L trong $\prod_{i=1}^r L_i$, theo ánh xạ đường chéo, là trù mật khắp nơi (\S 7, no. 2, Định lý 1) và $\prod_{i=1}^r L_i$ là trù mật trong $\prod_{i=1}^r \hat{L}_i$. Do đó ảnh chính tắc của $\hat{K} \otimes_K L$ trong $\prod_{i=1}^r \hat{L}_i$ là trù mật khắp nơi. Mặt khác ảnh này là một không gian con-vectơ $\hat{K}$ của $\prod_{i=1}^r \hat{L}_i$; vì $\prod_{i=1}^r \hat{L}_i$ có số chiều hữu hạn trên $\hat{K}$ theo (5), ảnh của $\hat{K} \otimes_K L$ là đóng (\S 5, no. 2, Hệ quả của Mệnh đề 4) và do đó bằng $\prod_{i=1}^r \hat{L}_i$. Vì số chiều của $\hat{K} \otimes_K L$ trên K là n, nên $\sum_{i=1}^r n_i \leq n$. Điều này đặc biệt cho thấy số nguyên r bị chặn trên bởi n và chứng minh mệnh đề đầu tiên của (b).

Bây giờ ta lấy $(v_1', \ldots, v_s')$ như trong mệnh đề. Tính chất rằng

$$
\phi : \hat{K} \otimes_K L \to \prod_{i=1}^s \hat{L}_i
$$

là toàn ánh và quan hệ (7) đã được chứng minh. Còn lại cần kiểm tra rằng hạt nhân n của $\phi$ là căn Jacobson $t$ của $\hat{K} \otimes_K L$. Vì $\prod_{i=1}^s \hat{L}_i$ là nửa đơn, nên $t \subset n$. Mặt khác, với mọi iđêan cực đại m của $\hat{K} \otimes_K L$, trường thương $L(m) = (\hat{K} \otimes_K L)/m$ là một mở rộng hợp thành của $\hat{K}$ và L trên K (Algebra,

Chapter VIII, § 8, Mệnh đề 1). Có một định giá w trên L(m) mở rộng $\vartheta$ (§ 3, no. 3, Mệnh đề 5); hạn chế $v'$ của w trên L mở rộng $v$. Vì $[L(m): \hat{K}]$ là hữu hạn, $L(m)$ là đầy đủ đối với w ($\S 5$, no. 2, Mệnh đề 4). Bây giờ bao đóng của L trong $L(m)$ là một trường chứa $\mathbf{K}$ và L và do đó bằng $L(m)$. Do đó $L(m)$ được đồng nhất với phần bù đầy đủ $\hat{L}_{v'}$ và m là hạt nhân của ánh xạ chính tắc của $\hat{K} \otimes_K L$ lên $\hat{L}_{v'}$. Bây giờ, theo giả thiết, tồn tại một chỉ số $i$ sao cho $v'$ và $v'_i$ phụ thuộc; do đó $L_{v'} = L_i$ ($\S 7$, no. 2, Mệnh đề 3). Vì vậy $n \subset m$, điều này chứng minh rằng $n \subset r$ và hoàn tất chứng minh.

#### Hệ quả 1 {#ac-vi-s8-prop-2-cor-1 .statement}

*Nếu K đầy đủ đối với v và v không là không thích hợp, hai định giá trên L mở rộng v là phụ thuộc.*

Điều này suy ra vì $\hat{K} \otimes_K L = L$.

#### Hệ quả 2 {#ac-vi-s8-prop-2-cor-2 .statement}

*Nếu $\hat{K}$ hoặc L là tách được trên K, ánh xạ chính tắc*

$$
\phi : \hat{K} \otimes_K L \to \prod_{i=1}^s \hat{L}_i
$$

*là một đẳng cấu*.

Căn Jacobson của $\hat{K} \otimes_K L$ khi đó là không (*Algebra*, Chapter VIII, § 7, no. 3, Định lý 1).

#### Nhận xét {#ac-vi-s8-n2-rem-1 .statement}

Mệnh đề 2 (b) chỉ ra rằng mọi mở rộng hợp thành của $\hat{K}$ và L trên K (*Algebra*, Chapter VIII, § 8) là đẳng cấu với một trong các phần bù đầy đủ $\hat{L}_i$ và rằng các phần bù này là các mở rộng hợp thành không có hai cái nào đẳng cấu.

### 3. QUAN HỆ $\sum_i e_i f_i \leq n$

Cho K là một trường, $v$ là một giá trị hóa trên K và L là một mở rộng hữu hạn của K có bậc $n$. Cho $(v'_1, \ldots, v'_r)$ là các giá trị hóa trên L mở rộng $v$ *không có hai giá trị nào trong chúng là tương đương; nếu* chúng *độc lập* (điều này luôn đúng nếu $v$ có chiều cao 1), thì

$$
\sum_{i \in I} e(v'_i|v) f(v'_i|v) \leq n
$$

theo Mệnh đề 2 (các công thức (6) và (7)). Ta sẽ thấy rằng kết quả này đúng trong trường hợp tổng quát. Nói chính xác hơn:

#### Định lý 1 {#ac-vi-s8-thm-1 .statement}

*Cho K là một trường, v là một giá trị hóa trên K và L là một mở rộng hữu hạn của K có bậc n. Khi đó:*

(a) *Mọi hệ đầy đủ $(v'_i)_{i \in I}$ các mở rộng của v lên L đều hữu hạn.*

(b) $\sum_{i \in I} e(v'_i|v) f(v'_i|v) \leq n$ và a fortiori $\operatorname{Card}(I) \leq n$

(c) *Không có hai vành nào trong các vành của $v'_i$ so sánh được theo quan hệ bao hàm.*

Vì định lý là tầm thường nếu $v$ là không đúng, ta sẽ giả sử rằng $v$ không phải là không đúng. Cho $(v'_1, \ldots, v'_s)$ là một họ hữu hạn bất kỳ các giá trị hóa trên L mở rộng $v$, không

QUAN HỆ $\sum_i e_i f_i \leq n$

có hai cái nào tương đương. Trước hết ta sẽ chứng minh rằng $\sum_{i=1}^s e(v'_i/v)f(v'_i/v) \leq n$. Điều này sẽ chứng minh (a) và (b).

Ta lập luận bằng quy nạp theo s và do đó giả sử rằng bất đẳng thức đã được thiết lập cho trường hợp có 0, 1, ..., s - 1 giá trị hóa. Ta phân biệt hai trường hợp.

(1) Giả sử rằng tồn tại ít nhất hai giá trị hóa độc lập $v'_i$. Khi đó tồn tại (\S 7, no. 2, Nhận xét 1) một phân hoạch $[1, s] = I_1 \cup \ldots \cup I_t$ của $[1, s]$ sao cho:
(i) để $v'_i$ và $v'_j$ phụ thuộc, điều kiện cần và đủ là $i$ và $j$ thuộc cùng một $I_k$;
(ii) Card$(I_k) < s$ với mọi $k$.

Ta chọn trong mỗi $I_k$ một chỉ số $i(k)$. Ký hiệu $\hat{L}_{i(k)}$ là phép đầy đủ của L đối với $v'_{i(k)}$ và $n(k) = [\hat{L}_{i(k)} : \hat{K}]$. Với mọi $i \in I_k$, $v'_i$ xác định trên $L$ cùng một tôpô như $v'_{i(k)}$ (\S 7, no. 2, Mệnh đề 3) và do đó có thể được mở rộng thành một giá trị hóa $\bar{v}'_i$ trên $\hat{L}_{i(k)}$ mà hạn chế của nó lên $\hat{K}$ là 0. Vì không có hai giá trị nào trong các $v'_i$ với $i \in I$, là tương đương, điều tương tự cũng đúng đối với các $\bar{v}'_i$. Giả thiết quy nạp áp dụng cho cặp có thứ tự $(\hat{K}, \hat{L}_{i(k)})$ cho thấy, nhờ Mệnh đề 2 (a), công thức (4), rằng $\sum_{i \in I_k} e(v'_i/v)f(v'_i/v) \leq n(k)$. Vì $\sum_{k=1}^t n(k) \leq n$ (Mệnh đề 2 (b), công thức (7)), chắc chắn $\sum_{i=1}^s e(v'_i/v)f(v'_i/v) \leq n$.

(2) Bây giờ ta chuyển sang trường hợp trong đó hai phần tử bất kỳ nào của $v'_i$ cũng phụ thuộc nhau. Gọi $A'_i$ là vành của $v'_i$ ($1 \leq i \leq s$); ký hiệu $A$ là vành của $v$, ta có $A'_i \cap K = A$ với mọi $i$. Gọi $B'$ là vành con của $L$ sinh bởi $A'_1, \ldots, A'_s$; ta ký hiệu $B = B' \cap K$; khi đó $B \supseteq A$. Khi đó $B$ là vành của một định giá $w$ trên $K$ và $B'$ là vành của một định giá $w'$ không suy biến và mở rộng $w$ (\S 7, no. 2, Mệnh đề 4); trường $\kappa(B')$ là một mở rộng của $\kappa(B)$ có bậc $f(w'/w)$. Xét các ảnh chính tắc $\bar{A}'_i, \bar{A}$ của $A'_i$ và $A$ trong $\kappa(B')$; khi đó $\bar{A}$ là vành của một định giá $\bar{v}$ trên $\kappa(B)$ và các $\bar{A}'_i$ là các vành của các định giá $\bar{v}'_i$ trên $\kappa(B')$ mở rộng $\bar{v}$. Vì các $A'_i$ sinh ra $B'$, các $\bar{A}'_i$ sinh ra $\kappa(B')$ và do đó các $\bar{v}'_i$ không phải tất cả đều phụ thuộc nhau (\S 7, no. 2, Mệnh đề 4). Từ phần đầu của chứng minh,

$$
\sum_{i=1}^s e(\bar{v}'_i/\bar{v})f(\bar{v}'_i/\bar{v}) \leq [\kappa(B') : \kappa(B)] = f(w'/w)
$$

và do đó

$$
\sum_{i=1}^s e(w'/w)e(\bar{v}'_i/\bar{v})f(\bar{v}'_i/\bar{v}) \leq e(w'/w)f(w'/w) \leq n \quad \text{(no. 1, Bổ đề 1).}
$$

Chứng minh của (a) và (b) vì thế sẽ hoàn tất nếu ta chứng minh rằng

$$
f(\bar{v}'_i/\bar{v}) = f(\bar{v}'_i/v), \quad e(w'/w)e(\bar{v}'_i/\bar{v}) = e(v'_i/v).
$$

Về điều này, ta nhận xét rằng $v$ và $\bar{v}$ (tương ứng $v'_i$ và $\bar{v}'_i$) có cùng trường thặng dư (§ 4, no. 1, Hệ quả của Mệnh đề 2); điều này chứng minh đẳng thức thứ nhất. Đối với đẳng thức thứ hai, theo Nhận xét trong §4, no. 3, ta có biểu đồ giao hoán sau, trong đó các hàng là các dãy khớp và các mũi tên đứng biểu diễn các đơn ánh chính tắc:

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

Để hoàn tất chứng minh của Định lý 1, còn phải chứng minh (c). Nếu vành của $v_i'$ chứa vành của $v_j'$, $\Gamma_{v_i'}$ được đồng nhất với một nhóm thương $\Gamma_{v_j'}/H$, $H$ là một nhóm con cô lập (§ 4, no. 3). Vì ánh xạ chính tắc hợp thành

$$
\Gamma_v \to \Gamma_{v_j} \to \Gamma_{v_j'}/H = \Gamma_{v_i'}
$$

là đơn ánh, $H \cap \Gamma_v = \{0\}$, do đó $H = \{0\}$ (Bổ đề 3, no. 1). Khi đó $v_i'$ và $v_j'$ là tương đương, do đó $i = j$.

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

Các iđêan của $A'$ chứa $mA'$ và phân biệt với $A'$ tương ứng với các tập con lớn của $\Gamma_w$ gồm các phần tử >0 và chứa các phần tử >0 của $\Gamma_v$ (\S 3, no. 5, Hệ quả của Mệnh đề 7). Do đó chúng có số lượng bằng $\varepsilon(w/v)$ và, vì chúng tạo thành một tập sắp thứ tự toàn phần theo quan hệ bao hàm, số này bằng độ dài của vành thương $A'/mA'$. Bây giờ một môđun có độ dài 1 trên $A'$ là một không gian vectơ chiều 1 trên $A'/m'$ và do đó là một môđun có độ dài $f(w/v)$ trên $A$; do đó, vì $A'/mA'$ có độ dài $\varepsilon(w/v)$ trên $A'$, nó có độ dài $\varepsilon(w/v) f(w/v)$ trên $A$, tức là trên $A/m$.

### 5. QUAN HỆ $\sum_i e_i f_i = n$

#### Mệnh đề 5 {#ac-vi-s8-prop-5 .statement}

*Cho* $K$ *là một trường, v một định giá trên* $K$, $A$ *là vành của nó, m là iđêan của nó, L một mở rộng hữu hạn của* $K$ *có bậc* $n$, $B$ *là bao đóng nguyên của* $A$ *trong* $L$ *và* $(v'_i)_{1 \leq i \leq s}$ *là một hệ đầy đủ các mở rộng của* $v$ *đến* $L$. *Khi đó*

$$
[B/mB : A/m] = \sum_{i=1}^s \varepsilon(v'_i/v) f(v'_i/v).
$$

Gọi $A_i$ là vành của $v'_i$; khi đó $A_i = B_{m_i}$ trong đó $m_i$ chạy qua họ các iđêan cực đại của $B$ (no. 3, Nhận xét). Gọi $q_i$ là bão hòa của $mB$ đối với $m_i$ (Chương II, \S 2, no. 4). Theo Chương V, Hệ quả 3 của Mệnh đề 1, no. 1, \S 2, đồng cấu chính tắc $B/mB \to \prod_{i=1}^s B/q_i$ là một đẳng cấu và $m_i$ là iđêan cực đại duy nhất của B chứa $q_i$. Do đó $B/q_i$ đẳng cấu chính tắc với $(B/q_i)_{m_i}$ (Chương II, § 3, no. 3, Mệnh đề 8), tức là với
$$
B_{m_i}/mB_{m_i} = A_i/mA_i.
$$
Vì vậy có một đẳng cấu chính tắc $B/mB \to \prod_{i=1}^s A_i/mA_i$, do đó có kết quả theo Mệnh đề 4 của no. 4.

#### Hệ quả {#ac-vi-s8-n5-cor-1 .statement}

*Với cùng các giả thiết và ký hiệu,
$$
[B/mB : A/m] = \sum_{i=1}^s \varepsilon(v'_i/v) f(v'_i/v) \leq \sum_{i=1}^s \varepsilon(v'_i/v) f(v'_i/v) \leq n.
$$
Ta biết rằng $\varepsilon(v'_i/v) \leq \varepsilon(v'_i/v)$ (no. 4, Hệ quả của Mệnh đề 3) và $\sum_{i=1}^s \varepsilon(v'_i/v) f(v'_i/v) \leq n$ (no. 3, Định lý 1).

#### Định lý 2 {#ac-vi-s8-thm-2 .statement}

*Với các giả thiết và ký hiệu của Mệnh đề 5, các điều kiện sau là tương đương :
(a) B là một A-môđun sinh hữu hạn;
(b) B là một A-môđun tự do;
(c) $[B/mB : A/m] = n;$
(d) $\sum_{i=1}^n \varepsilon(v'_i/v) f(v'_i/v) = n$ và $\varepsilon(v'_i/v) = \varepsilon(v'_i/v)$ với mọi i.

Sự tương đương của (a) và (b) suy ra từ Bổ đề 1, § 3, no. 6. Rõ ràng (b) kéo theo (c) (*Đại số*, Chương 11, § 1, no. 5, công thức (19)). Sự tương đương của (c) và (d) suy ra từ Hệ quả của Mệnh đề 5. Còn lại phải chứng minh rằng (c) kéo theo (b).

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

Vì không có hai $v'_i$ nào tương đương và chúng có chiều cao 1, chúng độc lập và Mệnh đề 2 của no. 2 cho thấy do đó rằng $e(v'_i/v) f(v'_i/v) \leq n_i$ với mọi $i$ và $\sum_{i=1}^s n_i \leq n$. Mệnh đề đầu tiên do đó suy ra từ các bất đẳng thức này và quan hệ $\sum_{i=1}^s e(v'_i/v) f(v'_i/v) = n$. Dưới đẳng cấu $\phi$, tự đồng cấu $z \mapsto z(1 \otimes x)$ của $\hat{K} \otimes_K L$ (với $x \in L$) được biến thành tự đồng cấu của $\prod_{i=1}^s \hat{L}_i$ giữ bất biến từng nhân tử và thu gọn trên mỗi nhân tử thành phép nhân với $x$ ($L$ được nhúng một cách chính tắc vào phần đầy đủ của nó $\hat{L}_i$); do đó suy ra mệnh đề liên quan đến đa thức đặc trưng của $x$ và hai công thức đầu tiên của (9). Cuối cùng, cho E là một mở rộng quasi-Galois hữu hạn của $\hat{K}$, chứa $\hat{L}_i$; vì $\hat{K}$ là đầy đủ và $\hat{\nu}$ có chiều cao 1, chỉ tồn tại duy nhất một định giá (tới tương đương) $w$ trên E mở rộng $\hat{\nu}$ (no. 2, Hệ quả 1 của Mệnh đề 2); khi đó, với mọi tự đẳng cấu $\hat{K}$ $\sigma$ của E, $w(\sigma(x)) = v'_i(x)$. Do đó
$$
\vartheta(N_{\hat{L}_i/\hat{K}}(x)) = n_i v'_i(x)
$$
(Đại số, Chương VIII, § 12, no. 2, công thức (15)), điều này chứng minh công thức của (9).

#### Hệ quả 4 {#ac-vi-s8-thm-2-cor-4 .statement}

*Dưới các giả thiết của Hệ quả 3, nếu L là một mở rộng tách được của K, mỗi $\hat{L}_i$ là một mở rộng tách được của $\hat{K}$. Nếu thêm nữa L là một mở rộng Galois của K với nhóm Galois $\mathcal{G}$ và $\mathcal{G}_i$ ký hiệu nhóm phân tích của iđêan của $v'_i$ trong B (Chương V, § 2, no. 2, Định nghĩa 2), thì $\hat{L}_i$ là một mở rộng Galois của $\hat{K}$ có nhóm Galois đẳng cấu với $\mathcal{G}_i$.*

Rõ ràng $\hat{L}_i = \hat{K}(L)$; do đó, nếu L là tách được trên K, $\hat{L}_i$ là tách được trên $\hat{K}$ (Đại số, Chương V, § 7, no. 6, Mệnh đề 10). Giả sử bây giờ rằng L là Galois. Mọi tự đẳng cấu $\sigma \in \mathcal{G}_i$ đều liên tục trên L với tôpô được xác định bởi $v'_i$, sự kiện rằng không có hai iđêan nào của các $v'_i$ so sánh được đối với quan hệ bao hàm (§ 7, no. 2, Hệ quả 1 của Định lý 1) tất yếu kéo theo rằng $v'_i = v'_i \circ \sigma$ theo định nghĩa của $\mathcal{G}_i$; do đó $\sigma$ có thể được mở rộng bởi tính liên tục thành một tự đẳng cấu $\hat{K}$ $\hat{\sigma}$ của $\hat{L}_i$. Điều này chứng minh rằng số các tự đẳng cấu $\hat{K}$ của $\hat{L}_i$ ít nhất bằng $\mathrm{Card}(\mathcal{G}_i)$. Nhưng vì các định giá $v'_i$ từng đôi một liên hợp dưới $\mathcal{G}$ (Chương V, § 2, no. 3, Mệnh đề 6), $s = (\mathcal{G}_i)$, do đó
$$
\mathrm{Card}(\mathcal{G}_i) = n/s \leq n.
$$
và mặt khác $n = sn$, theo Hệ quả 3; điều này chứng minh rằng $\hat{L}_i$ là một mở rộng Galois của $\hat{K}$ và rằng các mở rộng bởi tính liên tục của các tự đẳng cấu $\sigma \in \mathcal{G}_i$ là các tự đẳng cấu $\hat{K}$ duy nhất của $\hat{L}_i$.

*Nhận xét (2)*. Một phần các kết quả trên mở rộng được sang trường hợp các định giá trên một trường K *không nhất thiết giao hoán* (xem § 3, no. 1). Cho L là một mở rộng trường của K và cho $v'$ là một định giá trên L, $v$ là hạn chế của nó trên K và A' và A là các vành tương ứng của các định giá $v'$ và $v$; khi đó có xác định một chỉ số phân nhánh $e(v'/v)$ như trong no. 1; mặt khác, $\kappa(A)$ được đồng nhất với một trường con của $\kappa(A')$ và hạng thặng dư (trái) của $v'$ đối với $v$ được định nghĩa là số $f(v'/v)$ bằng số chiều của không gian vectơ trái $\kappa(A)$-không gian $\kappa(A')$, nếu chiều này hữu hạn, và $+\infty$ trong trường hợp đối. Khi đó, nếu L là một không gian vectơ trái K có số chiều hữu hạn $n$, Bổ đề 2 của no. 1 và chứng minh của nó vẫn giữ nguyên. Hơn nữa, nếu K đầy đủ đối với $v$, các mệnh đề của Hệ quả 2 của Định lý 2 của no. 5 (ngoài sự tồn tại của $u'$) cũng đúng ($n$ ký hiệu chiều của L như một không gian vectơ trái K) với chứng minh sau:

Trước hết, tôpô xác định bởi $v'$ trên L là Hausdorff và tương thích với cấu trúc không gian vectơ trái K của nó và do đó hai mở rộng của $v$ lên L cho cùng một tôpô trên L ($\S 5$, no. 2, Mệnh đề 4), điều này chứng minh rằng các mở rộng này là như nhau đến tương đương ($\S 6$, no. 2). Tiếp theo ta chứng minh rằng, nếu $m = m(A)$, $A'/mA'$ là một không gian vectơ trái $(A/m)$ có số chiều $e(v'/v) f(v'/v)$. Viết $e = e(v'/v)$, ta có thể giả sử rằng $v(K^*) = Z$ và $v'(L^*) = e^{-1}Z$; gọi $u'$ là một phần tử của L sao cho $v'(u') = e^{-1}$ và $u$ là một phần tử của K sao cho $v(u) = 1$; do đó $u = z{u'}^e$, trong đó $z \in L$ là phần tử sao cho $v'(z) = 0$. Vì m được sinh bởi $u$ (như một iđêan trái hoặc phải của A), $mA' = {u'}^eA' = A'{u'}^e$ và chỉ cần chứng minh rằng, với $0 \leq k \leq e - 1$, $A'{u'}^k/A'{u'}^{k+1}$ là một không gian vectơ trái $(A/m)$ có số chiều $f(v'/v)$. Nhưng $t \mapsto t{u'}^k$ là một đẳng cấu của A-môđun trái A lên A-môđun trái $A'{u'}^k$ biến $A'u'$ thành $A'{u'}^{k+1}$ và do đó bằng cách lấy thương cho một $(A/m)$-đẳng cấu của $A'/A'u'$ lên $A'{u'}^k/A'{u'}^{k+1}$, do đó mệnh đề của ta theo định nghĩa của $f(v'/v)$, $u'$ sinh iđêan cực đại của $A'$. Chứng minh được hoàn tất như trong trường hợp K và L giao hoán (sự kiện rằng một A-môđun xoắn không có xoắn sinh hữu hạn là tự do được chứng minh như trong $\S 3$, no. 6, Bổ đề 1).

### 6. CÁC VÀNH ĐỊNH GIÁ TRONG MỘT MỞ RỘNG ĐẠI SỐ

#### Mệnh đề 6 {#ac-vi-s8-prop-6 .statement}

Cho K là một trường, $v$ là một định giá trên K, A là vành của nó, L là một mở rộng đại số của K và $A'$ là bao đóng nguyên của A trong L. Cho 23 là tập hợp các vành định giá trên L mở rộng $v$ và $\mathfrak{M}'$ là tập hợp các iđêan cực đại của $A'$. Khi đó ánh xạ $V \mapsto m(V) \cap A'$ là một song ánh từ 23 lên $\mathfrak{M}'$ và $m' \mapsto A'_{m'}$ là song ánh ngược.

Mọi iđêan cực đại $m'$ của $A'$ đều sao cho $m' \cap A$ là iđêan cực đại của A (Chương V, § 2, no. 1, Mệnh đề 1) và $A'_{m'}$ bị trội bởi một vành định giá V của L (do đó nó là vành của một định giá trên L mở rộng $v$) ($\S 1$, no. 2, Hệ quả của Định lý 2). Trường L là hợp của một họ có hướng các mở rộng con K, của L hữu hạn trên K và sẽ đủ, để thấy rằng $V = A'_{m'}$, phải chứng minh rằng $V \cap K = A'_{m'} \cap K$, với mọi $\alpha$. Bây giờ, nếu ta viết $A'_\alpha = A' \cap K_\alpha$, thì $A'_\alpha$ là bao đóng nguyên của A trong K, và do đó là giao của các vành của các định giá trên K, mở rộng $v$ và các vành này $V_\alpha$ có số lượng hữu hạn và là các vành địa phương $(A'_\alpha)_{i|m_\alpha}$ của $A'_\alpha$ ($1 \leq i \leq n$), trong đó các $m'_{i\alpha}$ là các iđêan cực đại phân biệt của $A'_\alpha$ (no. 3, Nhận xét); nhưng $m' \cap A'_\alpha$ là một trong các $m'_{i\alpha}$ và $V \cap K_\alpha$ do đó bằng vành địa phương tương ứng $(A'_\alpha)_{m'_{i\alpha}} \subset A'_{m'}$, điều này hoàn thành chứng minh rằng $V = A'_{m'}$. Ngược lại, nếu $V \in \mathfrak{V}$, thì $A' \subset V$ (\$3, no. 3, Mệnh đề 6) và, nếu $m' = m(V) \cap A'$, thì $m' \cap A = m$, do đó $m'$ là một iđêan cực đại của $A'$ (Chương V, § 2, no. 1, Mệnh đề 1) và lập luận trên cho thấy rằng $V = A'_{m'}$.

#### Mệnh đề 7 {#ac-vi-s8-prop-7 .statement}

*Cho K là một trường, L một mở rộng quasi-Galois của K và f và $f'$ là các nơi của L với giá trị trong cùng một trường F. Giả sử rằng các hạn chế của f và $f'$ lên K trùng nhau. Khi đó tồn tại một tự đẳng cấu K của L sao cho $f' = f \circ s$.*

Gọi A là vành của nơi của K là hạn chế chung của f và $f'$. Các vành của f và $f'$ chứa bao đóng nguyên $A'$ của A trong L (\$ 1, no. 3, Hệ quả 3 của Định lý 3) và do đó (Chương V, § 2, no. 3, Hệ quả 1 của Mệnh đề 6) tồn tại một tự đẳng cấu K của L sao cho các hạn chế của f và $f \circ s$ lên $A'$ bằng nhau; nếu $m'$ là hạt nhân chung của các hạn chế này, $m' \cap A$ là iđêan cực đại của A, do đó $m'$ là một iđêan cực đại của $A'$ và các nơi $f'$ và $f \circ s$ trùng nhau trên vành $A'_{m'}$; nhưng theo Mệnh đề 6 vành định giá duy nhất của L trội lên $A'_{m'}$ là chính vành $A'_{m'}$ và do đó các vành của các nơi $f'$ và $f \circ s$ là như nhau.

#### Hệ quả 1 {#ac-vi-s8-prop-7-cor-1 .statement}

*Cho K là một trường, v một định giá trên K, L một mở rộng quasi-Galois của K và $v'$ và $v''$ là hai mở rộng của v lên L. Khi đó tồn tại một tự đẳng cấu K của L sao cho $v''$ tương đương với $v' \circ s$.*

Gọi $f'$ và $f''$ là các nơi của K liên kết với $v'$ và $v''$; thay thế chúng nếu cần bằng các nơi tương đương, ta có thể giả sử rằng cả hai đều nhận giá trị của chúng trong bao đóng đại số của trường thặng dư của v (no. 1, Mệnh đề 1). Khi đó tồn tại một tự đẳng cấu K của L sao cho $f'' = f' \circ s$ (Mệnh đề 7); do đó $v''$ tương đương với $v' \circ s$ theo sự tương ứng giữa các nơi và các định giá (\$ 3, no. 3).

#### Hệ quả 2 {#ac-vi-s8-prop-7-cor-2 .statement}

*Cho K là một trường, f một nơi của K (tương ứng v một định giá trên K) và L một mở rộng thuần phóng xạ của K. Khi đó tất cả các mở rộng của f (tương ứng v) lên L đều tương đương.*

L là một mở rộng quasi-Galois và tự đẳng cấu duy nhất của nó là đồng nhất. Hệ quả 2 do đó suy ra từ Mệnh đề 7 (tương ứng Hệ quả 1).

#### Mệnh đề 8 {#ac-vi-s8-prop-8 .statement}

*Cho K là một trường, v là một giá trị định chuẩn trên K, L là một mở rộng quasi-Galois hữu hạn của K có bậc n và $(v'_i)_{1 \leq i \leq g}$ là một hệ đầy đủ các mở rộng của v lên L. Khi đó $e(v'_i/v)$ và $f(v'_i/v)$ có các giá trị e và $\mathfrak{f}$ độc lập với i. Khi đó $ef g \leq n$. Nếu bao đóng nguyên trong L của vành A của v là một A-môđun sinh hữu hạn, thì $ef g = n$.*

Điều này suy ra ngay lập tức từ các Định lý 1 (no. 3) và 2 (no. 5).

### 7. MỞ RỘNG CÁC GIÁ TRỊ TUYỆT ĐỐI

#### Mệnh đề 9 {#ac-vi-s8-prop-9 .statement}

*Cho K là một trường, L là một mở rộng đại số của K và $\mathfrak{f}$ là một giá trị tuyệt đối trên K. Khi đó $\mathfrak{f}$ có thể được mở rộng thành một giá trị tuyệt đối trên L.*

Trước hết giả sử rằng tồn tại một giá trị định chuẩn $v$ trên $K$ với các giá trị thực sao cho $f(x) = e^{-v(x)}$. Tồn tại một giá trị định chuẩn $v'$ trên $L$ mà hạn chế của nó trên $K$ tương đương với $v$ ($\S 3$, no. 3, Mệnh đề 5). Khi đó $v'$ có chiều cao 0 hoặc 1 (no. 1, Hệ quả 2 của Mệnh đề 1) và do đó có thể giả sử rằng nó có các giá trị thực. Hạn chế của ánh xạ $x \mapsto e^{-v'(x)}$ trên $K$ là một giá trị tuyệt đối tương đương với $f$ và vì thế có dạng $f^s$ với $s > 0$ (*Tôpô đại cương*, Chương IX, $\S 3$, no. 2, Mệnh đề 5). Ta kết luận rằng

$$
x \mapsto e^{-v'(x)/s}
$$

là một giá trị tuyệt đối trên $L$ mở rộng $f$.

Bây giờ giả sử rằng $f$ không là phi Archimedes. Khi đó $K$ được đồng nhất với một trường con của $\mathbf{C}$ sao cho $f(x) = |x|^s$ trong đó $0 \leq s \leq 1$ ($\S 6$, no. 4, Định lý 2). Vì $\mathbf{C}$ là đóng đại số, $L$ được đồng nhất với một trường con của $\mathbf{C}$ và giá trị tuyệt đối $x \mapsto |x|^s$ mở rộng $f$.

#### Mệnh đề 10 {#ac-vi-s8-prop-10 .statement}

*Cho $K$ là một trường, $f$ là một giá trị tuyệt đối trên $K$ sao cho $K$ đầy đủ và không rời rạc đối với $f$ và $L$ là một mở rộng đại số của $K$. Khi đó $f$ có thể được mở rộng duy nhất thành một giá trị tuyệt đối $f'$ trên $L$ và, nếu $L$ có bậc hữu hạn $n$, thì*

$$
f'(x) = (f(N_{L/K}(x)))^{1/n}
$$

*đối với mọi* $x \in L$.

Sự tồn tại của $f'$ suy ra từ Mệnh đề 9 và tính duy nhất của nó (trên mọi mở rộng con hữu hạn của $L$ và do đó trên toàn bộ $L$) suy ra từ Bổ đề 2 của $\S 6$, no. 4. Gọi $f'$ là mở rộng duy nhất của f tới bao đóng đại số của $K$ và giả sử $L$ có bậc hữu hạn $n$. Ta biết rằng $N_{L/K}(x) = \prod_{i=1}^n x_i$, trong đó mỗi $x_i$ là một phần tử liên hợp của $x$ trên $K$ (*Đại số*, Chương VIII, $\S 12$, no. 2, Mệnh đề 4). Do tính duy nhất của $f'$, $f'(x_i) = f'(x)$ với mọi $i$, do đó có công thức đã nêu.

#### Mệnh đề 11 {#ac-vi-s8-prop-11 .statement}

*Cho $K$ là một trường, $f$ là một giá trị tuyệt đối không ultrametric trên $K$, $\hat{K}$ là bao đầy đủ của $K$ đối với $f$, $\hat{f}$ là mở rộng liên tục của f tới $\hat{K}$ và $L$ là một mở rộng hữu hạn của $K$ có bậc $n$.

(a) *Cho $f'$ là một giá trị tuyệt đối trên $L$ mở rộng $f$; ký hiệu $\hat{L}_{f'}$ là bao đầy đủ của $L$ đối với $f'$ và đồng nhất $\hat{K}$ với bao đóng của $K$ trong $\hat{L}_{f'}$; khi đó* $[\hat{L}_{f'} : K] \leq n$.

(b) *Các giá trị tuyệt đối trên $L$ mở rộng $f$ có số lượng hữu hạn. Nếu chúng được ký hiệu bởi* $f'_1, \ldots, f'_s$ *và bao đầy đủ của $L$ đối với* $f'_i$ *bởi* $\hat{L}_i$, *ánh xạ chính tắc*

$$
\hat{K} \otimes_K L \to \prod_{i=1}^s \hat{L}_i
$$

*là một đẳng cấu và*

$$
\sum_{i=1}^s [\hat{L}_i : \hat{K}] = n.
$$

(10)

Chứng minh cũng giống như chứng minh của các khẳng định tương tự trong Mệnh đề 2 (no. 2). Các tham chiếu

§ 7, no. 2, Định lý 1; § 5, no. 2, Hệ quả của Mệnh đề 4 nên được thay bằng các tham chiếu sau

§ 7, no. 3, Định lý 2; Không gian vectơ tôpô, Chương I,
§ 2, no. 3, Hệ quả 1 của Định lý 2.

Chú ý rằng hai mở rộng của f tới L xác định cùng một tôpô thì bằng nhau (Tôpô đại cương, Chương IX, § 3, no. 2, Mệnh đề 5). Cuối cùng, vì $f$ không ultrametric, K có đặc số 0 và do đó căn Jacobson của $\hat{K} \otimes_K L$ là không.

Nhận xét
(1) Mệnh đề 11 (b) chỉ ra rằng mọi mở rộng hợp thành của $\hat{K}$ và L trên K đều đẳng cấu với một trong các phép hoàn thành $\hat{L}_i$ và rằng các mở rộng này là những mở rộng hợp thành mà không có hai cái nào trong chúng đẳng cấu với nhau.
(2) Ta biết rằng các phép hoàn thành $\hat{K}$ và $\hat{L}_i$ đẳng cấu với $\mathbf{R}$ hoặc $\mathbf{C}$ ($\S 6$, no. 4, Định lý 2). Nếu $\hat{K}$ đẳng cấu với $\mathbf{C}$, thì $\hat{L}_i$ cũng vậy với mọi $i$ và (10) chỉ ra rằng số các mở rộng $f_i'$ là *bằng n*. Nếu $\hat{K}$ đẳng cấu với $\mathbf{R}$ (chẳng hạn nếu $K = \mathbf{Q}$), gọi $r_1$ (resp. $r_2$) là số các chỉ số $i$ sao cho $\hat{L}_i$ đẳng cấu với $\mathbf{R}$ (resp. $\mathbf{C}$); khi đó (10) có thể được viết:

$$
r_1 + 2r_2 = n.
$$

#### Mệnh đề 12 {#ac-vi-s8-prop-12 .statement}

*Cho K là một trường, f là một giá trị tuyệt đối trên K, L là một mở rộng quasi-Galois của K và $f'$ và $f''$ là hai mở rộng của f tới L. Khi đó tồn tại một tự đẳng cấu K s của L sao cho $f'' = f' \circ s$.*

Nếu $f$ là ultrametric, Hệ quả 1 của Mệnh đề 7 (no. 6) chỉ ra rằng tồn tại một tự đẳng cấu K s của L sao cho $f''$ và $f' \circ s$ là các giá trị tuyệt đối tương đương; khi đó tồn tại một số thực $a > 0$ sao cho $f''(x) = (f'(s(x)))^a$ với mọi $x \in L$. Nếu $f$ không suy biến, lấy $x \in K^*$ sao cho $f(x) \neq 1$, điều này chỉ ra rằng $a = 1$. Nếu $f$ suy biến, thì $f'$ và $f''$ cũng vậy (Hệ quả 2 của Mệnh đề 1, no. 1) và s có thể được chọn là tự đẳng cấu đồng nhất.

Nếu $f$ không ultrametric, tồn tại các đẳng cấu Q $u', u''$ của L lên các trường con của $\mathbf{C}$ và các số mũ thực $a' > 0, a'' > 0$ sao cho $f'(x) = |u'(x)|^{a'}$ và

$$
f''(x) = |u''(x)|^{a''}
$$

for all $x \in L$ ($\S 6$, no. 4, Định lý 2). Lấy $x = 2$, ta thấy rằng $a' = a''$. Các hạn chế của $u'$ và $u''$ lên K mở rộng bằng tính liên tục thành các đẳng cấu $u_1$ và $u_2$ của $\hat{K}$ lên $\mathbf{R}$ (resp. $\mathbf{C}$). Khi đó $u_2 \circ \bar{u}_1^{-1}$ là một tự đẳng cấu của trường *được định giá* $\mathbf{R}$ (resp. $\mathbf{C}$) và do đó là đồng nhất (resp. đồng nhất hoặc tự đẳng cấu $c : \zeta \to \bar{\zeta}$). Thay thế nếu cần $u'$ bởi $c \circ u'$, ta thấy rằng các hạn chế của $u'$ và $u''$ lên K có thể được giả thiết là trùng nhau. Đồng nhất hóa K với một trường con của $\mathbf{C}$ bằng hạn chế chung này, $u'$ và $u''$ là các K-đẳng cấu của L lên các trường con của $\mathbf{C}$. Vì L là một mở rộng Galois suy rộng của K, tồn tại một K-tự đẳng cấu s của L sao cho $u'' = u' \circ s$; vì $a' = a''$, ta suy ra ngay lập tức rằng $f'' = f' \circ s$.

Nhận xét (3). Nếu $\hat{K}$ đẳng cấu với $\mathbf{R}$, Mệnh đề 12 chỉ ra rằng mọi phép hoàn thiện $\hat{L}_t$ của $L$ (theo ký hiệu của Mệnh đề 11) đều đẳng cấu với nhau. Như vậy, với ký hiệu của Nhận xét 2 ở trên, hoặc là $r_1 = n$ và $r_2 = 0$, hoặc là $r_1 = 0$ và $2r_2 = n$.

### Bài tập {#ac-vi-s8-exercises}

Xem [các bài tập cho § 8](exercises/s8/).
