---
book: top
book_title: General Topology
chapter: X
chapter_title: Function spaces
section: 1
section_title: The uniformity of $\mathcal{G}$-convergence
lang: vi
source: top-v-x
pdf_pages: 0280-0289, 0324-0327
extraction: ocr
subsections:
    - "no": 1
      title: THE UNIFORMITY OF UNIFORM CONVERGENCE
      page: 0
      pdf_page: 280
    - "no": 2
      title: $\mathfrak{S}$-convergence
      page: 0
      pdf_page: 281
    - "no": 3
      title: EXAMPLES OF $\mathcal{E}$-CONVERGENCE
      page: 0
      pdf_page: 283
    - "no": 4
      title: PROPERTIES OF THE SPACES $\mathcal{F}_\mathcal{S}(X; Y)$
      page: 0
      pdf_page: 284
    - "no": 5
      title: COMPLETE SUBSETS OF $\mathcal{F}_\mathcal{S}(X; Y)$
      page: 0
      pdf_page: 285
    - "no": 6
      title: $\mathcal{E}$-CONVERGENCE IN SPACES OF CONTINUOUS MAPPINGS
      page: 0
      pdf_page: 286
statements: 33
exercises: 12
content_sha256: e9ad301c5d1d3b1e968551ac24dd94529831f0a42ef2ec4554ad1886841d28ea
translated_from: content/en/top/X/01_s1_the_uniformity_of_mathcal_g_convergence.md
source_content_sha256: df654399a9ca6be97ffed28b6ed69e1c999f8eb14fab79d88fd374cacd6a9c89
translation_model: gpt-5-6, gpt-5-6-mini, gpt-5.4-mini
translation_run: translate-vi-17a8f949
glossary_version: 34
glossary_terms_sha256: d6ca7dcf11bacedaadf039513758e51e1ee24add6932313b7a1bfee8c81bfad8
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 1. TÍNH ĐỒNG NHẤT CỦA SỰ HỘI TỤ $\mathcal{G}$

Ký hiệu. Nếu $X$ và $Y$ là hai tập hợp bất kỳ, ta nhắc lại rằng tập hợp tất cả các ánh xạ từ $X$ vào $Y$ được ký hiệu bởi $\mathcal{F}(X; Y)$, và có thể được đồng nhất với tập hợp tích $Y^X$ (Lý thuyết Tập hợp, Chương II, § 5, no. 2). Với mỗi tập con $H$ của $\mathcal{F}(X; Y)$ và mỗi $x \in X$, ta sẽ ký hiệu bởi $H(x)$ tập hợp các phần tử $u(x) \in Y$ khi $u$ chạy qua $H$. Nếu $\Phi$ là một cơ sở lọc trên $\mathcal{F}(X; Y)$, ta ký hiệu bởi $\Phi(x)$ cơ sở lọc trên $Y$ được tạo bởi các tập hợp $H(x)$ khi $H$ chạy qua $\Phi$. Cuối cùng, ta nhắc lại rằng, với mỗi $u \in \mathcal{F}(X; Y)$ và mỗi tập con $A$ của $X$, $u|A$ ký hiệu hạn chế của $u$ lên $A$, là một ánh xạ từ $A$ vào $Y$; nếu $H$ là một tập con của $\mathcal{F}(X; Y)$, $H|A$ sẽ ký hiệu tập hợp các hạn chế $u|A$ của các hàm $u \in H$.

### 1. TÍNH ĐỒNG NHẤT CỦA SỰ HỘI TỤ ĐỀU

Cho $X$ là một tập hợp và $Y$ là một không gian đồng nhất. Với mỗi lân cận đồng nhất $V$ của $Y$, ký hiệu $W(V)$ là tập hợp tất cả các cặp $(u, v)$ của các ánh xạ từ $X$ vào $Y$ sao cho $(u(x), v(x)) \in V$ với mọi $x \in X$. Khi $V$ chạy qua tập hợp các lân cận đồng nhất của $Y$, các tập hợp $W(V)$ tạo thành một hệ cơ sở của các lân cận đồng nhất của một tính đồng nhất trên $\mathcal{F}(X; Y)$. Vì chúng rõ ràng thỏa mãn Tiên đề $(U'_1)$ (Chương II, § 1, no. 1); nếu $V, V'$ là hai lân cận đồng nhất của $Y$ sao cho $V \subset V'$, ta có $W(V) \subset W(V')$, và do đó các tập hợp $W(V)$ thỏa mãn

$(B_1)$ (Chương I, § 6, no. 3); ta có $\widehat{W(V)} = W(\overline{V})$ nên $(U''_{II})$ được thỏa mãn; cuối cùng, các quan hệ "$(u(x), v(x)) \in V$ với mọi $x \in X$" và "$(v(x), w(x)) \in V$ với mọi $x \in X$" suy ra quan hệ "$(u(x), w(x)) \in \overline{V}^2$ với mọi $x \in X$"; nói cách khác, ta có $\widehat{W(V)} \subset W(\overline{V}^2)$, điều này chứng minh $(U'''_{III})$.

#### Định nghĩa 1 {#top-x-s1-def-1 .statement}

*Cấu trúc đều trên tập hợp $\mathcal{F}(X; Y)$ có một hệ cơ sở các lân cận là tập hợp các tập con $W(V)$, trong đó $V$ chạy qua tập hợp các lân cận của $Y$, được gọi là cấu trúc đều của hội tụ đều. Tôpô do nó cảm sinh được gọi là tôpô của hội tụ đều. Nếu một bộ lọc $\Phi$ trên $\mathcal{F}(X; Y)$ hội tụ đến một phần tử $u_0$ đối với tôpô này, thì $\Phi$ được nói là hội tụ đều đến $u_0$.*

Chú ý rằng *tôpô* của hội tụ đều trên $\mathcal{F}(X; Y)$ phụ thuộc vào cấu trúc đều của $Y$ chứ không chỉ vào tôpô của $Y$ (Bài tập 4).

Không gian đều thu được bằng cách trang bị cho $\mathcal{F}(X; Y)$ cấu trúc đều của hội tụ đều được ký hiệu là $\mathcal{F}_u(X; Y)$.

### 2. Hội tụ $\mathfrak{S}$

#### Định nghĩa 2 {#top-x-s1-def-2 .statement}

*Cho $X$ là một tập hợp, $Y$ là một không gian đều, $\mathfrak{S}$ là một tập hợp các tập con của $X$. Cấu trúc đều của hội tụ đều trong các tập hợp của $\mathfrak{S}$, hay đơn giản là cấu trúc đều của hội tụ $\mathfrak{S}$, là cấu trúc đều thô nhất trên $\mathcal{F}(X; Y)$ làm cho các ánh xạ hạn chế $u \to u|A$ của $\mathcal{F}(X, Y)$ vào các không gian đều $\mathcal{F}_u(A; Y)$ là liên tục đều, trong đó $A$ chạy qua $\mathfrak{S}$. Không gian đều thu được bằng cách trang bị cho $\mathcal{F}(X; Y)$ cấu trúc đều của hội tụ $\mathfrak{S}$ được ký hiệu là $\mathcal{F}_{\mathfrak{S}}(X; Y)$.*

Tôpô cảm sinh bởi cấu trúc đều của hội tụ $\mathfrak{S}$ được gọi là *tôpô của hội tụ $\mathfrak{S}$*; nó là tôpô thô nhất sao cho tất cả các ánh xạ $u \to u|A$ của $\mathcal{F}(X; Y)$ vào $\mathcal{F}_u(A; Y)$ ($A \in \mathfrak{S}$) là liên tục (Chương II, § 2, no. 3, Mệnh đề 4, Hệ quả).

Một bộ lọc $\Phi$ trên $\mathcal{F}(X; Y)$ hội tụ đến $u_0$ đối với tôpô của hội tụ $\mathfrak{S}$ khi và chỉ khi $u|A$ hội tụ đều đến $u_0|A$ đối với $\Phi$ với mọi $A \in \mathfrak{S}$ (Chương I, § 7, no. 6, Mệnh đề 10), và do đó $\Phi$ được nói là *hội tụ đều đến $u_0$ trên các tập hợp của $\mathfrak{S}$*.

Một cơ sở lọc $\Phi$ trên $\mathcal{F}_{\mathfrak{S}}(X; Y)$ là một cơ sở lọc Cauchy khi và chỉ khi, với mỗi $A \in \mathfrak{S}$, ảnh của $\Phi$ qua ánh xạ $u \to u|A$ là một cơ sở lọc Cauchy trên $\mathcal{F}_u(A; Y)$ (Chương II, § 3, no. 1, Mệnh đề 4).

Cho $f$ là một ánh xạ từ một không gian tôpô (tương ứng, không gian đều) $Z$ vào $\mathcal{F}_{\mathfrak{S}}(X; Y)$. Khi đó $f$ liên tục (tương ứng, liên tục đều) khi và chỉ khi, với mỗi $A \in \mathfrak{S}$, ánh xạ $z \to f(z)|A$ từ $Z$ vào $\mathcal{F}_u(A; Y)$ là liên tục (tương ứng, liên tục đều) (Chương I, § 2, no. 3, Mệnh đề 4; Chương II, § 2, no. 3, Mệnh đề 4).

Cuối cùng, cho $M$ là một tập con của $\mathcal{F}_{\mathfrak{S}}(X; Y)$; khi đó $M$ là tiền compact khi và chỉ khi, với mỗi $A \in \mathfrak{S}$, tập hợp các hạn chế $u|A$ với $u \in M$ là một tập con tiền compact của $\mathcal{F}_u(A; Y)$ (Chương II, § 4, no. 2, Mệnh đề 3).

#### Nhận xét 1 {#top-x-s1-n2-rem-1 .statement}

Định nghĩa tổng quát của các lân cận của một đều đặn ban đầu (Chương II, § 2, no. 3, Mệnh đề 4) cho thấy rằng một hệ cơ sở của các lân cận của $\mathcal{F}_\mathcal{S}(X; Y)$ có thể thu được như sau: với mỗi $A \in \mathcal{S}$ và mỗi lân cận $V$ của một hệ cơ sở các lân cận $\mathcal{B}$ của $Y$, gọi $W(A, V)$ là tập hợp tất cả các cặp ánh xạ $(u, v)$ từ $X$ vào $Y$ sao cho $(u(x), v(x)) \in V$ với mỗi $x \in A$; khi $A$ chạy qua $\mathcal{S}$ và $V$ chạy qua $\mathcal{B}$, các *giao hữu hạn của các tập hợp* $W(A, V)$ tạo thành một hệ cơ sở các lân cận của $\mathcal{F}_\mathcal{S}(X; Y)$.

Mô tả này cho thấy ngay lập tức rằng nếu $\mathcal{S}, \mathcal{S}'$ là hai tập hợp các tập con của $X$ sao cho $\mathcal{S} \subset \mathcal{S}'$, thì đều đặn của sự hội tụ theo $\mathcal{S}'$ là *mịn hơn* đều đặn của sự hội tụ theo $\mathcal{S}$.

#### Nhận xét 2 {#top-x-s1-n2-rem-2 .statement}

Tuy nhiên, đều đặn của sự hội tụ theo $\mathcal{S}$ không thay đổi khi thay thế $\mathcal{S}$ bởi tập hợp $\mathcal{S}'$ gồm tất cả các tập con của $X$ *được chứa trong các hợp hữu hạn của các tập hợp của* $\mathcal{S}$. Trong việc nghiên cứu sự hội tụ theo $\mathcal{S}$, do đó ta luôn có thể giới hạn vào trường hợp tập hợp $\mathcal{S}$ thỏa mãn hai điều kiện sau:

(F'$_1$) *Mọi tập con của một tập hợp thuộc* $\mathcal{S}$ *đều thuộc* $\mathcal{S}$.

(F'$_2$) *Mọi hợp hữu hạn của các tập hợp thuộc* $\mathcal{S}$ *đều thuộc* $\mathcal{S}$.

Nếu thỏa mãn (F'$_2$), ta thu được một hệ cơ bản các lân cận trong $\mathcal{F}_\mathcal{S}(X; Y)$ bằng cách lấy tất cả các tập hợp $W(A, V)$, trong đó $A$ chạy qua $\mathcal{S}$ và $V$ chạy qua một hệ cơ bản các lân cận của $Y$.

#### Nhận xét 3 {#top-x-s1-n2-rem-3 .statement}

Tính đều của sự hội tụ $\mathcal{S}$ là ảnh ngược, theo ánh xạ $u \to (u|A)_{A \in \mathcal{S}}$ của $\mathcal{F}(X; Y)$ vào $\prod_{A \in \mathcal{S}} \mathcal{F}_u(A; Y)$, của tính đều của không gian tích này (Chương II, § 2, no. 6, Mệnh đề 8). Nếu $\mathcal{S}$ là một *phủ* của $X$, ánh xạ này là *đơn ánh* và $\mathcal{F}_\mathcal{S}(X; Y)$ do đó đẳng cấu với không gian con đều của $\prod_{A \in \mathcal{S}} \mathcal{F}_u(A; Y)$ là ảnh của ánh xạ này.

#### Mệnh đề 1 {#top-x-s1-prop-1 .statement}

*Nếu* $Y$ *là Hausdorff và* $\mathcal{S}$ *là một phủ của* $X$, *thì không gian* $\mathcal{F}_\mathcal{S}(X; Y)$ *là Hausdorff*.

Cho $u, v$ là hai phần tử của $\mathcal{F}_\mathcal{S}(X; Y)$ sao cho $(u, v) \in W(A, V)$ với mọi lân cận $V$ của $Y$ và mọi $A \in \mathcal{S}$. Vì $Y$ là Hausdorff nên suy ra rằng $u$ và $v$ trùng nhau trên mọi tập hợp $A \in \mathcal{S}$, và vì $\mathcal{S}$ phủ $X$ nên ta phải có $u = v$.

#### Nhận xét 4 {#top-x-s1-n2-rem-4 .statement}

Cho $H$ là một tập con của $\mathcal{F}(X; Y)$. Do lạm dụng ngôn ngữ, tính đều (tương ứng tôpô) cảm sinh trên $H$ bởi tính đều (tương ứng tôpô) của sự hội tụ $\mathcal{S}$ trên $\mathcal{F}(X; Y)$ được gọi là tính đều (tương ứng tôpô) của sự hội tụ $\mathcal{S}$ trên tập hợp $H$.

#### Nhận xét 5 {#top-x-s1-n2-rem-5 .statement}

Cho $L$ là một tập hợp được lọc bởi một lọc $\mathfrak{S}$, và cho $\lambda \to u_\lambda$ là một ánh xạ của $L$ vào $\mathcal{F}_\mathcal{S}(X; Y)$ có giới hạn $v$ đối với $\mathfrak{S}$; khi đó ta nói rằng, *đối với lọc* $\mathfrak{S}$, *các ánh xạ* $u_\lambda$ *của* $X$ *vào* $Y$ *hội tụ đều tới* $v$ *[hoặc họ* $(u_\lambda)$ *hội tụ đều tới* $v$] *trong mỗi tập hợp của* $\mathcal{S}$. *Nếu* $L = \mathbf{N}$ *và* $\mathfrak{S}$ *là lọc Fréchet*, ta bỏ qua việc nhắc đến $\mathfrak{S}$ *trong mệnh đề này*.

More particularly, suppose that there is a commutative and associative law of composition (written additively) defined on $Y$. If $(u_n)$ is any sequence of mappings of $X$ into $Y$, let $v_n$ be the mapping defined by

$$
v_n(x) = \sum_{k=0}^n u_k(x) \quad (n \in \mathbf{N});
$$

we say that *the series whose general term is* $u_n$ *is uniformly convergent in every set of* $\mathcal{G}$ *if the sequence* $(v_n)$ *is uniformly convergent in every set of* $\mathcal{G}$. Likewise we define a *uniformly summable family* $(u_\lambda)_{\lambda \in L}$ of mappings of $X$ into $Y$ by considering the mappings $x \to \sum_{\lambda \in J} n_\lambda(x)$ for all finite subsets $J$ of $L$ and the limit of these mappings in $\mathcal{F}_\mathcal{G}(X; Y)$ with respect to the directed set of finite subsets of $L$ (Chương III, § 5, no. 1).

#### Nhận xét 6 {#top-x-s1-n2-rem-6 .statement}

Suy ra ngay từ Định nghĩa 1 và 2 rằng, với mọi $x \in \bigcup_{A \in \mathcal{G}} A$, ánh xạ $u \to u(x)$ của $\mathcal{F}_\mathcal{G}(X; Y)$ vào $Y$ là *liên tục đều*. Do đó, nói riêng, nếu $\overline{H}$ ký hiệu bao đóng của một tập con $H$ của $\mathcal{F}_\mathcal{G}(X; Y)$, ta có $\overline{H}(x) \subset \overline{H(x)}$ với mọi $x \in \bigcup_{A \in \mathcal{G}} A$ (Chương I, § 2, no. 1, Định lý 1).

### 3. CÁC VÍ DỤ VỀ $\mathcal{E}$-HỘI TỤ

I. *Hội tụ đều trong một tập con của* $X$. Cho $A$ là một tập con của $X$ và lấy $\mathcal{G} = \{ A \}$. Khi đó cấu trúc (resp. tôpô) của hội tụ $\mathcal{G}$ được gọi là *cấu trúc* (resp. *tôpô*) *của hội tụ đều trong* $A$; nếu một bộ lọc $\Phi$ trên $\mathcal{F}_\mathcal{G}(X; Y)$ hội tụ đến $u_0$, thì nói rằng nó hội tụ đến $u_0$ *đều trong* $A$. Khi $A = X$ ta thu lại cấu trúc hội tụ đều đã định nghĩa ở no. 1.

II. *Hội tụ từng điểm trong một tập con của* $X$. Cho $A$ là một tập con của $X$, và lấy $\mathcal{G}$ là tập hợp tất cả các tập con của $X$ chỉ gồm một điểm thuộc $A$ (theo Nhận xét 2 của no. 2 thì cũng như thế nếu ta lấy $\mathcal{G}$ là tập hợp tất cả các tập con hữu hạn của $A$). Khi đó cấu trúc (resp. tôpô) của hội tụ $\mathcal{G}$ được gọi là *cấu trúc* (resp. *tôpô*) *của hội tụ từng điểm trong* $A$; nếu một bộ lọc $\Phi$ trên $\mathcal{F}_\mathcal{G}(X; Y)$ hội tụ đến $u_0$, thì nói rằng nó hội tụ đến $u_0$ *từng điểm trong* $A$. Điều này xảy ra khi và chỉ khi, với mỗi $x \in A$, $u_0(x)$ là một giới hạn của $u(x)$ đối với bộ lọc $\Phi$.

Đặc biệt, khi $A = X$, tính đều (resp. tôpô) của hội tụ điểm trong $X$ được gọi đơn giản là *tính đều* (resp. *tôpô*) *của hội tụ điểm*; không gian đều thu được bằng cách trang bị cho $\mathcal{F}(X; Y)$ cấu trúc này được ký hiệu bởi $\mathcal{F}_s(X; Y)$. Chú ý rằng tôpô của hội tụ điểm chỉ là tôpô *tích* trên $Y^X$ và do đó chỉ phụ thuộc vào tôpô của $Y$, chứ không phụ thuộc vào cấu trúc đều của nó.

III. Hội tụ compact. Giả sử rằng $X$ là một không gian tôpô, và lấy $\mathcal{S}$ là tập hợp tất cả các tập con compact của $X$. Tính đều (resp. tôpô) của $\mathcal{S}$-hội tụ khi đó được gọi là tính đều (resp. tôpô) của hội tụ compact, và không gian đều thu được bằng cách trang bị cho $\mathcal{F}(X; Y)$ tính đều này được ký hiệu bởi $\mathcal{F}_c(X; Y)$. Cấu trúc của hội tụ compact thô hơn cấu trúc của hội tụ đều, và hai cấu trúc này trùng nhau nếu $X$ là compact; hơn nữa nó mịn hơn cấu trúc của hội tụ điểm, và hai cấu trúc này trùng nhau nếu $X$ là rời rạc.

Nếu $X$ là một không gian đều, ta có thể định nghĩa trên $\mathcal{F}(X; Y)$ tính đều của hội tụ tiềncompact bằng cách lấy $\mathcal{S}$ là tập hợp tất cả các tập con tiềncompact của $X$. Một lần nữa, nếu $X$ là một không gian metric, ta có thể lấy $\mathcal{S}$ là tập hợp tất cả các tập con bị chặn của $X$; tính đều của $\mathcal{S}$-hội tụ khi đó được gọi là tính đều của hội tụ bị chặn.

### 4. CÁC TÍNH CHẤT CỦA CÁC KHÔNG GIAN $\mathcal{F}_\mathcal{S}(X; Y)$

#### Mệnh đề 2 {#top-x-s1-prop-2 .statement}

Cho $X_1, X_2$ là hai tập hợp, cho $Y$ là một không gian đều và cho $\mathcal{S}_i$ là một tập hợp các tập con của $X_i$ ($i = 1, 2$) và $\mathcal{S}_1 \times \mathcal{S}_2$ là tập hợp các tập con của $X_1 \times X_2$ có dạng $A_1 \times A_2$, trong đó $A_i \in \mathcal{S}_i, i = 1, 2$. Khi đó song ánh chính tắc
$$
\mathcal{F}(X_1 \times X_2; Y) \to \mathcal{F}(X_1; \mathcal{F}(X_2; Y))
$$
(Lý thuyết tập hợp, R, § 4, no. 14) là một đẳng cấu của không gian đều
$$
\mathcal{F}_{\mathcal{S}_1 \times \mathcal{S}_2}(X_1 \times X_2; Y)
$$
lên $\mathcal{F}_{\mathcal{S}_1}(X_1; \mathcal{F}_{\mathcal{S}_2}(X_2; Y))$.

Cho $V$ là một lân cận đều của $Y$ và cho $A_i \in \mathcal{S}_i (i = 1, 2)$; khi đó suy ra ngay lập tức từ các định nghĩa rằng $W(A_1 \times A_2, V)$ được đồng nhất với $W(A_1, W(A_2, V))$ bởi song ánh chính tắc, và kết quả là ngay lập tức.

#### Mệnh đề 3 {#top-x-s1-prop-3 .statement}

a) Cho $X$ là một tập hợp; cho $\mathcal{S}$ là một tập hợp các tập con của $X$; cho $Y, Y'$ là hai không gian đều; và cho $f : Y \to Y'$ là một ánh xạ liên tục đều. Khi đó ánh xạ $u \to f \circ u$ từ $\mathcal{F}_\mathcal{S}(X; Y)$ vào $\mathcal{F}_\mathcal{S}(X; Y')$ là liên tục đều.

b) Cho $X, X'$ là hai tập hợp; cho $\mathcal{S}$ (tương ứng $\mathcal{S}'$) là một tập hợp các tập con của $X$ (tương ứng $X'$); cho $Y$ là một không gian đều; và cho $g : X' \to X$ là một ánh xạ sao cho, với mỗi $A' \in \mathcal{S}'$, $g(A')$ được chứa trong một hợp hữu hạn của các tập hợp thuộc $\mathcal{S}$. Khi đó ánh xạ $u \to u \circ g$ từ $\mathcal{F}_\mathcal{S}(X, Y)$ vào $\mathcal{F}_{\mathcal{S}'}(X'; Y)$ là đều liên tục.

#### Mệnh đề 4 {#top-x-s1-prop-4 .statement}

Cho $X, Y$ là hai tập hợp, cho $(X_\lambda)_{\lambda \in L}$ là một họ các tập hợp và cho $(Y_\mu)_{\mu \in M}$ là một họ các không gian đều. Với mỗi $\lambda \in L$, cho $\mathcal{S}_\lambda$ là một tập hợp các tập con của $X_\lambda$, cho $g_\lambda$ là một ánh xạ từ $X_\lambda$ vào $X$, và cho $\mathcal{S}$ là tập hợp các tập con của $X$ là hợp của các tập hợp $g_\lambda(\mathcal{S}_\lambda)$. Với mỗi $\mu \in M$, cho $f_\mu$ là một ánh xạ từ $Y$ vào $Y_\mu$, và trang bị cho $Y$ cấu trúc đều thô nhất sao cho các $f_\mu$ là đều liên tục. Khi đó cấu trúc đều của sự hội tụ $\mathcal{S}$ trên $\mathcal{F}(X; Y)$ là cấu trúc đều thô nhất làm cho các ánh xạ $u \to f_\mu \circ u \circ g_\lambda$ từ $\mathcal{F}(X; Y)$ vào $\mathcal{F}_{\mathcal{S}_\lambda}(X_\lambda, Y_\mu)$ đều liên tục.

Các mệnh đề này là những hệ quả ngay lập tức của mô tả một hệ cơ bản các lân cận của cấu trúc đều của sự hội tụ $\mathcal{S}$ được cho trong no. 2, Nhận xét 1; các chi tiết của các chứng minh được để cho người đọc. Mệnh đề 4 kéo theo, đặc biệt:

#### Hệ quả {#top-x-s1-n4-cor-1 .statement}

Cho $X$ là một tập hợp, cho $(Y_i)_{i \in I}$ là một họ các không gian đều và cho $\mathcal{S}$ là một tập hợp các tập con của $X$. Nếu ta trang bị $\prod_{i \in I} Y_i$ với cấu trúc đều tích, thì song ánh chính tắc của không gian đều $\mathcal{F}_\mathcal{S}(X, \prod_{i \in I} Y_i)$ lên không gian đều tích $\prod_{i \in I} \mathcal{F}_\mathcal{S}(X; Y_i)$ (Lý thuyết tập hợp, R, § 4, no. 13) là một đẳng cấu.

### 5. CÁC TẬP CON ĐẦY ĐỦ CỦA $\mathcal{F}_\mathcal{S}(X; Y)$

#### Mệnh đề 5 {#top-x-s1-prop-5 .statement}

Cho $\Phi$ là một tập hợp, $Y$ là một không gian đều và $\mathcal{S}$ là một tập hợp các tập con của $X$. Khi đó một lọc $\Phi$ trên $\mathcal{F}_\mathcal{S}(X; Y)$ hội tụ đến $u_0$ khi và chỉ khi $\Phi$ là một lọc Cauchy đối với cấu trúc đều của sự hội tụ $\mathcal{S}$ và hội tụ điểm tới điểm đến $u_0$ trong $B = \bigcup_{A \in \mathcal{S}} A$.

Vì cấu trúc của sự hội tụ điểm trong $B$ thô hơn cấu trúc của sự hội tụ $\mathcal{S}$, chỉ cần chỉ ra rằng với mỗi $A \in \mathcal{S}$ và mỗi lân cận đóng $V$ của $Y$, $W(A, V)$ là đóng trong $B$ đối với tôpô của sự hội tụ điểm (Chương II, § 3, no. 3, Mệnh đề 7). Bây giờ $W(A, V)$ là giao của các ảnh ngược của $V$ qua các ánh xạ $(u, v) \to (u(x), v(x))$ khi $x$ chạy qua $A$; các ánh xạ này liên tục đối với tôpô của sự hội tụ điểm (no. 2, Nhận xét 6), và kết quả suy ra.

#### Hệ quả 1 {#top-x-s1-prop-5-cor-1 .statement}

Một không gian con $H$ của $\mathcal{F}_\mathcal{S}(X; Y)$ là đầy đủ khi và chỉ khi, với mỗi lọ Cauchy $\Phi$ trên $H$, tồn tại $u_0 \in H$ sao cho $\Phi$ hội tụ điểm đến $u_0$ trong $B = \bigcup_{A \in \mathcal{S}} A$.

Điều này suy ra ngay lập tức từ Mệnh đề 5.

#### Hệ quả 2 {#top-x-s1-prop-5-cor-2 .statement}

Cho $\mathcal{S}_1, \mathcal{S}_2$ là hai tập hợp các tập con của $X$, có hợp bằng nhau và sao cho $\mathcal{S}_1 \subset \mathcal{S}_2$, và cho $H$ là một tập con của $\mathcal{F}(X; Y)$. Khi đó nếu $H$ là đầy đủ đối với sự hội tụ $\mathcal{S}_1$, thì nó là đầy đủ đối với sự hội tụ $\mathcal{S}_2$.

Vì mọi lọ Cauchy đối với sự hội tụ $\mathcal{G}_2$ cũng là một lọ Cauchy đối với sự hội tụ $\mathcal{G}_1$, và ta có thể áp dụng Hệ quả 1.

#### Hệ quả 3 {#top-x-s1-prop-5-cor-3 .statement}

*Cho $H$ là một tập con của $\mathcal{F}(X; Y)$ sao cho, với mỗi*
$$
x \notin B = \bigcup_{A \in \mathcal{G}} A,
$$
*bao đóng của $H(x)$ trong $Y$ là một không gian con đầy đủ của $Y$. Khi đó bao đóng $\overline{H}$ của $H$ trong $\mathcal{F}_{\mathcal{G}}(X; Y)$ là một không gian con đầy đủ.*

Cho $\Phi$ là một lọ Cauchy trên $\overline{H}$, và định nghĩa một ánh xạ $v : X \to Y$ như sau. Nếu $x \in B$, $\Phi(x)$ là một lọ Cauchy trên $\overline{H(x)}$ (no. 2, Nhận xét 6), do đó theo giả thiết nó có ít nhất một điểm giới hạn; lấy $v(x)$ là một trong các giới hạn này. Nếu $x \notin B$, lấy $v(x)$ là một điểm bất kỳ của $Y$. Với định nghĩa này của $v$, hiển nhiên rằng $\Phi$ hội tụ điểm đến $v$ trong $B$, và do đó $v$ là một giới hạn của $\Phi$ trong $\mathcal{F}_{\mathcal{G}}(X; Y)$ theo Mệnh đề 5.

Đặc biệt, nếu $Y$ là đầy đủ, giả thiết của Hệ quả 3 của Mệnh đề 5 được thỏa mãn với mọi $H \subset \mathcal{F}(X; Y)$; do đó:

#### Định lý 1 {#top-x-s1-thm-1 .statement}

*Cho $X$ là một tập hợp, cho $\mathcal{G}$ là một tập hợp các tập con của $X$, và cho $Y$ là một không gian đều đầy đủ. Khi đó không gian đều $\mathcal{F}_{\mathcal{G}}(X; Y)$ là đầy đủ.*

### 6. $\mathcal{E}$-HỘI TỤ TRONG CÁC KHÔNG GIAN CÁC ÁNH XẠ LIÊN TỤC

Cho $X, Y$ là hai không gian tôpô, và ký hiệu $\mathcal{C}(X; Y)$ tập hợp tất cả các *ánh xạ liên tục từ $X$ vào $Y$*. Nếu $\mathcal{G}$ là một tập hợp các tập con của $X$ và nếu $Y$ là một không gian đều, ta ký hiệu $\mathcal{C}_{\mathcal{G}}(X; Y)$ tập $\mathcal{C}(X; Y)$ được trang bị cấu trúc đều của $\mathcal{G}$-hội tụ. Đặc biệt $\mathcal{C}_s(X; Y), \mathcal{C}_c(X; Y)$ và $\mathcal{C}_u(X; Y)$ ký hiệu tập $\mathcal{C}(X; Y)$ được trang bị lần lượt cấu trúc đều của hội tụ từng điểm, hội tụ compact và hội tụ đều.

#### Mệnh đề 6 {#top-x-s1-prop-6 .statement}

*Cho $X$ là một không gian tôpô, $Y$ là một không gian đều và $\mathcal{G}$ là một tập hợp các tập con của $X$. Với mỗi $A \in \mathcal{G}$ và mỗi bao lân cận đóng $V$ của $Y$, các vết trên $\mathcal{C}(X; Y) \times \mathcal{C}(X; Y)$ của $W(A, V)$ và $W(\overline{A}, V)$ là như nhau.*

Vì nếu $u, v$ là các ánh xạ liên tục từ $X$ vào $Y$, thì ánh xạ $x \mapsto (u(x), v(x))$ từ $X$ vào $Y \times Y$ là liên tục, và giả thiết rằng $(u(x), v(x)) \in V$ với mọi $x \in A$ do đó suy ra rằng $(u(x), v(x)) \in \overline{V} = V$ với mọi $x \in \overline{A}$ (Chương I, § 2, no. 1, Định lý 1).

Nếu $\bar{\mathcal{G}}$ ký hiệu tập hợp các bao đóng trong $X$ của các tập của $\mathcal{G}$, Mệnh đề 6 cho thấy rằng, *trên* $\mathcal{C}(X; Y)$, các cấu trúc $\mathcal{G}$-hội tụ và $\bar{\mathcal{G}}$-hội tụ là giống hệt nhau.

**G-hội tụ trong các không gian các ánh xạ liên tục**

#### Hệ quả {#top-x-s1-n6-cor-1 .statement}

*Cho B là một tập con *trù mật* của X. Trên $C(X; Y)$, cấu trúc hội tụ đều trùng với cấu trúc hội tụ đều trong B.*

#### Mệnh đề 7 {#top-x-s1-prop-7 .statement}

*Cho X là một không gian tôpô, cho $\mathfrak{S}$ là một tập hợp các tập con của X và cho Y là một không gian đều. Nếu Y là Hausdorff và nếu hợp B của các tập hợp của $\mathfrak{S}$ là trù mật trong X, thì $C_{\mathfrak{S}}(X; Y)$ là Hausdorff.*

Vì nếu $(u, v)$ thuộc mọi tập $W(A, V)$, với $A \in \mathfrak{S}$ và V là một bao lân cận của Y, giả thiết rằng Y là Hausdorff cho ta biết rằng $u(x) = v(x)$ với mọi $x \in B$; nếu $u$ và $v$ liên tục, thì $u = v$ bởi nguyên lý mở rộng của các đẳng thức (Chương I, § 8, no. 1, Mệnh đề 2, Hệ quả 1).

Đặc biệt, trên $C(X; Y)$, tôpô hội tụ từng điểm trong một tập con *trù mật* của X là Hausdorff.

#### Mệnh đề 8 {#top-x-s1-prop-8 .statement}

*Cho X là một tập hợp, $\mathfrak{T}$ là một bộ lọc trên X, và Y là một không gian đều. Khi đó tập H các ánh xạ $u : X \to Y$ sao cho $u(\mathfrak{T})$ là một cơ sở Cauchy trên Y là đóng trong $F_u(X; Y)$. \*

Cho $u_0 : X \to Y$ thuộc bao đóng của H trong $F_u(X; Y)$. Với mỗi lân cận đối xứng V của Y, tồn tại một ánh xạ $u \in H$ sao cho $(u_0(x), u(x)) \in V$ với mọi $x \in X$; mặt khác, theo giả thiết có một tập $M \in \mathfrak{T}$ sao cho $(u(x), u(x')) \in V$ bất cứ khi nào $x$ và $x'$ thuộc M. Vì $(u_0(x), u(x)) \in V$ và $(u_0(x'), u(x')) \in V$, suy ra $(u_0(x), u_0(x')) \in V$ bất cứ khi nào $x$ và $x'$ thuộc M, và do đó $u_0(\mathfrak{T})$ là một cơ sở Cauchy trên Y.

#### Hệ quả 1 {#top-x-s1-prop-8-cor-1 .statement}

*Cho X là một không gian tôpô và Y là một không gian đều. Tập các ánh xạ của X vào Y liên tục tại một điểm $x_0 \in X$ là đóng trong $F_u(X; U)$. \*

Nếu V là bộ lọc lân cận của $x_0$ trong X, thì $u(x_0)$ là một điểm tụ của $u(V)$; do đó $u$ liên tục tại $x_0$ khi và chỉ khi $u(V)$ là một cơ sở Cauchy trên Y (Chương II, § 3, no. 2, Mệnh đề 5, Hệ quả 2).

#### Hệ quả 2 {#top-x-s1-prop-8-cor-2 .statement}

*Cho X, L là hai tập hợp được lọc bởi các bộ lọc $\mathfrak{T}, \mathfrak{G}$ tương ứng, và Y là một không gian đều đầy đủ. Với mỗi $\lambda \in L$, cho $u_\lambda$ là một ánh xạ của X vào Y. Giả sử rằng (i) họ $(u_\lambda)_{\lambda \in L}$ hội tụ đều trong X (theo bộ lọc $\mathfrak{G}$) tới một ánh xạ $v : X \to Y$; (ii) với mỗi $\lambda \in L$, $u_\lambda$ có một giới hạn $y_\lambda$ theo bộ lọc $\mathfrak{T}$. Trong những điều kiện này, v có một giới hạn theo $\mathfrak{T}$, và mọi giới hạn của v theo $\mathfrak{T}$ là một giới hạn của họ $(y_\lambda)_{\lambda \in L}$ theo $\mathfrak{G}$. \*

Vì v nằm trong bao đóng của tập hợp các $u_\lambda$ trong $F_u(X; Y)$, nên $v(\mathfrak{T})$ là một cơ sở Cauchy trên Y do Mệnh đề 8; điều đó cho thấy v có một giới hạn y theo $\mathfrak{T}$ vì Y đầy đủ. Cho

X' = X \cup \{ \omega \} là không gian tôpô liên kết với bộ lọc $\mathcal{F}$ (Chương I, § 6, no. 5), và mở rộng $u_\lambda$ (hay $v$) thành một ánh xạ $\bar{u}_\lambda$ (hay $\bar{v}$) từ $X'$ vào $Y$ bằng cách đặt $\bar{u}_\lambda(\omega) = y_\lambda$ [hay $\bar{v}(\omega) = y$]. Khi đó các ánh xạ $\bar{u}_\lambda, \bar{v}$ liên tục trên $X'$, và $\bar{u}_\lambda$ hội tụ đều trong $X$ đến $\bar{v}$ đối với $\mathcal{G}$; vì $X$ trù mật trong $X'$, Hệ quả của Mệnh đề 6 cho thấy rằng $\bar{u}_\lambda$ hội tụ đều trong $X'$ đến $\bar{v}$, và đặc biệt là $y = \lim_{\mathcal{G}} y_\lambda$.

#### Định lý 2 {#top-x-s1-thm-2 .statement}

*Cho $X$ là một không gian tôpô, $Y$ là một không gian đều. Khi đó tập $C(X; Y)$ gồm các ánh xạ liên tục từ $X$ vào $Y$ là một tập con đóng của không gian $F(X; Y)$ được trang bị tôpô của sự hội tụ đều.*

Đối với mỗi $x \in X$, tập các ánh xạ từ $X$ vào $Y$ liên tục tại $x$ là đóng trong $F_u(X; Y)$ (Mệnh đề 8, Hệ quả 1); do đó giao $C(X; Y)$ của các tập này cũng đóng.

Kết quả này có thể diễn đạt dưới dạng rằng *giới hạn đều của các hàm liên tục là liên tục*.

#### Hệ quả 1 {#top-x-s1-thm-2-cor-1 .statement}

*Nếu $Y$ là một không gian đều đầy đủ, thì $C_u(X; Y)$ đầy đủ.*

Vì, theo Định lý 2, $C_u(X; Y)$ là một không gian con đều đóng của không gian đều $F_u(X; Y)$, mà theo Định lý 1 của no. 5 thì đầy đủ.

#### Hệ quả 2 {#top-x-s1-thm-2-cor-2 .statement}

*Cho $X$ là một không gian tôpô, $\mathcal{S}$ là một tập con các tập con của $X$, và $Y$ là một không gian đều. Kí hiệu $\tilde{C}_\mathcal{S}(X; Y)$ là tập mọi ánh xạ từ $X$ vào $Y$ sao cho hạn chế của chúng trên từng tập của $\mathcal{S}$ đều liên tục. Khi đó $\tilde{C}_\mathcal{S}(X; Y)$ là một không gian con đóng của không gian đều $F_\mathcal{S}(X; Y)$ và đầy đủ nếu $Y$ đầy đủ.*

Giả sử $u$ nằm trong bao đóng của $\tilde{C}_\mathcal{S}(X; Y)$ trong $F_\mathcal{S}(X; Y)$; khi đó (no. 2), với mỗi $A \in \mathcal{S}$, $u|A$ nằm trong bao đóng của $C(A; Y)$ trong $F_u(A; Y)$, và do đó liên tục theo Định lý 2.

#### Hệ quả 3 {#top-x-s1-thm-2-cor-3 .statement}

*Cho $X$ là một không gian tôpô, hoặc mêtric hóa được hoặc cục bộ compact, và cho $Y$ là một không gian đều. Khi đó $C(X; Y)$ là đóng trong không gian đều $F_c(X; Y)$; nếu thêm nữa $Y$ là đầy đủ, thì không gian đều $C_c(X; Y)$ là đầy đủ.*

Theo Hệ quả 2, chỉ cần chứng minh rằng, nếu lấy $\mathcal{S}$ là tập hợp các tập con compact của $X$, thì ta có $\tilde{C}_\mathcal{S}(X; Y) = C(X; Y)$ trong cả hai trường hợp đang xét. Điều này hiển nhiên nếu $X$ là cục bộ compact. Nếu $X$ là mêtric hóa được, và $u : X \to Y$ là một ánh xạ mà hạn chế của nó lên mọi tập con compact của $X$ là liên tục, thì với mỗi $x \in X$ và mỗi dãy $(z_n)$ các điểm của $X$ hội tụ đến $x$, ta có $u(x) = \lim_{n \to \infty} u(z_n)$, do đó $u$ liên tục tại $x$ (Chương IX, § 2, no. 6, Mệnh đề 10).

Hãy lưu ý rằng lập luận trên áp dụng bất cứ khi nào mỗi điểm của $X$ có một *hệ cơ sở đếm được* các lân cận.

#### Nhận xét 1 {#top-x-s1-n6-rem-1 .statement}

Nói chung, tập $\mathcal{C}(X; Y)$ không đóng trong $\mathcal{F}(X; Y)$ đối với tôpô hội tụ *điểm một*: nói cách khác, một giới hạn điểm một của các hàm liên tục chưa chắc đã liên tục [Bài tập 5 a)].

#### Nhận xét 2 {#top-x-s1-n6-rem-2 .statement}

Một bộ lọc trên $\mathcal{C}(X; Y)$ có thể hội tụ *điểm một* tới một hàm *liên tục* mà không hội tụ đều tới hàm này.

Chẳng hạn, trên khoảng $I = [0, 1]$, hãy lấy $u_n$ là hàm giá trị thực bằng 0 khi $x = 0$ và $2/n \leq x \leq 1$, bằng 1 khi $x = 1/n$, và tuyến tính trên mỗi khoảng $[0, 1/n]$ và $[1/n, 2/n]$. Dãy $(u_n)$ hội tụ điểm một đến 0, nhưng không hội tụ đều đến 0 trong $I$ (xem Bài tập 6).

#### Nhận xét 3 {#top-x-s1-n6-rem-3 .statement}

Nếu $X$ là một không gian đều, một chứng minh tương tự như của Mệnh đề 8 cho thấy tập các ánh xạ *liên tục đều* từ $X$ vào $Y$ là *đóng* trong $\mathcal{F}_u(X; Y)$.

#### Nhận xét 4 {#top-x-s1-n6-rem-4 .statement}

Giả sử rằng không gian đều $Y$ mang một luật hợp thành giao hoán và kết hợp, được viết theo phép cộng, sao cho ánh xạ $(y, y') \to y + y'$ là liên tục trên $Y \times Y$. Khi đó, nếu $(u_n)$ là một dãy các ánh xạ liên tục từ $X$ vào $Y$ sao cho chuỗi có số hạng tổng quát là $u_n$ *hội tụ đều* trong $X$, thì tổng của chuỗi là liên tục trên $X$.

Chúng tôi để độc giả phát biểu kết quả tương ứng cho các họ *cộng được đều* (no. 1, Nhận xét 5) của các ánh xạ liên tục.

#### Mệnh đề 9 {#top-x-s1-prop-9 .statement}

*Cho $X$ là một không gian tôpô, $Y$ là một không gian đều. Khi đó ánh xạ $(f, x) \to f(x)$ từ $\mathcal{C}_u(X; Y) \times X$ vào $Y$ là liên tục.*

Cho $f_0 : X \to Y$ là một ánh xạ liên tục, cho $x_0$ là một điểm của $X$ và cho $V$ là một bao lân cận của $Y$. Tập hợp $T$ gồm các ánh xạ liên tục $f : X \to Y$ sao cho $(f(x), f(x_0)) \in V$ với mọi $x \in X$ là một lân cận của $f_0$ trong $\mathcal{C}_u(X; Y)$. Mặt khác, vì $f_0$ liên tục, nên tồn tại một lân cận $U$ của $x_0$ trong $X$ sao cho $(f_0(x), f_0(x_0)) \in V$ với mọi $x \in U$. Do đó ta có $(f(x), f(x_0)) \in V$ mỗi khi $(f, x) \in T \times U$, và kết quả được chứng minh.

### Bài tập {#top-x-s1-exercises}

Xem [các bài tập cho § 1](exercises/s1/).
