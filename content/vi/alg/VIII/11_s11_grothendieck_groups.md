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
      title: Change of Rings for $K_0(A)$
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
content_sha256: d19341c75ff92cb1174fa888cdecab2e1d604828252791313c11ae9009090461
translated_from: content/en/alg/VIII/11_s11_grothendieck_groups.md
source_content_sha256: bc6f23569d66726f9edb899a7ea492701ad1b2a6d43e816e11728c34011d5e59
translation_model: gpt-5-6, gpt-5-6-mini, gpt-5.4-mini
translation_run: translate-vi-265764f6
glossary_version: 34
glossary_terms_sha256: 8fb784226be024d20dd1c24158428831cffdc036e867a26208ec05555731720f
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 11. CÁC NHÓM GROTHENDIECK

### 1. Các hàm cộng tính của môđun

Cho A là một vành, và $\mathscr{C}$ là một tập hợp các lớp của A-môđun (VIII, p. 51); ta nói rằng một A-môđun có kiểu $\mathscr{C}$ nếu lớp của nó thuộc $\mathscr{C}$.

#### Định nghĩa 1 {#alg-viii-s11-def-1 .statement tag=00CS}

Ta nói rằng tập hợp $\mathscr{C}$ các lớp của A-môđun là cộng tính nếu mọi môđun không đều là kiểu $\mathscr{C}$ và tổng trực tiếp của hai môđun có kiểu $\mathscr{C}$ cũng có kiểu $\mathscr{C}$. Ta nói rằng $\mathscr{C}$ là di truyền nếu nó cộng tính và các môđun con và các môđun thương của một môđun có kiểu $\mathscr{C}$ đều có kiểu $\mathscr{C}$.

#### Ví dụ 1 {#alg-viii-s11-n1-exa-1 .statement tag=00CT}

Tập hợp các lớp của các A-môđun có độ dài hữu hạn là di truyền (II, §1, No. 10, p. 212, Mệnh đề 16).

#### Ví dụ 2 {#alg-viii-s11-n1-exa-2 .statement tag=00CU}

Tập hợp các lớp của các A-môđun sinh hữu hạn là cộng tính. Nếu vành A là Noether, thì tập hợp này là di truyền (VIII, p. 3, Mệnh đề 3 và VIII, p. 7, Mệnh đề 4).

#### Ví dụ 3 {#alg-viii-s11-n1-exa-3 .statement tag=00CV}

Tập hợp các lớp của các A-môđun xạ ảnh sinh hữu hạn là cộng tính nhưng nói chung không di truyền.

#### Định nghĩa 2 {#alg-viii-s11-def-2 .statement tag=00CW}

Cho $\varphi$ là một ánh xạ từ $\mathscr{C}$ vào một nhóm Abel G (viết theo phép cộng); đặt $\varphi (E) =\varphi$(cl(E)) với mọi A-môđun E có kiểu $\mathscr{C}$. Ta nói rằng $\varphi$ là một hàm cộng tính của môđun (resp. một hàm cộng tính yếu của môđun) nếu ta có $\varphi (E) =\varphi (E') +\varphi (E'')$ với mọi dãy khớp (resp. với mọi dãy khớp tách)

$$
0\longrightarrow E'\longrightarrow E\longrightarrow E''\longrightarrow 0
$$

của các môđun có kiểu $\mathscr{C}$.

#### Ví dụ 4 {#alg-viii-s11-n1-exa-4 .statement tag=00CX}

Cho $\mathcal{C}$ là tập hợp các lớp của các A-môđun có độ dài hữu hạn. Ánh xạ $\operatorname{long}_A : \mathcal{C} \to \mathbf{Z}$ gửi một lớp của các A-môđun có độ dài hữu hạn vào độ dài của nó là một hàm cộng tính của môđun (II, §1, No. 10, p. 213, Hệ quả 3). Các kết quả của tiểu mục này là một phép tổng quát hóa các kết quả về các môđun có độ dài hữu hạn được thiết lập trong II, §1, No. 10, p. 212–214.

Trong phần còn lại của tiểu mục này, ta xét một tập hợp cộng tính $\mathcal{C}$ của các A-môđun và một ánh xạ cộng tính $\varphi$ từ $\mathcal{C}$ vào một nhóm Abel $G$.

Cho E và $E'$ là các môđun có kiểu $\mathcal{C}$; khi đó $E \oplus E'$ có kiểu $\mathcal{C}$, và tồn tại một dãy khớp tách (II, §1, No. 9, p. 210)

$$
0 \longrightarrow E \longrightarrow E \oplus E' \longrightarrow E' \longrightarrow 0;
$$

từ đó, ta suy ra

(1)
$$
\varphi(E \oplus E') = \varphi(E) + \varphi(E').
$$

Đặc biệt, ta có $\varphi(0) = 0$.

#### Mệnh đề 1 {#alg-viii-s11-prop-1 .statement tag=00CY}

Giả sử $\mathcal{C}$ là di truyền. Cho E và F là các A-môđun và $u : E \to F$ là một ánh xạ tuyến tính.
a) Nếu E hoặc F có kiểu $\mathcal{C}$, thì ảnh của u cũng vậy.
b) Nếu E có kiểu $\mathcal{C}$, thì hạt nhân của u cũng vậy, và ta có

(2)
$$
\varphi(E) = \varphi(\operatorname{Ker}\,u) + \varphi(\operatorname{Im}\,u).
$$

c) Nếu F có kiểu $\mathcal{C}$, thì đối hạt nhân của u cũng vậy, và ta có

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

Cho $(E_i)_{0 \leq i \leq n}$ là một dãy hữu hạn các môđun có kiểu $\mathcal{C}$. Nếu tồn tại một dãy khớp

$$
0 \longrightarrow E_0 \xrightarrow{u_0} E_1 \xrightarrow{u_1} \cdots \xrightarrow{u_{n-1}} E_{n-1} \xrightarrow{u_n} E_n \longrightarrow 0,
$$

thì ta có

(4)
$$
\sum_{i=0}^n (-1)^i \varphi(E_i) = 0.
$$

Ta chứng minh hệ quả bằng quy nạp theo $n$; các trường hợp $n= 0$ và $n= 1$ là tầm thường. Vậy cho $n\geqslant 1$, và xét

$$
0\longrightarrow E_0\longrightarrow^{u_0}E_1\longrightarrow  \cdots  \longrightarrow^{u_1}E_{n-1}\longrightarrow^{u_{n-1}}E_n\overset{u}{-}-\rightarrow^{^n}E_{n+1}\longrightarrow 0
$$

là một dãy khớp của các môđun có kiểu $\mathscr{C}$. Theo Mệnh đề 1, hạt nhân F của $u_n$ là một môđun có kiểu $\mathscr{C}$, và ta có

$$
\varphi (F) =\varphi (E_n)-\varphi (E_{n+1}) \tag{5}
$$

Hơn nữa, ta có một dãy khớp

$$
0\longrightarrow E_0\longrightarrow E_1\longrightarrow E_2\longrightarrow  \cdots  \longrightarrow E_{n-1}\longrightarrow F\longrightarrow 0
$$

và giả thiết quy nạp cho ta quan hệ

$$
\sum^{n-1}_{i=0}(-1)^i\varphi (E_i) + (-1)^n\varphi (F) = 0 \tag{6}
$$

Từ (5) và (6), ta ngay lập tức suy ra rằng $\sum^{n+1}_{i=0}(-1)^i\varphi (E_i) = 0$, và hệ quả được chứng minh.

#### Mệnh đề 2 {#alg-viii-s11-prop-2 .statement tag=00D0}

Giả sử tập hợp $\mathscr{C}$ là di truyền. Cho E là một A-môđun, và cho M và N là các môđun con của E.

a) Nếu các môđun M và N có kiểu $\mathscr{C}$, thì các môđun $M\cap N$ và M + N cũng vậy, và ta có

$$
\varphi (M + N) +\varphi (M\cap N) =\varphi (M) +\varphi (N)
$$

b) Nếu các môđun $E/M$ và $E/N$ có kiểu $\mathscr{C}$, thì các môđun $E/(M\cap N)$ và $E/(M + N)$ cũng vậy, và ta có

$$
\varphi (E/(M + N)) +\varphi (E/(M\cap N)) =\varphi (E/M) +\varphi (E/N)
$$

Các mệnh đề a) và b) suy ra từ sự tồn tại của các dãy khớp

$$
0\rightarrow M\cap N\rightarrow M\oplus N\rightarrow M + N\rightarrow 0
$$

và

$$
0\rightarrow E/(M\cap N)\rightarrow (E/M)\oplus (E/N)\rightarrow E/(M + N)\rightarrow 0
$$

(II, §1, No. 7, p. 207, Mệnh đề 10).

#### Mệnh đề 3 {#alg-viii-s11-prop-3 .statement tag=00D1}

Giả sử $\mathscr{C}$ là di truyền. Cho E là một môđun có kiểu $\mathscr{C}$ và $(E_i)_{0\leqslant i\leqslant n}$ là một chuỗi hợp thành của E (I, §4, No. 7, p. 41). Với $1\leqslant i\leqslant n$, môđun $E_{i-1}/E_i$ có kiểu $\mathscr{C}$, và ta có

$$
\varphi (E) =\sum_{i=1}^n\varphi (E_{i-1}/E_i)
$$

Vì $\mathscr{C}$ là di truyền, các môđun $E_0/E_1$ và $E_1$ có kiểu $\mathscr{C}$, và ta có $\varphi (E) =\varphi (E_0/E_1) +\varphi (E_1)$. Vì dãy $(E_{i+1})_{0\leqslant i\leqslant n-1}$ là một chuỗi hợp thành của $E_1$, Mệnh đề 3 suy ra bằng quy nạp theo $n$.

### 2. Nhóm Grothendieck của một tập hợp cộng tính các môđun

Cho A là một vành. Trong tiểu mục này, ta xét một tập hợp cộng tính $\mathscr{C}$ gồm các lớp của các A-môđun; ta đồng nhất $\mathscr{C}$ với cơ sở chính tắc của nhóm Abel tự do $\mathbf{Z}^{(\mathscr{C})}$. Với mọi dãy khớp

$$
(\mathscr{E})0\longrightarrow E'\longrightarrow E\longrightarrow E''\longrightarrow 0
$$

của các môđun có kiểu $\mathscr{C}$, ta ký hiệu $r_{\mathscr{E}}$ là phần tử cl(E) $-$ cl(E$'$)$-$ cl(E$''$) của $\mathbf{Z}^{(\mathscr{C})}$. Gọi R là nhóm con của $\mathbf{Z}^{(\mathscr{C})}$ sinh bởi các phần tử có dạng $r_{\mathscr{E}}$; nhóm thương $\mathbf{Z}^{(\mathscr{C})}/R$ được gọi là nhóm Grothendieck của $\mathscr{C}$ và được ký hiệu là $K(\mathscr{C})$. Với một môđun E có kiểu $\mathscr{C}$, ta ký hiệu ảnh của cl(E) trong $K(\mathscr{C})$ là $[E]_{\mathscr{C}}$ (hoặc đôi khi [E] khi không rõ $\mathscr{C}$ đang được xét). Khi đó ta có tính chất phổ quát sau.

#### Mệnh đề 4 {#alg-viii-s11-prop-4 .statement tag=00D2}

a) Ánh xạ $E\mapsto [E]_{\mathscr{C}}$ từ $\mathscr{C}$ vào $K(\mathscr{C})$ là cộng tính.

b) Cho G là một nhóm Abel, và cho $\varphi :\mathscr{C}\rightarrow G$ là một hàm cộng tính trên các môđun. Tồn tại một đồng cấu duy nhất $u: K(\mathscr{C})\rightarrow G$ sao cho $\varphi (E) =u([E]_{\mathscr{C}})$ với mọi môđun E có kiểu $\mathscr{C}$.

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

Tiếp theo, cho $M_1, . . . ,M_m,N_1, . . . ,N_n$ là các A-môđun kiểu $\mathscr{C}$. Nếu ta có $\sum^m_{i=1}$ cl(M$_i$) $=\sum^n_{j=1}$ cl(N$_j$) trong nhóm $\mathbf{Z}^{(\mathscr{C})}$, thì ta có $m=n$ và tồn tại một phép hoán vị $\sigma \in \mathfrak{S}_m$ sao cho cl(M$_i$) $=$ cl(N$_{\sigma(i)}$) với mọi $1\leqslant i\leqslant m$ (I, §7, No. 9, p. 95, Mệnh đề 11). Do đó, các môđun $\bigoplus^m_{i=1}M_i$ và $\bigoplus^n_{j=1}N_j$ là đẳng cấu. Đặc biệt, từ (7), ta suy ra sự tồn tại của một đẳng cấu từ $E\oplus Q$ đến $F\oplus P$, trong đó ta đặt

$$
P = G'\oplus G''\oplus H,Q = G\oplus H'\oplus H''
$$

Ta cũng đặt

$$
L = G'\oplus H',M = G''\oplus H''
$$

Các môđun L, M, P, Q có kiểu $\mathscr{C}$, và dãy

$(\mathscr{E})$ 0 // L $^{\lambda}$ // P $^\mu$ // M // $0$,

trong đó ta định nghĩa $\lambda$ và $\mu$ bởi

$$
\lambda (g', h') = (g',0, r(h')),\mu(g', g'', h) = (g'', s(h))
$$

là khớp. Ta xây dựng một dãy khớp

$$
(\mathscr{F})0\longrightarrow L\longrightarrow Q\longrightarrow M\longrightarrow 0
$$

theo cùng cách đó; điều này kết thúc chứng minh.

Tập hợp $\mathscr{C}$ là một nửa nhóm giao hoán đối với luật hợp thành $(E,E')\mapsto$ cl(E$\oplus E'$). Đôi khi ta ký hiệu nhóm các hiệu của nửa nhóm giao hoán $\mathscr{C}$ (I, §2, No. 4, p. 20) bởi $K'(\mathscr{C})$ và gọi nó là nhóm Grothendieck của $\mathscr{C}$ đối với các tổng trực tiếp. Với mọi môđun E có kiểu $\mathscr{C}$, ta ký hiệu ảnh của cl(E) trong $K'(\mathscr{C})$ bởi $[E]'_{\mathscr{C}}$.

#### Mệnh đề 6 {#alg-viii-s11-prop-6 .statement tag=00D5}

a) Ánh xạ $E\mapsto [E]'_{\mathscr{C}}$ từ $\mathscr{C}$ vào $K'(\mathscr{C})$ là một hàm cộng tính yếu của các môđun.

b) Cho G là một nhóm Abel, và cho $\varphi :\mathscr{C}\rightarrow G$ là một hàm cộng tính yếu của các môđun. Tồn tại một đồng cấu nhóm duy nhất $u: K'(\mathscr{C})\rightarrow$ G sao cho $\varphi (E) =u([E]'_{\mathscr{C}})$ với mọi môđun E có kiểu $\mathscr{C}$.

c) Cho E và F là các môđun có kiểu $\mathscr{C}$. Ta có $[E]'_{\mathscr{C}}= [F]'_{\mathscr{C}}$ khi và chỉ khi tồn tại một môđun M có kiểu $\mathscr{C}$ sao cho $E\oplus M$ đẳng cấu với $F\oplus M$.

Mệnh đề a) là hiển nhiên. Mệnh đề b) suy ra từ (I, §2, No. 4, p. 19, Định lý 1) và mệnh đề c) từ (I, §2, No. 4, p. 18, Mệnh đề 6).

Vì ánh xạ $E\mapsto [E]_{\mathscr{C}}$ từ $\mathscr{C}$ vào $K(\mathscr{C})$ là một hàm cộng tính yếu của các môđun, ta có thể suy ra một đồng cấu $u: K'(\mathscr{C})\rightarrow K(\mathscr{C})$ từ nó. Đồng cấu này là toàn ánh nhưng không phải luôn là một đẳng cấu (VIII, p. 191, Nhận xét 2).

Cho $R'$ là nhóm con của $\mathbf{Z}^{(\mathscr{C})}$ sinh bởi các phần tử có dạng $r_{\mathscr{E}}$, trong đó $\mathscr{E}$ là một dãy khớp tách của các A-môđun kiểu $\mathscr{C}$, tức là bởi các phần tử có dạng cl(E$'\oplus E''$)$-$ cl(E$'$)$-$ cl(E$''$), trong đó $E'$ và $E''$ là các môđun kiểu $\mathscr{C}$. Ánh xạ chính tắc từ $\mathscr{C}$ vào nhóm thương $\mathbf{Z}^{(\mathscr{C})}/R'$ mở rộng thành một đồng cấu nhóm $v: K'(\mathscr{C})\rightarrow \mathbf{Z}^{(\mathscr{C})}/R'$. Đây là một đẳng cấu. Thật vậy, ánh xạ chính tắc từ $\mathscr{C}$ vào $K'(\mathscr{C})$ mở rộng thành một đồng cấu nhóm từ $\mathbf{Z}^{(\mathscr{C})}$ vào $K'(\mathscr{C})$ mà hạt nhân chứa $R'$, và do đó thành một đồng cấu $v':\mathbf{Z}^{(\mathscr{C})}/R'\rightarrow K'(\mathscr{C})$ bằng cách chuyển qua thương; rõ ràng $v$ và $v'$ là các song ánh nghịch đảo của nhau.

Một phần tử của $K'(\mathscr{C})$ được gọi là hiệu dụng nếu nó có dạng $[E]'_{\mathscr{C}}$ với một A-môđun E kiểu $\mathscr{C}$. Tập hợp các phần tử hiệu dụng của $K'(\mathscr{C})$ được ký hiệu là $K'(\mathscr{C})^+$.

### 3. Sử dụng các chuỗi hợp thành

Cho A là một vành. Cho E là một A-môđun có độ dài hữu hạn và S là một A-môđun đơn. Theo định lý Jordan–Hölder (I, §4, No. 7, p. 43, Định lý 6), số các thương của một chuỗi Jordan–Hölder của E đẳng cấu với S không phụ thuộc vào dãy. Ta ký hiệu số đó là $\ell_S(E)$ và gọi nó là bội số của S trong E. Giá đỡ của A-môđun E là tập hợp các lớp của các A-môđun đơn S sao cho $\ell_S(E)\not= 0$. Khi E là nửa đơn và có độ dài hữu hạn, số nguyên $\ell_S(E)$ là độ dài [E : S] của thành phần đẳng kiểu của E kiểu S (VIII, p. 72), và khái niệm giá đỡ trùng với khái niệm đã được đưa vào trong VIII, p. 66.

#### Bổ đề 1 {#alg-viii-s11-lem-1 .statement tag=00D6}

Cho E, $E'$, và $E''$ là các A-môđun có độ dài hữu hạn và

0 // ${E'}^i$ // E $^p$ // $E''$ // 0

là một dãy khớp. Ta có $\ell_S(E) =\ell_S(E') +\ell_S(E'')$.

Cho $\Sigma '$ và $\Sigma ''$ lần lượt là các chuỗi Jordan–Hölder của $i(E')$ và $E/i(E')$. Tồn tại một chuỗi Jordan–Hölder Σ của E mà dãy các thương của nó có thể thu được bằng cách ghép dãy các thương của Σ và dãy các thương của $\Sigma '$ (I, §4, No. 8, p. 44).

#### Mệnh đề 7 {#alg-viii-s11-prop-7 .statement tag=00D7}

Cho $\mathscr{C}$ là một tập hợp di truyền các lớp môđun sao cho mọi môđun kiểu $\mathscr{C}$ đều có độ dài hữu hạn. Cho $\mathscr{S}$ là tập hợp các lớp của các môđun đơn thuộc $\mathscr{C}$. Khi đó họ $([S]_{\mathscr{C}})_{S\in\mathscr{S}}$ là một cơ sở của môđun $\mathbf{Z}$ $K(\mathscr{C})$, và ta có

$$
[E]_{\mathscr{C}}=\sum_{S\in\mathscr{S}}\ell_S(E)[S]_{\mathscr{C}} \tag{8}
$$

với mọi môđun E kiểu $\mathscr{C}$.

Công thức (8) suy ra từ Mệnh đề 3 áp dụng cho một chuỗi Jordan–Hölder của E. Theo Bổ đề 1, với mọi phần tử S của $\mathscr{S}$, tồn tại một ánh xạ tuyến tính $\mathbf{Z}$-tuyến tính $\varphi_S$ từ $K(\mathscr{C})$ vào $\mathbf{Z}$ sao cho $\varphi_S([E]_{\mathscr{C}}) =\ell_S(E)$ với mọi môđun E thuộc kiểu $\mathscr{C}$. Đặc biệt, ta có $\varphi_S([S]_{\mathscr{C}}) = 1$ và $\varphi_S([S']_{\mathscr{C}}) = 0$ với mọi $S'\not= S$ trong $\mathscr{S}$. Suy ra rằng các phần tử có dạng $[S]_{\mathscr{C}}$ (với $S\in \mathscr{S}$) độc lập tuyến tính trên $\mathbf{Z}$; các phần tử này sinh $K(\mathscr{C})$ theo công thức (8).

#### Hệ quả {#alg-viii-s11-n3-cor-1 .statement tag=00D8}

Cho E và F là các môđun nửa đơn thuộc kiểu $\mathscr{C}$. Môđun E đẳng cấu với F khi và chỉ khi ta có $[E]_{\mathscr{C}}= [F]_{\mathscr{C}}$ trong $K(\mathscr{C})$.

Thật vậy, ta có $[E]_{\mathscr{C}}=\sum_{S\in\mathscr{S}}\ell_S(E)[S]_{\mathscr{C}}$ và một công thức tương tự cho F, và E đẳng cấu với F khi và chỉ khi ta có $\ell_S(E) =\ell_S(F)$ với mọi $S\in \mathscr{S}$ (VIII, p. 72).

#### Nhận xét {#alg-viii-s11-n3-rem-1 .statement tag=00D9}

Tập hợp $K(\mathscr{C})^+$ là monoid con của $K(\mathscr{C})$ sinh bởi họ $([S]_{\mathscr{C}})_{S\in\mathscr{S}}$.

### 4. Nhóm Grothendieck R(A)

Cho A là một vành. Cho $\mathscr{F}(A)$ là tập hợp các lớp của các A-môđun sinh hữu hạn (VIII, p. 51). Các lớp của các A-môđun có độ dài hữu hạn tạo thành một tập con $\mathscr{L}\mathscr{F}(A)$ của $\mathscr{F}(A)$; ta đã thấy rằng $\mathscr{L}\mathscr{F}(A)$ là một tập hợp di truyền của các lớp môđun. Ta ký hiệu nhóm Grothendieck liên kết với $\mathscr{L}\mathscr{F}(A)$ bởi R(A) và ảnh trong R(A) của lớp của một A-môđun E có độ dài hữu hạn bởi [E].

Các kết quả của Tiểu mục 3 kéo theo điều sau:

a) Cho $\mathscr{S}(A)$ là tập hợp các lớp của các A-môđun đơn. Họ $([S])_{S\in\mathscr{S}(A)}$ là một cơ sở của $\mathbf{Z}$-môđun R(A).

b) Cho E và F là các A-môđun nửa đơn có độ dài hữu hạn. Khi đó E và F đẳng cấu khi và chỉ khi ta có [E] = [F] trong R(A).

c) Cho E là một A-môđun có độ dài hữu hạn và $(E_i)_{0\leqslant i\leqslant n}$ là một chuỗi Jordan–Hölder của E. Đặt $F =\bigoplus^n_{i=1}(E_{i-1}/E_i)$. Khi đó F là một A-môđun nửa đơn có độ dài hữu hạn, và ta có [E] = [F] trong R(A).

d) Cho $\ell : R(A)\rightarrow \mathbf{Z}$ là đồng cấu được đặc trưng bởi $\ell ([S]) = 1$ với mọi A-môđun đơn S. Khi đó ta có $\ell ([E]) =\sum_{S\in\mathscr{S}(A)}\ell_S(E) =$ long$_A(E)$ với mọi A-môđun E có độ dài hữu hạn.

Nếu D là một trường, thì đồng cấu $\ell : R(D)\rightarrow \mathbf{Z}$ là một đẳng cấu.

#### Nhận xét 1 {#alg-viii-s11-n4-rem-1 .statement tag=00DA}

Cho $\mathscr{S}\mathscr{S}(A)$ là tập hợp di truyền của các lớp các A-môđun nửa đơn có độ dài hữu hạn. Theo Mệnh đề 7 của VIII, p. 190, nhóm Grothendieck $K(\mathscr{S}\mathscr{S}(A))$ là một $\mathbf{Z}$-môđun tự do mà các phần tử $[S]_{\mathscr{S}\mathscr{S}(A)}$ (với $S\in \mathscr{S}(A)$) tạo thành một cơ sở. Đồng cấu chính tắc $\gamma_{\mathscr{L}\mathscr{F}(A),\mathscr{S}\mathscr{S}(A)}$ (VIII, p. 186) do đó là một đẳng cấu.

#### Nhận xét 2 {#alg-viii-s11-n4-rem-2 .statement tag=00DB}

Cho $K'(\mathscr{L}\mathscr{F}(A))$ là nhóm Grothendieck của $\mathscr{L}\mathscr{F}(A)$ đối với các tổng trực tiếp (VIII, p. 188). Định lý Krull–Remak–Schmidt (VIII, p. 37) kéo theo rằng $K'(\mathscr{L}\mathscr{F}(A))$ là một $\mathbf{Z}$-môđun tự do với cơ sở là tập hợp các lớp của các A-môđun không phân tích được có độ dài hữu hạn, trong khi $K(\mathscr{L}\mathscr{F}(A))$ nhận tập hợp các lớp của các A-môđun đơn làm cơ sở.

#### Nhận xét 3 {#alg-viii-s11-n4-rem-3 .statement tag=00DC}

Cho E là một A-môđun có độ dài hữu hạn. Theo c), tồn tại một A-môđun nửa đơn $E'$ có độ dài hữu hạn sao cho $[E] = [E']$, và theo b), một môđun như vậy được xác định sai khác một đẳng cấu; đôi khi ta gọi nó là một nửa đơn hóa của E.

#### Mệnh đề 8 {#alg-viii-s11-prop-8 .statement tag=00DD}

Cho A là một miền iđêan chính không phải là một trường, và cho L là trường phân thức của nó. Tồn tại một đẳng cấu $\varphi : R(A)\rightarrow L^*/A^*$ sao cho ta có

$$
\varphi ([A/aA]) =aA^* \tag{9}
$$

với mọi $a\not= 0$ trong A.

Cho P là một hệ đại diện gồm các phần tử bất khả quy của A (VII, §1, No. 3, p. 3). Các iđêan cực đại của A là các iđêan $pA$ với $p\in P$; do đó mọi A-môđun đơn đều đẳng cấu với một môđun duy nhất $A/pA$. Hơn nữa (VII, §1, No. 3, p. 4, Định lý 2), nhóm Abel $L^*/A^*$ là tự do và có họ $(pA^*)_{p\in P}$ làm một cơ sở. Do đó tồn tại một đẳng cấu $\varphi$ từ R(A) đến $L^*/A^*$ được đặc trưng bởi $\varphi ([A/pA]) =pA^*$ đối với mọi $p\in P$.

Cho $a\not= 0$ trong A. Tồn tại một số nguyên $r\geqslant 0$, các phần tử $p_1, . . . , p_r$ của P, và một phần tử $u$ của $A^*$ sao cho ta có $a=up_1\cdots p_r$. Môđun $A/aA$ thừa nhận chuỗi hợp thành được cho bởi

$$
E_0= A/aA,E_i= (p_1\cdots p_iA)/aA(1\leqslant i\leqslant r)
$$

và môđun $E_{i-1}/E_i= (p_1\cdots p_{i-1}A)/(p_1\cdots p_iA)$ đẳng cấu với $A/p_iA$. Do đó ta có (VIII, p. 185, Mệnh đề 3)

$$
\varphi ([A/aA]) =\prod_{i=1}^r\varphi ([A/p_iA]) =p_1\cdots p_rA^*=aA^*
$$

#### Nhận xét 4 {#alg-viii-s11-n4-rem-4 .statement tag=00DE}

Ta giữ các giả thiết và ký hiệu của Mệnh đề 8. Cho E là một A-môđun có độ dài hữu hạn, và cho $a_1A, . . . , a_nA$ là các nhân tử bất biến của nó (VII, §4, No. 5, p. 20). Vì E đẳng cấu với $\bigoplus_{i=1}^nA/a_iA$, ta có

$$
\varphi ([E]) =\prod_{i=1}^n\varphi ([A/a_iA]) =a_1\cdots a_nA^* \tag{10}
$$

#### Nhận xét 5 {#alg-viii-s11-n4-rem-5 .statement tag=00SI}

Cho A là một vành Dedekind không phải là một trường (Comm. Alg., VIII, §2, No. 1). Bằng lập luận như trong Mệnh đề 8, ta có thể chứng minh sự tồn tại của một đẳng cấu $\varphi$ từ R(A) đến nhóm các iđêan phân thức của A, được đặc trưng bởi $\varphi ([A/\mathfrak{a}]) =\mathfrak{a}$ đối với mọi iđêan khác không $\mathfrak{a}$ của $A.*$

Mệnh đề 8 sẽ được dùng, chẳng hạn, trong hai trường hợp sau:

a) Giả sử ta có $A =\mathbf{Z}$. Các $\mathbf{Z}$-môđun có độ dài hữu hạn chẳng qua là các nhóm Abel hữu hạn. Vì $\mathbf{Q}^*$ là tích trực tiếp của $\mathbf{Z}^*=$ $\{1,-1\}$ và $\mathbf{Q}^*_+$, ta có thể suy ra từ Mệnh đề 8 một đẳng cấu $\varphi '$ từ $R(\mathbf{Z})$ đến $\mathbf{Q}^*_+$ được cho bởi

$\varphi '([G]) =$ Card(G)

với mọi nhóm Abel hữu hạn G.

b) Giả sử A là vành đa thức K[T] trên một biến T với hệ số trong một trường giao hoán K. Cho E là một không gian vectơ hữu hạn chiều trên K và $u$ là một tự đồng cấu của E. Như trong VII, §5, No. 1, p. 29, ký hiệu $E_u$ là A-môđun có nhóm cộng nền E và luật ngoài $(p, x)\mapsto p(u)x$. Môđun A $E_u$ có độ dài hữu hạn. Chiều ngược lại, mọi A-môđun đơn đều hữu hạn chiều trên K (VII, §4, No. 8, p. 25, Nhận xét 4). Do đó, mọi A-môđun có độ dài hữu hạn đều hữu hạn chiều trên K, nên có dạng $E_u$. Hơn nữa (VII, §5, No. 3, p. 32, Hệ quả 1), tích các nhân tử bất biến của $E_u$ bằng với đa thức đặc trưng $\chi_u$ của $u$. Do đó, Mệnh đề 8 cho một đẳng cấu

$$
\varphi : R(K[T])\rightarrow K(T)^*/K^*
$$

được đặc trưng bởi $\varphi ([E_u]) =\chi_uK^*$ (xem công thức (10)).

### 5. Thay đổi vành

Cho A và B là các vành, và cho $f: A\rightarrow B$ là một đồng cấu vành. Cho $\mathscr{C}$ là một tập hợp cộng tính các A-môđun và $\mathscr{D}$ là một tập hợp cộng tính các B-môđun.

Trước hết, giả sử rằng với mọi B-môđun M thuộc kiểu $\mathscr{D}$, A-môđun $f_*(M)$ thu được bằng cách hạn chế vành vô hướng về A thuộc kiểu $\mathscr{C}$. Khi đó ánh xạ từ $\mathscr{D}$ đến $K(\mathscr{C})$ gửi M đến $[f_*(M)]_{\mathscr{C}}$ là một hàm cộng tính của môđun; từ đó, ta suy ra một đồng cấu nhóm

$$
f_*: K(\mathscr{D})\longrightarrow K(\mathscr{C})
$$

Ta định nghĩa một đồng cấu nhóm $f_*: K'(\mathscr{D})\rightarrow K'(\mathscr{C})$ tương tự.

Bây giờ ta giả sử rằng với mọi A-môđun E thuộc kiểu $\mathscr{C}$, B-môđun $f^*(E)$ thu được từ E bằng cách mở rộng vô hướng qua $f$ (II, §5, No. 1, p. 277) thuộc kiểu $\mathscr{D}$. Ánh xạ từ $\mathscr{C}$ đến $K'(\mathscr{D})$ gửi một phần tử E của $\mathscr{C}$ đến $[f^*(E)]'_{\mathscr{D}}$ là một hàm cộng tính yếu của các môđun; do đó nó cảm sinh một đồng cấu nhóm $f^*: K'(\mathscr{C})\rightarrow K'(\mathscr{D})$.

Giả sử, hơn nữa, rằng với mọi dãy khớp

$$
0\longrightarrow E'\longrightarrow E\longrightarrow E''\longrightarrow 0
$$

của các A-môđun thuộc kiểu $\mathscr{C}$, dãy các B-môđun thuộc kiểu $\mathscr{D}$

$$
0\longrightarrow B\otimes_AE'\longrightarrow B\otimes_AE\longrightarrow B\otimes_AE''\longrightarrow 0
$$

là khớp. Điều này đúng, đặc biệt, trong các trường hợp sau:

a) Đồng cấu $f$ biến B thành một A-môđun xạ ảnh (II, §3, No. 6, p. 251, Mệnh đề 5 và II, §3, No. 7, p. 257, Hệ quả $6$)$*$hoặc, nói chung, một A-môđun phẳng (X, §1, n$^o3$, p. 8, Định nghĩa 1) A-môđun$*$.

b) $*$Tập hợp $\mathscr{C}$ là một tập hợp các lớp của các A-môđun xạ ảnh hoặc, nói chung, phẳng (X,

§4, n$^o5$, p. 72, Hệ quả 2) A-môđun$*$.

Ánh xạ từ $\mathscr{C}$ đến $K(\mathscr{D})$ gửi E đến $[f^*(E)]_{\mathscr{D}}$ khi đó là một hàm cộng tính. Do đó nó cảm sinh một đồng cấu nhóm $f^*: K(\mathscr{C})\rightarrow K(\mathscr{D})$.

### 6. Nhóm Grothendieck $R_K(A)$

Cho K là một trường giao hoán và A là một đại số trên K. Tập hợp các lớp của các A-môđun hữu hạn chiều trên K là di truyền. Nhóm Grothendieck tương ứng được ký hiệu bởi $R_K(A)$. Nó là một $\mathbf{Z}$-môđun tự do với cơ sở là họ $([S])_{S\in\mathscr{S}}$, trong đó $\mathscr{S}$ là tập hợp các lớp của các A-môđun đơn hữu hạn chiều trên K. Tồn tại một đồng cấu

dim$: R_K(A)\longrightarrow \mathbf{Z}$

được đặc trưng bởi dim([E]) = [E : K] đối với mọi A-môđun E hữu hạn chiều trên K. Khi A = K, nó là một đẳng cấu. Monoid con của các phần tử hiệu dụng được ký hiệu bởi $R_K(A)^+$.

#### Bổ đề 2 {#alg-viii-s11-lem-2 .statement tag=00DF}

Cho M và $M'$ là các A-môđun hữu hạn chiều trên K. Các giá đỡ (VIII, p. 190) của M và $M'$ rời nhau khi và chỉ khi tồn tại một $a\in A$ sao cho $a_M= 0_M$ và $a_{M'}= 1_{M'}$.

Giả sử tồn tại một $a\in A$ sao cho $a_M= 0_M$ và $a_{M'}= 1_{M'}$. Cho S là một A-môđun đơn. Nếu cl(S) thuộc giá đỡ $\mathscr{S}_M$ của M, thì A-môđun S đẳng cấu với một trong các thương của một dãy Jordan–Hölder của M và ta có $a_S= 0_S$. Tương tự, nếu cl(S) thuộc giá đỡ $\mathscr{S}_{M'}$ của M’, thì ta có $a_S= 1_S$. Suy ra rằng $\mathscr{S}_M$ và $\mathscr{S}_{M'}$ rời nhau.

Ngược lại, giả sử rằng các tập hợp $\mathscr{S}_M$ và $\mathscr{S}_{M'}$ rời nhau. Chúng hữu hạn vì M và $M'$ là hữu hạn chiều trên K. Mọi A-môđun đơn S mà lớp thuộc về $\mathscr{S}_M\cup \mathscr{S}_{M'}$ đều hữu hạn chiều trên K và a fortiori trên trường End$_A(S)$. Theo Hệ quả 1 của Mệnh đề 4 (VIII, p. 83), tồn tại một phần tử $b\in A$ sao cho ta có $b_S= 0_S$ (tương ứng $b_S= 1_S$) đối với mọi A-môđun đơn S mà lớp thuộc về $\mathscr{S}_M$ (tương ứng $\mathscr{S}_{M'}$). Cho $(M_i)_{0\leqslant i\leqslant n}$ là một chuỗi Jordan–Hölder của M. Theo điều trên, ta có $bM_i\subset M_{i+1}$ với $0\leqslant i < n$ và do đó $(b^n)_M= 0_M$. Sự tồn tại của một số tự nhiên $m$ sao cho $((1-b)^m)_{M'}= 0_{M'}$ được chứng minh theo cùng cách. Đặt $P(X) = 1-(1-X^n)^m$ và $a= P(b)$. Đa thức P(X) là một bội của $X^n$, nên ta có $a_M= 0_M$, trong khi đa thức $1-P(X)$ là một bội của $(1-X)^m$, nên ta có $a_{M'}= 1_{M'}$. Điều này kết thúc chứng minh.

Cho L là một mở rộng của K. Nếu M là một A-môđun hữu hạn chiều trên K, thì $M_{(L)}$ là một $A_{(L)}$-môđun hữu hạn chiều trên L. Hơn nữa, đối với mọi dãy khớp

$$
0\longrightarrow M'\longrightarrow M\longrightarrow M''\longrightarrow 0
$$

của các A-môđun, dãy các $A_{(L)}$-môđun

$$
0\longrightarrow M'_{(L)}\longrightarrow M_{(L)}\longrightarrow M''_{(L)}\longrightarrow 0
$$

suy ra từ nó bởi mở rộng vô hướng là khớp (II, §7, No. 7, p. 308, Mệnh đề 14). Do đó tồn tại một đồng cấu vành duy nhất $u: R_K(A)\rightarrow$ $R_L(A_{(L)})$ sao cho $u([M]) = [M_{(L)}]$ đối với mọi A-môđun M hữu hạn chiều trên K (No. 5).

#### Định lý 1 {#alg-viii-s11-thm-1 .statement tag=00DG}

Đồng cấu $u: R_K(A)\rightarrow R_L(A_{(L)})$ được xác định ở trên là đơn ánh. Cho $\xi$ là một phần tử của $R_K(A)$. Khi đó $\xi$ là hiệu dụng khi và chỉ khi $u(\xi )$ là hiệu dụng.

#### Bổ đề 3 {#alg-viii-s11-lem-3 .statement tag=00DH}

Cho S và T là hai A-môđun đơn không đẳng cấu hữu hạn chiều trên K. Các giá của các $A_{(L)}$-môđun $S_{(L)}$ và $T_{(L)}$ là rời nhau.

Theo Bổ đề 2, tồn tại một phần tử $a\in A$ sao cho $a_S= 0$ và $a_T= 1$. Phần tử $1\otimes a$ của $A_{(L)}$ tác động như 0 trên $S_{(L)}$ và như 1 trên $T_{(L)}$. Theo Bổ đề 2, các giá của các $A_{(L)}$-môđun $S_{(L)}$ và $T_{(L)}$ là rời nhau.

Chúng ta hãy chứng minh Định lý 1. Cho $\mathscr{S}$ là tập hợp các lớp của các A-môđun đơn hữu hạn chiều trên K. Họ $([S])_{S\in\mathscr{S}}$ là một cơ sở của $\mathbf{Z}$-môđun $R_K(A)$. Cho $S\in \mathscr{S}$. A-môđun $A_{(L)}$- $S_{(L)}$ không bằng không, do đó giá của nó không rỗng. Cho $S'$ là một phần tử của giá này. Theo Bổ đề 1 của VIII, p. 190, tồn tại một đồng cấu $f_{S'}: R_L(A_{(L)})\rightarrow \mathbf{Z}$ sao cho $f_{S'}([E]) =\ell_{S'}(E)$ với mọi A-môđun $A_{(L)}$- E hữu hạn chiều trên L. Theo phép dựng, ta có $f_{S'}([S_{(L)}])\not= 0$ và theo Bổ đề 3, $f([T_{(L)}]) = 0$ với mọi $T\in \mathscr{S}-\{S\}$. Do đó chúng ta đã chứng minh rằng các phần tử của $R_L(A_{(L)})$ có dạng $[S_{(L)}]$ với $S\in \mathscr{S}$ là độc lập tuyến tính trên $\mathbf{Z}$. Suy ra đồng cấu $u$ là đơn ánh.

Cho $S\in \mathscr{S}$, và cho $S'$ là một phần tử của giá của $S_{(L)}$. Với mọi $\xi \in R_K$(A), tọa độ của $\xi$ có chỉ số [S] trong cơ sở $([S])_{S\in\mathscr{S}}$ là $f_{S'}(u(\xi ))/[S_{(L)}: S']$. Suy ra rằng nếu $u(\xi )$ là hiệu dụng thì $\xi$ cũng vậy.

### 7. Cấu trúc nhân trên $K(\mathscr{C})$

Cho K là một vành giao hoán và A là một bigebra trên vành K (III, §11, No. 4, p. 585), với đồng tích $c$ và đồng đơn vị $\gamma$. Trừ khi có nói khác, các tích tenxơ đều trên K. Cho E và F là các A-môđun (trái). Tích tenxơ $E\otimes F$ được trang bị một cấu trúc môđun $(A\otimes$ A) được đặc trưng bởi công thức

$$
(a\otimes b)(x\otimes y) =ax\otimes by \tag{11}
$$

với $a, b\in A,x\in E$, và $y\in F$. Sử dụng đồng cấu $c: A\rightarrow A\otimes A$, từ A-môđun $(A\otimes$ A) này ta suy ra A-môđun $c_*(E\otimes F)$ (II, §1, No. 13, p. 221). Chính xác hơn, cho $a\in A$; nếu $c(a) =\sum_ia_i\otimes b_i$, thì ta có

$$
a(x\otimes y) =\sum_ia_ix\otimes b_iy \tag{12}
$$

với $x\in E$ và $y\in F$. Theo lạm dụng ký hiệu, ta cũng ký hiệu A-môđun thu được là $E\otimes F$. Từ tính kết hợp của $c$, suy ra ngay lập tức rằng đẳng cấu chính tắc của các K-môđun

$$
\varphi : (E\otimes F)\otimes G\longrightarrow E\otimes (F\otimes G)
$$

là A-tuyến tính với mọi A-môđun E, F và G. Tương tự, nếu bigebra A là đối giao hoán, thì đẳng cấu chính tắc từ $E\otimes F$ đến $F\otimes E$ là A-tuyến tính. Cuối cùng, cho $K_{\gamma}$ là A-môđun có nhóm nền K và phép toán ngoài $(a, x)\mapsto \gamma (a)x$. Đẳng cấu chính tắc từ $K\otimes E$ (resp. $E\otimes K$) đến E là một đẳng cấu các A-môđun từ $K_{\gamma}\otimes E$ (resp. $E\otimes K_{\gamma}$) đến E.

#### Mệnh đề 9 {#alg-viii-s11-prop-9 .statement tag=00DI}

Cho K là một vành giao hoán, A là một bigebra trên K với đồng đơn vị $\gamma$, và $\mathscr{C}$ là một tập hợp cộng tính các lớp A-môđun có các tính chất sau:

(i) Mọi A-môđun kiểu $\mathscr{C}$ đều là một K-môđun xạ ảnh $(*$hoặc, nói chung hơn, phẳng$*)$.

(ii) Nếu các A-môđun E và F là thuộc kiểu $\mathscr{C}$, thì A-môđun $E\otimes F$ cũng vậy.

(iii) A-môđun $K_{\gamma}$ được định nghĩa ở trên là thuộc kiểu $\mathscr{C}$. Khi đó tồn tại một cấu trúc vành duy nhất trên nhóm cộng $K(\mathscr{C})$ sao cho phép nhân của nó thỏa mãn

$$
[E]_{\mathscr{C}}[F]_{\mathscr{C}}= [E\otimes F]_{\mathscr{C}}
$$

với mọi A-môđun E và F thuộc kiểu $\mathscr{C}$. Phần tử đơn vị của $K(\mathscr{C})$ là $[K_{\gamma}]_{\mathscr{C}}$. Nếu đại số hai cấu A là đối giao hoán, thì vành $K(\mathscr{C})$ là giao hoán.

Được trang bị luật hợp thành cho bởi $(E,F)\mapsto$ cl(E $\otimes F$), tập hợp $\mathscr{C}$ là một nửa nhóm với phần tử đơn vị cl(K$_{\gamma}$). Do đó, $\mathbf{Z}^{(\mathscr{C})}$ được trang bị một cách chính tắc cấu trúc của một vành với phép nhân được đặc trưng bởi công thức

(13) cl(E) cl(F) = cl(E $\otimes F$)

và phần tử đơn vị cl(K$_{\gamma}$) (III, §2, No. 6, p. 446).

Cho một A-môđun F thuộc kiểu $\mathscr{C}$ và một dãy khớp

$$
(\mathscr{E})0\longrightarrow E'\longrightarrow E\longrightarrow E''\longrightarrow 0
$$

của các A-môđun thuộc kiểu $\mathscr{C}$, dãy

$$
(\mathscr{E}\otimes F)0\longrightarrow E'\otimes F\longrightarrow E\otimes F\longrightarrow E''\otimes F\longrightarrow 0
$$

suy ra từ $(\mathscr{E})$ là khớp vì F là xạ ảnh $(*$hoặc, tổng quát hơn, phẳng$*)$ trên K (II, §3, No. 6, p. 251, Mệnh đề 5 và II, §3, No. 7, p. 257, Hệ quả 6). Theo ký hiệu của No. 2, khi đó ta có

(14) $r_{\mathscr{E}\otimes F}=r_{\mathscr{E}}$ cl(F).

Suy ra rằng nhóm con R của $\mathbf{Z}^{(\mathscr{C})}$ sinh bởi các phần tử có dạng $r_{\mathscr{E}}$ là một iđêan phải của vành $\mathbf{Z}^{(\mathscr{C})}$, và người ta chứng minh tương tự rằng nó là một iđêan trái của $\mathbf{Z}^{(\mathscr{C})}$. Theo định nghĩa, $K(\mathscr{C})$ là nhóm thương $\mathbf{Z}^{(\mathscr{C})}/R$; do đó tồn tại một cấu trúc vành duy nhất trên $K(\mathscr{C})$ sao cho phép nhân của nó thỏa mãn $[E]_{\mathscr{C}}[F]_{\mathscr{C}}= [E\otimes F]_{\mathscr{C}}$ với mọi A-môđun E và F thuộc kiểu $\mathscr{C}$. Phần tử đơn vị của nó là $[K_{\gamma}]$.

Khi đại số hai cấu A là đối giao hoán, nửa nhóm $\mathscr{C}$ là giao hoán; suy ra vành $\mathbf{Z}^{(\mathscr{C})}$ và vành thương $K(\mathscr{C})$ là giao hoán.

#### Nhận xét {#alg-viii-s11-n7-rem-1 .statement tag=00DJ}

Chỉ với các giả thiết (i) và (ii) của Mệnh đề 9, nhóm Grothendieck $K'(\mathscr{C})$ đối với các tổng trực tiếp (VIII, p. 188) có một cấu trúc vành duy nhất sao cho phép nhân của nó thỏa mãn $[E]'_{\mathscr{C}}[F]'_{\mathscr{C}}= [E\otimes F]'_{\mathscr{C}}$. Phần tử đơn vị của nó là $[K_{\gamma}]'_{\mathscr{C}}$. Vành $K'(\mathscr{C})$ là giao hoán nếu đại số hai cấu A là đối giao hoán. Chứng minh tương tự như chứng minh của Mệnh đề 9 vì nhóm $K'(\mathscr{C})$ có thể được đồng nhất với $\mathbf{Z}^{(\mathscr{C})}/R'$, trong đó $R'$ là nhóm con của $\mathbf{Z}^{(\mathscr{C})}$ sinh bởi các phần tử có dạng cl(E$'\oplus E''$)$-$ cl(E$'$)$-$ cl(E$''$) (loc. cit.).

Dưới các giả thiết (i), (ii), và (iii) của Mệnh đề 9, vành $K(\mathscr{C})$ được gọi là vành Grothendieck của $\mathscr{C}$. Các điều kiện này, đặc biệt, được thỏa mãn khi K là một trường và $\mathscr{C}$ là tập hợp các lớp của các A-môđun hữu hạn chiều trên K. Do đó, ta có hệ quả sau.

#### Hệ quả {#alg-viii-s11-n7-cor-1 .statement tag=00DK}

Cho A là một đại số hai cấu với đồng đơn vị $\gamma$ trên một trường giao hoán K. Khi đó tồn tại một cấu trúc vành duy nhất trên nhóm cộng $R_K(A)$ sao cho phép nhân của nó thỏa mãn

$$
[E]_{\mathscr{C}}[F]_{\mathscr{C}}= [E\otimes_KF]_{\mathscr{C}}
$$

với mọi A-môđun E và F hữu hạn chiều trên K. Phần tử đơn vị của $R_K(A)$ là $[K_{\gamma}]_{\mathscr{C}}$. Nếu đại số hai cấu A là đối giao hoán, thì vành $R_K(A)$ là giao hoán.

#### Ví dụ 1 {#alg-viii-s11-n7-exa-1 .statement tag=00DL}

Cho K là một trường giao hoán. Cho G là một nhóm, và cho K[G] là đại số của nhóm G. Ta đồng nhất G với ảnh chính tắc của nó trong K[G] (III, §2, No. 6, p. 446).

We trang bị cho K[G] cấu trúc của một đại số song với đồng tích $c$ và đồng đơn vị $\gamma$ cho bởi

$$
c(g) =g\otimes g ,\gamma (g) = 1(g\in G) \tag{15}
$$

Cho E và F là các K[G]-môđun; theo công thức (12), cấu trúc K[G]-môđun trên $E\otimes F$ được cho bởi

$$
g(x\otimes y) =gx\otimes gy(g\in G, x\in E, y\in F) \tag{16}
$$

K[G]-môđun $K_{\gamma}$ là không gian vectơ K được trang bị tác động của G được định nghĩa bởi $g\lambda =\lambda$ với $g\in G$ và $\lambda \in K$.

Vành $R_K(K[G])$ cũng được ký hiệu là $R_K(G)$. Nó giao hoán; phép nhân của nó được cho bởi $[E] [F] = [E\otimes_KF]$, và phần tử đơn vị của $R_K(G)$ là $[K_{\gamma}]$.

#### Ví dụ 2 {#alg-viii-s11-n7-exa-2 .statement tag=00DM}

Cho $\mathfrak{g}$ là một đại số Lie trên một trường giao hoán K và $U(\mathfrak{g})$ là đại số bao của nó; ta đồng nhất $\mathfrak{g}$ với ảnh chính tắc của nó trong $U(\mathfrak{g}) ($Lie, I, §2, No. 7, p. 39, Hệ quả 2). Ta trang bị cho $U(\mathfrak{g})$ cấu trúc của một đại số song với đồng tích $c$ và đồng đơn vị $\gamma$ cho bởi

$$
c(\xi ) =\xi \otimes 1 + 1\otimes \xi ,\gamma (\xi ) = 0 \tag{17}
$$

với $\xi \in \mathfrak{g}($Lie, II, §1, No. 4, p. 115).

Cho E và F là các $U(\mathfrak{g}$)-môđun; theo công thức (17), cấu trúc $U(\mathfrak{g}$)-môđun trên $E\otimes F$ được đặc trưng bởi

$$
\xi (x\otimes y) =\xi x\otimes y+x\otimes \xi y \tag{18}
$$

với $\xi \in \mathfrak{g},x\in E$ và $y\in F$.

Vành Grothendieck $R_K(U(\mathfrak{g}))$ cũng được ký hiệu là $\mathscr{R}(\mathfrak{g})$ trong Lie, VIII, §7, No. 6, p. $139.*$

Cho A là một vành giao hoán. Ta có thể xem A như một đại số song đồng giao hoán trên chính nó, với đồng tích là đẳng cấu tự nhiên từ A đến $A\otimes_AA$ và đồng đơn vị Id$_A$ (III, §11, No. 4, p. 585). Theo Mệnh đề 9, ta thu được kết quả sau.

#### Mệnh đề 10 {#alg-viii-s11-prop-10 .statement tag=00DN}

Cho A là một vành giao hoán, và cho $\mathscr{C}$ là một tập hợp cộng tính các lớp của A-môđun thỏa mãn ba điều kiện sau:

(i) Mọi A-môđun thuộc kiểu $\mathscr{C}$ đều xạ ảnh $(*$hoặc, tổng quát hơn, phẳng$*)$.

(ii) Nếu E và F là các A-môđun thuộc kiểu $\mathscr{C}$, thì A-môđun $E\otimes_AF$ cũng thuộc kiểu $\mathscr{C}$.

(iii) A-môđun A thuộc kiểu $\mathscr{C}$.

Khi đó tồn tại duy nhất một cấu trúc vành trên nhóm cộng tính $K(\mathscr{C})$ thỏa mãn $[E]_{\mathscr{C}}[F]_{\mathscr{C}}= [E\otimes_AF]_{\mathscr{C}}$ với mọi cặp E, F của các A-môđun thuộc kiểu $\mathscr{C}$. Phần tử đơn vị của $K(\mathscr{C})$ là $[A]_{\mathscr{C}}$.

### 8. Nhóm Grothendieck $K_0(A)$

Cho A là một vành. Tập hợp $\mathscr{P}(A)$ các lớp của những A-môđun xạ ảnh sinh hữu hạn là cộng tính; ta ký hiệu nhóm Grothendieck $K(\mathscr{P}(A))$ bởi $K_0(A)$.

Đối với luật hợp thành $(E,E')\mapsto$ cl(E $\oplus E'$), tập hợp $\mathscr{P}(A)$ là một monoid giao hoán. Hơn nữa, mọi dãy khớp của các A-môđun xạ ảnh

$$
0\longrightarrow E'\longrightarrow E\longrightarrow E''\longrightarrow 0
$$

tách (II, §2, No. 2, p. 231, Mệnh đề 4), sao cho E đẳng cấu với $E'\oplus E''$. Ánh xạ $E\mapsto [E]$ từ $\mathscr{P}(A)$ vào $K_0(A)$ do đó xác định một đẳng cấu từ nhóm các hiệu của monoid $\mathscr{P}(A)$ vào $K_0(A)$ (VIII, p. 188).

Đối với mọi môđun xạ ảnh sinh hữu hạn P, tồn tại một môđun xạ ảnh sinh hữu hạn $P'$ sao cho $P\oplus P'$ là tự do (II, §2, No. 2, p. 232, Hệ quả 1). Cho E và F là các A-môđun xạ ảnh sinh hữu hạn; theo I, §2, No. 4, p. 18, Mệnh đề 6, ta có [E] = [F] trong $K_0(A)$ khi và chỉ khi tồn tại một A-môđun tự do sinh hữu hạn L sao cho các A-môđun $E\oplus L$ và $F\oplus L$ là đẳng cấu. Khi đó ta nói rằng E và F đẳng cấu ổn định; điều này không nhất thiết suy ra rằng E và F đẳng cấu (VIII, p. 207, Bài tập 2 và VIII, p. 210, Bài tập 14).

Khi vành A là giao hoán, tồn tại một cấu trúc vành giao hoán trên nhóm cộng $K_0(A)$ mà phép nhân được đặc trưng bởi công thức $[E]_{\mathscr{P}(A)}[F]_{\mathscr{P}(A)}= [E\otimes_AF]_{\mathscr{P}(A)}$ (VIII, p. 199, Mệnh đề 10).

#### Nhận xét {#alg-viii-s11-n8-rem-1 .statement tag=00DO}

Cho A là một vành nửa đơn. Khi đó mọi A-môđun đều nửa đơn và xạ ảnh (VIII, p. 138, Mệnh đề 4); do đó ta có đẳng thức

$$
\mathscr{L}\mathscr{F}(A) =\mathscr{S}\mathscr{S}(A) =\mathscr{P}(A)
$$

(xem No. 4 về các định nghĩa của $\mathscr{L}\mathscr{F}(A)$ và $\mathscr{S}\mathscr{S}(A)$). Do đó ta có $K_0(A) = R(A)$ theo các định nghĩa của các nhóm Grothendieck này.

#### Ví dụ {#alg-viii-s11-n8-exa-1 .statement tag=00DP}

Nếu mọi A-môđun xạ ảnh sinh hữu hạn đều tự do, thì hạng xác định một đẳng cấu từ $K_0(A)$ vào $\mathbf{Z}$. Điều này, đặc biệt, đúng khi A là một miền iđêan chính (VII, §1, No. 3, p. 15, Hệ quả 3) hoặc khi A là một vành địa phương (VIII, p. 36, Hệ quả 6).

### 9. Nhóm Grothendieck $K_0(A)$ của một vành Artin

Cho A là một vành Artin trái. Gọi $\mathfrak{r}$ là căn của nó; đó là một iđêan hai phía lũy linh của A, và vành $A/\mathfrak{r}$ là nửa đơn (VIII, p. 173, Mệnh đề 1). Theo hệ quả của VIII, p. 176, ánh xạ $P\mapsto$ cl(P$/\mathfrak{r}P$) là một đẳng cấu từ monoid $\mathscr{P}(A)$ vào monoid $\mathscr{P}(A/\mathfrak{r})$. Ta suy ra từ đó một đẳng cấu nhóm $\gamma$ từ $K_0(A)$ vào $K_0(A/\mathfrak{r})$ được đặc trưng bởi quan hệ $\gamma ([P]_{\mathscr{P}(A)}) = [P/\mathfrak{r}P]_{\mathscr{P}(A/\mathfrak{r})}$ đối với mọi A-môđun xạ ảnh sinh hữu hạn P.

Vì vành $A/\mathfrak{r}$ là nửa đơn, nhận xét trên suy ra đẳng thức $R(A/\mathfrak{r}) = K_0(A/\mathfrak{r})$. Các môđun có độ dài hữu hạn trên vành $A/\mathfrak{r}$ chính là các môđun nửa đơn có độ dài hữu hạn trên vành A (VIII, p. 174, Mệnh đề 2); do đó, ta có thể đồng nhất $\mathscr{L}\mathscr{F}(A/\mathfrak{r})$ với $\mathscr{S}\mathscr{S}(A)$ và $R(A/\mathfrak{r})$ với $K(\mathscr{S}\mathscr{S}(A))$. Ta ký hiệu $\delta$ là đồng cấu $\gamma_{\mathscr{L}\mathscr{F}(A),\mathscr{S}\mathscr{S}(A)}$ từ $R(A/\mathfrak{r}) = K(\mathscr{S}\mathscr{S}(A))$ vào $R(A) = K(\mathscr{L}\mathscr{F}(A))$ (VIII, p. 191, Nhận xét 1); nó là một đẳng cấu. Cuối cùng, ta có $\mathscr{P}(A)\subset \mathscr{L}\mathscr{F}$(A), và ta đặt $\varepsilon =$ \gamma_{\mathscr{LF}(A),\mathscr{P}(A)}. Ta đã xác định một biểu đồ

$$
\begin{array}{ccc}
K_0(A) & \xrightarrow{\gamma} & K_0(A/\mathfrak{r}) = R(A/\mathfrak{r}) \\
& \searrow^{\varepsilon} & \swarrow^{\delta} \\
& & R(A).
\end{array}
$$

Chúng tôi ký hiệu tập hợp (hữu hạn) các lớp của các A-môđun đơn bởi $\mathscr{S}$; với mọi $\lambda \in \mathscr{S}$, chọn một môđun $S_\lambda$ thuộc lớp $\lambda$ và một vỏ xạ ảnh $(P_\lambda, u_\lambda)$ của $S_\lambda$ (VIII, p. 175, Mệnh đề 4). Suy ra từ Mệnh đề 6 của VIII, p. 176 rằng $K_0(A)$ là một $\mathbf{Z}$-môđun tự do với cơ sở là họ $([P_\lambda]_{\mathscr{P}(A)})_{\lambda \in \mathscr{S}}$. Hơn nữa, vì $S_\lambda$ đẳng cấu với $P_\lambda / \mathfrak{r} P_\lambda$ (VIII, p. 176), $\gamma$ biến cơ sở $([P_\lambda]_{\mathscr{P}(A)})_{\lambda \in \mathscr{S}}$ của $K_0(A)$ thành cơ sở $([S_\lambda])_{\lambda \in \mathscr{S}}$ của $R(A/\mathfrak{r})$. Đẳng cấu $\delta$ biến cơ sở $([S_\lambda])_{\lambda \in \mathscr{S}}$ của $R(A/\mathfrak{r})$ thành cơ sở $([S_\lambda])_{\lambda \in \mathscr{S}}$ của $R(A)$.

*Ma trận Cartan* của $A$ là ma trận $(a_{\lambda \mu})$ của đồng cấu của các $\mathbf{Z}$-môđun $\varepsilon : K_0(A) \to R(A)$ đối với các cơ sở $([P_\lambda]_{\mathscr{P}(A)})_{\lambda \in \mathscr{S}}$ của $K_0(A)$ và $([S_\lambda])_{\lambda \in \mathscr{S}}$ của $R(A)$. Theo định nghĩa, ta có

$$
[P_\mu] = \sum_{\lambda \in \mathscr{S}} a_{\lambda \mu} [S_\lambda] \qquad (\mu \in \mathscr{S})
$$

trong nhóm $R(A)$. Nói cách khác, $a_{\lambda \mu}$ là số các thương đẳng cấu với $S_\lambda$ trong một chuỗi Jordan–Hölder của A-môđun $P_\mu$.

Đặt $\pi = \varepsilon \circ \gamma^{-1} \circ \delta^{-1}$; đó là một tự đồng cấu của nhóm $R(A)$. Nếu M là một A-môđun nửa đơn sinh hữu hạn và $(P, u)$ là một vỏ xạ ảnh của M, thì ta có $\pi([M]) = [P]$. Theo công thức (19), ma trận của $\pi$ đối với cơ sở $([S_\lambda])_{\lambda \in \mathscr{S}}$ của $R(A)$ chính là ma trận Cartan của $A$.

### 10. Thay đổi vành đối với $K_0(A)$

Cho A và B là các vành. Cho $f : A \to B$ là một đồng cấu vành. Nếu P là một A-môđun xạ ảnh sinh hữu hạn, thì B-môđun $f^*(P) = B \otimes_A P$ là xạ ảnh và sinh hữu hạn (II, §5, No. 2, p. 281, Hệ quả). Ánh xạ $P \mapsto \operatorname{cl}(f^*(P))$ là một đồng cấu từ monoid $\mathscr{P}(A)$ sang monoid $\mathscr{P}(B)$ và do đó xác định một đồng cấu $f^* : K_0(A) \to K_0(B)$ được đặc trưng bởi quan hệ $f^*([P]_{\mathscr{P}(A)}) = [f^*(P)]_{\mathscr{P}(B)}$ với mọi A-môđun xạ ảnh sinh hữu hạn P. Nếu $g : B \to C$ là một đồng cấu vành thứ hai, thì từ tính bắc cầu của mở rộng vô hướng (II, §5, No. 1, p. 278, Mệnh đề 2) suy ra rằng các đồng cấu $(g\circ f)^*$ và $g^*\circ f^*$ từ $K_0(A)$ đến $K_0(C)$ bằng nhau.

Do đó nếu $f$ làm cho $B$ trở thành một $A$-môđun xạ ảnh sinh hữu hạn bên trái. Cho $Q$ là một $B$-môđun xạ ảnh sinh hữu hạn bên trái. Khi đó $Q$ là một nhân tử trực tiếp của một $B$-môđun tự do sinh hữu hạn, vốn xạ ảnh và sinh hữu hạn trên $A$. Do đó, $A$-môđun $f_*(Q)$ thu được từ $Q$ bằng phép hạn chế vô hướng là xạ ảnh và sinh hữu hạn. Như trên, ta suy ra một đồng cấu $f_*: K_0(B)\rightarrow K_0(A)$ được đặc trưng bởi quan hệ $f_*([Q]_{\mathscr{P}(B)}) = [f_*(Q)]_{\mathscr{P}(A)}$ với mọi $B$-môđun xạ ảnh sinh hữu hạn $Q$. Nếu $g: B\rightarrow C$ là một đồng cấu vành làm cho $C$ trở thành một $B$-môđun xạ ảnh sinh hữu hạn, thì các đồng cấu $(g\circ f)_*$ và $f_*\circ g_*$ từ $K_0(C)$ đến $K_0(A)$ bằng nhau.

### 11. Luật tương hỗ Frobenius

Cho $A$ là một vành nửa đơn. Cho $f$ là một đồng cấu từ $A$ đến một vành nửa đơn $B$. Cho $S$ là một $A$-môđun đơn và $T$ một $B$-môđun đơn, và cho $D$ và $E$ lần lượt là các bộ giao hoán của $S$ và $T$. Theo bổ đề Schur (VIII, p. 47, Hệ quả), $D$ và $E$ là các trường. Cho $H$ là tập hợp các đồng cấu A-tuyến tính từ $S$ đến $f_*(T)$. Ta trang bị cho $H$ một cấu trúc song môđun $(E$, D) với các luật ngoài $(e, u)\mapsto e\circ u$ và $(d, u)\mapsto u\circ d$ với $e\in E,u\in H$, $d\in D$.

#### Mệnh đề 11 {#alg-viii-s11-prop-11 .statement tag=00DQ}

a) Bội số $[f_*(T) : S]$ của $A$-môđun đơn $S$ trong $A$-môđun nửa đơn $f_*(T)$ bằng số chiều của $H$ được xem như một không gian vectơ phải trên $D$.

b) Bội số $[f^*(S) : T]$ là hữu hạn và bằng số chiều của $H$ được xem như một không gian vectơ trái trên $E$.

Mệnh đề a) suy ra từ công thức (11) của VIII, p. 72.

$B$-môđun $f^*(S)$ là nửa đơn và sinh hữu hạn, do đó có độ dài hữu hạn. Theo công thức (12) của chỗ đã dẫn, ta có

(20) $[f^*(S) : T] =$ dim$_E$ Hom$_B(f^*(S),T)$.

Bây giờ, ở II, §5, No. 1, p. 277–278, công thức (2) và Nhận xét 2, ta đã định nghĩa một song ánh E-tuyến tính từ Hom$_A(S, f_*(T))$ đến Hom$_B(f^*(S),T)$. Khi đó mệnh đề b) suy ra từ công thức (20).

#### Hệ quả (luật tương hỗ Frobenius) {#alg-viii-s11-n11-cor-1 .statement tag=00S7}

Giả sử rằng $A$ và $B$ là các đại số nửa đơn hữu hạn chiều trên một trường giao hoán $K$ và rằng $f$ là K-tuyến tính. Khi đó các không gian vectơ trên $K$ S, $T$, $D$, $E$ và $H$ đều hữu hạn chiều, và ta có các đẳng thức

$$
[f_*(T) : S][D : K] = [f^*(S) : T][E : K] = [H : K] \tag{21}
$$

Đặc biệt, khi $K$ đóng đại số, ta có $D = E = K$ và

$$
[f_*(T) : S] = [f^*(S) : T] = [H : K] \tag{22}
$$

Vì $A$-môđun $S$ là đơn, nên nó đơn sinh, và $D$ là một không gian con tuyến tính của Hom$_K(S,S)$; do đó $S$ và $D$ đều hữu hạn chiều trên $K$. Vì lý do tương tự, $T$ và $E$ đều hữu hạn chiều trên $K$. Cuối cùng, $H$ là một không gian con tuyến tính của Hom$_K(S,T)$; vì thế nó cũng hữu hạn chiều. Công thức (21) khi đó suy ra từ Mệnh đề 11 vì số chiều của $H$ trên $K$ bằng $[H : D][D : K]$ và bằng $[H : E][E : K]$ (II, §1, No. 13, p. 222, Mệnh đề 25). Theo Định lý 1 của VIII, p. 47, nếu $K$ đóng đại số, ta có $D = E = K$. Phần thứ hai của hệ quả khi đó suy ra từ phần thứ nhất.

Cho $A$ và $B$ là các đại số nửa đơn hữu hạn chiều trên một trường giao hoán $K$, và cho $f$ là một đồng cấu K-đại số từ $A$ đến $B$.

Cho $\mathscr{S}(A)$ là tập hợp các lớp của các $A$-môđun đơn; với mọi $\lambda \in \mathscr{S}$ (A), cho $S_{\lambda}$ là một môđun thuộc lớp $\lambda$ và $D_{\lambda}$ là bộ giao hoán của nó. Khi đó $D_{\lambda}$ là một đại số bậc hữu hạn trên $K$; ta ký hiệu bậc này là $d_{\lambda}$. Ta định nghĩa $\mathscr{S}$(B), $T_\mu$, $E_\mu$, và $e_\mu$ cho $\mu$ trong $\mathscr{S}(B)$ tương tự. Nhóm Grothendieck $K_0(A)$ có họ $([S_{\lambda}])_{\lambda\in\mathscr{S}(A)}$ làm một cơ sở, và $K_0(B)$ có $([T_\mu])_{\mu\in\mathscr{S}(B)}$ làm một cơ sở. Cho $(a_{\mu\lambda})$ là ma trận của $f^*: K_0(A)\rightarrow K_0(B)$ và $(b_{\lambda \mu})$ là ma trận của $f_*: K_0(B)\rightarrow K_0(A)$ theo các cơ sở này. Theo định nghĩa, ta có

$$
a_{\mu\lambda}= [f^*(S_{\lambda}) : T_\mu],b_{\lambda \mu}= [f_*(T_\mu) : S_{\lambda}] \tag{23}
$$

với $\lambda$ trong $\mathscr{S}(A)$ và $\mu$ trong $\mathscr{S}(B)$. Ta ký hiệu số chiều của không gian vectơ Hom$_A(S_{\lambda}, f_*(T_\mu))$ trên trường $K$ là $h_{\lambda \mu}$. Theo hệ quả trên, ta có

$$
h_{\lambda \mu}=e_\mu a_{\mu\lambda}=d_{\lambda}b_{\lambda \mu} \tag{24}
$$

Khi trường K là đóng đại số, ta có $d_{\lambda}=e_\mu= 1$; do đó, ta có

$$
a_{\mu\lambda}=b_{\lambda \mu}=h_{\lambda \mu} \tag{25}
$$

Nói cách khác, các ma trận của $f_*$ và $f^*$ theo các cơ sở đã cho của $K_0(A)$ và $K_0(B)$ là chuyển vị của nhau.

### 12. Trường hợp các vành đơn

Cho A và B là các vành đơn và $f$ là một đồng cấu từ A đến B. Cho S là một A-môđun đơn và T là một B-môđun đơn. Đặt

(26) $i(f) = [f^*(S) : T] =$ độ dài$_B(f^*(S))$;

ta gọi lực lượng $i(f)$ là chỉ số của $f$. Khi A là một vành con của B và $f$ là đơn ánh chính tắc của A vào B, ta viết $i(B,A)$ thay cho $i(f)$, và ta gọi lực lượng này là chỉ số của A trong B. Ta định nghĩa độ cao $h(f)$ của $f$ tương tự:

(27) $h(f) = [f_*(T) : S] =$ độ dài$_A(f_*(T))$.

Khi A là một vành con của B và $f$ là đơn ánh chính tắc của A vào B, ta viết $h(B,A)$ cho $h(f)$, và ta gọi nó là độ cao của A trong B.

A-môđun S là đơn sinh, nên B-môđun $f^*(S) = B\otimes_AS$ cũng đơn sinh. Suy ra $i(f)$ hữu hạn và do đó là một số nguyên. Cho M là một A-môđun. Kí hiệu độ dài của nó là $\mathfrak{a}$; khi đó M đẳng cấu với $S^{(\mathfrak{a})}$. Do đó, B-môđun $f_*(M)$ đẳng cấu với $f_*(S)^{(\mathfrak{a})}$. Theo định nghĩa của $i(f)$, do đó ta có

(28) độ dài$_B(f^*(M)) =i(f)$ độ dài$_A(M)$.

Các $\mathbf{Z}$-môđun $K_0(A)$ và $K_0(B)$ là tự do có chiều 1, với các cơ sở tương ứng là [S] và [T], và ta có

$$
f^*([S]) =i(f)[T] \tag{29}
$$

Xét riêng $M = A_s$; khi đó $f^*(A_s) = B\otimes_AA_s$ đẳng cấu với $B_s$ (II, §3, No. 4, p. 249), nên

(30) $i(f) =$ độ dài(B)$/$ độ dài(A).

Theo Định lý của Wedderburn (VIII, p. 120, Định lý 1), tồn tại các số nguyên $m\geqslant$ 1 và $n\geqslant 1$ cùng các trường D và E sao cho A đẳng cấu với $\mathbf{M}_m(D)$ và B đẳng cấu với $\mathbf{M}_n(E)$. Theo công thức (30), ta có $i(f) =n/m$; nói riêng, $m$ chia hết $n$.

Cho N là một B-môđun; kí hiệu độ dài của nó là $\mathfrak{a}$. Khi đó N đẳng cấu với $T^{(\mathfrak{a})}$, nên A-môđun $f_*(N)$ đẳng cấu với $f_*(T)^{(\mathfrak{a})}$; theo định nghĩa của $h(f)$, ta có

(31) độ dài$_A(f_*(N)) =h(f)$ độ dài$_B(N)$.

Như ta đã thấy (VIII, p. 124, Mệnh đề 5), $f$ biến B thành một A-môđun tự do và mọi cơ sở của môđun này đều có cùng lực lượng, kí hiệu là $[B : A]_s$ và gọi là bậc (trái) của B trên A. A-môđun $f_*(B_s)$ đẳng cấu với $A_s^{[B:A]_s}$, nên có độ dài $[B : A]_s$ độ dài(A). Theo công thức (30) và công thức (31) áp dụng cho trường hợp riêng $N = B_s$, do đó ta có

$$
[B : A]_s=i(f)h(f) \tag{32}
$$

Bây giờ giả sử rằng B là một A-môđun hữu hạn sinh, tức là $[B : A]_s$ hữu hạn. Khi đó $h(f)$ hữu hạn theo công thức (32). Chúng ta đã định nghĩa (VIII, p. 202) một đồng cấu nhóm $f_*$ từ $K_0(B)$ đến $K_0(A)$; ta có

$$
f_*([T]) =h(f)[S] \tag{33}
$$

Giả sử rằng A và B là các đại số hữu hạn chiều trên một trường giao hoán K và rằng $f$ là K-tuyến tính. Như trước, tồn tại các số nguyên $m\geqslant 1$ và $n\geqslant 1$, các K-đại số D và E là các trường, và các đẳng cấu K-đại số từ A đến $\mathbf{M}_m(D)$ và từ B đến $\mathbf{M}_n(E)$. Đặt $d= [D : K]$ và $e= [E : K]$. Khi đó ta có các hệ thức

$$
[A : K] =m^2d ,[B : K] =n^2e ,[B : A]_s=\frac{n^2e}{m^2d}
$$

và, theo các công thức (30) và (32), các hệ thức

$$
i(f) =\frac{n}{m},h(f) =\frac{ne}{md}
$$

Khi trường K là đóng đại số, ta có $d=e= 1$ và do đó $i(f) =h(f)$ và $[B : A]_s=i(f)^2$.

Cho A, B, và C là các vành đơn, và cho $f: A\rightarrow B$ và $g: B\rightarrow C$ là các đồng cấu. Cho S là một A-môđun đơn. Các C-môđun $(g\circ f)^*(S)$ và $g^*(f^*(S))$ là đẳng cấu; do đó, theo các công thức (26) và (28), ta có

$i(g\circ f) =$ long$_C(g^*(f^*(S))) =i(g)$ long$_B(f^*(S)) =i(g)i(f)$.

Ta cũng có thể chứng minh đẳng thức $h(g\circ f) =h(g)h(f)$ tương tự. Khi A là một vành con của B và B là một vành con của C, và ta lấy các nhúng chính tắc cho $f$ và $g$, thì các đẳng thức này cho

$$
i(C,A) =i(C,B)i(B,A),h(C,A) =h(C,B)h(B,A) \tag{34}
$$

#### Mệnh đề 12 {#alg-viii-s11-prop-12 .statement tag=00DR}

Cho B là một vành đơn và A là một vành con đơn của B. Giả sử rằng B là một A-môđun trái hữu hạn sinh. Cho M là một B-môđun trái hữu hạn sinh khác không. Đặt $A'=$ End$_A(M)$ và $B'=$ End$_B(M)$. Khi đó $B'$ là một vành con của $A'$, các vành $A'$ và $B'$ là đơn, $A'$ là một $B'$-môđun trái hữu hạn sinh, và ta có các đẳng thức

$$
i(A',B') =h(B,A),h(A',B') =i(B,A),[A': B']_s= [B : A]_s
$$

Theo Mệnh đề 4 của VIII, p. 123, vành $A'$ là đơn, M là một $A'$-môđun có độ dài hữu hạn, và ta có

long$_A(M) =$ long(A$'$), long$_{A'}(M) =$ long(A).

Vì cùng những lý do đó, vành $B'$ là đơn, và ta có

long$_B(M) =$ long(B$'$), long$_{B'}(M) =$ long(B).

Theo các công thức (31) và (30), do đó ta có

$h(B,A) =$ long$_A(M)/$ long$_B(M) =$ long(A$'$)$/$ long(B$'$) $=i(A',B')$;

đẳng thức $h(A',B') =i(B,A)$ có thể được thiết lập tương tự. Từ đó, ta suy ra

$$
[A': B']_s=i(A',B')h(A',B') =h(B,A)i(B,A) = [B : A]_s
$$

sử dụng công thức (32). Đặc biệt, $A'$ là một $B'$-môđun trái hữu hạn sinh.

### Bài tập {#alg-viii-s11-exercises}

Xem các [bài tập cho § 11](exercises/s11/).
