---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: VII
chapter_title: CARTAN SUBALGEBRAS AND REGULAR ELEMENTS
section: 2
section_title: A connectedness property
appendix: true
lang: vi
source: lie-vii-ix
book_pages: 48-49, 67
pdf_pages: 0058-0059, 0076-0076
extraction: native
statements: 3
exercises: 2
content_sha256: ba53b29a637cc213562e73b177df818603f6dfd514eba87fd9f702d046fdb1ec
translated_from: content/en/lie/VII/A2_a2_a_connectedness_property.md
source_content_sha256: e52c40721671251b25cbd21bd6c6376bf20e17aa16de77c1b806f74183e1c74a
translation_model: gpt-5.4
translation_run: translate-vi-923b55d1
glossary_version: 34
glossary_terms_sha256: 9492393fd87f4afe1c57b615727f8bdcff1a02e84ebf757c3c87420dd2575cd1
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## PHỤ LỤC II MỘT TÍNH CHẤT LIÊN THÔNG

#### Bổ đề 1 {#lie-vii-a2-lem-1 .statement tag=00XN}

Cho X là một không gian tôpô liên thông và $\Omega$ là một tập con mở trù mật của X. Nếu, với mọi $x\in X$, tồn tại một lân cận V của $x$ sao cho $V\cap \Omega$ là liên thông, thì $\Omega$ là liên thông.

Thật vậy, gọi $\Omega_0$ là một tập con mở và đóng khác rỗng của $\Omega$. Lấy $x\in X$ và gọi V là một lân cận của $x$ sao cho $V\cap \Omega$ là liên thông. Nếu $x\in \overline{\Omega}_0$,

$$
(V\cap \Omega )\cap \Omega_0= V\cap \Omega_0\not=\emptyset
$$

nên $V\cap \Omega \subset \Omega_0$. Do đó, vì $\Omega$ trù mật trong $X,\overline{\Omega}_0$ là một lân cận của $x$. Do đó, $\Omega_0$ là không rỗng, mở và đóng, và vì X là liên thông, $\overline{\Omega}_0= X$. Vì $\Omega_0$ đóng trong $\Omega$, điều này suy ra $\Omega_0=\Omega \cap \overline{\Omega}_0=\Omega$, điều đó chứng minh rằng $\Omega$ là liên thông.

#### Bổ đề 2 {#lie-vii-a2-lem-2 .statement tag=00XO}

Cho U là một quả cầu mở trong $\mathbf{C}^n$ và $f: U\rightarrow \mathbf{C}$ là một hàm chỉnh hình, không đồng nhất bằng không. Cho A là một tập con của U sao cho $f= 0$ trên A. Khi đó U **--** A trù mật trong U và liên thông.

Mật độ của U**--** A suy ra từ Đa tạp khả vi và giải tích, Kết quả, 3.2.5. Trước hết giả sử rằng $n= 1$. Nếu $a\in A$, khai triển chuỗi lũy thừa của $f$ tại $a($Đa tạp khả vi và giải tích, Kết quả, 3.2.1) không rút gọn thành 0, và suy ra rằng tồn tại một lân cận $V_a$ của $a$ trong U sao cho $f$ không triệt tiêu trên $V_a$ **--** $\{a\}$. Do đó, $a$ cô lập trong A, điều này chứng tỏ rằng A là một tập con rời rạc của U, vì thế đếm được do U đếm được tại vô cực. Cho $x, y\in U$ **--** A. Hợp của các đường thẳng afin thực nối $x$ (tương ứng $y$) với một điểm của A là gầy (Tôpô đại cương, Chương IX, §5, no. 2, Định nghĩa 2). Vì thế, tồn tại $z\in U$ **--** A sao cho không đoạn nào trong hai đoạn $[x, z]$ và $[y, z]$ cắt A. Như vậy các điểm $x, y, z$ thuộc cùng một thành phần liên thông của U **--** A, điều này chứng tỏ bổ đề trong trường hợp $n= 1$. Ta chuyển sang trường hợp tổng quát. Ta có thể giả sử rằng A là tập hợp các điểm không của $f($Tôpô đại cương, Chương I, §11, no. 1, Mệnh đề 1). Cho $x, y\in U$**--** A và L là một đường thẳng afin chứa $x$ và $y$. Hạn chế của $f$ trên $L\cap U$ không đồng nhất bằng không vì $x\in L\cap U$. Theo điều đã được chứng minh ở trên, $x$ và $y$ thuộc cùng một thành phần liên thông của $(L\cap U)$ **--** $(L\cap A)$ và do đó thuộc cùng một thành phần liên thông của U **--** A.

#### Bổ đề 3 {#lie-vii-a2-lem-3 .statement tag=00XP}

Cho X là một đa tạp giải tích-phức liên thông hữu hạn chiều và A là một tập con của X thỏa mãn điều kiện sau:

Với mọi $x\in X$, tồn tại một mầm hàm giải tích $f_x$, không triệt tiêu

tại $x$, sao cho mầm của A tại $x$ được chứa trong mầm tại $x$ của tập hợp

các không điểm của $f_x$.

Khi đó X **--** A là trù mật trong X và liên thông.

Tính trù mật của X**--** A suy ra từ Đa tạp khả vi và giải tích, Các kết quả, 3.2.5. Ta có thể giả sử rằng A đóng (Tôpô đại cương, Chương I, §11, no. 1, Mệnh đề 1). Với mọi $x\in X$, tồn tại một lân cận mở V của $x$ và một đẳng cấu $c$ từ V lên một quả cầu mở trong $\mathbf{C}^n$ sao cho $c(A\cap V)$ được chứa trong tập hợp các không điểm của một hàm chỉnh hình không đồng nhất bằng không trên $c(V)$. Khi đó, theo Bổ đề $2, V\cap (X$ **--** A) là liên thông. Theo Bổ đề 1, điều này chứng minh rằng X **--** A là liên thông.

### Bài tập {#lie-vii-a2-exercises}

Xem [các bài tập cho Phụ lục 2](exercises/a2/).
