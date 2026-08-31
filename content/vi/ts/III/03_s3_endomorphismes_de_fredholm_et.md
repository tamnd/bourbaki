---
book: ts
book_title: Théories spectrales
chapter: III
chapter_title: APPLICATIONS LINÉAIRES COMPACTES ET PERTURBATIONS
section: 3
section_title: Endomorphismes de Fredholm et endomorphismes de Riesz
lang: vi
source: ts-iii-v-fr
book_pages: TS III.39-TS III.55, TS III.120-TS III.122
pdf_pages: 0053-0069, 0134-0136
extraction: native
subsections:
    - "no": 1
      title: Morphismes stricts et applications linéaires de rang fini
      page: 39
      pdf_page: 53
    - "no": 2
      title: Applications de Fredholm
      page: 40
      pdf_page: 54
    - "no": 3
      title: Indice d’une application de Fredholm
      page: 43
      pdf_page: 57
    - "no": 4
      title: Endomorphismes de Riesz
      page: 45
      pdf_page: 59
    - "no": 5
      title: Applications de Fredholm et applications de Riesz entre espaces de Fréchet
      page: 52
      pdf_page: 66
    - "no": 6
      title: Caractérisation spectrale des endomorphismes de Riesz
      page: 53
      pdf_page: 67
statements: 31
exercises: 8
content_sha256: 9eb607e29f9e08cf000c7d1a984af09b2bb2a344a2b9a5a20a3a95c3da531193
translated_from: content/en-mt/ts/III/03_s3_endomorphismes_de_fredholm_et.md
source_lang: en-mt
translation_method: machine
source_content_sha256: 98281531585184fdb511b806baf9788ce825200769240d82ff23b99318d7a1d4
translation_model: gpt-5.4
translation_run: translate-vi-a6053766
glossary_version: 34
glossary_terms_sha256: 227a2d5efe659d9b279502932beb3de54bd13553fe4a0d3caf5488ba1a0622ab
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 3. CÁC NỘI CẤU FREDHOLM VÀ CÁC NỘI CẤU RIESZ

### 1. Các cấu xạ ngặt và các ánh xạ tuyến tính hạng hữu hạn

#### Mệnh đề 1 {#ts-iii-s3-prop-1 .statement tag=02RE}

Cho E và F là các không gian lồi địa phương, $E_1$ là một không gian con đóng có đối chiều hữu hạn của E và $u$ là một ánh xạ tuyến tính liên tục từ E vào F. Để $u$ là một cấu xạ ngặt có ảnh đóng, điều kiện cần và đủ là $u|E_1$ cũng như vậy.

Trước hết giả sử rằng ánh xạ tuyến tính $u|E_1$ là đơn ánh. Khi đó ta có $E_1\cap$ Ker($u$) $=\{0\}$, nên Ker($u$) có số chiều hữu hạn. Gọi S là một không gian con vectơ của E bổ sung với $E_1+$ Ker($u$). Không gian E là tổng trực tiếp tôpô của $E_1$, Ker($u$) và S (EVT, I, p. 15, cor. 4 and prop. 3). Nếu $u$ là một cấu xạ ngặt có ảnh đóng, thì bằng hạn chế nó xác định một đẳng cấu từ $E_1\oplus S$ lên một không gian con vectơ đóng của F, và a fortiori một đẳng cấu từ $E_1$ lên một không gian con vectơ đóng của F. Ngược lại, giả sử rằng bằng hạn chế $u$ xác định một đẳng cấu từ $E_1$ lên $u(E_1)$ và rằng $u(E_1)$ đóng trong F. Ta có $u(E) =u(E_1)\oplus u(S)$. Suy ra $u(E)$ là tổng trực tiếp tôpô của $u(E_1)$ và $u$(S), và đóng trong F (loc. cit.). Vì $u(E_1)$ đóng và ta có $u(E_1)\cap u(S) =\{0\}$, nên không gian $u(S)$ là tách biệt và $u$ xác định bằng hạn chế một đẳng cấu từ S lên $u(S)$ (EVT, I, p. 15, cor. de la prop. 3), do đó cũng từ $E_1\oplus S$ lên $u(E)$. Điều này chứng minh rằng $u$ là một cấu xạ ngặt có ảnh đóng.

Chuyển qua trường hợp tổng quát. Đặt $N = E_1\cap$ Ker($u$) và $G = E/N$. Không gian lồi địa phương $E_1/N$ được đồng nhất với một không gian con vectơ đóng có đối chiều hữu hạn $G_1$ của G. Gọi $v: G\rightarrow F$ là ánh xạ tuyến tính liên tục suy ra từ $u$ bằng cách chuyển qua thương. Để $u$ (tương ứng, $u|E_1$) là một cấu xạ ngặt có ảnh đóng, điều kiện cần và đủ là $v$ (tương ứng, $v|G_1$) cũng như vậy. Điều này quy về trường hợp đã xét.

#### Hệ quả 1 {#ts-iii-s3-prop-1-cor-1 .statement tag=02RF}

Giả sử rằng F là tách biệt. Cho $v\in \mathscr{L}^f(E; F)$. Nếu $u$ là một cấu xạ ngặt có ảnh đóng từ E vào F, thì $u+v$ cũng vậy.

Vì F là tách biệt, hạt nhân của $v$ là một không gian con vectơ đóng của E; nó có đối chiều hữu hạn trong E và $u+v$ có cùng hạn chế như $u$ trên Ker($v$). Do đó hệ quả suy ra từ mệnh đề.

#### Hệ quả 2 {#ts-iii-s3-prop-1-cor-2 .statement tag=02RG}

Cho T là một không gian con vectơ tách biệt có số chiều hữu hạn của F. Gọi $\pi : F\rightarrow F/T$ là toàn cấu chính tắc. Để $u$ là một cấu xạ ngặt có ảnh đóng, điều kiện cần và đủ là $\pi \circ u$ cũng như vậy.

Ánh xạ đồng nhất của T vào chính nó kéo dài thành một ánh xạ liên tục $q: F\rightarrow T$ (EVT, II, p. 26, nhận xét). Hạt nhân S của $q$ là một không gian con bù tôpô đóng của T. Gọi $p: F\rightarrow F$ là phép chiếu có ảnh là S liên kết với phân tích $F = T\oplus S$. Để $\pi \circ u$ là một cấu xạ ngặt có ảnh đóng, điều kiện cần và đủ là $p\circ u$ có tính chất đó. Bây giờ $p\circ u$ và $u$ có cùng hạn chế trên $\overset{-1}{u}$(S), là một không gian con vectơ đóng đối chiều hữu hạn của E, và mệnh đề suy ra từ mệnh đề.

### 2. Ánh xạ Fredholm

Cho E và F là các không gian lồi địa phương. Trong số này, ta ký hiệu bởi $u\equiv v$ quan hệ đồng dư modulo $\mathscr{L}^f(E; F)$ của các phần tử $u$ và $v$ của $\mathscr{L}(E; F)$.

Nếu G là một không gian lồi địa phương, và nếu $u'$ và $v'$ là các phần tử của $\mathscr{L}(F; G)$, thì các quan hệ $u\equiv v$ và $u'\equiv v'$ suy ra quan hệ $u'\circ u\equiv v'\circ v$.

Một phần tử $w$ của $\mathscr{L}(F; E)$ được gọi là một nghịch đảo giả của phần tử $u$ của $\mathscr{L}(E; F)$ nếu ta có $w\circ u\equiv 1_E$ và $u\circ w\equiv 1_F$.

Giả sử rằng $w$ là một nghịch đảo giả của $u$. Nếu $u_1$ là một phần tử của $\mathscr{L}(E; F)$ và $w_1$ là một phần tử của $\mathscr{L}(F; E)$ sao cho $u_1\equiv u$ và $w_1\equiv w$, thì $w_1$ là một nghịch đảo giả của $u_1$ vì $w\circ u\equiv w_1\circ u_1$ và $u\circ w\equiv u_1\circ w_1$.

Nếu $w$ và $w_1$ là các nghịch đảo giả của $u$, thì $w_1\equiv w$ vì

$$
w_1= 1_E\circ w_1\equiv w\circ u\circ w_1\equiv w\circ 1_F=w
$$

#### Định nghĩa 1 {#ts-iii-s3-def-1 .statement tag=02RH}

Cho E và F là các không gian lồi địa phương. Một phần tử $u$ của $\mathscr{L}(E; F)$ được gọi là một ánh xạ Fredholm[^1] nếu nó có một nghịch đảo giả. Một ánh xạ Fredholm từ E vào E được gọi là một tự đồng cấu Fredholm của E.

Ta sẽ ký hiệu bởi $\mathscr{F}(E; F)$ tập hợp các ánh xạ Fredholm từ E vào F, và bởi $\mathscr{F}(E)$ tập hợp các tự đồng cấu Fredholm của E.

#### Nhận xét {#ts-iii-s3-n2-rem-1 .statement tag=02RI}

Cho E, F và G là các không gian lồi địa phương, $u: E\rightarrow F$ và $v: F\rightarrow G$ là các ánh xạ tuyến tính liên tục.

1) Giả sử rằng $u$ là một ánh xạ Fredholm và gọi $u_1$ là một nghịch đảo giả của $u$. Vì $u$ là một nghịch đảo giả của $u_1$, ánh xạ $u_1$ là một ánh xạ Fredholm.

2) Giả sử rằng $u$ và $v$ là các ánh xạ Fredholm, và gọi $u_1$ (tương ứng $v_1$) là một nghịch đảo giả của $u$ (tương ứng của $v$). Khi đó $v\circ u$ là một ánh xạ Fredholm từ E vào G và $u_1\circ v_1$ là một nghịch đảo giả của $v\circ u$. Thật vậy, ta tính được

$$
(u_1\circ v_1)\circ (v\circ u) =u_1\circ (v_1\circ v)\circ u\equiv u_1\circ 1_F\circ u=u_1\circ u\equiv 1_E
$$

$$
(v\circ u)\circ (u_1\circ v_1) =v\circ (u\circ u_1)\circ v_1\equiv v\circ 1_F\circ v_1=v\circ v_1\equiv 1_G
$$

3) Giả sử rằng $u$ và $v\circ u$ là các ánh xạ Fredholm, và gọi $w_1$ là một nghịch đảo giả của $v\circ u$. Khi đó $v$ là một ánh xạ Fredholm và $u\circ w_1$ là một nghịch đảo giả của $v$.

Thật vậy, theo nhận xét thứ nhất, $w_1$ là một ánh xạ Fredholm. Gọi $u_1$ là một nghịch đảo giả của $u$; theo nhận xét thứ hai, $u\circ w_1$ là một ánh xạ Fredholm và $(v\circ u)\circ u_1$ là một nghịch đảo giả của nó. Ta có $u\circ u_1\equiv 1_F$, do đó $v\circ u\circ u_1\equiv v$; điều này chứng minh mệnh đề.

4) Giả sử rằng $v$ và $v\circ u$ là các ánh xạ Fredholm, và gọi $w_1$ là một nghịch đảo giả của $v\circ u$. Khi đó $u$ là một ánh xạ Fredholm và $w_1\circ v$ là một nghịch đảo giả của $u$.

Chứng minh là tương tự như chứng minh của nhận xét trước.

#### Bổ đề 1 {#ts-iii-s3-lem-1 .statement tag=02RJ}

Cho E và F là các không gian lồi địa phương và gọi $u$ là một ánh xạ Fredholm từ E vào F. Hạt nhân và đối hạt nhân của $u$ có chiều hữu hạn.

Gọi $v: F\rightarrow E$ là một nghịch đảo giả của $u$. Hạt nhân của $u$ được chứa trong ảnh của ánh xạ tuyến tính hạng hữu hạn $1_E-v\circ u$, vì thế có chiều hữu hạn. Ảnh của $u$ chứa hạt nhân của ánh xạ tuyến tính hạng hữu hạn $1_F-u\circ v$, vì thế có đối chiều hữu hạn trong F.

#### Mệnh đề 2 {#ts-iii-s3-prop-2 .statement tag=02RK}

Cho E và F là các không gian lồi địa phương tách được và gọi $u$ là một phần tử của $\mathscr{L}(E; F)$. Các tính chất sau là tương đương:

(i) Ánh xạ $u$ là một ánh xạ Fredholm;

(ii) Ánh xạ $u$ là một cấu xạ ngặt, hạt nhân của nó có chiều hữu hạn, ảnh của nó đóng và có đối chiều hữu hạn trong F ;

(iii) Tồn tại các không gian con vectơ đóng đối chiều hữu hạn $E_1$ của E và $F_1$ của F sao cho $u$ xác định, bằng cách chuyển qua các không gian con, một đẳng cấu của $E_1$ lên $F_1$;

(iv) Tồn tại các phân tích thành tổng trực tiếp tôpô $E = E_1\oplus E_2$ và $F = F_1\oplus F_2$ sao cho $E_2$ và $F_2$ có chiều hữu hạn, $u$ triệt tiêu trên $E_2$ và xác định, bằng cách chuyển qua các không gian con, một đẳng cấu của $E_1$ lên $F_1$.

(i) $=\Rightarrow$ (iii): Cho $v$ là một nghịch đảo giả của $u, E_1$ là hạt nhân của $1_E-v\circ u$ và $F_1$ là hạt nhân của $1_F-u\circ v$. Vì các ánh xạ tuyến tính $1_E-v\circ u$ và $1_F-u\circ v$ là liên tục và có hạng hữu hạn, nên $E_1$ và $F_1$ lần lượt là các không gian con vectơ đóng của E và F và có đối chiều hữu hạn. Cho $x\in E_1$. Ta có

$$
(1_F-u\circ v)(u(x)) =u((1_E-v\circ u)(x)) =u(0) = 0
$$

do đó $u(x)\in F_1$. Vì vậy $u(E_1)\subset F_1$; tương tự, $v(F_1)\subset E_1$. Khi đó các ánh xạ tuyến tính liên tục $u_1: E_1\rightarrow F_1$ và $v_1: F_1\rightarrow E_1$ cảm sinh bởi $u$ và $v$ là các đẳng cấu nghịch đảo của nhau, vì $v\circ u$ và $1_E$ (resp. $u\circ v$ và $1_F$) trùng nhau trên $E_1$ (resp. trên $F_1$).

(iii) $=\Rightarrow$ (ii): Cho $E_1$ và $F_1$ thỏa mãn giả thiết của (iii). Ta có $E_1\cap$ Ker($u$) $=\{0\}$ và $F_1\subset$ Im($u$), do đó Ker($u$) hữu hạn chiều và Im($u$) đóng và có đối chiều hữu hạn trong F. Suy ra từ Mệnh đề 1 của III, p. 39 rằng ánh xạ $u$ là một cấu xạ ngặt.

(ii) $=\Rightarrow$ (iv): Giả sử điều kiện (ii) được thỏa mãn. Không gian con vectơ đóng $E_2=$ Ker($u$) của E là hữu hạn chiều, và tồn tại một không gian con vectơ $E_1$ của E là một phần bù tôpô của $E_2$ (TVS, II, p. 27, Hệ quả 2). Không gian con vectơ $F_1=$ Im($u$) của F là đóng và có đối chiều hữu hạn, và nhận một phần bù tôpô $F_2$ trong F. Theo Mệnh đề 1 của III, p. 39, ánh xạ $u|E_1$ là một cấu xạ ngặt, do đó $u$ cảm sinh một đẳng cấu của $E_1$ lên $F_1$.

(iv) $=\Rightarrow$ (i): Với các giả thiết của (iv), ánh xạ tuyến tính từ F vào E trùng với $u^{-1}_1$ trên $F_1$ và bằng không trên $F_2$ là một nghịch đảo giả của $u$.

#### Nhận xét 5 {#ts-iii-s3-n2-rem-5 .statement tag=02RL}

Cho E, F là các không gian lồi địa phương tách được và $u: E\rightarrow F$ là một ánh xạ Fredholm. Nếu $u$ là song ánh, thì $u$ là một đẳng cấu (thực vậy, $u$ là một cấu xạ ngặt theo Mệnh đề 2, (ii)).

### 3. Chỉ số của một Ánh xạ Fredholm

Cho E, F và G là các không gian lồi địa phương.

Cho $u: E\rightarrow F$ là một ánh xạ Fredholm. Các không gian vectơ Ker($u$) và Coker($u$) là hữu hạn chiều (Bổ đề 1 của III, p. 41). Nhớ lại rằng số nguyên

(1) dim Coker($u$)$-$ dim Ker($u$) $=$ codim$_F$ Im($u$)$-$ dim Ker($u$)

được gọi là chỉ số của $u$ và được ký hiệu là ind($u$) (A, V, p. 126).

Nếu $u: E\rightarrow F$ và $v: F\rightarrow G$ là các ánh xạ Fredholm, thì điều đó cũng đúng với $v\circ u($III, p. 41, nhận xét 2), và ta có (A, V, p. 127, bổ đề 2)

(2) ind($v\circ u$) $=$ ind($v$) $+$ ind($u$).

Giả sử E và F tách biệt và $u: E\rightarrow$ F là một ánh xạ Fredholm; dùng các ký hiệu của điều kiện (iv) của mệnh đề 2 ở III, p. 42. Khi đó ta có ind($u$) $=$ dim(F$_2$)$-$ dim(E$_2$). Trang bị đối ngẫu của mỗi không gian này với tôpô yếu (tương ứng, tôpô compact, tôpô hội tụ đều trên các tập bị chặn). Khi đó $E'$ được đồng nhất với tổng trực tiếp tôpô của $E'_1$ và $E'_2$, và $F'$ với tổng trực tiếp tôpô của $F'_1$ và $F'_2$, và $^tu$ gây ra một đẳng cấu của $F'_1$ lên $E'_1$ và triệt tiêu trên $F'_2$. Do đó chuyển vị $^tu: F'\rightarrow E'$ là một ánh xạ Fredholm (loc. cit.). Hạt nhân của $^tu$ là $F'_2$, và chiều của nó là chiều của $F_2$, nghĩa là chiều của đối hạt nhân của $u$. Vậy

(3) ind($u$) $=$ dim Ker($^tu$)$-$ dim Ker($u$). Hơn nữa, ảnh của $^tu$ là $E'_1$, và do đó chiều của đối hạt nhân của $^tu$ bằng chiều của $E'_2$, tức là chiều của hạt nhân $E_2$ của $u$. Ta suy ra

(4) ind($^tu$) $=-$ ind($u$).

Giả sử E và F tách biệt và $u: E\rightarrow$ F là một ánh xạ Fredholm có chỉ số 0. Khi đó $u$ là một cấu xạ ngặt theo mệnh đề 2 của III, p. 42. Vì dim Ker($u$) $=$ codim$_F$ Im($u$), ánh xạ $u$ là một đẳng cấu ngay khi nó là đơn ánh hoặc toàn ánh.

#### Mệnh đề 3 {#ts-iii-s3-prop-3 .statement tag=02RM}

Cho E và F là các không gian lồi địa phương và $u\in \mathscr{L}(E; F)$. Gọi $E_1($tương ứng $F_1)$ là một không gian con đóng có đối chiều hữu hạn của E (tương ứng của F). Giả sử rằng $u$ ánh xạ $E_1$ vào $F_1$ và ký hiệu bởi $u_1\in \mathscr{L}(E_1; F_1)$ ánh xạ trùng với $u$ trên $E_1$. Để $u$ là một ánh xạ Fredholm, điều kiện cần và đủ là $u_1$ là như vậy. Khi đó ta có

(5) ind($u$)$-$ ind($u_1$) $=$ codim$_F(F_1)-$ codim$_E(E_1)$.

Gọi $i: E_1\rightarrow E$ và $j: F_1\rightarrow F$ là các đơn ánh chính tắc. Chúng là các ánh xạ Fredholm, và ta có

ind($i$) $=$ codim$_E(E_1)$, ind($j$) $=$ codim$_F(F_1)$.

Vì $j\circ u_1=u\circ i$, ta thấy rằng $u$ là một ánh xạ Fredholm khi và chỉ khi $u_1$ là như vậy (Nhận xét 3 và 4 của III, p. 41). Nếu đúng như thế, ta có

ind($j$) $+$ ind($u_1$) $=$ ind($j\circ u_1$) $=$ ind($u\circ i$) $=$ ind($u$) $+$ ind($i$),

do đó có công thức (5).

#### Mệnh đề 4 {#ts-iii-s3-prop-4 .statement tag=02RN}

Cho E và F là các không gian lồi địa phương tách được, $u: E\rightarrow F$ là một ánh xạ Fredholm, và $\widehat{u}:\widehat{E}\rightarrow \widehat{F}$ là mở rộng của $u$ lên các đầy đủ hóa. Khi đó $\widehat{u}$ là một ánh xạ Fredholm và ta có Ker($\widehat{u}$) $=$ Ker($u$) và ind($\widehat{u}$) $=$ ind($u$).

Chúng ta dùng ký hiệu của điều kiện (iv) của Mệnh đề 2 của III, p. 42. Vì các không gian vectơ $E_2$ và $F_2$ là hữu hạn chiều nên chúng đầy đủ. Bổ sung của $E_1$ (resp. $F_1$) được đồng nhất với bao đóng của $E_1$ trong $\widehat{E}$ (resp. của $F_1$ trong $\widehat{F}$), và $\widehat{E}$ (resp. $\widehat{F}$) là tổng trực tiếp tôpô của $\widehat{E}_1$ và $E_2$ (resp. $\widehat{F}_1$ và $F_2$). Ánh xạ tuyến tính $\widehat{u}$ xác định, bằng hạn chế, một đẳng cấu từ $\widehat{E}_1$ lên $\widehat{F}_1$ và triệt tiêu trên $E_2$. Khi đó mệnh đề suy ra từ hệ quả (iv)$\Rightarrow$(i) của chỗ đã dẫn.

### 4. Các Tự Đồng Cấu Riesz

Cho E là một không gian vectơ và $u$ là một tự đồng cấu của E.

Dãy (Ker($u^n$))$_{n\in\mathbf{N}}$ các không gian con vectơ của E là tăng; hợp của chúng là một không gian con của E ổn định dưới $u$ và được gọi là không gian lũy linh của $u$.

Dãy (Im($u^n$))$_{n\in\mathbf{N}}$ các không gian con vectơ của E là giảm; giao của chúng là một không gian con của E ổn định dưới $u$ và được gọi là đối không gian lũy linh của $u$.

#### Bổ đề 2 {#ts-iii-s3-lem-2 .statement tag=02RO}

Cho E là một không gian vectơ và $u$ là một tự đồng cấu của E có một chỉ số (A, V, p. 126).

Nếu hai trong ba tính chất sau được thỏa mãn thì tính chất thứ ba cũng được thỏa mãn:

(i) Tự đồng cấu $u$ có chỉ số bằng 0;

(ii) Không gian lũy linh N của $u$ là hữu hạn chiều;

(iii) Đối không gian lũy linh I của $u$ có đối chiều hữu hạn.

Với mọi số nguyên $n\geqslant 0$, tự đồng cấu $u^n$ có một chỉ số, bằng $n$ ind($u$) (A, V, p. 127, Bổ đề 2). Dãy (dim(Ker($u^n$)))$_{n\in\mathbf{N}}$ các số nguyên tự nhiên là tăng; để nó dừng, điều kiện cần và đủ là không gian lũy linh của $u$ hữu hạn chiều. Dãy (codim$_E$(Im($u^n$)))$_{n\in\mathbf{N}}$ các số nguyên tự nhiên là tăng; để nó dừng, điều kiện cần và đủ là đối không gian lũy linh có số chiều hữu hạn. Giả sử điều kiện (i) được thỏa mãn; khi đó quan hệ

dim(Ker($u^n$))$-$ codim$_E$(Im($u^n$)) $=$ ind($u^n$) $=n$ ind($u$) $= 0$

suy ra tính tương đương của các điều kiện (ii) và (iii). Ngược lại, nếu các điều kiện (ii) và (iii) được thỏa mãn thì công thức này suy ra rằng dãy $(n$ ind($u$))$_{n\in\mathbf{N}}$ là dừng, do đó $u$ có chỉ số bằng không.

#### Bổ đề 3 {#ts-iii-s3-lem-3 .statement tag=02RP}

Cho E là một không gian vectơ và $u$ là một tự đồng cấu của E có một chỉ số. Giả sử rằng chỉ số của $u$ bằng không. Gọi N là không gian lũy linh của $u$ và I là đối không gian lũy linh của nó.

a) Khi đó không gian E là tổng trực tiếp của các không gian con N và I (phân rã Weyr-Fitting, cf. A, VIII, §2, n$^o2$, p. 25).

b) Tự đồng cấu $u$ cảm sinh, khi chuyển qua các không gian con, một tự đồng cấu lũy linh của N và một tự đẳng cấu $u_I$ của I.

c) Ký hiệu $v$ là tự đồng cấu của E bằng không trên N và trùng với $u^{-1}_I$ trên I. Ta có $u\circ v=v\circ u$ và tự đồng cấu $1_E-u\circ v$ là phép chiếu có ảnh là N và hạt nhân là I.

d) Mọi tự đồng cấu của E giao hoán với $u$ đều bảo toàn N và I, và giao hoán với $v$.

Tự đồng cấu $u$ thỏa mãn các tính chất của bổ đề trước.

Lấy $n\in \mathbf{N}$ sao cho Ker($u^n$) $= N$. Khi đó Ker($u^m$) $=$ Ker($u^n$) với mọi số nguyên $m\geqslant n$; vì ind($u^m$) $=m$ ind($u$) $= 0$, điều này kéo theo Im($u^m$) $=$ Im($u^n$) với $m\geqslant n$, do đó I = Im($u^n$). Từ A, VIII, p. 25, prop. 2 suy ra rằng các khẳng định a) và b) được thỏa mãn.

Với mọi $x\in N$, ta có $v(x) = 0$ và $u(x)\in N$, do đó $u(v(x)) = 0$ và $v(u(x)) = 0$. Với mọi $x\in I$, ta có $u(v(x)) =v(u(x)) =x$. Điều này suy ra $u\circ v=v\circ u$ và $1_E-u\circ v$ là phép chiếu có ảnh là N và hạt nhân là I.

Cho $w$ là một tự đồng cấu của E giao hoán với $u$. Lấy $n\in \mathbf{N}$ sao cho N = Ker($u^n$) và I = Im($u^n$). Cho $x\in N$; ta có $u^n(w(x)) =w(u^n(x)) = 0$, do đó $w(x)\in N$. Cho $x\in I$; tồn tại $y\in E$ sao cho $x=u^n(y)$; khi đó, $w(x) =w(u^n(y)) =u^n(w(y))\in I$. Điều này chứng tỏ rằng $w$ bảo toàn N và I.

Cuối cùng, ta chứng minh rằng $w$ và $v$ giao hoán được. Với mọi $x$ trong N, ta có $v(w(x)) = 0 =w(v(x))$. Cho $x\in I$; các phần tử $v(w(x))$ và $w(v(x))$ của E thuộc I và ảnh của chúng qua $u$ đều bằng $w(x)$, do đó chúng bằng nhau. Theo tính tuyến tính, điều này suy ra rằng $v$ và $w$ giao hoán.

#### Nhận xét {#ts-iii-s3-n4-rem-1 .statement tag=02RQ}

Giả sử tồn tại một số nguyên $n\geqslant 0$ sao cho Ker($u^n$) $=$ Ker($u^{n+1}$) (resp. Im($u^n$) $=$ Im($u^{n+1}$)); khi đó có Ker($u^m$) $=$ Ker($u^n$) (resp. Im($u^m$) $=$ Im($u^n$)) với mọi số nguyên $m\geqslant n$.

Giả sử $u$ có chỉ số không. Với mọi số nguyên $n\geqslant 0$, ta có

$n$ ind($u$) $=$ ind($u^n$) $=$ codim$_E$(Im($u^n$))$-$ dim(Ker($u^n$)).

Do đó các điều kiện Ker($u^n$) $=$ Ker($u^{n+1}$) và Im($u^n$) $=$ Im($u^{n+1}$) là tương đương. Khi các điều kiện ấy được thỏa mãn, không gian vectơ E là tổng trực tiếp của Ker($u^n$) và của Im($u^n$) (A, VIII, p. 25, mệnh đề 2), không gian Ker($u^n$) là hữu hạn chiều, và $u$ gây ra, bằng cách chuyển qua không gian con, một tự đẳng cấu của Im($u^n$).

#### Định nghĩa 2 {#ts-iii-s3-def-2 .statement tag=02RR}

Cho E là một không gian lồi địa phương tách rời. Một tự đồng cấu Riesz của E có nghĩa là mọi tự đồng cấu Fredholm của E mà không gian không hóa là hữu hạn chiều và đối không gian không hóa là đối chiều hữu hạn.

#### Mệnh đề 5 {#ts-iii-s3-prop-5 .statement tag=02RS}

Cho E là một không gian lồi địa phương tách rời. Mọi tự đồng cấu Riesz của E đều có chỉ số không.

Điều này suy ra từ định nghĩa và bổ đề 2.

#### Ví dụ 1 {#ts-iii-s3-n4-exa-1 .statement tag=02RT}

Mọi tự đẳng cấu của E đều là một tự đồng cấu Riesz của E. Nếu E là hữu hạn chiều, mọi phần tử của $\mathscr{L}(E)$ đều là một tự đồng cấu Riesz của E.

#### Ví dụ 2 {#ts-iii-s3-n4-exa-2 .statement tag=02RU}

Nếu $(E_i)_{i\in I}$ là một họ hữu hạn các không gian lồi địa phương tách rời và $u_i$ là một phần tử của $\mathscr{L}(E_i)$ với mọi $i$ trong I, thì tự đồng cấu $u=\bigoplus_{i\in I}u_i$ của không gian lồi địa phương $\bigoplus_{i\in I}E_i$ là một tự đồng cấu Riesz khi và chỉ khi $u_i$ là như vậy với mọi $i$.

#### Ví dụ 3 {#ts-iii-s3-n4-exa-3 .statement tag=02RV}

Cho E là một không gian lồi địa phương tách rời trên $\mathbf{R}$, và gọi $E_{(\mathbf{C})}$ là phức hóa của nó. Cho $u$ là một tự đồng cấu của E. Để $u$ là một tự đồng cấu Riesz, điều cần và đủ là phức hóa của nó $u_{(\mathbf{C})}$ là một tự đồng cấu Riesz của $E_{(\mathbf{C})}$.

#### Mệnh đề 6 {#ts-iii-s3-prop-6 .statement tag=02RW}

Cho E là một không gian lồi địa phương tách rời và gọi $u$ là một tự đồng cấu Riesz của E. Gọi N là không gian không hóa của $u$ và I là đối không gian không hóa của nó.

a) Các không gian con N và I của E là đóng và ổn định dưới $u$, và không gian E là tổng trực tiếp tôpô của chúng;

b) Tự đồng cấu $u$ xác định, bằng hạn chế, một tự đẳng cấu $u_I$ của I;

c) Không gian vectơ N là hữu hạn chiều và $u$ xác định, bằng hạn chế, một tự đồng cấu lũy linh $u_N$ của N;

d) Cho $v$ là phần tử của $\mathscr{L}(E)$ bằng không trên N và trùng với $u^{-1}_I$ trên I. Nó là một tự đồng cấu Riesz của E và một nghịch đảo giả của $u$ giao hoán với $u$. Tự đồng cấu $1_E-u\circ v$ của E là phép chiếu có ảnh là N và hạt nhân là I. Mọi phần tử của $\mathscr{L}(E)$ giao hoán với $u$ đều ổn định hóa N và I, và giao hoán với $v$.

Cho $n$ là một số tự nhiên sao cho Ker($u^n$) $= N$ và Im($u^n$) $= I$. Vì E tách và $u$ liên tục, N = Ker($u^n$) là đóng trong E. Vì $u$ là một tự đồng cấu Fredholm, điều này cũng đúng với $u^n$, và I = Im($u^n$) là đóng (III, p. 42, mệnh đề 2). Theo bổ đề 2, không gian E là tổng trực tiếp của N và I và khi đó mệnh đề a) suy ra từ mệnh đề 3 của EVT, I, p. 15.

Vì I đóng, có đối chiều hữu hạn trong E và ổn định dưới $u$, ánh xạ $u_I: I\rightarrow I$ suy ra từ $u$ là một tự đồng cấu Fredholm (III, p. 44, mệnh đề 3); nó cũng song ánh, nên là một tự đẳng cấu của I (III, p. 42, mệnh đề 2). Điều này chứng minh b), và các khẳng định còn lại suy ra từ bổ đề 2.

Tự đồng cấu $v$ được định nghĩa trong mệnh đề d) của mệnh đề này là một nghịch đảo giả của $u$, được gọi là nghịch đảo giả chính tắc của $u$.

Các tự đồng cấu Riesz có một số tính chất ổn định của các ánh xạ Fredholm.

#### Mệnh đề 7 {#ts-iii-s3-prop-7 .statement tag=02RX}

Cho E là một không gian lồi địa phương tách và cho $u$ là một tự đồng cấu của E.

a) Cho $E_1$ là một không gian con đóng có đối chiều hữu hạn của E, ổn định dưới $u$. Ký hiệu $u_1$ là phần tử của $\mathscr{L}(E_1)$ trùng với $u$ trên $E_1$. Khi đó $u$ là một tự đồng cấu Riesz nếu và chỉ nếu $u_1$ là một tự đồng cấu như vậy;

b) Giả sử rằng $u$ là một tự đồng cấu Fredholm có chỉ số 0. Cho $\widehat{E}$ là hoàn thành của E và cho $\widehat{u}\in \mathscr{L}(\widehat{E})$ là mở rộng của $u$ bằng tính liên tục. Khi đó $u$ là một tự đồng cấu Riesz nếu và chỉ nếu $\widehat{u}$ là một tự đồng cấu như vậy;

c) Trang bị cho đối ngẫu $E'$ của E tôpô hội tụ bị chặn, tôpô hội tụ compắc, hoặc tôpô yếu. Nếu $u$ là một tự đồng cấu Riesz của E, thì $^tu$ là một tự đồng cấu Riesz của $E'$.

a) Để $u$ là một tự đồng cấu Fredholm có chỉ số không, điều kiện cần và đủ là $u_1$ cũng như vậy (III, p. 44, mệnh đề 3). Mặt khác, với mọi $n\in \mathbf{N}$, ta có Ker($u^n_1$) $= E_1\cap$ Ker($u^n$), do đó

dim Ker($u^n_1$)$\leqslant$ dim Ker($u^n$)$\leqslant$ dim Ker($u^n_1$) $+$ codim$_E(E_1)$,

do đó dãy (dim Ker($u^n$))$_{n\in\mathbf{N}}$ bị chặn nếu và chỉ nếu dãy (dim Ker($u^n_1$))$_{n\in\mathbf{N}}$ bị chặn. Suy ra, $u$ là một tự đồng cấu Riesz của E nếu và chỉ nếu $u_1$ là một tự đồng cấu Riesz của $E_1$ (bổ đề 2).

b) Theo mệnh đề 4 của III, p. 44, với mọi $n\in \mathbf{N}$, ánh xạ $\widehat{u}^n$ là một tự đồng cấu Fredholm của $\widehat{E}$ sao cho Ker($\widehat{u}^n$) $=$ Ker($u^n$) và ind($\widehat{u}^n$) $=$ ind($u^n$) $=n$ ind($u$). Suy ra, $u$ là một tự đồng cấu Riesz nếu và chỉ nếu $\widehat{u}$ là một tự đồng cấu Riesz.

c) Chuyển vị $^tu$ là một tự đồng cấu Fredholm có chỉ số 0 của $E'($III, p. 43, n$^o3$). Vì hạt nhân của $(^tu)^n$ là trực giao của ảnh của $u^n$ (EVT, IV, p. 27, mệnh đề 2), dãy (Ker($^tu$)$^n$)$_n$ là dừng. Điều này chứng minh rằng $^tu$ là một tự đồng cấu Riesz của $E'$.

#### Mệnh đề 8 {#ts-iii-s3-prop-8 .statement tag=02RY}

Cho E là một không gian lồi địa phương tách và $u$ một tự đồng cấu của E. Các điều kiện sau là tương đương:

(i) $u$ là một tự đồng cấu Riesz của E;

(ii) Tồn tại một nghịch đảo giả $v$ của $u$ giao hoán với $u$;

(iii) Tồn tại một không gian con vectơ đóng $E_1$ của E, đối chiều hữu hạn, ổn định dưới tác dụng của $u$, sao cho $u$ cảm sinh một tự đẳng cấu của $E_1$.

Hàm ý (i) $=\Rightarrow$ (ii) suy ra từ mệnh đề 6, d).

Giả sử rằng $u$ có một nghịch đảo giả $v$ khả hoán với $u$. Hạt nhân $E_1$ của $1_E-u\circ v$ là một không gian con vectơ đóng của E, đối chiều hữu hạn, ổn định dưới tác dụng của $u$ và $v$. Vì ta có $u(v(x)) =v(u(x)) =x$ với mọi $x\in E_1$, các ánh xạ $u$ và $v$ cảm sinh các tự đẳng cấu của $E_1$ nghịch đảo với nhau. Do đó (ii) suy ra (iii).

Cuối cùng, hàm ý (iii) $=\Rightarrow$ (i) suy ra từ mệnh đề a) của mệnh đề 7 và từ việc một tự đẳng cấu là một tự đồng cấu Riesz.

#### Mệnh đề 9 {#ts-iii-s3-prop-9 .statement tag=02RZ}

Cho E là một không gian lồi địa phương tách và cho $u,v$ là các phần tử khả hoán của $\mathscr{L}(E)$. Các điều kiện sau là tương đương:

(i) Các tự đồng cấu $u$ và $v$ là các tự đồng cấu Riesz;

(ii) Tự đồng cấu $u\circ v$ là một tự đồng cấu Riesz.

Giả sử $u$ và $v$ là các tự đồng cấu Riesz; gọi $u'$ và $v'$ là các nghịch đảo giả chính tắc của chúng. Các tự đồng cấu $u,v,u'$ và $v'$ của E giao hoán (mệnh đề 6, d)). Tự đồng cấu $v'\circ u'$ là một nghịch đảo giả của $u\circ v$ và giao hoán với $u\circ v$, do đó $u\circ v$ là một tự đồng cấu Riesz (mệnh đề 8).

Ngược lại, giả sử $u\circ v$ là một tự đồng cấu Riesz, và gọi $w$ là nghịch đảo giả chính tắc của nó. Vì $u$ giao hoán với $u\circ v$, các tự đồng cấu $u$ và $w$ giao hoán theo mệnh đề 6, d). Tương tự $v$ và $w$ giao hoán. Do đó các tự đồng cấu $u,v$ và $w$ của E giao hoán; suy ra tự đồng cấu $v\circ w$ của E là một nghịch đảo giả của $u$ và $w\circ u$ là một nghịch đảo giả của $v$. Theo mệnh đề 8$,u$ và $v$ là các tự đồng cấu Riesz.

Cho $u$ là một tự đồng cấu Riesz của E. Nếu $v$ là một tự đẳng cấu của E, thì tự đồng cấu $u\circ v$ của E không nhất thiết là một tự đồng cấu Riesz của E, ngay cả khi $u\circ v-v\circ u$ có hạng hữu hạn. Nếu $h$ là một tự đồng cấu hạng hữu hạn của E, thì tự đồng cấu $u+h$ không nhất thiết là một tự đồng cấu Riesz (xem III, p. 120, bài tập 3).

#### Mệnh đề 10 {#ts-iii-s3-prop-10 .statement tag=02S0}

Cho E và F là các không gian lồi địa phương, $p\in \mathscr{L}(E; F)$ và $q\in \mathscr{L}(F; E)$. Đặt $u= 1_E-q\circ p$ và $v= 1_F-p\circ q$.

a) Cho $n\in \mathbf{N}$. Ánh xạ $p$ xác định bằng hạn chế một đẳng cấu của các không gian vectơ tôpô từ Ker($u^n$) lên Ker($v^n$) và xác định, bằng cách chuyển qua các thương, một đẳng cấu của các không gian vectơ tôpô từ Coker($u^n$) lên Coker($v^n$);

b) Nếu ảnh của $u$ đóng trong E, thì ảnh của $v$ đóng trong F;

c) Nếu Ker($u$) có một phần bù tôpô trong E, thì Ker($v$) có một phần bù như vậy trong F. Nếu Im($u$) có một phần bù tôpô trong E, thì Im($v$) có một phần bù như vậy trong F;

d) Nếu $u$ là một cấu xạ ngặt, thì $v$ là một cấu xạ ngặt;

e) Nếu $u$ là một tự đẳng cấu của E, thì $v$ là một tự đẳng cấu của F;

f) Nếu $u$ là một tự đồng cấu Fredholm của E, thì $v$ là một tự đồng cấu Fredholm của F, và ta có ind($u$) $=$ ind($v$);

g) Giả sử E và F tách được. Nếu $u$ là một tự đồng cấu Riesz của E, thì $v$ là một tự đồng cấu Riesz của F.

Trước hết, hãy chú ý các công thức

$$
q\circ v=u\circ q,v\circ p=p\circ u \tag{6}
$$

Sau đó ta chứng minh hai bổ đề.

#### Bổ đề 4 {#ts-iii-s3-lem-4 .statement tag=02S1}

Cho $n\in \mathbf{N}$. Đặt

$ni-1(n)i-1$

$q_n=\sum(-1)q\circ (p\circ q)$.

$$
i
$$

$i=1$

Ta có $u^n= 1_E-q_n\circ p$ và $v^n= 1_F-p\circ q_n$.

Ta có $(q\circ p)^i=q\circ (p\circ q)^{i-1}\circ p$ với mọi số nguyên $i\geqslant 1$. Khi đó ta tính được

$nnni-1(n)i$

$u= (1_E-q\circ p)= 1_E-\sum(-1)(q\circ p)= 1_E-q_n\circ p$

$$
i
$$

$$
i=1
$$

$nnni-1(n)i$

$v= (1_F-p\circ q)= 1_F-\sum(-1)(p\circ q)= 1_F-p\circ q_n$,

$$
i
$$

$i=1$

do đó suy ra kết quả.

#### Bổ đề 5 {#ts-iii-s3-lem-5 .statement tag=02S2}

Cho $u'$ là một phần tử của $\mathscr{L}(E)$. Đặt $v'= 1_F+p\circ u'\circ q$. Nếu $u'$ là một nghịch đảo của $u$, thì $v'$ là một nghịch đảo của $v$. Nếu $u'$ là một giả nghịch đảo của $u$, thì $v'$ là một giả nghịch đảo của $v$. Nếu $u'$ giao hoán với $u$, thì $v'$ giao hoán với $v$.

Dùng các công thức (6), ta tính được

$$
v-v'\circ v=-p\circ u'\circ q\circ v=-p\circ u'\circ u\circ q
$$

$$
v-v\circ v'=-v\circ p\circ u'\circ q=-p\circ u\circ u'\circ q
$$

do đó

$$
1_F-v'\circ v=p\circ (1_E-u'\circ u)\circ q
$$

$$
1_F-v\circ v'=p\circ (1_E-u\circ u')\circ q
$$

điều này chứng minh bổ đề.

Hãy chứng minh Mệnh đề 10. Có tính đến Bổ đề 4, chỉ cần chứng minh mệnh đề a) đối với $n= 1$. Theo các công thức (6), các ánh xạ $p$ và $q$ xác định, khi chuyển qua các không gian con, các ánh xạ tuyến tính liên tục $p':$ Ker($u$)$\rightarrow$ Ker($v$) và $q':$ Ker($v$)$\rightarrow$ Ker($u$), và khi chuyển qua các thương, các ánh xạ tuyến tính liên tục $p'':$ Coker($u$)$\rightarrow$ Coker($v$) và $q'':$ Coker($v$)$\rightarrow$ Coker($u$).

Vì $1_E-u=q\circ p$ và $1_F-v=p\circ q$, các ánh xạ $p'$ và $q'$ một mặt, $p''$ và $q''$ mặt khác, là các đẳng cấu nghịch đảo của nhau. Điều này chứng minh a).

Để ảnh của một ánh xạ tuyến tính liên tục là đóng, điều kiện cần và đủ là đối hạt nhân của ánh xạ này là một không gian tách được. Do đó b) suy ra từ a).

Kí hiệu $i: Ker(u)\rightarrow E$ và $j:$ Ker($v$)$\rightarrow F$ là các đơn cấu chính tắc. Giả sử rằng Ker($u$) có một phần bù tôpô trong E, và gọi $r: E\rightarrow$ Ker($u$) là một co rút tuyến tính liên tục của $i$. Đặt $r'=p'\circ r\circ q$. Ta có $r'\in \mathscr{L}(F$; Ker($v$)) và

$$
r'\circ j=p'\circ r\circ q\circ j=p'\circ r\circ i\circ q'=p'\circ q'= 1_{Ker(v)}
$$

do đó $r'$ là một co rút tuyến tính liên tục của $j$ và Ker($v$) có một phần bù tôpô trong F. Điều này chứng minh mệnh đề thứ nhất của c). Mệnh đề thứ hai được chứng minh tương tự, bằng cách nhận thấy rằng nếu $s:$ Coker($u$)$\rightarrow E$ là một tiết diện tuyến tính liên tục của toàn cấu chính tắc từ E lên Coker($u$), thì $p\circ s\circ q''$ là một tiết diện tuyến tính liên tục của toàn cấu chính tắc từ F lên Coker($v$).

Kí hiệu $\overline{u}: E/$ Ker($u$)$\rightarrow$ Im($u$) và $\overline{v}: F/$ Ker($v$)$\rightarrow$ Im($v$) là các ánh xạ tuyến tính liên tục song ánh cảm sinh bởi $u$ và $v$. Theo các công thức (6), ánh xạ $p$ định nghĩa, khi chuyển qua các thương, một ánh xạ tuyến tính liên tục $p_1: E/$ Ker($u$)$\rightarrow F/$ Ker($v$), và $p,q$ định nghĩa, khi chuyển qua các không gian con, các ánh xạ tuyến tính liên tục $p_0:$ Im($u$)$\rightarrow$ Im($v$) và $q_0:$ Im($v$)$\rightarrow$ Im($u$).

Gọi $t:$ Im($v$)$\rightarrow F/$ Ker($v$) là ánh xạ hợp thành của đơn ánh chính tắc Im($v$)$\rightarrow F$ và toàn cấu chính tắc $F\rightarrow F/$ Ker($v$); nó liên tục. Ta có $\overline{v}\circ t= 1_{Im(v)}-p_0\circ q_0$ và $\overline{v}\circ p_1=p_0\circ \overline{u}$, do đó

$$
\overline{v}\circ (t+p_1\circ \overline{u}^{-1}\circ q_0) =\overline{v}\circ t+p_0\circ q_0= 1_{Im(v)}
$$

Điều này chứng tỏ rằng $t+p_1\circ \overline{u}^{-1}\circ q_0$ là song ánh ngược của $\overline{v}$. Nếu $u$ ngặt, ánh xạ $\overline{u}^{-1}$ liên tục, và $\overline{v}^{-1}$ cũng vậy, điều đó chứng tỏ rằng $v$ ngặt. Điều này chứng tỏ d).

Theo bổ đề 5, nếu $u$ là một tự đẳng cấu của E, thì $v$ là một tự đẳng cấu của F. Tương tự, nếu $u$ là một tự đồng cấu Fredholm của E, thì $v$ là một tự đồng cấu Fredholm của F, và khi đó ta có ind($u$) $=$ ind($v$) theo a). Điều này chứng tỏ e) và f). Cuối cùng, nếu E và F là tách được và nếu $u$ là một tự đồng cấu Riesz của E, thì $v$ là một tự đồng cấu Riesz của F theo bổ đề 5 và điều kiện (ii) của mệnh đề 8; đó là mệnh đề g).

### 5. Các ánh xạ Fredholm và các ánh xạ Riesz giữa các không gian Fréchet

#### Mệnh đề 11 {#ts-iii-s3-prop-11 .statement tag=02S3}

Cho E và F là các không gian Fréchet. Để một ánh xạ tuyến tính liên tục $u$ từ E vào F là một ánh xạ Fredholm, điều kiện cần và đủ là hạt nhân và đối hạt nhân của nó đều hữu hạn chiều.

Điều này suy ra từ đặc trưng hóa các ánh xạ Fredholm cho bởi điều kiện (ii) của mệnh đề 2 của III, p. 42 và từ bổ đề sau:

#### Bổ đề 6 {#ts-iii-s3-lem-6 .statement tag=02S4}

Cho E và F là các không gian Fréchet và $u\in \mathscr{L}(E; F)$. Giả sử rằng ảnh của $u$ có đối chiều hữu hạn trong F. Khi đó ảnh của $u$ đóng trong F và $u$ là một cấu xạ ngặt.

Gọi G là một không gian con vectơ của F bù với Im($u$); không gian con G là đóng (TVS, I, p. 14, hệ quả 1), nên không gian thương $F/G$ là một không gian Fréchet (TG, IX, p. 25, mệnh đề 4). Gọi $\pi : F\rightarrow F/G$ là toàn cấu chính tắc. Ánh xạ $\pi \circ u$ là toàn ánh, nên ngặt (TVS, I, p. 19, hệ quả 3). Khi đó mệnh đề suy ra từ hệ quả 2 của III, p. 40.

#### Mệnh đề 12 {#ts-iii-s3-prop-12 .statement tag=02S5}

Cho E và F là các không gian Fréchet. Trang bị cho các đối ngẫu của chúng $E'$ và $F'$ tôpô yếu, tôpô hội tụ compắc, hoặc tôpô hội tụ bị chặn. Cho $u\in \mathscr{L}(E; F)$. Để $u$ là một ánh xạ Fredholm từ E vào F, điều kiện cần và đủ là $^tu$ là một ánh xạ Fredholm từ $F'$ vào $E'$.

Điều kiện là cần (III, p. 43, n$^o3$). Ta sẽ chứng minh rằng nó là đủ. Nếu $^tu$ là một ánh xạ Fredholm, thì nó là một cấu xạ ngặt (III, p. 42, mệnh đề 2), nên $u$ là một cấu xạ ngặt với ảnh đóng (TVS, IV, p. 28, định lý 1 và p. 29, hệ quả 3). Theo các đẳng cấu chính tắc Coker($^tu$)$\rightarrow$ Ker($u$)$'$ và Ker($^tu$)$\rightarrow$ Coker($u$)$'$ (TVS, IV, p. 27, mệnh đề 2), các không gian vectơ Ker($u$) và Coker($u$) đều hữu hạn chiều và $u$ là một ánh xạ Fredholm (mệnh đề 2 của III, p. 42).

#### Mệnh đề 13 {#ts-iii-s3-prop-13 .statement tag=02S6}

Cho E là một không gian Fréchet và $u\in \mathscr{L}(E)$.

a) Tự đồng cấu $u$ là một tự đồng cấu Riesz khi và chỉ khi không gian không linh N của nó hữu hạn chiều và không gian đối không linh I của nó có đối chiều hữu hạn ;

b) Trang bị cho $E'$ tôpô hội tụ bị chặn, tôpô hội tụ compact, hoặc tôpô yếu. Nếu $^tu$ là một tự đồng cấu Riesz của $E'$, thì $u$ là một tự đồng cấu Riesz của E.

a) Giả sử rằng không gian lũy linh N là hữu hạn chiều và không gian đối lũy linh I có đối chiều hữu hạn. Vì Ker($u$)$\subset N$ và $I\subset$ Im($u$), hạt nhân của $u$ là hữu hạn chiều và ảnh của $u$ có đối chiều hữu hạn. Theo định nghĩa và Mệnh đề 11, ánh xạ $u$ là một tự đồng cấu Riesz. Mệnh đề đảo lại suy ra từ định nghĩa.

b) Theo Mệnh đề 12, giả thiết kéo theo rằng $u$ là một tự đồng cấu Fredholm có chỉ số ind($^tu$) $=-$ ind($u$) $= 0$ (No.$^o3$, công thức (4)). Cho $n\in \mathbf{N}$. Vì ảnh của $u^n$ là đóng và có trực giao là hạt nhân của $^tu^n$ (EVT, IV, p. 27, Prop. 2), dãy (Im($u^n$)) là dừng, và do đó $u$ là một tự đồng cấu Riesz.

### 6. Đặc trưng hóa phổ của các tự đồng cấu Riesz

Cho E là một không gian Banach phức và $u$ là một tự đồng cấu của E. Nhắc lại rằng Sp($u$) kí hiệu phổ của $u$ đối với đại số Banach có đơn vị $\mathscr{L}(E) ($xem § 7 của I, p. 127).

Giả sử rằng 0 là một điểm cô lập của Sp($u$); nhắc lại rằng khi đó người ta kí hiệu bởi $e_0(u)$ phép chiếu phổ liên kết với $u$ và với tập con mở và đóng $\{0\}$ của phổ của $u($xem No.$^o3$ của I, p. 131). Ta có $e_0(u) =f(u)$ đối với mọi mầm của một hàm chỉnh hình $f$ trong một lân cận của Sp($u$) bằng 1 trong một lân cận của 0 và bằng không trong một lân cận của Sp($u$)$-\{0\}$.

Khi chuyển qua các không gian con, tự đồng cấu $u$ cảm sinh một tự đồng cấu lũy linh giả trên ảnh của $e_0(u)$, mà phổ thu về $\{0\}$, và một tự đẳng cấu của hạt nhân của $e_0(u)$, mà phổ là Sp($u$)$-\{0\}($loc. cit.).

#### Mệnh đề 14 {#ts-iii-s3-prop-14 .statement tag=02S7}

Cho E là một không gian Banach phức. Để một phần tử $u$ của $\mathscr{L}(E)$ là một tự đồng cấu Riesz của E, điều kiện cần và đủ là một trong hai điều kiện sau đây, loại trừ lẫn nhau, được thỏa mãn:

(i) Tự đồng cấu $u$ của E là một tự đẳng cấu của E;

(ii) Điểm 0 là một điểm cô lập của Sp($u$) và phép chiếu $e_0(u)$ có hạng hữu hạn.

Khi điều kiện (ii) được thỏa mãn, ảnh của $e_0(u)$ là không gian lũy linh của $u$ và hạt nhân của $e_0(u)$ là không gian đối lũy linh của $u$.

Mọi tự đẳng cấu của E đều là một tự đồng cấu Riesz của E (III, p. 47, nhận xét 1). Nếu $u$ thỏa mãn điều kiện (ii), hạt nhân F của $e_0(u)$ là một không gian con vectơ đóng có đối chiều hữu hạn của E, ổn định dưới $u$. Gọi $u_F$ là tự đồng cấu của F được cảm sinh bởi $u$. Phổ của nó được chứa trong $\mathbf{C}-\{0\}$ (No. 3 của I, p. 131), do đó $u_F$ là một tự đẳng cấu của F. Suy ra $u$ là một tự đồng cấu Riesz của E (III, p. 48, mệnh đề 8).

Ngược lại, giả sử $u$ là một tự đồng cấu Riesz của E. Gọi N là không gian không hóa của nó và I là đối không gian không hóa của nó. Theo mệnh đề 6 của III, p. 47, không gian E là tổng trực tiếp tôpô của N và I, và ánh xạ $u$ xác định, khi chuyển qua các không gian con ấy, một tự đồng cấu lũy linh $u_N$ của N và một tự đẳng cấu $u_I$ của I. Đặc biệt, ta có Sp($u_N$)$\subset  \{0\}$ và $0\not \in$ Sp($u_I$). Nếu N bằng không, thì I = E và $u$ là một tự đẳng cấu của E. Nếu không, thì 0 là một điểm cô lập của Sp($u$) và $e_0(u)$ là phép chiếu có ảnh là N và hạt nhân là I (mệnh đề 2 của I, p. 129); đặc biệt, nó có hạng hữu hạn.

#### Nhận xét {#ts-iii-s3-n6-rem-1 .statement tag=02S8}

Cho E là một không gian Banach thực và $u$ là một tự đồng cấu của E. Giả sử rằng 0 là một điểm cô lập của phổ phức của $u$, nghĩa là của phổ của tự đồng cấu $1\otimes u$ của không gian khả chuẩn đầy đủ phức hóa $E_{(\mathbf{C})}$ của E (I, p. 85, No. 13). Tập con $\{0\}$ của phổ phức của $u$ là mở và đóng, và bất biến đối với phép liên hợp; gọi $e_0(u)\in \mathscr{L}(E)$ là phép chiếu phổ liên kết với nó (No. 13 của I, p. 85). Mệnh đề 14 vẫn còn đúng, mutatis mutandis, trong cách đặt này.

## BÀI TẬP {#ts-iii-s3-exercises}

Xem [bài tập của § 3](exercises/s3/).

[^1]: Một số tác giả cũng nói "toán tử chỉ số" hoặc "giả đẳng cấu".
