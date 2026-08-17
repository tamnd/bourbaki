---
book: ens
book_title: Theory of Sets
chapter: II
chapter_title: THEORY OF SETS
section: 2
section_title: Ordered pairs
lang: vi
source: ens-i-iv
source_edition: 2004, Springer
book_pages: 72-75, 123-124
pdf_pages: 0079-0082, 0130-0131
extraction: ocr
subsections:
    - "no": 1
      title: THE AXIOM OF THE ORDERED PAIR
      page: 72
      pdf_page: 79
    - "no": 2
      title: PRODUCT OF TWO SETS
      page: 74
      pdf_page: 81
statements: 4
exercises: 2
content_sha256: 69edacf791916abc0f4850e775a07ae78849235650d970488e494a3a227a3ad8
translated_from: content/en/ens/II/02_s2_ordered_pairs.md
source_content_sha256: 39df2ab84c1a4cd7487506eb10473433071a3570142a04a0b8feb982b45bc203
translation_model: gpt-5.4
translation_run: translate-vi-4abbdd52
glossary_version: 29
glossary_terms_sha256: df8243a38159a7bd62daf35c2e1df16921609d27da37704f9da5940e44cf92fe
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 2. CÁC CẶP CÓ THỨ TỰ

### 1. TIÊN ĐỀ VỀ CẶP CÓ THỨ TỰ

Như chúng ta đã nói ở §1, no. 1, ký hiệu $\supset$ là một ký hiệu tạo số hạng có trọng số 2 trong lý thuyết tập hợp. Nếu T, U là các số hạng, thì $\supset$TU là một số hạng, trên thực tế được ký hiệu bởi (T, U). Trong ký hiệu này, *tiên đề về cặp có thứ tự* là như sau :

A3. $(\forall x)(\forall x')(\forall y)(\forall y')(((x, y) = (x', y')) \Rightarrow (x = x' \quad \text{và} \quad y = y'))$.

Vì quan hệ "$x = x'$ và $y = y'$" kéo theo $(x, y) = (x', y')$ theo C44 (Chương I, § 5, no. 2), nên quan hệ $(x, y) = (x', y')$ là *tương đương* với "$x = x'$ và $y = y'$".

¶ Quan hệ $(\exists x)(\exists y)(z=(x,y))$ được viết là “$z$ là một *cặp có thứ tự*”. Nếu $z$ là một cặp có thứ tự, thì các quan hệ

$$
(\exists y)(z=(x,y)),\qquad(\exists x)(z=(x,y))
$$

là các phiếm hàm đối với $x$ và $y$ tương ứng; đây là một hệ quả ngay lập tức của A3. Các số hạng

$$
\tau_x((\exists y)(z=(x,y)))\qquad\text{và}\qquad\tau_y((\exists x)(z=(x,y)))
$$

được ký hiệu tương ứng bởi $\operatorname{pr}_1z$ và $\operatorname{pr}_2z$, và được gọi là *tọa độ thứ nhất* (hoặc *phép chiếu thứ nhất*) và *tọa độ thứ hai* (hoặc *phép chiếu thứ hai*) của $z$. Nếu $z$ là một cặp có thứ tự, thì quan hệ $(\exists y)(z=(x,y))$ tương đương với $x=\operatorname{pr}_1z$, và quan hệ $(\exists x)(z=(x,y))$ tương đương với $y=\operatorname{pr}_2z$ (Chương I, §5, số 3).

¶ Quan hệ $z=(x,y)$ tương đương với “$z$ là một cặp có thứ tự, và $x=\operatorname{pr}_1z$ và $y=\operatorname{pr}_2z$”; vì quan hệ sau tương đương với

$$
(\exists x')(\exists y')(\exists x'')(\exists y'')(z=(x',y')\text{ và }z=(x,y'')\text{ và }z=(x'',y));
$$

theo A3, “$z=(x',y')$ và $z=(x,y'')$ và $z=(x'',y)$” tương đương với “$z=(x,y)$ và $x=x'$ và $x=x''$ và $y=y'$ và $y=y''$”; do đó theo C33 (Chương I, §4, no. 3), “$z$ là một cặp có thứ tự, và $x=\operatorname{pr}_1z$ và $y=\operatorname{pr}_2z$” tương đương với

$$
z=(x,y)\text{ và }(\exists x')(\exists y')(\exists x'')(\exists y'')(x=x'\text{ và }x=x''\text{ và }y=y'\text{ và }y=y''),
$$

điều này chứng minh mệnh đề của chúng ta. Hiển nhiên ta có

$$
\operatorname{pr}_1(x,y)=x,\qquad \operatorname{pr}_2(x,y)=y,
$$

và quan hệ $z=(\operatorname{pr}_1(z),\operatorname{pr}_2(z))$ tương đương với “$z$ là một cặp có thứ tự”.

¶ Cho $R\{x,y\}$ là một quan hệ, trong đó các chữ $x$ và $y$ là phân biệt và xuất hiện trong $R$. Cho $z$ là một chữ, phân biệt với $x$ và $y$, không xuất hiện trong $R$. Gọi $S\{z\}$ là quan hệ

$$
(\exists x)(\exists y)(z=(x,y)\text{ và }R\{x,y\});
$$

đây là một quan hệ chứa ít hơn $R$ một chữ cái, và *tương đương* với “$z$ là một cặp có thứ tự và $R\{\operatorname{pr}_1z,\operatorname{pr}_2z\}$”; điều này suy ra từ sự kiện rằng $z=(x,y)$ tương đương với “$z$ là một cặp có thứ tự và $x=\operatorname{pr}_1z$ và $y=\operatorname{pr}_2z$”, và từ các tiêu chuẩn C33 (Chương I, §4, no. 3)

và C47 (Chương I, §5, no. 3). Ngay lập tức suy ra rằng $R\{x, y\}$ tương đương với $S\{(x, y)\}$, và cũng tương đương với

$$(\exists z)(z = (x, y) \text{ và } S\{z\})$$

theo C47.

Điều đó có nghĩa là ta có thể diễn giải một quan hệ giữa các đối tượng $x$ và $y$ như một tính chất của cặp có thứ tự được tạo thành bởi các đối tượng ấy.

### 2. TÍCH CỦA HAI TẬP HỢP

#### Định lý 1 {#ens-ii-s2-thm-1 .statement tag=03PC}

*Quan hệ*

$$(\forall X)(\forall Y)(\exists Z)(\forall z)((z \in Z) \Leftrightarrow (\exists x)(\exists y)(z = (x, y) \text{ và } x \in X \text{ và } y \in Y)$$

*là đúng. Nói cách khác, với mọi* X *và mọi* Y *thì quan hệ* "$z$ *là một cặp có thứ tự và* $\mathrm{pr}_1 z \in X$ *và* $\mathrm{pr}_2 z \in Y$" *xác định tập theo* $z$.

Ký hiệu $A_y$ là tập hợp của mọi đối tượng dạng $(x, y)$ với $x \in X$ (xem §1, no. 6, tiêu chuẩn C53). Gọi R là quan hệ $z \in A_y$, tương đương với $(\exists x)(z = (x, y)$ and $x \in X)$. Hiển nhiên quan hệ

$$(\forall y)(\exists A)(\forall z)(R \Rightarrow (z \in A))$$

đúng, theo S5 (Chương I, §4, no. 2). Khi đó suy ra từ S8 rằng quan hệ $(\exists y)(y \in Y$ và R$)$ là xác định tập theo $z$. Nhưng quan hệ này tương đương với $(\exists x)(\exists y)(y \in Y$ và $x \in X$ và $z = (x, y))$; do đó có kết quả.

#### Định nghĩa 1 {#ens-ii-s2-def-1 .statement tag=03PD}

*Cho hai tập hợp* X *và* Y, *tập hợp*

$$\mathcal{E}_z((\exists x)(\exists y)(z = (x, y) \text{ và } x \in X \text{ và } y \in Y))$$

*được gọi là tích của* X *và* Y *và được ký hiệu là* X $\times$ Y.

Quan hệ $z \in X \times Y$ do đó tương đương với "$z$ là một cặp có thứ tự và $\mathrm{pr}_1 z \in X$ và $\mathrm{pr}_2 z \in Y$". Các tập hợp X và Y được gọi là *thừa số thứ nhất* và *thừa số thứ hai* của X $\times$ Y.

#### Mệnh đề 1 {#ens-ii-s2-prop-1 .statement tag=03PE}

*Nếu* A$'$, B$'$ *là các tập hợp không rỗng, quan hệ* A$' \times$ B$' \subset$ A $\times$ B *tương đương với* "A$' \subset$ A *và* B$' \subset$ B".

Trước hết, quan hệ $z \in A' \times B'$ tương đương với "$z$ là một cặp có thứ tự và $\mathrm{pr}_1 z \in A'$ và $\mathrm{pr}_2 z \in B'$"; do đó, không có bất kỳ hạn chế nào đối với A$'$ và B$'$, quan hệ "A$' \subset$ A và B$' \subset$ B" suy ra

$$A' \times B' \subset A \times B.$$

Ngược lại, trước hết ta hãy chỉ ra rằng nếu $B' \neq \emptyset$ (không có hạn chế nào đối với $A'$), quan hệ $A' \times B' \subset A \times B$ suy ra $A' \subset A$. Lấy $x$ là một phần tử của $A'$; vì $B' \neq \emptyset$, tồn tại một đối tượng $y$ là một phần tử của $B'$; ta có $(x, y) \in A' \times B'$, do đó $(x, y) \in A \times B$, và do đó $x \in A$; vậy $A' \subset A$. Tương tự, nếu $A' \neq \emptyset$, quan hệ $A' \times B' \subset A \times B$ suy ra $B' \subset B$. Do đó có kết quả phải chứng minh.

#### Mệnh đề 2 {#ens-ii-s2-prop-2 .statement tag=03PF}

*Cho* A *và* B *là hai tập hợp. Quan hệ* $A \times B = \emptyset$ *tương đương với* "$A = \emptyset$ *hoặc* $B = \emptyset$".

Thật vậy, quan hệ $z \in A \times B$ kéo theo $\mathrm{pr}_1 z \in A$ và $\mathrm{pr}_2 z \in B$; do đó $A \neq \emptyset$ và $B \neq \emptyset$. Ngược lại, quan hệ "$x \in A$ và $y \in B$" kéo theo $(x, y) \in A \times B$ và do đó $A \times B \neq \emptyset$. Nói cách khác, quan hệ $A \times B \neq \emptyset$ tương đương với "$A \neq \emptyset$ và $B \neq \emptyset$"; do đó suy ra kết quả.

Nếu A, B, C là các tập hợp, ta viết

$$(A \times B) \times C = A \times B \times C;$$

một phần tử $((x, y), z)$ của $A \times B \times C$ được viết là $(x, y, z)$ và được gọi là một *bộ ba*. Tương tự, nếu A, B, C, D là các tập hợp, ta viết

$$(A \times B \times C) \times D = A \times B \times C \times D;$$

vân vân.

### Bài tập {#ens-ii-s2-exercises}

Xem [bài tập của § 2](exercises/s2/).
