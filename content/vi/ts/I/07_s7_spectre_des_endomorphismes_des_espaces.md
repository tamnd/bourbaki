---
book: ts
book_title: Théories spectrales
chapter: I
chapter_title: ALGÈBRES NORMÉES
section: 7
section_title: Spectre des endomorphismes des espaces de Banach
lang: vi
source: ts-i-ii-fr
book_pages: TS I.127-TS I.142, TS I.187-TS I.191
pdf_pages: 0140-0155, 0200-0204
extraction: native
subsections:
    - "no": 1
      title: Spectre d’un endomorphisme
      page: 127
      pdf_page: 140
    - "no": 2
      title: Projecteurs spectraux
      page: 129
      pdf_page: 142
    - "no": 3
      title: Points isolés du spectre
      page: 131
      pdf_page: 144
    - "no": 4
      title: Spectre de la transposée d’un endomorphisme
      page: 131
      pdf_page: 144
    - "no": 5
      title: Cas des espaces hilbertiens
      page: 132
      pdf_page: 145
    - "no": 6
      title: Image numérique
      page: 135
      pdf_page: 148
    - "no": 7
      title: Éléments positifs
      page: 138
      pdf_page: 151
    - "no": 8
      title: Décomposition polaire
      page: 139
      pdf_page: 152
statements: 24
exercises: 16
content_sha256: b5672a2de54678870fc3be4167da6f00b36bcf0bb6cceaa265110c946e904c66
translated_from: content/en-mt/ts/I/07_s7_spectre_des_endomorphismes_des_espaces.md
source_lang: en-mt
translation_method: machine
source_content_sha256: c0d3782fe36d1716c0a232855572d590f23110c38326670940e28ab4d7ed8d02
translation_model: gpt-5.4
translation_run: translate-vi-634f7cbf
glossary_version: 34
glossary_terms_sha256: e2a1a6d0b67188e3f7209ffbf454f66410ff0b044fbda85ae6802d511d14b289
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 7. PHỔ CỦA CÁC TỰ ĐỒNG CẤU CỦA CÁC KHÔNG GIAN BANACH

Trừ khi nói khác, các không gian vectơ được xét trong số này đều là các không gian vectơ trên $\mathbf{C}$. Ta ký hiệu bởi $1_E$ ánh xạ đồng nhất của một không gian vectơ E. Một tự đồng cấu của một không gian vectơ tôpô E là một ánh xạ tuyến tính liên tục từ E vào E.

Cho E là một không gian vectơ tôpô và $u$ là một tự đồng cấu của E. Nếu F là một không gian con của E ổn định dưới $u$, ta sẽ nói rằng tự đồng cấu của F suy ra từ $u$ bằng cách chuyển qua không gian con là tự đồng cấu của F suy ra từ $u$. Ta ký hiệu nó bởi $u|F$.

### 1. Phổ của một tự đồng cấu

#### Định nghĩa 1 {#ts-i-s7-def-1 .statement tag=02G0}

Cho E là một không gian vectơ tôpô và $u$ là một tự đồng cấu của E. Phổ của $u$, ký hiệu là Sp($u$), là phổ của $u$ đối với đại số có đơn vị $\mathscr{L}(E)$.

Cho E là một không gian vectơ tôpô và $u\in \mathscr{L}(E)$. Phổ của $u$ là tập hợp các số phức $\lambda$ sao cho $u-\lambda 1_E$ không phải là một tự đẳng cấu của E. Nếu E đầy đủ khả mêtric, thì đó cũng là tập hợp các số phức $\lambda$ sao cho $u-\lambda 1_E$ không song ánh (EVT, I, p. 19, Hệ quả 1).

Mọi trị riêng của $u$ đều thuộc phổ của $u$, nhưng nói chung đảo lại là sai.

Trong phần còn lại của số này, ta sẽ giới hạn việc nghiên cứu khái niệm phổ vào trường hợp E là một không gian Banach.

#### Bổ đề 1 {#ts-i-s7-lem-1 .statement tag=02G1}

Cho E là một không gian Banach và $u$ là một tự đồng cấu của E. Cho $(E_i)_{i\in I}$ là một họ hữu hạn các không gian con đóng của E, ổn định dưới $u$, sao cho $E =\bigoplus_{i\in I}E_i$. Với mỗi $i\in I$, gọi $u_i$ là tự đồng cấu của $E_i$ suy ra từ $u$. Khi đó Sp($u$) $=\bigcup_{i\in I}$ Sp($u_i$), và với mọi $f\in \mathscr{O}$(Sp($u$)), tự đồng cấu $f(u)$ ổn định các không gian $E_i$, và $f(u)$ trùng với $f(u_i)$ trên $E_i$.

Tự đồng cấu $u$ là một đẳng cấu khi và chỉ khi $u_i$ là một đẳng cấu với mọi $i\in I$. Áp dụng tính chất này cho $u-\lambda 1_E$, ta suy ra rằng Sp($u$) là hợp của các tập hợp Sp($u_i$) với $i\in I$.

Cho $f\in \mathscr{O}$(Sp($u$)). Tự đồng cấu $f(u)$ của E thuộc đối giao hoán tử kép của $u$ trong $\mathscr{L}(E)$ (Định lý 5 của I, p. 74), và vì vậy giao hoán với các phép chiếu $p_i$. Do đó nó ổn định các không gian $E_i$. Xét cấu xạ liên tục có đơn vị $\varpi$ từ đại số tích $\prod_{i\in I}\mathscr{L}(E_i)$ vào $\mathscr{L}(E)$ được xác định bởi $(v_i)_{i\in I}\mapsto \bigoplus_iv_i$. Nó biến họ $(u_i)$ thành $u$. Khi đó Mệnh đề 7 của I, p. 75 suy ra Sp($u$)$\subset \bigcup_{i\in I}$ Sp($u_i$) và

$$
f(u) =f(\varpi ((u_i)_{i\in I})) =\varpi ((f(u_i))_{i\in I}) =\bigoplus_{i\in I}f(u_i)
$$

điều này kết thúc chứng minh bổ đề.

#### Mệnh đề 1 {#ts-i-s7-prop-1 .statement tag=02G2}

Cho E là một không gian Banach phức và $u$ là một tự đồng cấu của E. Cho $\lambda \in \mathbf{C}$ và $f\in \mathscr{O}$(Sp($u$)). Ta có

Ker($u-\lambda 1_E$)$\subset$ Ker($f(u)-f(\lambda )1_E$).

Cho $x\in E$ khác không. Tập hợp A các $v\in \mathscr{L}(E)$ sao cho $x$ là một vectơ riêng của $v$ là một đại số con có đơn vị của $\mathscr{L}(E)$.

Đại số A là đầy: nếu $v\in A$ khả nghịch trong $\mathscr{L}(E)$ và nếu $x$ là một vectơ riêng của $v$ ứng với trị riêng $\lambda$, thì $\lambda \not= 0$ và $v^{-1}(x) =\lambda^{-1}x$, điều này chứng minh rằng $v^{-1}\in A$.

Đại số A đóng trong $\mathscr{L}(E)$. Thật vậy, nếu $(v_n)_{n\in\mathbf{N}}$ là một dãy trong A sao cho $v_n$ hội tụ đến $v\in \mathscr{L}(E)$, thì dãy $(\lambda_n)_{n\in\mathbf{N}}$ sao cho $v_n(x) =\lambda_nx$ bị chặn, và do đó nhận một dãy con hội tụ đến một số phức $\mu$, vì thế $v(x) =\mu x$.

Giả sử rằng $x$ là một vectơ riêng của $u$ và $u(x) =\lambda x$. Đại số A chứa $u$, và vì vậy chứa đại số con đóng đầy có đơn vị B sinh bởi $u$, đại số này là giao hoán. Ánh xạ $\chi : B\rightarrow \mathbf{C}$ gán cho $v$ trị riêng của $v$ tương ứng với $x$ là một đặc trưng của B sao cho $\chi (u) =\lambda$. Với mọi $f\in \mathscr{O}$(Sp($u$)), ta có $f(u)\in B$ và $\chi (f(u)) =f(\chi (u)) =f(\lambda )$ theo Mệnh đề 7 của I, p. 75, do đó có mệnh đề.

### 2. Các phép chiếu phổ

Cho E là một không gian Banach. Ta ký hiệu bởi A đại số Banach có đơn vị $\mathscr{L}(E)$ của các tự đồng cấu của E. Cho $u\in A$.

Gọi H là một tập con của Sp($u$) vừa mở vừa đóng trong Sp($u$); gọi K là phần bù của nó trong Sp($u$).

Phần tử lũy đẳng liên kết với $u$ và H (No.$^o12$ của I, p. 81) là một phép chiếu liên tục của E, gọi là phép chiếu phổ liên kết với $u$ và H; nó được ký hiệu bởi $e_H(u)$, hoặc đơn giản là $e_H$. Ảnh của nó được gọi là không gian con phổ của E liên kết với $u$ và H, và được ký hiệu bởi $E_H(u)$, hoặc đơn giản là $E_H$. Hạt nhân của nó là $E_K(u)$, và cũng được ký hiệu bởi $\widetilde{E}_H(u)$, hoặc đơn giản là $\widetilde{E}_H$. Không gian E là tổng trực tiếp tôpô của các không gian con đóng $E_H$ và $E_K$. Để có $E_H= 0$, điều kiện cần và đủ là có $e_H= 0$, nghĩa là hàm đặc trưng $f_H$ của H trên Sp($u$) là hàm không, nghĩa là $H =\emptyset$.

Mọi tự đồng cấu $v$ của E giao hoán với $u$ cũng giao hoán với $e_H(u)$ (Định lý 5 của I, p. 74), do đó ổn định $E_H$ và $E_K$. Đặc biệt, tự đồng cấu $u$ để ổn định các không gian con $E_H$ và $E_K$. Không gian $E_K$ là phần bù tôpô duy nhất của $E_H$ trong E mà ổn định bởi $u$.

Đại số có đơn vị $A_H=e_HAe_H($loc. cit.) là đại số con của A gồm các tự đồng cấu của E ổn định $E_H$ và bằng không trên $E_K$. Với mọi $v\in A_H$, ta ký hiệu bởi $v|E_H$ tự đồng cấu của $E_H$ suy ra từ $v$. Ánh xạ $v\mapsto v|E_H$ là một đẳng cấu từ $A_H$ lên $\mathscr{L}(E_H)$. Đặc biệt, ta có Sp($u|E_H$) $=$ Sp$_{A_H}(u|E_H) = H$ và Sp$_{A_K}(u|E_K) = K$ theo công thức (18) của I, p. 82.

#### Mệnh đề 2 {#ts-i-s7-prop-2 .statement tag=02G3}

Cho E là một không gian Banach và $u$ là một tự đồng cấu của E. Cho $E_1$ và $E_2$ là các không gian con đóng của E, bất biến dưới $u$, sao cho $E = E_1\oplus E_2$. Giả sử rằng các tự đồng cấu $u_1$ và $u_2$ của $E_1$ và $E_2$ cảm sinh bởi $u$ có các phổ rời nhau $H_1=$ Sp($u_1$) và $H_2$ = Sp($u_2$). Khi đó Sp($u$) $= H_1\cup H_2$ và $e_{H_1}(u)$ là phép chiếu có ảnh là $E_1$ và hạt nhân là $E_2$. Đặc biệt, ta có $E_{H_1}= E_1$ và $E_{H_2}= E_2$.

Ta có Sp($u$) $= H_1\cup H_2($I, p. 128, Bổ đề 1). Vì các tập hợp $H_1$ và $H_2$ là compact, chúng vừa mở vừa đóng trong Sp($u$). Với mọi hàm chỉnh hình $f$ trong một lân cận của Sp($u$), tự đồng cấu $f(u)$ để $E_1$ và $E_2$ bất biến và trùng trên $E_1$ với $f(u_1)$, còn trên $E_2$ với $f(u_2)$ (loc. cit.). Đặc biệt lấy $f$ là mầm của hàm chỉnh hình $f_{H_1}$ bằng 1 trong một lân cận của $H_1$ và bằng 0 trong một lân cận của $H_2$ (x. No. 12 của I, p. 81); khi đó $f_{H_1}(u_1)$ là ánh xạ đồng nhất của $E_1$ vì $f_{H_1}$ = 1 trong một lân cận của $H_1=$ Sp($u_1$), và $f_{H_1}(u_2)$ bằng không vì $f_{H_1}= 0$ trong một lân cận của $H_2$. Do đó $e_{H_1}(u) =f_{H_1}(u)$ là phép chiếu có ảnh là $E_1$ và hạt nhân là $E_2$, và vì vậy ta có $E_1= E_{H_1}$ và $E_2= E_{H_2}$.

Cho E là một không gian Banach và $u$ là một tự đồng cấu của E. Cho $(H_i)_{i\in I}$ là một họ hữu hạn các tập con mở và đóng của Sp($u$), từng đôi một rời nhau, và gọi H là hợp của chúng. Các hệ thức (15) và (16) của I, p. 81 suy ra các mệnh đề sau :

a) Họ các phép chiếu $(e_{H_i}(u))_{i\in I}$ là trực giao (nghĩa là, $e_{H_i}(u)e_{H_j}(u) = 0$ với mọi $(i, j)$ trong $I^2$ sao cho $i\not=j$, xem A, II, p. 18, Def. 7) và tổng của chúng là $e_H(u)$;

b) Không gian vectơ $E_H$ là tổng trực tiếp tôpô của họ $(E_{H_i})_{i\in I}$;

c) Với mọi $j\in I$, ta có $E_{Sp(u)-H_j}= E_{Sp(u)-H}\oplus \bigoplus_{i\not=j}E_{H_i}$;

d) Không gian vectơ $E_{Sp(u)-H}$ là giao của họ $(E_{Sp(u)-H_i})_{i\in I}$.

Khi H = Sp($u$), phân tích thành tổng trực tiếp tôpô $\bigoplus_{i\in I}E_{H_i}$ của E được gọi là phân tích phổ của E liên kết với $u$ và với phân hoạch hữu hạn $(H_i)_{i\in I}$ của Sp($u$).

Cho $f$ là một phần tử của $\mathscr{O}$(Sp($u$)). Phổ của tự đồng cấu $f(u)$ của E là ảnh của phổ của $u$ qua $f$ (I, p. 75, Prop. 8). Cho L là một tập con vừa mở vừa đóng trong Sp($f(u)$). Tập H gồm các phần tử $\lambda \in$ Sp($u$) sao cho $f(\lambda )$ thuộc L là vừa mở vừa đóng trong Sp($u$), và ta có $e_L(f(u)) =e_H(u)$ vì $f_L\circ f=f_H$ trong $\mathscr{O}$(Sp($u$)) (loc. cit.).

### 3. Các điểm cô lập của phổ

Cho E là một không gian Banach và cho $u$ là một tự đồng cấu của E. Cho $\lambda \in \mathbf{C}$ là một điểm cô lập của Sp($u$). Khi đó ta đặt $E_{\lambda}(u) = E_{\{\lambda\}}(u)$ và $e_{\lambda}(u)$ cho phép chiếu phổ có ảnh là $E_{\lambda}(u)$ liên kết với $u$ và với $\{\lambda \}$.

Ta cũng đặt $\widetilde{E}_{\lambda}(u) = E_{Sp(u)-\{\lambda\}}(u)$. Phổ của tự đồng cấu của $\widetilde{E}_{\lambda}(u)$ cảm sinh bởi $u$ là Sp($u$)$-\{\lambda \}$; đặc biệt, $u-\lambda 1_E$ cảm sinh một tự đẳng cấu của $\widetilde{E}_{\lambda}(u)$.

Không gian $E_{\lambda}(u)$ khác không. Phổ của tự đồng cấu của $E_{\lambda}(u)$ cảm sinh bởi $u$ thu về $\lambda$, do đó $u-\lambda 1_E$ cảm sinh một tự đồng cấu giả lũy linh của $E_{\lambda}(u)$. Tự đồng cấu $u-\lambda 1_E$ cảm sinh một tự đẳng cấu của $\widetilde{E}_{\lambda}(u)$, do đó Ker($u-\lambda 1_E$)$^n\subset E_{\lambda}(u)$ với mọi $n\in \mathbf{N}$. Đặc biệt, ta có Ker($u-\lambda 1_E$)$\subset E_{\lambda}(u)$.

Để $\lambda$ là một cực bậc $p >0$ của phân giải thức của $u$, điều kiện cần và đủ là $(u-\lambda 1_E)^{p-1}e_{\lambda}(u)\not= 0$ và $(u-\lambda 1_E)^pe_{\lambda}(u) = 0$ (hệ quả của mệnh đề 17 của I, p. 83). Trong trường hợp này, ta có $E_{\lambda}(u) =$ Ker(($u-\lambda 1_E$)$^p$) và $\widetilde{E}_{\lambda}(u) =$ Im(($u-\lambda 1_E$)$^p$), vì $(u-\lambda 1_E)^p$ cảm sinh một tự đẳng cấu của $\widetilde{E}_{\lambda}(u)$. Ta cũng có

$(u-\lambda 1_E)^{p-1}e_{\lambda}(u) =$ lim$_{z\rightarrow\lambda}(z-\lambda 1_E)^pR(u, z)$

theo mệnh đề 17 của I, p. 83.

Cần lưu ý rằng nói chung $E_{\lambda}(u)$ không phải là hợp của họ (Ker(($u-\lambda 1_E$)$^n$))$_{n\in\mathbf{N}}$, thậm chí cũng không phải là bao đóng của hợp này; đặc biệt, một điểm cô lập của Sp($u$) không nhất thiết là một trị riêng của $u($I, p. 187, bài tập 1). Tương tự, có thể tồn tại các trị riêng của $u$ không phải là các điểm cô lập của Sp($u$) (I, p. 188, bài tập 2).

### 4. Phổ của chuyển vị của một tự đồng cấu

#### Mệnh đề 3 {#ts-i-s7-prop-3 .statement tag=02G4}

Cho E là một không gian Banach và $E'$ là đối ngẫu của nó. Cho $u$ là một tự đồng cấu của E.

a) Ta có Sp($u$) $=$ Sp($^tu$) ;

b) Với mọi $f\in \mathscr{O}$(Sp($u$)), ta có $f(^tu) =^tf(u)$ ;

c) Ta có $e_H(^tu) =^te_H(u)$ với mọi tập con H của Sp($u$) vừa mở vừa đóng.

Để một tự đồng cấu của E là một tự đẳng cấu, điều kiện cần và đủ là chuyển vị của nó là một tự đẳng cấu của $E'$ (EVT, IV, p. 30, hệ quả 5), do đó suy ra mệnh đề a).

Ánh xạ $v\mapsto^tv$ là một đồng cấu có đơn vị liên tục của đại số Banach $\mathscr{L}(E)$ vào đại số Banach đối của $\mathscr{L}(E')$ (EVT, IV, p. 7, mệnh đề 8). Vì đại số $\mathscr{O}$(Sp($^tu$)) là giao hoán, ánh xạ $f\mapsto^tf(u)$ là một đồng cấu có đơn vị liên tục của đại số $\mathscr{O}$(Sp($^tu$)) vào đại số $\mathscr{L}(E')$. Đồng cấu này ánh xạ mầm của ánh xạ đồng nhất của $\mathbf{C}$ tới $^tu$, và do đó trùng với đồng cấu $f\mapsto f(^tu)$ (định lý 5 của I, p. 74). Điều này chứng minh b).

Mệnh đề c) suy ra từ b), áp dụng cho hàm $f_H$ bằng 1 trong một lân cận của H và bằng 0 trong một lân cận của phần bù của nó trong Sp($u$).

#### Nhận xét {#ts-i-s7-n4-rem-1 .statement tag=02G5}

Cho H là một tập con vừa mở vừa đóng trong Sp($u$), với phân tích phổ liên kết là $E = E_H(u)\oplus \widetilde{E}_H(u)$. Từ mệnh đề c) suy ra rằng nếu ta đồng nhất $E'$ với $E_H(u)'\oplus \widetilde{E}_H(u)'$, thì ta có $E'_H(^tu) = E_H(u)'$ và $\widetilde{E}'_H(^tu) =\widetilde{E}_H(u)'$.

### 5. Trường hợp của các không gian Hilbert

Trong số này, xét các không gian Hilbert trên $K =\mathbf{R}$ hoặc $\mathbf{C}$. Ta ký hiệu bởi $\langle x_1|x_2\rangle$ tích vô hướng của hai vectơ $x_1$ và $x_2$ trong một không gian Hilbert E.

Nếu E là một không gian Hilbert phức, đại số Banach $\mathscr{L}(E)$ được trang bị phép đối hợp $u\mapsto u^*$ là một đại số sao (Ví dụ 1 của I, p. 102). Đặc biệt, nếu $u\in \mathscr{L}(E)$, ta có $\varrho (u^*) =\varrho (u)$ và Sp($u^*$) $=$ Sp($u$).

Cho $u\in \mathscr{L}(E)$ là một tự đồng cấu chuẩn tắc và cho $\lambda \in \mathbf{C}$. Không gian riêng của $u$ ứng với $\lambda$ trùng với không gian riêng của liên hợp $u^*$ ứng với $\lambda$ (EVT, V, p. 43, hệ quả của mệnh đề 8). Tuy nhiên, nói chung các không gian này không trùng nhau nếu $u$ không chuẩn tắc (bài tập 3 của I, p. 188).

Cho $\lambda$ và $\mu$ là các số phức sao cho $\lambda \not=\mu$. Cho $x$ là một vectơ riêng của $u$ ứng với $\lambda$ và cho $y$ là một vectơ riêng của $u$ ứng với $\mu$. Khi đó $u^*(x) =\lambda x$, do đó

$$
\mu\langle x|y\rangle =\langle x|u(y)\rangle =\langle u^*(x)|y\rangle =\langle \lambda x|y\rangle =\lambda \langle x|y\rangle
$$

Suy ra $\langle x|y\rangle = 0$; các không gian riêng của $u$ trực giao từng đôi một. Hơn nữa, với mọi $\lambda \in \mathbf{C}$, không gian riêng của $u$ ứng với $\lambda$ trùng với không gian con nguyên sơ của $u$ ứng với $\lambda$, nghĩa là (LIE, VII, §1, n$^o1$) hợp khi $k\in \mathbf{N}$ của các hạt nhân của $(u-\lambda 1_E)^k$ (EVT, V, p. 43, hệ quả của mệnh đề 8).

#### Bổ đề 2 {#ts-i-s7-lem-2 .statement tag=02G6}

Cho E là một không gian Hilbert phức và cho $u$ là một tự đồng cấu chuẩn tắc của E. Cho $(E_i)_{i\in I}$ là một họ hữu hạn các không gian con đóng của E, ổn định dưới $u$ và trực giao từng đôi một, sao cho $E =\bigoplus_{i\in I}E_i$. Với mỗi $i\in I$, ký hiệu $u_i$ là tự đồng cấu của $E_i$ cảm sinh bởi $u$. Ta có Sp($u$) $=\bigcup_{i\in I}$ Sp($u_i$), và với mọi $f\in \mathscr{C}$(Sp($u$)), tự đồng cấu $f(u)$ ổn định các không gian $E_i$, và $f(u)$ trùng với $f(u_i)$ trên $E_i$.

Chứng minh theo chứng minh của bổ đề 1 của I, p. 128, dùng nhận xét ở 6 của I, p. 110 và mệnh đề 8 của I, p. 112.

#### Mệnh đề 4 {#ts-i-s7-prop-4 .statement tag=02G7}

Cho E là một không gian Hilbert phức và cho $u$ là một tự đồng cấu chuẩn tắc của E. Với mọi hàm $f\in \mathscr{C}$ (Sp($u$)) và mọi $\lambda \in \mathbf{C}$, ta có

Ker($u-\lambda 1_E$)$\subset$ Ker($f(u)-f(\lambda )1_E$).

Chứng minh là tương tự với chứng minh của mệnh đề 1 trong I, p. 128; ta hãy xét lại các lập luận của nó. Đại số A được đưa vào ở chỗ đã dẫn ở đây là một đại số con có đơn vị, có phép đối hợp của $\mathscr{L}(E)$ (EVT, V, p. 43, hệ quả). Do đó nó chứa đại số con có đơn vị, có phép đối hợp B sinh bởi $u$, là giao hoán. Ánh xạ $\chi : B\rightarrow \mathbf{C}$ gán cho $v$ trị riêng của $v$ đối với $x$ là một đặc trưng của B sao cho $\chi (u) =\lambda$. Với mọi $f\in \mathscr{C}$ (Sp($u$))), ta có $f(u)\in B$ và $\chi (f(u)) =f(\chi (u)) =f(\lambda )$ theo mệnh đề 8 của I, p. 112, do đó suy ra mệnh đề.

#### Bổ đề 3 {#ts-i-s7-lem-3 .statement tag=02G8}

Cho E là một không gian Hilbert và $p\in \mathscr{L}(E)$ là một phép chiếu. Các mệnh đề sau là tương đương:

(i) Phép chiếu $p$ là một phép chiếu trực giao, nghĩa là Ker($p$) $=$ Im($p$)$^{\circ}$ (EVT, V, p. 13);

(ii) Phép chiếu $p$ là Hermit;

(iii) Phép chiếu $p$ là chuẩn tắc;

(iv) Ta có Ker($p$)$\subset$ Ker($p^*$) ;

(v) Ta có Im($p$)$\subset$ Im($p^*$) ;

(vi) Phép chiếu $p$ là dương;

(vii) Ta có $\|p\|\leqslant 1$.

Trước hết nhắc lại rằng Ker($p^*$) $=$ Im($p$)$^{\circ}$ và Ker($p$) $=$ Im($p^*$)$^{\circ}$ (EVT, V, p. 41, mệnh đề 4). Hơn nữa, ảnh của $p$ (resp. $p^*$) là đóng, vì nó trùng với hạt nhân của $1-p$ (resp. $1-p^*$). Vậy ta có

(1) Im($p$) $=$ Ker($p^*$)$^{\circ}$, Im($p^*$) $=$ Ker($p$)$^{\circ}$.

(i) $=\Rightarrow$ (ii)$:p^*$ là một phép chiếu có hạt nhân Im($p$)$^{\circ}=$ Ker($p$) và có ảnh là Im($p^*$)$^{\circ}=$ Ker($p$) $=$ Im($p$)$^{\circ}$; do đó $p^*=p$.

(ii) $=\Rightarrow$ (iii) vì mọi tự đồng cấu Hermit đều là chuẩn tắc.

(iii) $=\Rightarrow$ (iv) : vì $p$ là chuẩn tắc, ta có $\|p(x)\|^2=\|p^*(x)\|^2$ với mọi $x$ trong E (EVT, V, p. 43, Prop. 7), do đó suy ra bao hàm thức cần chứng minh.

(iv) $=\Rightarrow$ (v) suy ra từ các đẳng thức (1) ở trên.

(v) $=\Rightarrow$ (vi) : với mọi $x\in E$, ta có $p(x)\in$ Im($p^*$), và do đó $\langle p(x)|x\rangle =\langle p^*(p(x))|x\rangle =\|p(x)\|^2\geqslant 0$.

(vi) $=\Rightarrow$ (vii) : cho $x\in E$ và $y=x-p(x)\in$ Ker($p$). Với mọi $t\in \mathbf{R}$, theo giả thiết ta có

$$
\langle x+ty|p(x)\rangle =\langle x+ty|p(x+ty)\rangle \geqslant 0
$$

điều này chỉ có thể xảy ra nếu $\langle y|p(x)\rangle = 0$. Nhưng khi đó

$$
\|p(x)\|^2=\langle x|p(x)\rangle \leqslant \|x\|\|p(x)\|
$$

và do đó $\|p\|\leqslant 1$.

(vii) $=\Rightarrow$ (i) : cho $y\in$ Im($p$) ; ký hiệu $z$ là phép chiếu trực giao của $y$ lên Ker($p$)$^{\circ}$ và đặt $x=y-z\in$ Ker($p$). Ta có $p(z) =p(y) =y$, nên theo giả thiết $\|y\|\leqslant \|z\|$. Nhưng, vì $x$ và $z$ trực giao, ta có $\|y\|^2=\|x\|^2+\|z\|^2$, do đó $\|x\|= 0$, nghĩa là $y=z$. Vậy, Im($p$)$\subset$ Ker($p$)$^{\circ}$. Hơn nữa, vì $\|p^*\|=\|p\|\leqslant 1$, tương tự ta có Im($p^*$)$\subset$ Ker($p^*$)$^{\circ}$, điều này theo (1) cho bao hàm thức đảo lại.

#### Mệnh đề 5 {#ts-i-s7-prop-5 .statement tag=02G9}

Cho E là một không gian Hilbert phức và $u$ là một tự đồng cấu chuẩn tắc của E.

a) Với mọi tập con H vừa mở vừa đóng của phổ của $u$, phép chiếu phổ $e_H(u)$ là một phép chiếu trực giao mà hạt nhân của nó là ảnh của phép chiếu phổ $e_{Sp(u)-H}(u)$ ;

b) Nếu $H_1$ và $H_2$ là các tập con vừa mở vừa đóng rời nhau của phổ của $u$, thì các không gian con phổ $E_{H_1}$ và $E_{H_2}$ trực giao ;

c) Nếu $\lambda \in \mathbf{C}$ là một điểm cô lập của phổ của $u$, thì $\lambda$ là một trị riêng của $u$ và ảnh của phép chiếu phổ $e_{\lambda}(u)$ là không gian riêng của $u$ ứng với $\lambda$.

Hãy chứng minh a). Vì phép tính phiếm hàm chỉnh hình tương thích với phép tính phiếm hàm liên tục (I, p. 111, hệ quả 1), ta có $e_H(u) =\varphi_H(u)$, trong đó $\varphi_H\in \mathscr{C}$ (Sp($u$)) là hàm đặc trưng của H. Điều này kéo theo $e_H(u)^*=\overline{\varphi}_H(u) =\varphi_H(u) =e_H(u)$, do đó $e_H(u)$ là một phép chiếu trực giao (bổ đề 3, (ii)). Hạt nhân của nó là ảnh của phép chiếu $1-e_H(u) =e_{Sp(u)-H}(u)$.

Hãy chứng minh b). Các hàm đặc trưng $\varphi_{H_1}$ và $\varphi_{H_2}$ của $H_1$ và $H_2$ trong Sp($u$) là liên tục và tích của chúng bằng không, điều này kéo theo $e_{H_1}(u)\circ e_{H_2}(u) =e_{H_2}(u)\circ e_{H_1}(u) = 0$. Suy ra các bao hàm $E_{H_2}(u)\subset E_{H_1}(u)^{\circ}$ và $E_{H_1}(u)\subset E_{H_2}(u)^{\circ}$.

Sau cùng, hãy chứng minh mệnh đề c). Hàm đặc trưng $\varphi_{\lambda}$ của $\{\lambda \}$ là liên tục và khác không trên Sp($u$) ; nó thỏa mãn $(z-\lambda )\varphi_{\lambda}(z) = 0$ với mọi $z\in$ Sp($u$). Do đó ta có $(u-\lambda 1_E)\varphi_{\lambda}(u) = 0$. Vậy ảnh của $\varphi_{\lambda}(u)$, vốn khác không, được chứa trong không gian con thực sự của $u$ ứng với $\lambda$. Vì ta có $e_{\lambda}(u) =\varphi_{\lambda}(u)$ và ảnh của $e_{\lambda}(u)$ chứa không gian con thực sự của $u$ ứng với $\lambda$, mệnh đề được suy ra.

#### Bổ đề 4 {#ts-i-s7-lem-4 .statement tag=02GA}

Cho E là một không gian Hilbert và $u$ là một tự đồng cấu chuẩn tắc của E. Cho F là một không gian con đóng của E chứa một tập hợp toàn phần các vectơ riêng của $u$. Khi đó $F^{\circ}$ ổn định dưới tác động của $u$ và tự đồng cấu $\widetilde{u}$ của $F^{\circ}$ suy ra từ $u$ là chuẩn tắc.

Vì $u$ là chuẩn tắc, mọi vectơ riêng của $u$ cũng là một vectơ riêng của $u^*$ (EVT, V, p. 43, hệ quả). Do đó giả thiết kéo theo F ổn định dưới tác động của $u$ và của $u^*$. Theo EVT, V, p. 41, mệnh đề 4 (ii), vì thế ta có $u(F^{\circ})\subset F^{\circ}$ và $u^*(F^{\circ})\subset F^{\circ}$. Suy ra liên hợp của $\widetilde{u}$ là tự đồng cấu của $F^{\circ}$ suy ra từ $u^*$. Vì $u$ là chuẩn tắc, tự đồng cấu $\widetilde{u}$ là chuẩn tắc.

### 6. Ảnh số

#### Định nghĩa 2 {#ts-i-s7-def-2 .statement tag=02GB}

Cho E là một không gian Hilbert phức và $u$ là một tự đồng cấu của E. **Ảnh số** của $u$ là tập hợp các số phức có dạng $\langle x|u(x)\rangle$, trong đó $x$ chạy qua mặt cầu đơn vị của E. Ta ký hiệu bởi $\iota (u)$ ảnh số của $u$.

Ảnh số của $u^*$ là ảnh của $\iota (u)$ qua phép liên hợp phức. Với mọi số phức $\lambda$ và $\mu$, ảnh số của $\lambda u+\mu1_E$ bằng $\lambda \iota (u) +\mu$.

#### Mệnh đề 6 {#ts-i-s7-prop-6 .statement tag=02GC}

Cho E là một không gian Hilbert phức và $u$ là một tự đồng cấu của E.

a) Tập hợp các trị riêng của $u$ được chứa trong $\iota (u)$;

b) phổ của $u$ được chứa trong bao đóng của $\iota (u)$ trong $\mathbf{C}$.

Cho $\lambda$ là một trị riêng của $u$ và cho $x\in E$ là một vectơ khác không sao cho $u(x) =\lambda x$. Nếu cần, thay thế $x$ bởi $x/\|x\|$, ta có thể giả sử rằng $\|x\|= 1$. Khi đó $\langle x|u(x)\rangle =\lambda$, do đó $\lambda \in \iota (u)$.

Hãy chứng minh b). Xét $u-\lambda 1_E$, ta được quy về việc chứng minh rằng nếu 0 thuộc phổ của $u$, thì 0 là điểm dính của $\iota (u)$.

Trước hết giả sử rằng tồn tại một số thực $c >$ 0 sao cho $\|u(x)\|\geqslant c$ với mọi $x$ có chuẩn 1 trong E. Khi đó tự đồng cấu $u$ là đơn ánh và đóng (Bổ đề 8 của I, p. 107). Vì theo giả thiết nó không khả nghịch, nên nó không toàn ánh. Do đó trực giao bổ sung của hạt nhân của $u^*$ không bằng E (EVT, V, p. 41, Mệnh đề 4), điều này chứng minh rằng hạt nhân của $u^*$ không thu về 0. Vậy 0 thuộc $\iota (u^*)$, nên thuộc $\iota (u)$.

Nếu giả thiết trước không được thỏa mãn, thì với mọi số nguyên $n\geqslant 1$, tồn tại một vectơ $x_n$ có chuẩn 1 trong E sao cho $\|u(x_n)\|\leqslant 1/n$. Khi đó ta có $|\langle x_n|u(x_n)\rangle |\leqslant 1/n$, điều này kéo theo rằng 0 thuộc bao đóng của $\iota (u)$.

Mệnh đề 7 (Định lý Hausdorff-Toeplitz)

Cho E là một không gian Hilbert phức và cho $u\in \mathscr{L}(E)$. Miền giá trị số $\iota (u)$ là một tập con lồi của $\mathbf{C}$.

Ta sẽ cần hai bổ đề để chứng minh mệnh đề này.

#### Bổ đề 5 {#ts-i-s7-lem-5 .statement tag=02GD}

Cho E là một không gian Hilbert phức chiều 2. Hãy biến không gian vectơ thực $\mathscr{L}(E)_h$ của các tự đồng cấu Hermit của E thành một không gian tiền Hilbert có chuẩn bằng chuẩn $u\mapsto$ Tr($u^*u$)$^{1/2}$. Tập hợp các

$$
\surd
$$

phép chiếu trực giao hạng 1 của E là mặt cầu S bán kính $1/$ 2 tâm tại $\frac{1}{2}1_E$ trong không gian con afin chiều 3 của các tự đồng cấu có vết bằng 1 trong $\mathscr{L}(E)_h$.

Cho F là không gian con afin thực của $\mathscr{L}(E)_h$ gồm các phần tử có vết bằng 1. Các phép chiếu trực giao hạng 1 của E thuộc F (Bổ đề 3, (ii)).

Cho $u\in F$. Ta có $\|u-\frac{1}{2}1_E\|^2=$ Tr($u^2-u+\frac{1}{4}$) $=$ Tr($u^2$)$-\frac{1}{2}$. Do đó, $u\in S$ khi và chỉ khi Tr($u^2$) $= 1$. Vì 2 det($u$) $=$ Tr($u$)$^2-$ Tr($u^2$) $= 1-$ Tr($u^2$), điều kiện này tương đương với det($u$) $= 0$. Theo định lý Hamilton–Cayley (A, III, p. 107, prop. 20), vậy ta có $u\in S$ khi và chỉ khi $u^2-u= 0$, điều đó có nghĩa là $u$ là một phép chiếu Hermit hạng 1 (loc. cit.), do đó suy ra kết quả.

#### Bổ đề 6 {#ts-i-s7-lem-6 .statement tag=02GE}

Cho E là một không gian vectơ thực định chuẩn, F là một không gian vectơ thực, và $u: E\rightarrow F$ là một ánh xạ afin không đơn ánh. Gọi B là một quả cầu trong E và S là mặt cầu tương ứng. Khi đó $u(S) =$ $u(B)$, và đặc biệt, $u(S)$ là lồi.

Ta rút gọn về trường hợp $u$ là tuyến tính và B là quả cầu đơn vị của E. Ta có $u(S)\subset u(B)$. Ngược lại, cho $x\in B$ và cho $y$ là một phần tử khác không của Ker($u$). Ảnh của ánh xạ liên tục $t\mapsto  \|x+ty\|$ từ $\mathbf{R}$ vào $\mathbf{R}_+$ là một khoảng không bị chặn chứa số thực $\|x\|\leqslant 1$. Vậy tồn tại $t\in \mathbf{R}$ sao cho $\|x+ty\|= 1$. Khi đó $x+ty\in S$ và $u(x+ty) =u(x)$, suy ra $u(x)\in u(S)$.

Hãy chứng minh prop. 7. Cho $x$ và $y$ là các phần tử của mặt cầu đơn vị của E; hãy chứng minh rằng đoạn có hai đầu mút $\langle x|u(x)\rangle$ và $\langle y|u(y)\rangle$ được chứa trong ảnh số của $u$.

Gọi F là không gian con của E sinh bởi $x$ và $y$. Nếu dim(F) = 1, ta có $\langle x|u(x)\rangle =\langle y|u(y)\rangle$, do đó suy ra mệnh đề. Nếu không, dim(F) = 2; khi đó gọi $p$ là phép chiếu trực giao của E có ảnh là F, và ký hiệu bởi $u_F$ tự đồng cấu của F xác định bởi $x\mapsto p(u(x))$. Vì $p$ là Hermit (bổ đề 3 của I, p. 133), ta có $\langle z|u_F(z)\rangle =\langle z|u(z)\rangle$ với mọi $z\in F$, nên $\iota (u_F)\subset \iota (u)$. Vì vậy ta có thể giả sử rằng E = F.

Với mọi phần tử $z$ của E, ký hiệu $v_z$ là tự đồng cấu Hermit của E được xác định bởi $t\mapsto  \langle z|t\rangle z$; ta có $\langle z|u(z)\rangle =$ Tr($u\circ v_z$). Khi $z$ chạy qua mặt cầu đơn vị của E$,v_z$ chạy qua tập hợp các phép chiếu trực giao hạng 1 của E, là một mặt cầu S trong không gian con afin thực V của $\mathscr{L}(E)$ gồm các tự đồng cấu Hermit của E có vết bằng 1 (bổ đề 5). Vì vậy ảnh số của E là tập hợp các Tr($u\circ v$), với $v\in S$. Ánh xạ $v\mapsto$ Tr($u\circ v$) từ V vào $\mathbf{C}$ là tuyến tính. Vì dim$_{\mathbf{R}}(V) = 3>$ dim$_{\mathbf{R}}(\mathbf{C})$, nó không đơn ánh; do đó từ bổ đề 6 suy ra rằng $\iota (u)$ là lồi.

### 7. Các Phần Tử Dương

Cho E là một không gian Hilbert phức. Cho $u$ là một tự đồng cấu của E. Nhắc lại (EVT, V, p. 45, định nghĩa 6) rằng $u$ được gọi là dương nếu ta có $\langle x|u(x)\rangle \geqslant 0$ với mọi $x\in E$. Khi đó tự đồng cấu $u$ là Hermit (loc. cit.). Hơn nữa, nếu F là một không gian Hilbert phức và nếu $v\in$ $\mathscr{L}(F; E)$, thì tự đồng cấu $v^*uv$ của F là dương (EVT, V, p. 45, mệnh đề 12).

#### Mệnh đề 8 {#ts-i-s7-prop-8 .statement tag=02GF}

Cho E là một không gian Hilbert phức. Cho $u$ là một tự đồng cấu của E. Các điều kiện sau là tương đương:

(i) Tự đồng cấu $u$ là dương;

(ii) Ảnh số của $u$ được chứa trong $\mathbf{R}_+$;

(iii) Tự đồng cấu $u$ là một phần tử dương của đại số có đối hợp $\mathscr{L}(E)$ ;

(iv) Tồn tại một phần tử Hermit $v$ của $\mathscr{L}(E)$ sao cho $u=v^2$;

(v) Tồn tại một ánh xạ tuyến tính liên tục $v$ từ E vào một không gian Hilbert phức F sao cho $u=v^*v$.

Theo EVT, V, p. 45, định nghĩa $6,u$ là dương nếu và chỉ nếu nó là Hermit và nếu $\langle x|u(x)\rangle \geqslant 0$ với mọi $x\in E$. Do đó hệ quả (i) $=\Rightarrow$ (ii) suy ra từ định nghĩa của ảnh số.

(ii) $=\Rightarrow$ (iii) : giả thiết kéo theo rằng $u$ là Hermit (EVT, V, p. 45, và nhận xét, p. 2) và phổ của nó được chứa trong $\mathbf{R}_+$ (mệnh đề 6) ; vì thế $u$ là một phần tử dương của đại số có đối hợp $\mathscr{L}(E)$.

(iii) $=\Rightarrow$ (iv) : đây là một trường hợp riêng của mệnh đề 16 của I, p. 118.

(iv) $=\Rightarrow$ (v) là ngay lập tức.

(v) $=\Rightarrow$ (i) : cho F là một không gian Hilbert phức và cho $v\in \mathscr{L}(E; F)$ sao cho $u=v^*v$. Cho $x\in E$. Ta có $\langle x|u(x)\rangle =\langle x|(v^*v)(x)\rangle =\|v(x)\|^2$, điều này chứng minh rằng $u$ là dương.

Nhắc lại (EVT, V, p. 45, nhận xét 1) rằng, với mọi phần tử Hermit $u$ của $\mathscr{L}(E)$, ta đặt

$m(u) =$ inf$_{\|xx\in\|=1E}\langle x|u(x)\rangle =$ inf $\iota (u) =$ inf$_{x\in E-\{0\}}\frac{\langle x|u(x)\rangle}{\|x\|^2}$,

$M(u) =$ sup$_{x\in E}\langle x|u(x)\rangle =$ sup $\iota (u) =$ sup$_{x\in E-\{0\}}\frac{\langle x|u(x)\rangle}{\|x\|^2}$.

$\|x\|=1$

Nếu $E =\{0\}$, ta có $M(u) =-\infty ,m(u) = +\infty$ và $\iota (u) =\emptyset$.

Giả sử $E$ khác không; khi đó ta có $m(u)\leqslant M(u)$ và ảnh số của $u$ là một khoảng có hai đầu mút là $m(u)$ và $M(u)$. Theo Mệnh đề 6, Sp($u$) được chứa trong khoảng $[m(u),M(u)]$. Chính xác hơn:

#### Mệnh đề 9 {#ts-i-s7-prop-9 .statement tag=02GG}

Cho $E$ là một không gian Hilbert phức và $u$ là một phần tử Hermit của $\mathscr{L}(E)$.

a) Ta có $m(u) =$ inf Sp($u$) và $M(u) =$ sup Sp($u$) ;

b) Nếu $E$ khác không, ta có $\|u\|=$ sup($|m(u)|,|M(u)|$).

Cho $\lambda \in \mathbf{R}$. Để $\lambda$ là một cận dưới của phổ của $u$, điều kiện cần và đủ là $u-\lambda \geqslant 0$. Điều này tương đương (Mệnh đề 8, (ii)) với điều kiện $\langle x|u(x)\rangle \geqslant \lambda \|x\|^2$ với mọi $x\in E$, tức là với $m(u)\geqslant \lambda$. Điều này chứng tỏ rằng $m(u)$ là cận dưới lớn nhất của Sp($u$). Tương tự, ta kiểm tra được rằng $M(u)$ là cận trên nhỏ nhất của Sp($u$).

Vì $u$ là chuẩn tắc, ta có $\varrho (u) =\|u\|$ (Hệ quả 1 của I, p. 108). Vì $E\not=\{0\}$, phổ của $u$ không rỗng (Hệ quả 1 của I, p. 26) và $\varrho (u)$ là bán kính của đĩa nhỏ nhất có tâm 0 và chứa Sp($u$) (Định lý 1 của I, p. 24), do đó b) suy ra từ a).

### 8. Phân tích cực

Trong số này, ta xét các không gian Hilbert phức.

Cho $E_1$ và $E_2$ là các không gian Hilbert và $u\in \mathscr{L}(E_1; E_2)$. Tự đồng cấu $u^*u$ của $E_1$ là dương (Mệnh đề 8), do đó ta có thể lập phần tử dương $(u^*u)^{1/2}$ của $\mathscr{L}(E_1)$.

#### Định nghĩa 3 {#ts-i-s7-def-3 .statement tag=02GH}

Ta nói rằng $(u^*u)^{1/2}$ là giá trị tuyệt đối của $u$, và ký hiệu nó bởi $|u|$.

Trong trường hợp $E_1= E_2$, định nghĩa này trùng với định nghĩa đã cho trong Nhận xét 9 của I, p. 119.

Đối với một phần tử $u$ của $\mathscr{L}(E_1; E_2)$, nhắc lại rằng (EVT, V, p. 41, Định nghĩa 2) không gian con ban đầu của $u$ là không gian con đóng Ker($u$)$^{\circ}$ của $E_1$ và không gian con cuối của $u$ là không gian con đóng Im($u$) của $E_2$.

#### Mệnh đề 10 {#ts-i-s7-prop-10 .statement tag=02GI}

Cho $E_1$ và $E_2$ là các không gian Hilbert phức và cho $u\in \mathscr{L}(E_1; E_2)$.

a) Không gian con ban đầu và không gian con cuối của $|u|$ đều bằng không gian con ban đầu của $u$ và ta có $\||u|\|=\|u\|$;

b) Tồn tại một ánh xạ đẳng cự từng phần duy nhất $j$ từ $E_1$ vào $E_2$ sao cho Ker($j$) $=$ Ker($u$) và $u=j|u|$;

c) Không gian con ban đầu (tương ứng, cuối) của $j$ bằng không gian con ban đầu (tương ứng, cuối) của $u$;

d) Cho $u_1$ là một phần tử dương của $\mathscr{L}(E_1)$ và $j_1$ là một phần tử đẳng cự từng phần của $\mathscr{L}(E_1; E_2)$ sao cho $u=j_1u_1$ và Ker($j_1$) $=$ Ker($u_1$). Khi đó $u_1=|u|$ và $j_1=j$.

Với mọi $x\in E_1$, ta có

$$
\|u(x)\|^2=\langle x|(u^*u)(x)\rangle =\langle x||u|^2(x)\rangle =\||u|(x)\|^2 \tag{2}
$$

Điều này chứng tỏ rằng Ker($u$) $=$ Ker($|u|$) và $\||u|\|=\|u\|$. Vì $|u|$ là Hermit, bao đóng của ảnh của $|u|$ là trực giao bù của hạt nhân của nó (EVT, V, p. 41, mệnh đề 4), tức là không gian ban đầu của $u$, do đó suy ra a).

Công thức (2) kéo theo rằng tồn tại một ánh xạ đẳng cự $v$ từ Im($|u|$) lên Im($u$) sao cho $v(|u|(x)) =u(x)$ với mọi $x\in E_1$. Gọi $j$ là phần tử duy nhất của $\mathscr{L}(E_1; E_2)$ mở rộng $v$ và triệt tiêu trên Im($|u|$)$^{\circ}=$ Ker($|u|$) $=$ Ker($u$). Khi đó $j$ có các tính chất của b). Tính duy nhất của $j$ suy ra từ phân tích E = Ker($u$)$\oplus$ Im($|u|$).

Không gian ban đầu của $j$ là Ker($j$)$^{\circ}=$ Ker($u$)$^{\circ}$, tức không gian ban đầu của $u$. Không gian cuối của nó là $j$(Ker($u$)$^{\circ}$) $=j$(Im($|u|$)) $=$ Im($u$), tức không gian cuối của $u$. Điều này chứng minh c).

Bây giờ cho $u_1$ và $j_1$ như trong d). Ta có $u^*u=u_1j_1^*j_1u_1$. Ánh xạ $j_1^*j_1$ là phép chiếu trực giao có hạt nhân Ker($j_1$) $=$ Ker($u_1$) (EVT, V, p. 41, mệnh đề 5 (ii)) và do đó có ảnh là Im($u_1$). Vậy $u^*u=u^2_1$ và do đó $u_1= (u^*u)^{1/2}=|u|($I, p. 118, mệnh đề 16). Mệnh đề về tính duy nhất trong b) sau cùng suy ra rằng $j_1=j$.

#### Định nghĩa 4 {#ts-i-s7-def-4 .statement tag=02GJ}

Cho $E_1$ và $E_2$ là các không gian Hilbert phức và $u\in \mathscr{L}(E_1; E_2)$. Cặp $(j,|u|)$, trong đó $j$ là ánh xạ đẳng cự riêng phần duy nhất từ $E_1$ vào $E_2$ sao cho $u=j|u|$ và Ker($j$) $=$ Ker($u$), được gọi là phân tích cực của $u$.

#### Mệnh đề 11 {#ts-i-s7-prop-11 .statement tag=02GK}

Cho $E_1$ và $E_2$ là các không gian Hilbert phức và $u\in \mathscr{L}(E_1; E_2)$. Gọi $(j,|u|)$ là phân tích cực của $u$.

a) Ta có $|u|=j^*u=u^*j$;

b) Ta có $|u^*|=ju^*=uj^*$;

c) Phân tích cực của $u^*$ là $(j^*,|u^*|)$.

Đặt I = Ker($u$)$^{\circ}$ và F = Im($u$) là không gian con ban đầu và không gian con cuối của $u$; hơn nữa, ta có I = Ker($|u|$)$^{\circ}=$ Im($|u|$) (mệnh đề 10, a)). Ánh xạ $j^*j$ là phép chiếu trực giao của $E_1$ lên I (loc. cit. và EVT, V, p. 41, mệnh đề 5 (ii)). Do đó $j^*u=j^*j|u|=|u|$, rồi $u^*j= (j^*u)^*=|u|^*=|u|$, do đó suy ra a).

Tương tự, ta tính được $u^*$ = $|u|j^*= (j^*j|u|)j^*$ = $j^*(j|u|j^*)$. Tự đồng cấu $j|u|j^*$ của $E_2$ là dương. Ánh xạ tuyến tính $j^*$ là đẳng cự riêng phần, với không gian ban đầu là F và không gian cuối là I (EVT, V, p. 41, Mệnh đề 5), và các ánh xạ tuyến tính từ I vào F (resp. từ F vào I) suy ra từ $j$ và $j^*$ bằng cách chuyển sang các không gian con là các đẳng cấu nghịch đảo của nhau (loc. cit.). Do đó Ker($j|u|j^*$) $=$ Ker($|u|j^*$) $=$ Ker($j^*$), vì ảnh của $j^*$ được chứa trong Ker($u$)$^{\circ}=$ Ker($|u|$)$^{\circ}$. Theo Mệnh đề 10, d), cặp $(j^*, j|u|j^*)$ là phân tích cực của $u^*$. Điều này chứng minh c), và khi đó mệnh đề b) được suy ra từ mệnh đề a) áp dụng cho $u^*$.

#### Hệ quả {#ts-i-s7-n8-cor-1 .statement tag=02GL}

Cho $E_1$ và $E_2$ là các không gian Hilbert phức và cho $u\in \mathscr{L}(E_1; E_2)$. Khi đó Im($u$) $=$ Im($|u^*|$).

Gọi $(j,|u|)$ là phân tích cực của $u$. Ta có $|u^*|=j|u|j^*=uj^*$ theo mệnh đề trước. Theo EVT, V, p. 41, Mệnh đề 5, ánh xạ $j^*$ là đẳng cự riêng phần. Không gian cuối của nó là Ker($j$)$^{\circ}=$ Ker($u$)$^{\circ}$ (Mệnh đề 10, c)). Mệnh đề được suy ra.

#### Mệnh đề 12 {#ts-i-s7-prop-12 .statement tag=02GM}

Cho $E_1$ và $E_2$ là các không gian Hilbert phức và $u\in \mathscr{L}(E_1; E_2)$. Cho $(j,|u|)$ là phân tích cực của $u$. Để $u$ là song ánh, điều kiện cần và đủ là $|u|$ khả nghịch trong $\mathscr{L}(E_1)$ và $j$ là một đẳng cấu từ $E_1$ lên $E_2$.

Điều kiện ấy là đủ. Ngược lại, nếu $u$ là song ánh, thì $u^*u$ khả nghịch trong $\mathscr{L}(E_1)$, và $|u|= (u^*u)^{1/2}$ cũng khả nghịch vì phổ của nó được chứa trong $\mathbf{R}_+^*$. Hơn nữa, Ker($j$) $=$ Ker($u$) $=\{0\}$ và Im($j$) $=$ Im($u$) $= F$, do đó $j$ ánh xạ đẳng cự $E_1$ lên $E_2$.

#### Mệnh đề 13 {#ts-i-s7-prop-13 .statement tag=02GN}

Cho E là một không gian Hilbert phức và $u$ là một tự đồng cấu của E. Các điều kiện sau là tương đương:

(i) Tự đồng cấu $u$ là chuẩn tắc;

(ii) Tồn tại một phần tử unita $v$ của $\mathscr{L}(E)$, giao hoán với $|u|$, sao cho $u=v|u|$.

Cho $(j,|u|)$ là phân tích cực của $u$. Giả sử rằng $u$ là chuẩn. Khi đó $|u^*|= (uu^*)^{1/2}= (u^*u)^{1/2}=|u|$. Mệnh đề 11 khi đó suy ra rằng $|u|j=|u^*|j=ju^*j=j|u|$. Hơn nữa, $j$ để ổn định các không gian con trực giao bù nhau Ker($|u|$) $=$ Ker($j$) và Im($|u|$) $=$ Im($j$) (mệnh đề 10). Cho $v$ là phần tử của $\mathscr{L}(E)$ trùng với $j$ trên Ker($u$)$^{\circ}$ và với ánh xạ đồng nhất trên Ker($u$). Vì $j$ cảm sinh một phép đẳng cự từ Ker($u$)$^{\circ}$ lên Im($u$) $=$ Ker($u^*$)$^{\circ}=$ Ker($u$)$^{\circ}$ (vì $u$ là chuẩn), tự đồng cấu $v$ là unita; hơn nữa, nó giao hoán với $|u|$, vì $j|u|=|u|j$, và ta có $u=v|u|$.

Ngược lại, cho $v$ là một phần tử unita của $\mathscr{L}(E)$, giao hoán với $|u|$, sao cho $u=v|u|$. Ta có $uu^*=v|u|^2v^*=|u|^2vv^*=|u|^2=u^*u$, do đó $u$ là chuẩn.

Cho E là một không gian Hilbert phức và $u\in \mathscr{L}(E)$. Cho $(j,|u|)$ là phân tích cực của $u$. Có thể xảy ra rằng $j$ giao hoán với $|u|$ mà $u$ không chuẩn (Bài tập 11 của I, p. 189).

## BÀI TẬP {#ts-i-s7-exercises}

Trong các bài tập dưới đây, mọi không gian Banach đều trên $\mathbf{C}$.

Xem [các bài tập cho § 7](exercises/s7/).
