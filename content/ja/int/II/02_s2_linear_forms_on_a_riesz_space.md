---
book: int
book_title: Integration
chapter: II
chapter_title: RIESZ SPACES
section: 2
section_title: Linear forms on a Riesz space
lang: ja
source: int-i-vi
book_pages: INT II.19-INT II.21
pdf_pages: 0033-0039, 0043-0045
extraction: ocr
subsections:
    - "no": 1
      title: Positive linear forms on a Riesz space
      page: 9
      pdf_page: 33
    - "no": 2
      title: Relatively bounded linear forms
      page: 10
      pdf_page: 34
statements: 13
exercises: 9
content_sha256: ba60235bb777c40aa0088913cc0be8326f31db56dcda11c96bbb7c1556e37272
translated_from: content/en/int/II/02_s2_linear_forms_on_a_riesz_space.md
translation_method: google
source_content_sha256: 417cef2f31fafd157b7a2cbea53f12a17f40a56765605873734c2f538ed5f1ad
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-dda8bbaf
glossary_version: 34
glossary_terms_sha256: 8fde887fe0207e1c798bfa8621d5b52490dcb907549deca9a4257139d1b18a78
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## § 2。リースで線型形式空間

### 1. リース空間でポジティブ線型形式

次の定義 (TVS、II, §2, No. 5) を思い出します。

#### 定義 1 {#int-ii-s2-def-1 .statement tag=08KI}

順序付けられたベクトル空間 E が与えられた場合、E の線型形式 L は、E の $x \geq 0$ ごとに $L(x) \geq 0$ であれば正であると言われます。

$L(y) - L(x) = L(y - x)$ 以来、関係 $x \leq y$ が $L(x) \leq L(y)$ を暗示するか、または E で $L$ が増加する写像であると言うのは同じです。

#### 例 1 {#int-ii-s2-n1-exa-1 .statement tag=08KJ}

A を任意の集合、E を A 上で定義されたすべての実数値写像の空間 $\mathbf{R}^A$ の線形部分空間とします。すべての元 $a \in A$ について、写像 $x \mapsto x(a)$ は E 上の正の線型形式です。

#### 例 2 {#int-ii-s2-n1-exa-2 .statement tag=08KK}

$I = [a, b]$ を $\mathbf{R}$ のコンパクト区間とし、E は I (FRV、II, §1, No. 3) 上の規制された実数値写像によって形成されるリース空間とします。 写像 $x \mapsto \int_a^b x(t) \, dt$ は E のプラスの線型形式です。

#### 例 3 {#int-ii-s2-n1-exa-3 .statement tag=08KL}

F を F 上の任意の集合、$\mathscr{U}$ の限外フィルター (GT、I, §6, No. 4)、E を F 上の有界実数値写像の Riesz 空間 $\mathscr{B}(F)$ とします。 $x(\mathscr{U})$ は比較的コンパクトな集合 $x(F)$ 上の限外フィルターの基底であるため、すべての $x \in E$ に対して $\lim_{\mathscr{U}} x(t)$ が存在し、したがって収束します。 さらに、$x \geq 0$なら拡大の不等式原理により$\lim_{\mathscr{U}} x(t) \geq 0$になります。従って、写像 $x \mapsto \lim_{\mathscr{U}} x$ は E の正の線型形式です。 $\mathscr{U}$ を集合含む元 $a \in F$ によって形成される限外フィルターとすると、正の線型形式 $x \mapsto x(a)$ (例 1) が回収されます。

#### 命題 1 {#int-ii-s2-prop-1 .statement tag=08KM}

E を、$L(x + y) = L(x) + L(y)$ となり、関係 $x \geq 0$ が $L(x) \geq 0$ を意味するような、E の $\mathbf{R}$ への順序付けられたベクトル空間、L 写像とします。次に、すべてのスカラー $\lambda$ とすべての $x \geq 0$ に対して $L(\lambda x) = \lambda L(x)$ が計算されます。

$L(-x) = -L(x)$ ($L$ は $\mathbf{R}$ の加法群 E の表現である) なので、$\lambda \geq 0$ の場合に限定できます。 整数 $n \geq 0$ ごとに、$L(nx) = nL(x)$、よって $L((1/n)x) = (1/n)L(x)$ があり、その結果、すべての有理数数 $r \geq 0$ に対して $L(rx) = rL(x)$ が得られます。一方、$L$ は E では増加するです。 $r$ と $r'$ が $r \leq \lambda \leq r'$ となるような有理数である場合、$rL(x) \leq L(\lambda x) \leq r'L(x)$ になります。 $rL(x)$ と $r'L(x)$ は $\lambda L(x)$ とほとんど変わらないので、$L(\lambda x) = \lambda L(x)$ になります。

#### 命題 2 {#int-ii-s2-prop-2 .statement tag=08KN}

Let E be a real vector space, C a convex cone with vertex 0 in E such that $E = C - C$, and $x \mapsto M(x)$ a mapping of C into $\mathbf{R}$ such that $M(\lambda x + \mu y) = \lambda M(x) + \mu M(y)$ for all $x \in C$, $y \in C$, $\lambda \geq 0$, $\mu \geq 0$. すると、拡大する M to E という線型形式 L が唯一つ存在します。

仮定までに、すべての $z \in E$ は $z = y - x$ に書き込まれます。ここで、$x, y$ は属するから C です。さらに、$z = y' - x'$ と $x' \in C$、$y' \in C$ の場合、

$M(y) - M(x) = M(y') - M(x')$;なぜなら、関係 $y - x = y' - x'$ から $y + x' = x + y'$ が推論され、その結果 $M(y) + M(x') = M(x) + M(y')$ となるからです。 $z$ のすべての式について、$C$ の 2 つの元の差 $y - x$ を、$M(y) - M(x)$ の $L(z)$ 共通の値で表しましょう。 $L$ が $M$ を延長した $E$ 上の線型形式であることがすぐに検証されます。 $L$ の一意性は、$C$ 生成する空間 $E$ という事実から生じます。

#### 命題 3 {#int-ii-s2-prop-3 .statement tag=08KO}

*$E$を、元の$\geqslant 0$、$E$のベクトル空間、$P$集合、$P$の$x \mapsto M(x)$写像を$\mathbf{R}$に指定したものとします。 値 $\geqslant 0$、$P$ のすべての $x, y$ に対して $M(x + y) = M(x) + M(y)$ となります。すると、拡大する $M$ から $E$ までの正の線型形式 $L$ が 1 つだけ存在します。*

$E = P - P$ なので、提案 2 と同じ推論は、まず、$E$ の $\mathbf{R}$ への *加法* 写像 $L$ の存在と一意性が拡大する $M$ であることを証明します。 命題 1 は、すべての $\lambda \geqslant 0$ とすべての $x \in P$ に対して $L(\lambda x) = \lambda L(x)$ であることを示し、そこから明らかであるため、$L$ は線型形式になります。

### 2. 比較的限定された線型形式

$E$ を有向順序ベクトル空間とします。 $Q$ を $E$ の *正* 線型形式の集合とします。それは、$E$ の代数双対 $E^*$ の部分集合 ($E$ 上のすべての線型形式の空間) です。すべてのスカラー $\lambda > 0$ に対して $Q + Q \subset Q$ と $\lambda Q \subset Q$ が一致するのは明らかです (他の語では、$Q$ は $E^*$ の *凸円錐* です)。さらに、$Q \cap (-Q) = \{0\}$ は、$L$ と $-L$ が両方とも正の線型形式である場合、すべての $x \geqslant 0$ に対して $L(x) \geqslant 0$ と $L(x) \leqslant 0$、すべての $x \geqslant 0$ に対してよって $L(x) = 0$ となるため、 $L = 0$ (No. 1、提案 3)。 集合 $Q$ したがって、$E^*$ の定義するは *位数関係* $L \leqslant M$、« $M - L$ は $E$ の正の線型形式 »、またはすべての場合に再び « に相当します。 $x \geqslant 0$、$L(x) \leqslant M(x)$ »;この位数構造に対する $E^*$ の元 $\geqslant 0$ は、正の線型形式です (これにより、導入された用語が正当化されます)。 $\Omega$を、$Q$によって生成された$E^*$の線形部分空間、つまり$E$上の線型形式の集合、つまり*2つの正の線型形式の差*であるとします。 $E$ がリース空間の場合、$\Omega$ の元のうち他の特徴付けを与えることになります。

#### 定義 2 {#int-ii-s2-def-2 .statement tag=08KP}

*リース空間 $E$、$E$ の線型形式 $L$ は、$E$ のすべての $x \geqslant 0$ に対して、$L$ が $y \in E$ の集合で境界がある場合、相対的に有界であると言われます。 $|y| \leqslant x$.*

#### 定理 1 {#int-ii-s2-thm-1 .statement tag=08KQ}

1° *リース空間 $E$ 上の線型形式 $L$ が相対的に有限である位数において、それが 2 つの正の線型形式の差であることが必要かつ十分です。*

$E$ 上の相対的に有界な線型形式の 2° *順序付けされたベクトル空間 $\Omega$ は、完全に格子順序付けされたリース空間です。

$L = U - V$ の場合、$U$ と $V$ が $E$ で正の線型形式である場合、関係 $-x \leq y \leq x$ は、

$$
-U(x) \leq U(y) \leq U(x) \quad \text{and} \quad -V(x) \leq V(y) \leq V(x),
$$

よって $|L(y)| \leq U(x) + V(x)$ は明らかです。したがって、$L$ は比較的有界です。逆に、$L$ が比較的有界であると仮定します。つまり、すべての $x \geq 0$ に対して $N(x) \geq L(x)$ となるような正の線型形式 $N$ が存在するということは、$N - L$ が正の線型形式になるため、証明に帰着します。

さて、正の線型形式 $N$ がこの性質を持つ場合、すべての $x \geq 0$ と $0 \leq y \leq x$ について、$N(x) \geq N(y) \geq L(y)$ があり、したがって $N(x) \geq \sup_{0 \leq y \leq x} L(y)$ になります。実数値写像が証明されれば

$$
x \mapsto M(x) = \sup_{0 \leq y \leq x} L(y),
$$

元 $\geq 0$ の $E$ の集合 $P$ で定義され、$E$ のプラスの線型形式 ($M$ とも表される) に拡張できます。定理の最初の部分が実証され、次のようになります。さらに、$M$ が $\Omega$ における $0$ と $L$ の最高値であることも証明されました。 $P$の$M(x) \geq 0$から、すべては証明に帰着します。

$$
M(x + x') = M(x) + M(x')
$$

$E$ の元 $x \geq 0,\ x' \geq 0$ ごとに対 (No. 1、提案 3)。 定義までに、

$$
M(x) + M(x') = \sup_{0 \leq y \leq x} L(y) + \sup_{0 \leq y' \leq x'} L(y')
= \sup_{0 \leq y \leq x,\ 0 \leq y' \leq x'} L(y + y') \leq M(x + x').
$$

一方、$0 \leq z \leq x + x'$ のようなすべての $z$ に対して、$u \geq 0$ を伴う $x + x' = z + u$ が得られます。 分解補題 (§ 1, No. 1) により、$0 \leq y \leq x,\ 0 \leq y' \leq x'$ と $z = y + y',\ u = (x - y) + (x' - y')$ のような 2 つの元 $y,\ y'$ が存在します。それから

$$
L(z) = L(y) + L(y') \leq M(x) + M(x'),
$$

したがって、$M(x + x') = \sup_{0 \leq z \leq x + x'} L(z) \leq M(x) + M(x')$ は、定理の最初の部分の証明を完了します。さらに、$\Omega$ が *Riesz 空間* であり、$E$ 上の相対的に有界なすべての線型形式 $L$ とすべての $x \geq 0$ について、

(1)
$$
L^+(x) = \sup_{0 \leq y \leq x} L(y).
$$

$\Omega$ が完全に格子順序付けされているかどうかはまだわかりません。このためには、*正* 線型形式の任意の集合 $H$ が、上に境界があり、関係 $\leqslant$ に向けられており、$\Omega$ に最高値があることを示すだけで十分です。

より一般的には、次の補題があります。

#### 補題 {#int-ii-s2-n2-lem-1 .statement tag=08KR}

— *E を有向順序ベクトル空間、$E^*$ を正の元と正の線型形式として順序付ける双対とします。 $(u_\alpha)$ を $E^*$ の元の増加する直系家族とします。 E のすべての $x \geqslant 0$、$\sup u_\alpha(x) < +\infty$ について、家族 $(u_\alpha)$ には $E^*$ の最高値 $u$ があり、E のすべての $x \geqslant 0$ について、

$$
u(x) = \sup_{\alpha} u_\alpha(x).
$$

E のすべての $x \geqslant 0$ のうち集合 P では、公式による定義する写像 $u$ (2)。 $\lambda \geqslant 0$ と $x \in P$ のすべてに対して $u(\lambda x) = \lambda u(x)$ は明らかです。したがって、補題を証明するには、No. 1 の提案 2 によって、次のことを示せば十分です。

$$
u(x + y) = u(x) + u(y)
$$

Pの$x, y$の場合。しかし、これは添字の有向集合に関して$u(x) = \lim u_\alpha(x)$である観察するとの明らかです（モノトーン極限定理）。

公式 (1) から、$L$ と $M$ が E 上で相対的に境界のある 2 つの線型形式である場合、$x \geqslant 0$ ごとに、

$$
\begin{cases}
\sup(L, M)(x) = \sup_{y \geqslant 0,\ z \geqslant 0,\ y+z=x} (L(y) + M(z)) \\
\inf(L, M)(x) = \inf_{y \geqslant 0,\ z \geqslant 0,\ y+z=x} (L(y) + M(z)).
\end{cases}
$$

特に、これらの最初の公式で、$M$ が $-L$ に置き換えられると、次のようになります。

$$
|L|(x) = \sup_{y \geqslant 0,\ z \geqslant 0,\ y+z=x} L(y - z).
$$

ここで、$x = y + z$、$y \geqslant 0$、$z \geqslant 0$ の場合は、$-x \leqslant y - z \leqslant x$ になります。逆に、関係 $|u| \leqslant x$ は $L(u) \leqslant |L|(|u|) \leqslant |L|(x)$ を意味します。これから、公式を導き出します。

$$
|L|(x) = \sup_{|y| \leqslant x} L(y) \quad \text{for } x \geqslant 0,
$$

よって、特に、

$$
|L(x)| \leqslant |L|(|x|)
$$

すべての$x \in E$に。

#### 命題 4 {#int-ii-s2-prop-4 .statement tag=08KS}

— In order that two positive linear forms $L, M$ on a Riesz space $E$ be alien to each other in the space $\Omega$, it is necessary and sufficient that, for every number $\varepsilon > 0$ and every $x \geq 0$ in $E$, there exist two elements $y \geq 0, z \geq 0$ of $E$ such that $x = y + z$ and $L(y) + M(z) \leq \varepsilon$.

確かに、(3) の 2 番目の公式により、この条件はその $\inf(L, M) = 0$ を表します。

#### 命題 5 {#int-ii-s2-prop-5 .statement tag=08KT}

— リース空間 $E$ で $L$ を正の線型形式とします。 位数では、$\Omega$ の $L$ によって生成されたバンドに対して、$E$ 属するで正の線型形式 $M$ が$E$ のすべての $x \geq 0$ とすべての数 $\varepsilon > 0$ について、次のことが必要かつ十分です。 関係 $0 \leq y \leq x$ と $L(y) \leq \delta$ が $M(y) \leq \varepsilon$ を暗示するような数 $\delta > 0$ が存在します。

まず条件が必要であることを示しましょう。 $\Omega$ で $L$ によって生成されたバンドが $M \geq 0$ 属するの場合、 (§ 1, No. 5、提案 6 の修正)

$$
M = \sup_n \left( \inf(nL, M) \right).
$$

1 つ集合の場合

$$
U_n = M - \inf(nL, M),
$$

従って、$U_n$ は、$E$ では正の線型形式、$\Omega$ では$\inf_n U_n = 0$ になります。その結果、(補題) $U_n(x)$ は 0 になる傾向があり、$n$ は無限大になる傾向があり、$U_n(x) \leq \varepsilon/2$ となるような $n$ が存在します。このような $n$ を修正すると、$0 \leq y \leq x$ となるすべての $y$ に対して $U_n(y) \leq \varepsilon/2$ が得られ、したがって関係 $0 \leq y \leq x$ は意味します

$$
M(y) \leq \frac{\varepsilon}{2} + \inf(nL, M)(y) \leq \frac{\varepsilon}{2} + nL(y);
$$

$y$ が $L(y) \leq \varepsilon/2n$ である場合、$M(y) \leq \varepsilon$ が続き、主張が確立されます。

ここで、条件で十分であることを示しましょう。 $E$ のすべての正の線型形式 $M$ に対して、$M = U + V$ を書くことができます。ここで、$U$ 属するは、$\Omega$ の $L$ によって生成されたバンドに属し、$V$ は$L$、$U$、および$V$ は陽性です (§ 1, No. 5、Th. 1)。 $M$ が主張の条件を満たす場合、$0 \leq V \leq M$ 以降、$V = M - U$ も満たします。これから、$V = 0$ と推測します。 $E$ のすべての $x \geq 0$ とすべての数 $\eta > 0$ に対して、$x = y + z$ と $L(y) + V(z) \leq \eta$ のように、$E$ の 2 つの元 $y \geq 0, z \geq 0$ が存在します (提案 4)。任意の数 $\varepsilon > 0$、選ぶ $\eta \leq \varepsilon$ が与えられると、関係 $0 \leq u \leq x$ および $L(u) \leq \eta$ は $V(u) \leq \varepsilon$ を意味します。 $y$ と $z$ を上記のように決定すると、$L(y) \leq \eta$ となり、したがって $V(y) \leq \varepsilon$ となります。

$$
V(x) = V(y) + V(z) \leq \varepsilon + \eta \leq 2\varepsilon;
$$

$\varepsilon$ は任意なので、$x \geq 0$ ごとに $V(x) = 0$、つまり $V = 0$ になります。

#### 例 {#int-ii-s2-n2-exa-1 .statement tag=08KU}

E を、その順序付けられたベクトル空間構造 (TVS、II, §2, No. 7) と互換性のある局所凸位相を備えたリース空間とする。 E' を E の位相双対とし、加法において、E の元 $\geqslant 0$ の円錐 P が弱化された位相* $\sigma(E, E')$ に対して*完全であると仮定します。 次に、すべての連続線型形式 $x' \in E'$ は *比較的有界* です。なぜなら、これら条件の下では、$y \in E$ の E 集合のすべての $x \geqslant 0$ について、$|y| \leqslant x$ が *コンパクト* であることがわかるからです (TVS、II, §6, No. 8、提案 11 の Cor. 2)。 $\sigma(E, E')$。 このことから、E は *完全に格子順序付けされている * と推測されます。 ($§ 1$, No. 3, 提案 2) については、上で制限され $\leqslant$ に向けられたすべての集合 $H \subset E$ について、H の切断フィルター $\mathscr{F}$ が位相* $\sigma(E, E')$ (後者) について E に *収束することを示すだけで十分です。 E) の注文されたベクトル空間構造と互換性があります。 翻訳すると、$H \subset P$ と仮定でき、その後、$\mathscr{F}$ が $\sigma(E, E')$ に対する *Cauchy フィルター* であること、またはすべての連続する線型形式 $x' \in E'$ が $\mathscr{F}$ に関して極限を持つことを再度示すだけで十分です。 しかし、これは、$x'$ が *正* 線型形式であるとき、単調極限定理からすぐに続き、すべての線型形式 $x' \in E'$ は 2 つの正の線型形式 (Th. 1) の差であるため、私たちの主張が証明されます。

練習問題

### 練習問題 {#int-ii-s2-exercises}

[§ 2 に対して練習問題](exercises/s2/)を参照してください。
