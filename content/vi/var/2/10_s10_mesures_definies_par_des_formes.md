---
book: var
book_title: Variétés différentielles et analytiques
chapter: "2"
chapter_title: VARIÉTÉS DIFFÉRENTIELLES ET ANALYTIQUES, FASCICULE DE RÉSULTATS
section: 10
section_title: Mesures définies par des formes différentielles
lang: vi
source: var-fr
pdf_pages: 0126-0135
extraction: ocr
subsections:
    - "no": 1
      title: Mesure module d’une forme différentielle
      page: 0
      pdf_page: 126
    - "no": 2
      title: Orientations
      page: 0
      pdf_page: 128
    - "no": 3
      title: Formes différentielles M-tordues
      page: 0
      pdf_page: 131
    - "no": 4
      title: Mesure associée à une forme différentielle tordue
      page: 0
      pdf_page: 132
statements: 0
exercises: 0
content_sha256: 2731900b5dbe7b41f574c6fda9c3fa86616200b86bbec611eb9f2e62fcfb4d83
translated_from: content/en-mt/var/2/10_s10_mesures_definies_par_des_formes.md
source_lang: en-mt
translation_method: machine
source_content_sha256: 48948108d489270e2fea55f10b68791137abacd00a974022c223abd1f8be7413
translation_model: gpt-5-6
translation_run: translate-vi-433f3d94
glossary_version: 34
glossary_terms_sha256: 4cc69212ef75861641a428506c27c75d3333acd7f92a42616c6489212ccddf4d
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 10. Các độ đo được xác định bởi các dạng vi phân

Trong đoạn này, giả sử rằng $K$ là compact địa phương. Bắt đầu từ No. 10.2, giả sử rằng $K=\mathbf{R}$. Trong các No. 10.1 và 10.4, mọi đa tạp được xét đều được giả sử là hữu hạn chiều địa phương; khi chúng được phân ly, chúng là compact địa phương.

### 10.1. Độ đo môđun của một dạng vi phân

**Ký hiệu.** — Ta ký hiệu bởi $\mu$ một độ đo Haar (INT, VII, § 1, No. 2) trên nhóm cộng của $K$. Ta ký hiệu bởi $\mu^{\otimes n}$ độ đo $\mu\otimes\cdots\otimes\mu$ trên $K^n$ và bởi $\mu^{\otimes n}_U$ hạn chế của nó lên một tập con mở $U$ của $K^n$. Với $a\in K$, ta ký hiệu bởi $\operatorname{mod}(a)$ môđun của $a$ (INT, VII, § 1, No. 10 và AC, VI, § 9, No. 1). Nếu $K=\mathbf{R}$, ta có $\operatorname{mod}(a)=|a|$; nếu $K=\mathbf{C}$, ta có $\operatorname{mod}(a)=|a|^2$; nếu $K$ là siêu mêtric, ta có $\operatorname{mod}(a)=q^{-\nu(a)}$, trong đó $q$ chỉ số các phần tử của trường thặng dư của $K$ và $\nu$ là định giá đã nêu của $K$ (AC, VI, § 9, No. 1, prop. 1).

### 10.1.1. Cho $U$ và $V$ là các tập con mở của $K^n$, và cho $f:U\to V$ là một ánh xạ thuộc lớp $C^r$, với $r\in\mathbf{N}$. Cho $x\in U$; Jacobi của $f$ tại $x$, ký hiệu là $\operatorname{Jac}_x(f)$, được gọi là định thức của ánh xạ tuyến tính $Df(x)$ dẫn xuất từ $f$ tại $x$. Ta ký hiệu bởi $\operatorname{Jac}(f)$ hàm $x\mapsto\operatorname{Jac}_x(f)$; hàm $\operatorname{mod}(\operatorname{Jac}(f))$ là một hàm liên tục trong $U$ có các giá trị thực dương.

### 10.1.2 (« Thay đổi biến trong các tích phân »). Dưới các giả thiết của 10.1.1, giả sử rằng $f$ là một đẳng cấu thuộc lớp $C^r$ của đa tạp $U$ lên đa tạp $V$. Khi đó ảnh bởi $f$ của độ đo $\operatorname{mod}(\operatorname{Jac}(f))\mu^{\otimes n}_U$ là $\mu^{\otimes n}_V$; với mọi hàm liên tục có giá compact $\varphi:V\to\mathbf{C}$, ta có

$$
\int_V \varphi(y)\mu^{\otimes n}(y)=\int_U \varphi(f(x)).\operatorname{mod}(\operatorname{Jac}_x(f))\mu^{\otimes n}(x).
$$

### 10.1.3. Cho $X$ là một đa tạp thuộc lớp $C^r$, và cho $A$ là một tập con của $X$. Ta nói rằng $A$ là không đáng kể địa phương nếu, với mọi biểu đồ $(U,\varphi,K^n)$ của đa tạp $X$, tập hợp $\varphi(A\cap U)$ là $\mu^{\otimes n}$-không đáng kể (INT, IV, § 2, No. 2); điều kiện này không phụ thuộc vào lựa chọn $\mu$, và chỉ cần kiểm tra nó đối với một họ các biểu đồ mà miền của chúng phủ $A$. Mọi tập hợp được chứa trong hợp của một họ đếm được các tập không đáng kể địa phương đều là không đáng kể địa phương.

Ví dụ

a) Mọi đa tạp con của X có đối chiều $\geq 1$ tại mọi điểm (tức là có phần trong rỗng) đều không đáng kể địa phương.

b) Cho g là một hàm thuộc lớp $C^r$ trên X, và cho $A_g$ là tập hợp các điểm $x \in X$ sao cho $g(x) = 0$; giả sử rằng phần trong của $A_g$ là rỗng, và rằng $r = \omega$; khi đó $A_g$ là không đáng kể địa phương.

c) Cho $f : Y \to X$ là một cấu xạ của các đa tạp thuộc lớp $C^r$, đa tạp Y là một hợp đếm được của các tập con compact. Giả sử rằng ta có $\dim_y Y \leq \dim_{f(y)} X$ với mọi $y \in Y$. Ảnh bởi $f$ của mọi tập con không đáng kể địa phương của Y là một tập con không đáng kể địa phương của X. Điều tương tự cũng đúng đối với ảnh bởi $f$ của tập hợp các điểm tại đó $f$ không étale ("định lý thứ nhất của Sard"); đặc biệt, nếu $\dim_y Y < \dim_{f(y)} X$ với mọi $y \in Y, f(Y)$ là một tập con không đáng kể địa phương của X.

d) Giả sử K có đặc số không. Cho $f : Y \to X$ là một cấu xạ của các đa tạp thuộc lớp $C^r$ ($r \in \mathbf{N}_K, r \geq \infty$), Y là một hợp đếm được của các tập con compact. Cho C là tập hợp các điểm của Y tại đó $f$ không là một phép chìm ("các điểm tới hạn"). Khi đó $f(C)$ là một tập con không đáng kể địa phương của X ("định lý thứ hai của Sard").[^1]

10.1.4. Cho X là một đa tạp paracompact thuộc lớp $C^r$. Tồn tại trên X một lớp M các độ đo tương đương (INT, V, § 5, No. 6) và chỉ một lớp như vậy sao cho, với mọi $\nu \in M$ và mọi biểu đồ $c = (U, \varphi, K^n)$ của X, ảnh bởi $\varphi$ của hạn chế của $\nu$ lên U là tương đương với $\mu_{\varphi(U)}^{\otimes n}$. Lớp M được gọi là lớp độ đo chính tắc trên X. Đối với một tập con A của X, để A là không đáng kể địa phương (10.1.3), điều kiện cần và đủ là nó không đáng kể địa phương (INT, IV, § 2, No. 2) đối với một (tương ứng mọi) độ đo $\nu \in M$.

Nếu $K = \mathbf{R}$ và $r \neq \omega$ (tương ứng $K = \mathbf{R}$ hoặc $C$ và $r = \omega$, tương ứng K là ultrametric), tồn tại $\nu \in M$ sao cho, đối với mọi biểu đồ $c = (U, \varphi, K^n)$ của X, mật độ của $\varphi(\nu_U)$ đối với $\mu_{\varphi(U)}^{\otimes n}$ ở mọi nơi $> 0$ và thuộc lớp $C^{r-1}$ (tương ứng thuộc lớp $C^\infty$, tương ứng hằng địa phương). Nếu $\nu$ và $\nu'$ là hai độ đo như vậy, mật độ của $\nu'$ đối với $\nu$ ở mọi nơi $> 0$ và thuộc lớp $C^{r-1}$ (tương ứng thuộc lớp $C^\infty$, tương ứng hằng địa phương).

10.1.5. Cho $X$ là một đa tạp thuộc lớp $C^r$; $T'(X)$ là bó đối tiếp xúc của X (8.2.2) và đặt $\Omega = \det(T'(X))$ (7.9.9). Bó vectơ $\Omega$ có hạng 1 tại mỗi điểm; khi X thuần nhất về chiều $n$, nó được đồng nhất với bó vectơ $\mathrm{Alt}^n(T(X); K_X)$. Cho $\omega$ là một tiết diện của $\Omega$ trên X; người ta nói, do lạm dụng ngôn ngữ, rằng $\omega$ là một dạng vi phân có bậc cực đại trên X. Cho $c = (U, \varphi, K^n)$ là một bảng tọa độ của X; ký hiệu $u^1, \ldots, u^n$ là các hàm tọa độ trên $K^n$. Tồn tại duy nhất một hàm $f_c$ trên $\varphi(U)$ sao cho $\omega|U = \varphi^*(f_c du^1 \wedge \cdots \wedge du^n)$. Người ta nói rằng $\omega$ có môđun khả tích địa phương nếu, đối với mọi bảng tọa độ $c = (U, \varphi, K^n)$ của X, hàm thực $\mathrm{mod}(f_c) : \varphi(U) \to \mathbf{R}$ là khả tích địa phương đối với $\mu_{\varphi(U)}^{\otimes n}$ (INT, IV, § 4, No. 1); chỉ cần kiểm tra tính chất này đối với các bảng tọa độ của một atlat của X. Nếu $\omega$ liên tục, và đặc biệt nếu $\omega$ thuộc lớp $C^s$, với $s \in \mathbf{N}_K, s \leq r - 1$, thì $\omega$ có môđun khả tích địa phương.

10.1.6 (“Độ đo dương xác định bởi một dạng vi phân có bậc cực đại”). Giữ lại các ký hiệu của 10.1.5 và giả sử thêm rằng X là tách được và rằng $\omega$ có môđun khả tích địa phương. Nếu $c = (U, \varphi, K^n)$ là một bảng tọa độ của X, ký hiệu $\nu_c$ là độ đo trên $\varphi(U)$ là tích của độ đo $\mu_{\varphi(U)}^{\otimes n}$ với hàm mod$(f_c)$ (INT, V, § 5, No. 2, định nghĩa 2) và gọi $\alpha_c$ là ảnh của $\nu_c$ qua $\varphi^{-1}$. Tồn tại duy nhất trên X một độ đo $\alpha$ sao cho, đối với mọi bảng tọa độ $c = (U, \varphi, K^n)$ của X, hạn chế của $\alpha$ trên U bằng $\alpha_c$. Người ta nói rằng độ đo $\alpha$ là môđun của $\omega$ và ký hiệu nó là mod$(\omega)_\mu$. Đây là một độ đo dương. Khi $K = \mathbf{R}$ và $\mu$ là độ đo Lebesgue, người ta viết $|\omega|$ thay cho mod$(\omega)_\mu$.

Nếu X thuần nhất về chiều $n$, và nếu $a$ là một số thực $> 0$, ta có $\mathrm{mod}(\omega)_{a\mu} = a^n \mathrm{mod}(\omega)_\mu$.

Cho A là một tập con của X. Để A là không đáng kể địa phương (10.1.3), điều kiện cần và đủ là, đối với mọi tập mở U của X và mọi dạng vi phân có bậc cực đại $\omega$ trên U có môđun khả tích địa phương, tập $A \cap U$ là không đáng kể địa phương đối với độ đo $\mathrm{mod}(\omega)_\mu$.

Giả sử thêm rằng X là không gian paracompact và cho $\nu$ là một độ đo trên X thuộc lớp tương đương chính tắc M (10.1.4). Độ đo $\mathrm{mod}(\omega)_\mu$ dựa trên $\nu$ (INT, V, § 5, No. 2, định nghĩa 2). Để $\mathrm{mod}(\omega)_\mu$ thuộc M, điều kiện cần và đủ là tập hợp các $x \in X$ sao cho $\omega(x) = 0$ là không đáng kể địa phương.

10.1.7. Ví dụ. — Cho G là một nhóm Lie trên K, có số chiều hữu hạn $n$, và cho $\omega$ là một dạng vi phân bậc $n$ trên G, bất biến qua các phép tịnh tiến trái, và khác không. Độ đo tương ứng $\mathrm{mod}(\omega)_\mu$ khi đó là một độ đo Haar trái trên nhóm compact địa phương G.

Khi G là nhóm nhân $K^*$, ta có thể lấy $\omega$ là dạng $dx/x$, và ta có $\mathrm{mod}(\omega)_\mu = (\mathrm{mod})^{-1}.\mu$, cf. INT, VII, § 1, No. 10, mệnh đề 14.

### 10.2. Định hướng

Ta nhắc lại rằng, trong số này và các số tiếp theo, ta giả sử rằng $K = \mathbf{R}$.

10.2.1 (« Định hướng của một không gian vectơ thực »). Cho E là một không gian vectơ thực có số chiều hữu hạn $n$. Ta ký hiệu bởi Or(E) tập hợp các định hướng của E (A, VI, § 2, No. 7); các phần tử của Or(E) là hai nửa đường thẳng đóng của không gian vectơ $\det(E) = \bigwedge^n E$. Nếu $\xi \in \mathrm{Or}(E)$, phần tử kia của Or(E) được gọi là định hướng đối với $\xi$, và ký hiệu $-\xi$.

Cho $0 \to E' \xrightarrow{\alpha} E \xrightarrow{\beta} E'' \to 0$ là một dãy khớp của các không gian vectơ (thực) có số chiều hữu hạn; đặt $p' = \dim E',\ p'' = \dim E''$ và cho $\xi'$ (tương ứng $\xi''$) là một định hướng của E' (tương ứng E''). Ta ký hiệu bởi $\xi'\xi''$ (tương ứng $\xi''\xi'$) định hướng của E chứa một vectơ khác không $(p' + p'')$-chiều $u' \wedge u''$ (tương ứng $u'' \wedge u'$), trong đó $u'$ là ảnh qua $\wedge^\alpha$ của một $p'$-vectơ của E' thuộc $\xi'$ và trong đó $u''$ là một $p''$-vectơ của E có ảnh qua $\wedge^\beta$ thuộc $\xi''$ (cf. A, VI,§ 2, No. 7). Nếu $E = E' \times E''$, $\alpha$ và $\beta$ là các ánh xạ chính tắc, ta nói rằng $\xi'\xi''$ là tích của định hướng $\xi'$ và của định hướng $\xi''$.

10.2.2 (« Không gian các định hướng »). Cho B là một không gian tôpô và M là một bó vectơ thực với cơ sở B (theo nghĩa tôpô — cf. § 6, p. 61, Chú ý (*)), có hạng hữu hạn

(7.1.6). Cho $\mathrm{Or}_M$ là hợp rời nhau của các $\mathrm{Or}(M_b)$, với $b \in B$, và cho $\pi : \mathrm{Or}_M \to B$ là ánh xạ sao cho $\pi(\mathrm{Or}(M_b)) = \{b\}$. Trên $\mathrm{Or}_M$ tồn tại một và chỉ một cấu trúc của không gian tôpô sao cho:

a) $\pi$ là liên tục.

b) Nếu $s$ là một tiết diện liên tục và khác không tại mọi điểm của $\det(M)$ trên một tập mở $U$ của $B$, và nếu $\xi(s(b))$ là định hướng của $M_b$ được xác định bởi phần tử $s(b)$ của $\det(M_b)$, ánh xạ $b \mapsto \xi(s(b))$ của $U$ vào $\mathrm{Or}_M$ là liên tục.

Không gian $\mathrm{Or}_M$ được gọi là không gian các định hướng của $M$. Nhóm $\{\pm 1\}$ tác động trên $\mathrm{Or}_M$ bởi $\xi \mapsto \pm \xi$ (10.2.1). Bộ bốn $(\mathrm{Or}_M, \{\pm 1\}, B, \pi)$ là một phân thớ chính (6.2.1) với cơ sở $B$ và nhóm cấu trúc $\{\pm 1\}$; phép chiếu $\pi : \mathrm{Or}_M \to B$ xác định một đẳng cấu của $\mathrm{Or}_M/\{\pm 1\}$ lên $B$, cf. No. 6.2.

Khi $B$ được trang bị một cấu trúc đa tạp, $\mathrm{Or}_M$ được trang bị cấu trúc ảnh ngược của cấu trúc đó của $B$ bởi $\pi$ (5.8.1); phân thớ được xác định ở trên khi đó là một phân thớ của các đa tạp và cấu xạ $\pi$ là étale.

10.2.3. Giữ lại các giả thiết của 10.2.2. Một định hướng của bó vectơ $M$ được gọi là một tiết diện liên tục $\xi : B \to \mathrm{Or}_M$ của phép chiếu $\pi : \mathrm{Or}_M \to B$. Ta nói rằng $M$ là định hướng được nếu nó có một định hướng; điều này tương đương với việc nói rằng bó $\mathrm{Or}_M$ là tầm thường hóa được, tức là đẳng cấu với $B \times \{\pm 1\}$. Nếu $B$ liên thông và khác rỗng, mọi bó vectơ định hướng được với cơ sở $B$ đều có hai định hướng, đối nhau.

Khi $M$ được thu gọn về $0$, bó $\det(M)$ là bó tầm thường $R_B$ và $\mathrm{Or}_M$ được đồng nhất với $\mathrm{Or}(R) \times B$; bó $M$ có một định hướng chính tắc, tương ứng với nửa đường thẳng dương của $R$.

10.2.4 (« Định hướng của một đa tạp »). Cho $X$ là một đa tạp hữu hạn chiều địa phương trên $R$ thuộc lớp $C^r$, và cho $T(X)$ là bó tiếp xúc của nó. Ta ký hiệu $\tilde{X}$ là đa tạp $\mathrm{Or}_{T(X)}$; nhóm $\{\pm 1\}$ tác động đúng và tự do trên $\tilde{X}$ và $\tilde{X}/\{\pm 1\}$ được đồng nhất với $X$; các thớ của phép chiếu $\pi : \tilde{X} \to X$ là các tập hợp $\mathrm{Or}(T_x(X))$, với $x \in X$. Một định hướng của $X$ được gọi là một định hướng của bó $T(X)$, nói cách khác là một tiết diện liên tục của bó $\tilde{X}$; một tiết diện như vậy thuộc lớp $C^r$. Ta nói rằng $X$ là định hướng được nếu nó có một định hướng. Mọi đa tạp có chiều không đều định hướng được và có một định hướng chính tắc (10.2.3).

Cho $\xi \in \tilde{X}$ và cho $x = \pi(\xi)$ là ảnh của nó trong $X$; ánh xạ $T_\xi(\pi) : T_\xi(\tilde{X}) \to T_x(X)$ là một đẳng cấu; nó cho phép đồng nhất $\xi$ với một phần tử $\tilde{\xi}$ của $\mathrm{Or}(T_\xi(\tilde{X}))$. Ánh xạ $\xi \mapsto \tilde{\xi}$ là một định hướng của $\tilde{X}$, được gọi là chính tắc; đặc biệt, $\tilde{X}$ là định hướng được.

10.2.5 (« Định hướng của một cấu xạ »). Cho $X$ và $Y$ là hai đa tạp hữu hạn chiều địa phương và cho $f : X \to Y$ là một cấu xạ của các đa tạp. Một định hướng của $f$ được gọi là một cấu xạ $\tilde{f} : \tilde{X} \to \tilde{Y}$ làm cho biểu đồ sau giao hoán

$$
\begin{array}{ccc}
\tilde{X} & \xrightarrow{\tilde{f}} & \tilde{Y} \\
| & & | \\
X & \xrightarrow{f} & Y
\end{array}
$$

và tương thích với tác động của nhóm $\{\pm 1\}$.

Nếu $\tilde{f}$ là một định hướng của $f$ và nếu $\eta$ là một định hướng của $Y$, thì tồn tại duy nhất một định hướng $\xi$ của $X$ sao cho biểu đồ

$$
\begin{array}{ccc}
\tilde{X} & \xrightarrow{\tilde{f}} & \tilde{Y} \\
\xi \downarrow & & \eta \downarrow \\
X & \xrightarrow{f} & Y
\end{array}
$$

là giao hoán. Ta nói rằng $\xi$ được liên kết với $\eta$ bởi $\tilde{f}$.

**Ví dụ**

a) Nếu $Y$ thu về một điểm, một định hướng của $f$ tương đương với một định hướng của $X$.

b) Giả sử rằng $f$ là étale. Với mọi $x \in X$, ánh xạ $T_x(f)$ là một đẳng cấu từ $T_x(X)$ lên $T_{f(x)}(Y)$, và xác định (bởi phép chuyển cấu trúc) một song ánh

$$
\tilde{f}_x : \mathrm{Or}(T_x(X)) \to \mathrm{Or}(T_{f(x)}(Y)).
$$

Họ các $\tilde{f}_x$ xác định một định hướng $\tilde{f} : \tilde{X} \to \tilde{Y}$ của $f$, được gọi là chính tắc.

c) Nói chung hơn, giả sử rằng $f$ là một cấu xạ hạ, và cho $\alpha$ là một định hướng của bó $T(X/Y)$ (8.1.3). Cho $x \in X$ và $\xi$ là một định hướng của $T_x(X)$. Đặt $y = f(x)$; ta có một dãy khớp (8.1.3)

$$
0 \to T_x(X/Y) \to T_x(X) \xrightarrow{T_x(f)} T_y(Y) \to 0
$$

và do đó tồn tại duy nhất một định hướng $\tilde{f}_\alpha(\xi)$ của $T_y(Y)$ sao cho $\xi = \tilde{f}_\alpha(\xi)\alpha(x)$ (10.2.1). Ánh xạ $\tilde{f}_\alpha : \tilde{X} \to \tilde{Y}$ là một định hướng của $f$, được gọi là liên kết với $\alpha$. Ánh xạ $\alpha \mapsto \tilde{f}_\alpha$ là một song ánh của tập hợp các định hướng của $T(X/Y)$ lên tập hợp các định hướng của $f$.

d) Nếu $f : X \to Y$ là một phép nhúng, các định hướng của $f$ tương ứng với các định hướng của bó pháp tuyến của $f$.

10.2.6 (« Định hướng của một tích »). Cho $X_1$ (tương ứng $X_2$) là một đa tạp hữu hạn chiều địa phương và $\xi_1$ (tương ứng $\xi_2$) là một định hướng của $X_1$ (tương ứng $X_2$). Đặt $X = X_1 \times X_2$. Ánh xạ $(x_1, x_2) \mapsto \xi_1(x_1)\xi_2(x_2)$ (10.2.1) là một định hướng của $X_1 \times X_2$, được gọi là *tích* của các định hướng $\xi_1$ và $\xi_2$, và được ký hiệu bởi $\xi_1 \xi_2$, hoặc $\xi_1 \otimes \xi_2$.

Giả sử rằng $X_i$ ($i = 1, 2$) thuần túy có chiều $n_i$. Đẳng cấu chính tắc $X_1 \times X_2 \to X_2 \times X_1$ biến $\xi_1 \otimes \xi_2$ thành $\xi_2 \otimes \xi_1$ (tương ứng thành $-\xi_2 \otimes \xi_1$) nếu một trong các $n_i$ là chẵn (tương ứng nếu $n_1$ và $n_2$ là lẻ).

10.2.7 (« Trường hợp phức »). Cho $F$ là một không gian vectơ phức hữu hạn chiều và cho $F_\mathbf{R}$ là không gian vectơ thực nền. Cho $\{e_1, \ldots, e_m\}$ là một cơ sở của $F$; khi đó $\{e_1, ie_1, e_2, ie_2, \ldots, e_m, ie_m\}$ là một cơ sở của $F_\mathbf{R}$ và định hướng của $F_\mathbf{R}$ được xác định bởi $2m$-vectơ

$$
e_1 \wedge ie_1 \wedge e_2 \wedge ie_2 \wedge \cdots \wedge e_m \wedge ie_m
$$

không phụ thuộc vào sự lựa chọn cơ sở $\{e_1, \ldots, e_m\}$ của $F$; định hướng này được gọi là *định hướng của $F_\mathbf{R}$* được xác định *bởi cấu trúc phức đã cho*. Nếu $F$ là tổng trực tiếp của hai không gian con $G$ và $H$, thì định hướng của $F_\mathbf{R} = G_\mathbf{R} \oplus H_\mathbf{R}$ là tích của các định hướng của $G_\mathbf{R}$ và $H_\mathbf{R}$.

Cho X là một đa tạp thực hữu hạn chiều địa phương, được trang bị một cấu trúc phức gần đúng (8.8.3). Với mọi $x \in X$, cho $\xi(x)$ là định hướng của $T_x(X)$ được xác định bởi cấu trúc phức của nó. Ánh xạ $x \mapsto \xi(x)$ là một định hướng của X, được gọi là định hướng được xác định bởi cấu trúc phức gần đúng. Đặc biệt, ta sẽ trang bị cho đa tạp giải tích thực X nằm dưới một đa tạp giải tích phức $X^c$, hữu hạn chiều địa phương, định hướng được xác định bởi cấu trúc phức gần đúng liên kết (8.8.6). Nếu cấu trúc đa tạp giải tích phức đã cho trên X được thay thế bởi cấu trúc liên hợp của nó (5.4.12.b)), thì định hướng này được nhân với hàm $x \mapsto (-1)^{\dim_{\mathbf{R}} X^c}$.

10.2.8. Ví dụ

a) Cho E là một không gian vectơ thực hữu hạn chiều. Đa tạp giải tích thực được xác định bởi E (5.2.2) là định hướng được. Chính xác hơn, ánh xạ $\xi \mapsto \xi(0)$ là một song ánh từ tập hợp các định hướng của đa tạp này lên Or(E).

Đặc biệt, đa tạp $\mathbf{R}^n$ có một định hướng chính tắc $\xi^n$ được xác định bởi nửa đường thẳng $\mathbf{R}_+ e_1 \wedge \cdots \wedge e_n$ của Or($\mathbf{R}^n$).

(b) Cho $X$ là một *mặt cầu* có tâm 0 và bán kính $> 0$ trong $\mathbf{R}^n$; nó là một đa tạp con của $\mathbf{R}^n$. Với mọi $x \in X$, không gian $T_x(\mathbf{R}^n) = \mathbf{R}^n$ là tổng trực tiếp của đường thẳng phải Rx và siêu phẳng $T_x(X)$. Gọi $\eta_x$ là định hướng $\mathbf{R}_+ x$ của Rx (“pháp tuyến hướng ra ngoài”) và gọi $\xi_x$ là định hướng duy nhất của $T_x(X)$ sao cho tích của $\eta_x$ và $\xi_x$ là định hướng $\xi^n$ của $\mathbf{R}^n$. Ánh xạ $x \mapsto \xi_x$ là một định hướng của $X$, được gọi là chính tắc.

(c) Cho $X$ là một đa tạp liên thông, và cho $G$ là một nhóm rời rạc tác động đúng và tự do trên $X$. Để $X/G$ là định hướng được, điều kiện cần và đủ là $X$ là định hướng được và tác động của $G$ trên tập hợp các định hướng của $X$ là tầm thường.

(d) *Không gian xạ ảnh thực* $P_{n-1}(\mathbf{R})$ được đồng nhất với thương của mặt cầu $S_{n-1}$ theo nhóm $\{ \pm 1 \}$ tác động bởi $x \mapsto \pm x$; nó là định hướng được nếu $n$ là chẵn, và không định hướng được nếu $n$ là lẻ.

(e) Mọi thương của một nhóm Lie theo một nhóm con Lie *liên thông* đều là định hướng được.

### 10.3. Các dạng vi phân M-xoắn

10.3.1. Cho $X$ là một đa tạp thực thuộc lớp $C^r$, và cho $M$ là một bó vectơ với cơ sở $X$, hạng hữu hạn và thuộc lớp $C^k$, với $0 \leq k \leq r$. Gọi $\lambda_M = (\mathrm{Or}_M, \{ \pm 1 \}, X, \pi)$ là phân thớ chính liên kết với đa tạp các định hướng của $M$ (10.2.2). Cho nhóm cấu trúc $\{ \pm 1 \}$ tác động trên $\mathbf{R}$ bằng phép nhân. Ký hiệu $\tilde{R}_M$ là bó sợi liên kết với $\lambda_M$ có sợi điển hình $\mathbf{R}$ (được trang bị luật của phép toán đã định nghĩa ở trên) (6.5.1); nó được trang bị (7.10.2) một cấu trúc bó vectơ với cơ sở $X$, hạng 1 và thuộc lớp $C^k$; nó được gọi là *bó các vô hướng M-xoắn*.

10.3.2. Ta có một biểu đồ giao hoán:

$$
\begin{array}{ccc}
\mathrm{Or}_M \times \mathbf{R} & \xrightarrow{\rho} & \tilde{R}_M \\
\downarrow \mathrm{pr}_1 & & \downarrow p \\
\mathrm{Or}_M & \xrightarrow{\varphi} & X
\end{array}
$$

trong đó $p$ là phép chiếu chính tắc của $\tilde{\mathbf{R}}_M$ lên $X$, $\rho$ là ánh xạ khung (6.5.1) của $\tilde{\mathbf{R}}_M$ và $\varphi(\xi) = \rho(\xi, 1)$ với $\xi \in \mathrm{Or}_M$. Đặc biệt, ảnh ngược của bó $\tilde{\mathbf{R}}_M$ qua $\pi$ được đồng nhất với bó tầm thường $\mathrm{Or}_M \times \mathbf{R}$. Một phần tử $\xi$ của $\mathrm{Or}_M$ cũng được đồng nhất với ảnh của nó trong $\tilde{\mathbf{R}}_M$ qua $\varphi$; với quy ước này, ta có $\rho(\xi, a) = a\xi$ với mọi $(\xi, a) \in \mathrm{Or}_M \times \mathbf{R}$; ta có $a\xi = b\eta$ khi và chỉ khi tồn tại $e \in \{ \pm 1 \}$ sao cho $b = ea$ và $\eta = e\xi$. Một định hướng $\xi$ của $M$ do đó xác định một tiết diện $x \mapsto \xi(x)$ của $\tilde{\mathbf{R}}_M$.

Tồn tại duy nhất một đẳng cấu $j$ của $\tilde{\mathbf{R}}_M \otimes \tilde{\mathbf{R}}_M$ lên bó tầm thường $R_X = X \times \mathbf{R}$ sao cho $j(\xi \otimes \xi) = (\pi(\xi), 1)$ với mọi $\xi \in \mathrm{Or}_M$; điều này cho phép đồng nhất bó vectơ $\tilde{\mathbf{R}}_M$ với đối ngẫu của nó.

10.3.3. Hơn nữa, cho $F$ là một bó vectơ có cơ sở $X$ và thuộc lớp $C^{r-1}$. Một dạng vi phân trên $X$ với các giá trị trong $\tilde{\mathbf{R}}_M \otimes F$ được gọi là một dạng vi phân xoắn $M$ với các giá trị trong $F$. Một dạng như vậy có bậc $p$ là một tiết diện của bó $\mathrm{Alt}^p(T(X); \tilde{\mathbf{R}}_M \otimes F)$, được đồng nhất theo một cách hiển nhiên với $\tilde{\mathbf{R}}_M \otimes \mathrm{Alt}^p(T(X); F)$. Khi $F$ là bó tầm thường được xác định bởi một không gian Banach $E$, người ta đơn giản gọi đó là một dạng xoắn $M$ với các giá trị trong $E$; khi $E = \mathbf{C}$ (tương ứng $\mathbf{R}$), người ta gọi đó là dạng xoắn $M$ phức (tương ứng dạng xoắn $M$ thực, hay dạng xoắn $M$).

Cho $\omega$ là một dạng xoắn $M$ bậc $p$ với giá trị trong $F$. Sự kiện rằng $\pi : \mathrm{Or}_M \to X$ là étale và rằng $\pi^*(\tilde{\mathbf{R}}_M) = \mathrm{Or}_M \times \mathbf{R}$ cho phép đồng nhất $\pi^*(\mathbf{R}_M \otimes \mathrm{Alt}^p(T(X); F))$ với $\mathrm{Alt}^p(T(\mathrm{Or}_M); \pi^*(F))$ và $\omega$ xác định một tiết diện $\tilde{\omega}$ của $\mathrm{Alt}^p(T(\mathrm{Or}_M); \pi^*(F))$ (7.4.3), nói cách khác, một dạng vi phân bậc $p$ trên $\mathrm{Or}_M$ với giá trị trong $\pi^*(F)$. Do đó ta thu được một song ánh từ không gian các dạng xoắn $M$ bậc $p$ trên $X$ với giá trị trong $F$, lên không gian các dạng $\tilde{\omega}$ bậc $p$ trên $\mathrm{Or}_M$ với giá trị trong $\pi^*(F)$ sao cho
$$
\tilde{\omega}(-\xi) = -\tilde{\omega}(\xi) \quad \text{với mọi } \xi \in \mathrm{Or}_M.
$$
Khi $M$ được trang bị một định hướng $\xi$, ánh xạ $\omega \mapsto \xi \otimes \omega$ cho phép các tiết diện của $\mathrm{Alt}^p(T(X); F)$ (nói cách khác các dạng vi phân thông thường bậc $p$) được đồng nhất với các dạng xoắn $M$ bậc $p$ với giá trị trong $F$.

10.3.4. Cho $\omega$ là một dạng vi phân xoắn $M$ bậc $p$ trên $X$, với giá trị trong một không gian Banach $E$, và thuộc lớp $C^s$ ($1 \leq s \leq \inf(k, r-1)$). Tồn tại duy nhất một dạng vi phân xoắn $M$ $d\omega$, bậc $p+1$ trên $X$, với giá trị trong $E$, sao cho, với mọi tập mở $U$ của $X$, định hướng $\xi$ của $M|U$ và dạng vi phân $\alpha$ trên $U$ sao cho $\omega|U = \xi \otimes \alpha$, ta có $d\omega|U = \xi \otimes d\alpha$. Dạng $d\omega$ thuộc lớp $C^{s-1}$; nó được gọi là vi phân ngoài của $\omega$.

Nếu $\tilde{\omega}$ (tương ứng $\tilde{d\omega}$) biểu thị dạng vi phân trên $\mathrm{Or}_M$ tương ứng với $\omega$ (tương ứng với $d\omega$) như trong 10.3.3, ta có $d(\tilde{\omega}) = \tilde{d\omega}$.

Nếu $\zeta$ là một trường vectơ thuộc lớp $C^s$ trên $X$, ta định nghĩa tương tự dạng xoắn bởi $M$ $\theta_\zeta.\omega$. Ta có
$$
\theta_\zeta.\omega = d(i(\zeta)\omega) + i(\zeta)d\omega
$$
và $\theta_\zeta.\omega$ thuộc lớp $C^{s-1}$.

### 10.4. Độ đo liên kết với một dạng vi phân xoắn

Ta nhắc lại rằng, trong số này, ta giả sử $K = \mathbf{R}$ và tất cả các đa tạp được xét đều có số chiều hữu hạn địa phương.

10.4.1. Cho X là một đa tạp thuộc lớp C'. Ta có thể áp dụng các định nghĩa và các kết quả của 10.3 bằng cách lấy bó vectơ M là bó tiếp xúc T(X). Khi đó ta có Or_M = $\tilde{X}$ (10.2.4); ta ký hiệu $\tilde{R}_X$ và gọi đơn giản bó các vô hướng xoắn là bó $\tilde{R}_{T(X)}$ (10.3.1)[^2]; một dạng vi phân xoắn bởi T(X) với giá trị trong một bó vectơ F được gọi đơn giản là một dạng vi phân xoắn (hoặc lẻ) với giá trị trong F. Khi X được trang bị một định hướng, ánh xạ $\omega \mapsto \xi \otimes \omega$ cho phép đồng nhất các dạng vi phân thông thường (đôi khi được gọi là «cặp») với các dạng xoắn.

10.4.2. Cho $f : X \to Y$ là một cấu xạ của các đa tạp thuộc lớp C' và cho $\tilde{f} : \tilde{X} \to \tilde{Y}$ là một định hướng của $f$ (10.2.5). Tồn tại một và chỉ một đẳng cấu $j$ của $f^*(\tilde{R}_Y)$ lên $\tilde{R}_X$ sao cho $\tilde{x} = j(\pi(\tilde{x}), \tilde{f}(\tilde{x}))$ với mọi $\tilde{x} \in \tilde{X}$. Ta đồng nhất hai bó này nhờ $j$. Nếu $\omega$ là một dạng xoắn bậc $p$ trên Y với giá trị trong một bó vectơ F, thì ảnh ngược $f^*(\omega)$ được đồng nhất với một dạng vi phân xoắn bậc $p$ trên X với giá trị trong $f^*(F)$. Nếu ta ký hiệu bởi $\tilde{\omega}$ (tương ứng $\tilde{f}^*(\omega)$) dạng vi phân trên $\tilde{Y}$ (tương ứng $\tilde{X}$) tương ứng với $\omega$ (tương ứng $f^*(\omega)$) như trong 10.3.3, ta có $\tilde{f}^*(\tilde{\omega}) = \tilde{f}^*(\omega)$.

Khi F là bó tầm thường được xác định bởi một không gian Banach, phép toán $f^*$ giao hoán với phép vi phân ngoài (10.3.4).

10.4.3. Cho X là một đa tạp thuần nhất có chiều n, và cho $\omega$ là một dạng vi phân xoắn bậc n trên X, với giá trị trong một không gian Banach E. Cho $c = (U, \varphi, \mathbf{R}^n)$ là một biểu đồ của X và cho $\xi^n$ là định hướng chính tắc của $\mathbf{R}^n$; cho $u^1, \ldots, u^n$ là các hàm tọa độ trên $\mathbf{R}^n$. Tồn tại một và chỉ một hàm $f_c$ trên $\varphi(U)$, với giá trị trong E, sao cho

$$
\omega|U = \varphi^*(\xi^n \otimes f_c . du^1 \wedge \cdots \wedge du^n).
$$

Ta nói rằng $\omega$ khả tích địa phương nếu, đối với mọi biểu đồ $c = (U, \varphi, \mathbf{R}^n)$ của X, hàm tương ứng $f_c$ khả tích địa phương đối với $\lambda_{\varphi(U)}^{\otimes n}$ (trong đó $\lambda$ ký hiệu độ đo Lebesgue trên $\mathbf{R}$). Giả sử điều này xảy ra và X là tách được. Tồn tại trên X một và chỉ một độ đo vectơ $\alpha(\omega)$ có các giá trị trong E có tính chất sau: đối với mọi biểu đồ $c = (U, \varphi, \mathbf{R}^n)$ của X, ảnh qua $\varphi$ của hạn chế trên U của độ đo $\alpha(\omega)$ là độ đo $f_c . \lambda_{\varphi(U)}^{\otimes n}$ (INT, VI, § 2, No. 4). Ta nói rằng $\alpha(\omega)$ là độ đo được xác định bởi $\omega$ và thông thường ký hiệu nó đơn giản là $\omega$. Giá đỡ của $\alpha(\omega)$ được chứa trong giá đỡ Supp $\omega$ của $\omega$ (trong đó giá đỡ của một dạng vi phân $\omega$ được định nghĩa là bao đóng của tập hợp các $x \in X$ sao cho $\omega(x) \neq 0$).

Nếu $f$ là một hàm thực trên X, khả tích địa phương đối với độ đo $\alpha(\omega)$, thì dạng vi phân $f \omega$ khả tích địa phương và ta có $\alpha(f \omega) = f . \alpha(\omega)$.

Nếu $g$ là một hàm thực trên $X$ khả tích thực sự đối với $\alpha(\omega)$, tích phân của nó nói chung được ký hiệu $\int_X g \omega$, hoặc $\int g \omega$, hoặc $\int g(x) \omega(x)$; người ta tránh ký hiệu nó là $\int g \, d\omega$, vì nguy cơ nhầm lẫn với vi phân ngoài $d\omega$ của $\omega$, là cái được xác định (và hơn nữa bằng 0) nếu $\omega$ thuộc lớp $C^1$. Nếu A là một tập con của X mà hàm đặc trưng $\varphi_A$ của nó khả tích thực sự đối với $\alpha(\omega)$, tích phân của $\varphi_A$ được ký hiệu

∫_A ω. Nếu hằng 1 khả tích thực sự đối với α(ω), người ta nói rằng ω khả tích.

Bây giờ cho p là một số nguyên, với 0 ≤ p ≤ n, và cho $\omega$ là một dạng vi phân xoắn bậc p trên X, có các giá trị trong một không gian Banach E. Hơn nữa, cho Y là một đa tạp con thuần nhất có chiều p của X; giả sử rằng đơn ánh chính tắc i : Y → X được trang bị một định hướng. Ảnh ngược i*(ω) (10.4.2) đôi khi khi đó được ký hiệu là ω|Y. Nếu ω|Y khả tích, ta đặt

$$
\int_Y \omega = \int_Y \omega|Y.
$$

10.4.4. Cho X là một đa tạp thuần nhất chiều n, được trang bị một định hướng ξ. Sự đồng nhất hóa ω ↦ ξ ⊗ ω giữa các dạng vi phân thông thường và các dạng vi phân xoắn làm cho có thể áp dụng các kết quả trên cho các dạng bậc n trên X; như vậy, với mỗi dạng khả tích địa phương ω, bậc n, tương ứng với một độ đo trên X, vẫn ký hiệu là ω. Nếu E = R, một dạng như vậy ω có môđun khả tích địa phương (10.1.5) và độ đo tương ứng mod(ω)_μ (10.1.6) không gì khác ngoài giá trị tuyệt đối |ω| của độ đo ω (INT, III, § 1, No. 6).

10.4.5. Ví dụ. — Cho X là một đa tạp thực thuần nhất chiều 1, có định hướng, tách được, và cho z : X → C là một ánh xạ khả vi từ X vào C. Dạng vi phân phức dz xác định trên X một độ đo phức cũng ký hiệu là dz. Điều này đặc biệt áp dụng khi X là một đa tạp con vi phân thuần nhất chiều 1 của C, z là đơn ánh của X vào C.

Cụ thể hơn, lấy X là một đường tròn có tâm 0 và bán kính ρ > 0; định hướng X như đã chỉ ra trong 10.2.8, b), có tính đến sự đồng nhất hóa thông thường của C với R²; nếu x ∈ X, không gian tiếp xúc T_x(X) được đồng nhất hóa với nửa phải Rix của T_x(C) = C và định hướng được chọn là nửa phải R_+ ix. Nếu f là một hàm liên tục trên X, có các giá trị trong một không gian Banach phức, tích phân của f đối với độ đo dz được cho bởi công thức

$$
\int_X f(z)\,dz = i\rho \int_0^{2\pi} f(\rho e^{i\alpha})\,e^{i\alpha}\,d\alpha.
$$

Chẳng hạn, nếu n là một số nguyên, ta có

$$
\int_X z^n\,dz = i\rho^{n+1} \int_0^{2\pi} e^{(n+1)i\alpha}\,d\alpha = \begin{cases} 0 & \text{nếu } n \neq -1 \\ 2i\pi & \text{nếu } n = -1. \end{cases}
$$

10.4.6 (« Trường hợp phức »). Cho X^c là một đa tạp giải tích phức tách được, thuần nhất chiều m, và cho ω là một dạng vi phân giải tích bậc m trên X^c. Cho X là đa tạp giải tích thực nằm dưới X^c; dạng ω được đồng nhất hóa với một dạng kiểu (m, 0) trên X (8.8.9); cho $\overline{\omega}$ là liên hợp của nó (8.8.2). Dạng $i^{m^2} \omega \wedge \overline{\omega}$ là một dạng vi phân thực bậc 2m trên X; có tính đến định hướng chính tắc của X (10.2.7), dạng này được đồng nhất hóa với một độ đo trên X, là đúng bằng độ đo dương mod(ω)_μ được xác định trong 10.1.6, trong đó μ là độ đo được xác định bởi dạng vi phân $i\,dz\wedge d\bar z$, nói cách khác là hai lần độ đo Lebesgue $\lambda^{\otimes 2}$ trên $\mathbf{C}$ (được đồng nhất hóa với $\mathbf{R}^2$ theo cách thông thường).

Cho H là không gian các dạng giải tích $\omega$ bậc m trên $X^c$ sao cho độ đo $\omega\wedge\bar\omega$ bị chặn. Với $\alpha,\beta$ trong H, độ đo phức $\alpha\wedge\bar\beta$ bị chặn; bằng cách đặt

$$
(\alpha|\beta)=i^{m^2}\int_X \alpha\wedge\bar\beta,
$$

ta thu được một dạng Hermit trên H, dạng này làm cho H trở thành một không gian Hilbert.

[^1]: Khi $K = \mathbf{R}$, chỉ cần giả sử rằng $r > \sup_{y \in Y} (\dim_{f(y)} X - \dim_y Y)$; xem chẳng hạn A. SARD, Bull. Am. Math. Soc., XLVIII (1943), p. 883–890.

[^2]: Cần chú ý rằng ký hiệu này mâu thuẫn với ký hiệu $\tilde{R}_M$ khi ta xét X như được trang bị cấu trúc của một bó vectơ hạng 0 trên chính nó.
