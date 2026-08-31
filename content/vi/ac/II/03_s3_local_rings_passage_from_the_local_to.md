---
book: ac
book_title: Commutative Algebra
chapter: II
chapter_title: LOCALIZATION
section: 3
section_title: Local rings. Passage from the local to the global
lang: vi
source: ac-i-vii
book_pages: 80-94, 136-139
pdf_pages: 0100-0114, 0156-0159
extraction: ocr
subsections:
    - "no": 1
      title: LOCAL RINGS
      page: 80
      pdf_page: 100
    - "no": 2
      title: MODULES OVER A LOCAL RING
      page: 82
      pdf_page: 102
    - "no": 3
      title: PASSAGE FROM THE LOCAL TO THE GLOBAL
      page: 87
      pdf_page: 107
    - "no": 4
      title: LOCALIZATION OF FLATNESS
      page: 91
      pdf_page: 111
    - "no": 5
      title: SEMI-LOCAL RINGS
      page: 92
      pdf_page: 112
statements: 39
exercises: 14
content_sha256: ce517c4dfef8f95b775dc527bed6b10509b6d7292df62a77c0a132881ae99600
translated_from: content/en/ac/II/03_s3_local_rings_passage_from_the_local_to.md
source_content_sha256: 4f386f4871c58170a49537a2a50d87c0f1514cb0377ef14915c0c8c2f53a7186
translation_model: gpt-5.4-mini, gpt-5.4, gpt-5-6-mini
translation_run: translate-vi-690e73ff
glossary_version: 34
glossary_terms_sha256: 2865d449e7799cf3fb9fdad7d92b7881d3de169ed095ef298124744f3be58e88
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 3. VÀNH ĐỊA PHƯƠNG. CHUYỂN TỪ ĐỊA PHƯƠNG SANG TOÀN CỤC

### 1. VÀNH ĐỊA PHƯƠNG

#### Mệnh đề 1 {#ac-ii-s3-prop-1 .statement}

Cho $\mathbf{A}$ là một vành và $I$ là tập các phần tử không khả nghịch của $\mathbf{A}$. Tập $I$ là hợp của các iđêan của $\mathbf{A}$ khác $\mathbf{A}$. Hơn nữa, các điều kiện sau là tương đương:
(a) $I$ là một iđêan.
(b) Tập các iđêan của $\mathbf{A}$ khác $\mathbf{A}$ có một phần tử lớn nhất.
(c) $\mathbf{A}$ có một iđêan cực đại duy nhất.

Quan hệ $x \in I$ tương đương với $1 \notin xA$ và do đó $xA \neq \mathbf{A}$. Nếu $a$ là một iđêan của $\mathbf{A}$ khác $\mathbf{A}$ và $x \in a$, thì $xA \subset a$, do đó $xA \neq \mathbf{A}$ và $x \in I$. Vậy nên mọi iđêan của $\mathbf{A}$ khác $\mathbf{A}$ đều được chứa trong $I$ và mọi phần tử $x \in I$ đều thuộc một iđêan chính $xA \neq \mathbf{A}$. Điều này chứng minh mệnh đề đầu tiên, và ngay lập tức suy ra tính tương đương của (a), (b) và (c).

Nhận xét (1). Chú ý rằng, nếu (c) đúng, thì $I$ là căn Jacobson của vành $\mathbf{A}$ (Đại số, Chương VIII, §6, no. 3, Định nghĩa 3).

#### Định nghĩa 1 {#ac-ii-s3-def-1 .statement}

Một vành $\mathbf{A}$ được gọi là vành địa phương nếu nó thỏa mãn các điều kiện tương đương (a), (b) và (c) của Mệnh đề 1. Thương của $\mathbf{A}$ theo căn Jacobson của nó (khi đó là iđêan cực đại duy nhất của $\mathbf{A}$) được gọi là trường thặng dư của $\mathbf{A}$.

#### Định nghĩa 2 {#ac-ii-s3-def-2 .statement}

Cho $\mathbf{A}, \mathbf{B}$ là hai vành địa phương và $m, n$ là các iđêan cực đại tương ứng của chúng. Một đồng cấu $u : \mathbf{A} \to \mathbf{B}$ được gọi là địa phương nếu $u(m) \subset n$.

Điều đó tương đương với việc nói rằng $\bar{u}^{-1}(n) = m$, vì khi đó $\bar{u}^{-1}(n)$ là một iđêan chứa $m$ và không chứa 1, nên bằng $m$. Lấy các thương, ta suy ra một cách chính tắc từ $u$ một đơn cấu $\mathbf{A}/m \to \mathbf{B}/n$ từ trường thặng dư của $\mathbf{A}$ sang trường thặng dư của $\mathbf{B}$.

Ví dụ
(1) Một trường là một vành địa phương. Một vành được thu về $0$ không phải là một vành địa phương.
(2) Cho $\mathbf{A}$ là một vành địa phương và $k$ là trường thặng dư của nó. Vành chuỗi hình thức $B = \mathbf{A}[[X_1, \ldots, X_n]]$ là một vành địa phương, vì các phần tử không khả nghịch của $B$ là các chuỗi lũy thừa hình thức mà hạng hằng của chúng không khả nghịch trong $\mathbf{A}$ (Đại số, Chương IV, §5, no. 6, Mệnh đề 4). Đơn ánh chính tắc của $\mathbf{A}$ vào $B$ là một đồng cấu địa phương và đơn ánh tương ứng của các trường thặng dư là một đẳng cấu.
(3) Cho $b$ là một iđêan của một vành $\mathbf{A}$ chỉ được chứa trong đúng một iđêan cực đại $m$; khi đó $A/b$ là một *vành địa phương* có iđêan cực đại $m/b$ và trường thặng dư đẳng cấu chính tắc với $A/m$. Điều này áp dụng riêng cho trường hợp $b = m^k$, với $m$ là một iđêan cực đại bất kỳ của $A$ ($§ 1$, no. 1, Hệ quả của Mệnh đề 1). Nếu bản thân $A$ là một vành địa phương có iđêan cực đại $m$, thì với mọi iđêan $b \neq A$ của $A$, $A/b$ là một vành địa phương, đồng cấu chính tắc $A \to A/b$ là một đồng cấu địa phương và đồng cấu tương ứng của các trường thặng dư là một *đẳng cấu*.

(4) Cho $X$ là một không gian tôpô, $x_0$ là một điểm của $X$ và $A$ là vành các mầm tại điểm $x_0$ của các hàm thực liên tục trong một lân cận của $x_0$ (*Tôpô đại cương*, Chương I, § 6, no. 10). Rõ ràng, để mầm tại $x_0$ của một hàm liên tục $f$ khả nghịch trong $A$, điều kiện cần và đủ là $f(x_0) \neq 0$, vì điều đó kéo theo $f(x) \neq 0$ trong một lân cận của $x_0$. Do đó vành $A$ là một vành địa phương mà iđêan cực đại $m$ của nó là tập hợp các mầm của những hàm bằng không *tại* $x_0$; lấy thương, ánh xạ $g \mapsto g(x_0)$ từ $A$ vào $\mathbf{R}$ cho một *đẳng cấu* từ trường thặng dư $A/m$ lên $\mathbf{R}$.

#### Mệnh đề 2 {#ac-ii-s3-prop-2 .statement}

*Cho $A$ là một vành và $p$ là một iđêan nguyên tố của $A$. Vành $A_p$ là địa phương; iđêan cực đại của nó là iđêan $pA_p = p_v$, sinh bởi ảnh chính tắc của $p$ trong $A_p$; trường thặng dư của nó đẳng cấu chính tắc với trường phân thức của $A/p$.*

Cho $S = A - p$ và $j : A \to A_v$, là đồng cấu chính tắc; giả thiết rằng $p$ là nguyên tố suy ra rằng $p$ là bão hòa đối với $S$, do đó $j^{-1}(pA_p) = p$ ($§ 2$, no. 4, Proposition 10) và, vì các iđêan của $A$ không gặp $S$ là các iđêan được chứa trong $p$, hai khẳng định đầu tiên là những trường hợp riêng của $§ 2$, no. 5, Proposition 11 (ii). Hơn nữa, nếu $f$ là đồng cấu chính tắc $A \to A/p$, thì $f(S)$ là tập hợp các phần tử $\neq 0$ của miền nguyên $A/p$ và do đó khẳng định cuối cùng là một trường hợp riêng của $§ 2$, no. 5, Proposition 11 (i).

#### Định nghĩa 3 {#ac-ii-s3-def-3 .statement}

*Cho $A$ là một vành và $p$ là một iđêan nguyên tố của $A$. Vành $A$, được gọi là vành địa phương của $A$ tại $p$, hoặc là vành địa phương của $p$, khi không có sự nhập nhằng.*

*Nhận xét (2).* Nếu $A$ là một vành địa phương và $m$ là iđêan cực đại của nó, thì các phần tử của $A - m$ là khả nghịch (Proposition 1) và do đó $A_{m'}$ được đồng nhất một cách chính tắc với $A$ ($§ 2$, no. 1, Remark 5).

Ví dụ
(5) Cho $p$ là một số nguyên tố. Vành địa phương $\mathbf{Z}_{(p)}$ là tập hợp các số hữu tỉ $a/b$, trong đó $a, b$ là các số nguyên với $b$ nguyên tố cùng $p$; trường thặng dư của $\mathbf{Z}_{(p)}$ đẳng cấu với trường nguyên tố $\mathbf{F}_p = \mathbf{Z}/(p)$.

(6) Cho $V$ là một đa tạp đại số afin, $A$ là vành các hàm chính quy trên $V$, $W$ là một đa tạp con bất khả quy của $V$ và $p$ là iđêan (tất yếu là nguyên tố) của $A$ gồm các hàm triệt tiêu tại mọi điểm của $W$. Vành $A$, được gọi là vành địa phương của $W$ trên $V$. \*

#### Mệnh đề 3 {#ac-ii-s3-prop-3 .statement}

Cho $A$ là một vành, $p$ là một iđêan nguyên tố của $A$ và $S = A - p$. Với mọi iđêan $b'$ của $A_p$ phân biệt với $A_p$, đặt $b$ là iđêan $(i_A^S)^{-1}(b')$ của $A$ sao cho $b' = bA_p$.

(i) Cho $f$ là đồng cấu chính tắc $A \to A/b$. Đồng cấu từ $A$ đến $(A/b)_{p/b}$ liên kết với $f$ một cách chính tắc ($§ 2$, no. 1, Mệnh đề 2) là toàn ánh và hạt nhân của nó là $b'$, hạt nhân này xác định, bằng cách lấy thương, một đẳng cấu chính tắc từ $A_p/b'$ lên $(A/b)_{p/b}$.

(ii) Ánh xạ $b' \to b = (i_A^S)^{-1}(b')$, hạn chế vào tập hợp các iđêan nguyên tố của $A_p$, là một đẳng cấu (đối với quan hệ bao hàm) từ tập hợp này lên tập hợp các iđêan nguyên tố của $A$ được chứa trong $p$. Nếu $b'$ là nguyên tố trong $A_p$, tồn tại một đẳng cấu của vành $A_b$ lên vành $(A_p)_{b'}$, ánh xạ $a/s$ tới $(a/1)/(s/1)$ với mọi $a \in A, s \in A - b$.

Đây chỉ là một trường hợp riêng của $§ 2$, no. 5, Mệnh đề 11.

Nhận xét
(3) Nếu $a$ là một iđêan của $A$ không được chứa trong $p$, thì $aA_p = A$, và $(A/a)_p = 0$ ($§ 2$, no. 5, Nhận xét).
(4) Cho $A, B$ là hai vành, $\rho : A \to B$ một đồng cấu, $q$ một iđêan nguyên tố của $B$ và $p$ là iđêan nguyên tố $\rho^{-1}(q)$ của $A$. Vì $\rho(A - p) \subset B - q$, một đồng cấu chính tắc $\rho_q : A \to B_q$ được dẫn xuất từ $\rho$ ($§ 2$, no. 1, Mệnh đề 2) và ngay lập tức thấy rằng $\rho_q(pA_p) \subset qB_q$, do đó $\rho$ là một đồng cấu địa phương.

### 2. MÔĐUN TRÊN MỘT VÀNH ĐỊA PHƯƠNG

#### Mệnh đề 4 {#ac-ii-s3-prop-4 .statement}

Cho $A$ là một vành không nhất thiết giao hoán, $m$ một iđêan phải của $A$ được chứa trong căn Jacobson của $A$ và $M$ một A-môđun trái. Giả sử rằng một trong các điều kiện sau được thỏa mãn :
(i) $M$ sinh hữu hạn;
(ii) $m$ lũy linh.
Khi đó quan hệ $(A_d/m) \otimes_A M = 0$ kéo theo $M = 0$.

Mệnh đề đối với giả thiết (i) chính xác là Hệ quả 3 của Mệnh đề 6 trong Đại số, Chương VIII, $§ 6$, no. 3. Mặt khác, quan hệ $(A_d/m) \otimes_A M = 0$ tương đương với $M = mM$ và do đó kéo theo $M = m^nM$ với mọi số nguyên $n > 0$; do đó có mệnh đề đối với giả thiết (ii).

#### Hệ quả 1 {#ac-ii-s3-prop-4-cor-1 .statement}

Cho $A$ là một vành không nhất thiết giao hoán, $m$ là một iđêan phải của $A$ được chứa trong căn Jacobson của $A$, $M$ và $N$ là hai $A$-môđun trái và $u : M \to N$ là một ánh xạ $A$-tuyến tính. Nếu $N$ sinh hữu hạn hoặc $m$ là lũy linh và
$$
1 \otimes u : (A_d/m) \otimes_A M \to (A_d/m) \otimes_A N
$$
là toàn ánh, thì $u$ là toàn ánh.

$(A_d/m) \otimes_A (N/u(M))$ đẳng cấu chính tắc với
$$
((A_d/m) \otimes_A N)/\operatorname{Im}(1 \otimes u)
$$

#### Hệ quả 2 {#ac-ii-s3-prop-4-cor-2 .statement}

*Cho $A$ là một vành không nhất thiết giao hoán, $m$ là một iđêan hai phía của $A$ được chứa trong căn Jacobson của $A$, $M$ là một $A$-môđun trái và $(x_i)_{i \in I}$ là một họ các phần tử của $M$. Nếu $M$ sinh hữu hạn hoặc $m$ là lũy linh và các phần tử $1 \otimes x_i$ ($i \in I$) sinh môđun trái $(A/m)$ $(A/m) \otimes_A M$, thì các $x_i$ sinh $M$.*

Cho $(e_i)_{i \in I}$ là cơ sở chính tắc của $A$-môđun trái $A_s^{(I)}$: chỉ cần áp dụng Hệ quả 1 cho ánh xạ $A$-tuyến tính $u : A_s^{(I)} \to M$ sao cho $u(e_i) = x_i$ với mọi $i \in I$.

#### Mệnh đề 5 {#ac-ii-s3-prop-5 .statement}

*Cho $A$ là một vành không nhất thiết giao hoán, $m$ là một iđêan hai phía của $A$ được chứa trong căn Jacobson của $A$ và $M$ là một $A$-môđun trái. Giả sử một trong các điều kiện sau được thỏa mãn:
(i) $M$ được trình bày hữu hạn;
(ii) $m$ là lũy linh.
Khi đó, nếu $(A/m) \otimes_A M = M/mM$ là một môđun trái tự do trên $(A/m)$ và đồng cấu chính tắc từ $m \otimes_A M$ đến $M$ là đơn ánh, thì $M$ là một $A$-môđun tự do. Chính xác hơn, nếu $(x_i)_{i \in I}$ là một họ các phần tử của $M$ sao cho $(1 \otimes x_i)$ là một cơ sở của $(A/m)$-môđun $M/mM$, thì $(x_i)$ là một cơ sở của $M$.*

Nếu $a \in A$, $x \in M$ và $\bar{a}$ là lớp của $a$ trong $A/m$, thì $\bar{a} \otimes x = 1 \otimes (ax)$ và do đó giả thiết kéo theo rằng tồn tại một họ $(x_i)_{i \in I}$ các phần tử của $M$ sao cho $(1 \otimes x_i)$ là một cơ sở của $(A/m)$-môđun $(A/m) \otimes_A M$. Ta đã biết rằng các $x_i$ sinh ra $M$ (Hệ quả 2 của Mệnh đề 4); ta sẽ thấy rằng chúng độc lập tuyến tính trên $A$. Vì mục đích đó, ta xét A-môđun tự do $L = A_s^{(I)}$; gọi $(e_i)$ là cơ sở chính tắc của nó và $u : A_s^{(I)} \to M$ là ánh xạ $A$-tuyến tính sao cho $u(e_i) = x_i$ với mọi $i \in I$; nếu $R$ là hạt nhân của $u$, ta sẽ chứng minh rằng $R = 0$. Dưới giả thiết (i), $(A/m) \otimes_A M$ là một $(A/m)$-môđun sinh hữu hạn, do đó $I$ tất yếu là hữu hạn và $R$ là một A-môđun sinh hữu hạn theo Chương I, § 2, no. 8, Bổ đề 9. Khi đó theo Mệnh đề 4, sẽ đủ để chứng minh (dưới một trong hai giả thiết) rằng $R = mR$.

Gọi $j$ là đơn ánh chính tắc $R \to L$; khi đó có một biểu đồ giao hoán

$$
\begin{array}{ccccc}
m \otimes R & \xrightarrow{1 \otimes j} & m \otimes L & \xrightarrow{1 \otimes u} & m \otimes M \\
\downarrow^a & & \downarrow^c & & \downarrow^c \\
R & \xrightarrow{j} & L & \xrightarrow{u} & M
\end{array}
$$

trong đó hai hàng đều khớp, $j$ là đơn ánh và $1 \otimes u$ là toàn ánh (Chương

$$
0 \xrightarrow{d} \mathrm{Coker}(a) \longrightarrow \mathrm{Coker}(b) \xrightarrow{v} \mathrm{Coker}(c)
$$

(Chương I, § 1, no. 4, Mệnh đề 2); chỉ cần kiểm tra rằng v là song ánh, vì khi đó ta suy ra rằng Coker(a) = 0, nói cách khác rằng a là toàn ánh và do đó R = mR. Bây giờ, Coker(b) = (A/m) \otimes_A L và

$$
\mathrm{Coker}(c) = (A/m) \otimes_A M
$$

và theo định nghĩa v(1 \otimes e,) = 1 \otimes x,; vì (1 \otimes e,) là một cơ sở của (A/m) \otimes_A L, định nghĩa của các x, cho thấy rằng v là song ánh.

#### Hệ quả 1 {#ac-ii-s3-prop-5-cor-1 .statement}

Cho A là một vành không nhất thiết giao hoán, m là căn Jacobson của A và M là một A-môđun trái. Giả sử rằng A/m là một trường, rằng đồng cấu chính tắc từ m \otimes_A M vào M là đơn ánh và một trong các điều kiện (i), (ii) của Mệnh đề 5 được thỏa mãn. Để một họ (y_\lambda) các phần tử của M là một cơ sở của một nhân tử trực tiếp của M, điều kiện cần và đủ là họ (1 \otimes y_\lambda) là tự do trong M/mM.

Nếu điều kiện này được thỏa mãn, có thể giả sử rằng (y_\lambda) là một họ con của một họ (x_i) các phần tử của M sao cho (1 \otimes x_i) là một cơ sở của M/mM (Đại số, Chương II, § 7, no. 1, Định lý 2) và khi đó Mệnh đề 5 chứng minh rằng (x_i) là một cơ sở của M.

#### Hệ quả 2 {#ac-ii-s3-prop-5-cor-2 .statement}

Cho A là một vành không nhất thiết giao hoán, m là căn Jacobson của A và M là một A-môđun trái. Giả sử rằng A/m là một trường và một trong các điều kiện sau được thỏa mãn:
(i) M được cho bởi hữu hạn phần sinh và hữu hạn quan hệ;
(ii) m lũy linh.
Khi đó các tính chất sau là tương đương:
(a) M là tự do;
(b) M là xạ ảnh;
(c) M là phẳng;
(d) đồng cấu chính tắc m \otimes_A M \to M là đơn ánh;
(e) Tor_1^A(A/m, M) = 0.

Các hệ quả (a) \Rightarrow (b) \Rightarrow (c) \Rightarrow (d) là ngay lập tức. Vì A/m là một trường, (A/m) \otimes_A M là một $(A/m)$-môđun tự do và Mệnh đề 5 cho thấy rằng (d) kéo theo (a).

Sau cùng, ta biết rằng Tor_1^A(A, M) = 0 và từ dãy khớp 0 \to m \to A \to A/m \to 0 ta do đó suy ra dãy khớp

$$
0 \to \mathrm{Tor}_1^A(A/m, M) \to m \otimes_A M \to M;
$$

điều này chứng minh rằng Tor$_1^A(A/m, M)$ đẳng cấu với hạt nhân của đồng cấu chính tắc $m \otimes_A M \to M$; do đó có sự tương đương của (d) và (e). \*

Có thể chứng minh rằng, với mọi vành $A$ có căn Jacobson $m$ sao cho $A/m$ là một trường, *mọi* A-môđun xạ ảnh đều là tự do (Bài tập 3).

#### Mệnh đề 6 {#ac-ii-s3-prop-6 .statement}

*Cho $A$ là một vành không nhất thiết giao hoán và $m$ là căn Jacobson của nó; giả sử rằng $A/m$ là một trường. Cho $M$ và $N$ là hai A-môđun tự do sinh hữu hạn và $u: M \to N$ là một đồng cấu. Các tính chất sau là tương đương*:

(a) $u$ là một đẳng cấu của $M$ lên một nhân tử trực tiếp của $N$;
(b) $1 \otimes u: (A/m) \otimes_A M \to (A/m) \otimes_A N$ là đơn ánh;
(c) $u$ là đơn ánh và $\operatorname{Coker}(u)$ là một A-môđun tự do;
(d) đồng cấu chuyển vị ${}^t u: N^* \to M^*$ là toàn ánh.

Ta biết (*Algebra*, Chương II, § 1, no. 11, Mệnh đề 21) rằng, nếu $N/u(M)$ là tự do, thì $u(M)$ là một nhân tử trực tiếp của $N$, do đó (c) kéo theo (a); ngược lại, (a) kéo theo rằng $\operatorname{Coker}(u)$, đẳng cấu với một phần bù của $u(M)$ trong $N$, là một A-môđun xạ ảnh sinh hữu hạn và *a fortiori* được trình bày hữu hạn (Chương I, § 2, no. 8, Bổ đề 8); do đó môđun này là tự do theo Hệ quả 2 của Mệnh đề 5 và (a) kéo theo (c). Mặt khác, (a) hiển nhiên kéo theo (b). Để đơn giản, viết $M' = (A/m) \otimes_A M$, $N' = (A/m) \otimes_A N$; vì $M$ và $N$ là sinh hữu hạn, các đối ngẫu ${M'}^*$ và ${N'}^*$ của các $(A/m)$-môđun $M'$ và $N'$ được đồng nhất một cách chính tắc với $M^* \otimes_A (A/m)$ và $N^* \otimes_A (A/m)$, và ${}^t(1 \otimes u)$ với $({}^t u) \otimes 1$ (*Algebra*, Chương II, § 5, no. 4, Mệnh đề 8); vì $M'$ và $N'$ là các không gian vectơ trên trường $A/m$, giả thiết rằng $1 \otimes u$ là đơn ánh kéo theo rằng ${}^t(1 \otimes u)$ là toàn ánh (*Algebra*, Chương 11, § 7, no. 5, Mệnh đề 10); khi đó Hệ quả 1 của Mệnh đề 4 cho thấy rằng ${}^t u$ là toàn ánh và như vậy ta đã chứng minh rằng (b) kéo theo (d). Cuối cùng ta chứng minh rằng (d) kéo theo (a). Giả sử rằng ${}^t u$ là toàn ánh; vì $M^*$ là tự do, tồn tại một đồng cấu $f$ từ $M^*$ đến $N^*$ sao cho $1_{M^*} = {}^t u \circ f$ (*Algebra*, Chương II, § 1, no. 11, Mệnh đề 21); vì $M$ và $N$ là tự do và sinh hữu hạn, tồn tại một đồng cấu $g$ từ $N$ đến $M$ sao cho $f = {}^t g$; do đó ${}^t 1_M = 1_{M^*} = {}^t u \circ {}^t g = {}^t(g \circ u)$, do đó $1_M = g \circ u$; điều này chứng minh rằng $u$ là một đẳng cấu của $M$ lên một môđun con là một nhân tử trực tiếp của $N$ (*Algebra*, Chương 11, § 1, no. 9, Hệ quả 2 của Mệnh đề 15).

#### Hệ quả {#ac-ii-s3-n2-cor-1 .statement}

*Dưới các giả thiết của Mệnh đề 6, các tính chất sau là tương đương*:

(a) $u$ là một đẳng cấu của $M$ lên $N$;
(b) $M$ và $N$ có cùng hạng (*Algebra*, Chương II, § 7, no. 2) và $u$ là toàn ánh;
(c) $1 \otimes u: M/mM \to N/mN$ là song ánh.

Các mệnh đề đã được chứng minh ở trên trong no. này thường sẽ được áp dụng khi $A$ là một *vành địa phương* và $m$ là *iđêan cực đại* của nó. Hệ quả 2 của Mệnh đề 5 khi đó được hoàn chỉnh bởi

#### Mệnh đề 7 {#ac-ii-s3-prop-7 .statement}

*Cho $A$ là một vành địa phương reduced, $m$ là iđêan cực đại của nó, $(p_i)_{i \in I}$ là họ các iđêan nguyên tố cực tiểu của $A$, $K_i$ là trường phân thức của $A/p_i$ và $M$ là một $A$-môđun sinh hữu hạn. Để $M$ là tự do thì điều kiện cần và đủ là*

$$(1)\qquad [(A/m) \otimes_A M : (A/m)] = [K, \otimes_A M : K]\qquad \text{với mọi } i \in I.$$

Nếu M là tự do thì rõ ràng hai vế của (1) đều bằng hạng của M với mọi $i \in I$. Bây giờ giả sử điều kiện đó được thỏa mãn và ký hiệu bởi $n$ giá trị chung của hai vế của (1); theo Hệ quả 2 của Mệnh đề 4, M có một hệ gồm $n$ phần tử sinh $x_j$ ($1 \leq j \leq n$). Trước hết giả sử rằng $A$ là một *miền nguyên*, khi đó $p_i = 0$ với mọi $i \in I$. Các phần tử $1 \otimes x_j$ ($1 \leq j \leq n$) sinh không gian vectơ $K \otimes M$ trên trường phân thức K của $A$; nhưng vì theo giả thiết không gian này có chiều bằng $n$ trên K, nên các phần tử $1 \otimes x_j$ độc lập tuyến tính trên K. Suy ra (*Algebra*, Chương II, § 1, no. 13, *Nhận xét* 1) rằng các $x_j$ độc lập tuyến tính trên $A$ và do đó lập thành một cơ sở của M.

Chuyển qua trường hợp tổng quát, tồn tại một đồng cấu toàn ánh $v$ từ $L = A''$ lên M. Xét biểu đồ giao hoán

$$
\begin{array}{ccc}
L & \xrightarrow{v} & M \\
|u| \downarrow & & \downarrow u' \\
\prod_i ((A/p_i) \otimes L) & \xrightarrow{v'} & \prod_i ((A/p_i) \otimes M)
\end{array}
$$

trong đó $u$ (tương ứng $u'$) là ánh xạ $x \mapsto (\phi_i(x))$ (tương ứng $y \mapsto (\psi_i(y))$),

$$
\phi_i : L \to (A/p_i) \otimes L
$$

(và tương ứng $\psi_i : M \to (A/p_i) \otimes M$) là ánh xạ chính tắc, và $v'$ là tích của các $1_{A/p_i} @ v_e$. Khi đó $(A/p)/(m/p_i) \otimes_{A/p_i} ((A/p_i) \otimes_A M) = (A/m) \otimes_A M$ và, vì $A/p_i$ là một miền nguyên địa phương, nên từ phần đầu của lập luận suy ra rằng mỗi $1_{A/p_i} \otimes v$ là một đẳng cấu; do đó $v'$ cũng vậy. Mặt khác, vì $A$ là reduced, $\bigcap_i p_i = (0)$ ($§ 2$, no. 6, Proposition 13), do đó $\bigcap_i (p_i L) = 0$ vì $L$ là tự do (*Algebra*, Chương II, $§ 3$, no. 7, *Nhận xét*); vì $p_i L$ là hạt nhân của $\phi_i$, điều này cho thấy $u$ là đơn ánh. Suy ra $v' \circ u = u' \circ v$ là đơn ánh, nên $v$ là đơn ánh và, vì $v$ là toàn ánh theo định nghĩa, điều này cho thấy rằng $M$ là tự do.

### 3. CHUYỂN TỪ ĐỊA PHƯƠNG SANG TOÀN CỤC

#### Mệnh đề 8 {#ac-ii-s3-prop-8 .statement}

*Cho $A$ là một vành, $m$ là một iđêan cực đại của $A$ và $M$ là một $A$-môđun. Nếu tồn tại một iđêan $a$ của $A$ sao cho $m$ là iđêan cực đại duy nhất của $A$ chứa $a$ và $aM = 0$, thì đồng cấu chính tắc $M \to M$, là song ánh.*

Khi đó $A/a$ là một vành địa phương với iđêan cực đại $m/a$; có thể coi $M$ như một $(A/a)$-môđun; với mọi $s \in A - m$ ảnh chính tắc của $s$ trong $A/a$ là khả nghịch, do đó phép vị tự $x \mapsto sx$ của $M$ là song ánh theo định nghĩa của $M$, như nghiệm của một bài toán phổ quát ($§ 2$, no. 2); do đó có mệnh đề.

Đặc biệt, nếu tồn tại $k \geqslant 0$ sao cho $m^k M = 0$, thì đồng cấu $M \to M_m$ là song ánh ($§ 1$, no. 1, Hệ quả của Mệnh đề 1).

#### Mệnh đề 9 {#ac-ii-s3-prop-9 .statement}

*Cho $A$ là một vành, $m$ là một iđêan cực đại của $A$, $M$ là một $A$-môđun và $k$ là một số nguyên $\geqslant 0$. Đồng cấu chính tắc $M \to M_m/m^k M_m$ là toàn ánh, có hạt nhân là $m^k M$ và xác định một đẳng cấu từ $M/m^k M$ lên $M_m/m^k M_m$.*

Vì trường hợp $k = 0$ là tầm thường, giả sử rằng $k \geqslant 1$. Từ Mệnh đề 8 suy ra rằng đồng cấu chính tắc $M/m^k M \to (M/m^k M)_m$ là song ánh. Mặt khác $(M/m^k M)_m$ được đồng nhất một cách chính tắc với $M_m/(m^k M)_m$ (§ 2, no. 4, Định lý 1) và do đó $(m^k M)_m = m^k M_m$ (§ 2, no. 7, Hệ quả của Mệnh đề 18), do đó có một đẳng cấu của $M/m^k M$ lên $M_m/m^k M_m$ ánh xạ lớp của một phần tử $x \in M$ lên lớp của $x/1$.

#### Hệ quả {#ac-ii-s3-n3-cor-1 .statement}

*Cho $A$ là một vành, $m_1, m_2, \ldots, m_n$ là các iđêan cực đại phân biệt của $A$, $M$ là một $A$-môđun và $k_1, k_2, \ldots, k_n$ là các số nguyên $\geqslant 0$. Đồng cấu chính tắc từ $M$ tới $\prod^n M_m/m_{i_1}^{k_1} M_m$ là toàn ánh và hạt nhân của nó là $\left( \bigcap^n m_{i_1}^{k_1} \right) M$.*

Điều này suy ra dễ dàng từ Mệnh đề 9 và $§ 1$, no. 2, Mệnh đề 6, các $m_{i_1}^{k_1}$ đôi một nguyên tố cùng nhau ($§ 1$, no. 2, Mệnh đề 3).

*Trong phần còn lại của no. này, $A$ sẽ chỉ một vành và $\Omega(A)$ (hoặc $\Omega$) tập hợp các iđêan cực đại của $A$.*

#### Mệnh đề 10 {#ac-ii-s3-prop-10 .statement}

*$A$-môđun* $\bigoplus_{m \in \Omega} \mathbf{A}_m$, *tổng trực tiếp của các* $\mathbf{A}_m$ *với* $m \in \Omega$, *là trung thành phẳng*.

Mỗi $\mathbf{A}_m$ là một A-môđun phẳng (§ 2, no. 4, Định lý 1), do đó $E = \bigoplus_{m \in \Omega} \mathbf{A}_m$ là phẳng (Chương I, § 2, no. 3, Mệnh đề 2). Hơn nữa, với mọi iđêan cực đại $m$ của $A$, $mA_m$ là iđêan cực đại duy nhất của $\mathbf{A}_m$, do đó $mA_m \neq A_m$, từ đó suy ra $mE \neq E$ và vì thế $E$ là trung thành phẳng (Chương I, § 3, no. 1, Mệnh đề 1 (d)).

#### Định lý 1 {#ac-ii-s3-thm-1 .statement}

*Cho* $M, N$ *là hai A-môđun, $u : M \to N$ một A-đồng cấu và, với mọi* $m \in \Omega$, *cho* $u_m : M, \to N_m$ *là* $A_m$-*đồng cấu tương ứng* (§ 2, no. 2, Nhận xét 5). *Để* $u$ *là đơn ánh (tương ứng, toàn ánh, song ánh, không), điều kiện cần và đủ là, với mọi* $m \in \Omega$, $u_m$ *là đơn ánh (tương ứng, toàn ánh, song ánh, không)*.

Nói rằng, với mọi $m \in \Omega$, $u_m$ là đơn ánh (tương ứng, toàn ánh, song ánh, không) là tương đương với nói rằng đồng cấu $\bigoplus_m u_m : \bigoplus M, \to \bigoplus N$, có cùng tính chất đó. Nhưng $\bigoplus_m M_m = M \otimes_A E, \bigoplus_m N_m = N \otimes_A E$ và $\bigoplus_m u_m = u \otimes 1$, trong đó $E = \bigoplus_m \mathbf{A}_m$; vì $E$ là trung thành phẳng (Mệnh đề 10), định lý suy ra từ Chương I, § 3, no. 1, Mệnh đề 1 (c) và Mệnh đề 2.

#### Hệ quả 1 {#ac-ii-s3-thm-1-cor-1 .statement}

*Cho* $M$ *là một A-môđun, N một môđun con của* $M$ *và* $x$ *một phần tử của* $M$. *Để* $x \in N$, *điều kiện cần và đủ là, với mọi* $m \in R$, *ảnh chính tắc của* $x$ *trong* $M$, *thuộc* $N$.

Cho $\bar{x}$ là lớp của $x$ trong $M/N$; nói rằng $x \in N$ có nghĩa là ánh xạ A-tuyến tính $u : a \mapsto a\bar{x}$ từ $A$ đến $M/N$ là không. Bây giờ, $(M/N)_m$ được đồng nhất với $M_m/N_m$ (§ 2, no. 4, Định lý 1) và $u_m : A_m \to M_m/N_m$ với ánh xạ $A \mapsto \lambda \bar{x}_m$, trong đó $\bar{x}_m$ là lớp mod. $N$, của ảnh chính tắc của $x$ trong $M$. Vì quan hệ $u = 0$ là tương đương với $u_m = 0$ với mọi $m$ theo Định lý 1, điều này chứng minh hệ quả.

#### Hệ quả 2 {#ac-ii-s3-thm-1-cor-2 .statement}

*Cho* $M$ *là một A-môđun và, với mọi* $m \in \Omega$, *cho* $f_m$ *là ánh xạ chính tắc* $M \to M_m$. *Đồng cấu* $x \mapsto (f_m(x))$ *từ* $M$ *đến* $\prod_{m \in \Omega} M_m$ *là đơn ánh*.

Áp dụng Hệ quả 1 trong trường hợp $N = 0$, ta thấy rằng quan hệ $x = 0$ là tương đương với $f_m(x) = 0$ với mọi $m \in \Omega$.

#### Hệ quả 3 {#ac-ii-s3-thm-1-cor-3 .statement}

(i) *Cho* $b$ *là một iđêan của* $A$ *và* $a$ *là một phần tử của* $A$. *Để có* $a \in b$, *điều kiện cần và đủ là, với mọi* $m \in \Omega$, *ảnh chính tắc của* $a$ *trong* $A_m$ *thuộc* $bA_m$.

(ii) Đặc biệt, cho b và c là hai phần tử của A. Để c là một bội của b, điều kiện cần và đủ là, với mọi $m \in \Omega$, ảnh chính tắc của c trong A, là một bội của ảnh chính tắc của b.

Vì $bA_m = b_m$ (§ 2, no. 7, Hệ quả của Mệnh đề 18), (i) là một trường hợp riêng của Hệ quả 1; (ii) suy ra từ (i) áp dụng cho iđêan $Ab$.

#### Hệ quả 4 {#ac-ii-s3-thm-1-cor-4 .statement}

Cho A là một miền nguyên, K là trường phân thức của nó và M là một A-môđun không xoắn sao cho M được đồng nhất một cách chính tắc với một A-môđun con của $K \otimes_A M$. Khi đó, với mọi $m \in \Omega$, $M_m$ được đồng nhất một cách chính tắc với một A-môđun con của $K \otimes_A M$ và $M = \bigcap_{m \in \Omega} M_m$.

Vì M được đồng nhất với một môđun con của $K \otimes_A M$, $M_m$ được đồng nhất với một A-môđun con của $(K \otimes_A M)_m = K_m \otimes_A M$ (§ 2, no. 4, Định lý 1); vì $K_m = K$, ta thấy ngay rằng $M_m$ không xoắn; hơn nữa, tính giao hoán của biểu đồ

$$
\begin{array}{ccc}
M & \longrightarrow & K \otimes_A M \\
\downarrow & & \uparrow \\
M_m & \longrightarrow & (K \otimes_A M)_m
\end{array}
$$

chứng minh rằng ánh xạ chính tắc $M \to M_m$ là đơn ánh. Khi đó hệ quả suy ra từ Hệ quả 1 áp dụng cho A-môđun $K \otimes_A M$ và môđun con M của nó.

Đặc biệt, với mọi miền nguyên A,

(2)
$$
A = \bigcap_{m \in \Omega} A_m.
$$

#### Hệ quả 5 {#ac-ii-s3-thm-1-cor-5 .statement}

Cho A là một vành. Mọi hệ sinh của A-môđun $A^n$ gồm n phần tử đều là một cơ sở của $A^n$.

Cho $(e_i)_{1 \leq i \leq n}$ là cơ sở chính tắc của $A''$, $(x_i)_{1 \leq i \leq n}$ là một hệ sinh của $A^n$ gồm n phần tử và $u : A^n \to A''$ là ánh xạ A-tuyến tính sao cho $u(e_i) = x_i$ với $1 \leq i \leq n$. Theo giả thiết, $u$ là toàn ánh và cần phải chứng minh rằng $u$ là đơn ánh. Nhờ Định lý 1, điều này ngay lập tức có thể được quy về trường hợp A là một vành địa phương; nếu $m$ là iđêan cực đại của A, thì các phần tử $1 \otimes x_i$ ($1 \leq i \leq n$) trong $(A/m)^n$ khi đó tạo thành một hệ sinh của $(A/m)$-môđun tự do $(A/m)^n$; vì $A/m$ là một trường, hệ này là một cơ sở của $(A/m)^n$; vì $A^n$ là một A-môđun tự do, ta suy ra từ Mệnh đề 5 rằng $(x_i)$ là một cơ sở của $A^n$.

#### Mệnh đề 11 {#ac-ii-s3-prop-11 .statement}

Cho M là một A-môđun, N là một A-môđun hữu hạn sinh và $u : M \to N$ là một đồng cấu. Để $u$ là toàn ánh, điều kiện cần và đủ là, với mọi $m \in S_2$, đồng cấu $M/mM \to N/mN$ dẫn xuất từ $u$ bằng cách lấy thương là toàn ánh.

Từ Định lý 1 suy ra rằng, để $u$ là toàn ánh, điều kiện cần và đủ là $u_m : M_m \to N_m$ là toàn ánh với mọi $m \in \Omega$. Vì $A_m$ là một vành địa phương và $N_m$ là một $A_m$-môđun hữu hạn sinh, điều này tương đương với việc nói rằng đồng cấu $u'_m : M_m/mM_m \to N_m/mN_m$, thu được bằng cách lấy thương, là toàn ánh (no. 2, Hệ quả 1 của Mệnh đề 4); nhưng $M_m/mM_m$ (tương ứng $N_m/mN_m$) được đồng nhất với $M/mM$ (tương ứng $N/mN$) (Mệnh đề9), do đó có mệnh đề.

#### Mệnh đề 12 {#ac-ii-s3-prop-12 .statement}

*Cho E, F, G là ba A-môđun và $v : G \to F$, $u : E \to F$ là các đồng cấu. Giả sử E là hữu hạn trình bày. Để tồn tại một đồng cấu $w : E \to G$ sao cho $u$ phân tích thành $E \xrightarrow{w} G \xrightarrow{v} F$, điều kiện cần và đủ là, với mọi $m \in S_2$, tồn tại một đồng cấu $w^m : E_m \to G$, sao cho $u_m : E_m \to F$, phân tích thành $E \xrightarrow{w^m} G_m \xrightarrow{v_m} F$,*

Sự tồn tại của $w$ thỏa mãn mệnh đề trên là tương đương với tính chất sau: $u$ thuộc vào ảnh P của ánh xạ

$$
r = \operatorname{Hom}(1_E, v) : \operatorname{Hom}_A(E, G) \to \operatorname{Hom}_A(E, F).
$$

Bây giờ, $(\operatorname{Hom}_A(E, F))_m$ (tương ứng $(\operatorname{Hom}_A(E, G))_m$) được đồng nhất một cách chính tắc với $\operatorname{Hom}_{A_m}(E_m, F_m)$ (tương ứng $\operatorname{Hom}_{A_m}(E_m, G_m)$) (§ 2, no. 7, Mệnh đề 19 (i)), ảnh chính tắc của $u$ trong $(\operatorname{Hom}_A(E, F))_m$ được đồng nhất với $u_m$, $r_m$ được đồng nhất với $\operatorname{Hom}_{A_m}(1_{E_m}, v)$ và $P_m$ với ảnh của $r_m$. Khi đó mệnh đề suy ra từ Hệ quả 1 của Định lý 1 áp dụng cho $\operatorname{Hom}_A(E, F)$ và môđun con P của nó.

#### Hệ quả 1 {#ac-ii-s3-prop-12-cor-1 .statement}

*Cho M là một A-môđun và N là một môđun con của M sao cho M/N là hữu hạn trình bày. Để N là một nhân tử trực tiếp của M, điều kiện cần và đủ là, với mọi $m \in S_2$, N là một nhân tử trực tiếp của M.*

Nói rằng N là một nhân tử trực tiếp của M có nghĩa là đồng cấu đồng nhất trên M/N phân tích qua $M/N \xrightarrow{w} M \xrightarrow{\phi} M/N$ trong đó $\phi$ là đồng cấu chính tắc và $w$ là một đồng cấu (*Đại số*, Chương II, § 1, no. 9, Mệnh đề 14); vì $(M/N)_m = M_m/N_m$ và $\phi_m$ là đồng cấu chính tắc $M_m \to M_m/N_m$, hệ quả suy ra dễ dàng từ Mệnh đề 12.

#### Hệ quả 2 {#ac-ii-s3-prop-12-cor-2 .statement}

*Cho M là một A-môđun tự do sinh hữu hạn và N là một môđun con của M, bản thân nó là một A-môđun tự do sinh hữu hạn. Để N là một nhân tử trực tiếp của M, điều kiện cần và đủ là, với mọi $m \in \Omega$, ta có $mN = N \cap (mM)$.*

Theo định nghĩa, M/N được trình bày hữu hạn; mặt khác, N và M là các $A_n$-môđun tự do sinh hữu hạn. Để $N$ là một nhân tử trực tiếp của $M$, điều kiện cần và đủ là ánh xạ chính tắc $N_m / mN_m \to M_m / mM_m$ đơn ánh (no. 2, Mệnh đề 6); điều này cũng chính là nói rằng ánh xạ chính tắc $N / mN \to M / mM$ phải đơn ánh (Mệnh đề 9), và vì hạt nhân của nó là $(N \cap mM) / mN$, điều này chứng minh hệ quả.

Mệnh đề 12 (resp. Hệ quả 1 của nó) sẽ được áp dụng đặc biệt khi $A$ là Noether và $E$ (resp. $M/N$) là một $A$-môđun *sinh hữu hạn* (Chương I, § 2, no. 8, Bổ đề 8).

### 4. ĐỊA PHƯƠNG HÓA TÍNH PHẲNG

#### Mệnh đề 13 {#ac-ii-s3-prop-13 .statement}

*Cho $S$ là một tập con nhân tính của một vành $A$ và $M$ là một $A$-môđun. Nếu $M$ là phẳng (resp. trung thành phẳng), $S^{-1}M$ là một $S^{-1}A$-môđun phẳng (resp. trung thành phẳng) và là một $A$-môđun phẳng.*

Vì $S^{-1}M = M \otimes_A S^{-1}A$, mệnh đề thứ nhất suy ra từ Chương I, § 2, no. 7, Hệ quả 2 của Mệnh đề 8 (resp. Chương I, § 3, no. 3, Mệnh đề 5); hơn nữa, $S^{-1}A$ là một $A$-môđun phẳng ($§ 2$, no. 4, Định lý 1); do đó nếu $M$ là một $A$-môđun phẳng thì $S^{-1}M$ cũng vậy theo Chương I, § 2, no. 7, Hệ quả 3 của Mệnh đề 8.

#### Nhận xét {#ac-ii-s3-n4-rem-1 .statement}

Nếu $N$ là một $S^{-1}A$-môđun, $S^{-1}N$ được đồng nhất với $N$ và vì thế điều này *tương đương* với việc nói rằng $N$ là một $S^{-1}A$-môđun phẳng hoặc một $A$-môđun phẳng.

#### Mệnh đề 14 {#ac-ii-s3-prop-14 .statement}

*Cho $A$ là một vành, $B$ là một $A$-đại số giao hoán và $T$ là một tập con nhân tính của $B$. Nếu $N$ là một $B$-môđun phẳng như một $A$-môđun, thì $T^{-1}N$ là một $A$-môđun phẳng.*

$T^{-1}N = T^{-1}B \otimes_B N$; khi đó mệnh đề suy ra từ Chương I, § 2, no. 7, Mệnh đề 8, áp dụng với $A$ được thay bởi $B$, $B$ bởi $A$, $E$ bởi $T^{-1}B$ và $F$ bởi $N$.

#### Mệnh đề 15 {#ac-ii-s3-prop-15 .statement}

*Cho $A, B$ là hai vành, $\phi : A \to B$ là một đồng cấu và $N$ là một $B$-môđun. Các tính chất sau là tương đương:
(a) $N$ là một A-môđun phẳng.
(b) *Với mọi iđêan cực đại $n$ của $B$, $N_n$ là một A-môđun phẳng.*
(c) *Với mọi iđêan cực đại $n$ của $B$, nếu ta viết $m = \phi(n)$, thì $N_n$ là một $A_m$-môđun phẳng.*

Với mọi $a \notin m$, phép vị tự của $N_n$ cảm sinh bởi $a$ là song ánh, do đó $N_n$ được đồng nhất một cách chính tắc với $(N_n)_m$ và tính tương đương của (b) và (c) suy ra từ

Nhận xét theo sau Mệnh đề 13; việc (a) kéo theo (b) là một trường hợp riêng của Mệnh đề 14. Còn phải chứng minh rằng (b) kéo theo (a), nghĩa là, nếu (b) đúng thì với mọi đồng cấu đơn ánh của A-môđun $u : M \to M'$, đồng cấu $v = 1 @ u : N \otimes_A M \to N @^* M'$ là đơn ánh. Bây giờ, $v$ cũng là một đồng cấu B-môđun, và để nó là đơn ánh, điều kiện cần và đủ là $v,, : (N \otimes_A M),, \to (N \otimes_A M'),,$ cũng như vậy với mọi iđêan cực đại $n$ của $B$ (no. 3, Định lý 1). Vì
$$
(N \otimes_A M)_n = B_n \otimes_B (N @_A M) = N_n \otimes_A M,
$$
$v_n$ chính là đồng cấu $1 \otimes u : N_n \otimes_A M \to N_n \otimes_A M'$, đồng cấu này là đơn ánh vì theo giả thiết $N_n$ là một A-môđun phẳng.

#### Hệ quả {#ac-ii-s3-n4-cor-1 .statement}

*Để một A-môđun M là phẳng (tương ứng, phẳng trung thành), điều kiện cần và đủ là, với mọi iđêan cực đại m của A, M, là một $A_m$-môđun phẳng (tương ứng, phẳng trung thành).*

Tính cần thiết của các điều kiện suy ra từ Mệnh đề 13. Ngược lại, nếu $M,$ là một $A_m$-môđun phẳng với mọi iđêan cực đại $m$ của $A$, thì $M$ là một A-môđun phẳng theo Mệnh đề 15 áp dụng cho trường hợp $\phi$ là đồng nhất. Sau hết, nếu $M,$ là một $A_m$-môđun phẳng trung thành với mọi $m$, thì $mM_m = mA_mM_m \neq M,$ nên $mM \neq M$ với mọi $m$ (no. 3, Mệnh đề 9), điều đó chứng minh rằng $M$ là một A-môđun phẳng trung thành (Chương I, § 3, no. 1, Mệnh đề 1 (d)).

### 5. VÀNH NỬA ĐỊA PHƯƠNG

#### Mệnh đề 16 {#ac-ii-s3-prop-16 .statement}

*Cho A là một vành. Các tính chất sau là tương đương:
(a) tập hợp các iđêan cực đại của A là hữu hạn;
(b) thương của A theo căn Jacobson của nó là hợp thành trực tiếp của một số hữu hạn trường.*

Giả sử rằng thương của A theo căn Jacobson $\mathfrak{R}$ của nó là hợp thành trực tiếp của một số hữu hạn trường. Khi đó $A/\mathfrak{R}$ chỉ có một số hữu hạn iđêan và *a fortiori* chỉ có một số hữu hạn iđêan cực đại. Vì mọi iđêan cực đại đều chứa $\mathfrak{R}$ (*Algebra*, Chapter VIII, § 6, no. 2, Definition 2), các iđêan cực đại của A là các ảnh nghịch đảo của các iđêan cực đại của $A/\mathfrak{R}$ dưới đồng cấu chính tắc $A \to A/\mathfrak{R}$; do đó số lượng của chúng là hữu hạn.

Ngược lại, giả sử rằng A chỉ có một số hữu hạn iđêan cực đại phân biệt $m_1, \ldots, m_n$. Các $A/m_i$ là những trường và từ § 1, no. 2, Mệnh đề 5 suy ra rằng ánh xạ chính tắc $A \to \prod_{i=1}^n A/m_i$ là toàn ánh; vì hạt nhân của nó $\bigcap_{i=1}^n m_i$ là căn Jacobson $\mathfrak{R}$ (*Algebra*, Chapter VIII, § 6, no. 2, Definition 2), nên $A/\mathfrak{R}$ đẳng cấu với $\prod_{i=1}^n A/m_i$.

#### Định nghĩa 4 {#ac-ii-s3-def-4 .statement}

Một vành được gọi là nửa địa phương nếu nó thỏa mãn các điều kiện tương đương (a), (b) của Mệnh đề 16.

#### Ví dụ {#ac-ii-s3-n5-exa-1 .statement}

Mọi vành địa phương đều là nửa địa phương. Mọi thương của một vành nửa địa phương đều là nửa địa phương. Mọi tích hữu hạn của các vành nửa địa phương đều là nửa địa phương.

Nếu A là một vành Noether nửa địa phương và B là một đại số trên A đồng thời là một A-môđun hữu hạn sinh, thì B là nửa địa phương (Chương IV, § 2, no. 5, Hệ quả 3 của Mệnh đề 9).

Một ví dụ khác, tổng quát hóa phép dựng các vành địa phương $A_{\mathfrak{p}}$, được cho bởi mệnh đề sau:

#### Mệnh đề 17 {#ac-ii-s3-prop-17 .statement}

Cho A là một vành và $\mathfrak{p}_1, \ldots, \mathfrak{p}_n$ là các iđêan nguyên tố của A. Ta viết
$$ S = \bigcap_1^n (A - \mathfrak{p}_i) = A - \bigcup_1^n \mathfrak{p}_i. $$

(a) Vành $S^{-1}A$ là nửa địa phương; nếu $q_1, \ldots, q_r$ là các phần tử cực đại phân biệt (đối với phép bao hàm) của tập hợp các $\mathfrak{p}_i$, các iđêan cực đại của $S^{-1}A$ là các $S^{-1}q_j$ ($1 \leq j \leq r$) và các iđêan này là phân biệt.

(b) Vành $A_{\mathfrak{p}_i}$ đẳng cấu chính tắc với $(S^{-1}A)_{S^{-1}\mathfrak{p}_i}$ với $1 \leq i \leq n$.

(c) Nếu A là một miền nguyên, thì $S^{-1}A = \bigcap_1^n A_{\mathfrak{p}_i}$, trong trường các phân thức của A.

(a) Các iđêan của A không giao với S là các iđêan được chứa trong hợp của các $\mathfrak{p}_i$ và do đó trong ít nhất một trong các $\mathfrak{p}_i$ (§ 1, no. 1, Mệnh đề 2); các $q_j$ do đó là các phần tử cực đại của tập hợp các iđêan không giao với S; do đó, các $S^{-1}q_j$ là các iđêan cực đại của $S^{-1}A$ theo § 2, no. 5, Mệnh đề 11 (ii).

(b) là một trường hợp đặc biệt của § 2, no. 5, Mệnh đề 11 (iii).

(c) Giả sử rằng A là một miền nguyên. Nếu $\mathfrak{p}_i \subset \mathfrak{p}_k$, thì $A_{\mathfrak{p}_i} \supset A_{\mathfrak{p}_k}$; để chứng minh (c), do đó ta có thể giả sử rằng không có hai $\mathfrak{p}_i$ nào so sánh được. Khi đó suy ra từ (a) và no. 3, Hệ quả 4 của Định lý 1 rằng $S^{-1}A = \bigcap_1^n (S^{-1}A)_{S^{-1}\mathfrak{p}_i}$; do đó (c) theo (b).

Nếu A là một miền nguyên, thì $S^{-1}A$ cũng là một miền nguyên và Mệnh đề 17 khi đó cung cấp một ví dụ về một vành nửa địa phương không phải là một hợp thành trực tiếp của các vành địa phương (xem Chương III, § 2, no. 13).

#### Hệ quả {#ac-ii-s3-n5-cor-1 .statement}

Cho A là một miền nguyên và $\mathfrak{p}_1, \ldots, \mathfrak{p}_n$ là các iđêan nguyên tố của A, không có hai iđêan nào trong số đó so sánh được đối với phép bao hàm. Nếu $A = \bigcap_1^n A_{\mathfrak{p}_i}$ trong trường các phân thức của A, các iđêan cực đại của A là $\mathfrak{p}_1, \ldots, \mathfrak{p}_n$.

Đặt $S = \bigcap_{i=1}^n (\mathbf{A} - p_i)$, $S^{-1}\mathbf{A} = \mathbf{A}$ theo Mệnh đề 17 (c); do đó các phần tử của $S$ là khả nghịch trong $\mathbf{A}$ và $S^{-1}p_i = p_i$ với mọi $i$. Mệnh đề của chúng ta sau đó suy ra theo Mệnh đề 17 (a).

### Bài tập {#ac-ii-s3-exercises}

Xem các [bài tập cho § 3](exercises/s3/).
