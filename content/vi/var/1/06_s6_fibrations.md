---
book: var
book_title: Variétés différentielles et analytiques
chapter: "1"
chapter_title: VARIÉTÉS DIFFÉRENTIELLES ET ANALYTIQUES, FASCICULE DE RÉSULTATS
section: 6
section_title: Fibrations
lang: vi
source: var-fr
pdf_pages: 0059-0067
extraction: ocr
subsections:
    - "no": 1
      title: Fibrations
      page: 0
      pdf_page: 59
    - "no": 2
      title: Fibrations principales
      page: 0
      pdf_page: 60
    - "no": 3
      title: Morphismes de fibrations principales
      page: 0
      pdf_page: 61
    - "no": 4
      title: Construction de fibrations principales au moyen de cocycles
      page: 0
      pdf_page: 63
    - "no": 5
      title: Espaces fibrés associés à une fibration principale
      page: 0
      pdf_page: 64
    - "no": 6
      title: Extension et restriction du groupe structural
      page: 0
      pdf_page: 66
    - "no": 7
      title: Changements de structure
      page: 0
      pdf_page: 67
statements: 0
exercises: 0
content_sha256: 205dedafd27b46ce5ab35aae53d3901246bce458780b5a48ccc6ed4ba822f845
translated_from: content/en-mt/var/1/06_s6_fibrations.md
source_lang: en-mt
translation_method: machine
source_content_sha256: a242e363f8011bc48188d01d98463e2608dfef2f362a989490fe9ffa9cfa9701
translation_model: gpt-5-6-mini, gpt-5-6
translation_run: translate-vi-2e38b3d8
glossary_version: 34
glossary_terms_sha256: d8c4ac4fc6f0578c385be8563337f17a7eeb6feed3b9f8e8f4bc5ca129324f4b
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 6. Phân thớ¹

### 6.1. Phân thớ

6.1.1. Một phân thớ lớp $C'$, hay đơn giản là một phân thớ, được gọi là một bộ ba $(X, B, \pi)$ trong đó $B$ và $X$ là các đa tạp lớp $C'$ và $\pi$ là một cấu xạ từ $X$ vào $B$, có tính chất sau:

(F) Với mọi $x \in B$, tồn tại một lân cận mở $U$ của $x$, một đa tạp $F$, và một đẳng cấu $\varphi$ của $\pi^{-1}(U)$ lên $U \times F$ sao cho $\pi(\varphi^{-1}(x, y)) = x$ với mọi $x \in U$ và mọi $y \in F$.

Nếu $\lambda = (X, B, \pi)$ là một phân thớ, $X$ được gọi là không gian của $\lambda$, $B$ là cơ sở của $\lambda$, và $\pi$ là phép chiếu của $\lambda$. Ánh xạ $\pi$ là một phép chìm; đặc biệt $\pi(X)$ là mở trong $B$, và nếu $R$ biểu thị quan hệ tương đương được xác định bởi $\pi$ trong $X$, ánh xạ chính tắc của $X/R$ vào $\pi(X)$ là một đẳng cấu. Với mọi $x \in B$, ảnh ngược $\pi^{-1}(x)$ là một đa tạp con đóng của $X$, được gọi là thớ của $x$, và được ký hiệu là $X_x$.

6.1.2. Ví dụ:
(a) Nếu $B$ và $F$ là hai đa tạp, bộ ba $(B \times F, B, pr_1)$ là một phân thớ mà các thớ của nó một cách chính tắc đẳng cấu với $F$.
(b) Nếu $\lambda = (X, B, \pi)$ và $\lambda' = (X', B', \pi')$ là các phân thớ,
$$
\lambda \times \lambda' = (X \times X', B \times B', \pi \times \pi')
$$
là một phân thớ; nó được gọi là tích của $\lambda$ và của $\lambda'$.
(c) Nếu $\lambda = (X, B, \pi)$ và $\lambda' = (X', B, \pi')$ là các phân thớ có cùng cơ sở, $\lambda \times_B \lambda' = (X \times_B X', B, \pi \times_B \pi')$ là một phân thớ; nó được gọi là tích của $\lambda$ và của $\lambda'$ trên $B$, hoặc còn gọi là tích phân thớ của $\lambda$ và của $\lambda'$.

6.1.3. Cho $\lambda = (X, B, \pi)$ và $\lambda' = (X', B', \pi')$ là hai phân thớ. Một cấu xạ của $\lambda$ vào $\lambda'$ được gọi là một cặp bất kỳ $(f, g)$, trong đó $f$ là một cấu xạ của $B$ vào $B'$, và $g$ là một cấu xạ của $X$ vào $X'$, sao cho $\pi' \circ g = f \circ \pi$. Khi $B = B'$ và $f = \mathrm{Id}_B$, người ta nói rằng $g$ là một cấu xạ $B$ của $\lambda$ vào $\lambda'$; nếu $g$ là một đẳng cấu của $X$ lên $X'$, thì $g^{-1}$ là một cấu xạ $B$ của $\lambda'$ vào $\lambda$, và người ta nói rằng $g$ là một đẳng cấu $B$ của $\lambda$ lên $\lambda'$; để điều này xảy ra, điều kiện cần và đủ là, với mọi $x \in B$, ánh xạ $g_x : X_x \to X'_x$ cảm sinh bởi $g$ là một đẳng cấu.

¹ Các định nghĩa và phần lớn các kết quả của §§ 6 và 7 cũng áp dụng cho phạm trù các không gian tôpô; khi đó ta phải thay thế các từ « đa tạp », « đa tạp con », « cấu xạ » và « đa tạp nhóm » bằng « không gian tôpô », « không gian con tôpô », « ánh xạ liên tục » và « nhóm tôpô ». Các ngoại lệ là các kết quả liên quan đến các phép nhúng, các phép phân thớ con, và các quan hệ tương đương chính quy, cũng như các kết quả của No. 6.2.3 và 6.2.4 (a).

6.1.4. Phân thớ $(B \times F, B, pr_1)$ được gọi là phân thớ *tầm thường* có cơ sở $B$ và thớ $F$. Một đẳng cấu của một phân thớ $\lambda$ lên một phân thớ tầm thường được gọi là một *sự tầm thường hóa* của $\lambda$.

6.1.5. Cho $\lambda = (X, B, \pi)$ là một phân thớ, và cho $f : B' \to B$ là một cấu xạ. Gọi $\pi'$ là cấu xạ chính tắc từ $B' \times_B X$ vào $B'$. Bộ ba $(B' \times_B X, B', \pi')$ là một phân thớ, được gọi là *ảnh ngược của $\lambda$ bởi $f'$* hoặc phân thớ suy ra từ $\lambda$ bằng thay đổi cơ sở từ $B$ sang $B'$ theo $f$, và được ký hiệu bởi $B' \times_B \lambda$, hoặc cũng bởi $f^*\lambda$. Nếu $f'$ ký hiệu ánh xạ chính tắc từ $B' \times_B X$ vào $X$, thì cặp $(f, f')$ là một *cấu xạ* từ $B' \times_B \lambda$ vào $\lambda$; nó có tính chất phổ quát sau: nếu $(f, g)$ là một cấu xạ từ một phân thớ $\lambda'$ với cơ sở $B'$ vào phân thớ $\lambda$, thì tồn tại một cấu xạ-$B'$ duy nhất $\varphi : \lambda' \to B' \times_B \lambda$ sao cho $(f, g) = (f, f') \circ \varphi$.

Khi $B'$ là một đa tạp con của $B$, và $f$ là đơn ánh chính tắc của $B'$ vào $B$, $B' \times_B X$ được đồng nhất với đa tạp con $\pi^{-1}(B')$ của $X$, và $\pi'$ được đồng nhất với hạn chế của $\pi$ vào $\pi^{-1}(B')$; ảnh ngược của $\lambda$ bởi $f$ khi đó được gọi là *phân thớ cảm sinh bởi $\lambda$ trên $B'$*.

6.1.6. Nếu $\lambda = (X, B, \pi)$ là một phân thớ, người ta gọi *tiết diện cấu xạ* (hay đơn giản là *tiết diện*) của $\lambda$ là mọi cấu xạ $s : B \to X$ sao cho $\pi \circ s = \mathrm{Id}_B$.

### 6.2. Các phân thớ chính

6.2.1. Cho $B$ là một đa tạp và $G$ là một đa tạp nhóm. Người ta gọi *một phân thớ chính với cơ sở $B$ và nhóm cấu trúc $G$* là một bộ bốn $\lambda = (P, G, B, \pi)$ trong đó $P$ là một đa tạp mà trên đó $G$ tác động phải bởi $(x, g) \mapsto x . g$ (xem n° 5.12.5), và trong đó $\pi$ là một cấu xạ từ $P$ vào $B$, các dữ kiện này thỏa mãn tiên đề sau:

(P) Với mọi $b \in B$ tồn tại một lân cận mở $U$ của $b$ và một đẳng cấu $f : U \times G \to \pi^{-1}(U)$ sao cho ta có

$$
\pi(f(u, g)) = u \text{ và } f(u, gg') = f(u, g) \cdot g' \text{ nếu } u \in U \text{ và } g, g' \in G.
$$

6.2.2. Cho $\lambda = (P, G, B, \pi)$ là một phân thớ chính. Bộ ba $(P, B, \pi)$ là một phân thớ; ta có $\pi(P) = B$. Quan hệ tương đương $R$ được xác định bởi $\pi$ trong $P$ trùng với quan hệ được xác định bởi $G$; đồ thị của nó không gì khác ngoài tích $P \times_B P$ (xem No. 5.11.2); nó là một đa tạp con của $P \times P$. Ánh xạ $(x, g) \mapsto (x, x . g)$ là một đẳng cấu của $P \times G$ lên $P \times_B P$; ánh xạ tương ứng với mỗi $(x, y) \in P \times_B P$ phần tử duy nhất $g \in G$ sao cho $y = x . g$ là một cấu xạ của $P \times_B P$ vào $G$.

Nhóm $G$ tác động *chính quy và tự do* lên $P$ (xem Top. Gén., chap. III, 3e éd., § 4). Nếu $x \in P$ và nếu $b = \pi(x)$, ánh xạ $g \mapsto x . g$ là một *đẳng cấu của đa tạp $G$ lên thớ của $b$*.

6.2.3. Ngược lại, cho $G$ là một đa tạp nhóm, và cho $P$ là một đa tạp trên đó $G$ tác động bên phải sao cho thỏa mãn hai điều kiện sau:
(a) $G$ tác động chính quy và tự do lên $P$.
(b) Với mọi $x \in P$, ánh xạ $g \mapsto x . g$ là một phép nhúng của $G$ vào $P$.

Khi đó quan hệ tương đương được xác định bởi $G$ trong $P$ là chính quy; nếu ký hiệu $P/G$ là đa tạp thương, và $\pi$ là phép chiếu chính tắc của $P$ lên $P/G$, thì bộ bốn $(P, G, P/G, \pi)$ là một phân thớ chính.
Khi $K$ có đặc số 0 và $P$ là hữu hạn chiều, điều kiện (b) ở trên là một hệ quả của điều kiện (a).

6.2.4. Các điều kiện của No. trước được thỏa mãn trong hai trường hợp sau:
(a) $P$ là một đa tạp nhóm và $G$ là một đa tạp con nhóm tác động lên $P$ bằng các phép tịnh tiến phải; cơ sở của phân thớ chính thu được như vậy là không gian thuần nhất $P/G$.
(b) $G$ là một nhóm rời rạc tác động chính quy và tự do lên $P$. Phép chiếu $\pi : P \to P/G$ khi đó là một cấu xạ étale (No. 5.7.6).

6.2.5. Các ví dụ:
(a) Cho $B$ là một đa tạp và cho $G$ là một đa tạp nhóm. Cho $G$ tác động lên $B \times G$ bởi $(b, g) . g' = (b, gg')$. Bộ bốn $(B \times G, G, B, \mathrm{pr}_1)$ là một fibration chính.
(b) Cho $\lambda = (P, G, B, \pi)$ và $\lambda' = (P', G', B', \pi')$ là hai fibration chính. Cho $G \times G'$ tác động lên $P \times P'$ bởi công thức:
$$
(x, x') . (g, g') = (x.g, x'.g'), \quad x \in P, x' \in P', g \in G, g' \in G'.
$$
Bộ bốn $\lambda \times \lambda' = (P \times P', G \times G', B \times B', \pi \times \pi')$ là một fibration chính; nó được gọi là tích của $\lambda$ và $\lambda'$.
(c) Cho $\lambda = (P, G, B, \pi)$ và $\lambda' = (P', G', B, \pi')$ là hai fibration chính có cùng cơ sở. Đa tạp con $P \times_B P'$ của $P \times P'$ là ổn định dưới các phép toán của $G \times G'$, và bộ bốn
$$
\lambda \times_B \lambda' = (P \times_B P', G \times G', B, \pi \times_B \pi')
$$
là một fibration chính; nó được gọi là tích của $\lambda$ và $\lambda'$ trên $B$, hoặc còn gọi là tích phân thớ của $\lambda$ và $\lambda'$.

### 6.3. Các cấu xạ của các fibration chính

6.3.1. Cho $\lambda = (P, G, B, \pi)$ và $\lambda' = (P', G', B', \pi')$ là hai fibration chính. Một cấu xạ của $\lambda$ vào $\lambda'$ được gọi là mọi bộ ba $(f, \varphi, h)$, trong đó $f : P \to P'$ và $h : B \to B'$ là các cấu xạ, $\varphi : G \to G'$ là một đồng cấu của các đa tạp nhóm, và trong đó $\pi' \circ f = h \circ \pi$ và $f(x . g) = f(x) . \varphi(g)$ với $x \in P, g \in G$. Ta chú ý rằng $f$ xác định $h$; người ta thường nói rằng $(f, \varphi)$, hoặc thậm chí đơn giản là $f$, là một cấu xạ.

Khi $B = B'$ và $h = \mathrm{Id}_B$ (tương ứng khi $G = G'$ và $\varphi = \mathrm{Id}_G$), một cấu xạ được gọi là một cấu xạ $B$ tương thích với $\varphi$ (tương ứng một cấu xạ $G$ tương thích với $h$). Một cấu xạ đồng thời là một cấu xạ $B$ và một cấu xạ $G$ được gọi là một cấu xạ $G$-$B$ (ở đây một lần nữa, người ta thường chỉ nói đơn giản là “cấu xạ” khi không thể có sự nhầm lẫn). Mọi cấu xạ $G$-$B$ $f : P \to P'$ là một đẳng cấu của đa tạp $P$ lên đa tạp $P'$; đẳng cấu nghịch đảo $f^{-1}$ là một cấu xạ $G$-$B$: $f$ là một đẳng cấu $G$-$B$ của $P$ lên $P'$.

Hai không gian sợi chính $P$ và $P'$ có cùng cơ sở $B$ và cùng nhóm cấu trúc $G$ được gọi là $G$-$B$-đẳng cấu (hoặc đơn giản là đẳng cấu) nếu tồn tại một đẳng cấu $G$-$B$ của $P$ lên $P'$.

6.3.2. Phân thớ chính $(B \times G, G, B, \mathrm{pr}_1)$ được gọi là phân thớ chính *tầm thường* với cơ sở $B$ và nhóm cấu trúc $G$. Một đẳng cấu của một phân thớ chính $\lambda = (P, G, B, \pi)$ lên phân thớ chính tầm thường với cơ sở $B$ và nhóm cấu trúc $G$ được gọi là một *sự tầm thường hóa* của $\lambda$. Mọi tiết diện $s$ của $\lambda$ xác định một sự tầm thường hóa $f_s$ của $\lambda$ bởi công thức:

$$
f_s^{-1}(b, g) = s(b) \cdot g \quad \text{cho } b \in B \text{ và } g \in G.
$$

Do đó thu được một *song ánh từ tập hợp các tiết diện của $\lambda$ lên tập hợp các sự tầm thường hóa của $\lambda$*. Hơn nữa, nếu $s_0$ là một tiết diện của $\lambda$, mọi tiết diện $s$ của $\lambda$ có thể được viết duy nhất dưới dạng $s(b) = s_0(b) \cdot r(b)$, trong đó $r : B \to G$ là một cấu xạ.

6.3.3. Cho $\lambda = (P, G, B, \pi)$ là một phân thớ chính, và cho $h : B' \to B$ là một cấu xạ. Gọi $\pi'$ (tương ứng $h'$) là cấu xạ chính tắc từ $B' \times_B P$ vào $B'$ (tương ứng vào $P$). Cho $G$ tác động lên $B' \times_B P$ bởi công thức

$$
(b', x) \cdot g = (b', x \cdot g), \quad (b', x) \in B' \times_B P, \quad g \in G.
$$

Bộ bốn $(B' \times_B P, G, B', \pi')$ là một phân thớ chính, được gọi là *ảnh ngược* của $\lambda$ bởi $h$, và được ký hiệu bởi $B' \times_B \lambda$ hoặc cũng bởi $h^* \lambda$. Ánh xạ $h' : B' \times_B P \to P$ là một $G$-cấu xạ tương thích với $h$; nó có tính chất phổ quát sau: nếu $f$ là một $G$-cấu xạ tương thích với $h$ từ một phân thớ chính $\lambda'$ có cơ sở $B'$ vào phân thớ $\lambda$, thì tồn tại duy nhất một $G$-$B'$-đẳng cấu $k : \lambda' \to B' \times_B \lambda$ sao cho $f = h' \circ k$.

Khi $B'$ là một đa tạp con của $B$, và $h$ là đơn ánh chính tắc của $B'$ vào $B$, $B' \times_B P$ được đồng nhất với đa tạp con $\pi^{-1}(B')$ của $P$; nó được gọi là *không gian phân thớ chính cảm sinh bởi $P$ trên $B'$*, và được ký hiệu bởi $\pi^{-1}(B')$, hoặc cũng bởi $P|B'$. Mỗi $x \in V$ có một lân cận mở $U$ sao cho $P|U$ là tầm thường.

### 6.4. Phép dựng các phân thớ chính bằng các cocycle

Cho B là một đa tạp, G là một đa tạp nhóm và cho $\mathcal{U} = (U_i)_{i \in I}$ là một phủ mở của B.

6.4.1. Một xiclu lớp $C^r$ trên B với các giá trị trong G, phụ thuộc vào $\mathcal{U}$, được gọi là một họ $(g_{i,j})_{(i,j) \in I \times I}$ có hai tính chất sau:
(1) với mọi cặp $(i,j) \in I \times I$, $g_{i,j}$ là một ánh xạ lớp $C^r$ từ tập mở $U_i \cap U_j$ của B vào G;
(2) với mọi bộ ba $(i,j,k) \in I^3$, ta có
$$
g_{i,k}(x) = g_{i,j}(x) \cdot g_{j,k}(x) \quad \text{với mọi } x \in U_i \cap U_j \cap U_k.
$$
Hai xiclu như vậy $(g_{i,j})$ và $(g'_{i,j})$ được gọi là đồng điều nếu tồn tại một họ $(h_i)_{i \in I}$ sao cho, với mọi $i \in I$, $h_i$ là một ánh xạ lớp $C^r$ từ $U_i$ vào G, thỏa mãn:
(3)
$$
g'_{i,j}(x) = h_i(x)^{-1} \cdot g_{i,j}(x) \cdot h_j(x) \quad \text{với mọi } x \in U_i \cap U_j.
$$

6.4.2. Cho $\lambda = (P, G, B, \pi)$ là một phân thớ chính. Ta cho trước, với mỗi $i \in I$, một tiết diện $s_i$ của $\lambda$ trên $U_i$ (6.3.3). Với mỗi cặp $(i,j) \in I^2$, khi đó tồn tại duy nhất một cấu xạ $g_{i,j}$ từ $U_i \cap U_j$ vào G sao cho:
(4)
$$
s_j(b) = s_i(b) \cdot g_{i,j}(b) \quad \text{với mọi } b \in U_i \cap U_j.
$$
Họ các $g_{i,j}$ là một xiclu trên B với các giá trị trong G, phụ thuộc vào phủ mở $\mathcal{U}$. Xiclu này được gọi là liên kết với đối tượng $(\lambda, \mathcal{U}, (s_i)_{i \in I})$ và các ánh xạ $g_{i,j}$ được gọi là các hàm chuyển của đối tượng này.
Với $i \in I$, gọi $x \mapsto (\pi(x), f_i(x))$ là phép tầm thường hóa được xác định bởi tiết diện $s_i$ của $\lambda|U_i$ (6.3.2). Với $x \in \pi^{-1}(U_i \cap U_j)$, ta có:
(5)
$$
f_i(x) = g_{i,j}(\pi(x)) \cdot f_j(x).
$$

6.4.3. Ngược lại, cho $g = (g_{i,j})$ là một xiclu trên B với các giá trị trong G, phụ thuộc vào phủ $\mathcal{U}$. Khi đó tồn tại một phân thớ chính $\lambda = (P, G, B, \pi)$ và một họ các tiết diện $(s_i)_{i \in I}$ của $\lambda$ trên các $U_i$, sao cho quan hệ (4) được thỏa mãn. Khi đó điều tương tự cũng đúng với (5). Nếu hơn nữa $(\lambda', (s'_i))$ thỏa mãn cùng các điều kiện ấy, thì tồn tại duy nhất một G-B-đẳng cấu $f$ của $\lambda$ lên $\lambda'$ sao cho $s'_i = f \circ s_i$ với mọi $i \in I$. Kết quả này được phát biểu bằng cách nói rằng $(\lambda, (s_i))$ được xác định đến một đẳng cấu duy nhất bởi xiclu $g$.

6.4.4. Cho $\lambda = (P, G, B, \pi)$ và $\lambda' = (P', G, B, \pi')$ là hai phép phân thớ chính. Cho $(s_i)$ (tương ứng $(s'_i)$) là một họ các tiết diện của $\lambda$ (tương ứng $\lambda'$) trên các $U_i$ và cho $g$ (tương ứng $g'$) là cocycle liên kết với $(\lambda, \mathcal{U}, (s_i))$ (tương ứng $(\lambda', \mathcal{U}, (s'_i))$). Để $\lambda$ và $\lambda'$ là G-B-đẳng cấu, điều kiện cần và đủ là các cocycle $g$ và $g'$ là đồng điều. Chính xác hơn, với mỗi G-B-đẳng cấu $f$ của $\lambda$ lên $\lambda'$, tồn tại một và chỉ một họ $(h_i)_{i \in I}$ các cấu xạ của $U_i$ vào $G$ sao cho quan hệ (3) được thỏa mãn và sao cho ta có $f \circ (s'_i(x)) = s_i(x) \cdot h_i(x)$ với mọi $i \in I$ và mọi $x \in U_i$, và do đó thu được một song ánh từ tập hợp các G-B-đẳng cấu của $\lambda$ lên $\lambda'$ vào tập hợp các họ $(h_i)_{i \in I}$ thỏa mãn (3).

6.4.5. Ta lấy lại các ký hiệu của 6.4.2. và cho $\mathcal{V} = (V_\alpha)_{\alpha \in A}$ là một phủ mở mịn hơn phủ mở $\mathcal{U}$. Cho $\tau : A \to I$ là một ánh xạ sao cho $V_\alpha \subset U_{\tau(\alpha)}$ với mọi $\alpha \in A$. Cho $s'_\alpha$ là hạn chế của tiết diện $s_{\tau(\alpha)}$ xuống $V_\alpha$ và cho $g' = (g'_{\alpha,\beta})$ là cocycle phụ thuộc vào phủ mở $\mathcal{V}$ liên kết với $(\lambda, \mathcal{V}, (s'_\alpha))$. Khi đó hàm chuyển tiếp $g'_{\alpha,\beta}$ là hạn chế xuống $V_\alpha \cap V_\beta$ của hàm chuyển tiếp $g_{\tau(\alpha), \tau(\beta)}$.

### 6.5. Các không gian thớ liên kết với một phép phân thớ chính

6.5.1. Cho $\lambda = (P, G, B, \pi)$ là một phép phân thớ chính. Cho F là một đa dạng trên đó nhóm G tác động bên trái; ta ký hiệu luật phép toán của G trên F bởi $(g, y) \mapsto g \cdot y$. Nhóm G tác động bên phải trên $P \times F$ theo công thức $(x, f) \cdot g = (x \cdot g, g^{-1} \cdot f)$; quan hệ tương đương được xác định bởi G trong $P \times F$ là chính quy; thương $P \times^G F = (P \times F)/G$ được trang bị một cấu trúc đa dạng.

Cho E là một đa dạng. Ta nói rằng E được trang bị một cấu trúc của không gian thớ liên kết với $\lambda$ có kiểu thớ F khi ta đã cho một cấu xạ $\rho : P \times F \to E$ có tính chất sau:

(As) Có $\rho(x \cdot g, g^{-1}f) = \rho(x, f)$ với $x \in P, f \in F, g \in G$, và ánh xạ $\bar{\rho} : P \times^G F \to E$ suy ra từ $\rho$ bằng cách chuyển qua thương là một đẳng cấu của các đa dạng.

Điều này tương đương với việc nói rằng $(P \times F, G, E, \rho)$ là một phép phân thớ chính. Ánh xạ $\rho$ (hoặc đôi khi ánh xạ $\bar{\rho}$) được gọi là ánh xạ khung của E, và được ký hiệu $(x, f) \mapsto x \cdot f$; ta có

$$
(x \cdot g) \cdot f = x \cdot (g \cdot f), \quad \text{với } x \in P, g \in G \text{ và } f \in F.
$$

Dữ kiện của $\lambda$ và F xác định E sai khác một đẳng cấu duy nhất; đặc biệt, ta có thể lấy E là đa tạp $P \times^G F$; đa tạp này được gọi là không gian sợi liên kết với $\lambda$ có kiểu sợi F, và được ký hiệu bởi $\lambda(F)$.

6.5.2. Cho E là một không gian sợi liên kết với $\lambda$ và có kiểu sợi F. Tồn tại một cấu xạ duy nhất $\pi_E$ từ E vào B sao cho $\pi_E(x \cdot f) = \pi(x)$ nếu $x \in P, f \in F$; bộ ba $(E, B, \pi_E)$ là một phân thớ; nếu B và F là tách được, thì E là tách được.

Cho $b \in B$, và cho $F_b = \pi_E^{-1}(b)$; đây là một đa tạp con đóng của E. Nếu $x \in P$ sao cho $\pi(x) = b$, cho $\theta_x : F \to F_b$ là ánh xạ được xác định bởi $\theta_x(f) = x \cdot f$; đây là một đẳng cấu của các đa tạp. Hơn nữa, với mọi $g \in G$, ta có $\theta_{x \cdot g} = \theta_x \circ \rho_g$, trong đó $\rho_g$ biểu thị tự đẳng cấu $f \mapsto g \cdot f$ của F. Giả sử

F được trang bị một cấu trúc s thuộc một loài bất kỳ Σ (cf. Ens., chap. IV, § 1, n° 4) và giả sử rằng s là bất biến dưới G; khi đó trên $F_b$ tồn tại một cấu trúc $s_b$ thuộc loài Σ và chỉ một cấu trúc như vậy sao cho các $\theta_x : F \to F_b$ là các đẳng cấu; nó thu được bằng cách chuyển vận s nhờ một trong các $\theta_x$ (loc. cit., n° 5).

Nếu s là một tiết diện của P trên một tập mở U của B, ánh xạ $(b, f) \mapsto s(b) . f$ là một đẳng cấu của $U \times F$ lên $\pi_E^{-1}(U)$.

6.5.3. Ví dụ:
(a) Cho $\lambda = (B \times G, B, pr_1)$, cho $E = B \times F$, và cho
$$
\rho : (B \times G) \times F \to E
$$
là ánh xạ $(b, g, f) \mapsto (b, g . f)$. Khi đó ta thu được trên $B \times F$ một cấu trúc không gian sợi liên kết với $\lambda$ có kiểu sợi F, được gọi là tầm thường.

(b) Cho $\lambda = (P, G, B, \pi)$ và $\lambda' = (P', G', B', \pi')$ là hai phân thớ chính. Cho F (tương ứng F') là một đa tạp trên đó G (tương ứng G') tác động bên trái; và cho E (tương ứng E') là một không gian sợi liên kết với $\lambda$ (tương ứng với $\lambda'$) có kiểu sợi F (tương ứng F'). Nhóm $G \times G'$ tác động lên $F \times F'$ bởi $(g . g') . (f, f') = (g . f, g' . f')$. Ánh xạ $(P \times P') \times (F \times F') \to E \times E'$ sinh ra các ánh xạ $P \times F \to E$ và $P' \times F' \to E'$ trang bị cho $E \times E'$ một cấu trúc không gian sợi liên kết với $\lambda \times \lambda'$ có kiểu sợi $F \times F'$.

(c) Với ký hiệu của (b), nếu giả sử rằng $B' = B$, ta định nghĩa tương tự trên $E \times_B E'$ một cấu trúc không gian sợi liên kết với $\lambda \times_{B'} \lambda'$ có kiểu sợi $F \times F'$.

6.5.4. Với ký hiệu của n° 6.5.1, cho $h : B' \to B$ là một cấu xạ, cho $\lambda' = B' \times_B \lambda$, và cho $E' = E' \times_B E$. Nếu $P' = B' \times_B P$, định nghĩa một ánh xạ $P' \times F \to E'$ bằng cách đặt $(b', x) . f = (b', x . f)$; khi đó ta trang bị cho $E'$ một cấu trúc không gian sợi liên kết với $\lambda'$ có kiểu sợi F; nó được gọi là ảnh ngược theo h của cấu trúc đã cho trên $E$.

6.5.5. Cho $\lambda = (P, G, B, \pi)$ là một bó sợi chính, và cho E (tương ứng E') là một không gian sợi liên kết với $\lambda$ có kiểu sợi F (tương ứng F'). Cho $u : F \to F'$ là một cấu xạ tương thích với các phép toán của G (nghĩa là sao cho $u(g . f) = g . u(f)$ với $f \in F, g \in G$). Khi đó tồn tại một và chỉ một cấu xạ $\bar{u} : E \to E'$ sao cho $\bar{u}(x . f) = x . u(f)$ với $x \in P, f \in F$. Nếu $u$ là một phép nhúng (tương ứng một phép dưới ngập, một phép dưới nhúng), thì điều tương tự cũng đúng đối với $\bar{u}$.

Đặc biệt, giả sử rằng một đa tạp nhóm H tác động phải lên F sao cho $g . (f . h) = (g . f) . h$ với $g \in G, f \in F, h \in H$. Khi đó mỗi $h \in H$ xác định một tự đẳng cấu $u_h$ của F tương thích với các phép toán của G, do đó một tự đẳng cấu $\bar{u}_h$ của E; nhóm H tác động phải lên E bởi $(y, h) \mapsto \bar{u}_h(y)$.

6.5.6. Cho $\lambda = (P, G, B, \pi)$ là một bó sợi chính, và cho E là một không gian sợi liên kết với $\lambda$ có kiểu sợi F. Cho $s : B \to E$ là một tiết diện của E. Với mọi $x \in P$, tồn tại một phần tử duy nhất $\sigma(x) \in F$ sao cho $s(\pi(x)) = x . \sigma(x)$. Ánh xạ $\sigma : P \to F$ được xác định như vậy là một cấu xạ của các đa tạp, và thỏa mãn đồng nhất thức:

(*) $$
\sigma(x . g) = g^{-1} . \sigma(x).
$$

Ánh xạ $s \mapsto \sigma$ là một song ánh từ tập hợp các tiết diện của E lên tập hợp các cấu xạ từ P vào F thỏa mãn đồng nhất thức (*).

6.5.7. Cho $\lambda = (P, G, B, \pi)$ và $\lambda' = (P', G, B, \pi')$ là hai bó sợi chính có cùng cơ sở B và cùng nhóm cấu trúc G. Bó sợi chính $\lambda \times_B \lambda' = (P \times_B P', G \times G, B, (\pi, \pi')_B)$ có nhóm cấu trúc $G \times G$. Cho $G \times G$ tác động trái lên G bởi công thức:

$$
(g, g') . g_1 = g . g_1 . {g'}^{-1},
$$

và cho E là không gian sợi liên kết với $\lambda \times_B \lambda'$ có kiểu sợi G (được trang bị luật phép toán đã xác định ở trên). Khi đó các tiết diện của E tương ứng song ánh với các đẳng cấu của P lên P’. Chính xác hơn, nếu s là một tiết diện của E tương ứng (xem n° 6.5.6) với cấu xạ $\sigma : P \times_B P' \to G$, thì tồn tại một và chỉ một đẳng cấu G-B $f_s : P \to P'$ sao cho $\sigma(x, f_s(x)) = e$ với mọi $x \in P$; ánh xạ $s \mapsto f_s$ là một song ánh từ tập hợp các tiết diện của E lên tập hợp các đẳng cấu G-B của P lên P’.

### 6.6. Mở rộng và hạn chế của nhóm cấu trúc

6.6.1. Cho $\lambda = (P, G, B, \pi)$ là một bó sợi chính, và cho $\varphi$ là một đồng cấu của G vào một đa tạp nhóm H. Cho G tác động trái lên H bởi $g . h = \varphi(g) . h$ và cho $P \times^G H$ là không gian sợi liên kết với $\lambda$ có kiểu sợi H. Vì các phép tịnh tiến phải trong H tương thích với các phép toán của G, nhóm H tác động phải lên $P \times^G H$ (xem n° 6.5.5); nếu $\pi_H$ chỉ phép chiếu của $P \times^G H$ lên B, thì bộ bốn $(P \times^G H, H, B, \pi_H)$ là một bó sợi chính, được ký hiệu bởi $\varphi(\lambda)$; nó được gọi là suy ra từ $\lambda$ bởi đồng cấu $\varphi$.

Ánh xạ $f$ của P vào $P \times^G H$ gắn với $x \in P$ lớp của $(x, e)$ là một B-cấu xạ của P vào $P \times^G H$ tương thích với $\varphi$ (xem No. 6.3.1). Hơn nữa, nếu $f'$ là một B-cấu xạ của P vào một không gian thớ chính $P'$ với nhóm cấu trúc H, và nếu $f'$ tương thích với $\varphi$, thì tồn tại một H-B-đẳng cấu duy nhất $\theta$ của $P \times^G H$ lên $P'$ sao cho $f' = \theta \circ f$.

6.6.2. Giả sử rằng $\lambda$ được định nghĩa nhờ một phủ mở $\mathcal{V} = (U_i)$ của B và một cocycle $(g_{ij})$ (6.4.2). Khi đó $\varphi(\lambda)$ có thể được định nghĩa nhờ cùng phủ đó và cocycle $(h_{ij})$, với $h_{ij} = \varphi \circ g_{ij}$.

6.6.3. Cho F là một đa dạng trên đó nhóm H tác động bên trái; ta ký hiệu bởi $(h, y) \mapsto h . y$ luật tác động của H trên F. Nhóm G tác động trên F bởi $(g, y) \mapsto \varphi(g) . y$. Cho E là một không gian thớ liên kết với $\varphi(\lambda)$ có kiểu thớ F. Ánh xạ $(x, y) \mapsto f(x) . y$ của $P \times F$ vào E (ánh xạ $f$ là ánh xạ được định nghĩa trong No. 6.6.1) trang bị cho E một cấu trúc của không gian thớ liên kết với $\lambda$ có kiểu thớ F. Đặc biệt, $(P \times^G H) \times^H F$ được đồng nhất một cách chính tắc với $P \times^G F$.

6.6.4. Giả sử rằng G là một đa dạng nhóm con của H, và $\varphi : G \to H$ là đơn ánh chính tắc của G vào H. Khi đó người ta nói rằng $\varphi(\lambda)$ thu được từ $\lambda$ bằng mở rộng đến H của nhóm cấu trúc. Cấu xạ $f : P \to P \times^G H$ của No. 6.6.1 là một đẳng cấu của P lên một đa dạng con đóng của $P \times^G H$ (bằng $P \times^G H$ nếu $G = H$); đẳng cấu này tương thích với các phép toán của G (chú ý rằng G tác động trên $P \times^G H$ như một nhóm con của H).

6.6.5. Giả sử lại rằng G là một đa dạng nhóm con của H, và cho $\mu = (Q, H, B, \pi)$ là một phân thớ chính với nhóm cấu trúc H và cơ sở B, và cho E là một không gian thớ liên kết với $\mu$ có kiểu thớ $H/G$. Nếu $\gamma$ biểu thị phép chiếu chính tắc của H lên $H/G$, đặt $\delta(y) = y . \gamma(e)$, với $y \in Q$ (trong đó $e$ biểu thị phần tử đơn vị của H); khi đó ta thu được một cấu xạ $\delta : Q \to E$ và bộ bốn $(Q, G, E, \delta)$ là một phân thớ chính. Đặc biệt, $Q/G$ được đồng nhất một cách chính tắc với E, bản thân nó đẳng cấu với $Q \times^H H/G$ $^{1}$.

Bây giờ cho $s : B \to E$ là một tiết diện của E, và cho $\lambda_s$ là ảnh ngược bởi $s$ của phân thớ $(Q, G, E, \delta)$ mà ta vừa định nghĩa. Nó là một phân thớ chính, với cơ sở B và nhóm cấu trúc G và mở rộng của nó đến H đẳng cấu với $\mu$; mọi phân thớ có các tính chất này đều có thể thu được theo cách này, sai khác một đẳng cấu; hai tiết diện $s_1$ và $s_2$ của E xác định các phân thớ đẳng cấu khi và chỉ khi chúng được biến đổi thành nhau bởi một H-B-tự đẳng cấu của $\mu$.

### 6.7. Thay đổi cấu trúc

Các cấu trúc và phép toán được mô tả trong đoạn này tương thích với các thay đổi cấu trúc được mô tả trong các No. 5.13 và 5.14.

$^1$ Trong trường hợp tôpô (xem chú ý $^1$, trang 61), cần giả thiết rằng các phép tịnh tiến phải bởi các phần tử của G làm cho H là một không gian sợi chính với nhóm cấu trúc G, với cơ sở $H/G$; điều này tương đương với việc nói rằng tồn tại một tập con mở khác rỗng của $H/G$ mà trên đó phép chiếu $H \to H/G$ thừa nhận một tiết diện liên tục. Trong phạm trù các đa tạp, điều kiện tương tự luôn được thỏa mãn (xem No. 6.2.4).
