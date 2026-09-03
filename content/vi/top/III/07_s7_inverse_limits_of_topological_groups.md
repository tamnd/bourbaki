---
book: top
book_title: General Topology
chapter: III
chapter_title: Topological Groups
section: 7
section_title: Inverse limits of topological groups and rings
lang: vi
source: top-i-iv
pdf_pages: 0290-0301, 0330-0332
extraction: ocr
subsections:
    - "no": 1
      title: INVERSE LIMITS OF ALGEBRAIC STRUCTURES
      page: 0
      pdf_page: 290
    - "no": 2
      title: INVERSE LIMITS OF TOPOLOGICAL GROUPS AND SPACES WITH OPERATORS
      page: 0
      pdf_page: 292
    - "no": 3
      title: APPROXIMATION OF TOPOLOGICAL GROUPS
      page: 0
      pdf_page: 295
    - "no": 4
      title: APPLICATION TO INVERSE LIMITS
      page: 0
      pdf_page: 299
statements: 15
exercises: 5
content_sha256: a6dfcd574f347ce55ec55811aa6d0f75c062c6be581d851776e057893b66d603
translated_from: content/en/top/III/07_s7_inverse_limits_of_topological_groups.md
source_content_sha256: da72beb407a42503880dae63dda66a50e3bc4b2d19533c7e937095d250c0e5cd
translation_model: gpt-5.4-mini
translation_run: translate-vi-64f04776
glossary_version: 34
glossary_terms_sha256: fcdc57ab36366f46addd8420492dc0b4b4d7881f70355ba018cd99fbfbe44a53
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 7. GIỚI HẠN NGƯỢC CỦA CÁC NHÓM TÔPÔ VÀ VÀNH

Trong toàn tiết này, I ký hiệu một tập có hướng (*) không rỗng và $\alpha \leq \beta$ ký hiệu quan hệ thứ tự bộ phận trong I. Trừ khi có tuyên bố rõ ràng ngược lại, mọi hệ ngược được xét đều được chỉ số hóa bởi I.

### 1. GIỚI HẠN NGƯỢC CỦA CÁC CẤU TRÚC ĐẠI SỐ

Cho $(X_\alpha, f_{\alpha \beta})$ là một hệ ngược của các tập hợp, và giả sử rằng mỗi $X_\alpha$ được trang bị một luật hợp thành nội tại, xác định mọi nơi, và được viết theo phép nhân. Giả sử thêm rằng các $f_{\alpha \beta}$ là các đồng cấu đối với các luật nội tại này. Vì

$$
f_{\alpha \beta}(x_\beta \cdot y_\beta) = f_{\alpha \beta}(x_\beta) \cdot f_{\alpha \beta}(y_\beta)
$$

mỗi khi $\alpha \leq \beta$ và $x_\beta$ cùng $y_\beta$ thuộc $X_\beta$, thì rõ ràng $X = \varprojlim X_\alpha$ là một tập con ổn định của tích $\prod_\alpha X_\alpha$, đối với luật nội tại

$$
(x_\alpha) \cdot (y_\alpha) = (x_\alpha \cdot y_\alpha).
$$

Cho $(\Lambda_\alpha, \varphi_{\alpha \beta})$ là một hệ ngược khác của các tập hợp, được chỉ số hóa bởi I, và giả sử rằng mỗi $X_\alpha$ mang một luật hợp thành ngoại tại, xác định mọi nơi, được viết theo phép nhân và có $\Lambda_\alpha$ làm tập hợp các toán tử, sao cho mỗi khi $\alpha \leq \beta$ ta có

$$
f_{\alpha \beta}(\lambda_\beta \cdot x_\beta) = \varphi_{\alpha \beta}(\lambda_\beta) \cdot f_{\alpha \beta}(x_\beta)
$$

cho $\lambda_\beta \in \Lambda_\beta$ và $x_\beta \in X_\beta$. Khi đó ta có thể định nghĩa một luật ngoại tại trên $\prod_\alpha X_\alpha$, có $\prod_\alpha \Lambda_\alpha$ làm tập hợp các toán tử, bằng cách đặt $(\lambda_\alpha) \cdot (x_\alpha) = (\lambda_\alpha \cdot x_\alpha)$; khi giới hạn tập hợp các toán tử xuống $\Lambda = \varprojlim \Lambda_\alpha$, ta có một luật ngoại tại trên $\prod_\alpha X_\alpha$ đối với luật đó $X$ lại là một tập con ổn định. Luật nội tại (tương ứng ngoại tại) được định nghĩa như vậy trên $X$ được gọi là giới hạn ngược của các luật nội tại (tương ứng ngoại tại) của các $X_\alpha$. Trong trường hợp các luật ngoại tại, có thể xảy ra rằng mọi $\Lambda_\alpha$ đều đồng nhất với cùng một tập $\Lambda_0$ và

(*) Người đọc có thể dễ dàng kiểm tra rằng phần lớn các định nghĩa và kết quả đứng trước Mệnh đề 1 trong tiết này vẫn đúng nếu I chỉ đơn thuần là có thứ tự bộ phận.

rằng mọi $\varphi_{\alpha \beta}$ đều là các ánh xạ đồng nhất; khi đó, vì I là một tập có hướng, $\Lambda$ có thể được đồng nhất với $\Lambda_0$.

Ta kiểm tra ngay được rằng các tính chất thông thường của tính kết hợp, tính giao hoán, sự tồn tại của phần tử đơn vị cho một luật nội tại (với điều kiện các $f_{\alpha \beta}$ gửi phần tử đơn vị thành phần tử đơn vị), tính phân phối của một luật ngoại tại đối với một luật nội tại, v.v., được bảo toàn khi chuyển sang giới hạn ngược.

Cho $\Sigma$ là một loài cấu trúc đại số và cho $\Sigma_0$ là cấu trúc *bần cùng* tương ứng với $\Sigma$. Mỗi khi chúng ta nói đến một hệ ngược của các tập hợp $(X_\alpha, f_{\alpha \beta})$ được trang bị các cấu trúc thuộc loài $\Sigma$, ta luôn luôn giả sử rằng các $f_{\alpha \beta }$ là *đồng cấu* đối với các cấu trúc này. Nếu ta trang bị cho $X = \varprojlim X_\alpha$ các luật nội tại và ngoại tại là các giới hạn ngược tương ứng của các luật nội tại và ngoại tại của các $X_\alpha$, thì $X$ mang một cấu trúc đại số của *loài* $\Sigma_0$. Tự nhiên, trong mỗi trường hợp cụ thể vẫn phải xem cấu trúc này có thuộc loài $\Sigma$ hay không.

Chẳng hạn, nếu $(G_\alpha, f_{\alpha \beta})$ là một hệ ngược của các nhóm (tương ứng vành), thì $\varprojlim G_\alpha$ là một nhóm con (tương ứng vành con) của $\prod_\alpha G_\alpha$, và được gọi là giới hạn *ngược* của hệ $(G_\alpha, f_{\alpha \beta})$ các nhóm (tương ứng vành).

Cho $(X_\alpha, g_{\alpha \beta})$ là một hệ ngược của các tập hợp và cho $(G_\alpha, f_{\alpha \beta})$ là một hệ ngược của các nhóm; giả sử rằng mỗi $X_\alpha$ có $G_\alpha$ làm nhóm toán tử và rằng mỗi khi $\alpha \leq \beta$ ta có

(I)
$$
g_{\alpha \beta}(s_\beta \cdot x_\beta) = f_{\alpha \beta}(s_\beta) \cdot g_{\alpha \beta}(x_\beta)
$$
với $x_\beta \in X_\beta$ và $s_\beta \in G_\beta$. Khi đó $X = \varprojlim X_\alpha$ có $G = \varprojlim G_\alpha$ là nhóm tác động. Từ (I) suy ra rằng, nếu $\alpha \leq \beta$, các ánh xạ $f_{\alpha \beta}$ và $g_{\alpha \beta}$ tương thích (§ 2, no. 4) và do đó xác định một ánh xạ $\varphi_{\alpha \beta} : X_\beta / G_\beta \to X_\alpha / G_\alpha$ của các tập thương, sao cho $(X_\alpha / G_\alpha, \varphi_{\alpha \beta})$ là một hệ ngược. Hơn nữa, nếu $f_\alpha : G \to G_\alpha$ và $g_\alpha : X \to X_\alpha$ là các ánh xạ chính tắc, thì $f_\alpha$ và $g_\alpha$ tương thích và do đó xác định một ánh xạ $h_\alpha : X / G \to X_\alpha / G_\alpha$ của các tập thương; rõ ràng các $h_\alpha$ tạo thành một hệ ngược các ánh xạ, mà giới hạn ngược của nó do đó là một ánh xạ $h : X / G \to \varprojlim X_\alpha / G_\alpha$, *không nhất thiết là đơn ánh hay toàn ánh* (Bài tập 1).

Lại nữa, cho $(A_\alpha, \varphi_{\alpha \beta})$ là một hệ ngược các vành và cho $(M_\alpha, f_{\alpha \beta})$ là một hệ ngược các nhóm giao hoán; và giả sử rằng mỗi $M_\alpha$ mang một cấu trúc môđun trái trên $A_\alpha$ sao cho hễ $\alpha \leq \beta$ thì ta có

(2)
$$
f_{\alpha \beta}(\lambda_\beta \cdot x_\beta) = \varphi_{\alpha \beta}(\lambda_\beta) \cdot f_{\alpha \beta}(x_\beta)
$$
với $x_\beta \in M_\beta$ và $\lambda_\beta \in A_\beta$; khi đó $\varprojlim M_\alpha$ có một cấu trúc môđun trái trên $\varprojlim A_\alpha$. Nếu giả sử thêm rằng, với mỗi $\alpha$, $A_\alpha$ giao hoán và mỗi $M_\alpha$ có một cấu trúc $A_\alpha$-đại số, và cuối cùng rằng $(M_\alpha, f_{\alpha\beta})$ là một hệ ngược các *vành*, thì $\varprojlim M_\alpha$ có một cấu trúc của một *đại số* trên $\varprojlim A_\alpha$.

Cho $(G_\alpha, f_{\alpha\beta})$ là một hệ ngược các nhóm, và với mỗi $\alpha$ cho $H_\alpha$ là một nhóm con của $G_\alpha$. Nếu $f_{\alpha\beta}(H_\beta) \subset H_\alpha$ mỗi khi $\alpha \leq \beta$, thì hệ ngược các tập con $H_\alpha$ của $G_\alpha$ là một hệ ngược các nhóm đối với các phép hạn chế của các $f_{\alpha\beta}$, và $H = \varprojlim H_\alpha$ là một *nhóm con* của $G = \varprojlim G_\alpha$. Nếu mỗi $H_\alpha$ là một nhóm con chuẩn tắc của $G_\alpha$, thì $H$ là một nhóm con chuẩn tắc của $G$. Nếu $(G'_\alpha, f'_{\alpha\beta})$ là một hệ ngược các nhóm khác và, với mỗi $\alpha$, $u_\alpha : G_\alpha \to G'_\alpha$ là một đồng cấu sao cho các $u_\alpha$ tạo thành một hệ ngược các ánh xạ, thì, nếu $H_\alpha$ là hạt nhân của $u_\alpha$, ta có $f_{\alpha\beta}(H_\beta) \subset H_\alpha$ mỗi khi $\alpha \leq \beta$; $u = \varprojlim u_\alpha$ là một đồng cấu của $G$ vào $G' = \varprojlim G'_\alpha$, và $H = \varprojlim H_\alpha$ là hạt nhân của $u$. Nếu đặt $K_\alpha = u_\alpha(G_\alpha)$, thì ta có $f'_\alpha(K_\alpha) \subset K_\alpha$ mỗi khi $\alpha \leq \beta$, do đó các $K_\alpha$ tạo thành một hệ ngược các nhóm con của các $G'_\alpha$; nhưng $K = \varprojlim K_\alpha$ *không nhất thiết là ảnh của* $G$ *dưới* $u$ [Bài tập 1 c)].

Ta thu được các kết quả tương tự bằng cách thay thế "nhóm" bằng "vành", "nhóm con" bằng "iđêan" (trái hoặc phải); ta để lại cho bạn đọc việc phát biểu các kết quả tương tự cho môđun và đại số.

### 2. GIỚI HẠN NGƯỢC CỦA CÁC NHÓM TÔPÔ VÀ KHÔNG GIAN CÓ TOÁN TỬ

Ta sẽ nói rằng một hệ ngược $(G_\alpha, f_{\alpha\beta})$ là một *hệ ngược các nhóm tôpô* nếu các $G_\alpha$ là các nhóm tôpô và các $f_{\alpha\beta}$ là các đồng cấu *liên tục*. Khi đó $G = \varprojlim G_\alpha$ là một nhóm con của nhóm tích $\prod_\alpha G_\alpha$; nếu ta trang bị cho $G$ cấu trúc nhóm tôpô cảm sinh bởi cấu trúc của $\prod_\alpha G_\alpha$, thì nhóm tôpô thu được gọi là *giới hạn ngược* của hệ ngược các nhóm tôpô $(G_\alpha, f_{\alpha\beta})$. Nếu các $G_\alpha$ là Hausdorff (tương ứng Hausdorff và đầy đủ) thì $G$ là Hausdorff và đóng trong $\prod_\alpha G_\alpha$ (tương ứng Hausdorff và đầy đủ) (Chương I, § 8, no. 2, Mệnh đề 7, Hệ quả 2 và Chương II, § 3, no. 5, Hệ quả của Mệnh đề 10).

Nếu $(G'_\alpha, f'_{\alpha\beta})$ là một hệ ngược các nhóm tôpô khác và nếu, với mỗi $\alpha$, $u_\alpha : G_\alpha \to G'_\alpha$ là một đồng cấu liên tục sao cho các $u_\alpha$ tạo thành một hệ ngược các ánh xạ, thì $u = \varprojlim u_\alpha$ là một đồng cấu liên tục của $G$ vào $G' = \varprojlim G'_\alpha$ (Chương I, § 4, no. 4). Các kết quả tương tự cũng đúng khi thay thế "nhóm tôpô" bằng "vành tôpô"; ta để lại cho bạn đọc việc phát biểu các kết quả tương tự cho môđun tôpô (§ 6, no. 6).

#### Mệnh đề 1 {#top-iii-s7-prop-1 .statement}

*Giả sử rằng các $X_\alpha$ và các $G_\alpha$ thỏa mãn các giả thiết trên.*

a) *Nếu nhóm ổn định của mỗi điểm của $X_\alpha$ là một nhóm con compact của $G_\alpha$ với mỗi $\alpha \in I$, thì nhóm ổn định của mỗi điểm $x = (x_\alpha)$ của $X$ là một nhóm con compact của $G$; quỹ đạo của $x$ (đối với $G$) đồng phôi một cách chính tắc với giới hạn ngược của các quỹ đạo của các $x_\alpha$ (đối với $G_\alpha$); và ánh xạ chính tắc $h : X/G \to \varprojlim X_\alpha/G_\alpha$ là đơn ánh.*

b) *Nếu, với mỗi $\alpha \in I$, mọi quỹ đạo của một điểm của $X_\alpha$ (đối với $G_\alpha$) đều compact, thì mọi quỹ đạo của một điểm của $X$ (đối với $G$) đều tương đối compact, và $h$ là toàn ánh. Nếu thêm nữa $h$ là song ánh, thì mọi quỹ đạo của một điểm của $X$ đều compact.*

#### Hệ quả 1 {#top-iii-s7-prop-1-cor-1 .statement}

*Nếu $G_\alpha$ compact và $X_\alpha$ Hausdorff, thì các kết luận của a) và b) đều đúng.*

Thật vậy, các giả thiết của a) và b) được thỏa mãn, vì mọi nhóm con đóng của $G_\alpha$ đều compact và $u_\alpha : s_\alpha \to s_\alpha \cdot x_\alpha$ là một ánh xạ liên tục từ một không gian compact vào một không gian Hausdorff.

#### Hệ quả 2 {#top-iii-s7-prop-1-cor-2 .statement}

*Nếu, với mỗi $\alpha \in I$, nhóm $G_\alpha$ tác động bắc cầu trên không gian $X_\alpha$, và nếu nhóm ổn định của mỗi điểm của $X_\alpha$ là một nhóm con compact của $G_\alpha$, thì $G$ tác động bắc cầu trên $X$ và nhóm ổn định của mỗi điểm của $X$ là một nhóm con compact của $G$. \*

Vì giả thiết a) được thỏa mãn, và $X'_\alpha = X_\alpha$ với mỗi $\alpha$.

#### Hệ quả 3 {#top-iii-s7-prop-1-cor-3 .statement}

Cho $x = (x_\alpha) \in X$, và với mỗi $\alpha \in I$ đặt $X'_\alpha = G_\alpha \cdot x_\alpha$ là quỹ đạo của $x_\alpha$. Nếu $\alpha \leq \beta$, thì từ (i) và quan hệ $g_{\alpha\beta}(x_\beta) = x_\alpha$ suy ra $g_{\alpha\beta}(X'_\beta) \subset X'_\alpha$, và do đó $(X'_\alpha)$ là một hệ ngược các tập con của $X_\alpha$. Với mỗi $\alpha \in I$, đặt $u_\alpha : G_\alpha \to X'_\alpha$ là ánh xạ liên tục $s_\alpha \to s_\alpha \cdot x_\alpha$; các $u_\alpha$ lập thành một hệ ngược các ánh xạ, và $u = \varprojlim u_\alpha$ là ánh xạ liên tục $s \to s.x$ của $G$ vào không gian con $X' = \varprojlim X'_\alpha$ của $X$. Giả thiết của a) suy ra rằng $\overline{u}_\alpha(y_\alpha)$ là compact với mỗi $y_\alpha \in X'_\alpha$. Vì đồng thời $u_\alpha$ là toàn ánh, nên các điều kiện của Chương I, § 9, no. 6, Mệnh đề 8, Hệ quả 2 được thỏa mãn, và do đó hai khẳng định đầu tiên của a) được thiết lập. Suy ra, nếu $x = (x_\alpha)$ và $y = (y_\alpha)$ sao cho $x_\alpha$ và $y_\alpha$ thuộc cùng một quỹ đạo đối với $G_\alpha$ với mỗi $\alpha \in I$, thì $x$ và $y$ thuộc cùng một quỹ đạo đối với $G$, và do đó $h$ là đơn ánh.

Tương tự, giả thiết của b) suy ra rằng hệ ngược các ánh xạ chính tắc $v_\alpha : X_\alpha \to X_\alpha/G_\alpha$ thỏa mãn các điều kiện của Chương I, § 9, no. 6, Mệnh đề 8, Hệ quả 2, và do đó giới hạn ngược của nó $v = \varprojlim v_\alpha : X \to \varprojlim X_\alpha/G_\alpha$ là toàn ánh, và ảnh ngược qua v của mọi điểm của $\varprojlim X_\alpha / G_\alpha$ là compact. Vì v phân tích thành
$$
X \xrightarrow{\psi} X/G \xrightarrow{h} \varprojlim X_\alpha / G_\alpha,
$$
trong đó $\psi$ là ánh xạ chính tắc, nên các khẳng định của b) suy ra.

*Giả sử rằng các $G_\alpha$ là Hausdorff. Với mỗi $\alpha \in I$, gọi $K_\alpha$ là một nhóm con compact của $G_\alpha$, sao cho $f_{\alpha \beta} (K_\beta) \subset K_\alpha$ mỗi khi $\alpha \leq \beta$. Khi đó, nếu $K = \varprojlim K_\alpha$, ánh xạ chính tắc $h$ của không gian thuần nhất $G/K$ vào $\varprojlim G_\alpha / K_\alpha$ là một đồng phôi.*

Việc $h$ là song ánh suy ra từ Hệ quả 1, áp dụng bằng cách thay $X_\alpha$ bằng $G_\alpha$, và $G_\alpha$ bằng $K_\alpha$ tác động bởi các phép tịnh tiến phải (§ 2, no. 5). Gọi $\varphi$ là ánh xạ chính tắc $G \to G/K$, và với mỗi $\alpha$ gọi $f_\alpha$ là ánh xạ chính tắc $G \to G_\alpha$. Nếu, với mỗi $\alpha$, $V_\alpha$ chạy qua một hệ cơ bản các lân cận mở của phần tử đơn vị $e_\alpha$ của $G_\alpha$, thì các tập $V = \overline{f}_\alpha^{-1}(V_\alpha)$ ($\alpha$ và $V_\alpha$ biến) lập thành một hệ cơ bản các lân cận của phần tử đơn vị $e$ trong $G$ (Chương I, § 4, no. 4, Mệnh đề 9), và các tập $\varphi(V.K)$ lập thành một hệ cơ bản các lân cận của $\varphi(e)$ trong $G/K$. Ta phải chứng minh rằng ảnh của $\varphi(V.K)$ dưới $h$ chứa một lân cận của $h(\varphi(e))$, tức là tồn tại $\beta \geq \alpha$ và một lân cận $W_\beta$ của $e_\beta$ trong $G_\beta$ sao cho $\overline{f}_\beta^{-1}(W_\beta . K_\beta) \subset V.K$. Bây giờ, quan hệ $x \in V.K$ tương đương với sự tồn tại của $y$ trong $K$ sao cho $f_\alpha(xy^{-1}) \in V_\alpha$, tức là $f_\alpha(x) \in V_\alpha \cdot f_\alpha(K)$; do đó $V.K = \overline{f}_\alpha^{-1}(V_\alpha \cdot f_\alpha(K))$. Đặt $U_\alpha = V_\alpha \cdot f_\alpha(K)$; ta sẽ thấy rằng tồn tại $\beta \geq \alpha$ sao cho nếu ta đặt $U_\beta = \overline{f}_{\alpha \beta}^{-1}(U_\alpha)$, thì $K_\beta \subset U_\beta$; khi đó sẽ suy ra rằng có một lân cận $W_\beta$ của $e_\beta$ trong $G_\beta$ sao cho $W_\beta . K_\beta \subset U_\beta$ (Chương II, § 4, no. 3, Hệ quả của Mệnh đề 4), và điều này sẽ thiết lập quan hệ mong muốn
$$
\overline{f}_\beta^{-1}(W_\beta . K_\beta) \subset \overline{f}_\beta^{-1}(U_\beta) = V.K.
$$

Chúng ta tiến hành bằng *phản chứng*: với mỗi $\beta \geq \alpha$, đặt $M_\beta$ là $K_\beta \cap G U_\beta$; vì $f_{\beta \gamma}^{-1}(U_\beta) = U_\gamma$ nếu $\alpha \leq \beta \leq \gamma$, nên các $M_\beta$ tạo thành một hệ ngược các tập con compact của các $G_\beta$ (với $\beta \geq \alpha$). Nếu tất cả chúng đều không rỗng, thì giới hạn ngược của chúng $M$ cũng sẽ không rỗng (Chương I, § 9, no. 6, Mệnh đề 8). Rõ ràng $M \subset K$ và $f_\alpha(M) \subset M_\alpha$; nhưng điều này là vô lý vì $f_\alpha(K) \subset U_\alpha$, và do đó chứng minh hoàn tất.

### 3. XẤP XỈ CÁC NHÓM TÔPÔ

Cho $G$ là một nhóm và cho $(H_\alpha)_{\alpha \in I}$ là một họ các nhóm con chuẩn tắc của $G$ sao cho $H_\alpha \supset H_\beta$ bất cứ khi nào $\alpha \leq \beta$. Với mỗi $\alpha \in I$ đặt $G_\alpha = G / H_\alpha$, và với $\alpha \leq \beta$ đặt $f_{\alpha \beta}$ là đồng cấu chính tắc $G / H_\beta \to G / H_\alpha$, do đó nó ánh xạ một lớp kề $T$ của $H_\beta$ trong $G$ tới lớp kề $TH_\alpha$ của $H_\alpha$ trong $G$. Rõ ràng $(G_\alpha, f_{\alpha \beta})$ là một hệ ngược các nhóm; các phần tử của $\tilde{G} = \varprojlim G_\alpha$ là các họ $(T_\alpha)_{\alpha \in I}$, trong đó $T_\alpha$ là một lớp kề của $H_\alpha$ trong $G$ với mỗi $\alpha$, và $T_\alpha \supset T_\beta$ bất cứ khi nào $\alpha \leq \beta$. Ánh xạ $i : s \mapsto (s H_\alpha)$ của $G$ vào $\tilde{G}$ là giới hạn ngược của các đồng cấu chính tắc $G \to G / H_\alpha$ và do đó là một đồng cấu của $G$ vào $\tilde{G}$, và ảnh ngược qua $i$ của một phần tử $(T_\alpha) \in \tilde{G}$ bằng $\bigcap_{\alpha \in I} T_\alpha$. Hạt nhân của $i$ do đó là $\bigcap_{\alpha \in I} H_\alpha$, và ảnh của $i$ gồm tất cả các họ $(T_\alpha) \in \tilde{G}$ mà giao của chúng là *không rỗng*.

Giả sử bây giờ rằng $G$ là một *nhóm tôpô*; nếu ta cho mỗi $G_\alpha = G / H_\alpha$ tôpô thương, thì rõ ràng $(G_\alpha, f_{\alpha \beta})$ là một hệ ngược các nhóm tôpô, và $i : G \to \tilde{G}$ là một đồng cấu liên tục.

#### Mệnh đề 2 {#top-iii-s7-prop-2 .statement}

*Cho $G$ là một nhóm tôpô và cho $(H_\alpha)_{\alpha \in I}$ là một họ các nhóm con chuẩn tắc của $G$ sao cho $H_\alpha \supset H_\beta$ bất cứ khi nào $\alpha \leq \beta$, và thỏa mãn điều kiện sau:*

(AP) *Với mỗi $\alpha \in I$, $H_\alpha$ đóng trong $G$ và mọi lân cận của phần tử đơn vị $e$ trong $G$ đều chứa một trong các $H_\alpha$ (nói cách khác, cơ sở lọc do các $H_\alpha$ tạo thành hội tụ về $e$).*

*Khi đó ánh xạ $i : G \to \tilde{G} = \varprojlim G / H_\alpha$ là một cấu xạ ngặt từ $G$ lên $i(G)$; $\tilde{G}$ là Hausdorff và $i(G)$ trù mật trong $\tilde{G}$; và cuối cùng hạt nhân của $i$ là bao đóng của $\{e\}$ trong $G$. Nếu thêm nữa một trong các $H_\alpha$ đầy đủ, thì $i$ là toàn ánh.*

Rõ ràng $G_\alpha = G / H_\alpha$ là Hausdorff (§ 2, no. 5, Mệnh đề 13), do đó $\tilde{G}$ cũng vậy (vì nó là một không gian con của $\prod_{\alpha \in I} G_\alpha$). Hạt nhân $H$ của $i$ là giao của các $H_\alpha$ và vì thế là một nhóm con đóng của $G$. Vì mỗi lân cận của $e$ đều chứa một $H_\alpha$ nào đó, nên nó chứa $H$ và do đó [Chương I, § 4, no. 4, Mệnh đề 9] $H$ là bao đóng của $\{e\}$. Tiếp theo hãy chứng minh rằng $i(G)$ trù mật trong $\tilde{G}$. Gọi $f_\alpha$ là ánh xạ chính tắc $\tilde{G} \to G_\alpha$, tức là sự hạn chế lên $\tilde{G}$ của phép chiếu $pr_\alpha$; $\varphi_\alpha = f_\alpha \circ i$ là ánh xạ chính tắc $G \to G/H_\alpha$. Nếu $U$ là bất kỳ tập mở không rỗng nào của $\tilde{G}$, thì tồn tại một chỉ số $\alpha \in I$ và một tập mở không rỗng $U_\alpha$ trong $G_\alpha$ sao cho $\overline{f}_\alpha^{-1}(U_\alpha) \subset U$ (Chương I, § 4, no. 4, Mệnh đề 9); do đó
$$
\overline{i}^{-1}(U) \supset \overline{\varphi}_\alpha^{-1}(U_\alpha);
$$
nhưng vì $\varphi_\alpha$ là toàn ánh, $\overline{i}^{-1}(U)$ không rỗng, và do đó $i(G) \cap U \neq \emptyset$.

Để thấy rằng $i$ là một cấu xạ ngặt của $G$ lên $i(G)$, hãy xét một lân cận $V$ của $e$ trong $G$. Có một lân cận $W$ của $e$ trong $G$ sao cho $W^2 \subset V$, và một chỉ số $\alpha \in I$ sao cho $H_\alpha \subset W$; suy ra $V$ chứa $WH_\alpha = \overline{\varphi}_\alpha(\varphi_\alpha(W)) = \overline{i}^{-1}(\overline{f}_\alpha^{-1}(\varphi_\alpha(W)))$. Vì $\overline{f}_\alpha(\varphi_\alpha(W))$ là một lân cận của phần tử đơn vị trong $\tilde{G}$, suy ra điều phải chứng minh.

Cuối cùng, giả sử rằng có một chỉ số $\gamma \in I$ sao cho $H_\gamma$ đầy đủ. Để chứng minh rằng $i$ là toàn ánh, chỉ cần chứng minh rằng mọi họ $(T_\alpha)_{\alpha \in I} \in \tilde{G}$ đều có một giao không rỗng. Vì $T_\gamma$ thu được từ $H_\gamma$ bằng phép tịnh tiến, nó là một không gian con đầy đủ của $G$ (đối với cả cấu trúc đều phải và đều trái). Hơn nữa, vì mọi lân cận $U$ của $e$ trong $G$ đều chứa một trong các $H_\alpha$, tập tương ứng $T_\alpha$ là $U_{d-}$ (hoặc $U_{s-}$) nhỏ, và do đó họ các $T_\alpha$ được chứa trong $T_\gamma$ là một cơ sở lọc Cauchy; vì thế nó hội tụ trong $T_\gamma$, và vì các $T_\alpha$ là đóng trong $G$ (do chúng là các phép tịnh tiến của các $H_\alpha$), giao của chúng không rỗng.

Q.E.D.

#### Hệ quả 1 {#top-iii-s7-prop-2-cor-1 .statement}

*Nếu điều kiện (AP) được thỏa mãn và nếu thêm vào đó các nhóm (Hausdorff) $G/H_\alpha$ đầy đủ, thì nhóm $G$ có một sự đầy đủ hóa Hausdorff có thể được đồng nhất với $\tilde{G}$; và ánh xạ $i : G \to \tilde{G}$ khi đó được đồng nhất với ánh xạ chính tắc ($§ 3$, no. 3, Mệnh đề 5).*

Vì $\tilde{G}$ khi đó đầy đủ (no. 2), và Mệnh đề 2 cho thấy $i(G)$ đẳng cấu với nhóm Hausdorff liên kết với $G$; vì nó trù mật trong $\tilde{G}$, hệ quả suy ra ($§ 3$, no. 3, Mệnh đề 5). Nói riêng:

#### Hệ quả 2 {#top-iii-s7-prop-2-cor-2 .statement}

*Cho $G$ là một nhóm và cho $(H_\alpha)$ là một họ các nhóm con chuẩn tắc của $G$, có hướng đối với quan hệ $H_\alpha \supset H_\beta$. Nếu ta trang bị cho $G$ tôpô nhóm sao cho các $H_\alpha$ tạo thành một hệ cơ sở của các lân cận của phần tử đơn vị $e$, thì nhóm Hausdorff liên kết với $G$ đẳng cấu với $G_1 = G / \left( \bigcap_\alpha H_\alpha \right)$; $G_1$ có một sự đầy đủ hóa $\hat{G}_1 = \tilde{G}$; và ánh xạ chính tắc $G_1 \to \tilde{G} = \varprojlim G/H_\alpha$ mở rộng thành một đẳng cấu của $\hat{G} = \hat{G}_1$ lên $\tilde{G}$.*

Nhóm con $H_\alpha$ của $G$ là mở và do đó cũng đóng ($\S$ 2, no. 1, Hệ quả của Mệnh đề 4), và $G/H_\alpha$ là rời rạc ($\S$ 2, no. 6, Mệnh đề 18); do đó các điều kiện của Hệ quả 1 được thỏa mãn.

Trong phần còn lại của tiểu mục này, ta sẽ giả sử rằng $G$ là *Hausdorff* và rằng $(H_\alpha)$ là một họ các nhóm con chuẩn *compact* của $G$, có hướng theo quan hệ $H_\alpha \supset H_\beta$ và thỏa mãn điều kiện (AP); theo Mệnh đề 2, ánh xạ

$$
i : G \to \tilde{G} = \varprojlim G/H_\alpha
$$

khi đó là một *đẳng cấu của các nhóm tôpô* cho phép ta đồng nhất $G$ và $\tilde{G}$. Ta ký hiệu $f_\alpha$ là ánh xạ chính tắc $G \to G/H_\alpha$.

#### Bổ đề 1 {#top-iii-s7-lem-1 .statement}

*Dưới các giả thiết của Mệnh đề 2, nếu $E$ là bất kỳ tập con đóng nào của $G$ thì ta có* $E = \bigcap_\alpha E H_\alpha$.

Vì $E$ là giao của các tập $EV$ khi $V$ chạy qua họ lân cận của $e$ [$\S$ 3, no. 1, công thức (1)], và mọi lân cận của $e$ đều chứa một $H_\alpha$; do đó có kết quả, vì $E \subset EH_\alpha$.

#### Mệnh đề 3 {#top-iii-s7-prop-3 .statement}

*Giả sử rằng $G$ là Hausdorff và rằng các $H_\alpha$ là compact và thỏa mãn* (AP).

a) *Cho $L$ là một nhóm con đóng của $G$; khi đó, với mỗi $\alpha \in I$, nhóm con $L_\alpha = f_\alpha(L)$ của $G_\alpha = G/H_\alpha$ là đóng, và đẳng cấu $i$ của $G$ lên $\varprojlim G_\alpha$ cho, khi hạn chế, một đẳng cấu của $L$ lên $\varprojlim L_\alpha$. Nếu thêm nữa $L$ là chuẩn trong $G$, thì $L_\alpha$ là chuẩn trong $G_\alpha$ với mỗi $\alpha \in I$, và khi chuyển qua thương, $i$ cảm sinh một đẳng cấu của $G/L$ lên $\varprojlim G_\alpha/L_\alpha$.

b) *Ngược lại, với mỗi $\alpha \in I$ cho $L_\alpha$ là một nhóm con đóng của $G_\alpha$, sao cho $L_\alpha = f_{\alpha\beta}(L_\alpha)$ mỗi khi $\alpha \leq \beta$. Khi đó tồn tại duy nhất một nhóm con đóng $L$ của $G$ sao cho $L_\alpha = f_\alpha(L)$ với mỗi $\alpha \in I$; và nếu thêm vào đó $L_\alpha$ là chuẩn trong $G_\alpha$ với mỗi $\alpha \in I$, thì $L$ là chuẩn trong $G$.*

a) Vì $H_\alpha$ là compact, $LH_\alpha$ đóng trong $G$ ($\S$ 4, no. 1, Mệnh đề 1, Hệ quả 1) và do đó $L_\alpha$ đóng trong $G_\alpha$. Vì $i$ đồng nhất các nhóm tôpô $G$ và $\varprojlim G_\alpha$, và vì $\varprojlim L_\alpha$ có thể được đồng nhất với một nhóm con (tôpô) của $\varprojlim G_\alpha$, $i$ đồng nhất nhóm con $\bigcap_\alpha LH_\alpha$ của $G$ với $\varprojlim L_\alpha$, và để chứng minh khẳng định thứ nhất chỉ cần nhận xét rằng $L = \bigcap_\alpha LH_\alpha$ theo Bổ đề 1. Mặt khác, nếu $L$ là chuẩn tắc, thì với mỗi $\alpha \in I$ ánh xạ $f'_\alpha : G/L \to G_\alpha/L_\alpha$ cảm sinh bởi $f_\alpha$ là một cấu xạ ngặt toàn ánh ($\S$ 2, no. 8, Nhận xét 3), có hạt nhân là nhóm con chuẩn tắc *compact* $H_\alpha L/L$ của $G/L$, ảnh chính tắc của nhóm con compact $H_\alpha$ của $G$. Vì các nhóm con $H_\alpha L/L$ của $G/L$ thỏa mãn điều kiện (AP) ($\S$ 2, no. 8, Mệnh đề 24), và vì $G/L$ là Hausdorff, nên khẳng định cuối cùng của a) là hệ quả của Mệnh đề 2.

b) Đặt $f'_{\alpha \beta}$ là hạn chế của $f_{\alpha \beta}$ lên $L_\beta$ ($\alpha \leq \beta$). Khi đó $(L_\alpha, f'_{\alpha \beta})$ là một hệ ngược các nhóm tôpô, mà giới hạn ngược $L$ có thể được đồng nhất với nhóm con $G \cap \prod_\alpha L_\alpha$ của $G$. Theo giả thiết, $f'_{\alpha \beta}$ là toàn ánh và hạt nhân của nó là nhóm con compact $f_\beta(H_\alpha) \cap L_\beta$ của $L_\beta$; do đó (Chương I, $\S$ 9, no. 6, Hệ quả 1 của Mệnh đề 8) ta có $L_\alpha = f_\alpha(L)$ với mọi $\alpha \in I$. Nếu $L'$ là một nhóm con đóng khác của $G$ sao cho $f_\alpha(L') = L_\alpha$ với mọi $\alpha \in I$, thì $L'H_\alpha = \overline{f'}_\alpha(L_\alpha)$, do đó (Bổ đề 1) $L' = \bigcap_\alpha L'H_\alpha = \bigcap_\alpha \overline{f'}_\alpha(L_\alpha) = L$. Cuối cùng, khẳng định cuối cùng của b) suy ra từ công thức $L = \bigcap_\alpha \overline{f'}_\alpha(L_\alpha)$, vì các $\overline{f'}_\alpha(L_\alpha)$ nay là các nhóm con chuẩn tắc của $G$.

#### Mệnh đề 4 {#top-iii-s7-prop-4 .statement}

*Giả sử $G$ là Hausdorff, các $H_\alpha$ là compact và (AP) được thỏa mãn. Nếu $C_\alpha$ là thành phần liên thông đơn vị của $G_\alpha = G/H_\alpha$, thì thành phần liên thông đơn vị $C$ của $G$ có thể được đồng nhất với $\varprojlim C_\alpha$, và ta có $f_\alpha(C) = C_\alpha$.*

Mệnh đề là một hệ quả của bổ đề sau đây:

#### Bổ đề 2 {#top-iii-s7-lem-2 .statement}

*Cho $G$ là một nhóm tôpô Hausdorff và cho $H$ là một nhóm con chuẩn tắc compact của $G$, và $\varphi$ là ánh xạ chính tắc $G \to G/H$. Nếu $C$ là thành phần liên thông của đơn vị của $G$, thì $\varphi(C)$ là thành phần liên thông của đơn vị của $G' = G/H$.*

Khi bổ đề này đã được thiết lập, ta sẽ có $f_\alpha(C) = C_\alpha$ với mỗi $\alpha \in I$, và vì $C$ là một nhóm con đóng của $G$ (§ 2, no. 2, Mệnh đề 7) nên đủ áp dụng Mệnh đề 3 a).

Để chứng minh bổ đề, trước hết lưu ý rằng nếu $C'$ là thành phần của phần tử đơn vị $e'$ trong $G'$, thì $\varphi(C) \subset C'$ vì $\varphi(C)$ liên thông. Giả sử $\varphi(C) \neq C'$. Vì $C$ là một nhóm con chuẩn tắc đóng của $G$ (§ 2, no. 2, Mệnh đề 7), $\varphi(C)$ là một nhóm con chuẩn tắc của $G'$; nếu $\psi$ là ánh xạ chính tắc $G' \to G'/\varphi(C)$, thì $\psi(C')$ liên thông và không chỉ gồm riêng phần tử đơn vị; do đó thành phần liên thông của đơn vị của $G'/\varphi(C)$ không chỉ gồm riêng phần tử đơn vị. Nhưng $G'/\varphi(C)$ đẳng cấu với $(G/H)/(HC/H)$, do đó với $G/HC$, và do đó cũng đẳng cấu với $(G/C)/(HC/C)$ (§ 2, no. 7, Hệ quả của Mệnh đề 22, và Mệnh đề 20). Bây giờ, $G/C$ là Hausdorff và liên thông rời rạc hoàn toàn (Chương I, § 11, no. 5, Mệnh đề 9), và $HC/C$, là ảnh chính tắc của nhóm con chuẩn tắc compact $H$ của $G$, là một nhóm con compact của $G/C$. Vì vậy chỉ cần chứng minh Bổ đề 2 dưới giả thiết bổ sung rằng $G$ là *liên thông rời rạc hoàn toàn*, tức là $C = \{e\}$.

Giả sử khi đó $C' \neq \{e'\}$; thay $G$ bởi nhóm con $\overline{f'}(C')$ của nó, là liên thông rời rạc hoàn toàn và chứa $H$, ta có thể giả sử rằng $G'$ là *liên thông* và không chỉ gồm một điểm đơn.

Cho $\mathfrak{M}$ là tập hợp các nhóm con đóng $L$ của $G$ sao cho $LH = G$. Ta sẽ chứng minh rằng tập hợp $\mathfrak{M}$, được sắp thứ tự theo quan hệ $\supset$, là *quy nạp*. Thật vậy, nếu $\mathfrak{T}$ là một tập con có thứ tự tuyến tính của $\mathfrak{M}$, thì với mỗi $x \in G$ tập hợp các tập hợp $xH \cap L$ với $L \in \mathfrak{T}$ là một cơ sở lọc gồm các tập hợp đóng trong không gian compact $xH$; do đó giao của các tập hợp này không rỗng, điều đó cho thấy rằng giao của các nhóm con $L \in \mathfrak{T}$ thuộc $\mathfrak{M}$. Áp dụng bổ đề Zorn, do đó ta thấy rằng $\mathfrak{M}$ có một phần tử *cực tiểu* $L_0$. Vì $H$ là compact, $G/H = L_0H/H$ đẳng cấu với $L_0/(L_0 \cap H)$ (§ 4, no. 1, Mệnh đề 1, Hệ quả 3); vì $L_0$ hoàn toàn rời rạc và $L_0 \cap H$ compact, ta thấy rằng có thể thay $G$ bởi $L_0$; nói cách khác, ta có thể giả sử thêm rằng *không* có nhóm con đóng $L \neq G$ nào sao cho $LH = G$.

Bây giờ đặt $F$ là giao của các lân cận của phần tử đơn vị vừa mở vừa đóng trong $G$, và ta chứng minh rằng $F$ là một nhóm con đóng của $G$. Rõ ràng $F$ đóng trong $G$; do đó chỉ cần chứng minh rằng $F^{-1}F \subset F$. Nhưng nếu $x \in F$ và nếu $V$ là một lân cận mở và đóng của $e$ trong $G$, thì $xV$ cũng vậy; vì nếu không thì $e$ sẽ thuộc bù $W$ của $xV$ trong $G$, mà $W$ cũng mở và đóng, và ta phải có $x \notin W$; do đó $x \notin F$, trái với giả thiết. Suy ra rằng $xF$, là giao của các tập hợp $xV$ khi $V$ chạy qua các lân cận mở và đóng của $e$ trong $G$, chứa $F$; nói cách khác, $x^{-1}F \subset F$, điều đó chứng minh mệnh đề của chúng ta. Vì $G$ liên thông rời rạc toàn phần và $G \neq \{e\}$, ta có $F \neq G$. Nhưng nếu $V$ là một lân cận mở và đóng của $e$ trong $G$, thì $VH$ cũng mở và đóng trong $G$ (§ 4, số 1, Hệ quả 1 của Mệnh đề 1), do đó $\varphi(V)$ vừa mở vừa đóng trong $G/H$, và điều này suy ra $\varphi(V) = G/H$ theo giả thiết. Từ đó ta sẽ kết luận rằng $FH = G$, điều này sẽ cho ta mâu thuẫn mong muốn và hoàn tất chứng minh của bổ đề. Thật vậy, với mỗi $x \in G$, $xH$ gặp mọi lân cận $V$ của $e$ vừa mở vừa đóng, do đó cũng gặp giao $F$ của các lân cận này, vì các tập $Vx \cap H$ tạo thành một cơ sở lọc gồm các tập đóng trong không gian compact $xH$.

Q.E.D.

#### Nhận xét {#top-iii-s7-n3-rem-1 .statement}

Nếu nhóm con $H_\alpha$ là compact đối với *một* $\alpha \in I$, thì $H_\beta$ là compact với mọi $\beta \geq \alpha$, vì nó là một nhóm con đóng của $H_\alpha$. Vì tập tất cả các $\beta \in I$ sao cho $\beta \geq \alpha$ là đồng cuối trong $I$, nên trong việc nghiên cứu nhóm $G$, hầu như không có khác biệt nào giữa việc giả sử rằng một trong các $H_\alpha$ là compact hay rằng *tất cả* các $H_\alpha$ đều compact.

### 4. ỨNG DỤNG VÀO GIỚI HẠN NGƯỢC

#### Mệnh đề 5 {#top-iii-s7-prop-5 .statement}

==========

*Cho* $(G_\alpha, f_{\alpha\beta})$ *là một hệ ngược các nhóm tôpô Hausdorff sao cho các* $f_{\alpha\beta}$ *là các cấu xạ ngặt toàn ánh có hạt nhân compact.* Khi đó, với mỗi $\alpha \in I$ , ánh xạ chính tắc $f_\alpha$ của $G = \varprojlim G_\alpha$ vào $G_\alpha$ là một cấu xạ ngặt toàn ánh có hạt nhân compact.

Việc $f_\alpha$ toàn ánh và hạt nhân của nó compact là hệ quả của Chương I, § 9, no. 6, Hệ quả 1 của Mệnh đề 8. Còn phải chứng minh rằng $f_\alpha$ là một cấu xạ ngặt. Cho $e$ (resp. $e_\alpha$) ký hiệu phần tử đơn vị của $G$ (resp. $G_\alpha$). Mỗi lân cận $V$ của $e$ trong $G$ chứa một tập hợp có dạng $f_\beta^{-1}(V_\beta)$, trong đó $V_\beta$ là một lân cận của $e_\beta$ trong $G_\beta$, và ta có thể giả sử rằng $\beta \geq \alpha$; vì $f_{\alpha \beta}$ là một cấu xạ ngặt toàn ánh, $f_{\alpha \beta}(V_\beta)$ là một lân cận của $e_\alpha$ trong $G_\alpha$, và vì $f_\beta$ toàn ánh, ta có $V_\beta \subset f_\beta(V)$, do đó

$$
f_\alpha(V) = f_{\alpha \beta}(f_\beta(V)) \supset f_{\alpha \beta}(V_\beta);
$$

điều này cho thấy rằng $f_\alpha(V)$ là một lân cận của $e_\alpha$ trong $G_\alpha$.

Nếu $H_\alpha = f_\alpha^{-1}(e_\alpha)$, thì mỗi $H_\alpha$ là một nhóm con chuẩn tắc compact của $G$; các $H_\alpha$ rõ ràng thỏa mãn điều kiện (AP) của no. 3; và $G_\alpha$ có thể được đồng nhất với $G/H_\alpha$. Đặc biệt, Mệnh đề 3 và 4 của no. 3 áp dụng cho $G$ và các $H_\alpha$.

#### Hệ quả 1 {#top-iii-s7-prop-5-cor-1 .statement}

*Cho* $(G_\alpha, f_{\alpha \beta})$ *là một hệ ngược các nhóm tôpô thỏa mãn các giả thiết của Mệnh đề 5; cho* $(G'_\alpha, f'_{\alpha \beta})$ *là một hệ ngược các nhóm tôpô, và với mỗi* $\alpha$ *cho* $u_\alpha : G_\alpha \to G'_\alpha$ *là một cấu xạ ngặt toàn ánh có hạt nhân compact, sao cho các* $u_\alpha$ *tạo thành một hệ ngược các ánh xạ. Khi đó* $u = \varprojlim u_\alpha$ *là một cấu xạ ngặt của* $G = \varprojlim G_\alpha$ *lên* $G' = \varprojlim G'_\alpha$, *và hạt nhân của nó là compact*.

Cho $N_\alpha$ là hạt nhân của $u_\alpha$. Khi đó $L_\alpha = f_\alpha^{-1}(N_\alpha)$ là hạt nhân của cấu xạ ngặt toàn ánh $v_\alpha = u_\alpha \circ f_\alpha : G \to G'_\alpha$; vì $L_\alpha / H_\alpha$ đẳng cấu với $N_\alpha$ (§ 2, no. 7, Mệnh đề 20), nên $L_\alpha$ là một nhóm con chuẩn tắc *compact* của $G$ (§ 4, no. 1, Hệ quả 2 của Mệnh đề 2). Hạt nhân $L$ của $u$ là giao của các $L_\alpha$. Ký hiệu $\varphi$ là ánh xạ chính tắc $G \to G/L$; khi đó ta có thể viết $v_\alpha = w_\alpha \circ \varphi$, trong đó $w_\alpha$ là một cấu xạ ngặt của $G/L$ lên $G'_\alpha$, có hạt nhân là $L_\alpha / L$. Vì giao của các $L_\alpha / L$ là phần tử đơn vị của $G/L$, và vì các $L_\alpha / L$ tạo thành một cơ sở lọc và là compact, nên cơ sở lọc này hội tụ về phần tử đơn vị của $G/L$ (Chương I, § 9, no. 1, Hệ quả của Định lý 1). Mệnh đề 2 của no. 3 suy ra rằng $w = \varprojlim w_\alpha$ là một *đẳng cấu* từ $G/L$ lên $G'$; suy ra $w \circ \varphi$ là một cấu xạ ngặt của $G$ lên $G'$, với hạt nhân $L$. Nhưng hiển nhiên $u = w \circ \varphi$, và do đó hệ quả được chứng minh.

#### Hệ quả 2 {#top-iii-s7-prop-5-cor-2 .statement}

*Cho* $(G_\alpha, f_{\alpha \beta})$ *là một hệ ngược của các nhóm tôpô thỏa mãn các điều kiện của Mệnh đề 5, và cho* $G'$ *là một nhóm tôpô trong đó có một lân cận* $V'$ *của phần tử đơn vị* $e'$ *không chứa nhóm con nào* của $G'$ *khác* $\{ e' \}$. Khi đó nếu $v : G \to G'$ là một đồng cấu liên tục bất kỳ, thì tồn tại một chỉ số $\alpha \in I$ và một đồng cấu liên tục $v_\alpha : G_\alpha \to G'$ sao cho $v = v_\alpha \circ f_\alpha$.

Vì $\overline{v}^{-1}(V')$ là một lân cận của $e$ trong $G$, nên tồn tại một chỉ số $\alpha$ và một lân cận $V_\alpha$ của $e_\alpha$ trong $G_\alpha$ sao cho $f_\alpha^{-1}(V_\alpha) \subset \overline{v}^{-1}(V')$. Do đó $v(H_\alpha) \subset V'$, và vì $v(H_\alpha)$ là một nhóm con của $G'$, suy ra $v(H_\alpha) = \{ e' \}$. Vì $f_\alpha$ có thể được đồng nhất với ánh xạ chính tắc $G \to G/H_\alpha$, nên hệ quả là một hệ quả của phép phân tích chính tắc của một đồng cấu liên tục (§ 2, no. 8).

### Bài tập {#top-iii-s7-exercises}

Xem [các bài tập cho § 7](exercises/s7/).
