---
book: top
book_title: General Topology
chapter: VIII
chapter_title: Complex numbers
section: 2
section_title: Angular measure, trigonometric functions
lang: zh
source: top-v-x
pdf_pages: 0111-0121, 0131-0131
extraction: ocr
subsections:
    - "no": 1
      title: THE MULTIPLICATIVE GROUP U
      page: 0
      pdf_page: 111
    - "no": 2
      title: ANGLES
      page: 0
      pdf_page: 113
    - "no": 3
      title: ANGULAR MEASURE
      page: 0
      pdf_page: 114
    - "no": 4
      title: TRIGONOMETRIC FUNCTIONS
      page: 0
      pdf_page: 115
    - "no": 5
      title: ANGULAR SECTORS
      page: 0
      pdf_page: 118
    - "no": 6
      title: CROSSES
      page: 0
      pdf_page: 119
statements: 5
exercises: 4
content_sha256: 8642cb67f64e8088126d2b688b767492ed93071295d9a48c562657cf70c0624a
translated_from: content/en/top/VIII/02_s2_angular_measure_trigonometric_functions.md
translation_method: google
source_content_sha256: 021b6d0e671c54e66a21fa0d56b2ec8b29291d75506ee737a931d924894ce940
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-50f48bb3
glossary_version: 34
glossary_terms_sha256: 04b16820f9dba3b4680905d0567b19901fbdab9dff6ecc91f88ba4645292ab6a
prompt_sha256: 77d1eb2d7fcbd90aea4f1a996022f1b3908ace921dc0bfaa5df62ffc2d1f67a6
---

## 2. 角度测量，三角测量函数

### 1. 乘法群U

#### 定理 1 {#top-viii-s2-thm-1 .statement tag=0C09}

绝对值 1 的复数的乘法拓扑群 $U$ 同构于实数 mod 1 的加法拓扑群 $T$。

$U = S_1$ 是紧连通的，并且具有单位元素 -1 的邻域同胚于 $\mathbf{R}$ 开区间 (章 VI, § 2, no. 4, 命题 5)；因此，定理是章 V, § 2、定理 2 中给出的$T$ 的拓扑刻画的推论。

#### 推论{#top-viii-s2-n1-cor-1 .statement tag=0C0A}

非零复数的乘法群 $C^*$ 同构于群 $\mathbf{R} \times T$ (cf. § 1, no. 3, 命题 1)。

#### 注 {#top-viii-s2-n1-rem-1 .statement tag=0C0B}

群 $C^*$和$\mathbf{R} \times T$的同构意味着域$C$中每个“二项式方程”$z^n = a$都存在根。利用这个事实和$C$的局部兼容性，我们可以获得达朗贝尔高斯的定理的另一个证明（习题2）。

群 $\mathbf{T}$ 中只有*两个*不同的同构到群 $\mathbf{U}$；因为如果$g, g'$是$\mathbf{T}$的两个同构到$\mathbf{U}$，并且如果$h'$是$g'$的逆，那么$h' \circ g$是$\mathbf{T}$的自同构，因此(章VII, , no. 4，命题 6) 我们有相同的$g'(x) = g(x)$或$g'(x) = g(-x)$。我们可以总是假设$g$使得$i$在类 mod 1 of 点$\frac{1}{4}$的$g$下是像；那么，如果 $\varphi$ 表示 $\mathbf{R}$ 的典范同态到 $\mathbf{T}$，则加法群 $\mathbf{R}$ 到乘法群 $\mathbf{U}$ 的每个严格态射都是形式 $x \to g(\varphi(x/a))$，其中$a$ 实数 $\neq 0$ (章 VII, § 2, no. 3, 命题 4)； 注，区间$]-\frac{1}{2}|a|, \frac{1}{2}|a|[$是最大的$\mathbf{R}$的对称开区间，通过严格的态射一对一映射到其像，并且我们有$g(\varphi(\frac{1}{4})) = i$。我们用$x \to e(x)$表示同态$x \to g(\varphi(x))$；因此，$\mathbf{R}$到$\mathbf{U}$的每个严格态射都是形式$x \to e(x/a)$，其中$a \neq 0$。 函数 $e(x)$ 在 $\mathbf{R}$ 上连续，复值，且满足恒等式

(1) $$ |e(x)| = 1, $$
(2) $$ e(x + y) = e(x)e(y), $$

与关系一起

(3) $$ e(0) = 1,\quad e(\frac{1}{4}) = i,\quad e(\frac{1}{2}) = -1,\quad e(\frac{3}{4}) = -i,\quad e(1) = 1. $$

由(1)和(2)可知

(4) $$ e(-x) = \frac{1}{e(x)} = \overline{e(x)}, $$

并从 (2) 和 (3) 得知

$$
e(x + \frac{1}{4}) = ie(x),\quad e(x + \frac{1}{2}) = -e(x),
$$
$$
e(x + \frac{3}{4}) = -ie(x),\quad e(x + 1) = e(x).
$$

因此函数 $e(x)$ 是*周期性的*并且以 1 作为主周期。

#### 注 {#top-viii-s2-n1-rem-2 .statement tag=0C0C}

映射$x + iy \to e^{x}e(y)$是加法群$\mathbf{C}$到乘法群$\mathbf{C}^*$的严格态射，其限制到合适的邻域0是$\mathbf{C}$的局部同构，其中$\mathbf{C}^*$。因而，(章VII, § 2, no. 3)$\mathbf{C}$到$\mathbf{C}^*$的每个严格态射都是形式$x + iy \to e^{\alpha x + \beta y}e(\gamma x + \delta y)$，其中$\alpha, \beta, \gamma, \delta$是任何实数使得$\alpha \delta - \beta \gamma \neq 0$。稍后我们将看到，只有其中一个同态，用$z \to e^z$表示，这样

$$
\lim_{z \to 0} \frac{e^z - 1}{z} = 1;
$$

而这个同态到实轴的限制与$e^x$（从而记号）相同。

### 2. 角度

由于域$\mathbf{R}$是有序的，我们可以通过将$e_1 \wedge e_2$作为正双向量（$e_1, e_2$是典范基的向量）来定向实数平面$\mathbf{R}^2$。在定向实数平面 $\mathbf{R}^2$（在下文中用 $\mathbf{C}$ 标识）中，我们可以得到定义任意对射线 $(\Delta_1, \Delta_2)$ 与原点 o (*) 的角度 $(\Delta_1, \Delta_2)$。所有角度的集合 $\mathfrak{A}$ 的结构为阿贝尔的群（相加写法）定义为

$$
(\Delta_1, \Delta_3) = (\Delta_1, \Delta_2) + (\Delta_2, \Delta_3),
$$

因而，特别是$(\Delta_1, \Delta_1) = 0$和$(\Delta_2, \Delta_1) = - (\Delta_1, \Delta_2)$。

平角$\varpi$为$\mathfrak{A}$中方程$2\theta = 0$的解$\neq 0$；它是负实半轴与正实半轴所成的角度。

如果 $z$ 是任何非零复数，则 $z$ 的振幅（或参数）（用 $\mathrm{Am}(z)$ 表示）是原点为 o 穿过 $z$ 的射线与正实半轴所成的角度。 映射 $z \to \mathrm{Am}(z)$ 是乘法群 $\mathbf{C}^*$ 的同态到加法群 $\mathfrak{A}$，因此我们有

$$
\mathrm{Am}(zz') = \mathrm{Am}(z) + \mathrm{Am}(z') \quad \text{and} \quad \mathrm{Am}(\overline{z}) = \mathrm{Am}(z^{-1}) = - \mathrm{Am}(z).
$$

角$\delta = \mathrm{Am}(i)$称为正直角；它是方程$2\theta = \varpi$中$\mathfrak{A}$中的解之一，另一个是$- \delta = \delta + \varpi$。

同态$z \to \mathrm{Am}(z)$，仅限于$\mathbf{C}^*$的子群$\mathbf{U}$，是$\mathbf{U}$的群结构的同构到$\mathfrak{A} \ (***)$的同构；如果我们

(*) We know from 代数 that 等价关系 is defined on 集合 of all 右 $(\Delta_1, \Delta_2)$ of rays with origin o by considering two 右 $(\Delta_1, \Delta_2)$ and $(\Delta'_1, \Delta'_2)$ as equivalent if there exists a rotation which 变换 $\Delta_1$ into $\Delta'_1$和$\Delta_2$同时转换为$\Delta'_2$； 右$(\Delta_1, \Delta_2)$的角度，或$\Delta_2$与$\Delta_1$所成的角度，则乘以对$(\Delta_1, \Delta_2)$的定义等价类。

(**) This is because every ray with origin o meets the circle $S_1$, since the field $\mathbf{R}$ is Pythagorean.

用这个$\mathbf{U}$的同构到迁移拓扑到群$\mathfrak{A}$，后者群就变成了紧拓扑群，而$\mathbf{C}^*$的映射$z \to \mathrm{Am}\,(z)$到了$\mathfrak{A}$ 是拓扑群 $\mathbf{C}^*$ 到拓扑群 $\mathfrak{A}$ 的严格态射。

让我们用$\mathfrak{A}$到$\mathbf{U}$的$\theta \to f(\theta)$同构来表示，它是$\mathbf{U}$到$\mathfrak{A}$的同构$z \to \mathrm{Am}\,(z)$的逆。 定义$\Re(f(\theta))$表示为$\cos \theta$，称为角度$\theta$的余弦； $\Im(f(\theta))$用$\sin \theta$表示，称为角度$\theta$的正弦。这些函数在拓扑群$\mathfrak{A}$上是连续的，满足下面的关系（*loc.cit.*），它们是上面定义的直接的推论：

$$
\begin{align*}
\cos 0 &= 1, & \sin 0 &= 0, & \cos \varpi &= -1, & \sin \varpi &= 0, \\
\cos(-\theta) &= \cos \theta, & \sin(-\theta) &= -\sin \theta, \\
\cos(\theta + \theta') &= \cos \theta \cos \theta' - \sin \theta \sin \theta', \\
\sin(\theta + \theta') &= \sin \theta \cos \theta' + \sin \theta' \cos \theta, \\
\cos^2 \theta + \sin^2 \theta &= 1.
\end{align*}
$$

通过定义，角度$\theta \in \mathfrak{A}$的正切被定义为，每当$\cos \theta \neq 0$时，为$\sin \theta / \cos \theta$（*loc.cit.*）并用$\tan \theta$表示；它是一个连续的函数，通过对角$\delta$和$-\delta$取值$\infty$，扩展连续到$\tilde{\mathbf{R}}$（章VI, § 3, no. 4）。我们有$\tan (\theta + \varpi) = \tan \theta$。 $\theta$ 的余切，记为 $\cot \theta$，即 $\tilde{\mathbf{R}}$ 的元素等于 $1 / \tan \theta$。

注，如果$\mathrm{Am}\,(z) = \theta$，我们就有$z = |z| (\cos \theta + i \sin \theta)$；这个表达式称为复数 $z \neq 0$ 的三角形式。

### 3. 角度测量

通过no. 1的定理1，角的拓扑群$\mathfrak{A}$同构于$\mathbf{T}$。 $\mathbf{R}$到$\mathfrak{A}$的每个严格态射可以通过将$\mathbf{U}$的同构$z \to \mathrm{Am}\,(z)$组合到$\mathfrak{A}$以及$\mathbf{R}$的严格态射到$\mathbf{U}$来获得；如果我们把$\hat{x}(x) = \mathrm{Am}\,(e(x))$，$\mathbf{R}$的每个严格的态射放到$\mathfrak{A}$上，因此都是形式$x \to g(x/a)$（$a \neq 0$）。给定实数$a > 0$，一劳永逸地固定，每个角度$\theta$对应，由同态$x \to \hat{x}(x/a)$，到实数mod$a$的类（即元素 $\mathbf{Z}/a\mathbf{Z}$)，称为$\theta$相对于基$a$的度量；滥用语言，这个类中的每个实数也被称为$\theta$的度量；角度 $\hat{x}(x/a)$ 称为尺寸为 $x$ 的角度（相对于基 $a$。如果 $x$ 是 $\theta$ 的尺寸，$x'$ 是 $\theta'$ 的尺寸（相对于相同的基），那么$x + x'$ 是$\theta + \theta'$ 的度量，$-x$ 是$\theta$ 的度量。角度的主要度量（相对于基 $a$）是其位于区间$[0, a[$ 中的度量之一。

选择基 $a$。 我们总是将自己限制在基$a > 1$。 对于每个 $a > 1$ 对应都有一个角度 $\omega = \frac{\pi}{a}$，其主度量为 1，称为相对于基 $a$ 的角度度量的单位；相反，对于每个角度$\omega \neq 0$，都有对应一个唯一的$a > 1$，使得$\frac{\pi}{a} = \omega$，从而完全了解角度测量确定基$a > 1$的单位。

在数值计算中，通常取$a = 360$或$a = 400$；角度测量的相应的单位称为次数（$a = 360$）或等级（$a = 400$）。

在数学分析中，实际上在所有不涉及数值计算的数学分支中，基$a$由条件定义

$$
\lim_{x \to 0} \frac{e(x/a) - 1}{x} = i
$$

被普遍使用；这个基用$2\pi$表示。角度度量的相应的单位称为弧度，度量称为弧度度量；对于前面提到的复杂的$z$，我们有定义或$e^z$，对于所有$x \in \mathbf{R}$，我们有$e(x) = e^{2\pi ix}$。

一旦选择了基$a$，当人们谈到角度时，通常意味着该角度相对于基$a$的测量；这种语言的滥用没有缺点，只要（不涉及数值计算时总是如此）基$a$始终保持固定，并且只要记住两个实数是全等模$a$对应到相同的角度。

对于例，通常理解的复数$z \neq 0$的幅度是该角度的弧度度量，由取决于所考虑的问题的约定确定；一旦制定了这些约定，所选择的幅度测量值就用 Am $(z)$ 表示。

### 4. 三角函数函数

如果我们将函数$\cos \theta, \sin \theta, \tan \theta, \cot \theta$（在$\mathscr{A}$上定义）与$\mathbf{R}$的同态$x \to \frac{\pi}{a}(x/a)$组合到$\mathscr{A}$，函数

$$
\cos \left( \frac{x}{a} \right), \quad \sin \left( \frac{x}{a} \right), \quad \tan \left( \frac{x}{a} \right), \quad \cot \left( \frac{x}{a} \right)
$$

这样得到的分别称为*数* $x$相对于基$a$的余弦、正弦、正切、余切，记作$\cos_a x$、$\sin_a x$、$\tan_a x$、$\cot_a x$。 映射$x \to \cos_a x + i \sin_a x$是$\theta \to \cos \theta + i \sin \theta$和$x \to \tilde{\sigma}(x/a)$的合成，因此，从no. 2中$\cos \theta$和$\sin \theta$的定义，我们有恒等式

$$
e\left( \frac{x}{a} \right) = \cos_a x + i \sin_a x,
$$

这相当于

$$
\cos_a x = \Re \left( e\left( \frac{x}{a} \right) \right), \qquad \sin_a x = \Im \left( e\left( \frac{x}{a} \right) \right),
$$

并且，通过(4)，等价于

$$
\cos_a x = \frac{1}{2} \left( e\left( \frac{x}{a} \right) + e\left( -\frac{x}{a} \right) \right), \qquad \sin_a x = \frac{1}{2i} \left( e\left( \frac{x}{a} \right) - e\left( -\frac{x}{a} \right) \right).
$$

因此身份

$$
\cos_b x = \cos_a \left( \frac{ax}{b} \right), \qquad \sin_b x = \sin_a \left( \frac{ax}{b} \right).
$$

唯一出现在不涉及数值计算的数学分支中的三角函数函数是与上述基$2\pi$相关的三角函数；这些函数简单地用$\cos x$、$\sin x$、$\tan x$、$\cot x$来表示，代替$\cos_{2\pi} x$、$\sin_{2\pi} x$、$\tan_{2\pi} x$、$\cot_{2\pi} x$。为了数值计算的目的，三角函数函数、相应的至基、$a = 360$和$a = 400$有表； 公式 (6) 允许我们推导出三角函数函数相对于任何其他基的值。

前面回忆的*角度*的余弦和正弦之间的关系显然会在测量这些角度的*数*的余弦和正弦之间产生相同的关系；特别是，我们有

$$
\begin{align*}
\cos_a (x + y) &= \cos_a x \cos_a y - \sin_a x \sin_a y, \\
\sin_a (x + y) &= \sin_a x \cos_a y + \sin_a y \cos_a x, \\
\cos_a (-x) &= \cos_a x, \qquad \sin_a (-x) = -\sin_a x, \\
&\cos_a^2 x + \sin_a^2 x = 1.
\end{align*}
$$

函数 $\cos_a x$和$\sin_a x$在$\mathbf{R}$上连续，并且以周期$a$为周期；此外，$a$是这些函数的*主要周期*，因为关系$\cos_a x = \cos_a y$意味着$\sin_a x = \sin_a y$或

$$
\sin_a x = -\sin_a y,\quad \text{i.e.,}
$$

$$
e\left(\frac{x}{a}\right) = e\left(\frac{y}{a}\right)\quad \text{or}\quad e\left(\frac{x}{a}\right) = e\left(-\frac{y}{a}\right),
$$

所以无论是

$$
x \equiv y \pmod{a}\quad \text{or}\quad x \equiv -y \pmod{a};
$$

和类似地

$$
\sin_a x = \sin_a y
$$

相当于 $x \equiv y \pmod{a}$ 或 $x + y \equiv \frac{1}{2} a \pmod{a}$。

由此可见，$\cos_a x$在区间$[0, \frac{1}{2} a]$中绝不会两次采用相同的值；因此，当限制于该区间时，它是该区间到区间 $[-1, +1]$ 的*双射的* 映射。由于$\cos_a 0 = 1$和$\cos_a (\frac{1}{2} a) = -1$，$x \to \cos_a x$是$[0, \frac{1}{2} a]$*到*$[-1, 1]$的*严格递减*映射（章IV, § 2, no. 6、定理5和注）。我们有$\cos_a x = 0$对应$x = a/4$，$\cos_a x > 0$对应$0 \leq x < a/4$，$\cos_a x < 0$对应$a/4 < x \leq a/2$。由于$\cos_a (-x) = \cos_a x$，我们可以推断出$\cos_a x$如何在区间$[- \frac{1}{2} a, 0]$中变化，从而在整个$\mathbf{R}$中按周期性变化（图8）。由于$\sin_a x = -\cos_a(x + a/4)$，我们还可以推断出$\sin_a x$在$\mathbf{R}$中如何变化（图8）。

![显示 y = sin_a x 和 y = cos_a x 的图表](https://i.imgur.com/3Q5z5QG.png)

图 8.

函数 $\tan_a x$ 是 $\mathbf{R}$ 到 $\tilde{\mathbf{R}}$ 的连续映射； 值$\frac{1}{4} a + \frac{1}{2} k a \ (k \in \mathbf{Z})$需要值$\infty$。由于$\frac{1}{2} a$是$\tan_2 x$的周期，因此它是一个*主要周期*。在区间$[0, \frac{1}{4} a]$，$\sin_a x$从0增加到1，$\cos_a x$从1减少到0，因此$\tan_a x$在$[0, \frac{1}{4} a[$和映射这个区间到$[0, +\infty[$是*严格递增的*；由此可见，区间内 $\tan_a x$ 是严格递增的

![显示标记为 y 和 x 的曲线的图表，轴标记为 -a/4、0、a/4、a/2、3a/4](../images/complex_numbers_9.png)

图 9.

]— $\frac{1}{4} a, + \frac{1}{4} a$[。是这个区间在 $\mathbf{R}$ 上的同胚（图 9）。

### 5. 扇形角

给定两条不同的闭射线 $\Delta_1, \Delta_2$，原点为 o，令 $x$ 为角度 $(\widehat{\Delta_1, \Delta_2})$ 的主要度量（相对于基 $a$，一劳永逸地选择）。原点为 o 的闭（或开）射线 $\Delta$ 的并使得角度 $(\widehat{\Delta_1, \Delta})$ 的主度量 $y$ 满足 $0 \leq y \leq x$（或 $0 < y < x$）是具有原点 $\Delta_1$ 和端点的闭（或开）角扇区 S $\Delta_2$，如代数中所定义。因为通过旋转，我们总是可以约化到 S 不包含穿过点的射线的情况 — 1。如果 $\alpha$ 和 $\beta$ 分别是 $\Delta_1$ 和 $\Delta_2$ 分别与正实半轴所成的角度，则闭角扇区 S 是闭半线 $\Delta$ 的并与正实半轴形成角度 $\theta$，使得 $\tan \frac{1}{2} \alpha \leq \tan \frac{1}{2} \theta \leq \tan \frac{1}{2} \beta$。现在，如果 $u, v, t$ 分别是位于区间 ]— $\frac{1}{2} a, + \frac{1}{2} a$[ 中的 $\alpha, \beta, \theta$ 的度量，则这些不等式等价于 $\tan_a \frac{1}{2} u \leq \tan_a \frac{1}{2} t \leq \tan_a \frac{1}{2} v$；并且由于$\tan_a x$在区间]—$\frac{1}{4} a, + \frac{1}{4} a$[中是递增函数，因此它们也等价于$u \leq t \leq v$，或$0 \leq t - u \leq v - u$；从$x = v - u, y = t - u$开始，对于闭角扇形，结果得到证明，对于开角扇形，证明类似。

闭角扇区是$\mathbf{R}^2$中的闭角集合，同原点、同端点的开角扇区是其在$\mathbf{R}^2$的内部

图 10.

（章VI, § 2, no. 3、命题3）。角度$(\widehat{\Delta_1, \Delta_2})$，主尺寸为$x$，称为扇形S的角度；如果 $x < \frac{1}{2} a$，则 S 被称为凸形；如果 $x = \frac{1}{2} a$，则 S 被称为平面（或闭合半平面）；如果$x > \frac{1}{2} a$，则可重入。如果$x < \frac{1}{4} a$，凸角扇区是锐角，如果$x = \frac{1}{4} a$，则为右凸角，如果$x > \frac{1}{4} a$，则为钝角。扇形 S 的平分线是射线 $\Delta$，它与 $\Delta_1$ 形成角度 $y = \frac{1}{2} x$。

两条不同的闭合射线 $\Delta_1, \Delta_2$ 确定两个闭合角扇区；他们的并是真正的平面$\mathbf{R}^2$，他们的交是$\Delta_1 \cup \Delta_2$。

### 6. 叉积

我们还在对的代数叉积中定义了二维向量空间超过极大有序域的线（*）。这个定义尤其适用于真实平面$\mathbf{R}^2$。所有叉积中的集合 $\mathscr{A}_0$ 有阿贝尔的群中的结构 （相加地写）定义为

$$
(\overline{D_1, D_3}) = (\overline{D_1, D_2}) + (\overline{D_2, D_3})
$$

因此，特别是$(\overline{D_1, D_1}) = 0$和$(\overline{D_2, D_1}) = - (\overline{D_1, D_2})$。

右叉积$\delta_0$是$\mathscr{A}_0$中等式$2\theta = 0$的解$\neq 0$；虚轴与实轴成叉积。

(*) 我们记得，如果存在变换$D_1$的直接相似性，则等价关系是在$(D_1, D_2)$线的所有非各向同性对的集合上定义的，通过考虑线$(D_1, D_2)$和$(D'_1, D'_2)$的两个对是等效的同时进入$D'_1$和$D_2$进入$D'_2$； 对 $(D_1, D_2)$ 的叉积则为对的等价类。

我们通过将对应设为射线 $\Delta$ 与正实半轴所成的角度，将群 $\mathfrak{A}$ 的角度定义典范同态 $\varphi$ 置于叉积的群 $\mathfrak{A}_0$ 上，直线 D 包含 $\Delta$ 与实轴所成的叉积。 叉积$\theta_0$是两个角$\theta$和$\theta + \omega$的$\varphi$下的像；因此$\mathfrak{A}_0$同构于$\mathfrak{A}$除以子群$\{0, \omega\}$的商。如果我们通过与$\varphi$相关的双射同态将商群$\mathfrak{A}/\{0, \omega\}$从迁移到$\mathfrak{A}_0$拓扑，则$\mathfrak{A}_0$成为紧拓扑群，$\varphi$成为严格拓扑$\mathfrak{A}$ 的态射到$\mathfrak{A}_0$。

如果我们将$\mathfrak{A}$的同态$\varphi$组合到$\mathfrak{A}_0$上，并将$\mathbf{R}$的同态$x \to \tilde{\sigma}(x/a)$组合到$\mathfrak{A}$上，我们有$\mathbf{R}$的同态$x \to \tilde{\sigma}_0(x/a)$到$\mathfrak{A}_0$；每叉积 $\theta_0 \in \mathfrak{A}_0$ 对应，在此同态下，到实数 mod $\frac{1}{2} a$的类，称为叉积 $\theta_0$的度量（相对于基 $a$);滥用语言，这个类中的每个数被称为$\theta_0$的一个小节，而属于到间隔$[0, \frac{1}{2} a[$的那个被称为$\theta_0$的主要小节； 叉积 $\tilde{\sigma}_0(x/a)$ 是 $x$ 的叉积。 $\theta_0$ 的每个度量也是两个角 $\theta, \theta + \omega$ 之一的度量，其中像在同态 $\varphi$ 下是 $\theta_0$。

再次强调，一旦选择了基$a$，当我们谈到叉积时，我们通常通过滥用语言来表示叉积相对于基$a$的度量。

#### 注 {#top-viii-s2-n6-rem-1 .statement tag=0C0D}

我们可以将 $\mathbf{C}^*$ 的定义同态乘以映射到 $\mathfrak{A}_0$，每个复数 $z \neq 0$ 到叉积，即通过 o 和 $z$ 的直线与实轴的关系。显然，这个同态是$\varphi$的合成和$\mathbf{C}^*$的同态$z \to \mathrm{Am}\,(z)$到$\mathfrak{A}$；因此，它是拓扑群$\mathbf{C}^*$到拓扑群$\mathfrak{A}_0$的严格态射，并且相关联的双射同态是商群$\mathbf{C}^*/\mathbf{R}^*$的同构 $\mathfrak{A}_0$。

我们知道，如果 D 表示与实轴构成叉积 $\theta_0$ 的直线，且$(a, b)$ 是 D 的方向比对，则叉积 $\theta_0$（记为 $\tan\,\theta_0$）的正切为元素 $b/a$ $\tilde{\mathbf{R}}$（$a = 0$则为$= \infty$），也称为直线D的斜率。如果$\theta$和$\theta + \omega$是$\varphi$下的像为$\theta_0$的两个角，则有$\tan\,\theta_0 = \tan\,\theta = \tan(\theta + \omega)$。

映射$\theta_0 \to \tan\,\theta_0$是$\mathfrak{A}_0$到$\tilde{\mathbf{R}}$的同胚，因为拓扑空间$\mathbf{C}^*/\mathbf{R}^*$只是实射影线$\mathbf{P}_1$，并且从章VI, § 3, no. 3，映射一条线（视为$\mathbf{P}_1$的点）其斜率是$\mathbf{P}_1$到$\tilde{\mathbf{R}}$的同胚。如果现在我们通过映射$\theta_0 \to \tan\,\theta_0$将$\mathfrak{A}_0$的迁移到$\tilde{\mathbf{R}}$群结构，我们就定义了阿贝尔的拓扑群的$\tilde{\mathbf{R}}$结构，其中每当$t_1, t_2$属于到$\mathbf{R}$和$t_1 t_2 \neq 1$时，两个元素$t_1, t_2$中的乘积是$\frac{t_1 + t_2}{1 - t_1 t_2}$；对于不存在满足的对$(t_1, t_2)$，条件、$t_1$和$t_2$的乘积是通过将函数$\frac{x + y}{1 - xy}$连续延伸到$\tilde{\mathbf{R}} \times \tilde{\mathbf{R}}$获得的，并且仍然表示为$\frac{t_1 + t_2}{1 - t_1 t_2}$。

### 习题 {#top-viii-s2-exercises}

参见[习题为 § 2](exercises/s2/)。
