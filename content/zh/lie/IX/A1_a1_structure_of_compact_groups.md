---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: IX
chapter_title: COMPACT REAL LIE GROUPS
section: 1
section_title: Structure of compact groups
appendix: true
lang: zh
source: lie-vii-ix
book_pages: 381-385, 424-425
pdf_pages: 0388-0392, 0431-0432
extraction: native
subsections:
    - "no": 1
      title: EMBEDDING A COMPACT GROUP IN A PRODUCT OF LIE GROUPS
      page: 381
      pdf_page: 388
    - "no": 2
      title: PROJECTIVE LIMITS OF LIE GROUPS
      page: 382
      pdf_page: 389
    - "no": 3
      title: STRUCTURE OF CONNECTED COMPACT GROUPS
      page: 384
      pdf_page: 391
statements: 9
exercises: 1
content_sha256: 24bcf010dc42d27952a4e10b178599f3610022c9c2c63f38668f0662a53e9f69
translated_from: content/en/lie/IX/A1_a1_structure_of_compact_groups.md
translation_method: google
source_content_sha256: 5e7319fca99d12df0397567af8fdb7c23d7ffbc97775400d0463c84a608eb608
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-1fd6073a
glossary_version: 34
glossary_terms_sha256: 7619c82547c119195166c97147dbaee0730b13650566ab59ef428e41d74df8ca
prompt_sha256: 8cbde7b7ea18274bea5720e1f500823a36194a717a2895a9c9e7e3ffc4a3a3ae
---

## 附录I

# 紧群的结构

### 1. 将紧凑的群嵌入到李群的乘积中

#### 命题 1 {#lie-ix-a1-prop-1 .statement tag=01II}

每个紧拓扑群 G 都同构于乘积的紧李群的闭子群。

用有限维复数 Hilbert 空间上 G 的不可约连续酉表示 $\widehat{G}$ 集合类表示（谱理论，准备中）。对于所有$u\in \widehat{G}$，令$Hu$为与$u$伴随的$u$和$\rho_u: G\rightarrow \mathbf{U}(H_u)$同态的空间。根据Peter-Weyl 定理（谱理论，准备中），从G到$\prod_{u\in\widehat{G}}\mathbf{U}(H_u)$的连续同态$\rho = (\rho_u)_{u\in\widehat{G}}$是单射的；由于 G 是紧致的，$\rho$ 诱导同构

从 G 到群 $\prod_{u\in\widehat{G}}\mathbf{U}(H_u)$ 的闭子群。

#### 推论 1 {#lie-ix-a1-prop-1-cor-1 .statement tag=01IJ}

令 V 为 G 的单位元素的邻域。则 V 包含 G 的闭法线子群 H，使得商 $G/H$ 为李群。

令$(K_{\lambda})_{\lambda\in L}$为紧李群的族，使得G可以用$\prod_{\lambda\in L}K_{\lambda}$的闭子群来识别；对于$\lambda \in L$，将$p_{\lambda}: G\rightarrow K_{\lambda}$限制降级为规范投影的G。存在有限子集$J\subset L$，并且对于$K_{\lambda}$中原点的每个$\lambda \in J$邻域$V_{\lambda}$，使得V包含$\bigcap_{\lambda\in J}p^{-1}_{\lambda}(V_{\lambda})$。现在放入 $H =\bigcap_{\lambda\in J}$ Ker($p_{\lambda}$) 就足够了。

用G的闭正常子群的$(H_{\alpha})_{\alpha\in I}$递减过滤族表示，使得商$G/H_{\alpha}$是李群。考虑紧李群$G/H_{\alpha}$的投影系统（cf.一般拓扑，第III, §7, no. 2章，命题2）。

#### 推论 2 {#lie-ix-a1-prop-1-cor-2 .statement tag=01IK}

规范的映射$G\rightarrow$lim$_{_{\leftarrow -}}G/H_{\alpha}$是拓扑群的同构。 $\alpha$

确实，科. 1 意味着拓扑，第 1 章的条件 (PA)。 III, §7, no. 2，满意； 断言现在遵循 loc 的 Prop. 2。引用。

#### 推论 3 {#lie-ix-a1-prop-1-cor-3 .statement tag=01IL}

G 是李群当且仅当存在 G 的单位元素 $e$ 的邻域且包含不存在不同于 $\{e\}$ 的正常子群。

这个条件的必要性已经被证明了（第2章III, §4, no. 2，Cor.1），充分性是Cor.1的直接的推论。 1.

### 2. 射影极限 / 李群

#### 引理 1 {#lie-ix-a1-lem-1 .statement tag=01IM}

令$(G_{\alpha}, f_{\alpha \beta})$为拓扑群相对于过滤后的指标集合I的射影系统，G为极限。假设规范映射 $f_{\alpha}: G\rightarrow G_{\alpha}$ 是满射的。

a) 子群 $D(G_{\alpha})$（分别$C(G_{\alpha})$，分别$C(G_{\alpha})_0$）形式子集 $G_{\alpha}$ 的投影系统。

b) 我们有 D(G) = lim$_{_{\leftarrow -}\alpha}\overline{D(G_{\alpha})}$ 和 C(G) = lim$_{_{\leftarrow -}\alpha}C(G_{\alpha})$。

c) 如果$G_{\alpha}$ 对于所有$\alpha \in I$ 都是紧致的，则$C(G)_0=$ lim$_{_{\leftarrow -}\alpha}C(G_{\alpha})_0$。

令$\alpha , \beta$为I的两个元素，其中$\alpha \leq \beta$。然后 $f_{\alpha \beta}(D(G_{\beta}))\subset D(G_{\alpha})$ 和 $f_{\alpha \beta}(C(G_{\beta}))\subset C(G_{\alpha})$，因为 $f_{\alpha \beta}$ 是满射；由于 $f_{\alpha \beta}$ 是连续的，因此有 $f_{\alpha \beta}(\overline{D(G_{\beta})})\subset \overline{D(G_{\alpha})}$ 和 $f_{\alpha \beta}(C(G_{\beta})_0)\subset C(G_{\alpha})_0$，因此 a)。由于 $f_{\alpha}$ 是满射，$f_{\alpha}(D(G)) = D(G_{\alpha})$（代数，第 I, §6, no. 2 章，第 6 条命题），因此 $\overline{D(G)}=$ lim$_{\leftarrow -}\overline{D(G_{\alpha})}$（一般拓扑，第 I, §4, no. 4 章，第 9 条命题的修正）。 $f_{\alpha}$ 的满射性也意味着包含 $f_{\alpha}(C(G))\subset$ $C(G_{\alpha})$，因此包含$C(G)\subset$ lim$_{\leftarrow -}C(G_{\alpha})$；相反的内含物是直接的。最后，断言 c) 源自 b) 和一般拓扑，第 1 章。 III, §7, no. 2，提案 4）。

#### 引理 2 {#lie-ix-a1-lem-2 .statement tag=01IN}

令 $(S_a)_{a\in A},(T_b)_{b\in B}$ 为几乎简单、单连通的李群的两个有限族（第 III, § 9, no. 8，定义 3）$,u:\prod_{a\in A}S_a\rightarrow \prod_{b\in B}T_b$ 一个满射态射。那么存在一个单射映射$l: B\rightarrow A$和同构$u_b: S_{l(b)}\rightarrow T_b(b\in B)$，使得$u((s_a)_{a\in A}) = (u_b(s_{l(b)}))_{b\in B}$对于$\prod_{a\in A}S_a$的每个元素$(s_a)_{a\in A}$。

用$S_a$（分别$T_b$）的$\mathfrak{s}_a$（分别$\mathfrak{t}_b$）李代数表示$a\in A$（分别$b\in B$），并考虑同态$L(u) :\prod_{a\in A}\mathfrak{s}_a\rightarrow \prod_{b\in B}\mathfrak{t}_b$。 核

是半单李代数$\prod_{a\in A}\mathfrak{s}_a$的理想，因此是形式$\prod_{a\in A''}\mathfrak{s}_a$，以及$A''\subset A$（第I, §6, no. 2章，Cor.1）。把$A'= A$**--** $A''$。由

限制、$L(u)$诱导同构$f:\prod_{a\in A'}\mathfrak{s}_a\rightarrow \prod_{b\in B}\mathfrak{t}_b$。按地点。前述，对于所有$a\in A'$，理想的$f(\mathfrak{s}_a)$等于$\mathfrak{t}_b$之一；因此，存在双射$l: B\rightarrow A'$使得$f(\mathfrak{s}_{l(b)}) =\mathfrak{t}_b$对应$b\in B$，以及$f$诱导同构$f_b:\mathfrak{s}_{l(b)}\rightarrow \mathfrak{t}_b$。由于群 $S_a$ 和 $T_b$ 是单连通的，因此存在同构 $u_b: S_{l(b)}\rightarrow T_b$，使得 $L(u_b) =f_b$ 对应 $b\in B$（第 III, §6, no. 3 第 3 章）。

由 $\widetilde{u}:\prod_{a\in A}S_a\rightarrow \prod_{b\in B}T_b$ 表示态射由 $\widetilde{u}((s_a)_{a\in A}) =$ 定义

$(u_b(s_{l(b)}))_{b\in B}$。由构造，$L(\widetilde{u}) =f= L(u)$，所以$\widetilde{u}=u$，从而证明引理。

#### 引理 3 {#lie-ix-a1-lem-3 .statement tag=01IO}

在引理 1 的假设下，假设$G_{\alpha}$ 是单连通的紧李群。那么，拓扑群 G 同构于几乎简单、单连通紧李群族的乘积。

对于所有 $\alpha \in I$，群 $G_{\alpha}$ 是几乎简单、简单连接的有限族子群 $(S^{\lambda}_{\alpha})_{\lambda\in L_{\alpha}}$ 的直接乘积（第 III, §9, no. 8 章，第 28 条命题）。让$\beta \in I,\beta \geq \alpha$。到引理 2，存在映射 $l_{\beta \alpha}: L_{\alpha}\rightarrow L_{\beta}$，使得$f_{\alpha \beta}(S^{l_{\beta \alpha}(\lambda)}_{\beta}) = S^{\lambda}_{\alpha}$对应$\lambda \in L_{\alpha}$。我们有 $l_{\gamma \beta}\circ l_{\beta \alpha}=l_{\gamma \alpha}$ 对应 $\alpha \leq \beta \leq \gamma$，因此 $(L_{\alpha}, l_{\beta \alpha})$ 是集合相对于 I 的归纳系统。设L为其极限； 映射 $l_{\beta \alpha}$是单射的，$L_{\alpha}$可以与L的子集等同，因此$L =\bigcup_{\alpha\in I}L_{\alpha}$。

让$\lambda \in L$。当$\lambda  \notin L_{\alpha}$时置$S^{\lambda}_{\alpha}=\{1\}$，并表示由$f_{\alpha \beta}$诱发$\varphi^{\lambda}_{\alpha \beta}: S^{\lambda}_{\beta}\rightarrow S^{\lambda}_{\alpha}$态射；这给出了拓扑群$(S^{\lambda}_{\alpha}, \varphi^{\lambda}_{\alpha \beta})$的射影系统，其极限与$S_{\lambda}$同构的。拓扑典范同态群

林$_{_{\leftarrow -\alpha\in I}}((\prod_{\lambda\in L}S^{\lambda}_{\alpha})\rightarrow \prod_{\lambda\in L}($林$_{_{\alpha\leftarrow -\in I}}S^{\lambda}_{\alpha})$

是双射的（集合论，第III, §7, no. 3章，Cor.2）；因此它是同构，因为所讨论的群是紧凑的。但第一个群可以用G来识别，第二个可以用$S_{\lambda}$的乘积来识别，因此是引理。

### 3. 连接紧凑型结构群

令 G 为交换紧群。回想一下（谱理论，第II, §1, no. 9，命题11），G 同构于离散交换群 $\widehat{G}$ 的对偶拓扑群。 群 G 连通当且仅当 $\widehat{G}$ 无扭转（谱理论，第 II, §2, no. 2 章，第 4 条命题第 1 条）。

以下属性是等效的（光谱理论，第 II, §2, no. 2 章，第 4 号提案的 Cor.2 和 §1, no. 9，第 11 号提案的 Cor.2）：

(i) G 是完全不连续的；

(ii) $\widehat{G}$ 是挠元群；

(iii) 拓扑群 G 同构于有限（可交换）群的射影系统的极限，每个都有离散的拓扑。

下面的命题概括了Cor。 §1, no. 4 的第 4 号提案 1。

#### 命题 2 {#lie-ix-a1-prop-2 .statement tag=01IP}

令 G 为连通紧凑群。

a$) C(G)_0$ 是可交换连通紧群； D(G) 是连通紧凑群，等于其导出群。

b) 从$C(G)_0\times D(G)$到G的连续同态$(x, y) \rightarrow xy$是满射的，它的核是$C(G)_0\times D(G)$的中心子群，是紧致且完全不连续的。

c) 存在一个几乎简单的紧李群族$(S_{\lambda})_{\lambda\in L}$和一个满射连续同态$\prod_{\lambda\in L}S_{\lambda}\rightarrow D(G)$，其核是

完全不连续、紧凑、居中子群。

令$(G_{\alpha}, f_{\alpha \beta})$为紧李群的投影系统，相对于过滤后的集合I，使得G与lim$_{\leftarrow -}G_{\alpha}$同构的，并且规范的映射$f_{\alpha}: G\rightarrow G_{\alpha}$是满射的（第1条的Cor.2）。对于$\alpha \in I$，令$\pi_{\alpha}: \widetilde{D}(G_{\alpha})\rightarrow D(G_{\alpha})$是群$D(G_{\alpha})$的通用覆盖。 $f_{\alpha \beta}$诱导态射$\widetilde{f}_{\alpha \beta}: \widetilde{D}(G_{\beta})\rightarrow \widetilde{D}(G_{\alpha})$和$( \widetilde{D}(G_{\alpha}),\widetilde{f}_{\alpha \beta})$是拓扑群满足引理3的假设的射影系统。

由此引理可知，拓扑群 lim$_{\leftarrow -}\widetilde{D}(G_{\alpha})$同构于几乎简单的紧李群族$(S_{\lambda})_{\lambda\in L}$的乘积。 由引理1，同态射影系统$(\pi_{\alpha})$的极限可以用连续同态$\pi :\prod_{\lambda\in L}S_{\lambda}\rightarrow D(G)$来识别，

这是满射的（通则拓扑，第 I, §9, no. 6 章，第 8 号命题的 Cor. 2）。

现在观察群 $\prod_{\lambda\in L}S_{\lambda}$ 等于其导出群：

源自 §4, no. 5，Cor。命题 10 的结论。对于 D(G) 也是如此，因为 $\pi$ 是满射。因而，$D(G)\supset D(D(G)) = D(G)$。因而，群 D(G) 是紧的并且等于它的导出群；这证明了a)，因为断言关于$C(G)_0$是微不足道的。

另一方面，可以识别$\pi :\prod_{\lambda\in L}S_{\lambda}\rightarrow D(G)$的核

与 lim$_{\leftarrow -}$ Ker($\pi_{\alpha}$) $($代数，第 1 章II, §6, no. 1, 注 1)，因此有

紧凑，完全不连续，中心子群，因而 c)。

我们证明b）。对于I中的所有$\alpha$，态射$s_{\alpha}: C(G_{\alpha})_0\times D(G_{\alpha})\rightarrow G_{\alpha}$，使得$x\in C(G_{\alpha})_0, y\in D(G_{\alpha})$的$s_{\alpha}(x, y) =xy$是满射，并且其核是有限中心子群（§1, no. 4，第4条的Cor.1）。 $s_{\alpha}$ 形式映射的射影系统，其极限可以通过前面的内容与从 $C(G)_0\times D(G)$ 到 G 的同态 $(x, y) \rightarrow xy$ 等同。我们现在将其视为之前，这个映射是满射且其核位于中心且完全不连续，因而 b)。

#### 推论 {#lie-ix-a1-n3-cor-1 .statement tag=01IQ}

每个可解的连通紧致群都是可交换的。

事实上，导出群是可解的并且等于它的导出群（命题$2a$）$)$，因此减少到单位元素。

### 习题{#lie-ix-a1-exercises}

参见[习题附录 1](exercises/a1/)。
