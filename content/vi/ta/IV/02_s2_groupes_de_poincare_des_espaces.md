---
book: ta
book_title: Topologie algébrique
chapter: IV
chapter_title: ESPACES DÉLAÇABLES
section: 2
section_title: Groupes de Poincaré des espaces délaçables
lang: vi
source: ta-i-iv-fr
book_pages: TA IV.351-TA IV.368, TA IV.457-TA IV.458
pdf_pages: 0367-0384, 0473-0474
extraction: native
subsections:
    - "no": 1
      title: Propriétés des homomorphismes $\pi_1(f, a)$
      page: 351
      pdf_page: 367
    - "no": 2
      title: Applications relativement connexes
      page: 353
      pdf_page: 369
    - "no": 3
      title: Présentation des groupes de Poincaré
      page: 359
      pdf_page: 375
    - "no": 4
      title: Compléments sur les espaces polonais
      page: 360
      pdf_page: 376
    - "no": 5
      title: Relations d’équivalence maigres dans les espaces polonais
      page: 363
      pdf_page: 379
    - "no": 6
      title: Cardinal des groupes de Poincaré
      page: 365
      pdf_page: 381
statements: 30
exercises: 5
content_sha256: 5e86aa4bf7f68b496dc66c45054036bec9323c4a0abe9e41eb7770eb7a5721f9
translated_from: content/en-mt/ta/IV/02_s2_groupes_de_poincare_des_espaces.md
source_lang: en-mt
translation_method: machine
source_content_sha256: 4c430974a7d8e06ebe947357f0d54c7fd0baf1beadadb269fea12855e8e9e4df
translation_model: gpt-5-6-mini
translation_run: translate-vi-8f5e1762
glossary_version: 34
glossary_terms_sha256: 6d51bc45d90b3d9752981c2d7919f2e0f84a6ee3c64f4b0dce8d43e8f38df39d
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 2. CÁC NHÓM POINCARÉ CỦA CÁC KHÔNG GIAN KHÔNG THỂ THÁO GỠ

### 1. Các tính chất của các đồng cấu $\pi_1(f, a)$

Cho A và B là các không gian tôpô, cho $(E, p)$ là một phủ của A, cho $(E', p')$ là một phủ của B, cho $f: A\rightarrow B$ và $g: E\rightarrow E'$ là các ánh xạ liên tục sao cho $p'\circ g=f\circ p$. Cho $a$ là một điểm của A và cho $b=f(a)$. Với mọi $\gamma \in \pi_1(A, a)$ và mọi $x\in E_a$, ta có $g(x\cdot \gamma ) =g(x)\cdot f_*(\gamma )$, theo quan hệ (3), III, p. 304. Nếu biểu đồ

E $^gE'$

$pp'$

A $^f$ B

là một bình phương Descartes, ánh xạ $g$ cảm sinh một song ánh từ $E_a$ lên $E'_b$. Phép toán của $\pi_1(A, a)$ trên thớ $E_a$ khi đó là hợp thành của phép toán của nhóm $\pi_1(B, b)$ trên $E'_b$ và của đồng cấu $\pi_1(f, a)$ của $\pi_1(A, a)$ vào $\pi_1(B, b)$.

#### Mệnh đề 1 {#ta-iv-s2-prop-1 .statement tag=020S}

Cho A là một không gian tôpô không thể tháo gỡ, cho B là một không gian tôpô liên thông địa phương bởi các cung, và cho $f: A\rightarrow B$ là một ánh xạ liên tục. Cho $a$ là một điểm của A và $b=f(a)$. Giả sử rằng mọi phủ của A đều đẳng cấu với ảnh ngược qua $f$ của một phủ của B. Khi đó đồng cấu $\pi_1(f, a):\pi_1(A, a)\rightarrow$ $\pi_1(B, b)$ là đơn ánh.

Vì không gian A là không thể tháo gỡ, tồn tại một phủ E của A có thớ $E_a$ là một tập hợp chính thuần nhất $\pi_1(A, a)$ (IV, p. 342, Định lý 1). Theo giả thiết, phép toán này thu được nhờ đồng cấu $\pi_1(f, a)$ từ một phép toán của $\pi_1(B, b)$ trên $\pi_1(A, a)$. Điều này kéo theo tính đơn ánh của đồng cấu $\pi_1(f, a)$.

#### Mệnh đề 2 {#ta-iv-s2-prop-2 .statement tag=020T}

Cho A là một không gian tôpô liên thông liên thông địa phương bởi các cung, cho B là một không gian tôpô không thể tháo gỡ, và cho $f: A\rightarrow B$ là một ánh xạ liên tục. Cho $a$ là một điểm của A và $b=$ $f(a)$. Các khẳng định sau là tương đương:

(i) Đồng cấu $\pi_1(f, a):\pi_1(A, a)\rightarrow \pi_1(B, b)$ là toàn ánh.

(ii) Với mọi cặp $(E,E')$ các phủ của B, ánh xạ

$$
f^*:\mathscr{C}_B(E; E')\rightarrow \mathscr{C}_A(A\times_BE; A\times_BE')
$$

gán cho một B-cấu xạ $g: E\rightarrow E'$ cấu xạ A

$$
f^*(g): A\times_BE\rightarrow A\times_BE',(x, y)\mapsto (x, g(y))
$$

là song ánh.

Nhờ đồng cấu $\pi_1(f, a)$, mọi tập hợp $\pi_1(B, b)$ được trang bị một cấu trúc của tập hợp $\pi_1(A, a)$. Điều kiện (i) khi đó tương đương với điều kiện sau (i$'$):

(i$'$) Với mọi cặp $(F,F')$ các tập hợp $\pi_1(B, b)$, mọi $\pi_1(A, a)$-cấu xạ từ F vào $F'$ đều là một $\pi_1(B, b)$-cấu xạ.

Thật vậy, nếu đồng cấu $\pi_1(f, a)$ là toàn ánh, thì mọi $\pi_1(A, a)$-cấu xạ của các tập hợp $\pi_1(B, b)$ là một $\pi_1(B, b)$-cấu xạ. Ngược lại, ta lấy một tập hợp $\pi_1(B, b)$ là F thu gọn về một điểm và đặt $F'=\pi_1(B, b)/f_*(\pi_1(A, a))$. Ánh xạ của F vào $F'$ có ảnh là $f_*(\pi_1(A, a))$ là một $\pi_1(A, a)$-cấu xạ nhưng không phải là một $\pi_1(B, b)$-cấu xạ nếu $F'$ không thu gọn về một điểm, nghĩa là nếu $\pi_1(f, a)$ không toàn ánh.

Vì không gian B là không cuộn được, mọi tập hợp $\pi_1(B, b)$ đều đẳng cấu với tập hợp $\pi_1(B, b)$ $E_b$, trong đó E là một phủ của B (IV, p. 344, nhận xét 1). Sự tương đương của (i$'$) và (ii) do đó suy ra từ mệnh đề 2 của III, p. 310.

#### Mệnh đề 3 {#ta-iv-s2-prop-3 .statement tag=020U}

Cho B là một không gian tôpô không cuộn được và cho A là một không gian con liên thông và liên thông địa phương theo cung của B (ví dụ một tập con mở và liên thông). Cho $a$ là một điểm của A. Các tính chất sau là tương đương:

(i) Mọi phủ của B đều có thể tầm thường hóa trên A.

(ii) Ảnh của đồng cấu từ $\pi_1(A, a)$ vào $\pi_1(B, a)$ cảm sinh bởi đơn ánh chính tắc thu gọn về phần tử đơn vị.

Kéo theo (ii)$\Rightarrow$(i) suy ra từ hệ quả 3 (III, p. 309).

Ngược lại, giả sử rằng mọi phủ của B đều có thể tầm thường hóa trên A. Đặc biệt đây là trường hợp của phủ liên thông đơn giản theo cung $(\lambda_a(B), \varepsilon_B)$ (IV, p. 342, định lý 1), do đó đồng cấu $\pi_1(A, a)\rightarrow \pi_1(B, a)$ là tầm thường (III, p. 309, hệ quả 3 của mệnh đề 1).

### 2. Các ánh xạ liên thông tương đối

#### Định nghĩa 1 {#ta-iv-s2-def-1 .statement tag=020V}

Cho X và Y là các không gian tôpô và cho $f$ là một ánh xạ liên tục từ X vào Y. Ta nói rằng ánh xạ $f$ là liên thông tương đối nếu mọi điểm của Y sở hữu một hệ cơ bản

các lân cận gồm các tập hợp V sao cho $\overset{-1}{f}(V)$ là liên thông và khác rỗng.

Cho $f: X\rightarrow Y$ là một ánh xạ liên tục; để $f$ là liên thông tương đối, điều kiện cần và đủ là mọi điểm của Y sở hữu một lân cận V sao cho ánh xạ $f_V:\overset{-1}{f}(V)\rightarrow V$ cảm sinh bởi $f$ là liên thông tương đối.

Cho X và Y là các không gian tôpô và cho $f: X\rightarrow Y$ là một ánh xạ liên tục liên thông tương đối. Ảnh của $f$ là trù mật trong Y. Đối với mọi tập con mở của Y, ánh xạ $f_V:\overset{-1}{f}(V)\rightarrow V$ là liên thông tương đối.

#### Mệnh đề 4 {#ta-iv-s2-prop-4 .statement tag=020W}

Cho X và Y là các không gian tôpô và cho $f: X\rightarrow Y$ là một ánh xạ liên tục liên thông tương đối.

a) Đối với mọi thành phần liên thông U của X, $\overline{f(U)}$ là một tập con

liên thông, mở và đóng của Y, và ta có $\overset{-1}{f}(f(U)) = U$.

b) Đối với mọi thành phần liên thông V của Y, tồn tại một thành phần liên thông U của X sao cho $V =f(U)$. Ánh xạ của U vào V cảm sinh bởi $f$ bằng cách chuyển qua các tập con là liên thông tương đối.

c) Các thành phần liên thông của X ( resp. của Y) là mở và đóng.

a) Gọi V là tập hợp các $y\in Y$ sở hữu một lân cận W sao cho

$\overset{-1}{f}(W)$ là liên thông và gặp U; đây là một tập mở của Y. Nó chứa $\overline{f(U)}$ vì $f$ là liên thông tương đối. Ngược lại, cho $y\in V$; lấy

W là một lân cận của $y$ sao cho $\overset{-1}{f}(W)$ là liên thông và gặp U. Với

mọi lân cận $W'$ của $y$ sao cho $\overset{-1}{f}(W')$ là liên thông, $\overset{-1}{f}(W\cap W')$ là

khác rỗng, do đó $\overset{-1}{f}(W\cup W')$ là liên thông (TG, I, p. 81, mệnh đề 2). Theo

giả thiết, $\overset{-1}{f}(W\cup W')$ gặp U; do đó ta có $\overset{-1}{f}(W\cup W')\subset U$ và, a fortiori, $W'\cap f(U)=\not\emptyset$. Điều này chứng minh rằng $y\in \overline{f(U)}$; do đó, $V =\overline{f(U)}$. Đặc biệt, tập hợp $\overline{f(U)}$ là mở và đóng trong Y; mệnh đề 1 (TG, I, p. 81) còn suy ra rằng nó là liên thông.

Các lập luận trước đó còn cho thấy rằng $\overset{-1}{f}(f(U))\subset U$,

do đó đẳng thức $\overset{-1}{f}(f(U)) = U$, bao hàm kia là hiển nhiên. Đặc biệt, U là mở và đóng trong X.

b) Gọi V là thành phần liên thông của một điểm $y$ của Y, lấy W là một

lân cận của $y$ sao cho $\overset{-1}{f}(W)$ là liên thông và khác rỗng và lấy U là một

thành phần liên thông của X chứa $\overset{-1}{f}(W)$. Vì $y\in \overline{f(U)}$, từ a) và từ định nghĩa của thành phần liên thông của $y$ suy ra rằng $V =\overline{f(U)}$. Do đó V là mở và đóng trong Y.

#### Hệ quả 1 {#ta-iv-s2-prop-4-cor-1 .statement tag=020X}

Cho X và Y là các không gian tôpô và cho $f: X\rightarrow Y$ là một ánh xạ liên tục và liên thông tương đối. Bằng cách chuyển qua các thành phần liên thông, ánh xạ $f$ cảm sinh một song ánh từ tập hợp các thành phần liên thông của X lên tập hợp các thành phần liên thông của Y.

#### Hệ quả 2 {#ta-iv-s2-prop-4-cor-2 .statement tag=020Y}

Cho X và Y là các không gian tôpô và cho $f: X\rightarrow$ Y là một ánh xạ liên tục. Để $f$ liên thông tương đối, điều kiện cần và đủ là ba tính chất sau được thỏa mãn:

a) Ảnh $f(X)$ là trù mật trong Y;

b) Không gian Y liên thông địa phương; $-_1$

c) Với mọi tập hợp mở và liên thông V của Y, tập hợp $f(V)$ là liên thông.

Giả sử rằng ánh xạ $f$ liên thông tương đối. Mật độ của $f(X)$ trong Y suy ra từ định nghĩa của một

ánh xạ liên thông tương đối. Cho V là một tập con mở của Y; ánh xạ $f_V:\overset{-1}{f}(V)\rightarrow$ V là liên thông tương đối. Theo Mệnh đề 4, các thành phần liên thông của V là mở và đóng trong V. Suy ra Y liên thông địa phương (TG, I, p. 85, mệnh đề 11). Để chứng minh mệnh đề c), chỉ cần chứng minh rằng X liên thông nếu Y liên thông. Theo bổ đề, tồn tại

một thành phần liên thông U của X sao cho $Y =\overline{f(U)}$ và $\overset{-1}{f}(f(U)) = U$, do đó U = X và X liên thông.

Ngược lại, giả sử các điều kiện a), b), c) được thỏa mãn, và ta hãy chứng minh rằng $f$ liên thông tương đối. Cho $y$ là một điểm của Y; vì Y liên thông địa phương, $y$ có một hệ cơ bản các lân cận mở liên thông. Nếu W là một lân cận như vậy, các điều kiện

c) và a) suy ra rằng $\overset{-1}{f}(W)$ là liên thông và khác rỗng. Do đó ánh xạ $f$ liên thông tương đối.

#### Hệ quả 3 {#ta-iv-s2-prop-4-cor-3 .statement tag=020Z}

Cho X và Y là các không gian tôpô và cho $f: X\rightarrow Y$ là một ánh xạ liên tục và liên thông tương đối. Cho F là một tập hợp và cho $g: X\rightarrow F$ là một ánh xạ hằng địa phương. Tồn tại một ánh xạ hằng địa phương duy nhất $h: Y\rightarrow F$ sao cho $g=h\circ f$.

Hạn chế của $g$ trên mỗi thành phần liên thông của X là hằng. Theo Hệ quả 1, tồn tại một ánh xạ $h: Y\rightarrow F$, hằng trên mỗi thành phần liên thông của Y, sao cho $g=h\circ f$. Ánh xạ $h$ là hằng địa phương, vì các thành phần liên thông của Y là mở. Tính duy nhất của một ánh xạ như vậy suy ra từ sự kiện rằng $f(X)$ là trù mật trong Y.

#### Ví dụ 1 {#ta-iv-s2-n2-exa-1 .statement tag=0210}

Cho X là một không gian tôpô và cho R là một quan hệ tương đương trong X. Gọi Y là không gian tôpô thương $X/R$ và $f: X\rightarrow Y$ là ánh xạ chính tắc. Giả sử rằng các lớp tương đương của R là liên thông. Khi đó, với mọi tập con mở và liên thông V của Y, tập hợp $\overset{-1}{f}(V)$ là liên thông (TG, I, p. 23, hệ quả 1 và p. 82, mệnh đề 7). Nếu không gian Y liên thông địa phương, thì ánh xạ $f$ liên thông tương đối.

#### Ví dụ 2 {#ta-iv-s2-n2-exa-2 .statement tag=0211}

Cho Y là một không gian tôpô liên thông địa phương bằng các cung, và cho X là một tập con mở của Y. Không gian $\mathscr{C}_c(\mathbf{I}; X)$ của các đường đi trong X được đồng nhất với một không gian con của không gian $\mathscr{C}_c(\mathbf{I}; Y)$ của các đường đi trong Y; giả sử rằng nó là trù mật. Khi đó đơn ánh chính tắc của X vào Y là một ánh xạ liên thông tương đối.

Thực vậy, chỉ cần chứng minh rằng, với mọi tập con mở, liên thông và khác rỗng V của Y, tập hợp $V\cap X$ là liên thông và khác rỗng. Không gian $\mathscr{C}_c(\mathbf{I}; V)$ là một tập con mở khác rỗng của $\mathscr{C}_c(\mathbf{I}; Y)$; nó gặp $\mathscr{C}_c(\mathbf{I}; X)$, điều này chứng minh rằng $V\cap X=\not\emptyset$. Cho $x$ và $x'$ là các điểm của $V\cap X$. Vì $V\cap X$ liên thông địa phương bằng các cung, các điểm $x$ và $x'$ có các lân cận mở U và $U'$, liên thông bằng các cung và được chứa trong $V\cap X$. Vì V liên thông bằng các cung (III, p. 260, mệnh đề 7), tồn tại một đường đi trong V nối $x$ với $x'$. Theo giả thiết về mật độ và định nghĩa của tôpô hội tụ compact, tồn tại một đường đi trong $V\cap X$ nối một điểm của U với một điểm của $U'$. Khi đó tồn tại một đường đi nối $x$ với $x'$ trong $V\cap X$, điều này chứng minh rằng tập hợp $V\cap X$ là liên thông.

#### Mệnh đề 5 {#ta-iv-s2-prop-5 .statement tag=0212}

Cho X và Y là các không gian tôpô và cho $f: X\rightarrow$ Y là một ánh xạ liên tục và liên thông tương đối. Với mọi cặp $(T,T')$ các phủ của Y, ánh xạ $f^*:\mathscr{C}_Y(T; T')\rightarrow$ $\mathscr{C}_X(X\times_YT; X\times_YT')$ là song ánh.

Cho $\mathscr{F}$ là bó trên X của các cấu xạ X từ $X\times_YT$ vào $X\times_YT'$ và cho $\mathscr{G}$ là bó trên Y của các cấu xạ Y từ T vào $T'$(I, p. 45, ví dụ 4). Với mọi tập mở U của Y, đặt $\varphi_U= (f_U)^*:\mathscr{G}(U)\rightarrow$

$\mathscr{F}(\overset{-1}{f}(U))$. Các ánh xạ $\varphi_U$ xác định một cấu xạ bó $\varphi :\mathscr{G}\rightarrow \varphi_*(\mathscr{F})$ và chỉ cần chứng minh rằng $\varphi$ là một đẳng cấu của các bó.

Vì Y là liên thông địa phương (IV, p. 354, hệ quả 2), các tập mở liên thông mà trên đó T và $T'$ khả phân hoạch tầm thường tạo thành một cơ sở của tôpô của Y. Theo hệ quả 2 của I, p. 55, chỉ cần chứng minh rằng đối với một tập mở U như vậy, ánh xạ $\varphi_U$ là song ánh, điều này cho phép ta giả sử rằng Y là liên thông và các phủ T và $T'$ là các phủ tầm thường $Y\times F$ và $Y\times F'$ trong đó F và $F'$ là các tập hợp được trang bị tôpô rời rạc. Ánh xạ $(x,(y, t))\mapsto (x, t)$ đồng nhất không gian X $X\times_Y(Y\times F)$ với $X\times F$ (tương ứng không gian X $X\times_Y(Y\times F')$ với $X\times F'$). Vì không gian X là liên thông (IV, p. 354, hệ quả 2), các tập hợp $\mathscr{C}_Y(Y\times F; Y\times F')$ và $\mathscr{C}_X(X\times F; X\times F')$ đều được đồng nhất với tập hợp $\mathscr{F}(F; F')$ các ánh xạ từ F vào $F'$, và ánh xạ $f^*$ được đồng nhất với ánh xạ đồng nhất của $\mathscr{F}(F; F')$. Điều này kết thúc chứng minh.

#### Hệ quả 1 {#ta-iv-s2-prop-5-cor-1 .statement tag=0213}

Cho X và Y là các không gian tôpô và cho $f: X\rightarrow Y$ là một ánh xạ liên tục liên thông tương đối. Cho T và $T'$ là các phủ của Y. Nếu các phủ $X\times_YT$ và $X\times_YT'$ của X là đẳng cấu, thì các phủ T và $T'$ là đẳng cấu.

Thật vậy, cho $h: X\times_YT\rightarrow X\times_YT'$ và $h': X\times_YT'\rightarrow X\times_YT$ là các đẳng cấu X nghịch đảo của nhau. Theo mệnh đề 5, tồn tại các cấu xạ Y $g: T\rightarrow T'$ và $g': T'\rightarrow T$ sao cho $f^*(g) =h$ và $f^*(g') =h'$. Khi đó ta có $f^*(g'\circ g) =f^*(g')\circ f^*(g) =$ Id$_{X\times_YT}$, do đó $g'\circ g=$ Id$_T$, vì ánh xạ $f^*$ là đơn ánh. Tương tự, $g\circ g'=$ Id$_{T'}$. Do đó các phủ T và $T'$ là đẳng cấu.

#### Hệ quả 2 {#ta-iv-s2-prop-5-cor-2 .statement tag=0214}

Cho X và Y là các không gian tôpô và cho $f: X\rightarrow Y$ là một ánh xạ liên tục và liên thông tương đối. Nếu không gian X đơn liên thông, thì điều tương tự cũng đúng với không gian Y.

Theo hệ quả 1, mọi phủ của Y thực sự đều khả phân hoạch tầm thường.

#### Hệ quả 3 {#ta-iv-s2-prop-5-cor-3 .statement tag=0215}

Cho X là một không gian tôpô liên thông địa phương bởi các cung, Y là một không gian tôpô không cuộn được, và cho $f: X\rightarrow$ Y là một ánh xạ liên tục liên thông tương đối. Với mọi điểm $x$ của X, đồng cấu $\pi_1(f, x):\pi_1(X, x)\rightarrow \pi_1(Y, f(x))$ là toàn ánh.

Theo IV, p. 353, mệnh đề 4, ta có thể giả sử rằng các không gian X và Y là liên thông. Khi đó hệ quả suy ra từ mệnh đề 5 và mệnh đề 2 của IV, p. 352.

#### Mệnh đề 6 {#ta-iv-s2-prop-6 .statement tag=0216}

Cho X và Y là các không gian tôpô và cho $f: X\rightarrow Y$ là một ánh xạ liên tục và liên thông tương đối. Giả sử rằng mọi điểm của Y có một lân cận mở V mà ảnh ngược của nó $\overset{-1}{f}(V)$ là đơn liên thông. Khi đó, với mọi phủ Z của X, tồn tại một phủ T của Y sao cho $X\times_YT$ là X-đẳng cấu với Z.

Cho $\mathscr{U}$ là tập hợp các tập mở của Y mà ảnh ngược của chúng trong X

là đơn liên thông. Với mọi $V\in \mathscr{U}$, phủ $\overset{-1}{f}(V)\times_XZ$

của $\overset{-1}{f}(V)$ là tầm thường hóa được; do đó tồn tại một không gian rời rạc $F_V$ và một

đẳng cấu của các phép phủ $g_V:\overset{-1}{f}(V)\times_XZ\rightarrow \overset{-1}{f}(V)\times F_V$. Với mỗi

cặp $(V,V')$ các tập mở thuộc $\mathscr{U}$, ánh xạ $f_{V\cap V'}:\overset{-1}{f}(V\cap$ $V')\rightarrow V\cap V'$ là liên thông tương đối. Theo mệnh đề 5 của IV, p. 356, tồn tại một đẳng cấu duy nhất của các phép phủ của $V\cap V'$, $h_{V',V}: (V\cap V')\times F_V\rightarrow (V\cap V')\times F_{V'}$, sao cho ta có $f^*(h_{V',V})(x, t) =$ $g_{V'}(g_V^{-1}(x, t))$ với mọi $x\in V\cap V'$ và mọi $t\in F_V$. Nếu V, $V',V''$ là các phần tử của $\mathscr{U}$, ta có $h_{V'',V}(x, t) =h_{V'',V'}(h_{V',V}(x, t))$ với mọi $x\in V\cap V'\cap V''$ và mọi $t\in F_V$. Khi đó tồn tại một Y-không gian duy nhất T và, với mọi $V\in \mathscr{U}$, một đẳng cấu $h_V: T_V\rightarrow V\times F_V$, sao cho ta có $h_{V',V}(x, t) =h_{V'}\circ h^{-1}_V(x, t)$ với mọi cặp $(V,V')$ các tập mở thuộc $\mathscr{U}$, mọi $x\in V\cap V'$ và mọi $t\in F_V($cf. TG, I, p. 16). Không gian T đặc biệt là một phép phủ của Y. Hơn nữa tồn tại một

ánh xạ duy nhất từ $X\times_YT$ lên Z mà hạn chế của nó lên $\overset{-1}{f}(V)\times_YT$ được cho bởi $g^{-1}_V\circ f^*(h_V)$ và đây là một đẳng cấu của các X-không gian, do đó có mệnh đề.

#### Hệ quả {#ta-iv-s2-n2-cor-1 .statement tag=0217}

Cho X và Y là các không gian tôpô co được và cho $f: X\rightarrow Y$ là một ánh xạ liên tục và liên thông tương đối. Giả sử rằng mọi điểm của Y có một lân cận V mà ảnh ngược

$\overset{-1}{f}(V)$ là đơn liên. Khi đó, với mọi điểm $x$ của X, đồng cấu $\pi_1(f, x):\pi_1(X, x)\rightarrow \pi_1(Y, f(x))$ là song ánh.

Có thể giả sử các không gian X và Y liên thông (IV, p. 353, mệnh đề 4). Theo hệ quả 3 (IV, p. 357), đồng cấu $\pi_1(f, x)$ là toàn ánh. Mệnh đề 6 và mệnh đề 1 của IV, p. 351 suy ra rằng nó là đơn ánh.

#### Nhận xét {#ta-iv-s2-n2-rem-1 .statement tag=0218}

Cho Y là một không gian tôpô, và cho X, $X'$ và $Y'$ là các không gian con của Y sao cho $X\subset X'\subset Y'\subset Y$. Giả sử rằng đơn ánh chính tắc của X vào Y là liên thông tương đối. Với mọi tập con mở liên thông V của Y, tập $V\cap X$ là liên thông và trù mật trong V (IV, p. 354, hệ quả 2); do đó, tập $V\cap X'$ là liên thông (TG, I, p. 81, mệnh đề 1). Điều này chứng minh rằng đơn ánh chính tắc của $X'$ vào $Y'$ là liên thông tương đối.

Cho V là một tập con mở của Y; theo điều đã nói trước đó, đơn ánh chính tắc của $V\cap X$ vào $V\cap X'$ là liên thông tương đối. Nếu tập $V\cap X$ là đơn liên, thì $V\cap X'$ cũng vậy, theo hệ quả 2 của IV, p. 357. Do đó, nếu đơn ánh chính tắc của X vào Y thỏa mãn các giả thiết của mệnh đề 6, thì điều tương tự cũng đúng với đơn ánh chính tắc của $X'$ vào $Y'$.

#### Ví dụ {#ta-iv-s2-n2-exa-3 .statement tag=0219}

Cho Y là một đa tạp khả vi hữu hạn địa phương chiều và cho Z là một đa tạp con đóng của Y (VAR, R, 5.8.3). Đặt X = Y-Z.

a) Nếu đối chiều của Z ít nhất bằng 2 tại mọi điểm, đơn ánh chính tắc của X vào Y là liên thông tương đối. Thật vậy, cho $z$ là một điểm của Z; tồn tại một lân cận mở V của $z$ trong Y và một đồng phôi $\varphi$ của V lên một không gian vectơ hữu hạn chiều E trên $\mathbf{R}$ sao cho $\varphi (V\cap Z)$ là một không gian vectơ con F của E có đối chiều $\geqslant 2$. Tập E-F là liên thông (TG, VI, p. 5, mệnh đề 4), do đó có mệnh đề.

b) Hơn nữa, giả sử đối chiều của Z ít nhất bằng 3 tại mọi điểm; các giả thiết của mệnh đề 6 và của hệ quả của nó khi đó được thỏa mãn bởi vì, với các ký hiệu của đoạn trước, E-F là đơn liên (I, p. 128, ví dụ 4).

Các đa tạp khả vi là các không gian co được (IV, p. 347), các kết quả của số này thừa nhận trường hợp riêng sau đây.

Cho Y là một đa tạp khả vi hữu hạn địa phương chiều, Z một đa tạp con đóng của Y và $i$ là đơn ánh chính tắc của Y-Z vào Y.

a) Nếu đối chiều của Z trong Y là $\geqslant 1$ tại mọi điểm, đa tạp Y-Z là trù mật trong Y và ánh xạ $\pi_0(i)$ là toàn ánh.

b) Nếu đối chiều của Z trong Y là $\geqslant 2$ tại mọi điểm, ánh xạ $\pi_0(i)$ là song ánh và, với mọi điểm $x$ của Y-Z, ánh xạ $\pi_1(i, x)$ là toàn ánh.

c) Nếu đối chiều của Z trong Y là $\geqslant 3$ tại mọi điểm, các ánh xạ $\pi_0(i)$ và $\pi_1(i, x)$ là song ánh, với mọi điểm $x$ của Y-Z.

### 3. Trình bày các nhóm Poincaré

#### Định lý 1 {#ta-iv-s2-thm-1 .statement tag=021A}

Cho X là một không gian tôpô co rút được compact và $x$ là một điểm của X. Nhóm Poincaré $\pi_1(X, x)$ có một trình bày hữu hạn.

Thành phần liên thông theo cung của $x$ trong X là mở, đóng và co rút được; điều này cho phép giả sử rằng không gian X là liên thông. Vì không gian X là co rút được, không gian-X $E =\lambda_x(X)$, được trang bị ánh xạ tận cùng, là một phủ không rỗng đơn liên theo cung (IV, p. 342, th. 1). Nhóm G = Aut$_X(E)$ đẳng cấu với $\pi_1(X, x)$; do đó chỉ cần chứng minh rằng nhóm G có một trình bày hữu hạn.

Vì X là compact, mọi điểm $x$ của X có một lân cận compact $K_x$ trên đó phủ E là tầm thường hóa được (TG, I, p. 65, hệ quả). Vì X liên thông địa phương, mọi $x\in X$ có một lân cận mở liên thông $W_x$, được chứa trong $K_x$. Cho F là một tập con hữu hạn của X sao cho các $W_x$, với $x\in F$, phủ X. Gọi $n$ là lực lượng của F.

Ta sẽ chứng minh bằng quy nạp rằng, với mọi số nguyên $k$ sao cho 1 $\leqslant k\leqslant n$, tồn tại một tập con A có lực lượng $k$ được chứa trong F và, với $x\in A$, một tiết diện $s_x$ của $p$ trên $K_x$, sao cho hợp của các $s_x(W_x)$, với $x\in A$, là một tập con liên thông của E. Mệnh đề đúng với $k= 1$. Giả sử nó đúng với một số nguyên $k$ sao cho $1\leqslant k < n$ và ta hãy chứng minh rằng nó đúng với $k+ 1$. Cho A là một tập con của F có lực lượng $k$ và, với mọi $x\in A$, cho $s_x$ là một tiết diện của E trên $K_x$, sao cho $\bigcup_{x\in A}s_x(W_x)$ là liên thông. Các tập mở $\bigcup_{x\in A}W_x$ và $\bigcup_{x\in F-A}W_x$ là khác rỗng và phủ X; do đó giao của chúng là khác rỗng, vì X là liên thông. Vì vậy tồn tại $x\in A,y\in F-A$ và $z\in W_x\cap W_y$. Đặt $A'= A\cup  \{y\}$ và chọn một tiết diện $s_y$ của E trên $K_y$ sao cho $s_y(z) =s_x(z)$. Các tập mở liên thông $\bigcup_{p\in A}s_p(W_p)$ và $s_y(W_y)$ là khác rỗng và có một điểm chung; do đó hợp của chúng là liên thông. Điều này chứng minh mệnh đề với $k+ 1$. Bằng quy nạp, vì vậy nó đúng với mọi số nguyên $k\in  \{1, . . . , n\}$.

Áp dụng điều trên cho $k=n$, khi đó tồn tại, với mọi $x\in F$, một tiết diện $s_x$ của E trên $K_x$, sao cho $U =\bigcup_{x\in F}s_x(W_x)$ là một tập con mở liên thông của E. Ta có $p(U) = X$. Vì nhóm G tác động bắc cầu trong mỗi thớ của phủ E, ta có GU = E.

Bao đóng của U được chứa trong $\bigcup_{x\in F}s_x(K_x)$ và do đó là compact. Phép toán của G trên E là thực sự (I, p. 96, cor. 1), do đó tập hợp các cặp $(g, x)\in G\times E$ sao cho $x\in \overline{U}$ và $gx\in \overline{U}$ là một tập con compact của $G\times E$ (TG, I, p. 77, prop. 6). Suy ra tập hợp các $g\in G$ sao cho $\overline{U}\cap g\overline{U}=\not\emptyset$ là compact. Vì nó rời rạc, nó hữu hạn. A fortiori, tập hợp các $g\in G$ sao cho $U\cap gU=\not\emptyset$ là hữu hạn. Do đó định lý suy ra từ prop. 10 của I, p. 136.

### 4. Phần bù trong các không gian Polish

#### Bổ đề 1 {#ta-iv-s2-lem-1 .statement tag=021B}

Cho X là một không gian tôpô và A là một tập con của X. Để A là tập hợp loại một, điều kiện cần và đủ là tồn tại một phủ mở $(U_i)_{i\in I}$ của X sao cho $A\cap U_i$ là tập hợp loại một trong $U_i$ với mọi $i\in I$.

Cho $\mathscr{O}$ là tập hợp các tập con mở U của X sao cho $A\cap U$ là tập hợp loại một. Tập hợp các tập con của $\mathscr{O}$ gồm các tập con mở từng đôi một rời nhau, có thứ tự theo quan hệ bao hàm, là quy nạp. Cho $\mathfrak{U}$ là một phần tử cực đại; một phần tử như vậy tồn tại theo E, III, p. 20, th. 2.

Cho O là hợp của các tập con mở của X thuộc $\mathfrak{U}$. Với mỗi tập con mở $U\in \mathfrak{U}$, cho $(B_{U,n})$ là một dãy các tập con hiếm của U có hợp là $A\cap U$. Với mỗi số nguyên $n$, hợp $B_n$ của các tập con $B_{U,n}$, với U chạy qua $\mathfrak{U}$, là hiếm tương đối với O (TG, IX, p. 52, prop. 1). Theo TG, IX, p. 53, prop. 2, $B_n$ là một tập con hiếm của X, vì O mở trong X. Do đó, tập hợp $A\cap O$, bằng hợp của các $B_n$, là một tập hợp loại một của X.

Cho F là phần bù của O. Nó là một tập con đóng của X; ta hãy chứng minh rằng nó có nội điểm rỗng. Trong trường hợp ngược lại, cho $x$ là một điểm nội của F. Theo giả thiết, tồn tại một lân cận mở V của $x$, có thể giả sử được chứa trong F, sao cho $A\cap V$ là tập hợp loại một. Khi đó V rời nhau với các tập con mở của X thuộc $\mathfrak{U}$ và $\mathfrak{U}\cup  \{V\}$ là một tập hợp các tập con mở từng đôi một rời nhau thuộc $\mathscr{O}$, điều này mâu thuẫn với tính cực đại của $\mathfrak{U}$. Quan hệ

$$
A = (A\cap F)\cup (A\cap O)
$$

khi đó suy ra A là tập hợp loại một, điều phải chứng minh.

Cho X là một không gian tôpô.

Nhắc lại (TG, IX, p. 69) rằng một tập con A của X được gọi là khả tiếp cận nếu tồn tại một tập con mở U của X sao cho $U\cap \complement A$ và $A\cap \complement U$ là các tập hợp loại một trong X. Tập hợp các tập con khả tiếp cận của X là một bộ lạc chứa bộ lạc Borel (TG, IX, p. 69, bổ đề 8 và chứng minh của nó). Một tập hợp loại một là khả tiếp cận.

Với mỗi tập con A của X, cho D(A) là tập hợp các điểm $x\in X$ sao cho với mọi lân cận V của $x,A\cap V$ không là tập hợp loại một. Ta cũng đặt $D^*(A) = A\cup D(A)$.

#### Bổ đề 2 {#ta-iv-s2-lem-2 .statement tag=021C}

Cho X là một không gian tôpô và A là một tập con của X.

a) Tập hợp D(A) đóng trong X; phần bù của nó là tập con mở lớn nhất U của X sao cho $A\cap U$ là một tập hợp loại một.

b) Để A là tập hợp loại một, điều kiện cần và đủ là D(A) rỗng.

c) Tập hợp $D^*(A)$ là khả tiếp cận.

d) Với mọi tập hợp khả tiếp cận B của X chứa A, $D^*(A)\cap$ $\complement B$ là tập hợp loại một.

Cho U là hợp của các tập con mở V của X sao cho $A\cap V$ là tập hợp loại một. Để một điểm $x$ thuộc U, điều kiện cần và đủ là nó có một lân cận V sao cho $A\cap V$ là tập hợp loại một. Do đó ta có $U =\complement D(A)$ và vì vậy D(A) là một tập con đóng của X. Theo phép dựng, không gian con U có một phủ bởi các tập con mở mà giao của chúng với A là tập hợp loại một. Theo bổ đề 1, áp dụng cho không gian tôpô U và tập con $A\cap U$, $A\cap U$ là tập hợp loại một trong U, do đó cũng trong X. Điều này chứng minh mệnh đề a), vì theo phép dựng, mọi tập con mở V của X sao cho $A\cap V$ là tập hợp loại một đều được chứa trong U.

Mệnh đề b) suy ra ngay lập tức từ điều này.

c) Ta có $D^*(A) = A\cup D(A) = (A\cap U)\cup D(A)$. Tập hợp D(A) đóng, do đó khả tiếp cận (IV, p. 361); tập con loại một $A\cap U$ cũng vậy. Do đó $D^*(A)$ là khả tiếp cận (loc. cit.).

d) Cho B là một tập con tiếp cận được của X chứa A. Phần bù $\complement B$ của nó khi đó là một tập con tiếp cận được của X (loc. cit.) và do đó tồn tại một tập con mở V của X sao cho $V\cap B$ và $\complement V\cap \complement B$ là thưa. Vì $A\subset B$, $V\cap A$ vẫn là thưa, do đó $V\subset U$. Vì $\complement U\cap \complement B$ được chứa trong $\complement V\cap \complement B$, nó cũng là một tập con thưa của X. Cuối cùng, các phép bao hàm

$$
D^*(A)\cap \complement B =((A\cap U)\cap \complement B)\cup (\complement U\cap \complement B)\subset (A\cap U)\cup (\complement U\cap \complement B)
$$

chỉ ra rằng $D^*(A)\cap \complement B$ là một tập con thưa của X.

#### Nhận xét 1 {#ta-iv-s2-n4-rem-1 .statement tag=021D}

Cho G là một nhóm tôpô và cho A là một tập con thưa của G. Giả sử rằng A chứa một tập con mở khác rỗng U của G và cho $y$ là một điểm của U. Khi đó U là thưa và với mọi $x\in G,xy^{-1}U$ là một lân cận của $x$ trong G. Do đó mọi điểm của G đều có một lân cận thưa, do đó G là thưa (IV, p. 360, bổ đề 1).

Ngược lại, nếu G không thưa, mọi tập con thưa đều có phần trong rỗng và G là một không gian Baire. Vì một không gian Baire không thưa, điều này chứng minh mệnh đề sau: Để một nhóm tôpô là một không gian Baire, điều kiện cần và đủ là nó không thưa.

#### Mệnh đề 7 {#ta-iv-s2-prop-7 .statement tag=021E}

Cho X là một không gian tách. Mọi không gian con Souslinian (TG, IX, p. 59, định nghĩa 2) của X đều là tiếp cận được.

Cho S là một không gian con Souslinian của X. Theo định nghĩa, tồn tại một không gian mêtric đầy đủ P kiểu đếm được và một ánh xạ toàn ánh liên tục $g$ từ P lên S. Theo TG, IX, p. 64, bổ đề 3, tồn tại một sàng $C = (C_n, p_n, \varphi_n)_{n\in\mathbf{N}}$ của không gian mêtric P.

Với mỗi số nguyên $n$ và mỗi $c\in C_n$, ký hiệu $F_n(c)$ là ảnh của tập hợp $\varphi_n(c)$ qua $g$; ta cũng đặt $F^*_n(c) = D^*(F_n(c))$ và

$$
G_n(c) = F^*_n(c)\cap \complement \bigcup_{c'\in\overset{-1}{p_{n}}(c)}F^*_{n+1}(c') \tag{1}
$$

Với mỗi $c\in C_n,F^*_n(c)$ là tiếp cận được (IV, p. 361, bổ đề 2, c)). Vì $C_{n+1}$ là đếm được, hợp của các tập con tiếp cận được $F^*_{n+1}(c')$, trong đó $c'$ chạy qua $\overset{-1}{p_{n}}(c)$, lại là một tập con tiếp cận được của X. Nó chứa hợp của các $F_{n+1}(c')$, tập hợp này bằng $F_n(c)$. Do đó (loc. cit., d)), $G_n(c)$ là một tập con thưa của X. Hợp G của các tập con $G_n(c)$, với $n\in \mathbf{N}$ và $c\in C_n$, do đó là một tập con thưa của X.

Cho $c_0\in C_0$ và cho $x$ là một phần tử của $F^*_0(c_0)\cap \complement G$; ta hãy chứng minh rằng $x\in F_0(c_0)$. Vì $x\notin G_0(c_0)$ và $x\in F^*_0(c_0)$, tồn tại $c_1\in \overset{-1}{p_{0}}(c_0)$ sao cho $x\in F^*_1(c_1)$, theo quan hệ (1). Bằng quy nạp, tồn tại một phần tử $c= (c_n)_n$ của $\prod_nC_n$ sao cho, với mọi số nguyên $n\in \mathbf{N}$, ta có $x\in F^*_n(c_n)$ và $p_n(c_{n+1}) =c_n$.

Các tập con $\varphi_n(c_n)$ tạo thành một cơ sở của một lọc Cauchy trong P; lọc này hội tụ đến một điểm $p$ của P, vì P là đầy đủ. Ảnh của lọc này qua $g$ là một lọc F trên X, có cơ sở là tập hợp các $F_n(c_n)$ với $n\in \mathbf{N}$, lọc này hội tụ đến $g(p)$. Vì $F^*_n(c_n)$ được chứa trong $\overline{F_n(c_n)}$ và $x$ thuộc về mỗi $F_n(c_n)$, $x$ là một điểm bám của F, do đó $x=g(p)$ vì không gian X là tách được (TG, I, p. 52, mệnh đề 1). Điểm $p$ thuộc về $\overline{\varphi_1(c_1)}$, do đó thuộc về $\varphi_0(c_0)$. Do đó, $x\in F_0(c_0)$.

Do đó, tập hợp $F^*_0(c_0)$ - $F_0(c_0)$ được chứa trong G. Vì vậy nó là một tập con thưa của X, do đó cũng là một tập con tiếp cận được. Vì $F_0(c_0) = F^*_0(c_0)$ - $(F^*_0(c_0)$ - $F_0(c_0))$ và $F^*_0(c_0)$ là tiếp cận được, $F_0(c_0)$ là tiếp cận được, bởi vì các tập con tiếp cận được của X tạo thành một bộ lạc. Vì $C_0$ là đếm được, tập hợp S là hợp của các $F_0(c_0)$, với $c_0\in C_0$, lại là tiếp cận được.

### 5. Các quan hệ tương đương thưa trong các không gian Polish

#### Bổ đề 3 {#ta-iv-s2-lem-3 .statement tag=021F}

Cho $(U_i)_{i\in I}$ là một họ hữu hạn các tập con mở khác rỗng của một không gian tôpô X và cho O là một tập con mở trù mật của $X\times X$. Tồn tại một họ $(V_i)_{i\in I}$ các tập con mở khác rỗng của X sao cho $V_i\subset U_i$ với mọi $i\in I$ và sao cho $V_i\times V_{i'}\subset O$ với mọi cặp $(i, i')$ gồm các phần tử phân biệt của I.

Với mỗi cặp $(j_1, j_2)$ gồm các phần tử phân biệt của I, tập hợp các họ $(x_i)\in X^I$ sao cho $(x_{j_1}, x_{j_2})\in O$ là một tập con mở trù mật của $X^I$. Giao Ω của các tập mở này, khi $(j_1, j_2)$ chạy qua tập hữu hạn các cặp gồm các phần tử phân biệt của I, do đó là một tập con mở trù mật của $X^I$. Do đó, $\Omega \cap \prod_{i\in I}U_i$ là một tập con mở khác rỗng của $X^I$, vì thế chứa một tập con mở của $X^I$ có dạng $\prod_{i\in I}V_i$, trong đó với mỗi $i\in I$, $V_i$ là một tập con mở, khác rỗng, của $U_i$. Điều này chứng minh bổ đề.

#### Mệnh đề 8 {#ta-iv-s2-prop-8 .statement tag=021G}

Cho P là một không gian tôpô Polish khác rỗng và cho R là một quan hệ tương đương trong P mà đồ thị của nó là một tập con thưa của $P\times P$. Tồn tại một ánh xạ liên tục đơn ánh của tập $\{0,1\}^{\mathbf{N}}$, được trang bị tôpô tích của các tôpô rời rạc, vào P mà ảnh của nó gặp mỗi lớp tương đương đối với R tại nhiều nhất một điểm.

Trang bị cho không gian P một mêtric $d$ tương thích với tôpô của nó và theo đó nó là đầy đủ. Cho $(A_n)_{n\in\mathbf{N}}$ là một dãy tăng các tập con đóng của $P\times P$, có phần trong rỗng, sao cho đồ thị $\Gamma_R$ của quan hệ R được chứa trong hợp của các $A_n$.

Cho $\mathscr{O}$ là tập hợp các tập con mở khác rỗng của P. Ta sẽ xây dựng bằng quy nạp một dãy $(f_n)_{n\in\mathbf{N}}$, trong đó với mọi $n$, $f_n$ là một ánh xạ của $\{0,1\}^n$ vào $\mathscr{O}$, thỏa mãn các tính chất sau :

(i) Với mọi $n\geqslant 1$, mọi $x\in  \{0,1\}^{n-1}$ và mọi $t\in  \{0,1\}$, bao đóng của tập mở $f_n(x, t)$ được chứa trong $f_{n-1}(x)$;

(ii) Với mọi $x\in  \{0,1\}^n$, ta có diam($f_n(x)$)$\leqslant 2^{-n}$;

(iii) Với mọi $n\geqslant 1$ và mọi cặp $(x, x')$ gồm các phần tử phân biệt của $\{0,1\}^n,f_n(x)\times f_n(x')$ không giao với $A_{n-1}$.

Chọn một tập mở khác rỗng U của X có đường kính $\leqslant 1$ và định nghĩa $f_0$ là ánh xạ hằng có ảnh $\{U\}$. Giả sử các ánh xạ $f_0, . . . , f_n$ đã được xây dựng.

Gọi $p:\{0,1\}^{n+1}\rightarrow  \{0,1\}^n$ là ánh xạ được định nghĩa bởi $p(x_0, . . . , x_n) =$ $(x_0, . . . , x_{n-1})$. Theo bổ đề 3 ở trên, áp dụng cho họ các tập mở $(f_n(p(x)))$ với $x\in  \{0,1\}^{n+1}$ và cho tập mở trù mật $\complement A_n$ của $P\times P$, tồn tại một họ $(g(x))_{x\in \{0,1\}^{n+1}}$ các tập mở khác rỗng của P sao cho $g(x)\subset f_n(p(x))$ với mọi $x$ và sao cho $(g(x)\times g(x'))\cap A_n$ rỗng đối với mọi cặp $(x, x')$ gồm các phần tử phân biệt của $\{0,1\}^{n+1}$. Khi đó ta định nghĩa ánh xạ $f_{n+1}$ bằng cách chọn, với mỗi phần tử $x\in  \{0,1\}^{n+1}$, một tập con mở khác rỗng của $g(x)$ có đường kính $\leqslant 2^{-n-1}$ và có bao đóng được chứa trong $g(x)$.

Với mọi phần tử $x= (x_n)_{n\in\mathbf{N}}$ của $\{0,1\}^{\mathbf{N}}$, dãy các tập hợp $(f_n(x_0, . . . , x_{n-1}))_{n\in\mathbf{N}}$ là một dãy giảm các tập con mở của X, mỗi tập trong đó chứa bao đóng của tập tiếp theo và có đường kính dần về 0; giao của dãy tập hợp này do đó thu gọn thành một điểm (TG, II, p. 15), mà ta ký hiệu là $f(x)$. Nếu hai điểm $x,x'$ của $\{0,1\}^{\mathbf{N}}$ thỏa mãn $x_i=x'_i$ với $i\leqslant n$, thì có $d(f(x), f(x'))\leqslant 2^{-n}$. Do đó, ánh xạ $f:\{0,1\}^{\mathbf{N}}\rightarrow P$ là liên tục. Cho $x$ và $x'$ là các phần tử phân biệt của $\{0,1\}^{\mathbf{N}}$. Với $n\in \mathbf{N}$ sao cho $(x_0, . . . , x_n)=\not$ $(x'_0, . . . , x'_n)$, tập mở $f_{n+1}(x_0, . . . , x_n)\times f_{n+1}(x'_0, . . . , x'_n)$ rời khỏi $A_n$, theo định nghĩa của $f_{n+1}$, do đó cặp $(f(x), f(x'))$ không thuộc $A_n$. Suy ra rằng $f(x)$ và $f(x')$ không tương đương đối với quan hệ R. Do đó, $f$ là đơn ánh và ảnh của nó gặp mỗi lớp tương đương đối với R nhiều nhất tại một điểm. Mệnh đề được chứng minh.

### 6. Lực lượng của các nhóm Poincaré

#### Mệnh đề 9 {#ta-iv-s2-prop-9 .statement tag=021H}

Cho X là một không gian tôpô không thể tháo gỡ được và cho $\mathscr{W}$ là một cơ sở cho tôpô của X. Với mọi điểm $x$ của X, lực lượng của nhóm $\pi_1(X, x)$ bị chặn trên bởi sup(Card($\mathscr{W}$), Card($\mathbf{N}$)). Đặc biệt, nhóm Poincaré của một không gian mêtric kiểu đếm được và không thể tháo gỡ được là đếm được.

Thực vậy, không gian $\lambda_x(X)$ được trang bị ánh xạ đầu mút là một phủ liên thông của X mà thớ tại $x$ là $\pi_1(X, x)$. Mệnh đề đó suy ra từ I, p. 40, th. 3.

#### Bổ đề 4 {#ta-iv-s2-lem-4 .statement tag=021I}

Cho X là một không gian Baire, cho G là một nhóm tôpô tác động liên tục lên X và cho B là một tập con tiếp cận được của X không thưa. Tập hợp các điểm $g\in G$ sao cho $B\cap gB=\not\emptyset$ là một lân cận của phần tử đơn vị của G.

Vì B là tiếp cận được, $\complement B$ cũng là tiếp cận được, vì tập hợp các tập con tiếp cận được của X là một tộc. Do đó tồn tại một tập con mở U của X sao cho $U\cap \complement B$ và $B\cap \complement U$ là thưa trong X.

Cho V là một lân cận của phần tử đơn vị của G và W là một tập con mở khác rỗng của X được chứa trong U sao cho $V\cdot W\subset U$. Với mọi $g\in V$, $U\cap gU$ là khác rỗng.

Cho $g\in G$ sao cho $B\cap gB$ là rỗng. Các hệ thức

$$
U\cap gU = (U\cap gU)\cap \complement (B\cap gB)
$$

$$
= (U\cap gU)\cap (\complement B\cup g\complement B)
$$

$$
= (U\cap gU\cap \complement B)\cup (U\cap gU\cap g\complement B)
$$

$$
\subset (U\cap \complement B)\cup g(U\cap \complement B)
$$

suy ra rằng $U\cap gU$ là thưa trong X. Vì đây là một tập con mở và X là một không gian Baire, nó là rỗng. Do đó $g\notin V$, điều này chứng minh bổ đề.

#### Định lý 2 (Shelah[^1]) {#ta-iv-s2-thm-2 .statement tag=021J}

Cho X là một không gian Polish liên thông được liên thông địa phương bởi các cung, và cho $x$ là một điểm của X. Nếu X không thể tháo gỡ được, nhóm $\pi_1(X, x)$ có lực lượng của continuum.

Cho $d$ là một mêtric xác định tôpô của X mà theo đó nó là đầy đủ. Giả sử rằng X không thể tháo gỡ được. Khi đó tồn tại một điểm $a\in X$ và, với mọi số nguyên $n\geqslant 0$, một vòng $c_n$ tại $a$ trong X có ảnh có đường kính $\leqslant 2^{-n}$ và có lớp trong $\pi_1(X, a)$ là không tầm thường.

Ta ký hiệu K là tập hợp $\{0,1\}^{\mathbf{N}}$ và trang bị cho nó tôpô tích, không gian $\{0,1\}$ được trang bị tôpô rời rạc. Với mọi phần tử $\varepsilon = (\varepsilon_n)$ của K, cho $c_{\varepsilon}$ là ánh xạ của $\mathbf{I}$ vào X được xác định bởi $c_{\varepsilon}(0) =a$ và, với $2^{-n-1}\leqslant t\leqslant 2^{-n},c_{\varepsilon}(t) =c_n(2^{n+1}t-1)$ nếu $\varepsilon_n= 1$ và $c_{\varepsilon}(t) =a$ trong trường hợp khác. Ta có $c_{\varepsilon}(0) =c_{\varepsilon}(1) =a$. Ánh xạ $c_{\varepsilon}$ liên tục tại mọi điểm $t\in ]0,1]$. Nó cũng liên tục tại 0, vì $d(a, c_{\varepsilon}(t))\leqslant 2^{-n}$ nếu $t\in [0,2^{-n}]$. Do đó ánh xạ $c_{\varepsilon}$ là một vòng trong X tại $a$.

Nếu $\varepsilon$ và $\varepsilon '$ là các phần tử của K sao cho $(\varepsilon_0, . . . , \varepsilon_n) = (\varepsilon '_0, . . . , \varepsilon '_n)$, thì $c_{\varepsilon}(t) =c_{\varepsilon'}(t)$ với mọi $t\in [2^{-n-1},1]$ và $d(c_{\varepsilon}(t), c_{\varepsilon'}(t))\leqslant$ $d(a, c_{\varepsilon}(t)) +d(a, c_{\varepsilon'}(t))\leqslant 2^{-n}$ nếu $t\in [0,2^{-n-1}]$. Suy ra rằng ánh xạ $\varepsilon \mapsto c_{\varepsilon}$ của K vào không gian $\Omega_a(X)$ là liên tục, khi không gian $\Omega_a(X)$ được trang bị tôpô hội tụ compact.

Cho $\Gamma \subset K\times K$ là tập hợp các cặp $(\varepsilon , \varepsilon ')$ sao cho $c_{\varepsilon}$ đồng luân ngặt với $c_{\varepsilon'}$. Nó là đồ thị của một quan hệ tương đương R trên K.

#### Bổ đề 5 {#ta-iv-s2-lem-5 .statement tag=021K}

Tập hợp Γ là một tập hợp không đâu trù mật trong $K\times K$.

Cho Z là không gian $K\times K\times \mathscr{C}_c(\mathbf{I}\times \mathbf{I}; X)$. Tôpô của không gian $\mathscr{C}_c(\mathbf{I}\times \mathbf{I}; X)$ được xác định bởi khoảng cách $\delta$ cho bởi $\delta (h, h') =$ sup$_{u\in\mathbf{I}\times\mathbf{I}}d(h(u), h'(u))$ và nó đầy đủ đối với khoảng cách này (TG, X, p. 20, hệ quả và TG, X, p. 9, Hệ quả 1); sau TG, X, p. 24, Định lý 1, tôpô này có kiểu đếm được. Do đó, không gian $\mathscr{C}_c(\mathbf{I}\times \mathbf{I}; X)$ là một không gian Polish. Điều tương tự cũng đúng với không gian Z, vì K là một không gian Polish (TG, IX, p. 57, Mệnh đề 1).

Cho H là tập con của Z gồm các bộ ba $(\varepsilon , \varepsilon ', h)$ sao cho $h$ là một đồng luân ngặt nối $c_{\varepsilon}$ với $c_{\varepsilon'}$. Các ánh xạ từ Z vào $X^2$ được cho bởi $a_t: (\varepsilon , \varepsilon ', h)\mapsto (c_{\varepsilon}(t), h(t,0)),b_t: (\varepsilon , \varepsilon ', h)\mapsto$ $(c_{\varepsilon'}(t), h(t,1))$ và $c_t: (\varepsilon , \varepsilon ', h)\mapsto (h(0, t), h(1, t))$ là liên tục, với mọi $t\in \mathbf{I}$, vì ánh xạ $\varepsilon \mapsto c_{\varepsilon}$ từ K vào $\Omega_a(X)$ là liên tục, và tương tự các ánh xạ $h\mapsto h(s, t)$ từ $\mathscr{C}_c(\mathbf{I}\times \mathbf{I}; X)$ vào X.

Theo định nghĩa, H là giao của các tập hợp $\overset{-1}{a_{t}}(\Delta_X),\overset{-1}{b_{t}}(\Delta_X)$ và $\overset{-1}{c_{t}}((a, a))$, với $t\in \mathbf{I}$, trong đó $\Delta_X$ ký hiệu đường chéo của X. Điều này chứng minh rằng H là một tập con đóng của Z.

Suy ra H là một không gian Polish. Cho $p: Z\rightarrow K\times K$ là phép chiếu chính tắc; theo định nghĩa ta có $\Gamma  =p(H)$. Vì $K\times K$ là Hausdorff, Γ là một tập hợp Souslin của $K\times K$ (TG, IX, p. 59, định nghĩa 2). Sau IV, p. 362, Mệnh đề 7, nó là một tập hợp khả tiếp cận của $K\times K$.

Giả sử Γ không là một tập hợp không đâu trù mật. Không gian $K\times K$ là một không gian tôpô compact và do đó là một không gian Baire (TG, IX, p. 55, Định lý 1). Trang bị cho nhóm $G_0$ các phép hoán vị của tập hợp $\{0,1\}$ tôpô rời rạc; cho nhóm tôpô tích $G = G^{\mathbf{N}}_0$ tác động theo đường chéo trên $K =\{0,1\}^{\mathbf{N}}$. Khi đó nhóm G tác động liên tục trên $K\times K$ bởi ánh xạ $(g,(x, y))\mapsto (x, g\cdot y)$. Sau Bổ đề 4, tập hợp V gồm các phần tử $g\in G$ sao cho $\Gamma \cap g\cdot \Gamma =\not\emptyset$ là một lân cận của phần tử đơn vị của G.

Cho $g\in V$; cho $(\varepsilon , \varepsilon ')\in \Gamma \cap g\Gamma$. Vì $(\varepsilon , \varepsilon ')\in \Gamma$, ta có $R\{\varepsilon , \varepsilon '\}$; vì $(\varepsilon , \varepsilon ')\in g\Gamma ,g^{-1}\cdot (\varepsilon , \varepsilon ') = (\varepsilon , g^{-1}\varepsilon ')\in \Gamma$, nên $R\{\varepsilon , g^{-1}\varepsilon '\}$. Như vậy ta đã chứng minh rằng, với mọi $g\in V$, tồn tại $\varepsilon \in K$ sao cho $\varepsilon$ và $g\varepsilon$ tương đương đối với R.

Với $m\in \mathbf{N}$, ký hiệu $\tau_m$ là phần tử của G mà mọi số hạng của nó đều bằng $e$ ngoại trừ số hạng có chỉ số $m$, số hạng này bằng phần tử không tầm thường $\tau$ của $G_0$. Tồn tại một số nguyên $m$ sao cho $\tau_m$ thuộc V; khi đó, cho $\varepsilon \in K$ sao cho $\varepsilon$ và $\varepsilon '=\tau_m\cdot \varepsilon$ là tương đương đối với R. Điều này kéo theo rằng các vòng $c_{\varepsilon}$ và $c_{\varepsilon'}$ đồng luân chặt. Theo phép dựng, các vòng này trùng nhau trên các khoảng $[0,2^{-m-1}]$ và $[2^{-m},1]$; trên khoảng $[2^{-m-1},2^{-m}]$, một vòng là ánh xạ hằng có ảnh là $a$ và vòng kia là ánh xạ $t\mapsto c_m(2^{m+1}t-1)$. Suy ra rằng $c_m$ đồng luân chặt với vòng hằng có ảnh $\{a\}$, do đó là một mâu thuẫn. Bổ đề 5 được chứng minh.

Bây giờ ta hoàn tất chứng minh định lý 2. Theo Mệnh đề 8, tồn tại một ánh xạ liên tục đơn ánh $\gamma$ từ $\{0,1\}^{\mathbf{N}}$ vào K có ảnh gặp mỗi lớp tương đương đối với R tại nhiều nhất một điểm. Nếu $k$ và $k'$ là các phần tử phân biệt của $\{0,1\}^{\mathbf{N}}$, các vòng $c_{\gamma(k)}$ và $c_{\gamma(k')}$ không đồng luân chặt trong X, và ánh xạ $\{0,1\}^{\mathbf{N}}\rightarrow \pi_1(X, a)$ cho bởi $k\mapsto [c_{\gamma(k)}]$ là đơn ánh. Đặc biệt, Card($\pi_1(X, a)$)$\geqslant$ Card($\{0,1\}^{\mathbf{N}}$) $=$ Card($\mathfrak{P}(\mathbf{N})$). Vì X là một không gian tôpô mêtric được phân loại đếm được, điều tương tự cũng đúng với $\Omega_a(X)$ (TG, X, p. 24, đl. 1). Do đó $\Omega_a(X)$ là đồng phôi với một không gian con của $[0,1]^{\mathbf{N}}$ (TG, IX, p. 18, mđ. 12) và

Card(Ω$_a(X)$)$\leqslant$ Card([0$,1]^{\mathbf{N}}$) $=$ Card($\mathfrak{P}(\mathbf{N})^{\mathbf{N}}$)

= Card($\mathfrak{P}(\mathbf{N}\times \mathbf{N})$) $=$ Card($\mathfrak{P}(\mathbf{N})$).

A fortiori, Card($\pi_1(X, a)$)$\leqslant$ Card($\mathfrak{P}(\mathbf{N})$). Khi đó, từ Hệ quả 2 của E, III, p. 25, suy ra rằng $\pi_1(X, a)$ có lũy thừa của continuum, điều phải chứng minh.

#### Ví dụ {#ta-iv-s2-n6-exa-1 .statement tag=021L}

Cho P là không gian tôpô là hợp của các đường tròn có tâm $(2/n,0)$ đi qua gốc của mặt phẳng $\mathbf{R}^2$, với $n\geqslant$ 1 (III, p. 336, Bài tập 6). Nhóm Poincaré của P có lũy thừa của continuum (III, p. 338, Bài tập 9).

## BÀI TẬP {#ta-iv-s2-exercises}

Xem các [bài tập cho § 2](exercises/s2/).

[^1]: Xem "Can the fundamental (homotopy) group of a space be the rationals ?", Proc. Amer. Math. Soc. 103 (1988), No. 2, p. 627–632. Chứng minh tiếp theo dựa trên bài báo của J. Pawlikowski, "The fundamental group of a compact metric space", Proc. Amer. Math. Soc. 126 (1998), No. 10, p. 3083–3087.
