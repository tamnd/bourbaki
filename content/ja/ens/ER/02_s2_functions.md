---
book: ens
book_title: Theory of Sets
chapter: ER
chapter_title: SUMMARY OF RESULTS
section: 2
section_title: Functions
lang: ja
source: ens-i-iv
source_edition: 2004, Springer
book_pages: 351-357
pdf_pages: 0356-0362
extraction: ocr
statements: 0
exercises: 0
content_sha256: a64f513f662b352e94564abd57429bd359eac09dbc0c6458655a60cc4bc42af0
translated_from: content/en/ens/ER/02_s2_functions.md
translation_method: google
source_content_sha256: e080ea464bff6a7c05c7dc505f506fc7d9e94e4178becde6cca23d33e3bb7827
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-b071ad41
glossary_version: 34
glossary_terms_sha256: 58366d8a54c892a2affbea74dbe1faac227bafe3d975b6ffc6267360d7d12be8
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## 2. 写像

1. E と F を 2 つの集合とします。これは区別できる場合と区別できない場合があります。 E の変数元 $x$ と F の変数元 $y$ の間の関係は、すべての $x \in E$ について、指定された関係内にある一意の $y \in F$ が存在する場合、$y$ の *汎関数関係と呼ばれます。 $x$.*

演算に *写像* という名前を付けます。これは、このようにして、指定された関係と $x$ にあるすべての元 $x \in E$ 元 $y \in F$ に関連付けられます。 $y$ は、元 $x$ における写像の *値* であると言われ、写像は、与えられた関数関係によって *決定される*と言われます。 2 つの *同等* 機能関係決定すると *同じ* 写像。このような写像は、「その値を F で取得」し、「E で定義される」と言われます。より簡単に言うと、E を *写像に *F にしたものとも言われます。

2. 集合 E の集合 F への写像は、新しい集合の *元*、* E *into* F の写像の *集合です。$f$ がこれのいずれかの元である場合E の元 $x$ の $f$ の集合、値は、$f(x)$ で表されることがよくあります。状況によっては、記法 $f_x$ (*指標* 記法と呼ばれ、集合 E は *添字* 集合と呼ばれます) が好ましい場合があります。 関係 "$y = f(x)$" は、$y$ の機能的な関係であり、決定する $f$ です。

形 $y = \langle x \rangle$ の関係 (ここで、$\langle x \rangle$ は $x$ が出現する可能性のある記号の組み合わせを示します) が $y$、写像の汎関数関係である場合、決定するは記法で表されることがよくあります。 $x \rightarrow \langle x \rangle$、または単純に $\langle x \rangle$;これは非常に共通のの言葉の虐待です。たとえば、X と Y が集合 E の 2 つの汎用部分集合である場合、関係 $Y = \complement X$ は Y で機能します。 $\mathfrak{P}(E)$の写像を$\mathfrak{P}(E)$にすると、決定するは$X \rightarrow \complement X$、または単に$\complement X$で表されます。

という 「$f$ を E から F への写像とする」の代わりに、もっと簡単に「$f: E \rightarrow F$ とする」と言うことがよくあります。

複数の写像が関係する状況を説明するには、次のような *図式* も使用します。

$$\begin{array}{ccccc}
 & & \mathrm{C} & & \\
 & \overset{g}{\nearrow} & & \overset{h}{\searrow} & \\
\mathrm{A} \overset{f}{\longrightarrow} \mathrm{B} & \underset{v}{\longrightarrow} & & & \mathrm{E} \\
\downarrow u & & & & \downarrow w \\
\mathrm{D} & \underset{t}{\longleftarrow} & & & \mathrm{F}
\end{array}$$

ここで、矢印に付いている文字は、矢印の尾部の集合から頭の集合への写像を表します。

The relation of equality "$f = g$" between mappings of E into F is equivalent to the relation "for all $x \in \mathrm{E}, f(x) = g(x)$".

3. 集合 E で定義された写像は、E のすべての元 $x$ に対して同じ値 $a$ を取り、E の *定数* 写像と呼ばれます。それは関数関係 $y = a$ によって決定されます。

E の写像を E に結合し、E のそれぞれの元 $x$ と同じ元を *同一性* 写像と呼びます。それは関数関係 $y = x$ によって決定されます。

If A is any subset of E, the mapping of A into E which associates with each element $x$ of A the same element $x$ considered as an element of E is called the *canonical* mapping of A into E.

$f$ をそれ自体の集合 E の写像とします。 E の元 $x$ は、$f(x) = x$ の場合、$f$ より *固定* (または *不変量*) であると言われます。

E の元 $x$ は、E の写像の集合の下で E のそれぞれの下で固定されている場合、*固定* (または *不変量*) であると言われます。

4. $f$ を F の E の写像とし、X を E の任意の部分集合とします。すると、* $f$ の下* X の *像は、F の部分集合 Y、すべての元のからなるになります。 性質を持つ$y$ 「$x \in$ X と $f(x) = y$ となる$x \in$ E が存在します」。

この X と Y の間の定義する関係は Y で機能し、したがって $\mathfrak{P}(\mathrm{E})$ の決定する写像が $\mathfrak{P}(\mathrm{F})$ になります。この写像は、$f$ の * 集合から部分集合までの * 正規の拡大と呼ばれます。* 言葉の乱用により、これも $f$ で示され、$\mathrm{Y} = f(\mathrm{X})$ と書きます。

すべての $f$ と $x$ について、

$$f(\emptyset) = \emptyset \quad \text{and} \quad f(\{x\}) = \{f(x)\}.$$

言葉の乱用により、$f$ の $x$ の *値* $f(x)$ は、* $x$ * 下* $f$ の *像とも呼ばれます。

$y$ が F の総称元である場合、性質 "$y \in f(\mathrm{E})$" は、"$y$ * は形* $f(x)$ である" というというで表現できます。

言葉の乱用により、$f$ の E の像 $f(\mathrm{E})$ は、* $f$ の *像と呼ばれるときどきになります。

$f(\mathrm{E}) = \mathrm{F}$ がある場合、つまり、すべての $y \in$ F に対して、$y = f(x)$ となるような $x \in$ E が存在する場合、$f$ は、E *onto* F の写像、または *全射* 写像、または *全射* であると言われます。

$x$ を E の任意の元と X の任意の部分集合とします。 Instead of saying that $f(x)$ is the value of $f$ at $x$, and $f(\mathrm{X})$ the image of X under $f$, it is sometimes said that $f$ *transforms* (or *maps*) $x$ into $f(x)$ and X into $f(\mathrm{X})$; $f(x)$ and $f(\mathrm{X})$ are then called the *transforms* by $f$ of $x$ and X, respectively.

$f$ が E の写像である場合、E の部分集合 X は、$f(\mathrm{X}) \subset \mathrm{X}$ の場合、$f$ の下で *安定であると言われます。 X がこれら写像のそれぞれの下で安定している場合、部分集合 X は、E への写像の集合の下で *安定* であると言われます。

5. $f$ を E から F への写像とします。すると、次の命題が得られます。ここで、X と Y は E の任意の部分集合を表します。

(a) 関係 $\mathrm{X} \subset \mathrm{Y}$ は $f(\mathrm{X}) \subset f(\mathrm{Y})$ を意味します。

(b) 性質 $\mathrm{X} \neq \emptyset$ は $f(\mathrm{X}) \neq \emptyset$ と同等です。

(c) すべての X について、Y は次のとおりです。

$$(11) \qquad f(\mathrm{X} \cup \mathrm{Y}) = f(\mathrm{X}) \cup f(\mathrm{Y}),$$

$$(12) \qquad f(\mathrm{X} \cap \mathrm{Y}) \subset f(\mathrm{X}) \cap f(\mathrm{Y}).$$

6. $f$ を F の E の写像とし、Y を F の任意の部分集合とします。 * $f$ の下* Y の *逆像は、次のすべての元 $x$ の E からなるの部分集合 X です。 性質 $f(x) \in \mathrm{Y}$。

この X と Y の間の定義する関係は、X で機能します。したがって、$\mathfrak{P}(F)$ の決定する写像が $\mathfrak{P}(E)$ に変換され、f の *逆拡大から部分集合の集合への * 逆関数と呼ばれます。 $\overset{-1}{f}$で示されます。したがって、$X = \overset{-1}{f}(Y)$と書きます。

特に、$y$ が F の元である場合、$\overset{-1}{f}(\{y\})$ はすべての $x \in E$ の集合となり、$f(x) = y$ となります。 関係 「$f(x) = y$」と「$x \in \overset{-1}{f}(\{y\})$」は同等です。言葉の乱用により、$\overset{-1}{f}(\{y\})$の代わりに$\overset{-1}{f}(y)$と書くことがよくあります。

特定の部分集合 A 上の E の部分集合 X の *トレース* $X_A$ は、E (no. 3) への A の標準写像の下の X の逆像です。

7. $f$ を E から F への写像とします。すると、次の命題が得られます。ここで、X と Y は F の任意の部分集合を表します。

(a) 関係 $X \subset Y$ は $\overset{-1}{f}(X) \subset \overset{-1}{f}(Y)$ を意味します。

(b) すべての X について、Y は次のとおりです。

(13) $$\overset{-1}{f}(X \cup Y) = \overset{-1}{f}(X) \cup \overset{-1}{f}(Y),$$

(14) $$\overset{-1}{f}(X \cap Y) = \overset{-1}{f}(X) \cap \overset{-1}{f}(Y),$$

(15) $$\overset{-1}{f}(\complement X) = \complement \overset{-1}{f}(X).$$

注意式 (12) と (14) の違い。 $\overset{-1}{f}$ を F の任意の写像で E に置き換えた場合、(14) はすべての X と Y に当てはまりません。繰り返しますが、任意の写像の拡大については (15) に類似するものはありません。

さらに、$\overset{-1}{f}(\emptyset) = \emptyset$もあります。しかし、F の空ではない部分集合 X に対して $\overset{-1}{f}(X) = \emptyset$ を指定することもできます。 $X \neq \emptyset$ が $\overset{-1}{f}(X) \neq \emptyset$ を意味する順序では、$f$ が E *onto* F の写像であることが必要かつ十分です。

8. E から F への写像 $f$ が、すべての $y \in F$ に対して、$y = f(x)$ となるような * 最大 1 つ* の $x \in E$ が存在するようなものである場合 (他の語、集合 $\overset{-1}{f}(y)$ は空であるか、単一の元で構成されます)、その場合、$f$はEからFへの*1対1* 写像、または*単射* 写像、または*単射*であると言われます。したがって、すべての部分集合 X、E の Y、

(16) $$f(X \cap Y) = f(X) \cap f(Y).$$

9. E から F への写像 $f$ が、すべての $y \in F$ に対して *ちょうど 1 つ存在* $x \in E$ となり、$y = f(x)$ (他の語では、$\overset{-1}{f}(y)$ は 1 つの元で構成される) である場合、$f$ は次のようになります。 E *対* F の *1 対 1* 写像、または *全単射* 写像、または *全単射*。このような写像は、E から F への写像と、E から F への *1 対 1* の写像の両方であると特徴付けることができます。

$f$ が F に対する E の 1 対 1 写像である場合、関係 $y=f(x)$ は $y$ で機能するだけでなく、$x$ でも機能します。 $x$ の汎関数関係として、決定するは F から E への 1 対 1 の写像であり、写像 $f$ の *逆* と呼ばれます。

$f$ の逆数の *拡大は、$f$ の逆数拡大と同じであることに注意してください。

$g$ を $f$ の逆数とします。すると、関係 “$y=f(x)$” と “$x=g(y)$” は *同等* になります。 $g$の逆数は$f$です。 $f$ が E と F の 1 対 1 の写像である場合、関係 (16) だけでなく、E のすべての部分集合 X についても、

$$f(\mathrm{C}X)=\mathrm{C}f(X).$$

さらに、$f$の拡大は、$\wp(F)$に対する$\wp(E)$の写像と1対1です。

E から F への 1 対 1 写像は、その逆写像とともに、*E と F の間の 1 対 1 対応を実現すると言われています*。あるいは、E と F は *これらの写像* によって 1 対 1 の対応に入れられると言います。

集合 E とそれ自体に対する 1 対 1 の写像は、E の *置換* と呼ばれます。恒等写像は置換です。 置換がその逆数と同一である場合、それは *involtory* であると言われます。たとえば、写像 $X\rightarrow \mathrm{C}X$ の $\wp(E)$ 自体への入力は必然的です。

10. 次の命題では、X は E の任意の部分集合を示し、Y は F の任意の部分集合を示します。

(a) $f$ が E *into* F の写像である場合、次のようになります。

(17)
$$f^{-1}(Y)=f^{-1}(Y\cap f(E)),$$

(18)
$$X\subset f^{-1}(f(X)),$$

(19)
$$f(f^{-1}(Y))\subset Y.$$

(b) 「すべての Y について、$f(f^{-1}(Y))=Y$」と「$f$ は E から F への写像」という性質は *同等* です。

(c) 「すべての X、$f^{-1}(f(X))=X$ について」および「$f$ は E から F への *1 対 1* 写像である」特性は *同等* です。

(d) 「すべての X と Y について、

$$f^{-1}(f(X))=X\qquad\text{and}\qquad f(f^{-1}(Y))=Y$$

と「$f$ は E から F への *1 対 1* 写像」は *同等*です。

11. E、F、G を 3 つの集合とします。これらは区別できる場合と区別できない場合があります。 $f$ を F への E の写像とし、$g$ を F から G への写像とする。 E から G への写像のうち、E の任意の元 $x$ における値が $g(f(x))$ であることを、の *合成* と呼ぶ$g$ および $f$ であり、曖昧さの危険がない場合は $g \circ f$、または単に $gf$ で示されます。

等式 $h = g \circ f$ は、$h$ の *因数分解* と呼ばれます。

G が E と異なる場合、$f$ と $g$ の合成 (その順序) について話すことはできず、記法 $f \circ g$ は意味を持たないことに注意してください。 G が E と同一である場合、$f \circ g$ と $g \circ f$ は同じ集合 〜でない限りの元ではなく、F も E と同一です。たとえそうであっても、通常は $f \circ g \neq g \circ f$ です。したがって、$f$と$g$の合成の*順序*が必須です。

$\varphi$ を $g$ と $f$ の合成とし、X を E の任意の部分集合とし、Z を G の任意の部分集合とします。

(20) $$\varphi(\mathrm{X}) = g(f(\mathrm{X})),$$
(21) $$\overset{-1}{\varphi}(\mathrm{Z}) = \overset{-1}{f}(\overset{-1}{g}(\mathrm{Z})).$$

$f$ が E *onto* F の *1 対 1* 写像であり、$g$ が F *onto* G の *1 対 1* 写像である場合、$g \circ f$ は E *onto* G の *1 対 1* 写像です。

$h$ を G の写像から集合 H にすると、次のようになります。

$$h \circ (g \circ f) = (h \circ g) \circ f;$$

E から H へのこの写像は $h \circ g \circ f$ と書かれ、この順序の 3 つの写像 $h$、$g$、$f$ のうちの *合成* と呼ばれます。 3 つ以上の写像のうちの合成も同様に定義されます。

$f$ がそれ自体への E の写像である場合、$f$ の *反復* は、E 自体への写像 $f^n$ ($n$ 整数 $\geqslant 1$) として定義され、$n$ 上の帰納法によって定義されます。 関係 $f^1 = f$、$f^n = f^{n-1} \circ f$; $f^n$ は、$f$ の *n 番目の反復* と呼ばれます。 $f^{m+n} = f^m \circ f^n$ あります。

12. 一般に、写像 $f$ の逆数拡大と拡大の合成 $\overset{-1}{f} \circ f$ は、それ自体では $\mathfrak{P}(\mathrm{E})$ の恒等写像ではありません。同様に、$f \circ \overset{-1}{f}$ は通常、$\mathfrak{P}(\mathrm{E})$ の恒等写像自体にはなりません。これら 2 つの条件は、$f$ が E から F への *全単射* である場合にのみ同時に満たされます。

$f$ が F への E の全単射であり、$g$ が $f$ の逆数を表す場合、合成 $g \circ f$ と $f \circ g$ はそれぞれ E から E への恒等写像と F への F の恒等写像です。

逆に、$f$ が E から F への写像、F から E への $g$ 写像で、$g \circ f$ が E の置換で、$f \circ g$ が F の置換である場合、$f$ は E から F への全単射であり、 $g$はFの全単射をEに重ねたものです。

さらに、$g\circ f$ がそれ自体に対する E の恒等写像である場合、$g$ は $f$ の逆になります。

13. $f$ を E から F への写像とし、A を E の任意の部分集合とします。A から F への写像 $f_A$ のうち、A の任意の元 $x$ における値が $f(x)$ であるものを、 *$f$ から部分集合 A* の制限;それは、A の $f$ の合成と A の E への標準写像です。E から F への 2 つの写像 $f$、$g$ が A に対して同じ制限を持っている場合、それらは A について*同意する (または一致する)* と言われます。 逆に、$f$は E に対する $f_A$ の *拡大* であると言われています。

14. 集合 E *上* 集合 F の写像は、E *による* F の *パラメトリック表現* とも呼ばれます。 E は、この表現の *パラメータ集合* と呼ばれ、E の元は *parameters* という名前になります。

集合 F の *ファミリー 元* は、F の定義部分集合によってパラメトリック表現が与えられています。他の語において、Fの元のファミリーが与えられることは、いくつかの集合Eの写像がFに与えられることと同等である。この写像の下にあるEの像は、ファミリー*の元の*集合と呼ばれる。 F の元の 2 つの異なるファミリーは、その元の集合と同じ F の部分集合を持つ可能性があることに注意してください。

集合 F の各部分集合 A と、元の集合が A である元のファミリーを常に関連付けることができます。 A の *標準写像* によって定義されるファミリーを F に考慮するだけで十分です。

集合 I の写像 $\iota\mapsto x_\iota$ によって F に定義される F の元の族は、$(x_\iota)_{\iota\in I}$ で表されるか、添字集合について曖昧さの可能性がない場合は単に $(x_\iota)$ で表されます。

J が I の部分集合である場合、ファミリー $(x_\iota)_{\iota\in J}$ はファミリー $(x_\iota)_{\iota\in I}$ の J に対する *サブファミリー* 対応すると呼ばれます。 写像 $\iota\mapsto x_\iota$ の制限から J によって定義されます。
