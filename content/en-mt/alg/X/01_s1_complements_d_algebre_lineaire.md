---
book: alg
book_title: Algebra
chapter: X
chapter_title: ALGÈBRE HOMOLOGIQUE
section: 1
section_title: Compléments d’algèbre linéaire
lang: en
source: alg-x-fr
book_pages: A X.168-A X.173
pdf_pages: 0007-0029, 0174-0179
extraction: ocr
subsections:
    - "no": 1
      title: Diagrammes commutatifs
      page: 0
      pdf_page: 7
    - "no": 2
      title: Le diagramme du serpent
      page: 3
      pdf_page: 9
    - "no": 3
      title: Modules plats
      page: 8
      pdf_page: 14
    - "no": 4
      title: Modules de présentation finie
      page: 10
      pdf_page: 16
    - "no": 5
      title: Homomorphismes d’un module de présentation finie
      page: 12
      pdf_page: 18
    - "no": 6
      title: Structure des modules plats
      page: 13
      pdf_page: 19
    - "no": 7
      title: Modules injectifs
      page: 15
      pdf_page: 21
    - "no": 8
      title: Modules cogénérateurs injectifs
      page: 18
      pdf_page: 24
    - "no": 9
      title: Enveloppes injectives
      page: 19
      pdf_page: 25
    - "no": 10
      title: Structure des modules injectifs
      page: 22
      pdf_page: 28
statements: 55
exercises: 17
content_sha256: f55d142614aa6d7f23af6851df91ee735ca380fab8afe681cb5dd6ea12aba4d1
translated_from: content/fr/alg/X/01_s1_complements_d_algebre_lineaire.md
source_lang: fr
translation_method: machine
source_content_sha256: bc19da43004b19055ec3f2c2c05899eaf5dce7177cab8b30104e033843178968
translation_model: gpt-5-mini, gpt-5-6-mini, gpt-5-6
translation_run: translate-en-mt-e853d981
glossary_version: 34
glossary_terms_sha256: 7075ba3f4f9924484909ce32224ec411e1490557c2b56f04599a541c263bcedb
prompt_sha256: 5b9b7144015934413fe8e16b5155e2bc50bed2041525e1b1db7c19a297193094
---

## § 1. COMPLEMENTS OF LINEAR ALGEBRA

In this paragraph, the letter $\mathbf{A}$ denotes a ring. Unless expressly stated otherwise, all the modules considered are left modules, all the ideals considered are left ideals.

The definitions and results apply to right modules, by considering them as left modules over the opposite ring.

If $\mathbf{M}$ is an $\mathbf{A}$-module and if $a \in \mathbf{A}$, we denote by $a_M$ the homothety $x \mapsto ax$ of $\mathbf{M}$. We therefore have $1_M = \mathrm{Id}_M$ (identical mapping of $\mathbf{M}$); when there is no possible ambiguity, one sometimes simply writes $1$ instead of $1_M$.

Finally, we denote by $0$ an $\mathbf{A}$-module reduced to its identity element, chosen once and for all (cf. II, p. 8).

### 1. Commutative diagrams

Let for example B, C, D, E, F be five sets, and let $f$ be a mapping from E into F, $g$ a mapping from B into C, $h$ a mapping from D into E, $u$ a mapping from B into D and $v$ a mapping from C into E. To summarize a situation of this kind, one often makes use of diagrams; for example, the preceding situation will be summarized by the following diagram (E, II, p. 14):

$$
\begin{array}{ccc}
B & \xrightarrow{g} & C \\
u \downarrow & & v \downarrow \\
D & \xrightarrow{h} & E \xrightarrow{f} F .
\end{array}
$$

In such a diagram, the group of signs $E \xrightarrow{f} F$ schematizes the fact that $f$ is a mapping from E into F. When there can be no ambiguity about $f$, the letter $f$ is suppressed, and one simply writes $E \to F$.

When B, C, D, E, F are groups (resp. $\mathbf{A}$-modules) and $f, g, h, u, v$ are group homomorphisms (resp. A-module homomorphisms), one says for short that diagram (1) is a *diagram of groups* (resp. of A-modules).

In principle, a diagram is not a mathematical object, but only a *figure*, intended to facilitate the reading of a reasoning. In practice, diagrams are often used as *abbreviating symbols*, which avoid naming all the sets and all the mappings that one wishes to consider; one thus says “consider diagram (1)” instead of saying: “let B, C, D, E, F be five sets... and $v$ a mapping from C into E”; see for example the statement of prop. 1 of No. 2.

Consider for example the following diagram:

$$
\begin{array}{ccccccc}
B & \xrightarrow{\ f\ } & C & \xrightarrow{\ g\ } & D & \xrightarrow{\ h\ } & E\\
{\scriptstyle b}\downarrow && {\scriptstyle c}\downarrow && {\scriptstyle d}\downarrow && {\scriptstyle e}\downarrow\\
B' & \xrightarrow{\ f'\ } & C' & \xrightarrow{\ g'\ } & D' & \xrightarrow{\ h'\ } & E'
\end{array}
\tag{2}
$$

To every path composed of a certain number of segments of the diagram traversed in the direction indicated by the arrows, one makes correspond a mapping from the set represented by the origin of the first segment into the set represented by the extremity of the last segment, namely the composite of the mappings represented by the various segments traversed. For every vertex of the diagram, for example C, one agrees that there is a path reduced to C and one makes correspond to it the identical mapping $1_C$.

In (2), there are for example three paths starting from B and ending at D$'$; the corresponding mappings are $d\circ g\circ f$, $g'\circ c\circ f$ and $g'\circ f'\circ b$. A diagram is said to be *commutative* if, for every pair of paths of the diagram having the same origin and the same extremity, the two corresponding mappings are equal; in particular if a path has its extremity coinciding with its origin, the corresponding mapping must be the identity.

For diagram (2) to be commutative, it is necessary and sufficient that the relations hold:

$$
\tag{3}
f'\circ b=c\circ f,\qquad
g'\circ c=d\circ g,\qquad
h'\circ d=e\circ h ;
$$

in other words, it is necessary and sufficient that the three square diagrams extracted from (2) be commutative. Indeed, the relations (3) imply $d\circ g\circ f=g'\circ c\circ f$ since $d\circ g=g'\circ c$ and $g'\circ c\circ f=g'\circ f'\circ b$ since $c\circ f=f'\circ b$; therefore the three paths starting from B and ending at D$'$ give the same mapping. One verifies analogously that the four paths starting from B and ending at E$'$ (resp. the three paths starting from C and ending at E$'$) give the same mapping. The relations (3) mean that the two paths starting from B (resp. C, D) and ending at C$'$ (resp. D$'$, E$'$) give the same mapping. All the other pairs of vertices of (2) can be joined by at most one path, and diagram (2) is therefore indeed commutative.

In what follows, we shall leave it to the reader to formulate and verify analogous results for other types of diagrams.

### 2. The snake diagram

#### Proposition 1 {#alg-x-s1-prop-1 .statement}

Consider a commutative diagram of A-modules

$$
\tag{4}
\begin{array}{ccccc}
M & \xrightarrow{u} & N & \xrightarrow{v} & P\\
\downarrow f & & \downarrow g & & \downarrow h\\
M' & \xrightarrow{u'} & N' & \xrightarrow{v'} & P'
\end{array}
$$

Suppose that the two lines of (4) are exact. Then:

(i) If $h$ is injective, one has

$$
\tag{5}
\operatorname{Im}(g)\cap\operatorname{Im}(u')=\operatorname{Im}(u'\circ f)=\operatorname{Im}(g\circ u).
$$

(ii) If $f$ is surjective, one has

$$
\tag{6}
\operatorname{Ker}(g)+\operatorname{Im}(u)=\operatorname{Ker}(v'\circ g)=\operatorname{Ker}(h\circ v).
$$

Let us prove (i). It is clear that one has

$$
\operatorname{Im}(u'\circ f)=\operatorname{Im}(g\circ u)\subset\operatorname{Im}(g)\cap\operatorname{Im}(u').
$$

Inverse support, let $y'\in\operatorname{Im}(g)\cap\operatorname{Im}(u')$. There exists $y\in N$ such that $y'=g(y)$. Since $v'\circ u'=0$, we have $0=v'(y')=v'(g(y))=h(v(y))$, whence $v(y)=0$ since $h$ is injective. Since $(u,v)$ is an exact sequence, there exists $x\in M$ such that $y=u(x)$, whence $y'=g(u(x))$.

Let us prove (ii). Since $v\circ u=0$ and $v'\circ u'=0$, it is clear that

$$
\operatorname{Ker}(g)+\operatorname{Im}(u)\subset\operatorname{Ker}(v'\circ g)=\operatorname{Ker}(h\circ v).
$$

Conversely, let $y\in\operatorname{Ker}(v'\circ g)$. Then $g(y)\in\operatorname{Ker}(v')$, and there exists $x'\in M'$ such that $u'(x')=g(y)$ since the sequence $(u',v')$ is exact. Since $f$ is surjective, there exists $x\in M$ such that $f(x)=x'$, whence $g(y)=u'(f(x))=g(u(x))$; we conclude that $y-u(x)\in\operatorname{Ker}(g)$, which completes the proof.

#### Lemma 1 {#alg-x-s1-lem-1 .statement}

Consider a commutative diagram of A-modules

$$
\tag{7}
\begin{array}{ccc}
M & \xrightarrow{u} & N\\
\downarrow f & & \downarrow g\\
M' & \xrightarrow{u'} & N'
\end{array}
$$

Then there exists one and only one homomorphism $u_1:\operatorname{Ker}(f)\to\operatorname{Ker}(g)$, and one and only one homomorphism $u_2:\operatorname{Coker}(f)\to\operatorname{Coker}(g)$, such that the diagrams

$$
\tag{8}
\begin{array}{ccc}
\operatorname{Ker}(f) & \xrightarrow{u_1} & \operatorname{Ker}(g)\\
\downarrow i & & \downarrow j\\
M & \xrightarrow{u} & N
\end{array}
$$

and

$$
\begin{array}{ccc}
M' & \xrightarrow{u'} & N' \\
p \downarrow & & q \downarrow \\
\text{Coker } (f) & \xrightarrow{u_2} & \text{Coker } (g)
\end{array}
$$

are commutative, $i$ and $j$ denoting the canonical injections, $p$ and $q$ the canonical surjections.

Indeed, if $x \in \text{Ker } (f)$, we have $f(\bar{x}) = 0$ and $g(u(x)) = u'(f(x)) = 0$, hence $u(x) \in \text{Ker } (g)$, and the existence and uniqueness of $u_1$ are then immediate. Similarly, we have
$$
u'(f(M)) = g(u(M)) \subset g(N),
$$
hence $u'$ gives by passing to the quotients a homomorphism
$$
u_2 : \text{Coker } (f) \to \text{Coker } (g),
$$
which is the only homomorphism for which (9) is commutative.

Let us now start from a commutative diagram (4) of A-modules; by virtue of Lemma 1, there corresponds to it a commutative diagram

$$
\begin{array}{ccccccccc}
\text{Ker } (f) & \xrightarrow{u_1} & \text{Ker } (g) & \xrightarrow{v_1} & \text{Ker } (h) \\
i \downarrow & & j \downarrow & & k \downarrow \\
M & \xrightarrow{u} & N & \xrightarrow{v} & P \\
f \downarrow & & g \downarrow & & h \downarrow \\
M' & \xrightarrow{u'} & N' & \xrightarrow{v'} & P' \\
p \downarrow & & q \downarrow & & r \downarrow \\
\text{Coker } (f) & \xrightarrow{u_2} & \text{Coker } (g) & \xrightarrow{v_2} & \text{Coker } (h)
\end{array}
$$

where $i, j, k$ are the canonical injections, $p, q, r$ the canonical surjections, $u_1, u_2$ (resp. $v_1, v_2$) the homomorphisms deduced from $u, u'$ (resp. $v, v'$) by Lemma 1.

#### Proposition 2 {#alg-x-s1-prop-2 .statement}

Suppose that in the commutative diagram (4), the sequences $(u, v)$ and $(u', v')$ are exact. Then:
(i) We have $v_1 \circ u_1 = 0$; if $u'$ is injective, the sequence $(u_1, v_1)$ is exact.
(ii) We have $v_2 \circ u_2 = 0$; if $v$ is surjective, the sequence $(u_2, v_2)$ is exact.
(iii) Suppose that $u'$ is injective and $v$ is surjective. There exists then one and only one homomorphism $d : \text{Ker } (h) \to \text{Coker } (f)$ having the following property: if $z \in \text{Ker } (h), y \in N$ and $x' \in M'$ satisfy the relations $v(y) = k(z)$ and $u'(x') = g(y)$, we have $d(z) = p(x')$. Moreover the sequence
(*) $\text{Ker } (f) \xrightarrow{u_1} \text{Ker } (g) \xrightarrow{v_1} \text{Ker } (h) \xrightarrow{d} \text{Coker } (f) \xrightarrow{u_2} \text{Coker } (g) \xrightarrow{v_2} \text{Coker } (h)$
is exact.

$$
\begin{array}{ccccc}
\operatorname{Ker}(f)&\xrightarrow{u_1}&\operatorname{Ker}(g)&\xrightarrow{v_1}&\operatorname{Ker}(h)\\
\downarrow\scriptstyle i&&\downarrow\scriptstyle j&&\downarrow\scriptstyle k\\
M&\xrightarrow{u}&N&\xrightarrow{v}&P\\
\downarrow\scriptstyle f&&\downarrow\scriptstyle g&&\downarrow\scriptstyle h\\
M'&\xrightarrow{u'}&N'&\xrightarrow{v'}&P'\\
\downarrow\scriptstyle p&&\downarrow\scriptstyle q&&\downarrow\scriptstyle r\\
\operatorname{Coker}(f)&\xrightarrow{u_2}&\operatorname{Coker}(g)&\xrightarrow{v_2}&\operatorname{Coker}(h)
\end{array}
$$

Let us prove (i). Since $u_1$ and $v_1$ have the same graphs as the restrictions of $u$ and $v$ to $\operatorname{Ker}(f)$ and $\operatorname{Ker}(g)$ respectively, we have $v_1\circ u_1=0$. We have

$$
\operatorname{Ker}(v_1)=\operatorname{Ker}(g)\cap\operatorname{Ker}(v)=\operatorname{Ker}(g)\cap\operatorname{Im}(u)=\operatorname{Im}(j)\cap\operatorname{Im}(u).
$$

But by prop. 1 (i), we have $\operatorname{Ker}(v_1)=\operatorname{Im}(j\circ u_1)=\operatorname{Im}(u_1)$ if $u'$ is injective.

Let us prove (ii). Since $u_2$ and $v_2$ are obtained from $u$ and $v$ by passing to quotients, it is clear that $v_2\circ u_2=0$. Suppose that $v$ is surjective; since $q$ and $p$ are surjective, we have, by virtue of the hypotheses and prop. 1 (ii)

$$
\begin{aligned}
\operatorname{Ker}(v_2)&=q(\operatorname{Ker}(v_2\circ q))=q(\operatorname{Ker}(v')+\operatorname{Im}(g))=q(\operatorname{Ker}(v'))\\
&=q(\operatorname{Im}(u'))=\operatorname{Im}(q\circ u')=\operatorname{Im}(u_2\circ p)=\operatorname{Im}(u_2).
\end{aligned}
$$

Let us finally prove (iii). For $z\in\operatorname{Ker}(h)$, there exists $y\in N$ such that $v(y)=k(z)$ since $v$ is surjective; moreover, we have $v'(g(y))=h(k(z))=0$, and consequently there exists a unique $x'\in M'$ such that $u'(x')=g(y)$ since $u'$ is injective. Let us show that the element $p(x')\in\operatorname{Coker}(f)$ is independent of the element $y\in N$ such that $v(y)=k(z)$. Indeed, if $y_1\in N$ is a second element such that $v(y_1)=k(z)$, we have $y_1=y+u(x)$ where $x\in M$; let us show that if $x'_1\in M'$ is such that $u'(x'_1)=g(y_1)$, we have $x'_1=x'+f(x)$; indeed, we have $u'(x'+f(x))=u'(x')+u'(f(x))=g(y)+g(u(x))=g(y+u(x))=g(y_1)$. Finally, we conclude that $p(x'_1)=p(x')+p(f(x))=p(x')$. We can therefore set $d(z)=p(x')$ and we have thus defined a mapping $d:\operatorname{Ker}(h)\to\operatorname{Coker}(f)$.

If now $z_1,z_2$ are elements of $\operatorname{Ker}(h)$, if $\lambda_1,\lambda_2\in A$ and $z=\lambda_1z_1+\lambda_2z_2$, we take elements $y_1$ and $y_2$ of $N$ such that $v(y_1)=k(z_1)$ and $v(y_2)=k(z_2)$ and we choose for $y\in N$ the element $\lambda_1y_1+\lambda_2y_2$; it is then immediate that

$$
d(z)=\lambda_1d(z_1)+\lambda_2d(z_2),
$$

so $d$ is a homomorphism.

Suppose that $z=v_1(t)$ for some $t\in\operatorname{Ker}(g)$; we then take for $y\in N$ the element $j(t)$. Since $g(j(t))=0$, we conclude that $d(z)=0$, hence $d\circ v_1=0$. Conversely, suppose that $d(z)=0$. With the preceding notations, we thus have $x'=f(x)$, where x ∈ M. In this case, we have $g(y) = u'(f(x)) = g(u(x))$, or equivalently $g(y - u(x)) = 0$. The element $y - u(x)$ is therefore of the form $j(n)$ for $n \in \mathrm{Ker}\,(g)$, and we have

$$
k(z) = v(y) = v(u(x) + j(n)) = v(j(n)) = k(v_1(n));
$$

as $k$ is injective, $z = v_1(n)$, which proves that the sequence (*) is exact at $\mathrm{Ker}\,(h)$.

Finally, we have (with the same notations)

$$
u_2(d(z)) = u_2(p(x')) = q(u'(x')) = q(g(y)) = 0 \quad \text{therefore} \quad u_2 \circ d = 0 .
$$

Conversely, suppose that an element $w = p(x')$ of $\mathrm{Coker}\,(f)$ is such that

$$
u_2(w) = u_2(p(x')) = 0 \quad (\text{with } x' \in \mathbf{M}') .
$$

We thus have $q(u'(x')) = 0$, and consequently $u'(x') = g(y)$ for a $y \in \mathbf{N}$; since $v'(u'(x')) = 0$, we have $v'(g(y)) = 0$, hence $h(v(y)) = 0$, in other words $v(y) = k(z)$ for a $z \in \mathrm{Ker}\,(h)$, and by definition $w = d(z)$, which shows that the sequence (*) is exact at $\mathrm{Coker}\,(f)$. We have seen in (i) that it is exact at $\mathrm{Ker}\,(g)$ and in (ii) that it is exact at $\mathrm{Coker}\,(g)$, which completes the proving of (iii).

#### Corollary 1 {#alg-x-s1-prop-2-cor-1 .statement}

Suppose that the diagram (4) is commutative and has exact rows. Then:

(i) If $u', f$ and $h$ are injective, $g$ is injective.
(ii) If $v, f$ and $h$ are surjective, $g$ is surjective.

Assertion (i) is a consequence of assertion (i) of prop. 2: indeed we have $\mathrm{Ker}\,(f) = 0$ and $\mathrm{Ker}\,(h) = 0$, hence $\mathrm{Ker}\,(g) = 0$.

Assertion (ii) is a consequence of assertion (ii) of prop. 2: indeed, we have $\mathrm{Coker}\,(f) = 0$ and $\mathrm{Coker}\,(h) = 0$, hence $\mathrm{Coker}\,(g) = 0$.

#### Corollary 2 {#alg-x-s1-prop-2-cor-2 .statement}

Suppose that the diagram (4) is commutative and has exact rows. Under these conditions:

(i) If $g$ is injective and if $f$ and $v$ are surjective, then $h$ is injective.
(ii) If $g$ is surjective and if $h$ and $u'$ are injective, then $f$ is surjective.

To prove (i), consider the diagram

$$
\begin{array}{ccccc}
u(\mathbf{M}) & \xrightarrow{w} & \mathbf{N} & \xrightarrow{v} & \mathbf{P} \\
f' \downarrow & & g \downarrow & & h \downarrow \\
u'(\mathbf{M}') & \xrightarrow{w'} & \mathbf{N}' & \xrightarrow{v'} & \mathbf{P}'
\end{array}
$$

where $f'$ is the mapping having the same graph as the restriction of $g$ to $u(\mathbf{M})$, $w$ and $w'$ being the canonical injections; it is clear that this diagram is commutative and has exact rows. Moreover $w'$ is injective, and by assumption $v$ is surjective; we therefore have, by prop. 2 (iii), an exact sequence

$$
\mathrm{Ker}\,(g) \longrightarrow \mathrm{Ker}\,(h) \xrightarrow{d} \mathrm{Coker}\,(f');
$$

since $g$ is injective and $f'$ is surjective, we therefore have $\mathrm{Ker}\,(h) = 0$.

To prove (ii), consider the diagram

$$
\begin{array}{ccccc}
M&\xrightarrow{u}&N&\xrightarrow{w}&\nu(N)\\
{\scriptstyle f}\downarrow&&{\scriptstyle g}\downarrow&&{\scriptstyle h'}\downarrow\\
M'&\xrightarrow{u'}&N'&\xrightarrow{w'}&\nu'(N')
\end{array}
$$

where this time $h'$ is the mapping having the same graph as the restriction of $h$ to $\nu(N)$, and $w$ and $w'$ have respectively the same graphs as $\nu$ and $\nu'$; this diagram is commutative and its rows are exact. Moreover $w$ is surjective and by assumption $u'$ is injective; we therefore have, by prop. 2 (iii), an exact sequence

$$
\operatorname{Ker}(h')\xrightarrow{d}\operatorname{Coker}(f)\longrightarrow\operatorname{Coker}(g);
$$

since $g$ is surjective and $h'$ is injective, we therefore have $\operatorname{Coker}(f)=0$.

**Corollary 3 (Five Lemma).** — Consider a commutative diagram of $A$-modules

$$
\begin{array}{ccccccccc}
M_1&\xrightarrow{u_1}&M_2&\xrightarrow{u_2}&M_3&\xrightarrow{u_3}&M_4&\xrightarrow{u_4}&M_5\\
{\scriptstyle f_1}\downarrow&&{\scriptstyle f_2}\downarrow&&{\scriptstyle f_3}\downarrow&&{\scriptstyle f_4}\downarrow&&{\scriptstyle f_5}\downarrow\\
M'_1&\xrightarrow{u'_1}&M'_2&\xrightarrow{u'_2}&M'_3&\xrightarrow{u'_3}&M'_4&\xrightarrow{u'_4}&M'_5
\end{array}
$$

where the rows are exact.

(i) If $f_2$ and $f_4$ are injective and $f_1$ surjective, $f_3$ is injective.

(ii) If $f_2$ and $f_4$ are surjective and $f_5$ injective, $f_3$ is surjective.

In particular, if $f_1$, $f_2$, $f_4$ and $f_5$ are isomorphisms, the same is true of $f_3$.

To prove (i), put $\widetilde M_2=\operatorname{Coker}(u_1)$, $\widetilde M'_2=\operatorname{Coker}(u'_1)$ and denote by $\widetilde f_2:\widetilde M_2\to\widetilde M'_2$ the mapping deduced from $f_2$. It follows from cor. 2 (i) that $\widetilde f_2$ is injective. Applying cor. 1 (i) to the diagram

$$
\begin{array}{ccccc}
\widetilde M_2&\xrightarrow{\widetilde u_2}&M_3&\xrightarrow{u_3}&M_4\\
{\scriptstyle \widetilde f_2}\downarrow&&{\scriptstyle f_3}\downarrow&&{\scriptstyle f_4}\downarrow\\
\widetilde M'_2&\xrightarrow{\widetilde u'_2}&M'_3&\xrightarrow{u'_3}&M'_4
\end{array}
$$

where $\widetilde u_2$ and $\widetilde u'_2$ are deduced from $u_2$ and $u'_2$, we see that $f_3$ is injective.

To prove (ii), set $\widetilde M_4=\operatorname{Ker}(u_4)$, $\widetilde M'_4=\operatorname{Ker}(u'_4)$ and denote by $\widetilde f_4:\widetilde M_4\to\widetilde M'_4$ the mapping induced by $f_4$. It follows from cor. 2 (ii) that $\widetilde f_4$ is surjective. Applying cor. 1 (ii) to the diagram

$$
\begin{array}{ccccc}
M_2&\xrightarrow{u_2}&M_3&\xrightarrow{\widetilde u_3}&\widetilde M_4\\
{\scriptstyle f_2}\downarrow&&{\scriptstyle f_3}\downarrow&&{\scriptstyle \widetilde f_4}\downarrow\\
M'_2&\xrightarrow{u'_2}&M'_3&\xrightarrow{\widetilde u'_3}&\widetilde M'_4
\end{array}
$$

where $\widetilde u_3$ and $\widetilde u'_3$ have the same graph as $u_3$ and $u'_3$, one sees that $f_3$ is surjective.

### 3. Flat modules

#### Definition 1 {#alg-x-s1-def-1 .statement}

One says that the a-module E is flat if, for every exact sequence of right a-modules and homomorphisms

(11) $M' \xrightarrow{u} M \xrightarrow{v} M''$,

the sequence of $\mathbf{Z}$-linear mappings

(12) $M' \otimes_A E \xrightarrow{u \otimes 1} M \otimes_A E \xrightarrow{v \otimes 1} M'' \otimes_A E$

is exact.

#### Proposition 3 {#alg-x-s1-prop-3 .statement}

In order that the a-module E be flat, it is necessary and sufficient that, for every injective A-homomorphism $u : M' \to M$ of right A-modules, the mapping $u \otimes 1 : M' \otimes_A E \to M \otimes_A E$ be injective.

If E is flat and $u : M' \to M$ is injective, the sequence $0 \to M' \xrightarrow{u} M$ is exact, hence also the sequence $0 \longrightarrow M' \otimes_A E \xrightarrow{u \otimes 1} M \otimes_A E$, and $u \otimes 1$ is injective. Conversely, consider the exact sequence (11); put $M''_1 = v(M)$, and let $i : M''_1 \to M''$ be the canonical injection and $p : M \to M''_1$ the mapping $m \mapsto v(m)$. The sequence $M' \xrightarrow{u} M \xrightarrow{p} M''_1 \longrightarrow 0$ is exact; according to II, p. 58, prop. 5, the sequence $M' \otimes_A E \xrightarrow{u \otimes 1} M \otimes_A E \xrightarrow{p \otimes 1} M''_1 \otimes_A E$ is therefore exact. Moreover, one has $v = i \circ p$, hence $(v \otimes 1) = (i \otimes 1) \circ (p \otimes 1)$; if E satisfies the condition of the statement, then $i \otimes 1$ is injective, hence

$$
\operatorname{Ker}(v \otimes 1) = \operatorname{Ker}(p \otimes 1) = \operatorname{Im}(u \otimes 1)
$$

and the sequence (12) is exact.

#### Proposition 4 {#alg-x-s1-prop-4 .statement}

(i) Let $(E_i)_{i \in I}$ be a family of a-modules, $E = \bigoplus_{i \in I} E_i$ their direct sum. In order that the a-module E be flat, it is necessary and sufficient that each of the $E_i$ be so.

(ii) Let I be a right filtered preordered set, $(E_\alpha, f_{\beta \alpha})$ an inductive system of a-modules relative to I, $E = \varinjlim E_\alpha$ its inductive limit. If each of the a-modules $E_\alpha$ is flat, then E is flat.

Let $M' \to M \to M''$ be an exact sequence of right a-modules.

(i) In order that the sequence $\bigoplus_{i \in I} (M' \otimes_A E_i) \to \bigoplus_{i \in I} (M \otimes_A E_i) \to \bigoplus_{i \in I} (M'' \otimes_A E_i)$ be exact, it is necessary and sufficient that each of the sequences $M' \otimes_A E_i \to M \otimes_A E_i \to M'' \otimes_A E_i$ be so (II, p. 13, prop. 7), which proves (i) since $\bigoplus (M \otimes_A E_i)$ identifies canonically with $M \otimes_A E$ (II, p. 61, prop. 7).

(ii) By assumption, each of the sequences $M' \otimes_A E_i \to M \otimes_A E_i \to M'' \otimes_A E_i$ is exact, and hence so is the sequence $M' \otimes_A E \to M \otimes_A E \to M'' \otimes_A E$, since passage to the inductive limit commutes with the tensor product (II, p. 93, prop. 7) and preserves exactness (II, p. 91, prop. 3).

#### Example 1 {#alg-x-s1-n3-exa-1 .statement}

It is clear that $A_s$ is a flat $A$-module; it follows then from prop. 4 (i) that every free $A$-module, and more generally every projective $A$-module, is flat (see also II, p. 63, cor. 6).

\* Conversely, every finitely presented flat $A$-module is projective (No. 5). \*

#### Example 2 {#alg-x-s1-n3-exa-2 .statement}

According to prop. 4 (ii), every $A$-module which is an inductive limit of a filtered inductive system of free $A$-modules is flat. We shall prove a converse at No. 6.

#### Example 3 {#alg-x-s1-n3-exa-3 .statement}

If $A$ is semisimple, every $A$-module is projective (VIII, § 5, No. 1, prop. 1), hence flat.

#### Example 4 {#alg-x-s1-n3-exa-4 .statement}

\* If $A$ is an artinian local ring (not necessarily commutative), an $A$-module is flat if and only if it is free (AC II, § 3, No. 2, cor. 2 of prop. 5). \*

#### Example 5 {#alg-x-s1-n3-exa-5 .statement}

If $A$ is integral, the field of fractions $K$ of $A$ is a flat $A$-module (II, p. 118, prop. 27).

#### Example 6 {#alg-x-s1-n3-exa-6 .statement}

*In AC II and III, we shall study two important examples of $A$-modules flat when $A$ is commutative: the rings of fractions $S^{-1} A$, and, when $A$ is noetherian, the separated completions of $A$ for the J-adic topologies.*

#### Example 7 {#alg-x-s1-n3-exa-7 .statement}

Let $a \in A$ be such that the mapping $a_A : x \mapsto ax$ of $A$ into $A$ is injective (“$a$ is not a left divisor of 0”). If $E$ is a flat $A$-module, then the homothety $a_E$ is injective, since it is identified with $a_A \otimes 1 : A_d \otimes_A E \to A_d \otimes_A E$. In particular, if $A$ is integral, every flat $A$-module is without torsion. Conversely, if $A$ is principal, every torsion-free $A$-module is flat: indeed, if the $A$-module $E$ is without torsion, every finitely generated submodule of $E$ is free (VII, § 4, No. 4, Cor. 2 to Theorem 4), and $E$ is a filtered increasing union of flat submodules, hence is flat (Prop. 4 (ii)).

#### Example 8 {#alg-x-s1-n3-exa-8 .statement}

Let $B$ be a ring and $\rho : A \to B$ a homomorphism. If $E$ is a flat $A$-module, the $B$-module $E_{(B)} = B \otimes_A E$ is flat. Indeed, let $u : N' \to N$ be an injective homomorphism of right $B$-modules; then $u \otimes_B 1_{E_{(B)}}$ is canonically identified with the homomorphism $u \otimes_A 1_E : N' \otimes_A E \to N \otimes_A E$, which is injective if $E$ is flat.

#### Example 9 {#alg-x-s1-n3-exa-9 .statement}

Suppose that $A = K[X, Y]$, where $K$ is a field. Then the maximal ideal $m$ generated by $X$ and $Y$ is a torsion-free $A$-module, but not flat. Consider indeed the ring $B = A/(Y)$, which is isomorphic to $K[X]$, hence integral. The $B$-module $m_{(B)}$ is isomorphic to $m/Ym = (X, Y)/(XY, Y^2)$ in which the class of $Y$ is torsion. Consequently, $m_{(B)}$ is not a flat $B$-module, hence $m$ is not flat.

#### Example 10 {#alg-x-s1-n3-exa-10 .statement}

Suppose $A$ is commutative. Let $B$ be the algebra $A[X_1, ..., X_n]/(P)$, where $P$ is a nonzero polynomial. For every prime ideal $p$ of $A$, denote by $\kappa(p)$ the field of fractions of the integral ring $A/p$, by $E(p)$ the algebra $\kappa(p)[X_1, ..., X_n]$ and by $P(p)$ the image of $P$ in $E(p)$ by the canonical mapping.

We can show that, in order that $B$ be a $A$-module flat, it suffices that $P(p) \neq 0$ for every prime ideal $p$ of $A$. If $A$ is integral, this condition is necessary.

\* In geometric language, consider the projection $\pi : \mathrm{Spec}(B) \to \mathrm{Spec}(A)$. For every $p \in \mathrm{Spec}(A)$, the fibre $\pi^{-1}(p)$ is identified with the subvariety $V_p$ of the affine space $\mathbf{A}_{\kappa(p)}^n = \mathrm{Spec}(E(p))$ defined by $P(p)$, and the set $F$ of the $p$ for which this subvariety is the whole space (*i.e.* for which $P(p) = 0$) is a closed set of

Spec (A). The preceding condition means that this closed set is empty, in other words that for every $p$ the subvariety $V_p$ is a hypersurface in $\mathbf{A}_{k(p)}^n$.

#### Example 11 {#alg-x-s1-n3-exa-11 .statement}

\* Let S and X be two complex analytic spaces and let $f : X \to S$ be a morphism. We say that $f$ is flat at a point $x$ of X if $\mathcal{O}_{X,x}$, considered as $\mathcal{O}_{S,f(x)}$-module by means of the homomorphism $f^* : \mathcal{O}_{S,f(x)} \to \mathcal{O}_{X,x}$, is flat. The set of points of X where $f$ is flat is an open set of X, and the restriction of $f$ to this open set is an open mapping. If X and S are connected analytic varieties of finite dimension, $f$ is flat (at every point of X) if and only if $f(X)$ is open in S and the fibres $f^{-1}(s)$, for $s \in f(X)$, all have the same dimension. \*

### 4. Modules of finite presentation

A presentation (or presentation of length 1) of an $A$-module E is called an exact sequence

$$
L_1 \to L_0 \to E \to 0
$$

of A-modules where $L_0$ and $L_1$ are free.

Every A-module E admits a presentation. Indeed, we know (II, p. 27, prop. 20) that there exists a surjective homomorphism $u : L_0 \to E$, where $L_0$ is free; if R is the kernel of $u$, there exists analogously a surjective homomorphism $v : L_1 \to R$ where $L_1$ is free. If one considers $v$ as a homomorphism from $L_1$ into $L_0$, the sequence $L_1 \xrightarrow{v} L_0 \xrightarrow{u} E \to 0$ is exact by definition, whence our assertion.

If $\rho : A \to B$ is a homomorphism of rings, every presentation (13) of E provides a presentation of $E_{(B)} = B \otimes_A E$:

$$
B \otimes_A L_1 \to B \otimes_A L_0 \to B \otimes_A E \to 0
$$

by virtue of II, p. 58, prop. 5 and the fact that $B \otimes_A L$ is a B-module free when L is free.

On says that a presentation (13) of a module E is finite if the free modules $L_0$ and $L_1$ have finite bases. It is clear that if the presentation (13) is finite, the same is true of the presentation (14). We say that E is an a-module of finite presentation if it admits a finite presentation.

#### Proposition 5 {#alg-x-s1-prop-5 .statement}

(i) Every module admitting a finite presentation is finitely generated.
(ii) If A is a left noetherian ring, every finitely generated a-module admits a finite presentation.
(iii) Every finitely generated projective module admits a finite presentation.

Assertion (i) follows trivially from the definitions. Suppose A is left noetherian and E is finitely generated. There then exists a surjective homomorphism $u : L_0 \to E$, where $L_0$ is a free a-module having a finite basis; the kernel R of $u$ is finitely generated, hence there is a surjective homomorphism $v : L_1 \to R$ where $L_1$ is free with finite basis, and the exact sequence $L_1 \xrightarrow{v} L_0 \xrightarrow{u} E \to 0$ is a finite presentation of E; whence (ii).

Finally, suppose that E is a finitely generated projective module; it is then a direct factor of a finitely generated free module L_0 (II, p. 40, cor. 1); the kernel R of the surjective homomorphism L_0 → E is then isomorphic to a quotient of L_0, hence is finitely generated, and we conclude as above.

#### Proposition 6 {#alg-x-s1-prop-6 .statement}

Let A be a ring, E an a-module of finite presentation. For every exact sequence

$$
0 \to F \xrightarrow{j} G \xrightarrow{p} E \to 0
$$

where G is finitely generated, the module F is finitely generated.

Let L_1 \xrightarrow{r} L_0 \xrightarrow{s} E \to 0 be a finite presentation; if (e_i) is a basis of L_0, there exists for each i an element g_i \in G such that p(g_i) = s(e_i) ; the homomorphism u : L_0 \to G such that u(e_i) = g_i for all i is therefore such that s = p \circ u. Since s \circ r = 0, we have u(r(L_1)) \subset \mathrm{Ker}\ p, and since Ker p is isomorphic to F, we see that there is a homomorphism v : L_1 \to F such that the diagram

$$
\begin{array}{ccccccc}
L_1 & \xrightarrow{r} & L_0 & \xrightarrow{s} & E & \to & 0 \\
v \downarrow & & u \downarrow & & 1_E \downarrow & & \\
F & \xrightarrow{j} & G & \xrightarrow{p} & E & \to & 0
\end{array}
$$

is commutative. Since j is injective and s surjective, we can apply Proposition 2 of X, p. 4, in other words there is an exact sequence

$$
\mathrm{Ker}\ 1_E \xrightarrow{d} \mathrm{Coker}\ v \to \mathrm{Coker}\ u \to \mathrm{Coker}\ 1_E.
$$

This shows that Coker v is isomorphic to G/u(L_0), which is finitely generated by assumption. We have in addition the exact sequence

$$
0 \to v(L_1) \to F \to \mathrm{Coker}\ v \to 0
$$

and since v(L_1) and Coker v are finitely generated, the same is true of F (II, p. 17, cor. 5).

#### Proposition 7 {#alg-x-s1-prop-7 .statement}

Let M be an a-module. There exists an ordered set I inductive to the right and an inductive system of a-modules of finite presentation $(M_\alpha, \varphi_{\beta\alpha})$ relative to I such that M is isomorphic to $\lim_\alpha M_\alpha$. If M possesses a generating system of n elements, we can suppose that the same is true of the $M_\alpha$.

Consider a presentation

$$
A_s^{(K)} \xrightarrow{u} A_s^{(L)} \xrightarrow{v} M \to 0 ;
$$

let I be the set of pairs $\alpha = (K', L')$, where K' (resp. L') is a finite subset of K (resp.L), such that u induces a mapping u_\alpha from the submodule $A_s^{K'}$ of $A_s^{(K)}$ into the submodule $A_s^{L'}$ of $A_s^{(L)}$ ; for $\alpha \in I$, let $M_\alpha$ be the cokernel of $u_\alpha$ and $v_\alpha : A_s^{L'} \to M_\alpha$ the canonical mapping, so that we have a commutative diagram with exact rows:

$$
\begin{array}{ccccccc}
A_s^{(K)} & \xrightarrow{u} & A_s^{(L)} & \xrightarrow{l} & M & \to & 0 \\
i_\alpha \uparrow & & j_\alpha \uparrow & & f_\alpha \uparrow \\
A_s^{K'} & \xrightarrow{u_\alpha} & A_s^{L'} & \xrightarrow{v_\alpha} & M_\alpha & \to & 0 ,
\end{array}
$$

where $i_\alpha$ and $j_\alpha$ are the canonical injections, and where $f_\alpha$ is deduced from $j_\alpha$ by passing to quotients. We order the set I by the relation

$$
\alpha = (K',L') \leq \beta = (K'',L'') \quad \text{si}\quad K' \subset K'',\quad L' \subset L'' ;
$$

for $\alpha\leq\beta$, let $\varphi_{\beta\alpha}:M_\alpha\longrightarrow M_\beta$ be the homomorphism deduced by passing to quotients from the inclusion of $A_s^{L'}$ in $A_s^{L''}$. One verifies immediately that the ordered set I is inductive, that $(M_\alpha,\varphi_{\beta\alpha})$ is an inductive system of a-modules and that $(\varphi_\alpha)$ is an inductive system of a-homomorphisms. By passing to the inductive limit, we obtain a commutative diagram

$$
\begin{array}{ccccc}
A_s^{(K)} & \xrightarrow{u} & A_s^{(L)} & \xrightarrow{v} & M \longrightarrow 0\\
\uparrow\scriptstyle i && \uparrow\scriptstyle j && \uparrow\scriptstyle\varphi\\
\underset{\longrightarrow}{\lim}\,A_s^{K'} & \longrightarrow & \underset{\longrightarrow}{\lim}\,A_s^{L'} & \longrightarrow & \underset{\longrightarrow}{\lim}\,M_\alpha \longrightarrow 0
\end{array}
\tag{15}
$$

the rows of this diagram are exact (II, p. 91, prop. 3); since $i$ and $j$ are bijective, $\varphi$ is so also (X, p. 7, cor. 3), whence the proposition.

### 5. Homomorphisms of a module of finite presentation

Let E be an a-module. If I is a preordered inductive set and $(G_i,u_{ji})$ is an inductive system of a-modules relative to I, the canonical mappings $G_i\longrightarrow\underset{\longrightarrow}{\lim}\,G_i$ induce homomorphisms $\operatorname{Hom}_A(E,G_i)\longrightarrow\operatorname{Hom}_A(E,\underset{\longrightarrow}{\lim}\,G_i)$, whence a homomorphism called *canonical*

$$
\underset{\substack{\longrightarrow\\ i\in I}}{\lim}\operatorname{Hom}_A(E,G_i)
\longrightarrow
\operatorname{Hom}_A\left(E,\underset{\substack{\longrightarrow\\ i\in I}}{\lim}G_i\right).
\tag{16}
$$

Let B be another ring, F a B-module, G an (A, B)-bimodule; a canonical homomorphism has been defined in II, p. 75:

$$
\operatorname{Hom}_A(E,G)\otimes_B F
\longrightarrow
\operatorname{Hom}_A(E,G\otimes_B F).
\tag{17}
$$

#### Proposition 8 {#alg-x-s1-prop-8 .statement}

a) *If the A-module E is of finite type (resp. of finite presentation), the canonical homomorphism (16) is injective (resp. bijective).*

*b) Suppose that the B-module F is flat; if the A-module E is of finite type (resp. of finite presentation), the canonical homomorphism (17) is injective (resp. bijective).*

Let us prove for example b), the proof of a) being analogous. Consider A, B, F, G as fixed, and, for every right A-module E, put

$$
T(E)=\operatorname{Hom}_A(E,G)\otimes_B F,\qquad
T'(E)=\operatorname{Hom}_A(E,G\otimes_B F)
$$

and denote by $\nu_E$ the homomorphism (17); for every homomorphism $v:E\to E'$ of right A-modules, put $T(v)=\operatorname{Hom}(v,1_G)\otimes 1_F$ and $T'(v)=\operatorname{Hom}(v,1_G\otimes 1_F)$.

Let $L_1 \xrightarrow{v} L_0 \xrightarrow{w} E \to 0$ be a presentation of $E$; we suppose the free module $L_0$ (resp. the free modules $L_0$ and $L_1$) *of finite type*. The diagram

$$
\begin{array}{ccccccc}
0 & \to & T(E) & \xrightarrow{T(w)} & T(L_0) & \xrightarrow{T(v)} & T(L_1) \\
& & v_E \downarrow & & v_{L_0} \downarrow & & v_{L_1} \downarrow \\
0 & \to & T'(E) & \xrightarrow{T'(w)} & T'(L_0) & \xrightarrow{T'(v)} & T'(L_1)
\end{array}
$$

is commutative, and its second line is exact (II, p. 36, th. 1); moreover, the sequence

$$
0 \to \mathrm{Hom}_A(E, G) \to \mathrm{Hom}_A(L_0, G) \to \mathrm{Hom}_A(L_1, G)
$$

is exact (*loc. cit.*), and since $F$ is *flat*, the first line of (18) is also an exact sequence (X, p. 8, déf. 1). This being so, we know that $v_{L_0}$ is bijective (resp. that $v_{L_0}$ and $v_{L_1}$ are bijective) (II, p. 75, prop. 2). If we suppose only that $v_{L_0}$ is bijective, it follows from (18) that $v_{L_0} \circ T(w) = T'(w) \circ v_E$ is injective, hence $v_E$ is so also. If we suppose that $v_{L_0}$ and $v_{L_1}$ are both bijective, we deduce from cor. 2 (ii) of X, p. 6 that $v_E$ is surjective, and since we have just seen that $v_E$ is injective, it is bijective.

**COROLLARY. — Every flat module of finite presentation is projective.**

Indeed, let $E$ be a flat and of finite presentation $A$-module. Applying (*b*) to the case $B = A, G = {}_sA_d, F = E$, we see that the canonical homomorphism

$$
\mathrm{Hom}_A(E, A) \otimes_A E \to \mathrm{Hom}_A(E, E)
$$

is surjective. This implies that $E$ is projective (II, p. 77, remark 1).

According to the preceding corollary and prop. 5 of X, p. 10, there is an identity between flat modules of finite presentation and projective modules of finite type. On the other hand, there exist flat modules of finite type which are not of finite presentation, hence which are not projective (*cf.* X, p. 170, exercise 17, see however X, p. 169, exercises 13 and 14).

### 6. Structure of flat modules

**Lemma 2. — Let I be a right filtered ordered set, $(E_\alpha, \varphi_{\beta\alpha})$ an inductive system of sets relative to I, E its inductive limit and $\varphi_\alpha : E_\alpha \to E, \alpha \in I$, the canonical mappings. Let $f : I \to I$ be a mapping such that $f(\alpha) > \alpha$ for $\alpha \in I$, and suppose given, for each $\alpha \in I$, a set $L_\alpha$ and mappings $u_\alpha : E_\alpha \to L_\alpha$ and $v_\alpha : L_\alpha \to E_{f(\alpha)}$ such that $v_\alpha \circ u'_\alpha = \varphi_{f(\alpha), \alpha}$. Let J be the ordered set obtained by providing I with the relation « $\alpha \leq \beta$ if $\alpha = \beta$ or $f(\alpha) \leq \beta$ ». If $\alpha, \beta \in J$ with $\alpha \leq \beta$, let $\psi_{\beta\alpha} : L_\alpha \to L_\beta$ be the mapping such that $\psi_{\beta\alpha} = \mathrm{Id}$ if $\alpha = \beta$, $\psi_{\beta\alpha} = u_\beta \circ \varphi_{\beta, f(\alpha)} \circ v_\alpha$ if $f(\alpha) \leq \beta$. If $\alpha \in J$, let $\psi_\alpha : L_\alpha \to E$ be the mapping $\varphi_{f(\alpha)} \circ v_\alpha$. Then the ordered set J is filtered, $(L_\alpha, \psi_{\beta\alpha})$ is an inductive system relative to J, $(\psi_\alpha)$ is an inductive system of mappings and the mapping $\psi : \lim_{\alpha \in J} L_\alpha \to E$ deduced from the $\psi_\alpha$ is bijective.**

It is clear that J is inductive. If $\alpha, \beta \in J$ with $\alpha < \beta$, we have
$$
\psi_\beta \circ \psi_{\beta \alpha} = \varphi_{f(\beta)} \circ v_\beta \circ u_\beta \circ \varphi_{\beta, f(\alpha)} \circ v_\alpha \\
= \varphi_{f(\beta)} \circ \varphi_{f(\beta), \beta} \circ \varphi_{\beta, f(\alpha)} \circ v_\alpha = \varphi_{f(\alpha)} \circ v_\alpha = \psi_\alpha ;
$$
analogously, if $\alpha, \beta, \gamma \in J$ with $\alpha < \beta < \gamma$, we have
$$
\psi_{\gamma \beta} \circ \psi_{\beta \alpha} = u_\gamma \circ \varphi_{\gamma, f(\beta)} \circ v_\beta \circ u_\beta \circ \varphi_{\beta, f(\alpha)} \circ v_\alpha \\
= u_\gamma \circ \varphi_{\gamma, f(\beta)} \circ \varphi_{f(\beta), \beta} \circ \varphi_{\beta, f(\alpha)} \circ v_\alpha = u_\gamma \circ \varphi_{\gamma, f(\alpha)} \circ v_\alpha = \psi_{\gamma \alpha} .
$$
Let us prove the last assertion: for each $\alpha \in J$, we have
$$
\psi_\alpha \circ u_\alpha = \varphi_{f(\alpha)} \circ v_\alpha \circ u_\alpha = \varphi_{f(\alpha)} \circ \varphi_{f(\alpha), \alpha} = \varphi_\alpha ,
$$
hence $\varphi_\alpha(E_\alpha) = \psi_\alpha(u_\alpha(E_\alpha)) \subset \psi_\alpha(L_\alpha)$, and $\psi$ is surjective. Let $\alpha \in J$ and let $x, y \in L_\alpha$ with $\psi_\alpha(x) = \psi_\alpha(y)$, i.e. $\varphi_{f(\alpha)}(v_\alpha(x)) = \varphi_{f(\alpha)}(v_\alpha(y))$; there exists $\beta \in I$, $\beta \geq f(\alpha)$ such that
$$
\varphi_{\beta, f(\alpha)}(v_\alpha(x)) = \varphi_{\beta, f(\alpha)}(v_\alpha(y)) ,
$$
hence
$$
\psi_{\beta, \alpha}(x) = u_\beta(\varphi_{\beta, f(\alpha)}(v_\alpha(x))) = u_\beta(\varphi_{\beta, f(\alpha)}(v_\alpha(y))) = \psi_{\beta, \alpha}(y) .
$$
and $\psi$ is injective.

#### Theorem 1 (D. Lazard) {#alg-x-s1-thm-1 .statement}

For every A-module E, the following conditions are equivalent:
(i) E is flat.
(ii) For every A-module P of finite presentation, the canonical homomorphism
$$
\operatorname{Hom}_A(P, A) \otimes_A E \to \operatorname{Hom}_A(P, E)
$$
is surjective.
(iii) For every A-module P of finite presentation and every homomorphism $u : P \to E$, there exists a free A-module L of finite type and homomorphisms $v : P \to L$ and $w : L \to E$ such that $u = w \circ v$.
(iv) There exists a filtered ordered set J, an inductive system of free modules of finite type $(L_j)_{j \in J}$ and an isomorphism of E onto $\lim \overrightarrow{L_j}$.
(iv) $\Rightarrow$ (i) : this follows from prop. 4 (ii) of X, p. 8.
(i) $\Rightarrow$ (ii) : this follows from prop. 8b) of X, p. 12.
(ii) $\Rightarrow$ (iii) : let P be a A-module of finite presentation and $u : P \to E$ a homomorphism; by (ii), there exist $v_1, \ldots, v_n \in \operatorname{Hom}_A(P, A)$, $w_1, \ldots, w_n \in E$ such that $u(x) = \sum v_i(x) w_i$ for every $x \in P$; if $v : P \to A^n$ is the homomorphism of components $(v_i)$ and $w : A^n \to E$ the homomorphism $(a_i) \mapsto \sum a_i w_i$, we indeed have $u = w \circ v$.
(iii) $\Rightarrow$ (iv) : suppose (iii) is verified, and let $(E_\alpha, \varphi_{\beta, \alpha})$ be an inductive system, relative to a filtered set I, of A-modules of finite presentation, with inductive limit E

(X, p. 11, prop. 7). Replacing I by the lexicographic product I × N, with E_{(α,n)} = E_α for every n, we may suppose that I has no greatest element. For each α ∈ I, let L_α be a free A-module of finite type and let u_α : E_α → L_α, v'_α : L_α → E be homomorphisms such that v'_α ∘ u_α is the canonical mapping φ_α of E_α into E; since L_α is free of finite type and I has no greatest element, there exists an index β > α and a homomorphism v''_α : L_α → E_β such that v'_α = φ_β ∘ v''_α; since φ_β ∘ v''_α ∘ u_α = φ_β ∘ φ_β,α and E_α is of finite presentation, it follows from prop. 8a) of X, p. 12, that there exists γ ≥ β such that φ_{γβ} ∘ v''_α ∘ u_α = φ_{γβ} ∘ φ_{βα} = φ_{γα} ; let γ = f(α) and let v_α be the homomorphism φ_{γβ} ∘ v''_α from L_α into E_{f(α)} ; we have v_α ∘ u_α = φ_{f(α),α}. We can then apply lemma 2, whence (iv).

#### Corollary {#alg-x-s1-n6-cor-1 .statement}

Suppose A commutative. For every flat A-module E, the A-modules T(E), S(E), Λ(E), T^n(E), S^n(E), Λ^n(E) are flat.

Indeed, E is the inductive limit of a filtered system (L_j) of free A-modules of finite type, hence T(E) (resp. S(E), etc.) is the inductive limit of the filtered system of free A-modules T(L_j) (resp. S(L_j), etc.), hence is flat (cf. III, p. 61, prop. 6, p. 62, th. 1, p. 73, prop. 8, p. 75, th. 1, p. 83, prop. 9, and p. 86, th. 1).

#### Remark {#alg-x-s1-n6-rem-1 .statement}

Considering in (ii) a finite presentation A_s^J \xrightarrow{c} A_s^I \to P \to 0, one obtains the condition (ii’) still equivalent to the preceding ones:

(ii’) For every finite matrix (c_{ij})_{i \in I, j \in J} of elements of A, every solution

$$
e = (e_i)_{i \in I} \in E^I
$$

of the system of linear homogeneous equations

$$
\sum_{i \in I} c_{ij} e_i = 0,\quad j \in J,
$$

can be written b_1 z_1 + \cdots + b_n z_n, where b_1, ..., b_n \in E and where, for r = 1, ..., n, z_r = (z_{r,i})_{i \in I} is a solution in A^I of the system of equations

$$
\sum_{i \in I} z_{r,i} c_{ij} = 0,\quad j \in J.
$$

### 7. Injective modules

#### Definition 2 {#alg-x-s1-def-2 .statement}

One says that the A-module E is injective if, for every exact sequence of A-modules and homomorphisms

(19)
$$
M' \xrightarrow{u} M \xrightarrow{v} M'',
$$
the sequence of $\mathbf{Z}$-linear mappings

(20)
$$
\operatorname{Hom}_A(M'', E) \xrightarrow{\operatorname{Hom}_A(v, 1)} \operatorname{Hom}_A(M, E) \xrightarrow{\operatorname{Hom}_A(u, 1)} \operatorname{Hom}_A(M', E)
$$
is exact.

#### Lemma 3 {#alg-x-s1-lem-3 .statement}

*For the a-module E to be injective, it is necessary and sufficient that, for every injective a-linear mapping $u : M' \to M$, the mapping*

$$
\operatorname{Hom}_A(u,1) : \operatorname{Hom}_A(M,E) \to \operatorname{Hom}_A(M',E)
$$

*be surjective.*

If $E$ is injective and if $u : M' \to M$ is injective, then the sequence $0 \to M' \xrightarrow{u} M$ is exact, and hence so is the sequence $\operatorname{Hom}(M,E) \xrightarrow{\operatorname{Hom}(u,1)} \operatorname{Hom}(M',E) \to 0$, and $\operatorname{Hom}(u,1)$ is surjective. Conversely, consider the exact sequence (19); put $M''_1=\nu(M)$ and let $i : M''_1 \to M''$ be the canonical injection and $p : M \to M''_1$ the mapping $m\mapsto \nu(m)$. The sequence $M' \xrightarrow{u} M \xrightarrow{p} M''_1 \to 0$ is exact; by II, p. 36, th. 1, the sequence

$$
\operatorname{Hom}_A(M''_1,E)
\xrightarrow{\operatorname{Hom}(p,1)}
\operatorname{Hom}_A(M,E)
\xrightarrow{\operatorname{Hom}(u,1)}
\operatorname{Hom}_A(M',E)
$$

is exact. Moreover, one has $\operatorname{Hom}(\nu,1)=\operatorname{Hom}(p,1)\circ\operatorname{Hom}(i,1)$. If $E$ satisfies the condition of the lemma, $\operatorname{Hom}(i,1)$ is surjective, hence the image of $\operatorname{Hom}(\nu,1)$ is also that of $\operatorname{Hom}(p,1)$, and the sequence (20) is exact.

#### Remark {#alg-x-s1-n7-rem-1 .statement}

Let $E$ be an injective a-module, $u : M' \to M$ and $f : M' \to E$ homomorphisms of a-modules. If $\operatorname{Ker}u\subset\operatorname{Ker}f$, there exists a homomorphism $g : M \to E$ such that $g\circ u=f$. This follows indeed from what precedes applied to the injective homomorphism $M'/\operatorname{Ker}u \to M$ deduced from $u$.

#### Proposition 9 {#alg-x-s1-prop-9 .statement}

*Let $(E_i)_{i\in I}$ be a family of a-modules, $E=\prod_{i\in I}E_i$ their product. For the a-module $E$ to be injective, it is necessary and sufficient that each of the $E_i$ be so.*

Let $u : M' \to M$ be an injective homomorphism of a-modules. For the product homomorphism

$$
\prod_{i\in I}\operatorname{Hom}_A(M,E_i)
\longrightarrow
\prod_{i\in I}\operatorname{Hom}_A(M',E_i)
$$

to be surjective, it is necessary and sufficient that each of the homomorphisms $\operatorname{Hom}_A(M,E_i)\to\operatorname{Hom}_A(M',E_i)$ be so (II, p. 10, prop. 5); this proves the proposition since $\prod_{i\in I}\operatorname{Hom}_A(M,E_i)$ is canonically identified with $\operatorname{Hom}_A(M,E)$.

#### Proposition 10 {#alg-x-s1-prop-10 .statement}

*Let $E$ be an a-module. For $E$ to be injective, it is necessary and sufficient that, for every ideal $a$ of $A$ and every A-homomorphism $f : a\to E$, there exist $e\in E$ such that*

$$
f(a)=ae
$$

*for every $a\in a$.*

Suppose $E$ is injective; let $a$ be an ideal of $A$, $f : a\to E$ an A-homomorphism, and denote by $i : a\to A$ the canonical injection. Then the mapping

$$
\operatorname{Hom}_A(i,1) : \operatorname{Hom}_A(A,E)\to\operatorname{Hom}_A(a,E)
$$

is surjective (def. 2); if $g\in\operatorname{Hom}_A(A,E)$ is such that $f=g\circ i$, one has

$$
f(a)=g(a)=ag(1)
$$

for every $a\in a$.

Conversely, suppose the condition of the statement is satisfied, let $M$ be an A-module, $N$ a submodule of $M$, $u : N\to E$ an A-homomorphism, and prove that there exists an A-homomorphism $\bar u : M\to E$ extending $u$ (cf. *lemma* 3). Let $\mathcal P$ be the set of pairs $(P,v)$ where $P$ is a submodule of $M$ containing $N$ and $v$ is a homomorphism from $P$ into $E$ extending $u$. The set $\mathcal P$ ordered by the extension relation is *inductive*: if $(P_j, v_j)$ is a totally ordered family of elements of $\mathcal{P}$, put $Q = \cup P_j$ and let $w : Q \to E$ be the unique mapping inducing $v_j$ on $P_j$ for every $j$; then $(Q, w) \in \mathcal{P}$ and $(Q, w)$ majorizes $(P_j, v_j)$ for every $j$. Let then $(P, v)$ be a maximal element of $\mathcal{P}$ (E, III, p. 20, th. 2); it suffices to prove that $P = M$. Let $x \in M$ and let $\alpha$ be the ideal of the $a \in A$ such that $ax \in P$; put $f(a) = v(ax)$ for $a \in \alpha$; one thus obtains an $A$-homomorphism $f : \alpha \to E$. Let then $e$ be an element of $E$ such that $f(a) = ae$ for every $a \in \alpha$. Put $P' = P + Ax$ and let $v' : P' \to E$ be the unique $A$-homomorphism such that $v'(p + ax) = v(p) + ae$ for $p \in P, a \in A$; then $(P', v')$ belongs to $\mathcal{P}$ and majorizes $(P, v)$, hence $P' = P$, that is to say $x \in P$, which completes the proof.

#### Corollary 1 {#alg-x-s1-prop-10-cor-1 .statement}

*If the ring $A$ is left Noetherian, every direct sum of injective $A$-modules is injective.*

Let $(E_i)_{i \in I}$ be a family of injective $A$-modules, let $E$ be their direct sum, let $\alpha$ be an ideal of $A$ and let $u : \alpha \to E$ be an $A$-homomorphism. Since $A$ is noetherian, $\alpha$ is of finite type, and consequently the canonical mapping

$$
\varphi : \bigoplus_{i \in I} \operatorname{Hom}_A(\alpha, E_i) \to \operatorname{Hom}_A(\alpha, E)
$$

is bijective; let $(u_i)$ be the inverse image of $u$ by $\varphi$. Since each $E_i$ is injective, and the family $(u_i)$ has finite support, there exists an element $(e_i)_{i \in I}$ of $E$ such that $u_i(a) = ae_i$ for all $a \in \alpha$ and all $i \in I$, hence $u(a) = a((e_i))$ for all $a \in \alpha$, and $E$ is injective.

#### Remark {#alg-x-s1-n7-rem-2 .statement}

If every direct sum $A$-module of injective $A$-modules is injective, the ring $A$ is left noetherian (X, p. 170, exercise 21).

Suppose $A$ is integral. We say that the $A$-module $E$ is *divisible* if the homothety $a_E$ is surjective for every nonzero element $a$ of $A$.

#### Corollary 2 {#alg-x-s1-prop-10-cor-2 .statement}

*Suppose $A$ is integral.*
  *a)* *Every injective $A$-module is divisible.*
  *b)* *Every torsion-free (II, p. 115) and divisible $A$-module is injective.*
  *c)* *If $A$ is principal, every divisible $A$-module is injective.*

If $a \in A$ is nonzero, then $a_A$ is injective; on the other hand, for every $A$-module $E$, the homothety $a_E$ identifies canonically with

$$
\operatorname{Hom}(a_A, 1) : \operatorname{Hom}_A(A, E) \to \operatorname{Hom}_A(A, E),
$$

therefore $E$ is divisible if and only if $\operatorname{Hom}(a_E, 1_E)$ is surjective for every $a \in A$ nonzero. The assertion *a)* follows therefore from Definition 2 (X, p. 15).

Let $E$ be a divisible $A$-module; suppose that $A$ is principal (resp. $E$ is torsion-free) and let us prove that $E$ is injective by applying prop. 10. Let $\alpha$ be an ideal of $A$ and $f : \alpha \to E$ an $A$-homomorphism. Let $x \in \alpha$ be such that $\alpha = Ax$ (resp. such that $x \neq 0$ if $\alpha \neq 0$), and let $e \in E$ be such that $xe = f(x)$. Let us prove that for every $a \in \alpha$, we have

$$
f(a) = ae;
$$

this is clear if $a \in Ax$, whence the assertion in the case where A is principal; if E is torsion-free and if $xa \in a$, we have $xf(a) = f(ax) = axe$, hence $f(a) = ae$ since $x$ is nonzero if $a \neq 0$.

#### Example 1 {#alg-x-s1-n7-exa-1 .statement}

If A is integral, the field of fractions K of A is an A-module injective. If A is principal, $K/A$ is an A-module injective.
2) For example, the $\mathbf{Z}$-modules $\mathbf{Q}$ and $\mathbf{Q}/\mathbf{Z}$ are injective.
3) Let A be a principal ideal domain and let $a$ be a *nonzero* element of A. Then $A/aA$ is an $A/aA$-module injective (X, p. 170, exercise 20).

### 8. Injective cogenerators modules

#### Proposition 11 {#alg-x-s1-prop-11 .statement}

*Let B be a ring, F a B-module and P a (B, A)-bimodule. If F is an injective B-module and P a flat A-module, $\mathrm{Hom}_B(P, F)$ is an injective A-module.*

Let $u : M' \to M$ be an injective homomorphism of A-modules. We have a commutative diagram

$$
\begin{array}{ccc}
\mathrm{Hom}_A(M, \mathrm{Hom}_B(P, F)) & \xrightarrow{\mathrm{Hom}_A(u, 1)} & \mathrm{Hom}_A(M', \mathrm{Hom}_B(P, F)) \\
\beta \downarrow & & \beta' \downarrow \\
\mathrm{Hom}_B(P \otimes_A M, F) & \xrightarrow{\mathrm{Hom}(1_P \otimes u, 1_F)} & \mathrm{Hom}_B(P \otimes_A M', F)
\end{array}
$$

where $\beta$ and $\beta'$ are the canonical isomorphisms of II, p. 74. Since P is flat over A, the homomorphism $1_P \otimes u : P \otimes_A M' \to P \otimes_A M$ is injective. Since F is injective, $\mathrm{Hom}(1_P \otimes u, 1_F)$ is surjective, hence also $\mathrm{Hom}_A(u, 1)$, which proves that $\mathrm{Hom}_F(P, F)$ is an injective A-module (X, p. 16, lemma 3).

#### Definition 3 {#alg-x-s1-def-3 .statement}

*One says that the A-module E is a cogenerator if, for every A-module M and every nonzero element x of M, there exists an A-homomorphism $u : M \to E$ such that $u(x) \neq 0$.*

One says that the A-module L is a *generator* if, for every A-module M and every element x of M, there exists an A-homomorphism $u : L \to M$ such that $x \in u(L)$. For example, the A-module $A_s$ is a generator.

#### Proposition 12 {#alg-x-s1-prop-12 .statement}

*Let E be an injective A-module. In order that E be a cogenerator, it is necessary and sufficient that $\mathrm{Hom}_A(S, E) \neq 0$ for every simple A-module S.*

The condition is obviously necessary. Conversely, let M be an A-module and x a nonzero element of M; the submodule $Ax$ of M has a simple quotient S (VIII, § 2, no 1, prop. 3). If $\mathrm{Hom}_A(S, E) \neq 0$, then $\mathrm{Hom}_A(Ax, E) \neq 0$ and there exists a homomorphism $f : Ax \to E$ such that $f(x) \neq 0$; since E is injective, $f$ extends to a homomorphism $u$ of M into E and we have $u(x) = f(x) \neq 0$.

#### Example {#alg-x-s1-n8-exa-1 .statement}

The injective $\mathbf{Z}$-module $\mathbf{Q}/\mathbf{Z}$ (X, p. 18, example 2) is a cogenerator.
Indeed, every $\mathbf{Z}$-module simple module is isomorphic to a module $\mathbf{Z}/p\mathbf{Z}$, $p\ne 0$, and $\operatorname{Hom}_{\mathbf{Z}}(\mathbf{Z}/p\mathbf{Z},\mathbf{Q}/\mathbf{Z})$ is nonzero (it contains for example the element of $\mathbf{Z}/p\mathbf{Z}$ obtained by passing to quotients from the homomorphism $x\mapsto x/p$ of $\mathbf{Z}$ into $\mathbf{Q}$).

#### Proposition 13 {#alg-x-s1-prop-13 .statement}

Let $B$ be a ring, $F$ an injective cogenerator $B$-module, $P$ a $(B,A)$-bimodule. Suppose that $P$ is flat over $A$ and such that $P\otimes_A S\ne 0$ for every simple $A$-module $S$ (* that is, faithfully flat over $A$ in the sense of AC, I, §). Then the $A$-module $\operatorname{Hom}_B(P,F)$ is a cogenerator and injective.

Indeed, $\operatorname{Hom}_B(P,F)$ is injective by prop. 11. On the other hand, for every simple $A$-module $S$, $\operatorname{Hom}_A(S,\operatorname{Hom}_B(P,F))$ is isomorphic to $\operatorname{Hom}_B(P\otimes_A S,F)$, hence is nonzero since $P\otimes_A S\ne 0$ and the $B$-module $F$ is a cogenerator; the $A$-module $\operatorname{Hom}_B(P,F)$ is therefore a cogenerator by prop. 12.

#### Corollary 1 {#alg-x-s1-prop-13-cor-1 .statement}

The $A$-module $E_A=\operatorname{Hom}_{\mathbf{Z}}(A,\mathbf{Q}/\mathbf{Z})$ is injective and a cogenerator.

We apply prop. 13 with $B=\mathbf{Z}$, $F=\mathbf{Q}/\mathbf{Z}$ (example) and $P=A_d$.

For every $A$-module $M$, let

$$
I^0(M)=E_A^{\operatorname{Hom}(M,E_A)}
$$

and let $e_M:M\to I^0(M)$ be the homomorphism which associates to $m\in M$ the element

$$
(\varphi(m))_{\varphi\in\operatorname{Hom}(M,E_A)}\in I^0(M).
$$

Then:

#### Corollary 2 {#alg-x-s1-prop-13-cor-2 .statement}

The $A$-module $I^0(M)$ is injective and the $A$-homomorphism $e_M:M\to I^0(M)$ is injective.

Indeed, $I^0(M)$ is injective, since $E_A$ is injective (X, p. 16, prop. 9), on the other hand $e_M$ is injective since $E_A$ is a cogenerator.

#### Corollary 3 {#alg-x-s1-prop-13-cor-3 .statement}

Every $A$-module is isomorphic to a submodule of an injective $A$-module.

#### Corollary 4 {#alg-x-s1-prop-13-cor-4 .statement}

For the $A$-module $E$ to be injective, it is necessary and sufficient that every injective $A$-homomorphism $f:E\to F$ possess an $A$-linear retraction.

Suppose $E$ is injective and let $f:E\to F$ be an injective $A$-homomorphism. Then

$$
\operatorname{Hom}_A(f,1_E):\operatorname{Hom}_A(F,E)\to\operatorname{Hom}_A(E,E)
$$

is surjective; there therefore exists $r\in\operatorname{Hom}_A(F,E)$ such that $r\circ f=1_E$ and $r$ is an $A$-linear retraction of $f$. Conversely, there exists an injective $A$-module $I$ and an injective $A$-homomorphism $f:E\to I$ (cor. 2); if $f$ possesses an $A$-linear retraction, $E$ is injective by prop. 9 of X, p. 16.

### 9. Injective envelopes

#### Definition 4 {#alg-x-s1-def-4 .statement}

Let $M$ be an $A$-module. An injective envelope of $M$ is a pair $(I,i)$, where $I$ is an injective $A$-module and $i:M\to I$ is a homomorphism possessing the following property:

(E) for a submodule P of I to be zero, it is necessary and sufficient that i^{-1}(P) be zero.

Note that (E) implies that i is injective. One often identifies M with the submodule i(M) of I, and one then says that I is an injective envelope of M.

#### Example 1 {#alg-x-s1-n9-exa-1 .statement}

Suppose that A is integral and M is torsion-free. Let K be the field of fractions of A and let i : M → K ⊗_A M be the canonical homomorphism. Then (K ⊗_A M, i) is an injective envelope of M (II, p. 116, prop. 26 and X, p. 17, cor. 2).

#### Theorem 2 {#alg-x-s1-thm-2 .statement}

Let M be an A-module.
a) M possesses injective envelopes.
b) If (I, i) and (J, j) are two injective envelopes of M, there exists an isomorphism f : I → J such that f ∘ i = j.

It should be noted that the homomorphism f whose existence is asserted in b) is not uniquely determined in general.

a) We may suppose that M is a submodule of an injective A-module E (X, p. 19, cor. 3). Consider the set F, ordered by inclusion, of the submodules I of E, containing M, and such that the canonical injection i : M → I satisfies property (E). Since F is inductive, it possesses a maximal element (E, III, p. 20); let I be a maximal element of F. It suffices to prove that I is a direct factor submodule of E. Let N be a submodule of E such that N ∩ I = 0, and maximal for this property (such an N exists by loc. cit.). The composite homomorphism

$$
I \xrightarrow{u} E \xrightarrow{v} E/N,
$$

where u and v are the canonical homomorphisms, is injective; since E is injective, there therefore exists a homomorphism w : E/N → E such that w ∘ v ∘ u = u, that is to say w ∘ v(x) = x for x ∈ I. Put I′ = Im(w) = Im(w ∘ v) and let i′ : M → I′ be the canonical injection. Then I ⊂ I′; to complete the proof, it suffices to prove that i′ satisfies condition (E): this implies that I = I′ (maximal character of I) and hence that w ∘ v is a projector of E onto I.

Let therefore P be a submodule of I′ such that P ∩ M = 0. We have P = w ∘ v(Q), where Q is a submodule of E containing N; moreover

$$
Q \cap M = w \circ v(Q \cap M) \subset P \cap M = 0,
$$

hence Q ∩ I = 0 since i : M → I possesses property (E). By the maximal character of N, this implies Q = N, that is to say v(Q) = 0, hence P = 0, which was to be proved.

b) Let (I, i) and (J, j) be two injective envelopes of M. Since J is injective, there exists a homomorphism f : I → J such that f ∘ i = j; we have

$$
i^{-1}(\mathrm{Ker}\,f') = \mathrm{Ker}\,j = 0,
$$

hence Ker f = 0 and f is injective. Then f(I) is an injective submodule of J, hence a direct factor; since j satisfies (E), this implies f(I) = J and f is bijective.

#### Remark 1 {#alg-x-s1-n9-rem-1 .statement}

Let (I, i) be an injective envelope of M and $j : M \to J$ an injective homomorphism of M into an injective A-module J. By the proof above, there exists an *injective* homomorphism $f : I \to J$ such that $f \circ i = j$.

#### Remark 2 {#alg-x-s1-n9-rem-2 .statement}

Let (I, i) be an injective envelope of M. Identify M with the submodule $i(M)$ of I. For every submodule N of M, there exists an injective submodule of I which is an injective envelope of N (apply *Remark* 1 to N). Conversely, every injective submodule J of I is an injective envelope of $J \cap M$.

#### Proposition 14 {#alg-x-s1-prop-14 .statement}

*Let I be a nonzero injective A-module. The following conditions are equivalent*:
(i) *I is indecomposable* (VII, § 4, no 8, def. 3);
(ii) *0 is not the intersection of two nonzero submodules of I*;
(iii) *I is the injective envelope of all its nonzero submodules*;
(iv) *the ring* $\mathrm{End}_A(I)$ *is local* (VIII, § 1, no 4, def. 4).

(i) $\Rightarrow$ (iii) : let M be a nonzero submodule of I. By *Remark* 2 above, there exists a submodule I’ of I, which is an injective envelope of M. Since I’ is nonzero and a direct factor in I, we have $I = I'$ if I is indecomposable.

(iii) $\Rightarrow$ (ii) : let E and F be two submodules of I, such that $E \cap F = 0$. If $E \neq 0$, then I is an injective envelope of E by (iii), hence « $E \cap F = 0$ » implies « $F = 0$ ».

(ii) $\Rightarrow$ (i) : this is trivial.

(iv) $\Rightarrow$ (i) : this results from VIII, § 1, no 6, prop. 13.

(i) $\Rightarrow$ (iv) : suppose I is indecomposable. First note that every injective endomorphism $f$ of I is bijective (since $f(I)$ is then a nonzero direct factor submodule of I). Moreover, every endomorphism $f$ of I, whose restriction to a nonzero submodule E of I is injective, is injective (indeed, since (i) $\Rightarrow$ (iii), I is an injective envelope of E, hence « $E \cap \mathrm{Ker}\ f = 0$ » implies « $\mathrm{Ker}\ f = 0$ »). This being so, let $f$ be a noninvertible element of $\mathrm{End}_A(M)$; by VIII, § 1, no 4, prop. 9, it is a matter of proving that $1 - f$ is invertible. Since $f$ is not injective, we have $\mathrm{Ker}\ f \neq 0$; since the restriction of $1 - f$ to $\mathrm{Ker}\ f$ is injective, $1 - f$ is injective, hence bijective.

#### Corollary 1 {#alg-x-s1-prop-14-cor-1 .statement}

*The relation “I is a class of indecomposable injective A-modules” is collectivizing*.

Indeed, according to (iii) every indecomposable injective A-module is the injective envelope of a monogenic A-module.

#### Corollary 2 {#alg-x-s1-prop-14-cor-2 .statement}

*Let M be an A-module, I an injective envelope of M. In order that I be indecomposable, it is necessary and sufficient that 0 not be the intersection of two nonzero submodules of M*.

The condition is necessary according to prop. 14 ((i) $\Rightarrow$ (ii)). Conversely, if I is direct sum of the nonzero submodules $I_1$ and $I_2$, one has:

$$
I_1 \cap M \neq 0,\quad I_2 \cap M \neq 0\quad \text{et}\quad (I_1 \cap M) \cap (I_2 \cap M) = 0 .
$$

#### Example 2 {#alg-x-s1-n9-exa-2 .statement}

If A is commutative and noetherian, the indecomposable injective A-modules are exactly the injective envelopes of the modules A/p where p is a prime ideal (X, p. 171, exercise 27).

### 10. Structure of injective modules

#### Lemma 4 {#alg-x-s1-lem-4 .statement}

Let M be a nonzero noetherian A-module, I an injective envelope of M. Then I possesses an indecomposable injective submodule.

One may obviously suppose that M is a submodule of I. Let N be a submodule of M, such that I is not an injective envelope of N and maximal for this property. According to remark 2 (X, p. 21), there exists a submodule I₁ of I which is an injective envelope of N; then I₁ is a direct factor in I, let J be a direct factor complement. One has J ≠ 0, let us prove that J is indecomposable. If J′ is a nonzero direct factor submodule of J, one has J′ ∩ M ≠ 0 and

$$(J' \cap M) \cap N \subset J' \cap I_1 = 0.$$

The submodule N′ = (J′ ∩ M) + N of M is direct sum of J′ ∩ M and N, hence strictly contains N. Moreover N′ is contained in the submodule J′ + I₁ of J, which is direct sum of J′ and I₁, hence injective. According to the maximal character of N, this implies J′ + I₁ = I, hence J′ = J, and J is indecomposable.

Let $\mathcal{I}$ denote the set (X, p. 21, cor. 1) of classes of indecomposable injective A-modules.

Recall (X, p. 17, cor. 1) that, if A is left noetherian, every A-module direct sum of injective A-modules is injective.

#### Theorem 3 {#alg-x-s1-thm-3 .statement}

Let I be an injective A-module.

a) If I is the injective envelope of a noetherian A-module M, I is direct sum of a finite family of indecomposable (injective) submodules.

b) If A is left noetherian, I is direct sum of a family of indecomposable (injective) submodules.

c) If I is direct sum of indecomposable (injective) submodules, there exists one and only one family of cardinals $(a_E)_{E \in \mathcal{I}}$, such that I is isomorphic to

$$\bigoplus_{E \in \mathcal{I}} E^{(a_E)}.$$

Let us first note that c) follows from prop. 14 (X, p. 21) and from VIII, § 1, No. 7, theorem 2. Let us prove a).

Let N be a submodule of M whose injective envelopes are direct sum of a finite family of indecomposable submodules, and maximal for this property (there exists one since M is noetherian). According to remark 2 (X, p. 21), there exists a submodule I₁ of I which is an injective envelope of N. If I₁ = I, the proof is complete; otherwise, let $J$ be a direct factor complement of $I_1$ in $I$. Then $J$ is the injective envelope of the noetherian module $J\cap M$ (loc. cit.), hence possesses a nonzero indecomposable injective submodule $J'$ (lemma 4). Then $I_1+J'$ is injective, direct sum of a finite family of indecomposable submodules, and the injective envelope of the submodule $(I_1+J')\cap M$ of $M$ which strictly majorizes $N$, whence a contradiction.

Suppose $A$ is left noetherian and let us prove b). Let $X$ be the set sum of the sets $\operatorname{Hom}_A(E,I)$ for $E\in\mathcal{J}$. To each subset $Y$ of $X$ associate an $A$-module $E_Y$ and an $A$-homomorphism $f_Y:E_Y\to I$ in the following way: $Y$ is the sum of a family $(Y(E))_{E\in\mathcal{J}}$ where $Y(E)\subset\operatorname{Hom}_A(E,I)$, one sets

$$
E_Y=\bigoplus_{E\in\mathcal{J}}E^{(Y(E))}
$$

and the component of $f$ on the direct factor of $E_Y$ corresponding to the element $y$ of $Y(E)\subset\operatorname{Hom}_A(E,I)$ is $y:E\to I$. Let $Y$ be a subset of $X$, such that $f_Y$ is injective and that $Y$ is maximal for this property (such a subset exists according to E, III, p. 20); it suffices to prove that $f_Y$ is bijective. Otherwise, let $J$ be a direct factor complement of the injective submodule $\operatorname{Im}(f_Y)$ of $I$; since $J$ is nonzero, it possesses a nonzero noetherian submodule (because A is supposed noetherian), hence also a nonzero injective submodule $J'$ which is the injective envelope of a noetherian module. According to a), $J'$ is direct sum of a finite nonempty family of indecomposable submodules. There therefore exists a finite nonempty subset $Y'$ of $X$ such that $f_{Y'}$ maps bijectively $E_{Y'}$ onto $J'$. Since $\operatorname{Im}(f_Y)\cap J'=0$, one has $Y\cap Y'=\varnothing$ and $f_{Y\cup Y'}$ is injective; this contradicts the maximal character of $Y$ and completes the proof.

## EXERCISES {#alg-x-s1-exercises}

See the [exercises for § 1](exercises/s1/).
