---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: IV
chapter_title: COXETER GROUPS AND TITS SYSTEMS
section: 2
section_title: Tits Systems
lang: vi
source: lie-iv-vi
pdf_pages: 0028-0039, 0057-0072
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITIONS AND FIRST PROPERTIES
      page: 0
      pdf_page: 28
    - "no": 2
      title: AN EXAMPLE
      page: 0
      pdf_page: 30
    - "no": 3
      title: DECOMPOSITION OF G INTO DOUBLE COSETS
      page: 0
      pdf_page: 31
    - "no": 4
      title: RELATIONS WITH COXETER SYSTEMS
      page: 0
      pdf_page: 32
    - "no": 5
      title: SUBGROUPS OF G CONTAINING B
      page: 0
      pdf_page: 34
    - "no": 6
      title: PARABOLIC SUBGROUPS
      page: 0
      pdf_page: 35
    - "no": 7
      title: SIMPLICITY THEOREMS
      page: 0
      pdf_page: 36
statements: 30
exercises: 29
content_sha256: fc2b05c2065d3f9c7289fd9d092c291489740115ca0e1173cd7905f0d8ddf979
translated_from: content/en/lie/IV/02_s2_tits_systems.md
source_content_sha256: 346fa786ae647c2beb4852bcd6c8923f06ef4caf1b9f5ab62db22180acbb91d4
translation_model: gpt-5-6, gpt-5-6-mini
translation_run: translate-vi-c6e81366
glossary_version: 34
glossary_terms_sha256: f74b5b9a5c899256bb65cd0d8a4fe74a0ee0f555912d12b18e6d00fd43a77ec1
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 2. CÁC HỆ TITS

Trong đoạn này, các chữ G, B, N, S, T, W có nghĩa được chỉ ra trong no. 1 dưới đây.

### 1. ĐỊNH NGHĨA VÀ CÁC TÍNH CHẤT ĐẦU TIÊN

Cho G là một nhóm và B là một nhóm con của G. Nhóm $B \times B$ tác động lên G bởi $(b, b').g = bgb'^{-1}$ với $b, b' \in B$ và $g \in G$. Các quỹ đạo của $B \times B$ trên G là các tập hợp $BgB$ với $g \in G$, và được gọi là các lớp ghép kép của G đối với B. Chúng lập thành một phân hoạch của G; thương tương ứng được ký hiệu bởi $B \backslash G / B$. Nếu C và $C'$ là các lớp ghép kép, $CC'$ là một hợp của các lớp ghép kép.

#### Định nghĩa 1 {#lie-iv-s2-def-1 .statement}

Một hệ Tits là một bộ bốn $(G, B, N, S)$, trong đó G là một nhóm, B và N là hai nhóm con của G và S là một tập con của $N/(B \cap N)$, thỏa mãn các tiên đề sau:

(T1) Tập hợp $B \cup N$ sinh ra G và $B \cap N$ là một nhóm con chuẩn tắc của N.
(T2) Tập hợp S sinh ra nhóm $W = N/(B \cap N)$ và gồm các phần tử có cấp 2.
(T3) $sBw \subset BwB \cup BswB$ với $s \in S$ và $w \in W$.
(T4) Với mọi $s \in S$, $sBs \notin B$.

Nhóm $W = N/(B \cap N)$ đôi khi được gọi là nhóm Weyl của hệ Tits $(G, B, N, S)$.

5 Mọi phần tử của W là một lớp ghép modulo $B \cap N$, và do đó là một tập con của G; vì vậy các tích như $BwB$ có nghĩa. Nói chung hơn, với mọi tập con A của W, ta ký hiệu BAB là tập hợp $\bigcup_{w \in A} BwB$.

#### Nhận xét 1 {#lie-iv-s2-n1-rem-1 .statement}

Ta sẽ thấy trong no. 5 (Hệ quả của Định lý 3) rằng, nếu $(G, B, N)$ đã cho, tồn tại nhiều nhất một tập con $S$ của $N/(B \cap N)$ sao cho $(G, B, N, S)$ là một hệ Tits.

#### Nhận xét 2 {#lie-iv-s2-n1-rem-2 .statement}

Cho $(G, B, N, S)$ là một hệ Tits, và cho $Z$ là một nhóm con chuẩn tắc của G được chứa trong B. Cho $G' = G/Z, B' = B/Z, N' = N/(Z \cap N)$, và cho $S'$ là ảnh của S trong $N'/(B' \cap N')$. Khi đó ta thấy ngay lập tức rằng $(G', B', N', S')$ là một hệ Tits.

Trong suốt đoạn này, với $(G, B, N, S)$ ký hiệu một hệ Tits, ta đặt $T = B \cap N$ và $W = N/T$. Một lớp ghép kép nghĩa là một lớp ghép kép của $G$ đối với $B$. Với mọi $w \in W$, ta đặt $C(w) = BwB$; đây là một lớp ghép kép.

Ta sẽ suy ra một số hệ quả sơ cấp của các tiên đề (T1) đến (T4). Ta ký hiệu bởi $w, w', \ldots$ các phần tử của W và bởi $s, s', \ldots$ các phần tử của S. Các quan hệ sau là hiển nhiên:

$$
C(1) = B, \quad C(ww') \subset C(w).C(w'), \quad C(w^{-1}) = C(w)^{-1}.
$$

Tiên đề (T3) cũng có thể được viết dưới dạng

$$
C(s).C(w) \subset C(w) \cup C(sw).
$$

Hơn nữa, vì $C(sw) \subset C(s).C(w)$ theo (1) và vì $C(s).C(w)$ là một hợp của các lớp ghép kép, chỉ có hai khả năng:

$$
C(s).C(w) = \begin{cases}
C(sw) & \text{nếu } C(w) \not\subset C(s).C(w) \\
C(w) \cup C(sw) & \text{nếu } C(w) \subset C(s).C(w).
\end{cases}
$$

Theo (T4), $B \neq C(s).C(s)$; đặt $w = s$ trong (3) và sử dụng quan hệ $s^2 = 1$, ta thu được

$$
C(s).C(s) = B \cup C(s).
$$

Công thức này chỉ ra rằng $B \cup C(s)$ là một nhóm con của $G$. Nhân cả hai vế của (4) bên phải với $C(w)$, và sử dụng công thức (3) cùng quan hệ

$$
B.C(w) = C(w),
$$

ta thu được

$$
C(s).C(s).C(w) = C(w) \cup C(sw).
$$

Lấy các tập nghịch đảo của các tập xuất hiện trong các công thức (2), (3) và (5), rồi thay thế $w$ bởi $w^{-1}$, ta thu được các công thức

$$
C(w).C(s) \subset C(w) \cup C(ws)
$$
$$
C(w).C(s) = \begin{cases}
C(ws) & \text{nếu } C(w) \not\subset C(w).C(s) \\
C(w) \cup C(ws) & \text{nếu } C(w) \subset C(w).C(s)
\end{cases}
$$
$$
C(w).C(s).C(s) = C(w) \cup C(ws).
$$

#### Bổ đề 1 {#lie-iv-s2-lem-1 .statement}

Cho $s_1, \ldots, s_q \in S$ và cho $w \in W$. Ta có
$$
C(s_1 \ldots s_q).C(w) \subset \bigcup_{(i_1, \ldots, i_p)} C(s_{i_1} \ldots s_{i_p} w),
$$
trong đó $(i_1, \ldots, i_p)$ là tập hợp các dãy tăng ngặt của các số nguyên trong khoảng $[1, q]$.

Ta lập luận bằng quy nạp theo $q$, trường hợp $q = 0$ là tầm thường. Nếu $q \geqslant 1$, ta có $C(s_1 \ldots s_q).C(w) \subset C(s_1).C(s_2 \ldots s_q).C(w)$. Theo giả thiết quy nạp, $C(s_2 \ldots s_q).C(w)$ được chứa trong hợp của các $C(s_{j_1} \ldots s_{j_p} w)$, trong đó
$$
2 \leq j_1 < \cdots < j_p \leq q.
$$
Theo (T3), tập $C(s_1).C(s_{j_1} \ldots s_{j_p} w)$ được chứa trong hợp của các tập $C(s_1 s_{j_1} \ldots s_{j_p} w)$ và $C(s_{j_1} \ldots s_{j_p} w)$. Điều này chứng minh bổ đề.

### 2. MỘT VÍ DỤ

Cho $k$ là một trường, $n$ là một số nguyên $\geq 0$, và $(e_i)$ là cơ sở chính tắc của $k^n$. Cho $G = \mathbf{GL}(n, k)$, cho $B$ là nhóm con tam giác trên của $G$, và cho $N$ là nhóm con của $G$ gồm các ma trận có đúng một phần tử khác không trong mỗi hàng và cột. Một phần tử của $N$ hoán vị các đường thẳng $ke_i$; điều này cho một đồng cấu toàn ánh $N \to \mathcal{S}_n$ có hạt nhân là nhóm con $T = B \cap N$ gồm các ma trận đường chéo, và cho phép ta đồng nhất $W = N/T$ với $\mathcal{S}_n$. Ta ký hiệu bởi $s_j$ ($1 \leq j \leq n-1$) phần tử của $W$ tương ứng với phép chuyển vị của $j$ và $j+1$; cho $S$ là tập hợp các $s_j$. *Bộ bốn* $(G, B, N, S)$ *là một hệ Tits*. Thật vậy:

Tiên đề (T1) suy ra từ Hệ quả 2 của Mệnh đề 14 của *Algebra*, Chương II, § 10, no. 13.

Tiên đề (T2) được chứng minh trong *Algebra*, Chương I, Đính chính cho p. 97.
Tiên đề (T4) là ngay lập tức.
Còn lại là kiểm tra tiên đề (T3), tức là
$$
s_j B w \subset B w B \cup B s_j w B \quad \text{với } 1 \leq j \leq n-1, w \in W,
$$
hay tương đương,
$$
s_j B \subset B B' \cup B s_j B', \quad \text{với } B' = w B w^{-1}.
$$
Cho $G_j$ là nhóm con của $G$ gồm các phần tử cố định các $e_i$ với $i \neq j, j+1$ và ổn định mặt phẳng sinh bởi $e_j$ và $e_{j+1}$; nhóm này đẳng cấu với $\mathbf{GL}(2, k)$. Ta kiểm tra được rằng $G_j B = B G_j$. Vì $s_j \in G_j$, ta có $s_j B \subset B G_j$, và chỉ cần chứng minh rằng
$$
G_j \subset (B \cap G_j)(B' \cap G_j) \cup (\cap G_j) s_j (B' \cap G_j).
$$
Đồng nhất $G_j$ với $\mathbf{GL}(2, k)$; nhóm $B \cap G_j$ khi đó được đồng nhất với nhóm con tam giác trên $B_2$ của $\mathbf{GL}(2, k)$, trong khi nhóm $B' \cap G_j$ được đồng nhất với $B_2$ khi $w(j) < w(j+1)$ và với nhóm con tam giác dưới $B_2^-$ trong trường hợp ngược lại. Trong trường hợp thứ nhất, công thức cần chứng minh có thể viết là

$$
\mathbf{GL}(2, k) = B_2 \cup B_2 s B_2 \quad \text{trong đó } s = \begin{pmatrix} 0 & 1 \\ 1 & 0 \end{pmatrix};
$$

điều này suy ra chẳng hạn từ sự kiện rằng $B_2$ là nhóm ổn định của một điểm đối với tác động của $\mathbf{GL}(2, k)$ lên đường thẳng xạ ảnh $\mathbf{P}_1(k)$, và tác động bắc cầu trên phần bù của điểm này. Trong trường hợp thứ hai, công thức cần chứng minh có thể viết là

$$
\mathbf{GL}(2, k) = B_2 B_2^- \cup B_2 s B_2^-;
$$

vì $B_2^- = s B_2 s$, điều này suy ra từ công thức trước bằng cách nhân bên phải với $s$.

### 3. PHÂN TÍCH CỦA G THÀNH CÁC LỚP KÉP

#### Định lý 1 {#lie-iv-s2-thm-1 .statement}

*Ta có $G = \mathrm{BWB}$. Ánh xạ $w \mapsto C(w)$ là một song ánh từ $W$ đến tập hợp $B \backslash G / B$ gồm các lớp kép của $G$ đối với $B$.*

Hiển nhiên rằng $\mathrm{BWB}$ ổn định đối với $x \mapsto x^{-1}$, và Bổ đề 1 chỉ ra rằng nó ổn định đối với tích. Vì nó chứa $B$ và $N$, nên nó bằng $G$.

Còn lại là chứng minh rằng $C(w) \neq C(w')$ nếu $w \neq w'$. Vì mục đích này, ta sẽ chứng minh bằng quy nạp theo số nguyên $q$ mệnh đề sau:

(A_q) Nếu $w$ và $w'$ là các phần tử phân biệt của $W$ sao cho $l_S(w) \geq l_S(w') = q$, thì $C(w) \neq C(w')$.

(Để biết định nghĩa của $l_S(w)$, xem § 1, no. 1.)

Mệnh đề này là hiển nhiên với $q = 0$, vì khi đó $w' = 1$ và $w \neq 1$, do đó $C(w') = B$ và $C(w) \neq B$.

Giả sử rằng $q \geq 1$ và $w, w'$ thỏa mãn các giả thiết của (A_q). Có một $s \in S$ sao cho $sw'$ có độ dài $q - 1$. Ta có

$$
l_S(w) > l_S(sw')
$$

do đó $w \neq sw'$. Hơn nữa, $sw \neq sw'$; theo công thức (3) của § 1, no. 1, ta có

$$
l_S(sw) \geq l_S(w) - 1 \geq l_S(sw') = q - 1.
$$

Theo giả thiết quy nạp, $C(sw')$ phân biệt với $C(w)$ và với $C(sw)$; từ công thức (2) suy ra rằng

$$
C(sw') \cap C(s).C(w) = \varnothing.
$$

Vì $C(sw') \subset C(s).C(w')$, cuối cùng ta có $C(w) \neq C(w')$.

#### Nhận xét {#lie-iv-s2-n3-rem-1 .statement}

Tiên đề (T4) đã không được sử dụng trong chứng minh trước đó.

### 4. CÁC QUAN HỆ VỚI CÁC HỆ COXETER

#### Định lý 2 {#lie-iv-s2-thm-2 .statement}

Cặp $(W, S)$ là một hệ Coxeter. Hơn nữa, đối với $s \in S$ và $w \in W$, các quan hệ $C(sw) = C(s).C(w)$ và $l_S(sw) > l_S(w)$ là tương đương.

Với mọi $s \in S$, gọi $P_s$ là tập hợp các phần tử $w \in W$ sao cho
$$
C(s).C(w) = C(sw).
$$
Ta sẽ kiểm tra rằng các $P_s$ thỏa mãn các điều kiện (A'), (B') và (C) của § 1, no. 7; khi đó hai khẳng định của định lý sẽ suy ra từ Mệnh đề 6 của § 1, no. 7.

Điều kiện (A') là rõ ràng.

Ta kiểm tra (B'). Nếu $P_s$ và $sP_s$ có một phần tử $w$ chung, ta sẽ có $w \in P_s$ và $sw \in P_s$, và do đó
$$
C(s).C(w) = C(sw), \qquad C(s).C(sw) = C(w).
$$
Suy ra rằng $C(s).C(s).C(w) = C(w)$ và, theo công thức (5), điều này sẽ kéo theo $C(w) = C(sw)$, điều này mâu thuẫn với Đl. 1.

Ta kiểm tra (C). Cho $s, s' \in S$ và $w, w' \in W$ với $w' = ws'$. Giả thiết rằng $w \in P_s$ và $w' \notin P_s$ kéo theo rằng
$$
C(sw) = C(s).C(w) \tag{9}
$$
$$
C(w') \subset C(s).C(w') \tag{10}
$$
theo (3).

Từ (9) và quan hệ $w = w's'$, suy ra rằng
$$
C(s)w's'B = C(sw). \tag{11}
$$
Theo công thức (2'), $C(w').C(s') \subset C(w') \cup C(w's')$, điều này ngay lập tức kéo theo rằng
$$
C(w')s'B \subset C(ws') \cup C(w). \tag{12}
$$
Vì $C(w')$ là một hợp của các lớp kề trái $gB$ và vì
$$
C(s).C(w') = C(s)w'B,
$$
công thức (10) cho thấy rằng $C(s)w'$ giao với $C(w')$ và *a fortiori* rằng $C(s)w's'B$ giao với $C(w')s'B$. Từ các công thức (11) và (12) suy ra rằng lớp kề kép $C(sw)$ bằng một trong các lớp kề kép $C(ws')$ và $C(w)$; vì $sw \neq w$, Đl. 1 cho phép ta kết luận rằng $sw = ws'$.

#### Hệ quả 1 {#lie-iv-s2-thm-2-cor-1 .statement}

*Cho* $w_1, \ldots, w_q \in W$ *và cho* $w = w_1 \ldots w_q$. *Nếu*
$$
l_S(w) = l_S(w_1) + \cdots + l_S(w_q),
$$
*thì*
$$
C(w) = C(w_1) \ldots C(w_q).
$$

Khi lấy các phân tích thu gọn của các $w_i$, ta quy về trường hợp của một phân tích thu gọn

$$
w = s_1 \ldots s_q, \quad \text{với } s_i \in S.
$$

Nếu $u = s_2 \ldots s_q$, thì $w = s_1 u$ và $l_S(s_1 u) > l_S(u)$, do đó $C(w) = C(s_1).C(u)$ theo định lý. Công thức cần chứng minh suy ra từ điều này bằng quy nạp theo $q$.

#### Hệ quả 2 {#lie-iv-s2-thm-2-cor-2 .statement}

*Cho $w \in W$ và cho $T_w$ là tập con của $W$ liên kết với $w$ bởi thủ tục của Bổ đề 2 của § 1, no. 4. Nếu $t \in T_w$, thì*

$$
C(t) \subset C(w).C(w^{-1}).
$$

Nếu $t \in T_w$, theo định nghĩa tồn tại các phần tử $w', w'' \in W$ và $s \in S$ sao cho

$$
w = w' s w'', \quad l_S(w) = l_S(w') + l_S(w'') + 1 \quad \text{và} \quad t = w' s w'^{-1}.
$$

Theo Hệ quả 1,

$$
C(w).C(w^{-1}) = C(w').C(s).C(w'').C(w''^{-1}).C(s).C(w'^{-1}).
$$

Do đó,

$$
C(w).C(w^{-1}) \supset C(w').C(s).C(s).C(w'^{-1}).
$$

Theo (4), $C(s) \subset C(s).C(s)$. Do đó,

$$
C(w).C(w^{-1}) \supset C(w').C(s).C(w'^{-1}) \supset C(t).
$$

#### Hệ quả 3 {#lie-iv-s2-thm-2-cor-3 .statement}

*Cho $w \in W$ và cho $H_w$ là nhóm con của $G$ sinh bởi $C(w).C(w^{-1})$. Khi đó:*

a) *Với mọi phân tích rút gọn $(s_1, \ldots, s_q)$ của $w$,*

$$
C(s_j) \subset H_w \quad \text{với } 1 \leq j \leq q.
$$

b) *Nhóm $H_w$ chứa $C(w)$ và được sinh bởi $C(w)$.*

Ta chứng minh a) bằng quy nạp theo $j$. Giả sử rằng $C(s_k)$ được chứa trong $H_w$ với $k < j$. Đặt

$$
t = (s_1 \ldots s_{j-1}) s_j (s_1 \ldots s_{j-1})^{-1}.
$$

Phần tử $t$ thuộc tập con $T_w$ của $W$ được định nghĩa trong Bổ đề 2 của § 1, no. 4. Theo Hệ quả 2, $C(t) \subset H_w$, và do đó $C(s_j) \subset H_w$.

Vì $C(w) = C(s_1) \ldots C(s_q)$, xem Hệ quả 1, ta có $C(w) \subset H_w$, và b) suy ra.

#### Ví dụ {#lie-iv-s2-n4-exa-1 .statement}

Định lý 2, được áp dụng cho hệ Tits được mô tả trong no. 2, chỉ ra rằng *nhóm đối xứng* $\mathfrak{S}_n$, với tập các phép chuyển vị của các phần tử liên tiếp, *là một nhóm Coxeter*.

### 5. CÁC NHÓM CON CỦA G CHỨA B

Với mọi tập con X của S, ta ký hiệu bởi W_X nhóm con của W sinh bởi X (xem §1, no. 8) và bởi G_X hợp BW_XB của các lớp kép C(w), w ∈ W_X. Ta có G_∅ = B và G_S = G.

#### Định lý 3 {#lie-iv-s2-thm-3 .statement}

a) Với mọi tập con X của S, tập hợp G_X là một nhóm con của G, sinh bởi $\bigcup_{s \in X} C(s)$.

b) Ánh xạ X ↦ G_X là một song ánh từ $\mathcal{P}(S)$ vào tập hợp các nhóm con của G chứa B.

c) Cho $(X_i)_{i \in I}$ là một họ các tập con của X. Nếu $X = \bigcap_{i \in I} X_i$, thì $G_X = \bigcap_{i \in I} G_{X_i}$.

d) Cho X và Y là hai tập con của S. Khi đó $G_X \subset G_Y$ (tương ứng, $G_X = G_Y$) khi và chỉ khi $X \subset Y$ (tương ứng, $X = Y$).

Hiển nhiên là $G_X = (G_X)^{-1}$; Bổ đề 1 của no. 1 chỉ ra rằng $G_X . G_X \subset G_X$; và do đó a) suy ra, có tính đến Hệ quả 1 của Định lý 2.

Tính đơn ánh của ánh xạ X ↦ G_X suy ra từ tính đơn ánh của ánh xạ X ↦ W_X (§1, no. 8, Định lý 2). Ngược lại, cho H là một nhóm con của G chứa B. Gọi U là tập hợp các $w \in W$ sao cho $C(w) \subset H$. Ta có $H = BUB$ vì H là một hợp của các lớp kép. Đặt $X = U \cap S$; ta chứng minh rằng $H = G_X$. Rõ ràng, $G_X \subset H$. Mặt khác, cho $u \in U$ và $(s_1, \ldots, s_q)$ là một phân tích rút gọn của u. Hệ quả 3 của Định lý 2 suy ra rằng $C(s_j) \subset H$, và do đó $s_j \in X$ với $1 \leq j \leq q$. Vì vậy, $u \in W_X$, và vì H là hợp của các $C(u)$ với $u \in U$, ta có $H \subset G_X$, điều này chứng minh b).

Các khẳng định c) và d) suy ra từ các tính chất tương tự của W_X (§ 1, no. 8, Định lý 2).

#### Hệ quả {#lie-iv-s2-n5-cor-1 .statement}

Tập hợp S gồm các phần tử $w \in W$ sao cho $w \neq 1$ và $B \cup C(w)$ là một nhóm con của G.

Các phần tử $w \in W$ sao cho $B \cup C(w)$ là một nhóm con của G là các phần tử mà tồn tại $X \subset S$ với $W_X = \{1, w\}$. Hơn nữa, nếu $w \neq 1$, ta tất yếu có Card(X) = 1 , nghĩa là $w \in S$.

#### Nhận xét 1 {#lie-iv-s2-n5-rem-1 .statement}

Hệ quả trên cho thấy S được xác định bởi (G, B, N); vì lý do này, đôi khi ta cho phép mình nói rằng (G, B, N) là một hệ Tits, hoặc rằng (B, N) là một hệ Tits trong G.

#### Mệnh đề 1 {#lie-iv-s2-prop-1 .statement}

Cho X là một tập con của S và N' là một nhóm con của N có ảnh trong W bằng W_X. Khi đó, (G_X, B, N', X) là một hệ Tits.

Ta có $G_X = BW_XB = BN'B$, điều này cho thấy rằng $G_X$ được sinh bởi $B \cup N'$. Việc kiểm tra các tiên đề (T1) đến (T4) là ngay lập tức.

#### Mệnh đề 2 {#lie-iv-s2-prop-2 .statement}

Cho X, Y ⊂ S và $w \in W$. Ta có

$$
G_X w G_Y = BW_X w W_Y B.
$$

Cho $s_1, \ldots, s_q \in X$ và $t_1, \ldots, t_q \in Y$. Bổ đề 1 cho thấy rằng
$$
C(s_1 \ldots s_q).C(w).C(t_1 \ldots t_q) \subset BW_X w W_Y B,
$$
và do đó
$$
G_X w G_Y \subset BW_X w W_Y B.
$$
Bao hàm ngược lại là hiển nhiên.

#### Nhận xét 2 {#lie-iv-s2-n5-rem-2 .statement}

Ký hiệu $G_X \backslash G / G_Y$ là tập hợp các tập con của G có dạng $G_X g G_Y$, $g \in G$; và định nghĩa $W_X \backslash W / W_Y$ tương tự. Mệnh đề trước cho thấy rằng song ánh chính tắc $w \mapsto C(w)$ từ $W$ đến $B \backslash G / B$ xác định qua phép lấy thương một *song ánh* $W_X \backslash W / W_Y \to G_X \backslash G / G_Y$.

#### Mệnh đề 3 {#lie-iv-s2-prop-3 .statement}

*Cho $X \subset S$ và $g \in G$. Quan hệ $g B g^{-1} \subset G_X$ kéo theo rằng $g \in G_X$.*

Cho $w \in W$ sao cho $g \in C(w)$. Vì $B$ là một nhóm con của $G_X$, giả thiết $g B g^{-1} \subset G_X$ kéo theo rằng $C(w).C(w^{-1}) \subset G_X$, và do đó $C(w) \subset G_X$ theo Hệ quả 3 của Định lý 2, vậy nên $g$ thuộc về $G_X$.

### 6. CÁC NHÓM CON PARABOLIC

#### Định nghĩa 2 {#lie-iv-s2-def-2 .statement}

*Một nhóm con của $G$ được gọi là parabolic nếu nó chứa một liên hợp của $B$.*

Rõ ràng rằng mọi nhóm con chứa một nhóm con parabolic đều là parabolic.

#### Mệnh đề 4 {#lie-iv-s2-prop-4 .statement}

*Cho $P$ là một nhóm con của $G$.*

a) *$P$ là parabolic khi và chỉ khi tồn tại một tập con $X$ của $S$ sao cho $P$ liên hợp với $G_X$ (xem no. 5 về định nghĩa của $G_X$).*

b) *Cho $X, X' \subset S$ và $g, g' \in G$ sao cho $P = g G_X g^{-1} = g' G_{X'} g'^{-1}$. Khi đó, $X = X'$ và $g' g^{-1} \in P$.*

Mệnh đề a) suy ra từ Đl. 3, b).
Dưới các giả thiết của b), ta có
$$
g^{-1} g' B g'^{-1} g \subset g^{-1} g' G_{X'} g'^{-1} = G_X,
$$
và Mđ. 3 chỉ ra rằng $g^{-1} g' \in G_X$. Do đó, $G_{X'} = G_X$ và $X' = X$ theo Đl. 3, b). Cuối cùng,
$$
g' g^{-1} = g . g^{-1} g' . g^{-1} \in g G_X g^{-1},
$$
điều này chứng minh b).

Nếu nhóm con parabolic $P$ liên hợp với $G_X$, trong đó $X \subset S$, thì $P$ được gọi là có *kiểu X*.

#### Định lý 4 {#lie-iv-s2-thm-4 .statement}

(i) Cho $P_1$ và $P_2$ là hai nhóm con parabolic của $G$ mà giao của chúng là parabolic và cho $g \in G$ sao cho $gP_1g^{-1} \subset P_2$. Khi đó $g \in P_2$ và $P_1 \subset P_2$.

(ii) Hai nhóm con parabolic có giao là parabolic thì không liên hợp.

(iii) Cho $Q_1$ và $Q_2$ là hai nhóm con parabolic của $G$ được chứa trong một nhóm con $Q$ của $G$. Khi đó mọi $g \in G$ sao cho $gQ_1g^{-1} = Q_2$ đều thuộc $Q$.

(iv) Mọi nhóm con parabolic đều là nhóm chuẩn hoá của chính nó$^6$.

Mệnh đề (i) suy ra từ các Mđ. 3 và 4, và kéo theo (ii). Dưới các giả thiết của (iii), ta có $gQ_1g^{-1} \subset Q$, điều này suy ra $g \in Q$ theo (i). Cuối cùng, (iv) suy ra từ (iii) bằng cách lấy $Q_1 = Q_2 = Q$.

#### Mệnh đề 5 {#lie-iv-s2-prop-5 .statement}

Cho $P_1$ và $P_2$ là hai nhóm con parabolic của $G$. Khi đó $P_1 \cap P_2$ chứa một liên hợp của $T$.

Bằng cách trước hết biến đổi $P_1$ và $P_2$ bởi một tự đẳng cấu trong của $G$, ta có thể giả sử rằng $B \subset P_1$. Cho $g \in G$ sao cho $gB_2g^{-1} \subset P_2$. Theo Đl. 1, tồn tại $n \in N$ và $b, b' \in B$ sao cho $g = bn b'$. Vì $T$ là chuẩn trong $N$,

$$
P_2 \supset gB_2g^{-1} = bnBn^{-1}b^{-1} \supset bnTn^{-1}b^{-1} = bTb^{-1}
$$

và

$$
P_1 \supset B \supset bTb^{-1},
$$

điều này chứng minh mệnh đề.

### 7. CÁC ĐỊNH LÝ VỀ TÍNH ĐƠN

#### Bổ đề 2 {#lie-iv-s2-lem-2 .statement}

Cho $H$ là một nhóm con chuẩn tắc của $G$. Tồn tại một tập con $X$ của $S$ sao cho $BH = G_X$ và sao cho mọi phần tử của $X$ giao hoán với mọi phần tử của $S - X$.

Vì $BH$ là một nhóm con của $G$ chứa $B$, tồn tại duy nhất một tập con $X$ của $S$ sao cho $BH = G_X$ (Đl. 3).

Cho $s_1 \in X$ và $s_2 \in S - X$; gọi $n_1$ và $n_2$ lần lượt là các đại diện trong $N$ của $s_1$ và $s_2$. Khi đó $n_1 \in G_X = BH$ và tồn tại $b \in B$ sao cho $bn_1 \in H$. Vì $H$ là chuẩn tắc trong $G$, phần tử $h = n_2 b n_1 n_2^{-1}$ của $G$ thuộc $H$. Điều này có nghĩa là

$$
h \in C(s_2).C(s_1).C(s_2).
$$

Nếu độ dài của $s_2 s_1 s_2$ bằng 3, Hệ quả 1 của Đl. 2 suy ra rằng

$$
C(s_2).C(s_1).C(s_2) = C(s_2 s_1 s_2),
$$

\footnotetext{6}{Nếu $H$ là một nhóm con của một nhóm $G$, chuẩn hoá tử của $H$ trong $G$ là nhóm con $\mathfrak{N}(H)$ gồm các phần tử $g$ của $G$ sao cho $gHg^{-1} = H$. Một nhóm con $H'$ được gọi là chuẩn hoá $H$ nếu $H' \subset \mathfrak{N}(H)$, trong trường hợp đó $HH' = H'H$ là một nhóm con của $G$ trong đó $H$ là chuẩn tắc.}

và do đó $h \in H \cap C(s_2 s_1 s_2)$. Vì $H \cap C(s_2 s_1 s_2)$ là không rỗng, $s_2 s_1 s_2 \in W_X$. Vì $(s_2, s_1, s_2)$ là một phân tích rút gọn, suy ra $s_2 \in X$, trái với giả thiết của ta.

Do đó $l_S(s_2 s_1 s_2) \leq 2$; nếu $l_S(s_2 s_1 s_2) = 1$, thì $s_1 s_2 \in S$ và do đó $(s_1 s_2)^2 = 1$, hay $s_1 s_2 = s_2 s_1$. Nếu $l_S(s_2 s_1 s_2) = 2$, tính chất (E) của §1, no. 5 suy ra rằng $s_2 s_1 = s_1 s_2$, vì $s_1 \neq s_2$. Q.E.D.

Tính chất sau đây của một nhóm U được sử dụng trong Đl. 5 dưới đây:

(R) *Đối với mọi nhóm con chuẩn tắc V của U phân biệt với U, nhóm giao hoán tử* (xem *Đại số*, Chương I, §6, no. 8) *của U/V là phân biệt với U/V*.

Mọi nhóm giải được đều thỏa mãn (R); đặc biệt, mọi nhóm Abel đều thỏa mãn (R). Có thể chỉ ra rằng nhóm đối xứng $\mathfrak{S}_n$ thỏa mãn (R) (xem Bài tập 29).

#### Định lý 5 {#lie-iv-s2-thm-5 .statement}

*Gọi Z là giao của các liên hợp của B, gọi U là một nhóm con của B và gọi G_1 là nhóm con sinh bởi các liên hợp của U trong G. Ta đặt các giả thiết sau:*

(1) *U là chuẩn tắc trong B và B = UT*.
(2) *U có tính chất (R)*.
(3) *G_1 bằng nhóm giao hoán tử của nó*.
(4) *Hệ Coxeter (W, S) là bất khả quy* (xem §1, no. 9).

*Khi đó mọi nhóm con H của G được G_1 chuẩn hoá hoặc được chứa trong Z hoặc chứa G_1*.

*Trước hết ta chứng minh rằng $G = G_1 T$*. Nhóm $G_1 T$ chứa B và do đó là chuẩn hoá tử của chính nó (Đl. 4); nhưng vì N chuẩn hoá $G_1$ và T, nó cũng chuẩn hoá $G_1 T$, vậy $N \subset G_1 T$. Vì G được sinh bởi B và N, suy ra $G = G_1 T$.

*Tiếp theo, đặt*

$$
G' = G_1 H, \quad B' = B \cap G', \quad N' = N \cap G',
T' = T \cap G' = B' \cap N' \quad \text{và} \quad W' = N'/T'.
$$

Ta có $G = G'T$ vì $G'$ chứa $G_1$, và do đó $N = N'T$. Việc nhúng $N'$ vào N khi đó xác định, chuyển qua thương, một đẳng cấu $\alpha : W' \to W$. Đặt $S' = \alpha^{-1}(S)$.

*Bây giờ ta chứng minh rằng (G', B', N', S') là một hệ Tits*. Vì $G = BNB$ và $B = TU = UT$, ta có $G = UNU$. Vì U là một nhóm con của $G'$, suy ra $G' = UN'U$; vì $U \subset B'$, điều này chứng minh (T1). Tiên đề (T2) được thoả mãn vì $\alpha$ là một đẳng cấu. Cho $w \in W$ và đặt $w' = \alpha^{-1}(w)$ là phần tử tương ứng của $W'$. Ta có

$$
BwB = BwB' = Bw'B', \quad \text{since } B = B'T.
$$

Từ đó ta kết luận rằng $G' \cap BwB = B'w'B'$, nghĩa là việc nhúng $G'$ vào G xác định, khi chuyển qua thương, một song ánh từ

B'\setminus G'/B' đến B\setminus G/B. Tiên đề (T3) được suy ra ngay lập tức. Tiên đề (T4) suy ra từ B = B'T.

Nhóm con H là chuẩn tắc trong G'. Áp dụng Bổ đề 2 cho (G', B', N', S'), tồn tại một tập con X' của S' sao cho B'H = G'_X', và mọi phần tử của S' - X' giao hoán với mọi phần tử của X'. Theo giả thiết (4), chỉ có hai khả năng:

a) X' = $\varnothing$, tức là B'H = B', do đó H $\subset B' \subset B$. Nếu $g \in G$, thì $g = g_1 t$ với $g_1 \in G_1$, $t \in T$, và H $\subset g_1 B g_1^{-1}$ vì G_1 chuẩn hoá H. Vậy H $\subset g B g^{-1}$, và vì Z là giao của các $g B g^{-1}$, ta có H $\subset Z$.

b) X' = S', tức là B'H = G'. Vì $G = G'T$, ta có

$$ G = B'HT = HB'T = HB. $$

Vì B chuẩn hoá U, mọi liên hợp của U có dạng $hUh^{-1}$ với $h \in H$. Nhóm con như vậy được chứa trong nhóm UH, do đó $G_1 \subset UH$ theo định nghĩa của G_1. Vì vậy, ta có các đẳng cấu

$$ U/(U \cap H) \cong UH/H = G_1 H/H \cong G_1/(G_1 \cap H). $$

Theo giả thiết (3), $G_1/(G_1 \cap H)$ bằng nhóm giao hoán tử của nó. Giả thiết (2) nay chỉ ra rằng nhóm $U/(U \cap H)$, đẳng cấu với $G_1/(G_1 \cap H)$, thu gọn về phần tử đơn vị. Do đó $G_1 \cap H = G_1$ và $G_1 \subset H$, điều này hoàn tất chứng minh.

#### Hệ quả {#lie-iv-s2-n7-cor-1 .statement}

Dưới các giả thiết của Đl. 5, nhóm $G_1/(G_1 \cap Z)$ hoặc là đơn không Abel hoặc thu gọn về phần tử đơn vị.

Đl. 5 chỉ ra rằng $G_1/(G_1 \cap Z)$ là đơn hoặc thu gọn về phần tử đơn vị. Mặt khác, giả thiết (3) kéo theo rằng nó bằng nhóm giao hoán tử của nó. Suy ra hệ quả.

#### Nhận xét 1 {#lie-iv-s2-n7-rem-1 .statement}

Các giả thiết (2), (3), (4) không được dùng trong chứng minh rằng (G', B', N', S') là một hệ Tits.

#### Nhận xét 2 {#lie-iv-s2-n7-rem-2 .statement}

Giả sử rằng $Z \cap U = \{1\}$. Vì Z và U là chuẩn tắc trong B, suy ra mọi phần tử của Z giao hoán với mọi phần tử của U, và do đó với mọi phần tử của G_1. Theo hệ quả trước đó, suy ra $G_1 \cap Z$ là tâm của G_1.

#### Nhận xét 3 {#lie-iv-s2-n7-rem-3 .statement}

Giả thiết (3) được kéo theo bởi điều kiện sau:

(3') U được sinh bởi các giao hoán tử $b^{-1} u^{-1} b u$ với $u \in U$ và $b \in B \cap G_1$.

#### Ví dụ 1 {#lie-iv-s2-n7-exa-1 .statement}

Cho k là một trường, n là một số nguyên $\geqslant 0$, $G = \mathbf{GL}(n, k)$, và cho (G, B, N, S) là hệ Tits được mô tả trong no. 2. Cho U là nhóm con tam giác trên ngặt của G, tức là nhóm con của B gồm các ma trận có các phần tử đường chéo bằng 1. Điều kiện (1) trong Đl. 5 là ngay lập tức, và (2) cũng vậy vì U là giải được. Điều kiện (4) được thoả mãn nếu $n \geq 2$. Có thể chứng minh (xem *Algebra*, Ch. II, § 10, Bài tập 13) rằng (3) được thoả mãn nếu $n \geq 3$ và Card$(k) \geq 4$. Dưới các điều kiện này, ta kết luận rằng $G_1 / (G_1 \cap Z)$ là *đơn* và $G_1 \cap Z$ là tâm của $G_1$ (xem *Nhận xét* 2).

Khi $k$ là giao hoán, $G_1 = \mathbf{SL}(n, k)$ (xem *Algebra*, Ch. III, § 8, no. 9).

#### Ví dụ 2 {#lie-iv-s2-n7-exa-2 .statement}

Cho $g$ là một đại số Lie đơn trên $\mathbf{C}$, và cho $G$ là nhóm các tự đẳng cấu nội của $g$ (xem Ch. III, § 6, no. 2, Mệnh đề 2). Bằng cách sử dụng Đl. 5, ta có thể chứng minh rằng $G$ là đơn không Abel.

### Các bài tập {#lie-iv-s2-exercises}

Xem [các bài tập cho § 2](exercises/s2/).
