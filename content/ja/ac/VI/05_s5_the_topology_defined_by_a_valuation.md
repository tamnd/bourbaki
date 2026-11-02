---
book: ac
book_title: Commutative Algebra
chapter: VI
chapter_title: VALUATIONS
section: 5
section_title: The topology defined by a valuation
lang: ja
source: ac-i-vii
book_pages: 399-403, 454-459
pdf_pages: 0417-0421, 0472-0477
extraction: ocr
subsections:
    - "no": 1
      title: THE TOPOLOGY DEFINED BY A VALUATION
      page: 399
      pdf_page: 417
    - "no": 2
      title: TOPOLOGICAL VECTOR SPACES OVER A FIELD WITH A VALUATION
      page: 401
      pdf_page: 419
    - "no": 3
      title: THE COMPLETION OF A FIELD WITH A VALUATION
      page: 402
      pdf_page: 420
statements: 10
exercises: 10
content_sha256: 31caaa77834a0270f66807aa0e95c6e58229f5539a843aafe692752ef32f210d
translated_from: content/en/ac/VI/05_s5_the_topology_defined_by_a_valuation.md
translation_method: google
source_content_sha256: f97824efc1e49c2f3f557cc487ce4e195405a030102d3750617c5a288f2ba3cd
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-eeeca2ef
glossary_version: 34
glossary_terms_sha256: cbf91fe9a9ee5f5ae3ecf797ff80c11c0b032bba5067248843ed93d3d1d9c4b7
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## 5. 位相評価によって定義される

### 1. 位相評価によって定義される

K が必ずしも可換体である必要はなく、K と G の評価は完全に順序付けられた群 $v(K^*)$ であるとします。すべての $a \in G$ について、V を $v(x) > a$ となるような $x \in K$ の集合とします。この集合は K (§ 3, no. 1) の添加物部分群です。 K には固有の位相 $\mathscr{T}_v$ が存在し、その V、形は 0 の近傍の基本系 (*一般位相*、章 III, § 1, no. 2、例) です。 v が不適切であるためには、$\mathscr{T}_v$ が離散値位相であることが必要かつ十分です。

#### 補題 1 {#ac-vi-s5-lem-1 .statement tag=04UQ}

*$x \in K^*, y \in K^*$と$\alpha \in G$としましょう。もし*
$$
v(x - y) > \sup(\alpha + 2v(y), v(y)),
$$
*その後* $v(x^{-1} - y^{-1}) > a$。

$x^{-1} - y^{-1} = x^{-1}(y - x)y^{-1}$ そしてそれ以降
$$
v(x^{-1} - y^{-1}) = v(x - y) - v(x) - v(y).
$$
$v(x - y) > v(y)$ の場合、§ 3, no. 1 の 1 である命題は、$x = y + (x - y)$ 以降、$v(x) = v(y)$ であることを意味します。さらに、$v(x - y) > a + 2v(y)$ の場合、
$$
v(x^{-1} - y^{-1}) > a + 2v(y) - 2v(y) = a.
$$

#### 命題 1 {#ac-vi-s5-prop-1 .statement tag=04UR}

*位相 $\mathscr{T}_v$ はハウスドルフであり、K 上の体構造と互換性があります。 G に離散位相が与えられた場合、写像 $v : K^* \to G$ は連続です。*

$x \in K^*$ と $a = v(x)$ としましょう。次に $x \notin V_a$ ですが、これは $\mathscr{T}_v$ がハウスドルフであることを示しています。すべての$x_0 \in K$と$a \in G$に対して、$x_0 V_\beta \subset V_\alpha$と$V_\beta x_0 \subset V$のような$\beta \in G$が存在します（$\beta \geqslant a - v(x_0)$を取るだけで十分です）。一方、$a \geqslant 0$の場合は、$V_\alpha V_\alpha \subset V_v$となります。 *一般位相*、章 III, § 6, no. 3 の公理 (AV_I) と (AV_{II}) はこのように満たされ、$\mathscr{T}_v$ は $K$ 上の環構造と互換性があります。 $x_0 \in K^*$ にしましょう。 $x \in K^*$ が $v(x - x_0) > \sup(\alpha + 2v(x_0), v(x_0))$ を満たす場合、$v(x^{-1} - x_0^{-1}) > a$ (補題 1) になります。これは、$x \mapsto x^{-1}$ が連続であり、したがって $\mathscr{T}_v$ が $K$ 上の体構造と互換性があることを示します。最後に、単一の条件 $v(x - x_0) > v(x_0)$ は $v(x) = v(x_0)$ ($§ 3$, no. 1, 命題 1) を意味するため、$G$ に離散位相が与えられた場合、写像 $v : K^* \to G$ は連続です。

$\alpha \in G$ と $V'_\alpha$ を $v(x) \geq \alpha$ となるような $x \in K$ の集合とします。 $\beta < a$なら$V_\beta \supset V'_\alpha \supset V_v$。したがって、$v$ が不適切でない場合、$V'_\alpha$ 形は、$\mathscr{T}_v$ の 0 の近傍の基本的な系であることがわかります。

$V_v$ と $V'_\alpha$ は開いた加法部分群であるため、$K$ で閉じられており、したがってトポロジカル体 $K$ は *完全に切断* されます。 $v$ 含むの環と $V_v$ のゼロ以外の理想はすべて、$K$ で *開いたり閉じたり*します。したがって、$v$ の剰余体上の商位相は *離散* です。

$A$を$u$の環とします。 $v$ が離散の場合、$§ 3$、no. 6 の命題 8 は、$A$ 上の $\mathscr{T}_v$ によって誘導された位相が $m(A)$ 進数位相であることを示します。一般的にはそうではありません (練習問題 4)。

#### 命題 2 {#ac-vi-s5-prop-2 .statement tag=04US}

*$K$は必ずしも可換体ではなく、$v$は$K$、$A$、環の$v$、$m$は$v$の理想であり、不当ではない評価とします。 $K$ と位相 $\mathscr{T}_v$ が局所的にコンパクトになるには、次の条件が満たされることが必要かつ十分です。

(i) $K$ が完了している。
(ii) $v$ は離散的です。
(iii) *剰余体 $\kappa(A)$ は有限です。*

*そうであれば*、$A$はコンパクトです。

$K$ が局所的にコンパクトであると仮定します。これで完了です (*一般位相*、章 111、$§ 3$、no. 3、系 1 ～ 命題 4);さらに、0 のコンパクトな近傍が存在し、これは含む近傍 $V'_a$、ここで $a$ 属するから $v$ の値群です。他の語では、$K^*$に$a \neq 0$が存在し、$A . a$がコンパクトになり、$A = (A . a)a^{-1}$がコンパクトになります。 $A$ のすべての理想 $b \neq (0)$ が開いているため、$A/b$ はコンパクトで離散的 (*一般位相*、章 III、$§ 2$、no. 5、命題 14) であるため、有限であり、特に$\kappa(A) = A/m$ は有限です。さらに、$m$、環 $A/Ay$ の$y \neq 0$ が有限であるため、$A$ 含む $Ay$ と集合 $P$ という有限の理想は数しか存在しません。 元の形 $v(x)$ は次のようになります

$$
0 < v(x) \leq v(y)
$$

有限である。 $v(K^*)$ は完全に順序付けされているため、$P$ には最小の元 $y$ があります。次に、$v(x) > 0$、$v(x) > v(y) \geq y$、または $v(x) \leq v(y)$ のようなすべての $x \in A$ に対して、$v(x) \geq y$ 定義を足し、$y$ が $v(K^*)$ の元 $> 0$ の最小値になります。 *$P$ *は有限*であるため、$my \in P$, よって私の \leq v(y) < (m+1)\gamma となる最大の整数 $m \geq 0$ が存在します。 0 \leq v(y) - my < y であると推定され、y の定義によって、これは $v(y) = my$ を意味します。したがって、$v(K^*) = \mathbf{Z}.\gamma$ と評価 $v$ は離散的です。

逆に、条件 (i)、(ii)、(iii) が成り立つとします。私たちは、$v$ が標準である場合に注意を限定するかもしれません。 $u$ を $v$ の均一化要素にします。すると$\kappa(A) = A/Au$、したがって$A/Au$は有限になります。 加法群 $A/Au$ の商同型を $Au^n/Au^{n+1}$ に乗じて $x \mapsto xu^n$ 定義するとなるため、$A/Au^j$ はすべての $j \geq 0$ に対して有限になります。 $A$ は $K$ で閉じられているため、完全であり、したがって $A/Au^j$ の逆行列極限 (一般位相、章 111、§ 7, no. 3、命題 2) と同型であり、したがってコンパクトです。 $A$ は $K$ でオープンであるため、$K$ は局所的にコンパクトであることがわかります。

#### 注意 {#ac-vi-s5-n1-rem-1 .statement tag=04UT}

この証明では、$A$ が完了していると想定するだけで十分であることに注意してください。

§ 9 で、命題 2 の条件を満たす体 $K$ は、$p$ 進体の有限代数拡大である中心を認めるか、または体 $\mathbf{F}_q((T))$ の正式な冪系列が有限体を超えます。さらに、$K$ は、中心よりも有限階数です。

### 2. 評価付きのトポロジカルベクトル空間体

全体を通して、$K$ を (必ずしも可換ではない) 体、$v$ を $K$ および $G$ の位数群とします。 $K$ には位相 $\mathscr{T}_v$ が与えられます。

#### 命題 3 {#ac-vi-s5-prop-3 .statement tag=04UU}

$E$ を、ハウスドルフである次元 1 の $K$ 上の左トポロジー ベクトル空間とします。 $v$ が不適切ではないとします。 $E$ のすべての $x_0 \neq 0$ について、$K_s$ の $E$ 上の写像 $a \mapsto ax_0$ はトポロジカルな同型です。

この写像は連続代数同型です。 共連続であることを示せば十分です。 $\alpha \in G$ にしましょう。 $E$ に 0 の近傍 $V$ が存在し、関係 $ax_0 \in V$ が $v(a) > a$ を意味することを示す必要があります。 $a, \in K^*$ を $v(a_0) = a$ となるようにします。 $E$はハウスドルフなので、$E$には$a_0x_0 \notin W$となるような0の近傍$W$が存在します。 As $v$ is not improper, there exist a neighbourhood $W'$ of 0 in $E$ and an element $\beta$ of $G$ such that the relations $y \in W'$, $v(a) \geq \beta$ imply $ay \in W$. $a, \in K^*$ を $v(a_1) = -\beta$ となるようにします。 関係 $ax_0 \in a_1^{-1}W'$ と $v(a) \leq a$ は $a_1ax_0 \in W$ と $v(a_0a^{-1}a_1^{-1}) = \alpha + \beta - v(a) \geq \beta$ を暗示し、したがって $a_0x_0 = a_0a^{-1}a_1^{-1}(a_1ax_0) \in W$ になりますが、これは不合理です。他の語、関係 $ax, \in a_1^{-1}W$ は $v(a) > a$ を意味します。

#### 系 {#ac-vi-s5-n2-cor-1 .statement tag=04UV}

$E$ を、$K$、$H$ $E$ の閉じた超平面、および $D$ $E$ の 1 次元ベクトル部分空間、の代数補充上の左位相ベクトル空間とします。 $H$。 $v$ が不正ではないとします。この場合、$D$ は $H$ のトポロジカル補充です。

命題 1 と 3 を考慮すると、証明は位相幾何学的ベクトル空間、章 I, § 2、系 2 ～ 定理 1 と同じです。

#### 命題 4 {#ac-vi-s5-prop-4 .statement tag=04UW}

$v$ は不正ではなく、$K$ は完了しているとします。 $E$ を $K$ 上の左トポロジー ベクトル空間とします。これはハウスドルフであり、有限次元 $n$ のです。 $K$ 上の $E$ のすべての基底 $(e_i)_{1 \leq i \leq n}$ について、$E$ 上の $K^n_s$ の写像 $(a_i) \mapsto \sum_{i=1}^n a_i e_i$ はトポロジカルベクトル空間同型です。

命題 3 とその系を考慮すると、証明はトポロジカルベクトル空間、章 I, § 2、定理 2 と同じです。

#### 系 {#ac-vi-s5-n2-cor-2 .statement tag=04UX}

$v$ は不正ではなく、$K$ は完了しているとします。 $E$ を $K$ 上のハウスドルフ位相位相ベクトル空間とし、$F$ を $E$ の有限次元ベクトル部分空間とします。その後、$F$は閉じられます。

$F$が完成しました。

### 3. 評価を伴う体の完了

#### 命題 5 {#ac-vi-s5-prop-5 .statement tag=04UY}

$K$ は必ずしも可換体ではなく、$v$ は$K$ と$G$ 群 $v(K^*)$ を離散位相で評価したものとします。

(a) $K$ の完成環 $\hat{K}$ ($\mathscr{T}_v$ による) はトポロジカル体です。

(b) 写像 $v : K^* \to G$ は、連続する写像 $8 : \hat{K}^* \to G$ に一意に拡張できます。 写像 $0$ ($\hat{v}(0) = +\infty$ で延長) は、$\hat{K}$ と $\hat{v}(\hat{K}^*) = v(K^*)$ の評価です。

(c) $\hat{K}$ の位相は、評価 $0$ によって定義される位相です。

(d) すべての $a \in G$ について、$V_\alpha, V'_\alpha$ を条件 $v(x) > a, v(x) \geq a$ によって定義される $K$ の部分群とします。次に、$\hat{K}$ の$V_\alpha, V'_\alpha$ のクロージャ $\overline{V}_\alpha, \overline{V}'_\alpha$ は、それぞれ条件 $\hat{v}(x) > a, \hat{v}(x) \geq a$ によって定義されます。

(e) $0$ の環は、環 $A$ の $v$ の$\hat{A}$ の完了です。 $0$の理想は、$v$の理想$m$の完成$\hat{m}$です。

(f) $\hat{A} = A + m$; $8$ の剰余体は、標準的に $v$ の剰余体と同一視されます。

(a) を証明するには、次のことを示すだけで十分です (一般位相, 章 III, § 6, no. 8, 命題 7): $\mathfrak{F}$ を、$0$ がクラスターではない$K^*$ に対する (加法一様性構造に関して) コーシー フィルターとします。 点;この場合、全単射 $x \mapsto x^{-1}$ の下の $\mathfrak{F}$ の像はコーシー フィルターです (加法均一構造に関して)。なぜなら、$0$は$\mathfrak{F}$のクラスター点ではないので、$\beta$が$v(M)$の上界となるような$M \in \mathfrak{F}$と$\beta \in G$が存在するからです。 $a \in G$ にしましょう。 $M'$が$M$に含まれる$\mathfrak{F}$の元で、$x \in M'$と$y \in M'$が$v(x - y) > \sup(\alpha + 2\beta, \beta)$である場合、$x \in M'$と$y \in M'$は$v(x^{-1} - y^{-1}) > a$（no. 1、 補題 1)。 よって (a)。

no. 1 の命題 1 により、$v|K^*$ は $K^*$ から $G$ までの連続準同型であるため、$K^*$ から $G$ までの連続準同型 $0$ に一意に拡張できます。 関係

$$
\hat{v}(x + y) \geq \inf(\hat{v}(x), \hat{v}(y))
$$

$K^*$ で成り立つので、連続性により $\hat{K}^*$ でも成り立ちます。したがって、0 ($\hat{v}(0) = +\infty$ で拡張) は $\mathbf{K}$ の評価であり、(b) が証明されます。

次に (d) を示します。 $a \in G$と$x \in \mathscr{S}, -\{0\}$としましょう。 $V$ の $y$ については、$x$、$\hat{v}(x) = \hat{v}(y) = v(y)$、したがって $\hat{v}(x) > a$ に十分に近いです。逆に、$x \in \hat{K}^*$ を $\hat{v}(x) > a$ となるようにします。 $K^*$の$y$は$x$、$v(y) = \hat{v}(y) = \hat{v}(x)$に十分近いため、$y \in V$、よって $x \in \mathscr{S}$になります。したがって、$\mathscr{S}$ は $x \in \hat{K}$ の集合となり、$\hat{v}(x) > a$ となります。この議論は $V'_a$ についても同様です。これは (d) を証明します。

一般位相、章 III, § 3, no. 4の命題7を考慮すると、主張(c)は(d)の帰結となります。 主張 (e) は (d) の特殊なケースです。最後に $x \in \hat{A}$ にしましょう。 $\hat{v}(x - y) > 0$ となるような $y \in A$ が存在します。次に$z = x - y \in \hat{m}$、したがって$x = y + z \in A + \hat{m}$;したがって、$\hat{A} = A + \hat{m}$ は (f) を示します。

#### 注意 {#ac-vi-s5-n3-rem-1 .statement tag=04UZ}

所属から $\hat{A}$ までではないすべての $x \in \hat{K}$ について、$\hat{v}(x - x_0) > 0$、$\hat{v}(x) = \hat{v}(x_0) = v(x_0) < 0$ のような $x_0 \in K$ が存在します。次に、$x_0^{-1} x \in \hat{A}$、そして$x_0^{-1} \in A$ として、集合 $S = A - \{0\}$ とすれば、$\hat{K} = S^{-1} \hat{A}$ を書くことができることがわかります。

### 練習問題 {#ac-vi-s5-exercises}

次数 $n > 1$ など $a_i \neq 0$; 区間 $[0, n]$ に次のような真に増加する数列 $(i_k)_{0 \leq k \leq r}$ の整数が存在することを示します: (1) $i_0 = 0$, $i_r = n$; (2) $v(a_{i_k})$ は $0 \leq k \leq r$ に対して有限です。 (3) $0 \leq j \leq n$ が $i_k$ とは異なり、$v(a_j)$ が有限であるように、添字 $j$ ごとに、点
$$
(j, v(a_j)) \in \mathbf{R}^2
$$
移行から点 $(i_k, v(a_{i_k}))$ および $(i_{k+1}, v(a_{i_{k+1}}))$ の線の上にあり、$j < i_k$ または $j > i_{k+1}$ の場合は厳密にその線の上にあります。 点 $(i_k, v(a_{i_k}))$ と $(i_{k+1}, v(a_{i_{k+1}}))$ を結ぶ線分のうち和集合は P のニュートン多角形と呼ばれ、上記の線分は多角形の辺、点 $(i_k, v(a_{i_k}))$ は頂点と呼ばれます。

(b) K に対する P 属するのすべての零を仮定します。P のすべての零の評価が同じであるためには、$r = 1$ (他の語ではニュートン多角形簡約するが 1 辺になる) が必要かつ十分であることを示します。 (条件が十分であることを示すために、$P_1$ のすべての零が $v$ の環で反転可能である一方で、$P_2$ 属するのすべての積 $P_1P_2$ のニュートン多角形を考えてみましょう。 $v$。)

(c) P 属するのすべての零が K になるとします。 形 P のニュートン多角形を書きます。
$$
\rho_k = i_{k+1} - i_k, \quad \sigma_k = (v(a_{i_{k+1}}) - v(a_{i_k}))/\rho_k.
$$
$0 \leq k \leq r - 1$ について、P は正確に $\rho_k$ 零 (重複度の位数と数えて) を認め、その評価はすべて $\sigma_k$ に等しいことを示してください ((b) を使用し、$r$ で帰納法によって議論します)。

(d) 任意の評価 $v$ の場合に一般化します ($v$ の位数群 $\Gamma$ をベクトル Q 空間 $\Gamma_{(0)}$ に埋め込み、自然な全順序群構造を持ちます)。

95

[§ 5 に対して練習問題](exercises/s5/)を参照してください。
