---
book: ac
book_title: Commutative Algebra
chapter: IV
chapter_title: ASSOCIATED PRIME IDEALS AND PRIMARY DECOMPOSITION
section: 3
section_title: Primary decomposition in graded modules
lang: ja
source: ac-i-vii
book_pages: 283-285, 301
pdf_pages: 0303-0305, 0321-0321
extraction: ocr
subsections:
    - "no": 1
      title: PRIME IDEALS ASSOCIATED WITH A GRADED MODULE
      page: 283
      pdf_page: 303
    - "no": 2
      title: PRIMARY SUBMODULES CORRESPONDING TO GRADED PRIME IDEALS
      page: 284
      pdf_page: 304
    - "no": 3
      title: PRIMARY DECOMPOSITION IN GRADED MODULES
      page: 285
      pdf_page: 305
statements: 6
exercises: 3
content_sha256: 4267332f90136a215d441d9b57dbd52f0557dec95ac155ef5451f631468febf2
translated_from: content/en/ac/IV/03_s3_primary_decomposition_in_graded_modules.md
translation_method: google
source_content_sha256: 44d441232ef2de6c8b1ed43a9b9091b103360b9960ee00be0b5d251f8b5a5aff
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: 062012bcb1fc13da658fa56b28f59b5a3a2f5dcc285ec59113f236a6c81df6c8
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## 3. 初級分解グレード加群

### 1. グレード加群に関連付けられた主要な理想

#### 命題 1 {#ac-iv-s3-prop-1 .statement tag=04MJ}

$A$ をねじりなし可換群、$A$ を型 $A$ の等級付けされた環、および $M$ を型 $A$ の等級付けされた $A$ 加群とする。 $M$ に関連付けられたすべての素理想は等級付けされ、$M$ の同種の元の消滅子になります。

$A$ には、その群構造 (代数、章 II, § 11, no. 4、補題 2) と互換性のある合計位数構造を与えることができることがわかっています。 $p$ を $M$、元 $x \in M$ の消滅子に関連付けられた主要イデアとし、$(x_i)_{i \in \Delta}$ を$x$ の同種成分の族とする。 $i(1) < i(2) < \cdots < i(r)$ を $i$ の値とし、$x_i \neq 0$ とします。 元 $a \in p$ を考え、$(a_i)_{i \in \Delta}$ をその同種成分の族とします。すべての $i \in A$ に対して $a, \in p$ であることを証明し、$p$ が段階的な理想であることを示します。

添字 $i$ の数について帰納法によって $a, \neq 0$ となるように議論します。この数が 0 であれば、私たちの主張は明らかです。そうでない場合は、$m$ を添字 $i$ のうち最大のとし、$a, \neq 0$ とします。 $a, \in p$ を証明すると、帰納法の仮定を $a - a,$ に適用すると結論が得られます。さて、$ax = 0$;すべての $j \in A$ について、$ax$ の次数 $m + j$ の同次成分が 0 であるという事実を使用して、次のようになります。
$$
\sum_{i \in \Delta} a_{m-i} x_{j+i} = 0;
$$
私たちは結論する、その$a_m x_j$は添字$i > j$の$x_i$の線形結合です。したがって、特に $n < r$、$a_m^{r-n+1} x_{i(n)} = 0$ で帰納法を下降することで、$a_m x_{i(r)} = 0$、よってになります。次に、$a_m^r x = 0$、よって $a_m^r \in p$、そして$p$ は素数なので、$a, \in p$ となります。

ここで、$p$ が $M$ の同次元の消滅子であることを示します。 $1 \leq n \leq r$を$b_n = \operatorname{Ann}(x_{i(n)})$と書きましょう。 $p$ のすべての同次元 $b$ とすべての $n$ について、次数 $i(n) + \deg(b)$ の $bx$ の同次成分は $bx_{i(n)}$、したがって $bx_{i(n)} = 0$、したがって $b \in 6$ です。 $p$ は同種の元、$p \subset 6$ によって生成されます。一方、明らかに$\bigcap_{n=1}^r 6_n \subset \operatorname{Ann}(x) = p$; $p$ が素数であるため、$b_n \subset p$ (章 11, § 1, no. 1, 命題 1)、よって $b_n = P = \operatorname{Ann}(x_{i(n)})$ のような $n$ が存在し、証明が完成します。

#### 系 {#ac-iv-s3-n1-cor-1 .statement tag=04MK}

等級付けされた$A$モジュール$M$に関連付けられたすべての（必然的に等級付けされた）素イデアル$p$に対して、等級付けされた$A$モジュール$A/p$から逓減によって得られる等級付けされた$A$モジュール$(A/p)(k)$が得られるような添字$k \in A$が存在します。 $k$ (代数, 章 II, § 11, no. 2) による次数は、$M$ の等級付けされた部分加群と同型です。

命題 1 の証明の表記法を使用して、$A$ から $M$ の準同型性 $a \mapsto ax_{i(n)}$ から商を取ることによって得られる準同型性を考えます。後者は、次数 $i(n)$ の段階的準同型性であり、したがって、商を $A/p$ の次数 $i(n)$ の段階的全単射準同型性を $M$ の段階的部分加群に与えることができます。

#### 命題 2 {#ac-iv-s3-prop-2 .statement tag=04ML}

*$A$ をねじりなし可換群、$A$ 型 $A$ の段階付きネーター 環、および $M$ を型の段階付き有限生成 $A$ 加群とする$A$。 $M$ の段階的サブモジュールから構成される合成系列 $(\mathbf{M}_i)_{0 \leq i \leq n}$ が存在し、$0 \leq i \leq n - 1$ に対して段階的モジュール $\mathbf{M}_i / \mathbf{M}_{i+1}$ がシフトされた段階的モジュール $(A/p_i)(k_i)$ と同型になります。ここで、$p_i$ は $A$ と $k_i \in A$ の段階的素数イデアルです*。

§ 1, no. 4 の議論をたどるだけで十分です。定理 1 は、この機会に $\mathscr{G}$ を、ステートメントのプロパティを持つ合成系列を持つ $M$ の段階的サブモジュールのセットとみなします。命題 1 の帰結を使用して結論を​​導き出します。

### 2. プライマリ部分加群対応するから段階的なプライマリ理想まで

#### 命題 3 {#ac-iv-s3-prop-3 .statement tag=04MM}

*$A$ をねじりなし可換式群、$A$ ネーター 環の型 $A$、$p$ を $A$ と $M$ の段階的理想とする型 $A$ の $A$ モジュールは $0$ に縮小されません。 $M$ の比 $a$ の$p$ ホモテティー のすべての同次元 $a$ がほぼゼロポテンシャルであり、$A - p$ のすべての同次元 $b$ がほぼゼロであると仮定します。 $M$ に対する比 $b$ のホモテティー は単射です。この場合、$p$ は素数であり、$M$ の部分加群 $\{0\}$ は $p$-素数です*。

$\operatorname{Ass}(M) = \{p\}$ (§ 2, no. 1, 命題 1) を示すだけで十分です。 $q$ を $M$ に関連付けられた主要な理想とする。それは段階的な理想であり、同種の元 $x \neq 0$ の $M$ (no. 1、命題 1) の消滅子です。 $q$、$ax = 0$ のすべての同次元 $a$ に対して、$M$ に対する比 $a$ のホモテティー は単射的ではなく、よって $a \in p$ です。逆に、$b$ を $p$ の同次元とします。 $b^n x = 0$、よって $b^n \in \operatorname{Ann}(x) = q$ となる整数 $n > 0$ が存在し、$q$ は素数であるため、$b \in q$ となります。 $p$ と $q$ は、それぞれ同種の元、$p = q$ によって生成されるため、$\operatorname{Ass}(M) \subset \{p\}$ であることが証明されます。 $M \neq \{0\}, \operatorname{Ass}(M) \# \varnothing$ (§ 1, no. 1、系 1 ～ 命題 2)、よって $\operatorname{Ass}(M) = \{p\}$ として。

#### 命題 4 {#ac-iv-s3-prop-4 .statement tag=04MN}

*$A$ をねじりなし可換群、$A$ を型 $A$ の等級付けされたネーター 環、および $M$ を型の等級付けされた $A$ 加群とする$A$。 $p$を$A$と$N$の主イデアル、$M$に関して$p$主である$M$の部分加群とする。

(i) $p$ (代数, 章 11, § 11, no. 3) に含まれる $A$ の最大の段階イデアル $p'$ は素数です。

(ii) $N$ の最大の段階的サブモジュール $N'$ は、$M$ に関して $p'$-1 次です。

私たちは、$p'$ (それぞれ $N'$) の同種元は、$p$ (それぞれ $N$) の同種元であることを知っています (*loc. cit.*)。 $a$ を $p$ の同次元とします。 $x$ が $M$ の同次元である場合、 $a^n x \in N$ となる整数 $n > 0$ が存在します。 $a^n x$ は同次であるため、$a^n x \in N'$;すべての $y \in M$ は同次元の有限数の直和であるため、 $a^q y \in N'$ となる整数 $q > 0$ が存在することになり、$a$ の比率を持つホモテティー が存在すると結論する $M/N'$ はほぼ無力です。

ここで、$A - p'$ の同次元 $b$ を考えてみましょう。次に、$b$ は同次であるため、$b \notin p$ となります。 $x$ を $bx \in N'$ となるような $M$ の元とし、$(x_i)_{i \in \Delta}$ を $x$ の同種成分の族とする。 $N'$ はすべての $i$ に対して $bx_i \in N'$ であるため、$bx_i \in N$ となり、$b \notin p$ として、$x_i \in N$ は結論するとなります。 $x_i$ は同次であるため、$x_i \in N'$、よって $x \in N'$、ホモテティー は$M/N'$ に対する比 $b$ が単射です。 命題 4 は、命題 3 から$p'$ と $M/N'$ に適用されます。

### 3. 小学校分解 、等級加群

#### 命題 5 {#ac-iv-s3-prop-5 .statement tag=04MO}

$A$ をねじりなし可換群、$A$ 型 $A$ の段階付きネーター 環、$M$ 型の段階付き $A$ 加群とする$M$、$N$は$M$の部分加群、$N = \bigcap_{i \in I} Q_i$は$M$の$N$の主要な分解です。

(i) $Q'_i$ を、$Q_i$ に含まれる$M$ の部分加群を最大のとします。次に、$Q'_i$ がプライマリ、$N = \bigcap_{i \in I} Q'_i$ です。

(ii) 主要な分解 $N = \bigcap_{i \in I} Q_i$ が減少すると、主要な分解 $N = \bigcap_{i \in I} Q'_i$ も減少し、すべての $i \in I$ について、主要な理想対応するから $Q_i$ および $Q'_i$ が等しくなります。

(iii) $\operatorname{Ass}(M/N)$ の最小値元である主要理想値 $p_i$ に対して $Q_i$ 対応するの場合、$Q_i$ は $M$ の等級付けされた部分加群です。

$Q'_i$ が $M$ と $N \subset Q'' \subset Q_i$ に関して主要であること (no. 2, 命題 4) を見てきました。これは (i) を証明します。 no. 2 の命題は、主イデアル $p'_i$ 対応するから $Q'_i$ が、主イデアル $p_i$ 対応するから $Q_i$ に含まれる最大の段階イデアルであることも示しています。 分解 $N = \bigcap_{i \in I} Q_i$ が減少すると、すべての $i$ (§ 2, no. 3、命題 4) に対して $p_i \in \operatorname{Ass}(M/N)$ となるため、$p_i$ は段階的な理想値 (no. 1、命題 1) となり、したがって $p'_i = p_i$ となります。次に、$\operatorname{Ass}(M/N) = \bigcup_{i \in I} \{p'_i\}$ (§ 2, no. 3, 命題 4) です。これは、分解 $N = \bigcap_{i \in I} Q'_i$ が縮小されることを証明します (§ 2, no. 3, 命題 4)。最後に、$p_i$ が $\operatorname{Ass}(M/N)$ の最小値元である場合、$p_i$ は (no. 1, 命題 1)、§ 2, no. 3 によりよって $Q'_i = Q_i$ に格付けされるので、$p'_i = p_i$ となります。 命題 5.

### 練習問題 {#ac-iv-s3-exercises}

[§ 3 に対して練習問題](exercises/s3/)を参照してください。
