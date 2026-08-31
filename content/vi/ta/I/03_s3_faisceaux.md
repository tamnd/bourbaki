---
book: ta
book_title: Topologie algébrique
chapter: I
chapter_title: REVÊTEMENTS
section: 3
section_title: Faisceaux
lang: vi
source: ta-i-iv-fr
book_pages: TA I.42-TA I.67, TA I.141-TA I.145
pdf_pages: 0058-0083, 0157-0161
extraction: native
subsections:
    - "no": 1
      title: Faisceaux d’ensembles
      page: 42
      pdf_page: 58
    - "no": 2
      title: Sous-faisceaux d’un faisceau
      page: 44
      pdf_page: 60
    - "no": 3
      title: Exemples de faisceaux
      page: 44
      pdf_page: 60
    - "no": 4
      title: Morphismes de préfaisceaux
      page: 47
      pdf_page: 63
    - "no": 5
      title: Espace étalé associé à un préfaisceau
      page: 49
      pdf_page: 65
    - "no": 6
      title: Faisceau associé à un préfaisceau
      page: 53
      pdf_page: 69
    - "no": 7
      title: Image directe et image réciproque d’un faisceau
      page: 57
      pdf_page: 73
    - "no": 8
      title: Les homomorphismes $\alpha \mathbf{e}\mathbf{t}\beta$ ; adjonction
      page: 59
      pdf_page: 75
    - "no": 9
      title: Faisceaux mous
      page: 64
      pdf_page: 80
    - "no": 10
      title: Faisceaux de structures
      page: 66
      pdf_page: 82
statements: 35
exercises: 8
content_sha256: e60e10de49b1f7fa62fc2beb2343655ec846e54e18de85f7f28ad2aa9695b426
translated_from: content/en-mt/ta/I/03_s3_faisceaux.md
source_lang: en-mt
translation_method: machine
source_content_sha256: 52992bda508a3c0caa17b47af125817ccd2a2bd8f51eb6448ce1d4cae22b17ce
translation_model: gpt-5-6-mini, gpt-5-6
translation_run: translate-vi-f7047471
glossary_version: 34
glossary_terms_sha256: 3d252cd4cb381d03b8fc1cbc512c2c7f3bc816b1cc90a5be8759ac94ab48c2ed
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 3. BÓ

### 1. Các bó của tập hợp

Cho B là một không gian tôpô.

#### Định nghĩa 1 {#ta-i-s3-def-1 .statement tag=01NS}

Một tiền bó trên B, đối với một cơ sở $\mathscr{B}$ của tôpô của B, là một hệ xạ ảnh của các tập hợp, đối với tập hợp các chỉ số $\mathscr{B}$ có thứ tự bởi quan hệ bao hàm.

Nói cách khác (E, III, p. 52), một tiền bó $\mathscr{F}$ trên B đối với $\mathscr{B}$ là một cặp $((\mathscr{F}(U))_{U\in\mathscr{B}},(f_{UV}))$, cũng được ký hiệu là $(\mathscr{F}(U), f_{UV})$, trong đó $((\mathscr{F}(U))_{U\in\mathscr{B}}$ là một họ các tập hợp có $\mathscr{B}$ làm tập hợp các chỉ số và trong đó với mỗi cặp $(U,V)$ của các phần tử của $\mathscr{B}$ sao cho $U\subset V,f_{UV}$ là một ánh xạ từ $\mathscr{F}(V)$ vào $\mathscr{F}(U)$, các ánh xạ này thỏa mãn các điều kiện sau:

(PF$_1$) Các quan hệ $U\subset V\subset W$ suy ra $f_{UW}=f_{UV}\circ f_{VW}$;

(PF$_2$) Với mọi tập mở U $\in \mathscr{B},f_{UU}$ là ánh xạ đồng nhất của

$$
\mathscr{F}(U)
$$

Một tiền bó trên B đối với tập hợp các tập con mở của B đơn giản được gọi là một tiền bó trên B.

Cho $\mathscr{F}= (\mathscr{F}(U), f_{UV})$ là một tiền bó trên B, đối với một cơ sở $\mathscr{B}$ của tôpô của B. Cho U là một phần tử của cơ sở $\mathscr{B}$. Các phần tử của $\mathscr{F}(U)$ được gọi là các thiết diện của $\mathscr{F}$ trên U. Nếu V là một phần tử của cơ sở $\mathscr{B}$ chứa U và $s$ là một phần tử của $\mathscr{F}(V)$, phần tử $f_{UV}(s)$ của $\mathscr{F}(U)$ được gọi là hạn chế của $s$ lên U. Nếu không có nguy cơ nhầm lẫn về các ánh xạ $f_{UV}$, hạn chế của $s$ lên U sẽ được ký hiệu là $s|U$.

Cho $B'$ là một tập con mở của B và $\mathscr{B}'$ là một cơ sở của tôpô của $B'$ sao cho $\mathscr{B}'\subset \mathscr{B}$. Tiền bó trên $B'$, đối với $\mathscr{B}'$, suy ra từ $\mathscr{F}$ bằng hạn chế, được gọi là hạn chế của $\mathscr{F}$ lên $\mathscr{B}'$ và được ký hiệu bởi $\mathscr{F}|\mathscr{B}'$, hệ xạ ảnh $((\mathscr{F}(U))_{U\in\mathscr{B}'},(f_{UV}))$ suy ra từ $\mathscr{F}$ bằng cách hạn chế về $\mathscr{B}'$ của tập hợp các chỉ số (loc. cit.). Khi $\mathscr{F}$ là một tiền bó trên B và $\mathscr{B}'$ là tập hợp các tập mở của $B'$, tiền bó $\mathscr{F}|\mathscr{B}'$ cũng được ký hiệu bởi $\mathscr{F}|B'$ và được gọi là tiền bó suy ra từ $\mathscr{F}$ bằng hạn chế lên $B'$.

#### Định nghĩa 2 {#ta-i-s3-def-2 .statement tag=01NT}

Cho $\mathscr{F}= (\mathscr{F}(U), f_{UV})$ là một tiền bó trên B. Ta nói rằng $\mathscr{F}$ là một bó trên B nếu, với mọi tập con mở U của B và mọi họ $(U_i)_{i\in I}$ các tập con mở của B, có hợp U, các tính chất sau được thỏa mãn:

$(F_1)$ Ánh xạ $(f_{U_iU})_{i\in I}:\mathscr{F}(U)\rightarrow \prod_{i\in I}\mathscr{F}(U_i)$ là đơn ánh ;

$(F_2)$ Đối với mọi họ $(s_i)\in \prod_{i\in I}\mathscr{F}(U_i)$ sao cho $f_{(U_i\cap U_j)U_i}(s_i) =$

$f_{(U_i\cap U_j)U_j}(s_j)$ với mọi cặp $(i, j)\in I\times I$, tồn tại một phần tử $s$

của $\mathscr{F}(U)$ sao cho với mọi $i\in I$, ta có $f_{U_iU}(s) =s_i$.

#### Nhận xét {#ta-i-s3-n1-rem-1 .statement tag=01NU}

Cho $\mathscr{F}$ là một tiền bó trên B. Với mọi tập mở U của B, $f_{\emptyset U}$ là một ánh xạ của $\mathscr{F}(U)$ vào $\mathscr{F}(\emptyset )$, do đó $\mathscr{F}(\emptyset )$ không rỗng ngay khi tồn tại một tập mở U sao cho $\mathscr{F}(U)$ không rỗng. Nếu $\mathscr{F}$ là một bó, $\mathscr{F}(\emptyset )$ là một tập hợp một phần tử; điều này được thấy bằng cách áp dụng $(F_1)$ và $(F_2)$ vào phủ của tập rỗng bởi họ rỗng ($I =\emptyset$ ).

Cho $\mathscr{F}$ là một bó trên B và cho $B'$ là một tập con mở của B; tiền bó $\mathscr{F}|B'$ suy ra từ $\mathscr{F}$ bằng cách hạn chế vào $B'$ là một bó, được gọi là bó suy ra từ $\mathscr{F}$ bằng cách hạn chế vào $B'$.

### 2. Các tiền bó con của một bó

Cho B là một không gian tôpô. Cho $\mathscr{F}= (\mathscr{F}(U), f_{UV})$ là một tiền bó trên B, tương ứng với một cơ sở $\mathscr{B}$ của tôpô của B.

Giả sử đã cho, với mỗi tập mở $U\in \mathscr{B}$, một tập con $\mathscr{L}(U)$ của $\mathscr{F}(U)$. Nếu có $f_{UV}(\mathscr{L}(V))\subset \mathscr{L}(U)$ với mọi cặp $(U,V)$ của các phần tử của $\mathscr{B}$ sao cho $U\subset V$, cặp $\mathscr{L}= ((\mathscr{L}(U))_{U\in\mathscr{B}},(f'_{UV}))$, trong đó $f'_{UV}:\mathscr{L}(V)\rightarrow \mathscr{L}(U)$ là ánh xạ suy ra từ $f_{UV}$, là một tiền bó. Một tiền bó như vậy được gọi là một tiền bó con của $\mathscr{F}$. Vì các ánh xạ $f'_{UV}$ được xác định bởi tiền bó đã cho $\mathscr{F}$ và họ $(\mathscr{L}(U))_{U\in\mathscr{B}}$, người ta cũng nói, do lạm dụng ngôn ngữ, rằng họ $(\mathscr{L}(U))_{U\in\mathscr{B}}$ là một tiền bó con của $\mathscr{F}$.

Giả sử bây giờ rằng $\mathscr{F}$ là một bó trên B và với mỗi tập con mở U của B,$\mathscr{L}(U)$, một tập con của $\mathscr{F}(U)$. Để $(\mathscr{L}(U))_{U\in\mathscr{B}}$ là một tiền bó con của $\mathscr{F}$, và để tiền bó này là một bó, điều kiện cần và đủ là điều kiện sau đây được thỏa mãn:

(F) Cho $(U_i)_{i\in I}$ là một họ các tập mở của B, U là hợp của nó, và $s$ là một

phần tử của $\mathscr{F}(U)$. Để $s$ thuộc $\mathscr{L}(U)$, điều kiện cần và

đủ là với mọi $i$ trong I,$f_{U_iU}(s)$ thuộc $\mathscr{L}(U_i)$.

Thật vậy, nếu điều kiện (F) được thỏa mãn, ta có $f_{UV}(\mathscr{L}(V))\subset \mathscr{L}(U)$ với mọi cặp $(U,V)$ các tập mở của B sao cho $U\subset V$ và các tính chất $(F_1)$ và $(F_2)$ đối với tiền bó con $(\mathscr{L}(U))$ suy ra từ các tính chất tương tự đối với bó $\mathscr{F}$. Điều đảo lại là ngay lập tức.

Khi điều kiện (F) được thỏa mãn, người ta nói rằng $(\mathscr{L}(U))$ là một bó con của bó $\mathscr{F}$.

### 3. Ví dụ về các bó

Cho B là một không gian tôpô.

1) Các bó các ánh xạ

Cho X là một tập hợp. Với mỗi tập mở U của B, ký hiệu $\mathscr{F}(U; X)$ là tập hợp các ánh xạ từ U vào X (E, II, p. 31). Với mỗi cặp $(U,V)$ các tập mở của B sao cho $U\subset V$, cho $r_{UV}:\mathscr{F}(V; X)\rightarrow$ $\mathscr{F}(U; X)$ là ánh xạ hạn chế $f\mapsto f|U$. Rõ ràng rằng cặp $(\mathscr{F}(U; X), r_{UV})$ là một bó trên B. Nó được gọi là bó trên B các ánh xạ có giá trị trong X, và được ký hiệu bởi $\mathscr{F}(B; X)$.

2) Các bó các ánh xạ liên tục

Cho X là một không gian tôpô. Với mỗi tập mở U của B, cho $\mathscr{C}(U; X)$ là tập hợp các ánh xạ liên tục từ U vào X. Khi đó, $(\mathscr{C}(U; X))$ là một bó con của bó $\mathscr{F}(B; X)$ theo mệnh đề 4 của TG, I, p. 19. Bó thu được như vậy được ký hiệu bởi $\mathscr{C}(B; X)$ và được gọi là bó trên B các ánh xạ liên tục có giá trị trong X. Trong trường hợp riêng khi X được trang bị tôpô rời rạc, bó $\mathscr{C}(B; X)$ nhận tên là bó trên B các ánh xạ hằng địa phương có giá trị trong X.

3) Các bó các thiết diện liên tục

Cho E là một không gian tôpô và cho $p: E\rightarrow B$ là một ánh xạ liên tục. Với mỗi tập mở U của B, ký hiệu bởi $\mathscr{S}(U;p)$ (hoặc $\mathscr{S}(U; E)$ khi không thể có sự nhầm lẫn) tập hợp các thiết diện liên tục của $p$ trên U. Họ $(\mathscr{S}(U;p))$ là một bó con của bó $\mathscr{C}(B; E)$. Bó thu được như vậy được ký hiệu bởi $\mathscr{S}(B; E)$ hoặc đơn giản là $\mathscr{S}(E)$ và được gọi là bó trên B các thiết diện liên tục của không gian B $(E, p)$. Ta sẽ thấy trong no$^o6$ dưới đây rằng mọi bó trên B đều đẳng cấu với bó trên B các thiết diện liên tục của một không gian B étalé.

4) Các bó các cấu xạ B

Cho $(E, p)$ và $(E', p')$ là các không gian B. Với mỗi tập mở U của E, ký hiệu bởi $\mathscr{C}_B(U; E')$ tập hợp các cấu xạ B từ $(U, p|U)$ vào $(E', p')$. Họ $(\mathscr{C}_B(U; E'))$ là một bó con của bó $\mathscr{C}(E; E')$. Bó thu được như vậy được ký hiệu bởi $\mathscr{C}_B(E; E')$ và được gọi là bó trên E các cấu xạ B có giá trị trong $(E', p')$. Khi $(E, p)$ bằng $(B$, Id$_B)$, bó này là bó $\mathscr{S}(B; E)$ của ví dụ 3.

Với mỗi tập mở U của B, cho $\mathscr{M}(U)$ là tập hợp các cấu xạ U

từ $\overset{-1}{p}(U)$ vào $(^-{p'}^1)(U)$. Với mỗi cặp $(U,V)$ các tập mở của B sao cho $U\subset V$, cho $m_{UV}:\mathscr{M}(V)\rightarrow \mathscr{M}(U)$ là ánh xạ mà gán cho một cấu xạ V

$f:\overset{-1}{p}(V)\rightarrow (^-{p'}^1)(V)$ cấu xạ U từ $\overset{-1}{p}(U)$ vào $(^-{p'}^1)(U)$ suy ra từ $f$ bằng cách chuyển qua các tập con. Khi đó $(\mathscr{M}(U), m_{UV})$ là một bó trên B. Nó được ký hiệu bởi $\mathscr{M}$or$_B(E; E')$ và được gọi là bó trên B các cấu xạ B từ $(E, p)$ vào $(E', p')$.

Đối với mọi tập mở U của B, cho $\mathscr{I}$s(U) là tập con của $\mathscr{M}(U)$

gồm các đẳng cấu U của $\overset{-1}{p}(U)$ vào $(^-{p'}^1)(U)$. Họ $(\mathscr{I}$s(U)) là một dưới bó của bó $\mathscr{M}$or$_B(E; E')$ của các cấu xạ từ $(E, p)$ vào $(E', p')$. Bó thu được như vậy được ký hiệu là $\mathscr{I}$som$_B(E; E')$ và được gọi là bó trên B của các B-đẳng cấu từ $(E, p)$ vào $(E', p')$.

5) Các bó các ánh xạ thuộc lớp $C^r$

Cho X và Y là các đa tạp thuộc lớp $C^r$ trên một trường K (các quy ước liên quan đến K và $r$ là các quy ước của VAR, R). Đối với mọi tập mở U của X, cho $\mathscr{C}^r(U; Y)$ là tập các cấu xạ thuộc lớp $C^r$ từ U vào Y. Họ $(\mathscr{C}^r(U; Y))$ là một dưới bó của bó $\mathscr{C}(X; Y)$. Bó thu được như vậy được ký hiệu là $\mathscr{C}^r(X; Y)$ và được gọi là bó trên X của các ánh xạ thuộc lớp $C^r$ có giá trị trong Y (xem VAR, R, 5.4.2).

6) Các bó các không gian con

Nếu U và V là các tập mở của B sao cho $U\subset V$, ký hiệu $i_{UV}:\mathfrak{P}(V)\rightarrow$ $\mathfrak{P}(U)$ là ánh xạ gán cho một tập con A của V tập $A\cap U$. Cặp $(\mathfrak{P}(U), i_{UV})$ là một bó, được gọi là bó các không gian con của B và được ký hiệu là $\mathfrak{P}(B)$. Thật vậy, nếu X ký hiệu tập $\{0; 1\}$, ánh xạ gán cho mỗi tập con A của U hàm đặc trưng của nó $\varphi^U_A: U\rightarrow X$ là một song ánh của $\mathfrak{P}(U)$ lên $\mathscr{F}(U; X)$ (E, III, p. 38) ; hơn nữa, nếu U và V là các tập mở sao cho $U\subset V$, với mọi tập con A của V$,\varphi^U_{A\cap U}$ là hạn chế vào U của $\varphi^V_A$ sao cho $\mathfrak{P}(B)$ được đồng nhất với bó trên B của các ánh xạ có giá trị trong X.

Cho, với mọi tập mở U của B$,\mathscr{L}(U)$ là một tập con của $\mathfrak{P}(U)$. Để $(\mathscr{L}(U))$ là một dưới bó của $\mathfrak{P}(B)$, điều kiện cần và đủ là điều kiện sau được thỏa mãn:

$(F')$ Cho $(U_i)_{i\in I}$ là một họ các tập mở của B, U là hợp của chúng, và A là một

tập con của U ; để A thuộc $\mathscr{L}(U)$, điều kiện cần và đủ là đối với mọi $i$ trong I,

$A\cap U_i$ thuộc $\mathscr{L}(U_i)$.

Ví dụ, nếu $\mathscr{L}(U)$ là tập các tập con đóng của U, điều kiện $(F')$ được thỏa mãn.

7) Tích của các bó

Cho $\mathscr{B}$ là một cơ sở của tôpô của B và I là một tập hợp. Với mỗi $i\in I$, cho $\mathscr{F}_i= (\mathscr{F}_i(U), f_{i,UV})$ là một tiền bó trên B đối với cơ sở $\mathscr{B}$. Với mỗi tập mở $U\in \mathscr{B}$, đặt $\mathscr{F}(U) =\prod_{i\in I}\mathscr{F}_i(U)$, và với mỗi cặp $(U,V)$ các phần tử của $\mathscr{B}$ sao cho $U\subset V$, ký hiệu $f_{UV}$ là ánh xạ $(f_{i,UV})_{i\in I}:\mathscr{F}(V)\rightarrow \mathscr{F}(U)$. Khi đó $(\mathscr{F}(U), f_{UV})$ là một tiền bó trên B đối với $\mathscr{B}$ được gọi là tiền bó tích của họ $(\mathscr{F}_i)$ và được ký hiệu $\prod_{i\in I}\mathscr{F}_i$. Nó là một bó nếu với mọi $i\in I,\mathscr{F}_i$ là một bó.

### 4. Các cấu xạ của tiền bó

#### Định nghĩa 3 {#ta-i-s3-def-3 .statement tag=01NV}

Cho B là một không gian tôpô, $\mathscr{B}$ là một cơ sở của tôpô của B$,\mathscr{F}= (\mathscr{F}(U), f_{UV})$ và $\mathscr{G}= (\mathscr{G}(U), g_{UV})$ là các tiền bó trên B đối với $\mathscr{B}$. Một cấu xạ của các tiền bó từ $\mathscr{F}$ đến $\mathscr{G}$ được gọi là một hệ xạ ảnh của các ánh xạ từ $\mathscr{F}$ đến $\mathscr{G}$.

Nói cách khác (E, III, p. 54), một cấu xạ của các tiền bó từ $\mathscr{F}$ đến $\mathscr{G}$ là một họ $(\varphi_U)_{U\in\mathscr{B}}$ sao cho:

(MPF$_1$) Với mỗi tập mở U thuộc $\mathscr{B},\varphi_U$ là một ánh xạ

từ $\mathscr{F}(U)$ vào $\mathscr{G}(U)$ ;

(MPF$_2$) Với mỗi cặp $(U,V)$ các tập mở thuộc $\mathscr{B}$ sao cho

$U\subset V$, ta có $\varphi_U\circ f_{UV}=g_{UV}\circ \varphi_V$.

Khi $\mathscr{F}$ và $\mathscr{G}$ là các bó, một cấu xạ của các tiền bó từ $\mathscr{F}$ đến $\mathscr{G}$ cũng được gọi là một cấu xạ của các bó. Nếu $\mathscr{F}$ và $\mathscr{G}$ là các tiền bó trên B đối với $\mathscr{B}$, các cấu xạ của các tiền bó từ $\mathscr{F}$ đến $\mathscr{G}$ tạo thành một tập hợp được ký hiệu Mor($\mathscr{F};\mathscr{G}$). Thay vì nói: “cho $\varphi$ là một cấu xạ của các tiền bó từ $\mathscr{F}$ đến $\mathscr{G}$”, người ta thường nói “cho $\varphi :\mathscr{F}\rightarrow \mathscr{G}$ là một cấu xạ của các tiền bó”.

Cho $\mathscr{F},\mathscr{G},\mathscr{H}$ là các tiền bó trên B đối với $\mathscr{B}$ và $\varphi :\mathscr{F}\rightarrow \mathscr{G}$, $\psi :\mathscr{G}\rightarrow \mathscr{H}$ là các cấu xạ của tiền bó. Họ $(\psi_U\circ \varphi_U)_{U\in\mathscr{B}}$ là một cấu xạ của các tiền bó từ $\mathscr{F}$ vào $\mathscr{H}$, được ký hiệu là $\psi \circ \varphi$. Họ (Id$_{\mathscr{F}(U)}$)$_{U\in\mathscr{B}}$ là một cấu xạ của các tiền bó từ $\mathscr{F}$ vào chính nó, được ký hiệu là Id$_{\mathscr{F}}$.

Đối với một cấu xạ của các tiền bó $\varphi = (\varphi_U):\mathscr{F}\rightarrow \mathscr{G}$, để là một đẳng cấu, điều kiện cần và đủ là, với mọi tập con mở U của $\mathscr{B},\varphi_U$ là một song ánh từ $\mathscr{F}(U)$ lên $\mathscr{G}(U)$. Điều này tương đương với việc nói rằng tồn tại một cấu xạ của các tiền bó $\psi :\mathscr{G}\rightarrow \mathscr{F}$ sao cho $\psi \circ \varphi =$ Id$_{\mathscr{F}}$ và $\varphi \circ \psi =$ Id$_{\mathscr{G}}$.

Cho $\mathscr{F}$ và $\mathscr{G}$ là các tiền bó trên B, đối với một cơ sở $\mathscr{B}$ của tôpô của B, cho $B'$ là một tập con mở của B và $\mathscr{B}'$ là một cơ sở của tôpô của $B'$ sao cho $\mathscr{B}'\subset \mathscr{B}$. Cho $\varphi = (\varphi_U)_{U\in\mathscr{B}}$ là một cấu xạ của các tiền bó từ $\mathscr{F}$ vào $\mathscr{G}$. Khi đó $(\varphi_U)_{U\in\mathscr{B}'}$ là một cấu xạ của các tiền bó từ $\mathscr{F}|\mathscr{B}'$ vào $\mathscr{G}|\mathscr{B}'$, được ký hiệu là $\varphi |\mathscr{B}'$. Khi $\mathscr{B}$ là tập hợp các tập con mở của B và $\mathscr{B}'$ là tập hợp các tập con mở của $B',\varphi |\mathscr{B}'$ là một cấu xạ của các tiền bó từ $\mathscr{F}|B'$ vào $\mathscr{G}|B'$ và cũng được ký hiệu là $\varphi |B'$.

#### Ví dụ 1 {#ta-i-s3-n4-exa-1 .statement tag=01NW}

Cho B là một không gian tôpô, cho $(E, p)$ và $(E', p')$ là các không gian B và cho $f: E\rightarrow E'$ là một B-cấu xạ. Với mọi tập con mở U của B, định nghĩa ánh xạ $f_U:\mathscr{S}(U; E)\rightarrow \mathscr{S}(U; E')$ bởi $f_U(s) =$ $f\circ s$. Họ $\mathscr{S}(f) = (f_U)$ là một cấu xạ của các tiền bó từ $\mathscr{S}(B; E)$ vào $\mathscr{S}(B; E')$. Nếu $(E'', p'')$ là một không gian B và $g: E'\rightarrow E''$ là một B-cấu xạ, ta có $\mathscr{S}(g\circ f) =\mathscr{S}(g)\circ \mathscr{S}(f)$.

#### Ví dụ 2 {#ta-i-s3-n4-exa-2 .statement tag=01NX}

Cho B là một không gian tôpô, $\mathscr{B}$ là một cơ sở của tôpô của B, $\mathscr{F}= (\mathscr{F}(U), f_{UV})$ là một tiền bó trên B tương đối với $\mathscr{B}$ và $\mathscr{L}= (\mathscr{L}(U))$ là một tiền bó con của $\mathscr{F}$. Với mọi tập hợp mở $U\in \mathscr{B}$, ký hiệu $i_U$ là đơn ánh chính tắc của $\mathscr{L}(U)$ vào $\mathscr{F}(U)$. Khi đó $i= (i_U)_{U\in\mathscr{B}}$ là một cấu xạ của các tiền bó từ $\mathscr{L}$ vào $\mathscr{F}$. Ta gọi $i$ là cấu xạ chính tắc từ $\mathscr{L}$ vào $\mathscr{F}$.

#### Ví dụ 3 {#ta-i-s3-n4-exa-3 .statement tag=01NY}

Cho B là một không gian tôpô, $\mathscr{B}$ là một cơ sở của tôpô của B và I là một tập hợp. Với mọi $i\in I$, cho $\mathscr{F}_i= (\mathscr{F}_i(U), f_{i,UV})$ là một tiền bó trên B tương đối với $\mathscr{B}$. Ký hiệu $\mathscr{F}$ là tiền bó tích của họ $(\mathscr{F}_i)_{i\in I}$. Với mọi tập hợp mở $U\in \mathscr{B}$, ta có $\mathscr{F}(U) =\prod_{i\in I}\mathscr{F}_i(U)$; với mọi $i\in I$, ký hiệu pr$_{i,U}:\mathscr{F}(U)\rightarrow \mathscr{F}_i(U)$ là phép chiếu có chỉ số $i$. Theo ngay lập tức từ định nghĩa của tiền bó $\mathscr{F}$ rằng họ pr$_i$ = (pr$_{i,U}$)$_{U\in\mathscr{B}}$ là một cấu xạ của các tiền bó từ $\mathscr{F}$ vào $\mathscr{F}_i$. Cấu xạ pr$_i$ được gọi là cấu xạ phép chiếu có chỉ số $i$. Với mọi tiền bó $\mathscr{F}'$ trên B tương đối với $\mathscr{B}$ và mọi họ $(\psi_i)_{i\in I}$, trong đó $\psi_i$ là một cấu xạ của các tiền bó từ $\mathscr{F}'$ vào $\mathscr{F}_i$, tồn tại một cấu xạ duy nhất của các tiền bó $\psi :\mathscr{F}'\rightarrow \mathscr{F}$ sao cho với mọi $i\in I$, pr$_i\circ \psi =\psi_i$.

#### Ví dụ 4 {#ta-i-s3-n4-exa-4 .statement tag=01NZ}

Cho X là một đa tạp vi phân lớp $C^{\infty}$ trên $\mathbf{R}$ và cho $\mathscr{C}^{\infty}(X;\mathbf{R})$ là bó trên X của các hàm số lớp $C^{\infty}$. Nếu P là một toán tử vi phân với các hệ số $C^{\infty}$ trên X, thì họ các hạn chế của P lên các tập hợp mở của X là một cấu xạ của bó $\mathscr{C}^{\infty}(X;\mathbf{R})$ vào chính nó. Có thể chứng minh rằng ngược lại, mọi cấu xạ $\mathbf{R}$-tuyến tính của bó $\mathscr{C}^{\infty}(X;\mathbf{R})$ vào chính nó đều có dạng này địa phương (I, p. 142, bài tập 3).

### 5. Không gian Étale liên kết với một tiền bó

Cho B là một không gian tôpô, $\mathscr{B}$ là một cơ sở của tôpô của B và $\mathscr{F}= (\mathscr{F}(U), r_{UV})$ là một tiền bó trên B đối với cơ sở $\mathscr{B}$. Gọi L là tập hợp các cặp $(U, s)$ với U $\in \mathscr{B}$ và $s\in \mathscr{F}(U)$. Ký hiệu $X_{\mathscr{F}}$ là không gian tổng của họ $(U)_{(U,s)\in L}$. Do đó $X_{\mathscr{F}}$ là tập hợp các bộ ba $(U, s, x)$ trong đó $U\in \mathscr{B},s\in \mathscr{F}(U),x\in U$. Gọi $R_{\mathscr{F}}$ là quan hệ trong tập hợp $X_{\mathscr{F}}$ được xác định bởi $R_{\mathscr{F}}((U, s, x),(U', s', x'))$ khi và chỉ khi « $x$ = $x'$ và tồn tại W $\in \mathscr{B}$ sao cho $x\in W$, W $\subset U\cap U'$ và $r_{WU}(s) =r_{WU'}(s')$ ». Quan hệ $R_{\mathscr{F}}$ là một quan hệ tương đương trong $X_{\mathscr{F}}:$ theo định nghĩa, nó phản xạ và đối xứng; ta hãy chứng minh rằng nó bắc cầu. Cho $\xi = (U, s, x),\xi '= (U', s', x')$ và $\xi ''$ = $(U'', s'', x'')$ là các phần tử của $X_{\mathscr{F}}$ sao cho $R_{\mathscr{F}}(\xi , \xi ')$ và $R_{\mathscr{F}}(\xi ', \xi '')$. Khi đó ta có $x=x'$ = $x''$ và tồn tại hai phần tử $W'$ và $W''$ của $\mathscr{B}$ chứa $x$ sao cho $W'\subset U\cap U',W''\subset U'\cap U'',r_{W'U}(s) =$ $r_{W'U'}(s'),r_{W''U'}(s') =r_{W''U''}(s'')$. Lấy W là một phần tử của $\mathscr{B}$ chứa $x$ và được chứa trong $W'\cap W''$. Khi đó ta có $W\subset U\cap U''$,

$$
r_{WU}(s) =r_{WW'}\circ r_{W'U}(s) =r_{WW'}\circ r_{W'U'}(s') =r_{WU'}(s')
$$

và, tương tự, $r_{WU'}(s') =r_{WU''}(s'')$. Do đó, ta có $R_{\mathscr{F}}(\xi , \xi '')$ và quan hệ $R_{\mathscr{F}}$ là bắc cầu.

Gọi $E_{\mathscr{F}}$ là tập thương $X_{\mathscr{F}}/R_{\mathscr{F}}$ và $[U, s, x]$ là ảnh chính tắc trong $E_{\mathscr{F}}$ của một phần tử $(U, s, x)$ của $X_{\mathscr{F}}$. Với $U\in \mathscr{B}$ và $s\in \mathscr{F}(U)$, gọi $\sigma_{\mathscr{F}}(U, s): U\rightarrow E_{\mathscr{F}}$ là ánh xạ $x\mapsto [U, s, x]$. Trang bị cho tập $E_{\mathscr{F}}$ tôpô thương, tức là tôpô mịn nhất sao cho các ánh xạ $\sigma_{\mathscr{F}}(U, s)$ với $U\in \mathscr{B}$ và $s\in \mathscr{F}(U)$ là liên tục. Ánh xạ pr$_3: X_{\mathscr{F}}\rightarrow B$ xác định, sau khi chuyển qua thương, một ánh xạ liên tục $p: E_{\mathscr{F}}\rightarrow B$ : ta có $p([U, s, x]) =x$.

#### Mệnh đề 1 {#ta-i-s3-prop-1 .statement tag=01O0}

Ánh xạ $p: E_{\mathscr{F}}\rightarrow$ B là etale. Với mọi tập mở $U\in \mathscr{B}$ và mọi $s\in \mathscr{F}(U)$, ánh xạ $\sigma_{\mathscr{F}}(U, s)$ do đó là một tiết diện liên tục của $p$ trên U.

Cho $\lambda = (U, s)$ và $\mu= (U', s')$ là các phần tử của L. Theo định nghĩa của quan hệ $R_{\mathscr{F}}$, tập $A_{\lambda \mu}$ các điểm $x$ của $U\cap U'$ tại đó $\sigma_{\mathscr{F}}(U, s)$ và $\sigma_{\mathscr{F}}(U', s')$ trùng nhau là phần trong trong B, của tập các $x\in U\cap U'$ sao cho $s(x) =s'(x)$. Suy ra rằng $A_{\mu\lambda}= A_{\lambda \mu}$. Khi đó ta ký hiệu $h_{\mu\lambda}: A_{\lambda \mu}\rightarrow A_{\mu\lambda}$ là ánh xạ Id$_{A_{\lambda \mu}}$. Tập $E_{\mathscr{F}}$ thu được bằng cách dán các tập mở U dọc theo các $A_{\lambda \mu}$ bằng các song ánh $h_{\mu\lambda}$ (TG, I, p. 16). Theo mệnh đề 9 của TG, I, p. 17, ánh xạ $\sigma_{\mathscr{F}}(U, s)$ cảm sinh một đồng phôi từ U lên một tập con mở của $E_{\mathscr{F}}$. Điều này chứng minh rằng ánh xạ $p$ là etale (I, p. 33, mệnh đề 9).

Với mọi tập mở $U\in \mathscr{B}$ và mọi $s\in \mathscr{F}(U)$, ta có $\sigma_{\mathscr{F}}(U, s)(x) =$ $[U, s, x]$ với mọi $x\in U$. Khẳng định thứ hai do đó suy ra từ định nghĩa của $p$.

#### Định nghĩa 4 {#ta-i-s3-def-4 .statement tag=01O1}

Không gian B trải $(E_{\mathscr{F}}, p)$ được xác định ở trên được gọi là không gian B trải liên kết với bó tiền bó $\mathscr{F}$. Với $x\in B$, thớ của $E_{\mathscr{F}}$ tại $x$ được gọi là mầm của bó tiền bó $\mathscr{F}$ tại $x$ và được ký hiệu là $\mathscr{F}_x$. Với mọi tập mở $U\in \mathscr{B}$, mọi tiết diện $s\in \mathscr{F}(U)$ của $\mathscr{F}$ trên U và mọi điểm $x$ của U, phần tử $[U, s, x]$ của $E_{\mathscr{F}}$ được gọi là mầm tại $x$ của tiết diện $s$.

Cho $a$ là một điểm của B. Tập hợp $\mathscr{B}(a)$ gồm các tập mở $U\in \mathscr{B}$ chứa $a$ và có thứ tự theo quan hệ $\supset$ là lọc. Từ $\mathscr{F}$ suy ra, bằng hạn chế tập hợp các chỉ số vào $\mathscr{B}(a)$, một hệ quy nạp $((\mathscr{F}(U))_{U\in\mathscr{B}(a)},(r_{UV}))$. Theo định nghĩa (E, III, p. 60), giới hạn quy nạp của hệ này là thương của tập hợp các cặp $(U, s)$ sao cho $a\in U$ và $s\in \mathscr{F}(U)$ theo quan hệ tương đương R được xác định bởi $R((U, s),(U', s'))$ khi và chỉ khi tồn tại W $\in \mathscr{B}$ chứa $a$ và được chứa trong $U\cap U'$ sao cho $r_{WU}(s) =r_{WU'}(s')$. Do đó, theo định nghĩa của các giới hạn quy nạp, giới hạn này được đồng nhất với mầm $\mathscr{F}_a$ của $\mathscr{F}$ tại $a$.

Cho $\mathscr{G}$ là một bó tiền bó trên B đối với cơ sở $\mathscr{B}$ và cho $\varphi = (\varphi_U)_{U\in\mathscr{B}}$ là một cấu xạ của các bó tiền bó từ $\mathscr{F}$ vào $\mathscr{G}$. Ánh xạ $(U, s, x)\mapsto$ $(U, \varphi_U(s), x)$ từ $X_{\mathscr{F}}$ vào $X_{\mathscr{G}}$ tương thích với các quan hệ tương đương $R_{\mathscr{F}}$ và $R_{\mathscr{G}}$, theo định nghĩa của một cấu xạ của các bó tiền bó. Ta ký hiệu $E(\varphi ): E_{\mathscr{F}}\rightarrow E_{\mathscr{G}}$ là ánh xạ suy ra từ nó bằng cách chuyển qua các thương. Với mọi $U\in \mathscr{B}$ và mọi $s\in \mathscr{F}(U)$, ta có

$$
E(\varphi )\circ \sigma_{\mathscr{F}}(U, s) =\sigma_{\mathscr{G}}(U, \varphi_U(s))
$$

do đó, ánh xạ $E(\varphi )$ là liên tục. Ánh xạ $E(\varphi )$ là một B-cấu xạ; nó được gọi là B-cấu xạ của $E_{\mathscr{F}}$ vào $E_{\mathscr{G}}$ liên kết với cấu xạ của các tiền bó $\varphi$. Với mọi $a\in B$, bằng cách hạn chế vào các thớ tại $a$, $E(\varphi )$ xác định một ánh xạ từ thân $\mathscr{F}_a$ của $\mathscr{F}$ vào thân $\mathscr{G}_a$ của $\mathscr{G}$; nó được ký hiệu là $\varphi_a$. Nó cũng là giới hạn quy nạp của các ánh xạ $\varphi_U$ (E, III, p. 63), trong đó U chạy trên tập hợp $\mathscr{B}(a)$ gồm các tập mở thuộc cơ sở $\mathscr{B}$ và chứa $a$.

Ta có E(Id$_{\mathscr{F}}$) $=$ Id$_{E_{\mathscr{F}}}$.

Cho $\mathscr{H}$ là một tiền bó trên B đối với $\mathscr{B}$ và cho $\psi = (\psi_U)$ là một cấu xạ của các tiền bó từ $\mathscr{G}$ vào $\mathscr{H}$. Với $[U, s, x]\in E_{\mathscr{F}}$, ta có

$$
E(\psi \circ \varphi )([U, s, x]) = [U, \psi_U\circ \varphi_U(s), x]
$$

$$
= E(\psi )([U, \varphi_U(s), x])
$$

$$
= E(\psi )\circ E(\varphi )([U, s, x])
$$

Do đó, ta có $E(\psi \circ \varphi ) = E(\psi )\circ E(\varphi )$. Đặc biệt, nếu $a$ là một điểm của B, $(\psi \circ \varphi )_a=\psi_a\circ \varphi_a$.

Nếu $\varphi$ là một đẳng cấu, thì điều tương tự cũng đúng với $E(\varphi )$.

#### Nhận xét {#ta-i-s3-n5-rem-1 .statement tag=01O2}

Cho $\mathscr{F}$ là một bó trên B đối với cơ sở $\mathscr{B}$. Cho $B'$ là một tập con mở của B, cho $\mathscr{B}'$ là một cơ sở của tôpô của $B'$ sao cho $\mathscr{B}'\subset \mathscr{B}$. Cho $\mathscr{F}|\mathscr{B}'$ là tiền bó trên $B'$ đối với cơ sở $\mathscr{B}'$ suy ra từ $\mathscr{F}$ bằng cách hạn chế.

1) Tập hợp $X_{\mathscr{F}|\mathscr{B}'}$ khi đó là một tập con của $X_{\mathscr{F}}$ và quan hệ tương đương $R_{\mathscr{F}}$ cảm sinh trong $X_{\mathscr{F}|\mathscr{B}'}$ quan hệ tương đương $R_{\mathscr{F}|\mathscr{B}'}$. Do đó suy ra một đơn ánh chính tắc $i$ của $E_{\mathscr{F}|\mathscr{B}'}$ vào $E_{\mathscr{F}}$. Ảnh của nó là $\overset{-1}{p}(B')$ vì với mọi phần tử $[U, s, x]$ của $\overset{-1}{p}(B')$, tồn tại một phần tử V của $\mathscr{B}'$ sao cho $x\in V$ và $V\subset U$, và ta có $[U, s, x] =i([V, r_{VU}(s), x])$. Ánh xạ $i$ là liên tục vì tôpô của $X_{\mathscr{F}|\mathscr{B}'}$ là tôpô mịn nhất làm cho các ánh xạ được xác định bởi $x\mapsto [U, s, x]$, với $U\in \mathscr{B}'$ và $s\in \mathscr{F}(U)$, trở nên liên tục. Theo hệ quả 2 của Mệnh đề 6 trong I, p. 30, đơn ánh chính tắc $i$ của $E_{\mathscr{F}|\mathscr{B}'}$ vào $E_{\mathscr{F}}$ cảm sinh một đẳng cấu $B'$-của $E_{\mathscr{F}|\mathscr{B}'}$ lên $\overset{-1}{p}(B')$.

Đặc biệt, khi $B'$ bằng B$,i: E_{\mathscr{F}|\mathscr{B}'}\rightarrow E_{\mathscr{F}}$ là một đẳng cấu B của các không gian étalé.

2) Cho $\mathscr{G}$ là một tiền bó trên B đối với cơ sở $\mathscr{B}$ và cho $\varphi :\mathscr{F}\rightarrow \mathscr{G}$ là một cấu xạ của các tiền bó. Họ $\varphi '= (\varphi_U)_{U\in\mathscr{B}'}$ là một cấu xạ của các tiền bó từ $\mathscr{F}|\mathscr{B}'$ vào $\mathscr{G}|\mathscr{B}'$. Biểu đồ

$$
E\mathscr{F}|\mathscr{B}'E(\varphi ')E\mathscr{G}|\mathscr{B}'
$$

$ii'$

$E_{\mathscr{F}}^{E(\varphi)}E_{\mathscr{G}}$ , trong đó $i$ và $i'$ là các đơn ánh chính tắc, là giao hoán.

#### Ví dụ 1 {#ta-i-s3-n5-exa-1 .statement tag=01O3}

Cho B là một không gian tôpô, $\mathscr{B}$ là một cơ sở của tôpô của B và F là một tập hợp. Lấy $\mathscr{F}$ là tiền bó trên B đối với cơ sở $\mathscr{B}$ được xác định bởi $\mathscr{F}(U) = F$ với mọi $U\in \mathscr{B}$ và $r_{UV}$ = Id$_F$ với mọi cặp $(U,V)$ của các phần tử của $\mathscr{B}$ sao cho $U\subset V$. Ánh xạ $[U, s, x]\mapsto (x, s(x))$ là một đẳng cấu B của không gian B $E_{\mathscr{F}}$ lên không gian B $B\times F$ trong đó F được trang bị tôpô rời rạc. Ta sẽ nhận xét rằng khi $\mathscr{B}$ là tập hợp các tập con mở của B, tiền bó $\mathscr{F}$ trên B là một bó chỉ khi tập hợp F được rút gọn thành một điểm (xem I, p. 43, nhận xét).

#### Ví dụ 2 {#ta-i-s3-n5-exa-2 .statement tag=01O4}

Cho B là một không gian tôpô và $(E, p)$ là một B-không gian. Cho $\mathscr{F}$ là bó trên B của các tiết diện liên tục của $(E, p)$. Ánh xạ $(U, s, x)\mapsto s(x)$ từ $X_{\mathscr{F}}$ vào E là tương thích với quan hệ tương đương $R_{\mathscr{F}}$. Ánh xạ $e: E_{\mathscr{F}}\rightarrow E$ suy ra từ nó bằng cách chuyển qua thương là một B-cấu xạ; B-cấu xạ $e$ được gọi là chính tắc. Ảnh của $e$ là hợp của các ảnh của các tiết diện liên tục của $p$ trên các tập mở của B. Do đó ánh xạ $e$ là toàn ánh nếu $p$ là etale (I, p. 33, prop. 9). Mặt khác, ánh xạ $e$ là đơn ánh khi và chỉ khi với mọi tập mở U của B và mọi cặp $(s, s')$ các tiết diện liên tục của $p$ trên U, tập hợp các điểm $x\in U$ sao cho $s(x) =s'(x)$ là mở; đặc biệt đây là trường hợp nếu $p$ là etale (I, p. 34, prop. 11, b)). Do đó, nếu $(E, p)$ là một B-không gian etale, ánh xạ $e$ là một B-đẳng cấu.

#### Ví dụ 3 {#ta-i-s3-n5-exa-3 .statement tag=01O5}

Cho B là một không gian tôpô, $\mathscr{B}$ là một cơ sở của tôpô của B$,\mathscr{F}$ là một tiền bó trên B tương đối với $\mathscr{B}$ và $\mathscr{L}$ là một tiền bó con của $\mathscr{F}$. Khi đó tập hợp $X_{\mathscr{L}}$ được chứa trong tập hợp $X_{\mathscr{F}}$ và quan hệ tương đương $R_{\mathscr{F}}$ cảm sinh trong $X_{\mathscr{L}}$ quan hệ tương đương $R_{\mathscr{L}}$. B-cấu xạ $E(i): E_{\mathscr{L}}\rightarrow E_{\mathscr{F}}$ liên kết với cấu xạ chính tắc $i:\mathscr{L}\rightarrow \mathscr{F}($I, p. 48, ví dụ 2) do đó là đơn ánh. Vì $E_{\mathscr{L}}$ và $E_{\mathscr{F}}$ là các B-không gian etale, ánh xạ $E(i)$ là mở và thậm chí là etale (I, p. 30, cor. 1), và do đó cảm sinh một đồng phôi của $E_{\mathscr{L}}$ lên một tập con mở của $E_{\mathscr{F}}$.

### 6. Bó liên kết với một tiền bó

Ta giữ lại ký hiệu của No.$^o5$. Bó liên kết với tiền bó $\mathscr{F}$ là bó $\mathscr{S}(B; E_{\mathscr{F}})$ của các tiết diện liên tục của B-không gian etale $E_{\mathscr{F}}$ liên kết với tiền bó $\mathscr{F}$, và được ký hiệu bởi $\widetilde{\mathscr{F}}$. Với mỗi tập mở $U\in \mathscr{B}$, ký hiệu $\sigma_{\mathscr{F}}(U):\mathscr{F}(U)\rightarrow \widetilde{\mathscr{F}}(U)$ là ánh xạ mà, với $s\in \mathscr{F}(U)$, liên kết tiết diện liên tục $\sigma_{\mathscr{F}}(U, s):x\mapsto [U, s, x]$ của $E_{\mathscr{F}}$ trên U. Theo định nghĩa của quan hệ tương đương $R_{\mathscr{F}}$, họ $\sigma_{\mathscr{F}}= (\sigma_{\mathscr{F}}(U))_{U\in\mathscr{B}}$ là một cấu xạ của các tiền bó từ $\mathscr{F}$ vào tiền bó $\widetilde{\mathscr{F}}|\mathscr{B}$. Cấu xạ $\sigma_{\mathscr{F}}$ được gọi là cấu xạ chính tắc của $\mathscr{F}$ vào $\widetilde{\mathscr{F}}|\mathscr{B}$.

Ta ký hiệu bởi $j_{\mathscr{F}}: E_{\mathscr{F}}\rightarrow E_{\mathscr{F}}$ cấu xạ B là hợp thành của đẳng cấu B chính tắc $E_{\mathscr{F}|\mathscr{B}}\rightarrow E_{\mathscr{F}}\widetilde{(}I$, p. 51) và cấu xạ B $E(\sigma_{\mathscr{F}}): E_{\mathscr{F}}\rightarrow$ $E_{\widetilde{\mathscr{F}}|\mathscr{B}}$. Mặt khác, ta ký hiệu$\widetilde{s}$ bởi $e_{\mathscr{F}}:E_{\widetilde{\mathscr{F}}}\rightarrow E_{\mathscr{F}}$ đẳng cấu B chính tắc (I, p. 52, ví dụ 2).

#### Mệnh đề 2 {#ta-i-s3-prop-2 .statement tag=01O6}

Ánh xạ $j_{\mathscr{F}}$ là đẳng cấu B nghịch đảo của $e_{\mathscr{F}}$.

Với $U\in \mathscr{B},s\in \mathscr{F}(U)$ và $x\in U$, theo định nghĩa của $j_{\mathscr{F}}$ ta có:

$$
j_{\mathscr{F}}([U, s, x]) = [U, \sigma_{\mathscr{F}}(U, s), x]
$$

do đó $e_{\mathscr{F}}(j_{\mathscr{F}}([U, s, x])) =\sigma_{\mathscr{F}}(U, s)(x) = [U, s, x]$. Điều này chứng minh mệnh đề.

#### Hệ quả {#ta-i-s3-n6-cor-1 .statement tag=01O7}

Với mọi $a\in B$, ánh xạ $(\sigma_{\mathscr{F}})_a:\mathscr{F}_a\rightarrow \widetilde{\mathscr{F}}_a$ là song ánh.

Vì $j_{\mathscr{F}}$ là một đẳng cấu B, điều tương tự cũng đúng với $E(\sigma_{\mathscr{F}})$, và $(\sigma_{\mathscr{F}})_a$ được suy ra từ nó bằng cách chuyển qua các thớ tại $a$.

Cho $\mathscr{G}$ là một tiền bó trên B đối với $\mathscr{B}$ và cho $\varphi :\mathscr{F}\rightarrow \mathscr{G}$ là một cấu xạ của các tiền bó. Ta ký hiệu bởi $\widetilde{\varphi}:\widetilde{\mathscr{F}}\rightarrow \widetilde{\mathscr{G}}$ cấu xạ của các bó $\mathscr{S}_{E(\varphi)}($I, p. 48, ví dụ 1), trong đó $E(\varphi ): E_{\mathscr{F}}\rightarrow E_{\mathscr{G}}$ là cấu xạ B liên kết với $\varphi$. Với mọi tập mở $U\in \mathscr{B}$ và mọi $s\in \mathscr{F}(U)$, theo định nghĩa ta có,

$$
\widetilde{\varphi}_U(\sigma_{\mathscr{F}}(U, s)) = E(\varphi )\circ \sigma_{\mathscr{F}}(U, s) =\sigma_{\mathscr{G}}(U, \varphi_U(s))
$$

Do đó ta có:

(1) $\widetilde{\varphi}_U\circ \sigma_{\mathscr{F}}(U) =\sigma_{\mathscr{G}}(U)\circ \varphi_U$, với mọi $U\in \mathscr{B}$. Nói cách khác:

$$
\widetilde{\varphi}|\mathscr{B}\circ \sigma_{\mathscr{F}}=\sigma_{\mathscr{G}}\circ \varphi \tag{2}
$$

#### Mệnh đề 3 {#ta-i-s3-prop-3 .statement tag=01O8}

Cho B là một không gian tôpô, cho $\mathscr{B}$ là một cơ sở của tôpô của B, cho $\mathscr{F}= (\mathscr{F}(U), f_{UV})$ là một tiền bó trên B đối với $\mathscr{B}$, cho $\widetilde{\mathscr{F}}$ là bó liên kết và cho $\sigma_{\mathscr{F}}:\mathscr{F}\rightarrow \widetilde{\mathscr{F}}|\mathscr{B}$ là cấu xạ chính tắc. Cho một bó $\mathscr{G}= (\mathscr{G}(U), g_{UV})$ trên B và một cấu xạ của các tiền bó $\varphi :\mathscr{F}\rightarrow \mathscr{G}|\mathscr{B}$, tồn tại một cấu xạ duy nhất của các bó $\psi :\widetilde{\mathscr{F}}\rightarrow \mathscr{G}$ sao cho $\psi |\mathscr{B}\circ \sigma_{\mathscr{F}}=\varphi$.

#### Bổ đề {#ta-i-s3-n6-lem-1 .statement tag=01O9}

Cho U là một tập con mở của B và $s: U\rightarrow E_{\mathscr{F}}$ là một tiết diện liên tục của $E_{\mathscr{F}}$ trên U. Với mọi điểm $a$ của U, tồn tại một tập mở $V\in \mathscr{B}$ sao cho $a\in V$ và $V\subset U$, và một phần tử $v$ của $\mathscr{F}(V)$ sao cho $s|V =\sigma_{\mathscr{F}}(V, v)$.

Cho $a\in U$. Theo định nghĩa của không gian $E_{\mathscr{F}}$, tồn tại một tập mở $V'\in \mathscr{B}$ sao cho $a\in V'$ và một phần tử $t$ của $\mathscr{F}(V')$ sao cho $s(a) = [V', t, a]$. Khi đó $s$ và $\sigma_{\mathscr{F}}(V', t)$ cảm sinh bởi phép hạn chế hai tiết diện liên tục của $E_{\mathscr{F}}$ trên $V'\cap U$, bằng nhau tại điểm $a$. Theo Mệnh đề 11, b) của I, p. 34, tồn tại một lân cận mở V của $a$, được chứa trong $V'\cap U$, thuộc $\mathscr{B}$, sao cho $s$ và $\sigma_{\mathscr{F}}(V', t)$ bằng nhau tại mọi điểm của V. Nếu đặt $v=f_{VV'}(t)$, ta thực sự có $s|V =\sigma_{\mathscr{F}}(V, v)$.

Ta hãy chứng minh mệnh đề. Với mỗi tập mở U của B và mỗi tiết diện $s\in \widetilde{\mathscr{F}}(U)$, ký hiệu $D(U, s)$ là tập hợp các cặp $(V, v)$ sao cho $V\in \mathscr{B},V\subset U,v\in \mathscr{F}(U)$ và $s|V =\sigma_{\mathscr{F}}(V, v)$. Theo bổ đề, các tập mở V này tạo thành một phủ của U.

Nếu tồn tại một cấu xạ $\psi :\widetilde{\mathscr{F}}\rightarrow \mathscr{G}$ sao cho $\psi |\mathscr{B}\circ \sigma_{\mathscr{F}}=\varphi$, thì, với mọi tập mở U của B, mọi tiết diện $s\in \widetilde{\mathscr{F}}(U)$ và mọi cặp $(V, v)\in D(U, s)$, ta có $g_{VU}(\psi_U(s)) =\psi_V(s|V) =\varphi_V(v)$. Điều này chứng minh tính duy nhất của $\psi$ theo tính chất $(F_1)$ của các bó.

Cho U là một tập mở của B và $s$ là một phần tử của $\widetilde{\mathscr{F}}(U)$. Cho $(V, v)$ và $(V', v')$ là các phần tử của $D(U, s)$. Ta có $s(a) = [V, v, a] = [V', v', a]$ với mọi điểm $a\in V\cap V'$. Do đó tồn tại một cặp $(W, w)\in D(V\cap V', s)$ sao cho $a\in W$ và $f_{WV}(v) =f_{WV}(v') =w$. Khi đó

$$
g_{W(V\cap V')}\circ g_{(V\cap V')V}(\varphi_V(v)) =g_{WV}(\varphi_V(v)) =\varphi_W(f_{WV}(v)) =\varphi_W(w)
$$

và tương tự,

$$
g_{W(V\cap V')}\circ g_{(V\cap V')V'}(\varphi_{V'}(v')) =\varphi_W(w)
$$

do đó

$$
g_{W(V\cap V')}\circ g_{(V\cap V')V}(\varphi_V(v)) =g_{W(V\cap V')}\circ g_{(V\cap V')V'}(\varphi_{V'}(v'))
$$

Theo tính chất $(F_1)$ của các bó, do đó ta có

$$
g_{(V\cap V')V}(\varphi_V(v)) =g_{(V\cap V')V'}(\varphi_{V'}(v'))
$$

Theo các tính chất $(F_1)$ và $(F_2)$ của các bó, tồn tại một phần tử duy nhất $\psi_U(s)\in \mathscr{G}(U)$ sao cho:

(3) $g_{VU}(\psi_U(s)) =\varphi_V(v)$ với mọi $(V, v)\in D(u, s)$.

Gọi $\psi_U:\widetilde{\mathscr{F}}(U)\rightarrow \mathscr{G}(U)$ là ánh xạ thu được. Từ (3) suy ra ngay lập tức rằng họ $\psi = (\psi_U)$ là một cấu xạ của các bó và ta có $\varphi_V=\psi_V\circ \sigma_{\mathscr{F}}(V)$ với mọi $V\in \mathscr{B}$.

#### Hệ quả 1 {#ta-i-s3-prop-3-cor-1 .statement tag=01OA}

Cho B là một không gian tôpô, $\mathscr{F}$ là một tiền bó trên B$,\widetilde{\mathscr{F}}$ là bó liên kết và $\sigma_{\mathscr{F}}:\mathscr{F}\rightarrow \widetilde{\mathscr{F}}$ là cấu xạ chính tắc. Để $\mathscr{F}$ là một bó, điều kiện cần và đủ là $\sigma_{\mathscr{F}}$ là một đẳng cấu.

Nếu $\sigma_{\mathscr{F}}$ là một đẳng cấu, thì $\mathscr{F}$ là một bó. Ngược lại, nếu $\mathscr{F}$ là một bó, theo mệnh đề 3 tồn tại một cấu xạ $\varphi :\widetilde{\mathscr{F}}\rightarrow \mathscr{F}$ sao cho $\varphi \circ \sigma_{\mathscr{F}}=$ Id$_{\mathscr{F}}$. Vì Id$_{\mathscr{F}}$ là cấu xạ duy nhất $\psi :\widetilde{\mathscr{F}}\rightarrow \widetilde{\mathscr{F}}$ sao cho $\psi \circ \sigma_{\mathscr{F}}=\sigma_{\mathscr{F}}$, do đó ta có $\widetilde{\sigma}_{\mathscr{F}}\circ \varphi =$ Id$_{\widetilde{\mathscr{F}}}$.

#### Nhận xét {#ta-i-s3-n6-rem-1 .statement tag=01OB}

Cho B là một không gian tôpô, $\mathscr{F}$ là một tiền bó trên B, $\mathscr{G}$ là một bó trên B và $\varphi :\mathscr{F}\rightarrow \mathscr{G}$ là một cấu xạ của các tiền bó. Cấu xạ chính tắc $\sigma_{\mathscr{G}}:\mathscr{G}\rightarrow \widetilde{\mathscr{G}}$ là một đẳng cấu theo hệ quả 1. Theo quan hệ (2) của I, p. 54, cấu xạ duy nhất $\psi :\widetilde{\mathscr{F}}\rightarrow \mathscr{G}$ sao cho $\psi \circ \sigma_{\mathscr{F}}=\varphi$ do đó là $\sigma^{-1}_{\mathscr{G}}\circ \widetilde{\varphi}$.

#### Hệ quả 2 {#ta-i-s3-prop-3-cor-2 .statement tag=01OC}

Cho B là một không gian tôpô, $\mathscr{F}$ và $\mathscr{G}$ là các bó trên B và $\varphi$ là một cấu xạ của các bó từ $\mathscr{F}$ vào $\mathscr{G}$. Các mệnh đề sau là tương đương:

(i) $\varphi$ là một đẳng cấu;

(ii) Tồn tại một cơ sở $\mathscr{B}$ của tôpô của B sao cho với mọi $U\in \mathscr{B}$, ánh xạ $\varphi_U$ là song ánh;

(iii) Với mọi điểm $a$ của B, ánh xạ $\varphi_a$ là một song ánh của mầm $\mathscr{F}_a$ lên mầm $\mathscr{G}_a$.

Hệ quả (i)$\Rightarrow$(ii) là ngay lập tức.

(ii)$\Rightarrow$(iii) : xét biểu đồ giao hoán (I, p. 51)

$$
E\mathscr{F}|\mathscr{B}E(\varphi |\mathscr{B})E\mathscr{G}|\mathscr{B}
$$

$$
E_{\mathscr{F}}^{E(\varphi)}E_{\mathscr{G}}
$$

trong đó các mũi tên đứng là các đẳng cấu B chính tắc. Nếu điều kiện (ii) được thỏa mãn, $E(\varphi |\mathscr{B})$ là một đẳng cấu B, do đó $E(\varphi )$ cũng là một đẳng cấu B. Các ánh xạ $\varphi_a$ được suy ra từ $E(\varphi )$ bằng cách chuyển qua các thớ và do đó là song ánh.

(iii)$\Rightarrow$(i) : theo giả thiết (iii), ánh xạ $E(\varphi ): E_{\mathscr{F}}\rightarrow E_{\mathscr{G}}$ là một cấu xạ B song ánh của các không gian étalé và do đó là một đẳng cấu B (I, p. 30, cor. 2 of prop. 6). Do đó cấu xạ $\widetilde{\varphi}:\widetilde{\mathscr{F}}\rightarrow \widetilde{\mathscr{G}}$ là một đẳng cấu. Vì $\mathscr{F}$ và $\mathscr{G}$ là các bó, các cấu xạ chính tắc $\sigma_{\mathscr{F}}:\mathscr{F}\rightarrow \widetilde{\mathscr{F}}$ và $\sigma_{\mathscr{G}}:\mathscr{G}\rightarrow \widetilde{\mathscr{G}}$ là các đẳng cấu (hệ quả 1) và ta có $\widetilde{\varphi}\circ \sigma_{\mathscr{F}}=\sigma_{\mathscr{G}}\circ \varphi ($I, p. 54, relation (2)) do đó $\varphi$ là một đẳng cấu.

#### Chú giải {#ta-i-s3-n6-sch-1 .statement tag=01OD}

Cho B là một không gian tôpô. Với mỗi bó $\mathscr{F}$ trên B, ta liên kết một không gian B étalé $E_{\mathscr{F}}$ (I, p. 50, def. 4). Với mỗi không gian B étalé T, ta liên kết bó $\mathscr{S}(T)$ trên B gồm các tiết diện liên tục của nó (I, p. 45, example 3). Một đẳng cấu chính tắc của các bó $\sigma_{\mathscr{F}}:\mathscr{F}\rightarrow \mathscr{S}(E_{\mathscr{F}})$ đã được định nghĩa (I, p. 55, cor. 1) và một đẳng cấu chính tắc của các không gian B étalé $e_T: E_{\mathscr{S}(T)}\rightarrow T$ (I, p. 52, example 2).

Với mỗi cặp $(\mathscr{F},\mathscr{G})$ các bó trên B, một ánh xạ $\varphi \mapsto E(\varphi )$ từ tập hợp các cấu xạ của các bó từ $\mathscr{F}$ vào $\mathscr{G}$ vào tập hợp các cấu xạ B từ $E_{\mathscr{F}}$ vào $E_{\mathscr{G}}$ đã được định nghĩa (I, p. 50). Ta có các quan hệ

E(Id$_{\mathscr{F}}$) $=$ Id$_{E_{\mathscr{F}}},E(\psi \circ \varphi ) = E(\psi )\circ E(\varphi )$.

Với mỗi cặp $(T,U)$ các không gian étalé trên B, một ánh xạ $f\mapsto \mathscr{S}(f)$ từ tập hợp các cấu xạ B của T vào U đến tập hợp các cấu xạ bó của $\mathscr{S}(T)$ vào $\mathscr{S}(U)$ đã được định nghĩa (I, p. 48, Ví dụ 1). Ta có các hệ thức

$\mathscr{S}$ (Id$_T$) $=$ Id$_{\mathscr{S}(T)},\mathscr{S}(g\circ f) =\mathscr{S}(g)\circ \mathscr{S}(f)$.

Với ký hiệu trên, các biểu đồ sau là giao hoán:

$$
\mathscr{F}^{\varphi}\mathscr{G}E_{\mathscr{S}(T)}^{E(\mathscr{S}(f))}E_{\mathscr{S}(U)}
$$

(4) $\sigma_{_{\mathscr{F}}}\sigma_{_{\mathscr{G}}}$ (5) $e_{_T}e_{_U}$

$\mathscr{S}(E_{\mathscr{F}})^{\mathscr{S}(E(\varphi))}\mathscr{S}(E_{\mathscr{G}})$, T $^fU$.

Điều này suy ra từ I, p. 54, công thức (2) đối với biểu đồ thứ nhất, và là hệ quả ngay lập tức của các định nghĩa đối với biểu đồ thứ hai. Điều này kéo theo rằng với mỗi cặp $(\mathscr{F},\mathscr{G})$ các bó trên B và mỗi cặp $(T,U)$ các không gian étalé trên B, các ánh xạ $\varphi \mapsto E(\varphi )$ và $f\mapsto \mathscr{S}(f)$ đã xét ở trên là song ánh.

Các kết quả này cho phép suy ra một mệnh đề về các không gian étalé trên B từ một mệnh đề về các bó trên B, và ngược lại.

### 7. Ảnh trực tiếp và ảnh ngược của một bó

Cho A và B là các không gian tôpô và $u: A\rightarrow B$ là một ánh xạ liên tục.

Cho $\mathscr{F}= (\mathscr{F}(U), f_{UV})$ là một tiền bó trên A. Ta định nghĩa một tiền bó $\mathscr{F}'$ trên B như sau: với mỗi tập hợp mở U của B, đặt $\mathscr{F}'(U) =\mathscr{F}(\overset{-1}{u}(U))$ và với mỗi cặp $(U,V)$ các tập hợp mở của B sao cho U $\subset V$, đặt $f'_{UV}=f_{\overset{-1}{u}(U)\overset{-1}{u}(V)}$. Khi đó $(\mathscr{F}'(U), f'_{UV})$ là một tiền bó trên B. Nó được ký hiệu bởi $u_*(\mathscr{F})$ và được gọi là tiền bó ảnh trực tiếp của tiền bó $\mathscr{F}$ bởi ánh xạ $u$.

Nếu $(U_i)_{i\in I}$ là một họ các tập hợp mở của B, ta có $\overset{-1}{u}(\bigcup_{i\in I}U_i) =$ $\bigcup_{i\in I}\overset{-1}{u}(U_i)$ và $\overset{-1}{u}(\bigcap_{i\in I}U_i) =\bigcap_{i\in I}\overset{-1}{u}(U_i)$ (E, II, p. 25, Mệnh đề 3 và 4). Suy ra ngay rằng, nếu $\mathscr{F}$ có tính chất $(F_1)$ (resp. $(F_2)$) của các bó (I, p. 43), thì $u_*(\mathscr{F})$ cũng có tính chất đó. Do đó, ảnh trực tiếp của một bó là một bó.

Cho $\mathscr{F}_1$ và $\mathscr{F}_2$ là các tiền bó trên A và $\varphi :\mathscr{F}_1\rightarrow \mathscr{F}_2$ là một cấu xạ tiền bó. Khi đó tồn tại duy nhất một cấu xạ tiền bó $u_*\varphi :u_*\mathscr{F}_1\rightarrow u_*\mathscr{F}_2$ sao cho với mỗi tập hợp mở U của B, ánh xạ $(u_*\varphi )(U): (u_*\mathscr{F}_1)(U)\rightarrow (u_*\mathscr{F}_2)(U)$ là ánh xạ $\varphi (\overset{-1}{u}(U)):\mathscr{F}_1(\overset{-1}{u}(U))\rightarrow \mathscr{F}_2(\overset{-1}{u}(U))$. Nếu $\mathscr{F}_3$ là một tiền bó trên A và $\psi :\mathscr{F}_2\rightarrow \mathscr{F}_3$ là một cấu xạ tiền bó, ta có $u_*(\psi \circ \varphi ) =u_*(\psi )\circ u_*(\varphi )$.

Cho C là một không gian tôpô và $v: B\rightarrow$ C là một ánh xạ liên tục. Nếu $\mathscr{F}$ là một tiền bó trên A, các tiền bó $v_*(u_*(\mathscr{F}))$ và $(v\circ u)_*(\mathscr{F})$ trùng nhau. Nếu $\varphi :\mathscr{F}_1\rightarrow \mathscr{F}_2$ là một cấu xạ tiền bó trên A, ta có đẳng thức $v_*(u_*(\varphi )) = (v\circ u)_*(\varphi )$.

#### Ví dụ 1 {#ta-i-s3-n7-exa-1 .statement tag=01OE}

Cho B là một không gian tôpô, A là một không gian con của B và $\mathscr{F}= (\mathscr{F}(U), f_{UV})$ là một tiền bó trên A. Gọi $i: A\rightarrow B$ là đơn ánh chính tắc. Khi đó ta có $i_*(\mathscr{F}) = (\mathscr{F}'(U), f'_{UV})$, trong đó với mỗi tập hợp mở U của B$,\mathscr{F}'(U) =\mathscr{F}(U\cap A)$, và với mỗi cặp $(U,V)$ các tập hợp mở của B sao cho $U\subset V,f'_{UV}=f_{(U\cap A)(V\cap A)}$.

Bây giờ cho $\mathscr{G}$ là một tiền bó trên B. Ảnh ngược của tiền bó $\mathscr{G}$ qua $u$ được định nghĩa là, và được ký hiệu bởi $u^*(\mathscr{G})$, bó $\mathscr{C}_B(A; E_{\mathscr{G}})$ trên A của các cấu xạ B với giá trị trong không gian B $E_{\mathscr{G}}($I, p. 45, ví dụ 4). Nó đẳng cấu chính tắc với bó trên A của các mặt cắt của không gian A étalé $A\times_BE_{\mathscr{G}}$ (I, p. 9, mệnh đề 3). Từ đó suy ra (I, p. 52, ví dụ 2) một đẳng cấu chính tắc $\varphi$ của không gian étalé liên kết với $u^*(\mathscr{G})$ lên không gian A $A\times_BE_{\mathscr{G}}$. Nếu hơn nữa $\mathscr{G}$ là một bó, thì với mọi điểm $a$ của A tồn tại một song ánh chính tắc $\psi_a:u^*(\mathscr{G})_a\rightarrow \mathscr{G}_{u(a)}:$ với mọi lân cận mở U của $a$ trong A và mọi cấu xạ B $f: U\rightarrow E_{\mathscr{G}}$, ta có

$$
\varphi ([U, f, a]) = (a, f(a)),\psi_a([U, f, a]) =f(a)
$$

Cho $\mathscr{G}_1$ và $\mathscr{G}_2$ là các tiền bó trên B và cho $\varphi :\mathscr{G}_1\rightarrow \mathscr{G}_2$ là một cấu xạ của các tiền bó. Bằng phép đổi cơ sở của cấu xạ của các không gian B étalé $E(\varphi ): E_{\mathscr{G}_1}\rightarrow E_{\mathscr{G}_2}$ ta thu được một cấu xạ của các không gian A étalé $A\times_BE_{\mathscr{G}_1}\rightarrow A\times_BE_{\mathscr{G}_2}$, do đó một cấu xạ của các bó trên A$,u^*(\varphi ):u^*(\mathscr{G}_1)\rightarrow u^*(\mathscr{G}_2)$. Cho $\mathscr{G}_3$ là một tiền bó trên B và cho $\psi :\mathscr{G}_2\rightarrow \mathscr{G}_3$ là một cấu xạ của các tiền bó. Khi đó có đẳng thức $u^*(\psi \circ \varphi ) =u^*(\psi )\circ u^*(\varphi )$.

Cho C là một không gian tôpô và cho $v: B\rightarrow$ C là một ánh xạ liên tục. Nếu $\mathscr{G}$ là một tiền bó trên C, các bó $u^*(v^*(\mathscr{G}))$ và $(v\circ u)^*(\mathscr{G})$ được đồng nhất một cách chính tắc (I, p. 5). Nếu $\varphi :\mathscr{G}_1\rightarrow \mathscr{G}_2$ là một cấu xạ của các tiền bó trên C, hơn nữa có $u^*(v^*(\varphi )) = (v\circ u)^*(\varphi )$.

#### Nhận xét {#ta-i-s3-n7-rem-1 .statement tag=01OF}

Cấu xạ chính tắc $\sigma_{\mathscr{G}}:\mathscr{G}\rightarrow \widetilde{\mathscr{G}}$ của I, p. 53 tương ứng, theo ngôn ngữ của các không gian étalé, với đẳng cấu $j_{\mathscr{G}}$ của mệnh đề 2 của I, p. 53. Suy ra rằng $u^*(\sigma_{\mathscr{G}})$ là một đẳng cấu. Đặc biệt, nếu A = B và $u=$ Id$_A$, tiền bó $u^*(\mathscr{F})$ là bó $\widetilde{\mathscr{F}}$.

#### Ví dụ 2 {#ta-i-s3-n7-exa-2 .statement tag=01OG}

Cho B là một không gian tôpô và A là một không gian con của B. Gọi $i: A\rightarrow B$ là đơn ánh chính tắc. Với mọi bó $\mathscr{G}$ trên B, ký hiệu $\mathscr{G}_A$ là bó $i^*(\mathscr{G})$, và nói rằng $\mathscr{G}_A$ là bó trên A cảm sinh bởi bó $\mathscr{G}$. Bó $\mathscr{G}_A$ được đồng nhất với bó $\mathscr{S}(A; (E_{\mathscr{G}})_A)$ của các mặt cắt của không gian A étalé cảm sinh bởi $E_{\mathscr{G}}$ trên A.

Giả sử rằng A là một không gian con mở của B, và cho $\mathscr{G}$ là một bó trên B. Theo định nghĩa, bó $\mathscr{G}_A$ là bó $\widetilde{\mathscr{G}}|A$ suy ra từ $\widetilde{\mathscr{G}}$ bằng phép hạn chế vào tập hợp mở A (I, p. 43). Cho $\sigma_{\mathscr{G}}:\mathscr{G}\rightarrow \widetilde{\mathscr{G}}$ là đẳng cấu chính tắc (I, p. 55, hệ quả 1). Khi đó $\sigma_{\mathscr{G}}|A$ là một đẳng cấu, được gọi là chính tắc, của bó $\mathscr{G}|A$ lên bó $\mathscr{G}_A$, được gọi là đẳng cấu chính tắc của $\mathscr{G}|A$ lên $\mathscr{G}_A$.

### 8. Các đồng cấu $\alpha \mathbf{e}\mathbf{t}\beta$ ; phép nối

Cho A và B là các không gian tôpô và $u: A\rightarrow B$ là một ánh xạ liên tục. Cho $\mathscr{G}$ là một tiền bó trên B. Theo định nghĩa của ảnh trực tiếp của các tiền bó, một tiết diện của bó $u_*u^*\mathscr{G}$ trên một tập mở U của B là một tiết diện của bó $u^*\mathscr{G}$ trên tập mở $\overset{-1}{u}(U)$ của A, tức là, một cấu xạ B $\overset{-1}{u}(U)\rightarrow E_{\mathscr{G}}$. Do đó ta định nghĩa một cấu xạ bó $\widetilde{\mathscr{G}}\rightarrow u_*u^*\mathscr{G}$ bằng cách gắn với tiết diện $s$ của $E_{\mathscr{G}}$ trên một tập mở U của B tiết diện $s\circ u$ của $E_{\mathscr{G}}$ trên $\overset{-1}{u}(U)$. Hợp thành của cấu xạ này với cấu xạ chính tắc $\sigma_{\mathscr{G}}:\mathscr{G}\rightarrow \widetilde{\mathscr{G}}$ (I, p. 53) là một cấu xạ tiền bó $\mathscr{G}\rightarrow u_*u^*\mathscr{G}$ sẽ được ký hiệu là $\beta_{\mathscr{G}}^u$, hoặc đơn giản là $\beta_{\mathscr{G}}$ nếu không có sự nhập nhằng về ánh xạ $u$.

#### Nhận xét 1 {#ta-i-s3-n8-rem-1 .statement tag=01OH}

Cho A, B, C là các không gian tôpô, cho $u: A\rightarrow B,v: B\rightarrow C$ là các ánh xạ liên tục; đặt $w=v\circ u$. Cho $\mathscr{G}$ là một tiền bó trên C.

Cho U là một tập mở của C và $s$ là một tiết diện của $E_{\mathscr{G}}$ trên U. Khi đó $\beta_{\mathscr{G}}^v(s)$ là tiết diện $s\circ v$ của $E_{\mathscr{G}}$ trên $\overset{-1}{v}(U)$, và $v_*(\beta_{v^*\mathscr{G}}^u)(\beta^v_{\mathscr{G}}(s))$ là tiết diện $s\circ v\circ u=s\circ w$ của $E_{\mathscr{G}}$ trên $\overset{-1}{u}(\overset{-1}{v}(U)) =\overset{-1}{w}(U)$.

Suy ra rằng $\beta_{\mathscr{G}}^w=v_*(\beta_{v^*\mathscr{G}}^u)\circ \beta_{\mathscr{G}}^v$.

#### Nhận xét 2 {#ta-i-s3-n8-rem-2 .statement tag=01OI}

Nếu $\gamma :\mathscr{G}_1\rightarrow \mathscr{G}_2$ là một cấu xạ tiền bó trên B, các cấu xạ tiền bó $\beta_{\mathscr{G}_2}\circ \gamma$ và $u_*u^*(\gamma )\circ \beta_{\mathscr{G}_1}$ là bằng nhau. Thật vậy, nếu V là một tập mở của B và $s\in \mathscr{G}_1(V),\beta_{\mathscr{G}_1}(s)$ là tiết diện $t$ của $A\times_BE_{\mathscr{G}_1}$ trên $\overset{-1}{u}(V)$, được xác định bởi $x\mapsto (x,[V, s, u(x)])$. Ảnh của $t$ qua $u^*(\gamma )$ do đó là tiết diện của $A\times_BE_{\mathscr{G}_2}$ trên $\overset{-1}{u}(V)$ được cho bởi $x\mapsto (x,[V, \gamma (s), u(x)])$. Do đó quả thực $u_*u^*(\gamma )\circ \beta_{\mathscr{G}_1}(s) =\beta_{\mathscr{G}_2}(\gamma (s))$.

#### Mệnh đề 4 {#ta-i-s3-prop-4 .statement tag=01OJ}

Cho A và B là các không gian tôpô, $u: A\rightarrow B$ là một ánh xạ liên tục, $\mathscr{G}$ là một tiền bó trên B$,\mathscr{F}$ là một bó trên A.

Với mọi cấu xạ tiền bó $\varphi :\mathscr{G}\rightarrow u_*\mathscr{F}$, tồn tại duy nhất một cấu xạ bó $\psi :u^*(\mathscr{G})\rightarrow \mathscr{F}$ sao cho $\varphi =u_*(\psi )\circ \beta_{\mathscr{G}}$.

Nói cách khác, ánh xạ chính tắc

Mor($u^*(\mathscr{G}),\mathscr{F}$)$\rightarrow$ Mor($\mathscr{G}, u_*(\mathscr{F})$)$,\psi \mapsto u_*(\psi )\circ \beta_{\mathscr{G}}$

là một song ánh.

Với ký hiệu của mệnh đề 4, đôi khi người ta ký hiệu $\psi =\varphi^{\sharp}$ và $\varphi =\psi^{\flat}$.

Ta hãy chứng minh mệnh đề 4. Theo nhận xét 2 áp dụng cho cấu xạ $\sigma_{\mathscr{G}}:\mathscr{G}\rightarrow \widetilde{\mathscr{G}}$, cấu xạ $\beta_{\mathscr{G}}$ bằng hợp thành

$$
u_*(u^*(\sigma_{\mathscr{G}})^{-1})\circ \beta_{\widetilde{\mathscr{G}}}\circ \sigma_{\mathscr{G}}
$$

trong đó $u^*(\sigma_{\mathscr{G}}):u^*(\mathscr{G})\rightarrow u^*(\widetilde{\mathscr{G}})$ là đẳng cấu chính tắc của nhận xét trong I, p. 58. Gọi $\widetilde{\varphi}:\widetilde{\mathscr{G}}\rightarrow u_*\mathscr{F}$ là cấu xạ bó duy nhất sao cho $\widetilde{\varphi}\circ \sigma_{\mathscr{G}}=\varphi ($I, p. 54, mệnh đề 3). Khi đó chỉ cần chứng minh rằng tồn tại một cấu xạ bó duy nhất $\widetilde{\psi}:u^*(\mathscr{G})\rightarrow \mathscr{F}$ sao cho $u_*(\widetilde{\psi})\circ \beta_{\mathscr{G}}=\widetilde{\varphi}$.

Ta có thể do đó giả sử rằng $\mathscr{G}$ là một bó. Để một cấu xạ bó $\psi :u^*(\mathscr{G})\rightarrow \mathscr{F}$ thỏa mãn kết luận của mệnh đề 4, điều kiện cần và đủ là với mọi tập mở V của B và mọi tiết diện $t$ của $E_{\mathscr{G}}$ trên V, ta có

$$
\varphi_V(t) =\psi_{\overset{-1}{u}(V)}(t\circ u|\overset{-1}{u}(V)) \tag{6}
$$

Gọi $U_0$ là một tập mở của A và $s_0$ là một phần tử của $u^*(\mathscr{G})(U_0)$, nói cách khác là một cấu xạ B từ $U_0$ vào $E_{\mathscr{G}}$. Gọi $S(U_0, s_0)$ là tập hợp các bộ ba $(U,V, t)$ trong đó U là một tập mở của A được chứa trong $U_0$, V là một tập mở của B sao cho $u(U)\subset V$, và $t$ là một tiết diện của $E_{\mathscr{G}}$ trên V sao cho ta có

$$
t\circ u|U =s_0|U \tag{7}
$$

Nếu $U_1$ và $U_2$ là các tập mở của A với $U_1\subset U_2$, ta ký hiệu $f_{U_1U_2}$ là ánh xạ hạn chế $\mathscr{F}(U_2)\rightarrow \mathscr{F}(U_1)$. Với mọi $(U,V, t)\in S(U_0, s_0)$, ta có quan hệ

$$
f_{UU_0}(\psi_{U_0}(s_0)) =\psi_U(s_0|U)
$$

$$
=\psi_U(t\circ u|U)
$$

$$
=f_{U\overset{-1}{u}(V)}(\psi_{\overset{-1}{u}(V)}(t\circ u|\overset{-1}{u}(V)))
$$

Do đó, nếu $\psi :u^*(\mathscr{G})\rightarrow \mathscr{F}$ thỏa mãn (6), ta có

$$
f_{UU_0}(\psi_{U_0}(s_0)) =f_{U\overset{-1}{u}(V)}(\varphi_V(t)) \tag{8}
$$

Ta hãy chứng minh rằng, với mọi điểm $a$ của $U_0$, tồn tại một bộ ba $(U,V, t)\in S(U_0, s_0)$ sao cho $a\in U$. Thật vậy, cho $a$ là một điểm của $U_0$. Tồn tại một lân cận mở V của B chứa $u(a)$ và một tiết diện $t$ của không gian étale $E_{\mathscr{G}}$ trên V sao cho $t(u(a)) =s_0(a)$ (I, p. 33, mệnh đề 9). Đặt $U_1=\overset{-1}{u}(V)\cap U_0$. Các tiết diện $s_0|U_1$ và $t\circ u|U_1$ của không gian étale $U_1$ $E_{\mathscr{G}}\times_BU_1$ trùng nhau tại điểm $a$. Theo mệnh đề 11, b) của I, p. 34, tập hợp các điểm tại đó chúng trùng nhau là một tập mở U của $U_1$ chứa $a$. Khi đó bộ ba $(U,V, t)$ thuộc $S(U_0, s_0)$.

Công thức (8) và tính chất $(F_1)$ của các bó (I, p. 43) suy ra tính duy nhất của $\psi$.

Cho $(U,V, t)$ và $(U',V', t')$ là các phần tử của $S(U_0, s_0)$. Theo quan hệ (7), các hạn chế của $t$ và $t'$ lên $u(U\cap U')$ trùng nhau. Theo Mệnh đề 11, b) của I, p. 34, tồn tại một tập hợp mở W của B sao cho $u(U\cap U')\subset$ $W\subset V\cap V'$ và $t|W =t'|W$. Do đó

$$
f_{\overset{-1}{u}(W)\overset{-1}{u}(V)}(\varphi_V(t)) =\varphi_W(t|W) =\varphi_W(t'|W) =f_{\overset{-1}{u}(W)\overset{-1}{u}(V')}(\varphi_{V'}(t'))
$$

do đó

$$
f_{(U\cap U')\overset{-1}{u}(V)}(\varphi_V(t)) =f_{(U\cap U')\overset{-1}{u}(V')}(\varphi_{V'}(t')) \tag{9}
$$

Theo các tính chất $(F_1)$ và $(F_2)$ của bó $\mathscr{F}$, tồn tại một phần tử duy nhất $s'$ của $\mathscr{F}(U_0)$ sao cho với mọi bộ ba $(U,V, t)$ của $S(U_0, s_0)$, ta có:

$$
f_{UU_0}(s') =f_{U\overset{-1}{u}(V)}(\varphi_V(t)) \tag{10}
$$

Ta ký hiệu phần tử này là $\psi_{U_0}(s_0)$.

Cho $U_1$ là một tập hợp mở được chứa trong $U_0$ và cho $s_1=s_0|U_1$. Nếu $(U,V, t)\in$ $S(U_1, s_1)$, thì U là một tập hợp mở được chứa trong $U_0$ và $t\circ u|U =s_1|U =s_0|U$, do đó $(U, v, t)\in S(U_0, s_0)$ và quan hệ (10) suy ra rằng

$$
f_{UU_1}(f_{U_1U_0}(\psi_{U_0}(s_0))) =f_{UU_0}(\psi_{U_0}(s_0)) =f_{U\overset{-1}{u}(V)}(\varphi_V(t))
$$

Theo định nghĩa của $\psi_{U_1}(s_1)$, do đó ta có $\psi_{U_1}(s_1) =f_{U_1U_0}(\psi_{U_0}(s_0))$. Điều này chứng minh rằng họ $\psi = (\psi_U)$ là một cấu xạ của các bó từ $u^*(\mathscr{G})$ vào $\mathscr{F}$.

Ta hãy chứng minh rằng $\psi$ thỏa mãn quan hệ (6). Khi đó, cho V là một tập hợp mở của B và cho $t$ là một tiết diện của $E_{\mathscr{G}}$ trên V. Nếu U = $\overset{-1}{u}(V)$ và nếu $s=t\circ u|U$, bộ ba $(U,V, t)$ thuộc $S(U, s)$ và quan hệ (6) là một hệ quả ngay lập tức của quan hệ (10), áp dụng cho $U = U_0$.

#### Mệnh đề 5 {#ta-i-s3-prop-5 .statement tag=01OK}

Cho A và B là các không gian tôpô và cho $u: A\rightarrow B$ là một ánh xạ liên tục.

a) Cho $\mathscr{G}_1$ và $\mathscr{G}_2$ là các tiền bó trên B và cho $\gamma :\mathscr{G}_1\rightarrow \mathscr{G}_2$ là một cấu xạ của các tiền bó. Hơn nữa, cho $\mathscr{F}$ là một bó trên A và $\varphi :\mathscr{G}_2\rightarrow u_*\mathscr{F}$ là một cấu xạ của các tiền bó. Ta có đẳng thức

$$
(\varphi \circ \gamma )^{\sharp}=\varphi^{\sharp}\circ u^*(\gamma ) \tag{11}
$$

b) Cho $\mathscr{F}_1,\mathscr{F}_2$ là các bó trên A và cho $\mathscr{G}$ là một tiền bó trên B. Cho $\varphi :\mathscr{F}_1\rightarrow \mathscr{F}_2$ là một cấu xạ của các bó và cho $\gamma :\mathscr{G}\rightarrow$ $u_*\mathscr{F}_1$ là một cấu xạ của các tiền bó. Ta có quan hệ

$$
(u_*(\varphi )\circ \gamma )^{\sharp}=\varphi \circ \gamma^{\sharp}
$$

a) Theo định nghĩa của $\varphi^{\sharp}$ và Nhận xét 2 của I, p. 60, ta có

$$
\varphi \circ \gamma =u_*(\varphi^{\sharp})\circ \beta_{\mathscr{G}_2}\circ \gamma =u_*(\varphi^{\sharp})\circ u_*u^*(\gamma )\circ \beta_{\mathscr{G}_1}
$$

Do đó, $\varphi \circ \gamma =u_*(\varphi^{\sharp}\circ u^*(\gamma ))\circ \beta_{\mathscr{G}_1}$, do đó quan hệ (11).

b) Theo định nghĩa của $\gamma^{\sharp}$, ta có

$$
u_*(\varphi )\circ \gamma =u_*(\varphi )\circ u_*(\gamma^{\sharp})\circ \beta_{\mathscr{G}}=u_*(\varphi \circ \gamma^{\sharp})\circ \beta_{\mathscr{G}}
$$

do đó thu được quan hệ đã nêu, xét đến định nghĩa của $(u_*(\varphi )\circ \gamma )^{\sharp}$.

Đặt $\alpha_{\mathscr{F}}$ = Id$^{\sharp}_{u_*(\mathscr{F})}$; đó là cấu xạ bó duy nhất $\rho :u^*(u_*(\mathscr{F}))\rightarrow \mathscr{F}$ sao cho

Id$_{u_*(\mathscr{F})}=u_*(\rho )\circ \beta_{u_*(\mathscr{F})}$.

Quan hệ (11), áp dụng cho $\mathscr{G}_2=u_*(\mathscr{F})$ và cấu xạ $\varphi =$ Id$_{u_*(\mathscr{F})}$, cho với mọi cấu xạ bó giả $\gamma :\mathscr{G}\rightarrow u_*(\mathscr{F})$ phân tích

$$
\gamma^{\sharp}=\alpha_{\mathscr{F}}\circ u^*(\gamma )
$$

Từ Mệnh đề 4 suy ra rằng với mọi cấu xạ bó $\psi$ của $u^*(\mathscr{G})$ vào $\mathscr{F},\psi^{\flat}$ là cấu xạ duy nhất $\varphi :\mathscr{G}\rightarrow u_*(\mathscr{F})$ sao cho $\psi =\alpha_{\mathscr{F}}\circ u^*(\varphi )$.

#### Ví dụ 1 {#ta-i-s3-n8-exa-1 .statement tag=01OL}

Xét một không gian tôpô B, một không gian con A của B, và ký hiệu $i: A\rightarrow B$ là đơn ánh chính tắc. Cho $(E, p)$ và $(E', p')$ là các B-không gian. Lấy $\mathscr{G}$ là bó $\mathscr{M}$or$_B(E; E')$ (I, p. 45, ví dụ 4) và $\mathscr{F}$ là bó $\mathscr{M}$or$_A(E_A; E'_A)$. Với mọi tập hợp mở V của B và mọi V-cấu xạ $f: E_V\rightarrow E'_V$, đặt $\varphi_V(f) =f_{V\cap A}$, trong đó $f_{V\cap A}$ là $(V\cap A)$-cấu xạ của $E_{V\cap A}$ vào $E'_{V\cap A}$ cảm sinh bởi $f$. Họ $\varphi = (\varphi_V)$ thu được là một cấu xạ bó của $\mathscr{G}$ vào $i_*\mathscr{F}$. Theo Mệnh đề 4, tồn tại một cấu xạ bó duy nhất $\psi :\mathscr{M}$or$_B(E; E')_A\rightarrow \mathscr{M}$or$_A(E_A; E'_A)$ sao cho

$$
\psi_{V\cap A}(\sigma_{\mathscr{G}}(V, f)|V\cap A) =f_{V\cap A} \tag{12}
$$

với mọi tập hợp mở V của B và mọi $f\in \mathscr{C}_V(E_V; E'_V)$. Cấu xạ $\psi$ được gọi là cấu xạ chính tắc của $\mathscr{M}$or$_B(E; E')_A$ vào $\mathscr{M}$or$_A(E_A; E'_A)$.

Nếu A thu gọn thành một điểm $a$, cấu xạ này được đồng nhất với cấu xạ trên cuống tại $a$ của bó $\mathscr{M}$or$_B(E; E')$ lên tập hợp $\mathscr{C}(E_a; E'_a)$.

Bằng cách chuyển qua các bó con, cấu xạ $\psi$ cảm sinh một cấu xạ chính tắc của $\mathscr{I}$som$_B(E; E')_A$ vào $\mathscr{I}$som$_A(E_A; E'_A)$.

#### Ví dụ 2 {#ta-i-s3-n8-exa-2 .statement tag=01OM}

Cho A, B, C là các không gian tôpô và $u: A\rightarrow B$, $v: B\rightarrow C$ là các ánh xạ liên tục; đặt $w=v\circ u$. Cho E và $E'$ là các C-không gian. Cấu xạ chính tắc từ $\mathscr{M}$or$_C(E; E')_A$ vào $\mathscr{M}$or$_A(E_A; E'_A)$ là cấu xạ hợp thành của cấu xạ $\mathscr{M}$or$_C(E; E')_A\rightarrow \mathscr{M}$or$_B(E_B; E'_B)_A$ suy ra từ cấu xạ chính tắc của $\mathscr{M}$or$_C(E; E')_B$ vào $\mathscr{M}$or$_B(E_B; E'_B)$ và cấu xạ chính tắc của $\mathscr{M}$or$_B(E_B,E'_B)_A$ vào $\mathscr{M}$or$_A(E_A,E'_A)$.

### 9. Bó mềm

#### Định nghĩa 5 {#ta-i-s3-def-5 .statement tag=01ON}

Cho $p: E\rightarrow B$ là một ánh xạ étalé. Ta nói rằng ánh xạ $p$ là mềm, hay không gian B-étalé $(E, p)$ là mềm, nếu mọi tiết diện liên tục của $p$ trên một không gian con đóng của B đều mở rộng thành một tiết diện liên tục của $p$ trên B.

Cho $\mathscr{F}$ là một bó trên B. Ta nói rằng $\mathscr{F}$ là một bó mềm nếu không gian étalé liên kết với nó (I, p. 50, def. 4) là mềm.

Cho $\mathscr{F}$ là một bó trên B. Bó $\mathscr{F}$ là mềm khi và chỉ khi với mọi Z đóng trong B, mọi lân cận mở U của Z và mọi $s\in \mathscr{F}(U)$, tồn tại $t\in \mathscr{F}(B)$ và một lân cận mở V của Z được chứa trong U sao cho $s|V =t|V$.

Nếu $\mathscr{F}$ là một bó mềm, thì $\mathscr{F}(B)$ khác rỗng: thực vậy, tiết diện duy nhất của không gian étalé $E_{\mathscr{F}}$ liên kết với $\mathscr{F}$ trên $\emptyset$ mở rộng thành một tiết diện liên tục của $E_{\mathscr{F}}$ trên B.

Cho $p: E\rightarrow B$ là một ánh xạ étalé và A là một không gian con đóng của B. Nếu $p$ mềm, ánh xạ $p_A:\overset{-1}{p}(A)\rightarrow A$ mềm. Tương đương, nếu $\mathscr{F}$ là một bó mềm trên B, thì bó cảm sinh trên một không gian con đóng A là mềm.

#### Mệnh đề 6 {#ta-i-s3-prop-6 .statement tag=01OO}

Cho B là một không gian tôpô, $\mathscr{F}$ là một bó trên B và $(A_i)_{i\in I}$ là một phủ đóng hữu hạn địa phương của B. Để bó $\mathscr{F}$ mềm, điều kiện cần và đủ là, với mọi $i\in I$, bó cảm sinh $\mathscr{F}_{A_i}$ là mềm.

Điều kiện này hiển nhiên là cần. Ta hãy chứng minh rằng nó là đủ. Ký hiệu $p: E\rightarrow B$ là không gian B-étalé $E_{\mathscr{F}}$ liên kết với bó $\mathscr{F}$. Cho A là một không gian con đóng của B và $s: A\rightarrow E$ là một tiết diện liên tục của $p$ trên A; ta phải chứng minh rằng $s$ có một mở rộng liên tục lên B. Với mọi tập con J của I, đặt $A_J=\bigcup_{i\in J}A_i$; tập hợp $A_J$ là đóng trong B (TG, I, p. 6, prop. 4).

Cho $\mathscr{S}$ là tập hợp các cặp $(J, t)$ trong đó J là một tập con của I và $t$ là một tiết diện liên tục của E trên $A_J$ trùng với $s$ trên $A\cap A_J$. Ta trang bị cho $\mathscr{S}$ một quan hệ có thứ tự, được ký hiệu bởi $\leqslant$, trong đó $(J, t)\leqslant (J', t')$ nếu $J\subset J'$ và $t'|A_J=t$. Với $\sigma = (J, t)\in \mathscr{S}$, ta viết $J_{\sigma}= J$ và $t_{\sigma}=t$. Ta hãy chứng minh rằng tập có thứ tự $\mathscr{S}$ là quy nạp. Cho S là một tập con được sắp thứ tự toàn phần của $\mathscr{S}$. Đặt $J =\bigcup_{\sigma\in S}J_{\sigma}$; đây là một tập con của I. Khi đó định nghĩa một tiết diện $t$ của E trên $A_J$ bằng cách đặt $t(x) =t_{\sigma}(x)$, nếu $x\in A_{J_{\sigma}}$; do đó $t|A\cap A_J=s$. Cho $j\in J$ và lấy $\sigma \in S$ sao cho $j\in J_{\sigma}$; vì $t|A_j=t_{\sigma}|A_j$, hạn chế của $t$ trên $A_j$ là liên tục. Theo TG, I, p. 19, Prop. 4, suy ra rằng $t$ là liên tục. Vậy $(J, t)$ là một phần tử của $\mathscr{S}$; theo phép dựng, nó là một cận trên của S. Điều này chứng minh rằng tập hợp $\mathscr{S}$ là quy nạp. Do đó nó có một phần tử cực đại $(J, t)$ (E, III, p. 20, th. 2).

Ta lập luận phản chứng, giả sử rằng J $= I\not$ . Cho $i$ là một phần tử của I-J. Đặt $A'= (A_i\cap A)\cup (A_i\cap A_J)$ và định nghĩa một tiết diện $s'$ của E trên $A'$ bởi:

$'s(a)$ với $a\in A_i\cap A$,

$$
s(a) =
$$

$t(a)$ với $a\in A_i\cap A_J$,

điều này có thể thực hiện được vì $s$ và $t$ trùng nhau trên $A\cap A_J$. Hơn nữa, vì $A_i\cap A$ và $A_i\cap A_J$ là các tập đóng, tiết diện $s'$ là liên tục (TG, I, p. 19, prop. 4). Theo giả thiết, tồn tại một tiết diện liên tục $s_i: A_i\rightarrow E$ mở rộng $s'$. Vì các hạn chế của $s_i$ và $t$ trên $A_J\cap A_i$ bằng nhau, tiết diện liên tục $t': A_{J\cup \{i\}}\rightarrow E$ trùng với $t$ trên $A_J$ và với $s_i$ trên $A_i$ là một tiết diện liên tục của $p$ trên $A_{J\cup \{i\}}$, mở rộng $s|A\cap A_{J\cup \{i\}}$. Khi đó ta có $(J, t)<(J\cup  \{i\}, t')$, điều này mâu thuẫn với giả thiết rằng $(J, t)$ là cực đại.

Do đó, J = I, suy ra $A_J= B$ và $t$ là một tiết diện liên tục của E trên B mở rộng $s$.

#### Hệ quả 1 {#ta-i-s3-prop-6-cor-1 .statement tag=01OP}

Cho B là một không gian paracompact, $\mathscr{F}$ là một bó trên B và $(U_i)_{i\in I}$ là một phủ mở của B. Nếu, với mọi $i\in I$, bó cảm sinh $\mathscr{F}|U_i$ là mềm, thì bó $\mathscr{F}$ là mềm.

Thực tế, tồn tại một phủ đóng hữu hạn địa phương $(F_j)_{j\in J}$ mịn hơn phủ $(U_i)_{i\in I}$ (TG, IX, p. 49, prop. 4 và p. 48, cor. 1). Do đó, với mọi $j\in J$, bó $\mathscr{F}|F_j$ là mềm và mệnh đề suy ra rằng bó $\mathscr{F}$ là mềm.

#### Hệ quả 2 {#ta-i-s3-prop-6-cor-2 .statement tag=01OQ}

Cho B là một không gian paracompact, $\mathscr{F}$ là một bó trên B và $(A_i)_{i\in I}$ là một phủ đóng hữu hạn địa phương của B. Để bó $\mathscr{F}$ là mềm, điều kiện cần và đủ là điều kiện sau được thỏa mãn:

Với mọi $i\in I$, mọi tập con đóng A của $A_i$, mọi tập mở V của B chứa A và mọi phần tử $s$ của $\mathscr{F}(V)$, tồn tại một lân cận mở U của $A_i$ trong B, một phần tử $t$ của $\mathscr{F}(U)$ và một lân cận mở W của A trong B được chứa trong $U\cap V$ sao cho $t|W =s|W$.

Giả sử bó $\mathscr{F}$ là mềm, và hãy chứng minh rằng điều kiện được thỏa mãn. Cho $i\in I$, cho A là một tập con đóng của $A_i$, cho V là một tập mở của B chứa A và cho $s$ là một phần tử của $\mathscr{F}(V)$. Đặt $s_0=\sigma_{\mathscr{F}}(s)$. Đây là một tiết diện liên tục trên V của không gian étalé $E_{\mathscr{F}}$. Vì $A_i$ đóng, A đóng trong B và $s_0|A$ mở rộng thành một tiết diện $t_0: B\rightarrow E_{\mathscr{F}}$, theo định nghĩa của một bó mềm. Các tiết diện $s_0$ và $t_0|V$ của không gian étalé trên V $E_{\mathscr{F}}\times_BV$ trùng nhau trên A, do đó trên một lân cận W của A (I, p. 34, prop. 11, b)).

Ngược lại, giả sử điều kiện của hệ quả được thỏa mãn. Theo mệnh đề 6, chỉ cần chứng minh rằng, với mọi $i\in I$, bó $\mathscr{F}_{A_i}$ là mềm. Cho A là một tập con đóng của $A_i$ và cho $s_0$ là một tiết diện của không gian étale của $\mathscr{F}|A_i$ trên A, nghĩa là một tiết diện liên tục trên A của không gian étale $E_{\mathscr{F}}$. Vì A đóng trong B và vì B là paracompact, $s_0$ mở rộng thành một tiết diện $s$ trên một lân cận V của A trong B (I, p. 37, th. 2). Theo giả thiết, tồn tại một lân cận mở U của $A_i$ trong B và một tiết diện $t$ của $E_{\mathscr{F}}$ trên U trùng với $s$ trên một lân cận của A. Hạn chế của $t$ lên $A_i$ là một tiết diện của $\mathscr{F}_{A_i}$ mở rộng $s_0$. Do đó bó $\mathscr{F}_{A_i}$ là mềm. Theo mệnh đề 6, bó $\mathscr{F}$ là mềm.

### 10. Các bó của loài cấu trúc

Giả sử đã cho một Loài cấu trúc Σ và một khái niệm về $\sigma$-cấu xạ tương đối với Loài cấu trúc này.

Cho B là một không gian tôpô.

Một tiền bó $\mathscr{F}$ trên B được gọi là có giá trị trong Loài cấu trúc Σ nếu, với mọi tập mở U của B, tập hợp $\mathscr{F}(U)$ được trang bị một cấu trúc của Loài cấu trúc Σ và nếu các ánh xạ hạn chế là các $\sigma$-cấu xạ.

Một tiền bó như vậy sẽ được gọi là một bó có giá trị trong Loài cấu trúc Σ nếu, hơn nữa, nó là một bó của các tập hợp.

Nếu $\mathscr{F}$ và $\mathscr{G}$ là các tiền bó có giá trị trong Loài cấu trúc Σ, một cấu xạ $\varphi$ được gọi là một cấu xạ của các tiền bó có giá trị trong Σ nếu, với mọi tập mở U, ánh xạ $\varphi (U)$ là một $\sigma$-cấu xạ.

Do đó người ta nói, chẳng hạn, về các bó của các nhóm, của các nhóm Abel, của các $k$-môđun (đối với một vành $k$ cố định), của các vành, của các $k$-đại số (đối với một vành giao hoán $k$ cố định).

Bó trên B của các ánh xạ có giá trị trong một nhóm (tương ứng. một nhóm Abel, tương ứng. một $k$-môđun, tương ứng. một vành, tương ứng. một $k$-đại số) được trang bị một cách tự nhiên một cấu trúc của bó các nhóm (tương ứng. của các nhóm Abel, tương ứng. của các $k$-môđun, tương ứng. của các vành, tương ứng. của các $k$-đại số). Nếu X là một đa tạp khả vi thuộc lớp $C^r$ trên $\mathbf{R}$, bó $\mathscr{C}^r(X;\mathbf{R})$ của các hàm số thuộc lớp $C^r$ là một bó các $\mathbf{R}$-đại số, và bó trên X của các tiết diện thuộc lớp $C^r$ của một bó vectơ E trên X là một bó các không gian vectơ trên $\mathbf{R}$; một toán tử vi phân xác định một cấu xạ của các bó các không gian vectơ trên $\mathbf{R}$.

Đối với các Loài cấu trúc Σ này, từ phép dựng mà chúng ta đã cho suy ra rằng bó $\widetilde{F}$ liên kết với một tiền bó $\mathscr{F}$ có giá trị trong Loài cấu trúc Σ (các nhóm, các nhóm Abel, các $k$-môđun, các vành, các $k$-đại số) là một bó có giá trị trong Loài cấu trúc này, và cấu xạ chính tắc $j_{\mathscr{F}}:\mathscr{F}\rightarrow \widetilde{\mathscr{F}}$ là một cấu xạ của các tiền bó có giá trị trong Loài cấu trúc Σ.

Chẳng hạn, bó trên B của các ánh xạ có giá trị trong một nhóm được trang bị một cách tự nhiên một cấu trúc của bó các nhóm.

Cho A và B là các không gian tôpô và cho $u: A\rightarrow B$ là một ánh xạ liên tục. Nếu $\mathscr{F}$ là một (tiền)bó trên A có giá trị trong Loài cấu trúc Σ, điều tương tự cũng đúng đối với (tiền)bó ảnh trực tiếp $u_*(\mathscr{F})$ của (tiền)bó $\mathscr{F}$ theo u.

Giả sử thêm rằng Loài cấu trúc Σ là loài các nhóm, các nhóm Abel, các $k$-môđun, các vành hoặc các $k$-đại số. Nếu $\mathscr{G}$ là một bó (tiền)bó trên B nhận giá trị trong Loài cấu trúc Σ, thì bó $u^*\mathscr{G}$ trên A, là ảnh ngược của tiền bó $\mathscr{G}$ bởi ánh xạ $u$, được trang bị một cấu trúc bó nhận giá trị trong Σ. Trong trường hợp này, các cấu xạ phép nối $\alpha$ và $\beta$ là các cấu xạ của các tiền bó nhận giá trị trong Loài cấu trúc Σ. Đặc biệt, nếu $\varphi :\mathscr{G}\rightarrow u_*\mathscr{F}$ là một cấu xạ của các tiền bó nhận giá trị trong Σ, thì điều tương tự cũng đúng với cấu xạ $\varphi^{\sharp}$; nếu $\psi :u^*(\mathscr{G})\rightarrow \mathscr{F}$ là một cấu xạ của các tiền bó nhận giá trị trong Σ, thì điều tương tự cũng đúng với cấu xạ $\psi^{\flat}$.

## BÀI TẬP {#ta-i-s3-exercises}

Xem [các bài tập của § 3](exercises/s3/).
