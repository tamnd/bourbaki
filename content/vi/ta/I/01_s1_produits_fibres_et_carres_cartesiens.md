---
book: ta
book_title: Topologie algébrique
chapter: I
chapter_title: REVÊTEMENTS
section: 1
section_title: Produits fibrés et carrés cartésiens
lang: vi
source: ta-i-iv-fr
book_pages: TA I.1-TA I.24, TA I.139
pdf_pages: 0017-0040, 0155-0155
extraction: native
subsections:
    - "no": 1
      title: Structure de B-espace
      page: 1
      pdf_page: 17
    - "no": 2
      title: Opérations sur les B-espaces
      page: 2
      pdf_page: 18
    - "no": 3
      title: Produit fibré de deux B-espaces
      page: 3
      pdf_page: 19
    - "no": 4
      title: Changement de base
      page: 4
      pdf_page: 20
    - "no": 5
      title: Produit fibré d’une famille de B-espaces
      page: 5
      pdf_page: 21
    - "no": 6
      title: Carrés cartésiens
      page: 6
      pdf_page: 22
    - "no": 7
      title: Carrés cartésiens construits par passage aux sous-espaces
      page: 9
      pdf_page: 25
    - "no": 8
      title: Carrés cartésiens construits par produits, produits fibrés et sommes
      page: 11
      pdf_page: 27
    - "no": 9
      title: Composition de carrés cartésiens
      page: 15
      pdf_page: 31
    - "no": 10
      title: Applications strictes
      page: 17
      pdf_page: 33
    - "no": 11
      title: Applications universellement strictes
      page: 20
      pdf_page: 36
statements: 44
exercises: 2
content_sha256: 24550f821f4e09d4b3b6353c9a9f0c6bd9d971dfd8f7c8ea0551389911cd8f39
translated_from: content/en-mt/ta/I/01_s1_produits_fibres_et_carres_cartesiens.md
source_lang: en-mt
translation_method: machine
source_content_sha256: 73da3f125059daba7ca5accf87dc18d7a25a1c3ad2a43b8a6572294c162df91a
translation_model: gpt-5.4
translation_run: translate-vi-86369257
glossary_version: 34
glossary_terms_sha256: 3a902faf7c04333fbadb57166cfa3379022e6f7c7436c69eb3879b81499b20c1
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 1. TÍCH THỚ VÀ CÁC HÌNH VUÔNG DESCARTES

### 1. Cấu trúc của một không gian B

Cho B là một không gian tôpô.

#### Định nghĩa 1 {#ta-i-s1-def-1 .statement tag=01L9}

Một không gian tôpô B (hay đơn giản là một không gian B) là một không gian tôpô X, được trang bị một ánh xạ liên tục $p$ từ X vào B. Ánh xạ $p$ được gọi là phép chiếu của không gian B X.

Cho X, $X'$ là các không gian B và $p,p'$ là các phép chiếu tương ứng của chúng. Một cấu xạ B từ X vào $X'$ là một ánh xạ liên tục $f$ từ X vào $X'$ sao cho $p'\circ f=p$.

Đôi khi thuận tiện khi ký hiệu bởi $(X, p)$ không gian B thu được bằng cách trang bị cho không gian tôpô X ánh xạ liên tục $p$.

Hợp thành của hai cấu xạ B là một cấu xạ B. Các đẳng cấu của các không gian B, cũng gọi là các B-đẳng cấu, là các cấu xạ B đồng thời là các đồng phôi.

Vì vậy, nếu ta gọi một cấu trúc không gian B trên một tập hợp X là dữ kiện của một tôpô trên X và của một ánh xạ liên tục $p: X\rightarrow B$, thì ta có thể lấy các cấu xạ B làm các cấu xạ của cấu trúc không gian B đó (E, IV, p. 11).

© N. Bourbaki and Springer-Verlag Berlin Heidelberg 2  016

N. Bourbaki, Algebraic Topology, DOI 10.1007/978-3-662-49361-8_1  1

Cho X, $X'$ là các không gian B. Ta ký hiệu bởi $\mathscr{C}_B(X; X')$ tập hợp các cấu xạ B từ X vào $X'$, bởi Isom$_B(X; X')$ tập hợp các B-đẳng cấu từ X vào $X'$, và bởi Aut$_B(X)$ tập hợp các B-tự đẳng cấu của X, tức là các B-đẳng cấu từ X vào X.

Cho X là một không gian B và $p$ là phép chiếu của nó. Nếu B được trang bị cấu trúc không gian B có phép chiếu là Id$_B$, thì tập hợp $\mathscr{C}_B(B; X)$ là tập hợp các mặt cắt liên tục (E, II, p. 18, Định nghĩa 11) của $p$.

Cho X là một không gian B, $p$ là phép chiếu của nó và $b$ là một điểm của B. Không gian con $\overset{-1}{p}(b)$ của X được gọi là thớ của X tại $b$ (hay thớ của $p$ tại $b$) và được ký hiệu bởi $X_b$. Để một ánh xạ liên tục $f$ từ X vào một không gian B $X'$ là một cấu xạ B, điều kiện cần và đủ là $f(X_b)$ được chứa trong $X'_b$ với mọi $b\in B$.

Cho X là một không gian B và $p$ là phép chiếu của nó. Cho $f$ là một ánh xạ liên tục từ một không gian tôpô $B'$ vào B. Một ánh xạ liên tục $g: B'\rightarrow X$ sao cho $p\circ g=f$ được gọi là một phép nâng liên tục của $f$ lên X. Nói cách khác, nếu $B'$ được trang bị cấu trúc không gian B có phép chiếu là $f$, thì các phép nâng liên tục của $f$ lên X là các cấu xạ B từ $B'$ vào X.

### 2. Các phép toán trên các không gian B

Cho B là một không gian tôpô.

Cho X là một không gian B và $p$ là phép chiếu của nó. Mọi không gian con tôpô Y của X đều được trang bị cấu trúc không gian B có phép chiếu là $p|Y$. Cho A là một không gian con của B; khi được trang bị ánh xạ $p_A:\overset{-1}{p}(A)\rightarrow A$ suy ra từ $p$ bằng cách chuyển qua các tập con, không gian tôpô $\overset{-1}{p}(A)$ là một không gian A. Nó được gọi là không gian A cảm sinh bởi $(X, p)$ trên A và đôi khi được ký hiệu bởi $X_A$.

Cho $(X_i)_{i\in I}$ là một họ các không gian B, và $p_i$ là phép chiếu của $X_i$. Không gian tổng $X =\coprod_{i\in I}X_i$ (TG, I, p. 15), được trang bị ánh xạ $p: X\rightarrow$ B xác định bởi $p(i, x) =p_i(x)$ (với $i\in$ I và $x\in X_i$), là một không gian B gọi là tổng của họ các không gian B $(X_i)_{i\in I}$. Các đơn cấu chính tắc $X_i\rightarrow X$ là các cấu xạ B.

Cho X là một B-không gian, $p$ là phép chiếu của nó, và cho R là một quan hệ tương đương trên X. Ta ký hiệu bởi $X/R$ không gian thương (TG, I, p. 20, def. 3). Nếu ánh xạ $p: X\rightarrow B$ tương thích với quan hệ R (E, II, p. 44), thì ánh xạ $p': X/R\rightarrow B$ suy ra từ $p$ bằng cách chuyển qua thương là liên tục (TG, I, p. 21, prop. 6); khi đó B-không gian thu được bằng cách trang bị cho $X/R$ phép chiếu $p'$ được gọi là B-không gian thương của X theo quan hệ R.

### 3. Tích thớ của hai B-không gian

Cho B là một không gian tôpô, X và $X'$ là các B-không gian, $p$ và $p'$ là các phép chiếu tương ứng của chúng. Ta ký hiệu bởi $X\times_BX'$ không gian con tôpô của $X\times X'$ tạo bởi các cặp $(x, x')$ sao cho $p(x) =p'(x')$. Ánh xạ $q: X\times_BX'\rightarrow B$ xác định bởi $q(x, x') =p(x)$ là liên tục.

#### Định nghĩa 2 {#ta-i-s1-def-2 .statement tag=01LA}

Không gian tôpô $X\times_BX'$ được gọi là tích thớ của X và $X'$ trên B. B-không gian thu được bằng cách trang bị cho $X\times_BX'$ ánh xạ $q$ được gọi là B-không gian tích của X và $X'$.

Các hạn chế lên $X\times_BX'$ của các phép chiếu từ $X\times X'$ lên X và lên $X'$ vẫn được ký hiệu bởi pr$_1$ và pr$_2$ và được gọi là phép chiếu thứ nhất và thứ hai của tích thớ. Chúng là liên tục và là các B-cấu xạ, vì ta có $q=p\circ$ pr$_1=p'\circ$ pr$_2$.

Cần lưu ý rằng $X\times_BX'$ có thể rỗng ngay cả khi X và $X'$ không rỗng: thật vậy, hệ thức $X\times_BX'=\emptyset$ tương đương với việc nói rằng $p(X)$ và $p'(X')$ rời nhau.

Cho Y là một B-không gian và $u: Y\rightarrow X,u': Y\rightarrow X'$ là các B-cấu xạ. Tồn tại một B-cấu xạ duy nhất $v: Y\rightarrow X\times_BX'$ sao cho pr$_1\circ v=u$ và pr$_2\circ v$ = $u'$ (tính chất phổ quát của B-không gian tích của hai B-không gian): đó là ánh xạ $y\mapsto (u(y), u'(y))$ từ Y vào $X\times_BX'$, đôi khi được ký hiệu bởi $(u, u')$.

Cho $X,X',Y,Y'$ là các B-không gian, cho $f: X\rightarrow Y,f': X'\rightarrow Y'$ là các B-cấu xạ. Ánh xạ $(x, x')\mapsto (f(x), f'(x'))$ là một B-cấu xạ từ $X\times_BX'$ vào $Y\times_BY'$, được ký hiệu bởi $f\times_Bf'$ và được gọi là mở rộng của $f$ và $f'$ lên các tích thớ.

#### Ví dụ 1 {#ta-i-s1-n3-exa-1 .statement tag=01LB}

Cho X và $X'$ là các B-không gian; khi đó ánh xạ $(x, x')\mapsto (x', x)$ xác định một B-đẳng cấu từ $X\times_BX'$ lên $X'\times_BX$.

#### Ví dụ 2 {#ta-i-s1-n3-exa-2 .statement tag=01LC}

Cho X, $X',X''$ là các B-không gian và $p,p',p''$ là các phép chiếu tương ứng của chúng. B-không gian tích $(X\times_BX')\times_BX''$ là không gian con tôpô $X\times_BX'\times_BX''$ của $X\times X'\times X''$ gồm các bộ ba $(x, x', x'')$ sao cho $p(x) =p'(x') =p''(x'')$, được trang bị phép chiếu $q: X\times_BX'\times_BX''\rightarrow B$ xác định bởi $q(x, x', x'') =p(x)$.

#### Ví dụ 3 {#ta-i-s1-n3-exa-3 .statement tag=01LD}

Cho X là một B-không gian và $p$ là phép chiếu của nó. Tích thớ $X\times_BX$ của X với chính nó trên B được gọi là bình phương thớ của X. Đó là không gian con của $X\times X$ gồm các cặp $(x, x')$ sao cho $p(x) =p(x')$. Nó được trang bị cấu trúc của một B-không gian mà phép chiếu là ánh xạ $(x, x')\mapsto$ $p(x)$. Đường chéo $\Delta_X$ của $X\times X$ (E, II, p. 13) được chứa trong $X\times_BX$; nó cũng được gọi là đường chéo của $X\times_BX$. Ánh xạ $x\mapsto (x, x)$ từ X vào $X\times_BX$ là một B-cấu xạ, gọi là B-cấu xạ đường chéo và thường được ký hiệu bởi $\delta_X$; nó xác định một B-đẳng cấu từ X lên $\Delta_X$ (TG, I, p. 25, cor. 2).

#### Ví dụ 4 {#ta-i-s1-n3-exa-4 .statement tag=01LE}

Cho $(B_i)_{i\in I}$ là một họ các không gian tôpô và, với mỗi $i\in I$, cho $(X_i, p_i)$ và $(Y_i, q_i)$ là các $B_i$-không gian. Đặt $B =\prod_{i\in I}B_i$, $X =\prod_{i\in I}X_i$ và $Y =\prod_{i\in I}Y_i$. Khi được trang bị ánh xạ liên tục $p=\prod_ip_i$ (tương ứng $q=\prod_iq_i$), không gian tôpô X (tương ứng Y) là một B-không gian. Theo đẳng cấu tính kết hợp của các tích tôpô từ $\prod_i(X_i\times Y_i)$ lên $(\prod_iX_i)\times (\prod_iY_i) = X\times Y$ (TG, I, p. 25, prop. 2), không gian con $\prod_i(X_i\times_{B_i}Y_i)$ của $\prod_i(X_i\times Y_i)$ được đồng nhất với $X\times_BY$.

#### Ví dụ 5 {#ta-i-s1-n3-exa-5 .statement tag=01LF}

Cho $(X_i)_{i\in I}$ và $(Y_j)_{j\in J}$ là các họ B-không gian. Gọi X và Y là các tổng của chúng. Với mỗi $(i, j)\in I\times J$, ánh xạ $(x, y)\mapsto$ $((i, x),(j, y))$ là một B-đẳng cấu từ $X_i\times_BY_j$ lên không gian con $(\{i\} \times X_i)\times_B(\{j\} \times Y_j)$ của $X\times_BY$. Vì các không gian sau này tạo thành một phân hoạch của $X\times_BY$ thành các tập mở, nên ánh xạ

$$
h:\coprod_{(i,j)\in I\times J}(X_i\times_BY_j)\rightarrow X\times_BY
$$

xác định bởi $h((i, j),(x, y)) = ((i, x),(j, y))$ là một B-đẳng cấu.

### 4. Thay đổi cơ sở

Cho B, $B'$ là các không gian tôpô và $f: B'\rightarrow B$ là một ánh xạ liên tục. Cho X là một B-không gian. Ánh xạ $f$ trang bị cho $B'$ một cấu trúc B-không gian, điều này cho phép định nghĩa tích thớ $B'\times_BX$. Không gian sau, được trang bị ánh xạ pr$_1: B'\times_BX\rightarrow B'$, là một $B'$-không gian gọi là $B'$-không gian suy ra từ B-không gian X bởi phép thay đổi cơ sở $f: B'\rightarrow B$ (hoặc bởi phép thay đổi cơ sở từ B sang $B'$ theo $f$). Nó cũng được gọi là $B'$-không gian ảnh ngược của X bởi $f$. Nó được ký hiệu bởi $f^*(X)$, hoặc đôi khi bởi $X_{B'}$ khi không thể có sự nhầm lẫn nào về ánh xạ $f$.

Khi $B'$ là một không gian con của B và $f: B'\rightarrow B$ là đơn ánh chính tắc, ánh xạ $(b', x)\mapsto x$ từ $B'\times_BX'$ vào $\overset{-1}{p}(B')$ (trong đó $p$ là phép chiếu của X) là một $B'$-đẳng cấu của $f^*(X)$ lên $B'$-không gian cảm sinh bởi X trên $B'$.

Cho Y là một B-không gian thứ hai và $u: X\rightarrow Y$ là một B-cấu xạ. Ánh xạ Id$_{B'}\times_Bu: B'\times_BX\rightarrow B'\times_BY$ là một $B'$-cấu xạ, gọi là $B'$-cấu xạ suy ra từ B-cấu xạ $u$ bởi phép thay đổi cơ sở $f: B'\rightarrow B$ và đôi khi được ký hiệu bởi $f^*(u)$, hoặc $u_{B'}$ khi không thể có sự nhầm lẫn nào về ánh xạ $f$. Nó là $B'$-cấu xạ duy nhất $v$ từ $B'\times_BX$ vào $B'\times_BY$ sao cho pr$_2\circ v=u\circ$ pr$_2$.

Cho $B''$ là một không gian tôpô và cho $g: B''\rightarrow B'$ là một ánh xạ liên tục. Khi đó ánh xạ cho bởi $(b'',(b', x))\mapsto (b'', x)$ là một đẳng cấu các $B''$-không gian từ $g^*(f^*(X))$ lên $(f\circ g)^*(X)$, và sẽ được gọi là chính tắc.

### 5. Tích thớ của một họ các B-không gian

Cho $(X_i)_{i\in I}$ là một họ các B-không gian. Cho $p_i: X_i\rightarrow B$ là các phép chiếu của chúng. Ký hiệu $\prod_BX_i$ là không gian con tôpô của $B\times \prod_{i\in I}X_i$ tạo bởi các cặp $(b,(x_i)_{i\in I})$ sao cho $p_i(x_i) =b$ với mọi $i\in I$. Ánh xạ $p:\prod_BX_i\rightarrow B$ được định nghĩa bởi $p(b,(x_i)_{i\in I}) =b$ là liên tục.

#### Định nghĩa 3 {#ta-i-s1-def-3 .statement tag=01LG}

Không gian tôpô $\prod_BX_i$ được gọi là tích thớ của họ $(X_i)_{i\in I}$ trên B. B-không gian thu được bằng cách trang bị cho $\prod_BX_i$ ánh xạ $p$ được gọi là B-không gian tích của họ $(X_i)_{i\in I}$.

Cho $j\in I$. Ánh xạ $(b, x)\mapsto$ pr$_j(x)$ từ $\prod_BX_i$ vào $X_j$ được gọi là phép chiếu có chỉ số $j$ của tích thớ và lại được ký hiệu là pr$_j$. Nó liên tục. Nó là một B-cấu xạ, vì ta có $p=p_j\circ$ pr$_j$.

Cho Y là một B-không gian và $q$ là phép chiếu của nó. Với mỗi $i\in$ I, cho $u_i: Y\rightarrow X_i$ là một B-cấu xạ. Tồn tại một B-cấu xạ duy nhất $v: Y\rightarrow$ $\prod_BX_i$ sao cho pr$_i\circ v=u_i$ với mỗi $i\in I$ (tính chất phổ quát của B-không gian tích): đó là ánh xạ từ Y vào $\prod_BX_i$, được xác định bởi $y\mapsto (q(y),(u_i(y))_{i\in I})$, đôi khi được ký hiệu là $(u_i)_{i\in I}$.

Cho $(X_i)_{i\in I}$ và $(Y_i)_{i\in I}$ là các họ B-không gian và, với mỗi $i\in I$, cho $f_i: X_i\rightarrow Y_i$ là một B-cấu xạ. Ánh xạ $(b,(x_i)_{i\in I})\mapsto$ $(b,(f_i(x_i))_{i\in I})$ là một B-cấu xạ từ $\prod_BX_i$ vào $\prod_BY_i$, được ký hiệu là $\prod_Bf_i$ và được gọi là phép mở rộng của họ $(f_i)_{i\in I}$ tới các tích thớ.

#### Ví dụ 1 {#ta-i-s1-n5-exa-1 .statement tag=01LH}

Khi tập hợp I là rỗng, tập hợp $\prod_{i\in I}X_i$ chỉ gồm một phần tử duy nhất và B-không gian $\prod_BX_i$ được đồng nhất với B (được trang bị phép chiếu Id$_B$).

#### Ví dụ 2 {#ta-i-s1-n5-exa-2 .statement tag=01LI}

Khi I không rỗng, từ ánh xạ $(b, x)\mapsto x$ từ $B\times \prod_{i\in I}X_i$ vào $\prod_{i\in I}X_i$, bằng cách chuyển qua các không gian con, suy ra một đồng phôi từ $\prod_BX_i$ lên không gian con của $\prod_{i\in I}X_i$ tạo bởi các họ $(x_i)_{i\in I}$ sao cho $p_i(x_i) =p_j(x_j)$ với mọi $i, j\in I$. Không gian con này sẽ được gọi, theo lối nói lạm dụng, là tích thớ của họ $(X_i)_{i\in I}$.

#### Ví dụ 3 {#ta-i-s1-n5-exa-3 .statement tag=01LJ}

Khi tập hợp I là một tập hợp chỉ có một phần tử $\alpha$ (resp. có hai phần tử $\alpha$ và $\beta$; resp. có ba phần tử $\alpha ,\beta ,\gamma$ ), ánh xạ pr$_{\alpha}$ (resp. (pr$_{\alpha}$, pr$_{\beta}$) ; resp. (pr$_{\alpha}$, pr$_{\beta}$, pr$_{\gamma}$)) từ $\prod_BX_i$ vào $X_{\alpha}$ (resp. vào $X_{\alpha}\times_BX_{\beta}$; resp. vào $X_{\alpha}\times_BX_{\beta}\times_BX_{\gamma}$) là một B-đẳng cấu. Điều này sẽ cho phép chúng ta suy ra các tính chất của tích thớ của hai hay ba B-không gian từ các tính chất của tích thớ của các họ B-không gian.

Cho $(X_i)_{i\in I}$ là một họ các B-không gian và J là một tập con của I. Từ ánh xạ Id$_B\times$ pr$_J$ của $B\times \prod_{i\in I}X_i$ vào $B\times \prod_{i\in J}X_i$, bằng cách chuyển qua các tập con, suy ra một B-cấu xạ $\prod_{i\in IB}X_i\rightarrow \prod_{i\in JB}X_i$. Người ta

vẫn ký hiệu nó là pr$_J$ và gọi nó là phép chiếu chỉ số J của tích thớ.

Cho $(X_i)_{i\in I}$ là một họ các B-không gian. Cho $(J_{\lambda})_{\lambda\in L}$ là một phân hoạch

của I. Ánh xạ (pr$_{J_{\lambda}}$)$_{\lambda\in L}$ của $\prod_{i\in IB}X_i\rightarrow \prod_{\lambda\in LB}(\prod_{i\in J_{\lambda}B}X_i)$ là một

B-đẳng cấu ("tính kết hợp" của các tích thớ của các B-không gian).

### 6. Hình vuông Cartesian

Cho B, $B'$, X, $X'$ là các không gian tôpô và cho $f: B'\rightarrow B$, $f': X'\rightarrow X,p: X\rightarrow B,p': X'\rightarrow B'$ là các ánh xạ liên tục. Một bộ bốn $(f, f', p, p')$ như vậy có thể được biểu diễn bằng một biểu đồ

${X'}^{f'}$ X

$$
p'p \tag{1}
$$

${B'}^f$ B

(E, II, p. 14). Khi đó người ta nói: "Xét biểu đồ hình vuông (1)," hoặc đơn giản là "hình vuông (1)," thay vì nói: "Xét bộ bốn $(f, f', p, p')$ các ánh xạ liên tục." Người ta nói rằng hình vuông (1) là giao hoán nếu đẳng thức

$$
f\circ p'=p\circ f'
$$

được thỏa mãn. Trong trường hợp này, người ta thường trang bị cho $B'$, X và $X'$ các cấu trúc B-không gian lần lượt được xác định bởi các ánh xạ $f,p$ và $f\circ p'=p\circ f'$; khi đó các ánh xạ $p'$ và $f'$ là các B-cấu xạ.

#### Định nghĩa 4 {#ta-i-s1-def-4 .statement tag=01LK}

Người ta nói rằng hình vuông (1) là một hình vuông Cartesian của các không gian tôpô (hoặc, đơn giản, rằng nó là Cartesian) nếu nó giao hoán và nếu, với mọi không gian tôpô Y và mọi cặp ánh xạ liên tục $u: Y\rightarrow B',v: Y\rightarrow X$ sao cho $f\circ u=p\circ v$, tồn tại duy nhất một ánh xạ liên tục $w: Y\rightarrow X'$ sao cho $p'\circ w=u$ và $f'\circ w=v$.

Để hình vuông (1) là Cartesian, điều kiện cần và đủ là hình vuông

$$
{X'}^{p'}B'
$$

$$
(1')f'f
$$

X $^p$ B

là Cartesian.

#### Mệnh đề 1 {#ta-i-s1-prop-1 .statement tag=01LL}

Để hình vuông (1) là Cartesian, điều kiện cần và đủ là nó giao hoán và rằng, với mọi B-không gian Y và mọi cặp B-cấu xạ $u: Y\rightarrow B',v: Y\rightarrow X$, tồn tại duy nhất một B-cấu xạ $w: Y\rightarrow X'$ sao cho $p'\circ w=u$ và $f'\circ w=v$.

Giả sử hình vuông (1) là Cartesian. Cho Y là một B-không gian và cho $u: Y\rightarrow B',v: Y\rightarrow X$ là các B-cấu xạ. Các ánh xạ $f\circ u$ và $p\circ v$ đều bằng phép chiếu của B-không gian Y; khi đó ánh xạ liên tục duy nhất $w$ sao cho $p'\circ w=u$ và $f'\circ w=v$ là một B-cấu xạ. Điều này chứng minh tính cần thiết của điều kiện.

Ngược lại, giả sử điều kiện này được thỏa mãn. Cho Y là một không gian tôpô và cho $u: Y\rightarrow B',v: Y\rightarrow X$ là các ánh xạ liên tục sao cho $f\circ u=p\circ v$. Khi Y được trang bị cấu trúc của một B-không gian được xác định bởi $f\circ u$, $u$ và $v$ là các B-cấu xạ. Mọi ánh xạ liên tục $w: Y\rightarrow X'$ sao cho $p'\circ w=u$ và $f'\circ w=v$ đều là một B-cấu xạ, nên tồn tại một và chỉ một ánh xạ như vậy.

#### Mệnh đề 2 {#ta-i-s1-prop-2 .statement tag=01LM}

Cho B, $B'$ và X là các không gian tôpô và cho $p: X\rightarrow B,f: B'\rightarrow B$ là các ánh xạ liên tục.

a) Hình vuông

$B'\times_BX^{pr_2}$ X

(2) pr$_{_1}p$

${B'}^f$ B

là một hình vuông Cartesian.

b) Với mọi hình vuông giao hoán

${X'}^{f'}$ X

$$
p'p \tag{3}
$$

${B'}^f$ B

tồn tại một ánh xạ liên tục duy nhất $h: X'\rightarrow B'\times_BX$ sao cho pr$_1\circ h=p'$ và pr$_2\circ h=f'$.

c) Hình vuông giao hoán (3) là cartesian khi và chỉ khi $h$ là một đồng phôi.

Mệnh đề a) suy ra từ Mệnh đề 1 và từ tính chất phổ quát của B-không gian tích của hai B-không gian (I, p. 3). Mệnh đề b) suy ra từ đó.

Nếu hình vuông (3) là cartesian, thì tồn tại một ánh xạ liên tục duy nhất $h': B'\times_BX\rightarrow X'$ sao cho $f'\circ h'$ = pr$_2$ và $p'\circ h'=$ pr$_1$. Ta có $f'\circ h'\circ h=f'$ và $p'\circ h'\circ h=p'$, do đó $h'\circ h=$ Id$_{X'}$ vì hình vuông (3) là cartesian. Ta có pr$_1\circ h\circ h'$ = pr$_1$ và pr$_2\circ h\circ h'$ = pr$_2$, do đó $h\circ h'=$ Id$_{B'\times_BX}$ vì hình vuông (2) là cartesian. Điều này chứng minh rằng $h$ là một đồng phôi.

Ngược lại, giả sử rằng $h$ là một đồng phôi; vì hình vuông (2) là cartesian, hình vuông (3) cũng là cartesian.

Ánh xạ $h: X'\rightarrow B'\times_BX$ mà sự tồn tại và tính duy nhất được khẳng định trong mệnh đề b) của mệnh đề trước sẽ được gọi là chính tắc: đó là ánh xạ được ký hiệu bởi $(p', f')$ trong I, p. 3.

#### Mệnh đề 3 {#ta-i-s1-prop-3 .statement tag=01LN}

Cho

${X'}^{f'}$ X

$p'p$

${B'}^f$ B

là một hình vuông cartesian. Với mọi tiết diện liên tục $s$ của $p'$, ánh xạ $f'\circ s$ là một phép nâng liên tục của $f$ vào X. Ánh xạ $s\mapsto f'\circ s$ là một song ánh từ $\mathscr{C}_{B'}(B'; X')$ lên $\mathscr{C}_B(B'; X)$.

Nếu $s: B'\rightarrow X'$ là một tiết diện liên tục của $p'$, ta có $p\circ f'\circ s=$ $f\circ p'\circ s=f$, điều này chứng minh rằng $f'\circ s$ là một phép nâng liên tục của $f$ vào X, tức là một B-cấu xạ từ $B'$ vào X. Ngược lại, cho $g: B'\rightarrow X$ là một B-cấu xạ. Ta có $f\circ$ Id$_{B'}=p\circ g$; do đó, theo định nghĩa của một hình vuông cartesian, tồn tại một ánh xạ liên tục duy nhất $s: B'\rightarrow X'$ sao cho $p'\circ s=$ Id$_{B'}$ và $f'\circ s=g$, do đó suy ra mệnh đề.

### 7. Các hình vuông cartesian được xây dựng bằng cách chuyển qua các không gian con

#### Mệnh đề 4 {#ta-i-s1-prop-4 .statement tag=01LO}

Cho

${X'}^{f'}$ X

$$
p'p \tag{4}
$$

${B'}^f$ B

là một hình vuông cartesian, và cho $B_0,B'_0,X_0$ là các không gian con của B, $B'$ và X tương ứng. Giả sử rằng ta có $f(B'_0)\subset B_0,p(X_0)\subset B_0$ và đặt $X'_0=(\overset{-1}{p}')(B'_0)\cap (\overset{-1}{f}')(X_0)$. Khi đó hình vuông

$$
{X'_0}^{f'_0}X_0
$$

$$
(4')p'_{_0}p_{_0}
$$

$$
{B'_0}^{f_0}B_0
$$

(trong đó các ánh xạ $f_0,f'_0,p_0,p'_0$ được suy ra từ $f,f',p,p'$ tương ứng bằng cách chuyển qua các tập con) là cartesian.

Xét ánh xạ chính tắc $h: X'\rightarrow B'\times_BX$ suy ra từ biểu đồ giao hoán (4). Vì hình vuông (4) là Descartes, $h$ là một

đồng phôi. Theo phép dựng, ta có $X'_0=\overset{-1}{h}(B'_0\times_{B_0}X_0)$ và ánh xạ $h_0: X'_0\rightarrow B'_0\times_{B_0}X_0$ suy ra từ biểu đồ giao hoán ($4'$) được suy ra từ $h$ bằng cách chuyển qua các tập con. Do đó nó là một đồng phôi và hình vuông ($4'$) là Descartes (Mệnh đề 2).

#### Hệ quả {#ta-i-s1-n7-cor-1 .statement tag=01LP}

Cho

${X'}^{f'}$ X

$p'p$

${B'}^f$ B

là một hình vuông Descartes.

a) Với mọi điểm $b'$ của $B'$, ánh xạ $f'$ cảm sinh một đồng phôi từ thớ $X'_{b'}$ của $p'$ lên thớ $X_{f(b')}$ của $p$.

b) Nếu ánh xạ $p$ là đơn ánh (tương ứng, toàn ánh, tương ứng, song ánh), thì $p'$ cũng vậy.

Cho $b'$ là một điểm của $B'$. Đặt $b=f(b')$. Với mọi $x'\in X'_{b'}$, ta có $p(f'(x')) =f(p'(x')) =f(b') =b$, do đó $f'(x')\in X_b$. Điều này chứng minh rằng

ta có $X'_{b'}\subset (\overset{-1}{f}')(X_b)$. Trong Mệnh đề 4, lấy $B_0=\{b\},B'_0=\{b'\}$ và $X_0= X_b$; khi đó ta có $X'_0= X'_{b'}$, do đó suy ra mệnh đề a).

Để ánh xạ $p$ là đơn ánh (tương ứng, toàn ánh, tương ứng, song ánh), điều kiện cần và đủ là lực lượng của mỗi thớ của nó nhỏ hơn 1 (tương ứng, lớn hơn 1, tương ứng, bằng 1). Mệnh đề b) suy ra từ đó.

#### Ví dụ {#ta-i-s1-n7-exa-1 .statement tag=01LQ}

Cho $(X, p)$ là một B-không gian và A là một không gian con của B. Hình vuông

$\overset{-1}{p}(A)^j$ X

$$
p_{_A}p \tag{5}
$$

A $^i$ B

(trong đó $i$ và $j$ là các đơn ánh chính tắc) là Descartes.

Đặc biệt, nếu A và $A'$ là các không gian con của không gian tôpô B, thì hình vuông

$$
A\cap A'A'
$$

(6)

A B

(trong đó các mũi tên là các đơn ánh chính tắc) là Descartes.

### 8. Các hình vuông Descartes được dựng bởi tích, tích thớ và tổng

#### Mệnh đề 5 {#ta-i-s1-prop-5 .statement tag=01LR}

Cho I là một tập hợp và, với mỗi $i\in I$, cho

$$
{X'_i}^{f'_i}X_i
$$

$$
p'_{_i}p_{_i} \tag{7}
$$

$$
{B'_i}^{f_i}B_i
$$

là một hình vuông Descartes. Hình vuông

$$
\prod i\in IX'if'\prod i\in IXi
$$

$$
(7')p'p
$$

$$
\prod i\in IB'if\prod i\in IBi
$$

(trong đó $f,f',p,p'$ là các mở rộng của các họ $(f_i)$, $(f'_i)$, $(p_i)$, $(p'_i)$ lên các tích) là Descartes.

Cho Y là một không gian tôpô, cho $u: Y\rightarrow \prod_iB'_i$ và $v: Y\rightarrow \prod_iX_i$ là các ánh xạ liên tục sao cho $f\circ u=p\circ v$. Với $i\in I$, đặt $u_i$ = pr$_i\circ u$ và $v_i=$ pr$_i\circ v$; ta có $f_i\circ u_i=p_i\circ v_i$ và tồn tại một ánh xạ liên tục duy nhất $w_i: Y\rightarrow X'_i$ sao cho $p'_i\circ w_i=u_i$ và $f'_i\circ w_i=v_i$. Khi đó ánh xạ $w= (w_i)$ là một ánh xạ liên tục từ Y vào $\prod_iX'_i$ sao cho $p'\circ w=u$ và $f'\circ w=v$, và đó là ánh xạ duy nhất có các tính chất này.

#### Hệ quả 1 {#ta-i-s1-prop-5-cor-1 .statement tag=01LS}

Cho X là một B-không gian, cho $p$ là phép chiếu của nó, và cho F là một không gian tôpô. Bình phương

$$\begin{array}{ccc} X\times F & \overset{\mathrm{pr}_1}{\longrightarrow} & X \\ {\scriptstyle p\times \mathrm{Id}_F}\big\downarrow & & \big\downarrow{\scriptstyle p} \\ B\times F & \overset{\mathrm{pr}_1}{\longrightarrow} & B \end{array} \tag{8}$$

là Đề-các.

Cho P là một không gian tôpô gồm một điểm duy nhất. Hệ quả 1 suy ra từ Mệnh đề 5 áp dụng cho các bình phương Đề-các

$$\begin{array}{ccccccc} X & \overset{\mathrm{Id}_X}{\longrightarrow} & X & & F & \longrightarrow & P \\ {\scriptstyle p}\big\downarrow & & \big\downarrow{\scriptstyle p} & \text{và} & {\scriptstyle \mathrm{Id}_F}\big\downarrow & & \big\downarrow{\scriptstyle \mathrm{Id}_P} \\ B & \overset{\mathrm{Id}_B}{\longrightarrow} & B & & F & \longrightarrow & P \end{array}.$$

Cho B và $B'$ là các không gian tôpô và cho $f: B'\rightarrow$ B là một ánh xạ liên tục. Cho I là một tập hợp và, với mỗi $i\in I$, cho $X_i$ là một B-không gian, $X'_i$ là một $B'$-không gian, và $f'_i: X'_i\rightarrow X_i$ là một ánh xạ liên tục sao cho bình phương

$$
{X'_i}^{f'_i}X_i
$$

(9)

${B'}^f$ B

giao hoán. Tồn tại một ánh xạ liên tục duy nhất

$$
f':\prod_{i\in IB'}X'_i\rightarrow \prod_{i\in IB}X_i
$$

sao cho pr$_i\circ f'=f'_i\circ$ pr$_i$ với mọi $i\in I$ và sao cho bình phương

$i\prod\in IB'X'if'i\prod\in I$B $Xi$

$$
(9')
$$

${B'}^f$ B giao hoán (điều kiện sau cùng này suy ra từ các điều kiện kia nếu I $=\not\emptyset$ ) $:$ đó là ánh xạ suy ra từ ánh xạ

$$
f\times \prod_{i\in I}f'_i: B'\times \prod_{i\in I}X'_i\rightarrow B\times \prod_{i\in I}X_i
$$

bằng cách chuyển qua các tập con. Với các ký hiệu này:

#### Hệ quả 2 {#ta-i-s1-prop-5-cor-2 .statement tag=01LT}

Nếu bình phương (9) là Đề-các với mọi $i\in I$, thì bình phương ($9'$) là Đề-các.

Từ Mệnh đề 5 suy ra một bình phương Đề-các

$$
B'\times \prod_i{X'_i}^{Id_B\times}\prod_{_i}^{f'_i}B\times \prod_iX_i
$$

$$
B'\times (B')^{If\times}\prod_{_i}^fB\times B^I
$$

Cho $\Delta_{B'}$ và $\Delta_B$ ký hiệu các đường chéo của $B'\times (B')^I$ và $B\times B^I$. Biểu đồ

$i\prod\in IB'X'if'i\prod\in I$B $Xi$

$$
\Delta_{B'}\Delta_B
$$

suy ra từ biểu đồ đứng trước bằng cách chuyển qua các không gian con là Đề-các (I, p. 9, Mệnh đề 4). Nó được đồng nhất với biểu đồ ($9'$).

#### Ví dụ 1 {#ta-i-s1-n8-exa-1 .statement tag=01LU}

Cho

${X'}^{f'}$ X

$p'p$

${B'}^f$ B

là một bình phương Đề-các. Khi đó Hệ quả 2 cho một bình phương Đề-các

$$
X'\times_{B'}{X'}^{\varphi}X\times_BX
$$

${B'}^f$ B .

Ta có quan hệ $\overset{-1}{\varphi}(\Delta_X) = \Delta_{X'}$. Thật vậy, theo mệnh đề 2 của I, p. 8, chỉ cần xét trường hợp $X'= B'\times_BX$. Khi đó, cho $((b, x),(b, x'))$ là một phần tử của $X'\times_{B'}X'$ với $b\in B'$ và $x, x'\in X$. Phần tử này thuộc $\overset{-1}{\varphi}(\Delta_X)$ khi và chỉ khi $x=x'$.

#### Mệnh đề 6 {#ta-i-s1-prop-6 .statement tag=01LV}

Cho I là một tập hợp và, với mọi $i\in I$, cho

${X'_i}^{f'_i}$ X

$$
p'_{_i}p \tag{10}
$$

${B'_i}^{f_i}$ B

là một hình vuông cartesian. Cho $X'$ và $B'$ lần lượt là các không gian tổng của các họ $(X'_i)$ và $(B'_i)$. Cho $f: B'\rightarrow B,f': X'\rightarrow X$ và $p': X'\rightarrow B'$ là các ánh xạ suy ra từ các họ $(f_i)$, $(f'_i)$ và $(p'_i)$ tương ứng. Hình vuông

${X'}^{f'}$ X

$$
(10')p'p
$$

${B'}^f$ B

là cartesian.

Các ánh xạ $f,f'$ và $p'$ là liên tục. Tính giao hoán của hình vuông ($10'$) suy ra từ định nghĩa của nó. Ký hiệu $h_i$ là phép đồng phôi chính tắc từ $X'_i$ lên $B'_i\times_BX$ (I, p. 8, mệnh đề 2) và $h: X'\rightarrow B'\times_BX$ là ánh xạ chính tắc (đd.). Ta có $h=h''\circ h'$ trong đó $h': X'\rightarrow \coprod(B'_i\times_BX)$ là phép đồng phôi suy ra từ các $h_i$ và $h'':\coprod(B'_i\times_BX)\rightarrow (\coprod B'_i)\times_BX$ là ánh xạ được định nghĩa trong ví dụ 5 của I, p. 4. Ta kết luận nhờ mệnh đề 2 của I, p. 8.

#### Ví dụ 2 {#ta-i-s1-n8-exa-2 .statement tag=01LW}

Cho $(X, p)$ là một B-không gian và cho $(A_k)_{k\in K}$ là một họ các không gian con của B. Cho A là không gian tổng của họ $(A_k)_{k\in K}$ và cho Y là không gian tổng của họ $(\overset{-1}{p}(A_k))_{k\in K}$; ký hiệu $i: A\rightarrow B$, $j: Y\rightarrow X$ và $p': Y\rightarrow A$ là các ánh xạ suy ra từ các đơn ánh chính tắc của $A_k$ vào B, các đơn ánh chính tắc của $\overset{-1}{p}(A_k)$ vào X, và các ánh xạ $p_{A_k}:\overset{-1}{p}(A_k)\rightarrow A_k$, với $k\in K$. Hình vuông

Y $^j$ X

$$
p'p \tag{11}
$$

A $^i$ B là cartesian; điều này suy ra từ ví dụ ở I, p. 10 và từ mệnh đề 6.

### 9. Hợp thành của các hình vuông cartesian

#### Mệnh đề 7 {#ta-i-s1-prop-7 .statement tag=01LX}

Cho

${X''}^{g'}X'{X'}^{f'}$ X

(12) $p''p'$ và (13) $p'p$

${B''}^gB'{B'}^f$ B

là các hình vuông giao hoán; xét hình vuông

${X''}^{f'\circ g'}$ X

$$
p''p \tag{14}
$$

${B''}^{f\circ g}$ B .

Nó là giao hoán. Nếu các hình vuông (12) và (13) là cartesian, thì hình vuông (14) cũng vậy. Nếu các hình vuông (13) và (14) là cartesian, thì hình vuông (12) cũng vậy.

Hình vuông (14) là giao hoán, vì ta có $p\circ f'\circ g'=f\circ p'\circ g'=f\circ g\circ p''$.

Ký hiệu $h': X''\rightarrow B''\times_{B'}X',h: X'\rightarrow B'\times_BX$ và $h'': X''\rightarrow B''\times_BX$ là các ánh xạ liên tục chính tắc suy ra từ các hình vuông giao hoán (12), (13) và (14). Hơn nữa, ký hiệu

$$
j: B''\times_BX\rightarrow B''\times_{B'}(B'\times_BX)
$$

ánh xạ liên tục liên kết với $(b'', x)$ phần tử $(b'', g(b''), x)$. Đó là một phép đồng phôi và ta có $j\circ h''=$ (Id$_{B''}\times_Bh$)$\circ h'$.

Giả sử rằng hình vuông (13) là cartesian. Khi đó $h$ là một phép đồng phôi (I, p. 8, mệnh đề 2), do đó ánh xạ Id$_{B''}\times_Bh$ là một phép đồng phôi, và $h''$ là một phép đồng phôi khi và chỉ khi $h'$ là một phép đồng phôi. Điều này có nghĩa là hình vuông (12) là cartesian khi và chỉ khi hình vuông (14) là cartesian (loc. cit.).

Với ký hiệu của mệnh đề 7, đôi khi người ta nói rằng hình vuông (14) là hình vuông hợp thành bởi các hình vuông (13) và (12). Mệnh đề thứ nhất phát biểu rằng hình vuông hợp thành của hai hình vuông cartesian là cartesian. Đặc biệt, các $B''$-không gian $g^*(f^*(X))$ và $(f\circ g)^*(X)$ là đẳng cấu.

#### Nhận xét 1 {#ta-i-s1-n9-rem-1 .statement tag=01LY}

Có thể xảy ra rằng các hình vuông (12) và (14) là cartesian mà hình vuông (13) thì không như vậy (I, p. 139, bài tập 2).

#### Nhận xét 2 {#ta-i-s1-n9-rem-2 .statement tag=01LZ}

Cho $p: X\rightarrow B$ và $f: B'\rightarrow B$ là các ánh xạ liên tục. Ánh xạ $g: B'\rightarrow B'\times B$ được xác định bởi $g(b') = (b', f(b'))$ là một phép đồng phôi từ $B'$ lên đồ thị G của ánh xạ $f$ (TG, I, p. 25, hệ quả 2), và tích thớ $B'\times_BX$ được đồng nhất (I, p. 6) với không gian con của $B'\times X$, là ảnh ngược của G dưới ánh xạ Id$_{B'}\times p: B'\times X\rightarrow B'\times B$. Theo ví dụ ở I, p. 10 và hệ quả 1 của mệnh đề 5 (I, p. 11), các hình vuông

$B'\times_BX^iB'\times XB'\times X^{pr_2}$ X

pr$_1$ Id$_{B'}\times p$ and Id$_{B'}\times pp$

${B'}^gB'\times BB'\times B^{pr_2}$ B

(trong đó $i$ ký hiệu đơn ánh chính tắc) là cartesian, và hình vuông cartesian

$B'\times_BX^{pr_2}$ X

pr$_1p$

${B'}^f$ B

là hợp thành của chúng. Nói cách khác, mọi hình vuông cartesian đều được đồng nhất với hình vuông hợp thành của một hình vuông cartesian thu được bằng phép lấy tích (I, p. 11, hệ quả 1 của mệnh đề 5, hình vuông (8)) và của một hình vuông cartesian thu được bằng cách chuyển qua các không gian con (I, p. 10, ví dụ, hình vuông (5)).

#### Nhận xét 3 {#ta-i-s1-n9-rem-3 .statement tag=01M0}

Cho

$X_1^{g_1}$ X $X_2^{g_2}$ X

(15) $p_{_1}p$ and (16) $p_{_2}p$

$B_1^{f_1}$ B $B_2^{f_2}$ B

là các hình vuông cartesian. Xét hình vuông

$X_1\times_XX_2^g$ X

$$
p'p \tag{17}
$$

$B_1\times_BB_2^f$ B trong đó $f$ (tương ứng, $g$) là ánh xạ xác định cấu trúc B-không gian (tương ứng, cấu trúc X-không gian) của tích thớ $B_1\times_BB_2$ (tương ứng, của tích thớ $X_1\times_XX_2$), và trong đó $p'$ là ánh xạ suy ra từ $p_1\times p_2$ bằng cách chuyển qua các tập con. Nó là cartesian (I, p. 13, hệ quả 2 của mệnh đề 5).

Khi đó xét hai hình vuông giao hoán sau:

$$\begin{array}{ccc} X_1\times_XX_2 & \overset{\mathrm{pr}_1}{\longrightarrow} & X_1 \\ {\scriptstyle p'}\big\downarrow & & \big\downarrow{\scriptstyle p_1} \\ B_1\times_BB_2 & \overset{\mathrm{pr}_1}{\longrightarrow} & B_1 \end{array} \tag{18}$$

và

$$\begin{array}{ccc} X_1\times_XX_2 & \overset{\mathrm{pr}_2}{\longrightarrow} & X_2 \\ {\scriptstyle p'}\big\downarrow & & \big\downarrow{\scriptstyle p_2} \\ B_1\times_BB_2 & \overset{\mathrm{pr}_2}{\longrightarrow} & B_2 \end{array}. \tag{19}$$

Hình vuông (17) được hợp thành bởi các hình vuông (15) và (18), cũng như bởi các hình vuông (16) và (19). Theo mệnh đề 7, các hình vuông (18) và (19) là cartesian.

### 10. Ánh xạ ngặt

#### Mệnh đề 8 {#ta-i-s1-prop-8 .statement tag=01M1}

Cho

$$\begin{array}{ccc} X' & \overset{f'}{\longrightarrow} & X \\ {\scriptstyle p'}\big\downarrow & & \big\downarrow{\scriptstyle p} \\ B' & \overset{f}{\longrightarrow} & B \end{array}$$

là một hình vuông cartesian. Nếu ánh xạ $p$ là mở ( tương ứng là thực sự, tương ứng có trong một lân cận của mỗi điểm một tiết diện liên tục), thì $p'$ cũng có tính chất tương tự.

Theo nhận xét 2, I, p. 16, chỉ cần chứng minh mệnh đề đó đối với các hình vuông cartesian thuộc kiểu sau:

$$\begin{array}{ccccccc} \overset{-1}{p}(A) & \overset{j}{\longrightarrow} & X & & X\times F & \overset{\mathrm{pr}_1}{\longrightarrow} & X \\ {\scriptstyle p_A}\big\downarrow & & \big\downarrow{\scriptstyle p} & \text{và} & {\scriptstyle p\times \mathrm{Id}_F}\big\downarrow & & \big\downarrow{\scriptstyle p} \\ A & \overset{i}{\longrightarrow} & B & & B\times F & \overset{\mathrm{pr}_1}{\longrightarrow} & B \end{array},$$

trong đó F là một không gian tôpô, A là một không gian con của B, và $i,j$ là các đơn ánh chính tắc. Nếu ánh xạ $p$ là mở, các ánh xạ $p_A$ và $p\times$ Id$_F$ là mở (TG, I, p. 30, mệnh đề 2 và TG, I, p. 34, mệnh đề 8). Nếu ánh xạ $p$ là thực sự, các ánh xạ $p_A$ và $p\times$ Id$_F$ là thực sự (TG, I, p. 72, mệnh đề 3 và TG, I, p. 72, định nghĩa 1). Nếu U là một tập con mở của B và $s: U\rightarrow X$ là một tiết diện liên tục của $p$ trên U, ánh xạ $s|(A\cap U)$ là một tiết diện liên tục của $p_A$ trên $A\cap U$ và ánh xạ $s\times$ Id$_F$ là một tiết diện liên tục của $p\times$ Id$_F$ trên $U\times F$.

#### Nhận xét 1 {#ta-i-s1-n10-rem-1 .statement tag=01M2}

Với ký hiệu của mệnh đề 8, nếu $p$ là một ánh xạ đóng, điều đó không nhất thiết còn đúng đối với $p'($xem TG, I, p. 72, ví dụ). Tuy nhiên, nếu ánh xạ $p$ là đóng và nếu A là một không gian con của B, ánh xạ $p_A:\overset{-1}{p}(A)\rightarrow A$ là đóng (TG, I, p. 30, mệnh đề 2, a)).

#### Định nghĩa 5 {#ta-i-s1-def-5 .statement tag=01M3}

Cho X và Y là các không gian tôpô và $f: X\rightarrow Y$ là một ánh xạ. Gọi R là quan hệ tương đương liên kết với $f$, và

$$
X\rightarrow X/R-\overset{g}{\rightarrow}f(X)\rightarrow Y
$$

là phân tích chính tắc của $f$ (E, II, p. 44). Người ta nói rằng ánh xạ $f$ là ngặt nếu $g$ là một đồng phôi, khi $X/R$ được trang bị tôpô thương và $f(X)$ với tôpô cảm sinh bởi tôpô của Y.

Một ánh xạ ngặt là liên tục.

Nhắc lại rằng (TG, I, p. 22, mệnh đề 8), để một ánh xạ $f$ là ngặt, điều kiện cần và đủ là $f$ liên tục và với mọi tập con bão hòa mở (tương ứng đóng) A của X, tập hợp $f(A)$ mở (tương ứng đóng) trong $f(X)$.

#### Ví dụ 1 {#ta-i-s1-n10-exa-1 .statement tag=01M4}

Hợp thành của hai ánh xạ ngặt không nhất thiết là ngặt. Thật vậy, mọi ánh xạ liên tục $f: X\rightarrow Y$ đều là hợp thành của ánh xạ pr$_2: X\times Y\rightarrow$ Y và của ánh xạ $x\mapsto (x, f(x))$ từ X vào $X\times Y$, cả hai đều ngặt (TG, I, p. 26, mệnh đề 5 và TG, I, p. 25, hệ quả 2). Mặt khác, hợp thành của hai ánh xạ ngặt và đơn ánh (tương ứng toàn ánh) là một ánh xạ ngặt.

#### Ví dụ 2 {#ta-i-s1-n10-exa-2 .statement tag=01M5}

Một ánh xạ liên tục mà mở, hoặc đóng, hoặc có một tiết diện liên tục, thì là ngặt. Điều này suy ra từ mệnh đề 3 của TG, I, p. 32 và từ mệnh đề 9 của TG, I, p. 22.

#### Ví dụ 3 {#ta-i-s1-n10-exa-3 .statement tag=01M6}

Để một đồng cấu liên tục từ một nhóm tôpô vào một nhóm tôpô khác là một cấu xạ ngặt (TG, III, p. 16, định nghĩa 1), điều kiện cần và đủ là nó là một ánh xạ ngặt theo nghĩa của Định nghĩa 5.

#### Mệnh đề 9 {#ta-i-s1-prop-9 .statement tag=01M7}

Cho X, Y và Z là các không gian tôpô. Cho $f: X\rightarrow Y$ là một ánh xạ liên tục toàn ánh và $g: Y\rightarrow Z$ là một ánh xạ.

a) Nếu $f$ là ngặt và nếu $g\circ f$ liên tục, ánh xạ $g$ là liên tục.

b) Nếu $g$ liên tục và nếu $g\circ f$ là ngặt, ánh xạ $g$ là ngặt.

c) Nếu $f$ và $g\circ f$ là ngặt, $g$ là ngặt.

Hãy chứng minh mệnh đề a). Gọi R là quan hệ liên kết với $f$ trong X; theo giả thiết, ánh xạ từ $X/R$ lên Y suy ra từ $f$ bằng cách chuyển qua thương là một đồng phôi. Mệnh đề thứ nhất khi đó suy ra từ mệnh đề 6 của I, p. 21.

Hãy chứng minh b). Cho B là một tập con đóng bão hòa của Y đối với quan hệ được xác định bởi $g$ và đặt $A =\overset{-1}{f}(B)$. Vì $f$ liên tục, A đóng trong X, và A bão hòa đối với quan hệ tương đương được xác định bởi $g\circ f$. Vì $g\circ f$ là ngặt và $f$ là toàn ánh, nên $g(B) =g\circ f(A)$ do đó đóng trong Z. Vậy ánh xạ liên tục $g$ là ngặt.

Mệnh đề c) suy ra ngay lập tức từ các mệnh đề a) và b).

#### Mệnh đề 10 {#ta-i-s1-prop-10 .statement tag=01M8}

Cho X là một không gian tôpô và cho R là một quan hệ tương đương trong X. Cho Y là một không gian tôpô compact địa phương. Cho S là quan hệ tương đương trong $X\times Y$ là tích của quan hệ tương đương R trong X với quan hệ đẳng thức trong Y. Song ánh chính tắc $(X\times Y)/S\rightarrow (X/R)\times Y$ là một đồng phôi.

Nhắc lại rằng nếu U và V là các không gian tôpô, thì $\mathscr{C}_c(U; V)$ ký hiệu tập hợp các ánh xạ liên tục từ U vào V, được trang bị tôpô hội tụ compact (TG, X, p. 26, def. 1).

Cho $p: X\rightarrow X/R$ và $q: X\times Y\rightarrow (X\times Y)/S$ là các toàn ánh chính tắc. Cho $g: (X\times Y)/S\rightarrow (X/R)\times Y$ ký hiệu song ánh chính tắc. Nó liên tục; gọi $h$ là ánh xạ nghịch đảo của nó và hãy chứng minh rằng nó liên tục.

Ánh xạ $i: X\rightarrow \mathscr{C}_c(Y; X\times Y)$ sao cho, với mọi $x\in$ X, $i(x)$ là ánh xạ được xác định bởi $y\mapsto (x, y)$, là liên tục (TG, X, p. 28, th. 3). Ánh xạ $\widetilde{q}:\mathscr{C}_c(Y; X\times Y)\rightarrow \mathscr{C}_c(Y; (X\times Y)/S)$ gán cho một ánh xạ liên tục $\varphi$ ánh xạ $q\circ \varphi$, là liên tục (TG, X, p. 29, prop. 9). Do đó, ánh xạ $\widetilde{q}\circ i: X\rightarrow \mathscr{C}_c(Y; (X\times Y)/S)$ là liên tục. Nó tương thích với quan hệ tương đương R; vì thế ánh xạ duy nhất $j: X/R\rightarrow \mathscr{C}_c(Y; (X\times Y)/S)$ sao cho $j\circ p=\widetilde{q}\circ i$ là liên tục. Ta có $h(\xi , y) =j(\xi )(y)$ với mọi cặp $(\xi , y)\in (X/R)\times Y$. Vì Y là compact địa phương, nên từ TG, X, p. 28, th. 3 suy ra rằng ánh xạ $h$ là liên tục.

Kết luận của Mệnh đề 10 không còn nhất thiết đúng nữa nếu Y không compact địa phương (TG, I, p. 96, exerc. 6).

#### Hệ quả {#ta-i-s1-n10-cor-1 .statement tag=01M9}

Cho X và Y là các không gian tôpô và cho $f: X\rightarrow$ Y là một ánh xạ liên tục. Cho T là một không gian tôpô compact địa phương. Nếu ánh xạ $f$ là ngặt, thì ánh xạ $f\times$ Id$_T$ từ $X\times T$ vào $Y\times T$ cũng vậy.

### 11. Các ánh xạ ngặt phổ dụng

Cho

${X'}^{f'}$ X

$p'p$

${B'}^f$ B

là một hình vuông Descartes, trong đó ánh xạ $p$ là ngặt. Ánh xạ $p'$ không nhất thiết là ngặt (xem TG, I, p. 96, exerc. 6). Tuy nhiên, nếu A là một không gian con mở hoặc đóng của B, thì ánh xạ $p_A:\overset{-1}{p}(A)\rightarrow A$ là ngặt (TG, I, p. 23, cor. 1).

#### Định nghĩa 6 {#ta-i-s1-def-6 .statement tag=01MA}

Cho $p: X\rightarrow B$ là một ánh xạ liên tục. Người ta nói rằng ánh xạ $p$ là ngặt phổ dụng nếu với mọi hình vuông Descartes

${X'}^{f'}$ X

$p'p$

${B'}^f$ B

thì ánh xạ $p'$ là ngặt.

Một ánh xạ ngặt phổ dụng là ngặt. Với các ký hiệu của Định nghĩa 6, nếu ánh xạ $p$ là ngặt phổ dụng, thì $p'$ cũng vậy. Điều này suy ra ngay lập tức từ def. 6 và prop. 7 của I, p. 15.

#### Hệ quả {#ta-i-s1-n11-cor-1 .statement tag=01MB}

Một ánh xạ liên tục mở, hoặc thực sự, hoặc thừa nhận trong một lân cận của mọi điểm một tiết diện liên tục, là ngặt phổ dụng (prop. 8 và ví dụ 2).

#### Ví dụ {#ta-i-s1-n11-exa-1 .statement tag=01MC}

Cho B là một không gian tôpô và cho $(A_i)_{i\in I}$ là một phủ của B; gọi A là không gian tổng của họ $(A_i)_{i\in I}$, và cho $p: A\rightarrow B$ là ánh xạ chính tắc. Ánh xạ $p$ là ngặt phổ dụng dưới mỗi một trong hai giả thiết sau đây:

(i) Với mọi điểm $b\in B$, tồn tại $i\in I$ sao cho $b$ là một điểm trong của $A_i$;

(ii) Họ $(A_i)$ là hữu hạn địa phương và các $A_i$ là những tập con đóng của B.

Dưới giả thiết (i), ánh xạ $p$ có trong một lân cận của mọi điểm một tiết diện liên tục. Dưới giả thiết (ii), ánh xạ $p$ là thực sự theo định nghĩa của không gian tổng (resp. theo TG, I, p. 6, prop. 4 và TG, I, p. 75, th. 1). Do đó nó là ngặt phổ dụng.

#### Nhận xét {#ta-i-s1-n11-rem-1 .statement tag=01MD}

Một ánh xạ đóng không nhất thiết là ngặt phổ dụng (xem TG, I, p. 96, exerc. 6).

#### Mệnh đề 11 {#ta-i-s1-prop-11 .statement tag=01ME}

Cho

${X'}^{f'}$ X

$p'p$

${B'}^f$ B

một hình vuông Descartes.

a) Giả sử ánh xạ $f$ ngặt và toàn ánh. Khi đó, nếu ánh xạ $p'$ là mở (resp. đóng, resp. thực sự), thì $p$ cũng có tính chất ấy.

b) Giả sử rằng ánh xạ $f$ là đóng và toàn ánh. Khi đó, nếu ánh xạ $p'$ là ngặt, thì $p$ cũng có tính chất ấy.

c) Giả sử rằng ánh xạ $f$ là ngặt phổ dụng và toàn ánh. Khi đó, nếu ánh xạ $p'$ là ngặt, thì $p$ cũng có tính chất ấy.

Trước hết nhận xét rằng với mọi tập con A của X, ta có

$$
p'((\overset{-1}{f}')(A)) =\overset{-1}{f}(p(A)) \tag{20}
$$

Thật vậy, nếu $x'\in (\overset{-1}{f}')(A)$, thì $f(p'(x')) =p\circ f'(x')\in p(A)$. Ngược lại, nếu $b'\in \overset{-1}{f}(p(A))$, lấy $x\in A$ sao cho $f(b') =p(x)$. Theo định nghĩa của một hình vuông Descartes, tồn tại duy nhất $x'\in X'$ sao cho $f'(x') =x$ và $p'(x') =b'$, do đó $b'\in p'((\overset{-1}{f}')(A))$.

Ta chứng minh a). Trước hết giả sử rằng $p'$ là một ánh xạ mở (resp. đóng) và A là một tập mở (resp. đóng) trong X. Tập $(\overset{-1}{f}')(A)$ là mở (resp. đóng) trong $X'$. Vì thế tập $p'((\overset{-1}{f}')(A))$ là mở (resp. đóng) trong $B'$. Theo hệ thức (20), nó cũng bão hòa đối với quan hệ tương đương do $f$ xác định. Vì ánh xạ $f$ được giả sử là toàn ánh, khi đó ta có $p(A) =$

$f(p'((\overset{-1}{f}')(A)))$, và vì nó là ngặt, tập $p(A)$ là mở (resp. đóng) trong B. Vậy ánh xạ $p$ là mở (resp. đóng).

Để một ánh xạ liên tục là thực sự, điều kiện cần và đủ là nó đóng và các thớ của nó là giả-compacte (TG, I, p. 75, th. 1). Nếu ánh xạ $p'$ là thực sự, thì ánh xạ $p$ là đóng theo điều vừa chứng minh. Hãy xét các thớ của nó: nếu $b\in B$, lấy $b'\in B'$ sao cho $f(b') =b$. Theo hệ quả của I, p. 10, ánh xạ $f'$ cảm sinh một đồng phôi $X'_{b'}\rightarrow X_b$. Vì $p'$ là thực sự, $X'_{b'}$ là giả-compacte, do đó $X_b$ cũng vậy. Vậy ánh xạ $p$ là thực sự.

Ta chứng minh b) và c). Đặt Y = $p(X)$ và $Y'=p'(X')$ ; hệ thức (20) áp dụng cho X cho thấy rằng $Y'=\overset{-1}{f}(Y)$. Ký hiệu $g$ là ánh xạ từ $Y'$ vào Y do $f$ cảm sinh. Trong trường hợp b), ánh xạ $g$ là ngặt theo nhận xét 1, I, p. 18. Trong trường hợp c), nó là ngặt do định nghĩa 6 vì hình vuông

$Y'$ Y

$B'$ B

là Descartes.

Ký hiệu $q$ và $q'$ là các ánh xạ từ X vào Y và từ $X'$ vào $Y'$ được cảm sinh bởi $p$ và $p'$, sao cho hình vuông

${X'}^{f'}$ X

$q'q$

${Y'}^g$ Y

là đề-các. Vì các ánh xạ $g$ và $q'$ đều ngặt và toàn ánh, hợp thành của chúng $g\circ q'$ là ngặt. Do đó $q\circ f'$ là ngặt và bản thân $p\circ f'$ là ngặt. Vì $f$ là toàn ánh nên $f'$ cũng vậy, và $p$ là ngặt theo mệnh đề 9, b) của I, p. 18.

#### Hệ quả 1 {#ta-i-s1-prop-11-cor-1 .statement tag=01MF}

Giả sử rằng ánh xạ $f$ là ngặt phổ dụng và toàn ánh và rằng ánh xạ $p'$ là ngặt phổ dụng. Khi đó ánh xạ $p$ là ngặt phổ dụng.

Cho

Y $^{g'}$ X

$qp$

C $^g$ B

là một hình vuông đề-các; vấn đề là chứng minh rằng ánh xạ $q$ là ngặt. Theo nhận xét 3 của I, p. 16, các hình vuông

$$
X'\times_XY^{pr_1}X'
$$

$rp'$

$$
B'\times_BC^{pr_1}B'
$$

và

$X'\times_XY^{pr_2}$ Y

$$
rq \tag{21}
$$

$B'\times_BC^{pr_2}$ C

là đề-các, trong đó $r: X'\times_XY\rightarrow B'\times_BC$ ký hiệu ánh xạ cảm sinh bởi $(p', q)$. Vì ánh xạ $f$ là ngặt phổ dụng và toàn ánh, điều ấy cũng đúng với ánh xạ pr$_2: B'\times_BC\rightarrow C$ (I, p. 20, định nghĩa 6 và I, p. 10, hệ quả của mệnh đề 4). Mặt khác, ánh xạ $r$ là ngặt, vì $p'$ được giả thiết là ngặt phổ dụng. Áp dụng mệnh đề 11, c) cho hình vuông đề-các (21), suy ra ánh xạ $q$ là ngặt.

#### Hệ quả 2 {#ta-i-s1-prop-11-cor-2 .statement tag=01MG}

Cho B và X là các không gian tôpô và cho $p: X\rightarrow B$ là một ánh xạ liên tục. Cho $(A_i)_{i\in I}$ là một họ các tập con của B tạo thành một phủ mở của B, hoặc cũng có thể là một phủ đóng hữu hạn địa phương của B. Nếu với mọi $i\in$ I, ánh xạ $p_{A_i}:\overset{-1}{p}(A_i)\rightarrow A_i$ là ngặt (tương ứng, ngặt phổ dụng), thì ánh xạ $p$ là ngặt (tương ứng, ngặt phổ dụng).

Với mọi $i\in I$, đặt $Y_i=\overset{-1}{p}(A_i)$ và $p_i=p_{A_i}$. Gọi A là không gian tổng của họ $(A_i)_{i\in I}$, Y là không gian tổng của họ $(Y_i)_{i\in I}$; ký hiệu bởi $f: A\rightarrow B$ (tương ứng $g: Y\rightarrow X,q: Y\rightarrow A$) ánh xạ suy ra từ họ các đơn ánh chính tắc $A_i\rightarrow B$ (tương ứng từ các đơn ánh chính tắc $Y_i\rightarrow X$, từ các ánh xạ $p_i$). Hình vuông

Y $^g$ X

$qp$

A $^f$ B

là đề-các (ví dụ, I, p. 10 và p. 14). Theo hệ quả, I, p. 20, ánh xạ $f$ là ngặt phổ dụng. Do mệnh đề 11, vì thế chỉ còn phải chứng minh rằng ánh xạ $q$ là ngặt (tương ứng, ngặt phổ dụng) nếu các ánh xạ $p_i$, với $i\in I$, là như vậy. Như thế ta được đưa về việc chứng minh hệ quả trong trường hợp các tập $A_i$, $i\in I$, tạo thành một phân hoạch của không gian B thành các tập con vừa mở vừa đóng, và từ đây về sau ta sẽ giả thiết như vậy.

Giả sử rằng mỗi ánh xạ $p_i,i\in I$, là ngặt. Nếu U là một tập con mở của X và bão hòa đối với quan hệ tương đương được xác định bởi $p$, thì tập $p_i(X_i\cap U)$ là mở trong $A_i$ và $p(U) =$ $\bigcup_{i\in I}p_i(X_i\cap U)$ là mở trong B. Do đó ánh xạ $p$ là ngặt.

Bây giờ giả sử rằng mỗi ánh xạ $p_i,i\in I$, là ngặt phổ dụng, và bây giờ chứng minh rằng ánh xạ $p$ là ngặt phổ dụng. Cho C là một không gian tôpô và $h: C\rightarrow B$ là một ánh xạ liên tục. Vấn đề là chứng minh rằng ánh xạ pr$_1: X\times_BC\rightarrow C$ là ngặt. Không gian C được đồng nhất với không gian tổng của họ các $C_i=\overset{-1}{h}(A_i)$ và không gian $X\times_BC$ được đồng nhất với không gian tổng của họ các $X\times_BC_i= X_i\times_{A_i}C_i$. Vì $p_i$ là ngặt phổ dụng, nên ánh xạ pr$_1: X_i\times_{A_i}C_i\rightarrow C_i$ là ngặt. Theo điều đi trước, ánh xạ pr$_1: X\times_BC\rightarrow C$ là ngặt. Điều này chứng minh rằng ánh xạ $p$ là ngặt phổ dụng.

## BÀI TẬP {#ta-i-s1-exercises}

Xem [các bài tập cho § 1](exercises/s1/).
