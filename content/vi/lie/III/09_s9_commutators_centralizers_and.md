---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: III
chapter_title: LIE GROUPS
section: 9
section_title: Commutators, centralizers and normalizers in a Lie group
lang: vi
source: lie-i-iii
pdf_pages: 0360-0377, 0415-0427
extraction: ocr
subsections:
    - "no": 1
      title: COMMUTATORS IN A TOPOLOGICAL GROUP
      page: 0
      pdf_page: 360
    - "no": 2
      title: COMMUTATORS IN A LIE GROUP
      page: 0
      pdf_page: 361
    - "no": 3
      title: CENTRALIZERS
      page: 0
      pdf_page: 364
    - "no": 4
      title: NORMALIZERS
      page: 0
      pdf_page: 365
    - "no": 5
      title: NILPOTENT LIE GROUPS
      page: 0
      pdf_page: 365
    - "no": 6
      title: SOLVABLE LIE GROUPS
      page: 0
      pdf_page: 370
    - "no": 7
      title: RADICAL OF A LIE GROUP
      page: 0
      pdf_page: 372
    - "no": 8
      title: SEMI-SIMPLE LIE GROUPS
      page: 0
      pdf_page: 373
statements: 54
exercises: 29
content_sha256: f351442ebb73dd761070ddf1e9419995c758f1fd188ac6fef106d1d925148a98
translated_from: content/en/lie/III/09_s9_commutators_centralizers_and.md
source_content_sha256: 28599142f274ec5813551cdbb3bbe444ef139fc7c26b1c613596b1ce9597e9d3
translation_model: gpt-5-6-mini, gpt-5-6, gpt-5-mini
translation_run: translate-vi-36e3818b
glossary_version: 34
glossary_terms_sha256: c49d4c8047ade017f5126239322f69af9d9d0b8bb97a2636b4813718dfbbd1cd
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 9. Các phần tử giao hoán, các tâm hóa và các chuẩn hóa trong một nhóm Lie

Trong đoạn này, K được giả thiết là có đặc số không.

### 1. Các phần tử giao hoán trong một nhóm tôpô

Cho G là một nhóm tôpô. Ta định nghĩa các nhóm $\overline{D^0G}, \overline{D^1G}, \overline{D^2G}, \ldots$ và $\overline{C^1G}, \overline{C^2G}, \overline{C^3G}, \ldots$ bởi các công thức

$$
\begin{aligned}
\overline{D^0G} &= G, & \overline{D^{i+1}G} &= (\overline{D^iG}, \overline{D^iG}) \\
\overline{C^1G} &= G, & \overline{C^{i+1}G} &= (G, \overline{C^iG}).
\end{aligned}
$$

#### Mệnh đề 1 {#lie-iii-s9-prop-1 .statement}

*Cho G là một nhóm tôpô và A và B là các nhóm con của G. Khi đó* $(\overline{A}, \overline{B}) = (\overline{A}, \overline{B}), \overline{D^iA} = \overline{D^iA}, \overline{C^iA} = \overline{C^iA}$.

Cho $\phi$ là ánh xạ liên tục $(x, y) \mapsto x^{-1}y^{-1}xy$ của $G \times G$ vào G. Khi đó $\phi(A \times B) \subset (A, B)$, do đó $\phi(\overline{A} \times \overline{B}) \subset (\overline{A}, \overline{B})$ và do đó

$$
(\overline{A}, \overline{B}) \subset (\overline{A}, \overline{B});
$$

bao hàm ngược lại là hiển nhiên và vì vậy $(\overline{A}, \overline{B}) = (\overline{A}, \overline{B})$. Rõ ràng $\overline{D^0A} = \overline{D^0A}$; giả sử đẳng thức $\overline{D^iA} = \overline{D^iA}$, ta suy ra

$$
\overline{D^{i+1}A} = (\overline{D^iA}, \overline{D^iA}) = (\overline{D^iA}, \overline{D^iA}) = (\overline{D^iA}, \overline{D^iA}) = \overline{D^{i+1}A}
$$

và do đó $\overline{D^iA} = \overline{D^iA}$ với mọi $i$. Chứng minh của công thức $\overline{C^iA} = \overline{C^iA}$ là tương tự.

#### Hệ quả 1 {#lie-iii-s9-prop-1-cor-1 .statement}

*Nếu G là Hausdorff, các điều kiện sau là tương đương*:
(i) *G là giải được* (tương ứng *lũy linh*);
(ii) $\overline{D^iG} = \{e\}$ (tương ứng $\overline{C^iG} = \{e\}$) *với* $i$ *đủ lớn*.
$D^iG \subset \overline{D^iG}, C^iG \subset \overline{C^iG}$ và do đó (ii) $\Rightarrow$ (i). $\{e\} = \{\overline{e}\}$ và do đó (i) $\Rightarrow$ (ii) theo Mệnh đề 1.

#### Hệ quả 2 {#lie-iii-s9-prop-1-cor-2 .statement}

*Cho G là một nhóm tôpô Hausdorff và A là một nhóm con của G. Để A là giải được* (tương ứng *lũy linh, giao hoán*, *điều kiện cần và đủ là* $\overline{A}$ *cũng như vậy*).

§ 9.2

Điều này suy ra ngay lập tức từ Mệnh đề 1.

#### Mệnh đề 2 {#lie-iii-s9-prop-2 .statement}

Cho G là một nhóm tôpô và A và B là các nhóm con của G. Nếu A liên thông, (A, B) liên thông.

Với y cố định trong B, tập M_y gồm các (x, y) với x ∈ A là liên thông (vì ánh xạ x ↦ (x, y) của A vào G là liên tục). e ∈ M_y, và do đó hợp R của các M_y với y ∈ B là liên thông. Nhưng (A, B) là nhóm con của G sinh bởi R, do đó suy ra mệnh đề.

### 2. Các phần tử giao hoán trong một nhóm Lie

#### Mệnh đề 3 {#lie-iii-s9-prop-3 .statement}

Cho G là một nhóm Lie hữu hạn chiều và H_1 và H_2 là các nhóm con của G. Cho h_1, h_2 và h là các đại số con Lie tiếp xúc tại e với H_1 H_2 và (H_1, H_2) tương ứng. Khi đó [h_1, h_2] ⊂ h.

Cho a ∈ h_1, b ∈ h_2. Tồn tại một lân cận mở I của 0 trong K và các ánh xạ giải tích f_1, f_2 của I vào G sao cho

$$
f_1(0) = f_2(0) = e, \quad f_1(I) \subset H_1, \quad f_2(I) \subset H_2,
$$
$$
(T_0 f_1)1 = a, \quad (T_0 f_2)1 = b.
$$

Ta viết
$$
f(\lambda, \mu) = (f_1(\lambda), f_2(\mu)) \in (H_1, H_2) \quad \text{với } \lambda, \mu \text{ trong I}.
$$

Ta đồng nhất một lân cận mở của e trong G với một tập con mở của K' bằng một biểu đồ gửi e tới 0. Khi đó L(G) được đồng nhất với K'. Theo § 5, no. 2, Mệnh đề 1, khai triển của f(\lambda, \mu) thành chuỗi nguyên quanh gốc là
$$
f(\lambda, \mu) = \lambda \mu [a, b] + \sum_{i \geq 1, j \geq 1, i+j \geq 2} \lambda^i \mu^j a_{ij}
$$
trong đó a_{ij} ∈ K' (các số hạng theo \lambda^i và \mu^j trong khai triển của f(\lambda, \mu) bằng không vì f(\lambda, 0) = f(0, \mu) = 0). Ta cố định \mu trong I. Cho \lambda tiến tới 0, ta thấy rằng
$$
\mu [a, b] + \sum_{j \geq 2} \mu^j a_{1j} \in h.
$$
Vì điều này đúng với mọi \mu ∈ I, suy ra [a, b] ∈ h.

#### Nhận xét {#lie-iii-s9-n2-rem-1 .statement}

Ngay cả khi H_1 và H_2 là các nhóm con Lie liên thông của G, đại số con Lie của L(G) sinh bởi [h_1, h_2] nói chung phân biệt với h.

#### Mệnh đề 4 {#lie-iii-s9-prop-4 .statement}

Cho G là một nhóm Lie thực hoặc phức hữu hạn chiều. Cho A, B, C là các nhóm con nguyên của G sao cho [L(A), L(C)] ⊂ L(C) và
$$
[L(B), L(C)] \subset L(C).
$$
Nếu [L(A), L(B)] ⊂ L(C), thì (A, B) ⊂ C. Nếu [L(A), L(B)] = L(C), thì (A, B) = C.

Giả sử rằng $[L(A), L(B)] \subset L(C)$. Tổng $L(A) + L(B) + L(C)$ là một đại số con Lie của $L(G)$. Bằng cách xét một nhóm con nguyên của $G$ có đại số Lie là $L(A) + L(B) + L(C)$, bài toán được quy về trường hợp

$$
L(A) + L(B) + L(C) = L(G)
$$

và $G$ liên thông. Khi đó $L(C)$ là một iđêan của $L(G)$. Trước hết giả sử rằng $G$ đơn liên. Khi đó $C$ là một nhóm con Lie chuẩn của $G$ (\S 6, no. 6, Mệnh đề 14). Cho $\phi$ là cấu xạ chính tắc của $G$ lên $G/C$. Khi đó

$$
[L(\phi)(L(A)), L(\phi)(L(B))] = \{0\}
$$

và do đó $\phi(A)$ và $\phi(B)$ giao hoán theo công thức Hausdorff; do đó $(A, B) \subset C$. Trong trường hợp tổng quát, lấy $G'$ là phủ phổ quát của $G$ và $A', B', C'$ là các nhóm con nguyên của $G'$ sao cho $L(A') = L(A), L(B') = L(B), L(C') = L(C)$. Khi đó $(A', B') \subset C'$ và $A, B, C$ là các ảnh chính tắc của $A', B', C'$ trong $G$, do đó $(A, B) \subset C$. Mặt khác, $(A, B)$ là tập hợp nền của một nhóm con nguyên của $G$ (\S 6, no. 2, Hệ quả của Mệnh đề 4) và đại số Lie của nó chứa $[L(A), L(B)]$ (Mệnh đề 3). Nếu

$$
[L(A), L(B)] = L(C),
$$

thì $(A, B) \supset C$, do đó $(A, B) = C$.

#### Hệ quả {#lie-iii-s9-n2-cor-1 .statement}

*Cho G là một nhóm Lie thực hoặc phức liên thông hữu hạn chiều với đại số Lie g. Các nhóm con $D^iG$ (tương ứng $C^iG$) là các nhóm con nguyên với các đại số Lie $D^i\mathfrak{g}$ (tương ứng $C^i\mathfrak{g}$). Nếu G đơn liên thông, chúng là các nhóm con Lie.*

Mệnh đề thứ nhất suy ra từ Mệnh đề 4 bằng quy nạp theo $i$. Mệnh đề thứ hai suy ra từ mệnh đề thứ nhất và \S 6, no. 6, Mệnh đề 14.

#### Mệnh đề 5 {#lie-iii-s9-prop-5 .statement}

*Cho G là một nhóm Lie thực hoặc phức hữu hạn chiều và A là một nhóm con nguyên của G. Khi đó $DA = DA$. Đặc biệt, A là một nhóm con chuẩn của $\overline{A}$ và $\overline{A}/A$ là giao hoán.*

Lấy $a = L(A)$. Gọi $G_1$ là tập hợp các $g \in G$ sao cho

$$(\mathrm{Ad}\, g)x \equiv x \pmod{\mathcal{D}a} \quad \text{với mọi } x \in a.$$

Khi đó $G_1$ là một nhóm con đóng của $G$. Nếu $y \in a$, thì $\exp y \in G_1$, theo \S 6, no. 4, Hệ quả 3 (ii) của Mệnh đề 10. Do đó $G_1$ chứa $A$ và vì vậy chứa $\overline{A}$. Như vậy, với $g \in \overline{A}$, $L(\mathrm{Int}\, g)$ giữ $a$ ổn định và do đó $\mathrm{Int}\, g$ giữ $A$ ổn định; chính xác hơn, $L(\mathrm{Int}\, g)$ xác định tự đẳng cấu đồng nhất của $a/\mathcal{D}a$ và do đó $\mathrm{Int}\, g$ xác định tự đẳng cấu đồng nhất của $A/DA$. Điều này chứng minh rằng $(\overline{A}, A) \subset DA$. Với cấu trúc nhóm Lie thực trên $G$, $\overline{A}$ là một nhóm con Lie (\S 8, no. 2, Định lý 2); gọi $b$ là đại số Lie của nó. Gọi $G_2$ là tập hợp các $g \in G$ sao cho

$$(\mathrm{Ad}\, g)x \equiv x \pmod{\mathcal{D}a} \quad \text{với mọi } x \in b.$$

Theo trên, $G_2 \supseteq A$ và do đó $G_2 \supseteq \overline{A}$. Vì vậy, với $g \in \overline{A}$, Int $g$ giữ DA ổn định và xác định tự đẳng cấu đồng nhất của $\overline{A}/DA$. Do đó $DA \supseteq D\overline{A}$.

#### Mệnh đề 6 {#lie-iii-s9-prop-6 .statement}

*Giả sử rằng K là ultrametric. Cho G là một nhóm Lie hữu hạn chiều. Cho A, B, C là các nhóm con Lie của G sao cho $[L(A), L(C)] \subset L(C)$, $[L(B), L(C)] \subset L(C)$. Nếu $[L(A), L(B)] \subset L(C)$, tồn tại các nhóm con mở A', B' của A, B sao cho $(A', B') \subset C$. Nếu $[L(A), L(B)] \subset L(C)$, tồn tại các nhóm con mở A', B', C' của A, B, C sao cho $(A', B') = C'$.*

Giả sử rằng $[L(A), L(B)] \subset L(C)$. Như trong chứng minh của Mệnh đề 4, bài toán quy về trường hợp $L(C)$ là một iđêan của $L(G)$. Khi đó, bằng cách thay thế G bởi một nhóm con mở, ta quy về trường hợp C là chuẩn trong G ($\S 7$, no. 1, Mệnh đề 2). Cho $\phi$ là cấu xạ chính tắc của G lên $G/C$. Khi đó
$$
[L(\phi)(L(A)), L(\phi)(L(B))] = \{0\}.
$$
Theo công thức Hausdorff, tồn tại các nhóm con mở A', B' của A, B sao cho $\phi(A')$ và $\phi(B')$ giao hoán, do đó $(A', B') \subset C$. Giả sử thêm rằng
$$
[L(A), L(B)] = L(C).
$$
Theo Mệnh đề 3, đại số con Lie tiếp xúc với $(A', B')$ tại $e$ chứa $L(C)$. Do đó $(A', B')$ chứa một mầm nhóm con Lie của G với đại số Lie $L(C)$. Vì vậy $(A', B')$ là một nhóm con mở của C.

#### Hệ quả {#lie-iii-s9-n2-cor-2 .statement}

*Giả sử rằng K là ultrametric. Cho G là một nhóm Lie hữu hạn chiều với đại số Lie g. Tồn tại một nhóm con mở $G_0$ của G sao cho, với mọi $i$, $D^iG_0$ (tương ứng $C^iG_0$) là một nhóm con Lie của G với đại số Lie $\mathcal{D}^ig$ (tương ứng $\mathcal{C}^ig$).*

(a) Bằng Mệnh đề 3 được áp dụng quy nạp, với mọi nhóm con mở $G_1$ của G và với mọi $i$, $D^iG_1$ chứa một mầm nhóm con Lie của G với đại số Lie $\mathcal{D}^ig$.

(b) Cho $G'$ là một nhóm con mở của G sao cho, với $i \leq n$, $D^iG'$ là một nhóm con Lie của G với đại số Lie $\mathcal{D}^ig$. Theo Mệnh đề 6, tồn tại các nhóm con mở $H_1, H_2$ của $D^nG'$, sao cho $(H_1, H_2)$ là một nhóm con Lie với đại số Lie $\mathcal{D}^{n+1}g$. Cho $G''$ là một nhóm con mở của $G'$ đủ nhỏ để $D^nG'' \subset H_1 \cap H_2$. Khi đó $D^{n+1}G'' \subset (H_1, H_2)$. Các quan hệ
$$
D^0G'' \subset D^0G', D^1G'' \subset D^1G', \ldots, D^nG'' \subset D^nG', D^{n+1}G'' \subset (H_1, H_2)
$$
chứng minh, sử dụng (a), rằng $D^iG''$ là, với $i \leq n + 1$, một nhóm con Lie của G với đại số Lie $\mathcal{D}^ig$.

(c) Tồn tại một số nguyên $p$ sao cho $\mathcal{D}^pg = \mathcal{D}^{p+1}g = \cdots$. Theo điều trên, tồn tại một nhóm con mở $G_0$ của G sao cho $D^iG_0$ là, với $i \leq p$, một nhóm con Lie của G với đại số Lie $\mathcal{D}^ig$. Nhưng, theo (a), cùng mệnh đề vẫn đúng với $i > p$ vì $D^pG_0 \supset D^iG_0$ với $i > p$.

(d) Lập luận tương tự đối với $C^i$.

### 3. CÁC TÂM HÓA

Nhắc lại rằng hai phần tử $x, y$ của một nhóm được gọi là giao hoán được nếu $(x, y) = e$, hoặc $(\mathrm{Int}\, x)y = y$, hoặc $(\mathrm{Int}\, y)x = x$; và rằng hai phần tử $a, b$ của một đại số Lie được gọi là giao hoán được nếu $[a, b] = 0$, hoặc $(\mathrm{ad}\, a).b = 0$, hoặc $(\mathrm{ad}\, b).a = 0$. Cho $G$ là một nhóm Lie, $x \in G$, $a \in \mathbf{L}(G)$; $x$ và $a$ được gọi là giao hoán được nếu $(\mathrm{Ad}\, x).a = a$, tức là nếu $xa = ax$ trong $\mathbf{T}(G)$.

Cho $G$ là một nhóm Lie, $g$ là đại số Lie của nó, $A$ là một tập con của $G$ và $a$ là một tập con của $g$. Ký hiệu $Z_G(A)$ (tương ứng $Z_G(a)$) là tập hợp các phần tử của $G$ giao hoán được với mọi phần tử của $A$ (tương ứng $a$). Đây là một nhóm con đóng của $G$. Ký hiệu $\mathfrak{z}_g(A)$ (tương ứng $\mathfrak{z}_g(a)$) là tập hợp các phần tử của $g$ giao hoán được với mọi phần tử của $A$ (tương ứng $a$). Đây là một đại số con Lie đóng của $g$.

#### Mệnh đề 7 {#lie-iii-s9-prop-7 .statement}

*Cho $G$ là một nhóm Lie hữu hạn chiều, $g$ là đại số Lie của nó và $a$ là một tập con của $g$. Khi đó $Z_G(a)$ là một nhóm con Lie của $G$ với đại số Lie $\mathfrak{z}_g(a)$.*

Điều này suy ra từ § 3, Mệnh đề 44 và Hệ quả 2 của Mệnh đề 39.

#### Mệnh đề 8 {#lie-iii-s9-prop-8 .statement}

*Cho $G$ là một nhóm Lie thực hoặc phức hữu hạn chiều, $g$ là đại số Lie của nó và $A$ là một tập con của $G$. Khi đó $Z_G(A)$ là một nhóm con Lie của $G$ với đại số Lie $\mathfrak{z}_g(A)$.*

Giả sử rằng $A$ chỉ gồm một điểm duy nhất $a$. Khi đó $Z_G(A)$ là tập hợp các điểm bất động của $\mathrm{Int}\, a$; do đó $Z_G(A)$ là một nhóm con Lie của $G$ và $\mathbf{L}(Z_G(A))$ là tập hợp các điểm bất động của $\mathrm{Ad}\, a$, tức là $\mathfrak{z}_g(A)$ (§ 3, no. 8, Hệ quả 1 của Mệnh đề 29). Trường hợp tổng quát suy ra bằng cách dùng § 6, no. 2, Hệ quả 3 của Mệnh đề 1.

#### Mệnh đề 9 {#lie-iii-s9-prop-9 .statement}

*Cho $G$ là một nhóm Lie thực hoặc phức hữu hạn chiều, $g$ là đại số Lie của nó, $A$ là một nhóm con nguyên của $G$ và $a = \mathbf{L}(A)$. Khi đó $Z_G(A) = Z_G(a)$, $\mathfrak{z}_g(A) = \mathfrak{z}_g(a)$ và $Z_G(A)$ là một nhóm con Lie của $G$ với đại số Lie $\mathfrak{z}_g(a)$.*

Cho $x \in G$. Khi đó
$$
x \in Z_G(A) \iff A \subset Z_G(\{x\}) \\
\iff a \subset \mathbf{L}(Z_G(\{x\})) \quad (\text{§ 6, Hệ quả 2 của Mệnh đề 3}) \\
\iff a \subset \mathfrak{z}_g(\{x\}) \quad (\text{Mệnh đề 8}) \\
\iff x \in Z_G(a)
$$
và do đó $Z_G(A) = Z_G(a)$. Cho $u \in g$. Khi đó
$$
u \in \mathfrak{z}_g(A) \iff A \subset Z_G(\{u\}) \\
\iff a \subset \mathbf{L}(Z_G(\{u\})) \quad (\text{§ 6, Hệ quả 2 của Mệnh đề 3}) \\
\iff a \subset \mathfrak{z}_g(\{u\}) \quad (\text{Mệnh đề 7}) \\
\iff u \in \mathfrak{z}_g(a)
$$
và do đó $\mathfrak{z}_g(A) = \mathfrak{z}_g(a)$. Khẳng định cuối cùng suy ra từ Mệnh đề 7 hoặc Mệnh đề 8.

### 4. CÁC CHUẨN HÓA TỬ

Cho G là một nhóm Lie, $g$ là đại số Lie của nó, A là một tập con của G và $a$ là một tập con của $g$. Trong tiết này, $N_G(A)$ sẽ chỉ tập hợp các $g \in G$ sao cho $gAg^{-1} = A$. Nó là một nhóm con của G, đóng nếu A đóng. $n_g(a)$ sẽ chỉ tập hợp các $x \in g$ sao cho $[x, a] \subset a$ (xem Chương I, § 1, no. 4). Nó là một đại số con của $g$, đóng nếu $a$ đóng. $N_g(a)$ sẽ chỉ tập hợp các $g \in G$ sao cho $gag^{-1} = a$.

#### Mệnh đề 10 {#lie-iii-s9-prop-10 .statement}

*Cho G là một nhóm Lie hữu hạn chiều, g là đại số Lie của nó và a là một không gian con vectơ của g. Khi đó $N_G(a)$ là một nhóm con Lie của G với đại số Lie $n_g(a)$.* Điều này suy ra từ § 3, Mệnh đề 44 và Hệ quả 1 của Mệnh đề 39.

#### Mệnh đề 11 {#lie-iii-s9-prop-11 .statement}

*Cho G là một nhóm Lie thực hoặc phức hữu hạn chiều, g là đại số Lie của nó, A là một nhóm con nguyên của G và $a = L(A)$. Khi đó $N_G(A) = N_G(a)$ và $N_G(A)$ là một nhóm con Lie của G chứa $\overline{A}$, với đại số Lie $n_g(a)$.* Đẳng thức $N_G(A) = N_G(a)$ suy ra từ § 6, no. 2, Hệ quả 2 của Mệnh đề 3. Theo Mệnh đề 10, $N_G(A)$ khi đó là một nhóm con Lie của G với đại số Lie $n_g(a)$. Do đó $N_G(A)$ là đóng. Vì $N_G(A) \supset A$, $N_G(A) \supset \overline{A}$.

#### Hệ quả {#lie-iii-s9-n4-cor-1 .statement}

*Nếu $a = n_g(a)$, A là một nhóm con Lie của G và là thành phần đơn vị của $N_G(A)$.* Thành phần đơn vị này là một nhóm con Lie với đại số Lie $n_g(a)$ (Mệnh đề 11) và do đó bằng A theo § 6, no. 2, Định lý 2 (i).

### 5. CÁC NHÓM LIE LŨY LINH

#### Mệnh đề 12 {#lie-iii-s9-prop-12 .statement}

*Cho G là một nhóm Lie hữu hạn chiều. Để $L(G)$ lũy linh, điều kiện cần và đủ là G có một nhóm con mở lũy linh.* Giả sử rằng G có một nhóm con mở lũy linh $G_0$. Theo các Hệ quả của các Mệnh đề 4 và 6, no. 2, $C^iL(G_0) = \{0\}$ với $i$ đủ lớn. Do đó $L(G_0) = L(G)$ là lũy linh.

Giả sử $L(G)$ là lũy linh. Nếu $K = \mathbf{R}$ hoặc $\mathbf{C}$, thành phần đồng nhất $G_0$ của G là lũy linh theo Hệ quả của Mệnh đề 4, no. 2, và $G_0$ là mở trong G. Nếu K là ultrametric, Hệ quả của Mệnh đề 6, no. 2, chứng minh rằng tồn tại một nhóm con mở $G_1$ của G, một số nguyên $i > 0$ và một lân cận V của e trong G sao cho $C^iG_1 \cap V = \{e\}$. Khi đó, nếu $G_0$ là một nhóm con đủ nhỏ của $G_1$, $C^iG_0 \subset V$, do đó $C^iG_0 = \{e\}$ và $G_0$ là lũy linh.

Cho $g$ là một đại số Lie lũy linh. Chuỗi Hausdorff $H(X, Y)$ tương ứng với $g$ chỉ có một số hữu hạn các số hạng khác không và ta biết (Chương II, § 6, no. 5, *Nhận xét 3*) rằng luật hợp thành $(x, y) \mapsto H(x, y)$ xác định một cấu trúc nhóm trên $g$. Giả sử thêm rằng $g$ là đầy đủ và chuẩn hóa được. Rõ ràng luật H là một đa thức liên tục (*Đa tạp khả vi và giải tích*, R, Phụ lục). Do đó $g$, cùng với luật H, là một nhóm Lie G, được gọi là *liên kết với* $g$. Theo § 4, no. 2, Bổ đề 2 và 3, $L(G) = g$. Ánh xạ đồng nhất $\phi$ của $g$ vào $G$ là một ánh xạ mũ của $G$ sao cho $\phi(\lambda x)\phi(\lambda'x) = \phi((\lambda + \lambda')x)$ với mọi $x \in g, \lambda \in K, \lambda' \in K$. Mọi đại số con Lie $\mathfrak{h}$ của $g$ nhận một phần bù tôpô là một nhóm con Lie $H$ của $G$ và $L(H) = \mathfrak{h}$.

#### Mệnh đề 13 {#lie-iii-s9-prop-13 .statement}

*Cho $G$ là một nhóm Lie lũy linh liên thông đơn chiều hữu hạn trên $\mathbf{R}$ hoặc $\mathbf{C}$.*

(i) $\exp_G$ là một đẳng cấu của nhóm Lie liên kết với $L(G)$ lên trên $G$.

(ii) *Mọi nhóm con nguyên của $G$ là một nhóm con Lie liên thông đơn của $G$.*

Cho $g = L(G)$, là lũy linh (Mệnh đề 12). Vì hai nhóm Lie liên thông đơn trên $\mathbf{R}$ hoặc $\mathbf{C}$ có cùng đại số Lie thì đẳng cấu với nhau ($\S 6$, no. 3, Định lý 3 (ii)), nên chỉ cần chứng minh mệnh đề khi $G$ là nhóm liên kết với $g$. Khi đó (i) và (ii) suy ra từ những gì đã nói trước mệnh đề.

#### Mệnh đề 14 {#lie-iii-s9-prop-14 .statement}

*Cho $G$ là một nhóm Lie liên thông chiều hữu hạn trên $\mathbf{R}$ hoặc $\mathbf{C}$.*

(i) *Nếu $G$ là lũy linh, $\exp_G$ là étale và toàn ánh.*

(ii) *Nếu $K = \mathbf{C}$ và $\exp_G$ là étale, thì $G$ là lũy linh.*

Cho $G'$ là không gian phủ phổ quát của $G$. Cho $\phi$ là cấu xạ chính tắc của $G'$ lên $G$. Khi đó $\exp_G = \phi \circ \exp_{G'}$ ($\S 6$, no. 4, Mệnh đề 10) và do đó (i) suy ra từ Mệnh đề 13 (i).

Nếu $K = \mathbf{C}$ và $\exp$ là étale, thì, với mọi $x \in L(G)$, $x$ không có trị riêng thuộc $2i\pi(\mathbf{Z} - \{0\})$ ($\S 6$, no. 4, Hệ quả của Mệnh đề 12). Áp dụng điều này cho $\lambda x$, trong đó $\lambda$ biến thiên qua $\mathbf{C}$, suy ra mọi trị riêng của $\mathrm{ad}\, x$ đều là không và do đó $\mathrm{ad}\, x$ là lũy linh. Vì vậy $L(G)$ là lũy linh (Chương I, $\S 4$, Hệ quả 1 của Định lý 1) và do đó $G$ là lũy linh (Mệnh đề 12).

#### Mệnh đề 15 {#lie-iii-s9-prop-15 .statement}

*Cho $G$ là một nhóm Lie liên thông lũy linh hữu hạn chiều trên $\mathbf{R}$ hoặc $\mathbf{C}$ và $A$ là một nhóm con nguyên của $G$. Khi đó $Z_G(A)$ là nhóm Lie con liên thông của $G$ có đại số Lie $\mathfrak{z}_G(L(A))$.*

Theo Mệnh đề 9 của no. 3, chỉ cần chứng minh rằng $Z_G(A)$ là liên thông. Cho $g \in Z_G(A)$. Tồn tại $x \in L(G)$ sao cho $g = \exp x$ (Mệnh đề 14). Khi đó $\mathrm{Ad}\, g|L(A) = 1$ (no. 3, Mệnh đề 9), do đó $\mathrm{Ad}\, g^n|L(A) = 1$ với mọi $n \in \mathbf{Z}$ và do đó $\exp(\mathrm{ad}\, nx)|L(A) = 1$ với mọi $n \in \mathbf{Z}$. Vì ánh xạ

$$
\lambda \mapsto \exp(\mathrm{ad}\, \lambda x)|L(A)
$$

từ $K$ vào $\mathscr{L}(L(A), L(G))$ là đa thức, $\exp(\mathrm{ad}\, \lambda x)|L(A) = 1$ với mọi $\lambda \in K$, tức là $\exp(\lambda x) \in Z_G(A)$ với mọi $\lambda \in K$.

#### Mệnh đề 16 {#lie-iii-s9-prop-16 .statement}

*Cho $G$ là một nhóm Lie lũy linh hữu hạn chiều trên $\mathbf{R}$ hoặc $\mathbf{C}$ và $A$ là một nhóm con nguyên của $G$ khác với $G$. Khi đó $N_G(A)$ là một nhóm Lie con liên thông của $G$ khác với $A$.*

$N_G(A) \neq A$ (Đại số, Chương I, § 6, Hệ quả 1 của Mệnh đề 8). Theo Mệnh đề 11 của no. 4, ta chỉ cần chứng minh rằng $N_G(A)$ là liên thông. Cho $g \in N_G(A)$. Tồn tại $x \in L(G)$ sao cho $g = \exp x$ (Mệnh đề 14). Gọi $E$ là không gian con vectơ của $\mathcal{L}(L(G))$ gồm các $u \in \mathcal{L}(L(G))$ sao cho $u(L(A)) \subset L(A)$. Khi đó $\mathrm{Ad}\, g^n \in E$ và do đó $\exp(\mathrm{ad}\, nx) \in E$ với mọi $n \in \mathbf{Z}$. Suy ra $\exp(\mathrm{ad}\, \lambda x) \in E$ với mọi $\lambda \in K$, tức là $\exp(\lambda x) \in N_G(A)$ với mọi $\lambda \in K$.

#### Mệnh đề 17 {#lie-iii-s9-prop-17 .statement}

*Cho $g$ là một đại số Lie lũy linh hữu hạn chiều trên $K$ và $(g_0, g_1, \ldots, g_n)$ là một dãy giảm các iđêan của $g$ sao cho $g_0 = g, g_n = \{0\}$ và $[g, g_i] \subset g_{i+1}$ với $0 \leq i < n$. Cho $a_1, a_2, \ldots, a_p$ là các không gian con vectơ của $g$ sao cho mỗi $g_i$ là tổng trực tiếp của các giao của nó với các $a_j$. Cho $g$ được trang bị luật hợp thành Hausdorff $H$. Gọi $\phi$ là ánh xạ*

$$
(x_1, x_2, \ldots, x_p) \mapsto x_1 \mathbf{H} x_2 \mathbf{H} \cdots \mathbf{H} x_p
$$

của $a_1 \times a_2 \times \cdots \times a_p$ vào $g$.

(i) $\phi$ là một song ánh của $a_1 \times a_2 \times \cdots \times a_p$ lên $g$;
(ii) $\phi$ và $\phi^{-1}$ là các ánh xạ đa thức;
(iii) ánh xạ $(x, y) \mapsto \phi^{-1}(\phi(x) \cdot \phi(y)^{-1})$ của $(a_1 \times a_2 \times \cdots \times a_p)^2$ vào $a_1 \times a_2 \times \cdots \times a_p$ là đa thức.

Mệnh đề hiển nhiên đối với $\dim g = 0$. Giả sử rằng $\dim g > 0$ và mệnh đề đã được thiết lập cho các chiều $< \dim g$. Có thể giả sử rằng $g_{n-1} \neq \{0\}$ và khi đó $g_{n-1}$ là một iđêan trung tâm khác không của $g$. Tồn tại một chỉ số $j$ sao cho $h = g_{n-1} \cap a_j \neq \{0\}$. Gọi $g' = g/h$, $\theta$ là cấu xạ chính tắc của $g$ lên $g'$, $g'_i = \theta(g_i)$ và $a'_i = \theta(a_i)$. Khi đó $(g'_0, g'_1, \ldots, g'_n)$ là một dãy giảm các iđêan của $g'$ sao cho $g'_0 = g', g'_n = \{0\}$,

$$
[g', g'_i] \subset g'_{i+1}
$$

với $0 \leq i < n$ và mỗi $g'_i$ là tổng trực tiếp của các giao với các $a'_j$. Gọi $\phi'$ là ánh xạ

$$
(x'_1, x'_2, \ldots, x'_p) \mapsto x'_1 \mathbf{H} x'_2 \mathbf{H} \cdots \mathbf{H} x'_p
$$

của $a'_1 \times a'_2 \times \cdots \times a'_p$ vào $g'$. Theo giả thiết quy nạp, $\phi'$ là song ánh và $\phi', {\phi'}^{-1}$ là các ánh xạ đa thức.

Cho $x \in g$. Ta viết

(1)
$$
{\phi'}^{-1}(\theta(x)) = (x'_1(x), x'_2(x), \ldots, x'_p(x)).
$$
Khi đó
(2)
$$
\theta(x) = x'_1(x) \mathbf{H} x'_2(x) \mathbf{H} \cdots \mathbf{H} x'_p(x).
$$
Gọi $h_1$ là một không gian vectơ con phần bù của $h$ trong $g$, là tổng của các $a_k$ với $k \neq j$ và một phần bù của $h$ trong $a_j$. Tồn tại một song ánh $\eta$ của $g'$ lên $h_1$ sao cho $\theta \circ \eta = \mathrm{Id}_{g'}$. Với $x \in g$, ta viết
(3)
$$
\zeta(x) = \eta(x'_1(x)) \mathbf{H} \eta(x'_2(x)) \mathbf{H} \cdots \mathbf{H} \eta(x'_p(x)) \in g.
$$
(4)
$$
y(x) = \zeta(x)^{-1} \mathbf{H} x = (-\zeta(x)) \cdot x.
$$

Theo (2) và (3), $\theta(\zeta(x)) = \theta(x)$ và do đó $y(x) \in \mathfrak{h}$. Cuối cùng ta viết
$$
(5) \quad \psi(x) = (\eta(x_1'(x)), \ldots, \eta(x_p'(x)) + y(x), \ldots, \eta(x_p'(x))) \in a_1 \times \cdots \times a_p.
$$
Vì $y(x)$ là trung tâm trong $\mathfrak{g}$,
$$
\begin{align*}
\phi(\psi(x)) &= \eta(x_1'(x)) \mathbin{\mathbf{H}} \cdots \mathbin{\mathbf{H}} \eta(x_p'(x)) \mathbin{\mathbf{H}} \cdots \mathbin{\mathbf{H}} \eta(x_p'(x)) \mathbin{\mathbf{H}} y(x) \\
&= \zeta(x) \mathbin{\mathbf{H}} y(x) & \text{theo (3)} \\
&= x & \text{theo (4).}
\end{align*}
$$
Do đó $\phi \circ \psi = \mathrm{Id}_g$. Bây giờ cho $(x_1, x_2, \ldots, x_p) \in a_1 \times a_2 \times \cdots \times a_p$ và viết $x = \phi(x_1, x_2, \ldots, x_p) = x_1 \mathbin{\mathbf{H}} x_2 \mathbin{\mathbf{H}} \cdots \mathbin{\mathbf{H}} x_p$. Khi đó
$$
\theta(x) = \theta(x_1) \mathbin{\mathbf{H}} \theta(x_2) \mathbin{\mathbf{H}} \cdots \mathbin{\mathbf{H}} \theta(x_p),
$$
suy ra $x_i'(x) = \theta(x_i)$ với $1 \leq i \leq p$ và do đó
$$
\begin{align*}
\zeta(x) &= x_1 \mathbin{\mathbf{H}} x_2 \mathbin{\mathbf{H}} \cdots \mathbin{\mathbf{H}} (\eta \theta(x_j)) \mathbin{\mathbf{H}} \cdots \mathbin{\mathbf{H}} x_p \\
y(x) &= x_j - \eta \theta(x_j).
\end{align*}
$$
Khi đó theo (5)
$$
\psi(x) = (x_1, \ldots, \eta \theta(x_j) + x_j - \eta \theta(x_j), \ldots, x_p) = (x_1, x_2, \ldots, x_p).
$$
Do đó $\psi \circ \phi = \mathrm{Id}_{a_1 \times \ldots \times a_p}$. Điều này chứng minh (i). Vì luật Hausdorff là đa thức, $\phi$ là đa thức. Theo giả thiết quy nạp, ${\phi'}^{-1}$ là đa thức; theo công thức (1), các hàm $x_j'$ là đa thức, do đó $\zeta$ là đa thức (công thức (3)), $y$ là đa thức (công thức (4)) và $\psi$ là đa thức (công thức (5)). Điều này chứng minh (ii). Mệnh đề (iii) suy ra từ (i) và (ii) và sự kiện rằng luật Hausdorff là đa thức.

**Ví dụ về một nhóm Lie lũy linh.** Cho $G$ là nhóm con tam giác ngặt dưới của $\mathbf{GL}(n, K)$. Nó là một nhóm con Lie của $\mathbf{GL}(n, K)$ và $L(G) \subset \mathfrak{gl}(n, K)$ là đại số Lie của các ma trận tam giác dưới với đường chéo bằng không (\S 3, no. 10, Mệnh đề 36). Theo Chương II, \S 4, no. 6, *Nhận xét*, $G$ là lũy linh. Từ đây về sau giả sử rằng $K = \mathbf{R}$ hoặc $\mathbf{C}$. Vì $G$ là đồng phôi với $K^{n(n-1)/2}$, $G$ là đơn liên. Ánh xạ mũ từ $L(G)$ vào $G$ chính là ánh xạ
$$
u \mapsto \exp u = \sum_{k \geq 0} \frac{u^k}{k!} = \sum_{k=0}^{n-1} \frac{u^k}{k!}
$$
(\S 6, no. 4, *Ví dụ*). Theo Mệnh đề 13, ánh xạ mũ là một đẳng cấu của đa tạp $L(G)$ lên đa tạp $G$. Mệnh đề 17 của \S 6, no. 9 cho song ánh ngược $\log$. Ta trang bị $K^n$ một chuẩn. Theo *Các lý thuyết phổ*, Chương I, \S 4, no. 9, với $g \in G$ và $\|g - 1\| < 1$,
$$
\log g = \sum_{k \geq 1} \frac{(-1)^{k-1}}{k} (g - 1)^k
$$

nghĩa là
$$
\log g = \sum_{k=1}^{n-1} \frac{(-1)^{k-1}}{k} (g-1)^k.
$$
Nhưng hai vế của (6) là các hàm giải tích của $g$ với $g \in G$ và do đó bằng nhau với mọi $g \in G$.

#### Mệnh đề 18 {#lie-iii-s9-prop-18 .statement}

*Cho k là một trường giao hoán. V là một không gian vectơ có số chiều hữu hạn > 0 trên k và G là một nhóm con của $\mathbf{GL}(V)$ mà các phần tử của nó là unipotent.*
  (i) *Tồn tại một phần tử v khác không của V sao cho gv = v với mọi g \in G.*
  (ii) *Tồn tại một cơ sở B của V sao cho, với mọi g \in G, ma trận của g đối với B là tam giác dưới và tất cả các phần tử đường chéo của nó bằng 1.*
  (iii) *Nhóm G là lũy linh.*
    (a) Trước hết giả sử rằng k đóng đại số và biểu diễn đồng nhất của G là đơn. Cho a, b thuộc G. Khi đó
    $$
    \operatorname{Tr}(a(b-1)) = \operatorname{Tr}(ab-1) - \operatorname{Tr}(a-1) = 0 - 0 = 0
    $$
    vì $ab - 1$ và $a - 1$ là lũy linh. Vì không gian vectơ con của $\mathcal{L}(V)$ sinh bởi G là $\mathcal{L}(V)$ (*Đại số*, Chương VIII, § 4, Hệ quả 1 của Mệnh đề 2), $\operatorname{Tr}(u(b-1)) = 0$ với mọi $u \in \mathcal{L}(V)$ và do đó $b = 1$. Vì vậy $G = \{1\}$.
    (b) Bây giờ ta chuyển sang trường hợp tổng quát. Cho $\bar{k}$ là một bao đóng đại số của k, $\bar{V} = V \otimes_k \bar{k}$ và $\bar{G} \subset \mathbf{GL}(\bar{V})$ là tập hợp các $a \otimes 1$ với $a \in G$. Cho W (tương ứng. $W'$) là tập hợp các phần tử của V (tương ứng. $\bar{V}$) bất biến dưới G (tương ứng. $\bar{G}$). Khi đó $W' = W \otimes_k \bar{k}$ vì $W = \bigcap_{g \in G} \operatorname{Ker}(g-1)$ và $W' = \bigcap_{g \in G} \operatorname{Ker}(g-1) \otimes 1$. Nếu $V_1$ là một phần tử cực tiểu trong tập hợp các không gian vectơ con khác không của $\bar{V}$ ổn định dưới $\bar{G}$, thì $V_1 \subset W'$ theo phần (a) của chứng minh; do đó $W \neq \{0\}$, điều này chứng minh (i).
    (c) Bằng quy nạp theo $\dim V$, từ (i) suy ra rằng tồn tại một dãy tăng $(V_1, V_2, \ldots, V_n)$ các không gian vectơ con của V ổn định dưới G sao cho $V_n = V$ và nhóm tự đẳng cấu của $V_i/V_{i-1}$ được dẫn xuất một cách chính tắc từ G thu gọn về $\{1\}$ với mọi $i$ (ta quy ước rằng $V_r = \{0\}$ với $r \leq 0$). Điều này trước hết suy ra (ii) và do đó suy ra (iii) (Chương II, § 4, no. 6, *Nhận xét*).

#### Hệ quả 1 {#lie-iii-s9-prop-18-cor-1 .statement}

*Cho G là một nhóm Lie liên thông thực hoặc phức có số chiều hữu hạn. Để G lũy linh, điều kiện cần và đủ là mọi phần tử của Ad G đều lũy linh.*

Nếu mọi phần tử của Ad G là unipotent, thì Ad G là lũy linh (Mệnh đề 18) và do đó G, là một mở rộng trung tâm của Ad G, là lũy linh. Nếu G là lũy linh, $L(G)$ là lũy linh, do đó $\operatorname{ad} x$ là lũy linh với mọi $x \in L(G)$ và do đó $\operatorname{Ad}(\exp x) = \exp \operatorname{ad} x$ là unipotent; nhưng mọi phần tử của G đều có dạng $\exp x$ với một $x \in L(G)$ nào đó (Mệnh đề 14).

#### Hệ quả 2 {#lie-iii-s9-prop-18-cor-2 .statement}

*Mọi nhóm con giải tích của $\mathbf{GL}(n, K)$ gồm các phần tử unipotent đều là một nhóm con Lie đơn liên.*

Điều này suy ra từ các Mệnh đề 13 (ii) và 18 (ii) và sự kiện rằng nhóm tam giác ngặt dưới là đơn liên.

### 6. CÁC NHÓM LIE GIẢI ĐƯỢC

#### Mệnh đề 19 {#lie-iii-s9-prop-19 .statement}

*Một nhóm Lie hữu hạn chiều $G$. Để $L(G)$ giải được, điều kiện cần và đủ là $G$ sở hữu một nhóm con mở giải được.*

Chứng minh tương tự như chứng minh của Mệnh đề 12 của no. 5.

#### Mệnh đề 20 {#lie-iii-s9-prop-20 .statement}

*Cho $G$ là một nhóm Lie giải được đơn liên hữu hạn chiều $n$ trên $\mathbf{R}$ hoặc $\mathbf{C}$ và $g = L(G)$. Cho $(g_n, g_{n-1}, \ldots, g_0)$ là một dãy các đại số con của $g$ có các chiều $n, n-1, \ldots, 0$, sao cho $g_{i-1}$ là một iđêan của $g_i$ với $i = n, n-1, \ldots, 1.\dagger$ Cho $G_i$ là nhóm con nguyên của $G$ tương ứng với $g_i$. Cho $x_i$ là một vectơ của $g_i$ không thuộc $g_{i-1}$. Cho $\phi_i$ là ánh xạ*

$$
(\lambda_1, \lambda_2, \ldots, \lambda_i) \mapsto (\exp \lambda_1 x_1)(\exp \lambda_2 x_2) \cdots (\exp \lambda_i x_i)
$$

*của $K^i$ vào $G$. Khi đó $\phi_n$ là một đẳng cấu của các đa tạp giải tích và $\phi_i(K^i) = G_i$ với mọi $i$.*

Với $n = 0$ thì mệnh đề là hiển nhiên. Ta lập luận bằng quy nạp theo $n$. Gọi $H$ là nhóm con nguyên của $G$ sao cho $L(H) = Kx_n$. Theo § 6, no. 6, Hệ quả 1 của Mệnh đề 14, $H$ và $G_{n-1}$ là các nhóm con Lie đơn liên của $G$ và, như một nhóm Lie, $G$ là tích nửa trực tiếp của $H$ bởi $G_{n-1}$. Do đó $\lambda \mapsto \exp(\lambda x_n)$ là một đẳng cấu của $K$ lên $H$ và theo giả thiết quy nạp, ánh xạ

$$
(\lambda_1, \lambda_2, \ldots, \lambda_{n-1}) \mapsto (\exp \lambda_1 x_1)(\exp \lambda_2 x_2) \cdots (\exp \lambda_{n-1} x_{n-1})
$$

là một đẳng cấu của đa tạp giải tích $K^{n-1}$ lên đa tạp giải tích $G_{n-1}$, ánh xạ $K^i \times \{0\}$ vào $G_i$ với $i = 1, 2, \ldots, n-1$. Do đó có mệnh đề.

#### Mệnh đề 21 {#lie-iii-s9-prop-21 .statement}

*Cho $G$ là một nhóm Lie giải được liên thông đơn hữu hạn chiều trên $\mathbf{R}$ hoặc $\mathbf{C}$ và $M$ là một nhóm con nguyên của $G$. Khi đó $M$ là một nhóm con Lie của $G$ và liên thông đơn.*

Ta tiếp tục sử dụng ký hiệu $n, g, g_i, x_i, \phi$ của Mệnh đề 20 nhưng áp đặt lên các $x_i$ điều kiện bổ sung sau: giả sử $i_p > i_{p-1} > \cdots > i_1$ là các số nguyên $i$ sao cho $L(M) \cap g_i \neq L(M) \cap g_{i-1}$; khi đó ta lấy

$$
x_{i_k} \in L(M) \cap g_{i_k}
$$

\dagger Một dãy như vậy tồn tại theo Chương I, § 5, Mệnh đề 2.

với $k = 1, 2, \ldots, p$. Theo quy nạp theo $n$, dễ thấy rằng $(x_{i_p}, x_{i_{p-1}}, \ldots, x_{i_1})$ là một cơ sở của $L(M)$. Gọi $N$ là một nhóm Lie liên thông đơn sao cho tồn tại một đẳng cấu $h$ của $L(N)$ lên $L(M)$. Đặt
$$
y_p = h^{-1}(x_{i_p}), \ldots, y_1 = h^{-1}(x_{i_1}).
$$
Theo Mệnh đề 20, ánh xạ
$$
(\lambda_1, \lambda_2, \ldots, \lambda_p) \mapsto (\exp \lambda_1 y_1)(\exp \lambda_2 y_2) \cdots (\exp \lambda_p y_p)
$$
là một đẳng cấu của đa tạp $K^p$ lên đa tạp $N$. Tồn tại một cấu xạ nhóm Lie $\tau$ của $N$ vào $G$ sao cho $h = L(\tau)$ và $\tau(N) = M$ (\S 6, no. 2, Hệ quả 1 của Mệnh đề 1). Do đó $M$ là tập hợp các phần tử của $G$ có dạng
$$
\tau((\exp \lambda_1 y_1) \cdots (\exp \lambda_p y_p)) = \exp(\lambda_1 L(\tau)y_1) \cdots \exp(\lambda_p L(\tau)y_p)
= \exp(\lambda_1 x_{i_1}) \cdots \exp(\lambda_p x_{i_p}).
$$
Vậy $M = \phi(T)$ trong đó $T$ là một không gian con vectơ của $K^n$.

#### Mệnh đề 22 {#lie-iii-s9-prop-22 .statement}

*Giả sử rằng $K = \mathbf{R}$ hoặc $\mathbf{C}$. Cho $V$ là một không gian vectơ hữu hạn chiều và $G$ là một nhóm con giải được liên thông của $\mathbf{GL}(V)$. Giả sử rằng biểu diễn đồng nhất của $G$ là đơn.*
(i) *Nếu $K = \mathbf{R}$ thì $\dim V \leq 2$ và $G$ giao hoán.*
(ii) *Nếu $K = \mathbf{C}$ thì $\dim V = 1$.*
(i) Giả sử rằng $K = \mathbf{R}$. Khi đó bao đóng $H$ của $G$ trong $\mathbf{GL}(V)$ là một nhóm Lie con giải được liên thông của $\mathbf{GL}(V)$ (no. 1, Hệ quả 2 của Mệnh đề 1). Do đó $L(H)$ là giải được (Mệnh đề 19). Biểu diễn đồng nhất của $L(G)$ là đơn (\S 6, no. 5, Hệ quả 2 của Mệnh đề 13). Do đó $\dim V \leq 2$ và $L(G)$ giao hoán (Chương I, \S 5, Hệ quả 1 và 4 của Định lý 1). Do đó $G$ giao hoán.
(ii) Giả sử rằng $K = \mathbf{C}$. Cho $W$ là một phần tử cực tiểu trong số các không gian vectơ con thực khác không của $V$ ổn định dưới $G$. Không gian vectơ con phức của $V$ sinh bởi $W$ bằng $V$ vì biểu diễn đồng nhất của $G$ là đơn. Theo (i), $G|W$ giao hoán. Do đó $G$ giao hoán. Vì vậy mọi phần tử của $G$ là một phép vị tự (*Đại số*, Chương VIII, \S 4, Hệ quả 1 của Mệnh đề 2), sao cho $\dim V = 1$.

#### Hệ quả {#lie-iii-s9-n6-cor-1 .statement}

*Cho $V$ là một không gian vectơ phức có số chiều hữu hạn $> 0$ và $G$ là một nhóm con giải được liên thông của $\mathbf{GL}(V)$.*
(i) *Tồn tại một phần tử khác không $v$ của $V$ sao cho $gv \in Cv$ với mọi $g \in G$.*
(ii) *Tồn tại một cơ sở $B$ của $V$ sao cho, với mọi $g \in G$, ma trận của $g$ đối với $B$ là tam giác dưới.*
Cho $V_1$ là một phần tử cực tiểu trong số các không gian vectơ con khác không của $V$ ổn định dưới $G$. Theo Mệnh đề 22 (ii), $\dim V_1 = 1$. Điều này chứng minh (i). Bằng quy nạp theo $\dim V$, suy ra rằng tồn tại một dãy tăng $(V_1, V_2, \ldots, V_n)$ các không gian vectơ con của $V$ ổn định dưới $G$ sao cho $\dim V_{i+1}/V_i = 1$ với $i < n$ và $V_n = V$; do đó (ii).

### 7. CĂN CỦA MỘT NHÓM LIE

#### Mệnh đề 23 {#lie-iii-s9-prop-23 .statement}

*Cho $G$ là một nhóm Lie thực hoặc phức hữu hạn chiều, $r$ là căn của $L(G)$* (Chương I, § 5, Định nghĩa 2) *và $n$ là iđêan lũy linh lớn nhất của $L(G)$* (Chương I, § 4, no. 4). *Cho $R$ (tương ứng $N$) là nhóm con nguyên của $G$ có đại số Lie là $r$ (tương ứng $n$). Khi đó $R$ (tương ứng $N$) là một nhóm con Lie giải được (tương ứng lũy linh) của $G$, bất biến dưới mọi tự đẳng cấu liên tục của $G$. *Mọi nhóm con chuẩn liên thông giải được (tương ứng lũy linh) của $G$ đều được chứa trong $R$ (tương ứng $N$).*

Nhóm $R$ là giải được ($§ 6$, Mệnh đề 19). Giả sử rằng $K = R$. Cho $G'$ là một nhóm con chuẩn liên thông giải được của $G$. Khi đó $\overline{G'}$ là một nhóm con Lie chuẩn liên thông giải được (no. 1, Hệ quả 2 của Mệnh đề 1) của $G$ ($§ 8$, no. 2, Định lý 2). Do đó $L(\overline{G'})$ là một iđêan giải được của $L(G)$, do đó $L(\overline{G'}) \subset r$ và $\overline{G'} \subset R$. Đặc biệt, $\overline{R} \subset R$, do đó $R$ là đóng và vì vậy là một nhóm con Lie của $G$. Giả sử rằng $K = C$. Cho $H$ là nhóm con Lie thực nền của $G$. Nếu $r'$ là căn của $L(H)$, $ir'$ là một iđêan giải được của $L(H)$, do đó $r' = ir'$; vì vậy $r \subset r' \subset r$ và, theo trên, $R$ là đóng trong $H$ và do đó trong $G$; vậy nên $R$ là một nhóm con Lie của $G$. Mọi nhóm con chuẩn liên thông giải được của $G$ là một nhóm con chuẩn liên thông giải được của $H$ và do đó được chứa trong $R$. Vì vậy ta đã chứng minh rằng với $K = C$ và với $K = R$, $R$ là nhóm con chuẩn liên thông giải được lớn nhất của $G$; do đó $R$ là bất biến dưới mọi tự đẳng cấu liên tục của $G$. Chứng minh đối với $N$ hoàn toàn tương tự.

#### Định nghĩa 1 {#lie-iii-s9-def-1 .statement}

*Cho $G$ là một nhóm Lie thực hoặc phức hữu hạn chiều. Căn của $G$ là nhóm con chuẩn liên thông giải được lớn nhất của $G$.*

#### Nhận xét {#lie-iii-s9-n7-rem-1 .statement}

Ngay cả khi $G$ liên thông, có thể có các nhóm con chuẩn giải được của $G$ không được chứa trong căn của $G$.

#### Mệnh đề 24 {#lie-iii-s9-prop-24 .statement}

*Giả sử rằng $K = R$ hoặc $C$. Cho $G_1, G_2$ là hai nhóm Lie liên thông hữu hạn chiều, $R_1$ và $R_2$ là các căn của chúng và $\phi$ là một cấu xạ toàn ánh từ $G_1$ vào $G_2$. Khi đó $\phi(R_1) = R_2$.*

Theo $§ 3$, no. 8, Mệnh đề 28, $L(\phi)$ là toàn ánh. Do đó $L(\phi)(L(R_1)) = L(R_2)$ (Chương I, $§ 6$, Hệ quả 3 của Mệnh đề 2). Gọi $i$ là đơn ánh chính tắc của $R_1$ vào $G_1$. Khi đó ảnh của $\phi \circ i$ là $R_2$ ($§ 6$, no. 2, Hệ quả 1 của Mệnh đề 1).

#### Mệnh đề 25 {#lie-iii-s9-prop-25 .statement}

*Giả sử rằng $K = R$ hoặc $C$. Cho $G_1, G_2$ là các nhóm Lie liên thông hữu hạn chiều và $R_1$ và $R_2$ là các căn của chúng. Căn của $G_1 \times G_2$ là $R_1 \times R_2$.*

Điều này suy ra từ Chương I, $§ 5$, Mệnh đề 4.

### 8. CÁC NHÓM LIE NỬA ĐƠN

#### Mệnh đề 26 {#lie-iii-s9-prop-26 .statement}

Cho G là một nhóm Lie thực hoặc phức liên thông hữu hạn chiều. Các điều kiện sau là tương đương:
(i) $L(G)$ là nửa đơn;
(ii) căn của G là $\{e\}$;
(iii) mọi nhóm con giao hoán nguyên chuẩn của G đều bằng $\{e\}$.
Điều kiện (ii) có nghĩa là căn của $L(G)$ là $\{0\}$ và do đó (i) $\Leftrightarrow$ (ii) (Chương I, § 6, Định lý 1). Sự tương đương của (i) và (iii) suy ra từ § 6, no. 6, Mệnh đề 14.

#### Định nghĩa 2 {#lie-iii-s9-def-2 .statement}

Một nhóm Lie thực hoặc phức liên thông được gọi là nửa đơn nếu nó hữu hạn chiều và thỏa mãn các điều kiện của Mệnh đề 26.

#### Nhận xét 1 {#lie-iii-s9-n8-rem-1 .statement}

Cho G là một nhóm Lie thực hoặc phức liên thông hữu hạn chiều. Nếu G không là nửa đơn, G có một nhóm con Lie giao hoán liên thông $G'$ bất biến dưới mọi tự đẳng cấu liên tục, sao cho $G' \neq \{e\}$. Thật vậy, gọi n là iđêan lũy linh lớn nhất của $L(G)$; khi đó $n \neq \{0\}$ và nhóm con giải tích tương ứng N là một nhóm con Lie bất biến dưới mọi tự đẳng cấu liên tục của G (no. 7, Mệnh đề 23); tâm $G'$ của N có các tính chất mong muốn.

#### Mệnh đề 27 {#lie-iii-s9-prop-27 .statement}

Cho G là một nhóm Lie thực hoặc phức liên thông hữu hạn chiều. Các điều kiện sau là tương đương:
(i) $L(G)$ là đơn;
(ii) các nhóm con nguyên chuẩn duy nhất của G là $\{e\}$ và G, và hơn nữa G không giao hoán.
Điều này suy ra từ § 6, no. 6, Mệnh đề 14.

#### Định nghĩa 3 {#lie-iii-s9-def-3 .statement}

Một nhóm Lie thực hoặc phức liên thông được gọi là gần đơn nếu nó hữu hạn chiều và thỏa mãn các điều kiện của Mệnh đề 27.

#### Mệnh đề 28 {#lie-iii-s9-prop-28 .statement}

Cho G là một nhóm Lie thực hoặc phức đơn liên. Các điều kiện sau là tương đương:
(i) G là nửa đơn;
(ii) G đẳng cấu với tích của một số hữu hạn các nhóm gần đơn.
Nếu G là một tích hữu hạn của các nhóm Lie gần đơn, $L(G)$ là một tích hữu hạn của các đại số Lie đơn và do đó là nửa đơn. Nếu G là nửa đơn, $L(G)$ đẳng cấu với một tích của các đại số Lie đơn $L_1, \ldots, L_n$. Gọi $G_i$ là một nhóm Lie đơn liên có đại số Lie $L_i$, do đó nó là gần đơn. Khi đó G và $G_1 \times \cdots \times G_n$ là đơn liên và có các đại số Lie đẳng cấu, do đó chúng đẳng cấu.

#### Bổ đề 1 {#lie-iii-s9-lem-1 .statement}

Cho G là một nhóm tôpô liên thông, Z là tâm của nó và $Z'$ là một nhóm con rời rạc của Z. Khi đó tâm của $G/Z'$ là $Z/Z'$.
Gọi y là một phần tử của G mà lớp của nó modulo $Z'$ là một phần tử trung tâm của

G/Z'. Gọi $\phi$ là ánh xạ $g \mapsto gyg^{-1}y^{-1}$ của G vào G. Khi đó $\phi(G)$ là liên thông và được chứa trong $Z'$ và do đó $\phi(G) = \phi(\{e\}) = \{e\}$. Vì vậy $y \in Z$.

#### Mệnh đề 29 {#lie-iii-s9-prop-29 .statement}

*Cho G là một nhóm Lie liên thông nửa đơn thực hoặc phức.*
(i) $G = (G, G)$.
(ii) *Tâm Z của G là rời rạc.*
(iii) *Tâm của $G/Z$ là $\{e\}$*.
Mệnh đề (i) suy ra từ Hệ quả của Mệnh đề 4, no. 2 và Chương I, § 6, Định lý 1.
Mệnh đề (ii) suy ra từ § 6, no. 4, Hệ quả 4 của Mệnh đề 10 và Chương I, § 6, no. 1, *Nhận xét 2*.
Mệnh đề (iii) suy ra từ (ii) và Bổ đề 1.

#### Mệnh đề 30 {#lie-iii-s9-prop-30 .statement}

(i) *Cho $\mathfrak{g}$ là một đại số Lie nửa đơn thực hoặc phức. Khi đó Int $\mathfrak{g}$ là thành phần đơn vị của Aut $\mathfrak{g}$.*.
(ii) *Cho G là một nhóm Lie liên thông nửa đơn thực hoặc phức. Nhóm phụ hợp của G là thành phần đơn vị của Aut $L(G)$. Tâm của nó thu gọn về phần tử đơn vị.*
Mọi đạo hàm của $\mathfrak{g}$ đều là nội (Chương I, § 6, Hệ quả 3 của Mệnh đề 1) và do đó $L(\mathrm{Int}\,\mathfrak{g}) = L(\mathrm{Aut}\,\mathfrak{g})$, điều này chứng minh (i). Mệnh đề đầu tiên của (ii) suy ra từ (i). Mệnh đề thứ hai suy ra từ Mệnh đề 29 (iii) và § 6, no. 4, Hệ quả 4 (ii) của Mệnh đề 10.

#### Nhận xét 2 {#lie-iii-s9-n8-rem-2 .statement}

Cho $\mathfrak{g}$ là một đại số Lie nửa đơn phức và $\mathfrak{g}_0$ là đại số Lie thực nền của nó. Khi đó Aut$(\mathfrak{g})$ là mở trong Aut$(\mathfrak{g}_0)$, vì Int$(\mathfrak{g}_0) \subset \mathrm{Aut}(\mathfrak{g})$.

#### Mệnh đề 31 {#lie-iii-s9-prop-31 .statement}

*Cho G là một nhóm Lie liên thông đơn liên hữu hạn chiều thực hoặc phức và R là căn của nó. Tồn tại một nhóm Lie con S nửa đơn đơn liên của G sao cho G, như một nhóm Lie, là tích nửa trực tiếp của S bởi R. Nếu S' là một nhóm con nguyên nửa đơn của G, tồn tại x trong căn lũy linh của $L(G)$ sao cho*
$$
(\mathrm{Ad}\exp x)(S') \subset S.
$$
Điều này suy ra từ § 6, no. 6, Hệ quả 1 của Mệnh đề 14 và Chương I, § 6, Định lý 5 và Hệ quả 1.

#### Bổ đề 2 {#lie-iii-s9-lem-2 .statement}

*Cho G là một nhóm (tương ứng, một nhóm tôpô), G' là một nhóm con chuẩn của G, V là một không gian vectơ hữu hạn chiều trên một trường giao hoán k (tương ứng, trên K), $\rho$ là một biểu diễn tuyến tính (tương ứng, một biểu diễn tuyến tính liên tục) của G trên V và $\rho' = \rho|_{G'}$.*
(i) *Nếu $\rho$ là nửa đơn, $\rho'$ là nửa đơn.*
(ii) *Nếu $\rho'$ là nửa đơn và mọi biểu diễn tuyến tính k hữu hạn chiều (tương ứng, biểu diễn tuyến tính liên tục K) của $G/G'$ (tương ứng, $G/\overline{G}'$) là nửa đơn, thì $\rho$ là nửa đơn.*
Giả sử rằng $\rho$ là nửa đơn; ta chứng minh rằng $\rho'$ là nửa đơn. Chỉ cần xét trường hợp $\rho$ là đơn. Cho $V'$ là một môđun con-G' cực tiểu khác không của V. Với mọi $g \in G$, $\rho(G')\rho(g)V' = \rho(g)\rho(G')V' = \rho(g)V'$, nói cách khác $\rho(g)V'$ ổn định dưới $\rho(G')$; nếu $V''$ là một môđun con-$G'$ của $\rho(g)V'$, thì $\rho(g)^{-1}V''$ là một môđun con-$G'$ của $V'$ và do đó $V''$ bằng $\{0\}$ hoặc $\rho(g)V'$.

Vì vậy, với mọi $g \in G$, $\rho(g)V'$ là một môđun $G'$ đơn. Nhưng $\sum_{g \in G} \rho(g)V'$ là một môđun con-$G$ khác không của $V$, do đó $V = \sum_{g \in G} \rho(g)V'$. Do đó $\rho'$ là nửa đơn.

Giả sử rằng $\rho'$ là nửa đơn. Cho $W$ là một môđun con-$G$ khác không của $V$. Vì $\rho'$ là nửa đơn, tồn tại một phép chiếu $f_0$ của $V$ lên $W$ giao hoán với $\rho'(G)$. Gọi $E$ là tập hợp các $f \in \mathcal{L}(V, V)$ giao hoán với $\rho(G')$, ánh xạ $V$ vào $W$ và hạn chế của nó trên $W$ là một phép vị tự; với $f \in E$, ký hiệu $\alpha(f)$ là tỉ số của phép vị tự $f|W$. Khi đó $f_0 \in E$ và $\alpha(f_0) = 1$. Rõ ràng $\alpha$ là một dạng tuyến tính trên $E$. Gọi $F = \mathrm{Ker}\, \alpha$, là một siêu phẳng của $E$. Với $f \in E$ và $g \in G$, ta viết $\sigma(g)f = \rho(g) \circ f \circ \rho(g)^{-1}$; khi đó $\sigma(g)f$ ánh xạ $V$ vào $W$ và hạn chế của nó trên $W$ là phép vị tự có tỉ số $\alpha(f')$; nếu $g' \in G'$, thì
$$
\begin{align*}
\sigma(g)f \circ \rho(g') &= \rho(g) \circ f \circ \rho(g)^{-1} \circ \rho(g') \\
&= \rho(g) \circ f \circ \rho(g^{-1}g'g) \circ \rho(g^{-1}) \\
&= \rho(g) \circ \rho(g^{-1}g'g) \circ f \circ \rho(g^{-1}) \\
&= \rho(g') \circ \rho(g) \circ f \circ \rho(g^{-1}) \\
&= \rho(g') \circ \sigma(g)f.
\end{align*}
$$
Suy ra $\sigma(g)f \in E$. Do đó $\sigma$ là một $k$-biểu diễn tuyến tính (tương ứng một $K$-biểu diễn tuyến tính liên tục) của $G$ trên $E$ để lại $F$ ổn định. Khi đó $\sigma(g) = \mathrm{Id}_E$ với $g \in G'$ và do đó với $g \in \overline{G'}$ trong trường hợp tôpô. Giả sử rằng mọi biểu diễn tuyến tính $k$ hữu hạn chiều (tương ứng mọi biểu diễn tuyến tính $K$ liên tục) của $G/G'$ (tương ứng $G/\overline{G'}$) đều nửa đơn. Khi đó tồn tại trong $E$ một phần bù của $F$ ổn định dưới $G$. Nói cách khác, tồn tại $f \in E$ sao cho $\alpha(f) = 1$, bất biến dưới $G$. Khi đó $f$ là một phép chiếu của $V$ lên $W$, và, với $g \in G$, $\rho(g) \circ f \circ \rho(g^{-1}) = f$, nghĩa là $f$ giao hoán với $\rho(G)$. Vậy $\rho$ là nửa đơn.

#### Định lý 1 {#lie-iii-s9-thm-1 .statement}

*Cho $G$ là một nhóm Lie thực hoặc phức hữu hạn chiều, $G_0$ là thành phần đơn vị của nó, $R$ là căn của nó và $r$ là căn của $L(G)$; giả sử rằng $G/G_0$ là hữu hạn. Cho $\rho$ là một biểu diễn tuyến tính giải tích hữu hạn chiều của $G$. Các điều kiện sau là tương đương:*
(i) $\rho$ là nửa đơn;
(ii) $\rho|G_0$ là nửa đơn;
(iii) $\rho|R$ là nửa đơn;
(iv) $L(\rho)$ là nửa đơn;
(v) $L(\rho)|r$ là nửa đơn.
(i) $\Leftrightarrow$ (ii) theo Bổ đề 2 và *Integration*, Chương VII, § 3, Mệnh đề 1.
(ii) $\Leftrightarrow$ (iv) và (iii) $\Leftrightarrow$ (v) theo § 6, no. 5, Hệ quả 2 của Mệnh đề 13.
(iv) $\Leftrightarrow$ (v) theo Chương I, § 6, Định lý 4.

#### Hệ quả 1 {#lie-iii-s9-thm-1-cor-1 .statement}

*Cho $\rho, \rho_1, \rho_2$ là các biểu diễn tuyến tính giải tích nửa đơn hữu hạn chiều của $G$ và $n$ là một số nguyên $\geq 0$. Khi đó $\rho_1 \otimes \rho_2, T^n \rho, S^n \rho, \wedge^n \rho$ (Phụ lục) là nửa đơn.*

Tính nửa đơn của $\rho_1 \otimes \rho_2$ suy ra từ Định lý 1 và Chương I, § 6, Hệ quả 1 của Định lý 4. Tính nửa đơn của $T^n \rho, S^n \rho, \wedge^n \rho$ suy ra từ tính nửa đơn của $\rho_1 \otimes \rho_2$.

Ta sẽ thấy sau rằng, nếu $k$ là một trường giao hoán có đặc số 0, $\Gamma$ là một nhóm và $\rho_1$ và $\rho_2$ là các biểu diễn tuyến tính $k$ nửa đơn hữu hạn chiều của $\Gamma$, thì $\rho_1 \otimes \rho_2$ là nửa đơn.

#### Hệ quả 2 {#lie-iii-s9-thm-1-cor-2 .statement}

*Cho $\rho$ là một biểu diễn tuyến tính giải tích nửa đơn hữu hạn chiều của $G$ trên một không gian vectơ $V$, $S$ là đại số đối xứng của $V$ và $S^G$ là đại số con của $S$ gồm các phần tử bất biến dưới tác dụng của $(S\rho)(G)$. Khi đó $S^G$ là một đại số sinh hữu hạn.*

Điều này suy ra từ Định lý 1, Chương I, § 6, Định lý 6 (a) và *Đại số giao hoán*, Chương V, § 1, Định lý 2.

#### Hệ quả 3 {#lie-iii-s9-thm-1-cor-3 .statement}

*Cho $G$ là một nhóm Lie thực hoặc phức và $G_0$ là thành phần đơn vị của nó. Giả sử rằng $G_0$ là nửa đơn và rằng $G/G_0$ là hữu hạn. Khi đó mọi biểu diễn tuyến tính giải tích hữu hạn chiều của $G$ đều là nửa đơn.*

#### Mệnh đề 32 {#lie-iii-s9-prop-32 .statement}

*Cho $G$ là một nhóm Lie thực liên thông hữu hạn chiều. Giả sử rằng $L(G)$ là khả quy. Các điều kiện sau là tương đương:*

(i) $G/\overline{D^1}G$ là compact;
(ii) (resp. (ii')) mọi biểu diễn tuyến tính giải tích hữu hạn chiều của $G$ trên một không gian vectơ phức (resp. thực) đều là nửa đơn.

(i) $\Rightarrow$ (ii'): Giả sử rằng $G/\overline{D^1}G$ là compact. Khi đó mọi biểu diễn tuyến tính liên tục của $G/\overline{D^1}G$ trên một không gian vectơ thực hữu hạn chiều đều là nửa đơn (*Integration*, Chương VII, § 3, Mệnh đề 1). Cho $\rho$ là một biểu diễn tuyến tính giải tích hữu hạn chiều của $G$ trên một không gian vectơ thực. Khi đó $\rho|D^1G$ là giải tích, $D^1G$ là nửa đơn (Chương I, § 6, Mệnh đề 5) và do đó $\rho|D^1G$ là nửa đơn (Hệ quả 3 của Định lý 1). Vì vậy $\rho$ là nửa đơn (Bổ đề 2).

Tương tự, có thể thấy rằng (i) $\Rightarrow$ (ii').

(i) $\Rightarrow$ (ii): Giả sử rằng $G/\overline{D^1}G$ không compact và do đó đẳng cấu với một nhóm có dạng $\mathbf{R}^p \times \mathbf{T}^q$ với $p > 0$ ($\S 6$, no. 4, Mệnh đề 11 (ii)). Khi đó tồn tại một cấu xạ toàn ánh từ $G/\overline{D^1}G$ lên $\mathbf{R}$ và do đó tồn tại một cấu xạ toàn ánh từ $G$ lên $\mathbf{R}$. Ánh xạ

$$
g \mapsto \sigma(g) = \begin{pmatrix} 1 & 0 \\ \rho(g) & 1 \end{pmatrix}
$$

là một biểu diễn tuyến tính giải tích của $G$ trên $\mathbf{R}^2$ không nửa đơn, vì không gian con vectơ chiều 1 duy nhất của $\mathbf{R}^2$ ổn định dưới $\sigma(G)$ là $\mathbf{R}(0, 1)$.

Tương tự, có thể thấy rằng (ii) $\Rightarrow$ (i).

#### Mệnh đề 33 {#lie-iii-s9-prop-33 .statement}

Cho G là một nhóm Lie phức hữu hạn chiều mà số các thành phần liên thông là hữu hạn, $\varphi$ là một biểu diễn tuyến tính giải tích hữu hạn chiều của G và $G'$ là một nhóm con nguyên của nhóm Lie thực G sao cho $L(G')$ sinh ra $L(G)$ trên $\mathbf{C}$. Khi đó, để $\varphi$ nửa đơn, điều kiện cần và đủ là $\varphi|G'$ nửa đơn.

Đặt $\varphi' = \varphi|G'$. Để $\varphi$ (tương ứng $\varphi'$) nửa đơn, điều kiện cần và đủ là $L(\varphi)$ (tương ứng $L(\varphi')$) nửa đơn (Định lý 1). Gọi V là không gian của $\varphi$. Để một không gian con vectơ của V ổn định dưới $L(\varphi)(L(G))$, điều kiện cần và đủ là nó ổn định dưới $L(\varphi')(L(G'))$. Suy ra mệnh đề.

### Bài tập {#lie-iii-s9-exercises}

Xem [các bài tập của § 9](exercises/s9/).
