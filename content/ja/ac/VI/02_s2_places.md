---
book: ac
book_title: Commutative Algebra
chapter: VI
chapter_title: VALUATIONS
section: 2
section_title: Places
lang: ja
source: ac-i-vii
book_pages: 381-385, 444-446
pdf_pages: 0399-0403, 0462-0464
extraction: ocr
subsections:
    - "no": 1
      title: THE NOTION OF MORPHISM FOR LAWS OF COMPOSITION NOT EVERYWHERE DEFINED
      page: 381
      pdf_page: 399
    - "no": 2
      title: PLACES
      page: 381
      pdf_page: 399
    - "no": 3
      title: PLACES AND VALUATION RINGS
      page: 383
      pdf_page: 401
    - "no": 4
      title: EXTENSION OF PLACES
      page: 384
      pdf_page: 402
    - "no": 5
      title: CHARACTERIZATION OF INTEGRAL ELEMENTS BY MEANS OF PLACES
      page: 385
      pdf_page: 403
statements: 9
exercises: 6
content_sha256: 1ffa65cfa9030f722f082c8ecce50165ee26ce6724afeeb9b5cab1a88e0116d3
translated_from: content/en/ac/VI/02_s2_places.md
translation_method: google
source_content_sha256: 53c302660c61cd7fef1b70be1d4b1ffa083e7229208dbbe2c386c3d702cdbacb
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-eeeca2ef
glossary_version: 34
glossary_terms_sha256: a4df95bce0e7790aaa51448b1f158ae7c3601d6d659b32d3e5b4c9c96013ca49
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## 2. 場所

### 1. 合成の法則に対して射の概念がどこでも定義されているわけではありません

#### 定義 1 {#ac-vi-s2-def-1 .statement tag=04SN}

*E と E' を 2 つの集合とし、それぞれ合成の内部法則を $(x, y) \mapsto x * y$ で示しますが、どこでも定義されている必要はありません。 $f(x) * f(y)$ が定義されるような E のすべての $x, y$ に対して、合成 $x * y$ も定義され、かつ次の場合、写像 $f : E \to E'$ は射になります。

(1)
$$
f(x * y) = f(x) * f(y).
$$
より簡単に言うと、右辺が意味を持つときは必ず公式 (1) が成り立つはずです。

射の概念は、表現 (*代数*, 章 I, § 1, no. 1) のそれとは異なり、左辺が意味を持つ場合は常に式 (1) が成り立つことが要求されます。もちろん、合成の法則に対する 2 つの概念一致するはどこでも定義されています。

#### 定義 2 {#ac-vi-s2-def-2 .statement tag=04SO}

*E と E' を 2 つの集合とし、それぞれ合成 $(x, y) \mapsto x *_{\alpha} y, \alpha \in I$ の内部法則のファミリーを持ちます。 合成 $(x, y) \mapsto x *_{\alpha} y$ のそれぞれ法則が射であれば、写像 $f : E \to E'$ は射になります。*

表現と同様に、射満たす *集合理論*、章 IV, § 2 の公理 (MO_I)、(MO_{II})、(MO_{III}) も同様です。 $E \to E'$ が射の場合、$f(E)$ は $\mathbf{R}'$ の安定した部分集合です。

### 2. 場所

K が体の場合、$\mathbf{K}$ は K の集合和を表し、元は $\infty$ (*代数*、章 11、§ 9, no. 9) で表されることを思い出してください。 設定による K 拡大するの合成から $\mathbf{K}$ までの法則 (*loc. cit.*)

(2)
$$
a + \infty = \infty \quad \text{for } a \in \mathbf{K}, \quad a \neq \infty,
$$
(3)
$$
\infty . a = a . \infty = \infty \quad \text{for } a \in \tilde{\mathbf{K}}, \quad a \neq 0.
$$

したがって、定義されていない唯一の合成は、合成 ～ $+ \infty$、$\infty . 0$、および $0 . \infty$ です。一方、写像 $x \mapsto -x$ と $x \mapsto x^{-1}$ 拡大するは、設定 $-\infty = \infty, 0^{-1} = \infty, \infty^{-1} = 0$ による$\tilde{K}$ と同様です。 $x + (-y) = x - y$ とも書きます。

集合 $\tilde{K}$ は、$K$ に関連付けられた *射影体* と呼ばれ、*射影線* $P_1(K)$ (*loc. cit.*) で識別できます。

#### 定義 3 {#ac-vi-s2-def-3 .statement tag=04SP}

※$K$と$L$を2つの体とします。 射* $f$ *の* $K$ *から* $\tilde{L}$ *(加法と乗法の場合)* *$f(1) = 1$ *は*の場所と呼ばれます* $K$ *値を*に$L$。

他の語では、$x$と$y$が$K$の元で、$f(x) + f(y)$（それぞれ$f(x)f(y)$）が定義されている場合、$x + y$（それぞれ$xy$）が定義され、

$$
f(x + y) = f(x) + f(y)
$$
$$
f(xy) = f(x)f(y).
$$

$\infty + \infty$ が定義されていないため、$f(\infty) + f(\infty)$ も定義されていないことがわかります。
$$
f(\infty) = \infty.
$$

同様に、$0 \cdot \infty$ が定義されていないため、$f(0)f(\infty)$ も定義されていません。これは、(6) のおかげで、次のことを意味します。
$$
f(0) = 0.
$$

一方、
$$
f(a^{-1}) = f(a)^{-1} \quad \text{for all } a \in \tilde{K}.
$$

$f(a)f(a^{-1})$ が定義されている場合、$aa^{-1}$ は定義されているため、1 に等しくなります。次に $f(a)f(a^{-1}) = f(1) = 1$ となり、この場合は (8) が証明されます。 $f(a)f(a)^{-1}$ が定義されていない場合は、$f(a) = 0$ と $f(a^{-1}) = \infty$ または $f(a) = \infty$ と $f(a^{-1}) = 0$ のいずれかが成立し、(8) が引き続き成立します。

同様に、次のように示すことができます。
$$
f(-a) = -f(a) \quad \text{for all } a \in K.
$$

式 (8) と (9) から、合成 $(x, y) \mapsto x - y$ と $(x, y) \mapsto xy^{-1}$ の法則についても、$f$ は射であることがわかります。

$x \in \tilde{K}$ の場合、$f(x) \neq \infty$ の場合、$f$ は $x$ で有限と呼ばれます。これは (6) によって $x \in K$ を意味します。

If $f : K \to \tilde{L}$ is a place, $f(K)$ is a subset of $\tilde{L}$ which is stable for the laws of composition $(x, y) \mapsto x + y, (x, y) \mapsto x - y, (x, y) \mapsto xy$ and $(x, y) \mapsto xy^{-1}$ and which contains 1. E が $f(\tilde{K})$ の有限元の集合である場合、E は L と $f(\tilde{K}) = \tilde{E}$ の部分体です。 言語の乱用により、E は *valuefield* オフと呼ばれます。

2 つの場所の *合成* 写像が 1 つの場所です。

F を体の同型 K から体 L の部分体とする。 拡大する $f$ から $K$ までに設定 $f(\infty) = \infty$ までにさせてください。したがって、L の値で K の位が得られます。これは *trivial* と呼ばれ、しばしば同型 $f$ と識別されます。

### 3. 場所と評価環

#### 命題 1 {#ac-vi-s2-prop-1 .statement tag=04SQ}

K を体、K の評価環および $\mathbf{A}$ の $\kappa(\mathbf{A})$ 剰余体を $\mathbf{A}$ とします。 $x \notin \mathbf{A}$の場合、方程式$h_{\mathbf{A}}(x) = \infty$により、$\mathbf{A}$の拡大する標準写像を$\kappa(\mathbf{A})$から写像$h_{\mathbf{A}} : \tilde{K} \to (\kappa(\mathbf{A}))$に掛けます。このように定義された写像 $h_{\mathbf{A}}$ は、値フィールドが $\kappa(\mathbf{A})$ である K の場所です。

明らかに$h_{\mathbf{A}}(1) = 1$。

$h_{\mathbf{A}}$ は加法に対して射であることがわかります。 $x, y$ を $\tilde{K}$ の 2 つの元として、$h_{\mathbf{A}}(x) + h_{\mathbf{A}}(y)$ が定義されるようにします。 2 つの元 $x, y$ 属するの 1 つから $\mathbf{A}$ が定義され、したがって $x + y$ が定義されます。 $x \in \mathbf{A}$ と $y \in \mathbf{A}$ の場合、明らかに

$$
h_{\mathbf{A}}(x) + h_{\mathbf{A}}(y) = h_{\mathbf{A}}(x + y)
$$

が成立する。 $x \in \mathbf{A}$ と $y \notin \mathbf{A}$ の場合、$x + y \notin \mathbf{A}$ と上記の 2 つの辺公式は $\infty$ に等しくなります。

最後に、$h_{\mathbf{A}}$ が乗法に対して射であることを示します。 $x \in K, y \in K$ を $h_{\mathbf{A}}(x)h_{\mathbf{A}}(y)$ が定義されるようなものとします。 $x \in \mathbf{A}$ と $y \in \mathbf{A}$ の場合、明らかに $xy$ が定義され、$h_{\mathbf{A}}(x)h_{\mathbf{A}}(y) = h_{\mathbf{A}}(xy)$ となります。ここで、元 $x, y$ の 1 つ、たとえば $y$ が属するから $\mathbf{A}$ にならないとします。 $h_{\mathbf{A}}(y) = \infty$、$h_{\mathbf{A}}(x) \neq 0$、つまり $x \notin m(\mathbf{A})$、よって $x^{-1} \in \mathbf{A}$;したがって、$xy$ が定義され、$xy \notin \mathbf{A}$、よってが定義されます。

$$
h_{\mathbf{A}}(xy) = \infty = h_{\mathbf{A}}(x)h_{\mathbf{A}}(y).
$$

これは命題 1 を証明します。

$j$ が体 L の部分体上の $\kappa(\mathbf{A})$ の同型である場合、$j \circ h_{\mathbf{A}} : \tilde{K} \to \tilde{L}$ は、L の値と K の場所になります。実際、上記のプロセスにより、K 上のすべての場所が提供されます。正確に言うと、次のようになります。

#### 命題 2 {#ac-vi-s2-prop-2 .statement tag=04SR}

K と L を 2 つの体とし、f を L の値と合わせた K の場所とします。次に、Lの部分体に対して、Kの評価環$\mathbf{A}$と$\kappa(\mathbf{A})$の同型$j$が存在し、$f = j \circ h_{\mathbf{A}}$になります。これら条件決定する $\mathbf{A}$ と $j$ は一意です。 環 $\mathbf{A}$ は $f(x) \neq \infty$ のように $x \in K$ の集合であり、$m(\mathbf{A})$ は $f(x) = 0$ のように $x \in K$ の集合です。

$f = j \circ h_{\mathbf{A}}$ の場合、条件 $f(x) \neq \infty$ (それぞれ $f(x) = 0$) は条件 $h_{\mathbf{A}}(x) \neq \infty$ (それぞれ $h_{\mathbf{A}}(x) = 0$) と同等であり、したがって条件 $x \in \mathbf{A}$ (それぞれ $x \in m(\mathbf{A})$) と同等です。したがって、$\mathbf{A}$ は一意に決定され、$h_{\mathbf{A}}$ が全射であるように、$j$ も一意です。

ここで、$f$ を、L の値を含む K の任意の位とします。 $\mathbf{A}$ は $x \in K$ の集合を表し、$f(x) \neq \infty$ となるようにします。 $x \in \mathbf{A}$ と $y \in \mathbf{A}$ の場合、合成 $f(x) - f(y)$ と $f(x)f(y)$ が定義され、$\neq \infty$ は $x - y \in \mathbf{A}$ と $xy \in \mathbf{A}$ を示します。したがって、$\mathbf{A}$はKの部分環です。$x \notin \mathbf{A}$の場合、$f(x) = \infty$、したがって、$f(x^{-1}) = 0$と$x^{-1}$属するから準同型$f'$の$m$が核になります。 $f$ を $\mathbf{A}$ に制限します。逆に$y \in m$なら$y^{-1} \notin \mathbf{A}$です。これは、$\mathbf{A}$ が K の評価環であり、$m$ がその最大の理想であることを示しています。 f'から移行から商まで導いた$\kappa(\mathbf{A})$からLまでの$j$を単射準同型とします。すると、すべての $x \in A$ に対して $f(x) = j(h_A(x))$ となり、この方程式は $x \notin A$ にも当てはまり、両辺は $\infty$ に等しくなります。

分解 $f = j \circ h_A$ は、placef の標準分解と呼ばれます。 $A$は環オフ、$m(A)$は$f$、$\kappa(A)$は剰余体オフと呼ばれます。 2 つの場所 $f : \mathbf{K} \to \mathbf{L}$ と $f' : \mathbf{K} \to \mathbf{L}'$ が同じ環を持つには、$f' = s \circ f$ となるようなオフ上に値体の同型が存在することが必要かつ十分です。その場合、$f$ と $f'$ は同等と呼ばれます。評価環に関するすべての結果は、場所に関する結果に変換でき、またその逆も可能であることがわかります。これが次の番号で行うことです。

例場所の
(1) $K$ を体とします。 $K$の恒等写像は環$K$と理想的な$(0)$がある些細な場所です。
(2) $k$を体とします。 すべての $u \in k((T))^\sim$ について、$u \notin k[[T]]$ の場合は $f(u) = \infty$、$u \in k[[T]]$ の場合は $u$ の定数項となるように定義する $f(u)$ を書きましょう。 すると、$f$ は $k((T))$ の場所で、剰余体 $k$ と環 $k[[T]]$ になります。 For $k[[T]]$ is a valuation ring of $k((T))$ (§ 1, no. 4, Example 3 ) and the restriction of $f$ to $k[[T]]$ is identified with the canonical homomorphism of $k[[T]]$ onto its residue field.
(3) Let $k$ be a field, $a$ an element of $k$ and $A$ the set of $u \in k(X)$ such that $a$ is substitutable in $u$ (Algebra, Chapter IV, § 3, no. 2). $p$ が $k[X]$ の主イデアル $(X - a)$ を表す場合、$A = k[X]_p$ となるため、$A$ は $k(X)$ (§ 1, no. 4、命題 2) の評価環になります。 すべての$u \in k(X)^\sim$について、$u \notin A$の場合は$f(u) = \infty$、$u \in A$の場合は$f(u) = u(a)$と書きましょう。 すると、$f$ は剰余体 $k$ と環 $A$ を含む $k(X)$ の場所になります。 制限から $A$ までは、$A$ の準同型から核 $pA = m(A)$ の $k$ (代数、章 IV, § 3、命題 2) です。 元 $f(u) \in k$は、$u$に$X = a$を入れると得られると言われています。
\* (4) $S$ を、$S$ 上の有理型写像の次元 1 と $K$ 体の接続された複素解析多様体とします。 $K$ から $\mathbf{C}$ までのすべての $z_0 \in S$、写像 $f \mapsto f(z_0)$ は、環が集合オフ $\in K$ で、$z_0$ で正則であり、理想が集合オフである $K$ の場所です。 $z_0$の零である$\in K$。 この例とその他の類似物が項 「場所」の起源です。*

### 4. 拡大か所

#### 命題 3 {#ac-vi-s2-prop-3 .statement tag=04SS}

$K$ を $S$ から代数閉体 $L$ までの $K$ の体、$S$ 部分環、および $f$ 準同型とします。すると、拡大する $f$ である $L$ に値が入った $K$ の場所が存在します。

命題 1 を考慮すると、これは § 1, no. 2 の定理 2 の翻訳です。

#### 命題 4 {#ac-vi-s2-prop-4 .statement tag=04ST}

$K$を体、$f$を体$L$の値と$K$の$K'$拡大の$K$の位とします。 すると、$L$の拡大$L'$と、拡大する$f$の$L'$に値がある$K'$の$f'$が存在します。 $x_1, \ldots, x_n$ が $K$ と $a_1, \ldots, a_n$ に対して代数的に独立している $K$ の元である場合、元 $\in L$、$f'$ は $1 \leq i \leq n.$ に対して $f(x_i) = a_i$ となるように選択できます。

$V$ を環オフ、$g$ 制限を $V$ および $g$ から $V[x_1, \ldots, x_n]$ の $g'$ 拡大として、$1 \leq i \leq n.$ に対して $g'(x_i) = a,$ を$L'$ とすれば十分です。 $L$ と命題を適用する 3 から $g'$ と $L'$ の代数閉包: 拡大する $g'$ である $K' \to \tilde{L}'$ を取得します。 $x \in K - V,$ の場合、$x^{-1} \in m(V),$ よって $f(x^{-1}) = g(x^{-1}) = 0$ および $f'(x) = \infty = f(x);$ したがって、extendsf になります。

### 5. 場所による積分元の特徴付け

#### 命題 5 {#ac-vi-s2-prop-5 .statement tag=04SU}

Let $K$ be a field, $S$ a subring of $K, h$ a homomorphism from $S$ to a field and $p$ the kernel of $h.$ For an element $x$ of $K$ to be integral over the local ring $S,$ it is necessary and sufficient that every place of $K$ extending $h$ be finite at $x.$

$f$ が $K$ を拡張する場所である場合、$h, f$ は $S_p$ で有限であり、$pS_p$ では零であるため、$f$ の場所の環が$S_p.$ を支配します。 逆に、$V$ が評価額である場合$S_p,$ $V$ を支配する $K$ の環は、制限から $S$ までが準同型であり、$h;$ 置き換えることと同じ核を持つプレースである環です。 $f$ を等価な位で見ると、$V$ は拡大する $h.$ である $K$ の位の環であることがわかります。 $h$ を延長する $K$ のすべての位は $x$ で有限であると言うのは、 $S_p.$ 命題を支配する$K$ のすべての評価環に $x$ 属するを加えたというは、§ 1, no. 3 の 3 である定理から続きます。

#### 命題 6 {#ac-vi-s2-prop-6 .statement tag=04SV}

$K$ を体とし、$K.$ の $S$ 部分環とする。 元 $x \in K$ が $S,$ 上で積分するには、$S$ 上で有限である $K$ のすべての位が次であることが必要かつ十分である。 $x.$で有限

これも、§ 1, no. 3の定理3の帰結です。

### 練習問題 {#ac-vi-s2-exercises}

[§ 2 に対して練習問題](exercises/s2/)を参照してください。
