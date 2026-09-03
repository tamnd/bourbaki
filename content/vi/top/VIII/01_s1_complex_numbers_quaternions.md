---
book: top
book_title: General Topology
chapter: VIII
chapter_title: Complex numbers
section: 1
section_title: Complex numbers, quaternions
lang: vi
source: top-v-x
pdf_pages: 0106-0111, 0129-0131
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF COMPLEX NUMBERS
      page: 0
      pdf_page: 106
    - "no": 2
      title: THE TOPOLOGY OF $\mathbf{C}$
      page: 0
      pdf_page: 108
    - "no": 3
      title: THE MULTIPLICATIVE GROUP $\mathbf{C}^*$
      page: 0
      pdf_page: 109
    - "no": 4
      title: THE DIVISION RING OF QUATERNIONS
      page: 0
      pdf_page: 110
statements: 8
exercises: 5
content_sha256: 3c83f91cdbe882c51cf76b05968072c85ca007ec4a3e8cb074d20c21e1a8c0b2
translated_from: content/en/top/VIII/01_s1_complex_numbers_quaternions.md
source_content_sha256: 553535497dc7d86b3ebe016a77f3f220a1985737fb41450839e4f7c2c5d04e44
translation_model: gpt-5-6-mini
translation_run: translate-vi-c831aeb5
glossary_version: 34
glossary_terms_sha256: 04ce0f1d2e851794faa9b8323bc05703abb3a4dc019f1ce9dc0e6c121c0598a2
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 1. SỐ PHỨC, QUATERNION

### 1. ĐỊNH NGHĨA CÁC SỐ PHỨC

Đa thức $X^2 + 1$ không có nghiệm trong $\mathbf{R}$, vì $x^2 + 1 \geq 1$ với mọi $x \in \mathbf{R}$; do đó nó là bất khả quy trên $\mathbf{R}$. [Đây là một trường hợp riêng của kết quả tương tự áp dụng cho mọi trường có thứ tự.]

#### Định nghĩa 1 {#top-viii-s1-def-1 .statement}

*Trường* $\mathbf{R}[X]/(X^2 + 1)$ *được gọi là trường các số phức và được ký hiệu là* $\mathbf{C}$. *Ảnh chính tắc của* $X$ *trong* $\mathbf{C}$ *được ký hiệu là* $i$, *do đó* $\mathbf{C}$ *thu được từ trường* $\mathbf{R}$ *bằng phép nối đại số nghiệm* $i$ *của đa thức* $X^2 + 1$. *Các phần tử của* $\mathbf{C}$ *được gọi là các số phức*.

Về phương diện đại số, tầm quan trọng của trường $\mathbf{C}$ là do định lý cơ bản sau đây:

#### Định lý 1 {#top-viii-s1-thm-1 .statement}

(d'Alembert-Gauss). *Trường* $\mathbf{C}$ *các số phức là đóng đại số*.

Để chứng minh, chỉ cần chứng minh rằng (i) mọi phần tử $\geq 0$ trong $\mathbf{R}$ đều có một *căn bậc hai*, và (ii) mọi đa thức có *bậc lẻ* với các hệ số trong $\mathbf{R}$ đều có *ít nhất một nghiệm* trong $\mathbf{R}$. Mệnh đề thứ nhất trong các mệnh đề này đã được chứng minh trong Chương IV, § 3, no. 3. Còn đối với mệnh đề thứ hai, nếu $f(X) = a_0 X^n + a_1 X^{n-1} + \cdots + a_n$ là một đa thức có bậc lẻ $n$ ($a_0 \neq 0$) với các hệ số thực, ta có thể viết $f(x) = a_0 x^n g(x)$ với $x \neq 0$, trong đó

$$
g(x) = 1 + \frac{a_1}{a_0 x} + \cdots + \frac{a_n}{a_0 x^n}
$$

tiến tới $+1$ khi $x$ tiến tới $+\infty$ hoặc $-\infty$. Do đó tồn tại một số $a > 0$ sao cho $f(a)$ có dấu của $a_0$ và $f(-a)$ có dấu của $-a_0$;

và do đó theo định lý Bolzano (Chương IV, § 6, no. 1, Định lý 2), $f$ có ít nhất một nghiệm trong $[—a, a]$.

#### Nhận xét 1 {#top-viii-s1-n1-rem-1 .statement}

Định lý 1 có thể được chứng minh mà không cần viện đến lý thuyết các trường có thứ tự, bằng cách sử dụng các tính chất của tôpô của trường $\mathbf{C}$, sẽ được định nghĩa dưới đây (no. 2); xem § 2, Bài tập 2 và cả phần của bộ sách này dành cho tôpô đại số, trong đó định lý d’Alembert-Gauss sẽ xuất hiện như một hệ quả của các kết quả về bậc của một ánh xạ.
2) Vì $\mathbf{C}$ có bậc 2 trên $\mathbf{R}$, suy ra rằng $\mathbf{C}$, tới đẳng cấu, là mở rộng đại số duy nhất của $\mathbf{R}$ khác với chính $\mathbf{R}$, và không có trường nào được chứa trong $\mathbf{C}$ chứa $\mathbf{R}$, ngoài $\mathbf{R}$ và $\mathbf{C}$.

Ta biết rằng $\mathbf{R}$ có thể được đồng nhất với một trường con của $\mathbf{C}$, và mọi $z \in \mathbf{C}$ đều có thể được viết duy nhất dưới dạng $x + iy$, trong đó $x$ và $y$ là thực; $x$ được gọi là phần thực của $z$ và được ký hiệu bởi $\Re(z)$; $y$ là phần ảo của $z$, được ký hiệu bởi $\Im(z)$. Các số phức có dạng $iy$ ($y$ thực) được gọi là các số thuần ảo. Quan hệ $x + iy = 0$ ($x, y$ thực) tương đương với $x = 0$ và $y = 0$.

Vì $i^2 = -1$, các phần tử của $\mathbf{C}$ (khi được cho bởi phần thực và phần ảo của chúng) thỏa mãn các quy tắc tính toán sau:

$$
(x + iy) + (x' + iy') = (x + x') + i(y + y')
$$
$$
(x + iy)(x' + iy') = (xx' - yy') + i(xy' + x'y').
$$

Đặc biệt, $(x + iy)(x - iy) = x^2 + y^2 \in \mathbf{R}$, do đó, nếu $x + iy \neq 0$,

$$
\frac{1}{x + iy} = \frac{x}{x^2 + y^2} - i \frac{y}{x^2 + y^2}.
$$

Nghiệm thứ hai của đa thức $X^2 + 1$ trong $\mathbf{C}$ là $-i$; do đó tự đẳng cấu duy nhất của $\mathbf{C}$, khác ánh xạ đồng nhất, giữ bất biến mọi số thực, là tự đẳng cấu biến $z = x + iy$ thành $x - iy$; tự đẳng cấu sau được ký hiệu bởi $\overline{z}$ và (phù hợp với các định nghĩa tổng quát) được gọi là số phức liên hợp với $z$. Ta có

$$
\Re(z) = \frac{1}{2}(z + \overline{z}) \quad \text{và} \quad \Im(z) = \frac{1}{2i}(z - \overline{z}).
$$

Do tự đẳng cấu này, nếu $f(z)$ là một đa thức với các hệ số thực, ta có $f(\overline{z}) = \overline{f(z)}$ với mọi $z \in \mathbf{C}$.

Số thực $z \overline{z} = x^2 + y^2$ được gọi là chuẩn đại số của $z$, hoặc đơn giản là chuẩn khi không có nguy cơ nhầm lẫn; đó là một số thực $\geq 0$, bằng không chỉ khi $z = 0$. Số thực $\sqrt{z \overline{z}} = \sqrt{x^2 + y^2} \geq 0$ trở thành giá trị tuyệt đối của $z$ khi $z$ là thực, và ta vẫn gọi nó là giá trị tuyệt đối của $z$, và ký hiệu bởi $|z|$, khi $z$ là một số phức bất kỳ. Quan hệ $|z| = 0$ tương đương với $z = 0$. Nếu $z$ và $z'$ là hai số phức, số liên hợp của $zz'$ là $\overline{zz'}$, do đó $|zz'|^2 = zz'\overline{zz'} = |z|^2|z'|^2$ và vì vậy $|zz'| = |z|\cdot|z'|$: *giá trị tuyệt đối của một tích là tích các giá trị tuyệt đối của các thừa số.* Đặc biệt, nếu $z \neq 0$ và $z' = 1/z$, ta có $|1/z| = |1/z|$.

Cuối cùng, với mọi số phức $z, z'$, ta có *bất đẳng thức tam giác*
$$
|z + z'| \leq |z| + |z'|.
$$

### 2. TÔPÔ CỦA $\mathbf{C}$

Ánh xạ $(x, y) \to x + iy$ của mặt phẳng thực $\mathbf{R}^2$ lên $\mathbf{C}$ là \*song ánh\*; bằng song ánh này, ta có thể \*chuyển\* tôpô của $\mathbf{R}^2$ sang $\mathbf{C}$ (xem Chương VI, § 1, no. 5). Tôpô được xác định như vậy trên $\mathbf{C}$ \*tương thích\* với cấu trúc trường của $\mathbf{C}$ (Chương III, § 6, no. 7), vì nó tương thích với cấu trúc vành của $\mathbf{C}$ (Chương VI, § 1, no. 5) và, theo (3), $1/z$ liên tục trên phần bù $\mathbf{C}^*$ của 0 trong $\mathbf{C}$.

Nếu ta trang bị cho tập hợp $\mathbf{C}$ tôpô này và cấu trúc trường đã định nghĩa trước đó (no. 1, Định nghĩa 1), thì ta đã xác định trên $\mathbf{C}$ cấu trúc của một \*trường tôpô\* (Chương III, § 6, no. 7); từ nay, mỗi khi nói đến tôpô của $\mathbf{C}$, ta luôn hiểu đó là tôpô trên.

Trong tương lai, nói chung ta sẽ \*đồng nhất\* các tập hợp $\mathbf{C}$ và $\mathbf{R}^2$ được xét như các không gian tôpô; khi đó trường con $\mathbf{R}$ của $\mathbf{C}$ được đồng nhất với hoành độ của $\mathbf{R}^2$, vì lý do đó được gọi là \*trục thực\*; tương tự, tung độ được gọi là \*trục ảo\* (chú ý rằng đây \*không phải\* là một trường con của $\mathbf{C}$). Tia có gốc 0 và các tỉ số phương $(1, 0)$ (được đồng nhất với $\mathbf{R}_+$) được gọi là \*nửa trục thực dương\*; tia đối, có cùng gốc và các tỉ số phương $(-1, 0)$, được gọi là \*nửa trục thực âm\*.

Nhằm mục đích minh họa bằng hình vẽ, ta dùng biểu diễn của $\mathbf{R}^2$ (quen thuộc trong hình học giải tích sơ cấp) bằng các điểm của một mặt phẳng trong đó đã vẽ hai trục tọa độ vuông góc, lần lượt biểu diễn trục thực và trục ảo của $\mathbf{C}$ (Hình 7).

Cũng như trong mọi trường tôpô, mọi \*hàm hữu tỉ\* của $n$ biến phức với các hệ số phức đều \*liên tục\* tại mọi điểm của $\mathbf{C}^n$ mà tại đó mẫu khác không.

![Một biểu đồ cho thấy mặt phẳng phức với các trục được ký hiệu x và y, và một điểm được ký hiệu z = x + iy](https://i.imgur.com/3Q5z5QG.png)

Hình 7.

Phép hoán vị $z \to \overline{z}$ của $\mathbf{C}$ là liên tục, và do đó là một tự đẳng cấu của trường tôpô $\mathbf{C}$.

Thực ra đó là tự đẳng cấu duy nhất của trường tôpô $\mathbf{C}$ ngoài tự đẳng cấu đồng nhất (xem Bài tập 4).

Các hàm $\Re(z), \Im(z)$ chính là các phép chiếu của $\mathbf{R}^2$ lên các nhân tử của nó, và do đó liên tục; điều tương tự cũng đúng với giá trị tuyệt đối $|z|$, vì đó là chuẩn Euclid (Chương VI, § 2, no. 1) của điểm $(x, y)$ trong $\mathbf{R}^2$.

Các tính chất của giá trị tuyệt đối dẫn đến một chứng minh khác cho sự kiện rằng tôpô của $\mathbf{C}$ tương thích với cấu trúc trường của nó (xem Chương IX, § 3, no. 2); tính liên tục của $z + z'$ suy ra từ bất đẳng thức tam giác $|z + z'| \leq |z| + |z'|$; tính liên tục của $zz'$ suy ra từ quan hệ
$$
|zz' - z_0z'_0| = |z_0(z' - z'_0) + (z - z_0)z'_0 + (z - z_0)(z' - z'_0)| \\\\
\leq |z_0| \cdot |z' - z'_0| + |z'_0| \cdot |z - z_0| + |z - z_0| \cdot |z' - z'_0|;
$$
cuối cùng, tính liên tục của $z^{-1}$ suy ra từ quan hệ
$$
|z_0^{-1} - z^{-1}| = |z|^{-1} \cdot |z - z_0| \cdot |z_0|^{-1}.
$$

### 3. NHÓM NHÂN $\mathbf{C}^*$

Ta biết từ Chương III, § 6, no. 7 rằng tôpô cảm sinh trên nhóm nhân $\mathbf{C}^*$ của các số phức khác không tương thích với cấu trúc nhóm của $\mathbf{C}^*$. Vì $\mathbf{C}^*$ là mở trong $\mathbf{C}$, suy ra rằng $\mathbf{C}^*$ là một nhóm tôpô địa phương compact (Chương I, § 9, no. 7, Mệnh đề 13) và do đó đầy đủ (đối với cấu trúc đều nhân; xem Chương III, § 6, no. 8, Mệnh đề 8). Nhóm nhân $\mathbf{R}_+^*$ của các số thực $> 0$ là một nhóm con đóng của $\mathbf{C}^*$. Một nhóm con khác là tập hợp $\mathbf{U}$ gồm các số phức có giá trị tuyệt đối bằng 1, được đồng nhất với đường tròn đơn vị $S_1$ của $\mathbf{R}^2$, và do đó là một nhóm compact. Hơn nữa:

#### Mệnh đề 1 {#top-viii-s1-prop-1 .statement}

\*Nhóm tôpô $\mathbf{C}^*$ đẳng cấu với tích của các nhóm tôpô $\mathbf{R}^*$ và $\mathbf{U}$.\*

Vì ánh xạ $z \to \left( |z|, \frac{z}{|z|} \right)$ là một phép đồng phôi từ $\mathbf{C}^*$ lên $\mathbf{R}_+^* \times \mathbf{U}$ (Chapter VI, § 2, no. 3, Mệnh đề 3); và suy ra ngay lập tức rằng nó là một đẳng cấu của các cấu trúc nhóm.

Nhóm tôpô $\mathbf{R}_+^*$ đã được biết là đẳng cấu với nhóm cộng $\mathbf{R}$ (Chapter V, § 4, Định lý 1); do đó việc nghiên cứu nhóm tôpô $\mathbf{C}^*$ được quy về việc nghiên cứu $\mathbf{U}$, mà ta sẽ xét trong § 2.

### 4. VÀNH CHIA CỦA CÁC QUATERNION

Từ Định lý 1 suy ra rằng trường $\mathbf{R}$ là một trường có thứ tự cực đại, và do đó vành chia không giao hoán duy nhất có hạng hữu hạn trên $\mathbf{R}$ là (sai khác một đẳng cấu) vành chia của các quaternion trên $\mathbf{R}$; nó được ký hiệu là $\mathbf{H}$ và được gọi là vành chia của các quaternion thực (hoặc đơn giản là vành chia của các quaternion, khi không sợ nhầm lẫn). Vì $\mathbf{H}$ có hạng 4 trên trường $\mathbf{R}$, ta có thể định nghĩa trên $\mathbf{H}$ một tôpô đồng phôi với tôpô của $\mathbf{R}^4$ (Chapter VI, § 1, no. 5). Chính xác hơn, ta thường đồng nhất $\mathbf{H}$ với $\mathbf{R}^4$, các phần tử $i, i, j, k$ của cơ sở chính tắc của $\mathbf{H}$ lần lượt được đồng nhất với các vectơ $e_0, e_1, e_2, e_3$ của cơ sở chính tắc của $\mathbf{R}^4$.

Ta nhắc lại rằng bảng phép nhân của cơ sở chính tắc của $\mathbf{H}$ được cho bởi các công thức

$$
i^2 = j^2 = k^2 = -1, \quad ij = -ji = k,
jk = -kj = i, \quad ki = -ik = j.
$$

Tôpô của $\mathbf{H}$ không chỉ tương thích với cấu trúc vành của $\mathbf{H}$ (Chapter VI, § 1, no. 5) mà còn với cấu trúc vành chia của nó; vì nếu $x$ là một quaternion khác không, các tọa độ của $x^{-1}$ là các hàm hữu tỉ của các tọa độ của $x$, mà mẫu số không triệt tiêu. Do đó, vành chia $\mathbf{H}$, được trang bị tôpô này, là một vành chia tôpô không giao hoán. Các quaternion $a + bi$ ($a, b$ thực) tạo thành một trường con (tôpô) của $\mathbf{H}$, đẳng cấu với trường $\mathbf{C}$, mà với nó thường được đồng nhất.

Như vậy ta có một ví dụ thứ ba về một vành chia tôpô liên thông, compact địa phương, hai ví dụ kia là $\mathbf{R}$ và $\mathbf{C}$. Thực ra, đây là những vành chia tôpô duy nhất có hai tính chất này.

Từ đại số, ta biết rằng chuẩn rút gọn của một quaternion $x = x_0 + x_1 i + x_2 j + x_3 k$ là

$$
N(x) = x_0^2 + x_1^2 + x_2^2 + x_3^2 = ||x||^2
$$

(do đó nó là bình phương của chuẩn Euclid của $x$). Vì

$$
N(xy) = N(x)N(y),
$$

suy ra rằng tập hợp tất cả các quaternion có chuẩn bằng 1, đồng nhất với mặt cầu $S_3$, tạo thành một nhóm con compact của nhóm nhân $\mathbf{H}^*$ gồm các quaternion khác không.

#### Mệnh đề 2 {#top-viii-s1-prop-2 .statement}

Nhóm nhân $\mathbf{H}^*$ gồm các quaternion khác không là một nhóm tôpô đẳng cấu với tích của các nhóm con $\mathbf{R}_+^*$ và $S_3$.

Mọi quaternion $x / o$ đều có thể viết dưới dạng $x \cdot z$ trong đó $z$ là một quaternion có chuẩn bằng 1; vì $\|xx'\| = \|x\|\cdot\|x'\|$, ánh xạ $x \to (\|x\|, x_1, x_2)$ từ $H^*$ lên $\mathbf{R}_+^* \times S_2$ là một đẳng cấu của các cấu trúc nhóm, và theo Chapter VI, § 2, no. 2, Mệnh đề 2, nó là một đồng cấu từ $H^*$ lên $\mathbf{R}_+^* \times S_2$.

#### Nhận xét 1 {#top-viii-s1-n4-rem-1 .statement}

Bằng cách sử dụng các hệ thức $\|x + y\| = \|x\| + \|y\|$ và $\|xy\| = \|x\|\cdot\|y\|$ ta có thể chứng minh trực tiếp, như đối với trường các số phức trong no. 2, rằng tôpô của $\mathbf{R}^4$ tương thích với cấu trúc vành chia của $H$ (cf. Chapter IX, § 3, no. 2).

#### Nhận xét 2 {#top-viii-s1-n4-rem-2 .statement}

Từ những gì đã chứng minh, suy ra rằng các mặt cầu $S_1$ và $S_n$ có thể mang một cấu trúc nhóm tương thích với tôpô của chúng. Sau này ta sẽ thấy rằng, với mỗi số nguyên $n$ khác 1 và 3, không tồn tại cấu trúc nhóm nào trên $S_n$ tương thích với tôpô của $S_n$.

#### Nhận xét 3 {#top-viii-s1-n4-rem-3 .statement}

Mỗi điểm của nhóm $S_2$ đều có một lân cận đồng phôi với $\mathbf{R}^3$ (chương VI, § 2, no. 4, Mệnh đề 5), nhưng $S_4$ không địa phương đẳng cấu với $\mathbf{R}^3$; vì nếu có thì nó sẽ Abel, do nó liên thông (chương VII, § 2, no. 2, Định lý 1), và điều này không đúng, vì $i$ và $j$ thuộc $S_3$ và $ij \neq ji$ (xem chương V, § 3).

### Bài tập {#top-viii-s1-exercises}

Xem [các bài tập của § 1](exercises/s1/).
