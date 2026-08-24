---
book: alg
book_title: Algebra
chapter: V
chapter_title: COMMUTATIVE FIELDS
section: 1
section_title: Prime fields. Characteristic
lang: en
source: alg-iv-vii
source_edition: 2003, Springer
pdf_pages: 0115-0123, 0259-0260
extraction: ocr
subsections:
    - "no": 1
      title: Prime fields
      page: 0
      pdf_page: 115
    - "no": 2
      title: Characteristic of a ring and of a field
      page: 2
      pdf_page: 116
    - "no": 3
      title: Commutative rings of characteristic p
      page: 3
      pdf_page: 117
    - "no": 4
      title: Perfect rings of characteristic p
      page: 5
      pdf_page: 119
    - "no": 5
      title: Characteristic exponent of a field. Perfect fields
      page: 7
      pdf_page: 121
    - "no": 6
      title: Characterization of polynomials with zero differential
      page: 7
      pdf_page: 121
statements: 23
exercises: 5
content_sha256: 1386d6b11c452c9e28fae816dceda271a73d913c580b11b29f309d049d175b40
---

## § 1. PRIME FIELDS. CHARACTERISTIC

### 1. Prime fields

The field of fractions of the ring Z of rational integers is called the field of rational numbers and is denoted by Q (I, p. 117). For every prime number p the quotient ring $ \mathbf{Z}/(p) $ is a finite $ ^1 $ field of p elements, denoted by $ \mathbf{F}_p $ in the sequel. The field Q is infinite since it contains Z, and is therefore not isomorphic to any field $ \mathbf{F}_p $. If p and $ p' $ are distinct prime numbers, the fields $ \mathbf{F}_p $ and $ \mathbf{F}_{p'} $ have distinct cardinals and so are not isomorphic.

#### Definition 1 {#alg-v-s1-def-1 .statement}

A field is said to be prime if it is isomorphic either to Q or to one of the fields $ \mathbf{F}_p $.

Every subfield of Q contains the ring Z and hence the field of fractions Q of Z; every subring of $ \mathbf{F}_p $ is necessarily equal to $ \mathbf{F}_p $. Therefore every subfield of a prime field is necessarily equal to it (cf. Cor. 2 of Th. 1 below). Let P be a prime field and A a ring; if f and $ f' $ are two homomorphisms of P into A, then the set of $ x \in P $ such that $ f(x) = f'(x) $ is a subfield of P, hence by what has been said we must have $ f = f' $. In particular, the only endomorphism of a prime field is the identity mapping.

$ ^1 $ By abuse of language one says that a ring or field is finite if its underlying set is finite.

#### Theorem 1 {#alg-v-s1-thm-1 .statement}

— Let $ A $ be a ring ; suppose that there exists a subfield of $ A $. Then $ A $ has a unique subfield $ P $ which is a prime field. Moreover, $ P $ is contained in the centre of $ A $ and in every subfield of $ A $.

Let $ K $ be a subfield of $ A $, $ C $ the centre of $ A $, and put $ K' = K \cap C $; then $ K' $ is a subfield of $ A $. Let $ f $ be the unique homomorphism of $ \mathbf{Z} $ into $ A $ and $ p $ its kernel. Every subring of $ A $, in particular $ K' $, contains $ f(\mathbf{Z}) $; hence the ideal $ p $ is prime (I, p. 116-117). If $ p = (0) $, the homomorphism $ f $ of $ \mathbf{Z} $ into $ K' $ is injective; hence it extends (I, p. 116) to an isomorphism $ \bar{f} $ of $ \mathbf{Q} $ onto a subfield $ P $ of $ K' $. If $ p \neq (0) $, there is a strictly positive integer $ p $ such that $ p = (p) $ (I, p. 111); if we had $ p = ab $ with $ a > 1 $ and $ b > 1 $, this would mean $ a \notin p, b \notin p $ and $ ab \in p $ in contradiction with the fact that $ p $ is prime. The number $ p $ is therefore prime and by passage to quotients $ f $ defines an isomorphism of $ F_p = \mathbf{Z}/p $ onto a subfield $ P $ of $ K' $. In both cases $ P $ is a subfield of $ A $ contained in the centre $ C $ of $ A $, and it is a prime field. Let $ L $ be a subfield of $ A $; then $ P \cap L $ is a subfield of $ P $, and since $ P $ is prime, we have $ P \cap L = P $, whence $ P \subset L $. If $ P' $ is a subfield of $ A $ and is a prime field, then by what has been said, $ P \subset P' $, whence $ P = P' $ because $ P' $ is a prime field.

#### Corollary 1 {#alg-v-s1-thm-1-cor-1 .statement}

— Let $ K $ be a field. There exists a unique subfield of $ K $ which is a prime field, and this is the least subfield of $ K $.

#### Corollary 2 {#alg-v-s1-thm-1-cor-2 .statement}

— For a field to be prime it is necessary and sufficient that it should contain no subfield other than itself.

### 2. Characteristic of a ring and of a field

We shall define the characteristic of a ring $ A $ only when $ A $ has a subfield. When this is so, let $ f $ be the unique ring homomorphism of $ \mathbf{Z} $ into $ A $, and let $ n $ be the unique positive integer generating the ideal of $ \mathbf{Z} $ which is the kernel of $ f $ (I, p. 111); then the integer $ n $ is called the characteristic of $ A $.

Let $ A $ be a ring for which the characteristic is defined; then $ A $ does not reduce to 0. By Th. 1 there exists a unique subfield $ P $ of $ A $ which is a prime field; we shall call it the prime subfield of $ A $. By the proof of Th. 1 there are the following two possibilities:
$ a) $ the characteristic of $ A $ is 0, $ P $ is isomorphic to $ Q $,
$ b) $ the characteristic of $ A $ is a prime number $ p $, $ P $ is isomorphic to $ \mathbf{F}_p $.

If the characteristic of $ A $ is zero, there exists a unique ring homomorphism of $ Q $ into $ A $; its image is the prime subfield of $ A $, contained in the centre of $ A $. Therefore there exists a unique $ Q $-algebra structure of $ A $ compatible with the ring structure. When the characteristic of $ A $ is a prime number $ p $, we have the corresponding properties on replacing the field $ Q $ by the field $ \mathbf{F}_p $.

#### Proposition 1 {#alg-v-s1-prop-1 .statement}

— Let $ A $ be a ring not reduced to 0.
$ a) $ For $ A $ to be of characteristic 0 it is necessary and sufficient that the mapping $ x \mapsto n \cdot x $ of $ A $ into itself should be bijective, for every integer $ n \neq $

b) Let $ p $ be a prime number. For $ A $ to be of characteristic $ p $ it is necessary and sufficient that $ p \cdot x = 0 $ for all $ x \in A $.

Let $ f $ be the unique homomorphism of $ \mathbf{Z} $ into $ A $; we have $ n \cdot x = f(n)x $ for every integer $ n $ and every $ x $ in $ A $. For $ A $ to be of characteristic 0, it is necessary and sufficient that $ f $ should extend to a homomorphism of $ \mathbf{Q} $ into $ A $, that is, $ f(n) $ should be invertible in $ A $ for every $ n \neq 0 $ (I, p. 113); this proves $ a $. Similarly for $ A $ to be of characteristic $ p $ it is necessary and sufficient that $ f $ should annihilate $ p\mathbf{Z} $, that is, $ f(p) = 0 $, or also that $ p \cdot x = 0 $ for all $ x \in A $; this proves $ b $.

Let us take for $ A $ a not necessarily commutative field. The centre of $ A $ is a (commutative) field; therefore the characteristic and the prime subfield of $ A $ are defined.

#### Remark 1 {#alg-v-s1-n2-rem-1 .statement}

Let $ A $ and $ A' $ be two rings not reduced to 0. Suppose that the characteristic of $ A $ is defined and that there is a homomorphism $ u $ of $ A $ into $ A' $. The image under $ u $ of the prime subfield of $ A $ is a subfield $ P' $ of $ A' $, isomorphic to $ P $, and hence prime. It follows that the characteristic of $ A' $ is defined and is equal to that of $ A $. If $ A $ and $ A' $ are of characteristic 0 (resp. $ p \neq 0 $), the mapping $ u $ is a homomorphism of algebras over $ \mathbf{Q} $ (resp. $ \mathbf{F}_p $).

#### Remark 2 {#alg-v-s1-n2-rem-2 .statement}

Remark 1 shows that if $ A $ is a ring of characteristic 0 (resp. $ p \neq 0 $), the same holds of any ring $ A' $ containing $ A $ as subring, or of any quotient of $ A $ by a two-sided ideal $ a \neq A $. In particular, if $ K $ is a field, every subfield of $ K $ and every extension field of $ K $ have the same characteristic as $ K $.

#### Remark 3 {#alg-v-s1-n2-rem-3 .statement}

Let $ A $ be an algebra not reduced to 0 over a field $ K $. Since the mapping $ \lambda \mapsto \lambda \cdot 1 $ of $ K $ into $ A $ is a ring homomorphism, Remark 1 shows that the characteristic of $ A $ is defined and equal to that of $ K $.

#### Remark 4 {#alg-v-s1-n2-rem-4 .statement}

Since the field $ \mathbf{Q} $ is infinite, every ring of characteristic 0 is infinite; it follows that every finite field has non-zero characteristic.

#### Remark 5 {#alg-v-s1-n2-rem-5 .statement}

Let $ A $ be a ring not reduced to 0, whose additive group is a torsion-free $ \mathbf{Z} $-module, and put $ B = \mathbf{Q} \otimes_{\mathbf{Z}} A $. The mapping $ x \mapsto 1 \otimes x $ of $ A $ into $ B $ is injective (II, p. 314), hence $ A $ is isomorphic to a subring of a ring of characteristic 0.

### 3. Commutative rings of characteristic p

In this No. and the following one $ p $ denotes a prime number.

#### Theorem 2 {#alg-v-s1-thm-2 .statement}

— Let $ A $ be a commutative ring of characteristic $ p $. The mapping $ a \mapsto a^p $ is an endomorphism of the ring $ A $, that is, we have the relations

(1) $$(a + b)^p = a^p + b^p$$
(2) $$(ab)^p = a^p b^p$$

for $ a, b $ in $ A $.

Formula (2) follows from the commutativity of $ A $. To prove (1) we use the binomial formula $(a + b)^p = a^p + b^p + \sum_{i=1}^{p-1} \binom{p}{i} \cdot a^i b^{p-i}$; since $ p \cdot x = 0 $ for all $ x \in A $, it suffices to prove the following lemma:

#### Lemma 1 {#alg-v-s1-lem-1 .statement}

Let $ p $ be a prime number and $ i $ an integer in the range from 1 to $ p - 1 $, then the binomial coefficient $ \binom{p}{i} $ is an integer divisible by $ p $.

We argue by induction on $ i $, the case $ i = 1 $ being immediate from the formula $ \binom{p}{1} = p $. Suppose that $ 2 \leq i \leq p - 1 $ and that $ \binom{i}{i-1} $ is divisible by $ p $. Then the integer $ i \binom{p}{i} = (p - i + 1) \binom{p}{i-1} $ belongs to the prime ideal $ p\mathbf{Z} $ of $ \mathbf{Z} $; since $ i \notin p\mathbf{Z} $, we have $ \binom{p}{i} \in p\mathbf{Z} $ and the lemma follows.

Let $ A $ be a commutative ring of characteristic $ p $ and $ f $ an integer $ \geq 0 $. From Th. 2 we deduce by induction on $ f $ that the mapping $ a \mapsto a^{p^f} $ is an endomorphism of the ring $ A $. In particular we have the relation

$$
(a_1 + \cdots + a_n)^{p^f} = a_1^{p^f} + \cdots + a_n^{p^f}
$$

for any $ a_1, \ldots, a_n $ in $ A $. The mapping $ a \mapsto a^p $ is sometimes called the *Frobenius endomorphism* of $ A $. Taking $ A = \mathbf{F}_p $ and $ a_i = 1 $, we obtain from (3) the relation:

$$
n^{p^f} \equiv n \mod p \quad (n \in \mathbf{Z}, f \in \mathbf{N}) .
$$

For each subset $ S $ of $ A $ we denote by $ S^{p^f} $ the set of elements of $ A $ of the form $ x^{p^f} $ with $ x \in S $^1. In particular, if $ K $ is a subring of $ A $, the set $ K^{p^f} $ is a subring of $ A $. If $ K $ is a subring of $ A $ and $ S $ a subset of $ A $ we denote by $ K[S] $ the subring of $ A $ generated by $ K \cup S $; when $ A $ is a field, we denote by $ K(S) $ the field of fractions of $ K[S] $, that is, the subfield of $ A $ generated by $ K \cup S $.

#### Proposition 2 {#alg-v-s1-prop-2 .statement}

— *Let $ A $ be a commutative ring of characteristic $ p $, $ K $ a subring of $ A $, $ S $ a subset of $ A $ and $ f $ a positive integer.*

a) *We have $ K[S]^{p^f} = K^{p^f}[S^{p^f}] $, and if $ A $ is a field, $ K(S)^{p^f} = K^{p^f}(S^{p^f}) $.*

b) *If the $ K $-module $ K[S] $ is generated by the family $ (a_i)_{i \in I} $ of elements of $ A $, then the $ K $-module $ K[S^{p^f}] $ is generated by the family $ (a_i^{p^f})_{i \in I'} $*

Since $ K[S] $ is the subring of $ A $ generated by $ K \cup S $, its image $ KISlp^f $ under the endomorphism $ \pi : a \mapsto a^{p^f} $ of the ring $ A $ is the subring of $ A $ generated by the image $ K^{p^f} \cup S^{p^f} $ of $ K \cup S $ under $ \pi $, whence $ K[S]^{p^f} = K^{p^f}[S^{p^f}] $. The case of fields is treated similarly; this proves $ a) $.

It is clear that the family $ (a_i^{p^f})_{i \in I} $ generates the $ K^{p^f} $-module $ K[S]^{p^f} $. The $ K $-module $ K[S^{p^f}] $ is generated by products of the form $ x_1^{p^f} \cdots x_n^{p^f} = (x, \ldots x_n)^{p^f} $ with $ x_1, \ldots, x_n $ arbitrary in $ S $, hence also by the set $ K[S]^{p^f} $. Assertion $ b) $ follows directly from this.

^1 Of course the set $ S^{p^f} $ should not be confused with the set product of $ p^f $ sets equal to $ S $, nor with the set of products of $ p^f $ elements belonging to $ S $.

### 4. Perfect rings of characteristic p

#### Definition 2 {#alg-v-s1-def-2 .statement}

— A ring $ A $ of characteristic $ p \neq 0 $ is said to be perfect if it is commutative and the mapping $ a \mapsto a^p $ is bijective.

If the ring $ A $ is perfect of characteristic $ p $, the mapping $ a \mapsto a^{p^f} $ is an automorphism of the ring $ A $ for every integer $ f \geq 0 $; the inverse automorphism is denoted by $ a \mapsto a^{1/p^f} $ or $ a \mapsto a^{p^{-f}} $ and the image of a subset $ S $ of $ A $ under this automorphism is written $ S^{1/p^f} $ or $ S^{p^{-f}} $. It is clear that $ (a^{p^e})^{p^f} = a^{p^{e+f}} $ for all $ a \in A $ and any integers $ e $ and $ f $ (of whatever sign).

Let $ A $ be a commutative ring of characteristic $ p $. For every integer $ f \geq 0 $ let us write $ \mathfrak{n}_f $ for the kernel of the endomorphism $ a \mapsto a^p $ of the ring $ A $. Then $ (\mathfrak{n}_f)_{f \geq 0} $ is an increasing sequence of ideals of $ A $; since every positive integer is majorized by a power of $ p $, the ideal $ \mathfrak{n} = \bigcup_{f \geq 0} \mathfrak{n}_f $ consists of all the nilpotent elements of $ A $. In particular, if $ A $ is perfect, every nilpotent element of $ A $ is zero.

#### Definition 3 {#alg-v-s1-def-3 .statement}

— Let $ A $ be a commutative ring of characteristic $ p \neq 0 $. By a perfect closure of $ A $ we understand a pair $ (A, u) $ where $ A $ is a perfect ring of characteristic $ p $ and $ u $ is a homomorphism of $ A $ into $ A $ satisfying the following universal property:

(PC) *If B is a perfect ring of characteristic p and v is a homomorphism of A into B, then there exists a unique homomorphism h of A into B such that $ v = h \circ u $.*

The universal property (PC) implies at once the uniqueness of the perfect closure, in the following sense : if $ (A, u) $ and $ (A', u') $ are two perfect closures of $ A $, then there exists a unique isomorphism $ h $ of $ A $ onto $ A' $ such that $ u' = h \circ u $ (cf. *E, IV*, p. 23). We shall now establish the *existence* of the perfect closure :

#### Theorem 3 {#alg-v-s1-thm-3 .statement}

— Let $ A $ be a commutative ring of characteristic $ p \neq 0 $. There exists a perfect closure $ (A, u) $ of $ A $. Moreover, the kernel of $ u $ is the set of all nilpotent elements of $ A $ and for each $ x \in A $ there exists an integer $ n \geq 0 $ such that $ x^{p^n} \in u(A) $.

For each integer $ n \geq 0 $, put $ A_n = A $; when $ m \geq n $ we define a homomorphism $ \pi_{m,n} $ of $ A_n $ into $ A_m $ by $ \pi_{m,n}(a) = a^{p^{m-n}} $. We thus obtain a direct system of rings $ (A_n, \pi_{m,n}) $ (I, p. 120); let $ A $ be the direct limit of this system and $ u_n $ the canonical homomorphism of $ A_n = A $ into $ A $; we also put $ u = u_0 $. By construction of the direct limit the kernel $ \mathfrak{n} $ of $ u $ is the union of the kernels of the homomorphisms π_{n,0}: a \mapsto a^{p^n} of $ A $ into $ A $, thus it consists of all the nilpotent elements of $ A $. The ring $ A $ is commutative of characteristic $ p $ by Remark 1 of V, p. 3.

The ring $ A $ is the union of the ascending sequence $ (u, (A))_n $ of subrings. We have $ u_n(A)^{p^n} = A $; hence for each $ x \in \hat{A} $ there exists an integer $ n \geq 0 $ such that $ x^{p^n} \in u(A) $. We also have $ u_n(A) = u_{n+1}(A)^p $, whence $ \hat{A}^p = A $. Let $ x \in A $ be such that $ x^p = 0 $; choose an integer $ n \geq 1 $ and an element $ a \in A $ such that $ x = u_n(a) $. Then we have $ u_{n-1}(a) = u_n(a)^p = 0 $; by definition of the direct limit there exists an integer $ m $ such that $ \pi_m^{1,n-1}(a) = 0 $, that is, $ a^{p^{m-n}} = 0 $. We thus have $ \pi_{m,n}(a) = 0 $, whence $ u_n(a) = 0 $, that is, $ x = 0 $. Therefore the ring $ A $ is perfect of characteristic $ p $.

Let $ v $ be a homomorphism of $ A $ into a perfect ring $ B $ of characteristic $ p $. For every integer $ n \geq 0 $, the mapping $ b \mapsto b^{p^n} $ is an automorphism of $ B $ and so there exists a homomorphism $ v_n $ of $ A, = A $ into $ B $ characterized by $ v(a) = v_n(a)^{p^n} $. We then have $ v_m \circ \pi_{m,n} = v_n $ for $ m \geq n \geq 0 $; by definition of the direct limit there exists a homomorphism $ h $ of $ A $ into $ B $ such that $ v_n = h \circ u $, for all $ n \geq 0 $; in particular we have $ v = v_0 = h \circ u_0 = h \circ u $. Finally let $ h' $ be a homomorphism of $ A $ into $ B $ such that $ h' \circ u = v $. Let $ x \in A $; as we have seen, there exist an integer $ n \geq 0 $ and an element $ a \in A $ such that $ x^{p^n} = u(a) $. Then we have

$$
h(x)^{p^n} = h(u(a)) = v(a) = h'(u(a)) = h'(x)^{p^n},
$$

and since $ B $ is perfect, we find $ h(x) = h'(x) $. Thus we have $ h' = h $, and this completes the proof that $ (A, u) $ is a perfect closure of $ A $.

#### Proposition 3 {#alg-v-s1-prop-3 .statement}

— *Let $ B $ be a perfect ring of characteristic $ p $ and $ A $ a subring of $ B $. Write $ \mathbf{A}^{p^{-\infty}} = \bigcup_{f \geq 0} \mathbf{A}^{p^{-f}} $ and denote by $ j $ the canonical injection of $ A $ in $ \mathbf{A}^{p^{-\infty}} $. Then $ \mathbf{A}^{p^{-\infty}} $ is the smallest perfect subring of $ B $ containing $ A $ and $ (\mathbf{A}^{p^{-\infty}}, j) $ is a perfect closure of $ A $.*

For each integer $ f \in \mathbf{Z} $ denote by $ \pi_f $ the automorphism $ b \mapsto b^{p^f} $ of $ B $. The sequence of subrings $ \pi_{-f}(A) $ of $ B $ (for $ f \geq 0 $) is ascending and its union $ \mathbf{A}^{p^{-\infty}} $ is thus a subring of $ B $. We have $ \pi_1(\mathbf{A}^{p^{-\infty}}) = \bigcup_{f \geq 0} \pi_{-(f-1)}(A) = \mathbf{A}^{p^{-m}} $, hence $ \mathbf{A}^{p^{-\infty}} $ is a perfect subring of $ B $. Finally let $ B_0 $ be a perfect subring of $ B $ containing $ A $; for every integer $ f \geq 0 $ we have $ \pi_{-f}(A) \subset \pi_{-f}(B_0) = B_0 $, whence $ \mathbf{A}^{p^{-\infty}} \subset B_0 $.

If $ v $ is a homomorphism of $ A $ into a perfect ring $ B' $ of characteristic $ p $, then for every integer $ f \geq 0 $ we can define a homomorphism $ h_f $ of $ \pi_{-f}(A) $ into $ B' $ by $ h_f(\pi_{-f}(a)) = v(a)^{p^{-f}} $ for all $ a \in A $. We see at once that $ h_{f+1} $ agrees with $ h_f $ on $ \pi_{-f}(A) $; thus there exists a homomorphism $ h $ of $ \mathbf{A}^{p^{-\infty}} $ into $ B' $ which induces $ h_f $ on $ \pi_{-f}(A) $ for all $ f \geq 0 $ and in particular, $ h $ extends $ h_0 = v $. If $ h' $ is another extension of $ v $ to a homomorphism of $ A^{p^{-\infty}} $ into B, the equality $ h' = h $ may be established as in the proof of Th. 3.

### 5. Characteristic exponent of a field. Perfect fields

Let $ K $ be a field. By the *characteristic exponent* of $ K $ we understand the integer equal to *1* if $ K $ is of characteristic 0, and equal to the characteristic of $ K $ when this is non-zero.

#### Proposition 4 {#alg-v-s1-prop-4 .statement}

— *Let $ K $ be a field of characteristic exponent q. For every integer $ f \geq 0 $ the mapping $ x \mapsto x^{q^f} $ is an isomorphism of K on one of its subfields (denoted by $ K^{q^f} $).*
This follows from Th. 2 when q ≠ 1 and is trivial when q = 1.
Likewise one can extend Prop. 2 to the case where $ A $ is a field of characteristic exponent q, the case q = *1* being trivial.

#### Definition 4 {#alg-v-s1-def-4 .statement}

— *A field K of characteristic exponent q is said to be perfect if we have $ K^q = K $. When $ K^q \neq K $, K is called imperfect.*
By this definition a field is perfect if it is of characteristic 0, or if it is a perfect ring of characteristic $ p \neq 0 $ in the sense of Def. 2. If $ K $ is a field of characteristic $ p \neq 0 $ and $ (K, u) $ is a perfect closure of $ K $, then K is a field by Prop. 3 *(V, p. 6)* and $ u $ is an isomorphism of K onto a subfield of $ \hat{K} $. Frequently one identifies $ K $ with its image under $ u $ in $ \hat{K} $, so that we have $ \hat{K} = K^{p^{-\infty}} $ (Prop. **3**).
Let K be a field of characteristic *0* ; the characteristic exponent of $ K $ is then *1*. By convention the notation $ x^{q^{-f}} $ and $ S^{q^{-f}} $ is taken to mean x and S respectively *(for an element $ x $ of $ K $ and a subset S of $ K$)*. In particular we put $ K^{q^{-\infty}} = K $ and we agree to take the perfect closure of $ K $ to be $ K $.

#### Proposition 5 {#alg-v-s1-prop-5 .statement}

— *If K is a field of characteristic 0, or is finite, \* or algebraically closed \*, it is perfect. In particular every prime field is perfect.*
Suppose that $ K $ has characteristic $ p \neq 0 $. If $ K $ is finite, then the subfield $ K^p $ of $ K $ has the same cardinal as $ K $, whence $ K^p = K $. \* If $ K $ is algebraically closed, the polynomial $ X^p - a $ has a root $ x $ in $ K $ for each $ a \in K $ *(V, p. 20, Def. 1)* whence $ x^p = a $ and so $ K^p = K $. \* Finally a prime field is of characteristic *0* or finite.
Let $ K_0 $ be a field of characteristic $ p \neq 0 $ and $ K = K_0(X) $ the field of rational fractions in an indeterminate $ X $ over $ K_0 $. Then $ K $ is *imperfect*, for there exists no element $ u(X)/v(X) $ of $ K $ *(u, v polynomials in $ K_0[X] $)* such that $ (u(X)/v(X))^p = X $. This may be seen by writing this relation in the form $ u(X)^p = Xv(X)^p $ and comparing the degrees of the two sides.

### 6. Characterization of polynomials with zero differential

#### Proposition 6 {#alg-v-s1-prop-6 .statement}

— *Let K be a commutative ring, A the polynomial algebra $ K[X_i]_{i \in I} $, and S the set of elements F of A such that $ dF = 0 $.*

a) *If K is a ring of characteristic 0, then S = K.*
b) *If K is a ring of characteristic $ p \neq 0 $, then $ S = K[X_i^p]_{i \in I} $; if moreover K is perfect, then $ K = A^P $.*

The mapping $ F \mapsto dF $ of A into the module $ \Omega_K(A) $ of K-differentials of A is K-linear and satisfies the relation

$$
d(FF') = F \cdot dF' + F' \cdot dF
$$

(III, p. 569). Therefore S is a subalgebra.

When K is of characteristic $ p \neq 0 $, put $ T = K[X_i^p]_{i \in I} $; we thus have $ T = A^P $ if K is perfect ($ V $, p. 4, Prop. 2); moreover, we have $ d(X_i^p) = pX_i^{p-1} \cdot dX_i = 0 $ for all $ i \in I $, hence the subalgebra S of A contains T. If K is of characteristic 0, we put $ T = K $, and still find that $ T \subset S $. It remains to show that S is contained in T.

For every finite subset J of I let $ A_J $ be the subalgebra of A generated by the family $ (X_j)_{j \in J} $. We have $ A_\emptyset = K $ and $ A = \bigcup_{J \in I} A_J $; so it suffices to prove the relation $ S \cap A_J \subset T $, which we shall accomplish by induction on the cardinal of J. Thus let J be a finite subset of I such that $ S \cap A_J \subset T $, let i be an element of $ I - J $ and $ J' = J \cup \{ i \} $. Every element F of A may be written in just one way in the form

$$
F = \sum_{n=0}^\infty F_n \cdot X_i^n,
$$

with $ F_n \in A_J $ for all $ n \geq 0 $, and then

$$
dF = \sum_{n=0}^\infty X_i^n \cdot dF_n + \sum_{n=0}^\infty nX_i^{n-1}F_n \cdot dX_i.
$$

Suppose that F belongs to S; the family $ (dX_r)_{r \in J} $ is a basis of the A-module $ \Omega_K(A) $ (III, p. 570) and $ dF_n $ is a linear combination of the differentials $ dX_j $ for $ j \in J $ because $ F_n \in A_J = K[X_j]_{j \in J} $. By (6) we then have $ dF_n = 0 $ and $ nF_n = 0 $ for each integer $ n \geq 0 $. By the induction hypothesis $ F_n \in T $ for all $ n $, since $ dF_n = 0 $.

a) If K is of characteristic 0, we have $ nF_n = 0 $ for all $ n \geq 1 $, whence $ F_n = 0 $ by Prop. 1 ($ V $, p. 2); so we have $ F = F_0 $, whence $ F \in T $.

b) If K is of characteristic $ p \neq 0 $, then A is an algebra over the field $ \mathbf{F}_p $ and the relation $ nF_n = 0 $ implies $ F_n = 0 $ for every integer $ n $ not divisible by $ p $. So we have $ F = \sum_{m=0}^m F_{mp} X_i^{mp} $, whence $ F \in T $

#### Remark {#alg-v-s1-n6-rem-1 .statement}

— We still have $ S = K $ when the additive group of K is torsion-free; this follows from the above proof or from Remark 5 of V, p. 3.

#### Corollary {#alg-v-s1-n6-cor-1 .statement}

— Let K be a field and F(X) a polynomial with coefficients in K, whose derivative F'(X) is zero.
a) If K is of characteristic 0, then F ∈ K.
b) If K is of characteristic p ≠ 0, there exists a polynomial G(X) such that F(X) = G(X^p).
For we have dF = F . dX = 0.

### Exercises {#alg-v-s1-exercises}

See the [exercises for § 1](exercises/s1/).
