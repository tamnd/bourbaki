---
book: var
book_title: Variétés différentielles et analytiques
chapter: "1"
chapter_title: VARIÉTÉS DIFFÉRENTIELLES ET ANALYTIQUES, FASCICULE DE RÉSULTATS
section: 3
section_title: Fonctions analytiques réelles ou complexes
lang: vi
source: var-fr
pdf_pages: 0020-0028
extraction: ocr
subsections:
    - "no": 1
      title: Séries convergentes
      page: 0
      pdf_page: 20
    - "no": 2
      title: Fonctions analytiques
      page: 0
      pdf_page: 24
    - "no": 3
      title: Fonctions holomorphes
      page: 0
      pdf_page: 26
    - "no": 4
      title: Fonctions analytiques réelles
      page: 0
      pdf_page: 28
statements: 0
exercises: 0
content_sha256: 7cabddb2a89c3cde7bd84483904f18e5cd6ca95a78dcc45f4db0e8f6cb728bcd
translated_from: content/en-mt/var/1/03_s3_fonctions_analytiques_reelles_ou.md
source_lang: en-mt
translation_method: machine
source_content_sha256: f57b08ffe64096e3070f1e8db29f0883cd9e1d33972479170757b88e14b6846d
translation_model: gpt-5-6-mini, gpt-5-mini
translation_run: translate-vi-3307ed33
glossary_version: 34
glossary_terms_sha256: f26fd13fb34168cc57715b7403ec8018791aeb3be60b4d709f375f026ee4ed8c
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 3. Các hàm giải tích thực hoặc phức

Trong đoạn này, giả sử rằng $K = \mathbf{R}$ hoặc $\mathbf{C}$. Cho $(E_i),\ 1 \leq i \leq n$, là một họ hữu hạn các không gian chuẩn trên $K$, cho $E$ là không gian tích của các $E_i$, và cho $F$ là một không gian vectơ tôpô lồi địa phương tách được trên $K$.

### 3.1. Chuỗi hội tụ

3.1.1. Cho $f = \sum f_\alpha$ là một chuỗi hình thức thuộc $\hat{P}(E_1, \ldots, E_n; F)$ (Phụ lục, No. A.5). Nếu $\gamma$ là một nửa chuẩn liên tục trên $F$ và $R = (R_1, \ldots, R_n)$ là một dãy gồm $n$ số thực dương ngặt, ta đặt:

$$
\|f\|_{\gamma, R} = \sum_\alpha R^\alpha \|f_\alpha\|_\gamma.
$$

Nếu $F$ là một không gian chuẩn và nếu $\gamma$ là chuẩn của $F$, ta viết $\|f\|_R$ thay cho $\|f\|_{\gamma, R}$.

Tập hợp $\mathcal{H}_R(E_1, \ldots, E_n; F)$ gồm các $f \in \hat{P}(E_1, \ldots, E_n; F)$ sao cho $\|f\|_{\gamma, R}$ là hữu hạn đối với mọi nửa chuẩn liên tục $\gamma$ trên $F$ là một không gian con vectơ của $\hat{P}(E_1, \ldots, E_n; F)$. Ta có

$$
\mathcal{H}_R(E_1, \ldots, E_n; F) \subset \mathcal{H}_{R'}(E_1, \ldots, E_n; F)
$$

mỗi khi $R_i \geq R'_i$ với $1 \leq i \leq n$. Hợp của

$$
\mathcal{H}_R(E_1, \ldots, E_n; F)
$$

là một không gian con vectơ, được ký hiệu bởi $\mathcal{H}(E_1, \ldots, E_n; F)$, của $\hat{P}(E_1, \ldots, E_n; F)$, mà các phần tử của nó được gọi là các chuỗi hội tụ trên tích của các $E_i$, với giá trị trong $F$. Nó chỉ phụ thuộc vào tôpô của các $E_i$ chứ không phụ thuộc vào các chuẩn của chúng. Do đó ta có thể nói đến không gian $\mathcal{H}(E_1, \ldots, E_n; F)$ khi các $E_i$ là các không gian chuẩn hóa được, mà không cần phải chọn một chuẩn trên mỗi $E_i$.

3.1.2. Ánh xạ $f \mapsto \|f\|_{\gamma, R}$ là một nửa chuẩn trên $\mathcal{H}_R(E_1, \ldots, E_n; F)$. Tôpô được xác định bởi các nửa chuẩn này khi $\gamma$ chạy trên tập hợp các nửa chuẩn liên tục trên $F$ (hoặc đơn giản là một tập hợp các nửa chuẩn xác định tôpô của $F$) là tách được. Nếu $F$ là chuẩn hóa được (tương ứng, đầy đủ), điều tương tự cũng đúng đối với $\mathcal{H}_R(E_1, \ldots, E_n; F)$. Các nửa chuẩn trên $\mathcal{H}(E_1, \ldots, E_n; F)$ mà hạn chế của chúng trên mỗi $\mathcal{H}_R$ là liên tục xác định một tôpô tách được trên $\mathcal{H}(E_1, \ldots, E_n; F)$, tôpô này chỉ phụ thuộc vào các tôpô của các $E_i$. Đơn ánh của $\mathcal{H}(E_1, \ldots, E_n; F)$ vào $\hat{P}(E_1, \ldots, E_n; F)$ là liên tục.

3.1.3. Đẳng cấu chính tắc của $\hat{P}(E; F)$ lên $\hat{P}(E_1, \ldots, E_n; F)$ cho bởi hạn chế một đẳng cấu của các không gian vectơ tôpô của $\mathcal{H}(E; F)$ lên $\mathcal{H}(E_1, \ldots, E_n; F)$.

3.1.4. Cho $f \in \mathcal{H}(E_1, \ldots, E_n; F)$ và gọi $J(f)$ là tập hợp các $R \in (\mathbf{R}_+^*)^n$ sao cho $f \in \mathcal{H}_R(E_1, \ldots, E_n; F)$. Phần trong $I(f)$ của $J(f)$ được gọi là chỉ thị hội tụ ngặt của $f$. Nó gồm tập hợp các $R$ sao cho tồn tại một $R' \in J(f)$ với $0 < R_i < R'_i$ đối với $1 \leq i \leq n$. Ta ký hiệu $\Omega(f)$ là tập hợp các điểm $(\log R_1, \ldots, \log R_n)$ của $\mathbf{R}^n$ ứng với $R \in I(f)$: đây là một tập con lồi của $\mathbf{R}^n$.

Khi $n = 1$, tập hợp $I(f)$ là một khoảng $]0, \rho(f)[$ của $\mathbf{R}$, và $\rho(f)$ được gọi là bán kính hội tụ ngặt của $f$. Nó cũng là cận trên nhỏ nhất (hữu hạn hoặc $+\infty$) của tập hợp các số thực $R > 0$ sao cho với mọi nửa chuẩn liên tục $\gamma$ trên $F$, tồn tại một hằng $M$ sao cho $\|f_m\|_{\gamma} \leq MR^{-m}$ (với $f = \sum f_m, f_m \in P_m(E; F)$) đối với mọi số nguyên $m \geq 0$.

Tập hợp các điểm $x = (x_i) \in E_1 \times \cdots \times E_n$ sao cho tồn tại $R \in I(f)$ với $\|x_i\| \leq R_i$ đối với mọi $i$ được gọi là miền hội tụ ngặt của $f$ và được ký hiệu là $C(f)$. Nó cũng là phần trong của tập hợp các điểm $x$ mà với chúng tồn tại $R \in J(f)$ sao cho $\|x_i\| < R_i$ đối với mọi $i$.

3.1.5. Với $f_\alpha \in P_\alpha(E_1, \ldots, E_n; F)$ và với mọi nửa chuẩn liên tục $\gamma$ trên $F$, đặt:
$$
\|f_\alpha\|_{\gamma} = \sup_{\|x_i\| \leq 1} \|f_\alpha(x_1, \ldots, x_n)\|_{\gamma}.
$$
Khi đó ta có các bất đẳng thức:
$$
\|f_\alpha\|_{\gamma} \leq \|f_\alpha\|_{\gamma'} \leq \frac{\alpha^\alpha}{\alpha!} \|f_\alpha\|_{\gamma}.
$$
Với $f = \sum f_\alpha \in \hat{P}(E_1, \ldots, E_n; F)$ và $R \in (\mathbf{R}_+^*)^n$, đặt:
$$
\|f\|_{\gamma, R} = \sum_\alpha R^\alpha \|f_\alpha\|_{\gamma}
$$
và gọi $\tilde{\mathcal{H}}_R(E_1, \ldots, E_n; F)$ là không gian con vectơ của $\hat{P}(E_1, \ldots, E_n; F)$
gồm các $f$ sao cho $\|f\|_{\gamma, R}$ hữu hạn với mọi $\gamma$, được trang bị tôpô xác định bởi các nửa chuẩn $f \mapsto \|f\|_{\gamma, R}$. Ta có $\mathcal{H}_R \subset \tilde{\mathcal{H}}_R$ và đơn ánh của $\mathcal{H}_R$ vào $\tilde{\mathcal{H}}_R$ là liên tục. Không gian $\mathcal{H}(E_1, \ldots, E_n; F)$ là hợp của các $\tilde{\mathcal{H}}_R(E_1, \ldots, E_n; F)$ và tôpô của nó là tôpô lồi địa phương ngặt nhất sao cho các đơn ánh của các $\mathcal{H}_R$ vào $\mathcal{H}$ là liên tục.

Nếu $f \in \mathcal{H}(E_1, \ldots, E_n; F)$, **chỉ số hội tụ** được định nghĩa là phần trong $\tilde{I}(f)$ của tập $\tilde{J}(f)$ gồm các $R \in (\mathbf{R}_+^*)$ sao cho $f \in \tilde{\mathcal{H}}_R$. Ta có:
$$
e^{-1}\tilde{I}(f) \subset I(f) \subset \tilde{I}(f)
$$
(trong đó $e$ là cơ số của các logarit Nêpe). Từ $\tilde{I}(f)$ ta định nghĩa, như trong 3.1.4., miền hội tụ $\tilde{C}(f)$ và, khi $n = 1$, bán kính hội tụ $\tilde{\rho}(f)$. Đặc biệt, ta có:
$$
e^{-1}\tilde{\rho}(f) \leq \rho(f) \leq \tilde{\rho}(f).
$$

3.1.6. Với $R \in (\mathbf{R}_+^*)^n$, đa cầu (đóng) tâm 0 và bán kính $R$ trong $E$ là tập hợp $B(R)$ gồm các $x \in E$ sao cho $\|x_i\| \leq R_i$ với mọi $i$. Nếu $\dim E_i = 1$, người ta cũng gọi là đĩa đa chiều. Nếu $f \in \mathcal{H}(E_1, \ldots, E_n; F)$, miền hội tụ (tương ứng miền hội tụ ngặt) của $f$ là hợp của các đa cầu $B(R)$ với $R \in \tilde{I}(f)$ (tương ứng $R \in I(f)$).

3.1.7. Cho $f \in \mathcal{H}(E_1, \ldots, E_n; F)$. Giả sử rằng $F$ là gần đầy đủ. Với mọi $x \in \tilde{C}(f)$, họ các $f_a(x)$ là tổng được trong $F$. Tổng của nó, ký hiệu là $\hat{f}(x)$ hoặc đơn giản là $f(x)$, là một hàm liên tục trên $\tilde{C}(f)$. Chính xác hơn, với mọi $R$ sao cho $f \in \tilde{\mathcal{H}}_R$, họ các $f_a(x)$ là tổng được đều với $x \in B(R)$. Ánh xạ $f \mapsto \hat{f}$ là một ánh xạ tuyến tính liên tục đơn ánh từ $\tilde{\mathcal{H}}_R$ vào không gian các hàm liên tục bị chặn trên $B(R)$, được trang bị bởi tôpô hội tụ đều.

3.1.8. Cho $F_1, \ldots, F_m$ là các không gian đa chuẩn tách được và cho $u$ là một ánh xạ tuyến tính $m$-liên tục từ $F_1 \times \cdots \times F_m$ vào $F$. Cho $f_i \in \mathcal{H}(E_1, \ldots, E_n; F_i)$ với $1 \leq i \leq m$. Chuỗi hình thức $u(f_1, \ldots, f_m)$ thuộc về $\mathcal{H}(E_1, \ldots, E_n; F)$. Ta có:

$$
C(u(f_1, \ldots, f_m)) \supset \bigcap_i C(f_i)
$$
$$
\tilde{C}(u(f_1, \ldots, f_m)) \supset \bigcap_i \tilde{C}(f_i)
$$

và nếu $x \in \bigcap_i \tilde{C}(f_i)$, $F$ và các $F_i$ là gần đầy đủ, ta có:
$$
u(f_1, \ldots, f_m)(x) = u(f_1(x), \ldots, f_m(x)).
$$

3.1.9. Cho $F_1, \ldots, F_m$ là các không gian định chuẩn đầy đủ và giả sử rằng $F$ là gần đầy đủ. Cho $f = (f_i)_{1 \leq i \leq m}$ với $f_i \in \mathcal{H}(E_1, \ldots, E_n; F_i)$ và $g \in \mathcal{H}(F_1, \ldots, F_m; F)$, sao cho $(f_i(0))_{1 \leq i \leq m}$ thuộc về miền hội tụ ngặt của $g$. Khi đó, với mọi $\alpha \in \mathbf{N}^m$, chuỗi hình thức $g_\alpha \circ f$ thuộc về $\mathcal{H}(E_1, \ldots, E_n; F)$ và họ các $g_\alpha \circ f$ là tổng được trong $\mathcal{H}(E_1, \ldots, E_n; F)$ và a fortiori trong $\hat{P}(E_1, \ldots, E_n; F)$. Tổng của nó sẽ được ký hiệu là $g \circ f$.

Chính xác hơn, tồn tại $R \in \bigcap_i I(f_i)$ và $R' \in I(g)$ sao cho $\|f_i\|_R < R'_i$ với $1 \leq i \leq m$. Với các điều kiện này, chuỗi hình thức $g_\alpha \circ f$ thuộc về $\mathcal{H}_R(E_1, \ldots, E_n; F)$, và họ các $g_\alpha \circ f$ là tổng được trong $\mathcal{H}_R(E_1, \ldots, E_n; F)$. Cuối cùng, nếu $x \in B(R)$, thì $f(x) = (f_i(x))$ thuộc về $B(R') \subset F_1 \times \cdots \times F_m$ và ta có:
$$
g(f(x)) = (g \circ f)(x).
$$

3.1.10. Giả sử rằng $E_i = K$ với $1 \leq i \leq n$. Không gian $\hat{P}(K^n; F)$ khi đó được đồng nhất với không gian các chuỗi hình thức theo $n$ phần tử bất định $X_1, \ldots, X_n$ với các hệ số trong $F$, và một phần tử của $\hat{P}(K^n; F)$ được viết:

$$
f = \sum_{\alpha} X^\alpha c_\alpha \quad \text{với } c_\alpha \in F.
$$

Nếu $R \in (\mathbf{R}_+^*)^n$ và nếu $\gamma$ là một nửa chuẩn liên tục trên $F$, ta có:

$$
\| f \|_{\gamma, R} = \| f \|_{\gamma, R} = \sum_{\alpha} R^\alpha \| c_\alpha \|_\gamma
$$

Ta có $I(f) = \tilde{I}(f)$, $C(f) = \tilde{C}(f)$ và, khi $n = 1$, $\rho(f) = \tilde{\rho}(f)$.

Không gian $\mathcal{H}(K^n; K)$ các chuỗi hội tụ với các hệ số trong $K$ còn được ký hiệu bởi $K\{(X_1, \ldots, X_n)\}$; nó là một đại số con của $K[[X_1, \ldots, X_n]]$. Không gian $\mathcal{H}(K^n; F)$ là một môđun trên $K\{(X_1, \ldots, X_n)\}$ và nếu $F$ là hữu hạn chiều, môđun này được đồng nhất với $K\{(X_1, \ldots, X_n)\} \otimes_K F$.

3.1.11. Cho $f \in \mathcal{H}(K^n; K^m)$, được biểu diễn bởi một hệ gồm $m$ chuỗi hội tụ $f_j(X_1, \ldots, X_n)$, với các hệ số trong $K$. Tương tự, cho $g \in \mathcal{H}(K^m; K^p)$, được biểu diễn bởi một hệ gồm $p$ chuỗi hội tụ $g_k(Y_1, \ldots, Y_m) = \sum g_{k,\beta} Y^\beta$. Phần tử $h = g \circ f$ của $\mathcal{H}(K^n; K^p)$ (xem 3.1.9) được biểu diễn bởi $p$ chuỗi hình thức $h_k(X_1, \ldots, X_n)$, được xác định như sau: với $\alpha \in \mathbf{N}^n$ và $\beta \in \mathbf{N}^m$, gọi $c_{\alpha,\beta}$ là hệ số của $X^\alpha$ trong chuỗi hình thức $f^\beta = \prod f_j^{\beta_j}$; khi đó họ $(g_{k,\beta} c_{\alpha,\beta})_{\beta \in \mathbf{N}^m}$ là tổng được trong $K$ và có tổng là hệ số của $X^\alpha$ trong $h_k$.

3.1.12. Giả sử $F$ đầy đủ giả và gọi $\hat{E}_i$ là sự hoàn thành của $E_i$. Mọi đa thức liên tục trên $E_1 \times \cdots \times E_n$ với các giá trị trong $F$ đều mở rộng bởi tính liên tục thành một đa thức liên tục trên $\hat{E}_1 \times \cdots \times \hat{E}_n$, với các giá trị trong $F$. Từ đó suy ra một song ánh $j$ của $\hat{P}(E_1, \ldots, E_n; F)$ lên $\hat{P}(\hat{E}_1, \ldots, \hat{E}_n; F)$. Nếu $f \in \mathcal{H}(E_1, \ldots, E_n; F)$, thì $j(f) \in \mathcal{H}(\hat{E}_1, \ldots, \hat{E}_n; F)$ và ngược lại. Các chỉ báo hội tụ ngặt của $f$ và của $j(f)$ là như nhau.

3.1.13. Giả sử rằng $K = \mathbf{R}$, nhưng $F$ được trang bị một cấu trúc không gian vectơ phức tương thích với cấu trúc không gian vectơ thực của nó. Đặt $E_i^C = E_i \otimes_\mathbf{R} \mathbf{C}$. Nếu $y \in E_i^C$, đặt

$$
y = \inf \sum_k |a_k| \cdot \| x_k \|,
$$

cận dưới lớn nhất được lấy trên mọi họ hữu hạn các cặp $(x_k, a_k) \in E_i \times \mathbf{C}$ sao cho $y = \sum_k x_k \otimes a_k$. Bằng cách này ta thu được một chuẩn trên không gian vectơ phức $E_i^C$; chuẩn này mở rộng chuẩn đã cho trên $E_i$ nếu ta đồng nhất $x \in E_i$ với $x \otimes 1$. Cho $h$ là một ánh xạ $\mathbf{R}$-đa thức-liên tục trên $E_1 \times \cdots \times E_n$, với giá trị trong $F$, và thuần nhất với đa bậc $\alpha$; khi đó tồn tại duy nhất một ánh xạ $\mathbf{C}$-đa thức-liên tục $\tilde{h}$ trên $E_1^C \times \cdots \times E_n^C$, với giá trị trong $F$, mở rộng $h$, và thuần nhất với đa bậc $\alpha$. Ta có

$$
\| \tilde{h} \|_\gamma = \| h \|_\gamma
$$

với mọi nửa chuẩn liên tục $\gamma$ trên không gian vectơ phức $F$.

Nếu $f = \sum_{\alpha} f_{\alpha} \in \mathcal{H}(E_1, \ldots, E_n; F)$, thì $\tilde{f} = \sum_{\alpha} \tilde{f}_{\alpha} \in \mathcal{H}(E_1^c, \ldots, E_n^c; F)$. Các chuỗi $f$ và $\tilde{f}$ có cùng biểu chỉ số hội tụ ngặt (và cùng bán kính hội tụ ngặt khi $n = 1$).

Ngược lại, giả sử $K = C$. Gọi $E_i^0$ và $F^0$ là các không gian trên $\mathbf{R}$ thu được bằng hạn chế vô hướng. Nếu $f_{\alpha} \in P_{\alpha}(E_1, \ldots, E_n; F)$, thì $f_{\alpha} \in P_{\alpha}(E_1^0, \ldots, E_n^0; F^0)$. Nếu $f = \sum_{\alpha} f_{\alpha} \in \mathcal{H}(E_1, \ldots, E_n; F)$, thì chuỗi hình thức $f^0 = \sum_{\alpha} f_{\alpha} \in \hat{P}(E_1^0, \ldots, E_n^0; F^0)$ là một chuỗi hội tụ. Các biểu chỉ số hội tụ (tương ứng, các biểu chỉ số hội tụ ngặt) của $f$ và $f^0$ là đồng nhất và ta có $f(x) = f^0(x)$ với mọi $x \in \bar{C}(f) = \bar{C}(f^0)$.

### 3.2. Hàm giải tích

3.2.1. Cho $U$ là một tập mở của $E$ và $f$ là một ánh xạ của $U$ vào $F$. Ta nói rằng $f$ là _thuộc lớp_ $C^{\omega}$, hoặc _K-giải tích_ (hay đơn giản là _giải tích_) trong $U$ nếu, với mọi điểm $a$ của $U$, tồn tại một chuỗi hội tụ $f_{\alpha} \in \mathcal{H}(E; F)$ sao cho $f(a + x) = f_{\alpha}(x)$ với mọi $x$ trong $E$ đủ gần không. Nếu $K = \mathbf{R}$ (tương ứng $\mathbf{C}$), ta cũng nói rằng $f$ là _giải tích thực_ (tương ứng _giải tích phức_ hoặc _chỉnh hình_). Các ánh xạ giải tích của $U$ vào $F$ tạo thành một không gian con vectơ, ký hiệu bởi $\mathcal{C}^{\omega}(U; F)$, của không gian tất cả các ánh xạ của $U$ vào $F$.

Với $a \in U$, chuỗi hình thức $f_{\alpha}$ là duy nhất: nó được gọi là _khai triển lũy thừa_ của $f$ tại điểm $a$. Nếu $f_{\alpha} = \sum_{\alpha} (f_{\alpha})_{\alpha}$ (với $(f_{\alpha})_{\alpha} \in P_{\alpha}(E_1, \ldots, E_n; F)$), ta đặt:

Δ α f(a)=(f α  ) α  .

3.2.2. Nếu $f \in \mathcal{C}^{\omega}(U; F)$, ánh xạ $\Delta^{\alpha} f : a \mapsto \Delta^{\alpha} f(a)$ của $U$ vào

P α  (E 1  ,…,E n  ;F)

là giải tích. Ánh xạ $\Delta^{\alpha} : f \mapsto \Delta^{\alpha} f$ là một ánh xạ tuyến tính theo $K$ của $\mathcal{C}^{\omega}(U; F)$ vào $\mathcal{C}^{\omega}(U; P_{\alpha}(E_1, \ldots, E_n; F))$. Với $a \in U$, do đó ta có, với $\alpha, \beta \in \mathbf{N}^n$, $\Delta^{\beta}(\Delta^{\alpha} f)(a) \in P_{\beta}(E_1, \ldots, E_n; P_{\alpha}(E_1, \ldots, E_n; F))$. Nếu $x = (x_i) \in E$, do đó ta có $(\Delta^{\beta}(\Delta^{\alpha} f)(a))(x) \in P_{\alpha}(E_1, \ldots, E_n; F)$ và $((\Delta^{\beta}(\Delta^{\alpha} f)(a))(x))(x) \in F$. Phần tử này của $F$ bằng $((\alpha, \beta))(\Delta^{\alpha+\beta} f(a))(x)$. Điều này được biểu diễn bằng cách viết:

Δ β ∘Δ α =((α,β))Δ α+β .

3.2.3. Các chỉ số hội tụ ngặt (và các bán kính hội tụ ngặt khi $n = 1$) của các khai triển lũy thừa của $f$ và của $\Delta^{\alpha} f$ tại cùng một điểm $a$ của $U$ là đồng nhất.

3.2.4. Cho $f \in \mathcal{C}^\omega(U; F)$. Khi đó $f$ khả vi nghiêm ngặt và khả vi vô hạn lần trong $U$ (nếu $K = \mathbf{R}$, $f$ thuộc lớp $C^\infty$ trong $U$). Các đạo hàm lặp của $f$ là giải tích, và giá trị của chúng tại một điểm $a$ là các ánh xạ đa tuyến đối xứng. Khi đó ta có thể đưa vào ký hiệu $D^\alpha f$ cho các đạo hàm riêng lặp như trong No. 2.4.2. Ta có:

$$
\alpha! \Delta^\alpha f(a)(h) = D^\alpha f(a) . (h, \ldots, h)
$$

với mọi $a \in U$ và $h \in E$, được viết:

$$
\alpha! \Delta^\alpha f = D^\alpha f .
$$

3.2.5. Cho $U$ là một tập con mở của $E$ và cho $f, g$ là hai ánh xạ giải tích của $U$ vào $F$. Cho $a \in U$. Để $f$ và $g$ có tiếp xúc cấp $\geq k$ tại $a$, điều kiện cần và đủ là $\Delta^\alpha f(a) = \Delta^\alpha g(a)$ với mọi $\alpha$ sao cho $|\alpha| \leq k$. Nếu $f$ và $g$ có tiếp xúc cấp vô hạn tại $a$, chúng bằng nhau trong một lân cận của $a$. Tập hợp các điểm của $U$ tại đó $f$ và $g$ có tiếp xúc cấp vô hạn là mở và đóng.

Đặc biệt, nếu $U$ liên thông và nếu tồn tại một tập con mở khác rỗng của $U$ trên đó $f$ và $g$ bằng nhau, thì $f = g$ ("nguyên lý tiếp tục giải tích").

3.2.6. Cho $U$ là một tập con mở của $E$ và cho $f$ là một ánh xạ giải tích của $U$ vào $F$. Nếu đạo hàm $Df$ của $f$ là không, thì $f$ là hằng địa phương.

3.2.7. Giả sử $F$ là đầy đủ giả và cho $G$ là một không gian chuẩn đầy đủ. Cho $g$ là một ánh xạ giải tích của một tập mở $U$ của $E$ vào $G$ và cho $f$ là một ánh xạ giải tích của một tập mở $V$ của $G$, chứa $g(U)$, vào $F$. Ánh xạ hợp thành $f \circ g$ là giải tích trong $U$. Giả sử thêm rằng $0 \in U$ và $g(0) = 0$. Khi đó khai triển của $f \circ g$ thành chuỗi lũy thừa tại $0$ thu được bằng cách thế, trong khai triển của $f$ tại $0$, khai triển chuỗi lũy thừa của $g$ tại $0$ (3.1.9).

3.2.8. Cho $F_1, \ldots, F_m$ là các không gian đa chuẩn tách được và $u$ là một ánh xạ đa tuyến tính liên tục của $F_1 \times \cdots \times F_m$ vào $F$. Cho $U$ là một tập mở của $E$ và $f_i \in \mathcal{C}^\omega(U; F_i)$. Hàm $u(f_1, \ldots, f_m)$ là giải tích, và khai triển của nó thành một chuỗi lũy thừa tại một điểm $a \in U$ là chuỗi $u((f_1)_a, \ldots, (f_m)_a)$ (3.1.8).

3.2.9. Giả sử $F$ là đầy đủ giả. Cho $f \in \mathcal{H}(E_1, \ldots, E_n; F)$; hàm $x \mapsto f(x)$ (3.1.7) là giải tích trong tập mở $C(f)$, miền hội tụ ngặt của $f$. Nếu $n = 1$ và nếu $\|a\| < \rho(f)$, bán kính hội tụ ngặt của khai triển của $f$ thành một chuỗi lũy thừa tại $a$ ít nhất bằng $\rho(f) - \|a\|$. Nếu $\rho(f) = + \infty$, người ta nói rằng $f$ là một hàm nguyên.

3.2.10. Giữ lại các giả thiết của 3.2.9. Nếu $K = \mathbf{C}$, các kết quả của 3.2.9 vẫn đúng nếu thay $C(f)$ bởi $\tilde{C}(f)$ và $\rho(f)$ bởi $\tilde{\rho}(f)$ (đối với $n = 1$). Nếu $K = \mathbf{R}$, hàm $x \mapsto f(x)$ là giải tích trong $\tilde{C}(f)$.

3.2.11. Giả sử rằng $E_i = K$ với $1 \leq i \leq n$. Cho $U$ là một tập mở của $K^n$ và cho $f \in \mathcal{C}^\omega(K^n; F)$. Nếu $0 \in U$ và nếu $f_0 = \sum_\alpha X^\alpha c_\alpha$ là khai triển chuỗi lũy thừa của $f$ tại $0$, khai triển chuỗi lũy thừa của $\Delta^\alpha f$ tại $0$ được viết (sau khi nhận dạng $P_\alpha(K^n; F)$ với $F$):

$$
(\Delta^\alpha f)_0 = \sum_\beta ((\alpha, \beta)) X^\beta c_{\alpha + \beta}.
$$

Đặc biệt, với $1 \leq i \leq n$ và với $x \in C(f_0)$, ta có:

$$
\partial_i f(x) = \sum_\alpha (\alpha_i + 1) x^\alpha c_{\alpha + e_i}.
$$

### 3.3 Các hàm chỉnh hình

Trong Số này, giả sử rằng $K = \mathbf{C}$.

3.3.1. Giả sử $F$ đầy đủ nửa. Cho $U$ là một tập mở của $E$ và cho $f$ là một ánh xạ từ $U$ vào $F$. Các điều kiện sau là tương đương:
(i) $f$ là chỉnh hình;
(ii) $f$ khả vi;
(iii) $f$ bị chặn địa phương và, bất kể $a \in U$ và $h \in E$ là gì, hàm $t \mapsto f(a + th)$, được xác định trong một lân cận mở của $0$ trong $C$, là chỉnh hình;
(iv) $f$ bị chặn địa phương và với mọi dạng tuyến tính liên tục $u$ trên $F$, hàm nhận giá trị trong $\mathbf{C}$ $u \circ f$ là chỉnh hình;
(v) $f$ liên tục và bị chặn địa phương và tồn tại một tập hợp toàn phần $H$ của đối ngẫu của $F$ sao cho $u \circ f$ là chỉnh hình với mọi $u \in H$.

Khi $E$ là hữu hạn chiều (tương ứng, khi $F$ là một không gian Banach), các điều kiện này vẫn tương đương với các điều kiện (iii'), (iv') hoặc (v') (tương ứng, (iv') hoặc (v')) nhận được từ (iii), (iv) hoặc (v) (tương ứng, (iv) hoặc (v)) bằng cách bỏ giả thiết "$f$ là bị chặn địa phương".

3.3.2. Giả sử $F$ đầy đủ nửa. Cho $U$ là một tập mở của $E$ và $(f_n)$ là một dãy các ánh xạ chỉnh hình từ $U$ vào $F$, có tính chất sau:
(W) Mỗi điểm của $U$ có một lân cận trong đó dãy $(f_n)$ hội tụ đều.
Khi đó giới hạn $f$ của dãy $(f_n)$ là chỉnh hình, dãy các đạo hàm $(Df_n)$ (với các giá trị trong không gian đầy đủ nửa $\mathcal{L}(E; F)$) có tính chất (W), và $Df$ là giới hạn của $(Df_n)$.

3.3.3. Cho U là một tập mở của E và f là một ánh xạ chỉnh hình từ U vào F, được giả thiết là nửa đầy đủ. Cho $R = (R_i) \in (\mathbf{R}_+^*)^n$ và giả sử rằng đa cầu B(R) được chứa trong U và f bị chặn trên B(R). Khi đó, với mọi $α \in \mathbf{N}^n$ và mọi $x = (x_i) \in B(R)$:

$$
Δ^αf(0)(x) = \int_0^1 \cdots \int_0^1 f(e(\theta_1)x_1, \ldots, e(\theta_n)x_n)e(-α_1θ_1 - \cdots - α_nθ_n)\ dθ_1 \ldots dθ_n
$$

(với $e(θ) = \exp 2πi θ$).

Ngoài ra, cho $γ$ là một bán chuẩn liên tục trên F và cho M là cận trên của $\|f(x)\|_γ$ đối với $\|x_i\| = R_i$. Khi đó $\|Δ^αf(0)(x)\|_γ \leq M$ với mọi $x \in B(R)$ và $\|Δ^αf(0)\|_γ \leq MR^{-α}$. Cuối cùng, miền hội tụ của khai triển chuỗi của f tại 0 chứa phần trong của đa cầu B(R).

3.3.4. Ta giữ lại các giả thiết của 3.3.3 và giả sử thêm rằng $E_i = \mathbf{C}$. Cho $\sum_{α} X^αc_α$ là khai triển chuỗi của f tại 0. Ta có:

$$
c_α = R^{-α}\int_0^1 \cdots \int_0^1 f(e(\theta_1)R_1, \ldots, e(\theta_n)R_n)e(-α_1θ_1 - \cdots - α_nθ_n)\ dθ_1 \ldots dθ_n
$$

và:

$$
\|c_α\|_γ \leq R^{-α} \sup_{x \in B(R)} \|f(x)\|_γ
$$

(“các bất đẳng thức Cauchy”). Miền hội tụ ngặt của chuỗi $\sum_{α} X^αc_α$ chứa phần trong của B(R).

3.3.5. Giả sử E hữu hạn chiều và F nửa đầy đủ. Cho f là một ánh xạ chỉnh hình từ E vào F. Khi đó tồn tại trong $\mathscr{H}(E; F)$ duy nhất một chuỗi f_0, có bán kính hội tụ vô hạn (đối với mọi chuẩn trên E), sao cho $f(x) = f_0(x)$ với mọi $x \in E$.

3.3.6. Nếu f là một ánh xạ chỉnh hình từ E vào F sao cho $f(E)$ bị chặn, thì hàm f là hằng (“định lý Liouville”).

3.3.7. Ta giả sử rằng $E \neq 0$. Cho f là một ánh xạ chỉnh hình từ một tập mở U của E vào F. Cho a là một điểm của U và $γ$ là một bán chuẩn liên tục trên F. Với mọi lân cận V của a, được chứa trong U, tồn tại $x \in V, x \neq a$, sao cho:

$$
\|f(a)\|_γ \leq \|f(x)\|_γ.
$$

Nếu ngoài ra $F = \mathbf{C}$ và nếu f không hằng trong một lân cận của a, ta có $|f(a)| < \sup_{x \in V, x \neq a} |f(x)|$ và ánh xạ f là mở trong một lân cận của a.

Cuối cùng, cho B là một tập mở bị chặn có bao đóng được chứa trong U và cho B' là biên của nó. Ta có:

$$
\sup_{x \in \overline{B}} |f(x)| = \sup_{x \in B'} |f(x)|
$$

(“nguyên lý cực đại”).

3.3.8. Giả sử E hữu hạn chiều. Cho U là một tập mở của E, S là một không gian con vectơ có đối chiều $\geq 2$ của E và $f$ là một ánh xạ chỉnh hình từ $U \cap (E - S)$ vào F. Khi đó $f$ mở rộng bởi tính liên tục thành một ánh xạ chỉnh hình từ U vào F.

3.3.9. Giả sử rằng $E = \mathbf{C}$ và cho $0 \leq \lambda < \mu \leq +\infty$. Cho $f$ là một ánh xạ chỉnh hình từ tập mở $U = \{ z \in \mathbf{C} | \lambda < |z| < \mu \}$ vào F. Tồn tại duy nhất một họ $(a_n(f))_{n \in \mathbf{Z}}$ các phần tử của F sao cho, với mọi tập compact H của U, họ $(a_n(f)z^n)_{n \in \mathbf{Z}}$ là cộng được đều với tổng $f(z)$ khi z chạy trên H (“khai triển Laurent”).

Giả sử thêm rằng $\lambda = 0$. Cấp của $f$ tại điểm $x = 0$ được định nghĩa là cận dưới lớn nhất (hữu hạn hoặc vô hạn) của tập hợp các số nguyên n sao cho $a_n(f) \neq 0$. Nếu tồn tại một lân cận V của 0 sao cho $f$ bị chặn trong $V - \{0\}$, thì f có cấp 0 tại điểm $x = 0$ và mở rộng bởi tính liên tục thành một hàm chỉnh hình trên tập mở $|z| < \mu$. Cho $p$ là một số nguyên $> 0$; nếu $f$ có cấp $-p$ tại điểm $x = 0$, người ta nói rằng 0 là một cực cấp p của f.

3.3.10. Giả sử rằng $E = \mathbf{C}$ và F là định chuẩn. Cho $f$ là một ánh xạ chỉnh hình từ đĩa đơn vị mở U của E vào F, sao cho $f(0) = 0$ và đặt $M = \sup_{z \in U} \|f(z)\|$. Khi đó $\|f(z)\| \leq M \cdot |z|$ với mọi $z \in U$ ("bổ đề Schwarz").

### 3.4. Các hàm giải tích thực

Giả sử rằng $K = \mathbf{R}$.

3.4.1. Cho U là một tập hợp mở của E và $f$ là một ánh xạ từ U vào F, được giả sử là tựa đầy đủ.

Các điều kiện sau là tương đương:
(i) $f$ là giải tích.
(ii) $f$ thuộc lớp $C^\infty$ và, với mọi $a \in U$, tồn tại một lân cận $V_a$ của $a$ và một số thực $M$ sao cho, với mọi bán chuẩn liên tục $\gamma$ trên F, tồn tại một hằng $A_\gamma$ sao cho ta có
$$
\|\Delta^\alpha f(x)\|_\gamma \leq A_\gamma M^{|\alpha|} \quad \text{với mọi } x \in V_a \text{ và mọi } \alpha \in \mathbf{N}^n.
$$

3.4.2. Cho U là một tập hợp mở của E và $f$ là một ánh xạ từ U vào F. Nếu F là tựa đầy đủ, và nếu đối ngẫu mạnh $F'$ của nó là một không gian Baire, thì $f$ là giải tích khi và chỉ khi $u \circ f$ là giải tích với mọi $u \in F'$.
