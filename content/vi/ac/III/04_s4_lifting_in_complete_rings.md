---
book: ac
book_title: Commutative Algebra
chapter: III
chapter_title: GRADUATIONS. FILTRATIONS AND TOPOLOGIES
section: 4
section_title: Lifting in complete rings
lang: vi
source: ac-i-vii
book_pages: 209-226, 255-258
pdf_pages: 0229-0246, 0275-0278
extraction: ocr
subsections:
    - "no": 1
      title: STRONGLY RELATIVELY PRIME POLYNOMIALS
      page: 209
      pdf_page: 229
    - "no": 2
      title: RESTRICTED FORMAL POWER SERIES
      page: 212
      pdf_page: 232
    - "no": 3
      title: HENSEL'S LEMMA
      page: 215
      pdf_page: 235
    - "no": 4
      title: COMPOSITION OF SYSTEMS OF FORMAL POWER SERIES
      page: 218
      pdf_page: 238
    - "no": 5
      title: SYSTEMS OF EQUATIONS IN COMPLETE RINGS
      page: 220
      pdf_page: 240
    - "no": 6
      title: APPLICATION TO DECOMPOSITIONS OF RINGS
      page: 225
      pdf_page: 245
statements: 23
exercises: 8
content_sha256: 0c18e3ecba56fd218bf6fbaa147bc44b6f6f2b47d386dced05f23531591c268d
translated_from: content/en/ac/III/04_s4_lifting_in_complete_rings.md
source_content_sha256: fd6d32d67de2e7a2c06665c283c603769abbecc18a747834d78b6d8b219cd8d3
translation_model: gpt-5-6-mini, gpt-5-6, gpt-5.4
translation_run: translate-vi-76b01779
glossary_version: 34
glossary_terms_sha256: b18fc10f51fd09085e3e1b146a2321b359a03ac645bf3dac4e7e1bae34e106c1
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 4. NÂNG LÊN TRONG CÁC VÀNH ĐẦY ĐỦ

### 1. CÁC ĐA THỨC NGUYÊN TỐ CÙNG NHAU MẠNH

Cho $R$ là một vành giao hoán. Hai phần tử $x, y$ của $R$ được gọi là *nguyên tố cùng nhau mạnh* nếu các iđêan chính $Rx$ và $Ry$ là nguyên tố cùng nhau, nói cách khác (Chương II, § 1, no. 2) nếu $R x + R y = R$; điều này tương đương với việc nói rằng tồn tại hai phần tử $a, b$ của $R$ sao cho $ax + by = 1$.

**Bổ đề 1 ("Bổ đề Euclid").** *Cho $x, y$ là hai phần tử nguyên tố cùng nhau mạnh của $R$; nếu $z \in R$ là sao cho $x$ chia hết $yz$, thì $x$ chia hết $z$.*

Nếu $1 = ax + by$, thì $z = x(az) + (yz)b$.

Nếu $x$ và $y$ là nguyên tố cùng nhau mạnh trong $R$, thì
$$
R_{xy} = (Rx) \cap (Ry)
$$
(Chương II, § 1, no. 2, Mệnh đề 5); nếu $R$ là một miền nguyên, hai phần tử nguyên tố cùng nhau mạnh khi đó có *bội chung nhỏ nhất* bằng tích của chúng (*Đại số*, Chương VI, § 1, no. 8) và do đó là *nguyên tố cùng nhau* theo nghĩa của *Đại số*, Chương VI, § 1, no. 12. Ngược lại, nếu $R$ là một miền iđêan chính, hai phần tử nguyên tố cùng nhau cũng là nguyên tố cùng nhau mạnh, như suy ra từ đồng nhất thức Bezout (*Đại số*, Chương VII, § 1, no. 2, Định lý 1).

Đối với các vành đa thức ta có kết quả sau:

#### Mệnh đề 1 {#ac-iii-s4-prop-1 .statement}

*Cho $\mathbf{A}$ là một vành giao hoán và $P$ và $P'$ là hai đa thức nguyên tố cùng nhau mạnh trong $\mathbf{A}[X]$. Giả sử rằng $P$ là đơn thức cao nhất và có bậc $s$. Khi đó mọi đa thức $T$ trong $\mathbf{A}[X]$ có thể được viết duy nhất dưới dạng*
$$
T = PQ + P'Q'
$$
*trong đó $Q \in \mathbf{A}[X]$, $Q' \in \mathbf{A}[X]$ và $\deg(Q') < s$.
Nếu thêm nữa $\deg(T) \leq t$ và $\deg(P') \leq t - s$, thì $\deg(Q) \leq t - s$.*

Vì $P$ là đơn thức cao nhất, $PR \neq 0$ đối với mọi đa thức $R \neq 0$ của $\mathbf{A}[X]$ và trong trường hợp này $\deg(PR) = s + \deg(R)$.

Cho $T$ là một đa thức bất kỳ trong $\mathbf{A}[X]$. Vì iđêan sinh bởi $P$ và $P'$ là toàn bộ $\mathbf{A}[X]$, tồn tại các đa thức $Q_1$ và $Q'$ sao cho
$$
T = PQ_1 + P'_1Q'_1;
$$
vì $P$ là đơn thức bậc cao nhất của bậc $s$, phép chia Euclid (*Algebra*, Chương IV, § 1, no. 5) chỉ ra rằng tồn tại hai đa thức $Q', Q''$ sao cho $Q'_1 = PQ'' + Q'$ trong đó $\deg(Q') < s$; khi đó ta suy ra rằng
$$
T = PQ_1 + P'(PQ'' + Q') = PQ + P'Q'
$$
trong đó $Q = Q_1 + P'Q''$. Để chứng minh tính duy nhất của công thức (1), chỉ cần chứng minh rằng các hệ thức
$$
0 = PQ + P'Q', \quad \deg(Q') < s
$$
suy ra $Q = Q' = 0$. Bây giờ, nếu (2) đúng, $P$ chia $-PQ = P'Q'$ và, vì $P$ và

P' nguyên tố cùng nhau mạnh, P chia Q' theo Bổ đề 1; nếu Q' ≠ 0, sẽ tồn tại một đa thức S ≠ 0 sao cho Q' = PS, do đó

$$
\deg(Q') = s + \deg(S) \geq s,
$$

điều này là một mâu thuẫn. Ta kết luận rằng Q' = 0, do đó PQ = 0 và cuối cùng Q = 0 theo nhận xét ở đầu.

Cuối cùng, giả sử rằng $\deg(T) \leq t$ và $\deg(P') \leq t - s$; với đa thức T ở dạng (1),

$$
\deg(P'Q') \leq \deg(P') + \deg(Q') < s + \deg(P') \leq t
$$

và do đó

$$
s + \deg(Q) = \deg(PQ) = \deg(T - P'Q') \leq t
$$

do đó $\deg(Q) \leq t - s$.

#### Ví dụ {#ac-iii-s4-n1-exa-1 .statement}

Để một đa thức $P \in \mathbf{A}[X]$ nguyên tố cùng nhau mạnh với $X - a$ (trong đó $a \in \mathbf{A}$), điều kiện cần và đủ là $P(a)$ khả nghịch trong $\mathbf{A}$. Thật vậy, nếu P và $X - a$ nguyên tố cùng nhau mạnh, từ Mệnh đề 1 suy ra rằng tồn tại $c \in \mathbf{A}$ và một đa thức $Q \in \mathbf{A}[X]$ sao cho $cP + (X - a)Q = 1$, do đó $cP(a) = 1$ và $P(a)$ khả nghịch. Ngược lại, theo phép chia Euclid

$$
P = (X - a)R + P(a)
$$

và, nếu $P(a) = b^{-1}$, trong đó $b \in \mathbf{A}$, ta suy ra rằng $1 = bP - b(X - a)R$, điều này chỉ ra rằng P và $X - a$ nguyên tố cùng nhau mạnh.

Cho $\mathbf{A}$ và $\mathbf{B}$ là hai vành giao hoán và $f : \mathbf{A} \to \mathbf{B}$ là một đồng cấu vành. Nếu $P = \sum_{i \geq 0} a_i X^i$ là một chuỗi lũy thừa hình thức trong $\mathbf{A}[[X]]$, ký hiệu $\bar{f}(P)$ là chuỗi lũy thừa hình thức $\sum_{i \geq 0} f(a_i) X^i$ trong $\mathbf{B}[[X]]$. Nếu P là một đa thức, thì $\bar{f}(P)$ cũng là một đa thức và, nếu thêm nữa P là đơn thức cao nhất, thì $\bar{f}(P)$ là đơn thức cao nhất cùng bậc với P. Cuối cùng, $P \mapsto \bar{f}(P)$ rõ ràng là một đồng cấu từ $\mathbf{A}[[X]]$ vào $\mathbf{B}[[X]]$ mở rộng $f$ và biến X thành X. *Ký hiệu này sẽ được sử dụng thường xuyên theo nghĩa này trong phần còn lại của đoạn này.*

#### Mệnh đề 2 {#ac-iii-s4-prop-2 .statement}

*Cho $\mathbf{A}$ và $\mathbf{B}$ là hai vành giao hoán, $f$ một đồng cấu từ $\mathbf{A}$ đến $\mathbf{B}$ và $P, P'$ là hai đa thức trong $\mathbf{A}[X]$. Nếu $P$ và $P'$ nguyên tố cùng nhau mạnh trong $\mathbf{A}[X]$, thì $\bar{f}(P)$ và $\bar{f}(P')$ nguyên tố cùng nhau mạnh trong $\mathbf{B}[X]$. Mệnh đề đảo lại là đúng khi và chỉ khi là toàn ánh, nếu hạt nhân của nó được chứa trong căn Jacobson của $\mathbf{A}$ và nếu $P$ là đơn nhất.*

Giả sử rằng P và P' nguyên tố cùng nhau mạnh; khi đó tồn tại các đa thức Q, Q' trong $\mathbf{A}[X]$ sao cho $PQ + P'Q' = 1$; ta suy ra rằng

$$
\bar{f}(P)\bar{f}(Q) + \bar{f}(P')\bar{f}(Q') = 1,
$$

do đó có mệnh đề thứ nhất. Để chứng minh mệnh đề thứ hai, gọi a là hạt nhân của $f$;

gọi $E = A[X]$ và $F$ là iđêan của $E$ sinh bởi $P$ và $P'$; vì $f$ là toàn ánh và $\bar{f}(P)$ đơn nhất, Mệnh đề 1 cho thấy rằng với mọi đa thức $T \in A[X]$ tồn tại hai đa thức $Q, Q'$ trong $A[X]$ sao cho
$$
\bar{f}(T) = \bar{f}(P) \bar{f}(Q) + \bar{f}(P') \bar{f}(Q'),
$$
do đó có quan hệ $E = F + aE$. Bây giờ, $E/F$ là một A-môđun sinh hữu hạn, vì mọi đa thức đều đồng dư mod. $P$ với một đa thức bậc $< \deg(P)$, do $P$ là đơn nhất. Vì $E/F = a(E/F)$ và a được chứa trong căn Jacobson của $A$, Bổ đề Nakayama cho thấy rằng $E/F = 0$ (Đại số, Chương VIII, § 6, no. 3, Hệ quả 2 của Mệnh đề 6 ), điều đó có nghĩa là $P$ và $P'$ nguyên tố cùng nhau mạnh.

### 2. CHUỖI LŨY THỪA HÌNH THỨC HẠN CHẾ

#### Định nghĩa 1 {#ac-iii-s4-def-1 .statement}

Một vành tôpô giao hoán $A$ được gọi là tôpô hóa tuyến tính (và tôpô của nó được gọi là tuyến tính) nếu tồn tại một hệ cơ bản $\mathcal{B}$ các lân cận $\mathfrak{o}$ gồm các iđêan $\mathfrak{o} \subset A$.

Lưu ý rằng trong một vành như vậy, các iđêan $3 \in \mathcal{B}$ là mở và đóng (Tôpô đại cương, chương 111, § 2, no. 1, Hệ quả của Mệnh đề 4 ). Với mọi $3 \in \mathcal{B}$, vành tôpô thương $A/\mathfrak{J}$ khi đó là rời rạc; với $8 \in \mathcal{B}$, $8' \in \mathcal{B}$, $\mathfrak{J}' \subset 8$, đặt
$$
h_{\mathfrak{J}\mathfrak{J}'} : A/\mathfrak{J}' \to A/\mathfrak{J}
$$
là ánh xạ chính tắc. Ta biết (Tôpô đại cương, chương III, § 7, no. 3) rằng $(A/\mathfrak{J}, h_{\mathfrak{J}\mathfrak{J}'})$ là một hệ ngược của các vành rời rạc (đối với tập chỉ số $\mathcal{B}$ có thứ tự bởi $\supset$ và có hướng), mà giới hạn ngược của nó là một vành Hausdorff đầy đủ được tôpô hóa tuyến tính $\tilde{A}$; hơn nữa (sđd., Mệnh đề 2 ), một cấu xạ ngặt $i : A \to \tilde{A}$ được xác định, có hạt nhân là bao đóng của $\{0\}$ trong $A$ và có ảnh trù mật khắp nơi trong $\tilde{A}$, sao cho $\tilde{A}$ được đồng nhất một cách chính tắc với phần đầy đủ Hausdorff của $A$.

#### Định nghĩa 2 {#ac-iii-s4-def-2 .statement}

Cho một vành tôpô giao hoán $A$, một chuỗi lũy thừa hình thức
$$
T = \sum_{(n_i)} c_{n_1 n_2 \ldots n_p} X_1^{n_1} X_2^{n_2} \ldots X_p^{n_p}
$$
trong vành $A[[X_1, \ldots, X_p]]$ được gọi là hạn chế nếu, với mọi lân cận $V$ của 0 trong $A$, chỉ có một số hữu hạn các hệ số $c_{n_1 n_2 \ldots n_p}$ không thuộc $V$ (nói cách khác, họ $(c_{n_1 n_2 \ldots n_p})$ tiến tới 0 trong $A$ đối với bộ lọc các phần bù của các tập con hữu hạn của $\mathbf{N}^p$).

Nếu $A$ được tôpô hóa tuyến tính, các chuỗi lũy thừa hình thức hạn chế trong $A[[X_1, \ldots, X_p]]$ tạo thành một vành con của $A[[X_1, \ldots, X_p]]$, được ký hiệu là $A\{X_1, \ldots, X_p\}$: vì nếu
$$
T = \sum_{(n_i)} c_{n_1 \ldots n_p} X_1^{n_1} \ldots X_p^{n_p}, \quad T' = \sum_{(n_i)} c'_{n_1 \ldots n_p} X_1^{n_1} \ldots X_p^{n_p}
$$
là hai chuỗi lũy thừa hình thức hạn chế và $\mathfrak{J}$ là một lân cận của 0 trong $A$ là một iđêan của $A$, tồn tại một số nguyên $m$ sao cho $c_{n_1 \ldots n_p} \in \mathfrak{z}$ và $c'_{n_1 \ldots n_p} \in \mathfrak{g}$ với mọi hệ $(n_1, \ldots, n_p)$ sao cho $n_k \geq m$ đối với ít nhất một chỉ số $k$; khi đó, nếu

$$
T'' = TT' = \sum_{(n_i)} c''_{n_1 \ldots n_p} X_1^{n_1} \ldots X_p^{n_p},
$$

thì $c''_{n_1 \ldots n_p} = \sum c_{r_1 \ldots r_p} c'_{s_1 \ldots s_p}$ đối với mọi hệ $(r_k), (s_k)$ sao cho $r_k + s_k = n_k$ với $1 \leq k \leq p$; ta kết luận rằng nếu $n_k \geq 2m$, thì $r_k \geq m$ hoặc $s_k \geq m$ và do đó, vì $\mathfrak{z}$ là một iđêan, $c''_{n_1 \ldots n_p} \in \mathfrak{g}$ chừng nào $n_k \geq 2m$ đối với ít nhất một $k$, điều này thiết lập mệnh đề của ta. Hơn nữa, mọi đạo hàm $\partial T / \partial X_i$ ($1 \leq i \leq p$) của một chuỗi lũy thừa hình thức hạn chế đều hạn chế, như suy ra ngay lập tức từ định nghĩa và sự kiện rằng các lân cận $\mathfrak{z} \in \mathscr{B}$ là các nhóm con cộng tính của $\mathbf{A}$.

Nếu $\mathbf{A}$ là rời rạc, vành các chuỗi lũy thừa hình thức hạn chế chỉ là vành đa thức $\mathbf{A}[X_1, \ldots, X_n]$.

Luôn luôn giả sử rằng $\mathbf{A}$ là được trang bị tôpô tuyến tính và cho $\mathscr{B}$ là một hệ cơ sở các lân cận của 0 trong $\mathbf{A}$ gồm các iđêan của $\mathbf{A}$; với mọi $\mathfrak{g} \in \mathscr{B}$, cho $p_\mathfrak{g}: \mathbf{A} \to \mathbf{A}/\mathfrak{g}$ là đồng cấu chính tắc. Theo định nghĩa, với mọi chuỗi lũy thừa hình thức hạn chế $T \in \mathbf{A}\{X_1, \ldots, X_n\}$,

$$
\bar{p}_\mathfrak{g}(T) \in (\mathbf{A}/\mathfrak{g})[X_1, \ldots, X_p].
$$

Rõ ràng

$$
((\mathbf{A}/\mathfrak{g})[X_1, \ldots, X_p], \bar{h}_{\mathfrak{g}\mathfrak{g}'})
$$

là một hệ ngược các vành (đối với tập chỉ số có hướng $\mathscr{B}$) và $(\bar{p}_\mathfrak{g})$ là một hệ ngược các đồng cấu $\mathbf{A}\{X_1, \ldots, X_n\} \to (\mathbf{A}/\mathfrak{g})[X_1, \ldots, X_p]$; vì mọi đa thức đều là một chuỗi lũy thừa hình thức hạn chế, $\bar{p}_\mathfrak{g}$ là toàn ánh; hạt nhân của nó $N_\mathfrak{g}$ là iđêan của $\mathbf{A}\{X_1, \ldots, X_n\}$ gồm các chuỗi lũy thừa hình thức hạn chế mà tất cả các hệ số của chúng đều thuộc $\mathfrak{g}$; ta sẽ trang bị cho $\mathbf{A}\{X_1, \ldots, X_n\}$ tôpô (tuyến tính) mà đối với nó các $N_\mathfrak{g}$ (với $\mathfrak{g} \in \mathscr{B}$) tạo thành một hệ cơ sở các lân cận của 0 (một tôpô rõ ràng chỉ phụ thuộc vào tôpô trên $\mathbf{A}$). Khi đó, theo Tôpô đại cương, Chương III, § 7, no. 3, Mệnh đề 2, ta có

$$
\pi = \lim_{\leftarrow} \bar{p}_\mathfrak{g}: \mathbf{A}\{X_1, \ldots, X_n\} \to \lim_{\rightarrow} (\mathbf{A}/\mathfrak{g})[X_1, \ldots, X_p]
$$

là một cấu xạ ngặt có hạt nhân là bao đóng của $\{0\}$ trong $\mathbf{A}\{X_1, \ldots, X_n\}$ và có ảnh trù mật trong

$$
\mathbf{A}' = \lim_{\rightarrow} (\mathbf{A}/\mathfrak{g})[X_1, \ldots, X_n].
$$

#### Mệnh đề 3 {#ac-iii-s4-prop-3 .statement}

*Nếu vành giao hoán $\mathbf{A}$ được trang bị tôpô tuyến tính là Hausdorff và đầy đủ, thì đồng cấu chính tắc $\pi$ là một đẳng cấu vành tôpô.*

Với mọi $(n_1, \ldots, n) \in \mathbf{N}^p$ và mọi $3 \in \mathcal{B}$, cho $\phi_{n_1 \ldots n_p}^3$ là ánh xạ $(A/\mathfrak{J})[X_1, \ldots, X_p] \to A/\mathfrak{J}$ biến mọi đa thức thành hệ số của $X_1^{n_1} \ldots X_p^{n_p}$ trong đa thức này; rõ ràng các $\phi_{n_1 \ldots n_p}^3$ tạo thành một hệ ngược các đồng cấu môđun $(A/\mathfrak{J})$ (đối với tập có thứ tự $\mathcal{B}$) và, vì $A$ được đồng nhất một cách chính tắc với $\lim_{\leftarrow} (A/\mathfrak{J})$ theo giả thiết, $\phi_{n_1 \ldots n_p} = \lim_{\leftarrow} \phi_{n_1 \ldots n_p}^3$ là một $A$-đồng cấu liên tục từ $A'$ vào $A$. Với mọi phần tử $S = (S_\mathfrak{J})_{\mathfrak{J} \in \mathcal{B}}$ của $A'$, ta sẽ thấy rằng chuỗi lũy thừa hình thức $T = \sum_{(n_i)} \phi_{n_1 \ldots n_p}(S) X_1^{n_1} \ldots X_p^{n_p}$ là hạn chế và thỏa mãn $\pi(T) = S$. Với mọi $3 \in \mathcal{B}$ và mọi $\mathfrak{J}' \in \mathcal{B}$ sao cho $\mathfrak{J}' \subset \mathfrak{J}$, quan hệ $\phi_{n_1 \ldots n_p}^{\mathfrak{J}'}(S_{\mathfrak{J}'}) = 0$ kéo theo
$$
\phi_{n_1 \ldots n_p}^{\mathfrak{J}'}(S_{\mathfrak{J}'}) \in \mathfrak{J}/\mathfrak{J}'
$$
vì $S_{\mathfrak{J}}$ là một đa thức, ta thấy rằng $\phi_{n_1 \ldots n_p}(S) \in \mathfrak{J}$ ngoại trừ các $(n_1, \ldots, n_p)$, có số lượng hữu hạn, sao cho $\phi_{n_1 \ldots n_p}^{\mathfrak{J}}(S_{\mathfrak{J}}) \neq 0$, điều này chứng minh mệnh đề đầu tiên của ta; mệnh đề thứ hai suy ra từ các định nghĩa. Vì $A$ là Hausdorff, giao của các $\mathbf{N}_\mathfrak{J}$ thu gọn về 0 và do đó $\pi$ là *song ánh*, điều này hoàn tất chứng minh, vì $\pi$ là một cấu xạ ngặt.

#### Mệnh đề 4 {#ac-iii-s4-prop-4 .statement}

*Cho $A, B$ là hai vành giao hoán có tôpô tuyến tính, $B$ là Hausdorff và đầy đủ, và $u : A \to B$ là một đồng cấu liên tục. Với mọi họ $b = (b_i)_{1 \leq i \leq p}$ các phần tử của $B$, tồn tại một đồng cấu liên tục duy nhất*
$$
\tilde{u} : A\{X_1, \ldots, X_p\} \to B
$$
*thỏa mãn $\tilde{u}(a) = u(a)$ với mọi $a \in A$ và $\tilde{u}(X_i) = b_i$ với $1 \leq i \leq p$.*

Tồn tại một đồng cấu duy nhất $v : A[X_1, \ldots, X_p] \to B$ thỏa mãn $v(a) = u(a)$ với $a \in A$ và $v(X_i) = b_i$ với $1 \leq i \leq p$. Hơn nữa, nếu $\mathfrak{J}$ là một lân cận của 0 trong $B$ là một iđêan, $\overline{u}^{-1}(\mathfrak{J}) = 3$ là một iđêan của $A$ là một lân cận của 0 và, với mọi đa thức $P \in \mathbf{N}_\mathfrak{J}$, rõ ràng $v(P) \in \mathfrak{J}$ và do đó $v$ liên tục. Vì $A[X_1, \ldots, X_p]$ trù mật trong $A\{X_1, \ldots, X_p\}$, sự tồn tại và tính duy nhất của $\tilde{u}$ suy ra từ *Tôpô đại cương*, Chương 111,§ 3, no. 3, Mệnh đề 5 và nguyên lý mở rộng của các đồng nhất thức.

Trong trường hợp đặc biệt khi $A = B$ và $u$ là ánh xạ đồng nhất, ta sẽ viết $f(b_1, \ldots, b_p)$ hoặc $f(b)$ cho giá trị của $\tilde{u}(f)$ với mọi chuỗi lũy thừa hình thức hạn chế $f \in A\{X_1, \ldots, X_p\}$.

*Các nhận xét*

#### Nhận xét 1 {#ac-iii-s4-n2-rem-1 .statement}

Mệnh đề 4 chứng minh rằng với mọi iđêan *đóng* $a$ trong một vành $A$ được giả thiết là Hausdorff và đầy đủ, các quan hệ $b_i \in a$ với $1 \leq i \leq p$ kéo theo $f(b_1, \ldots, b_p) \in a$ với mọi chuỗi lũy thừa hình thức hạn chế $f \in A\{X_1, \ldots, X_p\}$.

#### Nhận xét 2 {#ac-iii-s4-n2-rem-2 .statement}

Giả sử rằng $A$ có tôpô tuyến tính; cho $r$ là một số nguyên sao cho 1 $\leq r \leq p$ và cho vành $A\{X_1, \ldots, X_r\}$ được trang bị tôpô đã định nghĩa ở trên. Khi đó vành tôpô $A\{X_1, \ldots, X_r\}$ được đồng nhất với vành các chuỗi lũy thừa hình thức hạn chế

$$
(A\{X_1, \ldots, X_r\})\{X_{r+1}, \ldots, X_p\}
$$

như suy ra ngay lập tức từ các định nghĩa.

#### Nhận xét 3 {#ac-iii-s4-n2-rem-3 .statement}

Với ký hiệu của *Nhận xét 2*, giả sử thêm rằng $A$ là Hausdorff và đầy đủ và hãy viết mọi chuỗi lũy thừa hình thức hạn chế $f \in A\{X_1, \ldots, X_r\}$ dưới dạng

$$
f = \sum_{(n_i)} c_{n_{r+1} \ldots n_p}(X_1, \ldots, X_r) X_{r+1}^{n_{r+1}} \ldots X_p^{n_p}
$$

trong đó các $c_{n_{r+1} \ldots n_p}$ là các chuỗi lũy thừa hình thức hạn chế. Với mọi hệ $x = (x_1, \ldots, x_r)$ các phần tử của $A$, đặt

$$
b_{n_{r+1} \ldots n_p} = c_{n_{r+1} \ldots n_p}(x_1, \ldots, x_p).
$$

Suy ra ngay lập tức từ *Nhận xét 1* rằng $\sum_{(n_i)} b_{n_{r+1} \ldots n_p} X_{r+1}^{n_{r+1}} \ldots X_p^{n_p}$ là một chuỗi lũy thừa hình thức *hạn chế* được ký hiệu bởi $f(x_1, \ldots, x_r, X_{r+1}, \ldots, X_p)$; nó được gọi là thu được bằng cách *thế* các $x_i$ cho các $X_i$ với $1 \leq i \leq r$ trong $f$.

### 3. BỔ ĐỀ HENSEL

Trong một vành tôpô $A$, một phần tử $x$ được gọi là *lũy linh tôpô* nếu $O$ là giới hạn của dãy $(x^n)_{n \geq 0}$. Nếu $A$ là một vành giao hoán *có tôpô tuyến tính*, việc nói rằng $x$ là lũy linh tôpô có nghĩa là với mọi iđêan mở $\mathfrak{J}$ của $A$, ảnh chính tắc của $x$ trong $A/\mathfrak{J}$ là một phần tử *lũy linh* của vành đó. Nếu $\mathfrak{r}_g$ là căn nil của $A/\mathfrak{J}$, rõ ràng $(\mathfrak{r}_g)$ là một hệ ngược của các tập hợp và tập hợp $t$ các phần tử lũy linh tôpô của $A$ là ảnh ngược của $\mathfrak{r} = \lim \mathfrak{r}_g$ qua đồng cấu chính tắc $A \to \lim A/\mathfrak{J}$; do đó nó là một *iđêan đóng* của $A$. Nếu ngoài ra $A$ là *Hausdorff* và *đầy đủ*, iđêan này được chứa trong căn Jacobson của $A$ và, để một phần tử $x \in A$ là khả nghịch, điều kiện cần và đủ là lớp của nó mod. $t$ là khả nghịch trong $A/t$ (\S 2, no. 13, Bổ đề 3).

Chú ý rằng nếu $A$ là một vành và $m$ là một iđêan hai phía của $A$, các phần tử của $m$ là lũy linh tôpô đối với tôpô *m-adic*.

**Định lý 1 (Hensel)**. Cho $A$ là một vành giao hoán có tôpô tuyến tính Hausdorff đầy đủ. Cho $m$ là một iđêan đóng của $A$ mà các phần tử của nó là lũy linh tôpô. Cho $B = A/m$ là vành tôpô thương và $\varphi : A \to B$ là ánh xạ chính tắc. Cho $R$ là một chuỗi lũy thừa hình thức hạn chế trong $A\{X\}$, $\overline{P}$ là một đa thức đơn khởi trong $B[X]$ và $\overline{Q}$ là một chuỗi lũy thừa hình thức hạn chế trong $B\{X\}$. Giả sử rằng $\overline{\varphi}(R) = \overline{P} \cdot \overline{Q}$ và rằng $\overline{P}$ và $\overline{Q}$ nguyên tố cùng nhau mạnh trong $B\{X\}$. Khi đó tồn tại duy nhất một cặp có thứ tự $(P, Q)$ gồm một đa thức đơn khởi $P \in A[X]$ và một chuỗi lũy thừa hình thức hạn chế $Q \in A\{X\}$ sao cho
(4)
$$
R = P.Q, \quad \bar{\varphi}(P) = P, \quad \bar{\varphi}(Q) = \overline{Q}.
$$
Hơn nữa, $P$ và $Q$ nguyên tố cùng nhau mạnh trong $A\{X\}$ và, nếu $R$ là một đa thức, thì $Q$ cũng là một đa thức.

Chứng minh được chia thành bốn bước. Trong ba bước đầu tiên ta giả sử rằng $A$ là rời rạc, trong trường hợp đó $R$ và $\overline{Q}$ là các đa thức.

(I) $m^2 = 0$
Cho $S, T$ là hai đa thức của $A[X]$ sao cho $S$ là đơn khởi và $\bar{\varphi}(S) = \overline{P}$, $\bar{\varphi}(T) = \overline{Q}$; Mệnh đề 2 của no. 1 chứng minh rằng $S$ và $T$ nguyên tố cùng nhau mạnh; do đó (no. 1, Mệnh đề 1) tồn tại một cặp có thứ tự duy nhất gồm các đa thức $(S', T')$ của $A[X]$ sao cho
(5)
$$
R - ST = ST' + TS' \quad \text{và} \quad \deg(S') < \deg(S) = \deg(\overline{P}).
$$
Các đa thức $P = S + TS'$, $Q = T + T'$ khi đó là nghiệm của bài toán; hơn nữa thực vậy
(6)
$$
\overline{P} \cdot \bar{\varphi}(T') + \overline{Q} \cdot \bar{\varphi}(S') = \bar{\varphi}(ST' + TS') = \bar{\varphi}(R - ST) = 0.
$$
Vì $\overline{P}$ là đơn khởi, $\overline{P}$ và $\overline{Q}$ nguyên tố cùng nhau mạnh và
$$
\deg(\bar{\varphi}(S')) < \deg(\overline{P}),
$$
Mệnh đề 1 của no. 1 chỉ ra rằng $\bar{\varphi}(S') = \bar{\varphi}(T') = 0$, nói cách khác các hệ số của $S'$ và $T'$ thuộc $m$ và quan hệ $m^2 = 0$ cho
$$
PQ = ST + ST' + TS' = R,
$$
thỏa mãn quan hệ (4). Vì $\bar{\varphi}(P) = \overline{P}$ và $\bar{\varphi}(Q) = \overline{Q}$, $P$ và $Q$ nguyên tố cùng nhau mạnh (no. 1, Mệnh đề 2); cuối cùng, nếu $P_1$ và $Q_1$ là hai đa thức khác trong $A[X]$ thỏa mãn (4) và sao cho $P_1$ là đơn khởi, thì tất yếu, đặt $S'_1 = P_1 - S, \ T'_1 = Q_1 - T, \ \deg(S'_1) < \deg(S)$ và $R - ST = ST'_1 + TS'_1$ vì $S'_1$ và $T'_1$ có các hệ số của chúng thuộc $m$; nhưng Mệnh đề 1 khi đó chứng minh rằng $S' = S'_1$ và $T' = T'_1$, điều này chứng minh tính duy nhất của cặp có thứ tự $(P, Q)$.

(2) $m$ là lũy linh
Cho $n$ là số nguyên nhỏ nhất sao cho $m^n = 0$ và ta lập luận bằng quy nạp theo $n > 2$, định lý đã được chứng minh cho $n = 2$. Đặt $A = A/m^{n-1}$, $m' = m/m^{n-1}$; vì $m'^{n-1} = 0$, tồn tại một cặp có thứ tự duy nhất $(P', Q')$ các đa thức trong $A'[X]$ sao cho $P'$ là monic, $R' = P'Q'$, $\psi(P') = \overline{P}$ và $\psi(Q') = \overline{Q}$, trong đó $\psi$ ký hiệu đồng cấu chính tắc $A' \to A'/m' = B$, $\theta$ ký hiệu đồng cấu chính tắc $A \to A'$ và $R' = \tilde{\theta}(R)$. Mặt khác, vì $(m^{n-1})^2 = 0$, tồn tại một cặp có thứ tự duy nhất $(P, Q)$ các đa thức trong $A[X]$ sao cho $P$ là monic và $R = PQ$, $\bar{\theta}(P) = \overline{P}$, $\bar{\theta}(Q) = \overline{Q}$; vì $\phi = \psi \circ \theta$, điều này chỉ ra sự tồn tại và tính duy nhất của $P$ và $Q$ thỏa mãn (4); hơn nữa $P'$ và $Q'$ nguyên tố cùng nhau mạnh theo giả thiết quy nạp và do đó $P$ và $Q$ cũng vậy.

(3) **A là rời rạc**

Chú ý rằng trong trường hợp này $m$ không còn nhất thiết lũy linh, nhưng theo giả thiết nó luôn là một *iđêan lũy linh*. Cho $P_0$, $Q_0$ là hai đa thức của $A[X]$ sao cho $\bar{\varphi}(P_0) = \overline{P}$, $\bar{\varphi}(Q_0) = \overline{Q}$ và $P_0$ là đơn thức đầu. Xét iđêan $n$ của $A$ sinh bởi các hệ số của $R - P_0 Q_0$; nó sinh hữu hạn và được chứa trong $m$, do đó nó *lũy linh* (chương 11, § 2, no. 6, Mệnh đề 15) và theo định nghĩa, nếu $\psi : A \to A/n$ là ánh xạ chính tắc, thì $\bar{\psi}(R) = \bar{\psi}(P_0) \bar{\psi}(Q_0)$. Hơn nữa, $\bar{\psi}(P_0)$ và $\bar{\psi}(Q_0)$ nguyên tố cùng nhau mạnh, như suy ra từ giả thiết đối với $\overline{P}$ và $\overline{Q}$ và Mệnh đề 2 của no. 1 áp dụng cho đồng cấu chính tắc $A/n \to A/m$. Theo trường hợp (2), do đó tồn tại một cặp có thứ tự $(P, Q)$ gồm các đa thức trong $A[X]$ sao cho $P$ là đơn thức đầu và các hệ thức (4) được thỏa mãn. Việc $\overline{P}$ và $\overline{Q}$ nguyên tố cùng nhau mạnh cũng kéo theo ở đây rằng $P$ và $Q$ nguyên tố cùng nhau mạnh trong $A[X]$ theo no. 1, Mệnh đề 2, vì $m$ được chứa trong căn Jacobson của $A$. Cuối cùng, giả sử $P_1$, $Q_1$ là hai đa thức trong $A[X]$ thỏa mãn (4) và $P_1$ là đơn thức đầu, và đặt $n_1$ là iđêan sinh hữu hạn của $A$ sinh bởi các hệ số của $P - P_1$ và các hệ số của $Q - Q_1$; vì $n_1$ được chứa trong $m$, nó lũy linh và, nếu $\psi_1 : A \to A/n_1$ là ánh xạ chính tắc, $\bar{\psi}_1(P) = \bar{\psi}_1(P_1)$ và
$$
\bar{\psi}_1(Q) = \bar{\psi}_1(Q_1);
$$
tính duy nhất trong trường hợp (2) do đó suy ra $P = P_1,\ Q = Q_1$.

(4) **Trường hợp tổng quát**

Cho $\mathcal{B}$ là một hệ cơ sở các lân cận của 0 trong $A$ gồm các iđêan của $A$. Với mọi $\mathfrak{s} \in \mathcal{B}$, gọi $f_{\mathfrak{s}}$ là ánh xạ chính tắc $A \to A/\mathfrak{s}$, $\phi_{\mathfrak{s}}$ là ánh xạ chính tắc
$$
A/\mathfrak{s} \mapsto (A/\mathfrak{s})/((m + \mathfrak{s})/\mathfrak{s}) = A/(m + \mathfrak{s}),
$$
$g_{\mathfrak{s}}$ là ánh xạ chính tắc $B = A/m \to A(m + \mathfrak{s})$ và đặt $R_{\mathfrak{s}} = f_{\mathfrak{s}}(R)$, $P_{\mathfrak{s}} = g_{\mathfrak{s}}(\overline{P})$, $\overline{Q}_{\mathfrak{s}} = g_{\mathfrak{s}}(\overline{Q})$. Vì mỗi vành $A/\mathfrak{s}$ là rời rạc, trường hợp (3) có thể được áp dụng cho nó và ta thấy rằng tồn tại một cặp có thứ tự duy nhất $(P_{\mathfrak{s}}, Q_{\mathfrak{s}})$ gồm các đa thức trong $(A/\mathfrak{s})[X]$ sao cho $P_{\mathfrak{s}}$ là đơn khởi và $R_{\mathfrak{s}} = P_{\mathfrak{s}} Q_{\mathfrak{s}}$, $\bar{\varphi}_{\mathfrak{s}}(P_{\mathfrak{s}}) = \overline{P}_{\mathfrak{s}}$, $\bar{\varphi}_{\mathfrak{s}}(Q_{\mathfrak{s}}) = \overline{Q}_{\mathfrak{s}}$. Tính duy nhất của cặp có thứ tự này suy ra rằng, nếu $\mathfrak{s}' \subset \mathfrak{s}$, $\mathfrak{s}' \in \mathcal{B}$ và $f_{\mathfrak{s}'\mathfrak{s}} : A/\mathfrak{s}' \to A/\mathfrak{s}$ là ánh xạ chính tắc, thì $P_{\mathfrak{s}} = f_{\mathfrak{s}'\mathfrak{s}}(P_{\mathfrak{s}'})$, $Q_{\mathfrak{s}} = f_{\mathfrak{s}'\mathfrak{s}}(Q_{\mathfrak{s}'})$. Khi đó, từ sự đồng nhất chính tắc của $A[X]$ với $\lim(A/\mathfrak{s})[X]$ (no. 2, Mệnh đề 3), suy ra rằng tồn tại $P \in A\{X\}$ và $Q \in A\{X\}$ sao cho $R = PQ$ và $\bar{f}_s(P) = P_s, \bar{f}_s(Q) = Q_s$ với mọi $s \in \mathcal{B}$. Hơn nữa,
$$
\bar{g}_s(\overline{P} - \overline{\varphi}(P)) = 0, \quad \bar{g}_s(\overline{Q} - \overline{\varphi}(Q)) = 0
$$
với mọi $s \in \mathcal{B}$, điều này có nghĩa là với mọi $\mathfrak{J} \in \mathcal{B}$ các hệ số của $\overline{P} - \overline{\varphi}(P)$ và $\overline{Q} - \overline{\varphi}(Q)$ đều thuộc $(m + \mathfrak{J})/m$. Nhưng, vì $m$ đóng trong $A$, $\bigcap_s (m + s) = m$, do đó $\overline{P} = \overline{\varphi}(P), \overline{Q} = \overline{\varphi}(Q)$ và $P$ và $Q$ khi đó hiển nhiên thỏa mãn (4); hơn nữa, vì các $P_s$ là đơn khởi và có cùng bậc, chuỗi lũy thừa hình thức hạn chế $P$ là một đa thức đơn khởi. Nếu $(P', Q')$ là một cặp có thứ tự khác thỏa mãn (4) và sao cho $P'$ là một đa thức đơn khởi, ta sẽ suy ra rằng $R_s = \bar{f}_s(P') \bar{f}_s(Q'), \bar{\varphi}_s(\bar{f}_s(P')) = \overline{P}_s$ và $\bar{\varphi}_s(\bar{f}_s(Q')) = \overline{Q}_s$ và theo tính duy nhất trong trường hợp (3) $\bar{f}_s(P') = P_s, \bar{f}_s(Q') = Q_s$ với mọi $s \in \mathcal{B}$, điều này kéo theo $P = P'$ và $Q = Q'$. Cuối cùng ta hãy chứng minh rằng $P$ và $Q$ nguyên tố cùng nhau mạnh; theo trường hợp (3) và Mệnh đề 1 của no. 1, với mọi $s \in \mathcal{B}$, tồn tại một cặp có thứ tự duy nhất $(S_s, T_s)$ gồm các đa thức trong $(A/\mathfrak{J})[X]$ sao cho
$$
1 = P_s S_s + Q_s T_s \quad \text{và} \quad \deg(T_s) < \deg(P_s) = \deg(\overline{P}).
$$
Tính duy nhất của cặp có thứ tự này cho thấy ngay lập tức rằng, với $3' \in \mathcal{B}$, $\mathfrak{J}' \subset \mathfrak{J}, S_{3'} = \bar{f}_{33'}(S_{3}), T_{3'} = \bar{f}_{33'}(T_{3});$ tính đến no. 2, Mệnh đề 3, ta kết luận rằng tồn tại hai chuỗi lũy thừa hình thức hạn chế $S, T$ của $A\{X\}$ sao cho $S_s = \bar{f}_s(S), T_s = \bar{f}_s(T)$ và $1 = PS + QT$.

Vẫn còn phải kiểm tra rằng, nếu $R$ là một đa thức thì $Q$ cũng là một đa thức. Bây giờ, các $Q_s$ là các đa thức theo phép dựng và, vì $P_s$ là đơn khởi, quan hệ $R_s = P_s Q_s$ kéo theo
$$
\deg(Q_s) \leq \deg(R_s) \leq \deg(R)
$$
với mọi $s \in \mathcal{B}$; do đó ngay lập tức suy ra kết quả cần thiết theo định nghĩa của $Q$.

### 4. HỢP THÀNH CỦA CÁC HỆ CHUỖI LŨY THỪA HÌNH THỨC

Cho $A$ là một vành giao hoán; ta sẽ nói rằng một hệ
$$
\mathbf{f} = (f_1, \ldots, f_p) \in (A[[X_1, \ldots, X_q]])^p
$$
các chuỗi lũy thừa hình thức theo các $X_j$ ($1 \leq j \leq q$), với các hệ số trong $A$, là *không có số hạng hằng* nếu điều này đúng với mọi $f_j$. Với mọi hệ (8) các chuỗi lũy thừa hình thức và mọi hệ
$$
\mathbf{g} = (g_1, \ldots, g_q) \in (A[[X_1, \ldots, X_r]])^q
$$
gồm $q$ chuỗi lũy thừa hình thức không có số hạng hằng, ta sẽ ký hiệu bởi $\mathbf{f} \circ \mathbf{g}$ (hoặc $\mathbf{f}(\mathbf{g})$) hệ các chuỗi lũy thừa hình thức $f_j(g_1, \ldots, g_q)$ ($1 \leq j \leq p$) trong
$$
(A[[X_1, \ldots, X_r]])^p
$$

(Đại số, Chương IV, § 5, no. 5). Nếu
$$
\mathbf{h} = (h_1, \ldots, h_r) \in (\mathbf{A}[[X_1, \ldots, X_s]])^r
$$
là một hệ thứ ba không có số hạng hằng, thì
$$(10)$$
$$(f \circ g) \circ h = f \circ (g \circ h).$$

Với mọi số nguyên $m$,
$$(f^{(m)} \circ g^{(m)}) \circ h^{(m)} = f^{(m)} \circ (g^{(m)} \circ h^{(m)})$$
trong đó $f^{(m)}, g^{(m)}, h^{(m)}$ ký hiệu các hệ các đa thức gồm các số hạng có bậc toàn phần $\leq m$ trong các hệ chuỗi lũy thừa hình thức $f, g, h$. Nhưng rõ ràng các số hạng có bậc toàn phần $\leq m$ trong chuỗi của $(f \circ g) \circ h$ (tương ứng $f \circ (g \circ h)$) cũng chính là các số hạng trong $(f^{(m)} \circ g^{(m)}) \circ h^{(m)}$ (tương ứng $f^{(m)} \circ (g^{(m)} \circ h^{(m)})$), do đó suy ra mệnh đề của ta.

Với mọi hệ (8), ta sẽ ký hiệu bởi $M_f$ hoặc $M_f(\mathbf{X})$, ma trận Jacobi $(\partial f_i / \partial X_j)$ ($1 \leq i \leq p, 1 \leq j \leq q$) trong đó $i$ là chỉ số của các hàng và $j$ là chỉ số của các cột; với hai hệ (8) và (9), trong đó $g$ không có số hạng hằng,
$$(11)$$
$$M_{f \circ g} = (M_f(g)). M_g$$
trong đó $M_f(g)$ là ma trận có các phần tử nhận được bằng cách thay $g$ cho $\mathbf{X}$, ($1 \leq j \leq q$) trong mỗi phần tử chuỗi của $M_f$; công thức này chỉ là một cách viết lại của công thức (9) của Đại số, Chương IV, § 5, no. 8. Ta sẽ ký hiệu bởi $M_f(0)$ ma trận của các số hạng hằng của các phần tử của $M_f$; khi đó ta suy ra từ (11) rằng
$$(12)$$
$$M_{f \circ g}(0) = M_f(0). M_g(0).$$

Cho một số nguyên $n > 0$, ta sẽ viết
$$(13)$$
$$\mathbf{1}_n = \mathbf{X} = (X_1, \ldots, X_n) \in (\mathbf{A}[[X_1, \ldots, X_n]])^n,$$
được xem như một ma trận có một cột duy nhất.

Đối với mọi hệ $\mathbf{f} = (f_1, \ldots, f_n) \in (\mathbf{A}[[X_1, \ldots, X_n]])^n$, $M_f$ là một ma trận vuông cấp $n$; ta sẽ ký hiệu $J_f$ hoặc $J_f(\mathbf{X})$ là định thức của nó và $J_f(0)$ là số hạng hằng của $J_f$, bằng với $\det(M_f(0))$; nếu $\mathbf{g} = (g_1, \ldots, g_n)$ là một hệ không có số hạng hằng trong $(\mathbf{A}[[X_1, \ldots, X_n]])^n$, thì, theo (11) và (12),
$$(14)$$
$$J_{f \circ g} = J_f(g) \cdot J_g$$
$$(15)$$
$$J_{f \circ g}(0) = J_f(g) J_g(0).$$

#### Mệnh đề 5 {#ac-iii-s4-prop-5 .statement}

*Cho $\mathbf{A}$ là một vành giao hoán và $\mathbf{f} = (f_1, \ldots, f_n)$ là một hệ không có số hạng hằng gồm $n$ chuỗi trong $\mathbf{A}[[X_1, \ldots, X_n]]$. Giả sử rằng $J_f(0)$ là khả nghịch trong $\mathbf{A}$. Khi đó tồn tại một hệ không có số hạng hằng $\mathbf{g} = (g_1, \ldots, g_n)$ gồm $n$ chuỗi trong $\mathbf{A}[[X_1, \ldots, X_n]]$ sao cho*
$$(16)$$
$$f \circ g = \mathbf{1}_n.$$

Hệ này là duy nhất và

(17) $g \circ f = 1_1$.

Sự tồn tại và tính duy nhất của $g$ suy ra từ Đại số, Chương IV, § 5, no. 9, Mệnh đề 10, áp dụng vào $n$ chuỗi lũy thừa hình thức

$$
f_i(Y_1, \ldots, Y_n) - X_i \quad (1 \leq i \leq n).
$$

Từ (15) và (16) suy ra rằng $J_f(0)J_g(0) = 1$ và do đó $J_g(0)$ cũng khả nghịch. Ta kết luận rằng tồn tại một hệ $h = (h_1, \ldots, h_n)$ gồm $n$ chuỗi không có số hạng hằng trong $A[[X_1, \ldots, X_n]]$ sao cho $g \circ h = 1_1$; từ quan hệ này và (16) suy ra, với sự trợ giúp của (10), rằng

$$
h = 1_n \circ h = (f \circ g) \circ h = f \circ (g \circ h) = f \circ 1_n = f.
$$

Mệnh đề 5 và các công thức (10) và (15) chỉ ra rằng với luật hợp thành $(f, g) \mapsto f \circ g$ tập hợp các hệ $f = (f_1, \ldots, f_n)$ gồm $n$ chuỗi không có số hạng hằng trong $A[[X_1, \ldots, X_n]]$ mà $J_f(0)$ khả nghịch trong $A$, là một nhóm.

### 5. CÁC HỆ PHƯƠNG TRÌNH TRONG CÁC VÀNH ĐẦY ĐỦ

Để viết gọn, từ nay về sau ta sẽ nói rằng một vành thỏa mãn *các điều kiện Hensel* nếu nó là giao hoán, có tôpô tuyến tính, Hausdorff và đầy đủ; cho một iđêan $m$ trong một vành như vậy, $m$ (hoặc cặp có thứ tự $(A, m)$) sẽ được nói là thỏa mãn *các điều kiện Hensel* nếu $m$ đóng trong $A$ và các phần tử của nó là lũy linh tôpô. Iđêan $t$ của $A$ gồm tất cả các phần tử lũy linh tôpô thỏa mãn các điều kiện Hensel (no. 3).

Đặc biệt, nếu $A$ là một vành giao hoán và $m$ là một iđêan của $A$ và $A$ là Hausdorff và đầy đủ đối với tôpô *m-adic*, thì cặp có thứ tự $(A, m)$ thỏa mãn các điều kiện Hensel.

#### Mệnh đề 6 {#ac-iii-s4-prop-6 .statement}

*Cho $A$ là một vành giao hoán, $B$ là một vành thỏa mãn các điều kiện của Hensel và $u : A \to B$ là một đồng cấu. Với mọi họ $x = (x_1, \ldots, x_n)$ gồm các phần tử lũy linh về mặt tôpô của $B$, tồn tại một đồng cấu duy nhất $\tilde{u}$ từ $A[[X_1, \ldots, X_n]]$ vào $B$ sao cho $\tilde{u}(a) = u(a)$ với mọi $a \in A$ và $\tilde{u}(X_i) = x_i$ với $1 \leq i \leq n$. Hơn nữa, nếu m ký hiệu iđêan các chuỗi không có số hạng hằng trong $A[[X_1, \ldots, X_n]]$, thì $\tilde{u}$ liên tục đối với tôpô m-adic.*

Cho $a$ là iđêan sinh hữu hạn được sinh trong $B$ bởi các $x_i$ ($1 \leq i \leq n$); với mọi iđêan mở $\mathfrak{H}$ của $B$, các ảnh của các $x_i$ trong $B/\mathfrak{H}$ là lũy linh, do đó iđêan $(a + \mathfrak{H})/\mathfrak{H}$ là lũy linh trong $B/\mathfrak{H}$ và tồn tại một số nguyên $k$ sao cho, với $\sum_{i=1}^n p_i \geq k$, ta có $x_1^{p_1} \cdots x_n^{p_n} \in \mathfrak{H}$. Vì mọi phần tử của $m^k$ là một tổng hữu hạn các chuỗi lũy thừa hình thức có dạng $X_1^{p_1} \cdots X_n^{p_n} g(X_1, \ldots, X_n)$, trong đó $\sum_{i=1}^n p_i \geq k$, nên thấy rằng, nếu $\tilde{u}$ giải quyết bài toán, thì $\tilde{u}(m^k) \subset \mathfrak{H}$, điều này chứng minh tính liên tục của $\tilde{u}$. Hiển nhiên tồn tại một đồng cấu duy nhất

$$
\nu : A[X_1, \ldots, X_n] \to B
$$

sao cho $\nu(a) = u(a)$ với $a \in A$ và $\nu(X_i) = x_i$ với $1 \leq i \leq n$ và lập luận trên cho thấy rằng $\nu$ liên tục đối với tôpô cảm sinh trên $A[X_1, \ldots, X_n]$ bởi tôpô m-adic. Vì $A[X_1, \ldots, X_r]$ trù mật trong $A[[X_1, \ldots, X_r]]$ đối với tôpô m-adic và B là Hausdorff và đầy đủ, điều đó hoàn tất chứng minh về sự tồn tại và tính duy nhất của $\tilde{u}$.

Chú ý rằng mệnh đề này lại cho ta như một trường hợp riêng (i) của Mệnh đề 11 ở § 2, no. 9.

Nếu bản thân $A$ được tôpô tuyến tính, thì hạn chế của $\tilde{u}$ lên $A\{X_1, \ldots, X_r\}$ trùng với đồng cấu dẫn xuất từ $u$ trong Mệnh đề 4 của no. 2. Điều này suy ra ngay lập tức từ việc $A[X_1, \ldots, X_r]$ trù mật trong $A\{X_1, \ldots, X_r\}$ nếu vành này được trang bị tôpô có hệ cơ bản các lân cận của 0 là các iđêan $m^k \cap N_3$ (theo ký hiệu của no. 2, tôpô này là cận trên bé nhất của tôpô cảm sinh trên $A\{X_1, \ldots, X_r\}$ bởi tôpô m-adic trên $A[[X_1, \ldots, X_n]]$ và tôpô được xác định ở no. 2).

Nếu $B = A$ và $u$ là ánh xạ đồng nhất, ta sẽ viết $f(x_1, \ldots, x_r)$ hoặc $f(x)$ cho phần tử $\tilde{u}(f)$ với mọi chuỗi lũy thừa hình thức $f \in A[[X_1, \ldots, X_r]]$; với mọi hệ $\mathbf{f} = (f_1, \ldots, f_r)$ các chuỗi lũy thừa hình thức của $A[[X_1, \ldots, X_r]]$, ký hiệu $\mathbf{f}(x)$ là phần tử $(f_1(x), \ldots, f_r(x))$ của $A^r$, khi đó ta nói nó thu được bằng cách thế các $x_i$ vào các $X_i$ trong $\mathbf{f}$. Nếu $n \leq m$ và F là một chuỗi lũy thừa hình thức của $A[[X_1, \ldots, X_m]]$, ta có thể xem F như một chuỗi lũy thừa hình thức theo các $X_{n+1}, \ldots, X_m$ với các hệ số trong $A[[X_1, \ldots, X_n]]$; ký hiệu

$$
F(x_1, \ldots, x_n, X_{n+1}, \ldots, X_m)
$$

là chuỗi lũy thừa hình thức trong $A[[X_{n+1}, \ldots, X_m]]$ thu được bằng cách thế các $x_i$ vào các $X_i$ trong các hệ số của F, với $1 \leq i \leq n$.

Ta lấy $B$ là vành các chuỗi lũy thừa hình thức $A[[X_1, \ldots, X_r]]$ và lấy $n$ là iđêan của các chuỗi trong $B$ không có số hạng hằng, sao cho $(B, n)$ thỏa mãn các điều kiện Hensel ($\S 2$, no. 6, Hệ quả của Mệnh đề 6). Mệnh đề 6 có thể được áp dụng bằng cách lấy các $x_i \in B$ là các chuỗi không có số hạng hằng; khi đó, với mọi chuỗi $\mathbf{f} \in A[[X_1, \ldots, X_r]]$, $\tilde{u}(f)$ chính là chuỗi lũy thừa hình thức $f(x_1, \ldots, x_n)$ được định nghĩa trong Đại số, Chương IV, $\S 5$, no. 5. Điều này là hiển nhiên nếu $f$ là một đa thức và trong trường hợp tổng quát nó suy ra từ mệnh đề bằng cách nhận xét rằng $f \mapsto f(x_1, \ldots, x_n)$ là liên tục trên $A[[X_1, \ldots, X_n]]$ đối với tôpô m-adic.

#### Hệ quả {#ac-iii-s4-n5-cor-1 .statement}

Cho $A$ là một vành thỏa mãn điều kiện Hensel và $x = (x_1, \ldots, x_n)$ là một họ các phần tử lũy linh tôpô của $A$. Cho $g = (g_1, \ldots, g_q)$ là một hệ không có số hạng hằng của các chuỗi trong $A[[X_1, \ldots, X_s]]$ và $f = (f_1, \ldots, f_p)$ là một hệ các chuỗi lũy thừa hình thức trong $A[[X_1, \ldots, X_q]]$. Khi đó $g(x) = (g_1(x), \ldots, g_q(x))$ là một họ các phần tử lũy linh tôpô của $A$ và

$$
(f \circ g)(x) = f(g(x)).
$$

Sự kiện các $g_i(x)$ là lũy linh tôpô suy ra ngay lập tức từ Mệnh đề 6 và sự kiện rằng trong $A$ iđêan của các phần tử lũy linh tôpô là đóng. Quan hệ (18) là hiển nhiên khi các $f_j$ là các đa thức; mặt khác, nếu $m$ và $m'$ là các iđêan của các chuỗi không có số hạng hằng trong

$$
A[[X_1, \ldots, X_q]] \quad \text{và} \quad A[[X_1, \ldots, X_n]]
$$

tương ứng, rõ ràng quan hệ $f \in m'^k$ kéo theo $f(g_1, \ldots, g_q) \in m'^k$. Do đó hai vế của (18) là các hàm liên tục của $f$ vào $(A[[X_1, \ldots, X_q]])^p$ nếu $A[[X_1, \ldots, X_q]]$ được trang bị tôpô $m$-adic, theo nhận xét trên và Mệnh đề 6; do đó quan hệ (18).

Trong phần sau, với một vành $A$ và một iđêan $m$ của $A$ chúng tôi sẽ ký hiệu bởi $m^{x^n}$ tập hợp tích $\prod_{i=1}^n m$, trong $A^n$, ở đó $m_i = m$ với $1 \leq i \leq n$, để tránh nhập nhằng.

#### Mệnh đề 7 {#ac-iii-s4-prop-7 .statement}

*Cho $A$ là một vành và $m$ là một iđêan của $A$ sao cho cặp có thứ tự $(A, m)$ thỏa mãn các điều kiện Hensel. Cho $f = (f_1, \ldots, f_n)$ là một hệ không có số hạng hằng gồm các chuỗi trong $A[[X_1, \ldots, X_n]]$ sao cho $J_f(0)$ khả nghịch trong $A$. Khi đó, với mọi $x \in m^{x^n}$, $f(x) \in m^{x^n}$ và $x \mapsto f(x)$ là một song ánh của $m^{x^n}$ lên chính nó, song ánh ngược là $x \mapsto g(x)$, trong đó $g$ được cho bởi quan hệ (16) ở no. 4.*

Sự kiện rằng $f(x) \in m^{x^n}$ là hiển nhiên khi các chuỗi ấy là các đa thức và trong trường hợp tổng quát suy ra từ Mệnh đề 6 và từ sự kiện rằng $m$ là đóng trong $A$. Khi đó các khẳng định khác của mệnh đề là những hệ quả ngay lập tức của (16), (17) và (18).

#### Hệ quả {#ac-iii-s4-n5-cor-2 .statement}

*Cho $q$ là một iđêan đóng của $A$ được chứa trong $m$. Khi đó quan hệ $x \equiv x' \pmod{q^{x^n}}$ là tương đương với $f(x) \equiv f(x') \pmod{q^{x^n}}$.*

Với mọi chuỗi lũy thừa hình thức $f \in A[[X_1, \ldots, X_n]]$,

$$
f(X_1, \ldots, X_n) - f(Y_1, \ldots, Y_n) = \sum_{i=1}^n (X_i - Y_i) h_i(X_1, \ldots, X_n, Y_1, \ldots, Y_n)
$$

trong đó các $h_i$ thuộc $A[[X_1, \ldots, X_n, Y_1, \ldots, Y_n]]$ (Đại số, Chương IV, § 5, no. 8, Mệnh đề 9); ngay lập tức suy ra rằng quan hệ $x \equiv x' \pmod{q^{x^n}}$ kéo theo $f(x) \equiv f(x') \pmod{q^{x^n}}$. Đảo lại thu được bằng cách thay thế $f$ bởi "nghịch đảo" $g$ của nó.

#### Định lý 2 {#ac-iii-s4-thm-2 .statement}

*Cho $A$ là một vành và $m$ là một iđêan của $A$ sao cho cặp có thứ tự $(A, m)$ thỏa mãn các điều kiện Hensel. Cho $f = (f_1, \ldots, f_n)$ là một hệ gồm $n$ phần tử của

A\{X_1, \ldots, X_n\} và cho $a \in A^n$; viết $J_t(a) = e$. Tồn tại một hệ $g = (g_1, \ldots, g_n)$ các chuỗi lũy thừa hình thức hạn chế không có hằng số trong $A\{X_1, \ldots, X_n\}$ sao cho
(i) $M_g(0) = I$, (ma trận đơn vị).
(ii) Với mọi $x \in A^n$,
$$(19)$$
$$f(a + ex) = f(a) + M_t(a) \cdot eg(x).$$
(iii) Cho $h = (h_1, \ldots, h_n)$ là hệ các chuỗi lũy thừa hình thức không có hằng số (không nhất thiết hạn chế) sao cho $g \circ h = 1_n$ (Mệnh đề 5). Với mọi $y \in m^{n \times n}$,
$$(20)$$
$$f(a + eh(y)) = f(a) + M_t(a) \cdot ey.$$
Với mọi chuỗi lũy thừa hình thức $f \in A[[X_1, \ldots, X_n]]$,
$$(21)$$
$$f(X + Y) = f(X) + M_f(X) \cdot Y + \sum_{1 \leq i < j \leq n} G_{ij}(X, Y)Y_i Y_j,$$
trong đó các $G_{ij}$ là các chuỗi lũy thừa hình thức được xác định duy nhất trong
$$A[[X_1, \ldots, X_n, Y_1, \ldots, Y_n]].$$
Nếu f là hạn chế, thì các phần tử của $M_f$ và các $G_{ij}$ cũng vậy, vì các chuỗi lũy thừa hình thức này là các đa thức nếu f là một đa thức và suy ra từ tính duy nhất của chúng rằng với mọi iđêan mở $\mathfrak{J}$ của $A$, ký hiệu $p_\mathfrak{J}: A \to A/\mathfrak{J}$ là ánh xạ chính tắc, ảnh của $G_{ij}$ dưới $p_\mathfrak{J}$ là hệ số của $Y_i Y_j$ trong $p_\mathfrak{J}(F)$ với $F$ là chuỗi lũy thừa hình thức $f(X + Y)$ trong $A[[X_1, \ldots, X_n, Y_1, \ldots, Y_n]]$; do đó mệnh đề của chúng ta.

Do đó, viết công thức (21) cho mỗi chuỗi fi $(1 \leq i \leq n)$, ta thu được với mọi $x \in A^n$ (no. 2, Mệnh đề 4),
$$(22)$$
$$f(a + ex) = f(a) + M_t(a) \cdot ex + e^2 r(x)$$
trong đó $r = (r_1, \ldots, r_r)$ là một hệ các chuỗi lũy thừa hình thức hạn chế, mỗi chuỗi đều có cấp toàn phần $\geq 2$. Suy ra từ các công thức (18) của Đại số, Chương III, § 6, no. 5 rằng tồn tại một ma trận vuông $M' \in \mathbf{M}_n(A)$ sao cho
$$(23)$$
$$M_t(a) \cdot M' = eI_n,$$
do đó dùng điều này trong (22)
$$(24)$$
$$f(a + ex) = f(a) + M_t(a) \cdot ex + M_t(a) M' \cdot er(x).$$

Viết $g = 1, + M' \cdot r$, ta thấy rằng $g$ thỏa mãn các điều kiện (i) và (ii); khi đó chỉ cần thay thế $x$ bởi $h(y)$ để thu được (iii).

#### Hệ quả 1 {#ac-iii-s4-thm-2-cor-1 .statement}

Cho $A$ là một vành và $m$ là một iđêan của $A$ sao cho cặp có thứ tự $(A, m)$ thỏa mãn các điều kiện của Hensel. Cho $f \in A\{X\}$, $a \in A$ và đặt $e = f'(a)$. Nếu $f(a) \equiv 0$ (mod. $e^2 m$), thì tồn tại $b \in A$ sao cho $f(b) = 0$ và $b \equiv a$ (mod. $em$). Nếu b' là một phần tử khác của $\mathbf{A}$ sao cho $f(b') = 0$ và $b' \equiv a \pmod{\mathfrak{m}}$, thì $e(b - b') = 0$. Đặc biệt, $b$ là duy nhất nếu $e$ không phải là một ước của không trong $\mathbf{A}$.

Đặt $f(a) = e^2 c$ với $c \in \mathfrak{m}$; công thức (20) với $n = 1$ cho
$$
f(a + eh(y)) = e^2(c + y)
$$
và do đó chỉ cần lấy $y = -c$, $b = a + eh(-c)$. Hơn nữa nếu $b = a + ex, b' = a + ex', x \in \mathfrak{m}, x' \in m, f(b) = f(b') = 0$, ta suy ra từ (19) rằng $e^2(g(x) - g(x')) = 0$. Vì $g(\mathbf{X}) - g(\mathbf{Y}) = (\mathbf{X} - \mathbf{Y})u(\mathbf{X}, \mathbf{Y})$, trong đó $u$ là hạn chế và $u(0, 0) = 1$, nên $g(x) - g(x') = (x - x')v$, trong đó $v \in \mathbf{A}$ là khả nghịch, vì, do $m$ là đóng, ta có $v - 1 = u(x, x') - 1 \in \mathfrak{m}$ và $m$ được chứa trong căn Jacobson của $\mathbf{A}$; do đó có quan hệ $e(b - b') = 0$.

#### Nhận xét {#ac-iii-s4-n5-rem-1 .statement}

Hệ quả này áp dụng đáng chú ý khi $e$ khả nghịch trong $\mathbf{A}$; khi đó ta cũng có thể suy ra sự tồn tại của $b$ từ Định lý Hensel, vì ảnh chính tắc của $f(\mathbf{X})$ trong $(\mathbf{A}/\mathfrak{m})\{\mathbf{X}\}$ có dạng $(\mathbf{X} - a)f_1(\mathbf{X}), \mathbf{X} - a$ và $f_1(\mathbf{X})$ nguyên tố cùng nhau mạnh, vì $f_1(\alpha) = f'(\alpha)$ là ảnh của $e$ (no. 1, Ví dụ).

Ví dụ
(1) Cho $p$ là một số nguyên tố $\neq 2$ và $n$ là một số nguyên sao cho lớp của nó mod. $p$ là một bình phương $\neq 0$ trong trường nguyên tố $\mathbf{F}_p$. Nếu $\mathbf{Z}_p$ là vành các số nguyên $p$-adic (\S 2, no. 12, Ví dụ 3), việc áp dụng Hệ quả 1 cho đa thức $\mathbf{X}^2 - n$ cho thấy rằng $n$ là một bình phương trong $\mathbf{Z}_p$; chẳng hạn 7 là một bình phương trong $\mathbf{Z}_3$.
(2) Cho $\mathbf{A} = \mathbf{K}[[\mathbf{Y}]]$ là vành các chuỗi lũy thừa hình thức theo một ẩn với hệ số trong một trường giao hoán $\mathbf{K}$; với tôpô $(\mathbf{Y})$-adic, vành $\mathbf{A}$ là Hausdorff và đầy đủ (\S 2, no. 6, Hệ quả của Mệnh đề 6) và ánh xạ $f(\mathbf{Y}) \mapsto f(0)$ xác định, bằng cách chuyển qua vành thương, một đẳng cấu từ $\mathbf{A}/(\mathbf{Y})$ lên trường $\mathbf{K}$. Theo Hệ quả 1, nếu $F(\mathbf{Y}, \mathbf{X})$ là một đa thức theo $\mathbf{X}$ với hệ số trong $\mathbf{A}$ và $a$ là một nghiệm đơn của $F(0, \mathbf{X})$ trong $\mathbf{K}$, thì tồn tại duy nhất một chuỗi lũy thừa hình thức $f(\mathbf{Y})$ sao cho $f(0) = a$ và $F(\mathbf{Y}, f(\mathbf{Y})) = 0$.

#### Hệ quả 2 {#ac-iii-s4-thm-2-cor-2 .statement}

Cho $\mathbf{A}$ là một vành và $\mathfrak{m}$ là một iđêan của $\mathbf{A}$ sao cho cặp có thứ tự $(\mathbf{A}, m)$ thỏa mãn các điều kiện của Hensel. Cho $r, n$ là các số nguyên sao cho $0 \leq r < n$ và $\mathbf{f} = (f_{r+1}, \ldots, f_n)$ là một hệ gồm $n - r$ phần tử của $\mathbf{A}\{\mathbf{X}_1, \ldots, \mathbf{X}_n\}$; gọi $J^{(n-r)}_{\mathbf{f}}(\mathbf{X})$ là định thức con của $M_{\mathbf{f}}(\mathbf{X})$ gồm các cột có chỉ số $j$ sao cho $r + 1 \leq j \leq n$. Cho $a \in \mathbf{A}^n$ sao cho $J^{(n-r)}_{\mathbf{f}}(a)$ khả nghịch trong $\mathbf{A}$ và $\mathbf{f}(a) \equiv 0 \pmod{\mathfrak{m}^{(n-r)}}$. Khi đó tồn tại duy nhất $\mathbf{x} = (x_1, \ldots, x_n) \in \mathbf{A}^n$ sao cho $x_k = a_k$ với $1 \leq k \leq r$, $\mathbf{x} \equiv a \pmod{\mathfrak{m}^n}$ và $\mathbf{f}(\mathbf{x}) = 0$.

Thay $a$, cho $X_k$ với $1 \leq k \leq r$ trong các $f_i$ (no. 2, Nhận xét 3 ), ta thấy ngay lập tức rằng để chứng minh hệ quả này, ta có thể chỉ cần xét trường hợp $r = 0$. Khi đó Định lý 1 và Mệnh đề 7 cho thấy $\mathbf{f}$ xác định một song ánh từ $a + \mathfrak{m}^n$ lên $\mathbf{f}(a) + \mathfrak{m}^n = \mathfrak{m}^n$; hệ quả suy ra từ việc $0 \in \mathfrak{m}^n$.

#### Hệ quả 3 {#ac-iii-s4-thm-2-cor-3 .statement}

*Với ký hiệu và Hệ quả 2, cho $a \in \mathbf{A}^n$; đặt $e = J_r^{(n-r)}(\mathbf{a})$ (không nhất thiết khả nghịch trong $\mathbf{A}$) và giả sử rằng $f(\mathbf{a}) \equiv 0$ (mod. $e^{2m^{\times(n-r)}}$). Khi đó tồn tại $n - r$ chuỗi lũy thừa hình thức không có hằng số $\phi_i$ ($r + 1 \leq i \leq n$) trong $\mathbf{A}[[X_1, \ldots, X_r]]$ sao cho, với mọi $t = (t_1, \ldots, t_r) \in m^{\times r}$,*

$$
f_i(a_1 + e^2 t_1, \ldots, a_r + e^2 t_r, a_{r+1} + e \phi_{r+1}(t), \ldots, a_n + e \phi_n(t)) = 0
$$

*đối với $r + 1 \leq i \leq n$.*

*Với $1 \leq i \leq r$, đặt $f_i(X) = X_i - a$, và đặt $u = (f_1, \ldots, f_n)$; khi đó $J_u(a) = e$ và Định lý 2 có thể được áp dụng cho hệ $u$. Với ký hiệu của Định lý 2, từ các định nghĩa trên suy ra rằng $g_i(X) = X$, với $1 \leq i \leq r$, do đó $h_i(X) = X_i$ với $1 \leq i \leq r$; hơn nữa, nếu $M' \in \mathbf{M}_n(\mathbf{A})$ sao cho $M_u(a) . M' = e I_n$, thì $M'$ có dạng*

$$
\begin{pmatrix}
e I_r & 0 \\
* & *
\end{pmatrix}.
$$

*Thay thế $y$ bởi $M'.z$ (trong đó $z = (z_1, \ldots, z_n) \in m^{\times n}$) trong công thức (20), ta được*

$$
f_i(a_1 + e^2 z_1, \ldots, a_r + e^2 z_r, a_{r+1} + e h_{r+1}(M'.z), \ldots, a_n + e h_n(M'.z))
= \& (a) + e^2 z_i \quad \text{với } 1 \leq i \leq n.
$$

*Theo giả thiết, $f_j(a) = e^2 b_j$, trong đó $b_j \in m$ với $r + 1 \leq j \leq n$. Đặt $\psi_j(X_1, \ldots, X_r) = h_j(M'.X)$ và*

$$
\phi_j(X_1, \ldots, X_r) = \psi_j(X_1, \ldots, X_r, -b_{r+1}, \ldots, -b_n)
$$

*với $r + 1 \leq j \leq n$. Với $r + 1 \leq i \leq n$, thay $t_j$ cho $z_j$ với $1 \leq j \leq r$ và $b_j$ cho $z_j$ với $r + 1 \leq j \leq n$ trong (26), ta thu được các hệ thức (25) với mọi $t \in m^{\times r}$.*

### 6. ÁP DỤNG VÀO SỰ PHÂN RÃ CỦA CÁC VÀNH

#### Bổ đề 2 {#ac-iii-s4-lem-2 .statement}

*Cho $\mathbf{A}$ là một vành và $m$ là một iđêan của $\mathbf{A}$ sao cho cặp có thứ tự $(\mathbf{A}, m)$ thỏa mãn các điều kiện của Hensel. Cho $\mathbf{B}$ là vành thương $\mathbf{A}/m$ và $\pi : \mathbf{A} \to \mathbf{B}$ là đồng cấu chính tắc. Với mọi lũy đẳng $c$ của $\mathbf{B}$, tồn tại một lũy đẳng duy nhất $e$ của $\mathbf{A}$ sao cho $\pi(e) = c$.*

Cho $a$ sao cho $\pi(a) = c$; Hệ quả 1 của Định lý 2 ở no. 5 có thể được áp dụng cho đa thức $f(X) = X^2 - X$ trong $\mathbf{A}[X]$ và phần tử $a \in \mathbf{A}$. Khi đó $f'(a) = 2a - 1$ và, vì $\pi(2a - 1) = 2c - 1$ và $(2c - 1)^2 = 1$ trong $\mathbf{B}$, nên $2c - 1$ khả nghịch trong $\mathbf{B}$ và do đó $2a - 1$ khả nghịch trong $\mathbf{A}$ (\S 2, no. 13, Bổ đề 3). Vì $f(a) \in m$, Hệ quả 1 của Định lý 2 ở no. 5 ngay lập tức cho sự tồn tại và tính duy nhất của $e$.

#### Mệnh đề 8 {#ac-iii-s4-prop-8 .statement}

*Cho $\mathbf{A}$ là một vành và $m$ là một iđêan của $\mathbf{A}$ sao cho cặp có thứ tự $(\mathbf{A}, m)$ thỏa mãn các điều kiện của Hensel. Cho $\mathbf{B}$ là vành thương $\mathbf{A}/m$ và $\pi : \mathbf{A} \to \mathbf{B}$ là đồng cấu chính tắc. *Nếu B là hợp thành trực tiếp của một họ hữu hạn* $(\mathfrak{b}_i)_{i \in I}$ *các iđêan, thì tồn tại một họ duy nhất* $(\mathfrak{a}_i)_{i \in I}$ *các iđêan của A sao cho* $\pi(\mathfrak{a}_i) = \mathfrak{b}_i$ *với mọi* $i \in I$ *và A là hợp thành trực tiếp của họ* $(\mathfrak{a}_i)$.

Cho $I = \sum_i c_i$ với $c_i \in \mathfrak{b}_i$ với mọi $i$; các $c_i$ là các phần tử lũy đẳng của $B$ sao cho $c_i c_j = 0$ với $i \neq j$. Theo Bổ đề 2, do đó tồn tại các phần tử lũy đẳng $e_i$ của $A$ ($i \in I$) sao cho $\pi(e_i) = c_i$ với mọi $i$; vì $e_i e_j$ là một phần tử lũy đẳng sao cho
$$
\pi(e_i e_j) = c_i c_j = 0
$$
với $i \neq j$, nên $e_i e_j = 0$ với $i \neq j$ (Bổ đề 2); vì $1 - \sum_i e_i$ là một phần tử lũy đẳng sao cho
$$
\pi\left(1 - \sum_i e_i\right) = 1 - \sum_i c_i = 0,
$$
tương tự suy ra $1 = \sum_i e_i$. Suy ra $A$ là hợp thành trực tiếp của các iđêan $\mathfrak{a}_i = e_i A$ và $\pi(\mathfrak{a}_i) = \pi(e_i) B = \mathfrak{b}_i$.

Còn phải chỉ ra tính duy nhất của một phân tích như vậy. Bây giờ, giả sử rằng $A$ là hợp thành trực tiếp của một họ khác $(\mathfrak{a}'_i)_{i \in I}$ các iđêan sao cho $\pi(\mathfrak{a}'_i) = \mathfrak{b}_i$ với mọi $i$; khi đó $1 = \sum_i e'_i$ trong đó $e'_i \in \mathfrak{a}'_i$, do đó, trong $B$, $1 = \sum_i \pi(e'_i)$ trong đó $\pi(e'_i) \in \mathfrak{b}_i$, điều này kéo theo $\pi(e'_i) = c_i$; vì $e'_i$ và $e_i$ là các phần tử lũy đẳng, tất yếu $e'_i = e_i$ (Bổ đề 2), điều này hoàn tất chứng minh.

#### Nhận xét {#ac-iii-s4-n6-rem-1 .statement}

Mệnh đề 8 lại cho cấu trúc của một vành nửa địa phương trên $A$ mà đối với tôpô $c$-adic thì Hausdorff và đầy đủ ($c$ là căn Jacobson của $A$), điều này đã thu được như một hệ quả của § 2, no. 13, Hệ quả của Mệnh đề 19.

### Bài tập {#ac-iii-s4-exercises}

Xem [các bài tập của § 4](exercises/s4/).
