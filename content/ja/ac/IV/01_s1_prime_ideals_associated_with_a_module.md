---
book: ac
book_title: Commutative Algebra
chapter: IV
chapter_title: ASSOCIATED PRIME IDEALS AND PRIMARY DECOMPOSITION
section: 1
section_title: Prime ideals associated with a module
lang: ja
source: ac-i-vii
book_pages: 261-267, 286-290
pdf_pages: 0281-0287, 0306-0310
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF ASSOCIATED PRIME IDEALS
      page: 261
      pdf_page: 281
    - "no": 2
      title: LOCALIZATION OF ASSOCIATED PRIME IDEALS
      page: 263
      pdf_page: 283
    - "no": 3
      title: RELATIONS WITH THE SUPPORT
      page: 265
      pdf_page: 285
    - "no": 4
      title: THE CASE OF FINITELY GENERATED MODULES OVER A NOETHERIAN RING
      page: 265
      pdf_page: 285
statements: 24
exercises: 19
content_sha256: f6e29e693022da7e5f5cd978d5904a6d2102d30b512ff0827a5c93546a26b86a
translated_from: content/en/ac/IV/01_s1_prime_ideals_associated_with_a_module.md
translation_method: google
source_content_sha256: 41bc8b6bc73ee003f10c2b0789585e99cc74ba8b5cfcd5f713cf440dd2d53406
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-eeeca2ef
glossary_version: 34
glossary_terms_sha256: 1e5dff038de7a4fc8633b7dcb22a579561b99dca5cdc311379506cbc491fe568
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## 1. 加群に関連する主な理想

### 1. 関連する主な理想の定義

#### 定義 1 {#ac-iv-s1-def-1 .statement tag=04J7}

M を環 A よりも加群とします。 p が消滅子 & x に等しい x ∈ M が存在する場合、素イデアル p は M に関連付けられていると言われます。 M に関連付けられた素イデアルの集合は、Ass_A(M) または単に Ass(M) で表されます。

\* 例。 Let a be an ideal in the polynomial ring A = \mathbf{C}[X_1, ..., X_n], V the corresponding affine algebraic variety and V_1, ..., V_p the irreducible components of V. If M is taken to be the ring A/a of functions which are regular on V, the set of prime ideals associated with M consists of the ideals of V_1, ..., V_p and in general other prime ideals each of which contains one of the ideals of the V_i. \*

0 の消滅子が A であるため、消滅子が素イデアである元 x ∈ M は必然的に ≠ 0 になります。素イデア p が M に関連付けられていると言うことは、

(*) この章の結果は、章I, § 4と章III, § 5を除く、本書IからVIと章IからIIIのみに依存します。

amounts to saying that $M$ contains a submodule *isomorphic to* $A/p$ (namely $Ax$, for all $x \in M$ whose annihilator is $p$).

$A$ モジュール $M$ が部分加群のファミリー $(M_i)_{i \in I}$ の和集合である場合、明らかに
$$
\operatorname{Ass}(M) = \bigcup_{i \in I} \operatorname{Ass}(M_i).
$$

#### 命題 1 {#ac-iv-s1-prop-1 .statement tag=04J8}

*環 $A$ のすべての素数イデアル $p$ と、$A/p$、$\operatorname{Ass}(M) = \{p\}$ のすべての部分加群 $M \neq 0$ に対して。

As the ring $A/p$ is an integral domain, the annihilator of an element $\neq 0$ of $A/p$ is $p$.

#### 命題 2 {#ac-iv-s1-prop-2 .statement tag=04J9}

*$M$を環$A$の上に加群とします。 集合の各極大元 、$\operatorname{Ann}(x)$ $A$ のうち、$x$ は、元の集合 $M$ の $\neq 0$、属するから$\operatorname{Ass}(M)$ まで続きます。*

$a = \operatorname{Ann}(x)$ ($x \in M, x \neq 0$) をそのような極大元とします。 $a$ が素数であることを示すだけで十分です。 $x \neq 0$、$a \neq A$として。 $b, c$ を $A$ の元とし、$bc \in a$ と $c \notin a$ とします。続いて$cx \neq 0$、$b \in \operatorname{Ann}(cx)$、$a \subset \operatorname{Ann}(cx)$。 $a$ が最大なので、$\operatorname{Ann}(cx) = a$、よって $b \in a$ なので、$a$ が素数になります。

#### 系 1 {#ac-iv-s1-prop-2-cor-1 .statement tag=04JA}

*$M$をネーター環$A$の上に加群とします。したがって、条件 $M \neq \{0\}$ は $\operatorname{Ass}(M) \neq \varnothing$ と同等です。*

$M = \{0\}$ の場合、明らかに $\operatorname{Ass}(M)$ は空です ($A$ には仮定がありません)。 $M \neq \{0\}$ の場合、形 $\operatorname{Ann}(x)$ の理想のうち集合 ($x \in M$ と $x \neq 0$) は空ではなく、$\# A$ の理想で構成されます。 $A$ はネーター であるため、この集合には極大元が含まれます。その場合は命題を適用する 2 で十分です。

#### 系 2 {#ac-iv-s1-prop-2-cor-2 .statement tag=04JB}

*$A$ をネーター 環、$M$ を $A$ モジュール、$a$ 元を $A$ とします。 $a$ の比を持つ $M$ 上のホモテティー が単射であるためには、$a$ 属するが $M$ に関連付けられた素イデアルを持たないことが必要かつ十分です。*

素数理想 $p \in \operatorname{Ass}(M)$ に対して $a$ 属するの場合、$p = \operatorname{Ann}(x)$、ここで $x \in M, x \neq 0$; よって $ax = 0$ とホモテティー の比率 $a$ は単射的ではありません。逆に、$x \# 0$ のような一部の $x \in M$ に対して $ax = 0$ の場合、$Ax \# \{0\}$、よって $\operatorname{Ass}(x) \neq \varnothing$ (系 1) となります。 $p \in \operatorname{Ass}(Ax)$ にしましょう。次に、明らかに $p \in \operatorname{Ass}(M)$ と $p = \operatorname{Ann}(bx)$、ここで $b \in A$; よって $a \in p$、$abx = 0$以来。

#### 系 3 {#ac-iv-s1-prop-2-cor-3 .statement tag=04JC}

*The set of divisors of zero in a Noetherian ring $A$ is the union of the ideals $p \in \operatorname{Ass}(A)$.*

#### 命題 3 {#ac-iv-s1-prop-3 .statement tag=04JD}

*$A$ を環、$M$ を $A$ モジュール、$N$ 部分加群を $N$ とします。それから*
$$
\operatorname{Ass}(N) \subset \operatorname{Ass}(M) \subset \operatorname{Ass}(N) \cup \operatorname{Ass}(M/N).
$$
*$\operatorname{Ass}(N) \subset \operatorname{Ass}(M)$ が含まれていることは明らかです。 $p \in \operatorname{Ass}(M)$、$E$ を $A/p$ および $F = E \cap N$ と同型の $M$ の部分加群とします。 $F = \{0\}$ の場合、$E$ は、$M/N$、よって $p \in \operatorname{Ass}(M/N)$ の a* 部分加群と同型です。 $F \neq \{0\}$ の場合、$F$ のすべての元 $\neq 0$ の消滅子は $p$ (命題 1) であるため、$p \in \operatorname{Ass}(F) \subset \operatorname{Ass}(N)$ になります。

#### 系 1 {#ac-iv-s1-prop-3-cor-1 .statement tag=04JE}

*A-加群 $M$ が部分加群の家族 $(M_i)_{i \in I}$ の直和である場合、* $\operatorname{Ass}(M) = \bigcup_{i \in I} \operatorname{Ass}(M_i)$ です。

それは、(1) によって $I$ が有限である場合に還元され、その後、$\operatorname{Card}(I)$ で帰納法により $\operatorname{Card}(I) = 2$ が有限である場合に還元される可能性があります。次に、$I = \{i, j\}$ とします。ここで、$i \neq j$; $M/M_i$ は $M_j$、$\operatorname{Ass}(M) \subset \operatorname{Ass}(M_i) \cup \operatorname{Ass}(M_j)$ (命題 3) と同型です。さらに、$\operatorname{Ass}(M)$ (命題 3)、よっての結果には、$\operatorname{Ass}(M_i)$ と $\operatorname{Ass}(M_j)$ が含まれています。

#### 系 2 {#ac-iv-s1-prop-3-cor-2 .statement tag=04JF}

*$M$をA-加群、$(Q_i)_{i \in I}$を$M$の部分加群の有限族とする。もし* $\bigcap_{i \in I} Q_i = \{0\}$、*その後*
$$
\operatorname{Ass}(M) \subset \bigcup_{i \in I} \operatorname{Ass}(M/Q_i).
$$
標準写像 $M \to \bigoplus_{i \in I} (M/Q_i)$ は単射です。その場合、命題を適用する 3 とその系 1 で十分です。

#### 命題 4 {#ac-iv-s1-prop-4 .statement tag=04JG}

※$M$をA-加群、$\Phi$を$\operatorname{Ass}(M)$の部分集合とします。次に、* $\operatorname{Ass}(N) = \operatorname{Ass}(M) - \Phi$ * と* $\operatorname{Ass}(M/N) = \Phi$ のような $M$ の部分加群 $N$ が存在します。

$\mathscr{E}$ を部分加群の集合、$M$ の $P$ として、$\operatorname{Ass}(P) \subset \operatorname{Ass}(M) - \Phi$ とします。 公式 (1) は、包含順に並べられた集合 $\mathscr{E}$ が *帰納的*であることを示しています。さらに、$\{0\} \in \mathscr{E}$ なので $\mathscr{E} \neq \varnothing$ です。 $N$を$\mathscr{E}$の極大元とします。続いて$\operatorname{Ass}(N) \subset \operatorname{Ass}(M) - \Phi$。 $\operatorname{Ass}(M/N) \subset \Phi$ がわかり、命題 3 までに証明が完了します。 $p \in \operatorname{Ass}(M/N)$ にしましょう。次に、$M/N$ 含む部分加群 $F/N$ は $A/p$ と同型です。 命題 1 と 3、$\operatorname{Ass}(F) \subset \operatorname{Ass}(N) \cup \{p\}$ までに。 $N$は$\mathscr{E}$、$F \notin \mathscr{E}$で最大なので、$p \in \Phi$となります。

### 2. 関連する主イデアルの位置特定

#### 命題 5 {#ac-iv-s1-prop-5 .statement tag=04JH}

*$A$を環、$S$を$A$の乗算部分集合、$S$と$M$を満たさない$A$の素イデアルの$\Phi$集合とするA-加群。その後*:
(i) *写像* $p \mapsto S^{-1}p$ *は* $\operatorname{Ass}_A(M) \cap \Phi$の全単射 *$\operatorname{Ass}_{S^{-1}A}(S^{-1}M)$の部分集合の上です。
(ii) *もし* $p \in \Phi$ *が有限生成された理想であり* $S^{-1}p \in \operatorname{Ass}_{S^{-1}A}(S^{-1}M)$、*その後* $p \in \operatorname{Ass}_A(M)$。

(章 II, § 2, no. 5, 命題 11) 写像 $p \mapsto S^{-1}p$ は、$S^{-1}A$ の素イデアルの集合上の $\Phi$ の全単射であることを思い出してください。 $p \in \operatorname{Ass}_A(M) \cap \Phi$ の場合、$p$ は $M$ の部分加群 $N$ の消滅子です。この場合、$S^{-1}p$ は、$S^{-1}M$ (章 II, § 2, no. 4, 公式 (9)) の単次部分加群 $S^{-1}N$ の消滅子となり、したがって $S^{-1}\mathfrak{p} \in \mathrm{Ass}_{S^{-1}A}(S^{-1}M)$ になります。逆に、$\mathfrak{p} \in \Phi$ が有限に生成され、$S^{-1}\mathfrak{p}$ が $S^{-1}M$ に関連付けられるとします。その場合、$S^{-1}\mathfrak{p}$ は $x/t$ の消滅子となるように、$x \in M$ と $t \in S$ が存在します。 $(a_i)_{1 \leq i \leq n}$ を $\mathfrak{p}$ の生成元の系とします。次に $(a_i/1)(x/t) = 0$ となり、したがって $s_i a_i x = 0 \ (1 \leq i \leq n)$ となる $s_i \in S$ が存在します。 $s = s_1 s_2 \ldots s_n$ と書きましょう。すべての$a \in \mathfrak{p}$、$s a x = 0$、よって $p \subset \mathrm{Ann}(s x)$。一方、$b \in A$ が $b s x = 0$ を満たす場合、定義、よって $b \in \mathfrak{p}$ により $b/1 \in S^{-1}\mathfrak{p}$ になります。続いて$\mathfrak{p} = \mathrm{Ann}(s x)$と$\mathfrak{p} \in \mathrm{Ass}_A(M)$。

#### 系 {#ac-iv-s1-n2-cor-1 .statement tag=04JI}

*環 A がネーター の場合、写像 $\mathfrak{p} \mapsto S^{-1}\mathfrak{p}$ は $\mathrm{Ass}_{S^{-1}A}(S^{-1}M)$ 上の $\mathrm{Ass}_A(M) \cap \Phi$ の全単射です。

A がネーター でない場合、$\mathrm{Ass}_A(M) \cap \Phi$ ～ $\mathrm{Ass}_{S^{-1}A}(S^{-1}M)$ の写像 $p \mapsto S^{-1}p$ は必ずしも全射ではありません (練習問題 1)。

#### 命題 6 {#ac-iv-s1-prop-6 .statement tag=04JJ}

*A をネーター 環、M A-加群、S を A の乗法部分集合と、S を満たさない元の $\mathrm{Ass}_A(M)$ の Y 集合とします。すると、標準写像 $M \to S^{-1}M$ の核 N となります。は、関係* を満たす M の一意の部分加群

$$
\mathrm{Ass}(N) = \mathrm{Ass}(M) - \Psi, \quad \mathrm{Ass}(M/N) = \Psi.
$$

no. 1 の命題 4 までに、関係 $\mathrm{Ass}(N') = \mathrm{Ass}(M) - Y$ と $\mathrm{Ass}(M/N') = \Psi$ を満たす M の部分加群 $N'$ が存在します。 $N = N'$ を証明する必要があります。可換図式を考えてみましょう

$$
\begin{array}{ccc}
M & \xrightarrow{p} & M/N' \\
|u| & & |v| \\
S^{-1}M & \xrightarrow{S^{-1}p} & S^{-1}(M/N')
\end{array}
$$

ここで、$p, u, v$ は標準準同型です。 $S^{-1}p$ と $v$ が単射であることを示し、$u$ と $p$ が同じ核であるため、$N = N'$ であることが証明されます。

$\mathrm{Ass}(N') \cap \Psi = \varnothing$ として、$\mathrm{Ass}(N')$ のすべての元は S と一致します。次に、$\mathrm{Ass}_{S^{-1}A}(S^{-1}N') = \varnothing$ (系から命題 5)、よって $S^{-1}N' = \{0\}$ (no. 1、系 1 から命題 2) になります。 $S^{-1}p$ が単射であることを証明します (章 II, §2, no. 4, 定理 1)。一方、$x$ 属するから $v$ の核 K であれば、$\mathrm{Ann}(x) \cap S \neq \varnothing$ (章 II, §2, no. 2, 命題 4);したがって $\mathrm{Ass}(K) = \varnothing$ 以来 $\mathrm{Ass}(K) \subset \mathrm{Ass}(M/N') = \Psi$; $K = \{0\}$ (no. 1、系 1 ～ 命題 2) および $v$ は単射であると推測します。

### 3. 関係サポート付き

M を環 A よりも加群とする。A の素イデアル $\mathfrak{p}$ の集合を思い出してください。$M, \neq 0$ は M のサポートと呼ばれ、$\operatorname{Supp}(M)$ (章 II, § 4, no. 4, 定義 5) で表されます。

#### 命題 7 {#ac-iv-s1-prop-7 .statement tag=04JK}

Aを環、MをA-加群とします。

(i) 含む元 $\in \operatorname{Ass}(M)$ 属するから $\operatorname{Supp}(M)$ までのすべての素数イデアル $\mathfrak{p}$。

(ii) 逆に、A がネーター の場合、すべての理想は $\mathfrak{p} \in \operatorname{Supp}(M)$ 含む元 $\in \operatorname{Ass}(M)$ になります。

$\mathfrak{p}$ 含む元 $q$ の $\operatorname{Ass}(M)$ の場合、$q \cap (A - \mathfrak{p}) = \varnothing$ となるため、$S = A - \mathfrak{p}$ と書くと、$S^{-1}\mathfrak{p}$ は $S^{-1}M = M$、(no. 2、命題 5) に関連付けられた主イデアルになります。 *なおさら* $M, \# 0$、したがって $\mathfrak{p} \in \operatorname{Supp}(M)$。逆に、A がネーター の場合、A も同様です (章 II, § 2, no. 4、系 2 ～ 命題 10)。 $M_{\mathfrak{p}} \neq 0$ の場合、$\operatorname{Ass}_{A_{\mathfrak{p}}}(M_{\mathfrak{p}}) \neq 0$ (no. 1, 系 1 ～ 命題 2) となり、$q \cap (A - \mathfrak{p}) = \varnothing$ (no. 2, 系 ～ 命題 5) となる $q \in \operatorname{Ass}_A(M)$ が存在します。

#### 系 1 {#ac-iv-s1-prop-7-cor-1 .statement tag=04JL}

M がネーター 環よりも加群である場合、$\operatorname{Ass}(M) \subset \operatorname{Supp}(M)$ となり、これら 2 つの集合は同じ最小値元を持ちます。

#### 系 2 {#ac-iv-s1-prop-7-cor-2 .statement tag=04JM}

ネーター 環 A のニルラジカルは、理想 $\mathfrak{p} \in \operatorname{Ass}(A)$ の共通部分です。

A のニルラジカルは、$\operatorname{Spec}(A) = \operatorname{Supp}(A)$ (章 II, § 2, no. 6, 命題 13) の最小値元の共通部分であることがわかります。

### 4. ネーター 環より有限生成加群の場合

#### 定理 1 {#ac-iv-s1-thm-1 .statement tag=04JN}

A をネーター 環、M を有限生成A-加群とします。 $0 \leq i \leq n - 1$ に対して、$M_i / M_{i+1}$ が $A / \mathfrak{p}_i$ と同型となるような M の組成列 $(M_i)_{0 \leq i \leq n}$ が存在します。ここで、$\mathfrak{p}_i$ は A の素イデアルです。

$\mathscr{G}$ を、主張の性質と組成列を持つ M の部分加群の集合とします。 $\mathscr{G}$ は空ではなく ($\{0\}$ 属するから $\mathscr{G}$ の場合)、M はネーター であるため、$\mathscr{G}$ は極大元 N を持ちます。 $M \neq N$ の場合、$M/N \neq 0$、したがって $\operatorname{Ass}(M/N) \neq \varnothing$ (no. 1, 系 1 ～ 命題 2);したがって、$M/N$ は、含む部分加群 $N'/N$ は、形 $A/\mathfrak{p}$ の A-加群と同型であり、$\mathfrak{p}$ は素数です。次に定義 $N' \in \mathscr{G}$ により、N の最大値指標である矛盾するになります。すると必然的に $N = M$ になります。

#### 定理 2 {#ac-iv-s1-thm-2 .statement tag=04JO}

M をネーター 環 A および $(M_i)_{0 \leq i \leq n}$ 組成列上の有限生成加群とし、$0 \leq i \leq n - 1$ に対して、$M_i / M_{i+1}$ が $A / \mathfrak{p}_i$ と同型となるようにします。ここで、$\mathfrak{p}_i$ は A の素イデアルです。 それから

(4)
$$
\operatorname{Ass}(M) \subset \{\mathfrak{p}_0, \ldots, \mathfrak{p}_{n-1}\} \subset \operatorname{Supp}(M);
$$

これら 3 つの集合の最小元は同じであり、一致するは素数理想含むの集合の最小元と同じです。

Ass(M) $\subset \{p_0, \ldots, p_{n-1}\}$ は、no. 1 の命題 1 と 3 の直後に続きます。 $0 \leq i \leq n - 1$ の場合、

$$
p_i \in \operatorname{Supp}(A/p_i) = \operatorname{Supp}(M_i/M_{i+1})
$$

(章 II, § 4, no. 4, 例)、よって $p_i \in \operatorname{Supp}(M_i) \subset \operatorname{Supp}(M)$ (章 II, § 4, no. 4, 命題 16)、これは包含を示します

$$
\{p_0, \ldots, p_{n-1}\} \subset \operatorname{Supp}(M).
$$

no. 3 の系 1 から命題 7 は、Ass(M) と Supp(M) が同じ最小値元を持つことを示し、(4) は、これらが $\{p_0, \ldots, p_{n-1}\}$ の最小値元にすぎないことを示します。 最後の主張は、章 II, § 4, no. 4、命題 17 から続きます。

#### 系 {#ac-iv-s1-n4-cor-1 .statement tag=04JP}

*If M is a finitely generated module over a Noetherian ring A, Ass(M) is finite.*

定理 2 の条件では、集合 $\{p_0, \ldots, p_{n-1}\}$ は必ずしも M によって一意に決定されるわけではありません。特に、Ass(M) (練習問題 6) とは異なる場合があります。

#### 命題 8 {#ac-iv-s1-prop-8 .statement tag=04JQ}

*A をネーター 環、A と M 有限生成A-加群の理想とする。次の条件は同等です:*

(a) *$ax = 0$となるような M の元 x $\# O$ が存在します。*
(b) *すべての $a \in a$ に対して、$ax = 0$ となるような M の元 x $\neq O$ が存在します。*
(c) *$a \subset p$となるような$p \in \operatorname{Ass}(M)$が存在します。*

明らかに (a) は (b) を意味します。 no. 1、系 2 から命題 2、条件 (b) は、Ass(M) が有限 (章 11、§ 1, no. 1、命題) であるため、イデアル a が M に関連付けられた素イデアルの和集合に含まれ、したがってそのうちの 1 つに含まれることを意味します。 2);したがって、(b) は (c) を意味します。 最後に、$a \subset p$ のような $p \in \operatorname{Ass}(M)$ が存在する場合、p は M (no. 1, 定義 1) および $ax = 0$ の元 $x \neq 0$ の消滅子です。したがって、(c) は (a) を意味します。

#### 命題 9 {#ac-iv-s1-prop-9 .statement tag=04JR}

*A をネーター 環とし、A と M 有限生成A-加群の理想を表します。 $a^n M = 0$ のような整数 $n > 0$ が存在するには、a が M に関連付けられた主イデアルの共通部分に含まれることが必要かつ十分です。

この共通部分は、Supp(M)の極小元(no. 3、系1から命題7)の元でもあり、この共通部分にaが含まれるということは、章の記法に$V(a) \supset \operatorname{Supp}(M)$が含まれるというと同等です。 II, § 4;結論は、章 11、§ 4, no. 4、系 2 から命題 17 となります。

#### 定義 2 {#ac-iv-s1-def-2 .statement tag=04JS}

$A$ 加群 $M$ が与えられた場合、すべての $x \in M$ に対して $u^{n(x)}(x) = 0$ となる整数 $n(x) > 0$ が存在する場合、$M$ の自己準同型 $u$ はほぼゼロポテントと呼ばれます。

$M$ が有限に生成される場合、ほぼすべての冪零自己準同型はゼロになります。

#### 系 {#ac-iv-s1-n4-cor-2 .statement tag=04JT}

$A$ をネーター 環とします。 $M$ と $A$ モジュール、および $A$ の $a$ 元。 $M$ の準同型 $a_M : x \mapsto ax$ がほぼ無能であるためには、$a$ 属するが $\operatorname{Ass}(M)$ のすべての理想に対して必要かつ十分です。

主張の条件は、すべての $x \in M$ に対して $(Aa)^{n(x)}(Ax) = 0$ となる $n(x) > 0$ が存在するというと同等です。 命題 9 ということは、$M$ の部分加群 $Ax$ に関連するすべての主要な理想に対して $a$ 属するが含まれることも意味します。 系は、$x$ が $M$ を通る$\operatorname{Ass}(M)$ が $\operatorname{Ass}(Ax)$ の和集合であるという事実から続きます (no. 1, 公式 (1))。

#### 命題 10 {#ac-iv-s1-prop-10 .statement tag=04JU}

$A$ をネーター 環、$E$ を有限生成された $A$ モジュール、$F$ を $A$ モジュールとします。それから

$$
\operatorname{Ass}(\operatorname{Hom}_A(E, F)) = \operatorname{Ass}(F) \cap \operatorname{Supp}(E).
$$

仮定により、$E$ は形 $A^n/R$ の $A$ 加群と同型であるため、$\operatorname{Hom}_A(E, F)$ は $\operatorname{Hom}_A(A^n, F)$ の部分加群と同型であり、後者は $F^n$ と同型です。現在、$\operatorname{Ass}(F^n) = \operatorname{Ass}(F)$ (no. 1、系 1 ～ 命題 3)。したがって$\operatorname{Ass}(\operatorname{Hom}_A(E, F)) \subset \operatorname{Ass}(F)$。一方、

$$
\operatorname{Supp}(\operatorname{Hom}_A(E, F)) \subset \operatorname{Supp}(E):
$$

$A$ のすべての素イデアル $p$ について、$\operatorname{Hom}_{A_p}(E_p, F_p)$ は $(\operatorname{Hom}_A(E, F))_p$ (章 11, § 2, no. 7, 命題 19)、よっての主張と同型です。次に、定理 2 から結論するとなります。

$$
\operatorname{Ass}(\operatorname{Hom}_A(E, F)) \subset \operatorname{Supp}(E).
$$

逆に、$p$ を $A$ 所属から $\operatorname{Ass}(F) \cap \operatorname{Supp}(E)$ の主要な理想とする。 定義、$F$ 含む部分加群は $A/p$ と同型です。一方、$E$と$E, \neq 0$は有限生成なので、$E$から$A/p$まで準同型$w \neq 0$(章II, § 4, no. 4,命題20)が存在することがわかります。 $A/p$から$F$までは単射準同型$j$、$j \circ w \in \operatorname{Hom}(E, F)$、$j \circ w \neq 0$が存在します。一方、一部の $a \in A$ の関係 $aw = 0$ は、$a \in p$ に相当し、$A/p$ のすべての元 $\neq 0$ の消滅子は $p$ です。それなら確かに $p \in \operatorname{Ass}(\operatorname{Hom}_A(E, F))$ です。

### 練習問題 {#ac-iv-s1-exercises}

[§ 1 に対して練習問題](exercises/s1/)を参照してください。
