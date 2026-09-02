---
book: alg
book_title: Algebra
chapter: X
chapter_title: ALGÈBRE HOMOLOGIQUE
section: 3
section_title: Résolutions
lang: vi
source: alg-x-fr
book_pages: A X.46-A X.61, A X.178-A X.184
pdf_pages: 0052-0067, 0184-0190
extraction: ocr
subsections:
    - "no": 1
      title: Prolongement de morphismes de complexes
      page: 46
      pdf_page: 52
    - "no": 2
      title: Résolutions
      page: 48
      pdf_page: 54
    - "no": 3
      title: La résolution libre canonique
      page: 50
      pdf_page: 56
    - "no": 4
      title: La résolution injective canonique
      page: 52
      pdf_page: 58
    - "no": 5
      title: Résolutions de type fini
      page: 53
      pdf_page: 59
    - "no": 6
      title: ' Résolutions projectives minimales'
      page: 54
      pdf_page: 60
    - "no": 7
      title: Résolutions graduées
      page: 56
      pdf_page: 62
    - "no": 8
      title: La résolution standard
      page: 57
      pdf_page: 63
    - "no": 9
      title: Résolutions et groupes de Grothendieck
      page: 58
      pdf_page: 64
statements: 29
exercises: 19
content_sha256: f352f2576ab279eed7807e006084b19b8fc7707f6a31e8022146dab85e262772
translated_from: content/en-mt/alg/X/03_s3_resolutions.md
source_lang: en-mt
translation_method: machine
source_content_sha256: a1b2e48f6dae81d4cf5b709be2d47f83208c48b5e620837f8b9559aaa92197bf
translation_model: gpt-5.4
translation_run: translate-vi-950f1267
glossary_version: 34
glossary_terms_sha256: dc5f6fbe0b5a18cd3315255f6163a5816edb7825a432e251fd864347cc3f43d7
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 3. PHÂN GIẢI

Chúng tôi giữ lại các quy ước của đoạn trước.

### 1. Mở rộng các cấu xạ của các phức

#### Bổ đề 1 {#alg-x-s3-lem-1 .statement}

Xét một biểu đồ các A-môđun và các đồng cấu

$$
\begin{array}{ccc}
M' & \xrightarrow{\alpha'} & M \\
f' \downarrow & & f \downarrow \\
N' & \xrightarrow{\beta'} & N
\end{array}
\quad
\begin{array}{ccc}
M & \xrightarrow{\alpha} & M'' \\
f \downarrow & & k'' \downarrow \\
N & \xrightarrow{\beta} & N''
\end{array}
$$

sao cho $f \circ \alpha' = \beta \circ f', \alpha \circ \alpha' = 0, \mathrm{Ker}\ \beta = \mathrm{Im}\ \beta', \text{và } f = k'' \circ \alpha + \beta \circ k \text{ và trong đó } M' \text{ là xạ ảnh. Tồn tại một A-đồng cấu } k': M' \to N' \text{ sao cho } f' = k \circ \alpha' + \beta' \circ k'.$

Thật vậy, đặt $g = f' - k \circ \alpha'$; ta có
$$
\beta \circ g = \beta \circ f' - \beta \circ k \circ \alpha' = f \circ \alpha' - \beta \circ k \circ \alpha' = k'' \circ \alpha \circ \alpha' = 0.
$$
Điều này suy ra $\mathrm{Im}\ (g) \subset \mathrm{Ker}\ (\beta) = \mathrm{Im}\ (\beta')$. Vì $M'$ là xạ ảnh, do đó tồn tại một A-đồng cấu $k': M' \to N'$ sao cho $\beta' \circ k' = g$, do đó bổ đề được chứng minh.

#### Bổ đề 2 {#alg-x-s3-lem-2 .statement}

Nếu trong biểu đồ giao hoán các A-môđun và các đồng cấu

$$
\begin{array}{ccc}
M' & \xrightarrow{\alpha'} & M \\
& \downarrow u & \downarrow u'' \\
N' & \xrightarrow{\beta'} & N
\end{array}
\quad
\begin{array}{ccc}
M & \xrightarrow{\alpha} & M'' \\
& \downarrow & \downarrow \\
N & \xrightarrow{\beta} & N''
\end{array}
$$

ta có $\alpha \circ \alpha' = 0, \mathrm{Ker}\ \beta = \mathrm{Im}\ \beta'$ và nếu $M'$ là xạ ảnh, thì tồn tại một A-đồng cấu $u': M' \to N'$ sao cho $\beta' \circ u' = u \circ \alpha'$.

Chỉ cần đặt $k'' = u'', k = -u, f = 0, f' = 0$ và $u' = k'$ trong Bổ đề 1.

Bổ đề 1 bis. — Xét một biểu đồ các A-môđun và các đồng cấu

$$
\begin{array}{ccc}
M' & \xrightarrow{\alpha'} & M \\
k' \downarrow & & k \downarrow \\
N' & \xrightarrow{\beta'} & N
\end{array}
\quad
\begin{array}{ccc}
M & \xrightarrow{\alpha} & M'' \\
f' \downarrow & & f \downarrow \\
N & \xrightarrow{\beta} & N''
\end{array}
$$

sao cho $f \circ \alpha' = \beta \circ f'$, $\mathrm{Ker}\, \alpha = \mathrm{Im}\, \alpha'$, $\beta \circ \beta' = 0$, and $f' = k \circ \alpha' + \beta' \circ k'$ and where $N''$ is injective. There exists an $A$-homomorphism $k'' : M'' \to N''$ such that $f = k'' \circ \alpha + \beta \circ k$.

Thật vậy, đặt $g = f - \beta \circ k$, ta có
$$
g \circ \alpha' = f \circ \alpha' - \beta \circ k \circ \alpha' = \beta \circ f' - \beta \circ k \circ \alpha' = \beta \circ \beta' \circ k' = 0 .
$$
Điều này suy ra $\mathrm{Ker}\, g \supset \mathrm{Im}\, \alpha' = \mathrm{Ker}\, \alpha$. Vì $N''$ là đơn ánh, do đó tồn tại (X, p. 16, nhận xét) một $A$-đồng cấu $k' : M'' \to N''$ sao cho $g = k'' \circ \alpha$, do đó bổ đề được chứng minh.

Bổ đề 2 bis. — Nếu, trong biểu đồ giao hoán các $A$-môđun và các đồng cấu

$$
\begin{array}{ccc}
M' & \xrightarrow{\alpha'} & M \xrightarrow{\alpha} M'' \\
u' \downarrow & & u \downarrow \\
N' & \xrightarrow{\beta'} & N \xrightarrow{\beta} N''
\end{array}
$$

ta có $\mathrm{Ker}\, \alpha = \mathrm{Im}\, \alpha', \beta \circ \beta' = 0$ và nếu $N''$ là đơn ánh, thì tồn tại một $A$-đồng cấu $u'' : M'' \to N''$ sao cho $u'' \circ \alpha = \beta \circ u$.
Chỉ cần đặt $u' = k', u = -k, f = 0, f' = 0$ và $k'' = u''$ trong Bổ đề 1 bis.

#### Mệnh đề 1 {#alg-x-s3-prop-1 .statement}

Cho $(P, d_P)$ và $(E, d_E)$ là hai phức các $A$-môđun và $r$ là một số nguyên.

a) Cho $(u_i : P_i \to E_i)_{i \leq r}$ là một họ các đồng cấu sao cho $d_E \circ u_i = u_{i-1} \circ d_P$ với $i \leq r$. Giả sử rằng $P_i$ là xạ ảnh với $i > r$ và $H_i(E) = 0$ với $i \geq r$. Khi đó họ các $u_i$ được mở rộng thành một cấu xạ của các phức từ $P$ vào $E$; hai mở rộng như vậy là đồng luân.

b) Cho $(u^i : P^i \to E^i)_{i \leq r}$ là một họ các đồng cấu sao cho $u^i \circ d_P = d_E \circ u^{i-1}$ với $i \leq r$. Giả sử rằng $E^i$ là đơn ánh với $i > r$ và $H^i(P) = 0$ với $i \geq r$. Khi đó họ các $u^i$ mở rộng thành một cấu xạ của các phức từ $P$ vào $E$; hai mở rộng như vậy là đồng luân.

Ta chứng minh a). Sự tồn tại của một mở rộng $v$ của họ $(u_i)_{i \leq r}$ suy ra ngay từ Bổ đề 2 bằng quy nạp. Cho $v'$ là một mở rộng khác; đặt $f = v' - v$, và xây dựng bằng quy nạp theo số nguyên $n$ một đồng cấu $k_n : P_n \to E_{n+1}$ sao cho $f_n = d_E \circ k_n + k_{n-1} \circ d_P$. Với $i \leq r$, lấy $k_i = 0$. Cho $n \geq r$ và giả sử rằng các $k_i$ đã được xây dựng với $i \leq n$. Khi đó xét biểu đồ

$$
\begin{array}{cccccc}
P_{n+1} & \xrightarrow{d_P} & P_n & \xrightarrow{d_P} & P_{n-1} \\
f_{n+1} \downarrow & & & & k_{n-1} \downarrow \\
E_{n+2} & \xrightarrow{d_E} & E_{n+1} & \xrightarrow{d_E} & E_n .
\end{array}
$$

Các giả thiết của Bổ đề 1 được thỏa mãn; do đó tồn tại một $A$-đồng cấu $k_{n+1} : P_{n+1} \to E_{n+2}$ sao cho $f_{n+1} = d_E \circ k_{n+1} + k_n \circ d_P$, do đó suy ra a).

Chứng minh của b) là tương tự, thông qua các Bổ đề 1 bis và 2 bis.

### 2. Phân giải

Trong phần sau, một môđun sẽ luôn luôn được đồng nhất với phức mà trong đó nó là thành phần bậc không và mọi thành phần khác của nó đều bằng không.

#### Định nghĩa 1 {#alg-x-s3-def-1 .statement}

Cho $M$ là một $A$-môđun. Một phân giải trái của $M$ là một cặp $(P,p)$ trong đó $P$ là một phức bằng không ở bên phải và $p:P\to M$ là một đồng cấu. Một phân giải phải của $M$ là một cặp $(e,E)$ trong đó $E$ là một phức bằng không ở bên trái và $e:M\to E$ là một đồng cấu.

Độ dài của phân giải $(P,p)$ (ứng với $(e,E)$) được gọi là độ dài của phức $P$ (ứng với $E$). Nếu $(P,p)$ và $(P',p')$ (ứng với $(e,E)$ và $(e',E')$) là hai phân giải trái (ứng với phải) của $M$, thì một cấu xạ của các phức $f:P\to P'$ sao cho $p'\circ f=p$ (ứng với $g:E\to E'$ sao cho $g\circ e=e'$) được gọi là một cấu xạ của các phân giải.

#### Mệnh đề 2 {#alg-x-s3-prop-2 .statement}

Cho $P$ là một phức bằng không ở bên phải và $p:P\to M$ là một cấu xạ.
Để $(P,p)$ là một phân giải trái của $M$, điều kiện cần và đủ là dãy

(1)

$$
\cdots\longrightarrow P_n\xrightarrow{d_P}P_{n-1}\longrightarrow\cdots\longrightarrow P_1\xrightarrow{d_P}P_0\xrightarrow{p}M\longrightarrow0
$$

là khớp.

Thật vậy, nói rằng $p:P\to M$ là một đồng cấu có nghĩa là $H_i(P)=0$ với $i>0$ và $p_0$ cảm sinh một đẳng cấu từ $\operatorname{Coker}(d_P:P_1\to P_0)$ lên $M$.

Tương tự:

**Mệnh đề 2bis.** — Cho $E$ là một phức triệt tiêu ở bên trái và $e:M\to E$ là một cấu xạ.
Để $(e,E)$ là một phân giải phải của $M$, điều kiện cần và đủ là dãy

(1 bis)

$$
0\longrightarrow M\xrightarrow{e_0}E^0\xrightarrow{d_E}E^1\longrightarrow\cdots\longrightarrow E^n\xrightarrow{d_E}E^{n+1}\longrightarrow\cdots
$$

là khớp.

Do lạm dụng ngôn ngữ, người ta thường nói rằng dãy (1) (tương ứng, (1 bis)) là một phân giải trái (tương ứng, phải) của $M$.

#### Định nghĩa 2 {#alg-x-s3-def-2 .statement}

Một phân giải xạ ảnh (tương ứng, tự do, tương ứng, phẳng) của $A$-môđun $M$ là một phân giải trái $(P,p)$ của $M$ sao cho phức $P$ là xạ ảnh (tương ứng, tự do, tương ứng, phẳng) (X, p. 25). Một phân giải nội xạ của $M$ là một phân giải phải $(e,E)$ của $M$ sao cho phức $E$ là nội xạ (loc. cit.).

#### Ví dụ 1 {#alg-x-s3-n2-exa-1 .statement}

Giả sử rằng vành $A$ là chính; cho $M$ là một $A$-môđun và $(x_i)_{i\in I}$ là một họ sinh của $M$. Ký hiệu $L_0$ là môđun tự do $A^{(I)}$, $(e_i)$ là cơ sở chính tắc của nó, và định nghĩa $p:L_0\to M$ bởi $p(e_i)=x_i$. Cấu xạ $p$ là toàn ánh và hạt nhân của nó $L_1$ là một $A$-môđun tự do theo VII, § 3, Hệ quả 2 của Định lý 1; do đó dãy khớp

$$
0\longrightarrow L_1\longrightarrow L_0\xrightarrow{p}M\longrightarrow0
$$

là một phân giải tự do của $M$ có độ dài 1. Nếu $I$ là hữu hạn, thì $L_0$ và $L_1$ là hữu hạn kiểu.

#### Ví dụ 2 {#alg-x-s3-n2-exa-2 .statement}

Giả sử A giao hoán; cho E là một A-môđun và u là một tự đồng cấu của E. Ký hiệu bởi $E_u$ môđun $A[X]$ thu được bằng cách trang bị cho E cấu trúc được định nghĩa bởi

$$
(p, x) \mapsto p(u)(x) \quad \text{với} \quad p \in A[X] \quad \text{và} \quad x \in E.
$$

Theo III, p. 106, ta có một dãy khớp:

$$
0 \to A[X] \otimes_A E \xrightarrow{\psi} A[X] \otimes_A E \xrightarrow{\varphi} E_u \to 0
$$

trong đó $\varphi(p \otimes x) = p.x$ và $\psi(p \otimes x) = Xp \otimes x - p \otimes u(x)$ với $p \in A[X]$ và $x \in E$. Dãy khớp này là một phân giải có độ dài 1 của $E_u$, tự do (tương ứng, xạ ảnh, tương ứng, hữu hạn kiểu) nếu E là một A-môđun tự do (tương ứng, xạ ảnh, tương ứng, hữu hạn kiểu).

#### Ví dụ 3 {#alg-x-s3-n2-exa-3 .statement}

Nếu A là chính, dãy khớp

$$
0 \to A \to K \to K/A \to 0
$$

là một phân giải nội xạ có độ dài 1 của A-môđun $A_s$ (X, p. 18, Ví dụ 1).

#### Mệnh đề 3 {#alg-x-s3-prop-3 .statement}

Cho $f : M' \to M$ là một đồng cấu của các A-môđun, $p' : P' \to M'$ là một cấu xạ vào $M'$ của một phức triệt tiêu ở bên phải và xạ ảnh $P'$, và $p : P \to M$ là một phân giải trái của M. Tồn tại một cấu xạ các phức $\tilde{f} : P' \to P$, và chỉ có một, sai khác bởi đồng luân, sao cho $p \circ \tilde{f} = f \circ p'$.

Xét phức $\overline{P}$ được xác định như sau: $\overline{P}_n = P_n$ với $n \neq -1$, $\overline{P}_{-1} = M$, $d_{\overline{P},n} = d_{P,n}$ với $n \neq 0, -1$, $d_{\overline{P},0} = p_0$, $d_{\overline{P},-1} = 0$, và phức $\overline{P}'$ được xác định tương tự. Áp dụng cho các phức $\overline{P}$ và $\overline{P}'$ Mệnh đề 1 a) với $r = 0$, $u_i = 0$ với $i < -1$ và $u_{-1} = f$, ta thu được Mệnh đề 3.

#### Hệ quả {#alg-x-s3-n2-cor-1 .statement}

Cho $(P, p)$ và $(P', p')$ là hai phân giải xạ ảnh của M. Tồn tại một cấu xạ, và chỉ một đến đồng luân, $\alpha : P' \to P$ sao cho $p \circ \alpha = p'$.

Thật vậy, tồn tại một cấu xạ $\alpha : P' \to P$ (tương ứng, $\beta : P \to P'$) sao cho $p \circ \alpha = p'$ (tương ứng, $p' \circ \beta = p$). Vì $p \circ \alpha \circ \beta = p$ (tương ứng, $p' \circ \beta \circ \alpha = p'$), nên $\alpha \circ \beta$ đồng luân với $1_P$ (tương ứng, $\beta \circ \alpha$ đồng luân với $1_{P'}$).

MỆNH ĐỀ 3 bis. — Cho $g : N \to N'$ là một đồng cấu các A-môđun, $e' : N' \to E'$ một cấu xạ từ $N'$ vào một phức trái không và đơn ánh $E'$, và $e : N \to E$ một phân giải phải của N. Tồn tại một cấu xạ các phức $\tilde{g} : E \to E'$, và chỉ một đến đồng luân, sao cho $\tilde{g} \circ e = e' \circ g$.

Điều này được chứng minh như Mệnh đề 3 với sự trợ giúp của Mệnh đề 1 b).

#### Hệ quả {#alg-x-s3-n2-cor-2 .statement}

Cho $(e, E)$ và $(e', E')$ là hai phân giải đơn ánh của N; tồn tại một cấu xạ $\alpha : E \to E'$ và chỉ một đến đồng luân sao cho $\alpha \circ e = e'$.

### 3. Phân giải tự do chính tắc

Với mọi A-môđun M, ký hiệu L_0(M) là A-môđun tự do A^{(M)} có cơ sở là M, ký hiệu (e_m)_{m \in M} là cơ sở chính tắc của nó, và ký hiệu $p_M : L_0(M) \to M$ là đồng cấu sao cho
$$
p_M(e_m) = m , \quad m \in M .
$$
Đặt $Z_0(M) = \mathrm{Ker}\, p_M$ và gọi $i_M : Z_0(M) \to L_0(M)$ là đơn ánh chính tắc. Ta có một dãy khớp
$$
(1) \qquad 0 \longrightarrow Z_0(M) \xrightarrow{i_M} L_0(M) \xrightarrow{p_M} M \longrightarrow 0 .
$$
Một môđun phân bậc L(M) được xác định bằng cách đặt $L_n(M) = 0$ với $n < 0$ và, bằng quy nạp theo số nguyên $n > 0$
$$
(2) \qquad L_n(M) = L_0(Z_{n-1}(M)) ; \qquad Z_n(M) = Z_0(Z_{n-1}(M)) .
$$
Các A-đồng cấu $d_n^M : L_n(M) \to L_{n-1}(M)$ được xác định bởi
$$
(3) \qquad \left\{ \begin{array}{ll}
d_n^M = 0 , & n \leqslant 0 , \\
d_1^M = i_M \circ p_{Z_0(M)} , \\
d_n^M = i_{Z_{n-2}(M)} \circ p_{Z_{n-1}(M)} , & n > 1 .
\end{array} \right.
$$
Theo phép dựng ta có một dãy khớp
$$
\longrightarrow L_n(M) \xrightarrow{d_n^M} L_{n-1}(M) \longrightarrow \cdots \longrightarrow L_0(M) \xrightarrow{p_M} M \longrightarrow 0 ,
$$
nên, nếu mở rộng $p_M$ thành một cấu xạ các phức
$$
p_M : (L(M), d^M) \to M ,
$$
ta thu được một phân giải tự do của M, gọi là phân giải tự do chính tắc của M.

Cho $f : M \to N$ là một A-đồng cấu của các A-môđun. Ký hiệu
$$
L_0(f) : L_0(M) \to L_0(N)
$$
là A-đồng cấu duy nhất sao cho $L_0(f)(e_m) = e_{f(m)}$ với mọi $m \in M$. Ta có
$$
(4) \qquad p_N \circ L_0(f) = f \circ p_M .
$$
Do đó $L_0(f)$ cảm sinh một A-đồng cấu $Z_0(f) : Z_0(M) \to Z_0(N)$ và ta có
$$
(5) \qquad i_N \circ Z_0(f) = L_0(f) \circ i_M .
$$
Đặt $L_n(f) = 0$, với $n < 0$ và định nghĩa bằng quy nạp theo số nguyên $n > 0$, các đồng cấu $L_n(f) : L_n(M) \to L_n(N)$ và $Z_n(f) : Z_n(M) \to Z_n(N)$ bởi
$$
(6) \qquad \left\{ \begin{array}{l}
L_n(f) = L_0(Z_{n-1}(f)) \\
Z_n(f) = Z_0(Z_{n-1}(f)) .
\end{array} \right.
$$

#### Mệnh đề 4 {#alg-x-s3-prop-4 .statement}

$L(f) : L(M) \to L(N)$ là một cấu xạ của các phức A-môđun; ta có $p_M \circ L(f) = f \circ p_N$.

Cần chứng minh, với mọi số nguyên $n > 0$, công thức

$$
d_n^N \circ L_n(f) = L_{n-1}(f) \circ d_n^M .
$$

Trước hết ta có

$$
\begin{align*}
d_1^N \circ L_1(f) &= i_N \circ p_{Z_0(N)} \circ L_0(Z_0(f)) & \text{(theo (3) và (6))} \\
&= i_N \circ Z_0(f) \circ p_{Z_0(M)} & \text{(theo (4))} \\
&= L_0(f) \circ i_M \circ p_{Z_0(M)} & \text{(theo (5))} \\
&= L_0(f) \circ d_1^M & \text{(theo (3))} .
\end{align*}
$$

Khi $n > 1$, ta lần lượt có

$$
\begin{align*}
d_n^N \circ L_n(f) &= i_{Z_{n-2}(N)} \circ p_{Z_{n-1}(N)} \circ L_0(Z_{n-1}(f)) & \text{(theo (3) và (6))} \\
&= i_{Z_{n-2}(N)} \circ Z_{n-1}(f) \circ p_{Z_{n-1}(M)} & \text{(theo (4))} \\
&= i_{Z_{n-2}(N)} \circ Z_0(Z_{n-2}(f)) \circ p_{Z_{n-1}(M)} & \text{(theo (6))} \\
&= L_0(Z_{n-2}(f)) \circ i_{Z_{n-2}(M)} \circ p_{Z_{n-1}(M)} & \text{(theo (5))} \\
&= L_{n-1}(f) \circ d_n^M & \text{(theo (3) và (6))} .
\end{align*}
$$

Ta có ngay

(7)
$$
L(1_M) = 1_{L(M)} .
$$

Mặt khác, nếu $g : N \to P$ là một A-đồng cấu của các A-môđun, ta có

(8)
$$
L(g \circ f) = L(g) \circ L(f) .
$$

Thật vậy, với $m \in M$, ta có
$$
L_0(g \circ f)(e_m) = e_{g \circ f(m)} = L_0(g)(e_{f(m)}) = L_0(g) \circ L_0(f)(e_m) ,
$$
do đó $L_0(g \circ f) = L(g) \circ L(f)$; do đó $Z_0(g \circ f) = Z_0(g) \circ Z_0(f)$; do đó ngay lập tức $L_n(g \circ f) = L_n(g) \circ L_n(f)$, với $n \geqslant 0$, bằng quy nạp theo $n$, do đó có (8).

#### Nhận xét {#alg-x-s3-n3-rem-1 .statement}

Nếu $f, g \in \mathrm{Hom}_A(M, N)$, ta không có $L(f + g) = L(f) + L(g)$. Tuy nhiên hai cấu xạ này là đồng luân theo X, p. 49, mệnh đề 3.

Cho $M$ là một A-môđun phải; ký hiệu $A^\circ$ là vành đối của $A$, $M^\circ$ là $A^\circ$-môđun nền của $M$, $L(M^\circ)$ là phân giải tự do chính tắc của nó. Phân giải này được ký hiệu là $L(M)$, và A-phức nền $L(M^\circ)^\circ$ của $L(M^\circ)$ được gọi là phân giải tự do chính tắc của $M$. Do đó ta có

$$
L(M^\circ) = L(M)^\circ .
$$

### 4. Phân giải nội xạ chính tắc

Cho $F$ là A-môđun $\operatorname{Hom}_{\mathbf Z}(A,\mathbf Q/\mathbf Z)$; với mọi A-môđun $M$, đặt $I^0(M)=F^{\operatorname{Hom}_A(M,F)}$ và ký hiệu bởi $e_M:M\longrightarrow I^0(M)$ đồng cấu gán cho $m\in M$ họ $(\varphi(m))_{\varphi\in\operatorname{Hom}_A(M,F)}$. Theo X, p. 19, hệ quả 2, $I^0(M)$ là một A-môđun nội xạ và $e_M$ là đơn ánh. Đặt $K^0(M)=\operatorname{Coker}e_M$ và ký hiệu bởi $q_M:I^0(M)\longrightarrow K^0(M)$ phép chiếu chính tắc. Do đó ta có một dãy khớp

$$
0\longrightarrow M\xrightarrow{e_M} I^0(M)\xrightarrow{q_M} K^0(M)\longrightarrow 0.
$$

Một $A$-môđun phân bậc $I(M)$ được định nghĩa bằng cách đặt $I^n(M)=0$ với $n<0$ và, theo phép truy hồi trên số nguyên $n>0$,

(9)
$$
I^n(M)=I^0(K^{n-1}(M)),\qquad K^n(M)=K^0(K^{n+1}(M)).
$$

Các $A$-đồng cấu $\delta_M^n:I^n(M)\longrightarrow I^{n+1}(M)$ được định nghĩa bởi

(10)
$$
\left\{
\begin{aligned}
\delta_M^n&=0, && n<0,\\
\delta_M^0&=\epsilon_{K^0(M)}\circ q_M,\\
\delta_M^n&=\epsilon_{K^n(M)}\circ q_{K^{n-1}(M)}, && n>0.
\end{aligned}
\right.
$$

Theo phép dựng, ta có một dãy khớp

$$
0\longrightarrow M\xrightarrow{e_M} I^0(M)\xrightarrow{\delta_M^0}\cdots\longrightarrow I^n(M)\xrightarrow{\delta_M^n}I^{n+1}(M)\longrightarrow\cdots,
$$

sao cho, nếu mở rộng $e_M$ thành một cấu xạ của các phức

$$
e_M:M\longrightarrow (I(M),\delta_M),
$$

thì ta thu được một giải đơn ánh của $M$, gọi là giải đơn ánh chính tắc của $M$.

Cho $f:M\longrightarrow N$ là một đồng cấu của các $A$-môđun. Gọi $I^0(f)$ là đồng cấu từ $I^0(M)=F^{\operatorname{Hom}_A(M,F)}$ vào $I^0(N)=F^{\operatorname{Hom}_A(N,F)}$ biến họ $(x_\varphi)_{\varphi\in\operatorname{Hom}_A(M,F)}$ thành họ $(x_{\psi\circ f})_{\psi\in\operatorname{Hom}_A(N,F)}$. Ta có:

(11)
$$
I^0(f)\circ e_M=e_N\circ f.
$$

Suy ra $I^0(f)$ cảm sinh một đồng cấu $K^0(f):K^0(M)\longrightarrow K^0(N)$ và ta có

(12)
$$
K^0(f)\circ q_M=q_N\circ K^0(f).
$$

Đặt $I^n(f)=0$ với $n<0$ và định nghĩa, theo phép truy hồi trên số nguyên $n>0$, các đồng cấu $I^n(f):I^n(M)\longrightarrow I^n(N)$ và $K^n(f):K^n(M)\longrightarrow K^n(N)$ bởi:

(13)
$$
\left\{
\begin{aligned}
I^n(f)&=I^0(K^{n-1}(f)),\\
K^n(f)&=K^0(K^{n-1}(f)).
\end{aligned}
\right.
$$

#### Mệnh đề 5 {#alg-x-s3-prop-5 .statement}

I(f) : I(M) → I(N) là một cấu xạ của các phức các A-môđun; ta có I(f) ◦ e_M = e_N ◦ f.
Điều này được chứng minh theo một cách tương tự như Mệnh đề 4.

Ta có
(14)
$$
I(1_M) = 1_{I(M)}
$$
và với mọi đồng cấu $g : N \to P$ của các A-môđun
(15)
$$
I(g \circ f) = I(g) \circ I(f) .
$$

#### Nhận xét {#alg-x-s3-n4-rem-1 .statement}

Nếu $f, g \in \mathrm{Hom}_A(M, N)$, thì không có $I(f + g) = I(f) + I(g)$. Tuy nhiên, hai cấu xạ này là đồng luân theo X, p. 49, mệnh đề 3 bis.

Nếu M là một A-môđun phải, thì đặt $I(M) = I(M^\circ)^\circ$; điều này được gọi là giải đơn ánh chính tắc của M, và ta có
$$
I(M^\circ) = I(M)^\circ .
$$

### 5. Các giải kiểu hữu hạn

Đặc biệt, từ hai số trước suy ra rằng mọi A-môđun đều có các giải đơn ánh, các giải tự do (do đó cũng có các giải xạ ảnh hoặc phẳng). Trong một số trường hợp, người ta có thể nói chính xác hơn:

Giả sử $A$ là Noether trái và $M$ là một $A$-môđun. Ta hãy xây dựng bằng quy nạp các dãy $(L_n)_{n \geq 0}$, $(Z_n)_{n \geq 0}$, $(d_n)_{n \geq 1}$ mà, với mọi $n \geq 0$, $L_n$ là một $A$-môđun tự do sinh hữu hạn, $Z_n$ là một môđun con của $L_n$ và $d_{n+1} : L_{n+1} \to L_n$ là một đồng cấu. Để làm việc đó, chọn một họ sinh hữu hạn $(m_i)_{i \in I_0}$ của $M$, đặt $L_0 = A^{(I_0)}$, định nghĩa $p : L_0 \to M$ bởi $p(e_i) = m_i$ và đặt $Z_0 = \mathrm{Ker}\,(p)$. Với $n \geq 0$, giả sử đã xây dựng $L_n$ và $Z_n$, thì $Z_n$ sinh hữu hạn vì được chứa trong $L_n$; chọn một họ sinh hữu hạn $(x_{n,i})_{i \in I_{n+1}}$ của $Z_n$; đặt $L_{n+1} = A^{(I_{n+1})}$, định nghĩa $d_{n+1}$ bởi $d_{n+1}(e_i) = x_{n,i}$ và đặt $Z_{n+1} = \mathrm{Ker}\,(d_{n+1})$.

Theo phép dựng ta có một dãy khớp
$$
\cdots \longrightarrow L_{n+1} \xrightarrow{d_{n+1}} L_n \longrightarrow \cdots \longrightarrow L_0 \xrightarrow{p} M \longrightarrow 0 ,
$$
do đó:

#### Mệnh đề 6 {#alg-x-s3-prop-6 .statement}

Khi $A$ là Noether trái, mọi $A$-môđun $M$ sinh hữu hạn đều có một phân giải tự do $p : L \to M$ sao cho $L_n$ sinh hữu hạn với mọi số nguyên n.
Nói chung hơn:

#### Mệnh đề 7 {#alg-x-s3-prop-7 .statement}

Cho $C$ là một $A$-phức và $a \in \mathbf{Z}$ sao cho $H_n(C) = 0$ với $n < a$.
a) Tồn tại một $A$-phức tự do $L$ sao cho $L_n = 0$ với $n < a$ và một đồng cấu đồng điều $f : L \to C$.

b) Giả sử $A$ là Noether trái và các $A$-môđun $H_n(C)$, $n\in \mathbf{Z}$, sinh hữu hạn.
Tồn tại một $A$-phức tự do $L$ sao cho $L_n=0$ với $n<a$ và $L_n$ là một $A$-môđun sinh hữu hạn với mọi $n$, và một đồng cấu $f:L\to C$.

Cho $C'$ là phức con của $C$ sao cho $C'_n=C_n$ với $n>a$, $C'_a=Z_a(C)$, $C'_n=0$ với $n<a$; khi đó đơn ánh chính tắc từ $C'$ vào $C$ là một đồng cấu. Do đó, bằng cách thay thế $C$ bởi $C'$, ta có thể giả sử rằng $C_n=0$ với $n<a$. Mệnh đề khi đó suy ra từ việc áp dụng lặp lại bổ đề sau, với $r=a,a+1,\ldots$ :

#### Bổ đề 3 {#alg-x-s3-lem-3 .statement}

Cho $C$ là một phức và cho $r\in \mathbf{Z}$. Tồn tại một phức $C'$ và một đồng cấu $f:C'\to C$ sao cho $f_n:C'_n\to C_n$ là một đẳng cấu với $n<r$ và sao cho $C'_r$ là một $A$-môđun tự do. Nếu $A$ là Noether và các $A$-môđun $H_r(C)$ và $C_{r-1}$ là kiểu hữu hạn, thì có thể đòi hỏi rằng $C'_r$ là kiểu hữu hạn.

a) Trước hết, cho $h:M\to C_r$ là một đồng cấu của các $A$-môđun; ký hiệu $d=(d_n)$ là vi phân của $C$. Cho $N$ là môđun con của $M\times C_{r+1}$ gồm các cặp $(m,x)$ sao cho $h(m)=d_{r+1}(x)$; định nghĩa một phức $(C',d')$ bởi $C'_n=C_n$ với $n\ne r,r+1$, $C'_r=M$, $C'_{r+1}=N$, $d'_n=d_n$ với $n\ne r,r+1$, $d'_r=h$, $d'_{r+1}(m,x)=m$ với $(m,x)\in N$ và $d'_{r+2}(y)=(0,d_{r+2}(y))$ với $y\in C_{r+2}$. Cũng xét cấu xạ của các phức $f:C'\to C$ sao cho $f_n=1_{C_n}$ với $n\ne r,r+1$, $f_r=h$, $f_{r+1}(m,x)=x$.

b) Phức $\operatorname{Ker}f$ bằng không ở bậc $\ne r,r+1$ và vi phân $d'_{r+1}$ cảm sinh một đẳng cấu từ $\operatorname{Ker}f_{r+1}$ lên $\operatorname{Ker}f_r$, do đó $H(\operatorname{Ker}f)=0$.

c) Khi ánh xạ hợp thành $M\xrightarrow{h}C_r\to C_r/B_r(C)$ là toàn ánh, người ta cũng thấy tương tự rằng $H(\operatorname{Coker}f)=0$, và khi đó $f$ là một đồng cấu (X, p. 31, hệ quả 2).

d) Khi giả thiết rằng $A$ là Noether và các A-môđun $H_r(C)$ và $C_{r-1}$ thuộc kiểu hữu hạn, thì $C_r/B_r(C)$ thuộc kiểu hữu hạn, do dãy khớp (X, p. 25)

$$
0\to H_r(C)\to C_r/B_r(C)\to C_{r-1}\ ;
$$

khi đó tồn tại một A-môđun tự do kiểu hữu hạn $M$ và một đồng cấu $h:M\to C_r$ sao cho điều kiện của c) được thỏa mãn; trong trường hợp tổng quát, tồn tại một môđun tự do $M$ và một đồng cấu toàn ánh $h:M\to C_r$. Điều này hoàn tất chứng minh.

### 6.  Phân giải xạ ảnh cực tiểu

Cho $M$ là một A-môđun và

$$
(P)\qquad \cdots \longrightarrow F_n \xrightarrow{d_n} F_{n-1}\longrightarrow \cdots \longrightarrow F_0\xrightarrow{d_0} M\longrightarrow 0
$$

một phân giải của $M$. Người ta nói rằng $(P)$ là một phân giải xạ ảnh cực tiểu nếu, với mọi $n\geq 0$, đồng cấu $\delta_n:P_n\to \operatorname{Im}(d_n)$ cảm sinh bởi $d_n$ là một phủ xạ ảnh (VIII, § 8, No. 5).

#### Proposition 8 {#alg-x-s3-prop-8 .statement}

Cho $M$ là một A-môđun, $P$ và $P'$ là hai phân giải xạ ảnh cực tiểu của $M$, và $f:P\to P'$ là một cấu xạ của các phân giải. Khi đó $f$ là một đẳng cấu.
Đặc biệt, hai phân giải xạ ảnh cực tiểu của $M$ là đẳng cấu.

Đặt $\widetilde P_n=P_n$ với $n\ne-1$ và $\widetilde P_{-1}=M$; định nghĩa $\widetilde P'_n$ tương tự và đặt $f_{-1}=1_M$. Ta sẽ chứng minh bằng quy nạp bắt đầu từ $-1$ rằng $f_n:\widetilde P_n\to\widetilde P'_n$ là một đẳng cấu với mọi $n$. Điều này hiển nhiên với $n=-1$; giả sử rằng $f_n$ và $f_{n-1}$ là các đẳng cấu. Từ tính giao hoán của biểu đồ

$$
\begin{array}{ccc}
P_n & \xrightarrow{\ d_n\ } & P_{n-1}\\
{\scriptstyle f_n}\downarrow && \downarrow{\scriptstyle f_{n-1}}\\
P'_n & \xrightarrow{\ d'_n\ } & P'_{n-1}
\end{array}
$$

suy ra rằng $f_n$ cảm sinh một đẳng cấu $g_n$ từ $\operatorname{Ker}d_n$ lên $\operatorname{Ker}d'_n$. Khi đó từ tính giao hoán của biểu đồ

$$
\begin{array}{ccc}
P_{n+1} & \xrightarrow{\ \delta_{n+1}\ } & \operatorname{Ker}d_n\\
{\scriptstyle f_{n+1}}\downarrow && \downarrow{\scriptstyle g_n}\\
P'_{n+1} & \xrightarrow{\ \delta'_{n+1}\ } & \operatorname{Ker}d'_n
\end{array}
$$

và từ VIII, *loc. cit*., suy ra rằng $f_{n+1}$ là một đẳng cấu.

#### Hệ quả {#alg-x-s3-n6-cor-1 .statement}

*Cho $M$ là một $A$-môđun, $P$ và $P'$ là hai phân giải xạ ảnh của $M$; giả sử rằng $P$ là cực tiểu. Cho $f:P\to P'$ và $g:P'\to P$ là hai cấu xạ của các phân giải. Khi đó $f$ là đơn ánh, $g$ là toàn ánh, và $P'$ là tổng trực tiếp của các phức con $\operatorname{Im}f$ và $\operatorname{Ker}g$. Hơn nữa $\operatorname{Ker}g$ có đồng điều bằng không.*

Thật vậy, $\alpha=g\circ f$ là một tự đẳng cấu của $P$ (Mệnh đề 8). Đặt $\widetilde f=f\circ\alpha^{-1}$.

Ta có

$$
\operatorname{Im}\widetilde f=\operatorname{Im}f
\quad\text{và}\quad
g\circ\widetilde f=1_P,
$$

điều đó cho thấy rằng $P'=\operatorname{Im}\widetilde f\oplus\operatorname{Ker}g$. Vì dãy

$$
0\longrightarrow\operatorname{Ker}g\longrightarrow P'
\xrightarrow{\ g\ }P\longrightarrow0
$$

là khớp và $g$ là một đồng cấu, $\operatorname{Ker}g$ có đồng điều bằng không.

#### Mệnh đề 9 {#alg-x-s3-prop-9 .statement}

*Cho $M$ là một $A$-môđun và $(P,p)$ là một phân giải xạ ảnh của $M$. Ký hiệu $r$ là căn của $A$. Giả sử hoặc $P_n$ là một $A$-môđun hữu hạn sinh với mọi $n$, hoặc $r$ là lũy linh. Khi đó điều kiện cần và đủ để $(P,p)$ là cực tiểu là phức $(A/r)\otimes_A P$ có vi phân bằng không, nói cách khác là*

$$
d_{n+1}(P_{n+1})\subset rP_n\quad\text{với mọi }n\geq0.
$$

Giả sử rằng $(P,p)$ là cực tiểu. Theo VIII, *loc. cit.*, đồng cấu

$$
1\otimes\delta_n:(A/r)\otimes_A P_n\longrightarrow(A/r)\otimes_A\operatorname{Im}d_n
$$

là một đẳng cấu. Khi đó từ dãy khớp

$$
0\longrightarrow\operatorname{Im}d_{n+1}
\xrightarrow{\ j_n\ }P_n
\xrightarrow{\ \delta_n\ }\operatorname{Im}d_n
\longrightarrow0
$$

suy ra rằng đồng cấu $1 \otimes j_n : (A/r) \otimes_A \operatorname{Im} d_{n+1} \to (A/r) \otimes_A P_n$ bằng không; vì $d_{n+1} = j_n \circ \delta_{n+1}$, ta suy ra rằng $1_{A/r} \otimes d_{n+1} = 0$ với $n \geqslant 0$.

Ngược lại, giả sử rằng với mọi $n \geqslant 1$, $1 \otimes d_n$ bằng không, nói cách khác là $\operatorname{Im} d_n = \operatorname{Ker} d_{n-1}$ được chứa trong $rP_{n-1}$. Vì $\delta_{n-1}$ là toàn ánh, theo VIII, loc. cit. suy ra rằng $\delta_{n-1}$ là một bao xạ ảnh với $n \geqslant 1$, do đó $(P, p)$ là cực tiểu.

#### Mệnh đề 10 {#alg-x-s3-prop-10 .statement}

*Giả sử rằng A là một vành địa phương Noether trái, và cho M là một A-môđun hữu hạn sinh. Khi đó M có một phân giải cực tiểu $(P, p)$; với mọi $n \geqslant 0$, $P_n$ là một môđun tự do sinh hữu hạn.*

Thật vậy, trong phép dựng đã thực hiện ở No. 5 (p. 53), nhờ VIII, loc. cit., có thể lấy $(L_0, p)$ là một bao xạ ảnh của M, và lấy $L_{n+1}$ là một bao xạ ảnh của $\operatorname{Ker} d_n$. Phân giải thu được như vậy khi đó là cực tiểu.

*Nhận xét. -- 1) Gọi m là iđêan cực đại của A và đặt $k = A/m$. Gọi P là một phân giải xạ ảnh cực tiểu của M, và đặt $b_n = \dim_k (k \otimes_A P_n)$. Khi đó $P_n$ là một A-môđun tự do hạng $b_n$. Từ hệ quả của Mệnh đề 8 suy ra rằng đối với mọi phân giải xạ ảnh khác $P'$ của M, ta có $\dim_k (k \otimes_A P'_n) \geqslant b_n$, và đẳng thức xảy ra khi và chỉ khi $P'$ là cực tiểu.

2) Theo Mệnh đề 9, $b_n$ là chiều trên $k$ của $H_n(k \otimes_A P)$, *nói cách khác là của $\operatorname{Tor}_n^A(k, M)$*. Nó cũng là chiều trên $k$ của $\operatorname{Ext}_A^n(M, k)$ (*x. X, p. 103, Nhận xét 3*).

### 7. Các phân giải phân bậc

Trong số này, giả thiết rằng vành A được trang bị một phân bậc $(A_n)_{n \in \mathbf{Z}}$, sao cho $A_n = 0$ với $n < 0$. Một A-môđun phân bậc M được gọi là *bị chặn dưới* nếu $M_n = 0$ với $n$ đủ nhỏ; mọi A-môđun phân bậc kiểu hữu hạn đều bị chặn dưới.

#### Proposition 11 {#alg-x-s3-prop-11 .statement}

*Nếu M là một A-môđun phân bậc bị chặn dưới (tương ứng nếu M là một A-môđun phân bậc kiểu hữu hạn và nếu A là Noether trái), thì tồn tại một dãy khớp các A-môđun phân bậc không bị chặn về bên trái*

$$
\cdots \longrightarrow L_n \xrightarrow{d_n} L_{n-1} \longrightarrow \cdots \longrightarrow L_1 \xrightarrow{d_1} L_0 \xrightarrow{d_0} M \longrightarrow 0
$$

*trong đó các $L_i$ là phân bậc tự do và bị chặn dưới (tương ứng phân bậc tự do và kiểu hữu hạn), và trong đó các $d_i$ là các đồng cấu phân bậc bậc 0.*

Nếu N là một A-môđun phân bậc bị chặn dưới (tương ứng và kiểu hữu hạn trên A noether), thì tồn tại một A-môđun tự do phân bậc bị chặn dưới (tương ứng và kiểu hữu hạn) L và một đồng cấu phân bậc toàn ánh $L \to N$ (II, p. 167, *Nhận xét 3*).

Giả sử như vậy đã cho một dãy khớp các A-môđun phân bậc và các đồng cấu phân bậc bậc 0

$$
L_n \xrightarrow{d_n} L_{n-1} \longrightarrow \cdots \longrightarrow L_0 \xrightarrow{d_0} M \longrightarrow 0,
$$

trong đó các $L_i, i = 0, \ldots, n$, là phân bậc tự do và bị chặn dưới (tương ứng phân bậc tự do và kiểu hữu hạn). Khi đó $N = \mathrm{Ker}\, d_n$ bị chặn dưới (tương ứng kiểu hữu hạn); vì thế tồn tại một A-môđun tự do phân bậc bị chặn dưới (tương ứng một A-môđun tự do phân bậc kiểu hữu hạn) $L_{n+1}$ và một đồng cấu phân bậc $d_{n+1} : L_{n+1} \to L_n$ bậc 0, sao cho $\mathrm{Im}\, d_{n+1} = N$; dãy

$$
L_{n+1} \xrightarrow{d_{n+1}} L_n \xrightarrow{d_n} L_{n-1} \longrightarrow \cdots \longrightarrow L_0 \xrightarrow{d_0} M \longrightarrow 0
$$

khi đó là khớp. Mệnh đề do đó suy ra từ điều trước bởi quy nạp theo $n$.

### 8. Phân giải tiêu chuẩn

Trong số này, giả sử rằng vành $A$ là một đại số (kết hợp và có đơn vị) trên một vành giao hoán $k$. Với $n \geqslant 0$, gọi $B_n$ là tích tenxơ trên $k$ của $(n + 2)$ môđun đều bằng $A$. Nó được xét như một $(A, A)$-song môđun bằng cách trang bị cho nó cấu trúc A-môđun trái (tương ứng phải) suy ra từ cấu trúc A-môđun trái (tương ứng phải) của nhân tử thứ nhất (tương ứng của nhân tử cuối cùng) của tích tenxơ.

Với $n \geqslant 1$, định nghĩa các đồng cấu song môđun $d_n^i$ (với $0 \leqslant i \leqslant n$) và $d_n$ từ $B_n$ vào $B_{n-1}$ bởi các công thức:

$$
d_n^i(x_0 \otimes \ldots \otimes x_{n+1}) = x_0 \otimes \ldots \otimes x_i\, x_{i+1} \otimes \ldots \otimes x_{n+1}, \quad 0 \leqslant i \leqslant n,
$$
$$
d_n = \sum_{i=0}^n (-1)^i d_n^i.
$$

Hiển nhiên là
$$
d_{n-1}^i \circ d_n^j = d_{n-1}^{j-1} \circ d_n^i \quad \text{for} \quad i < j
$$
và do đó
$$
d_{n-1} \circ d_n = \sum_{0 \leqslant i < j \leqslant n} (-1)^{i+j} d_{n-1}^i \circ d_n^j + \sum_{0 \leqslant j \leqslant i \leqslant n-1} (-1)^{i+j} d_{n-1}^i \circ d_n^j = 0.
$$

Do đó, nếu đặt $B_n = 0$ với $n < 0$ và $d_n = 0$ với $n \leqslant 0$, thì dãy $(B_n, d_n)$ xác định một phức các $(A, A)$-song môđun (X, p. 43), sẽ được ký hiệu là $B(A)$. Với mọi A-môđun trái $M$, gọi $B(A, M)$ là phức tạo bởi các $B_n \otimes_A M$ và các $d_n \otimes 1_M$, \* nói cách khác là phức tích tenxơ $B(A) \otimes_A M *$; nó là một phức các A-môđun trái.

Định nghĩa một ánh xạ A-tuyến tính $\varepsilon_M$ từ $B_0(A, M) = (A \otimes_k A) \otimes_A M$ vào $M$ bởi công thức $\varepsilon_M(a \otimes b \otimes m) = abm$ với $a, b \in A, m \in M$. Ta có $\varepsilon_M \circ d_1 = 0$, do đó đồng cấu phân bậc $\overline{\varepsilon}_M : B(A, M) \to M$, trùng với $\varepsilon_M$ ở bậc 0, là một cấu xạ của các phức các A-môđun.

#### Mệnh đề 12 {#alg-x-s3-prop-12 .statement}

Ánh xạ $\overline{\varepsilon}_M : B(A, M) \to M$ là một đồng luân cấu của các phức $k$-môđun. Đặc biệt, phức $B(A, M)$ tách trên $k$, và $(B(A, M), \overline{\varepsilon}_M)$ là một phân giải trái của A-môđun $M$.

Với $n \geqslant 0$, ta định nghĩa một ánh xạ $k$-tuyến tính $s_n : B_n \to B_{n+1}$ bởi công thức:

$$
s_n(x_0 \otimes \ldots \otimes x_{n+1}) = 1 \otimes x_0 \otimes \ldots \otimes x_{n+1} \quad \text{với } x_0, \ldots, x_{n+1} \in A .
$$

Đây là một đồng cấu của các A-môđun phải, thỏa mãn các đẳng thức:

$$
d_{n+1}^i \circ s_n = s_{n-1} \circ d_n^{i-1} \quad \text{với } n \geqslant 1 , \quad 1 \leqslant i \leqslant n + 1 ,
$$
$$
d_{n+1}^0 \circ s_n = 1_{B_n} \qquad \text{với } n \geqslant 1 ,
$$

và do đó ta có

(16)
$$
d_{n+1} \circ s_n + s_{n-1} \circ d_n = 1_{B_n} \quad \text{với } n \geqslant 1 .
$$

Hơn nữa, ta có

(17)
$$
d_1 \circ s_0(x_0 \otimes x_1) = x_0 \otimes x_1 - 1 \otimes x_0 x_1 \quad \text{với } x_0, x_1 \in A .
$$

Ký hiệu $\eta : A \to A \otimes_k A$ là ánh xạ được định nghĩa bởi $\eta(a) = 1 \otimes a$, và $\overline{\eta} : A \to B(A)$ là cấu xạ của các phức trùng với $\eta$ ở bậc 0. Rõ ràng $\overline{\varepsilon}_A \circ \overline{\eta} = 1_A$; các công thức (16) và (17) cho thấy rằng $d \circ s + s \circ d = 1_{B(A)} - \overline{\eta} \circ \overline{\varepsilon}_A$. Đặt $\overline{\eta}_M = \overline{\eta} \otimes 1_M$, $d_M = d \otimes 1_M$ và $s_M = s \otimes 1_M$, ta suy ra rằng $\overline{\varepsilon}_M \circ \overline{\eta}_M = 1_M$ và $d_M \circ s_M + s_M \circ d_M = 1_{B(A,M)} - \overline{\eta}_M \circ \overline{\varepsilon}_M$. Nói cách khác, (X, p. 33, Định nghĩa 5), $\overline{\varepsilon}_M$ là một đồng luân cấu của các phức $k$-môđun. Các khẳng định khác của mệnh đề suy ra ngay từ điều này.

#### Định nghĩa 3 {#alg-x-s3-def-3 .statement}

Phân giải trái $(B(A, M), \overline{\varepsilon}_M)$ của $M$ được gọi là phân giải tiêu chuẩn của A-môđun $M$.

Nếu $A$ và $M$ là các $k$-môđun xạ ảnh (resp. tự do, resp. phẳng), thì phân giải tiêu chuẩn $B(A, M)$ là một phân giải xạ ảnh (resp. tự do, resp. phẳng) của $M$.

### 9. Phân giải và các nhóm Grothendieck

Nếu $\mathcal{C}$ là một tập hợp các lớp các A-môđun, ta sẽ nói rằng một phân giải trái $(P, p)$ bị chặn kiểu $\mathcal{C}$ nếu phức $P$ bị chặn kiểu $\mathcal{C}$ (X, p. 41).

#### Định lý 1 {#alg-x-s3-thm-1 .statement}

Cho $\mathcal{C}_0$ và $\mathcal{C}$ là hai lớp các tập hợp môđun $A$ cộng tính và khớp trái sao cho $\mathcal{C}_0 \subset \mathcal{C}$ và mọi $A$-môđun thuộc kiểu $\mathcal{C}$ đều có một phân giải trái hữu hạn thuộc kiểu $\mathcal{C}_0$. Khi đó đồng cấu $\alpha : K(\mathcal{C}_0) \to K(\mathcal{C})$ suy ra từ bao hàm của $\mathcal{C}_0$ trong $\mathcal{C}$ là song ánh; nếu $M$ là một $A$-môđun thuộc kiểu $\mathcal{C}$ và $P$ là một phân giải trái hữu hạn của $M$ thuộc kiểu $\mathcal{C}_0$, thì ta có $\alpha^{-1}([M]_{\mathcal{C}}) = \chi_{\mathcal{C}_0}(P)$ (X, p. 41, ví dụ 6).

#### Bổ đề 4 {#alg-x-s3-lem-4 .statement}

Cho $f : M' \to M$ là một đồng cấu của các $A$-môđun thuộc kiểu $\mathcal{C}$, và $p : P \to M$ là một phân giải trái hữu hạn của $P$ thuộc kiểu $\mathcal{C}_0$. Tồn tại một phân giải trái hữu hạn $p' : P' \to M'$ thuộc kiểu $\mathcal{C}_0$ và một cấu xạ phức $u : P' \to P$ sao cho $p \circ u = f \circ p'$.

Ta lập luận bằng quy nạp theo độ dài $n$ của $P$, mệnh đề là tầm thường khi độ dài này $< 0$. Xét ánh xạ $g : M' \times P_0 \to M$ sao cho

$$
g(x, r') = f(x) - p_0(r')
$$
với $x \in M', r' \in P_0$,

và hạt nhân của nó là $K$; $A$-môđun $K$ thuộc kiểu $\mathcal{C}$ vì $g$ là toàn ánh và $M' \times P_0$ và $M$ thuộc kiểu $\mathcal{C}$. Cho $h : P'_0 \to K$ là một đồng cấu toàn ánh, trong đó $P'_0$ thuộc kiểu $\mathcal{C}_0$; ký hiệu $p'_0 : P'_0 \to M'$ (tương ứng $u_0 : P'_0 \to P_0$) là đồng cấu hợp thành của $h$ với phép chiếu $K \to M$ (tương ứng $K \to P_0$); đồng cấu $p'_0$ là toàn ánh và ta có biểu đồ giao hoán

$$
\begin{array}{ccc}
P'_0 & \xrightarrow{u_0} & P_0 \\
p'_0 \downarrow & & \downarrow p_0 \\
M' & \xrightarrow{f} & M .
\end{array}
$$

Khi đó chỉ cần áp dụng giả thiết quy nạp cho đồng cấu

$$
\operatorname{Ker} p'_0 \to \operatorname{Ker} p_0
$$

suy ra từ $u_0$.

#### Bổ đề 5 {#alg-x-s3-lem-5 .statement}

Xét một biểu đồ giao hoán

$$
\begin{array}{ccc}
P' & \xrightarrow{u} & P \\
p' \downarrow & & \downarrow p \\
0 & \xrightarrow{f} & M \to M'' \to 0
\end{array}
$$

trong đó $(P, p)$ (tương ứng $(P', p')$) là một phân giải trái của $M$ (tương ứng $M'$), và trong đó hàng ngang dưới là một dãy khớp. Tồn tại một đồng cấu $p'' : \operatorname{Con}(u) \to M''$.

Thật vậy, dãy khớp (X, p. 37, mệnh đề 7)

$$
0 \to P \xrightarrow{\pi} \operatorname{Con}(u) \xrightarrow{\delta} P'(-1) \to 0
$$

cho một dãy đồng điều khớp

$$
\to H_n(P) \to H_n(\operatorname{Con}(u)) \to H_{n-1}(P') \to \cdots
$$
$$
\cdots \to H_1(\operatorname{Con}(u)) \to H_0(P') \xrightarrow{\hat{\partial}} H_0(P) \to H_0(\operatorname{Con}(u)) \to 0 .
$$

Theo X, p. 38, bổ đề 3 a), ta có $\partial = - H_0(u)$. Vì $H_n(P) = 0 = H_n(P')$ với $n > 0$ và $H_0(u) : H_0(P') \to H_0(P)$ được đồng nhất với $f : M' \to M$, ta kết luận rằng $H_n(\operatorname{Con}(u)) = 0$ với $n > 0$ và $H_0(\operatorname{Con}(u))$ đẳng cấu với $M''$, do đó bổ đề được chứng minh.

Bây giờ ta chứng minh định lý.

a) Cho M là một A-môđun kiểu $\mathcal{C}$. Với mọi phân giải trái bị chặn $(P, p)$ của M kiểu $\mathcal{C}_0$, phần tử $\chi_{\mathcal{C}_0}(P)$ của $K(\mathcal{C}_0)$ chỉ phụ thuộc vào M. Thật vậy, cho $(P_1, p_1)$ và $(P_2, p_2)$ là hai phân giải thuộc kiểu này. Xét phân giải
$$
(P_1 \times P_2, p_1 \times p_2)
$$
của A-môđun $M \times M$ và đồng cấu $\Delta : x \mapsto (x, x)$ từ M vào $M \times M$. Theo bổ đề 4, tồn tại một phân giải trái bị chặn $(Q, q)$ của M kiểu $\mathcal{C}_0$ và một biểu đồ giao hoán
$$
\begin{array}{ccc}
Q & \xrightarrow{u} & P_1 \times P_2 \\
q \downarrow & & \downarrow p_1 \times p_2 \\
M & \xrightarrow{\Delta} & M \times M ;
\end{array}
$$
từ đó ta suy ra một biểu đồ giao hoán
$$
\begin{array}{ccc}
Q & \xrightarrow{u \circ pr_i} & P_i \\
q \downarrow & & \downarrow p_i \\
M & \xrightarrow{1_M} & M , \quad i = 1, 2 .
\end{array}
$$
Theo bổ đề 5, Con $(u \circ pr_i)$ có đồng điều không, do đó $u \circ pr_i$ là một đồng cấu đồng điều và $\chi_{\mathcal{C}_0}(Q) = \chi_{\mathcal{C}_0}(P_i)$ (X, p. 41, mệnh đề 10); suy ra $\chi_{\mathcal{C}_0}(P_1) = \chi_{\mathcal{C}_0}(P_2)$ như đã thông báo.

b) Với mọi A-môđun M kiểu $\mathcal{C}$, đặt $\varphi(M) \in K(\mathcal{C}_0)$ là giá trị chung của các $\chi_{\mathcal{C}_0}(P)$ đối với mọi phân giải trái bị chặn P của M kiểu $\mathcal{C}_0$. Ta sẽ chỉ ra rằng hàm $\varphi : \mathcal{C} \to K(\mathcal{C}_0)$ là cộng tính. Vậy cho
$$
0 \to M' \xrightarrow{f} M \to M'' \to 0
$$
là một dãy khớp các A-môđun kiểu $\mathcal{C}$. Theo Bổ đề 4, tồn tại một biểu đồ giao hoán
$$
\begin{array}{ccc}
P' & \xrightarrow{u} & P \\
p' \downarrow & & \downarrow p \\
0 & \xrightarrow{f} & M \xrightarrow{g} M'' \to 0
\end{array}
$$
trong đó $(P, p)$ và $(P', p')$ là các phân giải trái bị chặn kiểu $\mathcal{C}_0$. Khi đó ta có
$$
\varphi(M) = \chi_{\mathcal{C}_0}(P) , \qquad \varphi(M') = \chi_{\mathcal{C}_0}(P')
$$
và theo Bổ đề 5
$$
\varphi(M'') = \chi_{\mathcal{C}_0}(\mathrm{Con}\,(u)) = \chi_{\mathcal{C}_0}(P) - \chi_{\mathcal{C}_0}(P') = \varphi(M) - \varphi(M') ;
$$
điều phải chứng minh.

c) Khi đó, cho $\beta : K(\mathscr{C}) \to K(\mathscr{C}_0)$ là đồng cấu sao cho, với các ký hiệu đứng trước, ta có $\beta([M]_{\mathscr{C}})=\chi_{\mathscr{C}_0}(P)$. Vì $p$ là một đồng cấu, ta có $\chi_{\mathscr{C}}(P)=[M]_{\mathscr{C}}$, do đó $\alpha\circ\beta([M]_{\mathscr{C}})=\alpha(\chi_{\mathscr{C}_0}(P))=\chi_{\mathscr{C}}(P)=[M]_{\mathscr{C}}$ và $\alpha\circ\beta=1_{K(\mathscr{C})}$. Nếu $M$ là kiểu $\mathscr{C}_0$, thì $(M,1_M)$ là một phân giải của $M$, do đó $\varphi(M)=[M]_{\mathscr{C}_0}$ và $\beta\circ\alpha=1_{K(\mathscr{C}_0)}$, điều này hoàn tất chứng minh.

Ta sẽ áp dụng định lý này cho các môđun có "chiều xạ ảnh hữu hạn" trong § 8 (X, p. 137).

## BÀI TẬP {#alg-x-s3-exercises}

Xem [bài tập của § 3](exercises/s3/).
