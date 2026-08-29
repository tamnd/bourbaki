---
book: ac
book_title: Commutative Algebra
chapter: III
chapter_title: GRADUATIONS. FILTRATIONS AND TOPOLOGIES
section: 3
section_title: m-adic topologies on Noetherian rings
lang: vi
source: ac-i-vii
book_pages: 195-209, 245-255
pdf_pages: 0215-0229, 0265-0275
extraction: ocr
subsections:
    - "no": 1
      title: GOOD FILTRATIONS
      page: 195
      pdf_page: 215
    - "no": 2
      title: m-ADIC TOPOLOGIES ON NOETHERIAN RINGS
      page: 199
      pdf_page: 219
    - "no": 3
      title: ZARISKI RINGS
      page: 201
      pdf_page: 221
    - "no": 4
      title: THE HAUSDORFF COMPLETION OF A NOETHERIAN RING
      page: 202
      pdf_page: 222
    - "no": 5
      title: THE COMPLETION OF A ZARISKI RING
      page: 206
      pdf_page: 226
statements: 39
exercises: 7
content_sha256: 1de39e55c74385c34054c27fb968c53e9cc1e60852f6e4cfaaf397d4b080d963
translated_from: content/en/ac/III/03_s3_m_adic_topologies_on_noetherian_rings.md
source_content_sha256: 7f34e8fa776003d5116ba6baec027fc4736d0298ce93dee623ca18e4bbb7b4ec
translation_model: gpt-5-6-mini, gpt-5.4
translation_run: translate-vi-04807a92
glossary_version: 34
glossary_terms_sha256: 78a746f638393c0b9dd590de5a5fa8756837f5e9d59cc7fbe432a4a1a353838d
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 3. Các tôpô $\mathfrak{m}$-adic trên các vành Noether

Tất cả các lọc được xét trong đoạn này được giả thiết là đầy đủ.

### 1. CÁC LỌC TỐT

Cho $\mathbf{A}$ là một vành giao hoán có lọc, E là một $\mathbf{A}$-môđun có lọc và $(\mathbf{A}_n)$ và $(E_n)$

là các lọc tương ứng của $A$ và $E$; giả sử rằng $A_0 = A$. Trong vành đa thức $A[X]$, tập hợp $A' = \sum_{n \geq 0} A_n X^n$ là một *đại số con phân bậc trên A kiểu $\mathbf{N}$*; nhóm con $E' = \sum_{n \geq 0} E_n \otimes_A A X^n$ của $E \otimes_A A[X]$ là một *$A'$-môđun phân bậc kiểu $\mathbf{N}$*, vì
$$
A_m X^m (E_n \otimes_A A X^n) \subset (A_m E_n \otimes_A A X^n",") \subset E_{m+n} \otimes_A A X^{m+n}.
$$

#### Định nghĩa 1 {#ac-iii-s3-def-1 .statement}

*Cho $A$ là một vành giao hoán, $m$ là một iđêan của $A$, $E$ là một $A$-môđun và $(E_n)$ là một lọc trên nhóm cộng tính $E$ gồm các môđun con của $E$. Lọc $(E_n)$ được gọi là m-tốt nếu:*
(1) $m E_n \subset E_{n+1}$ với mọi $n \in \mathbf{Z}$;
(2) *tồn tại một số nguyên $n_0$ sao cho* $m E_n = E_{n+1}$ *với* $n \geq n_0$.

Khi đó, bằng quy nạp theo $q$, $m^q E_n = E_{n+q}$ với $n \geq n_0, q \geq 1$. Chú ý rằng điều kiện (1) có nghĩa là lọc $(E_n)$ tương thích với cấu trúc $A$-môđun trên $E$ nếu $A$ được cho lọc $m$-adic. Rõ ràng, trên mọi $A$-môđun $E$, lọc $m$-adic là m-tốt. Nếu một lọc trên một $A$-môđun $E$ là m-tốt, lọc thương trên mọi môđun thương của $E$ là m-tốt.

#### Định lý 1 {#ac-iii-s3-thm-1 .statement}

*Cho $A$ là một vành giao hoán, $m$ là một iđêan của $A$, $E$ là một $A$-môđun và $(E_n)$ là một lọc của nhóm cộng $E$ gồm các môđun con-$A$ sinh hữu hạn. Giả sử rằng $m E_n \subset E_{n+1}$ với mọi $n$. Gọi $A'$ là đại số con phân bậc $\sum_{n \geq 0} m^n X^n$ của $A[X]$ và $E'$ là $A'$-môđun phân bậc $\sum_{n \geq 0} E_n \otimes_A A X^n$. Hai điều kiện sau là tương đương:*
(a) *Lọc* $(E_n)$ *là m-tốt.*
(b) *$E'$ là một $A'$-môđun sinh hữu hạn.*

Giả sử rằng $m E_{n-1} = E_n$ với $n > n_0 \geq 0$. Với $i \leq n_0$, gọi $(e_i)_{i \leq n_0}$ là một hệ hữu hạn các phần tử sinh của $A$-môđun $E_i$. Vì $A$-môđun $E_n \otimes_A A X^n$ được sinh bởi các phần tử $e_{n,j} \otimes X^n$ với $0 \leq n \leq n_0$ và bằng
$$
m^{n-n_0} E_{n_0} \otimes_A A X^n
$$
với $n > n_0$, nên $A'$-môđun $E'$ được sinh bởi các phần tử $e_{n,j} \otimes X^n$ với $0 \leq n \leq n_0$ và $1 \leq j \leq r_n$; do đó hiển nhiên nó sinh hữu hạn.

Ngược lại, nếu $E'$ là một $A'$-môđun sinh hữu hạn, thì nó được sinh bởi một họ hữu hạn các phần tử dạng $e_k \otimes X^{n(k)}$, trong đó $e_k \in E_{n(k)}$. Gọi $n_0$ là số nguyên lớn nhất trong các số nguyên $n(k)$. Khi đó với $n \geq n_0$ và $f \in E_n$,
$$
f \otimes X^n = \sum_k t_k (e_k \otimes X^{n(k)})
$$
trong đó $t_k \in A'$; nếu cần, thay thế $t$, bằng thành phần thuần nhất bậc $n - n(k)$ của nó, ta có thể giả sử rằng $t_k = a_k X^{n-n(k)}$, trong đó $a_k \in m^{n-n(k)}$.

Vì phần tử duy nhất $X^n$ lập thành một cơ sở của A-môđun AX", phương trình $f \otimes X^n = \left( \sum_k a_k e_k \right) \otimes X^n$ suy ra $f = \sum_k a_k e_k$. Khi đó $E_n \subset m^{n-n_0} E_{n_0}$; vì bao hàm đối là hiển nhiên,

$$
E_n = m^{n-n_0} E_{n_0},
$$

do đó $E_n = m E_{n-1}$ với $n > n_0$.

#### Bổ đề 1 {#ac-iii-s3-lem-1 .statement}

*Một vành Noether giao hoán A và $m$ là một iđêan của A. Khi đó vành con $A' = \sum_{n \geq 0} m^n X^n$ của $A[X]$ là Noether.*

$A'$ là một đại số trên A sinh bởi $mX$; vì A là Noether, $mX$ là một A-môđun hữu hạn sinh và khi đó kết luận suy ra từ § 2, no. 10, Hệ quả 3 của Định lý 2.

#### Mệnh đề 1 {#ac-iii-s3-prop-1 .statement}

*Cho A là một vành giao hoán Noether và m là một iđêan của A; trang bị cho A lọc m-adic. Cho E, F là hai A-môđun có lọc và $j : F \to E$ là một đồng cấu đơn ánh tương thích với các lọc. Nếu E sinh hữu hạn và lọc của nó là m-tốt, thì F sinh hữu hạn và lọc của nó là m-tốt.*

Vì F đẳng cấu với một môđun con của E, nó sinh hữu hạn do A là Noether và E sinh hữu hạn. Gọi $(E,)$, $(F,)$ là các lọc tương ứng trên E và F, gồm các môđun con sinh hữu hạn; giữ nguyên ký hiệu của Bổ đề 1, đặt $E' = \sum_{n \geq 0} E_n \otimes_A A X^n, F' = \sum F_n \otimes_A A X^n$; vì theo giả thiết F, đẳng cấu với một môđun con của $E_n$, ta thấy rằng F' đẳng cấu với một môđun con của $E'$. Theo Định lý 1, $E'$ là một $A'$-môđun hữu hạn sinh và do đó F' cũng vậy vì A' là Noether (Bổ đề 1). Suy ra kết luận nhờ Định lý 1.

#### Hệ quả 1 (Bổ đề Artin-Rees) {#ac-iii-s3-prop-1-cor-1 .statement}

*Cho A là một vành giao hoán Noether, m là một iđêan của A, E là một A-môđun hữu hạn sinh và F là một môđun con của E. Lọc cảm sinh trên F bởi lọc m-adic trên E là m-tốt.*

Nói cách khác, tồn tại một số nguyên $n_0$ sao cho

$$
m((m^n E) \cap F) = (m^{n+1} E) \cap F
$$

với mọi $n \geq n_0$.

#### Hệ quả 2 {#ac-iii-s3-prop-1-cor-2 .statement}

*Cho A là một vành giao hoán Noether và a, b là hai iđêan của A. Tồn tại một số nguyên h > 0 sao cho $a^h \cap b \subset ab$.*

Tồn tại n sao cho $a^{n+1} \cap b = a(a^n \cap b) \subset ab$ theo Hệ quả 1 áp dụng cho $E = A, F = b$.

#### Hệ quả 3 {#ac-iii-s3-prop-1-cor-3 .statement}

*Cho A là một vành giao hoán Noether, m là một iđêan của A và x là một phần tử của $A$ không phải là ước của 0. Tồn tại một số nguyên $k > 0$ sao cho, với mọi $n \geq k$, quan hệ $xy \in m^n$ kéo theo $y \in m^{n-k}$.

Hệ quả 1 áp dụng cho $E = A, F = A x$ cho thấy rằng tồn tại $k$ sao cho, với mọi $n \geq k$, $m^n \cap Ax = m^{n-k}(m^k \cap Ax)$. Khi đó, nếu $xy \in m^n$,

$$
xy \in m^n \cap Ax \subset m^{n-k}x
$$

và vì $x$ không phải là ước của $0$, ta suy ra rằng $y \in m^{n-k}$.

Theo ký hiệu của các transporter (Chương I, § 2, no. 10), kết luận của Hệ quả 3 được viết là

(2)
$$
m^n : Ax \subset m^{n-k}.
$$

#### Hệ quả 4 {#ac-iii-s3-prop-1-cor-4 .statement}

Cho $A$ là một vành giao hoán Noether, $m$ là một iđêan của $A$, $E$ là một $A$-môđun hữu hạn sinh và $(E_n)$ và $(E'_n)$ là hai lọc gồm các môđun con của $E$. Giả sử rằng các lọc $(E_n)$ và $(E'_n)$ tương thích với cấu trúc $A$-môđun trên $E$ khi $A$ được trang bị lọc $m$-adic. Nếu lọc $(E_n)$ là $m$-tốt và $E'_n \subset E_n$ với mọi $n \in \mathbf{Z}$, thì lọc $(E'_n)$ là $m$-tốt.
Đây là một trường hợp riêng của Mệnh đề 1.

#### Bổ đề 2 {#ac-iii-s3-lem-2 .statement}

Cho $A, B$ là hai vành giao hoán Noether, $\phi : A \to B$ là một đồng cấu vành, $E$ là một A-môđun sinh hữu hạn và $F$ là một B-môđun sinh hữu hạn. Khi đó $\mathrm{Hom}_A(E, \phi_*(F))$ là một B-môđun sinh hữu hạn.

Theo giả thiết, tồn tại một A-đồng cấu toàn ánh $v : A^n \to E$; do đó ánh xạ $u \mapsto u \circ v$ từ $\mathrm{Hom}_A(E, \phi_*(F))$ vào $\mathrm{Hom}_A(A^n, \phi_*(F))$ là đơn ánh và, vì $B$ là Noether, chỉ cần chứng minh rằng $\mathrm{Hom}_A(A^n, \phi_*(F))$ là một B-môđun sinh hữu hạn; điều này là ngay lập tức vì nó đẳng cấu với $F^n$.

#### Mệnh đề 2 {#ac-iii-s3-prop-2 .statement}

Cho $A$ là một vành giao hoán Noether, $m$ là một iđêan của $A$ và $E, F$ là hai A-môđun sinh hữu hạn. Nếu $(F,)$ là một lọc $m$-tốt trên $F$, thì các môđun con $\mathrm{Hom}_A(E, F,)$ tạo thành một lọc $m$-tốt trên A-môđun $\mathrm{Hom}_A(E, F)$.
Vì $m^k F_n \subset F_{n+k}$ với $n \in \mathbf{Z}, k \geq 0$, nên cũng có

$$
m^k \mathrm{Hom}_A(E, F_n) \subset \mathrm{Hom}_A(E, F_{n+k});
$$

khi đó họ $(\mathrm{Hom}_A(E, F_n))_{n \in \mathbf{Z}}$ là một lọc trên $\mathrm{Hom}_A(E, F)$ tương thích với cấu trúc môđun của nó trên vành $A$ được lọc bởi lọc $m$-adic. Vì $E$ sinh hữu hạn, tồn tại một số nguyên $r > 0$ và một A-đồng cấu toàn ánh $u : A^r \to E$ xác định một A-đồng cấu đơn ánh

$$
v = \mathrm{Hom}(u, 1_F) : \mathrm{Hom}_A(E, F) \to \mathrm{Hom}_A(A^r, F);
$$

rõ ràng $v$ tương thích với các lọc $(\mathrm{Hom}_A(E, F,))$ và $(\mathrm{Hom}_A(A^r, F_n))$.
Vì $\mathrm{Hom}_A(E, F)$ và $\mathrm{Hom}_A(A^r, F)$ là sinh hữu hạn (Bổ đề 2), theo Mệnh đề 1 chỉ cần chỉ ra rằng lọc $(\mathrm{Hom}_A(A^r, F))$ là $m$-tốt; nhưng điều này là ngay lập tức nhờ sự tồn tại của đẳng cấu chính tắc $\mathrm{Hom}_A(A^r, F_r) \to F_n^r$ và thực tế là quan hệ $mF_n = F_n +$, suy ra $m(F_n^r) = (mF_n)^r = F_{n+1}^r$ (Đại số, Chương II, § 3, no. 7, Nhận xét).

#### Mệnh đề 3 {#ac-iii-s3-prop-3 .statement}

*Cho $A$ là một vành Noether và $m$ là một iđêan của $A$ sao cho $A$ tách biệt Hausdorff và đầy đủ đối với tôpô m-adic. Cho $E$ là một $A$-môđun lọc trên vành lọc $A$, hệ lọc $(E_n)$ của $A$ sao cho $E_0 = E$ và $E$ tách biệt Hausdorff đối với tôpô xác định bởi $(E_n)$. Khi đó các điều kiện sau là tương đương:
(a) $E$ là một $A$-môđun sinh hữu hạn và $(E_n)$ là một hệ lọc m-tốt.
(b) $\mathrm{gr}(E)$ là một $\mathrm{gr}(A)$-môđun sinh hữu hạn.
(c) Với mọi $n \geq 0$, $\mathrm{gr}_n(E)$ là một $A$-môđun sinh hữu hạn và tồn tại $n_0$ sao cho với $n \geq n_0$ đồng cấu chính tắc
$$
\mathrm{gr}_1(A) \otimes_A \mathrm{gr}_n(E) \to \mathrm{gr}_{n+1}(E)
$$
là toàn ánh.*

Ngay lập tức suy ra từ các định nghĩa rằng (a) kéo theo (c). Việc (b) kéo theo (c) là một hệ quả của § 1, no. 3, Bổ đề 1; ngược lại, nếu (c) đúng, rõ ràng $\mathrm{gr}(E)$ được sinh như một $\mathrm{gr}(A)$-môđun bởi tổng của các $\mathrm{gr}_p(E)$ với $p \leq n_0$ và do đó theo giả thiết thừa nhận một hệ sinh hữu hạn. Còn phải chứng minh rằng (c) kéo theo (a); vì các $\mathrm{gr}_n(E)$ sinh hữu hạn và $E_n = E$, trước hết rõ ràng, bằng quy nạp theo $n$, $E/E_n$ là một $A$-môđun sinh hữu hạn với mọi $n$; do đó chỉ cần chứng minh rằng, với $n > n_0$, $E_n$ là một $A$-môđun sinh hữu hạn và $mE_n = E_{n+1}$. Bây giờ, xét $A$-môđun $E_{n+1}$ với hệ lọc vét cạn và tách biệt $(E_{n+k})(k \geq 1)$; $mE_n \subset E_{n+1}$; giả thiết (c) kéo theo rằng ảnh của $mE_n$ trong $\mathrm{gr}_{n+1}(E) = E_{n+1}/E_{n+2}$ bằng $\mathrm{gr}_{n+1}(E)$ và sinh $\mathrm{gr}(A)$-môđun phân bậc $\mathrm{gr}(E_{n+1})$. Vì $\mathrm{gr}_{n+1}(E)$ theo giả thiết là một $A$-môđun sinh hữu hạn, suy ra từ § 2, no. 9, Mệnh đề 12 rằng $mE_n = E_{n+1}$ và $E_{n+1}$ là một $A$-môđun sinh hữu hạn.

### 2. CÁC TÔPÔ m-ADIC TRÊN CÁC VÀNH NOETHER

#### Mệnh đề 4 {#ac-iii-s3-prop-4 .statement}

*Mọi hệ lọc m-tốt trên $E$ đều xác định cùng một tôpô (cụ thể là tôpô m-adic).*

Cho $(E_n)$ là một lọc m-tốt trên $E$. Vì lọc này là toàn diện, mọi phần tử của $E$ thuộc một trong các $E_n$ và, vì $E$ là sinh hữu hạn và các $E_n$ là các $A$-môđun, tồn tại một số nguyên $n_1$ sao cho $E_{n_1} = E$. Mặt khác, lấy $n_0$ sao cho $mE_n = E_{n+1}$ với $n \geq n_0$; khi đó, với $n > n_0 - n_1$,
$m^n E \subset E_{n+n_1} = m^{n+n_1-n_0} E_{n_0} \subset m^{n+n_1-n_0} E$, điều này chứng minh mệnh đề.

**Định lý 2 (Krull).** *Cho $A$ là một vành giao hoán Noether, $m$ là một iđêan của $A$, $E$ là một $A$-môđun sinh hữu hạn và $F$ là một môđun con của $E$. Khi đó tôpô $m$-adic trên $F$ là tôpô cảm sinh bởi tôpô $m$-adic trên $E$.*

Suy ra từ no. 1, Mệnh đề 1 rằng lọc cảm sinh trên $F$ bởi lọc $m$-adic trên $E$ là m-tốt và khi đó kết luận suy ra từ Mệnh đề 4.

#### Hệ quả {#ac-iii-s3-n2-cor-1 .statement}

*Cho $A$ là một vành giao hoán Noether, $m$ là một iđêan của $A$, $E$ là một $A$-môđun và $F$ là một $A$-môđun sinh hữu hạn. Mọi ánh xạ tuyến tính $A$-tuyến tính $u : E \to F$ là một cấu xạ ngặt* (Tôpô Đại cương, Chương 111, § 2, no. 8) *đối với các tôpô $m$-adic*.

Vì $u(m^nE) = m^n u(E)$, $u$ là một cấu xạ ngặt từ $E$ lên $u(E)$ đối với các tôpô $m$-adic trên hai môđun này và tôpô $m$-adic trên $u(E)$ là cảm sinh bởi tôpô $m$-adic trên $F$ theo Định lý 2.

#### Mệnh đề 5 {#ac-iii-s3-prop-5 .statement}

*Cho $A$ là một vành giao hoán Noether, $m$ là một iđêan của $A$ và $E$ là một $A$-môđun sinh hữu hạn. Bao đóng* $\bigcap_{n=1}^m m^nE$ *của $\{0\}$ trong $E$ *đối với tôpô $m$-adic là tập hợp các $x \in E$ sao cho tồn tại một phần tử $m \in m$ thỏa mãn* $(1 - m)x = 0$.

Nếu $x = mx$ trong đó $m \in m$, $x = m^n x \in m^nE$ với mọi số nguyên $n \geq 0$ và do đó $x \in F = \bigcap_{n=0}^m m^nE$. Ngược lại, nếu $x \in F$, $Ax$ được chứa trong giao của các lân cận của 0 trong $E$; khi đó từ Định lý 2 suy ra rằng tôpô $m$-adic trên $Ax$, cảm sinh bởi tôpô trên $E$, là tôpô thô nhất; vì $mx$ theo định nghĩa là một lân cận của 0 đối với tôpô này, $mx = Ax$ và do đó tồn tại $m \in m$ sao cho $x = mx$.

Ta cũng có thể nói rằng $mF = F$ vì
$$
F = \bigcap_{n=1}^\infty m^{n+1}E \subset m. \bigcap_{n=1}^\infty m^nE = mF;
$$
vì $A$ là Noether, $F$ là một $A$-môđun sinh hữu hạn; khi đó chỉ cần áp dụng Chương II, § 2, no. 2, Hệ quả 3 vào Mệnh đề 4.

#### Hệ quả (Krull) {#ac-iii-s3-n2-cor-2 .statement}

*Cho $A$ là một vành giao hoán Noether và $m$ là một iđêan của $A$. Iđêan* $\bigcap_{n=1}^m m^n$ *là tập hợp các phần tử* $x \in A$ *mà tồn tại* $m \in m$ *sao cho* $(1 - m)x = 0$. *Đặc biệt, để* $\bigcap_{n=1}^\infty m^n = \{0\}$, *điều kiện cần và đủ là không có phần tử nào của* $1 + m$ *là một ước của* $0$ *trong* $A$.

Chỉ cần áp dụng Mệnh đề 5 cho $E = A$.

#### Nhận xét {#ac-iii-s3-n2-rem-1 .statement}

Giả thiết rằng $A$ là *Noether* là cốt yếu trong hệ quả này. Ví dụ, cho $A$ là vành các ánh xạ khả vi vô hạn từ $\mathbf{R}$ vào chính nó và cho $m$ là iđêan (cực đại) của $A$ gồm các hàm $f$ sao cho $f(0) = 0$. Hiển nhiên rằng $\bigcap_{n=0}^\infty m^n$ là tập hợp các hàm $f$ sao cho f^{(n)}(0) = 0 \text{ với mọi } n \geq 0 \text{ và tồn tại các hàm như vậy với } f(x) \neq 0, \text{ với mọi } x \neq 0, \text{ chẳng hạn hàm } f \text{ được xác định bởi } f(x) = e^{-1/x^2} \text{ với } x \neq 0 \text{ và } f(0) = 0.

#### Định nghĩa 1 {#ac-iii-s3-def-1-bis .statement}

*Cho $\mathbf{A}$ là một vành tôpô. Nếu một iđêan hai phía $m$ của $\mathbf{A}$ sao cho tôpô đã cho trên $\mathbf{A}$ là tôpô $m$-adic, thì $m$ được gọi là một iđêan xác định & tôpô trên $\mathbf{A}$.*

Cho $A$ là một vành giao hoán Noether, $m$ là một iđêan của $A$ và $t$ là căn của nó (Chương II, § 2, no. 6). Nếu $m'$ là một iđêan xác định của tôpô $m$-adic, thì tồn tại một số nguyên $n > 0$ sao cho ${m'}^n \subset m$ ($§ 2$, no. 5) và do đó $m' \subset t$; ngược lại, vì $A$ là Noether, tồn tại một số nguyên $k > 0$ sao cho $t^k \subset m$ (Chương II, § 2, no. 6, Mệnh đề 15) và do đó $t$ là *iđêan xác định lớn nhất* của tôpô $m$-adic.

### 3. CÁC VÀNH ZARISKI

#### Mệnh đề 6 {#ac-iii-s3-prop-6 .statement}

*Cho $A$ là một vành giao hoán Noether và $m$ là một iđêan của $A$. Các tính chất sau là tương đương:
(a) $m$ được chứa trong căn Jacobson của $A$.
(b) *Mọi $A$-môđun sinh hữu hạn đều Hausdorff đối với tôpô $m$-adic.*
(c) *Với mọi $A$-môđun sinh hữu hạn $E$, mọi môđun con của $E$ đều đóng đối với tôpô $m$-adic trên $E$.*
(d) *Mọi iđêan cực đại của $A$ đều đóng đối với tôpô $m$-adic.*

Ta hãy chỉ ra rằng (a) suy ra (b). Giả sử rằng $m$ được chứa trong căn Jacobson của $A$ và cho $E$ là một $A$-môđun sinh hữu hạn. Nếu $x \in E$ và $m \in m$ sao cho $(1 - m)x = 0$, thì $x = 0$, vì $1 - m$ khả nghịch trong $A$. Khi đó (no. 2, Mệnh đề 5) $E$ là Hausdorff đối với tôpô $m$-adic.

Ta hãy chứng minh rằng (b) suy ra (c). Giả sử (b) đúng. Cho $E$ là một $A$-môđun sinh hữu hạn và $F$ là một môđun con của $E$. Khi đó $E/F$ là Hausdorff đối với tôpô $m$-adic, là tôpô thương của tôpô $m$-adic trên $E$; khi đó $F$ đóng trong $E$.

Rõ ràng (c) suy ra (d). Sau cùng ta hãy chứng minh rằng (d) suy ra (a). Từ (d) suy ra rằng, với mọi iđêan cực đại $a$ của $A$, A-môđun $A/a$ là Hausdorff đối với tôpô $m$-adic. Điều này suy ra $m(A/a) \neq A/a$, trừ phi tôpô $m$-adic trên $A/a$ là tôpô thô nhất và $A/a$ thu về 0, điều này là vô lý vì $A/a$ là một *trường*. Do đó ảnh chính tắc của $m$ trong $A/a$ là một iđêan của $A/a$ phân biệt với $A/a$ và vì thế thu về 0; khi đó $m \subset a$, điều này chứng tỏ rằng $m$ được chứa trong căn Jacobson của $A$.

#### Định nghĩa 2 {#ac-iii-s3-def-2 .statement}

*Một vành tôpô $A$ được gọi là một vành Zariski nếu nó giao hoán và Noether và tồn tại một iđêan xác định $m$ cho tôpô trên $A$ thỏa mãn các điều kiện tương đương của Mệnh đề 6.*

Một vành Zariski $A$ tất yếu là *Hausdorff* (Mệnh đề 6) và *mọi* iđêan xác định của tôpô của nó đều được chứa trong căn Jacobson của $A$.

*Ví dụ về các vành Zariski*

#### Ví dụ 1 {#ac-iii-s3-n3-exa-1 .statement}

Cho $A$ là một vành giao hoán Noether và $m$ là một iđêan của $A$. Nếu $A$ là *Hausdorff và đầy đủ đối với tôpô m-adic*, thì $A$ là một vành Zariski đối với tôpô này, theo § 2, no. 13, Bổ đề 3.

#### Ví dụ 2 {#ac-iii-s3-n3-exa-2 .statement}

Mọi *vành thương* $A/b$ của một vành Zariski đều là một vành Zariski, vì nó là Noether và, nếu $m$ là một iđêan xác định của $A$, thì $m(A/b) = (m + b)/b$ được chứa trong căn Jacobson của $A/b$ (*Algebra*, Chương VIII, § 6, no. 3, Mệnh đề 7).

#### Ví dụ 3 {#ac-iii-s3-n3-exa-3 .statement}

Cho $A$ là một vành *Noether nửa địa phương* và $r$ là căn Jacobson của nó. Khi đó $A$, với tôpô $r$-adic, là một vành Zariski. Đây sẽ luôn luôn là tôpô được xét đến (trừ khi có nói rõ khác đi) khi ta xét một vành Noether nửa địa phương như một vành tôpô.

#### Mệnh đề 7 {#ac-iii-s3-prop-7 .statement}

*Cho $A, A'$ là hai vành giao hoán và $h : A \to A'$ là một đồng cấu vành. Giả sử rằng $A$ là Noether và rằng $A'$ là một A-môđun sinh hữu hạn (với cấu trúc được xác định bởi $h$). Cho $m$ là một iđêan của $A$ và đặt $m' = mA'$. Khi đó:*

(i) *Để tôpô $m'$-adic trên $A'$ là Hausdorff, điều kiện cần và đủ là các phần tử của $1 + h(m)$ không là ước của $0$ trong $A'$.*

(ii) *Nếu $A$, với tôpô $m$-adic, là một vành Zariski, thì $A'$, với tôpô $m'$-adic, là một vành Zariski.*

(iii) *Nếu $h$ là đơn ánh (do đó đồng nhất hoá $A$ với một vành con của $A'$), tôpô $m'$-adic trên $A'$ cảm sinh trên $A$ tôpô $m$-adic.*

Nhắc lại rằng bộ lọc $m'$-adic trên $A'$ trùng với bộ lọc $m$-adic trên *A-môđun* $A'$ (§ 2, no. 1, *Ví dụ 3*). Do đó mệnh đề (i) là một trường hợp riêng của Mệnh đề 5 của no. 2 và mệnh đề (iii) là một trường hợp riêng của Định lý 2 của no. 2. Sau hết, hãy chứng minh (ii). Giả sử rằng $A$ là một vành Zariski với tôpô $m$-adic và $E'$ là một $A'$-môđun hữu hạn sinh; nó cũng là một A-môđun hữu hạn sinh và các bộ lọc $m$-adic và $m'$-adic trên $E'$ trùng nhau; khi đó $E'$ là Hausdorff đối với tôpô $m'$-adic. Cuối cùng A-môđun $A'$ là Noether và vì thế vành $A'$ là Noether, điều này hoàn tất chứng minh rằng $A'$ là một vành Zariski.

### 4. BỔ SUNG HAUSDORFF CỦA MỘT VÀNH NOETHER

Cho $A$ là một vành giao hoán, $m$ là một iđêan của $A$ và $E$ là một A-môđun; ký hiệu $\hat{A}$ và $\hat{E}$ lần lượt là các bổ sung Hausdorff của $A$ và $E$ đối với tôpô $m$-adic và $j_E$ là ánh xạ chính tắc $E \to \hat{E}$. Ánh xạ $A$-song tuyến tính $(a, x) \mapsto aj_E(x)$ từ $\hat{A} \times E$ vào $\hat{E}$ xác định một ánh xạ A-tuyến tính

$$
\alpha_E : \hat{A} \otimes_A E \to \hat{E},
$$

được gọi là *chính tắc*. Cho $u : E \to F$ là một đồng cấu A-môđun và cho $\hat{u} : E \to \hat{F}$ là ánh xạ thu được bằng cách chuyển qua các bổ sung Hausdorff; với $a \in \hat{A}$, $x \in E$,

$$
\alpha_F(a \otimes u(x)) = aj_F(u(x)) = a\hat{u}(j_E(x)) = \hat{u}(\alpha_E(a \otimes x)),
$$

nói cách khác, biểu đồ

$$
\begin{array}{ccc}
\hat{A} \otimes_A E & \xrightarrow{1 \otimes u} & \hat{A} \otimes_A F \\
\downarrow \alpha_E & & \downarrow \alpha_F \\
\hat{E} & \xrightarrow{\hat{u}} & \hat{F}
\end{array}
$$

là giao hoán. Cuối cùng, suy ra từ § 2, no. 12, Mệnh đề 16 rằng, nếu E là sinh hữu hạn, thì đồng cấu $\alpha_E$ là toàn ánh.

#### Định lý 3 {#ac-iii-s3-thm-3 .statement}

*Cho A là một vành Noether giao hoán, m là một iđêan của A và E, F, G là ba A-môđun hữu hạn sinh. Khi đó:*

(i) *Nếu* $E \xrightarrow{u} F \xrightarrow{v} G$ *là một dãy khớp các ánh xạ A-tuyến tính, thì dãy* $\hat{E} \xrightarrow{\hat{u}} \hat{F} \xrightarrow{\hat{v}} \hat{G}$ *thu được bằng cách chuyển qua các bổ sung Hausdorff (đối với các tôpô m-adic) là khớp.*

(ii) *Ánh xạ A-tuyến tính chính tắc* $\alpha_E : \hat{A} \otimes_A E \to \hat{E}$ *là song ánh.*

(iii) *A-môđun* $\hat{A}$ *là phẳng.*

Ta đã thấy rằng $u$ và $v$ là các cấu xạ ngặt của các nhóm tôpô (no. 2, Hệ quả của Định lý 2). Khi đó mệnh đề (i) suy ra từ § 2, no. 12, Bổ đề 2. Mệnh đề (ii) là hiển nhiên khi $E = A$ và trường hợp E là một A-môđun tự do hữu hạn sinh có thể ngay lập tức quy về trường hợp đó. Trong trường hợp tổng quát, E thừa nhận một trình bày hữu hạn

$$
L \xrightarrow{u} L' \xrightarrow{v} E \longrightarrow 0
$$

(Chương I, § 2, no. 8, Bổ đề 8). Ta suy ra một biểu đồ giao hoán

$$
\begin{array}{ccccccccc}
\hat{A} \otimes_A L & \xrightarrow{1 \otimes u} & \hat{A} \otimes_A L' & \xrightarrow{1 \otimes v} & \hat{A} \otimes_A E & \longrightarrow & 0 \\
\downarrow \alpha_L & & \downarrow \alpha_{L'} & & \downarrow \alpha_E \\
\hat{L} & \longrightarrow & \hat{L}' & \longrightarrow & \hat{E} & \longrightarrow &
\end{array}
$$

Hàng thứ nhất là khớp (Chương I, § 2, no. 1, Bổ đề 1) và hàng thứ hai cũng vậy theo (i). Ta đã biết rằng $\alpha_E$ là toàn ánh (§ 2, no. 12, Mệnh đề 16); mặt khác, vì $\alpha_L$ và $\alpha_{L'}$ là song ánh và $1 \otimes v$ là toàn ánh, nên $\alpha_E$ là đơn ánh theo Chương I, § 1, no. 4, Hệ quả 2 của Mệnh đề 2; điều này chứng tỏ (ii).

Khi đó suy ra từ (i) và (ii) rằng, nếu $a$ là một iđêan của A (tất yếu sinh hữu hạn), ánh xạ chính tắc $\hat{A} \otimes_A a \to \hat{A}$ là đơn ánh, vì nó là hợp thành của $\hat{a} \to \hat{A}$ và $\alpha_E$, điều này chứng minh rằng $\hat{A}$ là một $A$-môđun phẳng (Chương I, § 2, no. 3, Mệnh đề 1).

Trong các điều kiện của Định lý 3, $\hat{A} \otimes_A E$ thường được đồng nhất với $E$ bằng ánh xạ chính tắc $\alpha_E$. Nếu $u : E \to F$ là một đồng cấu của các $A$-môđun sinh hữu hạn, thì khi đó $\hat{u} : E \to \hat{F}$ được đồng nhất với $1 @ u$ theo tính giao hoán của biểu đồ (4).

#### Hệ quả 1 {#ac-iii-s3-thm-3-cor-1 .statement}

Cho $A$ là một vành giao hoán Noether, $m$ một iđêan của $A$, $E$ một $A$-môđun sinh hữu hạn và $F$ và $G$ là hai môđun con của $E$. Trang bị cho $A, E, F, G$ các tôpô $m$-adic và gọi $i$ là ánh xạ chính tắc từ $E$ đến $e$. Khi đó:

$$
\hat{F} = \hat{A}.i(F), \quad (F + G)^{\wedge} = \hat{F} + \hat{G}, \quad (F \cap G)^{\wedge} = \hat{F} \cap \hat{G},
$$
$$
(F : G)^{\wedge} = \hat{F} : \hat{G}.
$$

Hơn nữa, nếu $a$ và $b$ là hai iđêan của $A$ và $c = ab, \hat{c} = \hat{a}\hat{b}$.

Theo Định lý 3, $\hat{E}, \hat{F}, \hat{G}$ được đồng nhất một cách chính tắc với $\hat{A} \otimes_A E, \hat{A} \otimes_A F, \hat{A} \otimes_A G$, điều này thiết lập hai công thức đầu tiên. Công thức thứ ba và thứ tư lần lượt suy ra từ Chương I, § 2, no. 6, Mệnh đề 6 và no. 10, Mệnh đề 12. Cuối cùng, vì $\hat{a} = \hat{A}i(a), \hat{b} = \hat{A}i(b), \hat{c} = \hat{A}i(c)$,
$$
\hat{c} = \hat{A}i(ab) = \hat{A}i(a)i(b) = \hat{a}\hat{b}.
$$

#### Hệ quả 2 {#ac-iii-s3-thm-3-cor-2 .statement}

Cho $A$ là một vành giao hoán Noether, $m$ một iđêan của $A$ và $\hat{A}$ là bổ sung Hausdorff của $A$ đối với tôpô $m$-adic. Nếu một phần tử $a \in A$ không là một ước của 0 trong $A$, thì ảnh chính tắc $a'$ của nó trong $\hat{A}$ không là một ước của 0 trong $\hat{A}$.

Vì $\hat{A}$ là một $A$-môđun phẳng, hệ quả này là một trường hợp riêng của Chương I, § 2, no. 4, Mệnh đề 3 (i).

#### Hệ quả 3 {#ac-iii-s3-thm-3-cor-3 .statement}

Nếu $A$ là một vành giao hoán Noether, thì vành các chuỗi lũy thừa hình thức $A[[X_1, \ldots, X_n]]$ là một $A$-môđun phẳng.

Đó là bổ túc của vành đa thức
$$
B = A[X_1, \ldots, X_n]
$$
đối với tôpô $m$-adic, trong đó $m$ là tập hợp các đa thức không có số hạng hằng ($§ 2,$ no. 12, Ví dụ 1); vì $B$ là Noether ($§ 2,$ no. 10, Hệ quả 2 của Định lý 2), nên $A[[X_1, \ldots, X_n]]$ là một B-môđun phẳng theo Định lý 3 và, vì $B$ là một A-môđun tự do, $A[[X_1, \ldots, X_n]]$ là một A-môđun phẳng (Chương I, § 2, no. 7, Hệ quả 3 của Mệnh đề 8).

#### Mệnh đề 8 {#ac-iii-s3-prop-8 .statement}

Cho $A$ là một vành giao hoán Noether, $m$ một iđêan của $A$, $\hat{A}$ là bổ túc Hausdorff của $A$ đối với tôpô $m$-adic và $j$ là ánh xạ chính tắc từ $A$ vào $\hat{A}$. Khi đó:
(i) $\hat{A}$ là một vành Zariski và $\hat{m} = \hat{A}.j(m)$ là một iđêan xác định của $\hat{A}$.

(ii) *Ánh xạ* $n \mapsto A = \hat{A}.j(n)$ *là một song ánh từ tập hợp các iđêan cực đại của* $A$ *chứa* $m$ *lên tập hợp các iđêan cực đại của* $\hat{A}$ *và* $q \mapsto j^{-1}(q)$ *là song ánh ngược*.

(iii) *Cho* $n$ *là một iđêan cực đại của* $A$ *chứa* $m$. *Đồng cấu* $j': A_n \to \hat{A}_{\hat{n}}$ *dẫn xuất từ* $j$ *là đơn ánh; nếu* $A$, *được đồng nhất nhờ* $j$ *với một vành con của* $\hat{A}$, *thì tôpô* $(nA_n)$*-adic trên* $A_n$ *được cảm sinh bởi tôpô* $A$*-adic trên* $\hat{A}_{\hat{n}}$ *và* $A_n$ *trù mật trong* $A$, *đối với tôpô* $A$*-adic*.

Ta hãy chứng minh (i). Vì $m$ là một iđêan sinh hữu hạn, $(m^n)^{\wedge} = (\hat{m})^n = m^n \hat{A}$ (§ 2, no. 12, Hệ quả 2 của Mệnh đề 16) và tôpô trên $\hat{A}$ là tôpô $m$-adic. Vì $\hat{A}/\hat{m}$ đẳng cấu với $A/m$, đó là một vành Noether và $\hat{m} = m \hat{A}$ là một A-môđun sinh hữu hạn và do đó $\hat{A}$ là Noether (§ 2, no. 10, Hệ quả 5 của Định lý 2); cuối cùng, vì $\hat{A}$ là Hausdorff và đầy đủ đối với tôpô $m$-adic, nên $\hat{A}$ là một vành Zariski (no. 3, *Ví dụ* 1).

Mệnh đề (ii) suy ra ngay lập tức từ việc đồng cấu chính tắc $A/m + \hat{A}/\hat{m}$ cảm sinh bởi $j$ là song ánh và từ việc mọi iđêan cực đại của $\hat{A}$ đều chứa $\hat{m}$, vì $\hat{A}$ là một vành Zariski và khi đó căn Jacobson của $\hat{A}$ chứa $m$ (no. 3, Mệnh đề 6).

Sau cùng, hãy chứng minh (iii). Vì $n = j^{-1}(A)$, ta có $j(A - n) \subset \hat{A} - \hat{n}$ và hiển nhiên $j$ xác định một đồng cấu $j': A_n \to \hat{A}_{\hat{n}}$ (Chương II, § 2, no. 1, Mệnh đề 2). Hãy chỉ ra rằng $j'$ là đơn ánh; giả sử $a \in A, s \in A - n$ sao cho
$$
j'(a/s) = j(a)/j(s) = 0;
$$
khi đó tồn tại $s' \in \hat{A} - \hat{n}$ sao cho $s'j(a) = 0$ (Chương II, § 2, no. 1, *Nhận xét* 3) và do đó linh hóa tử của $j(a)$ trong $\hat{A}$ không được chứa trong $\hat{n}$. Bây giờ, nếu $b$ là linh hóa tử của $a$ trong $A$, thì linh hóa tử của $j(a)$ trong $\hat{A}$ là $b$ (Hệ quả 1 của Định lý 3); vì thế $b \notin n$, điều này chứng tỏ rằng $a/s = 0$.

Hơn nữa, có một biểu đồ giao hoán
$$
\begin{array}{ccc}
A/n^k & \longrightarrow & A_n/(nA_n)^k \\
h \downarrow & & h' \downarrow \\
\hat{A}/\hat{n}^k & \longrightarrow & \hat{A}_{\hat{n}}/(\hat{n}\hat{A}_{\hat{n}})^k
\end{array}
$$
trong đó $h$ và $h'$ lần lượt được cảm sinh bởi $j$ và $j'$ còn các mũi tên ngang là các đẳng cấu chính tắc của Chương II, § 3, no. 3, Mệnh đề 9. Vì $n^k$ là một iđêan mở của $A$ (do nó chứa $m^k$), $h$ là song ánh và do đó $h'$ cũng vậy. Điều này trước hết cho thấy rằng $(nA_n)^k = j'((\hat{n}\hat{A}_{\hat{n}})^k)$ và do đó tôpô trên $A_n$ được cảm sinh bởi tôpô trên $A_n$; hơn nữa, $\hat{A}_{\hat{n}} = A_n + (\hat{n}\hat{A}_{\hat{n}})^k$ với mọi $k > 0$ và do đó $A_n$ trù mật trong $A_n$.

#### Hệ quả {#ac-iii-s3-n4-cor-1 .statement}

*Cho* $A$ *là một vành địa phương Noether* (resp. *nửa địa phương*) *và* $m$ *là căn Jacobson của nó. Khi đó* $\hat{A}$ *là một vành địa phương Noether* (resp. *nửa địa phương*) *mà căn Jacobson là* $\hat{m}$.

$\hat{A}$ là Noether theo Mệnh đề 8 (i), và phần còn lại suy ra từ Mệnh đề 8 (ii) và công thức thứ ba trong Hệ quả 1 của Định lý 3.

### 5. PHẦN HOÀN THÀNH CỦA MỘT VÀNH ZARISKI

#### Mệnh đề 9 {#ac-iii-s3-prop-9 .statement}

Cho $A$ là một vành giao hoán Noether và $m$ là một iđêan của $A$; giả sử $A$ được trang bị tôpô $m$-adic. Để $\hat{A}$ là một A-môđun phẳng trung thành, điều kiện cần và đủ là $A$ là một vành Zariski.

Đối với mọi $A$-môđun sinh hữu hạn $M$, ánh xạ chính tắc $M \to M \otimes_A \hat{A}$ được đồng nhất với ánh xạ chính tắc $M \to \hat{M}$ từ $M$ đến hoàn thành Hausdorff của nó đối với tôpô $m$-adic (no. 4, Định lý 3) và khi đó hạt nhân của ánh xạ này là bao đóng của $\{0\}$ trong $M$ đối với tôpô này. Vì ta đã biết rằng $\hat{A}$ là một $A$-môđun phẳng (no. 4, Định lý 3), mệnh đề suy ra từ đặc trưng hóa của các môđun phẳng trung thành (Chương I, § 3, no. 1, Mệnh đề 1 (b)) và đặc trưng hóa của các vành Zariski (no. 3, Mệnh đề 6).

Nếu $A$ là một vành Zariski và $E$ là một $A$-môđun sinh hữu hạn, ta có thể (nhờ Mệnh đề 9) đồng nhất $E$ với một tập con của $\hat{E}$ bằng ánh xạ chính tắc $j_E : E \to \hat{E}$. Với sự đồng nhất này:

#### Hệ quả 1 {#ac-iii-s3-prop-9-cor-1 .statement}

Cho $A$ là một vành Zariski, $E$ một $A$-môđun sinh hữu hạn và $F$ một môđun con của $E$. Khi đó $F = \hat{F} \cap E = (\hat{A}F) \cap E$.

Đây là một trường hợp riêng của Chương I, § 3, no. 5, Mệnh đề 10 (ii) và nó cũng suy ra từ no. 3, Mệnh đề 6.

#### Hệ quả 2 {#ac-iii-s3-prop-9-cor-2 .statement}

Cho $A$ là một vành Zariski và $E$ một $A$-môđun sinh hữu hạn. Nếu $\hat{E}$ là một $A$-môđun tự do, thì $E$ là một $A$-môđun tự do.

Gọi $m$ là một iđêan xác định của $A$, do đó được chứa trong căn Jacobson của $A$. Ta áp dụng tiêu chuẩn của Chương II, § 3, no. 5, Mệnh đề 5: ánh xạ chính tắc $j_E : E \to \hat{E}$ xác định một song ánh $i_E : E/mE \to \hat{E}/(mE)^{\wedge}$; tương tự, ánh xạ chính tắc $j_A : A \to \hat{A}$ xác định một song ánh $i_A : A/m \to \hat{A}/\hat{m}$, là một đẳng cấu vành. Khi đó $(mE)^{\wedge} = \hat{A}.mE = \hat{m}\hat{E}$ (no. 4, Định lý 3), nên $\hat{E}/(mE)^{\wedge}$ được trang bị một cấu trúc môđun trên $(\hat{A}/\hat{m})$ và do đó (bằng $i_A$) một cấu trúc môđun trên $(A/m)$. Ngay lập tức thấy rằng $i_E$ là $(A/m)$-tuyến tính, nên nó là một đẳng cấu môđun trên $(A/m)$. Vì $\hat{E}/\hat{m}\hat{E}$ là một môđun tự do trên $(\hat{A}/\hat{m})$, nên $E/mE$ là một môđun tự do trên $(A/m)$.

Mặt khác, gọi $\nu : m \otimes_A E \to E$ là đồng cấu chính tắc; vì $(m \otimes_A E) \otimes_A \hat{A}$ được đồng nhất một cách chính tắc với $m \otimes_A \hat{E}$ và $E \otimes_A \hat{A}$ với $\hat{E}$ (no. 4, Định lý 3), giả thiết rằng $\hat{E}$ là một $\hat{A}$-môđun tự do kéo theo rằng đồng cấu $\nu \otimes 1 : \hat{m} \otimes_{\hat{A}} \hat{E} \to \hat{E}$ là đơn ánh. Vì $\hat{A}$ là một $A$-môđun phẳng trung thành (Mệnh đề 9), ta kết luận rằng $\nu$ là đơn ánh (Chương I, § 3, no. 1, Mệnh đề 2) và quả thật các điều kiện để áp dụng tiêu chuẩn nói trên đều được thỏa mãn.

#### Hệ quả 3 {#ac-iii-s3-prop-9-cor-3 .statement}

Cho $A$ là một vành Zariski sao cho $\hat{A}$ là một miền nguyên và gọi $a$ là một iđêan của $A$. Nếu iđêan $a\hat{A}$ của $\hat{A}$ là chính, thì $a$ là chính.

Đây là một trường hợp riêng của Hệ quả 2.

#### Hệ quả 4 {#ac-iii-s3-prop-9-cor-4 .statement}

Cho $A$ là một vành Zariski sao cho $\hat{A}$ là một miền nguyên, $L$ là trường phân thức của $\hat{A}$ và $K \subset L$ là trường phân thức của $A$; khi đó $\hat{A} \cap K = A$.

Rõ ràng $A \subset \hat{A} \cap K$; mặt khác, nếu $x \in \hat{A} \cap K$, thì $\hat{A}x \subset \hat{A}$ và do đó, vì $\hat{A}x = \hat{A} \otimes_A (Ax)$ (no. 4, Định lý 3), nên $\hat{A} \otimes_A ((Ax + A)/A) = 0$. Vì $\hat{A}$ là một A-môđun phẳng trung thành (Mệnh đề 9), ta suy ra rằng $Ax \subset A$, do đó $x \in A$.

#### Hệ quả 5 {#ac-iii-s3-prop-9-cor-5 .statement}

Cho $A$ là một vành Noether giao hoán, $E, F$ là hai A-môđun sinh hữu hạn và $u : E \to F$ là một A-đồng cấu. Với mọi iđêan cực đại $m$ của $A$, gọi $A(m)$ (tương ứng $E(m), F(m)$) là hoàn thành Hausdorff của $A$ (tương ứng $E, F$) đối với tôpô $m$-adic và $u(m) : E(m) \to F(m)$ là đồng cấu tương ứng với $u$. Để $u$ là đơn ánh (tương ứng toàn ánh, song ánh, không), điều kiện cần và đủ là $u(m)$ cũng như vậy với mọi iđêan cực đại $m \notin A$.

Ta biết rằng để $u$ là đơn ánh (tương ứng toàn ánh, song ánh, không), điều kiện cần và đủ là $u_m : E_m \to F$, cũng như vậy với mọi iđêan cực đại $m$ của $A$ (Chương II, § 3, no. 3, Định lý 1). Bây giờ ta chú ý rằng $A_m$ là một vành địa phương Noether (Chương II, § 2, no. 4, Hệ quả 2 của Mệnh đề 10) và vì thế là một vành Zariski, và có một đẳng cấu đại số $A_m$-chính tắc $\hat{A}_m \to A(m)$ (§ 2, no. 13, Mệnh đề 18). Mặt khác (đầu no. 4), có một biểu đồ giao hoán

$$
\begin{array}{ccc}
E_m \otimes_{A_m} A(m) & \longrightarrow & E \otimes_A A(m) \longrightarrow E(m) \\
u_m \otimes 1 \downarrow & & \downarrow u \otimes 1 \downarrow u(m) \\
F_m \otimes_{A_m} A(m) & \longrightarrow & F \otimes_A A(m) \longrightarrow F(m)
\end{array}
$$

trong đó các mũi tên ngang bên trái xuất phát từ tính kết hợp của tích tenxơ và các đẳng cấu $E_m \to E \otimes_A A_m, F_m \to F \otimes_A A_m$; vì $E$ và $F$ là các A-môđun sinh hữu hạn, nên theo no. 4, Định lý 3, các hàng của biểu đồ này gồm toàn các đẳng cấu; do đó ta được quy về việc chứng minh rằng $u_m$ là đơn ánh (tương ứng toàn ánh, song ánh, không) tương đương với việc $u_m \otimes 1$ cũng như vậy. Nhưng điều này suy ra từ việc $\hat{A}_m$ (và do đó cả $A(m)$ nữa) là một $A_m$-môđun phẳng trung thành theo Mệnh đề 9 (Chương I, § 3, no. 1, các Mệnh đề 1 và 2).

#### Mệnh đề 10 {#ac-iii-s3-prop-10 .statement}

Cho $A, B$ là hai vành Zariski, $\hat{A}, \hat{B}$ là các hoàn thành của chúng, $f : A \to B$ là một đồng cấu vành liên tục và $\hat{f} : \hat{A} \to \hat{B}$ là đồng cấu nhận được từ $f$ bằng cách chuyển qua các hoàn thành; nếu $\hat{f}$ là song ánh, thì $A$-môđun $B$ là phẳng trung thành.

Vì $A$ và $B$ là Hausdorff, giả thiết rằng $\hat{f}$ là song ánh trước hết kéo theo rằng $f$ là đơn ánh. Đồng nhất (về mặt đại số) $A$ với $f(A)$ nhờ $f$ và $\hat{A}$ với $\hat{B}$ nhờ $\hat{f}$, khi đó ta được các bao hàm $A \subset B \subset \hat{A} = \mathbf{8}$; ta biết rằng $\hat{A}$ là một $A$-môđun phẳng trung thành và một $B$-môđun phẳng trung thành (Mệnh đề 9); ta kết luận rằng $B$ là một $A$-môđun phẳng trung thành (Chương I, § 3, no. 4, Nhận xét 2).

#### Mệnh đề 11 {#ac-iii-s3-prop-11 .statement}

Cho $\mathbf{A}$ là một vành địa phương Noether, $m$ là iđêan cực đại của nó, $\hat{\mathbf{A}}$ là hoàn thành $m$-adic của nó và $B$ là một vành sao cho $\mathbf{A} \subset B \subset \hat{\mathbf{A}}$. Giả sử rằng $B$ là một vành địa phương Noether mà iđêan cực đại $n$ của nó thỏa mãn quan hệ $n = mB$. Khi đó

$$
n^k = m^kB = \hat{m}^k \cap B
$$

với mọi $k \geq 1$, tôpô $n$-adic trên $B$ được cảm sinh bởi tôpô $m$-adic trên $\hat{\mathbf{A}}$, $B$ là một $\mathbf{A}$-môđun phẳng trung thành và có một đẳng cấu từ $\hat{\mathbf{A}}$ lên hoàn thành $n$-adic $\hat{B}$ của $B$, đẳng cấu này mở rộng đơn ánh chính tắc $\mathbf{A} \to B$.

Chỉ cần kiểm tra quan hệ $n^k = \hat{m}^k \cap B$, vì, do $B$ trù mật trong $\hat{\mathbf{A}}$ và tôpô $n$-adic được cảm sinh bởi tôpô $m$-adic, khẳng định cuối cùng sẽ suy ra từ *General Topology*, Chương II, § 3, no. 9, Hệ quả 1 của Mệnh đề 18 và khẳng định áp chót sẽ suy ra từ Mệnh đề 10. Đơn ánh $j_A : \mathbf{A} \to \hat{\mathbf{A}}$ (resp. $j : B \to \hat{\mathbf{A}}$) xác định bằng cách lấy thương một đồng cấu đơn cấu

$$
i_1 : \mathbf{A}/(\hat{m} \cap \mathbf{A}) \to \hat{\mathbf{A}}/\hat{m}
$$

(resp. $i_B : B/(\hat{m} \cap B) \to \hat{\mathbf{A}}/\hat{m}$). Ta biết rằng $m \cap \mathbf{A} = m$ và $i_A$ là song ánh, do đó $i_B$ là song ánh, điều này cho thấy $B/(\hat{m} \cap B)$ là một trường, suy ra $\hat{m} \cap B$ là một iđêan cực đại của $B$ và vì thế $m \cap B = n$. Vì $\mathbf{A} = \mathbf{A} + m$, nên $B = A + n = A + mB$; bằng quy nạp theo $k$ ta suy ra rằng

$$
B = A + m^kB = A + n^k
$$

với mọi $k > 1$. Vì $n^k \subset \hat{m}^k \cap B$, chỉ cần chứng minh rằng $\hat{m}^k \cap B \subset n^k$; nếu $b \in \hat{m}^k \cap B$, ta có thể viết $b = a + z$ với $a \in \mathbf{A}$, $z \in n^k$; do đó

$$
a = b - z \in \hat{m}^k \cap \mathbf{A} = m^k \subset n^k
$$

và $b \in n^k$.

\* Một trường hợp quan trọng mà điều này áp dụng được là trường hợp sau: $B$ là vành các chuỗi nguyên theo $n$ biến trên một trường đầy đủ định giá, hội tụ trong lân cận của 0, $\mathbf{A}$ là vành địa phương

$$
K[X_1, \ldots, X_n]_{\mathfrak{p}}
$$

trong đó $\mathfrak{p}$ là iđêan cực đại gồm các đa thức không có số hạng hằng và $\hat{\mathbf{A}}$ là vành các chuỗi lũy thừa hình thức $K[[X_1, \ldots, X_n]]$. \*

#### Nhận xét {#ac-iii-s3-n5-rem-1 .statement}

Một vành địa phương $B$ sao cho $\mathbf{A} \subset B \subset \hat{\mathbf{A}}$, có iđêan cực đại $n$ bằng $mB$ và có tôpô $n$-adic được cảm sinh bởi tôpô $m$-adic trên $\mathbf{A}$, không nhất thiết là Noether (Bài tập 14).

#### Mệnh đề 12 {#ac-iii-s3-prop-12 .statement}

Cho $A$ là một vành giao hoán Noether, $m$ là một iđêan của $A$, $S$ là tập con nhân $1 + m$ của $A$ và $E$ là một $A$-môđun sinh hữu hạn. Trong các điều kiện đó:

(i) $S^{-1}A$ là một vành Zariski đối với tôpô ($S^{-1}m$)-adic.

(ii) *Ánh xạ chính tắc* $f : E \to S^{-1}E$ *là liên tục nếu* $E$ *được trang bị tôpô m-adic và* $S^{-1}E$ *được trang bị tôpô* $(S^{-1}m)$-adic và $\hat{f} : E \to (S^{-1}E)^{\wedge}$ *là một đẳng cấu.*

Mọi phần tử của $1 + (S^{-1}m)$ đều có dạng
$$
1 + (m/(1 + m')) = (1 + m + m')/(1 + m)
$$
trong đó $m \in m$ và $m' \in m$; do đó nó khả nghịch trong $S^{-1}A$, điều này chứng minh rằng $S^{-1}m$ được chứa trong căn Jacobson của $S^{-1}A$; vì $S^{-1}A$ là Noether (Chương II, § 2, no. 4, Hệ quả 2 của Mệnh đề 10), $S^{-1}A$ là một vành Zariski đối với tôpô $(S^{-1}m)$-adic, điều này chứng minh (i). Hãy chứng minh (ii). Với mọi $n > 0$,
$$
\bar{f}^{-1}((S^{-1}m)^nE) = \bar{f}'(S^{-1}(m^nE)) = m^nE:
$$
vì rõ ràng trước hết $f(m^nE) \subset S^{-1}m^nE$; ngược lại, giả sử $x$ là một phần tử của $\bar{f}^{-1}(S^{-1}m^nE)$; khi đó tồn tại các phần tử $m', m''$ của $m$ và $x'' \in m^nE$ sao cho $(1 + m')((1 + m'')x - x'') = 0$, do đó $(1 - m)x = x'$, trong đó
$$
m = -(m' + m'' + m'm'') \in m
$$
và $x' = (1 + m')x'' \in m^nE$; ta kết luận rằng
$$
x = (1 + m + \cdots + m^{n-1})x' + m^n x \in m^nE.
$$
Điều này chứng minh rằng $f$ là một cấu xạ ngặt. Hơn nữa, hạt nhân của $f$, là tập hợp các $x \in E$ sao cho tồn tại một $s \in S$ với $sx = 0$, trùng với hạt nhân của ánh xạ chính tắc $j : E \to \hat{E}$ (no. 2, Mệnh đề 5). Khi đó tồn tại một đẳng cấu tôpô $f_0 : j(E) \to f(E)$ sao cho $f = f_0 \circ j$; vì $\hat{f}$ là một đẳng cấu tôpô, bài toán quy về việc kiểm tra rằng $f(E)$ trù mật trong $S^{-1}E$. Bây giờ, mọi phần tử của $S^{-1}E$ đều có thể viết dưới dạng $x/(1 - m)$, trong đó $m \in m$, và người ta kiểm tra ngay lập tức rằng
$$
x/(1 - m) \equiv ((1 + m + \cdots + m^{n-1})x)/1 \pmod{S^{-1}m^nE}
$$
điều này hoàn tất chứng minh.

### Bài tập {#ac-iii-s3-exercises}

Xem [bài tập của § 3](exercises/s3/).
