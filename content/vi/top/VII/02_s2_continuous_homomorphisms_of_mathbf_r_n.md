---
book: top
book_title: General Topology
chapter: VII
chapter_title: The additive groups $\mathbf{R}^n$
section: 2
section_title: Continuous homomorphisms of $\mathbf{R}^n$ and its quotient groups
lang: vi
source: top-v-x
pdf_pages: 0085-0089, 0099-0101
extraction: ocr
subsections:
    - "no": 1
      title: CONTINUOUS HOMOMORPHISMS OF THE GROUP $\mathbf{R}^m$ INTO THE GROUP $\mathbf{R}^n$
      page: 0
      pdf_page: 85
    - "no": 2
      title: LOCAL DEFINITION OF A CONTINUOUS HOMOMORPHISM OF $\mathbf{R}^n$ INTO A TOPOLOGICAL GROUP
      page: 0
      pdf_page: 85
    - "no": 3
      title: CONTINUOUS HOMOMORPHISMS OF $\mathbf{R}^m$ INTO $\mathbf{T}^n$
      page: 0
      pdf_page: 87
    - "no": 4
      title: AUTOMORPHISMS OF $\mathbf{T}^n$
      page: 0
      pdf_page: 88
statements: 10
exercises: 7
content_sha256: cd87a5f1f6488f4ae5e2cc3707a1dd509720b39554a184a36590004d0b0bf1b5
translated_from: content/en/top/VII/02_s2_continuous_homomorphisms_of_mathbf_r_n.md
source_content_sha256: 92b475781e2cf8088893813862965f43bc36bf3c5060161832b5e64d7459548d
translation_model: gpt-5-6-mini, gpt-5-6
translation_run: translate-vi-4b78a625
glossary_version: 34
glossary_terms_sha256: a5878a69ebe57533dd6412083dc1952dfcd782b1b322cc15ede40d4c2da19a7e
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 2. CÁC ĐỒNG CẤU LIÊN TỤC CỦA $\mathbf{R}^n$ VÀ CÁC NHÓM THƯƠNG CỦA NÓ

### 1. CÁC ĐỒNG CẤU LIÊN TỤC CỦA NHÓM $\mathbf{R}^m$ VÀO NHÓM $\mathbf{R}^n$

Mọi ánh xạ tuyến tính (xem Chương VI, § i, no. 3) của $\mathbf{R}^m$ vào $\mathbf{R}^n$ hiển nhiên là một đồng cấu liên tục của nhóm cộng $\mathbf{R}^m$ vào nhóm cộng $\mathbf{R}^n$. Ngược lại:

#### Mệnh đề 1 {#top-vii-s2-prop-1 .statement}

*Mọi đồng cấu liên tục* $f$ *của nhóm cộng* $\mathbf{R}^m$ *vào nhóm cộng* $\mathbf{R}^n$ *là một ánh xạ tuyến tính của* $\mathbf{R}^m$ *vào* $\mathbf{R}^n$.

Chỉ cần chứng minh rằng $f(tx) = tf(x)$ với mọi $x \in \mathbf{R}^n$ và mọi $t \in \mathbf{R}$. Lập luận cũng giống như lập luận của Mệnh đề 5 của Chương V, § i, no. 3 nếu ta thay $x$ bởi $x$ và $\mathbf{R}$ bởi $\mathbf{R}^m$.

### 2. ĐỊNH NGHĨA ĐỊA PHƯƠNG CỦA MỘT ĐỒNG CẤU LIÊN TỤC CỦA $\mathbf{R}^n$ VÀO MỘT NHÓM TÔPÔ

Mệnh đề 6 của Chương V, § i, no. 4 có thể được tổng quát hóa cho mọi nhóm $\mathbf{R}^n$.

#### Mệnh đề 2 {#top-vii-s2-prop-2 .statement}

*Cho* $A$ *là một hình hộp song song trong* $\mathbf{R}^n$ *chứa* $o$; *và cho* $f$ *là một ánh xạ liên tục của* $A$ *vào một nhóm tôpô* $G$ *(viết theo phép nhân)* *sao cho* $f(x + y) = f(x)f(y)$ *với mỗi cặp điểm* $x, y$ *sao cho* $x \in A,\ y \in A$ *và* $x + y \in A$. *Khi đó tồn tại một đồng cấu liên tục duy nhất của* $\mathbf{R}^n$ *vào* $G$ *mở rộng* $f$.

Theo cùng lập luận như trong Mệnh đề 6 của Chương V, § i, no. 4 ta chứng minh rằng đồng cấu mở rộng $f$, nếu tồn tại, là *duy nhất*. Tiếp theo, nhóm con $G_1$ của $G$, sinh bởi $f(A)$, là *giao hoán*; vì nếu $x$ và $y$ là hai điểm bất kỳ của $A$, thì $\frac{1}{2} x, \frac{1}{2} y$ và $\frac{1}{2} (x + y)$ thuộc $A$, do đó

$$
f \left( \frac{1}{2} (x + y) \right) = f \left( \frac{1}{2} x \right) \quad (f \frac{1}{2} y) = f \left( \frac{1}{2} y \right) f \left( \frac{1}{2} x \right),
$$

điều này cho thấy rằng $f \left( \frac{1}{2} x \right)$ và $f \left( \frac{1}{2} y \right)$ giao hoán; do đó $f(x) = (f \left( \frac{1}{2} x \right))^2$ và $f(y) = (f \left( \frac{1}{2} y \right))^2$ cũng vậy, điều này chứng minh mệnh đề.

Cho $a_1, a_2, \ldots, a_n$ là $n$ vectơ khác không thuộc $A$ và tỉ lệ với các vectơ cơ sở của hình hộp song song, và với mỗi chỉ số $i$ gọi $D_i$ là đường thẳng đi qua $o$ và $a_i$, nghĩa là tập hợp các điểm $ta_i$ khi $t$ chạy qua $\mathbf{R}$. Gọi $A_i$ là tập hợp mọi $t \in \mathbf{R}$ sao cho $ta_i \in A$; khi đó $A_i$ là một khoảng của $\mathbf{R}$ chứa $[0, 1]$, và hàm

$$
f_i(t) = f(ta_i)
$$

được xác định và liên tục trên $A_i$ và thỏa mãn quan hệ

$$
f_i(t + t') = f_i(t) f_i(t')
$$

khi $t, t'$ và $t + t'$ đều thuộc $A_i$. Theo Mệnh đề 6 của Chương V, § 1, no. 4, tồn tại một đồng cấu liên tục $\bar{f}_i$ của $\mathbf{R}$ vào $G$ mở rộng $f_i$. Vì $\mathbf{R}^n$ là tổng trực tiếp của các nhóm con $D_i$, ta có thể định nghĩa một đồng cấu $\bar{f}$ của $\mathbf{R}^n$ vào nhóm Abel $G_1$ bởi quy tắc $\bar{f}(x) = \prod_{i=1}^n \bar{f}_i(t_i)$ trong đó $x = \sum_{i=1}^n t_i a_i$; $\bar{f}$ là một mở rộng của $f$ vì, nếu $x \in A$, mọi thành phần $x_i$ của $x$ trên các đường thẳng $D_i$ cũng thuộc $A$, do sự lựa chọn các $a_i$; hơn nữa, $\bar{f}$ liên tục trên $\mathbf{R}^n$, vì nó liên tục trên mỗi đường thẳng $D_i$, và $x_i$ là một hàm tuyến tính của $x$ (và do đó liên tục).

#### Hệ quả 1 {#top-vii-s2-prop-2-cor-1 .statement}

*Gọi $V$ là một lân cận của $o$ trong $\mathbf{R}^n$ và gọi $f$ là một ánh xạ liên tục của $V$ vào một nhóm tôpô $G$ sao cho*

$$
f(x + y) = f(x) f(y)
$$

*đối với mỗi cặp phần tử $x, y$ sao cho $x \in V, y \in V$ và $x + y \in V$. Khi đó tồn tại một đồng cấu liên tục duy nhất của $\mathbf{R}^n$ vào $G$ trùng với $f$ tại mọi điểm của một lân cận $W$ của $o$.*

Lấy $W$ là một hộp mở có tâm $o$, được chứa trong $V$, và áp dụng Mệnh đề 2 cho $W$.

Sau này ta sẽ thấy rằng tính chất này của $\mathbf{R}^n$ mở rộng đến một lớp lớn hơn các nhóm tôpô, các nhóm "liên thông đơn".

#### Hệ quả 2 {#top-vii-s2-prop-2-cor-2 .statement}

*Cho $f$ là một đẳng cấu địa phương của $\mathbf{R}^n$ với một nhóm tôpô $G$. Khi đó tồn tại một cấu xạ ngặt duy nhất của $\mathbf{R}^n$ lên một nhóm con mở của $G$ trùng với $f$ tại mọi điểm của một lân cận nào đó của $o$.*

Gọi $\overline{f}$ là đồng cấu liên tục của $\mathbf{R}^n$ vào $G$ trùng với $f$ tại mọi điểm của một lân cận của $o$; theo giả thiết, $\overline{f}(\mathbf{R}^n)$ chứa một lân cận của phần tử đơn vị của $G$ và do đó (Chương III, § 2, no. 1, Hệ quả của Mệnh đề 4) là một nhóm con mở của $G$; hơn nữa $\overline{f}$ là một cấu xạ ngặt của $\mathbf{R}^n$ lên $\overline{f}(\mathbf{R}^n)$, theo Chương III, § 2, no. 8, Mệnh đề 24.

#### Định lý 1 {#top-vii-s2-thm-1 .statement}

*Mọi nhóm liên thông $G$ đẳng cấu địa phương với $\mathbf{R}^n$ đều đẳng cấu với một nhóm $\mathbf{R}^p \times \mathbf{T}^{n-p}$ ($0 \leqslant p \leqslant n$).*

Một đẳng cấu địa phương $f$ được chọn thích hợp của $\mathbf{R}^n$ với $G$ mở rộng thành một cấu xạ ngặt của $\mathbf{R}^n$ lên một nhóm con mở của $G$ (Mệnh đề 2, Hệ quả 2) và do đó lên chính $G$, vì $G$ liên thông. Suy ra $G$ đẳng cấu với một nhóm thương $\mathbf{R}^n/H$ của $\mathbf{R}^n$: $H$ là *rời rạc*, nếu không sẽ tồn tại các điểm $x \neq o$ của $H$ tùy ý gần $o$ và sao cho $f(x) = f(o)$, trái với giả thiết rằng $f$ là một đẳng cấu địa phương. Vì vậy định lý là một hệ quả của Định lý 1 của § 1, no. 1.

### 3. CÁC ĐỒNG CẤU LIÊN TỤC CỦA $\mathbf{R}^m$ VÀO $\mathbf{T}^n$

#### Mệnh đề 3 {#top-vii-s2-prop-3 .statement}

*Mọi đồng cấu liên tục từ $\mathbf{R}^m$ vào $\mathbf{T}^n$ đều có dạng $x \to \varphi(u(x))$, trong đó $\varphi$ là đồng cấu chính tắc của $\mathbf{R}^n$ lên $\mathbf{T}^n$ (được đồng nhất với $\mathbf{R}^n/\mathbf{Z}^n$) và $u$ là một ánh xạ tuyến tính từ $\mathbf{R}^m$ vào $\mathbf{R}^n$.*

Cho $f$ là một đồng cấu liên tục từ $\mathbf{R}^m$ vào $\mathbf{T}^n$. Ta sẽ chứng minh rằng có một ánh xạ tuyến tính $u$ từ $\mathbf{R}^m$ vào $\mathbf{R}^n$ sao cho các đồng cấu $x \to f(x)$ và $x \to \varphi(u(x))$ trùng nhau tại mọi điểm của một *lân cận của* $o$ trong $\mathbf{R}^m$; khi đó mệnh đề sẽ suy ra từ Hệ quả 1 của Mệnh đề 2 ở no. 2. Bây giờ cho $V$ là một lân cận của $o$ trong $\mathbf{R}^n$ sao cho $\varphi$, hạn chế trên $V$, là một đẳng cấu địa phương của $\mathbf{R}^n$ với $\mathbf{T}^n$, và cho $\psi$ là nghịch đảo của $\varphi$, được xác định trên $\varphi(V)$. Vì $f$ liên tục, $V' = \overline{f}^{-1}(\varphi(V))$ là một lân cận của $o$ trong $\mathbf{R}^m$; ánh xạ

$$
x \to \psi(f(x)),
$$

hạn chế trên $V'$, là một ánh xạ liên tục từ $V'$ vào $\mathbf{R}^n$ sao cho $\psi(f(x+y)) = \psi(f(x)) + \psi(f(y))$ với mỗi cặp điểm $x, y$ trong $\mathbf{R}^m$ sao cho $x \in V', y \in V'$ và $x + y \in V'$; do đó (no. 2, Hệ quả 1 của Mệnh đề 2) ánh xạ này trùng với một đồng cấu liên tục $u$ được xác định duy nhất từ $\mathbf{R}^m$ vào $\mathbf{R}^n$ tại mọi điểm của một lân cận $W$ của o trong $\mathbf{R}^m$. Theo Mệnh đề 1 (no. 1) $u$ là một ánh xạ tuyến tính từ $\mathbf{R}^m$ vào $\mathbf{R}^n$; do đó với mọi $x \in W$ ta có $f(x) = \varphi(u(x))$, điều này hoàn thành chứng minh.

#### Nhận xét {#top-vii-s2-n3-rem-1 .statement}

Lập luận tương tự chỉ ra, nói chung hơn, rằng nếu $\varphi$ là một cấu xạ ngặt từ $\mathbf{R}^n$ vào một nhóm $G$, mà hạn chế của nó trên một lân cận thích hợp của o là một đẳng cấu địa phương của $\mathbf{R}^n$ với $G$, thì mọi đồng cấu liên tục từ $\mathbf{R}^n$ vào $G$ đều có dạng $x \mapsto \varphi(u(x))$, trong đó $u$ là một ánh xạ tuyến tính từ $\mathbf{R}^m$ vào $\mathbf{R}^n$.

Trong trường hợp $m = n = 1$, Mệnh đề 3 cho:

#### Mệnh đề 4 {#top-vii-s2-prop-4 .statement}

*Nếu $\varphi$ là đồng cấu chính tắc của $\mathbf{R}$ lên $\mathbf{T}$, mọi đồng cấu liên tục từ $\mathbf{R}$ vào $\mathbf{T}$ đều có dạng $x \mapsto \varphi(ax)$ trong đó $a \in \mathbf{R}$; và nó là một cấu xạ ngặt từ $\mathbf{R}$ lên $\mathbf{T}$ nếu $a \neq 0$.*

### 4. CÁC TỰ ĐẲNG CẤU CỦA $\mathbf{T}^n$

Cho $H$ là một nhóm con đóng của $\mathbf{R}^n$ và cho $\varphi$ là đồng cấu chính tắc của $\mathbf{R}^n$ lên nhóm thương $\mathbf{R}^n/H$. Nếu $f$ là một đồng cấu liên tục từ $\mathbf{R}^n/H$ vào một nhóm tôpô $G$, thì $f = f \circ \varphi$ là một đồng cấu liên tục từ $\mathbf{R}^n$ vào $G$ tuần hoàn và có một nhóm các chu kỳ chứa $H$; ngược lại mọi đồng cấu liên tục tuần hoàn từ $\mathbf{R}^n$ vào $G$, mà nhóm các chu kỳ chứa $H$, đều có dạng này.

Trong trường hợp $H = \mathbf{Z}^n$, nhóm thương $\mathbf{R}^n/\mathbf{Z}^n = \mathbf{T}^n$ là *compact*, và do đó mọi đồng cấu liên tục $f$ của $\mathbf{T}^n$ vào một nhóm tôpô $G$ là một *cấu xạ ngặt* từ $\mathbf{T}^n$ vào $G$, với điều kiện $G$ là Hausdorff (Chương III, § 2, no. 8, Nhận xét 1); $f = f \circ \varphi$ là một cấu xạ ngặt từ $\mathbf{R}^n$ vào $G$; hơn nữa, $f(\mathbf{T}^n) = f(\mathbf{R}^n)$ là một nhóm con *compact* của $G$, đẳng cấu với một nhóm $\mathbf{T}^p$ ($0 \leq p \leq n$).

Đặc biệt, ta thấy rằng đồng cấu liên tục duy nhất từ $\mathbf{T}^n$ vào một nhóm $\mathbf{R}^m$ là ánh xạ *không*, vì $\{ o \}$ là nhóm con compact duy nhất của $\mathbf{R}^m$.

Ta áp dụng điều này cho các đồng cấu liên tục của $\mathbf{T}^n$ vào một nhóm $\mathbf{T}^p$; nếu $f$ là một đồng cấu như vậy, $\varphi$ là đồng cấu chính tắc của $\mathbf{R}^n$ lên $\mathbf{T}^n$, thì $f \circ \varphi$ là một đồng cấu liên tục của $\mathbf{R}^n$ vào $\mathbf{T}^p$; do đó (no. 3, Mệnh đề 3) nếu $\psi$ ký hiệu đồng cấu chính tắc của $\mathbf{R}^p$ lên $\mathbf{T}^p$, tồn tại một ánh xạ tuyến tính $u$ của $\mathbf{R}^n$ vào $\mathbf{R}^p$ sao cho $f \circ \varphi = \psi \circ u$. Nếu $x \in \mathbf{Z}^n$, $f(\varphi(x))$ là phần tử đơn vị của $\mathbf{T}^p$, do đó ta phải có $u(x) \in \mathbf{Z}^p$, nghĩa là, $u(\mathbf{Z}^n) \subset \mathbf{Z}^p$. Ngược lại, nếu $u$ là bất kỳ ánh xạ tuyến tính nào của $\mathbf{R}^n$ vào $\mathbf{R}^p$ thỏa mãn điều kiện này, thì $\psi \circ u$ là một đồng cấu liên tục tuần hoàn của $\mathbf{R}^n$ vào $\mathbf{T}^p$, mà nhóm các chu kỳ của nó chứa $\mathbf{Z}^n$, và do đó xác định một đồng cấu liên tục của $\mathbf{T}^n$ vào $\mathbf{T}^p$.

Xét các điều kiện để $f$ là một *đẳng cấu* của $\mathbf{T}^n$ lên một nhóm con của $\mathbf{T}^p$. Trước hết, $u$ phải là một ánh xạ *đơn ánh* của $\mathbf{R}^n$ vào $\mathbf{R}^p$, nếu không, không gian vectơ con $\overline{u}(0)$ sẽ chứa các điểm $x \neq 0$ tùy ý gần điểm gốc, và tại một điểm như vậy ta sẽ có
$$
f(\varphi(x)) = f(\varphi(0)) \quad \text{và} \quad \varphi(x) \neq \varphi(0),
$$
trái với giả thiết. Điều kiện này kéo theo $p \geq n$. Ảnh $u(\mathbf{Z}^n)$ khi đó là một nhóm con rời rạc hạng $n$ của nhóm $\mathbf{Z}^p$; các *nhân tử bất biến* của $u(\mathbf{Z}^n)$ đối với $\mathbf{Z}^p$ (\S 1, no. 1) phải đều bằng 1, nếu không sẽ tồn tại một điểm $x \in \mathbf{Z}^n$ và một số nguyên $k > 1$ sao cho $u(k^{-1}x) \in \mathbf{Z}^n$ và $k^{-1} \notin \mathbf{Z}^n$, do đó $f(\varphi(k^{-1}x)) = f(\varphi(0))$ và $\varphi(k^{-1}x) \neq \varphi(0)$, trái với giả thiết. Ngược lại, nếu điều kiện này được thỏa mãn, $u(\mathbf{R}^n) \cap \mathbf{Z}^n = u(\mathbf{Z}^n)$, và $f$ là một đẳng cấu của $\mathbf{T}^n$ lên $u(\mathbf{R}^n)/u(\mathbf{Z}^n)$.

Nếu ta áp dụng lập luận này vào trường hợp $p = n$, ta có mệnh đề sau:

#### Mệnh đề 5 {#top-vii-s2-prop-5 .statement}

*Mọi đẳng cấu của nhóm tôpô $\mathbf{T}^n$ lên một trong các nhóm con của nó là một tự đẳng cấu của $\mathbf{T}^n$ thu được bằng cách chuyển qua thương từ một ánh xạ tuyến tính $u$ của $\mathbf{R}^n$ lên chính nó, ánh xạ này, hạn chế trên $\mathbf{Z}^n$, là một tự đẳng cấu của $\mathbf{Z}^n$.*

Tương đương (\S 1, no. 1), nếu $u(e_i) = \sum_{j=1}^n a_{ij} e_j$, thì các $a_{ij}$ phải là các số nguyên sao cho $\det(a_{ij}) = \pm 1$. Đặc biệt, với $n = 1$:

#### Mệnh đề 6 {#top-vii-s2-prop-6 .statement}

*Các đẳng cấu duy nhất của nhóm tôpô $\mathbf{T}$ lên một trong các nhóm con của nó là ánh xạ đồng nhất và phép đối xứng $x \to -x$.*

### Bài tập {#top-vii-s2-exercises}

Xem [các bài tập cho § 2](exercises/s2/).
