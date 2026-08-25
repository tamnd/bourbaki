---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Semisimple Modules and Rings
section: 11
section_title: Grothendieck Groups
lang: vi
source: alg-viii
source_edition: 2023, Springer Nature
book_pages: A VIII.183-A VIII.210
pdf_pages: 0200-0227
extraction: native+ocr
subsections:
    - "no": 1
      title: Additive Functions of Modules
      page: 183
      pdf_page: 200
    - "no": 2
      title: The Grothendieck Group of an Additive Set of Modules
      page: 186
      pdf_page: 203
    - "no": 3
      title: Using Composition Series
      page: 189
      pdf_page: 206
    - "no": 4
      title: The Grothendieck Group R(A)
      page: 191
      pdf_page: 208
    - "no": 5
      title: Change of Rings
      page: 193
      pdf_page: 210
    - "no": 6
      title: The Grothendieck Group $R_K(A)$
      page: 194
      pdf_page: 211
    - "no": 7
      title: Multiplicative Structure on $K(\mathscr{C})$
      page: 196
      pdf_page: 213
    - "no": 8
      title: The Grothendieck Group $K_0(A)$
      page: 199
      pdf_page: 216
    - "no": 9
      title: The Grothendieck Group $K_0(A)$ of an Artinian Ring
      page: 200
      pdf_page: 217
    - "no": 10
      title: Change of Rings for $ K_0(A) $
      page: 201
      pdf_page: 218
    - "no": 11
      title: Frobenius Reciprocity
      page: 202
      pdf_page: 219
    - "no": 12
      title: The Case of Simple Rings
      page: 204
      pdf_page: 221
statements: 38
exercises: 14
content_sha256: e670b54db4eb209beb747325fb4305a2019770f82d473cfe419dbf8c4eda69d3
translated_from: content/en/alg/VIII/11_s11_grothendieck_groups.md
source_content_sha256: 097072a6252a31b52549d811e4b46eabb649dfcf3a7e8686d51686c1374532a2
translation_model: gpt-5-6-mini
translation_run: translate-vi-265764f6
glossary_version: 34
glossary_terms_sha256: 8fb784226be024d20dd1c24158428831cffdc036e867a26208ec05555731720f
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 11. CÁC NHÓM GROTHENDIECK

### 1. Các hàm cộng tính của môđun

Cho A là một vành, và cho $\mathscr{C}$ là một tập hợp các lớp của các A-môđun (VIII, p. 51); ta nói rằng một A-môđun là có kiểu $\mathscr{C}$ nếu lớp của nó thuộc $\mathscr{C}$.

#### Định nghĩa 1 {#alg-viii-s11-def-1 .statement tag=00CS}

Ta nói rằng tập hợp $\mathscr{C}$ các lớp của các A-môđun là cộng tính nếu mọi môđun không là có kiểu $\mathscr{C}$ và tổng trực tiếp của hai môđun có kiểu $\mathscr{C}$ là có kiểu $\mathscr{C}$. Ta nói rằng $\mathscr{C}$ là di truyền nếu nó là cộng tính và các môđun con và các môđun thương của một môđun có kiểu $\mathscr{C}$ đều có kiểu $\mathscr{C}$.

#### Ví dụ 1 {#alg-viii-s11-n1-exa-1 .statement tag=00CT}

Tập hợp các lớp của các A-môđun có độ dài hữu hạn là di truyền (II, §1, No. 10, p. 212, Mệnh đề 16).

#### Ví dụ 2 {#alg-viii-s11-n1-exa-2 .statement tag=00CU}

Tập hợp các lớp của các A-môđun sinh hữu hạn là cộng tính. Nếu vành A là Noether, thì tập hợp này là di truyền (VIII, p. 3, Mệnh đề 3 và VIII, p. 7, Mệnh đề 4).

#### Ví dụ 3 {#alg-viii-s11-n1-exa-3 .statement tag=00CV}

Tập hợp các lớp của các A-môđun xạ ảnh sinh hữu hạn là cộng tính nhưng nói chung không di truyền.

#### Định nghĩa 2 {#alg-viii-s11-def-2 .statement tag=00CW}

Cho $\varphi$ là một ánh xạ từ $\mathscr{C}$ vào một nhóm Abel G (được viết theo phép cộng); đặt $\varphi (E) =\varphi$(cl(E)) với mọi A-môđun E có kiểu $\mathscr{C}$. Ta nói rằng $\varphi$ là một hàm cộng tính của môđun (tương ứng, một hàm cộng tính yếu của môđun) nếu ta có $\varphi (E) =\varphi (E') +\varphi (E'')$ đối với mọi dãy khớp (tương ứng, đối với mọi dãy khớp tách)

$$
0\longrightarrow E'\longrightarrow E\longrightarrow E''\longrightarrow 0
$$

của các môđun có kiểu $\mathscr{C}$.

#### Ví dụ 4 {#alg-viii-s11-n1-exa-4 .statement tag=00CX}

Cho $ \mathcal{C} $ là tập hợp các lớp của các A-môđun có độ dài hữu hạn. Ánh xạ $ \operatorname{long}_A : \mathcal{C} \to \mathbf{Z} $ gửi một lớp của các A-môđun có độ dài hữu hạn vào độ dài của nó là một hàm cộng tính của môđun (II, §1, No. 10, p. 213, Hệ quả 3). Các kết quả của tiểu mục này là một phép tổng quát hóa của các kết quả về các môđun có độ dài hữu hạn được thiết lập trong II, §1, No. 10, p. 212–214.

Trong phần còn lại của tiểu mục này, ta xét một tập hợp cộng tính $ \mathcal{C} $ các A-môđun và một ánh xạ cộng tính $ \varphi $ từ $ \mathcal{C} $ vào một nhóm Abel $ G $.

Cho E và $ E' $ là các môđun có kiểu $ \mathcal{C} $; khi đó $ E \oplus E' $ có kiểu $ \mathcal{C} $, và tồn tại một dãy khớp tách (II, §1, No. 9, p. 210)

$$
0 \longrightarrow E \longrightarrow E \oplus E' \longrightarrow E' \longrightarrow 0;
$$

từ đó, ta suy ra

(1)
$$
\varphi(E \oplus E') = \varphi(E) + \varphi(E').
$$

Đặc biệt, ta có $ \varphi(0) = 0 $.

#### Mệnh đề 1 {#alg-viii-s11-prop-1 .statement tag=00CY}

Giả sử rằng $ \mathcal{C} $ là di truyền. Cho E và F là các A-môđun và $ u : E \to F $ là một ánh xạ tuyến tính.
a) Nếu E hoặc F có kiểu $ \mathcal{C} $, thì ảnh của u cũng có kiểu đó.
b) Nếu E có kiểu $ \mathcal{C} $, thì hạt nhân của u cũng có kiểu đó, và ta có

(2)
$$
\varphi(E) = \varphi(\operatorname{Ker}\,u) + \varphi(\operatorname{Im}\,u).
$$

c) Nếu F có kiểu $ \mathcal{C} $, thì đối hạt nhân của u cũng có kiểu đó, và ta có

(3)
$$
\varphi(F) = \varphi(\operatorname{Im}\,u) + \varphi(\operatorname{Coker}\,u).
$$

Mệnh đề suy ra từ sự tồn tại của các dãy khớp

$$
0 \longrightarrow \operatorname{Ker}\,u \longrightarrow E \longrightarrow \operatorname{Im}\,u \longrightarrow 0,
$$
$$
0 \longrightarrow \operatorname{Im}\,u \longrightarrow F \longrightarrow \operatorname{Coker}\,u \longrightarrow 0.
$$

#### Hệ quả {#alg-viii-s11-n1-cor-1 .statement tag=00CZ}

Cho $ (E_i)_{0 \leq i \leq n} $ là một dãy hữu hạn các môđun có kiểu $ \mathcal{C} $. Nếu tồn tại một dãy khớp

$$
0 \longrightarrow E_0 \xrightarrow{u_0} E_1 \xrightarrow{u_1} \cdots \xrightarrow{u_{n-1}} E_{n-1} \xrightarrow{u_n} E_n \longrightarrow 0,
$$

thì ta có

(4)
$$
\sum_{i=0}^n (-1)^i \varphi(E_i) = 0.
$$

Ta chứng minh hệ quả bằng quy nạp theo $n$; các trường hợp $n= 0$ và $n= 1$ là tầm thường. Vậy cho $n\geqslant 1$, và cho

$$
0\longrightarrow E_0\longrightarrow^{u_0}E_1\longrightarrow  \cdots  \longrightarrow^{u_1}E_{n-1}\longrightarrow^{u_{n-1}}E_n\overset{u}{-}-\rightarrow^{^n}E_{n+1}\longrightarrow 0
$$

là một dãy khớp các môđun có kiểu $\mathscr{C}$. Theo Mệnh đề 1, hạt nhân F của $u_n$ là một môđun có kiểu $\mathscr{C}$, và ta có

$$
\varphi (F) =\varphi (E_n)-\varphi (E_{n+1}) \tag{5}
$$

Hơn nữa, ta có một dãy khớp

$$
0\longrightarrow E_0\longrightarrow E_1\longrightarrow E_2\longrightarrow  \cdots  \longrightarrow E_{n-1}\longrightarrow F\longrightarrow 0
$$

và giả thiết quy nạp cho quan hệ

$$
\sum^{n-1}_{i=0}(-1)^i\varphi (E_i) + (-1)^n\varphi (F) = 0 \tag{6}
$$

Từ (5) và (6) ta ngay lập tức suy ra rằng $\sum^{n+1}_{i=0}(-1)^i\varphi (E_i) = 0$, và hệ quả được chứng minh.

#### Mệnh đề 2 {#alg-viii-s11-prop-2 .statement tag=00D0}

Giả sử rằng tập hợp $\mathscr{C}$ là di truyền. Cho E là một A-môđun, và cho M và N là các môđun con của E.

a) Nếu các môđun M và N có kiểu $\mathscr{C}$, thì các môđun $M\cap N$ và M + N cũng có kiểu đó, và ta có

$$
\varphi (M + N) +\varphi (M\cap N) =\varphi (M) +\varphi (N)
$$

b) Nếu các môđun $E/M$ và $E/N$ có kiểu $\mathscr{C}$, thì các môđun $E/(M\cap N)$ và $E/(M + N)$ cũng có kiểu $\mathscr{C}$, và ta có

$$
\varphi (E/(M + N)) +\varphi (E/(M\cap N)) =\varphi (E/M) +\varphi (E/N)
$$

Các khẳng định a) và b) suy ra từ sự tồn tại của các dãy khớp

$$
0\rightarrow M\cap N\rightarrow M\oplus N\rightarrow M + N\rightarrow 0
$$

và

$$
0\rightarrow E/(M\cap N)\rightarrow (E/M)\oplus (E/N)\rightarrow E/(M + N)\rightarrow 0
$$

(II, §1, No. 7, p. 207, Mệnh đề 10).

#### Mệnh đề 3 {#alg-viii-s11-prop-3 .statement tag=00D1}

Giả sử rằng $\mathscr{C}$ là di truyền. Cho E là một môđun có kiểu $\mathscr{C}$ và $(E_i)_{0\leqslant i\leqslant n}$ là một chuỗi hợp thành của E (I, §4, No. 7, p. 41). Với $1\leqslant i\leqslant n$, môđun $E_{i-1}/E_i$ có kiểu $\mathscr{C}$, và ta có

$$
\varphi (E) =\sum_{i=1}^n\varphi (E_{i-1}/E_i)
$$

Vì $\mathscr{C}$ là di truyền, các môđun $E_0/E_1$ và $E_1$ có kiểu $\mathscr{C}$, và ta có $\varphi (E) =\varphi (E_0/E_1) +\varphi (E_1)$. Vì dãy $(E_{i+1})_{0\leqslant i\leqslant n-1}$ là một chuỗi hợp thành của $E_1$, Mệnh đề 3 suy ra bằng quy nạp theo $n$.

### 2. Nhóm Grothendieck của một tập hợp cộng tính các môđun

Cho A là một vành. Trong tiểu mục này, ta xét một tập hợp cộng tính $\mathscr{C}$ gồm các lớp của các A-môđun; ta đồng nhất $\mathscr{C}$ với cơ sở chính tắc của nhóm Abel tự do $\mathbf{Z}^{(\mathscr{C})}$. Với mọi dãy khớp

$$
(\mathscr{E})0\longrightarrow E'\longrightarrow E\longrightarrow E''\longrightarrow 0
$$

của các môđun có kiểu $\mathscr{C}$, ta ký hiệu bởi $r_{\mathscr{E}}$ phần tử cl(E) $-$ cl(E$'$)$-$ cl(E$''$) của $\mathbf{Z}^{(\mathscr{C})}$. Cho R là nhóm con của $\mathbf{Z}^{(\mathscr{C})}$ sinh bởi các phần tử có dạng $r_{\mathscr{E}}$; nhóm thương $\mathbf{Z}^{(\mathscr{C})}/R$ được gọi là nhóm Grothendieck của $\mathscr{C}$ và được ký hiệu bởi $K(\mathscr{C})$. Với một môđun E có kiểu $\mathscr{C}$, ta ký hiệu ảnh của cl(E) trong $K(\mathscr{C})$ bởi $[E]_{\mathscr{C}}$ (hoặc đôi khi [E] khi có sự nhập nhằng về $\mathscr{C}$). Khi đó ta có tính chất phổ quát sau.

#### Mệnh đề 4 {#alg-viii-s11-prop-4 .statement tag=00D2}

a) Ánh xạ $E\mapsto [E]_{\mathscr{C}}$ từ $\mathscr{C}$ vào $K(\mathscr{C})$ là cộng tính.

b) Cho G là một nhóm Abel, và cho $\varphi :\mathscr{C}\rightarrow G$ là một hàm cộng tính của các môđun. Tồn tại một đồng cấu duy nhất $u: K(\mathscr{C})\rightarrow G$ sao cho ta có $\varphi (E) =u([E]_{\mathscr{C}})$ với mọi môđun E có kiểu $\mathscr{C}$.

Mệnh đề a) là hiển nhiên. Ta hãy chứng minh b). Có một đồng cấu $u':\mathbf{Z}^{(\mathscr{C})}\rightarrow G$ mở rộng $\varphi$. Vì $\varphi$ là cộng tính, ta có $u'(r_{\mathscr{E}}) = 0$ đối với mọi dãy khớp $(\mathscr{E})$ của các môđun kiểu $\mathscr{C}$; do đó, R được chứa trong hạt nhân của $u'$. Do đó, khi chuyển qua thương, $u'$ xác định một đồng cấu $u$ từ $K(\mathscr{C})$ đến G, và rõ ràng ta có $\varphi (E) =u([E]_{\mathscr{C}})$ đối với mọi A-môđun kiểu $\mathscr{C}$. Nhóm $K(\mathscr{C})$ được sinh bởi tập hợp các phần tử $[E]_{\mathscr{C}}$ với E chạy qua $\mathscr{C}$; tính duy nhất của $u$ được suy ra.

Cho $\mathscr{C}$ và $\mathscr{D}$ là các tập hợp cộng tính của các lớp A-môđun sao cho $\mathscr{C}\subset \mathscr{D}$. Vì ánh xạ $E\mapsto [E]_{\mathscr{D}}$ từn$\mathscr{C}$ đến nhóm GrothendiecknK($\mathscr{D}$) là cộng tính, tồn tại một đồng cấu $\gamma_{\mathscr{D},\mathscr{C}}: K(\mathscr{C})\rightarrow K(\mathscr{D})$, gọi là chính tắc, được đặc trưng bởi công thức $\gamma_{\mathscr{D},\mathscr{C}}([E]_{\mathscr{C}}) = [E]_{\mathscr{D}}$ đối với mọi môđun E kiểu $\mathscr{C}$. Nó không phải lúc nào cũng đơn ánh (VIII, p. 210, Bài tập 13).

#### Ví dụ {#alg-viii-s11-n2-exa-1 .statement tag=00D3}

$*$ Cho A là một vành Noether giao hoán, và cho Σ là phổ của nó. Với mọi số nguyên $n\geqslant 0$, ký hiệu $\mathscr{C}^{\geqslant n}$ là tập hợp các lớp của các A-môđun sinh hữu hạn có giá với đối chiều $\geqslant n$ trong Σ. Đặt $K(n,A) =$ $K(\mathscr{C}^{\geqslant n})$ và $\gamma_n=\gamma_{\mathscr{C}^{\geqslant n},\mathscr{C}^{\geqslant n+1}}$. Ta có một dãy các đồng cấu

$$
\gamma_n: K(n+ 1,A)\longrightarrow K(n,A)
$$

Ta có thể chứng minh (AC, VIII, §1, n$^o5$, p. 13, mệnh đề 10) rằng trong $K(n,A)$, các phần tử $[A/\mathfrak{p}]_{\mathscr{C}_n}$, trong đó $\mathfrak{p}$ chạy qua tập hợp các phần tử của Σ có chiều cao $n$, tạo thành một cơ sở của một $\mathbf{Z}$-môđun phụ cho ảnh của $\gamma_n$. Chính xác hơn, đối với mọi môđun E kiểu $\mathscr{C}^{\geqslant n}$, ta có

$[E]_{\mathscr{C}^{\geqslant n}}\equiv \sum$ long$_{A_{\mathfrak{p}}}(E_{\mathfrak{p}})\cdot [A/\mathfrak{p}]_{\mathscr{C}^{\geqslant n}}$ (mod Im $\gamma_n$)$.*$

$\{\mathfrak{p}\in \Sigma |$ht($\mathfrak{p}$)$=n\}$

Nhóm $K(\mathscr{C})$ được sinh bởi các phần tử có dạng $[E]_{\mathscr{C}}$ với $E\in \mathscr{C}$, và ta có $[E\oplus E']_{\mathscr{C}}= [E]_{\mathscr{C}}+ [E']_{\mathscr{C}}$ theo quan hệ (1) (VIII, p. 184). Mọi phần tử của $K(\mathscr{C})$ do đó có dạng $[E]_{\mathscr{C}}-[F]_{\mathscr{C}}$, trong đó E và F thuộc về $\mathscr{C}$.

Một phần tử của $K(\mathscr{C})$ được gọi là hiệu dụng nếu nó có dạng $[E]_{\mathscr{C}}$ với một A-môđun E có kiểu $\mathscr{C}$. Tập hợp các phần tử hiệu dụng của $K(\mathscr{C})$ được ký hiệu bởi $K(\mathscr{C})^+$; nó là một monoid con của $K(\mathscr{C})$, và $K(\mathscr{C})$ có thể được đồng nhất với nhóm các hiệu của $K(\mathscr{C})^+$ (I, §2, No. 4, p. 20).

#### Mệnh đề 5 {#alg-viii-s11-prop-5 .statement tag=00D4}

Cho E và F là các môđun có kiểu $\mathscr{C}$. Đẳng thức $[E]_{\mathscr{C}}= [F]_{\mathscr{C}}$ đúng khi và chỉ khi tồn tại các dãy khớp của các môđun có kiểu $\mathscr{C}$

$$
(\mathscr{E})0\longrightarrow L\longrightarrow P\longrightarrow M\longrightarrow 0
$$

$$
(\mathscr{F})0\longrightarrow L\longrightarrow Q\longrightarrow M\longrightarrow 0
$$

sao cho $E\oplus Q$ đẳng cấu với $F\oplus P$.

Điều kiện đã nêu là đủ vì nó kéo theo các quan hệ

$$
[P]_{\mathscr{C}}= [L]_{\mathscr{C}}+[M]_{\mathscr{C}},[Q]_{\mathscr{C}}= [L]_{\mathscr{C}}+[M]_{\mathscr{C}},[E]_{\mathscr{C}}+[Q]_{\mathscr{C}}= [F]_{\mathscr{C}}+[P]_{\mathscr{C}}
$$

suy ra $[E]_{\mathscr{C}}= [F]_{\mathscr{C}}$.

Bây giờ giả sử rằng ta có $[E]_{\mathscr{C}}= [F]_{\mathscr{C}}$. Theo phép dựng nhóm $K(\mathscr{C})$, tồn tại hai họ hữu hạn các dãy khớp của các môđun có kiểu $\mathscr{C}$

$$
(\mathscr{G}_i)0\longrightarrow G'_i\longrightarrow G_i\longrightarrow G''_i\longrightarrow 0
$$

với $i\in I$ và

$$
(\mathscr{H}_j)0\longrightarrow H'_j\longrightarrow H_j\longrightarrow H''_j\longrightarrow 0
$$

với $j\in J$ sao cho trong $\mathbf{Z}^{(\mathscr{C})}$, ta có

cl(E) $-$ cl(F) $=\sum_{j\in J}r_{\mathscr{H}_j}-\sum_{i\in I}r_{\mathscr{G}_i}$.

Tường minh hơn, quan hệ này có thể được viết dưới dạng

(7) cl(E) $+\sum_{i\in I}$ cl(G$_i$) $+\sum_{j\in J}$ cl(H$'_j$) $+\sum_{j\in J}$ cl(H$''_j$)

= cl(F) $+\sum_{i\in I}$ cl(G$'_i$) $+\sum_{i\in I}$ cl(G$''_i$) $+\sum_{j\in J}$ cl(H$_j$).

Đặt $G =\bigoplus_{i\in I}G_i, G'=\bigoplus_{i\in I}G'_i$, v.v. Bằng cách chuyển qua các tổng trực tiếp, ta thu được các dãy khớp

$(\mathscr{G})$ 0 // ${G'}^p$ // G $^q$ // $G''$ // $0$,

$(\mathscr{H})$ 0 // ${H'}^r$ // H $^s$ // $H''$ // 0

gồm các môđun có kiểu $\mathscr{C}$.
