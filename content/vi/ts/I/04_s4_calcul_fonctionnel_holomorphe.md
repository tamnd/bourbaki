---
book: ts
book_title: Théories spectrales
chapter: I
chapter_title: ALGÈBRES NORMÉES
section: 4
section_title: Calcul fonctionnel holomorphe
lang: vi
source: ts-i-ii-fr
book_pages: TS I.49-TS I.88, TS I.172-TS I.177
pdf_pages: 0062-0101, 0185-0190
extraction: native
subsections:
    - "no": 1
      title: Germes de fonctions holomorphes
      page: 49
      pdf_page: 62
    - "no": 2
      title: Énoncé du théorème principal
      page: 51
      pdf_page: 64
    - "no": 3
      title: Suites adaptées et formes différentielles associées
      page: 52
      pdf_page: 65
    - "no": 4
      title: Construction des applications $\Theta_{\boldsymbol{a}}$
      page: 58
      pdf_page: 71
    - "no": 5
      title: Propriétés des applications $\Theta_{\boldsymbol{a}}$
      page: 61
      pdf_page: 74
    - "no": 6
      title: Théorèmes d’approximation
      page: 67
      pdf_page: 80
    - "no": 7
      title: Existence et unicité du calcul fonctionnel holomorphe
      page: 70
      pdf_page: 83
    - "no": 8
      title: Substitution dans le calcul fonctionnel
      page: 72
      pdf_page: 85
    - "no": 9
      title: Calcul fonctionnel holomorphe en une variable
      page: 74
      pdf_page: 87
    - "no": 10
      title: Exponentielle et logarithme
      page: 78
      pdf_page: 91
    - "no": 11
      title: Partitions de l’espace des caractères
      page: 79
      pdf_page: 92
    - "no": 12
      title: Partitions du spectre d’un élément
      page: 81
      pdf_page: 94
    - "no": 13
      title: Calcul fonctionnel holomorphe dans une algèbre normable complète réelle ou complexe
      page: 85
      pdf_page: 98
    - "no": 14
      title: Cas d’une algèbre sans élément unité
      page: 88
      pdf_page: 101
statements: 55
exercises: 18
content_sha256: a830aec5cd6b5c1f8c27cedded031342be71cf89e03ce3d72129c3770c2a3cb7
translated_from: content/en-mt/ts/I/04_s4_calcul_fonctionnel_holomorphe.md
source_lang: en-mt
translation_method: machine
source_content_sha256: bfd3dd87c3f14314ac07c57cc45fa868c6aacf7968e0d4fd61ff3372c2d96b1d
translation_model: gpt-5.4
translation_run: translate-vi-9819947a
glossary_version: 34
glossary_terms_sha256: 4234d5c09fa6917e2cd55eb962c9bb39bb0a3c83854566d50d2ba825e7094568
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 4. PHÉP TÍNH PHIẾM HÀM CHỈNH HÌNH

### 1. Mầm của các hàm chỉnh hình

Cho E và F là các không gian Banach phức. Ta nhắc lại (x. VAR, R1, p. 26, 3.2.1, p. 22, 3.1 và p. 88, App.) rằng một ánh xạ chỉnh hình xác định trên một tập mở U của E và nhận giá trị trong F là một ánh xạ $f: U\rightarrow F$ sao cho, với mọi $x\in U$, tồn tại một chuỗi hội tụ

$$
f_x=\sum_{k\geqslant 0}f_{x,k}
$$

thỏa mãn $f(x+y) =f_x(y)$ với mọi $y\in E$ đủ gần 0, trong đó $f_{x,k}: E\rightarrow \mathbf{C}$ là một đa thức thuần nhất liên tục bậc $k$ trên E nhận giá trị trong F, nghĩa là một ánh xạ có dạng

$$
f_{x,k}(y) =\widetilde{f}_{x,k}(y, . . . , y)
$$

trong đó $\widetilde{f}_{x,k}: E^k\rightarrow F$ là một ánh xạ $k$-tuyến tính liên tục. Ta ký hiệu bởi $\mathscr{O}(U; F)$ không gian vectơ phức các hàm chỉnh hình trên U nhận giá trị trong F, được trang bị tôpô hội tụ compact. Đó là một không gian vectơ tôpô lồi địa phương, mà tôpô được xác định bởi các bán chuẩn $f\mapsto$ sup$_{z\in K}\|f(z)\|$, trong đó K chạy qua tập hợp các tập con compact của U.

Cho G là một không gian Banach phức và V là một tập con mở của G. Với mọi ánh xạ chỉnh hình $\varphi : V\rightarrow$ U, ánh xạ $\varphi^*:f\mapsto f\circ \varphi$ là một ánh xạ tuyến tính liên tục từ $\mathscr{O}(U; F)$ vào $\mathscr{O}(V; F)$.

Nếu H là một không gian Banach phức và $\varphi : F\rightarrow H$ là một ánh xạ tuyến tính liên tục, thì ánh xạ $f\mapsto \varphi \circ f$ là một ánh xạ tuyến tính liên tục từ $\mathscr{O}(U; F)$ vào $\mathscr{O}(U; H)$, được ký hiệu bởi $\varphi_*$.

Cho $n$ là một số tự nhiên và đặt $E =\mathbf{C}^n$. Cho K là một tập con compact của $\mathbf{C}^n$ và $\mathscr{U}$ là tập có hướng giảm các lân cận mở của K. Nếu $U,U'\in \mathscr{U}$ và $U'\subset U$, thì ánh xạ hạn chế các hàm từ $\mathscr{O}(U; F)$ vào $\mathscr{O}(U'; F)$ là liên tục. Giới hạn quy nạp của các không gian $\mathscr{O}(U; F)$ đối với các ánh xạ này được ký hiệu bởi $\mathscr{O}(K; F)$. Các phần tử của $\mathscr{O}(K; F)$ được gọi là các mầm của các hàm chỉnh hình trong một lân cận của K và nhận giá trị trong F.

Không gian $\mathscr{O}(K; F)$ được trang bị tôpô giới hạn quy nạp của các tôpô lồi địa phương của các $\mathscr{O}(U; F)$ (EVT, II, p. 31, ví dụ II). Cho X là một không gian vectơ tôpô lồi địa phương và $\varphi :\mathscr{O}(K; F)\rightarrow X$ là một ánh xạ. Với mọi lân cận mở U của K, ánh xạ $\mathscr{O}(U; F)\rightarrow X$ suy ra từ $\varphi$ bằng hợp thành với ánh xạ chính tắc $\mathscr{O}(U; F)\rightarrow \mathscr{O}(K; F)$ được ký hiệu bởi $\varphi^U$. Ánh xạ $\varphi$ là liên tục khi và chỉ khi $\varphi^U$ là liên tục với mọi U (EVT, II, p. 29, prop. 5, (iii)).

Cho $m$ là một số tự nhiên. Cho L là một tập con compact của $\mathbf{C}^m$ và V là một lân cận mở của L. Cho $\varphi : V\rightarrow \mathbf{C}^n$ là một ánh xạ chỉnh hình sao cho $\varphi (L)\subset K$. Các ánh xạ tuyến tính liên tục

$-1$

$$
\mathscr{O}(U; F)^{\varphi}\leftarrow^{^*}\rightarrow \mathscr{O}(\overset{-1}{\varphi}(U); F)^{\varphi^{\varphi}}\leftarrow^{^{(U)}}\rightarrow \mathscr{O}(L; F)
$$

với U là một lân cận mở của K, cảm sinh một ánh xạ tuyến tính liên tục $\varphi^*:\mathscr{O}(K; F)\rightarrow \mathscr{O}(L; F)$ (loc. cit.).

Cho H là một không gian Banach phức và $\varphi : F\rightarrow H$ là một ánh xạ tuyến tính liên tục. Các ánh xạ tuyến tính liên tục

$$
\mathscr{O}(U; F)^{\varphi}\leftarrow_{_*}\rightarrow \mathscr{O}(U; H)^{\varphi}\leftarrow^{^U}\rightarrow \mathscr{O}(K; F)
$$

trong đó U chạy qua tập hợp các lân cận mở của K trong $\mathbf{C}^n$, cảm sinh một ánh xạ tuyến tính liên tục $\varphi_*$ từ $\mathscr{O}(K; F)$ vào $\mathscr{O}(K; H)$ (loc. cit.). Đôi khi ta sẽ viết $\varphi \circ f=\varphi_*(f)$.

Với mọi lân cận mở U của K, phép hạn chế lên K là một ánh xạ tuyến tính liên tục $\mathscr{O}(U; F)\rightarrow \mathscr{C}(K; F)$; các ánh xạ này cảm sinh một ánh xạ tuyến tính liên tục $\mathscr{O}(K; F)\rightarrow \mathscr{C}(K; F)$, được gọi là sự đánh giá các mầm của các hàm chỉnh hình trên K.

Cho A là một đại số Banach phức có đơn vị. Các không gian $\mathscr{O}(U; A)$ và $\mathscr{O}(K; A)$ là những đại số có đơn vị. Nếu $A\not=\{0\}$, có thể đồng nhất một cách chính tắc $\mathscr{O}(U;\mathbf{C})$ (resp. $\mathscr{O}(K;\mathbf{C})$) với đại số con $\mathscr{O}(U;\mathbf{C})\cdot 1$ của $\mathscr{O}(U; A)$ (resp. với đại số con $\mathscr{O}(K;\mathbf{C})\cdot 1$ của $\mathscr{O}(K; A)$). Ta sẽ đặt $\mathscr{O}(U) =\mathscr{O}(U;\mathbf{C})$ và $\mathscr{O}(K) =\mathscr{O}(K;\mathbf{C})$.

### 2. Phát biểu của định lý chính

Cho X là một tập hợp. Nếu $m\leqslant n$, ta sẽ ký hiệu bởi $\pi_{m,n}$ ánh xạ từ $X^n$ vào $X^m$ sao cho $\pi_{m,n}(\boldsymbol{x}) = (x_1, . . . , x_m)$ với mọi $\boldsymbol{x}= (x_1, . . . , x_n)\in X^n$.

Cho A là một đại số Banach có đơn vị trên $\mathbf{C}$. Với mọi số nguyên $n\geqslant 1$ và mọi $\boldsymbol{a}\in A^n$, ta ký hiệu bởi Sp$^n(\boldsymbol{a})$ phổ đồng thời Sp$^{\{1,...,n\}}_A(\boldsymbol{a})$ (định nghĩa 2 của I, p. 42). Đó là một tập con compắc của $\mathbf{C}^n$. Với mọi số nguyên $m$ sao cho $1\leqslant m\leqslant n$, ta có $\pi_{m,n}$(Sp$^n(\boldsymbol{a})$) $=$ Sp$^m(\pi_{m,n}(\boldsymbol{a}))$ (I, p. 41, n$^o6$). Ánh xạ tuyến tính liên tục

$\pi_{m,n}^*:\mathscr{O}$(Sp$^m(\pi_{m,n}(\boldsymbol{a})); A$)$\longrightarrow \mathscr{O}$(Sp$^n(\boldsymbol{a}); A$)

là một cấu xạ của các đại số có đơn vị.

Cho A là một đại số Banach giao hoán có đơn vị trên $\mathbf{C}$. Cho $n\geqslant 1$ là một số nguyên. Một phép tính phiếm hàm chỉnh hình theo $n$ biến trên A là việc cho, với mọi $\boldsymbol{a}\in A^n$, một ánh xạ

$\Theta_{\boldsymbol{a}}:\mathscr{O}$(Sp$^n(\boldsymbol{a}); A$)$\longrightarrow A$

thỏa mãn các điều kiện:

(CF1) Với mọi $\boldsymbol{a}\in A^n$, ánh xạ $\Theta_{\boldsymbol{a}}$ là một cấu xạ liên tục của các đại số có đơn vị.

(CF2) Nếu $\boldsymbol{a}= (a_1, . . . , a_n)$, và nếu $z_1, . . . , z_n$ ký hiệu các mầm trong lân cận của Sp$^n(\boldsymbol{a})$ của các hàm tọa độ trên $\mathbf{C}^n$, thì ta có

$$
\Theta_{\boldsymbol{a}}(z_1) =a_1, . . . ,\Theta_{\boldsymbol{a}}(z_n) =a_n
$$

#### Nhận xét {#ts-i-s4-n2-rem-1 .statement tag=029U}

Nếu căn của đại số A bằng không, có thể bỏ điều kiện liên tục trong (CF1) (x. mệnh đề 9 của I, p. 40).

Một phép tính phiếm hàm chỉnh hình trên A là việc cho, với mọi số nguyên $n\geqslant 1$, một phép tính phiếm hàm chỉnh hình theo $n$ biến trên A, thỏa mãn:

(CF3) Với mọi số nguyên $m$ và $n$ sao cho $1\leqslant m\leqslant n$, và với mọi $\boldsymbol{a}\in A^n$ và $f\in \mathscr{O}$(Sp$^m(\pi_{m,n}(\boldsymbol{a}); A)$, ta có

$$
\Theta_{\boldsymbol{a}}(\pi^*_{m,n}(f)) = \Theta_{\pi_{m,n}(\boldsymbol{a})}(f)
$$

Mục đích của đoạn này là chứng minh định lý sau:

#### Định lý 1 {#ts-i-s4-thm-1 .statement tag=029V}

Cho A là một đại số Banach phức giao hoán có đơn vị. Tồn tại duy nhất một phép tính phiếm hàm chỉnh hình trên A.

Chứng minh của định lý này sẽ chiếm các số $^{os}3$ đến 7.

### 3. Các dãy thích nghi và các dạng vi phân liên kết

Trong số này, và cho đến số 5, ta ký hiệu bởi A một đại số Banach phức giao hoán có đơn vị và bởi $n$ một số nguyên $\geqslant 1$.

Khi chúng tôi nói đến các hàm khả vi vô hạn trên một tập mở của $\mathbf{C}^n$, thì đó sẽ là vấn đề các hàm khả vi vô hạn đối với cấu trúc đa tạp thực nền tảng. Các khái niệm của phép tính vi phân được dùng sẽ liên hệ với cấu trúc này.

#### Định nghĩa 1 {#ts-i-s4-def-1 .statement tag=029W}

Cho $\boldsymbol{a}= (a_1, . . . , a_n)\in A^n$, cho $h:\mathbf{C}^n\rightarrow \mathbf{C}$ là một ánh xạ và cho $u_1, . . . , u_n$ là các ánh xạ từ $\mathbf{C}^n$ vào A. Ta nói rằng dãy $(h, u_1, . . . , u_n)$ thích nghi với $\boldsymbol{a}$ nếu

(i) Ánh xạ $h$ khả vi vô hạn, có giá compact, và bằng 1 trong một lân cận của Sp$^n(\boldsymbol{a})$ ;

(ii) Các ánh xạ $u_1, . . . ,u_n$ khả vi vô hạn ;

(iii) Với mọi $\boldsymbol{z}= (z_1, . . . , z_n)\in \mathbf{C}^n$, ta có

$$
h(\boldsymbol{z}) + (z_1-a_1)u_1(\boldsymbol{z}) +\cdots + (z_n-a_n)u_n(\boldsymbol{z}) = 1 \tag{1}
$$

Dạng vi phân bậc $2n$ trên $\mathbf{C}^n$, với các hệ số trong A, được xác định bởi

$$
\omega =\bigwedge_{i=1}^n(du_i\wedge dz_i)
$$

được gọi là dạng vi phân liên kết với $(h, u_1, . . . , u_n)$.

Nếu $(h, u_1, . . . , u_n)$ thích nghi với $\boldsymbol{a}$, thì bằng cách vi phân hóa (1), ta thu được đẳng thức

$$
dh=-\sum_{i=1}^nu_idz_i-\sum_{i=1}^n(z_i-a_i)du_i \tag{2}
$$

do đó, với mọi $i$ sao cho $1\leqslant i\leqslant n$, có quan hệ

$$
dh\wedge dz_i\wedge \bigwedge_{j\not=i}(du_j\wedge dz_j) =-(z_i-a_i)\omega \tag{3}
$$

#### Bổ đề 1 {#ts-i-s4-lem-1 .statement tag=029X}

Cho U là một tập mở của $\mathbf{C}^n$ và K là một tập compact của U. Tồn tại một ánh xạ khả vi vô hạn $h$ từ $\mathbf{C}^n$ vào $\mathbf{C}$, bằng 1 trên K và có giá compact được chứa trong U.

Cho V là một lân cận mở tương đối compact của K sao cho $\overline{V}$ được chứa trong U (TG, I, p. 65, prop. 10). Tồn tại một hàm khả vi vô hạn $h$ từ $\mathbf{C}^n$ vào $\mathbf{C}$ mà giá được chứa trong V và bằng 1 trên K (VAR, R1, p. 40, 5.3.6). Hàm này có các tính chất cần có.

#### Ví dụ {#ts-i-s4-n3-exa-1 .statement tag=029Y}

Giả sử rằng $n= 1$. Cho $a\in A$. Với mọi lân cận mở U của Sp($a$), tồn tại một ánh xạ khả vi vô hạn $h$ từ $\mathbf{C}$ vào $\mathbf{C}$ có giá compact được chứa trong U, bằng 1 trong một lân cận của Sp($a$) (VAR, R1, p. 40, 5.3.6). Đặt

$$
u(z) = (1-h(z))(z-a)^{-1}
$$

với $z\in \mathbf{C}-$ Sp($a$) và $u(z) = 0$ nếu $z\in$ Sp($a$). Cặp $(h, u)$ thích nghi với $a$ và dạng vi phân liên kết là $\omega =du\wedge dz$.

#### Bổ đề 2 {#ts-i-s4-lem-2 .statement tag=029Z}

Cho $\boldsymbol{a}= (a_1, . . . , a_n)\in A^n$. Tồn tại các ánh xạ khả vi vô hạn $v_1, . . . , v_n$ từ $\mathbf{C}^n-$ Sp$^n(\boldsymbol{a})$ vào A sao cho

$$
(z_1-a_1)v_1(\boldsymbol{z}) +\cdots + (z_n-a_n)v_n(\boldsymbol{z}) = 1
$$

với mọi $\boldsymbol{z}= (z_1, . . . , z_n)\in \mathbf{C}^n-$ Sp$^n(\boldsymbol{a})$.

Cho $\boldsymbol{w}= (w_1, . . . , w_n)\in \mathbf{C}^n-$ Sp$^n(\boldsymbol{a})$. Theo định nghĩa của phổ đồng thời, tồn tại $b_1, . . . , b_n$ trong A sao cho

$$
(w_1-a_1)b_1+\cdots + (w_n-a_n)b_n= 1
$$

(I, p. 41, n$^o6$). Tồn tại một lân cận mở $W_{\boldsymbol{w}}$ của $\boldsymbol{w}$ sao cho phần tử $(z_1-a_1)b_1+\cdots + (z_n-a_n)b_n$ của A là khả nghịch nếu $\boldsymbol{z}= (z_1, . . . , z_n)$ thuộc $W_{\boldsymbol{w}}$. Với mọi số nguyên $j$ sao cho $1\leqslant j\leqslant n$ và mọi $\boldsymbol{z}$ trong $W_{\boldsymbol{w}}$, đặt

$$
u_j(\boldsymbol{z}) =b_j(\sum_{i=1}^n(z_i-a_i)b_i)^{-1}
$$

Các hàm $u_1, u_2, . . . , u_n$ từ $W_{\boldsymbol{w}}$ vào A được xác định như vậy là khả vi vô hạn trên $W_{\boldsymbol{w}}$, và ta có

$$
(z_1-a_1)u_1(\boldsymbol{z}) +\cdots + (z_n-a_n)u_n(\boldsymbol{z}) = 1
$$

với mọi $\boldsymbol{z}$ trong $W_{\boldsymbol{w}}$.

Vì họ $(W_{\boldsymbol{w}})_{\boldsymbol{w}\in\mathbf{C}^{n-}Sp^n(\boldsymbol{a})}$ là một phủ mở của $\mathbf{C}^n-$ Sp$^n(\boldsymbol{a})$, tồn tại một phủ mở hữu hạn địa phương $\mathscr{W}= (W_{\lambda})_{\lambda\in L}$ (TG, I, p. 70, đl. 5) và, với mọi $\lambda \in L$, các hàm $u_{1\lambda}, . . . , u_{n\lambda}$, nhận giá trị trong A, được xác định và khả vi vô hạn trên $W_{\lambda}$, sao cho $(z_1-a_1)u_{1\lambda}(\boldsymbol{z}) +\cdots + (z_n-a_n)u_{n\lambda}(\boldsymbol{z}) = 1$ với mọi $\boldsymbol{z}$ trong $W_{\lambda}$. Gọi $(f_{\lambda})_{\lambda\in L}$ là một phân hoạch đơn vị thích nghi với phủ $\mathscr{W}$, tạo thành bởi các hàm khả vi vô hạn (VAR, R1, p. 40, 5.3.6). Gọi $i$ là một số nguyên sao cho $1\leqslant i\leqslant n$. Với mọi $\lambda \in L$, gọi $u'_{i\lambda}$ là ánh xạ từ $\mathbf{C}^n-$ Sp$^n(\boldsymbol{a})$ vào A thu được bằng cách mở rộng bởi 0 hàm $f_{\lambda}u_{i\lambda}$ trên $(\mathbf{C}^n-$ Sp$^n(\boldsymbol{a}))-W_{\lambda}$. Các hàm $u'_{i\lambda}$ là khả vi vô hạn. Vì họ (Supp($u'_{i\lambda}$))$_{\lambda\in L}$ là hữu hạn địa phương, hàm $v_i=\sum_{\lambda\in L}u'_{i\lambda}$ được xác định và khả vi vô hạn trên

$\mathbf{C}^n-$ Sp$^n(\boldsymbol{a})$.

Cho $\boldsymbol{z}\in \mathbf{C}^n-$ Sp$^n(\boldsymbol{a})$. Ký hiệu bởi $L'$ tập hữu hạn các $\lambda \in L$ sao cho $\boldsymbol{z}\in W_{\lambda}$. Khi đó

$$
\sum_{i=1}^n(z_i-a_i)v_i(\boldsymbol{z}) =\sum_{\lambda\in L'}\sum_{i=1}^n(z_i-a_i)u'_{i\lambda}(\boldsymbol{z})
$$

$$
=\sum_{\lambda\in L'}f_{\lambda}(\boldsymbol{z})\sum_{i=1}^n(z_i-a_i)u_{i\lambda}(\boldsymbol{z}) =(\sum_{\lambda\in L'}f_{\lambda}(\boldsymbol{z}))\cdot 1 = 1
$$

#### Bổ đề 3 {#ts-i-s4-lem-3 .statement tag=02A0}

Cho $\boldsymbol{a}= (a_1, . . . , a_n)\in A^n$. Cho $h$ là một ánh xạ từ $\mathbf{C}^n$ vào $\mathbf{C}$, khả vi vô hạn, bằng 1 trên một lân cận của Sp$^n(\boldsymbol{a})$ và có giá compact. Tồn tại các ánh xạ khả vi vô hạn $u_1, . . . , u_n$ từ $\mathbf{C}^n$ vào A sao cho dãy $(h, u_1, . . . , u_n)$ thích nghi với $\boldsymbol{a}$.

Cho $v_1, . . . ,v_n$ là các ánh xạ khả vi vô hạn từ $\mathbf{C}^n-$ Sp$^n(\boldsymbol{a})$ vào A, sao cho

$$
\sum_{j=1}^n(z_j-a_j)v_j(\boldsymbol{z}) = 1
$$

với $\boldsymbol{z}$ thuộc $\mathbf{C}^n-$ Sp$^n(\boldsymbol{a})$ (bổ đề 2). Cho $i$ là một số nguyên sao cho $1\leqslant i\leqslant n$. Đặt $u_i(\boldsymbol{z}) = (1-h(\boldsymbol{z}))v_i(\boldsymbol{z})$ nếu $\boldsymbol{z}\in \mathbf{C}^n-$ Sp$^n(\boldsymbol{a})$ và $u_i(\boldsymbol{z}) = 0$ nếu $\boldsymbol{z}\in$ Sp$^n(\boldsymbol{a})$. Các ánh xạ $u_i$ là khả vi vô hạn trên $\mathbf{C}^n-$ Sp$^n(\boldsymbol{a})$ và triệt tiêu trên một lân cận của Sp$^n(\boldsymbol{a})$, do đó là khả vi vô hạn trên $\mathbf{C}^n$. Đẳng thức (1) đúng trên Sp$^n(\boldsymbol{a})$ vì các hàm số $u_i$ triệt tiêu trên Sp$^n(\boldsymbol{a})$ và $h$ bằng 1 trên một lân cận của Sp$^n(\boldsymbol{a})$. Nó cũng đúng trên $\mathbf{C}^n-$ Sp$^n(\boldsymbol{a})$ theo phép dựng.

#### Bổ đề 4 {#ts-i-s4-lem-4 .statement tag=02A1}

Cho $\boldsymbol{a}\in A^n$. Cho $(h, u_1, . . . , u_n)$ là một dãy thích nghi với $\boldsymbol{a}$ và $\omega$ là dạng vi phân liên kết.

a) Với $i= 1,2, . . . , n$, tồn tại một dạng vi phân $\beta_i$ trên $\mathbf{C}^n$, bậc $n-1$, với hệ số trong A, sao cho

$(z_i-a_i)\omega =d(h\beta_i\wedge dz_1\wedge  \cdots  \wedge dz_n)$ ;

b) Dạng vi phân $\omega$ có giá compact được chứa trong giá của $h$;

c) Tồn tại một dạng vi phân $\beta$ trên $\mathbf{C}^n$, bậc $n-1$, với hệ số trong A, sao cho

$$
(n+ 1)h\omega -\omega =d(h\beta \wedge dz_1\wedge  \cdots  \wedge dz_n)
$$

Cho $i$ là một số nguyên sao cho $1\leqslant i\leqslant n$. Tồn tại $\varepsilon_i\in  \{-1,1\}$ sao cho

$$
\varepsilon_i\bigwedge_{j\not=i}du_j\wedge dz_1\wedge  \cdots  \wedge dz_n=dz_i\wedge \bigwedge_{j\not=i}(du_j\wedge dz_j)
$$

Đặt $\beta_i=\varepsilon_i\bigwedge_{j\not=i}du_j$, để số hạng ở vế trái của công thức này là $\beta_i\wedge dz_1\wedge  \cdots  \wedge dz_n$ và $d\beta_i= 0$. Do đó

$$
d(h\beta_i\wedge dz_1\wedge  \cdots  \wedge dz_n)=dh\wedge \beta_i\wedge dz_1\wedge  \cdots  \wedge dz_n=
$$

$$
dh\wedge dz_i\wedge \bigwedge_{j\not=i}(du_j\wedge dz_j) = (z_i-a_i)\omega
$$

theo công thức (3), do đó suy ra mệnh đề a).

Từ mệnh đề a) và công thức (1) suy ra quan hệ

$$
\omega =h\omega + (1-h)\omega =h\omega +\sum_{i=1}^n(z_i-a_i)u_i\omega
$$

$$
=h\omega +\sum_{i=1}^nu_id(h\beta_i\wedge dz_1\wedge  \cdots  \wedge dz_n)
$$

do đó Supp($\omega$ )$\subset$ Supp($h$), điều này chứng minh b).

Cuối cùng, đặt

$\beta =\sum_{i=1}^n\varepsilon_iu_i\bigwedge_{j\not=i}du_j=\sum_{i=1}^nu_i\beta_i$, và $\tau =h\beta dz_1\wedge  \cdots  \wedge dz_n$.

Ta có $d\beta =\sum_idu_i\wedge \beta_i$ và vì vậy

$$
d\beta \wedge dz_1\wedge  \cdots  \wedge dz_n=\sum_idu_i\wedge dz_i\wedge \bigwedge_{j\not=i}(du_j\wedge dz_j) =n\omega
$$

Do đó

$$
d\tau =dh\wedge \beta \wedge dz_1\wedge  \cdots  \wedge dz_n+hd\beta \wedge dz_1\wedge  \cdots  \wedge dz_n
$$

$$
=\sum_{i=1}^nu_idh\wedge dz_i\wedge \bigwedge_{j\not=i}(du_j\wedge dz_j) +nh\omega
$$

$$
=-\sum_{i=1}^nu_i(z_i-a_i)\omega +nh\omega = (h-1)\omega +nh\omega = (n+ 1)h\omega -\omega
$$

có tính đến các công thức (3) và (1), do đó c).

Bây giờ chúng ta đề nghị nghiên cứu cách dạng vi phân $\omega$ liên kết với một dãy thích nghi với $\boldsymbol{a}$ biến thiên như một hàm của dãy này. Ta sẽ nói rằng các dãy $(h, u_1, . . . , u_n)$ và $(h', u'_1, . . . , u'_n)$ thích nghi với $\boldsymbol{a}$ là liên kết nếu tồn tại một dạng vi phân $\psi$ bậc $n-1$ trên $\mathbf{C}^n$, với hệ số trong A và với giá được chứa trong hợp của các giá của $h$ và của $h'$, sao cho các dạng vi phân liên kết $\omega$ và $\omega '$ thỏa mãn

$$
\omega -\omega '=d(\psi \wedge dz_1\wedge dz_2\wedge  \cdots  \wedge dz_n)
$$

Hãy bắt đầu bằng một phép biến đổi sơ cấp:

#### Bổ đề 5 {#ts-i-s4-lem-5 .statement tag=02A2}

Cho $\boldsymbol{a}\in A^n$, cho $(h, u_1, . . . , u_n)$ là một dãy thích nghi với $\boldsymbol{a}$, và cho $\omega$ là dạng vi phân liên kết.

Cho $w$ là một ánh xạ khả vi vô hạn từ $\mathbf{C}^n$ vào A, và cho $i$ và $j$ là hai số nguyên phân biệt giữa 1 và $n$. Định nghĩa $u'_1, . . . , u'_n$ bởi

$$
u'_i=u_i+ (z_j-a_j)w,u'_j=u_j-(z_i-a_i)w
$$

$u'_k=u_k$ với $k\not=i, j$.

Khi đó dãy $(h, u'_1, . . . , u'_n)$ thích nghi với $\boldsymbol{a}$ và liên kết với dãy $(h, u_1, . . . , u_n)$.

Hãy viết $d\boldsymbol{z}=dz_1\wedge  \cdots  \wedge dz_n$. Vì

$$
\sum_{k=1}^n(z_k-a_k)u'_k(\boldsymbol{z}) =\sum_{k=1}^n(z_k-a_k)u_k(\boldsymbol{z}) +w(\boldsymbol{z})(z_j-a_j)(z_i-a_i)
$$

$$
-w(\boldsymbol{z})(z_i-a_i)(z_j-a_j) = 1-h(\boldsymbol{z})
$$

với mọi $z\in \mathbf{C}^n$, dãy $(h, u'_1, . . . , u'_n)$ thích nghi với $\boldsymbol{a}$. Hơn nữa, ta có

$$
du'_i\wedge du'_j\wedge dz_1\wedge  \cdots  \wedge dz_n=
$$

$$
(du_i+w dz_j+ (z_j-a_j)dw)\wedge (du_j-w dz_i-(z_i-a_i)dw)\wedge d\boldsymbol{z}
$$

$$
=(du_i\wedge du_j-(z_i-a_i)du_i\wedge dw-(z_j-a_j)du_j\wedge dw)\wedge d\boldsymbol{z}
$$

Do đó tồn tại $\varepsilon \in  \{-1,1\}$ sao cho $\varepsilon (\omega -\omega ')$ bằng

$$
du'_i\wedge du'_j\wedge \bigwedge_{k\not=i,j}du'_k\wedge d\boldsymbol{z}-du_i\wedge du_j\wedge \bigwedge_{k\not=i,j}du_k\wedge d\boldsymbol{z}
$$

$$
=-((z_i-a_i)du_i\wedge dw+ (z_j-a_j)du_j\wedge dw)\wedge \bigwedge_{k\not=i,j}du_k\wedge d\boldsymbol{z}
$$

$$
=-(\sum_{k=1}^n(z_k-a_k)du_k)\wedge dw\wedge \bigwedge_{k\not=i,j}du_k\wedge d\boldsymbol{z}
$$

và, có tính đến (2), biểu thức này bằng

$$
dh\wedge dw\wedge \bigwedge_{k\not=i,j}du_k\wedge d\boldsymbol{z}=d(h dw\wedge \bigwedge_{k\not=i,j}du_k\wedge d\boldsymbol{z})
$$

do đó có kết quả.

#### Bổ đề 6 {#ts-i-s4-lem-6 .statement tag=02A3}

Cho $\boldsymbol{a}\in A^n$. Mọi dãy thích nghi với $\boldsymbol{a}$ đều liên kết.

Cho $(h, u_1, . . . , u_n)$ và $(h', u'_1, . . . , u'_n)$ là các dãy thích nghi với $\boldsymbol{a}$, và ký hiệu bởi $\omega$ và $\omega '$ các dạng vi phân liên kết.

Định nghĩa các ánh xạ khả vi vô hạn

$$
w_{ij}=u'_iu_j-u_iu'_j,1\leqslant i\leqslant n,1\leqslant j\leqslant n
$$

$$
s_i=u'_ih-u_ih',1\leqslant i\leqslant n
$$

sao cho $w_{ji}=-w_{ij}$, và Supp($s_i$)$\subset$ Supp($h$)$\cup$ Supp($h'$).

Đặt $u''_i=u'_i-s_i,\boldsymbol{u}= (u_1, . . . , u_n)$ và $\boldsymbol{u}''= (u''_1, . . . , u''_n)$. Ta cũng ký hiệu bởi $\boldsymbol{v}_{ij}$ ánh xạ từ $\mathbf{C}^n$ vào $A^n$ mà thành phần thứ $i$ là $(z_j-a_j)w_{ij}$, thành phần thứ $j$ là $(z_i-a_i)w_{ji}=-(z_i-a_i)w_{ij}$, và các thành phần khác bằng không. Khi đó ta có

$$
\boldsymbol{u}''=\boldsymbol{u}+\sum_{i<j}\boldsymbol{v}_{ij}
$$

Thật vậy, với mọi số nguyên $k$ sao cho $1\leqslant k\leqslant n$, thành phần thứ $k$ của vế phải là

$$
u_k+\sum^{k-1}_{i=1}(z_i-a_i)w_{ki}+\sum_{j=k+1}^n(z_j-a_j)w_{kj}=u_k+\sum_{i=1}^n(z_i-a_i)w_{ki}
$$

$$
=u_k+u'_k\sum_{i=1}^n(z_i-a_i)u_i-u_k\sum_{i=1}^n(z_i-a_i)u'_i
$$

$$
=u_k+ (1-h)u'_k-(1-h')u_k=u'_k-s_k
$$

Bằng quy nạp, ta suy ra từ Bổ đề 5, áp dụng cho các số nguyên $i$ và $j$ và cho các ánh xạ $w_{ij}$, rằng dãy $(h, u''_1, . . . , u''_n)$ thích nghi với $\boldsymbol{a}$ và liên kết với $(h, u_1, . . . , u_n)$. Gọi $\omega ''$ là dạng vi phân liên kết với $(h, u''_1, . . . , u''_n)$. Vì $u''_i=u'_i-s_i$, ta có

$$
\omega ''-\omega '=d(u'_1-s_1)\wedge dz_1\wedge  \cdots  \wedge d(u'_n-s_n)\wedge dz_n-
$$

$$
du'_1\wedge dz_1\wedge  \cdots  \wedge du'_n\wedge dz_n
$$

biểu thức này được viết thành một tổ hợp tuyến tính, với các hệ số 1 hoặc $-1$, của các dạng vi phân có dạng

$$
\xi_{I_1,I_2}=\bigwedge_{i\in I_1}ds_i\wedge \bigwedge_{i\in I_2}du'_i\wedge dz_1\wedge  \cdots  \wedge dz_n
$$

trong đó $I_1$ (resp. $I_2$) là một tập con khác rỗng (resp. một tập con) của $\{1, . . . , n\}$. Mỗi dạng vi phân $\xi_{I_1,I_2}$ cũng có thể được viết dưới dạng

$$
d(\widetilde{\psi}\wedge dz_1\wedge  \cdots  \wedge dz_n)
$$

trong đó giá của dạng vi phân $\widetilde{\psi}$ được chứa trong giá của $s_i$ với mọi $i\in I_1$. Vì $I_1$ khác rỗng, giá này được chứa trong Supp($h$)$\cup$ Supp($h'$). Do đó, $(h, u''_1, . . . , u''_n)$ liên kết với $(h', u'_1, . . . , u'_n)$, và bổ đề thu được bằng cách viết

$$
\omega -\omega '= (\omega -\omega '') + (\omega ''-\omega ')
$$

### 4. Phép dựng các ánh xạ $\Theta_{\boldsymbol{a}}$

Cho $\boldsymbol{a}= (a_1, . . . , a_n)\in A^n$ và cho U là một lân cận mở của Sp$^n(\boldsymbol{a})$. Cho $h$ là một ánh xạ khả vi vô hạn lần, bằng 1 trong một lân cận của Sp$^n(\boldsymbol{a})$ và sao cho giá của $h$ là compact và được chứa trong U (Bổ đề 1 của I, p. 52). Theo Bổ đề 3 của I, p. 54, tồn tại các ánh xạ khả vi vô hạn lần $(u_1, . . . , u_n)$ từ $\mathbf{C}^n$ vào A sao cho dãy $(h, u_1, . . . , u_n)$ thích nghi với $\boldsymbol{a}$. Gọi $\omega$ là dạng vi phân liên kết với nó; nó có giá compact được chứa trong U (Bổ đề 4 của I, p. 54). Tồn tại một hàm khả vi vô hạn lần $\psi$ có giá compact trong U và nhận giá trị trong A sao cho

$$
\omega =\psi  dx_1\wedge dy_1\wedge  \cdots  \wedge dx_n\wedge dy_n
$$

trong đó $x_j+iy_j$ là các hàm tọa độ trên $\mathbf{C}^n$, được đồng nhất với $\mathbf{R}^{2n}$. Gọi $\mu$ là độ đo Lebesgue trên $\mathbf{R}^{2n}$.

Cho $f\in \mathscr{C}(U; A)$. Dạng vi phân $f \omega |U$ trên U là liên tục và có giá compact. Độ đo vectơ liên kết với dạng vi phân này (VAR, R2, 10.4.3 and 10.4.4) là độ đo vectơ $f \psi \cdot \mu$; đó là một độ đo có cơ sở $\mu$ (INT, VI, §2, n$^o4$, Định nghĩa 4), giá của nó là compact và được chứa trong giá của $\omega$. Độ đo này bị chặn trên theo chuẩn của A (INT, VI, §2, n$^o4$, Mệnh đề 8); ta ký hiệu bởi $\|f \omega \|$ độ đo dương trên $\mathbf{C}^n$ liên kết với nó (INT, VI, §2, n$^o3$, Định nghĩa 3).

Theo INT, VI, §2, n$^o4$, Mệnh đề 8, b), ta có

$$
\|f \omega \|=\|f \psi \cdot \mu\|=\|f \psi \| \cdot \mu=\|f\| \|\omega \|
$$

Đặc biệt, tích phân của dạng vi phân $f \omega$ trên U thỏa mãn

$$
\|\int_Uf \omega \|\leqslant \int_U\|f\| \|\omega \|
$$

(INT, VI, §2, n$^o3$, Mệnh đề 5).

#### Bổ đề 7 {#ts-i-s4-lem-7 .statement tag=02A4}

Với mọi hàm $f\in \mathscr{O}(U; A)$, tích phân $\int_Uf \omega$ là một phần tử của A chỉ phụ thuộc vào $\boldsymbol{a}$ và vào mầm của $f$ trong một lân cận của Sp$^n(\boldsymbol{a})$. Nó thỏa mãn bất đẳng thức

(4) $\|\int f \omega \|\leqslant (\int\|\omega \|)$ sup $\|f(z)\|$,

U U $z\in$Supp($h$)

và

$$
\int_U(af)\omega =a\int_Uf \omega
$$

với mọi $a\in A$.

Ta đã thấy ở trên rằng tích phân được xác định với $f\in \mathscr{C}(U; A)$ và thỏa mãn

$\|\int f \omega \|\leqslant \int\|f\| \|\omega \|\leqslant (\int\|\omega \|)$ sup $\|f(z)\|$.

U U U $z\in$Supp($h$)

Hơn nữa, với mọi $a\in A$ và mọi $f\in \mathscr{C}(U; A)$, ta có

$$
\int_U(af)\omega =a\int_Uf \omega
$$

(INT, VI, §2, n$^o2$, Mệnh đề 2 áp dụng cho phép nhân bởi $a$).

Cho $(h', u'_1, . . . , u'_n)$ là một dãy thích nghi với $\boldsymbol{a}$ sao cho Supp($h'$)$\subset U$. Gọi $\omega '$ là dạng vi phân liên kết. Theo Bổ đề 6 của I, p. 57, tồn tại một dạng vi phân $\psi$ trên $\mathbf{C}^n$ bậc $n-1$, với các hệ số trong A và có giá được chứa trong Supp($h$)$\cup$ Supp($h'$)$\subset U$, sao cho

$$
\omega -\omega '=d(\psi \wedge dz_1\wedge  \cdots  \wedge dz_n)
$$

Cho $f\in \mathscr{O}(U; A)$. Vì ánh xạ $f$ là chỉnh hình, ta có

$$
df=\sum^n\frac{\partial f}{\partial z_i}dz_i
$$

$i=1$

(VAR, R2, p. 24, 8.8.9) và do đó

$$
f(\omega -\omega ') =f d(\psi \wedge dz_1\wedge  \cdots  \wedge dz_n) =d(f \psi \wedge dz_1\wedge  \cdots  \wedge dz_n)
$$

Theo công thức Stokes (VAR, R2, p. 48, 11.2.3), khi đó ta có

$$
\int_Uf(\omega -\omega ') = 0
$$

Do đó phần tử $\int_Uf \omega$ không phụ thuộc vào lựa chọn của dãy $(h, u_1, . . . , u_n)$.

Để kết luận, hãy chứng minh rằng $\int_Uf \omega$ chỉ phụ thuộc vào mầm của $f$ trong một lân cận của Sp$^n(\boldsymbol{a})$. Cho U và $U'$ là các lân cận mở của Sp$^n(\boldsymbol{a})$. Cho $f\in \mathscr{O}(U; A)$ và $f'\in \mathscr{O}(U'; A)$ sao cho $f$ và $f'$ trùng nhau trên một lân cận mở $U''$ của Sp$^n(\boldsymbol{a})$. Tồn tại một ánh xạ $h$ của $\mathbf{C}^n$ vào $\mathbf{C}$, khả vi vô hạn lần, bằng 1 trong một lân cận của Sp$^n(\boldsymbol{a})$, và có giá compact được chứa trong $U''$ (Bổ đề 1 của I, p. 52), và tồn tại $(u_1, . . . , u_n)$ sao cho dãy $(h, u_1, . . . , u_n)$ thích nghi với $\boldsymbol{a}$ (Bổ đề 3 của I, p. 54). Gọi $\omega$ là dạng vi phân liên kết. Vì Supp($\omega$ )$\subset$ Supp($h$)$\subset U''$ (Bổ đề 4, b) của I, p. 54), ta có

$$
\int_Uf \omega =\int_{U''}f \omega =\int_{U''}f'\omega =\int_{U'}f'\omega
$$

điều này hoàn thành chứng minh.

Bổ đề này chứng minh rằng tồn tại một ánh xạ A-tuyến tính duy nhất $\Theta_{\boldsymbol{a}}$ của $\mathscr{O}$(Sp$^n(\boldsymbol{a}); A$) vào A sao cho

(5) $\Theta_{\boldsymbol{a}}(f) =n$! $_n\int\widetilde{f \omega}$

$$
(2i\pi )_U
$$

với mọi tập mở U và mọi đại diện $\widetilde{f}\in \mathscr{O}(U; A)$ của một mầm $f\in \mathscr{O}$(Sp$^n(\boldsymbol{a}); A$). Ánh xạ tuyến tính $\Theta_{\boldsymbol{a}}$ là liên tục theo bất đẳng thức (4) và EVT, II, p. 29, Mệnh đề 5.

### 5. Các tính chất của các ánh xạ $\Theta_{\boldsymbol{a}}$

Chúng tôi nhắc lại (VAR, R2, p. 46 và p. 47, 11.1.3, d)) rằng nếu K là một tập con compact của $\mathbf{C}$, thì tồn tại một hệ cơ bản các lân cận compact V của K là những mảnh của $\mathbf{C}$ (nghĩa là, với mọi $x\in V$, tồn tại một bản đồ địa phương $(U, \varphi ,\mathbf{C})$ của $\mathbf{C}$ tại $x$ sao cho $\varphi (U\cap K)$ là một tập con mở của một nửa-không gian đóng của $\mathbf{C}$). Khi đó, ta ký hiệu bởi $\partial V$ biên của mảnh V được trang bị định hướng suy ra từ định hướng của $\mathbf{C}$ (VAR, R2, p. 47) và bởi $dz$ vi phân của đơn ánh $\partial V\rightarrow \mathbf{C}$.

#### Mệnh đề 1 {#ts-i-s4-prop-1 .statement tag=02A5}

Cho $a$ là một phần tử của A, cho U là một lân cận mở của Sp($a$), và cho $f\in \mathscr{O}(U; A)$. Cho V là một lân cận compact của Sp($a$) được chứa trong U và sao cho V là một mảnh của $\mathbf{C}$.

Khi đó $z\mapsto f(z)(z-a)^{-1}$ là liên tục trên $\partial V$, dạng vi phân $f(z)(z-a)^{-1}dz$ khả tích trên $\partial V$, và ta có

$$
\Theta_a(f) =\frac{1}{2i\pi}\int_{\partial V}f(z)(z-a)^{-1}dz
$$

Cho $h$ là một ánh xạ từ $\mathbf{C}$ vào $\mathbf{C}$, khả vi vô hạn, bằng 1 trong một lân cận của Sp($a$) và có giá compact được chứa trong phần trong của V (bổ đề 1 của I, p. 52). Cho $u$ là một ánh xạ từ $\mathbf{C}$ vào A sao cho $(h, u)$ thích nghi với $a($xem ví dụ 3 của I, p. 53). Dạng vi phân liên kết là $\omega =du\wedge dz$. Ta được $f \omega =f du\wedge dz=d(f u dz)$ vì $f$ là chỉnh hình. Hơn nữa, $u(z) = (z-a)^{-1}$ trên biên của V. Mặt khác, dạng vi phân $f u dz$ thuộc lớp $C^1$ trên U. Do đó

$$
2i\pi \Theta_a(f) =\int_Vd(f u dz) =\int_{\partial V}f u dz=\int_{\partial V}f(z)(z-a)^{-1}dz
$$

theo công thức (5) và công thức Stokes đối với mảnh V (VAR, R2, p. 47, 11.2.3).

#### Hệ quả {#ts-i-s4-n5-cor-1 .statement tag=02A6}

Cho $a\in A$. Ta có $\Theta_a(1) = 1$.

Cho $R> \varrho (a)$ là một số thực. Cho V là đĩa đóng tâm 0 bán kính R, sao cho Sp($a$)$\subset \mathring{V}$. Nó là một mảnh của $\mathbf{C}$ mà biên $\partial V$ là đường tròn tâm 0 bán kính R. Với $z\in \mathbf{C}-\mathring{V}$, ta có công thức $(z-a)^{-1}=z^{-1}(1-z^{-1}a)^{-1}=\sum^{+\infty}_{j=1}z^{-j}a^{j-1}$. Chuỗi hội tụ đều với $z\in \partial V$. Do đó

$$
\Theta_a(1) =\frac{1}{2i\pi}\sum^{+\infty}_{j=1}a^{j-1}\int_{\partial V}z^{-j}dz= 1
$$

vì

$$
\int_{\partial V}z^jdz= 0
$$

với mọi số nguyên $j\not=-1$ và

$$
\int_{\partial V}z^{-1}dz= 2i\pi
$$

(VAR, R2, p. 44, 10.4.5, và p. 47, 11.2.1, ví dụ).

#### Bổ đề 8 {#ts-i-s4-lem-8 .statement tag=02A7}

Cho U là một tập mở của $\mathbf{C}^n$. Cho $\omega_1$ là một dạng vi phân liên tục bậc $n$ trên U, có giá compact và nhận giá trị trong A (tương ứng, $\omega_2$ là một dạng vi phân liên tục bậc 2 trên $\mathbf{C}$, có giá compact và nhận giá trị trong $\mathbf{C}$). Ký hiệu $\pi_1$ và $\pi_2$ là các phép chiếu chính tắc của $U\times \mathbf{C}$ lên U và $\mathbf{C}$. Dạng vi phân $\pi_1^*\omega_1\wedge \pi_2^*\omega_2$ trên $U\times \mathbf{C}$ là liên tục, có giá compact và nhận giá trị trong A. Ta có

$$
\int_{U\times\mathbf{C}}\pi_1^*\omega_1\wedge \pi^*_2\omega_2=(\int_{\mathbf{C}}\omega_2)((\int_U\omega_1)
$$

Cho $\mu_n$ là độ đo Lebesgue trên $\mathbf{C}^n$ và $\mu_1$ là độ đo Lebesgue trên $\mathbf{C}$. Tồn tại $\psi_1\in \mathscr{K}(U; A)$ và $\psi_2\in \mathscr{K}(\mathbf{C})$ sao cho độ đo vectơ liên kết với $\omega_1$ bằng $\psi_1\cdot \mu_n$, và độ đo vectơ liên kết với $\omega_2$ bằng $\psi_2\cdot \mu_1$. Độ đo vectơ liên kết với dạng vi phân $\pi^*_1\omega_1\wedge \pi_2^*\omega_2$ là $(\psi_1\otimes \psi_2)\cdot \mu_n\otimes \mu_1$.

Cho $\ell$ là một dạng tuyến tính liên tục trên A. Theo INT, VI, §2, n$^o2$, định nghĩa 2 và định nghĩa của độ đo tích (INT, III, §4, n$^o1$, định nghĩa 1), suy ra rằng

$$
\ell (\int_{U\times\mathbf{C}}\pi_1^*\omega_1\wedge \pi^*_2\omega_2)=\int_{U\times\mathbf{C}}\ell \circ (\psi_1\otimes \psi_2)\mu_n\otimes \mu_1
$$

$$
=\int\psi_2(z)\ell (\psi_1(x))d\mu_n(x)d\mu_1(z)
$$

$$
=(\int^{U\times\mathbf{C}}_{\mathbf{C}}\psi_2(z)d\mu_1(z))(\int_U\ell (\psi_1(x))d\mu_n(x))
$$

$$
=(\int_{\mathbf{C}}\psi_2\mu_1)\ell (\int_U\psi_1\mu_n)
$$

do đó có kết quả (INT VI, loc. cit.).

#### Bổ đề 9 {#ts-i-s4-lem-9 .statement tag=02A8}

Cho $\boldsymbol{a}= (a_1, . . . , a_n)\in A^n$. Cho $p\in \mathbf{N}$ và $\boldsymbol{a}'$ = $(a_{n+1}, . . . , a_{n+p})\in A^p$. Khi đó ta có $\Theta_{(\boldsymbol{a},\boldsymbol{a}')}\circ \pi_{n,n+p}^*= \Theta_{\boldsymbol{a}}$. Đặc biệt, ta có $\Theta_{\boldsymbol{a}}(1) = 1$.

Vì ta có $\pi_{n,n+p}=\pi_{n,n+1}\circ \cdots \circ \pi_{n+p-1,n+p}$, nên chỉ cần chứng minh mệnh đề thứ nhất khi $p= 1$, điều mà từ đây về sau ta giả sử. Ta viết đơn giản $\pi =\pi_{n,n+1}$. Khi đó chỉ cần chứng minh rằng, với mọi lân cận mở U của Sp$^n(\boldsymbol{a})$, và mọi hàm $f\in \mathscr{O}(U; A)$, ta có $\Theta_{(\boldsymbol{a},a_{n+1})}(f\circ \pi ) = \Theta_{\boldsymbol{a}}(f)$. Đặt $g=f\circ \pi$. Gọi $h$ (tương ứng $h'$) là một ánh xạ từ $\mathbf{C}^n$ vào $\mathbf{C}$ (tương ứng từ $\mathbf{C}$ vào $\mathbf{C}$), khả vi vô hạn lần, bằng 1 trong một lân cận của Sp$^n(\boldsymbol{a})$ (tương ứng của Sp($\boldsymbol{a}'$)), có hỗ compact được chứa trong U (tương ứng trong $\mathbf{C}$). Tồn tại các ánh xạ $(u_1, . . . , u_n)$ từ $\mathbf{C}^n$ vào A, khả vi vô hạn lần, sao cho dãy $(h, u_1, . . . , u_n)$ thích nghi với $\boldsymbol{a}$ (bổ đề 3 của I, p. 54), và một ánh xạ $u_{n+1}$ khả vi vô hạn lần từ $\mathbf{C}$ vào A sao cho cặp $(h', u_{n+1})$ thích nghi với $a_{n+1}($loc. cit.)

Với $\boldsymbol{z}\in \mathbf{C}^n$ và $z_{n+1}\in \mathbf{C}$, viết $h''(\boldsymbol{z}, z_{n+1}) =h(\boldsymbol{z})h'(z_{n+1})$ và $u''_{n+1}(\boldsymbol{z}, z_{n+1}) =h(\boldsymbol{z})u_{n+1}(z_{n+1})$. Các hàm $h''$ và $u''_{n+1}$ khả vi vô hạn lần trên $\mathbf{C}^{n+1}$. Hàm $h''$ bằng 1 trong một lân cận của Sp$^{n+1}(\boldsymbol{a}, a_{n+1})$, và có hỗ compact được chứa trong $U\times \mathbf{C}$. Với mọi $\boldsymbol{w}= (\boldsymbol{z}, z_{n+1})\in \mathbf{C}^{n+1}$, ta có

$$
(z_1-a_1)(u_1\circ \pi )(\boldsymbol{w}) +\cdots + (z_n-a_n)(u_n\circ \pi )(\boldsymbol{w})
$$

$$
+ (z_{n+1}-a_{n+1})u''_{n+1}(\boldsymbol{w}) = 1-h(\boldsymbol{z}) +h(\boldsymbol{z})(1-h'(z_{n+1}))
$$

$$
= 1-h''(\boldsymbol{w})
$$

điều này chứng minh rằng dãy $(h'', u_1\circ \pi , . . . , u_n\circ \pi , u''_{n+1})$ thích nghi với $(\boldsymbol{a}, a_{n+1})$. Gọi $\omega$ là dạng vi phân liên kết.

Dạng vi phân $du_1\wedge dz_1\wedge  \cdots  \wedge du_n\wedge dz_n\wedge dh$ trên $\mathbf{C}^n$ có bậc $2n+ 1$, do đó bằng không. Vì thế

$$
\omega =d(u_1\circ \pi )\wedge dz_1\wedge  \cdots  \wedge d(u_n\circ \pi )\wedge dz_n\wedge du''_{n+1}\wedge dz_{n+1}
$$

$$
= (h\circ \pi )d(u_1\circ \pi )\wedge dz_1\wedge  \cdots  \wedge d(u_n\circ \pi )\wedge dz_n\wedge du_{n+1}\wedge dz_{n+1}
$$

Vì $g=f\circ \pi$, công thức (5) và bổ đề 8 suy ra

$\Theta_{\boldsymbol{a},\boldsymbol{a}'}(g) =$ (2$(ni\pi +$ 1)!$)^{n+1}\int_{U\times\mathbf{C}}g\omega =$ (2$(ni\pi +$ 1)!$)^{n+1}(\int_{\mathbf{C}}du_{n+1}\wedge dz_{n+1})$

$$
\times (\int_Uf h du_1\wedge dz_1\wedge  \cdots  \wedge du_n\wedge dz_n)
$$

Một mặt, ta có

$$
\int_{\mathbf{C}}du_{n+1}\wedge dz_{n+1}= 2i\pi \Theta^{\mathbf{C}}_{a_{n+1}}(1) = 2i\pi \cdot 1
$$

theo hệ quả 5. Mặt khác, phần c) của bổ đề 4 trong I, p. 54 và sự kiện rằng tích phân của một dạng đóng bằng không (VAR, R2, p. 48, 11.2.4) suy ra

$$
(n+ 1)\int_Uf hdu_1\wedge dz_1\wedge  \cdots  \wedge du_n\wedge dz_n=
$$

$\int_Uf du_1\wedge dz_1\wedge  \cdots  \wedge du_n\wedge dz_n=(2i\pi n$!$)^n\Theta_{\boldsymbol{a}}(f)$.

Do đó ta thu được

$\Theta_{\boldsymbol{a},\boldsymbol{a}'}(g) =$ (2$(ni\pi +$ 1)!$)^{n+1}\times ((2ni\pi +$ 1)!$)^n\Theta_{\boldsymbol{a}}(f)\times 2i\pi = \Theta_{\boldsymbol{a}}(f)$.

Cuối cùng, công thức $\Theta_{\boldsymbol{a}}(1) = 1$ suy ra từ những điều trên và từ hệ quả của Mệnh đề 1.

#### Bổ đề 10 {#ts-i-s4-lem-10 .statement tag=02A9}

Cho $\boldsymbol{a}\in A^n$. Cho $g$ là một hàm đa thức trên $\mathbf{C}^n$ với hệ số trong A và cho $f\in \mathscr{O}$(Sp$^n(\boldsymbol{a}); A$). Khi đó $\Theta_{\boldsymbol{a}}(gf) =g(\boldsymbol{a})\Theta_{\boldsymbol{a}}(f)$. Đặc biệt, $\Theta_{\boldsymbol{a}}(g) =g(\boldsymbol{a})$.

Theo Bổ đề 9, chỉ cần chứng minh mệnh đề thứ nhất.

Ký hiệu bởi $z_1, . . . , z_n$ các hàm tọa độ trên $\mathbf{C}^n$. Vì ánh xạ $\Theta_{\boldsymbol{a}}$ là A-tuyến tính, chỉ cần chứng minh mệnh đề của bổ đề trong trường hợp $g=z_1^{e_1}\cdots z^{e_n}_n$, với $(e_1, . . . , e_n)\in \mathbf{N}^n$. Lập luận bằng quy nạp theo $e_1+\cdots +e_n$, ta quy được về trường hợp tồn tại một số nguyên $i$ sao cho $1\leqslant i\leqslant n$ và $g=z_i$.

Cho U là một lân cận mở của Sp$^n(\boldsymbol{a})$. Cho $(h, u_1, . . . , u_n)$ là một dãy thích nghi với $\boldsymbol{a}$ sao cho giá của $h$ được chứa trong U (Bổ đề 1 của I, p. 52 và Bổ đề 3 của I, p. 54), và cho $\omega$ là dạng vi phân liên kết. Theo Bổ đề 4, a) của I, p. 54, tồn tại một dạng vi phân $\beta$ sao cho

$$
(z_i-a_i)\omega =d(h\beta \wedge dz_1\wedge  \cdots  \wedge dz_n)
$$

Do đó, với mọi hàm $f\in \mathscr{O}(U; A)$, ta có

$$
(z_i-a_i)f \omega =f d(h\beta \wedge dz_1\wedge  \cdots  \wedge dz_n) =d(f h\beta \wedge dz_1\wedge  \cdots  \wedge dz_n)
$$

vì $f$ là hàm chỉnh hình, nên $df\wedge dz_1\wedge  \cdots  \wedge dz_n= 0$. Áp dụng công thức Stokes (VAR, R2, p. 48, 11.2.4), ta được $\int_U(z_i-a_i)f \omega = 0$, do đó

$\Theta_{\boldsymbol{a}}(z_if) =(2i\pi n$!$)^n\int_Uz_if \omega =(2ni\pi$!$)^n\int_Ua_if \omega =a_i\Theta_{\boldsymbol{a}}(f)$

theo công thức (5). Kết quả suy ra.

#### Mệnh đề 2 {#ts-i-s4-prop-2 .statement tag=02AA}

Cho $\varrho_1, . . . , \varrho_n$ là các số thực $>0$ và cho $U\subset \mathbf{C}^n$ là đa đĩa bằng tích của các đĩa mở tâm 0 và bán kính $\varrho_i$. Cho

$$
\sum c(k_1, . . . , k_n)X^{k_1}_1\cdots X^{k_n}_n\in A[[X_1, . . . ,X_n]]
$$

$(k_1,...,k_n)\in \mathbf{N}^n$

là một chuỗi hình thức với hệ số trong A. Giả sử chuỗi này hội tụ trong U, và ký hiệu bởi $f$ hàm chỉnh hình trong U mà nó là tổng.

Cho $\boldsymbol{a}= (a_1, . . . , a_n)\in A^n$ sao cho $\varrho (a_i)< \varrho_i$ với $1\leqslant i\leqslant n$. Khi đó Sp$^n(\boldsymbol{a})\subset U$, họ $(c(k_1, . . . , k_n)a^{k_1}_1\cdots a^{k_n}_n)$ các phần tử của A là tổng được tuyệt đối, và

$$
\Theta_{\boldsymbol{a}}(f) =\sum c(k_1, . . . , k_n)a^{k_1}_1\cdots a^{k_n}_n
$$

$(k_1,...,k_n)\in \mathbf{N}^n$

Với mọi đặc trưng $\chi$ của A và mọi số nguyên $i$ sao cho $1\leqslant i\leqslant n$, ta có $|\chi (a_i)|\leqslant \varrho (a_i)< \varrho_i$, do đó Sp$^n(\boldsymbol{a})\subset U$ theo định nghĩa của phổ đồng thời. Gọi $z_1, . . . , z_n$ là các hạn chế lên U của các hàm tọa độ trên $\mathbf{C}^n$. Khi đó họ $(c(k_1, . . . , k_n)z_1^{k_1}\cdots z^{k_n}_n)$ là khả tổng trong $\mathscr{O}(U; A)$ và có tổng là $f$. Theo bổ đề 10 và tính liên tục của ánh xạ $\Theta^U_{\boldsymbol{a}}$, suy ra họ $(c(k_1, . . . , k_n)a^{k_1}_1. . . a^{k_n}_n)$ là khả tổng trong A và có tổng là $\Theta_{\boldsymbol{a}}(f)$. Với $1\leqslant i\leqslant n$, gọi $\lambda_i$ là một số thực sao cho $\varrho (a_i)< \lambda_i< \varrho_i$. Tồn tại $M_i<+\infty$ sao cho $\|a^k_i\|\leqslant M_i\lambda^k_i$ với mọi số nguyên $k\geqslant 0$. Khi đó ta có

$$
\sum\|c(k_1, . . . , k_n)\| \|a^{k_1}_1\cdots a^{k_n}_n\|\leqslant
$$

$(k_1,...,k_n)\in \mathbf{N}^n$

$M_1\cdots M_n\sum\|c(k_1, . . . , k_n)\|\lambda^{k_1}_1\cdots \lambda^{k_n}_n$

$(k_1,...,k_n)\in \mathbf{N}^n$ là hữu hạn theo giả thiết, do đó họ $(c(k_1, . . . , k_n)a^{k_1}_1\cdots a^{k_n}_n)$ là khả tổng tuyệt đối.

#### Hệ quả {#ts-i-s4-n5-cor-2 .statement tag=02AB}

Giả sử rằng A khác không. Cho $\boldsymbol{a}\in \mathbf{C}^n\subset A^n$. Ta có Sp$^n_A(\boldsymbol{a}) =\{\boldsymbol{a}\}$. Với mọi mầm $f\in \mathscr{O}(\{\boldsymbol{a}\}; A)$, ta có $\Theta_{\boldsymbol{a}}(f) =f(\boldsymbol{a})$.

#### Mệnh đề 3 {#ts-i-s4-prop-3 .statement tag=02AC}

Cho B là một đại số Banach giao hoán có đơn vị và $\varphi$ là một cấu xạ liên tục có đơn vị từ A vào B. Cho $\boldsymbol{a}= (a_1, . . . , a_n)\in A^n$. Đặt $\boldsymbol{b}= (\varphi (a_1), . . . , \varphi (a_n))$, do đó Sp$^n_B(\boldsymbol{b})\subset$ Sp$^n_A(\boldsymbol{a})$. Với mọi $f\in \mathscr{O}$(Sp$^n_A(\boldsymbol{a}); A$), ta có

$$
\varphi (\Theta_{\boldsymbol{a}}(f)) = \Theta_{\boldsymbol{b}}(\varphi_*(f))
$$

trong đó $\varphi_*(f)$ ký hiệu mầm của $\varphi \circ f$ trong một lân cận của Sp$^n_B(\boldsymbol{b})$.

Chỉ cần chứng minh rằng với mọi lân cận mở U của Sp$^n_A(\boldsymbol{a})$ và mọi $f\in \mathscr{O}(U; A)$, ta có $\varphi (\Theta_{\boldsymbol{a}}(f)) = \Theta_{\boldsymbol{b}}(\varphi \circ f)$, trong đó $\varphi \circ f\in \mathscr{O}(U; B)$. Gọi $(h, u_1, . . . , u_n)$ là một dãy thích nghi với $\boldsymbol{a}$, trong đó giá của $h$ được chứa trong U (bổ đề 1 của I, p. 52 và bổ đề 3 của I, p. 54). Gọi $\omega$ là dạng vi phân liên kết. Với mọi $\boldsymbol{z}\in \mathbf{C}^n$, ta có

$$
\sum_{j=1}^n(z_j-b_j)\varphi (u_i(\boldsymbol{z})) =\varphi (\sum_{j=1}^n(z_j-a_j)u_j(\boldsymbol{z}))= 1-h(\boldsymbol{z})
$$

do đó dãy $(h, \varphi \circ u_1, . . . , \varphi \circ u_n)$ thích nghi với $\boldsymbol{b}$. Gọi $\omega '$ là dạng vi phân liên kết. Gọi $\mu$ là độ đo Lebesgue trên $\mathbf{C}^n$. Cho $f\in \mathscr{O}(U; A)$. Ta viết $\psi \cdot \mu$ cho độ đo vectơ liên kết với dạng vi phân $f \omega$. Độ đo vectơ liên kết với dạng vi phân

$$
(\varphi \circ f)\omega '= (\varphi \circ f)d(\varphi \circ u_1)\wedge dz_1\wedge  \cdots  \wedge d(\varphi \circ u_n)\wedge dz_n
$$

bằng $(\varphi \circ \psi )\cdot \mu$. Do đó, theo công thức (5), và INT, VI, §2, n$^o2$, prop. 2, ta có

$\Theta_{\boldsymbol{b}}(\varphi \circ f) =(2i\pi n$!$)^n\int_U(\varphi \circ f)\mu=(2ni\pi$!$)^n\varphi (\int_U\psi  \mu)=\varphi (\Theta_{\boldsymbol{a}}(f))$,

như phải chứng minh.

#### Hệ quả 1 {#ts-i-s4-prop-3-cor-1 .statement tag=02AD}

Cho $\chi \in \mathsf{X}(A)$ và $\boldsymbol{a}\in A^n$. Với mọi mầm $f\in \mathscr{O}$(Sp$^n(\boldsymbol{a})$), ta có $\chi (\Theta_{\boldsymbol{a}}(f)) =f(\chi (a_1), . . . , \chi (a_n))$.

Đây là một hệ quả của Mệnh đề 3, áp dụng cho cấu xạ có đơn vị liên tục $\chi : A\rightarrow \mathbf{C}$ (Định lý 1 của I, p. 29), và của hệ quả của Mệnh đề 2, áp dụng cho đại số Banach $\mathbf{C}$.

#### Nhận xét {#ts-i-s4-n5-rem-1 .statement tag=02AE}

Giả sử rằng đại số A không có căn. Cho $\boldsymbol{a}= (a_1, . . . , a_n)\in A^n$. Theo Mệnh đề 8 của I, p. 38, ánh xạ $\Theta^U_{\boldsymbol{a}}$ là ánh xạ duy nhất $\varphi$ từ $\mathscr{O}(U)$ vào A sao cho $\chi (\varphi (f)) =f(\chi (a_1), . . . , \chi (a_n))$ với mọi $\chi \in \mathsf{X}(A)$ và mọi hàm $f\in \mathscr{O}(U)$.

#### Hệ quả 2 {#ts-i-s4-prop-3-cor-2 .statement tag=02AF}

Cho $p$ là một số nguyên $\geqslant$ 1. Với mọi họ $(f_1, . . . , f_p)$ các phần tử của $\mathscr{O}$(Sp$^n(\boldsymbol{a})$), ta có

Sp$^p((\Theta_{\boldsymbol{a}}(f_1), . . . ,\Theta_{\boldsymbol{a}}(f_p))) = (f_1, . . . , f_p$)(Sp$^n(\boldsymbol{a})$).

Đặc biệt, với mọi $f\in \mathscr{O}$(Sp$^n(\boldsymbol{a})$), ta có Sp(Θ$_{\boldsymbol{a}}(f)$) $=f$(Sp$^n(\boldsymbol{a})$).

Điều này suy ra từ Hệ quả 1 và định nghĩa của phổ chung.

#### Ví dụ {#ts-i-s4-n5-exa-1 .statement tag=02AG}

Cho A là đại số Banach phức các hàm trên đường tròn đơn vị có chuỗi Fourier hội tụ tuyệt đối (I, p. 19, Ví dụ 8). Cho $\varphi \in$ A. Cho $f$ là một mầm của một hàm chỉnh hình trong một lân cận của tập giá trị của $\varphi$. Khi đó $\psi = \Theta_{\varphi}(f)$ là một chuỗi Fourier hội tụ tuyệt đối sao cho với mọi $u\in \mathbf{U}$ ta có $\psi (u) =f(\varphi (u))$ (Hệ quả 1, áp dụng cho các đặc trưng $\varphi \mapsto \varphi (u)$). Nói cách khác, hàm $f\circ \varphi$ trên đường tròn đơn vị cũng có một chuỗi Fourier hội tụ tuyệt đối (“định lý của P. Lévy”). Kết quả này tổng quát hóa định lý của Wiener (I, p. 38, Ví dụ 4), liên quan đến trường hợp của hàm $f(z) = 1/z$ trên $\mathbf{C}-\{0\}$ khi $\varphi$ không triệt tiêu.

### 6. Các định lý xấp xỉ

Trong số này, A là một đại số Banach phức giao hoán có đơn vị.

#### Mệnh đề 4 {#ts-i-s4-prop-4 .statement tag=02AH}

Cho L là một tập con compắc lồi đa thức của $\mathbf{C}^n$ và cho U là một lân cận mở của L. Với mọi hàm $f\in \mathscr{O}(U; A)$, tồn tại một dãy các hàm đa thức trên $\mathbf{C}^n$ với hệ số trong A hội tụ đến $f|L$ trong $\mathscr{C}(L; A)$.

Có thể giả sử rằng L không rỗng và A khác không. Gọi P (resp. $P_0$) là tập các hạn chế lên L của các hàm đa thức trên $\mathbf{C}^n$ với hệ số trong A (resp. với hệ số trong $\mathbf{C}$). Gọi B (resp. $B_0$) là bao đóng đại số Banach của P (resp. của $P_0$) trong $\mathscr{C}(L; A)$. Gọi $\iota$ là đơn ánh từ A lên đại số con định chuẩn của B gồm các hàm hằng.

Cho $z_1, . . . , z_n$ là các hạn chế lên L của các hàm tọa độ trên $\mathbf{C}^n$; chúng là các phần tử của $B_0$, và, đặt $\boldsymbol{z}= (z_1, . . . , z_n)$, ta có Sp$^n_{B_0}(\boldsymbol{z}) = L$ theo Mệnh đề 15 của I, p. 47.

Cho $f\in \mathscr{O}(U; A)$. Bằng hợp thành với $\iota$, hàm $f$ xác định một phần tử $f_B=\iota \circ f$ của $\mathscr{O}(U; B)$. Vì Sp$^n_B(\boldsymbol{z})\subset$ Sp$^n_{B_0}(\boldsymbol{z})\subset U$, ta có thể lập phần tử $b= \Theta_{\boldsymbol{z}}(f_B)$ của B. Đặt $\boldsymbol{w}= (w_1, . . . , w_n)\in L$, và gọi $\varphi$ là cấu xạ có đơn vị liên tục $g\mapsto g(\boldsymbol{w})$ từ B vào A. Ta có $\varphi \circ \iota =$ Id$_A$, do đó $\varphi \circ f_B=f$. Vì $\varphi (z_i) =w_i$, mệnh đề 3 của I, p. 66 suy ra $\varphi (\Theta_{\boldsymbol{z}}(f_B)) = \Theta_{\boldsymbol{w}}(\varphi \circ f_B)$. Vậy

$$
b(\boldsymbol{w}) =\varphi (b) =\varphi (\Theta_{\boldsymbol{z}}(f_B)) = \Theta_{\boldsymbol{w}}(\varphi \circ f_B) = \Theta_{\boldsymbol{w}}(f) =f(\boldsymbol{w})
$$

theo hệ quả của mệnh đề 2 của I, p. 65. Như vậy ta có $f|L =b$; đặc biệt, $f|L$ thuộc B. Điều này chứng minh mệnh đề.

#### Định lý 2 (Oka–Weil) {#ts-i-s4-thm-2 .statement tag=02AI}

Cho K là một tập con compắc lồi đa thức của $\mathbf{C}^n$ và P là tập các mầm trên một lân cận của K của các hàm đa thức trên $\mathbf{C}^n$ với hệ số trong A. Khi đó P trù mật trong $\mathscr{O}(K; A)$. Chính xác hơn, mọi phần tử của $\mathscr{O}(K; A)$ đều là giới hạn của một dãy các phần tử của P.

Xét một phần tử của $\mathscr{O}(K; A)$, là mầm của một hàm $f\in$ $\mathscr{O}(U; A)$, trong đó U là một lân cận mở của K. Theo bổ đề 7 của I, p. 48, tồn tại một lân cận compắc L của K được chứa trong U và lồi đa thức. Gọi V là phần trong của L; đó là một lân cận của K.

Theo mệnh đề trước, tồn tại một dãy $(P_k)$ các hàm đa thức trên $\mathbf{C}^n$ với hệ số trong A hội tụ đến $f|L$ trong $\mathscr{C}(L; A)$. Đặc biệt, dãy $(P_k)$ hội tụ đến $f|V$ trong $\mathscr{O}(V; A)$.

Theo định nghĩa của tôpô trên $\mathscr{O}(K; A)$ (xem EVT, II, p. 29, mệnh đề 5), ánh xạ chính tắc từ $\mathscr{O}(V; A)$ vào $\mathscr{O}(K; A)$ là liên tục. Do đó, dãy các mầm trên một lân cận của K của các hàm $P_k$ hội tụ đến mầm của $f$ trên một lân cận của K trong không gian $\mathscr{O}(K; A)$, điều phải chứng minh.

#### Hệ quả 1 {#ts-i-s4-thm-2-cor-1 .statement tag=02AJ}

Cho U là một lân cận mở của K. Cho $u_1$ và $u_2$ là các ánh xạ liên tục từ $\mathscr{O}(U; A)$ vào một không gian tôpô X, phân tích qua $\mathscr{O}(K; A)$. Khi đó $u_1=u_2$ khi và chỉ khi $u_1$ và $u_2$ trùng nhau trên tập các hạn chế lên K của các hàm đa thức trên $\mathbf{C}^n$ với hệ số trong A.

#### Hệ quả 2 {#ts-i-s4-thm-2-cor-2 .statement tag=02AK}

Cho E là một không gian Banach. Cho K là một tập con compắc lồi đa thức của $\mathbf{C}^n$. Cho P là tập các mầm trên một lân cận của K của các hàm đa thức trên $\mathbf{C}^n$ nhận giá trị trong E. Khi đó mọi phần tử của $\mathscr{O}(K; E)$ đều là giới hạn của một dãy các phần tử của P.

Trang bị cho E phép nhân xác định bởi $ab= 0$ với mọi $a$ và $b$ trong E (ví dụ 1 của I, p. 17). Đó là một đại số Banach giao hoán. Gọi A là đại số Banach giao hoán có đơn vị thu được từ E bằng phép nối thêm một phần tử đơn vị. Vì ánh xạ chính tắc $\mathscr{O}(K; A)\rightarrow \mathscr{O}(K; E)$ là liên tục, mệnh đề được suy ra từ định lý Oka-Weil áp dụng cho đại số A.

Với $n= 1$ và $A =\mathbf{C}$, ta còn có kết quả sau đây, sẽ được làm chính xác hơn bởi hệ quả 2 của I, p. 150.

#### Định lý 3 (Runge) {#ts-i-s4-thm-3 .statement tag=02AL}

Cho K là một tập con compắc của $\mathbf{C}$, và Q là tập các mầm của các hàm hữu tỉ chỉnh hình trên một lân cận của K. Khi đó Q trù mật trong $\mathscr{O}(K)$.

Theo định nghĩa của tôpô trên $\mathscr{O}(K)$, chỉ cần chứng minh rằng với mọi lân cận mở U của K, và mọi tập con compắc L của U, mọi hàm $f\in \mathscr{O}(U)$ đều là giới hạn của các hàm hữu tỉ liên tục trên L. Ta có thể giả sử rằng L là một lân cận compắc của K.

Gọi $Q'$ là tập hợp các hạn chế trên L của các hàm hữu tỉ trên $\mathbf{C}$ liên tục trên L, và gọi C là bao đóng của $Q'$ trong $\mathscr{C}(L)$. Đó là một đại số không có căn.

Gọi $z\in C$ là ánh xạ đồng nhất của L. Khi đó C là đại số con đóng đầy đủ của $\mathscr{C}(L)$ sinh bởi $z$ (bổ đề 2 của I, p. 6). Do đó Sp$_C(z) =$ Sp$_{\mathscr{C}(L)}(z) = L$. Vậy có thể lập phần tử $c= \Theta_z(f)$ của C. Vì C không có căn, áp dụng hệ quả 1 của I, p. 66 cho các đặc trưng $g\mapsto g(w)$ của C, với mọi $w\in L$, cho thấy rằng $c$ trùng với hạn chế của $f$ trên L. Theo định nghĩa của C, điều này chứng minh rằng $f|L$ là giới hạn đều trên L của các phần tử của $Q'$, và điều này hoàn tất chứng minh của định lý.

### 7. Sự tồn tại và tính duy nhất của phép tính phiếm hàm chỉnh hình

Ta giả sử rằng A là một đại số Banach phức giao hoán có đơn vị.

#### Định nghĩa 2 {#ts-i-s4-def-2 .statement tag=02AM}

Gọi $n\geqslant 1$ là một số nguyên và gọi $\boldsymbol{a}\in A^n$. Gọi U là một lân cận mở của Sp$^n(\boldsymbol{a})$. Ta nói rằng một họ $\boldsymbol{a}'$ là một bao của $(\boldsymbol{a},U)$ nếu $\boldsymbol{a}'\in \mathbf{C}^{n+p}$ mở rộng $\boldsymbol{a}$ và nếu $U\times \mathbf{C}^p$ chứa bao lồi đa thức của Sp$^{n+p}(\boldsymbol{a}')$.

#### Bổ đề 11 {#ts-i-s4-lem-11 .statement tag=02AN}

Gọi $n\geqslant 1$ là một số nguyên. Gọi $\boldsymbol{a}\in A^n$. Với mọi lân cận mở U của Sp$^n(\boldsymbol{a})$, tồn tại một bao của $(\boldsymbol{a},U)$.

Gọi $(a_{\lambda})_{\lambda\in\Lambda}$ là một họ các phần tử của A mở rộng họ $\boldsymbol{a}$ và sinh tôpô đại số Banach có đơn vị A. Gọi $\pi$ là phép chiếu chính tắc của $\mathbf{C}^{\Lambda}$ lên $\mathbf{C}^n$ và gọi $U'=\pi^{-1}(U)$. Khi đó $U'$ là một lân cận của Sp$^{\Lambda}((a_{\lambda}))$, và Sp$^{\Lambda}((a_{\lambda}))$ là lồi đa thức (I, p. 44, bổ đề 4). Theo bổ đề 6 của I, p. 47, tồn tại một tập con hữu hạn $\Lambda_0$ của Λ chứa $\{1,2, . . . , n\}$ sao cho pr$_{\Lambda_0}(U')$ chứa bao lồi đa thức S của pr$_{\Lambda_0}$(Sp$^{\Lambda}((a_{\lambda})_{\lambda\in\Lambda})$) $=$ Sp$^{\Lambda_0}((a_{\lambda})_{\lambda\in\Lambda_0})$. Gọi $p\geqslant 0$ là số nguyên sao cho $\Lambda_0$ có lực lượng $n+p$, và gọi $j$ là một song ánh từ $\{1, . . . , n+p\}$ lên $\Lambda_0$ trùng với ánh xạ đồng nhất trên $\{1, . . . , n\}$. Vì phép chiếu của S được chứa trong U, họ $(a_{j(k)})_{1\leqslant k\leqslant n+p}$ là một bao của $(\boldsymbol{a},U)$.

#### Mệnh đề 5 {#ts-i-s4-prop-5 .statement tag=02AO}

Dữ liệu của các ánh xạ $\Theta_{\boldsymbol{a}}$, với $n\geqslant 1$ và $\boldsymbol{a}\in A^n$, tạo thành một phép tính phiếm hàm chỉnh hình trên A, nghĩa là các điều kiện (CF1), (CF2) và (CF3) của I, p. 51 được thỏa mãn.

Cho $n\geqslant 1$ là một số nguyên và $\boldsymbol{a}= (a_1, . . . , a_n)\in A^n$. Ánh xạ $\Theta_{\boldsymbol{a}}$ thỏa mãn $\Theta_{\boldsymbol{a}}(z_i) =a_i$ với mọi $i$ sao cho $1\leqslant i\leqslant n$ theo bổ đề 10 của I, p. 64, điều đó chứng minh tính chất (CF2). Bổ đề 9 của I, p. 63 suy ra tính chất (CF3) của các ánh xạ $\Theta_{\boldsymbol{a}}$.

Ánh xạ $\Theta_{\boldsymbol{a}}$ là A-tuyến tính và liên tục (I, p. 61, n$^o5$). Nó thỏa mãn $\Theta_{\boldsymbol{a}}(1) = 1$ (bổ đề 9 của I, p. 63). Để kiểm tra điều kiện (CF1), còn phải thiết lập rằng $\Theta_{\boldsymbol{a}}$ là một cấu xạ đại số. Để làm điều đó, chúng ta sẽ chứng minh rằng $\Theta^U_{\boldsymbol{a}}$ là một cấu xạ đại số với mọi lân cận mở U của Sp$^n(\boldsymbol{a})$.

Trước hết giả sử rằng U chứa bao lồi đa thức K của Sp$^n(\boldsymbol{a})$. Cho $f_1$ và $f_2$ là các phần tử của $\mathscr{O}(U; A)$. Tồn tại một dãy $(f_{1,k})$ (resp. $(f_{2,k})$) các hàm đa thức hội tụ tới $f_1$ (resp. tới $f_2$) trong $\mathscr{O}(K; A)$ (định lý 2 của I, p. 68), do đó trong $\mathscr{O}$(Sp$^n(\boldsymbol{a}); A$). Với mọi số nguyên $k$, ta có

$$
\Theta^U_{\boldsymbol{a}}(f_{1,k})\Theta^U_{\boldsymbol{a}}(f_{2,k}) = \Theta^U_{\boldsymbol{a}}(f_{1,k}f_{2,k})
$$

theo bổ đề 10 của I, p. 64, do đó $\Theta^U_{\boldsymbol{a}}(f_1)\Theta^U_{\boldsymbol{a}}(f_2) = \Theta^U_{\boldsymbol{a}}(f_1f_2)$ khi chuyển qua giới hạn.

Xét trường hợp tổng quát. Cho $\boldsymbol{a}'\in \mathbf{C}^{n+p}$ là một phủ của $(\boldsymbol{a},U)$ (bổ đề 11) và $\pi : U\times \mathbf{C}^p\rightarrow U$ là phép chiếu chính tắc. Vì $U\times \mathbf{C}^p$ chứa bao lồi đa thức của Sp$^{n+p}(\boldsymbol{a}')$, ta có

$$
\Theta^{U\times\mathbf{C}^p}_{\boldsymbol{a}'}(f_1\circ \pi )\Theta^{U\times\mathbf{C}^p}_{\boldsymbol{a}'}(f_2\circ \pi ) = \Theta^{U\times\mathbf{C}^p}_{\boldsymbol{a}'}(f_1f_2\circ \pi )
$$

với $f_1$ và $f_2$ trong $\mathscr{O}(U; A)$ theo trường hợp thứ nhất. Vì, với mọi hàm $f\in \mathscr{O}(U; A)$, ta có $\Theta^{U\times\mathbf{C}^p}_{\boldsymbol{a}'}(f\circ \pi ) = \Theta^U_{\boldsymbol{a}}(f)$ (điều kiện (CF3) đã chứng minh ở trên), kết luận suy ra, và do đó điều kiện (CF1) cũng vậy.

Bây giờ chúng ta có thể chứng minh định lý 1 của I, p. 51. Mệnh đề 5 cho thấy rằng họ các ánh xạ $(\Theta_{\boldsymbol{a}})_{\boldsymbol{a}}$ là một phép tính phiếm hàm chỉnh hình trên A. Vì vậy chỉ còn phải thiết lập tính duy nhất của phép tính phiếm hàm chỉnh hình trên A.

Cho $(\Psi_{\boldsymbol{a}})_{\boldsymbol{a}}$ là một họ các ánh xạ được xác định với mọi số nguyên $n\geqslant 1$ và mọi $\boldsymbol{a}\in A^n$ và thỏa mãn các điều kiện (CF1), (CF2), (CF3) của phép tính phiếm hàm chỉnh hình trên A (I, p. 51). Chỉ cần chứng minh rằng với mọi số nguyên $n\geqslant 1$, với mọi $\boldsymbol{a}\in A^n$ và với mọi lân cận mở U của $\boldsymbol{a}$, ta có $\Theta^U_{\boldsymbol{a}}= \Psi^U_{\boldsymbol{a}}$.

Cho $n\geqslant 1$ và $\boldsymbol{a}= (a_1, . . . , a_n)\in A^n$. Cho U là một lân cận mở của Sp$^n(\boldsymbol{a})$. Trước hết giả sử rằng U chứa bao lồi đa thức K của Sp$^n(\boldsymbol{a})$. Các cấu xạ $\Theta^U_{\boldsymbol{a}}$ và $\Psi^U_{\boldsymbol{a}}$ trùng nhau trên các hàm đa thức theo các tính chất (CF1) và (CF2). Bởi hệ quả của định lý 2 của I, p. 68 và tính chất liên tục (CF1), do đó các cấu xạ này bằng nhau.

Hãy chứng minh trường hợp tổng quát. Cho $\boldsymbol{a}'\in \mathbf{C}^{n+p}$ là một phủ của $(\boldsymbol{a},U)$ và $\pi : U\times \mathbf{C}^p\rightarrow U$ là phép chiếu chính tắc. Ta có

$$
\Theta^U_{\boldsymbol{a}}= \Theta^{U\times\mathbf{C}^p}_{\boldsymbol{a}'}\circ \pi^*= \Psi^{U\times\mathbf{C}^p}_{\boldsymbol{a}'}\circ \pi^*= \Psi^U_{\boldsymbol{a}}
$$

theo tính chất (CF3) và trường hợp trước. Điều này kết thúc chứng minh của định lý 1 của I, p. 51.

Hãy nhận xét rằng định lý 2 của I, p. 68 cũng kéo theo kết quả tính duy nhất sau đây:

#### Mệnh đề 6 {#ts-i-s4-prop-6 .statement tag=02AP}

Cho $\boldsymbol{a}\in A^n$. Giả sử Sp$^n(\boldsymbol{a})$ là lồi đa thức. Gọi $z_1, . . . , z_n$ là các mầm trong một lân cận của Sp$^n(\boldsymbol{a})$ của các hàm tọa độ trên $\mathbf{C}^n$. Khi đó ánh xạ $\Theta_{\boldsymbol{a}}$ là cấu xạ đại số liên tục có đơn vị duy nhất $\varphi$ từ $\mathscr{O}$(Sp$^n(\boldsymbol{a}); A$) vào A sao cho $\varphi (z_1) =a_1, . . . , \varphi (z_n) =a_n$.

Bổ đề 10 của I, p. 64 và hệ quả của mệnh đề 2 của I, p. 65 biện minh cho các ký hiệu sau đối với phép tính phiếm hàm chỉnh hình. Cho $n\geqslant 1$ và $\boldsymbol{a}\in A^n$. Với mọi mầm $f\in \mathscr{O}(K; A)$ (resp. với mọi hàm chỉnh hình $f\in \mathscr{O}(U; A)$ trên một lân cận mở U của Sp$^n(\boldsymbol{a})$), đặt

$$
f(\boldsymbol{a}) = \Theta_{\boldsymbol{a}}(f) \tag{6}
$$

Ký hiệu này phù hợp với ký hiệu đã được đưa vào trong A, IV, p. 4, n$^o3$, nếu $f$ là một đa thức, theo các tính chất (CF1) và (CF2).

Khi đó các tính chất (CF2) và (CF3) của I, p. 51 có thể được viết thành

$$
z_i(\boldsymbol{a}) =a_i,1\leqslant i\leqslant n,(f\circ \pi_{m,n})(\boldsymbol{a}) =f(\pi_{m,n}(\boldsymbol{a}))
$$

### 8. Phép thế trong phép tính phiếm hàm

Với các ký hiệu đã được đưa vào ở trên, các mệnh đề của hệ quả 1 của I, p. 66 và của hệ quả 2 của I, p. 67 lần lượt trở thành

$\chi (g(\boldsymbol{a})) =g(\chi (a_1), . . . , \chi (a_n))$, Sp($g(\boldsymbol{a})$) $=g$(Sp$^n(\boldsymbol{a})$)

đối với $f\in \mathscr{O}$(Sp$^n(\boldsymbol{a}); A$)$,\chi \in \mathsf{X}(A)$ và $g\in \mathscr{O}$(Sp$^n(\boldsymbol{a})$).

Bây giờ chúng tôi sẽ chứng minh một tính chất phép thế tổng quát hơn.

#### Định lý 4 {#ts-i-s4-thm-4 .statement tag=02AQ}

Cho A là một đại số Banach phức giao hoán có đơn vị, cho $n\geqslant 1$ là một số nguyên, và cho $\boldsymbol{a}= (a_1, . . . , a_n)\in A^n$. Cho $\boldsymbol{f}=$ $(f_1, . . . , f_p)$, trong đó $f_1, . . . , f_p$ là các phần tử của $\mathscr{O}$(Sp$^n(\boldsymbol{a})$). Ảnh của Sp$^n(\boldsymbol{a})$ dưới ánh xạ $\boldsymbol{z}\mapsto \boldsymbol{f}(\boldsymbol{z}) = (f_1(\boldsymbol{z}), . . . , f_p(\boldsymbol{z}))$ bằng Sp$^p(\boldsymbol{f}(\boldsymbol{a}))$.

Với mọi $g\in \mathscr{O}$(Sp$^p(\boldsymbol{f}(\boldsymbol{a})); A$), mầm hợp thành $g\circ \boldsymbol{f}$ là một phần tử của $\mathscr{O}$(Sp$^n(\boldsymbol{a}); A$) và ta có $g(\boldsymbol{f}(\boldsymbol{a})) = (g\circ \boldsymbol{f})(\boldsymbol{a})$.

Khẳng định thứ nhất về ảnh của Sp$^n(\boldsymbol{a})$ suy ra từ hệ quả 2 của I, p. 67. Để chứng minh khẳng định thứ hai, chúng tôi sẽ dùng bổ đề sau.

#### Bổ đề 12 {#ts-i-s4-lem-12 .statement tag=02AR}

Cho K là bao lồi đa thức của Sp$^p(\boldsymbol{f}(\boldsymbol{a}))$. Ta có $g(\boldsymbol{f}(\boldsymbol{a})) = (g\circ \boldsymbol{f})(\boldsymbol{a})$ với mọi mầm $g\in \mathscr{O}(K; A)$.

Gọi Ψ là ánh xạ từ $\mathscr{O}(K; A)$ vào A sao cho $\Psi (g) = (g\circ \boldsymbol{f})(\boldsymbol{a})$. Đó là một cấu xạ có đơn vị liên tục sao cho $\Psi (z_j) =f_j(\boldsymbol{a})$, trong đó $z_j$ là mầm của hàm tọa độ thứ $j$ trên $\mathbf{C}^p$. Do đó khi $g$ là mầm của một hàm đa thức, ta có $\Psi (g) =g(\boldsymbol{f}(\boldsymbol{a}))$. Theo định lý 2 của I, p. 68, công thức này vẫn đúng với mọi $g\in \mathscr{O}(K; A)$.

Bây giờ chúng ta hãy chứng minh định lý. Cho V là một lân cận mở của Sp$^p(\boldsymbol{f}(\boldsymbol{a}))$ và $\widetilde{g}\in \mathscr{O}(V; A)$ là một hàm chỉnh hình mà mầm của nó trong một lân cận của Sp$^p(\boldsymbol{f}(\boldsymbol{a}))$ bằng $g$. Cho $\boldsymbol{b}\in \mathbf{C}^{p+q}$ là một bao của $(\boldsymbol{f}(\boldsymbol{a}),V)$ (Bổ đề 11 của I, p. 70) và $\pi : V\times \mathbf{C}^q\rightarrow V$ là phép chiếu chính tắc.

Cho $\widetilde{f}_1, . . . ,\widetilde{f}_p$ là các hàm chỉnh hình mà các mầm của chúng là $f_1, . . . , f_p$ và cho U là một lân cận mở của Sp$^n(\boldsymbol{a})$ sao cho $(\widetilde{f}_1, . . . ,\widetilde{f}_p)(U)\subset V$. Cho $\pi '$ là phép chiếu chính tắc của $U\times \mathbf{C}^q$ lên U. Ký hiệu bởi $z_{n+1}, . . . , z_{n+q}$ các hàm tọa độ cuối cùng của $\mathbf{C}^{n+q}$. Đặt $h=\widetilde{g}\circ (\widetilde{f}_1, . . . ,\widetilde{f}_p)$ và

$$
\boldsymbol{c}= (a_1, . . . , a_n, b_{p+1}, . . . , b_{p+q})\in A^{n+q}
$$

Ánh xạ $\widetilde{g}\circ \pi$ là chỉnh hình trong lân cận mở $V\times \mathbf{C}^q$ của bao lồi đa thức L của Sp$^{p+q}(\boldsymbol{b})$. Theo Bổ đề 12, áp dụng cho $\boldsymbol{c}$, cho các mầm trong một lân cận của L của các hàm

$$
(\widetilde{f}_1\circ \pi ', . . . ,\widetilde{f}_p\circ \pi ', z_{n+1}, . . . , z_{n+q})
$$

và cho mầm của $\widetilde{g}\circ \pi$, ta có

$$
(g\circ \pi )((f_1\circ \pi ')(\boldsymbol{c}), . . . ,(f_p\circ \pi ')(\boldsymbol{c}), z_{n+1}(\boldsymbol{c}), . . . , z_{n+q}(\boldsymbol{c}))= (h\circ \pi ')(\boldsymbol{c})
$$

Vì $\pi '(\boldsymbol{c}) =\boldsymbol{a}$, nên ta có $(h\circ \pi ')(\boldsymbol{c}) =h(\boldsymbol{a})$ và $(f_i\circ \pi ')(\boldsymbol{c}) =f_i(\boldsymbol{a})$ với $1\leqslant i\leqslant p$ (tính chất (CF3) của phép tính phiếm hàm chỉnh hình). Hơn nữa, vì $z_{n+j}(\boldsymbol{c}) =b_{p+j}$ với $1\leqslant j\leqslant q$ (tính chất (CF2)), ta có

$$
(g\circ \pi )(f_1(\boldsymbol{a}), . . . , f_p(\boldsymbol{a}), b_{p+1}, . . . , b_{p+q}) =h(\boldsymbol{a})
$$

do đó suy ra $g(f_1(\boldsymbol{a}), . . . , f_p(\boldsymbol{a})) =h(\boldsymbol{a})$ bằng cách áp dụng lại tính chất (CF3).

### 9. Phép Tính Phiếm Hàm Chỉnh Hình Một Biến

#### Định lý 5 {#ts-i-s4-thm-5 .statement tag=02AS}

Cho A là một đại số Banach có đơn vị, không nhất thiết giao hoán. Cho $a$ là một phần tử của A và $z$ là mầm của hàm đồng nhất của $\mathbf{C}$ trong một lân cận của Sp$_A(a)$. Tồn tại duy nhất một cấu xạ liên tục có đơn vị $\varphi_a$ từ $\mathscr{O}$(Sp$_A(a)$) vào A sao cho $\varphi_a(z) =a$.

Ảnh của $\varphi_a$ được chứa trong đại số con đầy đủ đóng của A sinh bởi $a$. Đặc biệt, nó được chứa trong đối giao hoán tử kép của $a$.

Hãy chứng minh sự tồn tại của cấu xạ $\varphi_a$. Cho B là đại số con đầy đủ đóng của A sinh bởi $a$. Nó giao hoán, và ta có Sp$_B(a) =$ Sp$_A(a)$ (I, p. 5, No$^o5$). Ánh xạ $\Theta_a$ của phép tính phiếm hàm chỉnh hình trên B là một cấu xạ liên tục có đơn vị từ $\mathscr{O}$(Sp$_B(a)$) vào B sao cho $\Theta_a(z) =a$ (Định lý 1 của I, p. 51). Cấu xạ hợp thành bởi $\Theta_a$ và đơn ánh chính tắc từ B vào A là một cấu xạ liên tục có đơn vị $\varphi_a$ từ $\mathscr{O}$(Sp$_A(a)$) vào A sao cho ảnh của $z$ là $a$.

Hãy chứng minh tính duy nhất. Cho $\varphi '_a$ là một cấu xạ liên tục có đơn vị từ $\mathscr{O}$(Sp$_A(a)$) vào A sao cho $\varphi '_a(z) =a$. Khi đó $\varphi_a$ và $\varphi '_a$ trùng nhau trên tập các mầm của các đa thức trong một lân cận của Sp$_A(a)$, do đó trên tập các mầm của các phân thức hữu tỉ chỉnh hình trong một lân cận của Sp$_A(a)$. Nhưng các mầm này là trù mật trong $\mathscr{O}$(Sp$_A(a)$) (I, p. 69, đl. 3). Điều này kéo theo $\varphi_a=\varphi '_a$.

Phép dựng của $\varphi_a$ chứng tỏ rằng ảnh của nó được chứa trong đại số con giao hoán B, mà B được chứa trong đối giao hoán tử kép của $a($I, p. 6).

Nếu căn của đại số A bằng không, thì tính duy nhất của cấu xạ $\varphi_a$ là đúng mà không cần giả thiết nó liên tục (x. mệnh đề 9 của I, p. 40). Nói chung điều này không còn đúng nữa, x. G. R. Allan, Embedding the algebra of formal power series in a Banach algebra, Proc. London Math. Soc. (3) 25 (1972), 329–340.

Với mọi đại số Banach A, mọi phần tử $a$ của A và mọi mầm $f\in \mathscr{O}$(Sp$_A(a)$), người ta ký hiệu bởi $f(a)$ phần tử $\varphi_a(f)$ của định lý 5. Nếu A là một đại số Banach giao hoán, thì phần tử $f(a)$ này trùng với phần tử $f(a)$ do phép tính phiếm hàm chỉnh hình trên một đại số Banach giao hoán cung cấp (định lý 1 của I, p. 51).

Cho B là đại số con đầy đủ đóng của A sinh bởi $a$, sao cho Sp$_A(a) =$ Sp$_B(a)$. Phần tử $f(a)$ của A thuộc về B, và trùng với phần tử $f(a)$ được tính đối với đại số B.

#### Mệnh đề 7 {#ts-i-s4-prop-7 .statement tag=02AT}

Cho A và B là các đại số Banach có đơn vị và $\varphi$ là một cấu xạ liên tục có đơn vị từ A vào B. Cho $a\in$ A. Khi đó Sp$_B(\varphi (a))\subset$ Sp$_A(a)$ và ta có $\varphi (f(a))$ = $f(\varphi (a))$ với mọi $f\in \mathscr{O}$(Sp$_A(a)$). Đặc biệt, với mọi $\chi \in \mathsf{X}(A)$, ta có $\chi (f(a)) =f(\chi (a))$.

Điều này suy ra từ mệnh đề 3 của I, p. 66.

#### Mệnh đề 8 {#ts-i-s4-prop-8 .statement tag=02AU}

Cho A là một đại số Banach có đơn vị và $a\in A$. Cho $f\in \mathscr{O}$(Sp($a$)). Ta có $f$(Sp$_A(a)$) $=$ Sp$_A(f(a))$. Hơn nữa, với mọi $g\in \mathscr{O}$(Sp$_A(f(a))$), ta có $g\circ f\in \mathscr{O}$(Sp$_A(a)$) và $g(f(a)) = (g\circ f)(a)$.

Điều này suy ra từ đl. 4.

#### Mệnh đề 9 {#ts-i-s4-prop-9 .statement tag=02AV}

Cho A là một đại số Banach có đơn vị và $a\in A$. Cho U là một lân cận mở của Sp$_A(a)$ và $f\in \mathscr{O}(U)$. Giả sử thêm rằng V là một lân cận compắc của Sp$_A(a)$ được chứa trong U sao cho V là một mảnh của U với biên định hướng $\partial V$.

Với mọi số nguyên $n\geqslant 0$, ánh xạ $z\mapsto f(z)(z-a)^{-n-1}$ liên tục trên $\partial V$, dạng vi phân $z\mapsto f(z)(z-a)^{-n-1}dz$ khả tích trên $\partial V$ và ta có

(7) $f^{(n)}(a) =2ni\pi$! $\int_{\partial V}f(z)(z-a)^{-n-1}dz$

trong đó $f^{(n)}\in \mathscr{O}(U)$ là đạo hàm thứ $n$ của $f$.

Ta tiến hành bằng quy nạp theo $n$. Khi $n= 0$, kết quả suy ra từ Mệnh đề 1 của I, p. 61. Bây giờ giả sử rằng mệnh đề của mệnh đề này là đúng với số nguyên $n\geqslant 0$. Gọi $g\in \mathscr{O}(\mathbf{C}-$ Sp$_A(a); A)$ là hàm chỉnh hình được xác định bởi $g(z) = (z-a)^{-n-1}f(z)$. Dạng vi phân $g'(z)dz$ = $dg$ thuộc lớp $C^1$; vì mảnh V là compắc, công thức Stokes (VAR, R2, p. 47, 11.2.3) suy ra

$$
\int_{\partial V}g'(z)dz=\int_{\partial V}dg= 0
$$

Vì $g'(z) = (z-a)^{-n-1}f'(z)-(n+1)(z-a)^{-n-2}f(z)$, ta suy ra

$$
\int_{\partial V}f'(z)(z-a)^{-n-1}dz= (n+ 1)\int_{\partial V}f(z)(z-a)^{-n-2}dz
$$

Áp dụng giả thiết quy nạp cho $f'$, do đó ta được

$2ni\pi$! $f^{(n+1)}(a) = (n+ 1)\int_{\partial V}f(z)(z-a)^{-n-2}dz$,

đó là mệnh đề của mệnh đề này đối với số nguyên $n+ 1$. Điều này hoàn tất chứng minh.

#### Mệnh đề 10 {#ts-i-s4-prop-10 .statement tag=02AW}

Cho A là một đại số Banach có đơn vị và U là một tập con mở của $\mathbf{C}$.

a) Tập hợp Ω gồm các $a\in A$ sao cho Sp$_A(a)\subset U$ là mở trong A;

b) Cho $f\in \mathscr{O}(U)$. Ánh xạ $a\mapsto f(a)$ từ Ω vào A là chỉnh hình, và đặc biệt là liên tục.

Cho $a\in \Omega$. Tồn tại một lân cận compắc V của Sp$_A(a)$ được chứa trong U và là một mảnh của U (VAR, R2, p. 46 and p. 47, 11.1.3, d)).

Vì hàm giải thức của $a$ tiến tới 0 tại vô cực (Định lý 1, c) của I, p. 24), ánh xạ $z\mapsto  \|(z-a)^{-1}\|$ bị chặn trên $\mathbf{C}-\mathring{V}$. Gọi M là cận trên bé nhất của nó. Nếu $h\in A$ sao cho $\|h\|\leqslant (2M)^{-1}$ và nếu $z\in \mathbf{C}-\mathring{V}$, ta có

$$
z-(a+h) = (1-h(z-a)^{-1})(z-a)
$$

và $\|h(z-a)^{-1}\|\leqslant \frac{1}{2}$, do đó $z-(a+h)$ khả nghịch và nghịch đảo của nó thỏa mãn

$$
(z-(a+h))^{-1}= (z-a)^{-1}\sum_{n=0}^{\infty}(h(z-a)^{-1})^n \tag{8}
$$

với $\|(h(z-a)^{-1})^n\|\leqslant 2^{-n}$ (Mệnh đề 2 của I, p. 22). Do đó Sp$_A(a+h)$ được chứa trong V, nên trong U, điều này chứng minh rằng Ω là mở trong A.

Cho $f\in \mathscr{O}(U)$. Gọi $m$ là cận trên bé nhất của $|f(z)|$ với $z\in \partial V$. Cho $a\in A$. Với mọi $h\in A$ sao cho $\|h\|\leqslant (2M)^{-1}$, ta có

$$
f(a+h) =\frac{1}{2i\pi}\int_{\partial V}f(z)(z-(a+h))^{-1}dz
$$

(Mệnh đề 9). Chuỗi (8) hội tụ đều trên biên của V, do đó

$$
f(a+h) =\sum_{n=0}^{+\infty}f_{a,n}(h)
$$

trong đó ánh xạ $f_{a,n}$ từ A vào A được xác định bởi

$$
f_{a,n}(h) =\frac{1}{2i\pi}\int_{\partial V}f(z)(z-a)^{-1}(h(z-a)^{-1})^ndz
$$

Với mọi $n\in \mathbf{N}$, hàm $f_{a,n}$ là một hàm đa thức thuần nhất liên tục bậc $n$. Hơn nữa, ta được

$$
\|f_{a,n}(h)\|\leqslant \frac{mM}{\pi}(\int_{\partial V}\|dz\|)2^{-(n+1)}
$$

(INT, VI, §2, No.$^o3$, Mệnh đề 5). Do đó chuỗi $\sum_nf_{a,n}(h)$ hội tụ tuyệt đối với $\|h\|\leqslant (2M)^{-1}$. Điều này chứng minh rằng ánh xạ gán $f(a)$ cho $a$ là chỉnh hình trên Ω (VAR, R1, p. 26, 3.2.1).

#### Mệnh đề 11 {#ts-i-s4-prop-11 .statement tag=02AX}

Cho A là một đại số Banach có đơn vị, $a\in A$ và U là một lân cận mở của Sp$_A(a)$. Ký hiệu $\delta$ là khoảng cách từ Sp$_A(a)$ đến $\mathbf{C}-$ U. Cho $f\in \mathscr{O}(U)$.

a) Với mọi số thực $\eta$ sao cho $0< \eta  < \delta$, tồn tại một số thực $C\geqslant 0$ sao cho $\|f^{(n)}(a)\|\leqslant Cn$!$\eta^{-n}$ với mọi số nguyên $n\in \mathbf{N}$;

b) Nếu $b\in A$ giao hoán với $a$ và nếu $\varrho (b)< \delta$, ta có Sp$_A(a+b)\subset U$, và

$\infty (n)$

$f(a+b) =\sum fn$!$(a)b^n$,

$n=0$

trong đó chuỗi hội tụ tuyệt đối.

Cho $\eta$ là một số thực sao cho $0< \eta  < \delta$. Đặt $\varepsilon =\delta -\eta  >0$. Cho K là lân cận compắc của Sp$_A(a)$ gồm các điểm của $\mathbf{C}$ có khoảng cách đến Sp$_A(a)$ là $\leqslant \varepsilon /2$. Vì $f$ chỉnh hình trong mọi đĩa mở bán kính $\eta +\varepsilon /2$ có tâm thuộc K, nên theo các bất đẳng thức Cauchy (VAR, R1, p. 29, 3.3.4), tồn tại một số thực $C\geqslant 0$ sao cho

sup$_{z\in K}|f^(\overset{n)}{n}$!$(z)|\leqslant \frac{C}{\eta^n}$

với mọi số nguyên $n\geqslant 0$. Khi đó mệnh đề a) suy ra từ Mệnh đề 1 của I, p. 61 áp dụng cho $f^{(n)}$ và cho một mảnh V được chứa trong K.

Cho $b$ là một phần tử của A giao hoán với $a$ sao cho $\varrho (b)< \delta$. Thay thế A bằng đại số con đóng đầy đủ B sinh bởi $a$ và $b$, đại số này thỏa mãn Sp$_A(a) =$ Sp$_B(a)$ và Sp$_A(a+b) =$ Sp$_B(a+b)$, để chứng minh b), ta quy về trường hợp A giao hoán.

Vì $\varrho (b)< \delta$, ta có thể chọn $\eta$ sao cho $\varrho (b)< \eta  < \delta$. Gọi $V_1$ là tập hợp các điểm của $\mathbf{C}$ có khoảng cách tới Sp$_A(a)$ là $< \delta -\eta$, và $V_2$ là đĩa mở tâm 0 bán kính $\eta$ trong $\mathbf{C}$. Gọi $g$ là ánh xạ $(z_1, z_2)\mapsto z_1+z_2$ từ $V_1\times V_2$ vào U. Khi đó $h=f\circ g$ là ánh xạ $(z_1, z_2)\mapsto f(z_1+z_2)$ từ $V_1\times V_2$ vào $\mathbf{C}$. Ta có Sp$^2_A(a, b)\subset V_1\times V_2$, do đó Sp$_A(a+b)\subset U$ (x. hệ quả 2 của I, p. 67), và hơn nữa $f(a+b) =h(a, b)$ theo định lý 4 của I, p. 72. Bây giờ, trong không gian $\mathscr{O}(V_1\times V_2)$, ta có

$h(z_1, z_2) =\sum_{n\geqslant 0}f^{(n}\overset{)}{n}($!$z_1)z_2^n$,

(VAR, R1, p. 29, 3.3.4), do đó chuỗi

$\sum f^(\overset{n)}{n}$!$(a)b^n$

với $n\geqslant 0$ hội tụ trong A và tổng của nó là $h(a, b) =f(a+b)$. Hơn nữa, chuỗi này hội tụ tuyệt đối theo mệnh đề a).

### 10. Hàm mũ và lôgarit

Hàm mũ phức từ $\mathbf{C}$ vào $\mathbf{C}$ được ký hiệu là exp (FVR, III, p. 8, định nghĩa 2). Nó khả vi và thỏa exp$'=$ exp (FVR, III, p. 9, (26)), do đó là chỉnh hình trên $\mathbf{C}$. Cho A là một đại số Banach có đơn vị và $a$ là một phần tử của A. Theo mệnh đề 2 của I, p. 65 và công thức (9) của FVR, III, p. 16, ta có

$\infty n$

(9) exp($a$) $=\sum an$!.

$n=0$

Vì $\|a^n\|\leqslant \|a\|^n$, ta thấy $\|$exp($a$)$\|\leqslant$ exp($\|a\|$) và chuỗi (9) hội tụ đều trong mọi quả cầu của A. Ánh xạ $a\mapsto$ exp($a$) từ A vào A là chỉnh hình (mệnh đề 10 của I, p. 76). Hàm mũ của $a\in A$ đôi khi cũng được ký hiệu là $e^a$.

Khi $a$ là một tự đồng cấu của một không gian Banach E, hàm mũ exp($a$) thu được trong đại số Banach $\mathscr{L}(E)$ trùng với hàm mũ được định nghĩa trong FVR, IV, p. 27, định nghĩa 1, theo mệnh đề 7 (3) ở chỗ đã dẫn.

Với mọi phần tử $b$ của A giao hoán với $a$, ta cũng có

exp($a+b$) $=\sum^{\infty}bn^n$! exp($a$),

$n=0$

(mệnh đề 11 của I, p. 77), do đó

(10) exp($a+b$) $=$ exp($a$)$\cdot$ exp($b$).

Đặc biệt, exp($a$) là khả nghịch và

(11) exp($a$)$^{-1}=$ exp($-a$).

Gọi B là tập hợp các $z\in \mathbf{C}$ sao cho $-\pi  <\mathscr{I}z < \pi$. Gọi F là phần bù trong $\mathbf{C}$ của khoảng $\mathbf{R}_-$. Hạn chế của ánh xạ mũ lên B, bằng cách chuyển qua các không gian con, cảm sinh một song ánh từ B lên F (FVR, III, p. 10, n$^o7$), song ánh nghịch đảo của nó sẽ được ký hiệu là log.

Nếu $a\in A$ sao cho Sp$_A(a)\subset F$, ta có thể lập phần tử log($a$) của A. Ta có Sp$_A$(log($a$))$\subset B$, và

(12) exp(log($a$)) $=a$ theo mệnh đề 8 của I, p. 75. Ngược lại, gọi $b$ là một phần tử của A sao cho Sp$_A(b)\subset B$. Ta có Sp$_A$(exp($b$))$\subset F$ và

(13) log(exp($b$)) $=b$

(nơi đã dẫn).

Đặc biệt, nếu $a\in A$ sao cho $\varrho (a)<1$, thì ta có Sp$_A(1-a)\subset F$ và ta có thể lập log(1 $-a$). Với $n\geqslant 1$, đạo hàm bậc $n$ của ánh xạ $z\mapsto$ log(1$-z$) là $z\mapsto  -(n-$1)!(1$-z$)$^{-n}$ Vậy khai triển chuỗi lũy thừa của ánh xạ $z\mapsto$ log(1 $-z$) tại điểm 0 là

log(1 $-z$) $=-\sum^{\infty}\frac{z^n}{n}$,

$n=1$

đúng với $|z|<1$ (VAR, R1, p. 30, 3.3.9). Theo mệnh đề 2 của I, p. 65, ta thu được

(14) log(1 $-a$) $=-\sum_{n=1}^{\infty}\frac{a^n}{n}$.

#### Mệnh đề 12 {#ts-i-s4-prop-12 .statement tag=02AY}

Cho A là một đại số Banach giao hoán có đơn vị. Ảnh của ánh xạ mũ là thành phần liên thông của đơn vị của nhóm G các phần tử khả nghịch của A.

Các công thức (10) và (11) chứng minh rằng exp(A) là một nhóm con của G. Theo điều đi trước (xem công thức (12)), nhóm con này chứa quả cầu mở tâm 1 bán kính 1. Vậy đó là một nhóm con mở, do đó là một nhóm con đóng, của G. Mặt khác, A là liên thông và ánh xạ $a\mapsto$ exp($a$) là liên tục, nên exp(A) là liên thông. Do đó exp(A) là thành phần liên thông của đơn vị của G.

### 11. Các phân hoạch của không gian các đặc trưng

#### Mệnh đề 13 {#ts-i-s4-prop-13 .statement tag=02AZ}

Cho A là một đại số Banach giao hoán có đơn vị. Gọi $U_1$ và $U_2$ là các tập mở của $\mathsf{X}(A)$ lập thành một phân hoạch của $\mathsf{X}(A)$. Khi đó tồn tại duy nhất một phần tử lũy đẳng $j$ của A sao cho biến đổi Gelfand $\mathscr{G}(j)$ bằng 1 trên $U_1$ và bằng 0 trên $U_2$.

Hãy đồng nhất không gian $\mathsf{X}(A)$ với một tập con compắc của $\mathbf{C}^A$ bởi ánh xạ $\chi \mapsto (\chi (a))_{a\in A}($xem No.$^o6$ của I, p. 6 và hệ quả của Định lý 1 của I, p. 29). Các tập con $U_1$ và $U_2$ của không gian đều $\mathbf{C}^A$ là compắc và rời nhau. Theo TG, II, p. 31, Mệnh đề 4, tồn tại một tập con hữu hạn M của A và các tập con mở rời nhau $V_1$ và $V_2$ của $\mathbf{C}^M$ sao cho

$$
p(U_1)\subset V_1,p(U_2)\subset V_2
$$

trong đó $p$ là phép chiếu chính tắc của $\mathbf{C}^A$ lên $\mathbf{C}^M$.

Gọi $a_1, . . . , a_n$ là các phần tử phân biệt của M, và đồng nhất $\mathbf{C}^M$ với $\mathbf{C}^n$. Ta có Sp$^n_A(a_1, . . . , a_n)\subset p(\mathsf{X}(A))\subset V_1\cup V_2$ vì $U_1\cup U_2=\mathsf{X}(A)$. Gọi $f$ là hàm trên $V_1\cup V_2$ bằng 1 trên $V_1$ và bằng 0 trên $V_2$. Ta có $f\in \mathscr{O}(V_1\cup V_2)$. Đặt $j=f(a_1, . . . , a_n)$. Vì $f^2=f$, ta có $j^2=j$. Theo hệ quả 1 của I, p. 66, ta có $\chi (j) = 1$ nếu $\chi \in U_1$ và $\chi (j) = 0$ nếu $\chi \in U_2$, điều này chứng minh sự tồn tại của phần tử lũy đẳng cần tìm.

Hơn nữa, nếu $j_1$ là một phần tử lũy đẳng của A, các hệ thức $j^2=j$ và $j_1^2=j_1$ kéo theo $(j-j_1)(j+j_1-1) = 0$. Nếu $\mathscr{G}(j_1) =\mathscr{G}(j)$, biến đổi Gelfand của $j+j_1-1$ nhận các giá trị trong $\{-1,1\}$, do đó $j+j_1-1$ là khả nghịch (Mệnh đề 6 của I, p. 37), do đó $j=j_1$.

#### Hệ quả {#ts-i-s4-n11-cor-1 .statement tag=02B0}

Cho A là một đại số Banach giao hoán có đơn vị. Các mệnh đề sau là tương đương:

a) Không gian các đặc trưng $\mathsf{X}(A)$ không liên thông;

b) Tồn tại một phần tử lũy đẳng của A khác 0 và 1;

c) Đại số A đẳng cấu với tích của hai đại số Banach khác không.

Mệnh đề chứng minh rằng a) kéo theo b). Nếu $j$ là một phần tử lũy đẳng của A, đặt $I_1=jA$ và $I_2= (1-j)A$. Khi đó $I_1$ và $I_2$ là các iđêan đóng của A, và $I_1+ I_2= A$. Nếu $j \notin  \{0,1\}$, các iđêan $I_1$ và $I_2$ phân biệt với A. Mặt khác, iđêan $I_1$ (resp. $I_2$) là tập hợp các phần tử $x$ của A sao cho $jx=x$ (resp. $(1-j)x=x$), do đó $I_1\cap I_2=\{0\}$. Vì vậy đại số A được đồng nhất với tích $A/I_1\times A/I_2$. Như vậy mệnh đề b) kéo theo c). Cuối cùng, nếu A đẳng cấu với $A_1\times A_2$, không gian $\mathsf{X}(A)$ được đồng nhất với không gian tổng của $\mathsf{X}(A_1)$ và của $\mathsf{X}(A_2)$ (I, p. 6, n$^o6$), do đó c) kéo theo a).

#### Mệnh đề 14 {#ts-i-s4-prop-14 .statement tag=02B1}

Cho A là một đại số Banach giao hoán không có căn. Để A thừa nhận một phần tử đơn vị, điều kiện cần và đủ là $\mathsf{X}(A)$ compắc.

Điều kiện này là cần thiết (I, p. 29, hệ quả). Giả sử $\mathsf{X}(A)$ compắc. Gọi $\widetilde{A}$ là đại số Banach suy ra từ A bằng phép nối thêm một phần tử đơn vị, và đồng nhất $\mathsf{X}'(A)$ với $\mathsf{X}(\widetilde{A})$. Phần bù của $\mathsf{X}(A)$ trong $\mathsf{X}(\widetilde{A})$ thu về đặc trưng $\chi_0$ của $\widetilde{A}$ mà hạt nhân là A. Các tập con $\mathsf{X}(A)$ và $\{\chi_0\}$ là mở trong $\mathsf{X}(\widetilde{A})$. Theo Mệnh đề 13, tồn tại một phần tử $j\in A$ sao cho $\chi (j) = 1$ với mọi $\chi \in \mathsf{X}(A)$, và $\chi_0(j) = 0$. Do đó $j\in A$.

Khi đó, cho $x$ thuộc A. Ta có $\chi (jx) =\chi (x)$ với mọi $\chi \in \mathsf{X}(A)$, do đó $jx=x$ vì A không có căn. Vậy $j$ là một phần tử đơn vị của A.

#### Mệnh đề 15 {#ts-i-s4-prop-15 .statement tag=02B2}

Cho A là một đại số Banach giao hoán, cho $I_1$ là một iđêan của A và $F_1$ là tập hợp các $\chi \in \mathsf{X}(A)$ triệt tiêu trên $I_1$. Gọi $F_2$ là một tập con của $\mathsf{X}(A)$ rời nhau với $F_1$, đóng đối với tôpô Jacobson, và compắc đối với tôpô yếu. Khi đó tồn tại $u\in I_1$ sao cho $\mathscr{G}(u) = 1$ trên $F_2$.

Cho $I_2$ là giao của các hạt nhân của các đặc trưng thuộc $F_2$. Đại số Banach $A/I_2$ là nửa đơn (Mệnh đề 8 của I, p. 38). Vì $F_2$ đóng đối với tôpô Jacobson, các phần tử duy nhất của $\mathsf{X}(A)$ triệt tiêu trên $I_2$ là những phần tử của $F_2($xem I, p. 13). Do đó $F_2$, được trang bị tôpô cảm sinh bởi tôpô yếu của $\mathsf{X}(A)$, được đồng nhất với $\mathsf{X}(A/I_2)$ được trang bị tôpô yếu (I, p. 9, số$^o7$). Vì $F_2$ compắc yếu, đại số $A/I_2$ có một phần tử đơn vị (Mệnh đề 14).

Khi đó có $I_1+ I_2= A$. Nếu không, $(I_1+ I_2)/I_2$ sẽ là một iđêan thực sự, nên được chứa trong hạt nhân của một đặc trưng khác không của $A/I_2($I, p. 30, Định lý 2). Đặc trưng sau sẽ định nghĩa, bằng hợp thành với phép chiếu chính tắc $A\rightarrow A/I_2$, một đặc trưng khác không $\chi$ của A mà sẽ triệt tiêu trên $I_1$ và $I_2$, và do đó sẽ thuộc $F_1\cap F_2$, trái với giả thiết.

Vì $I_1+ I_2= A$, tồn tại $u\in I_1$ mà lớp của nó trong $A/I_2$ là một phần tử đơn vị của $A/I_2$. Khi đó $\chi (u) = 1$ với mọi $\chi \in F_2$, điều này kết thúc chứng minh.

#### Hệ quả {#ts-i-s4-n11-cor-2 .statement tag=02B3}

Cho A là một đại số Banach giao hoán. Cho $F_1$ và $F_2$ là hai tập con rời nhau của $\mathsf{X}(A)$, đóng đối với tôpô Jacobson. Giả sử rằng $F_2$ compắc yếu. Khi đó tồn tại $u\in A$ sao cho $\mathscr{G}(u) = 1$ trên $F_2$ và $\mathscr{G}(u) = 0$ trên $F_1$.

### 12. Các phân hoạch của phổ của một phần tử

Cho A là một đại số Banach có đơn vị, $x\in A$, và K = Sp$_A(x)$. Kí hiệu Π là tập hợp các tập con của K vừa mở vừa đóng trong K. Cho B là đại số con đóng đầy đủ của A sinh bởi $x$; nó là giao hoán.

Với mọi $H\in \Pi$, tồn tại một phần tử duy nhất $f_H$ của $\mathscr{O}(K)$ bằng 1 trong một lân cận của H và bằng 0 trong một lân cận của K - H. Đặt $j_H=f_H(x)$. Phần tử $j_H$ là một lũy đẳng của A, được gọi là liên kết với $x$ và H, và ta có các công thức sau:

$$
j_{H\cap H'}=j_Hj_{H'}=j_{H'}j_H(H,H'\in \Pi ) \tag{15}
$$

$$
j_{H\cup H'}=j_H+j_{H'}-j_{H'}j_H(H,H'\in \Pi ) \tag{16}
$$

$$
j_{\emptyset}= 0,j_K= 1
$$

Cho $H\in \Pi$. Định nghĩa $A_H=j_HAj_H$. Đây là một đại số con đóng của A, nhận phần tử đơn vị $j_H($xem Bổ đề 1 của I, p. 2). Cũng đặt $B_H=j_HBj_H$ và $x_H=xj_H=j_Hx=j_Hxj_H\in B_H$.

Cho $g_H$ là phần tử của $\mathscr{O}(K)$ được định nghĩa bởi $g_H(z) =z$ trong một lân cận của H và $g_H(z) = 0$ trong một lân cận của K - H. Ta có $g_H(z) =f_H(z)z$ trên K, và do đó $x_H=g_H(x)$. Suy ra rằng, nếu $H\not= K$, ta có

Sp$_A(x) =g_H(K) = H\cup  \{0\}$.

Cho $\lambda \in \mathbf{C}-$ H. Gọi $h_{H,\lambda}$ là phần tử của $\mathscr{O}(K)$ bằng $(\lambda -z)^{-1}$ trong một lân cận của H và bằng 0 trong một lân cận của K - H. Ta có $h_{H,\lambda}=f_Hh_{H,\lambda}$ và $(\lambda f_H-g_H)h_{H,\lambda}=f_H$. Nếu ta đặt $R_H(x, \lambda ) =h_{H,\lambda}(x)$, thì $R_H(x, \lambda )\in B_H$ và

$$
R_H(x, \lambda )(\lambda j_H-x_H) = (\lambda j_H-x_H)R_H(x, \lambda ) =j_H \tag{17}
$$

$$
R_H(x, \lambda )j_{K-H}=j_{K-H}R_H(x, \lambda ) = 0
$$

Đặc biệt, $\lambda \in \mathbf{C}-$ Sp$_{A_H}(x_H)$.

Bây giờ cho $\lambda \in H$. Giả sử rằng $\lambda j_H-x_H$ có một nghịch đảo $y$ trong $A_H$. Dùng các công thức $j_Hy=y$ (vì $y\in A_H$) và $j_{K-H}R_{K-H}(x, \lambda ) = R_{K-H}(x, \lambda )$ (vì $R_{K-H}(x, \lambda )\in A_{K-H}$), ta được

$$
(\lambda -x)(y+ R_{K-H}(x, \lambda )) = (\lambda -x)(j_Hy+j_{K-H}R_{K-H}(x, \lambda )) =
$$

$$
(\lambda j_H-xj_H)y+ (\lambda j_{K-H}-xj_{K-H})R_{K-H}(x, \lambda ) =j_H+j_{K-H}= 1
$$

(theo công thức (17) áp dụng cho K - H). Ta kiểm tra một cách tương tự rằng

$$
(y+ R_{K-H}(x, \lambda ))(\lambda -x) = 1
$$

Điều này chứng tỏ rằng $\lambda -x$ có trong A nghịch đảo là $y+ R_{K-H}(x, \lambda )$, điều này vô lý. Vậy ta có $\lambda \in$ Sp$_{A_H}(x_H)$. Do đó ta kết luận rằng

(18) Sp$_{A_H}(x_H) = H$. Đặc biệt, nếu H khác rỗng, thì phần tử lũy đẳng $j_H$ là khác không.

Các công thức (17) và (18) chứng minh rằng hàm $\lambda \mapsto R_H(x, \lambda )$, được xác định trên $\mathbf{C}-$ H, là resolvent của $x_H$ đối với $A_H$.

#### Mệnh đề 16 {#ts-i-s4-prop-16 .statement tag=02B4}

Ta giữ các ký hiệu trước đây. Cho $(H_i)_{1\leqslant i\leqslant n}$ là một phân hoạch của Sp$_A(x)$ thành các phần tử của Π.

a) Đại số B được đồng nhất một cách chính tắc với đại số $B_{H_1}\times \cdots \times B_{H_n}$;

b) Ta có $x_{H_i}x_{H_j}= 0$ với $i\not=j$, và

$$
x=x_{H_1}+x_{H_2}+\cdots +x_{H_n}
$$

c) Ta có

$$
R(x, \lambda ) = R_{H_1}(x, \lambda ) +\cdots + R_{H_n}(x, \lambda ) \tag{19}
$$

với mọi $\lambda \in \mathbf{C}-$ Sp$_A(x)$. Đặc biệt, nếu $H\in \Pi$, resolvent $\lambda \mapsto R(x, \lambda )$ bằng trong một lân cận của H với tổng của $R_H(x, \lambda )$ và một hàm chỉnh hình.

Quan hệ 1 = $j_{H_1}+\cdots +j_{H_n}$ là một phân tích của 1 thành các phần tử lũy đẳng trực giao từng đôi một của B, do đó đại số B được đồng nhất một cách chính tắc với đại số tích $B_{H_1}\times  \cdots  \times B_{H_n}$ (A, I, p. 105, mệnh đề 10).

Mệnh đề b) suy ra từ các quan hệ tương ứng đối với các hàm $g_{H_i}$; mệnh đề c) là một hệ quả của a) và của đẳng thức $R(x_H, \lambda ) = R_H(x, \lambda )$.

#### Mệnh đề 17 {#ts-i-s4-prop-17 .statement tag=02B5}

Cho $\mu$ là một điểm cô lập của Sp$_A(x)$. Khi đó

a) Với mọi $\lambda \in \mathbf{C}-$ Sp$_A(x)$, ta có

$R(x, \lambda ) = R_{\{\mu\}}(x, \lambda ) + R_{Sp_A(x)-\{\mu\}}(x, \lambda )$ ;

b) Hàm gán cho $\lambda$ giá trị $R_{Sp_A(x)-\{\mu\}}(x, \lambda )$ là chỉnh hình trong $\mathbf{C}-$ Sp$_A(x)$ và trong một lân cận của $\mu$; hơn nữa, hàm gán cho $\lambda$ giá trị $R_{\{\mu\}}(x, \lambda )$ là chỉnh hình trong $\mathbf{C}-\{\mu\}$;

c) Ta có

lim$_{n\rightarrow+\infty}\|(x-\mu)^nj_{\{\mu\}}\|^{1/n}= 0$

và, với $\lambda \in \mathbf{C}-\{\mu\}$, công thức

$$
R_{\{\mu\}}(x, \lambda ) =\sum_{n=0}^{\infty}(\lambda -\mu)^{-n-1}(x-\mu)^nj_{\{\mu\}} \tag{20}
$$

Những điều vừa nói kéo theo các khẳng định a) và b). Hãy chứng minh c). Thay thế $x$ bởi $x-\mu$, ta quy về trường hợp $\mu= 0$. Đặt $H =\{0\}$; đây là một tập con mở và đóng của Sp$_A(x)$. Theo công thức (18), phổ của $x_H$ trong $A_H$ là $\{0\}$, do đó $x_H$ là lũy linh giả, nghĩa là $\|x^nj_H\|^{1/n}=\|(xj_H)^n\|^{1/n}$ tiến tới 0 khi $n$ tiến tới $+\infty$. Hơn nữa, với $\lambda \not= 0$, ta có trong $A_H$

$$
(\lambda j_H-x_H)^{-1}=\sum_{n=0}^{\infty}\lambda^{-n-1}x^n_H
$$

(Định lý 1 của I, p. 24, d)), do đó có (20).

#### Hệ quả 1 {#ts-i-s4-prop-17-cor-1 .statement tag=02B6}

Cho $\mu$ là một điểm cô lập của Sp$_A(x)$ và $p$ là một số nguyên dương ngặt. Để $\mu$ là một cực bậc $p$ của giải thức của $x($xem VAR, R1, p. 30, 3.3.9), điều kiện cần và đủ là $(x-\mu)^{p-1}j_{\{\mu\}}\not= 0$ và $(x-\mu)^pj_{\{\mu\}}= 0$.

#### Hệ quả 2 {#ts-i-s4-prop-17-cor-2 .statement tag=02B7}

Cho $\mu$ là một điểm cô lập của Sp$_A(x)$. Cho Γ là biên định hướng của một đĩa mở Δ tâm $\mu$ sao cho

Sp$_A(x)\cap (\Gamma \cup \Delta ) =\{\mu\}$.

Khi đó lũy đẳng $j_{\{\mu\}}$ liên kết với $x$ và $\{\mu\}$ được cho bởi

$$
j_{\{\mu\}}=\frac{1}{2i\pi}\int_{\Gamma}(z-x)^{-1}dz
$$

*Nói cách khác, lũy đẳng $j_{\{\mu\}}$ là thặng dư tại $\mu$ của giải thức của $x.*$

Với $z\in \mathbf{C}-$ Sp$_A(x)$, ta có

$$
(z-u)^{-1}= R(x, z) = R_{\{\mu\}}(x, z) + R_H(x, z)
$$

trong đó H = Sp$_A(x)-\{\mu\}$ (công thức (19)). Hàm $z\mapsto R_H(x, z)$ là chỉnh hình trong $\mathbf{C}-$ H và trong một lân cận của $\{\mu\}$ (Mệnh đề 17, b)), do đó

$$
\frac{1}{2i\pi}\int_{\Gamma}R_H(x, z)dz= 0
$$

(VAR, R2, p. 48, 11.2.5). Hàm $z\mapsto R_{\{\lambda\}}(x, z)$ là giải thức của phần tử $j_{\{\mu\}}xj_{\{\mu\}}$ của đại số có đơn vị $A_{\{\mu\}}$. Khi đó ta có

$$
j_{\{\mu\}}=\frac{1}{2i\pi}\int_{\Gamma}R_{\{\mu\}}(x, z)dz
$$

theo Mệnh đề 9 của I, p. 75 áp dụng cho $A_{\{\mu\}}$ và cho hàm hằng 1 trong một lân cận của $\Delta \cup \Gamma$. Hệ quả được chứng minh.

### 13. Phép tính phiếm hàm chỉnh hình trong một đại số thực hoặc phức khả chuẩn đầy đủ

Cho E là một không gian vectơ tôpô thực. Không gian vectơ tôpô phức hóa $\mathbf{C}\otimes E$ của E (TVS, II, p. 65) được ký hiệu bởi $E_{(\mathbf{C})}$ và E được đồng nhất với một không gian con vectơ tôpô thực của $E_{(\mathbf{C})}$ qua ánh xạ $x\mapsto 1\otimes x$.

#### Mệnh đề 18 {#ts-i-s4-prop-18 .statement tag=02B8}

Không gian vectơ tôpô phức $E_{(\mathbf{C})}$ là khả chuẩn hóa (resp. đầy đủ) khi và chỉ khi E là khả chuẩn hóa (resp. đầy đủ).

Không gian vectơ tôpô thực nền của $E_{(\mathbf{C})}$ đẳng cấu với $E\times E$. Do đó $E_{(\mathbf{C})}$ là đầy đủ khi và chỉ khi E là đầy đủ, và E là khả chuẩn hóa nếu $E_{(\mathbf{C})}$ có tính chất đó.

Ngược lại, giả sử E là khả chuẩn hóa. Cho $p$ là một chuẩn xác định tôpô của E và B là quả cầu đơn vị của $p$. Tồn tại một lân cận cân bằng đóng V của 0 trong $E_{(\mathbf{C})}$ được chứa trong $B +iB$ (TVS, II, p. 66). Do đó các tập hợp $\lambda V$, trong đó $\lambda$ chạy qua $\mathbf{R}^*_+$, tạo thành một hệ lân cận cơ sở của 0 trong $E_{(\mathbf{C})}$. Phiếm hàm Minkowski của V là một chuẩn trên $E_{(\mathbf{C})}$ xác định tôpô của $E_{(\mathbf{C})}$, do đó $E_{(\mathbf{C})}$ là khả chuẩn hóa.

#### Nhận xét {#ts-i-s4-n13-rem-1 .statement tag=02B9}

Cho E và F là các không gian vectơ tôpô khả chuẩn hóa trên K. Không gian vectơ $\mathscr{L}(E; F)$ của các ánh xạ tuyến tính liên tục từ E vào F, được trang bị tôpô hội tụ bị chặn, là một không gian vectơ tôpô khả chuẩn hóa (TVS, III, p. 14).

Cho E và F là các không gian vectơ tôpô khả chuẩn hóa trên $\mathbf{R}$. Ánh xạ $\mathbf{C}$-tuyến tính $\varphi :\mathscr{L}(E; F)_{(\mathbf{C})}\rightarrow \mathscr{L}(E_{(\mathbf{C})}; F_{(\mathbf{C})})$ được xác định bởi $\varphi (\lambda \otimes u) =\lambda u_{(\mathbf{C})}$ là một đẳng cấu của các không gian vectơ tôpô phức. Đặc biệt, đối ngẫu của $E_{(\mathbf{C})}$ được đồng nhất với đối ngẫu phức hóa của E và đại số khả chuẩn hóa $\mathscr{L}(E_{(\mathbf{C})})$ với đại số phức hóa của đại số khả chuẩn hóa $\mathscr{L}(E)$.

Cho S là một tập con compắc của $\mathbf{C}$ ổn định dưới phép liên hợp phức. Xét $\mathbf{C}$-đại số $\mathscr{O}(S)$ của các mầm hàm chỉnh hình nhận giá trị phức trên một lân cận của S, được trang bị cấu trúc không gian lồi địa phương phức xác định trong No. 1 của I, p. 49. Nếu U là một lân cận mở của S trong $\mathbf{C}$, và $h: U\rightarrow \mathbf{C}$ là một hàm chỉnh hình, thì ảnh V của U dưới phép liên hợp phức là một lân cận mở của S trong $\mathbf{C}$ và $h^*:w\mapsto \overline{h(\overline{w})}$ là một hàm chỉnh hình trên V. Chuyển qua giới hạn quy nạp, ta suy ra được một phép đối hợp liên tục $f\mapsto f^*$ trong đại số $\mathscr{O}(S)$. Đặc biệt, ta có:

$$
(f+g)^*=f^*+g^*(f g)^*=f^*g^*(\lambda f)^*=\lambda f^*
$$

với $f, g$ trong $\mathscr{O}(S)$ và $\lambda$ trong $\mathbf{C}$.

Tập hợp các mầm $f\in \mathscr{O}(S)$ sao cho $f=f^*$ được ký hiệu bởi $\mathscr{O}_{\mathbf{R}}(S)$. Đó là một dưới-$\mathbf{R}$-đại số đầy đủ đóng của $\mathscr{O}(S)$.

#### Mệnh đề 19 {#ts-i-s4-prop-19 .statement tag=02BA}

Cho $z$ ký hiệu mầm trong $\mathscr{O}(S)$ của ánh xạ đồng nhất của $\mathbf{C}$. Khi đó $\mathscr{O}_{\mathbf{R}}(S)$ là dưới-$\mathbf{R}$-đại số đầy đủ đóng nhỏ nhất của $\mathscr{O}(S)$ chứa $z$.

Ta có $z^*=z$; do đó $z$ thuộc $\mathscr{O}_{\mathbf{R}}(S)$. Gọi B là một đại số con đầy đủ, đóng trên $\mathbf{R}$ của $\mathscr{O}(S)$ chứa $z$. Ánh xạ $f\mapsto f+f^*$ từ $\mathscr{O}(S)$ vào $\mathscr{O}_{\mathbf{R}}(S)$ là liên tục và toàn ánh, và tập hợp các mầm của các hàm hữu tỉ chỉnh hình trong một lân cận của S là trù mật trong $\mathscr{O}(S)$ (Định lý 3 của I, p. 69). Để chứng minh rằng B chứa $\mathscr{O}_{\mathbf{R}}(S)$, vì vậy chỉ cần chứng minh rằng nếu $f$ là mầm của một hàm hữu tỉ như thế, thì $f+f^*\in B$.

Tồn tại các đa thức P và Q trong $\mathbf{C}[X]$ sao cho Q không triệt tiêu tại điểm nào của S và sao cho ta có $f=\frac{P(z)}{Q(z)}$. Ký hiệu $P^*$ và $Q^*$ là các đa thức thu được bằng cách thay thế các hệ số của P và Q bởi các liên hợp của chúng. Khi đó ta có $P(z)^*= P^*(z)$ và $Q(z)^*= Q^*(z)$. Vì S ổn định đối với phép liên hợp phức, đa thức $Q^*$ không triệt tiêu tại điểm nào của S. Do đó các mầm $Q^*(z)$ và (QQ$^*$)$(z)$ khả nghịch trong $\mathscr{O}(S)$, và

$f+f^*=\frac{P(z)}{Q(z)}+\frac{P^*(z)}{Q^*(z)}=$ (PQ(QQ$^*+ P_*$)$(^*Q)(z)z$).

Vì các đa thức PQ$^*+ P^*Q$ và QQ$^*$ có các hệ số thực và B là một đại số con đầy đủ trên $\mathbf{R}$ của $\mathscr{O}(S)$ chứa $z$, phần tử $f+f^*$ thuộc B. Điều này kết thúc chứng minh của mệnh đề.

Cho A là một đại số chuẩn hóa được, đầy đủ, có đơn vị trên $\mathbf{R}$. Gọi $x$ là một phần tử của A. Phổ của phần tử $1\otimes x$ của đại số $A_{(\mathbf{C})}$ được gọi là phổ phức của $x$, và được ký hiệu bởi Sp$_{A_{(\mathbf{C})}}(x)$. Giao của nó với tập hợp $\mathbf{R}$ chính là phổ Sp$_A(x)$ của $x$ đối với A, phổ này đôi khi được gọi là phổ thực của $x$. Phổ phức Sp$_{A_{(\mathbf{C})}}(x)$ là một tập con compắc của $\mathbf{C}$, ổn định dưới phép liên hợp phức. Nó không rỗng khi đại số A không thu về 0.

Gọi $x$ là một phần tử của A. Bán kính phổ của $1\otimes x\in A_{(\mathbf{C})}$ bằng bán kính phổ $\varrho (x)$ của $x$. Đó là số thực nhỏ nhất $r\geqslant 0$ sao cho $|\lambda |\leqslant r$ với mọi $\lambda \in$ Sp$_{A_{(\mathbf{C})}}(x)$. Ta có

$\varrho (x) =$ lim$_{n\rightarrow+\infty}\|x^n\|^{1/n}=$ inf$_{n>0}\|x^n\|^{1/n}$

đối với mọi chuẩn trên A xác định tôpô của A. Thật vậy, có thể giả sử rằng chuẩn trên A là hạn chế của một chuẩn trên $A_{(\mathbf{C})}$ xác định tôpô của $A_{(\mathbf{C})}$ và áp dụng Prop. 1 của I, p. 20.

Kí hiệu bởi $u\mapsto \overline{u}$ tự đồng cấu của $\mathbf{R}$-đại số $A_{(\mathbf{C})}$ biến $\lambda \otimes a$ thành $\overline{\lambda}\otimes a$. Nó liên tục.

#### Bổ đề {#ts-i-s4-n13-lem-1 .statement tag=02BB}

Với mọi $f\in \mathscr{O}$(Sp$_{A_{(\mathbf{C})}}(x)$), ta có $f^*(1\otimes x) =\overline{f(1 \otimes x)}$.

Các ánh xạ $f\mapsto f(1\otimes x)$ và $f\mapsto \overline{f^*(1 \otimes x)}$ là các đồng cấu có đơn vị liên tục của các $\mathbf{C}$-đại số từ $\mathscr{O}$(Sp($x$)) vào $A_{(\mathbf{C})}$ biến $z$ thành $1\otimes x$; do đó chúng bằng nhau (I, p. 74, đl. 5).

#### Mệnh đề 20 {#ts-i-s4-prop-20 .statement tag=02BC}

Với mọi $f\in \mathscr{O}_{\mathbf{R}}$(Sp$_{A_{(\mathbf{C})}}(x)$), tồn tại một phần tử duy nhất $f(x)$ của A sao cho $f(1\otimes x) = 1\otimes f(x)$ trong $A_{(\mathbf{C})}$. Ánh xạ $f\mapsto f(x)$ từ $\mathscr{O}_{\mathbf{R}}$(Sp$_{A_{(\mathbf{C})}}(x)$) vào A là đồng cấu có đơn vị liên tục duy nhất của các $\mathbf{R}$-đại số biến mầm trong $\mathscr{O}_{\mathbf{R}}$(Sp$_{A_{(\mathbf{C})}}(x)$) của ánh xạ đồng nhất của $\mathbf{C}$ thành $x$.

Đặt S = Sp$_{A_{(\mathbf{C})}}(x)$. Theo bổ đề trên, với mọi mầm $f\in \mathscr{O}_{\mathbf{R}}$(Sp($x$)), ta có $f(1\otimes x) =\overline{f(1 \otimes x)}$. Khẳng định thứ nhất suy ra từ đó. Kí hiệu bởi $z$ mầm trong $\mathscr{O}_{\mathbf{R}}(S)$ của ánh xạ đồng nhất của $\mathbf{C}$. Ánh xạ $f\mapsto f(x)$ là một đồng cấu có đơn vị liên tục của $\mathbf{R}$-đại số $\mathscr{O}_{\mathbf{R}}$(Sp($x$)) vào A, biến $z$ thành $x$. Nó là ánh xạ duy nhất như vậy theo mệnh đề 19, vì mọi cấu xạ có các tính chất ấy đều được xác định duy nhất trên mọi đại số con-$\mathbf{R}$ đầy đủ đóng của $\mathscr{O}(S)$ chứa $z$.

Cho $f\in \mathscr{O}_{\mathbf{R}}$(Sp$_{A_{(\mathbf{C})}}(x)$). Phần tử $f(x)$ thuộc mọi đại số con đầy đủ đóng của A chứa $x$ (mệnh đề 19), và do đó thuộc đối giao hoán tử kép của $x$ trong A. Phổ phức của $f(x)$ bằng $f$(Sp($x$)) (I, p. 75, mệnh đề 8). Với mọi $g\in \mathscr{O}_{\mathbf{R}}(f$(Sp$_{A_{(\mathbf{C})}}(x)$)), ta có $g\circ f\in \mathscr{O}_{\mathbf{R}}$(Sp$_{A_{(\mathbf{C})}}(x)$) và (loc. cit.) $(g\circ f)(x) =g(f(x))$.

Cho U là một tập con mở của $\mathbf{C}$, ổn định đối với phép liên hợp phức. Tập Ω các phần tử $x$ của A mà phổ phức được chứa trong U là mở trong A (I, p. 76, Mệnh đề 10). Cho $f$ là một hàm chỉnh hình trên U sao cho $f^*=f$. Ánh xạ $x\mapsto f(x)$ từ Ω vào A là giải tích (loc. cit.).

Cho A, B là các đại số kết hợp có đơn vị, khả chuẩn và đầy đủ trên $\mathbf{R}$ và cho $\varphi : A\rightarrow$ B là một cấu xạ đại số có đơn vị liên tục. Cho $x\in A$. Phổ phức của $\varphi (x)$ được chứa trong phổ phức của $x$ và, với mọi $f\in \mathscr{O}_{\mathbf{R}}$(Sp$_{A_{(\mathbf{C})}}(x)$), ta có $f(\varphi (x)) =\varphi (f(x))$. Điều này suy ra ngay từ mệnh đề tương tự trong trường hợp phức (I, p. 75, Mệnh đề 8).

### 14. Trường hợp một Đại số không có Phần tử đơn vị

Cho A là một đại số khả chuẩn và đầy đủ, không nhất thiết có đơn vị, trên $K =\mathbf{R}$ hoặc $\mathbf{C}$. Ký hiệu $(\widetilde{A}, e)$ là đại số có đơn vị thu được từ A bằng phép nối một phần tử đơn vị. Nó là khả chuẩn và đầy đủ.

Cho $x$ là một phần tử của A. Nếu $K =\mathbf{C}$, đặt Sp$'(x) =$ Sp$_{\widetilde{A}}(x)$ là phổ của $x$ đối với $\widetilde{A}$, và xét một mầm $f\in \mathscr{O}$(Sp$'(x)$). Nếu $K =\mathbf{R}$, ký hiệu Sp$'(x)$ là phổ phức của phần tử $x$ của $\widetilde{A}$, và xét một mầm $f\in \mathscr{O}_{\mathbf{R}}$(Sp$'(x)$). Trong cả hai trường hợp, 0 thuộc Sp$'(x)$, và phần tử $f(x)$ của $\widetilde{A}$ thuộc A khi và chỉ khi $f$ thỏa mãn $f(0) = 0$. Thật vậy, phép chiếu $\pi :\widetilde{A}\rightarrow Ke$ là một cấu xạ liên tục có hạt nhân là A, và ta có $\pi (f(x)) =f(\pi (x)) =f(0)$.

## BÀI TẬP {#ts-i-s4-exercises}

Trong các bài tập dưới đây, mọi đại số được xét đều là trên $\mathbf{C}$, trừ khi có nói rõ ngược lại.

Xem [các bài tập cho § 4](exercises/s4/).
