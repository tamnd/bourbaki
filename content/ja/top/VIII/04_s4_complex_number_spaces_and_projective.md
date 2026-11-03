---
book: top
book_title: General Topology
chapter: VIII
chapter_title: Complex numbers
section: 4
section_title: Complex number spaces and projective spaces
lang: ja
source: top-v-x
pdf_pages: 0124-0128, 0133-0136
extraction: ocr
subsections:
    - "no": 1
      title: THE VECTOR SPACE $\mathbf{C}^n$
      page: 0
      pdf_page: 124
    - "no": 2
      title: TOPOLOGY OF VECTOR SPACES AND ALGEBRAS OVER THE FIELD $\mathbf{C}$
      page: 0
      pdf_page: 125
    - "no": 3
      title: COMPLEX PROJECTIVE SPACES
      page: 0
      pdf_page: 125
    - "no": 4
      title: SPACES OF COMPLEX PROJECTIVE LINEAR VARIETIES
      page: 0
      pdf_page: 127
statements: 3
exercises: 8
content_sha256: b48139107cdfe480f0fd45eb00c6def7671e092a23f355ba74024e3844bbda6c
translated_from: content/en/top/VIII/04_s4_complex_number_spaces_and_projective.md
translation_method: google
source_content_sha256: a0635aa3afab1817d675f46cf3f74b8d72a27d4aefcae7dd03e7963e1016fe2d
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: 9f663b0f90d855c105b27335fc1c42111446e174ac7a88650a9f5ab4bec37c74
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## 4. 複素数空間と射影空間

### 1. ザベクトル空間 $\mathbf{C}^n$

位相空間 $\mathbf{C}$ は $\mathbf{R}^2$ と同一視できるので、$\mathbf{C}$ と同一の $n$ 空間の位相積 $\mathbf{C}^n$ は位相空間 $\mathbf{R}^{2n}$ と同一視できる。同様に、$n$ 因子の加法的 (位相的) 群構造の積である $\mathbf{C}^n$ の位相的群構造は、加法的群 $\mathbf{R}^{2n}$ の位相群構造と識別できます。 しかし、$\mathbf{C}$ は体なので、複素数 $a$ の $\mathbf{C}$、積 $az$ 上の $n$ 次元のベクトル空間の $\mathbf{C}^n$ 構造に定義するが乗ってもよいでしょう。 $\mathbf{C}^n$ の点 $z = (z_i)$ は点 $(az_i)$ です。このベクトル空間構造は、$\mathbf{R}^{2n}$ (章 VI, § 1, no. 3) に定義された $\mathbf{R}$ 上の $2n$ 次元ベクトル空間の構造とは慎重に区別される必要があります。 記法 $\mathbf{C}^n$ は、$\mathbf{C}$ と同一の $n$ 空間の積であるトポロジカル空間に予約します。加法には、先ほど定義した $\mathbf{C}$ にベクトル空間構造が付与されています。 $\mathbf{C}^n$ は、$n$ 次元の複素数空間と呼ばれます。 写像 $(t, z) \to tz$ は $\mathbf{C} \times \mathbf{C}^n$ で連続していることに注意してください。

$\mathbf{C}^n$ の $\mathbf{C}^m$ へのアフィン線形写像は、$\mathbf{R}^{2n}$ の $\mathbf{R}^{2m}$ へのアフィン線形写像でもありますが、逆は偽です。

たとえば、写像 $z \to \overline{z}$ は、それ自体に対するベクトル空間 $\mathbf{R}^2$ の線形写像ですが、それ自体に対するベクトル空間 $\mathbf{C}$ の線形写像ではありません。

したがって、$\mathbf{C}^n$ から $\mathbf{C}^m$ へのすべてのアフィン線形写像は一様に連続です。特に、それ自体に対する $\mathbf{C}^n$ のすべてのアフィン線形写像は同相写像です。

ベクトル空間 $\mathbf{C}^n$ の $p$ 次元 ($p \leq n$) のすべてのアフィン線形多様体は、 ベクトル空間 $\mathbf{R}^{2n}$ の $2p$ 次元のアフィン線形多様体でもあります。ここでも、逆は false です。混乱を避けるために、$\mathbf{C}^n$ の $p$ 次元の (アフィン) 線形多様体は、 $p$ 次元の複素線形多様体と呼ばれます (誤解を防ぐために、必要に応じて $\mathbf{R}^{2n}$ の線形多様体は真線形多様体と呼ばれます)。特に、1 つの次元 (それぞれ 2 つの次元) の複素線形多様体は複素線 (それぞれ複素平面) と呼ばれ、$n - 1$ 次元の複素線形多様体は複素数超平面と呼ばれます。

多くの場合、関係 $J(z_k) = 0$ によって定義される $\mathbf{C}^n$ の部分集合で $\mathbf{R}^n$ を識別することにより、実数空間 $\mathbf{R}^n$ が複素数空間 $\mathbf{C}^n$ に埋め込まれていると考えると便利です。 ($1 \leq k \leq n$)。 $\mathbf{C}^n$ 一致するのトポロジカル群構造と $\mathbf{R}^n$ のトポロジカル群構造によって、この部分集合上にトポロジカル群構造が誘発されます。

このように $\mathbf{C}^n$ に埋め込まれた $\mathbf{R}^n$ は、$\mathbf{C}^n$ では複素線形多様体ではないことに注意してください。

$p$ の系 $\mathbf{R}^n$ のベクトルは、$\mathbf{R}$ では無料ですが、$\mathbf{C}$ では無料です。 $\mathbf{R}^n$ 生成するの $p$ 次元のすべての実線形多様体 $V$ $\mathbf{C}^n$ の $p$ 次元の複素線形多様体 $V'$ で、$V$ は $V'$ のトレースになります$\mathbf{R}^n$; $V$ が $n - p$ 線形方程式 $f_k(x) = a_k$ の系で定義されている場合、$f_k$ は $\mathbf{R}^n$ 上の線型形式 (実数は係数で、$\mathbf{R}$ にわたって線形独立)、$a_k$ は次のようになります。 実数の場合、同じ方程式定義する $V'$ になりますが、$x$ の座標は複素数値になります。

逆に、$p$ 次元の複素線形多様体に $\mathbf{R}^n$ を持つ空ではない共通部分がある場合、この共通部分は真の線形多様体ですが、その次元は $< p$ になる可能性があります。

### 2. 体 $\mathbf{C}$ を超えるベクトル空間と代数の位相

すべての定義とすべての No. の結果。 体 $\mathbf{R}$ 上のベクトル空間と代数のトポロジに関連する章 VI, § 1 の 5 と 6、特に $\mathbf{R}$ の元を含む行列の空間と代数は引き続き有効です。 置き換える $\mathbf{R}$ by $\mathbf{C}$ までは変更なしで。

### 3. 複素射影空間

章 VI, § 3, no. 1 で記法を呼び出すと、実射影空間の定義に類似して、次の定義を作成します。

#### 定義 1 {#top-viii-s4-def-1 .statement tag=0C0W}

*射影空間* $\mathbf{P}_n(\mathbf{C})$, ** $\mathbf{C}_{n+1}^*$ の商である位相に * 同値関係* $\Delta_n(\mathbf{C})$ を加えたもので、 * $n$ *次元の複素射影空間と呼ばれます。

射影空間 $\mathbf{P}_1(\mathbf{C})$ は *複素射影線 * と呼ばれ、 $\mathbf{P}_2(\mathbf{C})$ は *複素射影平面 * と呼ばれます。

引数のほとんどは実数射影空間拡大するに関連しており、複素射影空間にわずかな修正が加えられています。

まず第一に、章 VI, § 3 の命題 1 の引数により、位相位相空間 $P_n(\mathbf{C})$ が *Hausdorff* であることがわかります。 no. 1、これは置き換えること $\mathbf{R}$ $\mathbf{C}$ だけで語に語が適用されます。繰り返しますが、命題の証明、章の2、VI, § 3です。 no. 1 は、$P_n(\mathbf{C})$ が *コンパクトで接続* しており、$\Delta_n(\mathbf{C})$ によってこの球上に誘導された同値関係によって球 $S_{2n-1}$ ($R_{2n-2}^*$ と同一視される空間 $C_{n-1}^*$ に埋め込まれていると考えられる) の商と同型であることを示しています。唯一の違いは、点が、$n \geqslant 0$ の場合、この関係の同値類が円 $S_1$ と同型であることです。

このため、章 VI の命題 3 です。 § 3, no. 1 には、複素射影法空間に相当するものはありません。

次は、章 VI, § 3, no. 2 のように、空間 $P_n(\mathbf{C})$ のすべての $p$ 次元射影線形多様体が閉集合で、$P_r \mathbf{C}$ と同型であり、その補数が $p < n$ であれば $P_n(\mathbf{C})$ で密であることを示しています。 証明 of 命題 5 of 章 VI, § 3, no. 2 は、単に $\mathbf{R}$ を $\mathbf{C}$ に置き換えるだけでそのまま転置でき、($n \geqslant 0$ の場合) $P_n(\mathbf{C})$ の射影超平面の補数が以下と同相であることを示します。 $\mathbf{C}^*$、したがって、すべての点は $\mathbf{C}^*$ と同型の近傍を持ちます。この結果により、「無限大における超平面」（通常は超平面）と呼ばれる射影超平面の補数で$\mathbf{C}^*$を特定することにより、複素射影空間$P_n(\mathbf{C})$に複素数空間$\mathbf{C}^n$を*埋め込むことができます。方程式は$x_0 = 0$)。特定のケース $n = 1$ では、無限遠の超平面は *点* であり、Alexandroff の定理は、$P_1 \mathbf{C}$ が局所的にコンパクトな空間 $\mathbf{C}$ をコンパクト化することで得られる空間 $\tilde{\mathbf{C}}$ と同相であることを示しています。 $\infty$ で示される「無限遠の点」に隣接しています。 命題章 VI の 4。 § 2, no. 4 は、*複素射影線* $P_1(\mathbf{C})$ *球* $S_2$ と同相であることを示します。

章 VI と同様の結果を説明する作業は読者に委ねられます。 § 3。 no. 4、写像の場合、$\mathbf{C}$で値がかかります。

空間 $\mathbf{R}^{n+1}$ を $\mathbf{C}^{n+1}$ (no. 1) に *埋め込まれている* と考えてください。 $f$ を $C_{n-1}^*$ の標準写像として、商空間 $P_n(\mathbf{C})$ に加えます。 部分空間 $f(\mathbf{R}_{n-1}^*)$ は、*実* 同次座標の系を少なくとも 1 つ持つ $P_n(\mathbf{C})$ の点で構成されます。 $f(\mathbf{R}_{n-1}^*)$ が実数射影空間 $P_n(\mathbf{R})$ と同相であることを示してみましょう。これにより、空間 $P_n(\mathbf{R})$ を $P_n(\mathbf{C})$ に *埋め込まれた* とみなすことができます。現在、$\mathbf{R}_{n+1}^*$ の $\Delta_n(\mathbf{C})$ によって誘導された関係は $\Delta_n(\mathbf{R})$ です。 標準写像 $\varphi$ 件中

$$
\mathbf{R}_{n+1}^*/\Delta_n(\mathbf{R}) = P_n(\mathbf{R})
$$

$f(\mathbf{R}_{n-1}^*)$ は *連続* (章 I, § 3, no. 6, 命題 10);それ以来

$P_n(\mathbf{R})$ はコンパクトですが、$\varphi$ は同相写像 (章 I, § 9, no. 4, 定理 2, 系 2) でなければなりません。

また、章 I, § 3, no. 6 の命題 10 の基準を援用することで、$P_n(\mathbf{R})$ のコンパクト性を使用せずに、$\varphi$ が共連続であることを証明することもできます (練習問題 3 を参照)。

$\mathbf{R}^{n+1}$ の $p + 1$ 次元のすべてのベクトル部分空間は、 $\mathbf{C}^{n+1}$ の $p + 1$ 次元の複素ベクトル部分空間を生成するため、 $P_n(\mathbf{R})$ の $p$ 次元のすべての射影線形多様体 $V$ ($V$ は *実数* 射影線形多様体と呼ばれます) が射影線形多様体を生成することがわかります。 $P_n(\mathbf{C})$ の $p$ 次元の $V'$ ($V'$ は *複素* 射影線形多様体と呼ばれます)、$V$ は $P_n(\mathbf{R})$ 上の $V'$ のトレースになります。 さらに、変数に複素数値を取ることを許可すると、$V$ の (均質) 方程式のすべての系は、$V'$ の (均質) 方程式の系にもなります。

### 4. 複素射影線形多様体の空間

章 VI, § 3, no. 5 で思い出した記法を使用して、複素射影空間の射影線形多様体の定義するを同様に空間ます。

#### 定義 2 {#top-viii-s4-def-2 .statement tag=0C0X}

*商空間* $P_{n,p}(\mathbf{C})$ *トポロジー 空間* $L_{n+1,\ p+1}(\mathbf{C})$ *同値関係* $\Delta_{n,p}(\mathbf{C})$ *は射影空間* の射影線形多様体の空間と呼ばれます* $p \geqslant 0$ *次元 $P_n(\mathbf{C})$。

章 VI, § 3, no. 5 の命題 6 の議論により、まず、$P_{n,p}(\mathbf{C})$ が *Hausdorff* であることがわかります。次に、置き換えること部分空間 $V_{n+1,\ p+1}$ (命題 7 of 章 VI, § 3, no. 5 の証明) 部分空間 $W_{n+1,\ p+1}$ of $L_{n+1,\ p+1}(\mathbf{C})$ からなるによって *コンパクト* であることを証明します。 $p + 1$ ベクトルの系と形は *正規直交エルミート基底* ベクトル部分空間は生成するです。つまり、$W_{n+1,\ p+1}$ は行列 $X = (x_{ij})$ と満たす条件で構成されます。

$$
\sum_{j=0}^n x_{ij} \overline{x}_{ij} = 1 \quad (1 \leq i \leq p + 1),
$$
$$
\sum_{j=0}^n x_{ij} \overline{x}_{kj} = 0 \quad (i \neq k).
$$

証明 of 命題 8 of 章 VI, § 3, no. 5 拡大するは空間 $P_{n,p}(\mathbf{C})$ に対して変更されておらず、この空間が *接続* かつ *ローカル接続* されていて、それぞれの点に近傍があることが示されています。 $\mathbf{C}^{p+1,(n-p)}$ と同型。最後に、章 VI, § 3, no. 6 の 9 の命題の証明は、変更なしで適用されるため、グラスマン関数 $G_{n,p}(\mathbf{C})$ は $\mathbf{P}_{n,p}(\mathbf{C})$ と同相です。

#### 注意 {#top-viii-s4-n4-rem-1 .statement tag=0C0Y}

実数に対するプロパティ共通のおよび複素数空間 (射影空間) のほとんどは、クォータニオン $\mathbf{H}$ の除算環に対して同様に定義された数空間 (射影空間) でも有効です。実際、それらは、他の多くのトポロジー 体や除算環 (cf. 練習問題 2 と 6) への拡大を可能にします。

### 練習問題 {#top-viii-s4-exercises}

[§ 4 に対して練習問題](exercises/s4/)を参照してください。
