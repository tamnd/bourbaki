---
book: ac
book_title: Commutative Algebra
chapter: I
chapter_title: FLAT MODULES
section: 1
section_title: Diagrams and exact sequences
lang: zh
source: ac-i-vii
book_pages: 1-9, 39-40
pdf_pages: 0021-0029, 0059-0060
extraction: ocr
subsections:
    - "no": 1
      title: DIAGRAMS
      page: 1
      pdf_page: 21
    - "no": 2
      title: COMMUTATIVE DIAGRAMS
      page: 2
      pdf_page: 22
    - "no": 3
      title: EXACT SEQUENCES
      page: 3
      pdf_page: 23
    - "no": 4
      title: THE SNAKE DIAGRAM
      page: 4
      pdf_page: 24
statements: 7
exercises: 7
content_sha256: 548625ed5b0f80f5d67594e7080605c7b21a8f1c7deb8e502b4b45a933a5e59c
translated_from: content/en/ac/I/01_s1_diagrams_and_exact_sequences.md
translation_method: google
source_content_sha256: e122c6b77c1c3a3f195f1e5d14b8ed8bb246e933209f2cbcd2975f972a3111ae
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: 7d860333c3b6d441e0974e4924225834839e996cc4122ac5b4daea47c5a3260d
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## 1. 图表和正合序列

### 1.图表

对于例，$A, B, C, D, E$ 为 5 个集合，从 $A$ 到 $B$，$f$ 为映射，从 $B$ 到 $C$，$h$，$g$ 映射映射从$D$到$E$，$u$映射从$B$到$D$以及$v$映射从$C$到$E$。为了总结这种情况，我们经常使用图表；对于例，上述情况总结如下

(*) 除§ 4外，此章的结果仅取决于书籍I至VI。

图表（集合理论，章II, § 3, no. 4）

$$
\begin{array}{ccc}
A & \xrightarrow{f} & B \\
& & \downarrow u \\
& & D \\
& & \downarrow v \\
& & E \\
& & \xrightarrow{h}
\end{array}
$$

(1)

在这样的符号$A \xrightarrow{f} B$的图表群中，示意性地表达了从$A$到$B$$f$是映射的事实。如果$f$没有歧义，我们会隐藏字母$f$并简单地写为$A \to B$。

当 $A, B, C, D, E$ 为群（或可交换的群）且 $f, g, h, u, v$ 群同态时，图表 (1) 被缩写为图表或群（或可交换的群）。

在原理中，图表不是一个数学对象，而只是一个为了方便阅读论证而设计的图形。在实践中，图表经常被用作缩写符号，以避免命名所有正在考虑的集合和映射；因此，我们说“考虑图表（1）”而不是说“让A，B，C，D，E为五个集合...以及从C到E的$v$映射”；请参阅 no. 4 中命题 2 的例叙述。

### 2.可交换图表

对于例，考虑以下图表：

$$
\begin{array}{ccccccc}
A & \xrightarrow{f} & B & \xrightarrow{g} & C & \xrightarrow{h} & D \\
a \downarrow & & b \downarrow & & c \downarrow & & d \downarrow \\
A' & \xrightarrow{f'} & B' & \xrightarrow{g'} & C' & \xrightarrow{h'} & D'
\end{array}
$$

(2)

对于每条由段、图表的某个数、第一个线段的开头所代表的对应、映射、集合的箭头所示方向遍历到最后一个线段的结尾所代表的集合所组成的路径，即映射的合成由遍历的各个段表示。对于图表的每个顶点，对于例 B，按照约定，有一条简化为 B 的路径，其中对应恒等映射 1，

在(2)中，例有3条路径，起始于$A$，结束于$C'$； 相应的映射是$c \circ g \circ f, g' \circ b \circ f$和$g' \circ f' \circ a$。如果对于图表中具有相同起点和终点的每条对路径，相应的映射相等，则称图表是可交换的；特别是如果路径重合相应的映射的开头和结尾必须是同一元。

对于图表 (2) 可交换，关系是充分必要的
$$
f' \circ a = b \circ f, \quad g' \circ b = c \circ g, \quad h' \circ f = d \circ h;
$$
持有；在其他字中，(2)中包含的三个平方图表可交换是充分必要的。对于关系 (3) 意味着从$c \circ g = g' \circ b$开始为$c \circ g \circ f = g' \circ b \circ f$，从$b \circ f = f' \circ a$开始为$g' \circ b \circ f = g' \circ f' \circ a$；因此，从$A$开始到$C'$结束的三个路径给出相同的映射。可以类似地验证从$A$开始到$D'$结束的4条路径（分别从$B$开始到$D'$结束的3条路径）给出相同的映射。 关系 (3) 表示从 $A$（分别为 B、C）开始到 $B'$（分别为 C'、D'）结束的两条路径给出相同的映射。 (2) 的其他对顶点都不能由多条路径连接，因此图表 (2) 是可交换的。

下面我们将让读者验证图表的其他型的类似结果。

### 3.正合序列

回忆一下以下定义（代数，章II, § 1, no. 4）：

#### 定义 1 {#ac-i-s1-def-1 .statement tag=0421}

令$A$为环、$F, G, H$三个右（左）$A$模块、$F$至$G$的$f$同态和$g$同态 $G$ 至 $H$。如果$\overline{g}^{-1}(0) = f(F)$，即$g$的核等于$f$的像，则有序对$(f, g)$称为正合序列。

图表
$$
\begin{array}{ccc}
F & \xrightarrow{f} & G \\
& & \xrightarrow{g} \\
& & H
\end{array}
$$
也称为正合序列。

类似地考虑四个模和三个同态中的图表由……组成：
$$
E \xrightarrow{f} F \xrightarrow{g} G \xrightarrow{h} H.
$$
如果图表 $E \xrightarrow{f} F \xrightarrow{g} G$ 是正合序列，则该图表被认为精确于$F$；如果 $F \xrightarrow{g} G \xrightarrow{h} H$ 是正合序列，则据说精确于 $G$。如果 (5) 在 $F$ 和 $G$ 处精确，则称它是精确的，或者也是正合序列。 正合序列与项中的任何数的定义类似。

回想一下以下结果（前述），其中 $E, F, G$ 表示右（左）

A-模，箭头代表同态，$0$表示模减少到单位元素：

(a) 说$0 \to E \xrightarrow{f} F$是正合序列等价于说，$f$是单射的。

(b) 说 $E \xrightarrow{f} F \to 0$ 是正合序列等价于说 $f$ 是满射。

(c) 说$0 \to E \xrightarrow{f} F \to 0$是正合序列等价于说，$f$是双射，即$f$是$E$到$F$的同构。

(d) 如果$F$是$E$的子模并且$i$表示$F$的典范嵌入进入$E$并且$p$典范满射进入$E$进入$E/F$， 图表
$$
\begin{array}{ccccccc}
0 & \longrightarrow & F & \xrightarrow{i} & E & \xrightarrow{p} & E/F \longrightarrow 0
\end{array}
$$
是正合序列。

(e) 如果：$E \to F$ 是同态，图表
$$
\begin{array}{ccccccccc}
0 & \longrightarrow & f^{-1}(0) & \xrightarrow{i} & E & \xrightarrow{f} & F & \xrightarrow{p} & F/f(E) \longrightarrow 0
\end{array}
$$
（其中$i$是$(0)$的典范嵌入进入$E$和$p$，$F/f(E)$的规范投影）是正合序列。

(f) 图表
$$
\begin{array}{ccccc}
E & \xrightarrow{f} & F & \xrightarrow{g} & G
\end{array}
$$
要成为正合序列，存在模、$S$、$T$和同态、$a : E \to S$、$b : S \to F$、$c : F \to T$和$d : T \to G$是充分必要的，使得$f = b \circ a$， $g = d \circ c$ 和三个序列
$$
\begin{array}{ccccccccc}
E & \xrightarrow{a} & S & \longrightarrow & 0 \\
0 & \longrightarrow & S & \xrightarrow{b} & F & \xrightarrow{c} & T & \longrightarrow & 0 \\
0 & \longrightarrow & T & \xrightarrow{d} & G
\end{array}
$$
准确地说。

最后回想一下当且仅当：$E \to F$是A-模同态，我们集合$\operatorname{Ker}(f) = f^{-1}(0)$、$\operatorname{Im}(f) = f(E)$、$\operatorname{Coim}(f) = E/f^{-1}(0)$和$\operatorname{Coker}(f) = F/f(E)$。有了这个记号，就可以在(9)中取$S = \operatorname{Im}(f) = \operatorname{Ker}(g)$和$T = \operatorname{Im}(g)$（与$\operatorname{Coker}(f)$典型同构）。

### 4.蛇图表

#### 命题 1 {#ac-i-s1-prop-1 .statement tag=0422}

考虑交换性群的交换性图表：
$$
\begin{array}{ccccc}
A & \xrightarrow{u} & B & \xrightarrow{v} & C \\
a \downarrow & & b \downarrow & & c \downarrow \\
A' & \xrightarrow{u'} & B' & \xrightarrow{v'} & C'
\end{array}
$$

假设 (10) 的两行是精确的。然后：

(i) 如果 c 是单射的，我们有

(11) $\operatorname{Im}(b) \cap \operatorname{Im}(u') = \operatorname{Im}(u' \circ a) = \operatorname{Im}(b \circ u).$

(ii) 如果 a 是满射，我们有

(12) $\operatorname{Ker}(b) + \operatorname{Im}(u) = \operatorname{Ker}(v' \circ b) = \operatorname{Ker}(c \circ v).$

让我们证明（i）。显然

$$
\operatorname{Im}(u' \circ a) = \operatorname{Im}(b \circ u) \subset \operatorname{Im}(b) \cap \operatorname{Im}(u').
$$

相反，设$x \in \operatorname{Im}(b) \cap \operatorname{Im}(u')$。存在$y \in B$使得$x = b(y)$。作为 $v' \circ u' = 0$，我们有 $0 = v'(x) = v'(b(y)) = c(v(y))$、从而 $v(y) = 0$，因为 c 是单射的。由于$(u, v)$是正合序列，因此存在$z \in A$使得$y = u(z)$，从而$x = b(u(z))$。

让我们证明(ii)。由$v \circ u = 0$和$v' \circ u' = 0$可知

$$
\operatorname{Ker}(b) + \operatorname{Im}(u) \subset \operatorname{Ker}(v' \circ b) = \operatorname{Ker}(c \circ v).
$$

相反，令$x \in \operatorname{Ker}(v' \circ b)$。那么 $b(x) \in \operatorname{Ker}(v')$ 并且存在 $y' \in A'$ 这样 $u'(y') = b(x)$，因为序列 $(u', v')$ 是精确的。由于 a 是满射，因此存在 $y \in A$ 使得 $a(y) = y'$, 从而 $b(x) = u'(a(y)) = b(u(y))$；接下来是$x - u(y) \in \operatorname{Ker}(b)$，从而完成证明。

#### 引理 1 {#ac-i-s1-lem-1 .statement tag=0423}

考虑交换性群的交换性图表：

$$
\begin{array}{ccc}
A & \xrightarrow{u} & B \\
a \downarrow & & b \downarrow \\
A' & \xrightarrow{u'} & B'
\end{array}
$$

那么存在且仅有一个同态$u_1 : \operatorname{Ker}(a) \to \operatorname{Ker}(b)$和且仅有一个同态$u_2 : \operatorname{Coker}(a) \to \operatorname{Coker}(b)$使得图表

$$
\begin{array}{ccc}
\operatorname{Ker}(a) & \xrightarrow{u_1} & \operatorname{Ker}(b) \\
i \downarrow & & j \downarrow \\
A & & B
\end{array}
$$

和

$$
\begin{array}{ccc}
A' & \xrightarrow{u'} & B' \\
p \downarrow & & q \downarrow \\
\operatorname{Coker}(a) & \xrightarrow{u_2} & \operatorname{Coker}(b)
\end{array}
$$

是可交换的，i 和 j 表示典范嵌入，p 和 q 典范满射。

如果$x \in \mathrm{Ker}(a)$，则$a(x) = 0$和$b(u(x)) = u'(a(x)) = 0$，因此$u(x) \in \mathrm{Ker}(b)$，并且$u_1$的存在性和唯一性则为直接的。类似地，我们有 $u'(a(A)) = b(u(A)) \subset b(B)$，然后通过商 $u'$ 得到同态 $u_2 : \mathrm{Coker}(a) + \mathrm{Coker}(b)$，这是 (15) 唯一可交换的同态。

现在让我们从交换群的*交换*图表(10)开始； 对应到引理 1 图表

$$
\begin{array}{ccccccccc}
\mathrm{Ker}(a) & \xrightarrow{u_1} & \mathrm{Ker}(b) & \xrightarrow{v_1} & \mathrm{Ker}(c) \\
i \downarrow & & j \downarrow & & k \downarrow \\
A & \xrightarrow{u} & B & \xrightarrow{v} & C \\
a \downarrow & & b \downarrow & & c \downarrow \\
A' & \longrightarrow & B' & \longrightarrow & C' \\
\vdots & & \vdots & & \vdots \\
\cdots \to \mathrm{Coker}(a) & \xrightarrow{u_2} & \mathrm{Coker}(b) & \xrightarrow{v_2} & \mathrm{Coker}(c)
\end{array}
$$

其中 $i, j, k$ 是典范嵌入、$p, q, r$ 典范满射和 $u_1, u_2$（分别为 $v_1, v_2$）同态与 $u, u'$（分别为 $v, u'$）通过引理规范关联 1. 立即验证这个图表是可交换的。

#### 命题 2 {#ac-i-s1-prop-2 .statement tag=0424}

*假设在交换律中图表 (10) 序列 $(u, v)$ 和 $(u', u')$ 是精确的。然后：*

（一）$v_1 \circ u_1 = 0$；如果 $u'$ 是单射的，则序列 $(u_1, v_1)$ 是精确的。
(ii) $v_2 \circ u_2 = 0$；如果 $v$ 是满射，则序列 $(u_2, v_2)$ 是精确的。
(iii) *假设 $u'$ 是单射，$v$ 是满射。那么存在且仅有一个同态 $d : \mathrm{Ker}(c) \to \mathrm{Coker}(a)$ 和以下性质：如果$x \in \mathrm{Ker}(c)$、$y \in B$ 和$t' \in A'$ 满足关系 $v(y) = k(x)$ 和$u'(t') = b(y)$，则$d(x) = p(t')$。而且序列*

(*) $$
\begin{array}{cccccc}
\mathrm{Ker}(a) & \xrightarrow{u_1} & \mathrm{Ker}(b) & \xrightarrow{v_1} & \mathrm{Ker}(c) & \xrightarrow{d} \\
& & & & & \\
& & & & & \\
& & & & & \\
\mathrm{Coker}(a) & \xrightarrow{u_2} & \mathrm{Coker}(b) & \xrightarrow{v_2} & \mathrm{Coker}(c)
\end{array}
$$

是准确的。

让我们证明（i）。由于$u_1$和$v_1$分别与$u$和$v$到$\mathrm{Ker}(a)$和$\mathrm{Ker}(b)$的限制具有相同的图，因此我们有$v_1 \circ u_1 = 0$。然后
$$
\mathrm{Ker}(v_1) = \mathrm{Ker}(b) \cap \mathrm{Ker}(v) = \mathrm{Ker}(b) \cap \mathrm{Im}(u) = \mathrm{Im}(j) \cap \mathrm{Im}(u).
$$
但是，通过命题 1，(i)，如果 $u'$ 是单射的，则$\mathrm{Ker}(v_1) = \mathrm{Im}(j \circ u_1) = \mathrm{Im}(u_1)$。

让我们证明(ii)。由于$u_2$和$v_2$是由$u$和$v$取商得到的，所以显然$v_2 \circ u_2 = 0$。假设 $v$ 是满射；由于 $q$ 和 $p$ 是满射的，因此根据假设和命题 1，(ii)
$$
\begin{align*}
\mathrm{Ker}(v_2) &= q(\mathrm{Ker}(v_2 \circ q)) = q(\mathrm{Ker}(v') + \mathrm{Im}(b)) = q(\mathrm{Ker}(v')) = q(\mathrm{Im}(u')) \\
&= \mathrm{Im}(q \circ u') = \mathrm{Im}(u_2 \circ p) = \mathrm{Im}(u_2).
\end{align*}
$$

最后让我们证明(iii)。对于$x \in \mathrm{Ker}(c)$，存在$y \in B$，使得$v(y) = k(x)$，因为$v$是满射；此外，$v'(b(y)) = c(k(x)) = 0$，因此存在一个*唯一*$t' \in A'$，使得$u'(t') = b(y)$，因为$u'$是单射的。我们现在证明元素$p(t') \in \mathrm{Coker}(a)$是元素$y \in B$*独立*，使得$v(y) = k(x)$。因为如果$y' \in B$是另一个元素，使得$v(y') = k(x)$，则$y' = y + u(z)$，其中$z \in A$；我们证明，如果 $t'' \in A'$ 使得 $u'(t'') = b(y')$ 那么 $t'' = t' + a(z)$；为了
$$
u'(t' + a(z)) = u'(t') + u'(a(z)) = b(y) + b(u(z)) = b(y + u(z)) = b(y').
$$
最后得出$p(t'') = p(t') + p(a(z)) = p(t')$。那么就可以定义集合$d(x) = p(t')$和映射$d : \mathrm{Ker}(c) \to \mathrm{Coker}(a)$。

如果现在$x_1, x_2$是$\mathrm{Ker}(c)$和$x = x_1 + x_2$的元素，我们取$B$的元素$y_1, y_2$，这样$v(y_1) = k(x_1)$和$v(y_2) = k(x_2)$以及选择对于$y \in B$ 元素$y_1 + y_2$；那么直接的就是$d(x) = d(x_1) + d(x_2)$，因而$d$是*同态*。

假设$x = v_1(x')$对于某些$x' \in \mathrm{Ker}(b)$；然后取$y \in B$为元素$j(x')$。作为$b(j(x')) = 0$，可以得出$d(x) = 0$，因而$d \circ v_1 = 0$。相反，假设$d(x) = 0$。在上面的记号中，我们有$t' = a(s)$，其中$s \in A$。在这种情况下，我们有$b(y) = u'(t') = u'(a(s)) = b(u(s))$，或$b(y - u(s)) = 0$。因而，元素$y - u(s)$等于形式$j(n)$，其中$n \in \mathrm{Ker}(b)$，我们有$k(x) = v(y) = v(u(s) + j(n)) = v(j(n)) = k(v_1(n))$；由于 $k$ 是单射，$x = v_1(n)$，这证明序列 (*) 在 $\mathrm{Ker}(c)$ 处精确。

最后，我们有（总是在同一个记号）
$$
u_2(d(x)) = u_2(p(t')) = q(u'(t')) = q(b(y)) = 0
$$
因而$u_2 \circ d = 0$。相反，假设$\mathrm{Coker}(a)$的元素$w = p(t')$使得$u_2(w) = u_2(p(t')) = 0$（其中$t' \in A$）。然后$q(u'(t')) = 0$，因而$u'(t') = b(y)$对于一些$y \in B$；作为$v'(u'(t')) = 0$，我们有$v'(b(y)) = 0$，因而$c(v(y)) = 0$，在其他字$v(y) = k(x)$对于一些$x \in \mathrm{Ker}(c)$，以及定义$w = d(x)$，这表明序列（*）精确于

焦炭（一）。从 (i) 中可以看出，它在 Ker(b) 处精确，在 (ii) 中它在 Coker(b) 处精确，从而完成了 (iii) 的证明。

#### 注 {#ac-i-s1-n4-rem-1 .statement tag=0425}

如果图表（10）中的群都是（对于例，右）模超过环$A$并且同态是A-模同态，很快就可以验证同态d定义在命题2，(iii)也是A-模同态：如果$x \in \mathrm{Ker}(c)$和$a \in A$，并且$y \in B$使得$v(y) = k(x)$，则注足以满足$v(ya) = k(xa)$。

#### 推论 1 {#ac-i-s1-prop-2-cor-1 .statement tag=0426}

假设图表 (10) 是可交换的并且两行是精确的。然后：

(i) 如果 $u'$，a 和 c 是单射的，b 是单射的。
(ii) 如果 v、a 和 c 是满射，则 b 是满射。

断言 (i) 是命题 2 的断言 (i) 的推论：对于$\mathrm{Ker}(a) = 0$ 和$\mathrm{Ker}(c) = 0$，因而$\mathrm{Ker}(b) = 0$。

断言 (ii) 是命题 2 的断言 (ii) 的推论：对于$\mathrm{Coker}(a) = 0$ 和$\mathrm{Coker}(c) = 0$，因而$\mathrm{Coker}(b) = 0$。

#### 推论 2 {#ac-i-s1-prop-2-cor-2 .statement tag=0427}

假设图表 (10) 是可交换的并且两行是精确的。在这些条件下：

(i) 如果 b 是单射且 a 和 v 是满射，则 c 是单射。
(ii) 如果 b 是满射且 c 和 $u'$ 是单射，则 a 是满射。

为了证明 (i) 考虑图表

$$
\begin{array}{ccccc}
u(A) & \xrightarrow{w} & B & \xrightarrow{v} & C \\
a' \downarrow & & b \downarrow & & c \downarrow \\
u'(A') & \xrightarrow{w'} & B' & \xrightarrow{v'} & C'
\end{array}
$$

其中$a'$是映射，与b到$u(A)$的限制相同的图，w和$w'$是典范嵌入；显然，这个图表是可交换的，并且它的行是精确的。此外 $w'$ 是单射的，并且假设 v 是满射的；那么到命题 2 时，(iii) 我们有正合序列

$$
0 = \mathrm{Ker}(b) \longrightarrow \mathrm{Ker}(c) \xrightarrow{d} \mathrm{Coker}(a') = 0
$$

因为 b 是单射且 $a'$ 是满射； 从而$\mathrm{Ker}(c) = 0$。

为了证明 (ii) 考虑图表

$$
\begin{array}{ccccc}
A & \xrightarrow{u} & B & \xrightarrow{w} & v(B) \\
a' \downarrow & & b \downarrow & & c' \downarrow \\
A' & \xrightarrow{w'} & B' & \xrightarrow{\sigma'} & v'(B')
\end{array}
$$

其中，此时$c'$是映射，与c到v(B)的限制具有相同的图，并且w和w'分别与v和v'具有相同的图；这个图表是可交换的并且它的行是精确的。此外，w 是满射的，并且通过假设 u' 是单射的；那么到命题 2 时，(iii) 我们有正合序列

$$
0 = \operatorname{Ker}(c') \xrightarrow{d} \operatorname{Coker}(a) \longrightarrow \operatorname{Coker}(b) = 0
$$

因为 b 是满射而 c' 是单射； 从而焦化器 (a) = 0。

### 习题{#ac-i-s1-exercises}

§ 1](exercises/s1/)参见[习题。
