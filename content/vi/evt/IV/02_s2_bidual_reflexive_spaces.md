---
book: evt
book_title: Topological Vector Spaces
chapter: IV
chapter_title: DUALITY IN TOPOLOGICAL VECTOR SPACES
section: 2
section_title: Bidual. Reflexive spaces
lang: vi
source: evt-i-v
book_pages: TVS IV.14-TVS IV.21, TVS IV.52-TVS IV.57
pdf_pages: 0196-0203, 0234-0239
extraction: ocr
subsections:
    - "no": 1
      title: Bidual
      page: 14
      pdf_page: 196
    - "no": 2
      title: Semi-reflexive spaces
      page: 15
      pdf_page: 197
    - "no": 3
      title: Reflexive spaces
      page: 16
      pdf_page: 198
    - "no": 4
      title: The case of normed spaces
      page: 17
      pdf_page: 199
    - "no": 5
      title: Montel spaces
      page: 18
      pdf_page: 200
statements: 30
exercises: 24
content_sha256: 72d0e59f5c18ed423491784c4b84436cb8fd841e26535f7ef6e736673d4234e5
translated_from: content/en/evt/IV/02_s2_bidual_reflexive_spaces.md
source_content_sha256: c8f008de2daf8653ce90dda0cbafdb04b9e1842cb6daff4312ae7ca854ca1ef6
translation_model: gpt-5.4-mini
translation_run: translate-vi-0edebf1c
glossary_version: 34
glossary_terms_sha256: a6a1cb5d5595cb91b545ac240344bd2aea8d8084475dd1dec45fe4cca79fef6f
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 2. ĐỐI NGẪU CẤP HAI. KHÔNG GIAN PHẢN XẠ

### 1. Đối ngẫu cấp hai

#### Định nghĩa 1 {#evt-iv-s2-def-1 .statement}

— *Cho $E$ là một không gian địa phương lồi và $E'_b$ là đối ngẫu mạnh của nó. Đối ngẫu của không gian địa phương lồi $E'_b$ được gọi là đối ngẫu cấp hai của $E$ và được ký hiệu bởi $E''$.*

Với mọi $x \in E$, ký hiệu $\tilde{x}$ là dạng tuyến tính $x' \mapsto \langle x, x' \rangle$ trên $E'$; nó liên tục đối với tôpô yếu $\sigma(E', E)$, do đó *a fortiori*, đối với tôpô mạnh trên $E'$; vì vậy $\tilde{x} \in E''$ với mọi $x \in E$. Ánh xạ $c_E : x \mapsto \tilde{x}$ từ $E$ vào $E''$ là một ánh xạ tuyến tính, được gọi là *chính tắc*.

#### Mệnh đề 1 {#evt-iv-s2-prop-1 .statement}

— *Hạt nhân của $c_E : E \to E''$ là bao đóng của 0 trong $E$. Nếu $E$ là Hausdorff, thì $c_E$ là đơn ánh.*

Theo phép dựng, hạt nhân của $c_E$ là giao của các hạt nhân của các dạng tuyến tính liên tục trên $E$, *tức là* bao đóng của $\{0\}$ trong $E$ (II, p. 24, cor. 1).

Khi $E$ là Hausdorff, ta đồng nhất $E$ với một không gian con của $E''$, bằng ánh xạ $c_E$.

ĐỐI NGẪU CẤP HAI. KHÔNG GIAN PHẢN XẠ

TVS IV.15

Tôpô mạnh trên $E''$ là $\mathcal{S}$-tôpô, trong đó $\mathcal{S}$ là họ của mọi tập con bị chặn mạnh của $E'$. Vì mọi tập con đều liên tục của $E'$ đều bị chặn mạnh (III, p. 22, prop. 9), tôpô ban đầu trên $E$ thô hơn tôpô thu được bằng cách lấy ảnh ngược qua $c_E$ của tôpô mạnh trên $E''$; nó có thể thô hơn một cách nghiêm ngặt (IV, p. 52, exerc. 1). Tuy nhiên:

#### Mệnh đề 2 {#evt-iv-s2-prop-2 .statement}

— Giả sử không gian $E$ là bornological hoặc barrelled. Tôpô ban đầu trên $E$ là ảnh ngược qua $c_E$ của tôpô mạnh trên $E''$.

Thật vậy, mọi tập con của $E'$ bị chặn mạnh đều đều liên tục (III, p. 22, prop. 10 và III, p. 24).

#### Mệnh đề 3 {#evt-iv-s2-prop-3 .statement}

— Cho $E$ là một không gian địa phương lồi Hausdorff. Để đối ngẫu mạnh $E'_b$ của $E$ là barrelled, điều kiện cần và đủ là mọi tập con của $E''$ bị chặn đối với $\sigma(E'', E')$, đều được chứa trong bao đóng, đối với $\sigma(E'', E')$, của một tập con bị chặn của $E$.

Các tập con đều liên tục của $E''$ là các tập con được chứa trong song đối ngẫu (đối với đối ngẫu giữa $E''$ và $E'$) của một tập con bị chặn của không gian con $E$ của $E''$. Bây giờ chỉ cần áp dụng định lý về song đối ngẫu (II, p. 45, cor. 3) và định nghĩa của một không gian barrelled (III, p. 24).

#### Nhận xét {#evt-iv-s2-n1-rem-1 .statement}

Nếu $B$ là một tập con bị chặn của $E$, thì bao đóng $\overline{B}$ của nó trong $E'^*$ được trang bị bởi $\sigma(E'^*, E')$ được chứa trong $E''$: vì, đối cực $U = B^\circ$ của $B$ trong $E'$ là một lân cận của 0 trong $E'_b$, và ta có $\overline{B} \subset U^\circ \subset E''$.

### 2. Không gian nửa phản xạ

#### Định nghĩa 2 {#evt-iv-s2-def-2 .statement}

— Cho $E$ là một không gian lồi địa phương. Ta nói rằng $E$ là nửa phản xạ nếu ánh xạ chính tắc $c_E$ từ $E$ vào $E''$ là song ánh.

Điều này suy ra rằng $E$ là Hausdorff, và rằng mọi dạng tuyến tính trên $E'$, liên tục đối với tôpô mạnh $\beta(E', E)$, đều có dạng $x' \mapsto \langle x, x' \rangle$ với $x \in E$, tức là liên tục đối với tôpô yếu $\sigma(E', E)$.

#### Định lý 1 {#evt-iv-s2-thm-1 .statement}

— Một không gian Hausdorff lồi địa phương là nửa phản xạ khi và chỉ khi mọi tập con bị chặn của $E$ đều tương đối compact đối với tôpô suy yếu $\sigma(E, E')$. Nếu $E$ nửa phản xạ, thì đối ngẫu mạnh $E'_b$ của $E$ là barrelled.

Khẳng định thứ hai suy ra từ mệnh đề 3 (IV, p. 15), và từ sự đồng nhất giữa các tập con bị chặn đối với tôpô ban đầu và đối với tôpô suy yếu của $E$ (III, p. 27, hệ quả 3).

Nói rằng $E$ nửa phản xạ có nghĩa là tôpô trên $E'_b$ tương thích với tính đối ngẫu giữa $E$ và $E'$, nói cách khác, theo định lý Mackey (IV, p. 2, định lý 1) thì tôpô trên $E'_b$ thô hơn $\tau(E', E)$ (và thực ra trùng với nó); theo định nghĩa (IV, p. 2), điều này có nghĩa là mọi tập con đóng, lồi và bị chặn của $E$ đều compact đối với $\sigma(E, E')$, và điều này tương đương với việc nói rằng mọi tập con bị chặn của E đều tương đối compact đối với $\sigma(E, E')$, vì bao lồi đóng của một tập con bị chặn của E vẫn bị chặn (III, p. 3, mệnh đề 1).

#### Hệ quả {#evt-iv-s2-n2-cor-1 .statement}

— *Cho E là một không gian lồi địa phương nửa phản xạ. Mọi không gian con vectơ đóng M của E đều nửa phản xạ; hơn nữa, tôpô mạnh trên $E'/M^\circ$ (được xem như đối ngẫu của M) là thương của tôpô mạnh trên E'.*

Cho B là một tập con bị chặn của M. Vì B bị chặn trong E, và tôpô suy yếu $\sigma(M, M')$ trên M được cảm sinh bởi $\sigma(E, E')$ (IV, p. 10, mệnh đề 11), nên bao đóng của B trong M được trang bị $\sigma(M, M')$ là compact. Do đó, theo định lý 1, M nửa phản xạ. Khẳng định cuối cùng của hệ quả suy ra từ mệnh đề 10 của IV, p. 9, áp dụng cho tập $\mathcal{S}$ gồm tất cả các tập con đóng, lồi và bị chặn của E.

#### Nhận xét 1 {#evt-iv-s2-n2-rem-1 .statement}

Giả sử E nửa phản xạ. Mọi tập con của E lồi, đóng và bị chặn đối với tôpô ban đầu đều compact đối với tôpô $\sigma(E, E')$ (IV, p. 1, mệnh đề 1). *Mặt khác, mặt cầu đơn vị (với phương trình $\|x\| = 1$) của một không gian Hilbert thực vô hạn chiều E là đóng và bị chặn đối với tôpô ban đầu, nhưng không đóng đối với tôpô suy yếu, ngay cả khi E nửa phản xạ. \*
2) Theo nhận xét 3 của IV, p. 5, ta có thể phát biểu lại định lý 1 như sau: *không gian Hausdorff E là nửa phản xạ khi và chỉ khi nó quasi-đầy đủ đối với tôpô suy yếu của nó.* Nếu nó nửa phản xạ, thì nó *quasi-đầy đủ đối với tôpô ban đầu của nó* (IV, p. 5, Nhận xét 2).
3) Dưới các giả thiết của hệ quả trên, không gian E/M không nhất thiết là nửa phản xạ (IV, p. 63, exerc. 10).

### 3. Không gian phản xạ

#### Định nghĩa 3 {#evt-iv-s2-def-3 .statement}

— *Một không gian lồi địa phương E được gọi là phản xạ nếu ánh xạ chính tắc $c_E$ từ E vào $E''$ là một đẳng cấu không gian vectơ tôpô từ E lên đối ngẫu mạnh của $E'_b$. \*

Đặc biệt, một không gian phản xạ là nửa phản xạ, do đó Hausdorff.

#### Mệnh đề 4 {#evt-iv-s2-prop-4 .statement}

— *Đối ngẫu mạnh của một không gian phản xạ là phản xạ.*

Điều này suy ra ngay từ định nghĩa 3.

#### Định lý 2 {#evt-iv-s2-thm-2 .statement}

— *Để một không gian Hausdorff lồi địa phương E là phản xạ, điều cần và đủ là E là barrelled và mọi tập con bị chặn của E đều tương đối compact đối với tôpô suy yếu $\sigma(E, E')$.*

Theo định lý 1 (IV, p. 15), điều này cũng có nghĩa là E *phản xạ khi và chỉ khi nó nửa phản xạ và barrelled*.

Nếu E phản xạ, $E'_b$ phản xạ (mệnh đề 4) và do đó E là barrelled (IV, p. 15, định lý 1). Ngược lại, nếu E nửa phản xạ và barrelled, $c_E$ là một song ánh và là song liên tục theo IV, p. 15, mệnh đề 2, nên E phản xạ.

#### Nhận xét 1 {#evt-iv-s2-n3-rem-1 .statement}

Cho E là một không gian Hilbert thực vô hạn chiều. Gọi F là không gian E được trang bị tôpô suy yếu. Các không gian E và F có cùng đối ngẫu E', và E là một không gian Banach phản xạ (V, p. 17). Do đó, F là *nửa phản xạ*.

Tuy nhiên, tôpô mạnh và tôpô suy yếu trên E là khác nhau, nên F *không phản xạ*.

#### Nhận xét 2 {#evt-iv-s2-n3-rem-2 .statement}

Cho E là một không gian phản xạ và M là một không gian con vectơ đóng của E. Có thể xảy ra rằng cả M lẫn E/M đều không là các không gian phản xạ (IV, p. 63, exerc. 10). \* Đối với trường hợp các không gian định chuẩn, xem mệnh đề 7 của IV, p. 17. \*

### 4. Trường hợp các không gian định chuẩn

Cho E là một không gian định chuẩn. Tôpô mạnh trên đối ngẫu E' của E được xác định bởi chuẩn

(1)
$$
\|x'\| = \sup_{x \in E, \|x\| \leq 1} |\langle x, x' \rangle|,
$$
và đối ngẫu mạnh của E là một không gian Banach (III, p. 24, hệ quả 2). Khi đó, đối ngẫu kép E'' của E cũng là một không gian Banach, với chuẩn được xác định bởi

(2)
$$
\|x''\| = \sup_{x' \in E', \|x'\| \leq 1} |\langle x', x'' \rangle|.
$$

Theo mệnh đề 8, (i) của IV, p. 7, ánh xạ tuyến tính chính tắc $c_E : E \to E''$ là một đẳng cự. Từ nay về sau, *ta sẽ đồng nhất E với một không gian con định chuẩn của đối ngẫu kép E'' của nó*.

#### Mệnh đề 5 {#evt-iv-s2-prop-5 .statement}

— *Cho E là một không gian có chuẩn, E' là đối ngẫu của nó và E'' là đối ngẫu kép của nó. Quả cầu đơn vị (đóng) trong E'' là bao đóng của quả cầu đơn vị B trong E đối với tôpô yếu $\sigma(E'', E')$.*

Theo các công thức (1) và (2), quả cầu đơn vị trong E'' là song cực $B^{\circ \circ}$ của B. Mệnh đề 5 sau đó suy ra từ định lý song cực (II, p. 45, hệ quả 3).

#### Nhận xét {#evt-iv-s2-n4-rem-1 .statement}

— Một không gian Banach E là đóng trong đối ngẫu kép E'' đối với tôpô mạnh, nhưng trù mật đối với tôpô yếu (mệnh đề 5).

Để một không gian có chuẩn E là *phản xạ*, điều kiện cần và đủ là nó *bán phản xạ*; vì, tôpô ban đầu của E luôn được cảm sinh bởi tôpô mạnh của E''. Định lý 1 (IV, p. 15) suy ra kết quả sau :

#### Mệnh đề 6 {#evt-iv-s2-prop-6 .statement}

— *Để một không gian có chuẩn E là phản xạ, điều kiện cần và đủ là quả cầu đơn vị trong E là compact đối với tôpô suy yếu $\sigma(E, E')$.*

Ta nhận thấy rằng một không gian có chuẩn phản xạ là đầy đủ do đó là một không gian Banach, và rằng đối ngẫu của nó là một không gian Banach phản xạ theo mệnh đề 4 của IV, p. 16.

#### Mệnh đề 7 {#evt-iv-s2-prop-7 .statement}

— *Cho E là một không gian Banach phản xạ và M là một không gian vectơ con đóng của E. Khi đó M và E/M là các không gian Banach phản xạ.*

Cho E' là đối ngẫu của E và $M^\circ$ là phần trực giao của M trong E'. Xét như một không gian có chuẩn, ta có thể đồng nhất không gian $E'/M^\circ$ với đối ngẫu $M'$ của M (IV, p. 9, mệnh đề 10). Vì M bán phản xạ (IV, p. 16, hệ quả), nên M phản xạ, do đó $E'/M^\circ$ cũng phản xạ; tương tự $M^\circ$ phản xạ, cũng như đối ngẫu của nó $E/M^{\circ \circ} = E/M$.

#### Ví dụ {#evt-iv-s2-n4-exa-1 .statement}

— 1) Cho $\ell^\infty(\mathbf{N})$ ký hiệu không gian Banach của các dãy bị chặn $x = (x_n)_{n \in \mathbf{N}}$ gồm các số vô hướng, với chuẩn

(3) $$
\| \mathbf{x} \| = \sup_{n \in \mathbf{N}} |x_n| \quad (\text{I, p. 4}) .
$$

Cho $c_0(\mathbf{N})$ là không gian vectơ con đóng của $\ell^\infty(\mathbf{N})$ gồm các dãy tiến tới 0. Cuối cùng, cho $\ell^1(\mathbf{N})$ là không gian vectơ của các dãy khả tổng, được trang bị chuẩn

(4) $$
\| \mathbf{x} \|_1 = \sum_{n \in \mathbf{N}} |x_n| .
$$

Ta có thể chứng minh (IV, p. 47, bài tập 1) rằng đối ngẫu của $c_0(\mathbf{N})$ có thể được đồng nhất với $\ell^1(\mathbf{N})$ sao cho ta có

(5) $$
\langle \mathbf{x}, \mathbf{x}' \rangle = \sum_{n \in \mathbf{N}} x_n x'_n
$$

với mọi $\mathbf{x} \in c_0(\mathbf{N})$ và $\mathbf{x}' \in \ell^1(\mathbf{N})$. Tương tự, đối ngẫu của $\ell^1(\mathbf{N})$ có thể được đồng nhất với $\ell^\infty(\mathbf{N})$ sao cho ta có quan hệ (5) với mọi $\mathbf{x} \in \ell^1(\mathbf{N})$ và mọi $\mathbf{x}' \in \ell^\infty(\mathbf{N})$. Do đó $\ell^\infty(\mathbf{N})$ là đối ngẫu kép của $c_0(\mathbf{N})$, và không gian này không phản xạ.

* 2) Mọi không gian Hilbert đều là một không gian Banach phản xạ (V, p. 17).
* 3) Cho X là một không gian tôpô Hausdorff và $\mu$ là một độ đo phức trên X. Với mọi số thực $p > 1$, không gian Banach $L^p(X, \mu)$ là phản xạ, và đối ngẫu của nó có thể được đồng nhất với $L^q(X, \mu)$ với $p^{-1} + q^{-1} = 1$ (INT, V, ấn bản thứ hai, § 5, No. 8 và IX, § 1, No. 10).

### 5. Không gian Montel

#### Định nghĩa 4 {#evt-iv-s2-def-4 .statement}

*Một không gian lồi địa phương Hausdorff và barreled mà mọi tập con bị chặn đều tương đối compact được gọi là một không gian Montel.*

#### Ví dụ 1 {#evt-iv-s2-n5-exa-1 .statement}

Mọi không gian Hausdorff hữu hạn chiều là một không gian Montel. Một không gian có chuẩn là một không gian Montel thì compact địa phương, do đó hữu hạn chiều (I, p. 15, định lý 3).

#### Ví dụ 2 {#evt-iv-s2-n5-exa-2 .statement}

Với các ký hiệu và giả thiết của mệnh đề 7 của III, p. 6, không gian E, là giới hạn quy nạp của các không gian Banach, là barreled (III, p. 25); hơn nữa, mọi tập con bị chặn của E đều tương đối compact (III, p. 6, mệnh đề 7). Nói cách khác, E là một không gian Montel. Đặc biệt, các không gian Gevrey (III, p. 10) là các không gian Montel. * Điều này đúng cho không gian $\mathcal{H}(K)$ gồm các mầm của các hàm giải tích trong một lân cận của một tập con compact K của $\mathbf{C}^n$ (III, p. 10).*

#### Ví dụ 3 {#evt-iv-s2-n5-exa-3 .statement}

Mọi giới hạn quy nạp ngặt E của một dãy $(E_n)$ các không gian Montel (II, p. 33) sao cho $E_n$ là đóng trong $E_{n+1}$ với mọi n, là một không gian Montel; thật vậy, E là Hausdorff (II, p. 32, mệnh đề 9 (i)), barreled (III, p. 25, hệ quả 3) và mọi tập con bị chặn của E được chứa trong một trong các $E_n$ (III, p. 5, mệnh đề 6) do đó tương đối compact trong $E_n$, và do đó cũng trong E.

#### Ví dụ 4 {#evt-iv-s2-n5-exa-4 .statement}

Cho U là một tập mở trong $\mathbf{R}^n$ và cho $\mathcal{C}^\infty(U)$ là không gian Fréchet của các hàm khả vi vô hạn trên U (III, p. 9). Ta sẽ chứng minh rằng đây là một không gian Montel. Vì $\mathcal{C}^\infty(U)$ là một không gian Fréchet, nên nó là barreled (III, p. 25, hệ quả). Cho B là một tập con bị chặn của $\mathcal{C}^\infty(U)$ và cho K là một tập con compact của U. Với mọi $\alpha \in \mathbf{N}^n$ cho $H_{\alpha, K}$ là tập các hạn chế lên K của các hàm $\partial^\alpha f$, khi $f$ chạy qua B. Cho $\alpha \in \mathbf{N}^n$; với mọi $\beta \in \mathbf{N}^n$ sao cho $|\beta| = |\alpha| + 1$, tập $H_{\alpha, K}$ bị chặn trong $\mathcal{C}(K)$ vì B bị chặn trong $\mathcal{C}^\infty(U)$; theo VAR, R., No. 2.2.3, tập $H_{\alpha, K}$ đều liên tục, do đó (GT, X, § 2, No. 5) tương đối compact trong $\mathcal{C}(K)$. Nhưng tôpô của $\mathcal{C}^\infty(U)$ là thô nhất trong số các tôpô sao cho mọi ánh xạ $f \mapsto \partial^\alpha f|K$ từ $\mathcal{C}^\infty(U)$ vào $\mathcal{C}(K)$ đều liên tục, do đó B tương đối compact trong $\mathcal{C}^\infty(U)$ (GT, I, § 4, No. 1, mệnh đề 3 và § 9, No. 5, hệ quả).

Tương tự, *không gian $\mathcal{C}_0^\infty(U)$ của tất cả các hàm khả vi vô hạn có giá compact trong U* (III, p. 9) *là một không gian Montel*. Thật vậy, $\mathcal{C}_0^\infty(U)$ là giới hạn quy nạp ngặt của một dãy $\mathcal{C}_{H_n}^\infty(U)$ các không gian Fréchet (III, p. 9), và chỉ cần thấy rằng mỗi không gian $\mathcal{C}_{H_n}^\infty(U)$ là một không gian Montel (*Ví dụ 3*). Nhưng một tập con bị chặn và đóng của $\mathcal{C}_0^\infty(U)$ là đóng và bị chặn trong $\mathcal{C}^\infty(U)$, do đó compact trong $\mathcal{C}^\infty(U)$, và suy ra trong $\mathcal{C}_{H_n}^\infty(U)$. *

#### Mệnh đề 8 {#evt-iv-s2-prop-8 .statement}

*Cho E là một không gian Montel và $\mathfrak{T}$ là một lọc trên E, hội tụ đến một điểm $x_0$ trong E đối với tôpô yếu hơn. Nếu $\mathfrak{T}$ là một cơ sở đếm được, hoặc chứa một tập bị chặn, thì $\mathfrak{T}$ cũng hội tụ đến $x_0$ đối với tôpô ban đầu.*

Trước hết giả sử rằng tồn tại một tập bị chặn $\overline{B}$ trong $\mathfrak{T}$. Bao đóng $\overline{B}$ của B đối với tôpô ban đầu của E là bị chặn; thêm nữa, $\overline{B}$ là compact vì E là một không gian Montel. Tôpô trên $\overline{B}$ được cảm sinh bởi $\sigma(E, E')$ là Hausdorff và thô hơn tôpô được cảm sinh bởi tôpô ban đầu; do đó chúng trùng nhau (GT, I, § 9, No. 4). Điều này chứng minh mệnh đề trong trường hợp này.

Tiếp theo giả sử rằng $\mathfrak{T}$ có một cơ sở đếm được. Chỉ cần (GT, I, § 6, No. 8, mệnh đề 11) xét trường hợp của một dãy $(x_n)_{n \geq 1}$ tiến tới $x_0$ đối với $\sigma(E, E')$. Gọi B là tập hợp tất cả các $x_n$ với $n \geq 0$. Tập này bị chặn đối với $\sigma(E, E')$, do đó cũng bị chặn đối với tôpô ban đầu (III, p. 27, hệ quả 3). Vậy ta đã quy về trường hợp thứ nhất của chứng minh.

*Mọi không gian Montel đều phản xạ*: điều này suy ra từ định nghĩa 4 và từ định lý 2 của IV, p. 16. Hơn nữa:

#### Mệnh đề 9 {#evt-iv-s2-prop-9 .statement}

*Đối ngẫu mạnh của một không gian Montel là một không gian Montel.*

Cho E là một không gian Montel và $E'_b$ là đối ngẫu mạnh của nó. Vì E phản xạ, $E'_b$ là barrelled (IV, p. 15, th. 1). Vì mọi tập con bị chặn của E đều compact tương đối, tôpô mạnh trên $E'$ trùng với tôpô hội tụ compact. Gọi B là một tập con bị chặn của $E'_b$; nó bị chặn đối với tôpô yếu $\sigma(E', E)$, do đó là đều liên tục vì E là barrelled. Khi đó định lý Ascoli (GT, X, § 2, No. 4, hệ quả và § 2, No. 5, hệ quả 1) suy ra rằng bao đóng của B đối với $\sigma(E', E)$ là compact đối với tôpô hội tụ compact; do đó B compact tương đối trong $E'_b$.

#### Mệnh đề 10 {#evt-iv-s2-prop-10 .statement}

*Mọi không gian Montel khả metric thỏa mãn tiên đề đếm được thứ nhất.*

Cho E là một không gian Montel khả metric. Ta biết (II, p. 5) rằng E có thể được đồng nhất với một không gian con của tích $F = \prod_{n \in \mathbf{N}} F_n$ của một dãy các không gian có chuẩn, và thậm chí có thể giả sử rằng $\mathrm{pr}_n(E) = F_n$ với mọi $n \in \mathbf{N}$. Nếu mỗi không gian khả metric $F_n$ thỏa mãn tiên đề đếm được thứ nhất, thì F cũng thế (GT, IX, § 2, No. 8), và do đó E cũng thế.

Ta chứng minh bằng *phản chứng*. Giả sử chẳng hạn rằng $F_0$ không thỏa mãn tiên đề đếm được thứ nhất. Gọi $B_0$ là quả cầu đơn vị (đóng) trong $F_0$; đó là một không gian metric không thỏa mãn tiên đề đếm được thứ nhất. Ta sẽ dùng bổ đề sau:

#### Bổ đề 1 {#evt-iv-s2-lem-1 .statement}

*Giả sử không gian metric X không thỏa mãn tiên đề đếm được thứ nhất. Khi đó tồn tại một số thực $\varepsilon > 0$ và một tập con không đếm được A trong X sao cho $d(x, y) \geq \varepsilon$ với mọi cặp $x, y$ phân biệt trong A.*

Với mỗi số nguyên $n \geq 1$, gọi $\mathfrak{F}_n$ là tập hợp (được sắp thứ tự bởi bao hàm) các tập con D của X sao cho $d(x, y) \geq \frac{1}{n}$ với các $x, y$ phân biệt trong D. Tập $\mathfrak{F}_n$ có đặc trưng hữu hạn, nên có một phần tử cực đại $D_n$ (S, III, § 4, No. 5). Khi đó với mọi $y \in X$, tồn tại một điểm $x$ trong $D_n$ sao cho $d(x, y) < \frac{1}{n}$, do tính cực đại của $D_n$.

Đặt $D = \bigcup_n D_n$; khi đó tập D trù mật trong X, và vì X không thỏa mãn tiên đề đếm được thứ nhất, D không đếm được, nên một trong các $D_n$ không đếm được.

Q.E.D.

By bổ đề 1, áp dụng cho $B_0$, tồn tại một tập hợp con vô hạn đếm được $A_0$ của $F_0$ và một số $\varepsilon > 0$ sao cho $\|x\| \leq 1$ và $\|x - y\| \geq \varepsilon$ đối với các $x, y$ phân biệt trong $A_0$. Ta có $\mathrm{pr}_0(E) = F_0$ và do đó tồn tại một tập hợp con A của E sao cho $\mathrm{pr}_0$ cảm sinh một song ánh từ A lên $A_0$.

#### Bổ đề 2 {#evt-iv-s2-lem-2 .statement}

*Tồn tại một dãy $(x_m)_{m \geq 0}$ gồm các phần tử phân biệt của A, bị chặn trong E.*

Ta sẽ xây dựng một dãy $(x_m)_{m \geq 0}$ các điểm của A bằng quy nạp; và một dãy giảm $(C_m)_{m \geq 0}$ gồm các tập hợp con của A thỏa mãn các điều kiện sau :
a) Không một tập nào trong số các tập $C_m$ là đếm được.
b) Với mọi $n \geq 0$, tập $\mathrm{pr}_k(C_m)$ bị chặn trong $F_k$ với $0 \leq k \leq m$.
c) Với mọi $m \geq 0$, ta có $x_m \in C_m - C_{m+1}$.

Ta đặt $C_0 = A$. Giả sử các tập $C_m$ với $0 \leq m \leq n$ đã được định nghĩa, sao cho thỏa mãn a) và b) với $0 \leq m \leq n$, và đồng thời các điểm $x_m$ trong $C_m - C_{m+1}$ với $0 \leq m < n$. Với mọi số nguyên $r \geq 1$, ký hiệu $C_{n,r}$ là tập hợp tất cả các $x \in C_n$ sao cho

$$
r - 1 \leq \| \mathrm{pr}_{n+1}(x) \| < r .
$$

Vì $C_n$ không đếm được, tồn tại một số nguyên $r \geq 1$ sao cho $C_{n,r}$ không đếm được. Ta chọn một điểm $x_n$ trong $C_{n,r}$ và đặt $C_{n+1} = C_{n,r} - \{ x_n \}$. Hiển nhiên $C_{n+1} \subset C_n$ và $x_n \in C_n - C_{n+1}$, tập $C_{n+1}$ không đếm được và $\mathrm{pr}_k(C_{n+1})$ bị chặn trong $F_n$ với $0 \leq k \leq n + 1$.

Ta có $x_m \in C_m$, nên $x_m \in C_n$ với $m \geq n$. Do đó phép chiếu của dãy $(x_m)_{m \geq 0}$ lên $F_n$ bị chặn với mọi $n \geq 0$; nói cách khác, dãy $(x_m)_{m \geq 0}$ bị chặn trong E, và điều này chứng minh bổ đề 2.

Q.E.D.

Với các ký hiệu của bổ đề 2, dãy bị chặn $(x_m)_{m \geq 0}$ có một điểm giới hạn $y$ trong E. Do đó dãy $(\mathrm{pr}_0(x_m))_{m \geq 0}$ có một điểm giới hạn $\mathrm{pr}_0(y)$ trong $F_0$, nhưng điều này mâu thuẫn với phép dựng của $A_0$.

#### Hệ quả {#evt-iv-s2-n5-cor-1 .statement}

— Cho E là một không gian Montel khả mêtric. Khi đó tồn tại một tập trù mật đếm được trong đối ngẫu mạnh của E.

Trên đối ngẫu E' của E, tôpô mạnh trùng với tôpô hội tụ đều trên các tập compact, vì E là một không gian Montel. Bây giờ chỉ cần áp dụng hệ quả 1 của mệnh đề 6 của III, p. 18.

Ta có thể chứng minh rằng đối ngẫu mạnh của một không gian Montel khả mêtric E không khả mêtric nếu E là vô hạn chiều (IV, p. 57, bài tập 1).

### Bài tập {#evt-iv-s2-exercises}

Xem [các bài tập cho § 2](exercises/s2/).
