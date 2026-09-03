---
book: ts
book_title: Théories spectrales
chapter: I
chapter_title: ALGÈBRES NORMÉES
section: 1
section_title: Spectres et caractères
lang: vi
source: ts-i-ii-fr
book_pages: TS I.1-TS I.15, TS I.153-TS I.154
pdf_pages: 0014-0028, 0166-0167
extraction: native
subsections:
    - "no": 1
      title: Algèbres unifères
      page: 1
      pdf_page: 14
    - "no": 2
      title: Spectre d’un élément dans une algèbre unifère
      page: 2
      pdf_page: 15
    - "no": 3
      title: Résolvante
      page: 3
      pdf_page: 16
    - "no": 4
      title: Spectre d’un élément dans une algèbre
      page: 4
      pdf_page: 17
    - "no": 5
      title: Sous-algèbres pleines
      page: 5
      pdf_page: 18
    - "no": 6
      title: Caractères d’une algèbre unifère commutative
      page: 6
      pdf_page: 19
    - "no": 7
      title: Cas des algèbres sans élément unité
      page: 9
      pdf_page: 22
    - "no": 8
      title: Idéaux primitifs
      page: 11
      pdf_page: 24
statements: 33
exercises: 8
content_sha256: c155100aeeb55ef772953d6dffef6371465c4540ba0820b0c3065483a6dadf18
translated_from: content/en-mt/ts/I/01_s1_spectres_et_caracteres.md
source_lang: en-mt
translation_method: machine
source_content_sha256: ba4faed48a44431108215f0ef740029a61d76cccd70f4a61007ff33d6daafaad
translation_model: gpt-5-6-mini
translation_run: translate-vi-ff0e9d5f
glossary_version: 34
glossary_terms_sha256: 4ecc7c4a389f5005017308f55caab959ebed77e53a634d81ce281d8aa27bc554
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 1. PHỔ VÀ CÁC KÝ TỰ

Trong đoạn này, chữ K ký hiệu một trường giao hoán. Nếu E và F là các không gian vectơ trên K, ta viết $E\otimes F = E\otimes_KF$.

### 1. Các đại số có đơn vị

Một đại số có đơn vị trên K được định nghĩa là một cặp $(A, e)$ trong đó A là một đại số trên K với một phần tử đơn vị và $e$ là phần tử đơn vị của A. Vì $e$ được xác định duy nhất bởi A, đôi khi ta sẽ nói, bằng sự lạm dụng ngôn ngữ, rằng A là một đại số có đơn vị. Nếu $(A, e)$ và $(A', e')$ là các đại số có đơn vị, một cấu xạ có đơn vị của $(A, e)$ vào $(A', e')$ được định nghĩa là một cấu xạ $\varphi$ của A vào $A'$ sao cho $\varphi (e) =e'$. Một đại số con có đơn vị của $(A, e)$ là một cặp $(A', e)$, trong đó $A'$ là một đại số con của A chứa $e$.

Ta sẽ thường ký hiệu phần tử đơn vị bằng 1.

#### Bổ đề 1 {#ts-i-s1-lem-1 .statement tag=024R}

Cho A là một đại số. Với mọi phần tử lũy đẳng $j$ của A, không gian con $jAj$ của A là tập hợp các $x\in A$ sao cho $xj=jx=x$. Nó là một đại số con của A có $j$ làm phần tử đơn vị.

Chứng minh là sơ cấp.

### 2. Phổ của một phần tử trong một đại số có đơn vị

#### Định nghĩa 1 {#ts-i-s1-def-1 .statement tag=024S}

Cho A là một đại số có đơn vị trên K, và cho $e$ là phần tử đơn vị của nó. Với mọi $x\in A$, phổ của $x$ đối với A là tập hợp các $\lambda \in K$ sao cho $\lambda e-x$ không khả nghịch.

Phổ của $x$ sẽ được ký hiệu bởi Sp$_A(x)$, hoặc Sp($x$) nếu không thể xảy ra sự nhầm lẫn. Phần bù của Sp$_A(x)$ trong K được gọi là tập hợp giải của $x$.

#### Nhận xét 1 {#ts-i-s1-n2-rem-1 .statement tag=024T}

Nếu $A =\{0\}$, thì Sp(0) $=\emptyset$.

#### Nhận xét 2 {#ts-i-s1-n2-rem-2 .statement tag=024U}

Nếu $A\not=\{0\}$, thì Sp($\lambda e$) $=\{\lambda \}$ với mọi $\lambda \in K$.

#### Nhận xét 3 {#ts-i-s1-n2-rem-3 .statement tag=024V}

Để $x\in A$ là khả nghịch, điều kiện cần và đủ là $0\notin$ Sp($x$).

#### Nhận xét 4 {#ts-i-s1-n2-rem-4 .statement tag=024W}

Cho $R\in K(X)$ là một phân thức hữu tỉ và cho $x\in A$ là một phần tử có thể thế vào R, nghĩa là (A, IV, p. 20), tồn tại P và $Q\in K[X]$ sao cho $R = P/Q$ và $Q(x)$ khả nghịch; khi đó ta có thể tạo thành phần tử $R(x) = P(x)\cdot Q(x)^{-1}= Q(x)^{-1}\cdot P(x)$ của A; nó không phụ thuộc vào lựa chọn P và Q. Ta có $0\notin$ Q(Sp($x$)), do đó mọi phần tử của Sp($x$) đều có thể thế vào R.

Ta có R(Sp($x$))$\subset$ Sp(R($x$)). Thật vậy, cho $\lambda \in$ Sp($x$); tồn tại một đa thức $P_1$ sao cho $R(\lambda )-R(X) = (\lambda -X)P_1(X)/Q(X)$; khi đó, $R(\lambda )e-$ $R(x) = (\lambda e-x)(P_1(x)/Q(x))$, do đó $R(\lambda )-R(x)$ không khả nghịch, suy ra $R(\lambda )\in$ Sp(R($x$)).

Ngược lại, giả sử trường K đóng đại số. Trước hết, giả sử R không hằng và ta chứng minh rằng Sp(R($x$)) $=$ R(Sp($x$)). Lấy $\mu\in$ Sp(R($x$)). Vì R không hằng, $P-\mu Q$ không phải là đa thức không; viết $\mu Q-P =\alpha \prod(\lambda_i-X)$ thành một phân tích thành các thừa số bậc 1, sao cho $\mu e-R(x) =$ $\alpha \prod(\lambda_ie-x)Q(x)^{-1}$. Vì $\mu e-R(x)$ không khả nghịch, tồn tại $i$ sao cho $\lambda_ie-x$ không khả nghịch, do đó $\lambda_i\in$ Sp($x$), và khi đó $R(\lambda_i) =\mu\in$ R(Sp($x$)).

Khi R hằng, đẳng thức Sp(R($x$)) $=$ R(Sp($x$)) cũng đúng, với điều kiện Sp($x$) khác rỗng.

#### Nhận xét 5 {#ts-i-s1-n2-rem-5 .statement tag=024X}

Giả sử đại số A khác không. Cho $x\in A$ là một phần tử lũy linh. Cho $n$ là một số nguyên sao cho $x^n= 0$. Phổ của $x^n$ thu gọn về 0, do đó điều tương tự cũng đúng đối với phổ của $x$ theo Nhận xét 4.

#### Nhận xét 6 {#ts-i-s1-n2-rem-6 .statement tag=024Y}

Cho A và B là các đại số có đơn vị trên K và $\varphi : A\rightarrow B$ là một cấu xạ có đơn vị. Với mọi $x\in A$, ta có Sp$_B(\varphi (x))\subset$ Sp$_A(x)$.

#### Nhận xét 7 {#ts-i-s1-n2-rem-7 .statement tag=024Z}

Cho A là một đại số có đơn vị, R là căn của nó (A, VIII, p. 150, Định nghĩa 2), và $\varphi$ là cấu xạ chính tắc của A lên $B = A/R$. Nếu $x\in A$, ta có Sp$_B(\varphi (x)) =$ Sp$_A(x)$. Thực vậy, chỉ cần chứng minh rằng nếu $\varphi (x)$ khả nghịch trong B thì x khả nghịch trong A. Bây giờ, nếu $y\in A$ sao cho $\varphi (x)\varphi (y) =\varphi (y)\varphi (x) =\varphi (e)$, thì $xy\in e+ R,yx\in e+ R$, do đó xy và yx khả nghịch (A, VIII, p. 151, Định lý 1) và do đó x khả nghịch. Đặc biệt, nếu $x\in R$, ta có Sp$_A(x) =\{0\}$ nếu $A\not=\{0\}$.

#### Nhận xét 8 {#ts-i-s1-n2-rem-8 .statement tag=0250}

Cho $(B_i)_{i\in I}$ là một họ các đại số có đơn vị, với $B_i= (A_i, e_i)$ đối với $i\in I$. Đặt $A =\prod_iA_i,e= (e_i)_{i\in I}$. Khi đó $(A, e)$ là một đại số có đơn vị được gọi là tích của các $B_i$. Nếu $x= (x_i)_{i\in I}\in A$, ta có Sp$_A(x) =\bigcup_i$ Sp$_{A_i}(x_i)$.

#### Ví dụ 1 {#ts-i-s1-n2-exa-1 .statement tag=0251}

Cho X là một tập hợp và $A = K^X$ là đại số các hàm nhận giá trị trong K xác định trên X. Phổ của một phần tử f của A là tập hợp các giá trị của f.

#### Ví dụ 2 {#ts-i-s1-n2-exa-2 .statement tag=0252}

Cho A là một đại số có đơn vị và hạng hữu hạn trên K. Để $x\in A$ là khả nghịch, điều kiện cần và đủ là ánh xạ tuyến tính $y\mapsto xy$ của A vào A có định thức khác không. Suy ra rằng phổ của $x$ là tập hợp các nghiệm của đa thức đặc trưng của $x$ (A, III, p. 110). Nếu A là đại số tự đồng cấu của một không gian vectơ hữu hạn chiều V trên K, thì phổ của $x$ do đó là tập hợp các giá trị riêng của $x$. Điều này không phải luôn đúng khi V có chiều vô hạn (xem I, p. 153, bài tập 2).

### 3. Giải thức

#### Định nghĩa 2 {#ts-i-s1-def-2 .statement tag=0253}

Cho A là một đại số có đơn vị trên K và $x\in A$. Với mọi $\lambda \in K$ - Sp($x$), ta đặt

$$
R(x, \lambda ) = (\lambda e-x)^{-1}
$$

Ánh xạ từ K - Sp($x$) vào A được cho bởi $\lambda \mapsto R(x, \lambda )$ được gọi là giải thức của $x$.

Với $x$ cố định, các giá trị của $R(x, \lambda )$ từng đôi một giao hoán. Nếu $\lambda , \mu\in K$, ta có:

$$
(\lambda -\mu)e= (\lambda e-x)-(\mu e-x)
$$

do đó, nếu $\lambda , \mu\in K$ - Sp($x$), ta có quan hệ

$$
(\lambda -\mu)R(x, \lambda )R(x, \mu) = R(x, \mu)-R(x, \lambda ) \tag{1}
$$

Nếu $x, y\in A$ và $\lambda \in K$, ta có:

$$
y-x= (\lambda e-x)-(\lambda e-y)
$$

do đó, nếu $\lambda \in K$ - (Sp($x$)$\cup$ Sp($y$)), ta có quan hệ

$$
R(y, \lambda )(y-x)R(x, \lambda ) = R(y, \lambda )-R(x, \lambda ) \tag{2}
$$

### 4. Phổ của một phần tử trong một đại số

Cho A là một đại số trên K. Nhắc lại (A, III, p. 4) rằng người ta định nghĩa trên không gian vectơ $\widetilde{A} = K\times A$ một cấu trúc đại số sao cho:

$$
(\lambda , a)(\mu, b) = (\lambda \mu, \lambda b+\mu a+ab)
$$

Đặt $e= (1,0)$. Khi đó $(\widetilde{A}, e)$ là một đại số có đơn vị được gọi là đại số suy ra từ A bằng phép nối một phần tử đơn vị. Đại số A được đồng nhất với iđêan hai phía $\{0\} \times A$ của $\widetilde{A}$; đại số A là giao hoán khi và chỉ khi $\widetilde{A}$ là giao hoán.

Nếu $A'$ là một đại số thứ hai trên K, $(\widetilde{A}', e')$ là đại số có đơn vị suy ra từ $A'$ bằng phép nối một phần tử đơn vị, và $\varphi$ là một cấu xạ từ A vào $A'$, thì tồn tại một và chỉ một cấu xạ có đơn vị từ $(\widetilde{A}, e)$ vào $(\widetilde{A}', e')$ mở rộng $\varphi$.

Cho A là một đại số trên K và $x\in$ A. Phổ của $x$ tương đối với A được định nghĩa là phổ của $x$ tương đối với đại số có đơn vị $\widetilde{A}$ suy ra từ A bằng phép nối một phần tử đơn vị. Tập hợp này sẽ được ký hiệu bởi Sp$'_A(x)$, hoặc Sp$'(x)$ nếu không gây nhầm lẫn. Ta có $0\in$ Sp$'_A(x)$ với mọi $x\in A$.

Nếu $\varphi$ là một cấu xạ từ A vào một đại số B, ta có Sp$'_B(\varphi (x))\subset$ Sp$'_A(x)$.

#### Nhận xét 1 {#ts-i-s1-n4-rem-1 .statement tag=0254}

Cho $(A,1)$ là một đại số có đơn vị. Nếu $x\in A$, ta có

Sp$'_A(x) =$ Sp$_A(x)\cup  \{0\}$. Thật vậy, ta kiểm tra được rằng $(e-1)\cdot A = A\cdot (e-1) = 0$, do đó $\widetilde{A}$ là đại số có đơn vị là tích của A và $K(e-1)$. Do đó mệnh đề của ta suy ra từ Nhận xét 8 của I, p. 3.

#### Nhận xét 2 {#ts-i-s1-n4-rem-2 .statement tag=0255}

Suy ra từ Nhận xét 1 rằng, nếu B là một đại số trên K và nếu $x\in B$, thì:

Sp$'_B(x) =$ Sp$_{\widetilde{B}}(x) =$ Sp$_{\widetilde{B}}(x)\cup  \{0\}=$ Sp$'_{\widetilde{B}}(x)$.

#### Nhận xét 3 {#ts-i-s1-n4-rem-3 .statement tag=0256}

Nếu $x$ thuộc căn của A (A, VIII, p. 430, định nghĩa 3), thì Sp$'_A(x) =\{0\}$. Điều này suy ra từ Nhận xét 7 của I, p. 3.

#### Mệnh đề 1 {#ts-i-s1-prop-1 .statement tag=0257}

Cho A là một đại số và $x, y\in A$. Ta có Sp$'(xy) =$ Sp$'(yx)$.

Bằng cách chuyển qua $\widetilde{A}$, ta rút gọn về trường hợp A có một phần tử đơn vị e. Khi đó chỉ cần chứng minh rằng, nếu $\lambda \not= 0$ sao cho $xy-\lambda e$ có một nghịch đảo u, thì $yx-\lambda e$ khả nghịch. Đặt $z=yux-e$. Vì $xyu=\lambda u+e$, ta có

$$
(yx-\lambda e)z=y(xyu)x-yx-\lambda yux+\lambda e
$$

$$
=y(\lambda u+e)x-yx-\lambda yux+\lambda e=\lambda e
$$

và tương tự $z(yx-\lambda e) =\lambda e$. Vì $\lambda \not= 0$, suy ra $yx-\lambda e$ khả nghịch.

Nếu A là một đại số có đơn vị và $x, y\in A$, mệnh đề trên suy ra rằng Sp($xy$)$\cup \{0\}=$ Sp($yx$)$\cup \{0\}$, nhưng có thể có Sp($xy$)$\not=$ Sp($yx$) (xem I, p. 153, bài tập 3).

### 5. Các đại số con đầy đủ

Cho A là một đại số có đơn vị trên K.

#### Định nghĩa 3 {#ts-i-s1-def-3 .statement tag=0258}

Một đại số con đầy đủ của A là một đại số con có đơn vị B sao cho mọi phần tử của B khả nghịch trong A đều khả nghịch trong B.

Nói cách khác, B là một đại số con đầy đủ của A khi và chỉ khi Sp$_B(x) =$ Sp$_A(x)$ với mọi $x\in B$.

Giao của một họ các đại số con đầy đủ của A là một đại số con đầy đủ của A.

Cho M là một tập con của A. Giao của các đại số con đầy đủ của A chứa M là đại số con đầy đủ nhỏ nhất của A chứa M; nó được gọi là đại số con đầy đủ của A sinh bởi M. Hoán tập $M'$ của M trong A là một đại số con đầy đủ của A (vì, nếu x khả nghịch trong A và giao hoán với M, thì $x^{-1}$ giao hoán với M). Do đó đối giao hoán tử kép $M''$ của M là một đại số con đầy đủ của A chứa đại số con đầy đủ của A sinh bởi M.

Nếu các phần tử của M giao hoán từng đôi một, ta có $M\subset M'$ và $M''\subset M'''$; do đó đại số $M''$ là giao hoán và khi đó điều tương tự cũng đúng đối với đại số đầy đủ sinh bởi M.

Một đại số con giao hoán cực đại của A là một đại số con đầy đủ, vì nó bằng hoán tập của nó.

#### Bổ đề 2 {#ts-i-s1-lem-2 .statement tag=0259}

Cho $(x_{\lambda})_{\lambda\in\Lambda}$ là một họ các phần tử của A giao hoán từng đôi một. Đại số con đầy đủ sinh bởi $(x_{\lambda})$ là tập hợp các phần tử có dạng $R((x_{\lambda}))$, trong đó $R\in K((X_{\lambda}))$ chạy qua tập hợp các phân thức hữu tỉ mà họ $(x_{\lambda})$ có thể thế vào.

Let B là đại số con đầy đủ của A được sinh bởi họ $(x_{\lambda})$, và ký hiệu $B_1$ là tập hợp các phần tử có dạng $R((x_{\lambda}))$, trong đó $R((X_{\lambda}))$ là một phân thức hữu tỉ mà $(x_{\lambda})$ có thể được thay thế vào. Tường minh, $B_1$ là tập hợp các phần tử của A có dạng $P((x_{\lambda}))Q((x_{\lambda}))^{-1}$, trong đó $P,Q\in K[(X_{\lambda})]$ và $Q((x_{\lambda}))$ khả nghịch trong A. Tập hợp $B_1$ là một đại số con có đơn vị của A chứa họ $(x_{\lambda})$. Nó là một đại số con đầy đủ: nếu $P((x_{\lambda}))Q((x_{\lambda}))^{-1}$ khả nghịch trong A, thì $P((x_{\lambda}))$ khả nghịch trong A và phần tử nghịch đảo $Q((x_{\lambda}))P((x_{\lambda}))^{-1}$ của $P((x_{\lambda}))Q((x_{\lambda}))^{-1}$ thuộc $B_1$. Do đó $B\subset B_1$. Mặt khác, nếu $P,Q\in K[(X_{\lambda})]$, và nếu $Q((x_{\lambda}))$ khả nghịch trong A, thì $P((x_{\lambda}))\in B$ và $Q((x_{\lambda}))\in B$, do đó $Q((x_{\lambda}))^{-1}\in B$ và $P((x_{\lambda}))Q((x_{\lambda}))^{-1}\in B$, do đó $B_1\subset B$.

### 6. Đặc trưng của một đại số giao hoán có đơn vị

#### Định nghĩa 4 {#ts-i-s1-def-4 .statement tag=025A}

Cho A là một đại số giao hoán có đơn vị trên K. Một đặc trưng có đơn vị là một cấu xạ có đơn vị của A vào K.

Khi điều này không thể gây ra nhầm lẫn, ta sẽ đơn giản gọi là đặc trưng thay cho đặc trưng có đơn vị. Tập hợp các đặc trưng có đơn vị của A được ký hiệu bởi $\mathsf{X}(A)$. Nếu A là đại số không, thì $\mathsf{X}(A)$ là rỗng.

Cho A và B là các đại số giao hoán có đơn vị trên K và $h$ là một cấu xạ có đơn vị của A vào B. Ánh xạ $\chi \mapsto \chi \circ h$ từ $\mathsf{X}(B)$ vào $\mathsf{X}(A)$ được ký hiệu bởi $\mathsf{X}(h)$. Nếu $k$ là một cấu xạ của B vào một đại số giao hoán có đơn vị, ta có $\mathsf{X}(k\circ h) =\mathsf{X}(h)\circ \mathsf{X}(k)$. Ánh xạ $\mathsf{X}$(Id$_A$) là ánh xạ đồng nhất của $\mathsf{X}(A)$.

Nếu $h$ là toàn ánh, $\mathsf{X}(h)$ là một song ánh từ $\mathsf{X}(B)$ lên tập hợp các đặc trưng của A triệt tiêu trên hạt nhân của $h$.

Cho $(A_1, e_1), . . . ,(A_n, e_n)$ là các đại số giao hoán có đơn vị trên K và cho A là đại số có đơn vị $A_1\times  \cdots  \times A_n$, với phần tử đơn vị $(e_1, . . . , e_n)$. Với mỗi $i$, đồng nhất $A_i$ với một iđêan của A và cho $\pi_i$ là ánh xạ chính tắc từ A lên $A_i$. Khi đó $\mathsf{X}(\pi_i)$ là một song ánh của $\mathsf{X}(A_i)$ lên tập hợp $\mathsf{X}_i$ gồm các đặc trưng của A triệt tiêu trên $\prod_{j\not=i}A_j$. Các tập hợp $\mathsf{X}_i$ rời nhau từng đôi một. Mặt khác, cho $\chi \in \mathsf{X}(A)$. Vì $1 =\sum\chi (e_i)$, tồn tại $i$ sao cho $\chi (e_i)\not= 0$. Với mọi $j\not=i$ và mọi $y\in A_j$, ta có $\chi (e_i)\chi (y) =\chi (e_iy) =\chi (0) = 0$, do đó $\chi (A_j) = 0$. Vậy, $\chi$ triệt tiêu trên $\prod_{j\not=i}A_j$, suy ra $\mathsf{X}(A)$ là hợp của các $\mathsf{X}_i$.

Cho B là đại số có đơn vị $A_1\otimes  \cdots  \otimes A_n$. Ký hiệu $h_i$ là cấu xạ chính tắc $A_i\rightarrow B$. Khi đó

$$
\chi \mapsto (\chi \circ h_1, . . . , \chi \circ h_n)
$$

là một ánh xạ từ $\mathsf{X}(B)$ vào $\mathsf{X}(A_1)\times  \cdots  \times \mathsf{X}(A_n)$, và

$$
(\chi_1, . . . , \chi_n)\mapsto \chi_1\otimes  \cdots  \otimes \chi_n
$$

là một ánh xạ từ $\mathsf{X}(A_1)\times  \cdots  \times \mathsf{X}(A_n)$ vào $\mathsf{X}(B)$. Ta kiểm tra được rằng các ánh xạ này là các song ánh ngược nhau, nhờ đó đồng nhất $\mathsf{X}(B)$ với $\mathsf{X}(A_1)\times  \cdots  \times \mathsf{X}(A_n)$.

Cho A là một đại số giao hoán có đơn vị trên K. Cho Y là tập hợp các iđêan có đối chiều 1 của A. Với mọi $\chi \in \mathsf{X}(A)$, ta có Ker($\chi$ )$\in Y$. Ánh xạ $\chi \mapsto$ Ker($\chi$ ) là một song ánh của $\mathsf{X}(A)$ lên Y. Thật vậy, nếu $I\in Y$, tồn tại một đẳng cấu duy nhất của đại số K có đơn vị $A/I$ lên K và cấu xạ hợp thành

$$
A\longrightarrow A/I\longrightarrow K
$$

là đặc trưng duy nhất của A có hạt nhân I.

#### Định nghĩa 5 {#ts-i-s1-def-5 .statement tag=025B}

Cho A là một đại số giao hoán có đơn vị trên K. Với mọi $x\in A$, ký hiệu $\mathscr{G}_A(x)$, hoặc đơn giản là $\mathscr{G}(x)$, là ánh xạ $\chi \mapsto$ $\chi (x)$ của $\mathsf{X}(A)$ vào K. Nó được gọi là biến đổi Gelfand của $x$.

Ánh xạ $\mathscr{G}$ là một cấu xạ có đơn vị của A vào đại số có đơn vị $K^{\mathsf{X}(A)}$ gồm các ánh xạ từ $\mathsf{X}(A)$ vào K. Nó được gọi là biến đổi Gelfand của A.

Nếu $x\in$ A, ảnh của biến đổi Gelfand $\mathscr{G}_A(x)$ của $x$ được chứa trong Sp$_A(x)$. Thật vậy, lấy $\chi \in \mathsf{X}(A)$; vì $\chi (x-\chi (x)e) =$ 0, phần tử $x-\chi (x)e$ không khả nghịch.

Cho B là một đại số giao hoán có đơn vị trên K và $h$ là một cấu xạ có đơn vị của A vào B; khi đó $\mathsf{X}(h) :\mathsf{X}(B)\rightarrow \mathsf{X}(A)$ xác định một cấu xạ có đơn vị $h_*: K^{\mathsf{X}(A)}\rightarrow K^{\mathsf{X}(B)}$, và biểu đồ:

$\mathscr{G}\leftarrow_A\mathsf{X}(A)$

A $\rightarrow K$ (3) $\rightarrow \leftarrow_h\rightarrow \leftarrow_{h_*}$

$\mathscr{G}\leftarrow_B\mathsf{X}(B)$

B $\rightarrow K$

là giao hoán. Thật vậy, với mọi $x\in A$ và mọi $\chi \in \mathsf{X}(B)$, ta có:

$$
\mathscr{G}_B(h(x))(\chi ) =\chi (h(x)) = (\chi \circ h)(x)
$$

$$
= (\mathsf{X}(h)(\chi ))(x)
$$

$$
=\mathscr{G}_A(x)(\mathsf{X}(h)(\chi )) \tag{4}
$$

$$
=h_*(\mathscr{G}_A(x))(\chi )
$$

Bây giờ giả sử K là một trường tôpô. Khi đó trang bị cho $\mathsf{X}(A)$ tôpô hội tụ đơn giản trên A (xem EVT, III, p. 14, Ví dụ 1), và không gian tôpô $\mathsf{X}(A)$ được gọi là không gian các đặc trưng của A. Do đó, tôpô của $\mathsf{X}(A)$ là tôpô ít mịn nhất sao cho các hàm $\mathscr{G}_A(x)$ với $x\in A$ liên tục, và ánh xạ $\chi \mapsto (\chi (a))_{a\in A}$ đồng nhất không gian $\mathsf{X}(A)$ với một tập con của $K^A$.

Khi K = $\mathbf{R}$ hoặc $\mathbf{C}$, tôpô này là tôpô cảm sinh trên $\mathsf{X}(A)\subset A^*$ bởi tôpô yếu $\sigma (A^*,A)$ trên $A^*$ (EVT, II, p. 45, Định. 2); về phương diện này, ta cũng sẽ gọi nó là tôpô yếu trên $\mathsf{X}(A)$.

Nếu $h$ là một cấu xạ có đơn vị của A vào B, ánh xạ $\mathsf{X}(h) :\mathsf{X}(B)\rightarrow \mathsf{X}(A)$ là liên tục. Nếu $h$ là toàn ánh, ảnh của $\mathsf{X}(h)$, tức tập hợp các đặc trưng của A triệt tiêu trên hạt nhân của $h$, là đóng trong $\mathsf{X}(A)$; mặt khác, tôpô trên $\mathsf{X}(h)(\mathsf{X}(B))$ suy ra từ tôpô của $\mathsf{X}(B)$ qua song ánh $\mathsf{X}(h)$ là tôpô hội tụ đơn giản trong A, nghĩa là tôpô cảm sinh bởi tôpô của $\mathsf{X}(A)$; nói cách khác, $\mathsf{X}(h)$ là một đồng phôi của $\mathsf{X}(B)$ lên một tập con đóng của $\mathsf{X}(A)$.

Nếu $A_1, . . . ,A_n$ là các đại số giao hoán có đơn vị trên K, không gian $\mathsf{X}(A_1\times  \cdots  \times A_n)$ do đó được đồng nhất với tổng tôpô của $\mathsf{X}(A_1), . . . ,\mathsf{X}(A_n)$. Tương tự, $\mathsf{X}(A_1\otimes  \cdots  \otimes A_n)$ được đồng nhất với tích tôpô $\mathsf{X}(A_1)\times  \cdots  \times \mathsf{X}(A_n)$.

### 7. Trường hợp các đại số không có phần tử đơn vị

#### Định nghĩa 6 {#ts-i-s1-def-6 .statement tag=025C}

Cho A là một đại số giao hoán trên K. Một đặc trưng của A, theo định nghĩa, là một cấu xạ đại số của A vào K.

Tập hợp các đặc trưng của A sẽ được ký hiệu là $\mathsf{X}'(A)$.

Ánh xạ không là một cấu xạ đại số. Nếu A có một phần tử đơn vị $e$, một cấu xạ đại số khác không của A vào K là có đơn vị, tức là, là một đặc trưng có đơn vị của K theo nghĩa của Định nghĩa 4: thật vậy, để $\chi \in \mathsf{X}'(A)$ khác không, điều kiện cần và đủ là $\chi (e) = 1$.

Ta đặt $\mathsf{X}(A) =\mathsf{X}'(A)-\{0\}$; theo điều trên, ký hiệu này tương thích với ký hiệu đã đưa vào khi A có đơn vị.

Nếu $h: A\rightarrow B$ là một cấu xạ của các đại số giao hoán, ánh xạ $\chi \mapsto \chi \circ h$ là một ánh xạ $\mathsf{X}'(h) :\mathsf{X}'(B)\rightarrow \mathsf{X}'(A)$. Nó biến 0 thành 0. Nếu $k: B\rightarrow C$ là một cấu xạ của các đại số giao hoán, thì ta có $\mathsf{X}'(k\circ h) =\mathsf{X}'(h)\circ \mathsf{X}'(k)$. Nếu $h$ là toàn ánh, $\mathsf{X}'(h)$ là một song ánh của $\mathsf{X}'(B)$ lên tập hợp các đặc trưng của A triệt tiêu trên hạt nhân của $h$. Cho $A_1, . . . ,A_n$ là các đại số giao hoán, $A = A_1\times  \cdots  \times A_n$ và $\pi : A\rightarrow A_i$ là cấu xạ chính tắc; khi đó $\mathsf{X}'(\pi_i)$ là một song ánh của $\mathsf{X}'(A_i)$ lên một tập con $\mathsf{X}'_i$ của $\mathsf{X}'(A)$, tức là tập hợp các đặc trưng của A triệt tiêu trên $\prod_{j\not=i}A_j$; ta thấy như trong No.$^o6$ rằng $\mathsf{X}'(A)$ là hợp

của các $\mathsf{X}'_i$; mặt khác, $\mathsf{X}'_i\cap \mathsf{X}'_j=\{0\}$ với $i\not=j$; đặc biệt các $\mathsf{X}'_i-\{0\}$ tạo thành một phân hoạch của $\mathsf{X}'(A)-\{0\}=\mathsf{X}(A)$.

Với mọi $x\in A$, đặt $\mathscr{G}'_A(x)$, hoặc đơn giản là $\mathscr{G}'(x)$, là ánh xạ $\chi \mapsto \chi (x)$ của $\mathsf{X}'(A)$ vào K. Ánh xạ $\mathscr{G}'$ là một cấu xạ của A vào đại số $A_1$ của các ánh xạ $\mathsf{X}'(A)\rightarrow K$ triệt tiêu tại 0. Cho B là một đại số giao hoán, $B_1$ là đại số của các ánh xạ $\mathsf{X}'(B)\rightarrow$ K triệt tiêu tại 0, và $h$ là một cấu xạ của A vào B; khi đó $\mathsf{X}'(h)$ xác định một cấu xạ $h_1: A_1\rightarrow B_1$, và ta có $h_1\circ \mathscr{G}'_A=\mathscr{G}'_B\circ h$. Người ta ký hiệu bởi $\mathscr{G}_A(x)$, hoặc đơn giản là $\mathscr{G}(x)$, hạn chế của $\mathscr{G}'_A(x)$ lên $\mathsf{X}(A)$, và gọi nó là biến đổi Gelfand của $x$.

Cho $\widetilde{A}$ là đại số có đơn vị được suy ra từ A bằng phép nối một phần tử đơn vị. Bằng hạn chế, mọi đặc trưng của $\widetilde{A}$ xác định một đặc trưng của A; ngược lại, mọi đặc trưng của A mở rộng theo một cách duy nhất thành một đặc trưng của $\widetilde{A}$. Điều này xác định một song ánh chính tắc của $\mathsf{X}'(A)$ lên $\mathsf{X}(\widetilde{A})$, nhờ đó hai tập hợp này được đồng nhất. Đặc trưng 0 của A được đồng nhất với đặc trưng duy nhất của $\widetilde{A}$ có hạt nhân là A.

Nếu $x\in A$ và $\chi \in \mathsf{X}'(A)$, ta có $\chi (x)\in$ Sp$_{\widetilde{A}}(x)$, do đó $\chi (x)\in$ Sp$'_A(x)$.

#### Bổ đề 3 {#ts-i-s1-lem-3 .statement tag=025D}

Ánh xạ $\chi \mapsto$ Ker($\chi$ ) là một song ánh của $\mathsf{X}(A)$ lên tập hợp các iđêan chính quy có đối chiều 1 của A.

Ta nhắc lại (A, VIII, p. 426, Định nghĩa 1) rằng một iđêan I của A được gọi là chính quy nếu đại số thương $A/I$ nhận một phần tử đơn vị.

Hãy chứng minh bổ đề. Một mặt, $\mathsf{X}(A)$ được đồng nhất với tập hợp các ký tự của $\widetilde{A}$ không bằng không trên A. Mặt khác, theo A, VIII, p. 428, Mệnh đề 4, ánh xạ $I\mapsto A\cap I$ là một song ánh từ tập hợp các iđêan cực đại của $\widetilde{A}$ phân biệt với A lên tập hợp các iđêan cực đại chính quy của A. Bổ đề được suy ra từ các kết quả của No. 6.

Bây giờ giả sử rằng K là một trường tôpô. Khi đó ta trang bị $\mathsf{X}'(A)$ tôpô hội tụ đơn giản trên A; ký hiệu $\mathsf{X}'(A)$ từ nay sẽ chỉ không gian tôpô thu được như vậy. Khi $K =\mathbf{R}$ hoặc $\mathbf{C}$, ta cũng gọi nó là tôpô yếu. Với mọi $x\in A$, hàm $\mathscr{G}'_A(x)$ trên $\mathsf{X}'(A)$ là liên tục.

Nếu $h$ là một cấu xạ từ A vào B, ánh xạ $\mathsf{X}'(h) :\mathsf{X}'(B)\rightarrow$ $\mathsf{X}'(A)$ là liên tục. Nếu $h$ là toàn ánh, $\mathsf{X}'(h)$ là một đồng phôi của $\mathsf{X}'(B)$ lên ảnh của nó, và ảnh này là đóng trong $\mathsf{X}'(A)$.

Cho $A = A_1\times  \cdots  \times A_n$; với cùng ký hiệu như trên, $\mathsf{X}'(\pi_i)$ là một đồng phôi của $\mathsf{X}'(A_i)$ lên $\mathsf{X}'_i$ và $\mathsf{X}'_i$ là đóng trong $\mathsf{X}'(A)$. Do đó $\mathsf{X}'_i-\{0\}$ là mở trong $\mathsf{X}'(A)$; các $\mathsf{X}'(\pi_i)$ xác định một ánh xạ liên tục từ không gian tổng S của các $\mathsf{X}'(A_i)$ lên $\mathsf{X}'(A)$, và người ta kiểm tra ngay lập tức rằng hợp của các lân cận của các điểm $0\in \mathsf{X}'(A_1), . . . ,0\in \mathsf{X}'(A_n)$ có ảnh là một lân cận của $0\in \mathsf{X}'(A)$; từ tất cả những điều này suy ra rằng $\mathsf{X}'(A)$ được đồng nhất một cách chính tắc với một không gian thương của S. Đặc biệt, không gian $\mathsf{X}(A)$ được đồng nhất với không gian tổng của các $\mathsf{X}(A_i)$.

Song ánh chính tắc của $\mathsf{X}'(A)$ lên $\mathsf{X}(\widetilde{A})$ là một đồng phôi. Cho B là một đại số có đơn vị trên K và $B'$ là đại số nền; khi đó không gian $\mathsf{X}(B)$ được đồng nhất với không gian con $\mathsf{X}(B')$ của $\mathsf{X}'(B')$.

### 8. Các iđêan nguyên thủy

Cho A là một đại số trên K và E là một không gian vectơ trên K. Một biểu diễn của A trong E là một cấu xạ từ A vào đại số $\mathscr{L}(E)$ của các tự cấu xạ của E. Một biểu diễn đơn ánh được gọi là trung thành. Cho $\pi_1$ và $\pi_2$ là các biểu diễn của A trong các không gian $E_1,E_2$. Một cấu xạ từ $\pi_1$ vào $\pi_2$ là một ánh xạ K-tuyến tính $u: E_1\rightarrow E_2$ sao cho $u(\pi_1(a)x) =\pi_2(a)u(x)$ với mọi $a\in A$ và $x\in E_1$. Các biểu diễn được gọi là tương đương nếu tồn tại một cấu xạ từ $\pi_1$ vào $\pi_2$ là một đẳng cấu của các không gian vectơ. Khi đó nghịch đảo của nó là một cấu xạ từ $\pi_2$ vào $\pi_1$. Một biểu diễn $\pi$ của A trong E được gọi là bất khả quy nếu $E\not=\{0\}$ và nếu các không gian con vectơ duy nhất của E ổn định dưới $\pi (A)$ là $\{0\}$ và E.

#### Ví dụ {#ts-i-s1-n8-exa-1 .statement tag=025E}

Ánh xạ không từ A vào $\mathscr{L}(E)$ là một biểu diễn, gọi là tầm thường, của A. Nó là bất khả quy khi và chỉ khi E có chiều 1.

#### Bổ đề 4 {#ts-i-s1-lem-4 .statement tag=025F}

Cho $\pi$ là một biểu diễn bất khả quy không tầm thường của A trong E. Với mọi phần tử khác không $\xi$ của E, ta có $\pi (A)\xi = E$.

Không gian con $\pi (A)\xi$ của E là ổn định dưới $\pi (A)$. Giả sử nó bằng không. Khi đó không gian con khác không $K\xi$ của E sẽ ổn định dưới $\pi (A)$, và do đó bằng E; nhưng điều này sẽ suy ra rằng $\pi$ là biểu diễn không. Vậy ta có $\pi (A)\xi = E$.

Cho $\pi$ là một biểu diễn bất khả quy không tầm thường của A trong E. Theo bổ đề này, linh hóa tử R của $\xi$ trong A là một iđêan trái chính quy (A, VIII, p. 425, No.$^o1$) của A, và biểu diễn $\pi$ tương đương với biểu diễn được xác định bởi giả môđun A $A/R$. Vì $\pi$ là bất khả quy, iđêan R là một iđêan trái cực đại chính quy.

#### Định nghĩa 7 {#ts-i-s1-def-7 .statement tag=025G}

Cho A là một đại số trên K. Một iđêan nguyên thủy của A được định nghĩa là hạt nhân của một biểu diễn bất khả quy không tầm thường của A.

Nếu A giao hoán, các iđêan nguyên thủy của A là các iđêan cực đại chính quy của A. Thật vậy, các biểu diễn bất khả quy không tầm thường của A, sai khác một tương đương, là các biểu diễn $\pi_R$ được xác định bởi các giả môđun A $A/R$, trong đó R là một iđêan cực đại chính quy của A. Hạt nhân của $\pi_R$ chứa R. Nó thậm chí bằng R vì theo A, VIII, p. 426, Mệnh đề 2, tính giao hoán của A suy ra rằng $A/R$ là một trường. Do đó Ker($\pi_R$) là cực đại chính quy.

#### Bổ đề 5 {#ts-i-s1-lem-5 .statement tag=025H}

Cho $\pi$ là một biểu diễn bất khả quy của A trong một không gian vectơ E trên K.

a) Cho I là một iđêan hai phía của A. Nếu $\pi (I)\not=\{0\}$, thì $\pi |I$ là bất khả quy;

b) Cho $I_1$ và $I_2$ là hai iđêan hai phía của A sao cho $\pi (I_1)\not= 0$ và $\pi (I_2)\not= 0$. Khi đó $\pi (I_1I_2)\not= 0$.

Tập hợp các phần tử của E bị triệt tiêu bởi $\pi (I)$ là ổn định dưới $\pi (A)$ và phân biệt với E, do đó bằng 0. Vì vậy, nếu $\xi$ là một phần tử khác không của E, thì $\pi (I)\xi \not= 0$; vì $\pi (I)\xi$ ổn định dưới $\pi (A)$, nên $\pi (I)\xi = E$, điều này chứng minh a). Mặt khác, điều vừa chứng minh suy ra rằng $\pi (I_2)E = E$, $\pi (I_1)\pi (I_2)E = E$, do đó $\pi (I_1I_2)\not= 0$, do đó b).

#### Bổ đề 6 {#ts-i-s1-lem-6 .statement tag=025I}

Cho $I_1$ và $I_2$ là hai iđêan hai phía của A, I là một iđêan nguyên thủy của A. Nếu I chứa $I_1I_2($đặc biệt, nếu I chứa $I_1\cap I_2)$, thì I chứa $I_1$ hoặc $I_2$.

Cho $\pi$ là một biểu diễn bất khả quy có hạt nhân I. Nếu $I\not\supset I_1$ và $I\not\supset I_2$, Bổ đề 5, b) chứng minh rằng $\pi (I_1I_2)\not= 0$, do đó $I\not\supset I_1I_2$.

#### Bổ đề 7 {#ts-i-s1-lem-7 .statement tag=025J}

Giả sử A có một phần tử đơn vị. Cho I là một iđêan hai phía tối đại của A. Khi đó I là một iđêan nguyên thủy.

Có một iđêan trái cực đại R của A chứa I (A, I, p. 99, Định lý 1). Cho $\pi$ là biểu diễn chính tắc của A trong $A/R$, biểu diễn này bất khả quy và khác không. Vì IA $\subset R$, hạt nhân $I'$ của $\pi$ chứa I, do đó $I'= I$ và I là nguyên thủy.

Cho J(A) là tập hợp các iđêan nguyên thủy của A. Với mọi tập con M của A, ta ký hiệu V(M) là tập hợp các iđêan nguyên thủy của A chứa M; nếu I là iđêan hai phía của A sinh bởi M, thì ta có V(M) = V(I). Nếu M chỉ gồm một phần tử $x$, ta viết $V(x)$ thay cho $V(\{x\})$. Ánh xạ $M\mapsto V(M)$ là giảm đối với các quan hệ bao hàm. Ta có :

$$
V(\emptyset ) = J(A),V(A) =\emptyset \tag{5}
$$

$$
V(\bigcup_{i\in I}M_i)= V(\sum_{i\in I}M_i)=\bigcap_{i\in I}V(M_i) \tag{6}
$$

với mọi họ $(M_i)_{i\in I}$ các tập con của A. Mặt khác, theo bổ đề 6,

$$
V(I_1\cap I_2) = V(I_1I_2) = V(I_1)\cup V(I_2) \tag{7}
$$

với mọi iđêan hai phía $I_1,I_2$ của A. Các công thức (5) đến (7) chỉ ra rằng các tập con V(M) của J(A) là các tập đóng của một tôpô được gọi là tôpô Jacobson trên J(A).

Cho T là một tập con của J(A), và gọi Υ(T) là giao của các phần tử của T, sao cho Υ(T) là một iđêan hai phía của A. Khi đó bao đóng của T trong J(A) là tập con đóng nhỏ nhất của J(A) chứa T, nghĩa là V(Υ(T)). Đặc biệt, T là đóng khi và chỉ khi T = V(Υ(T)).

#### Mệnh đề 2 {#ts-i-s1-prop-2 .statement tag=025K}

Cho $I_1$ và $I_2$ là các điểm phân biệt của J(A). Khi đó một trong hai điểm này không kề với điểm kia.

Chẳng hạn, ta có $I_1\not\subset I_2$. Tập $V(I_1)$ gồm các $I\in J(A)$ sao cho $I_1\subset I$ là đóng trong J(A), và nó chứa $I_1$ nhưng không chứa $I_2$.

#### Mệnh đề 3 {#ts-i-s1-prop-3 .statement tag=025L}

Cho $I\in J(A)$. Để $\{I\}$ là đóng trong J(A), điều kiện cần và đủ là I là một iđêan nguyên thủy cực đại.

Thật vậy, bao đóng của $\{I\}$ gồm các iđêan nguyên thủy của A chứa I.

Quan hệ

“ $\pi_1,\pi_2$ là các biểu diễn của A đẳng cấu với nhau ”

là một quan hệ tương đương đối với $\pi_1$ và $\pi_2$. Với mỗi biểu diễn $\pi$ của A, ta ký hiệu bởi cl($\pi$ ) lớp tương đương của $\pi$, do đó đây là một biểu diễn của A đẳng cấu với $\pi$, sao cho hai biểu diễn $\pi_1$ và $\pi_2$ đẳng cấu với nhau khi và chỉ khi cl($\pi_1$) $=$ cl($\pi_2$). Ta nói rằng cl($\pi$ ) là lớp của $\pi$.

Gọi $\mathfrak{c}$ là lực lượng của A. Cho $\pi$ là một biểu diễn bất khả quy khác không của A trong một không gian vectơ trên K E. Gọi $\xi$ là một phần tử khác không của E. Vì $\pi (A)\xi = E$ (bổ đề 4), chiều của E là $\leqslant \mathfrak{c}$ (A, II, p. 97, hệ quả). Quan hệ

“ $\lambda$ là một lớp các biểu diễn bất khả quy của A

trong một không gian vectơ trên K có chiều $\leqslant \mathfrak{c}$ ”

là xác định tập theo $\lambda$ (E, II, p. 3). Thật vậy, mọi không gian vectơ có chiều $\leqslant \mathfrak{c}$ đều đẳng cấu với một không gian $K^B$ trong đó B là một tập con của A (A, II, p. 25, déf. 10), và khi đó mệnh đề suy ra từ E, II, p. 47.

Ta ký hiệu bởi $\widehat{A}$ tập hợp các lớp của các biểu diễn bất khả quy, không tầm thường, của A. Từ những điều trên, với mỗi biểu diễn bất khả quy không tầm thường $\pi$ của A, tồn tại một biểu diễn duy nhất $\widehat{\pi}\in \widehat{A}$ đẳng cấu với $\pi$.

Ánh xạ từ $\widehat{A}$ vào J(A) gán cho $\pi$ hạt nhân của nó là toàn ánh. Nếu A giao hoán, từ sự kiện rằng các iđêan nguyên thủy là các iđêan chính quy cực đại, suy ra rằng ánh xạ này là một song ánh.

Ta trang bị cho $\widehat{A}$ tôpô ảnh ngược của tôpô của J(A) bởi ánh xạ $\widehat{A}\rightarrow J(A)$.

#### Mệnh đề 4 {#ts-i-s1-prop-4 .statement tag=025M}

Nếu A có một phần tử đơn vị, các không gian J(A) và $\widehat{A}$ là quasi-compact.

Chỉ cần đưa ra chứng minh cho $J(A)$. Gọi $(T_j)$ là một họ các tập con đóng của $J(A)$ có giao là rỗng. Nếu tổng $\sum_j\Upsilon (T_j)$ không bằng A, thì tổng này sẽ được chứa trong một iđêan hai phía tối đại I. Iđêan I sẽ là nguyên thủy (Bổ đề 7); vì tập con $T_j$ là đóng, do đó bằng $V(\Upsilon (T_j))$, nên ta có $I\in T_j$ với mọi $j$, điều này mâu thuẫn với giả thiết. Vậy ta có $\sum_j\Upsilon (T_j) = A$, và do đó có thể viết $1 =x_1+\cdots +x_n$ với $n\geqslant 1$ và $x_i\in \Upsilon (T_{j_i})$ với mọi $i$. Điều này suy ra $\Upsilon (T_{j_1})+\cdots +\Upsilon (T_{j_n}) = A$, do đó $T_{j_1}\cap  \cdots  \cap T_{j_n}=\emptyset$.

Giả sử đại số A là giao hoán và có đơn vị. Tôpô Jacobson trên $J(A)$ là tôpô cảm sinh trên $J(A)$ bởi tôpô Zariski của phổ nguyên tố của A (AC, II, Định nghĩa 4, p. 125).

Giả sử A là giao hoán và K là một trường tôpô. Đẳng cấu chính tắc của K lên $\mathscr{L}(K)$ cho phép đồng nhất một phần tử của $\mathsf{X}(A)$ với một biểu diễn của A trong không gian vectơ K, biểu diễn này xác định một ánh xạ đơn ánh từ $\mathsf{X}(A)$ vào $\widehat{A}$. Do đó có thể đồng nhất $\mathsf{X}(A)$ với một tập con của $\widehat{A}$.

#### Mệnh đề 5 {#ts-i-s1-prop-5 .statement tag=025N}

Tôpô cảm sinh trên $\mathsf{X}(A)$ bởi tôpô của $\widehat{A}$ là thô hơn tôpô của $\mathsf{X}(A)$.

Thật vậy, cho T là một tập con đóng của $\widehat{A}$. Khi đó T là tập hợp các $\pi \in \widehat{A}$ mà hạt nhân chứa một tập con M của A. Do đó $T\cap \mathsf{X}(A)$ là tập hợp các $\chi \in \mathsf{X}(A)$ triệt tiêu trên M, nghĩa là một tập con đóng của $\mathsf{X}(A)$. Suy ra mệnh đề.

Nói chung, tôpô của $\mathsf{X}(A)$ không trùng với tôpô cảm sinh bởi tôpô của $\widehat{A}($cf. I, p. 193, Bài tập 6, c)).

## BÀI TẬP {#ts-i-s1-exercises}

Xem các [bài tập cho § 1](exercises/s1/).
