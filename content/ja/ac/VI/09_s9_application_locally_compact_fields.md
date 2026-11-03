---
book: ac
book_title: Commutative Algebra
chapter: VI
chapter_title: VALUATIONS
section: 9
section_title: 'Application: locally compact fields'
lang: ja
source: ac-i-vii
book_pages: 431-434, 470-471
pdf_pages: 0449-0452, 0488-0489
extraction: ocr
subsections:
    - "no": 1
      title: THE MODULUS FUNCTION ON A LOCALLY COMPACT FIELD
      page: 431
      pdf_page: 449
    - "no": 2
      title: EXISTENCE OF REPRESENTATIVES
      page: 432
      pdf_page: 450
    - "no": 3
      title: STRUCTURE OF LOCALLY COMPACT FIELDS
      page: 433
      pdf_page: 451
statements: 10
exercises: 5
content_sha256: c49b89f4f6c22bbbcaae82af2864b21902f00e6e8a1ae853e40c814d0ac2b518
translated_from: content/en/ac/VI/09_s9_application_locally_compact_fields.md
translation_method: google
source_content_sha256: cbf8d7f6c26e3c562858fae29ec698adc8ce0ba172721d0d36754a85dbdf6f59
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: c6151c3d1248aaed22757a68149a6061d5d509c7710baa254a5bcab83fe17ebe
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## 9. アプリケーション: ローカルコンパクト体

### 1. 局所コンパクト体の係数写像

$K$ を局所的にコンパクトな体とします (必ずしも可換であるとは限りません)。 写像 mod (または mod) が $K$ で次のように定義されている (Integration, 章 VII, § 1, no. 10, 定義 6) ことを思い出してください: $\operatorname{mod}_K(0) = 0$ および $K$ の $x \neq 0$ については、数 $\operatorname{mod}_K(x)$ が$K$ の自己同型 $y \mapsto xy$ の加法群の係数。

#### 命題 1 {#ac-vi-s9-prop-1 .statement tag=04XQ}

*$K$ がローカルのコンパクトフィールドの場合、関数 mod、属するから $\mathscr{V}(K)$ (§ 6, no. 1)。さらに:*
(i) *$s > 0$ が $(\operatorname{mod}_K)^s = g$ が絶対値値であるような場合、$K$ では $g$ 定義する位相となります。
(ii) *$K$ が離散的でなく、mod が超計量絶対値値である場合、$K$ に正規化された離散評価 $v$ が存在します。その環はコンパクトで、剰余場は $q$ 元で有限です。 $\operatorname{mod}, = q^{-v}$。 $K$ の位相は $v$ によって定義されます。*

これは、§ 6, no. 1、命題 1、§ 5, no. 1、命題 2、および統合、章 VII, § 1, no. 10、命題 12、13 に続きます。

#### 命題 2 {#ac-vi-s9-prop-2 .statement tag=04XR}

*$K, K'$ を、$K$ が $K'$ のトポロジー 部分体であり、$K$ が離散的でないように、局所的にコンパクトな 2 つの (必ずしも可換ではない) 体とします。次に:*
(i) *$K'$ は、$K$ 上の有限次元の左 (右) ベクトル空間です。
(ii) *$K$が$K'$の中心に含まれる場合、すべての$x \in K'$について*。
(1)
$$
\operatorname{mod}_{K'}(x) = \operatorname{mod}_K(N_{K'/K}(x)).
$$
$K$ は離散的ではない完全な値の体であるため、主張 (i) はトポロジカルベクトル空間、章 I, § 2, no. 4、定理 3 から求まります。 主張 (ii) は単なる統合、章 VII, § 1, no. 11、命題 17。

#### 系 1 {#ac-vi-s9-prop-2-cor-1 .statement tag=04XS}

*中心が離散的でないローカル コンパクトフィールドはすべて、その中心を超える有限階数です。

ローカル コンパクト体 $K$ の中心 $Z$ は $K$ で閉じられているため、ローカル コンパクトです。

#### 系 2 {#ac-vi-s9-prop-2-cor-2 .statement tag=04XT}

*$K'$ を局所的にコンパクトな体とし、$K$ を $K'$ の閉じた部分体とします (どちらも可換である必要はありません)。 $K'$ が有限次元 $n$ の $K$ の左 (または右) ベクトル空間である場合、*
(2)
$$
\operatorname{mod}_{K'}(x) = (\operatorname{mod}_K(x))^n \quad \text{for all } x \in K.
$$

一般に、$K$ 上の有限次元 $n$ の (左または右) ベクトル空間では、比率 $x \in K$ のホモテティー の係数は $(\mathrm{mod}_K(x))^n$ に等しいことが知られています。これを$K'$に当てはめれば十分です。

### 2. 代表者の存在

#### 命題 3 {#ac-vi-s9-prop-3 .statement tag=04XU}

*$K$ を (必ずしも可換ではない) 局所的にコンパクトな体とします。これは離散的ではなく、その位相は離散評価 $v$ によって定義されます。 $A$を環、$m$を$v$の理想とし、$\mathrm{Card}(A/m) = q = p^f$(p素数)と書きましょう。次に、$A$の$A/m$の代表$S$の系と$v$の均一化器$u$が存在し、$O \in S$、$S^* = S \cap K^*$は$K^*$の巡回部分群となり、 $u^{-1} Su = S$。さらに、$A$ のすべての元は、形 $\sum_{i=0}^\infty s_i u^i$ ($s_i \in S$) で一意に記述できます。*

次の補題を使用します。

#### 補題 1 {#ac-vi-s9-lem-1 .statement tag=04XV}

*$x, y$ を、$x - y \in m^j \ (j \geq 1)$ となるように $A$ の 2 つの置換可能な元とします。その後、整数 $n \geq 0$ ごとに $x^{p^n} - y^{p^n} \in m^{j+n}$ となります。*

$n$の帰納法までに、$n = 1$では証明補題に減ります。それから

$$
x^p - y^p = (x - y)(x^{p-1} + x^{p-2}y + \ldots + y^{p-1});
$$

2 番目の因子は、1 つの他の mod に一致する $p$ 項の和です。 $m$ そして、$A/m$ は $p$ の特徴であるため、$A$ では $p \cdot 1 \in m$ となり、したがって

$$
x^{p-1} + x^{p-2}y + \ldots + y^{p-1} \in m;
$$

よって $x^p - y^p \in m^{j+1}$。

乗法群 $(A/m)^*$ は、$q - 1$ 元 (*代数*, 章 V, § 11, no. 1, 定理 1) と循環する群であることがわかっています。 $x$ をこの群の生成元の $A$ の代表とします。次に、$x^q - x \in m$、よって、補題 1、$x^{q^{n+1}} - x^{q^n} \in m^{1+fn}$ になります。$x^q$ と $x$ は置換可能であるためです。これは、$(x^{q^n})_{n \geq 0}$ が $A$ のコーシー 数列であることを証明します。 $A$ はコンパクトで完全なので、この数列は $A$ に極限があり、明らかに $s \equiv x \pmod{m}$ と $s^q = s$ を満たします。 $s \neq 0$、$s^{q-1} = 1$ のように、より正確には $s$ は、$A$ の単位元* の *プリミティブ* $(q-1)$* 番目の根です。明らかに、$0$ の集合 $S$ からなると冪 $s^j \ (0 \leq j \leq q-2)$ は、$A$ mod の類の *系の代表者* です。 $m$ であり、$A$ の乗法では *不変量* です。

ここで、$a$ を $v$ の均一化要素とし、$K$ の内部自己同型 $y \mapsto a^{-1}ya$ を考慮します。それ自体に対しては写像 $A$、それ自体に対しては $m$ であるため、商を取ると、体 $A/m$ の定義する自己同型になります。 (*代数*, 章 V, § 11, no. 4, 命題 5) 自己同型は形 $z \mapsto z^{p^r}$ であり、$0 \leq r \leq f-1$ であることが知られています。次に、$a^{-1}s^j a \equiv s^{jp^r} \pmod{m}$ が $0 \leq j \leq q-2$ になります。 $a \in m$ と $s \notin m$ は、$s^{-j}as^{jp^r} \equiv a \pmod{m^2}$ を意味します。

書いてみましょう

$$
u = \sum_{i=0}^{q-2} s^{-1} a s^i p^r.
$$

その後、$p . 1 \in m$ から $u \equiv (q - l) a \equiv -a (\text{mod. } m^2)$;私たち結論するは、$u$も$v$の均一化要素であると考えます。さらに
(3)
$$
s^{-1} u s^{p^r} = u
$$
よって $u^{-1} S u = S$ と推測します。

Finally, for all $x \in A$ there exists a unique sequence $(s_i)$ ($i \in \mathbf{N}$) such that $s_i \in S$ for all $i$ and $x \equiv \sum s_i u^i$ (mod. $m^{n+1}$) for all $n \geq 0$: it is immediate by induction on $n$, every element $t$ of $m^{n+1}$ satisfying a relation of the form $t \equiv t' u^{n+1}$ (mod. $m^{n+2}$), where $t'$ is a uniquely determined element of $S$. 次に、$x = \sum_{i=0}^{\infty} s_i u^i$ と家族 $(s_i)$ 満たすこの関係など、すべての $i$ に対する $s_i \in S$ が一意に決まります。

### 3. 構造のローカルコンパクト体

$\mathbf{Q}$ ($p$ 任意の素数) 上の不適切でない絶対値値に関する体 $\mathbf{Q}$ の補完 $\mathbf{R}$ と $\mathbf{Q}_p$ は局所的にコンパクトです。一方、有限体 $F$ 上の形式的な冪系列の素数数 $p$、体 $\mathbf{F}_q((T))$ のすべての冪 $q = p^f$ について、次のように定義されます。 § 3, no. 4、例 3 は *局所的にコンパクト*です。評価の最大理想値環 $\mathbf{F}_q[[T]]$ は $T$ によって生成されます。この環は (T) 進数位相 (章 III, § 2, no. 6, 命題 6) で完全であることがわかっており、剰余体 $\mathbf{F}_q$ が有限であるため、§ 5, no. 1 の 2 が命題であることが証明されます。 主張。逆に:

#### 定理 1 {#ac-vi-s9-thm-1 .statement tag=04XW}

*K を (必ずしも可換である必要はない) 局所的にコンパクトな体とし、これは離散的ではありません。*

(i) *K が標数 0 であり、mod が超計量絶対値値ではない場合、K は体 $\mathbf{R}, \mathbf{C}$ または $\mathbf{H}$ のいずれかと同型です。*

(ii) *K が標数 0 で、mod が超計量絶対値値である場合、K は p 進体 $\mathbf{Q}_p$ 上の有限階数の代数です。*

(iii) *K が標数 $p \neq 0$ の場合、形式べき級数 $\mathbf{F}_q((T))$ ($q$ は $p$ の累乗) を中心とする体とその中心に対する有限階数の体と同型です。*

(i) オストロフスキーの定理 (§ 6, no. 4、定理 2) から、K はどこでも密な部分体 $\mathbf{R}, \mathbf{C}$ または $\mathbf{H}$ と同型の位相体であり、K が完全であるため、$\mathbf{R}, \mathbf{C}$ または $\mathbf{H}$ と同型であることがわかります。

(ii) A を絶対値 mod の環とし、m をその最大理想とする。 A/m は有限体 (§ 5, no. 1, 命題 2) であることがわかっているため、mod によって $\mathbf{Q}$ に誘導される絶対値値は有限の剰余体を持ち、これは $p$ 進の絶対値値と同等である場合にのみ可能です。 ($§ 6$、no. 3、命題 4);したがって、$K$ の $\mathbf{Q}$ の閉包は $\mathbf{Q}_p$ と同型であり、後者は $K$ で閉包されているため、$K$ の中心に含まれます。私たちはを用いて結論する命題 no. 1 の 2 です。

(iii) 2 番目の主張は、最初の系から no. 2 の命題 2 に続きます。 最初の主張を示すために、mod は必然的に超計量絶対値 ($§ 6$, no. 2、命題 3 の帰結) であることに注意してください。 no. 2 の命題 3 の証明の表記では、$K$ の中心 $Z$ は、$s$ と $u$ の両方と可換な要素で構成されます。しかし、(3) のおかげで、

$$
u^{-q} s u^q = s^{q p^r} = s,
$$

したがって、$u^q \in Z$ と私たち結論するは、$Z$ が離散的ではありません。 $Z$ は局所的にコンパクトであるため、$K$ が可換である場合に注意を限定することができます。 $K$ の部分$\mathbf{F}_p$-代数 $\mathbf{F}_p[s]$ は、$s^{q-1} = 1$ から有限体であり、この体のすべての元に対して明らかに $y^q = y$ であり、したがって、$S$ と同一であり、$\mathbf{F}_q$ と同型です。 $S \subset \mathbf{F}_p[s]$ には $q$ 元があります。 $S$の2つの元のうち和は$S$にあるので、冪系列$\sum_{i=0}^\infty s_i T^i \in \mathbf{F}_q[[T]]$から元$\sum_{i=0}^\infty s_i u^i$の写像を合わせた写像は全単射です環 $\mathbf{F}_q[[T]]$ の準同型を環 $A$、よってに即結論。

#### 系 1 {#ac-vi-s9-thm-1-cor-1 .statement tag=04XX}

*離散ではない*局所的にコンパクトなすべての体* は、その中心に対して有限階数* です。

#### 系 2 {#ac-vi-s9-thm-1-cor-2 .statement tag=04XY}

ローカルのすべての *コンパクト体* は接続されています *、または * 完全に切断されています。 *接続されている場合*、それは $\mathbf{R}, \mathbf{C}$ *または* $\mathbf{H}$ と *同型* です。

体 $K$ 上の位相が超計量絶対値値によって定義される場合、$K$ はこの位相と完全に切り離されます。

#### 注意 {#ac-vi-s9-n3-rem-1 .statement tag=04XZ}

$s$ を整数 $> 0$ とします。 部分体 $K = \mathbf{F}_q((T))$ の $\mathbf{F}_q((T^s)) = L$ は、 $K$ と $e(K/L) = s$ と $f(K/L) = 1$ はお休みです。したがって、離散的ではなく、$e(K/L)$ (および *なおさら* 次数 $[K:L]$) が任意に大きいような $K$ の閉じた部分体 $L$ が存在します (特性 0 の局所的にコンパクトな体で起こることとは対照的に、すべてのローカルでコンパクトです)このような体 $K$ の部分体 $L$ は必然的に含む $\mathbf{R}$ または $\mathbf{Q}_p$ となり、したがって $[K:L]$ は有界となります)。

### 練習問題 {#ac-vi-s9-exercises}

22. (a) 体 K に離散評価が存在する場合、K の代数閉包が K に対して無限であることを示します。

(b) K を体 $K_0$ の有限生成拡大とする。 K が $K_0$ に対して代数的でない場合、$K_0$ に対して $v(x) = 0$ となるような K に対する離散評価 $v$ が存在することを示します。

39

[§ 9 に対して練習問題](exercises/s9/)を参照してください。
