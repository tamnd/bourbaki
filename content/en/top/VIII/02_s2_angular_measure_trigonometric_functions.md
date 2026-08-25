---
book: top
book_title: General Topology
chapter: VIII
chapter_title: Complex numbers
section: 2
section_title: Angular measure, trigonometric functions
lang: en
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
content_sha256: a5d3b8b9967c53f54bbfeea4b7d7a20401592cd9d0f1108eb802855c2c0273b1
---

## 2. ANGULAR MEASURE, TRIGONOMETRIC FUNCTIONS

### 1. THE MULTIPLICATIVE GROUP U

#### Theorem 1 {#top-viii-s2-thm-1 .statement}

The (multiplicative, topological group $U$ of complex numbers of absolute value 1 is isomorphic to the (additive, topological group $T$ of real numbers mod 1.

$U = S_1$ is compact and connected, and has a neighbourhood of the identity element -1 homeomorphic to an open interval of $\mathbf{R}$ (Chapter VI, § 2, no. 4, Proposition 5); the theorem is therefore a consequence of the topological characterization of $T$ given in Chapter V, § 2, Theorem 2.

#### Corollary {#top-viii-s2-n1-cor-1 .statement}

The multiplicative group $C^*$ of non-zero complex numbers is isomorphic to the group $\mathbf{R} \times T$ (cf. § 1, no. 3, Proposition 1).

#### Remark {#top-viii-s2-n1-rem-1 .statement}

The isomorphism of the groups $C^*$ and $\mathbf{R} \times T$ implies the existence of roots of every "binomial equation" $z^n = a$ in the field $C$. Using this fact and the local compatibility of $C$, we can obtain another proof of the theorem of d'Alembert-Gauss (Exercise 2).

(1) $$ |e(x)| = 1, $$
(2) $$ e(x + y) = e(x)e(y), $$

together with the relations

(3) $$ e(0) = 1,\quad e(\frac{1}{4}) = i,\quad e(\frac{1}{2}) = -1,\quad e(\frac{3}{4}) = -i,\quad e(1) = 1. $$

From (1) and (2) it follows that

(4) $$ e(-x) = \frac{1}{e(x)} = \overline{e(x)}, $$

and from (2) and (3) that

$$
e(x + \frac{1}{4}) = ie(x),\quad e(x + \frac{1}{2}) = -e(x),
$$
$$
e(x + \frac{3}{4}) = -ie(x),\quad e(x + 1) = e(x).
$$

Thus the function $e(x)$ is *periodic* and has 1 as a principal period.

#### Remark {#top-viii-s2-n1-rem-2 .statement}

The mapping $x + iy \to e^{x}e(y)$ is a strict morphism of the additive group $\mathbf{C}$ onto the multiplicative group $\mathbf{C}^*$, and its restriction to a suitable neighbourhood of 0 is a local isomorphism of $\mathbf{C}$ with $\mathbf{C}^*$. Consequently (Chapter VII, § 2, no. 3) every strict morphism of $\mathbf{C}$ onto $\mathbf{C}^*$ is of the form $x + iy \to e^{\alpha x + \beta y}e(\gamma x + \delta y)$, where $\alpha, \beta, \gamma, \delta$ are any real numbers such that $\alpha \delta - \beta \gamma \neq 0$. We shall see later that there is just one of these homomorphisms, denoted by $z \to e^z$, such that

$$
\lim_{z \to 0} \frac{e^z - 1}{z} = 1;
$$

and the restriction of this homomorphism to the real axis is the same as $e^x$ (whence the notation).

### 2. ANGLES

Since the field $\mathbf{R}$ is ordered, we may orient the real number plane $\mathbf{R}^2$ by taking $e_1 \wedge e_2$ as positive bivector ($e_1, e_2$ being the vectors of the canonical basis). In the oriented real number plane $\mathbf{R}^2$ (identified with $\mathbf{C}$ in what follows) we can then define the angle $(\Delta_1, \Delta_2)$ of an arbitrary pair of rays $(\Delta_1, \Delta_2)$ with origin o (*). The set $\mathfrak{A}$ of all angles has the structure of an abelian group (written additively) defined by

$$
(\Delta_1, \Delta_3) = (\Delta_1, \Delta_2) + (\Delta_2, \Delta_3),
$$

so that, in particular, $(\Delta_1, \Delta_1) = 0$ and $(\Delta_2, \Delta_1) = - (\Delta_1, \Delta_2)$.

The flat angle $\varpi$ is the solution $\neq 0$ of the equation $2\theta = 0$ in $\mathfrak{A}$; it is the angle which the negative real semi-axis makes with the positive real semi-axis.

If $z$ is any non-zero complex number, the amplitude (or argument) of $z$, denoted by $\mathrm{Am}(z)$, is the angle which the ray through $z$ with origin o makes with the positive real semi-axis. The mapping $z \to \mathrm{Am}(z)$ is a homomorphism of the multiplicative group $\mathbf{C}^*$ onto the additive group $\mathfrak{A}$, and therefore we have

$$
\mathrm{Am}(zz') = \mathrm{Am}(z) + \mathrm{Am}(z') \quad \text{and} \quad \mathrm{Am}(\overline{z}) = \mathrm{Am}(z^{-1}) = - \mathrm{Am}(z).
$$

The angle $\delta = \mathrm{Am}(i)$ is called the positive right angle; it is one of the solutions in $\mathfrak{A}$ of the equation $2\theta = \varpi$, the other one being $- \delta = \delta + \varpi$.

The homomorphism $z \to \mathrm{Am}(z)$, restricted to the subgroup $\mathbf{U}$ of $\mathbf{C}^*$, is an isomorphism of the group structure of $\mathbf{U}$ onto that of $\mathfrak{A} \ (***)$; if we

(*) We know from algebra that an equivalence relation is defined on the set of all pairs $(\Delta_1, \Delta_2)$ of rays with origin o by considering two pairs $(\Delta_1, \Delta_2)$ and $(\Delta'_1, \Delta'_2)$ as equivalent if there exists a rotation which transforms $\Delta_1$ into $\Delta'_1$ and $\Delta_2$ into $\Delta'_2$ simultaneously; the angle of the pair $(\Delta_1, \Delta_2)$, or the angle $\Delta_2$ makes with $\Delta_1$, is then by definition the equivalence class of the pair $(\Delta_1, \Delta_2)$.

(**) This is because every ray with origin o meets the circle $S_1$, since the field $\mathbf{R}$ is Pythagorean.

use this isomorphism to transport the topology of $\mathbf{U}$ to the group $\mathfrak{A}$, the latter group becomes a compact topological group, and the mapping $z \to \mathrm{Am}\,(z)$ of $\mathbf{C}^*$ onto $\mathfrak{A}$ is a strict morphism of the topological group $\mathbf{C}^*$ onto the topological group $\mathfrak{A}$.

Let us denote by $\theta \to f(\theta)$ the isomorphism of $\mathfrak{A}$ onto $\mathbf{U}$ which is the inverse of the isomorphism $z \to \mathrm{Am}\,(z)$ of $\mathbf{U}$ onto $\mathfrak{A}$. By definition $\Re(f(\theta))$ is denoted by $\cos \theta$ and is called the cosine of the angle $\theta$; $\Im(f(\theta))$ is denoted by $\sin \theta$ and is called the sine of the angle $\theta$. These functions are continuous on the topological group $\mathfrak{A}$, and satisfy the following relations (*loc. cit.*), which are immediate consequences of the definitions above:

$$
\begin{align*}
\cos 0 &= 1, & \sin 0 &= 0, & \cos \varpi &= -1, & \sin \varpi &= 0, \\
\cos(-\theta) &= \cos \theta, & \sin(-\theta) &= -\sin \theta, \\
\cos(\theta + \theta') &= \cos \theta \cos \theta' - \sin \theta \sin \theta', \\
\sin(\theta + \theta') &= \sin \theta \cos \theta' + \sin \theta' \cos \theta, \\
\cos^2 \theta + \sin^2 \theta &= 1.
\end{align*}
$$

By definition, the tangent of an angle $\theta \in \mathfrak{A}$ is defined, whenever $\cos \theta \neq 0$, to be $\sin \theta / \cos \theta$ (*loc. cit.*) and is denoted by $\tan \theta$; it is a continuous function, which extends by continuity to $\tilde{\mathbf{R}}$ (Chapter VI, § 3, no. 4) by taking the value $\infty$ for the angles $\delta$ and $-\delta$. We have $\tan (\theta + \varpi) = \tan \theta$. The cotangent of $\theta$, denoted by $\cot \theta$, is the element of $\tilde{\mathbf{R}}$ equal to $1 / \tan \theta$.

Note that, if $\mathrm{Am}\,(z) = \theta$, we have $z = |z| (\cos \theta + i \sin \theta)$; this expression is called the trigonometric form of the complex number $z \neq 0$.

### 3. ANGULAR MEASURE

By Theorem 1 of no. 1, the topological group $\mathfrak{A}$ of angles is isomorphic to $\mathbf{T}$. Every strict morphism of $\mathbf{R}$ onto $\mathfrak{A}$ can be obtained by composing the isomorphism $z \to \mathrm{Am}\,(z)$ of $\mathbf{U}$ onto $\mathfrak{A}$ with a strict morphism of $\mathbf{R}$ onto $\mathbf{U}$; if we put $\hat{x}(x) = \mathrm{Am}\,(e(x))$, every strict morphism of $\mathbf{R}$ onto $\mathfrak{A}$ is therefore of the form $x \to g(x/a)$ ($a \neq 0$). Given a real number $a > 0$, fixed once and for all, every angle $\theta$ corresponds, by the homomorphism $x \to \hat{x}(x/a)$, to a class of real numbers mod $a$ (i.e., an element of $\mathbf{Z}/a\mathbf{Z}$) which is called the measure of $\theta$ relative to the base $a$; by abuse of language, every real number in this class is also called a measure of $\theta$; the angle $\hat{x}(x/a)$ is called the angle with measure $x$ (relative to the base $a$. If $x$ is a measure of $\theta$ and $x'$ a measure of $\theta'$ (relative to the same base) then $x + x'$ is a measure of $\theta + \theta'$, and $-x$ is a measure of $\theta$. The principal measure of an angle (relative to the base $a$) is that one of its measures which lies in the interval $[0, a[$.

Choice of a base $a$. We restrict ourselves always to bases $a > 1$. To each $a > 1$ corresponds an angle $\omega = \frac{\pi}{a}$ whose principal measure is 1, and which is called the unit of angular measure relative to the base $a$; conversely, to each angle $\omega \neq 0$ there corresponds a unique $a > 1$ such that $\frac{\pi}{a} = \omega$, so that knowledge of the unit of angular measure determines the base $a > 1$ entirely.

In numerical calculations one usually takes either $a = 360$ or $a = 400$; the corresponding unit of angular measure is called the degree ($a = 360$) or the grade ($a = 400$).

In analysis, and indeed in all branches of mathematics where numerical calculation is not involved, the base $a$ defined by the condition

$$
\lim_{x \to 0} \frac{e(x/a) - 1}{x} = i
$$

is universally used; this base is denoted by $2\pi$. The corresponding unit of angular measure is called a radian, and the measure is called radian measure; with the definition of $e^z$ for complex $z$ mentioned earlier, we have $e(x) = e^{2\pi ix}$ for all $x \in \mathbf{R}$.

Once the base $a$ has been chosen, when one speaks of an angle one usually means a measure of this angle relative to the base $a$; this abuse of language has no drawback provided (as is always the case when numerical calculations are not involved) the base $a$ remains fixed throughout, and provided that one remembers that two real numbers which are congruent mod $a$ correspond to the same angle.

For example, what is usually understood by the amplitude of a complex number $z \neq 0$ is a radian measure of this angle, determined by conventions which will depend on the question under consideration; once these conventions have been made, the measure of the amplitude thus chosen is denoted by Am $(z)$.

### 4. TRIGONOMETRIC FUNCTIONS

If we compose the functions $\cos \theta, \sin \theta, \tan \theta, \cot \theta$ (defined on $\mathcal{A}$) with the homomorphism $x \to \frac{\pi}{a}(x/a)$ of $\mathbf{R}$ onto $\mathcal{A}$, the functions

$$
\cos \left( \frac{x}{a} \right), \quad \sin \left( \frac{x}{a} \right), \quad \tan \left( \frac{x}{a} \right), \quad \cot \left( \frac{x}{a} \right)
$$

so obtained are called respectively the cosine, sine, tangent and cotangent of the *number* $x$ relative to the base $a$, and are written $\cos_a x$, $\sin_a x$, $\tan_a x$, $\cot_a x$. The mapping $x \to \cos_a x + i \sin_a x$ is the composition of $\theta \to \cos \theta + i \sin \theta$ and $x \to \tilde{\sigma}(x/a)$, so that, from the definition of $\cos \theta$ and $\sin \theta$ in no. 2, we have the identity

$$
e\left( \frac{x}{a} \right) = \cos_a x + i \sin_a x,
$$

which is equivalent to

$$
\cos_a x = \Re \left( e\left( \frac{x}{a} \right) \right), \qquad \sin_a x = \Im \left( e\left( \frac{x}{a} \right) \right),
$$

and also, by (4), equivalent to

$$
\cos_a x = \frac{1}{2} \left( e\left( \frac{x}{a} \right) + e\left( -\frac{x}{a} \right) \right), \qquad \sin_a x = \frac{1}{2i} \left( e\left( \frac{x}{a} \right) - e\left( -\frac{x}{a} \right) \right).
$$

Hence the identities

$$
\cos_b x = \cos_a \left( \frac{ax}{b} \right), \qquad \sin_b x = \sin_a \left( \frac{ax}{b} \right).
$$

The only trigonometric functions which arise in branches of mathematics where numerical calculation is not involved are those relative to the base $2\pi$ referred to above; these functions are denoted simply by $\cos x$, $\sin x$, $\tan x$, $\cot x$ in place of $\cos_{2\pi} x$, $\sin_{2\pi} x$, $\tan_{2\pi} x$, $\cot_{2\pi} x$. For the purposes of numerical calculation, there are tables of the trigonometric functions corresponding to the bases $a = 360$ and $a = 400$; and the formulae (6) allow us to deduce the values of the trigonometric functions relative to any other base.

The relations recalled earlier between the cosines and sines of *angles* evidently give rise to the same relations between the cosines and the sines of the *numbers* which measure these angles; in particular, we have

$$
\begin{align*}
\cos_a (x + y) &= \cos_a x \cos_a y - \sin_a x \sin_a y, \\
\sin_a (x + y) &= \sin_a x \cos_a y + \sin_a y \cos_a x, \\
\cos_a (-x) &= \cos_a x, \qquad \sin_a (-x) = -\sin_a x, \\
&\cos_a^2 x + \sin_a^2 x = 1.
\end{align*}
$$

The functions $\cos_a x$ and $\sin_a x$ are continuous on $\mathbf{R}$, and are periodic with period $a$; moreover, $a$ is a *principal period* of these functions, for the relation $\cos_a x = \cos_a y$ implies that either $\sin_a x = \sin_a y$ or

$$
\sin_a x = -\sin_a y,\quad \text{i.e.,}
$$

$$
e\left(\frac{x}{a}\right) = e\left(\frac{y}{a}\right)\quad \text{or}\quad e\left(\frac{x}{a}\right) = e\left(-\frac{y}{a}\right),
$$

so that either

$$
x \equiv y \pmod{a}\quad \text{or}\quad x \equiv -y \pmod{a};
$$

and similarly

$$
\sin_a x = \sin_a y
$$

is equivalent to either $x \equiv y \pmod{a}$ or $x + y \equiv \frac{1}{2} a \pmod{a}$.

It follows from this that $\cos_a x$ never takes the same value twice in the interval $[0, \frac{1}{2} a]$; hence, when restricted to this interval, it is a *bijective* mapping of this interval onto the interval $[-1, +1]$. Since $\cos_a 0 = 1$ and $\cos_a (\frac{1}{2} a) = -1$, $x \to \cos_a x$ is a *strictly decreasing* mapping of $[0, \frac{1}{2} a]$ *onto* $[-1, 1]$ (Chapter IV, § 2, no. 6, Theorem 5 and Remark). We have $\cos_a x = 0$ for $x = a/4$, $\cos_a x > 0$ for $0 \leq x < a/4$, $\cos_a x < 0$ for $a/4 < x \leq a/2$. Since $\cos_a (-x) = \cos_a x$ we can deduce how $\cos_a x$ varies in the interval $[- \frac{1}{2} a, 0]$, and hence throughout the whole of $\mathbf{R}$ by periodicity (Fig. 8). Since $\sin_a x = -\cos_a(x + a/4)$ we can also deduce how $\sin_a x$ varies in $\mathbf{R}$ (Fig. 8).

![Graph showing y = sin_a x and y = cos_a x](https://i.imgur.com/3Q5z5QG.png)

Figure 8.

The function $\tan_a x$ is a continuous mapping of $\mathbf{R}$ onto $\tilde{\mathbf{R}}$; it takes the value $\infty$ for the values $\frac{1}{4} a + \frac{1}{2} k a \ (k \in \mathbf{Z})$. Since $\frac{1}{2} a$ is a period of $\tan_2 x$, it is a *principal period*. In the interval $[0, \frac{1}{4} a]$, $\sin_a x$ increases from 0 to 1, $\cos_a x$ decreases from 1 to 0, and therefore $\tan_a x$ is *strictly increasing* in $[0, \frac{1}{4} a[$ and maps this interval onto $[0, +\infty[$; it follows that $\tan_a x$ is strictly increasing in the interval

![A graph showing curves labeled y and x, with axes marked -a/4, 0, a/4, a/2, 3a/4](../images/complex_numbers_9.png)

Figure 9.

]— $\frac{1}{4} a, + \frac{1}{4} a$[. and is a homeomorphism of this interval onto $\mathbf{R}$ (Fig. 9).

### 5. ANGULAR SECTORS

Given two distinct closed rays $\Delta_1, \Delta_2$ with origin o, let $x$ be the principal measure of the angle $(\widehat{\Delta_1, \Delta_2})$ (relative to a base $a$, chosen once and for all). The union of the closed (resp. open) rays $\Delta$ with origin o which are such that the principal measure $y$ of the angle $(\widehat{\Delta_1, \Delta})$ satisfies $0 \leq y \leq x$ (resp. $0 < y < x$) is the closed (resp. open) angular sector S with origin $\Delta_1$ and extremity $\Delta_2$, as defined in algebra. For by means of a rotation we can always reduce to the case where S does not contain the ray through the point — 1. If $\alpha$ and $\beta$ are then the angles which $\Delta_1$ and $\Delta_2$ respectively make with the positive real semi-axis, then the closed angular sector S is the union of the closed half-lines $\Delta$ which make an angle $\theta$ with the positive real semi-axis such that $\tan \frac{1}{2} \alpha \leq \tan \frac{1}{2} \theta \leq \tan \frac{1}{2} \beta$. Now if $u, v, t$ are the measures of $\alpha, \beta, \theta$ respectively which lie in the interval ]— $\frac{1}{2} a, + \frac{1}{2} a$[, these inequalities are equivalent to $\tan_a \frac{1}{2} u \leq \tan_a \frac{1}{2} t \leq \tan_a \frac{1}{2} v$; and since $\tan_a x$ is an increasing function in the interval ]— $\frac{1}{4} a, + \frac{1}{4} a$[, they are also equivalent to $u \leq t \leq v$, or to $0 \leq t - u \leq v - u$; since $x = v - u, y = t - u$, the result is proved for closed angular sectors, and the proof for open ones is similar.

A closed angular sector is a closed set in $\mathbf{R}^2$, and the open angular sector with the same origin and the same extremity is its interior in $\mathbf{R}^2$

Figure 10.

(Chapter VI, § 2, no. 3, Proposition 3). The angle $(\widehat{\Delta_1, \Delta_2})$, with principal measure $x$, is called the angle of the sector S; S is said to be salient if $x < \frac{1}{2} a$, flat (or a closed half-plane) if $x = \frac{1}{2} a$; re-entrant if $x > \frac{1}{2} a$. A salient angular sector is acute if $x < \frac{1}{4} a$, right if $x = \frac{1}{4} a$, obtuse if $x > \frac{1}{4} a$. The bisector of the sector S is the ray $\Delta$ which makes an angle $y = \frac{1}{2} x$ with $\Delta_1$.

Two distinct closed rays $\Delta_1, \Delta_2$ determine two closed angular sectors; their union is the real plane $\mathbf{R}^2$, and their intersection is $\Delta_1 \cup \Delta_2$.

### 6. CROSSES

We have also defined in algebra the cross of a pair of lines in a two-dimensional vector space over a maximal ordered field (*). This definition applies in particular to the real plane $\mathbf{R}^2$. The set $\mathcal{A}_0$ of all crosses has the structure of an abelian group (written additively) defined by

$$
(\overline{D_1, D_3}) = (\overline{D_1, D_2}) + (\overline{D_2, D_3})
$$

so that, in particular, $(\overline{D_1, D_1}) = 0$ and $(\overline{D_2, D_1}) = - (\overline{D_1, D_2})$.

The right cross $\delta_0$ is the solution $\neq 0$ of the equation $2\theta = 0$ in $\mathcal{A}_0$; it is the cross which the imaginary axis makes with the real axis.

(*) We recall that an equivalence relation is defined on the set of all non-isotropic pairs of lines $(D_1, D_2)$ by considering two pairs of lines $(D_1, D_2)$ and $(D'_1, D'_2)$ to be equivalent if there exists a direct similitude which transforms $D_1$ into $D'_1$ and $D_2$ into $D'_2$ simultaneously; the cross of the pair $(D_1, D_2)$ is then the equivalence class of the pair.

We define a canonical homomorphism $\varphi$ of the group $\mathfrak{A}$ of angles onto the group $\mathfrak{A}_0$ of crosses by making correspond to the angle which a ray $\Delta$ makes with the positive real semi-axis, the cross which the line D containing $\Delta$ makes with the real axis. A cross $\theta_0$ is the image under $\varphi$ of two angles $\theta$ and $\theta + \omega$; thus $\mathfrak{A}_0$ is isomorphic to the quotient of $\mathfrak{A}$ by the subgroup $\{0, \omega\}$. If we transport to $\mathfrak{A}_0$ the topology of the quotient group $\mathfrak{A}/\{0, \omega\}$ by means of the bijective homomorphism associated with $\varphi$, then $\mathfrak{A}_0$ becomes a compact topological group and $\varphi$ a strict morphism of $\mathfrak{A}$ onto $\mathfrak{A}_0$.

If we compose the homomorphism $\varphi$ of $\mathfrak{A}$ onto $\mathfrak{A}_0$ with the homomorphism $x \to \tilde{\sigma}(x/a)$ of $\mathbf{R}$ onto $\mathfrak{A}$, we have a homomorphism $x \to \tilde{\sigma}_0(x/a)$ of $\mathbf{R}$ onto $\mathfrak{A}_0$; every cross $\theta_0 \in \mathfrak{A}_0$ corresponds, under this homomorphism, to a class of real numbers mod $\frac{1}{2} a$, which is called the measure of the cross $\theta_0$ (relative to the base $a$); by abuse of language, every number in this class is called a measure of $\theta_0$, and that one which belongs to the interval $[0, \frac{1}{2} a[$ is called the principal measure of $\theta_0$; the cross $\tilde{\sigma}_0(x/a)$ is the cross of measure $x$. Every measure of $\theta_0$ is also a measure of one of the two angles $\theta, \theta + \omega$ whose image under the homomorphism $\varphi$ is $\theta_0$.

Here again, once the base $a$ has been chosen, when we speak of a cross we generally mean, by abuse of language, a measure of this cross relative to the base $a$.

#### Remark {#top-viii-s2-n6-rem-1 .statement}

We can define a homomorphism of $\mathbf{C}^*$ onto $\mathfrak{A}_0$ by mapping each complex number $z \neq 0$ to the cross which the line through o and $z$ makes with the real axis. Clearly this homomorphism is the composition of $\varphi$ and the homomorphism $z \to \mathrm{Am}\,(z)$ of $\mathbf{C}^*$ onto $\mathfrak{A}$; it is therefore a strict morphism of the topological group $\mathbf{C}^*$ onto the topological group $\mathfrak{A}_0$, and the associated bijective homomorphism is an isomorphism of the quotient group $\mathbf{C}^*/\mathbf{R}^*$ onto $\mathfrak{A}_0$.

We know that if D denotes a line making a cross $\theta_0$ with the real axis and if $(a, b)$ is a pair of direction ratios of D, then the tangent of the cross $\theta_0$ (denoted by $\tan\,\theta_0$) is the element $b/a$ of $\tilde{\mathbf{R}}$ ($= \infty$ if $a = 0$), which is also called the slope of the line D. If $\theta$ and $\theta + \omega$ are the two angles whose image under $\varphi$ is $\theta_0$, then we have $\tan\,\theta_0 = \tan\,\theta = \tan(\theta + \omega)$.

The mapping $\theta_0 \to \tan\,\theta_0$ is a homeomorphism of $\mathfrak{A}_0$ onto $\tilde{\mathbf{R}}$, for the topological space $\mathbf{C}^*/\mathbf{R}^*$ is just the real projective line $\mathbf{P}_1$, and from Chapter VI, § 3, no. 3, the mapping of a line (considered as a point of $\mathbf{P}_1$) to its slope is a homeomorphism of $\mathbf{P}_1$ onto $\tilde{\mathbf{R}}$. If now we transport to $\tilde{\mathbf{R}}$ the group structure of $\mathfrak{A}_0$ by means of the mapping $\theta_0 \to \tan\,\theta_0$, we have defined on $\tilde{\mathbf{R}}$ the structure of an abelian topological group, in which the product of two elements $t_1, t_2$ is $\frac{t_1 + t_2}{1 - t_1 t_2}$ whenever $t_1, t_2$ belong to $\mathbf{R}$ and $t_1 t_2 \neq 1$; for pairs $(t_1, t_2)$ which do not satisfy these conditions, the product of $t_1$ and $t_2$ is obtained by extending the function $\frac{x + y}{1 - xy}$ by continuity to $\tilde{\mathbf{R}} \times \tilde{\mathbf{R}}$, and is still denoted by $\frac{t_1 + t_2}{1 - t_1 t_2}$.

### Exercises {#top-viii-s2-exercises}

See the [exercises for § 2](exercises/s2/).
