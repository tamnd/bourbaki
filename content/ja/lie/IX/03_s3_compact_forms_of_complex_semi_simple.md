---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: IX
chapter_title: COMPACT REAL LIE GROUPS
section: 3
section_title: Compact forms of complex semi-simple Lie algebras
lang: ja
source: lie-vii-ix
book_pages: 296-303, 394-396
pdf_pages: 0303-0310, 0401-0403
extraction: native+ocr
subsections:
    - "no": 1
      title: REAL FORMS
      page: 296
      pdf_page: 303
    - "no": 2
      title: REAL FORMS ASSOCIATED TO A CHEVALLEY SYSTEM
      page: 297
      pdf_page: 304
    - "no": 3
      title: CONJUGACY OF COMPACT FORMS
      page: 299
      pdf_page: 306
    - "no": 4
      title: 'EXAMPLE I: COMPACT ALGEBRAS OF TYPE A$_{\boldsymbol{n}}$'
      page: 300
      pdf_page: 307
    - "no": 5
      title: 'EXAMPLE II: COMPACT ALGEBRAS OF TYPE B$_{\boldsymbol{n}}\mathbf{A}\mathbf{N}\mathbf{D}$ $\mathbf{D}_{\boldsymbol{n}}$'
      page: 301
      pdf_page: 308
    - "no": 6
      title: COMPACT GROUPS OF RANK 1
      page: 302
      pdf_page: 309
statements: 17
exercises: 9
content_sha256: 9154b052c0dcd35fc0fd332e438d049ffb7eb37c4003a60177d0ca6fca80653b
translated_from: content/en/lie/IX/03_s3_compact_forms_of_complex_semi_simple.md
translation_method: google
source_content_sha256: bf0ebd0cda151170c108a2f9b899a1c59ba20dd5f6195c4caf5f17e7cc05a3cd
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: b33d1192db113df2e05083310ad05d38a81ff4d2d36f5a82cffa4f389c15d332
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## § 3。コンパクトな形/複素半単純リー代数

### 1. リアル形

$\mathfrak{a}$ が複素数リー代数である場合、スカラーの制限によって得られる実数リー代数を $\mathfrak{a}_{[\mathbf{R}]}$ (またはときどき $\mathfrak{a}$) で表します。 $\mathfrak{g}$ が実数リー代数である場合、スカラーの拡大によって得られる複素数リー代数 $\mathbf{C}\otimes_{\mathbf{R}}\mathfrak{g}$ を $\mathfrak{g}_{(\mathbf{C})}$ (またはときどき $\mathfrak{g}_{\mathbf{C}}$) で表します。 実リー代数 $\mathfrak{g}\rightarrow \mathfrak{a}_{[\mathbf{R}]}$ の準同型性は、複素リー代数 $\mathfrak{g}_{(\mathbf{C})}\rightarrow \mathfrak{a}:$ の準同型性と全単射的に対応します。$f:\mathfrak{g}\rightarrow \mathfrak{a}_{[\mathbf{R}]}$ と $g:\mathfrak{g}_{(\mathbf{C})}\rightarrow \mathfrak{a}$ が対応する場合、$x\in \mathfrak{g}, \lambda \in \mathbf{C}$ に対して $f(x) =g(1\otimes x)$ と $g(\lambda \otimes x) =\lambda f(x)$ が得られます。

#### 定義 1 {#lie-ix-s3-def-1 .statement tag=01B1}

$\mathfrak{a}$ を複素数リー代数とします。 $\mathfrak{a}$の実数形は、$\mathfrak{a}$の実数部分代数$\mathfrak{g}$であり、$\mathbf{C}$ベクトル空間$\mathfrak{a}($代数上の$\mathbf{R}$構造です。 II, §8, no. 1、デフォルト。 1)。

これは、標準単射 $\mathfrak{g}\rightarrow \mathfrak{a}_{[\mathbf{R}]}$ に関連付けられた複素数リー代数 $\mathfrak{g}_{(\mathbf{C})}\rightarrow \mathfrak{a}$ の準同型が全単射であることを意味します。したがって、実数ベクトル空間 $\mathfrak{a}$ の部分空間 $\mathfrak{g}$ と $i\mathfrak{g}$ が相補的である場合に限り、$\mathfrak{a}$ の実数部分代数 $\mathfrak{g}$ は、$\mathfrak{a}$ の実数形となります。実数形 $\mathfrak{g}$ に対する $\mathfrak{a}$ の共役は、次のように写像 $\sigma :\mathfrak{a}\rightarrow \mathfrak{a}$ です。

$$
\sigma (x+iy) =x-iy,x, y\in \mathfrak{g} \tag{1}
$$

#### 命題 1 {#lie-ix-s3-prop-1 .statement tag=01JF}

$a)$ $\mathfrak{g}$ を $\mathfrak{a}$ の実数形と、$\mathfrak{g}$ に対する $\mathfrak{a}$ の共役$\sigma$ とします。それから：

$\sigma^2=$ ID$_{\mathfrak{a}}, \sigma (\lambda x+\mu y) = \overline{\lambda \sigma}(x) + \overline{\mu\sigma}(y),[\sigma (x), \sigma (y)] =\sigma [x, y]$ (2)

$\lambda , \mu\in \mathbf{C},x, y\in \mathfrak{a}$の場合。 $\sigma (x) =x$ の場合に限り、$\mathfrak{a}$ 属するから $\mathfrak{g}$ までの元 $x$。

b) $\sigma :\mathfrak{a}\rightarrow \mathfrak{a}$ を写像満たす (2) とします。 このとき、$\sigma$の不動点の集合$\mathfrak{g}$は$\mathfrak{a}$の実数形であり、$\sigma$は$\mathfrak{g}$に対する$\mathfrak{a}$の共役です。

証明は明らかです。

Bが$\mathfrak{a}$の殺害形を表し、$\mathfrak{g}$が$\mathfrak{a}$の実形である場合、$\mathfrak{g}$に対するBの制限は$\mathfrak{g}$の殺害形であることに注意してください。特に、B は $\mathfrak{g}\times \mathfrak{g}$ の実数値です。 $\mathfrak{a}$ が還元的であると仮定します。その場合、実数リー代数 $\mathfrak{g}$ は、B から $\mathfrak{g}$ の制限が負 (§1, no. 3) である場合にのみコンパクトです。この場合、$\mathfrak{g}$ は $\mathfrak{a}$ の圧縮実数形であると言います。

### 2. シュバレー 系に関連付けられたレアル形

In this number, we consider a split semi-simple Lie algebra $(\mathfrak{a},\mathfrak{h})$ over the field $\mathbf{C}$ (Chap. VIII, §2, no. 1), with root system $R(\mathfrak{a},\mathfrak{h}) = R$, and a Chevalley system $(X_{\alpha})_{\alpha\in R}$ of $(\mathfrak{a},\mathfrak{h})$ (Chap. VIII, §2, no. 4, Def. 3).

$\mathfrak{h}$ 上の $-$Id$_{\mathfrak{h}}$ と一致し、すべての $\alpha \in R$ について $X_{\alpha}$ から $X_{-\alpha}$ を写像する線形写像 $\theta :\mathfrak{a}\rightarrow \mathfrak{a}$ は、$\mathfrak{a}$ の自己同型であることを思い出してください (上記参照)。 さらに (上記引用、提案 7)、$\alpha , \beta , \alpha +\beta$ が根である場合、

$$
[X_{\alpha}, X_{\beta}] = N_{\alpha ,\beta}X_{\alpha+\beta} \tag{3}
$$

$N_{\alpha ,\beta}\in \mathbf{R}^*$ と

$$
N_{-\alpha ,-\beta}= N_{\alpha ,\beta} \tag{4}
$$

すべての $\alpha \in R$ に対して $\alpha (H)\in \mathbf{R}$ となるように、$H\in \mathfrak{h}$ の $\mathfrak{h}$ からなるの実数ベクトル部分空間を $\mathfrak{h}_0$ で表します。このとき、$\mathfrak{h}_0$は複合体ベクトル空間$\mathfrak{h}$上の$\mathbf{R}$構造であり、すべての$\alpha \in R$に対して$[X_{\alpha}, X_{-\alpha}]\in \mathfrak{h}_0$があり、$\mathfrak{a}$から$\mathfrak{h}_0$のKilling形Bの制限が正を分離しています（第2章）。 VIII, §2, no. 2、注意 2)。さらに、

$B(H, X_{\alpha}) = 0,B(X_{\alpha}, X_{\beta}) = 0$ $\alpha +\beta \not= 0,B(X_{\alpha}, X_{-\alpha})<0$ の場合 (5)

(第 VIII, §2, no. 2、提案 1 および no. 4、補題 3)。

#### 命題 2 {#lie-ix-s3-prop-2 .statement tag=01JG}

$a)$ $\mathfrak{a}$ の実際のベクトル部分空間 $\mathfrak{a}_0=\mathfrak{h}_0+\sum_{\alpha\in R}\mathbf{R}X_{\alpha}$ は、

$\mathfrak{a}$ の実数形のうち、$\mathfrak{h}_0$ はカルタン部分代数です。 対 $(\mathfrak{a}_0,\mathfrak{h}_0)$ は分裂半単純本物のリー代数で、そのうち $(X_{\alpha})$ はシュバレー 系です。

b) $\sigma$ を $\mathfrak{a}_0$ に対する $\mathfrak{a}$ の共役とします。次に$\sigma \circ \theta =\theta \circ \sigma$。 $\sigma \circ \theta$の固定点の集合は、$\mathfrak{a}$のコンパクト実数形$\mathfrak{a}_u$であり、そのうち$i\mathfrak{h}_0$はカルタン部分代数です。

部分 a) は前の内容の直後に続きます。 b)を証明します。 $\sigma \circ \theta$と$\theta \circ \sigma$は、$\mathfrak{a}$から$\mathfrak{a}$までの2つの半線形写像、$\mathfrak{a}_0$の一致するなので、一致するです。ここで、$\sigma \circ \theta$ は no. 1 の条件 (2) を満たすため、$x\in \mathfrak{a}$ の実数形 $\mathfrak{a}_u$ からなるに対する$\mathfrak{a}$ の共役は、$\sigma \circ \theta (x) =x$ となります (提案 1)。全員に $\alpha \in R$ を入れます

$$
u_{\alpha}=X_{\alpha}+X_{-\alpha},v_{\alpha}=i(X_{\alpha}-X_{-\alpha}) \tag{6}
$$

次に、$\mathbf{R}$ ベクトル空間 $\mathfrak{a}_u$ は、$i\mathfrak{h}_0$、$u_{\alpha}$、$v_{\alpha}$ によって生成されます。より正確には、R の室選ぶを C とすると、

$$
\mathfrak{a}_u=i\mathfrak{h}_0\oplus \bigoplus_{\alpha\in R_+(C)}(\mathbf{R}u_{\alpha}+\mathbf{R}v_{\alpha}) \tag{7}
$$

$i\mathfrak{h}_0$が$\mathfrak{a}_u$のカルタン部分代数であることは明らかですが、$\mathfrak{a}_u$に対するBの制限が負であることを証明する必要があります。ここで、$i\mathfrak{h}_0$ と形 $\mathbf{R}u_{\alpha}\oplus \mathbf{R}v_{\alpha}$ の異なる部分空間は、(5) により B に関して直交します。 $i\mathfrak{h}_0$に対するBの制限はマイナスであり、

$$
B(u_{\alpha}, u_{\alpha}) = B(v_{\alpha}, v_{\alpha}) = 2B(X_{\alpha}, X_{-\alpha})<0,B(u_{\alpha}, v_{\alpha}) = 0 \tag{8}
$$

したがって結論です。

#### 注意 {#lie-ix-s3-n2-rem-1 .statement tag=01B2}

前の記法を使用すると、次の公式が得られます。

$$
[h, u_{\alpha}] =-i\alpha (h)v_{\alpha},[h, v_{\alpha}] =i\alpha (h)u_{\alpha},[u_{\alpha}, v_{\alpha}] = 2iH_{\alpha},(h\in \mathfrak{h}) \tag{9}
$$

$$
[u_{\alpha}, u_{\beta}] = N_{\alpha ,\beta}u_{\alpha+\beta}+ N_{\alpha ,-\beta}u_{\alpha-\beta},\alpha \not=\pm \beta \tag{10}
$$

$$
[v_{\alpha}, v_{\beta}] =-N_{\alpha ,\beta}u_{\alpha+\beta}+ N_{\alpha ,-\beta}u_{\alpha-\beta},\alpha \not=\pm \beta \tag{11}
$$

$$
[u_{\alpha}, v_{\beta}] = N_{\alpha ,\beta}v_{\alpha+\beta}-N_{\alpha ,-\beta}v_{\alpha-\beta},\alpha \not=\pm \beta \tag{12}
$$

(最後の 3 つの公式では、通常どおり、$\gamma +\delta$ が根ではない場合、$N_{\gamma ,\delta}= 0$ であることが理解されます)。

$\sum\mathbf{R}u_{\alpha}$ は、$\mathfrak{a}$ の実際の部分代数、つまり $\mathfrak{a}_0\cap \mathfrak{a}_u$ であることに注意してください。

Q(R) を R の根基重みの群とする (VI, §1, no. 9 章)。すべての $h\in \mathfrak{h}$ と $f(\gamma )X_{\alpha}=$ $\gamma (\alpha )X_{\alpha}$ に対して $f(\gamma )(h) =h$ となるように、任意の準同型 $\gamma : Q(R)\rightarrow \mathbf{C}^*$ には $\mathfrak{a}$ の基本自己同型 $f(\gamma )$ が関連付けられていることを思い出してください (第 VIII, §5, no. 2)。

#### 命題 3 {#lie-ix-s3-prop-3 .statement tag=01B3}

$\mathfrak{g}$ を、$\mathfrak{g}\cap \mathfrak{h}=i\mathfrak{h}_0$ となるような $\mathfrak{a}$ の圧縮実数形とします。 $\mathfrak{g}=f(\gamma )(\mathfrak{a}_u)$ となるような準同型 $\gamma : Q(R)\rightarrow \mathbf{R}^*_+$ が存在します。

$\tau$ を $\mathfrak{g}$ に対する $\mathfrak{a}$ の共役とします。 仮定 $\tau (x) =x$ で $x\in i\mathfrak{h}_0$ なので、$\tau (x) =-x$ で $x\in \mathfrak{h}_0$ になります。したがって、すべての $\alpha \in R$ とすべての $h\in \mathfrak{h}_0$ について、

$$
[h, \tau (X_{\alpha})] = [-\tau (h), \tau (X_{\alpha})] =-\tau ([h, X_{\alpha}]) =-\tau (\alpha (h)X_{\alpha})
$$

すべての $h\in \mathfrak{h}_0$ について $[h, \tau (X_{\alpha})] =-\alpha (h)\tau (X_{\alpha})$ となり、したがってすべての $h\in \mathfrak{h}$ についても同様です。したがって、$\tau (X_{\alpha}) =c_{\alpha}X_{-\alpha}$ となるような $c_{\alpha}\in \mathbf{C}^*$ が存在します。 $[X_{\alpha}, X_{-\alpha}]\in \mathfrak{h}_0$ なので、$[\tau (X_{\alpha}), \tau (X_{-\alpha})] =-[X_{\alpha}, X_{-\alpha}]$ があるので、$c_{\alpha}c_{-\alpha}$ = 1;同様に、$\alpha , \beta , \alpha +\beta$ が根の場合、公式 (3) と (4) は $c_{\alpha+\beta}=c_{\alpha}c_{\beta}$ を与えます。章著。 VI, §1, no. 6、コル。提案 19 の 2 では、すべての $\alpha \in R$ に対して $\delta (\alpha ) =c_{\alpha}$ となるような準同型 $\delta : Q(R)\rightarrow \mathbf{C}^*$ が存在します。

ここで、それぞれの $c_{\alpha}$ が厳密に正であることを示します。確かに、$c_{\alpha}B(X_{\alpha}, X_{-\alpha}) =$ $B(X_{\alpha}, \tau (X_{\alpha}))$、そして $B(X_{\alpha}, X_{-\alpha})$ は負であるため、$\mathfrak{a}$ の非ゼロのすべての元 $z$ に対して $B(z, \tau (z))<0$ であることを示せば十分です。しかし、$\mathfrak{a}$ のすべての元は、$x$ と $y$ を$\mathfrak{g}$ に含めて、$x+iy$ として書くことができます。

$$
B(x+iy, \tau (x+iy)) = B(x+iy, x-iy) = B(x, x) + B(y, y)
$$

したがって、B から $\mathfrak{g}$ に記載されている主張、制限は負であり、仮定で区切られています。

したがって、準同型 $\delta$ は $\mathbf{R}^*_+$ で値をとります。したがって、$\delta =\gamma^{-2}$ となるような準同型 $\gamma : Q(R)\rightarrow \mathbf{R}^*_+$ が存在します。すると、$f(\gamma )^{-1}(\mathfrak{g})$ は $\mathfrak{a}$ の実数形になります。 対応する活用は$\tau '=f(\gamma )^{-1}\circ \tau \circ f(\gamma )$です。 $\alpha \in R$ の皆様には、

$$
\tau '(X_{\alpha}) =f(\gamma )^{-1}(\tau (c^{-1/2}_{\alpha}X_{\alpha})) =f(\gamma )^{-1}(c^{1/2}_{\alpha}X_{-\alpha}) =X_{-\alpha}
$$

そして $\tau '(h) =\tau (h) =h$ は $h\in i\mathfrak{h}_0$ です。したがって、$\tau '$ は $\mathfrak{a}_u$ に対する活用であり、したがって $f(\gamma )^{-1}(\mathfrak{g}) =\mathfrak{a}_u$ となります。

### 3. コンパクトの共役形

#### 定理 1 {#lie-ix-s3-thm-1 .statement tag=01B4}

$\mathfrak{a}$を複素半単純リー代数とします。

a$)\mathfrak{a}$ はコンパクトな (それぞれ分割可能な) 実数形を持っています。

b) 群 Int($\mathfrak{a}$) は、$\mathfrak{a}$ のコンパクト (分割可能) 実数形の集合で推移的に動作します。

$\mathfrak{h}$を$\mathfrak{a}$のカルタン部分代数とします。次に、$(\mathfrak{a},\mathfrak{h})$ は分裂 (章 VIII, §2, no. 1、注意 2) であり、シュバレー 系 $(X_{\alpha})$ (章 VIII, §4, no. 4、提案 5 の修正) があります。 部分 a) は提案 2 から導き出されます。$\mathfrak{g}$ を $\mathfrak{a}$ のコンパクト実数形とします。 $v(\mathfrak{a}_u) =\mathfrak{g}$ となるような $v\in$ Int($\mathfrak{a}$) が存在することを示します。 $\mathfrak{t}$ を $\mathfrak{g}$ のカルタン部分代数とします。その場合、$\mathfrak{t}_{(\mathbf{C})}$ は $\mathfrak{a}$ のカルタン部分代数です。 Int($\mathfrak{a}$) は $\mathfrak{a}$ のカルタン部分代数の集合で推移的に動作するため (第 1 章 VII, §3, no. 2)、$\mathfrak{t}_{(\mathbf{C})}=\mathfrak{h}$ の場合に帰着します。 $\mathfrak{g}$ はコンパクト形なので、$h\in \mathfrak{t}$ の自己準同型と $h$ の固有値は純粋に虚数です (§1, no. 3、提案 1)、つまり根 $\alpha \in R$ 写像 $\mathfrak{t}$ ～ $i\mathbf{R}$;これは $\mathfrak{t}=i\mathfrak{h}_0$ を意味します。すると、提案 3 (no. 2) により、$v(\mathfrak{a}_u) =\mathfrak{g}$ となるような $v\in$ Int($\mathfrak{a}$) が存在するので、コンパクト形の場合には b) となります。最後に、$\mathfrak{m}_1$ と $\mathfrak{m}_2$ を、$\mathfrak{a}$ の 2 つの分割可能な実数形とします。枠組み$(\mathfrak{m}_1,\mathfrak{h}_1,B_1,(X_{\alpha}^1))$と$(\mathfrak{m}_2,\mathfrak{h}_2,B_2,(X_{\alpha}^2))$が存在します（VIII, §4, no. 1章）。これらの拡大するは、基底 $e_1$ と $\mathfrak{a}$ の $e_2$ に明らかです。 $\mathfrak{a}$の自己同型、写像 $e_1$から$e_2$ 写像 $\mathfrak{m}_1$から$\mathfrak{m}_2$。したがって、第 5 章の提案 5 を適用するだけで十分です。 VIII, §5, no. 3、$u(\mathfrak{m}_1) =\mathfrak{m}_2$ となるような Aut$_0(\mathfrak{a}) =$ Int($\mathfrak{a}$) の元 $u$ の存在を取得します。

#### 注意 {#lie-ix-s3-n3-rem-1 .statement tag=01B5}

複素半単純リー代数の実際の形の一般的な分類は、ずっと後になります。

#### 系 1 {#lie-ix-s3-thm-1-cor-1 .statement tag=01B6}

$\mathfrak{g}$ と $\mathfrak{g}'$ を 2 つのコンパクト実リー群代数とします。このとき、$\mathfrak{g}$ と $\mathfrak{g}'$ は、複素数リー代数 $\mathfrak{g}_{(\mathbf{C})}$ と $\mathfrak{g}'_{(\mathbf{C})}$ が同型である場合に限り、同型になります。

条件は明らかに必要です。逆に、$\mathfrak{g}_{(\mathbf{C})}$ と $\mathfrak{g}'_{(\mathbf{C})}$ が同型であると仮定します。 $\mathfrak{c}$ (それぞれ $\mathfrak{c}'$) を $\mathfrak{g}$ (それぞれ $\mathfrak{g}'$) の中心および $\mathfrak{s}$ (それぞれ $\mathfrak{s}'$) を $\mathfrak{g}$ (それぞれ $\mathfrak{g}'$) の派生代数とします。この場合、$\mathfrak{c}_{(\mathbf{C})}$ と $\mathfrak{c}'_{(\mathbf{C})}$ は、それぞれ $\mathfrak{g}_{(\mathbf{C})}$ と $\mathfrak{g}'_{(\mathbf{C})}$ の中心であるため、同型です。したがって、可換代数 $\mathfrak{c}$ と $\mathfrak{c}'$ は同型であることがわかります。同様に、$\mathfrak{s}_{(\mathbf{C})}$ と $\mathfrak{s}'_{(\mathbf{C})}$ は同型であるため、2 つの同型複素半単純リー代数のコンパクト実数形である $\mathfrak{s}$ と $\mathfrak{s}'$ は Th による同型です。 $1b)$。

#### 系 2 {#lie-ix-s3-thm-1-cor-2 .statement tag=01B7}

$\mathfrak{a}$ を複素数リー代数とします。次の条件は同等です。

(i) $\mathfrak{a}$ は還元的です。

(ii) $\mathfrak{a}$ が $\mathfrak{g}_{(\mathbf{C})}$ と同型となるようなコンパクト実リー群代数 $\mathfrak{g}$ が存在します。

(iii) $\mathfrak{a}$ が $L(G)_{(\mathbf{C})}$ と同型となるようなコンパクト・リー群 G が存在します。

デフによる。 §1, no. 3、条件 (ii) および (iii) の 1 は同等であり、(i) を意味します。 $\mathfrak{a}$ が還元的である場合、それは可換代数の直接の積であり、明らかにコンパクトな実数形と Th による 1 を持つ半単純代数があります。 $1a)$ したがって、(i) は (ii) を意味します。

#### 系 3 {#lie-ix-s3-thm-1-cor-3 .statement tag=01B8}

$\mathfrak{a}_1$ と $\mathfrak{a}_2$ を 2 つの複素半単純リー代数とします。 $\mathfrak{a}_1\times \mathfrak{a}_2$ のコンパクト実数形は積 $\mathfrak{g}_1\times \mathfrak{g}_2$ です。ここで、$i= 1,2,\mathfrak{g}_i$ は $\mathfrak{a}_i$ のコンパクト実数形です。

実際、$\mathfrak{a}_1$ (それぞれ $\mathfrak{a}_2$) のコンパクトな実数形 $\mathfrak{g}_1$ (それぞれ $\mathfrak{g}_2$) が存在します。この場合、$\mathfrak{g}_1\times \mathfrak{g}_2$ は $\mathfrak{a}_1\times \mathfrak{a}_2$ の圧縮実数形です。 系は Th から続きます。 $1b)$、$\mathfrak{a}_1,\mathfrak{a}_2$と$\mathfrak{a}_1\times \mathfrak{a}_2$に適用されます。

これは Cor から続くことに注意してください。その上の 3 コンパクト実リー群代数 $\mathfrak{g}$ は、複素数リー代数 $\mathfrak{g}_{(\mathbf{C})}$ が単純である場合に限り、単純です。 $\mathfrak{g}_{(\mathbf{C})}$ が型 $A_n$ または $B_n,. .$ である場合、$\mathfrak{g}$ は型 $A_n$ または $B_n,. .$ であると言います。 (VIII, §2, no. 2章)。コル著上の 1 では、2 つのコンパクトな単純実数リー代数は、同じ型である場合にのみ同型です。

G をほぼ単純に接続されたコンパクト・リー群とします (章 III, §9, no. 8、定義 3)。 G がリー代数型 $A_n$ または $B_n,. .$ である場合、G は型 $A_n$ または $B_n,. .$ であると言います。 2 つの単純に接続されたほぼ単純なコンパクト・リー群は、それらが同じ型である場合にのみ同型です。

### 4. 例 I: 型 A$_{\boldsymbol{n}}$ のコンパクト代数

V を有限次元複素数ベクトル空間とし、$\Phi$ を V 上の分離正のエルミート形とします。 The unitary group associated to $\Phi$ (cf. Algebra, Chap. IX) is the subgroup $\mathbf{U}(\Phi )$ of $\mathbf{G}\mathbf{L}(V)$ consisting of the automorphisms of the complex Hilbert space $(V, \Phi )$; this is a (real) Lie subgroup of the group $\mathbf{G}\mathbf{L}$(V), whose Lie algebra is the subalgebra $\mathfrak{u}(\Phi )$ of the real Lie algebra $\mathfrak{g}\mathfrak{l}(V)$ consisting of the endomorphisms $x$ of V such that $x^*=-x$ (Chap. III, §3, no. 10, Cor. 2 of Prop. 37), where $x^*$ denotes the adjoint of $x$ relative to $\Phi$. 群 $\mathbf{U}(\Phi )$ はコンパクトなので (§1、いいえ $1$) $,\mathfrak{u}(\Phi )$ はコンパクト実リー群代数です。 同様に、特殊ユニタリー 群 $\mathbf{S}\mathbf{U}(\Phi ) =\mathbf{U}(\Phi )\cap \mathbf{S}\mathbf{L}(V)$ は $\mathbf{S}\mathbf{L}$(V) のコンパクトリー 部分群であり、そのリー代数は $\mathfrak{s}\mathfrak{u}(\Phi ) =\mathfrak{u}(\Phi )\cap \mathfrak{s}\mathfrak{l}(V)$ です。

$V =\mathbf{C}^n$ と $\Phi$ が通常のエルミート形 ($\mathbf{C}^n$ の標準基底が正規直交) の場合、$\mathbf{U}(\Phi ),\mathbf{S}\mathbf{U}(\Phi ),\mathfrak{u}(\Phi ),\mathfrak{s}\mathfrak{u}(\Phi )$ の代わりに $\mathbf{U}(n,\mathbf{C}),\mathbf{S}\mathbf{U}(n,\mathbf{C}),\mathfrak{u}(n,\mathbf{C}),\mathfrak{s}\mathfrak{u}(n,\mathbf{C})$ と書きます。 $\mathbf{U}(n,\mathbf{C})$ (それぞれ $\mathfrak{u}(n,\mathbf{C})$) の元は行列 $A\in M_n(\mathbf{C})$ であり、$A.^t\overline{A}=I_n$ (それぞれ $A=-^t\overline{A}$) は単一である (それぞれ反エルミート) と言われます。

#### 命題 4 {#lie-ix-s3-prop-4 .statement tag=01B9}

a) 複素数リー代数 $\mathfrak{s}\mathfrak{l}(V)$ のコンパクト実数形は代数 $\mathfrak{s}\mathfrak{u}(\Phi )$ で、複素数ベクトル空間上の分離正エルミート形の $\Phi$ 属するから集合です。 V。

b) 代数 $\mathfrak{u}(\Phi )$ は、$\mathfrak{g}\mathfrak{l}(V)$ の圧縮実数形です。

$\Phi$ を V の分離ポジティブエルミート形とします。 すべての $x\in \mathfrak{g}\mathfrak{l}$(V) に対して、 $\sigma (x) =-x^*$ を入力します (ここで、 $x^*$ は $\Phi$ に対する $x$ の随伴です)。 すると、$\sigma$ はno. 1 の提案 1 の条件 (2) を満たすので、$\mathfrak{g}\mathfrak{l}(V)$ (それぞれ$\mathfrak{s}\mathfrak{l}(V)$) 上の$\sigma$ の固定点の集合 $\mathfrak{u}(\Phi )$ (それぞれ$\mathfrak{s}\mathfrak{u}(\Phi )$) はコンパクト実数になります。 $\mathfrak{g}\mathfrak{l}(V)$ の形 (それぞれ $\mathfrak{s}\mathfrak{l}(V)$)。 $\mathbf{G}\mathbf{L}(V)$ は、V (代数、IX 章) の分離正エルミート形式の集合と、$\mathfrak{s}\mathfrak{l}(V)$ (no. 3、Th. 1 および章 VIII, §13, no. 1 (VII)) のコンパクトな実形式の集合に対して推移的に動作するため、提案 4 が証明されます。

#### 系 {#lie-ix-s3-n4-cor-1 .statement tag=01BA}

型 $A_n(n\geq 1)$ のすべてのコンパクト単純実数リー代数は $\mathfrak{s}\mathfrak{u}(n+ 1,\mathbf{C})$ と同型です。

Indeed, every complex Lie algebra of type $A_n$ is isomorphic to $\mathfrak{s}\mathfrak{l}(n+ 1,\mathbf{C})$ (Chap. VIII, §13, no. 1).

#### 注意 1 {#lie-ix-s3-n4-rem-1 .statement tag=01BB}

$\mathfrak{g}\mathfrak{l}(V) =\mathfrak{s}\mathfrak{l}(V)\times \mathbf{C}.1_V,\mathfrak{u}(\Phi ) =\mathfrak{s}\mathfrak{u}(\Phi )\times \mathbf{R}.i1_V$ があります。 $\mathfrak{g}\mathfrak{l}(V)$ のコンパクトな実形は $\mathfrak{s}\mathfrak{u}(\Phi )\times \mathbf{R}.\alpha 1_V,\alpha \in \mathbf{C}^*$ です。

#### 注意 2 {#lie-ix-s3-n4-rem-2 .statement tag=01BC}

複合施設リー代数 $\mathfrak{a}=\mathfrak{s}\mathfrak{l}(n,\mathbf{C})$ に、第 4 章で紹介した分裂と Chevalley 系が装備されている場合、 VIII, §13, no. 1 (IX)、その後、no. 2 に記法が入って、

$$
\mathfrak{a}_u=\mathfrak{s}\mathfrak{u}(n,\mathbf{C}),\mathfrak{a}_0=\mathfrak{s}\mathfrak{l}(n,\mathbf{R}),\mathfrak{a}_u\cap \mathfrak{a}_0=\mathfrak{o}(n,\mathbf{R})
$$

### 5. 例 II: コンパクト代数 OF 型 B$_{\boldsymbol{n}}\mathbf{A}\mathbf{N}\mathbf{D}$ $\mathbf{D}_{\boldsymbol{n}}$

V を有限次元の実数ベクトル空間とし、Q を V 上の正の二次方程式形を分離するものとします。 The orthogonal group associated to Q (Algebra, Chap. IX) is the subgroup $\mathbf{O}(Q)$ of $\mathbf{G}\mathbf{L}(V)$ consisting of the automorphisms of the real Hilbert space $(V,Q)$; this is a Lie subgroup of $\mathbf{G}\mathbf{L}$(V), whose Lie algebra is the subalgebra $\mathfrak{o}(Q)$ of $\mathfrak{g}\mathfrak{l}(V)$ consisting of the endomorphisms $x$ of V such that $x^*=-x$ (Chap. III, §3, no. 10, Cor. 2 of Prop. $37$)$,x^*$ denoting the adjoint of $x$ relative to Q. 群 $\mathbf{O}(Q)$ はコンパクトなので、$\mathfrak{o}(Q)$ はコンパクト実リー群代数になります。 Put $\mathbf{S}\mathbf{O}(Q) =\mathbf{O}(Q)\cap \mathbf{S}\mathbf{L}(V)$; this is a closed subgroup of finite index of $\mathbf{O}(Q)$ (of index 2 if dim $V\not= 0$), hence also with Lie algebra $\mathfrak{o}(Q)$.

$V =\mathbf{R}^n$ と Q が通常の 2 次式形 ($\mathbf{R}^n$ の標準基底が正規直交である) の場合、$\mathbf{O}(Q),\mathbf{S}\mathbf{O}(Q),\mathfrak{o}(Q)$ の代わりに $\mathbf{O}(n,\mathbf{R}),\mathbf{S}\mathbf{O}(n,\mathbf{R}),\mathfrak{o}(n,\mathbf{R})$ と書きます。 $\mathbf{O}(n,\mathbf{R})$ (それぞれ $\mathfrak{o}(n,\mathbf{R})$) の元は行列 $A\in M_n(\mathbf{R})$ であり、$A.^tA=I_n$ (それぞれ $A=-^tA$) は直交している (それぞれ反対称) と言われます。

$V_{(\mathbf{C})}$ を V に関連付けられた複素数ベクトル空間とし、$Q_{(\mathbf{C})}$ を Q に関連付けられた $V_{(\mathbf{C})}$ の 2 次式形とします。 同一視する $\mathfrak{g}\mathfrak{l}(V)_{(\mathbf{C})}$ と $\mathfrak{g}\mathfrak{l}(V_{(\mathbf{C})})$;次に、$\mathfrak{o}(Q)_{(\mathbf{C})}$ は $\mathfrak{o}(Q_{(\mathbf{C})}):$ と同一視されます。これは、$\mathfrak{g}\mathfrak{l}(V_{(\mathbf{C})})$ からそれ自体までの写像 $x \rightarrow x^*+x$ が $\mathbf{C}$ 線形であるため、明らかです。 $\mathfrak{o}(Q_{(\mathbf{C})})$ は、薄暗い場合は型 $B_n$、$V = 2n+ 1$、$n\geq 1$ であり、$V = 2n,n\geq 3$ が薄暗い場合は型 $D_n$ であるため（VIII, §13、番号 2 と 4）、次のように推測します。

#### 命題 5 {#lie-ix-s3-prop-5 .statement tag=01BD}

型 $B_n,n\geq 1$ (それぞれ型 $D_n,n\geq 3$) のすべてのコンパクト単純実数リー代数は、$\mathfrak{o}(2n+ 1,\mathbf{R})$ (それぞれ $\mathfrak{o}(2n,\mathbf{R})$) と同型です。

### 6. コンパクト群/階数 1

位相章、将軍よりVIII, §1, no. 4、提案 3、提案 4、および注意 4、トポロジカル群 $\mathbf{S}\mathbf{U}(2,\mathbf{C})$ は、ノルム 1 の四元数のトポロジカル群 $\mathbf{S}_3$ および $\mathbf{S}\mathbf{U}(2,\mathbf{C})$ の商と同型です。 行列 $I_2$ と $-I_2$ の部分群 Z からなるはトポロジー 群 $\mathbf{S}\mathbf{O}(3,\mathbf{R})$ と同型です。 Z は $\mathbf{S}\mathbf{U}(2,\mathbf{C}):$ の中心であることに注意してください。$\mathbf{H}=\mathbf{R}.\mathbf{S}_3$ 以降、群 $\mathbf{S}_3$ の中心のすべての元は代数 $\mathbf{H}$ の中心 $\mathbf{R}$ に含まれるため、 属するから群に元 $\mathbf{S}_3\cap \mathbf{R}=\{-1,1\}$ が 2 つあります。

#### 命題 6 {#lie-ix-s3-prop-6 .statement tag=01BE}

階数 1 のすべてのコンパクト半単純実数リー代数は、$\mathfrak{s}\mathfrak{u}(2,\mathbf{C})$ および $\mathfrak{o}(3,\mathbf{R})$ と同型です。 階数 1 の接続されたすべての半単純コンパクト・リー群は、単純接続されている場合は $\mathbf{S}\mathbf{U}(2,\mathbf{C})$ と同型であり、そうでない場合は $\mathbf{S}\mathbf{O}(3,\mathbf{R})$ と同型です。

最初の主張は Cor から続きます。提案4と提案5の。 Since $\mathbf{S}\mathbf{U}(2,\mathbf{C})$ is homeomorphic to $\mathbf{S}_3($General Topology, Chap. VIII, §1, no. 4, Remark 4), hence is simply-connected (General Topology, Chap. XI, in preparation), every simply-connected compact semi-simple Lie group of rank 1 is isomorphic to $\mathbf{S}\mathbf{U}(2,\mathbf{C})$; every connected compact semi-simple Lie group of rank 1 that is not simply-connected is isomorphic to a quotient of $\mathbf{S}\mathbf{U}(2,\mathbf{C})$ by a subgroup of Z that does not reduce to the identity element, hence to $\mathbf{S}\mathbf{O}(3,\mathbf{R})$.

#### 注意 {#lie-ix-s3-n6-rem-1 .statement tag=01BF}

上記では、$\mathbf{S}\mathbf{U}(2,\mathbf{C})$ が単純結合であり、$\pi_1(\mathbf{S}\mathbf{O}(3,\mathbf{R}))$ が位数 2 であることを見てきました。これらの結果がそれぞれ $\mathbf{S}\mathbf{U}(n,\mathbf{C}) (n\geq 1)$ と $\mathbf{S}\mathbf{O}(n,\mathbf{R}) (n\geq 3)$ に一般化されることがわかります (cf. も §3、演習 4 と 5)。

Recall (Chap. VIII, §1, no. 1) that the canonical basis of $\mathfrak{s}\mathfrak{l}(2,\mathbf{C})$ is the basis $(X_+, X_-, H)$, where

$(01)(00)(1$ 0 $)$

$X_+=$ 0 0 $, X_-=-1$ 0 $, H=$ 0 $-1$。

したがって、次のようにして、正規とも呼ばれる $\mathfrak{su}(2,\mathbf C)$ の基底 $(U,V,iH)$ を取得します。
$$
U=X_++X_-=
\begin{pmatrix}
0&1\\
-1&0
\end{pmatrix},
\qquad
V=i(X_+-X_-)=
\begin{pmatrix}
0&i\\
i&0
\end{pmatrix},
$$
$$
iH=
\begin{pmatrix}
i&0\\
0&-i
\end{pmatrix}.
$$

私たちは持っています
$$
[iH,U]=2V,\qquad [iH,V]=-2U,\qquad [U,V]=2iH.
\tag{13}
$$

B が $\mathfrak{su}(2,\mathbf C)$ 明らかの Killing 形を表す場合、計算は次のようになります。
$$
\mathrm{B}(aU+bV+ciH,a'U+b'V+c'iH)=-8(aa'+bb'+cc'),
\tag{14}
$$
つまり、標準基底を使って同一視する $\mathfrak{su}(2,\mathbf C)$ と $\mathbf R^3$ を結合すると、$\mathbf{SU}(2,\mathbf C)$ 定義する準同型 $\mathbf{SU}(2,\mathbf C)\to\mathbf{SO}(3,\mathbf R)$ の随伴表現 (上記のcf.) になります。

さらに、$\mathbf RiH$ は $\mathfrak{su}(2,\mathbf C)$ のカルタン部分代数であり、$\mathbf{SU}(2,\mathbf C)$ の最大トーラス T は、対応するが対角行列で構成されていることに注意してください。
$$
\begin{pmatrix}
a&0\\
0&\bar a
\end{pmatrix},
$$
ここで $a\bar a=1$ と指数関数写像
$$
\exp:\mathbf RiH\longrightarrow T
$$
写像 $xH$、$x\in\mathbf Ri$の場合、行列まで
$$
\begin{pmatrix}
\exp(x)&0\\
0&\exp(-x)
\end{pmatrix},
$$
したがって、核 $\mathbf Z.K$ になります。ここで、K は、次のように定義される $\mathfrak{su}(2,\mathbf C)$ の元です。
$$
K=2\pi iH=
\begin{pmatrix}
2\pi i&0\\
0&-2\pi i
\end{pmatrix}.
\tag{15}
$$

さらに、$\mathbf{SU}(2,\mathbf C)$の中心は正体と$\exp(K/2)$から構成されます。

置く
$$
\theta=
\begin{pmatrix}
0&-1\\
1&0
\end{pmatrix}
\in\mathbf{SU}(2,\mathbf C).
\tag{16}
$$

章著。 VIII, §1, no. 5、
$$
\theta^2=
\begin{pmatrix}
-1&0\\
0&-1
\end{pmatrix},
\qquad
(\mathrm{Int}\,\theta)t=t^{-1},\quad t\in T,
\tag{17}
$$
$$
(\mathrm{Ad}\,\theta)X_+=X_-,
\qquad
(\mathrm{Ad}\,\theta)X_-=X_+,
\qquad
(\mathrm{Ad}\,\theta)U=U,
\qquad
(\mathrm{Ad}\,\theta)V=-V.
\tag{18}
$$

最後に、$t=
\begin{pmatrix}
a&0\\
0&\bar a
\end{pmatrix}
\in T$ については、
$$
(\mathrm{Ad}\,t)X_+=a^2X_+,
\qquad
(\mathrm{Ad}\,t)X_-=a^{-2}X_-,
\qquad
(\mathrm{Ad}\,t)H=H,
\tag{19}
$$
$$
(\mathrm{Ad}\,t)U=\mathscr{R}(a^2)U+\mathscr{I}(a^2)V,
\qquad
(\mathrm{Ad}\,t)V=-\mathscr{I}(a^2)U+\mathscr{R}(a^2)V.
\tag{20}
$$

### 練習問題 {#lie-ix-s3-exercises}

[§ 3 に対して練習問題](exercises/s3/)を参照してください。
