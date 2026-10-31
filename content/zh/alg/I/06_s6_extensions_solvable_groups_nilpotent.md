---
book: alg
book_title: Algebra
chapter: I
chapter_title: ALGEBRAIC STRUCTURES
section: 6
section_title: Extensions, solvable groups, nilpotent groups
lang: zh
source: alg-i-iii
source_edition: 1998, Springer
book_pages: 65-81, 147-159
pdf_pages: 0089-0105, 0171-0183
extraction: ocr
subsections:
    - "no": 1
      title: EXTENSIONS
      page: 65
      pdf_page: 89
    - "no": 2
      title: COMMUTATORS
      page: 68
      pdf_page: 92
    - "no": 3
      title: LOWER CENTRAL SERIES, NILPOTENT GROUPS
      page: 71
      pdf_page: 95
    - "no": 4
      title: DERIVED SERIES, SOLVABLE GROUPS
      page: 74
      pdf_page: 98
    - "no": 5
      title: $p$-GROUPS
      page: 76
      pdf_page: 100
    - "no": 6
      title: SYLOW SUBGROUPS
      page: 78
      pdf_page: 102
    - "no": 7
      title: FINITE NILPOTENT GROUPS
      page: 80
      pdf_page: 104
statements: 58
exercises: 41
content_sha256: df1c7c3df8ffd270fbf9d0169c46e88e9e1b6721547a795c7baba69d0022ed83
translated_from: content/en/alg/I/06_s6_extensions_solvable_groups_nilpotent.md
translation_method: google
source_content_sha256: d821e97942b895b17be8ce1e792e14c608c04537847a1c472436cfaf015e5b24
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-39653cda
glossary_version: 34
glossary_terms_sha256: 334cb8eeb066d75e3f326be17a9a8c5c72d9f8a782c1dbade4c3a01cafcb66f1
prompt_sha256: 7fdd4e0b5e6067ff04498ebe670ef3580d6ba9506bf4d0c582d73af15fd73ef3
---

## § 6。 扩张，可溶解群，惰性群

在本段中，群运算、除非（另有明确提及）均以乘法书写。

### 1.扩张

#### 定义 1 {#alg-i-s6-def-1 .statement tag=05CQ}

令$F$和$G$为两个群。 $G$乘以$F$的扩张是三重$\mathscr{E} = (E, i, p)$，其中$E$是群，$F$的$i$单同态到$E$和$p$满同态 $E$ 到 $G$ 使得 $\operatorname{Im}(i) = \operatorname{Ker}(p)$。 同态$s : G \to E$（分别$r : E \to F$），使得$p \circ s = \operatorname{Id}_G$（分别$r \circ i = \operatorname{Id}_F$）被称为扩张$\mathscr{E}$的截面（分别收回）。

$F$对$G$的扩张$\mathscr{E} = (E, i, p)$通常表示为图表$\mathscr{E} : F \xrightarrow{i} E \xrightarrow{p} G$，其中$i$和$p$在不引起混淆的情况下省略有时。简单地说，有时是群$E$乘$F$是$G$的扩张。

对于群$E$是$G$乘$F$的扩张，包含正常的子群$F'$同构于$F$，使得商群$E/F'$同构是充分必要的到$G$。

如果像$i(F)$包含在$E$的中心中，扩张$\mathscr{E} : F \xrightarrow{i} E \xrightarrow{p} G$称为中心；仅当 $F$ 是可交换的时，这才有可能。

令$\mathscr{E} : F \xrightarrow{i} E \xrightarrow{p} G$和$\mathscr{E}' : F \xrightarrow{i'} E' \xrightarrow{p'} G$为$G$除$F$之二扩张。 $\mathscr{E}$到$\mathscr{E}'$的态射是同态$u : E \to E'$，使得$p' \circ u = p$和$u \circ i = i'$，或者，在其他字中，使得以下图表是可交换的：

$$
\begin{array}{ccc}
& & E \\
& i & \\
F & \xrightarrow{i'} & E' \\
& \downarrow & \downarrow \\
& & E \\
& p & \\
& & G
\end{array}
$$

$$
u \uparrow \quad \text{and} \quad p' \uparrow
$$

#### 命题 1 {#alg-i-s6-prop-1 .statement tag=05CR}

设$\mathscr{E}: F \xrightarrow{i} E \xrightarrow{p} G$和$\mathscr{E}': F \xrightarrow{i'} E' \xrightarrow{p'} G$为$G$除以$F$的扩张。如果$u: E \to E'$是$\mathscr{E}$的态射到$\mathscr{E}'$，$u$是$E$的同构到$E'$，$u^{-1}$是$\mathscr{E}'$的态射到$\mathscr{E}$。

令$x \in E$ 使得$u(x) = e$。然后$p(x) = p'(u(x)) = e$，从而$x \in i(F)$。令 $y \in F$ 使得 $x = i(y)$；然后$i'(y) = u(i(y)) = e$。由于 $i'$ 是单射的，$y = e$ 和 $x = e$。因此 $u$ 是单射的。根据§ 4, no. 6，推论1到命题7，$u$自$u(i(F)) = i'(F)$以来是满射的。 最后一个断言是直接的。

在其他字中，扩张$\mathscr{E}$和$\mathscr{E}'$是“同构的”当且仅当$\mathscr{E}$存在态射进入$\mathscr{E}'$。

设$F$和$G$为两个群，写为$E_0 = F \times G$；令 $i: F \to E_0$ 为典范嵌入，$p: E_0 \to G$ 为规范的投影。 $G$ 和 $F$ 同构于扩张 $\mathscr{E}_0: F \xrightarrow{i} E_0 \xrightarrow{p} G$ 的每个扩张被称为*平凡扩张*。

#### 命题 2 {#alg-i-s6-prop-2 .statement tag=05CS}

*令$\mathscr{E}: F \xrightarrow{i} E \xrightarrow{p} G$等于$G$除$F$的扩张。以下条件是等效的*：

(i) $\mathscr{E}$ 是一个平凡的扩张；
(ii) $\mathscr{E}$ 具有缩回 $r$；
(iii) $\mathscr{E}$具有截面$s$，使得$s(G)$包含在$i(F)$的扶正器中。

显然 (i) 意味着 (ii) 和 (iii)。如果(ii)成立，映射$(r, p): E \to F \times G$是$\mathscr{E}$的态射到$\mathscr{E}_0$，从而(i)。如果(iii)成立，$F \times G$的同态进入$E$，相应的到$(i, s)$（$\S$4，no. 9，命题12）是$\mathscr{E}_0$的态射进入$\mathscr{E}$，从而（一）。

扩张 $\mathscr{E}: F \to E \to G$ 可能并不平凡，但群 $E$ 同构于 $F \times G$ (习题 6)。

#### 定义 2 {#alg-i-s6-def-2 .statement tag=05CT}

*令$F$和$G$为$G$的两个群和$\tau$同态到$F$的自同构群。将$g \in G$和$f \in F$写成$\tau(g)(f) = gf$。 集合 $F \times G$ 律合成*

$$
((f, g), (f', g')) \mapsto (f, g) \cdot_{\tau} (f', g') = (f \cdot gf', gg')
$$

*被称为*$G$的外部半直接乘积相对于$\tau$的$F$。

$F$相对于$\tau$的$G$的外部半直接乘积表示为$F \times_{\tau} G$。

#### 命题 3 {#alg-i-s6-prop-3 .statement tag=05CU}

*外部半直接乘积$F \times_{\tau} G$为群。由$i(f) = (f, e)$定义的映射$i: F \to F \times_{\tau} G$、由$p(f, g) = g$定义的$p: F \times_{\tau} G \to G$以及$s(g) = (e, g)$定义的$s: G \to F \times_{\tau} G$为群同态。三重$(F \times_{\tau} G, i, p)$是$G$除以$F$的扩张，$s$是扩张的截面。*

我们有：

$$
((f, g) \cdot_{\tau} (f', g')) \cdot_{\tau} (f'', g'') = (f.gf', gg') \cdot_{\tau} (f'', g'')
= (f.gf'.gg'f'', gg'g'');
$$
$$
(f, g) \cdot_{\tau} ((f', g') \cdot_{\tau} (f'', g'')) = (f, g) \cdot_{\tau} (f'g'f'', g'g'')
= (f.g(f'.g'f''), gg'g'').
$$

现在$g(f'.g'f'') = gf'.gg'f''$，这表明由(1)定义的合成中的律是结合律。 元素$(e, e)$就是这个律下的身份。 元素 $(f, g)$ 承认为逆$(g^{-1}f^{-1}, g^{-1})$。因此，$F \times_{\tau} G$ 上的合成的律是群运算。其他断言是直接的。

使用命题 3 中的记号，$\mathscr{E}_{\tau}$ 将表示扩张

$$
F \xrightarrow{i} F \times_{\tau} G \xrightarrow{p} G.
$$

令$\mathscr{E}' : F \xrightarrow{i'} E' \xrightarrow{p'} G$等于$G$的扩张除以$F$以及$s' : G \to E'$截面除以$\mathscr{E}'$。我们在群 $F$ 定义运算 $\tau$ $G$ 通过：

(2)
$$
i'(\tau(g, f)) = s'(g)i'(f)s'(g)^{-1} = \operatorname{Int}(s'(g))(i'(f)).
$$

#### 命题 4 {#alg-i-s6-prop-4 .statement tag=05CV}

*对于上面的记号，$\mathscr{E}_{\tau}$中存在且仅有一个同构u到$\mathscr{E}'$，使得$u \circ s = s'$。

$$(f, g) = (f, e) \cdot_{\tau} (e, g) = i(f) \cdot_{\tau} s(g).$$ 因此，如果$u$是解到问题，则$u(f, g) = i'(f).s'(g)$、从而唯一性必然是$u$。我们证明存在。我们写$u(f, g) = i'(f).s'(g)$。然后

$$
\begin{align*}
u(f, g).u(f', g') &= i'(f)s'(g)i'(f')s'(g') \\
&= i'(f)(s'(g)i'(f')s'(g)^{-1})s'(g)s'(g') \\
&= i'(f)i'(\tau(g, f')).s'(g)s'(g') \\
&= i'(f.\tau(g, f')).s'(gg') \\
&= u((f, g) \cdot_{\tau} (f', g')).
\end{align*}
$$

因此，$u$是$F \times_{\tau} G$到$E'$的同态。显然是$u \circ i = i'$、$p' \circ u = p$和$u \circ s = s'$。

#### 注 {#alg-i-s6-n1-rem-1 .statement tag=05CW}

运算 $\tau$乘以公式 (2) 的定义取决于扩张$\mathscr{E}'$和截面$s'$。当$F$可交换时，运算$\tau$不依赖于$s'$。对于 $\operatorname{Int}(s'(g)) | i'(F)$ 则仅取决于 $s'(g)$ mod 的陪集。 $i'(F)$。

更一般地，令 $\mathscr{E} : F \to E \to G$ 通过交换群 $F$ 成为 $G$ 的扩张（不假设 $\mathscr{E}$ 承认截面）。 群$E$在$F$上运行内自同构，这个像在$F$的像上是微不足道的，因此在$F$上$G$的定义运算是微不足道的。如果$\mathscr{E}$承认截面，则这个运算就是由公式（2）定义的。

#### 推论{#alg-i-s6-n1-cor-1 .statement tag=05CX}

*令$G$为群、$H$和$K$$G$中的两个子群，使得$H$正常，$H \cap K = \{e\}$和$H.K = G$。令$\tau$等于$H$上$K$的运算除以$G$的内自同构。 映射 $(h, k) \mapsto hk$ 是 $H \times_{\tau} K$ 的同构到 $G$。

在这个推论的假设下，$G$据说是$K$乘以$H$的半直接乘积。

#### 例 {#alg-i-s6-n1-exa-1 .statement tag=05CY}

(1) 设$G$为群且$E$为齐次主体$G$集合；让$\Gamma$表示$G$的自同构群。 令 $A$ 为置换 $f$ $E$ 的集合，其中性质：
存在$\gamma \in \Gamma$使得$f$是$E$到$E$的$\gamma$态射（即$f(gb) = \gamma(g)f(b)$对于$b \in E$和$g \in G$）。
上面的公式$f(gb) = \gamma(g)f(b)$表明，如果$f \in A$存在唯一的$\gamma \in \Gamma$，使得$f$是$\gamma$态射，我们将其记为$p(f)$。
令$f, f'$位于$A$、$\gamma = p(f), \gamma' = p(f')$中。 然后，对于所有$b \in E$和所有$g \in G$，
$$
(f' \circ f)(gb) = f'(\gamma(g)f(b)) = \gamma'(\gamma(g))f'(f(b))
$$
这就证明了$f' \circ f \in A$和$p(f' \circ f) = p(f')p(f)$。 另一方面，$f(\gamma^{-1}(g)f^{-1}(b)) = gb$、从而、$f^{-1}(gb) = \gamma^{-1}(g)f^{-1}(b)$和$f^{-1} \in A$。 因此，$A$是$\mathscr{S}_E$的子群，$p$是$A$到$\Gamma$的同态。 $p$的核是$G$集合$E$的自同构的集合$\mathrm{Aut}_G(E)$。
我们修复$a \in E$。 我们在$G^0$的§ 5, no. 6同构$\psi_a$中定义到$\mathrm{Aut}_G(E)$，使得$\psi_a(x)(ga) = gxa$适用于$G$中的所有$g, x$。 另一方面，对于$\gamma \in \Gamma$，对于所有$g \in G$，令$s_a(\gamma)$为由$s_a(\gamma)(ga) = \gamma(g)a$定义的$E$的置换；立即验证$s_a$是$\Gamma$到$A$的同态，使得$p \circ s_a = \mathrm{Id}_{\tau}$。 因此，$G^0 \xrightarrow{\psi_a} A \xrightarrow{p} \Gamma$是$\Gamma$乘以$G^0$的扩张，$s_a$是这个扩张的截面。 $\Gamma$的这个扩张和这个截面定义运算作用于$G^0$，$s_a(\Gamma)$通过内自同构作用于$\psi_a(G^0)$；我们将这个运算写成指数形式。 我们证明这个运算是自然的运算（$§ 3$，no. 1，例3）：对于$G$和$\gamma \in \Gamma$中的$x, g$，
$$
(\psi_a(\gamma x))(ga) = (s_a(\gamma) \circ \psi_a(x) \circ s_a(\gamma)^{-1})(ga)
= (s_a(\gamma) \circ \psi_a(x))(\gamma^{-1}(g)a) = s_a(\gamma)(\gamma^{-1}(g)xa)
= g\gamma(x)a = \psi_a(\gamma(x))ga
$$
从而$^\gamma x = \gamma(x)$。
命题 4 则证明$A$ 在$G^0$ 上$\mathrm{Aut}(G)$ 的自然运算下与$\Gamma = \mathrm{Aut}(G)$ 的半直积同构于$G^0$。 Note that the isomorphism which we have constructed depends in general on the choice of the element $a \in E$.
(2) *Let $A$ be a commutative ring. 上三角形群 $T(n, A)$ 是上严格三角形群 $T_1(n, A)$ 对角线子群 $D(n, A)$ 的半直角乘积。*

### 2.换位子

#### 定义 3 {#alg-i-s6-def-3 .statement tag=05CZ}

令$G$为群，并且$x$和$y$为$G$的两个元素。 $G$的元素$x^{-1}y^{-1}xy$称为$x$和$y$的换位子。

(x,y)用于表示x和y的换位子。那么显然
$$(y, x) = (x, y)^{-1}.$$
对于 x 和 y 来说，$(x, y) = e$ 是充分必要的。更一般地说，
$$xy = yx(x, y).$$
另一方面我们写
(3)
$$x^y = y^{-1}xy = x(x, y) = (y, x^{-1})x.$$
因为映射 $x \mapsto x^y$ 是内自同构 $\operatorname{Int}(y^{-1})$，所以$(x, y)^z = (x^z, y^z)$ 对于所有 $x, y, z \in G$。

对于$x, y, z \in G$，我们证明以下关系：
(4)
$$(x, yz) = (x, z).(x, y)^z = (x, z).(z, (y, x)).(x, y)$$
（4之二）
$$(xy, z) = (x, z)^y.(y, z) = (x, z).((x, z), y).(y, z)$$
(5)
$$(x^y, (y, z)).(y^z, (z, y)).(z^x, (x, y)) = e$$
(6)
$$(x, yz).(z, xy).(y, zx) = e$$
（6之二）
$$(xy, z).(yz, x).(zx, y) = e.$$

现在
$$
\begin{align*}
(x, yz) &= x^{-1}z^{-1}y^{-1}xyz = (x, z)z^{-1}x^{-1}y^{-1}xyz = (x, z)(x, y)^z \\
&= (x, z)(z, (x, y)^{-1})(x, y)
\end{align*}
$$
由式（3），证明式（4）。 公式 (4之二) 类似。另一方面，
$$
\begin{align*}
(x^y, (y, z)) &= (x^y)^{-1}(z, y)(x^y)(y, z) \\
&= y^{-1}x^{-1}yz^{-1}y^{-1}zyy^{-1}xyy^{-1}z^{-1}yz \\
&= (yzy^{-1}xy)^{-1}(zxz^{-1}yz).
\end{align*}
$$
然后写出$u = yzy^{-1}xy, v = zxz^{-1}xy$和$w = xyx^{-1}zx$，我们得到
$$(x^y, (y, z)) = u^{-1}v.$$
通过循环排列$x, y, z$，我们推导出$(y^z, (z, x)) = v^{-1}w$并且
$$(z^x, (x, y)) = w^{-1}u,$$
这立即意味着（5）。最后，(6)将通过循环排列公式$(x, yz) = x^{-1}z^{-1}y^{-1}xyz = (yzx)^{-1}(xyz)$中的$x, y, z$得到的三个公式中的两侧相乘，对于(6之二)也类似。

如果A和B是G的两个子群，(A, B)表示由换位子$(a, b)$与$a \in A$和$b \in B$生成的子群。†则$(A, B) = \{e\}$当且仅当A集中B。$(A, B) \subset A$当且仅当B标准化A。如果A和B 是正常的（分别是特征），$(A, B)$ 也是如此。

† 我们在此拒绝§ 1中制定的符号约定，将合成的律延伸至子集。

#### 命题 5 {#alg-i-s6-prop-5 .statement tag=05D0}

令$A, B, C$为$G$中的三个子群。

(i) 子群$A$标准化子群$(A, B)$。

(ii) 如果子群$(B, C)$归一化$A$，子群$(A, (B, C))$由元素$(a, (b, c))$与$a \in A, b \in B$和$c \in C$生成。

(iii) 如果$A, B$和$C$正常，则

$$
(A, (B, C)) \subset (C, (B, A)).(B, (C, A)).
$$

通过（4之二），对于$a, a' \in A$和$b \in B$，

$$
(a, b)^{a'} = (aa', b).(a', b)^{-1},
$$

从而（一）。现在假设$(B, C)$标准化$A$。对于 $a \in A, b \in B, c \in C$ 和 $x \in G$，(4) 意味着

$$
(a, (b, c).x) = (a, x).(x, ((b, c), a))(a, (b, c))
$$

和$((b, c), a) \in A$，因为$(B, C)$通过归纳在$p$上规范化$A$，从而事实上，$\left( a, \prod_{i=1}^p (b_i, c_i) \right)$，对于$b_i \in B, c_i \in C$，属于到子群由元素生成形式$(a, (b, c))$。如果最终$A, B$和$C$是正常的，那么子群$(A, (B, C))$、$(C, (B, A))$和$(B, (C, A))$也是正常的。因此，只需证明 (ii)

$$
(a, (b, c)) \in (C, (B, A)).(B, (C, A))
$$

对于所有$a \in A, b \in B$和$c \in C$。现在由(5)，写$a^{b^{-1}} = u$

$$
(a, (b, c)) = ((u^b), (b, c)) = (c^u, (u, b))^{-1}.(b^c, (c, u))^{-1},
$$

从而（三）。

#### 定义 4 {#alg-i-s6-def-4 .statement tag=05D1}

设$G$为群。由$G$的元素的换位子生成的子群称为$G$的导出群。

因此，$G$的导出群是子群$(G, G)$。 也用$D(G)$表示。 通过滥用语言，它被称为有时 $G$ 的 *换位子群*，尽管它通常与 $G$ (习题 16) 的元素换位子集合不同。 $D(G) = \{e\}$当且仅当$G$是可交换的。

#### 命题 6 {#alg-i-s6-prop-6 .statement tag=05D2}

设$f : G \to G'$为群同态。然后$f(D(G)) \subset D(G')$。如果 $f$ 是满射，则 $D(G)$ 的同态到 $f$ 的 $D(G')$ 限制也是满射。

$G$元素换位子$f$下像为$G'$元素换位子。如果$f$是满射，则$G$换位子集合$f$下的像是$G'$换位子集合。因此，命题从§ 4, no. 3、推论3到命题2。

#### 推论 1 {#alg-i-s6-prop-6-cor-1 .statement tag=05D3}

群$G$的导出群是$G$的特征子群。特别是它是正常的子群 $G$。

#### 推论 2 {#alg-i-s6-prop-6-cor-2 .statement tag=05D4}

设G为群。 商群 G/D(G) 是可交换的。设$\pi : G \to G/D(G)$为典范同态。 G 的每个同态 f 到可交换的群 G' 都可以在形式 $f = \bar{f} \circ \pi$ 中唯一地表达，其中 $\bar{f} : G/D(G) \to G'$ 是同态。

现在$\pi(D(G)) = \{e\}$。由于$\pi$是满射，因此$D(G/D(G)) = \{e\}$，从而第一个断言。第二个来自 § 4, no. 4、命题 5。

#### 推论 3 {#alg-i-s6-prop-6-cor-3 .statement tag=05D5}

令 H 为 G 的子群。以下条件是等价的：

(i) $H \supset D(G)$；
(ii) H 是正规子群并且 $G/H$ 是可交换的。
(ii) $\Rightarrow$ (i) 由推论 2 和 (i) $\Rightarrow$ (ii) 由 § 4, no. 7、定理 4，因为可交换性群的每个子群都是正规的。

#### 推论 4 {#alg-i-s6-prop-6-cor-4 .statement tag=05D6}

设G为G的群和X子集，其中生成G。群D(G)是由X的元素的换位子生成的G的法线子群。

令H为由X的元素的换位子和$\phi : G \to G/H$典范同态生成的G的法线子群。 集合$\phi(X)$生成$G/H$。 $\phi(X)$ 的元素是成对可置换的，因此 H 是可交换的（§ 4, no. 3，推论 2 到命题 2）。因此（推论 3）H 包含于 D(G)。另一方面，显然$H \subset D(G)$。

#### 注 {#alg-i-s6-n2-rem-1 .statement tag=05D7}

(1) 推论2也可以用说表示，对于G来说，相对于交换律群和同态，从G到交换律群，$G/D(G)$与$\pi$一起，是普遍映射问题的解。

(2) 在推论4的假设下，X的元素的换位子生成的子群包含在D(G)中，但一般不等于D(G)(cf.习题15e)。

#### 例 {#alg-i-s6-n2-exa-1 .statement tag=05D8}

(1) 如果 G 是非交换简单群，则 $D(G) = G$。因此，G 的每个同态到可交换的群都是微不足道的。

(2) 对称群$S_n$的导出群为交错的群$A_n$。因为$A_n$是由乘积两次转置生成的；如果$\tau = \tau_{x,y}$和$\tau' = \tau_{x',y'}$是两个转置，则令$\sigma$为置换，使得$\sigma(x') = x$和$\sigma(y') = y$。那么$\tau' = \sigma^{-1} \tau \sigma$和$\tau \tau' = \tau^{-1} \tau' = \tau^{-1} \sigma^{-1} \tau \sigma$就是换位子。因此$A_n \subset D(S_n)$。由于$S_n/A_n$是可交换的，$A_n \supset D(S_n)$（推论3）。

### 3. 中下部级数，NILPOTENT 群

设G为群，G的H子群，K为G的正规子群。当且仅当$(G, H) \subset K$时，G/K中H的像包含在G/K的中心中。

#### 定义 5 {#alg-i-s6-def-5 .statement tag=05D9}

令 G 为群。 G 的下中心级数是 G 的子群的序列 $(C^n(G))_{n \geq 1}$，归纳定义为：
$$
C^1(G) = G, \quad C^{n+1}(G) = (G, C^n(G)).
$$

设$f : G \to G'$为群同态。由$n$上的归纳可以看出$f(C^n(G)) \subset C^n(G')$，并且如果$f$是满射，则$f(C^n(G)) = C^n(G')$。特别是，对于所有 $n \geq 1$，$C^2(G)$ 是 $G$ 的特征（因此是正常的）子群。对于所有$n \geq 1$，$C^n(G)/C^{n+1}(G)$包含在$G/C^{n+1}(G)$的中心中。

令 $(G_1, G_2, \ldots)$ 为 $G$ 正常子群的递减序列，使得 (1) $G_1 = G$； (2) 对于所有$i$，$G_i/G_{i+1}$包含在$G/G_{i+1}$的中心中。然后是$C^i(G) \subset G_i$，如$i$上的归纳所示。

现在
$$
(C^m(G), C^n(G)) \subset C^{m+n}(G).
$$
因为，如果这个关系用$(F_{m,n})$表示，那么它从$(F_{m,n})$，由no. 2，命题5得出，
$$
\begin{align*}
(C^m(G), C^{n+1}(G)) &\subset (G, (C^m(G), C^n(G))).(C^n(G), (G, C^m(G))) \\
&\subset C^{m+n+1}(G).(C^{m+1}(G), C^n(G)).
\end{align*}
$$
因此$((F_{m,n}) \text{ and } (F_{m+1,n})) \Rightarrow (F_{m,n+1})$。由于$(F_{m,1})$和$(F_{1,n})$是明显的，$(F_{m,n})$紧随其后的是归纳。

#### 定义 6 {#alg-i-s6-def-6 .statement tag=05DA}

*如果存在整数$n$使得$C^{n+1}(G) = \{e\}$，群$G$称为幂零。最小的整数 $n$ 使得 $C^{n+1}(G) = \{e\}$ 被称为幂零群 $G$ 的幂零类。*

如果类$n$的幂零$n \in \mathbf{N}$、群称为类$n$的幂零群。 有时表示，如果$G$是幂零的，则群$G$的幂零性类是有限的。

#### 例 {#alg-i-s6-n3-exa-1 .statement tag=05DB}

(1) 群是类 0（或$\leq 1$）的幂零当且仅当它由单位元素组成（或可交换）。

(2) *对于每个交换环 $A$ 和每个整数 $n \geq 1$，上严格三角形群 $T_1(n, A)$ 类 $\leq n - 1$ 幂幂（如果 $A \neq \{0\}$ 则恰好是类 $n - 1$）。*

(3) 设$G$为类$n$的幂零群。 $G$的每一个子群（或每商群）对于类$\leq n$都是幂零的。例如，如果$H$是$G$的子群，则$C^n(H) \subset C^n(G)$。如果$G'$是$G$的商群并且$\pi : G \to G'$是典范同态，则$C^n(G') = \pi(C^n(G))$。

(4) 幂零群的有限乘积是幂零的。

#### 命题 7 {#alg-i-s6-prop-7 .statement tag=05DC}

*令$G$为群且$n$整数。以下条件是等效的：*

(a) $G$ 类 $\leq n$ 幂零。
(b) *存在$G$的子群中的级数：*
$$
G = G^1 \supset G^2 \supset \ldots \supset G^{n+1} = \{e\}
$$
*这样*$(G, G^{k'}) \subset G^{k'+1}$*对于所有人*$k \in \{1, n\}$。

(c) 存在$G$的子群$A$包含在$G$的中心中，使得$G/A$对类$\leq n - 1$幂零。

(a)$\Rightarrow$ (b)：取$G^k = C^k(G)$即可。
(b) $\Rightarrow$ (a)：归纳于$k$、$C^k(G) \subset G^k$。
(a)$\Rightarrow$ (c)：取$A = C^n(G)$即可。
(c) $\Rightarrow$ (a)：令$\pi : G \to G/A$ 为典范同态；然后$\pi(C^n(G)) = C^n(G/A) = \{e\}$，因此$C^n(G) \subset A$，从而$C^{n+1}(G) = \{e\}$。

更简单地说：如果可以通过$n$连续的中心扩张从群$\{e\}$获得群，那么类$\leq n$是幂零的。

#### 推论{#alg-i-s6-n3-cor-1 .statement tag=05DD}

*幂零群的中心扩张（通过必然交换的群）是幂零的。*

#### 命题 8 {#alg-i-s6-prop-8 .statement tag=05DE}

*令$G$为类$\leq n$的幂零群，令$H$为$G$的子群。存在子群* 中的序列

$$
G = H^1 \supset H^2 \supset \ldots \supset H^{n+1} = H,
$$

*使得$H^{k+1}$在$H^k$中是正常的，并且$H^k/H^{k+1}$对于所有$k \leq n$来说是可交换的。*

Choose a sequence $(G^k)$ of subgroups of $G$ satisfying the conditions of Proposition 7 (b) for all $k$; $G^k$ is normal in $G$. 写：

$$
H^k = H.G^k.
$$

需要验证$H^{k+1}$被$H^k = H.G^k$归一化；由于它是通过$H$标准化的，因此只需验证它是通过$G^k$标准化的。现在，如果$s \in G^k$和$h \in H$，

$$
shs^{-1} = shs^{-1}h^{-1}.h \in (G, G^k).H
$$

并且$(G, G^k).H$包含在$G^{k+1}.H = H^{k+1}$中；因此$s.H^{k+1}.s^{-1} = H^{k+1}$，这表明$H^{k+1}$在$H^k$中是正常的。

最后，典范同态$G^k/G^{k+1} \to H^k/H^{k+1}$显然是满射的；由于第一个群是可交换的，所以第二个也是可交换的。

#### 推论 1 {#alg-i-s6-prop-8-cor-1 .statement tag=05DF}

*令 $G$ 为 $G$ 的幂零群和 $H$ 子群。如果$H$与$G$不同，则$G$中$H$的归一化器$N_G(H)$与$H$不同。*

令$k$为最大的指标，使得$H^k \neq H$。 群 $H^k$ 标准化了 $H$ 并且与 $H$ 不同。

#### 推论 2 {#alg-i-s6-prop-8-cor-2 .statement tag=05DG}

*令 $G$ 为 $G$ 的幂零群和$H$ 子群。如果 $H$ 与 $G$ 不同，则存在 $G$、包含于 $H$ 的正常子群 $N$，与 $G$ 不同，并且 $G/N$ 是可交换的。*

令 $k$ 是最小的指标，使得 $H^k \neq G$。 群$H^k$满足所需的条件。

#### 推论 3 {#alg-i-s6-prop-8-cor-3 .statement tag=05DH}

*设 G 为 G 的幂零群且 H 子群。如果 G = H.(G, G)，则 G = H。*

G 的每个子群 N 其中包含 H 并且使得 G/N 是可交换的包含 H.(G, G)。因此，推论 3 由推论 2 得出。

推论3也可以这样表述：设X为G的子集。对于X到生成G，G/D(G)中X的像生成G/D(G)是充分必要的。

#### 推论 4 {#alg-i-s6-prop-8-cor-4 .statement tag=05DI}

*令 f: G' → G 为群同态。假设*
(a) *G 是幂零的。*
(b) *同态 f₁：G'/(G', G') → G/(G, G)，由 f 通过经过得到商，是满射。*
*那么 f 是满射。*

这是从应用于子群 H = f(G') 的推论 3 得出的。

#### 命题 9 {#alg-i-s6-prop-9 .statement tag=05DJ}

*设 G 为类 ≤ n 的幂零群，令 N 为 G 的正规子群。存在子群的级数*

$$
N = N^1 \supset N^2 \supset \ldots \supset N^{n+1} = \{e\}
$$

*这样* (G, N^k) ⊂ N^{k+1} *对于 k = 1, ..., n.*

如果 (G^k) 满足命题 7 的条件 (b)，则取

$$
N^k = G^k \cap N.
$$

#### 推论 1 {#alg-i-s6-prop-9-cor-1 .statement tag=05DK}

*设 G 为 G 的幂零群，Z 中心，N 为 G 的正规子群。如果 N ≠ {e}，则 N ∩ Z ≠ {e}。*

令 k 为最大的指标，使得 N^k ≠ {e}。 群 N^k 包含在 N 中。 另一方面，(G, N^k) ⊂ N^{k+1} = {e}；因此 N^k 包含在 G 的中心 Z 中。

#### 推论 2 {#alg-i-s6-prop-9-cor-2 .statement tag=05DL}

*令 f 为从幂零群 G 到群 G' 的同态。如果 f 的限制到 G 的中心是内射的，则 f 是内射的。*

这是应用于 Ker(f) 的推论 1。

### 4.导出级数，可解群

#### 定义 7 {#alg-i-s6-def-7 .statement tag=05DM}

*设G为群。 G 的导出级数是级数 (D^n(G))_{n \in \mathbf{N}} 归纳定义为：*

$$
D^0(G) = G; \quad D^{n+1}(G) = D(D^n(G)) \quad \text{for } n \in \mathbf{N}.
$$

然后$D^0(G) = C^1(G) = G,\ D^1(G) = C^2(G) = D(G) = (G, G)$。对于所有 n \in \mathbf{N}，D^n(G) \子集 C^{2^n}(G)，如使用 no. 3 的公式 (7) 在 n 上的归纳所示。

令$f : G \to G'$为群同态。由 n 上的归纳可知 $f(D^n(G)) \subset D^n(G')$，并且如果 $f$ 是满射，则$f(D^n(G)) = D^n(G')$。特别是，对于所有$n \in \mathbf{N}$，$D^n(G)$是G的特征（因此正常）子群。对于所有$n \in \mathbf{N}$，群$D^n(G)/D^{n+1}(G)$是$G/D^{n+1}(G)$的交换范式（但不是一般中心）子群。

令 $(G_0, G_1, \ldots)$ 为 G 的子群的递减序列，使得： (1) $G_0 = G$； (2) 对于所有$i$，$G_{i+1}$在$G_i$中是正规的，$G_i/G_{i+1}$是可交换的。然后 $D^i(G) \subset G_i$ 对于所有 $i$，如$i$ 上的归纳所示。

#### 定义 8 {#alg-i-s6-def-8 .statement tag=05DN}

*如果存在整数 n 使得$D^n(G) = \{e\}$，则群 G 称为可解。如果 G 是可解的群，则使得 $D^n(G) = \{e\}$ 的最小整数 n 称为 G 的可解性类。*

可解性为类 $n$ 的可解群称为类 $n$ 的可解群。 群是有时，如果它是可解的，则称它具有有限可解性类。

#### 例 {#alg-i-s6-n4-exa-1 .statement tag=05DO}

(1) 群可解为类 0（或 $\leq 1$）当且仅当它减少到 $\{e\}$（或可交换）。

(2) 类 $\leq 2^n - 1$ 的每一个幂零群都可解为类 $\leq n$；这是从上面证明的关系$D^n(G) \subset C^{2^n}(G)$得出的。

(3) 令 G 为类 $\leq n$ 的可解群。 G 的每个子群（或商群）都可解为类 $\leq n$（证明类似于no. 3、例 3）。

(4) 如果 G 是类 $p$ 可解的群，并且 F 是类 $q$ 可解的群，则 F 的 G 的每个扩张 E 都是类可解的群 $\leq p + q$。对于，令$\pi : E \to G$为投影；那么$\pi(D^p(E)) \subset D^p(G) = \{e\}$，因此$D^p(E) \subset F$；由此可见$D^{p+q}(E) = D^q(D^p(E)) \subset D^q(F) = \{e\}$。

(5) 对称群 $S_n$ 可解当且仅当 $n < 5$ (cf. § 5, 习题 10 和 16)。

(6) *如果 A 为交换环，则上三角群 T(n, A) 可解，但一般不是幂零的。*

#### 命题 10 {#alg-i-s6-prop-10 .statement tag=05DP}

*设 G 为群，n 整数。以下条件是等效的：*

(i) *G 可解类 $\leq n$。*
(ii) *G的正常子群存在级数*
$$
G = G^0 \supset G^1 \supset \ldots \supset G^n = \{e\}
$$
*使得群 $G^k/G^{k+1}$ 是可交换的。*
(iii) *G的子群存在级数*
$$
G = G^0 \supset G^1 \supset \ldots \supset G^n = e
$$
*这样，对于所有 k，$G^{k+1}$ 是 $G^k$ 的正规子群，并且 $G^k/G^{k+1}$ 是可交换的。*

(iv) 存在$G$的正规交换律子群$A$，使得$G/A$可解类$\leq n - 1$。

对于 (i) $\Rightarrow$ (ii)，只要 $G^k$ 等于 $D^k(G)$ 即可。 (ii) $\Rightarrow$ (iii) 微不足道。 (iii) $\Rightarrow$ (i) $D^k(G)$ 必然包含在 $G^k$ 中。 (ii) 和 (iv) 的等价是$n$ 归纳的直接的。

更简单地说：如果可以通过$n$交换群的连续扩张获得群，那么类$\leq n$是可解的。

#### 推论{#alg-i-s6-n4-cor-1 .statement tag=05DQ}

令 $G$ 为有限群并且
$$
G = G^0 \supset G^1 \supset \ldots \supset G^n = \{e\}
$$
$G$ 的 Jordan-Hölder 级数要使 $G$ 可解，商 $G^k/G^{k+1}$ 是素数阶的循环是必要且充分的。

如果合成列与 $G$ 的商是循环的，因此可交换，则 $G$ 可通过命题 10 解。 相反，如果 $G$ 可解，则对于所有 $k$，群 $G^k/G^{k+1}$ 也是可解且简单的（$§ 4$、no. 7、命题 9）。 现在，每个可解的简单群$H$都是素数阶的循环。 For $D(H)$ is a normal subgroup of $H$; $D(H) = H$ is impossible for in that case $D^k(H) = H$ for all $k$; then $D(H) = \{e\}$ and $H$ is commutative. 然后推论从$§ 4$，no. 10，推论到命题 20。

### 5. $p$-组

In this number and the following, the letter $p$ denotes a prime number ($§ 4$, no 10, Proposition 16).

#### 定义 9 {#alg-i-s6-def-9 .statement tag=05DR}

阶是$p$的幂的有限群称为$p$群。

令 $G$ 为阶 $p^r$ 的$p$群。 $p^r$的每个除子都是$p$的幂（$§ 4$，no. 10，定理7的推论）。因此，$G$的每个子群和每个商群都是一个$p$群（$§ 4$，no. 4，命题4的推论）； $G$的每个齐次空间的基数是$p$的幂（$§ 5$，no. 5，定理1）。

$p$-群的$p$-群的扩张是$p$-群。

*例。 (1) 交换$p$群同构于循环群$\mathbf{Z}/p^n\mathbf{Z}$的乘积（cf.习题19以及VII，$§ 4$，no. 7，命题7）。
(2) 令$k$为特征$p$的有限域。严格三角形群$T_1(n, k)$是$p$群。
(3) 四元数群 $\{ \pm 1, \pm i, \pm j, \pm k \}$ 是一个 2 群 (cf. 习题 4).*

#### 命题 11 {#alg-i-s6-prop-11 .statement tag=05DS}

令$E$为有限集合，$G$为在$E$上运行的$p$群。让$E^G$表示$x \in E$的集合，使得$gx = x$适用于所有$g \in G$（固定的点）。然后
$$
\operatorname{Card}(E^G) \equiv \operatorname{Card}(E) \pmod{p}.
$$

E — E^G 是轨道的不相交的并，未减少到点。这样的轨道的基数是$p$的幂，与$p^0 = 1$不同，因此倍数是$p$。

#### 推论{#alg-i-s6-n5-cor-1 .statement tag=05DT}

*设 G 为 p 基团。如果 G 不减少为 e，则其中心不会减少为 e。*

让 G 对自身进行内自同构运算。固定点的集合是G的中心Z。由命题11，

$$
\operatorname{Card}(Z) \equiv \operatorname{Card}(G) \equiv 0 \pmod{p},
$$

从而$\operatorname{Card}(Z) \neq 1$和$Z \neq \{e\}$。

#### 定理 1 {#alg-i-s6-thm-1 .statement tag=05DU}

*设 G 为 p 群，$p^r$ 为阶。 G* 的子群存在序列

$$
G = G^1 \supset G^2 \supset \ldots \supset G^{r+1} = \{e\}
$$

*使得*$(G, G^k) \subset G^{k+1}, 1 \leq k \leq r,$和$G^k/G^{k+1}, 1 \leq k \leq r,$*是阶*$p$的循环。

定理对于 $G = \{e\}$ 成立。我们通过$\operatorname{Card}(G)$上的归纳来证明。设Z为G的中心，Z的$x \neq e$元素（命题11的推论）和x的$p^s, s \neq 0,$阶。那么$x^{p^s - 1}$是阶$p$的元素，因此Z包含子群$G'$是阶$p$的循环。到归纳假设时，群 $G' = G/G'$ 具有级数或子群 $({G'}^k)_{1 \leq k \leq r}$ 且具有所需的属性。设$\pi : G \to G'$为典范同态。由$G^k = \pi^{-1}({G'}^k), 1 \leq k \leq r, G^{r+1} = \{e\}$定义的G的子群的序列对于$G^k/G^{k+1}$来说是解，与$1 \leq k \leq r$的${G'}^k/{G'}^{k+1}$同构的（§ 4, no. 7，定理4）。

#### 推论{#alg-i-s6-n5-cor-2 .statement tag=05DV}

*每个 p 群都是幂零的。*

这是从 no. 3、命题 7 得出的。

#### 命题 12 {#alg-i-s6-prop-12 .statement tag=05DW}

*设 G 为 p 群，G 的 H 子群与 G 不同。则：*

(a) *归一化器* $N_G(H)$ *G 中的 H 与 G* 不同。
(b) *G 中存在指标 p 的正常子群* N *，其中包含* H。

断言 (a) 由no. 3、推论1 到命题 8。我们证明(b)。根据 no. 3，推论 2 到命题 8，存在 G 包含 H 的正规子群 $N'$，与 G 不同，并且 $G/N'$ 是可交换的。令 N 为与 G 包含 $N'$ 不同的最大子群。那么 N 是正规的（no. 2，推论 3 到命题 6），$G/N$ 是一个简单交换的 $p$ 群，因此是阶 $p$ 的循环（§ 4, no. 10，推论到命题 20）。

#### 推论{#alg-i-s6-n5-cor-3 .statement tag=05DX}

*设 G 为 p 基团。 指标 p 的 G 的每子群都是正常的。*

### 6.西洛子群

#### 定义 10 {#alg-i-s6-def-10 .statement tag=05DY}

令 G 为有限群。 G 的 Sylow p 子群是 G 满足以下两个条件的任意子群 P：

(a) P 是 p 基团。
(b) (G : P) 不是 p 的倍数。

如果G的阶写成形式$p^r m$，其中m不是$p$的倍数，则条件(a)和(b)等价于$\mathrm{Card}(P) = p^r$。

#### 例 {#alg-i-s6-n6-exa-1 .statement tag=05DZ}

(1) 在群$\mathfrak{S}_p$中，令$\zeta$为阶$p$的循环。由$\zeta$生成的子群是$\mathfrak{S}_p$的Sylow$p$子群，对于$p$不是除$(p - 1)!$。
(2) *令k为特征$p$的有限域，令n为正整数。严格三角形群 $T_1(n, k)$ 是群 $\mathbf{GL}(n, k)$ 的 Sylow $p$ 子群。*

#### 定理 2 {#alg-i-s6-thm-2 .statement tag=05E0}

每有限群包含一个Sylow$p$子群。

证明取决于以下引理。

#### 引理 {#alg-i-s6-n6-lem-1 .statement tag=05E1}

令$n = p^r m$，其中m是整数，它不是$p$的倍数。然后
$$
\binom{n}{p^r} \not\equiv 0 \pmod{p}.
$$

令 S 为阶 $p^r$ 的群（对于例 $\mathbf{Z}/p^r \mathbf{Z}$），T 集合，m 元素。写出$X = S \times T$，令E为X的子集集合和$p^r$元素。然后$\mathrm{Card}(X) = n$，从而$\mathrm{Card}(E) = \binom{n}{p^r}$（集合理论，III, § 5, no. 8，推论1到命题11）。让S对X进行$s.(x, y) = (sx, y) (s, x \in S, y \in T)$操作，并考虑这个运算到E的规范扩张。在no. 5的记号，命题11，集合$E^S$是集合 X的轨道，即形式$S \times \{ t \}, t \in T$的子集$Y \subset X$集合，从而$\mathrm{Card}(E^S) = m$。 no. 5、命题 11 点之前，
$$
\binom{n}{p^r} = \mathrm{Card}(E) \equiv \mathrm{Card}(E^S) = m \not\equiv 0 \pmod{p},
$$
这就证明了引理。

我们现在证明定理。设G为有限群，n为阶；我们写 $n = p^r m$，其中 m 不是 $p$ 的倍数。令 E 为 G 的子集的集合，其中$p^r$ 元素。然后
$$
\mathrm{Card}(E) = \binom{n}{p^r};
$$
从而，凭借引理、$\mathrm{Card}(E) \not\equiv 0 \pmod{p}$。通过左平移考虑 G 的运算的扩张到 E。存在 $X \in E$ ，其轨道具有非零基数模。 $p$。如果 $H_X$ 表示 X 的稳定子，则

$(G:H_x) \not\equiv 0 \pmod{p}$，即$p^r$除$\mathrm{Card}(H_x)$。但是 $H_x$ 由 $s \in G$ 组成，使得 $sX = X$；如果$x \in X$，则$H_x \subset X.x^{-1}$，从而$\mathrm{Card}(H_x) \leqslant \mathrm{Card}(X) = p^r$。因此$\mathrm{Card}(H_x) = p^r$。

#### 推论{#alg-i-s6-n6-cor-1 .statement tag=05E2}

*如果 G 的阶能被 p 整除，则阶 p 的群 G 包含元素*

凭借定理 2，这被简化为G是$p$群$\neq \{e\}$的情况；如果$x \in G$与e不同，则x生成的循环群是阶$p^n$和$n \geqslant 1$，因此它是阶$p$的包含子群。

#### 注 {#alg-i-s6-n6-rem-1 .statement tag=05E3}

对于每个素数数 q 除Card(G)，令P_q 为G 的Sylow q 子群。则P_q 生成的G 的子群 H 为每个q 的Card(P_q) 的阶倍数以及Card(G) 的阶除子，因此它等于G。

#### 定理 3 {#alg-i-s6-thm-3 .statement tag=05E4}

*设 G 为有限群。*
(a) *G 的 Sylow p 子群为共轭到 1 另一个。它们的数等于 1 mod。 p.*
(b) *作为 p 群的 G 的每个子群都包含在 Sylow p 子群中。*

令 P 为 G (定理 2) 的 Sylow $p$ 子群，并令 H 为 G 的 $p$ 子群。令 E = G/P，并考虑 G/P 上 H 的运算。作为卡片(E) $\not\equiv 0$ mod。 $p$, 命题 11 of no. 5，表明存在$x \in G/P$，使得$hx = x$ 对于所有$h \in H$。如果g是G中x的代表，则意味着$H \subset gPg^{-1}$，从而断言(b)。

如果 H 是 Sylow $p$ 子群，则 Card(H) = Card(P) = Card($gPg^{-1}$), 从而 $H = gPg^{-1}$，这就证明了(a)的第一个断言。

我们现在证明(a)的第二个断言。令 $\mathscr{S}$ 为 G 的 Sylow $p$ 子群的集合，并令 P 通过内自同构对 $\mathscr{S}$ 进行运算。 元素$P \in \mathscr{S}$是这个运算下固定的点，我们证明它是唯一的。设$Q \in \mathscr{S}$为固定的点； Q 是由 P 归一化的 G 的 Sylow 子群，因此 P 包含在 Q 的归一化子 N 中。 群 P 和 Q 是 N 的 Sylow $p$ 子群；因此存在$n \in N$使得$P = nQn^{-1} = Q$。由 no. 5、命题 11、卡($\mathscr{S}^P$) $\equiv$ 卡($\mathscr{S}^{P^P}$) = 1 (mod. $p$)。

#### 推论 1 {#alg-i-s6-thm-3-cor-1 .statement tag=05E5}

*设 P 为 G 的 Sylow p 子群，N 为 G 中的归一化子，M 为 G 包含于 N 的子群。G 中 M 的归一化子等于 M。*

令$s \in G$ 使得$sMs^{-1} = M$。 M 的子群 $sPs^{-1}$ 是 M 的 Sylow $p$ 子群。因此存在 $t \in M$ 使得 $sPs^{-1} = tPt^{-1}$；然后$t^{-1}s \in N$，从而$s \in tN \subset M$。

#### 推论 2 {#alg-i-s6-thm-3-cor-2 .statement tag=05E6}

*令 $f : G_1 \to G_2$ 为有限群中的同态。对于 $G_1$ 的每个 Sylow p 子群 $P_1$，都存在 $G_2$ 的 Sylow p 子群 $P_2$，使得 $f(P_1) \subset P_2$。*

这是从应用于 $G_2$ 的子群 $f(P_1)$ 的定理 3 (b) 得出的。

#### 推论 3 {#alg-i-s6-thm-3-cor-3 .statement tag=05E7}

(a) 设$H$为$G$的子群。对于$H$的每个Sylow $p$子群$P$，都存在$G$的Sylow $p$子群$Q$，使得$P = Q \cap H$。

(b) 相反，如果 $Q$ 是 $G$ 的 Sylow $p$ 子群，并且 $H$ 在 $G$ 中是正规子群，则群 $Q \cap H$ 是 $H$ 的 Sylow $p$ 子群。

(a) $p$群$P$包含在$G$的Sylow$p$子群$Q$中，$Q \cap H$是$H$包含于$P$的$p$子群，因此相等到$P$。

(b) 令 $P'$ 为 $H$ 的 Sylow $p$ 子群。存在元素$g \in G$使得$gP'g^{-1} \subset Q$。由于$H$是正常的，$P = gP'g^{-1}$包含在$H$中，因此包含在$Q \cap H$中。由于$Q \cap H$是$H$的$p$子群，$P$是$H$、$P = Q \cap H$的Sylow $p$子群。

#### 推论 4 {#alg-i-s6-thm-3-cor-4 .statement tag=05E8}

令 $N$ 为 $G$ 的正常子群。 $G$的Sylow $p$子群的$G/N$中的像是$G/N$的Sylow $p$子群，并且$G/N$的每个Sylow $p$子群都是通过这种方式获得的。

令$G' = G/N$和$P'$为$G$的Sylow$p$子群$P$的$G'$中的像。 群 $G$ 在 $G'/P'$ 上传递操作，因此 $G'/P'$ 等价于 $G/S$，其中 $S$ 是 $G$ 包含 $P$ 的子群。因此$(G':P')$除$(G:P)$，因此不是$p$的倍数，并且$p$群$P'$是$G'$的Sylow$p$子群。令 $Q'$ 为另一个 Sylow $p$-$G'$ 的子群；然后$Q' = g'P'{g'}^{-1}$对于一些$g' \in G'$；如果$g \in G$是$g'$的代表，那么群$Q'$就是$Q = gPg^{-1}$的像。

### 7. 有限幂零群

#### 定理 4 {#alg-i-s6-thm-4 .statement tag=05E9}

令 $G$ 为有限群。以下条件是等效的：

(a) $G$ 幂零的。
(b) $G$是$p$组中的乘积。
(c) 对于每个素数数$p$，都存在一个$G$的正规Sylow$p$子群。
(b) $\Rightarrow$ (a) (no. 5，定理 1 的推论)。

假设 (a) 成立并令 $P$ 为 $G$ 的 Sylow $p$ 子群。如果$N$是$G$中$P$的标准化子，推论1到定理3表明$N$是它自己的标准化子。由§ 6, no. 3，推论命题 8，这表明$N = G$。因此 (a) $\Rightarrow$ (c)。

假设 (c) 成立，且令 $I$ 为素数数除以 $\mathrm{Card}(G)$ 的集合。对于所有$p \in I$，令$P_p$是$G$的正规Sylow$p$子群。对于所有$p \neq q$，$P_p \cap P_q$减少为$e$，因为它既是$p$群又是$q$群，因此$P_p$和$P_q$集中一个另一个（$§ 4$，no. 9， 命题15)。设$\phi$为$\prod_{p \in I} P_p$的典范同态（$§ 4$，no. 9，命题12）到$G$。 同态 $\phi$ 是no. 6 的注的满射。由于 $\mathrm{Card}\left(\prod_{p \in I} P_p\right) = \mathrm{Card}(G)$，因此 $\phi$ 是双射的。

#### 注 {#alg-i-s6-n7-rem-1 .statement tag=05EA}

(1) 令 G 为有限群且$p$素数数。由no. 6，定理 3 (a) 和no. 6，定理 2，以下条件是等价的：
(i) G 存在正规 Sylow $p$ 子群；
(ii) G 的每个 Sylow $p$ 子群都是正规的；
(iii) G 只存在一个 Sylow $p$ 子群。

(2) 设 G 为幂零有限群。设我是卡(G)的素数除子的集合。由定理 4 和注 1，$G = \prod_{p \in I} G_p$，其中 $G_p$ 是 G 中唯一的 Sylow $p$ 群。

（3）应用于交换律群，定理 4 给出分解，交换律有限群作为主要成分乘积，将在章七中从另一个点的角度进行研究。

#### 例 {#alg-i-s6-n7-exa-1 .statement tag=05EB}

群 $\mathfrak{S}_3$ 是阶 6。包含阶 3 的正规 Sylow 3 子群：群 $A_3$。它包含阶2的三个Sylow 2子群：群$\{e, \tau\}$，其中$\tau$是转置。因此群$\mathfrak{S}_3$不是幂零的。

### 习题{#alg-i-s6-exercises}

§ 6](exercises/s6/)参见[习题。
