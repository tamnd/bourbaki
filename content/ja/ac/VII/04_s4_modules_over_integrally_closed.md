---
book: ac
book_title: Commutative Algebra
chapter: VII
chapter_title: DIVISORS
section: 4
section_title: Modules over integrally closed Noetherian domains
lang: ja
source: ac-i-vii
book_pages: 512-544, 571-578
pdf_pages: 0530-0562, 0589-0596
extraction: ocr
subsections:
    - "no": 1
      title: LATTICES
      page: 512
      pdf_page: 530
    - "no": 2
      title: DUALITY; REFLEXIVE MODULES
      page: 517
      pdf_page: 535
    - "no": 3
      title: LOCAL CONSTRUCTION OF REFLEXIVE MODULES
      page: 521
      pdf_page: 539
    - "no": 4
      title: PSEUDO-ISOMORPHISMS
      page: 523
      pdf_page: 541
    - "no": 5
      title: DIVISORS ATTACHED TO TORSION MODULES
      page: 527
      pdf_page: 545
    - "no": 6
      title: RELATIVE INVARIANT OF TWO LATTICES
      page: 529
      pdf_page: 547
    - "no": 7
      title: DIVISOR CLASSES ATTACHED TO FINITELY GENERATED MODULES
      page: 531
      pdf_page: 549
    - "no": 8
      title: PROPERTIES RELATIVE TO FINITE EXTENSIONS OF THE RING OF SCALARS
      page: 535
      pdf_page: 553
    - "no": 9
      title: A REDUCTION THEOREM
      page: 540
      pdf_page: 558
    - "no": 10
      title: MODULES OVER DEDEKIND DOMAINS
      page: 543
      pdf_page: 561
statements: 56
exercises: 26
content_sha256: 6d4ebbbb55f4dd1966e319249e14e84780a94dbb4e76cb69f1181f163481eda5
translated_from: content/en/ac/VII/04_s4_modules_over_integrally_closed.md
translation_method: google
source_content_sha256: 72d54cdf6923d26d9507679e68c08eb8627c1c668375ce55e331655e15e45177
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: 5fe2e5019493aa01063c16342ac5e855eb9bf4935bfde7a988af2d27e8c03403
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## 4. 加群が完全に閉じられたネーター ドメイン上で

この段落全体を通じて、$\mathbf{A}$ は分数 $K$ の体と *可換整域* になります。 no. 2 から始まり、$\mathbf{A}$ はさらに *ネーター で完全に閉じている* (したがって、Krull ドメイン ($\S$ 1、no. 3、系から定理 2)) であると想定されます。その場合、$P(\mathbf{A})$、$D(\mathbf{A})$、$C(\mathbf{A})$はそれぞれ、高さ1の$\mathbf{A}$（$\S$1、no. 6）の主イデアルの集合、$\mathbf{A}$の因子、群を表します。 ($\S$ 1, no. 3) と $\mathbf{A}$ ($\S$ 1, no. 10) の因子類群、これら後者は *加算* で書かれています。

統合的に閉じたネーター 領域 $\mathbf{A}$ 上で有限生成加群を研究する一般的な方法は、$\mathbf{A}$ の *高さ* 1 のすべての主要イデア $p \in P(\mathbf{A})$ に関して加群を「位置特定」することで構成されます。 $\mathbf{A}$ として、*離散評価環* ($\S$ 1、no. 6、定理 4)、有限生成された $\mathbf{A}_p$ モジュールの構造はよく知られています (*代数*、 章 VII, $\S$ 4) したがって、有限生成された $\mathbf{A}$ モジュールの構造に関する情報が得られます。 $\mathbf{A}$ がデデキント領域である特定のケースでは、$\mathbf{A}$ が主イデアル整域 (no. 10) である場合と同じくらい完全な理論に到達できます。

### 1. 格子

#### 定義 1 {#ac-vii-s4-def-1 .statement tag=052X}

*$V$を体$K$の上に有限次元ベクトル空間とします。 $\mathbf{A}$ に対する $V$ の格子 (または単に $V$ の格子) は、$V$ 満たすのサブ$\mathbf{A}$ モジュール $M$ と次の条件として定義されます。

$L_1 \subset M \subset L_2$ と $\mathrm{rg}_{\mathbf{A}}(L_1) = \mathrm{rg}_K(V)$ など、$V$ の 2 つの空きサブ$\mathbf{A}$ モジュール $L_1,\ L_2$ が存在します。

例
(1) $V = K$ を取ると、$K$ の格子は、$K$ の *分数イデアル* $\neq (0)$ ($\S$ 1, no. 1, 定義 1) にすぎません。

(2) $\mathrm{rg}_K(V) = n$ の場合、V のすべての*空き* サブ A モジュール L には、基底含むが最大で n 元あり、V のすべての部分集合は A 上で空き、K 上でも空きです。 L が V の格子であるためには、L が n 元のうち基底を持つことが必要かつ十分です (他の語では、$\mathrm{rg}_A(L) = n$)。

(3) A が *主イデアル整域* の場合、V のすべての格子 M は有限生成A-加群 (A がネーター であるため)、これはねじれがなく、したがって *自由* A-加群 (*代数*, 章) VII, § 4, no. 3、系 2 ～ 定理 2)。

#### 命題 1 {#ac-vii-s4-prop-1 .statement tag=052Y}

*V のサブ A モジュール M が V の格子であるためには、KM = V であり、M が有限生成された V のサブ A モジュールに含まれることが必要かつ十分です。

条件は、V 生成する V と同じ階数を備えた V の無料サブ A モジュールに明らかに必要です。逆に、KM = V の場合、M 含む基底 $(a_i)_{1 \leq i \leq n}$ の V は K を超え、したがって含むは、$a_i$ によって生成された空きサブ A モジュール L になります。一方、$M \subset M_1$ (M は元 b の有限数によって生成される V のサブ A モジュールであり、$(e_i)_{1 \leq i \leq n}$ が K 上の V の基底である場合、元が存在します) A の $\neq 0$ は、各 b が係数 *in* A を持つ $s^{-1}e_i$ の線形結合となる。 L が $s^{-1}e_i$ によって生成された V の空きサブ A モジュールである場合、$M \subset L_2$。

#### 系 {#ac-vii-s4-n1-cor-1 .statement tag=052Z}

*A がネーター であるとします。 V のサブ A モジュール M が V の格子となるためには、KM = V であり、M が有限に生成されることが必要かつ十分です。*

#### 注意 (1) {#ac-vii-s4-n1-rem-1 .statement tag=0530}

V 標準写像 $M \otimes_A K \to V$ のサブ A モジュール M は単射であり、像 KM (*代数*, 章 II, § 7, no. 10, 命題 26) であることを思い出してください。したがって、KM = V ということは、この写像が *全単射 * であることを意味します。

#### 命題 2 {#ac-vii-s4-prop-2 .statement tag=0531}

*M を V の格子、M を V のサブ A モジュールとする。 $xM \subset M_1 \subset yM$, $M_1$ が V の格子となる 2 つの元 x, y が $K^*$ に存在する場合、逆に、$M_1$ が V の格子である場合、$aM \subset M, \subset b^{-1}M$ となるような A の 2 つの非ゼロ元 a、b が存在します。

$L_1, L_2$ が 2 つの自由格子である V である場合、$L, \subset M \subset L,$、関係 $xM \subset M_1 \subset yM$ は $xL_1 \subset M, \subset yL_2$、$xL_1$ および $yL_2$ が自由格子であることを意味します。逆に、M が格子であり、A 上の関係 KM 上の L の $(e_i)_{1 \leq i \leq n}$ 基底 = V は、すべてに対して $xe_i \in M,$ が成り立つような $x = a/s \in K^*$ (a と s が非ゼロの A の元) の存在を意味します。 $i$、よって $xM \subset xL_2 \subset M_1$ および *なおさら* $aM \subset M,$; M と M の役割を交換すると、A には $bM_1 \subset M$ となるような $b \neq 0$ が存在することが同様に示されます。

#### 命題 3 {#ac-vii-s4-prop-3 .statement tag=0532}

(i) *$M_1$と$M_2$がVの格子である場合、$M_1 \cap M,$と$M_1 + M_2$も同様です。

(ii) *W が V のベクトル部分空間で、M が V の格子である場合、$M \cap W$ は W の格子です。*

(iii) $V, V_1, \ldots, V_k$ を $K$ 上の有限階数のベクトル空間として、
$$
f : V_1 \times \cdots \times V_k \to V
$$
像生成する $V$ の多重線形マッピングになります。 *$M_i$が$1 \leq i \leq k$の$V_i$の格子である場合、$f$($(M, x \ldots x M_k)$)によって生成される$V$のサブAモジュールは$V$の格子になります。

(iv) $V$ と $W$ を $K$ 上の有限階数の 2 つのベクトル空間 、$M$ を$V$ の格子、$N$ を$W$ の格子とする。 *サブ A モジュール $N$: $\mathrm{Hom}_K(V, W)$ の $M$、K-線型写像のからなる $f$ は、$f(M) \subset N$ が $\mathrm{Hom}_K(V, W)$ の格子になります。*

(i) 命題 2 により、$A$ には $aM_1 \subset M_2 \subset b^{-1}M_1$ となる非ゼロ$a$ と $b$ が存在します。 結論するでは、$M_1 \cap M_2$ と $M_1 + M_2$ は $aM_1$ と $b^{-1}M_1$ の間にあり、したがって命題 2 によって格子であると考えられます。

(ii) $S$ を $V$ の $W$ の補数、$L_w$ を $W$ の自由格子、$L_s$ を $S$ の自由格子とし、$L = L_w \oplus L_s$ を $V$ の自由格子とします。すると、$K^*$には$xL \subset M \subset yL$のような$x, y$が存在します。 $xL_w \subset M \cap W \subset yL_w$ を推定すると、$M \cap W$ が $W$ (命題 2) の格子であることがわかります。

(iii) $KM_i = V$ として、線形性により明らかに $f$ ($M_1 x \ldots x M_n$) 生成するベクトル K 空間 $V$;一方、すべての $i$ に対して、$M_i \subset N_i$ のような、$V$ の有限生成されたサブ A モジュール $N_i$ が存在します。 $f(N_1 x \ldots x N_n)$ によって生成された$V$ のサブ A 加群 $N$ は有限生成され、含む $M$ であるため、$M$ は$V$ (命題 1) の格子になります。

(iv) $P$ (それぞれ $Q$) を $V$ (それぞれ $W$) 含む $M$ (それぞれ $N$ に含まれる) の自由格子とする。明らかに$N : M \supset Q : P$。ここで、$Q : P$ が $\mathrm{Hom}_A(P, Q)$ と同型であるのは明らかです。したがって、階数 $(\mathrm{rg}_A P)(\mathrm{rg}_A Q)$ の自由A-加群 (*代数*, 章 II, § 1, no. 6, 系 1 から命題 6) したがって、格子は $\mathrm{Hom}_K(V, W)$ になります。同様に、$P'$ (それぞれ $Q'$) が $M$ (それぞれ含む $N$) に含まれる $V$ (それぞれ $W$) の自由格子である場合、$Q' : P' \supset N : M$ と $Q' : P'$ は$\mathrm{Hom}_K(V, W)$の格子。 よって結論。

*注意*
(2) 命題 3 (i) は、$V$ の格子の集合 $R(V)$ が包含に関して *格子順序付け* されていることを示します。さらに、$M$が$V$の固定格子である場合、$x$が$K^*$、$R(V)$の形部分集合を通過する$xM$は、*coinitial*と*cofinal*の両方です(*集合) 理論*、章 III, § 1, no. 7)。

(3) 命題 3(iv)の記法において、標準写像
$$
N : M \to \mathrm{Hom}_A(M, N),
$$
$f|_M$ と同じグラフを持つ $M$ から $N$ までの K-線型写像 $f \in N : M$ から A-線型写像までのすべての写像は *全単射 * であり、すべての A-線型写像 $g : M \to N$ は K-線型写像に埋め込むことができます
$$
g \otimes 1 : M \otimes_A K \to N \otimes_A K
$$

そして、$M \otimes_A K$ と $N \otimes_A K$ はそれぞれ $V$ と $W$ と同一視されていることがわかります。

特に、$W = K$、$N = A$、$\operatorname{Hom}_K(V, W)$ は、$V$ と $A$ の *二重ベクトル K 空間* $V^*$ です: $M$ は *二重 A-加群* と識別されます$M$中$M^*$;今後この識別を行い、$M^*$ は $M$ の *二重格子* であると言うことにします。つまり、* $x^* \in V^*$ の *集合です。 *そのような* $\langle x, x^* \rangle \in A$ *すべて* $x \in M$。

#### 系 {#ac-vii-s4-n1-cor-2 .statement tag=0533}

*U、V、W を K および f 上の有限階数の 3 つのベクトル空間とします: U × V → W は左の非縮退 K 双線形写像* (代数, 章 IX, § 1, no. 1, 定義 3)。 *M が V の格子であり、N が W の格子である場合、集合 N: ,M of x ∈ U thatf (x, y) ∈ N for ally ∈ M は U* の格子です。

$s_f: U \to \operatorname{Hom}_K(V, W)$ を K-線型写像と $f$ (代数, 章 IX, *loc. cit.*) に関連付けたままにし、$s_f(x)$ が線形写像 $y \mapsto f(x, y)$ になるようにします。 $f$ が非縮退のままであるということは、$s_f$ が *単射的*であることを意味することを思い出してください。 命題 3 (iv) により、$N: M$ は $\operatorname{Hom}_K(V, W)$ の格子になります。 $N: fM = s_f^{-1}(N: M)$ と $s_f$ は単射なので、系は命題 3 (ii) から続きます。

*例*

(4) $S$ を、有限階数と単位元の (必ずしも結合するわけではない) K-代数とします。この場合、$S \times S$ から $S$ への双線形マッピング $(x, y) \mapsto xy$ は (左と右) 非縮退です。 $M$ と $N$ が $A$ に関して $S$ の格子である場合、$x \in S$ の $M.N$ (命題 3 (iii)) と集合も同様であり、$xM \subset N$ (系から命題 3）。 $S$の*格子*である$S$の$S$含む単位元の*部分A代数*が存在することに注意してください。 $S$ の基底 $(e_i)_{1 \leq i \leq n}$ を考えて、$e_1$ が $S$ の単位元であり、$e_i e_j = \sum_k c_{ijk} e_k$ が $S$ ($1 \leq i \leq n, 1 \leq j \leq n$) の乗法表であるとします。 *したがって* $c_{1jk} = \delta_{jk}, c_{i1k} = \delta_{ik}$ (クロネッカー記号)。 $s \in A$ をゼロ以外とし、添字 $(i, j, k)$ のすべての三つ組に対して $c'_{ijk} = s \cdot c_{ijk} \in A$ となるようにします。 $i \geq 2$ を $e'_i = s^{-1} e_i$ と書くと、

$$
e'_i e'_j = s c'_{ij1} e'_1 + \sum_{k \geq 2} c'_{ijk} e'_k
$$

$i \geq 2$ と $j \geq 2$ の場合。 基底 $e_1$ を伴う $S$ の格子と $e'_i$ ($2 \leq i \leq n$) は単位元 $e_1$ を伴う $S$ の部分 A 代数です。

(5) $V$ を $K$ 上の有限次元ベクトル空間とし、$f$ を$V$ 上の非縮退双線形形式とします。 $M$ が $V$ の格子である場合、系から命題 3 まで、$x \in V$ の集合 $M^*_f$ が続き、味方 $\in M$ の $f(x, y) \in A$ も $V$ の格子になります。 $s_f: V \to V^*$ が線形写像と $f$ (全単射) に関連付けられたままの場合、$s_f(M^*_f)$ は単に $M$ の二重格子 $M^*$ です。

#### 命題 4 {#ac-vii-s4-prop-4 .statement tag=0534}

*B を整域、A を B と K の部分環、A と B のそれぞれの体と分数をL とします。V を K 上の有限次元ベクトル空間とします。

(i) $A$ に関する$V$ の各格子 $M$ について、$V_{(L)} = V \otimes_K L$ の$M_{(B)} = M \otimes_A B$ の像 $BM$ は、$B$ に関して$V_{(L)}$ の格子です。

(ii) さらに、$B$ がフラットな $A$ モジュールであると仮定します。すると、標準写像 $M_{(B)} \to BM$ は全単射です。さらに$B$が忠実に平坦であれば、$A$に関する$V$の各格子$M$から$B$に関する$V_{(L)}$の格子$BM$まで写像を加えた写像は単射的です。

(i) $KM = V$ として、明らかに $L . (BM) = V_{(L)}$;一方、$M$ は、$V$ の有限生成されたサブ$A$ モジュール $M_1$ に含まれているため、$BM$ は有限生成された $B$ モジュールである $BM_1$ に含まれます。 よって主張 (i) (命題 1)。

(ii) $V_{(L)} = V \otimes_K L = V \otimes_A L$ (章 II, § 2, no. 7、命題 18)、$L$ はフラット $B$ モジュールであるため、フラット $A$ モジュール (章 I, § 2, no. 7、系 3 ～ 命題 8）。 $B$ はフラットな $A$ 加群であるため、標準写像 $M \otimes_A B \to V \otimes_A B$ は単射的です。一方、$V$ はフリーの $K$ モジュール、$K$ はフラット $A$ モジュールであるため、$V$ はフラット $A$ モジュール (章 I, § 2, no. 7、系 3 ～ 命題 8) であり、したがって、標準写像 $V \otimes_A B \to V \otimes_A L$ は単射法であり、最初の主張が確立されます。 また、$B$ が忠実に平坦な $A$ 加群である場合、関係 $BM_1 = BM_2$ は、$A$ に関して $V$ の 2 つの格子 $M_1, M_2$ に対して $M_1 = M_2$ を意味し、注意が最初に $BM_1 \cap BM_2 = B(M_1 \cap M_2)$ であることを確認します。 (章 I, § 2, no. 6、命題 6);したがって、$M_1 \subset M$ と、主張が章 I, § 3, no. 1、命題 3 から標準単射 $M_1 \to M_2$ に適用される場合に注意を限定することができます。

#### 系 {#ac-vii-s4-n1-cor-3 .statement tag=0535}

$A$ が離散評価環であると仮定します。 $\hat{A}$ をその完了とし、$\hat{K}$ を $\hat{A}$ (章 VI, § 5, no. 3) の分数の体とします。 $\hat{A}$ に関して $V$ のすべての格子 $M$ を $\hat{V} = V \otimes_K \hat{K}$ の格子 $\hat{A}M$ にマッピングするマッピング $\phi$ は全単射であり、その逆マッピングは $\hat{A}$ に関して $\hat{V}$ のすべての格子 $M'$ をその交点にマッピングします。 $M' \cap V$ ($V$ は、$\hat{V}$ のベクトルサブ K 空間で正規に識別されます)。

If $L$ is a free lattice of $V$, the lattices $aL$ (for $a \in A, a \neq 0$) form a fundamental system of neighbourhoods of 0 for a topology $\mathscr{T}$ on $V$ (compatible with its $A$-module structure), which (when a basis of $L$ over $A$ is taken) is identified with the product topology on $K^n$); by virtue of Proposition 2, a fundamental system of neighbourhoods of 0 for $\mathscr{T}$ also consists of all the lattices of $V$ with respect to $A$; clearly $\hat{V}$ is the completion of $V$ with respect to $\mathscr{T}$. さらに、$m$が$A$の最大理想である場合、$M$は有限生成された$A$加群であるため、トポロジー$\mathscr{T}$は、$A$に関して$V$のすべての格子$M$に$m$進トポロジーを誘導します。 (III, § 3, no. 2 章、定理 2) および $\hat{A}M$ は、このトポロジーに関する $M$ の完成です (III, § 2, no. 12 章、命題 16)。さらに、$M$ が $V$、$\hat{A}M \cap V = M$ で開いている (したがって閉じている) ため、これは、$\dagger$ が単射であるという事実を再度証明します (これは、$A$ が忠実に平坦な $A$ 加群であるため、命題 4 (ii) から直接続きます)。 Finally, if $M'$ is a lattice of $\hat{V}$ with respect to $\hat{A}$, $M = M' \cap V$ is a lattice of $V$ with respect to $A$, for every element of $\hat{A}$ is the product of an element of $A$ and an invertible element of $\hat{A}$ and hence it follows from Proposition 2 that there exist $a, b$ in $A - \{0\}$ such that $a \hat{A}L \subset M' \subset b \hat{A}L$, whence $aL \subset M' \cap V \subset bL$. さらに、$M'$は$V$で開いており、$V$は$\hat{V}$で密集しているため、$M'$は$M' \cap V = M$の完了です。これは、$\phi$ が全射、よって系であることを証明します。

例 (6) $S$ を、含む 0 ではなく、$A$ の乗算部分集合とします。私たちは命題を適用する 4から$B = S^{-1}A$です。次に$L = K$、$BM = S^{-1}M$。したがって、$S^{-1}M$は$S^{-1}A$に関して$V$の格子です。さらに：

#### 命題 5 {#ac-vii-s4-prop-5 .statement tag=0536}

*有限階数の$V, W$ベクトル空間を$K$、$M$を$V$の格子、$N$を$W$の格子とします。 $M$ が有限生成される場合、(命題 3 の記法):*

(1)
$$
S^{-1}(N : M) = S^{-1}N : S^{-1}M
$$
* $\operatorname{Hom}_K(V, W)$ で。

(1) の左辺が右辺に含まれていることは明らかです。逆に、$f \in S^{-1}N : S^{-1}M$ と $(x_i)_{1 \leq i \leq n}$ を $M$ の生成元の系とします。すべての $i$ に対して $f(x_i) \in s^{-1}N$ となるような $s \in S$ が存在するため、$sf \in N : M$ となり、命題が証明されます。

### 2. 二元性。反射的加群

これ以降、領域 $A$ は *ネーター で完全に閉じている* と仮定し、 $P(A)$ (または単に $P$) は *高さ* 1 の $A$ の素イデアルの集合を表すことを思い出してください。 $A$ に関するすべての格子は *有限生成* されます$A$-モジュール (no. 1、系 ～ 命題 1)。

$V$ を $K$ 上の有限階数のベクトル空間とし、$V^*$ を双対、$V^{**}$ を双対とします。 標準写像 $c_V$ (*代数*, 章 II, § 7, no. 5, 定理 6) によって同一視する $V$ と $V^{**}$ を実行します。 $M$ を $V$ の格子とします。 $M$ の二重 $A$ モジュール $M^*$ は、すべての $x \in M$ に対して $\langle x, x^* \rangle \in A$ となるように、$M$、$x^* \in V^*$ の集合の *二重格子* で標準的に識別されることを思い出してください。したがって、$M$ の *双対* $A$ モジュール $M^{**}$ は、含む $M$ である $V$ の *格子* です。 さらに、$M^{***} = M^*$ は、関係 $M \subset M^{**}$ に対して、$(M^{**})^* \subset M^*$ を暗示し、逆に$M^* \subset (M^*)^{**}$ を上記により暗示します (cf. *集合理論*, 章 III, § 1, no. 5, 命題 2)。

$p$ が素イデアルである場合、命題 5 に $N = A$ を適用すると関係 $(M^*)_p = (M_p)^*$ が得られ、両方の項に対して記法 $M_p^*$ が正当化されます。

#### 定理 1 {#ac-vii-s4-thm-1 .statement tag=0537}

*$M$ が $V$ の格子である場合、* $M^* = \bigcap_{p \in P} M_p^*$ になります。

明らかに、$M_p^*$ のそれぞれに $M^*$ が含まれています。逆に、$x^* \in \bigcap M_p^*$ とします。 $x \in M$ の場合、$\langle x, x^* \rangle \in \bigcap_{p \in P} A_p$、そして $A = \bigcap_{p \in P} A_p$ (§ 1, no. 6、定理 4) のように、$x^* \in M^*$。

定理 1 を $M^*$ に適用すると、$M^{**} = \bigcap_{p \in P} M_p^{**}$ が示されます。しかし、$A$ は主イデアル整域 ($§ 1$、no. **6**、定理 **4**)、$M$ は有限生成された無料の $A$ モジュールであるため、$M_p^{**}$ は正規的に $M$ と識別されます。 (*代数*、章 II、$§ 2$、番号 **7**、命題 **14**)、よって系。

$A$、標準写像 $c_M : M \to M^{**}$ (*代数*、章 11、$§ 2$、番号 **7**) に関する任意の格子 $M$ については、元 $x \in M$ をそれ自体と同定します。 $x$ は、$M^*$ 生成する $V^*$ 以降、すべての $x^* \in M^*$ に対して $\langle x, x^* \rangle = \langle y, x^* \rangle$ となる、$V = V^{**}$ の一意元 $y$ です。 $M^{**} = M$ の場合、$M$ は *再帰的* であると言えます (*loc. cit.*)。上の $M^* = (M^*)^{**}$ のように、任意の格子 $M$ の *双対* は常に *再帰的*であることがわかります。

#### 注意 (1) {#ac-vii-s4-n2-rem-1 .statement tag=0538}

$M$ を有限生成された $A$ モジュールとします。 $\operatorname{Hom}_A(M, K)$のサブ$A$モジュールで識別される$M$の双対$M^*$がベクトル$K$空間$\operatorname{Hom}_A(M, K)$の*格子*であることは明らかです。特に、有限に生成されたすべての*再帰* $A$-加群は、適切なベクトル $K$-空間の格子に同型です。

#### 定理 2 {#ac-vii-s4-thm-2 .statement tag=0539}

*$M$ が $V$ の格子である場合、*次の条件は同等*:
(a) $M$ *再帰的*です。
(b) $M = \bigcap_{p \in P} M_p$。
(c) $\operatorname{Ass}(V/M) \subset P$。

(a) と (b) の同値は、系から定理 1 に続きます。(b) が当てはまる場合、$V/M$ は積 $\prod_{p \in P} (V/M_p)$ のサブ$A$ モジュールで正規に識別されます。しかし実際には、それは *直和* $\bigoplus_{p \in P} (V/M_p)$ に含まれています: $L \subset M$ が自由格子であり、$L$ の $(e_i)_{1 \leq i \leq n}$ 基底の場合、$(e_i)$ に関する点 $x \in V$ の各座標 $x_i$ 属する ～ $A$ ただし、$p \in P$ の値の有限の数を除きます。 関係 $V/M \subset \bigoplus_{p \in P} (V/M_p)$ は次のことを意味します。

$$
\operatorname{Ass}(V/M) \subset \bigcap_{p \in P} \operatorname{Ass}(V/M_p).
$$

$V/M_p$ は $A_p$ モジュールであるため、$A - p$ の元は $A$ で反転可能であるため、$A - p$ できないの元は $V/M_p$ の元 $\neq 0$ を消滅させます。したがって、$\operatorname{Ass}(V/M_p)$ の元は $p$ に含まれ、$V/M_p$ は捩れ $A$ モジュールであるため、$\neq 0$ になります。 $p$ の高さは **1** であるため、$V/M_p \neq (0)$ の場合は必然的に $\operatorname{Ass}(V/M_p) = \{ p \}$、$V/M_p = (0)$ の場合は $\operatorname{Ass}(V/M_p) = \varnothing$ になります。したがって$\operatorname{Ass}(V/M) \subset P$です。

最後に、条件 (c) が成立する場合、

$$
\operatorname{Ass}(M^{**}/M) \subset \operatorname{Ass}(V/M) \subset P.
$$

一方、$p \in P$ の場合、系から定理 1 の証明で、$M_p^{**} = M_p$、よって $p \notin \operatorname{Ass}(M^{**}/M)$ (章 IV、$§ 1$、no. 3、 系 1 ～ 命題 7)。 結論する Ass(M**/M) = ∅, よって M** = M (章 IV, § 1, no. 1, 系 1 から命題 2) となります。

#### 系 {#ac-vii-s4-n2-cor-1 .statement tag=053A}

M、N を、N が再帰的となるように、A に関して V の 2 つの格子とする。 M ⊂ N である位数において、すべての p ∈ P について M_p ⊂ N_p であることが必要かつ十分です。

条件は明らかに必要であり、それが満たされると、

$$
\bigcap_{p \in P} M_p \subset \bigcap_{p \in P} N_p = N.
$$

M ⊂ M** = \bigcap_p M_p なので、確かに M ⊂ N です。

例
(1) すべての自由格子は再帰的です。
(2) V = K とします。K の分数イデアル a が再帰格子であるためには、定理 2、§ 1, no. 4、命題 5、7 の基準 (b) により、それが除数イデアルであることが必要かつ十分です。
(3) M を A に関する格子とします。 S が含む 0 ではなく A の乗法部分集合である場合、no. 1 の命題 5 は S^{-1}(M*) = (S^{-1}M)* であることを示します。 M が再帰的であれば、S^{-1}M は S^{-1}A に関する再帰格子になります。

#### 命題 6 {#ac-vii-s4-prop-6 .statement tag=053B}

(i) M_1 と M が V の再帰格子であれば、M, n M も同様です。
(ii) W が V のベクトル部分空間で、M が V の再帰格子である場合、M n W は W の再帰格子です。
(iii) V, W を、K および M (それぞれ N) 上の有限階数の 2 つのベクトル空間、V (それぞれ W) の格子とします。 N が再帰的である場合、Hom_K(V, W) (no. 1, 命題 3) の格子 N: M は再帰的です。

(i) すべての p ∈ P (章 II, § 2, no. 4, 定理 1) に対して (M, n M_2)_p = (M_1)_p n (M_2)_p。 M_1 = \bigcap_{p \in P} (M_1)_p かつ M_2 = \bigcap_{p \in P} (M_2)_p の場合、

$$
M, n M_2 = \bigcap_{p \in P} (M, n M_2)_p
$$

よって定理 2 による結論。
(ii) 同様に (M n W)_p = M_p n W_p = M_p n W、よって

$$
M \cap W = \bigcap_{p \in P} (M \cap W)_p,
$$

これは(ii)を証明します。
(iii) M は有限に生成されるため、no. 1, 命題 5 から、(N: M)_p = N_p M_p となります。さらに、 関係 N = \bigcap_{p \in P} N_p は次のことを意味します。

$$
N: M = \bigcap_{p \in P} (N_p : M_p).
$$

$f \in \bigcap_{p \in P} (N_p : M_p)$ と $x \in M$ の場合、$f(x) \in \bigcap_{p \in P} N_p = N$、よって $f \in N : M$;これは、$N : M$ が再帰的であることを示しています。

Remarks
(2) If $M_1$ and $M_2$ are reflexive lattices of $V$, the lattice $M_1 + M_2$ is not necessarily reflexive (cf. § 1, Exercise 2).
(3) If $M$ is a finitely generated $A$-module and $T$ its torsion submodule, the dual $M^*$ of $M$ is the same as the dual of $M/T$, since, for every linear form $f$ on $M$, the image $f(T)$ is a torsion submodule of $A$ and hence zero. $M/T$ は $K$ 上のベクトル空間の格子と同型であるため、有限に生成されたすべての $A$ 加群の双対は再帰的であることがわかります。

#### 命題 7 {#ac-vii-s4-prop-7 .statement tag=053C}

$0 \to M \to N \to Q \to 0$ を $A$ モジュールの完全系列とします。 $N$ が有限に生成され、ねじれがないと仮定します。
(i) $M$ が再帰的である場合、$\operatorname{Ass}(Q) \subset P \cup \{\{0\}\}$ (他の語では、$Q$ に関連付けられたすべての理想は、$(0)$ または高さ 1 のいずれかになります)。
(ii) 逆に、$N$ が再帰的で、$\operatorname{Ass}(Q) \subset P \cup \{\{0\}\}$ の場合、$M$ は再帰的です。

$A$ はネーター であるため、$M$ も有限生成されます。 $V = M_{(K)}$、$W = N_{(K)}$、$M$ (それぞれ $N$) は、$V$ (それぞれ $W$) (no. 1, 命題 1) の格子で正規識別されます。 2 つの完全系列について考えてみましょう。
$$
0 \to V/M \to W/M \to W/V \to 0 \\
0 \to Q \to W/M \to W/N \to 0.
$$
(i) 次のように推測します (章 IV, § 1, no. 1, 命題 3):
$$
\operatorname{Ass}(Q) \subset \operatorname{ASS}(W/M) \subset \operatorname{ASS}(V/M) \cup \operatorname{ASS}(W/V).
$$
$M$ が再帰的であれば、$\operatorname{Ass}(V/M) \subset P$ (定理 2)。一方、$\operatorname{Ass}(W/V)$ は明らかに空であるか、$\{0\}$ に減らされています。 よって (i)。
(ii) 同様に:
$$
\operatorname{Ass}(V/M) \subset \operatorname{Ass}(W/M) \subset \operatorname{Ass}(Q) \cup \operatorname{Ass}(W/N).
$$
したがって、仮説は $\operatorname{Ass}(V/M) \subset P \cup \{\{0\}\}$ を意味します。しかし、$V/M$ は捩れ $A$ モジュールであるため、$\{0\} \notin \operatorname{Ass}(V/M)$ です。 定理 2 は、$M$ が再帰的であることを示します。

#### 命題 8 {#ac-vii-s4-prop-8 .statement tag=053D}

$R$ と $S$ を 2 つの可換環、$p : R \to S$ 環準同型および $M$ を有限生成された $R$ モジュールとします。 $R$ がネーター で、$S$ がフラット $R$ モジュールであると仮定します。次に、$M$ が再帰的である場合、$S$ モジュール $M_{(S)} = M \otimes_R S$ も再帰的です。
私たちは (章 I, § 2, no. 10, 命題 11) 標準同型 $\omega_M : (M^*)_{(S)} \to (M_{(S)})^*$ が存在することを知っています。
$$
\langle x \otimes 1, \omega_M(x^* \otimes 1) \rangle = \rho(\langle x, x^* \rangle)
$$

€または x \in M、x^* \in M^*。 M は有限生成された自由 R 加群 L の商であるため、M* は双対 L* のサブ R 加群と同型であり、L* は自由で有限生成されます。 $\mathbf{R}$ はネーター であるため、M* も有限生成された R 加群よって同型 $\omega_{M^*}: (M^{**})_{(S)} \to ((M^*)_{(S)})^*$ です。

$$
\langle x^* \otimes 1, \omega_{M^*}(x^{**} \otimes 1) \rangle = \rho(\langle x^*, x^{**} \rangle)
$$

$x^* \in M$ と $x^{**} \in M^{**}$ の場合。一方、合成標準同型による同型 $^t\omega_M: (M_{(S)})^{**} \to ((M^*)_{(S)})^*$、よってがあります。

$$
\phi = (t\omega_M^{-1}) \circ (\omega_{M^*}): (M^{**})_{(S)} \to (M_{(S)})^{**}
$$

上記記法では次のようになります。

(1)

$$
\langle \omega_M(x^* \otimes 1), \phi(x^{**} \otimes 1) \rangle = \rho(\langle x^*, x^{**} \rangle).
$$

ここで標準準同型 $c_M: M \to M^{**}$ を検討し、合成準同型が次のようになることを示します。

(2)

$$
\psi: M_{(S)} \xrightarrow{c_M \otimes 1} (M^{**})_{(S)} \longrightarrow (M_{(S)})^{**}
$$

ちょうど標準準同型 $c_{M_{(S)}}$ です。これは (1) からすぐに続き、 関係が得られます。

$$
\langle \omega_M(x^* \otimes 1), \psi(x \otimes 1) \rangle = \rho(\langle x^*, c_M(x) \rangle)
$$
$$
= \rho(\langle x, x^* \rangle) = \langle x \otimes 1, \omega_M(x^* \otimes 1) \rangle
$$

そして元 $\omega_M(x^* \otimes 1)$ 生成する $(M_{(S)})^*$ という事実から。そうなると、M が再帰的であるという仮定は、$c_M$ が全単射であることを意味し、したがって $c_M \otimes 1$ も同様であり、したがって $\psi = c_{M_{(S)}}$ は全単射であり、これは命題を示します。

### 3. 再帰的加群のローカル構成

記法と no. 2 の仮説を保持します。 $p \in P$ の集合が *有限* ではない場合、性質は *ほぼすべて* $p \in P$ に当てはまります。

#### 定理 3 {#ac-vii-s4-thm-3 .statement tag=053E}

*Vを、Aに関してVのKおよびM格子上の有限階数のベクトル空間とします。

(i) *N を A に関してV の格子とする。この場合、A のすべての素イデアル p について、$N_p$ は A に関して V の格子であり、ほぼすべて* $p \in P, N_p = M_p$ です。

(ii) *逆に、A に関して * V のすべて* $p \in P$ *格子* $N(p)$ について、* $N(p) = M_p$ * ほぼすべて* $p \in P$ が得られると仮定します。 *すると* $N = \bigcap N(p)$ *はAに関するAの再帰格子であり、それは* $N'_p = N(p)$ *すべて* $p \in P$となるようなAに関する*Vの唯一の再帰格子* $N'$です。

(i) 最初の主張は no. 1, 命題 4 から続きます。さらに、$\mathbf{K}^*$ には $xN \subset M \subset yN$ (no. 1, 命題 2) のように $x, y$ が存在します。ほぼすべての $p \in P, v_p(x) = v_p(y) = 0$ ($§ 1$、no. 6、定理 4) について、これは、$x$ と $y$ が $A$ で反転可能であること、つまり $M_p = N_p$ で反転可能であることを示しています。

(ii) $A$ の $x \neq 0$ を $x^{-1}M$ までに置き換える $M$ とし、すべての $p \in P$ について $N(p) \subset M$ と仮定します。 $p_1, \ldots, p_h$ を $P$ の元とし、$N(p) = M$ を、$p$ は $p_i$ ($1 \leq i \leq h$) とは区別します。私たちはこう書きます：

$$
Q = M \cap N(p_1) \cap \cdots \cap N(p_h).
$$

$N(p_i)$ 含むはそれぞれ $A_{p_i}$ に関して自由格子であるため、含む *なおさら* $A$ に関しては $V$ の格子であるため、$Q$ 含むは$A$ に対して$V$ (no. 1, 命題 3)、$Q$ が$M$ に含まれるため、$Q$ は$A$ に対して格子になります。すべての $p \in P$ に対して $Q_p = N(p)$ であることを証明するには、次の補題を使用します。

#### 補題 1 {#ac-vii-s4-lem-1 .statement tag=053F}

*$p$ と $p'$ を $A$ の 2 つの素イデアルとし、(0) が $p \cap p'$ に含まれる $A$ の唯一の素イデアルであるとします。次に、$V$ のサブ A モジュール $E$ ごとに、$(E_p)_{p'} = K.E.$*

$S$ を $A$ の乗算部分集合 $(A - p)(A - p')$ とします。 章 II、$§ 2$、no. 3、命題 7、$(E_p)_{p'} = S^{-1}E$ による。さらに、$A \subset S^{-1}A \subset K$; $S^{-1}A$ 対応するの主イデアルから $A$ の主イデアル $q$ へ、$q \cap S = \varnothing$ (章 II, $§ 2$, no. 5, 命題 11) となります。 仮定 (0) は、$S$ を満たさない、$A$ の唯一の主要な理想です。したがって、$S^{-1}A = K$ と $S^{-1}E = K.E.$

(ii)の証明に戻ります。 $p \in P$ が $p_i$ ($1 \leq i \leq h$) と異なる場合、$p_i$ と $p$ の高さは 1 であるため、補題 1 を $N(p_i)$ に適用すると、$((N(p_i))_{p_i})_p = (K.N(p_i))_p = V$ が得られます。

$$
Q_p = M_p \cap (N(p_1))_p \cap \cdots \cap (N(p_h))_p = M_p = N(p)
$$

(章 II、$§ 2$、no. 4)。一方、$p$ が $p_i$ ($1 \leq i \leq h$) に等しい場合、上記の引数と$(N(p_i))_{p_i} = N(p_i)$、よってにより、$i \neq j$ に対して $(N(p_i))_{p_j} = V$

$$
Q_{p_i} = M_{p_i} \cap N(p_i) = N(p_i).
$$

したがって、すべての $p \in P$ に対して $Q_p = N(p)$ であることが証明されました。それから

$$
N = Q^{**} = \bigcap_{p \in P} Q_p
$$

再帰的であり、すべての $p \in P$ に対して関係 $N_p = Q_p = N(p)$ を満たします。 一意性性質は、no. 2 の定理 2 の直後に続きます。

#### 注意 {#ac-vii-s4-n3-rem-1 .statement tag=053G}

$L$を$A$に関する$V$の自由格子とします。 $A_p$ は $p \in P$ の主イデアル整域であるため、$N(p)$ は $L$ と同じ階数の空き $A$ モジュールであり、$u(p)(L_p) = N(p)$ のような $u(p) \in \mathbf{GL}(V)$ が存在します。この条件さらに決定する $u(p)$ を $\mathbf{GL}(L_p)$ の元までに右乗法内に移動します。 ほぼすべての $p \in P$ に対して条件 $N(p) = L_p$ は、ほぼすべての $p \in P$ に対して必然的に $u(p) \in \mathbf{GL}(L_p)$ であることを意味します。 家族 $(u(p))_{p \in P}$ 満たす後者性質形乗法群 $\mathbf{GL}_a(V)$ 含むとして部分群積 $\prod_{p \in P} \mathbf{GL}(L_p)$ 。 次に、定理 3 は、V の再帰格子の *集合が同次の空間* $\mathbf{GL}_a(V)/\prod_{p \in P} \mathbf{GL}(L_p)$ と正準 1 対 1 対応であることを示します。 A 上の L の基底 $(e_i)_{1 \leq i \leq n}$ が選択された場合、$\mathbf{GL}(V)$ (それぞれ $\mathbf{GL}(L_p)$) は可逆行列 $\mathbf{GL}(n, K)$ (それぞれ $\mathbf{GL}(n, A, )$) のグループと識別され、グループ $\mathbf{GL}_a(V)$ は次数 $n$ の行列系のグループと識別されます。 $(U(p))_{p \in P}$、つまり、すべての $p \in P$ に対して $U(p) \in \mathbf{GL}(n, K)$ が、ほぼすべての $p \in P$ に対して $U(p) \in \mathbf{GL}(n, A_p)$ になります。 A がデデキント ドメインの場合、群 $\mathbf{GL}_a(V)$ は群 $\mathbf{GL}(n, A)$ とも識別されます。ここで、A は制限付きアデル ($§ 2$、no. 4) の環です。

### 4. 擬似同型性

記法と no の仮説を保持します。 2と3。

#### 命題 9 {#ac-vii-s4-prop-9 .statement tag=053H}

※Mを有限生成A-加群とします。次の条件は同等です*:

(a) $M_p = 0$ は、身長 $\leq 1$ の *すべての素数イデアル* $p$ を表します。
(b) *消滅子* $a \triangleleft M$ *は理想* $\neq (0)$ *および* $A : a = A$ (*A*: $a$ は、$§ 1$、no. 1、*集合の* $x \in K$ *そのような* $xa \in A$)。

(章 II, $§ 2$, no. 2, 系 2 ～ 命題 4) 条件 $M_p = 0$ は $a + p$ と等価であるため、$aA_p = A$、(章) と同等であることがわかります。 II、$§ 2$、no. 5、*注意*);一方、A のすべての整数イデアル $b \neq 0$ について、関係 "*$bA_p = A$、すべての $p \in P$*" は、$D(A)$ ($§ 1$、no. 4、命題 7) の $\operatorname{div} b = \operatorname{div} A = 0$、または $\operatorname{div}(A : b) = 0$ と等価です。そして、$A : b$ は約数 ($§ 1$、no. 1、命題 1) であるため、この関係も $A : b = A$ と等価です。次に、命題は、$p = (0)$ に対して $a \notin p$ は $a \neq (0)$ を意味することに注意します。

#### 注意 (1) {#ac-vii-s4-n4-rem-1 .statement tag=053I}

命題 9 に相当する条件は、$\operatorname{Ass}(M)$ 含むの身長$\leq 1$ の主な理想がないことも意味します。 *これらは、* $\operatorname{Supp}(M)$ *共次元* である* $\geq 2$ *in* $\operatorname{Spec}(A)$ とというによって解釈される場合もあります。 \*

#### 定義 2 {#ac-vii-s4-def-2 .statement tag=053J}

*A-加群 M は、有限に生成され、命題 9 と同等の条件を満たす場合、擬似ゼロと呼ばれます。*

この定義と命題 9 は、擬似ゼロ A-加群が *捩れ A-加群* であることを示しています。 逆は誤りです。

*例*
(1) A がデデキント領域である場合、A のすべての素イデアルの高さは $\leq 1$ です。 M が擬似ゼロであるということは、$\operatorname{Supp}(M) = \varnothing$ を意味し、したがって $M = 0$ (章 11, $§ 4$, no. 4) を意味します。

(2) 2 つの不定数で $k$ を体および $A = k[X, Y]$ 多項式環 $k$ とする。 $m$ が $A$ の最大理想値 $AX + AY$ である場合、$A$ 加群 $A/m$ は擬似ゼロです。なぜなら、その消滅子 $m$ は、含むの主要な素数理想$AX$ と $AY$ と異なるため、$\leq 1$ の高さではありません。したがって、$A : m = A$ (§ 1, no. 6、系 1 ～ 定理 3) となります。

#### 定義 3 {#ac-vii-s4-def-3 .statement tag=053K}

*$M$ と $N$ を 2 つの $A$ モジュールと $f : M \to N$ 準同型とします。 $\mathrm{Ker}(f)$ (それぞれ $\mathrm{Coker}(f)$、$\mathrm{Im}(f)$) が擬似ゼロの場合、$f$ は擬似単射的 (擬似全射的擬似ゼロ) と呼ばれます。 $f$ が疑似単射と疑似全射の両方である場合、疑似全単射と呼ばれます。*

擬似全単射準同型は *擬似同型* とも呼ばれます。

$M$ と $N$ が有限に生成されると仮定します。その場合、$f : M \to N$ が擬似単射 (それぞれ擬似全射、擬似ゼロ) であるためには、すべての $p \in P \cup \{\{0\}\}$、$f_p : M_p \to N_p$ が単射 (それぞれ全射、零) であることが必要かつ十分です。これは、$A$ モジュール $A$ の平坦度 (cf. 章 I, § 2, no. 3, *注意 2*) から得られます。

*例 (3)* $M$ をねじれのない有限生成された $A$ 加群とする。その場合、その二双対に対する $M$ の標準写像 $c_M : M \to M^{**}$ は *擬似同型* です。 $M$ は $V = M \otimes_A K$ (no. 1, 命題 1) の格子で識別されます。すべての $p \in P$ (no. 2、例 2) については $M_p = M_p^{**}$ であり、$p = 0$、$M_p$、$M_p^{**}$ は両方とも $V$ に等しいことがわかりました。

#### 定理 4 {#ac-vii-s4-thm-4 .statement tag=053L}

*$E$ を、$E$ と $M = E/T$ の$T$ 捩れ部分加群の有限生成された $A$ モジュールとします。擬似同型性が存在します*

$$
f : E \to T \times M.
$$

まず 2 つの補題を示します。

#### 補題 2 {#ac-vii-s4-lem-2 .statement tag=053M}

*$(p_i)_{1 \leq i \leq k}$ を高さ 1 の $A$ の素イデアルの空でない有限族とし、$S = \bigcap_i (A - p_i)$ とします。その場合、環 $S^{-1}A$ は主イデアル整域になります。*

$S^{-1}A$ は半局所環であり、その最大イデアルは $1 \leq i \leq k$ に対する $m_i = p_i S^{-1}A$ であり、局所環 $(S^{-1}A)_{m_i}$ は $A$ と同型であり (第 11 章、§ 3, no. 5、命題 17)、したがって離散評価環となります。 したがって、環 $S^{-1}A$ は Dedekind ドメイン (§ 2, no. 2, 定理 1 (f)、そして準ローカルであるため主イデアル整域 (§ 2, no. 2, 命題 1) です。

#### 補題 3 {#ac-vii-s4-lem-3 .statement tag=053N}

*制限から $T$ がホモテティー であり、擬似同型である準同型 $g : E \to T$ が存在します。

$a$ を $T$ の消滅子とします。 $T$ は有限生成された捩れ $A$ モジュール、$a \neq 0$ であるためです。 $p_i$ ($1 \leq i \leq k$) を高さ 1 含む $a$ (数 ($§\ 1$, no. 6, 定理 4) で有限です) の主イデアルとします。この数が 0 の場合、T は擬似ゼロ (命題 9(a)) であり、$g = 0$ を取ることができます。それ以外の場合は、$S = \bigcap_i (A - p_i)$ とします。 補題 2 により、$S^{-1}A$ は主イデアル整域となるため、ねじれのない有限生成された $S^{-1}A$ モジュールである $S^{-1}M$ は *自由* (*代数*, 章 VII, §4, no. 3, 系 2)から定理 2) そして、$S^{-1}M = (S^{-1}E)/(S^{-1}T)$ として、$S^{-1}T$ は $S^{-1}E$ の直因子です (*代数*、章 II, §1, no. 11、命題 21)。今、

$$
\operatorname{Hom}_{S^{-1}A}(S^{-1}E, S^{-1}T) = S^{-1} \operatorname{Hom}_A(E, T)
$$

(章 II, §2, no. 7、命題 19);したがって、$s_0^{-1}g_0$ が $S^{-1}T$ 上で $S^{-1}E$ の射影子となるような $s_0 \in S$ と $g_0 \in \operatorname{Hom}_A(E, T)$ が存在します。 $h_0 \in \operatorname{Hom}_A(T, T)$ が $g_0$ から $T$ の制限を表す場合、すべての $x \in T$ に対して $s_1 h_0(x) = s_1 s_0 x$ となるような $s_1 \in S$ が存在します。したがって、$s = s_1 s_0$、$g = s_1 g_0$、$h = s_1 h_0$、$h$と書くと、$T$に対する比率$s$のホモテティーとなり、$g$対$T$の制限となります。 $h$ が擬似同型であることを検証する必要があります。ここで、$p = 0$ または $p \in P$ が $p_i$ ($1 \leq i \leq k$)、$T_p = 0$ (章 II, §4, no. 4、命題 17) と異なる場合、$h,\ : T_p \to T_p$ は同型です。逆に、$p$ が $p_i$ ($1 \leq i \leq k$) のいずれかに等しい場合、$s$ は $A$ で可逆であり、$T_{p_i}$ に対する$s$ の比率の$h_{,,}$、ホモテティー も同型、これで補題 3 の証明が完了します。

ここで、定理 4 を証明します。$g : E \to T$ を準同型満たすを補題 3 の性質とします。 $h$ を $g$ から $T$ までの制限とし、$x$ を $E$ から $M$ までの正規の射影とします。 準同型 $f = (g, x) : E \to T \times M$ が問題を解くことを示します。可換図式があります:

$$
\begin{array}{ccccccccc}
0 & \longrightarrow & T & \longrightarrow & E & \longrightarrow & M & \longrightarrow & 0 \\
& & \downarrow h & & \downarrow f & & \downarrow I_M & & \\
0 & \longrightarrow & T & \longrightarrow & T \times M & \longrightarrow & M & \longrightarrow & 0
\end{array}
$$

行は正確です。ヘビ図式 (章 I, §1, no. 4, 命題 2) は完全系列を与えます:

$$
0 \to \operatorname{Ker}(h) \to \operatorname{Ker}(f) \to 0 \to \operatorname{Coker}(h) \to \operatorname{Coker}(f) \to 0
$$

したがって、$\operatorname{Ker}(f)$ は $\operatorname{Ker}(h)$ および $\operatorname{Coker}(f)$ から $\operatorname{Coker}(h)$ と同型です。 $h$ は擬似同型写像であるため、$f$ も擬似同型写像です。

「擬似同型内に」 定理 4 簡約する有限生成された $A$ 加群の研究は、一方ではねじれのない加群の研究に、他方では捩れ加群の研究に至ると言うことができます。さらに、上記 (*例 3*) で、ねじりのない加群はその双双対、したがって *再帰的* 加群に対して擬似同型であることを見てきました。 捩れ加群については、擬似同型内で決定するとなる次の結果があります。

#### 定理 5 {#ac-vii-s4-thm-5 .statement tag=053O}

T を有限生成された捩れ A-加群とします。 2 つの有限族 $(n_i)_{i \in I}$ と $(p_i)_{j \in I}$ が存在します。ここで、$n_i$ は整数 $\geq 1$、$p_i$ は高さ 1 の $A$ の素イデアルであるため、$T' = \bigoplus_{i \in I} A/p_i^{n_i}$ と書くと、次の$T$ の擬似同型写像が存在します。 $T'$。 さらに、この性質を持つファミリー $(n_i)_{i \in I}$ と $(p_i)_{i \in I}$ は、インデックス付け集合と $T$ の $p_i$ 含む消滅子の全単射内に固有です。

一意性: If: $T \to T'$ は擬似同型写像であり、$p \in P, f_p : T, \to T'_p$ は同型です。さて、$T'_p$ は $A_p/p^{n_i}A_p$ の直和で、和は添字 $i$ を超えており、$p_i = p$ になります。したがって、$p^{n_i}A_p$ は捩れ $A$ モジュール $T$ の *基本因子* です (*代数*, 章 VII, § 4, no. 7)。彼らの一意性は *代数*、章 VII, § 4, no. 7、命題 7 で証明されました。

存在: $T \neq 0$ の場合に注意を限定することができます。 $a$ を、$T$、$p_i$ ($1 \leq i \leq k$) の消滅子 (ゼロではなく、$A$ とは異なる)、高さ 1 の$A$ 含む $a$ (数で有限である) とします。 ($§ 1$、no. 6、定理 4)) および $S = \bigcap_i (A - p_i)$。準局所リング $A' = S^{-1}A$ は主イデアル整域 (補題 2) であり、最大理想値 $m_i = p_iA'$ を持ちます。 $S^{-1}T$ は有限生成された捩れ $A$ 加群であるため、有限直和 $\bigoplus_{j \in I} A'/m_{\phi(j)}^{n_j}$ と同型です。ここで、$\phi$ は有限集合 $I$ の写像です。 $[1, k]$ (*代数*、章 VII, § 4, no. 7、命題 7); $A'/m_{\phi(j)}^{n_j}$ は $S^{-1}(A/p_{\phi(j)}^{n_j})$ (章 II, § 2, no. 4) と同型であるため、目的の型と同型 $f_0$ の捩れ $A$ モジュール $T'$ が得られました。 $S^{-1}T$から$S^{-1}T'$へ。 $\operatorname{Hom}_{S^{-1}A}(S^{-1}T, S^{-1}T')$ は $S^{-1} \operatorname{Hom}_A(T, T')$ (章 11, § 2, no. 7, 命題 19) に等しいので、$f_0 = s^{-1}f$ となる$s \in S$ と準同型 $f : T \to T'$ が存在します。 $f$ が擬似同型であることを示すのはまだ残っています。 さて、$p = 0$ または $p \in P$ が $p_i$, $T_p = T'_p = 0$ (章 II, § 4, no. 4, 命題 17) とは異なる場合、逆に、$p$ が $p_i$ ($1 \leq i \leq k$) の 1 つである場合、$s$ は $A_p$ で反転可能であり、$f_{p_i} = s(f_0)_{p_i}$ と $(f_0)_{p_i}$ が $T_{p_i} = (S^{-1}T)_{m_i}$ から $T'_{p_i} = (S^{-1}T')_{m_i}$ への同型であるように、同様です。 $f_{p_i}$。

#### 注意 (2) {#ac-vii-s4-n4-rem-2 .statement tag=053P}

定理 5 の主張では、加群 $A/p_i^{n_i}$ は $A/p_i^{(n_i)}$ ($§ 1$、no. 4、命題 8) に置き換えることができます。すべての $p \in P$、標準写像 $g : A/p^n \to A/p^{(n)} = A/(A \cap p^nA_p)$ は、すべての $q \in P$ が $p$、$A_q/p^nA_q = A_q/p^{(n)}A_q = 0$、および $A_p/p^nA_p = A_p/p^{(n)}A_p$ とは異なるのと同様に、擬似同型写像です。

\* $A$ モジュールの完全系列が与えられた場合、$E \to F \to G$、$E$ と $G$ が疑似ゼロであれば、定義 2 と章 II, §2, no. 4、定理 1 からわかるように、$F$ も同様です。カテゴリの言語で言えば、$A$ モジュールのカテゴリ $\mathscr{C}$ では、擬似ゼロ加群のサブカテゴリ $\mathscr{C}'$ が *full* であり、その後定義する *商* カテゴリ $\mathscr{C}/\mathscr{C}'$ になる可能性があります。このカテゴリ内のオブジェクトも同様です$A$ モジュールですが、$E$ から $F$ までの射の集合 ($\mathscr{C}/\mathscr{C}'$ の $E, F$ の場合) は、可換群の集合の直接の極限です。 $\mathrm{Hom}_A(E', F')$、ここで、$E'$ (それぞれ $F'$) は、$E$ の部分加群の集合 (それぞれ商加群の集合 $F$ の $F/F''$) を通過します。 $E/E'$ (それぞれ $F''$) は擬似ゼロです。もちろん、$A$ モジュール $E, F$ の注文された対ごとに、標準準同型 $\mathrm{Hom}_{\mathscr{E}}(E, F) \to \mathrm{Hom}_{\mathscr{E}/\mathscr{E}'}(E, F)$ が存在します。 準同型 $u \in \mathrm{Hom}_A(E, F)$ が擬似ゼロ (それぞれ擬似単射、擬似全射、擬似全単射) であるということは、$\mathrm{Hom}_{\mathscr{E}/\mathscr{E}'}(E, F)$ の標準像が零 (単写、準同型、同型) であることを意味します。 \*

### 5. 因子が捩れ加群に接続されました

nos と同じ記法と仮説を維持します。 2、3、4。 $D(A)$ (または単に $D$) が加法的に書かれた $A$ の *除数群* を表すことを思い出してください。 $D$ が $P$ の要素によって生成される自由な $\mathbf{Z}$ 加群であることがわかります (§ 1, no. 3、定理 2)。

$T$ を有限生成された捩れ $A$ モジュールとします。 すべての $p \in P$ に対して、$T_p$ は有限生成された捩れ $A_p$ モジュールであるため、*有限長* の加群 (章 IV, § 2, no. 5、系 2 ～ 命題 7)。この長さを$l_p(T)$と表記します。 Now $T_p = 0$ for all $p$ not containing the annihilator of $T$ and hence for almost all $p$ (§ 1, no. 6, Theorem 4), which justifies the following definition:

#### 定義 4 {#ac-vii-s4-def-4 .statement tag=053Q}

*$T$ が有限生成された捩れ $A$ モジュールの場合、因子:*

$$
\chi(T) = \sum_{p \in P} l_p(T) \cdot p.
$$

*は$T$*のコンテンツと呼ばれます。

#### 命題 10 {#ac-vii-s4-prop-10 .statement tag=053R}

(i) *$0 \to T_1 \to T_2 \to T_3 \to 0$ を、有限生成された捩れ $A$ モジュールの完全系列とします。それから*

$$
\chi(T_2) = \chi(T_1) + \chi(T_3).
$$

(ii) *擬似同型性$f : T_1 \to T_2$が存在する場合、$\chi(T_1) = \chi(T_2)$。*

(iii) *$\chi(T) = 0$の位数において、$T$が擬似ゼロであることが必要十分である*。

定義 4 を考慮すると、$l_p$ の各 $p \in P$ 値について、捩れ加群を考慮するだけで十分です。 性質 (i) は、章 II, § 2, no. 4、定理 1 と、完全系列 (*代数* 章 11、§ 1, no. 10、命題 16) における長さの加法性とプロパティから続きます。 (ii) と (iii) は、no. 4 の定義の直後に続きます。

#### 系 {#ac-vii-s4-n5-cor-1 .statement tag=053S}

*$0 \to T_n \to T_{n-1} \to \ldots \to T_0 \to 0$ を、有限生成された捩れ $A$ モジュールの完全系列とします。それから* $\sum_{i=0}^n (-1)^i \chi(T_i) = 0$。

章 II, § 2, no. 4、定理 1 を考慮すると、これは、$l_p$ の類似の性質 (*代数*、章 II, § 1, no. 10、系 3 から命題 16) に続きます。

(章 II, § 5, no. 4) を思い出してください。同型の関係に関して、*類の有限生成A-加群* の *集合* $F(A)$ について話すことができます。 有限生成A-加群 M ごとに、$\mathrm{cl}(M)$ が $F(A)$ の対応する元を表すものとします。有限生成された捩れ A-加群の $F(A)$ からなるの類を $T(A)$ 部分集合で表すことにします。 明らかに、$T(A)$ から $D(A)$ の $\chi$ 定義する写像は、$\chi$ によって示され、$\chi(\mathrm{cl}(T)) = \chi(T)$ になります。

#### 命題 11 {#ac-vii-s4-prop-11 .statement tag=053T}

*G を加法的に書かれた可換群と $\phi : T(A) \to G$ 写像とします。有限に生成されるすべての捩れ A-加群 T に対して、言葉の乱用により、$\phi(T) = \phi(\mathrm{cl}(T))$ とも書きます。次の条件が満たされるとします。
(1) *$0 \to T_1 \to T_2 \to T_3 \to 0$ *が有限生成された捩れ A-加群の完全系列である場合*、* $\phi(T_2) = \phi(T_1) + \phi(T_3)$。
(2) *T *が擬似ゼロの場合*、$\phi(T) = 0$。
*その後、一意な準同型* $\theta : D(A) \to G$ *そのような* $\phi = \theta \circ \chi$ が存在します。*

すべての p について $\chi(A/p) = p$ であるため、すべての $p \in P$ について必然的に $\theta(p) = \phi(A/p)$ となり、P の元形 $D(A)$ の基底から、$\theta$ の一意性が証明されます。逆に、$\theta$ を $D(A)$ から G までの準同型とし、すべての $p \in P$ に対して $\theta(p) = \phi(A/p)$ となり、問題が解けることを示します。このために、次のように書きます。

$$
\psi(T) = \phi(T) - \theta(\chi(T))
$$

有限に生成されたすべての捩れ A-加群 T;明らかに、条件 (1) と (2) は、$\phi$ が $\psi$ に置き換えられた場合にも満たされます。一方、$p \in P$の場合は$\psi(A/p) = 0$です。 p が素イデアル $\neq 0$ で P に含まれない場合、$A/p$ の消滅子は P のどのイデアルにも含まれないため、(no. 4, 定理 5) $A/p$ は擬似ゼロとなり、したがって $\psi(A/p) = 0$ になります。そうなると、有限に生成されたすべての捩れ A-加群 T は、因子が形 $A/p$ の A-加群と同型である分解系列を認めます。ここで、$p \in \mathrm{Supp}(T)$ (章) IV, § 1, no. 4、定理 1 および 2)、T が捩れ加群であるため、$p \neq 0$ となります。この分解系列の長さ上の帰納法までに、($\psi$ の性質 (1) を考慮して) $\psi(T) = 0$ と推測します。

\* no. 4 と同様に、有限生成された擬似ゼロ捩れ A-加群の完全なサブカテゴリ $\mathscr{T}'$ によって、有限生成された捩れ A-加群のカテゴリ $\mathscr{T}$ の商カテゴリ $\mathscr{T}/\mathscr{T}'$ を考慮する場合があります。 アーベルカテゴリの言語では、命題 11 は、アーベルカテゴリ $\mathscr{T}/\mathscr{T}'$ の *グロタンディーク群* が $D(A)$ と標準的に同型であるという事実を表します。 \*

#### 命題 12 {#ac-vii-s4-prop-12 .statement tag=053U}

*a が A のイデアル $\neq 0$ である場合、

$$
\chi(A/a) = \chi((A : a)/A) = \mathrm{div}\, a.
$$

$p \in P$ にしましょう。次に、$A_p$ は離散評価環であるため、$aA_p = p^{n_p}A_p$ ここで $n_p \geq 0$ となります。 *として* $(A/a)_p = A_p/aA_p,\ l_p(A/a) = n_p$、よって $\chi(A/a) = \sum_{p \in P} n_p p = \mathrm{div}\, a$ (§ 1, no. 4、命題 7)。

一方、$(A : a) = A ; aA_p = p^{-n_p}A_p$ なので、$l_p((A : a)/A) = n_p$ となり、同様に結論するとなります。

### 6. 2 つの格子の相対不変量

私たちは記法とノーの仮説を保持します。 2から5。Vを$K$上の有限階数$n$のベクトル空間とし、MをAに関するVの格子とします。Wを外部冪$\bigwedge^n V$、つまりベクトル空間とします。 *$K$ 上の階数 1*、$M_w$ は、標準写像 $V^n \to \bigwedge^n V$ (no. 1, 命題 3 (iii) の下で $M^n$ の像によって生成される W の格子を表します。$M_w$ は必ずしもそうではないことに注意してください) $\bigwedge^n M$ (*代数*, 章 III, § 5, 練習問題 9)) と同型。 $e$ が K 上の W の基底である場合、$M = a.e$ と書くことができます。ここで、a は A の分数イデアル $\neq 0$ です。

$M'$ を V の別の格子とし、$M'_w = a'.e$ と書きます。ここで、$a'$ は A の分数イデアル $\neq 0$ です。約数 $\operatorname{div}(a) - \operatorname{div}(a')$ *基底の選択には依存しません* W、a、および $a'$ の $e$ は、基底が変更されると $K^*$ の同じ要素で乗算されます。 $\chi(M, M') = \operatorname{div}(a) - \operatorname{div}(a')$ と書き、この約数は *M に関して * $M'$ の *相対不変量* であると言いましょう。 明らかに、M、$M', M''$ が V の 3 つの格子である場合、次のようになります。

(3)
$$
\chi(M, M') + \chi(M', M'') + \chi(M'', M) = 0
$$
(4)
$$
\chi(M, M') + \chi(M', M) = 0.
$$

すべての $p \in P$ について、定義からすぐに $(M_w)_p = (M_p)_w$ が続きます。さらに、M は *afree* A,-module であるため、A は A 上の M の主イデアル整域, 基底であり、K 上の V の基底であるため、$(M_p)_w = \bigwedge^n (M_p)$ (章 II, § 2, no. 8) となり、分数イデアル $a_p = aA_p$ は次のようになります。 主イデアル整域。 集合 $a_p = p^{n_p}A_p$、$a' = p^{n'_p}A_p$ の場合、次のようになります。
$$
\chi(M, M') = \sum_{p \in P} (n_p - n'_p).p,
$$
これは次のように書くこともできます。
(5)
$$
\chi(M, M') = \sum_{p \in P} \chi(M_p, M'_p)
$$
$p$ によって生成された $D(A)$ のサブ Z モジュールで $D(A_p)$ を識別します。

#### 命題 13 {#ac-vii-s4-prop-13 .statement tag=053V}

*M を V の格子、u を V の K 自己同型とする。その後*:
(6)
$$
-\chi(M, u(M)) = \operatorname{div}(\det(u)).
$$
すべての $p \in P$ については、次に $\bigwedge^n (u(M)_p) = \bigwedge^n (u(M_p))$ です。 $(e_i)_{1 \leq i \leq n}$ が $M_p$ の基底である場合、
$$
\bigwedge^n (M_p) = A_p \cdot e_1 \text{ } A \text{ } e_2 \text{ } A \ldots A \text{ } e_n,
$$

そして、公式のおかげで、$\bigwedge^n (u(M_p)) = A_p \cdot \det(u) e_1 \wedge e_2 \mathbf{A} \ldots \mathbf{A} e_n$、よって命題 (5)。

#### 命題 14 {#ac-vii-s4-prop-14 .statement tag=053W}

*M、M' が 2 つの格子 V で、M' \部分集合 M、M/M' が有限生成された捩れ A-加群である場合、*

$$
\chi(M, M') = -\chi(M/M').
$$

Clearly M/M' \subset V/M' is a finitely generated torsion module; on the other hand, for all $p \in P$, we know (*Algebra*, Chapter VII, § 4, no. 2, Theorem 1) that there exist bases $(e_i)_{1 \leq i \leq n}$ of M, and $(e'_i)_{1 \leq i \leq n}$ of $M'_p$ such that $e'_i = \pi^{v_i} e_i$ for $1 \leq i \leq n$ and integers $v_i \geq 0$, $\pi$ being a uniformizer of $A_p$. したがって、(上で紹介した記法では) $n'_p - n_p = \sum_{i=1}^n v_i$;そしてその一方で、

$$(M/M')_p = M_p/M'_p$$ は捩れ A,-module $\bigoplus_{i=1}^n A_p/p^{v_i} A_p$ と同型であるため、その長さは $\sum_{i=1}^n v_i$ であり、no. 5 の (5) と定義 4 を考慮して命題が証明されます。

#### 系 {#ac-vii-s4-n6-cor-1 .statement tag=053X}

*L_1、L_2 を 2 自由 A-加群 & 同じ階数 n とし、f: L_1 \to L_2 を準同型とします。 L_1とL_2の基底に関してUを行列オフとする。 Coker(f) が捩れ A-加群になるには、 \det(U) \neq 0 であり、その後:* であることが必要かつ十分です。

$$
\chi(\operatorname{Coker}(f)) = \operatorname{div}(\det(U)).
$$

L_1 と L_2 は、それぞれ $V_1 = L_1 \otimes_A K$ と $V_2 = L_2 \otimes_A K$ の格子と考えることができ、f は K 準同型性 $f_{(K)}: V_1 \to V_2$ まで拡張されます。それから

$$(\operatorname{Coker}(f))_{(K)} = \operatorname{Coker}(f_{(K)})$$

そして、$\operatorname{Coker}(f)$ が捩れ A-加群であると言うことは、$\operatorname{Coker}(f_{(K)}) = 0$ を意味します。さて、$f_{(K)}$ が全射であると言うのも、$\det(U) \neq 0$、よってが最初の主張であると言うのも、同じことになります。一方、$f(L_1) = u(L_2)$ と書くこともできます。ここで、$u$ は、行列式 $\det(U)$ の $L_2$ の自己準同型です。として

$$\operatorname{Coker}(f) = L_2/u(L_2),$$

公式 (8) は (7) と (6) から続きます。

#### 例 {#ac-vii-s4-n6-exa-1 .statement tag=053Y}

$A = \mathbf{Z}$, $A$ の因子群は、有理数数 > 0 の乗法群 $\mathbf{Q}_+^*$ と同一視されます。すべての有限可換群 T について、$\chi(T)$ は次の *位数* です。 T;上記の系は、群 $\operatorname{Coker}(f)$ の位数が $\det(U)$ の *絶対値* (cf. *代数*, 章 VII, § 4, no. 7, 系) に等しいことを示しています。 3から定理3）。

### 7. 因子類が有限生成加群に接続されました

私たちは記法とノーの仮説を保持します。 2 ～ 6. C(A) (または単に C) は、本人の部分群による $A$ の因子類群、$D(A)$ の商を表していることを思い出してください。 因子。 因子 $d \in D$ ごとに、C の類を $c(d)$ で表します。

#### 命題 15 {#ac-vii-s4-prop-15 .statement tag=053Z}

※Mを有限生成A-加群とします。 M/L が捩れ加群および C の元 $c(\chi(M/L))$ となるような M の自由部分加群 L が存在します。* は、選択された自由部分加群 L に依存しません。

$S = A - \{0\}$と書いて$V = S^{-1}M = M \otimes_A K$とします。 $n$ が K 上の V の階数である場合、V 形基底に標準像が含まれる M の $n$ 元 $e_i$ ($1 \leq i \leq n$) が存在します。 Vの;これらの元は明らかに M において線形独立であるため、生成するは $S^{-1}(M/L) = S^{-1}M/S^{-1}L = 0$ となるような M の自由部分加群 L となり、M/L は捩れ加群となります。

さて、L を、階数 $n$ の M の他のを自由にする部分加群とします。 $S^{-1}L = S^{-1}L_1$ 以降、$sL_1 \subset L$ となるような $s \in S$ が存在します。したがって、$L_1 \subset L_2$ が階数 $n$ の M の 2 つ自由な部分加群である場合、極限を証明にすることができます。

$$
c(\chi(M/L_1)) = c(\chi(M/L_2)).
$$

さて、$\chi(M/L_1) = \chi(M/L_2) + \chi(L_2/L_1)$ と、no. 6、系から命題 14 から、$\chi(L_2/L_1)$ はプリンシパル因子であることがわかります。

$$
c(\chi(L_2/L_1)) = 0.
$$

以下では、元 $c(\chi(M/L))$ を $-c(M)$ と表記します。 $c(M)$ は因子類が M に接続されているとします。

#### 命題 16 {#ac-vii-s4-prop-16 .statement tag=0540}

(i) *$0 \to M_1 \xrightarrow{\alpha} M_2 \xrightarrow{g} M_3 \to 0$を有限生成A-加群の完全系列とします。それから*

$$
c(M_2) = c(M_1) + c(M_3).
$$

(ii) *M_1 から M_2 までの擬似同型性が存在する場合、$c(M_1) = c(M_2)$。

(iii) *T が捩れ加群の場合、$c(T) = -c(\chi(T))$。

(iv) *$a \neq 0$ が K の分数イデアルである場合、*

$$
c(a) = c(\operatorname{div}(a)).
$$

(v) ※Lが自由A-加群の場合、$c(L) = 0$。

(i) を証明するには、$M_1/L_1$ (それぞれ $M_3/L_3$) が捩れ加群となるような M, (それぞれ $M_3$) の自由サブモジュール $L_1$ (それぞれ $L_3$) を考えます。 $L_3$ は自由であり、$g$ は全射であるため、$g^{-1}(L_3)$ には、$L_3$ (*代数*, 章 II, § 1, no. 11, 命題 21) と同型である $\operatorname{Ker}(g)$ の自由補数 $L_{23}$ が存在します。しかし、$\operatorname{Ker}(g) = f(M_1)$ 含む $f(L_1) = L_{12}$ は、$f$ が単射法なので自由です。 和 $L_2 = L_{12} + L_{23}$ は直接であり、$L_2$ は$M$ の *フリー* 部分加群です。さらに、可換図式もあります。

$$
\begin{array}{ccccccccc}
0 & \longrightarrow & L_1 & \longrightarrow & L_2 & \longrightarrow & L_3 & \longrightarrow & 0 \\
0 & \longrightarrow & M_1 & \xrightarrow{f} & M_2 & \xrightarrow{g} & M_3 & \longrightarrow & 0
\end{array}
$$

ここで、行は正確で、垂直矢印は単射です。したがって、ヘビ図式 (章 I, § 1, no. 4, 命題 2) 完全系列から次のようになります。

$$
0 \to M_1/L_1 \to M_2/L_2 \to M_3/L_3 \to 0.
$$

$M_1/L_1$ と $M_3/L_3$ は捩れ加群であるため、この完全系列は、まず $M_2/L_2$ であることを示し、次に no. 5 の 10 である命題により、次のことがわかります。

$$
\chi(M_2/L_2) = \chi(M_1/L_1) + \chi(M_3/L_3)
$$

これは (i) を証明します。

主張 (iii) と (v) は定義から明らかです。 (ii)を証明します。したがって、$f : M_1 \to M_2$ を擬似同型写像とし、$L_1$ を $M_1/L_1$ が捩れ加群となるような $M_1$ の自由部分加群とする。私たちは集合 $L_2 = f(L_1)$; $\mathrm{Ker}(f)$ は擬似ゼロであるため、捩れ加群であるため、$\mathrm{Ker}(f) \cap L_1 = 0$ となり、したがって $L_2$ はフリーになります。 $\tilde{f} : M_1/L_1 \to M_2/L_2$ を商を取って $f$ から導出された準同型とします。 $\mathrm{Ker}(\tilde{f})$ は $\mathrm{Ker}(f)$ と同型であり、$\mathrm{Coker}(\tilde{f})$ は $\mathrm{Coker}(f)$ と同型であるため、$\tilde{f}$ は擬似同型です。さらに

$$
\mathrm{Coker}(\tilde{f}) = M_2/f(M_1)
$$

は捩れ加群であり、$f(M_1)/L_2 = \tilde{f}(M_1/L_1)$ も同様であるため、$M_2/L_2$ は捩れ加群となり、no. 5, 命題 10 (ii) から次のようになります。

$$
\chi(M_1/L_1) = \chi(M_2/L_2).
$$

最後に (iv) を証明することが残っています。 $x \in K^*$ を $a \subset xA$ となるようにします。 完全系列 $0 \to a \to xA \to xA/a \to 0$ を考慮すると、次のようになります。

$$
c(a) = c(xA) - c(xA/a) = -c(xA/a)
$$

(i) と (v) によって。しかし、$xA/a$ は (iii) により、$A/x^{-1}a$、よってと同型です。

$$
c(xA/a) = -c(\chi(A/x^{-1}a)) = -c(\mathrm{div}(x^{-1}a)) = -c(\mathrm{div}(a))
$$

(no. 5、命題 12)。これで証明は完了です。

$M$ が $A$, $\chi(M/L) = -\chi(M, L)$ (no. 6, 命題 14) に対する $V$ の *格子* であるとき。 $(e_i)_{1 \leq i \leq n}$ を $L$、$e = e_1 \wedge e_2 \wedge \ldots \wedge e_n$ の基底とします。

$M_w = a \cdot e$ (no. 6中記法);次に、$\chi(M, L) = \operatorname{div}(a)$、よって $c(M) = c(\operatorname{div}(a))$、これは命題 16 (v) を一般化します。

#### 系 1 {#ac-vii-s4-prop-16-cor-1 .statement tag=0541}

*$0 \to M, \xrightarrow{u} M_{n-1} \to \cdots \to M_0 \to 0$ *を有限生成A-加群の完全系列とします。* 次に、

$$
\sum_{i=0}^n (-1)^i c(M_i) = 0.
$$

$n$ について帰納法により議論し、ケース $n = 2$ は命題 16 (i) となります。 $M'_{n-1} = \operatorname{Coker}(u)$ の場合、完全系列が 2 つあります。

$$
\begin{align*}
0 &\to M, \to M_{n-1} \to M'_{n-1} \to 0 \\
0 &\to M'_{n-1} \to M_{n-2} \to \cdots \to M_0 \to 0.
\end{align*}
$$

最初の例は、$M'_{n-1}$ が有限に生成され、帰納法の仮定が次の結果を与えることを示しています。

$$
(-1)^{n-1} c(M'_{n-1}) + \sum_{t=0}^{n-a} (-1)^t c(M_t) = 0
$$

そして

$$
c(M'_{n-1}) = c(M_{n-1}) - c(M_n),
$$

よって系。

完全系列

$$
0 \to L_n \to L_{n-1} \to \cdots \to L_0 \to E \to 0
$$

ここで、$L_i$ ($0 \leq i \leq n$) は *有限に生成された自由* A-加群であり、 A-加群 E の *有限の自由解像度* と呼ばれます。

#### 系 2 {#ac-vii-s4-prop-16-cor-2 .statement tag=0542}

*除数分数イデアル* $a \neq 0$ *of* $\mathbf{A}$ *有限の自由な解決が認められる場合、それは原理的です。*

実際、系を適用する 1 を $a$ の有限自由解像度に変換します。

$$
0 \to L_n \to L_{n-1} \to \cdots \to L_0 \to a \to 0.
$$

命題 16 (v)、$c(a) = 0$ により、したがって命題 16 (iv) により、$\operatorname{div}(a)$ が主要です。 $a$ は除数であると想定されているため、主 (§ 1, no. 1) です。

#### 系 3 {#ac-vii-s4-prop-16-cor-3 .statement tag=0543}

*すべての除算イデアル* $\neq 0$ *of* $\mathbf{A}$ *が有限の自由解像度を認める場合*、 $\mathbf{A}$ *は階乗です*。

これは、系 2 と § 3, no. 1、定義 1 の明らか帰結です。

\* 通常の局所環は系 3 の仮定を満たすため、*階乗* であることが後でわかります。 \*

M が有限生成A-加群の場合、その *階数* を $r(M)$ で表します ($M_{(K)} = M \otimes_A K$ の K に対する階数であることを思い出してください)。 $0 \to M_1 \to M_2 \to M_3 \to 0$ が有限生成A-加群の完全系列である場合、数列

$$
0 \to (M_1)_{(K)} \to (M_2)_{(K)} \to (M_3)_{(K)} \to 0
$$

も正確なので、$r(M_2) = r(M_1) + r(M_3)$です。私たちは書きます

$$
\gamma(M) = (r(M), c(M)) \in \mathbf{Z} \times C(A);
$$

したがって、$\gamma$ は命題 16 の性質 (i) を満たし、M が擬似ゼロの場合、$\gamma(M) = 0$ (M は捩れ加群であるため) を満たします。 $F(A)$ から $\mathbf{Z} \times C(A)$ までの一意な写像が存在し、これも y で示され、有限生成A-加群 M ごとに $\gamma(M) = \gamma(\mathrm{cl}(M))$ になります。上記のプロパティが本質的に y を特徴付けることがわかります。

#### 命題 17 {#ac-vii-s4-prop-17 .statement tag=0544}

G を、*加法的に*書かれた可換な群と、*有限に*生成された A-加群の類の集合 $F(A)$ から G への *写像* である $\phi$ とする。 *有限に*生成されるすべての A-加群 M に対して、言葉の乱用により、$\phi(M) = \phi(\mathrm{cl}(M))$ とも書きます。 *次の条件が *満たされている* と仮定します。
  (1) *もし* $0 \to M_1 \to M_2 \to M_3 \to 0$ が *有限* 生成された A-加群の完全系列である場合、 $\phi(M_2) = \phi(M_1) + \phi(M_3)$ です。
  (2) *T が擬似ゼロの場合、$\phi(T) = 0$。
*すると* $\phi = 8 \circ y$ となるような一意な準同型 $\theta : Z \times C \to G$ が存在します。

命題 16 (iv) により、$Z \times C$ のすべての元は、いくつかの適切な有限生成A-加群 M に対して形 $(r(M), c(M))$ になります。 よって一意性/$\theta$。私たち命題を適用する 11 of no. 5 から制限 of $-\phi$ から $T(A)$: すると、次のような準同型 $\theta_0 : D \to G$ が存在します。

$$
-\phi(T) = \theta_0(\chi(T))
$$

有限に生成されたすべての捩れ A-加群 T に対して。x を A の非ゼロ元とします。 適用性質 (1) ～ 完全系列:

$$
0 \longrightarrow A \xrightarrow{h_x} A \longrightarrow A/xA \longrightarrow 0
$$

ここで、$h_x$ は乗法を x で表すと、$\phi(A/xA) = 0$、よって $\theta_0(\mathrm{div}(x)) = 0$ が得られます。 商, $\theta_0$ を取ると、定義する準同型 $\theta_1 : C \to G$ と $\phi(T) = \theta_1(c(T))$ が捩れ A-加群 T ごとに得られます。$\theta(n, z) = n.\phi(A) + \theta_1(z)$ で定義された準同型 $\theta$ が解けることを示します。 問題。このため、有限生成A-加群 M ごとに $\phi'(M) = \phi(M) - \theta(\gamma(M))$ を書き込みます。 $\phi$ を $\phi'$ に置き換えても、明らかに条件 (1) は満たされます。また、M が捩れ加群または自由加群の場合は $\phi'(M) = 0$ です。しかし、すべての有限生成A-加群 M については、M の空きサブモジュール L が存在し、M/L は捩れ加群 (命題 15)、性質 (1) は、すべての有限生成A-加群 M に対して $\phi'(M) = 0$ であることを示します。

\* アーベルカテゴリの言語では、命題 17 は、$\mathbf{Z} \times C(A)$ が商カテゴリ $\mathscr{F}/\mathscr{F}'$ のグロタンディーク群と正規同型であることを示します。ここで、$\mathscr{F}$ は有限生成A-加群のカテゴリ、$\mathscr{F}'$ は $\mathscr{F}$ の完全なサブカテゴリです擬似ゼロ加群のからなる。 \*

### 8. スカラーの有限拡大の環に関するプロパティ

この番号では、A と B は 2 つの統合的に閉じたネーター領域を表し、$A \subset B$ と B は有限生成された A 加群であり、K と L はそれぞれ A と B の分数体です。 A-加群が関係する場合は、それぞれ div、$\chi$、c、y、r の代わりに div$_A$、$\chi_A$、$c_A$、$\gamma_A$、$r_A$ と書き、B-加群には同様の記法を使用します。

B の素イデアル $\mathfrak{p}$ が高さ 1 であるためには、$\mathfrak{p} = \mathfrak{P} \cap A$ が高さ 1 であることが必要かつ十分であることがわかります (§ 1, no. 10)。さらに、(上記引用、命題 14) $\mathfrak{p} \in P(A)$ については、$\mathfrak{p}$ の上にある主要なイデア $\mathfrak{P} \in P(B)$ の有限の数のみが存在します。 省略すると、$\mathfrak{P}|_{\mathfrak{p}}$ 関係 「$\mathfrak{P}$ が $\mathfrak{p}$ の上にある」（つまり、$\mathfrak{p} = \mathfrak{P} \cap A$）と表し、その後、評価の分岐添字 $e(v_{\mathfrak{P}}/v_{\mathfrak{p}})$ を$e_{\mathfrak{P}/\mathfrak{p}}$ または $e(\mathfrak{P}/\mathfrak{p})$ で表します。 $v_{\mathfrak{P}}$ が評価 $v_{\mathfrak{p}}$ (章 VI, § 8, no. 1) で、$f_{\mathfrak{P}/\mathfrak{p}}$ または $f(\mathfrak{P}/\mathfrak{p})$ 剰余類次数 $f(v_{\mathfrak{P}}/v_{\mathfrak{p}})$ (上記参照)。 $v_{\mathfrak{p}}$ と $v_{\mathfrak{P}}$ が標準であり、その $f_{\mathfrak{P}/\mathfrak{p}}$ は、$A/\mathfrak{p}$ の分数の体を超え、 $B/\mathfrak{P}$ の分数の体の次数です。 私たちは集合 $n = r_A(B)$ で、B は A-加群と見なされます。したがって、定義 $n = [L:K]$ により、すべての $\mathfrak{p} \in P(A)$ に対して、$n$ はすべての $\mathfrak{P}|_{\mathfrak{p}}$ に対して空き A、モジュール B の階数になります。 次に、章 VI, § 8, no. 5、定理 2 から、すべての $\mathfrak{p} \in P(A)$ について次のようになります。

$$
\sum_{\mathfrak{P}|_{\mathfrak{p}}} e_{\mathfrak{P}/\mathfrak{p}} f_{\mathfrak{P}/\mathfrak{p}} = n.
$$

したがって、$D(A)$ と $D(B)$ は無料の $\mathbf{Z}$ モジュールであるため、注文した群 $N : D(B) \to D(A)$ ($N_{B/A}$ とも表される) の定義する増加する準同型を条件で計算します。

$$
N(\mathfrak{P}) = f_{\mathfrak{P}/\mathfrak{p}} \cdot \mathfrak{p} \quad \text{for} \quad \mathfrak{P} \in P(B), \quad \text{where} \quad \mathfrak{p} = \mathfrak{P} \cap A.
$$

一方 (§ 1, no. 10、命題 14) は、順序付けられた群 $i : D(A) \to D(B)$ ($i_{B/A}$ とも表される) の増加する準同型を条件によって定義しました。

$$
i(p) = \sum_{\mathfrak{P}|_p} e_{\mathfrak{P}/\mathfrak{p}} \cdot \mathfrak{P} \quad \text{for} \quad p \in P(A).
$$

明らかに、A (B) の因子のすべての家族 $(d_i)$ (それぞれ $(d'_i)$):

$$
N(\sup(d'_i)) = \sup(N(d'_i)), \qquad N(\inf(d'_i)) = \inf(N(d'_i))
$$
$$
i(\sup(d_i)) = \sup(i(d_i)), \qquad i(\inf(d_i)) = \inf(i(d_i)).
$$

公式 (9) は次のことを示しています。

(14) $$ N \circ i = n . 1_{D(A)} $$

すべての$a \in A$ (§ 1, no. 10、命題 14):

(15) $$ i(\operatorname{div}_A(a)) = \operatorname{div}_B(a). $$

$A$ の各分数イデアル $a$ について、((13) によって) 次のことが推定されます。

(16) $$ i(\operatorname{div}_A(a)) = \operatorname{div}_B(aB). $$

元 $b \in B$ ごとに、$N_{L/K}(b) \in A$ であることがわかります (章 V, § 1, no. 3、系から命題 11)。さらに (章 VI, § 8, no. 5, 公式 (9)):

(17) $$ v_p(N_{L/K}(b)) = \sum_{\mathfrak{p}/p} f_{\mathfrak{p}/p} v_{\mathfrak{p}}(b) $$

よって:

(18) $$ N(\operatorname{div}_B(b)) = \operatorname{div}_A(N_{L/K}(b)). $$

式 (15) と (18) は、商、準同型 $N$、$i$ 定義する準同型を採用すると、次のように表されます。

$$ N : C(B) \to C(A), \quad i : C(A) \to C(B). $$

準同型 $i : C(A) \to C(B)$ は一般に単射ではないことに注意してください (§ 3、練習問題 7)。

すべての $B$ モジュール $R$ について、$R_{[A]}$ は、スカラーを $A$ (代数、章 11、§ 1, no. 13) に制限することによって $R$ から取得された $A$ モジュールを表すことを思い出してください。

#### 命題 18 {#ac-vii-s4-prop-18 .statement tag=0545}

(i) *$R$ が擬似ゼロ $B$ モジュールであるためには、$A$ モジュール $R_{[A]}$ が擬似ゼロであることが必要かつ十分です。*

(ii) *$R$ が有限生成捩れ $B$ モジュールであるためには、$R_{[A]}$ が有限生成捩れ $A$ モジュールであることが必要かつ十分であり、その後:*

(19) $$ \chi_A(R_{[A]}) = N(\chi_B(R)). $$

(iii) *$R$ が有限生成された $B$ モジュールであるためには、 $R_{[A]}$ が有限生成された $A$ モジュールであることが必要かつ十分であり、その後:*

(20) $$ c_A(R_{[A]}) = N(c_B(R)) + r_B(R)c_A(B) $$
(21) $$ r_A(R_{[A]}) = n . r_B(R) \quad \text{(recall that } n = r_A(B)). $$

$B$ は有限生成された $A$ モジュールであるため、 $R$ が有限生成された $B$ モジュールであるためには、 $R_{[A]}$ が有限生成された $A$ モジュールであることが必要かつ十分です。さらに、$b$ が $R$ の消滅子である場合、$b \cap A = a$ は $R_{[A]}$ の消滅子です。 $B$ は $A$ に対して整数であるため、$A$ (章 V, § 2, no. 1、系 1 ～ 命題 1) の理想 0 よりも上にある 0 以外の理想は存在しないため、$a \neq 0$ またはそれと言うのは同じことになります。 $b \neq 0$。

(i) この最後の注意により、$R$ が捩れ $B$ モジュールである場合に注意を限定することができます。 $b$が素イデアル$\mathfrak{p} \in P(B)$に含まれる場合、$a$は高さ1の$\mathfrak{p} \cap A = p$に含まれます。逆に、$a$が素イデアル$p \in P(A)$に含まれる場合、含むである$B$の素イデアル$\mathfrak{p}$が存在します。 $b$ そして $p$ の上にあります (章 V, § 2, no. 1、系 2 ～ 定理 1)。 主張 (i) は、これらの注意と no. 4、定義 2 から続きます。

(ii) 有限に生成されたすべての捩れ $B$ モジュール $R$ について、次のように書きます。

$$
\phi(R) = \chi_A(R_{[A]});
$$

明らかに (有限生成された捩れ $B$ モジュールの場合) $\phi$ は、命題 II の no. 5 の条件 (1) および (2) を満たします ((i) を考慮して)。したがって、有限生成された捩れ $B$ モジュール $R$ ごとに $\phi(R) = \theta(\chi_B(R))$ となる準同型 $\theta : D(B) \to D(A)$ が存在します。 準同型 $\theta$ は、$\chi_B(B/\mathfrak{p}) = \mathfrak{p}$ 以降、形 $B/\mathfrak{p}$ の$\mathfrak{p} \in P(B)$ のすべての $B$ モジュールの値によって決定されます。さて、$P(A)$、$p \notin q$、そして$(B/\mathfrak{p})_q = 0$ の各素数理想$q \neq p = \mathfrak{p} \cap A$ についてです。一方、集合 $S = A - p$ とすると、$\mathfrak{p}.S^{-1}B$ は $S^{-1}B$ と $(B/\mathfrak{p})_p = S^{-1}B/\mathfrak{p}$ の最大の理想になります。 $S^{-1}B$ は、$B/\mathfrak{p}$ の分数の体 (章 II, § 2, no. 5, 命題 11)、つまり $v_{\mathfrak{p}}$ の剰余体と同型です。したがって、$A$ モジュールとしての長さは $f_{\mathfrak{p}/p}$ です。これは、$\theta = N$ (no. 5、定義 4) であることを証明します。

(iii) $T$ が $R$ の捩れ部分加群である場合、$T_{[A]}$ は $R_{[A]}$ と $(R/T)_{[A]} = R_{[A]}/T_{[A]}$ の捩れ部分加群です。 (21) を証明するには、したがって、$R$ にねじれがない場合に注意を限定することができます。 次に、$R$ は $R_{(L)}$ のサブ$B$ モジュールで識別され、$L$ を超える $R_{(L)}$ の基底 $(e_i)_1 < < m$ が含まれます。 $(b_j)_1 s < n$ が $B$ の要素からなる $K$ 上の $L$ の基底である場合、$b_j e_i$ は $R$ の要素からなる $K$ 上の $R_{(L)}$ の基底を形成します (21)。 一方、$M$ を $R$ の空きサブ$B$ モジュールとし、$R/M$ が捩れ $B$ モジュールとなるようにします。 $M_{[A]}$ は、命題 16 (i) により、$r_B(R)$ $A$ モジュールの直和が $B$ と同型であるため、

$$
c_A(M_{[A]}) = r_B(R).c_A(B).
$$

さらに、(19) により $c_A((R/M)_{[A]}) = -c_A(N(\chi_B(R/M)))$;しかし、準同型 $N : C(B) \to C(A)$ の定義によって、すべての $d \in D(B)$ に対して $c_A(N(d)) = N(c_B(d))$ が、そして定義によって $c_B(\chi(R/M)) = -c_B(R)$ として、最終的には

$$
c_A((R/M)_{[A]}) = N(c_B(R));
$$

その場合、(20) を得るには命題を適用する 16 (i) で十分です。

#### 命題 19 {#ac-vii-s4-prop-19 .statement tag=0546}

$R$ を *有限に* 生成された $B$ モジュールとします。 *$R$ が *再帰的* であるためには、 $R_{[A]}$ が *再帰的 * $A$ モジュールであることが *必要十分* です。

命題 18 の証明で、R がねじれのない B-加群であるためには、$R_{[A]}$ がねじれのない A モジュールであることが必要かつ十分であると述べました。したがって、R は B に関する $W = R \otimes_B L$ の格子であると仮定できます。次の補題を使用します。

#### 補題 4 {#ac-vii-s4-lem-4 .statement tag=0547}

*W を L 上の有限階数のベクトル空間とし、R を B に関する W の格子とします。すると、すべての $p \in P(A)$、$(R_{[A]})_p = \bigcap_{\mathfrak{p}/p} R_{\mathfrak{p}}$ について*

$S = A - p$ の場合、環 $S^{-1}B$ の素イデアルは、S を満たさない B の素イデアルによって生成され、他の語では、p とイデアル (0) の上にあるイデアル $\mathfrak{P}_i$ ($1 \leq i \leq m$) によって生成されます。これは、$S^{-1}B$ が半局所リングであり、その最大イデアルが m、$1 \leq i \leq m$ の $= \mathfrak{P}_i(S^{-1}B)$ であることを示しています。さらに、局所環 $(S^{-1}B)_{\mathfrak{P}_i}$ は $B_{\mathfrak{p}_i}$ (章 11、§ 2, no. 5、命題 11) と同型であるため、離散評価環です。したがって、環 $S^{-1}B$ はデデキントのドメイン (§ 2, no. 2, 定理 1 (f)) であり、準ローカルであるため、主イデアル整域 (§ 2, no. 2, 命題 1) です。そうであれば、$(R_{[A]})_p$ は A,-加群とみなされる $S^{-1}R$ に等しい。上記により、$S^{-1}R$ は $S^{-1}B$ に関する W の自由格子であり、no. 2 の 2 である定理がそれに適用され、$S^{-1}R = \bigcap_i (S^{-1}R)_{m_i}$ が得られます。しかし、$(S^{-1}R)_{m_i} = R_{\mathfrak{p}_i}$ となり、補題が証明されます。

命題 19 の証明に戻り、補題 4 までに、

$$
\bigcap_{\mathfrak{p} \in P(B)} R_{\mathfrak{p}} = \bigcap_{p \in P(A)} (R_{[A]})_p
$$

そして結論は no. 2、定理 2 から導き出されます。

#### 系 {#ac-vii-s4-n8-cor-1 .statement tag=0548}

*環 B は再帰的な A-加群です。*

#### 命題 20 {#ac-vii-s4-prop-20 .statement tag=0549}

(i) *有限生成A-加群 M が擬似ゼロであるためには、$M \otimes_A B$ が擬似ゼロである B-加群であることが必要かつ十分です。*
(ii) *M が有限生成された捩れ A-加群である場合、$M \otimes_A B$ は有限生成された B-加群であり、*
(22)
$$
\chi_B(M \otimes_A B) = i(\chi_A(M)).
$$
(iii) *M が有限生成A-加群の場合、$M \otimes_A B$ は有限生成された B-加群であり、*
(23)
$$
c_B(M \otimes_A B) = i(c_A(M))
$$
(24)
$$
r_B(M \otimes_A B) = r_A(M).
$$

(i) $\mathfrak{p}$ を $B$、$\mathfrak{p} = \mathfrak{P} \cap A$ の主要な理想とする。次に、$(M \otimes_A B)_{\mathfrak{p}} = M \otimes_A B_{\mathfrak{p}}$ (章 11、§ 2, no. 7、命題 18)、そしてその一方で
$$
M \otimes_A B_{\mathfrak{p}} = (M \otimes_A A_p) \otimes_{A_p} B_{\mathfrak{p}} = M_p \otimes_{A_p} B_{\mathfrak{p}};
$$
したがって、関係 $M_p = 0$ は $(M \otimes_A B)_{\mathfrak{p}} = 0$ (章 II, § 4, no. 4, 補題 4) と同等です。 (i) を証明するには、no. 4、定義 2 を考慮して、この注意を理想 $\mathfrak{P} = (0)$ と理想 $\mathfrak{p} \in P(B)$ に適用するだけで十分です。

(ii) を証明するには、次の補題を使用します。

#### 補題 5 {#ac-vii-s4-lem-5 .statement tag=054A}

*$M_1, M$ を 2 つの有限生成された $A$ モジュール、および $f : M_1 \to M_2$ 単射準同型とします。すると、$f \otimes 1 ; M_1 \otimes_A B \to M_2 \otimes_A B$の核は擬似ゼロになります*。

$\mathfrak{p}$を身長$\leq 1$の$A$の第一の理想とする。次に、$(M_i \otimes_A B)_\mathfrak{p} = (M_i)_\mathfrak{p} \otimes_{A_\mathfrak{p}} B_\mathfrak{p}$ ($i = 1, 2$) (章 11、§ 2, no. 7、命題 18) および $(f \otimes 1_B)_\mathfrak{p} = f_\mathfrak{p} \otimes 1_{B_\mathfrak{p}}$; 仮定 $f$ が単射であるということは、$f$, (章 II, § 2, no. 4, 定理 1) も単射であることを意味します。一方、$\mathfrak{p}$の選択を考慮すると、$A_\mathfrak{p}$は主イデアル整域と$B_\mathfrak{p}$は有限生成されたねじれのない$A_\mathfrak{p}$モジュールであり、したがって*フリー*です。私たちは結論する、その$f_\mathfrak{p} \otimes 1_{B_\mathfrak{p}}$自体は単射です。 $I = \mathrm{Ker}(f \otimes 1)$ の場合、$I_\mathfrak{p} = \mathrm{Ker}((f \otimes 1)_\mathfrak{p})$ (章 11、§ 2, no. 4、定理 1)。したがって、$\mathfrak{p}|p$ に対して $I_\mathfrak{p} = 0$, よって *なおさら* $I_\mathfrak{p} = (I_\mathfrak{p})_\mathfrak{p} = 0$ となり、補題 (no. 4, 定義 2) が証明されます。

(ii)の証明に戻ります。有限に生成されたすべての捩れ $A$ モジュール $M$ に対して、 $\phi(M) = \chi_B(M \otimes_A B)$ を書き込みます。 (i) から、$M$ が擬似ゼロであれば、$\phi(M) = 0$ ということがわかります。一方、有限生成された捩れ $A$ モジュールの完全系列を考えてみましょう。
$$
0 \to M_1 \to M_2 \to M_3 \to 0.
$$
補題 4 から、$B$ モジュールの完全系列が存在することがわかります。
$$
0 \to I \to M_1 \otimes_A B \to M_2 \otimes_A B \to M_3 \otimes_A B \to 0
$$
ここで、$I$ は擬似ゼロです。したがって、no. 5、系 ～ 命題 10 を使用すると、$\phi(M_2) = \phi(M_1) + \phi(M_3)$ が得られます。したがって、no. 5 の命題 11 から結論するは、有限に生成される捩れ $A$ モジュール $M$ ごとに $\phi(M) = \theta(\chi_A(M))$ となる準同型 $\theta : D(A) \to D(B)$ が存在することがわかります。 $\theta = i$ を証明するには、すべての $p \in P(A)$ に対して $\phi(A/p) = i(p)$ を示すだけで十分です。現在$(A/p) \otimes_A B = B/pB$、そして全員$\mathfrak{p} \in P(B)$、$(B/pB)_{\mathfrak{p}} = B_{\mathfrak{p}}/pB_{\mathfrak{p}}$。 $\mathfrak{p}$ が $p$ より上にない場合、最後の加群は 0 になります。逆に、$\mathfrak{p}|p$ の場合、$B_{\mathfrak{p}}/pB_{\mathfrak{p}}$ は、添字 (章 VI, § 8, no. 1) の定義による長さ $e(\mathfrak{p}/p)$ の $B_{\mathfrak{p}}$ 加群です。したがって、$\chi_B(B/pB) = \sum_{\mathfrak{p}|p} e_{\mathfrak{p}/p} . 13 = i(p)$ となり、(ii) の証明が​​完了します。

公式 (24) は明らか、
$$
(M \otimes_A B) \otimes_B L = M \otimes_A L = (M \otimes_A K) \otimes_K L
$$

そして、$L$以上の$(M \otimes_A K) \otimes_K L$の階数は、$K$以上の$M \otimes_A K$の階数と等しい。 (23) を表示するには、$Q = M/H$ が捩れ $A$ モジュールとなるような $M$ の空き部分加群 $H$ を考えます。 適用補題 4 を上記と同様に、$B$ モジュールの完全系列を取得します。

$$
0 \to I \to H \otimes_A B \to M \otimes_A B \to Q \otimes_A B \to 0
$$

ここで、$I$ は擬似ゼロです。したがって、no. 7、命題 16(ii)、(v)、および系 1 から命題 16 から次のことがわかります。

$$
c_B(M \otimes_A B) = c_B(Q \otimes_A B) = -c_B(\chi_B(Q \otimes_A B)) = -c_B(i(\chi_A(Q)))
$$

(ii) により。しかし、準同型 $i : C(A) \to C(B)$ の定義までに、
$c_B(i(\chi_A(Q))) = i(c_A(\chi_A(Q))) = -i(c_A(M))$、これで (23) の証明が完了します。

**注意**
(1) $M$ が再帰的な $A$ モジュールである場合、$M \otimes_A B$ は必ずしも再帰的であるとは限りません (練習問題 6)。ただし、$B$ がフラットな $A$ モジュール (no. 2、命題 8) の場合は当てはまります。
(2) $C$ を 3 番目の統合的に閉じたネーター 領域とし、$B \subset C$ と $C$ が有限生成された $B$ モジュール (したがって、有限生成された $A$ モジュール) となるようにします。次に、推移性の方程式ができます。

(25)
$$
N_{C/A} = N_{B/A} \circ N_{C/B},
$$
(26)
$$
i_{C/A} = i_{C/B} \circ i_{B/A}
$$

これは、分岐添字および剰余類次数 (章 VI, § 8, no. 1, 補題 1) の推移性方程式の直後に続きます。

### 9. 削減定理

記法と nos の仮説を保持します。 2から7まで。

#### 補題 6 {#ac-vii-s4-lem-6 .statement tag=054B}

*$R$ を可換環と $p_i$ ($1 \leq i \leq n$) の $R$ の異なる主理想とする。

(i) *$1 \leq i \leq n$ について、$H_i$ を $R/p_i$ 満たすの部分集合とし、次の条件: $\alpha_i + H_i$ 含むが理想的な$\neq 0$ となるような元 $\alpha_i \in R/p_i$ は存在しません。 $R/p_i$。すると、$1 \leq i \leq n$に対して、$R/p_i$の$a$の標準像が属するから$H_i$にならないような$a \in R$が存在します。

(ii) *$\operatorname{Card}(H_i) < \operatorname{Card}(R/p_i)$ の場合、(i) の $H_i$ 満たす条件。

(i) $n$ について帰納法によって議論しますが、$n = 0$ の場合は自明です。 したがって、$n \geq 1$ とします。 添字 $i$ で置換を作成し、$p_1$ が $p_i$ の中で最小であり、したがって $2 \leq i \leq n$ に対して、$c_i \notin p_1$ となるような $c_i \in p_i$ が存在すると仮定することができます。 帰納法の仮定までに、$R/p_i$の$b$の標準像が$2 \leq i \leq n$の属するから$H_i$にならないような$b \in R$が存在します。 すべての $x \in R$ については $a_i = b + x c_2 c_3 \ldots c_n$ と書きます。 $c_i \in p_i$ として、明らかに $2 \leq i \leq n$ の場合は $a_i \equiv b \pmod{p_i}$ です。 したがって、$\mathbf{R}/p_1$ の $a_i$ の標準像が属するから $H_1$ にならないような $x \in \mathbf{R}$ が存在することを証明すれば十分です。 さて、$x$ が $\mathbf{R}$ を通る$\mathbf{R}/p_1$ の $a_i$ の正準イメージのセットは、ちょうど $\beta + c$ です。ここで、$\beta$ は $b$ の正準イメージであり、$c$ は の正準イメージによって生成された $\mathbf{R}/p_1$ の理想です。 $c_2 c_3 \ldots c_n$; $\mathbf{R}/p_1$ は整数領域であり、$H_1$ に関する仮説は問題を解決する $x$ の存在を暗示しているため、$c_i$、$c \neq 0$ の選択によります。

(ii) $\mathbf{R}/p_i$ が整域であるため、$\mathbf{R}/p_i$ のすべての理想 $\neq 0$ は $\mathbf{R}/p_i$ の理想と等しい基数を持ち、同じことが、$\mathbf{R}/p_i$ の元、よっての結論による理想の翻訳にも当てはまります。

#### 定理 6 {#ac-vii-s4-thm-6 .statement tag=054C}

*M をねじりのない有限生成A-加群とします。 M/L が A のイデアルと同型となるような M の自由な部分加群 L が存在します。*

$M$の*階数*（$K$上の$V = M \otimes_A K$の階数）を$n$で表し、$M$を$A$に関する$V$の格子と考えます。次に、すべての $p \in P(A)$ について、$M_p$ は $A_p$ (no. 1, *例 6*) に対する $V$ の格子であり、$A$ と同様に、主イデアル整域, $M$ は *自由* $A$-階数 $n$ のモジュール。次のように書きます。

$$
M(p) = M_p/pM_p.
$$

$A/p$の分数の$k(p)$体（$A_p$の剰余体と同型）で表します。したがって、$M(p) = M \otimes_A k(p)$ は、$k(p)$ 上の階数 $n$ のベクトル空間です。すべての$x \in M$について、$M(p)$の$x$の$x(p)$標準像で表します。

#### 補題 7 {#ac-vii-s4-lem-7 .statement tag=054D}

*$x_i$ ($1 \leq i \leq m$) を $M$ の元 ($A$ または $K$ 以上、つまり同じ値) として線形独立とし、$L$ を $x_i$ によって生成される $M$ のサブ A モジュールとします。次に、ほぼすべての $p \in P$ について、$x_i(p) \in M(p)$ は $k(p)$ に対して線形独立です。すべての $p \in P$ に対して $k(p)$ にわたって線形独立であるためには、$M/L$ にねじれがないことが必要かつ十分です。*

$x_1, \ldots, x_n$を$M$の元とし、$x_1, \ldots, x_n$、$V$の形基底と合わせて、$N$を$x_i$によって生成された$M$の空きサブAモジュールとします。 ($1 \leq i \leq n$)。 no. 3、定理 3 から、ほぼすべての $p \in P$ について $N = M$ となります。 $k(p)$ に対する $N(p)$ の $x_1(p), \ldots, x_n(p)$ 形基底として、最初の主張が確立されます。

$M/L$ がねじれがない場合、すべての $p \in P$ (no. 1、*例 6*) に対して $(M/L)_p = M_p/L_p$ も同様です。また、$A_p$ が主イデアル整域であるため、$M_p/L_p$ は自由です。したがって、$M$ は $L$ の直和であり、階数 $n - m$ の空き $A$ モジュール $E$ です。したがって、$M(p)$は$L(p)$の直和、およびベクトル$k(p)$-スペース$E/pE$の階数$n - m$です。したがって、$L(p)$ は階数 $m$ であり、$x_i(p)$ ($1 \leq i \leq m$) によって生成されるため、後者は線形独立です。

逆に、$x_i(p)$ ($1 \leq i \leq m$) がすべての $p \in P$ に対して $k(p)$ に対して線形独立であるとします。次に、$L$ は、すべての $p$ (章 II, § 3, no. 2、系 1 ～ 命題 5) に対して、$M$ の直因子であるため、$M_p/L_p = (M/L)_p$ はすべての $p \in P$ に対してねじれがありません。私たちは結論するから $P \cap \operatorname{Ass}(M/L) = \varnothing$ を章 IV, § 1, no. 2, 系から命題 5 とします。しかし、L は再帰的であるため、no. 2, 命題 7 (i) から、 属する ～ $\operatorname{Ass}(M/L)$ が理想 (0) です。したがって、$M/L$ にはねじれがありません。

#### 補題 8 {#ac-vii-s4-lem-8 .statement tag=054E}

※$M$の階数$n$が$\geqslant 2$だとします。その場合、$M/Ax$ にはねじれがないような $M$ の元 $x \neq 0$ が存在します。*

$y \neq 0$を$M$の元とします。 補題 7, $p \in P$ の集合 $Y$ により、$y(p) = 0$ は有限になります。 $Y = \varnothing$ の場合、補題 7 から、単一の元 $y$ の数列 $(x_i)$ からなるに適用され、$M/Ay$ にはねじれがないことがわかります。したがって、$Y \# @$ と仮定して、$S = \bigcap_{p \in Y} (A - p)$ と書きます。私たちは (no. 4, 補題 2) $S^{-1}A$ が半局所的な主イデアル整域であり、その最大理想は $pS^{-1}A$ であり、$p \in Y$、対応する局所環は $A_p$ であることを知っています。したがって、
$$
S^{-1}A/pS^{-1}A = k(p),
$$
よって
$$
S^{-1}M/pS^{-1}M = (M/pM) \otimes_A S^{-1}A = M \otimes_A ((A/p) \otimes_A S^{-1}A) = M \otimes_A k(p) = M(p)
$$
$p \in Y$の皆さんへ。 章 II, § 1, no. 2, 命題 6 までに、元 $z/s \in S^{-1}M$ ($z \in M, s \in S$) が存在します。その $p \in Y$ の $M(p)$ の標準像はすべて $\neq 0$ です。 $S$の定義までなので、すべての$p \in Y$は$z(p) \neq 0$になります。さらに、$y$ と $z$ が $K$ に対して *一次独立* であると仮定することもできます。逆の場合、$y$ から線形独立である元 $t \in M$ を考えてみましょう (このようなものは $n \geqslant 2$ から存在します)。一方、元 $a \neq 0$ 所属を $\bigcap_{p \in Y} p$ に取り（$A$ は整域なので 0 には減りません）、$z' = z + at$ と書きます。明らかに $y$ と $z'$ は $K$ に対して線形独立です。 $p \in Y$すべてに対して$z'(p) = z(p) \neq 0$。

したがって、$y$ と $z$ が $K$ に関して線形独立であると仮定すると、$Z$ は $p \in P - Y$ の集合となり、$y(p)$ と $z(p)$ は $k(p)$ に関して線形独立になります。 補題 7 から、この集合は *有限* であることがわかります。したがって、すべての $p \in Z$ について、$\lambda(p) \in k(p)$ に $z(p) = \lambda(p)y(p)$ と書くことができます。さて、$p \in P$ 全員に対して $\operatorname{Card}(A/p) > 2$;したがって、補題 6 から、すべての $p \in Z$ について、$A/p$ の $b$ の標準像が $\lambda(p)$ とは異なるように、$b \in A$ が存在することがわかります。ここで、元 $x = z - by$ が問題を解くことを示します。 *すべて* $p \in P$ に対して $x(p) \neq 0$ であることを確認するには (補題 7 に $m = 1$ を適用することで) 十分です。今:

— $p \in Y$ の場合、$x(p) \neq 0$ by 構成;
— $p \in Z$ の場合、$x(p) = \mu_p y(p)$ ここで、$b$ の選択により $\mu_p \neq 0$ となり、したがって $y(p) \# 0$ から $x(p) \neq 0$ となります。
— $p \in P - (Y \cup Z)$、$y(p)$、$z(p)$ が線形独立である場合、$x(p) \neq 0$ となります。

これらの補題を確立したら、定理 6 の証明に進みます。$n$ について帰納法によって議論しますが、$M$ 自体が $A$ の理想と同型であるため、$n \leq 1$ のケースは自明です。したがって、$n \geq 2$; と仮定します。 補題 8 のおかげで、階数 1 の $M$ のうち、$M/L_0$ がねじれのない自由な部分加群 $L_0$ が存在します。したがって、$M/L_0$ は階数 $n - 1$ です。 帰納法の仮定までに、$(M/L_0)/L_1$ が $A$ の理想と同型となるような、$M/L_0$ の自由な部分加群 $L$ が存在します。 $L$ を $M$ の $L_1$ の逆像とします。 $L/L_0$ は $L_1$ と同型で、$L_1$ が自由であるため、$L$ は $L_0 \oplus L_1$ (代数, 章 II, § 1, no. 11, 命題 21) と同型であり、したがって自由です。 $M/L$ は $(M/L_0)/L_1$ と同型であるため、定理が示されています。

#### 注意 {#ac-vii-s4-n9-rem-1 .statement tag=054F}

$M$ が再帰的である場合、同じことが必ずしも $M/L$ (練習問題 9) に当てはまるとは限りません。

### 10. dedekind ドメイン上で加群

ここでは、$A$ が Dedekind ドメインであると仮定します。その場合、イデアル $p \in P$ が最大であり、それらが $A$ ($§ 2$, no. 1 ) の唯一の素イデアル $\neq 0$ であることがわかります。 群 $D(A)$ は、$A$ の分数イデアル $\neq 0$ の群 $I(A)$ と同一視されます。

#### 命題 21 {#ac-vii-s4-prop-21 .statement tag=054G}

$A$ を Dedekind ドメインとします。すべての擬似ゼロ $A$ モジュールは零です。すべての擬似単射 (それぞれ擬似全射、擬似全単射、擬似ゼロ) $A$ モジュール準同型は単射 (それぞれ全射、全単射、零) です。

最初の主張はすでに表示されています (no. 4、例 1)。他の人はすぐにそれに続きます。

#### 命題 22 {#ac-vii-s4-prop-22 .statement tag=054H}

$A$ をデデキントドメイン、$M$ を有限生成された $A$ モジュールとします。次のプロパティは同等です。
(a) $M$ はねじれがありません。
(b) $M$ は再帰的です。
(c) $M$ は射影です。

(整域 $A$ に仮定がない) (b) は (a) (no. 2, 注意 1) を意味し、(c) は (b) (代数, 章 II, § 2, no. 7, 系 4 まで) を意味することはすでにわかっています。 命題 14）。 $M$ にねじれがない場合、$A$ に関して $V = M \otimes_A K$ の格子で識別されます。したがって、$M$ は、$A$ が主イデアル整域であるため、すべての最大理想値 $p \in P$ に対する自由な $A_p$ モジュールです。 章 II, § 5, no. 2、定理 1 (b) から結論が導き出されます。

#### 系 {#ac-vii-s4-n10-cor-1 .statement tag=054I}

$M$ を有限生成された $A$ モジュールとし、$T$ をその捩れ部分加群とします。すると、$T$は$M$の直接因数となります。

$M/T$ はねじれがなく有限生成されるため、命題 22 によって射影され、系は代数、章 II, § 2, no. 2、命題 4 から続きます。

#### 命題 23 {#ac-vii-s4-prop-23 .statement tag=054J}

$A$ をデデキントドメイン、$T$ を有限生成された捩れ $A$ モジュールとします。 2 つの有限族 $(n_i)_{i \in I}$ と $(\mathfrak{p}_i)_{i \in I}$ が存在します。ここで、$n_i$ は整数 $\geq 1$ と $P$ の $\mathfrak{p}_i$ 元であり、$T$ は直和と同型です。 $\bigoplus_{i \in I} (A/\mathfrak{p}_i^{n_i})$。さらに、ファミリー $(n_i)_{i \in I}$ と $(\mathfrak{p}_i)_{i \in I}$ は、インデックス付け集合の全単射内で一意です。

これは、擬似同型写像がここ同型にあるという事実を考慮して、no. 4、定理 5 から続きます。

#### 命題 24 {#ac-vii-s4-prop-24 .statement tag=054K}

$A$ をデデキント領域、$M$ を有限生成されたねじれのない $A$ モジュールおよび階数 $n \geq 1$ とします。次に、$M$ が加群 $A^{n-1}$ および $b$ の直和と同型となるような $A$ の理想 $b \neq 0$ が存在します。また、理想$b$の類は、この条件によって一意に決まります。

no. 9の定理 6は、$M/L$が$A$のイデアル$a$と同型であるような$M$の自由部分加群$L$が存在することを示しています。 $a = 0$の場合、$b = A$を採用します。それ以外の場合、$a$ は階数 1 であるため、$L = A^{n-1}$ と $a$ は *射影* 加群 (命題 22) になります。したがって、$M$ は、$L$ および $a$ の直和 (*代数*, 章 II, § 2, no. 2, 命題 4) と同型であり、命題の最初の部分を証明します。さらに、no. 7、命題 16 (i)、(iv)、(v) から、$b$ の類の $c(M) = c(b)$ よって一意性が続きます。

注意
(1) 命題 23 と 24 および系から命題 22 決定するは、有限生成された $A$ モジュールの完全に構造です。 命題 24 は、ねじれのない有限生成された $A$ モジュールが、その *階数* とそれに接続されている *因子* 類によって同型まで決定されることを示しています。
(2) 有限生成されないデデキント領域射影加群上では必ず *自由* (練習問題 21) であり、射影加群のすべての部分加群は射影的 (練習問題 20) であることが示されます。

### 練習問題 {#ac-vii-s4-exercises}

[§ 4 に対して練習問題](exercises/s4/)を参照してください。
