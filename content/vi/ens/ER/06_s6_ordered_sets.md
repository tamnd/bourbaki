---
book: ens
book_title: Theory of Sets
chapter: ER
chapter_title: SUMMARY OF RESULTS
section: 6
section_title: Ordered sets
lang: vi
source: ens-i-iv
source_edition: 2004, Springer
book_pages: 373-380
pdf_pages: 0378-0385
extraction: ocr
statements: 0
exercises: 0
content_sha256: 5da442dfa2c082981e1a0f1e9d4211e6ba9e3ff8fac180b1d9986493fd1881aa
translated_from: content/en/ens/ER/06_s6_ordered_sets.md
source_content_sha256: 011cbefdb53dd46f43be31ed92b067ac148b886f8dc3965f2c33578b74501401
translation_model: gpt-5-6
translation_run: translate-vi-999992d8
glossary_version: 34
glossary_terms_sha256: ddaa24bbb3cbb6daadf435f2aeb70145ead5dfa4f449d6106905dfd8cfde4c01
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 6. CÁC TẬP HỢP CÓ THỨ TỰ

1. Một quan hệ $\omega\{x,y\}$ giữa hai phần tử tổng quát x, y của một tập hợp E được gọi là một quan hệ thứ tự trên E, nếu nó thỏa mãn hai điều kiện sau:
(a) Quan hệ “$\omega\{x,y\}$ và $\omega\{y,z\}$” kéo theo “$\omega\{x,z\}$” (tính bắc cầu).
(b) Quan hệ “$\omega\{x,y\}$ và $\omega\{y,x\}$” tương đương với “$x=y$”.
Điều kiện (b) kéo theo rằng $\omega$ là phản xạ.

Gọi C là tập con của $E\times E$ được xác định bởi quan hệ $\omega\{x,y\}$ như là một tính chất của cặp $(x,y)$. Khi đó các điều kiện (a) và (b) lần lượt tương đương với các điều kiện sau: (a′) $C \circ C \subset C$; (b′) $C \cap \overline{C}^{-1} = \Delta$. Các điều kiện này kéo theo rằng $C \circ C = C$.

Khi xét một quan hệ thứ tự cụ thể trên một tập hợp $E$, ta nói rằng $E$ có thứ tự bởi quan hệ này, và rằng quan hệ đó định nghĩa một cấu trúc thứ tự (xem §8) (hoặc một cách sắp thứ tự) trên $E$.

Nếu $\omega\{x,y\}$ là một quan hệ thứ tự trên $E$, thì $\omega^{-1}\{x,y\}$ cũng vậy. Hai quan hệ thứ tự này, và các thứ tự mà chúng định nghĩa, được gọi là đối nhau.

Cho $\omega\{x,y\}$ là một quan hệ thứ tự trên $E$, và cho $A$ là một tập con bất kỳ của $E$. Khi đó quan hệ $\omega\{x,y\}$ giữa hai phần tử tổng quát $x,y$ của $A$ là một quan hệ thứ tự trên $A$, và thứ tự mà nó định nghĩa trên $A$ được gọi là cảm sinh bởi thứ tự được định nghĩa bởi $\omega\{x,y\}$ trên $E$. Thứ tự đã cho trên $E$ được gọi là một mở rộng của thứ tự cảm sinh trên $A$.

Một quan hệ phản xạ và bắc cầu $\overline{\omega}\{x,y\}$ giữa hai phần tử tổng quát $x,y$ của $E$ được gọi là một quan hệ tiền thứ tự trên $E$. Quan hệ “$\overline{\omega}\{x,y\}$ và $\overline{\omega}\{y,x\}$” là một quan hệ tương đương $R$ trên $E$, và $\overline{\omega}\{x,y\}$ là tương thích (theo $x$ và $y$) với quan hệ này. Chuyển qua thương (đối với $x$ và $y$), $\overline{\omega}\{x,y\}$ cảm sinh trên tập hợp $E/R$ một quan hệ thứ tự, được gọi là liên kết với $\overline{\omega}\{x,y\}$. Một tập hợp được trang bị một quan hệ tiền thứ tự được gọi là một tập hợp tiền thứ tự.

2. Quan hệ bao hàm “$Y \subset X$” là một quan hệ thứ tự trên tập hợp các tập con $\mathfrak{P}(E)$ của một tập hợp bất kỳ $E$.

Nếu $E$ và $F$ là hai tập hợp, có thể phân biệt hoặc không, thì quan hệ “$g$ mở rộng $f$” là một quan hệ thứ tự trên tập hợp tất cả các ánh xạ của các tập con của $E$ vào $F$.

Tập hợp $\mathbf{N}$ các số nguyên tự nhiên [^1] được sắp thứ tự bởi quan hệ “$x \leq y$”.

3. Theo ví dụ cuối cùng này, khi một tập hợp $E$ có thứ tự bởi một quan hệ $\omega\{x,y\}$, thường thuận tiện khi ký hiệu quan hệ $\omega\{x,y\}$ bởi $x \leq y$, hoặc $y \geq x$; các quan hệ này được đọc là “$x$ nhỏ hơn $y$”, hoặc “$y$ lớn hơn $x$” [^2]. Các quan hệ “$x<y$” và “$y>x$” (đọc là “$x$ nhỏ hơn nghiêm ngặt $y$”, hoặc “$y$ lớn hơn nghiêm ngặt $x$”) theo định nghĩa tương đương với “$x\leq y$ và $x\neq y$”.

Quan hệ “$x\leq y$” tương đương với “$x<y$ hoặc $x=y$”. Quan hệ “$x\leq y$ và $y<z$” kéo theo “$x<z$”; tương tự, “$x<y$ và $y\leq z$” kéo theo “$x<z$”.

4. Một tập con X của một tập hợp E, có thứ tự bởi một quan hệ “$\leq$”, được gọi là *được sắp thứ tự toàn phần* bởi quan hệ này nếu, với mọi $x\in X$ và mọi $y\in X$, ta có hoặc $x\leq y$ hoặc $y\leq x$ (hay, tương đương, hoặc $x<y$ hoặc $x=y$ hoặc $x>y$, ba quan hệ này loại trừ lẫn nhau).
Tập con rỗng của một tập hợp có thứ tự luôn được sắp thứ tự toàn phần. Có thể xảy ra rằng toàn bộ tập hợp E được sắp thứ tự toàn phần, như trường hợp tập hợp $\mathbf{N}$ và quan hệ $x\leq y$.
Mọi tập con của một tập sắp thứ tự toàn phần đều được sắp thứ tự toàn phần bởi thứ tự cảm sinh.
Trong một tập hợp E có thứ tự, nếu $a$ và $b$ là hai phần tử sao cho $a\leq b$, tập con của E gồm các phần tử $x$ sao cho $a\leq x\leq b$ được gọi là *khoảng đóng với đầu mút trái a và đầu mút phải b*, và được ký hiệu bởi $[a,b]$. Tập hợp tất cả các $x\in E$ sao cho $a\leq x<b$ (resp. $a<x\leq b$) được gọi là *khoảng nửa đóng về phía phải* (resp. *về phía trái*) với các đầu mút $a$ và $b$, và được ký hiệu bởi $[a,b[$ (resp. $]a,b]$). Tập hợp tất cả các $x\in E$ sao cho $a<x<b$ được gọi là *khoảng mở* với các đầu mút $a$ và $b$, và được ký hiệu bởi $]a,b[$.
Tập hợp tất cả các $x\in E$ sao cho $x\leq a$ (resp. $x<a$) được gọi là *khoảng đóng* (resp. *mở*) *không bị chặn về phía trái, với đầu mút phải a*, và được ký hiệu bởi $] \leftarrow,a]$ (resp. $]\leftarrow,a[$); tương tự, tập hợp tất cả các $x\in E$ sao cho $x\geq a$ (resp. $x>a$) được gọi là *khoảng đóng* (resp. *mở*) *không bị chặn về phía phải, với đầu mút trái a*, và được ký hiệu bởi $[a,\rightarrow[$ (resp. $]a,\rightarrow[$). Cuối cùng, ta xem chính E như một *khoảng mở không bị chặn theo cả hai hướng*, và ký hiệu nó bởi $]\leftarrow,\rightarrow[$.

5. Nếu X là một tập con của một tập hợp có thứ tự E, có nhiều nhất một phần tử $a$ của X sao cho $a\leq x$ với mọi $x\in X$; khi tồn tại một phần tử $a$ có tính chất này, nó được gọi là *phần tử nhỏ nhất của X*. Tương tự, có nhiều nhất một phần tử $b$ sao cho $x\leq b$ với mọi $x\in X$; $b$, nếu tồn tại, được gọi là *phần tử lớn nhất của X*.
Trong một *tập sắp thứ tự toàn phần E*, mọi tập con *hữu hạn* khác rỗng đều có một phần tử lớn nhất và một phần tử nhỏ nhất, lần lượt được gọi là các phần tử *lớn nhất và nhỏ nhất* của tập con.
Một tập hợp có thứ tự trong đó mọi tập con khác rỗng đều có một phần tử nhỏ nhất được gọi là *được sắp tốt*. Tập $\mathbf{N}$ các số nguyên tự nhiên là được sắp tốt; một tập con của $\mathbf{N}$ có một phần tử lớn nhất khi và chỉ khi nó là hữu hạn và khác rỗng. Người ta chứng minh, bằng cách sử dụng tiên đề lựa chọn, rằng trên mọi tập hợp tồn tại một cách sắp tốt (*định lý Zermelo*).
Trong tập $\mathfrak{P}(E)$ các tập con của một tập hợp E, được sắp thứ tự bởi quan hệ bao hàm, một tập con $\mathfrak{F}$ của $\mathfrak{P}(E)$ có một phần tử nhỏ nhất khi và chỉ khi giao của các tập hợp của $\mathfrak{F}$ thuộc về $\mathfrak{F}$, và khi đó giao này là phần tử nhỏ nhất. Tương tự, $\mathfrak{F}$ có một phần tử lớn nhất khi và chỉ khi hợp của các tập hợp của $\mathfrak{F}$ thuộc về $\mathfrak{F}$, và khi đó hợp này là phần tử lớn nhất.
Một tập con X của một tập hợp có thứ tự E được gọi là *trù mật trên* (tương ứng *trù mật dưới*) trong E nếu, với mỗi $y\in E$, tồn tại $x\in X$ sao cho $y\leq x$ (tương ứng $y\geq x$). Nói rằng một tập hợp có thứ tự $E$ có một phần tử lớn nhất (tương ứng nhỏ nhất) có nghĩa là tồn tại một tập con trù mật trên (tương ứng trù mật dưới) của $E$ gồm một phần tử duy nhất.

6. Cho $X$ là một tập con của một tập hợp có thứ tự $E$. Mọi $x\in X$ sao cho không tồn tại phần tử nào $z\in X$ mà $z<x$ được gọi là một *phần tử cực tiểu* của $X$. Mọi $y\in X$ sao cho không tồn tại phần tử nào $z\in X$ mà $z>y$ được gọi là một *phần tử cực đại* của $X$. Tập hợp các phần tử cực đại (hoặc tập hợp các phần tử cực tiểu) có thể rỗng; nó cũng có thể vô hạn. Nếu $X$ có một phần tử nhỏ nhất $a$, thì $a$ là *phần tử cực tiểu duy nhất* của $X$; tương tự, nếu $X$ có một phần tử lớn nhất $b$, thì $b$ là *phần tử cực đại duy nhất* của $X$.

7. Cho $X$ là một tập con của một tập hợp có thứ tự $E$. Nếu một phần tử $x\in E$ sao cho $z\leq x$ với mọi $z\in X$, thì $x$ được gọi là *một cận trên* của $X$. Tương tự, một phần tử $y\in E$ sao cho $z\geq y$ với mọi $z\in X$ được gọi là *một cận dưới* của $X$.

Tập hợp các cận trên (hoặc tập hợp các cận dưới) của một tập con $X$ có thể rỗng. Một tập con $X$ mà tập hợp các cận trên (tương ứng cận dưới) của nó không rỗng được gọi là *bị chặn trên* (tương ứng *bị chặn dưới*). Một tập hợp vừa bị chặn trên vừa bị chặn dưới được gọi đơn giản là *bị chặn*. Mọi phần tử lớn hơn một cận trên của $X$ đều là một cận trên của $X$; mọi phần tử nhỏ hơn một cận dưới của $X$ đều là một cận dưới của $X$.

Nếu tập hợp các cận trên của một tập con $X$ có phần tử nhỏ nhất $a$, thì $a$ được gọi là *cận trên nhỏ nhất* hay *cận trên đúng* của $X$. Nếu tập hợp các cận dưới của $X$ có phần tử lớn nhất $b$, thì $b$ được gọi là *cận dưới lớn nhất* hay *cận dưới đúng* của $X$. Nếu các cận này tồn tại, chúng là duy nhất theo định nghĩa, và lần lượt được ký hiệu bởi $\sup_E X$ (hoặc $\sup X$), $\inf_E X$ (hoặc $\inf X$). Nếu $X$ có một phần tử lớn nhất, thì nó là cận trên nhỏ nhất của $X$; nếu $X$ có một phần tử nhỏ nhất, thì nó là cận dưới lớn nhất của $X$. Đảo lại, nếu cận trên nhỏ nhất (tương ứng cận dưới lớn nhất) của $X$ tồn tại và thuộc $X$, thì nó là phần tử lớn nhất (tương ứng nhỏ nhất) của $X$.

Cho $f$ là một ánh xạ của một tập hợp $A$ vào $E$. Nếu $f(A)$ được chặn trên (tương ứng được chặn dưới, được chặn), thì $f$ được gọi là *bị chặn trên* (tương ứng *bị chặn dưới, bị chặn*). Nếu $f(A)$ có một cận trên nhỏ nhất (tương ứng cận dưới lớn nhất) trong $E$, thì cận này được gọi là *cận trên nhỏ nhất* (tương ứng *cận dưới lớn nhất*) của $f$ và được ký hiệu bởi $\sup_{x\in A} f(x)$ (tương ứng $\inf_{x\in A} f(x)$).

8. Một tập hợp tiền thứ tự $E$ trong đó mọi tập con *hữu hạn không rỗng* của $E$ đều *được chặn trên* (tương ứng *được chặn dưới*) được gọi là *có hướng phải* (hay *có hướng*) (tương ứng *có hướng trái*).

Một tập hợp có thứ tự $E$ trong đó mọi tập con *hữu hạn không rỗng* của $E$ đều có một cận trên nhỏ nhất và một cận dưới lớn nhất được gọi là một *dàn*.

Tập hợp các tập con của bất kỳ tập hợp nào, được sắp thứ tự bởi quan hệ bao hàm, là một *dàn*. Mọi tập hợp sắp thứ tự toàn phần đều là một dàn.

9. Một tập hợp có thứ tự E được gọi là *quy nạp* nếu nó thỏa mãn điều kiện sau: *mọi tập con được sắp thứ tự toàn phần của E đều có một cận trên*.

Tập hợp $\mathfrak{P}(E)$, được sắp thứ tự bởi quan hệ bao hàm, là quy nạp. Tập hợp các ánh xạ của các tập con của một tập hợp E vào một tập hợp F cũng vậy khi được sắp thứ tự bởi quan hệ “g mở rộng f” giữa f và g.

Một tập con tùy ý của một tập hợp quy nạp nói chung không phải là quy nạp. Nhưng nếu a là một phần tử bất kỳ của một tập hợp quy nạp E, thì tập con của E gồm tất cả các phần tử $x \in E$ sao cho $x \geq a$ là quy nạp.

10. Mệnh đề sau được chứng minh nhờ tiên đề lựa chọn, và được gọi là *bổ đề Zorn*:

*Mọi tập hợp có thứ tự quy nạp đều có ít nhất một phần tử cực đại.*

11. Trong tập hợp các tập con $\mathfrak{P}(E)$ của một tập hợp E, được sắp thứ tự bởi quan hệ bao hàm, cận trên nhỏ nhất của một tập hợp $\mathfrak{F}$ gồm các tập con của E là *hợp* của các tập hợp của $\mathfrak{F}$. Áp dụng bổ đề Zorn cho ta kết quả sau:

*Nếu $\mathfrak{F}$ là một tập hợp các tập con của một tập hợp E sao cho, với mỗi tập con $\mathfrak{G}$ của $\mathfrak{F}$ được sắp thứ tự toàn phần bởi quan hệ bao hàm, hợp của các tập hợp của $\mathfrak{G}$ thuộc $\mathfrak{F}$, thì $\mathfrak{F}$ có ít nhất một phần tử cực đại* (nghĩa là, một tập con của E thuộc $\mathfrak{F}$ nhưng không được chứa trong bất kỳ tập con nào khác của E thuộc $\mathfrak{F}$).

Một tập hợp $\mathfrak{F}$ gồm các tập con của một tập hợp E được gọi là *có đặc trưng hữu hạn* nếu tính chất “$X \in \mathfrak{F}$” *tương đương* với tính chất “mọi tập con *hữu hạn* của X thuộc $\mathfrak{F}$”. Với định nghĩa này, ta có định lý sau:

*Mọi tập hợp các tập con của E có đặc trưng hữu hạn đều có ít nhất một phần tử cực đại.*

12. Một ánh xạ f của một tập con A của một tập hợp có thứ tự E vào một tập hợp có thứ tự F được gọi là *tăng* (tương ứng *giảm*) nếu quan hệ $x \leq y$ giữa các phần tử tùy ý của A kéo theo $f(x) \leq f(y)$ (tương ứng $f(y) \leq f(x)$). Mọi hàm hằng trên A do đó vừa tăng vừa giảm, và điều đảo lại đúng nếu A là có hướng (phải hoặc trái).

Một ánh xạ f được gọi là *tăng ngặt* (tương ứng *giảm nghiêm ngặt*) nếu quan hệ $x < y$ kéo theo $f(x) < f(y)$ (tương ứng $f(x) < f(y)$).

Nếu E được *sắp thứ tự toàn phần*, mọi ánh xạ *tăng ngặt* (hoặc *giảm nghiêm ngặt*) của một tập con A của E vào một tập hợp có thứ tự F đều là *đơn ánh*.

Nếu I là một tập hợp *có thứ tự* các chỉ số, một họ $(X_i)_{i \in I}$ gồm các tập con của một tập hợp E được gọi là *tăng* (tương ứng *giảm*) nếu ánh xạ $i \to X_i$ của I vào $\mathfrak{P}(E)$, được sắp thứ tự bởi quan hệ bao hàm, là tăng (tương ứng giảm).

13. Cho I là một tập có hướng, và cho $(E_\alpha)_{\alpha \in I}$ là một họ các tập hợp được đánh chỉ số bởi I. Với mỗi cặp $(\alpha, \beta)$ các chỉ số trong I sao cho $\alpha \leq \beta$, gọi $f_{\beta \alpha}$ là một ánh xạ *từ* $E_\alpha$ *vào* $E_\beta$, và giả sử rằng các quan hệ $\alpha \leq \beta \leq \gamma$ suy ra $f_{\gamma \alpha} = f_{\gamma \beta} \circ f_{\beta \alpha}$.

Cho F là tổng của họ các tập hợp $(E_\alpha)_{\alpha \in I}$. Theo lạm dụng ngôn ngữ, ta sẽ đồng nhất các $E_\alpha$ với các tập con tương ứng của F. Với hai phần tử x và y trong F, gọi R $\{x, y\}$ là quan hệ sau đây (trong đó $\alpha$ và $\beta$ ký hiệu các phần tử của I sao cho $x\in E_\alpha$ và $y\in E_\beta$): “tồn tại $\gamma\in I$ sao cho $\gamma\geq\alpha$ và $\gamma\geq\beta$ và $f_{\gamma\alpha}(x)=f_{\gamma\beta}(y)$”. Khi đó R là một quan hệ tương đương trên F. Cho $E$ là tập thương $F/R$, và cho $f$ là ánh xạ chính tắc $F\to F/R$. Tập hợp $E$ được gọi là *giới hạn trực tiếp của họ* $(E_\alpha)_{\alpha\in I}$ *đối với họ các ánh xạ* $(f_{\beta\alpha})$, và hạn chế $f_\alpha$ của f trên $E_\alpha$ được gọi là *ánh xạ chính tắc của $E_\alpha$ vào E*. Ta có $f_\beta\circ f_{\beta\alpha}=f_\alpha$ mỗi khi $\alpha\leq\beta$. Ta viết

$$
E=\underset{\longrightarrow}{\lim}\,(E_\alpha,f_{\beta\alpha})
$$

hoặc đơn giản $E=\underset{\longrightarrow}{\lim}\,E_\alpha$ khi không có nguy cơ nhầm lẫn. Theo lạm dụng ngôn ngữ, cặp $((E_\alpha),(f_{\beta\alpha}))$ được gọi là một *hệ trực tiếp của các tập hợp đối với* I.

Nếu các $f_{\beta\alpha}$ là đơn ánh, thì các $f_\alpha$ là đơn ánh. Trong trường hợp này, ta thường đồng nhất $E_\alpha$ và $f_\alpha(E_\alpha)$, và do đó xem E như *hợp* của các $E_\alpha$. Ngược lại, nếu một tập hợp $E'$ là hợp của một họ $(E'_\alpha)_{\alpha\in I}$ các tập con sao cho quan hệ $\alpha\leq\beta$ suy ra $E'_\alpha\subset E'_\beta$, và nếu (với $\alpha\leq\beta$) $j_{\beta\alpha}$ ký hiệu đơn ánh chính tắc của $E'_\alpha$ vào $E'_\beta$, thì ta có thể đồng nhất $\underset{\longrightarrow}{\lim}\,(E'_\alpha,j_{\beta\alpha})$ với $E'$, và các ánh xạ chính tắc của các $E'_\alpha$ vào $\underset{\longrightarrow}{\lim}\,(E'_\alpha,j_{\beta\alpha})$ với các đơn ánh chính tắc của các $E'_\alpha$ vào E.

Nói chung, cho $(E_\alpha,f_{\beta\alpha})$ là một hệ trực tiếp các tập hợp tương đối với $I$, và với mỗi $\alpha\in I$, cho $g_\alpha$ là một ánh xạ từ $E_\alpha$ vào một tập hợp $E'$ sao cho quan hệ $\alpha\leq\beta$ kéo theo $g_\beta\circ f_{\beta\alpha}=g_\alpha$. Khi đó tồn tại một ánh xạ duy nhất $g$ từ $E=\underset{\longrightarrow}{\lim}\,E_\alpha$ vào $E'$ sao cho $g_\alpha=g\circ f_\alpha$ với mọi $\alpha\in I$. Ánh xạ $g$ là toàn ánh khi và chỉ khi $E'$ là hợp của các $g_\alpha(E_\alpha)$. Ánh xạ $g$ là đơn ánh khi và chỉ khi, với mỗi $\alpha\in I$, các quan hệ $x\in E_\alpha$, $y\in E_\alpha$, $g_\alpha(x)=g_\alpha(y)$ kéo theo rằng tồn tại $\beta\geq\alpha$ sao cho $f_{\beta\alpha}(x)=f_{\beta\alpha}(y)$. Nếu $g$ là song ánh, $E'$ đôi khi được đồng nhất với giới hạn trực tiếp của các $E_\alpha$.

Cho $(A_\alpha,\varphi_{\beta\alpha})$ và $(B_\alpha,\psi_{\beta\alpha})$ là hai hệ trực tiếp các tập hợp tương đối với cùng một tập hợp chỉ số $I$. Cho $A=\underset{\longrightarrow}{\lim}\,(A_\alpha,\varphi_{\beta\alpha})$, $B=\underset{\longrightarrow}{\lim}\,(B_\alpha,\psi_{\beta\alpha})$, và với mỗi $\alpha\in I$, cho $\varphi_\alpha$ (resp. $\psi_\alpha$) là ánh xạ chính tắc từ $A_\alpha$ vào $A$ (resp. từ $B_\alpha$ vào $B$). Với mỗi $\alpha\in I$, cho $u_\alpha$ là một ánh xạ từ $A_\alpha$ vào $B_\alpha$ sao cho $u_\beta\circ\varphi_{\beta\alpha}=\psi_{\beta\alpha}\circ u_\alpha$ khi $\alpha\leq\beta$. Họ $(u_\alpha)$ được gọi là một *hệ trực tiếp các ánh xạ từ* $(A_\alpha,\varphi_{\beta\alpha})$ *vào* $(B_\alpha,\psi_{\beta\alpha})$. Trong các điều kiện này, tồn tại một ánh xạ duy nhất $u:A\to B$ sao cho $u\circ\varphi_\alpha=\psi_\alpha\circ u_\alpha$ với mọi $\alpha\in I$. Ánh xạ $u$ được gọi là *giới hạn trực tiếp của* các $u_\alpha$, và được viết $u=\underset{\longrightarrow}{\lim}\,u_\alpha$, miễn là không có nguy cơ nhầm lẫn. Cho $(C_\alpha,\theta_{\beta\alpha})$ là một hệ trực tiếp khác của các tập hợp tương đối với $I$, cho $(v_\alpha)$ là một hệ trực tiếp các ánh xạ từ $(B_\alpha,\psi_{\beta\alpha})$ vào $(C_\alpha,\theta_{\beta\alpha})$, và cho $v=\underset{\longrightarrow}{\lim}\,v_\alpha$. Khi đó

$$
\underset{\longrightarrow}{\lim}\,(v_\alpha\circ u_\alpha)=v\circ u.
$$

Giữ ký hiệu trên, đặt $D_\alpha=A_\alpha\times B_\alpha$ và $\omega_{\beta\alpha}=\varphi_{\beta\alpha}\times\psi_{\beta\alpha}$. Khi đó họ $(D_\alpha,\omega_{\beta\alpha})$ là một hệ trực tiếp các tập hợp. Đặt $D=\underset{\longrightarrow}{\lim}\,(D_\alpha,\omega_{\beta\alpha})$, gọi $\omega_\alpha$ là ánh xạ chính tắc của $D_\alpha$ vào $D$, đặt $D'=A\times B$, và gọi $\omega'_\alpha=\varphi_\alpha\times\psi_\alpha$. Khi đó tồn tại một song ánh duy nhất (gọi là chính tắc) $f:D\to D'$ sao cho $f\circ\omega_\alpha=\omega'_\alpha$ với mọi $\alpha\in I$. Ta thường đồng nhất tích $D'$ của các giới hạn trực tiếp với giới hạn trực tiếp $D$ của các tích $D_\alpha$.

Cho $J$ là một tập con cofinal của $I$; khi đó $J$ cũng có hướng. Nếu $( (E_\alpha)_{\alpha\in I},(f_{\beta\alpha})_{\alpha,\beta\in I})$ là một hệ trực tiếp các tập hợp đối với $I$, thì $( (E_\alpha)_{\alpha\in J},(f_{\beta\alpha})_{\alpha,\beta\in J})$ là một hệ trực tiếp các tập hợp đối với $J$. Gọi $E'$ là giới hạn trực tiếp của nó, và gọi $f'_\alpha$ là ánh xạ chính tắc của $E_\alpha$ vào $E'$ với mọi $\alpha\in J$. Khi đó tồn tại một ánh xạ duy nhất $g:E'\to E$ sao cho $g(f'_\alpha(x))=f_\alpha(x)$ với mọi $\alpha\in J$ và mọi $x\in E_\alpha$ (trong đó $f_\alpha$ chỉ ánh xạ chính tắc của $E_\alpha$ vào $E$). Ánh xạ này là một song ánh, nhờ đó $E'$ thường được đồng nhất với $E$.

14. Cho $I$ là một tập hợp có thứ tự trước và cho $(E_\alpha)_{\alpha\in I}$ là một họ các tập hợp được đánh chỉ số bởi $I$. Với mỗi cặp $(\alpha,\beta)$ các chỉ số của $I$ sao cho $\alpha\leq\beta$, gọi $f_{\alpha\beta}$ là một ánh xạ của $E_\beta$ vào $E_\alpha$, và giả sử rằng các quan hệ $\alpha\leq\beta\leq\gamma$ kéo theo $f_{\alpha\gamma}=f_{\alpha\beta}\circ f_{\beta\gamma}$.

Cho $G$ là tích của họ các tập hợp $(E_\alpha)_{\alpha\in I}$. Cho $E$ là tập con của $G$ gồm tất cả các phần tử $x$ thỏa mãn mọi quan hệ $pr_\alpha x=f_{\alpha\beta}(pr_\beta x)$, với mọi cặp chỉ số $\alpha,\beta$ sao cho $\alpha\leq\beta$. Tập hợp $E$ được gọi là giới hạn ngược của họ $(E_\alpha)_{\alpha\in I}$ đối với họ các ánh xạ $(f_{\alpha\beta})$, và hạn chế $f_\alpha$ của $pr_\alpha$ lên $E$ được gọi là ánh xạ chính tắc của $E$ vào $E_\alpha$. Ta có $f_\alpha=f_{\alpha\beta}\circ f_\beta$ khi $\alpha\leq\beta$. Ta viết

$$
E=\lim (E_\alpha,f_{\alpha\beta}),
$$

hoặc đơn giản

$$
E=\lim E_\alpha
$$

khi không có nguy cơ nhầm lẫn.

Theo cách nói lạm dụng, cặp $((E_\alpha),(f_{\alpha\beta}))$ được gọi là một hệ ngược các tập hợp đối với $I$.

Cần lưu ý rằng $E$ có thể rỗng, ngay cả khi tất cả các $E_\alpha$ đều khác rỗng và tất cả các ánh xạ $f_{\alpha\beta}$ đều toàn ánh.

Với mỗi $\alpha\in I$, cho $g_\alpha$ là một ánh xạ từ một tập hợp $E'$ vào $E_\alpha$ sao cho quan hệ $\alpha\leq\beta$ kéo theo $f_{\alpha\beta}\circ g_\beta=g_\alpha$. Khi đó tồn tại một ánh xạ duy nhất $g$ từ $E'$ vào $E$ sao cho $g_\alpha=f_\alpha\circ g$ với mọi $\alpha\in I$. Để $g$ đơn ánh, điều kiện cần và đủ là với mỗi cặp phần tử phân biệt $x',y'$ của $E'$, phải tồn tại $\alpha\in I$ sao cho $g_\alpha(x')\neq g_\alpha(y')$.

Cho $(A_\alpha,\varphi_{\alpha\beta})$ và $(B_\alpha,\psi_{\alpha\beta})$ là hai hệ ngược của các tập hợp đối với cùng một tập chỉ số $I$. Gọi $A=\lim(A_\alpha,\varphi_{\alpha\beta})$, $B=\lim(B_\alpha,\psi_{\alpha\beta})$, và với mỗi $\alpha\in I$ gọi $\varphi_\alpha$ (tương ứng $\psi_\alpha$) là ánh xạ chính tắc của $A$ vào $A_\alpha$ (tương ứng của $B$ vào $B_\alpha$). Với mỗi $\alpha\in I$ gọi $u_\alpha$ là một ánh xạ của $A_\alpha$ vào $B_\alpha$ sao cho $\psi_{\alpha\beta}\circ u_\beta=u_\alpha\circ\varphi_{\alpha\beta}$ mỗi khi $\alpha\leq\beta$. Họ $(u_\alpha)$ được gọi là một hệ ngược các ánh xạ của $(A_\alpha,\varphi_{\alpha\beta})$ vào $(B_\alpha,\psi_{\alpha\beta})$. Với các điều kiện này tồn tại một ánh xạ duy nhất $u:A\to B$ sao cho $\psi_\alpha\circ u=u_\alpha\circ\varphi_\alpha$ với mọi $\alpha\in I$. Ánh xạ $u$ được gọi là giới hạn ngược của các $u_\alpha$, và được viết là $u=\underset{\longleftarrow}{\lim}\,u_\alpha$ khi không có nguy cơ nhầm lẫn. Gọi $(C_\alpha,\theta_{\alpha\beta})$ là một hệ ngược khác của các tập hợp đối với $I$, gọi $v_\alpha$ là một hệ ngược các ánh xạ của $(B_\alpha,\psi_{\alpha\beta})$ vào $(C_\alpha,\theta_{\alpha\beta})$, và gọi $v=\underset{\longleftarrow}{\lim}\,v_\alpha$. Khi đó ta có $\underset{\longleftarrow}{\lim}\,(v_\alpha\mathbin{\circ}u_\alpha)=v\mathbin{\circ}u$.

Gọi $J$ là một tập con đồng đẳng của $I$, và giả sử rằng $J$ là *có hướng* (đối với thứ tự cảm sinh từ $I$). Nếu $((E_\alpha)_{\alpha\in I},(f_{\alpha\beta})_{\alpha,\beta\in I})$ là một hệ ngược các tập hợp đối với $I$, có giới hạn ngược $E$, thì $((E_\alpha)_{\alpha\in J},(f_{\alpha\beta})_{\alpha,\beta\in J})$ cũng là một hệ ngược các tập hợp, đối với $J$. Gọi $E'$ là giới hạn ngược của nó và gọi $f'_\alpha$ là ánh xạ chính tắc của $E'$ vào $E_\alpha$, trong đó $\alpha\in J$. Với mỗi $x\in E$ đặt $g(x)=(f_\alpha(x))_{\alpha\in J}\in E'$ (trong đó $f_\alpha$ chỉ ánh xạ chính tắc của $E$ vào $E_\alpha$). Khi đó $g$ là một *song ánh* của $E$ lên $E'$, nhờ đó $E'$ thường được đồng nhất với $E$.

[^1]: Theo quan điểm của chúng tôi trong Bản tóm tắt các kết quả này, chúng tôi giả sử lý thuyết về các số nguyên đã được biết. Nhưng không nên nghĩ rằng lý thuyết này là cần thiết để xây dựng lý thuyết tập hợp; khi tham khảo Chương III, độc giả sẽ thấy rằng ngược lại, các số nguyên có thể được định nghĩa, và tất cả các tính chất đã biết của chúng được chứng minh, từ các kết quả của lý thuyết tập hợp. Theo thuật ngữ của chúng tôi, $0$ thuộc $\mathbf{N}$.
[^2]: Như vậy, theo thuật ngữ của chúng tôi, “nhỏ hơn” và “lớn hơn” không loại trừ “bằng”.
