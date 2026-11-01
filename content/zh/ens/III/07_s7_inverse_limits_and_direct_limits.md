---
book: ens
book_title: Theory of Sets
chapter: III
chapter_title: ORDERED SETS, CARDINALS, INTEGERS
section: 7
section_title: Inverse limits and direct limits
lang: zh
source: ens-i-iv
source_edition: 2004, Springer
book_pages: 191-211, 251-254
pdf_pages: 0197-0217, 0257-0260
extraction: ocr
subsections:
    - "no": 1
      title: INVERSE LIMITS
      page: 191
      pdf_page: 197
    - "no": 2
      title: INVERSE SYSTEMS OF MAPPINGS
      page: 192
      pdf_page: 198
    - "no": 3
      title: DOUBLE INVERSE LIMIT
      page: 196
      pdf_page: 202
    - "no": 4
      title: CONDITIONS FOR AN INVERSE LIMIT TO BE NON-EMPTY
      page: 198
      pdf_page: 204
    - "no": 5
      title: DIRECT LIMITS
      page: 202
      pdf_page: 208
    - "no": 6
      title: DIRECT SYSTEMS OF MAPPINGS
      page: 204
      pdf_page: 210
    - "no": 7
      title: DOUBLE DIRECT LIMIT. PRODUCT OF DIRECT LIMITS
      page: 209
      pdf_page: 215
statements: 34
exercises: 9
errata:
    - says: no. 2, Proposition 2, Corollary 2
      read: no. 2, Proposition 1, Corollary 2
      why: The fact cited on page 197 is that the maps of an inverse system compose, h to the lambda nu being h to the lambda mu after h to the mu nu, and that is Corollary 2 of Proposition 1 of no. 2, the corollary on three inverse systems. Proposition 2 of that no. prints one corollary and it carries no number.
content_sha256: 1e2b46736839a7481841a69b4877adda7fcf3190ba6520600239e35da855f22b
translated_from: content/en/ens/III/07_s7_inverse_limits_and_direct_limits.md
translation_method: google
source_content_sha256: 32f34a0e7e91e7e94cb6dacf6471b60fe7158e208c5d0e1bd2901e3f619ccda7
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-50f48bb3
glossary_version: 34
glossary_terms_sha256: 88278c5f773226462a8e9bb4f805ddf7bb36f20cb2297efa0aab94e30727309a
prompt_sha256: 77d1eb2d7fcbd90aea4f1a996022f1b3908ace921dc0bfaa5df62ffc2d1f67a6
---

## 7. 逆极限和直极限

### 1. 逆极限

令$I$为预定的集合，并让$(E_\alpha)_{\alpha\in I}$为由$I$索引的集合族。对于$I$的元素的每个对$(\alpha,\beta)$使得$\alpha\leq\beta$，令$f_{\alpha\beta}$为$E_\alpha$的$E_\beta$的映射。假设 $f_{\alpha\beta}$ 满足以下条件 ：

$(\mathrm{LP}_I)$ *关系 $\alpha\leq\beta\leq\gamma$ 暗示$f_{\alpha\gamma}=f_{\alpha\beta}\circ f_{\beta\gamma}$.*

$(\mathrm{LP}_{II})$ *对于每个 $\alpha\in I$，$f_{\alpha\alpha}$ 是 $E_\alpha$ 中的恒等映射。*

令$G=\prod_{\alpha\in I}E_\alpha$为集合$(E_\alpha)_{\alpha\in I}$族的*乘积*，并让$E$表示所有$x$中$G$由……组成的子集，其中满足每个关系

(1)

$$\operatorname{pr}_{\alpha}x=f_{\alpha\beta}(\operatorname{pr}_{\beta}x)$$

对于指标$(\alpha,\beta)$中的每个对，使得$\alpha\leq\beta$。 $E$据说是家庭*逆极限*$(E_\alpha)_{\alpha\in I}$*相对于映射*$(f_{\alpha\beta})$的家庭，在没有歧义的情况下，我们写成$E=\underset{\longleftarrow}{\lim}\,(E_\alpha,f_{\alpha\beta})$或简单地写成$E=\underset{\longleftarrow}{\lim}\,E_\alpha$。通过滥用语言，对$((E_\alpha),(f_{\alpha\beta}))$（通常用$(E_{\alpha\beta},f_{\alpha\beta})$表示）被称为集合*的*逆系，相对于指标集合$I$。 投影 $\operatorname{pr}_\alpha$到$E$的*限制* $f_\alpha$称为$E$到$E_\alpha$的*典范映射*，我们有关系

(2)

$$f_\alpha=f_{\alpha\beta}\circ f_\beta$$

每当$\alpha\leq\beta$；这只是关系 (1) 其中定义 $E$ 的转录。

*例*

#### 例 1 {#ens-iii-s7-n1-exa-1 .statement tag=03TF}

假设$I$上的序关系是*等式*的关系。那么唯一的对$(\alpha,\beta)$使得$\alpha\leq\beta$是对$(\alpha,\alpha)$，其中$\alpha\in I$；并且由于 $f_{\alpha\alpha}$ 是恒等映射，因此 *所有* $x\in G$ 都满足关系 (1)；在其他字中，$\underset{\longleftarrow}{\lim}\,E_\alpha$则为*乘积* $\prod_{\alpha\in I}E_\alpha$。

#### 例 2 {#ens-iii-s7-n1-exa-2 .statement tag=03TG}

假设$I$是*右向的*，$E_\alpha$对于所有$\alpha\in I$来说都是相同的集合$F$，并且只要$\alpha\leq\beta$，$f_{\alpha\beta}$就是$F$的恒等映射到自身上。那么$E=\underset{\longleftarrow}{\lim}\,E_\alpha$就是乘积$\prod_{\alpha\in I}E_\alpha=F^I$的*对角的*$\Delta$。事实上，很明显每个 $x\in\Delta$ 都满足关系 (1)。相反，让$x$是$E$的元素，并让我们证明对于指标$(\alpha, \beta)$的每个对，我们有$\mathrm{pr}_\alpha x = \mathrm{pr}_\beta x$。到假设，存在指标$\gamma \in I$使得$\alpha \leqslant \gamma$和$\beta \leqslant \gamma$；因此，根据（1），我们有$\mathrm{pr}_\alpha x = f_{\alpha\gamma}(\mathrm{pr}_\gamma x) = \mathrm{pr}_\gamma x$，类似地还有$\mathrm{pr}_\beta x = \mathrm{pr}_\gamma x$，这证明了我们的断言。

应该注意的是，即使所有 $E_\alpha$ 都非空并且所有映射 $f_{\alpha\beta}$ 都是*满射*（习题 4；参见 no. 4），$E = \varprojlim E_\alpha$ 也可以是*空*。

¶ 很明显，对于$(E_\alpha)_{\alpha \in J}$和家族$(f_{\alpha\beta})$的I对由……组成的每个子集J，其中$\alpha \in J$、$\beta \in J$和$\alpha \leqslant \beta$又是逆系集合相对于 J；据说它是通过将指标集合*限制*到J而获得的。令E和E'分别表示家族$(E_\alpha)_{\alpha \in I}$和$(E_\alpha)_{\alpha \in J}$的逆极限。每$x \in E$元素

$$g(x) = (f_\alpha(x))_{\alpha \in J} \tag{3}$$

凭借(2)属于到E'； 映射 $g : E \to E'$ 这样定义的称为*规范*。如果 J' 是 J 的子集，并且 E'' 是 $(E_\alpha)_{\alpha \in J'}$ 族的逆极限，并且如果 $g' : E' \to E''$ 和 $g'' : E \to E''$ 是典范映射，那么到定义我们有

$$g'' = g' \circ g. \tag{4}$$

### 2. 映射的逆系

#### 命题 1 {#ens-iii-s7-prop-1 .statement tag=03OC}

*令* I *为有序集合，令* $(E_\alpha, f_{\alpha\beta})$ *为集合相对于* I的逆系，*让* $E = \varprojlim E_\alpha$ *为其逆极限，并且对于每个* $\alpha \in I$ *令*

$$f_\alpha : E \to E_\alpha$$

*为典范映射。对于每个*$\alpha \in I$，*让*$u_\alpha$*成为集合*F的映射*进入*$E_\alpha$*这样*

$$f_{\alpha\beta} \circ u_\beta = u_\alpha \qquad \textit{whenever } \alpha \leqslant \beta. \tag{5}$$

*然后:*

(a) *存在* F *进入* E *的唯一映射* $u$ *使得*

$$u_\alpha = f_\alpha \circ u \qquad \textit{for all } \alpha \in I;\tag{6}$$

(b) *映射* $u$ *是单射当且仅当，对于* F 的不同元素* $y$、$z$ *的每个对，*存在* $\alpha \in I$ *使得* $u_\alpha(y) \neq u_\alpha(z)$。

对于关系 $u_\alpha = f_\alpha \circ u$ 意味着对于每个 $y \in F$ 我们有

$$\mathrm{pr}_\alpha(u(y)) = u_\alpha(y);$$

元素 $u(y) \in \prod_{\alpha \in I} E_\alpha$ 由$u(y) = (u_\alpha(y))_{\alpha \in I}$唯一确定。仍有待证明的是，$u(y) \in E$对于所有$y \in F$，在其他字中，

$$\mathrm{pr}_\alpha(u(y)) = f_{\alpha\beta}(\mathrm{pr}_\beta(u(y)))$$

每当$\alpha \leqslant \beta$时。但这可以写成形式

$$u_\alpha(y) = f_{\alpha\beta}(u_\beta(y))$$

因此由 (5) 得出。 命题的第二个部分紧随定义之后。

#### 推论 1 {#ens-iii-s7-prop-1-cor-1 .statement tag=03RN}

*令*$(E_\alpha, f_{\alpha\beta})$*和*$(F_\alpha, g_{\alpha\beta})$*为集合中的两个逆系相对于相同的指标集合*I； *让* $E = \varprojlim E_\alpha$，$F = \varprojlim F_\alpha$，*并让* $f_\alpha$ *（分别* $g_\alpha$*）为* E *到* $E_\alpha$ *（分别为* F *到* $F_\alpha$*）的典范映射，对于每个* $\alpha \in I$，*对于每个* $\alpha \in I$，*让*$u_\alpha$*成为*E的映射*进入*$F_\alpha$*使得图表*

$$\begin{array}{ccc} E_\beta & \overset{u_\beta}{\longrightarrow} & F_\beta \\ {\scriptstyle f_{\alpha\beta}}\big\downarrow & & \big\downarrow{\scriptstyle g_{\alpha\beta}} \\ E_\alpha & \underset{u_\alpha}{\longrightarrow} & F_\alpha \end{array}$$

*可交换* [^1] *每当* $\alpha \leqslant \beta$。 *然后存在唯一映射* $u : E \to F$ *使得对于每个* $\alpha \in I$ *图表*

$$\begin{array}{ccc} E & \overset{u}{\longrightarrow} & F \\ {\scriptstyle f_\alpha}\big\downarrow & & \big\downarrow{\scriptstyle g_\alpha} \\ E_\alpha & \underset{u_\alpha}{\longrightarrow} & F_\alpha \end{array}$$

*是可交换的。*

输入$v_\alpha = u_\alpha \circ f_\alpha$。如果 $\alpha \leqslant \beta$，由 (2) 我们有，

$$g_{\alpha\beta} \circ v_\beta = g_{\alpha\beta} \circ u_\beta \circ f_\beta = u_\alpha \circ f_{\alpha\beta} \circ f_\beta = u_\alpha \circ f_\alpha = v_\alpha,$$

因此我们可以应用命题 1 到映射 $v_\alpha$；因此映射$u:E\to F$的存在和唯一性使得

$$
g_\alpha\circ u=v_\alpha=u_\alpha\circ f_\alpha
$$

对于每个$\alpha\in I$。

¶ 满足推论 1 的条件的映射 $u_\alpha:E_\alpha\to F_\alpha$ 族称为 $(E_\alpha,f_{\alpha\beta})$ 的映射* 到 $(F_\alpha,g_{\alpha\beta})$ 的 *逆系。推论1中定义的映射$u$称为$(u_\alpha)$族的*逆极限*，并且在不存在混淆风险的情况下写作$u=\underset{\leftarrow}{\lim}\,u_\alpha$。

#### 推论 2 {#ens-iii-s7-prop-1-cor-2 .statement tag=03RO}

令$(E_\alpha,f_{\alpha\beta})$、$(F_\alpha,g_{\alpha\beta})$、$(G_\alpha,h_{\alpha\beta})$为集合的三个*逆系相对于相同的指标集合*$I$；令$E=\underset{\leftarrow}{\lim}\,E_\alpha$、$F=\underset{\leftarrow}{\lim}\,F_\alpha$、$G=\underset{\leftarrow}{\lim}\,G_\alpha$，并让$f_\alpha$（分别$g_\alpha,h_\alpha$）成为$E$（分别$F,G$）的*典范映射**到*$E_\alpha$（分别$F_\alpha,G_\alpha$）。如果$(u_\alpha)$和$(v_\alpha)$是*两个映射的逆系*、$u_\alpha:E_\alpha\to F_\alpha$、$v_\alpha:F_\alpha\to G_\alpha$，那么*复合映射*$v_\alpha\circ u_\alpha:E_\alpha\to G_\alpha$形式和映射*的*逆系，我们有

(7)

$$
\underset{\leftarrow}{\lim}\,(v_\alpha\circ u_\alpha)
=
\left(\underset{\leftarrow}{\lim}\,v_\alpha\right)\circ
\left(\underset{\leftarrow}{\lim}\,u_\alpha\right).
$$

因为如果我们输入$w_\alpha=v_\alpha\circ u_\alpha$，那么如果$\alpha\leq\beta$我们有

$$
w_\alpha\circ f_{\alpha\beta}
=v_\alpha\circ(u_\alpha\circ f_{\alpha\beta})
=v_\alpha\circ(g_{\alpha\beta}\circ v_\beta)
=(h_{\alpha\beta}\circ v_\beta)\circ u_\beta
=h_{\alpha\beta}\circ w_\beta,
$$

这表明$(w_\alpha)$是映射的逆系。此外，如果$u=\underset{\leftarrow}{\lim}\,u_\alpha$和$v=\underset{\leftarrow}{\lim}\,v_\alpha$，则每个$\alpha\in I$都有$h_\alpha\circ(v\circ u)=(v_\alpha\circ g_\alpha)\circ u=(v_\alpha\circ u_\alpha)\circ f_\alpha$，因此，通过逆极限的唯一性，我们有$v\circ u=\underset{\leftarrow}{\lim}\,w_\alpha$。

¶ 令 $(E_\alpha,f_{\alpha\beta})$ 为集合的逆系，对于每个 $\alpha\in I$，令 $M_\alpha$ 为 $E_\alpha$ 的子集。如果$f_{\alpha\beta}(M_\beta)\subset M_\alpha$每当$\alpha\leq\beta$，则$M_\alpha$被称为形式和$E_\alpha$的子集*的*逆系。设$g_{\alpha\beta}$为$M_\beta$的映射到$M_\alpha$（其中$\alpha\leq\beta$），其图形与$f_{\alpha\beta}$到$M_\beta$的限制的图形相同。那么很明显 $(M_\alpha,g_{\alpha\beta})$ 是集合的逆系并且

(8)

$$
\underset{\leftarrow}{\lim}\,M_\alpha
=
\left(\underset{\leftarrow}{\lim}\,E_\alpha\right)\cap\prod_{\alpha\in I}M_\alpha.
$$

#### 命题 2 {#ens-iii-s7-prop-2 .statement tag=03RP}

令$(E_\alpha,f_{\alpha\beta})$和$(E'_\alpha,f'_{\alpha\beta})$为集合相对于*$I$的两个*逆系，并令$u_\alpha$为每个$\alpha\in I$的$E_\alpha$到$E'_\alpha$的映射，这样$u_\alpha$形式*逆系映射*。让$u=\underset{\leftarrow}{\lim}\,u_\alpha$。然后对于每个$x'=(x'_\alpha)\in E'=\underset{\leftarrow}{\lim}\,E'_\alpha$，$\bar u_\alpha^{-1}(x'_\alpha)$形式，$E_\alpha$和$\bar u^{-1}(x')=\underset{\leftarrow}{\lim}\,\bar u_\alpha^{-1}(x'_\alpha)$的子集*的*逆系。

对于如果 $\alpha \leqslant \beta$ 和 $x_\beta \in \overset{-1}{u_\beta}(x'_\beta)$，我们有

$$u_\alpha(f_{\alpha\beta}(x_\beta)) = f'_{\alpha\beta}(u_\beta(x_\beta)) = f'_{\alpha\beta}(x'_\beta) = x'_\alpha,$$

第一个断言随之而来；并说 $x = (x_\alpha) \in \mathrm{E} = \varprojlim \mathrm{E}_\alpha$ 使得 $u(x) = x'$ 意味着，通过定义，每个 $\alpha \in \mathrm{I}$ 都有 $u_\alpha(x_\alpha) = x'_\alpha$。

#### 推论{#ens-iii-s7-n2-cor-1 .statement tag=03OD}

*如果$u_\alpha$是单射*（或*双射的*）*对于每个$\alpha \in \mathrm{I}$，则$u$是单射*（或*双射的*）。

有了命题2的记号，像$u_\alpha(\mathrm{E}_\alpha)$还有$\mathrm{E}'_\alpha$的子集形式逆系，我们有

(9) $$u(\mathrm{E}) \subset \varprojlim u_\alpha(\mathrm{E}_\alpha);$$

但这个关系的两侧*不一定相等*（习题4）。

#### 命题 3 {#ens-iii-s7-prop-3 .statement tag=03OE}

*令$\mathrm{I}$为预定的集合，令$(\mathrm{E}_\alpha, f_{\alpha\beta})$为集合相对于$\mathrm{I}$的逆系，并令$\mathrm{E} = \varprojlim \mathrm{E}_\alpha$。令$\mathrm{J}$为$\mathrm{I}$的共尾子集，使得$\mathrm{J}$右向，并令$\mathrm{E}'$为通过限制指标从$(\mathrm{E}_\alpha, f_{\alpha\beta})$获得的集合的逆系的逆极限集合至 $\mathrm{J}$。那么 $\mathrm{E}$ 的典范映射 $g$ 到 $\mathrm{E}'$* (no. 1, *公式* (3)) *是双射*。

对于每个$\alpha \in \mathrm{J}$，令$f'_\alpha$为典范映射$\mathrm{E}' \to \mathrm{E}_\alpha$。 然后，通过（2）和（5），$g$是$\mathrm{E}$的唯一映射到$\mathrm{E}'$，使得$f_\alpha = f'_\alpha \circ g$对于所有$\alpha \in \mathrm{J}$（命题1）。 我们将使用命题 1 的准则来证明$g$是单射的。 如果$x$、$y$与$\mathrm{E}$不同元素，则到定义存在$\alpha \in \mathrm{I}$使得$f_\alpha(x) \neq f_\alpha(y)$；由于$\mathrm{J}$是$\mathrm{I}$的共尾，因此存在$\lambda \in \mathrm{J}$使得$\alpha \leqslant \lambda$；从$f_{\alpha\lambda}(f_\lambda(x)) \neq f_{\alpha\lambda}(f_\lambda(y))$开始，我们有$f_\lambda(x) \neq f_\lambda(y)$。 仍有待证明 $g$ 是满射的。 设$x' = (x'_\lambda)_{\lambda \in \mathrm{J}}$为$\mathrm{E}'$的元素。 对于每个$\alpha \in \mathrm{I}$，存在$\lambda \in \mathrm{J}$使得$\alpha \leqslant \lambda$，并且元素$f_{\alpha\lambda}(x'_\lambda)$不依赖于指标$\lambda \in \mathrm{J}$使得$\alpha \leqslant \lambda$；因为如果$\mu \in \mathrm{J}$使得$\alpha \leqslant \mu$，则存在$\nu \in \mathrm{J}$使得$\lambda \leqslant \nu$和$\mu \leqslant \nu$，因此存在$f_{\alpha\lambda}(x'_\lambda) = f_{\alpha\lambda}(f_{\lambda\nu}(x'_\nu)) = f_{\alpha\nu}(x'_\nu)$，并且类似地$f_{\alpha\mu}(x'_\mu) = f_{\alpha\nu}(x'_\nu)$。 令$x_\alpha$为$\lambda \in \mathrm{J}$的$f_{\alpha\lambda}(x'_\lambda)$的公共的值，使得$\alpha \leqslant \lambda$，并令$x = (x_\alpha)_{\alpha \in \mathrm{I}}$。 然后$x \in \mathrm{E}$，因为如果$\alpha \leqslant \beta$并且$\lambda \in \mathrm{J}$使得$\beta \leqslant \lambda$，我们有

$$f_{\alpha\beta}(x_\beta) = f_{\alpha\beta}(f_{\beta\lambda}(x'_\lambda)) = f_{\alpha\lambda}(x'_\lambda) = x_\alpha.$$

最后，我们对所有$\lambda \in \mathrm{J}$有$x'_\lambda = f_{\lambda\lambda}(x'_\lambda)$，因此对所有$\lambda \in \mathrm{J}$有$x_\lambda = x'_\lambda$；其他字，$f(x_\lambda) = x'_\lambda$，所以$g(x) = x'$。因此 $g$ 是满射，证明是完备的。

特别是，如果$\mathrm{I}$有*最大元素*$\omega$，我们可以采用$\mathrm{J} = \{\omega\}$，这样$\varprojlim \mathrm{E}_\alpha$就可以与$\mathrm{E}_\omega$规范地识别。

*注*

#### 注 1 {#ens-iii-s7-n2-rem-1 .statement tag=03TH}

对于每个$\alpha \in I$，放入$E'_\alpha = f_\alpha(E)$。那么根据(2)，$E_\alpha$的集合$E'_\alpha$形式*子集*的*逆系，立即可知$\varprojlim E'_\alpha = E = \varprojlim E_\alpha$。 映射$f'_{\alpha\beta} : E'_\beta \to E'_\alpha$（其中$\alpha \leqslant \beta$），其图与$f_{\alpha\beta}$到$E_\beta$的限制的图相同，是*满射*，我们有

$$(10) \qquad E'_\alpha = f_\alpha(E) \subset \bigcap_{\beta \geqslant \alpha} f_{\alpha\beta}(E_\beta)$$

对于所有$\alpha \in I$。

#### 注 2 {#ens-iii-s7-n2-rem-2 .statement tag=03TI}

令I为（*右*）*定向*有序集合，令$(E_\alpha, f_{\alpha\beta})$为集合相对于I的逆系，对于每个$\alpha \in I$令$u_\alpha : F \to E_\alpha$为映射，使得该族$(u_\alpha)$ 满足公式 (5)。考虑逆系$(F_\alpha, i_{\alpha\beta})$由I索引，其中$F_\alpha = F$对于所有$\alpha \in I$和$i_{\alpha\beta}$是F的恒等映射。然后（no. 1，例2）F被规范地标识为$\varprojlim F_\alpha$。如果我们将$u_\alpha$视为$F_\alpha$的映射进入$E_\alpha$，则$(u_\alpha)$是映射的逆系，并且（6）定义的映射$u : F \to E$与此的逆极限相同系统共映射。因而，通过滥用语言，我们写了$u = \varprojlim u_\alpha$。

#### 注 3 {#ens-iii-s7-n2-rem-3 .statement tag=03TJ}

令I为有序集合，并令$(E_\alpha, f_{\alpha\beta})$为集合相对于I的逆系。对于I的每个有限子集 J，令$F_J$为通过将指标集合限制为J而从$(E_\alpha, f_{\alpha\beta})$获得的（有限）逆系的逆极限。如果J和K是以下任意两个有限子集 I使得$J \subset K$，让$g_{JK}$表示$F_K$的典范映射（3）到$F_J$。那么关系 (4) 表明 $(F_J, g_{JK})$ 是集合相对于有限子集的*定向* 集合（相对于关系 $\subset$）$\mathfrak{F}(I)$ 的 *逆系* I。接下来，对于每个$J \in \mathfrak{F}(I)$，令$h_J : E \to F_J$为典范映射 (3)。根据(4)以及注(2)中提到的语言滥用，$(h_J)$是映射的*逆系*。输入$h = \varprojlim h_J : E \to F = \varprojlim F_J$，让我们证明$h$是*双射*（称为*规范*）。确实，让$y = (y_J) \in F$。到定义，我们有$y_J = (x_{\alpha, J})_{\alpha \in J}$，其中$x_{\alpha, J} \in E_\alpha$代表所有$\alpha \in J$。如果$J \subset K$，那么通过映射$g_{JK}$的定义，并且因为$y_J = g_{JK}(y_K)$，我们对所有$\alpha \in J$有$x_{\alpha, J} = x_{\alpha, K}$。因而，给定$\alpha \in I$，存在唯一元素$x_\alpha \in E_\alpha$，使得$x_\alpha = x_{\alpha, J}$对于I的所有有限子集J，其中包含$\alpha$。如果$\alpha \leqslant \beta$，I有有限子集J，其中包含既$\alpha$又$\beta$；因而$x_\alpha = f_{\alpha\beta}(x_\beta)$乘以定义。因而$x = (x_\alpha)$是E的唯一元素，使得$h(x) = y$。

### 3. 双重逆极限

令I、L为两个预先订购的集合，以及$I \times L$它们的乘积（§ 1, no. 4）。考虑集合$(E^\lambda_\alpha, f^{\lambda\mu}_{\alpha\beta})$相对于指标集合$I \times L$的逆系。

我们有

(11) 每当$\alpha \leqslant \beta \leqslant \gamma$和$\lambda \leqslant \mu \leqslant \nu$时，$\qquad f^{\lambda\nu}_{\alpha\gamma} = f^{\lambda\mu}_{\alpha\beta} \circ f^{\mu\nu}_{\beta\gamma}$。

让E或$\lim \mathrm{E}^{\lambda}_{\alpha}$表示这个逆系的逆极限。

对于每个$\lambda \in \mathrm{L}$，放入$g^{\lambda}_{\alpha\beta} = f^{\lambda\lambda}_{\alpha\beta} : \mathrm{E}^{\lambda}_{\beta} \to \mathrm{E}^{\lambda}_{\alpha}$。由(11)可知

(12) $\qquad g^{\lambda}_{\alpha\gamma} = g^{\lambda}_{\alpha\beta} \circ g^{\lambda}_{\beta\gamma}$ 每当$\alpha \leqslant \beta \leqslant \gamma$时，

这样$(\mathrm{E}^{\lambda}_{\alpha}, g^{\lambda}_{\alpha\beta})$相对于I来说是集合的逆系。让$\mathrm{F}^{\lambda} = \lim \mathrm{E}^{\lambda}_{\alpha}$表示它的逆极限。对于L中的固定$\lambda \leqslant \mu$，从(11)得出映射的$h^{\lambda\mu}_{\alpha} = f^{\lambda\mu}_{\alpha\alpha} : \mathrm{E}^{\mu}_{\alpha} \to \mathrm{E}^{\lambda}_{\alpha}$形式逆系，其逆极限我们用$h^{\lambda\mu} = \lim h^{\lambda\mu}_{\alpha} : \mathrm{F}^{\mu} \to \mathrm{F}^{\lambda}$表示。如果$\lambda \leqslant \mu \leqslant \nu$在L中，我们有

(13) $$h^{\lambda\nu} = h^{\lambda\mu} \circ h^{\mu\nu}$$

（no. 2，命题2，推论2）；因此，相对于L，$(\mathrm{F}^{\lambda}, h^{\lambda\mu})$是集合的逆系。令$\mathrm{F} = \lim \mathrm{F}^{\lambda}$为其逆极限。我们将定义*规范的双射*$\mathrm{F} \to \mathrm{E}$。为此，我们注 F 是$\prod_{\lambda \in \mathrm{L}} \mathrm{F}^{\lambda}$ 的定义子集，$\mathrm{F}^{\lambda}$ 是$\prod_{\alpha \in \mathrm{I}} \mathrm{E}^{\lambda}_{\alpha}$ 的子集；因此F可以被规范地识别为子集或$\prod_{(\alpha, \lambda) \in \mathrm{I} \times \mathrm{L}} \mathrm{E}^{\lambda}_{\alpha} = \mathrm{G}$（章II, § 5, no. 5，命题7）。对于每个 $z \in \mathrm{G}$，令 $\mathrm{pr}^{\lambda}(z)$ 表示 $\prod_{\alpha \in \mathrm{I}} \mathrm{E}^{\lambda}_{\alpha}$ 的元素 $(\mathrm{pr}^{\lambda}_{\alpha}(z))_{\alpha \in \mathrm{I}}$。那么 $z \in \mathrm{F}$ 当且仅当

(14) $\qquad \mathrm{pr}^{\lambda}(z) = h^{\lambda\mu}(\mathrm{pr}^{\mu}(z))$ 每当 $\lambda \leqslant \mu$ 在 L 时

和 $\mathrm{pr}^{\lambda}(z) \in \mathrm{F}^{\lambda}$ 对于所有 $\lambda \in \mathrm{L}$；也就是说，每当 $\alpha \leqslant \beta$ 在 I 时，我们有

(15) $$\mathrm{pr}^{\lambda}_{\alpha}(z) = f^{\lambda\lambda}_{\alpha\beta}(\mathrm{pr}^{\lambda}_{\beta}(z)).$$

但是$h^{\lambda\mu}(\mathrm{pr}^{\mu}(z)) = (f^{\mu\lambda}_{\alpha\alpha}(\mathrm{pr}^{\mu}_{\alpha}(z))_{\alpha \in \mathrm{I}}$；因此，从 (14) 和 (15) 可以得出，如果 $\alpha \leqslant \beta$ 和 $\lambda \leqslant \mu$，我们有

$$\mathrm{pr}^{\lambda}_{\alpha}(z) = f^{\lambda\mu}_{\alpha\alpha}(f^{\mu\mu}_{\alpha\beta}(\mathrm{pr}^{\mu}_{\beta}(z))) = f^{\lambda\mu}_{\alpha\beta}(\mathrm{pr}^{\mu}_{\beta}(z)),$$

这意味着$z \in \mathrm{E}$。 逆命题是显而易见的，因此我们证明了

#### 命题 4 {#ens-iii-s7-prop-4 .statement tag=03OF}

*如果* $(\mathrm{E}^\lambda_\alpha, f^{\lambda\mu}_{\alpha\beta})$ *是集合的逆系相对于乘积* $\mathrm{I} \times \mathrm{L}$ *预购的集合，那么（直到规范的双射）我们有*

$$(16) \qquad \varprojlim_{\alpha,\lambda} \mathrm{E}^\lambda_\alpha = \varprojlim_\lambda \; (\varprojlim_\alpha \mathrm{E}^\lambda_\alpha).$$

#### 推论 1 {#ens-iii-s7-prop-4-cor-1 .statement tag=03OG}

*设*$(\mathrm{{E}'}^\lambda_\alpha, {f'}^{\mu\lambda}_{\alpha\beta})$*为集合的另一个逆系相对于*$\mathrm{I} \times \mathrm{L}$，*并且对于每个*$(\alpha, \lambda) \in \mathrm{I} \times \mathrm{L}$*让*$u^\lambda_\alpha$*为*$\mathrm{E}^\lambda_\alpha$*的映射*到* $\mathrm{{E}'}^\lambda_\alpha$*使得$u^\lambda_\alpha$*形式逆系等于映射。然后*

$$(17) \qquad \varprojlim_{\alpha,\lambda} u^\lambda_\alpha = \varprojlim_\lambda \; (\varprojlim_\alpha u^\lambda_\alpha).$$

验证与命题4类似。

#### 推论 2 {#ens-iii-s7-prop-4-cor-2 .statement tag=03OH}

*设*$(\mathrm{E}^\lambda_\alpha, f^\lambda_{\alpha\beta})_{\lambda \in \mathrm{L}}$*是逆系与集合相对于*I的家庭。 *如果* $\prod_{\lambda \in \mathrm{L}} f^\lambda_{\alpha\beta}$ *表示扩张至乘积* (章 II, § 5, no. 7, 定义 2) *属于映射* $(f^\lambda_{\alpha\beta})_{\lambda \in \mathrm{L}}$ 的家族，*则* $\left( \prod_{\lambda \in \mathrm{L}} \mathrm{E}^\lambda_\alpha, \prod_{\lambda \in \mathrm{L}} f^\lambda_{\alpha\beta} \right)$ *是集合相对于* I的逆系，*并且（直到规范的双射）我们有*

$$(18) \qquad \varprojlim_\alpha \prod_{\lambda \in \mathrm{L}} \mathrm{E}^\lambda_\alpha = \prod_{\lambda \in \mathrm{L}} (\varprojlim_\alpha \mathrm{E}^\lambda_\alpha).$$

考虑双逆系$(\mathrm{E}^\lambda_\alpha, g^{\lambda\mu}_{\alpha\beta})$相对于$\mathrm{I} \times \mathrm{L}$，其中L上的序关系是等式（no. 1、例1）和应用命题4。

### 4. 条件逆极限非空

在这个小节中，我们将给两个最常用的足够的条件，使逆极限非空（另见习题5）。

#### 命题 5 {#ens-iii-s7-prop-5 .statement tag=03OI}

*设*$(\mathrm{E}_\alpha, f_{\alpha\beta})$*是集合的逆系，相对于一个*有向*集合*I*，它有一个*可数*共尾子集，并进一步假设*$f_{\alpha\beta}$*是*满射的。 *然后，如果* $\mathrm{E} = \varprojlim \mathrm{E}_\alpha$，*典范映射* $f_\alpha : \mathrm{E} \to \mathrm{E}_\alpha$ *对于每个* $\alpha \in \mathrm{I}$ *都是满射（并且，更不必说，* E *不为空，前提是* $\mathrm{E}_\alpha$ *都不为空）。*

令$(\alpha_n)$为I的元素的序列，其中形式是I的并尾子集。由于I有向，对于$i < n$和$\beta_n \geqslant \alpha_n$，我们可以通过条件$\beta_0 = \alpha_0, \beta_n \geqslant \beta_i$归纳出I的元素定义序列$(\beta_n)$。显然，序列$(\beta_n)$是递增，形式是I的并列子集。鉴于no. 1的命题1和$\alpha \leqslant \beta_n$的关系$f_\alpha = f_{\alpha\beta_n} \circ f_{\beta_n}$，对于$\mathrm{I} = \mathbf{N}$的情况，我们只需要证明命题即可。而且，显然只要证明$f_0$是满射即可。让$x_0 \in \mathrm{E}_0$。 定义$x_n \in \mathrm{E}_n$（对于$n \geqslant 1$）归纳为集合$\overset{-1}{f}_{n-1,n}(x_{n-1})$的元素，这是可能的，因为后者集合与假设非空。然后我们通过$n - m$上的归纳表明$x_m = f_{mn}(x_n)$对应于$m \leqslant n$，并且由此得出$x = (x_n)$属于到E。

第二个标准涉及逆系$(\mathrm{E}_\alpha, f_{\alpha\beta})$相对于指标集合I，这样对于每个$\alpha \in \mathrm{I}$，我们给出集合$\mathfrak{S}_\alpha$/子集$\mathrm{E}_\alpha$，其中满足以下条件：

(i) *集合属于至$\mathfrak{S}_\alpha$的每个交以及属于至$\mathfrak{S}_\alpha$。*

特别是（通过考虑空族的交）$\mathrm{E}_\alpha \in \mathfrak{S}_\alpha$。

(ii) *如果子集$\mathfrak{F} \subset \mathfrak{S}_\alpha$的集合使得集合属于到$\mathfrak{F}$的每个有限交非空，则$\bigcap\limits_{\mathbf{M} \in \mathfrak{F}} \mathrm{M}$非空。*

鉴于(i)，显然(ii)等价于以下条件：

(ii)′ *如果 $\mathfrak{G} \subset \mathfrak{S}_\alpha$ 是左有向的（相对于包含）并且不是包含空集，则 $\bigcap\limits_{\mathbf{M} \in \mathfrak{G}} \mathrm{M}$ 非空。*

#### 定理 1 {#ens-iii-s7-thm-1 .statement tag=03RQ}

*假设I是有向的，集合$\mathfrak{S}_\alpha$满足条件*(i)*和*(ii)，*并且逆系$(\mathrm{E}_\alpha, f_{\alpha\beta})$具有以下属性：*

(iii) *对于指标$\alpha$、$\beta$中的每个对，使得$\alpha \leqslant \beta$，以及每个$x_\alpha \in \mathrm{E}_\alpha$，我们有$\overset{-1}{f}_{\alpha\beta}(x_\alpha) \in \mathfrak{S}_\beta$。*

(iv) *对于指标$\alpha$、$\beta$中的每个对，使得$\alpha \leqslant \beta$，以及每个$\mathrm{M}_\beta \in \mathfrak{S}_\beta$，我们有$f_{\alpha\beta}(\mathrm{M}_\beta) \in \mathfrak{S}_\alpha$。*

*对于每个$\alpha \in \mathrm{I}$，令$\mathrm{E} = \varprojlim \mathrm{E}_\alpha$和$f_\alpha : \mathrm{E} \to \mathrm{E}_\alpha$为典范映射。然后：*

(a) *对于每个 $\alpha \in \mathrm{I}$ 我们有*

$$(19) \qquad f_\alpha(\mathrm{E}) = \bigcap_{\beta \geqslant \alpha} f_{\alpha\beta}(\mathrm{E}_\beta).$$

(b) *如果对于每个 $\alpha \in \mathrm{I}$ $\mathrm{E}_\alpha$ 非空，则 E 也非空。*

令$\Sigma$为家庭$\mathfrak{A} = (\mathrm{A}_\alpha)_{\alpha \in \mathrm{I}}$的集合，其中满足以下条件：

$$(20) \qquad \mathrm{A}_\alpha \neq \emptyset \quad \textit{and} \quad \mathrm{A}_\alpha \in \mathfrak{S}_\alpha \quad \textit{for all} \quad \alpha \in \mathrm{I};$$

$$(21) \qquad f_{\alpha\beta}(\mathrm{A}_\beta) \subset \mathrm{A}_\alpha \quad \textit{whenever} \quad \alpha \leqslant \beta.$$

如果$\mathfrak{A} = (A_\alpha)$和$\mathfrak{A}' = (A'_\alpha)$是$\Sigma$中的任意两个元素，则让关系$\mathfrak{A} \leqslant \mathfrak{A}'$意味着对于所有$\alpha$来说$A_\alpha \supset A'_\alpha$。显然，$\Sigma$ 是按此关系“排序”的。

(1) 我们首先证明有序的集合 $\Sigma$ 是*归纳*的。令L为全序集，令$\lambda \to \mathfrak{A}^\lambda = (A^\lambda_\alpha)_{\alpha \in I}$为L到$\Sigma$的严格递增的映射。对于每个$\alpha \in I$，放入$B_\alpha = \bigcap_{\lambda \in L} A^\lambda_\alpha$。那么立即可以看出家庭$\mathfrak{B} = (B_\alpha)_{\alpha \in I}$满足（21）；由于(i)和(ii)，它也满足(20)，因此属于到$\Sigma$；显然，$\mathfrak{B}$是$\mathfrak{A}^\lambda$的集合中的上界。

(2) 设 $\mathfrak{A} = (A_\alpha)$ 为 $\Sigma$ 的*极大* 元素。每当$\alpha \leqslant \beta$时，我们都会证明$A_\alpha = f_{\alpha\beta}(A_\beta)$。让$A'_\alpha = \bigcap_{\beta \geqslant \alpha} f_{\alpha\beta}(A_\beta)$代表所有$\alpha \in I$，并让我们证明$\mathfrak{A}' = (A'_\alpha)$属于到$\Sigma$。 注首先，如果$\alpha \leqslant \beta \leqslant \gamma$，我们通过 (21) 得到 $f_{\alpha\gamma}(A_\gamma) = f_{\alpha\beta}(f_{\beta\gamma}(A_\gamma)) \subset f_{\alpha\beta}(A_\beta)$；此外，$f_{\alpha\beta}(A_\beta) \in \mathfrak{S}_\alpha$由(iv)计算，$f_{\alpha\beta}(A_\beta) \neq \emptyset$由(20)计算。因此条件(i)和(ii)表明$\mathfrak{A}'$满足(20)。另外，如果$\alpha \leqslant \beta$，我们有

$$f_{\alpha\beta}(A'_\beta) \subset \bigcap_{\gamma \geqslant \beta} f_{\alpha\beta}(f_{\beta\gamma}(A_\gamma)) = \bigcap_{\gamma \geqslant \beta} f_{\alpha\gamma}(A_\gamma);$$

对于每个$\delta \geqslant \alpha$，都存在$\gamma \in I$，使得$\gamma \geqslant \delta$和$\gamma \geqslant \beta$，因而$f_{\alpha\gamma}(A_\gamma) \subset f_{\alpha\delta}(A_\delta)$，因而

$$\bigcap_{\gamma \geqslant \beta} f_{\alpha\gamma}(A_\gamma) = \bigcap_{\delta \geqslant \alpha} f_{\alpha\delta}(A_\delta) = A'_\alpha.$$

因而 $\mathfrak{A}'$ 满足 (21)，因此属于到 $\Sigma$。由于$A'_\alpha \subset A_\alpha$对于所有$\alpha$，$\Sigma$中$\mathfrak{A}$的最大值意味着$\mathfrak{A}' = \mathfrak{A}$，并且我们的断言被证明。

(3) 接下来我们将确定，如果$\mathfrak{A} = (A_\alpha)$是$\Sigma$的*极大*元素，那么每个$A_\alpha$*都由单个元素*组成。让$x_\alpha \in A_\alpha$。对于每个$\beta \geqslant \alpha$，放入$B_\beta = A_\beta \cap \overset{-1}{f}_{\alpha\beta}(x_\alpha)$；如果$\beta$不是$\geqslant \alpha$，则放入$B_\beta = A_\beta$；那么我们将看到$\mathfrak{B} = (B_\beta)$属于到$\Sigma$。如果$\beta$不是$\geqslant \alpha$，则关系$\beta \leqslant \gamma$意味着$f_{\beta\gamma}(B_\gamma) \subset f_{\beta\gamma}(A_\gamma) \subset A_\beta = B_\beta$。另一方面，如果$\alpha \leqslant \beta \leqslant \gamma$，那么从那时起

$$\overset{-1}{f}_{\alpha\gamma}(x_\alpha) = \overset{-1}{f}_{\beta\gamma}(\overset{-1}{f}_{\alpha\beta}(x_\alpha)),$$

我们有

$$f_{\beta\gamma}(\overset{-1}{f}_{\alpha\gamma}(x_\alpha)) \subset \overset{-1}{f}_{\alpha\beta}(x_\alpha),$$

从$f_{\beta\gamma}(A_\gamma) \subset A_\beta$开始，我们又得到了$f_{\beta\gamma}(B_\gamma) \subset B_\beta$，因此族$\mathfrak{B}$满足(21)。由于$A_\alpha = f_{\alpha\beta}(A_\beta)$每当$\alpha \leqslant \beta$乘以证明的部分(2)，显然$\mathrm{B}_\beta \neq \emptyset$对于所有$\beta \in \mathrm{I}$。最后，根据 (i) 和 (iii)，对于所有 $\beta \in \mathrm{I}$，我们有 $\mathrm{B}_\beta \in \mathfrak{S}_\beta$，因此也有 $\mathfrak{B} \in \Sigma$。由于$\mathrm{B}_\beta \subset \mathrm{A}_\beta$对于所有$\beta \in \mathrm{I}$，$\mathfrak{A}$的最大值意味着$\mathrm{B}_\beta = \mathrm{A}_\beta$对于所有$\beta$，特别是$\mathrm{A}_\alpha = \{x_\alpha\}$。

(4) 我们现在可以证明定理 1。让我们从(a)开始。我们有

$$f_\alpha(\mathrm{E}) \subset \bigcap_{\beta \geqslant \alpha} f_{\alpha\beta}(\mathrm{E}_\beta).$$

相反，让

$$x_\alpha \in \bigcap_{\beta \geqslant \alpha} f_{\alpha\beta}(\mathrm{E}_\beta),$$

并把

$$\mathrm{B}_\beta = \overset{-1}{f}_{\alpha\beta}(x_\alpha)$$

如果$\beta \geqslant \alpha$，则$\mathrm{B}_\beta = \mathrm{E}_\beta$。到 $x_\alpha$ 的定义时，$\mathrm{B}_\beta$ 非空，并且凭借 (iii) 和 (i)，我们对所有 $\beta \in \mathrm{I}$ 拥有 $\mathrm{B}_\beta \in \mathfrak{S}_\beta$；此外，很明显，每当$\beta \leqslant \gamma$时，$f_{\beta\gamma}(\mathrm{B}_\gamma) \subset \mathrm{B}_\beta$。因此$\mathfrak{B} = (\mathrm{B}_\beta) \in \Sigma$。令$\mathfrak{A} = (\mathrm{A}_\alpha)$为$\Sigma$的极大元素，使得$\mathfrak{A} \geqslant \mathfrak{B}$（$\mathfrak{A}$的存在性由(1)和§2, no. 4、定理2得出，推论1）。由于根据 (3)，对于所有 $\beta \in \mathrm{I}$，$\mathrm{A}_\beta$ 是形式 $\{y_\beta\}$，因此，$y = (y_\beta)$ 属于到 E，以及 $f_\alpha(y) = y_\alpha = x_\alpha$ 定义。

最后，(a) 暗示(b)。我们不妨假设I不为空（否则没有什么可证明的）。 假设 $\mathrm{E}_\alpha$ 非空意味着 $f_{\alpha\beta}(\mathrm{E}_\beta) \neq \emptyset$ 对于所有 $\beta \geqslant \alpha$。由于$f_{\alpha\beta}(\mathrm{E}_\beta)$，对于固定$\alpha$和可变$\beta \geqslant \alpha$，形式$\mathrm{E}_\alpha$属于的子集左有向集合到$\mathfrak{S}_\alpha$，条件 (ii)$'$证明那个

$$\bigcap_{\beta \geqslant \alpha} f_{\alpha\beta}(\mathrm{E}_\beta) \neq \emptyset.$$

因此 (a) 为 $f_\alpha(\mathrm{E}) \neq \emptyset$，并且 *更不必说* $\mathrm{E} \neq \emptyset$。 Q.E.D.

#### 注 {#ens-iii-s7-n4-rem-1 .statement tag=03OJ}

假设定理 1 中的条件 (iii) 被以下较弱的条件替换：

(iii)$'$ *对于每个* $\alpha \in \mathrm{I}$ *和每个非空集合* $\mathrm{M}_\alpha \in \mathfrak{S}_\alpha$ *存在* $x_\alpha \in \mathrm{M}_\alpha$ *使得* $\overset{-1}{f}_{\alpha\beta}(x_\alpha) \in \mathfrak{S}_\beta$ *对于每个* $\beta \geqslant \alpha$。

那么定理1的结论(b)仍然成立； 部分 (1) 的证明和定理 1 的 (2) 保持不变，并且部分 (3) 的证明仍然有效，前提是我们小心地采用 $x_\alpha \in \mathrm{A}_\alpha$，使得 $\overset{-1}{f}_{\alpha\beta}(x_\alpha)$ 属于到 $\mathfrak{S}_\beta$ 对于所有$\beta \geqslant \alpha$。最后，(4) 的证明表明，如果

$$\bigcap_{\beta \geqslant \alpha} f_{\alpha\beta}(\mathrm{E}_\beta) \neq \emptyset$$

如果我们在这个集合中选择一个$x_\alpha$，使得$\overset{-1}{f}_{\alpha\beta}(x_\alpha) \in \mathfrak{S}_\beta$每当$\beta \geqslant \alpha$时，都存在$y \in E$使得$f_\alpha(y) = x_\alpha$，这证明了我们的断言。

*例*

#### 例 1 {#ens-iii-s7-n4-exa-1 .statement tag=03TK}

如果$E_\alpha$是*有限*集合，则可以通过将$\mathfrak{S}_\alpha$取为$E_\alpha$的*所有*子集的集合来应用定理1。 \* 这个例在*一般拓扑*中被推广到其中$E_\alpha$是*紧凑*拓扑空间、$f_{\alpha\beta}$*连续*映射、以及*封闭*子集的$\mathfrak{S}_\alpha$集合的情况$E_\alpha$（*一般拓扑*、章I, § 9, no. 6）。 \*

#### 例 2 {#ens-iii-s7-n4-exa-2 .statement tag=03TL}

\* 设 A 为环和单位元素，对于每个 $\alpha \in I$，令 $T_\alpha$ 为 *阿廷的* 左A-模。令$E_\alpha$为$T_\alpha$的*同质空间*，$T_\alpha$忠实地在其上运行（因此$E_\alpha$是附加到$T_\alpha$的*仿射空间*）。对于 $\beta \geqslant \alpha$，假设 $f_{\alpha\beta} : E_\beta \to E_\alpha$ 是*仿射映射*。取$\mathfrak{S}_\alpha$为空集的集合由……组成以及$E_\alpha$中的*仿射线性簇*。那么条件 (i) 是平凡满足的，并且 (ii) 由$T_\alpha$ 是阿廷的的事实得出；因为这意味着在集合的有限交集合 $M \in \mathfrak{F}$ 中存在最小元素，并且这个最小元素必须等于 $\bigcap_{M \in \mathfrak{F}} M$。最后，由于 $f_{\alpha\beta}$ 是仿射的，条件 (iii) 和 (iv) 是简单满足的。 \*

### 5. 直极限

令I为（*右*）*定向*预排序的集合，并让$(E_\alpha)_{\alpha \in I}$为由I索引的集合族。对于I的元素的每个对$(\alpha, \beta)$使得$\alpha \leqslant \beta$，令$f_{\beta\alpha}$是*$E_\alpha$*到*$E_\beta$的*映射。假设 $f_{\beta\alpha}$ 满足以下条件 ：

(LI$_\mathrm{I}$) *关系* $\alpha \leqslant \beta \leqslant \gamma$ *暗示* $f_{\gamma\alpha} = f_{\gamma\beta} \circ f_{\beta\alpha}$。
(LI$_\mathrm{II}$) *对于每个* $\alpha \in I, f_{\alpha\alpha}$ *是* $E_\alpha$ 的恒等映射。

Let G be the set which is the *sum* of the family of sets $(E_\alpha)_{\alpha \in I}$ (Chapter II, § 4, no. 8); by abuse of language, we shall identify the $E_\alpha$ with their canonical images in G, and for each $x \in G$ we shall denote by $\lambda(x)$ the unique index $\alpha \in I$ such that $x \in E_\alpha$. 让$R\{x, y\}$表示G的两个元素、$x$、$y$之间的关系：“存在元素$\gamma \in I$使得$\gamma \geqslant \alpha = \lambda(x)$和$\gamma \geqslant \beta = \lambda(y)$对于$f_{\gamma\alpha}(x) = f_{\gamma\beta}(y)$”。 那么 R 是 *G 上的 *等价关系。 显然，R 在 G 上是自反且对称的。 为了证明 R 是传递性的，设$x \in E_\alpha, y \in E_\beta, z \in E_\gamma$，并假设存在$\lambda \in I$使得$\lambda \geqslant \alpha$、$\lambda \geqslant \beta$和$f_{\lambda\alpha}(x) = f_{\lambda\beta}(y)$，以及$\mu \in I$使得$\mu \geqslant \beta$、$\mu \geqslant \gamma$和$f_{\mu\beta}(y) = f_{\mu\gamma}(z)$。 由于I是有向集合，因此存在$\nu \in I$使得$\nu \geqslant \lambda$和$\nu \geqslant \mu$；

到 $(\mathrm{LI_I})$ 我们就有

$$f_{\nu\alpha}(x) = f_{\nu\lambda}(f_{\lambda\alpha}(x)) = f_{\nu\lambda}(f_{\lambda\beta}(y)) = f_{\nu\beta}(y)$$
$$= f_{\nu\mu}(f_{\mu\beta}(y)) = f_{\nu\mu}(f_{\mu\gamma}(z)) = f_{\nu\gamma}(z),$$

这就建立了我们的断言。 商集 $\mathrm{E} = \mathrm{G/R}$ 相对于映射* $(f_{\beta\alpha})$ 的家族被称为 *直极限家族* $(\mathrm{E}_\alpha)_{\alpha \in \mathrm{I}}$ *，并写作 $\mathrm{E} = \varinjlim (\mathrm{E}_\alpha, f_{\beta\alpha})$，或在不存在歧义的情况下简称为 $\mathrm{E} = \varinjlim \mathrm{E}_\alpha$。通过滥用语言，对$((\mathrm{E}_\alpha), (f_{\beta\alpha}))$（通常写作$(\mathrm{E}_\alpha, f_{\beta\alpha})$）被称为集合*的*直接系统，相对于有向集合I。

¶ 显然，只要 $\mathrm{E}_\alpha$ 中至少有一个不为空，E 就不为空。我们用G的典范映射$f$的$f_\alpha$限制到$\mathrm{E}_\alpha$到$\mathrm{E} = \mathrm{G/R}$来表示； $f_\alpha$ 被称为 $\mathrm{E}_\alpha$ 到 E 中的*典范映射*。如果$\alpha \leqslant \beta$，我们有关系

(22) $$f_\beta \circ f_{\beta\alpha} = f_\alpha$$

因为对于每个$x \in \mathrm{E}_\alpha$，我们有$f_{\beta\beta}(f_{\beta\alpha}(x)) = f_{\beta\alpha}(x)$乘以$(\mathrm{LI_I})$；因此元素 $x \in \mathrm{E}_\alpha$ 和 $f_{\beta\alpha}(x) \in \mathrm{E}_\beta$ 是全等的 mod R。

*例*

#### 例 1 {#ens-iii-s7-n5-exa-1 .statement tag=03TM}

设A，B为两个集合，并令$(\mathrm{V}_\alpha)_{\alpha \in \mathrm{I}}$为A的子集族，其指标集合I是有向的，并且使得关系$\alpha \leqslant \beta$蕴涵$\mathrm{V}_\beta \subset \mathrm{V}_\alpha$。让$\mathrm{E}_\alpha$表示B中$\mathrm{V}_\alpha$的所有映射的集合，并且对于指标$(\alpha, \beta)$的每个对，使得$\alpha \leqslant \beta$让$f_{\beta\alpha}$成为$\mathrm{E}_\alpha$的映射进入$\mathrm{E}_\beta$ 将每个函数 $u \in \mathrm{E}_\alpha$ 发送到其 *限制* 到 $\mathrm{V}_\beta$。显然，条件$(\mathrm{LI_I})$和$(\mathrm{LI_{II}})$满足，集合$\mathrm{E} = \varinjlim \mathrm{E}_\alpha$被称为$\mathrm{V}_\alpha$的映射**菌的集合进入B。\*最常见的情况是$(\mathrm{V}_\alpha)$是拓扑空间 A 的子集 *邻域*（*一般拓扑*、章 I, §6, no. 10）。 \*

#### 例 2 {#ens-iii-s7-n5-exa-2 .statement tag=03TN}

假设对于每个 $\alpha \in \mathrm{I}$，$\mathrm{E}_\alpha$ 都是相同的集合 F，并且无论何时 $\alpha \leqslant \beta$，$f_{\beta\alpha}$ 都是 F 自身的恒等映射。那么存在$\varinjlim \mathrm{E}_\alpha$到F的*规范双射*。在序到定义$\varinjlim \mathrm{E}_\alpha$，我们必须形式集合G，这是$(\mathrm{E}_\alpha)$族的和；因此，G 是相互不相交的集合的$(\mathrm{G}_\alpha)$族的并，并且对于每个$\alpha \in \mathrm{I}$，都有一个规范的双射$h_\alpha : \mathrm{F} \to \mathrm{G}_\alpha$。接下来我们要考虑 G 相应的到划分 $(\mathrm{P}_y)_{y \in \mathrm{F}}$ 上的等价关系 R，其中 $\mathrm{P}_y$ 是所有 $h_\alpha(y)$ 的集合，因为 $\alpha$ 穿过 I。显然，$y \to \mathrm{P}_y$ 是双射，其逆是双射。我们将通过这个规范的双射将认同F与$\varinjlim \mathrm{E}_\alpha$进行组合。

#### 引理 1 {#ens-iii-s7-lem-1 .statement tag=03OK}

*设*$(\mathrm{E}_\alpha, f_{\beta\alpha})$*为集合的直接系统，*$\mathrm{E} = \varinjlim \mathrm{E}_\alpha$*其直极限，并且对于每个*$\alpha \in \mathrm{I}$*让*$f_\alpha \colon \mathrm{E}_\alpha \to \mathrm{E}$*典范映射。*

(i) *令 $(x^{(i)})_{1 \leqslant i \leqslant n}$ 为* E 的元素的有限系统。 *则存在* $\alpha \in I$ *和* $E_\alpha$ *的元素的有限系统* $(x_\alpha^{(i)})_{1 \leqslant i \leqslant n}$ *这样* $x^{(i)} = f_\alpha(x_\alpha^{(i)})$*对于*$1 \leqslant i \leqslant n$。

(ii) *设* $(y_\alpha^{(i)})_{1 \leqslant i \leqslant n}$ *为某些* $E_\alpha$ 的元素的有限系统。 *如果*$f_\alpha(y_\alpha^{(i)}) = f_\alpha(y_\alpha^{(j)})$*对于指标*$(i, j)$的每个对，*则存在*$\beta \geqslant \alpha$*使得*$f_{\beta\alpha}(y_\alpha^{(i)}) = f_{\beta\alpha}(y_\alpha^{(j)})$*对于每个对*$(i, j)$。

(i) 通过 E 的定义，每个 $i$ 指标 $\beta_i \in I$ 和元素 $z_{\beta_i} \in E_{\beta_i}$ 都存在$x^{(i)} = f_{\beta_i}(z_{\beta_i})$。取$\alpha$，使得$\alpha \geqslant \beta_i$代表$1 \leqslant i \leqslant n$，以及$x_\alpha^{(i)} = f_{\alpha\beta_i}(z_{\beta_i})$。

(ii) 通过 E 的定义，对于每个对$(i, j)$，存在$\gamma_{ij} \in I$，使得$\gamma_{ij} \geqslant \alpha$和$f_{\gamma_{ij}\alpha}(y_\alpha^{(i)}) = f_{\gamma_{ij}\alpha}(y_\alpha^{(j)})$。采用 $\beta$ 使得 $\beta \geqslant \gamma_{ij}$ 对于所有对 $(i, j)$，并使用关系 $f_{\beta\alpha} = f_{\beta\gamma_{ij}} \circ f_{\gamma_{ij}\alpha}$。

### 6. 直接系统 / 映射

#### 命题 6 {#ens-iii-s7-prop-6 .statement tag=03RR}

*设*I*为有向集合，让*$(E_\alpha, f_{\beta\alpha})$*为集合相对于*I的直接系统，*让*$E = \varinjlim E_\alpha$*为直极限，并且对于每个*$\alpha \in I$*让*

$$f_\alpha : E_\alpha \to E$$

*为典范映射。对于每个* $\alpha \in I$，*让* $u_\alpha$ *成为* $E_\alpha$ *的映射 *进入集合* F *这样*

(23) $$u_\beta \circ f_{\beta\alpha} = u_\alpha \qquad \textit{whenever } \alpha \leqslant \beta.$$

*然后：*

(a) *存在唯一映射* $u$ *E *进入* F *这样*

(24) $$u_\alpha = u \circ f_\alpha \qquad \textit{for all } \alpha \in I.$$

(b) $u$ *是满射当且仅当* F *是并 of 集合* $u_\alpha(E_\alpha)$。

(c) $u$ *是单射当且仅当对于每个* $\alpha \in I$ *关系* $x \in E_\alpha$、$y \in E_\alpha$、$u_\alpha(x) = u_\alpha(y)$ *意味着存在* $\beta \geqslant \alpha$ *使得* $f_{\beta\alpha}(x) = f_{\beta\alpha}(y)$。

(a) 对于no. 5的记号，令$v$为G到F中的映射，对于每个$\alpha \in I$（章II, § 4, no. 7，命题8），它与$E_\alpha$上的$u_\alpha$一致。 假设意味着$v$ 与等价关系 R 相容的（章 II, § 6, no. 5）；因此，F 中存在 $E = G/R$ 的唯一映射 $u$，使得 $v = u \circ f$ (*loc.cit.*)。

(b) 由于 E 是 $f_\alpha(E_\alpha)$ 的并，因此关系 $F = \bigcup_{\alpha \in I} u_\alpha(E_\alpha)$ 显然对于$u$ 是满射而言是充分必要的。

(c) 通过no. 5的引理 1，$\mathbf{E}$的任何两个元素总是可以写成形式$f_\alpha(x)$和$f_\alpha(y)$，其中$x \in \mathrm{E}_\alpha$和$y \in \mathrm{E}_\alpha$，对于合适的选择 $\alpha \in \mathrm{I}$。从引理还可以得出，关系$f_\alpha(x) = f_\alpha(y)$等价于$\beta \geqslant \alpha$的存在，使得$f_{\beta\alpha}(x) = f_{\beta\alpha}(y)$。从$u_\alpha(x) = u(f_\alpha(x))$和$u_\alpha(y) = u(f_\alpha(y))$开始，这完成了证明。

¶ 如果映射 $u$ 是*双射的*，则有时通过滥用语言表示，F 是$(\mathrm{E}_\alpha)$ 家族的直极限。

#### 注 {#ens-iii-s7-n6-rem-1 .statement tag=03OL}

假设映射 $f_{\beta\alpha}$ 中的每一个都是*内射*。那么每个$f_\alpha$都是*单射的*，通过关系R的定义。在这种情况下，我们通常认同$\mathrm{E}_\alpha$和$f_\alpha(\mathrm{E}_\alpha)$，因此将E视为$\mathrm{E}_\alpha$的*并*。相反，令$(\mathrm{F}_\alpha)_{\alpha \in \mathrm{I}}$为集合F的子集的递增族，并假设F是该族的*并*。如果$j_{\beta\alpha}$将$\mathrm{F}_\alpha$的典范嵌入表示为$\alpha \leqslant \beta$的$\mathrm{F}_\beta$，那么从命题6可以得出认同F与$\mathrm{F}_\alpha$家族的直极限F关于映射的家族对于每个$\alpha \in \mathrm{I}$，将$(j_{\beta\alpha})$和$\mathrm{F}_\alpha$的典范映射转换为$\varinjlim \mathrm{F}_\alpha$，将$\mathrm{F}_\alpha$的典范嵌入转换为F。

#### 推论 1 {#ens-iii-s7-prop-6-cor-1 .statement tag=03RS}

*令*$(\mathrm{E}_\alpha, f_{\beta\alpha})$*和*$(\mathrm{F}_\alpha, g_{\beta\alpha})$*为集合中的两个直接系统相对于相同的指标集合*I； *让* $\mathrm{E} = \varinjlim \mathrm{E}_\alpha$，$\mathrm{F} = \varinjlim \mathrm{F}_\alpha$，*并且对于每个* $\alpha \in \mathrm{I}$ *让* $f_\alpha$（*分别* $g_\alpha$）*成为* $\mathrm{E}_\alpha$（*分别* $\mathrm{F}_\alpha$）的典范映射*进入* E（*分别* F）。 *对于每个* $\alpha \in \mathrm{I}$ *让* $u_\alpha$ *成为* $\mathrm{E}_\alpha$ *的映射 *进入* $\mathrm{F}_\alpha$ *这样，每当* $\alpha \leqslant \beta$，*图表*

$$\begin{array}{ccc} \mathrm{E}_\alpha & \overset{u_\alpha}{\longrightarrow} & \mathrm{F}_\alpha \\ {\scriptstyle f_{\beta\alpha}}\big\downarrow & & \big\downarrow{\scriptstyle g_{\beta\alpha}} \\ \mathrm{E}_\beta & \underset{u_\beta}{\longrightarrow} & \mathrm{F}_\beta \end{array}$$

* 是可交换的。那么存在唯一映射* $u : \mathrm{E} \rightarrow \mathrm{F}$ *这样，对于每个* $\alpha \in \mathrm{I}$，*图表*

$$\begin{array}{ccc} \mathrm{E}_\alpha & \overset{u_\alpha}{\longrightarrow} & \mathrm{F}_\alpha \\ {\scriptstyle f_\alpha}\big\downarrow & & \big\downarrow{\scriptstyle g_\alpha} \\ \mathrm{E} & \underset{u}{\longrightarrow} & \mathrm{F} \end{array}$$

*是可交换的。*

把$v_\alpha = g_\alpha \circ u_\alpha$。如果 $\alpha \leqslant \beta$，则由 (22) 我们有

$$v_\beta \circ f_{\beta\alpha} = g_\beta \circ u_\beta \circ f_{\beta\alpha} = g_\beta \circ g_{\beta\alpha} \circ u_\alpha = g_\alpha \circ u_\alpha = v_\alpha.$$

因此，我们可以应用命题 6 到映射 $v_\alpha$，从而映射 $u : \mathrm{E} \to \mathrm{F}$ 的存在和唯一性使得

$$u \circ f_\alpha = v_\alpha = g_\alpha \circ u_\alpha$$

对于所有$\alpha \in \mathrm{I}$。

¶ 满足推论 1 的条件的映射 $u_\alpha : \mathrm{E}_\alpha \to \mathrm{F}_\alpha$ 族称为 $(\mathrm{E}_\alpha, f_{\beta\alpha})$ 的映射* 的 *直接系统到 $(\mathrm{F}_\alpha, g_{\beta\alpha})$。推论1中定义的映射被称为$(u_\alpha)$族的*直极限*，并且在不存在歧义的情况下写作$u = \varinjlim u_\alpha$。

#### 推论 2 {#ens-iii-s7-prop-6-cor-2 .statement tag=03RT}

*令*$(\mathrm{E}_\alpha, f_{\beta\alpha})$、$(\mathrm{F}_\alpha, g_{\beta\alpha})$、$(\mathrm{G}_\alpha, h_{\beta\alpha})$*为集合相对于*I的三个直接系统。 *令* $\mathrm{E} = \varinjlim \mathrm{E}_\alpha$、$\mathrm{F} = \varinjlim \mathrm{F}_\alpha$、$\mathrm{G} = \varinjlim \mathrm{G}_\alpha$、*并令* $f_\alpha$ *（分别* $g_\alpha$、$h_\alpha$*）为* $\mathrm{E}_\alpha$ *（分别* $\mathrm{F}_\alpha$、$\mathrm{G}_\alpha$*）的典范映射* E *（分别* F、G*）。如果*$(u_\alpha)$*和*$(v_\alpha)$*是映射*$u_\alpha : \mathrm{E}_\alpha \to \mathrm{F}_\alpha$、$v_\alpha : \mathrm{F}_\alpha \to \mathrm{G}_\alpha$中的两个直接系统，*则映射中的映射*$v_\alpha \circ u_\alpha : \mathrm{E}_\alpha \to \mathrm{G}_\alpha$*形式直接系统，我们有*

(25) $$\varinjlim (v_\alpha \circ u_\alpha) = (\varinjlim v_\alpha) \circ (\varinjlim u_\alpha).$$

因为如果我们输入$w_\alpha = v_\alpha \circ u_\alpha$，那么对于$\alpha \leqslant \beta$，我们有

$$h_{\beta\alpha} \circ w_\alpha = (h_{\beta\alpha} \circ v_\alpha) \circ u_\alpha = (v_\beta \circ g_{\beta\alpha}) \circ u_\alpha = v_\beta \circ (u_\beta \circ f_{\beta\alpha}) = w_\beta \circ f_{\beta\alpha},$$

这表明 $(w_\alpha)$ 是映射的直接系统。此外，如果 $u = \varinjlim u_\alpha$ 和 $v = \varinjlim v_\alpha$，那么对于所有 $\alpha \in \mathrm{I}$ 我们有

$$(v \circ u) \circ f_\alpha = v \circ (g_\alpha \circ u_\alpha) = h_\alpha \circ (v_\alpha \circ u_\alpha),$$

凭借直极限的唯一性，我们有$v \circ u = \varinjlim w_\alpha$。

#### 命题 7 {#ens-iii-s7-prop-7 .statement tag=03RU}

*令*$(\mathrm{E}_\alpha, f_{\beta\alpha})$*和*$(\mathrm{E}'_\alpha, f'_{\beta\alpha})$*为集合的两个直接系统相对于*I，*并且对于每个*$\alpha \in \mathrm{I}$*让*$u_\alpha$*为*$\mathrm{E}_\alpha$*的映射*到* $\mathrm{E}'_\alpha$*使得映射的*$u_\alpha$*形式直接系统。让*$u = \varinjlim u_\alpha$。 *如果每个* $u_\alpha$ *是单射*（或*满射*）*则* $u$ *是单射*（或*满射*）。

令$\mathrm{E} = \varinjlim \mathrm{E}_\alpha$、$\mathrm{E}' = \varinjlim \mathrm{E}'_\alpha$，并令$f_\alpha : \mathrm{E}_\alpha \to \mathrm{E}$、$f'_\alpha : \mathrm{E}'_\alpha \to \mathrm{E}'$为典范映射。假设每个 $u_\alpha$ 都是单射的。为了证明$u$是单射的，通过命题6，验证如果$x \in \mathrm{E}_\alpha$和$y \in \mathrm{E}_\alpha$使得$f'_\alpha(u_\alpha(x)) = f'_\alpha(u_\alpha(y))$，那么存在$\beta \geqslant \alpha$使得$f_{\beta\alpha}(x) = f_{\beta\alpha}(y)$。现在假设意味着 (no. 6, 引理 1) 存在 $\beta \geqslant \alpha$ 使得

$$f'_{\beta\alpha}(u_\alpha(x)) = f'_{\beta\alpha}(u_\alpha(y)), \qquad \text{i.e.,} \qquad u_\beta(f_{\beta\alpha}(x)) = u_\beta(f_{\beta\alpha}(y)),$$

因此 $f_{\beta\alpha}(x) = f_{\beta\alpha}(y)$ 因为 $u_\beta$ 是单射的。

现在假设 $u_\alpha$ 是满射的。然后我们有

$$\mathrm{E}' = \bigcup_\alpha f'_\alpha(\mathrm{E}'_\alpha) = \bigcup_\alpha f'_\alpha(u_\alpha(\mathrm{E}_\alpha)) = \bigcup_\alpha u(f_\alpha(\mathrm{E}_\alpha)) = u\Big(\bigcup_\alpha f_\alpha(\mathrm{E}_\alpha)\Big) = u(\mathrm{E}).$$

当记号为命题7时，对于每个$\alpha \in \mathrm{I}$，令$\mathrm{M}_\alpha$为$\mathrm{E}_\alpha$的子集；如果每当 $\alpha \leqslant \beta$ 时我们就有 $f_{\beta\alpha}(\mathrm{M}_\alpha) \in \mathrm{M}_\beta$，则$(\mathrm{M}_\alpha)_{\alpha \in \mathrm{I}}$ 家庭被称为是* $\mathrm{E}_\alpha$ 的子集的 *直接系统。设$g_{\beta\alpha}$（其中$\alpha \leqslant \beta$）为$\mathrm{M}_\alpha$到$\mathrm{M}_\beta$的映射，其图形与$f_{\beta\alpha}$到$\mathrm{M}_\alpha$的限制的图形相同。那么显然$(\mathrm{M}_\alpha, g_{\beta\alpha})$是集合的直接系统； 命题 7，应用于典范嵌入$j_\alpha : \mathrm{M}_\alpha \to \mathrm{E}_\alpha$，允许我们通过单射$j = \varinjlim j_\alpha$*认同*$\mathrm{M} = \varinjlim \mathrm{M}_\alpha$与E的子集。

#### 推论{#ens-iii-s7-n6-cor-1 .statement tag=03ON}

*设*$(\mathrm{E}_\alpha, f_{\beta\alpha})$*和*$(\mathrm{E}'_\alpha, f'_{\beta\alpha})$*为集合之二直接系统，令*$(u_\alpha)$*为映射*$u_\alpha : \mathrm{E}_\alpha \to \mathrm{E}'_\alpha$直接系统，*且令*$u = \varinjlim u_\alpha$。

(i) *令*$(\mathrm{M}_\alpha)$*为*$\mathrm{E}_\alpha$的子集直接系统。 *那么*$(u_\alpha(\mathrm{M}_\alpha))$*是*$\mathrm{E}'_\alpha$的子集直接系统，*我们有*

(26) $$\varinjlim u_\alpha(\mathrm{M}_\alpha) = u\,(\varinjlim \mathrm{M}_\alpha).$$

(ii) *让* $(a'_\alpha)_{\alpha \in \mathbf{I}}$ *成为一个家庭，使得* $a'_\alpha \in \mathrm{E}'_\alpha$ *对于每个* $\alpha \in \mathrm{I}$ *和* $f'_{\beta\alpha}(a'_\alpha) = a'_\beta$ *每当* $\alpha \leqslant \beta$。 *然后* $\mathrm{E}_\alpha$ 子集集合* $\overset{-1}{u}_\alpha(a'_\alpha)$ *形式直接系统，*我们有*

(27) $$\varinjlim \overset{-1}{u}_\alpha(a'_\alpha) = \overset{-1}{u}(a'),$$

*其中*$a'$*是*$\varinjlim \mathrm{E}'_\alpha$的唯一元素*对于每个*$\alpha \in \mathrm{I}$，这是*$a'_\alpha$的典范像。

(i) 显然，$\mathrm{E}'_\alpha$的子集有$u_\alpha(\mathrm{M}_\alpha)$形式直接系统，我们可以写成$u_\alpha(\mathrm{M}_\alpha) = v_\alpha(\mathrm{M}_\alpha)$，其中$v_\alpha$是$\mathrm{M}_\alpha$的映射到$u_\alpha(\mathrm{M}_\alpha)$，其图形与限制 $u_\alpha$ 至 $\mathrm{M}_\alpha$。然后从命题 7 可以得出公式 (26)，因为 $v_\alpha$ 是满射的。

(ii) 设 $\mathrm{N}_\alpha = \overset{-1}{u}_\alpha(a'_\alpha)$。如果$\alpha \leqslant \beta$和$x_\alpha \in \mathrm{N}_\alpha$，那么

$$u_\beta(f_{\beta\alpha}(x_\alpha)) = f'_{\beta\alpha}(u_\alpha(x_\alpha) = f'_{\beta\alpha}(a'_\alpha) = a'_\beta;$$

因而$f_{\beta\alpha}(x_\alpha) \in \mathrm{N}_\beta$，$\mathrm{N}_\alpha$因而$\mathrm{E}_\alpha$的形式直接系统或子集。当记号证明命题 7 时，考虑元素 $x \in \varinjlim \mathrm{N}_\alpha$。存在$\alpha \in \mathrm{I}$和$x_\alpha \in \mathrm{N}_\alpha$使得$x = f_\alpha(x_\alpha)$，从而$u(x) = u(f_\alpha(x_\alpha)) = f'_\alpha(u_\alpha(x_\alpha)) = f'_\alpha(a'_\alpha) = a'$。相反，如果$x \in \overset{-1}{u}(a')$和$x = f_\alpha(x_\alpha)$对于一些$\alpha \in \mathrm{I}$和一些$x_\alpha \in \mathrm{E}_\alpha$，那么我们有$a' = u(f_\alpha(x_\alpha)) = f'_\alpha(u_\alpha(x_\alpha)) = f'_\alpha(a'_\alpha)$。因而 (no. 5, 引理 1) 存在$\beta \geqslant \alpha$使得$f'_{\beta\alpha}(u'_\alpha(x_\alpha)) = f'_{\beta\alpha}(a'_\alpha) = a'_\beta$；即$u_\alpha(f_{\beta\alpha}(x_\alpha)) = a'_\beta$，因而$f_{\beta\alpha}(x_\alpha) \in \mathrm{N}_\beta$。从$x = f_\beta(f_{\beta\alpha}(x_\alpha))$开始，得出$x \in \varinjlim \mathrm{N}_\alpha$。

#### 注 {#ens-iii-s7-n6-rem-2 .statement tag=03OO}

假设对于每个 $\alpha \in \mathrm{I}$，$u_\alpha : \mathrm{E}_\alpha \to \mathrm{E}'$ 是映射，使得族 $(u_\alpha)$ 满足 (23)。考虑直接系统$(\mathrm{E}_\alpha, i_{\beta\alpha})$相对于I，其中$\mathrm{E}'_\alpha = \mathrm{E}'$代表所有$\alpha \in \mathrm{I}$，$i_{\beta\alpha}$是$\mathrm{E}'$的恒等映射。那么(no. 5,例2)$\mathrm{E}'$可以与$\varinjlim \mathrm{E}'_\alpha$规范地识别。如果$u_\alpha$被认为是$\mathrm{E}_\alpha$的映射进入$\mathrm{E}'_\alpha$，则$(u_\alpha)$是映射的直接系统，并且由（24）定义的映射$u : \mathrm{E} \to \mathrm{E}'$与此的直极限相同系统共映射。因而，通过滥用语言，我们写了$u = \varinjlim u_\alpha$。

如果 J 是有向的 I 的子集（相对于诱导预序），则显然子族$(\mathrm{E}_\alpha)_{\alpha \in \mathrm{J}}$和族$(f_{\beta\alpha})$的对由……组成，其中$\alpha \leqslant \beta$和$\alpha \in \mathrm{J}$和$\beta \in \mathrm{J}$是相对于 J 的直接系统或集合；据说它是通过将指标集合*限制*到J而获得的。令E、E′分别表示$(\mathrm{E}_\alpha)_{\alpha \in \mathrm{I}}$和$(\mathrm{E}_\alpha)_{\alpha \in \mathrm{J}}$族的直极限，对于每个$\alpha \in \mathrm{I}$，让$f_\alpha : \mathrm{E}_\alpha \to \mathrm{E}$表示典范映射。那么$(f_\alpha)_{\alpha \in \mathrm{J}}$是映射的直接系统，因而$g = \varinjlim f_\alpha$是E′到E中的映射，称为*规范*。此外，如果 J′ 是 J 的有向子集，如果 E” 是族 $(\mathrm{E}_\alpha)_{\alpha \in \mathrm{J}'}$ 的直极限，并且如果

$$g' : \quad \mathrm{E}'' \to \mathrm{E}' \qquad \text{and} \qquad g'' : \mathrm{E}'' \to \mathrm{E}$$

是典范映射，那么从命题 6 可以立即得出

(28) $$g'' = g \circ g'.$$

#### 命题 8 {#ens-iii-s7-prop-8 .statement tag=03OP}

*设*I*为有向集合，让*$(\mathrm{E}_\alpha, f_{\beta\alpha})$*为集合相对于*I的直接系统，*并让*$\mathrm{E} = \varinjlim \mathrm{E}_\alpha$*为其直极限。令* J *为* I *的共尾子集，并令* E′ *为从* $(\mathrm{E}_\alpha, f_{\beta\alpha})$ *通过限制指标集合至* J 获得的集合直接系统的直极限。 *则典范映射* $g$ *的* E′ *到* E *是双射的。*

J 必然是有向集合 (§ 1, no. 10)。我们将使用命题 6 的判据来证明$g$是双射的。对于单射性，条件紧接在定义和引理 1 of no. 5之后。为了证明 $g$ 是满射的，我们注对于每个 $\alpha \in \mathrm{J}$ 我们有

$$g(\mathrm{E}_\alpha) = f_\alpha(\mathrm{E}_\alpha).$$

现在，对于每个$\beta \in I$，都存在$\gamma \in J$使得$\beta \leqslant \gamma$，从中可以得出$g(E_\gamma) \supset g(f_{\gamma\beta}(E_\beta)) = f_\beta(E_\beta)$。因此，E 是集合 $g(E_\alpha)$ 的并，因为 $\alpha$ 穿过 J。

### 7. 双直极限。 乘积直极限

令I、L为两个有向集合，并令$I \times L$为它们的乘积（§ 1, no. 4），加上乘积预购，又是有向集合。考虑集合$(E^\lambda_\alpha, f^{\mu\lambda}_{\beta\alpha})$相对于$I \times L$的直接系统。那么我们有

$$(29) \qquad f^{\nu\lambda}_{\gamma\alpha} = f^{\mu\nu}_{\gamma\beta} \circ f^{\mu\lambda}_{\beta\alpha}$$

每当$\alpha \leqslant \beta \leqslant \gamma$和$\lambda \leqslant \mu \leqslant \nu$时。

让E或$\varinjlim_{\alpha,\lambda} E^\lambda_\alpha$表示这个直接系统的直极限。对于每个$\lambda \in L$，放入$g^\lambda_{\beta\alpha} = f^{\lambda\lambda}_{\beta\alpha} : E^\lambda_\alpha \to E^\lambda_\beta$。然后从 (29) 我们有

$$(30) \qquad g^\lambda_{\gamma\alpha} = g^\lambda_{\gamma\beta} \circ g^\lambda_{\beta\alpha} \qquad \text{whenever } \alpha \leqslant \beta \leqslant \gamma;$$

在其他字中，$(E^\lambda_\alpha, g^\lambda_{\beta\alpha})$是集合相对于I的直接系统。让$F^\lambda = \varinjlim_\alpha E^\lambda_\alpha$表示它的直极限。如果$\lambda \leqslant \mu$固定为L的元素，则从(29)可以得出映射$h^{\mu\lambda}_\alpha = f^{\lambda\mu}_{\alpha\alpha} : E^\lambda_\alpha \to E^\mu_\alpha$形式直接系统映射。让$h^{\mu\lambda} = \varinjlim_\alpha h^{\mu\lambda}_\alpha : F^\lambda \to F^\mu$表示映射的系统中的直极限。如果$\lambda \leqslant \mu \leqslant \nu$在L中，那么

$$(31) \qquad h^{\nu\lambda} = h^{\nu\mu} \circ h^{\mu\lambda}$$

（no. 6，命题 6，推论 2），因此 $(F^\lambda, h^{\mu\lambda})$ 是集合相对于 L 的直接系统。令$F = \varinjlim F^\lambda$为其直极限。我们将定义*规范的双射*$E \to F$。为此，让$g^\lambda_\alpha$表示典范映射$E^\lambda_\alpha \to F^\lambda$，$h^\lambda$典范映射$F^\lambda \to F$，并放入$u^\lambda_\alpha = h^\lambda \circ g^\lambda_\alpha$。如果$\alpha \leqslant \beta$和$\lambda \leqslant \mu$，那么我们有

$$\begin{aligned} u^\mu_\beta \circ f^{\mu\lambda}_{\beta\alpha} &= h^\mu \circ g^\mu_\beta \circ f^{\mu\lambda}_{\beta\alpha} = h^\mu \circ g^\mu_\beta \circ f^{\mu\mu}_{\beta\alpha} \circ f^{\mu\lambda}_{\alpha\alpha} = h^\mu \circ g^\mu_\alpha \circ f^{\mu\lambda}_{\alpha\alpha} \\ &= h^\mu \circ h^{\mu\lambda} \circ g^\lambda_\alpha = h^\lambda \circ g^\lambda_\alpha = u^\lambda_\alpha \end{aligned}$$

来自 (29) 和 $h^{\mu\lambda}$ 的定义。因此，映射相对于$I \times L$的$u^\lambda_\alpha$形式直接系统。把$u = \varinjlim_{\alpha,\lambda} u^\lambda_\alpha : E \to F$。我们将证明$u$是no. 6、命题6的应用判据的双射。首先，F是集合$h^\lambda(F^\lambda)$的并，并且每个$F^\lambda$是并共集合 $g_\alpha^\lambda(\mathrm{E}_\alpha^\lambda)$；因此 F 是集合的并

$$h^\lambda(g_\alpha^\lambda(\mathrm{E}_\alpha^\lambda)) = u_\alpha^\lambda(\mathrm{E}_\alpha^\lambda).$$

接下来，令$x$、$y$为$\mathrm{E}_\alpha^\lambda$的两个元素，使得$u_\alpha^\lambda(x) = u_\alpha^\lambda(y)$，即$h^\lambda(g_\alpha^\lambda(x)) = h^\lambda(g_\alpha^\lambda(y))$。那么(no. 5,引理1)存在$\mu \geqslant \lambda$使得$h^{\mu\lambda}(g_\alpha^\lambda(x)) = h^{\mu\lambda}(g_\alpha^\lambda(y))$，即$g_\alpha^\mu(f_{\alpha\alpha}^{\mu\lambda}(x)) = g_\alpha^\mu(f_{\alpha\alpha}^{\mu\lambda}(y))$；同样，存在$\beta \geqslant \alpha$使得$g_{\beta\alpha}^\mu(f_{\alpha\alpha}^{\mu\lambda}(x)) = g_{\beta\alpha}^\mu(f_{\alpha\alpha}^{\mu\lambda}(y))$（no. 5，引理1），即$f_{\beta\alpha}^{\mu\lambda}(x) = f_{\beta\alpha}^{\mu\lambda}(y)$；这表明 (no. 6, 命题 6) $u$ 是单射的。因此我们证明了：

#### 命题 9 {#ens-iii-s7-prop-9 .statement tag=03RV}

*如果* $(\mathrm{E}_\alpha^\lambda, f_{\beta\alpha}^{\mu\lambda})$ *是集合的直接系统相对于乘积* $\mathrm{I} \times \mathrm{L}$ *两个有向集合，那么（直到规范的双射）我们有*

(32)
$$\varinjlim_{\alpha,\ \lambda} \mathrm{E}_\alpha^\lambda = \varinjlim_{\lambda}\ (\varinjlim_{\alpha} \mathrm{E}_\alpha^\lambda).$$

#### 推论{#ens-iii-s7-n7-cor-1 .statement tag=03OQ}

*令*$(\mathrm{{E}'}^\lambda_\alpha, {f'}^{\mu\lambda}_{\beta\alpha})$*成为集合的另一个直接系统相对于*$\mathrm{I} \times \mathrm{L}$，*并且对于每个*$(\alpha, \lambda) \in \mathrm{I} \times \mathrm{L}$*让*$u_\alpha^\lambda$*成为*$\mathrm{E}_\alpha^\lambda$*的映射*到*$\mathrm{{E}'}^\lambda_\alpha$，*使得* $u_\alpha^\lambda$ *形式直接系统共映射。然后我们有*

(33)
$$\varinjlim_{\alpha,\ \lambda} u_\alpha^\lambda = \varinjlim_{\lambda}\ (\varinjlim_{\alpha} u_\alpha^\lambda).$$

我们将验证留给读者。

#### 命题 10 {#ens-iii-s7-prop-10 .statement tag=03RW}

*令*$(\mathrm{E}_\alpha, f_{\beta\alpha})$*和*$(\mathrm{E}'_\alpha, f'_{\beta\alpha})$*为集合中的两个直接系统，两者都相对于相同的有向集合*I。 *让* $\mathrm{E} = \varinjlim \mathrm{E}_\alpha$、$\mathrm{E}' = \varinjlim \mathrm{E}'_\alpha$、*并让* $f_\alpha : \mathrm{E}_\alpha \to \mathrm{E}, f'_\alpha : \mathrm{E}'_\alpha \to \mathrm{E}'$ *表示典范映射，对于每个* $\alpha \in \mathrm{I}$。 *那么*$(\mathrm{E}_\alpha \times \mathrm{E}'_\alpha, f_{\beta\alpha} \times f'_{\beta\alpha})$*是集合的直接系统，*$(f_\alpha \times f'_\alpha)$*是映射的直接系统，并且*$\varinjlim (f_\alpha \times f'_\alpha)$*是双射*

(34)
$$\varinjlim (\mathrm{E}_\alpha \times \mathrm{E}'_\alpha) \to (\varinjlim \mathrm{E}_\alpha) \times (\varinjlim \mathrm{E}'_\alpha).$$

命题的前两个断言立即得到验证。为了证明 $g = \varinjlim (f_\alpha \times f'_\alpha)$ 是双射的，我们计算 no. 6 的应用命题 6。显然$\mathrm{E} \times \mathrm{E}'$是集合$f_\alpha(\mathrm{E}_\alpha) \times f'_\alpha(\mathrm{E}'_\alpha)$中的并；因此 $g$ 是满射的。如果$(x, x')$和$(y, y')$是$\mathrm{E}_\alpha \times \mathrm{E}'_\alpha$的两个元素使得$f_\alpha(x) = f_\alpha(y)$和$f'_\alpha(x') = f'_\alpha(y')$，则(no. 5，引理1)存在两个元素$\beta$，$\gamma$ I使得$\beta \geqslant \alpha$、$\gamma \geqslant \alpha$和$f_{\beta\alpha}(x) = f_{\beta\alpha}(y)$、$f'_{\gamma\alpha}(x') = f'_{\gamma\alpha}(y')$；由于I是有向的，因此存在$\delta \in \mathrm{I}$使得$\delta \geqslant \beta$和$\delta \geqslant \gamma$；因此$f_{\delta\alpha}(x) = f_{\delta\alpha}(y)$和$f'_{\delta\alpha}(x') = f'_{\delta\alpha}(y')$。这样就完成了证明。

双射 $g$ 被称为*规范*。

#### 推论{#ens-iii-s7-n7-cor-2 .statement tag=03RX}

*设*$(\mathrm{F}_\alpha, g_{\beta\alpha})$*和*$(\mathrm{F}'_\alpha, g'_{\beta\alpha})$*为集合的两个直接系统相对于*I，*并且对于每个*$\alpha \in \mathrm{I}$*让*$u_\alpha : \mathrm{E}_\alpha \to \mathrm{F}_\alpha$，$u'_\alpha : \mathrm{E}'_\alpha \to \mathrm{F}'_\alpha$*为映射使得*$(u_\alpha)$*和* $(u'_\alpha)$ *是映射中的两个直接系统。那么* $(u_\alpha \times u'_\alpha)$ *是映射的直接系统，并且（直到规范的双射）我们有*

(35) $$\varinjlim (u_\alpha \times u'_\alpha) = (\varinjlim u_\alpha) \times (\varinjlim u'_\alpha).$$

我们将验证留给读者。

### 习题{#ens-iii-s7-exercises}

参见[习题为 § 7](exercises/s7/)。

[^1]: This means that $u_\alpha \circ f_{\alpha\beta} = g_{\alpha\beta} \circ u_\beta$.
