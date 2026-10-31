---
book: ac
book_title: Commutative Algebra
chapter: V
chapter_title: INTEGERS
section: 3
section_title: Finitely generated algebras over a field
lang: zh
source: ac-i-vii
book_pages: 344-354, 370-373
pdf_pages: 0363-0373, 0389-0392
extraction: ocr
subsections:
    - "no": 1
      title: THE NORMALIZATION LEMMA
      page: 344
      pdf_page: 363
    - "no": 2
      title: THE INTEGRAL CLOSURE OF A FINITELY GENERATED ALGEBRA OVER A FIELD
      page: 348
      pdf_page: 367
    - "no": 3
      title: THE NULLSTELLENSATZ
      page: 349
      pdf_page: 368
    - "no": 4
      title: JACOBSON RINGS
      page: 351
      pdf_page: 370
statements: 17
exercises: 10
content_sha256: 550dfd6d6abd5359be7a9bb6a776473940451567d61f78834502fd5cb1d4d45b
translated_from: content/en/ac/V/03_s3_finitely_generated_algebras_over_a_field.md
translation_method: google
source_content_sha256: 6de44311d5d60b730fb626da1cd69b9f44af23562467fb568b226b7a0a3a5d4c
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-39653cda
glossary_version: 34
glossary_terms_sha256: de5354f7aa953bc803860fe8f26d7d24fa88408017ef8d612f11e82cffdc586b
prompt_sha256: 7fdd4e0b5e6067ff04498ebe670ef3580d6ba9506bf4d0c582d73af15fd73ef3
---

## 3. 有限生成代数超过域

### 1. 标准化引理

在这个没有。以下，k 表示交换域。

#### 定理 1（标准化引理）{#ac-v-s3-thm-1 .statement tag=04R8}

令 A 为有限生成的 K-代数，并令 $a_1 \subset a_2 \subset \ldots \subset a_p$ 为 A 理想的递增有限序列，使得 $p \geq 1$ 和 $a_p \neq A$。 A 的元素存在有限序列 $(x_i)_{1 \leq i \leq n}$，它们在代数上独立于 k (章 III, § 1, no. 1)，并且使得：
(a) A 是环 $B = k[x_1, \ldots, x_n]$ 上的积分。
(b) 对于所有j，使得$1 \leq j \leq p$，存在整数的递增序列$(h(j))_{j \leq j \leq p}$，使得对于所有j，生成B的理想$a_j \cap B$$x_1, \ldots, x_{h(j)}$。

注首先当A是多项式代数$k[Y_1, \ldots, Y_m]$时足以证明定理。因为在一般情况下，A 同构于这样的代数 A' 与理想$a'_0$ 的商；令 $a'_j$ 表示 A' 中 $a_j$ 的逆像，并令 $x'_i$ ($1 \leq i \leq r$) 为 A' 的元素，对于环 A'，叙述满足条件且递增序列理想$a'_0 \subset a'_1 \subset \ldots \subset a'_p$。然后A中的$x'_i$的像$x_i$为$i > h(0)$满足所需的条件；这对于条件 (b) 和条件 (a) 来说是显而易见的，这是从§ 1, no. 1、命题 2 得出的；最后，如果 $x_i(h(0) + 1 \leq i \leq r)$ 在 k 上不是代数独立的，则将存在一个非零多项式

$$
Q \in k[X_{h(0)+1}, \ldots, X_r]
$$

其中 $Q_j$ 是 $k[Y_1, \ldots, Y_m]$ 中的多项式；由于 $a_p \neq 0$ 在 $k$ 中是可逆的，所以 (4) 肯定是一个积分相关方程，其系数在 B 中，从而我们的断言。

因此，A 的分数 $k(Y_1, \ldots, Y_r)$ 的域是 B 的分数 $k(x_1, \ldots, x_m)$ 的域的代数，这证明 (代数, 章 V, § 5, no. 3, 定理 4) $x_i$ ($1 \leq i \leq m$) 是代数独立的。此外，$a \cap B = Bx_1$；对于每个元素 $z \in a, \cap B$ 可以写成 $z = x_1 z'$ 其中 $z' \in A \cap k(x_1, \ldots, x_r)$；但$A \cap k(x_1, \ldots, x_r) = k[x_1, \ldots, x_m] = B$，因为$B$是整体闭的（$\S$1，no. 3，推论2到命题13）；因此$z' \in B$，在这种情况下完成了属性（a）和（b）的证明。

(A2) **一般情况 ($p = 1$).**
我们通过归纳对$m$进行争论，$m = 0$的情况是微不足道的。 显然我们可以假设$a_i \neq 0$（否则我们可以对$1 \leq i \leq m$和$h(1) = 0$取$x_i = Y$）。 令$x_1$为$a_i$的非零元素；由(A1) 存在$t_2, \ldots, t_m$，使得$x_1, t_2, \ldots, t$在代数上独立于$k$，$A$在$C = k[x_1, t_2, \ldots, t_m]$和$x_1 A \cap C = x_1 C$上积分。 归纳假设存在 $k[t_2, \ldots, t_m]$ 和整数 $h$ 的元素 $x_2, \ldots, x_m$，使得 $k[t_2, \ldots, t_m]$ 在 $B' = k[x_2, \ldots, x_m]$ 上积分，$x_2, \ldots, x_m$ 在 $k$ 上代数独立，理想的 $a_i \cap B'$ 生成为$x_2, \ldots, x_h$。 那么 $C$ 是 $B = k[x_1, x_2, \ldots, x_m]$ 的积分 ($\S$ 1, no. 1, 命题 5 的推论)，因此 $A$ 也是 ($\S$ 1, no. 1, 命题 6 )；与情况 (A1) 中相同的论证表明 $x_1, \ldots, x_m$ 在代数上独立于 $k$；最后，因为$x_1 \in a_i$和$B = B'[x_1], a_i \cap B = Bx, + (a_i \cap B')$，并且因为$a_i \cap B'$是由$x_2, \ldots, x_h, a_i \cap B$生成（在$B'$中），是由$x_1, x_2, \ldots, x_h$生成（在$B$中）。

(B) **从 $p - 1$ 顶部开始的通道。**
令$t_1, \ldots, t_r$为理想$a_1 \subset \ldots \subset a_{p-1}$的递增序列为$A$满足条件为定理元素，并让我们写成$r = h(p - 1)$。由 (A2) 存在 $k[t_{r+1}, \ldots, t_m]$ 和整数的元素 $x_{r+1}, \ldots, x_s$ 使得
$$
C = k[t_{r+1}, \ldots, t_m]
$$
在 $B' = k[x_{r+1}, \ldots, x_m]$ 上积分，$x_{r+1}, \ldots, x_s$ 在 $k$ 上代数独立，理想的 $a_p \cap B'$ 由 $x_{r+1}, \ldots, x_s$ 生成。将$x_i = t_i$代入$i \leq r$，得到的$(x_i)_{1 \leq i \leq m}$家人可以用$h(p) = s$解决问题。
因为$A$是$C[t_1, \ldots, t_r] = C[x_1, \ldots, x_r]$的积分，因此也超过$B = k[x_1, \ldots, x_m] = B'[x_1, \ldots, x_r]$，因为$C$是$B'$的积分（$\S$1，no. 1，命题5和命题6的推论）；可以如情况 (A1) 所示，$x_i$ 在$k$ 上是代数独立的。另一方面，对于$j \leq p - 1$，理想的
$$
a_j \cap k[x_1, \ldots, x_r, t_{r+1}, \ldots, t_m]
$$
由 $x_1, \ldots, x_r, t_{r+1}, \ldots, t_m$ 中的多项式的假设集合组成，其所有单项式包含元素 $x_1, \ldots, x_{h(j)}$ 之一；由于$x_{r+1}, \ldots, x_m$是$t_{r+1}, \ldots, t$中的多项式，系数在$k$中，因此可以立即看出$x_1, \ldots, x_r, x_{r+1}, \ldots, x_s$中的多项式（其系数在$k$中）只有当其所有单项式包含之一时才能从属于到$a_j$ 元素$x_1, \ldots, x_{h(j)}$。最后，由于$x_1, \ldots, x_r$属于到$a_{p-1}$，因此也到$a_p$，$a_p \cap B'[x_1, \ldots, x_r]$由$x_1, \ldots, x_r$中的多项式和$B'$中的系数组成，其常数项属于到$a_p \cap B'$；因此，这个理想是由$x_1, \ldots, x_r, x_{r+1}, \ldots, x_t$产生的。

#### 推论 1 {#ac-v-s3-thm-1-cor-1 .statement tag=04R9}

设$A$为整环，$B$有限生成的$A$代数包含$A$为子环。则存在 $A$ 的元素 $s \neq 0$ 和 $B$ 的子代数 $B'$ 同构于多项式代数 $A[Y_1, \ldots, Y_n]$，使得 $B[s^{-1}]$ (章 II, § 2, no. 1) 整的$B'[s^{-1}]$。

我们写$S = A - \{0\}$，令$A$分数$k = S^{-1}A$域；显然 $S^{-1}B$ 是有限生成的 $k$ 代数，并且由于它包含 $k$ by 假设 (章 II, § 2, no. 4, 定理 1)，它不会减少到 0。通过定理 1 （应用的 top = 1）和$a_i = 0$）因此存在$S^{-1}B$的元素的有限序列$(x_i)_{1 \leq i \leq n}$，它们在代数上独立于$k$，并且$S^{-1}B$是$k[x_1, \ldots, x_n]$的积分。令$(z_j)_{1 \leq j \leq m}$为$A$-代数$B$的生成元的系统；在 $S^{-1}B$ 中，$z_j/1$ 中的每一个都满足积分相关方程

$$
(z_j/1)^{a_j} + \sum_{h < a_j} P_{hj}(x_1, \ldots, x_n)(z_j/1)^h = 0
$$

其中 $P_{hj}$ 是 $x_i$ 中的多项式，系数在 $k$ 中。 $A$存在元素$s \neq 0$，因此我们可以写出$x_i = y_i/s$，其中$1 \leq i \leq n$为$\in B$，$P_{hj}$的所有系数均为形式$c/s$，其中$c \in A$；最后，如果需要，替换，$s$乘以$S$的元素乘积，我们可以假设在$B$

$$
sz_j^{a_j} + \sum_{h < a_j} Q_{hj}z_j^h = 0
$$

其中 $Q_{hj}$ 是 $y_1, \ldots, y_n$ 中的多项式，系数在 $A$ 中；如果我们写 $z'_j = sz_j$，可以看出，将 (6) 乘以 $s^{a_j-1}$，$z'_j$ 是$B' = A[y_1, \ldots, y_n]$ 的整数。我们证明 $y_i$ 在代数上独立于 $A$；如果形式 $\sum_p a_p y_1^{p_1} \ldots y_n^{p_n} = 0$ 中有关系，其中 $a_p \in A$ 对应于所有 $p$，我们可以推导出 $S^{-1}B$ 中的 $\sum_p a'_p x_1^{p_1} \ldots x_n^{p_n} = 0$，其中 $k$ 中的 $a'_p = a_p s^{p_1 + \cdots + p_n}$； 假设，因此$a'_p = 0$对于所有$p$，从而$a_p = 0$对于所有$p$。此外，在环$B[s^{-1}]$中，每个$z'_j/1$在$B'[s^{-1}]$上积分（§ 1, no. 1，命题2），并且，如$B[s^{-1}]$中的$z_j/1 = (z'_j/1)(1/s)$，可以看出，$z_j/1$在$B'[s^{-1}]$上积分，完成证明 (§ 1, no. 1, 命题 4)。

#### 推出 2 {#ac-v-s3-thm-1-cor-2 .statement tag=04RA}

令$K$为域、$K$的$A$子环以及$A$的分数$L$域。如果$K$是有限生成的$A$代数，则$[K:L]$是有限的并且$A$中存在$a \neq 0$使得$L = A[a^{-1}]$。

由推论 1 可知，存在 $K$ 的元素 $x_1, \ldots, x_n$ 和 $A$ 的元素 $a \neq 0$，使得 $x_1, \ldots, x_n$ 在 $A$ 上（因此在 L 上）在代数上独立，并且 K 在子环上是整数$A[x_1, \ldots, x_n, a^{-1}]$。那么从 §2, no.1, 引理 2 可以得出 $A[x_1, \ldots, x_n, a^{-1}]$ 是域。但多项式环$C[Y_1, \ldots, Y_n]$中唯一超过整环C的可逆元是C的可逆元； 应用这个注到$C = A[a^{-1}]$，可以看出必然是$n = 0$并且$A[a^{-1}]$是域等于L除以后者的定义。由于 K 是 L 上的积分，并且是有限生成的 L-代数，因此次数 [K:L] 是有限的 (§ 1, no. 1，命题 4)。

#### 推论 3 {#ac-v-s3-thm-1-cor-3 .statement tag=04RB}

设A为整环，B为B的有限生成的A-代数和b元素，使得对于A中的所有$z \neq 0$和每个整数$n > 0$，$zb^n \neq 0$。设$\varphi : A \to B$为典范同态； A 中存在 $a \neq 0$，使得对于从 A 到代数闭域 L 的每个同态 f 使得 $f(a) \neq 0$，存在从 B 到 L 的同态 g 使得 $g(b) \neq 0$ 和 $f = g \circ \varphi$。

b 上的假设意味着，如果h是B到$B[b^{-1}]$的典范同态$x \mapsto x/1$，则A到$B[b^{-1}]$的同态$h \circ \varphi$是单射的。因此，根据推论 1，存在 A 的元素 $a \neq 0$ 和 $B[b^{-1}]$ 的子环 $B'$，使得 $B[b^{-1}, a^{-1}]$ 在 $B'[a^{-1}]$ 上积分，并且$B'$ 同构于多项式代数 $A[Y_1, \ldots, Y_n]$。令f为从A到代数闭域L的同态，使得$f(a) \neq 0$；存在从$A[Y_1, \ldots, Y_n]$到L延伸f的同态，因此存在从$B'$到L延伸f的同态$f'$。由于L中的$f'(a) \neq 0$，从$B'[a^{-1}]$到L存在同态$f''$，使得

$$
f''(x/a^n) = f'(x) \cdot (f(a))^{-n}
$$

对于所有$x \in B'$和所有$n > 0$（章II, §2, no. 1，命题1）。最后，由于$B[b^{-1}, a^{-1}]$是$B'[a^{-1}]$的积分，因此存在从$B[b^{-1}, a^{-1}]$到L延伸$f''$的同态$f'''$（§2, no. 1，推论4到定理1）。如果从 B 到 $B[b^{-1}, a^{-1}]$ $j : x \mapsto x/1$ 是典范同态，$g = f''' \circ j$ 可以求解问题，因为 $j(b)$ 在 $B[b^{-1}, a^{-1}]$ 中是可逆的，因此$f'''(j(b)) \neq 0$ 在 L 中是可逆的。

注，如果假设推论3中的B为整环且$A \subset B$，则b上的假设等价于$b \neq 0$。

### 2. 有限生成代数超过域的积分闭包

#### 定理 2 {#ac-v-s3-thm-2 .statement tag=04RC}

设A是有限生成的积分K-代数，K是分数的域，$A'$是A在域K'中的积分闭包，它是K的有限代数扩张。那么$A'$是有限生成A-模和有限生成的K-代数。

通过定理 1，存在 A 的子代数 C 同构于多项式代数 $k[X_1, \ldots, X_n]$，并且 A 对 C 是积分； $A'$显然是C在K'中的积分闭包(§ 1, no. 1,命题6)；因此，我们可以将注意力集中在$A = k[X_1, \ldots, X_n]$的情况。 令$N$为由$K'$生成的$K$（在$K$的代数闭包中）的拟伽罗瓦扩张，它是$K$的有限代数扩张（代数，章V, § 6, no. 3，推论1为命题9)。 只需证明$N$中$A$的积分闭包$B$是有限生成的$A$模，因为$A'$是$B$的子$A$模，$A$是诺特环 （章III, § 2, no. 10，推论2至定理2）。 因此，我们可以将注意力集中在$K'$是$K$的拟伽罗瓦扩展的情况。 然后我们知道（代数，章V, § 10, no. 9，命题14）$K'$是$K$的（有限）根式扩张$K''$的（有限）伽罗瓦扩张。 如果$A''$是$K''$中$A$的积分闭包，$A'$是$K'$中$A''$的积分闭包，则足以证明$A''$是有限生成的$A$模，$A'$是有限生成的$A''$-模块。 现在，如果证明$A''$是有限生成的$A$模，则它是诺特域，被定义整闭； $A$ 是有限生成的 $A''$ 模块这一事实将从 § 1, no. 6、推论 1 到命题 18 得出。

因此我们看到，我们可以将注意力集中在$A = k[X_1, \ldots, X_n]$且$K'$是$K = k(X_1, \ldots, X_r)$的有限根扩张的情况。那么$K'$由元素$(y_i)_{1 \leq i \leq m}$的有限族生成，并且存在$k$的特征指数幂$q$使得$y_i^q \in k(X_1, \ldots, X_r)$。设$c_j$($1 \leq j \leq r$)为$X_1, \ldots, X_r$中有理函数的分子和分母的系数，等于$y_i^q$($1 \leq i \leq m$)。那么$K'$包含在扩张$L = k'(X_1^{q^{-1}}, \ldots, X_n^{q^{-1}})$中，其中$k' = k(c_1^{q^{-1}}, \ldots, c_r^{q^{-1}})$（我们位于$K'$的代数闭包中），$A$包含在$A$的代数闭包$B'$中$L'$。现在，$k'$是$k$的代数，因此$C' = k'[X_1, \ldots, X_n]$是$A$的积分（$§ 1$、no. 1、命题 5）；由于 $k'[X_1^{q^{-1}}, \ldots, X_n^{q^{-1}}]$ 是整闭的（$§ 1$，no. 3，推论 2 到命题 13），可以看出，这个环是 $C'$ 在 $L'$ 的整闭，因此也是 $A$ 的整闭（$§ 1$， no. 1、命题6)，其他字$B' = k'[X_1^{q^{-1}}, \ldots, X_n^{q^{-1}}]$。现在显然$B'$是一个有限生成的$C'$模块（$§ 1$，no. 1，命题4），并且由于$k'$是$k$的有限扩张，所以$C'$是一个有限生成的$A$-模块，因此$B'$是有限生成的$A$-模块；由于$A$是诺特和$A \subset B'$，$A'$是有限生成的$A$模块。

### 3.零点定理

#### 命题 1 {#ac-v-s3-prop-1 .statement tag=04RD}

令 $A$ 为域 $k$ 和 $L$ 代数闭包上 $k$ 的有限生成的代数。

(i) 如果$A \neq \{0\}$，则存在从$A$到$L$的$k$同态。

(ii) 设$f_1, f_2$是从$A$到$L$的两个$k$同态。为了使$f_1$和$f_2$具有相同的核，存在$L$的$k$自同构$s$使得$f_2 = s \circ f_1$是充分必要的。

(iii) 设$a$为$A$的理想。为了使$a$极大，它是从$A$到$L$的k-同态的核是必要且充分的。

(iv) 对于$A$的元素$x$使得$f(x) = 0$对于从$A$到$L$的每个k-同态$f$，$x$是幂幂的充分必要。

断言 (i) 从no. 1得出，推论3到定理1应用替换$A$乘$k$，$B$乘$A$，$b$乘单位元 $B$和$f$由$k$的典范嵌入变为$L$。

如果$f$是从$A$到$L$的k-同态，则$f(A)$是$L$包含$k$的子环；因为$L$是$k$的代数扩张，$f(A)$是域（代数，章V, § 3, no. 2，命题3），并且如果$a$是核关闭，$A/a$与$f(A)$同构的，因此是域，这证明$a$是最大的。相反，如果$a$是$A$的最大理想，则从(i)可知存在从$A/a$到$L$的k-同态，因此存在$A$到$L$的k-同态，其核$b$ 包含$a$；但由于$a$极大，所以$b = a$；这就证明了(iii)。

我们现在证明(ii)。如果$s$是$L$的k-自同构，使得$f_2 = s \circ f_1$，显然$f_1$和$f_2$有相同的核。相反，假设$f_1$和$f_2$具有相同的核；则存在域$f_1(A)$到域$f_2(A)$的k-同构$s_0$使得$f_2 = s_0 \circ f_1$；但通过代数、章V, § 6, no. 3、命题7、$s_0$扩展到$L$的k自同构，因此$f_2 = s \circ f_1$。

最后，如果$x \in A$满足$x^n = 0$，对于从$A$到$L$的每个k-同态$f$，$(f(x))^n = f(x^n) = 0$，因此$f(x) = 0$，因为$L$是域。相反，假设 $x \in A$ 不是幂零的；那么 $A[x^{-1}]$ 是一个有限生成的 $A$ 代数（因此是有限生成的 K-代数），不会减少到 0 (章 11, § 2, no. 1, 注 3)，因此存在从 $A[x^{-1}]$ 到 的 k 同态 $g$ $L$ (i)。如果$j : A \to A[x^{-1}]$是典范同态，则$f = g \circ j$是从$A$到$L$和$f(x)g(1/x) = g(x/1)g(1/x) = g(1) = 1$、从而$f(x) \neq 0$的k同态。

设$k$为域且$L$扩张域为$k$； $L^n$的元素$x = (x_1, \ldots, x_n)$在多项式环$k[X_1, \ldots, X_n]$的理想$c$的$L^n$中被称为零，如果

$$
P(x) = P(x_1, \ldots, x_n) = 0
$$

对于所有$P \in r$。

#### 引理 1 {#ac-v-s3-lem-1 .statement tag=04RE}

设$A$是这个代数的生成元和$c$在域$k$、$(a_i)_{1 \leq i \leq n}$系统上的有限生成的代数和$a_i$之间的代数关系的理想，系数为$k$（代数、章IV, § 2, no. 1）。 对于$k$的每个扩张域$L$，映射$f \mapsto (f(a_i))_{1 \leq i \leq n}$是从$A$到$L$到集合的k同态的双射或集合 $L^n$ 中的$r$ 零。

存在$k[X_1, \ldots, X_n]$到$A$的唯一K-代数同态$h$，使得$h(X_i) = a_i$，对于$1 \leq i \leq n$和定义$r$是$h$的核。 映射 f $\mapsto$ 他从$A$到$L$的k-同态的集合的双射到从$k[X_1, \ldots, X_n]$到$L$的k-同态的集合，它们是c上的零。对于每个多项式 $P \in k[X_1, \ldots, X_n]$ 和每个元素 $x = (x_1, \ldots, x_i) \in L^n$，我们写 $h_x(P) = P(x)$；那么映射$x \mapsto h_x$是$L^n$的双射到从$k[X_1, \ldots, X_n]$到$L$的k同态的集合上（这样同态由其在$X_i$处的值确定） ($1 \leq i \leq n$));说$h_x$在c上是零意味着$x$是$L''$、从而引理中c的零。

如果将命题 1 应用于代数 $A = k[X_1, \ldots, X_n]/r$，其中c是与整个环不同的$k[X_1, \ldots, X_n]$的理想，我们通过引理 1获得以下叙述：

#### 命题 2 (希尔伯特零点定理) {#ac-v-s3-prop-2 .statement tag=04RF}

令 k 为域，k 为 L 代数闭包。

(i) 每个理想$r \not\subset k[X_1, \ldots, X_n]$而非包含1都在$L^n$中至少承认一个零。

(ii) 设$x = (x_1, \ldots, x_n), y = (y_1, \ldots, y_n)$为$L^n$中的两个元素；为了使 x 处的 $k[X_1, \ldots, X_n]$ 零多项式的集合与 y 处的 $k[X_1, \ldots, X_n]$ 零多项式的集合相同，存在 L 的 k 自同构 s 使得 $y_i = s(x_i)$ 对于 $1 \leq i \leq n$ 是充分必要的。

(iii) 为了使 $k[X_1, \ldots, X_n]$ 的理想 a 最大，$L^n$ 中存在一个 x，使得 a 是 $k[X_1, \ldots, X_n]$ 零在 x 处的多项式的集合，这是充分必要的。

(iv) 对于$k[X_1, \ldots, X_n]$的理想c的$L''$中$k[X_1, \ldots, X_n]$的多项式Q在零的集合上为零，存在整数 m > 0使得$Q^m \in c$是必要且充分的。

### 4.雅各布森环

#### 定义 1 {#ac-v-s3-def-1 .statement tag=04RG}

如果 A 的每个素理想都是极大理想族的交，则环 A 称为 Jacobson 环。

Examples

(1) 每个域都是雅各布森环。
(2) 环 $\mathbf{Z}$ 是 Jacobson 环，非极大值的唯一素理想 (0) 是 $\mathbf{Z}$ 的极大理想 $(p)$ 的交，其中 $p$ 贯穿素数数的集合 （cf.命题4）。
(3) 设 A 为 Jacobson 环，且 a 为 A 的理想。则 $A/a$ 为 Jacobson 环，因为 $A/a$ 的理想为形式 $b/a$，其中 b 为包含 a 的理想，$b/a$ 为素数（分别为最大值）当且仅当 b 是。

#### 命题 3 {#ac-v-s3-prop-3 .statement tag=04RH}

对于环 A 是雅各布森环，对于 A 的每个理想 a，$A/a$ 的雅各布森根式等于其零根式 (章 II, § 2, no. 6) 是充分必要的。

$A/a$ 的雅各布森根式（或零根式）是 $A/a$ 最大（或素数）理想的交 (*代数*, 章 VIII, § 6, no. 3, 定义 3 和 *交换代数*, 章 II, § 2, no. 6、命题 13)。因此，所述条件意味着对于素理想包含$a$的$A$交的每个理想$a$等于最大理想包含$a$的交。如果 $A$ 是 Jacobson 环，则条件显然适用于 $A$ 的每个理想 $a$；相反，如果它对于$A$的每个素理想都成立，则$A$是雅各布森环乘以定义。

#### 推论 {#ac-v-s3-n4-cor-1 .statement tag=04RI}

*设$A$为Jacobson环；对于$A$的每个理想$a$，$a$的根式是$A$包含$a$的最大理想交。*

$A/a$ 是 Jacobson 环就足以满足注的要求。

#### 命题 4 {#ac-v-s3-prop-4 .statement tag=04RJ}

*令$A$为主理想整环，$(\mathbf{p}_\lambda)_{\lambda \in L}$为$A$的极值元素的代表系统（*代数*，章VII, § 1, no. 3，定义2）。为了使$A$成为雅各布森环，$L$是无穷大是充分必要的。*

$A$ 的最大理想是 $A\mathbf{p}_\lambda$（*loc.cit.*、no. 2、命题 2）。如果$L$是有限的，则它们的交是理想的$Ax$，其中$x = \prod_{\lambda \in L} \mathbf{p}_\lambda$（*同上。*），因此与$(0)$不同；另一方面，如果$L$是无限的，$A\mathbf{p}_\lambda$的交是$(0)$，$A$的每个元素$\neq 0$只能被极值元素的有限数整除（*loc.引用。*，no. 3，定理2）。 命题那么，$(0)$ 是$A$ 中唯一非极大值的素理想 (*代数*, 章 VI, § 1, no. 13, 命题 14 (DIV))。

#### 命题 5 {#ac-v-s3-prop-5 .statement tag=04RK}

*令 $A$ 为环，并且 $B$ 为 $A$ 上的 $A$ 代数积分。如果 $A$ 是 Jacobson 环，那么 $B$ 也是。*

替换 $A$ 由$B$中的典范像，我们可以假设$A \subset B$。设$\mathfrak{p}'$为$B$的素理想，并设$\mathfrak{p} = A \cap \mathfrak{p}'$。 假设存在一个$(\mathfrak{m}_\lambda)_{\lambda \in L}$最大理想族$A$，其交等于顶。对于所有$\lambda \in L$，存在最大理想$\mathfrak{m}'_\lambda$，即$B$，位于$\mathfrak{m}_\lambda$和包含$\mathfrak{p}'$之上（§ 2, no. 1、命题1和推论2到定理1）。如果我们写$\mathfrak{q}' = \bigcap_{\lambda \in L} \mathfrak{m}'_\lambda$，则$\mathfrak{q}' \cap A = \bigcap_{\lambda \in L} \mathfrak{m}_\lambda = \mathfrak{p}$和$\mathfrak{q}' \supset \mathfrak{p}'$，从而$\mathfrak{q}' = \mathfrak{p}'$（$2$，no. 1，推论1到命题1）。

#### 定理 3 {#ac-v-s3-thm-3 .statement tag=04RL}

*令 $A$ 为 Jacobson 环，$B$ 为有限生成的 $A$ 代数，$\varphi : A \to B$ 典范同态。然后：*
(i) *$B$ 是 Jacobson 环。*
(ii) *对于$B$的每个最大理想$m'$，$m = \varphi^{-1}(m')$是$A$的最大理想，$B/m'$是$A/m$的有限代数扩张。*

设$\mathfrak{p}'$为$B$和$\mathfrak{p} = \varphi^{-1}(\mathfrak{p}')$的素理想。令 $v$ 为 $B/\mathfrak{p}'$ 的元素 $\neq 0$。

由于 $B/p'$ 是有限生成积分 (Alp) 代数，并且典范同态 $\phi : A/p \to B/p'$ 是单射，因此存在 $A/p$ 的元素 $u \neq 0$，使得对于从 $A/p$ 到每个同态 $f$ 代数闭域 $L$，其核不包含 $u$，从 $B/p'$ 到$L$，存在同态 $g$，其核不包含 $v$ 且$f = g \circ \phi$（no. 1，推论 3 至定理 1）。由于$A$是雅各布森环，因此存在$A$包含$p$的最大理想$m$，并且$u \notin m/p$。我们取$L$为$A/m$的代数闭包，$f$为典范同态$A/p \to L$；让

$$
g : B/p' \to L
$$

是同态使得$f = g \circ \phi$和$g(v) \neq 0$。然后

$$
A/m \subset g(B/p') \subset L,
$$

因此，$g(B/p')$是$K$的子域（代数，章V, § 3, no. 2，命题3），并且$g$的核因此是$B/p'$而不是包含的最大理想$v$。由此可见，$B/p'$的极大理想中的交减少为0，证明$B$是雅各布森环。此外，如果$p'$最大，则$g$必然是内射的，因此$p = m$最大；最后$B/p'$是在域$A/m$上有限生成的代数，因此是$A/m$的有限扩张（no. 1，推论2到定理1）。

#### 推论 1 {#ac-v-s3-thm-3-cor-1 .statement tag=04RM}

*每个在$\mathbf{Z}$上有限生成的代数$A$都是Jacobson环；对于素理想 $p \subset A$ 来说，环 $A/p$ 是有限的是充分必要的。*

如果整环$A/p$是有限的，则它是域，因为对于$A/p$中的每个$u \neq 0$，$A/p$的映射$v \mapsto uv$对其自身是单射的，因此是双射的，因为$A/p$是有限的。相反，对于$A$的每个最大理想$m$，$A$中$m$的逆像是最大理想（$p$），并且$A/m$在素数域$\mathbf{Z}/(p) = \mathbf{F}_p$上有限定理3。

#### 推论 2 {#ac-v-s3-thm-3-cor-2 .statement tag=04RN}

*令$(P_\lambda)_{\lambda \in L}$为$\mathbf{Z}[X_1, \ldots, X_n]$中的多项式族，并令$Q$为$\mathbf{Z}[X_1, \ldots, X_n]$中的多项式，使得对于元素$(x_i)_{1 \leq i \leq n}$属于到有限域的每一个系统且对于其中$P_\lambda(x_1, \ldots, x_n) = 0$适用于所有$\lambda$，还有$Q(x_1, \ldots, x_n) = 0$。那么，如果$a$是由$P_\lambda$生成的$\mathbf{Z}[X_1, \ldots, X_n]$的理想，则存在整数$m > 0$使得$Q^m \in a$。此外，对于$R$的每个减少的环$R$和元素的每个系统$(y_i)_{1 \leq i \leq n}$，使得$P_\lambda(y_1, \ldots, y_n) = 0$对于所有$\lambda$来说，也是$Q(y_1, \ldots, y_n) = 0$。

第二个断言是从第一个$\mathbf{Z}[X_1, \ldots, X_n]$由……组成多项式$P$的理想值得出的，这样$P(y_1, \ldots, y_n) = 0$包含$a$。为了显示第一个断言，注就足够了，对于$A = \mathbf{Z}[X_1, \ldots, X_n]$包含$a$的每个最大理想$m$，$A/m$是有限域（推论1）并且假设意味着： $A/m$中$Q$的典范像为零；然后$Q$属于到$A$包含$a$的最大理想交，这是$a$的根式（命题3的推论）。

#### 推论 3 {#ac-v-s3-thm-3-cor-3 .statement tag=04RO}

*令 $A$ 为 Jacobson 环。如果存在有限生成的$A$-代数$B$包含$A$且为域，则$A$为域且$B$为$A$的代数扩张。*

应用定理 3 (ii) 和 $m' = (0)$ 就足够了。

### 习题{#ac-v-s3-exercises}

对于$A$的每个素理想$\mathfrak{p}$，都存在一个位于$\mathfrak{p}$之上的$A'$素理想$\mathfrak{p}'$。通过 *reductio adabsurdum* 进行论证：let $x \in A' \cap \mathfrak{g}A$ 和 let $a = A \cap (x^{-1}A)$，这是与 $A$ 不同的理想。设$\mathfrak{p}$为与$A/a$相关的素理想；运输者$b = a : \mathfrak{p}$不同于$a$（章IV, § 1, no. 4，命题9），因此存在$y \in b$使得$xy \notin A$和
$$
xy \mathfrak{p} \subset \mathfrak{p}A' \cap A = \mathfrak{p};
$$
推导出矛盾。）

**93**

§ 3](exercises/s3/)参见[习题。
