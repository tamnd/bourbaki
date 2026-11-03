---
book: alg
book_title: Algebra
chapter: II
chapter_title: LINEAR ALGEBRA
section: 2
section_title: Modules of linear mappings. Duality
lang: ja
source: alg-i-iii
source_edition: 1998, Springer
book_pages: 227-243, 386-395
pdf_pages: 0251-0267, 0410-0419
extraction: ocr
subsections:
    - "no": 1
      title: PROPERTIES OF $\mathrm{Hom}_A(E, F)$ RELATIVE TO EXACT SEQUENCES
      page: 227
      pdf_page: 251
    - "no": 2
      title: PROJECTIVE MODULES
      page: 231
      pdf_page: 255
    - "no": 3
      title: LINEAR FORMS; DUAL OF A MODULE
      page: 232
      pdf_page: 256
    - "no": 4
      title: ORTHOGONALITY
      page: 234
      pdf_page: 258
    - "no": 5
      title: TRANSPOSE OF A LINEAR MAPPING
      page: 234
      pdf_page: 258
    - "no": 6
      title: DUAL OF A QUOTIENT MODULE. DUAL OF A DIRECT SUM. DUAL BASES
      page: 236
      pdf_page: 260
    - "no": 7
      title: BIDUAL
      page: 239
      pdf_page: 263
    - "no": 8
      title: LINEAR EQUATIONS
      page: 240
      pdf_page: 264
statements: 42
exercises: 26
content_sha256: 3bb2888b4facfbc0ea08608f76a6ab17b2ac189bc6458c1049606433e6404f8c
translated_from: content/en/alg/II/02_s2_modules_of_linear_mappings_duality.md
translation_method: google
source_content_sha256: b68d6b666aad78a9fe6c8ac80cb610da120336ed9a4c3178da2cb94e6cf08597
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: e33fc50fd8a2d7095cf14666ae3dc38447ad1e520d1050838f5090898095a9dd
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## § 2。 線形写像の加群。二元性

### 1. 完全系列に対する$\mathrm{Hom}_A(E, F)$の特性

#### 定理 1 {#alg-ii-s2-thm-1 .statement tag=05MV}

*A を環、E'、E、E'' を 3 つ A-加群、u : E' \to E、v : E \to E'' を 2 つ準同型とします。 数列*の場合

$$
\text{(1)} \quad E' \xrightarrow{u} E \xrightarrow{v} E'' \longrightarrow 0
$$

*正確には、A-加群 F ごとに、数列* であることが必要かつ十分です

$$
\text{(2)} \quad 0 \longrightarrow \mathrm{Hom}(E'', F) \xrightarrow{\bar{v}} \mathrm{Hom}(E, F) \xrightarrow{\bar{u}} \mathrm{Hom}(E', F)
$$

($\bar{u} = \mathrm{Hom}(u, 1_F)$、$\bar{v} = \mathrm{Hom}(v, 1_F)$) *正確にしてください*。

数列 (1) が正確であると仮定します。 $w \in \mathrm{Hom}(E'', F)$ と $\bar{v}(w) = w \circ v = 0$ の場合、$v$ は全射なので $w = 0$ になります。したがって、数列 (2) は $\mathrm{Hom}(E'', F)$ で正確です。 $\mathrm{Hom}(E, F)$ で正確であることがわかります。 $\bar{u} \circ \bar{v} = \mathrm{Hom}(v \circ u, 1_F)$ (§ 1, no. 2, 公式 (10)) および $v \circ u = 0$ は、数列 (1) が E で正確であるためです。したがって、$\bar{u} \circ \bar{v} = 0$、つまり $\mathrm{Im}(\bar{v}) \subset \mathrm{Ker}(\bar{u})$ です。一方、$w \in \mathrm{Ker}(\bar{u})$ の場合は、$w \circ u = 0$、したがって $\mathrm{Ker}(w) \supset \mathrm{Im}(u)$ となります。しかし、数列 (1) は E で正確であるため、$\mathrm{Im}(u) = \mathrm{Ker}(v)$、したがって $\mathrm{Ker}(w) \supset \mathrm{Ker}(v)$ になります。 $v$ は全射なので、§ 1, no. 3, *注意* から、w = w' \circ v = \bar{v}(w') となる $w' \in \mathrm{Hom}(E'', F)$ が存在することがわかります。したがって、Ker(\bar{u}) \部分集合 \operatorname{Im}(\bar{v}) となり、数列 (2) が正確であるという証明が​​完成します。

逆に、(2) がすべての A-加群 F に対して正確であるとします。すべての準同型 $w : E'' \to F$ に対して $\bar{u} \circ \bar{v} = \operatorname{Hom}(v \circ u, 1_F) = 0, w \circ v \circ u = 0$ と同じです。 $F = E''$ と $w = 1_{E''}$ を考慮すると、まず $v \circ u = 0$ 、つまり $u(E') \subset \operatorname{Ker}(v)$ がわかります。ここで、$F = \operatorname{Coker}(u)$ をとり、$\phi : E \to F = E/u(E')$ を標準写像とします。すると、定義による$\bar{u}(\phi) = \phi \circ u = 0$となり、$\phi = \bar{v}(\psi) = \psi \circ v$となるような$\psi \in \operatorname{Hom}(E'', F)$が存在します。これは明らかに $u(E') = \operatorname{Ker}(\phi) \supset \operatorname{Ker}(v)$ を意味しており、数列 (1) が E で正確であることが証明されます。最後に、$\theta$ を $F = E''/v(E)$ 上の $E''$ の標準準同型とします。次に $\bar{v}(\theta) = \theta \circ v = 0$、したがって $\theta = 0$;したがって、$F = \{0\}$ と $v$ は全射です。したがって、数列 (1) は $E''$ で正確です。

#### 系 {#alg-ii-s2-n1-cor-1 .statement tag=05MW}

*A-線型写像* $u : E \to F$ *全射法であること* (それぞれ *全単射*、それぞれ *零*)、 *すべての A-加群 G、写像* $\operatorname{Hom}(u, 1_G) : \operatorname{Hom}(F, G) \to \operatorname{Hom}(E, G)$ *単射法であること* (それぞれ *全単射*、それぞれ *零*) であることが必要かつ十分です。 *零*)。

$E'' = \{0\}$ (それぞれ $E' = \{0\}$ それぞれ $E'' = E$ と $v = 1_E$) の場合には、定理を適用する 1 で十分です。

完全系列から始まることに注意してください

$$
0 \longrightarrow E' \xrightarrow{u} E \xrightarrow{v} E'' \longrightarrow 0
$$

対応する数列

$$
0 \longrightarrow \operatorname{Hom}(E'', F) \xrightarrow{\bar{v}} \operatorname{Hom}(E, F) \xrightarrow{\bar{u}} \operatorname{Hom}(E', F) \longrightarrow 0
$$

*必ずしも正確であるとは限りません*、他の語、準同型 $\bar{u}$ は必ずしも全射ではありません。 $E'$ が E の部分加群と同一視される場合、これは、$E'$ の F できないの線形写像が常に E の F への線形写像に拡張されることを意味します (練習問題 11 および 12)。ただし:

#### 命題 1 {#alg-ii-s2-prop-1 .statement tag=05MX}

*線形写像の完全系列の場合*

(3)
$$
0 \longrightarrow E' \xrightarrow{u} E \xrightarrow{v} E'' \longrightarrow 0
$$

*分裂* (他の語では、$u(E')$ が E の *直因子* である場合) *数列*

(4)
$$
0 \longrightarrow \operatorname{Hom}(E'', F) \xrightarrow{\bar{v}} \operatorname{Hom}(E, F) \xrightarrow{\bar{u}} \operatorname{Hom}(E', F) \longrightarrow 0
$$

* は正確であり、分裂* です。 *逆に、すべての A-加群 F について、数列 (4) が正確である場合、数列 (3) 分裂* となります。

完全系列 (3) 分裂の場合、$u$ (§ 1, no. 9, 命題 15) に関連する線形後退 $u' : E \to E'$ が存在します。もし

$$
\bar{u}' = \operatorname{Hom}(u', 1_F) : \operatorname{Hom}(E', F) \to \operatorname{Hom}(E, F),
$$

$u' \circ u$ が同一性であるという事実は、$\bar{u} \circ \bar{u}'$ が同一性 ($§ 1$、no. 2、公式 (10)) であることを意味し、したがって最初の主張は $§ 1$、no. 9、命題 15 から続きます。 数列 (4) は $F = E'$ と完全に一致します。そして、$f \circ u = 1_{E'}$となるような元$f \in \mathrm{Hom}(E, E')$が存在し、$§ 1$、no. 9、命題15から結論が導き出されます。

命題 1 の最初の主張は、$§ 1$、no. 6、系 1 から命題 6 までの特殊なケースとみなされ、$\mathbf{Z}$ 線形マッピングによって $\mathrm{Hom}(E', F) \oplus \mathrm{Hom}(E'', F)$ と $\mathrm{Hom}(E' \oplus E'', F)$ が正規に識別されることに注意してください。 $\mathrm{Hom}(p', 1_F) + \mathrm{Hom}(p'', 1_F)$、$p': E' \oplus E'' \to E'$ と $p'': E' \oplus E'' \to E''$ は正規の射影です。

#### 定理 2 {#alg-ii-s2-thm-2 .statement tag=05MY}

*$A$を環、$F', F, F''$を3つの$A$モジュール、$u: F' \to F, v: F \to F''$を2つの準同型とします。 数列*用

$$
0 \longrightarrow F' \xrightarrow{v} F \xrightarrow{u} F''
$$

*正確に言うと、すべての $A$ モジュール $E$、数列* に対して必要かつ十分です

$$
0 \longrightarrow \mathrm{Hom}(E, F') \xrightarrow{\bar{u}} \mathrm{Hom}(E, F) \xrightarrow{\bar{v}} \mathrm{Hom}(E, F'')
$$

*($\bar{u} = \mathrm{Hom}(1_E, u), \bar{v} = \mathrm{Hom}(1_E, v)$) は正確に入力してください。*

数列 (5) が正確であると仮定します。 注意まずそれ

$$
\bar{v} \circ \bar{u} = \mathrm{Hom}(1_E, v \circ u) = 0
$$

(II、$§ 1$、no. 2、公式 (10)) $v \circ u = 0$ 以降。 したがって、$\bar{u}$ の $\mathrm{Hom}(E, F')$ のイメージは、$\bar{v}$ のカーネル $N$ に含まれます。 $f$ を、グラフが $\bar{u}$ のグラフと等しい $\mathbf{Z}$ 加群 $\mathrm{Hom}(E, F')$ から $N$ への準同型性とする。 $f$ が *全単射* であることを証明する必要があり、したがって、$f \circ g$ と $g \circ f$ が恒等マッピングとなるようなマッピング $g: N \to \mathrm{Hom}(E, F')$ を定義する必要があります。 この場合、$w$ を $N$ の元、つまり $v \circ w = 0$ となるように線形写像 $w: E \to F$ とします。 後者の関係は、仮定による$w(E) \subset \mathrm{Ker}(v) = u(F')$と等価です。したがって、$u$は単射であるため、$w = u \circ w'$となる線形写像$w': E \to F'$が1つだけ存在し、$g(w) = w'$がとられます。 $g$ が望ましい条件を満たすことがすぐに検証されます。

逆に、数列 (6) がすべての $A$ モジュール $E$ に対して正確であると仮定します。 $\mathrm{Hom}(1_E, v \circ u) = \bar{v} \circ \bar{u} = 0$ の場合、準同型 $w: E \to F'$ ごとに $v \circ u \circ w = 0$ となります。 $E = F'$ と $w = 1_{F'}$ を考慮すると、まず $v \circ u = 0$ 、つまり $u(F') \subset \mathrm{Ker}(v)$ がわかります。ここで、$E = \mathrm{Ker}(v)$ をとり、$\phi: E \to F$ を標準単射とします。次に、$\bar{v}(\phi) = v \circ \phi = 0$ by 定義となり、$\phi = \bar{u}(\psi) = u \circ \psi$ となるような$\psi \in \mathrm{Hom}(E, F')$ が存在します。これは明らかに$\mathrm{Ker}(v) \subset u(F')$ を暗示し、$F$ で (5) の正確性の証明が完成します。最後に、$\theta$ が $\mathrm{Ker}\, u$ の恒等写像である場合、$\bar{u}(\theta) = 0$、したがって $\theta = 0$ と $\mathrm{Ker}\, u = \{0\}$ となり、$F'$ における (5) の正確性が証明されます。

#### 注意 {#alg-ii-s2-n1-rem-1 .statement tag=05MZ}

(1) 定理 2 により、F のすべての部分加群 F' に対して、Hom(E, F) のサブ$\mathbf{Z}$ モジュールを使用して同一視する Hom(E, F') が可能になります。この識別が行われると、すべての家族について、F の部分加群の $(M_\lambda)$

$$
\operatorname{Hom}(E, \bigcap_\lambda M_\lambda) = \bigcap_\lambda \operatorname{Hom}(E, M_\lambda)
$$

たとえば、それぞれの $\operatorname{Hom}(E, M_\lambda)$ に $u \in \operatorname{Hom}(E, F)$ 属するを入力すると、すべての $x \in E$、$u(x) \in M_\lambda$ がすべての $\lambda$ となり、したがって $u$ 写像 E は $\bigcap_\lambda M_\lambda$ になります。

#### 系 {#alg-ii-s2-n1-cor-2 .statement tag=05N0}

*A-線型写像* $u : E \to F$ *単射法であるためには、すべての A-加群 G について、写像* $\operatorname{Hom}(1_G, u) : \operatorname{Hom}(G, E) \to \operatorname{Hom}(G, F)$ *単射法であることが必要かつ十分です。

$F' = \{0\}$の場合は定理を適用する 2で十分です。

完全系列から

$$
0 \longrightarrow F' \xrightarrow{u} F \xrightarrow{v} F'' \longrightarrow 0
$$

対応する数列

$$
0 \longrightarrow \operatorname{Hom}(E, F') \xrightarrow{\bar{u}} \operatorname{Hom}(E, F) \xrightarrow{\bar{v}} \operatorname{Hom}(E, F'') \longrightarrow 0
$$

*必ずしも正確であるとは限りません*、他の語 $\bar{v}$ は必ずしも全射的ではありません。 $F'$が$F$の部分加群と同一視され、$F''$が商加群$F/F'$と同一視される場合、$E$の$F''$への線形写像は必ずしも形$v \circ w$のものではないことを意味します。ここで、$w$ は $E$ の線形写像を $F$ に変換したものです。ただし:

#### 命題 2 {#alg-ii-s2-prop-2 .statement tag=05N1}

*完全系列の場合*

(7)

$$
0 \longrightarrow F' \xrightarrow{u} F \xrightarrow{v} F'' \longrightarrow 0
$$

*分裂* (他の語では、$u(F')$ が $F$ の *直因子* の場合)、*数列*

(8)

$$
0 \longrightarrow \operatorname{Hom}(E, F') \xrightarrow{\bar{u}} \operatorname{Hom}(E, F) \xrightarrow{\bar{v}} \operatorname{Hom}(E, F'') \longrightarrow 0
$$

* は正確で分裂* です。 *逆に、数列* (8) * がすべての A-加群 E に対して正確である場合、完全系列* (7) *分裂* となります。

最初の主張は、次の事実から導かれます。

$$
\operatorname{Hom}(E, F') \oplus \operatorname{Hom}(E, F'')
$$

は、$\mathbf{Z}$ 線形マッピング $\operatorname{Hom}(1_E, j') + \operatorname{Hom}(1_E, j''), j' : F' \to F' \oplus F''$ および $j'' : F'' \to F' \oplus F''$ が標準単射 (§ 1, no. 6、系 1 ～ 命題 6) であることにより、$\operatorname{Hom}(E, F' \oplus F'')$ と正規的に識別されます。逆に、数列 (8) が $E = F''$ に対して正確である場合、$v \circ g = 1_{F''}$ となる元 $g \in \operatorname{Hom}(F'', F)$ が存在し、§ 1, no. 9、命題 15 から結論が得られます。

注意 (2)。このNo.の結果です。は、演算子を使用したすべての可換群に対して変更なしで有効です。

### 2. 射影加群

#### 定義 1 {#alg-ii-s2-def-1 .statement tag=05N2}

A-加群 P は、A-線型写像、数列のすべての完全系列 F' → F → F'' について、射影と呼ばれます。

$$
\operatorname{Hom}(P, F') \to \operatorname{Hom}(P, F) \to \operatorname{Hom}(P, F'')
$$

正確です。

#### 命題 3 {#alg-ii-s2-prop-3 .statement tag=05N3}

部分加群 (M_i) の族の A-加群 P、直和が射影であるためには、各 M_i が射影であることが必要かつ十分です。

A-加群準同型 u : E → F ごとに、

$$
\operatorname{Hom}(1_P, u) : \operatorname{Hom}(P, E) \to \operatorname{Hom}(P, F)
$$

$\prod_i \operatorname{Hom}(1_{M_i}, u)$ (§ 1, no. 6、系 1 ～ 命題 6) で識別されます。したがって、定義 1 および § 1, no. 5、命題 5 (ii) から結論が得られます。

#### 系 {#alg-ii-s2-n2-cor-1 .statement tag=05N4}

すべての自由A-加群は射影的です。

A_s が射影であることを示すには、命題 3 によって十分であり、これは § 1, no. 14 の図式 (50) の可換性の直後に続きます。

#### 命題 4 {#alg-ii-s2-prop-4 .statement tag=05N5}

P を A-加群とします。次のプロパティは同等です。

(a) P は射影です。
(b) A-線型写像、数列の完全系列 0 → F' → F → F'' → 0ごとに

$$
0 \to \operatorname{Hom}(P, F') \to \operatorname{Hom}(P, F) \to \operatorname{Hom}(P, F'') \to 0
$$

正確です。

(c) すべての全射法 A-加群準同型 u : E → E'' およびすべての準同型 f : P → E'' に対して、 f = u ∘ g となるような準同型 g : P → E が存在します (f は P から E への準同型に「リフト」できると言われています)。

(d) A-線型写像分裂のすべての完全系列 0 → E' → E → P → 0 (したがって、P は E の直因子と同型です)。

(e) P は自由A-加群の直因子と同型です。

(a) が (b) を意味することは自明です。 (b) が (c) を暗示していることを確認するには、(b) を完全系列 0 → E' → E → E'' → 0 に適用するだけで十分です。ここで、(c) は次の事実を表しているため、E' = Ker(u) です。

$$
\operatorname{Hom}(1_P, u) : \operatorname{Hom}(P, E) \to \operatorname{Hom}(P, E'')
$$

全主観的です。 (c) が (d) を意味していることを確認するには、(c) を全射準同型 $v : E \to P$ と準同型 $l_P : P \to P$ に適用するだけで十分です。 $l_P = v \circ g$ が数列を意味するような準同型 $g : P \to E$ の存在

$$
0 \longrightarrow E' \longrightarrow E \xrightarrow{v} P \longrightarrow 0
$$

分裂 (§ 1, no. 9、命題 15)。すべての A-加群 M には、自由A-加群 L と完全系列 $0 \to R \to L \to M \to 0$ (§ 1, no. 11、命題 20) が存在し、明らかに (d) は (e) を意味します。最後に (e) は、命題 3 とその系によって (a) を意味します。

#### 系 1 {#alg-ii-s2-prop-4-cor-1 .statement tag=05N6}

*A-加群が射影的で有限に生成されるためには、それが有限の基底を持つ自由A-加群の直因子であることが必要かつ十分です。

条件で十分なのは明らかです。逆に、有限生成射影加群 E は有限基底 (§ 1, no. 11) を持つ自由加群 F の商と同型であり、命題 4 (d) により E は F の直因子と同型です。

#### 系 2 {#alg-ii-s2-prop-4-cor-2 .statement tag=05N7}

*C を可換環とし、E、F を 2 つの有限生成射影 C 加群とする。この場合、$\operatorname{Hom}_C(E, F)$ は有限生成された射影 C モジュールです。*

It may be assumed that there are two finitely generated free C-modules M, N such that $M = E \oplus E', N = F \oplus F'$; it follows from § 1, no. 6, Corollary 1 to Proposition 6 that $\operatorname{Hom}_C(M, N)$ is finitely generated and free and on the other hand that $\operatorname{Hom}_C(M, N)$ is isomorphic to

$$
\operatorname{Hom}_C(E, F) \oplus \operatorname{Hom}_C(E', F) \oplus \operatorname{Hom}_C(E, F') \oplus \operatorname{Hom}(E', F'),
$$

よって系。

### 3. 線型形式; 加群の双対

E を *left* A-加群とします。 A は (A, A)-bimodule であるため、$\operatorname{Hom}_A(E, A_s)$ は正規の *right* A-加群構造 (§ 1, no. 14) を持ちます。

#### 定義 2 {#alg-ii-s2-def-2 .statement tag=05N8}

*すべての右A-加群 E について、右A-加群 $\operatorname{Hom}_A(E, A_s)$ は E* の双対加群 (または単に E の *双対†*) と呼ばれ、*その元は E* 上の線型形式と呼ばれます。

E が *right* A-加群である場合、集合 $\operatorname{Hom}_A(E, A_d)$ とその標準 *left* A-加群構造は同様に E の *dual* と呼ばれ、その元は E 上の *線型形式* と呼ばれます。

† *トポロジカルベクトル空間*、IV では、ベクトル空間に対して、「デュアル空間」の *位相*、概念を定義するとします。これは、この位相に依存し、ここで定義されたものとは異なります。 読者は、この段落で確立されている「代数的」双対の性質を、「位相的」双対空間に対して不注意に適用注意しなければなりません。

この章では、$E^*$ は (左または右) A-加群 $E$ の双対を表すために使用されます。

#### 例 {#alg-ii-s2-n3-exa-1 .statement tag=05N9}

*$\mathbf{R}$の区間$[a, b]$における連続実数値写像のベクトル空間(体$\mathbf{R}$に関して)では、写像$x \mapsto \int_a^b x(t) dt$は線型形式です。

$E$ を左A-加群とし、$E^*$ をその双対とします。注文されたすべての元 $x \in E, x^* \in E^*$、元 $x^*(x)$ の対は、$\langle x, x^* \rangle$ で表されます。それでは関係

$$
\begin{align*}
(9) \quad & \langle x + y, x^* \rangle = \langle x, x^* \rangle + \langle y, x^* \rangle \\
(10) \quad & \langle x, x^* + y^* \rangle = \langle x, x^* \rangle + \langle x, y^* \rangle \\
(11) \quad & \langle \alpha x, x^* \rangle = \alpha \langle x, x^* \rangle \\
(12) \quad & \langle x, x^* \alpha \rangle = \langle x, x^* \rangle \alpha
\end{align*}
$$

$x, y$、$E, x^*, y^*$、$E^*$、$\alpha \in A$を押し続けます。 $E \times E^*$ の $A$ への写像 $(x, x^*) \mapsto \langle x, x^* \rangle$ は、$E \times E^*$ の正規の双線形形式と呼ばれます (双線形形式の概念は一般的に IX, § 1 で定義されます)。 $E$ のすべての線型形式 $x^*$ は、正規の双線形形式に対する部分的な写像 $x \mapsto \langle x, x^* \rangle$ 対応すると考えることができます。

$E$が右A-加群のとき、元$x \in E$における線型形式$x^* \in E^*$の値$x^*(x)$を$\langle x^*, x \rangle$で表し、対応する～(11)、(12)の式は次のように書けます。

$$
\begin{align*}
\langle x^*, x \alpha \rangle &= \langle x^*, x \rangle \alpha \\
\langle \alpha x^*, x \rangle &= \alpha \langle x^*, x \rangle.
\end{align*}
$$

A が可換である場合、記法のいずれかが許容されます。

#### 命題 5 {#alg-ii-s2-prop-5 .statement tag=05NA}

すべての環 A、写像は、$A_s$ のすべての $\xi \in A$ 線型形式 $\eta \mapsto \eta \xi$ と関連付けられており、$A_s$ の双対上の $A_d$ の同型です。

これは、§ 1, no. 14、注意 2、対応するから $E = A_s$ の標準同型 $E \to \mathrm{Hom}_A(A_s, E)$ の特別なケースです。 § 1, no. 14の図式(50)の可換性は、ここに右A-加群の同型があることを示しています。

$A_d$ が命題 5 の同型によって $A_s$ の双対と識別される場合、$A_s \times A_d$ の正規の双線形形式は次のように表されます。

$$
\langle \xi, \xi^* \rangle = \xi \xi^* \quad \text{for } \xi, \xi^* \text{ in } A.
$$

同様に、$A_d$ の双対は正規的に $A_s$ と識別され、$A_d \times A_s$ 上の正規の双線形形式は次のように表現されます。

$$
\langle \xi^*, \xi \rangle = \xi^* \xi \quad \text{for } \xi, \xi^* \text{ in } A.
$$

### 4. 直交性

#### 定義 3 {#alg-ii-s2-def-3 .statement tag=05NB}

E を A-加群とし、E* を双対とします。 ⟨x, x*⟩ = 0 の場合、元 x ∈ E および元 x* ∈ E* は直交と呼ばれます。

すべての x ∈ M、x* ∈ M'、x と x* が直交する場合、E の部分集合 M と E* の部分集合 M' は直交集合と呼ばれます。特に、x* ∈ E* (それぞれ x ∈ E) は、M (それぞれ M') のすべての元に直交する場合、M (それぞれ M') に直交していると呼ばれます。 x* と y* が M に直交する場合、(10) と (12) (no. 3) により、すべての α ∈ A に対して x* + y* と x*α も直交し、次の定義が正当化されます。

#### 定義 4 {#alg-ii-s2-def-4 .statement tag=05NC}

E の部分集合 M (または E* の部分集合 M') が与えられると、M (または M') に直交する x* ∈ E* の集合 (または x ∈ E の集合) は、M (または M') に完全に直交する部分加群と呼ばれます (または単に部分加群は、混乱が生じない限り M (それぞれ M') に直交します)。

線型形式の定義により、Eに直交するE*の部分加群は0になります。 {0} に直交する E* の部分加群は E* と同一です。

#### 命題 6 {#alg-ii-s2-prop-6 .statement tag=05ND}

M、N を、M ⊂ N となる E の 2 つの部分集合とする。 M' と N' がそれぞれ M と N に直交する E* の部分加群である場合、N' ⊂ M' です。

#### 命題 7 {#alg-ii-s2-prop-7 .statement tag=05NE}

(M_i) を E の部分集合の家族とする。 M_i の和集合に直交する部分加群は、それぞれ M_i に直交する部分加群 M'_i の共通部分です。この部分加群は、M_iの和集合によって生成されたEの部分加群とも直交する部分加群です。

これらの結果は、明らか帰結/定義です。

E* の部分集合に直交する E の部分加群には、類似した命題 (これについては読者に述べてもらいます) があります。

M が E の部分加群、M に直交する E* の M' 部分加群、M' に直交する E の M'' 部分加群であれば、M ⊂ M'' ですが、M ≠ M'' (練習問題 9) である可能性があります。 注意ただし、M'' が E* の M'' の直交である場合、M'' = M' になります。 M' ⊂ M'' の場合、一方で関係 M ⊂ M'' は M'' ⊂ M' を意味します。

### 5. 線形写像中転置

E、F を 2 左A-加群とします。すべての線形写像 u : E → F に対して、写像 Hom(u, l_{A_s}) は、右A-加群 F* の線形写像を右A-加群 E* (§ 1, no. 2) に変換し、u の転置と呼ばれます。

その他語:

#### 定義 5 {#alg-ii-s2-def-5 .statement tag=05NF}

A-加群 E の A-加群 F へのすべての線形写像 u について、F の双対 F* から E の双対 E* への線形写像 y* ↦ y* ∘ u は、u の転置と呼ばれ、t u で表されます。

したがって、転置 $^t u$ は関係によって定義されます
(15) $$
\langle u(x), y^* \rangle = \langle x, ^t u(y^*) \rangle \quad \text{for all } x \in E \text{ and all } y^* \in F^*.
$$

定義 5 は変更せずに右A-加群に適用され、関係と同等になります
$$
\langle y^*, u(x) \rangle = \langle ^t u(y^*), x \rangle \quad \text{for all } x \in E \text{ and all } y^* \in F^*.
$$

ここで§ 1, no. 2の式(9)と(10)は次のようになります。
(16) $$
^t(u_1 + u_2) = ^t u_1 + ^t u_2
$$
2 つの元 $u_1, u_2$ の $\mathrm{Hom}_A(E, F)$ と
(17) $$
^t(v \circ u) = ^t u \circ ^t v
$$
$u \in \mathrm{Hom}_A(E, F)$ と $v \in \mathrm{Hom}_A(F, G)$ の場合、G は 3 番目の A-加群です。最後に、はっきりと
(18) $$
^t 1_E = 1_{E^*}.
$$

#### 注意 {#alg-ii-s2-n5-rem-1 .statement tag=05NG}

(17) と (18) から、$u$ が左 (または右) 可逆である場合、$^t u$ は右 (または左) 可逆であることがわかります。

#### 命題 8 {#alg-ii-s2-prop-8 .statement tag=05NH}

*$u : E \to F$をA-線型写像、EのM部分加群、$E^*$におけるMの直交$M'$とする。 $F^*$ の $u(M)$ の直交は逆像 $^t u^{-1}(M')$ です。*

これは (15) の直後に続きます。

#### 系 {#alg-ii-s2-n5-cor-1 .statement tag=05NI}

*$F^*$の像$u(E)$の直交は、$^t u$の核$^t u^{-1}(0)$です。*

$E^*$ の E の直交は 0 です。

$u : E \to F$が同型であれば、$^t u : F^* \to E^*$は同型、$v : F \to E$が$u$の逆同型であれば、$^t v$は$^t u$の逆同型になります（式(17)、(18)）。

#### 定義 6 {#alg-ii-s2-def-6 .statement tag=05NJ}

* A-加群 E の同型 u を A-加群 F に与えると、u の逆同型の転置 (u の転置の逆同型に等しい) は、u の対偶同型と呼ばれ、$\tilde{u}$ で表されます。

したがって、同型 $\tilde{u}$ は関係によって特徴付けられます。
(19) $$
\langle u(x), \tilde{u}(y^*) \rangle = \langle x, x^* \rangle \quad \text{for } x \in E, x^* \in E^*.
$$

$v : F \to G$ が同型の場合、$v \circ u$ の反格同型は $\tilde{v} \circ \tilde{u}$ です。

特に、写像 $u \mapsto \tilde{u}$ は、線形群 $\mathbf{GL}(E^*)$ の部分群上に線形群 $\mathbf{GL}(E)$ の *同型* です。

$\sigma : A \to B$ を、環 $B$ への環 $A$ の *同型*、$E$ を左の $A$ モジュール、$F$ を左の $B$ モジュール、$u : E \to F$ を*半線形* 写像 (§ 1, no. 13) *$\sigma$ に対して*。 $\sigma^{-1}$ を $\sigma$ の逆同型とします。すべての $y^* \in F^*$、写像 $E$ の $x \mapsto \langle u(x), y^* \rangle^{\sigma^{-1}}$ を $A$ にすると *線型形式* になります。 ${}^t u(y^*)$ でも表される場合、写像 ${}^t u : F^* \to E^*$ が定義され、これは半線形マッピング $u$ の *転置* とも呼ばれます。したがって、それはアイデンティティによって特徴付けられます

$$
\langle u(x), y^* \rangle = \langle x, {}^t u(y^*) \rangle^\sigma
$$

$x \in E, y^* \in F^*$の場合。 ${}^t u$ が $\sigma^{-1}$ に対して *半線形* 写像であることがすぐに検証されます。 $v$ が写像 $u$ を $E$ から $\sigma_*(F)$ (§ 1, no. 13) への *A-linear* 写像とみなして表す場合、$u = \phi \circ v$ と書くことができます。ここで、$\phi$ は恒等写像 $\sigma_*(F) \to F$ と考えられます。 $\sigma$ を基準とした半線形マッピングとして。 ${}^t u = {}^t v \circ {}^t \phi$ と $({}^t \phi, \sigma^{-1})$ が同型 $\sigma^{-1}$ に対する $F^*$ の $(\sigma_*(F))^*$ への二同型であるのは明らかです。この関係により、半線形マッピングの線形写像から転置の転置のプロパティをすぐに拡大する行うことができます。

### 6. 商加群の二重。 直和のデュアル。デュアル基底

$F = A_s$ の場合に、no. 1 の定理を適用する 1 を適用します。

#### 命題 9 {#alg-ii-s2-prop-9 .statement tag=05NK}

*$E', E, E''$ *を A-加群とし、*

$$
E' \xrightarrow{u} E \xrightarrow{v} E'' \longrightarrow 0
$$

*線形写像の完全系列.* *その後、転置の数列写像*

$$
0 \longrightarrow {E''}^* \xrightarrow{{}^t v} E^* \xrightarrow{{}^t u} {E'}^*
$$

*正確です。*

#### 系 {#alg-ii-s2-n6-cor-1 .statement tag=05NL}

*M を A-加群 E と $\phi : E \to E/M$ 標準準同型の部分加群とします。すると* ${}^t \phi$ *は$E/M$ *部分加群* $M'$ *の* $E^*$ *直交* $M$の双対の同型です。

$j : M \to E$が標準単射なら、${}^t j$の核は$E^*$の$M$の直交定義によるものです。

さらに、系の記法では、移行から商のとき、${}^t j$から*単射法*準同型$E^*/M' \to M^*$が得られます。

#### 命題 10 {#alg-ii-s2-prop-10 .statement tag=05NM}

*$(E_i)_{i \in I}$ *A-加群の家族になりましょう* $i \in I$ *しましょう* $j_i : E_i \to E = \bigoplus_{i \in I} E_i$ *標準単射にしましょう* *それから積写像* $x^* \mapsto ({}^t j_i(x^*))$

*デュアル* $E^*$ *の* $E$ *上の積* $\prod_{i \in I} E_i^*$ の同型です。

これは、§ 1, no. 6、系 1 ～ 命題 6 の特定のケースであり、$\prod_{\lambda} F_{\lambda} = A_s$ の場合に適用されます。

標準単射 $j_i$ によって、$E_i$ が直和 $E$ の部分加群と識別され、積写像 $x^* \mapsto (tj_i(x^*))$ によって、$E^*$ が $\prod_{i \in I} E_i^*$ と識別される場合、 $\prod_{i \in I} E_i^*$ は $\bigoplus_{i \in I} E_i$ の双対であり、正規の双線形形式は次のように与えられると言われています。

$$
\langle (x_i), (x_i^*) \rangle = \sum_{i \in I} \langle x_i, x_i^* \rangle.
$$

(22)

#### 系 {#alg-ii-s2-n6-cor-2 .statement tag=05NN}

*Let M, N be two supplementary submodules in an A-module E and $p : E \to M, q : E \to N$ the corresponding projectors; then $^tp + ^tq : M^* \oplus N^* \to E^*$ is an isomorphism and $^tp$ (resp. $^tq$) is an isomorphism of $M^*$ (resp. $N^*$) onto the submodule of $E^*$ orthogonal to $N$ (resp. $M$). さらに、$i : M \to E$ と $j : N \to E$ が正準注入である場合、$^tp \circ ^ti$ と $^tq \circ ^tj$ は、$^tp(M^*)$ と $^tq(N^*)$ の直接和としての $E^*$ の分解に対応するプロジェクター $E^* \to ^tp(M^*)$ 、$E^* \to ^tq(N^*)$ です。

$p \circ i = 1_M, \quad q \circ j = 1_N, \quad p \circ j = q \circ i = 0, \quad i \circ p + j \circ q = 1_E$、よって、転置(no. 5、式(16)、(17)、(18))により、§ 1, no. 6、系 2から命題 6に$^ti \circ ^tp = 1_{M^*}, \ ^tj \circ ^tq = 1_{N^*}, \ ^tj \circ ^tp = ^ti \circ ^tq = 0. \ ^tp \circ ^ti + ^tq \circ ^tj = 1_{E^*}$、命題が続きます。

系の仮説の下では、$M^*$ (それぞれ $N^*$) は、$E^*$ の $N$ (それぞれ $M$) の直交 $^tp(M^*)$ (それぞれ $^tq(N^*)$) と識別されることが多く、したがってすべての線型形式が識別されます。 $M$ (それぞれ $N$) の $u$ と、$E$ の線型形式が $u$ に延長され、$N$ (それぞれ $M$) の零です。

A-加群 $E$ が *基底* $(e_t)_{t \in T}$ を認める場合、これに基底定義するを標準的に与えると同型 $u : A_s^{(T)} \to E$ となることがわかりました。 命題 10 と no. 3、命題 5 により、$A_s^{(T)}$ の双対は標準的に積 $A_d^T$ と識別されます。逆接同型 $\tilde{u} : A_d^T \to E^*$ を考えてみましょう。すべての $t \in T, f_t$ が $A_d^T$ の元で、その射影はすべて零ですが、添字 $t$ の例外は 1 に等しい場合、$e_t^* = \tilde{u}(f_t)$、元 $e_t^*$ と書くと、 $E^*$ は、(19) と (22) により、関係によって特徴付けられます。

$$
\langle e_t, e_{t'}^* \rangle = \begin{cases}
0 & \text{for } t' \neq t \\
1 & \text{for } t' = t.
\end{cases}
$$

(23)

$x = \sum_{t \in T} \xi_t e_t \in E, \ e_t^*(x) = \xi_t$ 全員にとって、これを言うのは同じことになります。また、$e_t^*$ は、$E$ 上の添字 $t$ の *座標形* とも呼ばれます。 (23) から、$(e_t^*)$ は $E^*$ の *free 系* であることがわかります。

特に、$T$ が *有限* である場合、$e_t^*$ 形は $E^*$ の *基底* となり、$f_t$ は $A_d^T$ の標準基底を形成します。したがって、次のようになります。

#### 命題 11 {#alg-ii-s2-prop-11 .statement tag=05NO}

*n 元の基底と自由加群の双対は、n 元の基底と自由加群です。*

自由加群と無限大基底の双対は、必ずしも自由加群 (VII, § 3, 練習問題 10) ではないことに注意してください。

#### 定義 7 {#alg-ii-s2-def-7 .statement tag=05NP}

*E が有限基底* $(e_t)$ を持つ自由加群である場合、 *関係 (23) で定義される双対 E* の *基底* $(e_t^*)$ は、関係 (23) で定義される双対基底 of* $(e_t)$ と呼ばれます。

関係 (23) は形にも書くことができます
$$
\langle e_t, e_{t'}^* \rangle = \delta_{tt'}
$$
ここで、$\delta_{tt'}$は$T \times T$の*クロネッカーシンボル*です。

$T$ が有限で、$(e_t^*)$ が $(e_t)$ の双対基底である場合、次のようになります。
$$ x = \sum_{t \in T} \xi_t e_t \in E, \quad x^* = \sum_{t \in T} \xi_t^* e_t^* \in E^*, $$
$$
\langle x, x^* \rangle = \sum_{t \in T} \xi_t \xi_t^*.
$$

*right* A-加群の有限基底の双対基底ももちろん同様に定義されます。

#### 系 {#alg-ii-s2-n6-cor-3 .statement tag=05NQ}

*有限生成射影加群の双対は有限生成射影加群です。*

有限生成射影左A-加群は、有限基底 (no. 2, 系 1 ～ 命題 4) を持つ自由A-加群 $A_s^n$ の直因子 M と識別できます。すると (命題 11 と系から命題 10) M* は $A_d^n$, よって系の直因子と同型です。

#### 命題 12 {#alg-ii-s2-prop-12 .statement tag=05NR}

*E を E の A-加群および* $(a_t)_{t \in T}$ *生成する系とします。次の条件は同等です:*
(a) *E は射影 A-加群.*
(b) *E 上に *線型形式の家族* $(a_t^*)_{t \in T}$ が存在し、すべて* $x \in E$ について、 *家族* $(\langle x, a_t^* \rangle)_{t \in T}$ *は有限台を持ち、*
$$
x = \sum_{t \in T} \langle x, a_t^* \rangle a_t.
$$

全射準同型 $u : L \to E$ が存在し、$L = A_s^{(T)}$ は、$(e_t)_{t \in T}$ が L の標準基底である場合、$u(e_t) = a_t$ (§ 1, no. 11, 命題 17) となります。 E が射影であるためには、$u \circ v = 1_E$ (no. 2, 命題 4 および § 1, no. 9, 命題 15) となる線形写像 $v : E \to L$ が存在することが必要かつ十分です。このような写像が存在し、${}^tv(e_t^*) = a_t^*$ と書くと、$\langle x, a_t^* \rangle = \langle x, {}^tv(e_t^*) \rangle = \langle v(x), e_t^* \rangle$ となり、家族 $(\langle x, a_t^* \rangle)$ はすべての $x \in E$ に対して有限台と $x = u \left( \sum_{t \in T} \langle (x), e_t^* \rangle e_t \right) = \sum_{t \in T} \langle x, a_t^* \rangle a_t$ を持ちます。逆に、主張の条件 (b) が満たされる場合、すべての $x \in E$ に対して和 $\sum_{t \in T} \langle x, a_t^* \rangle e_t$ が定義され、$x \to \sum_{t \in T} \langle x, a_t^* \rangle e_t$ は $u \circ v = 1_E$ となる線形写像 $v : E \to L$ になります。

### 7. バイデュアル

Eを左A-加群とします。 E の双対 $E^*$ の双対 $E^{**}$ は E の双対と呼ばれます。 左A-加群 (no. 3) でもあります。すべての $x \in E$ について、no. 3、式 (10) および (12) から、写像 $x^* \mapsto \langle x, x^* \rangle$ は右A-加群 $E^*$ では線型形式であり、他の語元は双対$E^{**}$ であることがわかります。 $\tilde{x}$ で表します。さらに、(9) と (11) (no. 3) から、E の $E^{**}$ への写像 $c_E : x \mapsto \tilde{x}$ は線形であることがすぐにわかります。この写像は正規と呼ばれます。一般に、E が有限に生成される場合でも、それは単射的でも全射的でもありません (cf. 練習問題 9(e) および § 7, no. 5, 定理 6)。

標準準同型 $c_E : E \to E^{**}$ が全単射の場合、A-加群 E は再帰的と呼ばれます。

F を 2 番目の左A-加群とします。すべての線形写像 $u : E \to F$、写像 $t(tu) : E^{**} \to F^{**}$ は、$tu$ によっても表され、線形であり、図式

$$
\begin{array}{ccc}
E & \xrightarrow{u} & F \\
c_E \downarrow & & \downarrow c_F \\
E^{**} & \xrightarrow{tu} & F^{**}
\end{array}
$$

は可換であり、定義と公式 (15) からすぐに次のようになり、線形写像の転置が得られます。

#### 命題 13 {#alg-ii-s2-prop-13 .statement tag=05NS}

*E が自由加群* (*自由加群と有限基底*) の場合、*標準写像* $c_E : E \to E^{**}$ *は単射* (*全単射*) です。

$(e_t)_{t \in T}$ を E の基底とし、$(e_t^*)$ を対応する座標形の族とする。 定義により、$x \in E$ が $\tilde{x} = 0$ である場合、すべての $t \in T$ に対して $\langle x, e_t^* \rangle = 0$ になります。他の語では、$x$ のすべての座標は零であるため、$x = 0$ になります。さらに、T が有限であると仮定します。 $\langle \tilde{e}_t, e_{t'}^* \rangle = \delta_{tt'}$ なので、$(\tilde{e}_t)$ は $E^{**}$ の $(e_t^*)$ の双対基底であり、E の $c_E$ 変換基底が $E^{**}$ の基底になるので、$c_E$ は次のようになります。全単射 (§ 1, no. 11、系 3 ～ 命題 17)。さらに次のことも証明しました。

#### 系 1 {#alg-ii-s2-prop-13-cor-1 .statement tag=05NT}

*E を有限の基底を持つ自由A-加群とします。 E のすべての基底* $(e_t)$ * について、$(c_E(e_t))$ * は基底* の双対基底 $(e_t^*)$ * $E^*$ * $(e_t)$ の二重です。

この場合、$(e_t)$と$(e_t^*)$は、1つの他の*の2つの*二重基底であると言われます。

#### 系 2 {#alg-ii-s2-prop-13-cor-2 .statement tag=05NU}

*E が有限基底を持つ自由A-加群である場合、E* のすべての有限基底は E の基底の双対基底です。

与えられた基底の E** 双対基底と、標準的に E** を使用して同一視する E を考慮するだけで十分です。

#### 系 3 {#alg-ii-s2-prop-13-cor-3 .statement tag=05NV}

*E、F を 2 つの A-加群とし、それぞれ有限の基底を持ち、E (それぞれ F) はその双対 E** (それぞれ F**) で正規に識別されます。次に、線形写像 u ごとに、E → F、$t^t u = u$.*

これは、図式の可換性 (27) の直後に続きます。

#### 系 4 {#alg-ii-s2-prop-13-cor-4 .statement tag=05NW}

*P が射影加群 (または有限生成射影加群) の場合、標準写像 $c_P : P \to P**$ は単射 (または全単射) です。*

次の補題を使用します。

#### 補題 1 {#alg-ii-s2-lem-1 .statement tag=05NX}

*M, N をA-加群 E の 2 つの補部分加群とし、i : M → E、j : N → E 標準単射とします。それでは図式*

$$
\begin{array}{ccc}
M \oplus N & \xrightarrow{c_M \oplus c_N} & M** \oplus N** \\
i + j \downarrow & & \uparrow t_{i_1} + t_{j_1} \\
E & \xrightarrow{c_E} & E**
\end{array}
$$

(28)

*は可換です。*

定義までに、$x \in M, y \in N, z^* \in E*$のために、

$$
\begin{align*}
\langle c_E(i(x) + j(y)), z^* \rangle &= \langle i(x) + j(y), z^* \rangle \\
&= \langle i(x), z^* \rangle + \langle j(y), z^* \rangle \\
&= \langle x, t_i(z^*) \rangle + \langle y, t_j(z^*) \rangle \\
&= \langle c_M(x), t_i(z^*) \rangle + \langle c_N(y), t_j(z^*) \rangle \\
&= \langle t_i(c_M(x)) + t_j(c_N(y)), z^* \rangle.
\end{align*}
$$

したがって、E が自由加群 (有限基底をもつ自由加群) である場合、$c_E$ は単射 (または全単射) です。一方、no. 6、命題 10 から、$t_i \oplus t_j$ は全単射であることがわかります。 図式 (28) の可換性は、$c_M \oplus c_N$ が単射 (それぞれ全単射) であることを意味し、したがって $c_M$ と $c_N$ (§ 1, no. 6, 系 1 から命題 7) になります。 no. 2、命題を考慮して、よって系 4.

### 8. 一次方程式

E、F を 2 A-加群とします。 形 $u(x) = y_0$ のすべての方程式。ここで、$u : E \to F$ は F の所与の線形写像、$y_0$ は F の所与の元であり、未知の $x$ は E でその値を取る条件の対象となり、a と呼ばれます。 *線形*方程式; $y_0$ は方程式の右辺と呼ばれます。 $y_0 = 0$ の場合、方程式は均一線形と呼ばれます。

$u(x_0) = y_0$ となるようなすべての元 $x_0 \in E$ は、線形方程式 $u(x) = y_0$ の解と呼ばれます。

大まかに言えば、問題が線形方程式の解を求めるのと同等であれば、問題は線形であるとよく言われます。

線形方程式 $u(x) = y_0$ が与えられると、方程式 $u(x) = 0$ は $u(x) = y_0$ に関連付けられた同次線形方程式と呼ばれます。

#### 命題 14 {#alg-ii-s2-prop-14 .statement tag=05NY}

*$x_0$ が線形方程式 $u(x) = y_0$ の解である場合、この方程式の解の集合は元 $x_0 + z$ の集合に等しくなります。ここで、$z$ は、解の集合を通過します。関連する同次方程式 $u(x) = 0$.*

関係 $u(x) = y_0$ は $u(x) = u(x_0)$ と書かれる場合があり、これは $u(x - x_0) = 0$ と同等です。

他の語では、方程式 $u(x) = y_0$ に少なくとも 1 つの解 $x_0$ がある場合、その解の集合は、核 $\overline{u}(0)$ からの翻訳によって得られる集合 $x_0 + \overline{u}(0)$ になります。 $u$。 部分加群である $\overline{u}(0)$ は、含む 0 (同次方程式 $u(x) = 0$ の零解、または自明解と呼ばれる) であるため、決して空ではないことに注意してください。

命題 14 のおかげで、線形方程式 $u(x) = y_0$ が *ちょうど 1 つの解* を持つには、少なくとも 1 つの解と $\overline{u}(0) = \{0\}$ が必要かつ十分です (他の語では、関連する等次方程式にゼロ以外の解がないこと、または$u$ *単射*);この場合、*すべて* $y \in F$ に対して、方程式 $u(x) = y$ には *最大で 1 つの解が含まれます。

#### 命題 15 {#alg-ii-s2-prop-15 .statement tag=05NZ}

※$u$を加群$E$の線形写像を加群$F$とします。方程式 $u(x) = y_0$ に少なくとも 1 つの解がある場合、$y_0$ は $^t u$ の核と直交します。*

$u(x) = y_0$ が解を認めるということは、$y_0 \in u(E)$ と命題が no. 5、系から命題 8 に続くことを意味します。

† これは実際には言葉の濫用です。論理的な点の観点から、ここでは語「解」を定義しているのではなく、単に「$x_0$は方程式$u(x) = y_0$の解である」という文が関係「$x_0 \in E$および$u(x_0) = y_0$」と同等であると定義しています。数学的な理論 $\mathscr{T}$ ここで、関係 "$A$ は環、$E$ と $F$ は $A$ モジュール、$u$ は $E$ の準同型であることに注意してください。 $F$, $y_0$ 元 of $F$" は定理、$\mathscr{T}$ のすべての *項* $T$ で、関係 "$T \in E$ と $u(T) = y_0$" が true になります$\mathscr{T}$ は、*集合理論*、I, § 5, no. 2 という意味で、方程式 $u(x) = y_0$ の *解* です。これは上記の言葉の乱用を正当化します。

命題 15 によって与えられる、$u(x) = y_0$ の解の存在に必要な基準は、$A$ が体 (§ 7, no. 6, 命題 12) である場合には十分ですが、*一般的には* (練習問題) ではないことに注意してください。 10)。

#### 注意 {#alg-ii-s2-n8-rem-1 .statement tag=05O0}

(1) $E$ を $A$ モジュール、$(F_i)_{i \in I}$ を $A$ モジュールのファミリー、すべての $i \in I$ について $u_i : E \to F_i$ を線形写像とします。線形方程式の系ごと
$$
u_i(x) = y_i \quad (i \in I)
$$
ここで、$y_i \in F_i$ は、*単一* 線形方程式 $u(x) = y$ と等価です。ここで、$u$ は、$E$ の写像 $x \mapsto (u_i(x))$ を $F = \prod_{i \in I} F_i$ および $y = (y_i)$ に変換したものです。 系 (29) は、すべての $i \in I$ に対して $y_i = 0$ である場合、*均質* と呼ばれます。

(2) $E$ が *基底* $(a_\lambda)_{\lambda \in L}$ を認めると仮定します。すべての $\lambda \in L$ について集合 $u(a_\lambda) = b_\lambda$ とすると、$x = \sum_{\lambda \in L} \xi_\lambda a_\lambda$ が方程式 $u(x) = y_0$ を満たすと言うのは、(有限台) $A$ の元の$(\xi_\lambda)_{\lambda \in L}$ が満たすというと同等です。 関係
$$
\sum_{\lambda \in L} \xi_\lambda b_\lambda = y_0.
$$

逆に、(30) を満たす有限サポートの $A$ の要素の族 $(\xi_\lambda)_{\lambda \in L}$ を探すことは、線形方程式 $u(x) = y_0$ を解くことと同じです。ここで、$u$ は、すべての $\lambda \in L$ について $u(a_\lambda) = b_\lambda$ となるような $E$ の $F$ への一意の線形マッピングです (§ 1, no. 11、系 3)提案17）。

(3) 線形方程式 $u(x) = y_0$ は、$F = A_s$ のとき *スカラー* と呼ばれ、したがって $u$ は $E$ および $y_0$ 上の *線型形式* です。 $E$ が基底 $(a_\lambda)_{\lambda \in L}$ を認める場合、*注意* (2) から、そのような方程式は次のように書くこともできることがわかります。
$$
\sum_{\lambda \in L} \xi_\lambda \alpha_\lambda = y_0 \in A
$$
ここで、スカラー族 $(\alpha_\lambda)$ は任意であり、族 $(\xi_\lambda)$ は有限台を持たなければならないことが理解されています。 一般に、スカラー線形方程式の系の *解* ($A$ における)
$$
\sum_{\lambda \in L} \xi_\lambda \alpha_{\lambda_i} = \eta_i \quad (i \in I)
$$
ここで、$\alpha_{\lambda_i} \in A$ と $\eta_i \in A$ は、*有限* サポートの元の $A$ と満たすのファミリー $(\xi_\lambda)_{\lambda \in L}$ と理解されます。 $\alpha_{\lambda_i}$ は方程式の系の *係数* と呼ばれ、$\eta_i$ は *右辺* と呼ばれます。 このような系の解は、$y = (\eta_i)$と$u : A_s^{(L)} \to A_s^I$が線形写像である方程式$u(x) = y$の解と等価です。
$$
(\xi_\lambda) \mapsto \left( \sum_{\lambda \in L} \xi_\lambda \alpha_{\lambda_i} \right).
$$

(4) 線形系 (32) は、混乱を避ける必要がある場合、左スカラー線形方程式 * 系とも呼ばれます。方程式の系
$$
\sum_{\lambda \in L} \alpha_{\lambda_i} \xi_\lambda = \eta_i \quad (i \in I)
$$

も同様に右スカラー線形方程式の系と呼ばれます。このような系は、$\xi_{\lambda}, \eta_i$ と $\alpha_{\lambda_i}$ を所属から反対環 $A^0$ から A とみなすことで、すぐに系 (32) に変換できます。

### 練習問題 {#alg-ii-s2-exercises}

[§ 2 に対して練習問題](exercises/s2/)を参照してください。
