---
book: top
book_title: General Topology
chapter: VII
chapter_title: The additive groups $\mathbf{R}^n$
section: 2
section_title: Continuous homomorphisms of $\mathbf{R}^n$ and its quotient groups
lang: ja
source: top-v-x
pdf_pages: 0085-0089, 0099-0101
extraction: ocr
subsections:
    - "no": 1
      title: CONTINUOUS HOMOMORPHISMS OF THE GROUP $\mathbf{R}^m$ INTO THE GROUP $\mathbf{R}^n$
      page: 0
      pdf_page: 85
    - "no": 2
      title: LOCAL DEFINITION OF A CONTINUOUS HOMOMORPHISM OF $\mathbf{R}^n$ INTO A TOPOLOGICAL GROUP
      page: 0
      pdf_page: 85
    - "no": 3
      title: CONTINUOUS HOMOMORPHISMS OF $\mathbf{R}^m$ INTO $\mathbf{T}^n$
      page: 0
      pdf_page: 87
    - "no": 4
      title: AUTOMORPHISMS OF $\mathbf{T}^n$
      page: 0
      pdf_page: 88
statements: 10
exercises: 7
content_sha256: 829d425b14e1a8f33b1bc4f434a199122d51d5ed2b9167cdc7b27f853ccd46ce
translated_from: content/en/top/VII/02_s2_continuous_homomorphisms_of_mathbf_r_n.md
translation_method: google
source_content_sha256: 3f006ad7fa82d9c7e014ebfbbac1ca9f11dfb28040f438d97d56329bb57b038d
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: bf042ac0e25ea3367303c5c49527ca0e90883aca319e4196943ae6b2574b40c3
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## 2. $\mathbf{R}^n$ の連続準同型とその剰余群

### 1. 群 $\mathbf{R}^m$ から群 $\mathbf{R}^n$ への継続的な準同型

$\mathbf{R}^m$ から $\mathbf{R}^n$ までのすべての線形写像 (cf. 章 VI, § i, no. 3) は、明らかに加法群 $\mathbf{R}^m$ から加法群までの連続する準同型です。 $\mathbf{R}^n$。逆に:

#### 命題 1 {#top-vii-s2-prop-1 .statement tag=0BZ3}

*すべての連続準同型* $f$ *of 加法群* $\mathbf{R}^m$ *into 加法群* $\mathbf{R}^n$ *は線形写像 of* $\mathbf{R}^m$ *into* $\mathbf{R}^n$。

すべての $x \in \mathbf{R}^n$ とすべての $t \in \mathbf{R}$ に対して $f(tx) = tf(x)$ であることを示すだけで十分です。この議論は、置き換える $x$ を $x$ で、$\mathbf{R}$ を $\mathbf{R}^m$ とすれば、章 V, § i, no. 3 の命題 5 と同じになります。

### 2. $\mathbf{R}^n$ の連続準同型のローカル定義をトポロジカル群に変換

命題章 V、§ i、no. 4 の 6 は、すべての群 $\mathbf{R}^n$ に一般化できます。

#### 命題 2 {#top-vii-s2-prop-2 .statement tag=0BZ4}

*$A$ *$\mathbf{R}^n$ *含む* $o$ の平行光学面であるとしましょう。 *そして* $f$ * $A$ の連続写像を *位相幾何学的な群* $G$ *(乗算的に書かれる)* *次のように* $f(x + y) = f(x)f(y)$ * 点* のそれぞれの対について $x, y$ *そのような* $x \in A,\ y \in A$ *そして* $x + y \in A$ *その後、* $\mathbf{R}^n$ * から* $G$ * 拡大する* $f$ への一意の連続準同型が存在します。

章 V、§ i、no. 4 の命題 6 と同じ推論により、$f$ を拡張する準同型が存在する場合、それは *一意* であることを示します。次に、$f(A)$ によって生成された $G$ の部分群 $G_1$ は *可換* です。 $x$ と $y$ が $A$ のいずれか 2 つの点である場合、$\frac{1}{2} x, \frac{1}{2} y$ と $\frac{1}{2} (x + y)$ 属するから $A$ となるため、

$$
f \left( \frac{1}{2} (x + y) \right) = f \left( \frac{1}{2} x \right) \quad (f \frac{1}{2} y) = f \left( \frac{1}{2} y \right) f \left( \frac{1}{2} x \right),
$$

これは、$f \left( \frac{1}{2} x \right)$ と $f \left( \frac{1}{2} y \right)$ が通勤していることを示しています。したがって、$f(x) = (f \left( \frac{1}{2} x \right))^2$ と $f(y) = (f \left( \frac{1}{2} y \right))^2$ も同様であり、主張が証明されます。

$a_1, a_2, \ldots, a_n$ を、$A$ に含まれ、平行六面体の基底ベクトルに比例する非ゼロベクトル $n$ とし、各インデックス $i$ について、$D_i$ を $o$ と $a_i$ を通る線、つまり、$t$ が通過する点$ta_i$ の集合とします。 $\mathbf{R}$。 $A_i$ を、$ta_i \in A$ となるようなすべての $t \in \mathbf{R}$ の集合とします。その場合、$A_i$ は $\mathbf{R}$ 含む $[0, 1]$ および写像の区間です

$$
f_i(t) = f(ta_i)
$$

$A_i$ で定義され連続しており、関係を満たす

$$
f_i(t + t') = f_i(t) f_i(t')
$$

$t, t'$ と $t + t'$ がすべて属するから $A_i$ になるたびに。 V, § 1, no. 4章の命題6により、$f_i$を拡張する$\mathbf{R}$から$G$への連続準同型$\bar{f}_i$が存在します。 Since $\mathbf{R}^n$ is the direct sum of the subgroups $D_i$, we can define a homomorphism $\bar{f}$ of $\mathbf{R}^n$ into the abelian group $G_1$ by the rule $\bar{f}(x) = \prod_{i=1}^n \bar{f}_i(t_i)$ where $x = \sum_{i=1}^n t_i a_i$; $\bar{f}$ is an extension of $f$ since, if $x \in A$, all the components $x_i$ of $x$ on the lines $D_i$ also belong to $A$, by reason of the choice of the $a_i$; moreover, $\bar{f}$ is continuous on $\mathbf{R}^n$, because it is continuous on each of the lines $D_i$, and $x_i$ is a linear function of $x$ (and therefore continuous).

#### 系 1 {#top-vii-s2-prop-2-cor-1 .statement tag=0BZ5}

*$V$ を $\mathbf{R}^n$ の $o$ の近傍とし、$f$ を $V$ の連続写像としてトポロジカル群 $G$ とする*

$$
f(x + y) = f(x) f(y)
$$

*$x \in V, y \in V$ と $x + y \in V$ のように、点 $x, y$ の各対に対して。次に、近傍の点、$o$の$W$、$f$と全く一致する$\mathbf{R}^n$から$G$へのユニークな連続準同型が存在します。

$W$ を、$V$ に含まれる中心 $o$ と命題を適用する 2 から $W$ が入った開いたボックスとします。

この $\mathbf{R}^n$ 拡大するの性質が、トポロジカル群のより大きな類、つまり「単純に接続されている」群であることが後でわかります。

#### 系 2 {#top-vii-s2-prop-2-cor-2 .statement tag=0BZ6}

*$f$ をトポロジー 群 $G$ を持つ $\mathbf{R}^n$ のローカル同型とします。 次に、$o$ の近傍のすべての点で $f$ と一致する $G$ の開いた部分群上に $\mathbf{R}^n$ の固有の厳密な射影が存在します。

$\overline{f}$ を、$\mathbf{R}^n$ から $G$ への連続した準同型とし、$f$ の近傍の$o$ の点と一致します。 $\overline{f}(\mathbf{R}^n)$ 含む、仮定、近傍、単位元、$G$ により、(章 III, § 2, no. 1、系から命題 4) は、部分群のオープンです。 $G$;さらに、$\overline{f}$ は、章 III, § 2, no. 8、命題 24 による、$\mathbf{R}^n$ から $\overline{f}(\mathbf{R}^n)$ への厳密な射です。

#### 定理 1 {#top-vii-s2-thm-1 .statement tag=0BZ7}

*局所的に $\mathbf{R}^n$ と同型である接続されたすべての群 $G$ は、群 $\mathbf{R}^p \times \mathbf{T}^{n-p}$ ($0 \leqslant p \leqslant n$) と同型です。*

適切に選択された$\mathbf{R}^n$ のローカル同型 $f$ と $G$ 拡大するから、$\mathbf{R}^n$ の厳密な射への $G$ (命題 2、系 2) のオープン部分群への、 $G$ が接続されているため、$G$ 自体。 したがって、$G$ は $\mathbf{R}^n$ の剰余群 $\mathbf{R}^n/H$ と同型です。 $H$ は *離散* です。そうでない場合は、$o$ に任意に近い $H$ の点 $x \neq o$ が存在し、逆に $f(x) = f(o)$ となるようなものになります。 仮定、その$f$は地元の同型です。 したがって、定理は、§ 1, no. 1 の定理 1 の帰結です。

### 3. $\mathbf{R}^m$ の準同型を $\mathbf{T}^n$ に継続

#### 命題 3 {#top-vii-s2-prop-3 .statement tag=0BZ8}

*$\mathbf{R}^m$ から $\mathbf{T}^n$ に続くすべての準同型は形 $x \to \varphi(u(x))$ であり、$\varphi$ は $\mathbf{R}^n$ から $\mathbf{T}^n$ ($\mathbf{R}^n/\mathbf{Z}^n$ で識別される) の標準準同型であり、$u$ は$\mathbf{R}^m$ の線形写像を $\mathbf{R}^n$ にします。*

$f$ を $\mathbf{R}^m$ から $\mathbf{T}^n$ に連続する準同型とします。 準同型性 $x \to f(x)$ と $x \to \varphi(u(x))$ が $\mathbf{R}^m$ の $o$ の*近傍* のすべての点で一致するように、$\mathbf{R}^m$ から $\mathbf{R}^n$ への線形写像 $u$ が存在することを示します。この命題は、no. 2 の系 1 から命題 2 に続きます。 ここで、$V$ を $\mathbf{R}^n$ の $o$ の近傍とし、$V$ に制限された $\varphi$ が $\mathbf{T}^n$ を持つ$\mathbf{R}^n$ のローカル同型とし、$\psi$ を で定義された $\varphi$ の逆数とします。 $\varphi(V)$。 $f$ は連続なので、$V' = \overline{f}^{-1}(\varphi(V))$ は $\mathbf{R}^m$ の $o$ の近傍です。 写像

$$
x \to \psi(f(x)),
$$

$V'$ に限定され、$V'$ から $\mathbf{R}^n$ への連続した写像であり、$\mathbf{R}^m$ の点 $x, y$ の対ごとに $\psi(f(x+y)) = \psi(f(x)) + \psi(f(y))$ が$x \in V', y \in V'$ と $x + y \in V'$ になります。したがって (no. 2、系 1 から命題 2) この写像一致するは、明確に決定された連続準同型 $u$ の $\mathbf{R}^m$ から $\mathbf{R}^n$ のすべて点になります。 $\mathbf{R}^m$のoの近傍 $W$。 命題 1 (no. 1) $u$ は、$\mathbf{R}^m$ の線形写像から $\mathbf{R}^n$ になります。したがって、すべての $x \in W$ に対して $f(x) = \varphi(u(x))$ があり、これで証明が完成します。

#### 注意 {#top-vii-s2-n3-rem-1 .statement tag=0BZ9}

同じ議論は、より一般的に、$\varphi$ が群 $G$ への$\mathbf{R}^n$ の厳密な射であり、その制限から o の適切な近傍が$G$ を伴う$\mathbf{R}^n$ の局所同型である場合、すべての連続$\mathbf{R}^n$ の $G$ への準同型は形 $x \mapsto \varphi(u(x))$ であり、$u$ は $\mathbf{R}^m$ の線形写像から $\mathbf{R}^n$ です。

$m = n = 1$, 命題 3 の場合、次のようになります。

#### 命題 4 {#top-vii-s2-prop-4 .statement tag=0BZA}

*$\varphi$ が $\mathbf{T}$ への $\mathbf{R}$ の標準準同型である場合、$\mathbf{R}$ から $\mathbf{T}$ への連続するすべての準同型は $a \in \mathbf{R}$ の形 $x \mapsto \varphi(ax)$ になります。そして、$a \neq 0$の場合、$\mathbf{R}$の厳密な射は$\mathbf{T}$になります。*

### 4. $\mathbf{T}^n$中自己同型

$H$を$\mathbf{R}^n$の閉じた部分群とし、$\varphi$を$\mathbf{R}^n$の剰余群$\mathbf{R}^n/H$に対する標準準同型とします。 $f$ がトポロジカル群 $G$ への $\mathbf{R}^n/H$ の連続準同型である場合、$f = f \circ \varphi$ は、$\mathbf{R}^n$ から $G$ への連続準同型であり、周期的で群の周期があります。 含む $H$;逆に、$\mathbf{R}^n$ $G$ へのすべての周期連続準同型は、含む $H$ の群が​​この形に属します。

$H = \mathbf{Z}^n$、剰余群 $\mathbf{R}^n/\mathbf{Z}^n = \mathbf{T}^n$ が *コンパクト* であるため、トポロジカル群 $G$ への $\mathbf{T}^n$ のすべての連続準同型 $f$ は、$\mathbf{T}^n$ の *厳密な射* になります。 $G$、$G$ がハウスドルフ (章 III, § 2, no. 8, 注意 1) である場合。 $f = f \circ \varphi$ は、$\mathbf{R}^n$ を $G$ に厳密に変換した射です。さらに、$f(\mathbf{T}^n) = f(\mathbf{R}^n)$ は $G$ の*圧縮* 部分群であり、群 $\mathbf{T}^p$ ($0 \leq p \leq n$) と同型です。

特に、$\{ o \}$ は $\mathbf{R}^m$ の唯一のコンパクトな部分群であるため、$\mathbf{T}^n$ から群 $\mathbf{R}^m$ に連続する唯一の準同型は *零* 写像であることがわかります。

これを、グループ $\mathbf{T}^p$ への $\mathbf{T}^n$ の連続準同型写像に適用してみましょう。 $f$ がそのような準同型である場合、$\varphi$ は $\mathbf{R}^n$ から $\mathbf{T}^n$ への正準準同型であり、$f \circ \varphi$ は $\mathbf{R}^n$ から $\mathbf{T}^p$ への連続準同型です。したがって (no. 3、命題 3) $\psi$ が $\mathbf{T}^p$ への $\mathbf{R}^p$ の正準準同型性を表す場合、$f \circ \varphi = \psi \circ u$ のような $\mathbf{R}^n$ から $\mathbf{R}^p$ への線形写像 $u$ が存在します。 $x \in \mathbf{Z}^n$ の場合、$f(\varphi(x))$ は $\mathbf{T}^p$ の単位元であるため、$u(x) \in \mathbf{Z}^p$、つまり $u(\mathbf{Z}^n) \subset \mathbf{Z}^p$ が必要になります。 逆に、$u$ が、この条件を満たす、$\mathbf{R}^n$ から $\mathbf{R}^p$ までのいずれかの線形写像である場合、$\psi \circ u$ は、$\mathbf{R}^n$ から $\mathbf{T}^p$ までの周期連続準同型であり、その群は周期です。 含む $\mathbf{Z}^n$、したがって定義するは $\mathbf{T}^n$ から $\mathbf{T}^p$ に続く準同型です。

条件 $f$ が $\mathbf{T}^p$ の部分群に対する $\mathbf{T}^n$ の *同型* であることを考えてください。 まず第一に、$u$ は $\mathbf{R}^n$ から $\mathbf{R}^p$ への*単射* 写像でなければなりません。そうでない場合、ベクトル部分空間 $\overline{u}(0)$ は任意に原点に近い含む点 $x \neq 0$ になり、そのような点で私たちは持つべきだ
$$
f(\varphi(x)) = f(\varphi(0)) \quad \text{and} \quad \varphi(x) \neq \varphi(0),
$$
仮定とは反対です。 この条件は $p \geq n$ を意味します。 像 $u(\mathbf{Z}^n)$ は、階数 $n$ の群 $\mathbf{Z}^p$ の離散部分群になります。 $\mathbf{Z}^p$ (§ 1, no. 1) に関する $u(\mathbf{Z}^n)$ の *不変式因子* はすべて 1 に等しくなければなりません。そうでない場合は、$u(k^{-1}x) \in \mathbf{Z}^n$ と $k^{-1} \notin \mathbf{Z}^n$ となるような点 $x \in \mathbf{Z}^n$ と整数 $k > 1$ が存在します。 仮定とは逆に、$f(\varphi(k^{-1}x)) = f(\varphi(0))$ と $\varphi(k^{-1}x) \neq \varphi(0)$ です。 逆に、この条件が満たされれば$u(\mathbf{R}^n) \cap \mathbf{Z}^n = u(\mathbf{Z}^n)$、$f$は$\mathbf{T}^n$の同型が$u(\mathbf{R}^n)/u(\mathbf{Z}^n)$になります。

この引数を $p = n$ のケースに適用すると、次の命題が得られます。

#### 命題 5 {#top-vii-s2-prop-5 .statement tag=0BZB}

*その部分群の 1 つにあるトポロジカル群 $\mathbf{T}^n$ のすべての同型は、$\mathbf{T}^n$ の自己同型であり、線形写像 $u$ の $\mathbf{R}^n$ から移行から商によって取得されます。 $\mathbf{Z}^n$ は、$\mathbf{Z}^n$ の自己同型です。*

同様に (§ 1, no. 1)、$u(e_i) = \sum_{j=1}^n a_{ij} e_j$ の場合、$a_{ij}$ は $\det(a_{ij}) = \pm 1$ となるように整数でなければなりません。特に $n = 1$ の場合:

#### 命題 6 {#top-vii-s2-prop-6 .statement tag=0BZC}

*その部分群の 1 つにあるトポロジカル群 $\mathbf{T}$ の同型のみが恒等写像であり、対称性 $x \to -x$ です。*

### 練習問題 {#top-vii-s2-exercises}

[§ 2 に対して練習問題](exercises/s2/)を参照してください。
