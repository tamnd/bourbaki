---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Semisimple Modules and Rings
section: 1
section_title: Algebras without Unit Element
appendix: true
lang: vi
source: alg-viii
source_edition: 2023, Springer Nature
book_pages: A VIII.435-A VIII.446
pdf_pages: 0452-0463
extraction: native
subsections:
    - "no": 1
      title: Regular Ideals
      page: 435
      pdf_page: 452
    - "no": 2
      title: Adjunction of a Unit Element
      page: 437
      pdf_page: 454
    - "no": 3
      title: The Radical of an Algebra
      page: 439
      pdf_page: 456
    - "no": 4
      title: Density Theorem
      page: 442
      pdf_page: 459
statements: 20
exercises: 15
content_sha256: 2d67e2a3e6694c9019fa7c443c507a30898d04ef0250ef5c0264fb9d083e1e8f
translated_from: content/en/alg/VIII/A1_a1_algebras_without_unit_element.md
source_content_sha256: 98c6a5e57906681f8c0a6b353e8a358c25cc514a68622fa99dc2d3817a1b28f4
translation_model: gpt-5-6, gpt-5.4
translation_run: translate-vi-74c08a00
glossary_version: 34
glossary_terms_sha256: 30c7096abc156c3bd08bd4acef2072f1c4b92e78fbf250bc1a8060b563229959
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## PHỤ LỤC 1 ĐẠI SỐ KHÔNG CÓ PHẦN TỬ KHẢ NGHỊCH

Trong phụ lục này, $k$ là một vành giao hoán; các $k$-đại số được giả thiết là kết hợp nhưng không nhất thiết có đơn vị.

### 1. Iđêan chính quy

Cho A là một $k$-đại số. Nhắc lại (III, §1, No. 2, p. 430) rằng một iđêan trái của A là một $k$-môđun con $\mathfrak{a}$ của A sao cho các quan hệ $a\in A, x\in \mathfrak{a}$ kéo theo $ax\in \mathfrak{a}$. Ta định nghĩa tương tự các khái niệm iđêan phải và iđêan hai phía. Nếu A là một $k$-đại số và $\mathfrak{a}$ là một iđêan hai phía của A, thì khi chuyển qua các thương, phép nhân trong A xác định một cấu trúc $k$-đại số trên $k$-môđun $A/\mathfrak{a}$ (loc. cit.).

Một iđêan trái của A được gọi là cực đại nếu nó là một phần tử cực đại của tập hợp các iđêan trái thực sự của A đối với quan hệ bao hàm.

#### Định nghĩa 1 {#alg-viii-a1-def-1 .statement tag=00P4}

Cho A là một $k$-đại số và $\mathfrak{a}$ là một iđêan trái của A. Một phần tử $u$ của A sao cho $au-a$ thuộc $\mathfrak{a}$ với mọi $a\in A$ được gọi là một đơn vị phải modulo $\mathfrak{a}$. Ta nói rằng iđêan $\mathfrak{a}$ là chính quy nếu tồn tại một đơn vị phải modulo $\mathfrak{a}$.

Tương tự, ta nói rằng một iđêan phải $\mathfrak{b}$ của A là chính quy nếu A có một đơn vị trái modulo $\mathfrak{b}$, nghĩa là, một phần tử $v$ sao cho $va-a\in \mathfrak{b}$ với mọi $a\in A$. Khi một iđêan là hai phía, cần chỉ rõ nó chính quy với tư cách iđêan trái hay với tư cách iđêan phải.

Khi đại số A có đơn vị, phần tử đơn vị của A là một đơn vị phải modulo $\mathfrak{a}$ đối với mọi iđêan trái $\mathfrak{a}$ của A; trong trường hợp này, mọi iđêan trái (hoặc phải) của A đều chính quy. Mặt khác, nếu A là một $k$-đại số mà mọi phần tử của nó đều lũy linh, thì A là iđêan duy nhất (trái hoặc phải) của A chính quy.

Cho $\mathfrak{a}$ là một iđêan trái chính quy của A và $u$ là một đơn vị phải modulo $\mathfrak{a}$. Nếu $\mathfrak{b}$ là một iđêan trái của A chứa $\mathfrak{a}$, thì $u$ là một đơn vị phải modulo $\mathfrak{a}$, do đó $\mathfrak{b}$ là chính quy. Vậy các iđêan trái của A cực đại và chính quy là các phần tử cực đại của tập hợp các iđêan trái thực sự chính quy của A. Hơn nữa, một iđêan trái $\mathfrak{b}$ của A chứa $\mathfrak{a}$ là thực sự khi và chỉ khi $u$ không thuộc $\mathfrak{b}$. Do đó, tập hợp các iđêan trái thực sự $\mathfrak{b}$ của A chứa $\mathfrak{a}$, có thứ tự bởi quan hệ bao hàm, là một tập quy nạp. Định lý 2 của Lý thuyết tập hợp, III, §2, No. 4, p. 154 áp dụng cho tập hợp này cho kết quả sau.

#### Mệnh đề 1 {#alg-viii-a1-prop-1 .statement tag=00P5}

Mọi iđêan trái (tương ứng phải) thực sự chính quy của A đều được chứa trong một iđêan trái (tương ứng phải) cực đại chính quy.

#### Mệnh đề 2 {#alg-viii-a1-prop-2 .statement tag=00P6}

Cho A là một $k$-đại số giao hoán. Một iđêan $\mathfrak{a}$ của A là một iđêan cực đại chính quy nếu và chỉ nếu giả vành $A/\mathfrak{a}$ (I, §8, No. 1, p. 98) là một trường.

Một phần tử $u$ của A là một đơn vị modulo $\mathfrak{a}$ (phải hoặc trái) nếu và chỉ nếu ảnh chính tắc của $u$ trong $A/\mathfrak{a}$ là một phần tử đơn vị của đại số $A/\mathfrak{a}$. Do đó, iđêan $\mathfrak{a}$ là chính quy nếu và chỉ nếu đại số $A/\mathfrak{a}$ có đơn vị. Giả sử các điều kiện này được thỏa mãn.

Ánh xạ $\mathfrak{b}\mapsto \mathfrak{b}/\mathfrak{a}$ là một song ánh từ tập hợp các iđêan của đại số A chứa $\mathfrak{a}$ tới tập hợp các iđêan của đại số $A/\mathfrak{a}$. Đây là các iđêan của vành $A/\mathfrak{a}$ vì đại số này có đơn vị. Cuối cùng, theo Định lý 1 của I, §9, No. 1, p. 115, vành $A/\mathfrak{a}$ là một trường nếu và chỉ nếu nó khác không và các iđêan duy nhất của nó là 0 và chính nó. Mệnh đề được chứng minh.

#### Ví dụ 1 {#alg-viii-a1-n1-exa-1 .statement tag=00P7}

Cho V là một không gian vectơ vô hạn chiều trên một trường giao hoán K. Gọi End$^f_K(V)$ là đại số con trên K của End$_K(V)$ gồm các tự đồng cấu có hạng hữu hạn. Cho W là một không gian con tuyến tính của V, và gọi $\mathfrak{a}_W$ là tập hợp các phần tử của End$^f_K(V)$ mà hạt nhân chứa W; đó là một iđêan trái của End$^f_K(V)$. Một phần tử $u$ của End$^f_K(V)$ là một đơn vị phải modulo $\mathfrak{a}_W$ khi và chỉ khi ta có $u(x) =x$ với mọi $x\in W$. Một phần tử như vậy $u$ tồn tại, nghĩa là, $\mathfrak{a}_W$ là chính quy, khi và chỉ khi W là hữu hạn chiều. Iđêan $\mathfrak{a}_W$ là cực đại và chính quy khi và chỉ khi W có chiều 1.

#### Ví dụ 2 {#alg-viii-a1-n1-exa-2 .statement tag=00P8}

Cho T là một không gian compact địa phương, và gọi $\mathscr{C}_0(T)$ là $\mathbf{C}$-đại số giao hoán của các ánh xạ liên tục từ T vào $\mathbf{C}$ mà tiến tới 0 ở vô cực (Gen. Top., X, §4, No. 4, p. 316); nó có đơn vị khi và chỉ khi T compact. Cho F là một tập con đóng của T, và gọi $\mathfrak{a}_F$ là tập hợp các phần tử của $\mathscr{C}_0(T)$ mà hạn chế của chúng trên F là hàm không; đó là một iđêan của $\mathscr{C}_0(T)$. Một phần tử $u$ của $\mathscr{C}_0(T)$ là một đơn vị modulo $\mathfrak{a}_F$ khi và chỉ khi ta có $u(t) = 1$ với mọi $t\in F$. Tồn tại một phần tử như vậy $u$, nghĩa là $\mathfrak{a}_F$ là chính quy, khi và chỉ khi F compact. Ánh xạ $t\mapsto \mathfrak{a}_{\{t\}}$ là một song ánh từ T lên tập hợp các iđêan cực đại chính quy của $\mathscr{C}_0(T)$ (TS, I, §3, n$^o2$, p. 32, hệ quả 1). Giả sử T không compact, và ký hiệu bởi $\mathfrak{a}$ tập con của $\mathscr{C}_0(T)$ gồm các hàm có giá compact; khi đó $\mathfrak{a}$ là một iđêan của $\mathscr{C}_0(T)$ không được chứa trong bất kỳ iđêan chính quy nào của $\mathscr{C}_0(T)$.

#### Ví dụ 3 {#alg-viii-a1-n1-exa-3 .statement tag=00P9}

Cho $L^1(\mathbf{R})$ là đại số chập của nhóm compact địa phương $\mathbf{R}$. Nhắc lại (xem Int., VIII, §4, No. 5, p. 38) rằng $L^1(\mathbf{R})$ là không gian các lớp hàm trên $\mathbf{R}$ khả tích đối với độ đo Lebesgue. Tích của các lớp của hai hàm $f$ và $g$ là lớp của hàm $f*g$ được xác định bởi công thức

$$
(f*g)(s) =\int_{-\infty}^{+\infty}f(t)g(s-t)dt
$$

với hầu khắp mọi $s\in \mathbf{R}$. Đại số $L^1(\mathbf{R})$ không có đơn vị. Với mọi $a$ trong $\mathbf{R}$, ký hiệu $\mathfrak{m}_a$ là tập hợp các phần tử $f$ của $L^1(\mathbf{R})$ thỏa mãn

$$
\int_{-\infty}^{+\infty}f(t)e^{-iat}dt= 0
$$

Theo TS, II, §3, n$^o2$, p. 252, định lý 1, ánh xạ $a\mapsto \mathfrak{m}_a$ là một song ánh từ $\mathbf{R}$ lên tập hợp các iđêan cực đại chính quy của đại số $L^1(\mathbf{R}).*$

### 2. Phép nối một phần tử đơn vị

Cho A là một $k$-đại số. Trong III, §1, No. 2, p. 431, chúng ta đã định nghĩa đại số có đơn vị $\widetilde{A}$ suy ra từ A bằng phép nối một phần tử đơn vị $e$. Ta đồng nhất A với một iđêan hai phía của $\widetilde{A}$. $k$-môđun $\widetilde{A}$ là tổng trực tiếp của các môđun con $ke$ và A.

#### Mệnh đề 3 {#alg-viii-a1-prop-3 .statement tag=00PA}

a) Cho $\widetilde{\mathfrak{a}}$ là một iđêan trái của $\widetilde{A}$ sao cho $\widetilde{A} =\widetilde{\mathfrak{a}}+ A$. Ta đặt $\mathfrak{a}=\widetilde{\mathfrak{a}}\cap A$. Tồn tại một phần tử $u$ của A sao cho $u-e$ thuộc $\widetilde{\mathfrak{a}}$. Nếu $u$ là một phần tử như vậy, thì nó là một phần tử khả nghịch phải của A modulo $\mathfrak{a}$, và ta có $\widetilde{\mathfrak{a}}=\mathfrak{a}+k(u-e)$; đặc biệt, iđêan $\mathfrak{a}$ là chính quy.

b) Ngược lại, cho $\mathfrak{a}$ là một iđêan trái chính quy của A và $u$ là một phần tử khả nghịch phải của A modulo $\mathfrak{a}$. Đặt $\widetilde{\mathfrak{a}}=\mathfrak{a}+k(u-e)$. Khi đó $\widetilde{\mathfrak{a}}$ là một iđêan trái của $\widetilde{A}$ sao cho $\widetilde{A} =\widetilde{\mathfrak{a}}+ A$, và ta có $\mathfrak{a}=\widetilde{\mathfrak{a}}\cap A$.

c) Nếu $k$ là một trường, thì điều kiện $\widetilde{A} =\widetilde{\mathfrak{a}}+ A$ tương đương với việc nói rằng $\widetilde{\mathfrak{a}}$ không được chứa trong A.

Dưới giả thiết của a), phần tử $e$ của $\widetilde{A}$ có thể được viết thành $(e-u)+u$ với $u\in A$ và $u-e\in \widetilde{\mathfrak{a}}$. Đặt $x=\lambda e+a$ là một phần tử của $\widetilde{A}$, trong đó $\lambda \in k$ và $a\in A$; nếu $x$ thuộc $\widetilde{\mathfrak{a}}$, thì phần tử $y=a+\lambda u=x+\lambda (u-e)$ của A thuộc $\mathfrak{a}$, và ta có $x=y-\lambda (u-e)$; điều này chứng minh đẳng thức $\widetilde{\mathfrak{a}}=\mathfrak{a}+k(u-e)$. Hơn nữa, với mọi $a$ trong A, phần tử $au-a=a(u-e)$ của A thuộc $\mathfrak{a}$, nên $u$ là một đơn vị phải modulo $\mathfrak{a}$. Điều này chứng minh mệnh đề a).

Cho $\mathfrak{a}$ và $u$ như trong b). Vì $\widetilde{A}$ là tổng trực tiếp của A và $k(u-e)$, ta có $\widetilde{\mathfrak{a}}+ A =\widetilde{A}$ và $\widetilde{\mathfrak{a}}\cap A =\mathfrak{a}$. Mọi phần tử của $\widetilde{\mathfrak{a}}$ đều có dạng $x+\lambda (u-e)$ với $x\in \mathfrak{a}$ và $\lambda \in k$. Với mọi $a\in A$, ta có

$$
a(x+\lambda (u-e)) =ax+\lambda (au-a)
$$

Vì $u$ là một phần tử khả nghịch phải của A modulo $\mathfrak{a}$, tổng $ax+\lambda (au-a)$ thuộc $\mathfrak{a}$, do đó $\widetilde{\mathfrak{a}}$ là một iđêan trái của A. Điều này chứng minh b).

Cuối cùng, nếu $k$ là một trường, thì A là một siêu phẳng trong $\widetilde{A}$, và $\widetilde{A}$ là tổng của $\widetilde{\mathfrak{a}}$ và A khi và chỉ khi $\widetilde{\mathfrak{a}}$ không được chứa trong A.

#### Hệ quả {#alg-viii-a1-n2-cor-1 .statement tag=00PB}

Các iđêan chính quy trái của A là các iđêan có dạng $A\cap \widetilde{\mathfrak{a}}$, trong đó $\widetilde{\mathfrak{a}}$ là một iđêan trái của $\widetilde{A}$ sao cho $\widetilde{A} =\widetilde{\mathfrak{a}}+ A$.

#### Mệnh đề 4 {#alg-viii-a1-prop-4 .statement tag=00PC}

a) Cho $\mathfrak{a}$ là một iđêan trái cực đại chính quy của A. Tồn tại một iđêan trái duy nhất $\widetilde{\mathfrak{a}}$ của $\widetilde{A}$ sao cho $\widetilde{A} =\widetilde{\mathfrak{a}}+ A$ và $\mathfrak{a}=\widetilde{\mathfrak{a}}\cap A$. Iđêan này là cực đại và không chứa A.

b) Ánh xạ $\widetilde{\mathfrak{a}}\mapsto \widetilde{\mathfrak{a}}\cap A$ là một song ánh từ tập hợp các iđêan trái cực đại của $\widetilde{A}$ không chứa A lên tập hợp các iđêan trái cực đại chính quy của A.

Cho $\mathfrak{a}$ là một iđêan trái cực đại chính quy của A. Theo Mệnh đề 3, a), các iđêan trái $\mathfrak{b}$ của $\widetilde{A}$ sao cho $\mathfrak{b}+ A =\widetilde{A}$ và $\mathfrak{b}\cap A =\mathfrak{a}$ là các iđêan $\mathfrak{a}+k(u-e)$, trong đó $u$ là một đơn vị phải modulo $\mathfrak{a}$. Do đó, để chứng minh tính duy nhất của $\widetilde{\mathfrak{a}}$, chỉ cần chứng minh rằng hai đơn vị phải $u$ và $u'$ của A modulo $\mathfrak{a}$ là đồng dư modulo $\mathfrak{a}$. Lập luận phản chứng, giả sử rằng $u-u'$ không thuộc $\mathfrak{a}$. Công thức $x(u-u') = (xu-x)-(xu'-x)$ cho thấy rằng ta có $A(u-u')\subset \mathfrak{a}$; suy ra $\mathfrak{a}+k(u-u')$ là một iđêan trái của A chứa $\mathfrak{a}$ và phân biệt với $\mathfrak{a}$. Vì $\mathfrak{a}$ là cực đại, do đó ta có $\mathfrak{a}+k(u-u') = A$, và do đó AA $\subset \mathfrak{a}$. Với mọi $x\in A$, ta có $x\equiv xu$ (mod $\mathfrak{a}$), và do đó $x\in \mathfrak{a}$ theo điều trên, mâu thuẫn với giả thiết $\mathfrak{a}\not= A$.

Do đó tồn tại một iđêan trái duy nhất $\widetilde{\mathfrak{a}}$ của $\widetilde{A}$ sao cho $\widetilde{A} =\widetilde{\mathfrak{a}}+ A$ và $\mathfrak{a}=\widetilde{\mathfrak{a}}\cap A$. Cho $\mathfrak{b}$ là một iđêan trái thực sự của $\widetilde{A}$ chứa $\widetilde{\mathfrak{a}}$. Khi đó $\mathfrak{b}\cap A$ là một iđêan trái thực sự của A chứa $\mathfrak{a}$. Vậy nó bằng $\mathfrak{a}$ vì $\mathfrak{a}$ là cực đại, điều này kéo theo $\mathfrak{b}=\widetilde{\mathfrak{a}}$ theo Bổ đề 2 của VIII, p. 4. Điều này chứng minh rằng $\widetilde{\mathfrak{a}}$ là một iđêan cực đại của $\widetilde{A}$; đối với một iđêan như thế, điều kiện $\widetilde{A} =\widetilde{\mathfrak{a}}+ A$ có nghĩa là $\widetilde{\mathfrak{a}}$ không chứa A.

Còn phải chứng minh rằng nếu $\widetilde{\mathfrak{a}}$ là một iđêan trái cực đại của $\widetilde{A}$ không chứa A, thì iđêan trái $\mathfrak{a}= A\cap \widetilde{\mathfrak{a}}$ của A là cực đại. Cho $\mathfrak{b}$ là một iđêan trái thực sự của A chứa $\mathfrak{a}$. Gọi $u$ là một đơn vị phải modulo $\mathfrak{a}$ sao cho $\widetilde{\mathfrak{a}}=\mathfrak{a}+k(u-e)$ (Mệnh đề 3). Nó cũng là một đơn vị phải modulo $\mathfrak{b}$; ký hiệu bởi $\widetilde{\mathfrak{b}}$ iđêan $\mathfrak{b}+k(u-e)$ của $\widetilde{A}$. Theo Mệnh đề 3, b), ta có $\mathfrak{b}= A\cap \widetilde{\mathfrak{b}}$. Iđêan $\widetilde{\mathfrak{a}}$, bằng $\mathfrak{a}+k(u-e)$, được chứa trong $\widetilde{\mathfrak{b}}$ và do đó bằng $\widetilde{\mathfrak{b}}$ vì $\widetilde{\mathfrak{b}}$ phân biệt với $\widetilde{A}$ và $\widetilde{\mathfrak{a}}$ là cực đại. Do đó, ta có $\mathfrak{a}=\mathfrak{b}$, và $\mathfrak{a}$ là cực đại.

Chúng tôi để độc giả chuyển Mệnh đề 3 và 4 sang các iđêan phải.

### 3. Căn của một đại số

Cho A là một $k$-đại số. Một môđun giả trái trên A là một $k$-môđun M được trang bị cấu trúc môđun giả trái trên giả vành A (II, Phụ lục, No. 2, p. 378) sao cho ta có $a(\lambda x) =\lambda (ax) = (\lambda a)x$ với $\lambda \in k$, $a\in A$, và $x\in M$. Ta cũng định nghĩa tương tự các môđun giả phải trên A.

Cho M là một môđun giả trái trên A; ta định nghĩa trên M một cấu trúc $\widetilde{A}$-môđun trái gọi là chính tắc bằng cách đặt

$(\lambda e+a)x=\lambda x+ax$ với $\lambda \in k, a\in A, x\in M$.

Ngược lại, mọi $\widetilde{A}$-môđun trái đều được trang bị một cách chính tắc, bằng cách hạn chế vành các toán tử vào $k$ và A, cấu trúc môđun giả trái trên A. Do đó, các loài cấu trúc của các môđun giả trái trên A và của các môđun trên $\widetilde{A}$ là tương đương (Lý thuyết Tập hợp, IV, §1, No. 7, p. 262).

Cho M là một môđun giả trái trên A, và cho N là một môđun con $k$ của M. Khi đó N là một môđun con $\widetilde{A}$ của M nếu và chỉ nếu nó ổn định dưới tác động của A; khi đó ta nói rằng N là một môđun giả con của M.

Như trong trường hợp các vành, ta định nghĩa giả môđun trái $A_s$ trên A và giả môđun phải $A_d$. Các iđêan trái (tương ứng, phải) của A là các môđun giả con của $A_s$ (tương ứng, $A_d$).

Cho $\mathfrak{a}$ là một iđêan trái chính quy của A và $u$ là một đơn vị phải modulo $\mathfrak{a}$. Đặt $M = A_s/\mathfrak{a}$, và ký hiệu ảnh của $u$ trong M là $z$. Ta có $M = Az$, và $\mathfrak{a}$ là linh hóa tử của $z$.

Ngược lại, cho M là một môđun giả trái trên A, và cho $z$ là một phần tử của M sao cho $M = Az$. Khi đó tồn tại một phần tử $u$ của A sao cho $z=uz$. Với mọi $a\in A$, ta có $(au-a)z= 0$, nên $au-a$ thuộc linh hóa tử $\mathfrak{a}$ của $z$. Do đó, $\mathfrak{a}$ là một iđêan trái chính quy của A, phần tử $u$ là một đơn vị phải modulo $\mathfrak{a}$, và khi chuyển qua thương, ánh xạ $a\mapsto az$ xác định một đẳng cấu từ $A_s/\mathfrak{a}$ lên M.

#### Định nghĩa 2 {#alg-viii-a1-def-2 .statement tag=00PD}

Ta nói rằng một giả môđun M trên A là đơn nếu ta có AM $\not= 0$ và nếu 0 và M là hai môđun giả con duy nhất của M.

Điều này tương ứng với việc nói rằng $\widetilde{A}$-môđun M là đơn và linh hóa tử của nó không chứa A. Khi A là một vành và M là một A-môđun, ta có AM = M, do đó Định nghĩa 2 trùng với Định nghĩa 1 của VIII, p. 45.

#### Mệnh đề 5 {#alg-viii-a1-prop-5 .statement tag=00PE}

a) Cho $\mathfrak{m}$ là một iđêan trái cực đại chính quy của A. Khi đó giả môđun $A_s/\mathfrak{m}$ là đơn, và tồn tại một phần tử khác không của $A_s/\mathfrak{m}$ có linh hóa tử là $\mathfrak{m}$.

b) Cho M là một giả môđun đơn, và cho $x$ là một phần tử khác không của M. Ta có $M = Ax$, linh hóa tử $\mathfrak{m}$ của $x$ là một iđêan trái cực đại chính quy của A, và khi chuyển qua thương, ánh xạ $a\mapsto ax$ xác định một đẳng cấu từ $A_s/\mathfrak{m}$ lên M.

c) Cho M là một giả môđun không thu về 0. Khi đó M là đơn nếu và chỉ nếu ta có $M = Ax$ với mọi phần tử khác không $x$ của M.

Cho $\mathfrak{m}$ là một iđêan trái cực đại chính quy của A. Ta đã thấy rằng tồn tại một phần tử khác không $z$ của $A_s/\mathfrak{m}$ có linh hóa tử bằng $\mathfrak{m}$ và sao cho $Az= A_s/\mathfrak{m}$; đặc biệt, ta có $A(A_s/\mathfrak{m})\not= 0$. Hơn nữa, mọi môđun giả con của $A_s/\mathfrak{m}$ đều có dạng $\mathfrak{n}/\mathfrak{m}$, trong đó $\mathfrak{n}$ là một iđêan trái của A chứa $\mathfrak{m}$. Vì $\mathfrak{m}$ là cực đại, các khả năng duy nhất là $\mathfrak{n}=\mathfrak{m}$ và $\mathfrak{n}= A$, do đó giả môđun $A_s/\mathfrak{a}$ là đơn. Điều này chứng minh a).

Dưới các giả thiết của b), tập hợp các phần tử $y$ của M sao cho $Ay= 0$ là một giả môđun con của M khác với M và do đó bằng 0. Do đó, $Ax$ là một giả môđun con khác không của M, điều này kéo theo $M = Ax$. Khi đó mệnh đề b) suy ra từ các nhận xét trước Định nghĩa 2.

Cho M là một giả môđun khác không. Giả sử rằng ta có $Ax= M$ đối với mọi phần tử khác không $x$ của M. Đặc biệt, ta có AM $\not= 0$. Cho N là một giả môđun con khác không của M, và $x$ là một phần tử khác không của N. Ta có $Ax= M$, và do đó N = M. Vậy M là đơn. Ngược lại, nếu M là đơn, thì ta có $M = Ax$ đối với mọi $x\not= 0$ theo b).

#### Định nghĩa 3 {#alg-viii-a1-def-3 .statement tag=00RT}

Căn của $k$-đại số A, ký hiệu là $\Re (A)$, là giao của các iđêan trái cực đại chính quy của A.

Khi A là một vành, mọi iđêan trái của A đều chính quy, nên định nghĩa của căn trùng với Định nghĩa 2 của VIII, p. 154.

#### Ví dụ 1 {#alg-viii-a1-n3-exa-1 .statement tag=00PF}

Căn của $k$-đại số End$^f_k(V)$ thu về 0 (VIII, p. 436, Ví dụ 1)$.*$ Điều tương tự cũng đúng với các đại số $\mathscr{C}_0(T)$ và $L^1(\mathbf{R}).*$

#### Ví dụ 2 {#alg-viii-a1-n3-exa-2 .statement tag=00PG}

Cho A là một giả vành trong đó mọi phần tử đều lũy linh. Căn của A bằng A vì A là iđêan trái chính quy duy nhất.

Mệnh đề 5 ngay lập tức kéo theo kết quả sau đây.

#### Mệnh đề 6 {#alg-viii-a1-prop-6 .statement tag=00PH}

Căn của đại số A là giao của các linh hóa tử của các giả môđun đơn. Đặc biệt, nó là một iđêan hai phía của A.

#### Mệnh đề 7 {#alg-viii-a1-prop-7 .statement tag=00PI}

Căn của A là vết trên A của căn của $\widetilde{A}$; nó cũng bằng căn của đại số đối $A^o($nghĩa là, bằng giao của các iđêan phải cực đại chính quy của A). Nếu vành $k$ không có căn, thì căn của A bằng căn của $\widetilde{A}$.

Đẳng thức $\Re (\widetilde{A})\cap A =\Re (A)$ suy ra từ Mệnh đề 4 của VIII, p. 438, b). Vì $\widetilde{A}$ và $\widetilde{A}^o$ có cùng căn (VIII, p. 156, Hệ quả 1), nên suy ra đẳng thức $\Re (A) =\Re (A^o)$. Nếu $k$ không có căn, thì giao của các iđêan trái cực đại của $\widetilde{A}$ chứa A thì bằng A. Do đó $\Re (\widetilde{A})$ được chứa trong A và vì thế bằng $\Re (A)$.

#### Nhận xét {#alg-viii-a1-n3-rem-1 .statement tag=00PJ}

Cho $x$ và $y$ là các phần tử của A; ta nói rằng $x$ là một đối nghịch trái của $y$, hoặc rằng $y$ là một đối nghịch phải của $x$, nếu, trong $\widetilde{A},x-e$ là một nghịch đảo trái của $y-e$, nghĩa là nếu ta có $x+y=xy$. Theo Mệnh đề 7 và định lý của Jacobson (VIII, p. 156, Định lý 1), căn của A gồm các phần tử $x$ của A sao cho $ux-e$ là khả nghịch trái trong $\widetilde{A}$ với mọi $u$ trong $\widetilde{A}$. Vì ta có $(a+\lambda e)x-e=ax+\lambda x-e$ (với $a\in A,\lambda \in k$), căn của A là tập hợp các phần tử $x$ của A sao cho $ax+\lambda x$ có một đối nghịch trái trong A với mọi $a\in A$ và $\lambda \in k$.

### 4. Định lý mật độ

Cho A là một $k$-đại số. Một môđun giả trái M được gọi là nửa đơn nếu nó là tổng trực tiếp của một họ các môđun giả trái đơn.

#### Bổ đề 1 {#alg-viii-a1-lem-1 .statement tag=00PK}

Cho M là một môđun giả trái A nửa đơn. Cho B là đối giao hoán tử kép của $\widetilde{A}$-môđun M. Khi đó mọi môđun giả con A của M đều là một B-môđun con của M.

$\widetilde{A}$-môđun M là nửa đơn. Cho N là một môđun giả con A của M. Khi đó N là một $\widetilde{A}$-môđun con của M. Theo Hệ quả 2 của VIII, p. 56, tồn tại một phép chiếu $p$ của A-môđun M có ảnh là N. Vì ta có quan hệ $pb=bp$ với mọi $b\in B$, suy ra N là một B-môđun con của M.

#### Bổ đề 2 {#alg-viii-a1-lem-2 .statement tag=00PL}

Cho M là một môđun giả trái A nửa đơn, và cho $x$ là một phần tử của M. Tồn tại một phần tử $a\in A$ sao cho $ax=x$.

Cho N là giả môđun A trái $\widetilde{A}x/Ax$. N thỏa mãn AN $=\{0\}$. Theo Hệ quả 3 của VIII, p. 56 áp dụng cho các $\widetilde{A}$-môđun M và $\widetilde{A}x$, giả môđun A N là nửa đơn. Theo định nghĩa, mọi giả môđun con đơn S của N đều thỏa mãn AS $\not=\{0\}$. Do đó giả môđun N là không, và suy ra $x\in Ax$.

#### Định lý 1 (định lý mật độ của Jacobson) {#alg-viii-a1-thm-1 .statement tag=00SD}

Cho M là một giả môđun A trái nửa đơn. Cho $b$ là một phần tử của đối giao hoán tử kép của $\widetilde{A}$-môđun M. Cho $F =\{x_1, . . . , x_n\}$ là một tập con hữu hạn của M. Khi đó tồn tại một phần tử $a\in A$ sao cho $bx_i=ax_i$ với mọi $i\in [1, n]$.

Cho B là đối giao hoán tử kép của $\widetilde{A}$-môđun M. Giả môđun A $M^n$ là nửa đơn. Cho $\boldsymbol{x}= (x_1, . . . , x_n)\in M^n$. Từ Bổ đề 2 suy ra rằng $\boldsymbol{x}\in$ $A\boldsymbol{x}$. Đối giao hoán tử kép của $\widetilde{A}$-môđun $M^n$ trùng với các vị tự của B-môđun $M^n$ (VIII, p. 79, Mệnh đề 2). Theo Bổ đề 1, môđun giả con A $A\boldsymbol{x}$ của $M^n$ do đó là một B-môđun con của $M^n$. Vì vậy ta có bao hàm $B\boldsymbol{x}\subset A\boldsymbol{x}$. Do đó tồn tại một $a\in A$ sao cho $b\boldsymbol{x}=a\boldsymbol{x}$. Kết quả suy ra.

### Bài tập {#alg-viii-a1-exercises}

Xem [các bài tập cho Phụ lục 1](exercises/a1/).
