---
book: ta
book_title: Topologie algébrique
chapter: III
chapter_title: HOMOTOPIE ET GROUPOÏDE DE POINCARÉ
section: 5
section_title: Homotopie et revêtements (cas des espaces localement connexes par arcs)
lang: vi
source: ta-i-iv-fr
book_pages: TA III.308-TA III.320, TA III.334-TA III.338
pdf_pages: 0324-0336, 0350-0354
extraction: native
subsections:
    - "no": 1
      title: Condition homotopique de relèvement des applications continues
      page: 308
      pdf_page: 324
    - "no": 2
      title: Opérations du groupe de Poincaré et morphismes de revêtements
      page: 310
      pdf_page: 326
    - "no": 3
      title: Opérations sans monodromie locale du groupoïde de Poincaré
      page: 312
      pdf_page: 328
    - "no": 4
      title: Topologie admissible des groupes de Poincaré
      page: 315
      pdf_page: 331
statements: 23
exercises: 10
content_sha256: a263eb543f9ca02d68000d5c098fb7f0c313b220ffab170b0581bbb48803497e
translated_from: content/en-mt/ta/III/05_s5_homotopie_et_revetements_cas_des.md
source_lang: en-mt
translation_method: machine
source_content_sha256: 3e9437934d252802ed8ffe4dc4e1276f2b4d6a063e837e3327e57c7807a6245d
translation_model: gpt-5-6-mini
translation_run: translate-vi-1e0c2743
glossary_version: 34
glossary_terms_sha256: 5029cd0c09a84fcc323b6366697403af97259b809ca8e0c076babf3abde9b612
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 5. ĐỒNG LUÂN VÀ CÁC PHép PHỦ (TRƯỜNG HỢP CÁC KHÔNG GIAN LIÊN THÔNG CUNG ĐỊA PHƯƠNG)

### 1. Điều kiện đồng luân để nâng các ánh xạ liên tục

#### Mệnh đề 1 {#ta-iii-s5-prop-1 .statement tag=01ZL}

Cho B là một không gian tôpô và cho $(E, p)$ là một phép phủ của B. Cho Y là một không gian tôpô và cho $f: Y\rightarrow B$ là một ánh xạ liên tục. Cho $y\in$ Y$,x\in$ E$,b\in$ B là các điểm sao cho $f(y) =p(x) =b$. Giả sử không gian Y liên thông và liên thông cung địa phương. Để tồn tại một ánh xạ nâng liên tục $g: Y\rightarrow E$ của $f$ sao cho $g(y) =x$, điều kiện cần và đủ là ảnh của đồng cấu $\pi_1(f, y):\pi_1(Y, y)\rightarrow \pi_1(B, b)$ được chứa trong ảnh của đồng cấu $\pi_1(p, x):\pi_1(E, x)\rightarrow \pi_1(B, b)$.

Điều kiện này là cần mà không cần bất kỳ giả thiết nào về không gian Y. Thật vậy, nếu một ánh xạ nâng $g$ như vậy tồn tại, ta có $\pi_1(f, y) =\pi_1(p, x)\circ \pi_1(g, y)$.

Hãy chứng minh rằng điều kiện này là đủ. Gọi $s: \Lambda_b(B)\rightarrow \Lambda_x(E)$ là đồng phôi nghịch đảo của đồng phôi $c\mapsto p\circ c($III, p. 302, hệ quả 2 của mệnh đề 3) và gọi $\varphi : \Lambda_y(Y)\rightarrow \Lambda_x(E)$ là ánh xạ $d\mapsto$ $s(f\circ d)$. Ánh xạ $\varphi$ là liên tục (I, p. 132, bổ đề).

Cho $d$ và $d'\in \Lambda_y(Y)$ là các đường đi có gốc $y$ có cùng số hạng; hãy chứng minh rằng các đường đi $\varphi (d)$ và $\varphi (d')$ có cùng số hạng. Đặt $c=f\circ d,c'=f\circ d'$. Vì đường đi $d*\overline{d'}$ là một vòng trong Y tại $y$, đường đi $c*\overline{c'}$ là một vòng trong B tại $b$ và lớp của nó thuộc về ảnh của đồng cấu $\pi_1(f, y)$, do đó thuộc về ảnh của đồng cấu $\pi_1(p, x)$ theo giả thiết. Theo hệ quả 2 của mệnh đề 4 (III, p. 303), đường đi $s(c*\overline{c'})$ là một vòng trong E tại $x$. Điều tương tự cũng đúng với đường đi $s(c'*\overline{c})$, đường đi này, do tính duy nhất của phép nâng các đường đi, bằng $s(c*\overline{c'})$. Do đó $s(c'*\overline{c})(\frac{1}{2}) =s(c')(1) =s(c)(1)$, như cần chứng minh.

Ta ký hiệu lần lượt bởi $e_E: \Lambda_x(E)\rightarrow E$ và $e_Y: \Lambda_y(Y)\rightarrow Y$ các ánh xạ số hạng. Vì không gian Y được giả sử là liên thông và liên thông cung địa phương, ánh xạ $e_Y$ là toàn ánh và mở (III, p. 262, mệnh đề 10). Theo đoạn trước, tồn tại một ánh xạ duy nhất $g: Y\rightarrow E$ sao cho $e_E\circ \varphi =g\circ e_Y$. Nó là liên tục, vì ánh xạ $e_Y$ là ngặt ( I, p. 18, ví dụ 2).

Cuối cùng hãy kiểm tra rằng ánh xạ $g$ nâng ánh xạ $f$ và rằng $g(y) =x$. Mọi điểm $z$ của Y là số hạng của một đường đi $c$ có gốc $y$. Đường đi $\varphi (c)$ là một phép nâng của $f\circ c$ có gốc $x$ và có số hạng là điểm $g(z)$. Do đó $p(g(z)) =f(z)$. Với $z=y$ và $c=e_y$, ta có $\varphi (e_y) =e_x$, do đó $g(y) =x$.

#### Hệ quả 1 {#ta-iii-s5-prop-1-cor-1 .statement tag=01ZM}

Cho B là một không gian tôpô liên thông, địa phương liên thông bởi các đường đi, và $b$ là một điểm của B. Để một phủ $(E, p)$ của B là tầm thường hóa được, điều kiện cần và đủ là, với mọi điểm $x$ của thớ $E_b$, đồng cấu $\pi_1(p, x)$ là song ánh.

Nhắc lại rằng đồng cấu $\pi_1(p, x)$ là đơn ánh (III, p. 303, hệ quả 1 của mệnh đề 4). Do đó mệnh đề này suy ra từ mệnh đề 1 và I, p. 81, hệ quả 4 của mệnh đề 6.

#### Nhận xét {#ta-iii-s5-n1-rem-1 .statement tag=01ZN}

Cho B là một không gian tôpô địa phương liên thông bởi các đường đi, $b$ là một điểm của B, và V là một lân cận mở liên thông của $b$ sao cho ảnh của đồng cấu từ $\pi_1(V, b)$ vào $\pi_1(B, b)$ là nhóm con rút gọn về phần tử đơn vị. Theo hệ quả 1, mọi phủ của B đều tầm thường hóa được trên V, và a fortiori trên mọi tập con của B được chứa trong V.

#### Hệ quả 2 {#ta-iii-s5-prop-1-cor-2 .statement tag=01ZO}

Cho B là một không gian tôpô liên thông, địa phương liên thông bởi các đường đi. Nếu, với một điểm $b$ của B, nhóm $\pi_1(B, b)$ rút gọn về phần tử đơn vị, thì không gian B đơn liên.

Thật vậy, theo hệ quả 1, dưới các giả thiết này, mọi phủ của B đều tầm thường hóa được.

#### Hệ quả 3 {#ta-iii-s5-prop-1-cor-3 .statement tag=01ZP}

Cho

${E'}^{f'}$ E

$p'p$

${B'}^f$ B

là một bình phương Descartes. Giả sử E là một phủ của B và không gian $B'$ liên thông và địa phương liên thông bởi các đường đi. Cho $b'$ là một điểm của $B'$ và $b=f(b')$. Để $(E', p')$ là một phủ tầm thường hóa được của $B'$, điều kiện cần và đủ là, với mọi điểm $x$ của thớ $E_b$, ảnh của $\pi_1(p, x)$ chứa ảnh của $\pi_1(f, b)$.

Điều này suy ra từ mệnh đề 1 và I, p. 81, hệ quả 5 của mệnh đề 6.

### 2. Các phép toán của nhóm Poincaré và các cấu xạ của các phủ

Cho B là một không gian tôpô liên thông, địa phương liên thông bởi các đường đi và $b$ là một điểm của B.

Cho E là một phủ của B. Vì không gian B được giả thiết là liên thông, thớ $E_b$ khác rỗng nếu E khác rỗng (I, p. 74, mệnh đề 4). Theo mệnh đề a) của định lý 1 của III, p. 305, phủ E liên thông và khác rỗng khi và chỉ khi nhóm $\pi_1(B, b)$ tác động bắc cầu trên $E_b$.

#### Mệnh đề 2 {#ta-iii-s5-prop-2 .statement tag=01ZQ}

Cho E và $E'$ là các phủ của B.

a) Cho $f: E\rightarrow E'$ là một cấu xạ B. Ánh xạ $f_b: E_b\rightarrow E'_b$ dẫn xuất từ f tương thích với các phép toán của $\pi_1(B, b)$ trên $E_b$ và $E'_b$ tương ứng. Nó là song ánh khi và chỉ khi f là một đẳng cấu.

b) Ánh xạ $f\mapsto f_b$ là một song ánh từ tập hợp $\mathscr{C}_B(E; E')$ các cấu xạ B từ E vào $E'$ lên tập hợp $\mathscr{F}_{\pi_1(B,b)}(E_b; E'_b)$ các cấu xạ $\pi_1(B, b)$ từ $E_b$ vào $E'_b$.

Nếu f là một cấu xạ B từ E vào $E'$, thì ánh xạ $f_b: E_b\rightarrow E'_b$ là một cấu xạ $\pi_1(B, b)$ (xem III, p. 305). Hơn nữa, hai cấu xạ B từ E vào $E'$ trùng nhau trên thớ $E_b$ thì bằng nhau (I, p. 80, hệ quả 3 của mệnh đề 6).

Cho $\varphi : E_b\rightarrow E'_b$ là một cấu xạ của các $\pi_1(B, b)$-tập hợp; ta hãy chứng minh rằng tồn tại một cấu xạ B $f$ của E vào $E'$ sao cho $f_b=\varphi$. Ta có thể giả sử rằng các không gian E và $E'$ là liên thông và không rỗng, do đó $E_b$ và $E'_b$ là các $\pi_1(B, b)$-tập hợp thuần nhất. Cho $x$ là một điểm của $E_b$; nhóm ổn định của nó G là ảnh của ánh xạ $\pi_1(p, x)$ (III, p. 305, Định lý 1). Vì ánh xạ $\varphi$ là một $\pi_1(B, b)$-cấu xạ, nhóm G cố định điểm $x'=\varphi (x)$ của $E'_b$, và do đó được chứa trong ảnh của ánh xạ $\pi_1(p', x')$. Theo Mệnh đề 1 của III, p. 308, tồn tại một cấu xạ B $f$ của E vào $E'$ sao cho $f(x) =x'$. Các ánh xạ $f_b$ và $\varphi$ là các $\pi_1(B, b)$-cấu xạ từ $\pi_1(B, b)$-tập hợp thuần nhất $E_b$ vào $E'_b$ trùng nhau tại điểm $x$; do đó chúng bằng nhau.

Nếu $f: E\rightarrow E'$ là một đẳng cấu B, ánh xạ $f_b: E_b\rightarrow E'_b$ là song ánh. Ngược lại, giả sử rằng ánh xạ $f_b$ là song ánh, và cho $g: E'\rightarrow$ E là một cấu xạ B sao cho $g_b= (f_b)^{-1}$. Cấu xạ B $g\circ f: E\rightarrow E$ cảm sinh trên $E_b$ ánh xạ đồng nhất; do đó suy ra từ mệnh đề rằng $g\circ f=$ Id$_E$. Tương tự, $f\circ g=$ Id$_{E'}$, điều này chứng minh rằng $f$ là một đẳng cấu B.

#### Hệ quả 1 {#ta-iii-s5-prop-2-cor-1 .statement tag=01ZR}

Các phủ E và $E'$ đẳng cấu khi và chỉ khi các $\pi_1(B, b)$-tập hợp $E_b$ và $E'_b$ đẳng cấu.

#### Hệ quả 2 {#ta-iii-s5-prop-2-cor-2 .statement tag=01ZS}

Cho $(E, p)$ và $(E', p')$ là các phủ liên thông của B. Cho $x$ là một điểm của $E_b$ và $x'$ là một điểm của $E'_b$. Để tồn tại một cấu xạ B $g: E\rightarrow E'$ sao cho $g(x) =x'$, điều kiện cần và đủ là ta có $p_*(\pi_1(E, x))\subset p'_*(\pi_1(E', x'))$. Một cấu xạ như vậy là duy nhất, và là một đẳng cấu khi và chỉ khi các nhóm con $p_*(\pi_1(E, x))$ và $p'_*(\pi_1(E', x'))$ của $\pi_1(B, b)$ bằng nhau.

Theo III, p. 305, Định lý 1, ánh xạ của $\pi_1(B, b)$ lên $E_b$ được xác định bởi $\gamma \mapsto x\cdot \gamma$ cảm sinh qua chuyển qua thương một đẳng cấu của $\pi_1(B, b)$-tập hợp $p_*(\pi_1(E, x))\backslash \pi_1(B, b)$ lên $E_b$. Tương tự, tồn tại một đẳng cấu duy nhất của các $\pi_1(B, b)$-tập hợp $p_*(\pi_1(E', x'))\backslash \pi_1(B, b)$ lên $E'_b$. Theo Mệnh đề 2, tồn tại một cấu xạ B $g: E\rightarrow E'$ sao cho $g(x) =x'$ khi và chỉ khi tồn tại một cấu xạ của các $\pi_1(B, b)$-tập hợp từ $p_*(\pi_1(E, x))\backslash \pi_1(B, b)$ lên $p'_*(\pi_1(E', x'))\backslash \pi_1(B, b)$ gửi lớp $p_*(\pi_1(E, x))$ lên lớp $p'_*(\pi_1(E', x'))$. Một cấu xạ như vậy tồn tại khi và chỉ khi có $p_*(\pi_1(E, x))\subset p'_*(\pi_1(E', x'))$. Khi đó nó là duy nhất, vì không gian E được giả thiết là liên thông (I, p. 34, hệ quả 2 của mệnh đề 11). Nó là một đẳng cấu khi và chỉ khi các nhóm con $p_*(\pi_1(E, x))$ và $p'_*(\pi_1(E', x'))$ của $\pi_1(B, b)$ bằng nhau.

#### Hệ quả 3 {#ta-iii-s5-prop-2-cor-3 .statement tag=01ZT}

Cho $(E, p)$ là một phủ liên thông của B và cho $x$ là một điểm của thớ $E_b$. Gọi N là chuẩn hóa tử của $p_*(\pi_1(E, x))$ trong $\pi_1(B, b)$. Với mọi phần tử $\gamma$ của N, tồn tại một tự đẳng cấu B duy nhất $g$ của E sao cho $g(x) =x\cdot \gamma$, và ánh xạ $\gamma \mapsto g$ xác định qua chuyển qua thương một đẳng cấu nhóm của $N/p_*(\pi_1(E, x))$ lên Aut$_B(E)$.

Cho $\gamma \in \pi_1(B, b)$; ta có $p_*(\pi_1(E, x)) =$ Int($\gamma$ )$(p_*(\pi_1(E, x\cdot \gamma )))$ (III, p. 305, Định lý 1, c)). Theo Hệ quả 2, để tồn tại một tự đẳng cấu B $g$ của E sao cho $g(x) =x\cdot \gamma$, điều kiện cần và đủ là $\gamma$ thuộc N. Một đẳng cấu như vậy là duy nhất. Gọi $\alpha : N\rightarrow$ Aut$_B(E)$ là ánh xạ $\gamma \mapsto g$ được xác định như trên.

Cho $\gamma$ và $\gamma '$ là hai phần tử của N. Đặt $g=\alpha (\gamma ),g'=\alpha (\gamma ')$; ta có $g(g'(x)) =g(x\cdot \gamma ') =g(x)\cdot \gamma '= (x\cdot \gamma )\cdot \gamma '=x\cdot (\gamma \gamma ')$ theo các quan hệ (4), III, p. 305 và (1), p. 304. Do đó, $\alpha$ là một đồng cấu nhóm. Để $\alpha (\gamma ) =$ Id$_E$, điều kiện cần và đủ là có $x\cdot \gamma =x$, theo tính duy nhất của $\alpha (\gamma )$, nghĩa là $\gamma \in p_*(\pi_1(E, x))$ (III, p. 305, Định lý 1, b)). Cuối cùng, nếu $g$ là một tự đẳng cấu B của E, tồn tại một đường đi $c$ nối $x$ với $g(x)$ trong E (vốn liên thông theo cung), và khi đó có $g(x) =x\cdot \gamma$, trong đó $\gamma$ là lớp của đường đi $p\circ c$. Điều này chứng minh rằng đồng cấu $\alpha$ là toàn ánh.

Nhóm Aut$_B(E)$ tác động trên thớ $E_b$ và được đồng nhất với nhóm tự đẳng cấu của tập hợp thuần nhất (phải) $\pi_1(B, b)$-tập hợp $E_b($cf. A, I, p. 56, mệnh đề 5 và 6).

#### Hệ quả 4 {#ta-iii-s5-prop-2-cor-4 .statement tag=01ZU}

Cho $(E, p)$ là một phủ liên thông của B và cho $x$ là một điểm của thớ $E_b$. Để E là một phủ Galois của B, điều kiện cần và đủ là $p_*(\pi_1(E, x))$ là một nhóm con đặc biệt của $\pi_1(B, b)$. Khi đó nhóm Aut$_B(E)$ đẳng cấu với nhóm thương $\pi_1(B, b)/p_*(\pi_1(E, x))$.

Nếu $p_*(\pi_1(E, x))$ là một nhóm con đặc biệt của $\pi_1(B, b)$, nhóm Aut$_B(E)$ tác động bắc cầu trên thớ $E_b$ theo Hệ quả 3, do đó E là một phủ Galois của B (I, p. 102, định lý 2). Đảo lại là mệnh đề d) của Định lý 1 (III, p. 305). Khẳng định cuối cùng suy ra từ Hệ quả 3.

### 3. Các phép toán không có đơn trị địa phương của groupoid Poincaré

#### Bổ đề 1 {#ta-iii-s5-lem-1 .statement tag=01ZV}

Cho B là một không gian tôpô liên thông địa phương bởi các đường, cho $p: E\rightarrow B$ và $p': E'\rightarrow B$ là các ánh xạ étale và tách thỏa mãn tính chất nâng đường (III, p. 302). Cho $g: E\rightarrow E'$ là một ánh xạ sao cho $p'\circ g=p$. Giả sử rằng $g$ tương thích với các phép toán chính tắc của groupoid $\varpi (B)$ trên E và $E'$. Khi đó $g$ liên tục.

Cho $c$ là một đường trong E; đặt $c'=g\circ c$ và chứng minh rằng ánh xạ $c'$ là liên tục. Gọi $d$ là đường $p\circ c$ trong B và, với mọi $t\in \mathbf{I}$, gọi $d_t$ là đường $s\mapsto d(st)$. Với mọi $t\in \mathbf{I}$, ta có $c(t) =c(0)\cdot d_t($III, p. 304, nhận xét 3), do đó $c'(t) =c'(0)\cdot d_t$ theo giả thiết đã đặt ra trên $g$, điều này chứng minh rằng $c'$ là một đường nâng đường $d$, theo cùng nhận xét. Điều này chứng minh rằng ánh xạ $g$ là liên tục theo đường. Vì không gian E liên thông địa phương bởi các đường (III, p. 261, hệ quả 2), ánh xạ $g$ là liên tục (III, p. 269, hệ quả của mệnh đề 13).

Cho B là một không gian tôpô. Xét một phép toán $\varphi$ = $(\varphi_{a,b})_{(a,b)\in B\times B}$ của groupoid $\varpi (B)$ trên một tập hợp E, tương đối với một ánh xạ $p: E\rightarrow B$. Người ta nói rằng $\varpi (B)$ tác động không có đơn trị trên E (cf. II, p. 168) nếu với mọi $b\in$ B và mọi lớp các vòng $\gamma \in \pi_1(B, b)$, tác động của $\gamma$ trên thớ $E_b$ là tầm thường. Nếu B liên thông bởi các đường, chỉ cần điều này đúng với một điểm của B là đủ (loc. cit.). Ta sẽ nói rằng phép toán $\varphi$ của groupoid $\varpi (B)$ không có đơn trị địa phương nếu mọi điểm của B đều có một lân cận V sao cho $\varpi (V)$ tác động không có đơn trị trên tập hợp $E_V$ = $\overset{-1}{p}(V)$ tương đối với ánh xạ $p_V=p|\overset{-1}{p}(V)$.

#### Nhận xét {#ta-iii-s5-n3-rem-1 .statement tag=01ZW}

Cho B là một không gian tôpô liên thông địa phương bởi các đường và giả sử rằng mọi điểm $b$ của B đều có một lân cận V sao cho ảnh của $\pi_1(V, b)$ trong $\pi_1(B, b)$ thu gọn thành phần tử đơn vị (cf. IV, p. 340, định nghĩa 2). Khi đó mọi phép toán của groupoid $\varpi (B)$ đều không có đơn trị địa phương.

Thật vậy, xét một tập hợp E, một ánh xạ $p: E\rightarrow B$ và một phép toán $\varphi$ của nhómoid $\varpi (B)$ trên E tương đối với $p$. Cho $a$ là một điểm của B và cho V là một lân cận của $a$ sao cho ảnh của $\pi_1(V, a)$ trong $\pi_1(B, a)$ thu gọn về phần tử đơn vị. Cho U là một lân cận liên thông đường của $a$ được chứa trong V. Cho $b$ là một điểm của U và cho $\gamma \in \pi_1(U, b)$. Cho $\delta$ là lớp của một đường đi nối $a$ với $b$ trong U. Khi đó $\delta \gamma \delta^{-1}$ là lớp của một vòng tại $a$ trong U; ảnh của nó trong $\pi_1(B, a)$ do đó là tầm thường. Vì vậy $\varphi_{a,a}(\delta \gamma \delta^{-1}) =$ Id$_{E_a}$, do đó $\varphi_{b,b}(\gamma ) =$ Id$_{E_b}$. Điều này chứng minh rằng phép toán của $\varpi (U)$ trên không gian U $E_U$ là không có đơn trị. Do đó, phép toán $\varphi$ là không có đơn trị địa phương.

#### Mệnh đề 3 {#ta-iii-s5-prop-3 .statement tag=01ZX}

Cho B là một không gian tôpô liên thông đường địa phương và cho E là một tập hợp được trang bị một phép toán không có đơn trị địa phương $\varphi$ của nhómoid $\varpi (B)$, tương đối với một ánh xạ $p: E\rightarrow B$. Khi đó tồn tại trên E một tôpô duy nhất sao cho các điều kiện sau được thỏa mãn:

(i) Tập hợp E được trang bị tôpô này và ánh xạ $p$ là một phép phủ của B;

(ii) Phép toán chính tắc của $\varpi (B)$ trên phép phủ này đồng nhất với phép toán $\varphi$.

Tính duy nhất của một tôpô như vậy suy ra từ bổ đề 1 của III, p. 312, trong đó lấy $g$ là ánh xạ đồng nhất của E. Để chứng minh sự tồn tại của nó, hơn nữa ta có thể giả sử rằng B là liên thông và khác rỗng.

Trước hết, giả sử rằng phép toán $\varphi = (\varphi_{a,b})_{(a,b)\in B\times B}$ của nhómoid $\varpi (B)$ trên tập hợp E, tương đối với $p$, là không có đơn trị.

Cho $a$ là một điểm của B. Với mỗi điểm $b\in B$, tồn tại một đường đi $c$ trong B nối $a$ với $b$. Nếu $\gamma \in \varpi_{a,b}(B)$ là lớp của đường đi $c$, thì song ánh $\varphi_{a,b}(\gamma ): E_a\rightarrow E_b$ độc lập với đường đi $c$, vì phép toán là không có đơn trị; ký hiệu $f_{a,b}$ là song ánh này. Ánh xạ $\Phi_a: B\times E_a\rightarrow$ E được xác định bởi $(b, x)\mapsto f_{a,b}(x)$ là một song ánh; song ánh ngược liên kết với $x\in E$ cặp $(p(x), f_{p(x),a}(x))$. Trang bị cho tập hợp $E_a$ tôpô rời rạc, sao cho không gian B $B\times E_a$ là một phép phủ tầm thường của B. Bằng phép chuyển cấu trúc, song ánh $\Phi_a$ trang bị cho E một tôpô làm cho nó trở thành một phép phủ của B.

Ta chứng minh rằng phép toán chính tắc của $\varpi (B)$ trên E trùng với phép toán $\varphi$. Cho $x$ là một điểm của $E_a$ và $b$ là một điểm của B. Cho $c$ là một đường trong B nối điểm $a$ với điểm $b$; ánh xạ $t\mapsto \Phi_a(c(t), x)$ khi đó là một đường trong E nối điểm $x$ với điểm $\Phi_a(b, x) =f_{a,b}(x)$. Nếu $\gamma \in \varpi_{a,b}(B)$ biểu thị lớp của đường $c$, thì ta có $x\cdot \gamma =f_{a,b}(x)$. Điều này chứng minh rằng phép toán chính tắc của $\varpi (B)$ trên phủ E và phép toán $\varphi$ trùng nhau trên các lớp của những đường có gốc $a$. Vì các lớp này sinh ra groupoid $\varpi (B)$, nên hai phép toán bằng nhau.

Bây giờ ta xét trường hợp tổng quát. Cho $\mathscr{B}$ là tập hợp các tập con mở V của E sao cho $\varpi (V)$ tác động không có đơn điều trên $\overset{-1}{p}(V)$. Theo giả thiết, các phần tử của $\mathscr{B}$ phủ B. Theo điều đã chứng minh ở trên, với mỗi $V\in \mathscr{B}$ tồn tại một tôpô duy nhất trên tập hợp $\overset{-1}{p}(V)$ sao cho $(\overset{-1}{p}(V), p_V)$ là một phủ của V và phép toán chính tắc của $\varpi (V)$ trên phủ này trùng với phép toán cảm sinh bởi $\varphi$.

Cho V và $V'\in \mathscr{B}$. Tôpô trên $\overset{-1}{p}(V\cap V')$ cảm sinh bởi tôpô của $\overset{-1}{p}(V)$ (tương ứng của $\overset{-1}{p}(V')$) đã xác định ở trên biến nó thành một phủ của $V\cap V'$ trên đó phép toán chính tắc của $\varpi (V\cap V')$ được cảm sinh bởi phép toán $\varphi$. Do đó các tôpô này trùng với tôpô của $\overset{-1}{p}(V\cap V')$. Khi đó tồn tại một tôpô duy nhất trên E cảm sinh trên mỗi $\overset{-1}{p}(V)$ tôpô đã xác định trước đó (xem I, § 2, p. 16).

Khi E được trang bị tôpô này, ánh xạ $p$ là liên tục và không gian B E là một phủ. Phép toán chính tắc của $\varpi (B)$ trên phủ này trùng với phép toán $\varphi$ trên các lớp của những đường mà ảnh được chứa trong một trong các tập mở của $\mathscr{B}$. Theo bổ đề 4 của III, p. 272, các lớp này sinh ra groupoid $\varpi (B)$. Suy ra rằng hai phép toán này bằng nhau (II, p. 167).

#### Hệ quả {#ta-iii-s5-n3-cor-1 .statement tag=01ZY}

Cho B là một không gian tôpô liên thông, liên thông địa phương bởi các cung, cho $(E, p)$ là một không gian B mà phép chiếu $p$ là étale, tách được, và có tính chất nâng đường. Nếu phép toán chính tắc của $\varpi (B)$ trên tập hợp E, đối với $p$, là không có đơn điều địa phương, thì E là một phủ của B.

Trang bị cho E phép toán chính tắc của $\varpi (B)$ được xác định bởi phép nâng đường (III, p. 303, n$^o3$). Tồn tại một tôpô trên E sao cho các điều kiện (i) và (ii) của mệnh đề 3 được thỏa mãn. Tôpô này trùng với tôpô đã cho trên E theo bổ đề 1 của III, p. 312.

### 4. Tôpô khả nạp của các nhóm Poincaré

Cho B là một không gian tôpô và cho $a$ là một điểm của B. Một nhóm con H của $\pi_1(B, a)$ được gọi là khả nạp nếu mọi điểm $b$ của B có một lân cận V sao cho ta có $\gamma i_*(\delta )\gamma^{-1}\in H$ với mọi $\gamma \in \varpi_{a,b}(B)$ và mọi $\delta \in \pi_1(V, b)$, trong đó $i: V\rightarrow$ B là đơn ánh chính tắc. Nếu H là một nhóm con chuẩn của $\pi_1(B, a)$, thì để H khả nạp, chỉ cần điều kiện này được thỏa mãn đối với một lớp đường $\gamma \in \varpi_{a,b}(B)$.

#### Mệnh đề 4 {#ta-iii-s5-prop-4 .statement tag=01ZZ}

Tồn tại một tôpô duy nhất trên $\pi_1(B, a)$, tương thích với cấu trúc nhóm của nó, sao cho các nhóm con chuẩn khả nạp của $\pi_1(B, a)$ tạo thành một hệ cơ bản các lân cận của phần tử đơn vị. Đối với tôpô này, các nhóm con mở chính là các nhóm con khả nạp.

Các sự kiện sau đây suy ra từ định nghĩa của một nhóm con khả nạp:

a) Nhóm $\pi_1(B, a)$ là khả nạp;

b) Một nhóm con chứa một nhóm con khả nạp là khả nạp;

c) Giao của một họ hữu hạn các nhóm con khả nạp là khả nạp;

d) Đối với mọi nhóm con chấp nhận được H của $\pi_1(B, a)$, giao của các nhóm con $\gamma H\gamma^{-1}$, khi $\gamma$ chạy qua $\pi_1(B, a)$, là chấp nhận được. Đặc biệt, tập hợp các nhóm con chuẩn chấp nhận được là một cơ sở lọc được tạo thành bởi các nhóm con của $\pi_1(B, a)$ thỏa mãn tiên đề (GV$'_{III}$) của III, p. 4, do đó phần thứ nhất của mệnh đề sau TG, III, p. 5, ví dụ. Phần thứ hai khi đó là ngay lập tức (xem TG, III, p. 7, hệ quả của mệnh đề 4).

Tôpô trên nhóm $\pi_1(B, a)$ được đặc trưng trong mệnh đề 4 được gọi là tôpô chấp nhận được.

#### Nhận xét 1 {#ta-iii-s5-n4-rem-1 .statement tag=0200}

Nếu $B_0$ ký hiệu thành phần liên thông đường đi của $a$ trong B, thì đẳng cấu chính tắc $\pi_1(B_0, a)\rightarrow \pi_1(B, a)$ là một đẳng cấu của các nhóm tôpô khi các nhóm này được trang bị tôpô chấp nhận được.

#### Nhận xét 2 {#ta-iii-s5-n4-rem-2 .statement tag=0201}

Cho B là một không gian tôpô. Cho $b$ và $b'$ là các điểm của B thuộc cùng một thành phần liên thông đường đi và cho $\gamma$ là một phần tử của $\varpi_{b,b'}(B)$. Từ định nghĩa của một nhóm con chấp nhận được suy ra rằng, đối với mọi nhóm con chấp nhận được H của $\pi_1(B, b')$, nhóm con $\gamma H\gamma^{-1}$ của $\pi_1(B, b)$ là chấp nhận được. Do đó, đẳng cấu $u_{\gamma}:\delta \mapsto \gamma \delta \gamma^{-1}$ của $\pi_1(B, b')$ lên $\pi_1(B, b)$ (xem III, p. 292) là một đồng phôi khi các nhóm này được trang bị các tôpô chấp nhận được.

#### Nhận xét 3 {#ta-iii-s5-n4-rem-3 .statement tag=0202}

Cho A và B là các không gian tôpô, cho $a$ là một điểm của A, và cho $f: A\rightarrow B$ là một ánh xạ liên tục. Đặt $b=f(a)$. Nếu H là một nhóm con chấp nhận được của $\pi_1(B, b)$, ảnh ngược của nó qua đồng cấu $\pi_1(f, a)$ là một nhóm con chấp nhận được của $\pi_1(A, a)$. Do đó, đồng cấu nhóm $\pi_1(f, a):\pi_1(A, a)\rightarrow \pi_1(B, b)$ là liên tục, khi các nhóm này được trang bị tôpô chấp nhận được.

#### Mệnh đề 5 {#ta-iii-s5-prop-5 .statement tag=0203}

Cho B là một không gian tôpô liên thông địa phương theo cung, và cho $a$ là một điểm của B. Để một nhóm con H của $\pi_1(B, a)$ là chấp nhận được, điều kiện cần và đủ là tồn tại một phủ $(E, p)$ của B và một điểm $x\in E_a$ sao cho $H =p_*(\pi_1(E, x))$.

Cho $(E, p)$ là một phủ của B và cho $x$ là một điểm của $E_a$; đặt $H =p_*(\pi_1(E, x))$ và ta hãy chứng minh rằng đây là một nhóm con chấp nhận được của $\pi_1(B, a)$. Cho $b$ là một điểm của B và cho V là một lân cận của $b$ sao cho $E_V=$ $(\overset{-1}{p}(V), p_V)$ là một phủ tầm thường hóa được của V. Cho $\gamma \in \varpi_{a,b}(B)$ ; ta sẽ chứng minh rằng đối với mọi phần tử $\delta \in \pi_1(V, b)$, lớp các đường $\gamma \delta \gamma^{-1}$ thuộc H.

Theo III, p. 301, mệnh đề 3, tồn tại duy nhất một lớp đồng luân ngặt $\gamma '$ của đường có gốc $x$ trong E sao cho $p_*(\gamma ') =\gamma$ Cho $y$ là điểm cuối của $\gamma '$; ta có $p(y) =b($III, p. 302, mệnh đề 4). Khi đó cho $\delta '$ là lớp đường duy nhất có gốc $y$ trong E sao cho $p_*(\delta ') =\delta$. Vì $E_V$ là tầm thường hóa được, $\delta '$ là lớp của một vòng tại $y$. Khi đó $\gamma '\delta '(\gamma ')^{-1}$ là lớp của một vòng tại $a$ trong E mà ảnh của nó qua $p_*$ là lớp $\gamma \delta \gamma^{-1}$, điều phải chứng minh.

Ngược lại, cho H là một nhóm con khả chấp nhận của $\pi_1(B, a)$. Cho $\lambda_a(B)$ là thương của không gian $\Lambda_a(B)$ gồm các đường đi có gốc $a$ theo quan hệ đồng luân ngặt; vì hai đường đi đồng luân ngặt có cùng điểm cuối, ánh xạ điểm cuối $e: \Lambda_a(B)\rightarrow B$ xác định, bằng cách chuyển qua thương, một ánh xạ $\varepsilon :\lambda_a(B)\rightarrow B$. Phép hợp thành của các lớp đường đi trang bị cho tập hợp $\lambda_a(B)$ một tác động trái của nhóm $\pi_1(B, a)$. Trang bị cho nó tác động của nhóm H suy ra bởi hạn chế, và ký hiệu $H\backslash \lambda_a(B)$ là tập hợp các quỹ đạo của nó.

Ánh xạ $\varepsilon :\lambda_a(B)\rightarrow B$ cảm sinh, bằng cách chuyển qua thương, một ánh xạ $q: H\backslash \lambda_a(B)\rightarrow B$. Phép hợp thành của các lớp đường đi trang bị cho tập hợp $H\backslash \lambda_a(B)$ một phép toán phải của nhómoid $\varpi (B)$ tương đối với ánh xạ $q$.

Phép toán này không có đơn tạp địa phương. Thật vậy, cho $b$ là một điểm của B và cho V là một lân cận của $b$ sao cho $\gamma i_*(\pi_1(V, b))\gamma^{-1}\subset H$ với mọi lớp đường đi $\gamma$ nối $a$ với $b$ trong B, trong đó $i$ ký hiệu phép bao của V vào B. Vì B liên thông cung địa phương, hơn nữa ta có thể giả sử rằng V liên thông cung. Cho $c\in V$, cho $\delta$ là lớp trong $\pi_1(B, c)$ của một vòng tại $c$ được chứa trong V, và cho $\delta '$ là một phần tử của $\lambda_a(B)$ sao cho $\varepsilon (\delta ') =c$. Cho $\delta ''$ là một phần tử của $\varpi_{c,b}(V)$ và đặt $\gamma =\delta '\delta ''$. Theo định nghĩa của V, phần tử $\delta '\delta (\delta ')^{-1}=\gamma ((\delta '')^{-1}\delta \delta '')\gamma^{-1}$ của $\pi_1(B, a)$ thuộc H. Khi đó $H\delta '\cdot \delta = H\delta '$; điều này chứng minh rằng $\pi_1(V, c)$ tác động tầm thường lên tập hợp $\overset{-1}{q}(c)$.

Theo III, p. 313, Mệnh đề 3, tồn tại một tôpô duy nhất trên $H\backslash \lambda_a(B)$ sao cho $q$ là liên tục và không gian B $(H\backslash \lambda_a(B), q)$ là một phủ sao cho phép toán chính tắc của $\varpi (B)$ trên phủ này là phép toán được định nghĩa ở trên. Theo mệnh đề b) của Định lý 1 của III, p. 305, nhóm $q_*(\pi_1(H\backslash \lambda_a(B),H))$ bằng H.

Ta sẽ nói rằng một phép toán của nhóm $\pi_1(B, b)$ trên một tập hợp X là khả chấp nhận nếu hạt nhân của ánh xạ chính tắc $\pi_1(B, b)\rightarrow \mathfrak{S}_X$ là một nhóm con mở của $\pi_1(B, b)$. Điều này tương đương với việc nói rằng đồng cấu $\pi_1(B, b)\rightarrow \mathfrak{S}_X$ là liên tục nếu nhóm $\mathfrak{S}_X$ được trang bị tôpô rời rạc. Khi đó ánh xạ $\pi_1(B, b)\times X\rightarrow X$ là liên tục, khi X được trang bị tôpô rời rạc. Ngược lại, xét một phép toán liên tục của $\pi_1(B, b)$ trên một không gian rời rạc X. Cho $x$ là một điểm của X; nhóm ổn định của nó là một nhóm con mở H của $\pi_1(B, b)$ theo giả thiết. Với $\gamma \in \pi_1(B, b)$, nhóm ổn định của $\gamma \cdot x$ là nhóm con $\gamma H\gamma^{-1}$, sao cho nhóm con của $\pi_1(B, b)$ cố định mỗi phần tử của quỹ đạo của $x$ là giao của các nhóm con $\gamma H\gamma^{-1}$, với $\gamma$ chạy trên $\pi_1(B, b)$. Nó là một nhóm con mở vì các nhóm con chuẩn mở của $\pi_1(B, b)$ tạo thành một cơ sở của tôpô của nó (III, p. 315, Mệnh đề 4). Suy ra rằng một phép toán liên tục của $\pi_1(B, b)$ trên một không gian rời rạc X là khả chấp nhận nếu nó là bắc cầu hoặc, nói chung hơn, nếu tập hợp các quỹ đạo của các phần tử của X là hữu hạn.

Với mọi nhóm rời rạc G, mọi phủ chính E của B với nhóm G, và mọi điểm $x\in E_b$, ta nhắc lại rằng ánh xạ $h_{(E,x)}$ từ $\pi_1(B, b)$ vào G, ánh xạ gán cho $\gamma \in \pi_1(B, b)$ phần tử duy nhất $g\in G$ sao cho $x\cdot g=x\cdot \gamma^{-1}$, là một đồng cấu nhóm (III, p. 306, mệnh đề 5).

#### Mệnh đề 6 {#ta-iii-s5-prop-6 .statement tag=0204}

Cho B là một không gian tôpô và b là một điểm của B. Trang bị cho nhóm $\pi_1(B, b)$ tôpô khả chấp nhận được.

a) Với mọi nhóm rời rạc G, mọi phủ chính E của B với nhóm G, và mọi $x\in E_b$, đồng cấu $h_{(E,x)}$ là một đồng cấu liên tục của các nhóm tôpô.

b) Với mọi phủ E của B, tác động chính tắc của $\pi_1(B, b)$ trên thớ $E_b$ là khả chấp nhận được.

Chỉ cần chứng minh mệnh đề thứ hai. Gọi K là tập hợp các phần tử $k\in \pi_1(B, b)$ sao cho $x\cdot k=x$ với mọi $x\in E_b$; ta hãy chứng minh rằng K là một nhóm con khả chấp nhận được của $\pi_1(B, b)$.

Cho $b'$ là một điểm của B và V' là một lân cận của $b'$ trong B trên đó phủ E tầm thường hóa được. Gọi $\gamma$ là lớp của một đường đi c nối b với $b'$ trong B và gọi c' là đường đi duy nhất trong E có điểm đầu x nâng c. Với mọi $\delta \in \pi_1(V', b')$ và mọi $x'\in E_{b'}$, ta có $x'\cdot \delta =x'$. Do đó, với $x\in E_b$ và $\delta \in \pi_1(V', b')$, ta có

$$
x\cdot \gamma \delta \gamma^{-1}= ((x\cdot \gamma )\cdot \delta )\cdot \gamma^{-1}= (x\cdot \gamma )\cdot \gamma^{-1}=x
$$

suy ra $\gamma \delta \gamma^{-1}$ thuộc K. Nói cách khác, K là một nhóm con khả chấp nhận được, do đó mệnh đề được chứng minh.

#### Mệnh đề 7 {#ta-iii-s5-prop-7 .statement tag=0205}

Cho B là một không gian tôpô liên thông, liên thông địa phương bởi các cung, và b là một điểm của B. Trang bị cho nhóm $\pi_1(B, b)$ tôpô khả chấp nhận được.

a) Cho G là một nhóm tôpô rời rạc. Với mọi đồng cấu liên tục $f:\pi_1(B, b)\rightarrow$ G, tồn tại một phủ chính E của B với nhóm G và một điểm $x$ của $E_b$ sao cho $h_{(E,x)}=f$.

b) Với mọi không gian tôpô rời rạc F được trang bị một tác động phải khả chấp nhận được của nhóm $\pi_1(B, b)$, tồn tại một phủ E của B sao cho các tập hợp $\pi_1(B, b)$-F và $E_b$ là đẳng cấu.

Ta hãy chứng minh a). Cho $f$ là một đồng cấu liên tục từ $\pi_1(B, b)$ vào một nhóm rời rạc G. Hạt nhân của nó là một nhóm con mở bất biến K của $\pi_1(B, b)$; gọi H là nhóm $\pi_1(B, b)/K$ và $\overline{f}: H\rightarrow G$ là đồng cấu nhóm suy ra từ f bằng cách chuyển qua thương. Theo III, p. 316, mệnh đề 5, tồn tại một phủ liên thông $E'$ của B sao cho nhóm con K là nhóm ổn định của mọi điểm của thớ $E'_b$; phủ $E'$ là chính với nhóm $H =\pi_1(B, b)/K$. Gọi $x'$ là một điểm của $E'_b$; đồng cấu $h_{(E',x')}:\pi_1(B, b)\rightarrow H$ là toàn ánh với hạt nhân K (III, p. 306, mệnh đề 5). Do đó tồn tại một đồng cấu nhóm duy nhất $\varphi : H\rightarrow G$ sao cho $\varphi \circ h_{(E',x')}=f$. Phủ liên kết $E = E'\times^HG$ của B là chính với nhóm G và ta có $h_{(E,x)}=\varphi \circ h_{(E',x')}=f$ (III, p. 307, ví dụ 2). Điều này chứng minh mệnh đề a).

Ta chứng minh b). Cho F là một tập hợp được trang bị một tác động phải khả chấp của nhóm $\pi_1(B, b)$. Gọi $f:\pi_1(B, b)\rightarrow \mathfrak{S}_F$ là tác động này và trang bị cho nhóm $\mathfrak{S}_F$ tôpô rời rạc. Theo a), tồn tại một phủ E của B, chính với nhóm $\mathfrak{S}_F$, và một điểm $x\in E$ sao cho đồng cấu $h_{(E,x)}$ bằng $f$. Tác động chính tắc của nhóm $\pi_1(B, b)$ trên thớ trên $b$ của phủ liên kết $E\times^{\mathfrak{S}_F}F$ của B được đồng nhất với tác động của $\pi_1(B, b)$ trên F (III, p. 306, Ví dụ 1).

#### Nhận xét 4 {#ta-iii-s5-n4-rem-4 .statement tag=0206}

Tôpô khả chấp trên $\pi_1(B, b)$ là tôpô ít mịn nhất sao cho tác động của $\pi_1(B, b)$ trên $E_b$ là liên tục đối với mọi phủ liên thông E của B (Mệnh đề 6 của III, p. 318 và Mệnh đề 7 của III, p. 318). Nếu E là một phủ liên thông của B và $x$ là một điểm của thớ $E_b$, ánh xạ $c'\mapsto c'(1)$ từ $\Lambda_x(E)$ vào E là liên tục. Do đó, ánh xạ $c\mapsto x\cdot c$ từ $\Lambda_b(B)$ vào E là liên tục (III, p. 302, Hệ quả 2 của Mệnh đề 3). Bằng hạn chế vào $\Omega_b(B)$ và chuyển qua thương, suy ra rằng ánh xạ $\gamma \mapsto x\cdot \gamma$ là liên tục khi nhóm $\pi_1(B, b)$ được trang bị tôpô không gian thương của $\Omega_b(B)$. Vì vậy tôpô khả chấp trên $\pi_1(B, b)$ ít mịn hơn tôpô thương của tôpô hội tụ compact. Nó có thể ít mịn hơn một cách thực sự (III, p. 337, Bài tập 7).

#### Nhận xét 5 {#ta-iii-s5-n4-rem-5 .statement tag=0207}

Cho B là một không gian tôpô liên thông và liên thông cung địa phương, cho $a$ là một điểm của B, và cho H là một nhóm con của $\pi_1(B, a)$. Theo nhận xét trước, nếu H là khả chấp, thì nó cũng là mở đối với tôpô thương của tôpô hội tụ compact. Ngược lại, giả sử rằng H là một nhóm con chuẩn của $\pi_1(B, a)$ mở đối với tôpô thương của tôpô hội tụ compact. Cho $x$ là một điểm của B và cho $\gamma \in \varpi_{a,x}(B)$. Nhóm con $\gamma^{-1}H\gamma$ của $\pi_1(B, x)$ lại mở đối với tôpô thương của tôpô hội tụ compact (III, p. 293, Nhận xét 3). Do đó tồn tại một lân cận V của $x$ trong B sao cho $\gamma^{-1}H\gamma$ chứa lớp của mọi đường vòng tại $x$ có ảnh được chứa trong V. Do đó $\gamma \pi_1(V, x)\gamma^{-1}\subset H$; vì H là chuẩn, điều này suy ra rằng H là một nhóm con khả chấp của $\pi_1(B, a)$.

## BÀI TẬP {#ta-iii-s5-exercises}

Xem [các bài tập cho § 5](exercises/s5/).
