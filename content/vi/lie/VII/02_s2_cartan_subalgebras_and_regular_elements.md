---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: VII
chapter_title: CARTAN SUBALGEBRAS AND REGULAR ELEMENTS
section: 2
section_title: Cartan subalgebras and regular elements of a Lie algebra
lang: vi
source: lie-vii-ix
book_pages: 12-20, 55-57
pdf_pages: 0022-0030, 0064-0066
extraction: native
subsections:
    - "no": 1
      title: CARTAN SUBALGEBRAS
      page: 13
      pdf_page: 23
    - "no": 2
      title: REGULAR ELEMENTS OF A LIE ALGEBRA
      page: 16
      pdf_page: 26
    - "no": 3
      title: CARTAN SUBALGEBRAS AND REGULAR ELEMENTS
      page: 18
      pdf_page: 28
    - "no": 4
      title: CARTAN SUBALGEBRAS OF SEMI-SIMPLE LIE ALGEBRAS
      page: 19
      pdf_page: 29
statements: 40
exercises: 16
content_sha256: ab1c9e112a8b7b9550e84ed45e89e2805d86c9a0e208a591abfd3569d6977857
translated_from: content/en/lie/VII/02_s2_cartan_subalgebras_and_regular_elements.md
source_content_sha256: cd216f4473ca42ded2206eb6bb0c4659b8f54dd4567c37dde5e1e1476691ef01
translation_model: gpt-5.4
translation_run: translate-vi-ee98954a
glossary_version: 34
glossary_terms_sha256: e474a3323d98841482a7adf0f23450f199d4258d34758896e0df75330e8a1587
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 2. CÁC ĐẠI SỐ CON CARTAN VÀ CÁC PHẦN TỬ CHÍNH QUY CỦA MỘT ĐẠI SỐ LIE

Từ no. 2 trở đi, trường $k$ được giả thiết là vô hạn.

### 1. CÁC ĐẠI SỐ CON CARTAN

#### Định nghĩa 1 {#lie-vii-s2-def-1 .statement tag=00TJ}

Cho $\mathfrak{g}$ là một đại số Lie. Một đại số con Cartan của $\mathfrak{g}$ là một đại số con lũy linh của $\mathfrak{g}$ bằng với chuẩn hóa tử của chính nó.

Sau này chúng ta sẽ thu được các kết quả sau:

1) nếu $k$ là vô hạn, $\mathfrak{g}$ có các đại số con Cartan (no. 3, Hệ quả 1 của Định lý 1);

2) nếu $k$ có đặc số không, mọi đại số con Cartan của $\mathfrak{g}$ đều có cùng chiều (§3, no. 3, Định lý 2);

3) nếu $k$ đóng đại số và có đặc số 0, mọi đại số con Cartan của $\mathfrak{g}$ đều liên hợp dưới nhóm các tự đẳng cấu sơ cấp của $\mathfrak{g}($§3, no. 2, Định lý 1).

#### Ví dụ 1 {#lie-vii-s2-n1-exa-1 .statement tag=00TK}

Nếu $\mathfrak{g}$ lũy linh, đại số con Cartan duy nhất của $\mathfrak{g}$ là chính $\mathfrak{g}$ (Chap. I, §4, no. 1, Mệnh đề 3).

#### Ví dụ 2 {#lie-vii-s2-n1-exa-2 .statement tag=00TL}

Cho $\mathfrak{g}=\mathfrak{g}\mathfrak{l}(n, k)$, và gọi $\mathfrak{h}$ là tập hợp các ma trận đường chéo thuộc $\mathfrak{g}$. Ta chứng minh rằng $\mathfrak{h}$ là một đại số con Cartan của $\mathfrak{g}$. Trước hết, $\mathfrak{h}$ là giao hoán, do đó lũy linh. Gọi $(E_{ij})$ là cơ sở chính tắc của $\mathfrak{g}\mathfrak{l}(n, k)$, và gọi $x=\sum\mu_{ij}E_{ij}$ là một phần tử của chuẩn hóa tử của $\mathfrak{h}$ trong $\mathfrak{g}$. Nếu $i\not=j$, các công thức (5) của Chương I, §1, no. 2 cho thấy rằng hệ số của $E_{ij}$ trong $[E_{ii}, x]$ là $\mu_{ij}$. Vì $E_{ii}\in \mathfrak{h}$, nên $[E_{ii}, x]\in \mathfrak{h}$, và hệ số đang xét bằng không. Do đó $\mu_{ij}= 0$ với $i\not=j$, suy ra $x\in \mathfrak{h}$, điều này cho thấy rằng $\mathfrak{h}$ quả thật là một đại số con Cartan của $\mathfrak{g}$.

#### Ví dụ 3 {#lie-vii-s2-n1-exa-3 .statement tag=00TM}

Cho $\mathfrak{h}$ là một đại số con Cartan của $\mathfrak{g}$ và cho $\mathfrak{g}_1$ là một đại số con của $\mathfrak{g}$ chứa $\mathfrak{h}$. Khi đó $\mathfrak{h}$ là một đại số con Cartan của $\mathfrak{g}_1$; điều này suy ra ngay lập tức từ Định nghĩa 1.

#### Mệnh đề 1 {#lie-vii-s2-prop-1 .statement tag=00TN}

Cho $\mathfrak{g}$ là một đại số Lie và cho $\mathfrak{h}$ là một đại số con Cartan của $\mathfrak{g}$. Khi đó $\mathfrak{h}$ là một đại số con lũy linh cực đại của $\mathfrak{g}$.

Cho $\mathfrak{h}'$ là một đại số con lũy linh của $\mathfrak{g}$ chứa $\mathfrak{h}$. Khi đó $\mathfrak{h}$ là một đại số con Cartan của $\mathfrak{h}'$ (Ví dụ 3), nên $\mathfrak{h}=\mathfrak{h}'$ (Ví dụ 1).

Có những đại số con lũy linh cực đại không phải là các đại số con Cartan (Bài tập 2).

#### Mệnh đề 2 {#lie-vii-s2-prop-2 .statement tag=00TO}

Cho $(\mathfrak{g}_i)_{i\in I}$ là một họ hữu hạn các đại số Lie và $\mathfrak{g}=\prod_{i\in I}\mathfrak{g}_i$.

Các đại số con Cartan của $\mathfrak{g}$ là các đại số con có dạng $\prod_{i\in I}\mathfrak{h}_i$, trong đó $\mathfrak{h}_i$

là một đại số con Cartan của $\mathfrak{g}_i$.

Nếu $\mathfrak{h}_i$ là một đại số con của $\mathfrak{g}_i$ với chuẩn hóa tử $\mathfrak{n}_i$, thì $\prod\mathfrak{h}_i$ là một đại số con của $\mathfrak{g}$ với chuẩn hóa tử $\prod\mathfrak{n}_i$; nếu các $\mathfrak{h}_i$ lũy linh, thì $\prod\mathfrak{h}_i$ lũy linh; do đó, nếu $\mathfrak{h}_i$ là một đại số con Cartan của $\mathfrak{g}_i$ với mọi $i,\prod\mathfrak{h}_i$ là một đại số con Cartan của $\mathfrak{g}$. Ngược lại, giả sử $\mathfrak{h}$ là một đại số con Cartan của $\mathfrak{g}$; phép chiếu $\mathfrak{h}_i$ của $\mathfrak{h}$ lên $\mathfrak{g}_i$ là một đại số con lũy linh của $\mathfrak{g}_i$, và $\prod\mathfrak{h}_i$ là một đại số con lũy linh của $\mathfrak{g}$ chứa $\mathfrak{h}$; do đó $\mathfrak{h}=\prod\mathfrak{h}_i$ (Mệnh đề 1); vậy, với mọi $i,\mathfrak{h}_i$ là chuẩn hóa tử của chính nó trong $\mathfrak{g}_i$, và vì thế là một đại số con Cartan của $\mathfrak{g}_i$.

#### Ví dụ 4 {#lie-vii-s2-n1-exa-4 .statement tag=00TP}

Nếu $k$ có đặc số $0,\mathfrak{g}\mathfrak{l}(n, k)$ là tích của các iđêan $\mathfrak{s}\mathfrak{l}(n, k)$ và $k.1$. Suy ra từ Ví dụ 2 và Mệnh đề 2 rằng tập hợp các ma trận đường chéo có vết bằng 0 trong $\mathfrak{s}\mathfrak{l}(n, k)$ là một đại số con Cartan của $\mathfrak{s}\mathfrak{l}(n, k)$.

#### Mệnh đề 3 {#lie-vii-s2-prop-3 .statement tag=00TQ}

Cho $\mathfrak{g}$ là một đại số Lie, $\mathfrak{h}$ một đại số con của $\mathfrak{g}$, và $k'$ là một mở rộng của $k$. Khi đó $\mathfrak{h}$ là một đại số con Cartan của $\mathfrak{g}$ nếu và chỉ nếu $\mathfrak{h}\otimes_kk'$ là một đại số con Cartan của $\mathfrak{g}\otimes_kk'$.

Thật vậy, $\mathfrak{h}$ là lũy linh nếu và chỉ nếu $\mathfrak{h}\otimes_kk'$ là lũy linh (Chương I, §4, no. 5). Mặt khác, nếu $\mathfrak{n}$ là bộ chuẩn hóa của $\mathfrak{h}$ trong $\mathfrak{g}$, thì bộ chuẩn hóa của $\mathfrak{h}\otimes_kk'$ trong $\mathfrak{g}\otimes_kk'$ là $\mathfrak{n}\otimes_kk'$ (Chương I, §3, no. 8).

#### Mệnh đề 4 {#lie-vii-s2-prop-4 .statement tag=00TR}

Cho $\mathfrak{g}$ là một đại số Lie, $\mathfrak{h}$ là một đại số con lũy linh của $\mathfrak{g}$. Khi đó $\mathfrak{h}$ là một đại số con Cartan của $\mathfrak{g}$ nếu và chỉ nếu $\mathfrak{g}^0(\mathfrak{h}) =\mathfrak{h}$.

Nếu $\mathfrak{g}^0(\mathfrak{h}) =\mathfrak{h},\mathfrak{h}$ là bộ chuẩn hoá của chính nó (§1, Mệnh đề 10 (i)), do đó $\mathfrak{h}$ là một đại số con Cartan của $\mathfrak{g}$. Giả sử rằng $\mathfrak{g}^0(\mathfrak{h})\not=\mathfrak{h}$. Xét biểu diễn của $\mathfrak{h}$ trên $\mathfrak{g}^0(\mathfrak{h})/\mathfrak{h}$ thu được từ biểu diễn phụ hợp bằng cách chuyển sang thương. Áp dụng định lý Engel (Chương I, §4, no. 2, Định lý 1), ta thấy tồn tại $x\in \mathfrak{g}^0(\mathfrak{h})$ sao cho $x \notin \mathfrak{h}$ và $[\mathfrak{h}, x]\subset \mathfrak{h}$; khi đó $x$ thuộc bộ chuẩn hoá của $\mathfrak{h}$ trong $\mathfrak{g}$, do đó $\mathfrak{h}$ không phải là một đại số con Cartan của $\mathfrak{g}$.

#### Hệ quả 1 {#lie-vii-s2-prop-4-cor-1 .statement tag=00TS}

Cho $\mathfrak{g}$ là một đại số Lie, $\mathfrak{h}$ là một đại số con Cartan của $\mathfrak{g}$. Nếu $k$ là vô hạn, tồn tại $x\in \mathfrak{h}$ sao cho $\mathfrak{h}=\mathfrak{g}^0(x)$.

Thật vậy, $\mathfrak{h}=\mathfrak{g}^0(\mathfrak{h})$ và ta có thể áp dụng Mệnh đề 9 (ii) của §1.

#### Hệ quả 2 {#lie-vii-s2-prop-4-cor-2 .statement tag=00TT}

Cho $f:\mathfrak{g}\rightarrow \mathfrak{g}'$ là một đồng cấu toàn ánh của các đại số Lie. Nếu $\mathfrak{h}$ là một đại số con Cartan của $\mathfrak{g},f(\mathfrak{h})$ là một đại số con Cartan của $\mathfrak{g}'$.

Thật vậy, $f(\mathfrak{h})$ là một đại số con lũy linh của $\mathfrak{g}'$. Mặt khác, xét biểu diễn $x \rightarrow$ ad $f(x)$ của $\mathfrak{h}$ trên $\mathfrak{g}'$. Theo Mệnh đề 9 (iv) của §1, no. 3, $f(\mathfrak{g}^0(\mathfrak{h})) ={\mathfrak{g}'}^0(\mathfrak{h})$. Mà $\mathfrak{g}^0(\mathfrak{h}) =\mathfrak{h}$, và mặt khác hiển nhiên rằng ${\mathfrak{g}'}^0(\mathfrak{h}) ={\mathfrak{g}'}^0(f(\mathfrak{h}))$. Do đó, $f(\mathfrak{h}) ={\mathfrak{g}'}^0(f(\mathfrak{h}))$ và chỉ cần áp dụng Mệnh đề 4.

#### Hệ quả 3 {#lie-vii-s2-prop-4-cor-3 .statement tag=00TU}

Cho $\mathfrak{h}$ là một đại số con Cartan của một đại số Lie $\mathfrak{g}$, và cho $\mathscr{C}^n\mathfrak{g}(n\geq 1)$ là một số hạng của chuỗi trung tâm giảm của $\mathfrak{g}$ (Chap. I, §1, no. 5). Khi đó $\mathfrak{g}=\mathfrak{h}+\mathscr{C}^n\mathfrak{g}$.

Thật vậy, Hệ quả 2 cho thấy rằng ảnh của $\mathfrak{h}$ trong $\mathfrak{g}/\mathscr{C}^n\mathfrak{g}$ là một đại số con Cartan của $\mathfrak{g}/\mathscr{C}^n\mathfrak{g}$, do đó bằng $\mathfrak{g}/\mathscr{C}^n\mathfrak{g}$ vì $\mathfrak{g}/\mathscr{C}^n\mathfrak{g}$ là lũy linh (Ví dụ 1).

#### Hệ quả 4 {#lie-vii-s2-prop-4-cor-4 .statement tag=00TV}

Cho $\mathfrak{g}$ là một đại số Lie, $\mathfrak{h}$ là một đại số con Cartan của $\mathfrak{g}$, và $\mathfrak{a}$ là một đại số con của $\mathfrak{g}$ chứa $\mathfrak{h}$.

(i) $\mathfrak{a}$ bằng chuẩn hóa tử của chính nó trong $\mathfrak{g}$.

(ii) Giả sử rằng $k=\mathbf{R}$ hoặc $\mathbf{C}$; cho G là một nhóm Lie có đại số Lie $\mathfrak{g}$, A là nhóm con nguyên của G có đại số Lie $\mathfrak{a}$. Khi đó A là một nhóm con Lie của G, và nó là thành phần đơn vị của chuẩn hóa tử của A trong G.

Gọi $\mathfrak{n}$ là chuẩn hóa tử của $\mathfrak{a}$ trong $\mathfrak{g}$. Vì $\mathfrak{h}$ là một đại số con Cartan của $\mathfrak{n}$ (Ví dụ $3$)$,\{0\}$ là một đại số con Cartan của $\mathfrak{n}/\mathfrak{a}$ (Hệ quả 2), nên bằng với chuẩn hóa tử của nó trong $\mathfrak{n}/\mathfrak{a}$; nói cách khác, $\mathfrak{n}=\mathfrak{a}$. Mệnh đề (ii) suy ra từ (i) và Chương III, §9, no. 4, Hệ quả của Mệnh đề 11.

#### Hệ quả 5 {#lie-vii-s2-prop-4-cor-5 .statement tag=00TW}

Cho $\mathfrak{g}$ là một đại số Lie, E là một tập con của $\mathfrak{g}$. Cho E tác động lên $\mathfrak{g}$ bởi biểu diễn liên hợp. Khi đó E là một đại số con Cartan của $\mathfrak{g}$ nếu và chỉ nếu $E =\mathfrak{g}^0(E)$.

Điều kiện ấy là cần thiết (Mệnh đề 4). Bây giờ giả sử rằng $E =\mathfrak{g}^0(E)$. Theo Mệnh đề 2 (ii) của §1, no. 1, khi đó E là một đại số con của $\mathfrak{g}$. Nếu $x\in E$, ad$_Ex$ là lũy linh vì $E\subset \mathfrak{g}^0(E)$; do đó đại số E là lũy linh. Nhưng khi đó E là một đại số con Cartan theo Mệnh đề 4.

#### Hệ quả 6 {#lie-vii-s2-prop-4-cor-6 .statement tag=00TX}

Cho $\mathfrak{g}$ là một đại số Lie, cho $k_0$ là một trường con của $k$ sao cho $[k:k_0]<+\infty$, và cho $\mathfrak{g}_0$ là đại số Lie thu được từ $\mathfrak{g}$ bằng cách hạn chế trường vô hướng xuống $k_0$. Cho $\mathfrak{h}$ là một tập con của $\mathfrak{g}$. Khi đó $\mathfrak{h}$ là một đại số con Cartan của $\mathfrak{g}$ nếu và chỉ nếu $\mathfrak{h}$ là một đại số con Cartan của $\mathfrak{g}_0$.

Điều này suy ra từ Hệ quả 5, vì điều kiện $\mathfrak{h}=\mathfrak{g}^0(\mathfrak{h})$ không liên quan đến trường cơ sở.

#### Mệnh đề 5 {#lie-vii-s2-prop-5 .statement tag=00TY}

Cho $\mathfrak{g}$ là một đại số Lie, $\mathfrak{c}$ là tâm của nó, $\mathfrak{h}$ là một không gian con vectơ của $\mathfrak{g}$. Khi đó $\mathfrak{h}$ là một đại số con Cartan của $\mathfrak{g}$ khi và chỉ khi $\mathfrak{h}$ chứa $\mathfrak{c}$ và $\mathfrak{h}/\mathfrak{c}$ là một đại số con Cartan của $\mathfrak{g}/\mathfrak{c}$.

Giả sử rằng $\mathfrak{h}$ là một đại số con Cartan của $\mathfrak{g}$. Vì $[\mathfrak{c},\mathfrak{g}]\subset \mathfrak{h}$, ta có $\mathfrak{c}\subset \mathfrak{h}$. Mặt khác, $\mathfrak{h}/\mathfrak{c}$ là một đại số con Cartan của $\mathfrak{g}/\mathfrak{c}$ theo Hệ quả 2 của Mệnh đề 4.

Giả sử rằng $\mathfrak{h}\supset \mathfrak{c}$ và $\mathfrak{h}/\mathfrak{c}$ là một đại số con Cartan của $\mathfrak{g}/\mathfrak{c}$. Gọi $f$ là cấu xạ chính tắc từ $\mathfrak{g}$ đến $\mathfrak{g}/\mathfrak{c}$. Đại số $\mathfrak{h}$, là một mở rộng trung tâm của $\mathfrak{h}/\mathfrak{c}$, là lũy linh. Gọi $\mathfrak{n}$ là bộ chuẩn hóa của $\mathfrak{h}$ trong $\mathfrak{g}$. Nếu $x\in \mathfrak{n}$, thì $[f(x),\mathfrak{h}/\mathfrak{c}]\subset \mathfrak{h}/\mathfrak{c}$, do đó $f(x)\in \mathfrak{h}/\mathfrak{c}$, và vì vậy $x\in \mathfrak{h}$. Điều này chứng tỏ rằng $\mathfrak{h}$ là một đại số con Cartan của $\mathfrak{g}$.

#### Hệ quả {#lie-vii-s2-n1-cor-1 .statement tag=00TZ}

Cho $\mathscr{C}_{\infty}\mathfrak{g}$ là hợp của chuỗi trung tâm tăng dần của đại số Lie $\mathfrak{g}$ (Chương I, §1, no. 6). Các đại số con Cartan của $\mathfrak{g}$ là các ảnh ngược của các đại số con Cartan của $\mathfrak{g}/\mathscr{C}_{\infty}\mathfrak{g}$.

Thật vậy, tâm của $\mathfrak{g}/\mathscr{C}_i\mathfrak{g}$ là $\mathscr{C}_{i+1}\mathfrak{g}/\mathscr{C}_i\mathfrak{g}$, và hệ quả suy ra ngay lập tức từ Mệnh đề 5 bằng quy nạp.

#### Nhận xét {#lie-vii-s2-n1-rem-1 .statement tag=00U0}

$\mathscr{C}_{\infty}\mathfrak{g}$ là iđêan nhỏ nhất $\mathfrak{n}$ của $\mathfrak{g}$ sao cho tâm của $\mathfrak{g}/\mathfrak{n}$ bằng không; nó là một iđêan đặc số và lũy linh của $\mathfrak{g}$.

### 2. CÁC PHẦN TỬ CHÍNH QUY CỦA MỘT ĐẠI SỐ LIE

[Nhắc lại rằng từ nay về sau $k$ được giả thiết là vô hạn.]

Cho $\mathfrak{g}$ là một đại số Lie chiều $n$. Nếu $x\in \mathfrak{g}$, viết đa thức đặc trưng của ad $x$ dưới dạng

det(T $-$ ad $x$) $=\sum_{i=0}^na_i(x)T^i$, với $a_i(x)\in k$.

Ta có $a_i(x) = (-1)^{n-i}$Tr $(\bigwedge^{n-i}$ ad $x)$, xem Đại số, Chương III, §8, no. 11. Điều này cho thấy rằng $x \rightarrow a_i(x)$ là một ánh xạ đa thức thuần nhất bậc $n-i$ từ $\mathfrak{g}$ vào $k($Đại số, Chương IV, §5, no. 9).

#### Nhận xét 1 {#lie-vii-s2-n2-rem-1 .statement tag=00U1}

Nếu $\mathfrak{g}\not=\{0\},a_0= 0$ vì (ad $x$)$(x) = 0$ với mọi $x\in \mathfrak{g}$.

#### Nhận xét 2 {#lie-vii-s2-n2-rem-2 .statement tag=00U2}

Cho $k'$ là một mở rộng của $k$. Viết det(T $-$ ad $x'$) $=\sum_{i=0}^na'_i(x')T^i$ với $x'\in \mathfrak{g}\otimes_kk'$. Khi đó $a'_i|\mathfrak{g}=a_i$ với mọi $i$.

#### Định nghĩa 2 {#lie-vii-s2-def-2 .statement tag=00U3}

Hạng của $\mathfrak{g}$, ký hiệu là rk($\mathfrak{g}$), là số nguyên nhỏ nhất $l$ sao cho $a_l\not= 0$. Một phần tử $x$ của $\mathfrak{g}$ được gọi là chính quy nếu $a_l(x)\not= 0$.

Với mọi $x\in \mathfrak{g}$, rk($\mathfrak{g}$)$\leq$ dim$\mathfrak{g}^0(x)$, và đẳng thức xảy ra khi và chỉ khi $x$ là chính quy.

Tập hợp các phần tử chính quy là trù mật và mở trong $\mathfrak{g}$ đối với tôpô Zariski (Phụ lục I).

#### Ví dụ 1 {#lie-vii-s2-n2-exa-1 .statement tag=00U4}

Nếu $\mathfrak{g}$ là lũy linh, rk($\mathfrak{g}$) $=$ dim$\mathfrak{g}$ và mọi phần tử của $\mathfrak{g}$ đều chính quy.

#### Ví dụ 2 {#lie-vii-s2-n2-exa-2 .statement tag=00U5}

Cho $\mathfrak{g}=\mathfrak{s}\mathfrak{l}(2, k)$. Nếu $x=(\gamma -\alpha )\in \mathfrak{g}$, một phép tính dễ dàng cho

$$
\beta \gamma
$$

det(T $-$ ad $x$) $= T^3-4(\alpha \beta +\gamma^2)T$.

Nếu đặc số của $k$ là $\not= 2$, thì rk($\mathfrak{g}$) $= 1$ và các phần tử chính quy là những $x$ sao cho $\alpha \beta +\gamma^2\not= 0$.

#### Ví dụ 3 {#lie-vii-s2-n2-exa-3 .statement tag=00U6}

Cho V là một không gian vectơ có số chiều hữu hạn $n$, và $\mathfrak{g}=\mathfrak{g}\mathfrak{l}(V)$. Gọi $\overline{k}$ là một bao đóng đại số của $k$. Cho $x\in \mathfrak{g}$, và gọi $\lambda_1, . . . , \lambda_n$ là các nghiệm trong $\overline{k}$ của đa thức đặc trưng của $x$ (mỗi nghiệm được viết lại một số lần bằng với bội số của nó). Đẳng cấu chính tắc từ $V^*\otimes V$ lên $\mathfrak{g}$ là tương thích với các cấu trúc $\mathfrak{g}$-môđun của hai không gian này, nói cách khác nó biến $1\otimes x-^tx\otimes 1$ thành ad $x$ (Chap. I, §3, no. 3, Prop. 4). Theo §1, Prop. 4 (i), suy ra rằng các nghiệm của đa thức đặc trưng của ad $x$ là các $\lambda_i-\lambda_j$ với $1\leq i\leq n,1\leq j\leq n$ (mỗi nghiệm được viết lại một số lần bằng với bội số của nó). Do đó, hạng của $\mathfrak{g}$ là $n$, và $x$ là chính quy khi và chỉ khi mỗi $\lambda_i$ là một nghiệm đơn của đa thức đặc trưng của $x$.

#### Mệnh đề 6 {#lie-vii-s2-prop-6 .statement tag=00U7}

Cho $\mathfrak{g}$ là một đại số Lie, $k'$ là một mở rộng của $k$, và $\mathfrak{g}'=$ $\mathfrak{g}\otimes_kk'$.

(i) Một phần tử $x$ của $\mathfrak{g}$ là chính quy trong $\mathfrak{g}$ khi và chỉ khi $x\otimes 1$ là chính quy trong $\mathfrak{g}'$.

(ii) rk($\mathfrak{g}$) $=$ rk($\mathfrak{g}'$).

Điều này suy ra từ Nhận xét 2.

#### Mệnh đề 7 {#lie-vii-s2-prop-7 .statement tag=01IY}

Cho $(\mathfrak{g}_i)_{i\in I}$ là một họ hữu hạn các đại số Lie, và cho $\mathfrak{g}=$ $\prod_{i\in I}\mathfrak{g}_i$.

(i) Một phần tử $(x_i)_{i\in I}$ của $\mathfrak{g}$ là chính quy trong $\mathfrak{g}$ khi và chỉ khi, với mọi $i\in I,x_i$ là chính quy trong $\mathfrak{g}_i$.

(ii) rk($\mathfrak{g}$) $=\sum_{i\in I}$ rk($\mathfrak{g}_i$).

Thật vậy, với mọi $x= (x_i)_{i\in I}\in \mathfrak{g}$, đa thức đặc trưng của ad$_{\mathfrak{g}}x$ là tích của các đa thức đặc trưng của các ad$_{\mathfrak{g}_i}x_i$.

#### Mệnh đề 8 {#lie-vii-s2-prop-8 .statement tag=00U8}

Cho $f:\mathfrak{g}\rightarrow \mathfrak{g}'$ là một đồng cấu toàn ánh của các đại số Lie.

(i) Nếu $x$ là một phần tử chính quy của $\mathfrak{g},f(x)$ là chính quy trong $\mathfrak{g}'$. Đảo lại là đúng nếu Ker $f$ được chứa trong tâm của $\mathfrak{g}$.

(ii) rk($\mathfrak{g}$)$\geq$ rk($\mathfrak{g}'$).

Đặt rk($\mathfrak{g}$) $=r$, rk($\mathfrak{g}'$) $=r'$. Cho $x\in \mathfrak{g}$. Các đa thức đặc số của ad $x$, ad $f(x)$ và ad $x|$Ker $f$ có dạng

$$
P(T) = T^n+a_{n-1}(x)T^{n-1}+\cdots +a_r(x)T^r
$$

$$
Q(T) = T^{n'}+b_{n'-1}(x)T^{n'-1}+\cdots +b_{r'}(x)T^{r'}
$$

$$
R(T) = T^{n''}+c_{n''-1}(x)T^{n''-1}+\cdots +c_{r''}(x)T^{r''}
$$

trong đó các $a_i, b_i, c_i$ là các hàm đa thức trên $\mathfrak{g}$, với $a_r\not= 0, b_{r'}\not= 0, c_{r''}\not= 0$. Ta có P = QR, nên $r=r'+r''$ và $a_r(x) =b_{r'}(x)c_{r''}(x)$, điều này chứng minh (ii) và mệnh đề thứ nhất của (i). Nếu Ker $f$ được chứa trong tâm của $\mathfrak{g}$, thì $R(T) = T^{n''}$ và do đó $a_r(x) =b_{r'}(x)$, suy ra mệnh đề thứ hai của (i).

#### Hệ quả {#lie-vii-s2-n2-cor-1 .statement tag=00U9}

Cho $\mathscr{C}_n\mathfrak{g}(n\geq 0)$ là một số hạng của chuỗi trung tâm tăng của $\mathfrak{g}$ (Chương I, §1, no. 6). Các phần tử chính quy của $\mathfrak{g}$ là những phần tử mà ảnh của chúng trong $\mathfrak{g}/\mathscr{C}_n\mathfrak{g}$ là chính quy.

#### Mệnh đề 9 {#lie-vii-s2-prop-9 .statement tag=00UA}

Cho $\mathfrak{g}$ là một đại số Lie, $\mathfrak{g}'$ là một đại số con của $\mathfrak{g}$. Mọi phần tử của $\mathfrak{g}'$ chính quy trong $\mathfrak{g}$ đều chính quy trong $\mathfrak{g}'$.

Với $x\in \mathfrak{g}'$, hạn chế của ad$_{\mathfrak{g}}x$ lên $\mathfrak{g}'$ là ad$_{\mathfrak{g}'}x$, và do đó xác định, bằng cách chuyển sang thương, một tự đồng cấu $u(x)$ của không gian vectơ $\mathfrak{g}/\mathfrak{g}'$. Gọi $d_0(x)$ (tương ứng $d_1(x)$) là chiều của không gian không hóa của ad$_{\mathfrak{g}'}(x)$ (tương ứng của $u(x)$), và gọi $c_0$ (tương ứng $c_1$) là giá trị nhỏ nhất của $d_0(x)$ (tương ứng $d_1(x)$) khi $x$ thuộc $\mathfrak{g}'$. Tồn tại các ánh xạ đa thức khác không $p_0, p_1$ từ $\mathfrak{g}'$ vào $k$ sao cho

$$
d_0(x) =c_0\Leftarrow \Rightarrow p_0(x)\not= 0,d_1(x) =c_1\Leftarrow \Rightarrow p_1(x)\not= 0
$$

Vì $k$ là vô hạn, tập hợp S gồm các $x\in \mathfrak{g}'$ sao cho $d_0(x) =c_0$ và $d_1(x) =c_1$ là không rỗng. Mọi phần tử của S đều chính quy trong $\mathfrak{g}'$. Mặt khác, S là tập hợp các phần tử của $\mathfrak{g}'$ sao cho không gian nil của ad$_{\mathfrak{g}}x$ có chiều nhỏ nhất, và do đó chứa mọi phần tử của $\mathfrak{g}'$ chính quy trong $\mathfrak{g}$.

#### Nhận xét 3 {#lie-vii-s2-n2-rem-3 .statement tag=00UB}

Các phần tử của $\mathfrak{g}'$ chính quy trong $\mathfrak{g}$ không nhất thiết tồn tại. Nếu có ít nhất một phần tử như vậy tồn tại, thì tập hợp các phần tử ấy chính xác là tập hợp đã được ký hiệu bởi S trong chứng minh trên.

### 3. CÁC ĐẠI SỐ CON CARTAN VÀ CÁC PHẦN TỬ CHÍNH QUY

#### Định lý 1 {#lie-vii-s2-thm-1 .statement tag=00UC}

Cho $\mathfrak{g}$ là một đại số Lie.

(i) Nếu $x$ là một phần tử chính quy của $\mathfrak{g},\mathfrak{g}^0(x)$ là một đại số con Cartan của $\mathfrak{g}$.

(ii) Nếu $\mathfrak{h}$ là một đại số con lũy linh cực đại của $\mathfrak{g}$, và nếu $x\in \mathfrak{h}$ là chính quy trong $\mathfrak{g}$, thì $\mathfrak{h}=\mathfrak{g}^0(x)$.

(iii) Nếu $\mathfrak{h}$ là một đại số con Cartan của $\mathfrak{g}$, thì dim($\mathfrak{h}$)$\geq$ rk($\mathfrak{g}$).

(iv) Các đại số con Cartan của $\mathfrak{g}$ có chiều rk($\mathfrak{g}$) là các $\mathfrak{g}^0(x)$ trong đó $x$ là một phần tử chính quy.

Cho $x$ là một phần tử chính quy của $\mathfrak{g}$ và đặt $\mathfrak{h}=\mathfrak{g}^0(x)$. Rõ ràng $\mathfrak{h}^0(x) =\mathfrak{h}$. Vì $x$ là chính quy trong $\mathfrak{h}$ (Mệnh đề 9), rk($\mathfrak{h}$) $=$ dim($\mathfrak{h}$), nên $\mathfrak{h}$ là lũy linh. Mặt khác, $\mathfrak{h}=\mathfrak{g}^0(x)\supset \mathfrak{g}^0(\mathfrak{h})\supset \mathfrak{h}$, nên $\mathfrak{h}=\mathfrak{g}^0(\mathfrak{h})$ là một đại số con Cartan của $\mathfrak{g}$ (Mệnh đề 4). Điều này chứng minh (i).

Nếu $\mathfrak{h}$ là một đại số con lũy linh cực đại của $\mathfrak{g}$, và nếu $x\in \mathfrak{h}$ là chính quy trong $\mathfrak{g}$, thì $\mathfrak{h}\subset \mathfrak{g}^0(x)$ và $\mathfrak{g}^0(x)$ là lũy linh theo (i), do đó $\mathfrak{h}=\mathfrak{g}^0(x)$, điều này chứng minh (ii).

Nếu $\mathfrak{h}$ là một đại số con Cartan của $\mathfrak{g}$, thì tồn tại $x\in \mathfrak{h}$ sao cho $\mathfrak{h}=\mathfrak{g}^0(x)$ (Hệ quả 1 của Mệnh đề 4), do đó chiều($\mathfrak{h}$)$\geq$ hạng($\mathfrak{g}$), điều này chứng minh (iii). Nếu hơn nữa chiều($\mathfrak{h}$) $=$ hạng($\mathfrak{g}$)$,x$ là chính quy. Cuối cùng, nếu $x'$ là chính quy trong $\mathfrak{g},\mathfrak{g}^0(x')$ là một đại số con Cartan theo (i), và hiển nhiên có chiều hạng($\mathfrak{g}$). Điều này chứng minh (iv).

Ta sẽ thấy ở §3, Định lý 2 rằng, khi $k$ có đặc số không, mọi đại số con Cartan của $\mathfrak{g}$ đều có chiều rk($\mathfrak{g}$).

#### Hệ quả 1 {#lie-vii-s2-thm-1-cor-1 .statement tag=00UD}

Mọi đại số Lie $\mathfrak{g}$ đều có các đại số con Cartan, và hạng của $\mathfrak{g}$ là chiều nhỏ nhất của một đại số con Cartan.

#### Hệ quả 2 {#lie-vii-s2-thm-1-cor-2 .statement tag=00UE}

Cho $f:\mathfrak{g}\rightarrow \mathfrak{g}'$ là một đồng cấu toàn ánh của các đại số Lie. Nếu $\mathfrak{h}'$ là một đại số con Cartan của $\mathfrak{g}'$, thì tồn tại một đại số con Cartan $\mathfrak{h}$ của $\mathfrak{g}$ sao cho $\mathfrak{h}'=f(\mathfrak{h})$.

Đặt $\mathfrak{a}=f^{-1}(\mathfrak{h}')$. Theo Hệ quả $1,\mathfrak{a}$ có một đại số con Cartan $\mathfrak{h}$. Theo Hệ quả 2 của Mệnh đề $4,f(\mathfrak{h}) =\mathfrak{h}'$. Ta sẽ chỉ ra rằng $\mathfrak{h}$ là một đại số con Cartan của $\mathfrak{g}$. Gọi $\mathfrak{n}$ là chuẩn hóa tử của $\mathfrak{h}$ trong $\mathfrak{g}$. Chỉ cần chứng minh rằng $\mathfrak{h}=\mathfrak{n}$. Nếu $x\in \mathfrak{n},f(x)$ thuộc chuẩn hóa tử của $\mathfrak{h}'$ trong $\mathfrak{g}'$, nên $f(x)\in \mathfrak{h}'$ và $x\in \mathfrak{a}$; nhưng $\mathfrak{h}$ là chuẩn hóa tử của chính nó trong $\mathfrak{a}$, nên $x\in \mathfrak{h}$.

#### Hệ quả 3 {#lie-vii-s2-thm-1-cor-3 .statement tag=00UF}

Mọi đại số Lie $\mathfrak{g}$ đều là tổng của các đại số con Cartan của nó.

Tổng $\mathfrak{s}$ của các đại số con Cartan của $\mathfrak{g}$ chứa tập hợp các phần tử chính quy của $\mathfrak{g}$ (Định lý 1 (i)). Vì tập hợp này là trù mật trong $\mathfrak{g}$ đối với tôpô Zariski, nên $\mathfrak{s}=\mathfrak{g}$.

#### Mệnh đề 10 {#lie-vii-s2-prop-10 .statement tag=00UG}

Cho $\mathfrak{g}$ là một đại số Lie, $\mathfrak{a}$ là một đại số con giao hoán của $\mathfrak{g}$ và $\mathfrak{c}$ là hoán tập của $\mathfrak{a}$ trong $\mathfrak{g}$. Giả sử rằng ad$_{\mathfrak{g}}x$ là nửa đơn với mọi $x\in \mathfrak{a}$. Khi đó các đại số con Cartan của $\mathfrak{c}$ là các đại số con Cartan của $\mathfrak{g}$ chứa $\mathfrak{a}$.

Cho $\mathfrak{h}$ là một đại số con Cartan của $\mathfrak{c}$. Vì $\mathfrak{a}$ được chứa trong tâm $\mathfrak{z}$ của $\mathfrak{c},\mathfrak{a}\subset \mathfrak{z}\subset \mathfrak{h}$ (Mệnh đề 5). Gọi $\mathfrak{n}$ là bộ chuẩn hoá của $\mathfrak{h}$ trong $\mathfrak{g}$. Khi đó

$$
[\mathfrak{a},\mathfrak{n}]\subset [\mathfrak{h},\mathfrak{n}]\subset \mathfrak{h}
$$

Vì các ad$_{\mathfrak{g}}x,x\in \mathfrak{a}$ là nửa đơn và giao hoán với nhau, nên theo Đại số, Chương VIII, §5, no. 1, suy ra tồn tại một không gian con vectơ $\mathfrak{d}$ của $\mathfrak{n}$ ổn định dưới ad$_{\mathfrak{g}}\mathfrak{a}$ và sao cho $\mathfrak{n}=\mathfrak{h}\oplus \mathfrak{d}$. Khi đó $[\mathfrak{a},\mathfrak{d}]\subset \mathfrak{h}\cap \mathfrak{d}= 0$, nên $\mathfrak{d}\subset \mathfrak{c}$. Do đó, $\mathfrak{n}$ là bộ chuẩn hoá của $\mathfrak{h}$ trong $\mathfrak{c}$, và vì thế $\mathfrak{n}=\mathfrak{h}$, nên $\mathfrak{h}$ là một đại số con Cartan của $\mathfrak{g}$ chứa $\mathfrak{a}$.

Ngược lại, cho $\mathfrak{h}$ là một đại số con Cartan của $\mathfrak{g}$ chứa $\mathfrak{a}$. Khi đó $\mathfrak{h}=$ $\mathfrak{g}^0(\mathfrak{h})\subset \mathfrak{g}^0(\mathfrak{a})$, và theo giả thiết $\mathfrak{g}_0(\mathfrak{a}) =\mathfrak{g}^0(\mathfrak{a}) =\mathfrak{c}$. Do đó $\mathfrak{a}\subset \mathfrak{h}\subset \mathfrak{c}$ và $\mathfrak{h}$ là một đại số con Cartan của $\mathfrak{c}$ (vì nó bằng với chuẩn hóa tử của chính nó trong $\mathfrak{g}$, và do đó a fortiori trong $\mathfrak{c}$).

#### Mệnh đề 11 {#lie-vii-s2-prop-11 .statement tag=00UH}

Cho $\mathfrak{n}$ là một đại số con lũy linh của một đại số Lie $\mathfrak{g}$. Tồn tại một đại số con Cartan của $\mathfrak{g}$ được chứa trong $\mathfrak{g}^0(\mathfrak{n})$.

Đặt $\mathfrak{a}=\mathfrak{g}^0(\mathfrak{n})$. Khi đó $\mathfrak{n}\subset \mathfrak{a}$ vì $\mathfrak{n}$ là lũy linh. Nếu $x\in \mathfrak{a}$, gọi $P(x)$ là định thức của tự đồng cấu của $\mathfrak{g}/\mathfrak{a}$ được xác định bởi ad $x$. Ký hiệu $\mathfrak{a}'$ là tập hợp các $x\in \mathfrak{a}$ sao cho $P(x)\not= 0$, đó là một tập con mở của $\mathfrak{a}$ trong tôpô Zariski; các quan hệ $x\in \mathfrak{a}'$ và $\mathfrak{g}^0(x)\subset \mathfrak{a}$ là tương đương. Theo Mệnh đề 7 (ii) của §1, no. 2, tồn tại $y\in \mathfrak{n}$ sao cho $\mathfrak{g}^0(y) =\mathfrak{a}$, và $y\in \mathfrak{a}'$ nên $\mathfrak{a}'$ là không rỗng. Vì $\mathfrak{a}'$ là mở, giao của nó với tập hợp các phần tử chính quy của $\mathfrak{a}$ là không rỗng. Lấy $x$ là một phần tử của giao này. Khi đó $\mathfrak{g}^0(x)\subset \mathfrak{a}$ và $\mathfrak{g}^0(x)$ là một đại số con Cartan của $\mathfrak{a}$, do đó nó lũy linh. Mặt khác, Mệnh đề 10 (i) của §1, no. 3, cho thấy rằng $\mathfrak{g}^0(x)$ là chuẩn hóa tử của chính nó trong $\mathfrak{g}$; bởi vậy nó là một đại số con Cartan của $\mathfrak{g}$, điều này hoàn thành chứng minh.

### 4. ĐẠI SỐ CON CARTAN CỦA CÁC ĐẠI SỐ LIE NỬA ĐƠN

#### Định lý 2 {#lie-vii-s2-thm-2 .statement tag=00UI}

Giả sử rằng $k$ có đặc số 0. Cho $\mathfrak{g}$ là một đại số Lie nửa đơn, $\mathfrak{h}$ là một đại số con Cartan của $\mathfrak{g}$. Khi đó $\mathfrak{h}$ là giao hoán, và mọi phần tử của nó đều là nửa đơn trong $\mathfrak{g}$ (Ch. I, §6, no. 3, Định nghĩa 3).

Vì $\mathfrak{h}=\mathfrak{g}^0(\mathfrak{h}),\mathfrak{h}$ là khả quy (§1, Mệnh đề 11), do đó giao hoán vì nó lũy linh. Mặt khác, hạn chế của biểu diễn kề của $\mathfrak{g}$ lên $\mathfrak{h}$ là nửa đơn (loc. cit.), nên các phần tử của $\mathfrak{h}$ là nửa đơn trong $\mathfrak{g}$ (Đại số, Ch. VIII, §5, no. 1).

#### Hệ quả 1 {#lie-vii-s2-thm-2-cor-1 .statement tag=00UJ}

Nếu $x\in \mathfrak{h}$ và $y\in \mathfrak{g}^{\lambda}(\mathfrak{h})$, ta có $[x, y] =\lambda (x)y$.

Thật vậy, $\mathfrak{g}^{\lambda(x)}(x) =\mathfrak{g}_{\lambda(x)}(x)$ vì ad $x$ là nửa đơn.

#### Hệ quả 2 {#lie-vii-s2-thm-2-cor-2 .statement tag=00UK}

Mọi phần tử chính quy của $\mathfrak{g}$ đều là nửa đơn.

Thật vậy, một phần tử như vậy thuộc một đại số con Cartan (no. 3, Th. 1 (i)).

#### Hệ quả 3 {#lie-vii-s2-thm-2-cor-3 .statement tag=00UL}

Cho $\mathfrak{h}$ là một đại số con Cartan của một đại số Lie khả quy $\mathfrak{g}$.

a$)\mathfrak{h}$ là giao hoán.

b) Nếu $\rho$ là một biểu diễn nửa đơn hữu hạn chiều của $\mathfrak{g}$, thì các phần tử của $\rho (\mathfrak{h})$ là nửa đơn.

Cho $\mathfrak{c}$ là tâm của $\mathfrak{g}$, và $\mathfrak{s}$ là đại số dẫn xuất của nó. Khi đó $\mathfrak{g}=\mathfrak{c}\times \mathfrak{s}$, nên $\mathfrak{h}=\mathfrak{c}\times \mathfrak{h}'$, trong đó $\mathfrak{h}'$ là một đại số con Cartan của $\mathfrak{s}$ (Mệnh đề 2). Theo Định lý $2,\mathfrak{h}'$ là giao hoán, do đó $\mathfrak{h}$ cũng giao hoán. Hơn nữa, $\rho (\mathfrak{h}')$ gồm các phần tử nửa đơn và $\rho (\mathfrak{c})$ cũng vậy (Chương I, §6, no. 5, Định lý 4); mệnh đề $b)$ được suy ra.

### Bài tập {#lie-vii-s2-exercises}

Xem [các bài tập cho § 2](exercises/s2/).
