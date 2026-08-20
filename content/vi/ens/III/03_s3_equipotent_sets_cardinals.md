---
book: ens
book_title: Theory of Sets
chapter: III
chapter_title: ORDERED SETS, CARDINALS, INTEGERS
section: 3
section_title: Equipotent sets. Cardinals
lang: vi
source: ens-i-iv
source_edition: 2004, Springer
book_pages: 157-165, 229-230
pdf_pages: 0163-0171, 0235-0236
extraction: ocr
subsections:
    - "no": 1
      title: THE CARDINAL OF A SET
      page: 157
      pdf_page: 163
    - "no": 2
      title: ORDER RELATION BETWEEN CARDINALS
      page: 158
      pdf_page: 164
    - "no": 3
      title: OPERATIONS ON CARDINALS
      page: 160
      pdf_page: 166
    - "no": 4
      title: PROPERTIES OF THE CARDINALS 0 AND 1
      page: 162
      pdf_page: 168
    - "no": 5
      title: EXPONENTIATION OF CARDINALS
      page: 163
      pdf_page: 169
    - "no": 6
      title: ORDER RELATION AND OPERATIONS ON CARDINALS
      page: 164
      pdf_page: 170
statements: 37
exercises: 6
errata:
    - says: § 5, no. 4, Proposition 5, Corollary 2
      read: § 5, no. 4, Proposition 6, Corollary 2
      why: The sentence on page 157 is a translation of the condition that a product set should be non-empty, which is Corollary 2 of no. 4 of § 5 of chapter II. The five corollaries of that no. are printed under Proposition 6 and the volume names them under Proposition 5 here as it does three times in chapter II itself.
    - says: § 6, no. 3, Theorem 3
      read: § 6, no. 3, Theorem 2
      why: Section 6 has no Theorem 3. No. 3 prints Theorem 2 on page 186, then Lemma 1 and Lemma 2, then the proof of Theorem 2 on page 187, then four corollaries on page 188. The Corollary 4 this sentence cites with it is the one that puts the product of two cardinals, one of them infinite, at their supremum, which is Corollary 4 of Theorem 2 and is what the sentence is about.
content_sha256: 384977de7176a8cfd4682e6139eda6057e3fccc7631710d29910fce82d7f02ce
translated_from: content/en/ens/III/03_s3_equipotent_sets_cardinals.md
source_content_sha256: da076d38fc218b1d22d88e12e76d715ae2c24eb275d05746754b09a72237c9f5
translation_model: gpt-5.4, gpt-5-6
translation_run: translate-vi-786fc151
glossary_version: 29
glossary_terms_sha256: c8a13a30b99cc61097cf1a7bb198f0f68d9460457ec82a4c38dcf44948fce268
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 3. CÁC TẬP HỢP ĐẲNG LỰC. CÁC LỰC LƯỢNG

### 1. LỰC LƯỢNG CỦA MỘT TẬP HỢP

#### Định nghĩa 1 {#ens-iii-s3-def-1 .statement tag=03QU}

Một tập hợp $X$ được gọi là đẳng lực với một tập hợp $Y$ nếu tồn tại một song ánh của $X$ lên $Y$. Quan hệ “$X$ đẳng lực với $Y$” được ký hiệu bởi $\operatorname{Eq}(X,Y)$.

Các quan hệ $\operatorname{Eq}(X,Y)$ và $\operatorname{Eq}(Y,X)$ rõ ràng là tương đương, do đó quan hệ $\operatorname{Eq}(X,Y)$ là *đối xứng*; khi nó đúng, ta nói rằng $X$ và $Y$ là *đẳng lực*. Tiếp theo, $\operatorname{Eq}(X,X)$ là đúng. Sau hết, quan hệ $\operatorname{Eq}(X,Y)$ là *bắc cầu* vì hợp thành của hai song ánh là một song ánh (Chương II, § 3, no. 8, Định lý 1); do đó nó là một *quan hệ tương đương*, phản xạ trên mọi tập hợp.

¶ Từ những gì đã nói suy ra rằng nếu $X$ và $Y$ là đẳng lực, thì quan hệ

$$
(\forall Z)(\operatorname{Eq}(X,Z)\Longleftrightarrow\operatorname{Eq}(Y,Z))
$$

là đúng. Bây giờ lược đồ tiên đề S7 (Chương I, § 5, no. 1) cho ta tiên đề sau đây :

$$
((\forall Z)(\operatorname{Eq}(X,Z)\Longleftrightarrow\operatorname{Eq}(Y,Z))\Rightarrow(\tau_Z(\operatorname{Eq}(X,Z))=\tau_Z(\operatorname{Eq}(Y,Z)))).
$$

Do đó, nếu X và Y là đẳng lực, thì ta có

$$\tau_Z(\mathrm{Eq}(X, Z)) = \tau_Z(\mathrm{Eq}(Y, Z)),$$

điều này biện minh cho định nghĩa sau đây :

#### Định nghĩa 2 {#ens-iii-s3-def-2 .statement tag=03QV}

*Tập hợp* $\tau_Z(\mathrm{Eq}(X, Z))$ *được gọi là lực lượng của* X (hoặc *lũy thừa* của X) *và được ký hiệu là* $\mathrm{Card}(X)$.

Vì $\mathrm{Eq}(X, X)$ là đúng, nên $\mathrm{Card}(X)$ *đẳng lực* với X (Chương I, § 4, Lược đồ S5). Vậy nên chúng ta đã chứng minh mệnh đề sau :

#### Mệnh đề 1 {#ens-iii-s3-prop-1 .statement tag=03QW}

*Hai tập hợp* X *và* Y *là đẳng lực khi và chỉ khi các lực lượng của chúng bằng nhau.*

*Ví dụ*

#### Ví dụ 1 {#ens-iii-s3-n1-exa-1 .statement tag=03T5}

$\mathrm{Card}(\emptyset)$ được ký hiệu bởi 0. Vì tập hợp duy nhất đẳng lực với $\emptyset$ là $\emptyset$ (Chương II, § 3, nos. 1 and 4), nên ta có $0 = \mathrm{Card}(\emptyset) = \emptyset$.

#### Ví dụ 2 {#ens-iii-s3-n1-exa-2 .statement tag=03T6}

Mọi tập hợp gồm một phần tử đều đẳng lực, vì $\{(a, b)\}$ là đồ thị của một song ánh từ $\{a\}$ lên $\{b\}$; đặc biệt, chúng đều đẳng lực với $\{\emptyset\}$. Lực lượng $\mathrm{Card}(\{\emptyset\}) = \tau_Z(\mathrm{Eq}(\{\emptyset\}, Z))$ được ký hiệu bởi 1. [^1]

#### Ví dụ 3 {#ens-iii-s3-n1-exa-3 .statement tag=03T7}

$\mathrm{Card}(\{\emptyset, \{\emptyset\}\})$ được ký hiệu bởi 2; đây là lực lượng của mọi tập hợp gồm hai phần tử phân biệt.

#### Ví dụ 4 {#ens-iii-s3-n1-exa-4 .statement tag=03T8}

Một không gian Hilbert kiểu đếm được đẳng lực với tập hợp các số thực. \*

### 2. QUAN HỆ THỨ TỰ GIỮA CÁC LỰC LƯỢNG

Quan hệ “X đẳng lực với một tập con của Y” là tương đương với “tồn tại một đơn ánh từ X vào Y”; nó cũng tương đương với quan hệ “Card (X) đẳng lực với một tập con của Card (Y)” (Chương II, § 3, no. 8, Định lý 1).

#### Định lý 1 {#ens-iii-s3-thm-1 .statement tag=03QX}

*Quan hệ $R\{\xi,\eta\}$: “$\xi$ và $\eta$ là các lực lượng và $\xi$ đẳng lực với một tập con của $\eta$” là một quan hệ thứ tự tốt (§ 2, no. 1).*

Vì $R\{\xi,\xi\}$ đúng với mọi lực lượng $\xi$, điều phải chứng minh là, với mọi tập hợp $E$ các lực lượng, quan hệ “$\xi\in E$ và $\eta\in E$ và $R\{\xi,\eta\}$” là một quan hệ thứ tự tốt trên $E$. Xét tập hợp $A=\bigcup_{\xi\in E}\xi$.

Mọi lực lượng $\xi\in E$ khi đó là một tập con của $A$. Theo § 2, định lý 1 tồn tại một quan hệ thứ tự tốt trên $A$, mà ta sẽ ký hiệu là $\xi\leq\eta$, và mọi tập con của $A$ đều đẳng lực với một đoạn của $A$ (§ 2, no. 5, định lý 3, hệ quả x). Với mỗi lực lượng $\xi\in E$, xét tập hợp các đoạn của $A$ đẳng lực với $\xi$; tập hợp các đoạn này không rỗng và do đó có phần tử nhỏ nhất (§ 2, no. 1, mệnh đề 2); gọi $\varphi(\xi)$ là phần tử nhỏ nhất này. Quan hệ

“$\xi\in E$ và $\eta\in E$ và $\xi$ đẳng lực với một tập con của $\eta$”

khi đó *tương đương* với

“$\xi\in E$ và $\eta\in E$ và $\varphi(\xi)\subset\varphi(\eta)$”.

Vì rõ ràng quan hệ thứ hai suy ra quan hệ thứ nhất. Ngược lại, nếu $\xi$ là đẳng lực với một tập con của $\varphi(\eta)$, thì không thể có $\varphi(\eta)\subset\varphi(\xi)$ và $\varphi(\eta)\neq\varphi(\xi)$; nếu không thì sẽ tồn tại một đoạn của $\varphi(\eta)$ đẳng lực với $\xi$ (§ 2, no. 5, Định lý 3, Hệ quả 3), trái với định nghĩa của $\varphi(\xi)$. Vì tập hợp các đoạn của $A$ được sắp tốt theo bao hàm (§ 2, no. 1, Mệnh đề 2), định lý được suy ra.

¶ Ta sẽ ký hiệu quan hệ $R\{\xi,\eta\}$ bởi $\xi\leq\eta$. Một tập hợp $X$ đẳng lực với một tập con của một tập hợp $Y$ khi và chỉ khi $\operatorname{Card}(X)\leq\operatorname{Card}(Y)$.

Rõ ràng ta có $0\leq\xi$ với mọi lực lượng $\xi$, và $1\leq\xi$ với mọi lực lượng $\xi\neq0$.

#### Hệ quả 1 {#ens-iii-s3-thm-1-cor-1 .statement tag=03QY}

*Cho hai tập hợp bất kỳ, một trong hai tập hợp đó đẳng lực với một tập con của tập hợp kia.*

#### Hệ quả 2 {#ens-iii-s3-thm-1-cor-2 .statement tag=03QZ}

*Hai tập hợp mà mỗi tập hợp đẳng lực với một tập con của tập hợp kia thì đẳng lực.*

#### Nhận xét {#ens-iii-s3-n2-rem-1 .statement tag=03R0}

Với mọi tập hợp $A$, tồn tại một tập hợp mà các phần tử của nó là các lực lượng $\operatorname{Card}(X)$ của mọi tập con $X$ của $A$, cụ thể là tập hợp các đối tượng có dạng $\operatorname{Card}(X)$ với $X\in\mathfrak{P}(A)$ (Chương II, § 1, no. 6). Do đó, với mọi lực lượng $\alpha$, quan hệ “$\xi$ là một lực lượng và $\xi\leq\alpha$” là xác định tập theo $\alpha$ (Chương II, § 1, no. 4), vì nó tương đương với

quan hệ “$\mathfrak{x}$ có dạng Card (X) với $X \subset \mathfrak{a}$”; tập hợp mọi $\mathfrak{x}$ thỏa mãn quan hệ này được gọi là *tập hợp các lực lượng* $\leqslant \mathfrak{a}$.

#### Mệnh đề 2 {#ens-iii-s3-prop-2 .statement tag=03KL}

*Với mọi họ* $(\mathfrak{a}_\iota)_{\iota \in I}$ *các lực lượng, tồn tại một lực lượng duy nhất* $\mathfrak{b}$ *sao cho* $\mathfrak{a}_\iota \leqslant \mathfrak{b}$ *với mọi* $\iota \in I$ *và sao cho mọi lực lượng* $\mathfrak{c}$ *mà đối với nó* $\mathfrak{a}_\iota \leqslant \mathfrak{c}$ *với mọi* $\iota \in I$ *đều* $\geqslant \mathfrak{b}$.

Tồn tại một tập hợp E chứa mọi tập hợp $\mathfrak{a}_\iota$ (chẳng hạn, tổng của các tập hợp này (Chương II, § 4, no. 8)), do đó $\mathfrak{a}_\iota \leqslant \mathfrak{a} = $ Card (E) với mọi $\iota \in I$. Tập hợp F các lực lượng $\leqslant \mathfrak{a}$ được sắp tốt và chứa mọi $\mathfrak{a}_\iota$, và vì thế họ $(\mathfrak{a}_\iota)_{\iota \in I}$ có một cận trên bé nhất $\mathfrak{b}$ trong F. Gọi $\mathfrak{c}$ là một lực lượng $\geqslant \mathfrak{a}_\iota$ với mọi $\iota \in I$; nếu $\mathfrak{c} < \mathfrak{b} \leqslant \mathfrak{a}$, thì $\mathfrak{c} \in F$, và bất đẳng thức $\mathfrak{a}_\iota \leqslant \mathfrak{c}$ mâu thuẫn với định nghĩa của cận trên bé nhất của họ $(\mathfrak{a}_\iota)$ trong tập hợp có thứ tự F; do đó có kết quả.

¶ Do lạm dụng ngôn ngữ, lực lượng $\mathfrak{b}$ được gọi là *cận trên bé nhất* của họ $(\mathfrak{a}_\iota)_{\iota \in I}$ và được ký hiệu bởi $\sup_{\iota \in I} \mathfrak{a}_\iota$.

#### Mệnh đề 3 {#ens-iii-s3-prop-3 .statement tag=03KM}

*Cho* X *và* Y *là các tập hợp. Nếu tồn tại một toàn ánh $f$ của* X *lên* Y, *thì* Card (Y) $\leqslant$ Card (X).

Thật vậy, tồn tại một tiết diện $s$ liên kết với $f$ (Chương II, § 3, no. 8, Mệnh đề 8) và $s$ là một đơn ánh của Y vào X.

### 3. CÁC PHÉP TOÁN TRÊN LỰC LƯỢNG

#### Định nghĩa 3 {#ens-iii-s3-def-3 .statement tag=03KN}

*Cho* $(\mathfrak{a}_\iota)_{\iota \in I}$ *là một họ các lực lượng. Lực lượng của tích* (resp. *tổng*) *của các tập hợp* $\mathfrak{a}_\iota$ *được gọi là tích lực lượng* (resp. *tổng lực lượng*) *của các lực lượng* $\mathfrak{a}_\iota$ *và được ký hiệu bởi* $\mathop{\mathbf{P}}_{\iota \in I} \mathfrak{a}_\iota$ $\left(\text{resp. } \sum_{\iota \in I} \mathfrak{a}_\iota\right)$.

Mỗi khi không có nguy cơ nhầm lẫn, ta sẽ nói đơn giản "tích" và "tổng" thay cho "tích lực lượng" và "tổng lực lượng", và ta sẽ viết $\prod_{\iota \in I} \mathfrak{a}_\iota$ thay cho $\mathop{\mathbf{P}}_{\iota \in I} \mathfrak{a}_\iota$ (xem Bài tập 2).

#### Mệnh đề 4 {#ens-iii-s3-prop-4 .statement tag=03KO}

*Cho* $(E_\iota)_{\iota \in I}$ *là một họ các tập hợp,* P *là tích của chúng, và* S *là tổng của chúng, và đặt* $\mathfrak{a}_\iota$ *là lực lượng của* $E_\iota$. *Khi đó lực lượng của* P (resp. S) *là tích lực lượng* (resp. *tổng lực lượng*) *của họ* $(\mathfrak{a}_\iota)_{\iota \in I}$.

Thật vậy, tồn tại một song ánh từ P (resp. S) lên tích (resp. tổng) của các tập hợp $(\mathfrak{a}_\iota)$ (Chương II, § 4, no. 8, Mệnh đề 10, và § 5, no. 7, Hệ quả của Mệnh đề 11).

#### Hệ quả {#ens-iii-s3-n3-cor-1 .statement tag=03KP}

*Nếu* $(E_\iota)_{\iota \in I}$ *là một họ tập hợp bất kỳ, thì lực lượng của hợp* $\bigcup_{\iota \in I} E_\iota$ *nhỏ hơn hoặc bằng tổng* $\sum_{\iota \in I}$ Card $(E_\iota)$.

Thật vậy, tồn tại một ánh xạ từ tổng S của các $\mathrm{E}_\iota$ lên hợp của các $\mathrm{E}_\iota$ (Chương II, § 4, no. 8); do đó Hệ quả suy ra từ các Mệnh đề 3 và 4.

#### Mệnh đề 5 {#ens-iii-s3-prop-5 .statement tag=03R1}

(a) *Cho* $(\mathfrak{a}_\iota)_{\iota \in \mathrm{I}}$ *là một họ các lực lượng, và cho f là một song ánh từ một tập hợp* K *lên tập hợp chỉ số* I. *Khi đó*

$$\sum_{x \in \mathrm{K}} \mathfrak{a}_{f(x)} = \sum_{\iota \in \mathrm{I}} \mathfrak{a}_\iota, \qquad \mathop{\mathrm{P}}_{x \in \mathrm{K}} \mathfrak{a}_{f(x)} = \mathop{\mathrm{P}}_{\iota \in \mathrm{I}} \mathfrak{a}_\iota.$$

(b) *Cho* $(\mathfrak{a}_\iota)_{\iota \in \mathrm{I}}$ *là một họ các lực lượng và cho* $(\mathrm{J}_\lambda)_{\lambda \in \mathrm{L}}$ *là một phân hoạch của* I. *Khi đó*

$$\sum_{\iota \in \mathrm{I}} \mathfrak{a}_\iota = \sum_{\lambda \in \mathrm{L}} \left( \sum_{\iota \in \mathrm{J}_\lambda} \mathfrak{a}_\iota \right), \qquad \mathop{\mathrm{P}}_{\iota \in \mathrm{I}} \mathfrak{a}_\iota = \mathop{\mathrm{P}}_{\lambda \in \mathrm{L}} \left( \mathop{\mathrm{P}}_{\iota \in \mathrm{J}_\lambda} \mathfrak{a}_\iota \right)$$

("tính kết hợp của tổng và tích").

(c) *Cho* $((\mathfrak{a}_{\lambda\iota})_{\iota \in \mathrm{J}_\lambda})_{\lambda \in \mathrm{L}}$ *là một họ (được đánh chỉ số bởi* L) *các họ lực lượng, và đặt* $\mathrm{I} = \coprod_{\lambda \in \mathrm{L}} \mathrm{J}_\lambda$. *Khi đó*

$$\mathop{\mathrm{P}}_{\lambda \in \mathrm{L}} \left( \sum_{\iota \in \mathrm{J}_\lambda} \mathfrak{a}_{\lambda\iota} \right) \sum_{f \in \mathrm{I}} = \left( \mathop{\mathrm{P}}_{\lambda \in \mathrm{L}} \mathfrak{a}_{\lambda, f(\lambda)} \right)$$

("tính phân phối của tích đối với tổng").

Các hệ thức trong (a) suy ra từ các công thức tương tự đối với hợp và tích của các tập hợp, vì việc $f$ là một song ánh kéo theo rằng nếu $(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$ là một họ các tập hợp đôi một rời nhau, thì các phần tử của họ $(\mathrm{X}_{f(x)})_{x \in \mathrm{K}}$ cũng đôi một rời nhau (xem Chương II, § 4, no. 1, Mệnh đề 1 và § 5, no. 3, Mệnh đề 4).

¶ Các hệ thức trong (b) là những hệ quả ngay lập tức của các công thức về tính kết hợp của hợp và tích (Chương II, § 4, no. 2, Mệnh đề 2 và § 5, no. 5, Mệnh đề 7) và của tính phân phối của giao đối với hợp (Chương II, § 5, no. 6, Mệnh đề 8), điều này cho thấy rằng nếu $(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$ là một họ các tập hợp đôi một rời nhau, thì các phần tử của họ

$$\left( \bigcup_{\iota \in \mathrm{J}_\lambda} \mathrm{X}_\iota \right)_{\lambda \in \mathrm{L}}$$

cũng đôi một rời nhau.

¶ Sau cùng, (c) suy ra từ tính phân phối của tích đối với hợp và giao (Chương II, § 5, no. 6, Mệnh đề 9 và Hệ quả 1).

¶ Cho $\mathfrak{a}$ và $\mathfrak{b}$ là hai lực lượng. Nếu I là một tập hợp gồm hai phần tử phân biệt (chẳng hạn lực lượng 2), thì tồn tại một ánh xạ $f$ từ I lên $\{\mathfrak{a}, \mathfrak{b}\}$ xác định một họ lực lượng. Tổng và tích của họ này

chỉ phụ thuộc vào $\mathfrak{a}$ và $\mathfrak{b}$ (theo Mệnh đề 5(a)); các lực lượng này được gọi tương ứng là *tổng* và *tích* của $\mathfrak{a}$ và $\mathfrak{b}$, và được ký hiệu bởi $\mathfrak{a} + \mathfrak{b}$ và $\mathfrak{a}\mathfrak{b}$. Tương tự đối với tổng và tích của ba hay nhiều lực lượng hơn. Khi đó Mệnh đề 5 kéo theo hệ quả sau :

#### Hệ quả {#ens-iii-s3-n3-cor-2 .statement tag=03R2}

*Cho $\mathfrak{a}$, $\mathfrak{b}$, $\mathfrak{c}$ là các lực lượng. Khi đó*

(1) $$\mathfrak{a} + \mathfrak{b} = \mathfrak{b} + \mathfrak{a}, \qquad \mathfrak{a}\mathfrak{b} = \mathfrak{b}\mathfrak{a};$$
(2) $$\mathfrak{a} + (\mathfrak{b} + \mathfrak{c}) = (\mathfrak{a} + \mathfrak{b}) + \mathfrak{c}, \qquad \mathfrak{a}(\mathfrak{b}\mathfrak{c}) = (\mathfrak{a}\mathfrak{b})\mathfrak{c};$$
(3) $$\mathfrak{a}(\mathfrak{b} + \mathfrak{c}) = \mathfrak{a}\mathfrak{b} + \mathfrak{a}\mathfrak{c}.$$

### 4. CÁC TÍNH CHẤT CỦA CÁC LỰC LƯỢNG 0 VÀ 1

#### Mệnh đề 6 {#ens-iii-s3-prop-6 .statement tag=03R3}

*Cho $(\mathfrak{a}_\iota)_{\iota \in \mathrm{I}}$ là một họ các lực lượng, và cho $\mathrm{J}$ (resp. $\mathrm{K}$) là một tập con của $\mathrm{I}$ sao cho $\mathfrak{a}_\iota = 0$ với mọi $\iota \notin \mathrm{J}$ (resp. $\mathfrak{a}_\iota = 1$ với mọi $\iota \notin \mathrm{K}$). Khi đó*

$$\sum_{\iota \in \mathrm{I}} \mathfrak{a}_\iota = \sum_{\iota \in \mathrm{J}} \mathfrak{a}_\iota \qquad \left(\text{resp. } \mathbf{P}_{\iota \in \mathrm{I}}\, \mathfrak{a}_\iota = \mathbf{P}_{\iota \in \mathrm{K}}\, \mathfrak{a}_\iota\right).$$

Mệnh đề là hiển nhiên đối với tổng, vì tổng $\mathrm{S}_\mathrm{I}$ của họ các tập hợp $(\mathfrak{a}_\iota)_{\iota \in \mathrm{I}}$ có cùng lực lượng với hợp của tổng $\mathrm{S}_\mathrm{J}$ của họ $(\mathfrak{a}_\iota)_{\iota \in \mathrm{I}}$ và tập rỗng, nên có cùng lực lượng với $\mathrm{S}_\mathrm{J}$. Mệnh đề liên quan đến các tích suy ra từ việc phép chiếu $\mathrm{pr}_\mathrm{K}$ của tập hợp tích $\prod_{\iota \in \mathrm{I}} \mathfrak{a}_\iota$ lên tích bộ phận $\prod_{\iota \in \mathrm{K}} \mathfrak{a}_\iota$ là một song ánh (Chương II, § 5, no. 5, Nhận xét 1).

#### Hệ quả 1 {#ens-iii-s3-prop-6-cor-1 .statement tag=03R4}

*Với mọi lực lượng $\mathfrak{a}$, ta có $\mathfrak{a} + 0 = \mathfrak{a} . 1 = \mathfrak{a}$.*

#### Hệ quả 2 {#ens-iii-s3-prop-6-cor-2 .statement tag=03R5}

*Cho $\mathfrak{a}$ và $\mathfrak{b}$ là các số lực và cho $\mathrm{I}$ là một tập hợp đẳng lực với $\mathfrak{b}$. Với mỗi $\iota \in \mathrm{I}$, đặt $\mathfrak{a}_\iota = \mathfrak{a}$, $\mathfrak{c}_\iota = 1$. Khi đó*

$$\mathfrak{a}\mathfrak{b} = \sum_{\iota \in \mathrm{I}} \mathfrak{a}_\iota, \qquad \mathfrak{b} = \sum_{\iota \in \mathrm{I}} \mathfrak{c}_\iota.$$

Công thức thứ hai là một hệ quả của sự kiện rằng mọi tập hợp đều là hợp của các tập con một phần tử của nó. Công thức thứ nhất suy ra từ công thức thứ hai bằng cách nhân với $\mathfrak{a}$ và dùng Hệ quả 1.

#### Mệnh đề 7 {#ens-iii-s3-prop-7 .statement tag=03R6}

*Cho $(\mathfrak{a}_\iota)_{\iota \in \mathrm{I}}$ là một họ các số lực. Khi đó $\mathbf{P}_{\iota \in \mathrm{I}}\, \mathfrak{a}_\iota \neq 0$ khi và chỉ khi $\mathfrak{a}_\iota \neq 0$ với mọi $\iota \in \mathrm{I}$.*

Đây chỉ đơn thuần là cách diễn đạt lại điều kiện để một tập tích là khác rỗng (Chương II, § 5, no. 4, Mệnh đề 5, Hệ quả 2).

#### Mệnh đề 8 {#ens-iii-s3-prop-8 .statement tag=03R7}

*Nếu $\mathfrak{a}$ và $\mathfrak{b}$ là các số lực sao cho $\mathfrak{a} + 1 = \mathfrak{b} + 1$, thì $\mathfrak{a} = \mathfrak{b}$.*

Cho $X = \mathfrak{a} + 1 = \mathfrak{b} + 1$. Khi đó tồn tại các tập con A, B của X có lực lượng tương ứng là $\mathfrak{a}$, $\mathfrak{b}$, sao cho các phần bù $X - A, X - B$ mỗi cái chỉ gồm một phần tử. Gọi $u$, $v$ là các phần tử ấy. Giao $C = A \cap B$ có phần bù trong X là tập hợp $\{u, v\}$. Nếu $u = v$ thì $A = B = C$, do đó $\mathfrak{a} = \mathfrak{b}$. Nếu $u \neq v$ thì $A = C \cup \{v\}$, $B = C \cup \{u\}$, và vì vậy $\mathfrak{a} = 1 + \mathrm{Card}\ (C) = \mathfrak{b}$.

☡

Người đọc nên thận trọng đừng cho rằng $\mathfrak{a} + \mathfrak{m} = \mathfrak{b} + \mathfrak{m}$ kéo theo $\mathfrak{a} = \mathfrak{b}$ đối với mọi lực lượng $\mathfrak{m}$ (xem § 6); \* tuy nhiên, ta sẽ thấy về sau rằng hệ quả này là đúng nếu $\mathfrak{m}$ là *hữu hạn* (§ 5, no. 2, Mệnh đề 3, Hệ quả 4 và § 6, no. 3, Định lý 3, Hệ quả 4). \*

### 5. PHÉP LŨY THỪA CỦA CÁC LỰC LƯỢNG

#### Định nghĩa 4 {#ens-iii-s3-def-4 .statement tag=03KQ}

*Cho $\mathfrak{a}$ và $\mathfrak{b}$ là các lực lượng. Lực lượng của tập hợp các ánh xạ từ $\mathfrak{b}$ vào $\mathfrak{a}$ được ký hiệu bởi $\mathfrak{a}^{\mathfrak{b}}$, do lạm dụng ký hiệu.*

Sự lạm dụng ký hiệu ở đây nằm ở chỗ $\mathfrak{a}^{\mathfrak{b}}$ đã ký hiệu tập hợp các đồ thị của các ánh xạ từ $\mathfrak{b}$ vào $\mathfrak{a}$ (Chương II, § 5, no. 3), và tập hợp này không tất yếu là một lực lượng (Bài tập 2). Từ ngữ cảnh, lúc nào cũng sẽ rõ phải gán cho ký hiệu $\mathfrak{a}^{\mathfrak{b}}$ nghĩa nào.

#### Mệnh đề 9 {#ens-iii-s3-prop-9 .statement tag=03KR}

*Cho X và Y là hai tập hợp, $\mathfrak{a}$ và $\mathfrak{b}$ là các lực lượng tương ứng của chúng. Khi đó tập hợp $X^{Y}$ có lực lượng $\mathfrak{a}^{\mathfrak{b}}$.*

Thật vậy, tồn tại một song ánh từ $X^{Y}$ lên tập hợp các ánh xạ từ $\mathfrak{b}$ vào $\mathfrak{a}$ (Chương II, § 5, no. 2, Mệnh đề 2, Hệ quả).

#### Mệnh đề 10 {#ens-iii-s3-prop-10 .statement tag=03KS}

*Cho $\mathfrak{a}$ và $\mathfrak{b}$ là các lực lượng và cho I là một tập hợp sao cho $\mathrm{Card}\ (I) = \mathfrak{b}$. Nếu $\mathfrak{a}_{\iota} = \mathfrak{a}$ với mọi $\iota \in I$, thì ta có $\mathfrak{a}^{\mathfrak{b}} = \mathbf{P}_{\iota \in I} \mathfrak{a}_{\iota}$.*

Điều này suy ra từ định nghĩa của tích của một họ tập hợp như một tập hợp các đồ thị phiếm hàm (Chương II, § 5, no. 3).

#### Hệ quả 1 {#ens-iii-s3-prop-10-cor-1 .statement tag=03KT}

*Cho $\mathfrak{a}$ là một lực lượng và cho $(\mathfrak{b}_{\iota})_{\iota \in I}$ là một họ các lực lượng. Khi đó*

$$\mathfrak{a}^{\sum_{\iota \in I} \mathfrak{b}_{\iota}} = \mathbf{P}_{\iota \in I} \mathfrak{a}^{\mathfrak{b}_{\iota}}.$$

Gọi S là tổng của các tập hợp $\mathfrak{b}_{\iota}$, và đặt $\mathfrak{a}_{s} = \mathfrak{a}$ với mọi $s \in S$. Khi đó hai vế của đẳng thức phải chứng minh đều bằng $\mathbf{P}_{s \in S} \mathfrak{a}_{s}$, theo Mệnh đề 10 và công thức tính kết hợp của các tích (no. 3, Mệnh đề 5(b)).

#### Hệ quả 2 {#ens-iii-s3-prop-10-cor-2 .statement tag=03KU}

*Cho $(\mathfrak{a}_\iota)_{\iota \in \mathbf{I}}$ là một họ các lực lượng và cho $\mathfrak{b}$ là một lực lượng. Khi đó*
$$\left( \mathop{\mathbf{P}}_{\iota \in \mathbf{I}} \mathfrak{a}_\iota \right)^{\mathfrak{b}} = \mathop{\mathbf{P}}_{\iota \in \mathbf{I}} \mathfrak{a}_\iota^{\mathfrak{b}}.$$

Đặt $\mathfrak{a}_{\iota\beta} = \mathfrak{a}_\iota$ với mỗi cặp $(\iota, \beta) \in \mathbf{I} \times \mathfrak{b}$. Khi đó, theo tính kết hợp của tích, ta có
$$\left( \mathop{\mathbf{P}}_{\iota \in \mathbf{I}} \mathfrak{a}_\iota \right)^{\mathfrak{b}} = \mathop{\mathbf{P}}_{\beta \in \mathfrak{b}} \left( \mathop{\mathbf{P}}_{\iota \in \mathbf{I}} \mathfrak{a}_{\iota\beta} \right) = \mathop{\mathbf{P}}_{\iota \in \mathbf{I}} \left( \mathop{\mathbf{P}}_{\beta \in \mathfrak{b}} \mathfrak{a}_{\iota\beta} \right) = \mathop{\mathbf{P}}_{\iota \in \mathbf{I}} \mathfrak{a}_\iota^{\mathfrak{b}}.$$

#### Hệ quả 3 {#ens-iii-s3-prop-10-cor-3 .statement tag=03KV}

*Cho $\mathfrak{a}$, $\mathfrak{b}$, $\mathfrak{c}$ là các lực lượng. Khi đó $\mathfrak{a}^{\mathfrak{b}\mathfrak{c}} = (\mathfrak{a}^{\mathfrak{b}})^{\mathfrak{c}}$.*

Cho $\mathfrak{b}_\gamma = \mathfrak{b}$ với mọi $\gamma \in \mathfrak{c}$. Khi đó
$$\mathfrak{a}^{\mathfrak{b}\mathfrak{c}} = \mathfrak{a}^{\sum\limits_{\gamma \in \mathfrak{c}} \mathfrak{b}_\gamma} = \mathop{\mathbf{P}}_{\gamma \in \mathfrak{c}} \mathfrak{a}^{\mathfrak{b}_\gamma} = (\mathfrak{a}^{\mathfrak{b}})^{\mathfrak{c}}$$
theo Hệ quả 1.

#### Mệnh đề 11 {#ens-iii-s3-prop-11 .statement tag=03KW}

*Cho $\mathfrak{a}$ là một lực lượng. Khi đó $\mathfrak{a}^0 = 1$, $\mathfrak{a}^1 = \mathfrak{a}$, $1^{\mathfrak{a}} = 1$; và $0^{\mathfrak{a}} = 0$ nếu $\mathfrak{a} \neq 0$.*

Thật vậy, tồn tại một ánh xạ duy nhất từ $\varnothing$ vào bất kỳ tập hợp đã cho nào (cụ thể là ánh xạ có đồ thị là tập rỗng); tập hợp các ánh xạ từ một tập hợp gồm một phần tử duy nhất vào một tập hợp tùy ý X là đẳng lực với X (Chương II, § 5, no. 3); tồn tại một ánh xạ duy nhất từ một tập hợp tùy ý vào một tập hợp gồm một phần tử duy nhất; và, cuối cùng, không có ánh xạ nào từ một tập hợp khác rỗng vào $\varnothing$.

¶ Đặc biệt, chú ý rằng $0^0 = 1$.

#### Mệnh đề 12 {#ens-iii-s3-prop-12 .statement tag=03KX}

*Cho X là một tập hợp và $\mathfrak{a}$ là lực lượng của nó. Khi đó lực lượng của tập hợp $\mathfrak{P}(\mathrm{X})$ gồm mọi tập con của X là $2^{\mathfrak{a}}$.*

Cho $\alpha$ và $\beta$ là các phần tử của lực lượng 2. Với mỗi tập con Y của X, gọi $f_{\mathrm{Y}}$ là ánh xạ từ X vào 2 được định nghĩa bởi $f_{\mathrm{Y}}(x) = \alpha$ nếu $x \in \mathrm{Y}$ và $f_{\mathrm{Y}}(x) = \beta$ nếu $x \in \mathrm{X} - \mathrm{Y}$. Gọi $u$ là ánh xạ $\mathrm{Y} \to f_{\mathrm{Y}}$ từ $\mathfrak{P}(\mathrm{X})$ vào $2^{\mathrm{X}}$. Ngược lại, với mỗi ánh xạ $g$ từ X vào 2, ta liên kết với nó tập con $\overset{-1}{g}(\alpha)$ của X, và gọi $v$ là ánh xạ $g \to \overset{-1}{g}(\alpha)$ từ $2^{\mathrm{X}}$ vào $\mathfrak{P}(\mathrm{X})$. Hiển nhiên $u \circ v$ và $v \circ u$ là các ánh xạ đồng nhất của $2^{\mathrm{X}}$ và $\mathfrak{P}(\mathrm{X})$; do đó $u$ và $v$ là các song ánh (chương II, § 3, no. 8, Mệnh đề 8, Hệ quả) và vì vậy Card $(\mathfrak{P}(\mathrm{X})) = 2^{\mathfrak{a}}$.

### 6. QUAN HỆ THỨ TỰ VÀ CÁC PHÉP TOÁN TRÊN LỰC LƯỢNG

#### Mệnh đề 13 {#ens-iii-s3-prop-13 .statement tag=03KY}

*Cho $\mathfrak{a}$ và $\mathfrak{b}$ là các lực lượng. Khi đó $\mathfrak{a} \geqslant \mathfrak{b}$ khi và chỉ khi tồn tại một lực lượng $\mathfrak{c}$ sao cho $\mathfrak{a} = \mathfrak{b} + \mathfrak{c}$.*

Quan hệ $\mathfrak{a} \geqslant \mathfrak{b}$ có nghĩa là tồn tại một tập con B của $\mathfrak{a}$ có cùng lực lượng với $\mathfrak{b}$ (số 2), tức là $\mathfrak{a}$ có cùng lực lượng với tập hợp là tổng của $\mathfrak{b}$ và một tập hợp $c$.

☡

Nếu $\mathfrak{a} \geqslant \mathfrak{b}$, thường tồn tại nhiều lực lượng $\mathfrak{c}$ sao cho $\mathfrak{a} = \mathfrak{b} + \mathfrak{c}$ (xem § 6); do đó, nói chung, không thể định nghĩa "hiệu" $\mathfrak{a} - \mathfrak{b}$ của hai lực lượng như vậy (xem § 5, số 2).

#### Mệnh đề 14 {#ens-iii-s3-prop-14 .statement tag=03KZ}

*Cho* $(\mathfrak{a}_\iota)_{\iota \in I}$ *và* $(\mathfrak{b}_\iota)_{\iota \in I}$ *là hai họ các số lực lượng, cả hai đều được đánh chỉ số bởi cùng một tập hợp* I, *và sao cho* $\mathfrak{a}_\iota \geqslant \mathfrak{b}_\iota$ *với mọi* $\iota \in I$. *Khi đó*

$$\sum_{\iota \in I} \mathfrak{a}_\iota \geqslant \sum_{\iota \in I} \mathfrak{b}_\iota, \qquad \mathbf{P}_{\iota \in I} \, \mathfrak{a}_\iota \geqslant \mathbf{P}_{\iota \in I} \, \mathfrak{b}_\iota.$$

Bất đẳng thức thứ hai suy ra từ các quan hệ bao hàm giữa các tích của các tập hợp (Chương II, § 5, số 4, Mệnh đề 6, Hệ quả 3). Đối với bất đẳng thức thứ nhất, nếu một tập hợp E là hợp của một họ $(A_\iota)_{\iota \in I}$ các tập con đôi một rời nhau và nếu $B_\iota \subset A_\iota$ với mọi $\iota \in I$, thì các $B_\iota$ cũng đôi một rời nhau và $\bigcup_\iota B_\iota \subset \bigcup_\iota A_\iota$ (Chương II, § 4, số 2).

#### Hệ quả 1 {#ens-iii-s3-prop-14-cor-1 .statement tag=03L0}

*Cho* $(\mathfrak{a}_\iota)_{\iota \in I}$ *là một họ các số lực lượng. Với mỗi tập con* J *của* I *ta có* $\sum_{\iota \in J} \mathfrak{a}_\iota \leqslant \sum_{\iota \in I} \mathfrak{a}_\iota$. *Nếu thêm* $\mathfrak{a}_\iota \neq 0$ *với mọi* $\iota \in I - J$, *thì* $\mathbf{P}_{\iota \in J} \, \mathfrak{a}_\iota \leqslant \mathbf{P}_{\iota \in I} \, \mathfrak{a}_\iota$.

Đặt $\mathfrak{b}_\iota = \mathfrak{a}_\iota$ nếu $\iota \in J$, và $\mathfrak{b}_\iota = 0$ (tương ứng $\mathfrak{b}_\iota = 1$) nếu $\iota \in I - J$. Khi đó áp dụng Mệnh đề 14, nhận thấy rằng quan hệ $\mathfrak{a} \neq 0$ kéo theo $\mathfrak{a} \geqslant 1$.

#### Hệ quả 2 {#ens-iii-s3-prop-14-cor-2 .statement tag=03L1}

*Nếu* $\mathfrak{a}$, $\mathfrak{a}'$, $\mathfrak{b}$, $\mathfrak{b}'$ *là các số lực lượng sao cho* $\mathfrak{a} \leqslant \mathfrak{a}'$, $\mathfrak{b} \leqslant \mathfrak{b}'$, *và* $\mathfrak{a}' > 0$, *thì* $\mathfrak{a}^\mathfrak{b} \leqslant \mathfrak{a}'^{\mathfrak{b}'}$.

For $\mathfrak{a}^\mathfrak{b} \leqslant \mathfrak{a}'^\mathfrak{b}$ theo Mệnh đề 10 và 14, và $\mathfrak{a}'^\mathfrak{b} \leqslant \mathfrak{a}'^{\mathfrak{b}'}$ theo Mệnh đề 10 và Hệ quả 1 của Mệnh đề 14.

#### Định lý 2 (Cantor) {#ens-iii-s3-thm-2 .statement tag=03R8}

— *Với mỗi lực lượng* $\mathfrak{a}$, *ta có* $2^\mathfrak{a} > \mathfrak{a}$.

Ta có $\mathrm{Card}(\mathfrak{P}(\mathfrak{a})) = 2^\mathfrak{a}$ (số 5, Mệnh đề 12). Ánh xạ $x \to \{x\}$ $(x \in \mathfrak{a})$ là một đơn ánh từ $\mathfrak{a}$ vào $\mathfrak{P}(\mathfrak{a})$, do đó $\mathfrak{a} \leqslant 2^\mathfrak{a}$. Vì thế chỉ cần chỉ ra rằng $\mathfrak{a} \neq 2^\mathfrak{a}$, nghĩa là, với mọi ánh xạ $f$ từ $\mathfrak{a}$ vào $\mathfrak{P}(\mathfrak{a})$, ảnh $f(\mathfrak{a})$ phân biệt với $\mathfrak{P}(\mathfrak{a})$. Gọi X là tập hợp tất cả các $x \in \mathfrak{a}$ sao cho $x \notin f(x)$. Nếu $x \in X$, ta có $x \notin f(x)$, do đó $f(x) \neq X$; nếu $x \in \mathfrak{a} - X$, ta có $x \in f(x)$ và $x \notin X$, do đó $f(x) = X$. Điều đó cho thấy rằng $X \notin f(\mathfrak{a})$ và chứng minh định lý.

#### Hệ quả {#ens-iii-s3-n6-cor-1 .statement tag=03L2}

*Không tồn tại một tập hợp có mọi lực lượng như một phần tử.*

Nếu U là một tập hợp như vậy, thì tồn tại một tập hợp S, là tổng của họ các tập hợp $(X)_{X \in U}$, sao cho mọi lực lượng là đẳng lực với một tập con của S. Đặc biệt, đặt $\mathfrak{S} = \mathrm{Card}(S)$; vì $2^\mathfrak{S}$ là một lực lượng, ta sẽ có $2^\mathfrak{S} \leqslant \mathfrak{S}$, trái với Định lý 2.

### Bài tập {#ens-iii-s3-exercises}

Xem các [bài tập của § 3](exercises/s3/).

[^1]: Số hạng toán học *được ký hiệu bởi* (Chương I, § 1, số 1) ký hiệu "1" dĩ nhiên không được nhầm lẫn với *từ* "một" trong ngôn ngữ thông thường. Số hạng được ký hiệu bởi "1" là bằng, theo định nghĩa ở trên, với số hạng được ký hiệu bởi ký hiệu $$\tau_Z((\exists u)(\exists U)(u = (U, \{\emptyset\}, Z) \text{ và } U \subset \{\emptyset\} \times Z$$ $$\text{và } (\forall x)((x \in \{\emptyset\}) \Rightarrow (\exists y)((x, y) \in U))$$ $$\text{và } (\forall x)(\forall y)(\forall y')(((x, y) \in U \text{ và } (x, y') \in U) \Rightarrow (y = y'))$$ $$\text{và } (\forall y)((y \in Z) \Rightarrow (\exists x)((x, y) \in U)))).$$ Theo một ước lượng sơ bộ, số hạng được *ký hiệu* như vậy là một tập hợp gồm vài chục nghìn dấu (mỗi dấu trong đó là một trong $\tau$, $\square$, $\vee$, $\neg$, $=$, $\in$, $\supset$).
