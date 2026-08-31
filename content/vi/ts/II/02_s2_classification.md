---
book: ts
book_title: Théories spectrales
chapter: II
chapter_title: GROUPES LOCALEMENT COMPACTS COMMUTATIFS
section: 2
section_title: Classification
lang: vi
source: ts-i-ii-fr
book_pages: TS II.244-TS II.250, TS II.304-TS II.308
pdf_pages: 0256-0262, 0316-0320
extraction: native
subsections:
    - "no": 1
      title: Groupes engendrés par une partie compacte
      page: 244
      pdf_page: 256
    - "no": 2
      title: Cas général
      page: 248
      pdf_page: 260
statements: 16
exercises: 14
content_sha256: a4b12bd54f1b4a46ef355d2c8fde9b87b6597b102b7459830359a9e8d5452124
translated_from: content/en-mt/ts/II/02_s2_classification.md
source_lang: en-mt
translation_method: machine
source_content_sha256: 6f1b6064fcac59396f70dfbd8ef9fe406fd9804439e01fc66754a0819308254b
translation_model: gpt-5.4
translation_run: translate-vi-f2ccc77a
glossary_version: 34
glossary_terms_sha256: 2ca5eee15117859f6e7aca1190e46ddc494d923c77ae75b96b011e6e8f83f46a
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 2. PHÂN LOẠI

### 1. Các nhóm sinh bởi một tập con compact

#### Bổ đề 1 {#ts-ii-s2-lem-1 .statement tag=02M9}

Cho H là một nhóm địa phương compact, và cho R là một trong hai nhóm $\mathbf{R}$ hoặc $\mathbf{Z}$. Cho $\varphi$ là một cấu xạ liên tục từ R vào H. Nếu $\varphi$ không phải là một đẳng cấu tôpô từ R lên một nhóm con của H, thì ảnh của R trong H là tương đối compact.

Gọi I là ảnh của $\varphi$. Sau khi thay thế H bằng $\overline{I}$, ta có thể giả sử rằng I trù mật trong H. Khi đó ta phải chứng minh rằng H là compact nếu $\varphi$ không phải là một đẳng cấu tôpô từ R lên I.

Giả sử tồn tại một lân cận V của $e$ trong H và một số nguyên $M>0$ sao cho, với mọi $t >M$ trong R, ta có $\varphi (t)\notin V$. Khi đó $\varphi$ là đơn ánh: nếu $\varphi (u) =e$, thì $\varphi (nu) =e$ với mọi số nguyên $n\geqslant 1$, do đó tập $\mathbf{N}u$ bị chặn trong R, điều đó có nghĩa là $u= 0$. Vì vậy hạn chế của $\varphi$ lên $[-M,M]\cap R$ là một đồng phôi lên ảnh của nó, ảnh này chứa $V\cap I$. Vì hạn chế của $\varphi^{-1}$ lên $V\cap I$ là liên tục, suy ra $\varphi$ là một đẳng cấu tôpô từ R lên I.

Bây giờ giả sử $\varphi$ không phải là một đẳng cấu tôpô từ R lên I. Cho W là một lân cận mở tương đối compact của $e$ trong H, và cho V là một lân cận đối xứng của $e$ sao cho $V^2\subset W$. Với mọi $x\in$ H = I, tồn tại một phần tử $s\in$ R sao cho $x\in \varphi (s)V$. Theo đoạn trước và giả thiết về $\varphi$, tồn tại $t\in$ R sao cho $t >|s|$ và $\varphi (t)\in V$. Khi đó ta có $x\in \varphi (t+s)\varphi (t)^{-1}V\subset \varphi (t+s)W$, và $t+s >0$. Do đó, các tập mở $\varphi (u)W$ với $u >0$ tạo thành một phủ mở của H. Vì W là tương đối compact, tồn tại một số nguyên $n\geqslant 1$ và các phần tử $u_1, . . . , u_n$ của R, dương ngặt, sao cho $W\subset \bigcup_{1\leqslant i\leqslant n}\varphi (u_i)W$. Gọi U là phần tử lớn nhất trong các $u_i$.

Cho $x\in H$ và đặt $s=$ inf$\{t\in R|t\geqslant 0,\varphi (t)x^{-1}\in \overline{W}\}$. Vì $\overline{W}$ là compact, khi đó ta có $\varphi (s)x^{-1}\in \overline{W}$. Tồn tại một số nguyên $i$ sao cho $\varphi (s)x^{-1}\in \varphi (u_i)W$, do đó $\varphi (s-u_i)x^{-1}\in \overline{W}$. Định nghĩa của $s$ kéo theo $s-u_i<0$, do đó $s\leqslant U$. Suy ra $H =\varphi ([0,U]\cap R)W$ là compact.

#### Bổ đề 2 {#ts-ii-s2-lem-2 .statement tag=02MA}

Nếu G được sinh bởi một tập con compact V, thì tồn tại một số nguyên $n\geqslant 0$ và một nhóm con rời rạc D của G đẳng cấu với $\mathbf{Z}^n$ sao cho $G/D$ là compact.

Sau khi thay thế V bằng $V\cup V^{-1}$, ta có thể giả sử rằng V là đối xứng; khi đó giả thiết có nghĩa là G là hợp của các tập $V^n$ với $n\in \mathbf{N}$.

Vì $V^2$ là compact, tồn tại một số nguyên $k\geqslant 1$ và các phần tử $x_1, . . . , x_k\in G$ sao cho $V^2\subset \bigcup_{1\leqslant i\leqslant k}x_iV$. Gọi $D_0$ là nhóm con của G sinh bởi họ $(x_i)_{1\leqslant i\leqslant k}$. Ta có $V^2\subset D_0V$, do đó bằng quy nạp $V^n\subset D_0V$ với mọi số nguyên $n\geqslant 1$, và vì thế $G = D_0V$ vì V sinh ra G. Khi đó gọi J là một tập con của $\{1,2, . . . , k\}$ sao cho nhóm con D sinh bởi họ $(x_i)_{i\in J}$ đẳng cấu tôpô với $\mathbf{Z}^{Card(J)}$, và cực đại đối với tính chất này. Hãy chứng minh rằng $G/D$ là compact.

Gọi $p$ là toàn cấu chính tắc từ G lên $G/D$. Gọi $i\in  \{1,2, . . . , k\}-J$. Nếu nhóm con $H_i$ của $G/D$ sinh bởi $p(x_i)$ đẳng cấu tôpô với $\mathbf{Z}$, thì nhóm con của G sinh bởi D và $x_i$ là rời rạc và ánh xạ $(d, n)\mapsto dx^n_i$ là một đẳng cấu từ $D\times \mathbf{Z}$ lên nhóm con này, trái với tính cực đại của J. Do đó Bổ đề 1 suy ra rằng $\overline{H}_i$ là compact. Vậy $G/D = (\prod_{i\notin J}\overline{H}_i)p(V)$ là compact

#### Bổ đề 3 {#ts-ii-s2-lem-3 .statement tag=02MB}

Cho A và B là các nhóm giao hoán sao cho A chia được. Gọi C là một nhóm con của B và $\varphi$ là một cấu xạ từ C vào A. Tồn tại một cấu xạ từ B vào A mở rộng $\varphi$.

Cho $\mathscr{O}$ là tập hợp các cặp $(X, f)$, trong đó X là một nhóm con của B chứa C và $f$ là một cấu xạ từ X vào A mở rộng $\varphi$. Hãy sắp thứ tự $\mathscr{O}$ bởi quan hệ “ $X\subset X'$ và $f'$ mở rộng $f$ ”. Ta kiểm tra được rằng $\mathscr{O}$ là quy nạp. Cho $(X, f)$ là một phần tử cực đại của $\mathscr{O}$ (E, III, p. 20 , Theorem 2). Nếu $X\not= B$, lấy một phần tử $b$ của B-X và gọi $X'$ là nhóm con sinh bởi X và $b$. Tính giao hoán của B cho thấy rằng $X'$ là tập hợp các phần tử $b^nx$ với $n\in \mathbf{Z}$ và $x\in X$. Trước hết giả sử rằng $b^n\notin X$ với mọi số nguyên $n\not= 0$ và định nghĩa $f'$ từ $X'$ vào A bằng cách lấy một phần tử tùy ý $y\in A$ và đặt $f'(b^nx) =y^nf(x)$ với mọi $n\in \mathbf{Z}$ và mọi $x\in X$. Vì A là giao hoán, $f'$ là một cấu xạ, và nó mở rộng $f$. Bây giờ giả sử tồn tại $n\not= 0$ sao cho $b^n\in X$ và gọi $m >0$ sao cho $m\mathbf{Z}=\{n\in \mathbf{Z}|b^n\in X\}$. Vì A là chia được, tồn tại một phần tử $y\in A$ sao cho $y^m=f(b^m)$. Khi đó ta mở rộng $f$ thành một cấu xạ từ $X'$ vào A bởi $f'(b^nx) =y^nf(x)$ với $n\in  \{0,1, . . . , m-1\}$ và $x\in X$. Trong cả hai trường hợp, $(X, f)$ sẽ không cực đại. Vậy X = B và bổ đề được chứng minh.

#### Nhận xét {#ts-ii-s2-n1-rem-1 .statement tag=02MC}

Theo ngôn ngữ các phạm trù, bổ đề nói rằng các nhóm chia được là các đối tượng đơn ánh trong phạm trù các nhóm giao hoán; xem A, VII, p. 53, bài tập 3.

#### Mệnh đề 1 {#ts-ii-s2-prop-1 .statement tag=02MD}

Các điều kiện sau là tương đương:

(i) G được sinh bởi một tập con compact;

(ii) tồn tại các số nguyên dương $p$ và $q$ và một nhóm compact K sao cho G đẳng cấu với $\mathbf{R}^p\times \mathbf{Z}^q\times K$;

(iii) tồn tại một số nguyên $n\geqslant 0$ sao cho $\widehat{G}$ đẳng cấu địa phương với $\mathbf{R}^n$;

(iv) tồn tại các số nguyên dương $p$ và $q$ và một nhóm rời rạc D sao cho $\widehat{G}$ đẳng cấu với $\mathbf{R}^p\times \mathbf{T}^q\times D$.

(i) $=\Rightarrow$ (iii) : nếu G có tính chất (i), tồn tại một số nguyên $n\geqslant 0$ và một nhóm con D của G đẳng cấu với $\mathbf{Z}^n$ sao cho $G/D$ là compact (bổ đề 2). Khi đó $D^{\bot}$, được đồng nhất với đối ngẫu của $G/D$, là rời rạc (Định lý 4 của II, p. 226 và mệnh đề 18 của II, p. 233). Do đó $\widehat{G}$ đẳng cấu địa phương với $\widehat{G}/D^{\bot}$, nghĩa là với $\widehat{D}$, đẳng cấu với $\mathbf{T}^n$ (Định lý 4 của II, p. 226 và mệnh đề 18 của II, p. 233). Bây giờ $\mathbf{T}^n$ đẳng cấu địa phương với $\mathbf{R}^n$.

(iii) $=\Rightarrow$ (iv) : nếu $\widehat{G}$ đẳng cấu địa phương với $\mathbf{R}^n$, tồn tại một số nguyên $p$ sao cho $0\leqslant p\leqslant n$ sao cho thành phần liên thông của đơn vị $\widehat{G}_0$ của $\widehat{G}$ là một nhóm con mở đẳng cấu với $\mathbf{R}^p\times \mathbf{T}^{n-p}$ (TG, VII, p. 13, Định lý 1). Đặc biệt, $\widehat{G}_0$ là một nhóm chia được. Khi đó ta áp dụng bổ đề 3 cho ánh xạ đồng nhất của nhóm con $\widehat{G}_0$ của nhóm $\widehat{G}$ vào nhóm chia được $\widehat{G}_0$. Do đó tồn tại một cấu xạ $\pi$ của $\widehat{G}$ vào $\widehat{G}_0$ là ánh xạ đồng nhất trên $\widehat{G}_0$. Do đó, ta có $\pi \circ \pi =\pi$, và $\pi$ là một phép chiếu. Nó liên tục, vì hạn chế của nó trên nhóm con mở $\widehat{G}_0$ là như vậy. Suy ra $\widehat{G}$ là tích trực tiếp của $\widehat{G}_0$ và nhóm con $\overset{-1}{\pi}(e)$, nhóm này là rời rạc vì nó đẳng cấu với $\widehat{G}/\widehat{G}_0$ (TG, III, p. 47, hệ quả)

(iv) $=\Rightarrow$ (ii) : suy ra từ mệnh đề 2 của II, p. 206, từ mệnh đề 18 của II, p. 233 và từ hệ quả 3 của II, p. 236.

(ii) $=\Rightarrow$ (i) : với mọi nhóm compact K, nhóm $\mathbf{R}^p\times \mathbf{Z}^q\times K$ được sinh bởi tập compact $[0,1]^p\times  \{0,1\}^q\times K$.

#### Hệ quả 1 {#ts-ii-s2-prop-1-cor-1 .statement tag=02ME}

Giả sử rằng G được sinh bởi một lân cận compact của $e$.

a) Tồn tại một nhóm con compact K của G và các số nguyên dương $p$ và $q$ sao cho G đẳng cấu với $\mathbf{R}^p\times \mathbf{Z}^q\times K$.

b) Ngược lại, cho K là một nhóm compact, cho $p$ và $q$ là các số nguyên dương, và cho G là một nhóm đẳng cấu với $\mathbf{R}^p\times \mathbf{Z}^q\times K$. Khi đó K là nhóm con compact cực đại duy nhất của G, và các số nguyên $(p, q)$ được xác định một cách duy nhất bởi G.

Mệnh đề a) suy ra từ mệnh đề 1. Bây giờ cho K là một nhóm compact, và cho $p,q$ là các số nguyên dương. Giả sử rằng G đẳng cấu với nhóm $\mathbf{R}^p\times \mathbf{Z}^q\times K$, và đồng nhất G với nhóm này. Bởi phép chiếu chính tắc của G lên $\mathbf{R}^p\times \mathbf{Z}^q$, ảnh của mọi nhóm con compact của G là một nhóm con compact của $\mathbf{R}^p\times \mathbf{Z}^q$, và do đó bị thu về phần tử đơn vị. Vậy $K'\subset K$ và K là nhóm con compact lớn nhất của G. Nhóm con $\mathbf{R}^p\times K$ cũng là duy nhất vì $\mathbf{R}^p$ là thành phần liên thông của đơn vị của $G/K$. Theo TG, VII, p. 13, hệ quả 3, số nguyên $p$ được xác định một cách duy nhất bởi G. Vì $G/(\mathbf{R}^p\times K)$ đẳng cấu với $\mathbf{Z}^q$, số nguyên $q$ cũng vậy được xác định một cách duy nhất bởi G.

#### Nhận xét {#ts-ii-s2-n1-rem-2 .statement tag=02MF}

Theo đối ngẫu, $\widehat{G}$ đẳng cấu với $\mathbf{R}^p\times \mathbf{T}^q\times D$ (mệnh đề 3 (iv)), trong đó các nhóm con $\mathbf{R}^p\times \mathbf{T}^q$ và $\mathbf{T}^q$, cùng các số nguyên $p$ và $q$, được xác định một cách duy nhất.

#### Hệ quả 2 {#ts-ii-s2-prop-1-cor-2 .statement tag=02MG}

Các điều kiện sau là tương đương:

(i) Các nhóm G và $\widehat{G}$ được sinh bởi các tập con compact ;

(ii) Tồn tại các số nguyên dương $n$ và $m$ sao cho G đẳng cấu địa phương với $\mathbf{R}^m$ và $\widehat{G}$ đẳng cấu địa phương với $\mathbf{R}^n$;

(iii) Tồn tại các số nguyên dương $p,q$ và $r$ và một nhóm hữu hạn A sao cho G đẳng cấu với $\mathbf{R}^p\times \mathbf{T}^q\times \mathbf{Z}^r\times A$ ;

(iv) Tồn tại các số nguyên dương $p,q$ và $r$ và một nhóm hữu hạn A sao cho $\widehat{G}$ đẳng cấu với một tích $\mathbf{R}^p\times \mathbf{Z}^q\times \mathbf{T}^r\times A$.

Ta có (i) $\Leftrightarrow$ (ii) theo mệnh đề 1, và (iii) $\Leftrightarrow$ (iv) theo đối ngẫu, do đó (iii) $\Rightarrow$ (i). Cuối cùng, nếu (i) đúng, thì $\widehat{G}$ đẳng cấu với $\mathbf{R}^p\times \mathbf{T}^r\times D$ trong đó D là rời rạc (mệnh đề 1). Nhóm D được sinh bởi một tập con compact, do đó hữu hạn, của D. Do đó, tồn tại $q\geqslant 0$ sao cho D đẳng cấu với $\mathbf{Z}^q\times A$, trong đó A là một nhóm hữu hạn (A, VII, p. 22, định lý 3).

#### Nhận xét {#ts-ii-s2-n1-rem-3 .statement tag=02MH}

Với các ký hiệu của hệ quả 2, nếu ta đồng nhất G với $\mathbf{R}^p\times$ $\mathbf{T}^q\times \mathbf{Z}^r\times A$, thì nhóm con $\mathbf{R}^p\times \mathbf{T}^q$ là thành phần trung hoà của G, nhóm con $\mathbf{T}^q\times A$ là nhóm con compact lớn nhất của nó và $\mathbf{T}^q$ là thành phần trung hoà của nhóm sau; các số nguyên $p, q, r$ được xác định một cách duy nhất bởi G theo nhận xét trước, và nhóm A được xác định bởi G tới đẳng cấu.

#### Mệnh đề 2 {#ts-ii-s2-prop-2 .statement tag=02MI}

Giả sử G compact. Tồn tại một họ lọc giảm $(H_i)_{i\in I}$ các nhóm con đóng của G sao cho

a) nhóm G được đồng nhất với giới hạn xạ ảnh của các $G/H_i$;

b) với mọi $i$, tồn tại một số nguyên $q\geqslant 0$ và một nhóm hữu hạn A sao cho $G/H_i$ đẳng cấu với $\mathbf{T}^q\times A$.

Thật vậy, $\widehat{G}$ là rời rạc (mệnh đề 18 của II, p. 233), do đó là hợp của một họ lọc tăng $(D_i)_{i\in I}$ các nhóm con kiểu hữu hạn. Đặt $H_i= D^{\bot}_i$ ; nhóm G được đồng nhất với giới hạn xạ ảnh của các $G/H_i($II, p. 234, hệ quả 3), và $(H_i)$ là một họ lọc giảm.

Cho $i\in I$. Tồn tại một số nguyên $q\geqslant 0$ và một nhóm hữu hạn A sao cho nhóm $D_i$ đẳng cấu với $\mathbf{Z}^q\times A$ (A, VII, p. 22, định lý 3), do đó $G/H_i$ đẳng cấu với $\mathbf{T}^q\times \widehat{A}($x. hệ quả 1 của II, p. 232).

#### Hệ quả {#ts-ii-s2-n1-cor-1 .statement tag=02MJ}

Nếu nhóm G được sinh bởi một tập con compact, thì nó là một giới hạn xạ ảnh của các nhóm đẳng cấu với các nhóm dạng $\mathbf{R}^p\times \mathbf{T}^q\times \mathbf{Z}^r\times A$, trong đó A là một nhóm hữu hạn và $p,q,r$ là các số nguyên dương.

Theo (ii) của mệnh đề 1 của II, p. 246, hệ quả suy ra từ mệnh đề 2.

### 2. Trường hợp tổng quát

Trong số này, G ký hiệu một nhóm giao hoán compact địa phương.

#### Mệnh đề 3 {#ts-ii-s2-prop-3 .statement tag=02MK}

a) Tồn tại một số nguyên $n\geqslant 0$ và một nhóm con L sao cho G là tích trực tiếp của L và một nhóm con đẳng cấu với $\mathbf{R}^n$, và hơn nữa L có một nhóm con compact mở K sao cho $L/K$ là rời rạc;

b) Nhóm G là hợp của một họ lọc tăng các nhóm con mở, mỗi nhóm trong đó là một giới hạn xạ ảnh của các nhóm đẳng cấu với các nhóm dạng $\mathbf{R}^p\times \mathbf{T}^q\times \mathbf{Z}^r\times A$, trong đó A là một nhóm hữu hạn và $p,q,r$ là các số nguyên dương.

Chứng minh b). Với mọi lân cận compact V của $e$, ký hiệu bởi $G_V$ nhóm con của G sinh bởi V. Nó là mở, và theo hệ quả của Mệnh đề 2, nhóm $G_V$ là giới hạn xạ ảnh của các nhóm dạng $\mathbf{R}^p\times \mathbf{T}^q\times \mathbf{Z}^r\times A$, trong đó A là một nhóm compact và $p,q$ và $r$ thuộc $\mathbf{N}$. Khi V chạy qua các lân cận compact của $e$, các nhóm con $G_V$ này tạo thành một họ lọc (vì $G_V$ và $G_W$ được chứa trong $G_{V\cup W}$ với mọi lân cận compact V và W của $e$). Sau hết, nhóm G là hợp của các nhóm con $G_V$.

Cho H là một nhóm con mở của G sinh bởi một lân cận compact của $e$. Tồn tại một nhóm compact K và các số nguyên dương $p$ và $q$ sao cho H đẳng cấu với $\mathbf{R}^p\times \mathbf{Z}^q\times K$ (Mệnh đề 1 của II, p. 246); đồng nhất H với tích này. Toàn cấu chính tắc của H lên nhóm chia được $\mathbf{R}^p$ mở rộng thành một cấu xạ $\pi$ của G lên $\mathbf{R}^p$ (Bổ đề 3 của II, p. 245). Đó là một phép chiếu $\pi$ của G lên $\mathbf{R}^p$, liên tục vì hạn chế của nó lên nhóm con mở H là liên tục. Do đó G là tích trực tiếp của $\mathbf{R}^p$ và hạt nhân L của $\pi$ (TG, III, p. 47, hệ quả). Ta có $\mathbf{Z}^q\times K = H\cap L$, nên $\mathbf{Z}^q\times K$ là một nhóm con mở của L. Vì thế K là một nhóm con compact mở của L, và do đó $L/K$ là rời rạc.

#### Mệnh đề 4 {#ts-ii-s2-prop-4 .statement tag=02ML}

Cho $B_G$ là tập hợp các phần tử của G sinh ra một nhóm con tương đối compact của G. Khi đó $B_G$ là một nhóm con đóng của G và $B^{\bot}_G$ là thành phần liên thông của đơn vị của $\widehat{G}$.

Tập hợp $B_G$ là một nhóm con của G vì tích của hai tập con compact của G là một tập con compact của G.

Cho H là một nhóm con mở của G sinh bởi một lân cận compact của $e$. Tồn tại các số nguyên dương $p$ và $q$ và một nhóm compact K sao cho nhóm con H đẳng cấu với $\mathbf{R}^p\times \mathbf{Z}^q\times K$ (Mệnh đề 1 của II, p. 246). Nếu đồng nhất các nhóm này, ta thấy rằng $B_G\cap H = K$ là đóng trong H. Vì họ các nhóm con mở H sinh bởi các lân cận compact là một phủ mở của G (chẳng hạn, $x$ thuộc nhóm con sinh bởi $U\cap  \{x\}$ với mọi lân cận compact cố định U của $e$), suy ra $B_G$ là đóng.

Bây giờ ta tính $B^{\bot}_G$. Theo Mệnh đề 3, a), tồn tại một số nguyên dương $n\geqslant 0$ và một nhóm L nhận một nhóm con compact mở sao cho G có thể được đồng nhất với $\mathbf{R}^n\times L$. Khi đó $B_G$ được đồng nhất với $\{0\} \times B_L$, và $B^{\bot}_G$ với $\mathbf{R}^n\times B^{\bot}_L$. Vì vậy ta quy được về trường hợp G = L nhận một nhóm con compact mở K.

Khi đó ta có $K\subset B_G$; nếu đồng nhất $G/\widehat{K}$ với $K^{\bot}$ (Định lý 4 của II, p. 226), trực giao $(B_G/K)^{\bot}$ của $B_G/K$ trong $\widehat{G}/K$ được đồng nhất với $B^{\bot}_G$. Nhưng mặt khác $B_G/K = B_{G/K}$, và vì $K^{\bot}$ là một nhóm con mở của $\widehat{G}$ (Hệ quả 2 của II, p. 233), thành phần liên thông $\widehat{G}_0$ của $\widehat{G}$ cũng là thành phần liên thông của $K^{\bot}$ (TG, III, p. 35, Prop. 14). Do đó mệnh đề đối với nhóm rời rạc $G/K$ là tương đương với mệnh đề đối với G.

Sau hết, giả sử G là rời rạc. Khi đó nhóm $\widehat{G}$ là compact (Prop. 18 của II, p. 233). Thành phần liên thông $(\widehat{G})_0$ là giao của các nhóm con mở của $\widehat{G}$ (TG, III, p. 35, Prop. 14) và một nhóm con của $\widehat{G}$ là mở khi và chỉ khi nó đóng và có chỉ số hữu hạn, hay tương đương, khi trực giao của nó là hữu hạn (Corollary 2 của II, p. 233); Corollary 4 của II, p. 228 cho thấy rằng $(\widehat{G})^{\bot}_0$ là hợp của các nhóm con hữu hạn của G, mà không là gì khác ngoài $B_G$ vì G là rời rạc. Ta kết luận bằng đối ngẫu.

#### Hệ quả 1 {#ts-ii-s2-prop-4-cor-1 .statement tag=02MM}

Giả sử G compact. Khi đó các điều kiện sau là tương đương:

(i) Nhóm G là liên thông;

(ii) Nhóm $\widehat{G}$ không có xoắn;

(iii) Nhóm G chia được.

Điều này suy ra từ Mệnh đề 4 và Hệ quả 7 của II, p. 229 vì $B_G= G$.

#### Hệ quả 2 {#ts-ii-s2-prop-4-cor-2 .statement tag=02MN}

Giả sử G compact. Khi đó G là hoàn toàn gián đoạn nếu và chỉ nếu $\widehat{G}$ là một nhóm xoắn.

Nhóm G là hoàn toàn gián đoạn khi và chỉ khi thành phần liên thông của nó thu về $\{e\}$; Mệnh đề 4 cho thấy điều kiện này tương đương với $B_{\widehat{G}}=\widehat{G}$. Vì nhóm $\widehat{G}$ là rời rạc (Prop. 18 của II, p. 233), điều này có nghĩa là mọi phần tử của $\widehat{G}$ sinh ra một nhóm hữu hạn, do đó $\widehat{G}$ là xoắn.

#### Hệ quả 3 {#ts-ii-s2-prop-4-cor-3 .statement tag=02MO}

Nếu G là liên thông, thì G chia được.

Thật vậy, tồn tại một nhóm compact liên thông K và một số nguyên $n\geqslant 0$ sao cho G đẳng cấu với $\mathbf{R}^n\times K$ (II, p. 248, Prop. 3, trong đó phải có L = K). Hệ quả 1 cho thấy K chia được, và do đó G chia được.

## BÀI TẬP {#ts-ii-s2-exercises}

Xem [các bài tập của § 2](exercises/s2/).
