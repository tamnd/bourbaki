---
book: top
book_title: General Topology
chapter: V
chapter_title: One-parameter groups
section: 1
section_title: Subgroups and quotient groups of R
lang: vi
source: top-v-x
pdf_pages: 0013-0017, 0030-0031
extraction: ocr
subsections:
    - "no": 1
      title: CLOSED SUBGROUPS OF $\mathbf{R}$
      page: 0
      pdf_page: 13
    - "no": 2
      title: QUOTIENT GROUPS OF $\mathbf{R}$
      page: 0
      pdf_page: 13
    - "no": 3
      title: CONTINUOUS HOMOMORPHISMS OF $\mathbf{R}$ INTO ITSELF
      page: 0
      pdf_page: 15
    - "no": 4
      title: LOCAL DEFINITION OF A CONTINUOUS HOMOMORPHISM OF $\mathbf{R}$ INTO A TOPOLOGICAL GROUP
      page: 0
      pdf_page: 15
statements: 13
exercises: 3
content_sha256: d02a922a7fc9c83f08e83ff795e24320fd1c8f84f9c0890b3bfb9ecedc7e9d1e
translated_from: content/en/top/V/01_s1_subgroups_and_quotient_groups_of_r.md
source_content_sha256: c002969ca857c3fbe860d348d27582dd457331b655514d3b9dbdafc9ddc370e0
translation_model: gpt-5.4-mini
translation_run: translate-vi-4f815443
glossary_version: 34
glossary_terms_sha256: f4b08022040eab6fd14d80fcbeef5a94465a97749bc8dd5eb02a41d5098ede30
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 1. NHÓM CON VÀ NHÓM THƯƠNG CỦA $\mathbf{R}$

### 1. NHÓM CON ĐÓNG CỦA $\mathbf{R}$

#### Mệnh đề 1 {#top-v-s1-prop-1 .statement}

*Mọi nhóm con đóng của nhóm cộng $\mathbf{R}$, khác $\mathbf{R}$ và $\{0\}$, đều là một nhóm rời rạc có dạng $a.\mathbf{Z}$, với $a > 0$* (nói cách khác, nó gồm các bội nguyên của $a$).

Ta bắt đầu bằng cách chứng minh rằng mọi nhóm con không rời rạc của $\mathbf{R}$ đều trù mật trong $\mathbf{R}$. Nếu một nhóm con $G$ của $\mathbf{R}$ không rời rạc, thì với mọi $\varepsilon > 0$ đều có một điểm $x \neq 0$ trong $G$ thuộc khoảng $[-\varepsilon, +\varepsilon]$; vì mọi bội nguyên của $x$ đều thuộc $G$, nên mọi khoảng có độ dài $> \varepsilon$ đều chứa một phần tử của $G$, và do đó $G$ trù mật trong $\mathbf{R}$.

Vì vậy, mọi nhóm con đóng của $\mathbf{R}$, khác chính $\mathbf{R}$, đều rời rạc. Còn lại chứng minh rằng mọi nhóm con rời rạc $G$ của $\mathbf{R}$, khác $\{0\}$, đều có dạng $a.\mathbf{Z}$, với $a > 0$. Bây giờ quan hệ $-G = G$ cho thấy tập hợp $H$ gồm các phần tử $> 0$ trong $G$ là không rỗng; nếu $b \in H$, giao của khoảng $[0, b]$ và $G$ là *compact và rời rạc*, nên là *hữu hạn*. Hãy để $a$ là phần tử nhỏ nhất của $H$ chứa trong $[0, b]$, và với mọi $x \in G$ đặt $m = [x/a]$, phần nguyên của $x/a$; khi đó ta có $x - ma \in G$ và $0 \leq x - ma < a$. Theo định nghĩa của $a$ suy ra $x - ma = 0$ và do đó $G = a.\mathbf{Z}$.

### 2. NHÓM THƯƠNG CỦA $\mathbf{R}$

Mọi nhóm thương *Hausdorff* của $\mathbf{R}$ đều có dạng $\mathbf{R}/H$, trong đó $H$ là một nhóm con *đóng* của $\mathbf{R}$ (Chương III, § 2, no. 6, Mệnh đề 18); do đó, theo Mệnh đề 1 của no. 1:

#### Mệnh đề 2 {#top-v-s1-prop-2 .statement}

*Các nhóm thương Hausdorff của* $\mathbf{R}$, *khác* $\{0\}$, *là các nhóm* $\mathbf{R}/a\mathbf{Z}$ ($a \geqslant 0$).
*Nếu* $a$ *và* $b$ *đều* $> 0$, *tự đẳng cấu* $x \to b/a\,x$ *của* $\mathbf{R}$ *biến* $a\mathbf{Z}$ *thành* $b\mathbf{Z}$, *và do đó* (Chương III, § 2, no. 8, Nhận xét 3) *các nhóm thương* $\mathbf{R}/a\mathbf{Z}$ *và* $\mathbf{R}/b\mathbf{Z}$ *đẳng cấu; nói cách khác*:

#### Mệnh đề 3 {#top-v-s1-prop-3 .statement}

*Mọi nhóm thương Hausdorff của* $\mathbf{R}$, *khác* $\mathbf{R}$ *và* $\{0\}$, *đều đẳng cấu với nhóm* $\mathbf{R}/\mathbf{Z}$.

#### Định nghĩa 1 {#top-v-s1-def-1 .statement}

*Nhóm tôpô* $\mathbf{R}/a\mathbf{Z}$ ($a > 0$) *được gọi là nhóm cộng của các số thực modulo* $a$. *Nhóm tôpô* $\mathbf{R}/\mathbf{Z}$ *được ký hiệu bởi* $\mathbf{T}$. *Xét như một không gian tôpô,* $\mathbf{T}$ *được gọi là xuyến một chiều* (nói một cách lạm dụng ngôn ngữ, nhóm tôpô $\mathbf{T}$ cũng được gọi là xuyến một chiều).

#### Nhận xét 1 {#top-v-s1-n2-rem-1 .statement}

*Quan hệ* $x \equiv y \pmod{a\mathbf{Z}}$ *thường được viết* $x \equiv y \pmod{a}$, *hoặc đơn giản là* $x \equiv y (a)$, *và được đọc là* "x và y đồng dư modulo a"; *nó có nghĩa là* $x - y$ *là một bội nguyên của* $a$. *Khi* $a$ *là một số nguyên, quan hệ cảm sinh trên* $\mathbf{Z}$ *bởi quan hệ này chính xác là đồng dư modulo* $a$; *điều đó biện minh cho ký hiệu này*.

#### Nhận xét 2 {#top-v-s1-n2-rem-2 .statement}

*Như ta sẽ thấy trong Chương VI, § 2, no. 4, không gian tôpô* $\mathbf{T}$ *đồng phôi với đường tròn* $x^2 + y^2 = 1$ *trong mặt phẳng số thực* $\mathbf{R}^2$; *không gian tích* $\mathbf{T}^2$ *đồng phôi với một xuyến tròn xoay trong* $\mathbf{R}^3$ *(Chương VII, § 1, Bài tập 15)*. *Đó là nguồn gốc của tên gọi* "xuyến một chiều" *dành cho* $\mathbf{T}$ *(trong Chương VII, § 1, ta sẽ gọi* $\mathbf{T}^n$ *là xuyến n chiều)*.

#### Mệnh đề 4 {#top-v-s1-prop-4 .statement}

*Xuyến* $\mathbf{T}$ *đồng phôi với không gian thương của bất kỳ đoạn đóng nào của* $\mathbf{R}$ *có dạng* $[a, a+1]$ *thu được bằng cách đồng nhất các đầu mút của đoạn này; nó compact, liên thông và liên thông địa phương*.

Mọi $x \in \mathbf{R}$ *đều đồng dư* $(\bmod\,1)$ *với một số trong khoảng* $[a, a+1]$, *cụ thể là với* $x - [x-a]$; *suy ra* $\mathbf{T}$ *là ảnh của khoảng này qua ánh xạ chính tắc* $\varphi$ *từ* $\mathbf{R}$ *lên* $\mathbf{R}/\mathbf{Z}$, *và do đó compact và liên thông* (Chương I, § 9, no. 4, Định lý 2, và § 11, no. 2, Mệnh đề 4). *Mặt khác, hai phần tử phân biệt của khoảng* $[a, a+1]$ *chỉ đồng dư* $(\bmod\,1)$ *nếu chúng là các đầu mút của khoảng; từ tính compact của* $\mathbf{T}$ *suy ra rằng* $\mathbf{T}$ *đồng phôi với không gian thương của* $[a, a+1]$ *thu được bằng cách đồng nhất các đầu mút* (Chương I, § 9, no. 4, Định lý 2, Hệ quả 4, và § 10, no. 4, Mệnh đề 8). *Cuối cùng,* $\mathbf{Z}$ *là một nhóm con rời rạc của* $\mathbf{R}$, $\mathbf{T} = \mathbf{R}/\mathbf{Z}$ *là* đẳng cấu địa phương *với* $\mathbf{R}$ *(Chương III, § 2, no. 6, Mệnh đề 19)* *và do đó đặc biệt là liên thông địa phương* (sự kiện cuối cùng này cũng là một hệ quả của Chương I, § 11, no. 6, Mệnh đề 12).

#### Nhận xét {#top-v-s1-n2-rem-3 .statement}

Chú ý rằng ánh xạ chính tắc $\varphi$ của $\mathbf{R}$ lên $T = \mathbf{R}/\mathbf{Z}$, khi được hạn chế trên khoảng nửa mở $[a, a+1[$, là một ánh xạ song ánh liên tục của khoảng này lên $T$; ánh xạ nghịch đảo liên tục tại mọi điểm của $T$ khác với $\varphi(a)$, nhưng không liên tục tại $\varphi(a)$. Đôi khi ta đồng nhất không gian $T$ với khoảng $[a, a+1[$, được trang bị tôpô là ảnh ngược qua $\varphi$ của tôpô của $T$ (Chương I, § 1, no. 3); dĩ nhiên tôpô này không phải là tôpô cảm sinh trên $[a, a+1[$ bởi tôpô của $\mathbf{R}$.

### 3. CÁC ĐỒNG CẤU LIÊN TỤC TỪ $\mathbf{R}$ VÀO CHÍNH NÓ

#### Mệnh đề 5 {#top-v-s1-prop-5 .statement}

Mọi đồng cấu liên tục $f$ của nhóm tôpô $\mathbf{R}$ vào chính nó đều có dạng $x \to ax$, với $a \in \mathbf{R}$; nó là một tự đẳng cấu của $\mathbf{R}$ nếu $a \neq 0$.

Với mọi $x \in \mathbf{R}$ và mọi số nguyên $p \in \mathbf{Z}$, ta có $f(px) = pf(x)$; thay thế $x$ bởi $(1/p)x$, suy ra rằng

$$
f\left(\frac{1}{p}x\right) = \frac{1}{p} f(x) \quad \text{nếu } p \neq 0;
$$

do đó, với mọi số nguyên $p$ và $q \neq 0$, ta có

$$
f\left(\frac{p}{q}x\right) = \frac{p}{q} f(x).
$$

Nói cách khác, $f(rx) = rf(x)$ với mọi số hữu tỉ $r$. Nếu bây giờ $t$ là một số thực tùy ý, do tính liên tục của $f$ ta có

$$
f(tx) = \lim_{r \to t, r \in \mathbf{Q}} f(rx) = \lim_{r \to t, r \in \mathbf{Q}} rf(x) = \left( \lim_{r \to t, r \in \mathbf{Q}} r \right) f(x) = tf(x).
$$

Đặc biệt, nếu $a = f(1)$ thì ta có $f(t) = at$, và mệnh đề được chứng minh.

Vì thế nhóm các tự đẳng cấu của nhóm tôpô $\mathbf{R}$ đẳng cấu với nhóm nhân $\mathbf{R}^*$ của các số thực khác không.

#### Hệ quả {#top-v-s1-n3-cor-1 .statement}

Cho $G$ là một nhóm tôpô đẳng cấu với $\mathbf{R}$. Với mỗi $a \in G$ có đúng một đồng cấu liên tục $f_a$ của $\mathbf{R}$ vào $G$ sao cho $f_a(1) = a$, và đồng cấu này là một đẳng cấu của $\mathbf{R}$ lên $G$ nếu $a$ không phải là phần tử không của $G$.

### 4. ĐỊNH NGHĨA ĐỊA PHƯƠNG CỦA MỘT ĐỒNG CẤU LIÊN TỤC TỪ $\mathbf{R}$ VÀO MỘT NHÓM TÔPÔ

#### Mệnh đề 6 {#top-v-s1-prop-6 .statement}

Nếu ta được cho một nhóm $G$ và một tập con $A$ của $G$ sinh ra $G$, thì hiển nhiên hai đồng cấu $f, g$ của $G$ vào một nhóm $G'$ trùng nhau nếu chúng nhận cùng một giá trị tại mọi điểm của $A$. Nhưng các giá trị trên $A$ của một đồng cấu $f$ của $G$ vào $G'$ nói chung không thể được lấy tùy ý; nếu $G$ và $G'$ được viết theo phép nhân, thì các giá trị ấy phải thỏa mãn điều kiện $f(xy) = f(x)f(y)$ với mỗi cặp $(x, y)$ sao cho $x \in A, y \in A$ và $xy \in A$. Hơn nữa, điều kiện cần này nói chung không đủ.

Đặc biệt, một *đẳng cấu địa phương* của một nhóm tôpô $G$ với một nhóm tôpô $G'$ không phải lúc nào cũng có thể được mở rộng thành một đồng cấu (liên tục hay không) của $G$ vào $G'$. Chẳng hạn, một đẳng cấu địa phương $f$ của $T$ với $\mathbf{R}$ không thể được mở rộng thành một đồng cấu của $T$ vào $\mathbf{R}$; vì nếu $f$ được xác định trên một lân cận $V$ của $o$, thì tồn tại một số nguyên $p > 0$ sao cho lớp $x \pmod{\mathbf{Z}}$ của $\frac{1}{p}$ thuộc $V$; vì $x$ có cấp $p$ trong $T$, ảnh của nó qua mọi đồng cấu của $T$ vào $\mathbf{R}$ nhất thiết là $o$ và do đó phân biệt với $f(x)$ theo giả thiết.

Về phương diện này, nhóm tôpô $\mathbf{R}$ có tính chất sau:

*Cho $I$ là một khoảng của $\mathbf{R}$ chứa $o$ và ít nhất một điểm khác; cho $f$ là một ánh xạ liên tục của $I$ vào một nhóm tôpô $G$ (viết theo phép nhân), sao cho $f(x+y) = f(x)f(y)$ với mỗi cặp điểm $(x, y)$ sao cho $x \in I, y \in I$ và $x + y \in I$. Khi đó tồn tại duy nhất một đồng cấu liên tục của $\mathbf{R}$ vào $G$ mở rộng $f$.*.

Tính duy nhất của phép mở rộng (nếu nó tồn tại) suy ra từ các nhận xét trên, vì $I$ sinh ra nhóm $\mathbf{R}$. Chúng ta phải chứng minh sự tồn tại của một phép mở rộng như vậy.

==========

Nếu $n$ là một số nguyên $> 0$ và nếu $x \in I$ và $nx \in I$, ta có $f(nx) = (f(x))^n$, theo quy nạp trên $n$ (vì $mx \in I$ với mọi số nguyên $m$ sao cho $1 \leq m \leq n$). Đặt $J = \bigcup_{n \in \mathbf{N}} nI$; $J$ hoặc là toàn bộ đường thẳng $\mathbf{R}$, hoặc là một trong các khoảng $[0, +\infty[$ hay $[-\infty, 0]$, tùy theo việc $o$ có là một điểm trong của $I$ hay không. Nếu $x \in J$ thì ta có $x/n \in I$ bất cứ khi nào $n$ là một số nguyên đủ lớn $> 0$. Cho $x \in J$, và cho $m, n$ là hai số nguyên $> 0$ sao cho $x/n \in I$ và $x/m \in I$; khi đó $x/mn \in I$, và do đó

$$
f\left( \frac{x}{m} \right) = \left( f\left( \frac{x}{mn} \right) \right)^n \quad \text{và} \quad f\left( \frac{x}{n} \right) = \left( f\left( \frac{x}{mn} \right) \right)^m;
$$

nói cách khác, phần tử $(f(x/n))^n$ của $G$ là như nhau đối với mọi số nguyên $n > 0$ sao cho $x/n \in I$. Ký hiệu phần tử này là $f_1(x)$; $f_1$ là một ánh xạ của $J$ vào $G$, trùng với $f$ trên $I$ và do đó liên tục tại điểm $o$ (xét theo $J$). Cho $x, y$ là hai phần tử của J và cho n là một số nguyên đủ lớn > 0 sao cho $\frac{x}{n} \in I, \frac{y}{n} \in I$ và $\frac{x+y}{n} \in I$; khi đó

$$
f\left( \frac{x+y}{n} \right) = f\left( \frac{x}{n} \right) f\left( \frac{y}{n} \right) = f\left( \frac{y}{n} \right) f\left( \frac{x}{n} \right),
$$

which shows that $f\left( \frac{x}{n} \right)$ and $f\left( \frac{y}{n} \right)$ commute; theo định nghĩa của $f_1$, do đó ta có $f_1(x+y) = f_1(x) f_1(y)$. Nếu $J = \mathbf{R}$, thì chứng minh đã hoàn tất; nếu không, giả sử $J = [0, +\infty[$, và với mỗi $x < 0$ đặt $f_1(x) = (f_1(-x))^{-1}$. Khi đó quan hệ $f_1(x+y) = f_1(x) f_1(y)$ vẫn đúng với mọi $x \in \mathbf{R}$ và mọi $y \in \mathbf{R}$. Điều này hiển nhiên nếu $x < 0$ và $y < 0$; nếu $x \geqslant 0$, $y < 0$ và $x + y \geqslant 0$ thì điều đó suy ra từ $f_1(x) = f_1(x+y) f_1(-y)$; chứng minh tương tự nếu $x \geqslant 0, y < 0$ và $x + y < 0$, vì khi đó ta có

$$
f_1(-y) = f_1(-x-y) f_1(x);
$$

chứng minh tương tự cho $x < 0$ và $y \geqslant 0$. Do đó ta thấy rằng $f_1$ là một đồng cấu của $\mathbf{R}$ vào G, suy ra $f_1(0) = e$, phần tử đơn vị của G; và vì $f_1$ liên tục đối với J, nên nó có giới hạn bên phải tại 0, bằng $e$; vì $f_1(-x) = (f_1(x))^{-1}$, nên $f_1$ cũng có giới hạn tại 0 ở bên trái, bằng $e$; vậy $f_1$ liên tục tại 0, và chứng minh đã hoàn tất.

#### Hệ quả {#top-v-s1-n4-cor-1 .statement}

*Cho f là một đẳng cấu địa phương của $\mathbf{R}$ với một nhóm tôpô G. Khi đó tồn tại duy nhất một cấu xạ ngặt của $\mathbf{R}$ lên một nhóm con mở của G trùng với f tại mọi điểm của một lân cận nào đó của 0.*

Gọi $\overline{f}$ là đồng cấu liên tục của $\mathbf{R}$ vào G trùng với $f$ tại mọi điểm của một khoảng mở I, chứa 0 và được chứa trong tập hợp trên đó $f$ được định nghĩa; theo giả thiết $\overline{f}(\mathbf{R})$ chứa một lân cận của phần tử đơn vị của G, do đó (Chương III, § 2, no. 1, Hệ quả của Mệnh đề 4) là một nhóm con mở của G; và $\overline{f}$ là một cấu xạ ngặt của $\mathbf{R}$ lên $\overline{f}(\mathbf{R})$, theo Chương III, § 2, no. 8, Mệnh đề 24.

#### Mệnh đề 7 {#top-v-s1-prop-7 .statement}

*Mọi nhóm liên thông G mà đẳng cấu địa phương với $\mathbf{R}$ thì đẳng cấu với hoặc $\mathbf{R}$ hoặc $\mathbf{T}$.*

Thật vậy, một đẳng cấu địa phương của $\mathbf{R}$ với G kéo dài thành một cấu xạ ngặt của $\mathbf{R}$ lên một nhóm con mở của G (Hệ quả của Mệnh đề 6), do đó lên chính G vì G liên thông. Suy ra G đẳng cấu với một nhóm thương của $\mathbf{R}$; vì G là Hausdorff và không chỉ gồm riêng phần tử đơn vị (vì nó đẳng cấu địa phương với $\mathbf{R}$), nên theo Mệnh đề 3 của no. 2, G đẳng cấu với hoặc $\mathbf{R}$ hoặc $\mathbf{T}$.

### Bài tập {#top-v-s1-exercises}

Xem [các bài tập cho § 1](exercises/s1/).
