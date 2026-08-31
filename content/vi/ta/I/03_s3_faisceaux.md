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
content_sha256: c5ac20092f105f30484a8651bd008933b7b8e514174e430a89d07ab39796b847
translated_from: content/en-mt/ta/I/03_s3_faisceaux.md
source_lang: en-mt
translation_method: machine
source_content_sha256: 52992bda508a3c0caa17b47af125817ccd2a2bd8f51eb6448ce1d4cae22b17ce
translation_model: gpt-5.4
translation_run: translate-vi-f7047471
glossary_version: 34
glossary_terms_sha256: 3d252cd4cb381d03b8fc1cbc512c2c7f3bc816b1cc90a5be8759ac94ab48c2ed
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 3. BÓ

### 1. Bó các tập hợp

Cho B là một không gian tôpô.

#### Định nghĩa 1 {#ta-i-s3-def-1 .statement tag=01NS}

Một tiền bó trên B, tương đối với một cơ sở $\mathscr{B}$ của tôpô trên B, là một hệ xạ ảnh các tập hợp, tương đối với tập hợp chỉ số $\mathscr{B}$ được sắp thứ tự bởi quan hệ bao hàm.

Nói cách khác (E, III, p. 52), một tiền bó $\mathscr{F}$ trên B tương đối với $\mathscr{B}$ là một cặp $((\mathscr{F}(U))_{U\in\mathscr{B}},(f_{UV}))$, cũng được ký hiệu là $(\mathscr{F}(U), f_{UV})$, trong đó $((\mathscr{F}(U))_{U\in\mathscr{B}}$ là một họ các tập hợp có $\mathscr{B}$ làm tập hợp chỉ số và với mỗi cặp $(U,V)$ các phần tử của $\mathscr{B}$ sao cho $U\subset V,f_{UV}$ là một ánh xạ từ $\mathscr{F}(V)$ vào $\mathscr{F}(U)$, các ánh xạ này thỏa mãn các điều kiện sau:

(PF$_1$) Các quan hệ $U\subset V\subset W$ kéo theo $f_{UW}=f_{UV}\circ f_{VW}$;

(PF$_2$) Với mọi tập hợp mở U $\in \mathscr{B},f_{UU}$ là ánh xạ đồng nhất của

$$
\mathscr{F}(U)
$$

Một tiền bó trên B tương đối với tập hợp các tập con mở của B được gọi đơn giản là một tiền bó trên B.

Cho $\mathscr{F}= (\mathscr{F}(U), f_{UV})$ là một tiền bó trên B, tương đối với một cơ sở $\mathscr{B}$ của tôpô trên B. Cho U là một phần tử của cơ sở $\mathscr{B}$. Các phần tử của $\mathscr{F}(U)$ được gọi là các thiết diện của $\mathscr{F}$ trên U. Nếu V là một phần tử của cơ sở $\mathscr{B}$ chứa U và $s$ là một phần tử của $\mathscr{F}(V)$, thì phần tử $f_{UV}(s)$ của $\mathscr{F}(U)$ được gọi là hạn chế của $s$ trên U. Nếu không có nguy cơ nhập nhằng đối với các ánh xạ $f_{UV}$, hạn chế của $s$ trên U sẽ được ký hiệu là $s|U$.

Cho $B'$ là một tập con mở của B và $\mathscr{B}'$ là một cơ sở của tôpô trên $B'$ sao cho $\mathscr{B}'\subset \mathscr{B}$. Tiền bó trên $B'$, tương đối với $\mathscr{B}'$, suy ra từ $\mathscr{F}$ bằng hạn chế, được gọi là hạn chế của $\mathscr{F}$ lên $\mathscr{B}'$ và được ký hiệu là $\mathscr{F}|\mathscr{B}'$, tức hệ xạ ảnh $((\mathscr{F}(U))_{U\in\mathscr{B}'},(f_{UV}))$ suy ra từ $\mathscr{F}$ bằng cách hạn chế tập hợp chỉ số xuống $\mathscr{B}'$ (loc. cit.). Khi $\mathscr{F}$ là một tiền bó trên B và $\mathscr{B}'$ là tập hợp các tập con mở của $B'$, tiền bó $\mathscr{F}|\mathscr{B}'$ cũng được ký hiệu là $\mathscr{F}|B'$ và được gọi là tiền bó suy ra từ $\mathscr{F}$ bằng hạn chế lên $B'$.

#### Định nghĩa 2 {#ta-i-s3-def-2 .statement tag=01NT}

Cho $\mathscr{F}= (\mathscr{F}(U), f_{UV})$ là một tiền bó trên B. Ta nói rằng $\mathscr{F}$ là một bó trên B nếu, với mọi tập con mở U của B và mọi họ $(U_i)_{i\in I}$ các tập con mở của B, có hợp là U, các tính chất sau được thỏa mãn:

$(F_1)$ Ánh xạ $(f_{U_iU})_{i\in I}:\mathscr{F}(U)\rightarrow \prod_{i\in I}\mathscr{F}(U_i)$ là đơn ánh ;

$(F_2)$ Với mọi họ $(s_i)\in \prod_{i\in I}\mathscr{F}(U_i)$ sao cho $f_{(U_i\cap U_j)U_i}(s_i) =$

$f_{(U_i\cap U_j)U_j}(s_j)$ với mọi cặp $(i, j)\in I\times I$, tồn tại một phần tử $s$

của $\mathscr{F}(U)$ sao cho với mọi $i\in I$, ta có $f_{U_iU}(s) =s_i$.

#### Nhận xét {#ta-i-s3-n1-rem-1 .statement tag=01NU}

Cho $\mathscr{F}$ là một tiền bó trên B. Với mọi tập hợp mở U của B, $f_{\emptyset U}$ là một ánh xạ từ $\mathscr{F}(U)$ vào $\mathscr{F}(\emptyset )$, do đó $\mathscr{F}(\emptyset )$ không rỗng ngay khi tồn tại một tập hợp mở U mà $\mathscr{F}(U)$ không rỗng. Nếu $\mathscr{F}$ là một bó, thì $\mathscr{F}(\emptyset )$ là một tập hợp một phần tử; điều này thấy được bằng cách áp dụng $(F_1)$ và $(F_2)$ cho phủ của tập rỗng bởi họ rỗng ($I =\emptyset$ ).

Cho $\mathscr{F}$ là một bó trên B và cho $B'$ là một tập con mở của B; tiền bó $\mathscr{F}|B'$ suy ra từ $\mathscr{F}$ bằng hạn chế lên $B'$ là một bó, gọi là bó suy ra từ $\mathscr{F}$ bằng hạn chế lên $B'$.

### 2. Các bó con của một bó

Cho B là một không gian tôpô. Cho $\mathscr{F}= (\mathscr{F}(U), f_{UV})$ là một tiền bó trên B, đối với một cơ sở $\mathscr{B}$ của tôpô của B.

Giả sử với mọi tập hợp mở $U\in \mathscr{B}$, đã cho một tập con $\mathscr{L}(U)$ của $\mathscr{F}(U)$. Nếu ta có $f_{UV}(\mathscr{L}(V))\subset \mathscr{L}(U)$ với mọi cặp $(U,V)$ các phần tử của $\mathscr{B}$ sao cho $U\subset V$, thì cặp $\mathscr{L}= ((\mathscr{L}(U))_{U\in\mathscr{B}},(f'_{UV}))$, trong đó $f'_{UV}:\mathscr{L}(V)\rightarrow \mathscr{L}(U)$ là ánh xạ suy ra từ $f_{UV}$, là một tiền bó. Một tiền bó như vậy được gọi là một tiền bó con của $\mathscr{F}$. Vì các ánh xạ $f'_{UV}$ được xác định bởi tiền bó đã cho $\mathscr{F}$ và họ $(\mathscr{L}(U))_{U\in\mathscr{B}}$, nên người ta cũng nói, do lạm dụng ngôn ngữ, rằng họ $(\mathscr{L}(U))_{U\in\mathscr{B}}$ là một tiền bó con của $\mathscr{F}$.

Bây giờ giả sử rằng $\mathscr{F}$ là một bó trên B và cho, với mọi tập con mở U của B$,\mathscr{L}(U)$, một tập con của $\mathscr{F}(U)$. Để cho $(\mathscr{L}(U))_{U\in\mathscr{B}}$ là một tiền bó con của $\mathscr{F}$, và để cho tiền bó này là một bó, điều kiện sau đây là cần và đủ:

(F) Cho $(U_i)_{i\in I}$ là một họ các tập hợp mở của B, U là hợp của chúng, và $s$ là một

phần tử của $\mathscr{F}(U)$. Để $s$ thuộc $\mathscr{L}(U)$, điều kiện cần và

đủ là với mọi $i$ trong I$,f_{U_iU}(s)$ thuộc $\mathscr{L}(U_i)$.

Thật vậy, nếu điều kiện (F) được thỏa mãn, ta có $f_{UV}(\mathscr{L}(V))\subset \mathscr{L}(U)$ với mọi cặp $(U,V)$ các tập mở của B sao cho $U\subset V$ và các tính chất $(F_1)$ và $(F_2)$ đối với tiền bó con $(\mathscr{L}(U))$ suy ra từ các tính chất tương tự đối với bó $\mathscr{F}$. Đảo lại là ngay lập tức.

Khi điều kiện (F) được thỏa mãn, ta nói rằng $(\mathscr{L}(U))$ là một bó con của bó $\mathscr{F}$.

### 3. Ví dụ về các bó

Cho B là một không gian tôpô.

1) Các bó ánh xạ

Cho X là một tập hợp. Với mọi tập mở U của B, ký hiệu bởi $\mathscr{F}(U; X)$ tập hợp các ánh xạ từ U vào X (E, II, p. 31). Với mọi cặp $(U,V)$ các tập mở của B sao cho $U\subset V$, đặt $r_{UV}:\mathscr{F}(V; X)\rightarrow$ $\mathscr{F}(U; X)$ là ánh xạ hạn chế $f\mapsto f|U$. Hiển nhiên cặp $(\mathscr{F}(U; X), r_{UV})$ là một bó trên B. Nó được gọi là bó trên B của các ánh xạ nhận giá trị trong X, và được ký hiệu bởi $\mathscr{F}(B; X)$.

2) Các bó ánh xạ liên tục

Cho X là một không gian tôpô. Với mọi tập mở U của B, đặt $\mathscr{C}(U; X)$ là tập hợp các ánh xạ liên tục từ U vào X. Khi đó, $(\mathscr{C}(U; X))$ là một bó con của bó $\mathscr{F}(B; X)$ theo mệnh đề 4 của TG, I, p. 19. Bó nhận được như vậy được ký hiệu bởi $\mathscr{C}(B; X)$ và gọi là bó trên B của các ánh xạ liên tục nhận giá trị trong X. Trong trường hợp riêng khi X được trang bị tôpô rời rạc, bó $\mathscr{C}(B; X)$ được gọi là bó trên B của các ánh xạ địa phương hằng nhận giá trị trong X.

3) Các bó tiết diện liên tục

Cho E là một không gian tôpô và cho $p: E\rightarrow B$ là một ánh xạ liên tục. Với mọi tập mở U của B, ký hiệu bởi $\mathscr{S}(U;p)$ (hoặc $\mathscr{S}(U; E)$ khi không thể có sự nhầm lẫn) tập hợp các tiết diện liên tục của $p$ trên U. Họ $(\mathscr{S}(U;p))$ là một bó con của bó $\mathscr{C}(B; E)$. Bó nhận được như vậy được ký hiệu bởi $\mathscr{S}(B; E)$ hoặc đơn giản là $\mathscr{S}(E)$ và gọi là bó trên B của các tiết diện liên tục của B-không gian $(E, p)$. Ta sẽ thấy ở no$^o6$ dưới đây rằng mọi bó trên B đều đẳng cấu với bó trên B của các tiết diện liên tục của một B-không gian étalé.

4) Các bó cấu xạ B

Cho $(E, p)$ và $(E', p')$ là các B-không gian. Với mọi tập mở U của E, ký hiệu bởi $\mathscr{C}_B(U; E')$ tập hợp các B-cấu xạ từ $(U, p|U)$ vào $(E', p')$. Họ $(\mathscr{C}_B(U; E'))$ là một bó con của bó $\mathscr{C}(E; E')$. Bó nhận được như vậy được ký hiệu bởi $\mathscr{C}_B(E; E')$ và gọi là bó trên E của các B-cấu xạ nhận giá trị trong $(E', p')$. Khi $(E, p)$ bằng với $(B$, Id$_B)$, bó này là bó $\mathscr{S}(B; E)$ của ví dụ 3.

Với mọi tập mở U của B, đặt $\mathscr{M}(U)$ là tập hợp các U-cấu xạ

từ $\overset{-1}{p}(U)$ vào $(^-{p'}^1)(U)$. Với mọi cặp $(U,V)$ các tập mở của B sao cho $U\subset V$, đặt $m_{UV}:\mathscr{M}(V)\rightarrow \mathscr{M}(U)$ là ánh xạ mà với một V-cấu xạ

$f:\overset{-1}{p}(V)\rightarrow (^-{p'}^1)(V)$ nó gán U-cấu xạ từ $\overset{-1}{p}(U)$ vào $(^-{p'}^1)(U)$ suy ra từ $f$ bằng cách chuyển qua các tập con. Khi đó $(\mathscr{M}(U), m_{UV})$ là một bó trên B. Nó được ký hiệu bởi $\mathscr{M}$or$_B(E; E')$ và được gọi là bó trên B của các B-cấu xạ từ $(E, p)$ vào $(E', p')$.

Với mọi tập mở U của B, gọi $\mathscr{I}$s(U) là tập con của $\mathscr{M}(U)$

gồm các U-đẳng cấu của $\overset{-1}{p}(U)$ vào $(^-{p'}^1)(U)$. Họ $(\mathscr{I}$s(U)) là một bó con của bó $\mathscr{M}$or$_B(E; E')$ các cấu xạ từ $(E, p)$ vào $(E', p')$. Bó do đó thu được được ký hiệu là $\mathscr{I}$som$_B(E; E')$ và được gọi là bó trên B các B-đẳng cấu từ $(E, p)$ vào $(E', p')$.

5) Các bó các ánh xạ lớp $C^r$

Cho X và Y là các đa tạp lớp $C^r$ trên một trường K (các quy ước liên quan đến K và $r$ là những quy ước của VAR, R). Với mọi tập mở U của X, gọi $\mathscr{C}^r(U; Y)$ là tập hợp các cấu xạ lớp $C^r$ từ U vào Y. Họ $(\mathscr{C}^r(U; Y))$ là một bó con của bó $\mathscr{C}(X; Y)$. Bó do đó thu được được ký hiệu là $\mathscr{C}^r(X; Y)$ và được gọi là bó trên X của các ánh xạ lớp $C^r$ nhận giá trị trong Y (xem VAR, R, 5.4.2).

6) Các bó các không gian con

Nếu U và V là các tập mở của B sao cho $U\subset V$, ký hiệu bởi $i_{UV}:\mathfrak{P}(V)\rightarrow$ $\mathfrak{P}(U)$ ánh xạ gán cho mỗi tập con A của V tập hợp $A\cap U$. Cặp $(\mathfrak{P}(U), i_{UV})$ là một bó, gọi là bó các không gian con của B và được ký hiệu là $\mathfrak{P}(B)$. Thật vậy, nếu X ký hiệu tập hợp $\{0; 1\}$, thì ánh xạ gán cho mỗi tập con A của U hàm đặc số của nó $\varphi^U_A: U\rightarrow X$ là một song ánh từ $\mathfrak{P}(U)$ lên $\mathscr{F}(U; X)$ (E, III, p. 38) ; hơn nữa, nếu U và V là các tập mở sao cho $U\subset V$, thì với mọi tập con A của V$,\varphi^U_{A\cap U}$ là hạn chế trên U của $\varphi^V_A$ để cho $\mathfrak{P}(B)$ được đồng nhất với bó trên B của các ánh xạ nhận giá trị trong X.

Gọi, với mọi tập mở U của B$,\mathscr{L}(U)$ là một tập con của $\mathfrak{P}(U)$. Để $(\mathscr{L}(U))$ là một bó con của $\mathfrak{P}(B)$, điều kiện sau đây là cần và đủ:

$(F')$ Cho $(U_i)_{i\in I}$ là một họ các tập mở của B, U là hợp của chúng, và A là một

tập con của U ; để A thuộc $\mathscr{L}(U)$, điều kiện cần và

đủ là với mọi $i$ trong I, $A\cap U_i$ thuộc $\mathscr{L}(U_i)$.

Ví dụ, nếu $\mathscr{L}(U)$ là tập hợp các tập con đóng của U, thì điều kiện $(F')$ được thỏa mãn.

7) Tích của các bó

Cho $\mathscr{B}$ là một cơ sở của tôpô của B và I là một tập hợp. Với mọi $i\in I$, cho $\mathscr{F}_i= (\mathscr{F}_i(U), f_{i,UV})$ là một tiền bó trên B đối với cơ sở $\mathscr{B}$. Với mọi tập mở $U\in \mathscr{B}$, đặt $\mathscr{F}(U) =\prod_{i\in I}\mathscr{F}_i(U)$, và với mọi cặp $(U,V)$ gồm các phần tử của $\mathscr{B}$ sao cho $U\subset V$, ký hiệu bởi $f_{UV}$ ánh xạ $(f_{i,UV})_{i\in I}:\mathscr{F}(V)\rightarrow \mathscr{F}(U)$. Khi đó $(\mathscr{F}(U), f_{UV})$ là một tiền bó trên B đối với $\mathscr{B}$, gọi là tiền bó tích của họ $(\mathscr{F}_i)$ và được ký hiệu $\prod_{i\in I}\mathscr{F}_i$. Nó là một bó nếu với mọi $i\in I,\mathscr{F}_i$ là một bó.

### 4. Cấu xạ của các tiền bó

#### Định nghĩa 3 {#ta-i-s3-def-3 .statement tag=01NV}

Cho B là một không gian tôpô, $\mathscr{B}$ một cơ sở của tôpô của B$,\mathscr{F}= (\mathscr{F}(U), f_{UV})$ và $\mathscr{G}= (\mathscr{G}(U), g_{UV})$ là các tiền bó trên B đối với $\mathscr{B}$. Một cấu xạ của các tiền bó từ $\mathscr{F}$ đến $\mathscr{G}$ được gọi là một hệ xạ ảnh các ánh xạ từ $\mathscr{F}$ đến $\mathscr{G}$.

Nói cách khác (E, III, p. 54), một cấu xạ của các tiền bó từ $\mathscr{F}$ đến $\mathscr{G}$ là một họ $(\varphi_U)_{U\in\mathscr{B}}$ sao cho :

(MPF$_1$) Với mọi tập mở U thuộc $\mathscr{B},\varphi_U$ là một ánh xạ

từ $\mathscr{F}(U)$ vào $\mathscr{G}(U)$ ;

(MPF$_2$) Với mọi cặp $(U,V)$ gồm các tập mở thuộc $\mathscr{B}$ sao cho

$U\subset V$, ta có $\varphi_U\circ f_{UV}=g_{UV}\circ \varphi_V$.

Khi $\mathscr{F}$ và $\mathscr{G}$ là các bó, một cấu xạ của các tiền bó từ $\mathscr{F}$ đến $\mathscr{G}$ cũng được gọi là một cấu xạ của các bó. Nếu $\mathscr{F}$ và $\mathscr{G}$ là các tiền bó trên B đối với $\mathscr{B}$, các cấu xạ của các tiền bó từ $\mathscr{F}$ đến $\mathscr{G}$ tạo thành một tập hợp ký hiệu là Mor($\mathscr{F};\mathscr{G}$). Thay vì nói : “cho $\varphi$ là một cấu xạ của các tiền bó từ $\mathscr{F}$ đến $\mathscr{G}$”, người ta thường sẽ nói “cho $\varphi :\mathscr{F}\rightarrow \mathscr{G}$ là một cấu xạ của các tiền bó”.

Cho $\mathscr{F},\mathscr{G},\mathscr{H}$ là các tiền bó trên B đối với $\mathscr{B}$ và cho $\varphi :\mathscr{F}\rightarrow \mathscr{G}$, $\psi :\mathscr{G}\rightarrow \mathscr{H}$ là các cấu xạ của các tiền bó. Họ $(\psi_U\circ \varphi_U)_{U\in\mathscr{B}}$ là một cấu xạ của các tiền bó từ $\mathscr{F}$ vào $\mathscr{H}$, được ký hiệu bởi $\psi \circ \varphi$. Họ (Id$_{\mathscr{F}(U)}$)$_{U\in\mathscr{B}}$ là một cấu xạ của các tiền bó từ $\mathscr{F}$ vào chính nó, được ký hiệu bởi Id$_{\mathscr{F}}$.

Để một cấu xạ của các tiền bó $\varphi = (\varphi_U):\mathscr{F}\rightarrow \mathscr{G}$ là một đẳng cấu, điều kiện cần và đủ là, với mọi tập con mở U của $\mathscr{B},\varphi_U$ là một song ánh từ $\mathscr{F}(U)$ lên $\mathscr{G}(U)$. Điều đó tương đương với việc nói rằng tồn tại một cấu xạ của các tiền bó $\psi :\mathscr{G}\rightarrow \mathscr{F}$ sao cho $\psi \circ \varphi =$ Id$_{\mathscr{F}}$ và $\varphi \circ \psi =$ Id$_{\mathscr{G}}$.

Cho $\mathscr{F}$ và $\mathscr{G}$ là các tiền bó trên B, đối với một cơ sở $\mathscr{B}$ của tôpô trên B, cho $B'$ là một tập con mở của B và cho $\mathscr{B}'$ là một cơ sở của tôpô của $B'$ sao cho $\mathscr{B}'\subset \mathscr{B}$. Cho $\varphi = (\varphi_U)_{U\in\mathscr{B}}$ là một cấu xạ của các tiền bó từ $\mathscr{F}$ vào $\mathscr{G}$. Khi đó $(\varphi_U)_{U\in\mathscr{B}'}$ là một cấu xạ của các tiền bó từ $\mathscr{F}|\mathscr{B}'$ vào $\mathscr{G}|\mathscr{B}'$, được ký hiệu bởi $\varphi |\mathscr{B}'$. Khi $\mathscr{B}$ là tập hợp các tập con mở của B và $\mathscr{B}'$ là tập hợp các tập con mở của $B',\varphi |\mathscr{B}'$ là một cấu xạ của các tiền bó từ $\mathscr{F}|B'$ vào $\mathscr{G}|B'$ và cũng được ký hiệu bởi $\varphi |B'$.

#### Ví dụ 1 {#ta-i-s3-n4-exa-1 .statement tag=01NW}

Cho B là một không gian tôpô, cho $(E, p)$ và $(E', p')$ là các B-không gian và cho $f: E\rightarrow E'$ là một B-cấu xạ. Với mỗi tập con mở U của B, định nghĩa ánh xạ $f_U:\mathscr{S}(U; E)\rightarrow \mathscr{S}(U; E')$ bởi $f_U(s) =$ $f\circ s$. Họ $\mathscr{S}(f) = (f_U)$ là một cấu xạ của các tiền bó từ $\mathscr{S}(B; E)$ vào $\mathscr{S}(B; E')$. Nếu $(E'', p'')$ là một B-không gian và $g: E'\rightarrow E''$ là một B-cấu xạ, ta có $\mathscr{S}(g\circ f) =\mathscr{S}(g)\circ \mathscr{S}(f)$.

#### Ví dụ 2 {#ta-i-s3-n4-exa-2 .statement tag=01NX}

Cho B là một không gian tôpô, $\mathscr{B}$ một cơ sở của tôpô trên B, $\mathscr{F}= (\mathscr{F}(U), f_{UV})$ một tiền bó trên B đối với $\mathscr{B}$ và $\mathscr{L}= (\mathscr{L}(U))$ một tiền bó con của $\mathscr{F}$. Với mọi tập mở $U\in \mathscr{B}$, ký hiệu bởi $i_U$ đơn ánh chính tắc của $\mathscr{L}(U)$ vào $\mathscr{F}(U)$. Khi đó $i= (i_U)_{U\in\mathscr{B}}$ là một cấu xạ của các tiền bó từ $\mathscr{L}$ vào $\mathscr{F}$. Ta nói rằng $i$ là cấu xạ chính tắc từ $\mathscr{L}$ vào $\mathscr{F}$.

#### Ví dụ 3 {#ta-i-s3-n4-exa-3 .statement tag=01NY}

Cho B là một không gian tôpô, $\mathscr{B}$ một cơ sở của tôpô trên B và I một tập hợp. Với mọi $i\in I$, cho $\mathscr{F}_i= (\mathscr{F}_i(U), f_{i,UV})$ là một tiền bó trên B đối với $\mathscr{B}$. Ký hiệu bởi $\mathscr{F}$ tiền bó tích của họ $(\mathscr{F}_i)_{i\in I}$. Với mọi tập mở $U\in \mathscr{B}$, ta có $\mathscr{F}(U) =\prod_{i\in I}\mathscr{F}_i(U)$; với mọi $i\in I$, ký hiệu bởi pr$_{i,U}:\mathscr{F}(U)\rightarrow \mathscr{F}_i(U)$ phép chiếu có chỉ số $i$. Theo ngay lập tức từ định nghĩa của tiền bó $\mathscr{F}$ rằng họ pr$_i$ = (pr$_{i,U}$)$_{U\in\mathscr{B}}$ là một cấu xạ của các tiền bó từ $\mathscr{F}$ vào $\mathscr{F}_i$. Cấu xạ pr$_i$ được gọi là cấu xạ chiếu có chỉ số $i$. Với mọi tiền bó $\mathscr{F}'$ trên B đối với $\mathscr{B}$ và mọi họ $(\psi_i)_{i\in I}$, trong đó $\psi_i$ là một cấu xạ của các tiền bó từ $\mathscr{F}'$ vào $\mathscr{F}_i$, tồn tại một cấu xạ duy nhất của các tiền bó $\psi :\mathscr{F}'\rightarrow \mathscr{F}$ sao cho với mọi $i\in I$, pr$_i\circ \psi =\psi_i$.

#### Ví dụ 4 {#ta-i-s3-n4-exa-4 .statement tag=01NZ}

Cho X là một đa tạp vi phân cấp $C^{\infty}$ trên $\mathbf{R}$ và cho $\mathscr{C}^{\infty}(X;\mathbf{R})$ là bó trên X của các hàm số trị số cấp $C^{\infty}$. Nếu P là một toán tử vi phân với các hệ số $C^{\infty}$ trên X, họ các hạn chế của P trên các tập mở của X là một cấu xạ của bó $\mathscr{C}^{\infty}(X;\mathbf{R})$ vào chính nó. Có thể chứng minh rằng ngược lại, mọi cấu xạ $\mathbf{R}$-tuyến tính của bó $\mathscr{C}^{\infty}(X;\mathbf{R})$ vào chính nó đều địa phương có dạng này (I, p. 142, exerc. 3).

### 5. Không gian étale liên kết với một tiền bó

Cho B là một không gian tôpô, $\mathscr{B}$ một cơ sở của tôpô trên B và $\mathscr{F}= (\mathscr{F}(U), r_{UV})$ một tiền bó trên B đối với cơ sở $\mathscr{B}$. Gọi L là tập hợp các cặp $(U, s)$ với U $\in \mathscr{B}$ và $s\in \mathscr{F}(U)$. Gọi $X_{\mathscr{F}}$ là không gian tổng của họ $(U)_{(U,s)\in L}$. Như vậy $X_{\mathscr{F}}$ là tập hợp các bộ ba $(U, s, x)$ trong đó $U\in \mathscr{B},s\in \mathscr{F}(U),x\in U$. Gọi $R_{\mathscr{F}}$ là quan hệ trên tập hợp $X_{\mathscr{F}}$ được xác định bởi $R_{\mathscr{F}}((U, s, x),(U', s', x'))$ khi và chỉ khi « $x$ = $x'$ và tồn tại W $\in \mathscr{B}$ sao cho $x\in W$, W $\subset U\cap U'$ và $r_{WU}(s) =r_{WU'}(s')$ ». Quan hệ $R_{\mathscr{F}}$ là một quan hệ tương đương trên $X_{\mathscr{F}}:$ theo định nghĩa, nó phản xạ và đối xứng; hãy chứng minh rằng nó bắc cầu. Gọi $\xi = (U, s, x),\xi '= (U', s', x')$ và $\xi ''$ = $(U'', s'', x'')$ là các phần tử của $X_{\mathscr{F}}$ sao cho ta có $R_{\mathscr{F}}(\xi , \xi ')$ và $R_{\mathscr{F}}(\xi ', \xi '')$. Khi đó ta có $x=x'$ = $x''$ và tồn tại hai phần tử $W'$ và $W''$ của $\mathscr{B}$ chứa $x$ sao cho $W'\subset U\cap U',W''\subset U'\cap U'',r_{W'U}(s) =$ $r_{W'U'}(s'),r_{W''U'}(s') =r_{W''U''}(s'')$. Gọi W là một phần tử của $\mathscr{B}$ chứa $x$ và được chứa trong $W'\cap W''$. Khi đó ta có $W\subset U\cap U''$,

$$
r_{WU}(s) =r_{WW'}\circ r_{W'U}(s) =r_{WW'}\circ r_{W'U'}(s') =r_{WU'}(s')
$$

và, tương tự, $r_{WU'}(s') =r_{WU''}(s'')$. Do đó, ta có $R_{\mathscr{F}}(\xi , \xi '')$ và quan hệ $R_{\mathscr{F}}$ là bắc cầu.

Kí hiệu $E_{\mathscr{F}}$ là tập thương $X_{\mathscr{F}}/R_{\mathscr{F}}$ và $[U, s, x]$ là ảnh chính tắc trong $E_{\mathscr{F}}$ của một phần tử $(U, s, x)$ của $X_{\mathscr{F}}$. Với $U\in \mathscr{B}$ và $s\in \mathscr{F}(U)$, kí hiệu $\sigma_{\mathscr{F}}(U, s): U\rightarrow E_{\mathscr{F}}$ là ánh xạ $x\mapsto [U, s, x]$. Trang bị cho tập hợp $E_{\mathscr{F}}$ tôpô thương, nghĩa là tôpô mịn nhất để các ánh xạ $\sigma_{\mathscr{F}}(U, s)$ với $U\in \mathscr{B}$ và $s\in \mathscr{F}(U)$ đều liên tục. Ánh xạ pr$_3: X_{\mathscr{F}}\rightarrow B$ xác định, sau khi chuyển qua thương, một ánh xạ liên tục $p: E_{\mathscr{F}}\rightarrow B$ : ta có $p([U, s, x]) =x$.

#### Mệnh đề 1 {#ta-i-s3-prop-1 .statement tag=01O0}

Ánh xạ $p: E_{\mathscr{F}}\rightarrow$ B là étale. Do đó, với mọi tập mở $U\in \mathscr{B}$ và mọi $s\in \mathscr{F}(U)$, ánh xạ $\sigma_{\mathscr{F}}(U, s)$ là một tiết diện liên tục của $p$ trên U.

Cho $\lambda = (U, s)$ và $\mu= (U', s')$ là các phần tử của L. Theo định nghĩa của quan hệ $R_{\mathscr{F}}$, tập hợp $A_{\lambda \mu}$ các điểm $x$ của $U\cap U'$ tại đó $\sigma_{\mathscr{F}}(U, s)$ và $\sigma_{\mathscr{F}}(U', s')$ trùng nhau là phần trong của tập hợp các $x\in U\cap U'$ sao cho $s(x) =s'(x)$, trong B. Suy ra $A_{\mu\lambda}= A_{\lambda \mu}$. Khi đó ta kí hiệu $h_{\mu\lambda}: A_{\lambda \mu}\rightarrow A_{\mu\lambda}$ là ánh xạ Id$_{A_{\lambda \mu}}$. Tập hợp $E_{\mathscr{F}}$ thu được bằng cách dán các tập mở U dọc theo các $A_{\lambda \mu}$ nhờ các song ánh $h_{\mu\lambda}$ (TG, I, p. 16). Theo mệnh đề 9 của TG, I, p. 17, ánh xạ $\sigma_{\mathscr{F}}(U, s)$ cảm sinh một đồng phôi từ U lên một tập con mở của $E_{\mathscr{F}}$. Điều này chứng tỏ rằng ánh xạ $p$ là étale (I, p. 33, prop 9).

Với mọi tập mở $U\in \mathscr{B}$ và mọi $s\in \mathscr{F}(U)$, ta có $\sigma_{\mathscr{F}}(U, s)(x) =$ $[U, s, x]$ với mọi $x\in U$. Do đó mệnh đề thứ hai suy ra từ định nghĩa của $p$.

#### Định nghĩa 4 {#ta-i-s3-def-4 .statement tag=01O1}

Không gian étalé trên B $(E_{\mathscr{F}}, p)$ được định nghĩa ở trên được gọi là không gian étalé trên B liên kết với tiền bó $\mathscr{F}$. Với $x\in B$, thớ của $E_{\mathscr{F}}$ tại $x$ được gọi là **stalk** của tiền bó $\mathscr{F}$ tại $x$ và được ký hiệu bởi $\mathscr{F}_x$. Với mọi tập mở $U\in \mathscr{B}$, mọi tiết diện $s\in \mathscr{F}(U)$ của $\mathscr{F}$ trên U và mọi điểm $x$ của U, phần tử $[U, s, x]$ của $E_{\mathscr{F}}$ được gọi là mầm tại $x$ của tiết diện $s$.

Cho $a$ là một điểm của B. Tập hợp $\mathscr{B}(a)$ các tập mở $U\in \mathscr{B}$ chứa $a$ và có thứ tự bởi quan hệ $\supset$ là lọc được. Từ $\mathscr{F}$ suy ra, bằng hạn chế của tập hợp chỉ số vào $\mathscr{B}(a)$, một hệ quy nạp $((\mathscr{F}(U))_{U\in\mathscr{B}(a)},(r_{UV}))$. Theo định nghĩa (E, III, p. 60), giới hạn quy nạp của hệ này là thương của tập hợp các cặp $(U, s)$ sao cho $a\in U$ và $s\in \mathscr{F}(U)$ theo quan hệ tương đương R được định nghĩa bởi $R((U, s),(U', s'))$ khi và chỉ khi tồn tại W $\in \mathscr{B}$ chứa $a$ và được chứa trong $U\cap U'$ sao cho $r_{WU}(s) =r_{WU'}(s')$. Vậy giới hạn này được đồng nhất với stalk $\mathscr{F}_a$ của $\mathscr{F}$ tại $a$, theo định nghĩa của giới hạn quy nạp.

Cho $\mathscr{G}$ là một tiền bó trên B đối với cơ sở $\mathscr{B}$ và cho $\varphi = (\varphi_U)_{U\in\mathscr{B}}$ là một cấu xạ tiền bó từ $\mathscr{F}$ vào $\mathscr{G}$. Ánh xạ $(U, s, x)\mapsto$ $(U, \varphi_U(s), x)$ từ $X_{\mathscr{F}}$ vào $X_{\mathscr{G}}$ là tương thích với các quan hệ tương đương $R_{\mathscr{F}}$ và $R_{\mathscr{G}}$, theo định nghĩa của một cấu xạ tiền bó. Ký hiệu bởi $E(\varphi ): E_{\mathscr{F}}\rightarrow E_{\mathscr{G}}$ ánh xạ suy ra từ đó bằng cách chuyển qua các thương. Với mọi $U\in \mathscr{B}$ và mọi $s\in \mathscr{F}(U)$, ta có

$$
E(\varphi )\circ \sigma_{\mathscr{F}}(U, s) =\sigma_{\mathscr{G}}(U, \varphi_U(s))
$$

do đó, ánh xạ $E(\varphi )$ là liên tục. Ánh xạ $E(\varphi )$ là một cấu xạ B; nó được gọi là cấu xạ B của $E_{\mathscr{F}}$ vào $E_{\mathscr{G}}$ liên kết với cấu xạ của các tiền bó $\varphi$. Với mọi $a\in B$, bằng hạn chế vào các thớ tại $a$, $E(\varphi )$ xác định một ánh xạ của thân $\mathscr{F}_a$ của $\mathscr{F}$ vào thân $\mathscr{G}_a$ của $\mathscr{G}$; nó được ký hiệu bởi $\varphi_a$. Nó cũng là giới hạn quy nạp của các ánh xạ $\varphi_U$ (E, III, p. 63), trong đó U chạy qua tập hợp $\mathscr{B}(a)$ các tập mở thuộc cơ sở $\mathscr{B}$ và chứa $a$.

Ta có E(Id$_{\mathscr{F}}$) $=$ Id$_{E_{\mathscr{F}}}$.

Cho $\mathscr{H}$ là một tiền bó trên B đối với $\mathscr{B}$ và cho $\psi = (\psi_U)$ là một cấu xạ các tiền bó từ $\mathscr{G}$ vào $\mathscr{H}$. Với $[U, s, x]\in E_{\mathscr{F}}$, ta có

$$
E(\psi \circ \varphi )([U, s, x]) = [U, \psi_U\circ \varphi_U(s), x]
$$

$$
= E(\psi )([U, \varphi_U(s), x])
$$

$$
= E(\psi )\circ E(\varphi )([U, s, x])
$$

Do đó, ta có $E(\psi \circ \varphi ) = E(\psi )\circ E(\varphi )$. Đặc biệt, nếu $a$ là một điểm của B, thì $(\psi \circ \varphi )_a=\psi_a\circ \varphi_a$.

Nếu $\varphi$ là một đẳng cấu, thì $E(\varphi )$ cũng vậy.

#### Nhận xét {#ta-i-s3-n5-rem-1 .statement tag=01O2}

Cho $\mathscr{F}$ là một bó trên B đối với cơ sở $\mathscr{B}$. Cho $B'$ là một tập con mở của B, cho $\mathscr{B}'$ là một cơ sở của tôpô của $B'$ sao cho $\mathscr{B}'\subset \mathscr{B}$. Gọi $\mathscr{F}|\mathscr{B}'$ là tiền bó trên $B'$ đối với cơ sở $\mathscr{B}'$ suy ra từ $\mathscr{F}$ bằng hạn chế.

1) Khi đó tập hợp $X_{\mathscr{F}|\mathscr{B}'}$ là một tập con của $X_{\mathscr{F}}$ và quan hệ tương đương $R_{\mathscr{F}}$ gây ra trên $X_{\mathscr{F}|\mathscr{B}'}$ quan hệ tương đương $R_{\mathscr{F}|\mathscr{B}'}$. Do đó suy ra một đơn ánh chính tắc $i$ từ $E_{\mathscr{F}|\mathscr{B}'}$ vào $E_{\mathscr{F}}$. Ảnh của nó là $\overset{-1}{p}(B')$ vì với mọi phần tử $[U, s, x]$ của $\overset{-1}{p}(B')$, tồn tại một phần tử V của $\mathscr{B}'$ sao cho $x\in V$ và $V\subset U$, và ta có $[U, s, x] =i([V, r_{VU}(s), x])$. Ánh xạ $i$ là liên tục vì tôpô của $X_{\mathscr{F}|\mathscr{B}'}$ là tôpô mịn nhất làm cho các ánh xạ xác định bởi $x\mapsto [U, s, x]$, với $U\in \mathscr{B}'$ và $s\in \mathscr{F}(U)$, đều liên tục. Theo hệ quả 2 của Mệnh đề 6 trong I, p. 30, đơn ánh chính tắc $i$ từ $E_{\mathscr{F}|\mathscr{B}'}$ vào $E_{\mathscr{F}}$ gây ra một B'-đẳng cấu từ $E_{\mathscr{F}|\mathscr{B}'}$ lên $\overset{-1}{p}(B')$.

Đặc biệt, khi $B'$ bằng B$,i: E_{\mathscr{F}|\mathscr{B}'}\rightarrow E_{\mathscr{F}}$ là một B-đẳng cấu của các không gian étalé.

2) Cho $\mathscr{G}$ là một tiền bó trên B đối với cơ sở $\mathscr{B}$ và cho $\varphi :\mathscr{F}\rightarrow \mathscr{G}$ là một cấu xạ của các tiền bó. Họ $\varphi '= (\varphi_U)_{U\in\mathscr{B}'}$ là một cấu xạ tiền bó từ $\mathscr{F}|\mathscr{B}'$ vào $\mathscr{G}|\mathscr{B}'$. Biểu đồ

$$
E\mathscr{F}|\mathscr{B}'E(\varphi ')E\mathscr{G}|\mathscr{B}'
$$

$ii'$

$E_{\mathscr{F}}^{E(\varphi)}E_{\mathscr{G}}$ , trong đó $i$ và $i'$ là các đơn ánh chính tắc, là giao hoán.

#### Ví dụ 1 {#ta-i-s3-n5-exa-1 .statement tag=01O3}

Cho B là một không gian tôpô, $\mathscr{B}$ là một cơ sở của tôpô của B và F là một tập hợp. Lấy $\mathscr{F}$ là tiền bó trên B đối với cơ sở $\mathscr{B}$ được xác định bởi $\mathscr{F}(U) = F$ với mọi $U\in \mathscr{B}$ và $r_{UV}$ = Id$_F$ với mọi cặp $(U,V)$ các phần tử của $\mathscr{B}$ sao cho $U\subset V$. Ánh xạ $[U, s, x]\mapsto (x, s(x))$ là một B-đẳng cấu của B-không gian $E_{\mathscr{F}}$ lên B-không gian $B\times F$ trong đó F được trang bị tôpô rời rạc. Cần lưu ý rằng khi $\mathscr{B}$ là tập hợp các tập con mở của B, tiền bó $\mathscr{F}$ trên B chỉ là một bó nếu tập hợp F thu về một điểm (xem I, p. 43, nhận xét).

#### Ví dụ 2 {#ta-i-s3-n5-exa-2 .statement tag=01O4}

Cho B là một không gian tôpô và $(E, p)$ một B-không gian. Cho $\mathscr{F}$ là bó trên B gồm các tiết diện liên tục của $(E, p)$. Ánh xạ $(U, s, x)\mapsto s(x)$ từ $X_{\mathscr{F}}$ vào E là tương thích với quan hệ tương đương $R_{\mathscr{F}}$. Ánh xạ $e: E_{\mathscr{F}}\rightarrow E$ suy ra từ đó bằng cách chuyển qua thương là một B-cấu xạ; B-cấu xạ $e$ được gọi là chính tắc. Ảnh của $e$ là hợp của các ảnh của các tiết diện liên tục của $p$ trên các tập mở của B. Do đó ánh xạ $e$ là toàn ánh nếu $p$ là étale (I, p. 33, mệnh đề 9). Mặt khác, ánh xạ $e$ là đơn ánh khi và chỉ khi với mọi tập mở U của B và mọi cặp $(s, s')$ các tiết diện liên tục của $p$ trên U, tập hợp các điểm $x\in U$ sao cho $s(x) =s'(x)$ là mở; điều này đặc biệt đúng nếu $p$ là étale (I, p. 34, mệnh đề 11, b)). Do đó, nếu $(E, p)$ là một B-không gian étale, ánh xạ $e$ là một B-đẳng cấu.

#### Ví dụ 3 {#ta-i-s3-n5-exa-3 .statement tag=01O5}

Cho B là một không gian tôpô, $\mathscr{B}$ một cơ sở của tôpô trên B$,\mathscr{F}$ một tiền bó trên B đối với $\mathscr{B}$ và $\mathscr{L}$ một bó con của $\mathscr{F}$. Khi đó tập hợp $X_{\mathscr{L}}$ được chứa trong tập hợp $X_{\mathscr{F}}$ và quan hệ tương đương $R_{\mathscr{F}}$ cảm sinh trên $X_{\mathscr{L}}$ quan hệ tương đương $R_{\mathscr{L}}$. B-cấu xạ $E(i): E_{\mathscr{L}}\rightarrow E_{\mathscr{F}}$ liên kết với cấu xạ chính tắc $i:\mathscr{L}\rightarrow \mathscr{F}($I, p. 48, ví dụ 2) do đó là đơn ánh. Vì $E_{\mathscr{L}}$ và $E_{\mathscr{F}}$ là các B-không gian étale, ánh xạ $E(i)$ là mở và thậm chí còn étale (I, p. 30, hệ quả 1), và do đó cảm sinh một đồng phôi từ $E_{\mathscr{L}}$ lên một tập con mở của $E_{\mathscr{F}}$.

### 6. Bó liên kết với một tiền bó

Giữ lại các ký hiệu của Số$^o5$. Bó liên kết với tiền bó $\mathscr{F}$ là bó $\mathscr{S}(B; E_{\mathscr{F}})$ gồm các tiết diện liên tục của B-không gian étale $E_{\mathscr{F}}$ liên kết với tiền bó $\mathscr{F}$, và được ký hiệu bởi $\widetilde{\mathscr{F}}$. Với mọi tập mở $U\in \mathscr{B}$, ký hiệu $\sigma_{\mathscr{F}}(U):\mathscr{F}(U)\rightarrow \widetilde{\mathscr{F}}(U)$ là ánh xạ gán cho $s\in \mathscr{F}(U)$ tiết diện liên tục $\sigma_{\mathscr{F}}(U, s):x\mapsto [U, s, x]$ của $E_{\mathscr{F}}$ trên U. Theo định nghĩa của quan hệ tương đương $R_{\mathscr{F}}$, họ $\sigma_{\mathscr{F}}= (\sigma_{\mathscr{F}}(U))_{U\in\mathscr{B}}$ là một cấu xạ tiền bó từ $\mathscr{F}$ vào tiền bó $\widetilde{\mathscr{F}}|\mathscr{B}$. Cấu xạ $\sigma_{\mathscr{F}}$ được gọi là cấu xạ chính tắc của $\mathscr{F}$ vào $\widetilde{\mathscr{F}}|\mathscr{B}$.

Chúng ta ký hiệu bởi $j_{\mathscr{F}}: E_{\mathscr{F}}\rightarrow E_{\mathscr{F}}$ B-cấu xạ hợp thành của B-đẳng cấu chính tắc $E_{\mathscr{F}|\mathscr{B}}\rightarrow E_{\mathscr{F}}\widetilde{(}I$, p. 51) và B-cấu xạ $E(\sigma_{\mathscr{F}}): E_{\mathscr{F}}\rightarrow$ $E_{\widetilde{\mathscr{F}}|\mathscr{B}}$. Mặt khác, ta ký hiệu$\widetilde{s}$ bởi $e_{\mathscr{F}}:E_{\widetilde{\mathscr{F}}}\rightarrow E_{\mathscr{F}}$ B-đẳng cấu chính tắc (I, p. 52, ví dụ 2).

#### Mệnh đề 2 {#ta-i-s3-prop-2 .statement tag=01O6}

Ánh xạ $j_{\mathscr{F}}$ là B-đẳng cấu nghịch đảo của $e_{\mathscr{F}}$.

Với $U\in \mathscr{B},s\in \mathscr{F}(U)$ và $x\in U$, theo định nghĩa của $j_{\mathscr{F}}:$

$$
j_{\mathscr{F}}([U, s, x]) = [U, \sigma_{\mathscr{F}}(U, s), x]
$$

do đó $e_{\mathscr{F}}(j_{\mathscr{F}}([U, s, x])) =\sigma_{\mathscr{F}}(U, s)(x) = [U, s, x]$. Điều này chứng minh mệnh đề.

#### Hệ quả {#ta-i-s3-n6-cor-1 .statement tag=01O7}

Với mọi $a\in B$, ánh xạ $(\sigma_{\mathscr{F}})_a:\mathscr{F}_a\rightarrow \widetilde{\mathscr{F}}_a$ là song ánh.

Vì $j_{\mathscr{F}}$ là một B-đẳng cấu, điều tương tự cũng đúng với $E(\sigma_{\mathscr{F}})$, và $(\sigma_{\mathscr{F}})_a$ được suy ra từ nó bằng cách chuyển qua các thớ tại $a$.

Cho $\mathscr{G}$ là một tiền bó trên B đối với $\mathscr{B}$ và cho $\varphi :\mathscr{F}\rightarrow \mathscr{G}$ là một cấu xạ của các tiền bó. Ta ký hiệu bởi $\widetilde{\varphi}:\widetilde{\mathscr{F}}\rightarrow \widetilde{\mathscr{G}}$ cấu xạ của các bó $\mathscr{S}_{E(\varphi)}($I, p. 48, ví dụ 1), trong đó $E(\varphi ): E_{\mathscr{F}}\rightarrow E_{\mathscr{G}}$ là B-cấu xạ liên kết với $\varphi$. Với mọi tập mở $U\in \mathscr{B}$ và mọi $s\in \mathscr{F}(U)$, theo định nghĩa, ta có

$$
\widetilde{\varphi}_U(\sigma_{\mathscr{F}}(U, s)) = E(\varphi )\circ \sigma_{\mathscr{F}}(U, s) =\sigma_{\mathscr{G}}(U, \varphi_U(s))
$$

Vì vậy ta có:

(1) $\widetilde{\varphi}_U\circ \sigma_{\mathscr{F}}(U) =\sigma_{\mathscr{G}}(U)\circ \varphi_U$, với mọi $U\in \mathscr{B}$. Nói cách khác:

$$
\widetilde{\varphi}|\mathscr{B}\circ \sigma_{\mathscr{F}}=\sigma_{\mathscr{G}}\circ \varphi \tag{2}
$$

#### Mệnh đề 3 {#ta-i-s3-prop-3 .statement tag=01O8}

Cho B là một không gian tôpô, cho $\mathscr{B}$ là một cơ sở của tôpô của B, cho $\mathscr{F}= (\mathscr{F}(U), f_{UV})$ là một tiền bó trên B đối với $\mathscr{B}$, cho $\widetilde{\mathscr{F}}$ là bó liên kết và cho $\sigma_{\mathscr{F}}:\mathscr{F}\rightarrow \widetilde{\mathscr{F}}|\mathscr{B}$ là cấu xạ chính tắc. Với một bó $\mathscr{G}= (\mathscr{G}(U), g_{UV})$ trên B và một cấu xạ của các tiền bó $\varphi :\mathscr{F}\rightarrow \mathscr{G}|\mathscr{B}$, tồn tại một cấu xạ duy nhất của các bó $\psi :\widetilde{\mathscr{F}}\rightarrow \mathscr{G}$ sao cho $\psi |\mathscr{B}\circ \sigma_{\mathscr{F}}=\varphi$.

#### Bổ đề {#ta-i-s3-n6-lem-1 .statement tag=01O9}

Cho U là một tập con mở của B và $s: U\rightarrow E_{\mathscr{F}}$ một tiết diện liên tục của $E_{\mathscr{F}}$ trên U. Với mọi điểm $a$ của U, tồn tại một tập mở $V\in \mathscr{B}$ sao cho $a\in V$ và $V\subset U$, và một phần tử $v$ của $\mathscr{F}(V)$ sao cho $s|V =\sigma_{\mathscr{F}}(V, v)$.

Cho $a\in U$. Theo định nghĩa của không gian $E_{\mathscr{F}}$, tồn tại một tập mở $V'\in \mathscr{B}$ sao cho $a\in V'$ và một phần tử $t$ của $\mathscr{F}(V')$ sao cho $s(a) = [V', t, a]$. Khi đó $s$ và $\sigma_{\mathscr{F}}(V', t)$ cảm sinh, bằng cách hạn chế, hai tiết diện liên tục của $E_{\mathscr{F}}$ trên $V'\cap U$ bằng nhau tại điểm $a$. Theo Mệnh đề 11, b) của I, p. 34, tồn tại một lân cận mở V của $a$, được chứa trong $V'\cap U$, thuộc $\mathscr{B}$, sao cho $s$ và $\sigma_{\mathscr{F}}(V', t)$ bằng nhau tại mọi điểm của V. Nếu đặt $v=f_{VV'}(t)$, thì quả thật ta có $s|V =\sigma_{\mathscr{F}}(V, v)$.

Ta chứng minh mệnh đề. Với mọi tập mở U của B và mọi tiết diện $s\in \widetilde{\mathscr{F}}(U)$, ký hiệu bởi $D(U, s)$ tập hợp các cặp $(V, v)$ sao cho $V\in \mathscr{B},V\subset U,v\in \mathscr{F}(U)$ và $s|V =\sigma_{\mathscr{F}}(V, v)$. Theo bổ đề, các tập mở V này tạo thành một phủ của U.

Nếu tồn tại một cấu xạ $\psi :\widetilde{\mathscr{F}}\rightarrow \mathscr{G}$ sao cho $\psi |\mathscr{B}\circ \sigma_{\mathscr{F}}=\varphi$, thì với mọi tập mở U của B, mọi tiết diện $s\in \widetilde{\mathscr{F}}(U)$ và mọi cặp $(V, v)\in D(U, s)$, ta có $g_{VU}(\psi_U(s)) =\psi_V(s|V) =\varphi_V(v)$. Điều này chứng minh tính duy nhất của $\psi$ do tính chất $(F_1)$ của các bó.

Cho U là một tập mở của B và $s$ là một phần tử của $\widetilde{\mathscr{F}}(U)$. Cho $(V, v)$ và $(V', v')$ là các phần tử của $D(U, s)$. Ta có $s(a) = [V, v, a] = [V', v', a]$ với mọi điểm $a\in V\cap V'$. Do đó tồn tại một cặp $(W, w)\in D(V\cap V', s)$ sao cho $a\in W$ và $f_{WV}(v) =f_{WV}(v') =w$. Khi đó ta có

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

Vì tính chất $(F_1)$ của các bó, do đó ta có

$$
g_{(V\cap V')V}(\varphi_V(v)) =g_{(V\cap V')V'}(\varphi_{V'}(v'))
$$

Theo các tính chất $(F_1)$ và $(F_2)$ của các bó, tồn tại một phần tử duy nhất $\psi_U(s)\in \mathscr{G}(U)$ sao cho ta có:

(3) $g_{VU}(\psi_U(s)) =\varphi_V(v)$ với mọi $(V, v)\in D(u, s)$.

Cho $\psi_U:\widetilde{\mathscr{F}}(U)\rightarrow \mathscr{G}(U)$ là ánh xạ thu được. Từ (3) suy ra ngay lập tức rằng họ $\psi = (\psi_U)$ là một cấu xạ của các bó và rằng ta có $\varphi_V=\psi_V\circ \sigma_{\mathscr{F}}(V)$ với mọi $V\in \mathscr{B}$.

#### Hệ quả 1 {#ta-i-s3-prop-3-cor-1 .statement tag=01OA}

Cho B là một không gian tôpô, $\mathscr{F}$ là một tiền bó trên B$,\widetilde{\mathscr{F}}$ là bó liên kết và $\sigma_{\mathscr{F}}:\mathscr{F}\rightarrow \widetilde{\mathscr{F}}$ là cấu xạ chính tắc. Để $\mathscr{F}$ là một bó, điều kiện cần và đủ là $\sigma_{\mathscr{F}}$ là một đẳng cấu.

Nếu $\sigma_{\mathscr{F}}$ là một đẳng cấu, thì $\mathscr{F}$ là một bó. Ngược lại, nếu $\mathscr{F}$ là một bó, thì theo mệnh đề 3 tồn tại một cấu xạ $\varphi :\widetilde{\mathscr{F}}\rightarrow \mathscr{F}$ sao cho $\varphi \circ \sigma_{\mathscr{F}}=$ Id$_{\mathscr{F}}$. Vì Id$_{\mathscr{F}}$ là cấu xạ duy nhất $\psi :\widetilde{\mathscr{F}}\rightarrow \widetilde{\mathscr{F}}$ sao cho $\psi \circ \sigma_{\mathscr{F}}=\sigma_{\mathscr{F}}$, do đó ta có $\widetilde{\sigma}_{\mathscr{F}}\circ \varphi =$ Id$_{\widetilde{\mathscr{F}}}$.

#### Nhận xét {#ta-i-s3-n6-rem-1 .statement tag=01OB}

Cho B là một không gian tôpô, $\mathscr{F}$ một tiền bó trên B, $\mathscr{G}$ một bó trên B và $\varphi :\mathscr{F}\rightarrow \mathscr{G}$ một cấu xạ của các tiền bó. Cấu xạ chính tắc $\sigma_{\mathscr{G}}:\mathscr{G}\rightarrow \widetilde{\mathscr{G}}$ là một đẳng cấu theo hệ quả 1. Theo quan hệ (2) của I, p. 54, cấu xạ duy nhất $\psi :\widetilde{\mathscr{F}}\rightarrow \mathscr{G}$ sao cho $\psi \circ \sigma_{\mathscr{F}}=\varphi$ do đó là $\sigma^{-1}_{\mathscr{G}}\circ \widetilde{\varphi}$.

#### Hệ quả 2 {#ta-i-s3-prop-3-cor-2 .statement tag=01OC}

Cho B là một không gian tôpô, $\mathscr{F}$ và $\mathscr{G}$ là các bó trên B và $\varphi$ là một cấu xạ của các bó từ $\mathscr{F}$ vào $\mathscr{G}$. Các khẳng định sau là tương đương:

(i) $\varphi$ là một đẳng cấu;

(ii) Tồn tại một cơ sở $\mathscr{B}$ của tôpô của B sao cho với mọi $U\in \mathscr{B}$, ánh xạ $\varphi_U$ là song ánh;

(iii) Với mọi điểm $a$ của B, ánh xạ $\varphi_a$ là một song ánh của thân $\mathscr{F}_a$ lên thân $\mathscr{G}_a$.

Hệ quả (i)$\Rightarrow$(ii) là ngay lập tức.

(ii)$\Rightarrow$(iii) : xét biểu đồ giao hoán (I, p. 51)

$$
E\mathscr{F}|\mathscr{B}E(\varphi |\mathscr{B})E\mathscr{G}|\mathscr{B}
$$

$$
E_{\mathscr{F}}^{E(\varphi)}E_{\mathscr{G}}
$$

trong đó các mũi tên thẳng đứng là các B-đẳng cấu chính tắc. Nếu điều kiện (ii) được thỏa mãn, thì $E(\varphi |\mathscr{B})$ là một B-đẳng cấu, do đó $E(\varphi )$ cũng là một B-đẳng cấu. Các ánh xạ $\varphi_a$ suy ra từ $E(\varphi )$ bằng cách chuyển qua các thớ và vì thế là song ánh.

(iii)$\Rightarrow$(i) : dưới giả thiết (iii), ánh xạ $E(\varphi ): E_{\mathscr{F}}\rightarrow E_{\mathscr{G}}$ là một B-cấu xạ song ánh của các không gian étalé và vì thế là một B-đẳng cấu (I, p. 30, hệ quả 2 của mệnh đề 6). Do đó cấu xạ $\widetilde{\varphi}:\widetilde{\mathscr{F}}\rightarrow \widetilde{\mathscr{G}}$ là một đẳng cấu. Vì $\mathscr{F}$ và $\mathscr{G}$ là các bó, các cấu xạ chính tắc $\sigma_{\mathscr{F}}:\mathscr{F}\rightarrow \widetilde{\mathscr{F}}$ và $\sigma_{\mathscr{G}}:\mathscr{G}\rightarrow \widetilde{\mathscr{G}}$ là các đẳng cấu (hệ quả 1) và ta có $\widetilde{\varphi}\circ \sigma_{\mathscr{F}}=\sigma_{\mathscr{G}}\circ \varphi ($I, p. 54, quan hệ (2)) do đó $\varphi$ là một đẳng cấu.

#### Chú giải {#ta-i-s3-n6-sch-1 .statement tag=01OD}

Cho B là một không gian tôpô. Với mỗi bó $\mathscr{F}$ trên B, người ta gắn với nó một không gian étalé trên B $E_{\mathscr{F}}$ (I, p. 50, định nghĩa 4). Với mỗi không gian étalé trên B T, người ta gắn với nó bó $\mathscr{S}(T)$ trên B gồm các thiết diện liên tục của nó (I, p. 45, ví dụ 3). Một đẳng cấu chính tắc của các bó $\sigma_{\mathscr{F}}:\mathscr{F}\rightarrow \mathscr{S}(E_{\mathscr{F}})$ đã được xác định (I, p. 55, hệ quả 1) và một đẳng cấu chính tắc của các không gian étalé trên B $e_T: E_{\mathscr{S}(T)}\rightarrow T$ (I, p. 52, ví dụ 2).

Với mọi cặp $(\mathscr{F},\mathscr{G})$ các bó trên B, một ánh xạ $\varphi \mapsto E(\varphi )$ từ tập hợp các cấu xạ của các bó từ $\mathscr{F}$ vào $\mathscr{G}$ vào tập hợp các B-cấu xạ từ $E_{\mathscr{F}}$ vào $E_{\mathscr{G}}$ đã được xác định (I, p. 50). Ta có các quan hệ

E(Id$_{\mathscr{F}}$) $=$ Id$_{E_{\mathscr{F}}},E(\psi \circ \varphi ) = E(\psi )\circ E(\varphi )$.

Với mọi cặp $(T,U)$ các không gian étalé trên B, một ánh xạ $f\mapsto \mathscr{S}(f)$ từ tập hợp các B-cấu xạ của T vào U tới tập hợp các cấu xạ bó của $\mathscr{S}(T)$ vào $\mathscr{S}(U)$ đã được định nghĩa (I, p. 48, Ví dụ 1). Ta có các hệ thức

$\mathscr{S}$ (Id$_T$) $=$ Id$_{\mathscr{S}(T)},\mathscr{S}(g\circ f) =\mathscr{S}(g)\circ \mathscr{S}(f)$.

Với ký hiệu ở trên, các biểu đồ sau là giao hoán:

$$
\mathscr{F}^{\varphi}\mathscr{G}E_{\mathscr{S}(T)}^{E(\mathscr{S}(f))}E_{\mathscr{S}(U)}
$$

(4) $\sigma_{_{\mathscr{F}}}\sigma_{_{\mathscr{G}}}$ (5) $e_{_T}e_{_U}$

$\mathscr{S}(E_{\mathscr{F}})^{\mathscr{S}(E(\varphi))}\mathscr{S}(E_{\mathscr{G}})$, T $^fU$.

Điều này suy ra từ I, p. 54, công thức (2) đối với biểu đồ thứ nhất, và là một hệ quả ngay lập tức của các định nghĩa đối với biểu đồ thứ hai. Điều này kéo theo rằng với mọi cặp $(\mathscr{F},\mathscr{G})$ các bó trên B và mọi cặp $(T,U)$ các không gian étalé trên B, các ánh xạ $\varphi \mapsto E(\varphi )$ và $f\mapsto \mathscr{S}(f)$ được xét ở trên là song ánh.

Các kết quả này cho phép suy ra một mệnh đề về các không gian étalé trên B từ một mệnh đề về các bó trên B, và ngược lại.

### 7. Ảnh trực tiếp và ảnh ngược của một bó

Cho A và B là các không gian tôpô và cho $u: A\rightarrow B$ là một ánh xạ liên tục.

Cho $\mathscr{F}= (\mathscr{F}(U), f_{UV})$ là một tiền bó trên A. Ta định nghĩa một tiền bó $\mathscr{F}'$ trên B như sau: với mọi tập mở U của B, đặt $\mathscr{F}'(U) =\mathscr{F}(\overset{-1}{u}(U))$ và với mọi cặp $(U,V)$ các tập mở của B sao cho U $\subset V$, đặt $f'_{UV}=f_{\overset{-1}{u}(U)\overset{-1}{u}(V)}$. Khi đó $(\mathscr{F}'(U), f'_{UV})$ là một tiền bó trên B. Nó được ký hiệu bởi $u_*(\mathscr{F})$ và được gọi là tiền bó ảnh trực tiếp của tiền bó $\mathscr{F}$ bởi ánh xạ $u$.

Nếu $(U_i)_{i\in I}$ là một họ các tập mở của B, ta có $\overset{-1}{u}(\bigcup_{i\in I}U_i) =$ $\bigcup_{i\in I}\overset{-1}{u}(U_i)$ và $\overset{-1}{u}(\bigcap_{i\in I}U_i) =\bigcap_{i\in I}\overset{-1}{u}(U_i)$ (E, II, p. 25, Prop. 3 and 4). Lập tức suy ra rằng, nếu $\mathscr{F}$ có tính chất $(F_1)$ (resp. $(F_2)$) của các bó (I, p. 43), thì $u_*(\mathscr{F})$ cũng có tính chất đó. Do đó, ảnh trực tiếp của một bó là một bó.

Cho $\mathscr{F}_1$ và $\mathscr{F}_2$ là các tiền bó trên A và cho $\varphi :\mathscr{F}_1\rightarrow \mathscr{F}_2$ là một cấu xạ tiền bó. Khi đó tồn tại một cấu xạ tiền bó duy nhất $u_*\varphi :u_*\mathscr{F}_1\rightarrow u_*\mathscr{F}_2$ sao cho với mọi tập mở U của B, ánh xạ $(u_*\varphi )(U): (u_*\mathscr{F}_1)(U)\rightarrow (u_*\mathscr{F}_2)(U)$ là ánh xạ $\varphi (\overset{-1}{u}(U)):\mathscr{F}_1(\overset{-1}{u}(U))\rightarrow \mathscr{F}_2(\overset{-1}{u}(U))$. Nếu $\mathscr{F}_3$ là một tiền bó trên A và nếu $\psi :\mathscr{F}_2\rightarrow \mathscr{F}_3$ là một cấu xạ tiền bó, ta có $u_*(\psi \circ \varphi ) =u_*(\psi )\circ u_*(\varphi )$.

Cho C là một không gian tôpô và cho $v: B\rightarrow$ C là một ánh xạ liên tục. Nếu $\mathscr{F}$ là một tiền bó trên A, thì các tiền bó $v_*(u_*(\mathscr{F}))$ và $(v\circ u)_*(\mathscr{F})$ trùng nhau. Nếu $\varphi :\mathscr{F}_1\rightarrow \mathscr{F}_2$ là một cấu xạ tiền bó trên A, ta có đẳng thức $v_*(u_*(\varphi )) = (v\circ u)_*(\varphi )$.

#### Ví dụ 1 {#ta-i-s3-n7-exa-1 .statement tag=01OE}

Cho B là một không gian tôpô, A là một không gian con của B và $\mathscr{F}= (\mathscr{F}(U), f_{UV})$ là một tiền bó trên A. Gọi $i: A\rightarrow B$ là đơn ánh chính tắc. Khi đó ta có $i_*(\mathscr{F}) = (\mathscr{F}'(U), f'_{UV})$ trong đó với mọi tập mở U của B$,\mathscr{F}'(U) =\mathscr{F}(U\cap A)$, và với mọi cặp $(U,V)$ các tập mở của B với $U\subset V,f'_{UV}=f_{(U\cap A)(V\cap A)}$.

Bây giờ cho $\mathscr{G}$ là một tiền bó trên B. Ảnh ngược của tiền bó $\mathscr{G}$ bởi $u$ được định nghĩa là, và được ký hiệu bởi $u^*(\mathscr{G})$, bó $\mathscr{C}_B(A; E_{\mathscr{G}})$ trên A gồm các B-cấu xạ với giá trị trong B-không gian $E_{\mathscr{G}}($I, p. 45, ví dụ 4). Nó đẳng cấu chính tắc với bó trên A gồm các thiết diện của không gian étalé A $A\times_BE_{\mathscr{G}}$ (I, p. 9, mệnh đề 3). Từ đó suy ra (I, p. 52, ví dụ 2) một đẳng cấu chính tắc $\varphi$ từ không gian étalé liên kết với $u^*(\mathscr{G})$ lên A-không gian $A\times_BE_{\mathscr{G}}$. Hơn nữa, nếu $\mathscr{G}$ là một bó, thì với mọi điểm $a$ của A có một song ánh chính tắc $\psi_a:u^*(\mathscr{G})_a\rightarrow \mathscr{G}_{u(a)}:$ với mọi lân cận mở U của $a$ trong A và mọi B-cấu xạ $f: U\rightarrow E_{\mathscr{G}}$, ta có

$$
\varphi ([U, f, a]) = (a, f(a)),\psi_a([U, f, a]) =f(a)
$$

Cho $\mathscr{G}_1$ và $\mathscr{G}_2$ là các tiền bó trên B và cho $\varphi :\mathscr{G}_1\rightarrow \mathscr{G}_2$ là một cấu xạ của các tiền bó. Bằng thay đổi cơ sở của cấu xạ các B-không gian étalé $E(\varphi ): E_{\mathscr{G}_1}\rightarrow E_{\mathscr{G}_2}$ ta thu được một cấu xạ của các A-không gian étalé $A\times_BE_{\mathscr{G}_1}\rightarrow A\times_BE_{\mathscr{G}_2}$, do đó một cấu xạ của các bó trên A$,u^*(\varphi ):u^*(\mathscr{G}_1)\rightarrow u^*(\mathscr{G}_2)$. Cho $\mathscr{G}_3$ là một tiền bó trên B và cho $\psi :\mathscr{G}_2\rightarrow \mathscr{G}_3$ là một cấu xạ của các tiền bó. Khi đó có đẳng thức $u^*(\psi \circ \varphi ) =u^*(\psi )\circ u^*(\varphi )$.

Cho C là một không gian tôpô và cho $v: B\rightarrow$ C là một ánh xạ liên tục. Nếu $\mathscr{G}$ là một tiền bó trên C, thì các bó $u^*(v^*(\mathscr{G}))$ và $(v\circ u)^*(\mathscr{G})$ được đồng nhất một cách chính tắc (I, p. 5). Nếu $\varphi :\mathscr{G}_1\rightarrow \mathscr{G}_2$ là một cấu xạ của các tiền bó trên C, thì hơn nữa ta có $u^*(v^*(\varphi )) = (v\circ u)^*(\varphi )$.

#### Nhận xét {#ta-i-s3-n7-rem-1 .statement tag=01OF}

Cấu xạ chính tắc $\sigma_{\mathscr{G}}:\mathscr{G}\rightarrow \widetilde{\mathscr{G}}$ ở I, p. 53 tương ứng, theo ngôn ngữ các không gian étalé, với đẳng cấu $j_{\mathscr{G}}$ của mệnh đề 2 ở I, p. 53. Suy ra rằng $u^*(\sigma_{\mathscr{G}})$ là một đẳng cấu. Đặc biệt, nếu A = B và $u=$ Id$_A$, thì tiền bó $u^*(\mathscr{F})$ là bó $\widetilde{\mathscr{F}}$.

#### Ví dụ 2 {#ta-i-s3-n7-exa-2 .statement tag=01OG}

Cho B là một không gian tôpô và A là một không gian con của B. Cho $i: A\rightarrow B$ ký hiệu đơn ánh chính tắc. Với mọi bó $\mathscr{G}$ trên B, ký hiệu $\mathscr{G}_A$ là bó $i^*(\mathscr{G})$, và nói rằng $\mathscr{G}_A$ là bó trên A cảm sinh bởi bó $\mathscr{G}$. Bó $\mathscr{G}_A$ được đồng nhất với bó $\mathscr{S}(A; (E_{\mathscr{G}})_A)$ gồm các thiết diện của không gian étalé A cảm sinh bởi $E_{\mathscr{G}}$ trên A.

Giả sử rằng A là một không gian con mở của B, và cho $\mathscr{G}$ là một bó trên B. Theo định nghĩa, bó $\mathscr{G}_A$ là bó $\widetilde{\mathscr{G}}|A$ suy ra từ $\widetilde{\mathscr{G}}$ bằng hạn chế vào tập mở A (I, p. 43). Cho $\sigma_{\mathscr{G}}:\mathscr{G}\rightarrow \widetilde{\mathscr{G}}$ là đẳng cấu chính tắc (I, p. 55, hệ quả 1). Khi đó $\sigma_{\mathscr{G}}|A$ là một đẳng cấu, gọi là chính tắc, từ bó $\mathscr{G}|A$ lên bó $\mathscr{G}_A$ và được gọi là đẳng cấu chính tắc từ $\mathscr{G}|A$ lên $\mathscr{G}_A$.

### 8. Các đồng cấu $\alpha \mathbf{e}\mathbf{t}\beta$ ; phép nối

Cho A và B là các không gian tôpô và cho $u: A\rightarrow B$ là một ánh xạ liên tục. Cho $\mathscr{G}$ là một tiền bó trên B. Theo định nghĩa của ảnh trực tiếp của các tiền bó, một tiết diện của bó $u_*u^*\mathscr{G}$ trên một tập mở U của B là một tiết diện của bó $u^*\mathscr{G}$ trên tập mở $\overset{-1}{u}(U)$ của A, tức là một B-cấu xạ $\overset{-1}{u}(U)\rightarrow E_{\mathscr{G}}$. Do đó người ta định nghĩa một cấu xạ bó $\widetilde{\mathscr{G}}\rightarrow u_*u^*\mathscr{G}$ bằng cách gán cho tiết diện $s$ của $E_{\mathscr{G}}$ trên một tập mở U của B tiết diện $s\circ u$ của $E_{\mathscr{G}}$ trên $\overset{-1}{u}(U)$. Hợp thành của cấu xạ này với cấu xạ chính tắc $\sigma_{\mathscr{G}}:\mathscr{G}\rightarrow \widetilde{\mathscr{G}}$ (I, p. 53) là một cấu xạ tiền bó $\mathscr{G}\rightarrow u_*u^*\mathscr{G}$ sẽ được ký hiệu bởi $\beta_{\mathscr{G}}^u$, hoặc thậm chí bởi $\beta_{\mathscr{G}}$ nếu không có sự mơ hồ nào về ánh xạ $u$.

#### Nhận xét 1 {#ta-i-s3-n8-rem-1 .statement tag=01OH}

Cho A, B, C là các không gian tôpô, cho $u: A\rightarrow B,v: B\rightarrow C$ là các ánh xạ liên tục; đặt $w=v\circ u$. Cho $\mathscr{G}$ là một tiền bó trên C.

Cho U là một tập mở của C và $s$ là một tiết diện của $E_{\mathscr{G}}$ trên U. Khi đó $\beta_{\mathscr{G}}^v(s)$ là tiết diện $s\circ v$ của $E_{\mathscr{G}}$ trên $\overset{-1}{v}(U)$, và $v_*(\beta_{v^*\mathscr{G}}^u)(\beta^v_{\mathscr{G}}(s))$ là tiết diện $s\circ v\circ u=s\circ w$ của $E_{\mathscr{G}}$ trên $\overset{-1}{u}(\overset{-1}{v}(U)) =\overset{-1}{w}(U)$.

Suy ra rằng $\beta_{\mathscr{G}}^w=v_*(\beta_{v^*\mathscr{G}}^u)\circ \beta_{\mathscr{G}}^v$.

#### Nhận xét 2 {#ta-i-s3-n8-rem-2 .statement tag=01OI}

Nếu $\gamma :\mathscr{G}_1\rightarrow \mathscr{G}_2$ là một cấu xạ tiền bó trên B, thì các cấu xạ tiền bó $\beta_{\mathscr{G}_2}\circ \gamma$ và $u_*u^*(\gamma )\circ \beta_{\mathscr{G}_1}$ là bằng nhau. Thật vậy, nếu V là một tập mở của B và $s\in \mathscr{G}_1(V),\beta_{\mathscr{G}_1}(s)$ là tiết diện $t$ của $A\times_BE_{\mathscr{G}_1}$ trên $\overset{-1}{u}(V)$, được xác định bởi $x\mapsto (x,[V, s, u(x)])$. Do đó ảnh của $t$ dưới $u^*(\gamma )$ là tiết diện của $A\times_BE_{\mathscr{G}_2}$ trên $\overset{-1}{u}(V)$ cho bởi $x\mapsto (x,[V, \gamma (s), u(x)])$. Vậy quả thật $u_*u^*(\gamma )\circ \beta_{\mathscr{G}_1}(s) =\beta_{\mathscr{G}_2}(\gamma (s))$.

#### Mệnh đề 4 {#ta-i-s3-prop-4 .statement tag=01OJ}

Cho A và B là các không gian tôpô, $u: A\rightarrow B$ là một ánh xạ liên tục, $\mathscr{G}$ là một tiền bó trên B$,\mathscr{F}$ là một bó trên A.

Với mọi cấu xạ tiền bó $\varphi :\mathscr{G}\rightarrow u_*\mathscr{F}$, tồn tại một cấu xạ bó duy nhất $\psi :u^*(\mathscr{G})\rightarrow \mathscr{F}$ sao cho $\varphi =u_*(\psi )\circ \beta_{\mathscr{G}}$.

Nói cách khác, ánh xạ chính tắc

Mor($u^*(\mathscr{G}),\mathscr{F}$)$\rightarrow$ Mor($\mathscr{G}, u_*(\mathscr{F})$)$,\psi \mapsto u_*(\psi )\circ \beta_{\mathscr{G}}$

là một song ánh.

Với ký hiệu của mệnh đề 4, đôi khi người ta sẽ ký hiệu $\psi =\varphi^{\sharp}$ và $\varphi =\psi^{\flat}$.

Ta chứng minh mệnh đề 4. Theo nhận xét 2 áp dụng cho cấu xạ $\sigma_{\mathscr{G}}:\mathscr{G}\rightarrow \widetilde{\mathscr{G}}$, cấu xạ $\beta_{\mathscr{G}}$ bằng hợp thành

$$
u_*(u^*(\sigma_{\mathscr{G}})^{-1})\circ \beta_{\widetilde{\mathscr{G}}}\circ \sigma_{\mathscr{G}}
$$

trong đó $u^*(\sigma_{\mathscr{G}}):u^*(\mathscr{G})\rightarrow u^*(\widetilde{\mathscr{G}})$ là đẳng cấu chính tắc của nhận xét ở I, p. 58. Gọi $\widetilde{\varphi}:\widetilde{\mathscr{G}}\rightarrow u_*\mathscr{F}$ là cấu xạ bó duy nhất sao cho $\widetilde{\varphi}\circ \sigma_{\mathscr{G}}=\varphi ($I, p. 54, mệnh đề 3). Khi đó chỉ cần chứng minh rằng tồn tại một cấu xạ bó duy nhất $\widetilde{\psi}:u^*(\mathscr{G})\rightarrow \mathscr{F}$ sao cho $u_*(\widetilde{\psi})\circ \beta_{\mathscr{G}}=\widetilde{\varphi}$.

Vì vậy ta c$\widetilde{o}$ thể giả sử rằng $\mathscr{G}$ là một bó. Để một cấu xạ bó $\psi :u^*(\mathscr{G})\rightarrow \mathscr{F}$ thỏa mãn kết luận của mệnh đề 4, điều kiện cần và đủ là với mọi tập mở V của B và mọi tiết diện $t$ của $E_{\mathscr{G}}$ trên V, ta có

$$
\varphi_V(t) =\psi_{\overset{-1}{u}(V)}(t\circ u|\overset{-1}{u}(V)) \tag{6}
$$

Gọi $U_0$ là một tập mở của A và $s_0$ là một phần tử của $u^*(\mathscr{G})(U_0)$, nói cách khác là một B-cấu xạ từ $U_0$ vào $E_{\mathscr{G}}$. Gọi $S(U_0, s_0)$ là tập hợp các bộ ba $(U,V, t)$ trong đó U là một tập mở của A được chứa trong $U_0$, V là một tập mở của B sao cho $u(U)\subset V$, và $t$ là một tiết diện của $E_{\mathscr{G}}$ trên V sao cho ta có

$$
t\circ u|U =s_0|U \tag{7}
$$

Nếu $U_1$ và $U_2$ là các tập mở của A với $U_1\subset U_2$, ta ký hiệu bởi $f_{U_1U_2}$ ánh xạ hạn chế $\mathscr{F}(U_2)\rightarrow \mathscr{F}(U_1)$. Với mọi $(U,V, t)\in S(U_0, s_0)$, khi đó ta có quan hệ

$$
f_{UU_0}(\psi_{U_0}(s_0)) =\psi_U(s_0|U)
$$

$$
=\psi_U(t\circ u|U)
$$

$$
=f_{U\overset{-1}{u}(V)}(\psi_{\overset{-1}{u}(V)}(t\circ u|\overset{-1}{u}(V)))
$$

Do đó, nếu $\psi :u^*(\mathscr{G})\rightarrow \mathscr{F}$ thỏa mãn (6), thì ta có

$$
f_{UU_0}(\psi_{U_0}(s_0)) =f_{U\overset{-1}{u}(V)}(\varphi_V(t)) \tag{8}
$$

Ta hãy chứng minh rằng, với mọi điểm $a$ của $U_0$, tồn tại một bộ ba $(U,V, t)\in S(U_0, s_0)$ sao cho $a\in U$. Thật vậy, gọi $a$ là một điểm của $U_0$. Tồn tại một lân cận mở V của B chứa $u(a)$ và một tiết diện $t$ của không gian étalé $E_{\mathscr{G}}$ trên V sao cho $t(u(a)) =s_0(a)$ (I, p. 33, mệnh đề 9). Đặt $U_1=\overset{-1}{u}(V)\cap U_0$. Các tiết diện $s_0|U_1$ và $t\circ u|U_1$ của không gian étalé trên $U_1$ là $E_{\mathscr{G}}\times_BU_1$ trùng nhau tại điểm $a$. Theo mệnh đề 11, b) của I, p. 34, tập hợp các điểm tại đó chúng trùng nhau là một tập mở U của $U_1$ chứa $a$. Khi đó bộ ba $(U,V, t)$ thuộc $S(U_0, s_0)$.

Công thức (8) và tính chất $(F_1)$ của các bó (I, p. 43) khi đó suy ra tính duy nhất của $\psi$.

Cho $(U,V, t)$ và $(U',V', t')$ là các phần tử của $S(U_0, s_0)$. Theo quan hệ (7), các hạn chế của $t$ và $t'$ lên $u(U\cap U')$ trùng nhau. Theo Mệnh đề 11, b) của I, p. 34, tồn tại một tập mở W của B sao cho $u(U\cap U')\subset$ $W\subset V\cap V'$ và $t|W =t'|W$. Do đó

$$
f_{\overset{-1}{u}(W)\overset{-1}{u}(V)}(\varphi_V(t)) =\varphi_W(t|W) =\varphi_W(t'|W) =f_{\overset{-1}{u}(W)\overset{-1}{u}(V')}(\varphi_{V'}(t'))
$$

suy ra

$$
f_{(U\cap U')\overset{-1}{u}(V)}(\varphi_V(t)) =f_{(U\cap U')\overset{-1}{u}(V')}(\varphi_{V'}(t')) \tag{9}
$$

Theo các tính chất $(F_1)$ và $(F_2)$ của bó $\mathscr{F}$, tồn tại một phần tử duy nhất $s'$ của $\mathscr{F}(U_0)$ sao cho với mọi bộ ba $(U,V, t)$ của $S(U_0, s_0)$, ta có:

$$
f_{UU_0}(s') =f_{U\overset{-1}{u}(V)}(\varphi_V(t)) \tag{10}
$$

Hãy ký hiệu phần tử này là $\psi_{U_0}(s_0)$.

Cho $U_1$ là một tập mở được chứa trong $U_0$ và đặt $s_1=s_0|U_1$. Nếu $(U,V, t)\in$ $S(U_1, s_1)$, thì U là một tập mở được chứa trong $U_0$ và $t\circ u|U =s_1|U =s_0|U$, do đó $(U, v, t)\in S(U_0, s_0)$ và khi ấy quan hệ (10) kéo theo rằng

$$
f_{UU_1}(f_{U_1U_0}(\psi_{U_0}(s_0))) =f_{UU_0}(\psi_{U_0}(s_0)) =f_{U\overset{-1}{u}(V)}(\varphi_V(t))
$$

Theo định nghĩa của $\psi_{U_1}(s_1)$, vì vậy ta có $\psi_{U_1}(s_1) =f_{U_1U_0}(\psi_{U_0}(s_0))$. Điều này chứng minh rằng họ $\psi = (\psi_U)$ là một cấu xạ của các bó từ $u^*(\mathscr{G})$ vào $\mathscr{F}$.

Hãy chứng minh rằng $\psi$ thỏa mãn quan hệ (6). Do đó cho V là một tập mở của B và cho $t$ là một tiết diện của $E_{\mathscr{G}}$ trên V. Nếu U = $\overset{-1}{u}(V)$ và nếu $s=t\circ u|U$, thì bộ ba $(U,V, t)$ thuộc $S(U, s)$ và quan hệ (6) là một hệ quả ngay lập tức của quan hệ (10), áp dụng cho $U = U_0$.

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

Do đó, $\varphi \circ \gamma =u_*(\varphi^{\sharp}\circ u^*(\gamma ))\circ \beta_{\mathscr{G}_1}$, suy ra quan hệ (11).

b) Theo định nghĩa của $\gamma^{\sharp}$, ta có

$$
u_*(\varphi )\circ \gamma =u_*(\varphi )\circ u_*(\gamma^{\sharp})\circ \beta_{\mathscr{G}}=u_*(\varphi \circ \gamma^{\sharp})\circ \beta_{\mathscr{G}}
$$

do đó có quan hệ đã phát biểu, xét đến định nghĩa của $(u_*(\varphi )\circ \gamma )^{\sharp}$.

Đặt $\alpha_{\mathscr{F}}$ = Id$^{\sharp}_{u_*(\mathscr{F})}$; đó là cấu xạ bó duy nhất $\rho :u^*(u_*(\mathscr{F}))\rightarrow \mathscr{F}$ sao cho

Id$_{u_*(\mathscr{F})}=u_*(\rho )\circ \beta_{u_*(\mathscr{F})}$.

Quan hệ (11), áp dụng cho $\mathscr{G}_2=u_*(\mathscr{F})$ và cho cấu xạ $\varphi =$ Id$_{u_*(\mathscr{F})}$, cho với mọi cấu xạ tiền bó $\gamma :\mathscr{G}\rightarrow u_*(\mathscr{F})$ sự phân tích

$$
\gamma^{\sharp}=\alpha_{\mathscr{F}}\circ u^*(\gamma )
$$

Từ đó theo mệnh đề 4 suy ra rằng với mọi cấu xạ bó $\psi$ từ $u^*(\mathscr{G})$ vào $\mathscr{F}$, $\psi^{\flat}$ là cấu xạ duy nhất $\varphi :\mathscr{G}\rightarrow u_*(\mathscr{F})$ sao cho $\psi =\alpha_{\mathscr{F}}\circ u^*(\varphi )$.

#### Ví dụ 1 {#ta-i-s3-n8-exa-1 .statement tag=01OL}

Xét một không gian tôpô B, một không gian con A của B, và ký hiệu bởi $i: A\rightarrow B$ đơn ánh chính tắc. Cho $(E, p)$ và $(E', p')$ là các B-không gian. Lấy $\mathscr{G}$ là bó $\mathscr{M}$or$_B(E; E')$ (I, p. 45, ví dụ 4) và $\mathscr{F}$ là bó $\mathscr{M}$or$_A(E_A; E'_A)$. Với mọi tập mở V của B và mọi V-cấu xạ $f: E_V\rightarrow E'_V$, đặt $\varphi_V(f) =f_{V\cap A}$, trong đó $f_{V\cap A}$ là $(V\cap A)$-cấu xạ từ $E_{V\cap A}$ vào $E'_{V\cap A}$ cảm sinh bởi $f$. Họ $\varphi = (\varphi_V)$ thu được là một cấu xạ bó từ $\mathscr{G}$ vào $i_*\mathscr{F}$. Theo mệnh đề 4, tồn tại một cấu xạ bó duy nhất $\psi :\mathscr{M}$or$_B(E; E')_A\rightarrow \mathscr{M}$or$_A(E_A; E'_A)$ sao cho ta có

$$
\psi_{V\cap A}(\sigma_{\mathscr{G}}(V, f)|V\cap A) =f_{V\cap A} \tag{12}
$$

với mọi tập mở V của B và mọi $f\in \mathscr{C}_V(E_V; E'_V)$. Cấu xạ $\psi$ được gọi là cấu xạ chính tắc từ $\mathscr{M}$or$_B(E; E')_A$ vào $\mathscr{M}$or$_A(E_A; E'_A)$.

Nếu A thu về một điểm $a$, thì cấu xạ này được đồng nhất với cấu xạ thân tại $a$ của bó $\mathscr{M}$or$_B(E; E')$ lên tập $\mathscr{C}(E_a; E'_a)$.

Chuyển qua các bó con, cấu xạ $\psi$ cảm sinh một cấu xạ chính tắc từ $\mathscr{I}$som$_B(E; E')_A$ vào $\mathscr{I}$som$_A(E_A; E'_A)$.

#### Ví dụ 2 {#ta-i-s3-n8-exa-2 .statement tag=01OM}

Cho A, B, C là các không gian tôpô và cho $u: A\rightarrow B$, $v: B\rightarrow C$ là các ánh xạ liên tục; đặt $w=v\circ u$. Cho E và $E'$ là các C-không gian. Cấu xạ chính tắc từ $\mathscr{M}$or$_C(E; E')_A$ vào $\mathscr{M}$or$_A(E_A; E'_A)$ là hợp thành của cấu xạ $\mathscr{M}$or$_C(E; E')_A\rightarrow \mathscr{M}$or$_B(E_B; E'_B)_A$ suy ra từ cấu xạ chính tắc của $\mathscr{M}$or$_C(E; E')_B$ vào $\mathscr{M}$or$_B(E_B; E'_B)$ và cấu xạ chính tắc của $\mathscr{M}$or$_B(E_B,E'_B)_A$ vào $\mathscr{M}$or$_A(E_A,E'_A)$.

### 9. Bó mềm

#### Định nghĩa 5 {#ta-i-s3-def-5 .statement tag=01ON}

Cho $p: E\rightarrow B$ là một ánh xạ étale. Ta nói rằng ánh xạ $p$ là mềm, hoặc rằng B-không gian étale $(E, p)$ là mềm, nếu mọi tiết diện liên tục của $p$ trên một không gian con đóng của B đều mở rộng được thành một tiết diện liên tục của $p$ trên B.

Cho $\mathscr{F}$ là một bó trên B. Ta nói rằng $\mathscr{F}$ là một bó mềm nếu không gian étale liên kết (I, p. 50, định nghĩa 4) là mềm.

Cho $\mathscr{F}$ là một bó trên B. Bó $\mathscr{F}$ là mềm khi và chỉ khi với mọi Z đóng của B, mọi lân cận mở U của Z và mọi $s\in \mathscr{F}(U)$, tồn tại $t\in \mathscr{F}(B)$ và một lân cận mở V của Z được chứa trong U sao cho $s|V =t|V$.

Nếu $\mathscr{F}$ là một bó mềm thì $\mathscr{F}(B)$ khác rỗng: thật vậy, tiết diện duy nhất của không gian étale $E_{\mathscr{F}}$ liên kết với $\mathscr{F}$ trên $\emptyset$ mở rộng được thành một tiết diện liên tục của $E_{\mathscr{F}}$ trên B.

Cho $p: E\rightarrow B$ là một ánh xạ étale và cho A là một không gian con đóng của B. Nếu $p$ là mềm thì ánh xạ $p_A:\overset{-1}{p}(A)\rightarrow A$ là mềm. Tương đương, nếu $\mathscr{F}$ là một bó mềm trên B thì bó cảm sinh trên một không gian con đóng A là mềm.

#### Mệnh đề 6 {#ta-i-s3-prop-6 .statement tag=01OO}

Cho B là một không gian tôpô, $\mathscr{F}$ là một bó trên B và $(A_i)_{i\in I}$ là một phủ đóng hữu hạn địa phương của B. Để bó $\mathscr{F}$ là mềm, điều kiện cần và đủ là, với mọi $i\in I$, bó cảm sinh $\mathscr{F}_{A_i}$ là mềm.

Điều kiện ấy hiển nhiên là cần. Hãy chứng minh rằng nó là đủ. Ký hiệu bởi $p: E\rightarrow B$ B-không gian étale $E_{\mathscr{F}}$ liên kết với bó $\mathscr{F}$. Cho A là một không gian con đóng của B và $s: A\rightarrow E$ là một tiết diện liên tục của $p$ trên A; vấn đề là chứng minh rằng $s$ có một mở rộng liên tục lên B. Với mọi tập con J của I, đặt $A_J=\bigcup_{i\in J}A_i$; tập hợp $A_J$ là đóng trong B (TG, I, p. 6, mệnh đề 4).

Cho $\mathscr{S}$ là tập hợp các cặp $(J, t)$ trong đó J là một tập con của I và $t$ là một tiết diện liên tục của E trên $A_J$ trùng với $s$ trên $A\cap A_J$. Ta biến $\mathscr{S}$ thành một tập hợp có thứ tự bởi quan hệ thứ tự ký hiệu là $\leqslant$ mà theo đó $(J, t)\leqslant (J', t')$ nếu $J\subset J'$ và $t'|A_J=t$. Với $\sigma = (J, t)\in \mathscr{S}$, ta viết $J_{\sigma}= J$ và $t_{\sigma}=t$. Hãy chỉ ra rằng tập hợp có thứ tự $\mathscr{S}$ là quy nạp. Cho S là một tập con được sắp thứ tự toàn phần của $\mathscr{S}$. Đặt $J =\bigcup_{\sigma\in S}J_{\sigma}$; đây là một tập con của I. Khi đó ta định nghĩa một tiết diện $t$ của E trên $A_J$ bằng cách đặt $t(x) =t_{\sigma}(x)$, nếu $x\in A_{J_{\sigma}}$; do đó $t|A\cap A_J=s$. Cho $j\in J$ và cho $\sigma \in S$ sao cho $j\in J_{\sigma}$; vì $t|A_j=t_{\sigma}|A_j$, hạn chế của $t$ trên $A_j$ là liên tục. Khi đó suy ra từ TG, I, p. 19, Prop. 4 rằng $t$ là liên tục. Vậy, $(J, t)$ là một phần tử của $\mathscr{S}$; theo phép dựng, nó là một cận trên của S. Điều này chứng minh rằng tập hợp $\mathscr{S}$ là quy nạp. Do đó nó có một phần tử cực đại $(J, t)$ (E, III, p. 20, th. 2).

Ta lập luận bằng phản chứng, giả sử rằng J $= I\not$ . Cho $i$ là một phần tử của I-J. Đặt $A'= (A_i\cap A)\cup (A_i\cap A_J)$ và định nghĩa một tiết diện $s'$ của E trên $A'$ bởi:

$'s(a)$ với $a\in A_i\cap A$,

$$
s(a) =
$$

$t(a)$ với $a\in A_i\cap A_J$,

điều này là có thể vì $s$ và $t$ trùng nhau trên $A\cap A_J$. Hơn nữa, vì $A_i\cap A$ và $A_i\cap A_J$ là đóng, nên tiết diện $s'$ là liên tục (TG, I, p. 19, mệnh đề 4). Theo giả thiết, tồn tại một tiết diện liên tục $s_i: A_i\rightarrow E$ kéo dài $s'$. Vì các hạn chế của $s_i$ và $t$ lên $A_J\cap A_i$ là bằng nhau, nên tiết diện liên tục $t': A_{J\cup \{i\}}\rightarrow E$ trùng với $t$ trên $A_J$ và với $s_i$ trên $A_i$ là một tiết diện liên tục của $p$ trên $A_{J\cup \{i\}}$, kéo dài $s|A\cap A_{J\cup \{i\}}$. Khi đó ta có $(J, t)<(J\cup  \{i\}, t')$, điều này mâu thuẫn với giả thiết rằng $(J, t)$ là cực đại.

Vậy, J = I, do đó $A_J= B$ và $t$ là một tiết diện liên tục của E trên B kéo dài $s$.

#### Hệ quả 1 {#ta-i-s3-prop-6-cor-1 .statement tag=01OP}

Cho B là một không gian paracompact, $\mathscr{F}$ một bó trên B và $(U_i)_{i\in I}$ một phủ mở của B. Nếu, với mọi $i\in I$, bó cảm sinh $\mathscr{F}|U_i$ là mềm, thì bó $\mathscr{F}$ là mềm.

Thật vậy, tồn tại một phủ đóng hữu hạn địa phương $(F_j)_{j\in J}$ mịn hơn phủ $(U_i)_{i\in I}$ (TG, IX, p. 49, mệnh đề 4 và p. 48, hệ quả 1). Do đó, với mọi $j\in J$, bó $\mathscr{F}|F_j$ là mềm và mệnh đề suy ra rằng bó $\mathscr{F}$ là mềm.

#### Hệ quả 2 {#ta-i-s3-prop-6-cor-2 .statement tag=01OQ}

Cho B là một không gian paracompact, $\mathscr{F}$ một bó trên B và $(A_i)_{i\in I}$ một phủ đóng hữu hạn địa phương của B. Để bó $\mathscr{F}$ là mềm, điều kiện cần và đủ là điều kiện sau được thỏa mãn:

Với mọi $i\in I$, mọi tập con đóng A của $A_i$, mọi tập mở V của B chứa A và mọi phần tử $s$ của $\mathscr{F}(V)$, tồn tại một lân cận mở U của $A_i$ trong B, một phần tử $t$ của $\mathscr{F}(U)$ và một lân cận mở W của A trong B được chứa trong $U\cap V$ sao cho $t|W =s|W$.

Giả sử rằng bó $\mathscr{F}$ là mềm, và hãy chỉ ra rằng điều kiện được thỏa mãn. Cho $i\in I$, cho A là một tập con đóng của $A_i$, cho V là một tập con mở của B chứa A và cho $s$ là một phần tử của $\mathscr{F}(V)$. Đặt $s_0=\sigma_{\mathscr{F}}(s)$. Đó là một tiết diện liên tục trên V của không gian étalé $E_{\mathscr{F}}$. Vì $A_i$ là đóng, A là đóng trong B và $s_0|A$ kéo dài thành một tiết diện $t_0: B\rightarrow E_{\mathscr{F}}$, theo định nghĩa của một bó mềm. Các tiết diện $s_0$ và $t_0|V$ của không gian étalé trên V $E_{\mathscr{F}}\times_BV$ trùng nhau trên A, nên trùng nhau trên một lân cận W của A (I, p. 34, mệnh đề 11, b)).

Ngược lại, giả sử điều kiện của hệ quả được thỏa mãn. Theo mệnh đề 6, chỉ cần chứng minh rằng, với mọi $i\in I$, bó $\mathscr{F}_{A_i}$ là mềm. Cho A là một tập con đóng của $A_i$ và cho $s_0$ là một tiết diện của không gian étalé của $\mathscr{F}|A_i$ trên A, nghĩa là, một tiết diện liên tục trên A của không gian étalé $E_{\mathscr{F}}$. Vì A đóng trong B và vì B là paracompact, $s_0$ mở rộng thành một tiết diện $s$ trên một lân cận V của A trong B (I, p. 37, đl. 2). Theo giả thiết, tồn tại một lân cận mở U của $A_i$ trong B và một tiết diện $t$ của $E_{\mathscr{F}}$ trên U trùng với $s$ trên một lân cận của A. Hạn chế của $t$ lên $A_i$ là một tiết diện của $\mathscr{F}_{A_i}$ mở rộng $s_0$. Vậy bó $\mathscr{F}_{A_i}$ là mềm. Theo mệnh đề 6, bó $\mathscr{F}$ là mềm.

### 10. Các bó cấu trúc

Giả sử đã cho một Loài cấu trúc Σ và một khái niệm $\sigma$-cấu xạ đối với Loài cấu trúc này.

Cho B là một không gian tôpô.

Một tiền bó $\mathscr{F}$ trên B được gọi là nhận giá trị trong Loài cấu trúc Σ nếu, với mọi tập mở U của B, tập hợp $\mathscr{F}(U)$ được trang bị một cấu trúc thuộc Loài Σ và nếu các ánh xạ hạn chế là các $\sigma$-cấu xạ.

Một tiền bó như thế sẽ được gọi là một bó nhận giá trị trong Loài cấu trúc Σ nếu hơn nữa nó là một bó các tập hợp.

Nếu $\mathscr{F}$ và $\mathscr{G}$ là các tiền bó nhận giá trị trong Loài cấu trúc Σ, một cấu xạ $\varphi$ được gọi là một cấu xạ của các tiền bó nhận giá trị trong Σ nếu, với mọi tập mở U, ánh xạ $\varphi (U)$ là một $\sigma$-cấu xạ.

Do đó, chẳng hạn, người ta nói đến các bó nhóm, các bó nhóm Abel, các bó $k$-môđun (với $k$ là một vành cố định), các bó vành, các bó $k$-đại số (với $k$ là một vành giao hoán cố định).

Bó trên B của các ánh xạ nhận giá trị trong một nhóm (resp. một nhóm Abel, resp. một $k$-môđun, resp. một vành, resp. một $k$-đại số) tự nhiên được trang bị một cấu trúc bó nhóm (resp. bó nhóm Abel, resp. bó $k$-môđun, resp. bó vành, resp. bó $k$-đại số). Nếu X là một đa tạp khả vi cấp $C^r$ trên $\mathbf{R}$, bó $\mathscr{C}^r(X;\mathbf{R})$ các hàm số thực cấp $C^r$ là một bó $\mathbf{R}$-đại số, và bó trên X các tiết diện cấp $C^r$ của một bó vectơ E trên X là một bó các không gian vectơ trên $\mathbf{R}$; một toán tử vi phân xác định một cấu xạ của các bó không gian vectơ trên $\mathbf{R}$.

Đối với các Loài cấu trúc Σ này, suy ra từ phép dựng mà chúng ta đã cho rằng bó $\widetilde{F}$ liên kết với một tiền bó $\mathscr{F}$ nhận giá trị trong Loài cấu trúc Σ (nhóm, nhóm Abel, $k$-môđun, vành, $k$-đại số) là một bó nhận giá trị trong Loài cấu trúc đó, và cấu xạ chính tắc $j_{\mathscr{F}}:\mathscr{F}\rightarrow \widetilde{\mathscr{F}}$ là một cấu xạ của các tiền bó nhận giá trị trong Loài cấu trúc Σ.

Chẳng hạn, bó trên B của các ánh xạ nhận giá trị trong một nhóm tự nhiên được trang bị một cấu trúc bó nhóm.

Cho A và B là các không gian tôpô và cho $u: A\rightarrow B$ là một ánh xạ liên tục. Nếu $\mathscr{F}$ là một (tiền)bó trên A nhận giá trị trong Loài cấu trúc Σ, thì (tiền)bó ảnh trực tiếp $u_*(\mathscr{F})$ của (tiền)bó $\mathscr{F}$ theo $u$ cũng vậy.

Giả sử hơn nữa rằng Loài cấu trúc Σ là loài nhóm, nhóm Abel, $k$-môđun, vành hoặc $k$-đại số. Nếu $\mathscr{G}$ là một (tiền)bó trên B nhận giá trị trong Loài cấu trúc Σ, thì bó $u^*\mathscr{G}$ trên A, ảnh ngược của tiền bó $\mathscr{G}$ bởi ánh xạ $u$, được trang bị một cấu trúc bó nhận giá trị trong Σ. Trong trường hợp này, các cấu xạ phép nối $\alpha$ và $\beta$ là các cấu xạ của những tiền bó nhận giá trị trong Loài cấu trúc Σ. Đặc biệt, nếu $\varphi :\mathscr{G}\rightarrow u_*\mathscr{F}$ là một cấu xạ của những tiền bó nhận giá trị trong Σ, thì cấu xạ $\varphi^{\sharp}$ cũng có tính chất đó; nếu $\psi :u^*(\mathscr{G})\rightarrow \mathscr{F}$ là một cấu xạ của những tiền bó nhận giá trị trong Σ, thì cấu xạ $\psi^{\flat}$ cũng có tính chất đó.

## BÀI TẬP {#ta-i-s3-exercises}

Xem [các bài tập của § 3](exercises/s3/).
