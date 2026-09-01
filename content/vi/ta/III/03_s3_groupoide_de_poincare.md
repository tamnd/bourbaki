---
book: ta
book_title: Topologie algébrique
chapter: III
chapter_title: HOMOTOPIE ET GROUPOÏDE DE POINCARÉ
section: 3
section_title: Groupoïde de Poincaré
lang: vi
source: ta-i-iv-fr
book_pages: TA III.289-TA III.300, TA III.334
pdf_pages: 0305-0316, 0350-0350
extraction: native
subsections:
    - "no": 1
      title: Groupoïde de Poincaré
      page: 289
      pdf_page: 305
    - "no": 2
      title: Fonctorialité du groupoïde de Poincaré
      page: 293
      pdf_page: 309
    - "no": 3
      title: Lacets librement homotopes
      page: 299
      pdf_page: 315
statements: 27
exercises: 2
content_sha256: 9397fd7f40d6837ff24a8dbd91cfd8ed55b4f6925628483c182cd8f5c8fbba6a
translated_from: content/en-mt/ta/III/03_s3_groupoide_de_poincare.md
source_lang: en-mt
translation_method: machine
source_content_sha256: ee54037fd61f5c94a013c52d01e32e0a8d06665295d56ff2380aa432000f2116
translation_model: gpt-5-6-mini
translation_run: translate-vi-0b656786
glossary_version: 34
glossary_terms_sha256: 7d6933132a3b31ef72a9a89c67cfd3fd03e8df8934c0101505528cd5bd172a83
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 3. NHÓMOID POINCARÉ

### 1. Nhómoid Poincaré

#### Định nghĩa 1 {#ta-iii-s3-def-1 .statement tag=01YE}

Cho X là một không gian tôpô, cho $c_0$ và $c_1$ là các đường đi trong X và $\sigma :\mathbf{I}\times \mathbf{I}\rightarrow X$ là một phép đồng luân nối $c_0$ với $c_1$. Người ta nói rằng $\sigma$ là một phép đồng luân ngặt nếu các ánh xạ $s\mapsto \sigma (0, s)$ và $s\mapsto \sigma (1, s)$ là hằng.

Người ta nói rằng các đường đi $c_0$ và $c_1$ trong X là đồng luân ngặt nếu tồn tại một phép đồng luân ngặt nối $c_0$ với $c_1$.

Hai đường đi đồng luân ngặt có cùng gốc và cùng đầu.

#### Ví dụ {#ta-iii-s3-n1-exa-1 .statement tag=01YF}

Cho $c$ là một đường đi trong X và cho $\varphi :\mathbf{I}\rightarrow \mathbf{I}$ là một ánh xạ liên tục sao cho $\varphi (0) = 0$ và $\varphi (1) = 1$. Các đường đi $c$ và $c\circ \varphi$ là đồng luân ngặt. Thật vậy, ánh xạ $\sigma :\mathbf{I}\times \mathbf{I}\rightarrow X$ xác định bởi $\sigma (t, s) =c((1-s)t+s\varphi (t))$ là một phép đồng luân ngặt nối $c$ với $c\circ \varphi$.

Cho X là một không gian tôpô. Nhắc lại (xem III, p. 257) rằng Λ(X) ký hiệu không gian tôpô $\mathscr{C}_c(\mathbf{I}; X)$ của các đường đi trong X và rằng với $x$, $y\in X$, $\Lambda_{x,y}(X)$ là không gian con của Λ(X) gồm các đường đi có gốc $x$ và đầu $y$. Họ các tập hợp $\Lambda_{x,y}(X)$, với $x,y\in X$, là một phân hoạch của không gian các đường đi trong X. Bởi song ánh chính tắc (III, p. 257, nhận xét 2) của $\mathscr{C}(\mathbf{I}\times \mathbf{I}; X)$ lên $\mathscr{C}(\mathbf{I}; \Lambda (X))$, các phép đồng luân ngặt tương ứng với các đường đi $c:\mathbf{I}\rightarrow \Lambda (X)$ có ảnh được chứa trong một không gian con có dạng $\Lambda_{x,y}(X)$. Quan hệ “các đường đi $c_0$ và $c_1$ là đồng luân ngặt” do đó là một quan hệ tương đương trong Λ(X) (III, p. 259, mệnh đề 5) và các lớp tương đương đối với quan hệ này là các thành phần liên thông cung của các không gian con $\Lambda_{x,y}(X)$ của không gian các đường đi trong X. Người ta ký hiệu $\varpi_{x,y}(X)$ là tập hợp $\pi_0(\Lambda_{x,y}(X))$ và gọi mọi phần tử của $\varpi_{x,y}(X)$ là một lớp các đường đi nối $x$ với $y$.

#### Định nghĩa 2 {#ta-iii-s3-def-2 .statement tag=01YG}

Người ta gọi không gian các vòng của X, và ký hiệu là Ω(X), không gian con của Λ(X) gồm các vòng (III, p. 256, định nghĩa 1) trong X.

Người ta ký hiệu $\Omega_x(X)$ là tập hợp $\Lambda_{x,x}(X)$. Các phần tử của $\Omega_x(X)$ được gọi là các vòng trong X tại $x$ và các phần tử của $\varpi_{x,x}(X)$ được gọi là các lớp các vòng trong X tại $x$. Ánh xạ hằng $e_x:\mathbf{I}\rightarrow X$ có ảnh $x$ là một vòng, được gọi là vòng hằng tại $x$; lớp đồng luân ngặt của nó được ký hiệu bởi $\varepsilon_x$. Ánh xạ $x\mapsto e_x$ của X vào Λ(X) là liên tục (III, p. 257, mệnh đề 1).

Cho X là một không gian tôpô và $x,y,z$ là các điểm của X. Bằng cách chuyển qua các thành phần liên thông cung, từ ánh xạ liên tục $c\mapsto \overline{c}$ của $\Lambda_{x,y}(X)$ vào $\Lambda_{y,x}(X)$ (III, p. 258, hệ quả), suy ra một ánh xạ của $\varpi_{x,y}(X)$ vào $\varpi_{y,x}(X)$, được ký hiệu là $\gamma \mapsto \overline{\gamma}$. Nếu $\gamma \in$ $\varpi_{x,y}(X),\overline{\gamma}$ được gọi là nghịch đảo của lớp đường $\gamma$.

Tương tự, nếu đồng nhất các tập hợp $\pi_0(\Lambda_{x,y}(X))\times \pi_0(\Lambda_{y,z}(X))$ và $\pi_0(\Lambda_{x,y}(X)\times \Lambda_{y,z}(X))$ (III, p. 260, Prop. 6), thì từ ánh xạ liên tục $(c, d)\mapsto c*d$ của $\Lambda_{x,y}(X)\times \Lambda_{y,z}(X)$ vào $\Lambda_{x,z}(X)$ (III, p. 258, hệ quả), bằng cách chuyển qua các thành phần liên thông cung, suy ra một ánh xạ $C_{x,y,z}:\varpi_{x,y}(X)\times \varpi_{y,z}(X)\rightarrow \varpi_{x,z}(X)$. Với $\gamma \in \varpi_{x,y}(X)$ và $\delta \in \varpi_{y,z}(X)$, lớp đồng luân ngặt $C_{x,y,z}(\gamma , \delta )$ được ký hiệu là $\gamma \delta$. Nó được gọi là hợp thành của các lớp đường có thể hợp thành $\gamma$ và $\delta$.

Ta có $\overline{\overline{\gamma}}=\gamma$ và $\overline{\gamma \delta}=\delta  \gamma$.

#### Mệnh đề 1 {#ta-iii-s3-prop-1 .statement tag=01YH}

Cho X là một không gian tôpô, cho $x,y,z,u$ là các điểm của X, và cho $\gamma_1\in \varpi_{x,y}(X),\gamma_2\in \varpi_{y,z}(X),\gamma_3\in \varpi_{z,u}(X)$ là các lớp đường. Ta có

$$
\varepsilon_x\gamma_1=\gamma_1\varepsilon_y=\gamma_1 \tag{1}
$$

$$
\gamma_1\overline{\gamma}_1=\varepsilon_x,\overline{\gamma}_1\gamma_1=\varepsilon_y \tag{2}
$$

$$
(\gamma_1\gamma_2)\gamma_3=\gamma_1(\gamma_2\gamma_3) \tag{3}
$$

Cho $c_1\in \Lambda_{x,y}(X),c_2\in \Lambda_{y,z}(X),c_3\in \Lambda_{z,u}(X)$ lần lượt là các đại diện của $\gamma_1,\gamma_2$ và $\gamma_3$. Cho $\varphi :\mathbf{I}\rightarrow \mathbf{I}$ là hàm được xác định bởi

$t/2$ với $0\leqslant t\leqslant 1/2$,

(4) $\varphi (t) =t-1/4$ với $1/2\leqslant t\leqslant 3/4$,

$2t-1$ với $3/4\leqslant t\leqslant 1$.

Hàm $\varphi$ là affine trên mỗi khoảng trong ba khoảng $[0,1/2]$, $[1/2,3/4]$ và $[3/4,1]$; do đó nó liên tục. Ta có $\varphi (0) = 0$ và $\varphi (1) = 1$. Theo công thức (1) của III, p. 256, định nghĩa phép ghép các đường, ta có

$$
c_1*(c_2*c_3) = ((c_1*c_2)*c_3)\circ \varphi
$$

Theo ví dụ của III, p. 289, các đường $c_1*(c_2*c_3)$ và $(c_1*c_2)*c_3$ đồng luân ngặt, do đó có đẳng thức (3).

Tương tự, hàm $\psi :\mathbf{I}\rightarrow \mathbf{I}$ được xác định bởi

$2t$ với $0\leqslant t\leqslant 1/2$,

$$
\psi (t) = \tag{5}
$$

1 với $1/2\leqslant t\leqslant 1$

là liên tục và thỏa mãn $\psi (0) = 0,\psi (1) = 1$. Đẳng thức $\gamma_1\varepsilon_y=\gamma_1$ suy ra từ sự kiện rằng

$$
c_1*e_y=c_1\circ \psi
$$

và đẳng thức $\varepsilon_x\gamma_1=\gamma_1$ được chứng minh tương tự, do đó có (1).

Ánh xạ $\sigma :\mathbf{I}\times \mathbf{I}\rightarrow X$ được xác định bởi

$c_1(2ts)$ với $0\leqslant t\leqslant 1/2$,

$$
\sigma (t, s) = \tag{6}
$$

$c_1(2(1-t)s)$ với $1/2\leqslant t\leqslant 1$

là liên tục; đó là một phép đồng luân ngặt nối đường đi $e_x$ với đường đi $c_1*\overline{c_1}$, do đó có đẳng thức thứ nhất trong (2). Đẳng thức thứ hai suy ra từ đẳng thức thứ nhất và từ sự kiện rằng, với mọi đường đi $c$, ta có $c=\overline{\overline{c}}$.

#### Nhận xét 1 {#ta-iii-s3-n1-rem-1 .statement tag=01YI}

Cho X là một không gian tôpô. Cho $n$ là một số nguyên $\geqslant 1$ và $(c_1, . . . , c_n)$ là một dãy các đường đi trong X sao cho $c_i$ và $c_{i+1}$ có thể ghép được với nhau với $1\leqslant i\leqslant n-1$ (một dãy như vậy được gọi là một dãy các đường đi có thể ghép được với nhau). Ký hiệu $c$ là đường đi

$$
c_1*(c_2*(\cdots  *(c_{n-1}*c_n). . .))
$$

và $c'$ là đường đi được định nghĩa bởi $c'(t) =c_i(nt-i+ 1)$ với $1\leqslant i\leqslant n$ và $t\in [\frac{i-1}{n},\frac{i}{n}]$. Các đường đi $c$ và $c'$ có cùng ảnh và đồng luân ngặt với nhau: một đường là hợp thành của đường kia với một đồng phôi của $\mathbf{I}$ giữ cố định 0 và 1 (xem III, p. 289, ví dụ). Đôi khi ta sẽ ký hiệu đường đi $c'$ bởi $c_1*c_2* \cdots  *c_n$.

Tồn tại duy nhất một đồ thị có hướng $\varpi (X)$ mà tập hợp các đỉnh là X và tập hợp các mũi tên nối một điểm $x$ với một điểm $y$ là $\varpi_{x,y}(X)$, và trong đó các ánh xạ $C_{x,y,z}$ xác định một luật hợp thành. Theo mệnh đề $1,\varpi (X)$ là một groupoid (II, p. 162, định nghĩa 4). Với mọi $x\in X$, phần tử đơn vị tại đỉnh $x$ của groupoid này là lớp của vòng lặp hằng có ảnh $x$. Nghịch đảo của một mũi tên $\gamma$ là mũi tên $\overline{\gamma}$, mà ta cũng sẽ ký hiệu là $\gamma^{-1}$. Đặc biệt, luật hợp thành $C_{x,x,x}$ trang bị cho tập hợp $\varpi_{x,x}(X)$, với mọi $x\in X$, một cấu trúc nhóm; nhóm này được ký hiệu là $\pi_1(X, x)$.

#### Định nghĩa 3 {#ta-iii-s3-def-3 .statement tag=01YJ}

Cho X là một không gian tôpô. Groupoid $\varpi (X)$ được gọi là groupoid Poincaré, hay groupoid cơ bản, của không gian X. Cho $x$ là một điểm của X; nhóm $\pi_1(X, x)$ gồm các lớp của các vòng lặp tại $x$ được gọi là nhóm Poincaré, hay nhóm cơ bản, của không gian X tại điểm $x$.

Cho $\mathscr{U}$ là một tập hợp các tập con của X mà các phần trong của chúng phủ X. Các lớp của các đường đi trong X có ảnh được chứa trong một trong các tập hợp thuộc $\mathscr{U}$ sinh ra groupoid $\varpi (X)$ (bổ đề 4 của III, p. 272).

Các quỹ đạo của groupoid $\varpi (X)$ (II, p. 162) trùng nhau với các thành phần liên thông theo cung của không gian X. Đặc biệt (loc. cit.), ta có:

#### Mệnh đề 2 {#ta-iii-s3-prop-2 .statement tag=01YK}

Cho X là một không gian tôpô.

a) Nếu không gian X liên thông theo cung, các nhóm $\pi_1(X, x)$ và $\pi_1(X, y)$ đẳng cấu với nhau với mọi điểm $x$ và $y$ của X.

b) Cho $x$ là một điểm của X; các điều kiện sau là tương đương:

(i) Nhóm $\pi_1(X, x)$ là tầm thường;

(ii) Hai đường đi có điểm đầu $x$ trong X và có cùng điểm cuối

là đồng luân ngặt với nhau;

(iii) Mọi vòng lặp có điểm đầu $x$ trong X đều đồng luân ngặt với

vòng lặp hằng có ảnh $x$.

Chính xác hơn, cho X là một không gian tôpô liên thông theo cung và $x$ và $y$ là các điểm của X. Với mọi phần tử $\delta$ của $\varpi_{x,y}(X)$, ánh xạ $u_{\delta}:\gamma \mapsto \delta \gamma \delta^{-1}$ của $\pi_1(X, y)$ vào $\pi_1(X, x)$ là một đẳng cấu nhóm mà đẳng cấu nghịch đảo là $u_{\delta^{-1}}$. Với $\delta \in \varpi_{x,y}(X)$ và $\gamma \in \pi_1(X, y)$, ta đặt $^{\delta}\gamma =u_{\delta}(\gamma )$. Khi $x=y$, ta có $^{\delta}\gamma =$ Int($\delta$ )$(\gamma )$, tức là $u_{\delta}=$ Int($\delta$ ).

Cho $x,y,z$ là các điểm của X. Với $\delta \in \varpi_{x,y}(X)$ và $\eta \in \varpi_{y,z}(X)$, ta có $u_{\delta \eta}=u_{\delta}\circ u_{\eta}$, điều này cũng có thể viết là $^{\delta \eta}\gamma =^{\delta}(^{\eta}\gamma )$ với $\gamma \in \pi_1(X, z)$.

Cho $x,y$ là các điểm của X và $\delta ,\delta '$ là các phần tử của $\varpi_{x,y}(X)$. Ta có

(7) $u_{\delta'}=u_{\delta}\circ$ Int($\delta^{-1}\delta '$) $=$ Int($\delta '\delta^{-1}$)$\circ u_{\delta}$.

#### Nhận xét 2 {#ta-iii-s3-n1-rem-2 .statement tag=01YL}

Cho X là một không gian tôpô và C là một thành phần liên thông theo cung của X. Nếu $x$ và $y$ là các điểm của C, không gian tôpô $\Lambda_{x,y}(C)$ được đồng nhất với không gian tôpô $\Lambda_{x,y}(X)$, sao cho tập hợp $\varpi_{x,y}(C)$ được đồng nhất với tập hợp $\varpi_{x,y}(X)$. Do đó, groupoid cơ bản $\varpi (C)$ được đồng nhất với subgroupoid đầy đủ của $\varpi (X)$ có C làm tập hợp các điểm. Đặc biệt, với mọi điểm $x$ của C, nhóm $\pi_1(C, x)$ được đồng nhất với nhóm $\pi_1(X, x)$.

#### Nhận xét 3 {#ta-iii-s3-n1-rem-3 .statement tag=01YM}

Cho X là một không gian tôpô và cho $x,y,z$ là các điểm của X. Ánh xạ $(c, d)\mapsto c*d$ của $\Lambda_{x,y}(X)\times \Lambda_{y,z}(X)$ vào $\Lambda_{x,z}(X)$ là liên tục (III, p. 258, hệ quả của Mệnh đề 2). Cần lưu ý rằng ánh xạ hợp thành $\varpi_{x,y}(X)\times \varpi_{y,z}(X)\rightarrow \varpi_{x,z}(X)$ suy ra từ nó không nhất thiết liên tục khi các tập hợp $\varpi_{x,y}(X),\varpi_{y,z}(X)$ và $\varpi_{x,z}(X)$ được trang bị các tôpô thương (xem TG, I, p. 35 và III, p. 259). Tuy nhiên, với mọi $\gamma_0\in \varpi_{x,y}(X)$ và mọi $\delta_0\in \varpi_{y,z}(X)$, các ánh xạ từng phần $\gamma \mapsto \gamma \delta_0$ của $\varpi_{x,y}(X)$ vào $\varpi_{x,z}(X)$ và $\delta \mapsto \gamma_0\delta$ của $\varpi_{y,z}(X)$ vào $\varpi_{x,z}(X)$ là các đồng phôi. Thật vậy, cho $c_0\in \Lambda_{x,y}(X)$ là một đường đi thuộc lớp $\gamma_0$. Ánh xạ $d\mapsto c_0*d$ là một ánh xạ liên tục của $\Lambda_{y,z}(X)$ vào $\Lambda_{x,z}(X)$. Ánh xạ $\delta \mapsto \gamma_0\delta$ được suy ra từ nó bằng cách chuyển qua các thương, và do đó là liên tục. Điều tương tự đúng cho ánh xạ $\delta '\mapsto \gamma_0^{-1}\delta '$ của $\varpi_{x,z}(X)$ vào $\varpi_{y,z}(X)$. Vì hai ánh xạ này là nghịch đảo của nhau, chúng là các đồng phôi. Người ta lập luận tương tự cho ánh xạ $\gamma \mapsto \gamma \delta_0$. Xem thêm IV, p. 374.

### 2. Tính hàm tử của groupoid Poincaré

Cho X, Y là các không gian tôpô và cho $f: X\rightarrow Y$ là một ánh xạ liên tục. Ánh xạ $c\mapsto f\circ c$ là một ánh xạ liên tục, được ký hiệu là $\Lambda (f)$, của Λ(X) = $\mathscr{C}_c(\mathbf{I}; X)$ vào Λ(Y) = $\mathscr{C}_c(\mathbf{I}; Y)$ (I, p. 132, bổ đề). Bằng cách chuyển qua các tập con, nó xác định các ánh xạ liên tục

$$
\Lambda_x(f): \Lambda_x(X)\rightarrow \Lambda_{f(x)}(Y)
$$

với $x\in X$,

$$
\Lambda_{x,y}(f): \Lambda_{x,y}(X)\rightarrow \Lambda_{f(x),f(y)}(Y)
$$

với $x,y\in X$ và

$$
\Omega (f): \Omega (X)\rightarrow \Omega (Y)
$$

Với $x\in X$, ánh xạ $\Lambda_{x,x}(f)$ cũng được ký hiệu là $\Omega_x(f)$. Bằng cách chuyển qua các thành phần liên thông theo đường đi (III, p. 290), từ ánh xạ $\Lambda_{x,y}(f)$ người ta suy ra một ánh xạ

$$
\varpi_{x,y}(f):\varpi_{x,y}(X)\rightarrow \varpi_{f(x),f(y)}(Y)
$$

Cho $x,y,z$ là các điểm của X và cho $c\in \Lambda_{x,y}(X),d\in \Lambda_{y,z}(X)$ là các đường đi; theo định nghĩa của phép ghép kề các đường đi, ta có

$$
f\circ (c*d) = (f\circ c)*(f\circ d)
$$

Bằng cách chuyển qua các lớp đồng luân ngặt, ta thu được quan hệ

$$
\varpi_{x,z}(f)(\gamma \delta ) = (\varpi_{x,y}(f)(\gamma ))(\varpi_{y,z}(f)(\delta ))
$$

với mọi $\gamma \in \varpi_{x,y}(X)$ và mọi $\delta \in \varpi_{y,z}(X)$. Như vậy, ánh xạ liên tục $f$ và các ánh xạ $\varpi_{x,y}(f)$, với $x$ và $y\in$ X, xác định một cấu xạ của groupoid $\varpi (X)$ vào groupoid $\varpi (Y)$ (II, p. 161, định nghĩa 3). Nó được ký hiệu là $\varpi (f)$ và được gọi là cấu xạ của các groupoid Poincaré suy ra từ ánh xạ liên tục $f$. Đặc biệt, nếu $x$ là một điểm của X, ánh xạ $\varpi_{x,x}(f)$ là một đồng cấu của nhóm $\pi_1(X, x)$ vào nhóm $\pi_1(X, f(x))$; đồng cấu này cũng được ký hiệu là $\pi_1(f, x)$.

#### Nhận xét 1 {#ta-iii-s3-n2-rem-1 .statement tag=01YN}

Đồng cấu $\varpi_{x,y}(f)$ là liên tục nếu trang bị cho các tập $\varpi_{x,y}(X)$ và $\varpi_{f(x),f(y)}(Y)$ tôpô thương của tôpô hội tụ compact trên $\mathscr{C}_c(\mathbf{I}; X)$ và $\mathscr{C}_c(\mathbf{I}; Y)$.

Để đơn giản hóa ký hiệu, nếu $x,y\in X$ và $\gamma \in \varpi_{x,y}(X)$, đôi khi ta sẽ viết $f_*(\gamma )$ cho phần tử $\varpi_{x,y}(f)(\gamma )$ của $\varpi_{f(x),f(y)}(Y)$.

Cho X, Y, Z là các không gian tôpô, cho $f: X\rightarrow Y,g: Y\rightarrow Z$ là các ánh xạ liên tục. Với mọi đường đi $c$ trong X, ta có $(g\circ f)\circ c=$ $g\circ (f\circ c)$. Do đó ta có

$$
\varpi (g\circ f) =\varpi (g)\circ \varpi (f)
$$

Cho X và Y là các không gian tôpô, cho $f_0$ và $f_1$ là các ánh xạ liên tục từ X vào Y, và cho $\sigma : X\times \mathbf{I}\rightarrow Y$ là một phép đồng luân nối $f_0$ với $f_1$. Vì ánh xạ $(c, t)\mapsto c(t)$ từ $\mathscr{C}_c(\mathbf{I}; X)\times \mathbf{I}$ vào X (III, p. 257, prop. 1) là liên tục, điều tương tự cũng đúng đối với ánh xạ từ $\mathscr{C}_c(\mathbf{I}; X)\times \mathbf{I}\times \mathbf{I}$ vào Y được cho bởi $(c, t, s)\mapsto \sigma (c(t), s)$. Do đó, ánh xạ $\Sigma : (c, s)\mapsto \sigma (c(\cdot ), s)$ là một ánh xạ liên tục từ $\mathscr{C}_c(\mathbf{I}; X)\times \mathbf{I}$ vào $\mathscr{C}_c(\mathbf{I}; Y)$ (loc. cit.). Ánh xạ Σ là một phép đồng luân nối ánh xạ $\Lambda (f_0)$ với ánh xạ $\Lambda (f_1)$. Bằng cách hạn chế vào các không gian vòng, ánh xạ Σ cảm sinh một phép đồng luân $\Omega (X)\times \mathbf{I}\rightarrow \Omega (Y)$ nối $\Omega (f_0)$ với $\Omega (f_1)$. Cho $x$ là một điểm của X; giả sử rằng phép đồng luân $\sigma$ là một phép đồng luân tại điểm $x$, và đặt $y=f_0(x) =f_1(x)$. Khi đó ánh xạ Σ cảm sinh một ánh xạ liên tục từ $\Omega_x(X)\times \mathbf{I}$ vào $\Omega_y(Y)$ là một phép đồng luân tại điểm $e_x$, nối ánh xạ $\Omega_x(f_0)$ với ánh xạ $\Omega_x(f_1)$.

#### Mệnh đề 3 {#ta-iii-s3-prop-3 .statement tag=01YO}

Cho X và Y là các không gian tôpô, $f_0$ và $f_1$ là các ánh xạ liên tục từ X vào Y, và cho $\sigma : X\times \mathbf{I}\rightarrow$ Y là một phép đồng luân nối $f_0$ với $f_1$. Cho $x$ là một điểm của X; đặt $y_0=f_0(x)$, $y_1=f_1(x)$, và ký hiệu $\delta \in \varpi_{y_0,y_1}(Y)$ là lớp của đường đi $d$ được xác định bởi $d(t) =\sigma (x, t)$ với $t\in \mathbf{I}$. Với mọi $\gamma \in \pi_1(X, x)$, ta có $(f_1)_*(\gamma ) =$ $\delta^{-1}((f_0)_*(\gamma ))\delta$.

Cho $c$ là một đường kín trong X tại $x$ và $\gamma$ là lớp đồng luân ngặt của nó. Đặt $\gamma_0= (f_0)_*(\gamma )$ và $\gamma_1= (f_1)_*(\gamma )$; đây là các lớp đồng luân ngặt của $f_0\circ c$ và $f_1\circ c$. Với $(t, s)\in \mathbf{I}\times \mathbf{I}$, đặt $\varphi (t, s) =\sigma (c(t), s)$. Với mọi $t\in \mathbf{I}$, ta có $\varphi (t,0) = (f_0\circ c)(t),\varphi (t,1) = (f_1\circ c)(t)$ và $\varphi (0, t) =\varphi (1, t) =d(t)$. Quan hệ $\gamma_0\delta =\delta \gamma_1$ do đó suy ra từ bổ đề sau.

#### Bổ đề 1 {#ta-iii-s3-lem-1 .statement tag=01YP}

Cho Y là một không gian tôpô và $\varphi :\mathbf{I}\times \mathbf{I}\rightarrow Y$ là một ánh xạ liên tục. Với $t\in \mathbf{I}$, đặt $c_0(t) =\varphi (t,0),c_1(t) =\varphi (t,1)$, $d_0(t) =\varphi (0, t)$ và $d_1(t) =\varphi (1, t)$. Các đường đi $c_0*d_1$ và $d_0*c_1$ đồng luân ngặt.

Gọi $c$ là đường đi trong $\mathbf{I}\times \mathbf{I}$ nhận được bằng cách ghép nối các đường đi $t\mapsto (t,0)$ và $t\mapsto (1, t)$; gọi $d$ là đường đi trong $\mathbf{I}\times \mathbf{I}$ nhận được bằng cách ghép nối các đường đi $t\mapsto (0, t)$ và $t\mapsto (t,1)$. Các đường đi $c$ và $d$ có cùng điểm đầu $(0,0)$ và cùng điểm cuối $(1,1)$. Ánh xạ $(t, s)\mapsto$ $(1-s)c(t)+sd(t)$ từ $\mathbf{I}\times \mathbf{I}$ vào $\mathbf{I}\times \mathbf{I}$ là một đồng luân ngặt nối $c$ với $d$. Ta có $c_0*d_1=\varphi \circ c$ và $d_0*c_1=\varphi \circ d$; do đó hai đường đi này đồng luân ngặt.

#### Hệ quả 1 {#ta-iii-s3-lem-1-cor-1 .statement tag=01YQ}

Cho X và Y là các không gian tôpô và $x$ là một điểm của X. Cho $f_0$ và $f_1$ là các ánh xạ liên tục từ X vào Y. Nếu tồn tại một đồng luân có điểm tại $x$ nối $f_0$ với $f_1$, thì $\pi_1(f_0, x) =$ $\pi_1(f_1, x)$.

Gọi $\sigma$ là một đồng luân có điểm tại $x$ nối $f_0$ với $f_1$. Với ký hiệu của Mệnh đề $3,\delta$ là lớp của một đường đi hằng có ảnh $f_0(x) =$ $f_1(x)$. Mệnh đề được suy ra.

#### Hệ quả 2 {#ta-iii-s3-lem-1-cor-2 .statement tag=01YR}

Cho X và Y là các không gian tôpô và $f: X\rightarrow$ Y là một đồng phôi. Với mọi điểm $x$ của X, đồng cấu

$$
\pi_1(f, x):\pi_1(X, x)\rightarrow \pi_1(Y, f(x))
$$

là một đẳng cấu.

Cho $g$ là một ánh xạ liên tục từ Y vào X, nghịch đảo của $f$ theo nghĩa đồng luân. Cho $x$ là một điểm của X. Theo Mệnh đề 3 áp dụng cho các ánh xạ đồng luân Id$_X$ và $g\circ f: X\rightarrow X$, suy ra ánh xạ $\pi_1(g\circ f, x)$ là một đẳng cấu của nhóm $\pi_1(X, x)$ lên nhóm $\pi_1(X, g\circ f(x))$. Vì

$$
\pi_1(g\circ f, x) =\pi_1(g, f(x))\circ \pi_1(f, x)
$$

đồng cấu $\pi_1(f, x)$ là đơn ánh và đồng cấu $\pi_1(g, f(x))$ là toàn ánh. Vì ánh xạ $g$ cũng là một tương đương đồng luân, đồng cấu $\pi_1(g, f(x))$ là đơn ánh; do đó nó là một đẳng cấu. Suy ra $\pi_1(f, x)$ là một đẳng cấu.

#### Ví dụ {#ta-iii-s3-n2-exa-1 .statement tag=01YS}

Cho G là một nhóm tôpô, cho $e$ là phần tử đơn vị của nó. Với mọi điểm $g$ của G, các phép tịnh tiến trái và phải, $x\mapsto gx$ và $x\mapsto xg$, là các đồng phôi của G lên chính nó (TG, III, p. 2) biến $e$ thành $g$. Theo Hệ quả 2, chúng cảm sinh các đẳng cấu của $\pi_1(G, e)$ lên $\pi_1(G, g)$. Các đẳng cấu này không nhất thiết bằng nhau (IV, p. 459, exerc. 1).

#### Hệ quả 3 {#ta-iii-s3-lem-1-cor-3 .statement tag=01YT}

Cho X là một không gian tôpô đồng luân với một điểm. Với mọi điểm $x$ của X, nhóm $\pi_1(X, x)$ thu về phần tử đơn vị.

Hệ quả 3 áp dụng đặc biệt khi X là không gian số $n$ chiều $\mathbf{R}^n$ và nói chung hơn khi X là một tập con của không gian $\mathbf{R}^n$ có dạng sao (III, p. 234) đối với một trong các điểm của nó.

#### Mệnh đề 4 {#ta-iii-s3-prop-4 .statement tag=01YU}

Cho X là không gian tích của một họ $(X_j)_{j\in J}$ các không gian tôpô. Cấu xạ của groupoid $\varpi (X)$ vào tích của các groupoid $\varpi (X_j)$, với $j\in J$, được xác định bởi họ các cấu xạ $(\varpi$(pr$_j$))$_{j\in J}$ là một đẳng cấu.

Cho $\varphi$ ký hiệu cấu xạ này của các groupoid. Ánh xạ suy ra từ nó bằng cách chuyển qua các đỉnh là ánh xạ đồng nhất $X\rightarrow \prod_jX_j$. Cho $x= (x_j)$ và $y= (y_j)$ là hai điểm của X. Cho $\varphi_{x,y}$ ký hiệu ánh xạ của $\varpi_{x,y}(X)$ vào $\prod_j\varpi_{x_j,y_j}(X_j)$ suy ra từ $\varphi$. Nếu với mọi $j\in J,c_j:\mathbf{I}\rightarrow$ $X_j$ là một đường đi nối $x_j$ với $y_j$, thì ánh xạ $t\mapsto (c_j(t))$ là một đường đi trong X nối $x$ với $y$ (TG, I, p. 25, prop. 1). Điều này chứng minh rằng $\varphi_{x,y}$ là toàn ánh. Cho $c$ và $d$ là hai đường đi trong X nối $x$ với $y$. Giả sử rằng với mọi $j\in J$ tồn tại một đồng luân ngặt $\sigma_j:\mathbf{I}\times \mathbf{I}\rightarrow X_j$ nối pr$_j\circ c$ với pr$_j\circ d$. Khi đó ánh xạ $(t, s)\mapsto (\sigma_j(t, s))$ của $\mathbf{I}\times \mathbf{I}$ vào X là một đồng luân ngặt nối $c$ với $d($loc. cit.). Điều này chứng minh rằng $\varphi_{x,y}$ là đơn ánh.

#### Hệ quả {#ta-iii-s3-n2-cor-1 .statement tag=01YV}

Cho $x= (x_j)_{j\in J}$ là một điểm của X. Ánh xạ

$$
\pi_1(X, x)\rightarrow \prod_{j\in J}\pi_1(X_j, x_j)
$$

suy ra từ các ánh xạ $\pi_1$(pr$_j, x_j$) là một đẳng cấu nhóm.

Đẳng cấu này được gọi là chính tắc. Trong phần tiếp theo, ta sẽ thường đồng nhất $\pi_1(X, x)$ với $\prod_{j\in J}\pi_1(X_j, x_j)$ nhờ đẳng cấu này.

#### Nhận xét 2 {#ta-iii-s3-n2-rem-2 .statement tag=01YW}

Cho $(X_j)_{j\in J}$ là một họ các không gian tôpô. Gọi X là không gian tôpô tích $\prod_{j\in J}X_j$ và cho $x= (x_j)$ là một điểm của X.

Với mọi $i\in J$, cho $u_i: X_i\rightarrow X$ là ánh xạ sao cho, với $z\in X_i$, pr$_i\circ u_i(z) =z$ và, với mọi $j\in J$ phân biệt với $i$, pr$_j\circ u_i(z) =$ $x_j$. Ánh xạ $u_i$ là liên tục và ánh xạ $\pi_1(u_i, x_i)$ được đồng nhất với đơn ánh chính tắc của nhân tử $\pi_1(X_i, x_i)$ vào nhóm tích của họ $(\pi_1(X_j, x_j))_{j\in J}($cf. A, I, p. 45).

Giả sử tập hợp J là hữu hạn và, với mọi $j\in J$, cho $\gamma_j$ là một phần tử của $\pi_1(X_j, x_j)$. Phần tử $(\gamma_j)$ của $\pi_1(X, x)$ là hợp thành của các lớp của các vòng $(u_j)_*(\gamma_j),j\in J$, các lớp này từng đôi một hoán vị được.

#### Nhận xét 3 {#ta-iii-s3-n2-rem-3 .statement tag=01YX}

Cho $(X_j)_{j\in J}$ là một họ các không gian tôpô. Gọi X là không gian tôpô tích $\prod_{j\in J}X_j$ và cho $x= (x_j)$ là một điểm của X.

Trang bị cho các tập $\pi_1(X, x)$ và $\pi_1(X_j, x_j)$ tôpô thương của tôpô hội tụ compact trên các không gian $\Lambda_x(X)$ và $\Lambda_{x_j}(X_j)$. Khi đó đẳng cấu $\pi_1(X, x)\rightarrow \prod_{j\in J}\pi_1(X_j, x_j)$ là một đồng phôi. Nó liên tục (III, p. 294, nhận xét 1). Tôpô hội tụ compact trên Λ(X) được sinh bởi các tập con có dạng $\mathbf{T}(K,U)$, trong đó K là một tập con compact của $\mathbf{I}$ và U là một tập con mở của X. Với $j\in J$, cho $U_j$ là một tập con mở của $X_j$, sao cho $\prod_{j\in J}U_j\subset U$. Khi đó (pr$_j$)$_*(\mathbf{T}(K,U))$ chứa $\mathbf{T}(K,U_j)$. Điều này cho thấy các ánh xạ (pr$_j$)$_*: \Lambda_x(X)\rightarrow \Lambda_{x_j}(X_j)$ là mở, và các ánh xạ $\pi_1$(pr$_j, x_j$) cũng là mở. Vì chúng toàn ánh, ánh xạ $\pi_1(X, x)\rightarrow \prod_{j\in J}\pi_1(X_j, x_j)$ là mở (TG, I, p. 34, Mệnh đề 8). Là liên tục và song ánh, nó là một đồng phôi (TG, I, p. 30, ví dụ 2).

#### Mệnh đề 5 {#ta-iii-s3-prop-5 .statement tag=01YY}

Cho X là một không gian tôpô và $(A_i)_{i\in I}$ là một họ tăng các tập con của X, được chỉ số bởi một tập I có thứ tự lọc, sao cho mọi tập con gần compact của X đều được chứa trong một trong các $A_i$. Cấu xạ nhómoid chính tắc

$\rho :$ lim$\longrightarrow_{i\in I}\varpi (A_i)\rightarrow \varpi (X)$,

cảm sinh bởi các đơn ánh chính tắc của $A_i$ vào X, là một đẳng cấu.

Nếu $i\leqslant j$, ký hiệu $\rho_{j,i}$ là cấu xạ nhómoid $\varpi (A_i)\rightarrow \varpi (A_j)$ cảm sinh bởi đơn ánh của $A_i$ vào $A_j$. Vì ánh xạ cảm sinh bởi $\rho_{j,i}$ khi chuyển qua các đỉnh là đơn ánh $A_i\rightarrow A_j$ và vì các $A_i$ phủ X, ánh xạ cảm sinh bởi $\rho$ khi chuyển qua các đỉnh là song ánh.

Cho $a$ và $b$ là các điểm của X và cho $c$ là một đường đi nối a với b trong X. Ảnh của c là một tập con gần compact của X (TG, I, p. 62, Định lý 2), vì $\mathbf{I}$ là compact. Do đó tồn tại một phần tử $i\in I$ sao cho ảnh của c được chứa trong $A_i$. Do đó, ánh xạ cảm sinh bởi $\rho$ khi chuyển qua các tập hợp mũi tên là toàn ánh.

Cho $i\in I$, cho $a$ và $b$ là các điểm của $A_i$, cho $c,c'$ là các đường đi nối $a$ với $b$ trong $A_i$; cho $h$ là một đồng luân ngặt nối $c$ với $c'$ trong X. Vì $\mathbf{I}\times \mathbf{I}$ là compact, $h(\mathbf{I}\times \mathbf{I})$ là một tập con quasi-compact của X (loc. cit.) và tồn tại một phần tử $i\in I$ sao cho ảnh của $h$ được chứa trong $A_i$. Các đường đi $c$ và $c'$ đồng luân ngặt trong $A_i$; a fortiori, các lớp đường đi $[c]$ và $[c']$ có cùng ảnh trong lim$\longrightarrow \varpi (A_i)$. Do đó, $\rho$ là đơn ánh.

#### Hệ quả {#ta-iii-s3-n2-cor-2 .statement tag=01YZ}

Cho $a$ là một điểm của X và cho J là tập hợp các $i\in I$ sao cho $a\in A_i$. Đồng cấu chính tắc

lim$\longrightarrow_{i\in J}\pi_1(A_i, a)\rightarrow \pi_1(X, a)$

là song ánh.

#### Nhận xét 4 {#ta-iii-s3-n2-rem-4 .statement tag=01Z0}

Mệnh đề và hệ quả của nó áp dụng đặc biệt khi $(A_i)_{i\in I}$ là một họ tăng các tập con của X được chỉ số bởi một tập hợp có thứ tự có hướng I sao cho các phần trong của $A_i$ phủ X.

### 3. Các vòng tự do đồng luân

#### Định nghĩa 4 {#ta-iii-s3-def-4 .statement tag=01Z1}

Cho X là một không gian tôpô và cho $c$ và $c'$ là hai vòng trong X. Một đồng luân tự do nối $c$ với $c'$ có nghĩa là một đồng luân $\sigma$ nối $c$ với $c'$ sao cho $\sigma (0, s) =\sigma (1, s)$ với mọi $s\in \mathbf{I}$. Ta nói rằng $c$ tự do đồng luân với $c'$ nếu tồn tại một đồng luân tự do nối $c$ với $c'$.

Các đồng luân tự do nối $c$ với $c'$ tương ứng với các đường đi nối $c$ với $c'$ trong không gian Ω(X) của các vòng trong X. Do đó, quan hệ “$c$ tự do đồng luân với $c'$” là một quan hệ tương đương trong Ω(X) mà các lớp tương đương của nó là các thành phần liên thông theo cung của Ω(X).

#### Nhận xét {#ta-iii-s3-n3-rem-1 .statement tag=01Z2}

Cho $\varphi$ là ánh xạ chính tắc của $\mathbf{R}$ lên $\mathbf{T}=\mathbf{R}/\mathbf{Z}$ (TG, V, p. 2). Ánh xạ $f\mapsto f\circ \varphi |\mathbf{I}$ là một đồng phôi của $\mathscr{C}_c(\mathbf{T}; X)$ lên Ω(X), do đó, bằng cách chuyển qua các thành phần liên thông theo cung, một song ánh của tập hợp $[\mathbf{T}; X]$ (III, p. 230) lên tập hợp các lớp đồng luân tự do của các vòng trong X.

#### Mệnh đề 6 {#ta-iii-s3-prop-6 .statement tag=01Z3}

Cho X là một không gian tôpô liên thông theo cung và cho $x$ là một điểm của X.

a) Mọi vòng trong X đều đồng luân tự do với một vòng tại $x$. Chính xác hơn, nếu $c$ là một vòng tại $y$ và $d$ là một đường đi có điểm đầu $y$ và điểm cuối $x$, thì $c$ đồng luân tự do với vòng $(\overline{d}*c)*d$ tại $x$.

b) Hai vòng trong X tại $x$ đồng luân tự do khi và chỉ khi các lớp đồng luân ngặt của chúng liên hợp trong nhóm $\pi_1(X, x)$.

Ta chứng minh a). Với mọi $s\in [0,1]$, gọi $d_s$ là đường đi trong X được định nghĩa bởi $d_s(t) =d(st)$ với $t\in \mathbf{I}$; điểm đầu của nó là $y$. Vì ánh xạ $(s, t)\mapsto d(st)$ liên tục, nên ánh xạ $s\mapsto d_s$ từ $\mathbf{I}$ vào $\mathscr{C}_c(\mathbf{I}; X)$ là liên tục (III, p. 257, mệnh đề 1). Khi đó ánh xạ $s\mapsto (\overline{d_s}*c)*d_s$ là một đường đi trong Ω(X) (III, p. 257, mệnh đề 2) nối $(e_y*c)*e_y$ với $(\overline{d}*c)*d$, do đó a).

Cho $c$ và $c'$ là hai vòng trong X tại $x$. Nếu các lớp đồng luân ngặt của chúng liên hợp trong $\pi_1(X, x)$, thì tồn tại một vòng $d$ tại $x$ sao cho $c'$ đồng luân ngặt với vòng $(\overline{d}*c)*d$. Theo a), suy ra $c$ và $c'$ đồng luân tự do. Ngược lại, giả sử tồn tại một đồng luân tự do $\varphi$ nối $c$ với $c'$. Đặt $d(t) =\varphi (0, t)$; ta cũng có $d(t) =\varphi (1, t)$ và $d$ là một vòng tại $x$. Theo bổ đề 1 của III, p. 295, các vòng $c*d$ và $d*c'$ đồng luân ngặt. Do đó các lớp đồng luân ngặt của $c$ và $c'$ liên hợp trong $\pi_1(X, x)$.

#### Chú giải {#ta-iii-s3-n3-sch-1 .statement tag=01Z4}

Cho X là một không gian tôpô liên thông theo cung và $x$ là một điểm của X. Mệnh đề 6 cho phép định nghĩa một song ánh chính tắc từ tập hợp các lớp đồng luân tự do của các vòng trong X lên tập hợp các lớp liên hợp trong $\pi_1(X, x)$.

## BÀI TẬP {#ta-iii-s3-exercises}
