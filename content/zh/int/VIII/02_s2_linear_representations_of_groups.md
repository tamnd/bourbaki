---
book: int
book_title: Integration
chapter: VIII
chapter_title: CONVOLUTION AND REPRESENTATIONS
section: 2
section_title: Linear representations of groups
lang: zh
source: int-vii-ix
book_pages: INT VIII.8-INT VIII.17
pdf_pages: 0108-0117, 0159-0161
extraction: ocr
subsections:
    - "no": 1
      title: Continuous linear representations
      page: 8
      pdf_page: 108
    - "no": 2
      title: Contragredient representation
      page: 10
      pdf_page: 110
    - "no": 3
      title: 'Example: linear representations in spaces of continuous functions'
      page: 11
      pdf_page: 111
    - "no": 4
      title: 'Example: linear representations in spaces of measures'
      page: 12
      pdf_page: 112
    - "no": 5
      title: 'Example: linear representations in the spaces $L^p$'
      page: 13
      pdf_page: 113
    - "no": 6
      title: Extension of a linear representation of $G$ to the measures on $G$
      page: 15
      pdf_page: 115
    - "no": 7
      title: Relations between the endomorphisms $U(\mu)$ and the endomorphisms $U(s)$
      page: 16
      pdf_page: 116
statements: 22
exercises: 10
content_sha256: 7e23f5298ea5c2470c0166b0fb25e2160f402255b5ac5a4fdf78503ca9052cc4
translated_from: content/en/int/VIII/02_s2_linear_representations_of_groups.md
translation_method: google
source_content_sha256: 5dafa58e78dc6307341df4bd75bf3a56cc18775819c83933d0c50e69c45de801
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-50f48bb3
glossary_version: 34
glossary_terms_sha256: 19a47299c2324d4f490ee85fb62da01a67d499f1149a6bcd6b08f930c2e9a48a
prompt_sha256: 77d1eb2d7fcbd90aea4f1a996022f1b3908ace921dc0bfaa5df62ffc2d1f67a6
---

## § 2。 线性表示群

### 1. 连续线性表示

设 G 为拓扑群，E 为 E 中 G 的局部凸空间，U 线性表示。

#### 定义 1 {#int-viii-s2-def-1 .statement tag=09IF}

— (i) 如果对于每个$s \in G$，$U(s)$是$E$的连续自同态，并且如果对于每个$x \in E$，$G$到$E$的映射$s \mapsto U(s)x$是连续的，则称$U$是单独连续的。

(ii) 如果$(s, x) \mapsto U(s)x$是$G \times E$到$E$的连续映射，则称$U$是连续的。

(iii) 如果$U$是连续的，并且如果自同态$U(s)$的集合（其中$s$超过$G$）是等连续的。

#### 注 1 {#int-viii-s2-n1-rem-1 .statement tag=09IG}

说$U$是单独连续意味着$s \mapsto U(s)$是$G$的连续映射到$E$的连续自同态的空间$\mathscr{L}(E; E)$，并配备了逐点收敛的拓扑。

#### 注 2 {#int-viii-s2-n1-rem-2 .statement tag=09IH}

说$U$是连续的，相当于下面的三个条件的集合：

a) 对于每个$s \in G$，$U(s)$是连续的； b) 存在$e$的邻域$V$，使得$U(V)$等连续； c) $E$ 中存在总计集合 $D$，使得对于每个 $x \in D$，映射 $s \mapsto U(s)x$ 是连续的。

这些条件显然是必要的。反之，假设满足条件 a), b), c)。在$U(V)$上，逐点收敛的拓扑与$D$中逐点收敛的拓扑相同（TVS，III, §3, No. 4，命题5）。因此，$V \times E$到$E$的映射$(s, x) \mapsto U(s)x$是连续的（GT，X, §2, No. 1，命题1的Cor.3）。由于 $U(s_0s)x = U(s_0)(U(s)x)$ 对于所有 $s_0 \in G$、$s \in G$、$x \in E$，可以看出 $U$ 是连续的。

当 $G$ 局部紧致时，条件 a) 和 b) 等价于条件：
$a')$对于$G$的每个紧致子集$K$，$U(K)$是等连续的。

#### 注 3 {#int-viii-s2-n1-rem-3 .statement tag=09II}

假设$U$是$G$在$E$中的连续线性表示。对于每个$s \in G$，让$\widehat{U}(s)$是$U(s)$的连续扩张到$E$的完成$\widehat{E}$。那么$\widehat{U}$是$\widehat{E}$、注2的满足条件a)和c)中$G$的线性表示，以及GT、X, §2, No. 2、命题4的条件b)。因此$\widehat{U}$是$\widehat{E}$中$G$的连续线性表示。

#### 注 4 {#int-viii-s2-n1-rem-4 .statement tag=09IJ}

当$E$是规范的空间时，如果每个$s \in G$都有$\|U(s)\| = 1$，则称$U$是等距的。为此，对于所有$s \in G$，$\|U(s)\| \leq 1$就足够了，因为这样就有
$$
1 = \|1\| \leq \|U(s)\| \cdot \|U(s^{-1})\|,
$$
从而 $\|U(s)\| = \|U(s^{-1})\| = 1$ 对于所有 $s \in G$。

#### 命题 1 {#int-viii-s2-prop-1 .statement tag=09IK}

— 如果 $G$ 是局部紧致群并且 $E$ 是桶状的，则 $E$ 中 $G$ 的每个单独连续的线性表示 $U$ 都是连续的。

对于$G$的每个紧致子集$K$，$U(K)$对于逐点收敛的拓扑是紧致的（注1），因此是等连续的（TVS，III, §4, No. 2，Th.1）；然后应用注 2。

#### 引理 1 {#int-viii-s2-lem-1 .statement tag=09IL}

令 G 为 G 上的局部紧致群，$\rho$ 为 G 上的下半连续有限数值函数 $\geqslant 0$，使得 $\rho(st) \leqslant \rho(s)\rho(t)$ 对于所有 $s,t \in G$。那么 $\rho$ 就在 G 的每个紧凑子集上有界。

G 存在非空开子集 U，使得 $\rho$ 在 U 上有界（GT，IX, §5, No. 4，Th.2）。令 K 为 G 的紧致子集。则 K 被集合 $s_1U, \ldots, s_nU$ 的有限数覆盖。对于每个 $x \in U$，都有 $\rho(s_ix) \leqslant \rho(s_i)\rho(x)$，因此 $\rho$ 在 $s_iU$ 上有界，因此在 K 上。

#### 引理 2 {#int-viii-s2-lem-2 .statement tag=09IM}

设 G 为赋范空间 E 中 G 的拓扑群，U 线性表示，A 为 E 的稠密子集。假设对于每个 $s \in G$，$U(s)$ 是连续的，并且对于每个 $x \in A$，$s \mapsto U(s)x$ 是连续的将G的映射代入E。则G上的函数$s \mapsto g(s) = \|U(s)\|$是下半连续且满足$g(st) \leqslant g(s)g(t)$。

设B为E的单位球，则$g(s) = \sup_{x \in B \cap A} \|U(s)x\|$，且各函数$s \mapsto \|U(s)x\|$在G上连续，因此$g$为下半连续。另一方面，

$$
g(st) = \|U(s)U(t)\| \leqslant \|U(s)\| \cdot \|U(t)\| = g(s)g(t).
$$

#### 命题 2 {#int-viii-s2-prop-2 .statement tag=09IN}

令 G 为 G 在赋范空间 E 中的局部紧致群，U 线性表示。令 A 为 E 的稠密子集。假设对于每个 $s \in G$，$U(s)$ 是连续的，并且对于每个 $x \in A$，$s \mapsto U(s)x$ 是连续的将 G 映射化为 E。则 U 是连续的。

因为，$\|U(s)\|$ 在 G 的每个紧凑子集上都以引理 1 和 2 为界，然后应用注 2。

### 2. 反对表示

令 U 为 G 在 E 中的单独连续线性表示。令 E' 为 E 的对偶。映射 $s \mapsto {}^tU(s)$ 是群 $G^0$ 与 G 相对的 E' 中的线性表示；我们可以说，这个表示是U的转置。映射$s \mapsto {}^tU(s^{-1}) = {}^tU(s)^{-1}$是E'中G的线性表示，称为U的反对。

#### 引理 3 {#int-viii-s2-lem-3 .statement tag=09IO}

令X为局部紧致空间，Y和Z拓扑为空间，$\varphi$为Z中$X \times Y$的连续映射，以及Y为Z中的$\varphi_x$映射$y \mapsto \varphi(x,y)$。 空间$\mathscr{C}(Y), \mathscr{C}(Z)$具备紧凑收敛的拓扑，$X \times \mathscr{C}(Z)$到$\mathscr{C}(Y)$的映射$(x,f) \mapsto f \circ \varphi_x$是连续的。

显然，考虑 X 是紧致的情况就足够了。设 $(x_0, f_0) \in X \times \mathscr{C}(Z)$，K 是 Y 的紧凑子集，以及 $\varepsilon > 0$。让$K' = \varphi(X \times K)$。由于$f_0 \circ \varphi$在$X \times K$中一致连续，因此存在$x_0$的邻域W，使得$x \in W$和$y \in K$有$|f_0(\varphi(x,y)) - f_0(\varphi(x_0,y))| \leq \varepsilon$。另一方面，如果对于所有 $z \in K'$ 来说，$f \in \mathscr{C}(Z)$ 是$|f(z) - f_0(z)| \leq \varepsilon$，那么$x \in X, y \in K$ 就会有 $|f(\varphi(x,y)) - f_0(\varphi(x,y))| \leq \varepsilon$，因此 $x \in W, y \in K$ 就有$|f(\varphi(x,y)) - f_0(\varphi(x_0,y))| \leq 2\varepsilon$。 从而引理。

现在让我们回到之前的记号。

#### 命题 3 {#int-viii-s2-prop-3 .statement tag=09IP}

(i) *如果 U 是单独连续的，则当 E' 配备弱拓扑 $\sigma(E', E)$ 时，$^tU$ 是单独连续的。*
(ii) *如果 G 是局部紧致的且 U 是连续的，则当 E' 配备紧致收敛的拓扑时，$^tU$ 是连续的。*

断言 (i) 是直接的。 断言 (ii) 是从引理 3 得出的，其中有人取了 $X = G, Y = Z = E, \varphi(s, x) = U(s)x$。

### 3. 例：连续函数中空间中的线性表示

设 G 是在集合 X 左侧运算的离散群。 $G \times X$ 上的复数函数 $\chi$ 称为 *乘子* 如果

(1) $\chi(e, x) = 1$ 对于所有 $x \in X;$
(2) $\chi(st, x) = \chi(s, tx)\chi(t, x)$ 对于 G 中的所有 $s, t$，$x \in X$。

由此可见

(3) $\chi(t^{-1}, tx)\chi(t, x) = 1$ 全部$t \in G, x \in X,$

特别是 $\chi(t, x) \neq 0$ 对于所有 $t \in G, x \in X$。

对于X上定义的每个复数函数$f$和每个$s \in G$，令$\gamma_\chi(s)f$为X上定义的复数函数

（4）$(\gamma_\chi(s)f)(x) = \chi(s^{-1}, x)f(s^{-1}x)$。

然后 $\gamma_\chi(e)f = f$ 和

$$
\begin{align*}
(\gamma_\chi(s)\gamma_\chi(s')f)(x) &= \chi(s^{-1}, x)(\gamma_\chi(s')f)(s^{-1}x) \\
&= \chi(s^{-1}, x)\chi({s'}^{-1}, s^{-1}x)f({s'}^{-1}s^{-1}x) \\
&= \chi((ss')^{-1}, x))f((ss')^{-1}x) = (\gamma_\chi(ss')f)(x),
\end{align*}
$$

因此 $\gamma_\chi$ * 是 G 的线性表示*。对于 $\chi = 1$，可以恢复自同态 $\gamma(s)$（第 VII, §1, No. 1、公式 (3)）。

现在假设G和X是局部紧致的，G在X上连续运行，并且$\chi$在$G \times X$上连续运行。那么$C(X)$和$K(X)$对于$C(X)$和$K(X)$中G的$\gamma_\chi(s)$、从而线性表示是稳定的，我们将再次表示$\gamma_\chi$。

#### 命题 4 {#int-viii-s2-prop-4 .statement tag=09IQ}

*G在$C(X)$和$K(X)$中的线性表示$\gamma_\chi$是连续的。*

$G \times C(X)$到$G \times C(X)$的映射$(s, f) \mapsto (s, \gamma(s)f)$是连续的（No. 2，引理3）。另一方面，$G \times C(X)$到$C(X)$的映射$(s, f) \mapsto \chi(s, \cdot)f$是连续的；因为，如果 G 中 s 趋向于 $s_0$，则 $\chi(s, \cdot)$ 在 X 的每个紧凑子集上一致趋于 $\chi(s_0, \cdot)$；此外，如果$f$在$C(X)$中趋向于$f_0$，那么$\chi(s, \cdot)f$在X、从而我们的断言的每个紧凑子集上均匀地趋向于$\chi(s_0, \cdot)f_0$。因此G在$C(X)$中的表示$\gamma_\chi$是连续的。

让我们证明 G 在 $K(X)$ 中的表示 $\gamma_\chi$ 是连续的。由于$K(X)$是Banach空间的直极限，它是桶状的（TVS，III, §4, No. 1，命题3的Cor.3），因此只需证明$\gamma_\chi$是单独连续的（No. 1，命题1）。现在，令 H 为 X 的紧凑子集，并令 $s_0 \in G$。令V为G中$s_0$的紧邻域，并令L = VH，其在X中是紧邻。对于每个$f \in K(X, H)$，$\gamma_\chi(s_0)f$的支持度都包含在L中，并且
$$
\sup_{x \in X} |(\gamma_\chi(s_0)f)(x)| \leq \sup_{x \in L} |\chi(s_0^{-1}, x)| \cdot \sup_{x \in X} |f(x)|,
$$
因此$f \mapsto \gamma_\chi(s_0)f$是$K(X, H)$到$K(X, L)$的连续线性映射；由此可见，$f \mapsto \gamma_\chi(s_0)f$ 是 $K(X)$ 自身的连续线性映射（TVS，II, §4, No. 4，命题 5）。另一方面，$K(X, L)$的拓扑是由$C(X)$的拓扑诱发的。已经证明，V到$K(X, L)$的映射$s \mapsto \gamma_\chi(s)f$是连续的。这样就完成了证明，$\gamma_\chi$是单独连续的。

#### 命题 5 {#int-viii-s2-prop-5 .statement tag=09IR}

*假设每个函数$\chi(s, \cdot)$都是有界的。那么$\gamma_\chi$离开$\overline{K(X)}$稳定，并且$\overline{K(X)}$中G的线性表示$\gamma_\chi$是连续的。*

很明显，$\gamma_\chi$使$\overline{K(X)}$稳定，并且每个$\gamma_\chi(s)$在$\overline{K(X)}$中都是连续的。另一方面，对于每个$f \in K(X)$，$s \mapsto \gamma_\chi(s)f$是G到$K(X)$的连续映射和到$\overline{K(X)}$的*更不必说*。因此$\overline{K(X)}$中的表示$\gamma_\chi$是连续的（No. 1，命题2）。

### 4. 例：空间措施中的线性表示

再次令 G 为局部紧致群，在局部紧致空间 X 中在左侧连续运行，并令 $\chi$ 为$G \times X$ 上的*连续* 乘子。 $\mathscr{K}(X)$中的$G$的线性表示$\gamma_\chi$在$\mathscr{M}(X)$中承认一个对立表示，我们将再次用$\gamma_\chi$表示，并由以下公式定义（其中$\mu \in \mathscr{M}(X) , f \in \mathscr{K}(X)$）：

$$
\langle \gamma_\chi(s)\mu, f \rangle = \langle \mu, \gamma_\chi(s^{-1})f \rangle = \langle \chi(s, \cdot) \cdot \mu, \gamma(s^{-1})f \rangle = \langle \gamma(s)(\chi(s, \cdot) \cdot \mu), f \rangle ,
$$

从而

$$
\gamma_\chi(s)\mu = \gamma(s)(\chi(s, \cdot) \cdot \mu) = (\gamma(s)\chi(s, \cdot)) \cdot (\gamma(s)\mu) .
$$

我们注

$$
(\gamma(s)\chi(s, \cdot))(x) = \chi(s, s^{-1}x) .
$$

$\mathscr{C}(X)$中$G$的线性表示$\gamma_\chi$在$X$上的测度的空间$\mathscr{C}'(X)$中承认具有紧支持的表示相矛盾，表示我们再次用$\gamma_\chi$表示； $\mathscr{C}'(X)$自同态$\gamma_\chi(s)$是$\mathscr{M}(X)$自同态$\gamma_\chi(s)$限制。

#### 命题 6 {#int-viii-s2-prop-6 .statement tag=09IS}

*如果在$\mathscr{K}(X)$（或$\mathscr{C}(X)$）的紧凑子集中为$\mathscr{M}(X)$（或$\mathscr{C}'(X)$）配备均匀收敛的拓扑，则$\mathscr{M}(X)$中的$G$的线性表示$\gamma_\chi$ （分别$\mathscr{C}'(X)$）是连续的。*

#### 命题 7 {#int-viii-s2-prop-7 .statement tag=09IT}

*假设每个函数$\chi(s, \cdot)$都是有界的。那么$\gamma_\chi$离开稳定的$\mathscr{M}^1(X)$，并且，如果$\mathscr{M}^1(X)$在$\mathscr{K}(X)$的紧子集中具备一致收敛的拓扑，则$G$的线性表示$\gamma_\chi$在$\mathscr{M}^1(X)$中是连续的。*
这些命题来自 Props。 3、4、5。

### 5. 例：线性表示在空间$L^p$

再次令 $G$ 为局部紧致群，在局部紧致空间 $X$ 的左侧连续操作。令 $\beta$ 成为$X$ 的积极测度，并有支持$X$。让我们假设 $G \times X$ 上存在一个*连续* 函数 $\chi > 0$，这样，对于每个 $s \in G$，

$$
\gamma(s)\beta = \chi(s^{-1}, \cdot) \cdot \beta
$$

（这特别意味着$\beta$在$G$下是准不变的）。 *然后，$\chi$ 是乘子。* 因为，给定 $G$ 中的 $s, t$，有

$$
\gamma(s)\gamma(t)\beta = \gamma(s)(\chi(t^{-1}, \cdot) \cdot \beta) = (\gamma(s)\chi(t^{-1}, \cdot)) \cdot (\gamma(s)\beta)
= (\gamma(s)\chi(t^{-1}, \cdot)) \cdot \chi(s^{-1}, \cdot) \cdot \beta ,
$$
$$
\gamma(st)\beta = \chi(t^{-1}s^{-1}, \cdot) \cdot \beta ,
$$

因而
$$
\chi(t^{-1}, s^{-1}x)\chi(s^{-1}, x) = \chi(t^{-1}s^{-1}, x)
$$
局部$\beta$-几乎无处不在，因此无处不在，因为$\chi$是连续的并且$\beta$有支持$X$。

让$p \in [1, +\infty[$。对于每个$f \in \mathscr{L}_C^p(X, \beta)$和每个$s \in G$，令$\gamma_{\chi,p}(s)f$在$X$上为函数，定义为
$$
(\gamma_{\chi,p}(s)f)(x) = \chi(s^{-1}, x)^{1/p} f(s^{-1}x).
$$
一个有
$$
\int^* |\chi(s^{-1}, x)^{1/p} f(s^{-1}x)|^p d\beta(x) = \int^* |f(s^{-1}x)|^p \chi(s^{-1}, x) d\beta(x)
$$
$$
= \int |f(x)|^p d\beta(x),
$$
因此$\gamma_{\chi,p}(s)f \in \mathscr{L}_C^p(X, \beta)$。我们可以看到，$\gamma_{\chi,p}(s)$是$\mathscr{L}_C^p(X, \beta)$和定义的*等距*自同态，通过商，$L_C^p(X, \beta)$的等距自同态，也表示为$\gamma_{\chi,p}(s)$。另一方面，$\chi^{1/p}$显然是乘子，因此根据我们在No. 3中看到的，$\gamma_{\chi,p}$是$L_C^p(X, \beta)$中$G$的线性表示。

#### 命题 8 {#int-viii-s2-prop-8 .statement tag=09IU}

*$L_C^p(X, \beta)$中$G$的线性表示$\gamma_{\chi,p}$是连续且等距的。*

让$f \in \mathscr{K}(X)$。当$s$在$G$中趋向于$s_0$时，$\gamma_{\chi,p}(s)f$在$\mathscr{K}(X)$中趋于$\gamma_{\chi,p}(s_0)f$，因此在$L_C^p(X, \beta)$中。由于$\gamma_{\chi,p}(s)$是等距的，因此命题8是由No. 1的应用 *注 2*得到的。

对于$\chi$不假设连续的情况，cf.§4，Exer。 13.

#### 命题 9 {#int-viii-s2-prop-9 .statement tag=09IV}

*假设每个函数 $\chi(s, \cdot)$ 都是有界的。那么$\gamma_\chi$离开$L_C^p(X, \beta)$稳定，$L_C^p(X, \beta)$中$G$的线性表示$\gamma_\chi$是连续的。*

让$f \in \mathscr{L}_C^p(X, \beta)$。然后
$$
\int^* |\chi(s^{-1}, x)f(s^{-1}x)|^p d\beta(x)
$$
$$
\leq \sup_{x \in X} \chi(s^{-1}, x)^{p-1} \int^* |f(s^{-1}x)|^p \chi(s^{-1}, x) d\beta(x)
$$
$$
= \sup_{x \in X} \chi(s^{-1}, x)^{p-1} \int |f(x)|^p d\beta(x),
$$
因此$\gamma_\chi(s)f \in \mathscr{L}_C^p(X, \beta)$，并且
$$
\| \gamma_\chi(s) \| \leq \sup_{x \in X} \chi(s^{-1}, x)^{1/q},
$$
(5) 其中$q$表示指数共轭至$p$。如果$f \in \mathscr{K}(X)$，则$\gamma_{\chi}(s)f$在$\mathscr{K}(X)$中趋向于$\gamma_{\chi}(s_0)f$，因此在$\mathscr{L}_C^p(X, \beta)$中，因为$s$趋于$s_0$。因此$L_C^p(X, \beta)$中$G$的表示$\gamma_{\chi}$是连续的（No. 1，命题2）。

如果$G$在$X$的右边运算，则与第3、4、5项类似的性质成立。

特别地，如果将$G$视为通过左或右平移对自身进行操作，并且如果取$\chi = 1$，则获得$\mathscr{C}(G)$、$\mathscr{K}(G)$、$\overline{\mathscr{K}}(G)$、$\mathscr{C}'(G)$、$\mathscr{M}(G)$中$G$的*左*和*右正则表示*， $\mathscr{M}^1(G)$。如果将$\beta$作为$G$的左（或右）Haar测度，并且如果将$\chi = 1$取，则获得$L_C^p(G, \beta)$中$G$的*左*（或*右*）*正则表示*。

### 6. $G$线性表示扩张至$G$措施

令$G$是群的局部紧致群，$E$是$E$中$G$的局部凸空间，$U$线性表示。假设$U$是连续的并且$E$是准完备的。然后，对于每一个度量 $\mu \in \mathscr{C}'(G)$，都有

$$
\int_G U(s)\, d\mu(s) \in \mathscr{L}(E; E)
$$

（第VI, §1, No. 7章）。我们写$U(\mu) = \int_G U(s)\, d\mu(s)$。我们在$\mathscr{C}(G)$中为$\mathscr{C}'(G)$配备了紧凑收敛的拓扑。 $\mathscr{C}'(G) \times E$到$E$的映射$(\mu, x) \mapsto U(\mu)x$相对于$\mathscr{C}'(G)$的等连续子集和$E$的紧致子集来说是*次连续的；特别是，$\mathscr{C}'(G)$到$\mathscr{L}(E; E)$的映射$\mu \mapsto U(\mu)$（配备紧凑收敛的拓扑）是连续的（*loc.cit.*，Prop.16）。

在阶中，为了稍后能够应用这些结果，我们注认为，如果$X$是局部紧致空间，则$\mathscr{C}(X)$配备紧致收敛的拓扑，是完整的（GT，X, §1, No. 6，Th.2的Cor.3）。另一方面，$\mathscr{K}(X)$是桶状的，因此它的对偶$\mathscr{M}(X)$，配备了$\mathscr{K}(X)$中紧凑收敛的拓扑，是准完备的（TVS，III, §4, No. 2，Th.1的Cor.4）。当然，$\mathscr{K}(X)$对于从范数推导出来的拓扑来说是完备的，因此它的*对偶*$\mathscr{M}^1(X)$对于$\mathscr{K}(X)$中紧致收敛的拓扑来说是准完备的（*loc.cit.*）。

现在让我们假设 $U$ 是 *Banach 空间* $E$ 上局部紧凑群 $G$ 的连续线性表示。 集合 $g(s) = \|U(s)\|$ 对于所有 $s \in G$。然后，如果 $\mu$ 是 $G$ 的测度，使得 $g$ 是 $\mu$ 可积，则有 $\int_G U(s)\, d\mu(s) \in \mathscr{L}(E; E)$ 和 $\|\int_G U(s)\, d\mu(s)\| \leq \int g(s)\, d|\mu|(s)$（第 VI, §1, No. 7，*注* 1）。我们再次写$U(\mu) = \int_G U(s)\, d\mu(s)$。

### 7. 关系自同态 $U(\mu)$ 和自同态 $U(s)$ 之间

#### 引理 4 {#int-viii-s2-lem-4 .statement tag=09IW}

令$T$为$T$的局部紧凑空间、$a$点、$\mathscr{M}(T)$的$M$子集以及$\mathfrak{F}$$M$上的过滤器。假设：
(i) 对于$T$、数$|\mu|(K)$、对于$\mu \in M$的每个紧凑子集$K$，都在上面有界；
(ii) $\lim_{\mu,\mathfrak{F}} |\mu|(K) = 0$ 对于子集 $K$ 或 $T - \{a\}$。
(iii) 在$T$中存在$a$的紧邻域$V$，使得$\lim_{\mu,\mathfrak{F}} \mu(V) = 1$。

然后，滤波器$\mathfrak{F}$在$\mathscr{M}(T)$中收敛到$\varepsilon_a$，并在$\mathscr{H}(T)$中配备紧凑收敛的拓扑。

通过假设 (i)，$M$ 是 $\mathscr{M}(T)$ 的等连续子集，因为它有模糊边界，并且 $\mathscr{H}(T)$ 是桶状的（TVS，III, §4, No. 2，Th.1）。因此，只要（GT，X, §2, No. 4，Th.1）证明如果$f \in \mathscr{H}(T)$，则$\lim_{\mu,\mathfrak{F}} \mu(f) = f(a)$。设$K$为$V$的并和$f$的支持度；如果$K'$是$K - V$的闭包，则有

$$
|\mu(K) - \mu(V)| = |\mu(K - V)| \leq |\mu|(K');
$$

因为 $K'$ 是紧致的，并且没有包含 $a$，因此结论就是 $\lim_{\mu,\mathfrak{F}} \mu(K) = 1$。令$\varepsilon > 0$，并让$W$是$a$在$K$中的开邻域，使得$|f(t) - f(a)| \leq \varepsilon$对于$t \in W$；一个人可以写

$$
\mu(f) - f(a) = f(a)(\mu(K) - 1) + \int_K (f(t) - f(a)) d\mu(t);
$$

$K$上的积分可以写成$W$和$K - W$上的类似积分的和；如果 $C = \sup |f|$，则有

$$
|\mu(f) - f(a)| \leq C|\mu(K) - 1| + \varepsilon \cdot |\mu|(K) + 2C \cdot |\mu|(K - W).
$$

由于右侧的第一个和第三个项相对于 $\mathfrak{F}$ 趋于 0，因此可以看到确实是 $\lim_{\mu,\mathfrak{F}} \mu(f) = f(a)$。

#### 推论 1 {#int-viii-s2-lem-4-cor-1 .statement tag=09IX}

根据引理 4 中的假设，假设在加法中存在一个由 $T$ 包含组成的紧凑子集 $K_0$，它是所有测度$\mu \in M$ 的支持。然后$\mathfrak{F}$也在$\mathscr{C}'(T)$中收敛到$\varepsilon_a$，并在$\mathscr{C}(T)$中配备了拓扑的紧凑收敛。

因为，$\mathscr{C}(T)$到$\mathscr{C}(K_0)$的限制映射是连续的；因此，如果$H$是$\mathscr{C}(T)$的紧致子集，则$H$形式中函数的限制到$K_0$是$\mathscr{C}(K_0)$的紧致子集。然后，只需在 $K_0$ 之前在替换 $T$ 上应用引理 4 即可。

#### 推论 2 {#int-viii-s2-lem-4-cor-2 .statement tag=09IY}

*如 Cor 中的假设。 1、令$f$为$T$的连续映射变为准完全局部凸空间$E$。然后*

$$
\lim_{\mu,\mathfrak{T}} \int f(t)\, d\mu(t) = f(a).
$$

这是从 Cor 得出的。 1 和第 14 章提案。 VI, §1, No. 6。

#### 推论 3 {#int-viii-s2-lem-4-cor-3 .statement tag=09IZ}

*令$G$为局部紧致群，$E$为准完全局部凸空间，$U$为$E$中$G$的连续线性表示。令 $\beta$ 为$G$、$a$ 元素 $G$ 和$\mathscr{B}$ 基的正测度，用于过滤$a$ 的邻域，由紧凑邻域组成。对于每个$V \in \mathscr{B}$，令$f_V$是$G$上的连续函数$\geqslant 0$，并包含$V$中的支持，从而$\int f_V\, d\beta = 1$。然后，对于每 $x \in E$，

$$
U(a)x = \lim_V U(f_V \cdot \beta)x,
$$

*极限是相对于$\mathscr{B}$的截面过滤器而取的。*

$G$到$E$的映射$s \mapsto U(s)x$是连续的。由科. 2、$U(a)x = \lim_V \int (U(s)x) \cdot f_V(s)\, d\beta(s)$相对于$\mathscr{B}$的截面滤波器，即$U(a)x = \lim_V U(f_V \cdot \beta)x$。

#### 命题 10 {#int-viii-s2-prop-10 .statement tag=09J0}

*设$G$为局部紧致群，$E$为准完全局部凸空间，$U$为$E$中$G$的连续线性表示，$\beta$为$G$上有支持的正测度$G$。

(i) 向量 $U(f \cdot \beta)x$，其中$f$超过$\mathscr{K}(G)$，$x$超过$E$，在$E$中是稠密的。

(ii) *令$F$为$E$的闭线性子空间。如果 $F$ 对于 $U$ 是稳定的，那么 $U(\mu)(F) \subset F$ 对于每个 $\mu \in \mathscr{C}'(G)$ 都是稳定的。相反，如果 $U(f \cdot \beta) \subset F$ 对于每个 $f \in \mathscr{K}(G)$，则 $F$ 对于 $U$ 是稳定的。*

(ii) 的第一个部分是直接的，因为$U(s)$到$F$ ($s \in G$) 定义的限制是准完全局部凸空间中$G$的连续线性表示 $F$。 (ii) 和 (i) 的第二个部分源自 Cor。 引理 4 中的 3 个。

### 习题 {#int-viii-s2-exercises}

参见[习题为 § 2](exercises/s2/)。
