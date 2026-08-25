---
book: alg
book_title: Algebra
chapter: IV
chapter_title: POLYNOMIALS AND RATIONAL FRACTIONS
section: 4
section_title: Formal power series
lang: vi
source: alg-iv-vii
source_edition: 2003, Springer
book_pages: A IV.24-A IV.41, A IV.90-A IV.91
pdf_pages: 0033-0050, 0099-0100
extraction: ocr
subsections:
    - "no": 1
      title: Definition of formal power series. Order
      page: 24
      pdf_page: 33
    - "no": 2
      title: Topology on the set of formal power series. Summable families
      page: 25
      pdf_page: 34
    - "no": 3
      title: Substitutions
      page: 28
      pdf_page: 37
    - "no": 4
      title: Invertible formal power series
      page: 30
      pdf_page: 39
    - "no": 5
      title: Taylor's formula for formal power series
      page: 31
      pdf_page: 40
    - "no": 6
      title: Derivations in the algebra of formal power series
      page: 32
      pdf_page: 41
    - "no": 7
      title: The solution of equations in a formal power series ring
      page: 35
      pdf_page: 44
    - "no": 8
      title: Formal power series over an integral domain
      page: 38
      pdf_page: 47
    - "no": 9
      title: The field of fractions of the ring of formal power series in one indeterminate over a field
      page: 38
      pdf_page: 47
    - "no": 10
      title: Exponential and logarithm
      page: 39
      pdf_page: 48
statements: 23
exercises: 8
content_sha256: 3d6a59e0f46954a7ba86646adbaeac17bc92de882458f85452b767f410203d74
translated_from: content/en/alg/IV/04_s4_formal_power_series.md
source_content_sha256: ace628286fbf81aac624b68384ad96ad2fa47f69b828b87b90696e070f925f67
translation_model: gpt-5.4-mini
translation_run: translate-vi-1e020711
glossary_version: 34
glossary_terms_sha256: 093778be7a45a8cc8ee79b385dc8af6c84e91ca3c618158d9bd113c2bea322e2
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 4. CHUỖI LŨY THỪA HÌNH THỨC

### 1. Định nghĩa chuỗi lũy thừa hình thức. Cấp

Cho I là một tập hợp. Ta nhắc lại (III, p. 454 and 456) rằng đại số toàn phần của monoid $N^{(I)}$ trên A được gọi là *đại số của các chuỗi lũy thừa hình thức đối với các ẩn* $X_i \ (i \in I)$ (hay theo các ẩn $X_i$) *với hệ số trong* A. Nó được kí hiệu bởi $A[[X_i]]_{i \in I}$ hoặc $A[[((X_i)_{i \in I}]]$ hoặc cũng $A[[X]]$, khi kí hiệu X là họ $(X_i)_{i \in I}$: trong đoạn này ta chủ yếu dùng kí hiệu $A[[I]]$. Đôi khi tiện viết ảnh chính tắc trong $A[[I]]$ của phần tử i của I bằng một kí hiệu khác $X_i$, chẳng hạn $Y_i, Z_i, T_i, \ldots$; các quy ước dùng trong trường hợp này tương tự như đối với đa thức (IV, p. 1). Khi đó đại số $A[[I]]$ được kí hiệu bởi $A[[Y_i]]_{i \in I}$, hoặc $A[[Y]]$ v.v.

Khi I là một tập hữu hạn gồm p phần tử, ta cũng nói rằng $A[[I]]$ là một đại số chuỗi lũy thừa hình thức trong p ẩn. Với p cố định, các đại số này đều đẳng cấu với nhau. Một đại số chuỗi lũy thừa hình thức trong 1, 2, ... ẩn cũng sẽ được kí hiệu bởi $A[[X]]$, $A[[U, V]]$, ..., khi tập I của các chỉ số không được nêu rõ.

Một chuỗi lũy thừa hình thức u thường được viết $u = \sum_{v \in N^{(I)}} a_v X^v$ (cf. IV, p. 1).

Các $\alpha_v$ là các *hệ số* của $u$; có thể có vô hạn nhiều trong số chúng $\neq 0$. Các $a_v X^v$ được gọi là các *số hạng* của $u$; để u là một đa thức thì điều kiện cần và đủ là $u$ chỉ có hữu hạn số hạng $\neq 0$. Các số hạng $a_v X^v$ sao cho |ν| = p được gọi là các số hạng có bậc toàn phần p. Chuỗi lũy thừa hình thức $u_p = \sum_{|\nu|=p} \alpha_\nu X^\nu$ được gọi là *thành phần thuần nhất bậc* p của u (nó là một đa thức khi I hữu hạn); $u_0$ được đồng nhất với một phần tử của A cũng được gọi là *số hạng hằng* của u. Ta nói u là thuần nhất bậc p nếu $u = u_p$. Nếu $u, v \in \mathbf{A}[[\mathrm{I}]]$ và $w = uv$, ta có

(1)
$$
w_p = \sum_{q+r=p} u_q v_r
$$
với mọi số nguyên $p \geq 0$.

Ta nhắc lại (III, p. 456), rằng *cấp* $\omega(u)$ của một chuỗi lũy thừa hình thức $u \neq 0$ là số nguyên nhỏ nhất p sao cho $u_p \neq 0$. Ta sẽ quy ước thêm vào Z một phần tử viết là $\infty$ và mở rộng quan hệ thứ tự và phép cộng từ Z sang $Z \cup \{\infty\}$ theo các quy ước
$$
n < \infty,\quad \infty + \infty = \infty,\quad \infty + n = n + \infty = \infty
$$
với mọi $n \in Z$; ta cũng đặt $\omega(0) = \infty$. Với các quy ước này ta có các hệ thức
$$
\begin{align*}
\omega(u+v) &\geq \inf(\omega(u), \omega(v)), \\
\omega(u+v) &= \inf(\omega(u), \omega(v)) \text{ nếu } \omega(u) \neq \omega(v), \\
\omega(uv) &\geq \omega(u) + \omega(v),
\end{align*}
$$
cho mọi chuỗi lũy thừa hình thức $u$ và $v$ trong $\mathbf{A}[[\mathrm{I}]]$.

Ta nhắc lại (III, p. 457) rằng với mọi tập con J của I ta đồng nhất $\mathbf{A}[[\mathrm{I}]]$ với $\mathbf{A}[[\mathrm{I}-J]] [[\mathrm{J}]]$, điều này cho phép định nghĩa cấp $\omega_J(u)$ của một chuỗi lũy thừa hình thức đối với các $X_j$ ($j \in J$), thành phần thuần nhất của $u$ đối với các $X_j$ ($j \in J$) v.v.

Cho $\varphi$ là một đồng cấu của A vào một vành B. Ta mở rộng $\varphi$ thành một đồng cấu $\overline{\varphi}$ của $\mathbf{A}[[\mathrm{I}]]$ vào $B[[\mathrm{I}]]$ bằng cách cho mỗi chuỗi lũy thừa hình thức $u = \sum \alpha_\nu X^\nu$ tương ứng với chuỗi lũy thừa hình thức $\sum \varphi(\alpha_\nu) X^\nu$; ta nói rằng chuỗi sau được thu được bằng cách *áp dụng* $\varphi$ *vào các hệ số của chuỗi lũy thừa hình thức* u. Đôi khi ta viết $^\varphi u$ để chỉ $\overline{\varphi}(u)$.

Đặc biệt, nếu A là một vành con của B và $\varphi$ là đơn ánh chính tắc của A vào B, thì đồng cấu $\overline{\varphi}$ của $\mathbf{A}[[\mathrm{I}]]$ vào $B[[\mathrm{I}]]$ là đơn ánh; nói chung ta sẽ đồng nhất $\mathbf{A}[[\mathrm{I}]]$ với một vành con của $B[[\mathrm{I}]]$ nhờ $\overline{\varphi}$.

### 2. Tôpô trên tập hợp các chuỗi lũy thừa hình thức. Các họ khả tổng

Theo định nghĩa $\mathbf{A}[[\mathrm{I}]]$ không gì khác hơn là tập hợp tích $\mathbf{A}^{N^{(I)}}$. Trừ khi có nói rõ điều ngược lại, ta sẽ trang bị cho A tôpô rời rạc và cho $\mathbf{A}[[\mathrm{I}]]$ tôpô tích (Gen. Top. I, p. 31 f.) mà ta sẽ gọi là tôpô chính tắc. Được trang bị phép cộng và tôpô rời rạc, $A$ là một nhóm tôpô tách biệt và đầy đủ; do đó với phép cộng $A[[I]]$ là một nhóm tôpô tách biệt và đầy đủ (Gen. Top., III, p. 238 and 242 and Gen. Top., II, p. 187). Hơn nữa đại số $A[(X_i)_{i \in I}]$ của các đa thức là trù mật trong $A[[I]]$ (Gen. Top., III p. 238, Mệnh đề 25) và vì thế ta có thể xem $A[[I]]$ như là phần đầy đủ hóa của $A[(X_i)_{i \in I}]$.

Với mỗi $\beta \in \mathbf{N}^{(I)}$ hãy đặt $S_\beta$ là tập hợp các đa chỉ số $v$ sao cho $v \leq \beta$ và đặt $a_\beta$ là tập hợp các chuỗi lũy thừa hình thức $u = \sum \alpha_v X^v$ sao cho $a_v = 0$ với $v \in S_\beta$. Rõ ràng $S_\beta$ là một tập con hữu hạn của $\mathbf{N}^{(I)}$, và mọi tập con hữu hạn của $\mathbf{N}^{(I)}$ đều được chứa trong một tập hợp dạng $S_\beta$. Suy ra họ $(a_\beta)_{\beta \in \mathbf{N}^{(I)}}$ là một hệ cơ bản các lân cận của 0 trong $A[[I]]$. Các tập hợp $a_\beta$ là các iđêan trong $A[[I]]$, do đó (Gen. Top., III, p. 275) $A[[I]]$ là một vành tôpô.

#### Bổ đề 1 {#alg-iv-s4-lem-1 .statement}

Cho $L$ là một tập vô hạn và $(u_\lambda)_{\lambda \in L}$ là một họ các phần tử của $A[[I]]$, và đặt $u_\lambda = \sum \alpha_{\lambda,v} X^v$ với $\lambda \in L$. Khi đó các điều kiện sau là tương đương:
(i) Họ $(u_\lambda)_{\lambda \in L}$ khả tổng (Gen. Top., III, p. 262) trong $A[[I]]$.
(ii) Ta có $\lim u_\lambda = 0$, lấy theo *bộ lọc* các phần bù của các tập con hữu hạn của $L$.
(iii) Với mọi $v \in \mathbf{N}^{(I)}$ ta có $\alpha_{\lambda,v} = 0$ trừ ra một số chỉ số $\lambda \in L$ *hữu hạn*.

Khi các điều kiện này thỏa mãn, chuỗi $u = \sum_{\lambda \in L} u_\lambda$ bằng $\sum \alpha_v X^v$ với $a_v = \sum_{\lambda \in L} \alpha_{\lambda,v}$ đối với mỗi $v \in \mathbf{N}^{(I)}$.

Sự tương đương của (i) và (ii) suy ra từ Hệ quả 2 của Gen. Top., III, p. 263.
Sự tương đương của (ii) và (iii) suy ra từ các tính chất của giới hạn trong một không gian tích (Gen. Top., I, p. 55, Hệ quả 1).
Khẳng định cuối cùng suy ra từ Mệnh đề 4 của Gen. Top., III, p. 266.

Hãy nêu một vài ví dụ về các họ khả tổng.

a) Cho $u \in A[[I]]$ và cho $a_v$ là hệ số của $X^v$ trong $u$. Khi đó họ $(\alpha_v X^v)_{v \in \mathbf{N}^{(I)}}$ là khả tổng, với tổng $u$ (điều đó biện minh cho việc viết $u = \sum \alpha_v X^v$).

b) Cho $u \in A[[I]]$; với mọi số nguyên $p \geq 0$ đặt $u_p$ là thành phần thuần nhất bậc $p$ của $u$. Khi đó họ $(u_p)_{p \geq 0}$ là khả tổng và ta có $u = \sum_{p \geq 0} u_p$.

c) Cho $(u_\lambda)_{\lambda \in L}$ là một họ các phần tử của $A[[I]]$ và giả sử rằng với mọi số nguyên $n \geq 0$ tập hợp các $\lambda \in L$ sao cho $\omega(u_\lambda) < n$ là hữu hạn. Khi đó họ $(u_\lambda)_{\lambda \in L}$ là khả tổng.

#### Nhận xét {#alg-iv-s4-n2-rem-1 .statement}

— Giả sử rằng $I$ là *hữu hạn*. Với mọi số nguyên $n \geq 0$ đặt $b_n$ là tập hợp các chuỗi lũy thừa hình thức $u \in A[[I]]$ sao cho $\omega(u) \geq n$. Dãy $(b_n)_{n \geq 0}$ là một hệ cơ bản các lân cận của 0 trong $\mathbf{A}[[\mathbf{I}]]$. Do đó một họ các phần tử $u_\lambda$ của $\mathbf{A}[[\mathbf{I}]]$ ($\lambda \in L$) là khả tổng khi và chỉ khi với mọi $n \in \mathbf{N}$ tập hợp các $\mathbf{A} \in L$ sao cho $\omega(u_\lambda) < n$ là hữu hạn.

#### Mệnh đề 1 {#alg-iv-s4-prop-1 .statement}

*Cho* $(u,)_{\mu \in \mathcal{J}}$ *và* $(v_\mu)_{\mu \in \mathcal{J}}$ *là hai họ khả tổng của các phần tử của* $\mathbf{A}[[\mathbf{I}]]$. *Khi đó họ* $(u_\lambda v_\mu)_{(\lambda, \mu) \in \mathcal{J} \times M}$ *là khả tổng và ta có*

$$
\sum_{(\lambda, \mu) \in L \times M} u_\lambda v_\mu = \left( \sum_{\lambda \in L} u_\lambda \right) \left( \sum_{\mu \in M} v_\mu \right)
$$

Cho $(\alpha_{\lambda, \nu})_{\nu \in \mathbf{N}^{(1)}}$ (resp. $(\beta_{\mu, \nu})_{\nu \in \mathbf{N}^{(1)}}$) là họ các hệ số của $u_\lambda$ (resp. $v_\nu$). Với mỗi $\nu \in \mathbf{N}^{(1)}$ chỉ tồn tại một số hữu hạn các cặp $(\nu_1, \nu_2) \in \mathbf{N}^{(1)} \times \mathbf{N}^{(1)}$ sao cho $\nu_1 + \nu_2 = \nu$, do đó chỉ có một số hữu hạn các cặp $(\lambda, \mu) \in L \times M$ sao cho hệ số của $X^\nu$ trong $u_\lambda v_\mu$ khác $0$. Vì thế họ $(u_\lambda v_\mu)_{(\lambda, \mu) \in L \times \mathcal{J}}$ là khả tổng. Nay công thức (2) suy ra từ tính kết hợp của tổng (Gen. Top., III, p. 265, công thức (2)).

Trong $\mathbf{A}[[\mathbf{I}]]$ phép nhân là một luật hợp thành kết hợp và giao hoán. Vì vậy ta có thể nói về một *họ nhân được* các phần tử của $\mathbf{A}[[\mathbf{I}]]$ và về *tích* của một họ nhân được (Gen. Top., III, p. 262, nhận xét 3).

#### Mệnh đề 2 {#alg-iv-s4-prop-2 .statement}

*Cho* $(u_\lambda)_\lambda$ *là một họ khả tổng của các phần tử của* $\mathbf{A}[[\mathbf{I}]]$.
(i) *Họ* $(1 + u_\lambda)_\lambda$ *là nhân được*.
(ii) *Cho* $\mathfrak{T}$ *là tập hợp tất cả các tập con hữu hạn của* $L$. *Với mọi* $M \in \mathcal{S}$ *đặt* $u_M = \prod_{\lambda \in M} u_\lambda$. *Khi đó họ* $(u_M)_{M \in \mathfrak{T}}$ *là khả tổng và ta có*

$$
\sum_{M \in \mathfrak{T}} u_M = \prod_{\lambda \in L} (1 + u_\lambda).
$$

Đặt các iđêan $\mathfrak{a}_\beta$ như ở đầu số này, và cho $\beta \in \mathbf{N}^{(1)}$. Tồn tại một tập con hữu hạn $L_0$ của $L$ sao cho $u_\lambda \in \mathfrak{a}_\beta$ với $\lambda \notin L_0$. Khi đó với mọi $M \in \mathcal{S}$ sao cho $M \not\subset L_0$ ta có $u_M \in \mathfrak{a}_\beta$. Suy ra họ $(u_M)_{M \in \mathfrak{T}}$ khả tổng. Mặt khác, với mọi tập con hữu hạn $M_0$ của $L$ ta có

$$
\sum_{M \subset M_0} u_M = \prod_{\lambda \in M_0} (1 + u_\lambda).
$$

Xét theo tập hợp có thứ tự lọc $\mathfrak{T}$, vế trái có giới hạn là $\sum_{M \in \mathfrak{T}} u_M$. Do đó vế phải có giới hạn là $\sum_{M \in \mathfrak{T}} u_M$, điều này chứng minh đồng thời (i) và (ii).

#### Mệnh đề 3 {#alg-iv-s4-prop-3 .statement}

*Cho* $u = \sum a_\nu X^\nu \in \mathbf{A}[[\mathbf{I}]]$ *và* $m$ *là một số nguyên* $> 0$. *Với mọi* $n \in \mathbf{N}$ *gọi* $(\alpha_{\nu, n})_{\nu \in \mathbf{N}^{(1)}}$ *là họ các hệ số của* $u^n$. *Nếu* $\alpha_0^m = 0$, *thì* $\alpha_{\nu, n} = 0$ *với* $n \geq |\nu| + m$.

Cho $v \in \mathbf{N}^{(1)}$ và $n \in \mathbf{N}$. Ta có

$$
\alpha_{v,n} = \sum_{v(1) + \cdots + v(n) = v} \alpha_{v(1)} \cdots \alpha_{v(n)} .
$$

Nếu $n \geq |v| + m$ và $v(1) + \cdots + v(n) = v$, ta có $|v(1)| + \cdots + |v(n)| \leq n - m$. Do đó ta có $v(r) = 0$ và vì thế $\alpha_{v(r)} = a_r$, đối với ít nhất $m$ giá trị phân biệt của $r$; suy ra $\alpha_{v(1)} \cdots \alpha_{v(n)} = 0$, do đó có kết quả.

#### Hệ quả {#alg-iv-s4-n2-cor-1 .statement}

— Cho $u \in A[[I]]$; để $\lim_{n \to \infty} u^n = 0$ thì cần và đủ rằng số hạng hằng của $u$ phải là lũy linh.

Gọi $a_0$ là số hạng hằng của $u$. Số hạng hằng của $u^n$ là $\alpha_0^n$, do đó điều kiện đã nêu là cần thiết; nó đủ theo Mệnh đề 3.

### 3. Phép thế

Cho $E$ là một $A$-đại số. Một tôpô trên $E$ được gọi là tuyến tính nếu nó bất biến dưới phép tịnh tiến và nếu tồn tại một hệ cơ bản các lân cận của 0 gồm các iđêan của $E$ (Gen. Top., III, p. 223). Khi đó tôpô trên $E$ tương thích với cấu trúc $A$-đại số của nó (khi $A$ mang tôpô rời rạc). Một $A$-đại số có tôpô tuyến tính được gọi là một $A$-đại số tôpô tuyến tính.

#### Mệnh đề 4 {#alg-iv-s4-prop-4 .statement}

— Cho $I$ là một tập hợp và $E$ là một $A$-đại số kết hợp, giao hoán, có đơn vị, được tôpô tuyến tính, tách biệt đầy đủ.

(i) Cho $\varphi$ là một đồng cấu liên tục của $A[[I]]$ vào $E$ và $x_i = \varphi(X_i)$. Khi đó:
(a) với mọi $i \in I$, $x_i^n$ tiến tới 0 khi $n$ tiến tới $+ \infty$;
(b) nếu $I$ là vô hạn, thì $x_i$ tiến tới 0 theo bộ lọc của các phần bù của các tập con hữu hạn của $I$.

(ii) Cho $x = (x_i)_i$, $_I$ là một họ các phần tử của $E$ thỏa mãn a) và b) của (i). Khi đó tồn tại một và chỉ một đồng cấu liên tục có đơn vị $\varphi$ của $A[[I]]$ vào $E$ sao cho $\varphi(X_i) = x_i$ với mọi $i \in I$.

Với mọi $i \in I$, rõ ràng $X_i^n$ tiến tới 0 trong $A[[I]]$ khi $n$ tiến tới $+ \infty$; mặt khác khi $I$ là vô hạn, $X_i$ tiến tới 0 theo bộ lọc của các phần bù của các tập con hữu hạn của $I$. Điều này chứng minh (i).

Cho $(x_i)_{i \in I}$ là một họ các phần tử của $E$ thỏa mãn các điều kiện a) và b) của (i), cho $\psi$ là đồng cấu $u \mapsto u((x_i)_{i \in I})$ của $A[(X_i)_{i \in I}]$ vào $E$, và cho $V$ là một lân cận của 0 của $E$ đồng thời là một iđêan của $E$. Theo b) tồn tại một tập con hữu hạn $J$ của $I$ sao cho $x_i \in V$ với mọi $i \in I - J$. Tiếp theo, theo a) tồn tại một số nguyên $n \geq 0$ sao cho $x_i^n \in V$ với mọi $i \in J$. Cho $\beta$ là phần tử của $\mathbf{N}^{(I)}$ sao cho $\beta_i = n - 1$ với $i \in J$ và $\beta_i = 0$ với $i \in I - J$. Nếu ta định nghĩa iđêan $a_\beta$ của $A[[I]]$ như ở đầu của No. 2 (IV, p. 26), thì

$$
u \in A[(X_i)_{i \in I}] \cap a_\beta \Rightarrow \psi(u) \in V
$$

Điều này cho thấy $\psi$ là liên tục nếu ta trang bị cho $A[(X_i)_{i \in I}]$ tôpô cảm sinh bởi tôpô của $A[[I]]$. Vì $E$ tách biệt và đầy đủ, $\psi$ mở rộng thành một đồng cấu có đơn vị liên tục $\varphi$ của $A[[I]]$ vào $E$. Ta có $\varphi(X_i) = \psi(X_i) = x_i$ với mọi $i \in I$. Cuối cùng, cho $\varphi'$ là một đồng cấu có đơn vị liên tục của $A[[I]]$ vào $E$ sao cho $\varphi'(X_i) = x_i$. Ta có $\varphi'(u) = \varphi(u)$ với mọi $u \in A[(X_i)_{i \in I}]$, do đó $\varphi' = \varphi$ vì $A[(X_i)_{i \in I}]$ trù mật trong $A[[I]]$.

Giữ nguyên ký hiệu ở trên. Nếu $u \in A[[I]]$, ảnh của $u$ qua $\varphi$ được ký hiệu là $u(x)$ hoặc $u((x_i)_{i \in I})$ (hoặc cũng là $u(x_1, ..., x_n)$ nếu $I = (1, 2, ..., n)$) và được gọi là phần tử của $E$ thu được bằng phép thế $x_i$ cho $X_i$ trong $u$, hay là giá trị của $u$ tại các giá trị $x_i$ của $X_i$ hoặc cũng là giá trị của $u$ với $X_i = x_i$. Đặc biệt ta có $u = u((X_i)_{i \in I})$.

Cho $E'$ là một $A$-đại số kết hợp, giao hoán và có đơn vị, được tôpô tuyến tính, tách biệt và đầy đủ. Cho $\lambda$ là một đồng cấu có đơn vị liên tục từ $E$ vào $E'$, và $(x_i)_{i \in I}$ là một họ các phần tử của $E$ thỏa mãn các điều kiện $a)$ và $b)$ của Mệnh đề 4 (IV, p. 28). Họ $(\lambda(x_i))_{i \in I}$ thỏa mãn cùng các điều kiện $a)$ và $b)$. Với mọi $u \in A[[I]]$ ta có

$$
\lambda(u((x_i)_{i \in I})) = u((\lambda(x_i))_{i \in I}),
$$

vì ánh xạ $u \mapsto A(u((x_i)_{i \in I}))$ là một đồng cấu có đơn vị liên tục của $A[[I]]$ vào $E'$ biến $X_i$ thành $\lambda(x_i)$ với mọi $i \in I$.

#### Mệnh đề 5 {#alg-iv-s4-prop-5 .statement}

Nếu $J$ và $K$ là hai tập hợp, ta ký hiệu bởi $A_{J, K}$ tập hợp tất cả các họ $(g_j)_{j \in J}$ thỏa mãn các điều kiện sau:
(i) với mọi $j \in J$, $g_j$ là một phần tử của $A[[K]]$ có số hạng tự do lũy linh;
(ii) nếu $J$ là vô hạn, thì $g_j$ tiến về 0 theo bộ lọc các phần bù của các tập con hữu hạn của $J$.

Chú ý rằng nếu $J$ là hữu hạn, mọi họ chuỗi lũy thừa hình thức $(g_j)_{j \in J}$ không có số hạng tự do trong $A[[K]]$ đều thuộc $A_{J, K}$.

Cho $(g_j)_{j \in J}$ thuộc $A_{J, K}$. Theo Hệ quả của Mệnh đề 3 (IV, p. 28) ta có $\lim_{n \to \infty} g_j^n = 0$ với mọi $j \in J$. Cho $f \in A[[J]]$; ta có thể thay $g_j$ cho biến có chỉ số $j$ trong $f$ và thu được một chuỗi lũy thừa hình thức $f((g_j)_{j \in J})$ thuộc $A[[K]]$. Hơn nữa, ánh xạ $f \mapsto f((g_j)_{j \in J})$ là một đồng cấu liên tục của các $A$-đại số $A[[J]]$ vào $A[[K]]$.

Đặc biệt nếu $J = (1, ..., p)$ và $f \in A[[X_1, ..., X_p]]$, ta có thể thay cho mỗi $X_j$ một chuỗi lũy thừa hình thức $g_j \in A[[K]]$ không có số hạng tự do; kết quả của phép thế này được viết $f(g_1, ..., g_p)$.

Cho $x = (x_k)_{k \in K}$ là một họ các phần tử của $E$ thỏa mãn các điều kiện $a)$ và $b)$ của Mệnh đề 4 (IV, p. 28). Áp dụng (3), lấy cho $A$ đồng cấu $u \mapsto u(x)$ của $A[[K]]$ vào $E$; ta được

$$
f((g_j)_{j \in J})(x) = f((g_j(x))_{j \in J}).
$$

Cho $f = (f_i)_{i \in I} \in (A[[J]])^I$ và $g = (g_j)_{j \in J} \in A_{J, K}$. Ta ký hiệu bởi $f(g)$ hay $f \circ g$ phần tử $(f_i((g_j),_{\epsilon_J}))_{i \in I}$ của $(A[[K]])^I$. Nếu $f \in A_{I, J}$, ta có $f \circ g \in A_{,,K}$ vì ánh xạ $f \mapsto f((g_j)_{i, J})$ của $A[[I]]$ vào $A[[K]]$ là liên tục.

Cho $f \in (A[[J]])^I$, $g \in A_{J, K}$, $h \in A_{K, L}$. Khi đó $g \circ h \in A_{J, L}$ và theo (4), ta có
$$
(f \circ g) \circ h = f \circ (g \circ h).
$$

### 4. Chuỗi lũy thừa hình thức khả nghịch

— *Trong vành $A[[T]]$ của các chuỗi lũy thừa hình thức theo một ẩn, đa thức $1 - T$ khả nghịch, và ta có* $(1 - T)^{-1} = \sum_{n=0}^m T^n$.

Khi đó
$$
(1 - T) \left( \sum_{n=0}^\infty T^n \right) = \sum_{n=0}^\infty T^n - \sum_{n=0}^\infty T^{n+1} = 1.
$$

#### Mệnh đề 6 {#alg-iv-s4-prop-6 .statement}

— *Cho $u \in A[[I]]$; khi đó để $u$ khả nghịch trong $A[[T]]$ thì cần và đủ rằng số hạng tự do của nó khả nghịch trong $A$.*

Giả sử tồn tại $v \in A[[I]]$ sao cho $uv = 1$. Gọi $a, \beta$ là các số hạng tự do của $u$ và $v$, khi đó $\alpha \beta = 1$, nên $a$ khả nghịch.

Ngược lại, giả sử số hạng tự do $a$ của $u$ khả nghịch. Khi đó tồn tại một chuỗi lũy thừa hình thức $t \in A[[I]]$ sao cho $u = \alpha (1 - t)$ và $\omega(t) > 0$. Lại có một đồng cấu vành $\varphi : A[[T]] \to A[[I]]$ sao cho $\varphi(T) = t$, và $1 - T$ khả nghịch trong $A[[T]]$ (Mệnh đề 5); do đó $1 - t$ khả nghịch trong $A[[I]]$, nên $u$ cũng khả nghịch.

#### Nhận xét {#alg-iv-s4-n4-rem-1 .statement}

— Cho $A$ là tập hợp tất cả các chuỗi lũy thừa hình thức có số hạng tự do bằng 1. Theo Mệnh đề 6, $M$ là một nhóm giao hoán theo phép nhân; do đó nhóm nhân của $A[[I]]$ là tích trực tiếp của $M$ và nhóm nhân của $A$. Ta sẽ trang bị cho $A$ tôpô cảm sinh từ tôpô của $A[[I]]$. Với mỗi $\beta \in \mathbf{N}^{(1)}$ ta đã định nghĩa ở IV, p. 26 iđêan $a_\beta$ của $A[[I]]$; khi đó $1 + a_\beta$ là một nhóm con của $M$ và họ $(1 + a_{\beta'})$ là một hệ cơ bản các lân cận của 1 trong $M$. Vì phép nhân trong $M$ liên tục, ta thấy rằng $A$ là một nhóm tôpô (Gen. Top., III, p. 223); nói cách khác, *ánh xạ* $f \mapsto f^{-1}$ *là liên tục trong* $M$.

Let $K$ là một trường giao hoán và $\mathcal{O}$ là vành con của trường các phân thức hữu tỉ $K((X_i)_{i,,})$ gồm các phân thức hữu tỉ mà phần tử $0$ của $K^1$ có thể thay vào. Nếu $f \in \mathcal{O}$, ta có $f = \frac{u}{v}$, trong đó $u$ và $v$ là các đa thức sao cho số hạng hằng của $v$ khác $0$, do đó $v$ khả nghịch trong $K[[I]]$. Ta có thể kiểm tra ngay rằng phần tử $uv^{-1}$ của $K[[I]]$ chỉ phụ thuộc vào $f$; ta nói rằng chuỗi lũy thừa hình thức $uv^{-1}$ là *khai triển tại gốc của phân thức hữu tỉ* $\frac{u}{v}$. Ánh xạ $f \mapsto uv^{-1}$ là một đồng cấu đơn ánh của $\mathcal{O}$ vào $K[[I]]$; ta sẽ thường đồng nhất $\mathcal{O}$ với ảnh của nó qua ánh xạ này.

### 5. Công thức Taylor cho chuỗi lũy thừa hình thức

Cho $X = (X_i)_{i \in I}$ và $Y = (Y_i)_{i \in I}$, là hai họ biến không xác định ứng với cùng một tập chỉ số I. Ta ký hiệu bởi $X + Y$ họ $(X_i + Y_i)_{i \in I}$, của các chuỗi lũy thừa hình thức trong $A[[X, Y]]$. Rõ ràng là ta có thể thay $X_i + Y_i$ cho $X_i$ trong một chuỗi lũy thừa hình thức $u \in A[[X]]$, kết quả được viết là $u(X + Y)$. Với mỗi $v \in \mathbf{N}^{(I)}$ ta ký hiệu $\Delta^v u$ là hệ số của $Y^v$ trong chuỗi lũy thừa hình thức $u(X + Y)$ xét như thuộc $A[[X]][[Y]]$ (III, p. 456). Nói cách khác, ta có

$$
u(X + Y) = \sum_v \Delta^v u(X) \cdot Y^v \quad (u \in A[[X]]) .
$$

Thay $(0, X)$ vào chỗ $(X, Y)$ ta được

$$
u(X) = \sum_v \Delta^v u(0) \cdot X^v ;
$$

Nói cách khác, số hạng hằng của $\Delta^v u$ là hệ số của $X^v$ trong $u$. Vì ánh xạ $u \mapsto u(X + Y)$ của $A[[X]]$ vào $A[[X, Y]]$ là liên tục, nên các ánh xạ $u \mapsto \Delta^v u$ của $A[[X]]$ vào chính nó cũng liên tục.

Cũng như trong trường hợp đa thức (IV, p. 7) ta có thể chứng minh các công thức

$$
\Delta^\sigma(uv) = \sum_{v+\rho=\sigma} \Delta^v(u) \Delta^\rho(v) ,
$$
$$
\Delta^\rho \Delta^\sigma u = \frac{(\rho + \sigma)!}{\rho! \; \sigma!} \Delta^{\rho + \sigma} u .
$$

Công thức nhị thức (I, p. 99, Hệ quả 2) cho giá trị sau của $\Delta^v u$ khi $u = \sum_\lambda \alpha_\lambda X^\lambda$

$$
\Delta^v u = \sum_\lambda \alpha_{\lambda + v} \frac{(\lambda + v)!}{\lambda! \; v!} X^\lambda .
$$

Xét riêng trường hợp $v = \epsilon_i$, tức là $v_i = 1, v_j = 0$ với $j \neq i$. Ta sẽ đặt $D_i u = \Delta^{\epsilon_i} u$; nói cách khác, $D_i u$ là hệ số của $Y_i$ trong $u(X + Y)$. Theo (10), do đó ta có

$$
D_i u = \sum_\lambda (\lambda_i + 1) \alpha_{\lambda + \epsilon_i} X^\lambda ;
$$

đặc biệt ta có $D_i(X_i) = 1$ và $D_i(X_j) = 0$ với $j \neq i$. Công thức (8) cho thấy $D_i$ là một đạo hàm của $A[[X]]$, và từ (9) ta suy ra quan hệ

$$
D^v u = v! \; \Delta^v u
$$

như trong trường hợp các đa thức (IV, p. 8) (ta đã đặt $D^\nu = \prod_{i \in I} D_i^{\nu_i}$ cho $\nu = (\nu_i)_{i \in I}$, trong $\mathbf{N}^{(I)}$). Khi A là một Q-đại số, các công thức (6), (7) và (12) suy ra các « công thức Taylor »:

$$
u(\mathbf{X} + \mathbf{Y}) = \sum \frac{1}{\nu!} D^\nu u(\mathbf{X}) \cdot \mathbf{Y}^\nu,
$$
$$
u(\mathbf{X}) = \sum \frac{1}{\nu!} D^\nu u(0) \cdot \mathbf{X}^\nu.
$$

*Nhận xét. — 1) Ta thường nói rằng $D_i u$ là *đạo hàm riêng của u theo X*, ; ta cũng dùng ký hiệu $D_{x_i} u, \frac{\partial u}{\partial x_i}$ và $u'_{x_i}$. Với một ẩn thức X duy nhất, đạo hàm riêng duy nhất $Du$ (cũng viết $\frac{du}{dX}$ hoặc $u'$) được gọi là *đạo hàm* của $u$.

2) Công thức (9) cho thấy các tự đồng cấu $A^p$ của A-môđun $A[[X]]$ giao hoán từng cặp. Do đó điều đó cũng đúng với các tự đồng cấu $D_i$.

3) Nếu $u \in A[(X_i)_{i \in I}]$ là một đa thức, thì các đa thức $A^p u$ và $D_i u$ được định nghĩa ở IV, p. 6 và 7 trùng nhau với các chuỗi lũy thừa hình thức được ký hiệu bởi cùng các ký hiệu ấy.*

### 6. Đạo hàm trong đại số các chuỗi lũy thừa hình thức

Cho I là một tập hợp, E là một A-đại số kết hợp, giao hoán và có đơn vị, được tôpô tuyến tính, tách biệt và đầy đủ, và $x = (x_i)_{i \in I}$ là một họ các phần tử của E thỏa mãn các điều kiện a) và b) của Mệnh đề 4 (IV, p. 28). Cho $\varphi$ là đồng cấu liên tục $u \mapsto u(x)$ của $A[[I]]$ vào E ; nó trang bị cho E một cấu trúc $A[[I]]$-môđun. Theo III, p. 552, một đạo hàm A của $A[[I]]$ vào $A[[I]]$-môđun E là do đó một ánh xạ A-tuyến tính $D : A[[I]] \to E$ thỏa mãn quan hệ
$$
D(uv) = u(x) \cdot D(v) + D(u) \cdot v(x)
$$
với $u, v$ trong $A[[I]]$.

#### Mệnh đề 7 {#alg-iv-s4-prop-7 .statement}

— *Cho $(y_i)_{i \in I}$, là một họ các phần tử của E. Khi I là vô hạn, *ta* giả sử rằng $y_i$ tiến tới 0 theo lọc các phần bù của những tập con hữu hạn của I. Khi đó tồn tại một đạo hàm A liên tục duy nhất D của $A[[I]]$ vào *A[[I]]-môđun* E sao cho $D(X_i) = y_i$ với mọi $i \in I$. Ta có*
$$
D(u) = \sum_{i \in I} (D_i u)(x) \cdot y_i \quad (u \in A[[I]]) .
$$

Vì 0 trong E có một hệ cơ bản các lân cận gồm các iđêan, nên họ $((D_i u)(x) \cdot y_i)_{i \in I}$ là khả tổng trong E với mọi $u \in A[[I]]$ (Gen. Top., III, p. 263, Hệ quả 2). Do đó công thức (16) xác định một ánh xạ A-tuyến tính $D : A[[I]] \to E$. Chúng tôi để độc giả tự kiểm tra rằng D là một đạo hàm liên tục.

Cho $D_1$ là một đạo hàm A liên tục của $A[[I]]$ vào E, sao cho $D_1(X_i) = y_i$ với mọi $i \in I$. Hạt nhân của đạo hàm liên tục $D - D_1$ là một đại số con đóng B của $\mathbf{A}[[\mathbf{I}]]$ chứa 1 và các biến $X_i$. Vì đại số đa thức $\mathbf{A}[(X_i)_{i \in I}]$ dày đặc trong $\mathbf{A}[[\mathbf{I}]]$, ta có $B = \mathbf{A}[[\mathbf{I}]]$ và do đó $D_1 = D$.

#### Hệ quả 1 {#alg-iv-s4-prop-7-cor-1 .statement}

— *Cho $\Delta$ là một đạo hàm liên tục của A-đại số E. Với mỗi chuỗi lũy thừa hình thức $u \in \mathbf{A}[[\mathbf{I}]]$ họ $((D_iu)(x) \cdot \Delta x_i)_{i \in I}$ là khả tổng và ta có*

$$
\Delta(u(x)) = \sum_{i \in I} (D_iu)(x) \cdot \Delta x_i .
$$

Điều này suy ra từ Mệnh đề 7 vì ánh xạ $u \mapsto \Delta(u(x))$ là một đạo hàm liên tục của $\mathbf{A}[[\mathbf{I}]]$ vào môđun E trên $\mathbf{A}[[\mathbf{I}]]$.

#### Hệ quả 2 {#alg-iv-s4-prop-7-cor-2 .statement}

— *Đạo hàm $D_i$ là đạo hàm liên tục duy nhất của đại số trên A $\mathbf{A}[[\mathbf{I}]]$ sao cho*

$$
D_i(X_i) = 1 , \quad D_i(X_j) = 0 \quad \text{cho} \quad j \neq i .
$$

Điều này suy ra từ Hệ quả 1.

#### Hệ quả 3 {#alg-iv-s4-prop-7-cor-3 .statement}

— *Cho $f \in \mathbf{A}[[X_1, ..., X_s]]$ và $g_i \in \mathbf{A}[[Y_1, ..., Y_q]]$ với $1 \leq i \leq p$. Giả sử rằng với $1 \leq i \leq p$ số hạng hằng của $g_i$ bằng không, và đặt $h = f(g_1, ..., g_p)$. Khi đó với $1 \leq j \leq q$ ta có*

$$
\frac{\partial h}{\partial Y_j} = \sum_{i=1}^p D_i f(g_1, ..., g_p) \cdot \frac{\partial g_i}{\partial Y_j} .
$$

Đây là trường hợp riêng $E = \mathbf{A}[[Y_1, ..., Y_s]]$, $x_i = q_i$ và $A = \partial / \partial Y_j$ của Hệ quả 1.

#### Mệnh đề 8 {#alg-iv-s4-prop-8 .statement}

— *Cho $X = (X_i)_i$, là một họ hữu hạn các ẩn.
(i) Mọi đạo hàm của vành chuỗi lũy thừa hình thức $\mathbf{A}[[X]]$ đều liên tục.
(ii) Mọi đạo hàm của vành đa thức $\mathbf{A}[X]$ vào vành chuỗi lũy thừa hình thức $\mathbf{A}[[X]]$ đều mở rộng một cách duy nhất thành một đạo hàm của vành $\mathbf{A}[[X]]$.
(iii) Họ $(D_i)_{i \in I}$ là một cơ sở của môđun trên $\mathbf{A}[[X]]$ các đạo hàm trên A của $\mathbf{A}[[X]]$ vào chính nó.
Cho $b_n$ là tập hợp tất cả các chuỗi lũy thừa hình thức có bậc $\geq n$. Rõ ràng $b_n$ là một iđêan trong vành $\mathbf{A}[[X]]$, sinh bởi các đơn thức bậc $n$. Do đó $b_n$ gồm các tổng hữu hạn của các tích của $n$ chuỗi lũy thừa hình thức không có số hạng hằng; nếu $D$ là một đạo hàm của $\mathbf{A}[[X]]$, ta có*

$$
D(f_1 \cdots f_n) = \sum_{i=1}^n f_1 \cdots f_{i-1} D(f_i) f_{i+1} \cdots f_n ,
$$

suy ra ngay rằng $Db_n \subset b_{n-1}$ với $n \geq 1$. Vì dãy $(b_n)_{n \geq 0}$ là một hệ cơ bản các lân cận của 0 trong $\mathbf{A}[[X]]$ (IV, p. 26 nhận xét), D liên tục và (i) được chứng minh.

Cho $A$ là một đạo hàm của $A[X]$ vào $A[[X]]$. Lập luận như trên, ta có thể ցույց ra rằng $A(h)$ thuộc $b, -_1$, với mọi đa thức thuần nhất $h$ bậc $n \geq 1$. Bây giờ cho $u \in A[[X]]$ và cho $u_n$ là thành phần thuần nhất bậc $n$ của $u$. Vì $A(u_n) \in b, -_1$ với $n \geq 1$, họ $(A(u)), \ldots$, là khả tổng trong $A[[X]]$ và ta có thể định nghĩa một đạo hàm $D$ của $A[[X]]$ vào chính nó bởi

$$
D(u) = \sum_{n \geq 0} \Delta(u_n)
$$

Chúng ta có $D(b,) \subset b, -_1$, do đó $D$ là một tự đồng cấu liên tục của nhóm cộng của $A[[X]]$. Ánh xạ $\Phi : (u, v) \mapsto D(uv) - uD(v) - D(u)v$ từ $A[[X]] \times A[[X]]$ vào $A[[X]]$ là liên tục và bằng 0 trên $A[X] \times A[X]$. Vì $A[X]$ trù mật trong $A[[X]]$, ta có $\Phi = 0$; nói cách khác, $D$ là một đạo hàm của $A[[X]]$ vào chính nó, mở rộng $A$.

Cuối cùng, $A[X]$ trù mật trong $A[[X]]$ và theo (i) mọi đạo hàm của $A[[X]]$ đều liên tục; do đó tồn tại một mở rộng duy nhất của $A$ thành một đạo hàm của $A[[X]]$. Điều này chứng minh (ii).

Còn phải chứng minh (iii). Công thức (18) (IV, p. 33) cho thấy họ $(D_i)_{i \in I}$ độc lập tuyến tính trên $A[[X]]$, và công thức (16) (IV, p. 32), áp dụng trong trường hợp $E = A[[X]]$, cho thấy mọi $A$-đạo hàm là một tổ hợp tuyến tính của các $D_i$ với các hệ số trong $A[[X]]$.

#### Mệnh đề 9 {#alg-iv-s4-prop-9 .statement}

— Cho $(u,) \ldots$ là một họ *cộng được* các phần tử của $A[[I]]$ không có số hạng hằng và $D$ là một đạo hàm liên tục của $A$-đại số $A[[I]]$. Nếu $f = \prod_{\lambda \in L} (1 + u_\lambda)$ (IV, p. 27, Mệnh đề 2), thì họ $(Du_\lambda/(1 + u_\lambda))_{\lambda \in L}$ là cộng được và ta có

$$
D(f)/f = \sum_{\lambda \in L} D(u_\lambda)/(1 + u_\lambda) .
$$

Nếu $g$ và $h$ là hai phần tử khả nghịch của $A[[I]]$, thì

$$
D(gh) = h \cdot Dg + g \cdot Dh
$$

do đó, khi chia cho $gh$,

$$
D(gh)/gh = D(g)/g + D(h)/h .
$$

Với mọi tập con hữu hạn $M$ của $L$ đặt $f_M = \prod_{\lambda \in M} (1 + u_\lambda)$. Từ (21) suy ra bằng quy nạp theo Card $M$ quan hệ

$$
D(f_M)/f_M = \sum_{\lambda \in M} D(u_\lambda)/(1 + u_\lambda)
$$

Điều này chứng minh Mệnh đề 9 khi $L$ hữu hạn. Bây giờ giả sử rằng $L$ là vô hạn và viết $\mathfrak{F}$ cho tập hợp có thứ tự lọc của các tập con hữu hạn của $L$. Ta có $\lim_{\mathfrak{F}} f_M = f$, và do đó (*IV*, p. 30 nhận xét)

$$
D(f)/f = \lim_{\mathfrak{F}} D(f_M)/f_M .
$$

Do đó Mệnh đề 9 suy ra bằng cách lấy giới hạn trong (22).

### 7. Nghiệm của các phương trình trong một vành chuỗi lũy thừa hình thức

#### Bổ đề 2 {#alg-iv-s4-lem-2 .statement}

*Cho* $(g_i)_i$ *là một họ các phần tử có bậc* $\geq 2$ *trong* $\mathbf{A}[[\mathbf{I}]]$. *Khi* $\mathbf{I}$ *vô hạn, giả sử rằng* $g_i$ *tiến tới 0 theo bộ lọc của các phần bù của các tập con hữu hạn của* $\mathbf{I}$. *Tồn tại một và chỉ một tự đẳng cấu* T *của A*-đại số tôpô* $\mathbf{A}[[\mathbf{I}]]$ *sao cho* $T(X_i) = X_i + g_i$ *đối với mọi* $i \in \mathbf{I}$. *Hơn nữa,

(23)
$$
\omega(T(u) - u) \geq \omega(u) + 1
$$
*đối với mỗi* $u \in \mathbf{A}[[\mathbf{I}]]$.

Chuỗi $f_i = X_i + g_i$ không có số hạng hằng và khi $\mathbf{I}$ là vô hạn, $f_i$ tiến tới 0 theo lọc các phần bù của các tập con hữu hạn của $\mathbf{I}$. Do đó (IV, p. 28, Mệnh đề 4) tồn tại chính xác một tự đồng cấu liên tục T của A-đại số $\mathbf{A}[[\mathbf{I}]]$ sao cho $T(X_i) = f_i$ với mọi $i \in \mathbf{I}$. Với mỗi $\nu \in \mathbf{N}'$ ta đặt

$$
v_\nu = T(X^\nu) - X^\nu = \prod_{i \in \mathbf{I}} (X_i + g_i)^{\nu(i)} - \prod_{i \in \mathbf{I}} X_i^{\nu(i)} ;
$$

các quan hệ $\omega(g_i) \geq 2$ suy ra $w(v_\nu) \geq |\nu| + 1$, và quan hệ (23) theo đó suy ra ngay.

Hãy chứng minh rằng $T$ là *đơn ánh*. Cho $u \in \mathbf{A}[[\mathbf{I}]]$ sao cho $T(u) = 0$, theo (23) ta có $w(u) \geq w(u) + 1$, điều này là không thể nếu $u \neq 0$ vì khi đó $w(u)$ sẽ là một số nguyên dương.

Với mọi chuỗi hình thức $v$ trong $\mathbf{A}[[\mathbf{I}]]$ ta ký hiệu bởi $H_n(v)$ thành phần thuần nhất bậc $n$ của nó. Đặt $S_0(v) = H_0(v)$ và định nghĩa các ánh xạ liên tục $S, : \mathbf{A}[[\mathbf{I}]] \to \mathbf{A}[[\mathbf{I}]]$ bởi các công thức đệ quy

(24)
$$
S_n(v) = H_n \left( v - T \left( \sum_{k=0}^{n-1} S_k(v) \right) \right) \quad \text{với} \quad n \geq 1
$$

Đặt $S(v) = \sum_{n \geq 0} S_n(v)$; nếu $\nu \in \mathbf{N}^{(\mathbf{I})}$ và $n = |\nu|$, thì hệ số $S^\nu(v)$ của $X^\nu$ trong $S(v)$ bằng hệ số của $X^\nu$ trong $S,(\nu)$; vì $S,$ là một ánh xạ liên tục, ánh xạ $S^\nu : \mathbf{A}[[\mathbf{I}]] \to \mathbf{A}$ là liên tục. Do đó, theo định nghĩa của tôpô tích trên $\mathbf{A}[[\mathbf{I}]] = \mathbf{A}^{\mathbf{N}^{(\mathbf{I})}}$, ánh xạ $S : \mathbf{A}[[\mathbf{I}]] \to \mathbf{A}[[\mathbf{I}]]$ là liên tục.

Ta sẽ chứng minh quan hệ $T(S(v)) = v$ với mọi $v \in \mathbf{A}[[\mathbf{I}]]$; điều này sẽ hoàn tất chứng minh của bổ đề. Cho $v \in \mathbf{A}[[\mathbf{I}]]$, $u_n = S_n(v)$ và $u = S(v)$. Cho $n$ là một số nguyên dương sao cho

(25)$_n$
$$
\omega(v - T(u)) \geq n .
$$

Ta có $w(u - (u_0 + \ldots + u_{n-1})) \geq n$, do đó

$$
\omega(T(u) - T(u_0 + \ldots + u_{n-1}) - u_n) \geq n + 1
$$

theo (23). Bây giờ công thức đệ quy (24) cho thấy rằng

$$
u_n = H_n(v - T(u_0 + \cdots + u_{n-1}))
$$

Theo (26) chuỗi lũy thừa hình thức $v - T(u)$ và $v - T(u_0 + \ldots + u_{n-1}) - u_n$ có cùng thành phần thuần nhất bậc $n$, và thành phần này bằng 0, theo (27). Vậy ta có $w(v - T(u)) \geq n + 1$, tức là $(25)_n$ suy ra $(25)_{n+1}$. Vì $(25)_0$ hiển nhiên đúng, nên ta có $\omega(v - T(u)) \geq n$ với mọi số nguyên $n \geq 0$, do đó $v = T(u) = T(S(v))$, như đã phải chứng minh.

Trong phần còn lại của số này, với mọi tập hợp $I$, ta ký hiệu bởi $A\{I\}$ tập hợp các họ $(f_i)_{i \in I}$ thỏa mãn các điều kiện sau:
(i) với mỗi $i \in I$, $f_i$ là một phần tử của $A[[I]]$ không có số hạng hằng;
(ii) nếu $I$ là vô hạn, thì $f_i$ tiến tới 0 theo lọc các phần bù của các tập con hữu hạn của $I$.

Tập hợp $A\{I\}$ là một nửa nhóm có đơn vị đối với luật hợp thành $(f, g) \mapsto f \circ g$, với $\{X_i\}_{i \in I}$ là phần tử đơn vị. Do đó tập các phần tử khả nghịch của $A\{I\}$ là một nhóm.

Mặt khác, cho $E$ là nửa nhóm của tất cả các tự đồng cấu liên tục có đơn vị của $A$-đại số $A[[I]]$ giữ bất biến iđêan của mọi chuỗi lũy thừa hình thức không có số hạng hằng. Nếu $f \in A\{I\}$ và $g \in A[[I]]$, thì phần tử $g(f)$ được xác định. Với $f$ cố định, ánh xạ $g \mapsto g(f)$ của $A[[I]]$ vào chính nó là một phần tử $W_f$ của $E$. Nếu $f_1, f_2 \in A\{I\}$ và $g \in A[[I]]$, ta có, theo công thức (5) (IV, p. 30)

$$
W_{f_1 \circ f_2}(g) = g(f_1 \circ f_2) = g(f_1) \circ f_2 = W_{f_2}(W_{f_1}(g))
$$

suy ra $f \mapsto W_f$ là một đồng cấu của nửa nhóm đối của $A\{I\}$ vào $E$. Theo Mệnh đề 4 (IV, p. 28) đồng cấu này là song ánh.

Cho $f = (f_i)_{i \in I} \in A\{I\}$ và cho $\sum_{j \in I} \alpha_{ij} X_j$ là thành phần thuần nhất bậc 1 của $f_i$. Với mỗi $j$ cố định trong $I$ ta có $\alpha_{ij} = 0$ trừ một số hữu hạn chỉ số $i$, theo giả thiết (ii) ở trên. Nếu $(\lambda_i) \in A^{(I)}$, ta do đó có $\left( \sum_{j \in I} \alpha_{ij} \lambda_j \right) \in A^{(I)}$.

Ta ký hiệu bởi $T_f$ ánh xạ $A$-tuyến tính $^1$

$$
(\lambda_i) \mapsto \left( \sum_{j \in I} \alpha_{ij} \lambda_j \right)
$$

từ $A^{(I)}$ vào $A^{(I)}$. Nếu $g \in A\{I\}$, dễ dàng kiểm tra rằng

$$
T_{f \circ g} = T_f \circ T_g .
$$

$^1$ Đôi khi $T_f$ được gọi là ánh xạ tuyến tính tiếp tuyến với $f$.

#### Mệnh đề 10 {#alg-iv-s4-prop-10 .statement}

— Cho $f \in A\{I\}$; khi đó các điều kiện sau là tương đương :
(i) $f$ khả nghịch trong $A\{I\}$ đối với luật $\circ$;
(ii) $T_f$ khả nghịch trong vành $\mathrm{End}(A^{(I)})$.

Hàm ý (i) $\Rightarrow$ (ii) là ngay lập tức từ (28). Giả sử bây giờ rằng $T_f$ là khả nghịch trong $\mathrm{End}(A^{(I)})$. Tồn tại $g = (g_i)_i \in A\{I\}$ sao cho mỗi $g_i$ là thuần nhất bậc $l$ và $T_g \circ T_f$ là ánh xạ đồng nhất của $A^{(I)}$. Đặt $h = g \circ f$; khi đó (28) cho thấy $T_h$ là ánh xạ đồng nhất của $A^{(I)}$, điều này tương đương với mệnh đề $\omega(h_i - X_i) \geq 2$. Theo Bổ đề 2 của IV, p. 35 $h$ do đó khả nghịch trong $A\{I\}$. Rõ ràng $g$ là khả nghịch trong $A\{I\}$, suy ra $f$ là khả nghịch trong $A\{I\}$.

#### Hệ quả {#alg-iv-s4-n7-cor-1 .statement}

— Cho $f_i(Y_1, Y_2, \ldots, Y_q, X_1, X_2, \ldots, X_p)$ ($1 \leq i \leq q$) là $q$ chuỗi lũy thừa hình thức không có số hạng hằng trong $A[[Y_1, \ldots, Y_q, X_1, \ldots, X_p]]$. Nếu số hạng hằng của chuỗi lũy thừa hình thức $D = \det \left( \frac{\partial f_i}{\partial Y_j} \right)$ là khả nghịch trong $A$, thì tồn tại duy nhất một hệ $q$ chuỗi lũy thừa hình thức $u_1(X_1, \ldots, X_p), \ldots, u_q(X_1, \ldots, X_p)$ sao cho
$$
f_i(u_1, \ldots, u_q, X_1, \ldots, X_p) = 0 \quad (1 \leq i \leq q).
$$
Đặt $f_{q+1} = X_1, \ldots, f_{q+p} = X_p$, $f = (f_1, \ldots, f_{p+q})$, khi đó $\det T_f$ bằng với số hạng hằng của $D$, do đó khả nghịch trong $A$; vì vậy $T_f$ khả nghịch. Theo Mệnh đề 10 tồn tại các chuỗi lũy thừa hình thức không có số hạng hằng
$$
g_1, \ldots, g_{q+p} \in A[[Y_1, \ldots, Y_q, X_1, \ldots, X_p]]
$$
sao cho, khi viết
$$
g = (g_1, \ldots, g_{p+q}), \quad 1_{p+q} = (Y_1, \ldots, Y_q, X_1, \ldots, X_p)
$$
ta có $f \circ g = g \circ f = 1_{p+q}$. Quan hệ $f \circ g = 1_{p+q}$, đặc biệt cho
$$
g_{q+1} = X_1, \ldots, g_{q+p} = X_p.
$$
Do đó
$$
f_i(g_1, \ldots, g_q, X_1, \ldots, X_p) = Y_i \quad (1 \leq i \leq q).
$$
Bây giờ đặt
$$
u_i(X_1, \ldots, X_p) = g_i(0, \ldots, 0, X_1, \ldots, X_p) \quad (1 \leq i \leq q);
$$
thay 0 cho mỗi $Y_i$ trong (30) ta thu được quan hệ (29) mong muốn.

Ngược lại, giả sử rằng các chuỗi lũy thừa hình thức $u_1, \ldots, u_q$ trong vành $A[[X_1, \ldots, X_p]]$ thỏa mãn quan hệ (29). Quan hệ $g \circ f = 1_{p+q}$ suy ra
$$
g_i(f_1, \ldots, f_q, X_1, \ldots, X_p) = Y_i \quad (1 \leq i \leq q);
$$
và thay $u_i$ cho $Y_i$ với $1 \leq i \leq q$ trong (32), ta thu được (31), do đó tính duy nhất của nghiệm của hệ (29).

### 8. Chuỗi lũy thừa hình thức trên một miền nguyên

#### Mệnh đề 11 {#alg-iv-s4-prop-11 .statement}

— Giả sử rằng $A$ là một miền nguyên.

(i) *Vành* $A[[I]]$ *lại là một miền nguyên*.

(ii) *Nếu* $u, v$ *là các phần tử khác không của* $A[[I]]$, *thì* $\omega(uv) = \omega(u) + \omega(v)$.

Với mỗi $J \subset I$, cho $\varphi_J$ là đồng cấu từ $A[[I]]$ vào $A[[J]]$ thu được bằng cách thay trong mỗi phần tử của $A[[I]]$, $X_i$ bằng $X_i$ khi $i \in J$ và bằng 0 cho $X_i$ khi $i \in I - J$. Cho $u, v$ là các phần tử khác 0 của $A[[I]]$, $p = \omega(u)$, $q = \omega(v)$; tồn tại một tập con hữu hạn $J$ của $I$ sao cho

$$
\varphi_J(u) \neq 0,\ \varphi_J(v) \neq 0,\ \omega(\varphi_J(u)) = p,\ \omega(\varphi_J(v)) = q.
$$

Cho a (resp. b) là thành phần thuần nhất bậc $p$ (resp. $q$) của $\varphi_J(u)$ (resp. $\varphi_J(v)$). Vì $J$ hữu hạn, a và b là các đa thức. Ta có $a \neq 0, b \neq 0$, do đó $ab \neq 0$ (IV, p. 9, Mệnh đề 8). Suy ra $\varphi_J(u)\ \varphi_J(v)$ khác 0, có cấp $p + q$. Từ đó suy ra $uv \neq 0$ và $\omega(uv) \leq p + q$; nhưng rõ ràng $\omega(uv) \geq p - q$.

### 9. Trường phân thức của vành các chuỗi lũy thừa hình thức theo một ẩn trên một trường

Nếu K là một trường giao hoán, ta ký hiệu $K((X))$ là trường phân thức của miền nguyên $K[[X]]$.

#### Mệnh đề 12 {#alg-iv-s4-prop-12 .statement}

— *Mỗi phần tử khác 0* $u$ *của* $K((X))$ *có thể được viết một cách duy nhất dưới dạng* $u = X^k v$, *trong đó* $k \in \mathbf{Z}$ *và* $v$ *là một chuỗi lũy thừa hình thức theo* $X$ *có cấp* 0.

Cho $u = w/t$, trong đó $w, t$ là các phần tử khác 0 của $K[[X]]$. Ta có $w = X^r w_1, t = X^s t_1$, trong đó $r, s \in \mathbf{N}$ và $w_1, t_1$ là các chuỗi lũy thừa hình thức có cấp 0, do đó khả nghịch trong $K[[X]]$ (IV, p. 30, Mệnh đề 6). Khi đó $u = X^{r-s} w_1 t_1^{-1}$ và $w_1 t_1^{-1}$ là một chuỗi lũy thừa hình thức có cấp 0.

Ta chứng minh tính duy nhất. Giả sử rằng $u = X^{k_1} v_1 = X^{k_2} v_2$ trong đó $k_1, k_2 \in \mathbf{Z}$ và $v_1, v_2$ là các chuỗi lũy thừa hình thức có cấp 0. Vì $X^{k_1 - k_2} = v_2 v_1^{-1}$ là một chuỗi lũy thừa hình thức có cấp 0, ta có $k_1 = k_2$ do đó $v_1 = v_2$ và điều này chứng minh mệnh đề tính duy nhất.

Ta sẽ hiểu các phần tử của $K((X))$ là *chuỗi lũy thừa hình thức tổng quát* theo $X$ với hệ số trong $K$, hay đơn giản là chuỗi lũy thừa hình thức khi không thể có sự nhầm lẫn (các phần tử của $K[[X]]$ khi đó được gọi là *chuỗi lũy thừa hình thức với số mũ dương*); nếu $u \neq 0$, thì số nguyên $k$ được định nghĩa trong Mệnh đề 12 cũng được gọi là *cấp* của $u$ và được viết là $\omega(u)$, ngay cả khi nó nhỏ hơn $0$; ta cũng đặt $\omega(0) = \infty$. Có thể kiểm tra ngay rằng

$$
\begin{align*}
\omega(u + v) &\geq \inf(\omega(u), \omega(v)) \\
\omega(u + v) &= \inf(\omega(u), \omega(v)) \quad \text{nếu}\ \ \omega(u) \neq \omega(v) \\
\omega(uv) &= \omega(u) + \omega(v)
\end{align*}
$$

vẫn đúng đối với các chuỗi lũy thừa hình thức tổng quát. Đặc biệt, nếu $u \neq 0$, thì $w(u^{-1}) = -w(u)$. \* Nói cách khác (Comm. Alg., VI, § 3, No. 6, p. 392, Định nghĩa 3), w là một định giá rời rạc chuẩn hóa của trường $K((X))$. \*

Với mỗi số nguyên $n \in \mathbf{Z}$ hãy đặt $p_n$ là tập hợp tất cả $u \in K((X))$ sao cho $\omega(u) \geq n$. Khi đó (p.), , , là một dãy giảm các nhóm con của nhóm cộng $K((X))$, với giao bằng 0 ; do đó tồn tại một tôpô trên $K((X))$, bất biến qua phép tịnh tiến, sao cho $(p_n)_{n \in \mathbf{Z}}$ là một hệ cơ bản các lân cận của 0 (Gen. Top., III, p. 223). Ta dễ dàng kiểm tra rằng $K((X))$ là một trường tôpô (Gen. Top., III, p. 281) và rằng $K[[X]]$ là một không gian con mở và đóng của $K((X))$.

Cho một họ các phần tử của $K$, và giả sử rằng tồn tại một số nguyên N sao cho $a_n = 0$ với mọi $n < N$. Khi đó họ' $(\alpha_n X^n)_{n \in \mathbf{Z}}$ là khả tổng trong $K((X))$ (Gen. Top., III, p. 263, Hệ quả) ; đặt $u = \sum_{n \in \mathbf{Z}} \alpha_n X^n$, khi đó $u = 0$ khi và chỉ khi $a_n = 0$ với mọi $n$; ngược lại cấp của $u$ là số nguyên nhỏ nhất k sao cho $\alpha_k \neq 0$. Sau cùng mọi phần tử của $K((X))$ đều có thể được viết duy nhất dưới dạng $\sum_{n \in \mathbf{Z}} \alpha_n X^n$, trong đó dãy (a,) thỏa mãn $\alpha_{-n} = 0$ với mọi n đủ lớn.

Vì vành $K[X]$ là một vành con của $K[[X]]$, mọi phân thức hữu tỉ $u/v \in K(X)$ (u, v là các đa thức theo X) có thể được đồng nhất với chuỗi lũy thừa hình thức (tổng quát) $uv^{-1}$ của $K((X))$, mà ta sẽ gọi là khai triển của nó tại gốc ; do đó trường $K(X)$ được đồng nhất với một trường con của $K((X))$.

### 10. Hàm mũ và logarit

Theo chuỗi lũy thừa mũ, ta hiểu phần tử $\sum_{n \geq 0} \frac{X^n}{n!}$ của $Q[[X]]$; nó sẽ được ký hiệu bởi exp X hoặc $e^X$.

#### Mệnh đề 13 {#alg-iv-s4-prop-13 .statement}

— Trong $Q[[X, Y]]$ ta có $e^{X+Y} = e^X e^Y$.

Vì công thức nhị thức cho

$$
\frac{(X+Y)^n}{n!} = \sum_{i+j=n} \frac{X^i}{i!} \frac{Y^j}{j!}
$$

Suy ra

$$
e^X e^Y = \left( \sum_{i \geq 0} \frac{X^i}{i!} \right) \left( \sum_{j \geq 0} \frac{Y^j}{j!} \right) = \sum_{i,j \geq 0} \frac{X^i}{i!} \frac{Y^j}{j!} = \sum_{n \geq 0} \sum_{i+j=n} \frac{X^i}{i!} \frac{Y^j}{j!}
$$
$$
= \sum_{n \geq 0} \frac{(X+Y)^n}{n!} = e^{X+Y}.
$$

Ta sẽ định nghĩa hai phần tử $e(X)$, l(X) của $Q[[X]]$ bởi

$$
e(X) = e^X - 1 = \sum_{n \geq 1} \frac{X^n}{n!}
$$

(34)
$$
l(X) = \sum_{n \geq 1} (-1)^{n-1} \frac{X^n}{n}.
$$

Ta có
(35)
$$
e(X+Y) = e(X) + e(Y) + e(X)e(Y)
$$
(36)
$$
D(e^X) = D(e(X)) = e^X
$$
(37)
$$
D(l(X)) = \sum_{n \geq 0} (-X)^n = (1+X)^{-1}.
$$

#### Mệnh đề 14 {#alg-iv-s4-prop-14 .statement}

— Chúng ta có $l(e(X)) = e(l(X)) = X$.

Chuỗi l và e không có số hạng hằng và các số hạng bậc 1 của chúng bằng X. Theo Mđ. 10 của IV, p. 37 thì chỉ cần chứng minh công thức $l(e(X)) = X$. Theo các công thức (36) và (37) và Hệ quả 3 của IV, p. 33 ta có

$$
D(l(e(X))) = (1 + e(X))^{-1} D(e(X)) = (e^X)^{-1} e^X = 1
$$

do đó $I(e(X)) = X$.

Cho K là một Q-algebra, khi đó các phần tử của K[[I]] không có số hạng hằng tạo thành một nhóm giao hoán $\mathcal{E}$ theo phép cộng. Các phần tử của K[[I]] có số hạng hằng bằng 1 tạo thành một nhóm giao hoán $\mathbf{A}$ theo phép nhân (IV, p. 30). Với mỗi $f \in \mathcal{E}$, ta có thể định nghĩa các phần tử $e \circ f$ và $I \circ f$ của $\mathcal{E}$, và theo Mđ. 14 ở trên, các ánh xạ $f \mapsto l \circ f$ và $f \mapsto e \circ f$ là các hoán vị nghịch đảo lẫn nhau của $\mathcal{E}$; rõ ràng chúng liên tục. Vì $\exp X = e(X) + 1$, ta thấy rằng ánh xạ mũ $f \mapsto \exp f = e \circ f + 1$ là một song ánh liên tục từ $\mathcal{E}$ lên $\mathcal{M}$. Theo công thức (4) của IV, p. 29 và Mđ. 13, ta có $\exp(f+g) = (\exp f)(\exp g)$ với $f, g \in \mathcal{E}$. Vậy hàm mũ là một đẳng cấu của nhóm tôpô $\mathcal{E}$ lên nhóm tôpô $\mathbf{A}$.

Đẳng cấu nghịch đảo của $\mathcal{M}$ lên $\mathcal{E}$ được gọi là lôgarit và được viết $g \mapsto \log g$. Do đó ta có $\log g = l(g-1)$ với $g$ trong $\mathcal{M}$, và đặc biệt,

(38)
$$
\log(1+X) = l(X).
$$

Vì lôgarit là một đồng cấu từ $\mathcal{M}$ vào $\mathcal{E}$, công thức $(1+X)(1+Y) = 1 + (X+Y+XY)$ suy ra

(39)
$$
l(X) + l(Y) = l(X+Y+XY).
$$

Cho $(u,)_{\lambda}$ là một họ các phần tử của $\mathcal{B}$, khi đó họ $(\exp u_{\lambda})_{\lambda \in L}$ là khả tổng và ta có

(40)
$$
\exp \left( \sum_{\lambda \in L} u_{\lambda} \right) = \prod_{\lambda \in L} \exp u_{\lambda}.
$$

Tương tự, nếu $(f_\lambda)_{\lambda \in L}$ là một họ khả nhân của các phần tử của A, thì họ $(\log f_\lambda)_{\lambda \in L}$ là khả tổng và ta có

(41)
$$
\log \left( \prod_{\lambda \in L} f_\lambda \right) = \sum_{\lambda \in L} \log f_\lambda .
$$

Cho $g \in A$, và cho D là một đạo hàm liên tục của $K[[I]]$. Ta có $\log g = l(g - 1)$, nên theo Hệ quả 3 của IV, p. 33 và (37) ta có

(42)
$$
D \log g = D(g)/g .
$$

Biểu thức $D(g)/g$ được gọi là đạo hàm lôgarit của g (đối với D).

### Bài tập {#alg-iv-s4-exercises}

Xem [các bài tập cho § 4](exercises/s4/).
