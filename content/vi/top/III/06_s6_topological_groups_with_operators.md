---
book: top
book_title: General Topology
chapter: III
chapter_title: Topological Groups
section: 6
section_title: Topological groups with operators; topological rings division rings and fields
lang: vi
source: top-i-iv
pdf_pages: 0277-0289, 0321-0330
extraction: ocr
subsections:
    - "no": 1
      title: TOPOLOGICAL GROUPS WITH OPERATORS
      page: 0
      pdf_page: 277
    - "no": 2
      title: TOPOLOGICAL DIRECT SUM OF STABLE SUBGROUPS
      page: 0
      pdf_page: 278
    - "no": 3
      title: TOPOLOGICAL RINGS
      page: 0
      pdf_page: 280
    - "no": 4
      title: SUBRINGS; IDEALS; QUOTIENT RINGS; PRODUCTS OF RINGS
      page: 0
      pdf_page: 282
    - "no": 5
      title: COMPLETION OF A TOPOLOGICAL RING
      page: 0
      pdf_page: 282
    - "no": 6
      title: TOPOLOGICAL MODULES
      page: 0
      pdf_page: 284
    - "no": 7
      title: TOPOLOGICAL DIVISION RINGS AND FIELDS
      page: 0
      pdf_page: 287
    - "no": 8
      title: UNIFORMITIES ON A TOPOLOGICAL DIVISION RING
      page: 0
      pdf_page: 288
statements: 23
exercises: 26
content_sha256: c9aee2aaf942e05705c2f665e698148f1f033de6337220bfce3c13136a1f231a
translated_from: content/en/top/III/06_s6_topological_groups_with_operators.md
source_content_sha256: af700ea75f1b1fcb3ce8c14c7ff443d7d8f2ec3968b54769d7e02a7e73e6a20a
translation_model: gpt-5-6-mini
translation_run: translate-vi-c62d55af
glossary_version: 34
glossary_terms_sha256: 8cfaa51995a30eb59eac31095baeff907ed6e83867ca6cf623dc2bd74f35f16c
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 6. NHÓM TÔPÔ VỚI TOÁN TỬ; VÀNH TÔPÔ, VÀNH CHIA VÀ TRƯỜNG

### 1. NHÓM TÔPÔ VỚI TOÁN TỬ

Trên một tập $G$, một cấu trúc nhóm với toán tử và một tôpô được gọi là tương thích nếu tôpô và cấu trúc nhóm của $G$ là tương thích (\$ 1, no. 1) và nếu thêm vào đó các tự đồng cấu của $G$ sinh bởi các toán tử là liên tục. Khi đó tập $G$, cùng với tôpô đã cho và cấu trúc nhóm với toán tử, được gọi là một nhóm tôpô với toán tử.

Nếu $H$ là một nhóm con ổn định của một nhóm tôpô $G$ với toán tử, thì tôpô cảm sinh trên $H$ bởi tôpô của $G$ là tương thích với cấu trúc nhóm với toán tử trên $H$. Hơn nữa:

#### Mệnh đề 1 {#top-iii-s6-prop-1 .statement}

*Nếu $H$ là một nhóm con ổn định của một nhóm tôpô $G$ với toán tử, thì bao đóng $\overline{H}$ của $H$ trong $G$ là một nhóm con ổn định của $G$.*

Ta đã biết (\$ 2, no. 1, Mệnh đề 1) rằng $\overline{H}$ là một nhóm con của $G$. Ngoài ra, nếu $\alpha$ là một toán tử tùy ý trên $G$, thì ảnh của $H$ qua ánh xạ liên tục $x \to x^\alpha$ được chứa trong $H$, và do đó ảnh của $\overline{H}$ được chứa trong $\overline{H}$ (Chương I, \$ 2, no. 1, Định lý 1).

Cho $H$ là một nhóm con chuẩn ổn định của một nhóm tôpô $G$ với toán tử. Khi đó, với mỗi toán tử $\alpha$ trên $G$, ánh xạ của $G/H$ vào chính nó cảm sinh bởi $x \to x^\alpha$ là liên tục (\$ 2, no. 8, Nhận xét 3), và do đó cấu trúc nhóm với toán tử trên $G/H$ là tương thích với tôpô thương trên $G/H$.

Cho $(G_i)_{i \in I}$ là một họ các nhóm tôpô với toán tử, trong đó mỗi $G_i$ được giả sử có cùng tập toán tử $\Omega$. Với mỗi $\alpha \in \Omega$, ánh xạ $x \to ((\mathrm{pr}_i x)^\alpha)$ của $G = \prod_{i \in I} G_i$ vào chính nó là liên tục (Chương I, \$ 4, no. 1, Mệnh đề 1), và do đó cấu trúc các nhóm với toán tử trên $G$ là tương thích với tôpô tích trên $G$.

Nếu $G$ là một nhóm tôpô Hausdorff với toán tử và nếu $G$ có một phép hoàn thiện $\hat{G}$ (\$ 3, no. 4), thì mọi tự đồng cấu $x \to x^\alpha$ của $G$ được xác định bởi một toán tử trên $G$ có thể được mở rộng bởi tính liên tục thành một tự đồng cấu của $\hat{G}$ (\S 3, no. 3, Mệnh đề 5). Do đó $\hat{G}$ có cấu trúc của một nhóm tôpô với toán tử, và tập toán tử là giống nhau đối với $\hat{G}$ và $G$.

### 2. TỔNG TRỰC TIẾP TÔPÔ CỦA CÁC NHÓM CON ỔN ĐỊNH

Vì việc nghiên cứu các nhóm giao hoán với toán tử là tương đương với việc nghiên cứu các môđun, đôi khi ta cho phép mình sử dụng thuật ngữ riêng của môđun cho các nhóm giao hoán tùy ý với toán tử; do đó ta có thể nói về các ánh xạ tuyến tính thay vì các đồng cấu nhóm của các nhóm giao hoán với toán tử, và ta có thể dùng từ *phép chiếu* để chỉ một tự đồng cấu lũy đẳng của một nhóm giao hoán với toán tử.

Nếu một nhóm tôpô giao hoán $E$ với toán tử (được viết theo phép cộng) là tổng trực tiếp của một họ *hữu hạn* $(M_i)_{1 \leq i \leq n}$ các nhóm con ổn định, thì song ánh chính tắc $(x_i) \to \sum_{i=1}^n x_i$ của nhóm tích $\prod_{i=1}^n M_i$ lên $E$ là *liên tục*, nhưng *không nhất thiết là một đồng phôi*.

#### Định nghĩa 1 {#top-iii-s6-def-1 .statement}

*Cho $E$ là một nhóm tôpô giao hoán với các toán tử, và cho $(M_i)_{1 \leq i \leq n}$ là một họ hữu hạn các nhóm con ổn định của $E$, sao cho $E$ là tổng trực tiếp của các $M_i$. Khi đó $E$ được gọi là tổng trực tiếp tôpô của các $M_i$ nếu ánh xạ chính tắc $(x_i) \to \sum_{i=1}^n x_i$ của nhóm tích $\prod_{i=1}^n M_i$ lên $E$ là một đồng phôi* (và do đó là một đẳng cấu của các nhóm tôpô với các toán tử).

#### Mệnh đề 2 {#top-iii-s6-prop-2 .statement}

*Cho $E$ là một nhóm tôpô giao hoán với các toán tử là tổng trực tiếp của các nhóm con ổn định $M_i$ ($1 \leq i \leq n$). Cho $(p_i)_{1 \leq i \leq n}$ là họ các phép chiếu liên kết với phân tích $E = \sum_{i=1}^n M_i$. Khi đó $E$ là tổng trực tiếp tôpô của các $M_i$ khi và chỉ khi các $p_i$ là liên tục.*

Vì ánh xạ $x \to (p_i(x))$ là nghịch đảo của ánh xạ $(x_i) \to \sum_{i=1}^n x_i$.

Vì $1 = \sum_{i=1}^n P_i$ (trong đó $1$ ký hiệu cho ánh xạ đồng nhất của $E$) nên chỉ cần $n - 1$ trong số các phép chiếu $p_i$ là liên tục để phép chiếu thứ $n$ cũng liên tục.

Nếu $E$ là tổng trực tiếp tôpô của hai nhóm con ổn định $M, N$, thì $N$ được gọi là một *phần bù tôpô* của $M$ trong $E$; điều này xảy ra khi và chỉ khi ánh xạ chính tắc của $E/M$ lên là một *đẳng cấu* của các nhóm tôpô với các toán tử.

#### Hệ quả {#top-iii-s6-n2-cor-1 .statement}

*Cho $E$ là một nhóm tôpô giao hoán với các toán tử, và cho $M$ là một nhóm con ổn định của $E$. Khi đó các điều kiện sau là tương đương:*

a) $M$ có một phần bù tôpô trong $E$.

b) *Có một phép chiếu liên tục $p$ của $E$ vào $E$ sao cho $p(E) = M$.*

c) *Ánh xạ đồng nhất của $M$ có thể được mở rộng thành một ánh xạ tuyến tính liên tục của $E$ lên $M$.*

Từ Mệnh đề 2 suy ra rằng a) kéo theo b), và hiển nhiên rằng b) kéo theo c). Cuối cùng, nếu $p$ là một ánh xạ tuyến tính liên tục của $E$ lên $M$ mở rộng ánh xạ đồng nhất của $M$, thì $p$ là một phép chiếu liên tục, và các phép chiếu $p$ và $1 - p$ liên kết với phân tích tổng trực tiếp $E = M + N$, trong đó $N = \overline{p}(0)$.

#### Nhận xét 1 {#top-iii-s6-n2-rem-1 .statement}

Để tránh nhầm lẫn, đôi khi ta sẽ nói rằng một nhóm con ổn định của $E$ là một phần bù của $M$ (theo nghĩa của cấu trúc nhóm với các toán tử, không có tôpô) là một *phần bù đại số* của $M$.

#### Nhận xét 2 {#top-iii-s6-n2-rem-2 .statement}

Nếu một nhóm tôpô giao hoán *Hausdorff* có toán tử là tổng trực tiếp tôpô của một họ $(M_i)_{1 \leq i \leq n}$ các nhóm con ổn định, thì mỗi nhóm con $M_i$ là *đóng* trong $E$, vì $M_i$ là tập hợp tất cả các $x \in E$ sao cho $p_i(x) = x$ (Chương I, § 8, no. 1, Mệnh đề 2).

#### Mệnh đề 3 {#top-iii-s6-prop-3 .statement}

*Cho $E, F$ là hai nhóm tôpô giao hoán có toán tử, và cho $u$ là một ánh xạ tuyến tính liên tục từ $E$ vào $F$. Để tồn tại một ánh xạ tuyến tính liên tục $v$ từ $F$ vào $E$ sao cho $u \circ v$ là ánh xạ đồng nhất của $F$ (trong trường hợp đó $u$ được gọi là khả nghịch phải và $v$ được gọi là một *nghịch đảo phải* của $u$), điều kiện cần và đủ là $u$ là một cấu xạ ngặt (\S 2, no. 8) từ $E$ lên $F$ và $\overline{u}(0)$ có một phần bù tôpô trong $E$.*

Các điều kiện là *cần thiết*. Thật vậy, khi đó ta có $u(v(F)) = F$ và *a fortiori* $u(E) = F$; hơn nữa, nếu $p = v \circ u$, thì $p$ là một ánh xạ tuyến tính liên tục từ $E$ vào chính nó sao cho $p^2 = p$; do đó (Hệ quả của Mệnh đề 2) $p(E) = v(u(E)) = v(F)$ có một phần bù tôpô $\overline{p}(0)$ trong $E$; nhưng vì $u(p(x))) = u(x)$ theo giả thiết, ta có $\overline{u}(0) = \overline{p}(0)$. Cuối cùng, ánh xạ song ánh từ $E/\overline{u}(0)$ lên $F$, liên kết với $u$, là hợp thành của ánh xạ song ánh từ $E/\overline{u}(0)$ lên $v(F)$, liên kết với $p$, và hạn chế của $u$ trên $v(F)$; vì $v$ liên tục, cả hai ánh xạ này đều là các đẳng cấu, và do đó $u$ là một cấu xạ ngặt từ $E$ lên $F$.

Các điều kiện là *đủ*. Thật vậy, nếu $\varphi$ là đồng cấu chính tắc từ E lên $E/\overline{u}^1(o)$, việc nói rằng $\overline{u}^1(o)$ có một phần bù tôpô M trong E chính là nói rằng hạn chế của $\varphi$ trên M là một đẳng cấu của M lên $E/\overline{u}^1(o)$. Mặt khác, vì $u = w \circ \varphi$, trong đó w là một đẳng cấu của $E/\overline{u}^1(o)$ lên F, ta thấy rằng hạn chế của u trên M là một đẳng cấu của M lên F, và đẳng cấu nghịch đảo v do đó thỏa mãn $u \circ v$ là ánh xạ đồng nhất của F lên chính nó.

#### Mệnh đề 4 {#top-iii-s6-prop-4 .statement}

*Cho E, F là hai nhóm tôpô giao hoán có toán tử, và cho u là một ánh xạ tuyến tính liên tục từ E vào F. Để tồn tại một ánh xạ tuyến tính liên tục v từ F vào E sao cho $v \circ u$ là ánh xạ đồng nhất của E lên chính nó* (trong trường hợp đó u được gọi là *khả nghịch trái* và v được gọi là một *nghịch đảo trái* của u), *điều kiện cần và đủ là u là một đẳng cấu (tôpô) của E lên u(E), và u(E) có một phần bù tôpô trong F.*

Các điều kiện là *đủ*, vì nếu chúng được thỏa mãn thì ta thu được một nghịch đảo trái v của u bằng cách lấy hợp thành của đẳng cấu từ u(E) lên E là nghịch đảo của u, với một phép chiếu liên tục của F lên u(E).

Các điều kiện là *cần thiết*. Thật vậy, quan hệ $v(u(x)) = x$ cho thấy rằng $\overline{u}^1(o) = \{ o \}$; do đó u là một song ánh của E lên u(E), và vì hạn chế của v trên u(E) là liên tục, suy ra rằng u là một đẳng cấu của E lên u(E). Mặt khác, nếu đặt $q = u \circ v$, thì q là một ánh xạ tuyến tính liên tục từ F lên u(E) sao cho $q^2 = q$, điều này chứng minh (Hệ quả của Mệnh đề 2) rằng u(E) có một phần bù tôpô trong F.

### 3. CÁC VÀNH TÔPÔ

#### Định nghĩa 2 {#top-iii-s6-def-2 .statement}

*Một vành tôpô là một tập hợp A mang một cấu trúc vành và một tôpô thỏa mãn các tiên đề sau:*

*(AT$_\mathrm{I}$)*. *Ánh xạ* $(x, y) \to x + y$ *của* $A \times A$ *vào* A *là liên tục.*
*(AT$_\mathrm{II}$)*. *Ánh xạ* $x \to -x$ *của* A *vào* A *là liên tục.*
*(AT$_\mathrm{III}$)*. *Ánh xạ* $(x, y) \to xy$ *của* $A \times A$ *vào* A *là liên tục.*

Hai tiên đề đầu biểu thị rằng tôpô của A tương thích với cấu trúc *nhóm cộng* của nó (\S 1, no. 1).

Nếu một cấu trúc vành và một tôpô được cho trên một tập hợp A, chúng được gọi là *tương thích* nếu chúng thỏa mãn các tiên đề (AT$_\mathrm{I}$), (AT$_\mathrm{II}$) và (AT$_\mathrm{III}$).

#### Ví dụ 1 {#top-iii-s6-n3-exa-1 .statement}

Trên mọi vành A, tôpô *rời rạc* là tương thích với cấu trúc vành. Một vành tôpô có tôpô rời rạc được gọi là một vành *rời rạc*.

#### Ví dụ 2 {#top-iii-s6-n3-exa-2 .statement}

Ta sẽ thấy trong Chương IV rằng tôpô của đường thẳng hữu tỉ Q (tương ứng đường thẳng thực R) là tương thích với cấu trúc vành của Q (tương ứng R).*

Trong một vành tôpô, mọi phép vị tự trái $x \to ax$ (tương ứng mọi phép vị tự phải $x \to xa$) là liên tục (và là một phép đồng phôi nếu $a$ là một phần tử khả nghịch của $A$).

Vì ta có thể viết đồng nhất
$$
xy - x_0 y_0 = (x - x_0)(y - y_0) + (x - x_0)y_0 + x_0(y - y_0)
$$
tiên đề (AT_{III}) [dựa vào (AT_I) và (AT_{II})] tương đương với phép hội của hai tiên đề sau:
(AT_{III a}). *Với mọi* $x_0 \in A$, *các ánh xạ* $x \to x_0 x$ *và* $x \to xx_0$ *là liên tục tại điểm* $x = 0$.
(AT_{III b}). *Ánh xạ* $(x, y) \to xy$ *của* $A \times A$ *vào* $A$ *là liên tục tại điểm* $(0, 0)$.

Từ đó ta có thể suy ra một hệ điều kiện cần và đủ mà bộ lọc $\mathcal{B}$ của các lân cận của $0$ trong một vành $A$ phải thỏa mãn để định nghĩa một tôpô trên $A$ tương thích với cấu trúc vành của nó: $\mathcal{B}$ phải thỏa mãn các tiên đề (GA_I) và (GA_{II}) của § 1, và thêm hai tiên đề sau:
(AV_I). *Với mọi* $x_0 \in A$ *và mọi* $V \in \mathcal{B}$, *tồn tại* $W \in \mathcal{B}$ *sao cho* $x_0 W \subset V$ *và* $W x_0 \subset V$.
(AV_{II}). *Với mọi* $V \in \mathcal{B}$, *tồn tại* $W \in \mathcal{B}$ *sao cho* $WW \subset V$.

#### Nhận xét {#top-iii-s6-n3-rem-1 .statement}

Trong giải tích, ta khá thường gặp các vành thỏa mãn các tiên đề (AT_I), (AT_{II}) và (AT_{III a}), nhưng không thỏa mãn (AT_{III b}). *Một ví dụ là vành các độ đo trên một nhóm compact, trong đó phép nhân là phép chập và tôpô là tôpô yếu.*

*Ví dụ 3).* Cho $\mathcal{B}$ là một cơ sở lọc trên một vành $A$, gồm các *iđêan hai phía*. $\mathcal{B}$ là một hệ cơ bản các lân cận của $0$ đối với một tôpô tương thích với cấu trúc nhóm cộng của $A$, và điều này suy ra ngay lập tức từ (AV_I) và (AV_{II}) rằng tôpô này tương thích với cấu trúc *vành* của $A$.

Cho $X$ là một không gian tôpô, và cho $f$ và $g$ là hai ánh xạ của $X$ vào một vành tôpô $A$. Nếu $f$ và $g$ liên tục tại một điểm $x_0 \in X$, thì $f + g$, $-f$ và $fg$ liên tục tại điểm này. Suy ra rằng các ánh xạ liên tục của $X$ vào $A$ tạo thành một *vành con* của vành $A^X$ của tất cả các ánh xạ của $X$ vào $A$. Ta cũng thấy rằng, nếu $A$ là *giao hoán*, thì mọi *đa thức n biến*, với các hệ số trong $A$ và xác định trên $A^n$, là *liên tục* trên $A^n$. Một lần nữa, cho $f$ và $g$ là hai ánh xạ của một tập hợp $X$, *lọc* bởi một bộ lọc $\mathfrak{F}$, vào một vành tôpô *Hausdorff* $A$; nếu $\lim_{\mathfrak{F}} f$ và $\lim_{\mathfrak{F}} g$ tồn tại, thì $\lim_{\mathfrak{F}} (f + g)$, $\lim_{\mathfrak{F}} (-f)$ và $\lim_{\mathfrak{F}} (fg)$ cũng tồn tại, và ta có (Chương I, § 7, no. 4, Mệnh đề 9, Hệ quả 1, và § 8, no. 1, Mệnh đề 1)

(1) $$ \lim_{\mathfrak{F}} (f + g) = \lim_{\mathfrak{F}} f + \lim_{\mathfrak{F}} g, $$
(2) $$ \lim_{\mathfrak{F}} (-f) = -\lim_{\mathfrak{F}} f, $$
(3) $$ \lim_{\mathfrak{F}} (fg) = (\lim_{\mathfrak{F}} f) (\lim_{\mathfrak{F}} g). $$

### 4. VÀNH CON; IĐÊAN; CÁC VÀNH THƯƠNG; CÁC TÍCH CỦA CÁC VÀNH

Nếu $H$ là một vành con của một vành tôpô $A$, thì tôpô cảm sinh trên $H$ bởi tôpô của $A$ là tương thích với cấu trúc vành của $H$. Cấu trúc vành tôpô được xác định như vậy trên $H$ được gọi là *cảm sinh* bởi cấu trúc vành của $A$.

#### Mệnh đề 5 {#top-iii-s6-prop-5 .statement}

*Cho $H$ là một vành con trù mật của một vành tôpô $A$, và cho $K$ là một vành con (tương ứng, iđêan trái, iđêan phải, iđêan hai phía) của $H$. Khi đó bao đóng $\overline{K}$ của $K$ trong $A$ là một vành con (tương ứng, iđêan trái, iđêan phải, iđêan hai phía) của $A$.*

Chứng minh giống như đối với Mệnh đề 8 của § 2, số 3 : nếu chẳng hạn $K$ là một iđêan trái trong $H$, thì ánh xạ $(z, x) \to zx$ là liên tục trên $A \times A$ và biến $H \times K$ vào $K$; do đó nó biến $A \times K = \overline{H} \times K$ vào $\overline{H}$.

Cho $H$ là một iđêan hai phía trong một vành tôpô $A$. Theo cùng lập luận như đối với các nhóm thương, ta thấy rằng thương của tôpô của $A$ theo quan hệ $x - y \in H$ là tương thích với cấu trúc vành của $A/H$. Đặc biệt, nếu $A$ không Hausdorff, thì bao đóng $N$ của $\{0\}$ trong $A$ là một *iđêan hai phía đóng*, theo Mệnh đề 5; vành thương, là Hausdorff ($\S$ 2, no. 5, Mệnh đề 13) được gọi là *vành Hausdorff liên kết với* $A$.

Cho $(A_i)_{i \in I}$ là một họ các vành tôpô. Trên tập hợp $A = \prod_{i \in I} A_i$, tích của các tôpô của các $A_i$ là tương thích với tích của các cấu trúc vành của các $A_i$ (chứng minh tương tự như đối với các nhóm tích); vành tôpô $A$ được xác định như vậy được gọi là *tích* của các vành tôpô $A_i$.

### 5. HOÀN THÀNH CỦA MỘT VÀNH TÔPÔ

Khi ta nói về *cấu trúc đều* của một vành tôpô, ta luôn hiểu là cấu trúc đều của *nhóm cộng tính* của nó, trừ khi có nói rõ điều ngược lại; đặc biệt, $A$ được gọi là một vành *đầy đủ* nếu nhóm cộng tính của $A$ là đầy đủ.

Cho $A$ là một vành tôpô *Hausdorff*; xét như một nhóm cộng tính, $A$ có thể được xem như một nhóm con trù mật của một nhóm *giao hoán Hausdorff đầy đủ* $\hat{A}$, được xác định sai khác bởi một đẳng cấu ($\S$ 3, no. 5, Định lý 2). Để có thể xem $A$ như một *vành con* của một *vành đầy đủ*, cần thiết phải có khả năng mở rộng hàm $xy$ bằng tính liên tục lên không gian $\hat{A} \times \hat{A}$. Khả năng của sự mở rộng này sẽ suy ra từ định lý tổng quát hơn sau đây :

#### Định lý 1 {#top-iii-s6-thm-1 .statement}

Cho E, F, G là ba nhóm giao hoán Hausdorff đầy đủ; cho A là một nhóm con trù mật của E và cho B là một nhóm con trù mật của F. Nếu f là một ánh xạ song tuyến tính $\mathbf{Z}$-liên tục $\mathbf{Z}$ (*) của $A \times B$ vào G, thì f có thể được mở rộng bằng tính liên tục thành một ánh xạ song tuyến tính $\mathbf{Z}$-liên tục của $E \times F$ vào G.

Cho $(x_0, y_0)$ là một điểm tùy ý của $E \times F$, và cho $\mathfrak{U}, \mathfrak{B}$ là các vết trên A, B tương ứng của các lọc lân cận của $x_0, y_0$ ($\mathfrak{U}, \mathfrak{B}$ là các lọc, theo giả thiết). Để chỉ ra rằng f có thể được mở rộng bằng tính liên tục, chỉ cần chỉ ra rằng $f(\mathfrak{U} \times \mathfrak{B})$ là một cơ sở lọc Cauchy trên G (Chương II, § 3, no. 6, Mệnh đề 11). Xét đẳng thức

$$
f(x', y') - f(x, y) = f(x' - x, y_1) + f(x_1, y' - y) + f(x' - x, y' - y_1).
$$

Ta sẽ chỉ ra rằng bằng cách lấy $(x, y)$ và $(x', y')$ trong một tập hợp đủ nhỏ của $\mathfrak{U} \times \mathfrak{B}$, và bằng cách chọn $x_1$ và $y_1$ thích hợp, ta có thể làm cho mỗi số hạng ở vế phải rất nhỏ. Cho W là một lân cận bất kỳ của 0 trong G; vì f liên tục tại $(0, 0) \in A \times B$, nên có một tập hợp $U \in \mathfrak{B}$ và một tập hợp $V \in \mathfrak{B}$ sao cho $f(x' - x, y' - y) \in W$ bất cứ khi nào $x \in U, x' \in U, y \in V, y' \in V$. Lấy một điểm $x_1 \in U$ và một điểm $y_1 \in V$; khi đó với mọi $x, x'$ trong U và mọi $y, y'$ trong V ta sẽ có

$$
f(x' - x, y' - y_1) + f(x - x_1, y' - y) \in W + W.
$$

Mặt khác, ánh xạ từng phần $x \to f(x, y_1)$ là liên tục trên A; do đó có một tập hợp $U' \subset U$, thuộc $\mathfrak{U}$, và sao cho, bất cứ khi nào $x$ và $x'$ thuộc $U'$, ta có $f(x' - x, y_1) \in W$. Tương tự, tồn tại $V' \subset V$ thuộc $\mathfrak{B}$ sao cho, bất cứ khi nào $y$ và $y'$ thuộc $V'$, ta có $f(x_1, y' - y) \in W$. Do đó, nếu $(x, y)$ và $(x', y')$ là hai điểm bất kỳ của $U' \times V'$, thì

$$
f(x', y') - f(x, y) \in W + W + W + W;
$$

điều này chứng minh sự tồn tại của mở rộng $\overline{f}$ của f. Việc $\overline{f}$ là $\mathbf{Z}$-song tuyến tính là một hệ quả ngay lập tức của nguyên lý mở rộng các đồng nhất thức (Chương I, § 8, no. 1, Hệ quả 1 của Mệnh đề 2).

Q.E.D.

Trong ứng dụng của định lý này vào một vành tôpô Hausdorff A, ta lấy E, F và G lần lượt là $\hat{A}$, A và B là vành A, và f là

(*) $f$ được gọi là $\mathbf{Z}$-song tuyến tính nếu, với mọi phần tử $x, x'$ của A và mọi phần tử $y, y' \in B$ ta có

$$
f(x + x', y) = f(x, y) + f(x', y)
$$
và
$$
f(x, y + y') = f(x, y) + f(x, y').
$$

ánh xạ $\mathbf{Z}$-song tuyến tính $(x, y) \to xy$, mà theo giả thiết là liên tục. Ta lại ký hiệu bởi $xy$ giá trị của hàm mở rộng trên $\hat{A} \times \hat{A}$; hàm này là một luật hợp thành trên $\hat{A}$, và nói rằng nó là $\mathbf{Z}$-song tuyến tính có nghĩa là nó phân phối về cả hai phía đối với phép cộng; và nó cũng *kết hợp*, theo nguyên lý mở rộng các đồng nhất thức. Do đó:

#### Mệnh đề 6 {#top-iii-s6-prop-6 .statement}

*Một vành tôpô Hausdorff* $A$ *là đẳng cấu với một vành con trù mật của một vành Hausdorff đầy đủ* $\hat{A}$, *được xác định đến một đẳng cấu* (và được gọi là *phép hoàn thành* của $A$).

Nếu $A$ là *giao hoán* (tương ứng *có một phần tử đơn vị*) thì điều tương tự cũng đúng đối với $\hat{A}$ (nguyên lý mở rộng các đồng nhất thức).

Cho $A$ là một vành tôpô, không nhất thiết Hausdorff; cho $N$ là bao đóng của $\{0\}$ trong $A$, và cho $A' = A/N$ là vành Hausdorff liên kết với $A$. Khi đó $\hat{A}'$, phép hoàn thành của $A'$, được gọi là *phép hoàn thành Hausdorff* của $A$ và cũng được ký hiệu là $\hat{A}$. Ta chứng minh như trong § 3, no. 4, Mệnh đề 8 rằng mọi đồng cấu vành liên tục $u$ của $A$ với một vành tôpô *Hausdorff đầy đủ* $C$ đều có thể được phân tích duy nhất thành $u = v \circ \varphi$, trong đó $v$ là một đồng cấu liên tục từ $\hat{A}$ vào $C$ và $\varphi$ là ánh xạ chính tắc của $A$ vào $\hat{A}$. Nếu $A, B$ là hai vành tôpô, và $u : A \to B$ là một đồng cấu liên tục, thì do đó tồn tại duy nhất một đồng cấu liên tục $\hat{u} : \hat{A} \to \hat{B}$ sao cho biểu đồ

$$
\begin{array}{ccc}
A & \xrightarrow{u} & B \\
\varphi \downarrow & & \psi \downarrow \\
\hat{A} & \xrightarrow{\hat{u}} & \hat{B}
\end{array}
$$

là giao hoán ($\varphi$ và $\psi$ là các ánh xạ chính tắc); ta chỉ cần áp dụng kết quả trước đó cho $\psi \circ u$.

### 6. CÁC MÔĐUN TÔPÔ

#### Định nghĩa 3 {#top-iii-s6-def-3 .statement}

*Cho một vành tôpô* $A$ *với một phần tử đơn vị, một môđun trái tôpô* $A$*-môđun là một tập hợp* $E$, *cùng với*:

1) *một cấu trúc môđun trái* $A$*;*
2) *một tôpô tương thích với cấu trúc nhóm cộng của* $E$, *và thỏa mãn tiên đề sau*:
(MT) *Ánh xạ* $(\lambda, x) \to \lambda x$ *của* $A \times E$ *vào* $E$ *là liên tục*.

Ta định nghĩa tương tự khái niệm môđun phải tôpô $A$; vì mọi môđun phải $A$ có thể được xem như một môđun trái $A^0$, trong đó $A^0$ là vành đối của $A$, và vì tôpô của $A$ tương thích với cấu trúc vành của $A^0$, nên không cần phân biệt giữa các môđun phải tôpô $A$ và các môđun trái tôpô $A^0$.

#### Ví dụ 1 {#top-iii-s6-n6-exa-1 .statement}

Một không gian vectơ tôpô trên $\mathbf{R}$ (tương ứng $\mathbf{C}$) là một môđun tôpô $\mathbf{R}$ (tương ứng $\mathbf{C}$).

#### Ví dụ 2 {#top-iii-s6-n6-exa-2 .statement}

Cho $A$ là một vành và cho $\mathcal{B}$ là một cơ sở lọc trên $A$ gồm các iđêan hai phía của $A$; cho $E$ là một $A$-môđun trái. Nếu ta trang bị cho $A$ tôpô (tương thích với cấu trúc vành của nó) mà $\mathcal{B}$ là một hệ cơ bản các lân cận của $0$ (no. 3, Ví dụ 3), và cho $E$ tôpô (tương thích với cấu trúc nhóm cộng của nó) trong đó các tập hợp $aE$, khi $a$ chạy qua $\mathcal{B}$, tạo thành một hệ cơ bản các lân cận của $0$ ($\S 1$, no. 2, Ví dụ), thì kiểm tra ngay lập tức được rằng $E$ là một $A$-môđun tôpô.

#### Nhận xét {#top-iii-s6-n6-rem-1 .statement}

Cho một vành tôpô $A$, xét trên một $A$-môđun trái $E$, một tôpô tương thích với cấu trúc nhóm cộng của $E$. Theo đẳng thức
$$
\lambda x - \lambda_0 x_0 = (\lambda - \lambda_0)x_0 + \lambda_0(x - x_0) + (\lambda - \lambda_0)(x - x_0)
$$
tiên đề (MT) tương đương với phép hội của ba tiên đề sau:
(MT$_I'$). *Với mỗi* $x_0 \in E$, *ánh xạ* $\lambda \to \lambda x_0$ *liên tục tại điểm* $\lambda = 0$.
(MT$_{II}'$). *Với mỗi* $\lambda_0 \in A$, *ánh xạ* $x \to \lambda_0 x$ *liên tục tại điểm* $x = 0$.
(MT$_{III}'$). *Ánh xạ* $(\lambda, x) \to \lambda x$ *liên tục tại điểm* $(0, 0)$.

Ta suy ra từ điều này một tập điều kiện cần và đủ mà *bộ lọc* $\mathcal{B}$ *của các lân cận của* $0$ *trong một* $A$*-môđun* $E$ *phải thỏa mãn để định nghĩa một tôpô trên* $E$ *tương thích với cấu trúc môđun của nó;* $\mathcal{B}$ *phải thỏa mãn các tiên đề* (GA$_I$) *và* (GA$_{II}$) *của* $\S 1$, *no. 2*, *và ngoài ra phải thỏa mãn ba tiên đề sau:*
(MV$_I$). *Với mỗi* $x_0 \in E$ *và* $V \in \mathcal{B}$, *có một lân cận* $S$ *của* $0$ *trong* $A$ *sao cho* $S.x_0 \subset V$.
(MV$_{II}$). *Với mỗi* $\lambda_0 \in A$ *và* $V \in \mathcal{B}$, *tồn tại* $W \in \mathcal{B}$ *sao cho* $\lambda_0 W \subset V$.
(MV$_{III}$). *Với mỗi* $V \in \mathcal{B}$ *tồn tại* $U \in \mathcal{B}$ *và một lân cận* $T$ *của* $0$ *trong* $A$ *sao cho* $T.U \subset V$.

Mọi nhóm tôpô giao hoán đều là một $\mathbf{Z}$-môđun tôpô khi vành $\mathbf{Z}$ được cho tôpô rời rạc.

Nếu $M$ là một môđun con của một $A$-môđun tôpô $E$, rõ ràng rằng tôpô cảm sinh trên $M$ bởi tôpô của $E$ là tương thích với cấu trúc môđun của $M$. Hơn nữa, trên $A$-môđun thương $E/M$, tôpô là thương bởi $M$ của tôpô của $E$ là tương thích với cấu trúc $A$-môđun. Để thấy điều này, chỉ cần chỉ ra rằng ánh xạ $(\lambda, x) \to \lambda x$ của $A \times (E/M)$ lên $E/M$ là liên tục (trong đó $x \to x'$ ký hiệu ánh xạ chính tắc của $E$ lên $E/M$). Bây giờ, vì ta có thể đồng nhất các nhóm tôpô cộng tính $A \times (E/M)$ và $(A \times E)/(\{0\} \times M)$ (\S 2, no. 9, Hệ quả của Mệnh đề 26), nên chỉ cần chỉ ra rằng ánh xạ $(\lambda, x) \to \lambda x'$ từ $A \times E$ vào $E/M$ là liên tục; và điều này là ngay lập tức, vì ánh xạ đang xét là hợp thành của $x \to x'$ và $(\lambda, x) \to \lambda x$.

Cho $(E_i)_{i \in I}$ là một họ tùy ý các $A$-môđun tôpô, và cho $E = \prod_{i \in I} E_i$ là $A$-môđun là tích của các $E_i$. Khi đó tôpô tích trên $E$ tương thích với cấu trúc $A$-môđun của $E$. Để chứng minh điều này, chỉ cần chỉ ra rằng ánh xạ $(\lambda, x) \to (\lambda \cdot \mathrm{pr}_i x)_{i \in I}$ từ $A \times E$ vào $E$ là liên tục, hoặc (theo Mệnh đề 1 của Chương I, \S 4, no. 1) rằng với mỗi chỉ số $x \in I$ ánh xạ $(\lambda, x) \to \lambda \cdot \mathrm{pr}_x x$ là một ánh xạ liên tục từ $A \times E$ vào $E_x$; nhưng ánh xạ này là hợp thành của $(\lambda, x_x) \to \lambda x_x$ và $(\lambda, x) \to (\lambda, \mathrm{pr}_x x)$, cả hai đều liên tục.

Cho $A$ là một vành tôpô Hausdorff và $E$ là một $A$-môđun tôpô Hausdorff. Cho $\hat{E}$ là nhóm cộng là phần hoàn thiện của nhóm tôpô giao hoán $E$ (\S 3, no. 5, Định lý 2). Ánh xạ $\mathbf{Z}$-song tuyến tính $(\lambda, x) \to \lambda x$ của tích $A \times E$ của các nhóm cộng $A, E$ vào nhóm cộng $E$ có thể được mở rộng bởi tính liên tục thành một ánh xạ $\mathbf{Z}$-song tuyến tính của $\hat{A} \times \hat{E}$ vào $\hat{E}$ (no. 5, Định lý 1), và ta tiếp tục ký hiệu ánh xạ này bởi $(\lambda, x) \to \lambda x$. Theo nguyên lý mở rộng các đẳng thức, ta có $\lambda (\mu x) = (\lambda \mu) x$ với $\lambda \in \hat{A}, \mu \in \hat{A}$ và $x \in \hat{E}$, và $1 \cdot x = x$ với mọi $x \in \hat{E}$; phép toán ngoài $(\lambda, x) \to \lambda x$ do đó xác định một cấu trúc $\hat{A}$-môđun trên $\hat{E}$ tương thích với tôpô của nó. $A$-môđun tôpô $\hat{E}$ được xác định như vậy được gọi là *phần hoàn thiện* của $A$-môđun tôpô $E$.

Cho $E$ là một môđun tôpô trên một vành tôpô $A$, trong đó $A$ cũng như $E$ không nhất thiết là Hausdorff. Gọi $N$ (tương ứng $F$) là bao đóng của $\{0\}$ trong $A$ (tương ứng $E$). $N$ là một iđêan hai phía của $A$ (no. 4, Mệnh đề 5) và $F$ là một môđun con-$A$ của $E$ (no. 1, Mệnh đề 1); hơn nữa, do tính liên tục ta có $\lambda x \in F$ bất cứ khi nào $\lambda \in N$ hoặc $x \in F$. Do đó ta có thể định nghĩa, bằng cách chuyển qua các thương, một ánh xạ $(\dot{\lambda}, \dot{x}) \to \dot{\lambda} \dot{x}$ từ $(A/N) \times (E/F)$ vào $E/F$; dễ dàng kiểm tra được (bằng cách sử dụng Hệ quả của Mệnh đề 26 của \S 2, no. 9) rằng ánh xạ này liên tục, và do đó định nghĩa một cấu trúc của một $(A/N)$-môđun tôpô trên $E/F$. Nếu đặt $B = A/N$ và $L = E/F$, thì môđun-$B$ $L$ được gọi là môđun Hausdorff *liên kết* với $E$; hoàn thành của nó $\hat{L}$ là một môđun tôpô trên hoàn thành Hausdorff $\hat{A}$ (bằng định nghĩa là $\hat{B}$) của $A$ (no. 5), và môđun $\hat{L}$ này được gọi là *hoàn thành Hausdorff* của $E$ và được ký hiệu

$$
\begin{array}{ccc}
E & \xrightarrow{u} & E' \\
\downarrow \varphi & & \downarrow \varphi' \\
\hat{E} & \xrightarrow{\hat{u}} & \hat{E}'
\end{array}
$$

là giao hoán, $\varphi$ và $\varphi'$ là các ánh xạ chính tắc.

Các định nghĩa và các kết quả của tiết này cũng áp dụng tương tự cho các *giả-môđun* trên một vành tôpô tùy ý, bằng cách xóa mọi đề cập đến phần tử đơn vị của vành.

### 7. CÁC VÀNH CHIA TÔPÔ VÀ CÁC TRƯỜNG

Trong phần tiếp theo, và trong các Chương IV và V, nếu $K$ là một *vành chia* thì ta sẽ ký hiệu $K^*$ là *nhóm nhân* của các phần tử khác không của $K$.

#### Định nghĩa 4 {#top-iii-s6-def-4 .statement}

*Một vành chia tôpô là một tập hợp* $K$ *mang một cấu trúc vành chia và một tôpô tương thích với cấu trúc vành của* $K$, *và thỏa mãn thêm tiên đề sau:*

(KT) *Ánh xạ* $x \to x^{-1}$ *từ* $K^*$ *vào* $K^*$ *là liên tục.*

*Một vành chia tôpô giao hoán được gọi là một trường tôpô.*

Một cấu trúc vành chia và một tôpô trên một tập hợp $K$ được gọi là *tương thích* nếu cấu trúc vành tương ứng và tôpô là tương thích, và nếu thêm vào đó tiên đề (KT) được thỏa mãn.

#### Ví dụ 1 {#top-iii-s6-n7-exa-1 .statement}

Trên mọi vành chia $K$, tôpô *rời rạc* là tương thích với cấu trúc vành chia. Một vành chia tôpô mà tôpô của nó là rời rạc được gọi là một vành chia *rời rạc*.
\* 2) Tôpô của đường hữu tỉ $Q$ (tương ứng đường thẳng thực $R$) là tương thích với cấu trúc trường của $R$ (tương ứng $R$) (xem Chương IV, § 3). \*

Định nghĩa 4 chỉ ra rằng, nếu $K$ là một vành chia tôpô, thì tôpô *cảm sinh* bởi tôpô của $K$ trên nhóm nhân $K^*$ là tương thích với cấu trúc nhóm của $K^*$.

Nếu $a \neq 0$, các phép vị tự $x \to ax$ và $x \to xa$ là các đồng phôi của $K$ lên chính nó; và ánh xạ $x \to ax + b$ cũng vậy với mọi $b \in K$. Chú ý rằng các phép vị tự $x \to ax$ và $x \to xa$ là các *tự đẳng cấu* của *nhóm cộng* (tôpô) của $K$ nếu $a \neq 0$. Nếu $V$ là một lân cận bất kỳ của $o$ trong $K$, thì do đó suy ra rằng $aV$ và $Va$ là các lân cận của $o$ với mọi $a \neq 0$.

Cho $X$ là một không gian tôpô, và cho $f$ là một ánh xạ từ $X$ vào một vành chia tôpô $K$. Nếu $f$ liên tục tại một điểm $x_0 \in X$ và nếu $f(x_0) \neq 0$, thì $f^{-1}$ liên tục tại $x_0$. Đặc biệt, nếu $K$ là một *trường* tôpô, thì mọi *hàm hữu tỉ* theo $n$ biến với các hệ số trong $K$ đều liên tục tại mọi điểm của $K^n$ mà tại đó mẫu số của nó không triệt tiêu.

Tương tự, nếu $f$ là một ánh xạ từ một tập hợp $X$, được lọc bởi một lọc $\mathfrak{F}$, vào một vành chia tôpô Hausdorff $K$, và nếu $\lim_{\mathfrak{F}} f$ tồn tại và khác $0$, thì $\lim_{\mathfrak{F}} f^{-1}$ tồn tại và ta có

$$
\lim_{\mathfrak{F}} f^{-1} = (\lim_{\mathfrak{F}} f)^{-1}.
$$

Nếu $H$ là một *vành con chia* của một vành chia tôpô $K$, thì tôpô cảm sinh trên $H$ bởi tôpô của $K$ tương thích với cấu trúc vành chia của $H$. Cấu trúc của một vành chia tôpô được xác định như vậy trên $H$ được gọi là *cảm sinh* bởi cấu trúc của $K$. Hơn nữa, $\overline{H}$ cũng là một *vành con chia* của $K$ (chứng minh tương tự như chứng minh của Mệnh đề 5).

Trong một vành chia tôpô $K$, bao đóng của tập hợp $\{0\}$ là một iđêan hai phía, theo Mệnh đề 5, và do đó phải là hoặc $\{0\}$ hoặc $K$. Nói cách khác, nếu tôpô của $K$ không phải là tôpô thô nhất (Chương I, § 2, no. 2) thì nó là Hausdorff (§ 1, no. 2, Mệnh đề 2).

### 8. CÁC CẤU TRÚC ĐỀU TRÊN MỘT VÀNH CHIA TÔPÔ

Nếu $K$ là một vành chia tôpô thì cần phải phân biệt giữa:
1) cấu trúc đều của *nhóm cộng* của $K$, được xác định trên $K$ và được gọi là *cấu trúc đều cộng* của $K$; và 2) các cấu trúc đều trái và phải của *nhóm nhân* $K^*$, được xác định trên $K^*$ và được gọi (do lạm dụng ngôn ngữ) là các cấu trúc đều *nhân* của $K$.

Tính *cảm sinh* trên $K^*$ bởi cấu trúc đều cộng tính của $K$ nói chung là *phân biệt* với các cấu trúc đều nhân của $K$ (xem Bài tập 17).

Theo Mệnh đề 6, một vành chia tôpô Hausdorff $K$ có thể được xem như một *vành con trù mật* của một *vành Hausdorff đầy đủ* $\hat{K}$. Để $\hat{K}$ là một *vành chia tôpô* thì cần thiết rằng ánh xạ

#### Mệnh đề 7 {#top-iii-s6-prop-7 .statement}

*Phép đầy đủ $\hat{K}$ của một vành chia tôpô Hausdorff K là một vành chia tôpô khi và chỉ khi ảnh qua ánh xạ $x \to x^{-1}$ của mọi lọc Cauchy (đối với cấu trúc cộng tính) không có điểm tụ tại 0 là một lọc Cauchy (đối với cấu trúc cộng tính).*

Có những vành chia tôpô trong đó điều kiện này không được thỏa mãn và trong đó vành $\hat{K}$ có các ước không (xem Bài tập 26). Hơn nữa, ngay cả khi phép đầy đủ $\hat{K}$ là một vành chia tôpô, không có lý do *tiên nghiệm* nào để giả sử rằng các cấu trúc *nhân* của $\hat{K}$ là các cấu trúc của một *không gian đầy đủ*. Tuy nhiên, điều này sẽ đúng đối với các vành chia $K$ sao cho $\hat{K}$ là *địa phương compact* (xem Chương I, § 9, no. 7, Mệnh đề 13, và Chương III, § 3, no. 3, Mệnh đề 4) và đối với các *trường* tôpô; đối với trường hợp sau, ta có mệnh đề sau:

#### Mệnh đề 8 {#top-iii-s6-prop-8 .statement}

*Nếu cấu trúc đều cộng tính của một trường tôpô K là một cấu trúc của một không gian Hausdorff đầy đủ, thì cấu trúc nhân trên K* là một cấu trúc của một không gian đầy đủ.*

Ta sẽ chứng minh rằng nếu $\mathfrak{F}$ là một lọc Cauchy đối với cấu trúc *nhân* trên K*, thì $\mathfrak{F}$ là một lọc Cauchy đối với cấu trúc *cộng tính* trên K, và không hội tụ về 0; điều này sẽ thiết lập kết quả. Cho U là một lân cận bất kỳ của 0 trong K, cho V là một lân cận đóng của 0 sao cho $V \subset U, VV \subset U$ [tiên đề (AV$_\text{II}$)] và $-1 \notin V$; khi đó theo giả thiết tồn tại một tập hợp $A \in \mathfrak{F}$ sao cho, với mọi $x \in A$ và $y \in A$, ta có $x^{-1}y \in 1 + V$. Cho $a \in A$, khi đó $A \subset a + aV$, và $a + aV$ là một tập hợp đóng không chứa 0; do đó 0 không thuộc bao đóng của A và vì vậy không là điểm tụ của $\mathfrak{F}$. Cho W là một lân cận của 0 sao cho $aW \subset V$ [tiên đề (AV$_\text{I}$)]; khi đó theo giả thiết tồn tại một tập hợp $B \in \mathfrak{F}$ sao cho $B \subset A$ và, với mọi $x \in B$ và $y \in B$, ta có $x^{-1}y \in 1 + W$; do đó $y - x \in xW \subset AW \subset aW + aVW$; nhưng K là giao hoán, và vì vậy $aVW = aWV \subset VW \subset U$; do đó $y - x \in U + U$ và Mệnh đề được chứng minh.

Cùng một chứng minh cho thấy Mệnh đề 8 có thể được mở rộng đến trường hợp trong đó mọi lọc Cauchy đối với *một* trong các cấu trúc nhân của K cũng là một lọc Cauchy đối với cấu trúc nhân kia.

### Bài tập {#top-iii-s6-exercises}

Xem [các bài tập của § 6](exercises/s6/).
