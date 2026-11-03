---
book: top
book_title: General Topology
chapter: III
chapter_title: Topological Groups
section: 7
section_title: Inverse limits of topological groups and rings
lang: zh
source: top-i-iv
book_pages: 284-295
pdf_pages: 0290-0301, 0330-0332
extraction: ocr
subsections:
    - "no": 1
      title: INVERSE LIMITS OF ALGEBRAIC STRUCTURES
      page: 284
      pdf_page: 290
    - "no": 2
      title: INVERSE LIMITS OF TOPOLOGICAL GROUPS AND SPACES WITH OPERATORS
      page: 286
      pdf_page: 292
    - "no": 3
      title: APPROXIMATION OF TOPOLOGICAL GROUPS
      page: 289
      pdf_page: 295
    - "no": 4
      title: APPLICATION TO INVERSE LIMITS
      page: 293
      pdf_page: 299
statements: 15
exercises: 6
content_sha256: 57247c4e1a85ac8c873353c1ace57ce8611fc6443cee96ed9b74051791a43b31
translated_from: content/en/top/III/07_s7_inverse_limits_of_topological_groups.md
translation_method: google
source_content_sha256: 7ec501cdab64114d3db1a7a9418dc84f5a203ec2564d94a09a0b43191852ce4d
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-1fd6073a
glossary_version: 34
glossary_terms_sha256: f58e6d93c6309a1afd7c0662f7397b1ea53c2e0488676dcd4dfe9bd0cbdad8fe
prompt_sha256: 8cbde7b7ea18274bea5720e1f500823a36194a717a2895a9c9e7e3ffc4a3a3ae
---

## 7. 拓扑群和环的逆极限

在整个截面中，I表示非空有向集合（*），$\alpha \leq \beta$表示I中的部分序关系。 除非则相反，明确指出，所有考虑的逆系均由I索引。

### 1. 代数结构的逆极限

令$(X_\alpha, f_{\alpha \beta})$为集合的逆系，并假设每个$X_\alpha$都被赋予了合成的内部律，在任何地方都以乘法方式定义和书写。还假设 $f_{\alpha \beta}$ 相对于这些内部律是同态。自从

$$
f_{\alpha \beta}(x_\beta \cdot y_\beta) = f_{\alpha \beta}(x_\beta) \cdot f_{\alpha \beta}(y_\beta)
$$

每当$\alpha \leq \beta$和$x_\beta$和$y_\beta$属于到$X_\beta$时，很明显，相对于内部律，$X = \varprojlim X_\alpha$是乘积$\prod_\alpha X_\alpha$的稳定子集

$$
(x_\alpha) \cdot (y_\alpha) = (x_\alpha \cdot y_\alpha).
$$

令$(\Lambda_\alpha, \varphi_{\alpha \beta})$为集合的另一个逆系，由I索引，并假设每个$X_\alpha$携带合成的外法则，在任何地方都被定义、乘法书写并且将$\Lambda_\alpha$作为运算符的集合，这样每当$\alpha \leq \beta$ 我们有

$$
f_{\alpha \beta}(\lambda_\beta \cdot x_\beta) = \varphi_{\alpha \beta}(\lambda_\beta) \cdot f_{\alpha \beta}(x_\beta)
$$

对于 $\lambda_\beta \in \Lambda_\beta$ 和 $x_\beta \in X_\beta$。然后我们可以在$\prod_\alpha X_\alpha$上实现定义外法则，将$\prod_\alpha \Lambda_\alpha$作为集合运算符，通过定义$(\lambda_\alpha) \cdot (x_\alpha) = (\lambda_\alpha \cdot x_\alpha)$；将运算符的集合限制为$\Lambda = \varprojlim \Lambda_\alpha$，我们在$\prod_\alpha X_\alpha$上有外法则，相对于此，$X$又是稳定的子集。因此在 $X$ 上定义的内部（或外部）律被称为 $X_\alpha$ 的内部（或外部）律的逆极限。对于外法则，可能会发生所有$\Lambda_\alpha$与相同的集合$\Lambda_0$相同的情况，并且

(*) 如果 I 只是部分排序，读者可以轻松验证定义的大部分以及截面中命题 1 之前的结果仍然有效。

所有$\varphi_{\alpha \beta}$都是恒等映射；那么，由于$I$是有向集合，所以$\Lambda$可以与$\Lambda_0$识别。

立即验证了结合性，交换律的通常属性，对于内部律存在单位元素（假设$f_{\alpha \beta}$映射单位元素到单位元素），对于内部外法则存在分配律律等，在通向逆极限的过程中被保留。

令$\Sigma$为代数结构的类，并让$\Sigma_0$为*贫困*结构相应的到$\Sigma$。每当我们谈到集合$(X_\alpha, f_{\alpha \beta})$赋予逆系和类$\Sigma$的结构时，我们总是假设$f_{\alpha \beta}$对于这些结构来说是*同态*。如果我们赋予$X = \varprojlim X_\alpha$内部和外法则，分别是内部的逆极限和$X_\alpha$的外法则，那么$X$携带*类*$\Sigma_0$的代数结构。当然，这个结构是否属于类 $\Sigma$，还有待具体情况判断。

例如，如果$(G_\alpha, f_{\alpha \beta})$是群（或环）的逆系，则$\varprojlim G_\alpha$是$\prod_\alpha G_\alpha$的子群（或子环），并且被称为系统的*逆*极限 $(G_\alpha, f_{\alpha \beta})$ 共群（分别为环）。

令$(X_\alpha, g_{\alpha \beta})$为集合的逆系，令$(G_\alpha, f_{\alpha \beta})$为群的逆系；假设每个 $X_\alpha$ 有 $G_\alpha$ 作为群运算符，并且每当 $\alpha \leq \beta$ 我们有

(I)
$$
g_{\alpha \beta}(s_\beta \cdot x_\beta) = f_{\alpha \beta}(s_\beta) \cdot g_{\alpha \beta}(x_\beta)
$$
对于 $x_\beta \in X_\beta$ 和 $s_\beta \in G_\beta$。那么$X = \varprojlim X_\alpha$有$G = \varprojlim G_\alpha$作为群个运算符。从 (I) 可以得出，如果 $\alpha \leq \beta$、映射 $f_{\alpha \beta}$ 和 $g_{\alpha \beta}$ 相容的 (§ 2, no. 4)，因此定义映射 $\varphi_{\alpha \beta} : X_\beta / G_\beta \to X_\alpha / G_\alpha$ 或商集，使得 $(X_\alpha / G_\alpha, \varphi_{\alpha \beta})$ 是逆系。此外，如果$f_\alpha : G \to G_\alpha$和$g_\alpha : X \to X_\alpha$是典范映射，那么$f_\alpha$和$g_\alpha$是兼容的，因此定义映射$h_\alpha : X / G \to X_\alpha / G_\alpha$等于商集；很明显，映射的$h_\alpha$形式逆系，因此其逆极限是映射$h : X / G \to \varprojlim X_\alpha / G_\alpha$，*这不一定是单射或满射*（习题 1）。

再次，令$(A_\alpha, \varphi_{\alpha \beta})$为环的逆系，并令$(M_\alpha, f_{\alpha \beta})$为可交换的群的逆系；并假设每个$M_\alpha$都带有一个左$A_\alpha$模块结构，这样每当$\alpha \leq \beta$我们有

(2)
$$
f_{\alpha \beta}(\lambda_\beta \cdot x_\beta) = \varphi_{\alpha \beta}(\lambda_\beta) \cdot f_{\alpha \beta}(x_\beta)
$$
对于 $x_\beta \in M_\beta$ 和 $\lambda_\beta \in A_\beta$；那么$\varprojlim M_\alpha$的结构比左模多于$\varprojlim A_\alpha$。如果我们假设在加法中，对于每个$\alpha$，$A_\alpha$是可交换的，并且每个$M_\alpha$都有一个$A_\alpha$代数结构，最后$(M_\alpha, f_{\alpha\beta})$是*环*的逆系，那么$\varprojlim M_\alpha$ 的结构的*代数* 超过$\varprojlim A_\alpha$。

令$(G_\alpha, f_{\alpha\beta})$为群的逆系，对于每个$\alpha$，令$H_\alpha$为$G_\alpha$的子群。如果$f_{\alpha\beta}(H_\beta) \subset H_\alpha$每当$\alpha \leq \beta$，则$G_\alpha$的子集$H_\alpha$的逆系相对于$f_{\alpha\beta}$的限制是群的逆系，并且$H = \varprojlim H_\alpha$是*子群* 共 $G = \varprojlim G_\alpha$。如果每个$H_\alpha$是$G_\alpha$的正常子群，则$H$是$G$的正常子群。如果$(G'_\alpha, f'_{\alpha\beta})$是群的另一个逆系，并且对于每个$\alpha$，$u_\alpha : G_\alpha \to G'_\alpha$是同态，使得映射的$u_\alpha$形式逆系，那么，如果$H_\alpha$是$u_\alpha$的核，每当$\alpha \leq \beta$我们就有$f_{\alpha\beta}(H_\beta) \subset H_\alpha$； $u = \varprojlim u_\alpha$是$G$的同态变成$G' = \varprojlim G'_\alpha$，$H = \varprojlim H_\alpha$是$u$的核。如果我们放入$K_\alpha = u_\alpha(G_\alpha)$，那么只要$\alpha \leq \beta$就有$f'_\alpha(K_\alpha) \subset K_\alpha$，这样$G'_\alpha$的子群就有$K_\alpha$形式逆系；但$K = \varprojlim K_\alpha$ *不一定是像于* $G$ *低于* $u$ [习题 1 c)]。

我们通过“替换”“群”“环”“子群”“理想”（左或右）获得类似的结果；我们将陈述模和代数的类似结果的任务留给读者。

### 2. 拓扑群和空间与运算符的逆极限

如果$G_\alpha$是拓扑群并且$f_{\alpha\beta}$是*连续*同态，我们可以说逆系$(G_\alpha, f_{\alpha\beta})$是拓扑群*的*逆系。那么$G = \varprojlim G_\alpha$就是乘积群$\prod_\alpha G_\alpha$的子群；如果我们赋予$G$由$\prod_\alpha G_\alpha$诱导出的拓扑群结构，则这样得到的拓扑群称为拓扑群$(G_\alpha, f_{\alpha\beta})$的逆系的*逆极限*。如果 $G_\alpha$ 是 Hausdorff（分别为 Hausdorff 和完备），那么 $G$ 是 Hausdorff 并且在 $\prod_\alpha G_\alpha$ 中闭合（分别为 Hausdorff 和完备）（章 I, § 8, no. 2、命题 7、推论 2 和章II, § 3, no. 5、推论至命题10)。

如果$(G'_\alpha, f'_{\alpha\beta})$是拓扑群的另一个逆系，并且如果对于每个$\alpha$，$u_\alpha : G_\alpha \to G'_\alpha$是连续的同态，使得$u_\alpha$形式逆系映射，则$u = \varprojlim u_\alpha$是$G$到$G' = \varprojlim G'_\alpha$的连续同态（章I, § 4, no. 4）。将“拓扑群”替换为“拓扑环”，结果相同；我们留给读者的任务是陈述拓扑模 (§ 6, no. 6) 的类似结果。

令$(X_\alpha, g_{\alpha\beta})$为拓扑空间的逆系，令$(G_\alpha, f_{\alpha\beta})$为拓扑群的逆系。假设每个$G_\alpha$在$X_\alpha$（§ 2, no. 4）上连续运行，并且关系（i）对于所有$x_\beta \in X_\beta, s_\beta \in G_\beta$和$\alpha \leq \beta$成立。我们已经看到（no. 1）$X = \varprojlim X_\alpha$有$G = \varprojlim G_\alpha$作为群的运算符；此外，$G$在$X$上持续运行。因为如果$g_\alpha$（或$f_\alpha$）是典范映射$X \to X_\alpha$（或$G \to G_\alpha$），则定义
$$
g_\alpha(s.x) = f_\alpha(s) \cdot g_\alpha(x)
$$
因此映射$(s.x) \to g_\alpha(s.x)$在$X \times G$上连续，这表明$(s, x) \to (s.x)$（章I, § 4, no. 4）的连续性。

因此，由 $f_\alpha$ 和 $g_\alpha$ 引发的映射 $h_\alpha : X/G \to X_\alpha/G_\alpha$ 是连续的 (§ 2, no. 4)，由 $h_\alpha$ 定义的映射 $h : X/G \to \varprojlim X_\alpha/G_\alpha$ 也是连续的 (章 I, § 2, no. 3, 命题) 4）。

#### 命题 1 {#top-iii-s7-prop-1 .statement tag=0BOG}

*假设$X_\alpha$和$G_\alpha$满足上述假设。*

a) *如果$X_\alpha$的每个点的稳定子是每个$\alpha \in I$的$G_\alpha$的紧凑子群，则$X$的每个点$x = (x_\alpha)$的稳定子是一个紧凑子群共$G$； $x$（相对于$G$）的轨道规范地同胚于$x_\alpha$（相对于$G_\alpha$）的轨道的逆极限；并且典范映射 $h : X/G \to \varprojlim X_\alpha/G_\alpha$ 是单射的。*

b) *如果，对于每个$\alpha \in I$，$X_\alpha$（相对于$G_\alpha$）的点的每一个轨道都是紧致的，那么$X$（相对于$G$）的点的每一个轨道都是相对紧致的，并且$h$ 是满射的。如果$h$也是双射，那么$X$的点的每个轨道都是紧的。*

令$x = (x_\alpha) \in X$，对于每个$\alpha \in I$，令$X'_\alpha = G_\alpha \cdot x_\alpha$为$x_\alpha$的轨道。如果$\alpha \leq \beta$，则从(i)和关系$g_{\alpha\beta}(x_\beta) = x_\alpha$得出$g_{\alpha\beta}(X'_\beta) \subset X'_\alpha$，因此$(X'_\alpha)$是$X_\alpha$的子集的逆系。对于每个 $\alpha \in I$ 令 $u_\alpha : G_\alpha \to X'_\alpha$ 为连续的映射 $s_\alpha \to s_\alpha \cdot x_\alpha$； 映射的$u_\alpha$形式逆系，$u = \varprojlim u_\alpha$是$G$的连续映射$s \to s.x$到$X$的子空间$X' = \varprojlim X'_\alpha$。 a) 的假设意味着$\overline{u}_\alpha(y_\alpha)$ 对于每个$y_\alpha \in X'_\alpha$ 都是紧凑的。由于$u_\alpha$也是满射，所以满足章I, § 9, no. 6、命题8、推论2的条件，因此a)的前两个断言成立。因此，如果对于每个$\alpha \in I$，$x = (x_\alpha)$和$y = (y_\alpha)$使得$x_\alpha$和$y_\alpha$属于相对于$G_\alpha$相同的轨道，则$x$和$y$ 属于与轨道相对于 $G$ 而言，因此 $h$ 是单射的。

同样，b)的假设意味着典范映射$v_\alpha : X_\alpha \to X_\alpha/G_\alpha$的逆系满足章I, § 9, no. 6、命题8、推论2的条件，因此它的逆极限 $v = \varprojlim v_\alpha : X \to \varprojlim X_\alpha/G_\alpha$是满射，$\varprojlim X_\alpha / G_\alpha$的每一个点的v下的逆像是紧的。由于 v 因式分解为
$$
X \xrightarrow{\psi} X/G \xrightarrow{h} \varprojlim X_\alpha / G_\alpha,
$$
其中 $\psi$ 是典范映射，b) 的断言紧随其后。

#### 推论 1 {#top-iii-s7-prop-1-cor-1 .statement tag=0BOH}

*如果$G_\alpha$是紧致的且$X_\alpha$豪斯多夫，则a)和b)的结论有效。*

因为满足 a) 和 b) 的假设，因为 $G_\alpha$ 的每个闭子群都是紧致的，并且 $u_\alpha : s_\alpha \to s_\alpha \cdot x_\alpha$ 是紧致空间到 Hausdorff 空间的连续映射。

#### 推论 2 {#top-iii-s7-prop-1-cor-2 .statement tag=0BOI}

*如果，对于每个$\alpha \in I$，群$G_\alpha$在空间$X_\alpha$上传递操作，并且如果$X_\alpha$的每个点的稳定子是$G_\alpha$的紧凑子群，则$G$在$X$和稳定子上进行传递操作，$X$的每个点是$G$的紧凑子群。*

对于假设 a) 满足，并且对于每个$\alpha$ $X'_\alpha = X_\alpha$。

#### 推论 3 {#top-iii-s7-prop-1-cor-3 .statement tag=0BOJ}

*假设$G_\alpha$是Hausdorff。对于每个$\alpha \in I$，令$K_\alpha$是$G_\alpha$的紧凑子群，这样每当$\alpha \leq \beta$时就有$f_{\alpha \beta} (K_\beta) \subset K_\alpha$。那么，如果齐次空间 $G/K$ 到 $\varprojlim G_\alpha / K_\alpha$ 的 $K = \varprojlim K_\alpha$、典范映射 $h$ 是同胚。*

$h$ 是双射的事实源于推论 1，由替换应用，$X_\alpha$ 由 $G_\alpha$ 应用的，以及 $G_\alpha$ 由 $K_\alpha$ 通过*右*翻译操作 (§ 2, no. 5)。令$\varphi$为典范映射$G \to G/K$，对于每个$\alpha$，令$f_\alpha$为典范映射$G \to G_\alpha$。如果对于每个$\alpha$，$V_\alpha$都经过$G_\alpha$的单位元素$e_\alpha$的开邻域的基本系统，则集合$V = \overline{f}_\alpha^{-1}(V_\alpha)$（$\alpha$和$V_\alpha$变量） $G$（章I, § 4, no. 4、命题9）和集合$\varphi(V.K)$中形式邻域的基本系统或单位元素$e$ 形式 $G/K$ $\varphi(e)$ 的邻域的基本系统。我们要证明$h(\varphi(e))$的$h$包含邻域下有$\varphi(V.K)$的像，即$G_\beta$中存在$\beta \geq \alpha$和$e_\beta$的邻域$W_\beta$这样那个$\overline{f}_\beta^{-1}(W_\beta . K_\beta) \subset V.K$。现在，关系$x \in V.K$等价于$K$中存在$y$，使得$f_\alpha(xy^{-1}) \in V_\alpha$，即$f_\alpha(x) \in V_\alpha \cdot f_\alpha(K)$；这样$V.K = \overline{f}_\alpha^{-1}(V_\alpha \cdot f_\alpha(K))$。让$U_\alpha = V_\alpha \cdot f_\alpha(K)$；我们将看到存在$\beta \geq \alpha$，如果我们放入$U_\beta = \overline{f}_{\alpha \beta}^{-1}(U_\alpha)$，我们就有$K_\beta \subset U_\beta$；然后，$G_\beta$中有$e_\beta$的邻域$W_\beta$，使得$W_\beta . K_\beta \subset U_\beta$（章II, § 4, no. 3，推论到命题4），这将建立所需的关系
$$
\overline{f}_\beta^{-1}(W_\beta . K_\beta) \subset \overline{f}_\beta^{-1}(U_\beta) = V.K.
$$

我们继续进行*归谬法*：对于每个$\beta \geq \alpha$，让$M_\beta$表示$K_\beta \cap G U_\beta$；由于$f_{\beta \gamma}^{-1}(U_\beta) = U_\gamma$如果$\alpha \leq \beta \leq \gamma$，$G_\beta$的紧凑子集的$M_\beta$形式逆系（对于$\beta \geq \alpha$）。如果它们都非空，那么它们的逆极限 $M$ 也将非空（章 I, § 9, no. 6，命题 8）。显然$M \subset K$和$f_\alpha(M) \subset M_\alpha$；但这是荒谬的，因为$f_\alpha(K) \subset U_\alpha$，因此证明是完整的。

### 3. 拓扑群的近似

令$G$为群，并令$(H_\alpha)_{\alpha \in I}$为$G$的正常子群族，使得每当$\alpha \leq \beta$时$H_\alpha \supset H_\beta$。对于每个$\alpha \in I$让$G_\alpha = G / H_\alpha$，对于$\alpha \leq \beta$让$f_{\alpha \beta}$是典范同态$G / H_\beta \to G / H_\alpha$，因此映射是$G$中$H_\beta$的陪集$T$到陪集$G$ 中的$H_\alpha$ 的$TH_\alpha$。显然$(G_\alpha, f_{\alpha \beta})$是群中的逆系； $\tilde{G} = \varprojlim G_\alpha$中的元素是族$(T_\alpha)_{\alpha \in I}$，其中$T_\alpha$是每个$\alpha$的$G$中$H_\alpha$的陪集，每当$\alpha \leq \beta$时$T_\alpha \supset T_\beta$。 $G$的映射$i : s \mapsto (s H_\alpha)$到$\tilde{G}$是典范同态$G \to G / H_\alpha$的逆极限，因此是$G$到$\tilde{G}$的同态，并且逆像在元素 $(T_\alpha) \in \tilde{G}$ 的$i$ 等于$\bigcap_{\alpha \in I} T_\alpha$。因此，$i$的核是$\bigcap_{\alpha \in I} H_\alpha$，$i$的像由所有交为*非空*的$(T_\alpha) \in \tilde{G}$族组成。

现在假设$G$是一个*拓扑群*；如果我们给出每个$G_\alpha = G / H_\alpha$ 商拓扑，很明显$(G_\alpha, f_{\alpha \beta})$是拓扑群的逆系，并且$i : G \to \tilde{G}$是连续的同态。

#### 命题 2 {#top-iii-s7-prop-2 .statement tag=0BOK}

*令$G$为拓扑群，并令$(H_\alpha)_{\alpha \in I}$为$G$的正常子群族，使得每当$\alpha \leq \beta$时$H_\alpha \supset H_\beta$，并且其中满足以下条件：*

(AP) *对于每个 $\alpha \in I$，$H_\alpha$ 在 $G$ 中闭合，并且$G$ 包含中的单位元素 $e$ 的每个邻域在$H_\alpha$ 之一中闭合（在其他字中，形成过滤器基由$H_\alpha$收敛到$e$）。*

*那么映射$i : G \to \tilde{G} = \varprojlim G / H_\alpha$是$G$到$i(G)$的严格态射； $\tilde{G}$ 是 Hausdorff，$i(G)$ 是$\tilde{G}$ 的稠密；最后$i$的核是$G$中$\{e\}$的闭包。如果在加法中 $H_\alpha$ 之一是完整的，则 $i$ 是满射的。*

显然，$G_\alpha = G / H_\alpha$ 是 Hausdorff（§ 2, no. 5，命题 13），因此 $\tilde{G}$ 也是豪斯多夫（$\prod_{\alpha \in I} G_\alpha$ 的子空间）。 $i$的核$H$是$H_\alpha$的交，因此是$G$的闭子群。由于 $e$ 包含的每个邻域都有一些 $H_\alpha$，因此它有包含 $H$，因此 [§ 3, no. 1, 公式 (1)] $H$ 是 $\{e\}$ 的闭包。接下来让我们证明$i(G)$在$\tilde{G}$中是稠密的。设$f_\alpha$为典范映射$\tilde{G} \to G_\alpha$，即投影$pr_\alpha$的限制到$\tilde{G}$； $\varphi_\alpha = f_\alpha \circ i$ 是典范映射 $G \to G/H_\alpha$。如果$U$是$\tilde{G}$的任何非空开集合，则$G_\alpha$中存在指标$\alpha \in I$和非空开集合$U_\alpha$，使得$\overline{f}_\alpha^{-1}(U_\alpha) \subset U$（章） I, § 4, no. 4、命题9)；因此
$$
\overline{i}^{-1}(U) \supset \overline{\varphi}_\alpha^{-1}(U_\alpha);
$$
但由于$\varphi_\alpha$是满射，$\overline{i}^{-1}(U)$不为空，因此$i(G) \cap U \neq \emptyset$。

要看到$i$是$G$到$i(G)$的严格态射，请考虑$G$中$e$的邻域$V$。 $G$中有$e$的邻域$W$使得$W^2 \subset V$，以及指标$\alpha \in I$使得$H_\alpha \subset W$；由此可见$V$包含于$WH_\alpha = \overline{\varphi}_\alpha(\varphi_\alpha(W)) = \overline{i}^{-1}(\overline{f}_\alpha^{-1}(\varphi_\alpha(W)))$。由于$\overline{f}_\alpha(\varphi_\alpha(W))$是$\tilde{G}$中单位元素的邻域，因此结果如下。

最后，假设有指标$\gamma \in I$使得$H_\gamma$完整。要证明$i$是满射，只需证明每个家庭$(T_\alpha)_{\alpha \in I} \in \tilde{G}$都有一个非空交即可。由于$T_\gamma$是从$H_\gamma$翻译而来，因此它是$G$的完整子空间（相对于左右均匀性）。此外，由于$G$包含中$e$的每个邻域$U$，$H_\alpha$、相应的集合$T_\alpha$之一都是$U_{d-}$（或$U_{s-}$）小，因此$T_\gamma$中包含的$T_\alpha$的集合是柯西滤波器基；因此它收敛于$T_\gamma$，并且由于$T_\alpha$在$G$中闭合（因为它们是$H_\alpha$的翻译），因此它们的交不为空。

Q.E.D.

#### 推论 1 {#top-iii-s7-prop-2-cor-1 .statement tag=0BOL}

*如果满足条件 (AP) 并且在加法中 (Hausdorff) 群 $G/H_\alpha$ 是完备的，则群 $G$ 具有 Hausdorff 完备性，可以用 $\tilde{G}$ 来识别；然后映射 $i : G \to \tilde{G}$ 被识别为典范映射 ($§ 3$, no. 3, 命题 5)。*

对于$\tilde{G}$则完备（no. 2），命题2表明$i(G)$与与$G$相关的Hausdorff群同构；由于$\tilde{G}$很稠密，所以推论紧随其后（$§ 3$，no. 3，命题5）。特别是：

#### 推论 2 {#top-iii-s7-prop-2-cor-2 .statement tag=0BOM}

*令$G$为群，并令$(H_\alpha)$为$G$的正常子群家庭，针对关系$H_\alpha \supset H_\beta$。如果我们赋予 $G$ 群拓扑 $H_\alpha$ 形式系统邻域单位元素 $e$，则 Hausdorff 群与$G$与$G_1 = G / \left( \bigcap_\alpha H_\alpha \right)$同构的； $G_1$已完成$\hat{G}_1 = \tilde{G}$；以及 $\hat{G} = \hat{G}_1$ 的典范映射 $G_1 \to \tilde{G} = \varprojlim G/H_\alpha$ 扩展至同构到 $\tilde{G}$。*

$G$ 的子群 $H_\alpha$ 是开路，因此也是闭路（$\S$ 2、no. 1、推论到命题 4），$G/H_\alpha$ 是离散的（$\S$ 2、no. 6、命题） 18);因此满足推论 1 中的条件。

对于本小节的其余部分，我们将假设$G$是*Hausdorff*并且$(H_\alpha)$是$G$的*紧凑*正常子群族，它相对于关系$H_\alpha \supset H_\beta$并且满足条件（AP）；凭借命题 2、映射

$$
i : G \to \tilde{G} = \varprojlim G/H_\alpha
$$

那么是拓扑群*的*同构，它允许我们认同$G$和$\tilde{G}$。我们用$f_\alpha$典范映射$G \to G/H_\alpha$表示。

#### 引理 1 {#top-iii-s7-lem-1 .statement tag=0BON}

*在命题 2 的假设下，如果$E$ 是$G$ 的任何闭子集，我们有* $E = \bigcap_\alpha E H_\alpha$。

对于 $E$ 是集合 $EV$ 的交，其中 $V$ 穿过 $e$ 的邻域过滤器 [$\S$ 3, no. 1, 公式 (1)]，并且每个$e$ 包含和 $H_\alpha$ 中的邻域；从 $E \subset EH_\alpha$ 开始，从而结果。

#### 命题 3 {#top-iii-s7-prop-3 .statement tag=0BOO}

*假设 $G$ 是 Hausdorff，且 $H_\alpha$ 是紧致的且满足* (AP)。

a) *令$L$为$G$的闭子群；那么，对于每个$\alpha \in I$，$G_\alpha = G/H_\alpha$的子群$L_\alpha = f_\alpha(L)$是闭集，并且$G$的同构$i$到$\varprojlim G_\alpha$由$L$的限制同构给出$\varprojlim L_\alpha$。如果$L$在$G$中也正常，则$L_\alpha$在$G_\alpha$中也正常，对于每个$\alpha \in I$，以及经过到商，$G/L$的$i$诱导同构到$\varprojlim G_\alpha/L_\alpha$。

b) *相反，对于每个$\alpha \in I$，让$L_\alpha$是$G_\alpha$的闭子群，这样只要$\alpha \leq \beta$就有$L_\alpha = f_{\alpha\beta}(L_\alpha)$。那么$G$有一个唯一的闭子群$L$，使得每个$\alpha \in I$有$L_\alpha = f_\alpha(L)$；如果对于每个$\alpha \in I$，加法$L_\alpha$在$G_\alpha$中是正常的，那么$L$在$G$中是正常的。*

a) 由于 $H_\alpha$ 是紧的，$LH_\alpha$ 在 $G$ 中闭（$\S$ 4, no. 1, 命题 1, 推论 1），因而 $L_\alpha$ 在 $G_\alpha$ 中闭。由于$i$识别拓扑群$G$和$\varprojlim G_\alpha$，并且由于$\varprojlim L_\alpha$可以用$\varprojlim G_\alpha$的（拓扑）子群识别，$i$识别子群$\bigcap_\alpha LH_\alpha$$G$与$\varprojlim L_\alpha$，并证明第一个断言，只需评论$L = \bigcap_\alpha LH_\alpha$乘以引理1就足够了。另一方面，如果$L$是正常的，那么对于由$f_\alpha$引起的每个$\alpha \in I$映射$f'_\alpha : G/L \to G_\alpha/L_\alpha$是满射严格态射 ($\S$ 2, no. 8, 注 3)，其核是紧致子群的 $G/L$、典范像的*紧*正规子群 $H_\alpha L/L$ $H_\alpha$ 共 $G$。由于 $G/L$ 满足条件 (AP) (§ 2, no. 8, 命题 24) 的子群 $H_\alpha L/L$，并且由于 $G/L$ 是 Hausdorff，所以 a) 的最后一个断言是 的推论命题2.

b) 设$f'_{\alpha \beta}$为$f_{\alpha \beta}$到$L_\beta$($\alpha \leq \beta$)中的限制。那么$(L_\alpha, f'_{\alpha \beta})$就是拓扑群的逆系，其逆极限$L$可以与$G$的子群$G \cap \prod_\alpha L_\alpha$等价。通过假设，$f'_{\alpha \beta}$是满射，其核是$L_\beta$的紧子群$f_\beta(H_\alpha) \cap L_\beta$；因而（章 I, § 9, no. 6、推论 1 到命题 8），对于所有 $\alpha \in I$，我们有 $L_\alpha = f_\alpha(L)$。如果$L'$是$G$的另一个闭子群，使得$f_\alpha(L') = L_\alpha$对于所有$\alpha \in I$，则$L'H_\alpha = \overline{f'}_\alpha(L_\alpha)$，从而（引理1）$L' = \bigcap_\alpha L'H_\alpha = \bigcap_\alpha \overline{f'}_\alpha(L_\alpha) = L$。最后，b) 的最后一个断言由公式 $L = \bigcap_\alpha \overline{f'}_\alpha(L_\alpha)$ 得出，因为 $\overline{f'}_\alpha(L_\alpha)$ 现在是 $G$ 的正常子群。

#### 命题 4 {#top-iii-s7-prop-4 .statement tag=0BOP}

*假设$G$是Hausdorff，$H_\alpha$是紧的并且满足(AP)。如果$C_\alpha$是$G_\alpha = G/H_\alpha$的恒等式分量，那么$G$的恒等式分量$C$可以用$\varprojlim C_\alpha$来标识，我们有$f_\alpha(C) = C_\alpha$。*

命题是以下引理中的推论：

#### 引理 2 {#top-iii-s7-lem-2 .statement tag=0BOQ}

*令$G$为豪斯多夫拓扑群，并令$H$为$G$的紧致法线子群，以及$\varphi$典范映射$G \to G/H$。如果$C$是$G$的恒等式分量，那么$\varphi(C)$就是$G' = G/H$的恒等式分量。*

一旦建立了这个引理，我们将为每个$\alpha \in I$拥有$f_\alpha(C) = C_\alpha$，并且由于$C$是$G$的闭子群（§ 2, no. 2，命题7），因此足以满足应用命题3a）。

为了证明引理，首先注意如果$G'$中$C'$是单位元素$e'$的分量，那么$\varphi(C) \subset C'$自$\varphi(C)$是连通的。假设$\varphi(C) \neq C'$。由于$C$是$G$的闭法线子群（§ 2, no. 2，命题7），$\varphi(C)$是$G'$的法线子群；如果 $\psi$ 是典范映射 $G' \to G'/\varphi(C)$，则 $\psi(C')$ 是连通的，并且不只由单位元素组成；因而$G'/\varphi(C)$的恒等式分量并不单独由单位元素组成。但$G'/\varphi(C)$与$(G/H)/(HC/H)$同构的，因此与$G/HC$同构的，因此也与$(G/C)/(HC/C)$同构的（§ 2, no. 7、推论同构于命题22和命题20）。现在，$G/C$是Hausdorff并且完全断开（章I, § 11, no. 5，命题9），并且$HC/C$是$G$的紧致法线子群$H$的典范像，是一个紧致子群共 $G/C$。因而，在额外的假设下证明引理2就足够了，$G$是*完全断开的*，即$C = \{e\}$。

假设$C' \neq \{e'\}$； 替换$G$通过其完全断开的子群$\overline{f'}(C')$和包含$H$，我们可以假设$G'$是*连接的*并且不由单个点组成。

令$\mathfrak{M}$为$G$的闭子群$L$的集合，使得$LH = G$。 我们将证明按关系$\supset$排序的集合$\mathfrak{M}$是*归纳的*。 事实上，如果$\mathfrak{T}$是$\mathfrak{M}$的线性有序子集，那么对于集合$xH \cap L$和$L \in \mathfrak{T}$的每个$x \in G$集合来说，是一个由紧凑空间中封闭的集合形成的过滤器基 $xH$；因此这些集合中的交不为空，这表明子群$L \in \mathfrak{T}$属于到$\mathfrak{M}$中的交。 应用 Zorn 的引理，因此我们看到 $\mathfrak{M}$ 有一个*最小* 元素 $L_0$。 由于 $H$ 是紧的，$G/H = L_0H/H$ 与 $L_0/(L_0 \cap H)$ 同构的 (§ 4, no. 1, 命题 1, 推论 3)；由于 $L_0$ 是完全断开的，而 $L_0 \cap H$ 是紧致的，我们发现我们可以通过 $L_0$ 来实现替换 $G$；在其他字中，我们可以假设在加法中*不*存在闭合的子群$L \neq G$使得$LH = G$。

现在让$F$是单位元素的邻域的交，它们在$G$中都是开闭的，并且让我们证明$F$是$G$的闭子群。显然$F$在$G$是闭合的；因此只要证明$F^{-1}F \subset F$就足够了。但如果$x \in F$且$V$是$G$中$e$的开闭邻域，那么$xV$也是；否则，$e$将属于对$G$中$xV$的补$W$进行补充，这又是开闭的，我们应该有$x \notin W$；因此$x \notin F$，与假设相反。由此可见，集合$xV$的$xF$、交与$V$一样，贯穿$G$、包含$F$中$e$的开闭邻域；另外字、$x^{-1}F \subset F$，这就证明了我们的断言。由于 $G$ 与 $G \neq \{e\}$ 完全断开，因此我们有 $F \neq G$。但如果$V$是$G$中$e$的开闭邻域，那么$VH$也在$G$中开闭（§ 4, no. 1，推论 1到命题1），因此$\varphi(V)$是在 $G/H$ 中既开又闭，这意味着 $\varphi(V) = G/H$ 凭借假设。我们将从这个$FH = G$得到结论，这将给我们所需的矛盾并完成引理的证明。事实上，对于每个$x \in G$，$xH$满足$e$的每个邻域$V$，既开又闭，因此也满足这些邻域中的交$F$，因为集合$Vx \cap H$ 形式过滤器基由……组成封闭式集合位于紧凑型空间 $xH$ 中。

Q.E.D.

#### 注{#top-iii-s7-n3-rem-1 .statement tag=0BOR}

如果子群 $H_\alpha$ 对于 *某些* $\alpha \in I$ 是紧致的，那么 $H_\beta$ 对于所有 $\beta \geq \alpha$ 也是紧致的，因为它是 $H_\alpha$ 的闭子群。由于所有$\beta \in I$中的集合使得$\beta \geq \alpha$在$I$中是共尾的，因此在群$G$的研究中，我们是否假设$H_\alpha$之一是紧致的或者*所有*$H_\alpha$都是紧致的，本质上没有区别。

### 4. 申请逆极限

#### 命题 5 {#top-iii-s7-prop-5 .statement tag=0BOS}

*设* $(G_\alpha, f_{\alpha\beta})$ *为豪斯多夫拓扑群的逆系，使得* $f_{\alpha\beta}$ *是满射严格态射和紧凑核。*然后对于$G = \varprojlim G_\alpha$的每个$\alpha \in I$典范映射$f_\alpha$ into $G_\alpha$ 是一个严格满射态射，其核是紧的。

$f_\alpha$是满射且核是紧的，事实是章I, § 9, no. 6、推论1到命题8的推论。还有待证明$f_\alpha$是严格的态射。让$e$（或$e_\alpha$）表示单位元素 / $G$（或$G_\alpha$）。 形式 $f_\beta^{-1}(V_\beta)$ 中$G$ 包含集合中$e$ 的每个邻域 $V$，其中$V_\beta$ 为$e_\beta$ 中的邻域 $G_\beta$，我们可以假设$\beta \geq \alpha$；由于$f_{\alpha \beta}$是满射严格态射，$f_{\alpha \beta}(V_\beta)$是$G_\alpha$中$e_\alpha$的邻域，并且由于$f_\beta$是满射，我们有$V_\beta \subset f_\beta(V)$，从而

$$
f_\alpha(V) = f_{\alpha \beta}(f_\beta(V)) \supset f_{\alpha \beta}(V_\beta);
$$

这表明$f_\alpha(V)$是$G_\alpha$中$e_\alpha$的邻域。

如果$H_\alpha = f_\alpha^{-1}(e_\alpha)$，那么每个$H_\alpha$都是$G$的紧凑法线子群； $H_\alpha$ 明显满足条件 (AP) no. 3； $G_\alpha$可以与$G/H_\alpha$识别。特别是no. 3的命题3和4适用于$G$和$H_\alpha$。

#### 推论 1 {#top-iii-s7-prop-5-cor-1 .statement tag=0BOT}

*设* $(G_\alpha, f_{\alpha \beta})$ *为拓扑群的逆系，满足命题 5的假设；让* $(G'_\alpha, f'_{\alpha \beta})$ *成为拓扑群的逆系，并且对于每个* $\alpha$ *让* $u_\alpha : G_\alpha \to G'_\alpha$ *成为具有紧凑核的满射严格态射，使得* $u_\alpha$ *从逆系映射。那么*$u = \varprojlim u_\alpha$*是*$G = \varprojlim G_\alpha$*到*$G' = \varprojlim G'_\alpha$的严格态射，*并且它的核是紧凑的*。

设$N_\alpha$为$u_\alpha$的核。那么 $L_\alpha = f_\alpha^{-1}(N_\alpha)$ 就是满射严格态射 $v_\alpha = u_\alpha \circ f_\alpha : G \to G'_\alpha$ 的核；由于 $L_\alpha / H_\alpha$ 与 $N_\alpha$ (§ 2, no. 7, 命题 20) 同构的，$L_\alpha$ 是 $G$ (§ 4, no. 1, 推论 2 到命题 2) 的*紧凑*正规子群。 $u$的核$L$是$L_\alpha$的交。让$\varphi$表示典范映射$G \to G/L$；那么我们可以将$v_\alpha = w_\alpha \circ \varphi$（其中$w_\alpha$是$G/L$的严格态射）写到$G'_\alpha$上，核是$L_\alpha / L$。由于$L_\alpha / L$的交是$G/L$的单位元素，并且由于$L_\alpha / L$形式是滤波器基并且是紧致的，因此该滤波器基收敛到$G/L$的单位元素 （章I, § 9, no. 1、推论至定理1）。 命题 2 of no. 3 则表明 $w = \varprojlim w_\alpha$ 是 $G/L$ 到 $G'$ 的 *同构的*；由此可见，$w \circ \varphi$ 是 $G$ 到 $G'$ 的严格态射，其中核 $L$。但显然$u = w \circ \varphi$，因此推论得证。

#### 推论 2 {#top-iii-s7-prop-5-cor-2 .statement tag=0BOU}

*设* $(G_\alpha, f_{\alpha \beta})$ *为拓扑群的逆系，满足命题 5的条件，并令* $G'$ *为拓扑群，其中有邻域* $V'$ * 单位元素* $e'$ *其中包含除 $\{ e' \}$ 之外，$G'$ 中没有子群*。那么如果$v : G \to G'$是任何连续的同态，则存在指标$\alpha \in I$和连续的同态$v_\alpha : G_\alpha \to G'$使得$v = v_\alpha \circ f_\alpha$。

因为由于$G$中$\overline{v}^{-1}(V')$是$e$的邻域，所以$G_\alpha$中存在$e_\alpha$的指标$\alpha$和邻域$V_\alpha$，使得$f_\alpha^{-1}(V_\alpha) \subset \overline{v}^{-1}(V')$。因此$v(H_\alpha) \subset V'$，并且由于$v(H_\alpha)$是$G'$的子群，因此得出$v(H_\alpha) = \{ e' \}$。由于 $f_\alpha$ 可以与典范映射 $G \to G/H_\alpha$ 等同，因此推论是连续同态 (§ 2, no. 8) 的规范因式分解的推论。

### 习题{#top-iii-s7-exercises}

请参阅[习题为 § 7](exercises/s7/)。
