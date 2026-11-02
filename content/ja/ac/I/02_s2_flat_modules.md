---
book: ac
book_title: Commutative Algebra
chapter: I
chapter_title: FLAT MODULES
section: 2
section_title: Flat modules
lang: ja
source: ac-i-vii
book_pages: 9-27, 41-49
pdf_pages: 0029-0047, 0061-0069
extraction: ocr
subsections:
    - "no": 1
      title: REVISION OF TENSOR PRODUCTS
      page: 9
      pdf_page: 29
    - "no": 2
      title: M-FLAT MODULES
      page: 10
      pdf_page: 30
    - "no": 3
      title: FLAT MODULES
      page: 12
      pdf_page: 32
    - "no": 4
      title: EXAMPLES OF FLAT MODULES
      page: 14
      pdf_page: 34
    - "no": 5
      title: FLATNESS OF QUOTIENT MODULES
      page: 15
      pdf_page: 35
    - "no": 6
      title: INTERSECTION PROPERTIES
      page: 17
      pdf_page: 37
    - "no": 7
      title: TENSOR PRODUCTS OF FLAT MODULES
      page: 19
      pdf_page: 39
    - "no": 8
      title: FINITELY PRESENTED MODULES
      page: 20
      pdf_page: 40
    - "no": 9
      title: EXTENSION OF SCALARS IN HOMOMORPHISM MODULES
      page: 22
      pdf_page: 42
    - "no": 10
      title: 'EXTENSION OF SCALARS: CASE OF COMMUTATIVE RINGS'
      page: 22
      pdf_page: 42
    - "no": 11
      title: INTERPRETATION OF FLATNESS IN TERMS OF RELATIONS (*)
      page: 25
      pdf_page: 45
statements: 37
exercises: 24
content_sha256: 72aa2246f66f03e453b03099ff370f4b15d2d7ee837b61337d2f27a19b139067
translated_from: content/en/ac/I/02_s2_flat_modules.md
translation_method: google
source_content_sha256: 28d69ca6e99e7466a70edf5b1c736029d397199a01db0537698a81ada5d7fea8
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-eeeca2ef
glossary_version: 34
glossary_terms_sha256: 4e1e138175d9682a555f6a3ecc5127debf7f742037a4d977aa5bf493f6d04a47
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## 2. フラット加群(*)

### 1. テンソル積の改訂

A を環、E 右A-加群、M 左A-加群とします。 代数、章 II, §3, no. 1 では、$\mathbf{Z}$ モジュールであるテンソル積 $E \otimes_A M$ を定義しました。 E' (または M') が右 (または左) A-加群および $u : E \to E'$ (それぞれ $v : M \to M'$) 準同型である場合、(loc. cit, no. 2) $\mathbf{Z}$ 準同型性も定義しました。

$$
u \otimes v : E \otimes_A M \to E' \otimes_A M'.
$$

#### 補題 1 {#ac-i-s2-lem-1 .statement tag=042F}

*$M' \xrightarrow{v} M \xrightarrow{w} M'' \to 0$ *を左A-加群と E 右A-加群の完全系列とします。それでは数列*

$$
E \otimes_A M' \xrightarrow{\text{1}\otimes v} E \otimes_A M \xrightarrow{u \otimes w} E \otimes_A M'' \longrightarrow 0
$$

*は可換群の完全系列です。*

代数、章 II, § 3, no. 6の系から命題の5です。

したがって、任意の左A-加群準同型 $u : M \to N$ について、

$$
E \otimes_A (\operatorname{Coker} u)
$$

完全系列に適用される場合、補題 1 が示すように、正規的には $\operatorname{Coker}(1_E \otimes u)$ で識別されます。

$$
M \xrightarrow{u} N \longrightarrow \operatorname{Coker} u \longrightarrow 0.
$$

補題 1 の記法では、v が*単射*である場合、つまり数列 $0 \to M' \xrightarrow{v} M \xrightarrow{w} M'' \to 0$ が正確である場合、必ずしも $1_E \otimes v$ が単射であるとは限らず、したがって一般に $E \otimes_A M'$ できないは

(*) すでにホモロジー 代数に精通している読者には、§ 4 でフラット加群の他の特徴付けが見つかることをお知らせします。

$E \otimes_A M$のサブグループ。ただし、次の結果 (代数、章 II, § 3, no. 7、系 5 ～ 命題 7) を思い出してください。

#### 補題 2 {#ac-i-s2-lem-2 .statement tag=042G}

*$v : M' \to M$が単射で、$v(M')$が$M$の直因子である場合、準同型$1, \otimes v$は単射で、その像は$E \otimes_A M$の直因子です。

### 2. M-フラット加群

#### 定義 1 {#ac-i-s2-def-1 .statement tag=042H}

$A$ を環、$E$ を右側の $A$ モジュール、$M$ を左側の $A$ モジュールとします。左のすべての $A$ モジュール $M'$ とすべての単射準同型 $v : M' \to M$、準同型 $l_E \otimes v : E \otimes_A M' \to E \otimes_A M$ が単射である場合、$E$ は $M$ (または $M$-フラット) に対してフラットであると言われます。

右側の $A$ モジュール $N$、$N$ フラット左加群の概念も同様に定義されます。右の $A$ モジュール $E$ が左 $A$ モジュール $M$ に対して平坦であると言うのは、左 $A^0$ モジュールとみなされる $E$ がというに相当します ($A^0$ が示すことを思い出してください) 反対環 ～ $A$)、右側の $A^0$ モジュール $M$ はフラットです。

#### 補題 3 {#ac-i-s2-lem-3 .statement tag=042I}

*タイトな$A$モジュール$E$が$M$フラットであるためには、$M$標準準同型*の有限生成されるすべての部分加群$M'$に対して、次のことが必要かつ十分です。

$$
l_E \otimes j : E \otimes_A M' \to E \otimes_A M
$$

(*j は標準単射 $M' \to M$) *単射語であること*。

この条件が成り立ち、$N$ を $M$ のいずれかの部分加群とします。 元の $E \otimes_A M$ に標準像があるとします。

$$
z = \sum x_i \otimes y_i \in E \otimes_A N \quad (x_i \in E, y_i \in N)
$$

は零であり、$M'$ をそれらによって生成された $N$ の有限生成された部分加群とします。 仮定によると、合成写像 $E \otimes_A M' \to E \otimes_A N \to E \otimes_A M$ は単射であり、和 $z' = \sum x_i \otimes y_i$ は、$E \otimes_A M'$ の元と見なされ、零になります。 *$z$は$z'$の像であるため、$z = 0$、よって補題もあります。

#### 補題 4 {#ac-i-s2-lem-4 .statement tag=042J}

*$E$が$M$フラットとなるように、$E$を右の$A$モジュール、$M$を左の$A$モジュールとします。 $N$ が $M$ の部分加群または商加群の場合、$E$ は $N$-フラット* になります。

$N$ が部分加群である場合は、$N'$ が $N$ の部分加群である場合、合成準同型であるため、簡単です。

$$
E \otimes_A N' \to E \otimes_A N \to E \otimes_A M
$$

は単射なので、$E \otimes_A N' \to E \otimes_A N$も同様です。次に、$N$ が $M$ の商加群であるとします。つまり、完全系列 $0 \to R \xrightarrow{i} M \xrightarrow{p} N \to 0$ が存在します。

$N'$を$N$と$M' = \overline{p}(N')$の部分加群とします。 $i'$は、$i$と同じグラフで$R$から$M'$の写像、$p'$は、$p$から$M'$の制限と同じグラフで、全射$M \to N'$を表すとします。 $\mathbf{R}$ から $\mathbf{R}$ までの $r$ 恒等写像、$m$ 標準単射 $M' \to M$ および$n$ 標準単射 $N' \to N$。 図式

$$
\begin{array}{ccccccccc}
0 & \longrightarrow & \mathbf{R} & \xrightarrow{i'} & M' & \xrightarrow{p'} & N' & \longrightarrow & 0 \\
& & \downarrow r & & \downarrow m & & \downarrow n & & \\
0 & \longrightarrow & \mathbf{R} & \xrightarrow{i} & M & \xrightarrow{p} & N & \longrightarrow & 0
\end{array}
$$

は可換であり、その行は正確です。

記述を簡略化するために、左のすべての $A$ モジュール $Q$ に対して集合 $T(Q) = E \otimes_A Q$ を、左のすべての $A$ モジュール準同型 $v$ に対して $T(v) = 1_E \otimes v$ を使用します。 図式

$$
\begin{array}{ccccccccc}
T(\mathbf{R}) & \xrightarrow{T(i')} & T(M') & \xrightarrow{T(p')} & T(N') & \longrightarrow & 0 \\
\downarrow T(r) & & \downarrow T(m) & & \downarrow T(n) & & \\
T(\mathbf{R}) & \xrightarrow{T(i)} & T(M) & \xrightarrow{T(p)} & T(N) & \longrightarrow & 0
\end{array}
$$

は可換であり、その行は no. 1 の補題 1 によって正確です。さらに、$E$ は $M$-フラットであるため、準同型 $T(m)$ は単射法です。 $T(r)$ と $T(p')$ は全射であるため、§ 1, no. 4, 系 2 から命題 2 から $T(n)$ は単射であることがわかり、補題が証明されます。

#### 補題 5 {#ac-i-s2-lem-5 .statement tag=042K}

$(M_i)_{i \in I}$ を左側の $A$ モジュール、$M = \bigoplus_{i \in I} M_i$ とその直和、および $E$ を右側の $A$ モジュールのファミリーとします。すべての $i \in I$ について、$E$ が $M_i$ に対してフラットである場合、$E$ は $M$ に対してフラットです。

(a) まず、$I = \{1, 2\}$ を仮定し、$M'$ を $M = M_1 \oplus M_2$、$M$、$M$ の部分加群とし、$M$ の部分加群と正規に識別します。 Denote by $M'_1$ the intersection $M' \cap M_1$, and by $M'_2$ the image of $M'$ in $M_2$ under the canonical projection $p$ of $M$ onto $M_2$. 図式があります

$$
\begin{array}{ccccccccc}
0 & \longrightarrow & M'_1 & \xrightarrow{i'} & M' & \xrightarrow{p'} & M'_2 & \longrightarrow & 0 \\
& & \downarrow v_1 & & \downarrow v & & \downarrow v_2 & & \\
0 & \longrightarrow & M_1 & \xrightarrow{i} & M & \xrightarrow{p} & M_2 & \longrightarrow & 0
\end{array}
$$

ここで、$v_1, v, v_2, i, i'$ は標準単射、$p'$ は写像で、$p$ ～ $M'$ の制限と同じグラフであり、これは全射です。この図式が可換であること、およびその行が正確であることがすぐに検証されます。 $T(Q)$ と $T(v)$ を補題 4 の証明と同じ意味で使用すると、可換図式が得られます。

$$
\begin{array}{ccccccccc}
T(M'_1) & \xrightarrow{T(i')} & T(M') & \xrightarrow{T(p')} & T(M'_2) \\
\downarrow T(v_1) & & \downarrow T(v) & & \downarrow T(v_2) \\
T(M_1) & \xrightarrow{T(i)} & T(M) & \xrightarrow{T(p)} & T(M_2)
\end{array}
$$

no. 1 の補題 1 までに、この図式の 2 行は正確です。 E は $M_1$ と $M_n$ に対してフラットなので、$T(v_1)$ と $T(v_2)$ は単射です。さらに、no. 1の補題2により、$T(i)$は単射法になります。 § 1, no. 4 の系 2 から命題 2 は、$T(v)$ が単射的であり、その結果 E が M-フラットであることを示します。

(b) If I is a finite set with n elements, the lemma follows by induction on n using (a).

(c) 一般の場合、$M'$ を M の有限生成された部分加群とします。そのとき、$M'$ が直和 $M_J = \bigoplus_{i \in J} M_i$ に含まれるようなインデックス集合 I の有限部分集合 J が存在します。 (b) E は $M_J$ に対してフラットです。従って、標準準同型 $E \otimes_A M' \to E \otimes_A M$ は単射法です。一方、$M_J$ は M の直因子であるため、標準準同型 $E \otimes_A M_J \to E \otimes_A M$ は単射法 (no. 1, 補題 2) です。 合成を取ると、$E \otimes_A M, \to E \otimes_A M$ は単射法であり、E は補題 3 によって M に対してフラットであることがわかります。

### 3. フラット加群

#### 命題 1 {#ac-i-s2-prop-1 .statement tag=042L}

Eを右A-加群とします。次の 3 つのプロパティは同等です。

(a) E は A に対して平坦です (他の語では、A のすべての左イデアル $a$ に対して、標準準同型 $E \otimes_A a \to E \otimes_A A, = E$ は単射法です)。
(b) E は左A-加群 M ごとの M-フラットです。
(c) 左A-加群と準同型の完全系列ごとに

$$
M' \xrightarrow{v} M \xrightarrow{w} M''
$$

数列

$$
E \otimes_A M' \xrightarrow{1 \otimes v} E \otimes_A M \xrightarrow{1 \otimes w} E \otimes_A M''
$$

正確です。

(b) が (a) を意味するのは明らかです。逆に、(a) が成り立つと仮定します。 no. 2 の補題 5 まで、E は無料の左A-加群ごとにフラットです。すべての左A-加群は自由加群の商 (代数、章 11、§ 1, no. 11、命題 20) と同型であるため、no. 2 の補題 4 から E は M に対してフラットであることがわかります。

(c) が (b) を意味することを示します。 $v : M' \to M$ が単射準同型の場合、数列 $0 \to M' \xrightarrow{v} M$ は正確です。 by (c) 数列

$$
0 \to E \otimes_A M' \xrightarrow{1 \otimes v} E \otimes_A M
$$

正確です。これは、$1 \otimes v$ が単射法であり、他の語では E が M-フラットであることを意味します。

最後に、(b) $\Rightarrow$ (c) の意味は、より正確には次の補題の帰結です。

#### 補題 6 {#ac-i-s2-lem-6 .statement tag=042M}

*$M' \xrightarrow{v} M \xrightarrow{w} M''$ が左A-加群の完全系列で、E が $M''$-フラット右A-加群、数列の場合*

$$
E \otimes_A M' \xrightarrow{1 \otimes v} E \otimes_A M \xrightarrow{1 \otimes w} E \otimes_A M''
$$

*正確です。*

記法 $T(Q)$ と $T(v)$ は、補題 4 の no. 2 の証明と同じ意味で使用します。 wと同じグラフで$M_1'' = w(M)$と書き、$i : M_1'' \to M''$をMから$M_1''$までの標準単射と$p$写像とします。 数列 $M' \xrightarrow{v} M \xrightarrow{p} M_1'' \to 0$ は正確で、no. 1 の補題 1 から数列になります。

$$
T(M') \xrightarrow{T(v)} T(M) \xrightarrow{T(p)} T(M_1'') \longrightarrow 0
$$

正確です。さらに、E は $M''$-フラットであるため、写像 $T(i) : T(M_1'') \to T(M'')$ は単射法であり、$T(i) \circ T(p) = T(w)$ として、数列

$$
T(M') \xrightarrow{T(v)} T(M) \xrightarrow{T(w)} T(M'')
$$

*正確です。* (§ 1, no. 3.)

#### 定義 2 {#ac-i-s2-def-2 .statement tag=042N}

*右A-加群 E は、命題 1 と同等の特性を持つ*場合、フラットと呼ばれます。

フラット左A-加群も同様に定義されます。 右A-加群 E がフラットであると言うのは、左の $A^0$ モジュールとみなされ、E がフラットであるというというと同等です。

注意

(1) no. 2 の補題 3 により、右A-加群 E がフラットになるためには、*有限に*生成される A の左イデアル $a$ ごとに、像 E を伴う標準写像 $E \otimes_A a \to E$ (命題 1) が単射であることが必要かつ十分です。

(2) E をフラット右A-加群とします。 $M'$ が左A-加群 M の部分加群である場合、標準単射 $E \otimes_A M' \to E \otimes_A M$ により、$E \otimes_A M$ の部分群で同一視する $E \otimes_A M'$ が可能になります。そこで、N を左A-加群、$u : M \to N$、準同型、$K = \mathrm{Ker}\, u$、$I = \mathrm{Im}\, u$ とします。 完全系列を考慮すると

$$
0 \longrightarrow K \longrightarrow M \xrightarrow{u} N
$$

$E \otimes_A (\mathrm{Ker}\, u)$ が $\mathrm{Ker}(1_E \otimes u)$ と *同一視* されていることは簡単にわかります (命題 1)。一方、$u$と同じグラフで全射準同型 $M \to I$ に対して$u'$、標準単射 $I \to N$, $1_E \otimes u'$ に対して$i$ と書くと全射になります(no. 1, 補題) 1) E がフラットなので、$1_E \otimes i$ は単射です。として

$$
1_E \otimes u = (1_E \otimes i) \circ (1_E \otimes u'),
$$

$E \otimes_A (\mathrm{Im}\, u)$ *は $\mathrm{Im}(1_E \otimes u)$ と同一視されます*。

#### 命題 2 {#ac-i-s2-prop-2 .statement tag=042O}

(i) $(E_t)_{t \in I}$ を右の $A$ モジュールの族とします。 $E = \bigoplus_{t \in I} E_t$ が平坦であるためには、$E_t$ のそれぞれが平坦であることが必要かつ十分です。

(ii) $I$ を、右側の $A$ モジュール (代数、章 II, § 6, no. 2) の順序付けられた集合および $(E_\alpha, f_{\beta \alpha})$ 直接系とします。それぞれの $E_\alpha$ がフラットであれば、$E = \lim_{\longrightarrow} E_\alpha$ もフラットになります。

$M' \to M$ を単射左 $A$ 加群準同型とします。

(i) 直和準同型の場合
$$
\bigoplus_{t \in I} (E_t \otimes_A M') \to \bigoplus_{t \in I} (E_t \otimes_A M)
$$
正確に言えば、準同型 $E_t \otimes_A M' \to E_t \otimes_A M$ のそれぞれがそうであること (代数, 章 II, § 1, no. 6, 系 1 of 命題 7) であることが必要かつ十分であり、$\bigoplus_{t \in I} (E_t \otimes_A M)$ が標準的に識別されるため、(i) が証明されます。 $E \otimes_A M$ (代数、章 II, § 3, no. 7、命題 7)。

(ii) 各数列仮定まで
$$
0 \to E_\alpha \otimes_A M' \to E_\alpha \otimes_A M
$$
正確です。それでは数列です
$$
0 \to E \otimes_A M' \to E \otimes_A M
$$
直接極限を使用すると、テンソル積 (代数、章 II, § 6, no. 3、命題 7) と互換性があり、正確性が保たれます (同上、§ 6, no. 2、命題 3)。

### 4. アパート加群の例

(1) 環 $A$、$A$ は、明らかにフラット $A$ モジュール (代数、章 II, § 3, no. 4、命題 4) です。次に、命題 2、no. 3 の (i) から、すべての自由権 $A$ モジュール、より一般的にはすべての射影権 $A$ モジュール (代数、章 11、§ 2, no. 2) はフラットであることがわかります。 $A$-モジュール。

(2) $A$ が半単純環 (代数, 章 VIII, § 5, no. 1, 定義 1) の場合、右すべての $A$ モジュール $E$ は半単純であるため、単純加群の直和になります。これらの後者のそれぞれは、$A$ の直因子と同型であるため (同上、§ 5, no. 1、命題 6)、$E$ は射影であるため、(1) (cf. 練習問題 16) によって平坦になります。

*(3) In Chapters II and III we shall study in detail two important examples of flat $A$-modules: rings of fractions $S^{-1}A$ and Hausdorff completions $\hat{A}$ of $A$ for $S$-adic topologies.*

#### 命題 3 {#ac-i-s2-prop-3 .statement tag=042P}

$A$ を環 、$E$ を右側の $A$ モジュールとします。

(i) $E$ がフラットであると仮定します。 $0(*)$ の権利因子ではないすべての元 $a \in A$ について、関係 $x \in E,\ xa = 0$ は $x = 0$ を暗示します。

(*) 環 $A$ の 0 の右 (それぞれ左) 因子は元 $b \in A$ であるため、写像 $x \mapsto xb$ (それぞれ $x \mapsto bx$) は単射的ではないことを思い出してください。

(ii) $A$ が整域で、有限に生成されたすべてのイデアルが主であるとします (たとえば、主イデアル整域 (代数, 章 VII, , no. 1))。次に、$E$ が平らであるためには、$E$ にねじれがないことが必要かつ十分です。

(i) を証明します。 $v : A, \to A$ を左側の $A$ モジュール準同型 $t \mapsto ta$ とします。 仮定は、$v$ が単射であることを意味します。 $E$ が平坦であるため、準同型 $1_E \otimes v : E \otimes_A A, \to E \otimes_A A$ も単射です。 $E \otimes_A A$ が正規的に $E$ と同一視されると、$1, \otimes v$ は $E$ の自己準同型 $x \mapsto xa$ になります。したがって、関係 $xa = 0$ は $x = 0$ を意味します。

(ii)を証明します。 (i) により、$E$ が平坦であれば、$E$ はねじれがありません。 逆に、$E$ をねじりのない $A$ モジュールとしましょう。 $A$ の有限生成された理想 $a$ ごとに、標準準同型 $E \otimes_A a \to E$ が単射 (no. 3, 注意 1) であることを検証します。 This assertion is obvious if $a = (0)$; otherwise, by hypothesis $a = Aa$ for some $a \in A, a \neq 0$, and $t \mapsto ta$ is then an isomorphism $v$ of $A$ onto $a$; using $i$ to denote the canonical injection $a \to A$, $i \circ v$ is the homothety with ratio $a$ on $E$ and is injective since $E$ is assumed to be torsion-free. 次に、$1, \otimes (i \circ v) = (1, \otimes i) \circ (1_E \otimes v)$; $1_E \otimes v$ は同型であるため、$1, \otimes i$ は単射法であり、証明が完成します。

#### 例 {#ac-i-s2-n4-exa-1 .statement tag=042Q}

適用命題 3 から環 $\mathbf{Z}$ を見ると、$\mathbf{Q}$ はフラット $\mathbf{Z}$ モジュールですが、$\mathbf{Z}/n\mathbf{Z}$ ($n \geq 2$ の場合) はフラット $\mathbf{Z}$ モジュールではないことがわかります。

### 5. 商加群の平坦度

#### 命題 4 {#ac-i-s2-prop-4 .statement tag=042R}

$E$ を右側の $A$ モジュールとします。次の 3 つのプロパティは同等です。

(a) $E$ はフラットです。
(b) 形の右側の $A$ モジュールのすべての完全系列について

(1)
$$
0 \longrightarrow G \xrightarrow{v} H \xrightarrow{w} E \longrightarrow 0
$$
および左すべての $A$-モジュール $F$、数列

(2)
$$
0 \longrightarrow G \otimes_A F \xrightarrow{v \otimes 1} H \otimes_A F \xrightarrow{w \otimes 1} E \otimes_A F \longrightarrow 0
$$
正確です。

(c) 完全系列 (1) が存在します。ここで、$H$ はフラットであり、数列 (2) は、形 $A_s/a$ のすべての左 $A$ モジュール $F$ に対して正確です。ここで、$a$ は、$A$ の有限生成された左イデアルです。

まず、(a) が (b) を意味することを示します。左側の $A$ モジュール $F$ は、自由加群 (代数、章 II, § 1, no. 11、命題 20) の商と同型です。他の語には完全系列があります

$$
0 \longrightarrow R \xrightarrow{i} L \xrightarrow{p} F \longrightarrow 0
$$

ここで、Lは無料です。 図式を検討してください

$$
\begin{array}{ccccccccc}
G \otimes R & \xrightarrow{v \otimes 1_R} & H \otimes R & \xrightarrow{w \otimes 1_R} & E \otimes R \\
\downarrow l_G \otimes i & & \downarrow l_H \otimes i & & \downarrow l_E \otimes i \\
G \otimes L & \xrightarrow{v \otimes 1_L} & H \otimes L & \xrightarrow{w \otimes 1_L} & E \otimes L \\
\downarrow l_G \otimes p & & \downarrow l_H \otimes p & & \\
G \otimes F & \xrightarrow{v \otimes 1_F} & H \otimes F
\end{array}
$$

(3)

この図式は可換であり、その行と列は no. 1 の補題 1 によって正確であることがすぐにわかります。さらに、$l_G \otimes p$ と $l_H \otimes p$ は全射法 (no. 1, 補題 1) なので、$G \otimes F = \operatorname{Coker}(l_G \otimes i)$ が得られます。

$$
H \otimes F = \operatorname{Coker}(l_H \otimes i);
$$

$w \otimes 1_1$ は全射法 (no. 1, 補題 1);最後に、L は自由でフラットであるため、$v \otimes 1_L$ は単射的です。したがって、ヘビ図式 (§ 1, no. 4, 命題 2, (iii)) は、完全系列の存在を証明するために適用できます。

(4) $$ \operatorname{Ker}(l_H \otimes i) \longrightarrow \operatorname{Ker}(l_E \otimes i) \xrightarrow{d} G \otimes F \xrightarrow{v \otimes 1_F} H \otimes F. $$

そうなると、E がフラットであれば、$l_E \otimes i$ は単射的であり、他の語 $\operatorname{Ker}(l_E \otimes i) = 0$ では、完全系列 (4) は、$v \otimes 1_F$ が単射的であることを示しているため、数列 (2) は正確です (no. 1 の補題 1 を考慮すると)。

(b) は明らかに (c) を意味するので、(c) が (a) を意味することを証明する必要があります。 $\mathbf{R} = \mathbf{a}, \mathbf{L} = \mathbf{A}_s, \mathbf{F} = \mathbf{A}_s/\mathbf{a}$の場合図式(3)を考え、完全系列(4)を当てはめます。 仮定 $v \otimes 1_F$ は単射法であるため、$\operatorname{Im}(d) = 0$;さらに、H は平坦なので、$\operatorname{Ker}(1, @i) = 0$ になります。 数列 (4) の正確性は $\operatorname{Ker}(l_E \otimes i) = 0$ を意味し、他の語、$1, \otimes i$ は単射的であり、これは E がフラット (no. 3, 注意 1) であることを証明します。

#### 命題 5 {#ac-i-s2-prop-5 .statement tag=042S}

*$0 \to E' \xrightarrow{v} E \xrightarrow{w} E'' \to 0$ *右側* $\mathbf{A}$* モジュールの完全系列とします。 * $E''$ * がフラットだと仮定します。次に、* * $E$ * が平らであるためには、* $E'$ * が平らであることが必要かつ十分です。*

$u : F' \to F$ を左の $\mathbf{A}$ モジュールの単射準同型とします。 図式を検討してください

$$
\begin{array}{ccccccccc}
E' \otimes F' & \xrightarrow{v \otimes 1_{F'}} & E \otimes F' & \xrightarrow{w \otimes 1_{F'}} & E'' \otimes F' \\
\downarrow l_{E'} \otimes u & & \downarrow l_E \otimes u & & \downarrow l_{E''} \otimes u \\
E' \otimes F & \xrightarrow{v \otimes 1_F} & E \otimes F & \xrightarrow{w \otimes 1_F} & E'' \otimes F
\end{array}
$$

これは可換であり、その行は正確です (no. 1, 補題 1)。 $E''$ は平坦なので、 l_{E''} \otimes u は単射法です。さらに、命題 4 は v \otimes 1_{F'} と v \otimes 1 が単射であることを証明します。従って、E が平坦な場合、 l_E \otimes u は単射なので、

$$(l_E \otimes u) \circ (v \otimes 1_{F'}) = (v \otimes 1_F) \circ (l_{E'} \otimes u);$$

従って、 l_{E'} \otimes u は単射的であり、その結果 E' はフラットになります。逆に、E' が平坦な場合、 l_{E'} \otimes u は単射です。次に、§ 1, no. 4, 系 1 から命題 2 から l_E \otimes u が単射であるため、E はフラットであることがわかります。

注意
(1) \mathbf{Z} モジュール E = \mathbf{Z}, E' = n\mathbf{Z}, E'' = \mathbf{Z}/n\mathbf{Z} (n \geq 2) の例が示すように、E'' が平坦でなくても E と E' は平坦である可能性があります。
(2) フラット加群の部分加群は、必ずしもフラット加群 (練習問題 3) であるとは限りません。

### 6. 共通部分物件

#### 補題 7 {#ac-i-s2-lem-7 .statement tag=042T}

E を右A-加群、F 左A-加群、および F'、F'' を F の 2 部分加群とし、F = F' + F'' とします。 このとき、E \otimes F の E \otimes F' と E \otimes F'' の標準像の共通部分は、E \otimes (F' \cap F'') の標準像に等しくなります。

図式を検討してください

$$
\begin{array}{ccccccc}
0 & \longrightarrow & F' \cap F'' & \longrightarrow & F' & \longrightarrow & F'/(F' \cap F'') \longrightarrow 0 \\
& & \downarrow & & \downarrow & & \downarrow \\
0 & \longrightarrow & F'' & \longrightarrow & F' + F'' & \longrightarrow & (F' + F'')/F'' \longrightarrow 0
\end{array}
$$

ここで、不特定の矢印は標準単射と全射、および代数、章 I, § 6, no. 13、定理 6 で定義された j 標準同型です。この図式は可換であり、その行は正確です。 (F = F' + F'' なので) 可換図式を導き出します。

$$
\begin{array}{ccc}
E \otimes (F' \cap F'') & \longrightarrow & E \otimes F' \longrightarrow E \otimes (F'/(F' \cap F'')) \\
\downarrow & & \downarrow \\
E \otimes F'' & \longrightarrow & E \otimes F \longrightarrow E \otimes (F/F'')
\end{array}
$$

この図式の行は正確 (no. 1, 補題 1) であり、1 \otimes j は同型です。従って、主張は、§ 1, no. 4、命題 1、(i) (cf. 練習問題 5) の特殊なケースになります。

#### 命題 6 {#ac-i-s2-prop-6 .statement tag=042U}

E が F-フラットになるように、E を右A-加群および F 左A-加群とします。 F のすべての部分加群 F' について、E \otimes F' の標準写像から E \otimes F までの E \otimes F' の \phi(F') 像で表します (これは no. 2 の定義 1 によって単射的です)。次に、F'、F'' が F の 2 つの部分加群である場合、次のようになります。

$$\phi(F' \cap F'') = \phi(F') \cap \phi(F'').$$

EはFフラットなので、$\phi(F' + F'')$は$E \otimes (F' + F'')$と識別され、部分加群、$\phi(F')$、$\phi(F'')$、$\phi(F' \cap F'')$はそれぞれ$E \otimes (F' + F'')$の$E \otimes F'$、$E \otimes F''$、$E \otimes (F' \cap F'')$の標準像と識別されます。 補題 7 からは命題 6 が続きます。

#### 注意 1 {#ac-i-s2-n6-rem-1 .statement tag=042V}

命題 6 の仮説では、$E \otimes_A F'$ は通常、$F$ の部分加群 $F'$ ごとに $\phi(F')$ と識別され、公式が得られます。
$$
E \otimes_A (F' \cap F'') = (E \otimes_A F') \cap (E \otimes_A F'').
$$

#### 命題 7 {#ac-i-s2-prop-7 .statement tag=042W}

※EをEの右A-加群、E'部分加群、FのF左A-加群、F'部分加群とし、E/E'またはF/F'がフラットであるとします。すると、$E \otimes F$の$E' \otimes F'$の標準像は、$E' \otimes F$の標準像の共通部分、$E \otimes F$の$E \otimes F'$になります。

たとえば、$E/E'$ がフラットであると仮定し、図式を検討します。
$$
\begin{array}{ccc}
E' \otimes F' & \longrightarrow & E \otimes F' \\
\downarrow & & \downarrow \\
E' \otimes F & \longrightarrow & E \otimes F
\end{array}
$$
$$
\begin{array}{ccc}
& & (E/E') \otimes F' \\
E \otimes F' & \longrightarrow & (E/E') \otimes F
\end{array}
$$
矢印は標準準同型です。この図式は可換であり、その行は正確です (no. 1, 補題 1)。 $E/E'$ は平坦なので、$u$ は単射法です。このとき、主張は、§ 1, no. 4, 命題 1, (i) の特殊なケースです。

#### 系 {#ac-i-s2-n6-cor-1 .statement tag=042X}

EをEの右A-加群、E'部分加群とします。

(i) ※E/E'はフラットとする。次に、A のすべての左イデアル a について、
$$
E'a = E' \cap Ea.
$$
(ii) *逆に、E が平坦で、A の有限生成された左イデアル a ごとに、関係 (5) が成り立つとします。するとE/E'はフラットになります*。

(i) $F = A$、$F' = a$の場合は命題を適用するで十分です。
(ii) $E/E'$ が平坦であることを証明するには、no. 5 の命題 4 の基準 (c) を適用します。次に、それを確立する必要があります数列
$$
0 \to E'/E'a \to E/Ea \to E/(E' + Ea) \to 0
$$
は、A の有限生成された左イデアル a ごとに、$E'/E'a$ で正確になります。これは、まさに関係 (5) が表すものです。

#### 注意 2 {#ac-i-s2-n6-rem-2 .statement tag=042Y}

$E/E'$ が F-フラットであるか、$F/F'$ が E-フラットであるとのみ仮定する場合、命題 7 の結論は真のままです。

### 7. アパート加群のテンソル積

$A, B$ を 2 つの環、$E$ を右の $A$ モジュール、$F$ を $(A,B)$ の 2 モジュール (*代数*、章 II, § 1, no. 14) とします。 (*代数*, 章 II, § 3, no. 4) $E \otimes_A F$ には正規の権利 $B$ モジュール構造があることを思い出してください。

$$
(x \otimes y)b = x \otimes (yb) \quad \text{for} \quad x \in E,\ y \in F,\ b \in B.
$$

#### 命題 8 {#ac-i-s2-prop-8 .statement tag=042Z}

*$A, B$ を 2 つの環、$E$ を右 $A$ モジュール、$F$ を $(A,B)$ バイモジュールとします。 $E$ がフラットであり、$F$ が $B$ モジュールとしてフラットであるとします。その場合、$B$ モジュール $E \otimes_A F$ はフラットになります。*

$G$ を左の $B$ モジュール、$G$ の $G'$ 部分加群とします。 $F$ は右 $B$ 加群として平坦なので、標準準同型 $F \otimes_B G' \to F \otimes_B G$ は単射です。 $E$は平坦なので、標準準同型

$$
E \otimes_A (F \otimes_B G') \to E \otimes_A (F \otimes_B G)
$$

は単射です。 $E \otimes_A (F \otimes_B G')$ と $E \otimes_A (F \otimes_B G)$ は正規的にそれぞれ $(E \otimes_A F) \otimes_B G'$ と $(E \otimes_A F) \otimes_B G$ (*代数*、章 II, § 3, no. 8、命題 8)、標準準同型として識別されます。

$$
(E \otimes_A F) \otimes_B G' \to (E \otimes_A F) \otimes_B G
$$

は単射であり、$E \otimes_A F$ が平坦な $B$ 加群であることが証明されます。

#### 系 1 {#ac-i-s2-prop-8-cor-1 .statement tag=0430}

$C$ を可換環、$E, F$ 2 つのフラット $C$ モジュールとします。次に、$E \otimes_C F$ はフラットな $C$ モジュールです。

$F$ は $(C, C)$ バイモジュールであり、$B = A = C$ を使用すると命題を適用する 8 に十分です。

#### 系 2 {#ac-i-s2-prop-8-cor-2 .statement tag=0431}

※$\rho$を環$A$～環$B$の準同型とします。 $E$ が平坦な右 $A$ モジュールの場合、スカラーの環を $B$ (*代数*, 章 II, § 5, no. 1) に拡張することによって得られる右 $B$ モジュール $\rho^*(E) = E_{(B)}$ は平坦です。

定義 $E_{(B)} = E \otimes_A B$ により、$B$ は $\rho$ によって $(A,B)$ バイモジュールとみなされます。右側の$B$モジュール$B_d$は平坦なので命題を適用する8で十分です。

#### 系 3 {#ac-i-s2-prop-8-cor-3 .statement tag=0432}

*$R, S$ を 2 つの環と $\phi : R \to S$ 環準同型とします。 $M$ が右フラット $S$ モジュール、$\phi_*(S_d)$ が右フラット $R$ モジュールの場合、$\phi_*(M)$ は右フラット $R$ モジュールです。*

$\phi_*(M)$ は、すべての $x \in M$ とすべての $r \in R$ (*代数*、章 II, § 1, no. 13) に対して、$x.r = x.\phi(r)$ によって定義された正しい $R$ モジュールであることを思い出してください。次に、命題を適用する 8 と $A = S, B = R, E = M$ および $F = S, S$ は、$\phi$ で定義された $(S, R)$-bimodule の構造を持ちます。したがって、右側の $R$ モジュール $M \otimes_S S$ は正確に $\phi_*(M)$ になります。

#### 命題 9 {#ac-i-s2-prop-9 .statement tag=0433}

*$(A_\alpha, f_{\beta\alpha})$ を環の直接系、$A = \lim A_\alpha$ をその直接の極限、$(E_\alpha, f_{\beta\alpha})$ 直接系を同じインデックス集合を持つ右側の $A_\alpha$ モジュールの直接系、$E = \lim E_\alpha$ をその直接の極限とします。これは右側の $A$ モジュール (代数、章 II, § 6, no. 2) です。それぞれの $\alpha$ と $E_\alpha$ がフラット \& モジュールである場合、 $E$ はフラット $A$ モジュールです。*

$E'_\alpha = E_\alpha \otimes_{A_\alpha} A$ とします。ここで、$A$ は、標準準同型 $A_\alpha \to A$ によって左の $A_\alpha$ モジュールと見なされます。右の $A$ 加群 $E$ が $\lim E'_\alpha$ (*上記引用*、系 2 から命題 7) と正準的に同型であることがわかっています。 系 2 から命題 8 に従うと、$E'_\alpha$ はすべての $\alpha$ に対して平坦な右 $A$ 加群であるため、$E$ は no. 3 の命題 2 による平坦な $A$ 加群になります。

### 8. 最終的に提示されました加群

$A$を環とします。 完全系列
$$
L_1 \to L_0 \to E \to 0
$$
左 (右) $A$ モジュール ($L_0$ と $L_1$ は空いている) は、左 (右) $A$ モジュール $E$ の *プレゼンテーション* (または長さ* 1 の *プレゼンテーション) と呼ばれます。

すべての $A$ モジュール $E$ はプレゼンテーションを許可します。実際、私たちは (*代数*、章 II, § 1, no. 11、命題 20) 全射準同型 $u : L_0 \to E$ が存在することを知っています。ここで、$L_0$ は無料です。 $R$ が $u$ の核である場合、同様に全射準同型 $v : L_1 \to R$ が存在し、$L_1$ は空いています。 $v$ を $L_1$ から $L_0$ の準同型とみなした場合、数列 $L_1 \xrightarrow{v} L_0 \xrightarrow{u} 0$ は、定義、よっての主張と正確です。

If $\rho : A \to B$ is a ring homomorphism, every presentation (6) of $E$ induces a presentation of $E_{(B)} = E \otimes_A B$:
$$
L_1 \otimes_A B \to L_0 \otimes_A B \to E \otimes_A B \to 0
$$
by Lemma 1 of no. 1 and the fact that $L \otimes_A B$ is a free $B$-module if $L$ is free.

自由加群 $L_0$ と $L_1$ が有限基底を持つ場合、加群 $E$ の表現 (6) は *有限* と呼ばれます。明らかに、プレゼンテーション (6) が有限であれば、プレゼンテーション (7) も有限です。 $E$ は、有限の提示を許可する場合、*有限提示 $A$-モジュール* と呼ばれます。

#### 補題 8 {#ac-i-s2-lem-8 .statement tag=0434}

(i) *有限のプレゼンテーションを認めるすべての加群は有限に生成されます。*
(ii) *$A$ が左ネーター環の場合、有限に生成されたすべての左 $A$ モジュールは有限のプレゼンテーションを許可します。
(iii) *すべての有限生成射影加群は有限のプレゼンテーションを許可します。*

主張 (i) は定義から自明に続きます。 $A$ が左ネーター で、全射準同型 $u : L_0 \to E$ が存在する場合、$L_0$ は有限基底を持つ自由左$A$ 加群であり、$u$ の核 $R$ が有限に生成されます(*代数*, 章 VIII, , no. 1, 命題 1 および no. 3, 命題 7) したがって、全射準同型 $u : L_1 \to R$ があり、$L_1$ は自由で有限です。 基底、および完全系列 $L_1 \xrightarrow{v} L_0 \xrightarrow{u} E \to 0$ は、$E$ の有限表現です。 よって (ii)

最後に、$E$ が有限生成射影加群であると仮定します。有限生成された自由加群 $L_0$ (*代数*、章 II, §2, no. 2、系 ～ 命題 4) の直因子です。 全射準同型 $L_0 \to E$ の核 $R$ は、$L_0$ の商と同型であるため、有限生成され、(ii) と同様に証明が完成します。

#### 補題 9 {#ac-i-s2-lem-9 .statement tag=0435}

*$A$を環、$E$を有限に提示された$A$モジュールとします。 完全系列* ごとに

$$
0 \longrightarrow F \xrightarrow{j} G \xrightarrow{p} E \longrightarrow 0
$$

*ここで、$G$は有限生成され、加群$F$は有限生成されます。

$L, \xrightarrow{r} L_0 \xrightarrow{s} E \to 0$ を有限のプレゼンテーションとします。 $(e_i)$ が $L_0$ の基底である場合、$i$ 元 $g_i \in G$ には $p(g_i) = s(e_i)$ が存在します。 準同型 $u : L_0 \to G$ は、すべての $i$ に対して $u(e_i) = g_i$ が $s = p \circ u$ を満たすようにします。 $s \circ r = 0$ として、$u(r(L_1)) \subset \mathrm{Ker}\, p$ があり、$\mathrm{Ker}\, p$ が $F$ と同型であるため、図式となるような準同型 $v : L, \to F$ があることがわかります。

$$
\begin{array}{ccccccccc}
L, & \xrightarrow{r} & L_0 & \xrightarrow{s} & E & \longrightarrow & 0 \\
\downarrow v & & \downarrow u & & \downarrow 1_E & & \\
F & \xrightarrow{i} & G & \xrightarrow{p} & E & \longrightarrow & 0
\end{array}
$$

可換です。 $j$ は単射法で、$s$ 全射法なので、ヘビ図式 ($\S$ 1、no. 4、命題 4) を適用できます。他の語には完全系列があります。

$$
0 = \mathrm{Ker}\, 1, \xrightarrow{d} \mathrm{Coker}\, v \longrightarrow \mathrm{Coker}\, u \longrightarrow \mathrm{Coker}\, 1, = 0.
$$

これは、$\mathrm{Coker}\, v$ が仮定によって有限生成される $G / u(L_0)$ と同型であることを示しています。さらに完全系列もあります

$$
0 \to v(L_1) \to F \to \mathrm{Coker}\, v \to 0
$$

そして、$v(L_1)$ と $\mathrm{Coker}\, v$ が有限に生成されるため、$F$ (*代数*、章 II, § 1, no. 7、系 5 ～ 命題 9) も有限に生成されます。

### 9. 準同型加群のスカラーの拡大

$A$ と $B$ を 2 つの環、$E$ を右 $A$ モジュール、$F$ を右 $B$ モジュール、$G$ を $(B, A)$ バイモジュールとします。 $\mathbf{Z}$ モジュールの (代数, 章 II, § 4, no. 2) 標準準同型を定義したことを思い出してください。

$$
\nu : F \otimes_B \operatorname{Hom}_A(E, G) \to \operatorname{Hom}_A(E, F \otimes_B G)
$$

つまり、同盟国 $\in F$ と $u \in \operatorname{Hom}_A(E, G)$ にとって、$\nu(y \otimes u)$ は $A$ 線形マッピング $x \mapsto y \otimes u(x)$ になります。

#### 命題 10 {#ac-i-s2-prop-10 .statement tag=0436}

*$A, B$ を 2 つの環、$E$ を右 $A$ モジュール、$F$ を右 $B$ モジュール、$G$ を $(B, A)$ バイモジュールとします。 $F$ がフラットだとします。次に、$E$ が有限に生成される (それぞれ有限に提示される) 場合、標準準同型 (8) は単射 (または全単射) です。

$A, B, F, G$ を固定として、各右側の $A$-モジュール $E$ 集合を考慮します。

$$
T(E) = F \otimes_B \operatorname{Hom}_A(E, G), \quad T'(E) = \operatorname{Hom}_A(E, F \otimes_B G)
$$

準同型 (8) を $\nu_E$ で表します。すべての右側の $A$ モジュール準同型 $v : E \to E'$、集合 $T(v) = 1, \otimes \operatorname{Hom}(v, 1_G)$ および $T'(v) = \operatorname{Hom}(v, 1, \otimes 1_G)$。 $L, \xrightarrow{v} L_0 \xrightarrow{w} E \to 0$ を $E$ のプレゼンテーションとします。 自由加群 $L_0$ (それぞれ自由加群 $L_0$ と $L_1$) が *有限生成* されると仮定します。 図式

$$
\begin{array}{ccccccccc}
0 & \longrightarrow & T(E) & \xrightarrow{T(w)} & T(L_0) & \xrightarrow{T(v)} & T(L_1) \\
& & \downarrow{\nu_E} & & \downarrow{\nu_{L_0}} & & \downarrow{\nu_{L_1}} \\
0 & \longrightarrow & T'(E) & \xrightarrow{T'(w)} & T'(L_0) & \xrightarrow{T'(v)} & T'(L_1)
\end{array}
$$

は可換であり、2 行目は正確です (代数, 章 II, § 2, no. 1, 定理 1)。さらに、数列

$$
0 \to \operatorname{Hom}_A(E, G) \to \operatorname{Hom}_A(L_0, G) \to \operatorname{Hom}_A(L_1, G)
$$

は正確 (*loc. cit.*) であり、$F$ *平坦* であるため、(9) の最初の行も完全系列 (no. 3, 命題 1) です。次に、$\nu_{L_0}$ (それぞれ $\nu_{L_0}$ と $\nu_{L_1}$) は *全単射* (それぞれ *全単射*) (代数, 章 II, § 4, no. 2, 命題 2) であることがわかります。 $\nu_{L_0}$ が全単射であるとのみ仮定すると、(9) から次のようになります。

$$
\nu_{L_0} \circ T(w) = T'(w) \circ \nu_E
$$

は単射なので、 $\nu_E$ も同様です。 $\nu_{L_0}$ と $\nu_{L_1}$ が両方とも全単射であると仮定すると、§ 1, no. 4、系 2、(ii) から命題 2 まで、$\nu_E$ が全単射であることがわかり、先ほど見たように、$\nu_E$ が単射であることがわかります。

### 10. スカラーの拡大: 可換環の場合

ここで、$A$ を *可換* 環、$B$ 環、$\rho : A \to B$ 環準同型として、$\rho(A)$ が $B$ の *中心* に含まれるようにします。他の語、$\rho$ 定義する、$B$の

A-代数構造。すべての A-加群 E、右B-加群 $E_{(B)} = E \otimes_A B$ は、$\rho_*(B_s)$ および $\rho_*(B_d)$ の $B \otimes_A E$、A-加群構造が仮定によって同一であると識別されます。 A-加群の順序付けされたすべての対 (E, F) について、正準 B 準同型を定義したことを思い出してください。

$$
\omega : (\operatorname{Hom}_A(E, F))_{(B)} \to \operatorname{Hom}_B(E_{(B)}, F_{(B)})
$$

すべての $u \in \operatorname{Hom}_A(E, F)$、$\omega(u \otimes 1) = u \otimes 1_B$ (代数、章 II, § 5, no. 3) についてです。

#### 命題 11 {#ac-i-s2-prop-11 .statement tag=0437}

Aを可換環、Bを環、Aの$\varphi$準同型からBの中心、EとFを2つのA-加群とする。 B がフラット A-加群で、E が有限に生成される (それぞれ有限に提示される) と仮定します。この場合、標準準同型 (10) は単射 (それぞれ全単射) です。

$\omega$ は標準同型で構成されているため

$$
\operatorname{Hom}_A(E, B \otimes_A F) \to \operatorname{Hom}_B(E_{(B)}, F_{(B)})
$$

そして標準準同型 (8)

$$
\nu : B \otimes_A \operatorname{Hom}_A(E, F) \to \operatorname{Hom}_A(E, B \otimes_A F)
$$

(前述)、命題は no. 9 の命題 10 の帰結です。

ここで、A と B が可換であり、3 つの A-加群 $E_1, E_2, E$ と A 双線形写像 $f : E_1 \times E \to E_3$ を考えるとします。すると、次のような B 双線形写像 $f_B : E_{1(B)} \times E_{2(B)} \to E_{3(B)}$ が 1 つだけ存在します。

$$
f_B(1 \otimes x_1, 1 \otimes x_2) = 1 \otimes f(x_1, x_2)
$$

すべての $x_1 \in E_1, x_2 \in E$、(代数、章 IX, § 1, no. 4、命題 1)。

In the statement which follows we shall suppose that B is a flat A-module and, for every submodule E' of $E_i$ ($i = 1, 2, 3$), we shall canonically identify $E'_{(B)}$ with its image in $E_{i(B)}$ (no. 3, Remark 2).

#### 命題 12 {#ac-i-s2-prop-12 .statement tag=0438}

A、B を A から B への可換環、$\varphi$ 準同型、$E_1, E_2, E_3$ 3 A-加群、$f : E_1 \times E \to E_3$ A 双線形写像とします。

$$
f_B : E_{1(B)} \times E_{2(B)} \to E_{3(B)}
$$

拡大です。 $E_2$ の部分加群 $F_2$、$E_3$ の部分加群 $F_3$ を考慮し、それら $x_1 \in E_1$ のうち $E_1$ からなるの部分加群を T で表し、すべてについて $f(x_1, x_2) \in F$ となるようにします。 $x_2 \in F$。 B がフラット A-加群で、$F_2$ が有限生成されるとします。すると、$T_{(B)}$ はそれら $x'_1 \in E_{1(B)}$ のうちの集合となり、すべての $x'_2 \in F_{2(B)}$ に対して $f_B(x'_1, x'_2) \in F_{3(B)}$ になります。

$p$ を標準全射 $E_3 \to E_3/F_3$ とします。それぞれの $x_1 \in E_1$ に $F_2$ から $E_3/F_3$ の A-線型写像 $x_2 \mapsto p(f(x_1, x_2))$ を関連付け、これを $g(x_1)$ で表します。この場合、$g$ は $E_1$ から $\mathrm{Hom}_A(F_2, E_3/F_3)$ の A 準同型であり、$g$ の核は正確に T です。B はフラット A-加群であるため、完全系列が得られます。

$$
0 \longrightarrow T_{(B)} \longrightarrow E_{1(B)} \xrightarrow{1 \otimes g} (\mathrm{Hom}_A(F_2, E_3/F_3))_{(B)}
$$

(no. 3、命題 1)。 命題 11 標準準同型までに

$$
\omega : (\mathrm{Hom}_A(F_2, E_3/F_3))_{(B)} \to \mathrm{Hom}_B(F_{2(B)}, (E_3/F_3)_{(B)})
$$

*単射*です。一方、B はフラット A-加群であるため、$(E_3/F_3)_{(B)}$ は標準的に $E_{3(B)}/F_{3(B)}$ と識別されます。 $\omega$の合成と$1 \otimes g$を組み合わせると、準同型 $u$、つまり数列が得られます。

$$
0 \longrightarrow T_{(B)} \longrightarrow E_{1(B)} \xrightarrow{u} \mathrm{Hom}_B(F_{2(B)}, E_{3(B)}/F_{3(B)})
$$

正確です。 定義からすぐに $u(x'_1)$ が続きます。

$$
x'_1 = 1 \otimes x_1 \in E_{1(B)},
$$

は $x'_2 \in F_{2(B)}$ から類までのそれぞれ写像である線形写像です。 $f_B(x'_1, x'_2)$中$F_{3(B)}$;線形性により、これはすべての $x'_1 \in E_{1(B)}$ にも当てはまります。 $u$の核は$T_{(B)}$なので、命題が証明されます。

#### 系 1 {#ac-i-s2-prop-12-cor-1 .statement tag=0439}

*A、B を 2 つの可換環、$p : A \to B$ 準同型とし、B を平坦 A-加群、E を有限表現 A-加群とします。 E の有限生成されたすべての部分加群 F について、$F_{(B)}$ に直交する $E_{(B)}$ の双対の部分加群は $(F')_{(B)}$ に等しくなります。ここで、$F'$ は F に直交する E の双対 $E^*$ の部分加群です。

命題 11 $(E^*)_{(B)}$ は、$E_{(B)}$ の双対 $(E_{(B)})^*$ と標準的に同型です。その場合、$E_1 = E^*$、$E_2 = E$、$E_3 = A$、$F_2 = F$、$F_3 = \{0\}$、$f$ を$E^* \times E$ の正規の双線形形式で命題を適用する 12 にするだけで十分です。

#### 系 2 {#ac-i-s2-prop-12-cor-2 .statement tag=043A}

*A、B を 2 つの可換環、$p : A \to B$ 準同型として、B がフラット A-加群と E A-加群であるとします。次に、有限に生成される E の部分加群 F ごとに、$F_{(B)}$ の消滅子が B の理想的な $aB$ になります。ここで、a は A の F の消滅子です。*

$E_1 = A$、$E_2 = E_3 = E$、$F_2 = F$、$F_3 = \{0\}$ で命題を適用する 12 で十分です。

#### 注意 {#ac-i-s2-n10-rem-1 .statement tag=043B}

加群 E にも双線形写像 $f$ にも曖昧さがない場合、$F_3 : F_2$ は命題 12 の T で示される加群を示すために使用されるときどきであり、それは F, to F, の *トランスポーター* と呼ばれます。 命題 12 の結論は次のようになります。

$$
F_{3(B)} : F_{2(B)} = (F_3 : F_2)_{(B)}.
$$

$E_i$ が環 $A, f$ が乗法で、$F_i$ 理想値 $a_i$ である特定のケースでは、*トランスポーター式* が得られます。

$$
B(a_3 : a_2) = Ba_3 : Ba_2
$$

$B$ がフラットな $A$ モジュールであり、$a_2$ が有限生成された理想である場合に有効です。

### 11. 関係の項における平坦度の解釈 (*)

この全体を通じて、No. $A$は環、$E$は右側の$A$モジュール、$F$は左側の$A$モジュールを表します。

$E \otimes_A F$ のすべての元は、形で少なくとも 1 つの方法で書くことができます
$$
z = \sum_{i=1}^n e_i \otimes f_i \text{ where } e_i \in E \text{ and } f_i \in F.
$$
次の補題は条件を与え、その下でこの和は零になります。

#### 補題 10 {#ac-i-s2-lem-10 .statement tag=043C}

*$(f_\lambda)_{\lambda \in L}$ *$F$ の生成元の家族、および* $(e_\lambda)_{\lambda \in L}$ *元の* $E$ *有限台の家族とする。 * $\sum_{\lambda \in L} e_\lambda \otimes f_\lambda = 0$ については、 *有限の集合* $J$、 *家族* $(x_j)_{j \in J}$ *of 元 of* $E$ *そして家族* $(a_{j,\lambda})$ *($j \in J, \lambda \in L$) of 元 of* が存在することが必要かつ十分です。 $A$ *次のプロパティ:*

(1) *家族* $(a_{j,\lambda})$ *は有限台;*

(2) $\sum_{\lambda \in L} a_{j,\lambda} f_\lambda = 0$ *全員* $j \in J;$

(3) $e_\lambda = \sum_{j \in J} x_j a_{j,\lambda}$ *全員* $\lambda \in L.$

大まかに言うと、$e_\lambda$の系は、「$f_\lambda$の間の関係」である系の元の$A$の$E$に係数が入った線形結合でなければなりません。

無料の $A$ モジュール $A_s^{(L)}$、その標準基底 $(u_\lambda)$ および準同型 $g : A_s^{(L)} \to F$ が、すべての $\lambda \in L$ に対して $g(u_\lambda) = f_\lambda$ になるように考えてください。 $g$ の $R$ 核で表すと、 ($f_\lambda$ 生成する $F$ 以降) 完全系列になります。

$$
R \xrightarrow{i} A_s^{(L)} \xrightarrow{g} F \longrightarrow 0
$$

ここで、$i$ は標準単射を表します。 no. 1 の補題 1 により、完全系列が導出されます。

$$
E \otimes_A R \xrightarrow{1 \otimes i} E \otimes_A A_s^{(L)} \xrightarrow{1 \otimes g} E \otimes_A F \longrightarrow 0.
$$

(*)このNo.の結果です。 § 3, no. 7 を除き、この章の残りの部分では使用されません。

現在、$E \otimes_A A_s^{(L)}$ は正規的に $E^{(L)}$ と識別され、ファミリー $e = (e_\lambda) \in E^{(L)}$ は $\sum_{\lambda \in L} e_\lambda \otimes u_\lambda$ (*代数*、章 II、 、no. 7、系 1 ～ 命題 7) と識別されます。このような家族が$1_E @ g$の属するから核にするには、$E \otimes_A F$の$\sum_{\lambda \in L} e_\lambda \otimes f_\lambda = 0$が必要十分です。 完全系列 (13) を考慮すると、これは $1, \otimes i$ の $e$ 属するから像がというに相当し、他の語には形の関係が存在します。

$$
\sum_{\lambda \in L} e_\lambda \otimes u_\lambda = \sum_{j \in J} x_j \otimes i(r_j)
$$

ここで、$x_j \in E, r_j \in R$ と $J$ は有限です。 $i(r_j) = \sum_{\lambda \in L} a_{j\lambda} u_\lambda$、仮定 $r_j \in R$ と書くと、すべての $j \in J$ に対して関係 $\sum_{\lambda \in L} a_{j\lambda} f_\lambda = 0$ を意味します。一方、関係 (14) は、すべての $\lambda \in L$ (*代数*、章 II, § 3, no. 7、系 1 ～ 命題 7) に対して $e_\lambda = \sum_{j \in J} x_j a_{j\lambda}$ を意味し、証明が完成します。

#### 命題 13 {#ac-i-s2-prop-13 .statement tag=043D}

*E が F-フラット* (no. 2, *定義 1*) であるためには、*次の条件が満たされることが必要かつ十分です*:

*(R)* *もし* $(e_i)_{i \in I}$ *と* $(f_i)_{i \in I}$ *が、それぞれEとFの元の2つの有限族であり、次のような* $\sum_{i \in I} e_i \otimes f_i = 0$ *in* $E \otimes_A F$, *有限の集合 J、つまり元の族* $(x_j)_{j \in J}$が存在します。 E と A の元の家族* $(a_{ji})$ *($j \in J, i \in I$) で、次の特性* があります:

(1) $\sum_{i \in I} a_{ji} f_i = 0$ *全員* $j \in J$;
(2) $e_i = \sum_{j \in J} x_j a_{ji}$ *全員* $i \in I$。

E が F-フラットであると仮定します。 $(e_i)$ と $(f_i)$ を $E \otimes_A F$ の $\sum_{i \in I} e_i \otimes f_i = 0$ となるような元の有限族とし、$F'$ を *$f_i$ によって生成された F の部分加群とします。 標準写像 $E \otimes_A F' \to E \otimes_A F$ は単射なので、 $\sum_{i \in I} e_i \otimes f_i = 0$ *in* $E \otimes_A F'$ * もあり、補題 10 を E と F' に適用できます。したがって、家族* $(x_j)$ * と* $(a_{ji})$ * は (R)* の満たす条件になります。

逆に、条件 (R) が成り立つとします。 $F'$ を F の部分加群とし、$y = \sum_{i \in I} e_i \otimes f_i$ を標準写像 $E \otimes_A F' \to E \otimes_A F$ の核の元とします。 (R) が成り立つので、家族 $(x_j)$ と $(a_{ji})$ 満たす条件 (1) と (2) が存在します。私たちは結論する、$E \otimes_A F'$には、

$$
y = \sum_{i,j} x_j a_{ji} \otimes f_i = \sum_{j \in J} (x_j \otimes \sum_{i \in I} a_{ji} f_i) = 0.
$$

したがって、$E \otimes_A F' \to E \otimes_A F$ は単射法です。

#### 系 1 {#ac-i-s2-prop-13-cor-1 .statement tag=043E}

右側の $A$ モジュール $E$ が平坦であるためには、次の条件が成立することが必要かつ十分です。

(RP) *If* $(e_i)_{i \in I}$ and $(b_i)_{i \in I}$ are two finite families of elements of $E$ and $A$ respectively such that $\sum e_i b_i = 0$, there exists a finite set $J$, a family $(x_j)_{j \in J}$ of elements of $E$ and a family $(a_{ji})$ ($j \in J, i \in I$) of elements of $A$ such that $\sum a_{ji} b_i = 0$ for all $j \in J$ and $e_i = \sum_{j \in J} x_j a_{ji}$ for all $i \in I$.

条件 (RP) は、命題 13 の条件 (R) を加群 $F = A_s$ に適用したものです。

大まかに言えば、(RP) は次のように述べています: $E$ に係数を含む $b_i$ 間のすべての「関係」は、係数と $b_i$ の間の「関係」の線形結合 ($E$ に係数を含む) です。 $A$。

特に、$A$ から環 $B$ の準同型を考えてみましょう。これにより、$B$ は正しい $A$ 加群になります。 (no. 3、命題 1) は、これが $A$ モジュールがフラットであること、または左すべての $A$ モジュール $A_s^m$ ($m \geqslant 1$) についてフラットであることは、というと同等であることがわかります。 命題 13 の適用条件 (R) に $E = B$ と $F = A_s^m$ を加えると、次の条件が得られます。

#### 系 2 {#ac-i-s2-prop-13-cor-2 .statement tag=043F}

環 $B$ が平らな右$A$ モジュールであるためには、満たす次の条件であることが必要かつ十分です。
(RP') *同次一次方程式の *各解* $(y_k)_{1 \leq k \leq n}$、からなる、元、$B$、系

$$
\sum_{k=1}^n y_k c_{ki} = 0 \quad (1 \leq i \leq m)
$$
*係数* $c_{ki}$ が $A$ の場合、*は線形結合*
$$
y_k = \sum_{j=1}^q b_j z_{jk} \quad (1 \leq k \leq n)
$$
*係数* $b_j \in B$、解 $(z_{jk})_{1 \leq k \leq n}$、系 (15)、からなる、元 $z_{jk}$、$A$。

### 練習問題 {#ac-i-s2-exercises}

[§ 2 に対して練習問題](exercises/s2/)を参照してください。
