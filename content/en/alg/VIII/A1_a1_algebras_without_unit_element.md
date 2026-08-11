---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Semisimple Modules and Rings
section: 1
section_title: Algebras without Unit Element
appendix: true
lang: en
source: alg-viii
source_edition: 2023, Springer Nature
book_pages: A VIII.435-A VIII.446
pdf_pages: 0452-0463
extraction: native
subsections:
    - "no": 1
      title: Regular Ideals
      page: 435
      pdf_page: 452
    - "no": 2
      title: Adjunction of a Unit Element
      page: 437
      pdf_page: 454
    - "no": 3
      title: The Radical of an Algebra
      page: 439
      pdf_page: 456
    - "no": 4
      title: Density Theorem
      page: 442
      pdf_page: 459
statements: 18
exercises: 15
content_sha256: a8b7d45f49181f6c2f03fd71f8ebce65615fe083d4ca82191a59ce2cb8c944fb
---

## APPENDIX 1 ALGEBRAS WITHOUT UNIT ELEMENT

In this appendix, $k$ is a commutative ring; the $k$-algebras are assumed associative but not necessarily unital.

### 1. Regular Ideals

Let A be a $k$-algebra. Recall (III, §1, No. 2, p. 430) that a left ideal of A is a $k$-submodule $\mathfrak{a}$ of A such that the relations $a\in A, x\in \mathfrak{a}$ imply $ax\in \mathfrak{a}$. We define the notions of right ideal and two-sided ideal likewise. If A is a $k$-algebra and $\mathfrak{a}$ a two-sided ideal of A, then when passing to the quotients, the multiplication in A defines a $k$-algebra structure on the $k$-module $A/\mathfrak{a}$ (loc. cit.).

A left ideal of A is called maximal if it is a maximal element of the set of proper left ideals of A for the inclusion.

#### Definition 1 {#alg-viii-a1-def-1 .statement}

Let A be a $k$-algebra and $\mathfrak{a}$ a left ideal of A. An element $u$ of A such that $au-a$ belongs to $\mathfrak{a}$ for every $a\in A$ is called a right unit modulo $\mathfrak{a}$. We say that the ideal $\mathfrak{a}$ is regular if there exists a right unit modulo $\mathfrak{a}$.

Likewise, we say that a right ideal $\mathfrak{b}$ of A is regular if A has a left unit modulo $\mathfrak{b}$, that is, an element $v$ such that $va-a\in \mathfrak{b}$ for every $a\in A$. When an ideal is two-sided, one needs to specify whether it is regular as a left ideal or as a right ideal.

When the algebra A is unital, the unit element of A is a right unit modulo $\mathfrak{a}$ for every left ideal $\mathfrak{a}$ of A; in this case, every left (or right) ideal of A is regular. On the other hand, if A is a $k$-algebra whose elements are all nilpotent, then A is the only (left or right) ideal of A that is regular.

Let $\mathfrak{a}$ be a regular left ideal of A and $u$ a right unit modulo $\mathfrak{a}$. If $\mathfrak{b}$ is a left ideal of A containing $\mathfrak{a}$, then $u$ is a right unit modulo $\mathfrak{a}$, so $\mathfrak{b}$ is regular. So the left ideals of A that are maximal and regular are the maximal elements of the set of regular proper left ideals of A. Moreover, a left ideal $\mathfrak{b}$ of A containing $\mathfrak{a}$ is proper if and only if $u$ does not belong to $\mathfrak{b}$. The set of proper left ideals $\mathfrak{b}$ of A containing $\mathfrak{a}$, ordered by inclusion, is therefore an inductive set. Theorem 2 of Set Theory, III, §2, No. 4, p. 154 applied to this set gives the following result.

#### Proposition 1 {#alg-viii-a1-prop-1 .statement}

Every regular proper left (resp. right) ideal of A is contained in a regular maximal left (resp. right) ideal.

#### Proposition 2 {#alg-viii-a1-prop-2 .statement}

Let A be a commutative $k$-algebra. An ideal $\mathfrak{a}$ of A is a regular maximal ideal if and only if the pseudoring $A/\mathfrak{a}$ (I, §8, No. 1, p. 98) is a field.

An element $u$ of A is a (right or left) unit modulo $\mathfrak{a}$ if and only if the canonical image of $u$ in $A/\mathfrak{a}$ is a unit element of the algebra $A/\mathfrak{a}$. Therefore, the ideal $\mathfrak{a}$ is regular if and only if the algebra $A/\mathfrak{a}$ is unital. Suppose that these conditions are satisfied.

The mapping $\mathfrak{b}\mapsto \mathfrak{b}/\mathfrak{a}$ is a bijection from the set of ideals of the algebra A containing $\mathfrak{a}$ to the set of ideals of the algebra $A/\mathfrak{a}$. These are the ideals of the ring $A/\mathfrak{a}$ because this algebra is unital. Finally, by Theorem 1 of I, §9, No. 1, p. 115, the ring $A/\mathfrak{a}$ is a field if and only if it is nonzero and its only ideals are 0 and itself. The proposition follows.

#### Example 1 {#alg-viii-a1-n1-exa-1 .statement}

Let V be an infinite-dimensional vector space over a commutative field K. Let End$^f_K(V)$ be the K-subalgebra of End$_K(V)$ consisting of the endomorphisms of finite rank. Let W be a linear subspace of V, and let $\mathfrak{a}_W$ be the set of elements of End$^f_K(V)$ whose kernel contains W; it is a left ideal of End$^f_K(V)$. An element $u$ of End$^f_K(V)$ is a right unit modulo $\mathfrak{a}_W$ if and only if we have $u(x) =x$ for every $x\in W$. Such an element $u$ exists, that is, $\mathfrak{a}_W$ is regular, if and only if W is finite-dimensional. The ideal $\mathfrak{a}_W$ is maximal and regular if and only if W has dimension 1.

#### Example 2 {#alg-viii-a1-n1-exa-2 .statement}

Let T be a locally compact space, and let $\mathscr{C}_0(T)$ be the commutative $\mathbf{C}$-algebra of continuous mappings from T to $\mathbf{C}$ that tend to 0 at infinity (Gen. Top., X, §4, No. 4, p. 316); it is unital if and only if T is compact. Let F be a closed subset of T, and let $\mathfrak{a}_F$ be the set of elements of $\mathscr{C}_0(T)$ whose restriction to F is the zero function; it is an ideal of $\mathscr{C}_0(T)$. An element $u$ of $\mathscr{C}_0(T)$ is a unit modulo $\mathfrak{a}_F$ if and only if we have $u(t) = 1$ for every $t\in F$. Such an element $u$ exists, that is, $\mathfrak{a}_F$ is regular, if and only if F is compact. The mapping $t\mapsto \mathfrak{a}_{\{t\}}$ is a bijection from T to the set of regular maximal ideals of $\mathscr{C}_0(T)$ (TS, I, §3, n$^o2$, p. 32, corollaire 1). Suppose that T is not compact, and denote by $\mathfrak{a}$ the subset of $\mathscr{C}_0(T)$ consisting of the functions with compact support; then $\mathfrak{a}$ is an ideal of $\mathscr{C}_0(T)$ that is not contained in any regular ideal of $\mathscr{C}_0(T)$.

#### Example 3 {#alg-viii-a1-n1-exa-3 .statement}

Let $L^1(\mathbf{R})$ be the convolution algebra of the locally compact group $\mathbf{R}$. Recall (cf. Int., VIII, §4, No. 5, p. 38) that $L^1(\mathbf{R})$ is the space of classes of functions on $\mathbf{R}$ that are integrable for the Lebesgue measure. The product of the classes of two functions $f$ and $g$ is the class of the function $f*g$ defined by the formula

$$
(f*g)(s) =\int_{-\infty}^{+\infty}f(t)g(s-t)dt
$$

for almost every $s\in \mathbf{R}$. The algebra $L^1(\mathbf{R})$ is not unital. For any $a$ in $\mathbf{R}$, denote by $\mathfrak{m}_a$ the set of elements $f$ of $L^1(\mathbf{R})$ satisfying

$$
\int_{-\infty}^{+\infty}f(t)e^{-iat}dt= 0
$$

By TS, II, §3, n$^o2$, p. 252, théorème 1, the mapping $a\mapsto \mathfrak{m}_a$ is a bijection from $\mathbf{R}$ to the set of regular maximal ideals of the algebra $L^1(\mathbf{R}).*$

### 2. Adjunction of a Unit Element

Let A be a $k$-algebra. In III, §1, No. 2, p. 431, we defined the unital algebra $\widetilde{A}$ deduced from A by the adjunction of a unit element $e$. We identify A with a two-sided ideal of $\widetilde{A}$. The $k$-module $\widetilde{A}$ is the direct sum of the submodules $ke$ and A.

#### Proposition 3 {#alg-viii-a1-prop-3 .statement}

a) Let $\widetilde{\mathfrak{a}}$ be a left ideal of $\widetilde{A}$ such that $\widetilde{A} =\widetilde{\mathfrak{a}}+ A$. We set $\mathfrak{a}=\widetilde{\mathfrak{a}}\cap A$. There exists an element $u$ of A such that $u-e$ belongs to $\widetilde{\mathfrak{a}}$. If $u$ is such an element, then it is a right unit of A modulo $\mathfrak{a}$, and we have $\widetilde{\mathfrak{a}}=\mathfrak{a}+k(u-e)$; in particular, the ideal $\mathfrak{a}$ is regular.

b) Conversely, let $\mathfrak{a}$ be a regular left ideal of A and $u$ a right unit of A modulo $\mathfrak{a}$. Set $\widetilde{\mathfrak{a}}=\mathfrak{a}+k(u-e)$. Then $\widetilde{\mathfrak{a}}$ is a left ideal of $\widetilde{A}$ such that $\widetilde{A} =\widetilde{\mathfrak{a}}+ A$, and we have $\mathfrak{a}=\widetilde{\mathfrak{a}}\cap A$.

c) If $k$ is a field, then the condition $\widetilde{A} =\widetilde{\mathfrak{a}}+ A$ is equivalent to saying that $\widetilde{\mathfrak{a}}$ is not contained in A.

Under the assumption of a), the element $e$ of $\widetilde{A}$ can be written as $(e-u)+u$ with $u\in A$ and $u-e\in \widetilde{\mathfrak{a}}$. Let $x=\lambda e+a$ be an element of $\widetilde{A}$, where $\lambda \in k$ and $a\in A$; if $x$ belongs to $\widetilde{\mathfrak{a}}$, then the element $y=a+\lambda u=x+\lambda (u-e)$ of A belongs to $\mathfrak{a}$, and we have $x=y-\lambda (u-e)$; this proves the equality $\widetilde{\mathfrak{a}}=\mathfrak{a}+k(u-e)$. Moreover, for every $a$ in A, the element $au-a=a(u-e)$ of A belongs to $\mathfrak{a}$, so $u$ is a right unit modulo $\mathfrak{a}$. This proves assertion a).

Let $\mathfrak{a}$ and $u$ be as in b). Since $\widetilde{A}$ is the direct sum of A and $k(u-e)$, we have $\widetilde{\mathfrak{a}}+ A =\widetilde{A}$ and $\widetilde{\mathfrak{a}}\cap A =\mathfrak{a}$. Every element of $\widetilde{\mathfrak{a}}$ is of the form $x+\lambda (u-e)$ with $x\in \mathfrak{a}$ and $\lambda \in k$. For every $a\in A$, we have

$$
a(x+\lambda (u-e)) =ax+\lambda (au-a)
$$

Since $u$ is a right unit of A modulo $\mathfrak{a}$, the sum $ax+\lambda (au-a)$ belongs to $\mathfrak{a}$, so that $\widetilde{\mathfrak{a}}$ is a left ideal of A. This proves b).

Finally, if $k$ is a field, then A is a hyperplane in $\widetilde{A}$, and $\widetilde{A}$ is the sum of $\widetilde{\mathfrak{a}}$ and A if and only if $\widetilde{\mathfrak{a}}$ is not contained in A.

#### Corollary {#alg-viii-a1-n2-cor-1 .statement}

The regular left ideals of A are the ideals of the form $A\cap \widetilde{\mathfrak{a}}$, where $\widetilde{\mathfrak{a}}$ is a left ideal of $\widetilde{A}$ such that $\widetilde{A} =\widetilde{\mathfrak{a}}+ A$.

#### Proposition 4 {#alg-viii-a1-prop-4 .statement}

a) Let $\mathfrak{a}$ be a regular maximal left ideal of A. There exists a unique left ideal $\widetilde{\mathfrak{a}}$ of $\widetilde{A}$ such that $\widetilde{A} =\widetilde{\mathfrak{a}}+ A$ and $\mathfrak{a}=\widetilde{\mathfrak{a}}\cap A$. This ideal is maximal and does not contain A.

b) The mapping $\widetilde{\mathfrak{a}}\mapsto \widetilde{\mathfrak{a}}\cap A$ is a bijection from the set of maximal left ideals of $\widetilde{A}$ not containing A to the set of regular maximal left ideals of A.

Let $\mathfrak{a}$ be a regular maximal left ideal of A. By Proposition 3, a), the left ideals $\mathfrak{b}$ of $\widetilde{A}$ such that $\mathfrak{b}+ A =\widetilde{A}$ and $\mathfrak{b}\cap A =\mathfrak{a}$ are the ideals $\mathfrak{a}+k(u-e)$, where $u$ is a right unit modulo $\mathfrak{a}$. To prove the uniqueness of $\widetilde{\mathfrak{a}}$, it therefore suffices to prove that two right units $u$ and $u'$ of A modulo $\mathfrak{a}$ are congruent modulo $\mathfrak{a}$. Let us reason by contradiction and suppose that $u-u'$ does not belong to $\mathfrak{a}$. The formula $x(u-u') = (xu-x)-(xu'-x)$ shows that we have $A(u-u')\subset \mathfrak{a}$; it follows that $\mathfrak{a}+k(u-u')$ is a left ideal of A containing $\mathfrak{a}$ and distinct from $\mathfrak{a}$. Since $\mathfrak{a}$ is maximal, we therefore have $\mathfrak{a}+k(u-u') = A$, and so AA $\subset \mathfrak{a}$. For every $x\in A$, we have $x\equiv xu$ (mod $\mathfrak{a})$, and therefore $x\in \mathfrak{a}$ by the above, which contradicts the assumption $\mathfrak{a}\not= A$.

Hence there exists a unique left ideal $\widetilde{\mathfrak{a}}$ of $\widetilde{A}$ such that $\widetilde{A} =\widetilde{\mathfrak{a}}+ A$ and $\mathfrak{a}=\widetilde{\mathfrak{a}}\cap A$. Let $\mathfrak{b}$ be a proper left ideal of $\widetilde{A}$ containing $\widetilde{\mathfrak{a}}$. Then $\mathfrak{b}\cap A$ is a proper left ideal of A containing $\mathfrak{a}$. It is therefore equal to $\mathfrak{a}$ because $\mathfrak{a}$ is maximal, which implies $\mathfrak{b}=\widetilde{\mathfrak{a}}$ by Lemma 2 of VIII, p. 4. This proves that $\widetilde{\mathfrak{a}}$ is a maximal ideal of $\widetilde{A}$; for such an ideal, the condition $\widetilde{A} =\widetilde{\mathfrak{a}}+ A$ means that $\widetilde{\mathfrak{a}}$ does not contain A.

It remains to prove that if $\widetilde{\mathfrak{a}}$ is a maximal left ideal of $\widetilde{A}$ that does not contain A, then the left ideal $\mathfrak{a}= A\cap \widetilde{\mathfrak{a}}$ of A is maximal. Let $\mathfrak{b}$ be a proper left ideal of A containing $\mathfrak{a}$. Let $u$ be a right unit modulo $\mathfrak{a}$ such that $\widetilde{\mathfrak{a}}=\mathfrak{a}+k(u-e)$ (Proposition 3). It is also a right unit modulo $\mathfrak{b}$; denote by $\widetilde{\mathfrak{b}}$ the ideal $\mathfrak{b}+k(u-e)$ of $\widetilde{A}$. By Proposition 3, b), we have $\mathfrak{b}= A\cap \widetilde{\mathfrak{b}}$. The ideal $\widetilde{\mathfrak{a}}$, equal to $\mathfrak{a}+k(u-e)$, is contained in $\widetilde{\mathfrak{b}}$ and is therefore equal to $\widetilde{\mathfrak{b}}$ because $\widetilde{\mathfrak{b}}$ is distinct from $\widetilde{A}$ and $\widetilde{\mathfrak{a}}$ is maximal. Consequently, we have $\mathfrak{a}=\mathfrak{b}$, and $\mathfrak{a}$ is maximal.

We leave it to the reader to translate Propositions 3 and 4 to right ideals.

### 3. The Radical of an Algebra

Let A be a $k$-algebra. A left pseudomodule over A is a $k$-module M endowed with the structure of a left pseudomodule over the pseudoring A (II, Appendix, No. 2, p. 378) such that we have $a(\lambda x) =\lambda (ax) = (\lambda a)x$ for $\lambda \in k$, $a\in A$, and $x\in M$. We define right pseudomodules over A likewise.

Let M be a left pseudomodule over A; we define a left $\widetilde{A}$-module structure on M called canonical by setting

$(\lambda e+a)x=\lambda x+ax$ for $\lambda \in k, a\in A, x\in M$.

Conversely, every left $\widetilde{A}$-module is canonically endowed, by restricting the ring of operators to $k$ and A, with the structure of a left pseudomodule over A. Thus, the species of structures of left pseudomodules over A and of modules over $\widetilde{A}$ are equivalent (Set Theory, IV, §1, No. 7, p. 262).

Let M be a left pseudomodule over A, and let N be a $k$-submodule of M. Then N is an $\widetilde{A}$-submodule of M if and only if it is stable under the action of A; we then say that N is a sub-pseudomodule of M.

As in the case of rings, we define the left pseudomodule $A_s$ over A and the right pseudomodule $A_d$. The left (resp. right) ideals of A are the sub-pseudomodules of $A_s$ (resp. $A_d)$.

Let $\mathfrak{a}$ be a regular left ideal of A and $u$ a right unit modulo $\mathfrak{a}$. Set $M = A_s/\mathfrak{a}$, and denote the image of $u$ in M by $z$. We have $M = Az$, and $\mathfrak{a}$ is the annihilator of $z$.

Conversely, let M be a left pseudomodule over A, and let $z$ be an element of M such that $M = Az$. Then there exists an element $u$ of A such that $z=uz$. For every $a\in A$, we have $(au-a)z= 0$, so $au-a$ belongs to the annihilator $\mathfrak{a}$ of $z$. Consequently, $\mathfrak{a}$ is a regular left ideal of A, the element $u$ is a right unit modulo $\mathfrak{a}$, and when passing to the quotient, the mapping $a\mapsto az$ defines an isomorphism from $A_s/\mathfrak{a}$ to M.

#### Definition 2 {#alg-viii-a1-def-2 .statement}

We say that a pseudomodule M over A is simple if we have AM $\not= 0$ and if 0 and M are the only sub-pseudomodules of M.

This corresponds to saying that the $\widetilde{A}$-module M is simple and that its annihilator does not contain A. When A is a ring and M is an A-module, we have AM = M, so Definition 2 coincides with Definition 1 of VIII, p. 45.

#### Proposition 5 {#alg-viii-a1-prop-5 .statement}

a) Let $\mathfrak{m}$ be a regular maximal left ideal of A. Then the pseudomodule $A_s/\mathfrak{m}$ is simple, and there exists a nonzero element of $A_s/\mathfrak{m}$ with annihilator $\mathfrak{m}$.

b) Let M be a simple pseudomodule, and let $x$ be a nonzero element of M. We have $M = Ax$, the annihilator $\mathfrak{m}$ of $x$ is a regular maximal left ideal of A, and when passing to the quotient, the mapping $a\mapsto ax$ defines an isomorphism from $A_s/\mathfrak{m}$ to M.

c) Let M be a pseudomodule not reduced to 0. Then M is simple if and only if we have $M = Ax$ for every nonzero element $x$ of M.

Let $\mathfrak{m}$ be a regular maximal left ideal of A. We have seen that there exists a nonzero element $z$ of $A_s/\mathfrak{m}$ with annihilator equal to $\mathfrak{m}$ and such that $Az= A_s/\mathfrak{m}$; in particular, we have $A(A_s/\mathfrak{m})\not= 0$. Moreover, every sub-pseudomodule of $A_s/\mathfrak{m}$ is of the form $\mathfrak{n}/\mathfrak{m}$, where $\mathfrak{n}$ is a left ideal of A containing $\mathfrak{m}$. Since $\mathfrak{m}$ is maximal, the only possibilities are $\mathfrak{n}=\mathfrak{m}$ and $\mathfrak{n}= A$, so that the pseudomodule $A_s/\mathfrak{a}$ is simple. This proves a).

Under the assumptions of b), the set of elements $y$ of M such that $Ay= 0$ is a sub-pseudomodule of M different from M and therefore reduced to 0. Consequently, $Ax$ is a nonzero sub-pseudomodule of M, which implies $M = Ax$. Assertion b) then follows from the remarks before Definition 2.

Let M be a nonzero pseudomodule. Suppose that we have $Ax= M$ for every nonzero element $x$ of M. In particular, we have AM $\not= 0$. Let N be a nonzero sub-pseudomodule of M, and let $x$ be a nonzero element of N. We have $Ax= M$, and therefore N = M. Hence M is simple. Conversely, if M is simple, then we have $M = Ax$ for every $x\not= 0$ by b). **Definition 3.** — The radical of the $k$-algebra A, denoted by $<(A)$, is the intersection of the regular maximal left ideals of A.

When A is a ring, every left ideal of A is regular, so the definition of the radical coincides with Definition 2 of VIII, p. 154.

#### Example 1 {#alg-viii-a1-n3-exa-1 .statement}

The radical of the $k$-algebra End$^f_k(V)$ is reduced to 0 (VIII, p. 436, Example 1$).*$ The same holds for the algebras $\mathscr{C}_0(T)$ and $L^1(\mathbf{R}).*$

#### Example 2 {#alg-viii-a1-n3-exa-2 .statement}

Let A be a pseudoring in which all elements are nilpotent. The radical of A is equal to A because A is the only regular left ideal.

Proposition 5 immediately implies the following result.

#### Proposition 6 {#alg-viii-a1-prop-6 .statement}

The radical of the algebra A is the intersection of the annihilators of the simple pseudomodules. It is, in particular, a two-sided ideal of A.

#### Proposition 7 {#alg-viii-a1-prop-7 .statement}

The radical of A is the trace on A of the radical of $\widetilde{A}$; it is also equal to the radical of the opposite algebra $A^o($that is, to the intersection of the regular maximal right ideals of A). If the ring $k$ is without radical, then the radical of A is equal to that of $\widetilde{A}$.

The equality $<(\widetilde{A})\cap A =<(A)$ follows from Proposition 4 of VIII, p. 438, b). Since $\widetilde{A}$ and $\widetilde{A}^o$ have the same radical (VIII, p. 156, Corollary 1), the equality $<(A) =<(A^o)$ follows. If $k$ is without radical, then the intersection of the maximal left ideals of $\widetilde{A}$ containing A is equal to A. Consequently, $<(\widetilde{A})$ is contained in A and therefore equal to $<(A)$.

#### Remark {#alg-viii-a1-n3-rem-1 .statement}

Let $x$ and $y$ be elements of A; we say that $x$ is a left adverse of $y$, or that $y$ is a right adverse of $x$, if, in $\widetilde{A},x-e$ is a left inverse of $y-e$, that is, if we have $x+y=xy$. By Proposition 7 and Jacobson’s theorem (VIII, p. 156, Theorem 1), the radical of A consists of the elements $x$ of A such that $ux-e$ is left invertible in $\widetilde{A}$ for every $u$ in $\widetilde{A}$. Since we have $(a+\lambda e)x-e=ax+\lambda x-e$ (for $a\in A,\lambda \in k)$, the radical of A is the set of elements $x$ of A such that $ax+\lambda x$ has a left adverse in A for every $a\in A$ and $\lambda \in k$.

### 4. Density Theorem

Let A be a $k$-algebra. A left pseudomodule M is called semisimple if it is the direct sum of a family of simple left pseudomodules.

#### Lemma 1 {#alg-viii-a1-lem-1 .statement}

Let M be a semisimple left A-pseudomodule. Let B be the bicommutant of the $\widetilde{A}$-module M. Then every A-sub-pseudomodule of M is a B-submodule of M.

The $\widetilde{A}$-module M is semisimple. Let N be an A-sub-pseudomodule of M. Then N is an $\widetilde{A}$-submodule of M. By Corollary 2 of VIII, p. 56, there exists a projector $p$ of the A-module M with image N. Since we have the relation $pb=bp$ for every $b\in B$, we obtain that N is a B-submodule of M.

#### Lemma 2 {#alg-viii-a1-lem-2 .statement}

Let M be a semisimple left A-pseudomodule, and let $x$ be an element of M. There exists an element $a\in A$ such that $ax=x$.

Let N be the left A-pseudomodule $\widetilde{A}x/Ax$. It satisfies AN $=\{0\}$. By Corollary 3 of VIII, p. 56 applied to the $\widetilde{A}$-modules M and $\widetilde{A}x$, the A-pseudomodule N is semisimple. By definition, every simple sub-pseudomodule S of N satisfies AS $\not=\{0\}$. Consequently, the pseudomodule N is zero, and we obtain that $x\in Ax$.

Theorem 1 (Jacobson’s density theorem). — Let M be a semisimple left A-pseudomodule. Let $b$ be an element of the bicommutant of the $\widetilde{A}$-module M. Let $F =\{x_1, . . . , x_n\}$ be a finite subset of M. Then there exists an element $a\in A$ such that $bx_i=ax_i$ for every $i\in [1, n]$.

Let B be the bicommutant of the $\widetilde{A}$-module M. The A-pseudomodule $M^n$ is semisimple. Let $\boldsymbol{x}= (x_1, . . . , x_n)\in M^n$. It follows from Lemma 2 that $\boldsymbol{x}\in$ $A\boldsymbol{x}$. The bicommutant of the $\widetilde{A}$-module $M^n$ coincides with the homotheties of the B-module $M^n$ (VIII, p. 79, Proposition 2). By Lemma 1, the A-sub-pseudomodule $A\boldsymbol{x}$ of $M^n$ is therefore a B-submodule of $M^n$. We therefore have the inclusion $B\boldsymbol{x}\subset A\boldsymbol{x}$. So there exists an $a\in A$ such that $b\boldsymbol{x}=a\boldsymbol{x}$. The result follows.

### Exercises {#alg-viii-a1-exercises}

1) Let A be a $k$-algebra. a) Prove that the only regular (left or right) ideal containing AA is A. b) A two-sided ideal $\mathfrak{a}$ of A is regular as a left ideal and as a right ideal if and only if the $k$-algebra $A/\mathfrak{a}$ is unital.

2) Let A be a $k$-algebra, and let $\mathfrak{a}$ and $\mathfrak{b}$ be regular (left) ideals of A. a) The ideal $\mathfrak{a}\cap \mathfrak{b}$ is regular if and only if there exist right units $u$ modulo $\mathfrak{a}$ and $v$ modulo $\mathfrak{b}$ such that $u-v\in \mathfrak{a}+\mathfrak{b}$. b) Deduce that $\mathfrak{a}\cap \mathfrak{b}$ is regular if $\mathfrak{a}$ is two-sided and right regular, or if $\mathfrak{a}$ is maximal. c) Let K be a commutative field, L be the free associative K-algebra in two variables X and Y (III, §2, No. 7, p. 448), and A be the K-subalgebra of L consisting of the elements of degree $\geqslant 1$. Prove that the ideals $A(1-X)$ and $A(1-Y)$ of A are regular but that their intersection is reduced to 0.

3) Let A be a $k$-algebra, $\mathfrak{a}$ a regular left ideal of A, and $u$ and $v$ right units modulo $\mathfrak{a}$. a) Give an example where $u-v$ does not belong to $\mathfrak{a}$ (cf. III, §9, p. 644, Exercise 1). Deduce an example where the mapping $\widetilde{\mathfrak{a}}\mapsto \widetilde{\mathfrak{a}}\cap A$ (Proposition 3 of VIII, p. 437) is not injective. b) Suppose that the ideal $\mathfrak{a}$ is two-sided and that the $k$-algebra $B = A/\mathfrak{a}$ does not contain any nonzero two-sided ideal $\mathfrak{b}$ such that $B\mathfrak{b}= 0$. Prove that $u-v$ belongs to $\mathfrak{a}$. This is, in particular, the case when A is commutative.

4) Let A be a $k$-algebra and $\mathfrak{a}$ a left ideal of A; we view $\mathfrak{a}$ as a $k$-algebra. Prove that we have $<(A)\cap \mathfrak{a}\subset  <(\mathfrak{a})$ (apply Proposition 7 of VIII, p. 441) and that we have equality when $\mathfrak{a}$ is two-sided (observe that every simple pseudomodule over A is simple over $\mathfrak{a}$ or annihilated by $\mathfrak{a})$. Give an example of a left ideal $\mathfrak{a}$ such that $<(A)\cap \mathfrak{a}\not=<(\mathfrak{a})$ (take A to be a matrix algebra).

$\P 5)$ Suppose that every pseudomodule M over A is the direct sum of AM and the sub-pseudomodule of M consisting of the elements annihilated by A. Prove that A is unital. (Taking $M =\widetilde{A}_s$, prove that A admits a right unit element $u$. Taking $M = A_s$, prove that we have $Ax\not= 0$ for every nonzero element $x$ of A. Conclude that $u$ is also a left unit element.)

6) We say that a $k$-algebra is primitive if it admits a pseudomodule that is simple and faithful (that is, whose annihilator is reduced to 0). a) Show that if the algebra $\widetilde{A}$ is primitive, then so is A. b) If the algebra A is primitive and unital, then the algebra $\widetilde{A}$ is not primitive. c) Suppose that $k$ is a field and that the algebra A is primitive and not unital. Prove that $\widetilde{A}$ is primitive (prove that if there exists a faithful pseudomodule over A that is not faithful as an $\widetilde{A}$-module, then A admits a right unit element $u$, and deduce a contradiction).

7) We say that the $k$-algebra A is Artinian if every decreasing sequence of left ideals of A is stationary. The ring $\widetilde{A}$ is Artinian if and only if the algebra A and the ring $k$ are Artinian. Prove that if $k$ is a field, then an Artinian algebra A without radical is unital (observe that the algebra $\widetilde{A}$ is semisimple).

8) Suppose that $k$ is a field and that A is a primitive algebra over $k$. Prove that if A admits a finite-dimensional nonzero left ideal over $k$, then the algebra A is finite-dimensional over $k$ and consequently a simple ring (cf. Exercise 7).

9) Suppose that $k$ is a field and that A is a nilpotent $k$-algebra, that is, that there exists an integer $n$ such that $A^n= 0$. Prove that A is finite-dimensional over $k$ (use induction on the least integer $n$ such that $A^n= 0)$.

10) Suppose that $k$ is a field, that A is an infinite-dimensional $k$-algebra, and that every proper left ideal of A is finite-dimensional over $k$. a) Prove that we have $A\mathfrak{a}= 0$ for every left ideal $\mathfrak{a}\not= A$ (consider the homomorphism $\gamma : A\rightarrow$ End$_k(\mathfrak{a}))$. b) Let $\mathfrak{r}$ be the sum of the maximal left ideals of A. Prove that $\mathfrak{r}$ is different from A (use Exercise 9), that $\mathfrak{r}$ is a two-sided ideal, and that $A/\mathfrak{r}$ is a field (cf. Exercise 7). c) Let $u$ be a (left or right) unit modulo $\mathfrak{r}$. Prove that we have $\mathfrak{r}u=\mathfrak{r}$ (observe that we have $Au= A)$. d) Prove that $\mathfrak{r}A$ is zero (consider the right annihilator of $\mathfrak{r}$ in A and reason as in a)) and then that $\mathfrak{r}$ is zero. Conclude that A is a field.

$\P 11)$ Suppose that $k$ is a field, that A is a $k$-algebra, and that every decreasing sequence of subalgebras of A is stationary. a) Prove that the algebra A is Artinian and that its radical is finite-dimensional over $k$ (apply Exercise 9). b) Let S be a simple component of $A/<(A)$ (Exercise 7); it is isomorphic to a matrix algebra over a field D, with center Z. Prove that D is finite-dimensional over Z (if D contains an element that is transcendental over Z, construct an infinite strictly decreasing sequence of subfields of D; if D is algebraic and infinite-dimensional over Z, construct an infinite strictly increasing sequence of subfields of D, and consider their commutants in D). c) Prove that if Z is infinite-dimensional over $k$, then we have S = D (consider the nilpotent subalgebras of B). d) Prove that Z is an algebraic extension of $k$. Let $p$ be the characteristic exponent of $k$ and L the largest separable extension of $k$ contained in Z. Prove that $L\cap Z^p$ has finite degree over $L^p$ (consider a $p$-basis of $L\cap Z^p$ over $L^p)$. e) Every decreasing sequence of subextensions of L is stationary. Give an example to show that this condition does not imply that L has finite degree over $k$ (cf. V, §12, p. 167, Exercise 3). f ) Conversely, let B be a $k$-algebra satisfying the conditions of a) such that every simple component of $B/<(B)$ satisfies the conditions of b), c), d), and e). Prove that every decreasing sequence of subalgebras of B is stationary.

(Reduce to the case when B is a field, with center Z. Let $(D_n)$ be a decreasing sequence of subfields of B; we may assume that the field D generated by $D_n$ and Z is independent of $n$. Observe that we can write $D = E\otimes_LZ$, where L is a subfield of Z of finite degree over $k$ and E is a field of finite degree over L whose center contains L. Prove that $D_n$ is then the field generated by E and $D_n\cap Z$. We are thus reduced to the case when B is a commutative field that is a $p$-radical extension of $k$. If $(F_n)$ is a decreasing sequence of subextensions of B, consider the subfield $k(F^p_{n^{\infty}})$, where $F^p_{n^{\infty}}=\cap_fF^p_{n^f}.)$

$\P 12)$ a) Suppose that $k$ is a field, that the $k$-algebra A is Artinian, and that every increasing sequence of subalgebras of A is stationary. Prove that A has finite degree over $k$. (Reason as in Exercise 11. Note that the field $k(X)$ contains an infinite strictly increasing sequence of subalgebras, using VII, §1, No. 5, p. 6, Proposition 6.) b) Prove that in the polynomial algebra $k[X]$, every increasing sequence of subalgebras is stationary. (Let $f\in k[X]$ be a nonconstant polynomial and A be the $k$-subalgebra of $k[X]$ generated by 1 and $f$. Observe that A is a principal ideal domain and $k[X]$ is a finitely generated A-module.)

13) Suppose that $k$ is a field and that A admits a finite basis over $k$ consisting of nilpotent elements. Prove that A is nilpotent (Exercise 9; reduce to the case when the algebra A is semisimple (cf. Exercise 7), and then of the form $\mathbf{M}_n(K)$ by extending the base field).

14) Let A and B be $k$-algebras; an $(A,B)$-pseudobimodule is a set E endowed with the structure of a left pseudomodule over A and the structure of a right pseudomodule over B such that the underlying $k$-module structures coincide. This corresponds to endowing E with the structure of a bimodule over the algebras $\widetilde{A}$ and $\widetilde{B}$. A multiplier of E is a pair $(S,D)$, where $S : B\rightarrow E$ is a homomorphism of right B-pseudomodules and $D : A\rightarrow E$ is a homomorphism of left A-pseudomodules, satisfying $aS(b) = D(a)b$ for $a\in A,b\in B$. We denote by $\mathscr{M}(E)$ the set of multipliers of E; it admits a natural $k$-module structure. a) For every $x\in E$, we denote by $D_x$ (resp. $S_x)$ the mapping $a\mapsto ax$ (resp. $b\mapsto xb)$. Show that the pair $m_x= (D_x,S_x)$ is a multiplier of E. b) For every $m= (S,D)\in \mathscr{M}$(E), $a\in A$, and $b\in B$, set $am=m_{D(a)}$ and $mb=m_{S(b)}$. Prove that this defines on the $k$-module $\mathscr{M}(E)$ the structure of a $(A$, B)-pseudobimodule and that the mapping $x\mapsto m_x$ is a homomorphism of $(A$, B)-pseudobimodules.

15) Let A be a $k$-algebra. A multiplier of A is a multiplier of the $(A,A)$-pseudobimodule A. We denote the $k$-algebra of multipliers of A by $\mathscr{M}(A)$. a) Prove that the mapping $µ:a\mapsto m_a$ is a $k$-algebra homomorphism and that we have $am=m_am$ and $ma=mm_a$ for $a\in A, m\in \mathscr{M}(A)$. The image of the homomorphism $µ$ is therefore a two-sided ideal of the ring $\mathscr{M}(A)$. b) A two-sided ideal $\mathfrak{b}$ of a $k$-algebra A is called faithful if its left and right annihilators are zero. Show that if A is faithful in A, then the homomorphism $µ$ is injective and the ideal $µ(A)$ is faithful in $\mathscr{M}(A)$. c) Let B be a unital $k$-algebra containing A as a two-sided ideal. For $b\in B$, let $\sigma_b$ and $\delta_b$ be the mappings from A to A such that for $a\in A$, we have $\sigma_b(a) =ba$ and $\delta_b(a) =ab$, and set $\pi (b) = (\sigma_b, \delta_b)$. Show that $\pi (b)\in \mathscr{M}(A)$ for every $b\in B$ and that the resulting mapping $\pi : B\rightarrow \mathscr{M}(A)$ is a ring homomorphism whose restriction to A is the mapping $a\mapsto m_a$. Show that $\pi$ is injective if the ideal A is faithful in B.
