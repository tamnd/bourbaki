---
book: alg
book_title: Algebra
chapter: VI
chapter_title: ORDERED GROUPS AND FIELDS
section: 2
section_title: Ordered fields
lang: ja
source: alg-iv-vii
source_edition: 2003, Springer
book_pages: A VI.37-A VI.47
pdf_pages: 0330-0341, 0348-0358
extraction: ocr
subsections:
    - "no": 1
      title: Ordered rings
      page: 19
      pdf_page: 330
    - "no": 2
      title: Ordered fields
      page: 20
      pdf_page: 331
    - "no": 3
      title: Extensions of ordered fields
      page: 21
      pdf_page: 332
    - "no": 4
      title: Algebraic extensions of ordered fields
      page: 23
      pdf_page: 334
    - "no": 5
      title: Maximal ordered fields
      page: 25
      pdf_page: 336
    - "no": 6
      title: Characterisation of maximal ordered fields. Euler-Lagrange Theorem
      page: 26
      pdf_page: 337
    - "no": 7
      title: Vector spaces over an ordered field
      page: 28
      pdf_page: 339
statements: 33
exercises: 41
content_sha256: f333b9b7a313e66b1a50e13677c22e6c5bcaa5572e61a8fddee525d431bb4feb
translated_from: content/en/alg/VI/02_s2_ordered_fields.md
translation_method: google
source_content_sha256: 10e2ee3ef0d0866e43d0f80ca2949c9e257a5a5b6c77401f65001eb032b1d94c
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-b071ad41
glossary_version: 34
glossary_terms_sha256: 288da7155ddd0a317e627b0a64aca7d2c3c7b3f6dacfd4078e6db881dd7256c4
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## § 2。 順序体

### 1. 注文しました環

#### 定義 1 {#alg-vi-s2-def-1 .statement tag=06YV}

— Given a commutative ring $\mathbf{A}$, we say that an ordering on $\mathbf{A}$ is compatible with the ring structure of $\mathbf{A}$ if it is compatible with the additive group structure of $\mathbf{A}$, and if it satisfies the following axiom :
(OR) The relations $x \geqslant 0$ and $y \geqslant 0$ imply $xy \geqslant 0$.
The ring $\mathbf{A}$, together with such an ordering, is called an ordered ring.

#### 例 1 {#alg-vi-s2-n1-exa-1 .statement tag=06YW}

環 $\mathbf{Q}$ と $\mathbf{Z}$ は、通常の注文では環となります。

#### 例 2 {#alg-vi-s2-n1-exa-2 .statement tag=06YX}

注文した環の積には、積の注文が装備されており、注文した環になります。特に、集合 $E$ から順序付き環 $\mathbf{A}$ までの写像の環 $\mathbf{A}^E$ は順序付き環です。

#### 例 3 {#alg-vi-s2-n1-exa-3 .statement tag=06YY}

順序付けされた環の部分環は、誘導順序付けにより、順序付けされた環になります。

順序付けされた環、関係 $x \geqslant y$、および $z \geqslant 0$ は $xz \geqslant yz$ を意味します。実際、これらの不等式はそれぞれ $x - y \geqslant 0$、$z \geqslant 0$、$(x - y)z \geqslant 0$ に相当します。
同様に、関係 $x \leqslant 0$ と $y \geqslant 0$ (それぞれ $y \leqslant 0$) は $xy \leqslant 0$ (それぞれ $xy \geqslant 0$) を暗示していることがわかります。これらの結果は、符号規則の名の下に呼び出されることがよくあります (2 つの元は、両方とも $\geqslant 0$ または両方とも $\leqslant 0$ である場合、同じ符号を持つと言われます)。これらは、$\mathbf{A}$ が完全に順序付けられた環である場合、すべての平方が正であり、特にすべての冪等 (たとえば、単位元) が正であることを意味します。

#### 例 {#alg-vi-s2-n1-exa-4 .statement tag=06YZ}

$\mathbf{Z}$ に完全に注文された環構造は 1 つだけです。実際、帰納法までに、自然数 $n \neq 0$ ごとに $1 > 0$、よって $n > 0$ です。対照的に、完全に順序付けられていない $\mathbf{Z}$ には順序付けられた環構造が存在します (以下を参照)。

$P$ を、順序付けられた環 $\mathbf{A}$ の正の元の集合とします。 $\mathbf{A}$ の順序は $P$ 決定するであることが知られています (VI、p. 3、提案 3)。 $\mathbf{A}$ が順序付けられた環であると言うのは、 $P$ が次の特性を満たすというと同等です。

$$
\begin{align*}
(\mathrm{AP}_I) &\quad P + P \subset P \\
(\mathrm{AP}_{II}) &\quad PP \subset P \\
(\mathrm{AP}_{III}) &\quad P \cap (-P) = \{0\}
\end{align*}
$$

確かに、$(\mathrm{AP}_I)$ と $(\mathrm{AP}_{III})$ は、$\mathbf{A}$ の加法群が順序付き群 (VI、p. 3、提案 3) であり、$(\mathrm{AP}_{,,})$ が (OR) の変換であると述べています。

$\mathbf{A}$ の位数関係を合計するには、次の条件が必要かつ十分であることを思い出してください。

$$
(\mathrm{AP}_{IV}) \quad P \cup (-P) = \mathbf{A}.
$$

#### 例 {#alg-vi-s2-n1-exa-5 .statement tag=06Z0}

$\mathbf{Z}$ では、$P$ を正の (通常の意味で) 整数の集合とすると、完全に順序付けられていない環が得られます。

また、完全に順序付けされたアーベル群、関係 $n \cdot x = 0$ (自然数 $n \neq 0$ の場合) は $x = 0$ (VI、p. 4) を意味することも思い出してください。これにより、次の結果が得られます。

#### 命題 1 {#alg-vi-s2-prop-1 .statement tag=06Z1}

— *完全に注文された環は、$\mathbf{Z}$ モジュール* (II、p. 313) として無料で捩れです。

### 2. 順序体

#### 定義 2 {#alg-vi-s2-def-2 .statement tag=06Z2}

— 全順序を備えた可換 *体は、 *その順序と環構造が互換性がある*場合、 順序体* と呼ばれます。

他のものは非常に「病的」であるため、体の *合計* 位数関係に制限します (VI、p. 38、例 6)。

#### 例 {#alg-vi-s2-n2-exa-2 .statement tag=0DID}

*1) 有理数数の体$\mathbf{Q}$は順序体です。
2) 順序体の部分体は、誘導順序付けすると、順序体になります。
3) \* 実数の体は順序体です。 \*

$K$を順序体とします。すべての $x \in K$ に対して、

$$
\begin{align*}
\operatorname{sgn}(x) &= 1 & \text{if } x > 0, \\
\operatorname{sgn}(x) &= -1 & \text{if } x < 0, \\
\operatorname{sgn}(x) &= 0 & \text{if } x = 0.
\end{align*}
$$

次に、$\operatorname{sgn}(xy) = \operatorname{sgn}(x) \operatorname{sgn}(y)$ になります。私たちは$\operatorname{sgn}(x)$を$x$の*記号*と呼びます。 The map $x \mapsto \operatorname{sgn}(x)$ from $K^*$ to the multiplicative group $\{-1, +1\}$ is a surjective homomorphism whose kernel, the set of strictly positive elements of $K$, is a subgroup of $K^*$ of index 2.

Conversely, if $K$ is a commutative field and $s : K^* \to \{-1, +1\}$ is a surjective homomorphism whose kernel is closed under addition, then $s$ is the sign map for a unique ordered field structure, where the set of strictly positive elements is the kernel of $s$.

$K$ のすべての $x$ と $y$ に対して、$x = \operatorname{sgn}(x)|x|$ と $|xy| = |x||y|$ があります。

一方、すべての順序体は標数0 になります (提案 1)。

#### 命題 2 {#alg-vi-s2-prop-2 .statement tag=06Z3}

— *$A$ を完全に順序付けられた整域とし、$K$ を分数の体とします。次に、$K$ には 1 つだけの順序が存在します。これは、$A$ の指定された順序に制限するを加えて、$K$ 順序体になります。*

すべての$x \in K$は形$x = ab^{-1}$で表現でき、$a$と$b$は$A$と$b \neq 0$で表現できます。 $x$ が正の場合、$a$ と $b$ は同じ符号を持ち、その逆も同様です。 したがって、規定の条件 $K$ 満たすに順序付けが存在する場合、それは一意であり、正の元の集合 $P$ は $ab^{-1}$ の集合と同一であることがわかります。ここで、$a$ と $b$ は同じ記号の $A$ の元と $b \neq 0$。 $P$ が条件 (AP$_I$)、(AP$_{II}$)、(AP$_{III}$)、および (AP$_{IV}$) を満たすことを示すことはまだ残っています。 これは (AP$_{II}$) と (AP$_{IV}$) については明らかです。 (AP$_I$) については、$ab^{-1} + cd^{-1}$ を考慮します。ここで、$a$、$b$、$c$、および $d$ が正であると仮定できます。この和は$(ad + bc)(bd)^{-1}$で、$ad + bc$と$bd$は正です。

$(\mathrm{AP}_{III})$ を表示するには、形 $ab^{-1} = -cd^{-1}$ の恒等式を考慮すると、$ad + bc = 0$ になります。 $a$ と $b$ が同じ符号を持ち、$c$ と $d$ が同じ符号を持つと仮定すると、符号規則は $ad$ と $bc$ が同じ符号を持つことを示します。 よって $ad = bc = 0$、つまり $a = c = 0$;したがって、$P$ は確かに満たす $(\mathrm{AP}_{III})$ になります。

#### 例 {#alg-vi-s2-n2-exa-1 .statement tag=06Z4}

— $Z$ は 1 つの完全な順序付け環構造 (*VI*、p. 19、*例*) のみを許可するため、体 $\mathbf{Q}$ は 1 つの順序付けのみを許可し、順序体になります。これは通常の順序付けです。

### 3. 拡大/順序体

#### 定義 3 {#alg-vi-s2-def-3 .statement tag=06Z5}

※$K$を順序体とします。 $K$ の順序付き拡大は対 $(E, u)$ です。ここで、$E$ は順序体、$u$ は $K$ から $E$ までの増加する準同型です。

$K$を体、$E$を順序体、$u : K \to E$を準同型とします。 関係
$$
x \leq y \quad \text{if} \quad u(x) \leq u(y)
$$
$K$ の合計位数関係は、順序体構造となり、$E$ の合計によって *誘発*されたと言われています。 $K$と$E$が順序体である場合、$K$の順序体構造が$E$の⟧の順序体構造が誘発された場合に限り、準同型$u : K \to E$は増加するになります。通常は同一視する $K$ で、その像は $u$ の下の $E$ になります。

#### 例 {#alg-vi-s2-n3-exa-1 .statement tag=06Z6}

— 1) すべての順序体 $K$ は、$\mathbf{Q}$ の順序付けられた拡大です。実際、$K$ は標数0 であるため、$\mathbf{Q}$ の拡大であり、一方、$\mathbf{Q}$ は、今見たように、一方向でのみ注文できます。

2) $K$ を順序体とし、$K(X)$ を $K$ 上の 1 つの不定数における有理数写像の体とする。正の元を $0$ とし、先頭の係数が正である多項式を使用して、多項式環 $K[X]$ の順序付け定義するを考えてみましょう。このようにして、完全に順序付けされた環が得られ、その順序付け拡大するは $K$ の順序付けとなります。 適用提案 2 により、$K$ の順序付けられた拡大の $K(X)$ 構造が得られます。 *$K = \mathbf{R}$ については、このように $K(X)$ で定義された位数関係は、$+\infty$ 付近の成長のものであることがわかります (cf. *VI*、p. 24、提案 4)。

#### 定理 1 {#alg-vi-s2-thm-1 .statement tag=06Z7}

*For an extension $E$ of $K$ to admit the structure of an ordered extension of $K$, the following condition is necessary and sufficient:*
*(OE)* *The relation $p_1 x_1^2 + \ldots + p_n x_n^2 = 0$ implies*
$$
p_1 x_1 = \ldots = p_n x_n = 0
$$
*for any finite sequence $(x_i, p_i)$ of pairs of elements $x$, of $E$ and positive elements $p_i$ of $K$.*

Condition (OE) is clearly equivalent to:
(OE') *The element – 1 is not a sum of elements of the form* $px^2$ ($x \in E, p \in K, p \geq 0$).

条件 (OE) が必要です。E が K の順序付けられた拡大である場合、元 $p_i x_i^2$ は E において正であるため、その和が零である場合、零になります。一方、$p_i x_i^2 = 0$ は $p_i x_i = 0$ と同等です。

逆に、条件 (OE) が満たされると仮定すると、条件 (AP_I)、(AP_{II})、(AP_{III})、および (AP_{IV}) を満たす E の部分集合 P を構築することによって、E に対する順序付けが定義する行われます。 K の正の元の含む集合 $K_+$。そのような部分集合 P は確実に E を K の順序付き拡大にします。なぜなら、$K \cap P = K_+$ が得られるからです。実際、P が K の含む元 $-a < 0$ であれば、a は属するから $P \cap (-P)$ となり、(APIIII) と矛盾します。

定義する P に対して、E の部分集合の集合 $\mathscr{M}$ のうち、満たす (AP_I)、(AP_{II})、および (AP_{III})、および $K_+$ の含む和集合と、 Eの集合C、平方、元。 この集合 $\mathscr{M}$ は、空でないです。つまり、形 $\sum p_i x_i^2$ の元の含む集合 $P_0$ ($P_0$ が (AP_{III}) を満たすことは、(OE) からすぐに続きます)。

さらに、$\mathscr{M}$ は帰納的です (*集合理論*、III、p. 154、定義 3)。したがって、Th によると、存在します。 $\mathscr{M}$ の *集合理論*、III、p. 154、極大元の 2 つ。これが満たされるかどうかはまだ証明する必要があります (AP_{IV})。これは次の補題から続きます。

#### 補題 {#alg-vi-s2-n3-lem-1 .statement tag=06Z8}

— *しましょう* $P \in \mathscr{M}$ *そして* $x \notin P$; *その後、* $P' \in \mathscr{M}$ *そのような* $P \subset P'$ *そして* $-x \in P'$ が存在します。

$P' = P - xP$ を取得し、$P'$ に必要なプロパティがあることを確認します。 $0 \in C \subset P$ なので、$P \subset P'$ になります。 よって $C \subset P'$ と $K_+ \subset P'$ 。 $1 \in C \subset P$ なので、$-x \in P'$ になります。私たちは持っています
$$
P' + P' = P - xP + P - xP = P + P - x(P + P) \subset P - xP = P',
$$
よって (AP_I)。私たちは持っています
$$
P'P' = (P - xP)(P - xP) \subset \\
\quad \subset PP + x^2PP - x(PP + PP) \subset P + CP - xP \subset P - xP = P',
$$
よって (AP_{II})。最後に、(AP_{III}) を確認してみましょう。P に対して $p, q, r, s$ 属するの ID が形 $p - xq = -(r - xs)$ であると仮定します。これから関係 $x(s + q) = p + r$ と推測します。 $s + q \neq 0$ があれば
$$
x = (s + q)^{-2}(s + q)(p + r) \in CPP \subset P,
$$
仮定とは反対。したがって、$s + q = 0$、よって $p + r = 0$; P は (AP_{III}) を満たすため、$s = q = r = p = 0$ が推定され、証明が完成します。

#### 系 1 (*« アルティン・シュライヤー 定理 »*) {#alg-vi-s2-thm-1-cor-1 .statement tag=06Z9}

— *可換体* E *それを順序体にする順序が存在するためには、*必要十分な条件、つまり関係* $x_1^2 + \ldots + x_n^2 = 0$ *暗黙* $x_1 = \ldots = x_n = 0$。

必要性は明らかです。逆に、記述された条件は、E が標数0 であり、したがって Q の拡大であることを意味します。次に、条件 $(OE)$ が満たされ、Th. 1 は、Q の順序付き拡大の E 構造、つまり順序体構造が存在することを示しています。

$-1$ が平方である体 E には、特に代数閉体には順序体構造は*存在しません*。

#### 系 2 {#alg-vi-s2-thm-1-cor-2 .statement tag=06ZA}

*E を、K の順序付き拡大の構造を認める K の拡大とします。E のすべての構造の下で元 $x \in E$ が正になるためには、x が形 $\sum_i p_i x_i^2$ であることが必要かつ十分です。ここで、$x_i \in E$ と $p_i$ K.* の元が正です。

条件で十分なのは明らかです。 (Th. 1 の証明の記法において) $x \notin P_0$ であれば、$x \notin P$ となる $\mathscr{M}$ の極大元 P が存在することも必要です。次に、$-x \in P$ by 補題、そして x は、$x \neq 0$ 以降、P で定義された順序付けでは正ではありません。

### 4. 代数拡大/順序体

K を順序体とし、f を K[X] の多項式とします。 $f(a) f(b) < 0$ となるような K に 2 つの元 a と b が存在する場合、*f 変更は K* に署名すると言います。次に、*f 変更 a と b* の間で符号すると言います。

#### 命題 3 {#alg-vi-s2-prop-3 .statement tag=06ZB}

*K を順序体とし、f を K の a と b の間で変更符号する K 上の既約多項式とします。その場合、K の拡大 $E = K[X]/(f)$ は順序付き拡大の構造を許容します。*

帰納法次数 noff までに議論します。 $n = 1$ にとって、証明は些細なことです。結果が次数 $\leq n - 1$ に当てはまると仮定し、次数 n について矛盾によって証明してみましょう。 Th 著1 したがって、形の関係を仮定します。

$$
1 + \sum_i p_i f_i^2(X) \equiv 0 \pmod{f(X)}, \quad \text{where } f_i \in K[X], \quad p_i \in K \quad \text{and} \quad p_i \geq 0
$$

一般性を失わずに、$f_i$ は次数 $\leq n - 1$ (*IV*, p. 11, Cor) を持つと仮定できます。それから

$$
1 + \sum_i p_i f_i^2(X) = h(X) f(X)
$$

ここで、$h \neq 0$ には次数が最大でも $n - 2$ 含まれます。 置き換えること X 上記の不等式の a と b により、$h(a) f(a) > 0$ と $h(b) f(b) > 0$ がわかります。 f 変更は a と b の間で仮定によって署名されるため、$h(a) h(b) < 0$ は結論するとなります。次に、$h(X)$ の既約因子 $g(X)$ の 1 つに対して、同様の不等式が得られます。つまり、$g(a)\ g(b) < 0$ です。しかし、$1 + \sum_i P_i f_i^2(X) \equiv 0 \pmod{g(X)}$ は、体 $K[X]/(g)$ できないが、帰納法の仮定とは反対に、$K$ (木曜日 1) の順序付けられた拡大であることを示しています。

#### 注意 {#alg-vi-s2-n4-rem-1 .statement tag=06ZC}

順序体 $K$ には、変更は$K$ にサインインしないが、$K[X]/(f)$ は$K$ の順序付けられた拡大の構造を認めるような既約多項式$f$ が存在します。 (cf. VI、p. 43、例 26、c))。

位数で前の命題を適用するには、次の結果が必要になります。

#### 命題 4 {#alg-vi-s2-prop-4 .statement tag=06ZD}

— *$K$を順序体とし、$f \in K[X]$とします。 $K$ には区間が存在し、その補数の $f$ はその最高次数項と同じ符号を取ります。*

モニック多項式の場合をすぐに簡約する理解できます。その場合、$x \neq 0$ を $f(x) = x^n(1 + a_1 x^{-1} + \ldots + a_n x^{-n})$ と書くことができます。しましょう

$$
M = \sup (1, |a_1| + \cdots + |a_n|).
$$

$|x| > M$ には $1 + a_1 x^{-1} + \ldots + a_n x^{-n} > 0$ があり、命題の証明が完成します。

#### 系 1 {#alg-vi-s2-prop-4-cor-1 .statement tag=06ZE}

— *奇数有限次数の順序体のすべての拡大は、順序付けられた拡大の構造を認めます。*

このような拡大は単次 (V、p. 40、Th. 1) であるため、$K[X]/(f)$ と同型です。ここで、$f$ は奇数次数の既約多項式です。次に、$f$ 変更が$K$ (提案 3) にサインインすることを示すだけで十分です。これは、提案 4 の直後に続きます。

#### 系 2 {#alg-vi-s2-prop-4-cor-2 .statement tag=06ZF}

— *$a$ が順序体 $K$ の正の元である場合、多項式 $X^2 - a$ のすべての分解体 $E$ は、次の順序付けられた拡大の構造を許容します。 $K$.*

$a$ が $K$ の平方であれば、結果は自明です。それ以外の場合、多項式 $f(X) = X^2 - a$ は既約であり、$f(0) < 0$ と $f(x)$ は $x^2$ と同じ符号を持ち、$K$ の一部の区間の補数で $x$ が正であるため、変更の符号になります。これで、適用提案 3 によって証明を完了できます。

#### 注意 {#alg-vi-s2-n4-rem-2 .statement tag=06ZG}

順序体 $K$ 含むの場合、$K$ (多項式 $X^2 - a$ の根) の正の元 $a$ の « 平方根 » の場合、記法 $\sqrt{a}$ は通常 *ポジティブ* 平方根のために予約されています。 $K$ が含む平方根 $b$ と体 $E$ の $a$ の $-b$ が*でない場合、後者は *2* で $K$ の順序付き拡大にすることができます。それぞれが、$b$ を $-b$ に送信する$K$-自己同型作用を*介して、お互いから誘導されます。これらの順序決定する $\sqrt{a}$ の 1 つの選択: 元 $b$ と $-b$ のいずれかが正です。

$a$ と $a'$ が $K$ の 2 つの正の元で、その平方根が $K$ にある場合、$\sqrt{a}$ の定義と符号規則から続く $\sqrt{aa'} = \sqrt{a} \sqrt{a'}$ です。

### 5. 極大順序体

#### 定義 4 {#alg-vi-s2-def-4 .statement tag=06ZH}

— *順序体 K のすべての順序代数拡大が自明である場合、K は最大になります。*

#### 例 {#alg-vi-s2-n5-exa-1 .statement tag=06ZI}

*後で (Gen. Top.、VIII、p. 1) で、実数の体 R が極大順序体であることがわかります。

極大順序体の存在は、次の定理の帰結です。

#### 定理 2 {#alg-vi-s2-thm-2 .statement tag=06ZJ}

— *すべての順序体 K は、極大順序体である順序代数拡大を認めます。*

この順序付けられた拡大が K-同型写像 (VI、p. 40、例 15) まで一意であることを示すことができます。

$\Omega$ を K の代数閉包とし、$\mathfrak{N}$ を対 $(A, w)$ の集合とします。ここで、$A$ は $\Omega$ のサブ K 拡張であり、$w$ は $A$ の順序付けです$A$ は $K$ の拡大を注文しました。 関係による位数 $\mathfrak{N}$ « L は、M と $L$ の間の M » の順序付けられた拡大です。この順序付けを適用すると、$\mathfrak{N}$ は *帰納的* 順序付けされた集合です。実際、$(L_i)$ が $\mathfrak{N}$ の元の完全に順序付けられた族である場合、$L_1 = \bigcup (L_i)_1$ を取ることによって順序付けされた体 $L = \bigcup L_i$ は、上界になります。 $L_i$。次に、$\mathfrak{N}$ は *集合理論*、III、p. 154、Th によって極大元になります。 2、これで証明が完了します。

#### 命題 5 {#alg-vi-s2-prop-5 .statement tag=06ZK}

— *K を極大順序体とし、f を K[X] の多項式とし、K の 2 つの元 a と b ($a < b$ を含む) の間で変更符号を付ける。この場合、f は K に $a < x < b$ となるような根 x を持ちます。*

$a$ と $b$ の間に、既約の因子の少なくとも 1 つ、たとえば $h$、変更の符号が存在します。次に、体 $K[X]/(h)$ は、$K$ の順序付けられた拡大の構造を認め (VI、p. 23、提案 3)、$h$ は次数 1 になります (定義 4)。 $h(a) h(b) < 0$ であるため、$h$ の一意の根 $x$ は、次数 1 の多項式関数が単調であるため、$a < x < b$ となります。

#### 命題 6 {#alg-vi-s2-prop-6 .statement tag=06ZL}

— *極大順序体 K のすべての正の元は、K に平方根を持ちます。K[X] の奇数次数のすべての多項式は、K に少なくとも 1 つの根を持ちます。

これはコルからすぐに続きます。 2 と 1 をVI、p. 24 の提案 4 に適用します。

#### 系 {#alg-vi-s2-n5-cor-1 .statement tag=06ZM}

— *極大順序体 K には、体構造と互換性のある順序が 1 つだけ存在します。*

実際、K の正の元はその代数構造によって決定され、それらは平方になります。

### 6. 極大順序体の特徴。オイラー・ラグランジュ定理

VIの提案6で表される性質、p. 25が極大順序体を特徴づけます。より正確には:

#### 定理 3 (オイラー ラグランジュ) {#alg-vi-s2-thm-3 .statement tag=06ZN}

— K を順序体とします。したがって、次の 3 つのプロパティは同等です。
a) 体 $K(i)$ は代数的に閉じています (i は -1 の平方根を示します)。
b) 順序体 K は最大です。
c) K のすべての正の元は平方であり、$K[X]$ の奇数次数のすべての多項式は K に根を持ちます。

a) が b) を暗示していることは明らかです。実際、K には、同型までの 2 つの代数拡大、K 自体の体、および -1 が平方であるためできないが順序付けされる $K(i)$ だけがあります。

b) が c) を意味するという事実は、VI, p. 25 の提案 6 に他なりません。

c) が a) を意味することを証明することは私たちに残されています。次の 2 つの命題以降がそれに続きます。

#### 命題 7 {#alg-vi-s2-prop-7 .statement tag=06ZO}

— K を順序体とし、すべての正の元が平方であるとします。すると、$K(i)$ のすべての元は平方となり、$K(i)$ 上の次数 2 のすべての多項式は、$K(i)$ に根を持ちます。

まず最初に 2 番目の主張簡約するを示しましょう。 2 番目の多項式次数 $aX^2 + bX + c$ ($a \neq 0$) を次の形に入れることができます。これは、多くの場合、正準三項式形と呼ばれます。

$$
a((X + (b/2a))^2 - (b^2 - 4ac)/4a^2)
$$

d が $(b^2 - 4ac)/4a^2$ の平方根である場合、$d - (b/2a)$ は考慮中の二次多項式の根です。

ここで、すべての元 $a + bi$ ($a \in K, b \in K$) が平方であることを示します。私たちは次のような元 $x + yi$ を探しています

$$
(x + yi)^2 = a + bi;
$$

これは、$x^2 - y^2 = a$ と $2xy = b$ に変換されます。これから推測すると、

$$
(x^2 + y^2)^2 = a^2 + b^2
$$

c が $a^2 + b^2$ の正の平方根を表すものとします。次に$c \geq |a|, c \geq |b|$と$x^2 + y^2 = c$。 よって $x^2 = (c + a)/2$ と $y^2 = (c - a)/2$ 。 $c \geq |a|$ なので、これらの方程式は K で可溶であり、$x_0$ と $y_0$ が 2 つの解である場合、$x_0^2 - y_0^2 = a$ と $2x_0y_0 = \pm b$ になります。 $x = x_0$ と $y = b/2x_0$ を取ることで、目的の平方根を取得します。

#### 命題 8 {#alg-vi-s2-prop-8 .statement tag=06ZP}

— 多項式 $X^2 + 1 \in K[X]$ (V, p. 21) に対して、K を (任意の特性の) 可換体とし、$K'$ を分解体とします。次のように仮定します。
a) 奇数次数の $K[X]$ のすべての多項式は $K'$ に根を持ちます。

b) 次数 2 の $K'[X]$ のすべての多項式は、$K'$ に根を持ちます。
この場合、$K'$ は代数的に閉じられます。

注意まず、$K[X]$ のすべての非定数多項式が $K'$ に根をもつことを証明できれば十分です。これは、$K' = K$ であれば確かに明らかです。 $K' \neq K$ の場合は $[K':K] = 2$; $a \mapsto a$ は、同一性写像とは異なる $K'$ の固有の $K$ 自己同型を表すものとします。 $f \in K'[X]$ で、$\bar{f}$ が $f$ の適用 $a \mapsto \bar{a}$ ～ 係数によって得られる多項式を表す場合、$f \bar{f} \in K[X]$。 $a \in K'$ が $f \bar{f}$ の根である場合、$a$ は $f$ の根または $\bar{f}$ のいずれかになります。したがって、$a$ または $a$ は、$f$ の根になります。

したがって、$f$ を、次数 $2^n p$、$p$ 奇数の $K$ にわたる多項式とします。 *私たち*は、$n$の帰納法までに進み、性質は仮定までに$n = 0$に当てはまります *a)*。 E を $K$ の拡大とし、$f$ 分裂を線形因子に変換します。

$$
f(X) = \prod_i (X - a_i)
$$

$b \in K$ にしましょう。 $y_{ij} = a_i + a_j + ba_i a_j \in E$を入れて、

$$
h(X) = \prod_{i < j} (X - y_{ij}) \in E[X].
$$

この多項式の係数は、$a_i$ では写像、$K$ では係数と対称です。したがって、属するから $K[X]$ (IV、p. 62、Th. 1)。 次数 $2^n p (2^n p - 1)/2 = 2^{n-1} p'$ ($p'$ 奇数) があるので、帰納法仮定により $K'$ では根 $y_{}$ になります。これがすべての $b \in K$ に当てはまり、$K$ が無限体であることに注意すると (実際、有限体は任意の大きな奇数次数 (V、p. 94、提案 3)、できない満たすの単次拡大を持ちます) *a)*) の場合、次のような少なくとも 1 つの対 $(i, j)$ の存在を推定できます。

$$
a_i + a_j + ba_i a_j \in K' \quad \text{and} \quad a_i + a_j + b'a_i a_j \in K',
$$

$b \neq b'$と。次に、$a_i + a_j$ と $a_i a_j$ は $K'$ の元であり、従って、$a_i$ と $a_j$ も二次方程式の根なので同様です。

$$
x^2 - (a_i + a_j)x + a_i a_j = 0.
$$

Q.E.D.

ガロア理論に基づく、提案 8 の一般化と代替案証明については、VI、p. 46、例を参照してください。 33.

Let $K$ be an ordered field and let $K' = K(i)$; for every element $z = a + bi$ of $K'$, the norm $z \overline{z} = a^2 + b'$ of $z$ relative to $K$ (III, p. 544, example 1) is a positive element of $K$, which vanishes only for $z = 0$. $K$ のすべての正の元が平方である場合 (特に $K$ が極大順序体の場合)、ノルム $z \overline{z}$ の正の平方根は $z$ の絶対値と呼ばれ、次のように書かれます。 $|z|$。 $|zz'|^2 = |z|^2 |z'|^2$ なので、$|zz'| = |z| \cdot |z'|$ になります。

さらに、三角形不等式

$$
|z + z'| \leq |z| + |z'|
$$

元 $z, z'$ の $K'$ のすべての対に当てはまります。確かに、$z = a + bi$ と $z' = a' + b'i$ の場合、この不等式は次と同等です。

$$
(a + a')^2 + (b + b')^2 \leq a^2 + b^2 + {a'}^2 + {b'}^2 + 2 \sqrt{(a^2 + b^2)({a'}^2 + {b'}^2)}
$$

したがって、また

$$
(aa' + bb')^2 \leq (a^2 + b^2)({a'}^2 + {b'}^2)
$$

$(ab' - ba')^2 \geq 0$と書くことができます。

Th. 3 により、極大順序体上のすべての既約多項式を決定するできるようになります。

#### 命題 9 {#alg-vi-s2-prop-9 .statement tag=06ZQ}

— *K が極大順序体の場合、K[X] の既約多項式は、最初の次数多項式と、$b^2 - 4ac < 0$ となる 2 番目の次数多項式 $aX^2 + bX + c$ だけです。

$K(i)$ は代数的に閉じているため、K のすべての代数拡大、したがって K 上のすべての既約多項式も次数 1 または 2 を持ちます。どの 2 番目の次数多項式が既約であるかを確認するには、正準形 $a((X + (b/2a))^2 - (b^2 - 4ac)/4a^2)$ を考慮するだけで十分です。 (cf. *VI*、p. 26、提案 7)。

#### 注意 {#alg-vi-s2-n6-rem-1 .statement tag=06ZR}

— 正準三項式形に変換すると、次のより強力な結果が得られます。特定の順序体 K 上の多項式 $aX^2 + bX + c$ が K の定数符号を持つために必要かつ十分な条件は、$b^2 - 4ac < 0$ であり、多項式の符号は $a$ になります。

### 7. ベクトル空間順序体

K を順序体とし、E を $K$ 以上のベクトル空間とします。 関係 « $K$ に $\lambda > 0$ が存在し、集合 $E - \{0\}$ の 2 つの元 $x$ と $y$ の間の $y = \lambda x$ » が *同値関係* になります。この関係の下の同値類は *原点 0 の開いたハーフライン * と呼ばれます。開いた半線の和集合と $\{0\}$ は、原点 0 の *閉じた半線 * (またはときどきは単に *ハーフライン *) と呼ばれます。 開いた (それぞれ閉じた) 半線 A に含まれるすべてのベクトル $a \neq 0$ は、 $A$ の * 方向ベクトル* と呼ばれ、 $A$ は、すべてのスカラー $A > 0$ (それぞれ $A \geq 0$) のベクトル $ha$ の集合です。 $D$ から 0 含むまでのすべての行は、原点 0 を持つちょうど 2 つの開いた (それぞれ閉じた) 半線です。 $A$ がこれらの 1 つである場合、$-A$ はもう 1 つです ($A$ の *反対* と呼ばれます)。

ここで、$F$ が $K$ 上の *アフィン空間*、および F の変換の E 空間である場合、形 $A = a + A_0$ の F の任意の部分集合 ($\Delta_0$ は E の開いた (または閉じた) 半線) は *open* と呼ばれます。 (それぞれ *閉じた*) *原点のある半線* $a \in F$。半線 $\Delta_0$ は、$A$ によって完全に決定され (これは、$A$ の任意の $b \neq a$ に対して、ベクトル $b - a$ の方向を持つ半線であるため)、$A$ の *方向* と呼ばれます。 $A$のベクトル方向は、$A$の*方向ベクトル*とも呼ばれます。

Suppose now that E has *finite* dimension $n$ over K ; then it is known (III, p. 518, Cor. 1) that the *n-th exterior power* $\Lambda^n E$ is a vector space of dimension 1 over K, and so the union of two opposite closed half-lines of origin 0. これらの半線は E の方向と呼ばれます。 空間 E とこれらの半線 A のいずれか 1 つが方向付けされていると言われます。 n ベクトル z は、A に対して属する (または −A) である場合、この配向の下で正 (または負) と呼ばれます。反対の方向では負（または正）になります。

An orientation of an affine space F over K is by definition an orientation of the space of translations of F; the space F, together with such an orientation, is called an oriented affine space.

E を K 上の次元 $n$ のベクトル空間とします。 E の順序付き基底 $(a_i)_{1 \leq i \leq n}$ は、n ベクトル $a_1 a_2 \ldots a_n$ が正 (それぞれ負) の場合、正または直接 (それぞれ負または逆) と呼ばれます。 $u$ がベクトル空間 E の自己同型である場合、すべての $z \in \bigwedge^n E$ に対して $(\bigwedge^n u)(z) = \det(u) \cdot z$ であるため、$\bigwedge^n u$ が E の方向を不変のままにする (または、方向を維持する) ために必要かつ十分な条件は、$\det(u) > 0$ です。この性質を持つ自己同型は、方向性のあるベクトル空間として正確に E の自己同型です。それらは形線形群 $\mathrm{GL}(E)$ の通常の部分群 $\mathrm{GL}^+(E)$ であり、$E \neq 0$ のたびに添字 2 になります。

$E = 0$ の場合、$\mathrm{GL}(E) = \mathrm{End}(E)$ 含むは ID 写像 1 のみとなり、定義 $\det(1_E) = 1$ までになります。この場合、$\bigwedge^n E = \bigwedge^0 E = K$ by 定義であることに注意してください。正のスカラーによって形成される K の半線は、零空間の正準配向と呼ばれます。

Let M and N be two complementary subspaces of dimensions p and $n - p$ respectively in the vector space E of dimension n; if $z'$ (resp. $z''$) is a nonzero vector in $\bigwedge^p M$ (resp. $\bigwedge^{n-p} N$), then $z' \wedge z''$ is a nonzero vector in $\bigwedge^n E$. M の方向と N の方向が与えられると、正の $z'$ および $z''$ 形の場合はベクトル $z' \wedge z''$、N の方向による M の方向の積方向と呼ばれます ($p(n-p)$ が奇数の場合、因子の位数に依存します)。 逆に、E と M 上に与えられた方向があると、E 上の与えられた方向が M 上の与えられた方向の積となり、N 上のこの方向が (つまり位数) となるような固有の方向が N 上に存在します。この配向は、E の配向に対して M の配向と相補的であると言われます。 $N'$ が M に対する 2 番目の相補的な部分空間である場合、M に平行な正規の射影 $N \to N'$ は、N の相補的な方向を $N'$ の方向にとります。 したがって、標準写像 $N \to E/M$ の下での N の相補的配向の像は、補数 N の選択から独立しています。 E の方向と M の方向を合わせたものを、E/M 上の商方向と呼びます。

練習問題

### 練習問題 {#alg-vi-s2-exercises}

考慮中のすべての環は、そうでない場合は明示的に指定された可換 〜でない限りであると想定されます。

[§ 2 に対して練習問題](exercises/s2/)を参照してください。
