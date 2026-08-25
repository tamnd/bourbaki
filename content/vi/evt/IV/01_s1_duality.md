---
book: evt
book_title: Topological Vector Spaces
chapter: IV
chapter_title: DUALITY IN TOPOLOGICAL VECTOR SPACES
section: 1
section_title: Duality
lang: vi
source: evt-i-v
pdf_pages: 0183-0196, 0229-0234
extraction: ocr
subsections:
    - "no": 1
      title: Topologies compatible with a duality
      page: 0
      pdf_page: 183
    - "no": 2
      title: Mackey topology and weakened topology on a locally convex space
      page: 4
      pdf_page: 186
    - "no": 3
      title: Transpose of a continuous linear mapping
      page: 6
      pdf_page: 188
    - "no": 4
      title: Dual of a quotient space and of a subspace
      page: 8
      pdf_page: 190
    - "no": 5
      title: Dual of a direct sum and of a product
      page: 11
      pdf_page: 193
statements: 35
exercises: 25
content_sha256: 621c016307113e02ca09012f19dc6b6f6a7361f765c10406ed57c6c11b6f9f3b
translated_from: content/en/evt/IV/01_s1_duality.md
source_content_sha256: 3595be17b3c9c8cdcadd6b2c560c42a34a50a45db1046b62b30aa9e2f9200799
translation_model: gpt-5.4-mini, gpt-5-6
translation_run: translate-vi-ad1f36fc
glossary_version: 34
glossary_terms_sha256: 92a6d1d7ce17f01eaf95c16f1f6aeccffe2d73261c65ed734e43d47d6469429e
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 1. TÍNH ĐỐI NGẪU

### 1. Các tôpô tương thích với một tính đối ngẫu

Trong mục này, E và F ký hiệu hai không gian vectơ được đặt trong tính đối ngẫu bởi một dạng song tuyến tính B (II, p. 40). Nhắc lại (II, p. 41) rằng ta đã định nghĩa hai ánh xạ tuyến tính

$$
d_B : F \to E^*, \quad s_B : E \to F^*
$$

được đặc trưng bởi hệ thức

(1)
$$
B(x, y) = \langle x, d_B(y) \rangle = \langle y, s_B(x) \rangle
$$

với $x \in E, \ y \in F$.

#### Định nghĩa 1 {#evt-iv-s1-def-1 .statement}

*Một tôpô lồi địa phương $\mathcal{T}$ trên E được gọi là tương thích với tính đối ngẫu giữa E và F nếu $d_B$ là một song ánh từ F lên không gian đối ngẫu của không gian lồi địa phương thu được khi trang bị cho E tôpô $\mathcal{T}$.*

Nếu tồn tại một tôpô $\mathcal{T}$ như vậy, thì ánh xạ $d_B$ là đơn ánh, tức là tính đối ngẫu giữa E và F là tách biệt trong F (II, p. 41).

#### Mệnh đề 1 {#evt-iv-s1-prop-1 .statement}

(i) *Các tập con lồi đóng của E là như nhau đối với mọi tôpô lồi địa phương trên E tương thích với tính đối ngẫu giữa E và F.*
(ii) *Các tập con bị chặn của E là như nhau đối với mọi tôpô lồi địa phương trên E tương thích với tính đối ngẫu giữa E và F.*

Cho $\mathcal{T}$ là một tôpô trên E tương thích với tính đối ngẫu giữa E và F, do đó mịn hơn $\sigma(E, F)$. Nếu một tập con lồi của E đóng đối với $\mathcal{T}$, thì nó là giao của các nửa không gian thực đóng (II, p. 38, hệ quả 1), do đó nó đóng đối với $\sigma(E, F)$. Điều này chứng minh (i). Mệnh đề (ii) đã được chứng minh ở hệ quả 3 của III, p. 27.

Ký hiệu $F_\sigma$ là không gian vectơ F được trang bị tôpô yếu $\sigma(F, E)$. Khi đó ánh xạ tuyến tính $s_B$ ánh xạ E lên không gian đối ngẫu $(F_\sigma)'$ của $F_\sigma$ (II, p. 43, mệnh đề 3). Cho $\mathfrak{S}$ là một họ các tập con bị chặn của $F_\sigma$. Nói một cách lạm dụng, ảnh ngược qua $s_B$ của tôpô $\mathfrak{S}$ trên $(F_\sigma)'$ được gọi là tôpô $\mathfrak{S}\text{-tôpô trên } E$. Nó được xác định bởi họ các nửa chuẩn

$$
p_A(x) = \sup_{y \in A} |B(x, y)|,
$$

trong đó A chạy qua $\mathfrak{S}$. Đặc biệt, khi $\mathfrak{S}$ là họ các tập con hữu hạn của F, thì tôpô $\mathfrak{S}$ chính xác là tôpô yếu $\sigma(E, F)$.

#### Định nghĩa 2 {#evt-iv-s1-def-2 .statement}

*Cho E và F là hai không gian trong tính đối ngẫu. Tôpô Mackey trên E, ký hiệu bởi $\tau(E, F)$, được định nghĩa là tôpô $\mathfrak{S}$ trên E, trong đó $\mathfrak{S}$ là họ tất cả các tập con của F có ảnh trong $E^*$ (qua $d_B$) là lồi, cân bằng và compact đối với $\sigma(E^*, E)$.*

Khi tính đối ngẫu giữa E và F là tách biệt trong F, thì $d_B$ là đơn ánh và tôpô $\sigma(F, E)$ trên F là ảnh ngược qua $d_B$ của tôpô $\sigma(E^*, E)$ trên $E^*$. Trong trường hợp này, $\mathfrak{S}$ gồm tất cả những tập con của F là lồi, cân bằng và compact đối với $\sigma(F, E)$.

Nói chung, nếu $F_1 = d_B(F) \subset E^*$, và nếu ta ký hiệu $(x, y_1) \mapsto B_1(x, y_1)$ là hạn chế của dạng song tuyến tính chính tắc $(x, x^*) \mapsto \langle x, x^* \rangle$ lên $E \times F_1$, thì E và $F_1$ được đặt trong tính đối ngẫu bởi $B_1$, và tính đối ngẫu này là tách biệt trong $F_1$, vì theo định nghĩa ta có $B(x, y) = B_1(x, d_B(y))$, định nghĩa 2 cho thấy $\tau(E, F) = \tau(E, F_1)$.

#### Nhận xét 1 {#evt-iv-s1-n1-rem-1 .statement}

— Cho A là một tập con lồi compact của một không gian lồi địa phương Hausdorff G, và cho $\tilde{A}$ là bao lồi cân bằng đóng của A. Khi trường K là $\mathbf{R}$, tập $\tilde{A}$ là bao lồi đóng của $A \cup (-A)$; khi K là $\mathbf{C}$, tập $\tilde{A}$ được chứa trong bao lồi đóng của $2A \cup (-2A) \cup (2iA) \cup (-2iA)$. Do đó (II, p. 14, mệnh đề 15), $\tilde{A}$ là compact.

Chúng tôi suy ra, đặc biệt, rằng khi song đôi giữa E và F là phân tách trong F, *tôpô Mackey $\tau(E, F)$ cũng là tôpô $\mathfrak{S}'$, trong đó $\mathfrak{S}'$ là tập hợp tất cả các tập con lồi của F compact đối với $\sigma(F, E)$*. Theo một cách tương tự, ta định nghĩa tôpô Mackey $\tau(F, E)$ trên F.

**Định lý 1 (Mackey).** — *Cho E và F là hai không gian đối ngẫu; giả sử rằng song đôi là phân tách trong F. Để một tôpô lồi địa phương $\mathcal{T}$ trên E tương thích với song đôi giữa E và F, điều kiện cần và đủ là $\mathcal{T}$ mịn hơn tôpô $\sigma(E, F)$ và thô hơn tôpô Mackey $\tau(E, F)$.*

Đồng nhất F với ảnh của nó trong $E^*$ dưới $d_B$. Ký hiệu $\mathfrak{S}_0$ là tập hợp tất cả các tập con của F vừa lồi, vừa cân bằng và compact đối với $\sigma(F, E)$. Theo định nghĩa, $\tau(E, F)$ là tôpô $\mathfrak{S}_0$ trên E, do đó mịn hơn $\sigma(E, F)$.

#### Bổ đề 1 {#evt-iv-s1-lem-1 .statement}

*Không gian con F của E* gồm tất cả các dạng tuyến tính trên E liên tục đối với $\tau(E, F)$.

Mọi phần tử của F đều là một ánh xạ liên tục đối với $\sigma(E, F)$, do đó đối với $\tau(E, F)$.

Ngược lại, lấy $f \in E^*$ liên tục đối với $\tau(E, F)$. Tồn tại một lân cận U của 0 trong E (đối với $\tau(E, F)$), sao cho $|f| \leq 1$ trên U; ta có thể giả sử rằng tồn tại một tập $A \in \mathcal{S}_0$ sao cho $U = A^\circ$. Nói cách khác, $f$ thuộc vào lưỡng cực $A^{\circ\circ}$ của A đối với song đôi giữa $E^*$ và E. Nhưng tôpô $\sigma(F, E)$ trên F được cảm sinh bởi $\sigma(E^*, E)$; do đó A lồi, cân bằng và compact đối với $\sigma(E^*, E)$, và định lý về các lưỡng cực (II, p. 44, định lý 1) suy ra đẳng thức $A = A^{\circ\circ}$. Vì vậy ta có $f \in F$, từ đó suy ra bổ đề.

#### Bổ đề 2 {#evt-iv-s1-lem-2 .statement}

*Cho $\mathcal{T}$ là một tôpô lồi địa phương trên E sao cho mọi dạng tuyến tính trên E liên tục đối với $\mathcal{T}$ đều thuộc F. Khi đó $\mathcal{T}$ thô hơn $\tau(E, F)$.*

*Cho $\mathcal{U}$ là tập hợp các lân cận lồi, cân bằng của 0 đối với $\mathcal{T}$. Cho $\mathcal{S}$ là tập hợp các cực của các phần tử của $\mathcal{U}$ trong F. Theo hệ quả 2 của III, p. 17, ta có $\mathcal{S} \subset \mathcal{S}_0$, và theo hệ quả 1 của mệnh đề 7 của III, p. 19, $\mathcal{T}$ đồng nhất với tôpô $\mathcal{S}'$, trong đó $\mathcal{S}'$ là tập hợp các cực của các tập của $\mathcal{U}$ trong đối ngẫu $E'$ của E. Nhưng theo giả thiết, $E' \subset F$, do đó mọi tập của $\mathcal{S}'$ đều được chứa trong một tập của $\mathcal{S}$; và bổ đề được suy ra.*

Cho $\mathcal{T}$ là một tôpô trên E tương thích với song đôi giữa E và F. Khi đó $\mathcal{T}$ thô hơn $\tau(E, F)$ theo bổ đề 2, và hiển nhiên $\mathcal{T}$ mịn hơn $\sigma(E, F)$. Ngược lại, F là đối ngẫu của E đối với tôpô $\tau(E, F)$ (bổ đề 1) và đối với tôpô $\sigma(E, F)$ (II, p. 43, mệnh đề 3), do đó cũng là đối ngẫu của E đối với mọi tôpô trung gian giữa $\tau(E, F)$ và $\sigma(E, F)$.

#### Hệ quả {#evt-iv-s1-n1-cor-1 .statement}

*Cho p là một bán chuẩn trên E. Các điều kiện sau là tương đương :*

(i) *p liên tục đối với tôpô $\tau(E, F)$;*
(ii) *mọi dạng tuyến tính f trên E, sao cho $|f| \leq p$, đều xuất phát từ một phần tử của F.*

(i) $\Rightarrow$ (ii) : nếu p liên tục đối với $\tau(E, F)$, mọi dạng tuyến tính f trên E sao cho $|f| \leq p$ đều liên tục đối với $\tau(E, F)$, do đó xuất phát từ một phần tử của F theo bổ đề 1.

(ii) $\Rightarrow$ (i) : cho $\mathcal{T}$ là tôpô trên E do nửa chuẩn p xác định. Nếu điều kiện (ii) được thỏa mãn, các dạng tuyến tính trên E liên tục đối với $\mathcal{T}$ thuộc F. Theo bổ đề 2, $\mathcal{T}$ thô hơn $\tau(E, F)$, do đó p liên tục đối với $\tau(E, F)$.

#### Nhận xét 2 {#evt-iv-s1-n1-rem-2 .statement}

*Cho K là một tập con lồi của F, compact đối với tôpô yếu $\sigma(F, E)$ và $\mu$ là một độ đo dương trên K. Đặt*

$$
p(x) = \int_K |B(x, y)| \, d\mu(y)
$$

*đối với mọi $x \in E$. Rõ ràng p là một nửa chuẩn. Hơn nữa, với mọi $x \in E$, quan hệ « $|B(x, y)| \leq 1$ với mọi $y \in K$ » suy ra $p(x) \leq \mu(K)$. Điều đó chứng tỏ rằng nửa chuẩn p trên E liên tục đối với tôpô Mackey $\tau(E, F)$. \*

#### Ví dụ {#evt-iv-s1-n1-exa-1 .statement}

Cho G là một không gian lồi địa phương và G' là đối ngẫu của nó. Trên G', tôpô yếu $\sigma(G', G)$ và tôpô hội tụ compact lồi (III, p. 14) tương thích với đối ngẫu giữa G' và G. Nói chung, tôpô mạnh và tôpô hội tụ compact trên G' không tương thích với đối ngẫu giữa G' và G. Tuy nhiên, hãy nhớ rằng khi G là Hausdorff và gần đầy đủ, tôpô hội tụ compact trên G' trùng với tôpô hội tụ compact lồi (III, p. 8), do đó tương thích với đối ngẫu giữa G' và G.

#### Định nghĩa 3 {#evt-iv-s1-def-3 .statement}

*Cho E và F là hai không gian vectơ đối ngẫu, và $\mathcal{T}$ là họ các tập con của F bị chặn đối với $\sigma(F, E)$. Khi đó tôpô $\mathcal{T}$ trên F được ký hiệu là $\beta(E, F)$.*

Tương tự, ta định nghĩa tôpô $\beta(F, E)$ trên F. Dễ thấy rằng tôpô $\beta(E, F)$ đồng nhất với $\beta(E, F/E^\circ)$, và ta có thể rút về trường hợp đối ngẫu giữa E và F phân biệt trên F.

*Nhận xét. —* 3) Ký hiệu $E_\sigma$ không gian E được trang bị tôpô $\sigma(E, F)$. Các thùng (III, p. 24) trong $E_\sigma$ là các tập con của E lồi, cân bằng, đóng và hấp thụ đối với $\sigma(E, F)$. Đó chẳng qua là các tập cực của các tập con của F lồi, cân bằng và bị chặn đối với $\sigma(F, E)$. Do đó, họ tất cả các thùng trong $E_\sigma$ là một hệ cơ bản các lân cận của 0 đối với tôpô $\beta(E, F)$ trong E. Nói cách khác, một nửa chuẩn trên E liên tục đối với $\beta(E, F)$ khi và chỉ khi nó nửa liên tục dưới đối với $\sigma(E, F)$ (*xem* III, p. 24, mệnh đề 1).

4) Cho $\mathcal{T}$ là một tôpô trên E tương thích với đối ngẫu giữa E và F. Theo mệnh đề 1, (ii) của IV, p. 1, tôpô $\beta(F, E)$ trên F chính là tôpô mạnh trên F, khi F được đồng nhất với đối ngẫu của E (với tôpô $\mathcal{T}$).

5) Tôpô $\beta(E, F)$ trên E mịn hơn $\tau(E, F)$. Nói chung, nó không tương thích với đối ngẫu giữa E và F (*xem* tuy nhiên § 2). Đặc biệt, một tập con của E bị chặn đối với $\sigma(E, F)$ không nhất thiết bị chặn đối với $\beta(E, F)$.

### 2. Tôpô Mackey và tôpô yếu trên một không gian lồi địa phương

Cho E là một không gian lồi địa phương và E' là đối ngẫu của nó. Ta đặt E và E' trong đối ngẫu với nhau bằng dạng song tuyến tính chính tắc $(x, x') \mapsto \langle x, x' \rangle$ trên $E \times E'$. Đối ngẫu này phân biệt trên E'. Ta sẽ xét ba tôpô trên E tương thích với đối ngẫu giữa E và E' :

a) tôpô đã cho trên E, mà ta sẽ gọi là *tôpô ban đầu*, khi nào dễ gây nhầm lẫn;

b) tôpô $\sigma(E, E')$, gọi là *tôpô yếu* trên E;

c) tôpô $\tau(E, E')$, gọi là *tôpô Mackey* trên E.

Tôpô ban đầu mịn hơn tôpô yếu và thô hơn tôpô Mackey; hơn nữa, ba tôpô này có thể phân biệt (IV, p. 49, bài tập 8).

Theo mệnh đề 1 của IV, p. 1, ba tôpô này có cùng các tập lồi đóng, cùng các thùng, cùng các tập bị chặn và cùng các bornology thích nghi. Đặc biệt :

#### Mệnh đề 2 {#evt-iv-s1-prop-2 .statement}

*Cho E là một không gian lồi địa phương, và cho A là một tập con lồi của E (ví dụ, một không gian con vectơ của E). Bao đóng của A là như nhau đối với tôpô ban đầu và tôpô yếu của E.*

#### Nhận xét 1 {#evt-iv-s1-n2-rem-1 .statement}

Để một họ $(x_i)_{i \in I}$ các phần tử của E là toàn (tương ứng độc lập tôpô) đối với tôpô ban đầu, cần và đủ nó cũng như vậy đối với tôpô yếu; điều này suy ra từ mệnh đề 2. Do đó ta có thể áp dụng các tiêu chuẩn của II, p. 43.

#### Nhận xét 2 {#evt-iv-s1-n2-rem-2 .statement}

Cho $\mathcal{T}_1$ và $\mathcal{T}_2$ là hai tôpô lồi địa phương trên E, tương thích với đối ngẫu giữa E và $E'$, với $\mathcal{T}_1$ mịn hơn $\mathcal{T}_2$. Khi đó mọi lân cận của 0 đối với $\mathcal{T}_1$, nếu lồi và đóng đối với $\mathcal{T}_1$, thì cũng đóng đối với $\mathcal{T}_2$ theo mệnh đề 1 của IV, p. 1. Do đó (GT, II, § 3, No. 3, hệ quả) mọi tập con của E đầy đủ đối với $\mathcal{T}_2$ cũng đầy đủ đối với $\mathcal{T}_1$.

Đặc biệt, mọi tập con của E đầy đủ đối với tôpô yếu đều đầy đủ đối với tôpô ban đầu, và mọi tập con của E đầy đủ đối với tôpô ban đầu thì cũng như vậy đối với tôpô Mackey. Nếu E nửa đầy đủ đối với tôpô yếu, thì nó cũng như vậy đối với mọi tôpô tương thích với đối ngẫu giữa E và $E'$. Nếu nó nửa đầy đủ đối với tôpô ban đầu, thì nó cũng như vậy đối với tôpô Mackey.

#### Nhận xét 3 {#evt-iv-s1-n2-rem-3 .statement}

Giả sử E là Hausdorff (đối với tôpô ban đầu). Cho A là một tập con của E đóng và bị chặn đối với $\sigma(E, E')$, do đó cũng đối với mọi tôpô tương thích với đối ngẫu giữa E và $E'$. Vì A là tiền compact đối với $\sigma(E, E')$ (III, p. 3, Nhận xét 5), việc giả sử rằng A là *compact* đối với $\sigma(E, E')$ tương đương với việc A là *đầy đủ* đối với $\sigma(E, E')$.

Do đó, dựa vào nhận xét 2, ta thấy rằng :

#### Mệnh đề 3 {#evt-iv-s1-prop-3 .statement}

*Giả sử E là Hausdorff, và $E'$ là đối ngẫu của nó. Mọi tập con của E tiền compact đối với tôpô ban đầu và compact đối với $\sigma(E, E')$, đều compact đối với tôpô ban đầu.*

#### Nhận xét 4 {#evt-iv-s1-n2-rem-4 .statement}

Tôpô $\beta(E, E')$ (IV, p. 4, def. 3) mịn hơn tôpô Mackey. Nếu $\beta(E, E')$ phân biệt với $\tau(E, E')$, thì nó không tương thích với đối ngẫu giữa E và $E'$. Không gian E là thùng nếu và chỉ nếu tôpô ban đầu bằng $\beta(E, E')$ (III, p. 24).

#### Mệnh đề 4 {#evt-iv-s1-prop-4 .statement}

*Cho E là một không gian lồi địa phương. Tôpô Mackey trên E trùng với tôpô ban đầu trong mỗi trường hợp sau :*

a) E là thùng;
b) E là sinh chuẩn;
c) E đo được.

Trước hết ta nhận xét rằng tôpô Mackey trên E trùng với tôpô ban đầu nếu và chỉ nếu mọi tập con lồi của $E'$ compact đối với $\sigma(E', E)$ đều liên tục đều. Điều này chắc chắn xảy ra nếu E là thùng (III, p. 24, hệ quả).

Giả sử E là sinh chuẩn; gọi V là một lân cận lồi và cân bằng của 0 trong E đối với tôpô $\tau(E, E')$. Gọi B là một tập con của E, bị chặn đối với tôpô ban đầu. Vì B bị chặn đối với tôpô Mackey, V hút B, và vì E là sinh chuẩn, V là một lân cận của 0 đối với tôpô ban đầu.

Trong trường hợp c), không gian E là sinh chuẩn (III, p. 12, prop. 2).

### 3. Chuyển vị của một ánh xạ tuyến tính liên tục

Trong tiết này, $E_1$ và $E_2$ biểu thị hai không gian lồi địa phương, với các đối ngẫu tương ứng $E'_1$ và $E'_2$.

Cho $u$ là một ánh xạ tuyến tính từ $E_1$ vào $E_2$. Để $u$ liên tục khi $E_1$ và $E_2$ được trang bị các tôpô yếu, điều kiện cần và đủ là $f \circ u$ thuộc $E'_1$ với mọi $f \in E'_2$; đây là trường hợp nếu $u$ liên tục. Khi đó ánh xạ tuyến tính $f \mapsto f \circ u$ từ $E'_2$ vào $E'_1$ được gọi là chuyển vị của $u$ và được ký hiệu bởi $^t u$.

#### Mệnh đề 5 {#evt-iv-s1-prop-5 .statement}

*Cho $u$ là một ánh xạ tuyến tính liên tục từ $E_1$ vào $E_2$.*

(i) *Nếu $E_1$ và $E_2$ là Hausdorff thì $u$ là đơn ánh khi và chỉ khi ảnh của $^t u$ là trù mật trong $E'_1$ đối với tôpô yếu $\sigma(E'_1 : E_1)$.*

(ii) *Để $^t u$ là đơn ánh, điều kiện cần và đủ là ảnh của $u$ là trù mật trong $E_2$.*

Một không gian con vectơ của $E_2$ là trù mật đối với tôpô ban đầu khi và chỉ khi nó trù mật đối với tôpô yếu (IV, p. 4, prop. 2). Mệnh đề 5 khi đó suy ra từ II, p. 47, hệ quả 2.

#### Mệnh đề 6 {#evt-iv-s1-prop-6 .statement}

*Cho $u$ là một ánh xạ tuyến tính từ $E_1$ vào $E_2$ liên tục đối với các tôpô suy yếu. Với $i = 1, 2$, đặt $\mathfrak{S}_i$ là một họ các tập bị chặn của $E_i$. Để cho $^t u$ là một ánh xạ liên tục từ $(E'_2)_{\mathfrak{S}_2}$ vào $(E'_1)_{\mathfrak{S}_1}$, điều kiện cần và đủ là, với mọi tập $A \in \mathfrak{S}_1$, tồn tại các tập $A_1, ..., A_n$ trong $\mathfrak{S}_2$ và một số thực $\lambda > 0$ sao cho $\lambda \cdot u(A)$ được chứa trong bao lồi cân bằng đóng của $A_1 \cup ... \cup A_n$\footnote{Nói cách khác, $u(\mathfrak{S}_1)$ được chứa trong bôrnôlôgi thích nghi nhỏ nhất chứa $\mathfrak{S}_2$ (III, p. 3).}.*

Đây là hệ quả ngay lập tức của mệnh đề 2 của III, p. 15.

#### Hệ quả {#evt-iv-s1-n3-cor-1 .statement}

*Cho $u$ là một ánh xạ tuyến tính liên tục từ $E_1$ vào $E_2$. Khi đó $^t u$ liên tục khi các đối ngẫu $E'_i$ được gán các tôpô sau:*
a) *các tôpô yếu $\sigma(E'_i, E_i)$;*
b) *các tôpô mạnh $\beta(E'_i, E_i)$;*
c) *các tôpô Mackey $\tau(E'_i, E_i)$;*
d) *các tôpô của hội tụ tiền compact.*
*Hơn nữa, nếu $E_2$ là Hausdorff, thì $^t u$ liên tục khi các đối ngẫu $E'_i$ được gán:*
e) *các tôpô của hội tụ compact* (resp. *compact lồi*).

Điểm duy nhất cần chứng minh là trường hợp c), khi các tôpô của $E_1$ và $E_2$ không nhất thiết là Hausdorff. Khi đó với mọi dạng tuyến tính $f \in E'_1*$, $f \circ ^t u$ là một dạng tuyến tính trên $E'_2$; do đó có một ánh xạ tuyến tính $v : E'_1* \to E'_2*$ liên tục đối với các tôpô $\sigma(E'_1*, E'_1)$ và $\sigma(E'_2*, E'_2)$ và sao cho $d_{B_2} \circ u = v \circ d_{B_1}$, trong đó $d_{B_i}$ là ánh xạ chính tắc từ $E_i$ vào $E'_i*$ ($i = 1, 2$). Do đó, nếu $A$ là một tập con của $E_1$ sao cho $d_{B_1}(A)$ là lồi, cân bằng và compact đối với $\sigma(E'_1*, E'_1)$ thì $d_{B_2}(u(A)) = v(d_{B_1}(A))$ là lồi, cân bằng và compact đối với $\sigma(E'_2*, E'_2)$ vì các tôpô $\sigma(E'_1*, E'_1)$ và $\sigma(E'_2*, E'_2)$ là Hausdorff.

#### Mệnh đề 7 {#evt-iv-s1-prop-7 .statement}

— Cho $u : E_1 \to E_2$ là một ánh xạ tuyến tính. Giả sử rằng $u$ liên tục đối với các tôpô suy yếu của $E_1$ và $E_2$.

(i) Ánh xạ $u$ liên tục nếu $E_1$ và $E_2$ được gán các tôpô Mackey của chúng.

(ii) Nếu $E_1$ là bornological hoặc barrelled, thì $u$ liên tục đối với các tôpô ban đầu của $E_1$ và $E_2$.

(iii) Để $u$ liên tục đối với các tôpô ban đầu của $E_1$ và $E_2$, điều kiện cần và đủ là ảnh qua $'u$ của mọi tập con đẳng liên tục của $E_2'$ là đẳng liên tục trong $E_1'$.

Giả thiết suy ra rằng $'u$ liên tục đối với các tôpô yếu $\sigma(E_2', E_2)$ và $\sigma(E_1', E_1)$ (II, p. 46, hệ quả) do đó ảnh qua $'u$ của một tập con lồi, cân bằng và compact đối với $\sigma(E_2', E_2)$ là lồi, cân bằng và compact đối với $\sigma(E_1', E_1)$, hai tôpô $\sigma(E_2', E_2)$ và $\sigma(E_1', E_1)$ đều là Hausdorff. Do đó, mệnh đề (i) suy ra từ GT, X, § 1, No. 4, mệnh đề 3, b). Mệnh đề (ii) là hệ quả của (i) : vì, nếu $E_1$ là bornôlogic hoặc barrelled, tôpô ban đầu của nó là tôpô Mackey, và tôpô Mackey của $E_2$ mịn hơn tôpô ban đầu của $E_2$. Cuối cùng, tôpô ban đầu của $E_i$ là tôpô hội tụ đều trên các tập con đẳng liên tục của $E_i'$ (III, p. 19, hệ quả 1 của mệnh đề 7). Điều này chứng minh (iii).

#### Hệ quả {#evt-iv-s1-n3-cor-2 .statement}

— *Giả sử $E_1$ là một không gian chuẩn. Cho $u$ là một ánh xạ tuyến tính từ $E_1$ vào $E_2$. Các tính chất sau là tương đương :*

a) $u$ liên tục;

b) $u$ liên tục đối với các tôpô suy yếu;

c) ảnh của quả cầu đơn vị trong $E_1$ qua $u$ bị chặn trong $E_2$;

d) với mọi dãy $(x_n)$ các điểm của $E_1$ tiến tới 0 đối với tôpô ban đầu, dãy $(u(x_n))$ bị chặn đối với tôpô suy yếu của $E_2$.

Vì $E_1$ là bornôlogic nên tính tương đương của a) và b) suy ra từ mệnh đề 7; tính tương đương của a) và c) là ngay lập tức. Tính tương đương của a) và d) suy ra từ mệnh đề 1 của IV, p. 1, và từ mệnh đề 1 của III, p. 11.

#### Mệnh đề 8 {#evt-iv-s1-prop-8 .statement}

— (i) Cho $E$ là một không gian chuẩn, với đối ngẫu $E'$. Với mọi $x \in E$, ta có

$$
\|x\| = \sup_{x' \in E', \|x'\| \leq 1} |\langle x, x' \rangle|.
$$

(ii) Cho $E_1$ và $E_2$ là hai không gian chuẩn và $u$ là một ánh xạ tuyến tính liên tục từ $E_1$ vào $E_2$. Ta có

$$
\|u\| = \|t u\|.
$$

Cho $x \in E$. Với mọi $x' \in E'$ thỏa mãn $\|x'\| \leq 1$, ta có

$$
|\langle x, x' \rangle| \leq \|x\| \cdot \|x'\| \leq \|x\|.
$$

Theo định lý Hahn-Banach (II, p. 23, hệ quả 2), tồn tại một phần tử $x'$ trong $E'$ sao cho $\|x'\| \leq 1$ và $\langle x, x' \rangle = \|x\|$. Điều này chứng minh (i).

Bây giờ chứng minh (ii). Theo công thức (3) và định nghĩa của chuyển vị, ta có

$$
\|^{t}u\| = \sup_{\|y'\| \leq 1} \|^{t}u(y')\| = \sup_{\|y'\| \leq 1, \|x\| \leq 1} |\langle x, ^{t}u(y') \rangle|
= \sup_{\|x\| \leq 1, \|y'\| \leq 1} |\langle u(x), y' \rangle| = \sup_{\|x\| \leq 1} \|u(x)\| = \|u\|.
$$

#### Nhận xét 1 {#evt-iv-s1-n3-rem-1 .statement}

Công thức (3) là một trường hợp riêng của (4), tương ứng với ánh xạ tuyến tính $\lambda \mapsto \lambda x$ từ K vào E.
2) Đặt $B(x, y') = \langle u(x), y' \rangle = \langle x, ^{t}u(y') \rangle$ với $x \in E_1,\ y' \in E'_2$. Chứng minh ở trên cho thấy B là một dạng song tuyến tính liên tục trên $E_1 \times E'_2$, với chuẩn (GT, X, § 3, No. 2) bằng $\|u\|$.

#### Hệ quả {#evt-iv-s1-n3-cor-3 .statement}

— *Giả sử $\dot{E}$ là một không gian chuẩn thỏa mãn tiên đề đếm được thứ nhất. Tồn tại một tập con đếm được D của $E' - \{0\}$ sao cho ta có*

$$
\|x\| = \sup_{\xi \in D} |\langle x, \xi \rangle| / \|\xi\|
$$

*đối với mọi* $x \in E$.

Cho B' là quả cầu đơn vị của đối ngẫu $E'$ của E với tôpô yếu $\sigma(E', E)$ được gán cho nó. Khi đó B' là một không gian compact khả métr hóa (III, p. 19, hệ quả 2); do đó tồn tại một tập con trù mật đếm được D' trong B'. Đặt $D = D' \cap (E' - \{0\})$. Cho $x \in E$; ánh xạ $x' \mapsto \langle x, x' \rangle$ từ B' vào K là liên tục, do đó

$$
\sup_{x' \in B'} |\langle x, x' \rangle| = \sup_{\xi \in D'} |\langle x, \xi \rangle| \leq \sup_{\xi \in D} |\langle x, \xi \rangle| / \|\xi\| \leq \|x\|.
$$

Công thức (5) bây giờ suy ra từ (3).

### 4. Đối ngẫu của một không gian thương và của một không gian con

Trong suốt mục này, E ký hiệu một không gian lồi địa phương, M là một không gian con vectơ của E, và $M^\circ$ là tập triệt tiêu của M trong đối ngẫu $E'$ của E. Cho $p$ là ánh xạ chính tắc từ E lên $E/M$; khi đó $^{t}p$ là đơn ánh, có ảnh là $M^\circ$, do đó xác định một đẳng cấu không gian vectơ (không tôpô)

$$
\pi : (E/M)' \to M^\circ .
$$

Tương tự, cho $i$ là đơn ánh chính tắc từ M vào E. Khi đó $^{t}i$ là toàn ánh (II, p. 24, mệnh đề 2); hạt nhân của nó bằng $M^\circ$, và ta được một đẳng cấu không gian vectơ (không tôpô)

$$
i : E'/M^\circ \to M'.
$$

#### Mệnh đề 9 {#evt-iv-s1-prop-9 .statement}

— (i) *Để một tập con A của* $(E/M)'$ *là đều liên tục, cần và đủ rằng* $\pi(A)$ *là một tập con đều liên tục của* $E'$.

(ii) Cho $\mathfrak{S}$ là một tập các tập con bị chặn của E, và $\mathfrak{S}_1$ là tập các ảnh của những tập con $A \in \mathfrak{S}$ trong $E/M$. Khi đó $\pi$ là một đẳng cấu từ $(E/M)'_{\mathfrak{S}_1}$ lên $M^\circ$, trong đó $M^\circ$ được gán tôpô cảm sinh bởi tôpô của $E'_{\mathfrak{S}}$.

(iii) Giả sử $E$ là một không gian có chuẩn thì $\pi$ là một đẳng cự từ không gian có chuẩn $(E/M)'$ lên không gian con có chuẩn $M^\circ$ của $E'$.

Cho $A$ là một tập con của $(E/M)'$ và $B = {}^t p(A) \subset E'$. Đặt
$$
q(\xi) = \sup_{\xi' \in A} |\langle \xi, \xi' \rangle|
$$
với mọi $\xi \in E/M$. Để $A$ là đều liên tục, cần và đủ rằng ánh xạ $q$ từ $E/M$ vào $\overline{\mathbf{R}}_+$ là một nửa chuẩn liên tục. Điều này suy ra rằng $q \circ p$ là một nửa chuẩn liên tục trên $E$ (II, p. 27, mệnh đề 5, (ii)). Vì ta có
$$
(q \circ p)(x) = \sup_{x' \in B} |\langle x, x' \rangle|
$$
với mọi $x \in E$, điều đó lại suy ra rằng $B$ là đều liên tục trong $E'$, và (i) suy ra.

Cho $A \in \mathfrak{S}$ và cho $f$ là một dạng tuyến tính liên tục trên $E/M$. Với mọi $\lambda \in \mathbf{R}_+$, ta có $|f| \leq \lambda$ trên $p(A)$ khi và chỉ khi $|{}^t p(f)| \leq \lambda$ trên $A$; do đó (ii).

Sau cùng ta chứng minh (iii). Cho $y'$ thuộc $(E/M)'$. Một phần tử của $E/M$ có chuẩn $< 1$ nếu và chỉ nếu nó là ảnh qua $p$ của một phần tử có chuẩn $< 1$ trong $E$. Do đó
$$
\begin{align*}
\|y'\| &= \sup_{y \in E/M, \|y\| < 1} |\langle y, y' \rangle| = \sup_{x \in E, \|x\| < 1} |\langle p(x), y' \rangle| \\
&= \sup_{x \in E, \|x\| < 1} |\langle x, {}^t p(y') \rangle| = \|{}^t p(y')\|,
\end{align*}
$$
và ${}^t p$ cảm sinh một đẳng cự từ $(E/M)'$ lên $M^\circ$.

#### Mệnh đề 10 {#evt-iv-s1-prop-10 .statement}

— (i) Để một tập con $A$ của $M'$ là đều liên tục, cần và đủ rằng nó là ảnh qua ${}^t i$ của một tập con đều liên tục của $E'$.

(ii) Giả sử $M$ là đóng trong $E$. Cho $\mathfrak{S}$ là một họ phủ của $E$ gồm các tập con bị chặn và cho $\mathfrak{S}_1$ là tập các tập con của $M$ có dạng $M \cap A$ với $A$ thuộc $\mathfrak{S}$. Ánh xạ tuyến tính song ánh $i$ từ $E'_{\mathfrak{S}}/M^\circ$ lên $M'_{\mathfrak{S}_1}$ là liên tục. Nó là một song ánh tôpô nếu $\mathfrak{S}$ là một tập có hướng đối với quan hệ $\subset$ và gồm các tập đóng, lồi và compact đối với $\sigma(E, E')$.

(iii) Nếu giả sử $E$ có chuẩn, thì $i$ là một đẳng cự từ $E'/M^\circ$ lên $M'$.

Ảnh qua ${}^t i$ của một tập con đều liên tục của $E'$ là một tập con đều liên tục của $M'$ (IV, p. 7, mệnh đề 7). Ngược lại, cho $A$ là một tập con đều liên tục của $M'$. Tôpô của $M$ được xác định bởi tập các hạn chế lên $M$ của các nửa chuẩn liên tục trên $E$. Do đó tồn tại một nửa chuẩn liên tục $p$ trên $E$ sao cho $|f(x)| \leq p(x)$ với mọi $f \in A$ và với mọi $x \in M$. Cho $B$ là tập tất cả các dạng tuyến tính $g$ trên $E$ sao cho $|g| \leq p$ và sao cho hạn chế của nó lên $M$ thuộc $A$. Tập $B$ đều liên tục trong $E'$; theo định lý Hahn-Banach (II, p. 23, hệ quả 1), ta có ${}^t i(B) = A$, suy ra (i).

Bây giờ chứng minh (ii). Theo mệnh đề 6 của IV, p. 6, ánh xạ tuyến tính ${}^t i$ từ $E'_{\mathfrak{S}}$ vào $M'_{\mathfrak{S}_1}$ là liên tục, và, qua phép thương, xác định một ánh xạ tuyến tính liên tục $\iota$ từ $E'_\mathcal{S}/M^\circ$ lên $M'_{\mathcal{S}_1}$. Kí hiệu $\mathcal{T}$ là tôpô trên $M'$ thu được bằng cách chuyển tôpô của $E'_\mathcal{S}/M^\circ$ qua $\iota$; tôpô này mịn hơn tôpô $\mathcal{S}_1$.

Giả sử bây giờ rằng $\mathcal{S}$ là một tập có hướng theo $\subset$ và gồm các tập đóng, lồi, cân bằng và compact đối với $\sigma(E, E')$. Để chỉ ra rằng $\iota$ là một đồng phôi, *tức là* $\mathcal{T}$ thô hơn tôpô $\mathcal{S}_1$ trên $M'$, chỉ cần chứng minh rằng $\mathcal{T}$ tương thích với tính đối ngẫu giữa $M'$ và $M$ và rằng mọi tập đều liên tục trong $M$ (xét như đối ngẫu của $M$ với $\mathcal{T}$) đều được chứa trong một tập vị tự của một tập thuộc $\mathcal{S}_1$. Vì $\mathcal{T}$ mịn hơn tôpô $\mathcal{S}_1$ và $\mathcal{S}_1$ là một phủ của $M$, dạng tuyến tính $y' \mapsto \langle y, y' \rangle$ trên $M'$ là liên tục đối với $\mathcal{T}$ với mọi $y \in M$. Cho $f$ là một dạng tuyến tính trên $M'$ liên tục đối với $\mathcal{T}$; khi đó $f \circ \iota$ là một dạng tuyến tính liên tục trên $E'_\mathcal{S}$. Tôpô $\mathcal{S}$ trên $E'$ thô hơn tôpô Mackey $\tau(E', E)$; vì ánh xạ $d_B : E \to {E'}^*$ là liên tục đối với các tôpô $\sigma(E, E')$ và $\sigma({E'}^*, E')$, và vì tôpô sau là Hausdorff, ảnh bởi $d_B$ của một tập compact đối với $\sigma(E, E')$ là compact đối với $\sigma({E'}^*, E')$. Theo bổ đề 1 của IV, p. 3, tồn tại $x_0 \in E$ sao cho $f(\iota(x')) = \langle x_0, x' \rangle$ với mọi $x' \in E'$. Đặc biệt, $\langle x_0, x' \rangle = 0$ với mọi $x' \in M^\circ$, và vì $M$ đóng trong $E$, ta có $x_0 \in M$ (II, p. 45, hệ quả 2); và cuối cùng, $f(y') = \langle x_0, y' \rangle$ với mọi $y' \in M'$. Điều này chứng tỏ rằng $\mathcal{T}$ *tương thích với tính đối ngẫu giữa* $M$ *và* $M'$.

Bây giờ cho $A$ là một tập con của $M$ đẳng liên đối với tôpô $\mathcal{T}$ trên $M'$. Theo định nghĩa của $\mathcal{T}$, và vì giả thiết rằng $\mathcal{S}$ có hướng, điều này có nghĩa là tồn tại một tập $B \in \mathcal{S}$ chứa 0 sao cho cận trên $\lambda$ của các số $|\langle y, x' \rangle|$ với $y \in A$ và $x' \in B^\circ$, là hữu hạn (III, p. 19, prop. 7). Vì $B$ đóng trong $E$, định lý song cực (II, p. 44, th. 1) cho thấy rằng ta có $A \subset \lambda(B \cap M)$; điều này hoàn tất chứng minh của (ii).

Bây giờ ta sẽ chứng minh (iii). Cho $y' \in M'$. Ta sẽ chứng minh công thức

$$
\|y'\| = \inf_{\iota(x') = y'} \|x'\|.
$$

Theo mệnh đề 8, (ii) của IV, p. 7, ta có $\|\iota\| = \|i\|$, do đó $\|\iota\| \leq 1$, và

$$
\|y'\| \leq \inf_{\iota(x') = y'} \|x'\|.
$$

Theo định lý Hahn-Banach (II, p. 23, cor. 3), tồn tại một dạng tuyến tính $x'_0$ trên $E$ mở rộng $y'$ và có cùng chuẩn; vì thế ta được bất đẳng thức ngược với (7), vì $\iota(x'_0) = y'$.

#### Nhận xét {#evt-iv-s1-n4-rem-1 .statement}

— Ta biết (II, p. 48, prop. 7, (ii)) rằng $\iota$ là một đẳng cấu không gian vectơ tôpô từ $E'_s/M^\circ$ onto $M'_s$ (đối ngẫu yếu). Đối với tôpô hội tụ lồi compact, mệnh đề 10 cho thấy rằng $\iota$ là một đẳng cấu từ $E'_{cc}/M^\circ$ onto $M'_{cc}$ khi $E$ là Hausdorff và $M$ đóng trong $E$. Đối với các tôpô mạnh, $\iota$ là một ánh xạ liên tục từ $E'_b/M^\circ$ onto $M'_b$; nó là một đẳng cấu nếu $E$ là một không gian Banach \* hoặc nếu $E$ là bán phản xạ và $M$ đóng trong $E$ (IV, p. 15) *, nhưng điều này không phải lúc nào cũng đúng nếu $E$ là một không gian Fréchet (IV, p. 58, exerc. 5, *c*)).

#### Mệnh đề 11 {#evt-iv-s1-prop-11 .statement}

— (i) *Tôpô suy yếu trên* $E/M$ *là tôpô thương của tôpô trên* $E$; *tôpô suy yếu trên* $M$ *được cảm sinh bởi tôpô của* $E$.

(ii) *Tôpô Mackey trên E/M là tôpô thương của tôpô trên E; tôpô Mackey trên M mịn hơn tôpô được cảm sinh bởi τ(E, E').*

Mệnh đề (i) suy ra từ mệnh đề 7 của II, p. 48.

Đơn ánh chính tắc $i : M \to E$ là liên tục đối với các tôpô suy yếu, do đó đối với các tôpô Mackey $\tau(M, M')$ và $\tau(E, E')$ (IV, p. 7, prop. 7). Tương tự, phép chiếu chính tắc $p : E \to E/M$ là liên tục đối với các tôpô Mackey. Ta thấy ngay rằng tôpô thương trên $E/M$ thu được từ $\tau(E, E')$ tương thích với đối ngẫu giữa $E/M$ và $(E/M)'$, do đó thô hơn tôpô Mackey trên $E/M$, theo định lý của Mackey (IV, p. 2, th. 1). Điều này chứng minh (ii).

### 5. Đối ngẫu của một tổng trực tiếp và của một tích

Với mọi $i \in I$, cho $(E_i, F_i)$ là một cặp không gian vectơ, được đặt đối ngẫu bởi một dạng song tuyến tính $B_i$. Ta đặt $E = \prod_{i \in I} E_i$ và $F = \bigoplus_{i \in I} F_i$, và đồng nhất mỗi $F_i$ với một không gian con của $F$. Ta đặt $E$ và $F$ vào thế đối ngẫu nhờ dạng song tuyến tính

$$
B(x, y) = \sum_{i \in I} B_i(x_i, y_i) \quad \text{với} \quad x = (x_i) \quad \text{và} \quad y = (y_i)
$$

(họ $(B_i(x_i, y_i))_{i \in I}$ có giá hữu hạn).

Ta nhắc lại (II, p. 50, Mệnh đề 8) rằng tôpô yếu $\sigma(E, F)$ là tích của các tôpô yếu $\sigma(E_i, F_i)$.

#### Bổ đề 3 {#evt-iv-s1-lem-3 .statement}

— (i) *Với mọi $i \in I$, cho $\mathfrak{S}_i$ là một họ các tập con của $F_i$, bị chặn đối với $\sigma(F_i, E_i)$; đặt $\mathfrak{S} = \bigcup_{i \in I} \mathfrak{S}_i$. Khi đó tôpô $\mathfrak{S}$ trên $E$ là tích của các tôpô $\mathfrak{S}_i$ trên các $E_i$.*

(ii) *Với mọi $i \in I$, cho $\mathfrak{J}_i$ là một hệ bị chặn thích nghi trên không gian $E_i$ được trang bị tôpô yếu $\sigma(E_i, F_i)$, không hệ nào bằng $\{ \varnothing \}$. Cho $\mathfrak{J}$ là họ các tập con $A$ của $E = \prod_{i \in I} E_i$ sao cho $\operatorname{pr}_i(A) \in \mathfrak{J}_i$ với mọi $i \in I$. Khi đó tôpô $\mathfrak{J}$ trên $F$ là tổng trực tiếp của các tôpô $\mathfrak{J}_i$ trên các $F_i$.*

Cho $\mathcal{T}$ là tích của các tôpô $\mathfrak{S}_i$. Các tập có dạng

$$
A = \prod_{i \in J} A_i^\circ \times \prod_{i \in I - J} E_i
$$

trong đó $J \subset I$ là hữu hạn và $A_i \in \mathfrak{S}_i$ với mọi $i \in J$, tạo thành một hệ cơ bản các lân cận của 0 cho $\mathcal{T}$. Ta có $A = (\bigcup_{i \in J} A_i)^\circ$, do đó $\mathcal{T}$ trùng với tôpô $\mathfrak{S}$. Điều này chứng minh (i).

Ta gán tôpô $\mathfrak{J}$ cho $F$ và tôpô $\mathfrak{J}_i$ cho từng $F_i$. Với mọi tập con $A$ của $E$, ta có $F_i \cap A^\circ = \operatorname{pr}_i(A)^\circ$, do đó đơn ánh từ $F_i$ vào $F$ là liên tục. Cho $q$ là một nửa chuẩn trên $F$; giả sử rằng hạn chế $q_i$ của $q$ trên $F_i$ là liên tục với mọi $i \in I$. Khi đó ta có thể tìm các tập con khác rỗng $A_i \in \mathfrak{J}_i$ sao cho ta có

$$
q_i(y_i) \leq \sup_{x_i \in A_i} |B_i(x_i, y_i)| \quad (y_i \in F_i) .
$$

Đặt $A = \prod_{i \in I} A_i$; khi đó $A \in \mathfrak{J}$. Với $y = (y_i)_{i \in I}$ trong $F$, ta có
$$
q(y) \leq \sum_{i \in I} q_i(y_i) \leq \sum_{i \in I} \sup_{x_i \in A_i} |B_i(x_i, y_i)| = \sup_{x \in A} |B(x, y)|,
$$
trong đó đẳng thức cuối cùng suy ra từ (8) vì họ $(y_i)_{i \in I}$ có giá hữu hạn và các $A_i$ khác rỗng và có thể giả sử cân bằng (GT, IV, § 5, No. 7, hệ quả 2 của mệnh đề 12). Bất đẳng thức này chứng tỏ rằng $q$ liên tục trên $F$, và do đó (ii).

#### Mệnh đề 12 {#evt-iv-s1-prop-12 .statement}

*Tôpô $\beta(F, E)$ là tổng trực tiếp của các tôpô $\beta(F_i, E_i)$. Tôpô $\beta(E, F)$ là tích của các tôpô $\beta(E_i, F_i)$.*

Ta sẽ áp dụng bổ đề 3, lấy cho $\mathfrak{S}_i$ họ tất cả các tập con của $F_i$ bị chặn đối với $\sigma(F_i, E_i)$ và cho $\mathfrak{J}_i$ họ tất cả các tập con của $E_i$ bị chặn đối với $\sigma(E_i, F_i)$.

Theo hệ quả 2 của III, p. 4, $\mathfrak{J}$ là họ tất cả các tập con của $E_i$ bị chặn đối với tôpô tích của các $\sigma(E_i, F_i)$, tôpô này trùng với $\sigma(E, F)$. Vì vậy mệnh đề của chúng ta về $\beta(F, E)$ suy ra.

Ta trang bị cho $F = \bigoplus_{i \in I} F_i$ tôpô $\mathcal{T}$, là tổng trực tiếp của các tôpô $\sigma(F_i, E_i)$. Khi đó đối ngẫu của $F$ gồm các dạng tuyến tính $y \mapsto B(x, y)$ với $x$ chạy qua $E$ (II, p. 30, mệnh đề 6). Theo mệnh đề 1 của IV, p. 1, các tôpô $\mathcal{T}$ và $\sigma(F, E)$ có cùng các tập bị chặn. Trước hết giả sử rằng các tôpô $\sigma(F_i, E_i)$ là Hausdorff. Theo mệnh đề 5 của III, p. 5, các tập hợp này được chứa trong một tập con có dạng $\sum_{i \in J} B_i$ với $J \subset I$ hữu hạn và $B_i$ bị chặn trong $F_i$ (đối với $\sigma(F_i, E_i)$) với mọi $i \in J$. Vì $\sum_{i \in J} B_i$ được chứa trong bao lồi của $\bigcup_{i \in J} nB_i$, trong đó $n = \mathrm{Card}(J)$, ta có thể áp dụng bổ đề 3 để chứng minh mệnh đề về $\beta(E, F)$ trong trường hợp này.

Trong trường hợp tổng quát, đặt $N_i$ là giao của mọi lân cận của 0 đối với $\sigma(F_i, E_i)$, và đặt $N = \sum_{i \in I} N_i$; khi đó $F/N$ là tổng trực tiếp tôpô của các $F_i/N_i$ (II, p. 31, mệnh đề 8); từ đây suy ra rằng mọi tập con của $F$ bị chặn đối với $\mathcal{T}$ đều được chứa trong một tập có dạng $N + \sum_{i \in J} B_i$ với $J \subset I$ hữu hạn và $B_i$ bị chặn trong $F_i$ với mọi $i \in J$ (III, p. 2, *Nhận xét* 3); vì đối cực của tập này trong $E$ trùng với đối cực của $\sum_{i \in J} B_i$, nên kết quả suy ra như trên.

#### Mệnh đề 13 {#evt-iv-s1-prop-13 .statement}

*Tôpô Mackey $\tau(F, E)$ là tổng trực tiếp của các tôpô Mackey $\tau(F_i, E_i)$. Tôpô $\tau(E, F)$ là tích của các tôpô $\tau(E_i, F_i)$.*

Mệnh đề về $\tau(F, E)$ suy ra từ bổ đề 3 (ii) và tính chất sau : để một tập con đóng, lồi và cân bằng của $F^* = \prod_{i \in I} F_i^*$ là compact đối với $\sigma(F^*, F)$, thì điều cần và đủ là phép chiếu của nó lên từng $F_i^*$ là compact đối với $\sigma(F_i^*, F_i)$.

Để chứng minh mệnh đề về $\tau(E, F)$, trước hết giả sử rằng các tôpô $\sigma(F_i, E_i)$ là Hausdorff, chỉ cần (bổ đề 3 (i)) chứng minh rằng mọi tập con $A$ của $F$ vừa lồi, vừa cân bằng và compact đối với $\sigma(F, E)$ đều được chứa trong một tập có dạng $\sum_{i \in J} A_i$ trong đó $J \subset I$ là hữu hạn và trong đó $A_i$ vừa lồi, vừa cân bằng và compact đối với $\sigma(F_i, E_i)$. Nhưng một tập con như vậy bị chặn đối với $\sigma(F, E)$. Theo chứng minh của mệnh đề 12, tồn tại một tập con hữu hạn $J$ của $I$ sao cho $A \subset \sum_{i \in J} F_i$, và chỉ cần lấy $A_i$ là phép chiếu của $A$ lên $F_i$.

Trong trường hợp tổng quát, với cùng các ký hiệu như trong chứng minh của mệnh đề 12, ta có $\tau(E_i, F_i) = \tau(E_i, F_i/N_i)$ và $\tau(E, F) = \tau(E, F/N)$ (IV, p. 2) và vì $F/N$ là tổng trực tiếp tôpô của các $F_i/N_i$, nên ta đã quy về trường hợp trước.

Q.E.D.

Đối với phần còn lại của đoạn này, ta giả sử rằng $(E_i)_{i \in I}$ là một họ các không gian lồi địa phương. Kí hiệu $S$ là tổng trực tiếp tôpô của các $E_i$ và $P$ là tích của chúng. Ta định nghĩa một ánh xạ tuyến tính $\theta : S' \to \prod_{i \in I} E_i'$, được gọi là *chính tắc*, bởi

$$
\theta(x') = (x'|E_i)_{i \in I} \quad (x' \in S')
$$

(trong đó $S'$ ký hiệu đối ngẫu của $S$, và $E_i'$ là đối ngẫu của $E_i$).

#### Mệnh đề 14 {#evt-iv-s1-prop-14 .statement}

(i) *Ánh xạ $\theta$ là một đẳng cấu từ đối ngẫu mạnh (tương ứng yếu) của $S = \bigoplus_{i \in I} E_i$ lên tích của các đối ngẫu mạnh (tương ứng yếu) của các $E_i$:*

(ii) *Để một tập con $A$ của $S'$ là đều liên tục, cần và đủ rằng phép chiếu của $\theta(A)$ lên $E_i'$ đều liên tục với mọi $i \in I$.*

(iii) *Tôpô Mackey $\tau(S, S')$ là tổng trực tiếp của các tôpô Mackey $\tau(E_i, E_i')$.*

(iv) *Tôpô $\beta(S, S')$ là tổng trực tiếp của các tôpô $\beta(E_i, E_i')$.*

Việc $\theta$ là song ánh suy ra ngay từ định nghĩa của tổng trực tiếp tôpô (II, p. 30, Mệnh đề 6). Mệnh đề (i) khi đó suy ra từ mệnh đề 12 của IV, p. 12, đối với các tôpô mạnh, và từ mệnh đề 8 của II, p. 50, đối với các tôpô yếu. Tương tự, (iii) suy ra từ mệnh đề 13 (IV, p. 12) và (iv) từ mệnh đề 12 (IV, p. 12).

Để chứng minh (ii), cho $A$ là một tập con của $S'$. Đặt

$$
q(x) = \sup_{x' \in A} |\langle x, x' \rangle| \quad \text{cho} \quad x \in S ;
$$

gọi $q_i$ là hạn chế của $q$ lên $E_i$, do đó

$$
q_i(x_i) = \sup_{x_i' \in A_i} |\langle x_i, x_i' \rangle| \quad \text{cho} \quad x_i \in E_i ,
$$

trong đó $A_i$ ký hiệu phép chiếu của $\theta(A)$ lên $E_i'$. Để $A$ đều liên tục, cần và đủ rằng $q$ là hữu hạn (tức là mỗi $q_i$ hữu hạn) và liên tục. Xét đặc trưng hóa các nửa chuẩn liên tục trên một tổng trực tiếp tôpô (II, p. 27, mệnh đề 5), điều này tương đương với việc giả sử rằng mỗi $q_i$ đều liên tục, hay thực ra, rằng mỗi tập $A_i$ đều liên tục.

Cho $\phi$ là ánh xạ tuyến tính, được gọi là *chính tắc*, từ $\bigoplus_{i \in I} E_i'$ vào đối ngẫu $P'$ của $P = \prod_{i \in I} E_i$, được xác định bởi công thức

$$
\langle x, \phi(x') \rangle = \sum_{i \in I} \langle x_i, x'_i \rangle
$$

với $x = (x_i)$ trong $P$ và $x' = (x'_i)$ trong $\bigoplus_{i \in I} E'_i$.

#### Mệnh đề 15 {#evt-iv-s1-prop-15 .statement}

— (i) *Ánh xạ $\phi$ là một đẳng cấu từ tổng trực tiếp tôpô của các đối ngẫu mạnh của các $E_i$ lên đối ngẫu mạnh của $P = \prod_{i \in I} E_i$.*

(ii) *Để một tập con $A$ của $P'$ là đều liên tục, điều kiện cần và đủ là nó được chứa trong một tổng hữu hạn $\sum_{i \in J} \phi(A_i)$, trong đó $J \subset I$ là hữu hạn và trong đó $A_i$ đều liên tục trong $E'_i$ với mọi $i \in J$. \*

(iii) *Tôpô Mackey $\tau(P, P')$ là tích của các tôpô $\tau(E_i, E'_i)$. \*

(iv) *Tôpô $\beta(P, P')$ là tích của các tôpô $\beta(E_i, E'_i)$. \*

Hiển nhiên rằng $\phi$ là đơn ánh. Một hệ cơ bản các lân cận của 0 trong $P$ gồm các tập có dạng $V = \prod_{i \in J} V_i \times \prod_{i \in I - J} E_i$, trong đó $J \subset I$ là hữu hạn và $V_i$ là một lân cận của 0 trong $E_i$ với $i$ thuộc $J$. Đối cực của $V$ trong $P'$ bằng $\sum_{i \in J} \phi(V_i^0)$.

Điều này chứng minh tính toàn ánh của $\phi$ và cũng chứng minh mệnh đề (ii).

Các mệnh đề (i) và (iv) suy ra từ Mệnh đề 12 (IV, p. 12) và (iii) từ Mệnh đề 13 (IV, p. 12).

#### Hệ quả {#evt-iv-s1-n5-cor-1 .statement}

— *Mọi tích của các không gian barrelled đều là barrelled.*

Một không gian địa phương lồi $E$ là barrelled khi và chỉ khi tôpô ban đầu trùng với $\beta(E, E')$ (IV, p. 4, *Nhận xét 3*). Vì vậy chỉ cần áp dụng Mệnh đề 15 (iv).

### Bài tập {#evt-iv-s1-exercises}

Xem [các bài tập cho § 1](exercises/s1/).
