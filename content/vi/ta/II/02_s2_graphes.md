---
book: ta
book_title: Topologie algébrique
chapter: II
chapter_title: GROUPOÏDES
section: 2
section_title: Graphes
lang: vi
source: ta-i-iv-fr
book_pages: TA II.155-TA II.159, TA II.219-TA II.223
pdf_pages: 0171-0175, 0235-0239
extraction: native
subsections:
    - "no": 1
      title: Définition d’un graphe
      page: 155
      pdf_page: 171
    - "no": 2
      title: Orientation d’un graphe
      page: 156
      pdf_page: 172
    - "no": 3
      title: Graphes orientés et carquois
      page: 156
      pdf_page: 172
    - "no": 4
      title: Arbres
      page: 157
      pdf_page: 173
statements: 5
exercises: 12
content_sha256: a6953fc7c4a854cb3c6d73d4a02e9ff6087bdec5c5b1d5988e7d23f44fba628f
translated_from: content/en-mt/ta/II/02_s2_graphes.md
source_lang: en-mt
translation_method: machine
source_content_sha256: 2b453f333fdb6d905983651acfc36b7060a9577a4763b395fc05b04e8eb89f0d
translation_model: gpt-5-6-mini, gpt-5-mini
translation_run: translate-vi-752d4eab
glossary_version: 34
glossary_terms_sha256: e62b74a8479332bedac74d03a5e75b3312f8d8b3dc328f332ff4f30951a9dee3
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 2. ĐỒ THỊ

### 1. Định nghĩa của một đồ thị

#### Định nghĩa 1 {#ta-ii-s2-def-1 .statement tag=01SU}

Một đồ thị[^1] là một quiver $(S,F, o, t)$ được trang bị một phép đối hợp trên F, ký hiệu bởi $f\mapsto \overline{f}$, không có điểm bất động và sao cho $t(\overline{f}) =o(f)$ với mọi $f\in F$.

Quiver $(S,F, o, t)$ được gọi là nằm dưới đồ thị này. Với mọi mũi tên $f$ của quiver này, theo định nghĩa, ta có $\overline{f}=f,\overline{f}=\not f$ và $t(\overline{f}) =$ $o(f)$. Áp dụng quan hệ cuối cùng này cho mũi tên $\overline{f}$, ta thu được đẳng thức $o(\overline{f}) =t(f)$. Mũi tên $\overline{f}$ được gọi là mũi tên đối của $f$.

Một cặp các mũi tên đối của đồ thị được gọi là một cạnh của đồ thị. Mỗi một trong hai mũi tên thuộc cặp này được gọi là một định hướng của cạnh này. Vì lý do đó, các mũi tên của một đồ thị còn được gọi là các cạnh định hướng của đồ thị.

Nếu G và $G'$ là các đồ thị, một cấu xạ đồ thị từ G vào $G'$ là một cấu xạ quiver $\varphi : G\rightarrow G'$ sao cho $\varphi (f) =\varphi (\overline{f})$ với mọi mũi tên $f$ của G.

Cho G và $G'$ là các đồ thị; ta nói rằng $G'$ là một đồ thị con của G nếu nó là một quiver con của G và nếu phép đối hợp của Fl(G$'$) là hạn chế của phép đối hợp của Fl(G).

### 2. Định hướng của một đồ thị

Cho G là một đồ thị. Một định hướng của G là một tập con A của tập hợp các mũi tên của G sao cho $A\cap \overline{A}=\emptyset$ và $A\cup \overline{A}=$ Fl(G).

Một đồ thị được trang bị một định hướng được gọi là một đồ thị định hướng.

Cho G là một đồ thị định hướng và A là định hướng của nó; một đồ thị con định hướng của G là một đồ thị con $G'$ của G được trang bị định hướng $A'=$ Fl(G$'$)$\cap A$.

Cho $(G,A)$ và $(G',A')$ là các đồ thị định hướng. Một cấu xạ đồ thị định hướng từ $(G,A)$ vào $(G',A')$ là một cấu xạ đồ thị $\varphi : G\rightarrow G'$ sao cho Fl($\varphi$ )$(A)\subset A'$.

### 3. Đồ thị định hướng và các quiver

Cho G là một đồ thị, $(S,F, o, t)$ là quiver nằm dưới G, và A là một định hướng của G. Khi đó $(S,A, o|A, t|A)$ là một quiver, được gọi là quiver liên kết với đồ thị định hướng $(G,A)$.

Ngược lại, cho $C = (S,F, o, t)$ là một quiver. Đặt $\widetilde{F} = F\times \{-1,1\}$ và gọi $\widetilde{o},\widetilde{t}$ là các ánh xạ từ $\widetilde{F}$ vào S được xác định bởi

$$
\widetilde{o}(f,1) =o(f)\widetilde{o}(f,-1) =t(f)
$$

$$
\widetilde{t}(f,1) =t(f)\widetilde{t}(f,-1) =o(f)
$$

với $f\in F$. Khi đó $\widetilde{C} = (S,\widetilde{F},\widetilde{o},\widetilde{t})$, được trang bị phép đối hợp $(f, \varepsilon )\mapsto (f,-\varepsilon )$ của $\widetilde{F}$, là một đồ thị, được gọi là đồ thị liên kết với quiver C. Tập hợp $A = F\times  \{1\}$ là một định hướng của đồ thị này. Ta nói rằng $(\widetilde{C},A)$ là đồ thị định hướng liên kết với quiver C.

Nếu $f$ là một mũi tên của C, ta cũng nói rằng $(f,1)$ là cạnh định hướng của $\widetilde{C}$ liên kết với $f$ và rằng cặp $\{(f,1),(f,-1)\}$ là cạnh của $\widetilde{C}$ liên kết với $f$.

Nếu $C'$ là một quiver con của C, đồ thị định hướng $\widetilde{C}'$ là một đồ thị con định hướng của $\widetilde{C}$.

Tồn tại một cấu xạ mũi tên duy nhất $\varphi$ từ C vào mũi tên nền của $\widetilde{C}$ sao cho $\varphi (f) = (f,1)$ đối với mọi mũi tên $f$ của G; nó là một đẳng cấu của C lên mũi tên liên kết với đồ thị có hướng $(\widetilde{C},A)$.

### 4. Cây

Khi nói về các đường đi, hoặc các thành phần liên thông, của một đồ thị, ta muốn nói đến các đường đi hoặc các thành phần liên thông của mũi tên nền. Hai đỉnh của một đồ thị thuộc cùng một thành phần liên thông khi và chỉ khi tồn tại một đường đi nối chúng.

Cho G là một đồ thị. Nếu $c= (a_0, f_1, a_1, . . . , f_n, a_n)$ là một đường đi trong G, dãy $\overline{c}= (a_n, f_n, . . . , a_1, f_1, a_0)$ là một đường đi trong G, được gọi là đường đi đối của $c$. Cho $c$ và $c'$ là các đường đi ghép trong G; khi đó $\overline{c'}$ và $\overline{c}$ là các đường đi ghép, và ta có $\overline{c*c'}=\overline{c'}*\overline{c}$.

Một đường đi $c$ trong G được gọi là không quay lại nếu không tồn tại cặp mũi tên liên tiếp nào của $c$ là đối nhau. Cho $c= (a_0, f_1, . . . , f_n, a_n)$ là một đường đi trong G nối $a_0$ và $a_n$. Nếu, với một số nguyên $i$ sao cho $1\leqslant i < n$, các mũi tên $f_i$ và $f_{i+1}$ là đối nhau, đường đi $(a_0, f_1, . . . , a_{i-1}, f_{i+2}, . . . , f_n, a_n)$ là một đường đi trong G nối $a_0$ với $a_n$ có độ dài nhỏ hơn một cách nghiêm ngặt độ dài của đường đi $c$. Bằng quy nạp, do đó tồn tại một đường đi không quay lại trong G nối $a_0$ với $a_n$.

#### Định nghĩa 2 {#ta-ii-s2-def-2 .statement tag=01SV}

Một rừng là một đồ thị trong đó mọi vòng không quay lại đều là một vòng hằng. Một cây là một rừng liên thông.

#### Mệnh đề 1 {#ta-ii-s2-prop-1 .statement tag=01SW}

Cho G là một đồ thị. Mọi rừng của G đều được chứa trong một rừng cực đại của G; đặc biệt, tồn tại một rừng cực đại của G.

Để một rừng của G là cực đại, điều kiện cần và đủ là tập hợp các đỉnh của nó bằng tập hợp các đỉnh của G và các thành phần liên thông của nó là các thành phần của G.

Cho $A_0$ là một rừng của G. Tập hợp các rừng của G, được trang bị quan hệ thứ tự “A là một đồ thị con của B”, là quy nạp. Do đó tồn tại một rừng cực đại của G mà $A_0$ là một đồ thị con (E, III, p. 21, Cor. 1).

Đồ thị con của G có tập hợp các đỉnh là Som(G) và có tập hợp các mũi tên là rỗng là một rừng của G. Do đó tồn tại một rừng cực đại của G.

Cho A là một rừng cực đại của G. Bây giờ chứng minh rằng A và G có cùng tập hợp các đỉnh. Đồ thị con của G có tập hợp các đỉnh là Som(G) và có tập hợp các mũi tên là Fl(A) là một rừng và có A là một đồ thị con. Do đó Som(A) = Som(G).

Bây giờ chứng minh rằng A và G có cùng các thành phần liên thông. Vì một mũi tên của A là một mũi tên của G, mọi thành phần liên thông của A được chứa trong một thành phần liên thông của G. Vì A và G có cùng tập hợp các đỉnh, chỉ cần chứng minh rằng hai đỉnh của G thuộc cùng một thành phần liên thông của G thì thuộc cùng một thành phần liên thông của A. Nếu không phải như vậy, quan hệ $R_A$, “thuộc cùng một thành phần liên thông của A”, là mịn hơn một cách nghiêm ngặt quan hệ $R_G$, và tồn tại hai đỉnh của G không thuộc cùng một thành phần liên thông của A nhưng tuy nhiên lại được nối bởi một mũi tên $f$ của G. Cho B là đồ thị con có hướng của G có tập hợp các đỉnh là Som(G) và có tập hợp các mũi tên là Fl(A) $\cup  \{f, f\}$; bây giờ chứng minh rằng B là một rừng của G. Cho $c= (a_0, f_1, . . . , f_n, a_n)$ là một vòng không hằng không quay lại trong B có độ dài cực tiểu. Vì A là một rừng, vòng $c$ không phải là một vòng trong A. Cho $i$ (tương ứng $j$) là số nguyên nhỏ nhất (tương ứng lớn nhất) của $\{0, . . . , n\}$ sao cho $a_0$ và $a_i$ (tương ứng $a_j$ và $a_n$) không thuộc cùng một thành phần liên thông của A. Điều này có nghĩa là các mũi tên $f_i$ và $f_{j+1}$ là các mũi tên có hướng của B liên kết với cạnh $\{f, f\}$ và chúng là đối nhau. Vì vòng $c$ không quay lại, $f_{i+1}=\not\overline{f_i}$, do đó $i=\not j$ và đường đi $(a_i, f_{i+1}, a_{i+1}, . . . , f_j, a_j)$ là một vòng không hằng không quay lại trong B có độ dài $< n$, mâu thuẫn với giả thiết rằng $c$ có độ dài cực tiểu. Suy ra B là một rừng. Điều này mâu thuẫn với giả thiết rằng A là một rừng cực đại của G.

Bây giờ cho A là một rừng của G sao cho Som(A) = Som(G) và $\pi_0(A) =\pi_0(G)$; ta chứng minh rằng nó là một rừng cực đại của G. Chỉ cần chứng minh rằng, nếu $f\notin$ Fl(A), thì đồ thị con B của G có tập các đỉnh là Som(G) và tập các mũi tên là Fl(A) $\cup  \{f, f\}$ không phải là một rừng. Theo giả thiết, các điểm $o(f)$ và $t(f)$ thuộc cùng một thành phần liên thông của A; do đó tồn tại một đường đi $c$ không quay ngược trong A nối $o(f)$ với $t(f)$. Khi đó đường đi $c*\overline{f}$ là một vòng không hằng không quay ngược trong B, điều này cho thấy B không phải là một rừng có hướng.

#### Hệ quả {#ta-ii-s2-n4-cor-1 .statement tag=01SX}

Một rừng cực đại của một đồ thị liên thông là một cây cực đại trong nó.

#### Nhận xét 1 {#ta-ii-s2-n4-rem-1 .statement tag=01SY}

Trong LIE, IV, p. 33, phụ lục, khái niệm đồ thị tổ hợp được định nghĩa là một cặp $(A,S)$, trong đó S là một tập hợp và A là một tập con của $\mathfrak{P}(S)$ gồm các tập hợp có hai phần tử; các phần tử của S được gọi là các đỉnh, các phần tử của A được gọi là các cạnh, và hai đỉnh $x$ và $y\in S$ được gọi là được nối với nhau nếu $\{x, y\}$ là một cạnh.

Với một đồ thị tổ hợp $\Gamma  = (A,S)$ như vậy, ta liên kết một đồ thị G có tập các đỉnh là S và tập các mũi tên $\widetilde{A}$ là tập con của $S^2$ gồm các cặp đỉnh được nối với nhau, ánh xạ gốc và ánh xạ ngọn trùng với các phép chiếu thứ nhất và thứ hai của $S^2$ lên S, và phép đối hợp $f\mapsto \overline{f}$ được cho bởi hạn chế vào $\widetilde{A}$ của ánh xạ $(x, y)\mapsto (y, x)$ của $S^2$ vào chính nó. Ánh xạ liên kết với một cạnh $\{f, f\}$ của G tập hợp $\{o(f), t(f)\}$ là một song ánh từ tập các cạnh của G lên tập các cạnh của đồ thị tổ hợp Γ.

Ngược lại, mọi đồ thị sao cho gốc và ngọn của mọi mũi tên là phân biệt, và sao cho một mũi tên được xác định bởi gốc và ngọn của nó, đều có dạng này.

Người đọc sẽ kiểm tra rằng các khái niệm về tính liên thông, cây và rừng đối với một đồ thị tổ hợp trùng với các khái niệm tương ứng đối với đồ thị liên kết với nó.

## BÀI TẬP {#ta-ii-s2-exercises}

Xem [các bài tập cho § 2](exercises/s2/).

[^1]: Cần chú ý không nhầm lẫn khái niệm đồ thị được đưa vào đây với khái niệm trong E, II, §3, n$^o1$.
