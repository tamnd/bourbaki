---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Semisimple Modules and Rings
section: 4
section_title: Trace of an Endomorphism of Finite Rank
appendix: true
lang: zh
source: alg-viii
source_edition: 2023, Springer Nature
book_pages: A VIII.463-A VIII.467
pdf_pages: 0480-0484
extraction: native
subsections:
    - "no": 1
      title: Linear Mappings of Finite Rank
      page: 463
      pdf_page: 480
    - "no": 2
      title: Trace of an Endomorphism of Finite Rank
      page: 464
      pdf_page: 481
statements: 5
exercises: 2
content_sha256: 0ba269d90a91d67171d782dc026ea59bcf6612c67c95378de155f7bf78318aa6
translated_from: content/en/alg/VIII/A4_a4_trace_of_an_endomorphism_of_finite_rank.md
translation_method: google
source_content_sha256: b21c8fa64810e183438c648b465f555368181eb6b34b8b9afdc829259a3d239d
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-50f48bb3
glossary_version: 34
glossary_terms_sha256: 746a03d70aef6f87a26cd9c519fe35acfd2719cfcd6352613465818eea9242da
prompt_sha256: 77d1eb2d7fcbd90aea4f1a996022f1b3908ace921dc0bfaa5df62ffc2d1f67a6
---

## 附录 4 自同态有限秩的痕迹

### 1. 线性映射 / 有限秩

令A为环，令E和F为A-模。我们用从E到F的线性映射的Hom$^f_A(E,F)$集合来表示，其中像包含在F的有限生成的子模中。它是Hom$_A(E,F)$的子群。当A为域时，从有限秩的E到F为线性映射的集合(II, §7, No. 4、p. 298、定义3)。 集合结束$^f_A(E) =$坎$^f_A(E,E)$。

令$E,F,G$为A-模，令$u: E\rightarrow F$和$v: F\rightarrow G$为A-线性映射。如果$u\in$Hom$^f_A(E,F)$或$v\in$Hom$^f_A(F,G)$，则$v\circ u$属于到Hom$^f_A(E,G)$。

用$\theta$表示从$E^*\otimes_AF$到Hom$_A(E,F)$的规范群同态（II, §4, No. 2，p. 271）；它将$E^*\otimes_AF$中的元素$x^*\otimes y$从E发送到映射$x\mapsto  \langle x, x^*\rangle y$到F。

#### 引理 1 {#alg-viii-a4-lem-1 .statement tag=00QO}

假设 A-模 F 是射影的。 群同态 $\theta$ 是单射，它的像是 Hom$^f_A(E,F)$。

按地点。引言，推论，同态$\theta$是单射的。它的像包含在Hom$^f_A(E,F)$中。让$u\in$坎$^f_A(E,F)$；让我们证明$\theta$的$u$属于到像。

首先，假设 A-模 F 是免费的。令$(f_i)_{i\in I}$为F的基，并令$(f_i^*)_{i\in I}$为$F^*$对$(f_i)_{i\in I}$的基。令J为I的有限子集，使得$u$的像包含在由$j\in J$的$f_j$生成的F的子模中。我们有

$$
u(x) =\sum_{j\in J}\langle u(x), f_j^*\rangle f_j=\sum_{j\in J}\langle x,^tu(f_j^*)\rangle f_j \tag{1}
$$

对于每 $x\in E$，因此

$$
u=\theta (\sum_{j\in J}^tu(f_j^*)\otimes f_j) \tag{2}
$$

一般情况下，存在自由A-模L和同态$i: F\rightarrow L$和$p: L\rightarrow F$使得$p\circ i= 1_F$。 同态$i\circ u$属于到霍姆$^f_A(E,L)$。通过上述，存在有限的集合 J，并且对于每个$j\in J$，$E^*$的元素$x^*_j$和L的$y_j$这样我们有

$$
i(u(x)) =\sum_{j\in J}\langle x, x^*_j\rangle y_j
$$

每$x\in E$。然后我们有

$$
u(x) =p(i(u(x))) =\sum_{j\in J}\langle x, x^*_j\rangle p(y_j)
$$

每 $x\in E$，因此 $u=\theta (\sum_{j\in J}x^*_j\otimes p(y_j))$。

### 2. 有限秩自同态的痕迹

在这个小节中，A表示交换环。令 E 为射影 A-模。那么End$^f_A(E)$就是End$_A$(E)的A-子模，从$E^*\otimes_AE$到End$^f_A(E)$，End$_A(E)$定义同构$\theta_E$是A-模的典范映射$E^*\otimes_AE\rightarrow$ （引理1）。考虑以公式 $\tau (x^*\otimes x) =\langle x, x^*\rangle$ 为特征的规范线性形式 $\tau : E^*\otimes_AE\rightarrow A$ (II, §4, No. 3, p. 273)。与同构$\theta^{-1}_E$合成，可推导出线性形式Tr：End$^f_A(E)\rightarrow A$，称为踪迹形式。当A-模 E 有限生成时，我们恢复II, §4, No. 3、p. 273 的定义。

#### 命题 1 {#alg-viii-a4-prop-1 .statement tag=00QP}

令 E 为自由A-模。令$(e_i)_{i\in I}$为E的基，并令$(e^*_i)_{i\in I}$为其对偶基。让$u\in$结束$^f_A(E)$。族$(\langle u(e_i), e^*_i\rangle )_{i\in I}$有有限支撑，其和等于Tr($u$)。

只要处理$u$为形式$\theta_E(x^*\otimes x)$以及$x\in E$和$x^*\in E^*$的情况就足够了。那么家庭$(\langle x, e^*_i\rangle )_{i\in I}$就有有限支撑，我们有$x=\sum_{i\in I}\langle x, e^*_i\rangle e_i$。因而，家庭$(\langle x, e^*_i\rangle \langle e_i, x^*\rangle )_{i\in I}$也有有限支撑，我们有$\langle x, x^*\rangle =\sum_{i\in I}\langle x, e^*_i\rangle \langle e_i, x^*\rangle$。现在，每 $i\in I$ 就有 $\langle u(e_i), e^*_i\rangle =\langle x, e^*_i\rangle \langle e_i, x^*\rangle$。这就证明了命题。

#### 命题 2 {#alg-viii-a4-prop-2 .statement tag=00QQ}

令 E, F 为射影 A-模。设$u\in$Hom$^f_A(E,F)$和$v\in$Hom$_A(F,E)$。我们有关系

(3) Tr($v\circ u$)$=$Tr($u\circ v$)。

当$u$是形式$\theta (x^*\otimes y)$以及$x^*\in E^*$和$y\in F$时，证明命题就足够了。在这种情况下，我们有

$v\circ u=\theta_E(x^*\otimes v(y))$ 和 $u\circ v=\theta_F(^tv(x^*)\otimes y)$,

因而

Tr($v\circ u$)$=\langle v(y), x^*\rangle =\langle y,^tv(x^*)\rangle =$Tr($u\circ v$)。

#### 推出{#alg-viii-a4-n2-cor-1 .statement tag=00QR}

Let E be a projective A-module, $u$ be an element of End$^f_A(E)$, and F be a projective A-submodule of E containing Im $u$. 用$u$诱导的F的$u_F$自同态表示。 我们有

(4) Tr($u$)$=$Tr($u_F$)。

用F到E中的$i$典范嵌入表示，并用从$u$推导出来的$v: E\rightarrow F$同态表示。我们有$u_F=v\circ i$和$u=i\circ v$。推论如下。

令 E 为射影 A-模和 $u\in$ End$^f_A(E)$。对于每个自然数$p$，A-模$\wedge^pE$都是投影（III, §7, No. 8，p. 519，推论2），并且自同态$\wedge^pu$属于到End$^f_A(\wedge^pE)$（III, §7, No. 3， p. 511、命题 6)，$p$ 足够大为零。 集合$1_E+$End$^f_A(E)$稳定在合成以下。我们定义映射从$1_E+$结束$^f_A(E)$出发设定到达A

检测（1$_E+u$）$=\sum_{p\geqslant 0}$Tr$\wedge^pu$

$u\in$结束$^f_A(E)$。

如果 E 是自由且有限维的，则根据 III, §8, No. 5、p. 530 的推论，该定义与 III, §8, No. 1、p. 522 一致。

#### 命题 3 {#alg-viii-a4-prop-3 .statement tag=00QS}

令 E 为射影 A-模。

a) 让$u\in$结束$^f_A(E)$。令 F 为 E 包含于 Im $u$ 的投影 A-子模，并令 $u_F$ 为由 $u$ 导出的 F 的自同态。我们有

（5）det（1$_E+u$）$=$det（1$_F+u_F$）。

b) 令$u$和$v$为End$^f_A(E)$的两个元素。我们有

(6) 检测$(1_E+u)\circ (1_E+v)$ = 检测(1$_E+u$) 检测(1$_E+v$)。

让我们证明a）。对于每个整数$p\geqslant 0$，射影A-模$\wedge^pF$可以用$\wedge^pE$的子模来识别（III, §7, No. 9，p. 520，推论）。 $\wedge^pu$的像包含在$\wedge^pF$中，由$\wedge^pu$诱发的$\wedge^pF$的自同态等于$\wedge^pu_F$。因而，根据命题 2 的推论，我们有 Tr($\wedge^pu$) $=$ Tr($\wedge^pu_F$)，因而 a)。

让我们证明b)。令 G 为 A-模，使得 A-模 $L = E\oplus G$ 是自由的。用L的$u'$和$v'$、自同态、$u\oplus 0_G$和$v\oplus 0_G$表示。通过 a)，我们有关系 det(1$_L+u'$) $=$ det(1$_E+u$)，det(1$_L+v'$) $=$ det(1$_E+v$)，并且

检测（1$_L+u'+v'+u'\circ v'$）$=$ 检测（1$_E+u+v+u\circ v$）。

因此，当A-模 E 自由时，证明断言 b) 就足够了。那么存在有限生成的 E 的自由子模 F，即 $u$ 的包含像和$v$ 的包含像。 集合$w=u+v+u\circ v$。 $w$的像包含在F中，我们有$w_F=u_F+v_F+u_F\circ v_F$。因此，根据 (5)，我们有 det(1$_E+u$) $=$ det(1$_F+u_F$)、det(1$_E+v$) $=$ det(1$_F+v_F$)，以及

检测$((1_E+u)\circ (1_E+v))$

= det(1$_E+w$) $=$ det(1$_F+w_F$) $=$ det((1$_F+u_F$)$\circ (1_F+v_F)$)。

由于 F 是有限生成的自由A-模，所以我们有

det((1$_F+u_F$)$\circ (1_F+v_F)$) $=$ det(1$_F+u_F$) det(1$_F+v_F$) $=$ det(1$_E+u$) det(1$_E+v$)。

### 习题 {#alg-viii-a4-exercises}

参见[习题附录 4](exercises/a4/)。
