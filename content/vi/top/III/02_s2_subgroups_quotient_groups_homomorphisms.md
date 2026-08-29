---
book: top
book_title: General Topology
chapter: III
chapter_title: Topological Groups
section: 2
section_title: Subgroups, quotient groups, homomorphisms homogeneous spaces, product groups
lang: vi
source: top-i-iv
pdf_pages: 0231-0248, 0304-0311
extraction: ocr
subsections:
    - "no": 1
      title: SUBGROUPS OF A TOPOLOGICAL GROUP
      page: 0
      pdf_page: 231
    - "no": 2
      title: COMPONENTS OF A TOPOLOGICAL GROUP
      page: 0
      pdf_page: 233
    - "no": 3
      title: DENSE SUBGROUPS
      page: 0
      pdf_page: 234
    - "no": 4
      title: SPACES WITH OPERATORS
      page: 0
      pdf_page: 234
    - "no": 5
      title: HOMOGENEOUS SPACES
      page: 0
      pdf_page: 237
    - "no": 6
      title: QUOTIENT GROUPS
      page: 0
      pdf_page: 238
    - "no": 7
      title: SUBGROUPS AND QUOTIENT GROUPS OF A QUOTIENT GROUP
      page: 0
      pdf_page: 239
    - "no": 8
      title: CONTINUOUS HOMOMORPHISMS AND STRICT MORPHISMS
      page: 0
      pdf_page: 241
    - "no": 9
      title: PRODUCTS OF TOPOLOGICAL GROUPS
      page: 0
      pdf_page: 243
    - "no": 10
      title: SEMI-DIRECT PRODUCTS
      page: 0
      pdf_page: 245
statements: 45
exercises: 31
content_sha256: 3a9b626cf8dfceae72121c337568c449ab99d3146b02c1473fdee26cd4bdb8e4
translated_from: content/en/top/III/02_s2_subgroups_quotient_groups_homomorphisms.md
source_content_sha256: 09d7ecdaae15234f6b98dd6b72f9c1f771f5a6bc26fa08e838278d792205c2fa
translation_model: gpt-5-6-mini, gpt-5-6, gpt-5.4
translation_run: translate-vi-bfba6fb6
glossary_version: 34
glossary_terms_sha256: a3b628d77a1d0db24647e9674444ccf78fdacc3e6a29a56da834f46faaab23bb
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 2. NHÓM CON, NHÓM THƯƠNG, ĐỒNG CẤU NHÓM, KHÔNG GIAN THUẦN NHẤT, NHÓM TÍCH

### 1. CÁC NHÓM CON CỦA MỘT NHÓM TÔPÔ

Cho G là một nhóm tôpô và H là một nhóm con của G. Theo (GT'), tôpô cảm sinh trên H bởi tôpô của G là tương thích với cấu trúc nhóm của H. Cấu trúc của một nhóm tôpô được xác định như vậy trên $H$ được gọi là *cảm sinh* bởi cấu trúc của $G$. Mỗi khi ta xét một nhóm con $H$ của $G$ như một nhóm tôpô, thì luôn luôn chính cấu trúc cảm sinh này đang được xét đến, trừ khi điều ngược lại được phát biểu rõ ràng.

#### Mệnh đề 1 {#top-iii-s2-prop-1 .statement}

*Bao đóng $\overline{H}$ của một nhóm con $H$ của một nhóm tôpô $G$ là một nhóm con của $G$. Nếu $H$ là một nhóm con chuẩn của $G$, thì $\overline{H}$ cũng vậy.*

Nếu $a, b \in \overline{H}$ thì $ab^{-1} \in \overline{H}$, bởi vì ánh xạ $(x, y) \to xy^{-1}$ là liên tục trên $G \times G$ và biến $H \times H$ thành $H$ (Chương I, § 2, no. 1, Định lý 1). Tương tự, tính liên tục của ánh xạ $x \to axa^{-1}$ chỉ ra rằng nếu $H$ là chuẩn thì $\overline{H}$ là chuẩn.

Đặc biệt, bao đóng $N$ của tập hợp $\{ e \}$ chỉ gồm phần tử đơn vị của $G$, là một *nhóm con chuẩn* của $G$; và $N = \{ e \}$ khi và chỉ khi $G$ là *Hausdorff* ($\S$ 1, no. 2, Mệnh đề 2).

#### Mệnh đề 2 {#top-iii-s2-prop-2 .statement}

*Nếu $G$ là một nhóm tôpô Hausdorff, thì bao đóng của một nhóm con giao hoán của $G$ là một nhóm con giao hoán của $G$.*

Theo Mệnh đề 1, ta có thể hạn chế vào trường hợp $H$ trù mật trong $G$. Các hàm liên tục $xy$ và $yx$ bằng nhau trên $H \times H$, và do đó bằng nhau trên $G \times G$, theo nguyên lý mở rộng của các đẳng thức (Chương I, § 8, no. 1, Mệnh đề 2, Hệ quả 1).

#### Mệnh đề 3 {#top-iii-s2-prop-3 .statement}

*Cho $G$ là một nhóm tôpô Hausdorff và cho $M$ là một tập con bất kỳ của $G$. Khi đó tập hợp $M'$ gồm các phần tử của $G$ giao hoán với mỗi phần tử của $M$ là một nhóm con đóng của $G$. Đặc biệt, tâm của $G$ là đóng trong $G$.*

Vì $M'$ là giao của các tập hợp $F_m (m \in M)$, trong đó $F_m$ là tập hợp tất cả các $x \in G$ sao cho $xm = mx$; và $F_m$ là đóng (Chương I, § 8, no. 1, Mệnh đề 2).

#### Mệnh đề 4 {#top-iii-s2-prop-4 .statement}

*Cho $G$ là một nhóm tôpô và cho $H$ là một nhóm con của $G$ địa phương đóng tại một điểm của $H$ (Chương I, § 3, no. 3, Định nghĩa 2). Khi đó $H$ là đóng trong $G$.*

Do phép tịnh tiến, $H$ là đóng địa phương tại mỗi điểm của nó, tức là $H$ là đóng địa phương trong $G$. Cho $V$ là một lân cận mở đối xứng của $e$ trong $G$ sao cho $V \cap H$ là đóng trong $V$. Nếu $x \in \overline{H}$, thì $xV$ gặp $H$; nếu $y \in xV \cap H$, ta có $x \in yV$, và $y(V \cap H) = (yV) \cap H$ là đóng trong $yV$. Nhưng $x$ nằm trong bao đóng của $(yV) \cap H$, do đó $x \in H$.

#### Hệ quả {#top-iii-s2-n1-cor-1 .statement}

*Một nhóm con của một nhóm tôpô là mở khi và chỉ khi nó có một điểm trong. Mọi nhóm con mở đều đóng.*

Nếu một nhóm con $H$ có một điểm trong, thì do phép tịnh tiến mọi điểm của $H$ đều là điểm trong và do đó $H$ là mở. Mệnh đề thứ hai của hệ quả là một trường hợp riêng của Mệnh đề 4.

#### Mệnh đề 5 {#top-iii-s2-prop-5 .statement}

*Một nhóm con $H$ của một nhóm tôpô $G$ là rời rạc khi và chỉ khi $H$ có một điểm cô lập. Mọi nhóm con rời rạc của một nhóm Hausdorff đều đóng.*

Nếu $H$ là rời rạc, mọi điểm của $H$ đều là cô lập. Ngược lại, nếu $H$ có một điểm cô lập, thì do phép tịnh tiến mọi điểm của $H$ đều là cô lập và do đó $H$ là rời rạc. Nếu $H$ là rời rạc và $G$ là Hausdorff, thì tồn tại một lân cận $V$ của $e$ sao cho $V \cap H = \{e\}$; $\{e\}$ là đóng trong $G$ và do đó *a fortiori* trong $V$, vì thế $H$ là đóng địa phương tại $e$. Suy ra $H$ là đóng trong $G$ theo Mệnh đề 4.

#### Nhận xét {#top-iii-s2-n1-rem-1 .statement}

Cho $H$ là một nhóm con bất kỳ của một nhóm tôpô $G$. Với mỗi $x \in \overline{H}$ ta có $x \overline{H} = x$. $\overline{H} = \overline{H}$, vì phép tịnh tiến bởi $x$ là một đồng phôi của $G$ lên $G$. Nói cách khác, với mỗi $x \in \overline{H}$, $xH$ là *trù mật* trong $\overline{H}$. Suy ra rằng nếu $H$ không đóng, thì $\overline{H} \cap CH$ là *trù mật* trong $\overline{H}$.

### 2. CÁC THÀNH PHẦN CỦA MỘT NHÓM TÔPÔ

Cho $V$ là một lân cận *đối xứng* của $e$ trong $G$. Nhóm con sinh bởi $V$, được ký hiệu là $V^\infty$, gồm tất cả các tích $\prod_{i=1}^n x_i$ của các dãy hữu hạn các phần tử của $V$. $V^\infty$ là *mở*, vì $e$ là một điểm trong của nó, và do đó là *đóng* theo Mệnh đề 4 của no. 1. Suy ra rằng:

#### Mệnh đề 6 {#top-iii-s2-prop-6 .statement}

*Một nhóm tôpô liên thông được sinh bởi mọi lân cận của phần tử đơn vị.*

Mệnh đề đảo lại của mệnh đề này nói chung là sai, như ta sẽ thấy ở Chương IV (§ 2, no. 5). Nếu một nhóm tôpô $G$ được sinh bởi mỗi lân cận của phần tử đơn vị, thì điều nhiều nhất có thể nói là $G$ không chứa *nhóm con mở nào* khác $G$.

\* Như một ví dụ về một nhóm không liên thông $G$ có một nhóm con mở phân biệt với $G$, ta có thể nêu *nhóm nhân* $\mathbf{R}^*$ của các số thực khác không, trong đó nhóm con $\mathbf{R}_+^*$ của các số thực $> 0$ vừa mở vừa đóng (xem Chương IV, § 3, no. 2). \*

#### Mệnh đề 7 {#top-iii-s2-prop-7 .statement}

*Trong một nhóm tôpô $G$, thành phần $K$ của phần tử đơn vị $e$ là một nhóm con chuẩn tắc đóng. Thành phần của bất kỳ điểm nào $x \in G$ là lớp kề $x.K = K.x$.*

Thành phần của phần tử đơn vị $e$ của $G$ được gọi là *thành phần đơn vị* của $G$.

### 3. CÁC NHÓM CON TRÙ MẬT

Mệnh đề sau tổng quát hóa Mệnh đề 1 của no. 1:

#### Mệnh đề 8 {#top-iii-s2-prop-8 .statement}

*Cho $H$ là một nhóm con trù mật của một nhóm tôpô $G$, và $K$ là một nhóm con chuẩn tắc của $H$. Khi đó bao đóng $\overline{K}$ của $K$ trong $G$ là một nhóm con chuẩn tắc của $G$.*

Vì ánh xạ $(z, x) \to zxz^{-1}$ liên tục trên $G \times G$, và ánh xạ $H \times K$ vào $K$; do đó (Chương I, § 2, no. 1, Định lý 1) nó ánh xạ $G \times \overline{K} = \overline{H} \times K$ vào $\overline{K}$.

#### Mệnh đề 9 {#top-iii-s2-prop-9 .statement}

*Cho $H$ là một nhóm con trù mật của một nhóm tôpô $G$. Nếu $H$ được sinh bởi mọi lân cận của phần tử đơn vị trong $H$, thì $G$ được sinh bởi mọi lân cận của phần tử đơn vị trong $G$.*

Cho $V$ là một lân cận đối xứng bất kỳ của $e$ trong $G$. Khi đó $V \cap H$ là một lân cận của $e$ trong $H$, và do đó sinh ra $H$. Suy ra $V$ sinh ra một nhóm con $H'$ chứa $H$; nhưng $H'$ là mở và đóng (no. 1, Hệ quả của Mệnh đề 4), và do đó chứa $\overline{H} = G$.

### 4. CÁC KHÔNG GIAN CÓ TOÁN TỬ

Cho $X$ là một không gian tôpô và cho $G$ là một nhóm tôpô. $G$ được gọi là *tác động liên tục* trên $X$ nếu các điều kiện sau được thỏa mãn:

1) $X$ có $G$ làm một nhóm các toán tử; nói cách khác $X$ được trang bị một phép toán ngoài hợp thành $(s, x) \to s.x$ mà $G$ là tập hợp các toán tử, và thỏa mãn $s.(t.x) = (st).x$ và $e.x = x$ với mọi $s, t \in G$ và mọi $x \in X$.

2) Ánh xạ $(s, x) \to s.x$ từ $G \times X$ vào $X$ là *liên tục*.

#### Bổ đề 1 {#top-iii-s2-lem-1 .statement}

*Nếu một nhóm tôpô* $G$ *tác động liên tục trên một không gian tôpô* $X$, *thì với mỗi* $s \in G$ *ánh xạ* $x \to s.x$ *là một đồng phôi của* $X$ *lên* $X$.

Vì ánh xạ này là một song ánh liên tục mà ánh xạ nghịch đảo $x \to s^{-1}.x$ cũng liên tục.

Ta nhắc lại rằng với mỗi $x \in X$, tập hợp $G.x$ gồm các ảnh $s.x$ của $x$ bởi các phần tử $s$ của $G$ được gọi là *quỹ đạo* của $x$ (đối với nhóm các toán tử $G$), và tập hợp tất cả các $s \in G$ sao cho $s.x = x$ là một nhóm con của $G$ được gọi là *nhóm ổn định* của $x$. Quan hệ $R(x, y) : "y$ thuộc quỹ đạo của $x"$ là một quan hệ tương đương trên $X$, được gọi là quan hệ tương đương *xác định bởi* $G$; các lớp tương đương đối với quan hệ này là các quỹ đạo của các điểm của $X$. Không gian tôpô $X/R$ được gọi là *không gian quỹ đạo* của $X$ (đối với $G$), hoặc *không gian thương của* $X$ *bởi nhóm* $G$, và được ký hiệu là $X/G$; và tôpô của $X/G$ được gọi là *thương của tôpô của* $X$ *bởi* $G$.

#### Bổ đề 2 {#top-iii-s2-lem-2 .statement}

*Nếu một nhóm tôpô* $G$ *tác động liên tục trên một không gian tôpô* $X$, *thì quan hệ tương đương* $R$ *xác định bởi* $G$ *là mở*.

Vì phần bão hòa đối với $R$ của một tập con mở $U$ của $X$ là tập hợp $\bigcup_{s \in G} s.U$, và mỗi $s.U$ là mở theo Bổ đề 1.

#### Ví dụ 1 {#top-iii-s2-n4-exa-1 .statement}

Cho $H$ là một nhóm con của nhóm tôpô $G$. $H$ tác động liên tục lên $G$ theo phép toán ngoài $(s, x) \to sx$. $H$ cũng tác động liên tục lên $G$ theo phép toán ngoài $(x, s) \to sxs^{-1}$.

#### Ví dụ 2 {#top-iii-s2-n4-exa-2 .statement}

\* Nếu $K$ là một vành chia tôpô ($§ 6$, no. 7), nhóm nhân $K^*$ tác động liên tục lên $K$ theo phép toán ngoài $(s, x) \to sx$. \*

#### Ví dụ 3 {#top-iii-s2-n4-exa-3 .statement}

Cho $G$ là một nhóm tôpô, $X$ là một không gian tôpô. Khi đó ánh xạ $(s, x) \to x$ từ $G \times X$ vào $X$ là một phép toán ngoài của hợp thành trên $X$, và $G$ tác động liên tục lên $X$ đối với luật này; khi đó ta nói $G$ tác động *tầm thường* lên $X$.

#### Nhận xét {#top-iii-s2-n4-rem-1 .statement}

Thay vì nói rằng một nhóm tôpô $G$ tác động liên tục lên một không gian tôpô $X$, người ta thường nói rằng $G$ tác động liên tục *bên trái* lên $X$. Khi nhóm tôpô $G^0$ đối của $G$ tác động liên tục lên $X$, ta nói rằng $G$ tác động liên tục *bên phải* lên $X$. Điều đó tương đương với việc nói rằng $X$ có một luật hợp thành ngoài liên tục $(s, x) \to s.x$ với $G$ làm tập hợp các toán tử, sao cho $s.(t.x) = (ts).x$ và $e.x = x$. Một luật như vậy thường được viết *bên phải* : $(s, x) \to x.s$ (do đó có thuật ngữ này), và khi đó ta có $(x.t).s = x.(ts)$. Nếu $G$ tác động liên tục bên phải lên $X$ theo luật $(s, x) \to x.s$, thì $G$ cũng tác động liên tục bên trái lên $X$ theo phép toán ngoài $(s, x) \to x.s^{-1}$, theo tiên đề (GT$_{II}$).

Cho $G$ là một nhóm tôpô tác động liên tục trên một không gian tôpô $X$, và cho $\varphi$ là ánh xạ chính tắc của $X$ lên không gian quỹ đạo $X/G$. Cho $A$ là một tập con bất kỳ của $X$, và cho $A'$ là không gian con của $X$ là bao bão hòa của $A$ đối với quan hệ tương đương $R$ xác định bởi $G$ (do đó $A'$ là hợp của các quỹ đạo của các điểm thuộc $A$, và được gọi là *bao bão hòa của $A$ đối với $G$*). $G$ tác động liên tục trên $A'$ bởi hạn chế của $(s, x) \to s.x$ lên $G \times A'$. Hơn nữa, vì $R$ là mở (Bổ đề 2) và $A'$ là bão hòa, từ Mệnh đề 4 của Chương I, § 5, no. 2, và từ quan hệ $\varphi(A) = \varphi(A')$, suy ra rằng:

#### Mệnh đề 10 {#top-iii-s2-prop-10 .statement}

*Song ánh chính tắc của không gian con $\varphi(A)$ của $X/G$ lên không gian quỹ đạo $A'/G$ là một phép đồng phôi.*

Bây giờ cho $S$ là một quan hệ tương đương trên $X$ sao cho, với mỗi $s \in G$, ánh xạ $x \to s.x$ là *tương thích* với $S$ [nói cách khác, sao cho quan hệ $x \equiv y \pmod{S}$ kéo theo $s.x \equiv s.y \pmod{S}$]; để ngắn gọn, ta sẽ nói rằng quan hệ $S$ là *tương thích với nhóm* $G$. Nếu $\psi$ là ánh xạ chính tắc của $X$ lên $X/S$, và nếu $s.\psi(x)$ ký hiệu lớp mod $S$ của $s.x$, thì $X/S$ có $G$ làm nhóm các toán tử đối với phép toán ngoài $(s, \psi(x)) \to s.\psi(x) = \psi(s.x)$. Hơn nữa:

#### Mệnh đề 11 {#top-iii-s2-prop-11 .statement}

*Nếu quan hệ tương đương $S$ trên $X$ là mở và tương thích với $G$, thì $G$ tác động liên tục trên $X/S$.*

Vì quan hệ đẳng thức trên $G$ và quan hệ $S$ trên $X$ đều mở, chỉ cần chứng minh rằng ánh xạ $(s, x) \to s.\psi(x) = \psi(s.x)$ từ $G \times X$ vào $X/S$ là liên tục (Chương I, § 5, no. 3, Hệ quả của Mệnh đề 8); nhưng điều này suy ra từ tính liên tục của $\psi$ và của ánh xạ

$$
(s, x) \to s.x.
$$

#### Nhận xét {#top-iii-s2-n4-rem-2 .statement}

Cho $G'$ là một nhóm tôpô khác tác động liên tục trên $X$, và giả sử rằng $s.(s'x) = s'(s.x)$ với mọi $s \in G, s' \in G'$ và x \in X. Khi đó quan hệ tương đương S xác định bởi G' tương thích với G, và vì S là mở (Bổ đề 2) nên suy ra G tác động liên tục trên X/G'. Tương tự, G' tác động liên tục trên X/G. Trong những trường hợp này, hai phép tác động của hai nhóm G và G' trên X được gọi là giao hoán.

### 5. KHÔNG GIAN THUẦN NHẤT

Cho G là một nhóm tôpô và H là một nhóm con của G. H tác động liên tục bên phải trên G theo phép toán ngoài $(t, x) \to xt$, và quỹ đạo của một điểm $x \in G$ là lớp ghép trái $xH$. Do đó tập các quỹ đạo chính là không gian thuần nhất $G/H$ mà trong đại số ta đã gọi như vậy. Mỗi khi nói đến $G/H$ như một không gian tôpô, ta luôn hiểu đó là không gian quỹ đạo của G (đối với H) trừ khi có tuyên bố rõ ràng ngược lại; tức là không gian thương của G theo quan hệ tương đương $x^{-1}y \in H$. Phù hợp với các định nghĩa tổng quát, ta nói rằng tôpô của không gian này là thương theo H của tôpô của G.

#### Mệnh đề 12 {#top-iii-s2-prop-12 .statement}

Nhóm G tác động liên tục trên mọi không gian thuần nhất $G/H$.

Vì quan hệ tương đương $x^{-1}y \in H$ là mở (no. 4, Bổ đề 2), đây là một trường hợp riêng của Mệnh đề 11 của no. 4.

#### Mệnh đề 13 {#top-iii-s2-prop-13 .statement}

Cho G là một nhóm tôpô và H là một nhóm con của G. Khi đó không gian thuần nhất $G/H$ là Hausdorff khi và chỉ khi H đóng trong G.

H là một lớp tương đương đối với quan hệ $x^{-1}y \in H$ và do đó, nếu $G/H$ là Hausdorff, thì H đóng trong G. Ngược lại, nếu H đóng, thì đồ thị của quan hệ này đóng trong $G \times G$, vì nó là ảnh ngược của H qua ánh xạ liên tục $(x, y) \to x^{-1}y$. Vì quan hệ $x^{-1}y \in H$ là mở, suy ra từ Chương I, § 8, no. 3, Mệnh đề 8 rằng $G/H$ là Hausdorff.

#### Mệnh đề 14 {#top-iii-s2-prop-14 .statement}

Cho G là một nhóm tôpô và H là một nhóm con của G. Khi đó không gian thuần nhất $G/H$ là rời rạc khi và chỉ khi H mở trong G.

Vì các ảnh ngược trong G của các điểm của $G/H$ qua ánh xạ chính tắc là các lớp ghép $xH$ ($x \in G$); và các tập này mở trong G khi và chỉ khi H mở trong G.

Cho X là một không gian tôpô trên đó một nhóm tôpô G tác động liên tục và bắc cầu; khi đó X là một không gian thuần nhất của G (theo nghĩa đại số). Cho x là một điểm của X, H_x là nhóm ổn định của nó. Ánh xạ toàn ánh liên tục s → s.x từ G lên X phân tích một cách chính tắc thành

$$
G \xrightarrow{f_x} G/H_x \xrightarrow{g_x} X
$$

trong đó f_x là ánh xạ chính tắc từ G lên không gian thuần nhất G/H_x, và g_x là song ánh s.H_x → s.x từ G/H_x lên X; hơn nữa (Chương I, § 3, no. 4, Mệnh đề 6) g_x là một ánh xạ liên tục. Nhưng g_x không nhất thiết là một phép đồng phôi từ G/H_x lên X (Bài tập 29). Nếu g_x là một phép đồng phôi với mỗi x ∈ X, thì ta nói X là một không gian thuần nhất tôpô (của nhóm tôpô G); để được như vậy, điều kiện cần và đủ là, với mỗi x ∈ E, ánh xạ s → s.x từ G vào X phải là mở.

#### Mệnh đề 15 {#top-iii-s2-prop-15 .statement}

Cho X là một không gian tôpô trên đó một nhóm tôpô G tác động liên tục và bắc cầu. Để X là một không gian thuần nhất tôpô (đối với G), chỉ cần tồn tại một điểm x_0 ∈ X sao cho ánh xạ s → s.x_0 biến mỗi lân cận của e trong G thành một lân cận của x_0 trong X.

Mọi x ∈ X đều có thể viết dưới dạng x = t.x_0 với một t ∈ G nào đó. Nếu V là một lân cận của e, thì V.x = (Vt).x_0 là một lân cận của x, vì ta có thể viết (Vt).x_0 = t((t^{-1}Vt).x_0), và mệnh đề này suy ra từ các sự kiện rằng t^{-1}Vt là một lân cận của e trong G và y → t.y là một phép đồng phôi của X lên chính nó (no. 4, Bổ đề 1). Suy ra rằng nếu U là một tập con mở bất kỳ của G và x là một điểm bất kỳ của X, thì U.x là mở trong X; vì nếu t ∈ U, thì t^{-1}U là một lân cận của e, do đó (t^{-1}U).x là một lân cận của x, và t.((t^{-1}U).x) = U.x là một lân cận của t.x. Vậy U.x là mở trong X, do đó ánh xạ s → s.x từ G vào X là mở. Điều này hoàn tất chứng minh.

### 6. NHÓM THƯƠNG

#### Mệnh đề 16 {#top-iii-s2-prop-16 .statement}

Cho G là một nhóm tôpô và H là một nhóm con chuẩn tắc của G. Khi đó thương theo H của tôpô của G tương thích với cấu trúc nhóm của G/H.

Nếu x → x̂ là ánh xạ chính tắc từ G lên G/H, thì ta phải chứng minh rằng (x̂, ŷ) → x̂ŷ^{-1} là một ánh xạ liên tục từ (G/H) × (G/H) vào G/H. Vì quan hệ tương đương x^{-1}y ∈ H là mở (no. 4, Bổ đề 2), chỉ cần chứng minh rằng (x, y) → x̂ŷ^{-1} là một ánh xạ liên tục từ G × G vào G/H (Chương I, § 5, no. 3, Hệ quả của Mệnh đề 8, và § 3, no. 4, Mệnh đề 6). Nhưng (x, y) → x̂ŷ^{-1} là hợp thành của các ánh xạ liên tục x → x̂ và (x, y) → xy^{-1}, nên là liên tục.

Mỗi khi trong phần sau ta xét một nhóm thương $G/H$ của một nhóm tôpô $G$ như một nhóm tôpô, luôn hiểu rằng tôpô của $G/H$ là thương theo $H$ của tôpô của $G$, trừ khi có tuyên bố rõ ràng ngược lại.

#### Mệnh đề 17 {#top-iii-s2-prop-17 .statement}

*Cho $\varphi$ là ánh xạ chính tắc từ một nhóm tôpô $G$ lên một nhóm thương $G/H$. Nếu $\mathcal{B}$ là một hệ cơ bản các lân cận của $e$ trong $G$, thì $\varphi(\mathcal{B})$ là một hệ cơ bản các lân cận của phần tử đơn vị $\varphi(e)$ của $G/H$.*

Đây là một trường hợp riêng của Mệnh đề 5 của Chương I, § 5, no. 3.

Các Mệnh đề 13 và 14 cho ta, đặc biệt, đối với các nhóm thương:

#### Mệnh đề 18 {#top-iii-s2-prop-18 .statement}

*Cho $G$ là một nhóm tôpô và cho $H$ là một nhóm con chuẩn tắc của $G$.
a) *Nhóm thương $G/H$ là Hausdorff khi và chỉ khi $H$ đóng trong $G$.
b) *Nhóm thương $G/H$ là rời rạc khi và chỉ khi $H$ mở trong $G$.*

Nếu $G$ là một nhóm tôpô và $N$ là bao đóng của $\{e\}$ trong $G$, thì $N$ là một nhóm con chuẩn tắc đóng của $G$ (no. 1, Mệnh đề 1), do đó $G/N$ là Hausdorff; $G/N$ được gọi là *nhóm Hausdorff liên kết với* $G$.

#### Mệnh đề 19 {#top-iii-s2-prop-19 .statement}

*Nếu $H$ là một nhóm con chuẩn tắc rời rạc của một nhóm tôpô $G$, thì $G/H$ đẳng cấu địa phương với $G$.*

Cho $V$ là một lân cận của $e$ trong $G$ không chứa điểm nào của $H$ ngoài $e$, và cho $W$ là một lân cận mở đối xứng của $e$ trong $G$ sao cho $W^2 \subset V$. Khi đó hạn chế lên $W$ của ánh xạ chính tắc $\varphi$ từ $G$ lên $G/H$ là *đơn ánh*; thật vậy, nếu $x, y \in W$ và $\varphi(x) = \varphi(y)$, thì $x^{-1}y \in W^2 \subset V$ và $x^{-1}y \in H$, nên $x = y$. Theo Mệnh đề 17 suy ra rằng hạn chế của $\varphi$ lên $W$ là một đồng phôi từ $W$ lên $\varphi(W)$; hơn nữa, vì $\varphi(xy) = \varphi(x)\varphi(y)$ với mọi $x, y \in W$, ta kết luận rằng $G$ và $G/H$ đẳng cấu địa phương (§ 1, no. 3, Mệnh đề 3).

### 7. NHÓM CON VÀ NHÓM THƯƠNG CỦA MỘT NHÓM THƯƠNG

Cho $G$ là một nhóm tôpô, cho $H$ là một nhóm con chuẩn tắc của $G$, và cho $\varphi : G \to G/H$ là ánh xạ chính tắc. Ta biết rằng nếu $A'$ là một nhóm con của $G/H$, thì $\overline{\varphi}(A')$ là một nhóm con của $G$ chứa $H$. Ngược lại, nếu $A$ là một nhóm con của $G$, thì $\varphi(A)$ là một nhóm con của $G/H$; hơn nữa, có một song ánh chính tắc từ nhóm thương $A/(A \cap H)$ lên nhóm con $\varphi(A)$ của $G/H$, và một song ánh chính tắc từ $\varphi(A)$ lên nhóm thương $AH/H$, và cả hai song ánh này đều là các đẳng cấu *đối với các cấu trúc nhóm*.

#### Mệnh đề 20 {#top-iii-s2-prop-20 .statement}

Cho $A$ là một nhóm con của một nhóm tôpô $G$, cho $H$ là một nhóm con chuẩn tắc của $G$, và cho $\varphi$ ký hiệu ánh xạ chính tắc của $G$ lên $G/H$. Khi đó song ánh chính tắc từ $\varphi(A)$ lên $AH/H$ là một đẳng cấu của các nhóm tôpô.

Điều này suy ra từ các nhận xét trước đó, và từ Mệnh đề 10 của no. 4.

Song ánh chính tắc từ $A/(A \cap H)$ lên $\varphi(A)$ là một đồng cấu liên tục, vì nó thu được từ hạn chế của $\varphi$ lên $A$ khi chuyển qua các thương; nhưng nói chung các nhóm tôpô $A/(A \cap H)$ và $AH/H$ không đẳng cấu (xem § 4, no. 1, Mệnh đề 1, Hệ quả 3).

\* Chẳng hạn, lấy $G$ là nhóm cộng $\mathbf{R}$ của các số thực, lấy $H$ là nhóm $\mathbf{Z}$ của các số nguyên, và lấy $A$ là nhóm $\theta \mathbf{Z}$ gồm các bội số nguyên của một số vô tỉ $\theta$. Khi đó $A \cap H = \{0\}$, nên $A/(A \cap H)$ là một nhóm rời rạc, đẳng cấu với $\mathbf{Z}$; mặt khác, $A + H$ trù mật trong $\mathbf{R}$ (như ta sẽ thấy ở Chương V, § 1, no. 1, Mệnh đề 1), do đó $(A + H)/H$, địa phương đẳng cấu với $A + H$ (no. 6, Mệnh đề 19), không phải là một nhóm rời rạc và vì thế không đẳng cấu với $A/(A \cap H)$. \*

Tuy nhiên, ta có mệnh đề sau:

#### Mệnh đề 21 {#top-iii-s2-prop-21 .statement}

Cho $G$ là một nhóm tôpô, $G_0$ là một nhóm con trù mật của $G$, $H_0$ là một nhóm con chuẩn tắc của $G_0$, $H$ là bao đóng của $H_0$ trong $G$ và $\varphi$ là ánh xạ chính tắc $G \to G/H$. Khi đó song ánh chính tắc $G_0/H_0 \to \varphi(G_0)$ là một đẳng cấu của nhóm tôpô $G_0/H_0$ lên một nhóm con trù mật của $G/H$.

Vì $H_0 = H \cap G_0$, chỉ cần chứng minh rằng nếu $U_0$ là một tập con mở bất kỳ của $G_0$ được bão hòa đối với quan hệ $x^{-1}y \in H_0$, thì $U_0$ là giao của $G_0$ với một tập con mở của $G$ được bão hòa đối với quan hệ $x^{-1}y \in H$ (Chương I, § 3, no. 6, Mệnh đề 10). Cho $U$ là một tập con mở của $G$ sao cho $U_0 = U \cap G_0$. Vì $U_0 = U_0 H_0$, dễ thấy rằng $U_0 = U H_0 \cap G_0$; nhưng $U H_0$ là mở trong $G$, nên ta có thể giả sử rằng $U = U H_0$. Tập hợp $U H$ là mở trong $G$ và được bão hòa đối với quan hệ $x^{-1}y \in H$; do đó mệnh đề sẽ được chứng minh nếu ta chỉ ra rằng $U H \cap G_0 = U_0$. Bây giờ, nếu $u \in U$ và $h \in H$ sao cho $u h \in G_0$, thì tồn tại một lân cận đối xứng $V$ của $e$ trong $G$ sao cho $u V \subset U$; vì $V h$ là một lân cận của $h$ trong $G$, nên tồn tại $z \in V$ sao cho $z h \in H_0$. Nhưng khi đó ta có $u z^{-1} \in U$, và $u h = (u z^{-1})(z h)$; vì thế $U H \cap G_0 \subset U H_0$. Nhưng $U H_0 = U$, do đó $U H \cap G_0 \subset U \cap G_0 = U_0$. Điều này hoàn tất chứng minh.

Cho $G$ là một nhóm tôpô tác động liên tục lên một không gian tôpô $X$, và cho $K$ là một nhóm con chuẩn tắc của $G$ được chứa trong nhóm ổn định của mỗi điểm của $X$. Khi đó, với mỗi $x \in X$, quan hệ $s \equiv t \pmod{K}$ kéo theo $s.x = t.x$, và chuyển qua thương ta định nghĩa một ánh xạ $s \to s.x$ từ $G/K$ vào $X$. Người ta kiểm tra ngay lập tức rằng đối với phép toán ngoài $(s', x) \to s'.x$, X có G/K làm một nhóm các toán tử. Hơn nữa, G/K tác động liên tục lên X đối với luật này; vì quan hệ đẳng thức trên X và quan hệ $s \equiv t \pmod{K}$ trên G đều là những quan hệ tương đương mở, và do đó kết quả suy ra từ tính liên tục của ánh xạ

$$(s, x) \to s'.x = s.x$$

từ $G \times X$ vào X (Chương I, § 5, no. 3, Hệ quả của Mệnh đề 8, và § 3, no. 4, Mệnh đề 6).

Bây giờ cho G là một nhóm tôpô tác động liên tục lên một không gian tôpô X, và cho H là một nhóm con chuẩn tắc bất kỳ của G; khi đó H tác động liên tục lên X. Gọi S là quan hệ tương đương do H xác định trên X; khi đó S là mở (no. 4, Bổ đề 2). Quan hệ S tương thích với nhóm G (no. 4); vì nếu $y \equiv x \pmod{S}$ thì tồn tại $t \in H$ sao cho $y = t.x$; do đó với mọi $s \in G$ ta có $s.y = (sts^{-1}).s.x$, và $sts^{-1} \in H$ vì H là chuẩn tắc trong G; vậy $s.y \equiv s.x \pmod{S}$. Nếu $\psi$ là ánh xạ chính tắc của X lên X/S, thì nhóm G do đó tác động liên tục lên X/S đối với phép toán ngoài

$$(s, \psi(x)) \to \psi(s.x)$$

(no. 4, Mệnh đề 11). Hơn nữa, nhóm H được chứa trong nhóm ổn định của mỗi điểm của X/S; như đã thấy ở trên, G/H tác động liên tục lên $X/S = X/H$ đối với phép toán ngoài $(s', \psi(x)) \to \psi(s.x)$. Nếu R ký hiệu quan hệ tương đương trên X do G xác định, thì quan hệ S kéo theo R, và quan hệ tương đương R/S trên X/S là quan hệ được xác định bởi nhóm G/H. Vậy nên (Chương I, § 3, no. 4, Mệnh đề 7):

#### Mệnh đề 22 {#top-iii-s2-prop-22 .statement}

*Cho G là một nhóm tôpô tác động liên tục lên một không gian tôpô X, và cho H là một nhóm con chuẩn tắc của G. Khi đó song ánh chính tắc từ X/G lên $(X/H)/(G/H)$ là một đồng phôi.*

#### Hệ quả {#top-iii-s2-n7-cor-1 .statement}

*Cho G là một nhóm tôpô, H là một nhóm con chuẩn tắc của G, và K là một nhóm con chuẩn tắc của G chứa H. Khi đó song ánh chính tắc từ G/K lên $(G/H)/(K/H)$ là một đẳng cấu của các nhóm tôpô.*

Ta đã biết rằng song ánh này là một đẳng cấu nhóm, và Mệnh đề 22 (áp dụng cho nhóm K tác động bên phải lên G) cho thấy rằng nó là một đồng phôi.

### 8. ĐỒNG CẤU LIÊN TỤC VÀ CẤU XẠ NGẶT

#### Mệnh đề 23 {#top-iii-s2-prop-23 .statement}

*Một đồng cấu f từ một nhóm tôpô G vào một nhóm tôpô $G'$ là liên tục trên G khi và chỉ khi nó liên tục tại một điểm của G.*

Giả sử $f$ liên tục tại một điểm $a \in G$; khi đó nếu $V'$ là một lân cận bất kỳ của $f(a)$, thì $V = \overline{f^{-1}}(V')$ là một lân cận của $a$. Do đó nếu $x$ là một điểm bất kỳ của $G$, ta có
$$
f(xa^{-1}V) = f(x)[f(a)]^{-1}f(V) \subset f(x)[f(a)]^{-1}V',
$$
và vì thế $f$ liên tục tại $x$.

Một đồng cấu liên tục từ một nhóm tôpô $G$ vào một nhóm tôpô $G'$ còn được gọi là một *cấu xạ* từ $G$ vào $G'$ đối với các cấu trúc nhóm tôpô.

Cho $f$ là một đồng cấu liên tục của một nhóm tôpô $G$ vào một nhóm tôpô $G'$; ảnh ngược $H = \overline{f^{-1}}(e')$ của phần tử đơn vị $e'$ của $G'$ là một *nhóm con chuẩn tắc* của $G$, và $f(G)$ là một *nhóm con* của $G'$. Xét sự phân tích chính tắc $f = \psi \circ \dot{f} \circ \varphi$, trong đó $\varphi$ là ánh xạ chính tắc $G \to G/H$, $\psi$ là đơn ánh chính tắc $f(G) \to G'$ và sau cùng $\dot{f}$ là một *đồng cấu liên tục song ánh* của nhóm thương $G/H$ lên nhóm con $f(G)$ (Chương I, § 3, no. 5); người ta nói rằng $\dot{f}$ là đồng cấu song ánh *liên kết* với $f$. Nói chung, $\dot{f}$ không phải là một đẳng cấu của các nhóm tôpô.

Ví dụ, cho $G'$ là một nhóm tôpô không rời rạc, và $G$ là nhóm tôpô thu được bằng cách trang bị cho $G'$ tôpô rời rạc; khi đó ánh xạ đồng nhất từ $G$ vào $G'$ là một đồng cấu liên tục song ánh, nhưng không song liên tục.

#### Định nghĩa 1 {#top-iii-s2-def-1 .statement}

*Một đồng cấu liên tục của một nhóm tôpô $G$ vào một nhóm tôpô $G'$ được gọi là một cấu xạ ngặt của $G$ vào $G'$ nếu đồng cấu song ánh $\dot{f}$ của $G/\overline{f^{-1}}(e')$ lên $f(G)$, liên kết với $f$, là một đẳng cấu của các nhóm tôpô (nói cách khác, nếu $\dot{f}$ là song liên tục).*

Vì vậy một đẳng cấu của một nhóm tôpô $G$ lên một nhóm tôpô $G'$ là một cấu xạ ngặt song ánh của $G$ lên $G'$.

#### Mệnh đề 24 {#top-iii-s2-prop-24 .statement}

*Cho $f$ là một đồng cấu liên tục của một nhóm tôpô $G$ vào một nhóm tôpô $G'$. Khi đó ba mệnh đề sau là tương đương:*
a) $f$ *là một cấu xạ ngặt.*
b) *Ảnh theo $f$ của mọi tập hợp mở trong $G$ là một tập hợp mở trong $f(G)$.*
c) *Ảnh theo $f$ của mọi lân cận của phần tử đơn vị trong $G$ là một lân cận của phần tử đơn vị trong $G'$.*

Theo Bổ đề 2 của no. 4, tính tương đương của a) và b) suy ra ngay lập tức từ các định nghĩa (Chương I, § 5, no. 3, Mệnh đề 5). Tính tương đương của b) và c) là một trường hợp riêng của Mệnh đề 15 của no. 5, nếu ta nhận thấy rằng $G$ tác động liên tục trên $f(G)$ bởi luật ngoài $(s, f(t)) \to f(st)$.

#### Nhận xét 1 {#top-iii-s2-n8-rem-1 .statement}

Từ điều kiện b) của Mệnh đề 24 suy ra rằng mọi đồng cấu liên tục của một nhóm tôpô vào một nhóm rời rạc đều là một cấu xạ ngặt.

Nếu G compact và $f(G)$ là Hausdorff, thì đồng cấu song ánh $f$ liên kết với $f$ là song liên tục (Chương I, § 10, no. 2, Định lý 1, Hệ quả 2, và no. 1, Mệnh đề 5, Hệ quả 4). Do đó mọi đồng cấu liên tục của một nhóm compact vào một nhóm Hausdorff đều là một cấu xạ ngặt.

#### Nhận xét 2 {#top-iii-s2-n8-rem-2 .statement}

Cho $f$ là một cấu xạ ngặt từ G vào $G'$ và $g$ là một cấu xạ ngặt từ $G'$ vào $G''$. Nếu $f$ toàn ánh hoặc nếu $g$ đơn ánh, thì suy ra ngay lập tức từ Mệnh đề 24 rằng $g \circ f$ là một cấu xạ ngặt từ G vào $G''$. Nhưng kết luận này không còn nhất thiết đúng nữa nếu không điều kiện nào trong hai điều kiện trước được thỏa mãn, ngay cả khi $f$ đơn ánh và $g$ toàn ánh (Bài tập 19).

#### Nhận xét 3 {#top-iii-s2-n8-rem-3 .statement}

Cho $f$ là một đồng cấu liên tục từ một nhóm tôpô G vào một nhóm tôpô $G'$, và cho H là một nhóm con chuẩn tắc của G. $f$ cảm sinh một đồng cấu $g$ từ nhóm $G/H$ lên nhóm thương $f(G)/f(H)$. Đồng cấu này $g$ là liên tục. Hơn nữa, nếu $f$ là một cấu xạ ngặt từ G vào $G'$, thì $g$ là một cấu xạ ngặt từ $G/H$ lên $f(G)/f(H)$; thật vậy, nếu U là mở trong $G/H$, và nếu $\varphi$ (tương ứng $\varphi'$) ký hiệu ánh xạ chính tắc từ G lên $G/H$ [tương ứng từ $f(G)$ lên $f(G)/f(H)$], thì ta có $g(u) = \varphi'(f(\overline{\varphi}^{-1}(u)))$, và vì $\overline{\varphi}^{-1}(u)$ là mở trong G, suy ra $g(u)$ là mở trong $f(G)/f(H)$, điều đó chứng minh mệnh đề của chúng ta.

### 9. TÍCH CỦA CÁC NHÓM TÔPÔ

Cho $(G_i)_{i \in I}$ là một họ các nhóm tôpô. Khi đó ta có thể định nghĩa một cấu trúc nhóm trên tập hợp tích

$$
G = \prod_{i \in I} G_i
$$

(tích của các cấu trúc nhóm của các $G_i$) bằng cách định nghĩa $(x_i).(y_i) = (x_i y_i)$. Nếu $e_i$ là phần tử đơn vị của $G_i$, thì $e = (e_i)$ là phần tử đơn vị của G, và ta có $(x_i)^{-1} = (x_i^{-1})$. Tôpô tích (Chương I, § 2, no. 3) của các tôpô của các $G_i$ là tương thích với cấu trúc nhóm này. Thật vậy, ánh xạ $((x_i), (y_i)) \to (x_i, y_i^{-1})$ từ $G \times G$ vào G là hợp thành của ánh xạ $((x_i, y_i)) \to (x_i y_i^{-1})$ từ

$$
\prod_{i \in I} G_i \times G_i \text{ vào } G,
$$

và ánh xạ chính tắc $((x_i), (y_i)) \to ((x_i, y_i))$ từ

$$
G \times G \text{ lên } \prod_{i \in I} (G_i \times G_i);
$$

và cả hai ánh xạ này đều liên tục (Chương I, § 4, no. 1, Hệ quả 1 của Mệnh đề 1, và Mệnh đề 2).

#### Định nghĩa 2 {#top-iii-s2-def-2 .statement}

*Nhóm tôpô thu được bằng cách trang bị cho tập hợp tích*

$$
G = \prod_{i \in I} G_i
$$

*cấu trúc nhóm là tích của các cấu trúc nhóm của các $G_i$ và tôpô là tích của các tôpô của các $G_i$ được gọi là tích của các nhóm tôpô $G_i$.*

Nếu $(J_x)_{x \in K}$ là một *phân hoạch* của $I$, thì $G$ đẳng cấu với tích của các nhóm tôpô $\prod_{i \in J_x} G_i$ (tính kết hợp của tích).

Nếu $H_i$ là một nhóm con của $G_i$, thì tích các nhóm tôpô $H_i$ đẳng cấu với nhóm con $\prod_{i \in J} H_i$ của $\prod_{i \in I} G_i$. Đặc biệt, nếu $J$ là một tập con bất kỳ của $I$, và $J' = C J$, thì nhóm tôpô $\prod_{i \in J} G_i$ đẳng cấu với nhóm con chuẩn tắc $G'_J = (\prod_{i \in J} G_i) \times (\prod_{i \in J'} \{e_i\})$ của $G$. Vì phép chiếu của mọi tập mở là một tập mở, phép chiếu $\mathrm{pr}_J$ của $G$ lên $\prod_{i \in J} G_i$ là một *cấu xạ ngặt*, và do đó nhóm thương $G/G'$ đẳng cấu với $G'_J$; $G$ đẳng cấu với tích $G'_J \times (G/G'_J)$.

#### Mệnh đề 25 {#top-iii-s2-prop-25 .statement}

*Cho $(G_i)_{i \in I}$ là một họ các nhóm tôpô, và cho $H$ là nhóm con chuẩn tắc của $G = \prod_{i \in I} G_i$ gồm mọi $x = (x_i)$ sao cho các $x_i$ bằng phần tử đơn vị $e_i$ của $G_i$ trừ ra chỉ với một số hữu hạn chỉ số. Khi đó nhóm con $H$ trù mật trong $G$.*

Đây là một trường hợp riêng của Chương I, § 4, no. 3, Mệnh đề 8.

Cho $(X_i)_{i \in I}$ là một họ các không gian tôpô, và với mỗi $i \in I$ cho $G_i$ là một nhóm tôpô tác động liên tục trên $X_i$. Rõ ràng là khi đó nhóm tích $G = \prod_{i \in I} G_i$ tác động liên tục trên không gian tích $X = \prod_{i \in I} X_i$ theo luật

$$
((s_i), (x_i)) \to (s_i \cdot x_i)
$$

(Chương I, § 4, no. 1, Mệnh đề 1, Hệ quả 1, và Mệnh đề 2). Hơn nữa quỹ đạo dưới tác động của $G$ của một điểm $x = (x_i)$ của $X$ là tích của các quỹ đạo của các $x_i$ (đối với các nhóm $G_i$). Gọi $\varphi_i$ là ánh xạ chính tắc từ $X_i$ lên $X_i/G_i$, và gọi $\varphi = (\varphi_i)$ là ánh xạ tích từ $X$ lên $\prod_{i \in I} (X_i/G_i)$; khi đó nhận xét trên cho thấy song ánh liên kết với $\varphi$ một cách chính tắc ánh xạ không gian quỹ đạo $X/G$ lên $\prod_{i \in I} (X_i/G_i)$. Hơn nữa:

#### Hệ quả {#top-iii-s2-n9-cor-1 .statement}

*Cho* $(G_i)_{i \in I}$ *là một họ các nhóm tôpô, và với mỗi* $i \in I$ *cho* $H_i$ *là một nhóm con chuẩn tắc của* $G_i$; *gọi* $\varphi_i$ *là ánh xạ chính tắc từ* $G_i$ *lên* $G_i/H_i$. *Đặt* $G = \prod_{i \in I} G_i, \ H = \prod_{i \in I} H_i$. *Khi đó đồng cấu song ánh từ* $G/H$ *lên* $\prod_{i \in I} (G_i/H_i)$ *liên kết với đồng cấu liên tục* $(x_i) \to (\varphi_i(x_i))$ *là một đẳng cấu các nhóm tôpô.*

Vì đồng cấu này là một đẳng cấu của các cấu trúc nhóm.

#### Nhận xét {#top-iii-s2-n9-rem-1 .statement}

Nếu $G$ là một nhóm tôpô *giao hoán*, viết theo lối cộng, thì ánh xạ $(x, y) \to x + y$ từ $G \times G$ lên $G$ là một *cấu xạ ngặt*. Thật vậy, vì $(x + x') + (y + y') = (x + y) + (x' + y')$ nên nó là một *đồng cấu* từ $G \times G$ lên $G$; ngoài ra nó liên tục, và ảnh của một lân cận $V \times V$ của phần tử không trong $G \times G$ qua ánh xạ này là lân cận $V + V$ của phần tử không trong $G$.

### 10. TÍCH NỬA TRỰC TIẾP

Cho $L, N$ là hai nhóm con của một nhóm $G$, sao cho $LN = NL$; khi đó $LN$ là một *nhóm con* của $G$, vì

$$
(LN)(LN)^{-1} = LNN^{-1}L^{-1} = LNL = LLN = LN
$$

Hơn nữa, ánh xạ $\varphi : (x, y) \to xy$ từ $N \times L$ vào $G$ là *đơn ánh* khi và chỉ khi $N \cap L = \{e\}$. Thật vậy, hiển nhiên nếu $\varphi$ là đơn ánh thì $N \cap L = \{e\}$; và ngược lại, quan hệ $x'y' = xy$, với $x, x' \in N$ và $y, y' \in L$, suy ra $x^{-1}x' = {yy'}^{-1} \in N \cap L$; do đó nếu $N \cap L = \{e\}$ thì $\varphi$ là đơn ánh. Vậy $\varphi$ là *song ánh* khi và chỉ khi $LN = G$ và $N \cap L = \{e\}$.

Nếu $N$ là một nhóm con *chuẩn tắc* của $G$ (hoặc nói chung hơn, là chuẩn tắc trong một nhóm con nào đó của $G$ chứa $N \cup L$), thì điều kiện $LN = NL$ tự động được thỏa mãn. Hơn nữa, với mỗi $y \in L$ ánh xạ $\sigma_y : x \to yxy^{-1}$ là một *tự đẳng cấu* của nhóm $N$, và với hai phần tử bất kỳ $u, v$ của $L$ ta có

$$(1)$$
$$
\sigma_{uv} = \sigma_u \circ \sigma_v;
$$

và với mọi $x, x'$ trong $\mathbf{N}$ và $y, y'$ trong $\mathbf{L}$ ta cũng có

$$(2)$$
$$(xy)(x'y') = (x\sigma_y(x'))(yy').$$

Ngược lại:

#### Mệnh đề 27 {#top-iii-s2-prop-27 .statement}

*Cho $\mathbf{N}$ và $\mathbf{L}$ là hai nhóm, $e'$ và $e''$ là các phần tử đơn vị tương ứng của chúng. Giả sử rằng ta được cho một đồng cấu $y \to \sigma_y$ từ $\mathbf{L}$ vào nhóm $\Gamma$ các tự đẳng cấu của $\mathbf{N}$. Khi đó:*

1) *Trên tập hợp tích $S = \mathbf{N} \times \mathbf{L}$, luật hợp thành trong*
$$(3)$$
$$(x, y)(x', y') = (x\sigma_y(x'), yy')$$
*xác định một cấu trúc nhóm, mà đối với nó $j_1 : x \to (x, e'')$ là một đẳng cấu từ $\mathbf{N}$ lên một nhóm con chuẩn tắc của $S$, $j_2 : y \to (e', y)$ là một đẳng cấu từ $\mathbf{L}$ lên một nhóm con của $S$, và $\mathrm{pr}_2 : S \to \mathbf{L}$ là một đồng cấu toàn ánh có hạt nhân là $j_1(\mathbf{N})$ và sao cho $\mathrm{pr}_2 \circ j_2$ là tự đẳng cấu đơn vị của $\mathbf{L}$.*

2) *Cho $f : \mathbf{N} \to G$, $g : \mathbf{L} \to G$ là hai đồng cấu vào một nhóm $G$, sao cho*
$$(4)$$
$$f(\sigma_y(x)) = g(y)f(x)g(y^{-1})$$
*với mọi $x \in \mathbf{N}$ và mọi $y \in \mathbf{L}$. Khi đó tồn tại một đồng cấu duy nhất $h : S \to G$ sao cho $f = h \circ j_1$, và $g = h \circ j_2$.*

Nếu $x, x', x''$ là các phần tử của $\mathbf{N}$ và $y, y', y''$ là các phần tử của $\mathbf{L}$, thì
$$
((x, y)(x', y'))(x'', y'') = (x\sigma_y(x'), yy')(x'', y'')
= (x\sigma_y(x')\sigma_{y'}(x''), yy'y'')
$$
và
$$
(x, y)((x', y')(x'', y'')) = (x, y)(x'\sigma_{y'}(x''), y'y'')
= (x\sigma_y(x'\sigma_{y'}(x'')), yy', y'')
$$
và do đó tính kết hợp của luật (3) suy ra từ các sự kiện rằng $y \to \sigma_y$ là một đồng cấu từ $\mathbf{L}$ vào $\Gamma$ và rằng $\sigma_y$ là một tự đẳng cấu của $\mathbf{N}$. Rõ ràng $(e', e'')$ là phần tử đơn vị của (3), và sau cùng
$$(x, y)(\sigma_{y^{-1}}(x^{-1}), y^{-1}) = (\sigma_{y^{-1}}(x^{-1}), y^{-1})(x, y) = (e', e'')$$
nên $(x, y)$ có một phần tử nghịch đảo trong $S$. Các mệnh đề khác của 1) là rõ ràng. Mặt khác, vì $(x, y) = (x, e'') (e', y)$, một đồng cấu $h$ thỏa mãn các điều kiện của 2) tất yếu phải thỏa mãn
$$h(x, y) = f(x)g(y),$$
do đó là duy nhất nếu nó tồn tại; hơn nữa từ (4) suy ra ngay lập tức rằng
$$f(x\sigma_y(x'))g(yy') = f(x)g(y)f(x')g(y^{-1})g(y)g(y') = f(x)g(y)f(x')g(y')$$

điều đó chứng tỏ rằng ánh xạ $(x, y) \to f(x)g(y)$ quả thật là một đồng cấu từ S vào G thỏa mãn các điều kiện của 2).

#### Hệ quả {#top-iii-s2-n10-cor-1 .statement}

*Đồng cấu h được xác định trong 2) của Mệnh đề 27 là đơn ánh khi và chỉ khi f và g là đơn ánh và $f(N) \cap g(L) = \{e\}$; và h là toàn ánh khi và chỉ khi $f(N)g(L) = G$.*

Vì $h(x, y) = f(x)g(y)$, mệnh đề thứ hai là hiển nhiên; hơn nữa từ (4) suy ra rằng $f(N)g(L) = g(L)f(N)$, và mệnh đề thứ nhất suy ra từ các nhận xét ở đầu tiểu tiết này.

Nhóm S được xác định trong Mệnh đề 27 được gọi là *tích nửa trực tiếp ngoài* của N và L (đối với $\sigma$); nói chung chúng ta sẽ đồng nhất N (tương ứng L) với nhóm con chuẩn tắc $j_1(N)$ [tương ứng nhóm con $j_2(L)$] của S. Nếu $\sigma_y$ là phần tử đơn vị của $\Gamma$ với mọi $y \in L$, ta thu lại khái niệm thông thường về *tích* của hai nhóm.

Bây giờ cho G là một nhóm, và cho L và N là hai nhóm con của G sao cho $LN = NL$ và sao cho N là *chuẩn tắc* trong NL, nên với mỗi $y \in L$, $\sigma_y : x \to yxy^{-1}$ là một tự đẳng cấu của N, và $y \to \sigma_y$ là một đồng cấu từ L vào nhóm tự đẳng cấu $\Gamma$ của N. Khi đó suy ra từ Mệnh đề 27 rằng nếu S là tích nửa trực tiếp ngoài của N và L (ứng với $\sigma$), thì $h : (x, y) \to xy$ là một *đồng cấu* từ S vào G. h là song ánh khi và chỉ khi ta có $N \cap L = \{e\}$ và $NL = G$ (Hệ quả của Mệnh đề 27); khi đó G được gọi là *tích nửa trực tiếp* của nhóm con chuẩn tắc N của nó và nhóm con L của nó, và ta thường đồng nhất G với S qua h.

#### Mệnh đề 28 {#top-iii-s2-prop-28 .statement}

*Cho L, N là hai nhóm tôpô, cho $y \to \sigma_y$ là một đồng cấu từ L vào nhóm các tự đẳng cấu $\Gamma$ của cấu trúc nhóm (phi tôpô) của N; và giả sử rằng ánh xạ $(x, y) \to \sigma_y(x)$ từ $N \times L$ vào N là liên tục. Khi đó:

1) *Trên tích nửa trực tiếp ngoài S của N và L, ứng với $\sigma$, tích các tôpô của N và L là tương thích với cấu trúc nhóm; các đơn cấu chính tắc $j_1 : N \to S$ và $j_2 : L \to S$ là các đẳng cấu của các nhóm tôpô N và L tương ứng lên các nhóm con $j_1(N)$ và $j_2(L)$ của S, và $pr_2$ là một cấu xạ ngặt từ S lên L.*

2) *Cho $f : N \to G$ và $g : L \to G$ là hai đồng cấu liên tục vào một nhóm tôpô G, thỏa mãn (4); khi đó đồng cấu*

$$
(x, y) \to f(x)g(y)
$$

*từ S vào G là liên tục.*

Điều này là một hệ quả ngay lập tức của các định nghĩa và của các tính chất của tôpô tích.

Nhóm tôpô S được định nghĩa như vậy được gọi là tích nửa trực tiếp tôpô ngoài của N và L (ứng với σ); lưu ý rằng điều kiện đặt lên σ kéo theo rằng L tác động liên tục bên trái lên N theo phép toán ngoài $(x, y) \to \sigma_y(x)$ [no. 4].

Bây giờ cho G là một nhóm tôpô và cho N và L là hai nhóm con của G sao cho G là tích nửa trực tiếp của N và L, xét như một nhóm phi tôpô; khi đó hiển nhiên là ánh xạ $(x, y) \to \sigma_y(x)$ là liên tục trên $N \times L$, và đồng cấu song ánh chính tắc

$$
h : (x, y) \to xy
$$

từ S lên G là liên tục. Nhưng đồng cấu này không nhất thiết là song liên tục; khi nó là song liên tục, G được gọi là tích nửa trực tiếp tôpô của N và L. Để điều đó xảy ra thì điều kiện cần và đủ là, nếu $p : G \to N$ và $q : G \to L$ là các ánh xạ làm tương ứng với $z \in G$ các phần tử duy nhất $p(z) \in N$ và $q(z) \in L$ sao cho $z = p(z)q(z)$, thì một trong hai ánh xạ $p, q$ là liên tục (khi đó cả hai đều liên tục). Nói như vậy cũng tương đương với việc nói rằng hạn chế lên L của ánh xạ chính tắc $G \to G/N$ là một đẳng cấu của nhóm tôpô L lên nhóm tôpô G/N.

### Bài tập {#top-iii-s2-exercises}

Xem [các bài tập cho § 2](exercises/s2/).
