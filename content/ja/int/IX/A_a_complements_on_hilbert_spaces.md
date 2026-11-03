---
book: int
book_title: Integration
chapter: IX
chapter_title: MEASURES ON HAUSDORFF TOPOLOGICAL SPACES
section: 0
section_title: Complements on Hilbert spaces
appendix: true
lang: ja
source: int-vii-ix
book_pages: INT IX.118-INT IX.119
pdf_pages: 0284-0288, 0300-0301
extraction: ocr
subsections:
    - "no": 1
      title: Trace of a quadratic form with respect to another$^{(1)}$
      page: 0
      pdf_page: 284
    - "no": 2
      title: Hilbert–Schmidt mappings$^{(2)}$
      page: 104
      pdf_page: 286
statements: 5
exercises: 9
content_sha256: 92e78b8f1e27427e0a943495e4a12087ed9b074d9bfeb47857611fbfc84e898f
translated_from: content/en/int/IX/A_a_complements_on_hilbert_spaces.md
translation_method: google
source_content_sha256: 345b39c6aa42db2dbb13f3b4da3d834dda0b94e5c0750c5ee630d5f4b9b588d5
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-dda8bbaf
glossary_version: 34
glossary_terms_sha256: 83973e00dc711ea40ad335cf969be389b4d93b181b1ac0ea35a3d3e4aa8c5f30
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## 別館

# ヒルベルトの補足空間

### 1. 他の$^{(1)}$ に対する二次方程式形のトレース

この番号では、$E$ によって実数ベクトル空間を表し、$Q, H$ によって $E$ 上の 2 つの正の二次方程式形を表します。以下の特徴を持つ 2 つの対称的な双線形形式 $(x, y) \mapsto (x|y)_Q$ と $(x, y) \mapsto (x|y)_H$ が存在します。
$$
Q(x) = (x|x)_Q , \quad H(x) = (x|x)_H
$$
$x \in E$ 全員のために。

1 つは H* に関する Q の *trace を呼び出し、もう 1 つは次のように定義される、有限であるかどうかに関係なく、正の実数を $\operatorname{Tr}(Q/H)$ で表します。

a) $H(x) = 0$ と $Q(x) \neq 0$ のような $x \in E$ が存在する場合、集合 $\operatorname{Tr}(Q/H) = +\infty$ が 1 つあります。

b) 逆の場合、$\operatorname{Tr}(Q/H)$ は形 $\sum_{i=1}^p Q(e_i)$ の数の集合の上限であり、$(e_1, \ldots, e_p)$ は $E$ の有限列の元の集合を超えます。 $H$。

$E$ を実ヒルベルト空間とし、$Q$ を $E$ 上の正の二次方程式形とします。 集合 $H(x) = \|x\|^2$ $x \in E$;この場合、$H$ は $E$ 上の正の二次方程式形です。 $\operatorname{Tr}(Q/H)$ が有限であれば、$Q$ は *核* であると言われます。 ノルム 1 の $x \in E$ ごとに、1 つは $Q(x) \leq \operatorname{Tr}(Q/H)$、よって $Q \leq \operatorname{Tr}(Q/H) \cdot H$ になります。特に、すべての核形 $Q$ は連続的です。

#### 注意 {#int-ix-a0-n1-rem-1 .statement tag=09T5}

— 1) $E$ の部分空間 $F$ ごとに、$Q$ から $F$ の$Q_F$ 制限と、$H$ の$H_F$ で表します。すると、$\operatorname{Tr}(Q_F/H_F) \leq \operatorname{Tr}(Q/H)$ と $\operatorname{Tr}(Q/H)$ は、$F \subset E$ 有限次元に対する数 $\operatorname{Tr}(Q_F/H_F)$ の上限となります。

2) $E_1$ を実数ベクトル空間、$Q_1$、$H_1$ を $E_1$ 上の 2 つの正の二次方程式形とし、$\pi : E \to E_1$ を全射線形写像とします。 $Q = Q_1 \circ \pi$ と $H = H_1 \circ \pi$ の場合は、$\operatorname{Tr}(Q/H) = \operatorname{Tr}(Q_1/H_1)$ です。

(1) 参照。テレビ、V, §4, No. 9。

#### 命題 1 {#int-ix-a0-prop-1 .statement tag=09T6}

— *E は有限次元であり、H は非縮退であると仮定します。*

a) *E の x, y に対して * $(x|y)_Q = (u(x)|y)_H$ によって特徴付けられる E の自己準同型 u が存在します*。

b) $\operatorname{Tr}(Q/H) = \operatorname{Tr}(u)$。

c) $\operatorname{Tr}(Q/H) = \sum_{i=1}^m Q(e_i)$ *すべての基底* $(e_1, \ldots, e_m)$ *H* に対する E の正規直交。

*a)* は、双線形形式 $(x, y) \mapsto (x|y)_H$ が非縮退であるという事実から導き出されます。 H の正規直交 E のすべての数列は、H の正規直交 E の基底まで完了できます。その結果、$\operatorname{Tr}(Q/H)$ は、E のすべての基底 $(e_1, \ldots, e_m)$ における、形 $\sum_{i=1}^m Q(e_i)$ の数の集合の上限になります。 *b)* と *c)* を証明するには、この種の基底ごとに $\sum_{i=1}^m Q(e_i) = \operatorname{Tr}(u)$ を示すだけで十分です。 $1 \leq i, j \leq m$ の場合は集合 $a_{ij} = (u(e_i)|e_j)_H = (e_i|e_j)_Q$。次に、$1 \leq i \leq m$、よってに対して $u(e_i) = \sum_{j=1}^m a_{ij} e_j$

$$
\operatorname{Tr}(u) = \sum_{i=1}^m a_{ii} = \sum_{i=1}^m (e_i|e_i)_Q = \sum_{i=1}^m Q(e_i).
$$

Q.E.D.

#### 命題 2 {#int-ix-a0-prop-2 .statement tag=09T7}

— *E が有限次元であると仮定します。 基底* $(e_1, \ldots, e_n)$ *E と整数 m with* $0 \leq m \leq n$ *そのような*

$$
\operatorname{H}\left( \sum_{i=1}^n t_i e_i \right) = \sum_{i=1}^m t_i^2
$$

*for* $t_1, \ldots, t_n$ *本物。さらに、関係* $\operatorname{H}(x) = 0$ が *$x \in E$ に対して *$Q(x) = 0$ *を暗示している場合、*その後* $\operatorname{Tr}(Q/H) = \sum_{i=1}^m Q(e_i)$ となります。

H に対して直交する E の基底 $(e'_1, \ldots, e'_n)$ が存在します。基底は、$1 \leq i \leq m$ に対しては $\operatorname{H}(e'_i) > 0$、$m < i \leq n$ に対しては $\operatorname{H}(e'_i) = 0$ となるような方法でインデックス付けされていると仮定できます。次に、$1 \leq i \leq m$ の場合は集合 $e_i = e'_i / \operatorname{H}(e'_i)^{1/2}$、$m < i \leq n$ の場合は $e_i = e'_i$ です。 関係 (1) は満たされています。

F を $e'_{m+1}, \ldots, e'_n$ によって生成された E の部分空間とします。それは $\operatorname{H}(x) = 0$ となる $x \in E$ の集合です。 E の $\pi$ 標準写像を $E_1 = E/F$ に示します。 Q と H は F 上で零であるため、$E_1$ 上には 2 つの正の 2 次方程式形 $Q_1$ と $H_1$ が存在し、$Q = Q_1 \circ \pi$ と $H = H_1 \circ \pi$ が存在します。さらに、$(\pi(e_1), \ldots, \pi(e_m))$ は $H_1$ の正規直交である $E_1$ の基底であるため、$H_1$ は非縮退です。

提案 1 および *注意 2* により、

$$
\operatorname{Tr}(Q/H) = \operatorname{Tr}(Q_1/H_1) = \sum_{i=1}^m Q_1(\pi(e_i)) = \sum_{i=1}^m Q(e_i).
$$

Q.E.D.

#### 注意 3 {#int-ix-a0-n1-rem-3 .statement tag=09T8}

— E は有限次元、H は非縮退であると仮定します。 $(e_1, \ldots, e_n)$ を E の基底とします。集合 $q = ((e_i|e_j)_Q)_{1 \leq i,j \leq n}$ と $h = ((e_i|e_j)_H)_{1 \leq i,j \leq n}$ です。提案 1 の記法では、E の基底 $(e_1, \ldots, e_n)$ に対する $u$ の行列は、$h^{-1}q$、よってに等しい

(2)
$$
\operatorname{Tr}(Q/H) = \operatorname{Tr}(h^{-1}q) = \operatorname{Tr}(qh^{-1}).
$$

### 2. ヒルベルト＝シュミット写像$^{(2)}$

E を実ヒルベルト空間とし、スカラー 積を $(x|y)$ で表します。 E の双対上には、公式によって特徴付けられる E のアイソメトリ $j_E$ が存在します。

(3)
$$
(x|y) = \langle x, j_E(y) \rangle \quad \text{for } x, y \text{ in E}
$$
(TVS、V, §1, No. 7、Th. 3)。

$E_1$ と $E_2$ を 2 つの実際のヒルベルト空間と、$u$ を $E_1$ から $E_2$ への連続線形写像とする。 $E_2$ から $E_1$ への連続線形写像 $u^* = j_{E_1}^{-1} \circ {}^t u \circ j_{E_2}$ を *u の随伴* と呼びます。 写像 $u^*$ は関係によって特徴付けられます

(4)
$$
(u(x_1)|x_2) = (x_1|u^*(x_2)) \quad \text{for } x_1 \in E_1,\ x_2 \in E_2.
$$

$v$ が $E_2$ の連続線形写像でヒルベルト空間 $E_3$ になる場合、$(v \circ u)^* = u^* \circ v^*$ になります。

$E_1$と$E_2$を、$E_1$を$E_2$に変換した2つの実際のヒルベルト空間と$u$線形写像とする。 1 つの定義する 2 つの正の二次方程式形 $E_1$ の公式による H と Q

$$
H(x) = \|x\|^2,\quad Q(x) = \|u(x)\|^2 \quad (x \in E_1).
$$

#### 命題 3 {#int-ix-a0-prop-3 .statement tag=09T9}

*u が連続であると仮定します。 $(e_i)_{i \in I}$ を $E_1$ の正規直交基底とし、$(f_j)_{j \in J}$ を $E_2$ の正規直交基底とします。それから*

$$
\operatorname{Tr}(Q|H) = \sum_{i \in I} \|u(e_i)\|^2 = \sum_{j \in J} \|u^*(f_j)\|^2 = \sum_{i \in I} \sum_{j \in J} (u(e_i)|f_j)^2.
$$

(2) 参照。テレビ、V, §4, No. 7。

$x \in E_1$ ごとに $\|x\|^2 = \sum_{i \in I} (x|e_i)^2$ があり、同様に $y \in E_2$ ごとに $\|y\|^2 = \sum_{j \in J} (y|f_j)^2$ があります。その結果、

$$
\sum_{i \in I} \|u(e_i)\|^2 = \sum_{i \in I} \sum_{j \in J} (u(e_i)|f_j)^2 \\
= \sum_{j \in J} \sum_{i \in I} (e_i|u^*(f_j))^2 \\
= \sum_{j \in J} \|u^*(f_j)\|^2 .
$$

特に、数 $\sum_{i \in I} \|u(e_i)\|^2$ は、$E_1$ の正規直交基底 $(e_i)_{i \in I}$ から独立しています。

集合 $t = \operatorname{Tr}(Q|H)$。 $I$ の有限部分集合 $I'$ ごとに、定義まで

$$
\sum_{i \in I'} \|u(e_i)\|^2 = \sum_{i \in I'} Q(e_i) \leq t ,
$$

よって $\sum_{i \in I} \|u(e_i)\|^2 \leq t$。 $(e'_1, \ldots, e'_p)$ を $E$ の有限正規直交関数数列とします。この数列は、$E_1$ の正規直交基底 $(e'_\alpha)_{\alpha \in A}$ まで完成できます。それから

$$
\sum_{\alpha=1}^p \|u(e'_\alpha)\|^2 \leq \sum_{\alpha \in A} \|u(e'_\alpha)\|^2 = \sum_{i \in I} \|u(e_i)\|^2
$$

そして、すべての $(e'_1, \ldots, e'_p)$ の最高値に対して移行を加えると、不等式 $t \leq \sum_{i \in I} \|u(e_i)\|^2$ が得られます。従って、等式 $t = \sum_{i \in I} \|u(e_i)\|^2$ を確立しました。

Q.E.D.

$E_1$ 上の正の二次方程式形 $Q : x \mapsto \|u(x)\|^2$ が核である場合、$u$ は $E_1$ の *ヒルベルト・シュミット写像* であり、$E_2$ になると言われています。この場合、$Q \leq \operatorname{Tr}(Q/H) \cdot H$ があるため、$u$ は連続であり、

$$
\|u\| \leq \operatorname{Tr}(Q/H)^{1/2} .
$$

$u : E_1 \to E_2$ を連続した線形写像とします。提案 3 により、$\sum_{i \in I} \|u(e_i)\|^2 < +\infty$ となるような$E_1$ の正規直交基底 $(e_i)_{i \in I}$ が存在する場合に限り、$u$ はヒルベルト・シュミット写像になります。この場合、$E_1$ のすべての正規直交基底は同じ性質を持ちます。さらに、$u$ がヒルベルト・シュミット写像である場合、公式 $\sum_{i \in I} \|u(e_i)\|^2 = \sum_{j \in J} \|u^*(f_j)\|^2$ により、その随伴物 $u^*$ も同様になります (提案 3)。

練習問題

### 練習問題 {#int-ix-a0-exercises}

[練習問題付録 0](exercises/a0/)を参照してください。
