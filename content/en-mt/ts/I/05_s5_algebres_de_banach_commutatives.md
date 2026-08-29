---
book: ts
book_title: Théories spectrales
chapter: I
chapter_title: ALGÈBRES NORMÉES
section: 5
section_title: Algèbres de Banach commutatives régulières
lang: en
source: ts-i-ii-fr
book_pages: TS I.88-TS I.95, TS I.178-TS I.180
pdf_pages: 0101-0108, 0191-0193
extraction: native
subsections:
    - "no": 1
      title: Définition
      page: 88
      pdf_page: 101
    - "no": 2
      title: Synthèse harmonique
      page: 91
      pdf_page: 104
statements: 16
exercises: 7
content_sha256: 8dd593cbb4218fac0351469777486cdf7a8f4d3e8dc8f530061b40e9ef71c147
translated_from: content/fr/ts/I/05_s5_algebres_de_banach_commutatives.md
source_lang: fr
translation_method: machine
source_content_sha256: 77bf9552a7e15b5eaff68232b4e04dcbe3abd5be58471a8f420d757b35bd8afa
translation_model: gpt-5-6-mini, gpt-5-mini, gpt-5.4
translation_run: translate-en-mt-6a92ff57
glossary_version: 34
glossary_terms_sha256: 65ccd110409e9c9826adf80392f54fed2dea10921b93840a26a39136301ceb4b
prompt_sha256: 5b9b7144015934413fe8e16b5155e2bc50bed2041525e1b1db7c19a297193094
---

## § 5. REGULAR COMMUTATIVE BANACH ALGEBRAS

In this section, the base field is $\mathbf{C}$.

### 1. Definition

#### Proposition 1 {#ts-i-s5-prop-1 .statement tag=02BV}

Let A be a commutative Banach algebra. The following conditions are equivalent:

(i) The weak topology and the Jacobson topology on $\mathsf{X}(A)$ coincide ;

(ii) For every $\chi \in \mathsf{X}(A)$ and every weakly closed subset F of $\mathsf{X}(A)$ such that $\chi \notin F$, there exists an $x\in A$ such that $\mathscr{G}(x)$ is equal to 1 at $\chi$ and to 0 on F;

(iii) For every weakly compact subset K and every weakly closed subset F of $\mathsf{X}(A)$ such that $K\cap F =\emptyset$, there exists an element $x\in A$ such that $\mathscr{G}(x)$ is equal to 1 on K and to 0 on F.

Let $M\subset \mathsf{X}(A)$. To say that M is closed for the Jacobson topology means that, for every $\chi \in \mathsf{X}(A)$ - M, there exists an $x\in A$ such that $\mathscr{G}(x)$ vanishes on M but not at $\chi$ (lemma 2 of I, p. 39). Condition (ii) therefore means that every weakly closed subset of $\mathsf{X}(A)$ is closed for the Jacobson topology, which shows that (ii) $=\Rightarrow$ (i). Moreover (iii) $=\Rightarrow$ (ii) since the subset $\{\chi \}$ is weakly compact in $\mathsf{X}(A)$. Finally (i) $=\Rightarrow$ (iii) according to the cor. of prop. 15 of I, p. 81.

#### Definition 1 {#ts-i-s5-def-1 .statement tag=02BW}

Let A be a commutative Banach algebra. It is said to be regular if it satisfies the equivalent conditions of Proposition 1.

#### Remark {#ts-i-s5-n1-rem-1 .statement tag=02BX}

Let $\widetilde{A}$ be the Banach algebra deduced from A by adjunction of a unit element $e$. Condition (ii) of prop. 1 shows that if $\widetilde{A}$ is regular, then A is regular. Suppose that A is regular and let us show that $\widetilde{A}$ is regular. Consider subsets F and $F'$ of $\mathsf{X}(\widetilde{A})$ which are disjoint and weakly closed (hence weakly compact) and construct an $x\in \widetilde{A}$ such that $\mathscr{G}(x)$ vanishes on F, and is equal to 1 on $F'$. Let $\chi_0\in \mathsf{X}(\widetilde{A})$ be the character which is zero on A. If $\chi_0\notin F'$, there exists, according to condition (iii) of prop. 1 and the assumption on A, an element $x\in A$ such that $\mathscr{G}(x)$ vanishes on F and is equal to 1 on $F'$. If $\chi_0\in F'$, we have $\chi_0\notin F$; there exists therefore an element $y\in A$ such that $\mathscr{G}(y)$ vanishes on $F'$ and is equal to 1 on F. The element $x=e-y$ of $\widetilde{A}$ then has the required property.

#### Example {#ts-i-s5-n1-exa-1 .statement tag=02BY}

Let us take up again the examples of n$^o2$ of I, p. 17.

The algebra of continuous functions with complex values tending to 0 at infinity on a locally compact space X (example 3 of I, p. 17) is regular (cf. I, p. 36, example 1).

The algebra of $n$ times differentiable functions on $[0,1]$ (example 4 of I, p. 18) is regular (cf. I, p. 36, example 2).

If G is a commutative locally compact group and $\mu$ a Haar measure on G, then the algebra $L^1(G, \mu)$ (example 7 of I, p. 19) is regular (cf. II, p. 219, cor. 2).

The algebra of functions which are continuous in the disk $|z|\leqslant 1$ and analytic in the interior (example 9 of I, p. 20) is not regular (cf. I, p. 193, exerc. 6).

#### Proposition 2 {#ts-i-s5-prop-2 .statement tag=02BZ}

Let A be a unital commutative regular Banach algebra. Let $n\geqslant 1$ be an integer and $(U_1, . . . ,U_n)$ an open covering of $\mathsf{X}(A)$. There exist elements $x_1, . . . , x_n$ of A of sum 1 such that Supp($\mathscr{G}(x_i)$)$\subset U_i$ for $i= 1, . . . ,n$.

Let us prove the proposition by induction on $n$. The assertion is valid if $n= 1$. Suppose that $n\geqslant 2$ and that the assertion is established for $n-1$.

There exists an open covering $(V_1, . . . ,V_n)$ of $\mathsf{X}(A)$ such that $\overline{V}_i\subset$ $U_i$ for all $i$. By the induction hypothesis, there exist elements $x, x_3, . . . , x_n\in A$ such that $x+x_3+\cdots +x_n= 1$ and Supp($\mathscr{G}(x)$)$\subset V_1\cup V_2$, Supp($\mathscr{G}(x_i)$)$\subset V_i$ for $i\geqslant 3$. Let K = Supp($\mathscr{G}(x)$)$\subset V_1\cup V_2$. Let $K_1$ (resp. $K_2$) be the set of elements of K which do not belong to $V_1$ (resp. $V_2$). Then $K_1$ and $K_2$ are disjoint compact subsets of K. Since the Banach algebra A is regular, there therefore exists $y\in A$ such that $\mathscr{G}(y) = 1$ on $K_1$ and $\mathscr{G}(y) = 0$ on $K_2$. Then $\mathscr{G}(xy)$ is zero on $\mathsf{X}(A)-K$ and on $K_2$, hence Supp $\mathscr{G}(xy)\subset \overline{V}_2\subset U_2$. Analogously, $\mathscr{G}(x(1-y))$ is zero on $\mathsf{X}(A)$ - K and on $K_1$, hence Supp $\mathscr{G}(x(1-y))\subset \overline{V}_1\subset U_1$. The elements $x_1=x(1-y),x_2=xy$, and $x_3, . . . ,x_n$ then satisfy the properties of the proposition.

#### Corollary 1 {#ts-i-s5-prop-2-cor-1 .statement tag=02C0}

Let A be a commutative regular unital Banach algebra, let I be an ideal of A and let $f:\mathsf{X}(A)\rightarrow \mathbf{C}$ be a continuous function. Suppose that, for every $\chi \in \mathsf{X}(A)$, there exists an element $y_{\chi}\in I$ such that $f=\mathscr{G}(y_{\chi})$ in a neighbourhood of $\chi$. Then there exists an element $y\in I$ such that $f=\mathscr{G}(y)$.

Since $\mathsf{X}(A)$ is compact, there exists a finite open covering $(U_1, . . . ,U_n)$ of $\mathsf{X}(A)$, and elements $y_1, . . . , y_n$ of I such that $f=\mathscr{G}(y_i)$ on $U_i$. By prop. 2, there exist elements $x_1, . . . , x_n$ of A of sum 1 such that Supp($\mathscr{G}(x_i)$)$\subset U_i$ for every $i$. Let $y=x_1y_1+\cdots +$ $x_ny_n$. This is an element of I having the required property. Indeed, let $\chi \in \mathsf{X}(A)$. For $1\leqslant i\leqslant n$, one has $\mathscr{G}(x_i)(\chi )\mathscr{G}(y_i)(\chi ) =\mathscr{G}(x_i)(\chi )f(\chi )$ since $\mathscr{G}(y_i)(\chi ) =f(\chi )$ if $\chi \in U_i$, and $\mathscr{G}(x_i)(\chi ) = 0$ if $\chi  \notin U_i$. It follows that

$$
\mathscr{G}(y)(\chi ) =\sum_{i=1}^n\mathscr{G}(x_i)(\chi )\mathscr{G}(y_i)(\chi ) =f(\chi )\sum_{i=1}^n\mathscr{G}(x_i)(\chi ) =f(\chi )
$$

#### Corollaire 2 {#ts-i-s5-prop-2-cor-2 .statement tag=02C1}

Let A be a commutative regular Banach algebra, I an ideal of A and $f:\mathsf{X}'(A)\rightarrow \mathbf{C}$ a continuous function. Suppose that, for every $\chi \in \mathsf{X}'(A)$, there exists an element $y_{\chi}\in I$ such that $f=\mathscr{G}'(y_{\chi})$ in a neighbourhood of $\chi$. Then there exists an element $y\in I$ such that $f=\mathscr{G}'(y)$.

Let $\widetilde{A}$ be the Banach algebra obtained from A by adjunction of a unit element. Then $\widetilde{A}$ is regular (remark 1), and $\mathsf{X}'(A) =\mathsf{X}(\widetilde{A})$; it is therefore sufficient to apply cor. 1 to $\widetilde{A}$ and to the ideal I.

If I is an ideal of a commutative Banach algebra, recall (cf. I, p. 30) that we denote by V(I) the set of $\chi \in \mathsf{X}(A)$ whose kernel contains I, in other words the set of $\chi \in \mathsf{X}(A)$ where all the functions $\mathscr{G}(x)$ vanish for $x\in I$. It is a closed subset of $\mathsf{X}(A)$ for the Jacobson topology.

#### Proposition 3 {#ts-i-s5-prop-3 .statement tag=02C2}

Let A be a commutative regular Banach algebra, I an ideal of A and K a compact subset of $\mathsf{X}(A)$ disjoint from V(I). There exists an element $x\in I$ such that $\mathscr{G}(x) = 1$ for every $x$ in K.

This is a special case of prop. 15 of I, p. 81 taking into account the fact that the Jacobson topology coincides with the weak topology on $\mathsf{X}(A)$.

### 2. Harmonic synthesis

Let A be a commutative Banach algebra. Recall that if M is a subset of $\mathsf{X}(A)$, we denote by Υ(M) the intersection of the kernels of the elements of M (cf. I, p. 30); it is an ideal of A.

#### Proposition 4 {#ts-i-s5-prop-4 .statement tag=02C3}

Let A be a commutative regular Banach algebra without radical. Let F be a closed subset of $\mathsf{X}(A)$. The set of ideals I of A such that V(I) = F, ordered by inclusion, has a greatest element, namely Υ(F), and a smallest element, namely the set J of $x\in A$ such that $\mathscr{G}(x)$ has compact support disjoint from F.

By construction, Υ(F) is an ideal of A such that V(Υ(F)) contains F, and it is the greatest ideal of A having this property. Since F is closed, there exists an ideal I of A such that V(I) = F; hence $I\subset \Upsilon (F)$, whence $V(\Upsilon (F))\subset V(I) = F$, so that V(Υ(F)) = F. This proves the first assertion.

The set J is an ideal of A and V(J) contains F. Let us show that V(J) = F. Let $\chi \in \mathsf{X}(A)$ not belonging to F. Let U be a compact neighbourhood of $\chi$ not meeting F (TG, I, p. 65, cor. of prop. 9). By assertion (ii) of prop. 1 of I, p. 88, there exists $x\in A$ such that $\mathscr{G}(x)$ is equal to 1 at $\chi$ and to 0 outside U. We then have $x\in J$ and therefore $\chi \notin V(J)$. This shows that $V(J)\subset F$ and therefore V(J) = F.

Finally, let I be an ideal of A such that V(I) = F. Let us show that $J\subset I$. Let $x\in J$ and let C be the support of $\mathscr{G}(x)$; the subset C is a compact subset of $\mathsf{X}(A)$ disjoint from F. By Prop. 3, there exists an element $u\in I$ such that $\mathscr{G}(u) = 1$ on C. We then have $\mathscr{G}(x) =\mathscr{G}(ux)$, and therefore $x=ux$ since A is without radical (Prop. 8 of I, p. 38). Consequently, we have $x\in I$, which shows that $J\subset I$.

#### Corollary 1 {#ts-i-s5-prop-4-cor-1 .statement tag=02C4}

Let A be a commutative regular Banach algebra without radical. Let J be the set of $x\in A$ such that $\mathscr{G}(x)$ has compact support. Suppose that J = A. Then every closed ideal of A distinct from A is contained in a regular maximal ideal.

If I is a closed ideal of A which is contained in no regular maximal ideal, then $V(I) =\emptyset$, hence $I\supset J$ (Prop. 4 applied to F = $\emptyset$ ), whence $I\supset \overline{J}= A$.

#### Corollary 2 {#ts-i-s5-prop-4-cor-2 .statement tag=02C5}

Let A be a commutative regular Banach algebra without radical. Let $x, y\in A$. If the support of $\mathscr{G}(x)$ is compact and contained in the set of characters $\chi$ such that $\mathscr{G}(y)(\chi )\not= 0$, then $x$ is a multiple of $y$ in A.

Let I be the ideal $Ay$ of A. Then V(I) is the set of zeros of $\mathscr{G}(y)$. Since the support F of $\mathscr{G}(x)$ is compact and disjoint from V(I), we have $x\in I$ (Prop. 4 applied to F).

#### Definition 2 {#ts-i-s5-def-2 .statement tag=02C6}

Let A be a commutative Banach algebra.

Let I be an ideal of A$,x\in A$, and $\chi \in \mathsf{X}'(A)$. One says that $x$ belongs to I in a neighbourhood of $\chi$ if there exists an element $y\in I$ such that $\mathscr{G}'(y)$ and $\mathscr{G}'(x)$ coincide in a neighbourhood of $\chi$.

One says that A satisfies Ditkin's condition if, for every $\chi \in \mathsf{X}'(A)$ and every $x\in A$ such that $\mathscr{G}'(x)$ vanishes at $\chi$, there exists a sequence $(x_n)$ in A such that $x=$ lim$_{n\rightarrow \infty}x_nx$ and such that each $\mathscr{G}'(x_n)$ vanishes in a neighbourhood $V_n$ of $\chi$.

#### Remark {#ts-i-s5-n2-rem-1 .statement tag=02C7}

Let A be a commutative Banach algebra.

1) If $\chi$ is such that $\mathscr{G}'(x)$ vanishes in a neighbourhood of $\chi$, then $x$ belongs to I in a neighbourhood of $\chi$.

2) If $x$ belongs to I in a neighbourhood of $\chi$ and $y\in A$ is an arbitrary element, then $xy$ belongs to I in a neighbourhood of $\chi$.

3) The set of $\chi$ such that $x$ belongs to I in a neighbourhood of $\chi$ is open in $\mathsf{X}'(A)$.

4) Suppose that A is regular and without radical. If $x$ belongs to I in a neighbourhood of $\chi$ for every $\chi \in \mathsf{X}'(A)$, then $x$ belongs to I (Cor. 2 of I, p. 91 applied to the function $f=\mathscr{G}'(x)$ and Prop. 8 of I, p. 38).

5) Suppose that A is regular. Let I be an ideal of A and $\chi$ an element of $\mathsf{X}(A)$ such that $\chi \notin V(I)$. Then every element $x$ of A belongs to I in a neighbourhood of $\chi$. In fact, by Definition 1 of I, p. 89, there exists a $z\in A$ such that $\mathscr{G}'(z)$ is equal to 1 in a neighbourhood of $\chi$, and equal to 0 in a neighbourhood of V(I). The support of $\mathscr{G}(z)$ is compact and therefore one has $z\in I$ (Prop. 4 applied to V(I)), hence $xz\in I$, and $\mathscr{G}'(xz) =\mathscr{G}'(x)$ in a neighbourhood of $\chi$.

Recall that a subspace K of a topological space X is said to be perfect if it is closed and has no isolated point (TG, I, p. 8).

#### Lemma 1 {#ts-i-s5-lem-1 .statement tag=02C8}

Let A be a commutative regular Banach algebra without radical, satisfying Ditkin's condition. Let I be a closed ideal of A and $x$ an element of Υ(V(I)). Let K be the set of $\chi \in \mathsf{X}'(A)$ such that $x$ does not belong to I in a neighbourhood of $\chi$. Then the set K is a perfect subset of $\mathsf{X}'(A)$.

Let G denote the complement of K in $\mathsf{X}'(A)$. The set G is open in $\mathsf{X}'(A)$ (Remark 3), therefore K is closed.

We proceed by contradiction, and suppose that K has an isolated point $\chi_0$. Let U denote a neighbourhood of $\chi_0$ such that U $-\{\chi_0\} \subset G$. Since $x$ does not belong to I in a neighbourhood of $\chi_0$, Remark 5 shows that $\chi_0\in V(I)$. In particular, one has $\chi_0(x) = 0$ since $x\in \Upsilon (V(I))$.

We shall show that there exists an element $y$ of A which belongs to I in a neighbourhood of every point of $\mathsf{X}'(A)-\{\chi_0\}$, which does not belong to I in a neighbourhood of $\chi_0$, and such that $\chi_0(y) = 0$.

Suppose first that the existence of such an element $y$ has been proved. Since A satisfies Ditkin's condition, there then exists a sequence $(x_n)$ in A such that $x_ny$ tends to $y$ and such that each $\mathscr{G}'(x_n)$ vanishes in a neighbourhood of $\chi_0$. For every $n$, the element $x_ny$ then belongs to I in a neighbourhood of every point of $\mathsf{X}'(A)$ (Remarks 1 and 2) and therefore $x_ny\in I$ (Remark 4). Since I is closed, one deduces that $y\in I$, which contradicts the fact that $y$ does not belong to I in a neighbourhood of $\chi_0$.

It remains to prove the existence of $y$. If $\chi_0\not= 0$, by assertion (iii) of Prop. 1 of I, p. 88, there exists a $u\in A$ such that $\mathscr{G}'(u)$ is equal to 1 in a neighbourhood of $\chi_0$ and equal to 0 in a neighbourhood of $\mathsf{X}'(A)$ - U. Let $y=ux$. Since $x$ belongs to I in a neighbourhood of $\chi$ for every $\chi \in U-\{\chi_0\}$, the same is true of $y$. Moreover, if $\chi \in \mathsf{X}'(A)$ - U, then $\mathscr{G}'(y)$ vanishes in a neighbourhood of $\chi$. Therefore (Remark 5) the element $y=ux$ belongs to I in a neighbourhood of every $\chi \not=\chi_0$. Since $\mathscr{G}'(y)$ coincides with $\mathscr{G}'(x)$ in a neighbourhood of $\chi_0$, the fact that $\chi_0$ belongs to K implies that $y$ does not belong to I in a neighbourhood of $\chi_0$. Finally, one has $\chi_0(y) =\chi_0(u)\chi_0(x) = 0$.

If $\chi_0= 0$, there similarly exists an element $v\in A$ such that $\mathscr{G}'(v)$ is zero in a neighbourhood of $\chi_0$ and equal to 1 in a neighbourhood of $\mathsf{X}'(A)$- U; as above, one deduces that the element $y=x-vx$ belongs to I in a neighbourhood of every $\chi \not=\chi_0$, that it does not belong to I in a neighbourhood of $\chi_0$, and that $\chi_0(y) = 0$.

#### Lemma 2 {#ts-i-s5-lem-2 .statement tag=02C9}

Let X be a topological space. Let F and D be disjoint subspaces of X such that F is closed and D discrete. If F contains no nonempty perfect subspace, the same is true of $F\cup D$.

Suppose indeed that K is a nonempty perfect subspace of $F\cup D$. Let $x$ be a point of K. If $x$ belongs to D, it is isolated in D, hence also in $F\cup D$ since F is closed. Therefore $x$ is isolated in K, which contradicts the assumptions.

#### Proposition 5 {#ts-i-s5-prop-5 .statement tag=02CA}

Let A be a regular commutative Banach algebra without radical, satisfying Ditkin's condition. Let I be a closed ideal of A such that the boundary F of V(I) contains no nonempty perfect set. Then I = Υ(V(I)), that is to say that I is the set of $x\in A$ such that $\mathscr{G}(x)$ vanishes on V(I). In particular, if V(I) reduces to a point $\chi$, one has I = Ker($\chi$ ).

One has $I\subset \Upsilon (V(I))$. Let now $x\in \Upsilon (V(I))$. Let G be the set of characters $\chi \in \mathsf{X}'(A)$ such that $x$ belongs to I in a neighbourhood of $\chi$. It is open and its complement K is perfect (Lemma 1). Since $\mathscr{G}'(x)$ is zero on V(I), the set G contains the interior of $V(I)\cup  \{0\}$ (Remark 1). It also contains $\mathsf{X}(A)$- V(I) by Remark 5. Therefore $K =\mathsf{X}'(A)$ - G is contained in the boundary $F_0$ of $V(I)\cup  \{0\}$. One has $F_0\subset F\cup  \{0\}$. The assumption therefore implies that $F_0$ contains no nonempty perfect set (Lemma 2). It therefore follows from Lemma 1 that the perfect set K is empty. Therefore $x$ belongs to I in a neighbourhood of every $\chi \in \mathsf{X}'(A)$, which means that $x\in I$ (Remark 4). Thus $\Upsilon (V(I))\subset$ I, which concludes the proof.

## EXERCISES {#ts-i-s5-exercises}

In the exercises below, all the algebras considered are over $\mathbf{C}$.

See the [exercises for § 5](exercises/s5/).
