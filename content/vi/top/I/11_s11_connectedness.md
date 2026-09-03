---
book: top
book_title: General Topology
chapter: I
chapter_title: Topological Structures
section: 11
section_title: Connectedness
lang: vi
source: top-i-iv
pdf_pages: 0113-0122, 0161-0167
extraction: ocr
subsections:
    - "no": 1
      title: CONNECTED SPACES AND CONNECTED SETS
      page: 0
      pdf_page: 113
    - "no": 2
      title: IMAGE OF A CONNECTED SET UNDER A CONTINUOUS MAPPING
      page: 0
      pdf_page: 115
    - "no": 3
      title: QUOTIENT SPACES OF A CONNECTED SPACE
      page: 0
      pdf_page: 116
    - "no": 4
      title: PRODUCT OF CONNECTED SPACES
      page: 0
      pdf_page: 116
    - "no": 5
      title: COMPONENTS
      page: 0
      pdf_page: 116
    - "no": 6
      title: LOCALLY CONNECTED SPACES
      page: 0
      pdf_page: 118
    - "no": 7
      title: 'APPLICATION : THE POINCARÉ-VOLTERRA THEOREM'
      page: 0
      pdf_page: 120
statements: 28
exercises: 25
content_sha256: acc64c08f0f23ffd3fd329fd286f91f9f0b8a4018a1de5b40e968fd7f40ffd10
translated_from: content/en/top/I/11_s11_connectedness.md
source_content_sha256: f12b0f535c856eb0eec6548992165cda0fcb6dde9247c96a02db10d1ed77685b
translation_model: gpt-5-6, gpt-5.4-mini
translation_run: translate-vi-a6bc2cb7
glossary_version: 34
glossary_terms_sha256: 9b534be55d8d9fab2b4309b0d7cadbee2a337f6b52510c41550a3009b5ec8071
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 11. TÍNH LIÊN THÔNG

### 1. CÁC KHÔNG GIAN LIÊN THÔNG VÀ CÁC TẬP LIÊN THÔNG

#### Định nghĩa 1 {#top-i-s11-def-1 .statement}

Một không gian tôpô X được gọi là liên thông nếu nó không là hợp của hai tập mở rời nhau khác rỗng.

Một định nghĩa tương đương thu được bằng cách thay thế các từ "tập mở" bởi "tập đóng". X liên thông khi và chỉ khi các tập con duy nhất của X vừa mở vừa đóng là tập rỗng và toàn bộ không gian X.

Nếu X liên thông và nếu A, B là hai tập con mở (tương ứng, đóng) khác rỗng sao cho A \cup B = X, thì A \cap B \neq \emptyset.

#### Ví dụ 1 {#top-i-s11-n1-exa-1 .statement}

Ta sẽ thấy trong Chương IV, § 2, no. 5 rằng đường thẳng thực là liên thông, còn đường thẳng hữu tỉ thì không. \*
2) Một không gian rời rạc có nhiều hơn một điểm thì không liên thông.

#### Định nghĩa 2 {#top-i-s11-def-2 .statement}

*Một tập con $A$ của một không gian tôpô $X$ được gọi là một tập liên thông nếu không gian con $A$ của $X$ là liên thông.*

Để $A$ là một tập con liên thông của $X$ thì điều kiện cần và đủ là, đối với mỗi phủ của $A$ bởi hai tập con mở (hoặc đóng) $B, C$ của $X$ sao cho $A \cap B$ và $A \cap C$ là khác rỗng, ta có $A \cap B \cap C \neq \emptyset$.

#### Ví dụ {#top-i-s11-n1-exa-2 .statement}

Trong mọi không gian tôpô, tập rỗng và mọi tập hợp gồm một điểm duy nhất đều liên thông. Trong một không gian Hausdorff $X$, mọi tập hữu hạn gồm nhiều hơn một điểm đều không liên thông, và nói chung mọi tập con của $X$ có nhiều hơn một điểm và có ít nhất một điểm cô lập đều không liên thông.

Nếu một tập con trù mật $A$ là liên thông, thì toàn bộ không gian $X$ là liên thông; nếu không, sẽ tồn tại hai tập con mở rời nhau khác rỗng $M, N$ của $X$ sao cho $M \cup N = X$, và $M \cap A, N \cap A$ sẽ là hai tập con mở rời nhau khác rỗng của $A$ có hợp là $A$. Do đó ta có

#### Mệnh đề 1 {#top-i-s11-prop-1 .statement}

*Nếu $A$ là một tập liên thông, thì mọi tập hợp $B$ sao cho $A \subset B \subset \overline{A}$ là liên thông.*

#### Mệnh đề 2 {#top-i-s11-prop-2 .statement}

*Hợp của một họ các tập liên thông có giao khác rỗng là liên thông.*

Cho $(A_i)_{i \in I}$ là một họ các tập con liên thông của $X$, tất cả đều chứa cùng một điểm $x$; ta phải chỉ ra rằng

$$
A = \bigcup_i A_i
$$

là liên thông. Nếu không, tồn tại hai tập mở $B$ và $C$ sao cho $B \cap A$ và $C \cap A$ là khác rỗng, và $A \subset B \cup C$ và $A \cap B \cap C = \emptyset$. $x$ thuộc một trong các tập $B, C$, giả sử $x \in B$; mặt khác một trong các tập $A_i$, giả sử $A_x$, gặp $C$; do đó ta có $A_x \subset B \cup C$, $A_x \cap B \cap C = \emptyset$ và $B \cap A_x$ và $C \cap A_x$ là khác rỗng. Vậy $A_x$ không liên thông, điều này mâu thuẫn.

#### Hệ quả {#top-i-s11-n1-cor-1 .statement}

*Cho $(A_n)_{n \geq 0}$ là một dãy vô hạn các tập liên thông sao cho $A_{n+1} \cap A_n \neq \emptyset$ với mọi $n \geq 0$. Khi đó hợp $\bigcup_{n=0}^\infty A_n$ là liên thông.*

Bằng quy nạp theo $n$ ta thấy ngay lập tức rằng tập hợp $B_n = \bigcup_{i=0}^n A_i$ là liên thông với mọi $n$, theo Mệnh đề 2. Các tập hợp $B_n$ có giao khác rỗng; do đó hợp của chúng, bằng $\bigcup_{n=0}^\infty A_n$, là liên thông theo Mệnh đề 2.

#### Mệnh đề 3 {#top-i-s11-prop-3 .statement}

*Cho $A$ là một tập con của một không gian tôpô $X$. Nếu $B$ là một tập con liên thông của $X$ gặp cả $A$ và $\complement A$, thì $B$ gặp biên của $A$.*

Nếu không, các giao của $B$ với phần trong và phần ngoài của $A$ sẽ là hai tập con mở của $B$ lập thành một phân hoạch của $B$, và $B$ sẽ không liên thông.

#### Hệ quả {#top-i-s11-n1-cor-2 .statement}

*Trong một không gian liên thông $X$, mọi tập hợp không rỗng khác $X$ đều có ít nhất một điểm biên.*

### 2. ẢNH CỦA MỘT TẬP HỢP LIÊN THÔNG QUA MỘT ÁNH XẠ LIÊN TỤC

#### Mệnh đề 4 {#top-i-s11-prop-4 .statement}

*Cho $A$ là một tập con liên thông của một không gian tôpô $X$, và cho $f$ là một ánh xạ liên tục từ $X$ vào một không gian tôpô $X'$. Khi đó $f(A)$ là liên thông.*

Giả sử $f(A)$ không liên thông. Khi đó tồn tại hai tập hợp $M', N'$ mở trong $f^{-1}(A)$ và lập thành một phân hoạch của $f(A)$; do đó $A \cap f^{-1}(M')$ và $A \cap f^{-1}(N')$ là mở trong $A$ và lập thành một phân hoạch của $A$; điều này mâu thuẫn với giả thiết rằng $A$ liên thông.

*Ảnh ngược* của một tập hợp liên thông qua một ánh xạ liên tục không nhất thiết là liên thông; xét ví dụ một ánh xạ từ một không gian rời rạc vào một không gian gồm một điểm.

Từ Mệnh đề 4 ta suy ra một đặc trưng hóa khác của *các không gian không liên thông*:

#### Mệnh đề 5 {#top-i-s11-prop-5 .statement}

*Để một không gian tôpô $X$ không liên thông, điều kiện cần và đủ là tồn tại một ánh xạ liên tục toàn ánh từ $X$ lên một không gian rời rạc chứa nhiều hơn một điểm.*

Điều kiện này là đủ theo Mệnh đề 4. Ngược lại, nếu $X$ không liên thông, tồn tại hai tập con mở rời nhau không rỗng $A, B$ có hợp là $X$, và ánh xạ $f$ từ $X$ lên một không gian rời rạc gồm hai phần tử $\{a, b\}$, được xác định bởi $f(A) = \{a\}$ và $f(B) = \{b\}$, là liên tục.

### 3. CÁC KHÔNG GIAN THƯƠNG CỦA MỘT KHÔNG GIAN LIÊN THÔNG

#### Mệnh đề 6 {#top-i-s11-prop-6 .statement}

Mọi không gian thương của một không gian liên thông đều liên thông.

Đây là một hệ quả ngay lập tức của Mệnh đề 4 của no. 2.

#### Mệnh đề 7 {#top-i-s11-prop-7 .statement}

Cho $X$ là một không gian tôpô và $R$ là một quan hệ tương đương trên $X$. Nếu không gian thương $X/R$ liên thông, và nếu mỗi lớp tương đương mod $R$ là liên thông, thì $X$ liên thông.

Giả sử $X$ không liên thông. Khi đó có một phân hoạch của $X$ thành hai tập mở $A, B$. Các tập $A, B$ là bão hòa đối với $R$; vì nếu $x \in A$ thì lớp tương đương $M$ của $x$ không thể gặp $B$, nếu không các tập $A \cap M, B \cap M$ sẽ tạo thành một phân hoạch của $M$ thành hai tập mở trong $M$, điều này là không thể vì $M$ liên thông. Các ảnh chính tắc của $A$ và $B$ do đó là các tập mở trong $X/R$ và tạo thành một phân hoạch của $X/R$; điều này mâu thuẫn với giả thiết rằng $X/R$ liên thông.

### 4. TÍCH CỦA CÁC KHÔNG GIAN LIÊN THÔNG

#### Mệnh đề 8 {#top-i-s11-prop-8 .statement}

Mọi tích của các không gian liên thông đều liên thông. Ngược lại, nếu một tích của các không gian khác rỗng là liên thông, thì mỗi không gian nhân tử đều liên thông.

Cho $X = \prod_{i \in I} X_i$ là một tích của các không gian tôpô. Nếu các $X_i$ khác rỗng, ta có $X_i = \operatorname{pr}_i X$ với mỗi $i \in I$; do đó nếu $X$ liên thông thì các $X_i$ cũng liên thông (no. 2, Mệnh đề 4). Ngược lại, giả sử rằng mỗi $X_i$ liên thông và $X$ không liên thông. Theo Mệnh đề 5 của no. 2, tồn tại một ánh xạ toàn ánh liên tục $f : X \to X'$, trong đó $X'$ là một không gian rời rạc chứa nhiều hơn một điểm. Cho $a = (a_i)$ là một điểm bất kỳ của $X$, và $x$ là một chỉ số bất kỳ; ánh xạ từng phần $f_x : X_x \to X'$, được xác định bởi $f_x(x) = f((y_i))$ trong đó $y_x = x$ và $y_i = a_i$ nếu $i \neq x$, là liên tục trên $X_x$; vì $X_x$ liên thông, $f_x$ phải là hằng trên $X_x$. Suy ra ngay lập tức bằng quy nạp rằng $f(x) = f(a)$ đối với mọi điểm $x = (x_i)$ sao cho $x_i = a_i$ với mọi chỉ số $i \in I$ trừ một số hữu hạn. Nhưng các điểm $x$ này tạo thành một tập con trù mật của $X$ (§ 4, no. 3, Mệnh đề 8). Do đó $f$ liên tục trên $X$ và hằng trên một tập con trù mật của $X$, và vì vậy hằng trên $X$ (§ 8, no. 1, Mệnh đề 2, Hệ quả 1). Nhưng điều này mâu thuẫn với định nghĩa của $f$.

### 5. CÁC THÀNH PHẦN

Cho một điểm $x$ của một không gian tôpô $X$, hợp của các tập con liên thông của $X$ chứa $x$ là liên thông (no. 1, Mệnh đề 2); do đó nó là tập con liên thông lớn nhất của $X$ whi chứa $x$.

#### Định nghĩa 3 {#top-i-s11-def-3 .statement}

Thành phần (hay thành phần liên thông) của một điểm của một không gian tôpô $X$ là tập con liên thông lớn nhất của $X$ chứa điểm này. Các thành phần của một tập con $A$ của $X$ là các thành phần của các điểm của $A$, xét trong không gian con $A$ của $X$.

Nếu một không gian liên thông, thì thành phần của mỗi điểm là toàn bộ không gian. Nếu một không gian $X$ sao cho với mỗi cặp $(x, y)$ điểm của $X$ đều có một tập hợp liên thông chứa $x$ và $y$, thì $X$ liên thông.

Một không gian $X$ được gọi là *hoàn toàn không liên thông* nếu thành phần của mỗi điểm của $X$ chỉ gồm riêng điểm đó. Một tập con $A$ của $X$ là một *tập hoàn toàn không liên thông* nếu không gian con $A$ của $X$ là hoàn toàn không liên thông.

Một không gian *rời rạc* là hoàn toàn không liên thông, nhưng cần tránh lẫn lộn hai khái niệm này; chẳng hạn, ta sẽ thấy trong Chương IV, § 2, no. 5, rằng trục hữu tỉ, không phải là một không gian rời rạc, thì hoàn toàn không liên thông.

Một tập hợp *vừa mở vừa đóng* chứa thành phần của mỗi điểm của nó, do đó *thành phần của một điểm được chứa trong giao của các tập hợp vừa mở vừa đóng và chứa điểm này*. Tuy nhiên, thành phần của một điểm không nhất thiết bằng giao này (xem Bài tập 9 và Chương II, § 4, no. 4, Mệnh đề 6).

#### Mệnh đề 9 {#top-i-s11-prop-9 .statement}

*Thành phần của mọi điểm trong một không gian tôpô $X$ là một tập đóng. Quan hệ "y thuộc thành phần của x" là một quan hệ tương đương $R \{ x, y \}$ trên $X$, và các lớp tương đương chính là các thành phần của $X$. Không gian thương $X/R$ là hoàn toàn không liên thông.*

Phần đầu của mệnh đề là một hệ quả trực tiếp của Định nghĩa 3 và thực tế rằng bao đóng của một tập liên thông thì liên thông (no. 1, Mệnh đề 1). Vì hợp của các tập liên thông có chung một điểm là liên thông (no. 1, Mệnh đề 2), quan hệ $R$ là bắc cầu, do đó là một quan hệ tương đương (vì nó hiển nhiên phản xạ và đối xứng) và lớp tương đương của $x$ theo $R$ chính là thành phần của $x$. Còn lại cần chứng minh rằng $X/R$ là hoàn toàn không liên thông. Gọi $f : X \to X/R$ là ánh xạ chính tắc, và gọi $F$ là một tập đóng trong $X/R$ *chứa ít nhất hai điểm phân biệt*; ảnh ngược $f^{-1}(F)$ của $F$ là tập đóng trong $X$, bão hòa đối với $R$, và chứa ít nhất hai thành phần phân biệt của $X$ và do đó *không liên thông*. Vậy tồn tại hai tập đóng không rỗng $B, C$ trong $X$ sao cho $B \cap C = \varnothing$ và $B \cup C = f^{-1}(F)$. Thành phần của mọi điểm $x$ của $f^{-1}(F)$ *trong* $f^{-1}(F)$ là thành phần của $x$ *trong* $X$ (theo định nghĩa của $R$) và do đó $B$ và $C$, cả hai đều vừa mở vừa đóng *trong* $f^{-1}(F)$, đều bão hòa đối với $R$. Do đó $f(B)$ và $f(C)$ là các tập đóng trong $X/R$, và $f(B) \cup f(C) = F$ và $f(B) \cap f(C) = \varnothing$; điều này cho thấy rằng $F$ *không liên thông* và do đó $X/R$ là hoàn toàn không liên thông.

#### Mệnh đề 10 {#top-i-s11-prop-10 .statement}

Trong một không gian tích $X = \prod_{i \in J} X_i$, thành phần của $x = (x_i)$ trong $X$ là tích của các thành phần của $x_i$ trong các thừa số $X_i$.

Tập tích này liên thông (no. 4, Mệnh đề 8). Ngược lại, nếu $A$ là một tập con liên thông của $X$ chứa $x$, thì $\operatorname{pr}_i(A)$ là một tập liên thông (no. 2, Mệnh đề 4) chứa $x$; vì $A \subset \prod_i \operatorname{pr}_i(A)$, suy ra $A$ được chứa trong tích của các thành phần của $x_i$.

### 6. CÁC KHÔNG GIAN ĐỊA PHƯƠNG LIÊN THÔNG

#### Định nghĩa 4 {#top-i-s11-def-4 .statement}

Một không gian tôpô $X$ được gọi là địa phương liên thông nếu mỗi điểm của $X$ có một hệ cơ bản các lân cận liên thông.

\* Ta sẽ thấy ở Chương IV, § 2, no. 5, rằng đường thẳng thực là một không gian địa phương liên thông. \*
Sự tồn tại, tại mỗi điểm $x$ của một không gian $X$, của một lân cận liên thông của $x$ hoàn toàn không suy ra rằng $X$ là địa phương liên thông. Đặc biệt, $X$ có thể liên thông nhưng không địa phương liên thông (Bài tập 2 và 13). Ngược lại, một không gian có thể địa phương liên thông nhưng không liên thông (chẳng hạn một không gian rời rạc chứa nhiều hơn một điểm).

#### Mệnh đề 11 {#top-i-s11-prop-11 .statement}

Điều kiện cần và đủ để một không gian $X$ là địa phương liên thông là mỗi thành phần của một tập mở trong $X$ đều mở trong $X$.

Điều kiện ấy là đủ, vì khi đó thành phần của $x$ tương đối với một lân cận mở của $x$ là một lân cận của $x$ trong $X$.

Ngược lại, cho $A$ là một tập con mở của một không gian địa phương liên thông $X$, cho $B$ là một thành phần của $A$, và cho $x \in B$. Cho $V$ là một lân cận liên thông của $x$ được chứa trong $A$; theo định nghĩa của các thành phần, $V$ được chứa trong $B$; do đó $B$ là mở trong $X$ (§ 1, no. 2, Mệnh đề 1).

Các thành phần của một không gian địa phương liên thông $X$ do đó lập thành một phân hoạch của $X$ thành các tập mở, và suy ra $X$ là tổng (§ 2, no. 4, Ví dụ 3) của các thành phần của nó.

#### Hệ quả {#top-i-s11-n6-cor-1 .statement}

Cho $U$ là một tập con mở của một không gian địa phương liên thông $X$, và cho $V$ là một thành phần của $U$. Khi đó biên của $V$ (xét tương đối với $X$) được chứa trong biên của $U$.

Vì $V$ vừa mở vừa đóng trong $U$, nên một điểm biên của $V$ (xét tương đối với $X$) không thể thuộc $U$, bởi vì nó cũng sẽ là một điểm biên của $V$ tương đối với $U$, và không có điểm nào như thế.

#### Mệnh đề 12 {#top-i-s11-prop-12 .statement}

Mọi không gian thương của một không gian địa phương liên thông đều địa phương liên thông.

Cho $X$ là một không gian liên thông địa phương, $R$ một quan hệ tương đương trên $X$, $\varphi : X \to X/R$ là ánh xạ chính tắc. Cho $A$ là một tập con mở của

X/R và C là một thành phần của A. Khi đó $\overline{\varphi}^1(C)$ là hợp của các thành phần của $\overline{\varphi}^1(A)$; vì nếu $x \in \overline{\varphi}^1(C)$ và nếu K là thành phần của x trong $\overline{\varphi}^1(A)$ thì $\varphi(K)$ liên thông (no. 2, Proposition 4), được chứa trong A, và chứa $\varphi(x)$; do đó $\varphi(K) \subset C$ theo định nghĩa của C, và vì thế $K \subset \overline{\varphi}^1(C)$. Vì X là liên thông địa phương và $\overline{\varphi}^1(A)$ là mở trong X, suy ra từ Proposition 11 rằng $\overline{\varphi}^1(C)$ là mở trong X; do đó C là mở trong X/R và vì vậy, lại theo Proposition 11, X/R là liên thông địa phương.

#### Mệnh đề 13 {#top-i-s11-prop-13 .statement}

a) Cho $(X_i)_{i \in I}$ là một họ các không gian liên thông địa phương sao cho $X_i$ liên thông với mọi chỉ số $i \in I$ trừ một số hữu hạn. Khi đó không gian tích $X = \prod_{i \in I} X_i$ là liên thông địa phương.

b) Ngược lại, nếu tích của một họ $(X_i)$ các không gian tôpô không rỗng là liên thông địa phương, thì mỗi $X_i$ đều liên thông địa phương, và $X_i$ liên thông với mọi chỉ số trừ một số hữu hạn.

a) Cho J là tập con hữu hạn của I sao cho $X_i$ không liên thông khi và chỉ khi $i \in J$. Cho
$$
U = \prod_{i \in I} U_i
$$
là một tập sơ cấp chứa một điểm $x = (x_i)$ của X và cho K là tập con hữu hạn của I sao cho $U_i \neq X_i$ khi và chỉ khi $i \in K$. Cho $V_i$ bằng $X_i$ với $i \notin J \cup K$, và cho $V_i$ là một lân cận liên thông của $x_i$ nằm trong $U_i$ với $i \in J \cup K$; khi đó
$$
V = \prod_{i \in I} V_i
$$
liên thông (theo Proposition 8 của no. 4) và là một lân cận của $x$ nằm trong U. Vậy X là liên thông địa phương.

b) Cho $a = (a_i)$ là một điểm của X và cho V là một lân cận liên thông của $a$ trong X. Vì ta có $\mathrm{pr}_i V = X_i$ trừ một số hữu hạn chỉ số (§ 4, no. 1) suy ra từ no. 2, Proposition 4 rằng các $X_i$ là liên thông, với mọi chỉ số trừ một số hữu hạn. Mặt khác, với mỗi $x \in I$, mỗi $a_x \in X_x$ và mỗi lân cận $V_x$ của $a_x$ trong $X_x$, có một điểm $x$ của X sao cho $\mathrm{pr}_x x = a_x$, và
$$
V = V_x \times \prod_{i \neq x} X_i
$$
là một lân cận của $x$ trong X; do đó V chứa một lân cận liên thông W của $x$, có ảnh chiếu $\mathrm{pr}_x W$ là một lân cận liên thông của $a_x$ nằm trong $V_x$ (no. 2, Proposition 4 và § 4, no. 2, Proposition 5). Vậy mỗi $X_x$ đều liên thông địa phương.

### 7. ỨNG DỤNG : ĐỊNH LÝ POINCARÉ-VOLTERRA

#### Định lý 1 {#top-i-s11-thm-1 .statement}

Cho $X$ là một không gian tôpô thỏa mãn tiên đề $(O_{III})$ (nhưng không nhất thiết Hausdorff), và giả sử $X$ liên thông và liên thông địa phương. Cho $Y$ là một không gian tôpô mà tôpô của nó có một cơ sở đếm được, và cho $p : X \to Y$ là một ánh xạ liên tục sao cho, với mỗi $y \in Y$, $\overline{p}^{-1}(y)$ là một không gian con rời rạc của $X$. Cuối cùng, cho $\mathcal{B}$ là một tập hợp các tập con của $X$ có các miền trong phủ $X$ và sao cho:
(i) *Phép hạn chế của* $p$ *lên từng* $V \in \mathcal{B}$ *là một ánh xạ đóng từ* $V$ *vào* $Y$.
(ii) *Mỗi* $V \in \mathcal{B}$ *đều có một tập con đếm được trù mật trong* $V$.

*Khi đó không gian* $X$ *là hợp của một họ đếm được các tập mở, mỗi tập đều được chứa trong một tập của* $\mathcal{B}$.

Cho $\mathcal{B}$ là một cơ sở đếm được của tôpô của $Y$. Ta sẽ gọi một cặp $(W, U)$ là *phân biệt* nếu (i) $U \in \mathcal{B}$ và (ii) $W$ là một thành phần của $\overline{p}^{-1}(U)$ được chứa trong một tập của $\mathcal{B}$.

#### Bổ đề 1 {#top-i-s11-lem-1 .statement}

*Nếu* $x$ *là một điểm bất kỳ của* $X$, *thì tồn tại một cặp phân biệt* $(W, U)$ *sao cho* $x \in W$.

Ảnh ngược $\overline{p}^{-1}(p(x))$ là rời rạc và do đó có một lân cận của $x$ trong $X$ mà mọi điểm $x'$ khác $x$ đều có ảnh $p(x') \neq p(x)$; vì $X$ thỏa mãn $(O_{III})$, có một lân cận *đóng* $V$ của $x$ có tính chất này, và ta cũng có thể giả sử rằng $V$ được chứa trong một tập của $\mathcal{B}$. Cho $F$ là biên của $V$ trong $X$. Theo điều kiện (i) của định lý, $p(F)$ là đóng trong $Y$; và vì $p(F)$ không chứa $p(x)$, có một tập $U \in \mathcal{B}$ chứa $p(x)$ và không giao với $p(F)$. Cho $W$ là thành phần của $x$ trong $\overline{p}^{-1}(U)$; khi đó chỉ cần chứng minh rằng $W \subset \mathbb{A}$. Nếu không phải như vậy, thì $W$ sẽ giao với $F$ (số 1, Mệnh đề 3) và do đó $p(F)$ sẽ giao với $U$, trái với định nghĩa của $U$.

#### Bổ đề 2 {#top-i-s11-lem-2 .statement}

*Nếu* $(W, U)$ *là một cặp đặc biệt thì tập hợp tất cả các cặp đặc biệt* $(W', U')$ *sao cho* $W'$ *giao với* $W$ *là đếm được*.

Vì $\mathcal{B}$ là đếm được nên chỉ cần chứng minh rằng, cho $U' \in \mathcal{B}$, tập các cặp phân biệt $(W', U')$ sao cho $W'$ giao với $W$ là đếm được. Các tập $W'$ này đều mở, vì $X$ là liên thông địa phương (no. 6, Mệnh đề 11) và đôi một rời nhau vì chúng là các thành phần của $\overline{p}^{-1}(U')$; do đó các tập $W' \cap W$ đều mở và đôi một rời nhau. Nhưng $W$ chứa một tập con đếm được trù mật trong $W$; vì vậy tập các $W'$ sao cho $W' \cap W$ không rỗng cũng đếm được.

To prove Theorem 1, xét quan hệ R sau đây giữa hai điểm x, x' của X: "Tồn tại một dãy hữu hạn các cặp đặc biệt (W_i, U_i) (1 \leq i \leq n) sao cho x \in W_1 và x' \in W_n và W_i \cap W_{i+1} \neq \emptyset for \leq 1 i \leq n — 1."

Bổ đề 1 cho biết rằng R là phản xạ, và dễ dàng kiểm tra rằng R là đối xứng và bắc cầu, nên R là một quan hệ tương đương; hơn nữa, vì các W_i là mở, mỗi lớp tương đương mod R đều mở trong X. Nhưng X liên thông; do đó chỉ có thể có một lớp tương đương, tức là bất kỳ hai điểm nào của X cũng tương đương mod R. Từ đây ta suy ra rằng X là hợp của một họ đếm được các thành phần thứ nhất của các cặp đặc biệt, và điều này sẽ chứng minh Định lý 1. Để làm điều đó, lấy x là một điểm bất kỳ của X, và định nghĩa bằng quy nạp theo n một dãy (C_n) các tập con mở của X như sau: theo Bổ đề 1, có một cặp đặc biệt (W_1, U_1) sao cho x \in W_1, và ta lấy C_1 = W_1; nếu n > 1 thì C_n được lấy bằng hợp của mọi thành phần thứ nhất W của các cặp đặc biệt (W, U) sao cho W giao với C_{n-1}. Bằng quy nạp theo n, nhờ Bổ đề 2, suy ra ngay rằng C_n là một hợp đếm được các thành phần thứ nhất của các cặp đặc biệt. Cuối cùng, mọi x' \in X đều thuộc một C_n nào đó; thật vậy, tồn tại một dãy hữu hạn

$$(W'_i, U'_i)_{1 \leq i \leq m}$$

các cặp đặc biệt sao cho x \in W'_1, x' \in W'_m và W'_i \cap W'_{i+1} \neq \emptyset for 1 \leq i \leq m — 1, và bằng quy nạp theo i ta thấy rằng W'_i \subset C_{i+1} đối với mọi i, do đó x' \in C_{m+1}.

Q.E.D.

#### Hệ quả 1 {#top-i-s11-lem-2-cor-1 .statement}

Cho Y là một không gian chính quy có tôpô có một cơ sở đếm được (*). Cho X là một không gian liên thông và liên thông địa phương, và cho p : X \to Y là một ánh xạ liên tục có tính chất sau: với mỗi x \in X, có một lân cận đóng V của x trong X sao cho hạn chế của p lên V là một đồng phôi của V lên một không gian con đóng của Y. Khi đó X là chính quy và tôpô của X có một cơ sở đếm được.

Trước hết, các giả thiết suy ra rằng X là chính quy (§ 8, no. 4, Mệnh đề 13). Ta hãy chứng minh rằng các điều kiện của Định lý 1 được thỏa mãn nếu ta lấy \mathfrak{B} là tập hợp mọi tập con đóng V của X sao cho hạn chế của p lên V là một đồng phôi của V lên một không gian con đóng của Y. Theo giả thiết, các phần trong của các tập thuộc \mathfrak{B} phủ Y và, nhờ giả thiết về Y, mỗi V \in \mathfrak{B} có một cơ sở đếm được và do đó chứa một tập con đếm được trù mật (§ 1, no. 6, Mệnh đề 6). Hơn nữa, nếu x \in p^{-1}(y), thì có một lân cận V \in \mathfrak{B} của x trong X sao cho V

(*) \* Có thể chứng minh rằng các điều kiện này suy ra tôpô của Y là mêtric hóa được (Chương IX, § 4, Bài tập 22). \*

chứa không điểm nào của $\overline{p}^{-1}(y)$ ngoài $x$, và do đó $\overline{p}^{-1}(y)$ là một không gian rời rạc. Vì vậy ta có thể áp dụng Định lý 1, điều này cho thấy rằng $X$ là hợp của một họ đếm được $(T_n)_{n \geq 0}$ các tập mở, sao cho mỗi không gian con $T_n$ có một cơ sở đếm được $(U_{mn})_{m \geq 0}$. Khi đó các $U_{mn}$ ($m \geq 0, n \geq 0$) tạo thành một cơ sở của tôpô của $X$ ($§ 3$, no. 1, Nhận xét).

#### Hệ quả 2 {#top-i-s11-lem-2-cor-2 .statement}

*Cho $X$ là địa phương compact, liên thông và liên thông địa phương, và giả sử mỗi điểm của $X$ có một lân cận có một cơ sở đếm được. Cho $Y$ là một không gian Hausdorff mà tôpô của nó có một cơ sở đếm được, và cho $p : X \to Y$ là một ánh xạ liên tục sao cho, với mỗi $y \in Y$, $\overline{p}^{-1}(y)$ là một không gian con rời rạc của $X$. Khi đó tôpô của $X$ có một cơ sở đếm được.*

Với mỗi $x \in X$, cho $V_x$ là một lân cận compact của $x$ trong $X$ có một cơ sở đếm được. Suy ra từ $§ 9$, no. 4, Định lý 2, Hệ quả 2, rằng tập hợp $\mathcal{B}$ gồm các $V_x$ thỏa mãn các điều kiện của Định lý 1, và ta hoàn tất chứng minh như trong Hệ quả 1.

Lưu ý rằng, trong hệ quả này, có thể xảy ra rằng sự hạn chế của $p$ lên một lân cận $V$ tùy ý nhỏ của một điểm của $X$ *không là một đẳng cấu tôpô của $V$ lên $p(V)$*.

#### Hệ quả 3 (Định lý Poincaré-Volterra) {#top-i-s11-lem-2-cor-3 .statement}

*Cho $Y$ là một không gian địa phương compact, địa phương liên thông mà tôpô của nó có một cơ sở đếm được. Cho $X$ là một không gian Hausdorff liên thông, và cho $p : X \to Y$ là một ánh xạ liên tục có tính chất sau : với mỗi $x \in X$ tồn tại một lân cận mở $U$ của $x$ trong $X$ sao cho sự hạn chế của $p$ lên $U$ là một đẳng cấu tôpô của $U$ lên một không gian con mở của $Y$. Khi đó $X$ là địa phương compact và địa phương liên thông, và tôpô của $X$ có một cơ sở đếm được.*

Rõ ràng $X$ là địa phương liên thông. Cũng vậy, mỗi $x \in X$ có một lân cận mở $U$ trong $X$ sao cho sự hạn chế của $p$ lên $U$ ánh xạ $U$ đẳng cấu tôpô lên một không gian con mở $p(U)$ của $Y$. Vì $p(U)$ là một không gian con compact địa phương của $Y$ ($§ 9$, no. 7, Mệnh đề 13), nên tồn tại một lân cận compact $W$ của $p(x)$ được chứa trong $p(U)$, do đó $U \cap \overline{p}^{-1}(W)$ là một lân cận compact của $x$ được chứa trong $U$; vậy $X$ là địa phương compact, vì theo giả thiết $X$ là Hausdorff. $U \cap \overline{p}^{-1}(W)$, là compact, nên đóng trong $X$ ($§ 9$, no. 3, Mệnh đề 4) và do đó các điều kiện của Hệ quả 1 được thỏa mãn; suy ra tôpô của $X$ có một cơ sở đếm được.

### Bài tập {#top-i-s11-exercises}

Xem [các bài tập cho § 11](exercises/s11/).
