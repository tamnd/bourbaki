---
book: int
book_title: Integration
chapter: VI
chapter_title: VECTORIAL INTEGRATION
section: 0
section_title: Complements on topological vector spaces
appendix: true
lang: ja
source: int-i-vi
pdf_pages: 0443-0447
extraction: ocr
subsections:
    - "no": 1
      title: Bilinear forms and linear mappings
      page: 0
      pdf_page: 443
    - "no": 2
      title: Some types of spaces having the property (GDF)
      page: 54
      pdf_page: 445
statements: 6
exercises: 0
content_sha256: 61fc41984a59e86b59467a80342770285b7951eb1282834d40f6adbeb914cf60
translated_from: content/en/int/VI/A_a_complements_on_topological_vector_spaces.md
translation_method: google
source_content_sha256: 02f42b389f24a36ddcc58d04da30cbfa4dd5961e3192d18701403d3e92f17929
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: 66452df2d36f16938501100bae425b4eaba1401bc59a2be9b8901afef508cb48
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## 付録

# トポロジカルベクトル空間の補数

### 1. 双線形形式と線形写像

$(F_1, G_1), (F_2, G_2)$ を、分離双対性 (TVS、II, §6, No. 1) における (実数または複素数) ベクトル空間の 2 つの対とします。これら空間のそれぞれに対応するの弱い位相 (*上記引用*、No. 2) が装備されていると仮定します。 A と B がこれら空間のいずれか 2 つである場合、通常どおり、A から B に連続する線形写像の $\mathscr{L}(A; B)$ ベクトル空間によって、および $A \times B$ 上で *別々に連続する* 双線形形式の $\mathfrak{B}(A, B)$ ベクトル空間によって表されます。

$F_1 \times F_2$ で個別に連続する双線形形式 $\Phi$ に対して、$x_1 \mapsto \Phi(x_1, x_2)$ は $F_1$ で連続する線型形式であるため、次のような元 ${}^r\Phi(x_2) \in G_1$ が 1 つだけ存在します。

$$
\Phi(x_1, x_2) = \langle x_1, {}^r\Phi(x_2) \rangle
$$

$x_1 \in F_1, x_2 \in F_2$ (TVS、III, §5, No. 1、(1)) の場合。 さらに、この公式は、$F_2$ と $G_1$ の (弱い) トポロジーに対して写像 $x_2 \mapsto {}^r\Phi(x_2)$ が線形で連続であることを示しています。 逆に、$F_2$ から $G_1$ に連続する線形写像 $u$ ごとに、$(x_1, x_2) \mapsto \Phi(x_1, x_2) = \langle x_1, u(x_2) \rangle$ は、$F_1 \times F_2$ と ${}^r\Phi = u$ で個別に連続する双線形形式になります。 したがって、$\mathfrak{B}(F_1, F_2)$ の定義する同型 $r : \Phi \mapsto {}^r\Phi$ が $\mathscr{L}(F_2; G_1)$ に重なり、*正規* と言われます。

同様に、公式

$$
\Phi(x_1, x_2) = \langle {}^l\Phi(x_1), x_2 \rangle
$$

$\mathfrak{B}(F_1, F_2)$ の $\mathscr{L}(F_1; G_2)$ への *正準同型* $l : \Phi \mapsto {}^l\Phi$ を定義します。そして明らかに可換図を持っています

$$
\begin{array}{ccc}
\mathscr{B}(F_1, F_2) & & \\
l & l^{-1} & r^{-1} \\
& & \\
\mathscr{L}(F_1; G_2) & \xleftarrow{t} & \mathscr{L}(F_2; G_1)
\end{array}
$$

ここで、$t$ は転置 $u \mapsto {}^t u$ の同型です。 $G_1$ と $G_2$ の弱いトポロジーの定義を考慮すると、明らか $\mathscr{B}(F_1, F_2)$、$\mathscr{L}(F_1; G_2)$、$\mathscr{L}(F_2; G_1)$ に点単位収束の位相が装備されている場合、その前の図式の同型は、トポロジー ベクトル空間構造の場合、同型。

ここで、$E, F$ を 2 つの局所的に凸なハウスドルフ空間、$E', F'$ のそれぞれの双対とします。弱化トポロジー $\sigma(E, E')$、$\sigma(F, F')$ を備えた $E_\sigma, F_\sigma$ 空間 $E, F$ と、弱いトポロジー $\sigma(E', E)$、$\sigma(F', F)$ を備えた $E'_s, F'_s$ 空間 $E', F'$ で表します。 したがって、前の注意は 3 つの空間 $\mathscr{B}(E_\sigma, F'_s)$、$\mathscr{L}(E_\sigma; F_\sigma)$、$\mathscr{L}(F'_s; E'_s)$ の間に標準同型を確立し、また 3 つの空間 $\mathscr{B}(E_\sigma, F_\sigma)$、$\mathscr{L}(E_\sigma; F'_s)$ および $\mathscr{L}(F_\sigma; E'_s)$ の間にも標準同型を確立します。 $E$ (それぞれ $F$) 上のすべての連続線型形式は連続しているため、$\mathscr{B}(E_\sigma, F_\sigma)$ は $E \times F$ ($E$ と $F$ は元のトポロジーを備えている) で個別に連続する双線形形式の空間 $\mathscr{B}(E, F)$ にも等しいことがわかります。 $E_\sigma$ (それぞれ $F_\sigma$) およびその逆 (TVS、II, §6, No. 1 および No. 2、提案 3)。

$\mathscr{B}(E, F)$ を $E \times F$ 上の連続双線形形式の空間とします ($E$ と $F$ には元のトポロジーが装備されています)。次に$\mathscr{B}(E, F) \subset \mathscr{B}(E, F)$。

#### 命題 1 {#int-vi-a0-prop-1 .statement tag=09CS}

*双線形形式 $\Phi \in \mathscr{B}(E, F)$ ～ 属する ～ $\mathscr{B}(E, F)$ については、${}^l \Phi$ の下の像が $F'$ の等連続部分集合である $E$ に 0 の近傍が存在することが必要かつ十分です。

なぜなら、$\Phi$ が連続であるということは、$x \in V$、$y \in W$ に対して $|\Phi(x, y)| \leq 1$ となるような、$E$ (それぞれ $F$) に 0 のバランスの取れた凸近傍 $V$ (それぞれ $W$) が存在することを意味するからです。これは、$x \in V$、$y \in W$、または ${}^l \Phi(V) \subset W^\circ$ の場合、$|\langle {}^l \Phi(x), y \rangle| \leq 1$ と書かれる場合があります。 よって命題は、$F'$ のすべての等連続部分集合が $F$ の 0 の近傍の極に含まれているという事実を考慮しています。

#### 系 {#int-vi-a0-n1-cor-1 .statement tag=09CT}

*$\Phi$が$E \times F$の連続双線形形式である場合、${}^l \Phi$は$E$の連続線形写像で、$F$の強力なデュアル$F'_b$になります。さらに、$E$ と $F$ が空間と正規化されている場合、$\|{}^l \Phi\| = \|\Phi\|$ となります。*

最初の主張は、提案 1 と、$F'_b$ の 0 のすべての近傍が $F'$ のすべての等連続部分集合を吸収するという事実から導かれます。 $E$ と $F$ が標準である場合、

$$
\|\Phi\| = \sup_{\|x\| \leq 1, \|y\| \leq 1} |\Phi(x, y)| = \sup_{\|x\| \leq 1} \left( \sup_{\|y\| \leq 1} |\langle l \Phi(x), y \rangle| \right)
= \sup_{\|x\| \leq 1} \|l \Phi(x)\| = \|l \Phi\|,
$$

よって 2番目の主張。

交換すること E と F の役割により、提案 1 とその系線形写像 $r \Phi$ に類似した結果が得られます。それらを述べる作業は読者に任せます。

### 2. 空間の一部の型に性質が含まれています (GDF)

すべてのフレシェ空間に性質 (GDF) (TVS、I, §3, No. 3、Th. 1 の Cor. 5) があることはすでにわかっています。

#### 命題 2 {#int-vi-a0-prop-2 .statement tag=09CU}

— E をベクトル空間、$(F_\alpha)_{\alpha \in A}$ を性質 (GDF) を持つ局所的にコンパクトな空間のファミリーとし、それぞれの $\alpha \in A$ に対して、$h_\alpha$ を E の $F_\alpha$ の線形写像とします。E に最も細かい局所凸型が装備されている場合位相は $h_\alpha$ を連続にし、E は性質 (GDF) になります。

$u$ を E の線形写像をバナッハ空間 B にすると、$u$ のグラフ $\Gamma$ のすべての収束数列の点の$E \times B$ のすべての極限も属するになります。 $\Gamma$。すべての $\alpha \in A$ に対して、$u \circ h_\alpha$ が $F_\alpha$ で連続していることを示すだけで十分です (TVS、II, §4, No. 4、提案 5)。さて、$(x_n)$ を極限 $a$ を持つ $F_\alpha$ の元の数列とし、数列 $\left(u(h_\alpha(x_n))\right)$ は極限 $b \in B$ を持つようにします。 $h_\alpha$ は連続なので、$h_\alpha(a)$ は E の数列 $(h_\alpha(x_n))$ の極限です。したがって、仮定 $b = u(h_\alpha(a))$ により、$F_\alpha$ には性質 (GDF) があるため、$u \circ h_\alpha$ は連続です。

#### 系 {#int-vi-a0-n2-cor-1 .statement tag=09CV}

— 性質 (GDF) を持つ局所凸空間のすべての商空間は性質 (GDF) を持ちます。

#### 命題 3 {#int-vi-a0-prop-3 .statement tag=09CW}

— 再帰的なフレシェ空間の強力な二重には性質 (GDF) があります。

これは提案 2 の帰結と次の補題 (または TVS、IV, §3, No. 4、提案 4) です。

#### 補題 {#int-vi-a0-n2-lem-1 .statement tag=09CX}

F をフレシェ空間、$F'$ の強力な双対、$F''$ の双対とする。 $\sigma(F'', F')$ に限定された$F''$ のすべての部分集合が F の有界部分集合の閉包 ($\sigma(F'', F')$ の) に含まれる場合、$F'$ はバナッハ空間の数列の直接の極限になります。

$(V_n)$ を、F の 0 の凸でバランスが取れた閉じた近傍の減少する基本関数数列とします。すべての整数 $n$ に対して、$G_n$ を極座標によって生成された $F'$ の線形部分空間とします。 $V_n$中$V_n^\circ$。 $G_n$では、$V_n^\circ$は吸収凸面集合であるため、そのゲージ$p_n$は$G_n$ではノルムです。さらに、$V_n^\circ$ は、強力な二重$F'$ の完全な部分集合です (TVS、III, §3, No. 8、提案 11)。したがって、ノルム $p_n$ を装備した $G_n$ は、Banach 空間 (GT、III, §3, No. 5、Prop. 9 の Cor. 2) です。 $F'$ 上の強い位相が、$G_n$ 上のこれらの Banach 空間トポロジーの直接極限であること、または、$F'$ の強く閉じられ、平衡した、凸状の部分集合 U が 0 の強い近傍であるためには、次のことが必要であることを示します。 $V_n^\circ$ のそれぞれを吸収するのに十分です。この条件が必要であることは明らかです。それが十分であることを確認するには、U 含むが $F'$ のバレルであることを証明すれば十分です。実際、$F''$ の極$U^\circ$ は$\sigma(F'', F')$ に限定されるため、仮定によって、F の有界部分集合 B の閉包 ($\sigma(F'', F')$ の) に含まれ、そこから U (閉包されている) を結論する求めることができます。 $\sigma(F', F'')$) 含む 0 の強力な近隣 $B^\circ$ (TVS、II, §6, No. 3、Th. 1 および §8, No. 4)。

仮定までに、整数 $n$ ごとに $\lambda_n V_n^\circ \subset \frac{1}{2}U$ となる数 $\lambda_n > 0$ が存在します。 $A_n$を、$i \leq n$に対する$\lambda_i V_i^\circ$の和集合の凸包絡線とします。次に、$n$ ごとに $A_n \subset \frac{1}{2}U$ が発生します。 W を $A_n$ の和集合とします。 W は、$\frac{1}{2}U$ に含まれる凸型でバランスの取れた吸収性の集合であり、その強力な閉鎖 (バレルである) が U に含まれていることを示すだけで十分です。

従って、$x'$ を U に対する所属ではなく、$F'$ の点とします。各 $V_n^\circ$ は $\sigma(F', F)$ に対してコンパクトであるため、同じことが $A_n$ (TVS、II, §2, No. 6、提案 15) にも当てはまり、$x' \notin 2A_n$ 以降、 元 $x_n$ 所属を F の $A_n$ の極点にすると、$\langle x', x_n \rangle = 2$ になります (TVS、II, §5, No. 3、提案 4)。 数列 $(x_n)$ は F で制限されています。つまり、すべての $y' \in F'$ 属するからいくつかの $V_k^\circ$ まで、その結果、$n \geq k$、よっての主張については $|\langle y', x_n \rangle| \leq \lambda_k^{-1}$ になります (TVS、IV, §1, No. 1、Prop. 1)。 C を、F 含むのすべての $x_n$ における有界でバランスの取れた凸面集合とします。この場合、$C^\circ$ は $F'$ の 0 の近傍であり、$F''$ の $C^\circ$ の極点 $C^{\circ\circ}$ は $\sigma(F'', F')$ に対してコンパクトです (TVS、III, §3, No. 4、提案 4 の Cor. 2 および No. 5、提案 7)。従って、数列 $(x_n)$ には、$\sigma(F'', F')$ の $F''$ にクラスター 点 $x''$ があることがわかります。明らかに$\langle x', x'' \rangle = 2$、そしてその一方で、$n$ごとに$F''$の$A_n$の極点に$x''$属する、従って$F''$のWの極点$W^\circ$になります。このことから、$x' \notin W^{\circ\circ}$ である 1 つの結論するは、$\sigma(F', F'')$ (TVS、II, §6, No. 3、Th. 1 および §8, No. 4) の W の閉包に含まれていないため、強い位相に対して *なおさら* となり、証明が完成します。

練習問題
