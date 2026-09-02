---
book: var
book_title: Variétés différentielles et analytiques
chapter: "1"
chapter_title: VARIÉTÉS DIFFÉRENTIELLES ET ANALYTIQUES, FASCICULE DE RÉSULTATS
section: 0
section_title: Polynômes-continus et séries formelles
appendix: true
lang: vi
source: var-fr
pdf_pages: 0086-0087
extraction: ocr
statements: 0
exercises: 0
content_sha256: ac5950f295f673d6f4380138039a8dbfb0c01a67a4284f4b58fcc16ebfe80939
translated_from: content/en-mt/var/1/A_a_polynomes_continus_et_series_formelles.md
source_lang: en-mt
translation_method: machine
source_content_sha256: 505abbfb6816269691d0798e92465645c01c3fa2d2c2d5b72db26a6a2931f5c6
translation_model: gpt-5.4
translation_run: translate-vi-72d599e5
glossary_version: 34
glossary_terms_sha256: 6b02e80453e78fb31cacfaefb7b919a1df39d8103381383c308f6a7094ebe131
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## PHỤ LỤC

# Đa thức liên tục và chuỗi hình thức

Trong Phụ lục này, F ký hiệu một không gian đa chuẩn tách biệt trên K, $E_i$ (với $1 \leq i \leq n$) một không gian chuẩn trên K và E là tích không gian vectơ tôpô của các $E_i$.

Với $\alpha \in \mathbf{N}^n$, và $1 \leq j \leq |\alpha|$, ta đặt:

$$
\alpha(j) = \inf \{ k \in \mathbf{N} \mid 1 \leq k \leq n \text{ và } j > \alpha_1 + \cdots + \alpha_{k-1} \}
$$

(vì thế dãy các $\alpha(j)$ được thu được bằng cách viết $\alpha_1$ lần 1, ..., $\alpha_n$ lần n).

Ta ký hiệu bởi $E_\alpha$ tích không gian vectơ tôpô của họ các $E_{\alpha(j)}$ với $1 \leq j \leq |\alpha|$. Ta ký hiệu bởi $\mathrm{Hom}_\alpha(E_1, \ldots, E_n; F)$ không gian các ánh xạ $|\alpha|$-tuyến tính từ $E_\alpha$ vào F và bởi $\mathcal{L}_\alpha(E_1, \ldots, E_n; F)$ không gian con của $\mathrm{Hom}_\alpha(E_1, \ldots, E_n; F)$ tạo bởi các ánh xạ đa tuyến tính liên tục được trang bị tôpô hội tụ đều trên các tập hợp bị chặn của $E_\alpha$; đó là một không gian đa chuẩn tách biệt, mà tôpô có thể được xác định bởi họ các nửa chuẩn $\|u\|_y$, trong đó, với một nửa chuẩn liên tục y trên F, ta ký hiệu bởi $\|u\|_y$ cận dưới lớn nhất của các số $a \geq 0$ sao cho

$$
\|u(x_1, \ldots, x_{|\alpha|})\|_y \leq a \|x_1\| \cdots \|x_{|\alpha|}\|
$$

trong đó mỗi $x_j$ chạy qua $E_{\alpha(j)}$.

Ta ký hiệu bởi $p_i$ phép chiếu chính tắc của E lên $E_i$. Với $\alpha \in \mathbf{N}^n$ và $\alpha \neq 0$, ta ký hiệu bởi $p_\alpha$ ánh xạ $x \mapsto (p_{\alpha(j)}(x))$ từ E vào $E_\alpha$.

A.1. Một ánh xạ $f$ từ E vào F được gọi là một đa thức đa thuần nhất có đa bậc $\alpha$ (với $\alpha \in \mathbf{N}^n$) trên E nhận giá trị trong F nếu tồn tại một phần tử

$$
u \in \mathrm{Hom}_\alpha(E_1, \ldots, E_n; F)
$$

sao cho $f = u \circ p_\alpha$.

A.2. Ta ký hiệu bởi $P_\alpha(E_1, \ldots, E_n; F)$ ảnh của $\mathcal{L}_\alpha(E_1, \ldots, E_n; F)$ bởi ánh xạ tuyến tính $u \mapsto u \circ p_\alpha$ từ $\mathrm{Hom}_\alpha(E_1, \ldots, E_n; F)$ vào không gian các ánh xạ từ E vào F, được trang bị tôpô thương của tôpô trên $\mathcal{L}_\alpha(E_1, \ldots, E_n; F)$. Một phần tử của $P_\alpha(E_1, \ldots, E_n; F)$ được gọi là một đa thức đa thuần nhất liên tục có đa bậc $\alpha$ trên E nhận giá trị trong F. Tôpô của $P_\alpha(E_1, \ldots, E_n; F)$ được xác định bởi họ các nửa chuẩn:

$$
\|f\|_y = \inf_{u \in \mathcal{L}_\alpha(E_1, \ldots, E_n; F), f = u \circ p_\alpha} \|u\|_y
$$

với $y$ mô tả tập hợp các nửa chuẩn liên tục trên F. Nếu F là một không gian chuẩn, có chuẩn $\gamma$, ta viết $\|f\|$ thay cho $\|f\|_y$. Không gian $P_\alpha(E_1, \ldots, E_n; F)$ và tôpô của nó không thay đổi nếu thay các chuẩn đã cho trên mỗi $E_i$ bằng các chuẩn tương đương. Vì thế chúng có thể được xác định khi các $E_i$ là các không gian vectơ tôpô khả chuẩn.

Đặc biệt, một phần tử của $P_k(E; F)$ được gọi là một đa thức thuần nhất liên tục có tổng bậc $k$ trên E nhận giá trị trong F. Không gian $P_k(E; F)$ là tổng trực tiếp tôpô của các không gian $P_\alpha(E_1, \ldots, E_n; F)$ với $|\alpha| = k$. Không gian $P_0(E; F)$ là không gian các ánh xạ hằng từ E vào F và được đồng nhất với F.

A.3. Ta ký hiệu bởi $P(E; F)$ hoặc $P(E_1, \ldots, E_n; F)$ không gian con vectơ của không gian vectơ tất cả các ánh xạ từ E vào F được sinh bởi các không gian con $P_k(E; F)$.

Nó là tổng trực tiếp của các không gian con $P_\alpha(E_1, \ldots, E_n; F)$ với $\alpha \in \mathbf{N}^n$, và cũng là tổng trực tiếp của các không gian con $P_k(E; F)$ với $k \in \mathbf{N}$. Một phần tử của $P(E; F)$ được gọi là một *đa thức liên tục* trên $E$ với giá trị trong $F$.

A.4. Cho $G_j$ là các không gian định chuẩn (với $1 \leq j \leq m$). Cho $f_j \in P(E_1, \ldots, E_n; G_j)$ (với $1 \leq j \leq m$) và cho $g \in P(G_1, \ldots, G_m; F)$. Ánh xạ
$$
h : x \mapsto g(f_1(x), \ldots, f_m(x))
$$
thuộc $P(E_1, \ldots, E_n; F)$. Hơn nữa, nếu $f_j \in P_\alpha(E_1, \ldots, E_n; G_j)$ với $1 \leq j \leq m$ (với $\alpha \in \mathbf{N}^n$) và $g \in P_\beta(G_1, \ldots, G_m; F)$, (với $\beta \in \mathbf{N}^m$), thì ta có $h \in P_{|\beta| \alpha}(E_1, \ldots, E_n; F)$ và
$$
\|h\|_\gamma \leq \|g\|_\gamma \cdot \|f\|^\beta
$$
với mọi nửa chuẩn liên tục $\gamma$ trên $F$ (đặt $\|f\|^\beta = \prod_{1 \leq j \leq m} \|f_j\|^{\beta_j}$).

A.5. Ta ký hiệu bởi $\hat{P}(E_1, \ldots, E_n; F)$ không gian vectơ tích của các $P_\alpha(E_1, \ldots, E_n; F)$ với $\alpha \in \mathbf{N}^n$, được trang bị tôpô tích của các tôpô *rời rạc* trên từng nhân tử. Tôpô này làm cho $\hat{P}(E_1, \ldots, E_n; F)$ trở thành một nhóm tôpô tách biệt *và đầy đủ*. Ánh xạ tuyến tính từ $P(E_1, \ldots, E_n; F)$ vào $\hat{P}(E_1, \ldots, E_n; F)$ kéo dài các đơn ánh chính tắc của các $P_\alpha(E_1, \ldots, E_n; F)$ là đơn ánh và ảnh của nó trù mật trong $\hat{P}(E_1, \ldots, E_n; F)$: nói chung người ta đồng nhất một đa thức liên tục trên $E$ với giá trị trong $F$ với ảnh của nó trong $\hat{P}(E_1, \ldots, E_n; F)$.

Ánh xạ đồng nhất của $P(E_1, \ldots, E_n; F) = P(E; F)$ kéo dài bởi tính liên tục thành một đẳng cấu của $\hat{P}(E_1, \ldots, E_n; F)$ lên $\hat{P}(E; F)$.

Một phần tử của $\hat{P}(E_1, \ldots, E_n; F)$ được gọi là một *chuỗi hình thức với các thành phần liên tục* (hoặc, do lạm dụng ngôn ngữ, một chuỗi *hình thức*) trên tích của các $E_i$ với giá trị trong $F$.

A.6. Cho $G_j$ (với $1 \leq j \leq m$) là các không gian định chuẩn và cho $g \in P(G_1, \ldots, G_m; F)$. Ánh xạ $f \mapsto g \circ f$ từ $\prod_{1 \leq j \leq m} P(E_1, \ldots, E_n; G_j)$ vào $P(E_1, \ldots, E_n; F)$ kéo dài bởi tính liên tục thành một ánh xạ (vẫn ký hiệu là $f \mapsto g \circ f$) từ $\prod_{1 \leq j \leq m} \hat{P}(E_1, \ldots, E_n; G_j)$ vào $\hat{P}(E_1, \ldots, E_n; F)$.

Cho $f_j = (f_{j,\alpha})_{\alpha \in \mathbf{N}^n} \in \hat{P}(E_1, \ldots, E_n; G_j)$, với $f_{j,0} = 0$. Đặt $f = (f_j)$: ánh xạ $g \mapsto g \circ f$ từ $P(G_1, \ldots, G_m; F)$ vào $\hat{P}(E_1, \ldots, E_n; F)$ được mở rộng bởi tính liên tục thành một ánh xạ (cũng được ký hiệu là $g \mapsto g \circ f$) từ $\hat{P}(G_1, \ldots, G_m; F)$ vào $\hat{P}(E_1, \ldots, E_n; F)$.
