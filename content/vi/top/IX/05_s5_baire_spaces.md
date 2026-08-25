---
book: top
book_title: General Topology
chapter: IX
chapter_title: Use of real numbers in general topology
section: 5
section_title: Baire spaces
lang: vi
source: top-v-x
pdf_pages: 0196-0201, 0256-0264
extraction: ocr
subsections:
    - "no": 1
      title: NOWHERE DENSE SETS
      page: 0
      pdf_page: 196
    - "no": 2
      title: MEAGRE SETS
      page: 0
      pdf_page: 198
    - "no": 3
      title: BAIRE SPACES
      page: 0
      pdf_page: 198
    - "no": 4
      title: SEMI-CONTINUOUS FUNCTIONS ON A BAIRE SPACE
      page: 0
      pdf_page: 200
statements: 16
exercises: 4
content_sha256: 9ec0e0174ab7ef23c3cf99deda9c629226e7f22f12aaa138e7aadc829ac948f0
translated_from: content/en/top/IX/05_s5_baire_spaces.md
source_content_sha256: a78fb82444d16ea24a2754a196d4056a293a2226bea0b831a8a986b6b09a213a
translation_model: gpt-5-6-mini
translation_run: translate-vi-a1691418
glossary_version: 34
glossary_terms_sha256: a151d17e036a08e243bd31bf436306536e909e36f7a79807601b14541e221994
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 5. KHÔNG GIAN BAIRE

### 1. TẬP HỢP KHÔNG TRÙ MẬT

#### Định nghĩa 1 {#top-ix-s5-def-1 .statement}

*Một tập con $A$ của một không gian tôpô $X$ được gọi là không trù mật nếu bao đóng của nó không có điểm trong.*

Tương đương, $A$ không trù mật trong $X$ khi và chỉ khi phần ngoài của $A$ trù mật trong $X$.

Một tập đóng $A$ không trù mật khi và chỉ khi nó không có điểm trong; tức là, khi và chỉ khi nó trùng với biên của nó. Một tập con tùy ý $A$ không trù mật khi và chỉ khi bao đóng của $A$ không trù mật. Mọi tập con của một tập không trù mật đều không trù mật.

#### Ví dụ 1 {#top-ix-s5-n1-exa-1 .statement}

Tập con rỗng của $X$ là không trù mật. Trong một không gian Hausdorff $X$, một tập gồm một điểm duy nhất là không trù mật khi và chỉ khi điểm đó không cô lập trong $X$. Một tập con trù mật không bao giờ không trù mật (trừ khi $X = \emptyset$).

#### Ví dụ 2 {#top-ix-s5-n1-exa-2 .statement}

Biên của một tập mở hoặc một tập đóng luôn không trù mật.

#### Ví dụ 3 {#top-ix-s5-n1-exa-3 .statement}

Trong không gian $\mathbf{R}^n$, mọi không gian con tuyến tính có chiều $p < n$ đều là một tập không trù mật (Chương VI, § 1, no. 4, Mệnh đề 2).

#### Nhận xét {#top-ix-s5-n1-rem-1 .statement}

Biên của một tập con tùy ý không nhất thiết phải không trù mật: chẳng hạn, nếu $A$ và $\overline{C}A$ đều là các tập trù mật, thì biên của $A$ là toàn bộ không gian.

#### Mệnh đề 1 {#top-ix-s5-prop-1 .statement}

*Hợp của một số hữu hạn các tập không trù mật là không trù mật.*

Chỉ cần chứng minh rằng hợp của hai tập không trù mật $A, B$ là không trù mật, và không mất tính tổng quát, ta có thể giả sử rằng $A$ và $B$ là đóng. Khi đó mệnh đề tương đương với việc nói rằng giao của hai tập mở trù mật $\overline{C}A, \overline{C}B$ là trù mật. Nếu $U$ là một tập mở không rỗng, thì $U \cap \overline{C}A$ là mở và không rỗng, do đó

$$
(U \cap \overline{C}A) \cap \overline{C}B = U \cap (\overline{C}A \cap \overline{C}B)
$$

là mở và không rỗng.

Cho $Y$ là một không gian con của một không gian tôpô $X$. Một không gian con $A$ của $Y$ được gọi là *không trù mật tương đối đối với* $Y$ nếu $A$ là không trù mật khi được xét như một tập con của không gian tôpô $Y$.

#### Mệnh đề 2 {#top-ix-s5-prop-2 .statement}

*Cho $Y$ là một không gian con của một không gian tôpô $X$, và cho $A$ là một tập con của $Y$. Nếu $A$ không trù mật tương đối đối với $Y$, thì $A$ không trù mật tương đối đối với $X$. Ngược lại, nếu $Y$ mở trong $X$ và $A$ không trù mật tương đối đối với $X$, thì $A$ không trù mật tương đối đối với $Y$.*

Giả sử rằng $A$ không trù mật tương đối đối với $Y$. Nếu bao đóng $\overline{A}$ của $A$ trong $X$ chứa một tập mở không rỗng $U$, thì $U \cap A$ không rỗng (theo định nghĩa của bao đóng); do đó $U \cap Y$ là một tập mở không rỗng tương đối đối với $Y$, và được chứa trong bao đóng $\overline{A} \cap Y$ của $A$ đối với $Y$, trái với giả thiết.

Bây giờ giả sử rằng $Y$ là mở trong $X$ và $A \subset Y$ là không trù mật nơi nào tương đối với $X$. Nếu $U$ là mở trong $Y$ và không rỗng, thì $U$ là mở trong $X$ và do đó chứa một tập hợp $V$ không rỗng, mở trong $X$ (và *a fortiori* trong $Y$) và không giao với $A$; suy ra $A$ là không trù mật nơi nào tương đối với $Y$.

Phần thứ hai của Mệnh đề 2 rõ ràng không đúng nếu $Y$ không mở trong $X$; xét, chẳng hạn, trường hợp $Y \neq \emptyset$ là không trù mật nơi nào trong $X$, và $A = Y$.

### 2. CÁC TẬP HỢP THƯA

#### Định nghĩa 2 {#top-ix-s5-def-2 .statement}

*Một tập con* $A$ *của một không gian tôpô* $X$ *được gọi là thưa nếu nó là hợp của một họ đếm được các tập hợp không trù mật nơi nào.*

Tương đương, $A$ là thưa nếu nó được chứa trong một hợp đếm được các tập hợp đóng mà mỗi tập đều không có điểm trong.

Một tập hợp thưa hoàn toàn có thể *trù mật* trong $X$; thậm chí toàn bộ không gian $X$ cũng có thể tự nó là một tập hợp thưa.

Một ví dụ về khả năng sau được cho bởi bất kỳ không gian Hausdorff *đếm được* nào không có điểm cô lập, chẳng hạn, đường hữu tỉ $\mathbf{Q}$. Nhưng một không gian tôpô $X$ là một tập hợp thưa trong $X$ không nhất thiết phải đếm được (xem Bài tập 9).

Mọi tập con của một tập hợp thưa trong một không gian $X$ đều thưa, và hợp của một họ *đếm được* các tập hợp thưa là thưa.

Cho $Y$ là một không gian con của $X$. Một tập con $A$ của $Y$ được gọi là *thưa tương đối với* $Y$ nếu $A$ là thưa khi được xem như một tập con của không gian tôpô $Y$. Theo Mệnh đề 2 của no. 1, nếu $A$ là một tập con của $Y$ thưa tương đối với $Y$, thì $A$ thưa tương đối với $X$; và nếu thêm $Y$ là *mở* trong $X$, thì mọi tập con $A$ của $Y$ thưa tương đối với $X$ đều thưa tương đối với $Y$.

### 3. CÁC KHÔNG GIAN BAIRE

#### Định nghĩa 3 {#top-ix-s5-def-3 .statement}

*Một không gian tôpô* $X$ *được gọi là một không gian Baire nếu nó thỏa mãn một trong hai điều kiện tương đương sau:*

*(EB)* *Mọi giao đếm được của các tập hợp mở trù mật trong* $X$ *đều trù mật trong* $X$.
*(EB')* *Mọi hợp đếm được của các tập hợp đóng không có điểm trong* $X$ *đều không có điểm trong* $X$.

Tiên đề (EB) có thể được phát biểu dưới hai dạng tương đương khác:

*(EB'')* *Mọi tập hợp mở không rỗng trong* $X$ *đều không thưa.*

Thật vậy, một tập hợp là thưa khi và chỉ khi nó được chứa trong một hợp đếm được các tập hợp đóng không có điểm trong.

(EB'') *Phần bù của một tập hợp thưa trong $X$ là trù mật trong $X$.*

Điều này có nghĩa là một tập hợp thưa không thể chứa một tập hợp mở không rỗng, và do đó tương đương với (EB").

#### Mệnh đề 3 {#top-ix-s5-prop-3 .statement}

*Mọi không gian con mở không rỗng $Y$ của một không gian Baire $X$ đều là một không gian Baire.*

Điều này suy ra từ (EB"), vì mọi tập hợp mở (t.ư. thưa) trong $Y$ đều mở (t.ư. thưa) trong $X$.

Theo Mệnh đề 3, mọi điểm của một không gian Baire đều có một hệ cơ sở các lân cận, mỗi lân cận trong đó là một không gian Baire. Ngược lại:

#### Mệnh đề 4 {#top-ix-s5-prop-4 .statement}

*Nếu mọi điểm của một không gian tôpô $X$ có một lân cận là một không gian Baire, thì $X$ là một không gian Baire.*

Cho $A$ là một tập mở không rỗng trong $X$, cho $x \in A$ và cho $V$ là một lân cận mở của $x$ là một không gian Baire. Nếu $A$ là tập loại thứ nhất trong $X$, thì $V \cap A$ sẽ là tập loại thứ nhất trong $V$ và mở trong $V$, điều này trái với giả thiết.

#### Mệnh đề 5 {#top-ix-s5-prop-5 .statement}

*Trong một không gian Baire $X$, phần bù của một tập loại thứ nhất là một không gian Baire.*

Cho $A$ là một tập loại thứ nhất trong $X$; khi đó phần bù $Y = \complement_A$ của nó trong $X$ là trù mật trong $X$. Cho $B$ là một tập loại thứ nhất tương đối đối với $Y$; $B$ cũng là tập loại thứ nhất tương đối đối với $X$, do đó $A \cup B$ là tập loại thứ nhất tương đối đối với $X$. Vì vậy phần bù của $A \cup B$ trong $X$, cũng là phần bù của $B$ trong $Y$, là trù mật trong $X$ và *a fortiori* trù mật trong $Y$. Do đó $Y$ là một không gian Baire.

#### Định lý 1 (Baire) {#top-ix-s5-thm-1 .statement}

(i) *Mọi không gian địa phương compact $X$ đều là một không gian Baire.* (ii) *Mọi không gian tôpô $X$ trên đó tồn tại một mêtric, tương thích với tôpô của $X$ và xác định trên $X$ cấu trúc của một không gian mêtric đầy đủ, đều là một không gian Baire.*

Ta sẽ chứng minh rằng tiên đề (EB) được thỏa mãn trong mỗi trường hợp. Cho $(A_n)$ là một dãy các tập mở trù mật trong $X$, và cho $G$ là một tập mở không rỗng bất kỳ. Khi đó ta có thể định nghĩa quy nạp một dãy $(G_n)$ các tập mở không rỗng sao cho $G_1 = G$ và $\overline{G}_{n+1} \subset G_n \cap A_n$: vì theo giả thiết $G_n$ không rỗng, nên $G_n \cap A_n$ là một tập mở không rỗng; và vì $X$ là *chính quy* trong cả hai trường hợp được xét, nên tồn tại một tập mở không rỗng $G_{n+1}$ sao cho $\overline{G}_{n+1} \subset G_n \cap A_n$. Do đó tập $G \cap \bigcap_{n=1}^\infty A_n$ chứa giao của các tập $G_n$, bằng giao của các tập $\overline{G}_n$; vì vậy chỉ cần chứng minh rằng $\bigcap_{n=1}^\infty \overline{G}_n \neq \varnothing$. Bây giờ nếu $X$ là địa phương compact, ta có thể giả sử rằng $\overline{G}_2$ là compact; trong không gian compact $\overline{G}_2$, các $\overline{G}_n (n \geq 2)$ tạo thành một dãy giảm các tập đóng không rỗng, và giao của chúng do đó không rỗng theo tiên đề (C'') (xem Chương I, § 9, no. 1, Định nghĩa 1]. Nếu $X$ là một không gian mêtric đầy đủ (đối với một mêtric tương thích với tôpô của nó), ta có thể giả sử rằng $\overline{G}_n$ đã được chọn sao cho đường kính của nó (đối với mêtric này) dần về 0 khi $n$ dần tới $+\infty$; do đó các $\overline{G}_n$ tạo thành một cơ sở lọc Cauchy hội tụ đến một điểm $x$, và $x$ nhất thiết thuộc giao của các tập $\overline{G}_n$.

Q.E.D.

#### Nhận xét {#top-ix-s5-n3-rem-1 .statement}

Có những không gian Baire không thuộc một trong hai loại này, đặc biệt là những không gian Baire không vừa mêtric hóa được vừa không địa phương compact (Bài tập 16); cũng có những không gian Baire mêtric hóa được nhưng không có cấu trúc không gian mêtric đầy đủ nào tương thích với tôpô của chúng (Bài tập 14).

### 4. HÀM BÁN LIÊN TỤC TRÊN MỘT KHÔNG GIAN BAIRE

#### Định lý 2 {#top-ix-s5-thm-2 .statement}

Cho $X$ là một không gian Baire và $(f_\alpha)$ là một họ các hàm thực nửa liên tục dưới trên $X$ sao cho, tại mọi điểm $x$ của $X$, bao trên $\sup_\alpha f_\alpha(x)$ là hữu hạn. Khi đó mọi tập hợp mở không rỗng trong $X$ chứa một tập hợp mở không rỗng trên đó họ $(f_\alpha)$ bị chặn trên đều.

Định lý này cũng có thể được phát biểu dưới dạng: tập hợp các điểm mà trong một lân cận của chúng họ $(f_\alpha)$ bị chặn trên đều là một tập hợp mở trù mật.

Cho $f = \sup_\alpha f_\alpha$ là bao trên của họ $(f_\alpha)$. Hàm $f$ là nửa liên tục dưới (Chương IV, § 6, no. 2, Định lý 4) và hữu hạn tại mọi điểm của $X$. Vì vậy chỉ cần thực hiện chứng minh trong trường hợp họ $(f_\alpha)$ gồm một hàm duy nhất $f$. Gọi $A_n$ là tập hợp các điểm $x \in X$ sao cho $f(x) \leq n$; $A_n$ là đóng (Chương IV, § 6, no. 2, Mệnh đề 1), và các giả thiết suy ra rằng $X$ là hợp của các tập hợp $A_n$; do đó ít nhất một trong các $A_n$ có một điểm trong, và vì vậy tồn tại một tập hợp mở không rỗng trên đó $f$ bị chặn trên (bởi một số nguyên $n$). Nếu áp dụng kết quả này cho mọi tập hợp con mở không rỗng của $X$ (không gian con này cũng là một không gian Baire theo Mệnh đề 3 của no. 3), ta có định lý.

Trong các áp dụng của định lý này, nói chung các $f_\alpha$ là liên tục trên $X$.

#### Nhận xét {#top-ix-s5-n4-rem-1 .statement}

Định lý có thể sai nếu ta không giả sử rằng $X$ là một không gian Baire. Ví dụ nếu, với mỗi số hữu tỉ $p/q$ ($p, q$ là các số nguyên nguyên tố cùng nhau, $q > 0$) ta đặt $f(p/q) = q$, ta có một hàm $f$ nửa liên tục dưới trên đường thẳng hữu tỉ $Q$ hữu hạn tại mỗi điểm (xem Chương IV, § 6, no. 2); nhưng không có tập hợp mở không rỗng nào trong $Q$ trên đó $f$ bị chặn trên.

### Bài tập {#top-ix-s5-exercises}

Xem các [bài tập cho § 5](exercises/s5/).
