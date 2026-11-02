---
book: ac
book_title: Commutative Algebra
chapter: IV
chapter_title: ASSOCIATED PRIME IDEALS AND PRIMARY DECOMPOSITION
section: 2
section_title: Primary decomposition
lang: ja
source: ac-i-vii
book_pages: 267-282, 290-301
pdf_pages: 0287-0302, 0310-0321
extraction: ocr
subsections:
    - "no": 1
      title: PRIMARY S BMODULES
      page: 267
      pdf_page: 287
    - "no": 2
      title: THE EXISTENCE OF A PRIMARY DECOMPOSITION
      page: 270
      pdf_page: 290
    - "no": 3
      title: UNIQUENESS PROPERTIES IN THE PRIMARY DECOMPOSITION
      page: 270
      pdf_page: 290
    - "no": 4
      title: THE LOCALIZATION OF A PRIMARY DECOMPOSITION
      page: 272
      pdf_page: 292
    - "no": 5
      title: RINGS AND MODULES OF FINITE LENGTH
      page: 274
      pdf_page: 294
    - "no": 6
      title: PRIMARY DECOMPOSITION AND EXTENSION OF SCALARS
      page: 279
      pdf_page: 299
statements: 39
exercises: 35
content_sha256: d89d85b71acb94f84663341c7b6857892ccd4501ded7c18db1efe71f04d8b2dd
translated_from: content/en/ac/IV/02_s2_primary_decomposition.md
translation_method: google
source_content_sha256: 412a1eb43c414ef74369ccfcd275c3769490e226305405794c9a0f41eee4ebea
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-eeeca2ef
glossary_version: 34
glossary_terms_sha256: 8b9743e2da08283cc69bb8685704648f551bf6b61fcbbbeaf34973f1d3889492
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## 2. 初等協会分解

### 1. プライマリS bモジュール

#### 命題 1 {#ac-iv-s2-prop-1 .statement tag=04KE}

$A$ をネーター 環とし、$M$ を $A$ モジュールとします。次の条件は同等です。
(a) $\operatorname{Ass}(M)$ は 1 つの元に減らされます。

(b) $M \neq 0$ と $M$ のすべてのホモテティー は単射性かほぼ無能です ($§ 1$、no. 4)。 *これらの条件が満たされ、$p$ が $a \in A$ の集合で、ホモテティー $a_M$ がほぼゼロポテントである場合、$\operatorname{Ass}(M) = \{p\}$ になります。

これは、$§ 1$、no. 4、系から命題 9 と no. 1、系 2 から命題 2 に続きます。

#### 定義 1 {#ac-iv-s2-def-1 .statement tag=04KF}

*$A$ をネーター 環、$N$ を $A$ モジュール、$N$ の $Q$ 部分加群とします。 *もし* 加群 $M = N/Q$ が命題 1 の条件を満たす場合、 $Q$ は * $N$ (または *in* $N$) に関して *p-primary と呼ばれます。

曖昧さがない場合は、単に $Q$ が「p-primary」または「primary」であると言うことにします。明らかに、$N$ 含む $Q$ のすべての部分加群 $N' \neq Q$ について、$Q$ は $N'$ の p-primary です。

定義 1 は、特に $N = A$ の場合に適用されます。 $N$の部分加群は$A$の*理想*であり、したがって、$\operatorname{Ass}(A/q)$に単一の元がある場合、または$A \neq q$とすべての場合に同じになる場合、$A$の理想$q$は*主*と呼ばれます。 環 $A/q$ の零の因子は *無能* です。 $q$ が p-primary である場合、定義 1 から、$p$ は理想値 $q$ の *根基* (章 II, $§ 2$, no. 6) であることがわかります。

#### 注意 {#ac-iv-s2-n1-rem-1 .statement tag=04KG}

$q$ を $A$ モジュール $N$ の p 一次的 部分加群とします。 $N/Q$ が *有限生成* される場合、$§ 1$, no. 4, 命題 9 により $p^k N \subset Q$ となるような整数 $k > 0$ が存在します。

*例*

#### 例 1 {#ac-iv-s2-n1-exa-1 .statement tag=04KH}

$p$ が $A$ の素イデアルである場合、$p$ は p 一次的 ($§ 1$, no. 1, 命題 1) です。

#### 例 2 {#ac-iv-s2-n1-exa-2 .statement tag=04KI}

Let $q$ be an ideal of $A$ such that there exists *a single* prime ideal $m$ (necessarily maximal) containing $q$; then, if $M$ is an $A$-module such that $qM \neq M$, $qM$ is *m-primary* with respect to $M$. $\operatorname{Ass}(M/qM)$ 含む $q$ のすべての元は、$m$ および $\operatorname{Ass}(M/qM) \neq 0$ ($§ 1$、no. 1、系 1 ～ 命題 2) に等しくなります。 特に、$q$ は、$A$ の *m-primary* イデアルです。

#### 例 3 {#ac-iv-s2-n1-exa-3 .statement tag=04KJ}

$m$ を $A$ の *最大* 理想とする。その場合、m-主イデアは、$m^n \subset q \subset m$ となるような整数 $n \geq 1$ が存在する $A$ のイデア $q$ になります。 なぜなら、$m^n \subset q \subset m$、$m$ が唯一の素イデアル含む $q$ (章 11、$§ 1$、no. 1、系から命題 1) であり、結論は *例 2* から得られます。逆に、$q$ が m-primary の場合、$m$ は $q$ の根基であるため、$m^n \subset q$ (章 II, $§ 2$, no. 6, 命題) となる $n \geq 1$ が存在します。 15）。

#### 例 4 {#ac-iv-s2-n1-exa-4 .statement tag=04KK}

*主イデアル整域* $A$ では、主な理想は $(0)$ と形 $Ap^n$ であり、$p$ は極値の元と $n \geq 1$ です。これは *例 3* の直後に続きます。

#### 例 5 {#ac-iv-s2-n1-exa-5 .statement tag=04KL}

主要イデアルの冪は、必ずしも主要イデアル (練習問題 1) であるとは限りません。一方で、素イデアル(練習問題 1)の冪ではない主イデアルも存在します。

#### 命題 2 {#ac-iv-s2-prop-2 .statement tag=04KM}

M をネーター 環 A 上の加群とし、p を A の素イデアル、$(\mathscr{Q}_i)_{i \in I}$ を M に関して p プライマリーである M の部分加群の空でない有限族とする。すると、$\bigcap_{i \in I} \mathscr{Q}_i$ は M に関して p プライマリーとなる。

$M / (\bigcap_{i \in I} \mathscr{Q}_i)$ は、直和 $\bigoplus_{i \in I} (M / \mathscr{Q}_i)$ の部分加群 $\neq 0$ と同型です。今

$$
\operatorname{Ass}\left( \bigoplus_{i \in I} (M / \mathscr{Q}_i) \right) = \bigcup_{i \in I} \operatorname{Ass}(M / \mathscr{Q}_i) = \{p\}
$$

(§ 1, no. 1、系 1 ～ 命題 3)。したがって、$\operatorname{Ass}\left(M / (\bigcap_{i \in I} \mathscr{Q}_i)\right) = \{p\}$ (§ 1, no. 1、命題 3、系 1 ～ 命題 2) となります。

#### 命題 3 {#ac-iv-s2-prop-3 .statement tag=04KN}

A をネーター 環、S を A の乗算部分集合、p を A の素イデアル、M A-加群、N 部分加群と M の $S^{-1}M$ に対する M の $i = i_A^S$ 標準写像とします。

(i) $p \cap S \neq \varnothing$ と仮定します。 N が M に関して p-primary である場合、$S^{-1}N = S^{-1}M$ です。

(ii) $p \cap S = \varnothing$ と仮定します。 N が M に関して p-primary であるためには、N が形 $i_1(N')$ であることが必要かつ十分です。ここで、$N'$ は、$S^{-1}M$ に関して $(S^{-1}p)$-primary である $S^{-1}M$ のサブ $S^{-1}A$ 加群です。次に$N' = S^{-1}N$。

(i) $p \cap S \neq \varnothing$ であり、N が M に関して p プライマリーである場合、

$$
\operatorname{Ass}_{S^{-1}A}(S^{-1}(M/N)) = \varnothing
$$

(§ 1, no. 2、系 ～ 命題 5)、したがって $S^{-1}(M/N) = 0$ (§ 1, no. 1、系 1 ～ 命題 2)、よって $S^{-1}M/S^{-1}N = 0$。

(ii) $p \cap S = \varnothing$ と仮定します。 N が M に関して p-primary である場合、$\operatorname{Ass}_{S^{-1}A}(S^{-1}(M/N)) = \{S^{-1}p\}$ (§ 1, no. 2、系 ～ 命題 5) であるため、$S^{-1}M$ の部分加群 $N' = S^{-1}N$ は $(S^{-1}p)$-primary です。さらに、$s \in S$ と $m \in M$ が $sm \in N$ である場合、$m \in N$ は、M/N の比 s を持つホモテティー に対して単射であるため、よって $N = i_1(N')$ (章 II, § 2, no. 4, 命題 10) となります。逆に、$N'$ を $S^{-1}M$ に関して $(S^{-1}p)$ 主要である $S^{-1}M$ の部分加群とします。 $N = i_1(N')$と書きましょう。次に、$N' = S^{-1}N$ (章 II, § 2, no. 4、命題 10)、$\operatorname{Ass}_{S^{-1}A}(S^{-1}(M/N)) = \operatorname{Ass}_{S^{-1}A}((S^{-1}M)/N') = \{S^{-1}p\}$ です。 標準写像 $M/N \to S(M/N)$ は単射なので、M/N に関連付けられた A の素イデアルは S (§ 1, no. 2, 命題 6) と一致しません。したがって、$\operatorname{Ass}(M/N) = \{p\}$ (§ 1, no. 2, 系 ～ 命題 5) となるため、N は M に関して p プライマリーになります。

### 2. 一次的 分解の存在

#### 定義 2 {#ac-iv-s2-def-2 .statement tag=04KO}

$A$ をネーター 環、$M$ を $A$ モジュール、$N$ 部分加群を $M$ とします。 $M$に関して主であり、$N = \bigcap_{i \in I} \mathscr{Q}_i$が$M$における$N$の主分解と呼ばれる有限族$M$の部分加群の有限族$(\mathscr{Q}_i)_{i \in I}$。

#### 例 {#ac-iv-s2-n2-exa-1 .statement tag=04KP}

整数 $n > 0$ について、$A = \mathbf{Z}$、$M = \mathbf{Z}$、$N = n\mathbf{Z}$ を考えてみましょう。 $n = p_1^{\alpha_1} \cdots p_k^{\alpha_k}$ が $n$ の分解を素数因子にすると、
$$
n\mathbf{Z} = (p_1^{\alpha_1}\mathbf{Z}) \cap \ldots \cap (p_k^{\alpha_k}\mathbf{Z})
$$
$\mathbf{Z}$ の $n\mathbf{Z}$ のプライマリ分解と no. 1 の例 4 です。

言葉の乱用により、関係 $N = \bigcap_{i \in I} \mathscr{Q}_i$ は、$M$ の $N$ の主要な分解と呼ばれます。 $\{0\} = \bigcap_{i \in I} (\mathscr{Q}_i/N)$ が $M/N$ の $\{0\}$ の主要な分解であると言うのは同じことになります。 $(\mathscr{Q}_i)_{i \in I}$ が $M$ の $N$ の主分解である場合、$M/N$ から $\bigoplus_{i \in I} (M/\mathscr{Q}_i)$ までの標準写像は単射です。 Conversely let $N$ be a submodule of $M$ and $f$ an injective homomorphism from $M/N$ to a finite direct sum $P = \bigoplus_{i \in I} P_i$, where each set $\operatorname{Ass}(P_i)$ is reduced to a single element $p_i$; let $f_i$ be the homomorphism $M/N \to P_i$ obtained by taking the composition off with the projection $P \to P_i$, and let $Q_i/N$ be the kernel off.; then the $Q_i$ distinct from $M$ are primary with respect to $M$ (no. 1, Definition 1) and $N = \bigcap_{i \in I} Q_i$. さらに、§ 1, no. 1、命題 3 のおかげで $\operatorname{Ass}(M/N) \subset \bigcup_{i \in I} \{p_i\}$ になります。

#### 定理 1 {#ac-iv-s2-thm-1 .statement tag=04KQ}

$M$ をネーター 環の有限生成加群とし、$N$ を $M$ の部分加群とします。 形の $N$ のプライマリ分解が存在します
$$
N = \bigcap_{p \in \operatorname{Ass}(M/N)} Q(p)
$$
ここで、すべての $p \in \operatorname{Ass}(M/N)$ について、$Q(p)$ は $M$ に関して $p$ 主要です。

$M/N$ によって置き換える $M$ となるため、$N = 0$ と仮定します。 § 1, no. 4、系から定理 2 までに、$\operatorname{Ass}(M)$ は有限です。 § 1, no. 1, 命題 4 により、$M$ の$p \in \operatorname{Ass}(M)$, 部分加群 $Q(p)$ に対して、$\operatorname{Ass}(M/Q(p)) = \{p\}$ と $\operatorname{Ass}(Q(p)) = \operatorname{Ass}(M) - \{p\}$ が存在します。 $P = \bigcap_{p \in \operatorname{Ass}(M)} Q(p)$ と書きましょう。すべての $p \in \operatorname{Ass}(M)$、$\operatorname{Ass}(P) \subset \operatorname{Ass}(Q(p))$、したがって $\operatorname{Ass}(P) = \varnothing$ は、$P = 0$ (§ 1, no. 1、系 1 から命題 2) を意味し、したがって定理が証明されます。

### 3. プライマリ分解の一意性プロパティ

#### 定義 3 {#ac-iv-s2-def-3 .statement tag=04KR}

$M$ をネーター 環と $M$ の $N$ 部分加群を超える加群とします。 $M$ の $N$ の主要な分解 $N = \bigcap_{i \in I} Q_i$ は、次の条件が満たされる場合、reduced と呼ばれます。

(a) *添字* $i \in I$ *そのような* $\bigcap_{j \neq i} Q_j \subset Q_i;$ は存在しません

(b) *if* $\operatorname{Ass}(M/Q_i) = \{p_i\}$、*the* $p_i$ (*i* $\in I$) *は別個です*。

$M$ の $N$ のすべての主分解 $N = \bigcap_{i \in I} Q_i$ から、$N$ の $M$ の *縮小された主分解は次のように推定できます。 $J$ を最小の元の集合とします。 部分集合 $I'$/$I$ は $N = \bigcap_{i \in I'} Q_i$ になります。明らかに $(Q_i)_{i \in J}$ は条件 (a) を満たします。次に、$\Phi$ を $i \in J$ の $p_i$ の集合とします。すべての $p \in \Phi$ について、$H(p)$ を $i \in J$ の集合とし、$p_i = p$ とし、$Q(p) = \bigcap_{i \in H(p)} Q_i$ とします。 no. 1 の命題 2 から、$Q(p)$ は $M$ に関して $p$ 主要であることがわかります。さらに $N = \bigcap_{p \in \Phi} Q(p)$ であり、家族 $Q((p))_{p \in \Phi}$ は、$M$ の $N$ の縮小プライマリー 分解です。

no. 2 の定理 1 の証明で定義されたプライマリ分解が *縮小* されていることがわかります。これは次の命題から導き出されます。

#### 命題 4 {#ac-iv-s2-prop-4 .statement tag=04KS}

*Let* $M$ *be a module over a Noetherian ring, N a submodule of M, $N = \bigcap_{i \in I} Q_i$ *a primary decomposition of N in M and, for all* $i \in I$, *let* $\{p_i\} = \operatorname{Ass}(M/Q_i)$. *この分解を削減するには、* $p_i$ * が区別され、 属するが * $\operatorname{Ass}(M/N)$ になることが必要かつ十分です。 *それから*

(2)
$$
\operatorname{Ass}(M/N) = \bigcup_{i \in I} \{p_i\}
$$

(3)
$$
\operatorname{Ass}(Q_i/N) = \bigcup_{j \neq i} \{p_j\} \quad \text{for all } i \in I.
$$

主張の条件が満たされる場合、$N = \bigcap_{j \neq i} Q_j$ できないが成り立ちます。なぜなら、仮定に反して、$\operatorname{Ass}(M/N) \subset \bigcup_{j \neq i} \{p_j\}$ (§ 1, no. 1、系 2 ～ 命題 3) が推測されるからです。 $N$ の主要な分解 $(Q_i)_{i \in I}$ は確実に減少します。逆に、$\operatorname{Ass}(M/N) \subset \bigcup_{i \in I} \{p_i\}$ は常に成り立ちます (§ 1, no. 1、系 2 ～ 命題 3)。一方、すべての $i \in I$ について、$P_i = \bigcap_j Q_j$ と書きましょう。次に、$P_i \cap Q_i = N$ と $P_i \neq N$ $(Q_i)_{i \in I}$ が減算されると、$P_i/N$ はゼロではなく、$M/Q_i$、よって $\{p_i\} = \operatorname{Ass}(P_i/N)$ (§ 1, no. 1、命題) の部分加群 $(P_i + Q_i)/Q_i$ と同型です。 3 および系 1 ～ 命題 2); $P_i/N \subset M/N, p_i \in \operatorname{Ass}(M/N)$として、主張と公式における条件の必然性の証明が完成します。最後に、$N = \bigcap_{j \neq i} (Q_j \cap Q_i), \operatorname{Ass}(Q_i/N) \subset \bigcup_{j \neq i} \operatorname{Ass}(Q_i/(Q_j \cap Q_i))$ (§ 1, no. 1、系 2 から命題 3) となります。しかし、$Q_i/(Q_j \cap Q_i)$ は $M/Q_j$ の部分加群 $(Q_i + Q_j)/Q_j$ と同型なので、$\operatorname{Ass}(Q_i/(Q_j \cap Q_i)) \subset \{p_j\}$ となります。
$$
\operatorname{Ass}(Q_i/N) \subset \bigcup_{j \neq i} \{p_j\};
$$

#### 系 {#ac-iv-s2-n3-cor-1 .statement tag=04KT}

Let $A$ be a Noetherian ring, $M$ an $A$-module, $N$ a submodule of $M$ and $(Q_i)_{i \in I}$ a primary decomposition of $N$ in $M$. 次に、$\mathrm{Card}(I) \geq \mathrm{Card}(\mathrm{Ass}(M/N))$; $(Q_i)_{i \in I}$ が縮小プライマリー 分解であるためには、$\mathrm{Card}(I) = \mathrm{Card}(\mathrm{Ass}(M/N))$ が必要かつ十分です。

命題 4 に先行する注意から、$M$ には $\mathrm{Card}(J) \leq \mathrm{Card}(I)$ のような $N$ の縮小された主要な分解 $(R_j)_{j \in J}$ が存在することがわかります。最初の主張が 2 番目の後に続き、後者は命題 4 の帰結です。

#### 命題 5 {#ac-iv-s2-prop-5 .statement tag=04KU}

Let $A$ be a Noetherian ring, $M$ an $A$-module, $N$ a submodule of $M$, $N = \bigcap_{i \in I} Q_i$ a reduced primary decomposition of $N$ in $M$ and, for all $i \in I$, let $\{p_i\} = \mathrm{Ass}(M/Q_i)$. $p_i$ が $\mathrm{Ass}(M/N)$ の最小値元である場合、$Q_i$ は、$p_i$ (章 11, § 2, no. 4) (cf. 練習問題 2) に関する$N$ の彩度に等しくなります。

明らかに、$N = 0$、必要に応じて置き換えることが $M$ x $M/N$ になる場合に注意を限定することができます。 $\mathrm{Ass}(M)$ で $p_i$ が最小の場合、$A - p_i$ 簡約する ～ $p_i$ を満たさない $\mathrm{Ass}(M)$ の元のうち集合です。 命題は、上記の公式 (3) と標準写像 $M \to M_0$ の § 1, no. 2、命題 6、核から続き、$p_i$ (章 11、 § 2, no. 4）。

#### 注意 {#ac-iv-s2-n3-rem-1 .statement tag=04KV}

この集合の極小元ではない素イデアル $p_i \in \mathrm{Ass}(M/N)$ は、$M/N$ に関連付けられた *埋没* 素イデアルと呼ばれるときどきです。 $M/N$ が有限生成される場合、$p_0 \in \mathrm{Ass}(M/N)$ が浸されるためには、$V(p_0)$ が $\mathrm{Supp}(M/N)$ (章 II, § 4, no. 3、系 2 から命題 14) の既約成分ではないことが必要かつ十分です。 $(Q(p))_{p \in \mathrm{Ass}(M/N)}$ と $(Q'(p))_{p \in \mathrm{Ass}(M/N)}$ が $M$ の $N$ の 2 つの還元された主要な分解である場合、$Q'(p_0) \neq Q(p_0)$ (練習問題 24 (c)) となる可能性があります。 $M$ の $N$ の *正規* 縮小プライマリー 分解は、その中に現れるプライマリー 部分加群に補足的な条件を課すことによって常に定義できます (練習問題 4)。

### 4. 一次的 分解の位置特定

Given a submodule $N$ of a module $M$ over a Noetherian ring $A$, to simplify we shall denote by $D_I(M/N)$, in this no., the set of reduced primary decompositions of $N$ in $M$ whose indexing set is $I$ (equipotent to $\mathrm{Ass}(M/N)$).

#### 命題 6 {#ac-iv-s2-prop-6 .statement tag=04KW}

$A$ をネーター 環、$M$ を $A$ モジュール、$M$ と $I = \mathrm{Ass}(M/N)$ の $N$ 部分加群とします。 $S$ を $A$ と $J$ 部分集合の $I$ からなるの添字の乗算部分集合を$S \cap p_i = \varnothing$ とします。 $M$の$S$に対する$N$の彩度を$N'$とします。 それから：

(i) *もし* $(Q_i)_{i \in I}$ *が* $D_I(M/N)$の元である場合、*家族* $(Q_i)_{i \in J}$ *は* $D_J(M/N')$の元であり、家族* $(S^{-1}Q_i)_{i \in J}$ *は* $D_J(S^{-1}M/S^{-1}N)$の元である。

(ii) *写像* $(Q_i)_{i \in J} \to (S^{-1}Q_i)_{i \in J}$ *は* $D_J(M/N')$ *の上* $D_J(S^{-1}M/S^{-1}N)$の全単射です。

(iii) *If* $(Q_i)_{i \in J}$ *is an element of* $D_J(M/N')$ *and* $(R_i)_{i \in I}$ *an element of* $D_I(M/N)$, *the family* $(T_i)_{i \in I}$ *such that* $T_i = Q_i$ *for* $i \in J$ *and* $T_i = R_i$ *for* $i \in I - J$ *is an element of* $D_I(M/N)$.

(i) $i \in J, S^{-1}Q_i$ は $S^{-1}p_i$ にとって主要であり、$i \in I - J, S^{-1}Q_i = S^{-1}M$ については主要であることがわかります (no. 1、命題 3)。 $S^{-1}N = \bigcap S^{-1}Q_i$ (章 II, § 2, no. 4) の場合は、$S^{-1}N = \bigcap_{i \in J} S^{-1}Q_i$ も同様です。 $i \in J$ の $S^{-1}p_i$ は個別であり、その集合は $\operatorname{Ass}(S^{-1}M/S^{-1}N)$ ($§ 1$、no. 2、系から命題 5) です。この場合、(命題 4) $(S^{-1}Q_i)_{i \in J}$ は、$S^{-1}N$ の縮小された主要な分解です。さらに、$Q_i = (i_M^S)^{-1}(S^{-1}Q_i)$ (no. 1 命題 3) であるため、$N' = (i_M^S)^{-1}(S^{-1}N) = \bigcap_{i \in J} Q_i$ と $(Q_i)_{i \in J}$ は明らかに $M$ の $N'$ の縮小プライマリー 分解です。

(ii) *$S^{-1}N' = S^{-1}N$ として、$N'$ によって置き換える $N$ になる可能性があります。つまり、$J = I$ と仮定します。 $(P_i)_{i \in I}$ を $S^{-1}M$ の $S^{-1}N$ の縮小された主要な分解とし、$Q_i = (i_M^S)^{-1}(P_i)$ と書きましょう。 no. 1, 命題 3 から、$Q_i$ は $p_i$ ($i \in I$) の主であり、$(Q_i)_{i \in I}$ は、no. 3 により $M$ の $N$ の縮小主分解になります。 系から命題 4. 最後に、すべての $i \in I$ とすべての部分加群 $Q'_i$ について、$M$ は、no. 1、命題のおかげで、$M, Q'_i = (i_M^S)^{-1}(S^{-1}Q'_i)$ に関して$p_i$-primary になります。と仮定 $J = I$ では、2 つの写像 $D_I(M/N) \to D_I(S^{-1}M/S^{-1}N)$ と $D_I(S^{-1}M/S^{-1}N) \to D_I(M/N)$ が定義されており、その合成が $D_I(M/N)$ と $D_I(S^{-1}M/S^{-1}N)$ 上の同一性であることがわかり、これは (ii) を証明します。

(iii) (i) により、$N' = \bigcap_{i \in J} R_i$、よって

$$
N = N' \cap \bigcap_{i \in I - J} R_i = \left( \bigcap_{i \in J} Q_i \right) \cap \left( \bigcap_{i \in I - J} R_i \right)
$$

そして、no. 3、系から命題 4 に続いて、この主要な分解が減少します。

#### 系 {#ac-iv-s2-n4-cor-1 .statement tag=04KX}

*写像*

$$
D_I(M/N) \to D_J(M/N') \quad \text{and} \quad D_I(M/N) \to D_J(S^{-1}M/S^{-1}N)
$$

*命題 6 (i) で定義* *全射法です*。

命題 6 (iii) は、写像 $D_I(M/N) \to D_J(M/N')$ が全射であることを示し、命題 6 (ii) は、写像を示します。
$$
D_I(M/N) \to D_J(S^{-1}M/S^{-1}N)
$$
全主観的です。

### 5. 環と加群の有限長

$A$ モジュール $M$ が有限長である場合、この長さを $\operatorname{long}_A(M)$ または $\operatorname{long}(M)$ で表します。すべてのアルティン環はネーター (代数、章 VIII, § 6, no. 5、系 3 ～ 命題 12) であり、アルティン環上のすべての有限生成加群は有限長であることを思い出してください。前掲*、系 1 ～ 命題 12)。さらに、すべてのアルティン整域は体 (代数、章 VIII, § 6, no. 4、命題 9) です。

#### 命題 7 {#ac-iv-s2-prop-7 .statement tag=04KY}

*$M$ をネーター 環 $A$ よりも有限生成加群とします。次のプロパティは同等です:*
(a) $M$ は有限長のものです。
(b) *すべての理想 $p \in \operatorname{Ass}(M)$ は、$A$ の最大の理想です。*
(c) *すべての理想 $p \in \operatorname{Supp}(M)$ は、$A$ の最大の理想です。*

$(M_i)_{0 \leq i \leq n}$ を $M$ の組成列とし、$0 \leq i \leq n - 1$ に対して、$M_i/M_{i+1}$ は $A/p_i$ と同型であり、$p_i$ は素数 ($§ 1$, no. 4, 定理 1) です。 $M$ が有限長である場合、各 $A$ モジュール $A/p_i$ も同様です。これは、環 $A/p_i$ のそれぞれがアルティンであることを意味します。しかし、$A/p_i$ は整域であるため、体となり、他の場合には語 $p_i$ が最大になります。私たちは結論する、(a) は (b) を意味します ($§ 1$, no. 4, 定理 2)。 条件 (b) は、$§ 1$、no. 3、命題 7 によって (c) を暗示します。最後に、$\operatorname{Supp}(M)$ のすべての理想が最大である場合、$p_i$ ($§ 1$、no. 4、定理 2)、したがって、$A/p_i$ は単純な $A$ モジュールであり、$M$ は有限長であり、証明が完成します。

#### 系 1 {#ac-iv-s2-prop-7-cor-1 .statement tag=04KZ}

*ネーター を超える有限長 $M$ の加群ごとに、$A$、$\operatorname{Ass}(M) = \operatorname{Supp}(M)$ が加算されます。*

$\operatorname{Supp}(M)$ のすべての元は $\operatorname{Supp}(M)$ で最小となり、$§ 1$、no. 3、系 1 から命題 7 まで結論が続きます。

#### 系 2 {#ac-iv-s2-prop-7-cor-2 .statement tag=04L0}

*$M$ をネーター 環 $A$ および $p$ を$A$ の主要な理想である有限生成加群とします。 $M_p$ が有限長の非ゼロ加群 $A_p$ であるためには、$p$ が $\operatorname{Ass}(M)$ の最小値元であることが必要かつ十分です。

$§ 1$、no. 2、系から命題5まで、$\operatorname{Ass}_{A_p}(M_p)$は$q_p$の理想の集合であり、$q$は$p$に含まれる$\operatorname{Ass}(M)$の理想の集合を貫いています。 一方、$p_p$ は、$A_p$ の独自の最大理想です。 命題 7 により、$M_p$ が有限長の $A_p$ モジュールであるためには、$\operatorname{Ass}(M)$ の元が厳密に $p$ に含まれないことが必要かつ十分です。 On the other hand, for $M_p \neq 0$, it is necessary and sufficient by definition that $p \in \operatorname{Supp}(M)$ (Chapter 11, § 4, no. 4), that is that $p$ contain an element of $\operatorname{Ass}(M)$ ($§ 1$, no. 3, Proposition 7). これは系を証明します。

#### 注意 (1) {#ac-iv-s2-n5-rem-1 .statement tag=04L1}

$M$ をネーター 環 $A$ よりも有限生成加群とします。 $(M_1), \ldots$ を $M$ の組成列とし、$0 \leq i \leq n - 1$ に対して、$M_i / M_{i+1}$ が $A/p_i$ と同型となるようにします。ここで、$p_i$ は $A$ ($§ 1$、no. 4、定理 1) の素イデアルです。 $p$ が $\operatorname{Ass}(M)$ の最小値元である場合、長さ $\operatorname{long}_{A_p}(M_p)$ は、$p_i = p$ となる添字* $i$ の *数に等しくなります。 $M$ の $(M_i)_p$ 形組成列について、$(M_i)_p / (M_{i+1})_p$ は $(A/p_i)_p$ と同型であるため、$p_i \neq p$ であれば $\{0\}$ と同型です ($p$ は集合で最小であるため) $p_i$ by $§ 1$、no. 4、定理 2) $p_i = p$ の場合、体である $(A/p)_p$ まで。

#### 命題 8 {#ac-iv-s2-prop-8 .statement tag=04L2}

*$M$ をネーター 環 $A$ 上の有限長の加群とします。*

(i) *$\operatorname{Ass}(M)$ によってインデックス付けされた $M$ に関して、$\{0\}$ のプライマリ分解が 1 つだけ存在します (必要に応じて削減されます) — $\{0\} = \bigcap_{p \in \operatorname{Ass}(M)} Q(p)$ をこの分解とします。ここで、$Q(p)$ は、$p$ に関してプライマリです。 $M$.*

(ii) *すべての $n \geq n_0$ とすべての $p \in \operatorname{Ass}(M)$、$Q(p) = p^n M$ となるような整数 $n_0$ が存在します。*

(iii) *すべての$p \in \operatorname{Ass}(M)$、$M$から$M_p$の標準写像は全射であり、その核は$Q(p)$です。

(iv) *$M$ の $\bigoplus_{p \in \operatorname{Ass}(M)} (M/Q(p))$ への標準単射は全単射です。*

$\operatorname{Ass}(M)$ (命題 7) ではすべての元 $p \in \operatorname{Ass}(M)$ が最小であるため、no. 3、命題 5 から主張 (i) が続きます。 $M$ は有限に生成されるため、すべてに対して $p^n M \subset Q(p)$ となるような $n_0$ が存在します。 $p \in \operatorname{Ass}(M)$ とすべての $n \geq n_0$ (no. 1、*注意*);しかし、$p$ は最大理想であるため、$p^n M$ は $M$ (no. 1、*例 2 および 3*) に関して $p$ 主要であり、$\bigcap_{p \in \operatorname{Ass}(M)} p^n M = \{0\}$ と同様に、(i) から必然的にすべてに対して $p^n M = Q(p)$ が得られます。 $p \in \operatorname{Ass}(M)$; よって (ii)。 $p \in \operatorname{Ass}(M)$ に対する $p^n$ は対 (章 11, § 1, no. 2, 命題 3) で相対的に素であるため、標準写像 $M \to \bigoplus_{p \in \operatorname{Ass}(M)} (M/p^n M)$ は全射です (章 11, § 1, no. 2、命題 6)、よって (iv)。次に、$\operatorname{Ass}(Q(p)) = \operatorname{Ass}(M) - \{p\}$ と $\operatorname{Ass}(M/Q(p)) = \{p\}$ (no. 3、命題 4)。 $\operatorname{Ass}(M)$ の元が最大の理想であるため、$\operatorname{Ass}(M)$ のうち $A - p$ を満たさない唯一の元が、$p$ です。したがって、$Q(p)$ は、標準写像 $j : M \to M_p$ の核 ($§ 1$、no. 2、命題 6) です。 $s \in A - p$ の場合、比 $s$ を持つ $M/Q(p)$ のホモテティー は、関係 $\operatorname{Ass}(M/Q(p)) = \{p\}$ (no. 1, 命題 1) により単射的です。 $M/Q(p)$ はアルティンなので、このホモテティー は全単射です (*代数*, 章 VIII, § 1, no. 2, 補題 3)。 標準写像 $M \to M/Q(p)$ は $f \circ j$ と書かれます。ここで、$f : M_p \to M/Q(p)$ は $A$ 準同型写像 (章 II, § 2, no. 2, 命題 3) です。 $\operatorname{Ker}(j) = \operatorname{Ker}(f \circ j) = Q(p)$、$f$ は単射です。私たちは結論する、$j$は全射であり、$f$は全単射です。

#### 系 {#ac-iv-s2-n5-cor-1 .statement tag=04L3}

*M がネーター 環 A 以上の有限長の加群である場合、*

$$
\operatorname{long}_A(M) = \sum_{p \in \operatorname{Ass}(M)} \operatorname{long}_{A_p}(M_p).
$$

これを証明すると、命題 8 (iv) から導かれます。

$$
\operatorname{long}_A(M/\mathscr{Q}(p)) = \operatorname{long}_{A_p}(M_p).
$$

さて、no. 1 の命題 1 から、$M/\mathscr{Q}(p)$ の比率 s を持つすべての $s \in A - p$ ホモテティー は単射であることがわかります。したがって、$M/\mathscr{Q}(p)$ の R が部分加群ごとに比 s であるホモテティー は単射であり、R がアルティンであるため、全単射です (*代数*, 章 VIII, § 2, no. 2, 補題 3)。私たちは結論する、$M/\mathscr{Q}(p)$のサブAモジュールはMのサブAモジュールの全単射$f : M, \to M/\mathscr{Q}(p)$の下にある像、(章11、§ 2, no. 3)、よって私たちの主張です。

#### 命題 9 {#ac-iv-s2-prop-9 .statement tag=04L4}

*A をネーター 環とします。次の条件は同等です:*
(a) *はアルティンです*。
(b) *A のすべての素イデアル $\mathfrak{a}$ は極大イデアルです。*
(c) *Ass(A) のすべての元は最大の理想です。*

*これらの条件が満たされる場合、A は有限の数の素イデアルのみを持ち、それらはすべて最大であり、A-加群 A に関連付けられます。さらに、A は半局所環であり、その Jacobson 根基はゼロポテントです。

A がアルティンであるということは、A が有限長の A-加群であるというというと同等です。したがって、(a) と (c) は命題 7 によって等価です。明らかに (b) は (c) を意味します。最後に、すべてのアルティン整域は体であるため、(a) は (b) を意味します。したがって、特性 (a)、(b)、および (c) は同等です。

彼らが保持していると仮定してください。 Supp(A) に対する属するのすべての素イデアル、および Supp(A) のすべての元含む元 Ass(A) ($\S$ 1、no. 3、命題 7) から、(c) から、Ass(A) はすべての素イデアルの集合であることがわかります。 A;この場合、A には有限の数個の素イデアルのみがあり、それらはすべて最大であり、A-加群 A に関連付けられています。これは明らかに A が準局所的であることを意味します。最後に、アルティン環のジェイコブソン根基が無能であることがわかります (*代数*、章 VIII, § 6, no. 4、定理 3)。

#### 注意 (2) {#ac-iv-s2-n5-rem-2 .statement tag=04L5}

The conditions of Proposition 9 for a *Noetherian* ring A imply that the spectrum of A is *finite* and *discrete*, every point of Spec(A) being therefore closed (Chapter 11, § 4, no. 3, Corollary 6 to Proposition 11). 逆に、*ネーター* 環 A の場合、Spec(A) の *すべての点* $\mathfrak{a}$ が *閉じている* ということは、A のすべての素イデアルが最大 (*loc. cit.*.) であることを意味し、したがって、この条件は命題 9 のそれと等価です。

#### 系 1 {#ac-iv-s2-prop-9-cor-1 .statement tag=04L6}

*すべてのアルティン環 A は、アルティン局所環の有限族の直接合成と同型です。*

命題 9 と命題 8 (iii) と (iv) から、$(\mathfrak{m}_i)_{1 \leq i \leq n}$ が $A$ の最大イデアルの族である場合、標準写像 $A \to \prod_i A_{\mathfrak{m}_i}$ は全単射であることがわかります。

#### 注意 (3) {#ac-iv-s2-n5-rem-3 .statement tag=04L7}

この系は、$\operatorname{Spec}(A)$ が有限で離散的であること、および章 11、§ 4, no. 3、命題 15 であるという事実からも推定できます。

#### 系 2 {#ac-iv-s2-prop-9-cor-2 .statement tag=04L8}

$A$ をネーター 環とし、$m$ を $A$ の理想とします。次の条件は同等です。

(a) $A$ は半局所リングであり、$m$ は $A$ の定義的な理想です。
(b) $A$ は $m$ 進数位相を持つザリスキー 環で、$A/m$ はアルティンです。

(a) が成り立つ場合、$A$ は $m$ 進数位相 (章 III, § 3, no. 3, 例 3) を持つザリスキー 環です。さらに、ジェイコブソンの仮定 $m$ 含む冪 $A$ の根基 $r$ のように、$A$ のすべての素理想は含む $m$ も含む $r$ (章 II, § 1, no. 1, 命題 1);したがって、$r$ は最大イデアルの有限共通部分であるため、これは最大です (\emph{loc. cit.})。 命題 9 は、$A/m$ がアルティンであることを示します。逆に、(b) が成り立つ場合、$A$ 含むのすべての最大イデアル $p$ は、$A$ のジェイコブソン根基、したがって含む $m$ (章 III, § 3, no. 3, 命題) 6); $A/m$ がアルティンであるため、イデアル $p/m$ は数 (命題 9) で有限であるため、$A$ の最大イデアルは有限の数のみであり、これは半局所的であることを意味します。

#### 系 3 {#ac-iv-s2-prop-9-cor-3 .statement tag=04L9}

$A, A'$を$A$から$A'$までの環と$h$準同型の2つとします。 $A$ がセミローカルであり、ネーター であり、$A'$ が有限生成された $A$ モジュールであると仮定します。次に、環 $A'$ は準ローカルで、ネーター です。 $m$ が $A$ の決定的な理想である場合、$mA'$ は $A'$ の決定的な理想です。

$A'$ は、$mA'$ 進数位相 (章 III, § 3, no. 3, 命題 7) を持つザリスキー 環であることがわかります。 $A/m$ はアルティン (系 2) であり、$A'/mA'$ は有限生成された $(A/m)$ モジュールであるため、$A'/mA'$ はアルティン環であるため、$A'$ は準ローカルであり、$mA'$ は定義的な理想です$A'$ (系 2)。

#### 系 4 {#ac-iv-s2-prop-9-cor-4 .statement tag=04LA}

$A$ を完全な半局所的なネーター 環、$m$ を定義する理想的な $A$、$E$ を有限生成された $A$ モジュール、および $(F_n)$ 減少列とします。 $E$ の部分加群は $\bigcap_n F_n = 0$ になります。すると、すべての $p > 0$ に対して、 $F_n \subset m^p E$ となるような $n > 0$ が存在します。

$A$ はザリスキー 環であるため、$E$ はハウスドルフであり、$F_n$ は $m$ 進数位相の下で閉じられます。一方、$E$は完了です（章III, § 2, no. 12、系1～命題16）。最後に、$E/m^p E$ は環 $A/m^p$ を超える有限生成加群であり、アルティン (系 2) です。この場合、$E/m^p E$ はアルティン $(A/m^p)$ モジュール、つまりアルティン $A$ モジュールです。 系は、章 III, § 2, no. 7、命題 8 から続きます。

#### 系 5 {#ac-iv-s2-prop-9-cor-5 .statement tag=04LB}

完全な半ローカルネーター 環では、共通部分が 0 であるすべての減少列 $\phi$ 理想は、0 に収束するフィルター 基底です。

系を適用する 4 から A-加群 $\mathbf{A}$ までで十分です。

#### 命題 10 {#ac-iv-s2-prop-10 .statement tag=04LC}

$A$ をネーター 環と $p_1, \ldots, p_n$ を、A-加群 $A$ に関連付けられた主要な理想とし、$p_i \neq p_j$ を $i \neq j$ とします。

(i) 集合 $S = \bigcap_{i=1}^n (A - p_i)$ は、$A$ の 0 の因子ではない元の集合です。

(ii) すべての$p_i$ が$\operatorname{Ass}(A)$ の最小元である場合、$A$ 分数 $S^{-1}A$ の合計環はアルティンです。

(iii) 環 $A$ が減少すると、すべての $p_i$ は $\operatorname{Ass}(A)$ の最小元 (したがって、$\operatorname{Spec}(A)$ の最小元) となり、それぞれの $A_{p_i}$ は体になります。それぞれの添字 $i$、標準準同型 $S^{-1}A \to A_{p_i}$ (章 II, § 2, no. 1、系 1 ～ 命題 2) は全射であり、その核は $S^{-1}p_i$ です。最後に$S^{-1}A$から$\prod_{i=1}^n (S^{-1}A/S^{-1}p_i)$までの標準準同型は全単射です。

$S$が$\mathbf{A}$の0の因子ではなく、元の集合であるという事実はすでに見られています（§ 1, no. 1、系3から命題2）。 $S^{-1}A$ の主イデアルは形 $S^{-1}p$ です。ここで、$p$ は、$p_i$ のいずれかに含まれる $\bigcup_{i=1}^n p_i$ (章 11、§ 2, no. 5、命題 10) に含まれる $A$ の主イデアルです。 (章 II, § 1, no. 1、命題 2)。 $p_i$ が $\operatorname{Ass}(A)$ の最小値元である場合、それは $\operatorname{Spec}(A)$ の最小値元 (§ 1, no. 3、系 ～ 命題 7) です。それぞれの $p_i$ が $\operatorname{Ass}(A)$ の最小元である場合、$S^{-1}A$ の主イデアルは $S^{-1}p_i$ であり、したがってそれらはすべて最大であることがわかり、$S^{-1}A$ がアルティン (命題 9) であることが証明されます。

最終的に環 $A$ が減少したとします。次に$\bigcap_{i=1}^n p_i = \{0\}$ (§ 1, no. 3、系 2 ～ 命題 7)。 $\{0\} = \bigcap_{i=1}^n p_i$ は、理想的な $\{0\}$ (no. 3、系から命題 4) の * 縮小された * 主要な分解であると推定します。特に、$p_i$ はどれも添字 $j \neq i$ の $p_j$ を含むできないため、$p_i$ はすべて $\operatorname{Ass}(A)$ の最小の元になります。 環 $S^{-1}A$ は (ii) によりアルティンになります。 $S^{-1}p_i$ は、$S^{-1}A$ モジュール $S^{-1}A$ (§ 1, no. 2、系 ～ 命題 5) および $\{0\} = S^{-1} \left( \bigcap_{i=1}^n p_i \right) = \bigcap_{i=1}^n S^{-1}p_i$ (章 II, § 2, no. 4) に関連付けられた主要なイデアルです。 $S^{-1}p_i$ は別個であるため、$(S^{-1}p_i)_{1 \leq i \leq n}$ は、$S^{-1}A$ (no. 3、系から命題 4) の $\{0\}$ の縮小された主要な分解です。 命題 8 は、正準準同型写像が次のとおりであることを示します。 $S^{-1}A \to (S^{-1}A)_{p_i}$ は全射であり、 核 $S^{-1}p_i$ と標準準同型 $S^{-1}A \to \prod_{i=1}^n (S^{-1}A/S^{-1}p_i)$ は全単射です。さらに、標準準同型 $S^{-1}A \to A$ は g と同型 $(S^{-1}A)_{S^{-1}p_i} \to A$ (章 II, § 2, no. 3, 命題 7) で構成されていることがわかります。最後に、命題 8 から、$S^{-1}p_i$ が最大イデアルであるため、$(S^{-1}A)_{S^{-1}p_i}$ は $S^{-1}A/S^{-1}p_i$ と同型であり、したがって体になります。

### 6. スカラーの主分解と拡大

この番号では、A と B は 2 つの環を表し、$B$ を A-代数にする環準同型 $\rho : A \to B$ を考えます。すべての B-加群 F について、$\rho_*(F)$ は、すべての $a \in A, y \in F$ について $a.y = \rho(a)y$ によって定義される A-加群構造との可換群 F であることを思い出してください。

#### 補題 1 {#ac-iv-s2-lem-1 .statement tag=04LD}

A をネーター 環、$p$ として A、E A-加群の主イデアルとし、その $p$ の消滅子含む冪と、$\rho_*(F)$ がフラットになるような $\operatorname{Ass}(E) = \{p\}$ および F B-加群を仮定します。 A-加群。 条件 $\mathfrak{P} \in \operatorname{Ass}_B(E \otimes_A F)$ は $\rho^{-1}(\mathfrak{P}) = p$ を意味します。

n が $p^nE = 0$ である場合、$p^nB \subset \operatorname{Ann}(E \otimes_A F)$、よって $p^nB \subset \mathfrak{P}$ は、$\rho_1(\mathfrak{P})$ が素数であるため、$p^n \subset \rho_1(\mathfrak{P})$、したがって $p \subset \rho_1(\mathfrak{P})$ を意味します。さらに、$a \in A - p$, ホモテティー h と E に対する比率 a は単射法です ($§ 1$, no. 1, 系 2 から命題 2)。 $h \otimes 1_F$ はホモテティー $h'$ で、$E \otimes_A F$ に対する比率 $\rho(a)$ があり、$\rho_*(F)$ はフラット、$h'$ は単射法です (章 I, § 2, no. 2, 定義 1)。これは、$\rho(a) \notin \mathfrak{P}$、よって $\rho^{-1}(\mathfrak{P}) = p$ であることを証明します。

#### 定理 2 {#ac-iv-s2-thm-2 .statement tag=04LE}

$\rho : A \to B$ を環準同型、E A-加群、F B-加群として、$\rho_*(F)$ がフラット A-加群となるようにします。それから

$$
\operatorname{Ass}_B(E \otimes_A F) \supset \bigcup_{p \in \operatorname{Ass}_A(E)} \operatorname{Ass}_B(F/pF).
$$

Aがネーターのとき、(5)の両辺は等しい。

$p \in \operatorname{Ass}_A(E)$ にしましょう。 定義までに完全系列が存在します

$$
0 \to A/p \to E.
$$

F はフラット A-加群なので、完全系列を導き出します。

$$
0 \to F/pF \to E \otimes_A F
$$

よって $\operatorname{Ass}_B(F/pF) \subset \operatorname{Ass}_B(E \otimes_A F)$、これは包含 (5) を証明します。

ここで、A がネーター であると仮定し、反対の包含を証明しましょう。

段階的に進めていきます。

(i) まず、E が有限生成A-加群であり、Ass_A(E) が単一の元 $p$ に還元されると仮定します。 § 1, no. 4, 定理 1 により、$E_i/E_{i+1}$ が $A/p_i$ と同型となるような E の組成列 $(E_i)_{0 \leq i \leq n}$ が存在します。ここで、$p_i$ は A の素イデアルです。さらに ($§ 1$、no. 4、定理 2 および no. 3、命題 7) すべての $p_i$ 含む $p$。 F はフラット A-加群なので、$E \otimes_A F$ と $(E_i \otimes_A F)/(E_{i+1} \otimes_A F)$ の $E_i \otimes_A F$ 形組成列は次のように識別されます。
$$
(A/p_i) \otimes_A F = F/p_i F.
$$
その後、$§ 1$、no. 1、命題 3 によって
$$
\operatorname{Ass}_B(E \otimes_A F) \subset \bigcup_{i=0}^{n-1} \operatorname{Ass}_B(F/p_i F).
$$
E は $p$ (no. 1, 注意) の冪によって全滅することがわかります。 補題 1 は、すべての $\mathfrak{P} \in \operatorname{Ass}_B(E \otimes_A F)$ について、$\rho^{-1}(\mathfrak{P}) = p$ であることを示します。 $F/p_i F$ は、補題 1 により、すべての $\mathfrak{P}' \in \operatorname{Ass}_B(F/p_i F)$ に対して $(A/p_i) \otimes_A F$、$\rho^{-1}(\mathfrak{P}') = p_i$ と同型であるため、$p_i \neq p$ であれば、よって $\operatorname{Ass}_B(E \otimes_A F) \cap \operatorname{Ass}(F/p_i F) = \varnothing$ となり、検討したケースでは定理であることが証明されます。

(ii) E が有限生成A-加群であるとのみ仮定します。 $p_i$ ($1 \leq i \leq n$) を $\operatorname{Ass}_A(E)$ の元とし、$\{0\} = \bigcap^n Q_i$ を対応するの縮小プライマリー 分解 (no. 3) とします。 E は、$E_i = E/Q_i$ の直和の部分加群と同型であり、F がフラット A-加群であるため、$E \otimes_A F$ は B-加群 $E_i \otimes_A F$ の直和の部分加群と同型です。 ($§ 1$、no. 1、命題 3 および系 1 ～ 命題 3) は次のように推測されます。
$$
\operatorname{Ass}_B(E \otimes_A F) \subset \bigcup_{i=1}^n \operatorname{Ass}_B(E_i \otimes_A F).
$$
しかし、$E_i$ は有限生成A-加群であるため、$\operatorname{Ass}_A(E_i)$ は 1 つの元 $p_i$ (no. 1, 定義 1) に縮小されます。 (i) により、この場合、$\operatorname{Ass}_B(E_i \otimes_A F) = \operatorname{Ass}_B(F/p_i F)$、よって定理となります。

(iii) *一般的なケース* B-加群 $E \otimes_A F$ は、部分加群 $E' \otimes_A F$ の和集合であり、$E'$ は、A-加群の有限生成された部分加群の集合を通過します。 E. $\mathfrak{P}$ の場合属するから $\operatorname{Ass}_B(E \otimes_A F)$ までの場合、$\mathfrak{P} \in \operatorname{Ass}_B(E' \otimes_A F)$ となるような E の有限生成された部分加群 $E'$ が存在します。 (ii) により、$\mathfrak{P} \in \operatorname{Ass}_B(F/pF)$ となるような $p \in \operatorname{Ass}_A(E')$ が存在します。 $\operatorname{Ass}_A(E') \subset \operatorname{Ass}_A(E)$ として、これで定理 2 の証明が完了します。

#### 系 1 {#ac-iv-s2-thm-2-cor-1 .statement tag=04LF}

*A がネーター と $\mathfrak{P} \in \operatorname{Ass}_B(E \otimes_A F)$ の場合、$\mathfrak{P} \in \operatorname{Ass}_B(F/pF)$ となるような A の素イデアル $p$ は $\rho^{-1}(\mathfrak{P}) \in \operatorname{Ass}_A(E)$ と $\rho^{-1}(\mathfrak{P})$ だけです。

#### 系 2 {#ac-iv-s2-thm-2-cor-2 .statement tag=04LG}

$A$ と $B$ がネーター で、$B$ がフラットな $A$ モジュールであると仮定します。 $p$を$A$の主イデアル、$Q \subset E$を$p$の主イデアル部分加群、$\mathfrak{P}$を$B$の主イデアルとする。 $Q \otimes_A B$ が $E \otimes_A B$ の $q$ 主要部分加群であるためには、$pB$ が $B$ の「p 主要イデアル」であることが必要かつ十分です。

定理を適用する 2 を $A$ モジュール $E/Q$ と $B$ モジュール $B$ に入力しましょう。この場合、$\operatorname{Ass}_A(E/Q) = \{p\}$ と $(E/Q) \otimes_A B$ は $(E \otimes_A B)/(Q \otimes_A B)$ と同型であるため、$\operatorname{Ass}_B((E \otimes_A B)/(Q \otimes_A B)) = \operatorname{Ass}_B(B/pB)$ となります。したがって、$Q \otimes_A B$ が $E \otimes_A B$ の $\mathfrak{P}$ 主要であるということは、$\operatorname{Ass}_B(B/pB)$ が $\mathfrak{P}$、よって系に還元されることを意味します。

#### 注意 {#ac-iv-s2-n6-rem-1 .statement tag=04LH}

$A$ と $B$ がネーター であるとします。 $\mathfrak{P}$ を $B$ の主な理想とし、$p = \overline{\rho}^{-1}(\mathfrak{P})$ とします。 $S = A - p$と書き、$k(p) = S^{-1}(A/p)$を$A/p$の分数の体とします。 $\mathfrak{P}$ 含む $pB$ なので、$\mathfrak{P}/pB$ は $B/pB$ の主要な理想です。 $\rho'$ が準同型 $A \xrightarrow{\rho} B \to B/pB$ の合成である場合、$S^{-1}(B/pB)$ は、この環 (章 II, § 2, no. 2, 命題) の理想として、環 $(\rho'(S))^{-1}(B/pB)$ および $\mathfrak{P}' = S^{-1}(\mathfrak{P}/pB)$ と同一視されることがわかります。 6); $\mathfrak{P}/pB$ は $\rho'(S)$ を満たさないため、$\mathfrak{P}'$ は $S^{-1}(B/pB)$ (章 11、§ 2, no. 5、命題 11) の主要な理想です。さらに、$S^{-1}(B/pB)$、$S^{-1}((A/p) \otimes_A B)$、$(S^{-1}(A/p)) \otimes_A B = k(p) \otimes_A B$の間には標準同型があります。同様に、$S^{-1}(F/pF)$ は正規的に $k(p) \otimes_A F$ と識別されます。したがって、定理 2 の仮説の下では、*位数では* $\mathfrak{P} \in \operatorname{Ass}_B(E \otimes_A F)$、*必要十分* $p \in \operatorname{Ass}_A(E)$ および
$$
\mathfrak{P}' \in \operatorname{Ass}_{k(p) \otimes_A B}(k(p) \otimes_A F).
$$
定理 2 とその系 1 により、条件を検証することになります。
$$
\text{``}\mathfrak{P} \in \operatorname{Ass}_B(F/pF)\text{''} \quad \text{and} \quad \text{``}\mathfrak{P}' \in \operatorname{Ass}_{k(p) \otimes_A B}(k(p) \otimes_A F)\text{''}
$$
は同等です。ただし、$B$ はネーター であるため、これは § 1, no. 2、系から命題 5 および上記の識別に続きます。

#### 命題 11 {#ac-iv-s2-prop-11 .statement tag=04LI}

$A$ と $B$ がネーター で、$B$ がフラットな $A$ モジュールであると仮定します。 Let $E$ be an $A$-module and $E'$ a submodule of $E$ such that, for every ideal $p \in \operatorname{Ass}_A(E/E')$, $pB$ is a prime ideal of $B$ or equal to $B$. $E' = \bigcap_{p \in \operatorname{Ass}(E/E')} Q(p)$ を $E$ の $E'$ の縮小プライマリー 分解とし、$Q(p)$ をすべての $p \in \operatorname{Ass}(E/E')$ の $p$ プライマリーとします。
(i) *$p \in \operatorname{Ass}(E/E')$ *かつ* $pB = B$の場合、*その後* $Q(p) \otimes_A B = E \otimes_A B$。
(ii) *もし* $p \in \operatorname{Ass}(E/E')$ *かつ* $pB$ *が素数*である場合、$Q(p)$ *は* $pB$*-初等* *in* $E \otimes_A B$。
(iii) *もし* $\Phi$ *が集合* $\mathfrak{p} \in \operatorname{Ass}(E/E')$ *そのような* $pB$ *が素数*である場合、*その後*
$$
E' \otimes_A B = \bigcap_{p \in \Phi} (Q(p) \otimes_A B)
$$
*そしてこの関係は、* $E' \otimes_A B$ *in* $E \otimes_A B$ の縮小された主要な分解です。

$pB = B$、定理 2 を $E/\mathbf{Q}(p)$ と $B$ に適用すると、次のことがわかります。
$$
\operatorname{Ass}_B((E/\mathbf{Q}(p)) \otimes_A B) = \varnothing
$$
そして、$B$ はネーター でフラットな $A$ モジュールであるため、$\mathbf{Q}(p) \otimes_A B = E \otimes_A B$ を結論する (§ 1, no. 1、系 1 から命題 2) とします。 主張 (ii) は、系 2 から $\mathfrak{P} = pB$ を取り、定理 2 に続きます。最後に、関係 $E' \otimes_A B = \bigcap_{p \in \Phi} (\mathbf{Q}(p) \otimes_A B)$ は、$B$ がフラットな $A$ モジュール (章 I, § 2, no. 6, 命題 6) であるという事実から導かれます。 $p \in \Phi$ (補題 1) の場合は $p = \overline{\rho}^{-1}(pB)$、集合 $\Phi$ の 2 つの異なる理想 $p, p'$ の場合は $pB \neq p'B$ です。一方、
$$
\operatorname{Ass}((E \otimes_A B)/(E' \otimes_A B)) = \Phi
$$
定理 2 著;私たちは no. 3 から結論する、命題 4
$$
E' \otimes_A B = \bigcap_{p \in \Phi} (\mathbf{Q}(p) \otimes_A B)
$$
縮小プライマリー分解です。

#### 系 {#ac-iv-s2-n6-cor-1 .statement tag=04LJ}

*$pB$ *すべての素数* $p \in \operatorname{Ass}_A(E/E')$ だと仮定します。 *次に、* $p_1, \ldots, p_n$ * が* $\operatorname{Ass}_A(E/E')$ の最小元である場合、** $p_iB$ * は* の最小元です
$$
\operatorname{Ass}_A((E \otimes_A B)/(E' \otimes_A B)).
$$
命題 11 から、この場合は $i \# j$ に対して $p_iB \neq p_jB$ となります。

*例*
(1) $B = S^{-1}A$ を考えます。ここで、$S$ は $A$ の乗算部分集合です。 $A$ がネーター の場合、命題 11 の仮説が満たされ、no. 4 の命題 6 の部分が回復されます。
(2) $A$ をネーター 環、$m$ を $A$ のイデアル、$B$ を $m$ 進法位相に関する $A$ のハウスドルフ完成とします。この場合、$B$ はフラットな $A$ モジュールであり、定理 2 は $F = B$ に適用できます。しかし一般に、命題 11 の仮説は、$A$ (章 III, § 2, 練習問題 15 (b)) の主イデアに対して満たされません。
(3) $A$ をネーター 環とし、$B$ を多項式代数 $A[X_1, \ldots, X_n]$ とします。 $B$ はネーター で、無料の $A$ モジュールであるためフラットです。 また、$p$ が $A$ の素イデアルである場合、$B/pB$ は整域である $(A/p)[X_1, \ldots, X_n]$ と同型であるため、$pB$ は素数になります。したがって、命題 11 の仮説は、すべての $A$ モジュール $E$ と $E$ のすべての部分加群 $E'$ で満たされます。
(4) $A$ を、$k$ の体 $k$、$K$ 拡大、および$K$ の拡大によって得られる $B = A \otimes_k K$ 代数にわたって有限生成された代数とします。スカラー; $A$ と $B$ はネーター で、$B$ は無料の $A$ モジュールであるため、定理 2 は $F = B$ に適用できます。 特定の場合 (たとえば、$k$ が代数的に閉じている場合) は、$A$ のすべての素イデアル $p$ について、$pB$ が素数または $B$ に等しいことが示されます。この例については後で戻ります。

### 練習問題 {#ac-iv-s2-exercises}

[§ 2 に対して練習問題](exercises/s2/)を参照してください。
