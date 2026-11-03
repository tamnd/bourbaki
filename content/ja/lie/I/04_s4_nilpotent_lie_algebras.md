---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: I
chapter_title: Lie Algebras
section: 4
section_title: Nilpotent Lie algebras
lang: ja
source: lie-i-iii
book_pages: 38-42, 91-98
pdf_pages: 0056-0060, 0109-0116
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF NILPOTENT LIE ALGEBRAS
      page: 38
      pdf_page: 56
    - "no": 2
      title: ENGEL'S THEOREM
      page: 39
      pdf_page: 57
    - "no": 3
      title: THE LARGEST NILPOTENCY IDEAL OF A REPRESENTATION
      page: 40
      pdf_page: 58
    - "no": 4
      title: THE LARGEST NILPOTENT IDEAL OF A LIE ALGEBRA
      page: 42
      pdf_page: 60
    - "no": 5
      title: EXTENSION OF THE BASE FIELD
      page: 42
      pdf_page: 60
statements: 18
exercises: 27
content_sha256: 69f956293520964dcdcaeb30b34b763130d5c94193b8d88db450225d542b2b3c
translated_from: content/en/lie/I/04_s4_nilpotent_lie_algebras.md
translation_method: google
source_content_sha256: 9f6dbd6648d7739560a7db8789c8dcacb1593afb46758c4bce763121741c6605
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-dda8bbaf
glossary_version: 34
glossary_terms_sha256: e9b539669399c6bc96000e09b00a0b16725d6c4d21c44e0c0abfc723f5cb84d4
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## § 4。 べき零リー代数

*以降、$K$ は可換体を表すことに注意してください。残りの章リー代数は、$K$ 上で有限次元であると仮定されます。*

### 1. べき零リー代数中定義

#### 定義 1 {#lie-i-s4-def-1 .statement tag=09WS}

*A Lie algebra $g$ is called nilpotent if there exists a decreasing finite sequence of ideals $(g_i)_{1 \leq i \leq p}$ of $g$ with $g_0 = g, g_p = \{0\}$, such that* $[g, g_i] \subset g_{i+1}$ *for* $0 \leq i < p$.

可換リー代数は nilpotent です。

#### 命題 1 {#lie-i-s4-prop-1 .statement tag=09WT}

※$g$をリー代数とします。 The following conditions are equivalent:*
(a) $g$ *is nilpotent;*
(b) $\mathscr{C}^k g = \{0\}$ *for sufficiently large* $k$;
(c) $\mathscr{C}_k g = g$ *for sufficiently large* $k$;
(d) *there exists an integer* $k$ *such that* $\operatorname{ad} x_1 \circ \operatorname{ad} x_2 \circ \cdots \circ \operatorname{ad} x_k = 0$ *for all elements* $x_1, x_2, \ldots, x_k$ *in* $g$;
(e) *there exists a decreasing sequence of ideals* $(g_i)_{0 \leq i \leq n}$ *of* $g$ *with* $g_0 = g, g_n = \{0\}$, *such that* $[g, g_i] \subset g_{i+1}$ *and* $\dim g_i / g_{i+1} = 1$ *for* $0 \leq i < n$.

$\mathscr{C}^k g = \{0\}$ (それぞれ $\mathscr{C}_k g = g$) の場合、明らかに数列 $\mathscr{C}^1 g, \ldots, \mathscr{C}^k g$ (それぞれ $\mathscr{C}_k g, \mathscr{C}_{k-1} g, \ldots, \mathscr{C}_0 g$) は定義 1 の特性を持ち、したがって $g$ はゼロポテントです。逆に、定義 1 の性質を持つ数列 $(g_i)_{0 \leq i \leq p}$ が存在するとします。 $n$ 上の帰納法からは、$g_i \supset \mathscr{C}^{i+1} g$ と $g_{p-i} \subset \mathscr{C}_i g$ が見えます。したがって、$\mathscr{C}^{p+1} g = \{0\}$ と $\mathscr{C}_p g = g$ です。したがって、条件 (a)、(b)、(c) が同等であることが証明されました。一方、$\mathscr{C}^1 g$ は、形の元の線形結合の集合です。

$$
[x_1, [x_2, \ldots, [x_{i-2}, [x_{i-1}, x_i]] \ldots]]
$$

ここで、$x_1, x_2, \ldots, x_i$ は $g$ まで続きます。したがって、条件 (b) と (d) は同等です。最後に、次の特性を持つ数列 $(g_i)_{0 \leq i \leq p}$ の理想が存在するとします。

Definition 1, there exists a decreasing sequence $(\mathfrak{h}_i)_{0 \leq i \leq n}$ of vector subspaces of $g$ of dimensions $n, n-1, n-2, \ldots, 0$ and a sequence of indices
$$
i_0 < i_1 < \cdots < i_p
$$
with $g_0 = \mathfrak{h}_{i_0}, g_1 = \mathfrak{h}_{i_1}, \ldots, g_p = \mathfrak{h}_{i_p}$; then as $[g, \mathfrak{h}_{i_k}] \subset \mathfrak{h}_{i_{k+1}}$ the $\mathfrak{h}_i$ are ideals and $[g, \mathfrak{h}_i] \subset \mathfrak{h}_{i+1}$ for all $i$. したがって、条件 (a) と (e) は同等です。

#### 系 1 {#lie-i-s4-prop-1-cor-1 .statement tag=09WU}

*ゼロ以外のべき零リー代数の中心はゼロではありません。*

#### 系 2 {#lie-i-s4-prop-1-cor-2 .statement tag=09WV}

*べき零リー代数の形を倒すと零になります。*
べき零リー代数のすべての $x$ と $y$ について、 $\operatorname{ad} x \circ \operatorname{ad} y$ はゼロポテントであるため、 零トレースはゼロになります。

#### 命題 2 {#lie-i-s4-prop-2 .statement tag=09WW}

*部分代数、商、代数、およびべき零リー代数の中央の拡大は無力です。 べき零リー代数の有限の積はべき零リー代数です。*
$g$を$g$のリー代数、$g'$部分代数、$\mathfrak{h}$を$g$の$g$、$\mathfrak{k} = g/\mathfrak{h}$、$\phi$標準写像を$\mathfrak{k}$にするとします。 $g$ が無能である場合、一部の整数 $k$ については $\mathscr{C}^k g = \{0\}$、したがって $\mathscr{C}^k g' \subset \mathscr{C}^k g = \{0\}$ と $\mathscr{C}^k \mathfrak{k} = \phi(\mathscr{C}^k g) = \{0\}$、したがって $g'$ と $\mathfrak{k}$ は無能です。 $\mathfrak{k}$ が無能で、$\mathfrak{h}$ が $g$ の中心に含まれる場合、一部の整数 $k$ に対して $\mathscr{C}^k \mathfrak{k} = \{0\}$、したがって $\mathscr{C}^k g \subset \mathfrak{h}$、したがって $\mathscr{C}^{k+1} g \subset [\mathfrak{h}, g] = \{0\}$ となり、$g$ は次のようになります。無能。最後に、例えば命題 1 の主張 (a) $\Leftrightarrow$ (d) から、積に関する主張が続きます。

定義 1 と命題 2 は、べき零リー代数が中心拡大の数列による可換リー代数から正確に代数として得られることを示しています。

#### 命題 3 {#lie-i-s4-prop-3 .statement tag=09WX}

*$g$ をべき零リー代数と $g$ の $\mathfrak{h}$ 部分代数を $g$ とは区別します。 $g$ の $\mathfrak{h}$ のノーマライザーは、$\mathfrak{h}$ とは異なります。*
$k$ を最大の整数として、$\mathscr{C}^k g + \mathfrak{h} \neq \mathfrak{h}$ とします。それから
$$
[\mathscr{C}^k g + \mathfrak{h}, \mathfrak{h}] \subset \mathscr{C}^{k+1} g + \mathfrak{h} \subset \mathfrak{h}
$$
したがって、$g$ 含む $\mathscr{C}^k g + \mathfrak{h}$ の $\mathfrak{h}$ のノーマライザーです。

### 2. エンゲルス定理

#### 補題 1 {#lie-i-s4-lem-1 .statement tag=09WY}

※$V$を$\mathbf{K}$の上にベクトル空間とします。 $x$ が $V$ の冪零自己準同型である場合、$\mathscr{L}(V)$ の $\mathscr{L}(V)$ への写像 $y \mapsto [x, y]$ はゼロポテントです。*
$f$がこの写像を表すとすると、$f^m(y)$は$i + j = m$と形$\pm x^i y x^j$の項の和です。 $x^k = 0$ の場合、すべての $y$ に対して $f^{2k-1}(y) = 0$ になります。

#### 定理 1 (エンゲル) {#lie-i-s4-thm-1 .statement tag=09WZ}

*$V$ を $\mathbf{K}$ 上のベクトル空間とし、$g$ を $\mathfrak{gl}(V)$ の有限次元部分代数とし、その元は $V$ の冪零自己準同型であるとします。 $V \neq \{0\}$ の場合、$V$ には $u \neq 0$ が存在し、すべての $x \in g$ に対して $x.u = 0$ になります。*

証明は、$g$ の次元 $n$ に帰納法だけ進みます。 $n = 0$なら定理は明らかです。 次元 $< n$ の代数に当てはまるとします。

$h$ を次元 $m < n$ の $g$ の嘘部分代数とします。 $x \in h$、および$\mathrm{ad}_g x$ 写像 $h$ がそれ自体に、移行の定義するが商自己準同型 $\sigma(x)$ の空間 $g/h$ の場合。 補題 1 $\mathrm{ad}_g x$ は nilpotent であるため、$\sigma(x)$ は nilpotent です。 帰納法の仮定までに、$g/h$ の非ゼロの元が存在し、すべての $\sigma(x),\ x \in h$ によって消滅します。したがって、$h$ は、$g$ の特定の $(m+1)$ 次元部分代数における理想であるということになります。

結論する ($h = \{0\}$ から始まる反復により) $g$ には次元 $n-1$ の理想的な $h$ があると考えられます。 $a \in g,\ a \notin h$ にしましょう。再び帰納法の仮定: V のすべての $x \in h$ 形がゼロ以外のベクトル部分空間 U に対して $x.u = 0$ となるような $u \in V$ を使用します。この部分空間は$a$ (§ 3, no. 5、命題 5) で安定しています。 $a$ は V の冪零自己準同型であるため、$a$ によって消滅し、したがって $g$ の元ごとに消滅する U の非ゼロ元が存在します。

#### 系 1 {#lie-i-s4-thm-1-cor-1 .statement tag=09X0}

*リー代数 g がゼロ能であるためには、すべての $x \in g$、$\mathrm{ad}\ x$ がゼロ能であることが必要かつ十分です。

条件が必要です (命題 1)。 次元 $< n$ ($n \neq 0$) のうちリー代数について十分性が証明されたとします。 $g$ を、すべての $x \in g$ に対して、$\mathrm{ad}\ x$ が零になるような $n$ 次元のリー代数とします。 定理 1 を $\mathrm{ad}\ x\ (x \in g)$ の集合に適用すると、$g$ の中心 $c$ がゼロ以外であることが証明されます。次に、$g$ は、リー代数 $g/c$ の中央の拡大であり、私たちの帰納法の仮定によって無力です。 証明は適用命題 2 までに完了します。

#### 系 2 {#lie-i-s4-thm-1-cor-2 .statement tag=09X1}

*gをリー代数、hをgのイデアルとする。 $g/h$ が nilpotent であり、すべての $x \in g$ について、$\mathrm{ad}\ x$ から h までの制限が nilpotent であると仮定します。この場合、 g はゼロポテントです。*

$x \in g$ にしましょう。 $g/h$ は零であるため、$(\mathrm{ad}\ x)^k(g) \subset h$ となるような整数 $k$ が存在します。 仮定までに、$(\mathrm{ad}\ x)^{k'}(h) = \{0\}$ となるような整数 $k'$ が存在します。したがって$(\mathrm{ad}\ x)^{k+k'}(g) = \{0\}$です。 系 2 は、系 1 の帰結になります。

#### 系 3 {#lie-i-s4-thm-1-cor-3 .statement tag=09X2}

*Vをベクトル空間とし、元がVの冪零自己準同型である$\mathfrak{gl}(V)$の有限次元部分代数とする。すると g はべき零リー代数になります。*

これは、補題 1 と系 1 の直後に続きます。

#### 例 {#lie-i-s4-n2-exa-1 .statement tag=09X3}

代数 $\mathfrak{n}(n, K)$ (§ 1, no. 2, 例 2 (3)) はゼロです。

### 3. 最大の表現の無能理想

#### 補題 2 {#lie-i-s4-lem-2 .statement tag=09X4}

* g をリー代数とし、a を g の理想とし、M を単純な g 加群とします。すべての $x \in a,\ x_M$ が無能である場合、すべての $x \in a$ に対して $x_M = 0$ になります。*

N を、すべての $x \in a$ に対して $x_M.m = 0$ となるように、$m \in M$ の M からなるの部分空間とします。 定理 1、$N \neq \{0\}$までに。一方、すべての $y \in g$ について、N は $y_M$ (§ 3, no. 5、命題 5) の下で安定です。したがって $N = M$ となり、補題が証明されます。

#### 補題 3 {#lie-i-s4-lem-3 .statement tag=09X5}

*g をリー代数、g の理想、M a g-module を有限次元以上とします*

K と $(M_i)_{0 \leq i \leq n}$ $g$ モジュール $M$ の Jordan-Hölder 系列。次の条件は同等です。

(a) for all $x \in a$, $x_M$ is nilpotent;
(b) for all $x \in a$, $x_M$ is in the Jacobson radical of the associative algebra $A$ generated by 1 and the $y_M$ where $y \in g$;
(c) for all $x \in a$,
$$
x_M(M_0) \subset M_1, x_M(M_1) \subset M_2, \ldots, x_M(M_{n-1}) \subset M_n.
$$

これら条件が満たされる場合、$g$ モジュール $M$ に関連付けられた双線形形式に関して、$a$ は $g$ と直交します。

(b) $\Rightarrow$ (a): $A$ は $K$ 上で有限次元であるため、$A$ のヤコブソン根基は冪能イデアル (*代数*、章 VIII, § 6, no. 4、定理 3) であるため、この根基のうち元は無能です。

(a) $\Rightarrow$ (c): 各 $Q_i = M_i/M_{i+1}$ ($0 \leq i < n$) は単純な $g$ モジュールです。すべての $x \in a$、自己準同型 $x_{Q_i}$ ($M_i$ と移行を商に制限することで $x_M$ から導出される) は、条件 (a) が成り立つ場合、つまり補題 2 により零が零になります。他には語、$x_M(M_i) \subset M_{i+1}$。

(c) $\Rightarrow$ (b): 条件 (c) が成立すると仮定します。 $x \in a$ と $z \in A$ としましょう。次に、$z(M_i) \subset M_i$ ($0 \leq i < n$)、したがって $(zx_M)^n(M) = \{0\}$;したがって、$Ax_M$ は $A$ の左ニリデールであり、したがって $A$ のヤコブソン根基 (*代数*、章 VIII, § 6, no. 3、系 3 ～ 定理 1) に含まれます。

最後に、条件 (a)、(b)、(c) が成り立つとします。 $x \in a$ と $y \in g$ としましょう。 $y_M x_M$ はゼロポテントであるため、$\operatorname{Tr}(y_M x_M) = 0$ となり、補題の最後の主張が証明されることがわかりました。

#### 命題 4 {#lie-i-s4-prop-4 .statement tag=09X6}

$g$ をリー代数、$M$ を $K$ 上の有限次元の $g$ 加群、$A$ を 1 と $x_M$ ($x \in g$) の集合によって生成された結合代数とします。

(a) $x_M$ がすべての $x \in a$ に対して無力であるような$g$ の理想 $a$ は、そのうちの 1 つである $n$ にすべて含まれています。

(b) イデアル$n$は$x \in g$の集合で、$A$のヤコブソン根基に対して$x_M$属するとなる。

(c) $(M_i)_{0 \leq i \leq n}$ を、$g$ モジュール $M$ の Jordan-Hölder 系列とします。この場合、$n$ も $x \in g$ の集合となり、すべての $i$ に対して $(x)_{M_i/M_{i+1}} = 0$ になります。

(d) $n$ は、$\varphi$ に関連付けられた双線形形式に関して$g$ と直交します。

$x \in g$の集合は、$A$のジェイコブソン根基に対する$x_M$属するは、明らかに$g$の理想です。 命題は、補題 3 の直後に続きます。

#### 定義 2 {#lie-i-s4-def-2 .statement tag=09X7}

命題 4 の理想 $n$ は、$g$ モジュール $M$ の最大の零位理想、または対応する表現の最大の零点理想と呼ばれます。

この表現の$n$含む核は明らかに。 $M$ が半単純 (命題 4 (c)) の場合に等しくなりますが、一般的にはそうではありません。 $x_M$ がゼロであるような $g$ の $x$ の元は、必ずしも属するから $n$ になるわけではないことに注意してください。

また、補題 3 の特定のケースでは、すぐに次の結果が得られることにも注意してください。

#### 命題 5 {#lie-i-s4-prop-5 .statement tag=09X8}

$V$ を $K$ 上の有限次元 $n$ のベクトル空間とし、$g$ を元が $V$ の冪零自己準同型である $gl(V)$ のリー部分代数とする。次に、ベクトル部分空間 $V_0, V_1, \ldots, V_n$ の $V$、次元 $n, n-1, \ldots, 0$ の減少列が存在し、すべての $x \in g$ と $i = 0, 1, \ldots, n-1$ に対して $x(V_i) \subset V_{i+1}$ が存在します。

### 4. 最大のリー代数の無能な理想

$g$をリー代数、$a$を$g$の理想とします。 $a$ が nilpotent であるためには、すべての $x \in a$、$\operatorname{ad}_g x$ が nilpotent であることが必要かつ十分です。 条件は明らかに十分であり、必要です。なぜなら、$a$ がゼロであり、$x \in a$ である場合、$\operatorname{ad}_a x$ がゼロであり、$\operatorname{ad}_g x$ 写像 $g$ が $a$ になるため、$\operatorname{ad}_g x$ はゼロであるからです。 次に、$g$ の随伴物表現に命題 4 を適用すると、次の結果が得られます。

#### 命題 6 {#lie-i-s4-prop-6 .statement tag=09X9}

$g$ をリー代数とし、$E$ を 1 と $\operatorname{ad}_g x$ ($x \in g$) によって生成された $\mathscr{L}(g)$ の結合部分代数とします。 $R$ を $E$ のジェイコブソン根基とします。
(a) $\operatorname{ad}_g y \in R$ が $g$ のゼロポテントイデアルである最大のとなるような $y \in g$ の集合 $n$。
(b) Killing 形の下で $g$ と直交します。

$g/n$ はゼロ以外の nilpotent イデアルを持つ可能性があることに注意してください。

### 5. 基礎体中拡大

$g$ を嘘$K$-代数、$K$ と $g' = g_{(K_1)}$ の$K_1$ 拡大とします。 $\mathscr{C}^k g' = (\mathscr{C}^k g)_{(K_1)}$ と同様に、$g'$ が nilpotent である場合にのみ、$g$ も nilpotent になります。

$M$ を、$K$、$n$ 最大の上の有限次元の$g$ 加群とし、$M$ と $M' = M_{(K_1)}$ に理想的とします。 $(M_i)_{0 \leq i \leq n}$ を $g$ モジュール $M$ の Jordan-Hölder 系列とします。次に、すべての $i$ とすべての $x \in n$ に対して $x_M(M_i) \subset M_{i+1}$、したがって

$$
x'_{M'}((M_i)_{(K_1)}) \subset (M_{i+1})_{(K_1)}
$$

すべての $i$ とすべての $x' \in n_{(K_1)}$ に対して。したがって、$x'_{M'}$は$x' \in n_{(K_1)}$に対して零能であるため、$n_{(K_1)}$は$M'$にとって最大のの零位理想$n'$に含まれます。ここで、*$K_1$ が $K$ 上で分離可能であれば、$n' = n_{(K_1)}$* であることがわかります。 $E$ を 1 と $x_M$ ($x \in g$) によって生成された結合 $K$-代数、$E'$ を 1 と $x_{M'}$ ($x' \in g'$) および $R$ によって生成された結合 $K$-代数とし、 $R'$ $E$ と $E'$ のジェイコブソン根基。 代数 $E'$ は正規的に $E_{(K_1)}$ と識別されます。次に、$R' = R_{(K_1)}$ (*代数*、章 VIII, § 7, no. 2、系 2 (c) ～ 命題 3)。次に、$y' \in n'$ と書きます。

$$
y' = \sum_{i=1}^n \lambda_i y_i,
$$

ここで、$y_i$ は $g$ 内にあり、$\lambda_i \in K_1$ は $K$ にわたって線形独立です。次に$y'_{M'} = \sum_{i=1}^n \lambda_i (y_i)_{M'}$と$y'_{M'} \in R' = R_{(K_1)}$。したがって、$i$すべてに対して$(y_i)_M \in R$、したがって$y_i \in n$となります。したがって、$y' \in n_{(K_1)}$、よって $n' \subset n_{(K_1)}$ となります。

特に、$K_1$ が $K$ 上で分離可能である場合、基礎体を $K$ から $K_1$ に拡張することにより、$g_{(K_1)}$ の最大の埠頭イデアルが $g$ の埠頭イデアルから導出されます。

### 練習問題 {#lie-i-s4-exercises}

§ 4 の規則は、特に記載されていない限り、引き続き有効です 〜でない限り。

[§ 4 に対して練習問題](exercises/s4/)を参照してください。
