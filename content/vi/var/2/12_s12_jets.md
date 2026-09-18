---
book: var
book_title: Variétés différentielles et analytiques
chapter: "2"
chapter_title: VARIÉTÉS DIFFÉRENTIELLES ET ANALYTIQUES, FASCICULE DE RÉSULTATS
section: 12
section_title: Jets
lang: vi
source: var-fr
pdf_pages: 0143-0151
extraction: ocr
subsections:
    - "no": 1
      title: Jets d’applications
      page: 0
      pdf_page: 143
    - "no": 2
      title: Jets d’applications d’espaces de Banach
      page: 0
      pdf_page: 144
    - "no": 3
      title: Variétés de jets
      page: 0
      pdf_page: 144
    - "no": 4
      title: Repères et fibrations principales
      page: 0
      pdf_page: 146
    - "no": 5
      title: Jets de sections
      page: 0
      pdf_page: 147
    - "no": 6
      title: Jets de sections d’un fibré vectoriel
      page: 0
      pdf_page: 148
    - "no": 7
      title: Affaiblissement de structure
      page: 0
      pdf_page: 150
statements: 1
exercises: 0
content_sha256: 00b3497081930699afe6e24a6a55824cb5f755afa45ef4f9809be69797ab6144
translated_from: content/en-mt/var/2/12_s12_jets.md
source_lang: en-mt
translation_method: machine
source_content_sha256: 6a78df6ef6f5cba7d9349c6327ba42a6324ad921a394aeb47acd6d730a4fa2b8
translation_model: gpt-5-6, gpt-5-6-mini
translation_run: translate-vi-17c53b1c
glossary_version: 34
glossary_terms_sha256: 81074f021bd29e950116a92082f9490e96578bee8d6bc209e7105d53e69c2855
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 12. Jets

Trong đoạn này, ta ký hiệu $X$ và $Y$ là hai đa tạp thuộc lớp $C^r$, trong đó $r \in \mathbf{N}_k$, và $k$ là một số nguyên sao cho $0 \leq k \leq r$.

Từ No. 12.3 trở đi, ta giả sử:

— hoặc $K$ có đặc số không;

— hoặc các đa tạp, không gian Banach và bó vectơ được xét có số chiều hữu hạn địa phương.

### 12.1. Jets của ánh xạ

### 12.1.1. Cho $x \in X$ và $f, g$ là hai ánh xạ liên tục xác định trong một lân cận của $x$ và nhận giá trị trong $Y$. Ta nói rằng $f$ và $g$ có tiếp xúc cấp $\geq k$ tại $x$ nếu $f(x)=g(x)$ và tồn tại các bản đồ $(U,\varphi,E)$ của $X$ tại $x$ và $(V,\psi,F)$ của $Y$ tại $f(x)$ sao cho các ánh xạ $\psi \circ f \circ \varphi^{-1}$ và $\psi \circ g \circ \varphi^{-1}$, được xác định trong một lân cận của $\varphi(x)$ trong $E$ và nhận giá trị trong $F$, có tiếp xúc cấp $\geq k$ tại $\varphi(x)$ (1.1.2). Tính chất này khi đó được thỏa mãn bởi mọi bản đồ của $X$ tại $x$ và của $Y$ tại $f(x)$.

### 12.1.2. Cho $x \in X$, $y \in Y$. Trong tập hợp các ánh xạ thuộc lớp $C^r$ được xác định trong một lân cận của $x$, nhận giá trị trong $Y$, và ánh xạ $x$ lên $y$, quan hệ « $f$ và $g$ có tiếp xúc cấp $\geq k$ » là một quan hệ tương đương; lớp của $f$ đối với quan hệ này được ký hiệu bởi $j^k_x(f)$ và được gọi là jet cấp $k$ của $f$ với nguồn $x$ và đích $y$. Nguồn của một jet được ký hiệu bởi $s(j)$ và đích của nó bởi $b(j)$.

Tập hợp các jet cấp $k$ từ $X$ vào $Y$ (tương ứng với nguồn $x$, tương ứng với đích $y$) được ký hiệu bởi $J^k(X,Y)$ (tương ứng $J^k_x(X,Y)$, tương ứng $J^k(X,Y)_y$) và ta đặt

$$
J^k(X,Y)_y^x = J^k_x(X,Y) \cap J^k(X,Y)_y.
$$

### 12.1.3. Nếu $U$ và $V$ lần lượt là các tập con mở của $X$ và $Y$, thì theo một cách hiển nhiên, người ta đồng nhất $J^k(U,V)$ với ảnh ngược của $U \times V$ qua ánh xạ

$$
(s,b): J^k(X,Y) \longrightarrow X \times Y.
$$

### 12.1.4. Cho $Z$ là một đa tạp lớp $C^r$, và cho $(x,y,z) \in X \times Y \times Z$. Cho $j \in J^k(X,Y)_y$ và $j' \in J^k(Y,Z)_z$. Các ánh xạ $f' \circ f$, với $f \in j$ và $f' \in j'$, có cùng jet cấp $k$ tại $x$; jet này được gọi là hợp của $j$ và $j'$ và được ký hiệu là $j' \circ j$; ta có $s(j' \circ j)=s(j)$ và $b(j' \circ j)=b(j')$. Nếu $T$ là một đa tạp lớp $C^r$ và nếu $j'' \in J^k_z(Z,T)$, thì ta có

$$
j'' \circ (j' \circ j)=(j'' \circ j')\circ j.
$$

12.1.5. Cho $j \in J_x^k(X, Y)$, với $x \in X$, và cho $k'$ là một số nguyên sao cho $0 \leq k' \leq k$. Các jet $j_x^{k'}(f)$, với $f \in j$, bằng nhau; jet được xác định như vậy được ký hiệu là $r^{k', k}(j)$; ánh xạ $r^{k, k'} : J^k(X, Y) \to J^{k'}(X, Y)$ là toàn ánh.

12.1.6. Giả sử $r$ bằng $\infty$ hoặc $\omega$. Cho $f$ và $g$ là hai ánh xạ lớp $C^r$ được xác định trong một lân cận của một điểm $x \in X$, và nhận giá trị trong $Y$. Nếu $j_x^m(f) = j_x^m(g)$ với mọi số nguyên $m \geq 0$, người ta nói rằng $f$ và $g$ có tiếp xúc cấp vô hạn tại $x$. Như vậy ta được một quan hệ tương đương mà các lớp của nó được gọi là các jet cấp vô hạn tại $x$; jet cấp vô hạn của $f$ được ký hiệu bởi $j_x^\infty(f)$ hoặc $j_x^\omega(f)$. Các định nghĩa và kết quả ở trên mở rộng không thay đổi đến các jet cấp vô hạn.

### 12.2. Các jet của ánh xạ giữa các không gian Banach

Trong No. này, $E$ và $F$ ký hiệu hai không gian Banach. Nếu $m$ là một số nguyên $\geq 0$, ta ký hiệu $P_m(E; F)$ là không gian Banach của các đa thức thuần nhất liên tục bậc $m$ trên $E$ nhận giá trị trong $F$ (Phần 1, phụ lục, A.2).

12.2.1. Cho U là một tập con mở của E, cho $f : U \to F$ là một ánh xạ thuộc lớp $C^r$, và cho $a \in U$. Tồn tại duy nhất một đa thức liên tục
$$
\tilde{f} = f_0 + \cdots + f_k \quad (\text{avec } f_m \in P_m(E; F))
$$
có bậc $\leq k$, có tại gốc cùng một jet cấp $k$ với ánh xạ $x \mapsto f(x - a)$. Nếu $0 \leq m \leq k$, thành phần thứ $m$ $f_m$ của $\tilde{f}$ được ký hiệu là $\Delta^m f(a)$ hoặc $\Delta_a^m(f)$. Khi $r = \omega$, ký hiệu này trùng với ký hiệu của 3.2.1 và 4.2.1; khi $r \leq \infty$, ta có
$$
m! \Delta^m f(a)(h) = D^m f(a)(h, \ldots, h) = D^m f(a) . h^m.
$$
Ánh xạ $f \mapsto \tilde{f}$ xác định, bằng phép chuyển qua thương, một song ánh từ $J_a^k(E, F)$ lên $\prod_{0 \leq m \leq k} P_m(E; F)$ nhờ đó hai không gian này được đồng nhất; đặc biệt, $J_a^k(E, F)$ được trang bị một cấu trúc không gian Banach trên K. Nếu $j \in J_a^k(E, F)$, ta ký hiệu $\Delta_a^m(j)$ là thành phần thứ $m$ của $j$; ta có
$$
\Delta_a^m(j) \in P_m(E; F) \quad \text{pour} \quad 0 \leq m \leq k, \quad \text{et} \quad \Delta_a^0(j) = b(j) \in F.
$$

12.2.2. Cho U (resp. V) là một tập con mở của E (resp. F). Ký hiệu $Q^k(E, F)$ là không gian Banach tích của các $P_m(E; F)$ với $1 \leq m \leq k$. Ánh xạ
$$
j \mapsto (s(j), b(j), \Delta_{s(j)}^1(j), \ldots, \Delta_{s(j)}^k(j))
$$
là một song ánh từ $J^k(U, V)$ lên $U \times V \times Q^k(E, F)$, nhờ đó hai tập hợp này được đồng nhất. Đặc biệt, $J_0^k(E, F)_0$ được đồng nhất với $Q^k(E, F)$.

### 12.3. Các đa tạp jet

12.3.1. Cho $c = (U, \varphi, E)$ và $c' = (V, \psi, F)$ lần lượt là các biểu đồ của X và Y. Các ánh xạ $\varphi$ và $\psi$ xác định, bằng phép chuyển cấu trúc, một song ánh $\pi$ từ $J^k(U, V)$ lên
$$
J^k(\varphi(U), \psi(V)) = \varphi(U) \times \psi(V) \times Q^k(E, F),
$$
xem 12.2.2. Nếu đặt $W = J^k(U, V)$ và $G = E \times F \times Q^k(E, F)$, bộ ba $(W, \pi, G)$ là một biểu đồ của $J^k(X, Y)$. Các biểu đồ thu được như vậy lập thành một atlas $C^{r-k}$ và điều này trang bị cho $J^k(X, Y)$ một *cấu trúc của một K-đa tạp thuộc lớp $C^{r-k}$*[^1]

Nếu $(x, y) \in X \times Y$, các tập hợp $J_x^k(X, Y), J^k(X, Y)_y$ và $J_x^k(X, Y)_y$ là các đa tạp con đóng của $J^k(X, Y)$.

12.3.2. Nếu $X$ và $Y$ đều thuần (resp. hữu hạn chiều, resp. tách được, resp. liên thông), thì điều tương tự cũng đúng đối với $J^k(X, Y)$.

Nếu $U$ (resp. $V$) là mở trong $X$ (resp. trong $Y$), $J^k(U, V)$ là một đa tạp con mở của $J^k(X, Y)$, xem 12.1.3.

12.3.3. Các ánh xạ $s : J^k(X, Y) \to X, b : J^k(X, Y) \to Y$ và $(s, b) : J^k(X, Y) \to X \times Y$ là các phân thớ (6.1.1) thuộc lớp $C^{r-k}$. Khi $k = 0$, $(s, b)$ là một đẳng cấu.

12.3.4. Gọi $T_X$ và $T_Y$ là các bó vectơ $pr_1^* T(X)$ và $pr_2^* T(Y)$ trên $X \times Y$, và gọi $\mathscr{L}(T_X; T_Y)$ là bó các đồng cấu từ $T_X$ vào $T_Y$ (7.7.3); nếu $(x, y) \in X \times Y$, ta có
$$
\mathscr{L}(T_X; T_Y)_{(x, y)} = \mathscr{L}(T_x(X); T_y(Y)).
$$
Cho $j \in J^k(X, Y), k \geqslant 1$, và $f \in j$. Ánh xạ tiếp tuyến của $f$ tại $x = s(j)$ chỉ phụ thuộc vào $j$; ta ký hiệu nó bởi $T(j)$; nó là một phần tử của $\mathscr{L}(T_x(X); T_y(Y))$, trong đó $y = b(j)$. Khi $k = 1$, ánh xạ
$$
T : J^1(X, Y) \to \mathscr{L}(T_X; T_Y)
$$
thu được là một đẳng cấu của các đa tạp thuộc lớp $C^{r-1}$.

Với $X = K$, đẳng cấu này đồng nhất $J_0^1(K, Y)$ với $T(Y)$; với $Y = K$, nó đồng nhất $J^1(X, K)_0$ với không gian đối ngẫu $T'(X)$ của $T(X)$.

12.3.5. Cho $k'$ là một số nguyên sao cho $0 \leqslant k' \leqslant k$. Ánh xạ
$$
\rho^{k, k'} : J^k(X, Y) \to J^{k'}(X, Y)
$$
là một phân thớ thuộc lớp $C^{r-k}$.

12.3.6. Cho $Z$ là một đa tạp thuộc lớp $C^r$, và cho $T$ là tập hợp các cặp
$$
(j, j') \in J^k(X, Y) \times J^k(Y, Z)
$$
sao cho $b(j) = s(j')$. Khi đó $T$ là một đa tạp con của $J^k(X, Y) \times J^k(Y, Z)$ và ánh xạ $(j, j') \mapsto j' \circ j$ là một cấu xạ thuộc lớp $C^{r-k}$ từ $T$ vào $J^k(X, Z)$.

12.3.7. Nếu $f : X \to Y$ là một cấu xạ thuộc lớp $C^r$, ánh xạ $x \mapsto j_x^k(f)$ là một cấu xạ $j^k(f)$ thuộc lớp $C^{r-k}$ từ $X$ vào $J^k(X, Y)$.

12.3.8. Cho $k'$ và $k''$ là các số nguyên dương có tổng bằng $k$. Cho $x \in X$, cho $U$ là một lân cận mở của $x$, và cho $f : U \to Y$ là một cấu xạ thuộc lớp $C^r$. Ánh xạ
$$
x \mapsto j_x^{k'}(f) : U \to J^{k'}(X, Y)
$$
thuộc lớp $C^{r-k'}$ và jet cấp $k''$ của nó tại $x$ chỉ phụ thuộc vào $j_x^k(f)$. Do đó ta thu được một ánh xạ chính tắc
$$
\alpha : J^k(X, Y) \to J^{k''}(X, J^{k'}(X, Y))
$$
thuộc lớp $C^{r-k}$; nếu $K$ có đặc số không, thì nó là một phép nhúng.

12.3.9. Cho $X', Y'$ là các đa tạp thuộc lớp $C^r$, cho $f : X \to X'$ và $g : Y' \to Y$ là các cấu xạ, và cho $(x, y') \in X \times Y'$, $x' = f(x)$, $y = g(y')$. Nếu $u \in J_{x'}^k(X', Y')_{y'}$, đặt
$$
J_{x'}^k(f, g)_y(u) = j_y^k(g) \circ u \circ j_x^k(f).
$$
Do đó ta thu được một ánh xạ
$$
J^k(f, g) : J^k(X', Y') \times_{X'} X \to J^k(X, Y)
$$
thuộc lớp $C^{r-k}$.

12.3.10. Cho $A$ là một tập con compact của $X$. Cho $\mathscr{C}^k(X; Y)$ là tập hợp các ánh xạ thuộc lớp $C^k$ từ $X$ vào $Y$. Với mọi $f \in \mathscr{C}^k(X; Y)$, ánh xạ $j^k(f)|A$ thuộc tập hợp $\mathscr{C}(A; J^k(X, Y))$ các ánh xạ liên tục từ $A$ vào $J^k(X, Y)$. Do đó ta đã xác định một ánh xạ $\lambda$ từ $\mathscr{C}^k(X; Y)$ vào $\mathscr{C}(A; J^k(X, Y))$. Ảnh ngược bởi $\lambda$ của tôpô hội tụ compact trên $\mathscr{C}(A; J^k(X, Y))$ (TG, X, § 3, Định nghĩa 1) là một tôpô trên $\mathscr{C}^k(X; Y)$; nó được gọi là *tôpô hội tụ $C^k$ đều trên $A$*.

### 12.4. Khung và các phân thớ chính

12.4.1. Cho $j \in J^k(X, Y)$ và cho $x = s(j)$, $y = b(j)$. Ta nói rằng $j$ là *khả nghịch* nếu tồn tại $j' \in J_y^k(Y, X)_x$ sao cho $j' \circ j = j_x^k(\mathrm{Id}_X)$ và $j \circ j' = j_y^k(\mathrm{Id}_Y)$; khi đó jet $j'$ được xác định duy nhất; ta ký hiệu nó là $j^{-1}$. Nếu $k = 0$, mọi jet đều khả nghịch. Nếu $k \geqslant 1$, các điều kiện sau là tương đương:
a) $j$ khả nghịch;
b) ánh xạ $T(j) : T_x(X) \to T_y(Y)$ (cf. 12.3.4) là một đẳng cấu;
c) tồn tại một đẳng cấu $g$ lớp $C^r$ từ một lân cận mở của $x$ lên một lân cận mở của $y$, sao cho $j_x^k(g) = j$.

12.4.2. Cho $E$ là một không gian Banach. Ta ký hiệu $\mathbf{GL}^k(E)$ là tập hợp các jet cấp $k$ từ $E$ vào $E$ khả nghịch và có $0$ làm nguồn và đích; đó là một tập mở của $J_0^k(E, E)_0$. Được trang bị luật hợp thành của các jet và cấu trúc đa tạp cảm sinh bởi cấu trúc của không gian Banach $J_0^k(E, E)_0 = Q^k(E, E)$, nó là một đa tạp nhóm lớp $C^\omega$.

Ta có $\mathbf{GL}^0(E) = \{ e \}$. Nhóm $\mathbf{GL}^1(E)$ được đồng nhất, thông qua $T$, với nhóm $\mathbf{GL}(E)$ các tự đẳng cấu của $E$.

Nếu $k' \leqslant k$, ánh xạ $r^{k, k'} : \mathbf{GL}^k(E) \to \mathbf{GL}^{k'}(E)$ là một đồng cấu lớp $C^\omega$ và là một phép ngập toàn ánh. Ánh xạ $f \mapsto \mathrm{Id}_E + f$ là một đẳng cấu của các đa tạp nhóm từ $P_k(E, E)$ lên hạt nhân của $r^{k, k-1}$.

12.4.3. Cho E là một không gian Banach. Với mọi $x \in X$, một E-khung cấp k của X tại x được gọi là bất kỳ phần tử khả nghịch nào của $J_0^k(E, X)_x$. Tập hợp các E-khung cấp k của X là một đa tạp con mở $R^k(E, X)$ của $J_0^k(E, X)$; ánh xạ b có hạn chế của nó là một cấu xạ, vẫn ký hiệu là b, từ $R^k(E, X)$ vào X; tương tự, nếu $k' \leq k$, ta vẫn ký hiệu $r^{k, k'}$ là cấu xạ từ $R^k(E, X)$ vào $R^{k'}(E, X)$, hạn chế của ánh xạ $r^{k, k'}$ của 12.1.5.

12.4.4. Ta giả sử rằng X thuần túy kiểu E (5.1.7). Nhóm $GL^k(E)$ tác động bên phải trên $R^k(E, X)$ theo luật $(\rho, u) \mapsto \rho \circ u$ và bộ bốn $\lambda_X = (R^k(E, X), GL^k(E), X, b)$ là một phân thớ chính (6.2.1) với nhóm cấu trúc $GL^k(E)$, cơ sở X và lớp $C^{r-k}$.

Nếu $k' \leq k$, gọi H là hạt nhân của $r^{k, k'} : GL^k(E) \to GL^{k'}(E)$; bộ bốn $(R^k(E, X), H, R^{k'}(E, X), r^{k, k'})$ là một phân thớ chính lớp $C^{r-k}$.

Đa tạp $J^k(X, Y)$ được trang bị một cấu trúc của không gian sợi liên kết với $\lambda_X$ (6.5.1): sợi kiểu là $J_0^k(E, Y)$ trên đó $GL^k(E)$ tác động bên trái theo luật $(u, j) \mapsto j \circ u^{-1}$; ánh xạ khung $R^k(E, X) \times J_0^k(E, Y) \to J^k(X, Y)$ biến $(\rho, j)$ thành $j \circ \rho^{-1}$. Phép chiếu $J^k(X, Y) \to X$ tương ứng với cấu trúc không gian sợi liên kết này là s.

12.4.5. Cho F là một không gian Banach, và giả sử rằng Y thuần túy có kiểu F. Khi đó $J^k(X, Y)$ được trang bị một cấu trúc của không gian sợi liên kết với $\lambda_Y$: sợi kiểu là $J^k(X, F)_0$ trên đó $GL^k(F)$ tác động bên trái theo luật $(v, j) \mapsto v \circ j$; ánh xạ khung là $(\sigma, j) \mapsto \sigma \circ j$; phép chiếu $J^k(X, Y) \to Y$ là b.

12.4.6. Với các giả thiết là các giả thiết của 12.4.4 và 12.4.5, cho $\mu$ là phân thớ chính
$$
(R^k(E, X) \times R^k(F, Y), GL^k(E) \times GL^k(F), X \times Y, b \times b),
$$
tích của $\lambda_X$ và $\lambda_Y$. Khi đó $J^k(X, Y)$ được trang bị một cấu trúc của không gian sợi liên kết với $\mu$: sợi kiểu là $J_0^k(E, F)_0$ trên đó $GL^k(E) \times GL^k(F)$ tác động bên trái theo luật $((u, v), j) \mapsto v \circ j \circ u^{-1}$; ánh xạ khung là $((\rho, \sigma), j) \mapsto \sigma \circ j \circ \rho^{-1}$; phép chiếu $J^k(X, Y) \to X \times Y$ là $(s, b)$.

### 12.5. Các jet của các tiết diện

12.5.1. Cho $\pi : Y \to X$ là một phép chìm, cho $x \in X$, và cho $s \in J_x^k(X, Y)$. Ta nói rằng s là một jet của tiết diện (cấp k) của $\pi$ nếu s có dạng $j_x^k(f)$, trong đó f là một tiết diện lớp $C^r$ của $\pi$ phía trên một lân cận mở của x; điều kiện này tương đương với
$$
j_{b(s)}^k(\pi) \circ s = j_x^k(\mathrm{Id}_X).
$$
Ta ký hiệu bởi $P_x^k(\pi)$ (tương ứng $P^k(\pi)$) tập hợp các jet $s \in J_x^k(X, Y)$ (tương ứng $J^k(X, Y)$) là các jet của tiết diện của $\pi$; nó là một đa tạp lớp $C^{r-k}$ của $J^k(X, Y)$. Các ánh xạ
$$
s : P^k(\pi) \to X \quad \text{và} \quad b : P^k(\pi) \to Y
$$
là các phép chìm; nếu $\pi$ là một phân thớ, chúng là các phân thớ. Với $k = 0$, b là một đẳng cấu, nhờ đó ta đồng nhất $P^0(\pi)$ với Y.

Nếu $k' \leq k$, ánh xạ $r^{k, k'} : J^k(X, Y) \to J^{k'}(X, Y)$ áp dụng $P^k(\pi)$ vào $P^{k'}(\pi)$; ánh xạ từ $P^k(\pi)$ vào $P^{k'}(\pi)$ suy ra từ $r^{k, k'}$ là một phân thớ lớp $C^{r-k}$.

12.5.2. Cho $Z$ là một đa tạp lớp $C^r$; giả sử rằng $Y = X \times Z$ và đặt $\pi = \mathrm{pr}_1 : Y \to X$. Hạn chế của $J^k(\mathrm{Id}_X, \mathrm{pr}_2)$ (xem 12.3.9) lên $P^k(\pi)$ là một đẳng cấu của $P^k(\pi)$ lên $J^k(X, Z)$, qua đó ta đồng nhất hai đa tạp này.

12.5.3. Cho $Y'$ là một đa tạp lớp $C^r$, cho $\pi : Y \to X$ và $\pi' : Y' \to X$ là các phép chìm và cho $g : Y \to Y'$ là một cấu xạ sao cho $\pi' \circ g = \pi$. Ánh xạ $J^k(\mathrm{Id}_X, g)$ có hạn chế là một ánh xạ

$$
P^k(g) : P^k(\pi) \to P^k(\pi')
$$

có lớp $C^{r-k}$.

Cho $X'$ là một đa tạp lớp $C^r$, và cho $f : X' \to X$ là một cấu xạ; đặt $(Y', \pi') = f^*(Y, \pi)$, xem 5.11.5. Ánh xạ $J^k(f, \mathrm{Id}_Y)$ (xem 12.3.9) định nghĩa một ánh xạ lớp $C^{r-k}$ từ $f^*P^k(\pi)$ vào $P^k(\pi')$.

### 12.6. Tiết diện của các bó vectơ

12.6.1. Cho $E$ là một bó vectơ lớp $C^r$ có cơ sở $X$, và cho $\pi$ là phép chiếu của nó. Cho $c_0 = (U, \varphi, F_0)$ là một biểu đồ bó vectơ của $E$ và $c_1 = (U, \psi, F_1)$ là một biểu đồ của đa tạp $X$, với cùng miền $U$. Các biểu đồ này xác định một song ánh $\theta$ từ $P^k(\pi)|U$ lên $J^k(\psi(U), F_0) = \psi(U) \times F_0 \times Q^k(F_1, F_0)$, xem 12.2.2 và 12.3.1, do đó một biểu đồ bó vectơ

$$
d = (U, \theta, G), \quad \text{with} \quad G = F_0 \times Q^k(F_1, F_0) = \prod_{m=0}^k P_m(F_1; F_0)
$$

của $P^k(\pi)$. Các biểu đồ thu được như vậy lập thành một $C^{r-k}$-atlas bó vectơ, trang bị cho $P^k(\pi)$ cấu trúc của một bó vectơ lớp $C^{r-k}$, có cơ sở $X$. Bó vectơ này được ký hiệu là $P^k(E)$; cấu trúc đa tạp cơ sở là cấu trúc được định nghĩa trong 12.5.1.

Cho $U$ là một tập con mở của $X$, và cho $f \in \mathscr{S}_E^r(U)$ là một tiết diện lớp $C^r$ của $E$ trên $U$. Ánh xạ $j^k(f) : x \mapsto j_x^k(f)$ là một tiết diện lớp $C^{r-k}$ của $P^k(E)$ trên $U$. Ánh xạ $j^k : \mathscr{S}_E^r(U) \to \mathscr{S}_{P^k(E)}^{r-k}(U)$ là $K$-tuyến tính.

12.6.2. Nếu $F$ là một không gian Banach, phép nhận dạng (12.5.2) của $P^k(F_X)$ với $J^k(X, F)$ trang bị cho đa tạp sau một cấu trúc bó vectơ lớp $C^{r-k}$, với cơ sở $X$. Khi $F = K$, ta viết $P^k(X)$ thay cho $P^k(K_X)$.

#### Ví dụ {#var-2-s12-n6-exa-1 .statement}

Cho $X = K^n$, và ký hiệu $u_1, \ldots, u_n$ là các hàm tọa độ trên $K^n$; khi đó thớ $P^k_0(X)$ của $P^k(X)$ tại 0 có họ các jet cấp $k$ của các đơn thức $u_1^{m_1} \ldots u_n^{m_n}$ làm cơ sở, với $m_i \geqslant 0, \sum_{i=0}^n m_i \leqslant k$.

12.6.3. Cho $d$ là một số nguyên $\geqslant 0$, cho $E_1, \ldots, E_d, F$ là các bó vectơ lớp $C^r$ với cơ sở $X$, và cho $u : E_1 \times_X \cdots \times_X E_d \to F$ là một cấu xạ đa tuyến tính (7.3.1) lớp $C^r$. Khi đó tồn tại duy nhất một cấu xạ đa tuyến tính

$$
P^k(u) : P^k(E_1) \times_X \cdots \times_X P^k(E_d) \to P^k(F)
$$

sao cho

$$
P^k(u)(j^k(s_1), \ldots, j^k(s_d)) = j^k(u(s_1, \ldots, s_d))
$$

với mọi tập mở $U$ của $X$ và mọi dãy các tiết diện $s_i \in \mathscr{S}_{E_i}'(U)$ với $1 \leq i \leq d$.

Nếu $A$ là một bó đại số (7.3.2) với cơ sở $X$, cấu xạ từ $P^k(A) \times_X P^k(A)$ vào $P^k(A)$ cảm sinh bởi phép nhân $A \times_X A \to A$ làm cho $P^k(A)$ thành một bó đại số; nếu $A$ là một bó đại số kết hợp, $P^k(A)$ là một bó đại số kết hợp; nếu thêm vào đó, $M$ là một bó $A$-môđun (7.3.3), thì $P^k(M)$ là một bó $P^k(A)$-môđun. Đặc biệt, $P^k(X)$ là một *bó đại số kết hợp, giao hoán và có đơn vị*; nếu $E$ là một bó vectơ, $P^k(E)$ là một *bó $P^k(X)$-môđun*. Nếu $u : E \to F$ là một cấu xạ của các bó vectơ, thì $P^k(u) : P^k(E) \to P^k(F)$ là một $P^k(X)$-đồng cấu.

12.6.4. Nếu $E \xrightarrow{u} F \xrightarrow{v} G$ là một dãy khớp tách địa phương của các bó vectơ với cơ sở $X$, thì điều tương tự cũng đúng đối với dãy

$$
P^k(E) \to P^k(F) \to P^k(G)
$$

trong đó các đồng cấu được xét là $P^k(u)$ và $P^k(v)$.

12.6.5. Cho $k'$ và $k''$ là hai số nguyên dương có tổng bằng $k$, và cho $E$ là một bó vectơ lớp $C^r$ với cơ sở $X$. Cấu xạ

$$
\alpha : J^k(X, E) \to J^{k''}(X, J^{k'}(X, E)) \quad (\text{cf. } 12.3.8)
$$

cảm sinh một cấu xạ của các bó vectơ

$$
\beta : P^k(E) \to P^{k''}(P^{k'}(E))
$$

có lớp $C^{r-k}$. Nếu $U$ là một tập mở của $X$ và $f \in \mathscr{S}_E'(U)$, ta có

$$
\beta(j^{k}(f)) = j^{k''}(j^{k'}(f)).
$$

Khi $K$ có đặc số không, $\beta$ là một đẳng cấu của $P^k(E)$ lên một bó con vectơ của $P^{k''}(P^{k'}(E))$.

12.6.6. Cho $k'$ là một số nguyên sao cho $0 \leq k' \leq k$, và cho $E$ là một bó vectơ lớp $C^r$ với cơ sở $X$. Ánh xạ

$$
r^{k, k'} : P^k(E) \to P^{k'}(E)
$$

là một cấu xạ toàn ánh địa phương trực tiếp thuộc lớp $C^{r-k}$. Hạt nhân của nó $N^{k, k'}(E)$ gồm các jet tiết diện của E có tiếp xúc cấp $\geq k'$ với tiết diện không.

12.6.7 (*Hàm tử vectơ $P_m$*). Với ký hiệu của 7.6, 7.7, 7.8, đặt $I_+ = \{0\}, I_- = \{1\}$ và cho m là một số nguyên $\geq 0$. Nếu $\mathscr{V} = (V_0, V_1)$ là một cặp không gian Banach, ký hiệu $\tau_m(\mathscr{V})$ là không gian Banach $P_m(V_1; V_0)$ gồm các *đa thức liên tục thuần nhất* bậc m trên $V_1$ nhận giá trị trong $V_0$ (A.2). Tương tự, nếu $f = (f_0, f_1)$. trong đó $f_0 : V_0 \to V'_0$ và $f_1 : V'_1 \to V_1$ là các cấu xạ của các không gian Banach, ký hiệu $\tau_m(f)$ là cấu xạ $p \mapsto f_0 \circ p \circ f_1$ từ $P_m(V_1; V_0)$ vào $P_m(V'_1; V'_0)$. Như vậy ta thu được một *hàm tử* vectơ $\tau_m$ thuộc lớp $C^\omega$. Nếu $E_0$ và $E_1$ là hai bó vectơ có cơ sở $X$, ký hiệu $P_m(E_1; E_0)$ là bó vectơ suy ra từ $(E_0, E_1)$ bằng $\tau_m$ (7.6.2).

12.6.8. Ta tiếp tục sử dụng ký hiệu và các giả thiết của 12.6.1. Tồn tại duy nhất một cấu xạ của các bó vectơ

$$
\iota : P_k(T(X); E) \to P^k(E) \quad (\text{cf. } 12.6.6),
$$

sao cho, với mọi biểu đồ vectơ $c_0 = (U, \varphi, F_0)$ của $E$ và biểu đồ $c_1 = (U, \psi, F_1)$ của $X$, biểu đồ sau là giao hoán:

$$
\begin{array}{ccc}
P_k(T(X), E)|U & \xrightarrow{\iota|U} & P^k(E)|U \\
\downarrow \eta & & \downarrow \theta \\
U \times P_k(F_1; F_0) & \xrightarrow{i} & U \times \prod_{m=0}^k P_m(F_1; F_0)
\end{array}
$$

trong đó: 1) $\iota|U$ là hạn chế của $\iota$ lên $P_k(T(X), E)|U$;
   2) $\theta$ là song ánh được định nghĩa trong 12.6.1;
   3) $i$ là ánh xạ $(u, p) \mapsto (u, 0, \ldots, 0, p)$;
   4) $\eta$ được suy ra, bằng hàm tử vectơ $\tau_k$, từ biểu đồ vectơ $c'_1$ của $T(X)$ (cf. 8.1.1) và biểu đồ vectơ $c_0$ của $E$.

Cấu xạ $\iota$ là một đẳng cấu của $P_k(T(X); E)$ lên bó con vectơ $N^{k, k-1}(E)$ của $P^k(E)$ (cf. 12.6.6); dãy

$$
0 \to P_k(T(X); E) \xrightarrow{\iota} P^k(E) \xrightarrow{\tau^{k, k-1}} P^{k-1}(E) \to 0
$$

là một dãy khớp địa phương trực tiếp của các bó vectơ.

Nói chung, đặt $N_0 = P^k(E)$, $N_m = N^{k, m-1}(E)$ với $m \geq 1$, sao cho các $N_m$ lập thành một dãy giảm các bó con vectơ của $P^k(E)$:

$$
P^k(E) = N_0 \supset N_1 \supset \cdots \supset N_k \supset N_{k+1} = 0.
$$

Với $0 \leq m \leq k$, phép chiếu $r^{k, m} : P^k(E) \to P^m(E)$ xác định một đẳng cấu của $N_m/N_{m+1}$ lên $N^{m, m-1}(E)$; được xem như trong ánh sáng của những điều vừa nói, ta thu được các đẳng cấu

$$
\iota_m : N_m/N_{m+1} \to P_m(T(X); E) \quad (0 \leq m \leq k).
$$

Đặc biệt, $N_0/N_1 \simeq E$ và $N_1/N_2 \simeq \mathscr{L}(T(X); E)$. Với $k = 1$, điều này cho một dãy khớp:

$$
0 \to \mathscr{L}(T(X); E) \to P^1(E) \to E \to 0.
$$

### 12.7. Làm yếu cấu trúc

Giả sử $K = \mathbf{R}$. Cho $r' \in N_k$ với $k \leq r' \leq r$ và cho $X'$ và $Y'$ là các đa tạp lớp $C^{r'}$ thu được từ $X$ và $Y$ bằng cách làm yếu cấu trúc (5.13.1). Cho $x \in X$ và $j \in J_x^k(X, Y)$; cho $U$ là một tập con mở của $X$ chứa $x$ và $f$ là một ánh xạ lớp $C^k$ từ $U$ vào $Y$, sao cho $j_x^k(f) = j$. Xét $f$ như một mầm của cấu xạ từ X' vào Y'; jet của nó $j' \in J_x^k(X', Y')$ chỉ phụ thuộc vào $j$. Ánh xạ $j \mapsto j'$ là một đẳng cấu lớp $C^{r'-k}$ từ $J^k(X, Y)$ lên $J^k(X', Y')$; nó cho phép ta đồng nhất $J^k(X', Y')$ với đa tạp lớp $C^{r'-k}$ suy ra từ đa tạp $J^k(X, Y)$ lớp $C^{r-k}$ bằng cách làm yếu cấu trúc. Một kết quả tương tự áp dụng cho các đa tạp $P^k(\pi)$ và $P^k(E)$ của Nos. 12.5 và 12.6.

[^1]: Khi $k = r$ (điều này chỉ có thể xảy ra nếu $K = \mathbf{R}$), $J^k(X, Y)$ được trang bị một cấu trúc của *đa tạp tôpô* (xem *Quy ước và Ký hiệu*) và các cấu xạ và các phép phân thớ được xét dưới đây phải được hiểu theo nghĩa thuần túy tôpô (xem chú thích chân trang của §6).
