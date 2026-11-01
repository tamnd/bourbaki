---
book: ens
book_title: Theory of Sets
chapter: ER
chapter_title: SUMMARY OF RESULTS
section: 5
section_title: Equivalence relations and quotient sets
lang: zh
source: ens-i-iv
source_edition: 2004, Springer
book_pages: 370-373
pdf_pages: 0375-0378
extraction: ocr
statements: 0
exercises: 0
content_sha256: a9e8d258324b6e5d3c7503548fddd116fb74498464031ee4674a24cd9d13e361
translated_from: content/en/ens/ER/05_s5_equivalence_relations_and_quotient_sets.md
translation_method: google
source_content_sha256: de7dfd40c6cfa021011ad6534250a579d1efe1882e81ad993bcb4259f6eb1c68
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-50f48bb3
glossary_version: 34
glossary_terms_sha256: e4ed284e58b906f07b2b0b07337d8624f58f9c7607c88ade7d8cf660a8568982
prompt_sha256: 77d1eb2d7fcbd90aea4f1a996022f1b3908ace921dc0bfaa5df62ffc2d1f67a6
---

## 5. 等价关系和商集

1. 令$(A_i)_{i\in I}$为集合E的划分。关系$R\{x,y\}$：“存在$i\in I$使得$x\in A_i$和$y\in A_i$”，E的两个泛型元素$x,y$之间满足以下条件 ：

(a) $R\{x,x\}$ 是恒等式（R 的自反性）。

(b) $R\{x,y\}$ 和 $R\{y,x\}$ 等价（R 对称）。

(c) 关系$R\{x,y\}$和$R\{y,z\}$意味着$R\{x,z\}$（R的传递性）。

若C表示由关系R定义的$E\times E$的子集，则条件(a)、(b)、(c)分别等价于以下条件：$(a')\ \Delta\subset C$； $(b')\ \overline{C}=C$； $(c')\ C\circ C\subset C$。从$(a')$和$(c')$得出$C\circ C=C$。

2. 相反，令$R\{x,y\}$为自反、对称且传递的关系，并令C为其在$E\times E$中的图。那么E的映射$x\mapsto C(x)$到$\mathfrak{P}(E)$下的E的像$\mathfrak{F}$是E的划分，并且关系“存在子集Xε$\mathfrak{F}$使得xX并且y ∈ X” 等价于
$R\{x,y\}$。

每个满足条件 (a)、(b) 和 (c) 的关系在 E 上称为等价关系。 划分 $\mathfrak{F}$，其中定义，被视为 $\mathscr{P}(E)$ 的子集，在 E 上被关系称为商集 R，用E/R表示；它的元素相对于R被称为等价类。E到E/R的映射$x \mapsto C(x)$，其中映射E到等价类的每个元素x，其中包含x被称为E到E/R的典范映射。

等式$x = y$的关系是等价关系。 E 到相应的商集的典范映射就是 $x \mapsto \{x\}$，并且是双射的。

若R为等价关系，则记号“$x \equiv y$(mod R)”为有时，用作$R\{x,y\}$的同义词；读作“x 等于 y 模 R”。

3. 在乘积集合$E \times F$上，关系z和z′之间的“$\operatorname{pr}_1 z = \operatorname{pr}_1 z'$”是等价关系R，商集$(E \times F)/R$可以与E一一对应对应（这就是商集名字的由来）。

更一般地，令 f 为集合 E 到集合 F 中的映射。那么关系“$f(x)=f(y)$”就是 E 上的等价关系。如果我们用 R 表示这个关系，则映射 $z \mapsto f^{-1}(z)$（其中 $f^{-1}(z)$ 被认为是E/R 的元素) 是 E/R 上的 $f(E)$ 的双射。

由此可见，在给定的序中，f可以被视为以下三个映射中的合成：
(1) 将F的子集$f(E)$中的典范映射化为集合F；
(2) E/R 到 $f(E)$ 的双射映射，其逆矩阵刚刚定义；
(3) E 的典范映射到 E/R。

映射的这个分解称为其规范分解或规范因式分解。

4. 集合 E 上的每个等价关系 R 都可以如前面的小节那样通过映射来定义；因为，如果C是R的图，关系“$C(x)=C(y)$”等价于$R\{x,y\}$。

5. 令R为集合 E上的等价关系，并令A为E的子集。则A的两个泛型元素 x, y之间的关系$R\{x,y\}$为A上的等价关系，称为由R在A上诱导的关系，表示为$R_A$。令f为E到E/R的典范映射，并令g为A到$A/R_A$的典范映射。通过使E/R的元素和$A/R_A$对应的元素分别为f和g下E的相同元素的像，我们在f和g下A的像$f(A)$之间有一个一对一的对应， 商集$A/R_A$。如果 φ 表示 A 到 E 的典范映射，则这个对应由映射 $z \to f(\varphi(g^{-1}(z)))$ 及其逆来实现，两者也称为*规范*。

6. 如果对于 R 的 $x$ 的每个 $x \in A$ 等价类都包含在 A 中，则 E 的子集 A 相对于等价关系 R 被称为“饱和”。在其他字中，关于 R 的饱和集合是等价类的 *并，其中尊重 R*。如果$f$是E到E/R上的典范映射，则集合是饱和的，如果它是形式$f^{-1}(X)$，其中$X \subset E/R$。

令A为E的子集。饱和集合的交，其中包含A为$f^{-1}(f(A))$。这个集合也可以被定义为A的等价类或元素的并，并且被称为A的*饱和度*（相对于R）。

7. 设$P\{x,y,z\}$为关系，其中出现E的泛型元素$x$。则称P与等价关系*R*相容的*（在$x$中）*与等价关系*R，如果关系“$P\{x,y,z\}$和$x \equiv x'$（mod R）”*意味着* $P\{x',y,z\}$。

令$f$为E到E/R的典范映射，并令$t$为E/R的泛型元素。 关系“存在$x \in f^{-1}(t)$使得$P\{x,y,z\}$”相当于“对于所有$x \in f^{-1}(t)$，$P\{x,y,z\}$”；后者是 $t$、$y$、$z$ 之间的关系，据说是由 P *在经过上“诱导”得到商*（相对于 $x$）。如果我们用$P'\{t,y,z\}$表示，那么$P\{x,y,z\}$就相当于$P'\{f(x),y,z\}$。

对于涉及任何数参数的关系，以及关系在 *几个* 参数中与 R 兼容的情况，都有类似的定义。对于例，如果A是E的子集，则说关系“$x \in A$”与R兼容（在$x$中）相当于说，A相对于R是饱和的。如果$\varphi$是E的映射， 集合 F，说泛函关系“$y=\varphi(x)$”与 R 相容的（在 $x$ 中），就是说 $\varphi$ 在每个等价类上相对于 R 是恒定的。 经过为商，R 因此诱导关系之间$y$ 和 E/R 的通用元素 $t$；这个关系在$y$中起作用，因此E/R的确定映射$\varphi'$进入F，满足身份$\varphi(x)=\varphi'(f(x))$。

8. 设 R 为集合 E 上的等价关系，设 S 为集合 F 上的等价关系，并设 $f$ 为 E 到 F 的映射。 如果关系，映射 $f$ 被认为与 R 和 S* 相容的$x \equiv x'$ (mod R) *意味着* $f(x) \equiv f(x')$ (mod S)。如果$g$是F到F/S上的典范映射，则复合函数$g \circ f$对于R而言在等价类$z$的所有元素具有相同的值；如果我们用$h(z)$表示这个公共的值，那么$h$是E/R到F/S的映射，并且据说是*由f在经过上引出的商*。

9. 令 E 上的 R 为等价关系，并令 E/R 上的 S 为等价关系。如果$f$是E到E/R的典范映射，则“$f(x)\equiv f(y)\pmod S$”是E上的等价关系T。因此，相对于T的等价类相对于R是等价类的E中的并，它们相对于S彼此相等； 关系“$x\equiv y\pmod R$”意味着“$x\equiv y\pmod T$”。如果$g$和$\varphi$分别是$E$的典范映射到$E/R$和$E/T$，我们通过以下方式获得$(E/R)/S$和$E/T$之间的一对一的对应（称为规范） $(E/R)/S$的元素和$E/T$对应的元素彼此，如果它们分别是$g$和$\varphi$下E的相同元素的像。

相反，让 R 和 T 是 E 上的两个等价关系，这样“$x\equiv y\pmod R$”意味着“$x\equiv y\pmod T$”。那么 T 在 x 和 y 上都与 R 相容的（在no. 7的意义上）；通过经过商 $E/R$（相对于 x 和 y），T 诱导等价关系 S 在 $E/R$ 上。如果$\varphi$再次将E的典范映射表示到$E/R$上，则关系“$\varphi(x)=\varphi(y)\pmod S$”相当于“$x\equiv y\pmod T$”。 等价关系 S称为T与R的商，记为T/R。从上一段我们看到，$(E/R)/(T/R)$和$E/T$之间存在一对一的对应（规范的对应）。

10. 现在令 E、F 为任意两个集合，它们可能不同，也可能不同。设E上的$\{x, y\}$为等价关系，F上的$\{z, t\}$为等价关系。然后关系$\{x, y\}\times\{z, t\}$在元素$(x,z)$和$(y,t)$之间乘积集合 $E\times F$是$E\times F$上的等价关系，用S称为R的乘积，记为$R\times S$。每个$R\times S$的等价类对于R来说是等价类的乘积，对于S来说是等价类。如果u表示$E/R$的泛型元素，而v表示$F/S$的泛型元素，则$(u,v)\mapsto u\times v$ 是 $(E/R)\times(F/S)$ 到 $(E\times F)/(R\times S)$ 的双射（称为规范）。
