---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: VII
chapter_title: CARTAN SUBALGEBRAS AND REGULAR ELEMENTS
section: 1
section_title: Polynomial maps and Zariski topology
appendix: true
lang: en
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
content_sha256: 924d229258599545b2e684cddeddef2bd0e7a75b8d133f6a0fc19c591581eb15
---

## APPENDIX I POLYNOMIAL MAPS AND ZARISKI TOPOLOGY

In this appendix, $k$ is assumed to be infinite.

### 1. ZARISKI TOPOLOGY

Let V be a finite dimensional vector space. We denote by $A_V$ the algebra of polynomial functions on V with values in $k($Algebra, Chap. IV, §5, no. 10, Def. 4). This is a graded algebra; its component of degree 1 is the dual $V^*$ of V, and the injection of $V^*$ into $A_V$ extends to an isomorphism from the symmetric algebra $\mathbf{S}(V^*)$ to $A_V($Algebra, Chap. IV, §5, no. 11, Remark 2).

If $(e_1, . . . , e_n)$ is a basis of V, and $(X_1, . . . ,X_n)$ a sequence of indeterminates, the map from $k[X_1, . . . ,X_n]$ to $A_V$ that takes any element $f$ of $k[X_1, . . . ,X_n]$ to the function

$$
\sum_{i=1}^n\lambda_ie_i \rightarrow f(\lambda_1, . . . , \lambda_n)
$$

is an isomorphism of algebras (Algebra, Chap. IV, §5, no. 10, Cor. of Prop. 19).

#### Proposition 1 {#lie-vii-a1-prop-1 .statement tag=00XC}

Let H be the set of algebra homomorphisms from $A_V$ to $k$. For any $x\in V$, let $h_x$ be the homomorphism $f \rightarrow f(x)$ from $A_V$ to $k$. Then, the map $x \rightarrow h_x$ is a bijection from V to H.

Indeed, let $H'$ be the set of algebra homomorphisms from $k[X_1, . . . ,X_n]$ to $k$. The map $\chi  \rightarrow (\chi (X_1), . . . , \chi (X_n))$ is clearly a bijection from $H'$ to $k^n$.

#### Corollary {#lie-vii-a1-n1-cor-1 .statement tag=00XD}

For any $x\in V$, let $\mathfrak{m}_x=$ Ker($h_x$). Then the map $x \rightarrow \mathfrak{m}_x$ is a bijection from V to the set of ideals $\mathfrak{m}$ of $A_V$ such that $A_V/\mathfrak{m}=k$.

A subset F of V is said to be closed if there exists a family $(f_i)_{i\in I}$ of elements of $A_V$ such that

$x\in F\Leftarrow \Rightarrow x\in V$ and $f_i(x) = 0$ for all $i\in I$.

It is clear that $\emptyset$ and V are closed, and that any intersection of closed sets is closed. If F is defined by the vanishing of the $f_i$ and $F'$ by that of the $f'_j$, $F\cup F'$ is defined by the vanishing of the $f_if'_j$, and hence is closed. Thus, there exists a topology on V such that the closed sets for this topology are exactly the closed sets in the above sense. This topology is called the Zariski topology on V. For any $f\in A_V$, we denote by $V_f$ the set of $x\in V$ such that $f(x)\not= 0$; this is an open subset of V. It is clear that the $V_f$ form a base of the Zariski topology. (If $k$ is a topological field, the canonical topology of V is finer than the Zariski topology.)

The map $x \rightarrow \mathfrak{m}_x$ of the Cor. of Prop. 1 can be considered as a map $\varepsilon$ from V to the prime spectrum Spec(A$_V)$ of $A_V($Commutative Algebra, Chap. II, §4, no. 3, Def. 4). It is immediate that the Zariski topology is the inverse image under $\varepsilon$ of the topology of Spec(A$_V)$.

#### Proposition 2 {#lie-vii-a1-prop-2 .statement tag=00XE}

The vector space V, equipped with the Zariski topology, is an irreducible noetherian space. In particular, every non-empty open subset of V is dense.

Since $A_V$ is noetherian, Spec(A$_V)$ is noetherian (Commutative Algebra, Chap. II, §4, no. 3, Cor. 7 of Prop. 11), and every subspace of a noetherian space is noetherian (loc. cit., no. 2, Prop. 8). With the notation of the Cor. of Prop. 1, the intersection of the $\mathfrak{m}_x$ is $\{0\}$, and $\{0\}$ is a prime ideal of $A_V$; thus V is irreducible (loc. cit., no. 3, Prop. 14).

### 2. DOMINANT POLYNOMIAL MAPS

Let $V,W$ be finite dimensional vector spaces. Let $f$ be a polynomial map from V to W (Algebra, Chap. IV, §5, no. 10, Def. 4). If $\psi \in A_W,\psi \circ f\in A_V$ (loc. cit., Prop. 17). The map $\psi  \rightarrow \psi \circ f$ is a homomorphism from $A_W$ to $A_V$, said to be associated to $f$. Its kernel consists of the functions $\psi \in A_W$ which vanish on $f(V)$ (and hence also on the closure of $f(V)$ in the Zariski topology).

#### Definition 1 {#lie-vii-a1-def-1 .statement tag=00XF}

A polynomial map $f: V\rightarrow W$ is said to be dominant if the homomorphism from $A_W$ to $A_V$ associated to $f$ is injective.

In view of the preceding, $f$ is dominant if and only if $f(V)$ is dense in W in the Zariski topology.

#### Proposition 3 {#lie-vii-a1-prop-3 .statement tag=00XG}

Assume that $k$ is algebraically closed. Let $f: V\rightarrow W$ be a dominant polynomial map. The image under $f$ of any dense open subset of V contains a dense open subset of W.

It suffices to prove that, for every non-zero element $\varphi$ of $A_V,f(V_{\varphi})$ contains a dense open subset of W. Identify $A_W$ with a subalgebra of $A_V$ by means of the homomorphism associated to $f$. There exists a non-zero element $\psi$ of $A_W$ such that every homomorphism $w: A_W\rightarrow k$ which does not annihilate $\psi$ extends to a homomorphism $v: A_V\rightarrow k$ which does not annihilate $\varphi ($Commutative Algebra, Chap. V, §3, no. 1, Cor. 3 of Th. 1). Now such a $w$ (resp. $v)$ can be identified with an element of $W_{\psi}$ (resp. of $V_{\varphi})$ and to say that $v$ extends $w$ means that $f(v) =w$. Hence, $W_{\psi}\subset f(V_{\varphi})$. Q.E.D.

Let $f: V\rightarrow W$ be a polynomial map, and $x_0\in V$. The map $h \rightarrow f(x_0+h)$ from V to W is polynomial. Decompose it into a finite sum of homogeneous polynomial maps:

$$
f(x_0+h) =f(x_0) + D_1(h) + D_2(h) +\cdots
$$

where $D_i: V\rightarrow W$ is homogeneous of degree $i($Algebra, Chap. IV, §5, no. 10, Prop. 19). The linear map $D_1$ is called the tangent linear map of $f$ at $x_0$. We denote it by $Df(x_0)$.

#### Proposition 4 {#lie-vii-a1-prop-4 .statement tag=00XH}

Let $f: V\rightarrow W$ be a polynomial map. Assume that there exists $x_0\in V$ such that $(Df)(x_0)$ is surjective. Then $f$ is dominant.

Applying a translation in V and one in W, we can assume that $x_0= 0$ and $f(x_0) = 0$. The decomposition of $f$ as a sum of homogeneous elements can then be written

$f=f_1+f_2+\cdots$ with deg $f_i=i$,

and the linear map $f_1$ is surjective by hypothesis. Suppose that $f$ is not dominant. Then there exists a non-zero element $\psi$ of $A_W$ such that $\psi \circ f= 0$. Let $\psi =\psi_m+\psi_{m+1}+\cdots$ be the decomposition of $\psi$ into homogeneous elements, with deg $\psi_i=i$ and $\psi_m\not= 0$. Then

$$
0 =\psi \circ f=\psi_m\circ f+\psi_{m+1}\circ f+\cdots
$$

$$
=\psi_m\circ f_1+\rho
$$

where $\rho$ is a sum of homogeneous polynomial maps of degrees $> m$. It follows that $\psi_m\circ f_1= 0$. Since $f_1$ is surjective, $\psi_m= 0$, a contradiction.

#### Corollary {#lie-vii-a1-n2-cor-1 .statement tag=00XI}

If $k$ is algebraically closed and if $f$ satisfies the assumptions of Prop. 4, the image under $f$ of any dense open subset of V contains a dense open subset of W.

This follows from Props. 3 and 4.

### Exercises {#lie-vii-a1-exercises}

Denote by V a finite dimensional vector space over $k$.

See the [exercises for Appendix 1](exercises/a1/).
