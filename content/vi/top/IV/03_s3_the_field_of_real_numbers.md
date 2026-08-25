---
book: top
book_title: General Topology
chapter: IV
chapter_title: Real Numbers
section: 3
section_title: The field of real numbers
lang: vi
source: top-i-iv
pdf_pages: 0345-0348, 0393-0394
extraction: ocr
subsections:
    - "no": 1
      title: MULTIPLICATION IN $\mathbf{R}$
      page: 0
      pdf_page: 345
    - "no": 2
      title: THE MULTIPLICATIVE GROUP $\mathbf{R}^*$
      page: 0
      pdf_page: 346
    - "no": 3
      title: '*n*TH ROOTS'
      page: 0
      pdf_page: 347
statements: 2
exercises: 3
content_sha256: 7e9fd20a5f07701f8b8136c006c7d342796e0cab1dd5c9335841bda2be273887
translated_from: content/en/top/IV/03_s3_the_field_of_real_numbers.md
source_content_sha256: 195704c1333f5f2d91a6ce305c05eaeb27c6a686881d525615a04e249dba1f90
translation_model: gpt-5.4
translation_run: translate-vi-cf7e820d
glossary_version: 34
glossary_terms_sha256: 303088e87c0945157be32820873be67d886c68af0d566869c0427a99534af5b0
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 3. TRƯỜNG SỐ THỰC

### 1. PHÉP NHÂN TRONG $\mathbf{R}$

Tôpô của đường thẳng hữu tỉ $\mathbf{Q}$ không những tương thích với cấu trúc *nhóm cộng*, mà còn với cấu trúc *trường* của $\mathbf{Q}$. Thật vậy, hàm $xy$ liên tục tại $(0, 0) \in \mathbf{Q} \times \mathbf{Q}$, vì với mỗi số nguyên $n > 0$, các quan hệ $|x| \leq 1/n$ và $|y| \leq 1/n$ cùng nhau kéo theo $|xy| \leq 1/n^2 \leq 1/n$; mặt khác, nếu $a$ là một số hữu tỉ khác không bất kỳ, thì hàm $ax$ liên tục tại $x = 0$, vì với mỗi số nguyên $n > 0$, quan hệ $|x| \leq 1/|n|a|$ kéo theo $|ax| \leq 1/n$. Điều đó cho thấy $xy$ liên tục tại mọi điểm của $\mathbf{Q} \times \mathbf{Q}$ (Chương III, § 6, no. 3).

Để chứng minh rằng $1/x$ liên tục trên $\mathbf{Q}^*$, ta sẽ thiết lập chính xác hơn rằng $1/x$ là *liên tục đều* (đối với cấu trúc cộng tính) trong phần bù của mọi lân cận V của 0. Cụ thể, ta có $$
\left| \frac{1}{x} - \frac{1}{y} \right| = \frac{|x-y|}{xy}
$$; tồn tại một số nguyên $m > 0$ sao cho $|x| \geq 1/m$ với mọi $x \in \mathcal{G}_V$; nếu $x$ và $y$ là hai điểm bất kỳ của $\mathcal{G}_V$ sao cho $|x-y| \leq 1/m^2 n$, thì khi đó ta sẽ có $$
\left| \frac{1}{x} - \frac{1}{y} \right| \leq \frac{1}{n}.
$$

#### Mệnh đề 1 {#top-iv-s3-prop-1 .statement}

*Các hàm xy và $1/x$, được định nghĩa tương ứng trên $\mathbf{Q} \times \mathbf{Q}$ và $\mathbf{Q}^*$, có thể được mở rộng bằng tính liên tục lên $\mathbf{R} \times \mathbf{R}$ và $\mathbf{R}^*$ tương ứng, và xác định một cấu trúc trường trên $\mathbf{R}$. Được trang bị cấu trúc này, $\mathbf{R}$ được gọi là trường số thực.*

Dĩ nhiên, mọi tính chất của các trường tôpô đã được thiết lập trong § 6 của Chương III đều áp dụng được; đặc biệt, mọi *hàm hữu tỉ* của $n$ biến thực, với các hệ số thực, đều *liên tục* tại mọi điểm của $\mathbf{R}^n$ mà tại đó mẫu số của nó không triệt tiêu.

### 2. NHÓM NHÂN $\mathbf{R}^*$

Ta biết từ Chương III, § 6, no. 7, rằng tôpô cảm sinh trên $\mathbf{R}^*$ bởi tôpô của đường thẳng thực là *tương thích* với cấu trúc nhóm nhân của $\mathbf{R}^*$; vì $\mathbf{R}^*$ là một tập con *mở* của không gian compact địa phương $\mathbf{R}$, suy ra $\mathbf{R}^*$ là một nhóm tôpô *compact địa phương* (Chương I, § 9, no. 7, Mệnh đề 13) và do đó *đầy đủ* (Chương III, § 3, no. 3, Hệ quả 1 của Mệnh đề 4; điều này cũng suy ra từ Chương III, § 6, no. 8, Mệnh đề 8); dĩ nhiên, tính chất sau này liên quan đến cấu trúc đều *nhân* trên $\mathbf{R}^*$ chứ không phải cấu trúc đều cảm sinh trên $\mathbf{R}^*$ bởi cấu trúc đều cộng tính của $\mathbf{R}$.

Hàm $xy$ ánh xạ tập hợp $\mathbf{Q}_+ \times \mathbf{Q}_+$ vào $\mathbf{Q}_+$, và do đó nó ánh xạ $\mathbf{R}_+ \times \mathbf{R}_+$ vào $\mathbf{R}_+$ (Chương I, § 2, no. 1, Định lý 1); nói cách khác, *tích của hai số thực $\geqslant 0$ là $\geqslant 0$*. Khi đó các công thức $(-x)y = -xy$ và $(-x)(-y) = xy$ cho thấy rằng tích của một số $\geqslant 0$ và một số $\leqslant 0$ là $\leqslant 0$, và rằng tích của hai số $\leqslant 0$ là $\geqslant 0$; từ đó suy ra rằng

$$(1)$$
$$|xy| = |x| \cdot |y|$$

(điều này cũng có thể thu được bằng cách mở rộng quan hệ tương ứng trên $\mathbf{Q} \times \mathbf{Q}$).

Nếu $x > 0$ và $y > 0$ thì ta có $xy \neq 0$, và do đó $xy > 0$; tương tự, nếu $x < 0$ và $y > 0$ thì $xy < 0$; và nếu $x < 0$ và $y < 0$ thì $xy > 0$. Đặc biệt, nếu $x \neq 0$ thì ta có $x^2 > 0$, vì thế một *tổng các bình phương* của các số thực không thể bằng không trừ khi mỗi số đó đều bằng không.

Nếu $x > 0$ và $y \leqslant z$ (tương ứng $y < z$) thì ta có $xy \leqslant xz$ (tương ứng $xy < xz$), nói cách khác, *một phép vị tự có tỉ số* $> 0$ *bảo toàn thứ tự trên* $\mathbf{R}$. Vì $(-x)y = -xy$, một phép vị tự có tỉ số $< 0$ biến thứ tự trên $\mathbf{R}$ thành thứ tự đối.

Nếu $x > 0$ thì ta có $1/x > 0$, vì $x.(1/x) = 1 > 0$. Nếu $0 < x < y$ thì ta có $xy > 0$, do đó $x.(1/xy) < y.(1/xy)$, tức là $1/y < 1/x$. Suy ra ánh xạ $x \to 1/x$ của tập hợp $\mathbf{R}_+^*$ các số thực $> 0$ lên chính nó là giảm nghiêm ngặt.

Ta cũng thấy theo cùng cách rằng hàm $1/x$ giảm nghiêm ngặt trên ]$\leftarrow, 0[$, và do đó hàm $\frac{1}{x-a}$ giảm nghiêm ngặt trên mỗi khoảng ]$\leftarrow, a[$ và $]a, \to[$.

Từ những điều đi trước suy ra rằng $\mathbf{R}_+^*$ là một nhóm con của nhóm nhân $\mathbf{R}^*$; hơn nữa, quan hệ thứ tự $x \leq y$ tương thích với cấu trúc nhóm nhân của $\mathbf{R}_+^*$; nói cách khác, $\mathbf{R}_+^*$ là một nhóm có thứ tự toàn phần.

Sự kiện rằng tích của hai số thực $\geq 0$ lại là $\geq 0$ có thể được diễn đạt bằng cách nói rằng $\mathbf{R}$ là một trường có thứ tự: mọi tính chất trên đây đều chung cho mọi trường có thứ tự.

#### Mệnh đề 2 {#top-iv-s3-prop-2 .statement}

*Nhóm nhân $\mathbf{R}^*$ của các số thực $\neq 0$ là một nhóm tôpô đẳng cấu với tích của các nhóm con $\mathbf{R}_+^*$ và $\mathbf{U}_0$, trong đó*

$$
\mathbf{U}_0 = \{ -1, +1 \}.
$$

Với mỗi $x \neq 0$ ký hiệu $\operatorname{sgn} x$ chỉ $\frac{x}{|x|}$ (*dấu của* $x$). Hàm $\operatorname{sgn}$ là một đồng cấu từ $\mathbf{R}^*$ lên $\mathbf{U}_0$. Ta có $x = |x|\operatorname{sgn} x$, và phân tích này của $x$ thành tích của một phần tử của $\mathbf{R}_+^*$ và một phần tử của $\mathbf{U}_0$ là duy nhất; do đó cấu trúc nhóm của $\mathbf{R}^*$ là tích của các cấu trúc nhóm của $\mathbf{R}_+^*$ và $\mathbf{U}_0$. Mặt khác, ánh xạ $x \to |x|$ là liên tục, và ánh xạ $x \to \operatorname{sgn} x = \frac{x}{|x|}$ cũng vậy, vì $x \neq 0$. Do đó có kết quả.
Ta mở rộng hàm $\operatorname{sgn}$ ra toàn bộ $\mathbf{R}$ bằng cách đặt $\operatorname{sgn} 0 = 0$.

Ta sẽ thấy trong Chương V (\S 4, no. 1, Định lý 1) rằng nhóm tôpô $\mathbf{R}_+^*$ *đẳng cấu* với nhóm *cộng tính* $\mathbf{R}$; điều này sẽ hoàn tất việc xác định cấu trúc của nhóm tôpô $\mathbf{R}_*$.

### 3. CĂN BẬC *n*

Cho $n$ là một số nguyên bất kỳ $> 0$. Từ quan hệ $0 < x < y$ ta suy ra, bằng quy nạp theo $n$, rằng $0 < x^n < y^n$. Nói cách khác, hàm $x \to x^n$ là *tăng ngặt* với $x \geq 0$; nó rõ ràng liên tục tại mọi điểm và vì thế (\S 2, no. 6, Định lý 5) là một đồng phôi từ $\mathbf{R}_+$ lên một khoảng $I$. Mặt khác, vì $x \geqslant 1$ kéo theo $x^{n-1} \geqslant 1$ và do đó $x^n \geqslant x$, nên suy ra $I$ không bị chặn và vì thế $I = \mathbf{R}_+$. Giá trị, với $x \geqslant 0$, của ánh xạ nghịch đảo của ánh xạ $x \to x^n$ được ký hiệu bởi $x^{1/n}$ hoặc $\sqrt[n]{x}$ và được gọi là $x$ lũy thừa $1/n$ hoặc căn bậc n của $x$ (với $n = 2, 3$ ta nói căn bậc hai, căn bậc ba; với $n = 2$ ta viết $\sqrt{x}$ thay cho $\sqrt[2]{x}$). Vì vậy, số dương $x^{1/n}$ được định nghĩa là nghiệm dương duy nhất của phương trình

$$
y^n = x \quad (x \geqslant 0).
$$

Đặc biệt ta thấy rằng tồn tại một số thực $x$ sao cho $x^2 = 2$, trong khi không có số hữu tỉ nào có tính chất này; như vậy ta thu lại sự kiện rằng đường thẳng hữu tỉ $\mathbf{Q}$ không phải là một không gian đầy đủ.

Ánh xạ $x \to x^{1/n}$ của $\mathbf{R}_+$ lên chính nó là tăng ngặt và liên tục. Theo (2) ta có $0^{1/n} = 0, 1^{1/n} = 1$, và còn có

$$
(xy)^{1/n} = x^{1/n} y^{1/n};
$$

do đó $x \to x^{1/n}$ là một tự đẳng cấu của nhóm tôpô $\mathbf{R}_+^*$.

Trong Chương V, \S 4, no. 1, ta sẽ tổng quát hóa kết quả này bằng cách tìm tất cả các tự đẳng cấu của nhóm nhân $\mathbf{R}_+^*$.

### Bài tập {#top-iv-s3-exercises}

Xem [bài tập của § 3](exercises/s3/).
