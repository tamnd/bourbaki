---
book: alg
book_title: Algebra
chapter: I
chapter_title: ALGEBRAIC STRUCTURES
section: 5
section_title: Groups operating on a set
lang: vi
source: alg-i-iii
source_edition: 1998, Springer
pdf_pages: 0076-0089, 0164-0171
extraction: ocr
subsections:
    - "no": 1
      title: MONOID OPERATING ON A SET
      page: 0
      pdf_page: 76
    - "no": 2
      title: STABILIZER, FIXER
      page: 0
      pdf_page: 78
    - "no": 3
      title: INNER AUTOMORPHISMS
      page: 0
      pdf_page: 79
    - "no": 4
      title: ORBITS
      page: 0
      pdf_page: 80
    - "no": 5
      title: HOMOGENEOUS SETS
      page: 0
      pdf_page: 82
    - "no": 6
      title: HOMOGENEOUS PRINCIPAL SETS
      page: 0
      pdf_page: 84
    - "no": 7
      title: PERMUTATION GROUPS OF A FINITE SET
      page: 0
      pdf_page: 85
statements: 32
exercises: 29
content_sha256: 6f22e69787c7147dcc0aff8bf0fe5b2edc05d1c970bfdb3082b43dfb860dc633
translated_from: content/en/alg/I/05_s5_groups_operating_on_a_set.md
source_content_sha256: 1bfc7d980bffef016673f763fb429cbbf5132ed5919da50c944ba75ba35ea265
translation_model: gpt-5-6-mini, gpt-5-6
translation_run: translate-vi-4c9756fc
glossary_version: 34
glossary_terms_sha256: d58c525fee6d71ad09a54d0eaefaf1e510ce8a4f3a22da8c429c3fa75edc3371
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 5. CÁC NHÓM TÁC ĐỘNG TRÊN MỘT TẬP HỢP

### 1. ĐƠN VỊ TÁC ĐỘNG TRÊN MỘT TẬP HỢP

#### Định nghĩa 1 {#alg-i-s5-def-1 .statement}

Cho M là một đơn vị, với luật được viết theo phép nhân và phần tử đơn vị được ký hiệu bởi e, và E là một tập hợp. Một tác động $\alpha \mapsto f_\alpha$ của M trên E được gọi là tác động trái (resp. phải) của M trên E nếu $f_e = \mathrm{Id}_E$ và $f_{\alpha \beta} = f_\alpha \circ f_\beta$ (resp. $f_{\alpha \beta} = f_\beta \circ f_\alpha$) với mọi $\alpha, \beta \in M$.

Nói cách khác, một tác động trái (resp. phải) của một đơn vị M trên một tập hợp E là một đồng cấu đơn vị từ M vào đơn vị $E^E$ (resp. đơn vị đối của $E^E$) với phép hợp thành của các ánh xạ. Nếu luật tác động tương ứng với tác động của M được ký hiệu bởi phép nhân trái (resp. phải), thì sự kiện tác động này là một tác động trái (resp. phải) có thể được biểu thị bằng các công thức

(1)
$$
e.x = x; \quad \alpha.(\beta.x) = (\alpha \beta).x \quad \text{với } \alpha, \beta \in M \text{ và } x \in E.
$$
(resp. $x.e = x; \quad (x.\alpha).\beta = x.(\alpha \beta) \quad \text{với } \alpha, \beta \in M \text{ và } x \in E$).

Với các điều kiện này, người ta cũng nói rằng M tác động trên E ở bên trái (resp. phải) và các luật tác động tương ứng là các luật tác động trái (resp. phải) của đơn vị M trên E.

Cho M là một đơn vị; một tập hợp E với một tác động trái (resp. phải) của M trên E được gọi là một M-tập hợp trái (resp. phải). Đơn vị M được nói là tác động trung thành ở bên trái (resp. phải) nếu ánh xạ $\alpha \mapsto f_\alpha$ của M vào $E^E$ là đơn ánh.

#### Ví dụ {#alg-i-s5-n1-exa-1 .statement}

(1) Cho E là một tập hợp; tác động chính tắc của $E^E$ trên E (\S 3, no. 1, Ví dụ 3) là một tác động trái.

(2) Cho M là một đơn vị. Tác động trái (resp. phải) của M trên chính nó dẫn xuất từ luật trên M (\S 3, no. 3, Ví dụ 7) là một tác động trái (resp. phải) của M trên chính nó. Khi xét tác động này, ta nói rằng M tác động trên chính nó bằng phép tịnh tiến trái (resp. phải).

Cho E là một M-tập hợp trái (resp. phải) và $M^0$ là đơn vị đối của M. Với cùng tác động ấy, đơn vị $M^0$ tác động trên E ở bên phải (resp. trái). $M^0$-tập hợp thu được được gọi là đối của M-tập hợp E. Các định nghĩa và kết quả liên quan đến các M-tập hợp trái được chuyển sang các M-tập hợp phải $M^0$ khi chuyển qua các cấu trúc đối.

Trong phần còn lại của đoạn này, ta sẽ xét, trừ khi có nói khác đi, chỉ các M-tập hợp trái mà ta sẽ gọi đơn giản là các M-tập hợp. Luật tác động của chúng sẽ được ký hiệu bởi phép nhân trái.

Cho E là một tập hợp. Cho G là một nhóm tác động trên E. Với mọi $\alpha$ trong G, phần tử của $E^E$ được xác định bởi $\alpha$ là một phép hoán vị của E ($\S$ 2, no. 3, Ví dụ 2). Do đó, cho một tác động của G trên E tương đương với cho một đồng cấu của G vào $\mathfrak{S}_E$.

Phù hợp với $\S$ 3, no. 3, ta đưa ra định nghĩa sau:

#### Định nghĩa 2 {#alg-i-s5-def-2 .statement}

*Cho M là một đơn vị và E và E' là các M-tập hợp. Một ánh xạ f của E vào E' sao cho, với mọi $x \in E$ và mọi $\alpha \in M$, $f(\alpha.x) = \alpha.f(x)$ được gọi là một đồng cấu M-tập hợp (hay một M-cấu xạ, hay một ánh xạ tương thích với các tác động của M).*

Ánh xạ đồng nhất của một M-tập hợp là một M-cấu xạ. Hợp thành của hai M-cấu xạ là một M-cấu xạ. Đối với một ánh xạ từ một M-tập hợp này vào một M-tập hợp khác, để là một đẳng cấu, điều kiện cần và đủ là nó là một M-cấu xạ song ánh và khi đó ánh xạ nghịch đảo là một M-cấu xạ.

Cho $(E_i)_{i \in I}$ là một họ các M-tập hợp và E là tập hợp tích của $E_i$. Đơn vị M tác động trên E bởi $\alpha.(x_i)_{i \in I} = (\alpha.x_i)_{i \in I}$ và E, với tác động này, là một M-tập hợp; cho E' là một M-tập hợp; một ánh xạ f của E' vào E là một M-cấu xạ khi và chỉ khi $pr_i \circ f$ là một M-cấu xạ của E' vào $E_i$ với mọi $i \in I$.

Cho E là một M-tập hợp và F là một tập con ổn định của E dưới tác động của M; với luật cảm sinh, F là một M-tập hợp và đơn ánh chính tắc $F \to E$ là một M-cấu xạ.

Cho E là một M-tập hợp và R là một quan hệ tương đương trên E tương thích với tác động của M; thương $E/R$ với tác động thương là một M-tập hợp và ánh xạ chính tắc $E \to E/R$ là một M-cấu xạ.

Cho $\phi : M \to M'$ là một đồng cấu đơn vị, E là một M-tập hợp và E' là một $M'$-tập hợp. Một ánh xạ f của E vào E' sao cho, với mọi $x \in E$ và $\alpha \in M$,

$$
f(\alpha.x) = \phi(\alpha).f(x)
$$

được gọi là một $\phi$-cấu xạ của E vào E' (xem $\S$ 3, no. 1).

*Mở rộng một luật tác động.* Cho (chẳng hạn) ba tập hợp $F_1, F_2, F_3$, các phép hoán vị $f_1, f_2, f_3$ của $F_1, F_2, F_3$ tương ứng và một cấu trúc tầng F trên các tập hợp cơ sở $F_1, F_2, F_3$ (*Lý thuyết tập hợp*, IV, $\S$ 1, no. 1), ta có thể, tiến hành từng bước theo phép dựng cấu trúc tầng F, xác định một phép hoán vị của F được gọi là *mở rộng chính tắc* của $f_1, f_2, f_3$ lên F (*Lý thuyết tập hợp*, IV, $\S$ 1, no. 2); ta sẽ ký hiệu nó bởi $\phi_F(f_1, f_2, f_3)$.

Khi đó cho G là một nhóm và $h_i$ là một đồng cấu của G vào nhóm đối xứng của $F_i$ ($i = 1, 2, 3$), nói cách khác là một tác động của G trên $F_i$. Ánh xạ $x \mapsto x_F = \phi_F(h_1(x), h_2(x), h_3(x))$ là một đồng cấu của G vào $\mathfrak{S}_F$, nói cách khác là một tác động của G trên F, được gọi là *mở rộng* của $h_1, h_2, h_3$ lên F. Cho P là một tập con của F sao cho, với mọi $x \in G$, $x_F(P) = P$; cho $x_P$ là hạn chế của $x_F$ lên

P; khi đó ánh xạ $x \mapsto x_P$ là một phép toán của G trên P, cũng gọi là phép mở rộng của $h_1, h_2, h_3$ lên P.

Chẳng hạn, cho K và L là hai thang trên $F_1, F_2, F_3$; lấy F là tập hợp các tập con của $K \times L$ và P là tập hợp các ánh xạ từ K vào L, được đồng nhất với các đồ thị của chúng. Nếu $w \in P$ và $x \in G$, $x_P(w)$ là ánh xạ $k \mapsto x_L(w(x_K^{-1}(k)))$ từ K vào L.

### 2. NHÓM ỔN ĐỊNH, NHÓM CỐ ĐỊNH

#### Định nghĩa 3 {#alg-i-s5-def-3 .statement}

*Cho M là một monoid tác động trên một tập hợp E và A và B là các tập con của E. Tập hợp các $\alpha \in M$ sao cho $\alpha A \subset B$ (tương ứng, $\alpha A = B$) được gọi là tập chuyển của A vào B (tương ứng, tập chuyển ngặt). Tập chuyển (tương ứng, tập chuyển ngặt) của A vào A được gọi là nhóm ổn định (tương ứng, nhóm ổn định ngặt) của A. Tập hợp các $\alpha \in M$ sao cho $\alpha a = a$ với mọi $a \in A$ được gọi là tập cố định của A.*

Một phần tử $\alpha$ của M được nói là ổn định (tương ứng, ổn định ngặt, tương ứng, cố định) một tập con A của E nếu $\alpha$ thuộc nhóm ổn định (tương ứng, nhóm ổn định ngặt, tương ứng, tập cố định) của A. Một tập con P của M được nói là ổn định (tương ứng, ổn định ngặt, tương ứng, cố định) một tập con A của E nếu mọi phần tử của P đều ổn định (tương ứng, ổn định ngặt, tương ứng, cố định) A. Tập cố định của A được chứa trong nhóm ổn định ngặt của A, mà chính nó được chứa trong nhóm ổn định của A.

#### Mệnh đề 1 {#alg-i-s5-prop-1 .statement}

*Cho M là một monoid tác động trên một tập hợp E và A là một tập con của E.*
(a) *Nhóm ổn định, nhóm ổn định ngặt và tập cố định của A là các monoid con của M.*
(b) *Cho $\alpha$ là một phần tử khả nghịch của M; nếu $\alpha$ thuộc nhóm ổn định ngặt (tương ứng, tập cố định) của A thì $\alpha^{-1}$ cũng vậy.*

Cho e là phần tử đơn vị của M; khi đó $ea = a$ với mọi phần tử $a \in A$ và do đó e thuộc tập cố định của A. Cho $\alpha$ và $\beta$ là các phần tử của E ổn định A. Khi đó $(\alpha \beta)A = \alpha(\beta A) \subset \alpha A \subset A$ và do đó nhóm ổn định của A là một monoid con của M. Tương tự đối với nhóm ổn định ngặt và tập cố định của A, do đó có (a). Nếu $\alpha A = A$, thì $A = \alpha^{-1}(\alpha A) = \alpha^{-1}A$. Nếu với mọi $a \in A$, $\alpha a = a$, thì $a = \alpha^{-1}(\alpha a) = \alpha^{-1}a$, do đó có (b).

#### Hệ quả {#alg-i-s5-n2-cor-1 .statement}

*Cho G là một nhóm tác động trên một tập hợp E và A là một tập con của E. Nhóm ổn định ngặt S và tập cố định F của A là các nhóm con của G và F là một nhóm con chuẩn tắc của S.*

Mệnh đề thứ nhất suy ra từ mệnh đề trên và F là hạt nhân của đồng cấu từ S vào $\mathfrak{S}_A$ liên kết với phép toán của S trên A.

Một nhóm G tác động trung thành trên một tập hợp E khi và chỉ khi tập cố định của E gồm phần tử đơn vị của G. Tập cố định của E là hạt nhân của đồng cấu đã cho từ G vào $\mathfrak{S}_E$; đồng cấu này đơn ánh khi và chỉ khi hạt nhân của nó gồm phần tử đơn vị (\S 4, no. 5, Định lý 3).

Cho M là một monoid, E một M-tập và $a$ một phần tử của E. Tập cố định, nhóm ổn định ngặt và nhóm ổn định của $\{a\}$ bằng nhau; monoid này cũng được gọi là tập cố định hoặc nhóm ổn định của $a$. Tập cố định của một tập con A của E là giao của các tập cố định của các phần tử của A. $a$ được gọi là một phần tử bất biến của E nếu tập cố định của $a$ là monoid M. M được nói là tác động tầm thường trên E nếu mọi phần tử của E đều bất biến.

#### Mệnh đề 2 {#alg-i-s5-prop-2 .statement}

*Cho G là một nhóm tác động trên một tập hợp E và, với mọi $x \in E$, cho $S_x$ là nhóm ổn định của x. Với mọi $\alpha \in G$, $S_{\alpha x} = \alpha S_x \alpha^{-1}$.*

Nếu $s \in S_x$, thì $\alpha s \alpha^{-1}(\alpha x) = \alpha s x = \alpha x$, do đó $\alpha S_x \alpha^{-1} \subset S_{\alpha x}$. Vì $x = \alpha^{-1}(\alpha x)$, $\alpha^{-1} S_{\alpha x} \alpha \subset S_x$, do đó $S_{\alpha x} \subset \alpha S_x \alpha^{-1}$.

Tương tự, ta thấy rằng, nếu A và B là hai tập con của E và T là tập chuyển (tương ứng, tập chuyển ngặt) của A vào B, thì tập chuyển (tương ứng, tập chuyển ngặt) của $\alpha A$ vào $\alpha B$ bằng $\alpha T \alpha^{-1}$.

### 3. TỰ ĐẲNG CẤU NỘI

Cho G là một nhóm. Tập hợp Aut(G) các tự đẳng cấu của nhóm G là một nhóm con của $\mathcal{G}_G$ (\S 4, no. 1, Ví dụ 2).

#### Mệnh đề 3 {#alg-i-s5-prop-3 .statement}

*Cho G là một nhóm. Với mọi phần tử x của G, ánh xạ Int(x): $y \mapsto xyx^{-1}$ từ G vào chính nó là một tự đẳng cấu của G. Ánh xạ Int: $x \mapsto \operatorname{Int}(x)$ từ G vào Aut(G) là một đồng cấu nhóm, có hạt nhân là tâm của G và có ảnh là một nhóm con chuẩn tắc của Aut(G).*

Nếu $x, y$ và $z$ là các phần tử của G, thì $(xyx^{-1})(xz x^{-1}) = xyz x^{-1}$ và do đó Int(x) là một tự đồng cấu của G. Với $x$ và $y$ là các phần tử của G,

$$
\operatorname{Int}(x) \circ \operatorname{Int}(y) = \operatorname{Int}(xy):
$$

với mọi $z \in G$, $x(yzy^{-1})x^{-1} = (xy)z(xy)^{-1}$. Mặt khác, $\operatorname{Int}(e)$ là ánh xạ đồng nhất của G. Do đó ánh xạ Int là một đồng cấu monoid từ G vào monoid End(G) của các đồng cấu của nhóm G. Vì các phần tử của G đều khả nghịch, ánh xạ Int nhận giá trị trong tập Aut(G) các phần tử khả nghịch của End(G) (\S 2, no. 3). Khi đó $xyx^{-1} = y$ khi và chỉ khi $x$ và $y$ giao hoán và do đó $\operatorname{Int}(x)$ là ánh xạ đồng nhất của G khi và chỉ khi $x$ là một phần tử trung tâm. Cuối cùng, cho $\alpha$ là một tự đẳng cấu của G và cho $x \in G$; khi đó

$$
\operatorname{Int}(\alpha(x)) = \alpha \circ \operatorname{Int}(x) \circ \alpha^{-1}.
$$

Với $y \in G$,

$$
\alpha(x) \cdot y \cdot \alpha(x)^{-1} = \alpha(x) \cdot \alpha(\alpha^{-1}(y)) \cdot \alpha(x)^{-1} = \alpha(x \cdot \alpha^{-1}(y) \cdot x^{-1}).
$$

Do đó $\alpha \cdot \operatorname{Int}(G) \cdot \alpha^{-1} \subset \operatorname{Int}(G)$.

#### Định nghĩa 4 {#alg-i-s5-def-4 .statement}

*Cho G là một nhóm và $x \in G$. Tự đẳng cấu $y \mapsto xyx^{-1}$ được gọi là tự đẳng cấu trong của G xác định bởi x và được ký hiệu là $\operatorname{Int} x$.*

Với $x, y \in G$, ta cũng viết $x^y = y^{-1}xy = (\operatorname{Int} y^{-1})(x)$.

Một nhóm con của G là chuẩn nếu và chỉ nếu nó ổn định dưới mọi tự đẳng cấu trong của G (\S 4, no. 4, Định nghĩa 5). Một nhóm con của G được gọi là bất biến nếu nó ổn định dưới mọi tự đẳng cấu của G. Tâm của một nhóm G là một nhóm con bất biến (công thức (2)).

Tâm của một nhóm G không nhất thiết ổn định dưới mọi đồng cấu của G (Bài tập 22). Đặc biệt, tâm của một nhóm có toán tử không nhất thiết là một nhóm con ổn định.

#### Mệnh đề 4 {#alg-i-s5-prop-4 .statement}

Cho G là một nhóm, H là một nhóm con bất biến (tương ứng, chuẩn) của G và K là một nhóm con bất biến của H. Khi đó K là một nhóm con bất biến (tương ứng, chuẩn) của G.

Hạn chế trên H của một tự đẳng cấu (tương ứng, tự đẳng cấu trong) của G là một tự đẳng cấu của H và do đó giữ K bất biến.

Cho G là một nhóm, A $\subset$ G và $b \in G$. b được gọi là chuẩn hóa A nếu $bAb^{-1} = A$; b được gọi là trung tâm hóa A nếu, với mọi $a \in A$, $bab^{-1} = a$. Cho A và B là các tập con của G; B được gọi là chuẩn hóa (tương ứng, trung tâm hóa) A nếu mọi phần tử của B chuẩn hóa (tương ứng, trung tâm hóa) A.

Tập hợp các $g \in G$ chuẩn hóa (tương ứng, trung tâm hóa) A được gọi là nhóm chuẩn hóa (tương ứng, nhóm trung tâm hóa) của A (xem § 1, no. 5, Định nghĩa 9); nó đôi khi được ký hiệu bởi $N_G(A)$ hoặc đơn giản là $N(A)$ (tương ứng, $C_G(A)$ hoặc $C(A)$). Nó là một nhóm con của G. Khi A là một nhóm con của G, $N_G(A)$ có thể được đặc trưng như là nhóm con lớn nhất của G chứa A và trong đó A là chuẩn.

#### Nhận xét {#alg-i-s5-n3-rem-1 .statement}

(1) Nhóm chuẩn hóa (tương ứng, nhóm trung tâm hóa) của A là nhóm ổn định ngặt (tương ứng, nhóm cố định) của A khi G tác động lên chính nó bởi các tự đẳng cấu trong. Đặc biệt nhóm trung tâm hóa là một nhóm con chuẩn của nhóm chuẩn hóa.

(2) Tập hợp các phần tử $b \in G$ sao cho $bAb^{-1} \subset A$ là một monoid con của G. Ngay cả khi A là một nhóm con của G, tập hợp này không nhất thiết là một nhóm con của G (Bài tập 27).

### 4. QUỸ ĐẠO

#### Định nghĩa 5 {#alg-i-s5-def-5 .statement}

Cho G là một nhóm, E là một G-tập hợp và $x \in G$. Một phần tử $y \in E$ được gọi là liên hợp với x dưới tác động của G nếu tồn tại một phần tử $\alpha \in G$ sao cho $y = \alpha x$. Tập hợp các phần tử liên hợp với x được gọi là quỹ đạo của x trong E.

Quan hệ "y liên hợp với x" là một quan hệ tương đương. Với $x = ex$; nếu $y = \alpha x$, thì $x = \alpha^{-1} y$; nếu $y = \alpha x$ và $z = \beta y$, thì $z = \beta \alpha x$. Các quỹ đạo là các lớp tương đương theo quan hệ này.

Một tập con X của E ổn định khi và chỉ khi nó là tập hợp bão hòa đối với quan hệ liên hợp.

Ánh xạ $\alpha \mapsto \alpha x$ từ G vào E đôi khi được gọi là ánh xạ quỹ đạo xác định bởi x. Nó là một G-cấu xạ từ G (với tác động của G lên chính nó bởi phép tịnh tiến trái) vào E. Ảnh $G . x$ của G qua ánh xạ này là quỹ đạo của x.

G được nói là tác động tự do trên E nếu, với mọi $x \in E$, ánh xạ quỹ đạo xác định bởi x là đơn ánh, hay tương đương nếu ánh xạ $(g, x) \mapsto (gx, x)$ từ $G \times E$ vào $E \times E$ là đơn ánh.

#### Ví dụ {#alg-i-s5-n4-exa-1 .statement}

(1) Cho G là một nhóm và xét tác động của G lên chính nó bởi các tự đẳng cấu trong. Hai phần tử của G liên hợp dưới tác động này được gọi là liên hợp dưới các tự đẳng cấu trong hoặc đơn giản là liên hợp. Các quỹ đạo được gọi là các lớp liên hợp. Tương tự, hai tập con H và H' của G được gọi là liên hợp nếu tồn tại một phần tử $\alpha \in G$ sao cho $H' = \alpha . H . \alpha^{-1}$, tức là nếu chúng liên hợp dưới mở rộng lên $\mathcal{P}(G)$ của tác động của G lên chính nó bởi các tự đẳng cấu trong.

(2) *Trong không gian $\mathbf{R}^n$, quỹ đạo của một điểm x dưới tác động của nhóm trực giao $\mathbf{O}(n, \mathbf{R})$ là mặt cầu Euclid bán kính $\|x\|_*$.*

Các nhóm ổn định của hai phần tử liên hợp của E là các nhóm con liên hợp của G (no. 2, Mệnh đề 2).

Tập thương của E theo quan hệ liên hợp là tập hợp các quỹ đạo của E; đôi khi nó được ký hiệu là E/G hoặc G\|E. (Đôi khi ký hiệu E/G được dành cho trường hợp E là một G-tập hợp phải và ký hiệu G\|E cho trường hợp E là một G-tập hợp trái.)

Cho G là một nhóm tác động lên một tập hợp E ở bên phải. Cho H là một nhóm con chuẩn của G. Nhóm G tác động lên E/H ở bên phải, luật tác động phải tương ứng là $(xH, g) \mapsto xHg = xgH$; dưới tác động này, H tác động tầm thường, do đó G/H tác động phải trên E/H. Cho $\phi$ là ánh xạ chính tắc từ E/H lên E/G; các ảnh nghịch của các điểm của E/G qua $\phi$ là các quỹ đạo của G (hoặc của G/H) trong E/H. Do đó $\phi$ xác định, khi chuyển qua thương, một song ánh, được gọi là chính tắc, từ $(E/H)/G = (E/H)/(G/H)$ lên E/G.

Cho G (tương ứng H) là một nhóm tác động lên một tập hợp E ở bên trái (tương ứng bên phải). Giả sử các tác động của G và H trên E giao hoán, nghĩa là

$$
(g.x).h = g.(x.h) \quad \text{với } g \in G, x \in E \text{ và } h \in H.
$$

Tác động của H trên E cũng là một tác động bên trái của nhóm đối $H^0$ của H. Do đó, theo § 4, no. 9, Mệnh đề 12, ánh xạ gán cho phần tử $(g, h) \in G \times H^0$ ánh xạ $x \mapsto g . x . h$ của E vào chính nó là một tác động bên trái của $G \times H^0$ trên E. Quỹ đạo của một phần tử $x \in E$ dưới tác động này là tập hợp $GxH$. Tập hợp các quỹ đạo này được ký hiệu bởi $G\|E/H$. Mặt khác, tác động của G (tương ứng H) tương thích với quan hệ liên hợp đối với tác động của H (tương ứng G) và tập hợp các quỹ đạo $G\|(E/H)$ (tương ứng $(G\|E)/H$) được đồng nhất với $G\|E/H$: trong biểu đồ

$$
\begin{array}{ccc}
& & E \\
& \swarrow_{\alpha} & \searrow_{\beta} \\
G\|E & & E/H \\
& \downarrow_{\varepsilon} & \\
& & G\|E/H \\
& \searrow_{\delta} & \swarrow_{\gamma}
\end{array}
$$

(trong đó $\alpha, \beta, \gamma, \delta, \varepsilon$ lần lượt ký hiệu các ánh xạ chính tắc lấy thương), $\gamma \circ \alpha = \delta \circ \beta = \varepsilon$.

Cho G là một nhóm và H là một nhóm con của G. Xét tác động bên phải của H trên G bởi phép dịch phải (no. 1, Ví dụ 2). Tập hợp các quỹ đạo $G/H$ là tập hợp các lớp ghép trái theo H; chú ý rằng G tác động lên $G/H$ ở bên trái theo luật $(g, xH) \mapsto gxH$ (cf. no. 5). Tương tự, tập hợp các lớp ghép phải theo H là tập hợp $H\backslash G$ các quỹ đạo của tác động bên trái của H trên G bởi phép dịch trái. Nếu K là một nhóm con của G chứa H và $\Gamma$ là một lớp ghép trái (tương ứng phải) theo H, thì $\Gamma K$ (tương ứng $K\Gamma$) là một lớp ghép trái (tương ứng phải) theo K. Ánh xạ $\Gamma \mapsto \Gamma K$ (tương ứng $\Gamma \mapsto K\Gamma$) được gọi là ánh xạ chính tắc từ $G/H$ vào $G/K$ (tương ứng từ $H\backslash G$ vào $K\backslash G$). Nó là toàn ánh.

Cho G là một nhóm và H và K là hai nhóm con của G. Cho H tác động lên G ở bên trái bởi phép dịch trái và K ở bên phải bởi phép dịch phải; hai phép toán này giao hoán, do đó cho phép ta xét tập hợp $H\backslash G/K$. Các phần tử của $H\backslash G/K$ được gọi là các lớp ghép kép của G theo H và K. Khi $K = H$, ta gọi đơn giản là các lớp ghép kép theo H. Để ánh xạ chính tắc từ $G/H$ lên $H\backslash G/H$ là một song ánh, điều kiện cần và đủ là H là một nhóm con chuẩn tắc của G.

### 5. TẬP HỢP THUẦN NHẤT

#### Định nghĩa 6 {#alg-i-s5-def-6 .statement}

*Cho G là một nhóm. Một tác động của G trên một tập hợp E được gọi là bắc cầu nếu tồn tại một phần tử $x \in E$ có quỹ đạo là E. Một G-tập hợp E được gọi là thuần nhất nếu tác động của G trên E là bắc cầu.*

Người ta cũng nói rằng G *tác động bắc cầu* trên E; hoặc E là một *tập hợp thuần nhất dưới tác động của* G. Điều đó tương đương với việc nói rằng E *khác rỗng* và rằng, với mọi phần tử $x$ và $y$ của E, tồn tại một phần tử $\alpha \in G$ sao cho $\alpha.x = y$.

#### Ví dụ {#alg-i-s5-n5-exa-1 .statement}

Nếu E là một G-tập hợp, mỗi quỹ đạo của E, với tác động cảm sinh, là một tập hợp thuần nhất dưới tác động của G.

Cho G là một nhóm và H là một nhóm con của G. Xét tập hợp $G/H$ các lớp ghép trái theo H. Nhóm G tác động lên $G/H$ ở bên trái theo $(g, xH) \mapsto gxH$. Gọi N là chuẩn tắc hóa tử của H. Nhóm N tác động lên $G/H$ ở bên phải theo $(xH, n) \mapsto xHn = xnH$. Tác động này cảm sinh trên H tác động tầm thường và do đó, chuyển qua thương, $N/H$ tác động lên $G/H$ ở bên phải. Gọi $\phi : (N/H)^0 \to S_{G/H}$ là đồng cấu tương ứng với tác động này.

#### Mệnh đề 5 {#alg-i-s5-prop-5 .statement}

*Với các ký hiệu trên, G/H là một G-tập hợp thuần nhất. Ánh xạ $\phi$ cảm sinh một đẳng cấu từ $(N/H)^0$ lên nhóm các tự đẳng cấu của G-tập hợp G/H.*

Quỹ đạo trong $G/H$ của phần tử $e = H$ là $G/H$, do đó mệnh đề đầu tiên. Bây giờ chứng minh mệnh đề thứ hai. Nếu $n \in N$ xác định ánh xạ đồng nhất trên $G/H$ bằng phép dịch phải, thì $e.n = e$, nghĩa là $H.n = H$, do đó $n \in H$. Vì vậy

N/H tác động trung thành trên G/H ở bên phải và $\phi$ là đơn ánh. Phép toán bên trái của G và phép toán bên phải của N/H trên G/H giao hoán với nhau và do đó các toán tử của N/H xác định các G-cấu xạ của G/H vào chính nó, nhất thiết là các G-đẳng cấu vì chúng song ánh. Do đó $\phi$ nhận giá trị trong nhóm $\Phi$ các G-đẳng cấu của G/H. Ta chứng minh rằng ảnh của $\phi$ là $\Phi$. Cho $f \in \Phi$. Bằng phép chuyển cấu trúc, nhóm ổn định của $f(\dot{e})$ trong G bằng nhóm ổn định của $\dot{e}$ và do đó bằng H. Cho $n \in G$ sao cho $f(\dot{e}) = n\dot{e}$. Nhóm ổn định của $n\dot{e}$ trong G là $nHn^{-1}$ (no. 2, Mệnh đề 2), do đó $nHn^{-1} = H$ và $n \in N$. Với mọi phần tử $xH$ của G/H, $f(xH) = f(x.\dot{e}) = x.f(\dot{e}) = xnH = xHn$ và $f$ trùng với ánh xạ được xác định bởi $n$.

#### Nhận xét {#alg-i-s5-n5-rem-1 .statement}

(1) Cho G là một nhóm, H là một nhóm con của G và $\phi : G \to \mathcal{S}_{G/H}$ là đồng cấu tương ứng với phép toán của G trên G/H. Hạt nhân của $\phi$ là giao của các liên hợp của H (no. 2, Mệnh đề 2). Nó cũng là nhóm con chuẩn tắc lớn nhất được chứa trong H (no. 3). Đặc biệt, G tác động trung thành trên G/H khi và chỉ khi giao của các liên hợp của H thu gọn thành $\{e\}$.

(2) Cho G là một nhóm và H và K là các nhóm con sao cho H là một nhóm con chuẩn tắc của K. K/H tác động trên G-tập hợp G/H ở bên phải và ánh xạ chính tắc từ G/H lên G/K xác định, khi chuyển qua thương, một G-tập hợp đẳng cấu $(G/H)/(K/H) \to G/K$ (xem no. 4).

#### Mệnh đề 6 {#alg-i-s5-prop-6 .statement}

*Cho G là một nhóm, E là một G-tập hợp thuần nhất, $a \in E$, H là nhóm ổn định của a và K là một nhóm con của G được chứa trong H. Tồn tại duy nhất một G-cấu xạ f từ G/K vào E sao cho $f(e.K) = a$. Nếu K = H, f là một đẳng cấu.*

Nếu f là một nghiệm, thì $f(x.K) = x.a$ với mọi x trong G, do đó có tính duy nhất; ta chứng minh sự tồn tại. Ánh xạ quỹ đạo được xác định bởi a tương thích với quan hệ tương đương $y \in xK$ trên G. Thật vậy, nếu $y = xk, k \in K$, thì
$$
y.a = xk.a = x.a.
$$
Do đó suy ra một ánh xạ f từ G/K vào H thỏa mãn $f(x.K) = x.a$ với mọi x trong G. Ánh xạ này là một G-cấu xạ và $f(K) = a$. Ánh xạ này là toàn ánh vì ảnh của nó là một tập con khác rỗng ổn định của E. Giả sử K = H và ta chứng minh rằng f là đơn ánh. Nếu $f(x.H) = f(y.H)$, thì $x.a = y.a$, do đó $x^{-1}y.a = a$ và $x^{-1}y \in H$, do đó $x.H = y.H$.

#### Định lý 1 {#alg-i-s5-thm-1 .statement}

*Cho G là một nhóm.*
(a) *Mọi G-tập hợp thuần nhất đều đẳng cấu với một G-tập hợp thuần nhất có dạng G/H, trong đó H là một nhóm con của G.*
(b) *Cho H và H' là hai nhóm con của G. Các G-tập hợp G/H và G/H' đẳng cấu với nhau khi và chỉ khi H và H' liên hợp.*

Vì một G-tập hợp thuần nhất là khác rỗng, mệnh đề (a) suy ra từ Mệnh đề 6. Ta chứng minh (b). Cho $f : G/H \to G/H'$ là một G-tập hợp đẳng cấu. Nhóm con H là nhóm ổn định của H và do đó, bằng phép chuyển cấu trúc, là nhóm ổn định của một phần tử của $G/H'$. Vì vậy các nhóm con $H$ và $H'$ liên hợp với nhau (no. 2, Mệnh đề 2). Nếu $H' = \alpha H \alpha^{-1}$, thì $H'$ là nhóm ổn định của phần tử $\alpha . H$ của $G/H$ (no. 2, Mệnh đề 2) và do đó $G/H'$ đẳng cấu với $G/H$ (Mệnh đề 6).

#### Ví dụ {#alg-i-s5-n5-exa-2 .statement}

(1) Cho $E$ là một tập hợp khác rỗng. Nhóm $S_E$ tác động bắc cầu trên $E$. Nếu $x$ và $y$ là hai phần tử của $E$, ánh xạ $\tau : E \to E$ sao cho $\tau(x) = y$, $\tau(y) = x$ và $\tau(z) = z$ với $z \neq x, y$, là một phép hoán vị của $E$. Cho $a \in E$. Nhóm ổn định của $a$ được đồng nhất với $S_F$, trong đó $F = E - \{a\}$. $G$-tập thuần nhất $E$ do đó đẳng cấu với $S_E / S_F$.

(2) Cho $E$ là một tập hợp gồm $n$ phần tử và $(p_i)_{i \in I}$ là một họ hữu hạn các số nguyên $> 0$ sao cho $\sum_i p_i = n$. Cho $X$ là tập hợp các phân hoạch $(F_i)_{i \in I}$ của $E$ sao cho $\mathrm{Card}(F_i) = p_i$ với mọi $i$. Nhóm $S_E$ tác động bắc cầu trên $X$. Nhóm ổn định $H$ của một phần tử $(F_i)_{i \in I}$ của $X$ đẳng cấu một cách chính tắc với $\prod_{i \in I} S_{F_i}$ và do đó có cấp $\prod_{i \in I} p_i!$. Áp dụng Định lý 1 và § 4, no. 4, Hệ quả của Mệnh đề 4, ta thu được một chứng minh mới cho sự kiện là

$$
\mathrm{Card}(X) = \frac{n!}{\prod_{i \in I} p_i!}
$$

Đặc biệt, lấy $I = \{1, 2, \ldots, r\}$, $E = \{1, 2, \ldots, n\}$,

$$
F_i = \{p_1 + \cdots + p_{i-1} + 1, \ldots, p_1 + \cdots + p_i\}
$$

với $1 \leq i \leq r$. Gọi $S$ là tập hợp các $\tau \in S_E$ sao cho $\tau|_{F_i}$ là tăng với $1 \leq i \leq r$. Nếu $(G_1, \ldots, G_r) \in X$ thì tồn tại duy nhất một $\tau \in S$ ánh xạ $(F_1, \ldots, F_r)$ vào $(G_1, \ldots, G_r)$. Nói cách khác, mỗi lớp ghép trái của $S_E$ theo $H$ gặp $S$ tại duy nhất một điểm.

(3) *Cho $n$ là một số nguyên $\geq 1$. Nhóm trực giao $O(n, \mathbf{R})$ tác động bắc cầu trên mặt cầu đơn vị $S_{n-1}$ trong $\mathbf{R}^n$. Nhóm ổn định của điểm $(0, \ldots, 0, 1)$ được đồng nhất với nhóm trực giao $O(n-1, \mathbf{R})$. Tập $O(n, \mathbf{R})$ thuần nhất $S_{n-1}$ do đó đẳng cấu với $O(n, \mathbf{R})/O(n-1, \mathbf{R})$.*

### 6. CÁC TẬP CHÍNH THUẦN NHẤT

#### Định nghĩa 7 {#alg-i-s5-def-7 .statement}

*Cho $G$ là một nhóm. Một phép toán của $G$ trên một tập $E$ được gọi là đơn tác nếu tồn tại một phần tử $x$ của $E$ sao cho ánh xạ quỹ đạo xác định bởi $x$ là một song ánh. Một tập $E$, cùng với một tác động trái đơn tác của $G$ trên $E$, được gọi là một tập $G$ chính thuần nhất trái (hoặc tập chính thuần nhất trái dưới $G$).*

Nói cách khác, $G$ tác động tự do và bắc cầu trên $E$, hoặc cũng có thể nói rằng tồn tại một phần tử $x \in E$ sao cho ánh xạ quỹ đạo xác định bởi $x$ là một đẳng cấu của tập $G$ của $G$ (trong đó $G$ tác động bằng phép tịnh tiến trái) lên $E$; hoặc cũng có thể nói rằng hai điều kiện sau được thỏa mãn:

(i) $E$ khác rỗng.
(ii) với mọi phần tử $x$ và $y$ của $E$, tồn tại duy nhất một phần tử $\alpha \in G$ sao cho $\alpha x = y$.

Điều kiện (ii) cũng tương đương với điều kiện sau:

(iii) ánh xạ $(\alpha, x) \mapsto (\alpha x, x)$ là một song ánh từ $G \times E$ lên $E \times E$.

Ta để cho người đọc định nghĩa các tập G chính thuần nhất phải.

#### Ví dụ {#alg-i-s5-n6-exa-1 .statement}

(1) Cho G tác động trên chính nó bằng phép tịnh tiến trái (tương ứng phải). Khi đó một cấu trúc tập G chính thuần nhất trái (tương ứng phải) được xác định trên G, đôi khi được ký hiệu là $G_s$ (tương ứng $G_d$).

(2) Cho E là một tập thuần nhất dưới một nhóm *giao hoán* G. Nếu G tác động trung thành trên E, thì E là một tập chính thuần nhất.

(3) Cho E và F là hai tập đẳng cấu với các cấu trúc cùng một loài và cho Isom(E, F) là tập các đẳng cấu từ E lên F (với các cấu trúc đã cho). Nhóm Aut(E) các tự đẳng cấu của E (với cấu trúc đã cho) tác động lên Isom(E, F) ở bên phải theo luật $(\sigma, f) \mapsto f \circ \sigma$ và Isom(E, F) là một tập Aut(E) chính thuần nhất phải. Tương tự, nhóm Aut(F) tác động lên Isom(E, F) ở bên trái theo luật $(\sigma, f) \mapsto \sigma \circ f$ và Isom(E, F) là một tập Aut(F) chính thuần nhất trái.

(4) *Một tập chính thuần nhất dưới nhóm cộng của một không gian vectơ được gọi là một *không gian affine* (xem II, § 9, no. 1).*

Nhóm các tự đẳng cấu của tập G chính thuần nhất $G_s$ (Ví dụ 1) là nhóm các phép tịnh tiến phải của G, được đồng nhất với $G^0$ (no. 5, Mệnh đề 5). Cho E là một tập G chính thuần nhất và $a$ là một phần tử của E. Ánh xạ quỹ đạo $\omega_a$ xác định bởi $a$ là một đẳng cấu của tập G $G_s$ lên E. Bằng cách chuyển cấu trúc, một đẳng cấu $\psi_a$ của $G^0$ lên Aut(E) được dẫn xuất. Cần lưu ý rằng $\psi_a$ *nói chung phụ thuộc vào a*; chính xác hơn, với $\alpha \in G$,

$$
\psi_{\alpha a} = \psi_a \circ \operatorname{Int}_{G^0}(\alpha) = \psi_a \circ \operatorname{Int}(\alpha^{-1}).
$$

Thật vậy, ký hiệu $\delta_a$ là phép tịnh tiến $x \mapsto x \alpha$ trên G,

$$
\omega_{\alpha a} = \phi \omega_a \circ \delta_\alpha
$$
và
$$
\psi_a(x) = \omega_a \circ \delta_x \circ \omega_a^{-1}, \quad x \in G,
$$
do đó
$$
\psi_{\alpha a}(x) = \omega_a \circ \delta_\alpha \circ \delta_x \circ \delta_\alpha^{-1} \circ \omega_a^{-1} = \omega_a \circ \delta_{\alpha^{-1} x \alpha} \circ \omega_a^{-1} = \psi_a(\alpha^{-1} x \alpha).
$$

### 7. CÁC NHÓM HOÁN VỊ CỦA MỘT TẬP HỮU HẠN

Nếu E là một tập hợp hữu hạn có $n$ phần tử, nhóm đối xứng $\mathfrak{S}_E$ (§ 4, no. 1) là một nhóm hữu hạn có cấp $n!$. Khi E là khoảng $\{1, n\}$ của tập hợp $\mathbf{N}$ các số tự nhiên, nhóm đối xứng tương ứng được ký hiệu là $\mathfrak{S}_n$; nhóm đối xứng của bất kỳ tập hợp nào có $n$ phần tử đều đẳng cấu với $\mathfrak{S}_n$.

#### Định nghĩa 8 {#alg-i-s5-def-8 .statement}

Cho E là một tập hợp hữu hạn, $\zeta \in \mathfrak{S}_E$ là một phép hoán vị của E và $\bar{\zeta}$ là nhóm con của $\mathfrak{S}_E$ sinh bởi $\zeta$. $\zeta$ được gọi là một chu trình nếu, dưới phép toán của $\bar{\zeta}$ trên E, tồn tại một và chỉ một quỹ đạo không thu về một phần tử duy nhất. Quỹ đạo này được gọi là giá của $\zeta$.

Cho $\zeta$ là một chu trình. Giá $\operatorname{supp}(\zeta)$ của $\zeta$ là tập hợp các $x \in E$ sao cho $\zeta(x) \neq x$.

Cấp của một chu trình $\zeta$ bằng lực lượng của giá của nó. Nhóm con $\bar{\zeta}$ sinh bởi $\zeta$ tác động bắc cầu và trung thành trên $\operatorname{supp}(\zeta)$. Vì $\zeta$ là giao hoán, $\operatorname{supp}(\zeta)$ là một tập hợp chính dưới $\bar{\zeta}$ (no. 6, Ví dụ 2) và do đó $\operatorname{Card}(\operatorname{supp}(\zeta)) = \operatorname{Card}(\bar{\zeta})$.

#### Bổ đề 1 {#alg-i-s5-lem-1 .statement}

Cho $(\zeta_i)_{i \in I}$ là một họ các chu trình có các giá từng đôi một rời nhau. Khi đó các $\zeta_i$ từng đôi một khả hoán. Đặt $\sigma = \prod_{i \in I} \zeta_i$ và $\bar{\sigma}$ là nhóm con sinh bởi $\sigma$. Khi đó $\sigma(x) = \zeta_i(x)$ với $x \in S_i, i \in I$, và $\sigma(x) = x$ với $x \notin \bigcup_{i \in I} S_i$. Ánh xạ $i \mapsto S_i$ là một song ánh của I lên tập hợp các quỹ đạo của $\bar{\sigma}$ không gồm một phần tử duy nhất.

Cho $\zeta$ và $\zeta'$ là hai chu trình có các giá mang rời nhau. Nếu
$$
x \notin \operatorname{supp}(\zeta) \cup \operatorname{supp}(\zeta'),
$$
thì $\zeta \zeta'(x) = \zeta' \zeta(x) = x$. Nếu $x$ thuộc giá mang của $\zeta$, thì $\zeta'(x) = x$, và $\zeta(x)$ thuộc giá mang của $\zeta$, do đó $\zeta \zeta'(x) = \zeta' \zeta(x) = \zeta(x)$. Tương tự, khi $x$ thuộc giá mang của $\zeta'$, thì $\zeta' \zeta(x) = \zeta \zeta'(x) = \zeta'(x)$. Suy ra $\zeta \zeta' = \zeta' \zeta$. Do đó các $\zeta_i$ từng đôi một khả hoán và, với $i \in I$ và $x \in S_i$, $\sigma(x) = \zeta_i(x) \in S_i$. Các ánh xạ $\sigma$ và $\zeta_i$ trùng nhau trên $S_i$, do đó $S_i$ ổn định dưới $\sigma$ và nhóm con của $\mathfrak{S}_{S_i}$ sinh bởi hạn chế của $\sigma$ lên $S_i$ tác động bắc cầu trên $S_i$; do đó $S_i$ là một quỹ đạo $\bar{\sigma}$. Vì các $S_i$ đều không rỗng và từng đôi một rời nhau, ánh xạ $i \mapsto S_i$ là đơn ánh. Vì $\bigcup_i S_i$ là tập hợp các $x$ sao cho $\sigma(x) \neq x$, nên mọi quỹ đạo $\bar{\sigma}$ không gồm một phần tử duy nhất đều là một trong các $S_i$.

#### Mệnh đề 7 {#alg-i-s5-prop-7 .statement}

Cho E là một tập hợp hữu hạn và $\sigma$ là một phép hoán vị của E. Tồn tại duy nhất một tập hợp hữu hạn C gồm các chu trình thỏa mãn hai điều kiện sau:

(a) các giá mang của các phần tử của C từng đôi một rời nhau;

(b) $\sigma = \prod_{\zeta \in C} \zeta$ (các phần tử của C từng đôi một khả hoán theo Bổ đề 1).

Cho $\bar{\sigma}$ là nhóm con sinh bởi $\sigma$ và S là tập hợp các quỹ đạo $\bar{\sigma}$ không gồm một phần tử duy nhất. Với $s \in S$, đặt $\zeta_s(x) = \sigma(x)$ nếu $x \in s$ và $\zeta_s(x) = x$ nếu $x \notin s$. Với mọi $s \in S$, $\zeta_s$ là một chu trình có giá mang là $s$ và $\sigma = \prod_{s \in S} \zeta_s$, như thấy được bằng cách áp dụng hai vế cho một phần tử bất kỳ của E. Tính duy nhất của C suy ra từ Bổ đề 1.

#### Định nghĩa 9 {#alg-i-s5-def-9 .statement}

*Một chu trình có cấp 2 được gọi là một phép chuyển vị.*

Cho $x$ và $y$ là hai phần tử *phân biệt* của E. Ký hiệu $\tau_{x,y}$ là phép chuyển vị duy nhất có giá mang $\{x, y\}$.

Với mọi phép hoán vị $\sigma$ của E, phép hoán vị $\sigma \cdot \tau_{x,y} \cdot \sigma^{-1}$ là một phép chuyển vị có giá mang $\{\sigma(x), \sigma(y)\}$. Do đó:

(4)
$$
\sigma \cdot \tau_{x,y} \cdot \sigma^{-1} = \tau_{\sigma(x), \sigma(y)}.
$$

Các phép chuyển vị do đó tạo thành một lớp liên hợp trong nhóm $\mathfrak{S}_E$.

#### Mệnh đề 8 {#alg-i-s5-prop-8 .statement}

*Một tập hợp hữu hạn E. Nhóm $\mathfrak{S}_E$ được sinh bởi các phép chuyển vị.*

Với mọi phép hoán vị $\sigma$, gọi $F_\sigma$ là tập hợp các $x \in E$ sao cho $\sigma(x) = x$. Ta chứng minh bằng quy nạp giảm dần theo $p$ rằng mọi phép hoán vị $\sigma$ sao cho $\mathrm{Card}(F_\sigma) = p$ đều là một tích của các phép chuyển trí. Nếu $p \geq \mathrm{Card}(E)$, phép hoán vị $\sigma$ là ánh xạ đồng nhất của E; nó là tích của họ rỗng các phép chuyển trí. Nếu $p < \mathrm{Card}(E)$, giả sử tính chất đã được chứng minh cho mọi phép hoán vị $\sigma'$ sao cho $\mathrm{Card}(F_{\sigma'}) > p$. Khi đó $E - F_\sigma \neq \varnothing$; lấy $x \in E - F_\sigma$ và $y \in \sigma(x)$. Khi đó $y \neq x$ và $y \in E - F_\sigma$. Đặt $\sigma' = \tau_{x,y} \cdot \sigma$. Tập hợp $F_{\sigma'}$ chứa $F_\sigma$ và $x$ và do đó $\mathrm{Card}(F_{\sigma'}) > \mathrm{Card}(F_\sigma) = p$. Theo giả thiết quy nạp $\sigma'$ là một tích của các phép chuyển trí và do đó $\sigma = \tau_{x,y} \cdot \sigma'$ là một tích của các phép chuyển trí.

#### Mệnh đề 9 {#alg-i-s5-prop-9 .statement}

*Cho n là một số nguyên $\geq 0$. Nhóm $\mathfrak{S}_n$ được sinh bởi các phép chuyển trí* $(\tau_{i, i+1})_{1 \leq i \leq n-1}$.

Theo Mệnh đề 8, chỉ cần chứng minh rằng mọi phép chuyển trí $\tau_{p,q}$, $1 \leq p < q \leq n$, thuộc nhóm con H được sinh bởi các $\tau_{i, i+1}$, $1 \leq i \leq n-1$. Ta chứng minh điều này bằng quy nạp theo $q-p$. Với $q-p = 1$, điều này hiển nhiên. Nếu $q-p > 1$, thì (công thức (4)) $\tau_{p,q} = \tau_{q-1,q} \tau_{p,q-1} \tau_{q-1,q}$. Theo giả thiết quy nạp $\tau_{p,q-1} \in H$ và do đó $\tau_{p,q} \in H$.

Nếu $\sigma \in \mathfrak{S}_n$, mọi cặp có thứ tự $(i, j)$ của các phần tử của $\{1, n\}$ sao cho $i < j$ và $\sigma(i) > \sigma(j)$ được gọi là một *nghịch thế* của $\sigma$. Gọi $\nu(\sigma)$ là số nghịch thế của $\sigma$.

Cho P là nhóm cộng của các ánh xạ từ $\mathbf{Z}^n$ vào $\mathbf{Z}$. Với $f \in P$ và $\sigma \in \mathfrak{S}_n$, gọi $\sigma f$ là phần tử của P được xác định bởi

(5)
$$
\sigma f(z_1, \ldots, z_n) = f(z_{\sigma(1)}, \ldots, z_{\sigma(n)}).
$$

Tác động của $\mathfrak{S}_n$ trên P được xác định như vậy là một phép toán; với mọi $\sigma, \tau \in \mathfrak{S}_n$ và $f \in P$, $\sigma f = f$ và
$$
\begin{align*}
(\tau(\sigma f))(z_1, \ldots, z_n) &= \sigma f(z_{\tau(1)}, \ldots, z_{\tau(n)}) = f(z_{\tau \sigma(1)}, \ldots, z_{\tau \sigma(n)}) \\
&= ((\tau \sigma) f)(z_1, \ldots, z_n).
\end{align*}
$$
Công thức (5) cho thấy rằng $\sigma(-f) = -\sigma f$ với $\sigma \in \mathfrak{S}_n$ và $f \in P$.

Cho $p$ là phần tử của P được xác định bởi

$$
p(z_1, \ldots, z_n) = \prod_{i < j} (z_j - z_i).
$$

#### Bổ đề 2 {#alg-i-s5-lem-2 .statement}

$p \neq 0$ và $\sigma p = (-1)^{\nu(\sigma)}$ với $\sigma \in \mathfrak{S}_n$.

$p(1, 2, \ldots, n) = \prod_{i < j} (j - i) \neq 0$ và do đó $p \neq 0$. Mặt khác, nếu $\sigma \in \mathfrak{S}_n$, thì

$$
\sigma p(z_1, \ldots, z_n) = p(z_{\sigma(1)}, \ldots, z_{\sigma(n)}) = \prod_{i < j} (z_{\sigma(j)} - z_{\sigma(i)}).
$$

Cho C là tập hợp các cặp có thứ tự $(i, j)$ sao cho $1 \leq i \leq n,\ 1 \leq j \leq n,\ i < j$. Một phép hoán vị $\theta$ được xác định trên C bằng cách đặt $\theta(i, j) = (\sigma(i), \sigma(j))$ nếu $(i, j)$ không phải là một nghịch thế, $\theta(i, j) = (\sigma(j), \sigma(i))$ nếu $(i, j)$ là một nghịch thế. Điều này suy ra $\sigma p = (-1)^{\nu(\sigma)} p$.

#### Định lý 2 {#alg-i-s5-thm-2 .statement}

*Một tập hợp hữu hạn E có một và chỉ một đồng cấu $\varepsilon$ từ $\mathfrak{S}_n$ vào nhóm nhân $\{-1, +1\}$ sao cho $\varepsilon(\tau) = -1$ với mọi phép chuyển vị $\tau$.*

Tính duy nhất suy ra từ Mệnh đề 8. Ta chứng minh sự tồn tại. Bằng cách chuyển cấu trúc, có thể giả sử rằng $E = \{1, n\}$. Với ký hiệu trên, đặt $\varepsilon(\sigma) = (-1)^{\nu(\sigma)}$. Khi đó (Bổ đề 2)

$$
\sigma(\sigma' p) = \sigma(\varepsilon(\sigma') p) = \varepsilon(\sigma') (\sigma p) = \varepsilon(\sigma') \varepsilon(\sigma) p.
$$

Mặt khác,

$$
\sigma(\sigma' p) = (\sigma \sigma') p = \varepsilon(\sigma \sigma') p.
$$

Vì $p \neq -p$, suy ra $\varepsilon(\sigma \sigma') = \varepsilon(\sigma) \varepsilon(\sigma')$ và do đó $\varepsilon$ là một đồng cấu. Bây giờ ta chứng minh rằng, với mọi phép chuyển vị $\tau$, $\varepsilon(\tau) = -1$. $\nu(\tau_{n-1, n}) = 1$, do đó $\varepsilon(\tau_{n-1, n}) = -1$. Vì mọi phép chuyển vị $\tau$ đều liên hợp với $\tau_{n-1, n}$ và nhóm $\{-1, +1\}$ là giao hoán, $\varepsilon(\tau) = \varepsilon(\tau_{n-1, n}) = -1$.

#### Định nghĩa 10 {#alg-i-s5-def-10 .statement}

*Theo ký hiệu của Định lý 2, số $\varepsilon(\sigma)$ (cũng được ký hiệu là $\varepsilon_\sigma$) được gọi là dấu của phép hoán vị $\sigma$. Hạt nhân của đồng cấu $\varepsilon$ được gọi là nhóm phản xứng của E.*

$\sigma$ được gọi là *chẵn* (resp. *lẻ*) nếu $\varepsilon(\sigma) = 1$ (resp. $\varepsilon(\sigma) = -1$). Nhóm phản xứng của E được ký hiệu là $\mathfrak{A}_E$. Nó là một nhóm con chuẩn tắc của $\mathfrak{S}_E$. Khi $E = \{1, n\}$, nó được ký hiệu đơn giản là $\mathfrak{A}_n$. Khi lực lượng $n$ của E là $\geq 2$, nó là một nhóm con có chỉ số 2 và do đó có cấp $n! / 2$. Có thể chứng minh rằng, với $n = 3$ hoặc $n \geq 5$, nhóm $\mathfrak{A}_n$ là một nhóm đơn (*xem Bài tập 16*).

#### Ví dụ {#alg-i-s5-n7-exa-1 .statement}

Nếu $\sigma$ là một chu trình có cấp $d$, thì
$$
\varepsilon(\sigma) = (-1)^{d-1}.
$$
Số nghịch thế của phép hoán vị
$$
(1, 2, 3, \ldots, d) \mapsto (d, 1, 2, \ldots, d-1)
$$
bằng $d-1$.

### Bài tập {#alg-i-s5-exercises}

Xem [các bài tập của § 5](exercises/s5/).
