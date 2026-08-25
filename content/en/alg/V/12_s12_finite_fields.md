---
book: alg
book_title: Algebra
chapter: V
chapter_title: COMMUTATIVE FIELDS
section: 12
section_title: Finite fields
lang: en
source: alg-iv-vii
source_edition: 2003, Springer
book_pages: A V.166-A V.170
pdf_pages: 0207-0212, 0280-0284
extraction: ocr
subsections:
    - "no": 1
      title: The structure of finite fields
      page: 0
      pdf_page: 207
    - "no": 2
      title: Algebraic extensions of a finite field
      page: 94
      pdf_page: 208
    - "no": 3
      title: The Galois group of the algebraic closure of a finite field
      page: 96
      pdf_page: 210
    - "no": 4
      title: Cyclotomic polynomials over a finite field
      page: 97
      pdf_page: 211
statements: 11
exercises: 14
content_sha256: e60a2a890add7e12050f25d7a498d8768d7ca3d96969eb55b1ce5018b03c8a13
---

## § 12. FINITE FIELDS

### 1. The structure of finite fields

#### Proposition 1 {#alg-v-s12-prop-1 .statement}

— Let K be a finite field with q elements.

a) The characteristic of K is a prime number p, and there exists an integer f \geq 1 such that q = p^f.

b) The additive group of K is a direct sum of f cyclic groups of order p.

c) The multiplicative group of K is cyclic of order q - 1.

Since Z is infinite and K finite, the unique ring homomorphism \varphi : Z \to K is not injective and its kernel is a prime ideal of Z not equal to 0. Therefore the characteristic of K is a prime number and K is an algebra over the field \mathbf{F}_p of p elements (V, p. 2). Let f be the degree of K over \mathbf{F}_p. If f were infinite, K would contain, for each integer n \geq 0 a subspace of dimension n over \mathbf{F}_p, whence q \geq p^n, which is absurd. Therefore f is finite. The additive group of K is thus isomorphic to (\mathbf{F}_p)^f, whence the assertions a) and b).

Assertion c) follows by Lemma 1 (V, p. 78).

#### Proposition 2 {#alg-v-s12-prop-2 .statement}

— Let K be a finite field of q elements. The field K is a splitting field of the polynomial X^q - X of \mathbf{F}_p[X] and it is the set of all roots of this polynomial.

1 In agreement with the conventions of this chapter we shall only be concerned here with finite commutative fields. In fact, every finite field is commutative, as we shall see in Chapter VIII (cf. V, p. 170, Exercise 14).

For every $x \neq 0$ in $K$ we have $x^{q-1} = 1$ because $K^*$ is a finite group of order $q-1$ (I, p. 52). It follows that $x^q = x$ for each $x$ in $K$. The polynomial $X^q - X$ of $\mathbf{F}_p[X]$ is of degree $q$ and it has $q$ roots in $K$, whence

$$
X^q - X = \prod_{\xi \in K} (X - \xi).
$$

Proposition 2 follows at once from this.

#### Corollary {#alg-v-s12-n1-cor-1 .statement}

— *Two finite fields of the same cardinal are isomorphic.*

Let $K'$ be a finite field of $q$ elements; its characteristic is a prime number $p'$ dividing $q = p^f$, whence $p' = p$. Therefore $K'$ is a splitting field of the polynomial $X^q - X$ in $\mathbf{F}_p[X]$ (Prop. 2), and so $K$ and $K'$ are isomorphic (V, p. 22, Cor.).

When $K = \mathbf{F}_p$, Formula (1) reduces to the relation

$$
X^p - X \equiv \prod_{i=0}^{p-1} (X - i) \mod p \mathbf{Z}[X]
$$

in the polynomial ring $\mathbf{Z}[X]$.

Formula (2) may also be written

$$
X^{p-1} - 1 \equiv \prod_{i=1}^{p-1} (X - i) \mod p \mathbf{Z}[X]
$$

In particular for $X = 0$ we obtain (« Wilson's formula »)

$$
(p-1)! \equiv -1 \mod p
$$

### 2. Algebraic extensions of a finite field

#### Proposition 3 {#alg-v-s12-prop-3 .statement}

— *Let $K$ be a finite field of $q$ elements, $\Omega$ an algebraically closed extension of $K$ and $m$ an integer $\geqslant 1$.
a) There exists a unique subextension $K_m$ of $\Omega$ which is of degree $m$ over $K$.
b) The field $K_m$ has $q^m$ elements and is the set of fixed points of the automorphism $x \mapsto x^{q^m}$ of $\Omega$.
c) We have $K_m = K(\zeta)$ for every generator $\zeta$ of the cyclic group $K_m^*$.
Let $p$ be the characteristic of $K$ and $f$ the degree of $K$ over $\mathbf{F}_p$. We have $q^m = p^{fm}$ and the mapping $x \mapsto x^{q^m}$ is thus an automorphism of the perfect field $\Omega$ (V, p. 7, Prop. 4). Therefore the set $K_m$ of roots of the polynomial $X^{q^m} - X$ of $K[X]$ is a subfield of $\Omega$. Since the derivative of $X^{q^m} - X$ is equal to $-1$, all the roots of this polynomial are simple (IV, p. 17, Prop. 7) and so $K_m$ has $q^m$ elements. It follows that $[K_m : K] = m$.

Now let L be a subextension of $\Omega$, of degree $m$ over $K$. As vector space over $K$, $L$ is isomorphic to $K^m$ and so has $q^m$ elements. We thus have $x^{q^m} = x$ for all $x \in L$ (Prop. 2), whence $L \subset K_m$. Since $[L : K] = [K_m : K] = m$, we finally have $L = K_m$.

We have thus proved Assertions $a)$ and $b)$, and $c)$ is trivial.

#### Corollary {#alg-v-s12-n2-cor-1 .statement}

— *Let $K$ be a finite field and $\Omega$ an algebraically closed extension of $K$. The relative algebraic closure $\overline{K}$ of $K$ in $\Omega$ consists of () and roots of unity and is an algebraic closure of $K$.*

We know $K$ to be an algebraic closure of $K$ (V, p. 22, Example 2) and it is clear that every root of unity in $\Omega$ belongs to $K$. Further, given $x \neq 0$ in $\overline{K}$, of degree $m$ over $K$, if $K$ has $q$ elements, then the field $K(x)$ has $q^m$, whence $x^{q^m - 1} = 1$, and so $x$ is a root of unity in $\Omega$.

Let $p$ be a prime number and let $\mathbf{F}_p = \mathbf{Z}/p\mathbf{Z}$ be the field of $p$ elements. We choose an algebraic closure $\Omega$ of $\mathbf{F}_p$, whose existence follows from Steinitz's theorem (V, p. 23, Th. 2). Let $f$ be a positive integer and $q = p^f$. By Prop. 3 there exists a unique subfield of $\Omega$ which is of degree $f$ over $\mathbf{F}_p$; we shall denote it by $\mathbf{F}_q(\Omega)$ or by abuse of notation $\mathbf{F}_q$. It is the unique subextension of $\Omega$ which has degree $f$ over $\mathbf{F}_p$. It is the unique subfield of $\Omega$ of cardinal $q$, and every field of cardinal $q$ is isomorphic (not canonically) to $\mathbf{F}_q$ (Cor. of Prop. 2). We note that $\mathbf{F}_q$ consists of those $x$ in $\Omega$ for which $x^q = x$ and that $F, \subset \mathbf{F}_{q'}$ if and only if $q'$ is a power of $q$.

#### Proposition 4 {#alg-v-s12-prop-4 .statement}

— *Let $\mathbf{K}$ be a finite field of $q$ elements and $\mathbf{K}_m$ an extension of finite degree $m$ of $K$.

a) The field $\mathbf{K}_m$ is a Galois extension of $K$ whose Galois group is the cyclic group of order $m$ generated by the automorphism $\sigma_q : x \mapsto x^q$.

b) For each $x \in \mathbf{K}_m$ the norm of $x$ with respect to $K$ is equal to $x^{(q^m - 1)/(q - 1)}$.

c) Every element of $K$ is the trace (resp. norm) of an element of $\mathbf{K}_m$.*

Let $\Gamma$ be the cyclic group of automorphisms of $\mathbf{K}_m$ generated by $\sigma_q$. The field of invariants of $\Gamma$ consists of the elements $x$ of $\mathbf{K}_m$ such that $x^q = x$, hence is equal to $K$. Therefore $\mathbf{K}_m$ is a Galois extension of $K$ with Galois group $\Gamma$, and this latter has order equal to $[K_m : K] = m$ (V, p. 66, Th. 3). Thus $a)$ follows.

We have $\Gamma = \{1, \sigma_q, \sigma_q^2, \ldots, \sigma_q^{m-1}\}$; the norm of an element $x$ of $\mathbf{K}_m$ with respect to $K$ is thus $N(x) = \prod_{i=0}^{m-1} \sigma_q^i(x) = x^{1 + q + \cdots + q^{m-1}}$ and we have $1 + q + \cdots + q^{m-1} = \frac{q^m - 1}{q - 1}$. This proves b). Let $\xi$ be a generator of the cyclic group $\mathbf{K}_m^*$; the image of the norm $N : \mathbf{K}_m^* \to K^*$ is the cyclic subgroup of $K^*$ generated by the element $\xi = N(\xi) = \xi^{(q^m - 1)/(q - 1)}$; since $\xi$ is of order $q^m - 1$, $\xi$ is of order $q - 1$, and so generates $K^*$. This proves that every non-zero element of K is norm of a non-zero element of K ; moreover, we have $0 = N(0)$.

Finally since $K_m$ is a separable algebraic extension of K, the trace is a non-zero linear form on the vector space $K_m$ over K (V, p. 49, Cor.) ; so every element of K is the trace of an element of $K_m$.

### 3. The Galois group of the algebraic closure of a finite field

Let $S \neq \{1\}$ be a set of integers $\geq 1$ stable under multiplication ; we shall order it by the relation « m divides n ». When m divides n, we have $m\mathbf{Z} \supset n\mathbf{Z}$, hence there is a canonical homomorphism $\pi_{m,n}$ of the ring $\mathbf{Z}/n\mathbf{Z}$ onto the ring $\mathbf{Z}/m\mathbf{Z}$. We denote by $A(S)$ the inverse limit of the inverse system of rings $(\mathbf{Z}/m\mathbf{Z}, \pi_{m,n})$ indexed by S. Each finite set $\mathbf{Z}/m\mathbf{Z}$ is equipped with the discrete topology and $A(S)$ with the topology induced by that of the product $\prod_{n \in S} (\mathbf{Z}/n\mathbf{Z})$.

Then $A(S)$ is a compact topological ring (Gen. Top. I, p. 64, Prop. 8). We see at once that the unique ring homomorphism $\varphi$ of $\mathbf{Z}$ into $A(S)$ is injective with a dense image ; *we shall identify $\mathbf{Z}$ with its image under $\varphi$ in $A(S)$*. For the topology induced on $\mathbf{Z}$ by that of $A(S)$, *the sets $m\mathbf{Z}$ (for $m \in S$) form a base of neighbourhoods of 0*.

When $S = \mathbf{N}^*$, $A(S)$ is written $\hat{\mathbf{Z}}$. When S consists of the powers of a prime number $l$, $A(S)$ is written $\mathbf{Z}_l$ and is called « ring of I-adic integers ». We thus have

$$
\hat{\mathbf{Z}} = \lim_{\leftarrow m \geq 1} \mathbf{Z}/m\mathbf{Z} , \quad \mathbf{Z}_l = \lim_{\leftarrow n \geq 0} \mathbf{Z}/l^n\mathbf{Z} .
$$

When S and T are two sets of integers stable under multiplication such that $S \supset T$, we have a natural projection $A(S) \to A(T)$ which is a continuous homomorphism of topological rings. In particular, for every prime number $l$ we have a continuous homomorphism $\mathbf{Z} \to \mathbf{Z}_l$. From it we obtain a continuous homomorphism

$$
\hat{\mathbf{Z}} \to \prod_l \mathbf{Z}_l
$$

(product extended over all prime numbers) ; this is an *isomorphism of topological rings*, as follows from the passage to the inverse limit in I, p. 112, Prop. 11.

Let K be a finite field of q elements and K an algebraic closure of K. For every integer $m \geq 1$ we denote by $K_m$ the unique subfield of K which is of degree m over K (Prop. 3). We have $\overline{K} = \bigcup_{m \geq 1} K_m$. Further we denote by $\sigma_q$ the automorphism $x \mapsto x^q$ of the perfect field $\overline{K}$; it is called the *Frobenius automorphism* of K (relative to K).

#### Proposition 5 {#alg-v-s12-prop-5 .statement}

— There exists a unique isomorphism of topological groups $\pi_K : \mathbf{Z} \to \mathrm{Gal}(\bar{K}/K)$ such that $\pi_K(1) = \sigma_q$.

Let $\Gamma$ be the subgroup of $\mathrm{Gal}(\bar{K}/K)$ generated by $\sigma_q$. For every integer $m > 0$ we have $\sigma_q^m(x) = x^{q^m}$ for all $x \in \bar{K}$, hence the set of fixed points of $\sigma_q^m$ is equal to $K$. Since $K \neq \bar{K}$, we have $\sigma_q^m \neq 1$. Hence there is an isomorphism $\pi_0$ of $\mathbf{Z}$ onto $\Gamma$ which maps 1 to $\sigma_q$.

The field of invariants of $\Gamma$ consists of the $x \in K$ such that $x^q = x$, hence is equal to $K$. Therefore (V, p. 67, Lemma 2) the group $\Gamma$ is dense in $\mathrm{Gal}(\bar{K}/K)$. Since every subextension of $\bar{K}$ of finite degree over $K$ is one of the fields $K_m$, the subgroups $\mathrm{Gal}(\bar{K}/K_m)$ form a fundamental system of neighbourhoods of 1 in $\mathrm{Gal}(\bar{K}/K)$. It is clear that $\Gamma \cap \mathrm{Gal}(\bar{K}/K_m)$ is the cyclic group generated by $\sigma_q^m$, hence equal to $\pi_0(m\mathbf{Z})$.

From the above remarks about the topology of $\mathbf{Z}$ the isomorphism $\pi_0 : \mathbf{Z} \to \Gamma$ extends in a unique fashion to an isomorphism of topological groups $\pi_K : \mathbf{Z} \to \mathrm{Gal}(\bar{K}/K)$.

Let $m \geq 1$ be an integer; it is clear that the Frobenius automorphism of $\bar{K}$ relative to $K$ is $\sigma_q^m$. Hence we obtain the relation

$$
\pi_{K_m}(a) = \pi_K(ma) \quad \text{for } a \in \mathbf{Z}.
$$

### 4. Cyclotomic polynomials over a finite field

Let $K$ be a finite field of $q$ elements, $n \geq 1$ an integer not divisible by the characteristic $p$ of $K$ and $R_n$, a cyclotomic extension of level $n$ of $K$ (V, p. 81). We know that the group $\mu_n(R_n) = \mu_n$ of $n$-th roots of unity in $R_n$, is cyclic of order $n$, that $R_n = K(\mu_n)$ and that there exists an injective homomorphism

$$
\varphi_n : \mathrm{Gal}(R_n/K) \to (\mathbf{Z}/n\mathbf{Z})^*
$$

such that $\sigma(\zeta) = \zeta^j$ for $\sigma \in \mathrm{Gal}(R_n/K)$, $\zeta \in \mu_n$ and $j \in \varphi_n(\sigma)$.

Further, if $f$ is the degree of $R_n$ over $K$, then the Galois group of $R_n$ over $K$ is cyclic of order $f$, generated by the automorphism $\sigma_q : x \mapsto x^q$ (V, p. 95, Prop. 4). We have at once:

#### Proposition 6 {#alg-v-s12-prop-6 .statement}

— The image under $\varphi_n$ of the Frobenius automorphism $\sigma_q$ is the residue class of $q \mod n$.

Therefore, taking into account Prop. 6 of V, p. 84 :

#### Corollary {#alg-v-s12-n4-cor-1 .statement}

— The degree of $R_n$ over $K$ is the least integer $f \geq 1$ such that $q^f \equiv 1 \pmod{n}$. For the cyclotomic polynomial $\Phi_n$ to be irreducible over $K$ it is necessary and sufficient that the group $(\mathbf{Z}/n\mathbf{Z})^*$ should be generated by the residue class of $q$ modulo $n$.

#### Example 1 {#alg-v-s12-n4-exa-1 .statement}

The polynomial $\Phi_3(X) = X^2 + X + 1$ is irreducible in $F_q[X]$ if and only if $q \equiv 2 \pmod{3}$. Likewise $\Phi_4(X) = X^2 + 1$ is irreducible in $F_q[X]$ if and only if $q \equiv 3 \pmod{4}$ and for $\Phi_5 = X^4 + X^3 + X^2 + X + 1$, the irreducibility condition reads $q \equiv 2,\ 3 \pmod{5}$.

#### Example 2 {#alg-v-s12-n4-exa-2 .statement}

We have $5^2 \equiv 1 \pmod{12}$, hence the residue class of 5 (mod 12) does not generate $(\mathbf{Z}/12\mathbf{Z})^*$. So the polynomial $\Phi_{12}(X) = X^4 - X^2 + 1$ is not irreducible in $F_5[X]$; in fact we have
$$
\Phi_5(X) = (X^2 + 2X - 1)(X^2 - 2X - 1)
$$
in $F_5[X]$.

### Exercises {#alg-v-s12-exercises}

See the [exercises for § 12](exercises/s12/).
