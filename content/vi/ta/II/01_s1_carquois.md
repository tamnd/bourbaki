---
book: ta
book_title: Topologie algébrique
chapter: II
chapter_title: GROUPOÏDES
section: 1
section_title: Carquois
lang: vi
source: ta-i-iv-fr
book_pages: TA II.151-TA II.155, TA II.215-TA II.218
pdf_pages: 0167-0171, 0231-0234
extraction: native
subsections:
    - "no": 1
      title: Définition d’un carquois
      page: 151
      pdf_page: 167
    - "no": 2
      title: Sous-carquois
      page: 152
      pdf_page: 168
    - "no": 3
      title: Morphismes de carquois
      page: 152
      pdf_page: 168
    - "no": 4
      title: Produits de carquois
      page: 153
      pdf_page: 169
    - "no": 5
      title: Chemins et lacets dans un carquois
      page: 154
      pdf_page: 170
    - "no": 6
      title: Composantes connexes d’un carquois
      page: 154
      pdf_page: 170
statements: 2
exercises: 10
content_sha256: 72c12e9e43bd8c32499f0941593d988bc19a85d4b7a736d93f3e1f92a46b4088
translated_from: content/en-mt/ta/II/01_s1_carquois.md
source_lang: en-mt
translation_method: machine
source_content_sha256: efe28e60038f2693e1a5ba938564c626f052607bb9c4dbb84cfc0a6a0a6620d5
translation_model: gpt-5.4
translation_run: translate-vi-6c6cf1e9
glossary_version: 34
glossary_terms_sha256: c8024a46234c1309d154c571005283d2c2b44f21deed5578a1d8d15c7034f4a2
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 1. QUIVER

Đài kỷ niệm của nó, tráng lệ giữa các đài kỷ niệm,

Dựng tua tủa, phía trên một bức tường gạch khô, chóp các tháp của nó như một ống tên...

Victor Hugo, La Légende des siècles

### 1. Định nghĩa của một quiver

#### Định nghĩa 1 {#ta-ii-s1-def-1 .statement tag=01SS}

Một quiver là một bộ bốn $(S,F, o, t)$, trong đó S và F là các tập hợp và $o,t$ là các ánh xạ từ F vào S.

Cho $C = (S,F, o, t)$ là một quiver. Các phần tử của S được gọi là các đỉnh của C. Các phần tử của F được gọi là các mũi tên của C. Cho $f$ là một mũi tên của C; đỉnh $o(f)$ được gọi là gốc hay nguồn của $f$, đỉnh $t(f)$ được gọi là đầu, hay đích, của $f$; người ta cũng nói rằng $f$ nối đỉnh $o(f)$ với đỉnh $t(f)$. Các ánh xạ $o$ và $t$ lần lượt được gọi là ánh xạ nguồn và ánh xạ đích, hoặc gốc và đầu, của quiver C.

© N. Bourbaki and Springer-Verlag Berlin Heidelberg 2   016

N. Bourbaki, Algebraic Topology, DOI 10.1007/978-3-662-49361-8_2  151

Khi C là một quiver, Som(C), Fl(C), $o_C$ và $t_C$ lần lượt sẽ ký hiệu tập hợp các đỉnh, tập hợp các mũi tên, ánh xạ nguồn và ánh xạ đích của C. Cho $a$ và $b$ là các đỉnh của C; tập hợp các mũi tên của C nối $a$ với $b$ được ký hiệu bởi Fl$_{a,b}(C)$, hoặc cũng bởi $C_{a,b}$.

Để các lập luận dễ hiểu hơn, người ta có thể biểu diễn một quiver bằng một biểu đồ gồm các điểm và các đường có mũi tên tương ứng với các đỉnh và các mũi tên. Biểu đồ:

$$
f_1g
$$

$\bullet \bullet \bullet k$

$abc$

$f_2h$

biểu diễn một quiver có các đỉnh là $a,b,c$, các mũi tên là $f_1, f_2, g, h, k$, và các ánh xạ nguồn và đích được cho bởi

$$
o(f_1) =o(f_2) =ao(g) =bo(h) =co(k) =c
$$

$$
t(f_1) =t(f_2) =bt(g) =ct(h) =bt(k) =c
$$

### 2. Quiver con

Cho C và $C'$ là các quiver. Người ta nói rằng $C'$ là một quiver con của C nếu có Som(C$'$)$\subset$ Som(C), Fl(C$'$)$\subset$ Fl(C) và nếu các ánh xạ $o_{C'}$ và $t_{C'}$ trùng nhau trên Fl(C$'$) với các ánh xạ $o_C$ và $t_C$. Nếu hơn nữa, mọi mũi tên của C mà nguồn và đích đều thuộc Som(C$'$) đều là một mũi tên của $C'$, thì người ta nói rằng $C'$ là một quiver con đầy đủ của C.

Cho C là một quiver và cho $(C_i)_{i\in I}$ là một họ các quiver con của C. Giao của họ $(C_i)_{i\in I}$ được định nghĩa là, và được ký hiệu bởi $\bigcap_{i\in I}C_i$, quiver con của C mà tập hợp các đỉnh là $\bigcap_{i\in I}$ Som(C$_i$) và tập hợp các mũi tên là $\bigcap_{i\in I}$ Fl(C$_i$).

### 3. Cấu xạ của các quiver

Cho C và $C'$ là các quiver. Một cấu xạ quiver từ C vào $C'$ là một cặp $(u, v)$, trong đó $u:$ Som(C) $\rightarrow$ Som(C$'$) và $v:$ Fl(C) $\rightarrow$ Fl(C$'$) là các ánh xạ sao cho $o_{C'}\circ v=u\circ o_C$ và $t_{C'}\circ v=u\circ t_C$.

Cho $\varphi = (u, v)$ là một cấu xạ quiver từ C vào $C'$. Các ánh xạ $u$ và $v$ được ký hiệu bởi Som($\varphi$ ) và Fl($\varphi$ ). Nếu $a$ là một đỉnh của C, ta sẽ ký hiệu một cách lạm dụng bởi $\varphi (a)$ ảnh của đỉnh $a$ của C, và ta sẽ nói rằng $\varphi (a)$ là ảnh của $a$ dưới $\varphi$. Tương tự, nếu $f$ là một mũi tên của C, ta sẽ ký hiệu một cách lạm dụng bởi $\varphi (f)$ mũi tên $v(f)$ của $C'$ và ta sẽ nói rằng đó là ảnh của $f$ dưới $\varphi$.

Cho C, $C',C''$ là ba quiver, cho $\varphi = (u, v)$ là một cấu xạ từ C vào $C'$ và cho $\varphi '= (u', v')$ là một cấu xạ từ $C'$ vào $C''$. Khi đó $(u'\circ u, v'\circ v)$ là một cấu xạ từ C vào $C''$ được ký hiệu bởi $\varphi '\circ \varphi$ và được gọi là hợp thành của $\varphi '$ và $\varphi$.

Id$_C$ ký hiệu cấu xạ (Id$_{Som(C)}$, Id$_{Fl(C)}$) từ C vào chính nó.

Cho $\varphi$ là một cấu xạ quiver từ C vào $C'$. Để $\varphi$ là một đẳng cấu, điều kiện cần và đủ là các ánh xạ Som($\varphi$ ) và Fl($\varphi$ ) là song ánh (x. E, IV, p. 6).

Vì vậy, nếu ta gọi một cấu trúc quiver trên các tập hợp S và F là dữ liệu của hai ánh xạ $o, t: F\rightarrow S$, thì có thể lấy các cấu xạ quiver làm các cấu xạ của cấu trúc này (E, IV, p. 11).

Cho $\varphi$ là một cấu xạ quiver từ C vào $C'$. Tồn tại duy nhất một quiver con của $C'$ mà các tập hợp đỉnh và mũi tên lần lượt là các ảnh của Som($\varphi$ ) và Fl($\varphi$ ). Nó được ký hiệu bởi $\varphi (C)$ và được gọi là ảnh của C dưới $\varphi$. Ta nói rằng $\varphi$ là đơn ánh nếu các ánh xạ Som($\varphi$ ) và Fl($\varphi$ ) là đơn ánh; trong trường hợp đó, $\varphi$ cảm sinh một đẳng cấu từ C lên ảnh của nó.

Cho $\varphi$ và $\psi$ là các cấu xạ của đồ thị có hướng từ C đến $C'$. Tồn tại một đồ thị con duy nhất của C mà các đỉnh và các mũi tên của nó lần lượt là các đỉnh và các mũi tên của C có cùng ảnh dưới $\varphi$ và $\psi$. Nó được gọi là bộ cân bằng của $\varphi$ và $\psi$.

### 4. Tích của các đồ thị có hướng

Cho $(C_i)_{i\in I}$ là một họ các đồ thị có hướng. Đặt S = $\prod_{i\in I}$ Som(C$_i$), $F =\prod_{i\in I}$ Fl(C$_i$), và gọi $o$ và $t$ lần lượt là các ánh xạ $\prod_{i\in I}o_{C_i}$ và $\prod_{i\in I}t_{C_i}$. Bộ bốn $C = (S,F, o, t)$ là một đồ thị có hướng, được gọi là đồ thị có hướng tích của họ $(C_i)_{i\in I}$.

Tồn tại một cấu xạ duy nhất của đồ thị có hướng pr$_i: C\rightarrow C_i$ sao cho các ánh xạ Som(pr$_i$) và Fl(pr$_i$) lần lượt là các phép chiếu có chỉ số $i$ từ Som(C) lên Som(C$_i$) và từ Fl(C) lên Fl(C$_i$).

Ta có tính chất phổ quát sau đây: Cho $C'$ là một đồ thị có hướng; với mọi họ $(\varphi_i)_{i\in I}$, trong đó, với mọi $i\in I,\varphi_i: C'\rightarrow C_i$ là một cấu xạ của đồ thị có hướng, tồn tại một cấu xạ duy nhất của đồ thị có hướng $\varphi : C'\rightarrow C$ sao cho $\varphi_i=$ pr$_i\circ \varphi$ với mọi $i\in I$.

### 5. Đường đi và vòng trong một đồ thị có hướng

#### Định nghĩa 2 {#ta-ii-s1-def-2 .statement tag=01ST}

Cho C là một đồ thị có hướng. Một đường đi trong C là một dãy $c= (a_0, f_1, a_1, . . . , a_{n-1}, f_n, a_n)$, trong đó $n$ là một số nguyên $\geqslant 0,a_0, . . . , a_n$ là các đỉnh của C, và trong đó, với $1\leqslant i\leqslant n,f_i$ là một mũi tên của C nối $a_{i-1}$ với $a_i$. Người ta nói rằng đường đi $c$ có độ dài $n$.

Cho $c= (a_0, f_1, a_1, . . . , a_{n-1}, f_n, a_n)$ là một đường đi độ dài $n$ trong C. Đỉnh $a_0$ được gọi là gốc, hay nguồn, của $c$; đỉnh $a_n$ được gọi là đích, hay điểm cuối, của $c$; người ta cũng nói rằng $c$ nối đỉnh $a_0$ với đỉnh $a_n$. Đỉnh $a_i$, với $0\leqslant i\leqslant n$, được gọi là đỉnh có chỉ số $i$; mũi tên $f_i$, với $1\leqslant i\leqslant n$, được gọi là mũi tên thứ $i$, hay mũi tên có chỉ số $i$. Một đường đi có độ dài $\geqslant 1$ được xác định bởi dãy các mũi tên của nó.

Một đường đi mà gốc bằng đích được gọi là một vòng. Một đường đi có độ dài 0 là một vòng, được gọi là hằng.

Người ta nói rằng các đường đi

$c= (a_0, f_1, a_1, . . . , a_{n-1}, f_n, a_n)$ và $c'= (a'_0, f'_1, a'_1, . . . , a'_{m-1}, f'_m, a'_m)$

trong C được ghép nối nếu số hạng $a_n$ của $c$ là gốc $a'_0$ của $c'$. Trong trường hợp này, dãy $(a_0, f_1, a_1, . . . , a_{n-1}, f_n, a_n, f'_1, a'_1, . . . , f'_m, a'_m)$ là một đường đi trong C, được ký hiệu bởi $c*c'$ và được gọi là đường đi ghép của $c$ và $c'$. Nó nối gốc của $c$ với số hạng cuối của $c'$; độ dài của nó là tổng các độ dài của các đường đi $c$ và $c'$.

### 6. Các thành phần liên thông của một quiver

Cho $C = (S,F, o, t)$ là một quiver. Xét quan hệ tương đương tinh nhất $R_C$ trên S sao cho quan hệ $R_C\{o(f), t(f)\}$ được thỏa mãn với mọi mũi tên $f$ của C. Hai đỉnh $a,b$ của C tương đương đối với quan hệ này khi và chỉ khi tồn tại một số nguyên $n\geqslant 0$, các đỉnh $a_0, . . . , a_n$ của C và các mũi tên $f_1, . . . , f_n$ của C sao cho $a_0=a,a_n=b$ và sao cho, với $1\leqslant i\leqslant n$, mũi tên $f_i$ nối hoặc $a_{i-1}$ với $a_i$, hoặc $a_i$ với $a_{i-1}$.

Các lớp tương đương của quan hệ tương đương này được gọi là các thành phần liên thông của C. Ta ký hiệu bởi $\pi_0(C)$ tập hợp các thành phần liên thông của C. Sau hết, ta nói rằng C liên thông nếu nó có nhiều nhất một thành phần liên thông.

Cho $\varphi : C\rightarrow C'$ là một cấu xạ của các quiver. Ánh xạ Som($\varphi$ ) xác định, bằng cách chuyển qua các thương, một ánh xạ từ $\pi_0(C)$ vào $\pi_0(C')$ mà ta sẽ ký hiệu là $\pi_0(\varphi )$.

## BÀI TẬP {#ta-ii-s1-exercises}

Xem [các bài tập cho § 1](exercises/s1/).
