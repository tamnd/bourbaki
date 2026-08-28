---
book: ac
book_title: Commutative Algebra
chapter: II
chapter_title: LOCALIZATION
section: 5
section_title: Finitely generated projective modules. Invertible fractional ideals
lang: vi
source: ac-i-vii
book_pages: 108-120, 146-153
pdf_pages: 0128-0140, 0166-0173
extraction: ocr
subsections:
    - "no": 1
      title: LOCALIZATION WITH RESPECT TO AN ELEMENT
      page: 108
      pdf_page: 128
    - "no": 2
      title: LOCAL CHARACTERIZATION OF FINITELY GENERATED PROJECTIVE MODULES
      page: 109
      pdf_page: 129
    - "no": 3
      title: RANKS OF PROJECTIVE MODULES
      page: 111
      pdf_page: 131
    - "no": 4
      title: PROJECTIVE MODULES OF RANK 1
      page: 114
      pdf_page: 134
    - "no": 5
      title: NON-DEGENERATE SUBMODULES
      page: 116
      pdf_page: 136
    - "no": 6
      title: INVERTIBLE SUBMODULES
      page: 117
      pdf_page: 137
    - "no": 7
      title: THE GROUP OF CLASSES OF INVERTIBLE MODULES
      page: 119
      pdf_page: 139
statements: 34
exercises: 8
content_sha256: 92d636d2f57f1c947a0bcff6c246f6e062e68562972a9a06c360454be321e17d
translated_from: content/en/ac/II/05_s5_finitely_generated_projective_modules.md
source_content_sha256: 1cbbdb2e32921c4f6ee5337af18e13c88d05528cbdfb0af689b4b382c3f1454e
translation_model: gpt-5-6-mini, gpt-5-6
translation_run: translate-vi-5e8c59f3
glossary_version: 34
glossary_terms_sha256: d5ab3db1f1a54a92c0d18fd6bc6b0a04065e0cd8faa6195c75d1cd9e4af40dac
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 5. MÔĐUN XẠ ẢNH SINH HỮU HẠN. IĐÊAN PHÂN SỐ KHẢ NGHỊCH

### 1. ĐỊA PHƯƠNG HÓA ĐỐI VỚI MỘT PHẦN TỬ

Cho $A$ là một vành và $M$ là một $A$-môđun. Với mọi phần tử $f \in A$, ta sẽ viết $A_f = A[f^{-1}], M_f = M[f^{-1}] = M \otimes_A A[f^{-1}]$ (\S 2, nos. 1 and 2); nếu $S_f$ là tập hợp off" for $n \geq 0$, thì $A_{S_f} = S_f^{-1}A, M_{S_f} = S_f^{-1}M$. Nếu f khả nghịch trong $A$, $A_f$ (resp. $M_f$) được đồng nhất một cách chính tắc với $A$ (resp. $M$); nếu f lũy linh, thì $A_f = 0$ và $M_f = 0$. Với mọi đồng cấu $A$-môđun $u : M \to N$, ta viết $u_f = u \otimes 1 : M_f \to N_f$.

Cho $g$ là một phần tử khác của $A$; $A_g$ (resp. $M_g$) được đồng nhất một cách chính tắc với $(A,)_{g/1}$ (resp. $(M_f)_{g/1}$), trong đó $g/1$ là ảnh của $g$ trong $A_g$, và $u_{f,g}$ với $(u_f)_{g/1}$ (\S 2, no. 3, Mệnh đề 7).

#### Mệnh đề 1 {#ac-ii-s5-prop-1 .statement}

*Cho $f$ là một phần tử của một vành $A$ và $\phi : A \to A_f$, ánh xạ chính tắc. Ánh xạ $^a\phi : \operatorname{Spec}(A_f) \to \operatorname{Spec}(A)$ là một phép đồng phôi của $\operatorname{Spec}(A_f)$ lên không gian con mở $X_f$ của $X = \operatorname{Spec}(A)$ (\S 4, no. 3).*

Đây là một trường hợp riêng của \S 4, no. 3, Hệ quả của Mệnh đề 13.

#### Mệnh đề 2 {#ac-ii-s5-prop-2 .statement}

*Cho $A$ là một vành, $u : M \to N$ là một đồng cấu $A$-môđun và $p$ là một iđêan nguyên tố của $A$.

(i) Giả sử rằng $u_p : M_p \to N_p$ là toàn ánh và $N$ là sinh hữu hạn. Khi đó tồn tại $f \in A - p$ sao cho $u_f : M \to N$, là toàn ánh.

(ii) Giả sử rằng $u_p$ là song ánh, $M$ là sinh hữu hạn và $N$ là trình bày hữu hạn. Khi đó tồn tại $f \in A - p$ sao cho $u_f$ là song ánh.*

Cho $R$ và $Q$ lần lượt là hạt nhân và đối hạt nhân của $u$; nếu $g \in A$, hạt nhân và đối hạt nhân của $u_g$ (resp. $u_p$) lần lượt là $R_g$ và $Q_g$, (resp. $R_p$ và $Q_p$) (\S 2, no. 4, Định lý 1). Khi đó $Q_p = 0$; vì $N$ sinh hữu hạn, nên $Q$ cũng sinh hữu hạn và tồn tại $g' \in A - p$ sao cho $g'Q = 0$ (\S 2, no. 2, Hệ quả 2 của Mệnh đề 4), do đó $Q_{g'} = 0$. Dưới các giả thiết của (ii), dãy $0 \to R_{g'} \to M \to N \to 0$ là khớp, do đó $R_{g'}$ sinh hữu hạn (Chương I, \S 2, no. 8, Bổ đề 9). Bây giờ,

$$
(R_{g'})_{pR_{g'}} = R_p = 0;
$$

do đó tồn tại $g_1 \in A, - pA_{g'}$ sao cho $g_1 R_{g'} = 0$ (\S 2, no. 2, Hệ quả 2 của Mệnh đề 4). Khi đó $g_1 = g''/{g'}^h$, trong đó $g'' \in A - p$; vì $g'/1$ khả nghịch trong $R_{g'}$, $(g''/1)R_{g'} = 0$, do đó $R_{g'g''} = (R_{g'})_{g''/1} = 0$. Nếu $f = g'g''$, $f \in A - p$, $Q_f = 0$ và $R_f = 0$, nên $u_f$ song ánh.

#### Hệ quả {#ac-ii-s5-n1-cor-1 .statement}

*Nếu $N$ được trình bày hữu hạn và $N_p$ là một $A_p$-môđun tự do có hạng $p$, thì tồn tại $f \in A - p$ sao cho $N$, là một $A_f$-môđun tự do có hạng $p$.*

Theo giả thiết, tồn tại $p$ phần tử $x_i \in \mathbf{N}$ ($1 \leq i \leq p$) sao cho các $x_i/1$ lập thành một cơ sở của $A_,-$-môđun tự do $N_p$. Xét đồng cấu $u : A^p \to \mathbf{N}$ sao cho $u(e_i) = x_i$ với $1 \leq i \leq p$, $(e_i)_{1 \leq i \leq p}$ là cơ sở chính tắc của $A^p$. Vì $u_p$ song ánh theo giả thiết, tồn tại $f \in A - p$ sao cho $u_f$ song ánh, theo Mệnh đề 2.

#### Mệnh đề 3 {#ac-ii-s5-prop-3 .statement}

*Cho* $(f_i)_{i \in I}$ *là một họ hữu hạn các phần tử của một vành* $A$, *sinh iđêan* $A$ *của* $A$. *Vành* $B = \prod_{i \in I} A_i$, *khi đó là một* $A$*-môđun phẳng trung thành*.

Theo § 2, số **4**, Định lý 1, mỗi $A_i$ là một $A$-môđun phẳng, do đó $B$ cũng vậy (Chương I, § 2, no. 3, Mệnh đề 2). Mặt khác, nếu $p$ là một iđêan nguyên tố của $A$, tồn tại một chỉ số $i$ sao cho $f_i \notin p$ và do đó $p_{f_i} = pA_{f_i}$ là một iđêan nguyên tố của $A_{f_i}$. Khi đó $pB \subset pA_{f_i} \times \prod_{j \neq i} A_j \neq B$ vì $pA_{f_i} \neq A_{f_i}$; điều này đủ để suy ra rằng $B$ là một $A$-môđun phẳng trung thành (Chương I, § 3, no. 1, Mệnh đề 1).

#### Hệ quả {#ac-ii-s5-n1-cor-2 .statement}

*Dưới các giả thiết của Mệnh đề 3, đối với một* $A$*-môđun* $M$ *để là sinh hữu hạn (tương ứng, hữu hạn trình bày), điều kiện cần và đủ là, với mọi chỉ số* $i$, *$A_{f_i}$*-môđun* $M_{f_i}$ *là sinh hữu hạn (tương ứng, hữu hạn trình bày)*.

Điều kiện này hiển nhiên là cần thiết (§ 2, số **4**). Ngược lại, nếu tất cả các $M_{f_i}$ đều sinh hữu hạn (tương ứng, hữu hạn trình bày), $M' = \prod_{i \in I} M_{f_i}$ là một $B$-môđun sinh hữu hạn (tương ứng, hữu hạn trình bày), vì hiển nhiên ta có thể giả sử rằng với mỗi $i$ tồn tại một dãy khớp $AT_i \to A^n_{f_i} \to M_{f_i} \to 0$, trong đó $m$ và $n$ độc lập với $i$. Bây giờ, $M' = M \otimes_A B$. Hệ quả suy ra từ Mệnh đề 3 và Chương I, § 3, số **6**, Mệnh đề 11.

Chú ý rằng điều kiện trên các $f_i$ có nghĩa là các tập mở $X_{f_i}$ tạo thành một *phủ* của $\mathrm{Spec}(A)$ (§ 4, no. 3, Hệ quả 3 của Mệnh đề 11).

### 2. ĐẶC TRƯNG HÓA ĐỊA PHƯƠNG CÁC MÔĐUN XẠ ẢNH HỮU HẠN SINH

#### Định lý 1 {#ac-ii-s5-thm-1 .statement}

*Cho* $A$ *là một vành và* $P$ *là một* $A$*-môđun*. *Các tính chất sau là tương đương*:

(a) $P$ *là một môđun xạ ảnh hữu hạn sinh*.
(b) $P$ *là một môđun hữu hạn trình bày và, với mọi iđêan cực đại* $m$ *của* $A$, $P_m$ *là một* $A_m$*-môđun tự do*.
(c) $P$ *là một môđun hữu hạn sinh, với mọi* $p \in \mathrm{Spec}(A)$, *$A_p$*-môđun* $P_p$ *là tự do và, nếu ký hiệu hạng của nó là* $r_p$, *hàm* $p \mapsto r_p$ *là hằng địa phương trong không gian tôpô* $\mathrm{Spec}(A)$ *(nghĩa là, mọi điểm của* $\mathrm{Spec}(A)$ *đều có một lân cận trên đó hàm này là hằng)*.

(d) Tồn tại một họ hữu hạn $(f_i)_{i \in I}$ các phần tử của $A$, sinh iđêan $A$, sao cho, với mọi $i \in I$, $A,$-môđun $P_{f_i}$ là tự do có hạng hữu hạn.

(e) Với mọi iđêan cực đại $m$ của $A$, tồn tại $f \in A - m$ sao cho $P_f$ là một $A,$-môđun tự do có hạng hữu hạn.

Ta chứng minh định lý bằng cách chứng minh sơ đồ các suy luận sau

(a) ⇔ (d)

(b) ⇌ (e)

(c)

(a) ⇒ (b): Ta biết rằng một môđun xạ ảnh sinh hữu hạn là môđun trình bày hữu hạn (Chương I, § 2, no. 8, Bổ đề 8 (iii)); nếu $P$ là một môđun xạ ảnh $A$-môđun, $P_m = P \otimes_A A_m$ là một môđun xạ ảnh $A_m$-môđun (\emph{Algebra}, Chương II, § 5, no. 1, Hệ quả của Mệnh đề 4); cuối cùng, vì $A,$ là một vành địa phương, mọi môđun xạ ảnh trình bày hữu hạn $A,,$-môđun đều tự do (\S 3, no. 2, Hệ quả của Mệnh đề 5).

(b) ⇒ (e): Điều này suy ra từ Hệ quả của Mệnh đề 2 của no. 1.

(c) ⇒ (e): Cho $m$ là một iđêan cực đại của $A$; viết $r_m = n$ và cho $(x_i)_{1 \leq i \leq n}$ là một cơ sở của $P$. Ta có thể giả sử rằng các $x_i$ là các ảnh chính tắc của các phần tử $p_i \in P$ $(1 \leq i \leq n)$ sai khác bởi phép nhân với một phần tử khả nghịch của $A,$. Cho $(e_i)_{1 \leq i \leq n}$ là cơ sở chính tắc của $A^n$ và $u : A^n \to P$ là đồng cấu sao cho $u(e_i) = p_i$ với $1 \leq i \leq n$. Vì $P$ sinh hữu hạn, theo Mệnh đề 2 của no. 1, tồn tại $f \in A - m$ sao cho $u_f$ là toàn ánh. Ta kết luận rằng $u_{f,g}$ cũng toàn ánh với mọi $g \in A - m$ và theo giả thiết tồn tại $g \in A - m$ sao cho $r_p = n$ với $p \in X,$. Khi thay thế $f$ bởi $f g$, ta có thể giả sử rằng $r_p = n$ với mọi $p \in X,$. Khi đó $u_p : A_p^n \to P_p$ là một đồng cấu toàn ánh và $P_p$ và $A_p$ đều là các $A,$-môđun tự do có cùng hạng; do đó (\S 3, no. 2, Hệ quả của Mệnh đề 6) $u_p$ là song ánh với mọi $p \in X_f$. Cho $p'$ là một iđêan nguyên tố của $A,$ và cho $p$ là ảnh ngược của nó trong $A$ qua ánh xạ chính tắc; nếu $(A_f^{n})_{p'}$ và $(P_f)_{p'}$ được đồng nhất với $A_p^n$ và $P_p$ qua các đẳng cấu chính tắc, thì $(u_f)_{p'}$ được đồng nhất với $u_p$ và do đó là song ánh. Ta kết luận rằng $u_f$ là song ánh (\$3, no. 3, Định lý 1), điều này chứng minh (e).

(e) ⇒ (d): Cho $E$ là tập hợp $\in A$ sao cho $P_f$ là một A-môđun tự do sinh hữu hạn $A_f$. Giả thiết suy ra rằng $E$ không được chứa trong bất kỳ iđêan cực đại nào của $A,$ do đó $E$ sinh iđêan $A$ và vì vậy tồn tại một họ hữu hạn $(f_i)_{1 \leq i \leq n}$ các phần tử của $E$ và $a_i \in A$ $(1 \leq i \leq n)$ sao cho $1 = \sum_{i=1}^n a_i f_i$; do đó (d).

(d) ⇒ (c): Theo no. 1, Hệ quả của Mệnh đề 3 suy ra rằng $P$ là sinh hữu hạn. Mặt khác, với mọi iđêan nguyên tố $p$ của $A$, tồn tại một chỉ số $i$ sao cho $p \in X_{f_i}$; nếu $p' = p_{f_i}$, thì $P_p = (P_{f_i})_{p'}$ (\S 2, no. 5, Mệnh đề

10) và do đó theo giả thiết $P_p$ là tự do và có cùng hạng với $P_{f_i}$, điều này chứng minh (c).

(d) ⇒ (a): Xét vành $B = \prod_{i \in I} A_i$ và B-môđun
$$
M = \prod_{i \in I} P_i = P \otimes_A B.
$$
Với mỗi chỉ số $i$, tồn tại một A_i-môđun tự do $L$, sao cho $P_i$ là một nhân tử trực tiếp của $L$, và có thể giả thiết rằng mọi $L$, có cùng hạng; khi đó $L = \prod_{i \in I} L_i$ là một B-môđun tự do mà M là một nhân tử trực tiếp, nói cách khác M là một B-môđun xạ ảnh sinh hữu hạn. Vì B là một A-môđun phẳng trung thành (no. 1, Mệnh đề 3), ta kết luận rằng P là một A-môđun xạ ảnh sinh hữu hạn (Chương I, §3, no. 6, Mệnh đề 12).

#### Hệ quả 1 {#ac-ii-s5-thm-1-cor-1 .statement}

Giả sử các tính chất tương đương của mệnh đề của Định lý 1 được thỏa mãn. Cho m là một số nguyên > 0 sao cho, với mọi họ $(x_i)_{1 \leq i \leq m}$ các phần tử của P, tồn tại một họ $(a_i)_{1 \leq i \leq m}$ các phần tử của A, mà không phải tất cả đều là ước của không và sao cho $\sum_{i=1}^m a_i x_i = 0$. Khi đó, với mọi $p \in \operatorname{Spec}(A)$, $r_p \leq m$.

Cho p là một iđêan nguyên tố của A; đặt $r = r_p$ và cho $(y_j)_{1 \leq j \leq r}$ là một cơ sở của A_p-môđun tự do $P_p$. Tồn tại các phần tử $x_j$ ($1 \leq j \leq r$) của P và $s \in A - p$ sao cho $y_j = x_j / s$ với mọi $j$. Khi đó, với mọi họ $(a_j)_{1 \leq j \leq r}$ các phần tử của A sao cho $\sum_{j=1}^r a_j x_j = 0$, $\sum_{j=1}^r (a_j/1) y_j = 0$ trong $P_p$, do đó $a_j/1 = 0$ với $1 \leq j \leq r$. Vì $A - p$ không chứa 0, điều này chứng tỏ rằng các $a_j$ đều là ước của không trong A (\S 2, no. 1, Nhận xét 3), do đó tất yếu $r \leq m$.

#### Hệ quả 2 {#ac-ii-s5-thm-1-cor-2 .statement}

Mọi môđun phẳng trình bày hữu hạn đều là xạ ảnh.

Nếu P là một A-môđun phẳng trình bày hữu hạn và m là một iđêan cực đại của A, A_m-môđun $P$, là phẳng (\S 3, no. 4, Mệnh đề 13) và trình bày hữu hạn (\S 2, no. 4) và do đó tự do (\$3, no. 2, Hệ quả 2 của Mệnh đề 5), Điều kiện (b) của Định lý 1 do đó được thỏa mãn.

Nhận xét
(1) Tồn tại các môđun phẳng sinh hữu hạn không phải là xạ ảnh (Bài tập 7).
(2) Hệ quả 2 của Định lý 1 mở rộng đến các môđun trên các vành không giao hoán (Chương I, §2, Bài tập 15).

### 3. HẠNG CỦA CÁC MÔĐUN XẠ ẢNH

#### Định nghĩa 1 {#ac-ii-s5-def-1 .statement}

Cho P là một A-môđun xạ ảnh sinh hữu hạn. Với mọi iđêan nguyên tố $p$ của A, hạng của A_p-môđun tự do $P_p$ được gọi là hạng của P tại $p$ và được ký hiệu bởi $\operatorname{rg}_p(P)$.

Theo Định lý 1, hàm nhận giá trị nguyên $p \mapsto \mathrm{rg}_p(P)$ là *hằng địa phương* trên $X = \mathrm{Spec}(A)$; do đó nó là hằng nếu $X$ *liên thông* và đặc biệt nếu vành $A$ là một *miền nguyên* (\S 4, no. 3, Hệ quả 2 của Mệnh đề 15).

#### Định nghĩa 2 {#ac-ii-s5-def-2 .statement}

*Cho $n$ là một số nguyên $\geqslant 0$. Một môđun $A$ xạ ảnh $P$ được gọi là *có hạng* $n$ nếu nó sinh hữu hạn và $\mathrm{rg}_p(P) = n$ với mọi iđêan nguyên tố $p$ của $A$.*

Rõ ràng mọi $A$-môđun *tự do* $L$ sinh hữu hạn đều có hạng $n$ theo nghĩa của Định nghĩa 2, $n$ bằng *chiều* (hay *hạng*) của $L$ được định nghĩa trong *Đại số*, Chương II, \S 7, no. 2.

Một môđun xạ ảnh có hạng 0 là không (\S 3, no. 3, Hệ quả 2 của Định lý 1). Nếu $A$ không rút gọn về 0 và một $A$-môđun xạ ảnh $P$ có hạng $n$, thì số nguyên $n$ được xác định duy nhất; khi đó nó được ký hiệu là $\mathrm{rg}(P)$.

#### Định lý 2 {#ac-ii-s5-thm-2 .statement}

*Cho $P$ là một $A$-môđun và $n$ là một số nguyên $\geqslant 0$. Các tính chất sau là tương đương:*

(a) *$P$ là xạ ảnh có hạng* $n$.

(b) *$P$ sinh hữu hạn và, với mọi iđêan cực đại* $m$ *của* $A$, *$A$-*môđun* $P$, *là tự do có hạng* $n$.

(c) *$P$ sinh hữu hạn và, với mọi iđêan nguyên tố* $p$ *của* $A$, *$A$-*môđun* $P_p$ *là tự do có hạng* $n$.

(d) *Với mọi iđêan cực đại* $m$ *của* $A$, *tồn tại* $f \in A - m$ *sao cho* $A$-*môđun* $P_f$ *là tự do có hạng* $n$.

Theo Định nghĩa 2 và Định lý 1, (a) và (c) là tương đương; (b) suy ra (c), vì, với mọi iđêan nguyên tố $p$ của $A$, tồn tại một iđêan cực đại $m$ chứa $p$ và, đặt $p' = p_m$, $P_p$ đẳng cấu với $(P_m)_{p'}$ (\S 2, no. 5, Mệnh đề 11); nếu $P_m$ là tự do có hạng $n$, thì $P_{p'}$ cũng vậy. Tính chất (c) suy ra (d) theo Định lý 1 và sự kiện rằng, iff $\in A - m$ và $m' = m_f$, $P_m$ đẳng cấu với $(P_f)_{m'}$ và do đó các hạng của $P_f$ và $P$ bằng nhau. Cuối cùng, lập luận sau cùng này và Định lý 1 cho thấy (d) suy ra (b).

#### Nhận xét {#ac-ii-s5-n3-rem-1 .statement}

*Nếu* $A$ *là một miền nguyên, một* $A$-*môđun xạ ảnh có một hạng được xác định tốt* (theo nghĩa của Định nghĩa 2), *như đã nhận thấy ở trên; hơn nữa, hạng này trùng với hạng được định nghĩa trong Đại số, Chương II, \S 7, no. 2; chỉ cần áp dụng Định lý 2 (c) với* $p = (0)$.

Cho $E$ và $F$ là hai $A$-môđun xạ ảnh sinh hữu hạn. Ta biết (*Đại số*, Chương II, §§ 2 và 3) rằng $E \times F$, $E \otimes_A F$, $\mathrm{Hom}_A(E, F)$ và môđun đối ngẫu $E^*$ của $E$ là xạ ảnh và sinh hữu hạn; lũy thừa ngoại $\bigwedge^k E$ cũng vậy với mọi số nguyên $k > 0$ (*Đại số*, Chương 111). Ngoài ra, theo Định nghĩa 1 và \S 2, no. 7, các Mệnh đề 18 và 19 và no. 8, suy ra ngay lập tức rằng, với mọi iđêan nguyên tố $p$ của $A$:

(1)
$$
\mathrm{rg}_p(E \times F) = \mathrm{rg}_p(E) + \mathrm{rg}_p(F)
$$

(2) $\mathrm{rg}_p(E \otimes_A F) = \mathrm{rg}_p(E) \cdot \mathrm{rg}_p(F)$

(3) $\mathrm{rg}_p(\mathrm{Hom}_A(E, F)) = \mathrm{rg}_p(E) \cdot \mathrm{rg}_p(F)$

(4) $\mathrm{rg}_p(E^*) = \mathrm{rg}_p(E)$

(5) $\mathrm{rg}_p(\wedge^k E) = \binom{\mathrm{rg}_p(E)}{k}$.

Nếu các hạng của E và F được xác định, thì các hạng của $E \times F, E \otimes_A F,$ $\mathrm{Hom}_A(E, F), E^*$ và $\wedge^k E$ cũng được xác định và các đẳng thức trên cũng đúng khi bỏ chỉ số $p$. Hơn nữa:

#### Hệ quả {#ac-ii-s5-n3-cor-1 .statement}

*Để một A-môđun xạ ảnh sinh hữu hạn P có hạng n, điều kiện cần và đủ là $\mathbf{A}^n P$ có hạng 1.*

#### Mệnh đề 4 {#ac-ii-s5-prop-4 .statement}

*Cho B là một đại số giao hoán trên A và P là một A-môđun xạ ảnh có hạng n. Khi đó B-môđun $P_{(B)} = B \otimes_A P$ là xạ ảnh có hạng n.*

Ta biết rằng $P_{(B)}$ là xạ ảnh và sinh hữu hạn (*Đại số*, Chương II, § 5, no. 1, Hệ quả của Mệnh đề 4). Nếu q là một iđêan nguyên tố của B và p là ảnh ngược của nó trong A, thì

$$
(P_{(B)})_q = (P \otimes_A B) \otimes_B B_q = P @_A B_q = (P \otimes_A A_i) \otimes_A B_q
$$

và, theo giả thiết, $P \otimes_A A_i$ là một A,-môđun tự do có hạng $n$, $(P_{(B)})_q$ là một $B_q$-môđun tự do có hạng $n$.

#### Mệnh đề 5 {#ac-ii-s5-prop-5 .statement}

*Cho A là một vành bán địa phương và P là một A-môđun xạ ảnh sinh hữu hạn. Nếu hạng của P được xác định, thì P là một A-môđun tự do.*

Trước hết giả sử rằng A đẳng cấu với một tích các trường $K_i$ ($1 \leq i \leq n$). Các $K_i$ khi đó được đồng nhất với các iđêan cực tiểu (*Algebra*, Chương VIII, § 3, no. 1) của A và, với mọi $i$, tổng $p_i$ của các K, có chỉ số $j \neq i$ là một iđêan cực đại của A, các $p_i$ ($1 \leq i \leq n$) là các iđêan nguyên tố duy nhất của A. Mọi A-môđun sinh hữu hạn P do đó là tổng trực tiếp của các thành phần đẳng kiểu của nó $P_i$ ($1 \leq i \leq n$), $P_i$ đẳng cấu với một tổng trực tiếp của một số hữu hạn $r_i$ A-môđun đẳng cấu với K, (*Algebra*, Chương VIII, § 5, no. 1, Mệnh đề 1 và no. 3, Mệnh đề 11); vành $A_{r_i}$ được đồng nhất với K, và linh hóa tử các $P_j$ có chỉ số $j \neq i$, do đó $r_i = \mathrm{rg}_{p_i}(P)$; nếu tất cả các $r_i$ bằng cùng một số $r$, thì P đẳng cấu với $A^r$, do đó có mệnh đề trong trường hợp này. Trong trường hợp tổng quát, đặt $\mathfrak{R}$ là căn Jacobson của A và $B = A / \mathfrak{R}$; vì B là một tích các trường, B-môđun xạ ảnh $P_{(B)}$ là tự do theo các nhận xét đứng trước Mệnh đề 4. *Ngoài ra P là một A-môđun phẳng và khi đó mệnh đề suy ra từ § 3, no. 2, Mệnh đề 5.*

### 4. CÁC MÔĐUN XẠ ẢNH HẠNG 1

#### Định lý 3 {#ac-ii-s5-thm-3 .statement}

Cho $A$ là một vành và $M$ là một A-môđun sinh hữu hạn.

(i) *Nếu tồn tại một A-môđun $N$ sao cho $M \otimes_A N$ đẳng cấu với $A$, thì môđun $M$ là xạ ảnh hạng 1.*

(ii) *Ngược lại, nếu $M$ là xạ ảnh hạng 1 và $M^*$ là đối ngẫu của $M$, thì đồng cấu chính tắc $u : M \otimes_A M^* \to A$ tương ứng với dạng song tuyến tính chính tắc $(x, x^*) \to \langle x, x^* \rangle$ trên $M \times M^*$ (Algebra, Chương II, § 2, no. 3) là song ánh.*

(i) Cần chứng minh rằng, đối với mọi iđêan cực đại $m$ của $A$, A-môđun $M$, là tự do hạng 1 (Định lý 2 (b)); ta tự do thay thế $A$ bởi $A_m$ và do đó có thể giả sử rằng $A$ là một vành *địa phương* ($\S 2$, no. 7, Mệnh đề 18). Đặt $k = A/m$. Đẳng cấu $v : M \otimes_A N \to A$ xác định một đẳng cấu

$$
v \otimes 1_k : (M/mM) \otimes_k (N/mN) \to k
$$

vì hạng trên $k$ của $(M/mM) \otimes_k (N/mN)$ là tích các hạng của $M/mM$ và $N/mN$, các hạng này tất nhiên đều bằng 1, nói cách khác $M/mM$ là đơn sinh. Suy ra rằng $M$ là đơn sinh ($\S 3$, no. 2, Hệ quả 2 của Mệnh đề 4); mặt khác, linh hóa tử của $M$ cũng linh hóa tử $M \otimes_A N$ và do đó bằng không, điều này chứng minh rằng $M$ đẳng cấu với $A$.

(ii) Chỉ cần chứng minh rằng, với mọi iđêan cực đại $m$ của $A$, $u_m$ là một đẳng cấu ($\S 3$, no. 3, Định lý 1). Vì $M$ là sinh hữu hạn trình bày (Chương I, $\S 2$, no. 8, Bổ đề 8), $(M^*)_m$ được đồng nhất một cách chính tắc với đối ngẫu $(M_m)^*$ ($\S 2$, no. 7, Mệnh đề 19) và, vì $M_m$ là tự do hạng 1 như đối ngẫu $(M_m)^*$ của nó, rõ ràng đồng cấu chính tắc $u_m : (M,) \otimes_{A_m} (M_m)^* \to A_m$ là song ánh, điều này hoàn tất chứng minh.

*Nhận xét* (1). Nếu $M$ là xạ ảnh hạng 1 và $N$ là sao cho $M \otimes_A N$ đẳng cấu với $A$, thì $N$ đẳng cấu với $M^*$: có các đẳng cấu

$$
N \to N \otimes A \to N \otimes M \otimes M^* + A \otimes M^* \to M^*.
$$

#### Mệnh đề 6 {#ac-ii-s5-prop-6 .statement}

*Cho $M$ và $N$ là các $A$-môđun xạ ảnh hạng 1. Khi đó $M \otimes_A N$, $\operatorname{Hom}_A(M, N)$ và đối ngẫu $M^*$ của $M$ là các môđun xạ ảnh hạng 1.*

Điều này suy ra ngay lập tức từ các công thức (2), (3) và (4).

Bây giờ ta chú ý rằng mọi $A$-môđun sinh hữu hạn đều đẳng cấu với một môđun thương của $L = \mathbf{A}^{(\mathbf{N})}$; do đó ta có thể nói về *tập hợp $F(A)$ gồm các lớp của các $A$-môđun sinh hữu hạn* đối với đẳng cấu (*Lý thuyết tập hợp*, Chương I, §6, no. 9); ta ký hiệu bởi $P(A)$ tập con của $F(A)$ gồm các lớp của các $A$-môđun xạ ảnh hạng 1 và bởi $\operatorname{cl}(M)$ ảnh trong $P(A)$ của một $A$-môđun xạ ảnh hạng 1 $M$. Hiển nhiên rằng, đối với hai $A$-môđun xạ ảnh $M$,

N hạng 1, cl(M \otimes_A N) chỉ phụ thuộc vào cl(M) và cl(N); theo định nghĩa ta đặt

(6) $$ \mathrm{cl}(M) + \mathrm{cl}(N) = \mathrm{cl}(M \otimes AN) $$

và do đó một luật hợp thành nội tại được xác định trên $P(A)$.

#### Mệnh đề 7 {#ac-ii-s5-prop-7 .statement}

*Tập hợp $P(A)$ các lớp của các A-môđun xạ ảnh hạng 1, với luật hợp thành (6), là một nhóm giao hoán. Nếu M là một A-môđun xạ ảnh hạng 1 và $M^*$ là đối ngẫu của nó, thì*

(7) $$ \mathrm{cl}(M^*) = -\mathrm{cl}(M) \quad \text{và} \quad \mathrm{cl}(A) = 0. $$

Tính kết hợp và tính giao hoán của tích tenxơ chỉ ra rằng luật hợp thành (6) là kết hợp và giao hoán; đẳng cấu giữa $A \otimes_A M$ và M chứng minh rằng $\mathrm{cl}(A)$ là phần tử đơn vị đối với luật này và, theo Định lý 3, $\mathrm{cl}(M) + \mathrm{cl}(M^*) = \mathrm{cl}(A)$, do đó có mệnh đề.

Cho B là một A-đại số giao hoán và M là một A-môđun xạ ảnh hạng 1; khi đó $M_{(B)} = B \otimes_A M$ là một B-môđun xạ ảnh hạng 1 (no. 3, Mệnh đề 4). Khi đó tồn tại một ánh xạ được gọi là chính tắc $\phi : P(A) \to P(B)$ sao cho

(8) $$ \phi(\mathrm{cl}(M)) = \mathrm{cl}(M_{(B)}). $$

Đẳng thức $M_{(B)} \otimes_B N_{(B)} = (M \otimes_A N)_{(B)}$ đối với hai A-môđun M, N chứng minh rằng ánh xạ $\phi$ là một *đồng cấu* nhóm giao hoán.

*Nhận xét (2).* Điều kiện (e) của Định lý 1 (tương đương với việc P là xạ ảnh và sinh hữu hạn) cũng có thể được phát biểu bằng cách nói rằng *bó các môđun* $\tilde{P}$ trên $X = \mathrm{Spec}(A)$ *liên kết(*) với P là tự do địa phương và kiểu hữu hạn* và do đó có thể được diễn giải như bó các tiết diện của một bó vectơ trên X. Ngược lại, mọi bó vectơ trên X đều phát sinh từ một môđun xạ ảnh hữu hạn sinh, môđun này được xác định tới một đẳng cấu duy nhất; vì thế các môđun xạ ảnh hạng $n$ tương ứng với các bó vectơ mà mọi thớ của chúng đều có chiều $n$. Đặc biệt, các bó vectơ hạng 1 tương ứng với các môđun xạ ảnh hạng 1. Nếu ký hiệu bởi $\mathcal{O}_X$ bó cấu trúc $\tilde{A}$ và bởi $\mathcal{O}_X^*$ *bó các đơn vị* của $\mathcal{O}_X$ (mà các tiết diện của nó trên một tập mở U của X là các phần tử khả nghịch của vành các tiết diện của $\mathcal{O}_X$ trên U), thì suy ra rằng nhóm $P(A)$ đẳng cấu với nhóm đối đồng điều bậc nhất $H^1(X, \mathcal{O}_X^*)$.*

(* Xem A. Grothendieck, Éléments de géométrie algébrique, I (\S 1) (Publ. Math. I.H.E.S., no. 4, 1960).

### 5. CÁC MÔĐUN CON KHÔNG SUY BIẾN

Trong số này và hai số tiếp theo, $A$ ký hiệu một vành, $S$ một tập con nhân tính của $A$ gồm các phần tử không là ước của không trong $A$, và $B$ là vành $S^{-1}A$; $A$ được đồng nhất một cách chính tắc với một vành con của $B$ ($\S 2$, no. 1, Nhận xét 3). Do đó các phần tử của $S$ là khả nghịch trong $B$.

Một trong những trường hợp riêng quan trọng nhất đối với các ứng dụng là trường hợp $A$ là một miền nguyên và $S$ là tập hợp các phần tử $\neq 0$ của $A$; khi đó $B$ là trường phân thức của $A$.

#### Định nghĩa 3 {#ac-ii-s5-def-3 .statement}

Cho $M$ là một A-môđun con của $B$. $M$ được gọi là không suy biến nếu $B.M = B$.

Nếu $B$ là một trường, điều kiện này đơn giản có nghĩa là $M$ không bị thu về 0.

#### Mệnh đề 8 {#ac-ii-s5-prop-8 .statement}

Cho $M$ là một A-môđun con của $B$. Các điều kiện sau là tương đương:
(a) $M$ là không suy biến.
(b) $M$ giao với $S$.
(c) Nếu $j : M \to B$ là đơn ánh chính tắc, thì đồng cấu $u = S^{-1}j : S^{-1}M \to B$ là song ánh.

(a) suy ra (b), vì nếu $B.M = B$, thì tồn tại $a \in A, s \in S$ và $x \in M$ sao cho $(a/s)x = 1$, do đó $ax = s$ thuộc $S \cap M$. Để thấy rằng (b) suy ra (c), chú ý rằng $u$ đã là đơn ánh ($\S 2$, no. 4, Định lý 1); hơn nữa, nếu $x \in M \cap S$, thì ảnh qua $u$ của $x/x \in S^{-1}M$ trong $B$ bằng 1 và do đó $u$ là toàn ánh. Cuối cùng, (c) rõ ràng suy ra (a).

#### Hệ quả {#ac-ii-s5-n5-cor-1 .statement}

Nếu $M$ và $N$ là hai A-môđun con không suy biến của $B$, thì các A-môđun $M + N, M.N$ và $M \cap N$ đều không suy biến.

Mệnh đề là tầm thường đối với $M + N$; mặt khác nếu $s \in S \cap M$ và $t \in S \cap N$, thì $st \in S \cap (M.N)$ và $st \in S \cap (M \cap N)$.

Cho hai môđun con-A $M$ và $N$ của $B$, ký hiệu $N : M$ là môđun con-A của $B$ gồm các $b \in B$ sao cho $bM \subset N$ (Chương I, $\S 2$, no. 10, Nhận xét). Nếu mỗi $b \in N : M$ được ánh xạ tới đồng cấu $h_b : x \mapsto bx$ từ $M$ vào $N$, thì thu được một đồng cấu chính tắc $b \mapsto h_b$ từ $N : M$ tới $\operatorname{Hom}_A(M, N)$.

#### Mệnh đề 9 {#ac-ii-s5-prop-9 .statement}

Cho $M, N$ là hai môđun con-A của $B$. Nếu $M$ không suy biến, thì đồng cấu chính tắc từ $N : M$ tới $\operatorname{Hom}_A(M, N)$ là song ánh.

Lấy $s \in S \cap M$. Nếu $b \in N : M$ sao cho $bx = 0$ với mọi $x \in M$, thì $bs = 0$, do đó $b = 0$ vì $s$ không phải là một ước của 0 trong $B$. Mặt khác, cho f \in \mathrm{Hom}_A(M, N) \text{ và đặt } b = f(s)/s; \text{ với mọi } x \in M, \text{ tồn tại } t \in S \text{ sao cho } tx \in A. \text{ Khi đó}
$$
f(x) = s^{-1}t^{-1}f(stx) = s^{-1}t^{-1}txf(s) = bx,
$$
do đó $b \in N : M$ và $f = h_b$, điều này chứng minh mệnh đề.

#### Nhận xét {#ac-ii-s5-n5-rem-1 .statement}

Đặc biệt, $A : M$ được đồng nhất một cách chính tắc với đối ngẫu $M^*$ của $M$, dạng song tuyến tính chính tắc trên $M \times M^*$ được đồng nhất với hạn chế lên $M \times (A : M)$ của phép nhân $B \times B \to B$.

### 6. CÁC MÔĐUN CON KHẢ NGHỊCH

(Ta giữ nguyên ký hiệu của no. 5.)

#### Định nghĩa 4 {#ac-ii-s5-def-4 .statement}

*Một môđun con*-A $M$ của $B$ được gọi là khả nghịch nếu tồn tại một *môđun con*-A $N$ của $B$ sao cho $M.N = A$.

#### Ví dụ {#ac-ii-s5-n6-exa-1 .statement}

Nếu $b$ là một phần tử khả nghịch của $B$, thì $A$-môđun $Ab$ là khả nghịch, như thấy được bằng cách lấy $N = Ab^{-1}$.

#### Mệnh đề 10 {#ac-ii-s5-prop-10 .statement}

*Cho $M$ là một môđun con*-A*-môđun khả nghịch của $B$. Khi đó:
(i) Tồn tại $s \in S$ sao cho $As \subset M \subset As^{-1}$ (và đặc biệt $M$ là không suy biến).
(ii) $A : M$ là *môđun con*-A*-môđun* duy nhất $N$ của $B$ sao cho $M.N = A$.

Nếu $M.N = A$, thì $B.M = B.(B.M) \supset B.(M.N) = B.A = B$, do đó $M$ là không suy biến. Tương tự $N$ là không suy biến. Nếu $t \in S \cap M$ và $u \in S \cap N$ (no. 5, Mệnh đề 8 ), phần tử $s = tu$ thuộc $S \cap M \cap N$, do đó $Ms \subset M.N = A$ và vì thế $As \subset M \subset As^{-1}$.
Mặt khác, hiển nhiên $N \subset A : M$, do đó
$$
A = M.N \subset M.(A : M) \subset A
$$
và $M.(A : M) = A$; nhân hai vế với $N$, ta suy ra $A : M = N$, điều này hoàn tất chứng minh.

#### Định lý 4 {#ac-ii-s5-thm-4 .statement}

*Cho $M$ là một môđun con*-A*-môđun* không suy biến của $B$. *Các tính chất sau là tương đương*:
(a) $M$ là khả nghịch.
(b) $M$ là xạ ảnh.
(c) $M$ là xạ ảnh hạng 1.
(d) $M$ là một $A$-môđun sinh hữu hạn và, với mọi iđêan cực đại $m$ của $A$, $A_m$-môđun $M_m$ là đơn sinh.

Trước hết ta chứng minh sự tương đương của các tính chất (a), (b) và (c). Nếu (a) đúng và $N$ là môđun con-A-môđun của $B$ sao cho M . N = A, thì tồn tại một quan hệ

$$
\sum_{i=1}^{p} m_i n_i = 1 \quad (m_i \in M, n_i \in N \text{ với mọi } i).
$$

Với mọi $x \in M$, đặt $v_i(x) = n_i x$; các $v_i$ là các dạng tuyến tính trên M và theo (9) $x = \sum_{i=1}^{n} m_i v_i(x)$ với mọi $x \in M$; điều này chứng minh (Đại số, Chương 11, §2, no. 6, Mệnh đề 12) rằng M là xạ ảnh và được sinh bởi các $m_i$; do đó M là một môđun xạ ảnh hữu hạn sinh.

Cho m là một iđêan cực đại của A; ta chứng minh rằng số nguyên $r = \mathrm{rg}_m(M)$ bằng 1. Gọi S' là ảnh của S trong $\mathbf{A}_{m'}$; vì các phần tử của S không là các ước của 0 trong A, nên các phần tử của S' không là các ước của 0 trong $\mathbf{A}_{m'}$ vì $\mathbf{A}_{m'}$ là một A-môđun phẳng (\S 2, no. 4, Định lý 1 và Chương I, §2, no. 4, Mệnh đề 3); khi đó ${S'}^{-1}A_m \neq 0$ và, vì $M_m$ là một $A_m$-môđun tự do có hạng $r$, ${S'}^{-1}M_m$ là một ${S'}^{-1}A_m$-môđun tự do có hạng $r$. Nhưng nếu T' là ảnh của A $-m$ trong $S^{-1}A$, thì ${S'}^{-1}A$, (tương ứng ${S'}^{-1}M_m$) được đồng nhất một cách chính tắc với ${T'}^{-1}(S^{-1}A)$ (tương ứng ${T'}^{-1}(S^{-1}M)$) (\S 2, no. 3, Mệnh đề 7). Bây giờ $S^{-1}M = B$ (Mệnh đề 8 (c)) và do đó ${T'}^{-1}(S^{-1}M)$ là một A-môđun tự do có hạng 1 trên ${T'}^{-1}(S^{-1}A)$, điều này chứng minh rằng $r = 1$ và chỉ ra kéo theo (a) $\Rightarrow$ (c).

Kéo theo (c) $\Rightarrow$ (b) là tầm thường. Ta hãy chứng minh rằng (b) $\Rightarrow$ (a). Theo giả thiết, tồn tại một họ (không nhất thiết hữu hạn) $(f_\lambda)_{\lambda \in L}$ các dạng tuyến tính trên M và một họ $(m_\lambda)_{\lambda \in L}$ các phần tử của M sao cho, với mọi $x \in M$, họ $(f_\lambda(x))$ có giá hữu hạn và $x = \sum_{\lambda \in L} m_\lambda f_\lambda(x)$ (Đại số, Chương II, §2, no. 6, Mệnh đề 12). Vì M không suy biến, $f_\lambda(x) = n_\lambda x$ với một $n_\lambda \in A$: M theo Mệnh đề 9 của no. 5. Lấy x là một phần tử của M $\cap S$ (no. 5, Mệnh đề 8), ta thấy tất yếu rằng $n_\lambda = 0$ ngoại trừ một số hữu hạn các chỉ số và $\sum_{\lambda \in L} m_\lambda n_\lambda = 1$. Điều này hiển nhiên kéo theo M . (A: M) = A, do đó có (a).

Theo Định nghĩa 2 của no. 3, (c) kéo theo (d). Ta hãy chứng minh đảo lại. Vì M không suy biến, linh hóa tử của nó là không (Mệnh đề 8 (b)), do đó linh hóa tử của $M_m$ cũng vậy (\S 2, no. 4, công thức (9)). Vì M, được giả thiết là một &-môđun đơn sinh, nên nó là tự do có hạng 1 và từ no. 3, Định lý 2 suy ra rằng M là xạ ảnh có hạng 1.

#### Hệ quả {#ac-ii-s5-n6-cor-1 .statement}

Mọi môđun con khả nghịch của B đều phẳng và có trình bày hữu hạn.
Điều này suy ra từ Định lý 4 (c).

#### Mệnh đề 11 {#ac-ii-s5-prop-11 .statement}

Cho M, N là hai A-môđun con của B. Giả sử rằng M là khả nghịch. Khi đó:
(i) Đồng cấu chính tắc $M \otimes_A N \to M . N$ là song ánh.
(ii) $N : M = N . (A : M)$ và $N = (N : M) . M$.

Gọi $j$ là đơn ánh chính tắc $N \to B$. Vì $M$ là một A-môđun phẳng (Hệ quả của Định lý 4), $1 \otimes j : M \otimes_A N \to M \otimes_A B$ là đơn ánh. Nhưng, vì $B = S^{-1}A$, B-môđun $M \otimes_A B$ bằng $S^{-1}M$ và do đó được đồng nhất với B vì M không suy biến (no. 5, Mệnh đề 8). Nếu thực hiện sự đồng nhất này, ảnh của $1 \otimes j$ là $M . N$, do đó có (i).

Đặt $M' = A : M$. Khi đó hiển nhiên $M'.N \subset N : M$ và $M.(N : M) \subset N$. Mặt khác, vì $M.M' = A$ (Mệnh đề 10),

$$
N : M = M'.M.(N : M) \subset M'.N
$$

và $N = M.M'.N \subset M.(N : M)$, do đó có (ii).

#### Nhận xét {#ac-ii-s5-n6-rem-1 .statement}

Chứng minh của (i) trong Mệnh đề 11 chỉ sử dụng sự kiện rằng $M$ là phẳng và không suy biến.

### 7. NHÓM CÁC LỚP CỦA CÁC MÔĐUN KHẢ NGHỊCH

(Ta giữ ký hiệu của các no. 5 và 6.)

Dưới phép nhân, các A-môđun con của B lập thành một nửa nhóm giao hoán $\mathfrak{m}$, với A là phần tử đơn vị. Khi đó các môđun khả nghịch là các phần tử khả nghịch của $\mathfrak{m}$ và do đó lập thành một nhóm giao hoán $\mathfrak{z}$. Ta đã thấy (no. 6, Mệnh đề 10) rằng nghịch đảo của $M \in \mathfrak{z}$ là $A : M$.

Cho $A^*$ (resp. $B^*$) là nhóm nhân của các phần tử khả nghịch của A (resp. B) và ký hiệu $u$ là đơn ánh chính tắc $A + B$. Với mọi $b \in B^*$, $\theta(b) = bA$ là một A-môđun con khả nghịch. Ánh xạ $\theta : B^* \to \mathfrak{g}$ là một đồng cấu có hạt nhân là $u(A^*)$; đối hạt nhân của nó sẽ được ký hiệu là $\mathfrak{c}$ hoặc $\mathfrak{c}(A)$. Nhóm $\mathfrak{c}$ được gọi là nhóm các lớp của các A-môđun con khả nghịch của B. Dãy khớp sau đây đã được xây dựng

$$
\text{(10)} \quad (1) \longrightarrow A^* \xrightarrow{u} B^* \xrightarrow{\theta} \mathfrak{g} \xrightarrow{\rho} \mathfrak{c} \longrightarrow (1)
$$

trong đó (1) ký hiệu nhóm chỉ gồm phần tử đơn vị và $\rho$ là ánh xạ chính tắc $\mathfrak{g} \to \mathfrak{c} = \mathfrak{g}/\theta(B^*)$.

Vì mọi A-môđun con khả nghịch M của B đều là xạ ảnh có hạng 1 (no. 6, Định lý 4), phần tử $cl(M) \in P(A)$ được xác định (no. 4).

#### Mệnh đề 12 {#ac-ii-s5-prop-12 .statement}

*Ánh xạ* $cl : \mathfrak{g} \to P(A)$ *xác định, bằng cách lấy thương, một đẳng cấu từ* $\mathfrak{c} = \mathfrak{g}/\theta(B^*)$ *lên hạt nhân của đồng cấu chính tắc*

$$
\phi : P(A) \to P(B)
$$

(no. 4).

Nói cách khác, có một dãy khớp

$$
\text{(11)} \quad (1) \longrightarrow A^* \xrightarrow{u} B^* \xrightarrow{\theta} \mathfrak{g} \xrightarrow{cl} P(A) \xrightarrow{\phi} P(B).
$$

Từ Mệnh đề 11 của no. 6 và định nghĩa phép cộng trong $P(A)$ suy ra rằng $cl(M.N) = cl(M) + cl(N)$ với $M, N$ trong $\mathbf{3}$, điều này cho thấy $cl$ là một đồng cấu. Nếu $M \in \mathfrak{J}$ đẳng cấu với $A$, thì tồn tại $b \in B$ sao cho $M = Ab$ và, vì $M$ khả nghịch, tồn tại $b' \in B$ sao cho $b'b = 1$, nói cách khác $b$ khả nghịch trong $B$; đảo lại là ngay lập tức. Do đó hạt nhân của $cl$ trong $\mathfrak{J}$ là $\theta(B^*)$.

Bây giờ ta xác định ảnh của $cl$. Nếu $M \in \mathfrak{J}$, thì $M \otimes_A B = S^{-1}M = B$ (no. 5, Mệnh đề 8 (c)), do đó $cl(M) \in \mathrm{Ker}(\phi)$. Ngược lại, cho $P$ là một $A$-môđun xạ ảnh hạng 1 sao cho $P_{(B)} = P \otimes_A B$ là đẳng cấu với $B$-môđun $B$. Vì $P$ là một $A$-môđun phẳng, đơn ánh $u : A \to B$ xác định một đơn ánh $u \otimes 1 : P \to P_{(B)} = B$ và do đó $P$ được đồng nhất với một môđun con-$A$ của $B$; theo Mệnh đề 8 (c) của no. 5, $P$ là không suy biến và Định lý 4 của no. 6 cho thấy rằng $P$ là khả nghịch. Hạt nhân của $\phi$ vì vậy bằng ảnh của $cl : \mathfrak{J} \to P(A)$.

#### Hệ quả 1 {#ac-ii-s5-prop-12-cor-1 .statement}

*Đối với hai môđun con-$A$ khả nghịch của B có cùng ảnh trong $\mathfrak{C}$, điều kiện cần và đủ là chúng đẳng cấu.*

#### Hệ quả 2 {#ac-ii-s5-prop-12-cor-2 .statement}

*Nếu vành $B$ là nửa địa phương, nhóm $\mathfrak{C}$ các lớp của các môđun con-$A$ khả nghịch của B được đồng nhất một cách chính tắc với nhóm $P(A)$ các lớp của các $A$-môđun xạ ảnh hạng 1.*

Trong trường hợp này $P(B) = 0$ (no. 3, Mệnh đề 5).

#### Nhận xét {#ac-ii-s5-n7-rem-1 .statement}

Giả thiết của Hệ quả 2 được thỏa mãn trong hai trường hợp sau:

(1) $A$ là một miền nguyên và $S$ là tập hợp các phần tử $\neq 0$ của $A$, khi đó $B$ là trường phân thức của $A$. Các môđun con-$A$ khả nghịch của $B$ còn được gọi trong trường hợp này là *các iđêan phân thức khả nghịch*; các môđun trong số đó là các $A$-môđun tự do đơn sinh $Ab$ ($b \# 0$ trong $B$) chính là *các iđêan chính phân thức* được định nghĩa trong *Đại số*, Chương VI, § 1, no. 5.

*(2)* Vành $A$ là Noether và $S$ là tập hợp các phần tử của $A$ không phải là các ước của 0 sao cho $B$ là vành phân thức toàn phần của $A$. Trong trường hợp này $S = A - \bigcup p_i$, trong đó các $p_i$ là các phần tử (có số lượng hữu hạn) của $\mathrm{Ass}(A)$ (Chương IV, § 1), do đó $B$ là nửa địa phương (§ 3, no. 5, Mệnh đề 17).*

### Bài tập {#ac-ii-s5-exercises}

Xem các [bài tập cho § 5](exercises/s5/).
