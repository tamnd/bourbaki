---
book: ens
book_title: Theory of Sets
chapter: II
chapter_title: THEORY OF SETS
section: 4
section_title: Union and intersection of a family of sets
lang: vi
source: ens-i-iv
source_edition: 2004, Springer
book_pages: 90-101, 125-126
pdf_pages: 0097-0108, 0132-0133
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF THE UNION AND THE INTERSECTION OF A FAMILY OF SETS
      page: 90
      pdf_page: 97
    - "no": 2
      title: PROPERTIES OF UNION AND INTERSECTION
      page: 93
      pdf_page: 100
    - "no": 3
      title: IMAGES OF A UNION AND AN INTERSECTION
      page: 94
      pdf_page: 101
    - "no": 4
      title: COMPLEMENTS OF UNIONS AND INTERSECTIONS
      page: 96
      pdf_page: 103
    - "no": 5
      title: UNION AND INTERSECTION OF TWO SETS
      page: 96
      pdf_page: 103
    - "no": 6
      title: COVERINGS
      page: 98
      pdf_page: 105
    - "no": 7
      title: PARTITIONS
      page: 99
      pdf_page: 106
    - "no": 8
      title: SUM OF A FAMILY OF SETS
      page: 100
      pdf_page: 107
statements: 22
exercises: 8
content_sha256: b5ada03a0f6d1b8274837838265522e7cba7bbe70c20b75fd998e0b025e32044
translated_from: content/en/ens/II/04_s4_union_and_intersection_of_a_family_of.md
source_content_sha256: fa664243f694205d57fee07324e9530b13d7e92d6d61e5dd3cf3c072e6ee2fa0
translation_model: gpt-5.4
translation_run: translate-vi-2bfc6108
glossary_version: 29
glossary_terms_sha256: c4a0b7c86d1793f7b6ede43b3c4857e23d29ab1b07199dcffcae838f438b7841
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 4. HỢP VÀ GIAO CỦA MỘT HỌ CÁC TẬP HỢP

### 1. ĐỊNH NGHĨA CỦA HỢP VÀ GIAO CỦA MỘT HỌ CÁC TẬP HỢP

Cho X là một họ (§3, số 4) và I là tập chỉ số của nó. Để giúp cho cách giải thích trực quan về điều sau đây, ta sẽ gọi X là một *họ các tập hợp*. Nếu $(\mathrm{X}, \mathrm{I}, \mathfrak{G})$ là một *họ các tập con của một tập hợp* E (nghĩa là một họ mà đích $\mathfrak{G}$ của nó có tính chất là quan hệ $\mathrm{Y} \in \mathfrak{G}$ kéo theo $\mathrm{Y} \subset \mathrm{E}$), ta sẽ ký hiệu họ đó bởi $(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}(\mathrm{X}_\iota \in \mathfrak{G})$ hoặc đơn giản bởi $(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$ (§3, số 6); lạm dụng ký hiệu, ta sẽ ký hiệu mọi họ các tập hợp có I làm tập chỉ số bởi $(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$.

¶ Vì quan hệ $(\forall x)((\iota \in \mathrm{I}$ và $x \in \mathrm{X}_\iota) \Rightarrow (x \in \mathrm{X}_\iota))$ là đúng, nên từ S5 (Chương I, §4, số 2.) suy ra rằng quan hệ

$$(\forall \iota)(\exists \mathrm{Z})(\forall x)((\iota \in \mathrm{I} \text{ và } x \in \mathrm{X}_\iota) \Rightarrow (x \in \mathrm{Z}))$$

là đúng. Theo lược đồ S8 (§1, số 6), quan hệ $(\exists \iota)(\iota \in \mathrm{I}$ và $x \in \mathrm{X}_\iota)$ là *xác định tập theo $x$*.

#### Định nghĩa 1 {#ens-ii-s4-def-1 .statement tag=03I1}

*Cho $(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$ là một họ các tập hợp* (hoặc *một họ các tập con của một tập hợp* E). *Tập hợp $\mathcal{E}_x((\exists \iota)(\iota \in \mathrm{I}$ và $x \in \mathrm{X}_\iota))$, nghĩa là tập hợp mọi $x$*

*thuộc ít nhất một tập hợp của họ $(X_l)_{l\in I}$, được gọi là hợp của họ, và được ký hiệu bởi*
$$\bigcup_{l\in I}X_l,$$ [^1]

Nếu $(X_l)_{l\in I}$ là một họ các tập con của một tập hợp $E$, thì hợp của nó là một tập con của $E$; lưu ý rằng nó không phụ thuộc vào $E$, cũng không phụ thuộc vào đích $\mathcal{G}$ của ánh xạ $l\to X_l$.

Hiển nhiên là nếu $I=\varnothing$, ta có $\displaystyle\bigcup_{l\in I}X_l=\varnothing$, vì khi đó quan hệ $(\exists l)(l\in I\text{ và }x\in X_l)$ là sai.

¶ Giả sử bây giờ rằng $I\neq\varnothing$. Nếu $\alpha$ là một phần tử của $I$, quan hệ
$$ (\forall l)((l\in I)\Longrightarrow(x\in X_l)) $$
suy ra $x\in X_\alpha$ và do đó, theo C52 (§1, số 6), quan hệ này là *xác định tập theo $x$.*

#### Định nghĩa 2 {#ens-ii-s4-def-2 .statement tag=03PT}

*Cho $(X_l)_{l\in I}$ là một họ các tập hợp có tập chỉ số $I$ không rỗng. Tập $\mathcal{E}_x((\forall l)((l\in I)\Longrightarrow(x\in X_l)))$, tức là tập hợp mọi $x$ thuộc mọi tập hợp của họ $(X_l)_{l\in I}$, được gọi là giao của họ và được ký hiệu bởi*
$$\bigcap_{l\in I}X_l.$$

Nếu $I=\varnothing$, thì quan hệ $(\forall l)((l\in I)\Longrightarrow(x\in X_l))$ không xác định tập theo $x$; thật vậy, đó là một quan hệ đúng và không tồn tại tập hợp $Y$ nào sao cho $x\in Y$ là một quan hệ đúng, bởi vì khi đó $Y$ sẽ là tập hợp của mọi đối tượng (xem §1, no. 7, chú ý).

Nếu $(X_l)_{l\in I}$ là một họ các tập con của một tập hợp $E$ và nếu $I\neq\varnothing$, thì quan hệ “$x\in E$ and $(\forall l)((l\in I)\Longrightarrow(x\in X_l))$” là tương đương với
$$ (\forall l)((l\in I)\Longrightarrow(x\in X_l)); $$
do đó nó xác định tập theo $x$, và tập hợp mọi $x$ thỏa mãn quan hệ này bằng $\displaystyle\bigcap_{l\in I}X_l$. Nếu $I=\varnothing$, thì quan hệ “$x\in E$ and $(\forall l)((l\in I)\Longrightarrow(x\in X_l))$” là tương đương với $x\in E$; vì thế nó xác định tập theo $x$, và tập hợp mọi $x$ thỏa mãn quan hệ này là $E$. Do đó ta có thể phát biểu định nghĩa sau :

#### Định nghĩa 3 {#ens-ii-s4-def-3 .statement tag=03PU}

*Cho $(X_l)_{l\in I}$ là một họ các tập hợp con của một tập hợp $E$. Tập hợp*
$$\mathcal{E}_x\left(x\in E\text{ và }(\forall l)((l\in I)\Longrightarrow(x\in X_l))\right),$$

*nói cách khác, tập hợp của mọi $x$ thuộc* E *và thuộc mỗi tập hợp* $X_\iota$, *được gọi là giao của họ và được ký hiệu bởi* $\bigcap\limits_{\iota \in I} X_\iota$.

Vì thế đối với một họ $(X_\iota)_{\iota \in \emptyset}$ các tập hợp con của E ta có

$$\bigcap_{\iota \in \emptyset} X_\iota = E.$$

Nhưng đối với một họ $(X_\iota)_{\iota \in I}$ các tập hợp con của E mà tập hợp chỉ số không rỗng, giao $\bigcap\limits_{\iota \in I} X_\iota$ không phụ thuộc vào E cũng không phụ thuộc vào đối tượng đích của $\iota \rightarrow X_\iota$; và điều này biện minh cho việc dùng cùng một ký hiệu trong các Định nghĩa 2 và 3.

#### Mệnh đề 1 {#ens-ii-s4-prop-1 .statement tag=03PV}

*Cho* $(X_\iota)_{\iota \in I}$ *là một họ các tập hợp, và cho $f$ là một ánh xạ của một tập hợp* K *lên* I. *Khi đó*

$$\bigcup_{\varkappa \in K} X_{f(\varkappa)} = \bigcup_{\iota \in I} X_\iota,$$

*và, nếu* $I \neq \emptyset$,

$$\bigcap_{\varkappa \in K} X_{f(\varkappa)} = \bigcap_{\iota \in I} X_\iota.$$

Cho $x$ là một phần tử của $\bigcap\limits_{\iota \in I} X_\iota$. Tồn tại một chỉ số $\iota \in I$ sao cho $x \in X_\iota$. Vì $f\langle K \rangle = I$, tồn tại một chỉ số $\varkappa \in K$ sao cho $\iota = f(\varkappa)$, do đó $x \in X_{f(\varkappa)}$ và do đó

$$x \in \bigcup_{\varkappa \in K} X_{f(\varkappa)}.$$

Ngược lại, nếu $x \in \bigcup\limits_{\varkappa \in K} X_{f(\varkappa)}$, thì tồn tại $\varkappa \in K$ sao cho $x \in X_{f(\varkappa)}$, và vì thế, do $f(\varkappa) \in I$, ta có $x \in \bigcup\limits_{\iota \in I} X_\iota$. Vậy nên

$$\bigcup_{\varkappa \in K} X_{f(\varkappa)} = \bigcup_{\iota \in I} X_\iota.$$

¶ Bây giờ giả sử rằng $I \neq \emptyset$, và cho $x$ là một phần tử của $\bigcap\limits_{\iota \in I} X_\iota$. Với mỗi phần tử $\varkappa$ của K, ta có $f(\varkappa) \in I$, nên $x \in X_{f(\varkappa)}$, và vì thế

$$x \in \bigcap_{\varkappa \in K} X_{f(\varkappa)}.$$

Ngược lại, cho $x$ là một phần tử của $\bigcap\limits_{\varkappa \in K} X_{f(\varkappa)}$. Nếu $\iota$ là một phần tử bất kỳ của I, thì tồn tại một phần tử $\varkappa$ của K sao cho $\iota = f(\varkappa)$, do đó $x \in X_\iota$ và

do đó $x \in \bigcap_{\iota \in I} X_\iota$. Vậy

$$\bigcap_{\varkappa \in K} X_{f(\varkappa)} = \bigcap_{\iota \in I} X_\iota.$$

Đối với các họ tập hợp con của một tập hợp cho trước, rõ ràng là phần thứ hai của Mệnh đề 1 vẫn đúng mà không cần hạn chế $I \neq \emptyset$.

#### Hệ quả {#ens-ii-s4-n1-cor-1 .statement tag=03I2}

*Cho* $(X_\iota)_{\iota \in I}$ *là một họ tập hợp sao cho* $X_\iota = X_\varkappa$ *với mỗi cặp chỉ số* $(\iota, \varkappa)$. *Khi đó với mỗi* $\alpha \in I$ *ta có*

$$\bigcup_{\iota \in I} X_\iota = X_\alpha, \qquad \textit{và (nếu } I \neq \emptyset) \qquad \bigcap_{\iota \in I} X_\iota = X_\alpha.$$

Áp dụng Mệnh đề 1 cho ánh xạ hằng $\iota \to \alpha$ từ I lên $\{\alpha\}$.

#### Định nghĩa 4 {#ens-ii-s4-def-4 .statement tag=03I3}

*Cho* $\mathfrak{F}$ *là một tập hợp các tập hợp và cho* $\Phi$ *là họ các tập hợp được định nghĩa bởi ánh xạ đồng nhất của* $\mathfrak{F}$. *Hợp của các tập hợp thuộc* $\Phi$ *và (nếu* $\mathfrak{F}$ *không rỗng) giao của các tập hợp thuộc* $\Phi$ *được gọi, tương ứng, là* hợp *và* giao *của các tập hợp thuộc* $\mathfrak{F}$, *và được ký hiệu bởi* $\bigcup_{X \in \mathfrak{F}} X$ *và* $\bigcap_{X \in \mathfrak{F}} X$.

Từ Mệnh đề 1 suy ra ngay lập tức rằng nếu $(X_\iota)_{\iota \in I}$ là một họ các tập hợp, thì hợp và (nếu $I \neq \emptyset$) giao của họ này lần lượt bằng hợp và giao của các tập hợp của tập hợp các phần tử của họ này.

### 2. TÍNH CHẤT CỦA HỢP VÀ GIAO

Nếu $(X_\iota)_{\iota \in I}$ và $(Y_\iota)_{\iota \in I}$ là các họ tập hợp có cùng tập chỉ số I, và nếu $Y_\iota \subset X_\iota$ với mọi $\iota \in I$, thì hiển nhiên là

$$\bigcup_{\iota \in I} Y_\iota \subset \bigcup_{\iota \in I} X_\iota, \qquad \text{và (nếu } I \neq \emptyset) \qquad \bigcap_{\iota \in I} Y_\iota \subset \bigcap_{\iota \in I} X_\iota.$$

¶ Cho $(X_\iota)_{\iota \in I}$ là một họ tập hợp. Nếu $J \subset I$, ta có

$$\bigcup_{\iota \in J} X_\iota \subset \bigcup_{\iota \in I} X_\iota, \qquad \text{và (nếu } J \neq \emptyset) \qquad \bigcap_{\iota \in J} X_\iota \supset \bigcap_{\iota \in I} X_\iota.$$

#### Mệnh đề 2 {#ens-ii-s4-prop-2 .statement tag=03I4}

*Cho* $(X_\iota)_{\iota \in I}$ *là một họ tập hợp mà tập hợp chỉ số* I *là hợp của một họ* $(J_\lambda)_{\lambda \in L}$ *gồm các tập hợp. Khi đó*

$$\bigcup_{\iota \in I} X_\iota = \bigcup_{\lambda \in L} \left( \bigcup_{\iota \in J_\lambda} X_\iota \right),$$

*và* (*nếu* $L \neq \emptyset$ và $J_\lambda \neq \emptyset$ *với mọi* $\lambda \in L$)

$$\bigcap_{\iota \in I} X_\iota = \bigcap_{\lambda \in L} \left( \bigcap_{\iota \in J_\lambda} X_\iota \right)$$

("tính kết hợp" của hợp và giao).

Cho $x$ là một phần tử của $\bigcup_{\iota \in I} X_\iota$. Tồn tại một chỉ số $\iota \in I$ sao cho $x \in X_\iota$. Vì I là hợp của họ $(J_\lambda)_{\lambda \in L}$, nên tồn tại một chỉ số $\lambda \in L$ sao cho $\iota \in J_\lambda$, do đó $x \in \bigcup_{\iota \in J_\lambda} X_\iota$, và do đó

$$x \in \bigcup_{\lambda \in L} \left( \bigcup_{\iota \in J_\lambda} X_\iota \right).$$

Ngược lại, cho $x$ là một phần tử của tập hợp này. Tồn tại một chỉ số $\lambda \in L$ sao cho $x \in \bigcup_{\iota \in J_\lambda} X_\iota$, do đó tồn tại một chỉ số $\iota \in J_\lambda$ (và vì thế $\iota \in I$) sao cho $x \in X_\iota$; suy ra rằng

$$x \in \bigcup_{\iota \in I} X_\iota.$$

Bây giờ giả sử rằng $L \neq \emptyset$ và $J_\lambda \neq \emptyset$ với mỗi $\lambda \in L$. Khi đó $I \neq \emptyset$. Cho $x$ là một phần tử của $\bigcap_{\iota \in I} X_\iota$. Nếu $\lambda \in L$, ta có $x \in X_\iota$ với mỗi $\iota \in J_\lambda$ (vì $J_\lambda \subset I$), do đó $x \in \bigcap_{\iota \in J_\lambda} X_\iota$. Vì điều bao hàm sau cùng này đúng với mọi $\lambda \in L$, $x$ thuộc về $\bigcap_{\lambda \in L} \left( \bigcap_{\iota \in J_\lambda} X_\iota \right)$. Ngược lại, cho $x$ là một phần tử của tập hợp sau này, và cho $\iota$ là một phần tử bất kỳ của I. Tồn tại $\lambda \in L$ sao cho $\iota \in J_\lambda$; vì $x \in \bigcap_{\iota \in J_\lambda} X_\iota$, ta có $x \in X_\iota$, điều này đúng với mọi $\iota \in I$. Vậy $x \in \bigcap_{\iota \in I} X_\iota$. Điều này hoàn tất chứng minh.

Đối với các họ tập con của một tập hợp đã cho, phần thứ hai của Mệnh đề 2 vẫn đúng mà không có hạn chế nào đối với L và $J_\lambda$.

### 3. ẢNH CỦA HỢP VÀ GIAO

#### Mệnh đề 3 {#ens-ii-s4-prop-3 .statement tag=03I5}

*Cho* $(X_\iota)_{\iota \in I}$ *là một họ các tập con của tập hợp* A, *và cho* $\Gamma$ *là một sự tương ứng giữa* A *và* B. *Khi đó*

$$\Gamma \left\langle \bigcup_{\iota \in I} X_\iota \right\rangle = \bigcup_{\iota \in I} \Gamma \langle X_\iota \rangle, \qquad \Gamma \left\langle \bigcap_{\iota \in I} X_\iota \right\rangle \subset \bigcap_{\iota \in I} \Gamma \langle X_\iota \rangle.$$

Quan hệ $(\exists x)\left(x \in \bigcup_{\iota \in I} X_\iota \text{ và } y \in \Gamma(x)\right)$ tương đương với

$$(\exists x)(\exists \iota)(\iota \in I \text{ và } x \in X_\iota \text{ và } y \in \Gamma(x)),$$

do đó tương đương với $(\exists \iota)(\iota \in I$ và $y \in \Gamma\langle X_\iota \rangle)$, do đó tương đương với $y \in \bigcup_{\iota \in I} \Gamma\langle X_\iota \rangle$; điều này chứng minh công thức thứ nhất. Đối với công thức thứ hai, ta có $\bigcap_{\iota \in I} X_\iota \subset X_\iota$ với mọi $\iota \in I$, do đó (§3, Mệnh đề 2)

$$\Gamma\left\langle \bigcap_{\iota \in I} X_\iota \right\rangle \subset \Gamma\langle X_\iota \rangle,$$

và do đó

$$\Gamma\left\langle \bigcap_{\iota \in I} X_\iota \right\rangle \subset \bigcap_{\iota \in I} \Gamma\langle X_\iota \rangle.$$

¶ Nếu $\Gamma$ là một sự tương ứng tùy ý (và đặc biệt là một hàm tùy ý), công thức

$$\Gamma\left\langle \bigcap_{\iota \in I} X_\iota \right\rangle = \bigcap_{\iota \in I} \Gamma\langle X_\iota \rangle$$

thường là *sai*.

\* Ví dụ, trong mặt phẳng $\mathbf{R}^2$, các phép chiếu thứ nhất của các đường thẳng $y = x$ và $y = x + 1$ đều bằng $\mathbf{R}$, nhưng giao của các đường thẳng ấy là rỗng, và do đó phép chiếu thứ nhất của giao này cũng rỗng [^2]. \*

Tuy nhiên, ta có kết quả quan trọng sau :

#### Mệnh đề 4 {#ens-ii-s4-prop-4 .statement tag=03I6}

*Cho $f$ là một ánh xạ từ* A *vào* B *và cho* $(Y_\iota)_{\iota \in I}$ *là một họ các tập con của* B. *Khi đó* $\overset{-1}{f}\left\langle \bigcap_{\iota \in I} Y_\iota \right\rangle = \bigcap_{\iota \in I} \overset{-1}{f}\langle Y_\iota \rangle.$

Để chứng minh điều này, lấy $x$ là một phần tử của $\bigcap_{\iota \in I} \overset{-1}{f}\langle Y_\iota \rangle$. Ta có $f(x) \in Y_\iota$ với mọi $\iota \in I$, do đó $f(x) \in \bigcap_{\iota \in I} Y_\iota$, và vì thế

$$x \in \overset{-1}{f}\left\langle \bigcap_{\iota \in I} Y_\iota \right\rangle.$$

Vậy $\bigcap_{\iota \in I} \overset{-1}{f}(Y_\iota) \subset \overset{-1}{f}\left\langle \bigcap_{\iota \in I} Y_\iota \right\rangle$; quan hệ này, cùng với Mệnh đề 3, cho kết quả.

#### Hệ quả {#ens-ii-s4-n3-cor-1 .statement tag=03I7}

*Nếu $f$ là một đơn ánh từ* A *vào* B *và nếu* $(X_\iota)_{\iota \in I}$ *là một họ các tập con của* A *mà tập chỉ số* I *không rỗng, thì* $f\left\langle \bigcap_{\iota \in I} X_\iota \right\rangle = \bigcap_{\iota \in I} f\langle X_\iota \rangle$.

Thật vậy, ta có thể viết $f = i \circ g$, trong đó $i$ là đơn ánh chính tắc của $f\langle A \rangle$ vào B và $g$ là một song ánh của A lên $f\langle A \rangle$. Nếu $h$ ký hiệu ánh xạ nghịch đảo của $g$, thì ta có $f\langle X \rangle = \overset{-1}{h}\langle X \rangle$ với mọi tập con X của A, và do đó ta quy về Mệnh đề 4.

### 4. PHẦN BÙ CỦA HỢP VÀ GIAO

#### Mệnh đề 5 {#ens-ii-s4-prop-5 .statement tag=03I8}

*Với mọi họ* $(X_\iota)_{\iota \in I}$ *các tập con của một tập hợp* E, *ta có*

$$\complement_E\left(\bigcup_{\iota \in I} X_\iota\right) = \bigcap_{\iota \in I} (\complement_E X_\iota), \qquad \complement_E\left(\bigcap_{\iota \in I} X_\iota\right) = \bigcup_{\iota \in I} (\complement_E X_\iota).$$

Cho $x \in \complement_E\left(\bigcup_{\iota \in I} X_\iota\right)$. Khi đó $x \in E$ và, với mọi $\iota \in I$, $x \notin X_\iota$, nên $x \in \complement_E X_\iota$; do đó

$$x \in \bigcap_{\iota \in I} (\complement_E X_\iota).$$

Ngược lại, cho $x$ là một phần tử của $\bigcap_{\iota \in I} (\complement_E X_\iota)$; theo định nghĩa của giao ta có $x \in E$. Hơn nữa, nếu ta có $x \in \bigcup_{\iota \in I} X_\iota$, thì sẽ tồn tại một chỉ số $\varkappa \in I$ sao cho $x \in X_\varkappa$, điều này mâu thuẫn với giả thiết $x \in \bigcap_{\iota \in I} (\complement_E X_\iota)$; vì thế

$$x \in \complement_E\left(\bigcup_{\iota \in I} X_\iota\right).$$

Điều này chứng minh công thức thứ nhất; công thức thứ hai là một hệ quả ngay lập tức, xét theo quan hệ $\complement_E(\complement_E X) = X$ với mọi tập con X của E.

### 5. HỢP VÀ GIAO CỦA HAI TẬP HỢP

Nếu A, B là các tập hợp, ta viết

$$A \cup B = \bigcup_{X \in \{A, B\}} X, \qquad A \cap B = \bigcap_{X \in \{A, B\}} X.$$

Rõ ràng $A \cup B$ là tập hợp của mọi đối tượng thuộc $A$ hoặc thuộc $B$ (hoặc có thể thuộc cả hai), còn $A \cap B$ là tập hợp của mọi đối tượng đồng thời thuộc $A$ và $B$. Đặc biệt, $\{x, y\} = \{x\} \cup \{y\}$.

¶ Đặt $\{x, y, z\} = \{x, y\} \cup \{z\}$. Tập hợp $\{x, y, z\}$ là tập hợp mà các phần tử duy nhất của nó là $x$, $y$ và $z$. Tương tự, ta viết

$$\{x, y, z, t\} = \{x, y, z\} \cup \{t\},$$

và cứ tiếp tục như vậy.

¶ Nếu bây giờ $A$, $B$, $C$, $D$ là các tập hợp, ta viết

$$A \cup B \cup C = \bigcup_{X \in \{A,\, B,\, C\}} X, \qquad A \cap B \cap C = \bigcap_{X \in \{A,\, B,\, C\}} X;$$

$$A \cup B \cup C \cup D = \bigcup_{X \in \{A,\, B,\, C,\, D\}} X, \qquad A \cap B \cap C \cap D = \bigcap_{X \in \{A,\, B,\, C,\, D\}} X;$$

và cứ tiếp tục như vậy.

¶ Cho $A, B, C$ là các tập hợp. Từ các Mệnh đề 1 và 2 ta suy ra các công thức

$$A \cup B = B \cup A, \qquad A \cap B = B \cap A,$$
$$A \cup (B \cup C) = (A \cup B) \cup C = A \cup B \cup C,$$
$$A \cap (B \cap C) = (A \cap B) \cap C = A \cap B \cap C.$$

Các công thức này cũng là những hệ quả ngay lập tức của các định lý được phát biểu trong tiêu chuẩn C24 (chương I, §3, no. 5). Tương tự, người ta chứng minh các công thức

$$A \cup (B \cap C) = (A \cup B) \cap (A \cup C), \qquad A \cap (B \cup C) = (A \cap B) \cup (A \cap C)$$

("tính phân phối" của hợp đối với giao và của giao đối với hợp; xem §5, no. 6).

¶ Quan hệ $A \subset B$ tương đương với $A \cup B = B$ và với $A \cap B = A$. Nếu $A$ và $B$ là các tập con của một tập hợp $E$, ta suy ra từ Mệnh đề 5 (hoặc từ tiêu chuẩn C24) các công thức

$$\complement_E(A \cup B) = (\complement_E A) \cap (\complement_E B), \qquad \complement_E(A \cap B) = (\complement_E A) \cup (\complement_E B);$$

hơn nữa, ta có

$$A \cup (\complement_E A) = E, \qquad A \cap (\complement_E A) = \emptyset.$$

¶ Nếu $\Gamma$ là một sự tương ứng giữa $E$ và $F$, và nếu $A$, $B$ là các tập con của $E$, thì từ Mệnh đề 3 suy ra rằng

$$\Gamma\langle A \cup B \rangle = \Gamma\langle A \rangle \cup \Gamma\langle B \rangle, \qquad \Gamma\langle A \cap B \rangle \subset \Gamma\langle A \rangle \cap \Gamma\langle B \rangle,$$

và rằng, nếu $f$ là một ánh xạ từ F vào E,

$$\overset{-1}{f}\langle \mathrm{A} \cap \mathrm{B} \rangle = \overset{-1}{f}\langle \mathrm{A} \rangle \cap \overset{-1}{f}\langle \mathrm{B} \rangle$$

theo Mệnh đề 4.

¶ Chúng tôi cũng ghi lại Mệnh đề sau về các phần bù :

#### Mệnh đề 6 {#ens-ii-s4-prop-6 .statement tag=03PW}

*Cho $f$ là một ánh xạ từ* A *vào* B. *Với mọi tập con* Y *của* B, *ta có*

$$\overset{-1}{f}\langle \mathrm{B} - \mathrm{Y} \rangle = \overset{-1}{f}\langle \mathrm{B} \rangle - \overset{-1}{f}\langle \mathrm{Y} \rangle.$$

Thật vậy, $x$ thuộc $\overset{-1}{f}\langle \mathrm{B} - \mathrm{Y} \rangle$ khi và chỉ khi $f(x)$ thuộc B nhưng không thuộc Y, nghĩa là, khi và chỉ khi $x$ thuộc $\overset{-1}{f}\ \langle \mathrm{B} \rangle$ nhưng không thuộc $\overset{-1}{f}\ \langle \mathrm{Y} \rangle$.

#### Hệ quả {#ens-ii-s4-n5-cor-1 .statement tag=03PX}

*Cho $f$ là một đơn ánh từ* A *vào* B. *Với mọi tập con* X *của* A, *ta có $f\langle \mathrm{A} - \mathrm{X} \rangle = f\langle \mathrm{A} \rangle - f\langle \mathrm{X} \rangle$.*

Viết $f = i \circ g$, trong đó $i$ là đơn ánh chính tắc của $f\langle \mathrm{A} \rangle$ vào B, ta rút gọn Hệ quả về Mệnh đề 6 áp dụng cho $\overset{-1}{g}$.

¶ Giao $\mathrm{X} \cap \mathrm{A}$ đôi khi được gọi là *vết* của X trên A. Nếu $\mathfrak{F}$ là một họ các tập hợp, tập hợp các vết trên A của các tập hợp thuộc $\mathfrak{F}$ được gọi là *vết* của $\mathfrak{F}$ trên A.

### 6. PHỦ

#### Định nghĩa 5 {#ens-ii-s4-def-5 .statement tag=03PY}

*Một họ các tập hợp $(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$ được gọi là một phủ của một tập hợp* E *(hoặc phủ* E) *nếu $\mathrm{E} \subset \bigcup\limits_{\iota \in \mathrm{I}} \mathrm{X}_\iota$. Nếu $(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$ và $(\mathrm{Y}_\varkappa)_{\varkappa \in \mathrm{K}}$ là các phủ của* E, *thì phủ thứ hai được gọi là mịn hơn phủ thứ nhất (hoặc là một sự tinh luyện của phủ thứ nhất, hoặc tinh luyện phủ thứ nhất) nếu, với mỗi $\varkappa \in \mathrm{K}$, tồn tại $\iota \in \mathrm{I}$ sao cho*

$$\mathrm{Y}_\varkappa \subset \mathrm{X}_\iota.$$

Một tập hợp các tập hợp $\mathfrak{R}$ là một phủ của E nếu họ các tập hợp được định nghĩa bởi ánh xạ đồng nhất của $\mathfrak{R}$ là một phủ của E, nói cách khác, nếu $\mathrm{E} \subset \bigcup\limits_{\mathrm{X} \in \mathfrak{R}} \mathrm{X}$.

Nếu $\mathfrak{R}$, $\mathfrak{R}'$, $\mathfrak{R}''$ là ba phủ của E sao cho $\mathfrak{R}'$ tinh hơn $\mathfrak{R}$ và $\mathfrak{R}''$ tinh hơn $\mathfrak{R}'$, thì rõ ràng $\mathfrak{R}''$ tinh hơn $\mathfrak{R}$.

Cho $(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$ là một phủ của E. Nếu J là một tập con của I sao cho $(\mathrm{X}_\iota)_{\iota \in \mathrm{J}}$ vẫn còn là một phủ của E, thì phủ này rõ ràng tinh hơn $(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$.

¶ Cho $(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$ và $(\mathrm{Y}_\varkappa)_{\varkappa \in \mathrm{K}}$ là các phủ của tập hợp E. Khi đó họ các tập hợp $(\mathrm{X}_\iota \cap \mathrm{Y}_\varkappa)_{(\iota, \varkappa) \in \mathrm{I} \times \mathrm{K}}$ là một phủ của E. Thật vậy, nếu $x \in \mathrm{E}$, thì tồn tại các chỉ số $\iota \in \mathrm{I}$ và $\varkappa \in \mathrm{K}$ sao cho $x \in \mathrm{X}_\iota$ và $x \in \mathrm{Y}_\varkappa$, do đó $x \in \mathrm{X}_\iota \cap \mathrm{Y}_\varkappa$ Hơn nữa, hiển nhiên là phủ $(\mathrm{X}_\iota \cap \mathrm{Y}_\varkappa)_{(\iota, \varkappa) \in \mathrm{I} \times \mathrm{K}}$ tinh hơn từng

các phủ $(X_\iota)_{\iota \in I}$, $(Y_\varkappa)_{\varkappa \in K}$. Ngược lại, cho $(Z_\lambda)_{\lambda \in L}$ là một phủ của E tinh hơn mỗi phủ $(X_\iota)_{\iota \in I}$, $(Y_\varkappa)_{\varkappa \in K}$; nếu $\lambda \in L$ thì tồn tại các chỉ số $\iota \in I$ và $\varkappa \in K$ sao cho $Z_\lambda \subset X_\iota$ và $Z_\lambda \subset Y_\varkappa$, nên $Z_\lambda \subset X_\iota \cap Y_\varkappa$; do đó phủ $(Z_\lambda)_{\lambda \in L}$ là một sự làm mịn của

$$(X_\iota \cap Y_\varkappa)_{(\iota, \varkappa) \in I \times K}.$$

¶ Cho $(X_\iota)_{\iota \in I}$ là một phủ của tập hợp A, và cho $f$ là một ánh xạ của A *lên* một tập hợp B. Khi đó họ $(f\langle X_\iota \rangle)_{\iota \in I}$ là một phủ của B (Mệnh đề 3), được gọi là *ảnh theo* $f$ *của phủ* $(X_\iota)_{\iota \in I}$. Nếu $g$ là một ánh xạ của một tập hợp C vào tập hợp A, thì họ $(\overset{-1}{g}\langle X_\iota \rangle)_{\iota \in I}$ là một phủ của C, được gọi là *ảnh ngược theo* $g$ *của phủ* $(X_\iota)_{\iota \in I}$.
¶ Cho E và F là các tập hợp, cho $(X_\iota)_{\iota \in I}$ là một phủ của E, và cho $(Y_\varkappa)_{\varkappa \in K}$ là một phủ của F. Khi đó họ $(X_\iota \times Y_\varkappa)_{(\iota, \varkappa) \in I \times K}$ là một phủ của $E \times F$, được gọi là *tích* của các phủ $(X_\iota)_{\iota \in I}$ của E và $(Y_\varkappa)_{\varkappa \in K}$ của F.

#### Mệnh đề 7 {#ens-ii-s4-prop-7 .statement tag=03PZ}

(1) *Cho* E *là một tập hợp và* $(X_\iota)_{\iota \in I}$ *là một phủ của* E. *Nếu* $f$ *và* $g$ *là hai ánh xạ có tập xác định là* E *sao cho* $f$ *và* $g$ *trùng nhau trên* $E \cap X_\iota$ *với mọi* $\iota \in I$, *thì* $f$ *và* $g$ *trùng nhau trên* E.

(2) *Cho* $(X_\iota)_{\iota \in I}$ *là một họ tập hợp và cho* $(f_\iota)_{\iota \in I}$ *là một họ ánh xạ có cùng đích* F *sao cho với mọi* $\iota \in I$ *nguồn của* $f_\iota$ *là* $X_\iota$, *và với mọi cặp* $(\iota, \varkappa) \in I \times I$, $f_\iota$ *và* $f_\varkappa$ *trùng nhau trên* $X_\iota \cap X_\varkappa$. *Khi đó tồn tại đúng một hàm* $f$ *có nguồn* $A = \bigcup_{\iota \in I} X_\iota$ *và đích* F *kéo dài mỗi hàm* $f_\iota$ $(i \in I)$.

(1) Cho $x$ là một phần tử bất kỳ của E. Khi đó tồn tại $\iota \in I$ sao cho $x \in X_\iota$, do đó $f(x) = g(x)$ theo giả thiết.
(2) Gọi $G_\iota$ là đồ thị của $f_\iota$ và đặt $G = \bigcup_{\iota \in I} G_\iota$; hãy chứng tỏ rằng G là một đồ thị phiếm hàm. Nếu $(x, y) \in G$ và $(x, y') \in G$, thì tồn tại hai chỉ số $\iota$, $\varkappa$ trong I sao cho $(x, y) \in G_\iota$ và $(x, y') \in G_\varkappa$. Điều này kéo theo $x \in X_\iota$, $x \in X_\varkappa$, $y = f_\iota(x)$, $y' = f_\varkappa(x)$; nhưng vì $x \in X_\iota \cap X_\varkappa$, ta có

$$f_\iota(x) = f_\varkappa(x),$$

tức là, $y = y'$. Đồ thị G có tập xác định $\mathrm{pr}_1 G = \bigcup_{\iota \in I} \mathrm{pr}_1 G_\iota = A$; do đó hàm $f = (G, A, F)$ thỏa mãn các điều kiện đã yêu cầu. Tính duy nhất của nó suy ra từ phần thứ nhất của Mệnh đề.

### 7. PHÂN HOẠCH

#### Định nghĩa 6 {#ens-ii-s4-def-6 .statement tag=03Q0}

*Hai tập hợp* A *và* B *được gọi là rời nhau* (*hay không giao nhau*) *nếu* $A \cap B = \emptyset$. *Nếu* $A \cap B \neq \emptyset$, *ta nói rằng* A *gặp* (*hay giao*) B. *Cho*

$(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$ *là một họ các tập hợp. Các tập hợp của họ này được gọi là đôi một rời nhau nếu các điều kiện* $\iota \in \mathrm{I}$, $\varkappa \in \mathrm{I}$, $\iota \neq \varkappa$ *kéo theo* $\mathrm{X}_\iota \cap \mathrm{X}_\varkappa = \emptyset$.

Cho $f$ là một ánh xạ của A vào B, và cho $(\mathrm{Y}_\iota)_{\iota \in \mathrm{I}}$ là một họ các tập con đôi một rời nhau của B. Mệnh đề 4 khi đó cho thấy rằng các tập hợp của họ $(\overset{-1}{f}\langle \mathrm{Y}_\iota \rangle)_{\iota \in \mathrm{I}}$ gồm các tập con của A là đôi một rời nhau. Mặt khác, nếu $(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$ là một họ các tập con đôi một rời nhau của A, thì nói chung các tập hợp của họ $(f \langle \mathrm{X}_\iota \rangle)_{\iota \in \mathrm{I}}$ không đôi một rời nhau.

#### Mệnh đề 8 {#ens-ii-s4-prop-8 .statement tag=03Q1}

*Cho* $(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$ *là một họ các tập hợp đôi một rời nhau, và cho* $(f_\iota)_{\iota \in \mathrm{I}}$ *là một họ các hàm cùng có đích là* F *sao cho miền xác định của* $f_\iota$ *là* $\mathrm{X}_\iota$ *với mỗi* $\iota \in \mathrm{I}$. *Khi đó tồn tại đúng một hàm f có miền xác định là* $\bigcup_{\iota \in \mathrm{I}} \mathrm{X}_\iota$ *và có đích là* F *mở rộng từng hàm* $f_\iota$ $(\iota \in \mathrm{I})$.

Đây là một hệ quả của Mệnh đề 7, vì $f_\iota$ và $f_\varkappa$ rõ ràng trùng nhau trên $\mathrm{X}_\iota \cap \mathrm{X}_\varkappa = \emptyset$ với mọi $\iota \neq \varkappa$.

#### Định nghĩa 7 {#ens-ii-s4-def-7 .statement tag=03Q2}

*Một phân hoạch của một tập hợp* E *là một họ các tập con* khác rỗng *đôi một rời nhau của* E *mà hợp bằng* E.

#### Ví dụ {#ens-ii-s4-n7-exa-1 .statement tag=03I9}

Với mọi tập hợp A khác rỗng, họ $(\{x\})_{x \in \mathrm{A}}$ là một phân hoạch của A.

Nếu $(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$ là một phân hoạch của một tập hợp E, thì ánh xạ $\iota \rightarrow \mathrm{X}_\iota$ từ I lên tập hợp $\mathfrak{F}$ các phần tử $\mathrm{X}_\iota$ của phân hoạch là song ánh. Do đó, nếu $\mathfrak{F}$ đã cho, thì phân hoạch được xác định đến một sự tương ứng một-một giữa các tập hợp chỉ số. Thông thường khi nói đến một phân hoạch, điều mà ta xét là tập hợp các phần tử của phân hoạch.

### 8. TỔNG CỦA MỘT HỌ TẬP HỢP

#### Mệnh đề 9 {#ens-ii-s4-prop-9 .statement tag=03Q3}

*Cho* $(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$ *là một họ tập hợp. Khi đó tồn tại một tập hợp* X *có tính chất sau* : X *là hợp của một họ* $(\mathrm{X}'_\iota)_{\iota \in \mathrm{I}}$ *các tập hợp đôi một rời nhau sao cho với mỗi* $\iota \in \mathrm{I}$ *tồn tại một ánh xạ một-một từ* $\mathrm{X}_\iota$ *lên* $\mathrm{X}'_\iota$.

Cho $\mathrm{A} = \bigcup_{\iota \in \mathrm{I}} \mathrm{X}_\iota$. Nếu $\iota \in \mathrm{I}$, ánh xạ $x \rightarrow (x, \iota)$ $(x \in \mathrm{X}_\iota)$ là một ánh xạ một-một của $\mathrm{X}_\iota$ lên một tập con $\mathrm{X}'_\iota$ của $\mathrm{A} \times \mathrm{I}$. Hơn nữa, ảnh của $\mathrm{X}'_\iota$ dưới hàm tọa độ thứ hai trên $\mathrm{A} \times \mathrm{I}$ được chứa trong tập hợp $\{\iota\}$; suy ra $\mathrm{X}'_\iota \cap \mathrm{X}'_\varkappa = \emptyset$ mỗi khi $\iota \neq \varkappa$. Khi đó ta có thể lấy $\mathrm{X} = \bigcup_{\iota \in \mathrm{I}} \mathrm{X}'_\iota$.

#### Định nghĩa 8 {#ens-ii-s4-def-8 .statement tag=03Q4}

*Cho* $(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$ *là một họ tập hợp. Tổng của họ này là hợp của họ các tập hợp* $(\mathrm{X}_\iota \times \{\iota\})_{\iota \in \mathrm{I}}$.

#### Mệnh đề 10 {#ens-ii-s4-prop-10 .statement tag=03IA}

*Cho* $(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$ *là một họ các tập hợp đôi một rời nhau. Gọi* A *là hợp của chúng và* S *là tổng của chúng. Khi đó tồn tại một ánh xạ song ánh của* A *lên* S.

Với mỗi $\iota \in \mathrm{I}$, gọi $f_\iota$ là một song ánh của $\mathrm{X}_\iota$ lên $\mathrm{X}_\iota \times \{\iota\}$. Do Mệnh đề 8, tồn tại một ánh xạ $f$ của A vào S mở rộng mọi ánh xạ $f_\iota$. Ngay lập tức kiểm tra được rằng $f$ là một ánh xạ song ánh của A lên S.

Do lạm dụng ngôn ngữ, nói rằng một tập hợp E là *tổng* của một họ các tập hợp $(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$ nếu tồn tại một song ánh của E lên tổng của họ ấy, như được định nghĩa trong Định nghĩa 8.

Chú ý rằng nếu $(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$ là một họ tùy ý các tập hợp, thì lập luận của Mệnh đề 10 cho thấy rằng tồn tại một ánh xạ của tổng S *lên* hợp A.

### Bài tập {#ens-ii-s4-exercises}

Xem [bài tập cho § 4](exercises/s4/).

[^1]: Do đó lược đồ S8 cho phép ta định nghĩa hợp của một họ các tập hợp mà không giả thiết *a priori* rằng các tập hợp ấy là các tập hợp con của cùng một tập hợp (đó là giả thiết được đưa ra trong định nghĩa của hợp trong *Tóm tắt các kết quả*, §4, no. 2).
[^2]: Một sai lầm nổi tiếng nảy sinh từ việc áp dụng công thức này là sai lầm của H. Lebesgue trong cố gắng chứng minh rằng phép chiếu trên một trục của một tập hợp Borel trong mặt phẳng lại là một tập hợp Borel (mệnh đề này về sau được chỉ ra là không đúng, và cuộc thảo luận do đó gợi ra là nguồn gốc của lý thuyết các tập hợp "Souslin") : Lebesgue đã khẳng định rằng phép chiếu của giao của một dãy giảm các tập hợp bằng giao các phép chiếu của chúng (*Journal de Mathématiques*, (6) **1** (1905), pp. 191-192).
