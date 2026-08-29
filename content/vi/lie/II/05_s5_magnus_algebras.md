---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: II
chapter_title: FREE LIE ALGEBRAS
section: 5
section_title: Magnus algebras
lang: vi
source: lie-i-iii
pdf_pages: 0167-0173, 0211-0219
extraction: ocr
subsections:
    - "no": 1
      title: MAGNUS ALGEBRAS
      page: 0
      pdf_page: 167
    - "no": 2
      title: MAGNUS GROUP
      page: 0
      pdf_page: 168
    - "no": 3
      title: MAGNUS GROUP AND FREE GROUP
      page: 0
      pdf_page: 169
    - "no": 4
      title: LOWER CENTRAL SERIES OF A FREE GROUP
      page: 0
      pdf_page: 170
    - "no": 5
      title: '*p*-Filtration of Free Groups'
      page: 0
      pdf_page: 172
statements: 14
exercises: 12
content_sha256: c115ac7d11730fe5d45fb64a998b0771ca638940f4496e118f89a0dc7611d8a7
translated_from: content/en/lie/II/05_s5_magnus_algebras.md
source_content_sha256: b447c834d904c0c1c87c668ee3a9a6c76b5fc3212a84bf648612ad2a0a49f556
translation_model: gpt-5.4
translation_run: translate-vi-e5cf4dff
glossary_version: 34
glossary_terms_sha256: 0d05d8f9043c61b814341524d44c7436fca0c07dc1f56335413a9373c3270530
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 5. ĐẠI SỐ MAGNUS

Trong đoạn này, X chỉ một tập hợp, F(X) nhóm tự do được xây dựng trên X (Đại số, Chương I, § 7, no. 5) và A(X) đại số kết hợp tự do được xây dựng trên X với phân bậc toàn phần $(A^n(X))_{n \geq 0}$ của nó (xem Đại số, Chương III, § 3, no. 1, Ví dụ 3). X được đồng nhất với các ảnh của nó trong F(X) và A(X).

### 1. ĐẠI SỐ MAGNUS

Cho $\hat{A}(X)$ là môđun tích $\prod_{n \geq 0} A^n(X)$. Ta định nghĩa trên $\hat{A}(X)$ một phép nhân theo quy tắc

$$
(a \cdot b)_n = \sum_{i=0}^n a_i \cdot b_{n-i}
$$

trong đó $a = (a_n)$ và $b = (b_n)$ thuộc $\hat{A}(X)$. Ta biết (Đại số giao hoán, Chương III, § 2, no. 12, Ví dụ 1) rằng $\hat{A}(X)$ là một đại số kết hợp và $A(X)$ được đồng nhất với đại số con của $\hat{A}(X)$ gồm các dãy mà mọi số hạng đều bằng không trừ ra một số hữu hạn số hạng.

$\hat{A}(X)$ được trang bị tôpô tích của các tôpô rời rạc trên các thừa số

A^n(X); tôpô này biến $\hat{A}(X)$ thành một đại số tôpô Hausdorff đầy đủ, khi vành K mang tôpô rời rạc, và $A(X)$ trù mật trong $\hat{A}(X)$

Cho $a = (a_n) \in \hat{A}(X)$; họ $(a_n)_{n \geq 0}$ là khả tổng và $a = \sum_{n \geq 0} a_n$.

Với mọi số nguyên $m \geq 0$, ký hiệu $\hat{A}_m(X)$ là iđêan gồm các chuỗi $a = \sum_{n \geq m} a_n$ sao cho $a_n \in A^n(X)$ với mọi $n \geq m$. Dãy các iđêan này là một hệ cơ bản các lân cận của 0 trong $\hat{A}(X)$ và một lọc nguyên trên $\hat{A}(X)$. Hàm cấp liên kết với lọc trên được ký hiệu bởi $\omega$; khi đó $\omega(0) = +\infty$ và $\omega(a) = m$ nếu $a = \sum_{n \geq m} a_n$ với $a_n \in A^n(X)$ với mọi $n \geq m$ và $a_m \neq 0$ (§ 4, nos. 1 and 2).

$\hat{A}(X)$ được gọi là *đại số Magnus* của tập hợp X với các hệ số trong K. Nếu có sự nhập nhằng nào về K thì ta viết $\hat{A}_K(X)$.

#### Mệnh đề 1 {#lie-ii-s5-prop-1 .statement}

*Cho B là một đại số kết hợp có đơn vị với một lọc thực $(B_\alpha)_{\alpha \in \mathbf{R}}$ sao cho B là Hausdorff và đầy đủ (§ 4, số 1 và 2). Cho f là một ánh xạ của X vào B sao cho tồn tại $\lambda > 0$ mà $f(X) \subset B_\lambda$. Khi đó f có thể được mở rộng theo một và chỉ một cách thành một đồng cấu có đơn vị liên tục $\hat{f}$ của $\hat{A}(X)$ vào B.*

Gọi $f'$ là đồng cấu đại số có đơn vị duy nhất của $A(X)$ vào B mở rộng $f$ (*Đại số*, Chương III, § 2, no. 7, Mệnh đề 7). Ta sẽ chỉ ra rằng $f'$ là *liên tục*: $f'(A^n(X)) \subset B_{n\lambda}$ do đó $f'(\hat{A}_n(X) \cap A(X)) \subset B_{n\lambda}$. Vì vậy $f'$ có thể được mở rộng theo một và chỉ một cách bằng tính liên tục thành một đồng cấu $\hat{f} : \hat{A}(X) \to B$.

Ta giữ nguyên các giả thiết và ký hiệu của Mệnh đề 1 và lấy $u \in \hat{A}(X)$. Phần tử $\hat{f}(u)$ được ký hiệu bởi $u((f(x))_{x \in X})$ và được gọi là *kết quả của việc thay các f(x) cho các x trong u*. Đặc biệt, $u((x)_{x \in X}) = u$. Bây giờ cho $u = (u_y)_{y \in Y}$ là một họ các phần tử của $\hat{A}_1(X)$ và cho $v \in \hat{A}(Y)$. Điều trên cho phép ta định nghĩa phần tử $v((u_y)_{y \in Y}) \in \hat{A}(X)$. Nó được ký hiệu bởi $v \circ u$. Vì $u_y((f(x))) \in B_\lambda$, nên các phần tử $u_y((f(x)))$ có thể được thay cho các y trong v. Khi đó các ánh xạ $v \mapsto (v \circ u)((f(x)))$ và $v \mapsto v((u_y((f(x))))))$ là hai đồng cấu liên tục của các đại số có đơn vị từ $\hat{A}(X)$ vào B, nhận cùng một giá trị $u_y((f(x)))$ tại phần tử $y \in Y$. Do đó (Mệnh đề 1)

$$
(v \circ u)((f(x))) = v((u_y((f(x))))))
$$

với mọi $v \in \hat{A}(Y)$.

### 2. NHÓM MAGNUS

Với mọi $a = (a_n)_{n \geq 0}$ trong $\hat{A}(X)$, phần tử $a_0$ của K sẽ được gọi là *số hạng hằng* của a và được ký hiệu bởi $\varepsilon(a)$. Công thức (1) cho thấy rằng $\varepsilon$ là một đồng cấu đại số từ $\hat{A}(X)$ vào K.

#### Bổ đề 1 {#lie-ii-s5-lem-1 .statement}

*Để một phần tử a của $\hat{A}(X)$ là khả nghịch, điều kiện cần và đủ là số hạng hằng của nó khả nghịch trong K.*

Nếu $a$ khả nghịch trong $\hat{\mathbf{A}}(\mathbf{X})$, thì $\varepsilon(a)$ khả nghịch trong $K$. Ngược lại, nếu $\varepsilon(a)$ khả nghịch trong $K$, tồn tại $u \in \hat{\mathbf{A}}_1(\mathbf{X})$ sao cho $a = \varepsilon(a)(1-u)$; ta viết $b = \left( \sum_{n \geq 0} u^n \right) \varepsilon(a)^{-1}$. Khi đó $ab = ba = 1$ và $a$ khả nghịch.

Tập hợp các phần tử của $\hat{\mathbf{A}}(\mathbf{X})$ có hệ số hằng bằng 1 do đó là một nhóm con của monoide nhân $\hat{\mathbf{A}}(\mathbf{X})$, gọi là *nhóm Magnus* được xây dựng trên $\mathbf{X}$ (đối với $K$). Trong chương này nó sẽ được ký hiệu là $\Gamma(\mathbf{X})$ hoặc đơn giản là $\Gamma$. Với mọi số nguyên $n \geq 1$, ta ký hiệu bởi $\Gamma_n$ tập hợp các $a \in \Gamma$ sao cho $\omega(a-1) \geq n$. Theo Mệnh đề 2 của § 4, no. 5, dãy $(\Gamma_n)_{n \geq 1}$ là một *bộ lọc trung tâm nguyên trên $\Gamma$*.

### 3. NHÓM MAGNUS VÀ NHÓM TỰ DO

#### Định lý 1 {#lie-ii-s5-thm-1 .statement}

*Cho $r$ là một ánh xạ từ $\mathbf{X}$ vào $\hat{\mathbf{A}}(\mathbf{X})$ sao cho $\omega(r(x)) \geq 2$ với mọi $x \in \mathbf{X}$. Đồng cấu duy nhất $g$ của nhóm tự do $F(\mathbf{X})$ vào nhóm Magnus $\Gamma(\mathbf{X})$ sao cho $g(x) = 1 + x + r(x)$ với mọi $x \in \mathbf{X}$ là đơn ánh.*

Trước hết ta chứng minh ba bổ đề.

#### Bổ đề 2 {#lie-ii-s5-lem-2 .statement}

*Cho $n$ là một số nguyên hữu tỉ khác không. Trong vành các chuỗi lũy thừa hình thức $K[[t]]$ ta viết $(1+t)^n = \sum_{j \geq 0} c_{j,n} t^j$. Tồn tại một số nguyên $j \geq 1$ sao cho $c_{j,n} \neq 0$.

Nếu $n > 0$, thì $c_{n,n} = 1$ theo công thức nhị thức.
Giả sử $n < 0$ và đặt $m = -n$. Nếu $c_{j,n} = 0$ với mọi $j \geq 1$, thì $(1+t)^n = 1$, do đó, lấy nghịch đảo, $(1+t)^m = 1$, điều này mâu thuẫn với công thức $c_{m,m} = 1$.*

#### Bổ đề 3 {#lie-ii-s5-lem-3 .statement}

*Cho $x_1, \ldots, x_s$ là các phần tử của $\mathbf{X}$ sao cho $s \geq 1$ và $x_i \neq x_{i+1}$ với $1 \leq i \leq s-1$; và cho $n_1, \ldots, n_s$ là các số nguyên hữu tỉ khác không. Khi đó phần tử $\prod_{i=1}^s (1+x_i)^{n_i}$ của $\hat{\mathbf{A}}(\mathbf{X})$ là $\neq 1$.*

Cho $m$ là một iđêan cực đại của $K$ và $k$ là trường $K/m$; gọi $p : \hat{\mathbf{A}}_K(\mathbf{X}) \to \hat{\mathbf{A}}_k(\mathbf{X})$ là đồng cấu liên tục duy nhất của các $K$-đại số có đơn vị sao cho $p(x) = x$ với $x \in \mathbf{X}$ (no. 1, Mệnh đề 1). Chỉ cần chứng minh rằng $p\left( \prod_{i=1}^s (1+x_i)^{n_i} \right) \neq 1$ và bài toán được quy về trường hợp $K$ là một trường.

Theo ký hiệu của Bổ đề 2:

$$
\prod_{i=1}^s (1+x_i)^{n_i} = \sum_{b_1 \geq 0} \cdots \sum_{b_s \geq 0} c_{b_1, n_1} \cdots c_{b_s, n_s} x_1^{b_1} \cdots x_s^{b_s}.
$$

Theo Bổ đề 2, tồn tại các số nguyên $a_i > 0$ sao cho $c_{a_i, n_i} \neq 0$ ($1 \leq i \leq s$). Theo *Đại số*, Chương I, § 7, no. 4, Mệnh đề 6, không có đơn thức nào $x_1^{b_1} \cdots x_s^{b_s}$ sao cho $b_i \geq 0$ và $(b_1, \ldots, b_s) \neq (a_1, \ldots, a_s)$ có thể bằng $x_1^{a_1} \ldots x_s^{a_s}$. Suy ra hệ số của $x_1^{a_1} \ldots x_s^{a_s}$ trong $\prod_{i=1}^s (1 + x_i)^{n_i}$ là $c_{a_1, n_1} \ldots c_{a_s, n_s} \neq 0$, điều này suy ra kết quả.

#### Bổ đề 4 {#lie-ii-s5-lem-4 .statement}

*Cho $\sigma$ là tự đồng cấu liên tục của $\hat{A}(X)$ sao cho $\sigma(x) = x + r(x)$ với mọi $x \in X$ (no. 1, Mệnh đề 1). Khi đó $\sigma$ là một tự đẳng cấu và $\sigma(\hat{A}_m(X)) = \hat{A}_m(X)$ với mọi $m \in \mathbf{N}$.

$\sigma(x) \equiv x \mod \hat{A}_2(X)$ với $x \in X$, do đó, với $n \geq 1$ và $x_1, \ldots, x_n$ trong $X$,
$$
\sigma(x_1) \ldots \sigma(x_n) \equiv x_1 \ldots x_n \mod \hat{A}_{n+1}(X);
$$
theo tính tuyến tính suy ra rằng $\sigma(a) \equiv a$ modulo $\hat{A}_{n+1}(X)$ với mọi $a \in A^n(X)$ và đặc biệt $\sigma(A^n(X)) \subset \hat{A}_n(X)$. Suy ra $\sigma(A^n(X)) \subset \hat{A}_n(X)$ với $m \geq n$, do đó $\sigma(\hat{A}_n(X)) \subset \hat{A}_n(X)$. Nói cách khác, $\sigma$ tương thích với phép lọc $(\hat{A}_m(X))$ trên $A(X)$ và hạn chế của nó lên vành phân bậc liên kết là đồng nhất. Vậy $\sigma$ là song ánh (*Đại số giao hoán*, chương III, § 2, no. 8, hệ quả 3 của định lý 1).

Cuối cùng ta chứng minh Định lý 1. Cho $w \neq 1$ là một phần tử của $F(X)$. Theo *Đại số*, Chương I, § 7, no. 5, Mệnh đề 7, tồn tại các $x_1, \ldots, x_s$ trong $X$ và các số nguyên hữu tỉ khác không $n_1, \ldots, n_s$ sao cho $s \geq 1$, $x_i \neq x_{i+1}$ ($1 \leq i \leq s-1$) và
$$
w = x_1^{n_1} \ldots x_s^{n_s}.
$$
Theo ký hiệu của Bổ đề 4,
$$
g(w) = \prod (1 + \sigma(x_i))^{n_i} = \sigma(\prod (1 + x_i)^{n_i}),
$$
do đó $g(w) \neq 1$ theo các Bổ đề 3 và 4.

### 4. CHUỖI TRUNG TÂM GIẢM CỦA MỘT NHÓM TỰ DO

Ta sẽ chứng minh hai định lý sau đây:

#### Định lý 2 {#lie-ii-s5-thm-2 .statement}

*Giả sử rằng trong vành $K$ quan hệ $n.1 = 0$ kéo theo $n = 0$ với mọi số nguyên $n$. Gọi $r$ là một ánh xạ từ $X$ vào $\hat{A}(X)$ sao cho $\omega(r(x)) \geq 2$ với $x \in X$ và gọi $g$ là đồng cấu từ $F(X)$ vào nhóm Magnus $\Gamma(X)$ sao cho $g(x) = 1 + x + r(x)$ với $x \in X$. Với mọi $n \geq 1$, $C^n F(X)$ là ảnh ngược theo $g$ của nhóm con $1 + \hat{A}_n(X)$ của $\Gamma(X)$.*

#### Định lý 3 {#lie-ii-s5-thm-3 .statement}

*Với mọi $x \in X$, gọi $c(x)$ là ảnh chính tắc của $x$ trong $F(X)/(F(X), F(X))$. Gọi $g$ là đại số Lie phân bậc trên $\mathbf{Z}$ liên kết với bộ lọc $(C^n F(X))_{n \geq 1}$ của $F(X)$ (§ 4, no. 6). Đồng cấu duy nhất của đại số Lie tự do trên $\mathbf{Z}$ $L_\mathbf{Z}(X)$ vào $g$ mở rộng $c$ là một đẳng cấu.*

Nói một cách lỏng lẻo, đại số Lie phân bậc trên $\mathbf{Z}$ liên kết với nhóm tự do $F(X)$ (với chuỗi trung tâm dưới) là đại số Lie tự do trên $\mathbf{Z}$ $L_\mathbf{Z}(X)$.

Ta viết $F(X) = F, \Gamma(X) = \Gamma, \hat{A}(X) = \hat{A}, \hat{A}_\mathbf{Z}(X) = \hat{A}_\mathbf{Z}, C^n F(X) = C^n, \Gamma_n = 1 + \hat{A}_n(X)$ và gọi $\alpha : L_\mathbf{Z}(X) \to g$ là đồng cấu được đưa vào trong mệnh đề của Định lý 3.

(A) Các rút gọn sơ bộ.

Ký hiệu $\gamma$ là đồng cấu từ $F$ vào $\Gamma$ được xác định bởi $\gamma(x) = 1 + x$ với $x \in X$. Theo Bổ đề 4, tồn tại một tự đẳng cấu $\sigma$ của đại số $\hat{A}$ tương thích với lọc trên $\hat{A}$ và sao cho $\sigma(1 + x) = g(x)$ với mọi $x \in X$; khi đó $\sigma(\Gamma_n) = \Gamma_n$ với mọi $n$. Vì các đồng cấu $g$ và $\sigma \circ \gamma$ từ $F$ vào $\Gamma$ trùng nhau trên $X, g = \sigma \circ \gamma$ và do đó $g^{-1}(\Gamma_n) = \gamma^{-1}(\Gamma_n)$. Dưới các giả thiết của Định lý 2, $\mathbf{Z}$ có thể được đồng nhất với một vành con của $K$; vì thế đại số Magnus $\hat{A}_\mathbf{Z}$ được đồng nhất với một vành con của $\hat{A}$ và lọc trên $\hat{A}_\mathbf{Z}$ được cảm sinh bởi lọc trên $\hat{A}$. Vì $\gamma$ ánh xạ $F$ vào $\hat{A}_\mathbf{Z}$, ta thấy rằng chỉ cần chứng minh các Định lý 2 và 3 dưới các giả thiết bổ sung $K = \mathbf{Z}, r = 0$ và do đó $g = \gamma$, những giả thiết mà từ nay về sau ta sẽ đặt ra.

(B) Tính toàn ánh của $\alpha$.

Vì $X$ sinh nhóm $F = C^1$, nên tập hợp $c(X)$ sinh $\mathbf{Z}$-môđun $g^1 = C^1/C^2$. Nhưng $g^1$ sinh đại số Lie trên $\mathbf{Z}$ $g$ (§ 4, no. 6, Mệnh đề 5), và do đó $c(X)$ sinh $g$, điều này chứng minh rằng $\alpha$ là toàn ánh.

(C) Ta đồng nhất đại số phân bậc $\mathrm{gr}(\hat{A})$ với $A(X)$ dưới các đẳng cấu chính tắc $A^n(X) \to \hat{A}_n/\hat{A}_{n+1}$. Với mọi số nguyên $n \geq 1$, ta đặt $F^n = \gamma^{-1}(\Gamma_n)$; ta biết (§ 4, no. 5) rằng $(F^n)_{n \geq 1}$ là một lọc trung tâm nguyên trên $F$. Ký hiệu $g'$ là đại số Lie $\mathbf{Z}$ phân bậc liên kết (§ 4, no. 4). Gọi $f$ là đồng cấu đại số Lie từ $g'$ vào $A(X)$ liên kết với $\gamma$ (§ 4, no. 5, Mệnh đề 3). Bây giờ $C^n \subset F^n$ với mọi số nguyên $n \geq 1$ (§ 4, no. 6, Mệnh đề 4) và do đó có một đồng cấu chính tắc $\varepsilon$ từ $g = \bigoplus_{n \geq 1} C^n/C^{n+1}$ vào $g' = \bigoplus_{n \geq 1} F^n/F^{n+1}$

$$
L_\mathbf{Z}(X) \xrightarrow{\alpha} g \xrightarrow{\varepsilon} g' \xrightarrow{f} A(X).
$$

Ta viết $\beta = f \circ \varepsilon$; ta cho $\beta$ một cách tường minh như sau: nếu $u$ là lớp modulo $C^{n+1}$ của một phần tử $w$ của $C^n$, thì $\gamma(w) - 1$ có cấp $\geq n$ trong $\hat{A}$ và $\beta(u)$ là thành phần thuần nhất của $\gamma(w) - 1$ có bậc $n$. Đặc biệt,

$$
\beta(c(x)) = x \quad \text{với mọi } x \in X.
$$

(D) Chứng minh của Định lý 2 và 3.

Đồng cấu đại số Lie $\beta \circ \alpha : L_\mathbf{Z}(X) \to A(X)$ hạn chế trên $X$ là đồng nhất theo (3) và do đó là đơn ánh chính tắc (§ 3, no. 1). Vì thế $\alpha$ là đơn ánh và do đó song ánh theo (B); điều này chứng minh Định lý 3. Vì $\beta \circ \alpha = f \circ \varepsilon \circ \alpha$ là đơn ánh và $\alpha$ là song ánh, nên $\varepsilon$ là đơn ánh. Với mọi $n \geq 1$,

$$
\varepsilon_n : C^n/C^{n+1} \to F^n/F^{n+1}
$$

là đơn ánh và do đó

$$
C^n \cap F^{n+1} = C^{n+1}.
$$

C^1 = F = F^1; nếu C^n = F^n, thì C^n \cap F^{n+1} = F^{n+1} do đó C^{n+1} = F^{n+1}
điều này chứng minh Định lý 2 bằng quy nạp theo n \geqslant 1.

#### Hệ quả {#lie-ii-s5-n4-cor-1 .statement}

$$
\bigcap_{n \geqslant 1} C^n F(X) = \{e\}.
$$

Áp dụng Định lý 2 với K = \mathbf{Z} và r = 0,
$$
\bigcap_{n \geqslant 1} C^n F(X) = \bigcap_{n \geqslant 1} g^{-1}(1 + \hat{A}_n(X)) = g^{-1}\left(\bigcap_{n \geqslant 1} (1 + \hat{A}_n(X))\right) = g^{-1}(1) = \{e\}.
$$

#### Nhận xét {#lie-ii-s5-n4-rem-1 .statement}

Cho H là một tập Hall đối với X (§ 2, no. 10). Cho M là magma được xác định bởi luật hợp thành (x, y) \mapsto (x, y) = x^{-1}y^{-1}xy trên F(X) và cho $\phi$ là đồng cấu từ M(X) vào M mà hạn chế của nó trên X là đồng nhất. Các phần tử của $\phi(H)$ được gọi là các *giao hoán tử cơ bản* của F(X) liên kết với tập Hall H. Với mọi số nguyên n \geqslant 1, cho H_n là tập con của H gồm các phần tử có độ dài n; ta biết (§ 2, no. 11, Định lý 1) rằng ánh xạ chính tắc của H_n vào L_\mathbf{Z}(X) là một cơ sở của nhóm Abel L_\mathbf{Z}^n(X). Hơn nữa, $\phi(H_n) \subset C^n$; với mọi m \in H_n, cho $\phi_n(m)$ ký hiệu lớp mod. C^{n+1} của $\phi(m) \in C^n$. Khi đó Định lý 3 cho thấy rằng $\phi_n$ là *một song ánh từ H_n lên một cơ sở của nhóm Abel* C^n/C^{n+1}. Suy ra ngay lập tức rằng, với mọi w \in F(X) và mọi i \geqslant 1, tồn tại một phần tử duy nhất $\alpha_i$ của $\mathbf{Z}^{(H_i)}$ sao cho, với n \geqslant 1,

$$
w = \prod_{i=1}^n \prod_{m \in H_i} \phi(m)^{\alpha_i(m)} \mod. C^{n+1},
$$

trong đó tích được tính theo thứ tự toàn phần đã cho trên H.

#### Ví dụ {#lie-ii-s5-n4-exa-1 .statement}

Giả sử rằng X là một tập hợp có hai phần tử x, y và cho H_1 = \{x, y\}, H_2 = \{xy\}. Do đó mọi phần tử w của F(X) đều có thể viết được
$$
w \equiv x^a y^b (x, y)^c \mod. C^3 \quad \text{với } a, b, c \text{ trong } \mathbf{Z}.
$$
Với w = (xy)^n, ta có a = b = n và c = n(1 - n)/2 (xem Bài tập 9), do đó
$$
(xy)^n \equiv x^n y^n (x, y)^{n(1-n)/2} \mod. C^3.
$$

### 5. Bộ lọc *p* của các nhóm tự do

Trong số này, *p* ký hiệu một số nguyên tố và ta giả thiết rằng K = \mathbf{F}_p. Gọi $\gamma$ là đồng cấu từ F(X) vào $\Gamma(X)$ được xác định bởi $\gamma(x) = 1 + x$ với mọi x trong X; ta viết $F_n^{(p)}(X) = \gamma^{-1}(1 + \hat{A}_n(X))$. Dãy $(F_n^{(p)}(X))_{n \geqslant 1}$ là một bộ lọc trung tâm nguyên trên F(X), và là *tách được* vì $\gamma$ là đơn ánh (no. 3, Định lý 1). Nó được gọi là bộ lọc *p* trên F(X).

#### Mệnh đề 2 {#lie-ii-s5-prop-2 .statement}

*Giả sử rằng X là hữu hạn. Với mọi số nguyên n \geqslant 1, nhóm F(X)/F_n^{(p)}(X) là một p-nhóm hữu hạn có lớp lũy linh \leqslant n.*

Lập luận bằng quy nạp theo $n$, chỉ cần chứng minh rằng $F_n^{(p)}(X)/F_{n+1}^{(p)}(X)$ là một $p$-nhóm giao hoán hữu hạn với mọi $n \geqslant 1$. Với mọi $w \in F_n^{(p)}(X)$, phần tử $\gamma(w) - 1$ của $\hat{A}(X)$ có cấp $\geqslant n$; ta ký hiệu bởi $\delta_n(w)$ thành phần thuần nhất của $\gamma(w) - 1$ có bậc $n$. Ánh xạ $\delta_n : F_n^{(p)}(X) \to A^n(X)$ là một đồng cấu với hạt nhân $F_{n+1}^{(p)}(X)$ (§ 4, no. 5, Mệnh đề 3) và do đó $F_n^{(p)}(X)/F_{n+1}^{(p)}(X)$ đẳng cấu với một nhóm con của $A^n(X)$. Vì $X$ là hữu hạn, $A^n(X)$ là một không gian vectơ hữu hạn chiều trên $\mathbf{F}_p$ và do đó là một $p$-nhóm giao hoán hữu hạn, và vì thế $F_n^{(p)}(X)/F_{n+1}^{(p)}(X)$ cũng vậy.

#### Mệnh đề 3 {#lie-ii-s5-prop-3 .statement}

*Với mọi $w \neq 1$ trong $F(X)$, tồn tại một $p$-nhóm hữu hạn $G$ và một đồng cấu $f$ của $F(X)$ vào $G$ sao cho $f(w) \neq 1$.*

Tồn tại các phần tử $x_1, \ldots, x_r$ của $X$ và các số nguyên $n_1, \ldots, n_r$ sao cho $w = x_1^{n_1} \ldots x_r^{n_r}$. Đặt $Y = \{x_1, \ldots, x_r\}$. Đơn ánh chính tắc của $Y$ vào $X$ kéo dài thành một đồng cấu $\alpha : F(Y) \to F(X)$; mặt khác, gọi $\beta$ là đồng cấu của $F(X)$ vào $F(Y)$ mà hạn chế trên $Y$ là đồng nhất và ánh xạ $X - Y$ vào $\{1\}$. Khi đó $\beta(\alpha(y)) = y$ với $y \in Y$ và do đó $\beta \circ \alpha$ là tự đẳng cấu đồng nhất của $F(Y)$. Hiển nhiên tồn tại $w'$ trong $F(Y)$ sao cho $w = \alpha(w')$; khi đó $\beta(w) = w' \neq 1$; mà $\bigcap_{n \geqslant 1} F_n^{(p)}(Y) = \{1\}$ và vì vậy tồn tại một số nguyên $n \geqslant 1$ sao cho $\beta(w) \notin F_n^{(p)}(Y)$. Theo Mệnh đề 2, nhóm $G = F(Y)/F_n^{(p)}(Y)$ là một $p$-nhóm hữu hạn. Nếu $f$ là hợp thành của $\beta$ với đồng cấu chính tắc của $F(Y)$ lên $G$, thì $f(w) \neq 1$.

#### Hệ quả {#lie-ii-s5-n5-cor-1 .statement}

*Giao của các nhóm con chuẩn có chỉ số hữu hạn trong $F(X)$ là $\{1\}$.*

### Bài tập {#lie-ii-s5-exercises}

Trong các bài tập sau đây, ta giả sử các giả thiết và ký hiệu của § 5. $F$ ký hiệu nhóm tự do $F(X)$ và $g$ ký hiệu đồng cấu duy nhất của $F$ vào nhóm Magnus $\Gamma(X)$ sao cho $g(x) = 1 + x$ với mọi $x \in X$ (x. Định lý 1).

Xem [bài tập của § 5](exercises/s5/).
