---
book: ens
book_title: Theory of Sets
chapter: ER
chapter_title: SUMMARY OF RESULTS
section: 5
section_title: Equivalence relations and quotient sets
lang: vi
source: ens-i-iv
source_edition: 2004, Springer
book_pages: 370-373
pdf_pages: 0375-0378
extraction: ocr
statements: 0
exercises: 0
content_sha256: 49e215ed1ff568eee3fef30476ad37251be78483681ba9d3c97509b06572485e
translated_from: content/en/ens/ER/05_s5_equivalence_relations_and_quotient_sets.md
source_content_sha256: ce494510e445f599fcaf23ba1f07c6def110ff6bae8350afcf9683adfcde4921
translation_model: gpt-5-6, copied
translation_run: translate-vi-79e29246
glossary_version: 34
glossary_terms_sha256: 6a8912079ceca85d919368143fd133f8f1758dd2bb55f3296d60b162b453c272
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 5. QUAN HỆ TƯƠNG ĐƯƠNG VÀ TẬP THƯƠNG

1. Cho $(A_i)_{i\in I}$ là một phân hoạch của một tập hợp E. Quan hệ $R\{x,y\}$: “tồn tại $i\in I$ sao cho $x\in A_i$ và $y\in A_i$,” giữa hai phần tử bất kỳ $x,y$ của E thỏa mãn các điều kiện sau:

(a) $R\{x,x\}$ là một đồng nhất thức (tính phản xạ của R).

(b) $R\{x,y\}$ và $R\{y,x\}$ là tương đương (tính đối xứng của R).

(c) Quan hệ $R\{x,y\}$ và $R\{y,z\}$ kéo theo $R\{x,z\}$ (tính bắc cầu của R).

Nếu C ký hiệu tập con của $E\times E$ được xác định bởi quan hệ R, thì các điều kiện (a), (b), (c) lần lượt tương đương với các điều kiện sau: $(a')\ \Delta\subset C$; $(b')\ \overline{C}=C$; $(c')\ C\circ C\subset C$. Từ $(a')$ và $(c')$ suy ra rằng $C\circ C=C$.

2. Ngược lại, cho $R\{x,y\}$ là một quan hệ phản xạ, đối xứng và bắc cầu, và cho C là đồ thị của nó trong $E\times E$. Khi đó ảnh $\mathfrak{P}$ của E qua ánh xạ $x\mapsto C(x)$ từ E vào $\mathfrak{P}(E)$ là một phân hoạch của E, và quan hệ “tồn tại một tập con X ∈ $\mathfrak{S}̃$ sao cho x ∈ X và y ∈ X” tương đương với
$R\{x,y\}$.

Mọi quan hệ thỏa mãn các điều kiện (a), (b), và (c) đều được gọi là một quan hệ tương đương trên E. Phân hoạch $\mathfrak{S}̃$ mà nó xác định, được xét như một tập con của $\mathscr{P}(E)$, được gọi là tập thương của E theo quan hệ R, và được ký hiệu bởi E/R; các phần tử của nó được gọi là các lớp tương đương theo R. Ánh xạ $x \mapsto C(x)$ của E lên E/R, ánh xạ mỗi phần tử x của E vào lớp tương đương chứa x, được gọi là ánh xạ chính tắc của E lên E/R.

Quan hệ đẳng thức $x = y$ là một quan hệ tương đương. Ánh xạ chính tắc của E lên tập thương tương ứng chỉ là $x \mapsto \{x\}$, và là song ánh.

Nếu R là một quan hệ tương đương, ký hiệu “$x \equiv y$ (mod R)” đôi khi được dùng như một từ đồng nghĩa với $R\{x,y\}$; nó được đọc là “x tương đương với y modulo R”.

3. Trên một tập tích $E \times F$, quan hệ “$\operatorname{pr}_1 z = \operatorname{pr}_1 z'$” giữa z và z′ là một quan hệ tương đương R, và tập thương $(E \times F)/R$ có thể đặt tương ứng một-một với E (đây là nguồn gốc của tên gọi tập thương).

Tổng quát hơn, cho f là một ánh xạ từ một tập hợp E vào một tập hợp F. Khi đó quan hệ “$f(x)=f(y)$” là một quan hệ tương đương trên E. Nếu ta ký hiệu quan hệ này bởi R, ánh xạ $z \mapsto f^{-1}(z)$ (trong đó $f^{-1}(z)$ được xem như một phần tử của E/R) là một song ánh của $f(E)$ lên E/R.

Suy ra rằng f có thể được xem như hợp thành của ba ánh xạ sau đây, theo thứ tự đã cho:
(1) ánh xạ chính tắc của tập con $f(E)$ của F vào tập hợp F;
(2) ánh xạ song ánh của E/R lên $f(E)$, mà ánh xạ nghịch đảo của nó vừa được xác định;
(3) ánh xạ chính tắc của E lên E/R.

Phân tích này của một ánh xạ được gọi là phân tích chính tắc hoặc phân tích nhân tử chính tắc của nó.

4. Mọi quan hệ tương đương R trên một tập hợp E đều có thể được xác định bằng một ánh xạ như trong tiểu mục trước; thật vậy, nếu C là đồ thị của R, thì quan hệ “$C(x)=C(y)$” tương đương với $R\{x,y\}$.

5. Cho R là một quan hệ tương đương trên một tập hợp E, và cho A là một tập con của E. Khi đó quan hệ $R\{x,y\}$ giữa hai phần tử bất kỳ x, y của A là một quan hệ tương đương trên A, được gọi là quan hệ cảm sinh bởi R trên A, và được ký hiệu bởi $R_A$. Cho f là ánh xạ chính tắc của E lên E/R và cho g là ánh xạ chính tắc của A lên $A/R_A$. Bằng cách cho một phần tử của E/R và một phần tử của $A/R_A$ tương ứng với nhau nếu chúng là ảnh của cùng một phần tử của E qua f và g tương ứng, ta có một sự tương ứng một-một giữa ảnh $f(A)$ của A qua f và tập thương $A/R_A$. Nếu φ ký hiệu ánh xạ chính tắc của A vào E, sự tương ứng này được thực hiện bởi ánh xạ $z \to f(\varphi(g^{-1}(z)))$ và ánh xạ nghịch đảo của nó, cả hai đều được gọi là *chính tắc*.

6. Một tập con A của E được gọi là *bão hòa* đối với quan hệ tương đương R nếu với mỗi $x \in A$, lớp tương đương của x theo R được chứa trong A. Nói cách khác, các tập hợp bão hòa đối với R là *hợp của các lớp tương đương theo R*. Nếu $f$ là ánh xạ chính tắc của E lên E/R, thì một tập hợp là bão hòa nếu nó có dạng $f^{-1}(X)$, trong đó $X \subset E/R$.

Cho A là một tập con của E. Giao của các tập hợp bão hòa chứa A là $f^{-1}(f(A))$. Tập hợp này cũng có thể được xác định là hợp của các lớp tương đương của các phần tử của A, và được gọi là *bão hòa* của A (đối với R).

7. Cho $P\{x,y,z\}$ là một quan hệ trong đó xuất hiện một phần tử bất kỳ $x$ của E. Khi đó P được gọi là *tương thích* (theo $x$) *với quan hệ tương đương* R nếu quan hệ “$P\{x,y,z\}$ và $x \equiv x'$ (mod R)” *kéo theo* $P\{x',y,z\}$.

Cho $f$ là ánh xạ chính tắc của E lên E/R, và cho $t$ là một phần tử bất kỳ của E/R. Quan hệ “tồn tại $x \in f^{-1}(t)$ sao cho $P\{x,y,z\}$” khi đó tương đương với “với mọi $x \in f^{-1}(t)$, $P\{x,y,z\}$”; quan hệ sau là một quan hệ giữa $t$, $y$, $z$, được gọi là *cảm sinh* bởi P *khi chuyển qua thương* (đối với $x$). Nếu ký hiệu nó bởi $P'\{t,y,z\}$, thì $P\{x,y,z\}$ tương đương với $P'\{f(x),y,z\}$.

Có các định nghĩa tương tự đối với một quan hệ liên quan đến một số bất kỳ các đối số, và đối với trường hợp quan hệ tương thích với R theo *nhiều* đối số của nó. Ví dụ, nếu A là một tập con của E, nói rằng quan hệ “$x \in A$” tương thích (theo $x$) với R tương đương với nói rằng A là bão hòa đối với R. Nếu $\varphi$ là một ánh xạ của E vào một tập hợp F, nói rằng quan hệ phiếm hàm “$y=\varphi(x)$” tương thích (theo $x$) với R có nghĩa là $\varphi$ là hằng trên mỗi lớp tương đương đối với R. Khi chuyển qua thương, R do đó cảm sinh một quan hệ giữa $y$ và một phần tử bất kỳ $t$ của E/R; quan hệ này là phiếm hàm theo $y$ và do đó xác định một ánh xạ $\varphi'$ của E/R vào F, thỏa mãn đồng nhất thức $\varphi(x)=\varphi'(f(x))$.

8. Cho R là một quan hệ tương đương trên một tập hợp E, cho S là một quan hệ tương đương trên một tập hợp F, và cho $f$ là một ánh xạ của E vào F. Ánh xạ $f$ được gọi là *tương thích với R và S* nếu quan hệ $x \equiv x'$ (mod R) *suy ra* $f(x) \equiv f(x')$ (mod S). Nếu $g$ là ánh xạ chính tắc của F lên F/S, thì hàm hợp $g \circ f$ có cùng một giá trị tại mọi phần tử của một lớp tương đương $z$ đối với R; nếu ký hiệu giá trị chung này bởi $h(z)$, thì $h$ là một ánh xạ của E/R vào F/S, và được gọi là *cảm sinh bởi f khi chuyển qua các thương*.

9. Cho R là một quan hệ tương đương trên E, và cho S là một quan hệ tương đương trên E/R. Nếu $f$ là ánh xạ chính tắc của E lên E/R, thì “$f(x)\equiv f(y)\pmod S$” là một quan hệ tương đương T trên E. Do đó, một lớp tương đương đối với T là hợp trong E của các lớp tương đương đối với R tương đương với nhau đối với S; và quan hệ “$x\equiv y\pmod R$” *suy ra* “$x\equiv y\pmod T$”. Nếu $g$ và $\varphi$ lần lượt là các ánh xạ chính tắc của $E$ lên $E/R$ và $E/T$, ta nhận được một sự tương ứng một-một (gọi là chính tắc) giữa $(E/R)/S$ và $E/T$ bằng cách cho một phần tử của $(E/R)/S$ và một phần tử của $E/T$ tương ứng với nhau nếu chúng lần lượt là ảnh của cùng một phần tử của E qua $g$ và $\varphi$.

Ngược lại, cho R và T là hai quan hệ tương đương trên E sao cho “$x\equiv y\pmod R$” *suy ra* “$x\equiv y\pmod T$”. Khi đó T tương thích (theo nghĩa của no. 7) với R, cả theo x lẫn theo y; bằng cách chuyển qua thương $E/R$ (đối với x và y), T cảm sinh một quan hệ tương đương S trên $E/R$. Nếu $\varphi$ lại ký hiệu ánh xạ chính tắc của E lên $E/R$, quan hệ “$\varphi(x)=\varphi(y)\pmod S$” tương đương với “$x\equiv y\pmod T$”. Quan hệ tương đương S được gọi là thương của T bởi R, và được ký hiệu bởi T/R. Từ đoạn trước ta thấy rằng tồn tại một sự tương ứng một-một (sự tương ứng chính tắc) giữa $(E/R)/(T/R)$ và $E/T$.

10. Now let E, F be any two sets, which may or may not be distinct. Let $\{x, y\}$ be an equivalence relation on E and let $\{z, t\}$ be an equivalence relation on F. Then the relation $\{x, y\}\times\{z, t\}$ between elements $(x,z)$ and $(y,t)$ of the product set $E\times F$ is an equivalence relation on $E\times F$, called the product of R by S, and denoted by $R\times S$. Every equivalence class with respect to $R\times S$ is the product of an equivalence class with respect to R and an equivalence class with respect to S. If u denotes a generic element of $E/R$, and v a generic element of $F/S$, then $(u,v)\mapsto u\times v$ is a bijection (called canonical) of $(E/R)\times(F/S)$ onto $(E\times F)/(R\times S)$.
