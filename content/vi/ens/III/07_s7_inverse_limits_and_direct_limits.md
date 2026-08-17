---
book: ens
book_title: Theory of Sets
chapter: III
chapter_title: ORDERED SETS, CARDINALS, INTEGERS
section: 7
section_title: Inverse limits and direct limits
lang: vi
source: ens-i-iv
source_edition: 2004, Springer
book_pages: 191-211, 251-254
pdf_pages: 0197-0217, 0257-0260
extraction: ocr
subsections:
    - "no": 1
      title: INVERSE LIMITS
      page: 191
      pdf_page: 197
    - "no": 2
      title: INVERSE SYSTEMS OF MAPPINGS
      page: 192
      pdf_page: 198
    - "no": 3
      title: DOUBLE INVERSE LIMIT
      page: 196
      pdf_page: 202
    - "no": 4
      title: CONDITIONS FOR AN INVERSE LIMIT TO BE NON-EMPTY
      page: 198
      pdf_page: 204
    - "no": 5
      title: DIRECT LIMITS
      page: 202
      pdf_page: 208
    - "no": 6
      title: DIRECT SYSTEMS OF MAPPINGS
      page: 204
      pdf_page: 210
    - "no": 7
      title: DOUBLE DIRECT LIMIT. PRODUCT OF DIRECT LIMITS
      page: 209
      pdf_page: 215
statements: 34
exercises: 9
errata:
    - says: no. 2, Proposition 2, Corollary 2
      read: no. 2, Proposition 1, Corollary 2
      why: The fact cited on page 197 is that the maps of an inverse system compose, h to the lambda nu being h to the lambda mu after h to the mu nu, and that is Corollary 2 of Proposition 1 of no. 2, the corollary on three inverse systems. Proposition 2 of that no. prints one corollary and it carries no number.
content_sha256: bf84b83179911a9d9955fd49a55221dff23c09fa06bff6d18a95618e8985f026
translated_from: content/en/ens/III/07_s7_inverse_limits_and_direct_limits.md
source_content_sha256: a49555c4f56c60d7aca4de0b044ddea42c75f0dbc65c50f4a3e879299a765497
translation_model: gpt-5-6, gpt-5-6-mini, gpt-5.4, nemotron-3-ultra-free
translation_run: translate-vi-786fc151
glossary_version: 29
glossary_terms_sha256: 7460ccb7ab747636181ff4e6a149d10bc90b8626116296b8c4361e04f71e73e4
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 7. GIỚI HẠN NGHỊCH ĐẢO VÀ GIỚI HẠN TRỰC TIẾP

### 1. GIỚI HẠN NGHỊCH ĐẢO

Cho $I$ là một tập hợp tiền thứ tự và cho $(E_\alpha)_{\alpha\in I}$ là một họ các tập hợp được chỉ số bởi $I$. Với mỗi cặp $(\alpha,\beta)$ các phần tử của $I$ sao cho $\alpha\leq\beta$, cho $f_{\alpha\beta}$ là một ánh xạ từ $E_\beta$ vào $E_\alpha$. Giả sử rằng các $f_{\alpha\beta}$ thỏa mãn các điều kiện sau :

$(\mathrm{LP}_I)$ *Các quan hệ $\alpha\leq\beta\leq\gamma$ suy ra $f_{\alpha\gamma}=f_{\alpha\beta}\circ f_{\beta\gamma}$.*

$(\mathrm{LP}_{II})$ *Với mỗi $\alpha\in I$, $f_{\alpha\alpha}$ là ánh xạ đồng nhất của $E_\alpha$.*

Cho $G=\prod_{\alpha\in I}E_\alpha$ là *tích* của họ các tập hợp $(E_\alpha)_{\alpha\in I}$, và gọi $E$ là tập con của $G$ gồm tất cả các $x$ thỏa mãn mỗi quan hệ

(1)

$$\operatorname{pr}_{\alpha}x=f_{\alpha\beta}(\operatorname{pr}_{\beta}x)$$

đối với mỗi cặp chỉ số $(\alpha,\beta)$ sao cho $\alpha\leq\beta$. $E$ được gọi là *giới hạn ngược của họ* $(E_\alpha)_{\alpha\in I}$ *đối với họ ánh xạ* $(f_{\alpha\beta})$, và ta viết $E=\underset{\longleftarrow}{\lim}\,(E_\alpha,f_{\alpha\beta})$ hoặc đơn giản là $E=\underset{\longleftarrow}{\lim}\,E_\alpha$ khi không có nguy cơ gây nhầm lẫn. Với sự lạm dụng ngôn ngữ, cặp $((E_\alpha),(f_{\alpha\beta}))$ (thường được ký hiệu bởi $(E_{\alpha\beta},f_{\alpha\beta})$) được gọi là một *hệ ngược các tập hợp*, tương đối với tập hợp chỉ số $I$. *Hạn chế* $f_\alpha$ của phép chiếu $\operatorname{pr}_\alpha$ lên $E$ được gọi là *ánh xạ chính tắc* của $E$ vào $E_\alpha$, và ta có quan hệ

(2)

$$f_\alpha=f_{\alpha\beta}\circ f_\beta$$

với mọi $\alpha\leq\beta$; đây chỉ là sự chép lại các quan hệ (1) định nghĩa $E$.

*Các ví dụ*

#### Ví dụ 1 {#ens-iii-s7-n1-exa-1 .statement tag=03TF}

Giả sử rằng quan hệ thứ tự trên $I$ là quan hệ *đẳng thức*. Khi đó các cặp $(\alpha,\beta)$ duy nhất sao cho $\alpha\leq\beta$ là các cặp $(\alpha,\alpha)$ với $\alpha\in I$; và vì $f_{\alpha\alpha}$ là ánh xạ đồng nhất, quan hệ (1) được thỏa mãn đối với *mọi* $x\in G$; nói cách khác, $\underset{\longleftarrow}{\lim}\,E_\alpha$ khi đó là *tích* $\prod_{\alpha\in I}E_\alpha$.

#### Ví dụ 2 {#ens-iii-s7-n1-exa-2 .statement tag=03TG}

Giả sử rằng $I$ là *có hướng phải*, rằng $E_\alpha$ là cùng một tập hợp $F$ đối với mọi $\alpha\in I$, và rằng $f_{\alpha\beta}$ là ánh xạ đồng nhất của $F$ lên chính nó mỗi khi $\alpha\leq\beta$. Khi đó $E=\underset{\longleftarrow}{\lim}\,E_\alpha$ là *đường chéo* $\Delta$ của tích $\prod_{\alpha\in I}E_\alpha=F^I$. Thật vậy, hiển nhiên rằng mỗi $x\in\Delta$ thỏa mãn các hệ thức (1). Ngược lại, cho $x$ là một phần tử của $E$, và ta hãy chứng minh rằng đối với mỗi cặp chỉ số

$(\alpha, \beta)$ ta có $\mathrm{pr}_\alpha x = \mathrm{pr}_\beta x$. Theo giả thiết, tồn tại một chỉ số $\gamma \in I$ sao cho $\alpha \leqslant \gamma$ và $\beta \leqslant \gamma$; do đó theo (1) ta có $\mathrm{pr}_\alpha x = f_{\alpha\gamma}(\mathrm{pr}_\gamma x) = \mathrm{pr}_\gamma x$, và tương tự $\mathrm{pr}_\beta x = \mathrm{pr}_\gamma x$, điều này chứng minh mệnh đề của chúng ta.

Cần lưu ý rằng $E = \varprojlim E_\alpha$ có thể *rỗng* ngay cả khi mọi $E_\alpha$ đều không rỗng và mọi ánh xạ $f_{\alpha\beta}$ đều *toàn ánh* (Bài tập 4; xem số 4).

¶ Rõ ràng là với mỗi tập con J của I, cặp gồm họ con $(E_\alpha)_{\alpha \in J}$ và họ $(f_{\alpha\beta})$, trong đó $\alpha \in J$, $\beta \in J$, và $\alpha \leqslant \beta$, lại là một hệ ngược của các tập hợp tương đối với J; người ta nói rằng nó thu được bằng cách *hạn chế* tập chỉ số vào J. Gọi tương ứng E và E' là các giới hạn ngược của các họ $(E_\alpha)_{\alpha \in I}$ và $(E_\alpha)_{\alpha \in J}$. Với mỗi $x \in E$, phần tử

$$g(x) = (f_\alpha(x))_{\alpha \in J} \tag{3}$$

thuộc E' theo (2); ánh xạ $g : E \to E'$ được định nghĩa như vậy được gọi là *chính tắc*. Nếu J' là một tập con của J, E'' là giới hạn ngược của họ $(E_\alpha)_{\alpha \in J'}$, và nếu $g' : E' \to E''$ và $g'' : E \to E''$ là các ánh xạ chính tắc, thì theo định nghĩa ta có

$$g'' = g' \circ g. \tag{4}$$

### 2. CÁC HỆ NGƯỢC CỦA ÁNH XẠ

#### Mệnh đề 1 {#ens-iii-s7-prop-1 .statement tag=03OC}

*Cho* I *là một tập hợp có thứ tự, cho* $(E_\alpha, f_{\alpha\beta})$ *là một hệ ngược của các tập hợp tương đối với* I, *cho* $E = \varprojlim E_\alpha$ *là giới hạn ngược của nó, và với mỗi* $\alpha \in I$ *cho*

$$f_\alpha : E \to E_\alpha$$

*là ánh xạ chính tắc. Với mỗi* $\alpha \in I$, *cho* $u_\alpha$ *là một ánh xạ của một tập hợp* F *vào* $E_\alpha$ *sao cho*

$$f_{\alpha\beta} \circ u_\beta = u_\alpha \qquad \textit{khi } \alpha \leqslant \beta. \tag{5}$$

*Khi đó :*

(a) *tồn tại một ánh xạ duy nhất* $u$ *của* F *vào* E *sao cho*

$$u_\alpha = f_\alpha \circ u \qquad \textit{với mọi } \alpha \in I;\tag{6}$$

(b) *ánh xạ* $u$ *là đơn ánh khi và chỉ khi, với mỗi cặp phần tử phân biệt* $y$, $z$ *của* F, *tồn tại* $\alpha \in I$ *sao cho* $u_\alpha(y) \neq u_\alpha(z)$.

Vì quan hệ $u_\alpha = f_\alpha \circ u$ có nghĩa là đối với mỗi $y \in F$ ta có

$$\mathrm{pr}_\alpha(u(y)) = u_\alpha(y);$$

phần tử $u(y) \in \prod_{\alpha \in I} E_\alpha$ được xác định duy nhất bởi $u(y) = (u_\alpha(y))_{\alpha \in I}$. Còn phải chứng minh rằng $u(y) \in E$ với mọi $y \in F$, nói cách khác, rằng

$$\mathrm{pr}_\alpha(u(y)) = f_{\alpha\beta}(\mathrm{pr}_\beta(u(y)))$$

mỗi khi $\alpha \leqslant \beta$. Nhưng điều này có thể được viết dưới dạng

$$u_\alpha(y) = f_{\alpha\beta}(u_\beta(y))$$

và do đó suy ra từ (5). Phần thứ hai của Mệnh đề suy ra ngay lập tức từ các định nghĩa.

#### Hệ quả 1 {#ens-iii-s7-prop-1-cor-1 .statement tag=03RN}

*Cho* $(E_\alpha, f_{\alpha\beta})$ *và* $(F_\alpha, g_{\alpha\beta})$ *là hai hệ nghịch đảo các tập hợp đối với cùng một tập hợp chỉ số* I; *đặt* $E = \varprojlim E_\alpha$, $F = \varprojlim F_\alpha$, *và đặt* $f_\alpha$ *(tương ứng,* $g_\alpha$*) là ánh xạ chính tắc của* E *vào* $E_\alpha$ *(tương ứng của* F *vào* $F_\alpha$*) với mỗi* $\alpha \in I$, *Với mỗi* $\alpha \in I$, *cho* $u_\alpha$ *là một ánh xạ từ* E *vào* $F_\alpha$ *sao cho biểu đồ*

$$\begin{array}{ccc} E_\beta & \overset{u_\beta}{\longrightarrow} & F_\beta \\ {\scriptstyle f_{\alpha\beta}}\big\downarrow & & \big\downarrow{\scriptstyle g_{\alpha\beta}} \\ E_\alpha & \underset{u_\alpha}{\longrightarrow} & F_\alpha \end{array}$$

*giao hoán* (\*)[^1] *khi* $\alpha \leqslant \beta$. *Khi đó tồn tại một ánh xạ duy nhất* $u : E \to F$ *sao cho với mỗi* $\alpha \in I$ *biểu đồ*

$$\begin{array}{ccc} E & \overset{u}{\longrightarrow} & F \\ {\scriptstyle f_\alpha}\big\downarrow & & \big\downarrow{\scriptstyle g_\alpha} \\ E_\alpha & \underset{u_\alpha}{\longrightarrow} & F_\alpha \end{array}$$

*giao hoán.*

Đặt $v_\alpha = u_\alpha \circ f_\alpha$. Nếu $\alpha \leqslant \beta$, theo (2), ta có

$$g_{\alpha\beta} \circ v_\beta = g_{\alpha\beta} \circ u_\beta \circ f_\beta = u_\alpha \circ f_{\alpha\beta} \circ f_\beta = u_\alpha \circ f_\alpha = v_\alpha,$$

và do đó ta có thể áp dụng Mệnh đề 1 cho các ánh xạ $v_\alpha$; suy ra sự

tồn tại và tính duy nhất của một ánh xạ $u:E\to F$ sao cho

$$
g_\alpha\circ u=v_\alpha=u_\alpha\circ f_\alpha
$$

với mỗi $\alpha\in I$.

¶ Một họ các ánh xạ $u_\alpha:E_\alpha\to F_\alpha$ thỏa mãn các điều kiện của Hệ quả 1 được gọi là một *hệ ngược các ánh xạ* của $(E_\alpha,f_{\alpha\beta})$ vào $(F_\alpha,g_{\alpha\beta})$. Ánh xạ $u$ được định nghĩa trong Hệ quả 1 được gọi là *giới hạn ngược* của họ $(u_\alpha)$ và được viết là $u=\underset{\leftarrow}{\lim}\,u_\alpha$ khi không có nguy cơ nhầm lẫn.

#### Hệ quả 2 {#ens-iii-s7-prop-1-cor-2 .statement tag=03RO}

Cho $(E_\alpha,f_{\alpha\beta})$, $(F_\alpha,g_{\alpha\beta})$, $(G_\alpha,h_{\alpha\beta})$ là ba *hệ ngược của các tập hợp tương đối với cùng một tập chỉ số* $I$; cho $E=\underset{\leftarrow}{\lim}\,E_\alpha$, $F=\underset{\leftarrow}{\lim}\,F_\alpha$, $G=\underset{\leftarrow}{\lim}\,G_\alpha$, và cho $f_\alpha$ (resp. $g_\alpha,h_\alpha$) là *ánh xạ chính tắc* của $E$ (resp. $F,G$) *vào* $E_\alpha$ (resp. $F_\alpha,G_\alpha$). Nếu $(u_\alpha)$ và $(v_\alpha)$ là *hai hệ ngược của các ánh xạ*, $u_\alpha:E_\alpha\to F_\alpha$, $v_\alpha:F_\alpha\to G_\alpha$, thì các *ánh xạ hợp thành* $v_\alpha\circ u_\alpha:E_\alpha\to G_\alpha$ lập thành một *hệ ngược của các ánh xạ*, và ta có

(7)

$$
\underset{\leftarrow}{\lim}\,(v_\alpha\circ u_\alpha)
=
\left(\underset{\leftarrow}{\lim}\,v_\alpha\right)\circ
\left(\underset{\leftarrow}{\lim}\,u_\alpha\right).
$$

Thật vậy, nếu đặt $w_\alpha=v_\alpha\circ u_\alpha$, thì với $\alpha\leq\beta$ ta có

$$
w_\alpha\circ f_{\alpha\beta}
=v_\alpha\circ(u_\alpha\circ f_{\alpha\beta})
=v_\alpha\circ(g_{\alpha\beta}\circ v_\beta)
=(h_{\alpha\beta}\circ v_\beta)\circ u_\beta
=h_{\alpha\beta}\circ w_\beta,
$$

suy ra $(w_\alpha)$ là một hệ ngược các ánh xạ. Hơn nữa, nếu $u=\underset{\leftarrow}{\lim}\,u_\alpha$ và $v=\underset{\leftarrow}{\lim}\,v_\alpha$, thì $h_\alpha\circ(v\circ u)=(v_\alpha\circ g_\alpha)\circ u=(v_\alpha\circ u_\alpha)\circ f_\alpha$ với mỗi $\alpha\in I$, và do đó, theo tính duy nhất của giới hạn ngược, ta có $v\circ u=\underset{\leftarrow}{\lim}\,w_\alpha$.

¶ Cho $(E_\alpha,f_{\alpha\beta})$ là một hệ ngược các tập hợp, và với mỗi $\alpha\in I$ cho $M_\alpha$ là một tập con của $E_\alpha$. Nếu $f_{\alpha\beta}(M_\beta)\subset M_\alpha$ mỗi khi $\alpha\leq\beta$, thì các $M_\alpha$ được gọi là tạo thành một *hệ ngược các tập con* của các $E_\alpha$. Cho $g_{\alpha\beta}$ là ánh xạ của $M_\beta$ vào $M_\alpha$ (trong đó $\alpha\leq\beta$) có đồ thị trùng với đồ thị của hạn chế của $f_{\alpha\beta}$ lên $M_\beta$. Khi đó rõ ràng $(M_\alpha,g_{\alpha\beta})$ là một hệ ngược các tập hợp và rằng

(8)

$$
\underset{\leftarrow}{\lim}\,M_\alpha
=
\left(\underset{\leftarrow}{\lim}\,E_\alpha\right)\cap\prod_{\alpha\in I}M_\alpha.
$$

#### Mệnh đề 2 {#ens-iii-s7-prop-2 .statement tag=03RP}

Cho $(E_\alpha,f_{\alpha\beta})$ và $(E'_\alpha,f'_{\alpha\beta})$ là hai *hệ ngược của các tập hợp tương đối với* $I$, và cho $u_\alpha$ là một ánh xạ từ $E_\alpha$ vào $E'_\alpha$ với mỗi $\alpha\in I$, sao cho các $u_\alpha$ tạo thành một *hệ ngược của các ánh xạ*. Đặt $u=\underset{\leftarrow}{\lim}\,u_\alpha$. Khi đó với mỗi $x'=(x'_\alpha)\in E'=\underset{\leftarrow}{\lim}\,E'_\alpha$, các $\bar u_\alpha^{-1}(x'_\alpha)$ tạo thành một *hệ ngược của các tập con* của các $E_\alpha$, và $\bar u^{-1}(x')=\underset{\leftarrow}{\lim}\,\bar u_\alpha^{-1}(x'_\alpha)$.

Thật vậy, nếu $\alpha \leqslant \beta$ và $x_\beta \in \overset{-1}{u_\beta}(x'_\beta)$, thì ta có

$$u_\alpha(f_{\alpha\beta}(x_\beta)) = f'_{\alpha\beta}(u_\beta(x_\beta)) = f'_{\alpha\beta}(x'_\beta) = x'_\alpha,$$

từ đó mệnh đề thứ nhất suy ra; và nói rằng $x = (x_\alpha) \in \mathrm{E} = \varprojlim \mathrm{E}_\alpha$ sao cho $u(x) = x'$ theo định nghĩa có nghĩa là $u_\alpha(x_\alpha) = x'_\alpha$ với mỗi $\alpha \in \mathrm{I}$.

#### Hệ quả {#ens-iii-s7-n2-cor-1 .statement tag=03OD}

*Nếu $u_\alpha$ là đơn ánh* (tương ứng, *song ánh*) *với mọi $\alpha \in \mathrm{I}$, thì $u$ là đơn ánh* (tương ứng, *song ánh*).

Với ký hiệu của Mệnh đề 2, các ảnh $u_\alpha(\mathrm{E}_\alpha)$ cũng tạo thành một hệ ngược các tập con của các $\mathrm{E}'_\alpha$, và ta có

(9) $$u(\mathrm{E}) \subset \varprojlim u_\alpha(\mathrm{E}_\alpha);$$

nhưng hai vế của quan hệ này *không tất yếu bằng nhau* (Bài tập 4).

#### Mệnh đề 3 {#ens-iii-s7-prop-3 .statement tag=03OE}

*Cho $\mathrm{I}$ là một tập hợp tiền thứ tự, cho $(\mathrm{E}_\alpha, f_{\alpha\beta})$ là một hệ ngược các tập hợp tương đối với $\mathrm{I}$, và cho $\mathrm{E} = \varprojlim \mathrm{E}_\alpha$. Cho $\mathrm{J}$ là một tập con đồng cuối của $\mathrm{I}$ sao cho $\mathrm{J}$ phải có hướng, và cho $\mathrm{E}'$ là giới hạn ngược của hệ ngược các tập hợp thu được từ $(\mathrm{E}_\alpha, f_{\alpha\beta})$ bằng cách hạn chế tập hợp chỉ số vào $\mathrm{J}$. Khi đó ánh xạ chính tắc $g$ từ $\mathrm{E}$ vào $\mathrm{E}'$* (no. 1, *công thức* (3)) *là song ánh*.

Với mỗi $\alpha \in \mathrm{J}$, đặt $f'_\alpha$ là ánh xạ chính tắc $\mathrm{E}' \to \mathrm{E}_\alpha$. Khi đó, theo (2) và (5), $g$ là ánh xạ duy nhất từ $\mathrm{E}$ vào $\mathrm{E}'$ sao cho $f_\alpha = f'_\alpha \circ g$ với mọi $\alpha \in \mathrm{J}$ (Mệnh đề 1). Ta sẽ chứng minh rằng $g$ là đơn ánh bằng cách dùng tiêu chuẩn của Mệnh đề 1. Nếu $x$, $y$ là các phần tử phân biệt của $\mathrm{E}$, thì theo định nghĩa tồn tại $\alpha \in \mathrm{I}$ sao cho $f_\alpha(x) \neq f_\alpha(y)$; do $\mathrm{J}$ là đồng cuối trong $\mathrm{I}$, tồn tại $\lambda \in \mathrm{J}$ sao cho $\alpha \leqslant \lambda$; vì $f_{\alpha\lambda}(f_\lambda(x)) \neq f_{\alpha\lambda}(f_\lambda(y))$, nên ta có $f_\lambda(x) \neq f_\lambda(y)$. Còn phải chứng minh rằng $g$ là toàn ánh. Lấy $x' = (x'_\lambda)_{\lambda \in \mathrm{J}}$ là một phần tử của $\mathrm{E}'$. Với mỗi $\alpha \in \mathrm{I}$ tồn tại $\lambda \in \mathrm{J}$ sao cho $\alpha \leqslant \lambda$, và phần tử $f_{\alpha\lambda}(x'_\lambda)$ không phụ thuộc vào chỉ số $\lambda \in \mathrm{J}$ sao cho $\alpha \leqslant \lambda$; thật vậy, nếu $\mu \in \mathrm{J}$ sao cho $\alpha \leqslant \mu$, thì tồn tại $\nu \in \mathrm{J}$ sao cho $\lambda \leqslant \nu$ và $\mu \leqslant \nu$, do đó $f_{\alpha\lambda}(x'_\lambda) = f_{\alpha\lambda}(f_{\lambda\nu}(x'_\nu)) = f_{\alpha\nu}(x'_\nu)$, và tương tự $f_{\alpha\mu}(x'_\mu) = f_{\alpha\nu}(x'_\nu)$. Gọi $x_\alpha$ là giá trị chung của các $f_{\alpha\lambda}(x'_\lambda)$ ứng với các $\lambda \in \mathrm{J}$ sao cho $\alpha \leqslant \lambda$, và đặt $x = (x_\alpha)_{\alpha \in \mathrm{I}}$. Khi đó $x \in \mathrm{E}$, vì nếu $\alpha \leqslant \beta$ và nếu $\lambda \in \mathrm{J}$ sao cho $\beta \leqslant \lambda$, thì ta có

$$f_{\alpha\beta}(x_\beta) = f_{\alpha\beta}(f_{\beta\lambda}(x'_\lambda)) = f_{\alpha\lambda}(x'_\lambda) = x_\alpha.$$

Cuối cùng, ta có $x'_\lambda = f_{\lambda\lambda}(x'_\lambda)$ với mọi $\lambda \in \mathrm{J}$, do đó $x_\lambda = x'_\lambda$ với mọi $\lambda \in \mathrm{J}$; nói cách khác, $f(x_\lambda) = x'_\lambda$, và do đó $g(x) = x'$. Vậy $g$ là toàn ánh và chứng minh đã hoàn tất.

Đặc biệt, nếu $\mathrm{I}$ có một *phần tử lớn nhất* $\omega$, ta có thể lấy $\mathrm{J} = \{\omega\}$, sao cho $\varprojlim \mathrm{E}_\alpha$ được đồng nhất một cách chính tắc với $\mathrm{E}_\omega$.

*Nhận xét*

#### Nhận xét 1 {#ens-iii-s7-n2-rem-1 .statement tag=03TH}

Với mỗi $\alpha \in I$ đặt $E'_\alpha = f_\alpha(E)$. Khi đó các tập hợp $E'_\alpha$ tạo thành một *hệ ngược các tập con* của các $E_\alpha$ vì lý do của (2), và ngay lập tức rõ rằng $\varprojlim E'_\alpha = E = \varprojlim E_\alpha$. Ánh xạ $f'_{\alpha\beta} : E'_\beta \to E'_\alpha$ (trong đó $\alpha \leqslant \beta$), mà đồ thị là cùng một đồ thị như đồ thị của hạn chế của $f_{\alpha\beta}$ lên $E_\beta$, là *toàn ánh*, và ta có

$$(10) \qquad E'_\alpha = f_\alpha(E) \subset \bigcap_{\beta \geqslant \alpha} f_{\alpha\beta}(E_\beta)$$

với mọi $\alpha \in I$.

#### Nhận xét 2 {#ens-iii-s7-n2-rem-2 .statement tag=03TI}

Cho I là một tập hợp có thứ tự (*phải*) *có hướng*, cho $(E_\alpha, f_{\alpha\beta})$ là một hệ ngược các tập hợp tương đối với I, và với mỗi $\alpha \in I$ cho $u_\alpha : F \to E_\alpha$ là một ánh xạ sao cho họ $(u_\alpha)$ thỏa mãn công thức (5). Xét hệ ngược $(F_\alpha, i_{\alpha\beta})$ được đánh chỉ số bởi I, trong đó $F_\alpha = F$ với mọi $\alpha \in I$ và $i_{\alpha\beta}$ là ánh xạ đồng nhất của F. Khi đó (no. 1, Ví dụ 2) F được đồng nhất một cách chính tắc với $\varprojlim F_\alpha$. Nếu ta xét $u_\alpha$ như một ánh xạ từ $F_\alpha$ vào $E_\alpha$, thì $(u_\alpha)$ là một hệ ngược các ánh xạ, và ánh xạ $u : F \to E$ được định nghĩa bởi (6) được đồng nhất với giới hạn ngược của hệ các ánh xạ này. Do đó, theo lối nói lạm dụng, ta viết $u = \varprojlim u_\alpha$.

#### Nhận xét 3 {#ens-iii-s7-n2-rem-3 .statement tag=03TJ}

Cho I là một tập hợp có thứ tự và $(E_\alpha, f_{\alpha\beta})$ là một hệ ngược các tập hợp tương đối với I. Với mỗi tập con hữu hạn J của I, gọi $F_J$ là giới hạn ngược của hệ ngược (hữu hạn) thu được từ $(E_\alpha, f_{\alpha\beta})$ bằng cách hạn chế tập hợp chỉ số vào J. Nếu J và K là hai tập con hữu hạn bất kỳ của I sao cho $J \subset K$, ký hiệu $g_{JK}$ là ánh xạ chính tắc (3) từ $F_K$ vào $F_J$. Khi đó quan hệ (4) cho thấy rằng $(F_J, g_{JK})$ là một *hệ ngược* các tập hợp tương đối với tập hợp *có hướng* (đối với quan hệ $\subset$) $\mathfrak{F}(I)$ gồm các tập con hữu hạn của I. Tiếp theo, với mỗi $J \in \mathfrak{F}(I)$, gọi $h_J : E \to F_J$ là ánh xạ chính tắc (3). Theo (4) và với sự lạm dụng ngôn ngữ đã nói ở Chú ý (2), $(h_J)$ là một *hệ ngược* các ánh xạ. Đặt $h = \varprojlim h_J : E \to F = \varprojlim F_J$, và ta sẽ chỉ ra rằng $h$ là một *song ánh* (gọi là *chính tắc*). Thật vậy, lấy $y = (y_J) \in F$. Theo định nghĩa ta có $y_J = (x_{\alpha, J})_{\alpha \in J}$, trong đó $x_{\alpha, J} \in E_\alpha$ với mọi $\alpha \in J$. Nếu $J \subset K$, thì theo định nghĩa của ánh xạ $g_{JK}$ và vì $y_J = g_{JK}(y_K)$, ta có $x_{\alpha, J} = x_{\alpha, K}$ với mọi $\alpha \in J$. Bởi vậy, với mỗi $\alpha \in I$, có một phần tử duy nhất $x_\alpha \in E_\alpha$ sao cho $x_\alpha = x_{\alpha, J}$ đối với mọi tập con hữu hạn J của I chứa $\alpha$. Nếu $\alpha \leqslant \beta$, tồn tại một tập con hữu hạn J của I chứa cả $\alpha$ và $\beta$; do đó $x_\alpha = f_{\alpha\beta}(x_\beta)$ theo định nghĩa. Do đó $x = (x_\alpha)$ là phần tử duy nhất của E sao cho $h(x) = y$.

### 3. GIỚI HẠN NGƯỢC KÉP

Cho I, L là hai tập hợp tiền thứ tự, và $I \times L$ là tích của chúng (§ 1, no. 4). Xét một hệ ngược của các tập hợp $(E^\lambda_\alpha, f^{\lambda\mu}_{\alpha\beta})$ tương đối với tập hợp chỉ số $I \times L$.

Ta có

(11) $\qquad f^{\lambda\nu}_{\alpha\gamma} = f^{\lambda\mu}_{\alpha\beta} \circ f^{\mu\nu}_{\beta\gamma}$ khi $\alpha \leqslant \beta \leqslant \gamma$ và $\lambda \leqslant \mu \leqslant \nu$.

Ký hiệu E hoặc $\lim \mathrm{E}^{\lambda}_{\alpha}$ là giới hạn ngược của hệ ngược này.

Với mỗi $\lambda \in \mathrm{L}$, đặt $g^{\lambda}_{\alpha\beta} = f^{\lambda\lambda}_{\alpha\beta} : \mathrm{E}^{\lambda}_{\beta} \to \mathrm{E}^{\lambda}_{\alpha}$. Từ (11) suy ra

(12) $\qquad g^{\lambda}_{\alpha\gamma} = g^{\lambda}_{\alpha\beta} \circ g^{\lambda}_{\beta\gamma}$ khi $\alpha \leqslant \beta \leqslant \gamma$,

sao cho $(\mathrm{E}^{\lambda}_{\alpha}, g^{\lambda}_{\alpha\beta})$ là một hệ ngược của các tập hợp đối với I. Ký hiệu $\mathrm{F}^{\lambda} = \lim \mathrm{E}^{\lambda}_{\alpha}$ là giới hạn ngược của nó. Với $\lambda \leqslant \mu$ cố định trong L, từ (11) suy ra rằng các $h^{\lambda\mu}_{\alpha} = f^{\lambda\mu}_{\alpha\alpha} : \mathrm{E}^{\mu}_{\alpha} \to \mathrm{E}^{\lambda}_{\alpha}$ tạo thành một hệ ngược các ánh xạ, mà giới hạn ngược của nó được ký hiệu bởi $h^{\lambda\mu} = \lim h^{\lambda\mu}_{\alpha} : \mathrm{F}^{\mu} \to \mathrm{F}^{\lambda}$. Nếu $\lambda \leqslant \mu \leqslant \nu$ trong L, ta có

(13) $$h^{\lambda\nu} = h^{\lambda\mu} \circ h^{\mu\nu}$$

(no. 2, Mệnh đề 2, Hệ quả 2); do đó $(\mathrm{F}^{\lambda}, h^{\lambda\mu})$ là một hệ ngược các tập hợp tương đối với L. Gọi $\mathrm{F} = \lim \mathrm{F}^{\lambda}$ là giới hạn ngược của nó. Ta sẽ định nghĩa một *song ánh chính tắc* $\mathrm{F} \to \mathrm{E}$. Để làm điều này, ta chú ý rằng F theo định nghĩa là một tập con của $\prod_{\lambda \in \mathrm{L}} \mathrm{F}^{\lambda}$, và $\mathrm{F}^{\lambda}$ là một tập con của $\prod_{\alpha \in \mathrm{I}} \mathrm{E}^{\lambda}_{\alpha}$; do đó F có thể được đồng nhất một cách chính tắc với một tập con của $\prod_{(\alpha, \lambda) \in \mathrm{I} \times \mathrm{L}} \mathrm{E}^{\lambda}_{\alpha} = \mathrm{G}$ (Chương II, § 5, no. 5, Mệnh đề 7). Với mỗi $z \in \mathrm{G}$, gọi $\mathrm{pr}^{\lambda}(z)$ là phần tử $(\mathrm{pr}^{\lambda}_{\alpha}(z))_{\alpha \in \mathrm{I}}$ của $\prod_{\alpha \in \mathrm{I}} \mathrm{E}^{\lambda}_{\alpha}$. Khi đó $z \in \mathrm{F}$ khi và chỉ khi

(14) $\qquad \mathrm{pr}^{\lambda}(z) = h^{\lambda\mu}(\mathrm{pr}^{\mu}(z))$ mỗi khi $\lambda \leqslant \mu$ trong L

và $\mathrm{pr}^{\lambda}(z) \in \mathrm{F}^{\lambda}$ với mọi $\lambda \in \mathrm{L}$; nghĩa là, mỗi khi $\alpha \leqslant \beta$ trong I thì ta có

(15) $$\mathrm{pr}^{\lambda}_{\alpha}(z) = f^{\lambda\lambda}_{\alpha\beta}(\mathrm{pr}^{\lambda}_{\beta}(z)).$$

Nhưng $h^{\lambda\mu}(\mathrm{pr}^{\mu}(z)) = (f^{\mu\lambda}_{\alpha\alpha}(\mathrm{pr}^{\mu}_{\alpha}(z))_{\alpha \in \mathrm{I}}$; do đó suy ra từ (14) và (15) rằng nếu $\alpha \leqslant \beta$ và $\lambda \leqslant \mu$, thì ta có

$$\mathrm{pr}^{\lambda}_{\alpha}(z) = f^{\lambda\mu}_{\alpha\alpha}(f^{\mu\mu}_{\alpha\beta}(\mathrm{pr}^{\mu}_{\beta}(z))) = f^{\lambda\mu}_{\alpha\beta}(\mathrm{pr}^{\mu}_{\beta}(z)),$$

điều này kéo theo rằng $z \in \mathrm{E}$. Mệnh đề đảo lại là hiển nhiên, và vì vậy ta đã chứng minh

#### Mệnh đề 4 {#ens-iii-s7-prop-4 .statement tag=03OF}

*Nếu* $(\mathrm{E}^\lambda_\alpha, f^{\lambda\mu}_{\alpha\beta})$ *là một hệ ngược các tập hợp tương đối với một tích* $\mathrm{I} \times \mathrm{L}$ *của các tập hợp tiền thứ tự, thì (sai khác một song ánh chính tắc) ta có*

$$(16) \qquad \varprojlim_{\alpha,\lambda} \mathrm{E}^\lambda_\alpha = \varprojlim_\lambda \; (\varprojlim_\alpha \mathrm{E}^\lambda_\alpha).$$

#### Hệ quả 1 {#ens-iii-s7-prop-4-cor-1 .statement tag=03OG}

*Cho* $(\mathrm{E}'^\lambda_\alpha, f'^{\mu\lambda}_{\alpha\beta})$ *là một hệ ngược khác của các tập hợp tương đối với* $\mathrm{I} \times \mathrm{L}$, *và với mỗi* $(\alpha, \lambda) \in \mathrm{I} \times \mathrm{L}$ *cho* $u^\lambda_\alpha$ *là một ánh xạ từ* $\mathrm{E}^\lambda_\alpha$ *vào* $\mathrm{E}'^\lambda_\alpha$ *sao cho các* $u^\lambda_\alpha$ *tạo thành một hệ ngược các ánh xạ. Khi đó*

$$(17) \qquad \varprojlim_{\alpha,\lambda} u^\lambda_\alpha = \varprojlim_\lambda \; (\varprojlim_\alpha u^\lambda_\alpha).$$

Việc kiểm tra tương tự như đối với Mệnh đề 4.

#### Hệ quả 2 {#ens-iii-s7-prop-4-cor-2 .statement tag=03OH}

*Cho* $(\mathrm{E}^\lambda_\alpha, f^\lambda_{\alpha\beta})_{\lambda \in \mathrm{L}}$ *là một họ các hệ ngược của các tập hợp tương đối với* I. *Nếu* $\prod_{\lambda \in \mathrm{L}} f^\lambda_{\alpha\beta}$ *ký hiệu mở rộng lên các tích* (Chương II, § 5, no. 7, Định nghĩa 2) *của họ các ánh xạ* $(f^\lambda_{\alpha\beta})_{\lambda \in \mathrm{L}}$, *thì* $\left( \prod_{\lambda \in \mathrm{L}} \mathrm{E}^\lambda_\alpha, \prod_{\lambda \in \mathrm{L}} f^\lambda_{\alpha\beta} \right)$ *là một hệ ngược của các tập hợp tương đối với* I, *và (cho đến một song ánh chính tắc) ta có*

$$(18) \qquad \varprojlim_\alpha \prod_{\lambda \in \mathrm{L}} \mathrm{E}^\lambda_\alpha = \prod_{\lambda \in \mathrm{L}} (\varprojlim_\alpha \mathrm{E}^\lambda_\alpha).$$

Xét hệ ngược kép $(\mathrm{E}^\lambda_\alpha, g^{\lambda\mu}_{\alpha\beta})$ tương đối với $\mathrm{I} \times \mathrm{L}$, trong đó quan hệ thứ tự trên L là đẳng thức (no. 1, Ví dụ 1), và áp dụng Mệnh đề 4.

### 4. ĐIỀU KIỆN ĐỂ MỘT GIỚI HẠN NGƯỢC KHÔNG RỖNG

Trong tiểu mục này chúng tôi sẽ nêu ra hai điều kiện đủ được dùng thường xuyên nhất để một giới hạn ngược không rỗng (xem thêm Bài tập 5).

#### Mệnh đề 5 {#ens-iii-s7-prop-5 .statement tag=03OI}

*Cho* $(\mathrm{E}_\alpha, f_{\alpha\beta})$ *là một hệ ngược các tập hợp đối với một tập hợp* có hướng I *có một tập con đồng tận* đếm được, *và giả sử thêm rằng các* $f_{\alpha\beta}$ *là* toàn ánh. *Khi đó, nếu* $\mathrm{E} = \varprojlim \mathrm{E}_\alpha$, *thì ánh xạ chính tắc* $f_\alpha : \mathrm{E} \to \mathrm{E}_\alpha$ *là* toàn ánh *với mọi* $\alpha \in \mathrm{I}$ *(và, a fortiori,* E *không rỗng nếu không một* $\mathrm{E}_\alpha$ *nào là rỗng).*

Lấy $(\alpha_n)$ là một dãy các phần tử của I tạo thành một tập con đồng tận của I. Vì I có hướng, ta có thể định nghĩa quy nạp một dãy $(\beta_n)$ các phần tử của I bởi các điều kiện $\beta_0 = \alpha_0, \beta_n \geqslant \beta_i$ với $i < n$ và $\beta_n \geqslant \alpha_n$. Rõ ràng dãy $(\beta_n)$ là tăng và tạo thành một tập con đồng tận của I. Theo Mệnh đề 1 của no. 1 và các hệ thức $f_\alpha = f_{\alpha\beta_n} \circ f_{\beta_n}$ đối với

$\alpha \leqslant \beta_n$, ta chỉ cần chứng minh Mệnh đề trong trường hợp $\mathrm{I} = \mathbf{N}$. Hơn nữa, hiển nhiên là chỉ cần chứng minh rằng $f_0$ là toàn ánh. Lấy $x_0 \in \mathrm{E}_0$. Định nghĩa quy nạp $x_n \in \mathrm{E}_n$ (với $n \geqslant 1$) là một phần tử của tập hợp $\overset{-1}{f}_{n-1,n}(x_{n-1})$, điều này là có thể vì tập hợp sau không rỗng theo giả thiết. Khi đó ta chứng minh bằng quy nạp theo $n - m$ rằng $x_m = f_{mn}(x_n)$ với $m \leqslant n$, và suy ra $x = (x_n)$ thuộc E.

Tiêu chuẩn thứ hai liên quan đến các hệ nghịch đảo $(\mathrm{E}_\alpha, f_{\alpha\beta})$ tương đối với một tập hợp chỉ số I sao cho với mỗi $\alpha \in \mathrm{I}$ ta được cho một tập hợp $\mathfrak{S}_\alpha$ gồm các tập con của $\mathrm{E}_\alpha$ thỏa mãn các điều kiện sau :

(i)  *Mọi giao của các tập hợp thuộc $\mathfrak{S}_\alpha$ cũng thuộc $\mathfrak{S}_\alpha$.*

Đặc biệt suy ra (bằng cách xét giao của họ rỗng) rằng $\mathrm{E}_\alpha \in \mathfrak{S}_\alpha$.

(ii)  *Nếu một tập hợp các tập con $\mathfrak{F} \subset \mathfrak{S}_\alpha$ có tính chất là mọi giao hữu hạn của các tập hợp thuộc $\mathfrak{F}$ đều khác rỗng, thì $\bigcap\limits_{\mathbf{M} \in \mathfrak{F}} \mathrm{M}$ khác rỗng.*

Theo (i), hiển nhiên là (ii) tương đương với điều kiện sau đây :

(ii)′  *Nếu $\mathfrak{G} \subset \mathfrak{S}_\alpha$ có hướng trái (đối với quan hệ bao hàm) và không chứa tập rỗng, thì $\bigcap\limits_{\mathbf{M} \in \mathfrak{G}} \mathrm{M}$ khác rỗng.*

#### Định lý 1 {#ens-iii-s7-thm-1 .statement tag=03RQ}

*Giả sử rằng I có hướng, các tập hợp $\mathfrak{S}_\alpha$ thỏa mãn các điều kiện* (i) *và* (ii), *và hệ ngược $(\mathrm{E}_\alpha, f_{\alpha\beta})$ có tính chất sau:*

(iii)  *Với mỗi cặp chỉ số $\alpha$, $\beta$ sao cho $\alpha \leqslant \beta$, và mỗi $x_\alpha \in \mathrm{E}_\alpha$, ta có $\overset{-1}{f}_{\alpha\beta}(x_\alpha) \in \mathfrak{S}_\beta$.*

(iv)  *Với mỗi cặp chỉ số $\alpha$, $\beta$ sao cho $\alpha \leqslant \beta$, và với mỗi $\mathrm{M}_\beta \in \mathfrak{S}_\beta$, ta có $f_{\alpha\beta}(\mathrm{M}_\beta) \in \mathfrak{S}_\alpha$.*

*Đặt $\mathrm{E} = \varprojlim \mathrm{E}_\alpha$ và gọi $f_\alpha : \mathrm{E} \to \mathrm{E}_\alpha$ là ánh xạ chính tắc với mỗi $\alpha \in \mathrm{I}$. Khi đó:*

(a)  *Với mỗi $\alpha \in \mathrm{I}$ ta có*

$$(19) \qquad f_\alpha(\mathrm{E}) = \bigcap_{\beta \geqslant \alpha} f_{\alpha\beta}(\mathrm{E}_\beta).$$

(b)  *Nếu $\mathrm{E}_\alpha$ không rỗng với mỗi $\alpha \in \mathrm{I}$, thì E không rỗng.*

Gọi $\Sigma$ là tập hợp các họ $\mathfrak{A} = (\mathrm{A}_\alpha)_{\alpha \in \mathrm{I}}$ thỏa mãn các điều kiện sau :

$$(20) \qquad \mathrm{A}_\alpha \neq \emptyset \quad \textit{và} \quad \mathrm{A}_\alpha \in \mathfrak{S}_\alpha \quad \textit{với mọi} \quad \alpha \in \mathrm{I};$$

$$(21) \qquad f_{\alpha\beta}(\mathrm{A}_\beta) \subset \mathrm{A}_\alpha \quad \textit{khi} \quad \alpha \leqslant \beta.$$

Nếu $\mathfrak{A} = (A_\alpha)$ và $\mathfrak{A}' = (A'_\alpha)$ là hai phần tử bất kỳ của $\Sigma$, gọi quan hệ $\mathfrak{A} \leqslant \mathfrak{A}'$ là quan hệ $A_\alpha \supset A'_\alpha$ với mọi $\alpha$. Rõ ràng $\Sigma$ có thứ tự theo quan hệ này.

(1) Trước hết, hãy chỉ ra rằng tập hợp có thứ tự $\Sigma$ là *quy nạp*. Cho L là một tập sắp thứ tự toàn phần và $\lambda \to \mathfrak{A}^\lambda = (A^\lambda_\alpha)_{\alpha \in I}$ là một ánh xạ tăng ngặt từ L vào $\Sigma$. Với mỗi $\alpha \in I$, đặt $B_\alpha = \bigcap_{\lambda \in L} A^\lambda_\alpha$. Khi đó ngay lập tức thấy rằng họ $\mathfrak{B} = (B_\alpha)_{\alpha \in I}$ thỏa mãn (21); do (i) và (ii), nó cũng thỏa mãn (20), nên thuộc $\Sigma$; và hiển nhiên $\mathfrak{B}$ là một cận trên của tập hợp các $\mathfrak{A}^\lambda$.

(2) Cho $\mathfrak{A} = (A_\alpha)$ là một phần tử *cực đại* của $\Sigma$. Ta sẽ chỉ ra rằng $A_\alpha = f_{\alpha\beta}(A_\beta)$ với mọi $\alpha \leqslant \beta$. Đặt $A'_\alpha = \bigcap_{\beta \geqslant \alpha} f_{\alpha\beta}(A_\beta)$ với mọi $\alpha \in I$, và hãy chỉ ra rằng $\mathfrak{A}' = (A'_\alpha)$ thuộc $\Sigma$. Trước hết lưu ý rằng nếu $\alpha \leqslant \beta \leqslant \gamma$, thì ta có $f_{\alpha\gamma}(A_\gamma) = f_{\alpha\beta}(f_{\beta\gamma}(A_\gamma)) \subset f_{\alpha\beta}(A_\beta)$ theo (21); hơn nữa, $f_{\alpha\beta}(A_\beta) \in \mathfrak{S}_\alpha$ theo (iv), và $f_{\alpha\beta}(A_\beta) \neq \emptyset$ theo (20). Do đó các điều kiện (i) và (ii) cho thấy rằng $\mathfrak{A}'$ thỏa mãn (20). Ngoài ra, nếu $\alpha \leqslant \beta$, ta có

$$f_{\alpha\beta}(A'_\beta) \subset \bigcap_{\gamma \geqslant \beta} f_{\alpha\beta}(f_{\beta\gamma}(A_\gamma)) = \bigcap_{\gamma \geqslant \beta} f_{\alpha\gamma}(A_\gamma);$$

và với mỗi $\delta \geqslant \alpha$ tồn tại $\gamma \in I$ sao cho $\gamma \geqslant \delta$ và $\gamma \geqslant \beta$, nên $f_{\alpha\gamma}(A_\gamma) \subset f_{\alpha\delta}(A_\delta)$ và do đó

$$\bigcap_{\gamma \geqslant \beta} f_{\alpha\gamma}(A_\gamma) = \bigcap_{\delta \geqslant \alpha} f_{\alpha\delta}(A_\delta) = A'_\alpha.$$

Do đó $\mathfrak{A}'$ thỏa mãn (21) và vì thế thuộc $\Sigma$. Vì $A'_\alpha \subset A_\alpha$ với mọi $\alpha$, tính tối đại của $\mathfrak{A}$ trong $\Sigma$ kéo theo $\mathfrak{A}' = \mathfrak{A}$, và mệnh đề của chúng ta đã được chứng minh.

(3) Tiếp theo chúng ta sẽ thiết lập rằng nếu $\mathfrak{A} = (A_\alpha)$ là một phần tử *cực đại* của $\Sigma$, thì mỗi $A_\alpha$ *chỉ gồm một phần tử*. Lấy $x_\alpha \in A_\alpha$. Với mỗi $\beta \geqslant \alpha$, đặt $B_\beta = A_\beta \cap \overset{-1}{f}_{\alpha\beta}(x_\alpha)$; nếu $\beta$ không $\geqslant \alpha$, đặt $B_\beta = A_\beta$; khi đó ta sẽ thấy rằng $\mathfrak{B} = (B_\beta)$ thuộc $\Sigma$. Nếu $\beta$ không $\geqslant \alpha$, quan hệ $\beta \leqslant \gamma$ suy ra $f_{\beta\gamma}(B_\gamma) \subset f_{\beta\gamma}(A_\gamma) \subset A_\beta = B_\beta$. Mặt khác, nếu $\alpha \leqslant \beta \leqslant \gamma$, thì vì

$$\overset{-1}{f}_{\alpha\gamma}(x_\alpha) = \overset{-1}{f}_{\beta\gamma}(\overset{-1}{f}_{\alpha\beta}(x_\alpha)),$$

ta có

$$f_{\beta\gamma}(\overset{-1}{f}_{\alpha\gamma}(x_\alpha)) \subset \overset{-1}{f}_{\alpha\beta}(x_\alpha),$$

và vì $f_{\beta\gamma}(A_\gamma) \subset A_\beta$, ta lại có $f_{\beta\gamma}(B_\gamma) \subset B_\beta$, do đó họ $\mathfrak{B}$ thỏa mãn (21). Vì $A_\alpha = f_{\alpha\beta}(A_\beta)$ mỗi khi $\alpha \leqslant \beta$ theo phần (2) của

chứng minh, hiển nhiên là $\mathrm{B}_\beta \neq \emptyset$ với mọi $\beta \in \mathrm{I}$. Sau cùng, do (i) và (iii), ta có $\mathrm{B}_\beta \in \mathfrak{S}_\beta$ với mọi $\beta \in \mathrm{I}$, và do đó $\mathfrak{B} \in \Sigma$. Vì $\mathrm{B}_\beta \subset \mathrm{A}_\beta$ với mọi $\beta \in \mathrm{I}$, tính tối đại của $\mathfrak{A}$ suy ra $\mathrm{B}_\beta = \mathrm{A}_\beta$ với mọi $\beta$, và đặc biệt $\mathrm{A}_\alpha = \{x_\alpha\}$.

(4) Bây giờ ta đã ở vị trí để chứng minh Định lý 1. Hãy bắt đầu với (a). Ta có

$$f_\alpha(\mathrm{E}) \subset \bigcap_{\beta \geqslant \alpha} f_{\alpha\beta}(\mathrm{E}_\beta).$$

Ngược lại, giả sử

$$x_\alpha \in \bigcap_{\beta \geqslant \alpha} f_{\alpha\beta}(\mathrm{E}_\beta),$$

và đặt

$$\mathrm{B}_\beta = \overset{-1}{f}_{\alpha\beta}(x_\alpha)$$

nếu $\beta \geqslant \alpha$, và $\mathrm{B}_\beta = \mathrm{E}_\beta$ nếu không. Theo định nghĩa của $x_\alpha$, các $\mathrm{B}_\beta$ là không rỗng, và ta có $\mathrm{B}_\beta \in \mathfrak{S}_\beta$ với mọi $\beta \in \mathrm{I}$ theo (iii) và (i); hơn nữa, hiển nhiên là $f_{\beta\gamma}(\mathrm{B}_\gamma) \subset \mathrm{B}_\beta$ mỗi khi $\beta \leqslant \gamma$. Do đó $\mathfrak{B} = (\mathrm{B}_\beta) \in \Sigma$. Gọi $\mathfrak{A} = (\mathrm{A}_\alpha)$ là một phần tử cực đại của $\Sigma$ sao cho $\mathfrak{A} \geqslant \mathfrak{B}$ (sự tồn tại của $\mathfrak{A}$ suy ra từ (1) và §2, no. 4, Định lý 2, Hệ quả 1). Vì, theo (3), $\mathrm{A}_\beta$ có dạng $\{y_\beta\}$ với mọi $\beta \in \mathrm{I}$, suy ra $y = (y_\beta)$ thuộc E, và theo định nghĩa thì $f_\alpha(y) = y_\alpha = x_\alpha$.

Cuối cùng, (a) suy ra (b). Ta có thể giả sử rằng I không rỗng (nếu không thì không có gì phải chứng minh). Giả thiết rằng các $\mathrm{E}_\alpha$ không rỗng suy ra rằng $f_{\alpha\beta}(\mathrm{E}_\beta) \neq \emptyset$ với mọi $\beta \geqslant \alpha$. Vì các $f_{\alpha\beta}(\mathrm{E}_\beta)$, với $\alpha$ cố định và $\beta \geqslant \alpha$ là biến, lập thành một tập có hướng trái các tập con của $\mathrm{E}_\alpha$ thuộc $\mathfrak{S}_\alpha$, điều kiện (ii)$'$ chứng tỏ rằng

$$\bigcap_{\beta \geqslant \alpha} f_{\alpha\beta}(\mathrm{E}_\beta) \neq \emptyset.$$

Do đó $f_\alpha(\mathrm{E}) \neq \emptyset$ theo (a), và *a fortiori* $\mathrm{E} \neq \emptyset$. Q.E.D.

#### Nhận xét {#ens-iii-s7-n4-rem-1 .statement tag=03OJ}

Giả sử rằng điều kiện (iii) trong Định lý 1 được thay bằng điều kiện yếu hơn sau đây :

(iii)$'$ *Với mỗi* $\alpha \in \mathrm{I}$ *và mỗi tập hợp không rỗng* $\mathrm{M}_\alpha \in \mathfrak{S}_\alpha$ *tồn tại* $x_\alpha \in \mathrm{M}_\alpha$ *sao cho* $\overset{-1}{f}_{\alpha\beta}(x_\alpha) \in \mathfrak{S}_\beta$ *với mọi* $\beta \geqslant \alpha$.

Khi đó kết luận (b) của Định lý 1 vẫn đúng; các chứng minh của các phần (1) và (2) của Định lý 1 vẫn không thay đổi và chứng minh của phần (3) vẫn đúng với điều kiện ta cẩn thận lấy $x_\alpha \in \mathrm{A}_\alpha$ sao cho $\overset{-1}{f}_{\alpha\beta}(x_\alpha)$ thuộc $\mathfrak{S}_\beta$ với mọi $\beta \geqslant \alpha$. Cuối cùng, chứng minh của (4) cho thấy rằng nếu

$$\bigcap_{\beta \geqslant \alpha} f_{\alpha\beta}(\mathrm{E}_\beta) \neq \emptyset$$

và nếu ta chọn một $x_\alpha$ trong tập hợp này sao cho $\overset{-1}{f}_{\alpha\beta}(x_\alpha) \in \mathfrak{S}_\beta$ với mọi $\beta \geqslant \alpha$, thì tồn tại $y \in E$ sao cho $f_\alpha(y) = x_\alpha$, điều này chứng minh mệnh đề của chúng ta.

*Ví dụ*

#### Ví dụ 1 {#ens-iii-s7-n4-exa-1 .statement tag=03TK}

Nếu các $E_\alpha$ là những tập hợp *hữu hạn*, thì có thể áp dụng Định lý 1 bằng cách lấy $\mathfrak{S}_\alpha$ là tập hợp của *tất cả* các tập con của $E_\alpha$. \* Ví dụ này được tổng quát hóa trong *Tôpô đại cương* thành trường hợp mà các $E_\alpha$ là những không gian tôpô *compact*, các $f_{\alpha\beta}$ là những ánh xạ *liên tục*, và $\mathfrak{S}_\alpha$ là tập hợp các tập con *đóng* của $E_\alpha$ (*Tôpô đại cương*, Chương I, § 9, no. 6). \*

#### Ví dụ 2 {#ens-iii-s7-n4-exa-2 .statement tag=03TL}

Cho A là một vành có một phần tử đơn vị, và với mỗi $\alpha \in I$ gọi $T_\alpha$ là một A-môđun trái *Artin*. Gọi $E_\alpha$ là một *không gian thuần nhất* của $T_\alpha$ mà trên đó $T_\alpha$ tác động một cách trung thành (để cho $E_\alpha$ là một *không gian afin* gắn với $T_\alpha$). Với $\beta \geqslant \alpha$, giả sử rằng $f_{\alpha\beta} : E_\beta \to E_\alpha$ là một *ánh xạ afin*. Lấy $\mathfrak{S}_\alpha$ là tập hợp gồm tập rỗng và các *đa tạp tuyến tính afin* trong $E_\alpha$. Khi đó điều kiện (i) được thỏa mãn một cách hiển nhiên, và (ii) suy ra từ thực tế rằng $T_\alpha$ là Artin; vì điều đó kéo theo rằng tồn tại một phần tử cực tiểu trong tập hợp các giao hữu hạn của các tập hợp $M \in \mathfrak{F}$, và phần tử cực tiểu này ắt phải bằng $\bigcap_{M \in \mathfrak{F}} M$. Sau hết, vì $f_{\alpha\beta}$ là afin, các điều kiện (iii) và (iv) được thỏa mãn một cách hiển nhiên. \*

### 5. GIỚI HẠN TRỰC TIẾP

Cho I là một tập hợp tiền thứ tự (*phải*) *có hướng* và $(E_\alpha)_{\alpha \in I}$ là một họ các tập hợp được đánh chỉ số bởi I. Với mỗi cặp $(\alpha, \beta)$ các phần tử của I sao cho $\alpha \leqslant \beta$, gọi $f_{\beta\alpha}$ là một *ánh xạ của* $E_\alpha$ *vào* $E_\beta$. Giả sử rằng các $f_{\beta\alpha}$ thỏa mãn các điều kiện sau đây :

(LI$_\mathrm{I}$)  *Các quan hệ* $\alpha \leqslant \beta \leqslant \gamma$ *kéo theo* $f_{\gamma\alpha} = f_{\gamma\beta} \circ f_{\beta\alpha}$.
(LI$_\mathrm{II}$)  *Với mỗi* $\alpha \in I, f_{\alpha\alpha}$ *là ánh xạ đồng nhất của* $E_\alpha$.

Gọi G là tập hợp là *tổng* của họ các tập hợp $(E_\alpha)_{\alpha \in I}$ (Chương II, § 4, no. 8); do lạm dụng ngôn ngữ, ta sẽ đồng nhất các $E_\alpha$ với các ảnh chính tắc của chúng trong G, và với mỗi $x \in G$ ta sẽ ký hiệu bởi $\lambda(x)$ chỉ số duy nhất $\alpha \in I$ sao cho $x \in E_\alpha$. Gọi $R\{x, y\}$ là quan hệ sau đây giữa hai phần tử $x$, $y$ của G : "tồn tại một phần tử $\gamma \in I$ sao cho $\gamma \geqslant \alpha = \lambda(x)$ và $\gamma \geqslant \beta = \lambda(y)$ và sao cho $f_{\gamma\alpha}(x) = f_{\gamma\beta}(y)$". Khi đó R là một *quan hệ tương đương trên* G. Hiển nhiên R là phản xạ và đối xứng trên G. Để chứng minh rằng R bắc cầu, lấy $x \in E_\alpha, y \in E_\beta, z \in E_\gamma$, và giả sử tồn tại $\lambda \in I$ sao cho $\lambda \geqslant \alpha$, $\lambda \geqslant \beta$ và $f_{\lambda\alpha}(x) = f_{\lambda\beta}(y)$, và $\mu \in I$ sao cho $\mu \geqslant \beta$, $\mu \geqslant \gamma$, và $f_{\mu\beta}(y) = f_{\mu\gamma}(z)$. Vì I là một tập có hướng, tồn tại $\nu \in I$ sao cho $\nu \geqslant \lambda$ và $\nu \geqslant \mu$;

theo $(\mathrm{LI_I})$ khi đó ta có

$$f_{\nu\alpha}(x) = f_{\nu\lambda}(f_{\lambda\alpha}(x)) = f_{\nu\lambda}(f_{\lambda\beta}(y)) = f_{\nu\beta}(y)$$
$$= f_{\nu\mu}(f_{\mu\beta}(y)) = f_{\nu\mu}(f_{\mu\gamma}(z)) = f_{\nu\gamma}(z),$$

điều đó thiết lập mệnh đề của chúng ta. Tập thương $\mathrm{E} = \mathrm{G/R}$ được gọi là *giới hạn trực tiếp của họ* $(\mathrm{E}_\alpha)_{\alpha \in \mathrm{I}}$ *đối với họ các ánh xạ* $(f_{\beta\alpha})$, và được viết là $\mathrm{E} = \varinjlim (\mathrm{E}_\alpha, f_{\beta\alpha})$, hoặc đơn giản là $\mathrm{E} = \varinjlim \mathrm{E}_\alpha$ khi không có nguy cơ nhập nhằng. Theo cách nói lạm dụng, cặp $((\mathrm{E}_\alpha), (f_{\beta\alpha}))$ (thường được viết là $(\mathrm{E}_\alpha, f_{\beta\alpha})$) được gọi là một *hệ trực tiếp các tập hợp*, tương đối với tập có hướng I.

¶ Rõ ràng E không rỗng miễn là ít nhất một trong các $\mathrm{E}_\alpha$ không rỗng. Ta ký hiệu bởi $f_\alpha$ hạn chế trên $\mathrm{E}_\alpha$ của ánh xạ chính tắc $f$ của G lên $\mathrm{E} = \mathrm{G/R}$; $f_\alpha$ được gọi là *ánh xạ chính tắc* của $\mathrm{E}_\alpha$ vào E. Nếu $\alpha \leqslant \beta$, ta có quan hệ

(22) $$f_\beta \circ f_{\beta\alpha} = f_\alpha$$

vì với mỗi $x \in \mathrm{E}_\alpha$ ta có $f_{\beta\beta}(f_{\beta\alpha}(x)) = f_{\beta\alpha}(x)$ theo $(\mathrm{LI_I})$; do đó các phần tử $x \in \mathrm{E}_\alpha$ và $f_{\beta\alpha}(x) \in \mathrm{E}_\beta$ là đồng dư mod R.

*Ví dụ*

#### Ví dụ 1 {#ens-iii-s7-n5-exa-1 .statement tag=03TM}

Cho A, B là hai tập hợp, và cho $(\mathrm{V}_\alpha)_{\alpha \in \mathrm{I}}$ là một họ các tập con của A có tập chỉ số I có hướng, và sao cho quan hệ $\alpha \leqslant \beta$ kéo theo $\mathrm{V}_\beta \subset \mathrm{V}_\alpha$. Ký hiệu $\mathrm{E}_\alpha$ là tập hợp tất cả các ánh xạ từ $\mathrm{V}_\alpha$ vào B, và với mỗi cặp chỉ số $(\alpha, \beta)$ sao cho $\alpha \leqslant \beta$, ký hiệu $f_{\beta\alpha}$ là ánh xạ từ $\mathrm{E}_\alpha$ vào $\mathrm{E}_\beta$ biến mỗi hàm $u \in \mathrm{E}_\alpha$ thành *hạn chế* của nó lên $\mathrm{V}_\beta$. Hiển nhiên rằng các điều kiện $(\mathrm{LI_I})$ và $(\mathrm{LI_{II}})$ được thỏa mãn, và tập hợp $\mathrm{E} = \varinjlim \mathrm{E}_\alpha$ được gọi là tập hợp các *mầm của ánh xạ* của các $\mathrm{V}_\alpha$ vào B. \* Trường hợp thường gặp nhất là trường hợp trong đó $(\mathrm{V}_\alpha)$ là họ các *lân cận* của một tập con của một không gian tôpô A (*Tôpô đại cương*, Chương I, §6, số 10). \*

#### Ví dụ 2 {#ens-iii-s7-n5-exa-2 .statement tag=03TN}

Giả sử rằng, với mỗi $\alpha \in \mathrm{I}$, $\mathrm{E}_\alpha$ là cùng một tập hợp F và rằng bất cứ khi nào $\alpha \leqslant \beta$, $f_{\beta\alpha}$ là ánh xạ đồng nhất của F lên chính nó. Khi đó tồn tại một *song ánh chính tắc* của $\varinjlim \mathrm{E}_\alpha$ lên F. Để định nghĩa $\varinjlim \mathrm{E}_\alpha$, ta phải tạo thành tập hợp G là tổng của họ $(\mathrm{E}_\alpha)$; do đó G là hợp của một họ $(\mathrm{G}_\alpha)$ gồm các tập hợp rời nhau từng đôi một, và với mỗi $\alpha \in \mathrm{I}$ có một song ánh chính tắc $h_\alpha : \mathrm{F} \to \mathrm{G}_\alpha$. Tiếp theo ta phải xét quan hệ tương đương R trên G tương ứng với phân hoạch $(\mathrm{P}_y)_{y \in \mathrm{F}}$, trong đó $\mathrm{P}_y$ là tập hợp tất cả các $h_\alpha(y)$ khi $\alpha$ chạy qua I. Rõ ràng $y \to \mathrm{P}_y$ là một song ánh mà nghịch đảo của nó là song ánh cần tìm. Ta sẽ đồng nhất F với $\varinjlim \mathrm{E}_\alpha$ bằng song ánh chính tắc này.

#### Bổ đề 1 {#ens-iii-s7-lem-1 .statement tag=03OK}

*Cho* $(\mathrm{E}_\alpha, f_{\beta\alpha})$ *là một hệ trực tiếp các tập hợp,* $\mathrm{E} = \varinjlim \mathrm{E}_\alpha$ *là giới hạn trực tiếp của nó, và với mỗi* $\alpha \in \mathrm{I}$ *gọi* $f_\alpha \colon \mathrm{E}_\alpha \to \mathrm{E}$ *là ánh xạ chính tắc.*

(i) *Cho* $(x^{(i)})_{1 \leqslant i \leqslant n}$ *là một hệ hữu hạn các phần tử của* E. *Khi đó tồn tại* $\alpha \in I$ *và một hệ hữu hạn* $(x_\alpha^{(i)})_{1 \leqslant i \leqslant n}$ *các phần tử của* $E_\alpha$ *sao cho* $x^{(i)} = f_\alpha(x_\alpha^{(i)})$ *với* $1 \leqslant i \leqslant n$.

(ii) *Cho* $(y_\alpha^{(i)})_{1 \leqslant i \leqslant n}$ *là một hệ hữu hạn các phần tử của một* $E_\alpha$ *nào đó. Nếu* $f_\alpha(y_\alpha^{(i)}) = f_\alpha(y_\alpha^{(j)})$ *với mỗi cặp chỉ số* $(i, j)$, *thì tồn tại* $\beta \geqslant \alpha$ *sao cho* $f_{\beta\alpha}(y_\alpha^{(i)}) = f_{\beta\alpha}(y_\alpha^{(j)})$ *với mỗi cặp* $(i, j)$.

(i) Theo định nghĩa của E, với mỗi $i$ tồn tại một chỉ số $\beta_i \in I$ và một phần tử $z_{\beta_i} \in E_{\beta_i}$ sao cho $x^{(i)} = f_{\beta_i}(z_{\beta_i})$. Lấy $\alpha$ sao cho $\alpha \geqslant \beta_i$ với $1 \leqslant i \leqslant n$, và $x_\alpha^{(i)} = f_{\alpha\beta_i}(z_{\beta_i})$.

(ii) Theo định nghĩa của E, với mỗi cặp $(i, j)$ tồn tại $\gamma_{ij} \in I$ sao cho $\gamma_{ij} \geqslant \alpha$ và $f_{\gamma_{ij}\alpha}(y_\alpha^{(i)}) = f_{\gamma_{ij}\alpha}(y_\alpha^{(j)})$. Lấy $\beta$ sao cho $\beta \geqslant \gamma_{ij}$ với mọi cặp $(i, j)$, và dùng các hệ thức $f_{\beta\alpha} = f_{\beta\gamma_{ij}} \circ f_{\gamma_{ij}\alpha}$.

### 6. HỆ TRỰC TIẾP CỦA CÁC ÁNH XẠ

#### Mệnh đề 6 {#ens-iii-s7-prop-6 .statement tag=03RR}

*Cho* I *là một tập có hướng, cho* $(E_\alpha, f_{\beta\alpha})$ *là một hệ trực tiếp các tập hợp tương đối với* I, *cho* $E = \varinjlim E_\alpha$ *là giới hạn trực tiếp, và với mỗi* $\alpha \in I$ *cho*

$$f_\alpha : E_\alpha \to E$$

*là ánh xạ chính tắc. Với mỗi* $\alpha \in I$, *cho* $u_\alpha$ *là một ánh xạ từ* $E_\alpha$ *vào một tập hợp* F *sao cho*

(23) $$u_\beta \circ f_{\beta\alpha} = u_\alpha \qquad \textit{khi } \alpha \leqslant \beta.$$

*Do đó:*

(a) *Tồn tại một ánh xạ duy nhất* $u$ *từ* E *vào* F *sao cho*

(24) $$u_\alpha = u \circ f_\alpha \qquad \textit{với mọi } \alpha \in I.$$

(b) $u$ *là toàn ánh khi và chỉ khi* F *là hợp của các tập hợp* $u_\alpha(E_\alpha)$.

(c) $u$ *là đơn ánh khi và chỉ khi với mỗi* $\alpha \in I$ *các quan hệ* $x \in E_\alpha$, $y \in E_\alpha$, $u_\alpha(x) = u_\alpha(y)$ *suy ra rằng tồn tại* $\beta \geqslant \alpha$ *sao cho* $f_{\beta\alpha}(x) = f_{\beta\alpha}(y)$.

(a) Với ký hiệu của no. 5, gọi $v$ là ánh xạ từ G vào F trùng với $u_\alpha$ trên $E_\alpha$ với mỗi $\alpha \in I$ (Chương II, § 4, no. 7, Mệnh đề 8). Giả thiết kéo theo rằng $v$ tương thích với quan hệ tương đương R (Chương II, § 6, no. 5); do đó tồn tại một ánh xạ duy nhất $u$ từ $E = G/R$ vào F sao cho $v = u \circ f$ (*loc. cit.*).

(b) Vì E là hợp của các $f_\alpha(E_\alpha)$, quan hệ $F = \bigcup_{\alpha \in I} u_\alpha(E_\alpha)$ rõ ràng là điều kiện cần và đủ để $u$ là toàn ánh.

(c) Theo Bổ đề 1 của no. 5, hai phần tử bất kỳ của $\mathbf{E}$ luôn có thể được viết dưới dạng $f_\alpha(x)$ và $f_\alpha(y)$, trong đó $x \in \mathrm{E}_\alpha$ và $y \in \mathrm{E}_\alpha$, với một lựa chọn thích hợp của $\alpha \in \mathrm{I}$. Từ bổ đề cũng suy ra rằng quan hệ $f_\alpha(x) = f_\alpha(y)$ là tương đương với sự tồn tại của $\beta \geqslant \alpha$ sao cho $f_{\beta\alpha}(x) = f_{\beta\alpha}(y)$. Vì $u_\alpha(x) = u(f_\alpha(x))$ và $u_\alpha(y) = u(f_\alpha(y))$, điều này hoàn tất chứng minh.

¶ Nếu ánh xạ $u$ là *song ánh*, thì đôi khi người ta nói, do lạm dụng ngôn ngữ, rằng F là giới hạn trực tiếp của họ $(\mathrm{E}_\alpha)$.

#### Nhận xét {#ens-iii-s7-n6-rem-1 .statement tag=03OL}

Giả sử rằng mỗi ánh xạ $f_{\beta\alpha}$ đều là *đơn ánh*. Khi đó mỗi $f_\alpha$ đều là *đơn ánh*, theo định nghĩa của quan hệ R. Trong trường hợp này, nói chung ta đồng nhất $\mathrm{E}_\alpha$ và $f_\alpha(\mathrm{E}_\alpha)$, và do đó coi E là *hợp* của các $\mathrm{E}_\alpha$. Ngược lại, cho $(\mathrm{F}_\alpha)_{\alpha \in \mathrm{I}}$ là một họ tăng các tập con của một tập hợp F và giả sử rằng F là *hợp* của họ này. Nếu $j_{\beta\alpha}$ ký hiệu đơn ánh chính tắc của $\mathrm{F}_\alpha$ vào $\mathrm{F}_\beta$ với $\alpha \leqslant \beta$, thì theo Mệnh đề 6, suy ra rằng ta có thể đồng nhất F với giới hạn trực tiếp của họ $\mathrm{F}_\alpha$ đối với họ các ánh xạ $(j_{\beta\alpha})$, và ánh xạ chính tắc của $\mathrm{F}_\alpha$ vào $\varinjlim \mathrm{F}_\alpha$ với đơn ánh chính tắc của $\mathrm{F}_\alpha$ vào F, với mỗi $\alpha \in \mathrm{I}$.

#### Hệ quả 1 {#ens-iii-s7-prop-6-cor-1 .statement tag=03RS}

*Cho* $(\mathrm{E}_\alpha, f_{\beta\alpha})$ *và* $(\mathrm{F}_\alpha, g_{\beta\alpha})$ *là hai hệ trực tiếp của các tập hợp tương đối với cùng một tập hợp chỉ số* I; *đặt* $\mathrm{E} = \varinjlim \mathrm{E}_\alpha$, $\mathrm{F} = \varinjlim \mathrm{F}_\alpha$, *và với mỗi* $\alpha \in \mathrm{I}$ *cho* $f_\alpha$ (*tương ứng* $g_\alpha$) *là ánh xạ chính tắc của* $\mathrm{E}_\alpha$ (*tương ứng* $\mathrm{F}_\alpha$) *vào* E (*tương ứng* F). *Với mỗi* $\alpha \in \mathrm{I}$ *cho* $u_\alpha$ *là một ánh xạ của* $\mathrm{E}_\alpha$ *vào* $\mathrm{F}_\alpha$ *sao cho, mỗi khi* $\alpha \leqslant \beta$, *biểu đồ*

$$\begin{array}{ccc} \mathrm{E}_\alpha & \overset{u_\alpha}{\longrightarrow} & \mathrm{F}_\alpha \\ {\scriptstyle f_{\beta\alpha}}\big\downarrow & & \big\downarrow{\scriptstyle g_{\beta\alpha}} \\ \mathrm{E}_\beta & \underset{u_\beta}{\longrightarrow} & \mathrm{F}_\beta \end{array}$$

*là giao hoán. Khi đó tồn tại một ánh xạ duy nhất* $u : \mathrm{E} \rightarrow \mathrm{F}$ *sao cho, với mỗi* $\alpha \in \mathrm{I}$, *biểu đồ*

$$\begin{array}{ccc} \mathrm{E}_\alpha & \overset{u_\alpha}{\longrightarrow} & \mathrm{F}_\alpha \\ {\scriptstyle f_\alpha}\big\downarrow & & \big\downarrow{\scriptstyle g_\alpha} \\ \mathrm{E} & \underset{u}{\longrightarrow} & \mathrm{F} \end{array}$$

*là giao hoán.*

Đặt $v_\alpha = g_\alpha \circ u_\alpha$. Nếu $\alpha \leqslant \beta$, thì theo (22) ta có

$$v_\beta \circ f_{\beta\alpha} = g_\beta \circ u_\beta \circ f_{\beta\alpha} = g_\beta \circ g_{\beta\alpha} \circ u_\alpha = g_\alpha \circ u_\alpha = v_\alpha.$$

Do đó ta có thể áp dụng Mệnh đề 6 cho các ánh xạ $v_\alpha$, do đó suy ra sự tồn tại và tính duy nhất của một ánh xạ $u : \mathrm{E} \to \mathrm{F}$ sao cho

$$u \circ f_\alpha = v_\alpha = g_\alpha \circ u_\alpha$$

với mọi $\alpha \in \mathrm{I}$.

¶ Một họ các ánh xạ $u_\alpha : \mathrm{E}_\alpha \to \mathrm{F}_\alpha$ thỏa mãn các điều kiện của Hệ quả 1 được gọi là một *hệ trực tiếp các ánh xạ* của $(\mathrm{E}_\alpha, f_{\beta\alpha})$ vào $(\mathrm{F}_\alpha, g_{\beta\alpha})$. Ánh xạ được xác định trong Hệ quả 1 được gọi là *giới hạn trực tiếp* của họ $(u_\alpha)$ và được viết là $u = \varinjlim u_\alpha$ khi không có nguy cơ nhập nhằng.

#### Hệ quả 2 {#ens-iii-s7-prop-6-cor-2 .statement tag=03RT}

*Cho* $(\mathrm{E}_\alpha, f_{\beta\alpha})$, $(\mathrm{F}_\alpha, g_{\beta\alpha})$, $(\mathrm{G}_\alpha, h_{\beta\alpha})$ *là ba hệ trực tiếp các tập hợp tương đối với* I. *Cho* $\mathrm{E} = \varinjlim \mathrm{E}_\alpha$, $\mathrm{F} = \varinjlim \mathrm{F}_\alpha$, $\mathrm{G} = \varinjlim \mathrm{G}_\alpha$, *và cho* $f_\alpha$ *(tương ứng* $g_\alpha$, $h_\alpha$*) là ánh xạ chính tắc của* $\mathrm{E}_\alpha$ *(tương ứng của* $\mathrm{F}_\alpha$, $\mathrm{G}_\alpha$*) vào* E *(tương ứng vào* F, G*). Nếu* $(u_\alpha)$ *và* $(v_\alpha)$ *là hai hệ trực tiếp các ánh xạ* $u_\alpha : \mathrm{E}_\alpha \to \mathrm{F}_\alpha$, $v_\alpha : \mathrm{F}_\alpha \to \mathrm{G}_\alpha$, *thì các ánh xạ* $v_\alpha \circ u_\alpha : \mathrm{E}_\alpha \to \mathrm{G}_\alpha$ *tạo thành một hệ trực tiếp các ánh xạ, và ta có*

(25) $$\varinjlim (v_\alpha \circ u_\alpha) = (\varinjlim v_\alpha) \circ (\varinjlim u_\alpha).$$

Thật vậy, nếu ta đặt $w_\alpha = v_\alpha \circ u_\alpha$, thì với $\alpha \leqslant \beta$ ta có

$$h_{\beta\alpha} \circ w_\alpha = (h_{\beta\alpha} \circ v_\alpha) \circ u_\alpha = (v_\beta \circ g_{\beta\alpha}) \circ u_\alpha = v_\beta \circ (u_\beta \circ f_{\beta\alpha}) = w_\beta \circ f_{\beta\alpha},$$

điều đó cho thấy $(w_\alpha)$ là một hệ trực tiếp các ánh xạ. Hơn nữa, nếu $u = \varinjlim u_\alpha$ và $v = \varinjlim v_\alpha$, thì với mọi $\alpha \in \mathrm{I}$ ta có

$$(v \circ u) \circ f_\alpha = v \circ (g_\alpha \circ u_\alpha) = h_\alpha \circ (v_\alpha \circ u_\alpha),$$

và do tính duy nhất của giới hạn trực tiếp, ta có $v \circ u = \varinjlim w_\alpha$.

#### Mệnh đề 7 {#ens-iii-s7-prop-7 .statement tag=03RU}

*Cho* $(\mathrm{E}_\alpha, f_{\beta\alpha})$ *và* $(\mathrm{E}'_\alpha, f'_{\beta\alpha})$ *là hai hệ trực tiếp các tập hợp tương đối với* I, *và với mỗi* $\alpha \in \mathrm{I}$ *cho* $u_\alpha$ *là một ánh xạ từ* $\mathrm{E}_\alpha$ *vào* $\mathrm{E}'_\alpha$ *sao cho các* $u_\alpha$ *lập thành một hệ trực tiếp các ánh xạ. Đặt* $u = \varinjlim u_\alpha$. *Nếu mỗi* $u_\alpha$ *là đơn ánh* (tương ứng, *toàn ánh*) *thì* $u$ *là đơn ánh* (tương ứng, *toàn ánh*).

Cho $\mathrm{E} = \varinjlim \mathrm{E}_\alpha$, $\mathrm{E}' = \varinjlim \mathrm{E}'_\alpha$, và gọi $f_\alpha : \mathrm{E}_\alpha \to \mathrm{E}$, $f'_\alpha : \mathrm{E}'_\alpha \to \mathrm{E}'$ là các ánh xạ chính tắc. Giả sử rằng mỗi $u_\alpha$ đều đơn ánh. Để chứng minh rằng $u$ là đơn ánh, theo Mệnh đề 6, chỉ cần kiểm tra rằng nếu $x \in \mathrm{E}_\alpha$ và $y \in \mathrm{E}_\alpha$ sao cho $f'_\alpha(u_\alpha(x)) = f'_\alpha(u_\alpha(y))$, thì tồn tại $\beta \geqslant \alpha$ sao cho $f_{\beta\alpha}(x) = f_{\beta\alpha}(y)$. Bây giờ giả thiết suy ra (no. 6, Bổ đề 1) rằng tồn tại $\beta \geqslant \alpha$ sao cho

$$f'_{\beta\alpha}(u_\alpha(x)) = f'_{\beta\alpha}(u_\alpha(y)), \qquad \text{i.e.,} \qquad u_\beta(f_{\beta\alpha}(x)) = u_\beta(f_{\beta\alpha}(y)),$$

và do đó $f_{\beta\alpha}(x) = f_{\beta\alpha}(y)$ vì $u_\beta$ là đơn ánh.

Bây giờ giả sử rằng các $u_\alpha$ là toàn ánh. Khi đó ta có

$$\mathrm{E}' = \bigcup_\alpha f'_\alpha(\mathrm{E}'_\alpha) = \bigcup_\alpha f'_\alpha(u_\alpha(\mathrm{E}_\alpha)) = \bigcup_\alpha u(f_\alpha(\mathrm{E}_\alpha)) = u\Big(\bigcup_\alpha f_\alpha(\mathrm{E}_\alpha)\Big) = u(\mathrm{E}).$$

Với ký hiệu của Mệnh đề 7, cho $\mathrm{M}_\alpha$ là một tập con của $\mathrm{E}_\alpha$ với mỗi $\alpha \in \mathrm{I}$; nếu ta có $f_{\beta\alpha}(\mathrm{M}_\alpha) \in \mathrm{M}_\beta$ mỗi khi $\alpha \leqslant \beta$, thì họ $(\mathrm{M}_\alpha)_{\alpha \in \mathrm{I}}$ được gọi là một *hệ trực tiếp các tập con của* $\mathrm{E}_\alpha$. Cho $g_{\beta\alpha}$ (với $\alpha \leqslant \beta$) là ánh xạ của $\mathrm{M}_\alpha$ vào $\mathrm{M}_\beta$ mà đồ thị của nó là cùng một đồ thị như đồ thị của hạn chế của $f_{\beta\alpha}$ trên $\mathrm{M}_\alpha$. Khi đó hiển nhiên $(\mathrm{M}_\alpha, g_{\beta\alpha})$ là một hệ trực tiếp các tập hợp; và Mệnh đề 7, áp dụng cho các đơn ánh chính tắc $j_\alpha : \mathrm{M}_\alpha \to \mathrm{E}_\alpha$, cho phép ta *đồng nhất* $\mathrm{M} = \varinjlim \mathrm{M}_\alpha$ với một tập con của E nhờ đơn ánh $j = \varinjlim j_\alpha$.

#### Hệ quả {#ens-iii-s7-n6-cor-1 .statement tag=03ON}

*Cho* $(\mathrm{E}_\alpha, f_{\beta\alpha})$ *và* $(\mathrm{E}'_\alpha, f'_{\beta\alpha})$ *là hai hệ trực tiếp các tập hợp, cho* $(u_\alpha)$ *là một hệ trực tiếp các ánh xạ* $u_\alpha : \mathrm{E}_\alpha \to \mathrm{E}'_\alpha$, *và đặt* $u = \varinjlim u_\alpha$.

(i) *Cho* $(\mathrm{M}_\alpha)$ *là một hệ trực tiếp các tập con của các* $\mathrm{E}_\alpha$. *Khi đó* $(u_\alpha(\mathrm{M}_\alpha))$ *là một hệ trực tiếp các tập con của các* $\mathrm{E}'_\alpha$, *và ta có*

(26) $$\varinjlim u_\alpha(\mathrm{M}_\alpha) = u\,(\varinjlim \mathrm{M}_\alpha).$$

(ii) *Cho* $(a'_\alpha)_{\alpha \in \mathbf{I}}$ *là một họ sao cho* $a'_\alpha \in \mathrm{E}'_\alpha$ *với mỗi* $\alpha \in \mathrm{I}$ *và* $f'_{\beta\alpha}(a'_\alpha) = a'_\beta$ *mỗi khi* $\alpha \leqslant \beta$. *Khi đó các tập hợp* $\overset{-1}{u}_\alpha(a'_\alpha)$ *tạo thành một hệ trực tiếp các tập con của các* $\mathrm{E}_\alpha$, *và ta có*

(27) $$\varinjlim \overset{-1}{u}_\alpha(a'_\alpha) = \overset{-1}{u}(a'),$$

*trong đó* $a'$ *là phần tử duy nhất của* $\varinjlim \mathrm{E}'_\alpha$ *là ảnh chính tắc của* $a'_\alpha$ *với mỗi* $\alpha \in \mathrm{I}$.

(i) Hiển nhiên rằng các $u_\alpha(\mathrm{M}_\alpha)$ tạo thành một hệ trực tiếp các tập con của các $\mathrm{E}'_\alpha$, và ta có thể viết $u_\alpha(\mathrm{M}_\alpha) = v_\alpha(\mathrm{M}_\alpha)$, trong đó $v_\alpha$ là ánh xạ của $\mathrm{M}_\alpha$ lên $u_\alpha(\mathrm{M}_\alpha)$ có đồ thị trùng với đồ thị của hạn chế của $u_\alpha$ vào $\mathrm{M}_\alpha$. Khi đó công thức (26) suy ra từ Mệnh đề 7 vì các $v_\alpha$ là toàn ánh.

(ii) Đặt $\mathrm{N}_\alpha = \overset{-1}{u}_\alpha(a'_\alpha)$. Nếu $\alpha \leqslant \beta$ và $x_\alpha \in \mathrm{N}_\alpha$, thì

$$u_\beta(f_{\beta\alpha}(x_\alpha)) = f'_{\beta\alpha}(u_\alpha(x_\alpha) = f'_{\beta\alpha}(a'_\alpha) = a'_\beta;$$

do đó $f_{\beta\alpha}(x_\alpha) \in \mathrm{N}_\beta$, và vì thế các $\mathrm{N}_\alpha$ tạo thành một hệ trực tiếp các tập con của các $\mathrm{E}_\alpha$. Với ký hiệu của chứng minh Mệnh đề 7, xét một phần tử $x \in \varinjlim \mathrm{N}_\alpha$. Tồn tại $\alpha \in \mathrm{I}$ và $x_\alpha \in \mathrm{N}_\alpha$ sao cho $x = f_\alpha(x_\alpha)$, do đó $u(x) = u(f_\alpha(x_\alpha)) = f'_\alpha(u_\alpha(x_\alpha)) = f'_\alpha(a'_\alpha) = a'$. Ngược lại, nếu

$x \in \overset{-1}{u}(a')$ và nếu $x = f_\alpha(x_\alpha)$ với một $\alpha \in \mathrm{I}$ nào đó và một $x_\alpha \in \mathrm{E}_\alpha$ nào đó, thì ta có $a' = u(f_\alpha(x_\alpha)) = f'_\alpha(u_\alpha(x_\alpha)) = f'_\alpha(a'_\alpha)$. Do đó (số 5, Bổ đề 1) tồn tại $\beta \geqslant \alpha$ sao cho $f'_{\beta\alpha}(u'_\alpha(x_\alpha)) = f'_{\beta\alpha}(a'_\alpha) = a'_\beta$; tức là, $u_\alpha(f_{\beta\alpha}(x_\alpha)) = a'_\beta$, và vì thế $f_{\beta\alpha}(x_\alpha) \in \mathrm{N}_\beta$. Vì $x = f_\beta(f_{\beta\alpha}(x_\alpha))$, suy ra $x \in \varinjlim \mathrm{N}_\alpha$.

#### Chú ý {#ens-iii-s7-n6-rem-2 .statement tag=03OO}

Giả sử rằng, với mỗi $\alpha \in \mathrm{I}$, $u_\alpha : \mathrm{E}_\alpha \to \mathrm{E}'$ là một ánh xạ sao cho họ $(u_\alpha)$ thỏa mãn (23). Xét hệ trực tiếp $(\mathrm{E}_\alpha, i_{\beta\alpha})$ tương đối với I, trong đó $\mathrm{E}'_\alpha = \mathrm{E}'$ với mọi $\alpha \in \mathrm{I}$, và $i_{\beta\alpha}$ là ánh xạ đồng nhất của $\mathrm{E}'$. Khi đó (no. 5, Ví dụ 2) $\mathrm{E}'$ có thể được đồng nhất một cách chính tắc với $\varinjlim \mathrm{E}'_\alpha$. Nếu $u_\alpha$ được xét như một ánh xạ từ $\mathrm{E}_\alpha$ vào $\mathrm{E}'_\alpha$, thì $(u_\alpha)$ là một hệ trực tiếp các ánh xạ, và ánh xạ $u : \mathrm{E} \to \mathrm{E}'$ được định nghĩa bởi (24) được đồng nhất với giới hạn trực tiếp của hệ các ánh xạ này. Do đó, do lạm dụng ngôn ngữ, ta viết $u = \varinjlim u_\alpha$.

Nếu J là một tập con của I có hướng (đối với tiền thứ tự cảm sinh), thì rõ ràng cặp gồm họ con $(\mathrm{E}_\alpha)_{\alpha \in \mathrm{J}}$ và họ $(f_{\beta\alpha})$, trong đó $\alpha \leqslant \beta$ và $\alpha \in \mathrm{J}$ và $\beta \in \mathrm{J}$, là một hệ trực tiếp các tập hợp đối với J; người ta nói rằng nó thu được bằng cách *hạn chế* tập hợp chỉ số vào J. Gọi E, E′ tương ứng là các giới hạn trực tiếp của các họ $(\mathrm{E}_\alpha)_{\alpha \in \mathrm{I}}$ và $(\mathrm{E}_\alpha)_{\alpha \in \mathrm{J}}$, và với mỗi $\alpha \in \mathrm{I}$, gọi $f_\alpha : \mathrm{E}_\alpha \to \mathrm{E}$ là ánh xạ chính tắc. Khi đó $(f_\alpha)_{\alpha \in \mathrm{J}}$ là một hệ trực tiếp các ánh xạ, và do đó $g = \varinjlim f_\alpha$ là một ánh xạ từ E′ vào E, được gọi là *chính tắc*. Hơn nữa, nếu J′ là một tập con có hướng của J, nếu E″ là giới hạn trực tiếp của họ $(\mathrm{E}_\alpha)_{\alpha \in \mathrm{J}'}$, và nếu

$$g' : \quad \mathrm{E}'' \to \mathrm{E}' \qquad \text{và} \qquad g'' : \mathrm{E}'' \to \mathrm{E}$$

là các ánh xạ chính tắc, thì suy ra ngay lập tức từ Mệnh đề 6 rằng

(28) $$g'' = g \circ g'.$$

#### Mệnh đề 8 {#ens-iii-s7-prop-8 .statement tag=03OP}

*Cho* I *là một tập hợp có hướng, cho* $(\mathrm{E}_\alpha, f_{\beta\alpha})$ *là một hệ trực tiếp các tập hợp tương đối với* I, *và đặt* $\mathrm{E} = \varinjlim \mathrm{E}_\alpha$ *là giới hạn trực tiếp của nó. Cho* J *là một tập con đồng cuối của* I *và đặt* E′ *là giới hạn trực tiếp của hệ trực tiếp các tập hợp thu được từ* $(\mathrm{E}_\alpha, f_{\beta\alpha})$ *bằng cách hạn chế tập chỉ số vào* J. *Khi đó ánh xạ chính tắc* $g$ *từ* E′ *vào* E *là song ánh.*

J tất yếu là một tập hợp có hướng (§ 1, no. 10). Chúng tôi sẽ dùng các tiêu chuẩn của Mệnh đề 6 để chỉ ra rằng $g$ là song ánh. Điều kiện để có tính đơn ánh suy ra ngay lập tức từ các định nghĩa và từ Bổ đề 1 của no. 5. Để chỉ ra rằng $g$ là toàn ánh, ta chú ý rằng với mỗi $\alpha \in \mathrm{J}$ ta có

$$g(\mathrm{E}_\alpha) = f_\alpha(\mathrm{E}_\alpha).$$

Bây giờ, với mỗi $\beta \in I$, tồn tại $\gamma \in J$ sao cho $\beta \leqslant \gamma$, từ đó suy ra rằng $g(E_\gamma) \supset g(f_{\gamma\beta}(E_\beta)) = f_\beta(E_\beta)$. Vậy E là hợp của các tập hợp $g(E_\alpha)$ khi $\alpha$ chạy qua J.

### 7. GIỚI HẠN TRỰC TIẾP KÉP. TÍCH CỦA CÁC GIỚI HẠN TRỰC TIẾP

Cho I, L là hai tập có hướng, và $I \times L$ là tích của chúng (§ 1, no. 4), với quan hệ tiền thứ tự tích, lại là một tập có hướng. Xét một hệ trực tiếp của các tập $(E^\lambda_\alpha, f^{\mu\lambda}_{\beta\alpha})$ tương đối với $I \times L$. Khi đó ta có

$$(29) \qquad f^{\nu\lambda}_{\gamma\alpha} = f^{\mu\nu}_{\gamma\beta} \circ f^{\mu\lambda}_{\beta\alpha}$$

mỗi khi $\alpha \leqslant \beta \leqslant \gamma$ và $\lambda \leqslant \mu \leqslant \nu$.

Ký hiệu E hoặc $\varinjlim_{\alpha,\lambda} E^\lambda_\alpha$ là giới hạn trực tiếp của hệ trực tiếp này. Với mỗi $\lambda \in L$, đặt $g^\lambda_{\beta\alpha} = f^{\lambda\lambda}_{\beta\alpha} : E^\lambda_\alpha \to E^\lambda_\beta$. Khi đó từ (29) ta có

$$(30) \qquad g^\lambda_{\gamma\alpha} = g^\lambda_{\gamma\beta} \circ g^\lambda_{\beta\alpha} \qquad \text{khi } \alpha \leqslant \beta \leqslant \gamma;$$

nói cách khác, $(E^\lambda_\alpha, g^\lambda_{\beta\alpha})$ là một hệ trực tiếp các tập hợp tương đối với I. Ký hiệu $F^\lambda = \varinjlim_\alpha E^\lambda_\alpha$ là giới hạn trực tiếp của nó. Nếu $\lambda \leqslant \mu$ là những phần tử cố định của L, thì từ (29) suy ra rằng các ánh xạ $h^{\mu\lambda}_\alpha = f^{\lambda\mu}_{\alpha\alpha} : E^\lambda_\alpha \to E^\mu_\alpha$ tạo thành một hệ trực tiếp các ánh xạ. Ký hiệu $h^{\mu\lambda} = \varinjlim_\alpha h^{\mu\lambda}_\alpha : F^\lambda \to F^\mu$ là giới hạn trực tiếp của hệ ánh xạ này. Nếu $\lambda \leqslant \mu \leqslant \nu$ trong L, thì

$$(31) \qquad h^{\nu\lambda} = h^{\nu\mu} \circ h^{\mu\lambda}$$

(no. 6, Mệnh đề 6, Hệ quả 2), và do đó $(F^\lambda, h^{\mu\lambda})$ là một hệ trực tiếp các tập hợp tương đối với L. Gọi $F = \varinjlim F^\lambda$ là giới hạn trực tiếp của nó. Ta sẽ định nghĩa một *song ánh chính tắc* $E \to F$. Vì mục đích đó, gọi $g^\lambda_\alpha$ là ánh xạ chính tắc $E^\lambda_\alpha \to F^\lambda$, và $h^\lambda$ là ánh xạ chính tắc $F^\lambda \to F$, và đặt $u^\lambda_\alpha = h^\lambda \circ g^\lambda_\alpha$. Nếu $\alpha \leqslant \beta$ và $\lambda \leqslant \mu$, thì ta có

$$\begin{aligned} u^\mu_\beta \circ f^{\mu\lambda}_{\beta\alpha} &= h^\mu \circ g^\mu_\beta \circ f^{\mu\lambda}_{\beta\alpha} = h^\mu \circ g^\mu_\beta \circ f^{\mu\mu}_{\beta\alpha} \circ f^{\mu\lambda}_{\alpha\alpha} = h^\mu \circ g^\mu_\alpha \circ f^{\mu\lambda}_{\alpha\alpha} \\ &= h^\mu \circ h^{\mu\lambda} \circ g^\lambda_\alpha = h^\lambda \circ g^\lambda_\alpha = u^\lambda_\alpha \end{aligned}$$

từ (29) và định nghĩa của các $h^{\mu\lambda}$. Do đó các $u^\lambda_\alpha$ tạo thành một hệ trực tiếp các ánh xạ tương đối đối với $I \times L$. Đặt $u = \varinjlim_{\alpha,\lambda} u^\lambda_\alpha : E \to F$. Ta sẽ chứng minh rằng $u$ là song ánh bằng cách áp dụng các tiêu chuẩn của no. 6, Mệnh đề 6. Trước hết, F là hợp của các tập hợp $h^\lambda(F^\lambda)$, và mỗi $F^\lambda$ là

hợp của các tập hợp $g_\alpha^\lambda(\mathrm{E}_\alpha^\lambda)$; do đó F là hợp của các tập hợp

$$h^\lambda(g_\alpha^\lambda(\mathrm{E}_\alpha^\lambda)) = u_\alpha^\lambda(\mathrm{E}_\alpha^\lambda).$$

Tiếp theo, cho $x$, $y$ là hai phần tử của $\mathrm{E}_\alpha^\lambda$ sao cho $u_\alpha^\lambda(x) = u_\alpha^\lambda(y)$, tức là $h^\lambda(g_\alpha^\lambda(x)) = h^\lambda(g_\alpha^\lambda(y))$. Khi đó (no. 5, Bổ đề 1) tồn tại $\mu \geqslant \lambda$ sao cho $h^{\mu\lambda}(g_\alpha^\lambda(x)) = h^{\mu\lambda}(g_\alpha^\lambda(y))$, tức là $g_\alpha^\mu(f_{\alpha\alpha}^{\mu\lambda}(x)) = g_\alpha^\mu(f_{\alpha\alpha}^{\mu\lambda}(y))$; tương tự tồn tại $\beta \geqslant \alpha$ sao cho $g_{\beta\alpha}^\mu(f_{\alpha\alpha}^{\mu\lambda}(x)) = g_{\beta\alpha}^\mu(f_{\alpha\alpha}^{\mu\lambda}(y))$ (no. 5, Bổ đề 1), tức là $f_{\beta\alpha}^{\mu\lambda}(x) = f_{\beta\alpha}^{\mu\lambda}(y)$; và điều này chứng tỏ (no. 6, Mệnh đề 6) rằng $u$ là đơn ánh. Vậy ta đã chứng minh được :

#### Mệnh đề 9 {#ens-iii-s7-prop-9 .statement tag=03RV}

*Nếu* $(\mathrm{E}_\alpha^\lambda, f_{\beta\alpha}^{\mu\lambda})$ *là một hệ trực tiếp các tập hợp tương đối với một tích* $\mathrm{I} \times \mathrm{L}$ *của hai tập hợp có hướng, thì (theo một song ánh chính tắc) ta có*

(32)
$$\varinjlim_{\alpha,\ \lambda} \mathrm{E}_\alpha^\lambda = \varinjlim_{\lambda}\ (\varinjlim_{\alpha} \mathrm{E}_\alpha^\lambda).$$

#### Hệ quả {#ens-iii-s7-n7-cor-1 .statement tag=03OQ}

*Cho* $(\mathrm{E}'^\lambda_\alpha, f'^{\mu\lambda}_{\beta\alpha})$ *là một hệ trực tiếp khác của các tập hợp tương đối với* $\mathrm{I} \times \mathrm{L}$, *và với mỗi* $(\alpha, \lambda) \in \mathrm{I} \times \mathrm{L}$ *cho* $u_\alpha^\lambda$ *là một ánh xạ từ* $\mathrm{E}_\alpha^\lambda$ *vào* $\mathrm{E}'^\lambda_\alpha$, *sao cho các* $u_\alpha^\lambda$ *tạo thành một hệ trực tiếp các ánh xạ. Khi đó ta có*

(33)
$$\varinjlim_{\alpha,\ \lambda} u_\alpha^\lambda = \varinjlim_{\lambda}\ (\varinjlim_{\alpha} u_\alpha^\lambda).$$

Ta để việc kiểm chứng lại cho người đọc.

#### Mệnh đề 10 {#ens-iii-s7-prop-10 .statement tag=03RW}

*Cho* $(\mathrm{E}_\alpha, f_{\beta\alpha})$ *và* $(\mathrm{E}'_\alpha, f'_{\beta\alpha})$ *là hai hệ trực tiếp của các tập hợp, cùng tương đối với một tập có hướng* I. *Đặt* $\mathrm{E} = \varinjlim \mathrm{E}_\alpha$, $\mathrm{E}' = \varinjlim \mathrm{E}'_\alpha$, *và gọi* $f_\alpha : \mathrm{E}_\alpha \to \mathrm{E}, f'_\alpha : \mathrm{E}'_\alpha \to \mathrm{E}'$ *là các ánh xạ chính tắc, với mỗi* $\alpha \in \mathrm{I}$. *Khi đó* $(\mathrm{E}_\alpha \times \mathrm{E}'_\alpha, f_{\beta\alpha} \times f'_{\beta\alpha})$ *là một hệ trực tiếp các tập hợp,* $(f_\alpha \times f'_\alpha)$ *là một hệ trực tiếp các ánh xạ, và* $\varinjlim (f_\alpha \times f'_\alpha)$ *là một song ánh*

(34)
$$\varinjlim (\mathrm{E}_\alpha \times \mathrm{E}'_\alpha) \to (\varinjlim \mathrm{E}_\alpha) \times (\varinjlim \mathrm{E}'_\alpha).$$

Hai khẳng định đầu tiên của Mệnh đề được kiểm tra ngay lập tức. Để chứng tỏ rằng $g = \varinjlim (f_\alpha \times f'_\alpha)$ là song ánh, ta áp dụng Mệnh đề 6 của no. 6. Rõ ràng $\mathrm{E} \times \mathrm{E}'$ là hợp của các tập hợp $f_\alpha(\mathrm{E}_\alpha) \times f'_\alpha(\mathrm{E}'_\alpha)$; do đó $g$ là toàn ánh. Nếu $(x, x')$ và $(y, y')$ là hai phần tử của $\mathrm{E}_\alpha \times \mathrm{E}'_\alpha$ sao cho $f_\alpha(x) = f_\alpha(y)$ và $f'_\alpha(x') = f'_\alpha(y')$, thì (no. 5, Bổ đề 1) tồn tại hai phần tử $\beta$, $\gamma$ của I sao cho $\beta \geqslant \alpha$, $\gamma \geqslant \alpha$, và $f_{\beta\alpha}(x) = f_{\beta\alpha}(y)$, $f'_{\gamma\alpha}(x') = f'_{\gamma\alpha}(y')$; vì I có hướng, tồn tại $\delta \in \mathrm{I}$ sao cho $\delta \geqslant \beta$ và $\delta \geqslant \gamma$; do đó $f_{\delta\alpha}(x) = f_{\delta\alpha}(y)$ và $f'_{\delta\alpha}(x') = f'_{\delta\alpha}(y')$. Điều này hoàn tất chứng minh.

Song ánh $g$ được gọi là *chính tắc*.

#### Hệ quả {#ens-iii-s7-n7-cor-2 .statement tag=03RX}

*Cho* $(\mathrm{F}_\alpha, g_{\beta\alpha})$ *và* $(\mathrm{F}'_\alpha, g'_{\beta\alpha})$ *là hai hệ trực tiếp các tập hợp tương đối với* I, *và với mỗi* $\alpha \in \mathrm{I}$ *cho* $u_\alpha : \mathrm{E}_\alpha \to \mathrm{F}_\alpha$, $u'_\alpha : \mathrm{E}'_\alpha \to \mathrm{F}'_\alpha$ *là các ánh xạ sao cho* $(u_\alpha)$ *và* $(u'_\alpha)$ *là hai hệ trực tiếp các ánh xạ. Khi đó* $(u_\alpha \times u'_\alpha)$ *là một hệ trực tiếp các ánh xạ, và (theo các song ánh chính tắc) ta có*

(35) $$\varinjlim (u_\alpha \times u'_\alpha) = (\varinjlim u_\alpha) \times (\varinjlim u'_\alpha).$$

Chúng tôi để việc kiểm tra lại cho bạn đọc.

### Bài tập {#ens-iii-s7-exercises}

Xem [các bài tập của § 7](exercises/s7/).

[^1]: (\*) Điều này có nghĩa là $u_\alpha \circ f_{\alpha\beta} = g_{\alpha\beta} \circ u_\beta$.
