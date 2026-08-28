---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: I
chapter_title: Lie Algebras
section: 6
section_title: Semi-simple Lie algebras
lang: vi
source: lie-i-iii
pdf_pages: 0068-0086, 0120-0127
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF SEMI-SIMPLE LIE ALGEBRAS
      page: 0
      pdf_page: 68
    - "no": 2
      title: SEMI-SIMPLICITY OF REPRESENTATIONS
      page: 0
      pdf_page: 69
    - "no": 3
      title: SEMI-SIMPLE ELEMENTS AND NILPOTENT ELEMENTS IN SEMI-SIMPLE LIE ALGEBRAS
      page: 0
      pdf_page: 72
    - "no": 4
      title: REDUCTIVE LIE ALGEBRAS
      page: 0
      pdf_page: 74
    - "no": 5
      title: 'APPLICATION: A CRITERION FOR SEMI-SIMPLICITY OF REPRESENTATIONS'
      page: 0
      pdf_page: 76
    - "no": 6
      title: SUBALGEBRAS REDUCTIVE IN A LIE ALGEBRA
      page: 0
      pdf_page: 77
    - "no": 7
      title: EXAMPLES OF SEMI-SIMPLE LIE ALGEBRAS
      page: 0
      pdf_page: 78
    - "no": 8
      title: THE LEVI-MALCEV THEOREM
      page: 0
      pdf_page: 80
    - "no": 9
      title: THE INVARIANTS THEOREM
      page: 0
      pdf_page: 84
    - "no": 10
      title: CHANGE OF BASE FIELD
      page: 0
      pdf_page: 86
statements: 50
exercises: 27
content_sha256: bdb3caedb5662f51a80305eb3132726db81e0e318033307a2040c717da673bd3
translated_from: content/en/lie/I/06_s6_semi_simple_lie_algebras.md
source_content_sha256: b1e634de71044113952c7b93184eddb90c01c9866c2a39749c1000a89ffd9f13
translation_model: gpt-5-6-mini, gpt-5.4, gpt-5-6
translation_run: translate-vi-91c34402
glossary_version: 34
glossary_terms_sha256: 2f0b4e9ffaaa1b6bcb2ecaac9c6a1372820fd4f8bc7bdda9fce8f542c731299c
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 6. ĐẠI SỐ LIE NỬA ĐƠN

*Nhắc lại rằng K ký hiệu một trường có đặc số 0 và mọi đại số Lie đều được giả sử là hữu hạn chiều trên K.*

### 1. ĐỊNH NGHĨA CÁC ĐẠI SỐ LIE NỬA ĐƠN

#### Định nghĩa 1 {#lie-i-s6-def-1 .statement}

*Cho g là một đại số Lie. g được gọi là nửa đơn khi và chỉ khi iđêan giao hoán duy nhất của g là {0}.*

#### Nhận xét {#lie-i-s6-n1-rem-1 .statement}

(1) Đại số {0} là nửa đơn. Một đại số có chiều 1 hoặc 2 không phải là nửa đơn (cf. § 5, no. 1, Ví dụ 1). Tồn tại các đại số nửa đơn có chiều 3 (cf. no. 7).

(2) Một đại số nửa đơn có tâm không và do đó biểu diễn liên hợp của nó là trung thành.

(3) Nếu $g_1, \ldots, g_n$ là các đại số nửa đơn, $g = g_1 \times \cdots \times g_n$ là nửa đơn: vì nếu a là một iđêan giao hoán của g, các phép chiếu của a lên $g_1, \ldots, g_n$ đều rút gọn về {0}.

#### Định lý 1 {#lie-i-s6-thm-1 .statement}

*Cho g là một đại số Lie. Các điều kiện sau là tương đương:*

(a) *g là nửa đơn.*
(b) *Căn r của g là không.*
(c) *Dạng Killing $\beta$ của g là không suy biến.*

*Hơn nữa, một đại số Lie nửa đơn bằng iđêan dẫn xuất của nó.*

(a) $\Rightarrow$ (b): vì nếu $r \neq \{0\}$, đại số dẫn xuất cuối cùng khác không của r là một iđêan giao hoán của g.

(b) $\Rightarrow$ (c): điều này suy ra từ Mệnh đề 5 (b) của § 5, no. 5 (đồng thời chứng minh khẳng định cuối cùng của định lý).

(c) $\Rightarrow$ (a): điều này suy ra từ Mệnh đề 6 (b) của § 4, no. 4.

#### Hệ quả {#lie-i-s6-n1-cor-1 .statement}

*Cho g là một đại số Lie nửa đơn và $\rho$ là một biểu diễn của g trên một không gian vectơ hữu hạn chiều V. Khi đó $\rho(g) \subset \mathfrak{sl}(V)$.*

Dạng tuyến tính $x \mapsto \operatorname{Tr} \rho(x)$ ($x \in g$) bằng không khi x có dạng $[y, z]$ ($y \in g, z \in g$) và do đó trên $\mathcal{D}g = g$.

#### Mệnh đề 1 {#lie-i-s6-prop-1 .statement}

Cho $g$ là một đại số Lie nửa đơn và $\varphi$ là một biểu diễn trung thành hữu hạn chiều của $g$. Khi đó dạng song tuyến tính trên $g$ liên kết với $\varphi$ là không suy biến.

Phần trực giao của $g$ đối với dạng này là một iđêan giải được ($\S 5$, no. 4, Định lý 2) và do đó là không.

#### Hệ quả 1 {#lie-i-s6-prop-1-cor-1 .statement}

Cho $g$ là một đại số Lie, $\beta$ là dạng Killing của nó và $a$ là một đại số con nửa đơn của $g$. Phần trực giao $h$ của $a$ đối với $\beta$ là một không gian con bổ sung của $a$ trong $g$ và $[a, h] \subset h$. Nếu $a$ là một iđêan của $g$, thì h cũng vậy, và khi đó h là toán tử trung tâm hóa của a trong g.

Cho $\beta'$ là hạn chế của $\beta$ lên $a$: đó là dạng song tuyến tính liên kết với biểu diễn $x \mapsto \operatorname{ad}_g x$ của a trên không gian g. Biểu diễn này là trung thành và do đó $\beta'$ không suy biến (Mệnh đề 1). Vì vậy h bổ sung cho a trong g. Mặt khác, nếu $x, y$ thuộc a và $z \in h$, thì

$$
\beta(x, [y, z]) = \beta([x, y], z) = 0,
$$

vì $[x, y] \in a$, và do đó $[y, z] \in h$, điều này chứng tỏ rằng $[a, h] \subset h$. Nếu $a$ là một iđêan của $g$, ta biết rằng $h$ là một iđêan của $g$ ($\S 3$, Mệnh đề 7) và $g$ được đồng nhất với $a \times h$. Vì tâm của $a$ bằng không, bộ trung tâm hóa của $a$ trong $g$ là $h$.

#### Hệ quả 2 {#lie-i-s6-prop-1-cor-2 .statement}

Mọi mở rộng của một đại số Lie nửa đơn bởi một đại số Lie nửa đơn đều là nửa đơn và tầm thường.

Điều này suy ra ngay lập tức từ Hệ quả 1.

#### Hệ quả 3 {#lie-i-s6-prop-1-cor-3 .statement}

Nếu $g$ là nửa đơn, mọi đạo hàm của $g$ đều là nội.

$\operatorname{ad} g$ đẳng cấu với $g$ và do đó là nửa đơn, và là một iđêan của đại số Lie $\delta$ các đạo hàm của $g$ ($\S 1$, Mệnh đề 1). Nếu $D \in \delta$ giao hoán với các phần tử của $\operatorname{ad} g$, thì, với mọi $x \in g$, $\operatorname{ad} D(x) = [D, \operatorname{ad} x] = 0$, do đó $D(x) = 0$; suy ra $D = 0$. Khi đó Hệ quả 3 suy ra từ Hệ quả 1.

### 2. TÍNH NỬA ĐƠN CỦA CÁC BIỂU DIỄN

#### Bổ đề 1 {#lie-i-s6-lem-1 .statement}

Cho $g$ là một đại số Lie nửa đơn. Biểu diễn phụ hợp của $g$ là nửa đơn. Mọi iđêan và mọi đại số thương của $g$ đều là nửa đơn.

Cho $a$ là một iđêan của $g$. Phần trực giao $b$ của $a$ trong $g$ đối với dạng Killing là một iđêan của $g$ và $a \cap b$ là một iđêan giao hoán ($\S 3$, no. 6, Mệnh đề 7) và do đó bằng không. Vậy $b$ là phần bù của $a$ trong $g$. Hơn nữa, vì dạng Killing của $g$ là không suy biến, nên các hạn chế của nó lên $a$ và $b$ cũng không suy biến (*Algebra*, Chương IX, $\S 4$, no. 1, Hệ quả của Mệnh đề 1) và do đó $a$ và $b$ là nửa đơn (no. 1, Định lý 1 và $\S 3$, no. 6, Mệnh đề 9).

#### Bổ đề 2 {#lie-i-s6-lem-2 .statement}

Cho $g$ là một đại số Lie. Khi đó hai điều kiện sau là tương đương:
(a) Mọi biểu diễn tuyến tính hữu hạn chiều của $g$ đều là nửa đơn.
(b) Cho một biểu diễn tuyến tính $\varphi$ của $g$ trên một không gian vectơ hữu hạn chiều $V$ và một không gian con vectơ W có đối chiều bằng 1 sao cho $\rho(x)(V) \subset W$ với mọi $x \in g$, tồn tại một đường thẳng bù của W ổn định dưới $\rho(g)$ (và do đó bị triệt tiêu bởi $\rho(g)$).

Rõ ràng (a) suy ra (b). Giả sử (b) đúng. Cho $\sigma$ là một biểu diễn hữu hạn chiều của $g$ trên một không gian vectơ M và N là một không gian con của M ổn định dưới $\sigma(g)$. Cho $\mu$ là biểu diễn của $g$ trên $\mathcal{L}(M)$ được dẫn xuất một cách chính tắc từ $\sigma$ (\S 3, no. 3): nhắc lại rằng $\mu(x) = \mathrm{ad}_{\mathcal{L}(M)} \rho(x)$. Gọi V (tương ứng W) là không gian con của $\mathcal{L}(M)$ gồm các ánh xạ tuyến tính từ M vào N mà hạn chế của chúng lên N là một phép vị tự (tương ứng bằng không); khi đó W có đối chiều 1 trong V và $\mu(x)(V) \subset W$ với mọi $x \in g$. Theo điều kiện (b), tồn tại $u \in V$ bị triệt tiêu bởi $\mu(x)$ với mọi $x \in g$ và có hạn chế lên N là một phép vị tự khác không. Nhân $u$ với một vô hướng thích hợp, có thể giả sử rằng $u$ là một phép chiếu của M lên N. Việc nói rằng $\mu(x) \cdot u = 0$ có nghĩa là $u$ giao hoán được với $\sigma(x)$. Do đó hạt nhân của $u$ là một phần bù của N trong M ổn định dưới $\sigma(x)$ với mọi $x \in g$. Vậy $\sigma$ là nửa đơn.

#### Bổ đề 3 {#lie-i-s6-lem-3 .statement}

*Cho g là một đại số Lie nửa đơn, $\rho$ là một biểu diễn tuyến tính của g trên một không gian vectơ hữu hạn chiều V và W là một không gian con của V có đối chiều 1 sao cho $\rho(x)(V) \subset W$ với mọi $x \in g$. Khi đó tồn tại một đường thẳng bổ sung của W ổn định dưới $\rho(g)$.*

Với mọi $x \in g$ gọi $\sigma(x)$ là hạn chế của $\rho(x)$ lên W. Trước hết giả sử rằng $\sigma$ là đơn. Nếu $\sigma = 0$, khi đó $\rho(x)\rho(y) = 0$ với mọi $x, y$ trong $g$, do đó $\rho(g) = \rho(\mathcal{D}g) = \{0\}$ và mệnh đề của chúng ta là hiển nhiên. Nếu $\sigma \neq 0$, gọi n là hạt nhân của $\sigma$ và gọi m là một iđêan bổ sung của n trong $g$ (Bổ đề 1); khi đó $m \neq \{0\}$ và hạn chế của $\sigma$ lên m là trung thành; hạn chế lên m của dạng song tuyến tính liên kết với $\sigma$ là không suy biến (Mệnh đề 1) và do đó phần tử Casimir c liên kết với m và $\sigma$ có thể được lập. Theo Mệnh đề 12 của \S 3, no. 7, $\sigma(c)$ là một tự đẳng cấu của W. Mặt khác, $\rho(c)(V) \subset W$. Do đó hạt nhân Z của $\rho(c)$ là một đường thẳng bổ sung của W; vì c thuộc tâm của đại số bao quanh của $g$, $\rho(c)$ giao hoán được với $\rho(x)$ với mọi $x \in g$ và do đó Z ổn định dưới $\rho(g)$.

Trong trường hợp tổng quát, ta lập luận bằng quy nạp theo chiều của V. Gọi T là một không gian con ổn định cực tiểu khác không của W. Gọi $\rho'$ là biểu diễn thương trên $V' = V/T$. Khi đó, với mọi $x \in g$, $\rho'(x)(V') \subset W'$, trong đó $W' = W/T$ có đối chiều 1 trong $V'$. Theo giả thiết quy nạp tồn tại một đường thẳng $Z'$ bù cho $W'$ và ổn định đối với $\rho'(g)$. Ảnh ngược của nó Z trong V là ổn định đối với $\rho(g)$, chứa T như một không gian con có đối chiều 1, $Z \cap W = T$, và do đó $\rho(x)(Z) \subset T$ với mọi $x \in g$. Theo điều đã chứng minh ở trên, tồn tại một đường thẳng bù của T trong Z ổn định đối với $\rho(g)$; đường thẳng này bù cho W trong V, điều này hoàn tất chứng minh.

#### Định lý 2 (H. Weyl) {#lie-i-s6-thm-2 .statement}

*Mọi biểu diễn tuyến tính hữu hạn chiều của một đại số Lie nửa đơn đều hoàn toàn khả quy.*

Điều này suy ra từ các Bổ đề 2 và 3.

#### Định nghĩa 2 {#lie-i-s6-def-2 .statement}

*Một đại số Lie g được gọi là đơn nếu các iđêan duy nhất của g là {0} và g và nếu thêm nữa g không giao hoán.*

Một đại số Lie đơn là nửa đơn. Đại số {0} không đơn.

#### Mệnh đề 2 {#lie-i-s6-prop-2 .statement}

*Để một đại số Lie g là nửa đơn, điều kiện cần và đủ là nó là một tích của các đại số đơn.*

Điều kiện này là đủ (no. 1, Nhận xét 3). Ngược lại, giả sử rằng g là nửa đơn. Vì biểu diễn phụ hợp của g là nửa đơn, g là tổng trực tiếp của các iđêan cực tiểu khác không $a_1, \ldots, a_m$. Khi đó g được đồng nhất với đại số tích của các $a_i$ (\S 1, no. 1). Mọi iđêan của $a_i$ khi đó là một iđêan của g và do đó bằng không hoặc bằng $a_i$. Mặt khác $a_i$ không giao hoán. Vậy các $a_i$ là các đại số Lie đơn.

#### Hệ quả 1 {#lie-i-s6-prop-2-cor-1 .statement}

*Một đại số Lie nửa đơn là tích của các iđêan đơn của nó $g_i$. Mọi iđêan của g là tích của một số các $g_i$.*

$g = a_1 \times \cdots \times a_m$, trong đó các $a_i$ là đơn. Vì tâm của $a_i$ bằng không, đại số giao hoán hóa của $a_i$ trong g là tích của các $a_j$ với $j \neq i$. Khi đó cho a là một iđêan của g. Nếu nó không chứa $a_i$, thì $a \cap a_i = \{0\}$, do đó $[a, a_i] = \{0\}$ và a được chứa trong tích của các $a_j$ với $j \neq i$. Suy ra a là tích của một số các $a_i$. Vì vậy các iđêan đơn của g chính xác là các $a_i$.

Các iđêan đơn của một đại số Lie nửa đơn được gọi là các *thành phần đơn* của g.

#### Hệ quả 2 {#lie-i-s6-prop-2-cor-2 .statement}

*Cho g, $g'$ là hai đại số Lie, r và $r'$ là các căn của chúng và f là một đồng cấu của g lên $g'$. Khi đó $r' = f(r)$.*

Vì $f(r)$ giải được, $f(r) \subset r'$. Mặt khác, $g/r$ là nửa đơn (\S 5, no. 2, Mệnh đề 3), do đó $g'/f(r)$, là đẳng cấu với một thương của $g/r$, là nửa đơn (Bổ đề 1) và do đó $f(r) \supset r'$ (\S 5, no. 2, Mệnh đề 3).

#### Nhận xét {#lie-i-s6-n2-rem-1 .statement}

(1) Định lý 2 thừa nhận đảo lại: nếu mọi biểu diễn hữu hạn chiều của g đều là nửa đơn, thì g là nửa đơn. Thật vậy, vì biểu diễn phụ hợp là nửa đơn, mọi iđêan của g đều có một iđêan bù và do đó có thể được xem như một thương của g. Nếu g không nửa đơn thì g có một thương giao hoán khác không và do đó có một thương chiều 1. Khi đó đại số Lie K chiều 1 thừa nhận các biểu diễn không nửa đơn, ví dụ

$$
\lambda \mapsto \begin{pmatrix} 0 & 0 \\ \lambda & 0 \end{pmatrix}.
$$

(2) Cho g là một đại số Lie trên K và $\sigma$ là một biểu diễn của g trên một không gian vectơ M. Mặt khác cho $f$ là một ánh xạ K-tuyến tính của $g$ vào M sao cho:

$$
f([x, y]) = \sigma(x) \cdot f(y) - \sigma(y) \cdot f(x)
$$

với mọi $x, y$ trong $g$. Theo § 1, no. 8, Ví dụ 2, việc cho $\sigma$ và $f$ tương đương với việc cho một đồng cấu $x \mapsto (f(x), \sigma(x))$ của $g$ vào $\mathfrak{af}(M)$. Mặt khác ta đã thấy (loc. cit.) rằng phần tử $(f(x), \sigma(x))$ của $\mathfrak{af}(M)$ được đồng nhất một cách chính tắc với phần tử $\rho(x)$ của $\mathfrak{gl}(N)$ (trong đó $N = M \times K$), phần tử này cảm sinh $\sigma(x)$ trên M và gửi phần tử $(0, 1)$ của N vào $f(x)$. Và khi đó $\rho$ là một biểu diễn của $g$ trên N sao cho $\rho(x)(N) \subset M$ với mọi $x \in g$.

Khi đó, nếu $g$ là nửa đơn, tồn tại (Bổ đề 3) một đường thẳng Z phụ với M trong N và bị triệt tiêu bởi $\rho(g)$. Nói cách khác, *tồn tại một phần tử* $m_0 \in M$ sao cho $(-m_0, 1) \in N$ bị triệt tiêu bởi $\rho(x)$, nghĩa là *sao cho*

$$
f(x) = \sigma(x) \cdot m_0
$$

*với mọi* $x \in g$.

*Giả sử rằng $K = \mathbf{R}$. Cho G là một nhóm Lie liên thông với đại số Lie g. Xét một đồng cấu giải tích $\phi$ của G vào nhóm afin A của M tương ứng với một đồng cấu $x \mapsto (f(x), \sigma(x))$ của g vào $\mathfrak{af}(M)$. Các kết quả trên có thể được diễn giải bằng cách nói rằng nếu g là nửa đơn thì $\phi(G)$ giữ cố định một điểm của M. Thật vậy, cho H là tập hợp các phần tử của $\mathbf{GL}(N)$ giữ ổn định mọi đa tạp tuyến tính của N song song với M. Tồn tại (§ 1, no. 8, Ví dụ 2) một đẳng cấu chính tắc $\psi$ của A lên H. Cho Z là một đường thẳng phụ của M trong N. Nói rằng $\rho(g)$ triệt tiêu Z tương đương với việc nói rằng $(\psi \circ \phi)(G)$ giữ cố định các điểm của Z và do đó (tính đến định nghĩa của $\psi$) rằng $\phi(G)$ giữ cố định phép chiếu lên M của giao điểm của Z và $M \times \{1\}$.*

### 3. CÁC PHẦN TỬ NỬA ĐƠN VÀ CÁC PHẦN TỬ LŨY LINH TRONG CÁC ĐẠI SỐ LIE NỬA ĐƠN

#### Mệnh đề 3 {#lie-i-s6-prop-3 .statement}

*Cho M là một không gian vectơ hữu hạn chiều trên K và $g$ là một đại số con nửa đơn của $\mathfrak{gl}(M)$. Khi đó $g$ chứa các thành phần nửa đơn và lũy linh của các phần tử của nó.*

Nếu $K_1$ là một mở rộng của K, dạng Killing của $g_{(K_1)}$ là mở rộng lên $g_{(K_1)}$ của dạng Killing của $g$ (§ 3, no. 8) và do đó không suy biến; vì vậy $g_{(K_1)}$ là nửa đơn. Do đó chỉ cần chứng minh Mệnh đề 3 khi trường cơ sở là đóng đại số, điều mà từ nay ta sẽ giả sử là đúng.

Với mọi không gian con N của M, đặt $g_N$ là đại số con của $\mathfrak{gl}(M)$ gồm các phần tử làm cho N ổn định và có hạn chế lên N có vết bằng không. Vì $g = \mathcal{D}g$, ta có $g \subset g_N$ nếu N ổn định dưới $g$. Khi đó đặt $g^*$ là giao của bộ chuẩn hóa của $g$ trong $\mathfrak{gl}(M)$ với các đại số $g_N$ khi N chạy qua tập hợp các không gian con của M ổn định dưới g. Vì thành phần nửa đơn (ứng với nilpotent) s (ứng với n) của $x \in gl(M)$ là một đa thức theo x không có hằng số và ad s (ứng với ad n) là phần nửa đơn (ứng với nilpotent) của ad x ($\S 5$, no. 4, Bổ đề 2), rõ ràng $x \in g^*$ kéo theo $s \in g^*$ và $n \in g^*$; do đó chỉ cần chứng minh rằng $g^* = g$. Vì g là một iđêan nửa đơn của $g^*$, nên $g^* = a \times g$ (no. 1, Hệ quả 1 của Mệnh đề 1). Lấy $a \in a$ và lấy N là một không gian con cực tiểu trong các không gian con khác không của M ổn định dưới g. Hạn chế của a lên N là một bội vô hướng của đồng nhất thức theo Định lý Burnside, có vết bằng không theo phép dựng, và vì thế bằng không vì K có đặc số 0. Vì M là tổng trực tiếp của các không gian con như N, suy ra $a = 0$ và do đó $g^* = g$.

#### Hệ quả {#lie-i-s6-n3-cor-1 .statement}

Một phần tử x của g là một tự đồng cấu nửa đơn (ứng với nilpotent) của M khi và chỉ khi $ad_g x$ là một tự đồng cấu nửa đơn (ứng với nilpotent) của g.

Gọi s (ứng với n) là thành phần nửa đơn (ứng với nilpotent) của $x \in g$. Khi đó $s \in g$ và $n \in g$ (Mệnh đề 3). Khi đó $ad_g s$ (ứng với $ad_g n$) là thành phần nửa đơn (ứng với nilpotent) của $ad_g x$, theo Bổ đề 2 của $\S 5$, no. 4. Nếu x là nửa đơn (ứng với nilpotent) thì $ad_g x$ cũng vậy. Nếu bây giờ $ad_g x$ là nửa đơn (ứng với nilpotent), thì nó bằng $ad_g s$ (ứng với $ad_g n$) và do đó $x = s$ (ứng với $x = n$) vì biểu diễn liên hợp của g là trung thành.

#### Định nghĩa 3 {#lie-i-s6-def-3 .statement}

Cho g là một đại số Lie nửa đơn. Một phần tử x của g được gọi là nửa đơn (ứng với nilpotent) nếu, với mọi g-môđun M có số chiều hữu hạn trên K, $x_M$ là một tự đồng cấu nửa đơn (ứng với nilpotent) của M.

#### Mệnh đề 4 {#lie-i-s6-prop-4 .statement}

Cho g, g' là các đại số Lie nửa đơn và f là một đồng cấu từ g vào g'. Nếu $x \in g$ là nửa đơn (ứng với nilpotent), thì $f(x)$ cũng vậy. Nếu f là toàn ánh, mọi phần tử nửa đơn (ứng với nilpotent) của g' đều là ảnh qua f của một phần tử nửa đơn (ứng với nilpotent) của g.

Nếu $\rho$ là một biểu diễn của g', thì $\rho \circ f$ là một biểu diễn của g, do đó có mệnh đề thứ nhất. Nếu f là toàn ánh, tồn tại một đồng cấu g từ g' vào g sao cho $f \circ g$ là đồng cấu đồng nhất của g' (no. 1, Hệ quả 2 của Mệnh đề 1) và khi đó mệnh đề thứ hai suy ra từ mệnh đề thứ nhất.

#### Định lý 3 {#lie-i-s6-thm-3 .statement}

Cho g là một đại số Lie nửa đơn.

(a) Cho $x \in g$. Nếu tồn tại một biểu diễn trung thành $\rho$ của g sao cho $\rho(x)$ là một tự đồng cấu nửa đơn (ứng với nilpotent), thì x là nửa đơn (ứng với nilpotent).

(b) Mọi phần tử của g có thể được viết một cách duy nhất thành tổng của một phần tử nửa đơn và một phần tử nilpotent giao hoán với nhau.

Giả sử giả thiết của (a) được thỏa mãn. Gọi $\sigma$ là một biểu diễn của g, b là iđêan phụ bù của hạt nhân của $\sigma$ và $\alpha$ là phép chiếu của g lên b. Khi đó $ad_g x$ là nửa đơn (ứng với nilpotent) theo Hệ quả của Mệnh đề 3 và do đó $ad_b \alpha(x)$ là nửa đơn (ứng với nilpotent). Vì $\sigma(x) = \sigma(\alpha(x))$, mệnh đề thứ nhất suy ra từ Hệ quả của Mệnh đề 3. Kết quả thứ hai khi đó suy ra từ Mệnh đề 3 áp dụng cho một biểu diễn trung thành.

### 4. CÁC ĐẠI SỐ LIE KHẢ QUY

#### Định nghĩa 4 {#lie-i-s6-def-4 .statement}

*Một đại số Lie được gọi là khả quy nếu biểu diễn liên hợp của nó là nửa đơn.*

#### Mệnh đề 5 {#lie-i-s6-prop-5 .statement}

*Cho $g$ là một đại số Lie và $r$ căn của nó. Các điều kiện sau là tương đương:*
(a) $g$ là khả quy.
(b) $\mathcal{D}g$ là nửa đơn.
(c) $g$ là tích của một đại số nửa đơn và một đại số giao hoán.
(d) $g$ có một biểu diễn hữu hạn chiều sao cho dạng song tuyến tính liên kết là không suy biến.
(e) $g$ có một biểu diễn nửa đơn hữu hạn chiều trung thành.
(f) *Căn nilpotent của $g$ bằng không.*
(g) $r$ là tâm của $g$.

(a) $\Rightarrow$ (b): nếu biểu diễn phụ hợp của $g$ là nửa đơn, $g$ là một tổng trực tiếp của các iđêan cực tiểu khác không $a_i$ và do đó $g$ đẳng cấu với tích của các $a_i$; và $a_i$ không có iđêan nào khác ngoài $\{0\}$ và $a_i$ và do đó là đơn hoặc giao hoán có chiều 1. Vì vậy $\mathcal{D}g$ bằng tích của những $a_i$ đơn và do đó là nửa đơn.

(b) $\Rightarrow$ (c): nếu $\mathcal{D}g$ là nửa đơn, $g$ đẳng cấu với tích của $\mathcal{D}g$ bởi một đại số Lie $h$ (no. 1, Hệ quả 1 của Mệnh đề 1); $h$ đẳng cấu với $g/\mathcal{D}g$ và do đó giao hoán.

(c) $\Rightarrow$ (d): cho $g_1$ và $g_2$ là hai đại số Lie, $\rho_i$ là một biểu diễn hữu hạn chiều của $g_i$ và $\beta_i$ là dạng song tuyến tính trên $g_i$ liên kết với $\rho_i$ ($i = 1, 2$); $\rho_1$ và $\rho_2$ có thể được xem là các biểu diễn của $g = g_1 \times g_2$; gọi $\rho$ là tổng trực tiếp của chúng. Rõ ràng dạng song tuyến tính trên $g$ liên kết với $\rho$ là tổng trực tiếp của $\beta_1$ và $\beta_2$ và do đó không suy biến nếu $\beta_1$ và $\beta_2$ không suy biến. Khi đó để chứng minh kéo theo (c) $\Rightarrow$ (d) chỉ cần xét 2 trường hợp sau: (1) $g$ là nửa đơn; khi đó biểu diễn phụ hợp có dạng liên kết là dạng Killing, không suy biến; (2) $g = K$; khi đó biểu diễn đồng nhất của $g$ trên $K$ có một dạng song tuyến tính liên kết không suy biến.

(d) $\Rightarrow$ (e): cho $\rho$ là một biểu diễn hữu hạn chiều của $g$ và $\beta$ là dạng song tuyến tính liên kết; theo Mệnh đề 4 của § 4, no. 3, tồn tại một biểu diễn nửa đơn hữu hạn chiều $\sigma$ của $g$ sao cho hạt nhân $n$ của $\sigma$ trực giao với $g$ đối với $\beta$. Nếu $\beta$ không suy biến, thì $n = \{0\}$ và do đó $\sigma$ là trung thành.

(e) $\Rightarrow$ (f): điều này là hiển nhiên.

(f) $\Rightarrow$ (g): nếu căn lũy linh của $g$ bằng không, thì $\mathcal{D}g \cap r$ bằng không ($\S 5$, no. 3, Định lý 1); vì $[g, r] \subset \mathcal{D}g \cap r$, nên $r$ là tâm của $g$.

(g) ⇒ (a): nếu r là tâm của g, thì biểu diễn kề của g được đồng nhất với một biểu diễn của g/r, mà g/r là một đại số Lie nửa đơn (§ 5, no. 2, Mệnh đề 3); do đó biểu diễn này là nửa đơn (Định lý 2).

#### Nhận xét {#lie-i-s6-n4-rem-1 .statement}

Nếu một đại số Lie g có thể được phân tích thành một tích a × b của một đại số Lie giao hoán a và một đại số Lie nửa đơn b, thì phân tích này là duy nhất. Chính xác hơn, tâm của g bằng tích của các tâm của a và b và vì thế bằng a. Và $\mathcal{D}g = \mathcal{D}a \times \mathcal{D}b = b$.

#### Hệ quả {#lie-i-s6-n4-cor-1 .statement}

(a) Mọi tích hữu hạn của các đại số khả quy đều là một đại số khả quy.
(b) Nếu g là một đại số Lie khả quy có tâm c, thì mọi iđêan của g là một nhân tử trực tiếp, bằng tích của các giao của nó với c và $\mathcal{D}g$, và là một đại số Lie khả quy.
(c) Mọi thương của một đại số Lie khả quy đều là một đại số Lie khả quy.

Mệnh đề (a) suy ra chẳng hạn từ điều kiện (c) của Mệnh đề 5.

Giả sử rằng g là khả quy. Gọi a là một iđêan của g. Vì biểu diễn kề của g là nửa đơn, a có một iđêan bù b và g được đồng nhất với a × b. Với mọi $x \in g$, gọi $\rho(x)$ là hạn chế của $\mathrm{ad}_g x$ lên a. Khi đó $\rho$ là một biểu diễn nửa đơn của g, bằng không trên b và khi chuyển qua thương xác định biểu diễn kề trên a. Do đó a là khả quy. Tương tự, g/a và b, là đẳng cấu, đều khả quy. Sau cùng, gọi d, d' là các tâm của a và b; khi đó $a = d \times \mathcal{D}a, b = d' \times \mathcal{D}b, d \times d' = c, \mathcal{D}a \times \mathcal{D}b = \mathcal{D}g$; do đó $a = (a \cap c) + (a \cap \mathcal{D}g)$.

#### Mệnh đề 6 {#lie-i-s6-prop-6 .statement}

Cho g là một đại số Lie, r là căn của nó và s là căn lũy linh của nó.
(a) $s = [g, r] = \mathcal{D}g \cap r$.
(b) s là giao của các trực giao của g đối với các dạng song tuyến tính liên kết với các biểu diễn hữu hạn chiều của g.

Rõ ràng $[g, r] \subset \mathcal{D}g \cap r$. Bây giờ $\mathcal{D}g \cap r = s$ theo Định lý 1 của § 5, no. 3. Gọi $g' = g/[g, r]$ và f là đồng cấu chính tắc của g lên $g'$; khi đó $f(r)$ là căn $r'$ của $g'$ (Hệ quả 3 của Mệnh đề 2, no. 2), do đó $[g', r'] = \{0\}$ và $r'$ là tâm của $g'$; vì thế (Mệnh đề 5) $g'$ có một biểu diễn hữu hạn chiều trung thành nửa đơn, do đó $s \subset [g, r]$. Điều này chứng minh (a).

Gọi t là giao của các trực giao của g đối với các dạng song tuyến tính liên kết với các biểu diễn hữu hạn chiều của g. Khi đó $s \subset t$ (§ 4, no. 3, Mệnh đề 4 (d)). Mặt khác, $g/s$ có một biểu diễn hữu hạn chiều trung thành nửa đơn và vì thế (Mệnh đề 5) có một biểu diễn hữu hạn chiều $\rho$ sao cho dạng song tuyến tính liên kết là không suy biến; khi được xét như một biểu diễn của g, $\rho$ có một dạng song tuyến tính liên kết $\beta$ trên g và trực giao của g đối với $\beta$ là s, do đó $t \subset s$. Vậy $t = s$.

Ngay cả khi $s \neq \{0\}$ vẫn có thể tồn tại các dạng song tuyến tính đối xứng không suy biến trên g (Bài tập 18 (c)). Dĩ nhiên, các dạng như thế không liên kết với bất kỳ biểu diễn nào của g.

#### Hệ quả {#lie-i-s6-n4-cor-2 .statement}

Cho $g, g'$ là các đại số Lie, $s$ (tương ứng $s'$) là căn lũy linh của $g$ (tương ứng của $g'$) và $f$ là một đồng cấu từ $g$ lên $g'$.
(a) Khi đó $s' = f(s)$.
(b) $g'$ là khả quy khi và chỉ khi hạt nhân của $f$ chứa $s$.

Nếu $r, r'$ là các căn của $g, g'$, thì $s' = [g', r'] = [f(g), f(r)] = f([g, r]) = f(s)$. Mệnh đề (b) là một hệ quả ngay lập tức của (a).

### 5. ÁP DỤNG: MỘT TIÊU CHUẨN CHO TÍNH NỬA ĐƠN CỦA CÁC BIỂU DIỄN

#### Định lý 4 {#lie-i-s6-thm-4 .statement}

Cho $g$ là một đại số Lie, $r$ là căn của nó, $\rho$ là một biểu diễn hữu hạn chiều của $g$, $g' = \rho(g)$ và $r' = \rho(r)$. Khi đó các điều kiện sau là tương đương:
(a) $\rho$ là nửa đơn;
(b) $g'$ là khả quy và tâm của nó gồm các nội tự đồng cấu nửa đơn;
(c) $r'$ gồm các nội tự đồng cấu nửa đơn;
(d) hạn chế của $\rho$ lên $r$ là nửa đơn.

(a) $\Rightarrow$ (b): nếu $\rho$ là nửa đơn thì $g'$ là khả quy (Mệnh đề 5); đại số kết hợp được sinh bởi 1 và $g'$ là nửa đơn (\emph{Algebra}, Chapter VIII, § 5, no. 1, Proposition 3), do đó tâm của nó là nửa đơn (\emph{loc. cit.}, § 5, no. 4, Proposition 12) và vì thế các phần tử của tâm này là nửa đơn (\emph{loc. cit.}, § 9, no. 1, Proposition 2).

(b) $\Rightarrow$ (c): nếu $g'$ là khả quy thì tâm của nó bằng căn của nó, tức là $r'$, do đó suy ra (b) $\Rightarrow$ (c).

(c) $\Rightarrow$ (d): giả sử rằng $r'$ gồm các nội tự đồng cấu nửa đơn. Vì $[g', r']$ gồm các nội tự đồng cấu lũy linh (no. 4, Proposition 6), nên $[g', r'] = \{0\}$. Khi đó suy ra (c) $\Rightarrow$ (d) từ \emph{Algebra}, Chapter VIII, § 9, no. 2, Theorem 1.

(d) $\Rightarrow$ (a): cho $s$ là căn lũy linh của $g$ và $\rho'$ là hạn chế của $\rho$ lên $r$. Các phần tử của $\rho(s)$ là lũy linh và do đó $s$ được chứa trong iđêan lũy linh lớn nhất của $\rho'$. Vì $\rho'$ là nửa đơn nên $\rho'(s) = \{0\}$ và $g'$ là khả quy (Hệ quả của Mệnh đề 6), vì vậy $g' = a' \times r'$ với $a'$ nửa đơn (Mệnh đề 5). Gọi $A'$ (tương ứng $R'$) là đại số kết hợp được sinh bởi 1 và $a'$ (tương ứng $r'$). Nó là nửa đơn (\emph{Algebra}, Chapter VIII, § 5, no. 1, Proposition 3), do đó $A' \otimes_K R'$ là nửa đơn (\emph{loc. cit.}, § 7, no. 6, Corollary 4 to Theorem 3) và vì thế đại số kết hợp được sinh bởi 1 và $g'$, là một thương của $A' \otimes_K R'$, là nửa đơn, điều này chứng minh rằng $\rho$ là nửa đơn.

#### Hệ quả 1 {#lie-i-s6-thm-4-cor-1 .statement}

Cho $g$ là một đại số Lie và $\rho$ và $\rho'$ là hai biểu diễn hữu hạn chiều nửa đơn của $g$. Khi đó tích tenxơ của $\rho$ và $\rho'$ là nửa đơn.

Cho $r$ là căn của $g$. Với $x \in r$, $\rho(x)$ và $\rho'(x)$ là nửa đơn (Định lý 4), do đó $\rho(x) \otimes 1 + 1 \otimes \rho'(x)$ là nửa đơn (\emph{Algebra}, Chapter VIII, § 9, Corollary to Theorem 1) và vì thế tích tenxơ của $\rho$ và $\rho'$ là nửa đơn (Định lý 4).

#### Hệ quả 2 {#lie-i-s6-thm-4-cor-2 .statement}

Cho $g$ là một đại số Lie, $\rho$ là một biểu diễn nửa đơn của $g$ trên một không gian vectơ hữu hạn chiều $V$, $T$ và $S$ là các đại số tenxơ và đối xứng của $V$, và $\sigma_T$, $\sigma_S$ là các biểu diễn của $g$ trên $T$ và $S$ được dẫn xuất một cách chính tắc từ $\rho$. Khi đó $\sigma_T$ và $\sigma_S$ là nửa đơn, và chính xác hơn, là các tổng trực tiếp của các biểu diễn đơn hữu hạn chiều.

Cho $T^n$ là không gian con của $T$ gồm các tenxơ thuần nhất cấp $n$. Không gian con này ổn định đối với $\sigma_T$, và biểu diễn do $\sigma_T$ xác định trên $T^n$ là nửa đơn (Hệ quả 1). Suy ra hệ quả đối với $\sigma_T$ và do đó đối với $\sigma_S$, là biểu diễn thương của $\sigma_T$.

#### Hệ quả 3 {#lie-i-s6-thm-4-cor-3 .statement}

Cho $g$ là một đại số Lie và $\rho$, $\rho'$ là hai biểu diễn nửa đơn hữu hạn chiều của $g$ trên các không gian $M$ và $M'$. Khi đó biểu diễn của $g$ trên $\mathcal{L}_K(M, M')$ được dẫn xuất một cách chính tắc từ $\rho$ và $\rho'$ là nửa đơn.

$g$-môđun $\mathcal{L}_K(M, M')$ được đồng nhất một cách chính tắc với $g$-môđun $M^* \otimes_K M'$ (\S 3, no. 3, Mệnh đề 4), nên Hệ quả 3 suy ra từ Hệ quả 1.

#### Hệ quả 4 {#lie-i-s6-thm-4-cor-4 .statement}

Cho $g$ là một đại số Lie, $a$ là một iđêan của $g$, và $\rho$ là một biểu diễn nửa đơn của $g$.
(a) Hạn chế $\rho'$ của $\rho$ lên $a$ là nửa đơn.
(b) Nếu $\rho$ là đơn thì $\rho'$ là một tổng của các biểu diễn đơn đẳng cấu với nhau.

Chuyển qua thương theo hạt nhân của $\rho$, có thể giả sử rằng $\rho$ là trung thành. Khi đó $g$ là khả quy. Đặt $g = g_1 \times g_2$, trong đó $g_1$ là tâm của $g$ và $g_2$ là nửa đơn. Khi đó $a = a_1 \times a_2$, trong đó $a_1 \subset g_1$, $a_2 \subset g_2$ và $a_1$ là tâm của $a$. Các phần tử của $\rho(g_1)$, và đặc biệt các phần tử của $\rho(a_1)$, là nửa đơn (Định lý 4) và do đó $\rho'$ là nửa đơn (Định lý 4). Suy ra (a). Mệnh đề (b) suy ra từ (a), dùng \S 3, no. 1, Hệ quả của Mệnh đề 1.

### 6. CÁC ĐẠI SỐ CON KHẢ QUY TRONG MỘT ĐẠI SỐ LIE

#### Định nghĩa 5 {#lie-i-s6-def-5 .statement}

Cho $g$ là một đại số Lie và $h$ là một đại số con Lie của $g$. Ta gọi $h$ là khả quy trong $g$ nếu biểu diễn $x \mapsto \operatorname{ad}_g x$ của $h$ là nửa đơn.

Biểu diễn này nhận biểu diễn phụ hợp của $h$ làm biểu diễn con. Do đó, nếu $h$ khả quy trong $g$ thì $h$ là khả quy. Mặt khác, nói rằng một đại số Lie khả quy trong chính nó tương đương với nói rằng nó là khả quy.

#### Mệnh đề 7 {#lie-i-s6-prop-7 .statement}

Cho $g$ là một đại số Lie, $h$ là một đại số con khả quy trong $g$, $\rho$ là một biểu diễn của $g$ trên một không gian vectơ $V$ và $W$ là tổng của các không gian con hữu hạn chiều của $V$ là các $h$-môđun đơn. Khi đó $W$ ổn định dưới $\rho(g)$.

Cho $W_0$ là một $h$-môđun con đơn hữu hạn chiều của $V$. Ta cần chứng minh rằng $\rho(x)(W_0) \subset W$ với mọi $x \in g$. Ký hiệu $M$ là không gian vectơ $g$ được coi là một $h$-môđun nhờ biểu diễn $x \mapsto \operatorname{ad}_g x$ của $h$ trên $g$. Khi đó $M \otimes_K W_0$ là một $h$-môđun nửa đơn (Hệ quả 1 của Định lý 4). Cho $\theta$ là ánh xạ K-tuyến tính từ $M \otimes_K W_0$ vào V được xác định bởi $\theta(x \otimes w) = \rho(x)w$. Đây là một đồng cấu $\mathfrak{h}$-môđun, vì nếu $y \in \mathfrak{h}$ thì:

$$
\begin{align*}
\theta([y, x] \otimes w + x \otimes \rho(y)w) &= \rho([y, x])w + \rho(x)\rho(y)w \\
&= \rho(y)\rho(x)w = \rho(y)\theta(x \otimes w).
\end{align*}
$$

Do đó $\theta(M \otimes_K W_0)$ là một $\mathfrak{h}$-môđun nửa đơn hữu hạn chiều. Do đó $\theta(M \otimes_K W_0) \subset W$, nghĩa là $\rho(x)(W_0) \subset W$ với mọi $x \in g$.

#### Hệ quả 1 {#lie-i-s6-prop-7-cor-1 .statement}

*Cho $g$ là một đại số Lie, $\mathfrak{h}$ là một đại số con khả quy trong $g$ và $\rho$ là một biểu diễn nửa đơn hữu hạn chiều của $g$. Khi đó hạn chế của $\rho$ lên $\mathfrak{h}$ là nửa đơn.*

Chỉ cần xét trường hợp $\rho$ đơn. Ta dùng ký hiệu V, W của Mệnh đề 4. Gọi $W_1$ là một không gian con khác không cực tiểu của V ổn định dưới $\rho(\mathfrak{h})$. Khi đó $W_1 \subset W$, do đó $W \neq \{0\}$ và do đó $W = V$.

#### Hệ quả 2 {#lie-i-s6-prop-7-cor-2 .statement}

*Cho $g$ là một đại số Lie, $\mathfrak{h}$ là một đại số con khả quy trong $g$ và $\mathfrak{k}$ là một đại số con của $\mathfrak{h}$ khả quy trong $\mathfrak{h}$. Khi đó $\mathfrak{k}$ khả quy trong $g$.*

Biểu diễn $x \mapsto \mathrm{ad}_g x$ của $\mathfrak{h}$ trên $g$ là nửa đơn và do đó hạn chế của nó lên $\mathfrak{k}$ là nửa đơn (Hệ quả 1).

### 7. VÍ DỤ VỀ CÁC ĐẠI SỐ LIE NỬA ĐƠN

#### Mệnh đề 8 {#lie-i-s6-prop-8 .statement}

*Cho $V$ là một không gian vectơ hữu hạn chiều. Khi đó $\mathrm{gl}(V)$ là khả quy. Tâm của nó là tập hợp các phép vị tự của $V$, đại số dẫn xuất của nó là $\mathrm{sl}(V)$ và đại số sau là nửa đơn.*

Biểu diễn đồng nhất của $\mathrm{gl}(V)$ là đơn, do đó $\mathrm{gl}(V)$ là khả quy và vì vậy $\mathrm{gl}(V)$ là tổng trực tiếp của tâm $c$ và đại số dẫn xuất $\mathcal{D}(\mathrm{gl}(V))$ của nó. Tâm $c$ là tập hợp các phép vị tự (*Đại số*, Chương II, § 2, no. 5, Hệ quả 1 của Mệnh đề 5). Rõ ràng $\mathcal{D}(\mathrm{gl}(V)) \subset \mathrm{sl}(V)$. Vì $\mathrm{sl}(V) \cap c = \{0\}$, $\mathcal{D}(\mathrm{gl}(V)) = \mathrm{sl}(V)$. Do đó $\mathrm{sl}(V)$ là nửa đơn.

#### Ví dụ {#lie-i-s6-n7-exa-1 .statement}

Ta đồng nhất $\mathrm{sl}(K^2)$ với đại số Lie của các ma trận cấp 2 và vết bằng không. Ta viết

$$
X = \begin{pmatrix} 0 & 1 \\ 0 & 0 \end{pmatrix} \quad Y = \begin{pmatrix} 0 & 0 \\ 1 & 0 \end{pmatrix} \quad H = \begin{pmatrix} 1 & 0 \\ 0 & -1 \end{pmatrix}.
$$

Khi đó $X, Y, H$ lập thành một cơ sở của $\mathrm{sl}(K^2)$ và

$$
[H, X] = 2X \qquad [H, Y] = -2Y \qquad [X, Y] = H.
$$

Vì một đại số có chiều 1 hoặc 2 không nửa đơn (no. 1, *Nhận xét 1*), $\mathrm{sl}(K^2)$ là đơn. Thực ra, $\mathrm{sl}(V)$ là đơn với $\dim V \geq 2$, như ta sẽ thấy sau (xem thêm Bài tập 21 và 24).

#### Mệnh đề 9 {#lie-i-s6-prop-9 .statement}

Cho V là một không gian vectơ có số chiều hữu hạn n trên K và β là một dạng song tuyến tính đối xứng (tương ứng phản xứng) không suy biến trên V. Gọi g là đại số Lie gồm các $x \in \mathrm{gl}(V)$ sao cho β(xm, m') + β(m, xm') = 0 với mọi m, m' trong V. Khi đó g khả quy; g thậm chí nửa đơn trừ trường hợp β đối xứng và n = 2.

Với mọi u ∈ gl(V), ký hiệu u* là phần tử liên hợp của nó đối với β; khi đó Tr(u) = Tr(u*) theo Mệnh đề 7 của Đại số, Chương IX, § 1, no. 8. Điều kiện

$$
\beta(um, m') + \beta(m, um') = 0
$$

với mọi m, m' trong V có nghĩa là $u + u^* = 0$. Đặc biệt, nếu $v \in \mathrm{gl}(V)$ thì $(v - v^*)^* = v^* - v$ và do đó $v - v^* \in g$. Khi đó gọi u là một phần tử của g trực giao với g đối với dạng song tuyến tính φ liên kết với biểu diễn đồng nhất của g. Với mọi $v \in \mathrm{gl}(V)$, $\mathrm{Tr}\,u(v - v^*) = 0$, do đó

$$
\mathrm{Tr}(uv) = \mathrm{Tr}(uv^*) = \mathrm{Tr}(uv^*)^* = \mathrm{Tr}(vu^*) = -\mathrm{Tr}(vu) = -\mathrm{Tr}(uw)
$$

và do đó $\mathrm{Tr}(uw) = 0$. Suy ra $u = 0$, do đó φ không suy biến. Vậy g là khả quy (Mệnh đề 5). Còn phải chứng minh rằng tâm của g bằng không (trừ khi β đối xứng và $n = 2$). Bằng cách mở rộng trường cơ sở, ta có thể giả sử rằng K đóng đại số.

(a) Khi β đối xứng, nó có thể được đồng nhất với dạng song tuyến tính trên $K^n$ có ma trận $I_n$ đối với cơ sở chính tắc (Algebra, Chương IX, § 6, Hệ quả 1 của Định lý 1). Trong các điều kiện này, g được đồng nhất với đại số Lie của các ma trận phản đối xứng ($\S 3$, no. 4, Ví dụ 1). Cho $U = (u_{ij}) \in g$; ta sử dụng sự kiện rằng U giao hoán với ma trận $(v_{ij}) \in g$ mà mọi phần tử của nó đều bằng không ngoại trừ $v_{i_0j_0}$ và $v_{j_0i_0}$ ($i_0 \neq j_0$), lần lượt bằng 1 và −1. Ta nhận được rằng $u_{i_0j} = u_{j_0i} = u_{i_0} = u_{j_0} = 0$ với $i \neq i_0, j_0$ và $j \neq i_0, j_0$. Nếu $n > 2$, với mọi cặp chỉ số phân biệt $i_0$ và $j$, tồn tại các chỉ số phân biệt i và $j_0$ sao cho $i \neq i_0, j_0 \neq j, j_0 \neq i_0$; do đó $u_{i_0j} = 0$. Điều này chứng minh rằng một phần tử của tâm của g bằng không.

(b) Khi β phản xứng và $n = 2m$, β có thể được đồng nhất với dạng song tuyến tính trên $K^{2m}$ có ma trận $\begin{pmatrix} 0 & I_m \\ -I_m & 0 \end{pmatrix}$ đối với cơ sở chính tắc (Algebra, Chương IX, § 5, Hệ quả 1 của Định lý 1). Trong các điều kiện này, g được đồng nhất với đại số Lie của các ma trận dạng $U = \begin{pmatrix} A & B \\ C & D \end{pmatrix}$ trong đó $D = -{}^tA$, B và C đối xứng ($A, B, C, D$ trong $\mathbf{M}_m(K)$) ($\S 3$, no. 4, Ví dụ 1). Trước hết ta sử dụng sự kiện rằng U giao hoán với ma trận $\begin{pmatrix} X & 0 \\ 0 & -{}^tX \end{pmatrix}$, trong đó $X \in \mathbf{M}_m(K)$. Khi đó $AX = XA, CX = -{}^tXC, XB = -B\cdot{}^tX$; vì các đẳng thức này phải đúng với mọi X, suy ra A là một ma trận vô hướng $\lambda I_m$. Bây giờ ta sử dụng sự kiện rằng U giao hoán với ma trận $\begin{pmatrix} 0 & Y \\ 0 & 0 \end{pmatrix}$, trong đó

Y là một ma trận đối xứng của $\mathbf{M}_m(\mathbf{K})$. Khi đó $\lambda Y = YC = CY = 0$. Điều này trước hết chứng minh rằng $\lambda = 0$. Hơn nữa, với mọi $X \in \mathbf{M}_m(\mathbf{K})$, $X + {}^tX$ là đối xứng và do đó $XC = -{}^tXC$. Sử dụng phương trình $CX = -{}^tXC$ thu được ở trên, ta thấy rằng C giao hoán với mọi phần tử của $\mathbf{M}_m(\mathbf{K})$ và do đó C là một ma trận vô hướng, nhất thiết bằng không vì $YC = 0$. Tương tự, ta chứng minh được rằng $B = 0$.

Với $\beta$ đối xứng và $n = 2$, $g$ có chiều 1 và do đó giao hoán. Với các trường hợp khác, xem Bài tập 25 và 26.

### 8. ĐỊNH LÝ LEVI-MALCEV

Cho E là một không gian vectơ định chuẩn đầy đủ trên $\mathbf{R}$ và u là một tự đồng cấu liên tục của E. Ta đã thấy (Functions of a real variable, Chương IV, § 2, no. 6) rằng dãy $\frac{u^n}{n!}$ khả tổng trong $\mathcal{L}(E)$ và ta đã viết

$$
e^u = \exp u = \sum_{n=0}^\infty \frac{u^n}{n!}.
$$

Bây giờ cho E là một không gian vectơ trên trường K và u là một tự đồng cấu lũy linh của E. Chuỗi $\sum_{n=0}^\infty \frac{u^n}{n!}$ chỉ có một số hữu hạn số hạng khác không và do đó ta có thể viết

$$
e^u = \exp u = \sum_{n=0}^\infty \frac{u^n}{n!}.
$$

Định nghĩa này trùng với định nghĩa trên nếu $K = \mathbf{R}$ và nếu E đầy đủ và định chuẩn. Nếu v là một tự đồng cấu lũy linh khác của E giao hoán với u, thì:

$$
e^{u+v} = \left( \sum_{n=0}^\infty \frac{u^n}{n!} \right) \left( \sum_{p=0}^\infty \frac{v^p}{p!} \right) = \sum_{n,p=0}^\infty \frac{u^n v^p}{n! p!}
$$
$$
= \sum_{q=0}^\infty \frac{1}{q!} \left( \sum_{n+p=q} \binom{q}{n} u^n v^p \right) = \sum_{q=0}^\infty \frac{1}{q!} (u+v)^q = e^{u+v}.
$$

Đặc biệt, $e^u e^{-u} = e^{-u} e^u = e^0 = 1$ và do đó $e^u$ luôn là một tự đẳng cấu của E.

Nếu hơn nữa E là một đại số (không nhất thiết kết hợp) và $u$ là một đạo hàm (lũy linh) của E, thì $e^u$ là một tự đẳng cấu của đại số E. Thật vậy, nếu $x, y \in E$ thì

$$
u^p(xy) = \sum_{r+s=p} \binom{p}{r} u^r(x) u^s(y)
$$

với mọi số nguyên $p \geqslant 0$ (công thức Leibniz). Suy ra rằng

$$
e^{u}(xy) = \sum_{p \geqslant 0} \frac{1}{p!} u^p(xy) = \sum_{p \geqslant 0} \sum_{r+s=p} \frac{u^r(x)}{r!} \frac{u^s(y)}{s!}
$$

$$
= \sum_{r,s=0}^{\infty} \frac{u^r(x)}{r!} \frac{u^s(y)}{s!} = e^{u}(x)e^{u}(y)
$$

do đó mệnh đề của chúng ta được chứng minh.

Bây giờ cho $g$ là một đại số Lie. Nếu $x$ thuộc căn lũy linh của $g$, đạo hàm $\mathrm{ad}_g x$ của $g$ là lũy linh. Do đó ta có thể đưa ra định nghĩa sau:

#### Định nghĩa 6 {#lie-i-s6-def-6 .statement}

*Một tự đẳng cấu đặc biệt của $g$ là một tự đẳng cấu của $g$ có dạng $e^{\mathrm{ad}\, x}$, trong đó $x$ nằm trong căn lũy linh của $g$.*

Rõ ràng một tự đẳng cấu đặc biệt giữ ổn định mọi iđêan của $g$.

#### Định nghĩa 7 {#lie-i-s6-def-7 .statement}

*Cho $g$ là một đại số Lie và $r$ là căn của nó. Một đại số con Levi của $g$ là bất kỳ đại số con nào của $g$ phụ với $r$.*

Một đại số con Levi đẳng cấu với $g/r$ và do đó là nửa đơn. Vì một đại số con nửa đơn chỉ có 0 là phần chung với $r$, mọi đại số con nửa đơn $h$ sao cho $g = r + h$ là một đại số con Levi; do đó ảnh của một đại số con Levi qua một đồng cấu toàn ánh là một đại số con Levi.

#### Định lý 5 (Levi–Malcev) {#lie-i-s6-thm-5 .statement}

*Một đại số Lie $g$ luôn có một đại số con Levi $s$. Mọi đại số con Levi của $g$ là ảnh của $s$ qua một tự đẳng cấu đặc biệt.*

Gọi $r$ là căn của $g$. Trước hết ta xét hai trường hợp đặc biệt.

(a) $[g, r] = \{0\}$.

Theo Mệnh đề 5, khi đó $g$ là tích của tâm $r$ của nó với $\mathcal{D}g$ là nửa đơn. Do đó $\mathcal{D}g$ là một đại số con Levi. Hơn nữa, nếu $s'$ là một đại số con nửa đơn, thì $s' = \mathcal{D}s'$ (Định lý 1), do đó $s' \subset \mathcal{D}g$ và $\mathcal{D}g$ là đại số con Levi duy nhất của $g$.

(b) $[g, r] \neq \{0\}$ và các iđêan duy nhất của $g$ được chứa trong $r$ là $\{0\}$ và $r$.

Sau đó $[g, r] = r,\ [r, r] = \{0\}$ và tâm của $g$ là không. Gọi $M$ (tương ứng $N$) là không gian con của $\mathcal{L}(g)$ gồm các ánh xạ tuyến tính từ $g$ vào $r$ mà hạn chế lên $r$ là một phép vị tự (tương ứng không); do đó $N$ có đối chiều 1 trong $M$. Với $m \in M$, ký hiệu $\lambda(m)$ là tỉ số của phép vị tự của $r$ được xác định bởi $m$. Gọi $\sigma$ là biểu diễn của $g$ trên $\mathcal{L}(g) được dẫn xuất một cách chính tắc từ biểu diễn liên hợp; nhắc lại rằng $\sigma(x).u = [\mathrm{ad}_g x, u]$ với mọi $x \in g$ và mọi $u \in \mathcal{L}(g)$.

Rõ ràng $\sigma(x)(M) \subset N$ với mọi $x \in g$. Hơn nữa, nếu $x \in r, y \in g$ và $u \in M$, thì
$$
(\sigma(x).u)(y) = [x, u(y)] - u([x, y]) = -\lambda(u)[x, y]
$$
vì $[r, r] = \{0\}$; và (4) có thể được viết:
$$
(x).u = -\mathrm{ad}(\lambda(u).x).
$$

Vì tâm của $g$ là không, ánh xạ $x \mapsto \mathrm{ad}_g x$ xác định một song ánh $\phi$ của $r$ lên một không gian con $P$ của $\mathcal{L}(g)$. Không gian con này ổn định dưới $\sigma(g)$ và được chứa trong $N$ vì $r$ là một iđêan giao hoán và (5) chỉ ra rằng $\sigma(x)(M) \subset P$ với $x \in r$. Biểu diễn của $g$ trên $M/P = V$ dẫn xuất từ $\sigma$ do đó là không trên $r$ và xác định một biểu diễn $\sigma'$ của đại số nửa đơn $g/r$ trên $V$. Với mọi $y \in g/r$, không gian $\sigma'(y)(V)$ được chứa trong $N/P$, có đối hợp mã 1 trong $V$. Do đó (no. 2, Bổ đề 3) tồn tại $u_0 \in M$ sao cho $\lambda(u_0) = -1$ và $\sigma(x).u_0 \in P$ với mọi $x \in g$. Ánh xạ $x \mapsto \phi^{-1}(\sigma(x).u_0)$ là một ánh xạ tuyến tính từ $g$ vào $r$. Theo (5), hạn chế của nó trên $r$ là ánh xạ đồng nhất của $r$. Vì thế hạt nhân của nó là một không gian con $s$ của $g$ bù với $r$ trong $g$. Vì $s$ là tập hợp các $x \in g$ sao cho $\sigma(x).u_0 = 0$, $s$ là một đại số con của $g$ và do đó là một đại số con Levi của $g$.

Cho $s'$ là một đại số con Levi khác. Với mọi $x \in s'$, gọi $h(x)$ là phần tử duy nhất của $r$ sao cho $x + h(x) \in s$. Vì $s$ là một đại số con và $r$ giao hoán, với $x, y$ thuộc $s'$:
$$
[x + h(x), y + h(y)] = [x, y] + [x, h(y)] + [h(x), y] \in s
$$
do đó
$$
h([x, y]) = (\mathrm{ad}\, x).h(y) - (\mathrm{ad}\, y).h(x).
$$
Theo Nhận xét 2 của no. 2, tồn tại $a \in r$ sao cho $h(x) = -[x, a]$ với mọi $x \in s'$. Khi đó:
$$
x + h(x) = x + [a, x] = (1 + \mathrm{ad}\, a).x.
$$
Vì $r$ giao hoán, $(\mathrm{ad}\, a)^2 = 0$ và do đó $1 + \mathrm{ad}\, a = e^{\mathrm{ad}\, a}$. Vì $r = [g, r]$, $e^{\mathrm{ad}\, a}$ là một tự đẳng cấu đặc biệt của $g$. Theo (6), tự đẳng cấu đặc biệt này biến $s'$ thành $s$.

(c) Trường hợp tổng quát:

Ta lập luận bằng quy nạp theo chiều $n$ của căn. Không có gì phải chứng minh nếu $n = 0$ và do đó có thể giả sử rằng định lý đúng đối với các đại số Lie có căn có chiều $< \dim r$. Theo (a), chỉ cần xét trường hợp $[g, r] \neq \{0\}$. Vì $[g, r]$ lũy linh (no. 4, Mệnh đề 6), tâm $c$ của nó $\neq \{0\}$. Gọi $m$ là một iđêan cực tiểu khác không của $g$ được chứa trong $c$. Nếu $m = r$, ta có trường hợp (b). Do đó, đặt $m \neq r$ và gọi $f$ là ánh xạ chính tắc của $g$ lên $g' = g/m$. Căn của $g'$ là $r' = r/m$. Theo giả thiết quy nạp, $g'$ có một đại số con Levi $l'$. Khi đó $b = f(l')$ là một đại số con của g chứa m sao cho h/m = h' là nửa đơn và do đó có m làm căn. Theo giả thiết quy nạp h = m + s trong đó s là một đại số con nửa đơn. Khi đó đẳng thức g' = r' + h' suy ra g = r + h = r + m + s = r + s và do đó s là một đại số con Levi của g.

Cho s' là một đại số con Levi khác của g. Khi đó f(s) và f(s') là hai đại số con Levi của g' và theo giả thiết quy nạp tồn tại a' ∈ [g', r'] sao cho e^{ad\alpha'}(f(s')) = f(s). Nếu a ∈ [g, r] sao cho f(a) = a', thì suy ra:

s_1 = e^{ada}(s') \subset m + s = h.

Khi đó s_1 và s là hai đại số con Levi của h và theo giả thiết quy nạp tồn tại b ∈ m sao cho e^{adb}(s_1) = s. Do đó s = e^{adb}.e^{ada}(s'). Cuối cùng, vì m nằm trong tâm của [g, r], e^{adb}.e^{ada} = e^{ad(b+a)} và b + a ∈ [g, r], điều này hoàn tất chứng minh.

#### Hệ quả 1 {#lie-i-s6-thm-5-cor-1 .statement}

Cho s là một đại số con Levi của g và h là một đại số con nửa đơn của g.
(a) Tồn tại một tự đẳng cấu đặc biệt của g biến h thành một đại số con của s.
(b) h được chứa trong một đại số con Levi của g.

Gọi r là căn của g và a = h + r, là một đại số con của g. Khi đó a/r là nửa đơn và r giải được, do đó r là căn của a và h là một đại số con Levi của a. Mặt khác, a ∩ s = h' là một đại số con bổ sung cho r trong a và do đó cũng là một đại số con Levi của a. Khi đó tồn tại (Định lý 5) a ∈ [a, r] sao cho e^{ada} biến h thành h'. Bây giờ a ∈ [g, r]; e^{ada} biến h thành một đại số con của s và e^{-ada}(s) là một đại số con Levi của g chứa h.

#### Hệ quả 2 {#lie-i-s6-thm-5-cor-2 .statement}

Để một đại số con h của g là một đại số con Levi của g, điều kiện cần và đủ là h là một đại số con nửa đơn cực đại của g.

Điều này suy ra ngay lập tức từ Hệ quả 1.

#### Hệ quả 3 {#lie-i-s6-thm-5-cor-3 .statement}

Cho g là một đại số Lie và m là một iđêan của g sao cho g/m là nửa đơn. Khi đó g chứa một đại số con bổ sung cho m trong g. Nói cách khác, mọi mở rộng của một đại số Lie nửa đơn đều là không cốt yếu.

Cho s là một đại số con Levi của g (Định lý 5). Ảnh chính tắc của nó trong g/m là một đại số con Levi và do đó bằng g/m, suy ra g = s + m. Khi đó một iđêan của s bổ sung trong s cho iđêan m ∩ s là một đại số con của g bổ sung cho m trong g.

#### Hệ quả 4 {#lie-i-s6-thm-5-cor-4 .statement}

Cho g là một đại số Lie, r là căn của nó, s là một đại số con Levi của g và m là một iđêan của g. Khi đó m là tổng trực tiếp của m ∩ r, là căn của nó, và m ∩ s, là một đại số con Levi của m.

Ta biết rằng m ∩ s là căn của m (§ 5, no. 5, Hệ quả 3 của Mệnh đề 5). Gọi h là một đại số con Levi của m và s' là một đại số con Levi của g chứa h (Hệ quả 1). Đại số m ∩ s' là một iđêan của s', do đó là nửa đơn, và chứa h nên bằng h. Do đó m là tổng trực tiếp của $m \cap r$ và $m \cap s'$. Tồn tại một tự đẳng cấu đặc biệt biến $s'$ thành $s$; tự đẳng cấu này giữ bất biến $r$ và $m$; do đó m là tổng trực tiếp của $m \cap r$ và $m \cap s$ và $m \cap s$ là một đại số con Levi của $m$.

### 9. ĐỊNH LÝ CÁC BẤT BIẾN

Cho $g$ là một đại số Lie và $\rho$ là một biểu diễn của $g$ trên một không gian vectơ $M$. Với mỗi lớp $\delta$ của các biểu diễn đơn của $g$, ký hiệu $M_\delta$ là thành phần đẳng kiểu của $M$ thuộc loài $\delta$. Không gian con $M_0$ gồm các phần tử bất biến của $M$ chính là $M_{\delta_0}$, trong đó $\delta_0$ ký hiệu lớp của biểu diễn không của $g$ trên một không gian có chiều 1.

#### Bổ đề 4 {#lie-i-s6-lem-4 .statement}

*Cho $\rho, \sigma, \tau$ là các biểu diễn của $g$ trên các không gian vectơ $M, N, P$. Giả sử ta được cho một ánh xạ song tuyến tính trên $K$ $(m, n) \mapsto m.n$ từ $M \times N$ vào $P$ sao cho*

$$
(\rho(x)m).n + m.(\sigma(x)n) = \tau(x)(m.n)
$$

*với mọi $m \in M, n \in N, x \in g$.*

(a) *Nếu $m_0 \in M_0$, ánh xạ $n \mapsto m_0.n$ là một đồng cấu $g$-môđun.*

(b) *Nếu $n \in N_\delta$, thì $m_0.n \in P_\delta$.*

(c) *Nếu $M$ là một đại số (không nhất thiết kết hợp) và các $\rho(x)$ là các phép đạo hàm của $M$, thì $M_0$ là một đại số con của $M$ và mỗi $M_\delta$ là một môđun phải và trái trên $M_0$.*

Với $m_0 \in M_0, n \in N$ và $x \in g$,

$$
\tau(x)(m_0.n) = m_0.(\sigma(x)n),
$$

do đó suy ra (a). Mệnh đề (b) suy ra từ (a) (*Đại số*, Chương VIII, § 3, no. 4, Mệnh đề 10). Nếu $N = P = M$ và $\sigma = \tau = \rho$, mệnh đề (b) cho mệnh đề (c) như một trường hợp đặc biệt.

#### Bổ đề 5 {#lie-i-s6-lem-5 .statement}

*Giả sử thêm rằng $\sigma$ và $\tau$ là nửa đơn và do đó $N$ (tương ứng $P$) là tổng trực tiếp của các $N_\delta$ (tương ứng $P_\delta$). Với mọi $n \in N$ (tương ứng $p \in P$), ký hiệu $n^\natural$ (tương ứng $p^\natural$) là thành phần của nó trong $N_0$ (tương ứng $P_0$). Cho $m_0 \in M_0$. Khi đó với mọi $n \in N$, $(m_0.n)^\natural = m_0.n^\natural$.*

Do tính tuyến tính, chỉ cần xét trường hợp $n \in N_\delta$. Nếu $\delta \neq \delta_0$, $n^\natural = 0$ và $m_0.n \in P_\delta$ (Bổ đề 4), do đó $(m_0.n)^\natural = 0 = m_0.n^\natural$. Nếu $\delta = \delta_0$, $n^\natural = n$ và $m_0.n \in P_0$ (Bổ đề 4), do đó $(m_0.n)^\natural = m_0.n = m_0.n^\natural$.

#### Định lý 6 {#lie-i-s6-thm-6 .statement}

*Cho $g$ là một đại số Lie, $V$ là một $g$-môđun nửa đơn hữu hạn chiều trên $K$, $S$ là đại số đối xứng của $V$ và $x_S$ là đạo hàm của $S$ mở rộng $x_V$ (sao cho ánh xạ $x \mapsto x_S$ là một biểu diễn của $g$ trên $S$).*

(a) *Đại số $S_0$ của các phần tử bất biến của $S$ được sinh bởi một số hữu hạn phần tử.*

(b) *Với mỗi lớp $\delta$ của các biểu diễn đơn của $g$ hữu hạn chiều trên $K$, gọi $S_\delta$ là thành phần đẳng kiểu của $S$ thuộc loài $\delta$. Khi đó $S_\delta$ là một $S_0$-môđun sinh hữu hạn.*

Gọi $\overline{S} \subset S$ là iđêan của các phần tử của $S$ không có số hạng hằng. Gọi $I$ là iđêan của $S$ được sinh bởi $S_0 \cap \overline{S}$ và gọi $(s_1, s_2, \ldots, s_p)$ là một hệ hữu hạn các phần tử sinh của iđêan $I$ (Đại số giao hoán, Chương III, § 3). Có thể giả thiết rằng các $s_i$ thuộc $S_0 \cap S̄$ và thuần nhất (các $x_S$ bảo toàn các bậc và do đó mỗi $S_\delta$ là một môđun con phân bậc). Gọi $S_1$ là đại số con của $S$ được sinh bởi 1 và các $s_i$. Khi đó $S_1 \subset S_0$. Ta chứng minh rằng $S_1 = S_0$. Vì mục đích này, ta chứng minh rằng mọi phần tử thuần nhất $s$ của $S_0$ đều thuộc $S_1$, bằng cách quy nạp theo bậc $n$ của $s$. Nếu $n = 0$, mệnh đề của ta là hiển nhiên. Do đó giả sử $n > 0$ và mệnh đề của ta đã được chứng minh khi bậc của $s$ là $< n$. Vì $s \in I$, $s = $\sum_{i=1}^{p} s_i s'_i$, trong đó các $s'_i$ là các phần tử của $S$ có thể giả thiết là thuần nhất, với deg(s'_i) = deg(s) − deg(s_i) < n. Có thể áp dụng Bổ đề 5, vì $g$-môđun $S$ là nửa đơn (no. 5, Hệ quả 2 của Định lý 4); theo ký hiệu của bổ đề này,

$$
s = s^{\natural} = \sum_{i=1}^{p} (s_i s'_i)^{\natural} = \sum_{i=1}^{p} s_i {s'_i}^{\natural}.
$$

Các {s'_i}^{\natural} là các phần tử của $S_0$ thuần nhất và có bậc $< n$ (vì mỗi $S_\delta$ là một môđun con phân bậc). Do đó chúng thuộc $S_1$ theo giả thiết quy nạp. Vậy $s \in S_1$, điều này chứng minh (a).

Bây giờ ta xét một biểu diễn đơn của $g$ thuộc lớp $\delta$ trên một không gian hữu hạn chiều $M$. Gọi L = $\mathcal{L}_K(M, S)$. Với mọi s ∈ S và mọi f ∈ L, gọi sf là phần tử của L được xác định bởi (sf)(m) = s.f(m) (m ∈ M); do đó một cấu trúc $S$-môđun được xác định trên L; vì M hữu hạn chiều trên K, rõ ràng L là một $S$-môđun sinh hữu hạn và do đó là một $S$-môđun Noether vì vành S là Noether. Mặt khác, L có một cấu trúc $g$-môđun chính tắc. Với mỗi số nguyên n ≥ 0, gọi S^n là tập hợp các phần tử thuần nhất của S có bậc n; khi đó $g$-môđun $\mathcal{L}_K(M, S^n)$ là nửa đơn (no. 5, Hệ quả 3 của Định lý 4) và do đó $g$-môđun L là nửa đơn. Hơn nữa, với s ∈ S, f ∈ L, x ∈ g và m ∈ M,

$$
(x_L(sf))(m) = x_S((sf)(m)) - (sf)(x_M m)
= x_S(s.f(m)) - s.f(x_M m)
= (x_S s).f(m) + s.(x_S f(m)) - s.f(x_M m)
= ((x_S s)f)(m) + (s(x_L f))(m)
$$

và do đó $x_L(sf) = (x_S s)f + s(x_L f)$. Vì vậy ta có thể áp dụng Bổ đề 5.

Tập con L_0 của các phần tử bất biến của L chính là tập hợp các đồng cấu của $g$-môđun M vào $g$-môđun S. Do đó, nếu φ ký hiệu cho đồng cấu chính tắc của M ⊗_K L lên S, $\phi(M \otimes_K L_0) = S_\delta$. Vì φ hiển nhiên là một đồng cấu $S$-môđun, chỉ cần chứng minh rằng L_0 là một $S_0$-môđun sinh hữu hạn. Gọi J là $S$-môđun con của L được sinh bởi L_0. Vì L là một $S$-môđun Noether, tồn tại một dãy hữu hạn (f_1, ..., f_q) các phần tử của L_0 sinh ra $S$-môđun J. Gọi L_1 là $S_0$-môđun được sinh bởi f_1, \ldots, f_q. Khi đó L_1 \subset L_0. Mặt khác, nếu f \in L_0, thì $f = \sum_{i=1}^q s_i f_i$ với $s_i \in S$ với mọi $i$ và do đó theo Bổ đề 5 mà ta dùng ký hiệu:

$$
f = f^\mathfrak{h} = \left( \sum_{i=1}^q s_i f_i \right)^\mathfrak{h} = \sum_{i=1}^q s_i^\mathfrak{h} f_i \in L_1.
$$

Do đó $L_0 = L_1$, vậy $L_0$ là một $S_0$-môđun sinh hữu hạn.

### 10. ĐỔI TRƯỜNG CƠ SỞ

Cho $K_1$ là một mở rộng giao hoán của $K$. Để một đại số Lie $g$ trên $K$ là nửa đơn, điều kiện cần và đủ là $g_{(K_1)}$ là nửa đơn; vì dạng Killing $\beta_1$ của $g_{(K_1)}$ được dẫn xuất từ dạng Killing $\beta$ của $g$ bằng cách mở rộng trường cơ sở từ $K$ đến $K_1$; do đó $\beta_1$ không suy biến khi và chỉ khi $\beta$ không suy biến (*Algebra*, Chương IX, § 1, no. 4, Hệ quả của Mệnh đề 3).

Nếu $g_{(K_1)}$ là đơn, thì $g$ là nửa đơn theo trên và không thể là một tích của hai iđêan khác không, do đó $g$ là đơn. Mặt khác nếu $g$ là đơn thì $g_{(K_1)}$ (vốn là nửa đơn) có thể không đơn (Các bài tập 17 và 26 (b)).

Cho $g$ là một đại số Lie và $r$ là căn của nó. Khi đó $r_{(K_1)}$ là căn của $g_{(K_1)}$ (\S 5, no. 6). Vì vậy, nếu $s$ ký hiệu căn lũy linh của $g$, thì căn lũy linh của $g_{(K_1)}$ là $[g_{(K_1)}, r_{(K_1)}] = [g, r]_{(K_1)} = s_{(K_1)}$. Suy ra rằng $g$ là khả quy khi và chỉ khi $g_{(K_1)}$ là khả quy.

Cho $g$ là một đại số Lie và $h$ là một đại số con. Nhắc lại rằng một biểu diễn của $h$ là nửa đơn khi và chỉ khi biểu diễn của $h_{(K_1)}$ được dẫn xuất bằng cách mở rộng trường cơ sở đến $K_1$ là nửa đơn. Do đó $h$ là khả quy trong $g$ khi và chỉ khi $h_{(K_1)}$ là khả quy trong $g_{(K_1)}$.

Bây giờ cho $K_0$ là một trường con của $K$ sao cho $[K : K_0]$ hữu hạn. Cho $g$ là một đại số Lie và $g_0$ là đại số Lie (hữu hạn chiều) dẫn xuất từ $g$ bằng cách hạn chế trường cơ sở từ $K$ xuống $K_0$. Mọi iđêan giao hoán của $g$ đều là một iđêan giao hoán của $g_0$; ngược lại, nếu $a_0$ là một iđêan giao hoán của $g_0$ thì không gian vectơ nhỏ nhất trên $K$ của $g$ chứa $a_0$ là một iđêan giao hoán của $g$; do đó $g$ là nửa đơn khi và chỉ khi $g_0$ là nửa đơn. Nếu $g_0$ là đơn thì rõ ràng $g$ là đơn. Ngược lại, giả sử $g$ là đơn. Ta chứng minh rằng $g_0$ là đơn. Cho $a_0$ là một thành phần đơn của $g_0$. Với mọi $\lambda \in K^*$, $\lambda a_0$ là một iđêan của $g_0$ và

$$
[a_0, \lambda a_0] = \lambda [a_0, a_0] = \lambda a_0 \neq \{0\},
$$

do đó $\lambda a_0 \supset a_0$ và vì vậy $\lambda a_0 = a_0$ vì $\dim_{K_0}(\lambda a_0) = \dim_{K_0} a_0$. Khi đó không gian vectơ của $g$ được sinh bởi $a_0$ là một iđêan khác không của $g$ và do đó là toàn bộ $g$. Suy ra $g = a_0$, điều này chứng minh mệnh đề của chúng ta.

### Bài tập {#lie-i-s6-exercises}

Các quy ước của § 6 vẫn có hiệu lực trừ khi có quy định khác.

Xem [các bài tập của § 6](exercises/s6/).
