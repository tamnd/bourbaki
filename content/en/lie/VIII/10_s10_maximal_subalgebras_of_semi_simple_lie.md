---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: VIII
chapter_title: SPLIT SEMI-SIMPLE LIE ALGEBRAS
section: 10
section_title: Maximal subalgebras of semi-simple Lie algebras
lang: en
source: lie-vii-ix
book_pages: 159-163, 260-261
pdf_pages: 0167-0171, 0268-0269
extraction: native
statements: 8
exercises: 7
content_sha256: 345f66620b2c4fae05d0eb5d76aa4f165ea7875de6e8bd6a97f18302eec6a845
---

## § 10. MAXIMAL SUBALGEBRAS OF SEMI-SIMPLE LIE ALGEBRAS

#### Theorem 1 {#lie-viii-s10-thm-1 .statement tag=016L}

Let V be a finite dimensional vector space, $\mathfrak{g}$ a reductive Lie subalgebra in $\mathfrak{g}\mathfrak{l}(V),\mathfrak{q}$ a Lie subalgebra of $\mathfrak{g}$ and $\Phi$ the bilinear form $(x, y) \rightarrow$ Tr($xy$) on $\mathfrak{g}\times \mathfrak{g}$. Assume that the orthogonal complement $\mathfrak{n}$ of $\mathfrak{q}$ with respect to $\Phi$ is a Lie subalgebra of $\mathfrak{g}$ consisting of nilpotent endomorphisms of V. Then $\mathfrak{q}$ is a parabolic subalgebra of $\mathfrak{g}$.

$a)\mathfrak{q}$ is the normalizer of $\mathfrak{n}$ in $\mathfrak{g}:$ let $\mathfrak{p}$ be this normalizer. Let $x\in \mathfrak{q}$ and $y\in \mathfrak{n}$; for all $z\in \mathfrak{q}$, we have $[z, x]\in \mathfrak{q}$, so

$$
\Phi ([x, y], z) =\Phi (y,[z, x]) = 0
$$

in other words, $[x, y]\in \mathfrak{n}$. Hence $\mathfrak{q}\subset \mathfrak{p}$. Since $\mathfrak{n}$ is an ideal of $\mathfrak{p}$ consisting of nilpotent endomorphisms of V, P is orthogonal to $\mathfrak{n}$ with respect to $\Phi$ (Chap. I, no. 3, Prop. $4d$)$)$. Since $\Phi$ is non-degenerate$^4,\mathfrak{p}\subset \mathfrak{q}$, hence our assertion.

b) There exists a reductive Lie subalgebra $\mathfrak{m}$ in $\mathfrak{g}\mathfrak{l}(V)$ such that $\mathfrak{q}$ is the semi-direct product of $\mathfrak{m}$ and $\mathfrak{n}:$ let $\mathfrak{n}_V(\mathfrak{q})$ be the largest ideal of $\mathfrak{q}$ consisting of nilpotent endomorphisms of V. Then $\mathfrak{n}_V(\mathfrak{q})$ contains $\mathfrak{n}$, and it is orthogonal to $\mathfrak{q}($loc. cit.); hence $\mathfrak{n}=\mathfrak{n}_V(\mathfrak{q})$. Moreover, $\mathfrak{g}$ is reductive in $\mathfrak{g}\mathfrak{l}(V)$ by hypothesis, hence decomposable (Chap. VII, §5, no. 1, Prop. 2); since $\mathfrak{q}$ is the intersection of $\mathfrak{g}$ with the normalizer of $\mathfrak{n}$ in $\mathfrak{g}\mathfrak{l}$(V), it is a decomposable Lie algebra (loc. cit., Cor. 1 of Prop. 3). Thus, our assertion follows from Prop. 7 of Chap. VII, §5, no. 3.

Choose a Cartan subalgebra $\mathfrak{h}$ of $\mathfrak{m}$; denote by $\mathfrak{g}_1$ the commutant of $\mathfrak{h}$ in $\mathfrak{g}$, and put $\mathfrak{q}_1=\mathfrak{q}\cap \mathfrak{g}_1,\mathfrak{n}_1=\mathfrak{n}\cap \mathfrak{g}_1$.

c) The Lie algebras $\mathfrak{g}_1,\mathfrak{q}_1$ and $\mathfrak{n}_1$ satisfy the same hypotheses as $\mathfrak{g},\mathfrak{q}$ and $\mathfrak{n}:$ since $\mathfrak{m}$ is reductive in $\mathfrak{g}\mathfrak{l}$(V), $\mathfrak{h}$ is commutative and is composed of semi-simple endomorphisms of V (Chap. VII, §2, no. 4, Cor. 3 of Th. 2). Thus $\mathfrak{g}_1=\mathfrak{g}^0(\mathfrak{h})$ is reductive in $\mathfrak{g}$ (Chap. VII, §1, no. 3, Prop. 11), hence also in $\mathfrak{g}\mathfrak{l}(V)$ (Chap. I, §6, no. 6, Cor. 2 of Prop. 7). It is clear that $\mathfrak{n}_1$ is composed

$^4$ Let $\mathfrak{z}$ be the orthogonal complement of $\mathfrak{g}$ with respect to $\Phi$; this is an ideal of $\mathfrak{g}$ contained in $\mathfrak{n}$, so every element of $\mathfrak{z}$ is nilpotent. The identity representation of $\mathfrak{g}$ is semi-simple (Chap. I, §6, Cor. 1 of Prop. 7). Hence $\mathfrak{z}= 0$ (Chap. I, §4, no. 3, Lemma 2). of nilpotent endomorphisms of V. Since $\mathfrak{h}$ is a subalgebra of $\mathfrak{q}$, reductive in $\mathfrak{g}\mathfrak{l}$(V), the adjoint representation of $\mathfrak{h}$ on $\mathfrak{q}$ is semi-simple; by construction, $\mathfrak{q}_1$ is the set of invariants of ad$_{\mathfrak{q}}(\mathfrak{h})$, so $\mathfrak{q}=\mathfrak{q}_1+ [\mathfrak{h},\mathfrak{q}]$ (Chap. I, §3, no. 5, Prop. 6). Since

$$
\Phi (\mathfrak{g}_1,[\mathfrak{h},\mathfrak{q}]) =\Phi ([\mathfrak{h},\mathfrak{g}_1],\mathfrak{q}) = 0
$$

an element of $\mathfrak{g}_1$ is orthogonal to $\mathfrak{q}_1$ if and only if it is orthogonal to $\mathfrak{q}$; consequently, $\mathfrak{n}_1=\mathfrak{g}_1\cap \mathfrak{n}$ is the orthogonal complement of $\mathfrak{q}_1$ in $\mathfrak{g}_1$.

d) The Cartan subalgebra $\mathfrak{h}$ of $\mathfrak{m}$ is a Cartan subalgebra of $\mathfrak{g}:$ We have $\mathfrak{q}=\mathfrak{m}\oplus \mathfrak{n}$ and $\mathfrak{h}=\mathfrak{m}\cap \mathfrak{g}_1$, so it is immediate that $\mathfrak{q}_1=\mathfrak{h}\oplus \mathfrak{n}_1$. Moreover, $[\mathfrak{h},\mathfrak{n}_1] = 0,\mathfrak{h}$ is commutative and $\mathfrak{n}_1$ is nilpotent, so the Lie algebra $\mathfrak{q}_1$ is nilpotent. By a) and $c),\mathfrak{q}_1$ is the normalizer of $\mathfrak{n}_1$ in $\mathfrak{g}_1$; a fortiori$,\mathfrak{q}_1$ is equal to its normalizer in $\mathfrak{g}_1$, hence is a Cartan subalgebra of $\mathfrak{g}_1$. Since $\mathfrak{g}_1$ is reductive in $\mathfrak{g}\mathfrak{l}$(V), it follows from Cor. 3 of Th. 2 of Chap. VII, §2, no. 4, that $\mathfrak{q}_1$ is composed of semi-simple endomorphisms of V; thus, since $\mathfrak{n}_1$ is composed of nilpotent endomorphisms of V, we have $\mathfrak{n}_1= 0$. Consequently, $\mathfrak{h}=\mathfrak{q}_1$ is a Cartan subalgebra of $\mathfrak{g}_1$, and since $\mathfrak{g}_1$ normalizes $\mathfrak{h}$, we have $\mathfrak{h}=\mathfrak{g}_1$. Thus, we have proved that every element of $\mathfrak{h}$ is a semi-simple element of $\mathfrak{g}$, and that the commutant of $\mathfrak{h}$ in $\mathfrak{g}$ is equal to $\mathfrak{h}$; it follows that $\mathfrak{h}=\mathfrak{g}^0(\mathfrak{h})$, so $\mathfrak{h}$ is a Cartan subalgebra of $\mathfrak{g}$.

$e)\mathfrak{q}$ is a parabolic subalgebra of $\mathfrak{g}:$ by the preceding, $\mathfrak{h}$ is a Cartan subalgebra of $\mathfrak{g},\mathfrak{n}$ consists of nilpotent elements of $\mathfrak{g}$, and $[\mathfrak{h},\mathfrak{n}]\subset \mathfrak{n}$. Let $\overline{k}$ be an algebraic closure of $k$; by definition, $\mathfrak{q}$ is parabolic in $\mathfrak{g}$ if and only if $\overline{k}\otimes_k\mathfrak{q}$ is a parabolic subalgebra of $\overline{k}\otimes_k\mathfrak{g}$. The properties stated above being preserved by extension of scalars, for the proof we can restrict ourselves to the case in which $\mathfrak{h}$ is splitting. Let R be the root system of $(\mathfrak{g},\mathfrak{h})$; by Prop. 2 (v) of §3, no. 1, there exists a subset P of R such that $P\cap (-P) =\emptyset$ and $\mathfrak{n}=\sum_{\alpha\in P}\mathfrak{g}^{\alpha}$.

Let $P'$ be the set of roots $\alpha$ such that $-\alpha  \notin P$; we have $P'\cup (-P') = R$, and the orthogonal complement $\mathfrak{q}$ of $\mathfrak{n}$ in $\mathfrak{g}$ is equal to $\mathfrak{h}+\sum_{\alpha\in P'}\mathfrak{g}^{\alpha}$. We have

proved that $\mathfrak{q}$ is parabolic. Q.E.D.

#### Lemma 1 {#lie-viii-s10-lem-1 .statement tag=016M}

Let $\mathfrak{g}$ be a semi-simple Lie algebra, V a finite dimensional vector space, $\rho$ a linear representation of $\mathfrak{g}$ on V, D a vector subspace of V$,\mathfrak{h}$ a Cartan subalgebra of $\mathfrak{g},\mathfrak{s}$ (resp. $\mathfrak{s}'$) the set of $x\in \mathfrak{h}$ such that $\rho (x)D\subset D$ (resp. $\rho (x)D = 0$), and $\Phi$ the bilinear form on $\mathfrak{g}$ associated $^5$ to $\rho$.

(i) If $\mathfrak{h}$ is splitting, the vector subspaces $\mathfrak{s}$ and $\mathfrak{s}'$ of $\mathfrak{h}$ are rational over $\mathbf{Q}$.

(ii) If $\rho$ is injective, the restriction of $\Phi$ to $\mathfrak{s}$ (resp. $\mathfrak{s}'$) is non-degenerate.

Assume that the Cartan subalgebra $\mathfrak{h}$ is splitting. Let $d$ be the dimension of D; put $W =\bigwedge^d(V)$ and $\sigma =\bigwedge^d(\rho )$; denote also by $(e_1, . . . , e_d)$ a basis of D and $e=e_1\wedge  \cdots  \wedge e_d$ a decomposable $d$-vector associated to D. Let P be the set of weights of $\sigma$ with respect to $\mathfrak{h}$; denote by $W^\mu$ the subspace of

$^5$ In other words, $\Phi (x, y) =$ Tr($\rho (x)\rho (y)$) for $x, y\in \mathfrak{g}$. W associated to the weight $\mu$, and put $e=\sum_{\mu\in P}e^\mu$ (with $e^\mu\in W^\mu$ for all

$\mu\in P)$; finally, let $P'$ be the set of weights $\mu$ such that $e^\mu\not= 0$ and let $P''$ be the set of differences of elements of $P'$. Let $x$ be in $\mathfrak{h}$; then $x$ belongs to $\mathfrak{s}$ if and only if there exists $c$ in $k$ such that $\rho (x).e=c.e$ (Chap. VII, §5, no. 4, Lemma 2 (i)). Since $\rho (x).e^\mu=\mu(x).e^\mu$, we see that $x\in \mathfrak{s}$ is equivalent to the relation “$\mu(x) = 0$ for all $\mu\in P''$ ”. Now, the $\mathbf{Q}$-structure of $\mathfrak{h}$ is the $\mathbf{Q}$-vector subspace $\mathfrak{h}_{\mathbf{Q}}$ of $\mathfrak{h}$ generated by the coroots $H_{\alpha}$ and all $\mu$ in $P''$ take rational values on $\mathfrak{h}_{\mathbf{Q}}$; it follows (Algebra, Chap. II, §8, no. 4, Prop. 5) that $\mathfrak{s}$ is a subspace of $\mathfrak{h}$ rational over $\mathbf{Q}$.

For any weight $\mu\in P$, let $p_\mu$ be the projection onto $V^\mu$ associated to the decomposition $V =\bigoplus_{\mu\in P}V^\mu$; denote by $P_1$ the set of $\mu\in P$ such that

$p_\mu(D)\not= 0$. It is immediate that $\mathfrak{s}'$ is the intersection of the kernels (in $\mathfrak{h}$) of the elements of $P_1$; it follows, in the same way as for $\mathfrak{s}$, that $\mathfrak{s}'$ is a subspace of $\mathfrak{h}$ rational over $\mathbf{Q}$. This proves (i).

By extension of scalars, it suffices to prove (ii) when $k$ is algebraically closed, hence when $\mathfrak{h}$ is splitting. Let $\mathfrak{m}$ be a vector subspace of $\mathfrak{h}$ rational over $\mathbf{Q}$; for all non-zero $x$ in $\mathfrak{m}_{\mathbf{Q}}=\mathfrak{m}\cap \mathfrak{h}_{\mathbf{Q}}$, we have $\Phi (x, x)>0$ by the Cor. of Prop. 1 of §7, no. 1. The restriction of $\Phi$ to $\mathfrak{m}_{\mathbf{Q}}$ is non-degenerate, and hence so is the restriction of $\Phi$ to $\mathfrak{m}$ since $\mathfrak{m}$ is canonically isomorphic to $k\otimes_{\mathbf{Q}}\mathfrak{m}_{\mathbf{Q}}$.

#### Definition 1 {#lie-viii-s10-def-1 .statement tag=016N}

Let $\mathfrak{q}$ be a Lie subalgebra of the semi-simple Lie algebra $\mathfrak{g}$. Then $\mathfrak{q}$ is said to be decomposable in $\mathfrak{g}$ if, for all $x\in \mathfrak{q}$, the semi-simple and nilpotent components of $x$ in $\mathfrak{g}$ belong to $\mathfrak{q}$. Denote by $\mathfrak{n}_{\mathfrak{g}}(\mathfrak{q})$ the set of elements $x$ of the radical of $\mathfrak{q}$ such that ad$_{\mathfrak{g}}x$ is nilpotent.

Let $\rho$ be an injective representation of $\mathfrak{g}$ on a finite dimensional vector space V. We know (Chap. I, §6, no. 3, Th. 3) that an element $x$ of $\mathfrak{g}$ is semi-simple (resp. nilpotent) if and only if the endomorphism $\rho (x)$ of V is semi-simple (resp. nilpotent). It follows immediately that the algebra $\mathfrak{q}$ is decomposable in $\mathfrak{g}$ if and only if $\rho (\mathfrak{q})$ is a decomposable subalgebra of $\mathfrak{g}\mathfrak{l}(V)$ in the sense of Definition 1 of Chap. VII, §5, no. 1. With the notations of Chap. VII, §5, no. 3, we also have

$$
\rho (\mathfrak{n}_{\mathfrak{g}}(\mathfrak{q})) =\mathfrak{n}_V(\rho (\mathfrak{q}))
$$

#### Theorem 2 {#lie-viii-s10-thm-2 .statement tag=016O}

Let $\mathfrak{g}$ be a semi-simple Lie algebra, $\mathfrak{n}$ a subalgebra of $\mathfrak{g}$ consisting of nilpotent elements, $\mathfrak{q}$ the normalizer of $\mathfrak{n}$ in $\mathfrak{g}$. Assume that $\mathfrak{n}$ is the set of nilpotent elements of the radical of $\mathfrak{q}$. Then $\mathfrak{q}$ is parabolic.

Note first of all that $\mathfrak{q}$ is decomposable (Chap. VII, §5, no. 1, Cor. 1 of Prop. 3). By Th. 1, it suffices to prove that $\mathfrak{q}$ is the orthogonal complement $\mathfrak{n}^0$ of $\mathfrak{n}$ with respect to the Killing form $\Phi$ of $\mathfrak{g}$. We know that $\mathfrak{q}\subset \mathfrak{n}^0$ (Chap. I, §4, no. 3, Prop. $4d$)$)$. By Chap. VII, §5, no. 3, Prop. 7, there exists a subalgebra $\mathfrak{m}$ of $\mathfrak{q}$, reductive in $\mathfrak{g}$, such that $\mathfrak{q}$ is the semi-direct product of $\mathfrak{m}$ and $\mathfrak{n}$. We show that the restriction of $\Phi$ to $\mathfrak{m}$ is non-degenerate. Let $\mathfrak{c}$ be the centre of $\mathfrak{m}$. We have $\Phi ([\mathfrak{m},\mathfrak{m}],\mathfrak{c}) = 0$ by Chap. I, §5, no. 5, Prop. 5, and the restriction of $\Phi$ to $[\mathfrak{m},\mathfrak{m}]$ is non-degenerate by Chap. I, §6, no. 1, Prop. 1. It remains to see that the restriction of $\Phi$ to $\mathfrak{c}$ is non-degenerate. Let $\mathfrak{k}$ be a Cartan subalgebra of $[\mathfrak{m},\mathfrak{m}]$; then $\mathfrak{k}\oplus \mathfrak{c}$ is commutative and reductive in $\mathfrak{g}$. Let $\mathfrak{h}$ be a Cartan subalgebra of $\mathfrak{g}$ containing $\mathfrak{k}\oplus \mathfrak{c}$ (Chap. VII, §2, no. 3, Prop. 10). Then $\mathfrak{h}\cap \mathfrak{q}$ is a commutative subalgebra of $\mathfrak{q}$ containing $\mathfrak{k}\oplus \mathfrak{c}$, and ad$_{\mathfrak{q}}x$ is semi-simple for all $x\in \mathfrak{h}\cap \mathfrak{q}$; hence $\mathfrak{h}\cap \mathfrak{q}$ is contained in a Cartan subalgebra $\mathfrak{h}'$ of $\mathfrak{q}$ (Chap. VII, §2, no. 3, Prop. 10); let $f$ be the projection of $\mathfrak{q}$ onto $\mathfrak{m}$ with kernel $\mathfrak{n}$; then $f(\mathfrak{h}')$ is a Cartan subalgebra of $\mathfrak{m}$ (Chap. VII, §2, no. 1, Cor. 2 of Prop. 4) containing $\mathfrak{k}\oplus \mathfrak{c}$, and consequently equal to $\mathfrak{k}\oplus \mathfrak{c}$; this proves that $f(\mathfrak{h}\cap \mathfrak{q}) =\mathfrak{k}\oplus \mathfrak{c}$, and since every element of $\mathfrak{h}$ is semi-simple in $\mathfrak{g}$, we have $\mathfrak{h}\cap \mathfrak{q}=\mathfrak{k}\oplus \mathfrak{c}$. Thus,

$\mathfrak{c}=\{x\in \mathfrak{h}|[x,\mathfrak{n}]\subset \mathfrak{n}$ and $[x,[\mathfrak{m},\mathfrak{m}]] = 0\}$.

By Lemma 1, the restriction of $\Phi$ to $\mathfrak{c}$ is non-degenerate.

Let $\mathfrak{q}^0$ be the orthogonal complement of $\mathfrak{q}$ in $\mathfrak{g}$ relative to $\Phi$. The preceding proves that $\mathfrak{q}\cap \mathfrak{q}^0=\mathfrak{n}$. Assume that $\mathfrak{q}\not=\mathfrak{q}^0$, so $\mathfrak{q}^0\not=\mathfrak{n}$ (and $\mathfrak{q}^0\supset \mathfrak{n}$). Since ad$_{\mathfrak{g}}\mathfrak{n}$ leaves $\mathfrak{q}$ stable, ad$_{\mathfrak{g}}\mathfrak{n}$ leaves $\mathfrak{q}^0$ stable; Engel’s theorem proves that there exists $x\in \mathfrak{q}^0$ such that $x \notin \mathfrak{n}$ and $[x,\mathfrak{n}]\subset \mathfrak{n}$. But then $x\in \mathfrak{q}^0\cap \mathfrak{q}=\mathfrak{n}$, a contradiction. Hence $\mathfrak{q}=\mathfrak{n}^0$.

#### Corollary 1 {#lie-viii-s10-thm-2-cor-1 .statement tag=016P}

Let $\mathfrak{q}$ be a maximal element of the set of subalgebras of $\mathfrak{g}$ distinct from $\mathfrak{g}$. Then $\mathfrak{q}$ is either parabolic or reductive in $\mathfrak{g}$.

We can assume that $\mathfrak{g}$ is a Lie subalgebra of $\mathfrak{g}\mathfrak{l}(V)$ for some finite dimensional vector space V. Let $\mathfrak{e}(\mathfrak{q})\subset \mathfrak{g}$ be the decomposable envelope of $\mathfrak{q}$. If $\mathfrak{e}(\mathfrak{q}) =\mathfrak{g},\mathfrak{q}$ is an ideal of $\mathfrak{g}$ (Chap. VII, §5, no. 2, Prop. 4), hence is semi-simple, and consequently $\mathfrak{q}$ is reductive in $\mathfrak{g}$. Assume that $\mathfrak{e}(\mathfrak{q})\not=\mathfrak{g}$. Then $\mathfrak{e}(\mathfrak{q}) =\mathfrak{q}$, so $\mathfrak{q}$ is decomposable. Assume that $\mathfrak{q}$ is not reductive in $\mathfrak{g}$. Let $\mathfrak{n}$ be the set of nilpotent elements of the radical of $\mathfrak{q}$. Then $\mathfrak{n}\not= 0$ (Chap. VII, §5, no. 3, Prop. 7 (i)). Let $\mathfrak{p}$ be the normalizer of $\mathfrak{n}$ in $\mathfrak{g}$. Then $\mathfrak{p}\supset \mathfrak{q}$, and $\mathfrak{p}\not=\mathfrak{g}$ since $\mathfrak{g}$ is semi-simple. Hence $\mathfrak{p}=\mathfrak{q}$. Thus $\mathfrak{q}$ is parabolic (Th. 1).

#### Corollary 2 {#lie-viii-s10-thm-2-cor-2 .statement tag=016Q}

Let $\mathfrak{n}$ be a subalgebra of $\mathfrak{g}$ consisting of nilpotent elements. There exists a parabolic subalgebra $\mathfrak{q}$ of $\mathfrak{g}$ with the following properties:

(i) $\mathfrak{n}\subset \mathfrak{n}_{\mathfrak{g}}(\mathfrak{q})$;

(ii) the normalizer of $\mathfrak{n}$ in $\mathfrak{g}$ is contained in $\mathfrak{q}$;

(iii) every automorphism of $\mathfrak{g}$ leaving $\mathfrak{n}$ invariant leaves $\mathfrak{q}$ invariant.

If $\mathfrak{g}$ is splittable, $\mathfrak{n}$ is contained in a Borel subalgebra of $\mathfrak{g}$.

Let $\mathfrak{q}_1$ be the normalizer of $\mathfrak{n}$ in $\mathfrak{g}$. This is a decomposable subalgebra of $\mathfrak{g}$. Let $\mathfrak{n}_1=\mathfrak{n}_{\mathfrak{g}}(\mathfrak{q}_1)$. Define inductively $\mathfrak{q}_i$ to be the normalizer of $\mathfrak{n}_{i-1}$ in $\mathfrak{g}$, and $\mathfrak{n}_i$ to be equal to $\mathfrak{n}_{\mathfrak{g}}(\mathfrak{q}_i)$. The sequences $(\mathfrak{n},\mathfrak{n}_1,\mathfrak{n}_2, . . .)$ and $(\mathfrak{q}_1,\mathfrak{q}_2, . . .)$ are increasing. There exists $j$ such that $\mathfrak{q}_j=\mathfrak{q}_{j+1}$, in other words $\mathfrak{q}_j$ is the normalizer of $\mathfrak{n}_{\mathfrak{g}}(\mathfrak{q}_j)$ in $\mathfrak{g}$. Thus $\mathfrak{q}_j$ is parabolic (Th. 1). We have $\mathfrak{n}\subset \mathfrak{n}_j=$ $\mathfrak{n}_{\mathfrak{g}}(\mathfrak{q}_j)$, and $\mathfrak{q}_1\subset \mathfrak{q}_j$; every automorphism of $\mathfrak{g}$ leaving $\mathfrak{n}$ invariant evidently leaves $\mathfrak{n}_1,\mathfrak{n}_2, . .$. and $\mathfrak{q}_1,\mathfrak{q}_2, . .$. invariant. If $\mathfrak{g}$ is splittable, $\mathfrak{q}_j$ contains a Borel subalgebra $\mathfrak{b}$, and consequently (§3, no. 4, Prop. 13), we have $\mathfrak{b}\supset \mathfrak{n}_{\mathfrak{g}}(\mathfrak{q}_j)\supset \mathfrak{n}$.

#### Theorem 3 {#lie-viii-s10-thm-3 .statement tag=016R}

Assume that $k$ is algebraically closed. Let $\mathfrak{g}$ be a semi-simple Lie algebra. Let $\mathfrak{a}$ be a solvable subalgebra of $\mathfrak{g}$. There exists a Borel subalgebra of $\mathfrak{g}$ containing $\mathfrak{a}$.

By Chap. VII, §5, no. 2, Cor. 1 (ii) of Prop. 4, we can assume that $\mathfrak{a}$ is decomposable. There exists a commutative subalgebra $\mathfrak{t}$ of $\mathfrak{g}$, consisting of semi-simple elements, such that $\mathfrak{a}$ is the semi-direct product of $\mathfrak{t}$ and $\mathfrak{n}_{\mathfrak{g}}(\mathfrak{a})$ (Chap. VII, §5, no. 3, Cor. 2 of Prop. 6). There exists (Cor. 2 of Th. 2) a parabolic subalgebra $\mathfrak{q}$ of $\mathfrak{g}$ such that $\mathfrak{n}_{\mathfrak{g}}(\mathfrak{a})\subset \mathfrak{n}_{\mathfrak{g}}(\mathfrak{q})$, and such that the normalizer of $\mathfrak{n}_{\mathfrak{g}}(\mathfrak{a})$ in $\mathfrak{g}$ is contained in $\mathfrak{q}$; a fortiori$,\mathfrak{a}\subset \mathfrak{q}$. Let $\mathfrak{b}$ be a Borel subalgebra of $\mathfrak{g}$ contained in $\mathfrak{q}$ and $\mathfrak{h}$ a Cartan subalgebra of $\mathfrak{g}$ contained in $\mathfrak{b}$. Then $\mathfrak{h}$ is a Cartan subalgebra of $\mathfrak{q}$, so there exists $s\in$ Aut$_e(\mathfrak{q})$ such that $s(\mathfrak{t})\subset \mathfrak{h}$ (Chap. VII, §2, no. 3, Prop. 10 and Chap. VII, §3, no. 2, Th. 1). We have $s(\mathfrak{n}_{\mathfrak{g}}(\mathfrak{q})) =\mathfrak{n}_{\mathfrak{g}}(\mathfrak{q})$ (Chap. VII, §3, no. 1, Remark 1), so

$$
s(\mathfrak{a}) =s(\mathfrak{t}) +s(\mathfrak{n}_{\mathfrak{g}}(\mathfrak{a}))\subset \mathfrak{h}+s(\mathfrak{n}_{\mathfrak{g}}(\mathfrak{q})) =\mathfrak{h}+\mathfrak{n}_{\mathfrak{g}}(\mathfrak{q})\subset \mathfrak{b}
$$

#### Corollary {#lie-viii-s10-n0-cor-1 .statement tag=016S}

If $k$ is algebraically closed, every maximal solvable subalgebra of $\mathfrak{g}$ is a Borel subalgebra.

### Exercises {#lie-viii-s10-exercises}

See the [exercises for § 10](exercises/s10/).
