---
book: ens
book_title: Theory of Sets
chapter: II
chapter_title: THEORY OF SETS
section: 4
section_title: Union and intersection of a family of sets
lang: ja
source: ens-i-iv
source_edition: 2004, Springer
book_pages: 90-101, 125-126
pdf_pages: 0097-0108, 0132-0133
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF THE UNION AND THE INTERSECTION OF A FAMILY OF SETS
      page: 90
      pdf_page: 97
    - "no": 2
      title: PROPERTIES OF UNION AND INTERSECTION
      page: 93
      pdf_page: 100
    - "no": 3
      title: IMAGES OF A UNION AND AN INTERSECTION
      page: 94
      pdf_page: 101
    - "no": 4
      title: COMPLEMENTS OF UNIONS AND INTERSECTIONS
      page: 96
      pdf_page: 103
    - "no": 5
      title: UNION AND INTERSECTION OF TWO SETS
      page: 96
      pdf_page: 103
    - "no": 6
      title: COVERINGS
      page: 98
      pdf_page: 105
    - "no": 7
      title: PARTITIONS
      page: 99
      pdf_page: 106
    - "no": 8
      title: SUM OF A FAMILY OF SETS
      page: 100
      pdf_page: 107
statements: 22
exercises: 8
content_sha256: 57eef82d3cdba446e128e912b4a55fbbf21a7174d8435e3038be6e6eedcae48f
translated_from: content/en/ens/II/04_s4_union_and_intersection_of_a_family_of.md
translation_method: google
source_content_sha256: 79a8f1cdc57e7dce0167dd11f3e335382fe0479c90c58a053fba7bbc5d06a5f5
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: 0696d7b89d7c1a9798083f95c913cd2794b77bae997e918c88e96ab31953a657
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## 4. 集合人家族の和集合と共通部分

### 1. 集合人家族の和集合の定義と共通部分

X を家族 (§3, no. 4) とし、I をその添字集合とします。以下の内容を直感的に解釈できるように、X を *集合* のファミリーとして参照します。 $(\mathrm{X}, \mathrm{I}, \mathfrak{G})$ が集合* E の部分集合の *ファミリー (つまり、ターゲット $\mathfrak{G}$ が関係 $\mathrm{Y} \in \mathfrak{G}$ が $\mathrm{Y} \subset \mathrm{E}$ を暗示するようなファミリー) である場合、そのファミリーを $(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}(\mathrm{X}_\iota \in \mathfrak{G})$ または単に $(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$ で表すものとします。 (§3, no. 6); 記法の乱用により、Iをその添字集合とする集合の家族を$(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$で表すことにします。

¶ 関係 $(\forall x)((\iota \in \mathrm{I}$ と $x \in \mathrm{X}_\iota) \Rightarrow (x \in \mathrm{X}_\iota))$ が真であるため、S5 (章 I, §4、2 はありません) から、関係が成り立ちます。

$$(\forall \iota)(\exists \mathrm{Z})(\forall x)((\iota \in \mathrm{I} \text{ and } x \in \mathrm{X}_\iota) \Rightarrow (x \in \mathrm{Z}))$$

それは本当です。スキームにより、S8 (§1, no. 6) 関係 $(\exists \iota)(\iota \in \mathrm{I}$ および $x \in \mathrm{X}_\iota)$ は * $x$* に集合します。

#### 定義 1 {#ens-ii-s4-def-1 .statement tag=03I1}

*$(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$ を集合* のファミリー (それぞれ * 集合* E の部分集合のファミリー) とします。 *集合 $\mathscr{E}_x((\exists \iota)(\iota \in \mathrm{I}$ と $x \in \mathrm{X}_\iota))$、つまり、すべての $x$* のうちの集合 * 属するから家族 $(X_l)_{l\in I}$ の少なくとも 1 つの集合を家族の和集合と呼び、* で表します
$$\bigcup_{l\in I}X_l,$$ [^1]

$(X_l)_{l\in I}$ が集合 $E$ の部分集合のファミリーである場合、その和集合は $E$ の部分集合です。 $E$ にも、写像 $l\to X_l$ のターゲット $\mathfrak{G}$ にも依存しないことに注意してください。

$I=\varnothing$ の場合、関係 $(\exists l)(l\in I\text{ and }x\in X_l)$ が偽となるため、$\displaystyle\bigcup_{l\in I}X_l=\varnothing$ があることは明らかです。

¶ 今、$I\neq\varnothing$ だと仮定します。 $\alpha$ が $I$ の元である場合、関係
$$ (\forall l)((l\in I)\Longrightarrow(x\in X_l)) $$
は $x\in X_\alpha$ を意味し、したがって C52 (§1, no. 6) のおかげで、この関係は *$x$ で集合化されます*。

#### 定義 2 {#ens-ii-s4-def-2 .statement tag=03PT}

*$(X_l)_{l\in I}$ を、添字集合 $I$ が空ではない集合の家族とする。 集合 $\mathscr{E}_x((\forall l)((l\in I)\Longrightarrow(x\in X_l)))$、つまり、家族 $(X_l)_{l\in I}$ のすべての集合に属するを加えたすべての $x$ の集合は、家族の共通部分と呼ばれ、* で示されます。
$$\bigcap_{l\in I}X_l.$$

$I=\varnothing$ の場合、関係 $(\forall l)((l\in I)\Longrightarrow(x\in X_l))$ は $x$ で集合化していません。なぜなら、それは真の関係であり、$x\in Y$ が真の関係となるような集合 $Y$ は存在しないからです。なぜなら、$Y$ はすべてのオブジェクト (cf. §1, no. 7, 注意) の集合になるからです。

$(X_l)_{l\in I}$ が集合 $E$ の部分集合の家族で、$I\neq\varnothing$ の場合、関係 「$x\in E$ と $(\forall l)((l\in I)\Longrightarrow(x\in X_l))$」は、
$$ (\forall l)((l\in I)\Longrightarrow(x\in X_l)); $$
その結果、$x$とすべての$x$のうち集合で集団化しており、満たすこの関係は$\displaystyle\bigcap_{l\in I}X_l$に等しい。 $I=\varnothing$ の場合、関係 「$x\in E$ および $(\forall l)((l\in I)\Longrightarrow(x\in X_l))$」は $x\in E$ と同等です。従って、すべての$x$のうち$x$と集合で集団化しており、満たすこの関係は$E$です。従って、次のように言えます定義 :

#### 定義 3 {#ens-ii-s4-def-3 .statement tag=03PU}

*$(X_l)_{l\in I}$を集合$E$の部分集合の家族とします。 集合*
$$\mathscr{E}_x\left(x\in E\text{ and }(\forall l)((l\in I)\Longrightarrow(x\in X_l))\right),$$

*言い換えれば、* E * と各集合* $X_\iota$ に属するすべての $x$ の集合は、 * 族の共通部分と呼ばれ、* $\bigcap\limits_{\iota \in I} X_\iota$ で表されます。

従って、E の部分集合の家族 $(X_\iota)_{\iota \in \emptyset}$ については、次のようになります。

$$\bigcap_{\iota \in \emptyset} X_\iota = E.$$

しかし、添字集合が空ではない E の部分集合の族 $(X_\iota)_{\iota \in I}$ の場合、共通部分 $\bigcap\limits_{\iota \in I} X_\iota$ は E にも $\iota \rightarrow X_\iota$ のターゲットにも依存しません。これにより、定義 2 と 3 で同じ記法を使用することが正当化されます。

#### 命題 1 {#ens-ii-s4-prop-1 .statement tag=03PV}

*$(X_\iota)_{\iota \in I}$ * を集合の家族とし、$f$ を集合* K *上* I の写像とします。 *それから*

$$\bigcup_{\varkappa \in K} X_{f(\varkappa)} = \bigcup_{\iota \in I} X_\iota,$$

*そして、* $I \neq \emptyset$ の場合、

$$\bigcap_{\varkappa \in K} X_{f(\varkappa)} = \bigcap_{\iota \in I} X_\iota.$$

$x$を$\bigcap\limits_{\iota \in I} X_\iota$の元とします。 $x \in X_\iota$ となるような添字 $\iota \in I$ が存在します。 $f\langle K \rangle = I$ 以降、$\iota = f(\varkappa)$、よって $x \in X_{f(\varkappa)}$ となるような添字 $\varkappa \in K$ が存在し、その結果、

$$x \in \bigcup_{\varkappa \in K} X_{f(\varkappa)}.$$

逆に、$x \in \bigcup\limits_{\varkappa \in K} X_{f(\varkappa)}$ の場合、$x \in X_{f(\varkappa)}$ となるような $\varkappa \in K$ が存在するため、$f(\varkappa) \in I$ 以降、$x \in \bigcup\limits_{\iota \in I} X_\iota$ となります。従って、

$$\bigcup_{\varkappa \in K} X_{f(\varkappa)} = \bigcup_{\iota \in I} X_\iota.$$

¶ ここで、$I \neq \emptyset$ を仮定し、$x$ を $\bigcap\limits_{\iota \in I} X_\iota$ の元とします。 K の各元 $\varkappa$ には $f(\varkappa) \in I$ があり、従って $x \in X_{f(\varkappa)}$ があり、従って

$$x \in \bigcap_{\varkappa \in K} X_{f(\varkappa)}.$$

逆に、$x$を$\bigcap\limits_{\varkappa \in K} X_{f(\varkappa)}$の元とします。 $\iota$ が I のいずれかの元である場合、$\iota = f(\varkappa)$、よって $x \in X_\iota$、そして結果として $x \in \bigcap_{\iota \in I} X_\iota$ となるような K の元 $\varkappa$ が存在します。従って、

$$\bigcap_{\varkappa \in K} X_{f(\varkappa)} = \bigcap_{\iota \in I} X_\iota.$$

特定の集合の部分集合のファミリーの場合、命題 1 の 2 番目の部分が制限 $I \neq \emptyset$ なしで有効なままであることは明らかです。

#### 系 {#ens-ii-s4-n1-cor-1 .statement tag=03I2}

*$(X_\iota)_{\iota \in I}$ *添字* $(\iota, \varkappa)$ の各対に対して * $X_\iota = X_\varkappa$ となるような集合の家族としましょう。 *それぞれについて* $\alpha \in I$ *私たちは*

$$\bigcup_{\iota \in I} X_\iota = X_\alpha, \qquad \textit{and (if } I \neq \emptyset) \qquad \bigcap_{\iota \in I} X_\iota = X_\alpha.$$

命題を適用する 1 を I の定数写像 $\iota \to \alpha$ を$\{\alpha\}$ に代入します。

#### 定義 4 {#ens-ii-s4-def-4 .statement tag=03I3}

* $\mathfrak{F}$ * を集合の集合とし、* $\Phi$ * を * $\mathfrak{F}$ の恒等写像によって定義される集合のファミリーとします。 *和集合 of 集合 of* $\Phi$ *および (* $\mathfrak{F}$ *が空でない場合) 共通部分 of 集合 of* $\Phi$ *は、それぞれ* 和集合 *および* 共通部分 *of 集合 of* $\mathfrak{F}$、*およびは* $\bigcup_{X \in \mathfrak{F}} X$ *および* $\bigcap_{X \in \mathfrak{F}} X$ で表されます。

命題 1 からすぐに、$(X_\iota)_{\iota \in I}$ が集合のファミリーである場合、そのファミリーの和集合および ($I \neq \emptyset$ の場合) 共通部分は、それぞれ、集合の集合の和集合および共通部分に等しいことがわかります。この家族の元。

### 2. 和集合と共通部分のプロパティ

$(X_\iota)_{\iota \in I}$ と $(Y_\iota)_{\iota \in I}$ が同じ添字集合 I を持つ集合の家族であり、それぞれの $\iota \in I$ に $Y_\iota \subset X_\iota$ がある場合、次のことが明らかです。

$$\bigcup_{\iota \in I} Y_\iota \subset \bigcup_{\iota \in I} X_\iota, \qquad \text{and (if } I \neq \emptyset) \qquad \bigcap_{\iota \in I} Y_\iota \subset \bigcap_{\iota \in I} X_\iota.$$

¶ $(X_\iota)_{\iota \in I}$ を集合の家族とします。 $J \subset I$ の場合、

$$\bigcup_{\iota \in J} X_\iota \subset \bigcup_{\iota \in I} X_\iota, \qquad \text{and (if } J \neq \emptyset) \qquad \bigcap_{\iota \in J} X_\iota \supset \bigcap_{\iota \in I} X_\iota.$$

#### 命題 2 {#ens-ii-s4-prop-2 .statement tag=03I4}

*$(X_\iota)_{\iota \in I}$ *を集合の集合とし、そのインデックス集合* I *は集合の集合* $(J_\lambda)_{\lambda \in L}$ *の和集合です。 それから*

$$\bigcup_{\iota \in I} X_\iota = \bigcup_{\lambda \in L} \left( \bigcup_{\iota \in J_\lambda} X_\iota \right),$$

*および* (*場合* $L \neq \emptyset$ と $J_\lambda \neq \emptyset$ *それぞれ* $\lambda \in L$)

$$\bigcap_{\iota \in I} X_\iota = \bigcap_{\lambda \in L} \left( \bigcap_{\iota \in J_\lambda} X_\iota \right)$$

(和集合と共通部分の「結合性」)。

$x$を$\bigcup_{\iota \in I} X_\iota$の元とします。 $x \in X_\iota$ となるような添字 $\iota \in I$ が存在します。 I は家族 $(J_\lambda)_{\lambda \in L}$ の和集合であるため、$\iota \in J_\lambda$、よって $x \in \bigcup_{\iota \in J_\lambda} X_\iota$ のような添字 $\lambda \in L$ が存在し、その結果、

$$x \in \bigcup_{\lambda \in L} \left( \bigcup_{\iota \in J_\lambda} X_\iota \right).$$

逆に、$x$をこの集合の元とします。 $x \in \bigcup_{\iota \in J_\lambda} X_\iota$ となる添字 $\lambda \in L$ が存在するため、$x \in X_\iota$ となる添字 $\iota \in J_\lambda$ (従って $\iota \in I$) が存在します。それは次のとおりです

$$x \in \bigcup_{\iota \in I} X_\iota.$$

ここで、$\lambda \in L$ ごとに $L \neq \emptyset$ と $J_\lambda \neq \emptyset$ があるとします。次に$I \neq \emptyset$。 $x$を$\bigcap_{\iota \in I} X_\iota$の元とします。 $\lambda \in L$ の場合、$\iota \in J_\lambda$ ($J_\lambda \subset I$ 以降)、よって $x \in \bigcap_{\iota \in J_\lambda} X_\iota$ ごとに $x \in X_\iota$ が得られます。最後の包含はすべての$\lambda \in L$、$x$、属するから$\bigcap_{\lambda \in L} \left( \bigcap_{\iota \in J_\lambda} X_\iota \right)$に当てはまります。逆に、$x$ を後者の集合の元とし、$\iota$ を I の任意の元とします。 $\iota \in J_\lambda$ となるような $\lambda \in L$ が存在します。 $x \in \bigcap_{\iota \in J_\lambda} X_\iota$ 以降、$x \in X_\iota$ があり、これはすべての $\iota \in I$ に当てはまります。従って$x \in \bigcap_{\iota \in I} X_\iota$です。これで証明は完了です。

特定の集合の部分集合のファミリーの場合、命題 2 の 2 番目の部分は、L と $J_\lambda$ の制限なしで有効のままです。

### 3. 和集合と共通部分の像

#### 命題 3 {#ens-ii-s4-prop-3 .statement tag=03I5}

*$(X_\iota)_{\iota \in I}$ *を集合* A の部分集合の家族とし、*そして * $\Gamma$ * A * と* B の間の対応とします。 *その後*

$$\Gamma \left\langle \bigcup_{\iota \in I} X_\iota \right\rangle = \bigcup_{\iota \in I} \Gamma \langle X_\iota \rangle, \qquad \Gamma \left\langle \bigcap_{\iota \in I} X_\iota \right\rangle \subset \bigcap_{\iota \in I} \Gamma \langle X_\iota \rangle.$$

関係 $(\exists x)\left(x \in \bigcup_{\iota \in I} X_\iota \text{ and } y \in \Gamma(x)\right)$ は以下と同等です

$$(\exists x)(\exists \iota)(\iota \in I \text{ and } x \in X_\iota \text{ and } y \in \Gamma(x)),$$

従って、$(\exists \iota)(\iota \in I$ と $y \in \Gamma\langle X_\iota \rangle)$ は、$y \in \bigcup_{\iota \in I} \Gamma\langle X_\iota \rangle$ に相当します。これは最初の公式を証明します。 2 番目の公式については、$\iota \in I$、よって (§3、命題 2) がすべて $\bigcap_{\iota \in I} X_\iota \subset X_\iota$ になります。

$$\Gamma\left\langle \bigcap_{\iota \in I} X_\iota \right\rangle \subset \Gamma\langle X_\iota \rangle,$$

そしてその結果として

$$\Gamma\left\langle \bigcap_{\iota \in I} X_\iota \right\rangle \subset \bigcap_{\iota \in I} \Gamma\langle X_\iota \rangle.$$

¶ $\Gamma$ が任意の対応 (特に任意の写像) の場合、公式

$$\Gamma\left\langle \bigcap_{\iota \in I} X_\iota \right\rangle = \bigcap_{\iota \in I} \Gamma\langle X_\iota \rangle$$

通常は *false* です。

\* たとえば、平面 $\mathbf{R}^2$ では、線 $y = x$ と $y = x + 1$ の最初の射影は $\mathbf{R}$ に等しいですが、これらの線の共通部分は空であるため、この共通部分 [^2] の最初の射影も同様です。 \*

ただし、次の重要な結果が得られました。

#### 命題 4 {#ens-ii-s4-prop-4 .statement tag=03I6}

*$f$を* A *into* Bの写像とし、* $(Y_\iota)_{\iota \in I}$ *を* Bの部分集合の家族とする。 *その後* $\overset{-1}{f}\left\langle \bigcap_{\iota \in I} Y_\iota \right\rangle = \bigcap_{\iota \in I} \overset{-1}{f}\langle Y_\iota \rangle.$

これを証明するには、$x$ を $\bigcap_{\iota \in I} \overset{-1}{f}\langle Y_\iota \rangle$ の元とします。すべての $\iota \in I$、よって $f(x) \in \bigcap_{\iota \in I} Y_\iota$ に対して $f(x) \in Y_\iota$ があり、従って

$$x \in \overset{-1}{f}\left\langle \bigcap_{\iota \in I} Y_\iota \right\rangle.$$

従って、$\bigcap_{\iota \in I} \overset{-1}{f}(Y_\iota) \subset \overset{-1}{f}\left\langle \bigcap_{\iota \in I} Y_\iota \right\rangle$;この関係と命題 3 が結果を与えます。

#### 系 {#ens-ii-s4-n3-cor-1 .statement tag=03I7}

*$f$ が * A *into* B の単射であり、* $(X_\iota)_{\iota \in I}$ * が * A の部分集合の族である場合 * その添字集合* I *が空でない場合、* $f\left\langle \bigcap_{\iota \in I} X_\iota \right\rangle = \bigcap_{\iota \in I} f\langle X_\iota \rangle$。

なぜなら、$f = i \circ g$、ここで$i$は$f\langle A \rangle$の標準単射をBに、$g$はAの全単射を$f\langle A \rangle$に書くことができるからです。 $h$ が $g$ の逆数写像を表す場合、A のすべての部分集合 X に対して $f\langle X \rangle = \overset{-1}{h}\langle X \rangle$ が得られるため、命題 4 に戻されます。

### 4. 和集合と共通部分の補数

#### 命題 5 {#ens-ii-s4-prop-5 .statement tag=03I8}

*すべての家族に* $(X_\iota)_{\iota \in I}$ *of 部分集合 of 集合* E、*私たちは*を持っています

$$\complement_E\left(\bigcup_{\iota \in I} X_\iota\right) = \bigcap_{\iota \in I} (\complement_E X_\iota), \qquad \complement_E\left(\bigcap_{\iota \in I} X_\iota\right) = \bigcup_{\iota \in I} (\complement_E X_\iota).$$

$x \in \complement_E\left(\bigcup_{\iota \in I} X_\iota\right)$ にしましょう。次に $x \in E$、そして $\iota \in I$ ごとに $x \notin X_\iota$ となり、$x \in \complement_E X_\iota$ になります。その結果

$$x \in \bigcap_{\iota \in I} (\complement_E X_\iota).$$

逆に、$x$ を $\bigcap_{\iota \in I} (\complement_E X_\iota)$ の元とします。 共通部分中定義までに$x \in E$ができました。さらに、$x \in \bigcup_{\iota \in I} X_\iota$ がある場合、$x \in X_\varkappa$ となる添字 $\varkappa \in I$ が存在し、矛盾するの仮説 $x \in \bigcap_{\iota \in I} (\complement_E X_\iota)$ が存在します。従って

$$x \in \complement_E\left(\bigcup_{\iota \in I} X_\iota\right).$$

これは最初の公式を証明します。 2 番目は、E の部分集合 X ごとに関係 $\complement_E(\complement_E X) = X$ を考慮すると、明らか帰結です。

### 5. 2 つの集合のうち和集合と共通部分

A、B が集合の場合、次のように書きます。

$$A \cup B = \bigcup_{X \in \{A, B\}} X, \qquad A \cap B = \bigcap_{X \in \{A, B\}} X.$$

$A \cup B$ は、$A$ または $B$ (あるいは両方) に属するするすべてのオブジェクトの集合であり、$A \cap B$ は、$A$ と $B$ の両方に属するするすべてのオブジェクトの集合であることは明らかです。特に$\{x, y\} = \{x\} \cup \{y\}$。

¶ $\{x, y, z\} = \{x, y\} \cup \{z\}$ とします。 集合 $\{x, y, z\}$ は集合で、その元は $x$、$y$、$z$ だけです。同様に、次のように書きます

$$\{x, y, z, t\} = \{x, y, z\} \cup \{t\},$$

等々。

¶ 今、$A$、$B$、$C$、$D$ が集合である場合、次のように書きます。

$$A \cup B \cup C = \bigcup_{X \in \{A,\, B,\, C\}} X, \qquad A \cap B \cap C = \bigcap_{X \in \{A,\, B,\, C\}} X;$$

$$A \cup B \cup C \cup D = \bigcup_{X \in \{A,\, B,\, C,\, D\}} X, \qquad A \cap B \cap C \cap D = \bigcap_{X \in \{A,\, B,\, C,\, D\}} X;$$

等々。

¶ $A, B, C$ を集合とします。 命題 1 と 2 から公式を導き出します。

$$A \cup B = B \cup A, \qquad A \cap B = B \cap A,$$
$$A \cup (B \cup C) = (A \cup B) \cup C = A \cup B \cup C,$$
$$A \cap (B \cap C) = (A \cap B) \cap C = A \cap B \cap C.$$

これらの式は、基準 C24 (章 I, §3, no. 5) で明示される明らか帰結または定理でもあります。同様に公式を証明します

$$A \cup (B \cap C) = (A \cup B) \cap (A \cup C), \qquad A \cap (B \cup C) = (A \cap B) \cup (A \cap C)$$

(共通部分に対する和集合および和集合に対する共通部分の「分配性」; cf. §5, no. 6)。

¶ 関係 $A \subset B$ は、$A \cup B = B$ および $A \cap B = A$ と同等です。 $A$ と $B$ が集合 $E$ の部分集合である場合、命題 5 (または基準 C24) から次の式を導き出します。

$$\complement_E(A \cup B) = (\complement_E A) \cap (\complement_E B), \qquad \complement_E(A \cap B) = (\complement_E A) \cup (\complement_E B);$$

さらに、私たちは

$$A \cup (\complement_E A) = E, \qquad A \cap (\complement_E A) = \emptyset.$$

¶ $\Gamma$ が $E$ と $F$ の間の対応であり、$A$、$B$ が $E$ の部分集合である場合、命題 3 から次のようになります。

$$\Gamma\langle A \cup B \rangle = \Gamma\langle A \rangle \cup \Gamma\langle B \rangle, \qquad \Gamma\langle A \cap B \rangle \subset \Gamma\langle A \rangle \cap \Gamma\langle B \rangle,$$

そして、$f$ が F から E への写像である場合、

$$\overset{-1}{f}\langle \mathrm{A} \cap \mathrm{B} \rangle = \overset{-1}{f}\langle \mathrm{A} \rangle \cap \overset{-1}{f}\langle \mathrm{B} \rangle$$

命題から 4.

¶ 補足として次の命題も記録します。

#### 命題 6 {#ens-ii-s4-prop-6 .statement tag=03PW}

*$f$を* Aの*から* Bへの写像とします。 *Bの*すべての部分集合* Yについて、*次のようになります*

$$\overset{-1}{f}\langle \mathrm{B} - \mathrm{Y} \rangle = \overset{-1}{f}\langle \mathrm{B} \rangle - \overset{-1}{f}\langle \mathrm{Y} \rangle.$$

$x$ 属するから $\overset{-1}{f}\langle \mathrm{B} - \mathrm{Y} \rangle$ については、$f(x)$ 属するが Y にはではなく B に移行する場合に限ります。つまり、$x$ 属するから $\overset{-1}{f}\ \langle \mathrm{B} \rangle$ に移行するが、$\overset{-1}{f}\ \langle \mathrm{Y} \rangle$ には移行しない場合に限ります。

#### 系 {#ens-ii-s4-n5-cor-1 .statement tag=03PX}

*$f$ を * A の単射を B に * 入れます。 * A の * 部分集合* X ごとに、 * $f\langle \mathrm{A} - \mathrm{X} \rangle = f\langle \mathrm{A} \rangle - f\langle \mathrm{X} \rangle$ になります。

$i$が$f\langle \mathrm{A} \rangle$の標準単射である$f = i \circ g$をBに書くと、簡約する系から命題6が$\overset{-1}{g}$に適用されます。

¶ 共通部分 $\mathrm{X} \cap \mathrm{A}$ は、A 上の X の *トレース* と呼ばれるときどきです。 $\mathfrak{F}$ が集合のファミリーである場合、集合所属 ～ $\mathfrak{F}$ の A 上のトレースの集合は A 上の $\mathfrak{F}$ の *トレース* と呼ばれます。

### 6. カバーリング

#### 定義 5 {#ens-ii-s4-def-5 .statement tag=03PY}

*集合 $(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$ のファミリーは、集合* E *(またはカバー* E) *$\mathrm{E} \subset \bigcup\limits_{\iota \in \mathrm{I}} \mathrm{X}_\iota$ の場合、カバーであると言われます。 $(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$ と $(\mathrm{Y}_\varkappa)_{\varkappa \in \mathrm{K}}$ が * E の覆いである場合、* それぞれの $\varkappa \in \mathrm{K}$ に対して次のような $\iota \in \mathrm{I}$ が存在する場合、*これらの覆いの 2 番目は最初の覆いよりもより細かいであると言われます (または最初の改良である、または最初の改良であると言えます)。

$$\mathrm{Y}_\varkappa \subset \mathrm{X}_\iota.$$

集合 $\mathfrak{R}$ の集合は、$\mathfrak{R}$ の恒等写像で定義される集合のファミリーが E のカバーである場合、語は、$\mathrm{E} \subset \bigcup\limits_{\mathrm{X} \in \mathfrak{R}} \mathrm{X}$ の場合、E のカバーです。

$\mathfrak{R}$、$\mathfrak{R}'$、$\mathfrak{R}''$ が、$\mathfrak{R}'$ が $\mathfrak{R}$ をリファインし、$\mathfrak{R}''$ が $\mathfrak{R}'$ をリファインするような E の 3 つのカバーである場合、$\mathfrak{R}''$ が $\mathfrak{R}$ をリファインすることは明らかです。

$(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$ を E のカバーとします。J が I の部分集合で、$(\mathrm{X}_\iota)_{\iota \in \mathrm{J}}$ がまだ E のカバーである場合、このカバーは明らかに $(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$ を洗練します。

¶ $(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$ と $(\mathrm{Y}_\varkappa)_{\varkappa \in \mathrm{K}}$ を集合 E のカバーとする。 すると、集合 $(\mathrm{X}_\iota \cap \mathrm{Y}_\varkappa)_{(\iota, \varkappa) \in \mathrm{I} \times \mathrm{K}}$ のファミリーは E のカバーになります。 $x \in \mathrm{E}$ の場合、$x \in \mathrm{X}_\iota$ と $x \in \mathrm{Y}_\varkappa$ のような添字 $\iota \in \mathrm{I}$ と $\varkappa \in \mathrm{K}$ が存在するため、$x \in \mathrm{X}_\iota \cap \mathrm{Y}_\varkappa$ さらに、カバー$(\mathrm{X}_\iota \cap \mathrm{Y}_\varkappa)_{(\iota, \varkappa) \in \mathrm{I} \times \mathrm{K}}$ がカバー$(X_\iota)_{\iota \in I}$、$(Y_\varkappa)_{\varkappa \in K}$ のそれぞれを洗練していることは明らかです。 逆に、$(Z_\lambda)_{\lambda \in L}$ を、各カバー $(X_\iota)_{\iota \in I}$、$(Y_\varkappa)_{\varkappa \in K}$ を洗練する E のカバーとします。 $\lambda \in L$ の場合、$Z_\lambda \subset X_\iota$ と $Z_\lambda \subset Y_\varkappa$ のように添字 $\iota \in I$ と $\varkappa \in K$ が存在するため、$Z_\lambda \subset X_\iota \cap Y_\varkappa$ になります。したがって、カバー$(Z_\lambda)_{\lambda \in L}$は、

$$(X_\iota \cap Y_\varkappa)_{(\iota, \varkappa) \in I \times K}.$$

¶ $(X_\iota)_{\iota \in I}$ を集合 A のカバーとし、$f$ を A の写像と *onto* 集合 B とします。ファミリー $(f\langle X_\iota \rangle)_{\iota \in I}$ は B (命題 3) のカバーであり、* $f$ * の下の *像と呼ばれます。カバー* $(X_\iota)_{\iota \in I}$。 $g$ が集合 C の写像から集合 A である場合、ファミリー $(\overset{-1}{g}\langle X_\iota \rangle)_{\iota \in I}$ は C のカバーであり、*$g$ *カバー* $(X_\iota)_{\iota \in I}$ の下*逆像と呼ばれます。
¶ E と F を集合、$(X_\iota)_{\iota \in I}$ を E のカバー、$(Y_\varkappa)_{\varkappa \in K}$ を F のカバーとする。すると、ファミリー $(X_\iota \times Y_\varkappa)_{(\iota, \varkappa) \in I \times K}$ は $E \times F$ のカバーとなり、E のカバー $(X_\iota)_{\iota \in I}$ と F の $(Y_\varkappa)_{\varkappa \in K}$ の *積* と呼ばれる。

#### 命題 7 {#ens-ii-s4-prop-7 .statement tag=03PZ}

(1) *E を集合および* $(X_\iota)_{\iota \in I}$ *E を *カバーする* とする。 *もし* $f$ *と* $g$ *が 2 つの写像でドメイン* E *が * $f$ * と* $g$ *同意* $E \cap X_\iota$ *それぞれについて* $\iota \in I$、*その後* $f$ *そして* $g$ *同意* E.

(2) *$(X_\iota)_{\iota \in I}$ * を集合の族とし、* $(f_\iota)_{\iota \in I}$ * を同じターゲットを持つ写像の族とする * F *それぞれについて* $\iota \in I$ * $f_\iota$ * のドメインが * $X_\iota$、* およびそれぞれの対* $(\iota, \varkappa) \in I \times I$、$f_\iota$ *そして* $f_\varkappa$ *同意* $X_\iota \cap X_\varkappa$。 *その場合、*ドメイン* $A = \bigcup_{\iota \in I} X_\iota$ *およびターゲット* F *を持つ写像* $f$ *それぞれ写像* $f_\iota$ $(i \in I)$ 拡大するが 1 つだけ存在します。

(1) $x$ を E の任意の元とします。すると、$x \in X_\iota$, よって $f(x) = g(x)$ by 仮定となるような $\iota \in I$ が存在します。
(2) $f_\iota$ のグラフを$G_\iota$ とし、$G = \bigcup_{\iota \in I} G_\iota$ とします。 G が関数グラフであることを示しましょう。 $(x, y) \in G$と$(x, y') \in G$の場合、Iには$(x, y) \in G_\iota$と$(x, y') \in G_\varkappa$のように、添字$\iota$、$\varkappa$が2つ存在します。これは、$x \in X_\iota$、$x \in X_\varkappa$、$y = f_\iota(x)$、$y' = f_\varkappa(x)$ を意味します。しかし、$x \in X_\iota \cap X_\varkappa$ 以降、私たちは

$$f_\iota(x) = f_\varkappa(x),$$

つまり、$y = y'$です。グラフ G のドメインは $\mathrm{pr}_1 G = \bigcup_{\iota \in I} \mathrm{pr}_1 G_\iota = A$ です。したがって、写像 $f = (G, A, F)$ は必要な条件を満たします。その一意性は、命題の最初の部分に続きます。

### 7. 分割

#### 定義 6 {#ens-ii-s4-def-6 .statement tag=03Q0}

*2 つの集合* A * と* B *は、*$A \cap B = \emptyset$ の場合、互いに素* (*交差しない*) と言われます。 *もし* $A \cap B \neq \emptyset$ なら、*A が B に *出会っている* (*または交差*) と *言います。 *$(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$ *を集合の家族にしましょう。この家族の集合は、条件* $\iota \in \mathrm{I}$、$\varkappa \in \mathrm{I}$、$\iota \neq \varkappa$ *暗黙* $\mathrm{X}_\iota \cap \mathrm{X}_\varkappa = \emptyset$ の場合、相互に互いに素であると言われます。

$f$ を A の写像を B に変換し、$(\mathrm{Y}_\iota)_{\iota \in \mathrm{I}}$ を B の相互互いに素部分集合のファミリーとします。 命題 4 は、A の部分集合のファミリー $(\overset{-1}{f}\langle \mathrm{Y}_\iota \rangle)_{\iota \in \mathrm{I}}$ の集合が相互に一致することを示します。 互いに素。一方、$(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$がAの相互互いに素部分集合の家族である場合、家族$(f \langle \mathrm{X}_\iota \rangle)_{\iota \in \mathrm{I}}$の集合は一般に相互に互いに素ではありません。

#### 命題 8 {#ens-ii-s4-prop-8 .statement tag=03Q1}

*$(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$ * を相互に互いに素集合の族とし、* $(f_\iota)_{\iota \in \mathrm{I}}$ * を同じターゲット* F を持つ写像の族とする * $f_\iota$ * の定義域が * $\mathrm{X}_\iota$ * それぞれ* $\iota \in \mathrm{I}$ であるようにします。 *すると、ドメイン* $\bigcup_{\iota \in \mathrm{I}} \mathrm{X}_\iota$ * とターゲット* F * それぞれ写像* $f_\iota$ $(\iota \in \mathrm{I})$ の拡大するを持つ写像 f が 1 つだけ存在します。

$f_\iota$ と $f_\varkappa$ は $\iota \neq \varkappa$ のときはいつでも $\mathrm{X}_\iota \cap \mathrm{X}_\varkappa = \emptyset$ に明確に一致するため、これは命題 7 の系です。

#### 定義 7 {#ens-ii-s4-def-7 .statement tag=03Q2}

*集合* E の *分割は、 *E を *カバーする* E の * 空ではない * 相互に互いに素部分集合の族です。

#### 例 {#ens-ii-s4-n7-exa-1 .statement tag=03I9}

空ではないすべての集合 A に対して、ファミリー $(\{x\})_{x \in \mathrm{A}}$ は A の分割です。

$(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$ が集合 E の分割である場合、集合元の $\mathfrak{F}$ に分割の $\mathrm{X}_\iota$ をI の写像 $\iota \rightarrow \mathrm{X}_\iota$ は次のようになります。全単射。したがって、$\mathfrak{F}$が与えられた場合、添字集合の間で対応までは分割が決まります。通常、私たちが分割について話すとき、私たちが関心を持つのは元の分割の集合です。

### 8. 集合の家族の和

#### 命題 9 {#ens-ii-s4-prop-9 .statement tag=03Q3}

*$(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$ *集合の家族としましょう。次に、 集合* X *次の性質* が存在します: X * 和集合は家族です* $(\mathrm{X}'_\iota)_{\iota \in \mathrm{I}}$ * 相互に互いに素集合であるため、それぞれ* $\iota \in \mathrm{I}$ * が存在します1 対 1 写像の* $\mathrm{X}_\iota$ *対* $\mathrm{X}'_\iota$。

$\mathrm{A} = \bigcup_{\iota \in \mathrm{I}} \mathrm{X}_\iota$ にしましょう。 $\iota \in \mathrm{I}$ の場合、写像 $x \rightarrow (x, \iota)$ $(x \in \mathrm{X}_\iota)$ は、$\mathrm{X}_\iota$ の写像と $\mathrm{A} \times \mathrm{I}$ の部分集合 $\mathrm{X}'_\iota$ に対する 1 対 1 です。さらに、$\mathrm{A} \times \mathrm{I}$ の 2 番目の座標写像の下にある $\mathrm{X}'_\iota$ の像は集合 $\{\iota\}$ に含まれます。 $\iota \neq \varkappa$ のときはいつでも $\mathrm{X}'_\iota \cap \mathrm{X}'_\varkappa = \emptyset$ ということになります。その場合は$\mathrm{X} = \bigcup_{\iota \in \mathrm{I}} \mathrm{X}'_\iota$を取る可能性があります。

#### 定義 8 {#ens-ii-s4-def-8 .statement tag=03Q4}

*$(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$ *集合の家族にしましょう。この家族の和は、集合* $(\mathrm{X}_\iota \times \{\iota\})_{\iota \in \mathrm{I}}$ の家族の和集合です。

#### 命題 10 {#ens-ii-s4-prop-10 .statement tag=03IA}

*$(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$ *お互いに互いに素集合の家族になりましょう。 * A * を和集合とし、* S * を和とします。そのとき、* A *onto* S の全単射写像が存在します。

それぞれの $\iota \in \mathrm{I}$ について、$f_\iota$ を $\mathrm{X}_\iota$ の全単射を $\mathrm{X}_\iota \times \{\iota\}$ に加えます。 命題 8 により、A の写像 $f$ が S に存在し、拡大するすべての写像 $f_\iota$ が存在します。 $f$ が A から S への全単射写像であることがすぐに検証されます。

言語の乱用により、定義 8 で定義されているように、和の上に E の全単射が存在する場合、集合 E は集合 $(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$ の家族の *和* であると言われます。

$(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$ が集合の任意の族である場合、命題 10 の引数は、和 S *onto* 和集合 A の写像が存在することを示していることに注意してください。

### 練習問題 {#ens-ii-s4-exercises}

[§ 4 に対して練習問題](exercises/s4/)を参照してください。

[^1]: したがって、スキーム S8 では、これらの集合が同じ集合の部分集合 (*結果の概要* で与えられた和集合の定義で作成された仮定である) と*先験的に仮定することなく、集合の族の定義する和集合を計算することができます。 §4, no. 2）。
[^2]: この公式の適用から生じる有名なエラーは、H. ルベーグは、平面上のボレル集合の軸上の射影が再びボレル集合であることを証明しようとしました (この主張は後に誤りであることが示され、それが引き起こした議論は「スーリン」集合の理論の起源でした) : ルベーグは次のように主張しました。 集合の減少列の共通部分の射影は、射影の共通部分に等しい (*Journal de Mathématiques*、(6) **1** (1905)、pp. 191-192)。
