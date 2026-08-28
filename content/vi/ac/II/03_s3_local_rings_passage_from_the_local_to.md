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
content_sha256: 9c20c3c214e5ae3c3da7451136844419ef43b2c85c04f0fc975cf6678b1e0508
translated_from: content/en/ac/II/03_s3_local_rings_passage_from_the_local_to.md
source_content_sha256: b95c1024d708413f196f7407025c624c77589ba41ff70622a5c8b484baf0c3a4
translation_model: gpt-5.4-mini, gpt-5-6-mini
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
(1) Một trường là một vành địa phương. Một vành được thu gọn về 0 không phải là một vành địa phương.
(2) Cho $\mathbf{A}$ là một vành địa phương và $k$ là trường thặng dư của nó. Vành chuỗi lũy thừa hình thức $B = \mathbf{A}[[X_1, \ldots, X_n]]$ là một vành địa phương, vì các phần tử không khả nghịch của $B$ là các chuỗi lũy thừa hình thức mà các số hằng không khả nghịch trong $\mathbf{A}$ (Đại số, Chương IV, §5, no. 6, Mệnh đề 4). Đơn ánh chính tắc của $\mathbf{A}$ vào $B$ là một đồng cấu địa phương và đơn ánh tương ứng của các trường thặng dư là một đẳng cấu.
(3) Cho $b$ là một iđêan của một vành $\mathbf{A}$ chỉ được chứa trong một iđêan cực đại duy nhất $m$; khi đó $A/b$ là một *vành địa phương* với iđêan cực đại $m/b$ và trường thặng dư đẳng cấu chính tắc với $A/m$. Điều này đặc biệt áp dụng cho trường hợp $b = m^k$, $m$ là một iđêan cực đại bất kỳ của $A$ ($\S 1$, no. 1, Hệ quả của Mệnh đề 1). Nếu bản thân $A$ là một vành địa phương với iđêan cực đại $m$, thì với mọi iđêan $b \neq A$ của $A$, $A/b$ là một vành địa phương, đồng cấu chính tắc $A \to A/b$ là một đồng cấu địa phương và đồng cấu tương ứng của các trường thặng dư là một *đẳng cấu*.

(4) Cho $X$ là một không gian tôpô, $x_0$ là một điểm của $X$ và $A$ là vành các mầm tại điểm $x_0$ của các hàm thực liên tục trong một lân cận của $x_0$ (*Tôpô đại cương*, Chương I, \$6, no. 10). Rõ ràng, để mầm tại $x_0$ của một hàm liên tục $f$ khả nghịch trong $A$, điều kiện cần và đủ là $f(x_0) \neq 0$, vì điều đó suy ra $f(x) \neq 0$ trong một lân cận của $x_0$. Do đó vành $A$ là một vành địa phương có iđêan cực đại $m$ là tập hợp các mầm của những hàm bằng không *tại* $x_0$; lấy các thương, ánh xạ $g \mapsto g(x_0)$ từ $A$ vào $\mathbf{R}$ cho một *đẳng cấu* của trường thặng dư $A/m$ lên $\mathbf{R}$.

#### Mệnh đề 2 {#ac-ii-s3-prop-2 .statement}

*Cho $A$ là một vành và $p$ là một iđêan nguyên tố của $A$. Vành $A$, là địa phương; iđêan cực đại của nó là iđêan $pA_p = p_v$, được sinh bởi ảnh chính tắc của $p$ trong $A$; trường thặng dư của nó đẳng cấu chính tắc với trường phân thức của $A/p$.*

Cho $S = A - p$ và $j : A \to A_v$, là đồng cấu chính tắc; giả thiết rằng $p$ là nguyên tố suy ra rằng $p$ bão hòa đối với $S$, do đó $j^{-1}(pA_p) = p$ ($\S 2$, no. 4, Mệnh đề 10) và, vì các iđêan của $A$ không giao với $S$ chính là các iđêan được chứa trong $p$, hai mệnh đề đầu là các trường hợp riêng của $\S 2$, no. 5, Mệnh đề 11 (ii). Hơn nữa, iff là đồng cấu chính tắc $A \to A/p$, $f(S)$ là tập hợp các phần tử $\neq 0$ của miền nguyên $A/p$ và do đó khẳng định cuối cùng là một trường hợp riêng của $\S 2$, no. 5, Mệnh đề 11 (i).

#### Định nghĩa 3 {#ac-ii-s3-def-3 .statement}

*Cho $A$ là một vành và $p$ là một iđêan nguyên tố của $A$. Vành $A$, được gọi là vành địa phương của $A$ tại $p$, hay vành địa phương của $p$, khi không có sự nhập nhằng.*

*Nhận xét (2).* Nếu $A$ là một vành địa phương và $m$ là iđêan cực đại của nó, các phần tử của $A - m$ là khả nghịch (Mệnh đề 1) và do đó $A_{m'}$ được đồng nhất một cách chính tắc với $A$ ($\S 2$, no. 1, Nhận xét 5).

Ví dụ
(5) Cho $p$ là một số nguyên tố. Vành địa phương $\mathbf{Z}_{(p)}$ là tập hợp các số hữu tỉ $a/b$, trong đó $a, b$ là các số nguyên hữu tỉ với $b$ nguyên tố trên; trường thặng dư của $\mathbf{Z}_{(p)}$ đẳng cấu với trường nguyên tố $\mathbf{F}_p = \mathbf{Z}/(p)$.

(6) Cho $V$ là một đa tạp đại số affine, $A$ là vành các hàm chính quy trên $V$, $W$ là một đa tạp con bất khả quy của $V$ và $p$ là iđêan (nhất thiết là nguyên tố) của $A$ gồm các hàm bằng không tại mọi điểm của $W$. Vành $A$, được gọi là vành địa phương của $W$ trên $V$. \*

#### Mệnh đề 3 {#ac-ii-s3-prop-3 .statement}

Cho $A$ là một vành, $p$ là một iđêan nguyên tố của $A$ và $S = A - p$. Với mọi iđêan $b'$ của $A_p$ phân biệt với $A_p$, gọi $b$ là iđêan $(i_A^S)^{-1}(b')$ của $A$ sao cho $b' = bA_p$.

(i) Cho $f$ là đồng cấu chính tắc $A \to A/b$. Đồng cấu từ $A$ vào $(A/b)_{p/b}$ liên kết một cách chính tắc với $f$ ($\S 2$, no. 1, Mệnh đề 2) là toàn ánh và hạt nhân của nó là $b'$, do đó, bằng cách lấy thương, xác định một đẳng cấu chính tắc của $A_p/b'$ lên $(A/b)_{p/b}$.

(ii) Ánh xạ $b' \to b = (i_A^S)^{-1}(b')$, hạn chế trên tập hợp các iđêan nguyên tố của $A_p$, là một đẳng cấu (theo quan hệ bao hàm) của tập hợp này lên tập hợp các iđêan nguyên tố của $A$ được chứa trong $p$. Nếu $b'$ là nguyên tố trong $A_p$, tồn tại một đẳng cấu của vành $A_b$ lên vành $(A_p)_{b'}$, ánh xạ $a/s$ thành $(a/1)/(s/1)$ với mọi $a \in A, s \in A - b$.

Đây chỉ là một trường hợp riêng của $\S 2$, no. 5, Mệnh đề 11.

Nhận xét
(3) Nếu $a$ là một iđêan của $A$ không được chứa trong $p$, thì $aA_p = A$, và $(A/a)_p = 0$ ($\S 2$, no. 5, Nhận xét).
(4) Cho $A, B$ là hai vành, $\rho : A \to B$ là một đồng cấu, $q$ là một iđêan nguyên tố của $B$ và $p$ là iđêan nguyên tố $\rho^{-1}(q)$ của $A$. Vì $\rho(A - p) \subset B - q$, một đồng cấu chính tắc $\rho_q : A \to B_q$ được dẫn xuất từ $\rho$ ($\S 2$, no. 1, Mệnh đề 2) và ngay lập tức có $\rho_q(pA_p) \subset qB_q$, do đó $\rho$ là một đồng cấu địa phương.

### 2. MÔĐUN TRÊN MỘT VÀNH ĐỊA PHƯƠNG

#### Mệnh đề 4 {#ac-ii-s3-prop-4 .statement}

Cho $A$ là một vành không nhất thiết giao hoán, $m$ là một iđêan phải của $A$ được chứa trong căn Jacobson của $A$ và $M$ là một $A$-môđun trái. Giả sử một trong các điều kiện sau được thỏa mãn:
(i) $M$ sinh hữu hạn;
(ii) $m$ lũy linh.
Khi đó quan hệ $(A_d/m) \otimes_A M = 0$ kéo theo $M = 0$.

Mệnh đề tương ứng với giả thiết (i) chính xác là Hệ quả 3 của Mệnh đề 6 của Đại số, chương VIII, $\S 6$, no. 3. Mặt khác, quan hệ $(A_d/m) \otimes_A M = 0$ tương đương với $M = mM$ và do đó kéo theo $M = m^nM$ với mọi số nguyên $n > 0$; do đó có mệnh đề tương ứng với giả thiết (ii).

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

Nếu $a \in A$, $x \in M$ và $\bar{a}$ là lớp của $a$ trong $A/m$, thì $\bar{a} \otimes x = 1 \otimes (ax)$ và do đó giả thiết suy ra rằng tồn tại một họ $(x_i)_{i \in I}$ các phần tử của $M$ sao cho $(1 \otimes x_i)$ là một cơ sở của $(A/m)$-môđun $(A/m) \otimes_A M$. Ta đã biết rằng các $x_i$ sinh $M$ (Hệ quả 2 của Mệnh đề 4); ta sẽ thấy rằng chúng độc lập tuyến tính trên $A$. Với mục đích này, xét môđun $A$ tự do $L = A_s^{(I)}$; gọi $(e_i)$ là cơ sở chính tắc của nó và $u : A_s^{(I)} \to M$ là ánh xạ $A$-tuyến tính sao cho $u(e_i) = x_i$ với mọi $i \in I$; nếu $R$ là hạt nhân của $u$, ta sẽ chứng minh rằng $R = 0$. Theo giả thiết (i), $(A/m) \otimes_A M$ là một $(A/m)$-môđun sinh hữu hạn, do đó $I$ nhất thiết hữu hạn và $R$ là một $A$-môđun sinh hữu hạn theo Chương I, § 2, no. 8, Bổ đề 9. Khi đó theo Mệnh đề 4, chỉ cần chứng minh (dưới một trong hai giả thiết) rằng $R = mR$ là đủ.

Gọi $j$ là đơn ánh chính tắc $R \to L$; khi đó có một biểu đồ giao hoán

$$
\begin{array}{ccccc}
m \otimes R & \xrightarrow{1 \otimes j} & m \otimes L & \xrightarrow{1 \otimes u} & m \otimes M \\
\downarrow^a & & \downarrow^c & & \downarrow^c \\
R & \xrightarrow{j} & L & \xrightarrow{u} & M
\end{array}
$$

trong đó hai hàng là khớp, $j$ là đơn ánh và $1 \otimes u$ là toàn ánh (Chương

$$
0 \xrightarrow{d} \mathrm{Coker}(a) \longrightarrow \mathrm{Coker}(b) \xrightarrow{v} \mathrm{Coker}(c)
$$

(Chương I, § 1, no. 4, Mệnh đề 2); chỉ cần kiểm tra rằng v là song ánh, vì khi đó ta suy ra rằng Coker(a) = 0, nói cách khác là $a$ là toàn ánh và do đó $R = mR$. Bây giờ, Coker(b) = (A/m) \otimes_A L và

$$
\mathrm{Coker}(c) = (A/m) \otimes_A M
$$

và theo định nghĩa $v(1 \otimes e,) = 1 \otimes x,;$ vì $(1 \otimes e,)$ là một cơ sở của $(A/m) \otimes_A L$, định nghĩa của các $x,$ cho thấy rằng v là song ánh.

#### Hệ quả 1 {#ac-ii-s3-prop-5-cor-1 .statement}

Cho A là một vành không nhất thiết giao hoán, m là căn Jacobson của A và M là một A-môđun trái. Giả sử rằng A/m là một trường, rằng đồng cấu chính tắc từ $m \otimes_A M$ đến $M$ là đơn ánh và rằng một trong các điều kiện (i), (ii) của Mệnh đề 5 được thỏa mãn. Để một họ $(y_\lambda)$ các phần tử của M là một cơ sở của một nhân tử trực tiếp của M, điều kiện cần và đủ là họ $(1 \otimes y_\lambda)$ là tự do trong M/mM.

Nếu điều kiện này đúng, có thể giả sử rằng $(y_\lambda)$ là một họ con của một họ $(x_i)$ các phần tử của M sao cho $(1 \otimes x_i)$ là một cơ sở của M/mM (Đại số, Chương II, § 7, no. 1, Định lý 2) và Mệnh đề 5 khi đó chứng minh rằng $(x_i)$ là một cơ sở của M.

#### Hệ quả 2 {#ac-ii-s3-prop-5-cor-2 .statement}

Cho A là một vành không nhất thiết giao hoán, m là căn Jacobson của A và M là một A-môđun trái. Giả sử rằng A/m là một trường và một trong các điều kiện sau đây được thỏa mãn:
(i) M là hữu hạn trình bày;
(ii) m là lũy linh.
Khi đó các tính chất sau là tương đương:
(a) M là tự do;
(b) M là xạ ảnh;
(c) M là phẳng;
(d) đồng cấu chính tắc $m \otimes_A M \to M$ là đơn ánh;
(e) Tor_1^A(A/m, M) = 0.

Các kéo theo (a) $\Rightarrow$ (b) $\Rightarrow$ (c) $\Rightarrow$ (d) là ngay lập tức. Vì A/m là một trường, $(A/m) \otimes_A M$ là một $(A/m)$-môđun tự do và Mệnh đề 5 cho thấy rằng (d) kéo theo (a).

Cuối cùng, ta biết rằng Tor_1^A(A, M) = 0 và từ dãy khớp $0 \to m \to A \to A/m \to 0$ ta suy ra do đó dãy khớp

$$
0 \to \mathrm{Tor}_1^A(A/m, M) \to m \otimes_A M \to M;
$$

điều này chứng minh rằng Tor$_1^A(A/m, M)$ đẳng cấu với hạt nhân của đồng cấu chính tắc $m \otimes_A M \to M$; do đó sự tương đương của (d) và (e). \*

Có thể chứng minh rằng, với mọi vành $A$ có căn Jacobson $m$ sao cho $A/m$ là một trường, *mọi* A-môđun xạ ảnh đều tự do (Bài tập 3).

#### Mệnh đề 6 {#ac-ii-s3-prop-6 .statement}

*Cho $A$ là một vành không nhất thiết giao hoán và $m$ là căn Jacobson của nó; giả sử rằng $A/m$ là một trường. Cho $M$ và $N$ là hai A-môđun tự do sinh hữu hạn và $u: M \to N$ là một đồng cấu. Các tính chất sau là tương đương*:

(a) $u$ là một đẳng cấu của $M$ lên một nhân tử trực tiếp của $N$;
(b) $1 \otimes u: (A/m) \otimes_A M \to (A/m) \otimes_A N$ là đơn ánh;
(c) $u$ là đơn ánh và $\operatorname{Coker}(u)$ là một A-môđun tự do;
(d) đồng cấu chuyển vị ${}^t u: N^* \to M^*$ là toàn ánh.

Ta biết (*đại số*, chương II, § 1, no. 11, Mệnh đề 21) rằng, nếu $N/u(M)$ là tự do, thì $u(M)$ là một nhân tử trực tiếp của $N$, do đó (c) suy ra (a); ngược lại, (a) suy ra rằng $\operatorname{Coker}(u)$, đẳng cấu với một phần bù của $u(M)$ trong $N$, là một $A$-môđun xạ ảnh sinh hữu hạn và *a fortiori* có một hệ sinh hữu hạn (chương I, § 2, no. 8, Bổ đề 8); do đó môđun này là tự do theo Hệ quả 2 của Mệnh đề 5 và (a) suy ra (c). Mặt khác, (a) hiển nhiên suy ra (b). Để đơn giản, ta viết $M' = (A/m) \otimes_A M$, $N' = (A/m) \otimes_A N$; vì $M$ và $N$ sinh hữu hạn, các đối ngẫu ${M'}^*$ và ${N'}^*$ của các $(A/m)$-môđun $M'$ và $N'$ được đồng nhất một cách chính tắc với $M^* \otimes_A (A/m)$ và $N^* \otimes_A (A/m)$ và ${}^t(1 \otimes u)$ với $({}^t u) \otimes 1$ (*đại số*, chương II, § 5, no. 4, Mệnh đề 8); vì $M'$ và $N'$ là các không gian vectơ trên trường $A/m$, giả thiết rằng $1 \otimes u$ đơn ánh suy ra rằng ${}^t(1 \otimes u)$ toàn ánh (*đại số*, chương 11, § 7, no. 5, Mệnh đề 10); Hệ quả 1 của Mệnh đề 4 khi đó cho thấy rằng ${}^t u$ toàn ánh và do đó ta đã chứng minh rằng (b) suy ra (d). Cuối cùng ta chứng minh rằng (d) suy ra (a). Giả sử ${}^t u$ toàn ánh; vì $M^*$ tự do, tồn tại một đồng cấu $f$ từ $M^*$ vào $N^*$ sao cho $1_{M^*} = {}^t u \circ f$ (*đại số*, chương II, § 1, no. 11, Mệnh đề 21); vì $M$ và $N$ tự do và sinh hữu hạn, tồn tại một đồng cấu $g$ từ $N$ vào $M$ sao cho $f = {}^t g$; do đó ${}^t 1_M = 1_{M^*} = {}^t u \circ {}^t g = {}^t(g \circ u)$, do đó $1_M = g \circ u$; điều này chứng minh rằng $u$ là một đẳng cấu của $M$ lên một môđun con là một nhân tử trực tiếp của $N$ (*đại số*, chương 11, § 1, no. 9, Hệ quả 2 của Mệnh đề 15).

#### Hệ quả {#ac-ii-s3-n2-cor-1 .statement}

*Dưới các giả thiết của Mệnh đề 6, các tính chất sau là tương đương*:

(a) $u$ là một đẳng cấu của $M$ lên $N$;
(b) $M$ và $N$ có cùng hạng (*đại số*, chương II, § 7, no. 2) và $u$ toàn ánh;
(c) $1 \otimes u: M/mM \to N/mN$ là song ánh.

Các mệnh đề đã chứng minh ở trên trong no. này thường được áp dụng khi $A$ là một *vành địa phương* và $m$ là *iđêan cực đại* của nó. Khi đó Hệ quả 2 của Mệnh đề 5 được hoàn tất bởi

#### Mệnh đề 7 {#ac-ii-s3-prop-7 .statement}

Cho $A$ là một vành địa phương giảm, $m$ là iđêan cực đại của nó, $(p_i)_{i \in I}$ là họ các iđêan nguyên tố cực tiểu của $A$, $K_i$ là trường phân thức của $A/p_i$ và $M$ là một môđun $A$ sinh hữu hạn. Để $M$ tự do, điều kiện cần và đủ là

$$(1)\qquad [(A/m) \otimes_A M : (A/m)] = [K, \otimes_A M : K]\qquad \text{với mọi } i \in I.$$

Nếu M tự do, rõ ràng hai vế của (1) đều bằng hạng của M với mọi $i \in I$. Giả sử bây giờ điều kiện được thỏa mãn và ký hiệu $n$ là giá trị chung của hai vế của (1); theo Hệ quả 2 của Mệnh đề 4, M có một hệ gồm $n$ phần tử sinh $x_j$ ($1 \leq j \leq n$). Trước hết giả sử rằng $A$ là một *miền nguyên*, trong trường hợp đó $p_i = 0$ với mọi $i \in I$. Các phần tử $1 \otimes x_j$ ($1 \leq j \leq n$) sinh không gian vectơ $K \otimes M$ trên trường phân thức K của $A$; nhưng theo giả thiết không gian này có chiều $n$ trên K, các phần tử $1 \otimes x_j$ độc lập tuyến tính trên K. Suy ra (*Đại số*, Chương II, § 1, no. 13, *Nhận xét* 1) rằng các $x_j$ độc lập tuyến tính trên $A$ và do đó tạo thành một cơ sở của M.

Chuyển sang trường hợp tổng quát, tồn tại một đồng cấu toàn ánh $v$ từ $L = A''$ lên M. Xét biểu đồ giao hoán

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

(tương ứng $\psi_i : M \to (A/p_i) \otimes M$) là ánh xạ chính tắc, và $v'$ là tích của các $1_{A/p_i} @ v_e$. Khi đó $(A/p)/(m/p_i) \otimes_{A/p_i} ((A/p_i) \otimes_A M) = (A/m) \otimes_A M$ và, vì $A/p_i$ là một miền nguyên địa phương, suy ra từ phần đầu của lập luận rằng mỗi một trong các $1_{A/p_i} \otimes v$ là một đẳng cấu; do đó $v'$ cũng là một đẳng cấu. Mặt khác, vì $A$ là giảm, $\bigcap_i p_i = (0)$ ($\S 2$, no. 6, Mệnh đề 13), do đó $\bigcap_i (p_i L) = 0$ vì $L$ là tự do (*Đại số*, Chương II, $\S 3$, no. 7, *Nhận xét*); vì $p_i L$ là hạt nhân của $\phi_i$, điều này chứng tỏ rằng $u$ là đơn ánh. Suy ra rằng $v' \circ u = u' \circ v$ là đơn ánh, do đó $v$ là đơn ánh và, vì $v$ là toàn ánh theo định nghĩa, điều này chứng tỏ rằng $M$ là tự do.

### 3. CHUYỂN TỪ ĐỊA PHƯƠNG SANG TOÀN CỤC

#### Mệnh đề 8 {#ac-ii-s3-prop-8 .statement}

*Cho $A$ là một vành, $m$ là một iđêan cực đại của $A$ và $M$ là một $A$-môđun. Nếu tồn tại một iđêan $a$ của $A$ sao cho $m$ là iđêan cực đại duy nhất của $A$ chứa $a$ và $aM = 0$, thì đồng cấu chính tắc $M \to M$, là song ánh.*

$A/a$ khi đó là một vành địa phương với iđêan cực đại $m/a$; $M$ có thể được xét như một $(A/a)$-môđun; với mọi $s \in A - m$ ảnh chính tắc của $s$ trong $A/a$ là khả nghịch, do đó phép vị tự $x \mapsto sx$ của $M$ là song ánh theo định nghĩa của $M$, như là nghiệm của một bài toán phổ quát ($\S 2$, no. 2); do đó mệnh đề.

Đặc biệt, nếu tồn tại $k \geqslant 0$ sao cho $m^k M = 0$, thì đồng cấu $M \to M_m$ là song ánh ($\S 1$, no. 1, Hệ quả của Mệnh đề 1).

#### Mệnh đề 9 {#ac-ii-s3-prop-9 .statement}

*Cho $A$ là một vành, $m$ là một iđêan cực đại của $A$, $M$ là một $A$-môđun và $k$ là một số nguyên $\geqslant 0$. Đồng cấu chính tắc $M \to M_m/m^k M_m$ là toàn ánh, có hạt nhân $m^k M$ và xác định một đẳng cấu từ $M/m^k M$ lên $M_m/m^k M_m$.*

Vì trường hợp $k = 0$ là tầm thường, giả sử rằng $k \geqslant 1$. Suy ra từ Mệnh đề 8 rằng đồng cấu chính tắc $M/m^k M \to (M/m^k M)_m$ là song ánh. Mặt khác $(M/m^k M)_m$ được đồng nhất một cách chính tắc với $M_m/(m^k M)_m$ (\$2, no. 4, Định lý 1) và do đó $(m^k M)_m = m^k M_m$ (\$2, no. 7, Hệ quả của Mệnh đề 18), do đó có một đẳng cấu từ $M/m^k M$ lên $M_m/m^k M_m$ ánh xạ lớp của một phần tử $x \in M$ thành lớp của $x/1$.

#### Hệ quả {#ac-ii-s3-n3-cor-1 .statement}

*Cho $A$ là một vành, $m_1, m_2, \ldots, m_n$ là các iđêan cực đại phân biệt của $A$, $M$ là một $A$-môđun và $k_1, k_2, \ldots, k_n$ là các số nguyên $\geqslant 0$. Đồng cấu chính tắc từ $M$ đến $\prod^n M_m/m_{i_1}^{k_1} M_m$ là toàn ánh và hạt nhân của nó là $\left( \bigcap^n m_{i_1}^{k_1} \right) M$.*

Điều này suy ra dễ dàng từ Mệnh đề 9 và $\S 1$, no. 2, Mệnh đề 6, do các $m_{i_1}^{k_1}$ nguyên tố cùng nhau từng đôi một ($\S 1$, no. 2, Mệnh đề 3).

*Trong phần còn lại của no. này, $A$ sẽ ký hiệu một vành và $\Omega(A)$ (hoặc $\Omega$) là tập hợp các iđêan cực đại của $A$.*

#### Mệnh đề 10 {#ac-ii-s3-prop-10 .statement}

*A-môđun* $\bigoplus_{m \in \Omega} \mathbf{A}_m$, *tổng trực tiếp của các* $\mathbf{A}_m$ *với* $m \in \Omega$, *là phẳng trung thành*.

Mỗi $\mathbf{A}_m$ là một A-môđun phẳng (\$2, no. 4, Định lý 1), do đó $E = \bigoplus_{m \in \Omega} \mathbf{A}_m$ là phẳng (Chương I, § 2, no. 3, Mệnh đề 2). Hơn nữa, với mọi iđêan cực đại $m$ của $A$, $mA_m$ là iđêan cực đại duy nhất của $\mathbf{A}_m$, do đó $mA_m \neq A_m$, từ đó suy ra $mE \neq E$ và do đó $E$ là phẳng trung thành (Chương I, § 3, no. 1, Mệnh đề 1 (d)).

#### Định lý 1 {#ac-ii-s3-thm-1 .statement}

*Cho* $M, N$ *là hai A-môđun, $u : M \to N$ là một đồng cấu A và, với mọi* $m \in \Omega$, *cho* $u_m : M, \to N_m$ *là* $A_m$-*đồng cấu tương ứng* (\$2, no. 2, Nhận xét 5). *Để* $u$ *đơn ánh (tương ứng toàn ánh, song ánh, không), điều kiện cần và đủ là, với mọi* $m \in \Omega$, $u_m$ *đơn ánh (tương ứng toàn ánh, song ánh, không)*.

Nói rằng, với mọi $m \in \Omega$, $u_m$ đơn ánh (tương ứng toàn ánh, song ánh, không) tương đương với nói rằng đồng cấu $\bigoplus_m u_m : \bigoplus M, \to \bigoplus N$, có cùng tính chất. Nhưng $\bigoplus_m M_m = M \otimes_A E, \bigoplus_m N_m = N \otimes_A E$ và $\bigoplus_m u_m = u \otimes 1$, trong đó $E = \bigoplus_m \mathbf{A}_m$; vì $E$ là phẳng trung thành (Mệnh đề 10), định lý suy ra từ Chương I, § 3, no. 1, Mệnh đề 1 (c) và Mệnh đề 2.

#### Hệ quả 1 {#ac-ii-s3-thm-1-cor-1 .statement}

*Cho* $M$ *là một A-môđun, N là một môđun con của* $M$ *và* $x$ *là một phần tử của* $M$. *Để* $x \in N$, *điều kiện cần và đủ là, với mọi* $m \in R$, *ảnh chính tắc của* $x$ *trong* $M$, *thuộc* $N$.

Cho $\bar{x}$ là lớp của $x$ trong $M/N$; nói rằng $x \in N$ có nghĩa là ánh xạ A-tuyến tính $u : a \mapsto a\bar{x}$ từ $A$ vào $M/N$ là không. Bây giờ, $(M/N)_m$ được đồng nhất với $M_m/N_m$ (\$2, no. 4, Định lý 1) và $u_m : A_m \to M_m/N_m$ với ánh xạ $A \mapsto \lambda \bar{x}_m$, trong đó $\bar{x}_m$ là lớp mod. $N$, của ảnh chính tắc của $x$ trong $M$. Vì quan hệ $u = 0$ tương đương với $u_m = 0$ với mọi $m$ theo Định lý 1, điều này chứng minh hệ quả.

#### Hệ quả 2 {#ac-ii-s3-thm-1-cor-2 .statement}

*Cho* $M$ *là một A-môđun và, với mọi* $m \in \Omega$, *cho* $f_m$ *là ánh xạ chính tắc* $M \to M_m$. *Đồng cấu* $x \mapsto (f_m(x))$ *của* $M$ *vào* $\prod_{m \in \Omega} M_m$ *là đơn ánh*.

Áp dụng Hệ quả 1 trong trường hợp $N = 0$, ta thấy rằng quan hệ $x = 0$ tương đương với $f_m(x) = 0$ với mọi $m \in \Omega$.

#### Hệ quả 3 {#ac-ii-s3-thm-1-cor-3 .statement}

(i) *Cho* $b$ *là một iđêan của* $A$ *và* $a$ *là một phần tử của* $A$. *Đối với* $a \in b$, *điều kiện cần và đủ là, với mọi* $m \in \Omega$, *ảnh chính tắc của* $a$ *trong* $A_m$ *thuộc* $bA_m$.

(ii) Đặc biệt, cho b và c là hai phần tử của A. Để c là một bội của b, điều kiện cần và đủ là, với mọi $m \in \Omega$, ảnh chính tắc của c trong A là một bội của ảnh của b.

Vì $bA_m = b_m$ (\S 2, no. 7, Hệ quả của Mệnh đề 18), (i) là một trường hợp đặc biệt của Hệ quả 1; (ii) suy ra từ (i) áp dụng cho iđêan $Ab$.

#### Hệ quả 4 {#ac-ii-s3-thm-1-cor-4 .statement}

Cho A là một miền nguyên, K là trường phân thức của nó và M là một A-môđun không xoắn sao cho M được đồng nhất một cách chính tắc với một môđun con-A của $K \otimes_A M$. Khi đó, với mọi $m \in \Omega$, $M_m$ được đồng nhất một cách chính tắc với một môđun con-A của $K \otimes_A M$ và $M = \bigcap_{m \in \Omega} M_m$.

Vì M được đồng nhất với một môđun con của $K \otimes_A M$, M, được đồng nhất với một môđun con-&-module của $(K \otimes_A M)_m = K_m \otimes_A M$ (\S 2, no. 4, Định lý 1); vì $K_m = K$, ta thấy ngay rằng $M_m$ là không xoắn; hơn nữa, tính giao hoán của biểu đồ

$$
\begin{array}{ccc}
M & \longrightarrow & K \otimes_A M \\
\downarrow & & \uparrow \\
M_m & \longrightarrow & (K \otimes_A M)_m
\end{array}
$$

chứng minh rằng ánh xạ chính tắc $M \to M_m$ là đơn ánh. Hệ quả sau đó suy ra từ Hệ quả 1 áp dụng cho A-môđun $K \otimes_A M$ và môđun con M của nó.

Đặc biệt, với mọi miền nguyên A,

(2)
$$
A = \bigcap_{m \in \Omega} A_m.
$$

#### Hệ quả 5 {#ac-ii-s3-thm-1-cor-5 .statement}

Cho A là một vành. Mọi hệ sinh của A-môđun $A^n$ gồm n phần tử là một cơ sở của $A^n$.

Cho $(e_i)_{1 \leq i \leq n}$ là cơ sở chính tắc của $A''$, $(x_i)_{1 \leq i \leq n}$ là một hệ sinh của $A^n$ với n phần tử và $u : A^n \to A''$ là ánh xạ A-tuyến tính sao cho $u(e_i) = x_i$ với $1 \leq i \leq n$. Theo giả thiết $u$ là toàn ánh và cần chứng minh rằng $u$ là đơn ánh. Theo Định lý 1, điều này có thể ngay lập tức quy về trường hợp A là một vành địa phương; nếu $m$ là iđêan cực đại của A, khi đó các phần tử $1 \otimes x_i$ ($1 \leq i \leq n$) trong $(A/m)^n$ tạo thành một hệ sinh của $(A/m)$-môđun tự do $(A/m)^n$; vì $A/m$ là một trường, hệ này là một cơ sở của $(A/m)^n$; vì $A^n$ là một A-môđun tự do, ta suy ra từ Mệnh đề 5 rằng $(x_i)$ là một cơ sở của $A^n$.

#### Mệnh đề 11 {#ac-ii-s3-prop-11 .statement}

Cho M là một A-môđun, N là một A-môđun hữu hạn sinh và $u : M \to N$ là một đồng cấu. Để u toàn ánh, điều kiện cần và đủ là, với mọi $m \in S_2$, đồng cấu $M/mM \to N/mN$ dẫn xuất từ $u$ bằng cách lấy thương là toàn ánh.

Từ Định lý 1 suy ra rằng, để $u$ toàn ánh, điều kiện cần và đủ là $u_m : M_m \to N_m$ toàn ánh với mọi $m \in \Omega$. Vì A là một vành địa phương và $N_m$ là một $A_m$-môđun hữu hạn sinh, điều này tương đương với việc nói rằng đồng cấu $u'_m : M_m/mM_m \to N_m/mN_m$, nhận được bằng cách lấy thương, là toàn ánh (no. 2, Hệ quả 1 của Mệnh đề 4); nhưng $M_m/mM_m$ (resp. $N_m/mN_m$) được đồng nhất với $M/mM$ (resp. $N/mN$) (Proposition9), do đó có mệnh đề.

#### Mệnh đề 12 {#ac-ii-s3-prop-12 .statement}

*Cho E, F, G là ba A-môđun và $v : G \to F$, $u : E \to F$ là các đồng cấu. Giả sử E là hữu hạn trình bày. Để tồn tại một đồng cấu $w : E \to G$ sao cho u phân tích qua $E \xrightarrow{w} G \xrightarrow{v} F$, điều kiện cần và đủ là, với mọi $m \in S_2$, tồn tại một đồng cấu $w^m : E_m \to G$, sao cho $u_m : E_m \to F$, phân tích qua $E \xrightarrow{w^m} G_m \xrightarrow{v_m} F$,*

Sự tồn tại của $w$ thỏa mãn mệnh đề trên tương đương với tính chất sau: $u$ thuộc ảnh P của ánh xạ

$$
r = \operatorname{Hom}(1_E, v) : \operatorname{Hom}_A(E, G) \to \operatorname{Hom}_A(E, F).
$$

Bây giờ, $(\operatorname{Hom}_A(E, F))_m$ (resp. $(\operatorname{Hom}_A(E, G))_m$) được đồng nhất một cách chính tắc với $\operatorname{Hom}_{A_m}(E_m, F_m)$ (resp. $\operatorname{Hom}_{A_m}(E_m, G_m)$) (\S 2, no. 7, Proposition 19 (i)), ảnh chính tắc của $u$ trong $(\operatorname{Hom}_A(E, F))_m$ được đồng nhất với $u_m$, $r_m$ được đồng nhất với $\operatorname{Hom}_{A_m}(1_{E_m}, v)$ và $P_m$ với ảnh của $r_m$. Mệnh đề sau đó suy ra từ Hệ quả 1 của Định lý 1 áp dụng cho $\operatorname{Hom}_A(E, F)$ và môđun con P của nó.

#### Hệ quả 1 {#ac-ii-s3-prop-12-cor-1 .statement}

*Cho M là một A-môđun và N là một môđun con của M sao cho M/N là hữu hạn trình bày. Để N là một nhân tử trực tiếp của M, điều kiện cần và đủ là, với mọi $m \in S_2$, N là một nhân tử trực tiếp của M.*

Nói rằng N là một nhân tử trực tiếp của M có nghĩa là đồng cấu đồng nhất trên M/N phân tích thành $M/N \xrightarrow{w} M \xrightarrow{\phi} M/N$ trong đó $\phi$ là đồng cấu chính tắc và $w$ là một đồng cấu (*Algebra*, chương II, § 1, no. 9, Mệnh đề 14); vì $(M/N)_m = M_m/N_m$ và $\phi_m$ là đồng cấu chính tắc $M_m \to M_m/N_m$, hệ quả suy ra dễ dàng từ Mệnh đề 12.

#### Hệ quả 2 {#ac-ii-s3-prop-12-cor-2 .statement}

*Cho M là một A-môđun tự do sinh hữu hạn và N là một môđun con của M là một A-môđun tự do sinh hữu hạn. Để N là một nhân tử trực tiếp của M, điều kiện cần và đủ là, với mọi $m \in \Omega$, $mN = N \cap (mM)$.*

Theo định nghĩa M/N là hữu hạn trình bày; mặt khác, N và M là các $A_n$-môđun tự do sinh hữu hạn. Để $N$ là một nhân tử trực tiếp của $M$, điều kiện cần và đủ là ánh xạ chính tắc $N_m / mN_m \to M_m / mM_m$ là đơn ánh (no. 2, Mệnh đề 6); điều này cũng chính là nói rằng ánh xạ chính tắc $N / mN \to M / mM$ phải là đơn ánh (Mệnh đề 9), và vì hạt nhân của nó là $(N \cap mM) / mN$, điều này chứng minh hệ quả.

Mệnh đề 12 (tương ứng Hệ quả 1 của nó) sẽ được áp dụng đặc biệt khi $A$ là Noether và $E$ (tương ứng $M/N$) là một *A-môđun sinh hữu hạn* (Chương I, § 2, no. 8, Bổ đề 8).

### 4. ĐỊA PHƯƠNG HÓA TÍNH PHẲNG

#### Mệnh đề 13 {#ac-ii-s3-prop-13 .statement}

*Cho $S$ là một tập con nhân của một vành $A$ và $M$ là một $A$-môđun. Nếu $M$ là phẳng (tương ứng phẳng trung thành), $S^{-1}M$ là một $S^{-1}A$-môđun phẳng (tương ứng phẳng trung thành) và một $A$-môđun phẳng.*

Vì $S^{-1}M = M \otimes_A S^{-1}A$, mệnh đề đầu tiên suy ra từ Chương I, § 2, no. 7, Hệ quả 2 của Mệnh đề 8 (tương ứng Chương I, § 3, no. 3, Mệnh đề 5); hơn nữa, $S^{-1}A$ là một $A$-môđun phẳng ($§ 2$, no. 4, Định lý 1); do đó nếu $M$ là một $A$-môđun phẳng, thì $S^{-1}M$ cũng vậy nhờ Chương I, § 2, no. 7, Hệ quả 3 của Mệnh đề 8.

#### Nhận xét {#ac-ii-s3-n4-rem-1 .statement}

Nếu $N$ là một $S^{-1}A$-môđun, $S^{-1}N$ được đồng nhất với $N$ và điều này do đó *tương đương* với việc nói rằng $N$ là một $S^{-1}A$-môđun phẳng hoặc một $A$-môđun phẳng.

#### Mệnh đề 14 {#ac-ii-s3-prop-14 .statement}

*Cho $A$ là một vành, $B$ là một $A$-đại số giao hoán và $T$ là một tập con nhân của $B$. Nếu $N$ là một $B$-môđun phẳng như một $A$-môđun, $T^{-1}N$ là một $A$-môđun phẳng.*

$T^{-1}N = T^{-1}B \otimes_B N$; khi đó mệnh đề suy ra từ Chương I, § 2, no. 7, Mệnh đề 8, áp dụng với $A$ được thay bởi $B$, $B$ bởi $A$, $E$ bởi $T^{-1}B$ và $F$ bởi $N$.

#### Mệnh đề 15 {#ac-ii-s3-prop-15 .statement}

*Cho $A, B$ là hai vành, $\phi : A \to B$ là một đồng cấu và $N$ là một B-môđun. Các tính chất sau là tương đương:
(a) $N$ là một A-môđun phẳng.
(b) *Với mọi iđêan cực đại $n$ của $B$, $N_n$ là một A-môđun phẳng.*
(c) *Với mọi iđêan cực đại $n$ của $B$, nếu ta viết $m = \phi(n)$, thì $N_n$ là một $A_m$-môđun phẳng.*

Với mọi $a \notin m$, phép vị tự của $N_n$ cảm sinh bởi $a$ là song ánh, do đó $N_n$ được đồng nhất một cách chính tắc với $(N_n)_m$ và tính tương đương của (b) và (c) suy ra từ

Nhận xét sau Mệnh đề 13; sự kiện (a) kéo theo (b) là một trường hợp đặc biệt của Mệnh đề 14. Còn lại phải chứng minh rằng (b) kéo theo (a), nghĩa là, nếu (b) đúng, với mọi đồng cấu đơn ánh A-môđun $u : M \to M'$, đồng cấu $v = 1 @ u : N \otimes_A M \to N @^* M'$ là đơn ánh. Bây giờ, $v$ cũng là một đồng cấu B-môđun và, để nó là đơn ánh, điều kiện cần và đủ là $v,, : (N \otimes_A M),, \to (N \otimes_A M'),,$ cũng là như vậy với mọi iđêan cực đại $n$ của $B$ (no. 3, Định lý 1). Vì
$$
(N \otimes_A M)_n = B_n \otimes_B (N @_A M) = N_n \otimes_A M,
$$
$v_n$ chính là đồng cấu $1 \otimes u : N_n \otimes_A M \to N_n \otimes_A M'$, là đơn ánh vì $N_n$ là một A-môđun phẳng theo giả thiết.

#### Hệ quả {#ac-ii-s3-n4-cor-1 .statement}

*Để một A-môđun M là phẳng (tương ứng, phẳng trung thành), điều kiện cần và đủ là, với mọi iđêan cực đại $m$ của A, $M,$ là một $A_m$-môđun phẳng (tương ứng, phẳng trung thành).*

Tính cần thiết của các điều kiện suy ra từ Mệnh đề 13. Ngược lại, nếu $M,$ là một $A_m$-môđun phẳng với mọi iđêan cực đại $m$ của A, thì $M$ là một A-môđun phẳng theo Mệnh đề 15 áp dụng vào trường hợp $\phi$ là đồng nhất. Cuối cùng, nếu $M,$ là một $A_m$-môđun phẳng trung thành với mọi $m$, thì $mM_m = mA_mM_m \neq M,$ do đó $mM \neq M$ với mọi $m$ (no. 3, Mệnh đề 9), điều này chứng minh rằng $M$ là một A-môđun phẳng trung thành (Chương I, § 3, no. 1, Mệnh đề 1 (d)).

### 5. VÀNH NỬA ĐỊA PHƯƠNG

#### Mệnh đề 16 {#ac-ii-s3-prop-16 .statement}

*Cho A là một vành. Các tính chất sau là tương đương:
(a) tập hợp các iđêan cực đại của A là hữu hạn;
(b) thương của A theo căn Jacobson của nó là hợp thành trực tiếp của một số hữu hạn các trường.*

Giả sử rằng thương của A theo căn Jacobson của nó $\mathfrak{R}$ là một hợp thành trực tiếp của một số hữu hạn các trường. Khi đó $A/\mathfrak{R}$ chỉ có một số hữu hạn các iđêan và *a fortiori* chỉ có một số hữu hạn các iđêan cực đại. Vì mọi iđêan cực đại chứa $\mathfrak{R}$ (*Algebra*, Chương VIII, § 6, no. 2, Định nghĩa 2), các iđêan cực đại của A là các ảnh nghịch đảo của các iđêan cực đại của $A/\mathfrak{R}$ qua đồng cấu chính tắc $A \to A/\mathfrak{R}$; do đó số lượng của chúng là hữu hạn.

Ngược lại, giả sử rằng A chỉ có một số hữu hạn các iđêan cực đại phân biệt $m_1, \ldots, m_n$. Các $A/m_i$ là các trường và suy ra từ § 1, no. 2, Mệnh đề 5 rằng ánh xạ chính tắc $A \to \prod_{i=1}^n A/m_i$ là toàn ánh; vì hạt nhân của nó $\bigcap_{i=1}^n m_i$ là căn Jacobson $\mathfrak{R}$ (*Algebra*, Chương VIII, § 6, no. 2, Định nghĩa 2), $A/\mathfrak{R}$ đẳng cấu với $\prod_{i=1}^n A/m_i$.

#### Định nghĩa 4 {#ac-ii-s3-def-4 .statement}

Một vành được gọi là nửa địa phương nếu nó thỏa mãn các điều kiện tương đương (a), (b) của Mệnh đề 16.

#### Ví dụ {#ac-ii-s3-n5-exa-1 .statement}

Mọi vành địa phương đều là nửa địa phương. Mọi thương của một vành nửa địa phương đều là nửa địa phương. Mọi tích hữu hạn của các vành nửa địa phương đều là nửa địa phương.

Nếu A là một vành nửa địa phương Noether và B là một A-đại số là một A-môđun sinh hữu hạn, thì B là nửa địa phương (Chương IV, § 2, no. 5, Hệ quả 3 của Mệnh đề 9).

Một ví dụ khác, khái quát phép dựng các vành địa phương $A_{\mathfrak{p}}$, được cung cấp bởi mệnh đề sau:

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
