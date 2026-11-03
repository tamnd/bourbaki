---
book: ens
book_title: Theory of Sets
chapter: ER
chapter_title: SUMMARY OF RESULTS
section: 4
section_title: Union, intersection, product of a family of sets
lang: zh
source: ens-i-iv
source_edition: 2004, Springer
book_pages: 363-370
pdf_pages: 0368-0375
extraction: ocr
statements: 0
exercises: 0
content_sha256: b7ece19b960b00fbc840eb0f2cf9de2d1f36873c076d3c17a4bc5732caec6d4d
translated_from: content/en/ens/ER/04_s4_union_intersection_product_of_a_family.md
translation_method: google
source_content_sha256: 4b835593887f6b43eb749a64666773682e6a55745eeea04dc0f501209be0cff8
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-1fd6073a
glossary_version: 34
glossary_terms_sha256: 40b383969c556695a4fd6d696b7ef9c309a6b81fb141b6cce39d378872857cc5
prompt_sha256: 8cbde7b7ea18274bea5720e1f500823a36194a717a2895a9c9e7e3ffc4a3a3ae
---

## 4. 并、交、集族的积

1. 在这个截面中，我们考虑集合$E$的子集的$(X_i)_{i\in I}$族，其中指标集合$I$是任意的； $E$ 属于的集合 / 子集给家庭将用$\mathfrak{X}$ 表示（因此是子集 / $\mathfrak{P}(E)$）。

如果$I$是有限的，$(X_i)$约化对$E$的几个子集的考虑，可能是不同的，也可能不是不同的，并且在数中等于$I$的元素的数。例如，$E$形式任意三个子集$X_1,X_2,X_3$$E$子集，指标集合这里由……组成数1,2,3。

2. 令$J$为$I$中的任意子集，并考虑所有具有性质的元素$x$中的集合，“存在$i\in J$使得$x\in X_i$”。这个集合称为集合$(X_i)_{i\in J}$家族的并，记为$\displaystyle\bigcup_{i\in J}X_i$。

我们还可以将这个定义表述如下：将$I$的映射$i\mapsto X_i$转化为$\mathfrak{P}(E)$，其中对应有一个明确定义的$I\times E$的子集$C$，使得$X_i=C(i)$ (§ 3, no. 7)，我们有$\displaystyle\bigcup_{i\in J}X_i=C(J)$。

特别是，

$$
\bigcup_{i\in\varnothing}X_i=C(\varnothing)=\varnothing .
$$

当$J=I$时，我们经常写$\displaystyle\bigcup X_i$，或者简称为$\displaystyle\bigcup X_i$，来代替$\displaystyle\bigcup_{i\in I}X_i$。

并$\displaystyle\bigcup_{i\in I}X_i$仅取决于集合$\mathfrak{X}$；其他字，两个家庭的相应的到$\mathfrak{P}(E)$的子集$\mathfrak{X}$是一样的。特别是，它等于$\mathfrak{X}$的典范映射到$\mathfrak{P}(E)$定义的族的并，因此我们可以写为$\displaystyle\bigcup_{X\in\mathfrak{X}}X$，也称为集合属于到$\mathfrak{X}$的并。

当$I$是集合且元素被显式指定时，例如数1,2,3，我们有

$$
\bigcup_{i\in I}X_i=X_1\cup X_2\cup X_3,
$$

这证明了一般情况下给出的名称“并”是集合$\displaystyle\bigcup_{i\in I}X_i$。

# 结果总结

3. 对于任意$J\subset I$，我们有

$$
\bigcup_{\iota\in J}X_{\iota}\subset\bigcup_{\iota\in I}X_{\iota}.
$$

特别是，对于所有 $\iota\in I$，我们有

$$
X_{\iota}\subset\bigcup_{\iota\in I}X_{\iota}.
$$

相反，如果 $Y$ 是 $E$ 的子集，使得 $X_{\iota}\subset Y$ 对于所有 $\iota\in I$，则

$$
\bigcup_{\iota}X_{\iota}\subset Y.
$$

更一般地，如果$(Y_{\iota})$是$E$的子集的另一个族，由相同的集合$I$索引，并且如果$X_{\iota}\subset Y_{\iota}$对于所有$\iota\in I$，则

$$
\bigcup_{\iota}X_{\iota}\subset\bigcup_{\iota}Y_{\iota}.
$$

令$F$为另一个集合，并令$X\to K(X)$为$\mathfrak{P}(E)$的映射，进入由$E\times F$的子集$K$定义的$\mathfrak{P}(F)$。然后我们有

(34)

$$
K\left(\bigcup_{\iota\in J}X_{\iota}\right)=\bigcup_{\iota\in J}K(X_{\iota}).
$$

现在令$L$为另一个指标集合，$(J_{\lambda})_{\lambda\in L}$为$I$的子集家族。然后

(35)

$$
\bigcup_{\iota\in\bigcup_{\lambda\in L}J_{\lambda}}X_{\iota}
=
\bigcup_{\lambda\in L}\left(\bigcup_{\iota\in J_{\lambda}}X_{\iota}\right).
$$

这是并的通用 *结合性* 公式。当$I$和$L$是集合且元素被显式指定时，我们得到的关系已经被给定了（参见§ 1, no. 14）。如果 $L$ 单独满足这个条件并且由数 1, 2 组成，我们有

(36)

$$
\bigcup_{\iota\in J_1\cup J_2}X_{\iota}
=
\left(\bigcup_{\iota\in J_1}X_{\iota}\right)\cup
\left(\bigcup_{\iota\in J_2}X_{\iota}\right).
$$

令$(X_{\iota})_{\iota\in I}$和$(Y_{\chi})_{\chi\in K}$为$E$的子集的任意两个族。然后我们有

(37)

$$
\left(\bigcup_{\iota\in I}X_{\iota}\right)\cap
\left(\bigcup_{\chi\in K}Y_{\chi}\right)
=
\bigcup_{(\iota,\chi)\in I\times K}(X_{\iota}\cap Y_{\chi}).
$$

*分配律* 公式，其中包括（10）的第二个公式作为特殊情况。

如果$(X_i)_{i\in I}$是E的子集族，并且如果$(Y_x)_{x\in K}$是F的子集族，那么

(38)

$$
\left(\bigcup_{i\in I}X_i\right)\times\left(\bigcup_{x\in K}Y_x\right)=\bigcup_{(i,x)\in I\times K}(X_i\times Y_x).
$$

4. E 的子集的族 $(X_i)_{i\in I}$ 是 E 的子集 A 的*覆盖*，或者覆盖 A，如果

$$
A\subset\bigcup_{i\in I}X_i.
$$

特别是，如果 $(X_i)$ 是 E 的覆盖，我们有

$$
\bigcup_{i\in I}X_i=E.
$$

E 的 *划分* 是 E 的覆盖$(X_i)$，使得

(a) $X_i\neq\varnothing$ 对于所有 $i\in I$；

(b) $X_i\cap X_j=\varnothing$ 对于 I 中*不同* 指标 $i,\ j$ 的每个对。 （第二个条件可以用说来表示，$X_i$是*成对的不相交的*。）

这些条件意味着$i\mapsto X_i$是I的*双射*到划分的子集的集合$\mathfrak{P}$。因此，如果给出 $\mathfrak{P}$，则该家庭被确定在指标集合的一对一对应范围内。特别是，划分可以被无差别地视为子集的集合或子集的*家族*。

5. 令$(X_i)_{i\in I}$为集合E的任何非空子集族。在乘积$I\times E$中，令$X'_i$对于每个$i\in I$表示子集$\{i\}\times X_i$。 集合

$$
S=\bigcup_{i\in I}X'_i
$$

被称为$(X_i)_{i\in I}$家族的*和*。很明显，家族$(X'_i)_{i\in I}$是S的划分，并且对于每个$i\in I$映射$x_i\mapsto(i,x_i)$来说，$X_i$的双射到$X'_i$。通过滥用语言，与 S 一对一的对应中的任何集合通常被称为 $(X_i)_{i\in I}$ 家族的和，而 $X_i$ 通常被认为是他们对应的这个集合的子集。

两个非空集合 E 和 F 的和通常被认为是通过“邻接”集合 F 到 E 获得的。

6. 与no. 2的记号，元素$x$的集合，其中有性质“对于所有$i\in J$，$x\in X_i$”称为族的*交集合*

$(X_\iota)_{\iota\in J}$，记为$\displaystyle\bigcap_{\iota\in J}X_\iota$；当$J=I$时，我们经常写$\displaystyle\bigcap_\iota X_\iota$，或者简称为$\displaystyle\cap X_\iota$，而不是$\displaystyle\bigcap_{\iota\in I}X_\iota$。

我们有

(39)
$$
\mathrm{C}\left(\bigcup_{\iota\in J}X_\iota\right)=\bigcap_{\iota\in J}(\mathrm{C}X_\iota).
$$

特别是，如果$J=\varnothing$，

(40)
$$
\bigcap_{\iota\in\varnothing}X_\iota=E.
$$

交$\displaystyle\bigcap_\iota X_\iota$仅依赖于集合$\mathfrak{F}$，并且可以写成$\displaystyle\bigcap_{X\in\mathfrak{F}}X$。例如，如果 $I$ 由数 $1$、$2$、$3$ 组成，我们有

$$
\bigcap_\iota X_\iota=X_1\cap X_2\cap X_3.
$$

7. 公式 (39) 使我们能够推广*对偶规则*。如果E的子集A是通过应用（在任何序中）从其他子集X、Y、Z和族$(X_\iota)$、$(Y_\iota)$、$(Z_\lambda)$获得E的子集（在任何序中）*仅*运算 $\mathrm{C}$, $\cup$, $\cap$, $\displaystyle\bigcup$, $\displaystyle\bigcap$, 那么我们就可以得到替换子集 X, Y, Z, $X_\iota$, $Y_\iota$的补码$\mathrm{C}A$, $Z_\lambda$ 的补码，以及运算 $\cup$、$\cap$、$\displaystyle\bigcup$、$\displaystyle\bigcap$ 分别由 $\cap$、$\cup$、$\displaystyle\bigcap$、$\displaystyle\bigcup$、序组成运算被保存；当然，交和并中的运算适用于写在$\displaystyle\bigcup$和$\displaystyle\bigcap$符号下的*指标* 集合，则不可更改。

与§ 1, no. 15一样，我们定义关系A = B或A$\subset$B的*对偶*，其中A和B是上述形式的E的子集。

8. 对于所有$J\subset I$，我们有

$$
\bigcap_{\iota\in I}X_\iota\subset\bigcap_{\iota\in J}X_\iota.
$$

特别是，对于所有$x\in I$，我们有

$$
\bigcap_\iota X_\iota\subset X_x.
$$

相反，如果 $Y\subset X_\iota$ 对于所有 $\iota\in I$，则

$$
Y\subset\bigcap_\iota X_\iota.
$$

更一般地，如果$(Y_i)$是E的子集的另一个族，由相同的集合I索引，并且如果$X_i\subset Y_i$对于所有$i\in I$，则

$$\bigcap_{i}X_i\subset\bigcap_iY_i.$$

集合$X_i$的并是所有集合$Y$的交，这样$X_i\subset Y$对于所有$i\in I$。 $X_i$的交是所有$Z$的并，这样$Z\subset X_i$对于所有$i\in I$。

以下公式分别是 (35) 和 (37) 的对偶：

(41)

$$\bigcap_{i\in\bigcup_{\lambda\in L}J_\lambda}X_i=\bigcap_{\lambda\in L}\left(\bigcap_{i\in J_\lambda}X_i\right)\qquad\text{(associativity)};$$

(42)

$$\left(\bigcap_{i\in I}X_i\right)\cup\left(\bigcap_{x\in K}Y_x\right)=\bigcap_{(i,x)\in I\times K}(X_i\cup Y_x)\qquad\text{(distributivity)}.$$

如果$(X_i)_{i\in I}$是E的子集族，并且$(Y_x)_{x\in K}$是F的子集族，那么

(43)

$$\left(\bigcap_{i\in I}X_i\right)\times\left(\bigcap_{x\in K}Y_x\right)=\bigcap_{(i,x)\in I\times K}(X_i\times Y_x).$$

此外，如果$(X_i)$和$(Y_i)$分别是E和F的子集族，并由相同的集合I索引，则

(44)

$$\left(\bigcap_{i\in I}X_i\right)\times\left(\bigcap_{i\in I}Y_i\right)=\bigcap_{i\in I}(X_i\times Y_i).$$

公式(34)没有对偶；总的来说，我们只能说

(45)

$$K\left(\bigcap_{i\in J}X_i\right)\subset\bigcap_{i\in J}K(X_i).$$

仅当$X\mapsto K(X)$是F的子集的映射到E的逆扩张时，我们在(45)中才有等式，对于所有族$(X_i)$。因而，如果$f$是F到E的映射，我们有（推广（14））

(46)

$$\overline{f}^{\, -1}\left(\bigcap_{i\in J}X_i\right)=\bigcap_{i\in J}\overline{f}^{\, -1}(X_i).$$

9. 令 E 为任意集合，令 I 为任意指标集合。 E 的所有元素族 $(x_i)_{i\in I}$ 的集合，索引为 I，用 $E^I$ 表示，从 E 到 $E^I$ 的运算称为求幂。因而，通过考虑这些映射的图，$E^I$与I到E的所有映射的集合一一对应（由于这个原因，由于滥用语言，通常用$E^I$表示），并且与$\mathfrak{P}(I \times E)$的子集一一对应。 因而，集合 I 的集合 $E^J$ 相应的至子集 $J$ 可以被视为全部为相同集合的子集，其与对应与子集是一一对应的。 $\mathfrak{P}(I \times E)$。

现在让$(X_\ell)_{\ell\in I}$是E的子集*的*族，由相同的集合I索引，并让J是I的任何子集。 性质“对于$(x_\ell)_{\ell\in J}$定义子集家族$E^J$的所有$\ell\in J$、$x_\ell\in X_\ell$”，称为集合*$(X_\ell)_{\ell\in J}$家族的*乘积，并用$\displaystyle\prod_{\ell\in J} X_\ell$表示（或者当 $J=I$ 时简单地 $\displaystyle\prod_\ell X_\ell$）。 $X_\ell$称为乘积的*因子*。请注意，$\displaystyle\prod_{\ell\in\varnothing} X_\ell$ 是元素的集合由……组成（相应的到$I\times E$ 的空子集）。如果 $X_\ell=E$ 对于所有 $\ell\in J$，那么我们有

$$
\prod_{\ell\in J} X_\ell=E^J.
$$

例如，如果 I 由三个数 1、2、3 组成，则 $\displaystyle\prod_{\ell\in J} X_\ell$ 与集合 $X_1\times X_2\times X_3$ 是一对一的对应。

10. 如果 $R\{x,y\}$ 是集合 E 的泛型元素 $x$ 和集合 F 的泛型元素 $y$ 之间的关系，则以下命题 *等效*：

“对于每个$x$，都存在$y$，使得$R\{x,y\}$”

和

“存在 E 到 F 的映射 $f$，使得 $R\{x,f(x)\}$ 对于所有 $x$”。

这个等价的断言被称为*选择*公理（或*Zermelo公理*）。我们将有时指出证明或定理是否依赖于它。

选择的公理“等价”于以下命题：“如果对于每个 $\ell\in I$，我们有 $X_\ell\ne\varnothing$，则$\displaystyle\prod_{\ell\in I}X_\ell\ne\varnothing$”。

11. 在这个和接下来的小节中，我们将考虑非空乘积$\displaystyle\prod_{\ell\in I}A_\ell$，其中$(A_\ell)$是E的（非空）子集的任何*家族*。

令 J 为 I 的子集。 $\displaystyle\prod_{\ell\in I}A_\ell$到$\displaystyle\prod_{\ell\in J}A_\ell$的映射$(x_\ell)_{\ell\in I}\to(x_\ell)_{\ell\in J}$称为$\displaystyle\prod_{\ell\in I}A_\ell$到$\displaystyle\prod_{\ell\in J}A_\ell$的*投影*，记为$\operatorname{pr}_J$。

特别地，$\displaystyle\prod_{\ell\in I}A_\ell$到$A_\kappa$的映射$(x_\ell)_{\ell\in I}\to x_\kappa$称为*指标*$\kappa$的*坐标函数*（或*投影*），并用$\operatorname{pr}_\kappa$表示。

如果$z$是$\displaystyle\prod_{\ell\in I}A_\ell$的元素，我们有$z=(\operatorname{pr}_\ell z)_{\ell\in I}$。

设$J_1, J_2$是两个集合，形成$I$的划分。那么$z\mapsto(\operatorname{pr}_{J_1}z,\operatorname{pr}_{J_2}z)$是$\prod_{i\in I}A_i$到$\prod_{i\in J_1}A_i\times\prod_{i\in J_2}A_i$的一对一的映射。

一般来说，如果$(J_\lambda)_{\lambda\in L}$是集合$I$中的任何划分，则映射$z\mapsto(\operatorname{pr}_{J_\lambda}z)_{\lambda\in L}$是$\prod_{i\in I}A_i$到乘积$\prod_{\lambda\in L}(\prod_{i\in J_\lambda}A_i)$的双射（称为规范）。这也可以用说来表示，集族的积是结合律。

12. 以下命题概括了§3, no. 3； $(X_i)$、$(Y_i)$表示$E$的子集族，使得$X_i\subset A_i$和$Y_i\subset A_i$，对于所有$i\in I$； $Z$表示$\prod A_i$中的任意子集。

(a) 如果$\prod_iX_i\neq\varnothing$,关系“$\prod_iX_i\subset\prod_iY_i$”相当于“对于所有$i\in I$,$X_i\subset Y_i$”。

(b) 我们有$\operatorname{pr}_x^{-1}(X_x)=\prod_iY_i$，其中只要$i\neq x$就有$Y_x=X_x$和$Y_i=A_i$。因此

$$
\prod_{i\in I}X_i=\bigcap_{i\in I}\operatorname{pr}_i^{-1}(X_i).
$$

(c) 如果 $\prod_iX_i\neq\varnothing$，则

$$
\operatorname{pr}_x\left(\prod_iX_i\right)=X_x.
$$

(d) 对于所有$Z$，我们有

$$
Z\subset\prod_i\operatorname{pr}_i(Z).
$$

(e) 令$(J_1,J_2)$为$I$的划分分成两个集合，令$(a_i)_{i\in J_1}$为$E$的元素的族，并令$(X_i)_{i\in J_2}$为$E$的子集的族，使得$a_i\in A_i$适用于所有$i\in J_1$，$X_i\subset A_i$适用于所有$i\in J_2$。然后乘积$\prod_iY_i$，其中当$i\in J_1$时为$Y_i=\{a_i\}$，当$i\in J_2$时为$Y_i=X_i$，可以通过投影到后者集合上将对应与$\prod_{i\in J_2}X_i$一一对应。

13. 令$(A_i)_{i\in I}$为集合$F$的子集的族，并令$f$为集合$E$的映射进入乘积$\prod_iA_i$。如果我们把$f_i(x)=\operatorname{pr}_i(f(x))$，那么$f_i$就是$E$的映射放入$A_i$，$f$就是映射$x\mapsto(f_i(x))$。相反，如果对于每个指标$i\in I$，$f_i$是$E$的映射到$A_i$，那么

$$
x\mapsto(f_i(x))
$$

是E的映射变成$\prod_{i\in I} A_i$，用$(f_i)$表示（滥用语言，因为这个记号已经表示映射$f_i$的家族）。因此，我们将集合$(\prod_{i\in I} A_i)^E$的定义双射（称为规范）转换为集合$\prod_{i\in I}(A_i^E)$。

14.设E、F、G为三个集合。对于$F \times G$到$E$的每个映射$f$和每个$y\in G$，令$f_y$表示$F$到$E$的部分映射$x\mapsto f(x,y)$。那么$y\mapsto f_y$就是$G$的映射到$E^F$。相反，对于$G$到$E^F$的每个映射$g$，都存在$F\times G$到$E$的唯一映射$f$，这样对于所有$y\in G$都有$f_y=g(y)$。因此，我们将集合$E^{F\times G}$的定义双射（称为规范）转换为集合$(E^F)^G$。

15. 设$(A_i)_{i\in I}$为集合E的非空子集族。对于每个$i\in I$，令$f_i$为$A_i$的映射到集合F，这样，对于每个对指标 $(i,x)$、$f_i$ 和 $f_x$ 同意$A_i\cap A_x$。那么，如果

$$
A=\bigcup_{i\in I}A_i,
$$

存在 A 到 F 的唯一映射 $f$，使得 $f$ 到每个 $A_i$ 的限制等于 $f_i$。特别是，如果 $A_i\cap A_x=\varnothing$ 每当 $i\ne x$ 时，我们会看到集合 $F^A$ 和 $\prod_{i\in I}F^{A_i}$ 是一对一的对应（称为规范）。
