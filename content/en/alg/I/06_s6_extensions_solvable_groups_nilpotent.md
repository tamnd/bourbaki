---
book: alg
book_title: Algebra
chapter: I
chapter_title: ALGEBRAIC STRUCTURES
section: 6
section_title: Extensions, solvable groups, nilpotent groups
lang: en
source: alg-i-iii
source_edition: 1998, Springer
pdf_pages: 0089-0105, 0171-0183
extraction: ocr
subsections:
    - "no": 1
      title: EXTENSIONS
      page: 0
      pdf_page: 89
    - "no": 2
      title: COMMUTATORS
      page: 0
      pdf_page: 92
    - "no": 3
      title: LOWER CENTRAL SERIES, NILPOTENT GROUPS
      page: 0
      pdf_page: 95
    - "no": 4
      title: DERIVED SERIES, SOLVABLE GROUPS
      page: 0
      pdf_page: 98
    - "no": 5
      title: $p$-GROUPS
      page: 0
      pdf_page: 100
    - "no": 6
      title: SYLOW SUBGROUPS
      page: 0
      pdf_page: 102
    - "no": 7
      title: FINITE NILPOTENT GROUPS
      page: 0
      pdf_page: 104
statements: 58
exercises: 8
content_sha256: 5e97e8733a0ddc8d0586f23204c8a05ccc9e62763723a694e63593829f247770
---

## § 6. EXTENSIONS, SOLVABLE GROUPS, NILPOTENT GROUPS

Throughout this paragraph, the group laws are, unless expressly mentioned otherwise, written multiplicatively.

### 1. EXTENSIONS

#### Definition 1 {#alg-i-s6-def-1 .statement}

Let $F$ and $G$ be two groups. An extension of $G$ by $F$ is a triple $\mathcal{E} = (E, i, p)$, where $E$ is a group, $i$ an injective homomorphism of $F$ into $E$ and $p$ a surjective homomorphism of $E$ onto $G$ such that $\operatorname{Im}(i) = \operatorname{Ker}(p)$. A homomorphism $s : G \to E$ (resp. $r : E \to F$) such that $p \circ s = \operatorname{Id}_G$ (resp. $r \circ i = \operatorname{Id}_F$) is called a section (resp. retraction) of the extension $\mathcal{E}$.

An extension $\mathcal{E} = (E, i, p)$ of $G$ by $F$ is often denoted by the diagram $\mathcal{E} : F \xrightarrow{i} E \xrightarrow{p} G$, in which $i$ and $p$ are sometimes omitted if no confusion can arise. It is sometimes said simply that the group $E$ is an extension of $G$ by $F$.

For a group $E$ to be an extension of $G$ by $F$, it is necessary and sufficient that it contain a normal subgroup $F'$ isomorphic to $F$ such that the quotient group $E/F'$ is isomorphic to $G$.

An extension $\mathcal{E} : F \xrightarrow{i} E \xrightarrow{p} G$ is called central if the image $i(F)$ is contained in the centre of $E$; this is only possible if $F$ is commutative.

Let $\mathcal{E} : F \xrightarrow{i} E \xrightarrow{p} G$ and $\mathcal{E}' : F \xrightarrow{i'} E' \xrightarrow{p'} G$ be two extensions of $G$ by $F$. A morphism of $\mathcal{E}$ into $\mathcal{E}'$ is a homomorphism $u : E \to E'$ such that $p' \circ u = p$ and $u \circ i = i'$, or, in other words, such that the following diagram is commutative:

$$
\begin{array}{ccc}
& & E \\
& i & \\
F & \xrightarrow{i'} & E' \\
& \downarrow & \downarrow \\
& & E \\
& p & \\
& & G
\end{array}
$$

u \uparrow \quad \text{and} \quad p' \uparrow

#### Proposition 1 {#alg-i-s6-prop-1 .statement}

Let $\mathcal{E}: F \xrightarrow{i} E \xrightarrow{p} G$ and $\mathcal{E}': F \xrightarrow{i'} E' \xrightarrow{p'} G$ be extensions of $G$ by $F$. If $u: E \to E'$ is a morphism of $\mathcal{E}$ into $\mathcal{E}'$, $u$ is an isomorphism of $E$ onto $E'$ and $u^{-1}$ is a morphism of $\mathcal{E}'$ into $\mathcal{E}$.

Let $x \in E$ be such that $u(x) = e$. Then $p(x) = p'(u(x)) = e$, whence $x \in i(F)$. Let $y \in F$ be such that $x = i(y)$; then $i'(y) = u(i(y)) = e$. As $i'$ is injective, $y = e$ and $x = e$. Therefore $u$ is injective. By virtue of § 4, no. 6, Corollary 1 to Proposition 7, $u$ is surjective since $u(i(F)) = i'(F)$. The last assertion is immediate.

In other words, the extensions $\mathcal{E}$ and $\mathcal{E}'$ are *isomorphic* if and only if there exists a morphism of $\mathcal{E}$ into $\mathcal{E}'$.

Let $F$ and $G$ be two groups and write $E_0 = F \times G$; let $i: F \to E_0$ be the canonical injection and $p: E_0 \to G$ be the canonical projection. Every extension of $G$ by $F$ isomorphic to the extension $\mathcal{E}_0: F \xrightarrow{i} E_0 \xrightarrow{p} G$ is called a *trivial extension*.

#### Proposition 2 {#alg-i-s6-prop-2 .statement}

*Let $\mathcal{E}: F \xrightarrow{i} E \xrightarrow{p} G$ be an extension of $G$ by $F$. The following conditions are equivalent*:

(i) $\mathcal{E}$ is a trivial extension;
(ii) $\mathcal{E}$ has a retraction $r$;
(iii) $\mathcal{E}$ has a section $s$ such that $s(G)$ is contained in the centralizer of $i(F)$.

Clearly (i) implies (ii) and (iii). If (ii) holds, the mapping $(r, p): E \to F \times G$ is a morphism of $\mathcal{E}$ into $\mathcal{E}_0$, whence (i). If (iii) holds, the homomorphism of $F \times G$ into $E$ corresponding to $(i, s)$ ($\S$ 4, no. 9, Proposition 12) is a morphism of $\mathcal{E}_0$ into $\mathcal{E}$, whence (i).

It may be that an extension $\mathcal{E}: F \to E \to G$ is not trivial and yet the group $E$ is isomorphic to $F \times G$ (Exercise 6).

#### Definition 2 {#alg-i-s6-def-2 .statement}

*Let $F$ and $G$ be two groups and $\tau$ a homomorphism of $G$ into the automorphism group of $F$. Write $\tau(g)(f) = gf$ for $g \in G$ and $f \in F$. The set $F \times G$ with the law of composition*

$$
((f, g), (f', g')) \mapsto (f, g) \cdot_{\tau} (f', g') = (f \cdot gf', gg')
$$

*is called* the external semi-direct product of $G$ by $F$ relative to $\tau$.

The external semi-direct product of $G$ by $F$ relative to $\tau$ is denoted by $F \times_{\tau} G$.

#### Proposition 3 {#alg-i-s6-prop-3 .statement}

*The external semi-direct product $F \times_{\tau} G$ is a group. The mappings $i: F \to F \times_{\tau} G$ defined by $i(f) = (f, e)$, $p: F \times_{\tau} G \to G$ defined by $p(f, g) = g$, and $s: G \to F \times_{\tau} G$ defined by $s(g) = (e, g)$ are group homomorphisms. The triple $(F \times_{\tau} G, i, p)$ is an extension of $G$ by $F$ and $s$ is a section of the extension.*

We have:

$$
((f, g) \cdot_{\tau} (f', g')) \cdot_{\tau} (f'', g'') = (f.gf', gg') \cdot_{\tau} (f'', g'')
= (f.gf'.gg'f'', gg'g'');
$$
$$
(f, g) \cdot_{\tau} ((f', g') \cdot_{\tau} (f'', g'')) = (f, g) \cdot_{\tau} (f'g'f'', g'g'')
= (f.g(f'.g'f''), gg'g'').
$$

Now $g(f'.g'f'') = gf'.gg'f''$, which shows that the law of composition defined by (1) is associative. The element $(e, e)$ is the identity under this law. The element $(f, g)$ admits as inverse $(g^{-1}f^{-1}, g^{-1})$. Hence the law of composition on $F \times_{\tau} G$ is a group law. The other assertions are immediate.

Using the notation of Proposition 3, $\mathscr{E}_{\tau}$ will denote the extension

$$
F \xrightarrow{i} F \times_{\tau} G \xrightarrow{p} G.
$$

Let $\mathscr{E}' : F \xrightarrow{i'} E' \xrightarrow{p'} G$ be an extension of $G$ by $F$ and $s' : G \to E'$ a section of $\mathscr{E}'$. We define an operation $\tau$ of $G$ on the group $F$ by:

(2)
$$
i'(\tau(g, f)) = s'(g)i'(f)s'(g)^{-1} = \operatorname{Int}(s'(g))(i'(f)).
$$

#### Proposition 4 {#alg-i-s6-prop-4 .statement}

*With the above notation, there exists one and only one isomorphism u of $\mathscr{E}_{\tau}$ onto $\mathscr{E}'$ such that $u \circ s = s'$.

$$(f, g) = (f, e) \cdot_{\tau} (e, g) = i(f) \cdot_{\tau} s(g).$$ Therefore, if $u$ is a solution to the problem, of necessity $u(f, g) = i'(f).s'(g)$, whence the uniqueness of $u$. We prove the existence. We write $u(f, g) = i'(f).s'(g)$. Then

$$
\begin{align*}
u(f, g).u(f', g') &= i'(f)s'(g)i'(f')s'(g') \\
&= i'(f)(s'(g)i'(f')s'(g)^{-1})s'(g)s'(g') \\
&= i'(f)i'(\tau(g, f')).s'(g)s'(g') \\
&= i'(f.\tau(g, f')).s'(gg') \\
&= u((f, g) \cdot_{\tau} (f', g')).
\end{align*}
$$

Therefore, $u$ is a homomorphism of $F \times_{\tau} G$ into $E'$. Obviously $u \circ i = i'$, $p' \circ u = p$ and $u \circ s = s'$.

#### Remark {#alg-i-s6-n1-rem-1 .statement}

The definition of the operation $\tau$ by formula (2) depends on the extension $\mathscr{E}'$ and the section $s'$. When $F$ is commutative, the operation $\tau$ does not depend on $s'$. For $\operatorname{Int}(s'(g)) | i'(F)$ depends then only on the coset of $s'(g)$ mod. $i'(F)$.

More generally, let $\mathscr{E} : F \to E \to G$ be an extension of $G$ by a commutative group $F$ (it is not assumed that $\mathscr{E}$ admits a section). The group $E$ operates on $F$ by inner automorphisms, this image is trivial on the image of $F$ and hence defines an operation of $G$ on $F$. If $\mathscr{E}$ admits a section, this operation is that defined by formula (2).

#### Corollary {#alg-i-s6-n1-cor-1 .statement}

*Let $G$ be a group and $H$ and $K$ two subgroups of $G$ such that $H$ is normal, $H \cap K = \{e\}$ and $H.K = G$. Let $\tau$ be the operation of $K$ on $H$ by inner automorphisms of $G$. The mapping $(h, k) \mapsto hk$ is an isomorphism of $H \times_{\tau} K$ onto $G$.

Under the hypotheses of this corollary, $G$ is said to be the semi-direct product of $K$ by $H$.

#### Example {#alg-i-s6-n1-exa-1 .statement}

(1) Let $G$ be a group and $E$ a homogeneous principal $G$-set; let $\Gamma$ denote the automorphism group of $G$. Let $A$ be the set of permutations $f$ of $E$ with the following property:
There exists $\gamma \in \Gamma$ such that $f$ is a $\gamma$-morphism of $E$ into $E$ (that is, $f(gb) = \gamma(g)f(b)$ for $b \in E$ and $g \in G$).
The above formula $f(gb) = \gamma(g)f(b)$ shows that if $f \in A$ there exists a unique $\gamma \in \Gamma$ such that $f$ is a $\gamma$-morphism, we shall denote it by $p(f)$.
Let $f, f'$ be in $A$, $\gamma = p(f), \gamma' = p(f')$. Then, for all $b \in E$ and all $g \in G$,
$$
(f' \circ f)(gb) = f'(\gamma(g)f(b)) = \gamma'(\gamma(g))f'(f(b))
$$
which proves that $f' \circ f \in A$ and that $p(f' \circ f) = p(f')p(f)$. On the other hand, $f(\gamma^{-1}(g)f^{-1}(b)) = gb$, whence $f^{-1}(gb) = \gamma^{-1}(g)f^{-1}(b)$ and $f^{-1} \in A$. Thus $A$ is a subgroup of $\mathcal{S}_E$ and $p$ is a homomorphism of $A$ into $\Gamma$. The kernel of $p$ is the set $\mathrm{Aut}_G(E)$ of automorphisms of the $G$-set $E$.
We fix $a \in E$. We have defined in § 5, no. 6 an isomorphism $\psi_a$ of $G^0$ onto $\mathrm{Aut}_G(E)$ such that $\psi_a(x)(ga) = gxa$ for all $g, x$ in $G$. On the other hand, for $\gamma \in \Gamma$, let $s_a(\gamma)$ be the permutation of $E$ defined by $s_a(\gamma)(ga) = \gamma(g)a$ for all $g \in G$; it is immediately verified that $s_a$ is a homomorphism of $\Gamma$ into $A$ such that $p \circ s_a = \mathrm{Id}_{\tau}$. Thus $G^0 \xrightarrow{\psi_a} A \xrightarrow{p} \Gamma$ is an extension of $\Gamma$ by $G^0$ and $s_a$ is a section of this extension. This extension and this section define an operation of $\Gamma$ on $G^0$, $s_a(\Gamma)$ acting on $\psi_a(G^0)$ by inner automorphisms; we write this operation exponentially. We show that this operation is the natural operation ($§ 3$, no. 1, Example 3): for $x, g$ in $G$ and $\gamma \in \Gamma$,
$$
(\psi_a(\gamma x))(ga) = (s_a(\gamma) \circ \psi_a(x) \circ s_a(\gamma)^{-1})(ga)
= (s_a(\gamma) \circ \psi_a(x))(\gamma^{-1}(g)a) = s_a(\gamma)(\gamma^{-1}(g)xa)
= g\gamma(x)a = \psi_a(\gamma(x))ga
$$
whence $^\gamma x = \gamma(x)$.
Proposition 4 then shows that $A$ is isomorphic to the semidirect product of $\Gamma = \mathrm{Aut}(G)$ by $G^0$ under the natural operation of $\mathrm{Aut}(G)$ on $G^0$. Note that the isomorphism which we have constructed depends in general on the choice of the element $a \in E$.
(2) *Let $A$ be a commutative ring. The upper triangular group $T(n, A)$ is the semi-direct product of the diagonal subgroup $D(n, A)$ by the upper strict triangular group $T_1(n, A)$.*

### 2. COMMUTATORS

#### Definition 3 {#alg-i-s6-def-3 .statement}

Let $G$ be a group and $x$ and $y$ two elements of $G$. The element $x^{-1}y^{-1}xy$ of $G$ is called the commutator of $x$ and $y$.

(x, y) is used to denote the commutator of x and y. Then obviously
$$(y, x) = (x, y)^{-1}.$$
For x and y to commute it is necessary and sufficient that $(x, y) = e$. More generally,
$$xy = yx(x, y).$$
On the other hand we write
(3)
$$x^y = y^{-1}xy = x(x, y) = (y, x^{-1})x.$$
As the mapping $x \mapsto x^y$ is the inner automorphism $\operatorname{Int}(y^{-1})$, $(x, y)^z = (x^z, y^z)$ for all $x, y, z \in G$.

For $x, y, z \in G$, we prove the following relations:
(4)
$$(x, yz) = (x, z).(x, y)^z = (x, z).(z, (y, x)).(x, y)$$
(4 bis)
$$(xy, z) = (x, z)^y.(y, z) = (x, z).((x, z), y).(y, z)$$
(5)
$$(x^y, (y, z)).(y^z, (z, y)).(z^x, (x, y)) = e$$
(6)
$$(x, yz).(z, xy).(y, zx) = e$$
(6 bis)
$$(xy, z).(yz, x).(zx, y) = e.$$

Now
$$
\begin{align*}
(x, yz) &= x^{-1}z^{-1}y^{-1}xyz = (x, z)z^{-1}x^{-1}y^{-1}xyz = (x, z)(x, y)^z \\
&= (x, z)(z, (x, y)^{-1})(x, y)
\end{align*}
$$
by (3), which proves (4). Formula (4 bis) follows similarly. On the other hand,
$$
\begin{align*}
(x^y, (y, z)) &= (x^y)^{-1}(z, y)(x^y)(y, z) \\
&= y^{-1}x^{-1}yz^{-1}y^{-1}zyy^{-1}xyy^{-1}z^{-1}yz \\
&= (yzy^{-1}xy)^{-1}(zxz^{-1}yz).
\end{align*}
$$
Then writing $u = yzy^{-1}xy, v = zxz^{-1}xy$ and $w = xyx^{-1}zx$, we obtain
$$(x^y, (y, z)) = u^{-1}v.$$
By cyclically permuting $x, y, z$, we deduce $(y^z, (z, x)) = v^{-1}w$ and
$$(z^x, (x, y)) = w^{-1}u,$$
which immediately imply (5). Finally, (6) follows by multiplying together the two sides in the three formulae obtained by cyclically permuting $x, y, z$ in the formula $(x, yz) = x^{-1}z^{-1}y^{-1}xyz = (yzx)^{-1}(xyz)$, and similarly for (6 bis).

If A and B are two subgroups of G, (A, B) denotes the subgroup generated by the commutators $(a, b)$ with $a \in A$ and $b \in B$.† Then $(A, B) = \{e\}$ if and only if A centralizes B. $(A, B) \subset A$ if and only if B normalizes A. If A and B are normal (resp. characteristic), so is $(A, B)$.

† We here reject the notational convention made in § 1, no 1 of extending a law of composition to subsets.

#### Proposition 5 {#alg-i-s6-prop-5 .statement}

Let $A, B, C$ be three subgroups of $G$.

(i) The subgroup $A$ normalizes the subgroup $(A, B)$.

(ii) If the subgroup $(B, C)$ normalizes $A$, the subgroup $(A, (B, C))$ is generated by the elements $(a, (b, c))$ with $a \in A, b \in B$ and $c \in C$.

(iii) If $A, B$ and $C$ are normal, then

$$
(A, (B, C)) \subset (C, (B, A)).(B, (C, A)).
$$

By (4 bis), for $a, a' \in A$ and $b \in B$,

$$
(a, b)^{a'} = (aa', b).(a', b)^{-1},
$$

whence (i). Suppose now that $(B, C)$ normalizes $A$. For $a \in A, b \in B, c \in C$ and $x \in G$, (4) implies

$$
(a, (b, c).x) = (a, x).(x, ((b, c), a))(a, (b, c))
$$

and $((b, c), a) \in A$ since $(B, C)$ normalizes $A$, whence by induction on $p$ the fact that $\left( a, \prod_{i=1}^p (b_i, c_i) \right)$, for $b_i \in B, c_i \in C$, belongs to the subgroup generated by the elements of the form $(a, (b, c))$. If finally $A, B$ and $C$ are normal, so are the subgroups $(A, (B, C))$, $(C, (B, A))$ and $(B, (C, A))$. It therefore suffices by (ii) to show that

$$
(a, (b, c)) \in (C, (B, A)).(B, (C, A))
$$

for all $a \in A, b \in B$ and $c \in C$. Now by (5), writing $a^{b^{-1}} = u$

$$
(a, (b, c)) = ((u^b), (b, c)) = (c^u, (u, b))^{-1}.(b^c, (c, u))^{-1},
$$

whence (iii).

#### Definition 4 {#alg-i-s6-def-4 .statement}

Let $G$ be a group. The subgroup generated by the commutators of elements of $G$ is called the derived group of $G$.

The derived group of $G$ is thus the subgroup $(G, G)$. It is also denoted by $D(G)$. By an abuse of language, it is sometimes called the *commutator group* of $G$ although it is in general distinct from the set of commutators of elements of $G$ (Exercise 16). $D(G) = \{e\}$ if and only if $G$ is commutative.

#### Proposition 6 {#alg-i-s6-prop-6 .statement}

Let $f : G \to G'$ be a group homomorphism. Then $f(D(G)) \subset D(G')$. If $f$ is surjective, the homomorphism of $D(G)$ into $D(G')$ the restriction of $f$ is surjective.

The image under $f$ of a commutator of elements of $G$ is a commutator of elements of $G'$. If $f$ is surjective, the image under $f$ of the set of commutators of $G$ is the set of commutators of $G'$. The proposition thus follows from § 4, no. 3, Corollary 3 to Proposition 2.

#### Corollary 1 {#alg-i-s6-prop-6-cor-1 .statement}

The derived group of a group $G$ is a characteristic subgroup of $G$. In particular it is a normal subgroup of $G$.

#### Corollary 2 {#alg-i-s6-prop-6-cor-2 .statement}

Let G be a group. The quotient group G/D(G) is commutative. Let $\pi : G \to G/D(G)$ be the canonical homomorphism. Every homomorphism f of G into a commutative group G' can be expressed uniquely in the form $f = \bar{f} \circ \pi$, where $\bar{f} : G/D(G) \to G'$ is a homomorphism.

Now $\pi(D(G)) = \{e\}$. As $\pi$ is surjective, it follows that $D(G/D(G)) = \{e\}$, whence the first assertion. The second follows from § 4, no. 4, Proposition 5.

#### Corollary 3 {#alg-i-s6-prop-6-cor-3 .statement}

Let H be a subgroup of G. The following conditions are equivalent:

(i) $H \supset D(G)$;
(ii) H is a normal subgroup and $G/H$ is commutative.
(ii) $\Rightarrow$ (i) by Corollary 2 and (i) $\Rightarrow$ (ii) by § 4, no. 7, Theorem 4, since every subgroup of a commutative group is normal.

#### Corollary 4 {#alg-i-s6-prop-6-cor-4 .statement}

Let G be a group and X a subset of G which generates G. The group D(G) is the normal subgroup of G generated by the commutators of elements of X.

Let H be the normal subgroup of G generated by the commutators of elements of X and $\phi : G \to G/H$ the canonical homomorphism. The set $\phi(X)$ generates $G/H$. The elements of $\phi(X)$ are pairwise permutable and hence H is commutative (§ 4, no. 3, Corollary 2 to Proposition 2). Hence (Corollary 3) H contains D(G). On the other hand, obviously $H \subset D(G)$.

#### Remark {#alg-i-s6-n2-rem-1 .statement}

(1) Corollary 2 can also be expressed by saying that $G/D(G)$, together with $\pi$, is a solution of the universal mapping problem for G, relative to commutative groups and homomorphisms from G to commutative groups.

(2) Under the hypotheses of Corollary 4, the subgroup generated by the commutators of elements of X is contained in D(G) but is not in general equal to D(G) (cf. Exercise 15e).

#### Example {#alg-i-s6-n2-exa-1 .statement}

(1) If G is a non-commutative simple group, then $D(G) = G$. Therefore every homomorphism of G into a commutative group is trivial.

(2) The derived group of the symmetric group $S_n$ is the alternating group $A_n$. For $A_n$ is generated by the products of two transpositions; if $\tau = \tau_{x,y}$ and $\tau' = \tau_{x',y'}$ are two transpositions, let $\sigma$ be a permutation such that $\sigma(x') = x$ and $\sigma(y') = y$. Then $\tau' = \sigma^{-1} \tau \sigma$ and $\tau \tau' = \tau^{-1} \tau' = \tau^{-1} \sigma^{-1} \tau \sigma$ is a commutator. Hence $A_n \subset D(S_n)$. As $S_n/A_n$ is commutative, $A_n \supset D(S_n)$ (Corollary 3).

### 3. LOWER CENTRAL SERIES, NILPOTENT GROUPS

Let G be a group, H a subgroup of G and K a normal subgroup of G. The image of H in G/K is contained in the centre of G/K if and only if $(G, H) \subset K$.

#### Definition 5 {#alg-i-s6-def-5 .statement}

Let G be a group. The lower central series of G is the sequence $(C^n(G))_{n \geq 1}$ of subgroups of G defined inductively by:
$$
C^1(G) = G, \quad C^{n+1}(G) = (G, C^n(G)).
$$

Let $f : G \to G'$ be a group homomorphism. It is seen, by induction on $n$, that $f(C^n(G)) \subset C^n(G')$ and that, if $f$ is surjective, $f(C^n(G)) = C^n(G')$. In particular, for all $n \geq 1$, $C^2(G)$ is a characteristic (and hence normal) subgroup of $G$. For all $n \geq 1$, $C^n(G)/C^{n+1}(G)$ is contained in the centre of $G/C^{n+1}(G)$.

Let $(G_1, G_2, \ldots)$ be a decreasing sequence of normal subgroups of $G$ such that (1) $G_1 = G$; (2) for all $i$, $G_i/G_{i+1}$ is contained in the centre of $G/G_{i+1}$. Then $C^i(G) \subset G_i$, as is seen by induction on $i$.

Now
$$
(C^m(G), C^n(G)) \subset C^{m+n}(G).
$$
For, if this relation is denoted by $(F_{m,n})$, it follows from $(F_{m,n})$, by no. 2, Proposition 5, that
$$
\begin{align*}
(C^m(G), C^{n+1}(G)) &\subset (G, (C^m(G), C^n(G))).(C^n(G), (G, C^m(G))) \\
&\subset C^{m+n+1}(G).(C^{m+1}(G), C^n(G)).
\end{align*}
$$
Hence $((F_{m,n}) \text{ and } (F_{m+1,n})) \Rightarrow (F_{m,n+1})$. As $(F_{m,1})$ and $(F_{1,n})$ are obvious $(F_{m,n})$ follows by induction.

#### Definition 6 {#alg-i-s6-def-6 .statement}

*A group $G$ is called nilpotent if there exists an integer $n$ such that $C^{n+1}(G) = \{e\}$. The least integer $n$ such that $C^{n+1}(G) = \{e\}$ is called the nilpotency class of a nilpotent group $G$.*

If $n \in \mathbf{N}$, a group of nilpotency class $n$ is called a nilpotent group of class $n$. It is sometimes said that the nilpotency class of a group $G$ is finite if $G$ is nilpotent.

#### Example {#alg-i-s6-n3-exa-1 .statement}

(1) A group is nilpotent of class 0 (resp. $\leq 1$) if and only if it consists of the identity element (resp. is commutative).

(2) *For every commutative ring $A$ and every integer $n \geq 1$, the upper strict triangular group $T_1(n, A)$ is nilpotent of class $\leq n - 1$ (and exactly of class $n - 1$ if $A \neq \{0\}$).*

(3) Let $G$ be a nilpotent group of class $n$. Every subgroup (resp. every quotient group) of $G$ is nilpotent of class $\leq n$. For, if $H$ is a subgroup of $G$, then $C^n(H) \subset C^n(G)$. If $G'$ is a quotient group of $G$ and $\pi : G \to G'$ is the canonical homomorphism, then $C^n(G') = \pi(C^n(G))$.

(4) A finite product of nilpotent groups is nilpotent.

#### Proposition 7 {#alg-i-s6-prop-7 .statement}

*Let $G$ be a group and $n$ an integer. The following conditions are equivalent:*

(a) $G$ is nilpotent of class $\leq n$.
(b) *There exists a series of subgroups of $G$:*
$$
G = G^1 \supset G^2 \supset \ldots \supset G^{n+1} = \{e\}
$$
*such that* $(G, G^{k'}) \subset G^{k'+1}$ *for all* $k \in \{1, n\}$.

(c) There exists a subgroup $A$ of $G$ contained in the centre of $G$ such that $G/A$ is nilpotent of class $\leq n - 1$.

(a) $\Rightarrow$ (b): it suffices to take $G^k = C^k(G)$.
(b) $\Rightarrow$ (a): by induction on $k$, $C^k(G) \subset G^k$.
(a) $\Rightarrow$ (c): it suffices to take $A = C^n(G)$.
(c) $\Rightarrow$ (a): let $\pi : G \to G/A$ be the canonical homomorphism; then $\pi(C^n(G)) = C^n(G/A) = \{e\}$ and hence $C^n(G) \subset A$, whence $C^{n+1}(G) = \{e\}$.

More briefly: a group is nilpotent of class $\leq n$ if it can be obtained from the group $\{e\}$ by $n$ successive central extensions.

#### Corollary {#alg-i-s6-n3-cor-1 .statement}

*A central extension of a nilpotent group (by a necessarily commutative group) is nilpotent.*

#### Proposition 8 {#alg-i-s6-prop-8 .statement}

*Let $G$ be a nilpotent group of class $\leq n$ and let $H$ be a subgroup of $G$. There exists a sequence of subgroups*

$$
G = H^1 \supset H^2 \supset \ldots \supset H^{n+1} = H,
$$

*such that $H^{k+1}$ is normal in $H^k$ and $H^k/H^{k+1}$ is commutative for all $k \leq n$.*

Choose a sequence $(G^k)$ of subgroups of $G$ satisfying the conditions of Proposition 7 (b) for all $k$; $G^k$ is normal in $G$. Write:

$$
H^k = H.G^k.
$$

It is necessary to verify that $H^{k+1}$ is normalized by $H^k = H.G^k$; as it is normalized by $H$, it suffices to verify that it is by $G^k$. Now, if $s \in G^k$ and $h \in H$,

$$
shs^{-1} = shs^{-1}h^{-1}.h \in (G, G^k).H
$$

and $(G, G^k).H$ is contained in $G^{k+1}.H = H^{k+1}$; hence $s.H^{k+1}.s^{-1} = H^{k+1}$, which shows that $H^{k+1}$ is normal in $H^k$.

Finally, the canonical homomorphism $G^k/G^{k+1} \to H^k/H^{k+1}$ is obviously surjective; as the first group is commutative, so is the second.

#### Corollary 1 {#alg-i-s6-prop-8-cor-1 .statement}

*Let $G$ be a nilpotent group and $H$ a subgroup of $G$. If $H$ is distinct from $G$, the normalizer $N_G(H)$ of $H$ in $G$ is distinct from $H$.*

Let $k$ be the largest index such that $H^k \neq H$. The group $H^k$ normalizes $H$ and is distinct from $H$.

#### Corollary 2 {#alg-i-s6-prop-8-cor-2 .statement}

*Let $G$ be a nilpotent group and $H$ a subgroup of $G$. If $H$ is distinct from $G$, there exists a normal subgroup $N$ of $G$, containing $H$, distinct from $G$ and such that $G/N$ is commutative.*

Let $k$ be the least index such that $H^k \neq G$. The group $H^k$ satisfies the required conditions.

#### Corollary 3 {#alg-i-s6-prop-8-cor-3 .statement}

*Let G be a nilpotent group and H a subgroup of G. If G = H.(G, G), then G = H.*

Every subgroup N of G which contains H and such that G/N is commutative contains H.(G, G). Corollary 3 thus follows from Corollary 2.

Corollary 3 can also be formulated thus: let X be a subset of G. For X to generate G, it is necessary and sufficient that the image of X in G/D(G) generate G/D(G).

#### Corollary 4 {#alg-i-s6-prop-8-cor-4 .statement}

*Let f: G' → G be a group homomorphism. Suppose that*
(a) *G is nilpotent.*
(b) *The homomorphism f₁: G'/(G', G') → G/(G, G), derived from f by passing to the quotients, is surjective.*
*Then f is surjective.*

This follows from Corollary 3 applied to the subgroup H = f(G').

#### Proposition 9 {#alg-i-s6-prop-9 .statement}

*Let G be a nilpotent group of class ≤ n and let N be a normal subgroup of G. There exists a series of subgroups*

$$
N = N^1 \supset N^2 \supset \ldots \supset N^{n+1} = \{e\}
$$

*such that* (G, N^k) ⊂ N^{k+1} *for k = 1, ..., n.*

If (G^k) satisfies condition (b) of Proposition 7, then take

$$
N^k = G^k \cap N.
$$

#### Corollary 1 {#alg-i-s6-prop-9-cor-1 .statement}

*Let G be a nilpotent group, Z the centre of G and N a normal subgroup of G. If N ≠ {e}, then N ∩ Z ≠ {e}.*

Let k be the largest index such that N^k ≠ {e}. The group N^k is contained in N. On the other hand, (G, N^k) ⊂ N^{k+1} = {e}; hence N^k is contained in the centre Z of G.

#### Corollary 2 {#alg-i-s6-prop-9-cor-2 .statement}

*Let f be a homomorphism from a nilpotent group G to a group G'. If the restriction of f to the centre of G is injective, f is injective.*

This is Corollary 1 applied to Ker(f).

### 4. DERIVED SERIES, SOLVABLE GROUPS

#### Definition 7 {#alg-i-s6-def-7 .statement}

*Let G be a group. The derived series of G is the series (D^n(G))_{n \in \mathbf{N}} defined inductively by:*

$$
D^0(G) = G; \quad D^{n+1}(G) = D(D^n(G)) \quad \text{for } n \in \mathbf{N}.
$$

Then $D^0(G) = C^1(G) = G,\ D^1(G) = C^2(G) = D(G) = (G, G)$. For all n \in \mathbf{N}, D^n(G) \subset C^{2^n}(G), as is seen by induction on n using formula (7) of no. 3.

Let $f : G \to G'$ be a group homomorphism. It is seen, by induction on n, that $f(D^n(G)) \subset D^n(G')$ and that, if $f$ is surjective, $f(D^n(G)) = D^n(G')$. In particular, for all $n \in \mathbf{N}$, $D^n(G)$ is a characteristic (and therefore normal) subgroup of G. For all $n \in \mathbf{N}$, the group $D^n(G)/D^{n+1}(G)$ is a commutative normal (but not in general central) subgroup of $G/D^{n+1}(G)$.

Let $(G_0, G_1, \ldots)$ be a decreasing sequence of subgroups of G such that: (1) $G_0 = G$; (2) for all $i$, $G_{i+1}$ is normal in $G_i$ and $G_i/G_{i+1}$ is commutative. Then $D^i(G) \subset G_i$ for all $i$, as is seen by induction on $i$.

#### Definition 8 {#alg-i-s6-def-8 .statement}

*A group G is called solvable if there exists an integer n such that $D^n(G) = \{e\}$. If G is a solvable group, the least integer n such that $D^n(G) = \{e\}$ is called the solvability class of G.*

A solvable group of solvability class $n$ is called a solvable group of class $n$. A group is sometimes said to be of finite solvability class if it is solvable.

#### Example {#alg-i-s6-n4-exa-1 .statement}

(1) A group is solvable of class 0 (resp. $\leq 1$) if and only if it is reduced to $\{e\}$ (resp. is commutative).

(2) Every nilpotent group of class $\leq 2^n - 1$ is solvable of class $\leq n$; this follows from the relation $D^n(G) \subset C^{2^n}(G)$ proved above.

(3) Let G be a solvable group of class $\leq n$. Every subgroup (resp. quotient group) of G is solvable of class $\leq n$ (proof analogous to that of no. 3, Example 3).

(4) If G is a solvable group of class $p$ and F is a solvable group of class $q$, every extension E of G by F is a solvable group of class $\leq p + q$. For, let $\pi : E \to G$ be the projection; then $\pi(D^p(E)) \subset D^p(G) = \{e\}$ and therefore $D^p(E) \subset F$; it follows that $D^{p+q}(E) = D^q(D^p(E)) \subset D^q(F) = \{e\}$.

(5) The symmetric group $S_n$ is solvable if and only if $n < 5$ (cf. § 5, Exercises 10 and 16).

(6) *If A is a commutative ring, the upper triangular group T(n, A) is solvable but not in general nilpotent.*

#### Proposition 10 {#alg-i-s6-prop-10 .statement}

*Let G be a group and n an integer. The following conditions are equivalent:*

(i) *G is solvable of class $\leq n$.*
(ii) *There exists a series of normal subgroups of G*
$$
G = G^0 \supset G^1 \supset \ldots \supset G^n = \{e\}
$$
*such that the groups $G^k/G^{k+1}$ are commutative.*
(iii) *There exists a series of subgroups of G*
$$
G = G^0 \supset G^1 \supset \ldots \supset G^n = e
$$
*such that, for all k, $G^{k+1}$ is a normal subgroup of $G^k$ and $G^k/G^{k+1}$ is commutative.*

(iv) There exists a normal commutative subgroup $A$ of $G$ such that $G/A$ is solvable of class $\leq n - 1$.

For (i) $\Rightarrow$ (ii) it suffices to take $G^k$ equal to $D^k(G)$. (ii) $\Rightarrow$ (iii) trivially. (iii) $\Rightarrow$ (i) for $D^k(G)$ is necessarily contained in $G^k$. The equivalence of (ii) and (iv) is immediate by induction on $n$.

More briefly: a group is solvable of class $\leq n$ if it can be obtained by successive extensions of $n$ commutative groups.

#### Corollary {#alg-i-s6-n4-cor-1 .statement}

Let $G$ be a finite group and
$$
G = G^0 \supset G^1 \supset \ldots \supset G^n = \{e\}
$$
a Jordan-Hölder series of $G$ For $G$ to be solvable, it is necessary and sufficient that the quotients $G^k/G^{k+1}$ be cyclic of prime order.

If the quotients of a composition series of $G$ are cyclic and hence commutative, $G$ is solvable by Proposition 10. Conversely, if $G$ is solvable, the group $G^k/G^{k+1}$ is, for all $k$, solvable and simple ($§ 4$, no. 7, Proposition 9). Now, every solvable simple group $H$ is cyclic of prime order. For $D(H)$ is a normal subgroup of $H$; $D(H) = H$ is impossible for in that case $D^k(H) = H$ for all $k$; then $D(H) = \{e\}$ and $H$ is commutative. The corollary then follows from $§ 4$, no. 10, Corollary to Proposition 20.

### 5. $p$-GROUPS

In this number and the following, the letter $p$ denotes a prime number ($§ 4$, no 10, Proposition 16).

#### Definition 9 {#alg-i-s6-def-9 .statement}

A finite group whose order is a power of $p$ is called a $p$-group.

Let $G$ be a $p$-group of order $p^r$. Every divisor of $p^r$ is a power of $p$ ($§ 4$, no. 10, Corollary to Theorem 7). Therefore every subgroup and every quotient group of $G$ is a $p$-group ($§ 4$, no. 4, Corollary to Proposition 4); the cardinal of every homogeneous space of $G$ is a power of $p$ ($§ 5$, no. 5, Theorem 1).

An extension of a $p$-group by a $p$-group is a $p$-group.

*Examples. (1) A commutative $p$-group is isomorphic to a product of cyclic groups $\mathbf{Z}/p^n\mathbf{Z}$ (cf. Exercise 19 and also VII, $§ 4$, no. 7, Proposition 7).
(2) Let $k$ be a finite field of characteristic $p$. The strict triangular group $T_1(n, k)$ is a $p$-group.
(3) The quaternionic group $\{ \pm 1, \pm i, \pm j, \pm k \}$ is a 2-group (cf. Exercise 4).*

#### Proposition 11 {#alg-i-s6-prop-11 .statement}

Let $E$ be a finite set and $G$ a $p$-group operating on $E$. Let $E^G$ denote the set of $x \in E$ such that $gx = x$ for all $g \in G$ (the fixed points). Then
$$
\operatorname{Card}(E^G) \equiv \operatorname{Card}(E) \pmod{p}.
$$

E — E^G is a disjoint union of orbits not reduced to a point. The cardinal of such an orbit is a power of $p$ distinct from $p^0 = 1$ and hence a multiple of $p$.

#### Corollary {#alg-i-s6-n5-cor-1 .statement}

*Let G be a p-group. If G is not reduced to e, its centre is not reduced to e.*

Let G operate on itself by inner automorphisms. The set of fixed points is the centre Z of G. By Proposition 11,

$$
\operatorname{Card}(Z) \equiv \operatorname{Card}(G) \equiv 0 \pmod{p},
$$

whence $\operatorname{Card}(Z) \neq 1$ and $Z \neq \{e\}$.

#### Theorem 1 {#alg-i-s6-thm-1 .statement}

*Let G be a p-group and $p^r$ its order. There exists a sequence of subgroups of G*

$$
G = G^1 \supset G^2 \supset \ldots \supset G^{r+1} = \{e\}
$$

*such that* $(G, G^k) \subset G^{k+1}, 1 \leq k \leq r,$ and $G^k/G^{k+1}, 1 \leq k \leq r,$ *is cyclic of order* $p$.

The theorem is true for $G = \{e\}$. We prove it by induction on $\operatorname{Card}(G)$. Let Z be the centre of G, $x \neq e$ an element of Z (Corollary to Proposition 11) and $p^s, s \neq 0,$ the order of x. Then $x^{p^s - 1}$ is an element of order $p$ and therefore Z contains a subgroup $G'$ which is cyclic of order $p$. By the induction hypothesis, the group $G' = G/G'$ has a series of subgroups $({G'}^k)_{1 \leq k \leq r}$ with the required properties. Let $\pi : G \to G'$ be the canonical homomorphism. The sequence of subgroups of G defined by $G^k = \pi^{-1}({G'}^k), 1 \leq k \leq r, G^{r+1} = \{e\}$ is a solution for $G^k/G^{k+1}$ is isomorphic to ${G'}^k/{G'}^{k+1}$ for $1 \leq k \leq r$ (§ 4, no. 7, Theorem 4).

#### Corollary {#alg-i-s6-n5-cor-2 .statement}

*Every p-group is nilpotent.*

This follows from no. 3, Proposition 7.

#### Proposition 12 {#alg-i-s6-prop-12 .statement}

*Let G be a p-group and H a subgroup of G distinct from G. Then:*

(a) *The normalizer* $N_G(H)$ *of H in G is distinct from G*.
(b) *There exists a normal subgroup* N *of G of index p in G, which contains* H.

Assertion (a) follows from no. 3, Corollary 1 to Proposition 8. We prove (b). By no. 3, Corollary 2 to Proposition 8, there exists a normal subgroup $N'$ of G containing H, distinct from G and such that $G/N'$ is commutative. Let N be a maximal subgroup distinct from G containing $N'$. Then N is normal (no. 2, Corollary 3 to Proposition 6) and $G/N$ is a simple commutative $p$-group and hence cyclic of order $p$ (§ 4, no. 10, Corollary to Proposition 20).

#### Corollary {#alg-i-s6-n5-cor-3 .statement}

*Let G be a p-group. Every subgroup of G of index p is normal.*

### 6. SYLOW SUBGROUPS

#### Definition 10 {#alg-i-s6-def-10 .statement}

Let G be a finite group. A Sylow p-subgroup of G is any subgroup P of G satisfying the two following conditions:

(a) P is a p-group.
(b) (G : P) is not a multiple of p.

If the order of G is written in the form $p^r m$, where m is not a multiple of $p$, conditions (a) and (b) are equivalent to $\mathrm{Card}(P) = p^r$.

#### Example {#alg-i-s6-n6-exa-1 .statement}

(1) In the group $\mathfrak{S}_p$ let $\zeta$ be a cycle of order $p$. The subgroup generated by $\zeta$ is a Sylow $p$-subgroup of $\mathfrak{S}_p$ for $p$ does not divide $(p - 1)!$.
(2) *Let k be a finite field of characteristic $p$ and let n be a positive integer. The strict triangular group $T_1(n, k)$ is a Sylow $p$-subgroup of the group $\mathbf{GL}(n, k)$.*

#### Theorem 2 {#alg-i-s6-thm-2 .statement}

Every finite group contains a Sylow $p$-subgroup.

The proof depends on the following lemma.

#### Lemma {#alg-i-s6-n6-lem-1 .statement}

Let $n = p^r m$, where m is an integer which is not a multiple of $p$. Then
$$
\binom{n}{p^r} \not\equiv 0 \pmod{p}.
$$

Let S be a group of order $p^r$ (for example $\mathbf{Z}/p^r \mathbf{Z}$) and T a set with m elements. Write $X = S \times T$ and let E be the set of subsets of X with $p^r$ elements. Then $\mathrm{Card}(X) = n$, whence $\mathrm{Card}(E) = \binom{n}{p^r}$ (Set Theory, III, § 5, no. 8, Corollary 1 to Proposition 11). Let S operate on X by $s.(x, y) = (sx, y) (s, x \in S, y \in T)$ and consider the canonical extension of this operation to E. In the notation of no. 5, Proposition 11, the set $E^S$ is the set of orbits of X, that is the set of subsets $Y \subset X$ of the form $S \times \{ t \}, t \in T$, whence $\mathrm{Card}(E^S) = m$. By no. 5, Proposition 11,
$$
\binom{n}{p^r} = \mathrm{Card}(E) \equiv \mathrm{Card}(E^S) = m \not\equiv 0 \pmod{p},
$$
which proves the lemma.

We now prove the theorem. Let G be a finite group and n its order; we write $n = p^r m$, where m is not a multiple of $p$. Let E be the set of subsets of G with $p^r$ elements. Then
$$
\mathrm{Card}(E) = \binom{n}{p^r};
$$
whence, by virtue of the lemma, $\mathrm{Card}(E) \not\equiv 0 \pmod{p}$. Consider the extension to E of the operation of G on itself by left translation. There exists $X \in E$ whose orbit has non-zero cardinal mod. $p$. If $H_X$ denotes the stabilizer of X, then

(G:H_x) \not\equiv 0 \pmod{p}, which means that $p^r$ divides Card(H_x). But H_x consists of the $s \in G$ such that $sX = X$; if $x \in X$, then $H_x \subset X.x^{-1}$, whence Card(H_x) $\leqslant$ Card(X) = $p^r$. Hence Card(H_x) = $p^r$.

#### Corollary {#alg-i-s6-n6-cor-1 .statement}

*If the order of G is divisible by p, the group G contains an element of order p.*

By virtue of Theorem 2, this is reduced to the case where G is a $p$-group $\neq \{e\}$; if $x \in G$ is different from e, the cyclic group generated by x is then of order $p^n$ with $n \geqslant 1$ and it therefore contains a subgroup of order $p$.

#### Remark {#alg-i-s6-n6-rem-1 .statement}

For every prime number q dividing Card(G), let P_q be a Sylow q-subgroup of G. Then the subgroup H of G generated by the P_q is of order a multiple of Card(P_q) for each q and of order a divisor of Card(G), hence it is equal to G.

#### Theorem 3 {#alg-i-s6-thm-3 .statement}

*Let G be a finite group.*
(a) *The Sylow p-subgroups of G are conjugate to one another. Their number is congruent to 1 mod. p.*
(b) *Every subgroup of G which is a p-group is contained in a Sylow p-subgroup.*

Let P be a Sylow $p$-subgroup of G (Theorem 2) and let H be a $p$-subgroup of G. Let E = G/P and consider the operation of H on G/P. As Card(E) $\not\equiv 0$ mod. $p$, Proposition 11 of no. 5, shows that there exists $x \in G/P$ such that $hx = x$ for all $h \in H$. If g is a representative of x in G, this means that $H \subset gPg^{-1}$, whence assertion (b).

If H is a Sylow $p$-subgroup, then Card(H) = Card(P) = Card($gPg^{-1}$), whence $H = gPg^{-1}$, which proves the first assertion of (a).

We now prove the second assertion of (a). Let $\mathcal{S}$ be the set of Sylow $p$-subgroups of G and let P operate on $\mathcal{S}$ by inner automorphisms. The element $P \in \mathcal{S}$ is a fixed point under this operation, we show that it is the only one. Let $Q \in \mathcal{S}$ be a fixed point; Q is a Sylow subgroup of G normalized by P and hence P is contained in the normalizer N of Q. The groups P and Q are Sylow $p$-subgroups of N; hence there exists $n \in N$ such that $P = nQn^{-1} = Q$. By no. 5, Proposition 11, Card($\mathcal{S}^P$) $\equiv$ Card($\mathcal{S}^{P^P}$) = 1 (mod. $p$).

#### Corollary 1 {#alg-i-s6-thm-3-cor-1 .statement}

*Let P be a Sylow p-subgroup of G, let N be its normalizer in G and let M be a subgroup of G containing N. The normalizer of M in G is equal to M.*

Let $s \in G$ be such that $sMs^{-1} = M$. The subgroup $sPs^{-1}$ of M is a Sylow $p$-subgroup of M. There thus exists $t \in M$ such that $sPs^{-1} = tPt^{-1}$; then $t^{-1}s \in N$, whence $s \in tN \subset M$.

#### Corollary 2 {#alg-i-s6-thm-3-cor-2 .statement}

*Let $f : G_1 \to G_2$ be a homomorphism of finite groups. For every Sylow p-subgroup $P_1$ of $G_1$ there exists a Sylow p-subgroup $P_2$ of $G_2$ such that $f(P_1) \subset P_2$.*

This follows from Theorem 3 (b) applied to the subgroup $f(P_1)$ of $G_2$.

#### Corollary 3 {#alg-i-s6-thm-3-cor-3 .statement}

(a) Let $H$ be a subgroup of $G$. For every Sylow $p$-subgroup $P$ of $H$ there exists a Sylow $p$-subgroup $Q$ of $G$ such that $P = Q \cap H$.

(b) Conversely, if $Q$ is a Sylow $p$-subgroup of $G$ and $H$ is normal in $G$, the group $Q \cap H$ is a Sylow $p$-subgroup of $H$.

(a) The $p$-group $P$ is contained in a Sylow $p$-subgroup $Q$ of $G$ and $Q \cap H$ is a $p$-subgroup of $H$ containing $P$ and is hence equal to $P$.

(b) Let $P'$ be a Sylow $p$-subgroup of $H$. There exists an element $g \in G$ such that $gP'g^{-1} \subset Q$. As $H$ is normal, $P = gP'g^{-1}$ is contained in $H$ and hence in $Q \cap H$. As $Q \cap H$ is a $p$-subgroup of $H$ and $P$ is a Sylow $p$-subgroup of $H$, $P = Q \cap H$.

#### Corollary 4 {#alg-i-s6-thm-3-cor-4 .statement}

Let $N$ be a normal subgroup of $G$. The image in $G/N$ of a Sylow $p$-subgroup of $G$ is a Sylow $p$-subgroup of $G/N$ and every Sylow $p$-subgroup of $G/N$ is obtained in this way.

Let $G' = G/N$ and $P'$ be the image in $G'$ of a Sylow $p$-subgroup $P$ of $G$. The group $G$ operates transitively on $G'/P'$ and hence $G'/P'$ is equipotent to $G/S$, where $S$ is a subgroup of $G$ containing $P$. Therefore $(G':P')$ divides $(G:P)$, is thus not a multiple of $p$ and the $p$-group $P'$ is a Sylow $p$-subgroup of $G'$. Let $Q'$ be another Sylow $p$-subgroup of $G'$; then $Q' = g'P'{g'}^{-1}$ for some $g' \in G'$; if $g \in G$ is a representative of $g'$, the group $Q'$ is the image of $Q = gPg^{-1}$.

### 7. FINITE NILPOTENT GROUPS

#### Theorem 4 {#alg-i-s6-thm-4 .statement}

Let $G$ be a finite group. The following conditions are equivalent:

(a) $G$ is nilpotent.
(b) $G$ is a product of $p$-groups.
(c) For every prime number $p$ there exists a normal Sylow $p$-subgroup of $G$.
(b) $\Rightarrow$ (a) (no. 5, Corollary to Theorem 1).

Suppose (a) holds and let $P$ be a Sylow $p$-subgroup of $G$. If $N$ is the normalizer of $P$ in $G$, Corollary 1 to Theorem 3 shows that $N$ is its own normalizer. By § 6, no. 3, Corollary to Proposition 8, this shows that $N = G$. Hence (a) $\Rightarrow$ (c).

Suppose (c) holds and let $I$ be the set of prime numbers dividing $\mathrm{Card}(G)$. For all $p \in I$, let $P_p$ be a normal Sylow $p$-subgroup of $G$. For all $p \neq q$, $P_p \cap P_q$ is reduced to $e$ for it is both a $p$-group and a $q$-group, hence $P_p$ and $P_q$ centralize one another ($§ 4$, no. 9, Proposition 15). Let $\phi$ be the canonical homomorphism ($§ 4$, no. 9, Proposition 12) of $\prod_{p \in I} P_p$ into $G$. The homomorphism $\phi$ is surjective by the Remark of no. 6. As $\mathrm{Card}\left(\prod_{p \in I} P_p\right) = \mathrm{Card}(G)$, it follows that $\phi$ is bijective.

#### Remark {#alg-i-s6-n7-rem-1 .statement}

(1) Let G be a finite group and $p$ a prime number. By no. 6, Theorem 3 (a) and no. 6, Theorem 2, the following conditions are equivalent:
(i) there exists a normal Sylow $p$-subgroup of G;
(ii) every Sylow $p$-subgroup of G is normal;
(iii) there exists only one Sylow $p$-subgroup of G.

(2) Let G be a nilpotent finite group. Let I be the set of prime divisors of Card(G). By Theorem 4 and Remark 1, $G = \prod_{p \in I} G_p$, where $G_p$ is the unique Sylow $p$-group of G.

(3) Applied to commutative groups, Theorem 4 gives the decomposition, of commutative finite groups as a product of primary components, which will be studied from another point of view in Chapter VII.

#### Example {#alg-i-s6-n7-exa-1 .statement}

The group $\mathfrak{S}_3$ is of order 6. It contains a normal Sylow 3-subgroup of order 3: the group $A_3$. It contains three Sylow 2-subgroups of order 2: the groups $\{e, \tau\}$, where $\tau$ is a transposition. The group $\mathfrak{S}_3$ is thus not nilpotent.

### Exercises {#alg-i-s6-exercises}

See the [exercises for § 6](exercises/s6/).
