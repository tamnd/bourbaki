---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: VII
chapter_title: CARTAN SUBALGEBRAS AND REGULAR ELEMENTS
section: 1
section_title: Polynomial maps and Zariski topology
appendix: true
lang: zh
source: lie-vii-ix
book_pages: 45-47, 66
pdf_pages: 0055-0057, 0075-0075
extraction: native
subsections:
    - "no": 1
      title: ZARISKI TOPOLOGY
      page: 45
      pdf_page: 55
    - "no": 2
      title: DOMINANT POLYNOMIAL MAPS
      page: 46
      pdf_page: 56
statements: 7
exercises: 4
content_sha256: 9715d04b4f510f6cd72e84f33eb032a824a415b19fb143a0f43cfd8543beceb8
translated_from: content/en/lie/VII/A1_a1_polynomial_maps_and_zariski_topology.md
translation_method: google
source_content_sha256: 35b05a39838f20b88ddf3fc98b3fdd147867c98e1efaf99bb5c98caf247537a5
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-50f48bb3
glossary_version: 34
glossary_terms_sha256: 8e00d862c9dc9914765ea32bb0a09a4b797910c2c6e2d69908a272ea9d4b1773
prompt_sha256: 77d1eb2d7fcbd90aea4f1a996022f1b3908ace921dc0bfaa5df62ffc2d1f67a6
---

## 附录 I 多项式映射和 ZARISKI 拓扑

在这个附录中，$k$被假设为无穷大。

### 1. 扎里斯基拓扑

令 V 为有限维向量空间。 We denote by $A_V$ the algebra of polynomial functions on V with values in $k($Algebra, Chap. IV, §5, no. 10, Def. 4). 这是分级代数； 次数 1 的分量是 V 的对偶 $V^*$ 和 $V^*$ 的单射到 $A_V$ 扩展到同构，从对称代数 $\mathbf{S}(V^*)$ 到$A_V($代数，第 1 章IV, §5, no. 11、注 2)。

如果 $(e_1, . . . , e_n)$ 是 V 的基，并且 $(X_1, . . . ,X_n)$ 序列是不定式，则映射从 $k[X_1, . . . ,X_n]$ 到 $A_V$ 取 $k[X_1, . . . ,X_n]$ 到函数的任何元素 $f$

$$
\sum_{i=1}^n\lambda_ie_i \rightarrow f(\lambda_1, . . . , \lambda_n)
$$

是代数的同构（代数，第IV, §5, no. 10章，第19号提案的Cor.）。

#### 命题 1 {#lie-vii-a1-prop-1 .statement tag=00XC}

令H为从$A_V$到$k$的代数同态的集合。对于任何$x\in V$，令$h_x$为从$A_V$到$k$的同态$f \rightarrow f(x)$。那么，从V到H，映射$x \rightarrow h_x$就是双射。

事实上，让$H'$是从$k[X_1, . . . ,X_n]$到$k$的代数同态的集合。从$H'$到$k^n$，映射$\chi  \rightarrow (\chi (X_1), . . . , \chi (X_n))$显然是双射。

#### 推论{#lie-vii-a1-n1-cor-1 .statement tag=00XD}

对于任何$x\in V$，设$\mathfrak{m}_x=$ Ker($h_x$)。那么映射$x \rightarrow \mathfrak{m}_x$是$A_V$的理想$\mathfrak{m}$从V到集合的双射，使得$A_V/\mathfrak{m}=k$。

如果存在$A_V$的元素的$(f_i)_{i\in I}$族，使得$x\in F\Leftarrow \Rightarrow x\in V$和$f_i(x) = 0$对于所有$i\in I$来说，V的子集F被认为是封闭的。

显然$\emptyset$和V是闭的，并且闭的集合中的任意交都是闭的。如果 F 由 $f_i$ 的消失定义，$F'$ 由 $f'_j$ 的消失定义，则 $F\cup F'$ 由 $f_if'_j$ 的消失定义，因此是闭集。因此，V上存在拓扑，使得该拓扑的闭集合恰好是上述意义上的闭集合。这个拓扑称为V上的Zariski拓扑。对于任何$f\in A_V$，我们用$x\in V$的$V_f$集合表示，使得$f(x)\not= 0$；这是 V 的开子集。很明显，Zariski 拓扑的$V_f$形式基。 （如果$k$是拓扑域，则V的规范拓扑比Zariski拓扑是更细。）

Cor 的映射 $x \rightarrow \mathfrak{m}_x$。命题1可以被认为是从V到$A_V($交换代数的素谱Spec(A$_V$)的映射$\varepsilon$，第1章。 II, §4, no. 3，防御。 4). Spec(A$_V$)的拓扑的$\varepsilon$下的Zariski拓扑为逆像为直接的。

#### 命题 2 {#lie-vii-a1-prop-2 .statement tag=00XE}

向量空间V，配备Zariski拓扑，是不可约的诺特空间。特别是，V的每个非空开子集都是稠密的。

由于$A_V$是诺特，Spec(A$_V$)是诺特（交换代数，第II, §4, no. 3章，第11号提案第7章），诺特空间的每个子空间是诺特 （前述，no. 2，第 8 号提案）。与Cor的记号。命题1中，$\mathfrak{m}_x$的交是$\{0\}$，$\{0\}$是$A_V$的素理想；因此 V 是不可约的（前述，no. 3，第 14 条命题）。

### 2. DOMINANT POLYNOMIAL MAPS

令 $V,W$ 为有限维向量空间。令 $f$ 为从 V 到 W 的多项式映射（代数，第 IV, §5, no. 10 章，定义 4）。如果 $\psi \in A_W,\psi \circ f\in A_V$（参见第 17 条提案）。 映射$\psi  \rightarrow \psi \circ f$是从$A_W$到$A_V$的同态，据说与$f$相关。它的核由函数$\psi \in A_W$组成，在$f(V)$上消失（因此也在Zariski拓扑中的$f(V)$闭合时消失）。

#### 定义 1 {#lie-vii-a1-def-1 .statement tag=00XF}

如果与 $f$ 关联的从 $A_W$ 到 $A_V$ 的同态是单射的，则称多项式映射 $f: V\rightarrow W$ 是显性的。

鉴于前述，当且仅当 $f(V)$ 在 Zariski 拓扑中的 W 中稠密时，$f$ 占主导地位。

#### 命题 3 {#lie-vii-a1-prop-3 .statement tag=00XG}

假设 $k$ 是代数闭的。 设$f: V\rightarrow W$为支配多项式映射。 V 包含的任何密集开子集 $f$ 下的像 W 的密集开子集。

足以证明，对于$A_V,f(V_{\varphi})$包含的每个非零元素$\varphi$，W.认同$A_W$的密集开子集和$A_V$的子代数通过同态关联到$f$。存在 $A_W$ 的非零元素 $\psi$，使得每个同态 $w: A_W\rightarrow k$ 不会湮灭 $\psi$ 扩展到同态 $v: A_V\rightarrow k$ 不会湮灭$\varphi ($交换代数，第 1 章V, §3, no. 1，科。 3 Th。 1）。现在，这样的$w$（或$v$）可以与$W_{\psi}$（或$V_{\varphi}$）的元素识别，并且说$v$、扩展、$w$意味着$f(v) =w$。因此，$W_{\psi}\subset f(V_{\varphi})$。 Q.E.D.

令$f: V\rightarrow W$为多项式映射，且$x_0\in V$。从V到W的映射$h \rightarrow f(x_0+h)$是多项式。将其分解为齐次多项式映射的有限和：

$$
f(x_0+h) =f(x_0) + D_1(h) + D_2(h) +\cdots
$$

其中 $D_i: V\rightarrow W$ 是次数 $i($代数的齐次，第 1 章。 IV, §5, no. 10，提案 19）。直线映射$D_1$称为$f$在$x_0$的切线映射。我们用$Df(x_0)$表示。

#### 命题 4 {#lie-vii-a1-prop-4 .statement tag=00XH}

设 $f: V\rightarrow W$ 为多项式映射。假设存在$x_0\in V$使得$(Df)(x_0)$是满射的。那么$f$占主导地位。

应用 V 的翻译和 W 的翻译，我们可以假设 $x_0= 0$ 和 $f(x_0) = 0$。 $f$的分解可以写成齐次元素的和

$f=f_1+f_2+\cdots$ 度数$f_i=i$，

线性映射 $f_1$ 与假设满射。假设 $f$ 不占优势。那么存在 $A_W$ 的非零元素 $\psi$ 使得 $\psi \circ f= 0$。设 $\psi =\psi_m+\psi_{m+1}+\cdots$ 为 $\psi$ 的分解并入齐次元素，度为 $\psi_i=i$ 和 $\psi_m\not= 0$。然后

$$
0 =\psi \circ f=\psi_m\circ f+\psi_{m+1}\circ f+\cdots
$$

$$
=\psi_m\circ f_1+\rho
$$

其中 $\rho$ 是次数 $> m$ 的齐次多项式映射的和。由此可见$\psi_m\circ f_1= 0$。由于 $f_1$ 是满射，$\psi_m= 0$ 是矛盾的。

#### 推论{#lie-vii-a1-n2-cor-1 .statement tag=00XI}

如果$k$是代数闭的，并且如果$f$满足命题4的假设，则像位于V包含的任何稠密开子集的$f$下，W的稠密开子集。

这是从 Props 得出的。 3和4。

### 习题 {#lie-vii-a1-exercises}

用 V 表示 $k$ 上的有限维向量空间。

参见[习题附录 1](exercises/a1/)。
