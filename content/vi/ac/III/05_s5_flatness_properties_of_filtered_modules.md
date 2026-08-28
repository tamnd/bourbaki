---
book: ac
book_title: Commutative Algebra
chapter: III
chapter_title: GRADUATIONS. FILTRATIONS AND TOPOLOGIES
section: 5
section_title: Flatness properties of filtered modules
lang: vi
source: ac-i-vii
book_pages: 226-231, 259-260
pdf_pages: 0246-0251, 0279-0280
extraction: ocr
subsections:
    - "no": 1
      title: IDEALLY HAUSDORFF MODULES
      page: 226
      pdf_page: 246
    - "no": 2
      title: STATEMENT OF THE FLATNESS CRITERION
      page: 227
      pdf_page: 247
    - "no": 3
      title: PROOF OF THE FLATNESS CRITERION
      page: 228
      pdf_page: 248
    - "no": 4
      title: APPLICATIONS
      page: 230
      pdf_page: 250
statements: 11
exercises: 8
content_sha256: ed052c99d8c3a50811b8f1ff8f03716d836cf68bdcffb15e8b06b5514252a9b4
translated_from: content/en/ac/III/05_s5_flatness_properties_of_filtered_modules.md
source_content_sha256: ecfeb5870aae5a62e0cd6ec8aeeeb2de8dc1a67bcfdae539b9dd6ae798043826
translation_model: gpt-5-6-mini
translation_run: translate-vi-dabaaa90
glossary_version: 34
glossary_terms_sha256: 06d13f8a54b0a5e1233fee303228cda56676c3d0ece76e1e7350793f912feb01
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 5. CÁC TÍNH CHẤT PHẲNG CỦA CÁC MÔĐUN LỌC

### 1. CÁC MÔĐUN HAUSDORFF THEO IĐÊAN

#### Định nghĩa 1 {#ac-iii-s5-def-1 .statement}

*Cho A là một vành giao hoán và $\mathfrak{g}$ là một iđêan của A. Một A-môđun M được gọi là Hausdorff theo iđêan đối với 3 (hoặc đơn giản là Hausdorff theo iđêan nếu không có sự nhập nhằng) nếu, với mọi iđêan $\mathfrak{a}$ sinh hữu hạn của A, A-môđun $\mathfrak{a} \otimes_A M$ là Hausdorff đối với tôpô 3-adic.*

Đặt $\mathfrak{a} = A$ trong định nghĩa này, ta đã thấy rằng M nhất thiết là *Hausdorff* đối với tôpô 3-adic.

*Các ví dụ*

#### Ví dụ 1 {#ac-iii-s5-n1-exa-1 .statement}

Nếu A là Noether và $\mathfrak{g}$ được chứa trong căn Jacobson của A (nói cách khác nếu A là một vành Zariski với tôpô 3-adic), mọi A-môđun *sinh hữu hạn* đều là Hausdorff theo iđêan (*§3*, no. 3, Mệnh đề 6).

#### Ví dụ 2 {#ac-iii-s5-n1-exa-2 .statement}

Mọi tổng trực tiếp của các môđun Hausdorff theo iđêan đều là một môđun Hausdorff theo iđêan, nhờ các quan hệ
$$
\mathfrak{g}^n \left( a \otimes_A \bigoplus_{\lambda \in L} M_\lambda \right) = \mathfrak{g}^n \bigoplus_{\lambda \in L} (a \otimes_A M_\lambda) = \bigoplus_{\lambda \in L} \mathfrak{g}^n (a \otimes_A M_\lambda).
$$

#### Ví dụ 3 {#ac-iii-s5-n1-exa-3 .statement}

Nếu một A-môđun M là phẳng và Hausdorff đối với tôpô $\mathfrak{g}$-adic thì nó là Hausdorff theo iđêan, vì $a \otimes_A M$ khi đó được đồng nhất với một môđun con của M và tôpô $\mathfrak{g}$-adic trên $a \otimes_A M$ mịn hơn tôpô cảm sinh trên $a \otimes_A M$ bởi tôpô $\mathfrak{g}$-adic trên M, tôpô này là Hausdorff theo giả thiết.

### 2. PHÁT BIỂU CỦA TIÊU CHUẨN PHẲNG

Cho A là một vành, $\mathfrak{z}$ là một iđêan hai phía của A, M là một môđun trái và gr(A) và gr(M) lần lượt là vành phân bậc và môđun gr(A)-phân bậc liên kết với vành A và với môđun M cùng với các lọc $\mathfrak{g}$-adic (§ 2, no. 3). Ta đã thấy (loc. cit.) rằng với mọi số nguyên $n \geq 0$ tồn tại một đồng cấu môđun $\mathbf{Z}$ toàn ánh
$$
\gamma_n : (\mathfrak{g}^n / \mathfrak{g}^{n+1}) \otimes_{A/\mathfrak{g}} (M / \mathfrak{g}M) \to \mathfrak{g}^n M / \mathfrak{g}^{n+1} M
$$
và một đồng cấu phân bậc bậc 0 của các môđun gr(A)-phân bậc
$$
\gamma_M : \mathrm{gr}(A) \otimes_{\mathrm{gr}_0(A)} \mathrm{gr}_0(M) \to \mathrm{gr}(M)
$$
mà hạn chế của nó lên $\mathrm{gr}_n(A) \otimes_{\mathrm{gr}_0(A)} \mathrm{gr}_0(M)$ là $\gamma_n$ với mọi $n$ và do đó là toàn ánh.

#### Định lý 1 {#ac-iii-s5-thm-1 .statement}

Cho A là một vành giao hoán, $\mathfrak{g}$ là một iđêan của A và M là một A-môđun. Xét các tính chất sau:
(i) M là một A-môđun phẳng.
(ii) $\mathrm{Tor}_1^A(N, M) = 0$ với mọi A-môđun N bị triệt tiêu bởi $\mathfrak{z}$.
(iii) $M / \mathfrak{g}M$ là môđun phẳng $(A / \mathfrak{g})$ và ánh xạ chính tắc $\mathfrak{z} \otimes_A M \to \mathfrak{g}M$ là song ánh (điều kiện sau tương đương với $\mathrm{Tor}_1^A(A / \mathfrak{g}, M) = 0$ nhờ quan hệ $\mathrm{Tor}_1^A(A, M) = 0$ và dãy khớp
$$
\mathrm{Tor}_1^A(A, M) \to \mathrm{Tor}_1^A(A / \mathfrak{g}, M) \to \mathfrak{z} \otimes_A M \to M ).
$$
(iv) $M / \mathfrak{g}M$ là môđun phẳng $(A / \mathfrak{g})$ và đồng cấu chính tắc
$$
\gamma_M : \mathrm{gr}(A) \otimes_{\mathrm{gr}_0(A)} \mathrm{gr}_0(M) \to \mathrm{gr}(M)
$$
là song ánh (tính chất (GR) của § 2, no. 8).
(v) Với mọi $n \geq 1$, $M / \mathfrak{g}^n M$ là môđun phẳng $(A / \mathfrak{g}^n)$.
Khi đó (i) $\Rightarrow$ (ii) $\Leftrightarrow$ (iii) $\Rightarrow$ (iv) $\Leftrightarrow$ (v).
Nếu thêm $\mathfrak{g}$ là lũy linh hoặc nếu A là Noether và M là Hausdorff theo iđêan, các tính chất (i), (ii), (iii), (iv) và (v) là tương đương.

#### Nhận xét {#ac-iii-s5-n1-rem-1 .statement}

Nếu $A / \mathfrak{g}$ là một trường (như thường xảy ra trong các ứng dụng) thì điều kiện "M/ $\mathfrak{g}M$ là một môđun phẳng $(A / \mathfrak{g})$" tự động đúng với mọi A-môđun M, điều này làm đơn giản hóa phát biểu của các tính chất (iii) và (iv); hơn nữa, trong trường hợp này, tính chất (v) tương đương với việc nói rằng $M / \mathfrak{g}^n M$ là một môđun tự do $(A / \mathfrak{g}^n)$ với mọi số nguyên $n \geq 1$ (Chương 11, § 3, no. 2, Hệ quả 2 của Mệnh đề 5).

### 3. CHỨNG MINH TIÊU CHUẨN PHẲNG

(A) *Các kéo theo* (i) $\Rightarrow$ (ii) $\Leftrightarrow$ (iii)

Kéo theo (i) $\Rightarrow$ (ii) là ngay lập tức (Chương I, § 4). Sự tương đương (ii) $\Leftrightarrow$ (iii) là một trường hợp đặc biệt của Chương I, § 4, Mệnh đề 2 áp dụng cho $R = A, S = A/\mathfrak{g}, F = M, E = N$, có tính đến sự kiện rằng việc cho một cấu trúc môđun $(A/\mathfrak{g})$ trên N tương đương với việc cho một cấu trúc A-môđun mà theo đó N bị triệt tiêu bởi 3.

*Nhận xét* (1). Điều kiện (ii) cũng tương đương với điều sau:

(ii') $\operatorname{Tor}_1^A(N, M) = 0$ *với mọi* $A$*-môđun* $N$ *bị triệt tiêu bởi một lũy thừa của* 3.

Rõ ràng (ii') suy ra (ii). Ngược lại, nếu (ii) đúng, thì đặc biệt $\operatorname{Tor}_1^A(\mathfrak{g}^n N / \mathfrak{g}^{n+1} N, M) = 0$ với mọi $n$; từ dãy khớp
$$
0 \to \mathfrak{g}^{n+1} N \to \mathfrak{g}^n N \to \mathfrak{g}^n N / \mathfrak{g}^{n+1} N \to 0
$$
ta suy ra dãy khớp
$$
\operatorname{Tor}_1^A(\mathfrak{g}^{n+1} N, M) \to \operatorname{Tor}_1^A(\mathfrak{g}^n N, M) \to \operatorname{Tor}_1^A(\mathfrak{g}^n N / \mathfrak{g}^{n+1} N, M)
$$
và, vì tồn tại một số nguyên $m$ sao cho $\mathfrak{g}^m N = 0$, ta suy ra bằng quy nạp lùi theo $n$ rằng $\operatorname{Tor}_1^A(\mathfrak{g}^n N, M) = 0$ với mọi $n \leq m$ và đặc biệt với $n = 0$.

Từ đó suy ra rằng nếu 9 là *lũy linh*, (ii) suy ra (i), vì (ii') khi đó có nghĩa là $\operatorname{Tor}_1^A(N, M) = 0$ đối với *mọi* $A$*-môđun* $N$ và do đó $M$ là phẳng (Chương I, § 4).

(B) Ta hãy chứng minh mệnh đề sau:

#### Mệnh đề 1 {#ac-iii-s5-prop-1 .statement}

*Cho* $A$ *là một vành giao hoán, 3 là một iđêan của* $A$ *và* $M$ *là một* $A$*-môđun*. *Các điều kiện sau là tương đương*:
(a) *Với mọi* $n \geq 1$, $\operatorname{Tor}_1^A(A/\mathfrak{g}^n, M) = 0$.
(b) *Với mọi* $n \geq 1$, *đồng cấu chính tắc*
$$
\theta_n : \mathfrak{g}^n \otimes_A M \to \mathfrak{g}^n M
$$
*là song ánh*.

*Hơn nữa các điều kiện này kéo theo* :
(c) *Đồng cấu chính tắc* $\gamma_M : \operatorname{gr}(A) \otimes_{\operatorname{gr}_0(A)} \operatorname{gr}_r(M) \to \operatorname{gr}(M)$ *là song ánh*. *Ngược lại, nếu* $\mathfrak{g}$ *là lũy linh, (c) suy ra (a) và (b)*.

Sự tương đương của (a) và (b) suy ra từ dãy khớp
$$
0 = \operatorname{Tor}_1^A(A, M) \to \operatorname{Tor}_1^A(A/\mathfrak{g}^n, M) \to \mathfrak{g}^n \otimes_A M \to M.
$$

Xét tiếp biểu đồ
$$
\begin{array}{ccccccccc}
\mathfrak{g}^{n+1} \otimes_A M & \longrightarrow & \mathfrak{g}^n \otimes_A M & \longrightarrow & (\mathfrak{g}^n / \mathfrak{g}^{n+1}) \otimes_A (M / \mathfrak{g} M) & \longrightarrow & 0 \\
\downarrow \theta_{n+1} & & \downarrow \theta_n & & \downarrow \gamma_n & & \\
0 & \longrightarrow & \mathfrak{g}^{n+1} M & \longrightarrow & \mathfrak{g}^n M & \longrightarrow & \operatorname{gr}_n(M) & \longrightarrow & 0
\end{array}
$$

trong đó ta chú ý rằng $(\mathfrak{g}^n/\mathfrak{g}^{n+1}) \otimes_A (M/\mathfrak{g}M)$ được đồng nhất một cách chính tắc với $(\mathfrak{g}^n/\mathfrak{g}^{n+1}) \otimes_{A/\mathfrak{g}} (M/\mathfrak{g}M)$. Biểu đồ này giao hoán theo định nghĩa của $\gamma_n$ và các hàng của nó là khớp. Nếu (b) đúng, $0$, và $\theta_{n+1}$ là song ánh và do đó $\gamma_n$ cũng là song ánh theo định nghĩa của đối hạt nhân, vì vậy (b) suy ra (c). Ngược lại, giả sử rằng $\mathfrak{g}$ là lũy linh, ta hãy chứng minh rằng (c) suy ra (b); ta sẽ lập luận bằng quy nạp lùi theo $n$, vì $\mathfrak{g}^n \otimes_A M = \mathfrak{g}^n M = 0$ với $n$ đủ lớn. Giả sử khi đó rằng trong biểu đồ (1), $\gamma_n$ và $\theta_{n+1}$ là song ánh; khi đó $\theta_n$ cũng là song ánh theo Chương I, § 1, no. 4, Hệ quả 1 của Mệnh đề 2.

(C) *Hệ quả* (ii) $\Rightarrow$ (iv)

Nếu (ii) đúng, thì (ii') cũng đúng theo *Nhận xét* 1; Mệnh đề 1 khi đó chỉ ra rằng $\gamma_M$ là một đẳng cấu. Mặt khác, ta đã biết rằng (ii) suy ra (iii) và do đó $M/\mathfrak{g}M$ là một $(A/\mathfrak{g})$-môđun phẳng, điều này hoàn tất chứng minh rằng (ii) suy ra (iv).

*Nhận xét* (2). Mệnh đề 1 chỉ ra rằng, nếu $\mathfrak{g}$ là lũy linh, (iv) suy ra (iii); xét đến *Nhận xét* 1, vì vậy ta đã chứng minh trong trường hợp này rằng (i), (ii), (iii) và (iv) là tương đương.

(D) *Sự tương đương* (iv) $\Leftrightarrow$ (v)

Với mọi $n \geq 1$, $M/\mathfrak{g}^n M$ có một cấu trúc môđun $(A/\mathfrak{g}^n)$ chính tắc. Nếu nó được lọc bởi phép lọc $(\mathfrak{g}/\mathfrak{g}^n)$-adic, thì hiển nhiên rằng $\mathrm{gr}_m(M/\mathfrak{g}^n M) = \mathrm{gr}_m(M)$ nếu $m < n$ và $\mathrm{gr}_m(M/\mathfrak{g}^n M) = 0$ nếu $m \geq n$. Với mọi $k \geq 1$, đặt $A_k = A/\mathfrak{g}^k$, $\mathfrak{g}_k = \mathfrak{g}/\mathfrak{g}^k$, $M_k = M/\mathfrak{g}^k M$; gọi (iv), (tương ứng $(v)_k$) là mệnh đề dẫn xuất từ (iv) (tương ứng (v)) bằng cách thay $A, \mathfrak{g}, M$ bởi $A_k, \mathfrak{g}_k, M_k$. Từ điều vừa nói suy ra rằng (iv) tương đương với "với mọi $k \geq 1$, $(iv)_k$" và hiển nhiên (v) tương đương với "với mọi $k \geq 1$, $(v)_k$". Khi đó chỉ cần thiết lập sự tương đương $(iv)_k \Leftrightarrow (v)_k$ với mọi $k$, hoặc cũng chỉ cần chứng minh rằng (iv) $\Leftrightarrow$ (v) khi $3$ là *lũy linh*. Bây giờ (*Nhận xét* 2) ta đã thấy rằng trong trường hợp đó (iv) tương đương với (i). Vì $M/\mathfrak{g}^n M$ đẳng cấu với $M \otimes_A (A/\mathfrak{g}^n)$, (i) suy ra (v) (Chương I, § 2, no. 7, Hệ quả 2 của Mệnh đề 8); hơn nữa hiển nhiên (v) khi đó suy ra (i). Do đó ta đã chứng minh sự tương đương (iv) $\Leftrightarrow$ (v) trong mọi trường hợp và cũng chứng minh sự tương đương của tất cả các tính chất của định lý trong trường hợp $3$ là lũy linh.

(E) *Sự kéo theo* (v) $\Rightarrow$ (i) *khi* $A$ *là Noether và* $M$ *là Hausdorff theo iđêan*

Chỉ cần chứng minh rằng với mọi iđêan $a$ của $A$, ánh xạ chính tắc $j : a \otimes_A M \to M$ là *đơn ánh* (Chương I, § 2, no. 3, Mệnh đề 1). Cho $x \in \mathrm{Ker}\, j$;
$a \otimes_A M$ là Hausdorff với tôpô $\mathfrak{g}$-adic, chỉ cần kiểm tra rằng, với mọi số nguyên $n > 0$, $x \in \mathfrak{g}^n(a \otimes_A M)$. Gọi $f : \mathfrak{g}^n a \to a$ là đơn ánh chính tắc; chỉ cần chứng minh rằng $x \in \mathrm{Im}(f \otimes 1_M)$; vì nếu $b \in \mathfrak{g}^n$, $a \in a$ và $m \in M$, ảnh qua $f \otimes 1$, của phần tử $(ba) \otimes m$ của $(\mathfrak{g}^n a) \otimes_A M$ là phần tử $(ba) \otimes m = b(a \otimes m)$ của $a \otimes_A M$ và do đó $\mathrm{Im}(f \otimes 1_M) \subset \mathfrak{g}^n(a \otimes_A M)$. Theo Định lý Krull (§ 3, no. 2, Định lý 2), tồn tại một số nguyên $k$ sao cho $a_j = a \cap \mathfrak{g}^k \subset \mathfrak{g}^n a$; nếu $i : a_j \to a$ là đơn ánh chính tắc, thì khi đó chỉ cần chứng minh rằng $x \in \operatorname{Im}(i \otimes 1_M)$. Bây giờ, ký hiệu $p : a \to a/a_k$ và $h : a/a_k \to A/\mathfrak{g}^k$ là các ánh xạ chính tắc, ta có một biểu đồ giao hoán

$$
\begin{array}{ccccccccc}
a_k \otimes_A M & \xrightarrow{i \otimes 1_M} & a \otimes_A M & \xrightarrow{p \otimes 1_M} & (a/a_k) \otimes_A M & \longrightarrow & 0 \\
& & \downarrow & & \downarrow h \otimes 1_M & & \\
& & M & \longrightarrow & (A/\mathfrak{g}^k) \otimes_A M & &
\end{array}
$$

trong đó hàng thứ nhất là khớp. Chỉ cần chứng minh rằng $x \in \operatorname{Ker}(p \otimes 1_M)$ và, vì $x \in \operatorname{Ker} j$ theo giả thiết, chỉ cần kiểm tra rằng ánh xạ $h \otimes 1_1$, là đơn ánh. Bây giờ, nó cũng có thể được viết (Đại số, Chương II, § 3, no. 6, Hệ quả 3 của Mệnh đề 6)

$$
h \otimes 1_{M/\mathfrak{g}^k M} : (a/a_k) \otimes_{A/\mathfrak{g}^k} (M/\mathfrak{g}^k M) \to M/\mathfrak{g}^k M
$$

và, vì $h$ là đơn ánh và, theo (v), $M/\mathfrak{g}^k M$ là một $(A/\mathfrak{g}^k)$-môđun phẳng, điều này hoàn tất chứng minh.

### 4. CÁC ỨNG DỤNG

#### Mệnh đề 2 {#ac-iii-s5-prop-2 .statement}

Cho $A$ là một vành giao hoán, $\mathfrak{g}$ là một iđêan của $A$ và $B$ là một đại số $A$-giao hoán Noether sao cho $B$ được chứa trong căn Jacobson của $B$. Khi đó mọi $B$-môđun $M$ sinh hữu hạn đều là một $A$-môđun Hausdorff theo iđêan đối với $\mathfrak{g}$.

Nói tổng quát hơn, ta sẽ thấy rằng với mọi $A$-môđun $N$ sinh hữu hạn, $N \otimes_A M$ là Hausdorff với tôpô $3$-adic. Thật vậy, $N_{(B)} = N \otimes_A B$ là một $B$-môđun sinh hữu hạn và $B$-môđun $N \otimes_A M$ được đồng nhất một cách chính tắc với $N_{,,} \otimes_B M$ nhờ tính kết hợp của tích tenxơ. Gọi $\mathfrak{L}$ là căn Jacobson của $B$; vì $\mathfrak{g} B$ được chứa trong $\mathfrak{L}$, tôpô $\mathfrak{g}$-adic trên $N \otimes_A M$ do đó được đồng nhất với một tôpô mịn hơn tôpô $\mathfrak{L}$-adic trên $N_{(B)} \otimes_B M$; nhưng tôpô sau này là Hausdorff vì $N_{,,} \otimes_B M$ là một $B$-môđun sinh hữu hạn (no. 1, Ví dụ 1), do đó có kết luận.

#### Mệnh đề 3 {#ac-iii-s5-prop-3 .statement}

Cho $A$ là một vành giao hoán, $B$ là một đại số $A$-giao hoán, $\mathfrak{g}$ là một iđêan của $A$ và $M$ là một $B$-môđun. Giả sử rằng $B$ là một vành Noether và là một $A$-môđun phẳng và rằng $M$ là Hausdorff theo iđêan đối với $\mathfrak{g} B$. Các điều kiện sau là tương đương:
(a) $M$ là một $B$-môđun phẳng.
(b) $M$ là một $A$-môđun phẳng và $M/\mathfrak{g} M = M/(\mathfrak{g} B) M$ là một $(B/\mathfrak{g} B)$-môđun phẳng.
Nếu hơn nữa đồng cấu chính tắc $A/\mathfrak{g} \to B/\mathfrak{g} B$ là song ánh, các điều kiện (a) và (b) cũng tương đương với:
(c) $M$ là một $A$-môđun phẳng.

Điều kiện (a) suy ra (b) theo Chương I, §2, no. 7, các Hệ quả 2 và 3 đối với Mệnh đề 8 và sự kiện rằng $M/\mathfrak{g} M$ đẳng cấu với $M \otimes_B (B/\mathfrak{g} B)$. Giả sử điều kiện (b) đúng; để chứng minh rằng $M$ là một $B$-môđun phẳng, ta sẽ áp dụng Định lý 1 của no. 2 với $A$ được thay bởi $B$ và $\mathfrak{g}$ bởi $\mathfrak{g} B$. Do đó chỉ cần chứng minh rằng ánh xạ chính tắc $f : \mathfrak{J}B \otimes_B M \to \mathfrak{J}M$ là đơn ánh. Gọi $f_1$ là ánh xạ chính tắc $\mathfrak{J} \otimes_A B \to \mathfrak{J}B$ và $f_2$ là đẳng cấu chính tắc $\mathfrak{J} \otimes_A M \to (\mathfrak{J} \otimes_A B) \otimes_B M ; f \circ (f_1 \circ 1_M) \circ f_2$ là ánh xạ chính tắc $f' : \mathfrak{J} \otimes_A M \to \mathfrak{J}M$, như dễ dàng kiểm tra. Bây giờ $f'$ là một đẳng cấu vì $M$ là một $A$-môđun phẳng, trong khi đó $f_1$ là một đẳng cấu vì $B$ là phẳng trên $A$; khi đó $f$ là một đẳng cấu.

Cho $p : A/\mathfrak{J} \to B/\mathfrak{J}B$ là đồng cấu chính tắc; cấu trúc môđun $(A/\mathfrak{J})$ trên $M/\mathfrak{J}M$ dẫn xuất nhờ $p$ từ cấu trúc môđun $(B/\mathfrak{J}B)$ của nó là đẳng cấu với cấu trúc trên $M \otimes_A (A/\mathfrak{J})$. Khi đó suy ra rằng, nếu $M$ là một $A$-môđun phẳng, thì $M/\mathfrak{J}M$ là một $(A/\mathfrak{J})$-môđun phẳng và do đó cũng là một $(B/\mathfrak{J}B)$-môđun phẳng nếu $p$ là một đẳng cấu; như vậy ta đã chứng minh rằng (c) $\Rightarrow$ (b) trong trường hợp đó.

#### Hệ quả {#ac-iii-s5-n4-cor-1 .statement}

*Cho $A$ là một vành Noether giao hoán, $\mathfrak{J}$ là một iđêan của $A$, $\hat{A}$ là hoàn thành Hausdorff của $A$ đối với tôpô $\mathfrak{J}$-adic và $M$ là một $\hat{A}$-môđun Hausdorff lý tưởng đối với $\mathfrak{J} \hat{A}$. Để $M$ là một $A$-môđun phẳng, điều kiện cần và đủ là $M$ là một $\hat{A}$-môđun phẳng.*

Thực tế ta biết rằng $\hat{A}$ là một vành Noether ($§ 3$, no. **4**, Mệnh đề 8) và một $A$-môđun phẳng ($§ 3$, no. **4**, Định lý 3), rằng $\mathfrak{J} \hat{A} = \hat{\mathfrak{J}}$ ($§ 2$, no. 12, Mệnh đề **16**) và rằng đồng cấu chính tắc $A/\mathfrak{J} \to \hat{A}/\hat{\mathfrak{J}}$ là song ánh ($§ 2$, no. 12, Mệnh đề 15); do đó có thể áp dụng Mệnh đề **3**.

#### Mệnh đề 4 {#ac-iii-s5-prop-4 .statement}

*Cho $A$ và $B$ là hai vành giao hoán Noether, $h : A \to B$ là một đồng cấu vành, $3$ là một iđêan của $A$ và $2$ là một iđêan của $B$ chứa $\mathfrak{J}B$ và được chứa trong căn Jacobson của $B$. Gọi $\hat{A}$ là phép hoàn thành Hausdorff của $A$ đối với tôpô $3$-adic và $\hat{B}$ là phép hoàn thành Hausdorff của $B$ đối với tôpô $2$-adic; $h$ liên tục đối với các tôpô này và $h : \hat{A} \to \hat{B}$ do đó làm cho $\mathbf{8}$ trở thành một $\hat{A}$-đại số. Cho $M$ là một $B$-môđun sinh hữu hạn và $\hat{M}$ là phép hoàn thành Hausdorff của nó đối với tôpô $2$-adic; các tính chất sau là tương đương:
(a) $M$ là một $A$-môđun phẳng.
(b) $\hat{M}$ là một $A$-môđun phẳng.
(c) $\hat{M}$ là một $\hat{A}$-môđun phẳng.*

Vì $B$ với tôpô $2$-adic là một vành Zariski, $\hat{B}$ là một $B$-môđun phẳng trung thành ($§ 3$, no. 5, Mệnh đề 9) và $M$ đẳng cấu chính tắc với $M \otimes_B \hat{B}$ ($§ 3$, no. **4**, Định lý 3); người ta kiểm tra ngay lập tức rằng đẳng cấu chính tắc này là một đẳng cấu từ cấu trúc môđun $A$ trên $\hat{M}$ lên cấu trúc môđun $A$ trên $M \otimes_B \hat{B}$ dẫn xuất từ cấu trúc trên $M$. Áp dụng Mệnh đề 4 của Chương I, $§ 3$, no. 2 với $R$ được thay bởi $B$, $S$ bởi $A$, $E$ bởi $\hat{B}$, $F$ bởi $M$, ta thấy rằng để $M$ là một $A$-môđun phẳng, điều kiện cần và đủ là $\hat{M}$ là một $A$-môđun phẳng. Hơn nữa, $\hat{M}$ là một $\hat{B}$-môđun sinh hữu hạn và $\mathfrak{J} \hat{B}$ được chứa trong $\mathfrak{Q} = \mathfrak{Q} \hat{B}$ và do đó trong căn Jacobson của $\hat{B}$ ($§ 3$, no. **4**, Mệnh đề 8); vì vậy $\hat{M}$ là một $A$-môđun Hausdorff lý tưởng đối với $\mathfrak{J} \hat{A}$ (Mệnh đề 2). Các điều kiện (b) và (c) do đó tương đương theo Hệ quả của Mệnh đề 3.

### Bài tập {#ac-iii-s5-exercises}

Xem [các bài tập cho § 5](exercises/s5/).
