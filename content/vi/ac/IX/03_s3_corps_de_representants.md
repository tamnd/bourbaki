---
book: ac
book_title: Commutative Algebra
chapter: IX
chapter_title: ANNEAUX LOCAUX NOETHÉRIENS COMPLETS
section: 3
section_title: Corps de représentants
lang: vi
source: ac-viii-ix-fr
book_pages: AC IX.28-AC IX.30, AC IX.75-AC IX.78
pdf_pages: 0140-0142, 0187-0190
extraction: ocr
subsections:
    - "no": 1
      title: Anneaux locaux d’égales caractéristiques
      page: 28
      pdf_page: 140
    - "no": 2
      title: Un théorème de relèvement
      page: 28
      pdf_page: 140
    - "no": 3
      title: Corps de représentants
      page: 29
      pdf_page: 141
statements: 7
exercises: 9
content_sha256: 22cd14f17ceaf4ea7bf8c00216f226793be6856fcb0b18a3fe686ceac88827a1
translated_from: content/en-mt/ac/IX/03_s3_corps_de_representants.md
source_lang: en-mt
translation_method: machine
source_content_sha256: 6c19e36e8e9fe2a14bd3f138891e6c1cece185efb7ead4bcf2d5736981b90781
translation_model: gpt-5-6-mini
translation_run: translate-vi-0a5ada6c
glossary_version: 34
glossary_terms_sha256: 07af02a9967e968dcbda8589e7d906d0d562943efff40734a5b0ebccfb4610ff
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 3. Các trường đại diện

### 1. Các vành địa phương có cùng đặc số

Cho A là một vành. Nhắc lại (A, V, p. 2) rằng đặc số của A được xác định khi A chứa một trường con. Nó bằng 0 khi và chỉ khi A chứa một trường con đẳng cấu với $\mathbf{Q}$; và bằng một số nguyên tố $p$ khi và chỉ khi ta có $p1_A = 0$. Nếu đặc số của A được xác định, và nếu $f : A \to B$ là một đồng cấu khác không của các vành, thì đặc số của B được xác định và nó bằng đặc số của A.

Cho A là một vành địa phương, với iđêan cực đại $m$, và trường thặng dư $k$.

a) Giả sử rằng $k$ có đặc số 0. Khi đó A chứa một trường và đặc số của A bằng 0. Thật vậy, đồng cấu chính tắc từ $\mathbf{Z}$ vào A là đơn ánh, và với mọi số nguyên khác không $n$, $n1_A$ là khả nghịch trong A, vì nó không thuộc $m$.

b) Giả sử rằng $k$ có đặc số $p \neq 0$. Khi đó A chứa một trường khi và chỉ khi $p1_A = 0$. Trong trường hợp này đặc số của A bằng $p$.

Giả sử rằng A là một vành địa phương nguyên, với trường phân thức K và trường thặng dư $k$.

a’) Vành A chứa một trường con khi và chỉ khi các đặc số của $k$ và K bằng nhau. Trong trường hợp này, đặc số của A bằng đặc số của $k$ và K, và ta nói rằng A là một vành địa phương có cùng đặc số.

b’) Giả sử rằng các trường $k$ và K không có cùng đặc số. Khi đó tồn tại một số nguyên tố $p$ sao cho $k$ có đặc số $p$. Vì ta có $q1_A \neq 0$ với mọi số nguyên tố $q \neq p$, nên trường K có đặc số 0. Khi đó ta nói rằng A là một vành địa phương có các đặc số khác nhau.

### 2. Một định lý nâng

#### Mệnh đề 1 {#ac-ix-s3-prop-1 .statement}

Cho $k_0$ là một trường, A là một $k_0$-đại số là một vành địa phương tách và đầy đủ, K là một mở rộng con-$k_0$ của $\kappa_A$ có một cơ sở siêu việt tách được $(\xi_{\lambda})_{\lambda \in \Lambda}$ trên $k_0$ (A, V, p. 130, déf. 1). Với mỗi $\lambda \in \Lambda$, gọi $x_{\lambda}$ là một đại diện của $\xi_{\lambda}$ trong A. Tồn tại duy nhất một trường con L của A, chứa $k_0$ và các phần tử $x_{\lambda}$, sao cho đồng cấu chính tắc $\pi$ từ A lên $\kappa_A$ cảm sinh một đẳng cấu của L lên K.

Gọi $\varphi$ là $k_0$-đồng cấu của vành đa thức $k_0[(X_{\lambda})_{\lambda \in \Lambda}]$ vào A biến $X_{\lambda}$ thành $x_{\lambda}$ với mọi $\lambda \in \Lambda$. Gọi $u$ là một phần tử khác không của $k_0[(X_{\lambda})_{\lambda \in \Lambda}]$; ta có $\pi(\varphi(u)) \neq 0$, bởi vì họ $(\xi_{\lambda})_{\lambda \in \Lambda}$ là tự do đại số trên $k_0$ trong $\kappa_A$; do đó, $\varphi(u)$ là khả nghịch trong vành địa phương A. Suy ra rằng $\varphi$ mở rộng thành một đồng cấu $\psi$ của trường $k_1 = k_0((X_{\lambda})_{\lambda \in \Lambda})$ vào A. Khi đó A là một $k_1$-đại số, $\kappa_A$ là một mở rộng của $k_1$ và K là một mở rộng con của $\kappa_A$ là đại số và tách được trên $k_1$. Còn phải chứng minh rằng tồn tại duy nhất một trường con L của A chứa $\psi(k_1)$ và sao cho $\pi(L) = K$.

a) *Sự tồn tại của L*: Gọi S là tập hợp các trường con L của A, chứa $\psi(k_1)$ và sao cho $\pi(L) \subset K$; nó là quy nạp đối với quan hệ bao hàm. Gọi L là một phần tử cực đại của S; ta xem K như một mở rộng (đại số và tách được, theo A, V, p. 40, mệnh đề 9) của L. Gọi $\xi \in K$ và gọi $P \in L[X]$ là đa thức tối tiểu của nó trên L. Vì $\xi$ là một nghiệm đơn của P, bổ đề Hensel (III, § 4, no. 5, hệ quả 1 của định lý 2) đảm bảo sự tồn tại của một phần tử x của A sao cho $\pi(x) = \xi$ và $P(x) = 0$. Vành con $L[X]$ của A thuộc S; do tính chất cực đại của L, do đó ta có $x \in L$, do đó $\xi \in \pi(L)$. Cuối cùng ta có $\pi(L) = K$.

b) *Tính duy nhất của L*: Gọi L và L’ là hai trường con của A chứa $\psi(k_1)$ và sao cho $\pi(L) = \pi(L') = K$. Gọi $\xi \in K$, và gọi $x \in L$ và $x' \in L'$ là các phần tử sao cho $\pi(x) = \pi(x') = \xi$. Nếu $P \in k_1[X]$ là đa thức tối tiểu của $\xi$ trên $k_1$, thì $\xi$ là một nghiệm đơn của P, và ta có $P(x) = P(x') = 0$. Theo bổ đề Hensel (*loc. cit.*) ta có $x = x'$. Do đó $L = L'$.

#### Nhận xét {#ac-ix-s3-n2-rem-1 .statement}

\* Chứng minh trước đây áp dụng tổng quát hơn cho trường hợp người ta chỉ giả thiết rằng A là một vành địa phương hensel*. Chứng minh tính duy nhất sử dụng giả thiết rằng vành địa phương A là tách được, nhưng không sử dụng giả thiết rằng nó đầy đủ.

### 3. Các trường đại diện

#### Định nghĩa 1 {#ac-ix-s3-def-1 .statement}

*Cho A là một vành địa phương. Một trường đại diện của A là bất kỳ trường con K nào của A sao cho đồng cấu chính tắc của A lên $\kappa_A$ cảm sinh một đẳng cấu của K lên $\kappa_A$ (nói cách khác, sao cho $A = K + m_A$).*

Một trường đại diện của A chỉ có thể tồn tại nếu A có một đặc số. Điều kiện này là đủ khi A là tách được và đầy đủ. Chính xác hơn, ta có định lý sau:

#### Định lý 1 {#ac-ix-s3-thm-1 .statement}

*Cho A là một vành địa phương tách được và đầy đủ có đặc số p.*

a) *Giả sử $p = 0$ và $(x_\lambda)_{\lambda \in \Lambda}$ là một họ các phần tử của A mà các lớp của chúng modulo $m_A$ tạo thành một cơ sở siêu việt của $\kappa_A$ trên $\mathbf{Q}$. Có một trường đại diện duy nhất của A chứa các phần tử $x_\lambda$.*

b) *Giả sử $p \neq 0$. Cho $(x_\lambda)_{\lambda \in \Lambda}$ là một họ các phần tử của A mà các lớp của chúng modulo $m_A$ tạo thành một cơ sở p của $\kappa_A$ (A, V, p. 95). Có một trường đại diện duy nhất của A chứa các phần tử $x_\lambda$. Nó là một vành con Cohen của A.*

Giả sử rằng ta có $p = 0$, sao cho A là một $\mathbf{Q}$-đại số. Mọi cơ sở siêu việt của $\kappa_A$ trên $\mathbf{Q}$ đều là tách được, nên mệnh đề a) suy ra từ mệnh đề 1 của no. 1 áp dụng cho trường hợp $k_0 = \mathbf{Q}$, $K = \kappa_A$.

Bây giờ giả sử rằng ta có $p \neq 0$. Khi đó ta có $p1_A = 0$, và mọi vành con Cohen C của A thỏa mãn $pC = 0$. Nói cách khác, có sự đồng nhất giữa các khái niệm trường đại diện và vành con Cohen của A. Mệnh đề b) khi đó suy ra từ § 2, no. 2, định lý 1.

#### Hệ quả 1 {#ac-ix-s3-thm-1-cor-1 .statement}

Cho $A$ là một vành địa phương tách được và đầy đủ, có trường thặng dư là một mở rộng đại số của $\mathbf{Q}$. Khi đó tồn tại một trường đại diện duy nhất của $A$.
Thật vậy vành $A$ có đặc số 0 (no. 1).

#### Hệ quả 2 {#ac-ix-s3-thm-1-cor-2 .statement}

Cho $A$ là một vành địa phương tách được và đầy đủ có đặc số $p \neq 0$. Giả sử rằng trường thặng dư $\kappa_A$ là hoàn hảo. Khi đó tồn tại một trường đại diện duy nhất của $A$, cụ thể là tập hợp các đại diện nhân.
Hệ quả 2 suy ra ngay lập tức từ định lý 1 và mệnh đề 7 của § 2, no. 4.

#### Định lý 2 {#ac-ix-s3-thm-2 .statement}

Cho $A$ là một vành địa phương Noether đầy đủ có chiều $d$ chứa một trường. Cho $K$ là một trường hệ số của $A$, và cho $m$ là chiều của không gian vectơ $m_A/m_A^2$ trên trường $K$.
a) Tồn tại một iđêan $a$ của $K[[T_1, ..., T_m]]$ sao cho đại số $K$ $A$ là đẳng cấu với $K[[T_1, ..., T_m]]/a$.
b) Tồn tại một đại số con-$K$ $A'$ của $A$, đẳng cấu với $K[[T_1, ..., T_d]]$ và sao cho $A$ là một đại số hữu hạn trên $A'$.
c) Giả sử vành địa phương Noether $A$ là chính quy, tức là $d = m$. Khi đó tồn tại một $K$-đẳng cấu từ $A$ lên $K[[T_1, ..., T_d]]$.
Cho $t_1, ..., t_m$ là các phần tử của $m_A$ mà các lớp của chúng modulo $m_A^2$ sinh không gian vectơ $m_A/m_A^2$ trên $K$. Theo bổ đề 3 của § 2, No. 5, tồn tại một đồng cấu $K$ toàn ánh từ $K[[T_1, ..., T_m]]$ vào $A$, ánh xạ $T_i$ thành $t_i$ với $1 \leq i \leq m$. Điều này chứng minh $a$.
Tương tự, mệnh đề $b$ suy ra từ bổ đề 4 của cùng chỗ đã dẫn và từ sự tồn tại của một dãy cát tuyến cực đại đối với $A$ (VIII, § 3, No. 2, Định lý 1).
Cuối cùng, mệnh đề $c$ không gì khác ngoài hệ quả 3 của Định lý 1 của VIII, § 5, No. 2.

## BÀI TẬP {#ac-ix-s3-exercises}

Xem [các bài tập cho § 3](exercises/s3/).
