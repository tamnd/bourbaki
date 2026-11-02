---
book: ac
book_title: Commutative Algebra
chapter: VII
chapter_title: DIVISORS
section: 2
section_title: Dedekind domains
lang: ja
source: ac-i-vii
book_pages: 493-502, 556-563
pdf_pages: 0511-0520, 0574-0581
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF DEDEKIND DOMAINS
      page: 493
      pdf_page: 511
    - "no": 2
      title: CHARACTERIZATIONS OF DEDEKIND DOMAINS
      page: 494
      pdf_page: 512
    - "no": 3
      title: DECOMPOSITION OF IDEALS INTO PRODUCTS OF PRIME IDEALS
      page: 496
      pdf_page: 514
    - "no": 4
      title: THE APPROXIMATION THEOREM FOR DEDEKIND DOMAINS
      page: 497
      pdf_page: 515
    - "no": 5
      title: THE KRULL-AKIZUKI THEOREM
      page: 499
      pdf_page: 517
statements: 15
exercises: 22
content_sha256: 33afe9b61bd89257289677efb6b57bfb9e6be137711fafdb1047ef5641680b9b
translated_from: content/en/ac/VII/02_s2_dedekind_domains.md
translation_method: google
source_content_sha256: 608c7dd934256b19a42a5a2679369ddf6b2698e699e08b46c35914c9e02a03b8
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-eeeca2ef
glossary_version: 34
glossary_terms_sha256: 8fa62d365f9448e615bc38576dc4098f9c118382610b00ef0f5278b986786fee
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## 2. デデキントのドメイン

### 1. dedekind ドメインの定義

$A$を整域とします。明らかに、次の条件は同等です。
(a) $A$ の非ゼロ素数イデアルのうち、包含に関して比較できるものは 2 つもない。
(b) $A$ の非ゼロ素数イデアルが極大である。
(c) $A$ の非ゼロ素数イデアルは高さ 1 です。

#### 定義 1 {#ac-vii-s2-def-1 .statement tag=050M}

非ゼロ素数イデアルのすべてが最大であるクルル領域は、デデキント領域と呼ばれます。

Dedekind ドメインの例
(1) すべての主イデアル整域はデデキントのドメインです。
(2) K を $\mathbf{Q}$ の有限拡大とし、A を K の $\mathbf{Z}$ の積分閉包とする。環 A はクルール領域 (§ 1, no. 8, 命題 12) である。 $\mathfrak{p}$ を A の非ゼロの素イデアルとします。その場合、$\mathfrak{p} \cap \mathbf{Z}$ は非ゼロ (章 V, § 2, no. 1、系から命題 1) であるため、$\mathbf{Z}$ の最大イデアルになります。したがって、$\mathfrak{p}$ は A の最大イデアルです (*上記引用*、命題 1)。したがって、A はデデキント領域です。一般に、A は主イデアル整域 (*代数*、章 VII, § 1、練習問題 12) ではありません。
(3) \* V をアフィン代数多様体とし、V で正則な写像の A 環とします。 A が体ではない (つまり、V が点に還元されない) と仮定します。 A がデデキント領域であるためには、V が特異点点のない既約曲線であることが必要かつ十分です。つまり、A が整域であると言うと、V は既約であることになり、というになります。 A のゼロ以外のすべての素イデアルが最大であると言うのは、A が曲線であるというというに相当します。最後に、A がネーター であるため、これがクルル領域であると言うのは、積分的に閉じているという、つまり V が正規曲線であるか、または特異点点が存在しないことになります。 \*
(4) デデキント領域の分数 $S^{-1}A$ の環 A は、$0 \notin S$ であればデデキント領域です。なぜなら、$S^{-1}A$ はクルール領域 (§ 1, no. 4、命題 6) であり、$S^{-1}A$ のすべての非ゼロ素数イデアルは、章 II, § 2, no. 5、命題 11 によって最大になります。

### 2. dedekind ドメインの特徴付け

#### 定理 1 {#ac-vii-s2-thm-1 .statement tag=050N}

A を整域とし、K を分数の体とします。次の条件は同等です。
(a) A はデデキント ドメインです。
(b) A は Krull ドメインであり、A に対してプラスである K に対する不適切でないすべての評価は、A の本質的な評価と同等です。
(c) A はクルル領域であり、A のすべての分数イデアル $\mathfrak{J} \neq (0)$ は約数です。
(d) A のすべての分数イデアル $3 \neq (0)$ は可逆です。
(e) A はネーター 積分閉領域であり、A のゼロ以外のすべての素イデアルは最大です。
(f) A はネーター であり、A の各最大イデアル m に対して、$A_m$ は体または離散評価環のいずれかになります。
(g) A はネーター で、A の各最大イデアル m に対して、$A_m$ は主イデアル整域です。

(a)と(b)の最初の同値を示します。 系 2 から定理 3、§ 1, no. 6 は、(a) が (b) を意味することを直ちに示します。逆に、(b) は (a) を意味します。なぜなら、$A$ のすべての素イデアル $p$ に対して、$A_p$ (章 VI, § 1, no. 2、系 ～ 定理) を支配する$K$ の評価環が存在するからです。 2)。

証明の残りは証明によって実行され、次のような意味が生じます。

$$
(a) \Rightarrow (c) \Rightarrow (d) \Rightarrow (e) \Rightarrow (f) \Rightarrow (g) \Rightarrow (a).
$$

$A$ がデデキント領域で、$b$ がゼロ以外の分数イデアルである場合、各極大イデアル $p$ ($§ 1$、no. 4、命題 7) に対して $bA_p = bA_p$、したがって $b = 6$ (章) II、$§ 3$、no. 3、系 3 ～ 定理 1);したがって、(a) は (c) を意味します。

ここで、(c) が (d) を意味することを示します。 (c) が成り立つ場合、写像 $a \mapsto \operatorname{div} a$ は、$I(A)$ の全単射を $D(A)$ (cf. $§ 1$, no. 1) に加えます。そのまま準同型 ($§ 1$, no. 2) であり、$D(A)$ は群であるため、$I(A)$ のすべての元は反転可能です。

(d) が (e) を意味することを示します。 (d) が成り立つ場合、$A$ のすべての整数イデアル $\neq (0)$ は有限生成されます (章 11、$§ 5$、no. 6、定理 4) ため、$A$ はネーター になります。 $I(A)$ は群、$D(A)$ は群であるため、$A$ は完全に一体的に閉じています ($§ 1$、no. 2、定理 1)。最後に、$p$ が $A$ の非ゼロ素イデアルで、$m$ が $A$ 含む $p$ の最大イデアルである場合、環 $A_{m}$ は主イデアル整域 (章) II、$§ 5$、no. 6、定理 4); $pA_m$ は素数で非ゼロなので、必然的に $pA_m = mA_m$ (主イデアル整域はデデキントドメイン) よって $p = m$ (章 11, $§ 2$, no. 5, 命題 11) となります。 $p$ が最大です。

ここで、(e) が (f) を意味することを示します。 $m$ が $A$ の最大イデアルであり、(e) が成り立つ場合、$A_{m}$ は積分閉領域ネーター であり、その最大イデアル $mA_m$ は、(0) または $A_{m}$ の唯一の非ゼロ素イデアルのいずれかになります。したがって、$A_{m}$は体、または$§ 1$、no. 7の命題11による離散評価環です。

(f) が (g) を意味するという事実は明らかです。

最後に、(g) が (a) を意味することを示します。 $A$ は $A_{m}$ の共通部分であるため、$m$ は最大理想の集合を実行します (章 II、$§ 3$、no. 3、系 4 ～ 定理) 1)、(g) は、$A$ が積分的に閉じており、ネーター であるため、$A$ がクルル領域 ($§ 1$、no. 3、系から定理 2) であることを意味します。一方、$A$ のすべての非ゼロ素数イデアルは、証明 (d) $\Rightarrow$ (e) のように最大であることがわかります。

#### 命題 1 {#ac-vii-s2-prop-1 .statement tag=050O}

*セミローカルの Dedekind ドメインは主イデアル整域です。*

$A$ を準ローカルなデデキントのドメイン、$K$ を分数の体、$p_1, \ldots, p_n$ をその最大の理想、$v_1, \ldots, v$、対応するを本質的な評価とします。これらは、$A$ の唯一の重要な評価です。 $a$ を $A$ のゼロ以外の整数理想とする。 Since it is divisorial, there exists ($§ 1$, no. 4, Proposition 5) integers $q_1, \ldots, q_n$ such that $a$ is the set of $x \in K$ such that $v_i(x) \geq q_i$ for $1 \leq i \leq n$. $x_0$ を $K$ の元とし、$1 \leq i \leq n$ に対して $v_i(x_0) = q_i$ とします (章 VI、$§ 7$、no. 2、系 1 ～ 定理 1)。 すると、$a$ は $x \in K$ の集合となり、$1 \leq i \leq n$ に対して $v_i(xx_0^{-1}) \geq 0$ になります。 したがって、$a = Ax_0$。

$A$ がデデキント領域である場合、定理 1 の証明で、A の因子の群 D(A) が分数イデアル $a \neq (0)$ の群 I(A) と同一視されることがわかります (A はネーター、ゼロ以外のすべての分数イデアルは有限に生成されます)。次に、A ($§ 1$、no. 2) の因子類群 C(A) は、A の理想類の $\neq 0$ (章 II で定義) の群と識別されます。 $§ 5$、no. 7）。

### 3. 分解の理想を積の主要な理想に

Let A be a Dedekind domain, I(A) the ordered multiplicative group of non-zero fractional ideals of A and D(A) the group of divisors of A. The isomorphism $a \mapsto \operatorname{div} a$ of I(A) onto D(A) maps the extremal divisors to the non-zero prime ideals of A ($§ 1$, no. 6, Theorem 3) and hence the multiplicative group I(A) admits as basis the set of non-zero prime ideals of A ($§ 1$, no. 3, Theorem 2). 他の語では、*A のゼロ以外のすべての分数イデアル a は、形* の一意の分解を許容します。

$$
a = \prod_p p^{n(p)}
$$

ここで、積拡大するは、A の非ゼロ素数イデアルに対して、指数 $n(p)$ は、有限の数を除いて零になります。さらに、$n(p)$ がすべて正である場合に限り、a は整数です。 関係 (1) は、a の *分解を素数因子* に変換したものと呼ばれます。特に、a が主要な理想 $Ax$ である場合、すべての $p$、$n(p) = v_p(x)$ について、$v_p$ は本質的な評価対応するから $p$ を示します。これは、$§ 1$、no. 3 の公式 (4) から続きます。させて

$$
a = \prod_p p^{m(p)}, \quad b = \prod_p p^{n(p)}
$$

A の 2 つの非ゼロの分数イデアルになります。

$$
ab = \prod_p p^{m(p) + n(p)} \tag{2}
$$
$$
a : b = ab^{-1} = \prod_p p^{m(p) - n(p)} \tag{3}
$$
$$
a + b = \prod_p p^{\inf(m(p), n(p))} \tag{4}
$$
$$
a \cap b = \prod_p p^{\sup(m(p), n(p))} \tag{5}
$$

関係 (2) は明らかです。 関係 (3) はそれから続き、方程式 $a : b = ab^{-1}$ は方程式から続きます。

$$
\operatorname{div}(a : b) = \operatorname{div} a - \operatorname{div} b
$$

($§ 1$、no. 2、系 ～ 定理 1);式 (4) と (5) は、命題 2、$§ 1$、no. 1 から続きます。

これらの結果は、特に、$\mathbf{Q}$ の有限拡大における$\mathbf{Z}$ の積分閉包に当てはまります。

$A$ が主イデアル整域の場合、上記の結果は再び代数、章 VII, § 1, no. 3 になります。

### 4. dedekind ドメインの近似値定理

デデキントの領域には、章 VI, § 7, no. 2 の定理 1 と § 1, no. 5 の命題 9 の両方を強化する「近似値定理」があります。

#### 命題 2 {#ac-vii-s2-prop-2 .statement tag=050P}

$A$ をデデキント領域、$K$ を分数の体と $A$ の非ゼロ素数イデアルの $P$ 集合とします。 $p \in P$ の場合、$v_p$ は $A$ の必須評価対応するを表します。 $p_1, \ldots, p_q$ を $P$ の元と $n_1, \ldots, n_q$ の有理数整数および $K$ の $x_1, \ldots, x_q$ 元とします。次に、$p_i$ とは異なるすべての $p \in P$ に対して $1 \leq i \leq q$ に対して $v_{p_i}(x - x_i) \geq n_i$ と $v_p(x) \geq 0$ が存在するような $x \in K$ が存在します。

置き換えることが整数より大きい$n_i$ である必要がある場合、それらはすべて正であると想定できます。まず、$x_i$ が $A$ にある場合を検討します。それは明らかに $x \in A$ 満たすの合同式を見つけることになります

$$
x \equiv x_i \pmod{p_i^{n_i}}
$$

そして、章 II, § 1, no. 2、命題 5 から $x$ の存在が続きます。

ここで一般的なケースに移ります。 $A$ の $s, y_i$ に $x_i = s^{-1} y_i$ と書くこともできます。 $x = s^{-1} y$ と書くと、$p_i$ とは異なるすべての $p \in P$ に対して、一方では $v_{p_i}(y - y_i) \geq n_i + v_{p_i}(s)$、他方では$v_p(y) \geq v_p(s)$ となるような $y \in A$ を見つけることになります。 添字 $p$ の有限の数を除いて、$v_p(s) = 0$ として、上記の場合に帰着します。 よって命題。

命題 2 は密度定理として解釈される場合があります。 正確に言うと、すべての $p \in P$ について、$\hat{K}_p$ (それぞれ $\hat{A}_p$) が離散評価 $v_p$ に関する $K$ (それぞれ $A$) の完了であるとし、積 $\prod_{p \in P} \hat{K}_p$ を考慮します。この積の元 $x = (x_p)$ は、有限の数を除くすべての $p \in P$ に対して $x_p \in \hat{A}_p$ である場合、$A$ の制限されたアデルと呼ばれます。 明らかに、制限されたアドルの集合 $A$ は、$\prod_{p \in P} \hat{K}_p$ の部分環であり、これは含む積環 $A, = \prod_{p \in P} \hat{A}_p$ です。 $A$、積位相、どちらの $A,$ が完了しているかを考えてください。 $A$ には、その加法群構造と互換性のある固有の位相 $\mathscr{T}$ があり、$A$ の 0 の近傍、形の基本的な系 $\mathscr{G}$ の近傍 0. 位相 $\mathscr{T}$ は、$A$ の環構造と互換性があります。一般位相、章 111、§ 6, no. 3 の明らかに公理 (AVII) が成り立ち、$A,$ の $\mathscr{T}$ によって誘導される位相は、$A,$ の環構造と互換性があります。 一方、すべての $x \in A$ に対して $P$ の有限部分集合 $J$ が存在し、$J' = P - J, \ K_J \leq \prod_{p \in J} \hat{K}_p, \ A_{J'} = \prod_{p \in J'} \hat{A}_p,$ と書くと x \in K_J \times A_{J'} となり、$\hat{A}_p$ がすべての p について $\hat{K}_p$ でオープンであるため、$\mathscr{G}$ は基底関数です$K_J \times A_{J'}$ の積位相の 0 の近傍の系。後者はこの積上の環構造と互換性があるため、*General 位相*、章 III、*loc の公理 (AV_1) です。 cit.* も成り立つことが見られ、これは私たちの主張を証明します。 明らかに、A は A の *開* 部分環であり、したがって A は *完全* 環 (*一般位相*、章 III, § 3, no. 3、命題 4) でもあります。

すべての $x \in K$ について、$\Delta(x)$ を元 $(x_p) \in \prod_{p \in P} \hat{K}_p$ とし、すべての $p \in P$ について $x_p = x$ とします。 p、$\Delta(x) \in A$の値の有限数を除き、$x_p \in \hat{A}_p$として。したがって、$P \neq \varnothing$ (つまり、A が体ではない場合) の場合、*単射*である準同型 $A : K \to A$ を定義しました。 $\Delta(K)$ のうち元は *主要制限アデル* と呼ばれ、明らかに $\Delta(A) \subset A$ です。

#### 命題 3 {#ac-vii-s2-prop-3 .statement tag=050Q}

*環 A, (それぞれ A ) は、近傍 & 0 の基本系と A のすべての整数理想 $\neq (0)$ が構成される環位相に関する A (それぞれ K) の完了と同一視されます。

A(またはK)で考えられる位相がハウスドルフであるのは明らかです。 A に関するno. 3, 主張を考慮すると、章 111, § 2, no. 13, 命題 17 が続きます。したがって、これは、$\Delta(A)$ が A に密であることを示します。同様に、$\Delta(K)$ が A で密であることを確認するには、すべての $x = (x_i) \in A$ に対して、$v_p(x_p) < 0$ となるような $p \in P$ の有限の数しか存在しないことに注意してください。したがって、§ 1, no. 5, 命題 9 により、すべての $p \in P$ に対して $sx_p \in \hat{A}_p$ となるような $s \in K$ があり、他の語 $\Delta(s)x \in A$ には、$\Delta(s)$ による乗法が A からそれ自体まで準同型であるため、十分です。 $\Delta(A)$ が A で密であるという事実を適用して、 $\Delta(K)$ が A で密であると推定します。

もちろん、命題 2 を使用して、$\Delta(K)$ が A で密であることを証明することもできます。

ここで、行列 $U \in \mathbf{M}_n(A)$ の乗法群 $\mathbf{SL}(n, A)$ からなるが $\det(U) = 1$ になるように考えてみましょう。 $\mathbf{M}_n(A) = A^{n^2}$ に積位相が与えられた場合、$\mathbf{SL}(n, A)$ 位相の誘導する *$\mathbf{SL}(n, A)$ の群構造* と互換性があります。 写像 $U \mapsto U^{-1}$ が $\mathbf{SL}(n, A)$ で連続していることを検証するだけで十分です。しかし、U は単モジュールであるため、$U^{-1}$ の元は U の *マイナー* であることが知られており (*代数*, 章 III, § 6, no. 5, 公式 (17))、したがって U の元の多項式になります。 主張。 K が A によって A の部分環と同一視されると、群 $\mathbf{SL}(n, K)$ は $\mathbf{SL}(n, A)$ の部分群になります。

#### 命題 4 {#ac-vii-s2-prop-4 .statement tag=050R}

*群 $\mathbf{SL}(n, K)$ は $\mathbf{SL}(n, A)$ に密集しています。*

G を $\mathbf{SL}(n, A)$ における $\mathbf{SL}(n, K)$ の閉包とします。 K は A (命題 3)、G 含むでは形 $I + a . E_{ij}$ の$i \neq j$ と $a \in A$ のすべての行列が密であるためです。すべての $p \in P$ とすべての $\lambda \in \hat{K}_p$ について、$\lambda(p)$ を制限付きアデル $x = (x_q)_{q \in P}$ とし、$x_p = \lambda$ と $x_q = 0$ が $q \neq p$ となるようにします。上記は、$i \neq j$ に対して G 含む行列 $I + \lambda(p)E_{ij}$ であることを示しています。しかし、$\lambda \in \hat{K}_p$ 生成する群 $\mathbf{SL}(n, \hat{K}_p)$ (*代数*, 章 111) に対する形 $I + \lambda E_{ij}$ の行列はわかっています。すべての行列 $U \in \mathbf{SL}(n, A)$ について、$U_p$ は $\mathbf{SL}(n, \hat{\mathbf{K}}_p)$ の $U$ の標準像を表します。したがって、すべての $p \in P$、$G$ 含む行列 $U \in \mathbf{SL}(n, A)$ については、すべての $q \# p$ について $U_q = I$ となることがわかります。 $G$ は群なので、$p \in P$ の *有限* 数を除いて、$U_p = I$ となるようなすべての行列 $U \in \mathbf{SL}(n, A)$ も含むになります。さて、$A$ の位相の定義は、これらの行列のうち集合が $\mathbf{SL}(n, A)$ に密であることをすぐに示しています。

### 5. クルール秋月定理

#### 補題 1 {#ac-vii-s2-lem-1 .statement tag=050S}

*$A$ を、すべての非ゼロプライムイデアルが最大であり、$M$ が有限に生成される捩れ $A$ 加群であるネーター 領域とします。すると、$M$ の長さ $\operatorname{long}_A(M)$ は無限になります。*

$M$ は捩れ加群であるため、$M$ に関連付けられたすべての素イデアルは $\neq (0)$ となり、したがって最大になります。 補題は、章 IV, § 2, no. 5、命題 7 から続きます。

#### 補題 2 {#ac-vii-s2-lem-2 .statement tag=050T}

*$A$を環、$T$を$A$モジュール、$(T_i)$を和集合$T$を含む$T$の部分加群の右方向ファミリーとします。次に、$\operatorname{long}_A(T) = \sup_i (\operatorname{long}_A(T_i))$.*

$i$ 全員に対して $\operatorname{long}_A(T_i) \leq \operatorname{long}_A(T)$。 整数が $\operatorname{long}_A(T_i)$ を超えなければ、補題は明らかであり、その場合、両辺は無限になります。それ以外の場合、$i_0$ を添字とし、$\operatorname{long}_A(T_{i_0})$ はその最大の値をとります。次に、家族 $(T_i)$ が指示されているため、$T_{i_0} = T$ になります。この場合、よっては私たちの主張です。

#### 注意 {#ac-vii-s2-n5-rem-1 .statement tag=050U}

この証明は、$A$ が可換であることを前提としていません。

#### 補題 3 {#ac-vii-s2-lem-3 .statement tag=050V}

*Let $A$ be a Noetherian domain such that every non-zero prime ideal $\& A$ is maximal, $M$ a torsion-free $A$-module of finite rank $r$ and a non-zero element of $A$. この場合、$A/Aa$ は有限長の $A$ モジュールであり、次のようになります:*
$$
\operatorname{long}_A(M/aM) \leq r \cdot \operatorname{long}_A(A/Aa).
$$
補題 1 は、$\operatorname{long}_A(A/Aa)$ が有限であることを示します。 まず、$M$が*有限生成*された場合の(6)を示します。 $M$ はねじれがなく、階数 $r$ であるため、$A'$ と同型である $M$ の部分加群 $L$ が存在し、$Q = M/L$ は有限生成された捩れ $A$ 加群であるため、 有限長 (補題 1)。 すべての整数 $n \geq 1$ について、標準全射 $M/a^nM \to Q/a^nQ$ の核は $(L + a^nM)/a^nM$ に等しく、$L/(a^nM \cap L)$ と同型です。として
$$
a^nL \subset a^nM \cap L,
$$
したがって
$$
\operatorname{long}_A(M/a^nM) \leq \\
\operatorname{long}_A(L/a^nL) + \operatorname{long}_A(Q/a^nQ) \leq \operatorname{long}_A(L/a^nL) + \operatorname{long}_A(Q).
$$
さて、$M$ はねじれがないので、乗法 by $a$ 定義する同型

M/aM から aA/a^2M へ。 L についても同様です。 よって、n 上の帰納法による式:

$$
\text{long}_A(M/a^nM) = n \cdot \text{long}_A(M/aM).
$$
$$
\text{long}_A(L/a^nL) = n \cdot \text{long}_A(L/aL).
$$

(7) を考慮すると、次のように推測されます。

$$
\text{long}_A(M/aM) \leq \text{long}_A(L/aL) + n^{-1}\text{long}_A(Q)
$$

すべての$n > 0$; L は A', $\text{long}_A(L/aL) = r \text{long}_A(A/Aa)$ と同型です。 (9) で $n$ を無限大にすることで、よって (6)。

ここで一般的なケースに移ります。 $(M_i)$ を M の有限生成部分加群の族とします。 加群 $T = M/aM$ は部分加群 $T_i = (M_i + aM)/aM = M_i/(M_i \cap aM)$ の和集合です。さて、T は $M_i/aM_i$ の商と同型なので、

$$
\text{long}_A(T_i) \leq r \text{long}_A(A/Aa)
$$

私たちが今証明したことによって。 よって

$$
\text{long}_A(T) \leq r \text{long}_A(A/Aa)
$$

by 補題 2.

#### 命題 5 (クルル-秋月) {#ac-vii-s2-prop-5 .statement tag=050W}

*A をそれぞれ非ゼロ素数イデアルが最大であるネーター 領域、K を分数の体、K の有限拡大である L および L 含む A の B 部分環とする。すると、B はネーター であり、すべての非ゼロ素数イデアルであるB の値が最大になります。さらに、B のすべての理想 $b \neq (0)$ に対して、B/b は有限生成A-加群です。*

b を B の非ゼロ理想とする。B/b は有限長の A-加群 (したがって、*なおさら*、有限長の B-加群) であり、b は有限生成された B-加群であることを示します。

b の非ゼロ元 y は、形の方程式を満たします。

$$
a_r y^r + a_{r-1} y^{r-1} + \cdots + a_1 = 0 \quad (a_i \in A, a_1 \neq 0).
$$

この式は $a_1 \in By \subset b$ を示します。 適用補題 3 から $M = B$ まで、$B/a_0B$ は有限長の A-加群であることがわかります。 商加群であるB/bも同様です。さらにB-加群 b 含むとして、部分加群, $a_0B$ が有限に生成されます。 $b/a_0B$ は有限長であるため ($B/a_0B$ の部分加群として)、有限生成されるため、 b は確かに有限生成される B-加群です。

上記は、まず B がネーター であることを示しています。一方、$p$ が B の非ゼロ素イデアルである場合、環 $B/p$ は整域であり、有限長であるため、体 (*代数*, 章 VIII, § 6, no. 4, 命題 9) となります。 $p$ が最大です。

#### 系 1 {#ac-vii-s2-prop-5-cor-1 .statement tag=050X}

*A のすべての素イデアル p に対して、p の上にある B の素イデアルの集合は有限です。*

Suppose first that $p = (0)$; then the only prime ideal $q$ of $B$ such that $q \cap A = (0)$ is $(0)$; otherwise, writing $S = A - \{0\}, S^{-1}q$ would be a non-zero prime ideal of $S^{-1}B$ (Chapter 11, § 2, no. 5, Proposition 11) and $S^{-1}B$ is just the field of fractions of $B$, for it is a subring of $L$ containing $K$ (\emph{Algebra}, Chapter V, § 3, no. 2, Proposition 3); whence an absurd conclusion. 現在 $p \neq (0)$ であれば、命題 5 から、$B/pB$ は体 $A/p$ を超えて有限次元ベクトル空間であることがわかり、したがって \emph{アルティン} 環となり、したがって有限の素イデアル (章) の数しかありません。 IV, § 2, no. 5, 命題 9)、これは、$B$ 含む $p$ の素イデアルのうち有限の数しか存在しないことを証明しています。

#### 系 2 {#ac-vii-s2-prop-5-cor-2 .statement tag=050Y}

*$L$ の $A$ の積分閉包はデデキント領域です。*

この積分閉包は、非ゼロ素イデアルがすべて最大である積分閉ネーター 領域です。したがって、no. 2 の定理を適用する 1 で十分です。

特に：

#### 系 3 {#ac-vii-s2-prop-5-cor-3 .statement tag=050Z}

*デデキント領域の分数の体の有限拡大における積分閉包がデデキント領域です。

#### 命題 6 {#ac-vii-s2-prop-6 .statement tag=0510}

*$A$ をデデキント領域、$K$ を分数の体、$L$ を $K$ の有限拡大、$B$ を $L$ の $A$ の積分閉包とします。 $p$ を、$A$、$v$ 対応する $K$ の本質的評価の非ゼロ素イデアルとし、*

$$
Bp = \prod_i p_i^{e(i)}
$$

*理想 $Bp$ の分解を主要理想の積として。次に:*
(a) *$p$の上にある$B$の主要な理想は、$e(i) > 0$となるような$p_i$です。*
(b) *これらの理想 $p_i$ に対する $L$ 対応するの評価 $v_i$ は、同値まで、$v$ を拡張した $L$ の評価です;*
(c) $[B/p_i : A/p] = f(v_i/v);$
(d) $e_i = e(v_i/v)$ (cf. 章 VI, § 8, no. 1、定義 1 および 2)。

(a) To say that a prime ideal $q$ of $B$ lies above $p$ amounts to saying that $q \supseteq p$, hence that $q \supseteq Bp$ and that $q$ contains one of the $p_i$ such that $e(i) > 0$ (Chapter 11, § 1, no. 1, Proposition 1).
(b) This follows, taking account of (a), from § 1, no. 8, Corollary to Proposition 12.
(c) The residue field of $v$ is identified with $A/p$ and that of $v_i$ with $B/p_i$ (§ 1, no. 4, Corollary 1 to Proposition 6).

(d) $a$ (それぞれ $a_i$) を $v$ (それぞれ $v_i$) の均一化器とします。それから
$$
a B_{p_i} = a A_p B_{p_i} = p A_p B_{p_i} = p B . B_{p_i} = \left( \prod_j p_j^{e(j)} \right) B_{p_i} = \prod_j (p_j B_{p_i})^{e(j)} \\
= (p_i B_{p_i})^{e(i)} = a_i^{e(i)} B_{p_i}
$$
$p_j B_{p_i} = B_j$ から $j \neq i$ まで。 よって (d)、$e(v_i/v) = v_i(a)$ 以降。

### 練習問題 {#ac-vii-s2-exercises}

[§ 2 に対して練習問題](exercises/s2/)を参照してください。
