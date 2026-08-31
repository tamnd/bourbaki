---
book: alg
book_title: Algebra
chapter: X
chapter_title: ALGÈBRE HOMOLOGIQUE
section: 2
section_title: Complexes de A-modules
lang: vi
source: alg-x-fr
book_pages: A X.23-A X.46, A X.173-A X.178
pdf_pages: 0029-0052, 0179-0184
extraction: ocr
subsections:
    - "no": 1
      title: Complexes de A-modules
      page: 23
      pdf_page: 29
    - "no": 2
      title: ' Opérations sur les complexes'
      page: 27
      pdf_page: 33
    - "no": 3
      title: L’homomorphisme de liaison et la suite exacte d’homologie
      page: 29
      pdf_page: 35
    - "no": 4
      title: Homotopies
      page: 32
      pdf_page: 38
    - "no": 5
      title: Complexes scindés
      page: 34
      pdf_page: 40
    - "no": 6
      title: Cône et cylindre d’un morphisme de complexes
      page: 36
      pdf_page: 42
    - "no": 7
      title: Le cône d’un morphisme injectif ; nouvelle définition de l’homomorphisme de liaison
      page: 39
      pdf_page: 45
    - "no": 8
      title: Caractéristiques d’Euler-Poincaré
      page: 40
      pdf_page: 46
    - "no": 9
      title: Complexes de modules à droite, complexes de multimodules
      page: 43
      pdf_page: 49
    - "no": 10
      title: 'Exemple : complexe de de Rham'
      page: 43
      pdf_page: 49
statements: 56
exercises: 18
content_sha256: e2aebd6606d20fdc1dbc7207888ea5e278df47782b80f42f0b99f84b7c375a72
translated_from: content/en-mt/alg/X/02_s2_complexes_de_a_modules.md
source_lang: en-mt
translation_method: machine
source_content_sha256: 861a391434771556fa8eb6b95600862c1fab35a9ef0810851b123295d669544a
translation_model: gpt-5.4
translation_run: translate-vi-8787b258
glossary_version: 34
glossary_terms_sha256: 8435ea42b4d01fd614eddcad79cffe7813c18c2f27e4b90cb60977eacdcaf97e
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 2. PHỨC CỦA A-MÔĐUN

*Trong đoạn này, $A$ ký hiệu một vành. Khi nói đến các $A$-môđun mà không nói rõ thêm, thì luôn luôn đó là các $A$-môđun trái.*

*Ta sẽ gọi các môđun phân bậc là các môđun phân bậc kiểu $\mathbf{Z}$ (II, p. 164).*

*Nếu $M$ là một $A$-môđun phân bậc, có phân bậc $(M_n)_{n\in\mathbf{Z}}$, ta đặt $M^n=M_{-n}$ và nói rằng $M_n$ (tương ứng $M^n$) là thành phần thuần nhất bậc giảm dần $n$ (tương ứng bậc tăng dần $n$) của $M$. Nếu $u:M\to N$ là một đồng cấu phân bậc bậc $p$ của các $A$-môđun phân bậc (II, p. 166), ta ký hiệu bởi $u_n:M_n\to M_{n+p}$ (tương ứng $u^n:M^n\to M^{n-p}$) đồng cấu suy ra từ $u$; nó được gọi là thành phần thuần nhất bậc giảm dần (tương ứng bậc tăng dần) $n$ của $u$; người ta cũng nói rằng $u$ có bậc giảm dần $p$ hoặc bậc tăng dần $-p$.*

### 1. Phức của A-Môđun

#### Định nghĩa 1 {#alg-x-s2-def-1 .statement}

*Một phức vi phân của các $A$-môđun là một cặp $(C,d)$ tạo bởi một $A$-môđun phân bậc $C$ và một tự đồng cấu $d:C\to C$ phân bậc bậc giảm dần $-1$ và sao cho $d\circ d=0$.*

Nó cũng được gọi là một phức của các $A$-môđun, hoặc một $A$-phức, hoặc một phức. Người ta thường viết C thay cho (C, d); tự đồng cấu d được gọi là vi phân của phức (C, d), hoặc nói lạm là của C.

Nếu C_n (tương ứng C^n) là thành phần thuần nhất bậc giảm dần (tương ứng bậc tăng dần) n của C, thì dữ kiện của d là tương đương với dữ kiện của dãy các đồng cấu

(1)
$$
\cdots \longrightarrow C_{n+1} \xrightarrow{d_{n+1}} C_n \xrightarrow{d_n} C_{n-1} \longrightarrow \cdots
$$
tương ứng

(1')
$$
\cdots \longrightarrow C^{n-1} \xrightarrow{d^{n-1}} C^n \xrightarrow{d^n} C^{n+1} \longrightarrow \cdots
$$
sao cho $d_n \circ d_{n+1} = 0$ với mọi $n \in \mathbf{Z}$ (tương ứng $d^n \circ d^{n-1} = 0$ với mọi $n \in \mathbf{Z}$). Nói lạm, người ta cũng sẽ gọi là phức dữ kiện của một dãy như thế các $A$-môđun và các đồng cấu.

Người ta sẽ nhận xét, như một phương tiện ghi nhớ, rằng khi “đi theo chiều của các mũi tên” trong các sơ đồ (1) và (1’), thì bậc giảm dần giảm xuống còn bậc tăng dần tăng lên.

Mọi $A$-môđun phân bậc sẽ mặc nhiên được xem như một phức bằng cách trang bị cho nó vi phân không; các phức như thế sẽ được gọi là các phức có vi phân không. Đặc biệt, mọi $A$-môđun M sẽ được trang bị cấu trúc $A$-phức duy nhất sao cho $M_0 = M^0 = M$. Phức (C, d) được gọi là không nếu C thu về 0. Trong phần sau, ta ký hiệu bởi 0 một phức không, được chọn một lần là xong.

Ghép thêm vào tập hợp có thứ tự $\mathbf{Z}$ hai phần tử ký hiệu là $-\infty$ và $+\infty$; ký hiệu bởi $\overline{\mathbf{Z}}$ tập hợp thu được, và trang bị cho nó quan hệ thứ tự mở rộng quan hệ của $\mathbf{Z}$ và sao cho $-\infty < n < +\infty$ với mọi $n \in \mathbf{Z}$; mọi tập con của $\overline{\mathbf{Z}}$ đều có một cận dưới lớn nhất và một cận trên lớn nhất.

Cho C là một phức; người ta gọi các cận phải và cận trái $^1$ của C là các phần tử $b_d(C)$ và $b_g(C)$ của $\overline{\mathbf{Z}}$ được xác định bởi
$$
b_d(C) = \inf \{ n \in \mathbf{Z}, C_n \neq 0 \}, \quad b_g(C) = \sup \{ n \in \mathbf{Z}, C_n \neq 0 \}.
$$
Người ta nói rằng C bằng không ở bên phải nếu $b_d(C) \geqslant 0$, bị chặn ở bên phải nếu $b_d(C) \neq -\infty$, bằng không ở bên trái nếu $b_g(C) \leqslant 0$, bị chặn ở bên trái nếu $b_g(C) \neq +\infty$; người ta nói rằng C bị chặn nếu
$$
b_d(C) \neq -\infty, \quad b_g(C) \neq +\infty.
$$
Người ta gọi độ dài $^2$ của C và ký hiệu bởi $l(C)$ phần tử của $\overline{\mathbf{Z}}$ được xác định như sau: nếu C bằng không, $l(C) = -\infty$; nếu C bị chặn và khác không, $l(C) = b_g(C) - b_d(C)$; nếu C

$^1$ Các từ phải và trái là tương đối đối với mô tả của C bằng các biểu đồ (1) và (1’).
$^2$ Không được lẫn khái niệm độ dài của phức $(C, d)$ với khái niệm độ dài của môđun C (II, p. 21).

không bị chặn, $l(C) = + \infty$. \* Với các quy ước của TG, IV, p. 13-17, luôn luôn có $l(C) = b_g(C) - b_d(C)$. \*

Ví dụ, nếu $k$ thành phần liên tiếp của $C$ khác không, các thành phần khác bằng không, thì có $l(C) = k - 1$ nếu $k > 0$, $l(C) = - \infty$ nếu $k = 0$.

Người ta nói rằng phức $(C, d)$ là tự do, xạ ảnh, phẳng, đơn ánh, nếu mỗi môđun $C_n$ đều như vậy. Ta sẽ lưu ý rằng phức $(C, d)$ là xạ ảnh hoặc phẳng khi và chỉ khi môđun $C$ như vậy (II, p. 39, mệnh đề 3 và X, p. 8, mệnh đề 4), nhưng $C$ có thể tự do mà phức $(C, d)$ lại không như vậy (vì một nhân tử trực tiếp của một môđun tự do không phải lúc nào cũng tự do); tương tự, $(C, d)$ có thể đơn ánh mà $C$ lại không như vậy (X, p. 170, bài tập 21).

Cho $(C, d)$ là một phức. Đặt $Z(C, d) = \mathrm{Ker}\,(d)$, $B(C, d) = \mathrm{Im}\,(d)$; đó là các môđun con phân bậc của $C$, được gọi tương ứng là môđun các chu trình và môđun các biên của $(C, d)$; các thành phần thuần nhất của $Z(C, d)$ và $B(C, d)$ được ký hiệu bởi $Z_n(C, d) = Z^{-n}(C, d)$, $B_n(C, d) = B^{-n}(C, d)$; ta có $Z_n(C, d) = \mathrm{Ker}\,(d_n)$, $B_n(C, d) = \mathrm{Im}\,(d_{n+1})$, $Z^n(C, d) = \mathrm{Ker}\,(d^n)$, $B^n(C, d) = \mathrm{Im}\,(d^{n-1})$.

Vì $d \circ d = 0$, ta có $B(C) \subset Z(C)$; hai chu trình được gọi là đồng điều nếu hiệu của chúng là một biên; môđun thương phân bậc $H(C, d) = Z(C, d)/B(C, d)$ được gọi là môđun đồng điều của $(C, d)$; các phần tử của nó là các lớp đồng điều; các thành phần thuần nhất của nó được ký hiệu bởi $H_n(C, d) = H^{-n}(C, d)$.

#### Ví dụ {#alg-x-s2-n1-exa-1 .statement}

Nếu $C$ có vi phân bằng không, ta có $Z(C) = C$, $B(C) = 0$ và $H(C)$ được đồng nhất một cách chính tắc với $C$.

Có các dãy khớp, được gọi là chính tắc:

(I$_n$) $$ 0 \to Z_n(C) \to C_n \xrightarrow{\delta_n} B_{n-1}(C) \to 0 $$
(II$_n$) $$ 0 \to B_n(C) \to Z_n(C) \to H_n(C) \to 0 $$
(III$_n$) $$ 0 \to B_n(C) \to C_n \to C_n/B_n(C) \to 0 $$
(IV$_n$) $$ 0 \to H_n(C) \to C_n/B_n(C) \xrightarrow{\overline{\delta}_n} B_{n-1}(C) \to 0 $$

trong đó $\delta_n$ và $\overline{\delta}_n$ được suy ra từ $d_n$. Ghép (IV$_n$) với (II$_{n-1}$), ta thu được dãy khớp

(V$_n$) $$ 0 \to H_n(C) \to C_n/B_n(C) \to Z_{n-1}(C) \to H_{n-1}(C) \to 0 , $$

dãy này cũng được viết, khi thay $n$ bằng $-n$,

(V$^n$) $$ 0 \to H^n(C) \to C^n/B^n(C) \to Z^{n+1}(C) \to H^{n+1}(C) \to 0 . $$

#### Định nghĩa 2 {#alg-x-s2-def-2 .statement}

Cho $(C, d)$ và $(C', d')$ là hai phức. Một cấu xạ $^1$ từ $(C, d)$ đến $(C', d')$ là một đồng cấu phân bậc A bậc 0 từ $C$ đến $C'$ sao cho
$$
d' \circ u = u \circ d .
$$

¹ Hoặc cấu xạ bậc 0 (x. X, p. 81).

Do đó, với mọi $n$, ta có $d'_n \circ u_n = u_{n-1} \circ d_n$ và ${d''}^n \circ u^n = u^{n+1} \circ d^n$. Ta có
$$
u(Z(C)) \subset Z(C') , \quad u(B(C)) \subset B(C') ,
$$
và ta ký hiệu bởi $Z(u) : Z(C) \to Z(C')$, $B(u) : B(C) \to B(C')$, $H(u) : H(C) \to H(C')$ các đồng cấu của các A-môđun được suy ra từ đó; các thành phần thuần nhất của các cấu xạ này được ký hiệu là $Z_n(u)$, $Z^n(u)$, ...

Nếu $v$ là một cấu xạ khác từ $(C, d)$ đến $(C', d')$, thì $u + v$ là một cấu xạ từ $(C, d)$ đến $(C', d')$, và ta có
$$
Z(u + v) = Z(u) + Z(v) , \quad B(u + v) = B(u) + B(v) , \quad H(u + v) = H(u) + H(v) .
$$
Tương tự, nếu $A$ là một đại số trên một vành giao hoán $k$, và nếu $\lambda \in k$, thì $\lambda u$ là một cấu xạ từ $(C, d)$ đến $(C', d')$ và ta có
$$
Z(\lambda u) = \lambda Z(u) , \quad B(\lambda u) = \lambda B(u) , \quad H(\lambda u) = \lambda H(u) .
$$
Nếu $u' : (C', d') \to (C'', d'')$ là một cấu xạ khác của các phức, thì $u' \circ u$ là một cấu xạ từ $(C, d)$ đến $(C'', d'')$ và ta có
$$
Z(u' \circ u) = Z(u') \circ Z(u) , \quad B(u' \circ u) = B(u') \circ B(u) , \quad H(u' \circ u) = H(u') \circ H(u) .
$$
Hiển nhiên một cấu xạ song ánh là một đẳng cấu.

#### Định nghĩa 3 {#alg-x-s2-def-3 .statement}

Cho $(C, d)$ và $(C', d')$ là hai phức. Một đẳng cấu đồng điều (hay giả đẳng cấu) từ $(C, d)$ đến $(C', d')$ là một cấu xạ $u$ từ $(C, d)$ đến $(C', d')$ sao cho $H(u)$ là song ánh.

Mọi đẳng cấu đều là một đẳng cấu đồng điều, mọi cấu xạ hợp thành bởi các đẳng cấu đồng điều đều là một đẳng cấu đồng điều.

Ta nói rằng $(C, d)$ có đồng điều không nếu $H(C) = 0$, nghĩa là nếu cấu xạ duy nhất của các phức $0 \to C$ (resp. $C \to 0$) là một đẳng cấu đồng điều. Ta nói rằng $(C, d)$ là acyclic theo bậc giảm dần $n$ (resp. theo bậc tăng dần $n$) nếu $H_n(C) = 0$ (resp. $H^n(C) = 0$).

Cho $(C, d)$ là một phức và $p \in \mathbf{Z}$. Bản dịch thứ $p$ của $(C, d)$ là phức $(C(p), d(p))$ thu được như sau: $C(p)$ là A-môđun thu được bằng cách tịnh tiến phân bậc của $C$ đi $p$ (II, p. 163; Ví dụ 3), sao cho
$$
C(p)_n = C_{n+p} , \quad C(p)^n = C^{n-p} ;
$$
đặc biệt $C(p)_0 = C_p$; chú ý thêm rằng $C$ là tổng trực tiếp của các môđun con phân bậc $C_p(-p)$, $p \in \mathbf{Z}$ (resp. $C^p(p)$, $p \in \mathbf{Z}$). Ta đặt $d(p) = (-1)^p d$.
Ta có $Z(C(p)) = Z(C)(p)$, $B(C(p)) = B(C)(p)$ và $H(C(p)) = H(C)(p)$.

Ví dụ, $d$ là một cấu xạ của các phức từ $C$ đến $C(-1)$ và
$$
H(d) : H(C) \to H(C)(-1)
$$
là không.

Với mọi cấu xạ của các phức $u : (C,d) \to (C',d')$, và mọi $p \in \mathbf{Z}$, $u$ cũng là một cấu xạ từ $(C(p),d(p))$ đến $(C'(p),d'(p))$; đôi khi nó được ký hiệu là $u(p)$ và ta có
$$
u(p)_n = u_{n+p}, \qquad u(p)^n = u^{n-p}.
$$

### 2. Các phép toán trên các phức

Trên tập hợp $A \times A$, hai luật
$$
(a,b) + (a',b') = (a+a',b+b')
$$
$$
(a,b)(a',b') = (aa',ab'+ba')
$$
định nghĩa một cấu trúc vành, ký hiệu là $A(\varepsilon)$, với phần tử đơn vị $1=(1,0)$; đơn ánh $a \mapsto (a,0)=a1$ cho phép ta đồng nhất $A$ với một vành con của $A(\varepsilon)$; môđun $A(\varepsilon)$ là tự do với cơ sở $\{1,\varepsilon\}$ trong đó $\varepsilon=(0,1)$; ta có $\varepsilon^2=0$ và $\varepsilon$ là trung tâm trong $A(\varepsilon)$.

Khi $A$ giao hoán, $A(\varepsilon)$ là một đại số số đối ngẫu trên $A$ (III, p. 15).

Hãy trang bị cho $A(\varepsilon)$ phân bậc vành (II, p. 164) mà đối với nó $A(\varepsilon)_0 = A\mathbin{.}1$, $A(\varepsilon)_{-1} = A\mathbin{.}\varepsilon$, và $A(\varepsilon)_n = 0$ với $n \neq 0, -1$. Rõ ràng việc cho một cấu trúc phức trên $A$ trên một tập hợp $C$ là tương đương với việc cho trên $C$ một cấu trúc $A(\varepsilon)$-môđun phân bậc, vi phân $d$ tương ứng với phép vị tự $\varepsilon_C$; tương tự, các cấu xạ của phức tương ứng với các đồng cấu phân bậc bậc 0 của các $A(\varepsilon)$-môđun phân bậc. Do đó loài các cấu trúc $A(\varepsilon)$-môđun phân bậc và các cấu trúc phức trên $A$ là tương đương (E, IV, p. 9-10). Chúng ta sẽ dùng sự kiện này để chuyển sang lý thuyết các phức các khái niệm thông thường của lý thuyết môđun phân bậc.

Với khái niệm môđun con phân bậc của $A(\varepsilon)$ tương ứng khái niệm phức con: như vậy, một phức con của phức $(C,d)$ là một môđun con phân bậc $C'$ của $C$ sao cho, với mọi $n \in \mathbf{Z}$, $d_n(C'_n) \subset C'_{n-1}$; nếu ta ký hiệu bởi $d'$ đồng cấu phân bậc của $A$ từ $C'$ vào $C'$ cảm sinh bởi $d$, thì $(C', d')$ là một cấu trúc phức, gọi là cấu trúc cảm sinh bởi $(C,d)$. Trừ khi được nói tường minh ngược lại, mọi phức con đều được giả thiết là được trang bị cấu trúc cảm sinh.

Chúng tôi để bạn đọc tự triển khai theo cùng cách các khái niệm phức thương, dãy khớp của các phức, hạt nhân, đối hạt nhân, ảnh của một cấu xạ của các phức, theo từ điển dưới đây:

$$
\begin{array}{rcl}
A(\varepsilon)\text{-môđun phân bậc thương} & = & \textit{phức thương},\\[2mm]
\left.
\begin{array}{l}
\text{hạt nhân, đối hạt nhân, ảnh của một }A(\varepsilon)\text{-}\\
\text{đồng cấu phân bậc bậc 0}
\end{array}
\right\} & = &
\begin{array}{l}
\textit{hạt nhân, đối hạt nhân, ảnh của một cấu xạ}\\
\textit{của các phức},
\end{array}\\[4mm]
\left.
\begin{array}{l}
\text{dãy khớp của các }A(\varepsilon)\text{-môđun phân bậc và các đồng cấu phân bậc}\\
\text{bậc 0}
\end{array}
\right\} & = & \textit{dãy khớp của các phức.}
\end{array}
$$

Ví dụ, các dãy khớp chính tắc của No. 1 cho các dãy khớp chính tắc của các phức:

(I) $0 \to Z(C) \to C \xrightarrow{\delta} B(C) (-1) \to 0$,
(II) $0 \to B(C) \to Z(C) \to H(C) \to 0$,
(III) $0 \to B(C) \to C \to C/B(C) \to 0$,
(IV) $0 \to H(C) \to C/B(C) \xrightarrow{\delta} B(C) (-1) \to 0$,
(V) $0 \to H(C) \to C/B(C) \to Z(C) (-1) \to H(C) (-1) \to 0$.

Ta định nghĩa tương tự các khái niệm tổng trực tiếp của các phức, hệ quy nạp của các phức, giới hạn quy nạp của một hệ quy nạp các phức.

Cho $(C_i, d_i)$ là một họ các phức. Ta gọi tích của họ này và ký hiệu $\prod_{i \in I} (C_i, d_i)$ là phức $(C, d)$ thu được như sau:

a) với mỗi $n \in \mathbf{Z}$, $C_n$ là A-môđun tích $\prod_{i \in I} (C_i)_n$ của các thành phần thuần nhất $(C_i)_n$ của các phức đã cho,
b) với mỗi $n \in \mathbf{Z}$, $d_n : C_n \to C_{n-1}$ là đồng cấu thành phần A $(d_i)_n$.

Khi $I$ là hữu hạn, $\prod_{i \in I} (C_i, d_i)$ bằng $\bigoplus_{i \in I} (C_i, d_i)$. Cần chú ý rằng nói chung, A-môđun nền của phức tích $\prod_{i \in I} (C_i, d_i)$ không phải là A-môđun tích $\prod_{i \in I} C_i$.

Xét một họ (tương ứng, một hệ quy nạp lọc) các phức $(C_i)_{i \in I}$. Gọi $C$ là tổng trực tiếp (tương ứng, giới hạn quy nạp) của các $C_i$, và gọi $\alpha_i : C_i \to C$ là các đồng cấu chính tắc. Khi đó các $H(\alpha_i) : H(C_i) \to H(C)$ xác định một đồng cấu phân bậc chính tắc bậc 0 từ $\bigoplus_{i \in I} H(C_i)$ (tương ứng, $\varprojlim_{i \in I} H(C_i)$) vào $H(C)$. Tương tự, các phép chiếu chính tắc $\prod_{i \in I} C_i \to C_i$ xác định một đồng cấu phân bậc chính tắc bậc 0 từ $H(\prod_{i \in I} C_i)$ vào $\prod_{i \in I} H(C_i)$.

#### Mệnh đề 1 {#alg-x-s2-prop-1 .statement}

Với mọi họ các phức $(C_i)_{i \in I}$, các đồng cấu chính tắc
$$
\bigoplus_{i \in I} H(C_i) \to H(\bigoplus_{i \in I} C_i), \quad H(\prod_{i \in I} C_i) \to \prod_{i \in I} H(C_i)
$$
đều là song ánh.

Với mọi hệ quy nạp lọc các phức $(C_i)_{i \in I}$, đồng cấu chính tắc
$$
\varprojlim_{i \in I} H(C_i) \to H(\varprojlim_{i \in I} C_i)
$$
là song ánh.

Điều này suy ra ngay lập tức từ II, p. 14, cor. 1 to prop. 7, p. 11, cor. to prop. 5, và p. 91, prop. 3.

### 3. Đồng cấu nối và dãy đồng điều khớp

Trong số này, ta xét một dãy khớp các phức
$$
0 \longrightarrow C' \xrightarrow{u} C \xrightarrow{v} C'' \longrightarrow 0 ;
$$
ta ký hiệu bởi cùng một chữ $d$ các vi phân của $C, C'$ và $C''$.

Gọi $\Gamma$ là tập hợp các $x \in C$ sao cho $dx \in \operatorname{Im}(u)$; với $x \in \Gamma$, ta có
$$
d(\bar{u}^{-1}(dx)) = \bar{u}^{-1}(dd(x)) = 0 ,
$$
do đó $\bar{u}^{-1}(dx) \in Z(C')$; ta cũng có $dv(x) = v(dx) \in \operatorname{Im}(v \circ u) = 0$, do đó $v(x) \in Z(C'')$; khi đó ta xét ánh xạ tuyến tính $\varphi : \Gamma \to H(C'') \times H(C')$ ánh xạ mỗi phần tử $x \in \Gamma$ lên lớp của $(v(x), \bar{u}^{-1}(dx))$.

#### Bổ đề 1 {#alg-x-s2-lem-1 .statement}

Ảnh $\varphi(\Gamma)$ của $\Gamma$ trong $H(C'') \times H(C')$ là đồ thị của một A-đồng cấu phân bậc bậc $-1$ từ $H(C'')$ vào $H(C')$.

a) Nếu $x \in \Gamma$ và nếu $v(x) \in B(C'')$, thì $\bar{u}^{-1}(dx) \in B(C')$ : thực vậy, tồn tại $z'' \in C''$ sao cho $v(x) = dz''$, khi đó tồn tại $z \in C$ sao cho $z'' = v(z)$, do đó $v(x) = v(dz)$, rồi tồn tại $t' \in C'$ sao cho $x - dz = u(t')$, suy ra $dx = u(dt')$, do đó $\bar{u}^{-1}(dx) = dt' \in B(C')$.

b) Mọi phần tử của $Z(C'')$ đều là ảnh bởi $v$ của một phần tử $x$ của $C$ sao cho $v(dx) = 0$, tức là $dx \in \operatorname{Im} u$, nghĩa là sao cho $x \in \Gamma$.

c) Từ a) và b) suy ra rằng $\varphi(\Gamma)$ thực sự là một đồ thị phiếm hàm; vì $\varphi$ là song thuần nhất với song bậc $(0, -1)$, điều này hoàn tất chứng minh.

Đồng cấu phân bậc bậc $-1$ từ $H(C'')$ vào $H(C')$ do đó được xác định được gọi là đồng cấu nối liên kết với dãy khớp $(u, v)$; nó được ký hiệu là $\partial(u, v)$ hoặc $\partial_{u,v}$ hoặc đơn giản là $\partial$. Các thành phần thuần nhất của nó được ký hiệu
$$
\partial_n(u, v) : H_n(C'') \to H_{n-1}(C') \quad \text{và} \quad \partial^n(u, v) : H^n(C'') \to H^{n+1}(C') .
$$

Theo định nghĩa, để xây dựng ảnh của một lớp $\alpha \in H_n(C'')$ bởi $\partial$, ta chọn một chu trình $z'' \in Z_n(C'')$ trong lớp $\alpha$, rồi một phần tử $x$ của $C_n$ sao cho $v(x) = z''$; khi đó $dx$ có dạng $u(t')$, $t' \in C'_{n-1}$, và $\partial(\alpha)$ là lớp đồng điều của $t'$.

Xét theo các sự tương ứng, do đó $\partial_n(u, v)$ thu được từ sự tương ứng $\bar{u}_{n-1}^{-1} \circ d_n \circ \bar{v}_n^{-1}$ giữa $C''_n$ và $C'_{n-1}$, bằng cách chuyển qua các tập con $Z_n(C'')$ và $Z_{n-1}(C')$, rồi đến các thương của chúng $H_n(C'')$ và $H_{n-1}(C')$. Điều này đặc biệt cho thấy rằng, nếu thay $C, C', C'', u, v$ bởi $C(p), C'(p), C''(p), u(p), v(p)$, ta có
$$
\partial(u(p), v(p)) = (-1)^p \partial(u, v) ;
$$
tương tự, nếu $\lambda$ và $\mu$ là hai phần tử khả nghịch của tâm của $A$, thì ta có
$$
\partial(\lambda u, \mu v) = \lambda^{-1} \mu^{-1} \partial(u, v) .
$$

Ta cũng có thể liên hệ $\partial(u, v)$ với biểu đồ con rắn (X, p. 4). Theo loc. cit., mệnh đề 2, các dãy
$$
0 \longrightarrow Z_n(C') \xrightarrow{Z_n(u)} Z_n(C) \xrightarrow{Z_n(v)} Z_n(C'')
$$

và

$$
C'_n/B_n(C') \xrightarrow{\overline{u}_n} C_n/B_n(C) \xrightarrow{\overline{v}_n} C''_n/B_n(C'') \longrightarrow 0 ,
$$

trong đó $\overline{u}_n$ và $\overline{v}_n$ được suy ra từ $u$ và $v$, là khớp. Dùng các dãy khớp chính tắc $(V_n)$, ta thu được một *biểu đồ giao hoán* với các hàng và cột khớp

$$
\begin{array}{ccccccccc}
&&0&&0&&0&&\\
&&\downarrow&&\downarrow&&\downarrow&&\\
&&H_n(C')&\xrightarrow{H_n(u)}&H_n(C)&\xrightarrow{H_n(v)}&H_n(C'')&&\\
&&\downarrow&&\downarrow&&\downarrow&&\\
0&\longrightarrow&C'_n/B_n(C')&\xrightarrow{\overline{u}_n}&C_n/B_n(C)&\xrightarrow{\overline{v}_n}&C''_n/B_n(C'')&\longrightarrow&0\\
&&\downarrow&&\downarrow&&\downarrow&&\\
0&\longrightarrow&Z_{n-1}(C')&\xrightarrow{Z_{n-1}(u)}&Z_{n-1}(C)&\xrightarrow{Z_{n-1}(v)}&Z_{n-1}(C'')&&\\
&&\downarrow&&\downarrow&&\downarrow&&\\
&&H_{n-1}(C')&\xrightarrow{H_{n-1}(u)}&H_{n-1}(C)&\xrightarrow{H_{n-1}(v)}&H_{n-1}(C'')&&\\
&&\downarrow&&\downarrow&&\downarrow&&\\
&&0&&0&&0&&
\end{array}
$$

Đồng cấu $H_n(C'')\to H_{n-1}(C')$ liên kết với biểu đồ này (loc. cit., mệnh đề 2, (iii)) trùng theo phép dựng với $\partial_n(u,v).$ Điều này hơn nữa kéo theo rằng dãy các đồng cấu $(H_n(u),\ H_n(v),\ \partial_n(u,v),\ H_{n-1}(u),\ H_{n-1}(v))$ là khớp; do đó:

#### Định lý 1 {#alg-x-s2-thm-1 .statement}

*Dãy vô hạn các đồng cấu của các* $A$-*môđun*

$$
\cdots \longrightarrow H_{n+1}(C'') \xrightarrow{\partial_{n+1}(u,v)} H_n(C') \xrightarrow{H_n(u)} H_n(C) \xrightarrow{H_n(v)} H_n(C'')
$$

$$
\xrightarrow{\partial_n(u,v)} H_{n-1}(C') \xrightarrow{H_{n-1}(u)} H_{n-1}(C) \xrightarrow{H_{n-1}(v)} H_{n-1}(C'') \xrightarrow{\partial_{n-1}(u,v)} H_{n-2}(C') \longrightarrow \cdots
$$

*là khớp.*

Dãy này được gọi là *dãy đồng điều khớp* liên kết với dãy khớp $(u,v)$; đôi khi nó được viết dưới dạng một *tam giác khớp của các* $A$-*môđun*

$$
\begin{array}{ccc}
&&H(C)\\
&\nearrow^{H(u)}&\searrow^{H(v)}\\
H(C')&\xleftarrow{\partial(u,v)}&H(C'') .
\end{array}
$$

#### Hệ quả 1 {#alg-x-s2-thm-1-cor-1 .statement}

*Nếu hai trong các phức* $C$, $C'$, $C''$ *có đồng điều bằng không, thì phức thứ ba cũng vậy. Để* $u$ *(tương ứng.* $v$*) là một đồng cấu, điều kiện cần và đủ là* $C''$ *(tương ứng.* $C'$*) *có đồng điều bằng không. Để* $\partial(u,v)$ *là song ánh, điều kiện cần và đủ là* $C$ *có đồng điều bằng không.*

#### Hệ quả 2 {#alg-x-s2-thm-1-cor-2 .statement}

Cho u là một cấu xạ của các phức. Nếu Ker u và Coker u có đồng điều bằng không, thì u là một đồng cấu trên đồng điều.

Thật vậy, cho u : E → E’ là một cấu xạ của các phức. Nếu Ker u (tương ứng. Coker u) có đồng điều bằng không, thì cấu xạ chính tắc E → Im u (tương ứng. Im u → E’) là một đồng cấu trên đồng điều theo Hệ quả 1.

#### Mệnh đề 2 {#alg-x-s2-prop-2 .statement}

Xét một biểu đồ giao hoán các phức với các hàng khớp

$$
\begin{array}{ccccccccc}
0 & \longrightarrow & C' & \xrightarrow{u} & C & \xrightarrow{v} & C'' & \longrightarrow & 0 \\
& & f' \downarrow & & f \downarrow & & f'' \downarrow & & \\
0 & \longrightarrow & C'_1 & \xrightarrow{u_1} & C_1 & \xrightarrow{v_1} & C''_1 & \longrightarrow & 0 .
\end{array}
$$

Khi đó $\mathrm{H}(f') \circ \partial(u, v) = \partial(u_1, v_1) \circ \mathrm{H}(f'')$.

Cho $\alpha'' \in \mathrm{H}(C'')$; cho $z''$ là một chu trình có lớp $\alpha''$ và $x$ là một phần tử của $C$ sao cho $v(x) = z''$. Ta có
$$
(\partial_{u_1, v_1} \circ \mathrm{H}(f'')) (\alpha'') = \partial_{u_1, v_1}(\overline{f''(z'')}) = \overline{u_1^{-1}(df(x))} = \overline{f'(u_1^{-1}(dx))} =
= \mathrm{H}(f') (\overline{u^{-1}(dx)}) = (\mathrm{H}(f') \circ \partial_{u, v}) (\alpha'') .
$$

#### Ví dụ {#alg-x-s2-n3-exa-1 .statement}

Cho $C$ là một phức. Xét dãy khớp chính tắc

(I)
$$
0 \longrightarrow Z(C) \xrightarrow{j} C \xrightarrow{\delta} B(C) (-1) \longrightarrow 0 ,
$$
và cho $i : B(C) \to Z(C)$ là đơn ánh chính tắc. Khi đó đồng cấu nối $\partial(j, \delta) : \mathrm{H}(B(C)) (-1) \to \mathrm{H}(Z(C)) (-1)$ được đồng nhất với $\mathrm{H}(i) (-1)$, như ta kiểm tra ngay được. Vì $\mathrm{H}(\delta) = 0$, dãy khớp đồng điều gắn với (I) phân tách thành các dãy khớp ngắn

(II_n)
$$
0 \longrightarrow B_n(C) \xrightarrow{i} Z_n(C) \xrightarrow{\mathrm{H}(j)} H_n(C) \longrightarrow 0 .
$$

\* Ánh xạ :

1) Đồng điều kỳ dị

Cho $A$ là một vành. Với mọi không gian tôpô $X$, ta định nghĩa phức kỳ dị $C(X, A)$ của $X$ với hệ số trong $A$ như sau:

Trong $\mathbf{R}^{(N)}$, ký hiệu $(e_n)$ là cơ sở chính tắc; ta gọi đơn hình chính tắc $n$ là bao lồi $\Delta_n$ của $\{ e_0, ..., e_n \}$. Với $i \in \{ 0, ..., n \}$, ta định nghĩa ánh xạ afin $\iota_i : \Delta_{n-1} \to \Delta_n$ bởi $\iota_i(e_k) = e_k$ nếu $k < i$ và $\iota_i(e_k) = e_{k+1}$ nếu $k \geq i$. Ta ký hiệu $C_n(X, A)$ là A-môđun $A^{(\Sigma_n(X))}$, trong đó $\Sigma_n(X)$ là tập hợp các ánh xạ liên tục từ $\Delta_n$ vào $X$; với $n < 0$, ta đặt $C_n = 0$. Với $i \in \{ 0, ..., n \}$, ta định nghĩa ánh xạ tuyến tính $\partial_{n, i} : C_n(X, A) \to C_{n-1}(X, A)$ bởi $\partial_{n, i}(e_s) = e_{s \circ \iota_i}$ với $s \in \Sigma_n(X)$, và ta đặt $d_n = \Sigma (-1)^i \partial_{n, i}$. Ta kiểm tra rằng

$$
... C_n(X, A) \xrightarrow{d_n} C_{n-1}(X, A) \to ...
$$

là một phức. Đồng điều của nó được gọi là đồng điều kỳ dị của $X$ với hệ số trong $A$ và được ký hiệu là $\mathrm{H}(X, A)$ hoặc đơn giản là $\mathrm{H}(X)$.

Nếu $Y$ là một không gian con của $X$, ta ký hiệu $C(X, Y, A)$ là phức thương $C(X, A)/C(Y, A)$, và $\mathrm{H}(X, Y, A)$ là đồng điều của nó. Suy ra từ Định lý 1 rằng có một dãy khớp:

$$
... \to \mathrm{H}_n(Y, A) \to \mathrm{H}_n(X, A) \to \mathrm{H}_n(X, Y, A) \to \mathrm{H}_{n-1}(Y, A) \to \mathrm{H}_{n-1}(X, A) \to ...
$$

2) Phân tích tế bào hữu hạn

Cho $X$ là một không gian tôpô tách biệt. Một phân tích tế bào hữu hạn của $X$ được cho bởi một dãy tăng $(X_n)_{n \in \mathbf{Z}}$ các không gian con đóng của $X$ thỏa mãn các điều kiện sau:
(i) $X_n = \varnothing$ với $n < 0$;
(ii) tồn tại một $N$ sao cho $X_N = X$ (do đó $X_n = X$ với $n > N$);
(iii) với mọi $n$, không gian $X_n - X_{n-1}$ chỉ có một số hữu hạn thành phần liên thông, gọi là các tế bào $n$-chiều;
(iv) với mọi $n$, và với mọi thành phần liên thông $C$ của $X_n - X_{n-1}$, tồn tại một đồng phôi từ quả cầu Euclid mở $n$-chiều $\hat{B}_n$ (TG, VI, p. 10) lên $C$ mở rộng thành một ánh xạ liên tục của quả cầu đóng vào $X$.

Có thể chứng minh rằng các điều kiện này kéo theo $\mathrm{H}_n(X_n, X_{n-1}, A)$ là một A-môđun tự do $\Gamma_n$ có hạng bằng số các tế bào $n$-chiều, và $\mathrm{H}_i(X_n, X_{n-1}, A) = 0$ với $i \neq n$. Ta có $C(X_n, X_{n-1}, A) = C(X_n, X_{n-2}, A)/C(X_{n-1}, X_{n-2}, A)$, do đó có một dãy khớp

$$
\mathrm{H}_n(X_n, X_{n-2}) \longrightarrow \mathrm{H}_n(X_n, X_{n-1}) \xrightarrow{d_n} \mathrm{H}_{n-1}(X_{n-1}, X_{n-2}) \longrightarrow \mathrm{H}_{n-1}(X_n, X_{n-2}) ,
$$

trong đó xuất hiện một đồng cấu nối $d_n : \Gamma_n \to \Gamma_{n-1}$. Ta có $d_n \circ d_{n+1} = 0$, điều này cho phép định nghĩa một phức $\Gamma : \cdots \to \Gamma_n \xrightarrow{d_n} \Gamma_{n-1} \to \cdots$.

Dãy khớp

(Ghi chú: Dòng cuối cùng "Dãy khớp" được để lại như một phần của văn bản vì nguồn kết thúc ở đó.)

$$
H_{n+1}(X_p, X_{p-1}) \to H_n(X_{p-1}) \to H_n(X_p) \to H_n(X_p, X_{p-1}) \to H_{n-1}(X_{p-1})
$$

cho thấy bằng quy nạp theo p rằng $H_n(X_p) = 0$ với $p < n$, rằng $H_n(X_n) = \mathrm{Ker}\,(d_n : \Gamma_n \to \Gamma_{n-1})$ và rằng $H_n(X_p) = H_n(\Gamma)$ với $p > n$. Đặc biệt $H_n(X)$ được đồng nhất với $H_n(\Gamma)$.

#### Ví dụ {#alg-x-s2-n3-exa-2 .statement}

Xét tích các mặt cầu $S_2 \times S_2$ và không gian xạ ảnh phức $P_2(\mathbf{C})$.
Cho $b \in S_2$, ta định nghĩa một phân tích tế bào $(Y_n)$ của $Y = S_2 \times S_2$ bằng cách đặt

$$
Y_0 = Y_1 = \{ (b, b) \} , \quad Y_2 = Y_3 = (\{ b \} \times S_2) \cup (S_2 \times \{ b \}) \quad \text{và} \quad Y_4 = S_2 \times S_2 ;
$$

phân tích này có một tế bào chiều 0, hai tế bào chiều 2 và một tế bào chiều 4. Các vi phân của phức liên kết tất yếu bằng không, nên $H_0(Y)$, $H_2(Y)$ và $H_4(Y)$ lần lượt là tự do có hạng 1, 2 và 1, và $H_n(Y) = 0$ với $n \notin \{ 0, 2, 4 \}$.
Ta thu được một phân tích tế bào $(Z_n)$ của $P_2(\mathbf{C})$ bằng cách đặt

$$
Z_0 = Z_1 = \{ c \} , \quad Z_2 = Z_3 = P_1(\mathbf{C}) , \quad Z_4 = P_2(\mathbf{C}) ,
$$

không gian $P_1(\mathbf{C})$ được nhúng vào $P_2(\mathbf{C})$ (TG, VIII, p. 20), và c là một điểm của $P_1(\mathbf{C})$; sự phân tích này có một ô chiều 0, một ô chiều 2 và một ô chiều 4. Ở đây nữa các vi phân của phức tất yếu đều bằng không, và suy ra rằng $H_n(P_2(\mathbf{C}))$ đẳng cấu với A đối với $n \in \{ 0, 2, 4 \}$ và đẳng cấu với 0 trong các trường hợp khác.
Vì các môđun đồng điều ở bậc 2 của hai không gian được xét lần lượt là tự do hạng 2 và 1, nên các không gian này không đồng phôi. \*

### 4. Đồng luân

#### Định nghĩa 4 {#alg-x-s2-def-4 .statement}

Cho $(C, d)$ và $(C', d')$ là hai phức, $f$ và $g$ là hai cấu xạ từ $C$ đến $C'$. Một đồng luân nối $f$ với $g$ là mọi A-đồng cấu phân bậc $s$ bậc 1 từ $C$ đến $C'$ sao cho $g - f = d' \circ s + s \circ d$.
Ta nói rằng $f$ và $g$ đồng luân nếu tồn tại một đồng luân nối $f$ với $g$.
Nếu $h$ là một cấu xạ thứ ba từ $C$ đến $C'$ và nếu $s$ (resp. $t$) là một đồng luân nối $f$ với $g$ (resp. $g$ với $h$), thì $s + t$ là một đồng luân nối $f$ với $h$; do đó, quan hệ « $f$ và $g$ là hai cấu xạ đồng luân từ $C$ đến $C'$ » là một quan hệ tương đương, mà các lớp của nó được gọi là *các lớp đồng luân của các cấu xạ từ $C$ đến $C'$*.

Cho hai không gian tôpô $X$ và $Y$, và một ánh xạ liên tục $f : X \to Y$, người ta định nghĩa một ánh xạ tuyến tính $f_*$ từ phức kỳ dị (*xem No. 3*) $C(X, A)$ vào $C(Y, A)$ bằng cách đặt $f_*(e_s) = e_{f \circ s}$ với $s \in \Sigma_n(X)$. Ánh xạ này là một cấu xạ của các phức.
Hai ánh xạ liên tục $f$ và $g$ từ $X$ vào $Y$ được gọi là *đồng luân* theo nghĩa tôpô nếu tồn tại một ánh xạ liên tục $h$ từ $[0, 1] \times X$ vào $Y$ sao cho $h(0, x) = f(x)$ và $h(1, x) = g(x)$ với mọi $x \in X$. Người ta chứng minh rằng, nếu $f$ và $g$ đồng luân theo nghĩa tôpô, thì các cấu xạ $f_*$ và $g_*$ là đồng luân theo nghĩa của Định nghĩa 4 ở trên. Chính sự kiện này là nguồn gốc của thuật ngữ dùng trong đại số.

#### Mệnh đề 3 {#alg-x-s2-prop-3 .statement}

*Nếu $f$ và $g$ là hai cấu xạ đồng luân từ $C$ vào $C'$, thì $\mathrm{H}(f) = \mathrm{H}(g)$.* Gọi $s$ là một đồng luân nối $f$ với $g$. Ta có
$$
(g - f)(\mathbf{Z}(C)) = (d' \circ s + s \circ d)(\mathbf{Z}(C)) = (d' \circ s)(\mathbf{Z}(C)) \subset \mathbf{B}(C') ,
$$
do đó $\mathrm{H}(g - f) = 0$ và $\mathrm{H}(g) = \mathrm{H}(f)$.

#### Hệ quả {#alg-x-s2-n4-cor-1 .statement}

*Một cấu xạ đồng luân với một đẳng cấu đồng điều là một đẳng cấu đồng điều.*

#### Mệnh đề 4 {#alg-x-s2-prop-4 .statement}

*Cho $C, C', D, D'$ là bốn phức, $f : C \to C'$, $g : C \to C'$, $u : D \to C$, $v : C' \to D'$ là bốn cấu xạ. Nếu $s$ là một đồng luân nối $f$ với $g$, thì $v \circ s \circ u$ là một đồng luân nối $v \circ f \circ u$ với $v \circ g \circ u$. Nếu $f$ và $g$ đồng luân, thì $v \circ f \circ u$ và $v \circ g \circ u$ cũng đồng luân.*
Điều này là hiển nhiên.

#### Hệ quả {#alg-x-s2-n4-cor-2 .statement}

*Cho $C, C', C''$ là ba phức, $f$ và $g$ là hai cấu xạ từ $C$ vào $C'$, $f_1$ và $g_1$ là hai cấu xạ từ $C'$ vào $C''$. Nếu $s$ và $s_1$ là các đồng luân nối $f$ với $g$ và $f_1$ với $g_1$ tương ứng, thì $s_1 \circ f + g_1 \circ s$ là một đồng luân nối $f_1 \circ f$ với $g_1 \circ g$. Nếu $f$ và $f_1$ đồng luân với $g$ và $g_1$ tương ứng, thì $f_1 \circ f$ đồng luân với $g_1 \circ g$.
Thật vậy, $s_1 \circ f$ nối $f_1 \circ f$ với $g_1 \circ f$ và $g_1 \circ s$ nối $g_1 \circ f$ với $g_1 \circ g$.*

#### Định nghĩa 5 {#alg-x-s2-def-5 .statement}

*Một cấu xạ của các phức $f : C \to C'$ được gọi là một đồng luân tương đương nếu tồn tại một cấu xạ $f' : C' \to C$ sao cho $f' \circ f$ và $f \circ f'$ đồng luân với $1_C$ và $1_{C'}$ tương ứng.*

Hiển nhiên khi đó $f'$ cũng là một đồng luân tương đương; người ta cũng nói rằng $f'$ là *nghịch đảo của $f$ đối với đồng luân*. Nếu $f'$ và $f'_1$ đều là các nghịch đảo của $f$ đối với đồng luân, thì $f'$ và $f'_1$ đồng luân với nhau (thật vậy theo hệ quả trước đó, $f'_1 = f'_1 \circ 1_{C'}$ đồng luân với $f'_1 \circ f \circ f'$, nên đồng luân với $1_C \circ f' = f'$).

#### Mệnh đề 5 {#alg-x-s2-prop-5 .statement}

*Một đồng luân tương đương là một đồng điều tương đương; một cấu xạ là hợp thành của các đồng luân tương đương là một đồng luân tương đương. Một cấu xạ đồng luân với một đồng luân tương đương là một đồng luân tương đương.*

Cho $f : C \to C'$ và $f_1 : C' \to C''$ là các đồng luân tương đương của các phức, $f' : C' \to C$ và $f'_1 : C'' \to C'$ là các cấu xạ nghịch đảo đến đồng luân. Ta có
$$
\mathrm{H}(f') \circ \mathrm{H}(f) = \mathrm{H}(f' \circ f) = \mathrm{H}(1_C) = 1_{\mathrm{H}(C)} \quad (\text{prop. 3})
$$

và tương tự $\mathrm{H}(f) \circ \mathrm{H}(f') = 1_{\mathrm{H}(C')}$, nên $\mathrm{H}(f)$ là song ánh và $f$ là một đẳng cấu đồng điều. Mặt khác, $(f' \circ f'_1) \circ (f_1 \circ f)$ đồng luân với $f' \circ 1_C' \circ f$ (mệnh đề 4), do đó với $1_C$; tương tự, $(f_1 \circ f) \circ (f' \circ f'_1)$ đồng luân với $1_{C''}$ và $f_1 \circ f$ là một tương đương đồng luân. Sau cùng, nếu $g : C \to C'$ là một cấu xạ đồng luân với $f$, thì $f' \circ g$ đồng luân với $f' \circ f$, do đó với $1_C$; tương tự, $g \circ f'$ đồng luân với $f \circ f'$, do đó với $1_{C'}$ và $g$ là một tương đương đồng luân.

#### Hệ quả {#alg-x-s2-n4-cor-3 .statement}

Cho $C, C', D, D'$ là bốn phức, $f : C \to C'$ là một cấu xạ, $u : D \to C$ và $v : C' \to D'$ là các tương đương đồng luân. Để $v \circ f \circ u$ là một tương đương đồng luân (tương ứng, một đẳng cấu đồng điều), điều kiện cần và đủ là $f$ là như vậy.

Nếu $f$ là một tương đương đồng luân (tương ứng, một đẳng cấu đồng điều), thì $v \circ f \circ u$ là một hợp thành của các tương đương đồng luân (tương ứng, các đẳng cấu đồng điều), do đó nó cũng là như vậy. Ngược lại, cho $\overline{u}$ và $\overline{v}$ là các cấu xạ nghịch đảo của $u$ và $v$ theo đồng luân; khi đó $\overline{v} \circ (v \circ f \circ u) \circ \overline{u}$ đồng luân với $f$ theo mệnh đề 4; do đó kết luận suy ra từ mệnh đề 5, và hệ quả của mệnh đề 3.

Người ta nói rằng phức $C$ đồng luân với không nếu $1_C$ đồng luân với ánh xạ không, nghĩa là nếu tồn tại một tự đồng cấu phân bậc $s$ bậc 1 của $C$ sao cho $1_C = s \circ d + d \circ s$. Điều này cũng tương đương với việc nói rằng cấu xạ duy nhất $0 \to C$ (tương ứng, $C \to 0$) là một tương đương đồng luân. Một phức đồng luân với không có đồng điều không (mệnh đề 5).

#### Ví dụ {#alg-x-s2-n4-exa-1 .statement}

Cho $u : M \to N$ và $v : N \to P$ là các đồng cấu của các $A$-môđun sao cho $v \circ u = 0$; gọi $C$ là phức sao cho $C_2 = M, C_1 = N, C_0 = P, C_i = 0$ với $i \neq 0, 1, 2$, $d_2 = u, d_1 = v, d_i = 0$ với $i \neq 1, 2$. Khi đó $C$ có đồng điều không nếu và chỉ nếu dãy $0 \to M \xrightarrow{u} N \xrightarrow{v} P \to 0$ là khớp. Nó đồng luân với không nếu và chỉ nếu dãy này tách. Thật vậy, việc nói rằng $C$ đồng luân với không có nghĩa là tồn tại các đồng cấu $A$-môđun $s : P \to N$ và $t : N \to M$ sao cho $v \circ s = 1_P, s \circ v + u \circ t = 1_N, t \circ u = 1_M$; điều này suy ra rằng dãy là tách; ngược lại, nếu $s$ là một tiết diện $A$-tuyến tính của $v$, ta định nghĩa $t$ bởi $u \circ t = 1_N - s \circ v$, điều này là có thể được vì $v \circ (1_N - s \circ v) = v - v \circ s \circ v = 0$.

### 5. Các phức tách

#### Mệnh đề 6 {#alg-x-s2-prop-6 .statement}

Cho $(C, d)$ là một phức. Các điều kiện sau là tương đương:
(i) tồn tại một tương đương đồng luân từ $(C, d)$ đến $(\mathrm{H}(C), 0)$;
(ii) tồn tại một tự đồng cấu $A$-môđun $s$ của $C$, phân bậc bậc 1, sao cho $d = d \circ s \circ d$;
(iii) $B(C)$ và $Z(C)$ là các hạng tử trực tiếp của $C$;
(iv) $(C, d)$ là một tổng trực tiếp của các phức con hoặc có độ dài 0, hoặc có độ dài 1 và có đồng điều không.

(i) $\Rightarrow$ (ii): gọi $\varphi : C \to \mathrm{H}(C)$ là một tương đương đồng luân; khi đó tồn tại một cấu xạ của các phức $\psi : \mathrm{H}(C) \to C$ và một tự đồng cấu $s$ của $C$, phân bậc bậc 1, sao cho $\psi \circ \varphi = 1_C - s \circ d - d \circ s$. Ta có $d \circ \psi = \psi \circ 0 = 0$, do đó
$$
0 = d \circ \psi \circ \varphi = d - d \circ s \circ d - d \circ d \circ s = d - d \circ s \circ d ,
$$
do đó (ii).

$(ii) \Rightarrow (iii)$: gọi $s$ như trong (ii). Khi đó $d \circ (1_C-s\circ d)=0$, nên $1_C-s\circ d$ là một phép chiếu của $C$ lên $Z(C)$, và $(d\circ s)\circ d=d$, nên $d\circ s$ là một phép chiếu của $C$ lên $B(C)$.

$(iii) \Rightarrow (iv)$: với mỗi $n\in\mathbf{Z}$, đặt $Z_n=Z_n(C)$, $B_n=B_n(C)$ và chọn các môđun con $K_n$ và $B'_n$ của $C_n$ sao cho $C_n=B'_n\oplus Z_n$, $Z_n=K_n\oplus B_n$. Khi đó

$$
E_{(n)}=K_n(-n)\quad\text{và}\quad F_{(n)}=B'_n(-n)\oplus B_{n-1}(1-n)
$$

là các phức con của $(C,d)$; ta có

$$
(C,d)=\bigoplus_{n\in\mathbf{Z}}(E_{(n)}\oplus F_{(n)})
$$

; mỗi $E_{(n)}$ hoặc bằng không hoặc có độ dài $0$, mỗi $F_{(n)}$ hoặc bằng không hoặc có độ dài $1$ và có đồng điều không, do đó có (iv).

$(iv) \Rightarrow (i)$: chỉ cần nhận thấy rằng (i) được thỏa mãn khi $C$ có độ dài không, hoặc có đồng điều không và độ dài $1$.

#### Định nghĩa 6 {#alg-x-s2-def-6 .statement}

*Một phức $C$ được gọi là tách nếu nó thỏa mãn các điều kiện tương đương của Mệnh đề 6.*

Một tự đồng cấu $s$ của $C$ thỏa mãn điều kiện (ii) của Mệnh đề 6 được gọi là một *tách* của $C$.

#### Ví dụ 1 {#alg-x-s2-n5-exa-1 .statement}

Một phức có vi phân không là tách.

#### Ví dụ 2 {#alg-x-s2-n5-exa-2 .statement}

Các phức đồng luân với không là các phức tách có đồng điều không, *nghĩa là* các phức $C$ sao cho $H(C)=0$ và $Z(C)$ là một nhân tử trực tiếp của $C$.

#### Ví dụ 3 {#alg-x-s2-n5-exa-3 .statement}

Cho $f:M\to N$ là một đồng cấu của các A-môđun và $C$ là phức sao cho $C_1=M$, $C_0=N$, $C_i=0$ với $i\ne0,1$, $d_1=f$, $d_i=0$ với $i\ne1$. Khi đó $C$ là tách khi và chỉ khi $\operatorname{Ker}f$ là một nhân tử trực tiếp của $M$ và $\operatorname{Im}f$ là một nhân tử trực tiếp của $N$.

#### Ví dụ 4 {#alg-x-s2-n5-exa-4 .statement}

*Phức $C$ là tách ngay khi $B(C)$ và $H(C)$ là xạ ảnh (tương ứng, ngay khi $B_n(C)$ và $H_n(C)$ là đơn ánh với mỗi $n$).* Thật vậy, theo các dãy khớp $(I_n)$ đến $(IV_n)$ của No. 1, khi đó $Z(C)$ là một nhân tử trực tiếp của $C$ và $B(C)$ là một nhân tử trực tiếp của $Z(C)$ (tương ứng $B(C)$ là một nhân tử trực tiếp của $C$ và $Z(C)/B(C)$ là một nhân tử trực tiếp của $C/B(C)$).

#### Ví dụ 5 {#alg-x-s2-n5-exa-5 .statement}

Đặc biệt, nếu A là chính, một phức tự do $C$ là tách khi và chỉ khi $H(C)$ là tự do (nghĩa là $H_n(C)$ tự do với mọi $n\in\mathbf{Z}$).

#### Nhận xét {#alg-x-s2-n5-rem-1 .statement}

a) Giả sử dãy khớp chính tắc của các A-môđun phân bậc

$$
\tag{II}
0\longrightarrow B(C)\longrightarrow Z(C)\xrightarrow{\pi}H(C)\longrightarrow0
$$

được tách (điều này xảy ra chẳng hạn nếu $H(C)$ xạ ảnh, hoặc $B_n(C)$ đơn ánh với mọi $n$); gọi $\sigma:H(C)\to Z(C)$ là một tiết diện phân bậc A-tuyến tính của $\pi$, và gọi $\psi$ là đồng cấu $x\mapsto\sigma(x)$ từ $H(C)$ vào $C$. Khi đó $\psi$ là một *homologism* từ $(H(C),0)$ vào $C$, sao cho

$$
H(\psi)=1_{H(C)}.
$$

b) Giả sử dãy khớp chính tắc của các A-môđun phân bậc

$$
\tag{IV}
0\longrightarrow H(C)\xrightarrow{i}C/B(C)\longrightarrow B(C)(-1)\longrightarrow0
$$

được tách (điều này xảy ra chẳng hạn nếu $B(C)$ xạ ảnh, hoặc $H_n(C)$ đơn ánh với mọi $n$); gọi $\tau : C/B(C) \to H(C)$ là một phép co rút phân bậc A-tuyến tính của $i$ và gọi $\varphi$ là đồng cấu từ $C$ vào $H(C)$ gán cho mỗi phần tử của $C$ ảnh qua $\tau$ của lớp của nó modulo $B(C)$. Khi đó $\varphi$ là một *homologism từ $C$ vào $(H(C), 0)$ sao cho* $H(\varphi) = 1_{H(C)}$.

### 6. Nón và trụ của một cấu xạ của các phức

Cho $u : (C', d') \to (C, d)$ là một cấu xạ của các phức. Gọi $\mathrm{Cyl}\,(u)$ và $\mathrm{Con}\,(u)$ là các A-môđun phân bậc $\mathrm{Cyl}\,(u) = C' \oplus C'(-1) \oplus C$, $\mathrm{Con}\,(u) = C'(-1) \oplus C$, và định nghĩa các ánh xạ phân bậc A-tuyến tính bậc $(-1)$

$$
\overline{D} : \mathrm{Cyl}\,(u) \to \mathrm{Cyl}\,(u) , \quad \overline{D}(x', y', x) = (d'x' + y', -d'y', dx - u(y')),
$$
$$
D : \mathrm{Con}\,(u) \to \mathrm{Con}\,(u) , \quad D(y', x) = (-d'y', dx - u(y')) .
$$

(Ở đây, và trong phần sau, $x, y, \ldots$ ký hiệu các phần tử tùy ý của $C$, $x', y', \ldots$ các phần tử tùy ý của $C'$.)

#### Bổ đề 2 {#alg-x-s2-lem-2 .statement}

(*Cyl* $(u)$, $\overline{D}$) *và* (*Con* $(u)$, $D$) *là các phức của A-môđun*.

Thật vậy, ta có
$$
\overline{D} \circ \overline{D}(x', y', x) = \overline{D}(d'x' + y', -d'y', dx - u(y')) =
$$
$$
= (d'(d'x' + y') - d'y', -d'(-d'y'), d(dx - u(y')) - u(-d'y')) = 0
$$
vì $d' \circ d' = 0$, $d \circ d = 0$ và $d \circ u = u \circ d'$. Tương tự $D \circ D = 0$.

#### Định nghĩa 7 {#alg-x-s2-def-7 .statement}

*Các phức* $\mathrm{Cyl}\,(u)$ *và* $\mathrm{Con}\,(u)$ *được gọi tương ứng là trụ* *và nón của cấu xạ* $u$.

#### Ví dụ {#alg-x-s2-n6-exa-1 .statement}

Cho $u : M \to N$ là một đồng cấu của các A-môđun; khi đó các thành phần thuần nhất khác không duy nhất của $\mathrm{Cyl}\,(u)$ và $\mathrm{Con}\,(u)$ là
$$
\mathrm{Cyl}_1\,(u) = M , \qquad \mathrm{Cyl}_0\,(u) = M \oplus N ,
$$
$$
\mathrm{Con}_1\,(u) = M , \qquad \mathrm{Con}_0\,(u) = N ,
$$
và ta có $\overline{D}(m) = (m, -u(m))$, $D(m) = -u(m)$ với $m \in M$; do đó,
$$
H_1(\mathrm{Con}\,(u)) = \mathrm{Ker}\,(u) , \quad H_0(\mathrm{Con}\,(u)) = \mathrm{Coker}\,(u) .
$$

*Cho* $X$ *và* $Y$ *là hai không gian tôpô và* $f$ *là một ánh xạ liên tục từ* $X$ *vào* $Y$. *Trụ* của $f$ được gọi là không gian thương $\mathrm{Cyl}\,(f)$ của tổng tôpô của $[0, 1] \times X$ và $Y$ theo quan hệ tương đương đồng nhất điểm $(1, x)$ của $[0, 1] \times X$ với điểm $f(x)$ của $Y$ với mọi $x \in X$. *Nón* của $f$ được gọi là không gian thương $\mathrm{Con}\,(f)$ của tổng tôpô của một không gian thu về một điểm $s$ và $\mathrm{Cyl}\,(f)$ theo quan hệ tương đương đồng nhất $s$ với ảnh của $(0, x)$ với mọi $x \in X$: ta vẫn ký hiệu bởi $s$ ảnh của $s$ trong $\mathrm{Con}\,(f)$.

Giả sử rằng $X$ và $Y$ được trang bị các phân tích tế bào $(X_n)$ và $(Y_n)$ (*xem.* No. 3), và giả sử rằng $f(X_n) \subset Y_n$ với mọi $n$. Ta thu được một phân tích tế bào $(S_n)$ của $\mathrm{Cyl}\,(f)$ (resp. của $\mathrm{Con}\,(f)$) bằng cách lấy $S_n$ là ảnh của $(\{0\} \times X_n) \cup ([0, 1] \times X_{n-1}) \cup Y_n$
$$
(\text{resp. của } \{s\} \cup ([0, 1] \times X_{n-1}) \cup Y_n , \quad \text{nếu } n \geqslant 0) .
$$
Ký hiệu bởi $\Gamma(X), \Gamma(Y), \Gamma(\mathrm{Cyl}\,(f)), \Gamma(\mathrm{Con}\,(f))$ các phức liên kết với các phân tích tế bào này.

Phức $\Gamma(s)$ liên kết với không gian $\{ s \}$ được trang bị phân tích tế bào duy nhất của nó được thu về môđun $\mathbf{A}$ và được đồng nhất với một phức con của $\Gamma(\mathrm{Con}\,(f))$; ký hiệu bởi $\Gamma(\mathrm{Con}\,(f),\,s)$ phức thương. Ánh xạ $f$ xác định một cấu xạ của các phức $\Gamma(f) : \Gamma(X) \to \Gamma(Y)$, và người ta có thể chứng minh rằng các phức $\Gamma(\mathrm{Cyl}\,(f))$ và $\Gamma(\mathrm{Con}\,(f),\,s)$ được đồng nhất tương ứng với $\mathrm{Cyl}\,(\Gamma(f))$ và $\mathrm{Con}\,(\Gamma(f))$.

Mặt khác, và không cần giả thiết gì trên $X$ và $Y$, ta gắn với $f$ một cấu xạ phức $f_* : C(X,\,\mathbf{A}) \to C(Y,\,\mathbf{A})$. Có thể xây dựng các homotopisme đơn cấu từ $\mathrm{Cyl}\,(f_*)$ vào $C(\mathrm{Cyl}\,(f),\,\mathbf{A})$ và từ $\mathrm{Con}\,(f_*)$ vào $C(\mathrm{Con}\,(f),\,\{s\},\,\mathbf{A})$.
Gọi $\tilde{f} : X \to \mathrm{Cyl}\,(f)$ là ánh xạ gán cho $x$ ảnh của $(0,\,x)$, $\alpha : Y \to \mathrm{Cyl}\,(f)$ là ánh xạ chính tắc và $\beta : \mathrm{Cyl}\,(f) \to Y$ là ánh xạ gán $y$ cho ảnh của nó trong $\mathrm{Cyl}\,(f)$ với $y \in Y$ và gán $f(x)$ cho ảnh của $(t,\,x)$ trong $\mathrm{Cyl}\,(f)$ với $t \in [0,\,1]$ và $x \in X$. Ánh xạ $\tilde{f}$ là một đồng phôi từ $X$ lên một tập đóng của $\mathrm{Cyl}\,(f)$, ta có $\beta \circ \alpha = \mathrm{Id}_Y$, và $\alpha \circ \beta$ đồng luân theo nghĩa tôpô với đồng nhất trên $\mathrm{Cyl}\,(f)$. Các tính chất này cần được đối chiếu với mệnh đề 7 dưới đây. \*

Bây giờ hãy xét các ánh xạ $\mathbf{A}$-tuyến tính phân bậc bậc 0

$$
\begin{align*}
\tilde{u} : C' &\to \mathrm{Cyl}\,(u)\,, & \tilde{u}(x') &= (x',\,0,\,0)\,, \\
\alpha : C &\to \mathrm{Cyl}\,(u)\,, & \alpha(x) &= (0,\,0,\,x)\,, \\
\beta : \mathrm{Cyl}\,(u) &\to C\,, & \beta(x',\,y',\,x) &= u(x') + x\,, \\
\pi : C &\to \mathrm{Con}\,(u)\,, & \pi(x) &= (0,\,x)\,, \\
\tilde{\pi} : \mathrm{Cyl}\,(u) &\to \mathrm{Con}\,(u)\,, & \tilde{\pi}(x',\,y',\,x) &= (y',\,x)\,, \\
\delta : \mathrm{Con}\,(u) &\to C'(-1)\,, & \delta(y',\,x) &= y'\,.
\end{align*}
$$

#### Mệnh đề 7 {#alg-x-s2-prop-7 .statement}

*a)* *Các ánh xạ* $\tilde{u},\, \alpha,\, \beta,\, \pi,\, \tilde{\pi},\, \delta$ *là các cấu xạ phức* : ta có $u = \beta \circ \tilde{u},\, \pi = \tilde{\pi} \circ \alpha,\, \beta \circ \alpha = 1_C$.

*b)* *Các dãy cấu xạ phức*

(6) $$ 0 \to C' \xrightarrow{\tilde{u}} \mathrm{Cyl}\,(u) \xrightarrow{\tilde{\pi}} \mathrm{Con}\,(u) \to 0 $$

(7) $$ 0 \to C \xrightarrow{\pi} \mathrm{Con}\,(u) \xrightarrow{\delta} C'(-1) \to 0 $$

*là khớp*.

*c)* *Các cấu xạ* $\alpha : C \to \mathrm{Cyl}\,(u)$ *và* $\beta : \mathrm{Cyl}\,(u) \to C$ *là các homotopisme nghịch đảo của nhau, sai khác một đồng luân*.

Mệnh đề *a)* tương đương với các công thức

$$
\begin{align*}
\tilde{u} \circ d' &= \overline{D} \circ \tilde{u}\,, & \alpha \circ d &= \overline{D} \circ \alpha\,, & \beta \circ \overline{D} &= d \circ \beta\,, & \pi \circ d &= D \circ \pi\,, \\
\tilde{\pi} \circ \overline{D} &= D \circ \tilde{\pi}\,, & \delta \circ D &= -d' \circ \delta\,, & u &= \beta \circ \tilde{u}\,, & \pi &= \tilde{\pi} \circ \alpha\,, & \beta \circ \alpha &= 1_C
\end{align*}
$$

mà ta kiểm tra được bằng những phép tính trực tiếp. Mệnh đề *b)* là tầm thường. Chứng minh *c)* ; một mặt ta có $\beta \circ \alpha = 1_C$; mặt khác nếu $\sigma : \mathrm{Cyl}\,(u) \to \mathrm{Cyl}\,(u)$ là ánh xạ $\mathbf{A}$-tuyến tính phân bậc bậc 1 sao cho $\sigma(x',\,y',\,x) = (0,\,x',\,0)$, thì ta kiểm tra ngay được rằng

$$
\overline{D} \circ \sigma + \sigma \circ \overline{D} + \alpha \circ \beta = 1_{\mathrm{Cyl}\,(u)}\,,
$$

suy ra *c)*.

Có thể tóm tắt mệnh đề 7 bằng sơ đồ giao hoán sau đây, trong đó các hàng là khớp, và các mũi tên thẳng đứng là các homotopisme:

$$
\begin{array}{ccccccccc}
0 & \longrightarrow & C & \xrightarrow{\pi} & \mathrm{Con}\,(u) & \xrightarrow{\delta} & C'(-1) & \longrightarrow & 0 \\
& & \downarrow^{\alpha} & & \downarrow^1 & & & & \\
0 & \longrightarrow & C' & \xrightarrow{\tilde{u}} & \mathrm{Cyl}\,(u) & \xrightarrow{\tilde{\pi}} & \mathrm{Con}\,(u) & \longrightarrow & 0 \\
& & \downarrow^1 & & \downarrow^{\beta} & & & & \\
& & C' & \xrightarrow{u} & C & & & &
\end{array}
$$

#### Hệ quả {#alg-x-s2-n6-cor-1 .statement}

*Với mọi cấu xạ phức* $u : C' \to C$, *tồn tại một cấu xạ đơn cấu của các phức* $\tilde{u} : C' \to C_1$ *và một homotopisme* $\beta : C_1 \to C$ *sao cho* $u = \beta \circ \tilde{u}$.

#### Bổ đề 3 {#alg-x-s2-lem-3 .statement}

*a)* *Đồng cấu liên kết*
$$
\partial_{n+1}(\pi, \delta) : H_n(C') \to H_n(C)
$$
*ứng với dãy khớp (7) bằng* $-H_n(u)$.

*b)* *Đồng cấu liên kết*
$$
\partial_n(\tilde{u}, \tilde{\pi}) : H_n(\mathrm{Con}\,(u)) \to H_{n-1}(C')
$$
*ứng với dãy khớp (6) bằng* $H_n(\delta)$.

Cho $x' \in Z_n(C')$; vì $x' = \delta(x', 0)$ và
$$
- D(x', 0) = (d'x', u(x')) = (0, u(x')) = \pi(u(x')) ,
$$
nên theo định nghĩa, $\partial(\pi, \delta)$ biến lớp của $x'$ trong $H_n(C')$ thành lớp của $-u(x')$ trong $H_n(C)$, suy ra *a)*.

Giả sử $(y', x) \in \mathrm{Con}_n(u)$ sao cho $D(y', x) = 0$; khi đó ta có $(-d'y', dx - u(y')) = 0$. Vì $(y', x) = \tilde{\pi}(0, y', x)$ và
$$
\overline{D}(0, y', x) = (y', -d'y', dx - u(y')) = (y', 0, 0) = \tilde{u}(\delta(y', x)) ,
$$
nên theo định nghĩa, $\partial(\tilde{u}, \tilde{\pi})$ ánh xạ lớp của $(y', x)$ trong $H_n(\mathrm{Con}\,(u))$ lên lớp của $\delta(y', x)$ trong $H_{n-1}(C')$, do đó được *b)*.

#### Mệnh đề 8 {#alg-x-s2-prop-8 .statement}

*Ta có dãy khớp vô hạn*
(8) $$ \cdots \longrightarrow H_n(C') \xrightarrow{H_n(u)} H_n(C) \xrightarrow{H_n(\pi)} H_n(\mathrm{Con}\,(u)) \xrightarrow{H_n(\delta)} H_{n-1}(C') \longrightarrow \cdots . $$

Thật vậy, có xét đến *bổ đề 3, a)*, điều này suy ra từ định lý 1 của X, p. 30, áp dụng cho dãy khớp (7).

#### Hệ quả {#alg-x-s2-n6-cor-2 .statement}

*Để u là một homologisme, điều kiện cần và đủ là Con (u) có đồng điều bằng không.*

#### Nhận xét {#alg-x-s2-n6-rem-1 .statement}

Xét biểu đồ

$$
\begin{array}{ccccccccc}
\cdots & \longrightarrow & H_n(C') & \xrightarrow{H_n(\tilde{u})} & H_n(\mathrm{Cyl}\,(u)) & \xrightarrow{H_n(\pi)} & H_n(\mathrm{Con}\,(u)) & \xrightarrow{\partial_n(\tilde{u},\pi)} & H_{n-1}(C') \longrightarrow \cdots \\
& & \downarrow 1 & & \downarrow H_n(\beta) & & \downarrow 1 & & \downarrow 1 \\
\cdots & \longrightarrow & H_n(C') & \xrightarrow{H_n(u)} & H_n(C) & \xrightarrow{H_n(\pi)} & H_n(\mathrm{Con}\,(u)) & \xrightarrow{H_n(\delta)} & H_{n-1}(C') \longrightarrow \cdots
\end{array}
$$

trong đó dòng thứ nhất (resp. dòng thứ hai) là dãy khớp đồng điều gắn với dãy khớp (6) (resp. (7)). Các ánh xạ $H_n(\beta)$ là song ánh (mệnh đề 7, c)) và biểu đồ là giao hoán, vì
a) $u = \beta \circ \tilde{u}$ (mệnh đề 7, a)) nên $H_n(u) = H_n(\beta) \circ H_n(\tilde{u})$,
b) $H_n(\beta) = H_n(\alpha)^{-1}$ và $\pi = \tilde{\pi} \circ \alpha$ (mệnh đề 7, a) và c)), nên $H_n(\tilde{\pi}) = H_n(\pi) \circ H_n(\beta)$,
c) $H_n(\delta) = \partial_n(\tilde{u},\tilde{\pi})$ (*bổ đề 3, b*)).

### 7. Nón của một cấu xạ đơn ánh; định nghĩa mới của đồng cấu nối

Bây giờ xét một dãy khớp các phức

(9)
$$
0 \to C' \xrightarrow{u} C \xrightarrow{v} C'' \to 0 .
$$

Định nghĩa một ánh xạ A-tuyến tính phân bậc bậc 0
$$
\varphi : \mathrm{Con}\,(u) \to C''
$$
bởi $\varphi(y', x) = v(x)$. Khi đó ta có một biểu đồ giao hoán các A-môđun với các hàng khớp

(10)
$$
\begin{array}{ccccccccc}
0 & \longrightarrow & C' & \xrightarrow{\tilde{u}} & \mathrm{Cyl}\,(u) & \xrightarrow{\tilde{\pi}} & \mathrm{Con}\,(u) & \longrightarrow & 0 \\
& & \downarrow 1 & & \downarrow \beta & & \downarrow \varphi & & \\
0 & \longrightarrow & C' & \xrightarrow{u} & C & \xrightarrow{v} & C'' & \longrightarrow & 0 .
\end{array}
$$

#### Mệnh đề 9 {#alg-x-s2-prop-9 .statement}

*Các ánh xạ* $\beta$ *và* $\varphi$ *là các homologisme của các phức*.
Đối với $\beta$, điều này suy ra từ mệnh đề 7, c). Ta có
$$
\begin{align*}
\varphi \circ D(y', x) &= \varphi(-d'y', dx - u(y')) = v(dx - u(y')) \\
&= v(dx) = d'' v(x) = d''(\varphi(y', x)) ,
\end{align*}
$$
nên $\varphi$ quả thật là một cấu xạ của các phức. Mặt khác, $\varphi$ là toàn ánh và hạt nhân của nó được đồng nhất với phức $(\mathbf{K}, d_\mathbf{K})$ sao cho $\mathbf{K} = C'(-1) \oplus C'$,
$$
d_\mathbf{K}(y', x') = (-d'y', d'x' - y') ;
$$
nếu $d_\mathbf{K}(y', x') = 0$, thì ta có $y' = d' x'$, nên $(y', x') = d_\mathbf{K}(0, -x')$; suy ra $\mathrm{H}(\mathbf{K}) = 0$ và $\varphi$ là một homologisme theo X, p. 30, hệ quả 1.

#### Nhận xét {#alg-x-s2-n7-rem-1 .statement}

Homologisme $\beta$ là một homotopisme, nhưng nói chung $\varphi$ không phải là một homotopisme (*cf.* X, p. 173, bài tập 8).

#### Hệ quả {#alg-x-s2-n7-cor-1 .statement}

*Biểu đồ các A-môđun phân bậc*

$$
\begin{array}{ccccc}
&& H(\operatorname{Con}(u)) &&\\
&\nearrow^{H(\pi)}&&\searrow^{H(\delta)}&\\
H(C)& &\downarrow^{H(\varphi)}&&H(C')(-.1)\\
&\searrow_{H(\iota)}&&\nearrow_{\partial(u,v)}&\\
&&H(C'')&&
\end{array}
$$

là giao hoán và $H(\varphi)$ là song ánh.

Trong biểu đồ giao hoán (10), ta có $H(1_{C'})\circ\widetilde{\partial}(\tilde u,\tilde\pi)=\partial(u,v)\circ H(\varphi)$ (X, p. 31, mệnh đề 2) và $\widetilde{\partial}(\tilde u,\tilde\pi)=H(\delta)$ (X, p. 38, *bổ đề 3, b*)), do đó

$$
\partial(u,v)\circ H(\varphi)=H(\delta)\ ;
$$

mặt khác, $H(v)\circ H(\beta)=H(\varphi)\circ H(\tilde\pi)=H(\varphi)\circ H(\pi)\circ H(\beta)$ theo X, p. 39, nhận xét. Vì $H(\beta)$ là song ánh, suy ra $H(v)=H(\varphi)\circ H(\pi)$.

Vậy ta có $\partial(u,v)=H(\delta)\circ H(\varphi)^{-1}$, điều này cung cấp một *định nghĩa mới* của đồng cấu nối $\partial(u,v)$. Mặt khác, cũng lưu ý rằng nếu đồng nhất $H(\operatorname{Con}(u))$ với $H(C'')$ qua $H(\varphi)$, thì hệ quả trước đó có nghĩa là *dãy khớp* (8) *khi đó được đồng nhất với dãy khớp đồng điều tương đối với* (9).

### 8. Đặc trưng Euler-Poincaré

Trong no này, xét một tập hợp $\mathcal C$ các lớp A-môđun *cộng tính và khớp trái*, nghĩa là thỏa mãn hai điều kiện sau:

(A) *Nếu* $M$ *và* $N$ *là hai A-môđun kiểu* $\mathcal C$, $M\oplus N$ *thuộc kiểu* $\mathcal C$.

(G) Nếu $0\to M'\to M\to M''\to0$ là một dãy khớp các A-môđun và nếu $M$ và $M''$ thuộc kiểu $\mathcal C$, thì $M'$ thuộc kiểu $\mathcal C$.

Ta nói rằng $\mathcal C$ là ổn định nếu nó thỏa mãn các điều kiện sau, các điều kiện này kéo theo (A) và (G):

(E) ("$\mathcal C$ ổn định dưới các mở rộng.") Nếu $0\to M'\to M\to M''\to0$ là một dãy khớp các A-môđun và nếu $M'$ và $M''$ thuộc kiểu $\mathcal C$, thì $M$ thuộc kiểu $\mathcal C$.

(S) ("$\mathcal C$ ổn định dưới các hạt nhân và đối hạt nhân.") Với mọi đồng cấu $f$ của các A-môđun thuộc kiểu $\mathcal C$, các A-môđun $\operatorname{Ker}f$ và $\operatorname{Coker}f$ thuộc kiểu $\mathcal C$.

Ta ký hiệu bởi $K(\mathcal C)$ nhóm Grothendieck của $\mathcal C$ và bởi $[M]_{\mathcal C}$ hoặc $[M]$ phần tử của $K(\mathcal C)$ được xác định bởi A-môđun $M$ (VIII, §6, No. 2). Cho $G$ là một nhóm giao hoán và $\varphi$ là một đồng cấu từ $K(\mathcal C)$ vào $G$.

#### Ví dụ 1 {#alg-x-s2-n8-exa-1 .statement}

Nếu A là một trường, ta có thể lấy $\mathcal C$ là tập hợp các lớp của các không gian vectơ hữu hạn chiều và $\varphi$ là đẳng cấu từ $K(\mathcal C)$ lên $\mathbf Z$ được xác định bởi $\varphi([M]) = \dim(M)$.

#### Ví dụ 2 {#alg-x-s2-n8-exa-2 .statement}

Ta có thể lấy $\mathcal C$ là tập hợp các lớp của các môđun có độ dài hữu hạn và $\varphi: K(\mathcal C) \to \mathbf Z$ là đồng cấu được xác định bởi $\varphi([M]) = \operatorname{long}_A(M)$.

Ta nói rằng một A-môđun phân bậc M thuộc kiểu $\mathcal C$ nếu $M_n$ thuộc kiểu $\mathcal C$ với mọi n (điều này là cần thiết khi M bị chặn và là đủ khi $\mathcal C$ ổn định để môđun M thuộc kiểu $\mathcal C$).

#### Định nghĩa 8 {#alg-x-s2-def-8 .statement}

Cho M là một A-môđun phân bậc bị chặn thuộc kiểu $\mathcal C$ và $(M_n)$ là phân bậc của nó. Ta gọi **đặc số**-$\varphi$ của M, và ký hiệu nó bởi $\chi_\varphi(M)$ hoặc đơn giản là $\chi(M)$, là phần tử $\sum (-1)^n \varphi([M_n])$ của G.

Định nghĩa này áp dụng đặc biệt khi M là môđun phân bậc nền của một phức các A-môđun.

#### Ví dụ 3 {#alg-x-s2-n8-exa-3 .statement}

Nếu M bị chặn và thuộc kiểu $\mathcal{C}$, thì tương tự cũng đúng đối với $M(p)$ với mọi $p \in \mathbf{Z}$, và ta có $\chi(M(p)) = (-1)^p \chi(M)$.

4) Cho $0 \to M' \to M \to M'' \to 0$ là một dãy khớp các A-môđun phân bậc và các đồng cấu phân bậc bậc 0. Nếu M, M' và M'' bị chặn và thuộc kiểu $\mathcal{C}$, ta có
$$
\chi(M) = \chi(M') + \chi(M'').
$$
Nếu M và M'' bị chặn và thuộc kiểu $\mathcal{C}$, thì tương tự cũng đúng đối với M'; nếu $\mathcal{C}$ ổn định và nếu hai trong ba môđun bị chặn và thuộc kiểu $\mathcal{C}$, thì tương tự cũng đúng đối với môđun thứ ba.

5) Cho $u : C' \to C$ là một cấu xạ của các phức bị chặn kiểu $\mathcal{C}$. Khi đó Con ($u$) bị chặn kiểu $\mathcal{C}$, và ta có:
$$
\chi(\operatorname{Con}(u)) = \chi(C) - \chi(C').
$$

6) Có thể lấy cho G chính nhóm $K(\mathcal{C})$, và cho $\varphi$ cấu xạ đồng nhất; trong trường hợp này người ta ký hiệu bởi $\chi_{\mathcal{C}}(M)$ phần tử $\chi_\varphi(M) = \sum (-1)^n[M_n]$ của $K(\mathcal{C})$.

#### Nhận xét {#alg-x-s2-n8-rem-1 .statement}

Người ta gọi đa thức Poincaré của M đối với $\varphi$ là phần tử $P_M(t) = \sum \varphi([M_n]) t^n \in G \otimes \mathbf{Z}[t, t^{-1}]$. Ta có $P_M(1) = \varphi([M])$ và $P_M(-1) = \chi(M)$.

#### Bổ đề 4 {#alg-x-s2-lem-4 .statement}

Cho C là một phức bị chặn kiểu $\mathcal{C}$. Nếu $H(C) = 0$, thì ta có $\chi(C) = 0$.
Điều này suy ra từ VIII, § 6, No. 1, hệ quả của Mệnh đề 1.

#### Mệnh đề 10 {#alg-x-s2-prop-10 .statement}

Cho C và C' là hai phức bị chặn kiểu $\mathcal{C}$. Nếu tồn tại một cấu xạ đồng điều $u : C' \to C$, thì ta có $\chi(C) = \chi(C')$.
Thật vậy, Con ($u$) bị chặn kiểu $\mathcal{C}$ và ta có $\chi(\operatorname{Con}(u)) = \chi(C) - \chi(C')$; mặt khác, $H(\operatorname{Con}(u)) = 0$ theo X, p. 38, hệ quả, do đó $\chi(\operatorname{Con}(u)) = 0$ (bổ đề 4).

#### Mệnh đề 11 {#alg-x-s2-prop-11 .statement}

Cho C là một phức bị chặn kiểu $\mathcal{C}$.
a) Nếu $\mathcal{C}$ ổn định, thì $H(C)$ là kiểu $\mathcal{C}$.
b) Nếu $H(C)$ là kiểu $\mathcal{C}$, thì tương tự cũng vậy đối với $B(C)$ và $Z(C)$, và ta có $\chi(H(C)) = \chi(C)$.

a) Nếu $\mathcal{C}$ ổn định, thì với mọi $n$ môđun $Z_n(C)$ là kiểu $\mathcal{C}$ như hạt nhân của $d_n : C_n \to C_{n-1}$, và $H_n(C)$ là kiểu $\mathcal{C}$ như đối hạt nhân của $C_{n+1} \to Z_n$. Mặt khác, $H_n(C) = 0$ ngay khi $C_n = 0$.

b) Giả sử $H(C)$ là kiểu $\mathcal{C}$. Các dãy khớp chính tắc:

$$
0 \to Z_n(C) \to C_n \to B_{n-1}(C) \to 0
$$
$$
0 \to B_n(C) \to Z_n(C) \to H_n(C) \to 0
$$

cho thấy bằng quy nạp theo $n$, bắt đầu từ cận phải của $C$, rằng $Z_n(C)$ và $B_n(C)$ đều là kiểu $\mathcal{C}$ với mọi $n$. Khi đó ta có

$$
\chi(C) = \chi(Z(C)) + \chi(B(C) (-1)) = \chi(Z(C)) - \chi(B(C)) = \chi(H(C)) .
$$

#### Hệ quả {#alg-x-s2-n8-cor-1 .statement}

*Nếu $\mathcal{C}$ ổn định và $C$ bị chặn kiểu $\mathcal{C}$, thì môđun phân bậc $H(C)$ bị chặn kiểu $\mathcal{C}$ và ta có $\chi(H(C)) = \chi(C)$.*

#### Mệnh đề 12 {#alg-x-s2-prop-12 .statement}

*Cho $0 \to C' \to C \to C'' \to 0$ là một dãy khớp các phức.*

*a) Nếu $H(C), H(C')$ và $H(C'')$ bị chặn kiểu $\mathcal{C}$, thì ta có*
$$
\chi(H(C)) = \chi(H(C')) + \chi(H(C'')) .
$$

*b) Nếu $\mathcal{C}$ ổn định, và nếu hai trong ba môđun phân bậc $H(C), H(C')$ và $H(C'')$ bị chặn kiểu $\mathcal{C}$, thì điều tương tự cũng đúng với môđun thứ ba.*

Phần a) suy ra từ Bổ đề 4 áp dụng cho phức có đồng điều không được xác định bởi dãy khớp đồng điều liên kết với dãy khớp đã cho. Phần b) suy ra, khi xét dãy khớp đồng điều này, từ bổ đề sau:

*Bổ đề 5. — Cho $M \to N \to P \to Q \to R$ là một dãy khớp các $A$-môđun. Nếu $\mathcal{C}$ ổn định, và nếu $M, N, Q$ và $R$ thuộc kiểu $\mathcal{C}$, thì môđun $P$ thuộc kiểu $\mathcal{C}$.
Đặt $N' = \operatorname{Coker}(M \to N)$ và $Q' = \operatorname{Ker}(Q \to R)$. Các môđun $N'$ và $Q'$ thuộc kiểu $\mathcal{C}$, và ta có một dãy khớp $0 \to N' \to P \to Q' \to 0$.*

#### Hệ quả {#alg-x-s2-n8-cor-2 .statement}

*Giả sử $\mathcal{C}$ ổn định, và cho $u : C' \to C$ là một cấu xạ các phức sao cho $H(C)$ và $H(C')$ bị chặn kiểu $\mathcal{C}$. Khi đó $H(\operatorname{Con}(u))$ bị chặn kiểu $\mathcal{C}$, và ta có*
$$
\chi(H(\operatorname{Con}(u))) = \chi(H(C)) - \chi(H(C')) .
$$

Điều này suy ra từ Mệnh đề 12 áp dụng cho dãy khớp các phức (X, p. 37, Mệnh đề 7)
$$
0 \to C \to \operatorname{Con}(u) \to C'(-1) \to 0 .
$$

*Nhận xét. — Cho $E$ là một phức, $h : E \to C$ và $h' : E \to C'$ là các tương đương đồng luân với $C$ và $C'$ bị chặn kiểu $\mathcal{C}$. Khi đó $\chi(C) = \chi(C')$. Thật vậy, nếu $h_1$ là một nghịch đảo của $h$ với sai khác đồng luân, thì $h' \circ h_1$ là một tương đương đồng luân, do đó là một đẳng cấu đồng điều từ $C$ tới $C'$, và ta có thể áp dụng Mệnh đề 10. Do đó, ta có thể mở rộng Định nghĩa 8 bằng cách đặt $\chi(E) = \chi(C)$ mỗi khi tồn tại một tương đương đồng luân từ $E$ tới một phức $C$ bị chặn kiểu $\mathcal{C}$. Các Mệnh đề 10, 11, 12 và các hệ quả của chúng được tổng quát hóa trong cách đặt này.*

Áp dụng:

\* Cho X là một không gian tôpô thừa nhận một phân tích tế bào hữu hạn (xem No. 3).
    a) Cho K và K' là hai trường, đặt $b_i = \dim_K(H_i(X, K))$ và $b'_i = \dim_{K'}(H_i(X, K'))$. Không nhất thiết có $b_i = b'_i$, nhưng ta có $\Sigma (-1)^i b_i = \Sigma (-1)^i b'_i$.
    b) Cho $(X_n)$ và $(X'_n)$ là hai phân tích tế bào hữu hạn của X, và ký hiệu bởi $c_n$ và $c'_n$ số các ô có chiều n trong hai phân tích này. Ta có
    $$
    \Sigma (-1)^i c_i = \Sigma (-1)^i c'_i .
    $$
    c) Với các ký hiệu của a) và b), ta có $\Sigma (-1)^i c_i = \Sigma (--1)^i b_i$.
    Các tính chất a) và b) suy ra từ c), và c) suy ra từ mệnh đề 11 áp dụng cho phức $\Gamma$ được mô tả ở No. 3, lấy cho $\mathcal{C}$ lớp các K-không gian vectơ hữu hạn chiều và cho $\varphi$ hàm được xác định bởi $\varphi([M]) = \dim_K(M)$ (X, p. 40, ví dụ 1).

### 9. Phức các môđun phải, phức các đa môđun

Một phức các A-môđun phải là một A-môđun phải phân bậc $(M_n)_{n \in \mathbf{Z}}$ được trang bị một tự đồng cấu phân bậc $d$ bậc -1 và bình phương bằng không; do đó nó là một phức các môđun trên vành đối của A. Vì vậy mọi định nghĩa và tính chất đã được phát biểu trong các số trước đều áp dụng cho các phức môđun phải khi xem chúng như các phức môđun trên vành $A^\circ$.

Tương tự, nếu A và B là hai vành, một phức các song môđun (A, B) là một song môđun (A, B) phân bậc M được trang bị một tự đồng cấu phân bậc $d$ bậc (-1) và bình phương bằng không; nếu M được trang bị cấu trúc chính tắc của môđun trái $A \otimes_\mathbf{Z} B^\circ$, thì $d$ trang bị cho nó một cấu trúc phức $A \otimes_\mathbf{Z} B^-$-. Vì vậy mọi định nghĩa và tính chất đã được phát biểu trong các số trước đều áp dụng cho các phức song môđun. Người ta định nghĩa tương tự các phức đa môđun.

### 10. Ví dụ: phức de Rham

Trong số này, giả thiết rằng A là một đại số giao hoán trên k trên một vành giao hoán k. Ta ký hiệu bởi $\Omega^1_{A/k}$ A-môđun các vi phân k của A (III, p. 134), bởi $d^0 : A \to \Omega^1_{A/k}$ đạo hàm k $d_{A/k}$, và bởi $\Omega_{A/k}$ đại số k phân bậc $\Lambda_A(\Omega^1_{A/k})$.

#### Mệnh đề 13 {#alg-x-s2-prop-13 .statement}

Tồn tại duy nhất một phản đạo hàm k $d : \Omega_{A/k} \to \Omega_{A/k}$ bậc 1, bình phương bằng không, mở rộng đạo hàm $d^0 : A \to \Omega^1_{A/k}$.

Hãy chứng minh tính duy nhất của phản đạo hàm d. Vì $d \circ d = 0$, ta có với $y, x_1, \ldots, x_p \in A$:
$$
d(y dx_1 \wedge \ldots \wedge dx_p) = dy \wedge dx_1 \wedge \ldots \wedge dx_p .
$$
A-môđun $\Omega^p_{A/k}$ được sinh bởi các phần tử $dx_1 \wedge \ldots \wedge dx_p$, điều này chứng minh tính duy nhất của d.

Để chứng minh sự tồn tại, chỉ cần xây dựng một $k$-đồng cấu $d^1 : \Omega_{A/k}^1 \to \Omega_{A/k}^2$ sao cho $d^1 \circ d^0 = 0$ và
$$
d^1(a \omega) = d^0(a) \wedge \omega + a d^1(\omega) \quad \text{với } a \in A , \quad \omega \in \Omega_{A/k}^1 .
$$
Thật vậy, khi đó suy ra từ III, p. 128, mệnh đề 14 (có tính đến III, p. 118, nhận xét 2) rằng tồn tại một phản đạo hàm $d : \Omega_{A/k} \to \Omega_{A/k}$ trùng với $d^0$ ở bậc 0 và với $d^1$ ở bậc 1. Vì $d^0$ bằng không trên $A$, phản đạo hàm $d$ là $k$-tuyến tính; vì $d^1 \circ d^0 = 0$, ta có $d \circ d = 0$ vì $\Omega_{A/k}$ được sinh như một A-đại số bởi các phần tử $d^0 a$ với $a \in A$.

Để định nghĩa $d^1$, hãy nhắc lại (III, p. 133) rằng $\Omega_{A/k}^1$ bằng A-môđun $\mathfrak{J}/\mathfrak{J}^2$, trong đó $\mathfrak{J}$ là hạt nhân của phép nhân $m : A \otimes_k A \to A$. Xét ánh xạ $k$-tuyến tính $u : A \otimes_k A \to \Omega_{A/k}^2$ được định nghĩa bởi $u(x \otimes y) = d^0(y) \wedge d^0(x)$. Ta có
$$
u(ax \otimes y - x \otimes ay) = d^0(y) \wedge d^0(ax) - d^0(ay) \wedge d^0(x) = d^0(xy) \wedge d^0(a)
$$
với $x, y$ và $a$ thuộc $A$, do đó
$$
u((a \otimes 1 - 1 \otimes a) \xi) = d^0(m(\xi)) \wedge d^0(a) , \quad \xi \in A \otimes_k A , \quad a \in A .
$$
Vì $\mathfrak{J}$ được sinh như một A-môđun trái bởi các phần tử $(a \otimes 1 - 1 \otimes a)$ với $a \in A$, ta suy ra rằng $u(\mathfrak{J}^2) = 0$; do đó $u$ xác định, bằng cách hạn chế lên $\mathfrak{J}$ rồi chuyển qua thương, một ánh xạ $k$-tuyến tính $d^1 : \mathfrak{J}/\mathfrak{J}^2 \to \Omega_{A/k}^2$.

Bằng cách đặt $\xi = b \otimes 1$ trong (12), với $b \in A$, ta thu được $d^1(b d^0(a)) = d^0(b) \wedge d^0(a)$; suy ra $d^1 \circ d^0 = 0$ và $d^1(c \omega) = d^0(c) \wedge \omega + c d^1(\omega)$ với $c \in A$ và $\omega = b d^0(a)$. Vì $\Omega_{A/k}^1$ được sinh như một $k$-môđun bởi các phần tử $b d^0(a)$, với $a$ và $b$ thuộc $A$, công thức (11) được thỏa mãn với mọi $\omega \in \Omega_{A/k}$, điều này hoàn tất chứng minh của mệnh đề.

Đôi khi người ta nói rằng các phần tử $\omega \in \Omega_{A/k}^p$ là các *dạng vi phân ngoài bậc* $p$ của $A$ trên $k$, và phản đạo hàm $d$ là *vi phân ngoài* của $\Omega_{A/k}$; phức $(\Omega_{A/k}, d)$ được gọi là *phức de Rham của A trên k*, và đồng điều của nó là *đối đồng điều de Rham của A trên k*.

#### Ví dụ 1 {#alg-x-s2-n10-exa-1 .statement}

Lấy $A$ là vành $k[X_1, ..., X_n]$. Khi đó $\Omega_{A/k}^1$ là một $A$-môđun tự do với cơ sở $dX_1, ..., dX_n$ (III, p. 134, ví dụ). Do đó, nếu, với mọi tập con $I = \{ i_1, ..., i_p \}$ của $\{ 1, n \}$, ta đặt $dX_I = dX_{i_1} \wedge ... \wedge dX_{i_p}$ (với $i_1 < ... < i_p$), thì $A$-môđun $\Omega_{A/k}^p$ nhận các phần tử $dX_I$ làm cơ sở, trong đó $I$ chạy qua tập hợp các tập con của $\{ 1, n \}$ có lực lượng $p$. Ta có
$$
d(P dX_I) = dP \wedge dX_I = \sum_{i \notin I} (-1)^{n(I,i)} \frac{\partial P}{\partial X_i} dX_{I \cup \{ i \}} ,
$$
trong đó $n(I, i)$ chỉ số phần tử của $I$ nhỏ hơn hẳn $i$.

Do đó, các chu trình của $Z^p(\Omega_{A/k})$ là các phần tử $\omega = \sum_{\operatorname{Card}(I) = p} P_I dX_I$ sao cho, với mọi tập con $J$ có $(p + 1)$ phần tử của $\{ 1, n \}$, ta có:
$$
\sum_{i \in J} (-1)^{n(J,i)} \frac{\partial P_{J-\{i\}}}{\partial X_i} = 0 .
$$

Phần tử $\omega$ là một biên nếu có thể chọn, với mọi tập con $J \subset \{1, n\}$ có $(p - 1)$ phần tử, một đa thức $Q_J \in A$ sao cho:

$$
P_I = \sum_{j \in I} (-1)^{n(I,j)} \frac{\partial Q_{I-\{j\}}}{\partial X_j}.
$$

Ta sẽ thấy ở § 9 rằng phức de Rham của $A$ trên $k$ là acyclic trong các bậc $> 0$ nếu $k$ là một $\mathbf{Q}$-đại số (X, p. 159, *nhận xét 4*).

#### Ví dụ 2 {#alg-x-s2-n10-exa-2 .statement}

Giả sử $k = \mathbf{C}$$ và $A = \mathbf{C} [X_1, ..., X_n]/(P_1, ..., P_r)$, trong đó các $P_i$ là các đa thức theo $X_1, ..., X_n$, sao cho tập hợp các điểm của $\mathbf{C}^n$ tại đó mọi $P_i$ đều triệt tiêu là một tập con đại số giải tích $V$ của $\mathbf{C}^n$. Có thể chỉ ra rằng đối đồng điều de Rham của $A$ trên $\mathbf{C}$ đẳng cấu với *đối đồng điều kỳ dị* $H(V, \mathbf{C})$.

Bây giờ cho $M$ là một $A$-môđun và $\nabla^0$ là một ánh xạ tuyến tính $k$ từ $M$ vào $M \otimes_A \Omega^1_{A/k}$ sao cho

$$(13)$$
$$
\nabla^0(am) = a \nabla^0(m) + m \otimes da \quad \text{với} \quad a \in A,\ m \in M
$$
(đôi khi người ta nói rằng $\nabla^0$ là một *connection* trên $A$-môđun $M$).

#### Mệnh đề 14 {#alg-x-s2-prop-14 .statement}

(i) *Tồn tại một ánh xạ $k$-tuyến tính duy nhất $\nabla$ từ $\Omega_{A/k}$-môđun phải $M \otimes_A \Omega_{A/k}$ vào chính nó, phân bậc bậc 1, mở rộng $\nabla^0$ ở bậc 0 và thỏa mãn đẳng thức* :

$$(14)$$
$$
\nabla(x \omega) = (\nabla x) \omega + (-1)^p x(d\omega) \quad \text{với} \quad x \in M \otimes_A \Omega^p_{A/k},\ \omega \in \Omega_{A/k}.
$$

(ii) *Ánh xạ hợp thành $\nabla \circ \nabla$ là $\Omega_{A/k}$-tuyến tính ; đặc biệt ánh xạ $R = \nabla^1 \circ \nabla^0$ từ $M$ vào $M \otimes_A \Omega^2_{A/k}$ là $A$-tuyến tính, và ta có*
$$
\nabla \circ \nabla(m \otimes \omega) = R(m).\omega \quad \text{với} \quad m \in M,\ \omega \in \Omega_{A/k}.
$$

Đồng cấu $R$ đôi khi được gọi là *đồng cấu độ cong* của liên kết $\nabla^0$; nếu nó bằng không, cặp $(M \otimes_A \Omega_{A/k}, \nabla)$ là một phức, cũng được gọi là *phức de Rham của* $(M, \nabla^0)$ *trên* $k$.

Hãy chứng minh (i). Tính duy nhất của $\nabla$ là hiển nhiên. Hãy định nghĩa một $k$-đồng cấu $\overline{\nabla}$ từ $M \otimes_k \Omega_{A/k}$ vào $M \otimes_A \Omega_{A/k}$ bởi
$$
\overline{\nabla}(m \otimes_k \omega) = (\nabla^0 m) \omega + m \otimes d\omega \quad \text{với} \quad m \in M,\ \omega \in \Omega_{A/k}.
$$

Từ (13) suy ra rằng $\overline{\nabla}(am \otimes \omega) = \overline{\nabla}(m \otimes a \omega)$, nên khi chuyển qua thương ta thu được một $k$-đồng cấu $\nabla$ từ $M \otimes_A \Omega_{A/k}$ vào chính nó, phân bậc bậc 1, mở rộng $\nabla^0$ ở bậc 0. Hãy kiểm tra (14): ta có với $m \in M$, $\alpha \in \Omega^p_{A/k}$, $\omega \in \Omega_{A/k}$ :
$$
\begin{align*}
\nabla((m \otimes \alpha).\omega) &= \nabla(m \otimes (\alpha \wedge \omega)) = \nabla^0(m).(\alpha \wedge \omega) + m \otimes d(\alpha \wedge \omega) \\
&= \nabla^0(m) \alpha.\omega + (m \otimes d\alpha) \omega + (-1)^p (m \otimes \alpha) d\omega \\
&= (\nabla(m \otimes \alpha)) \omega + (-1)^p (m \otimes \alpha) d\omega
\end{align*}
$$
điều này chứng minh (14) cho $x = m \otimes \alpha$; trường hợp tổng quát suy ra bởi tính tuyến tính.

Hãy chứng minh (ii). Cho $x \in M \otimes_A \Omega_{A/k}^p, \omega \in \Omega_{A/k}$; bằng cách áp dụng lặp lại (14), ta được :
$$
\nabla \circ \nabla(x \omega) = \nabla(\nabla(x) \omega) + (-1)^p \nabla(x d \omega)
= (\nabla \circ \nabla(x)) \omega + (-1)^{p+1} \nabla(x)(d \omega) + (-1)^p \nabla(x)(d \omega)
= (\nabla \circ \nabla(x)) \omega,
$$
điều này chứng minh mệnh đề thứ nhất của (ii); các mệnh đề khác suy ra ngay lập tức.

## BÀI TẬP {#alg-x-s2-exercises}

Xem [các bài tập cho § 2](exercises/s2/).
