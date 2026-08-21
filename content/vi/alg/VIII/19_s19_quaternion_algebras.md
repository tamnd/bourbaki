---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Semisimple Modules and Rings
section: 19
section_title: Quaternion Algebras
lang: vi
source: alg-viii
source_edition: 2023, Springer Nature
book_pages: A VIII.361-A VIII.371
pdf_pages: 0378-0388
extraction: native
subsections:
    - "no": 1
      title: General Properties of Quaternion Algebras
      page: 361
      pdf_page: 378
    - "no": 2
      title: The Center of a Quaternion Algebra
      page: 363
      pdf_page: 380
    - "no": 3
      title: Simplicity of Quaternion Algebras
      page: 363
      pdf_page: 380
    - "no": 4
      title: Criteria for a Quaternion Algebra to Be a Field
      page: 366
      pdf_page: 383
    - "no": 5
      title: Algebras over Maximal Ordered Fields
      page: 367
      pdf_page: 384
statements: 16
exercises: 8
content_sha256: 468b416f21fef7c43e44ab86fe6566124db981e0554c7ebe6a7421e86409554a
translated_from: content/en/alg/VIII/19_s19_quaternion_algebras.md
source_content_sha256: 29c7745ce44d10980513b080b27eb063e43ebe7bda18a9a407a496a816099f84
translation_model: gpt-5.4
translation_run: translate-vi-74c08a00
glossary_version: 34
glossary_terms_sha256: 7a2070c1f12ce35bba4f185e4042235ff114105974985e96a2bdf576c949ebc1
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 19. ĐẠI SỐ QUATERNION

Trong mục này, K là một trường giao hoán.

### 1. Các tính chất tổng quát của các đại số quaternion

Cho $\alpha , \beta , \gamma$ là các phần tử của K, và cho F là đại số quaternion kiểu $(\alpha , \beta , \gamma )$. Nhắc lại rằng (III, §2, No. 5, p. 445)[^1] F là một K-đại số kết hợp có đơn vị, có một cơ sở $(1, i, j, k)$ trên K thỏa mãn các quan hệ

$$
i^2=\alpha +\beta i ,j^2=\gamma  ,ij=k ,ji=\beta j-k \tag{1}
$$

Đó là một đại số Cayley (III, §2, No. 4, p. 441, Định nghĩa 1) mà phép liên hợp thỏa mãn

$$
\overline{i}=\beta -i ,\overline{j}=-j ,\overline{k}=-k \tag{2}
$$

Nhắc lại rằng vết Cayley và chuẩn của F là các ánh xạ $T_F$ và $N_F$ từ F vào K được định nghĩa bởi $T_F(q) =q+\overline{q}$ và $N_F(q) =qq$.

Không gian con tuyến tính E của F với cơ sở $(1, i)$ là một đại số con Cayley giao hoán của F; nó là một đại số bậc hai kiểu $(\alpha , \beta )$, và F có thể được đồng nhất với mở rộng Cayley của E được xác định bởi $\gamma$ (III, §2, No. 5, p. 444). Với mọi $z\in E$, ta có $zj=jz$. Mỗi phần tử $q$ của F có thể được viết duy nhất dưới dạng $x+jy$ với $x, y\in E$, và ta có

$$
\overline{q}=\overline{x}-jy ,T_F(q) =x+\overline{x},N_F(q) =xx-\gamma yy \tag{3}
$$

#### Mệnh đề 1 {#alg-viii-s19-prop-1 .statement tag=00LQ}

Đa thức đặc trưng của một phần tử $q$ của F bằng $(X^2-T_F(q)X + N_F(q))^2$.

Theo trên đây, đại số F là một E-môđun phải tự do với cơ sở $(1, j)$. Do đó, F[X] là một E[X]-môđun phải tự do với cơ sở $(1, j)$. Ta ký hiệu bởi $u$ tự đồng cấu của E[X]-môđun phải F[X] được xác định bởi $u(P) =$ $(X-q)P$ với $P\in F[X]$. Đa thức đặc trưng của $q$ là định thức của $u$ được xem như một tự đồng cấu của K[X]-môđun F[X]. Theo Mệnh đề 6 của III, §9, No. 4, p. 546, nó bằng N(det $u$), trong đó N ký hiệu chuẩn từ E[X] tới K[X]. Viết $q$ dưới dạng $x+jy$ với $x, y\in E$. Ma trận của $u$ đối với cơ sở $(1, j)$ là $\begin{pmatrix} X-x & -\gamma y \\ -y & X-\overline{x} \end{pmatrix}$ ; định thức của nó bằng $D = (X-x)(X-\overline{x})-\gamma yy= X^2-T_F(q)X + N_F(q)$ (xem công thức (3)). Vì D thuộc K[X], ta có $N(D) = D^2$; Mệnh đề 1 được suy ra.

#### Nhận xét 1 {#alg-viii-s19-n1-rem-1 .statement tag=00LR}

Giả sử đặc số của K khác 2, và đặt $i'= 2i-\beta$. Khi đó $(1, i')$ là một cơ sở của E trên K, và ta có ${i'}^2= 4\alpha +\beta^2$. Suy ra E đẳng cấu với đại số bậc hai kiểu $(4\alpha +\beta^2,0)$ và F đẳng cấu với đại số quaternion kiểu $(4\alpha +\beta^2,0, \gamma )$.

#### Nhận xét 2 {#alg-viii-s19-n1-rem-2 .statement tag=00LS}

Đại số quaternion kiểu $(\alpha ,0, \gamma )$ đẳng cấu với đại số quaternion kiểu $(\gamma ,0, \alpha )$ (III, §2, No. 5, p. 445). Nó cũng đẳng cấu với đại số quaternion kiểu $(\alpha a^2,0, \gamma c^2)$ với mọi cặp $(a, c)$ gồm các phần tử khác không của K.

#### Nhận xét 3 {#alg-viii-s19-n1-rem-3 .statement tag=00LT}

Cho $q$ là một phần tử của F. Khi đó $q$ là lũy linh khi và chỉ khi đa thức đặc trưng của nó bằng $X^4$, tức là, $T_F(q) = N_F(q) = 0$; khi đó ta có $q^2= 0$.

#### Ví dụ {#alg-viii-s19-n1-exa-1 .statement tag=00LU}

Đại số ma trận $\mathbf{M}_2(K)$ đẳng cấu với đại số quaternion kiểu $(0,1,1)$. Thật vậy, xét đại số bậc hai $E = K\times K$ (kiểu $(0,1)$) và đại số quaternion $F = E + Ej$, là mở rộng Cayley của E được xác định bởi phần tử $\gamma = 1$. Ánh xạ $(a, b)\mapsto \begin{pmatrix} a & 0 \\ 0 & b \end{pmatrix}$ là một đồng cấu đại số từ E vào $\mathbf{M}_2(K)$. Vì với $a, b$ trong K, ta có

$$
(01)((01)(10)(01)((a0)(b0)((01)
$$

=, =,

1 0 1 0 0 1 1 0 0 $b$ 0 $a$ 1 0

đồng cấu này mở rộng thành một đồng cấu đại số $\theta : F\longrightarrow \mathbf{M}_2(K)$ được xác định bởi

$$
(ac)
$$

$$
\theta ((a, b) + (c, d)j)=
$$

$$
db
$$

Đồng cấu này là song ánh. Khi đặc số của K khác 2, đại số $\mathbf{M}_2(K)$ cũng đẳng cấu với đại số quaternion kiểu $(1,0,1)$ (Nhận xét 1).

### 2. Tâm của một đại số quaternion

Cho $\alpha ,\beta ,\gamma$ là các phần tử của K, và gọi F là đại số quaternion kiểu $(\alpha , \beta , \gamma )$.

#### Mệnh đề 2 {#alg-viii-s19-prop-2 .statement tag=00LV}

a) Giả sử rằng trường K có đặc số khác 2. Nếu $\gamma$ hoặc $4\alpha +\beta^2$ khác không, thì tâm của F bằng K; nếu không, nó có chiều 2 và được sinh bởi 1 và $ij-ji$.

b) Giả sử rằng trường K có đặc số 2. Nếu $\beta \not= 0$, thì tâm của F bằng K; nếu $\beta = 0$, thì đại số F là giao hoán.

Theo công thức (30) của III, §2, No. 5, p. 444, ta có

$$
ij-ji=-\beta j+ 2k ,jk-kj=\beta \gamma -2\gamma i ,ki-ik=-2\alpha j-\beta k \tag{4}
$$

Một phần tử $q=x+yi+zj+tk$ của F là trung tâm khi và chỉ khi nó giao hoán với $i$ và $j$, nghĩa là ta có

(5) $2z+\beta t=-\beta z+ 2\alpha t= 0$ and $2\gamma t=\beta \gamma t= 2y=\beta y= 0$.

Trước hết giả sử đặc số của K khác 2. Nếu $\gamma$ khác không, thì các đẳng thức trong (5) suy ra $y=t= 0$ và khi đó $z= 0$; do đó, ta có $q\in K$. Nếu $\gamma = 0$ và $4\alpha +\beta^2\not= 0$, thì chúng suy ra $y=z=t= 0$, nên ta có $q\in K$. Nếu $\gamma = 4\alpha +\beta^2= 0$, thì hệ (5) thu về $y= 2z+\beta t= 0$, nên ta có $q=x+t/2(ij-ji)$, điều này hoàn tất chứng minh của a).

Bây giờ giả sử trường K có đặc số 2. Khi đó hệ (5) có thể được viết thành $\beta t=\beta z=\beta y= 0$; mệnh đề b) suy ra.

### 3. Tính đơn của các đại số quaternion

#### Mệnh đề 3 {#alg-viii-s19-prop-3 .statement tag=00LW}

Cho $\alpha ,\beta ,\gamma$ là các phần tử của K, và cho $f$ là một đại số quaternion kiểu $(\alpha , \beta , \gamma )$. Ký hiệu vết Cayley và chuẩn Cayley của nó bởi $T_F$ và $N_F$. Các tính chất sau là tương đương:

(i) Đại số F là đơn tâm.

(ii) Với mọi phần tử khác không $x$ của F, tồn tại một phần tử $y$ trong F sao cho $T_F(xy)\not= 0$.

(iii) Ta có $(4\alpha +\beta^2)\gamma \not= 0$.

Giả sử rằng các tính chất này đúng. Khi đó với mọi $x$ trong F, đa thức đặc trưng rút gọn của $x$ là $X^2-T_F(x)X + N_F(x)$. Đặc biệt, $T_F(x)$ là vết rút gọn của $x$, và $N_F(x)$ là chuẩn rút gọn của nó.

(i)$\Rightarrow$(ii): Nếu đại số F là đơn tâm, thì theo Mệnh đề 1 của VIII, p. 361 và định nghĩa của vết rút gọn (VIII, p. 340, Định nghĩa 2), suy ra $T_F$ là vết rút gọn của nó; mệnh đề (ii) suy ra được (VIII, p. 343, Mệnh đề 5).

(ii)$\Leftrightarrow$(iii): Cho $(e_i)_{1\leqslant i\leqslant 4}$ là một cơ sở của F kiểu $(\alpha , \beta , \gamma )$ (III, §2, No. 5, p. 445). Ma trận $(T_F(e_ie_j))$ bằng

2 $\beta$ 0 0

$\beta 2\alpha +\beta^2$ 0 0

.

0 0 $2\gamma \beta \gamma$

0 0 $\beta \gamma -2\alpha \gamma$

Định thức của nó là $-\gamma^2(4\alpha +\beta^2)^2$. Sự tương đương của các tính chất (ii) và (iii) suy ra từ V, §8, No. 2, p. 49, Bổ đề 1.

(iii)$\Rightarrow$(i): Giả sử $(4\alpha +\beta^2)\gamma \not= 0$. Khi đó ta có $\gamma \not= 0$, và ta có $\beta \not= 0$ nếu K có đặc số 2. Theo Mệnh đề 2, đại số F là trung tâm. Gọi $x$ là một phần tử của căn Jacobson của F. Với mọi $y\in F,xy$ là lũy linh, nên $T_F(xy) = 0$ (Nhận xét 3 của VIII, p. 362). Vì (ii) tương đương với (iii), suy ra $x= 0$. Điều này chứng tỏ F là một đại số nửa đơn trên K. Vì tâm của nó là K, nó là đơn.

Khẳng định cuối cùng suy ra từ Mệnh đề 1 của VIII, p. 361 và định nghĩa của đa thức đặc trưng rút gọn (VIII, p. 340, Định nghĩa 1).

Ký hiệu đặc số của K là $p$. Theo Mệnh đề 3, nếu $p\not= 2$, thì mọi đại số quaternion trên K kiểu $(\alpha ,0, \gamma )$ với $\alpha$ và $\gamma$ thuộc $K^*$ đều là đơn tâm. Nếu $p= 2$, thì mọi đại số quaternion kiểu $(\alpha ,1, \gamma )$ với $\alpha \in K$ và $\gamma \in K^*$ đều là đơn tâm. Ngược lại, ta có điều sau đây.

#### Mệnh đề 4 {#alg-viii-s19-prop-4 .statement tag=00LX}

Cho A là một đại số đơn tâm bậc 4 trên K. Ký hiệu đặc số của K là $p$.

a) Nếu $p\not= 2$, thì tồn tại các phần tử khác không $\alpha$ và $\gamma$ của K sao cho đại số A đẳng cấu với đại số quaternion kiểu $(\alpha ,0, \gamma )$.

b) Nếu $p= 2$, thì tồn tại một phần tử $\alpha$ của K và một phần tử $\gamma$ của $K^*$ sao cho đại số A đẳng cấu với đại số quaternion kiểu $(\alpha ,1, \gamma )$.

Theo định lý của Wedderburn (VIII, p. 120, Định lý 1), tồn tại một số nguyên $r\geqslant 1$ và một trường D có tâm K sao cho A đẳng cấu với $\mathbf{M}_r(D)$. Khi đó ta có $r^2[D : K] = [A : K] = 4$. Nếu $r= 2$, thì A đẳng cấu với $\mathbf{M}_2$(K), và Mệnh đề 4 suy ra từ ví dụ ở VIII, p. 362. Nếu không, ta có $r= 1$, và A là một trường có tâm K. Khi đó nó có một trường con giao hoán cực đại E là một mở rộng tách được của K; vì A có bậc 4 trên K, nên mở rộng E có bậc 2 trên K (VIII, p. 265, Hệ quả 2). Do đó nó là bậc hai (III, §2, No. 3, p. 439). Gọi $s$ là phép liên hợp của E (III, §2, No. 3, p. 440). Theo định lý Skolem–Noether (VIII, p. 256, Hệ quả 1), tồn tại một phần tử khả nghịch $j$ của A sao cho ta có $s(x) =jxj^{-1}$ với mọi $x$ trong E. Trường E là tách được trên K, nên ta có $s\not=$ Id$_E$, do đó $j \notin E$. Vì A là một không gian vectơ chiều 4 trên K, nên nó là một không gian vectơ trái chiều 2 trên E, do đó ta có $A = E\oplus Ej$. Ta có $s^2=$ Id$_E$, nên phần tử $j^2$ của A thuộc tâm của A; do đó tồn tại một phần tử $\gamma$ của $K^*$ sao cho $j^2=\gamma$.

Khi $p\not= 2$, tồn tại một phần tử $i$ của E và một phần tử $\alpha \in K^*$ sao cho $E = K(i)$ và $i^2=\alpha$ (V, §11, No. 9, p. 93, Ví dụ 3); trong trường hợp này, A đẳng cấu với đại số quaternion kiểu $(\alpha ,0, \gamma )$. Khi $p= 2$, tồn tại một phần tử $i$ của E và một phần tử $\alpha$ của K sao cho $E = K(i)$ và $i^2=i+\alpha$ (V, §11, No. 9, p. 93, Ví dụ 2), do đó A đẳng cấu với đại số quaternion kiểu $(\alpha ,1, \gamma )$.

#### Hệ quả 1 {#alg-viii-s19-prop-4-cor-1 .statement tag=00LY}

Cho A là một đại số đơn tâm trên K có bậc hữu hạn $>1$ mà mọi phần tử đều đại số trên K với bậc $\leqslant 2$. Khi đó A đẳng cấu với một đại số quaternion trên K.

Nếu K là hữu hạn, thì đại số A đẳng cấu với một đại số ma trận $\mathbf{M}_n(K)$ (VIII, p. 357, Hệ quả 2) và do đó chứa các phần tử bậc $n$ trên K; giả thiết suy ra $n= 2$ và do đó cho kết quả trong trường hợp này (VIII, p. 362, Ví dụ). Giả sử trường K là vô hạn. Gọi L là một dưới đại số étale cực đại của A. Theo V, §7, No. 4, p. 41, Mệnh đề 7, tồn tại một phần tử $x$ của A sao cho đại số trên K L bằng $K[x]$, do đó theo giả thiết có bậc $\leqslant 2$. Vì ta có $[A : K] = [L : K]^2$ (VIII, p. 264, Mệnh đề 4 and p. 262, Mệnh đề 3), ta kết luận rằng [A : K] = 4. Khi đó Hệ quả 1 suy ra từ Mệnh đề 4.

#### Hệ quả 2 {#alg-viii-s19-prop-4-cor-2 .statement tag=00LZ}

Cho $(E, s)$ là một đại số Cayley trên K sao cho đại số trên K E là đơn tâm bậc hữu hạn $>1$ trên K. Khi đó E đẳng cấu với một đại số quaternion trên K.

Mọi phần tử $u$ của E đều thỏa mãn $u^2-T_E(u)u+ N_E(u) = 0$, do đó đại số trên K E đẳng cấu với một đại số quaternion (Hệ quả 1).

### 4. Các tiêu chuẩn để một Đại số Quaternion là một Trường

Cho $\alpha , \beta , \gamma$ là các phần tử của trường K, và F là đại số quaternion kiểu $(\alpha , \beta , \gamma )$. Như trong No.1, ta ký hiệu cơ sở chính tắc của F là $(1, i, j, k)$ và đại số con $K + Ki$ của F là E.

#### Mệnh đề 5 {#alg-viii-s19-prop-5 .statement tag=00M0}

Các tính chất sau là tương đương:

(i) Đại số quaternion F là một trường.

(ii) Không có phần tử khác không nào $q\in F$ sao cho $T_F(q) = N_F(q) = 0$.

(iii) Mọi phần tử của F có bình phương bằng không đều bằng không.

(iv) Không tồn tại vectơ khác không nào $(x, y, z, t)$ trong $K^4$ sao cho

$$
x^2+\beta xy-\alpha y^2-\gamma (z^2+\beta zt-\alpha t^2) = 0
$$

(v) Không tồn tại vectơ khác không nào $(x, y, z)$ trong $K^3$ sao cho

$$
x^2+\beta xy-\alpha y^2-\gamma z^2= 0
$$

(vi) Đại số bậc hai E là một trường, và $\gamma$ không phải là chuẩn của một phần tử của E.

Một phần tử $q$ của F là khả nghịch khi và chỉ khi $N_F(q)$ khác 0. Do đó tính tương đương của (i) và (iv) suy ra từ công thức (31) của III, §2, No. 5, p. 445; hiển nhiên là (i) kéo theo (iii) và (iv) kéo theo (v).

Tính tương đương của (ii) và (iii) suy ra từ Nhận xét 3 của VIII, p. 362.

Giả sử F không phải là một trường. Nếu $\gamma (4\alpha +\beta^2)\not= 0$, thì đại số F là đơn tâm bậc 4 trên K; nó đẳng cấu với đại số $\mathbf{M}_2(K)$ (VIII, p. 120, Định lý 1) và do đó chứa một phần tử khác không có bình phương bằng không. Nếu $\gamma = 0$, thì ta có $j^2= 0$. Nếu $4\alpha +\beta^2= 0$, thì ta có $(2i-\beta )^2= 0$ và $2i-\beta \not= 0$ nếu K có đặc số khác 2. Cuối cùng, nếu K có đặc số 2 và $\beta$ bằng không, thì ta có $T_F(q) = 0$ với mọi $q\in F$ (III, §2, No. 5, p. 445, công thức (31)). Vì F không phải là một trường, tồn tại một phần tử khác không $q$ của F sao cho $N_F(q) = 0$; ta có $q^2= 0$. Điều này chứng minh hàm ý (iii)$\Rightarrow$(i).

Cho $q=x+yi$ là một phần tử của E. Ta có $N_{E/K}(q) =x^2+\beta xy-\alpha y^2$. Giả sử rằng tính chất (v) được thỏa mãn. Ta có $N_{E/K}(q)-\gamma \not= 0$ và $N_{E/K}(q)\not= 0$ nếu $q\not= 0$, và do đó (vi).

Cuối cùng, giả sử rằng tính chất (vi) được thỏa mãn. Cho $q$ là một phần tử khác không của F; ta viết nó dưới dạng $u+vj$ với $u$ và $v$ thuộc E. Nếu $v$ bằng không, thì $q$ khả nghịch. Nếu $v$ khác không, thì ta có $N_F(q) = N_F(v)N_F(v^{-1}u+j) =$ $N_{E/K}(v)(N_{E/K}(v^{-1}u)-\gamma )$ theo III, §2, No. 5, p. 443, công thức (24). Vì $\gamma$ không phải là một chuẩn, nên $N_F(q)$ khác không, và $q$ khả nghịch.

#### Nhận xét {#alg-viii-s19-n4-rem-1 .statement tag=00RQ}

Giả sử rằng đại số quaternion F là một trường. Từ đẳng thức $j^2=\gamma$ suy ra $\gamma \not= 0$. Theo Mệnh đề 2 của VIII, p. 363, tâm của F bằng K trừ khi K có đặc số 2 và $\beta$ bằng không; trong trường hợp đó đại số F là giao hoán.

### 5. Các Đại số trên các Trường Cực đại được Sắp thứ tự

Cho R là một trường có thứ tự cực đại (VI, §2, No. 5, p. 25). Cho C là đại số bậc hai trên R kiểu $(-1,0)$; nếu $(1, i)$ là cơ sở chính tắc của nó, thì ta có $i^2=-1$. Hơn nữa, C là một bao đóng đại số của R (VI, §2, No. 6, p. 26, Định lý 3). Cho H là đại số quaternion trên R kiểu $(-1,0,-1)$. Bảng phép nhân của H trong cơ sở chính tắc $(1, i, j, k)$ của nó được cho bởi

$$
i^2=j^2=k^2=-1,ij=-ji=k,-ik=ki=j ,jk=-kj=i
$$

Ta đồng nhất C với đại số con $R + Ri$ của H. Phần tử liên hợp của một phần tử $q=x+yi+zj+tk$ của H là $\overline{q}=x-yi-zj-tk$. Vết Cayley và chuẩn của $q$ được cho bởi

$$
T(q) =q+\overline{q}= 2x ,N(q) =qq=x^2+y^2+z^2+t^2
$$

Vì R là một trường có thứ tự, ta có $N(q)>0$ nếu $q\not= 0$, nên H là một trường, với tâm là R (VIII, p. 363, Mệnh đề 2). Vết rút gọn và chuẩn của một phần tử $q$ của H lần lượt là $T(q)$ và $N(q)$.

#### Định lý 1 {#alg-viii-s19-thm-1 .statement tag=00M1}

Cho D là một đại số trên R bậc hữu hạn đồng thời là một trường. Khi đó D đẳng cấu với R, C, hoặc H.

Ký hiệu tâm của D là Z, và gọi L là một trường con giao hoán cực đại của D. Ta có $[D : Z] = [L : Z]^2$ theo VIII, p. 265, Hệ quả 2; ta cũng có $[L : R]\leqslant 2$ vì C là một bao đóng đại số của R. Do đó có ba trường hợp có thể xảy ra:

a) Ta có R = Z = L, nên [D : Z] = 1 và D = R.

b) Ta có $R\not= Z$ và Z = L, nên [D : Z] = 1 và D = L. Trong trường hợp này, D đẳng cấu với C.

c) Ta có R = Z và [L : R] = 2, nên [D : R] = 4. Theo Mệnh đề 4 của VIII, p. 364, đại số trên R D đẳng cấu với một đại số quaternion kiểu $(\alpha ,0, \gamma )$, trong đó $\alpha$ và $\gamma$ là những phần tử khác không của R. Lấy $i\in D$- Z sao cho $i^2=\alpha$. Ta có $\alpha \not= 0$. Nếu $\alpha  >0$, thì tồn tại $a\in R$ sao cho $a^2=\alpha$ (VI, §2, No. 6, p. 26, Định lý 3); khi đó ta có $(a-i)(a+i) = 0$, điều này vô lý vì D là một trường. Vậy ta có $\alpha  <0$. Bất đẳng thức $\gamma  <0$ được chứng minh tương tự. Khi đó tồn tại các phần tử $a$ và $c$ của $R^*$ sao cho $\alpha =-a^2$ và $\gamma =-c^2$ (loc. cit.). Do đó đại số D đẳng cấu với đại số quaternion kiểu $(-1,0,-1)$ (VIII, p. 362, Nhận xét 2), tức là với H.

#### Nhận xét 1 {#alg-viii-s19-n5-rem-1 .statement tag=00M2}

Cho O là đại số octonion kiểu $(-1,0,-1,-1)$ trên R (III, Phụ lục, No. 3, p. 615). Cho D là một đại số thay thế Cayley trên R sao cho mọi phần tử khác không của D đều có một nghịch đảo. Có thể chứng minh (VIII, p. 370, Bài tập 5) rằng D đẳng cấu với R, C, H, hoặc O.

#### Nhận xét 2 {#alg-viii-s19-n5-rem-2 .statement tag=00M3}

Điều trên áp dụng cho trường $\mathbf{R}$ của các số thực. Mọi $\mathbf{R}$-đại số bậc hữu hạn là một trường đều đẳng cấu với $\mathbf{R},\mathbf{C}$, hoặc $\mathbf{H}$.

#### Nhận xét 3 {#alg-viii-s19-n5-rem-3 .statement tag=00M4}

Cho A là một đại số định chuẩn trên trường $\mathbf{R}$. Giả sử rằng A là một trường. Khi đó A đẳng cấu với $\mathbf{R},\mathbf{C}$, hoặc $\mathbf{H}$ (“định lý Gelfand–Mazur”) (xem Comm. Alg., VI, §6, No. 4, p. 407, Định lý 1 và TS, I, §2, n$^o5$, p. 26, hệ quả $2$)$.*$

### Bài tập {#alg-viii-s19-exercises}

Xem [các bài tập cho § 19](exercises/s19/).

[^1]: Trong trường hợp $\beta = 0$, người ta cũng nói rằng F là một đại số quaternion kiểu $(\alpha , \gamma )$.
