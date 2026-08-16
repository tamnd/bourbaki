---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: VII
chapter_title: CARTAN SUBALGEBRAS AND REGULAR ELEMENTS
section: 1
section_title: Primary decomposition of linear representations
lang: en
source: lie-vii-ix
book_pages: 1-12, 51-55
pdf_pages: 0011-0022, 0060-0064
extraction: native
subsections:
    - "no": 1
      title: DECOMPOSITION OF A FAMILY OF ENDOMORPHISMS
      page: 1
      pdf_page: 11
    - "no": 2
      title: THE CASE OF A LINEAR FAMILY OF ENDOMORPHISMS
      page: 6
      pdf_page: 16
    - "no": 3
      title: DECOMPOSITION OF REPRESENTATIONS OF A NILPOTENT LIE ALGEBRA
      page: 8
      pdf_page: 18
    - "no": 4
      title: DECOMPOSITION OF A LIE ALGEBRA RELATIVE TO AN AUTOMORPHISM
      page: 11
      pdf_page: 21
    - "no": 5
      title: INVARIANTS OF A SEMI-SIMPLE LIE ALGEBRA RELATIVE TO A SEMI-SIMPLE ACTION
      page: 11
      pdf_page: 21
statements: 25
exercises: 11
content_sha256: 575b6f0a3f9a3d5aa4cd76cd44622cddd588e8d2cf1d3e2ec7c24cb9b797b8be
---

## § 1. PRIMARY DECOMPOSITION OF LINEAR REPRESENTATIONS

### 1. DECOMPOSITION OF A FAMILY OF ENDOMORPHISMS

Let V be a vector space, S a set, and $r$ a map from S to End(V). Denote by P the set of maps from S to $k$. If $\lambda \in P$, denote by $V_{\lambda}(S)$ (resp. $V^{\lambda}(S))$ the set of $v\in V$ such that, for all $s\in S,r(s)v=\lambda (s)v$ (resp. $(r(s)-\lambda (s))^nv= 0$ for $n$ sufficiently large). The sets $V_{\lambda}(S)$ and $V^{\lambda}(S)$ are vector subspaces of V, and $V_{\lambda}(S)\subset V^{\lambda}(S)$. We say that $V_{\lambda}(S)$ is the eigenspace of V relative to $\lambda$ (and to $r)$, that $V^{\lambda}(S)$ is the primary subspace of V relative to $\lambda$ (and to $r)$, and that $V^0(S)$ is the nilspace of V (relative to $r)$. We say that $\lambda$ is a weight of S in V if $V^{\lambda}(S)\not= 0$.

In particular, if S reduces to a single element $s, P$ can be identified with $k$; we use the notations $V_{\lambda(s)}(s)$ and $V^{\lambda(s)}(s)$, or $V_{\lambda(s)}(r(s))$ and $V^{\lambda(s)}(r(s))$, instead of $V_{\lambda}(\{s\}), V^{\lambda}(\{s\})$; we speak of eigenspaces, primary subspaces and the nilspace of $r(s)$; an element $v$ of $V_{\lambda(s)}(s)$ is called an eigenvector of $r(s)$, and, if $v\not= 0,\lambda (s)$ is called the corresponding eigenvalue (cf. Algebra, Chap. VII, §5).

For all $\lambda \in P$, the following relations are immediate:

$$
V^{\lambda}(S) =\bigcap_{s\in S}V^{\lambda(s)}(s) \tag{1}
$$

$$
V_{\lambda}(S) =\bigcap_{s\in S}V_{\lambda(s)}(s) \tag{2}
$$

Let $k'$ be an extension of $k$. The canonical map from End(V) to End($V\otimes_kk'$) gives, by composition with $r$, a map $r': S\rightarrow$ End($V\otimes_kk'$). Similarly, every map $\lambda$ from S to $k$ defines canonically a map, also denoted by $\lambda$, from S to $k'$. With these notations, we have the following proposition:

#### Proposition 1 {#lie-vii-s1-prop-1 .statement tag=00SJ}

For all $\lambda \in P$,

$(V\otimes_kk')^{\lambda}(S) = V^{\lambda}(S)\otimes_kk'$ and $(V\otimes_kk')_{\lambda}(S) = V_{\lambda}(S)\otimes_kk'$.

Let $(a_i)$ be a basis of the $k$-vector space $k'$. If $v\in V\otimes_kk',v$ can be expressed uniquely in the form $\sum v_i\otimes a_i$ where $(v_i)$ is a finitely-supported family of elements of V. For all $s\in S$,

$$
(r'(s)-\lambda (s))^n(v) =\sum(r(s)-\lambda (s))^nv_i\otimes a_i
$$

It follows that

$v\in (V\otimes_kk')^{\lambda}(S)\Leftarrow \Rightarrow v_i\in V^{\lambda}(S)$ for all $i$,

$v\in (V\otimes_kk')_{\lambda}(S)\Leftarrow \Rightarrow v_i\in V_{\lambda}(S)$ for all $i$,

which implies the proposition.

#### Proposition 2 {#lie-vii-s1-prop-2 .statement tag=00SK}

Let $V,V',W$ be vector spaces. Let $r$ : S $\rightarrow$ End(V), $r': S\rightarrow$ End(V$')$ and $q: S\rightarrow$ End(W) be maps.

(i) Let $f: V\rightarrow W$ be a linear map such that $q(s)f(v) =f(r(s)v)$ for $s\in S$ and $v\in V$. Then, for all $\lambda \in P,f$ maps $V^{\lambda}(S)$ (resp. $V_{\lambda}(S))$ into $W^{\lambda}(S)$ (resp. $W_{\lambda}(S))$.

(ii) Let $B : V\times V'\rightarrow W$ be a bilinear map such that

$$
q(s)B(v, v') = B(r(s)v, v') + B(v, r'(s)v')
$$

for $s\in S,v\in V,v'\in V'$. Then, for all $\lambda , \mu\in P$, B maps $V^{\lambda}(S)\times {V'}^\mu(S)$ (resp. $V_{\lambda}(S)\times V'_\mu(S))$ into $W^{\lambda+\mu}(S)$ (resp. $W_{\lambda+\mu}(S))$.

(iii) Let $B : V\times V'\rightarrow W$ be a bilinear map such that

$$
q(s)B(v, v') = B(r(s)v, r'(s)v')
$$

for $s\in S,v\in V,v'\in V'$. Then, for all $\lambda , \mu\in P$, B maps $V^{\lambda}(S)\times {V'}^\mu(S)$ (resp. $V_{\lambda}(S)\times V'_\mu(S))$ into $W^{\lambda \mu}(S)$ (resp. $W_{\lambda \mu}(S))$.

In case (i), $(q(s)-\lambda (s))^nf(v) =f((r(s)-\lambda (s))^nv)$ for $s\in S$ and $v\in V$, hence the conclusion. In case (ii),

$$
(q(s)-\lambda (s)-\mu(s))B(v, v') = B((r(s)-\lambda (s))v, v') + B(v,(r'(s)-\mu(s))v')
$$

for $s\in S,v\in V,v'\in V'$, hence by induction on $n$

$$
'(n)''
$$

$(q(s)-\lambda (s)-\mu(s))^nB(v, v) =\sum B((r(s)-\lambda (s))^iv,(r(s)-\mu(s))^jv)$.

$$
i
$$

$i+j=n$

The assertions in (ii) follow immediately. In case (iii), $(q(s)-\lambda (s)\mu(s))B(v, v') = B((r(s)-\lambda (s))v, r'(s)v')+B(\lambda (s)v,(r'(s)-\mu(s))v')$ for $s\in S,v\in V,v'\in V'$, hence by induction on $n$

$$
(q(s)-\lambda (s)\mu(s))^nB(v, v')
$$

= $\sum(n)B(\lambda (s)^j(r(s)-\lambda (s))^iv, r'(s)^i(r'(s)-\mu(s))^jv')$.

$$
i
$$

$i+j=n$

The assertions in (iii) follow immediately.

#### Proposition 3 {#lie-vii-s1-prop-3 .statement tag=00SL}

The sum $\sum_{\lambda\in P}V^{\lambda}(S)$ is direct. The sum $\sum_{\lambda\in P}V_{\lambda}(S)$ is direct.

The second assertion is a consequence of the first; hence it suffices to prove that. We distinguish several cases.

$a) S$ is empty. The assertion is trivial.

$b) S$ is reduced to a single element $s$. Let $\lambda_0, \lambda_1, . . . , \lambda_n$ be distinct elements of $k$. For $i= 0,1, . . . , n$, let $v_i\in V^{\lambda_i}(s)$ and assume that $v_0=v_1+\cdots +v_n$. It suffices to prove that $v_0$ = 0. For $i= 0, . . . , n$, there exists an integer $q_i>$ 0 such that $(r(s)-\lambda_i)^{q_i}v_i$ = 0. Consider the polynomials $P(X) =\prod_{i\geq 1}(X-\lambda_i)^{q_i}$ and $Q(X) = (X-\lambda_0)^{q_0}$. We have $Q(r(s))v_0= 0$, and

$P(r(s))v_0=\sum_{i=1}^nP(r(s))v_i= 0$. Since P and Q are relatively prime, the Bezout identity proves that $v_0= 0$.

$c) S$ is finite and non-empty. We argue by induction on the cardinal of S. Let $s\in S$ and $S'= S$**--** $\{s\}$. Let $(v_{\lambda})_{\lambda\in P}$ be a finitely-supported family of elements of V such that $\sum_{\lambda\in P}v_{\lambda}= 0$ and $v_{\lambda}\in V^{\lambda}(S)$. Let $\lambda_0\in P$. Let $P'$ be the set of $\lambda \in P$ such that $\lambda |S'=\lambda_0|S'$. By the induction hypothesis applied to $S'$, we have $\sum_{\lambda\in P'}v_{\lambda}= 0$. If $\lambda , \mu$ are distinct elements of $P',\lambda (s)\not=\mu(s)$.

Since the sum $\sum_{\alpha\in k}V^{\alpha}(s)$ is direct by $b)$, and since $v_{\lambda}\in V^{\lambda(s)}(s),v_{\lambda}= 0$ for all $\lambda \in P'$, and in particular $v_{\lambda_0}= 0$, which we had to prove.

$d)$ General case. Let $(v_{\lambda})_{\lambda\in P}$ be a finitely-supported family of elements of V such that $\sum_{\lambda\in P}v_{\lambda}= 0$ and $v_{\lambda}\in V^{\lambda}(S)$. Let $P'$ be the finite set of $\lambda \in P$ such that $v_{\lambda}\not= 0$, and let $S'$ be a finite subset of S such that the conditions $\lambda \in P'$, $\mu\in P',\lambda |S'=\mu|S'$ imply that $\lambda =\mu$. We have $v_{\lambda}\in V^{\lambda|S'}(S')$; applying $c)$, we see that $v_{\lambda}= 0$ for $\lambda \in P'$, which completes the proof.

Recall that, if $x\in$ End(V), we denote by ad $x$ the map $y \rightarrow xy-yx= [x, y]$ from End(V) to itself.

#### Lemma 1 {#lie-vii-s1-lem-1 .statement tag=00SM}

Let $x, y\in$ End(V).

(i) Assume that V is finite dimensional. Then $x$ is triangularizable if and only if $V =\sum_{a\in k}V^a(x)$.

(ii) If there exists an integer $n$ such that (ad $x)^ny= 0$, each $V^a(x)$ is stable under $y$.

(iii) Assume that V is finite dimensional. If $V =\sum_{a\in k}V^a(x)$ and if each

$V^a(x)$ is stable under $y$, there exists an integer $n$ such that (ad $x)^ny= 0$.

Part (i) follows from Algebra, Chap. VII, §5, no. 2, Prop. 3.

Let E = End(V). Let B be the bilinear map $(u, v) \rightarrow u(v)$ from $E\times V$ to V. By the definition of ad $x$,

$x(B(u, v)) =B(u, x(v)) +$ B((ad $x)(u), v)$

for $x\in E,u\in E,v\in V$. Let $x$ operate on E via ad $x$. By Prop. 2 (ii), $B(E^0(x),V^a(x))\subset V^a(x)$ for all $a\in k$. If (ad $x)^ny= 0$, then $y\in E^0(x)$, so $y(V^a(x))\subset V^a(x)$, which proves (ii).

To prove (iii), we can replace V by $V^a(x)$ and $x$ (resp. $y)$ by its restriction to $V^a(x)$. Replacing $x$ by $x-a$, we can assume that $x$ is nilpotent. Then, (ad $x)^{2 dim V-1}= 0$ (Chap. I, §4, no. 2), which proves (iii).

#### Remark {#lie-vii-s1-n1-rem-1 .statement tag=00SN}

The argument proves that, if V is finite dimensional and if there exists an integer $n$ such that (ad $x)^ny= 0$, then (ad $x)^{2 dim V-1}y= 0$.

In the sequel, we shall say that the map $r: S\rightarrow$ End(V) satisfies condition (AC) (“almost commutative”) if:

(AC) For every pair $(s, s')$ of elements of S, there exists an integer $n$ such that

(ad $r(s))^nr(s') = 0$.

#### Theorem 1 {#lie-vii-s1-thm-1 .statement tag=00SO}

Assume that V is finite dimensional. The following conditions are equivalent:

(i) Condition (AC) is satisfied and, for all $s\in S,r(s)$ is triangularizable.

(ii) For all $\lambda \in P$, $V^{\lambda}(S)$ is stable under $r(S)$, and $V =\sum_{\lambda\in P}V^{\lambda}(S)$.

If $V =\sum_{\lambda\in P}V^{\lambda}$(S), then $V =\sum_{a\in k}V^a(s)$ for all $s\in S$, and it follows from

Lemma 1 that (ii) implies (i). Assume that condition (i) is satisfied. Lemma 1 and formula (1) imply that each $V^{\lambda}(S)$ is stable under $r(S)$. It remains to prove that $V =\sum_{\lambda\in P}V^{\lambda}(S)$. We argue by induction on dim V. We distinguish two cases.

$a)$ For all $s\in S,r(s)$ has a single eigenvalue $\lambda (s)$. Then $V = V^{\lambda}(S)$.

$b)$ There exists $s\in S$ such that $r(s)$ has at least two distinct eigenvalues. Then V is the direct sum of the $V^a(s)$ for $a\in k$, and dim $V^a(s)<$ dim V for all $a$. Each $V^a(s)$ is stable under $r$(S), and it suffices to apply the induction hypothesis.

#### Corollary 1 {#lie-vii-s1-thm-1-cor-1 .statement tag=00SP}

Assume that V is finite dimensional and that condition (AC) is satisfied. Let $k'$ be an extension of $k$. Assume that, for all $s\in S$, the endomorphism $r(s)\otimes 1$ of $V\otimes_kk'$ is triangularizable. Let $P'$ be the set of maps from S to $k'$. Then $V\otimes_kk'=\sum_{\lambda'\in P'}(V\otimes_kk')^{\lambda'}(S)$.

Let $r': S\rightarrow$ End(V$\otimes_kk')$ be the map defined by $r$. If $s_1, s_2\in S$, there exists an integer $n$ such that (ad $r(s_1))^nr(s_2) = 0$, hence (ad $r'(s_1))^nr'(s_2) = 0$. It now suffices to apply Th. 1.

#### Corollary 2 {#lie-vii-s1-thm-1-cor-2 .statement tag=00SQ}

Assume that V is finite dimensional and that condition (AC) is satisfied. Denote by $V^+(S)$ the vector subspace $\sum_{s\in S}((\bigcap_{i\geq 1}r(s)^iV)$. Then:

(i) $V^0(S)$ and $V^+(S)$ are stable under $r(S)$;

(ii) $V = V^0(S)\oplus V^+(S)$;

(iii) every vector subspace W of V, stable under $r(S)$ and such that $W^0(S) = 0$, is contained in $V^+(S)$;

(iv) $\sum_{s\in S}r(s)V^+(S) = V^+(S)$.

Moreover, $V^+(S)$ is the only vector subspace of V with properties (i) and (ii). For any extension $k'$ of $k,(V\otimes_kk')^+(S) = V^+(S)\otimes_kk'$.

The last assertion is immediate. Thus, taking Prop. 1 into account, in proving the others we can assume that $k$ is algebraically closed. By Th. 1, V = $\sum_{\lambda\in P}V^{\lambda}$(S), and the $V^{\lambda}(S)$ are stable under $r(S)$. If $s\in S$, the characteristic

polynomial of $r(s)|V^{\lambda}(S)$ is $(X-\lambda (s))^{dim V^{\lambda}(S)}$; it follows that $\bigcap_{i\geq 1}r(s)^iV^{\lambda}(s)$

is zero if $\lambda (s) = 0$ and is equal to $V^{\lambda}(S)$ if $\lambda (s)\not= 0$; hence,

$$
V^+(S) =\sum_{\lambda\in P,\lambda\not=0}V^{\lambda}(S) \tag{3}
$$

which proves (i), (ii) and (iv). If W is a vector subspace of V stable under $r$(S), then $W =\sum_{\lambda\in P}W^{\lambda}(S)$ and $W^{\lambda}(S) = W\cap V^{\lambda}(S)$. If $W^0(S) = 0$, we see that $W\subset V^+$(S), which proves (iii).

Let $V'$ be a vector subspace of V stable under $r(S)$ and such that $V'\cap V^0(S) = 0$. Then ${V'}^0(S) = 0$, so $V'\subset V^+(S)$ by (iii). If, in addition, $V = V^0(S) + V'$, we see that $V'= V^+(S)$. Q.E.D.

We sometimes call $(V^0(S),V^+(S))$ the Fitting decomposition of V, or of the map $r: S\rightarrow$ End(V). If S reduces to a single element $s$, we write $V^+(s)$ or $V^+(r(s))$ instead of $V^+(\{s\})$. We have that $V = V^0(s)\oplus V^+(s), V^0(s)$ and $V^+(s)$ are stable under $r(s),r(s)|V^0(s)$ is nilpotent and $r(s)|V^+(s)$ is bijective.

#### Corollary 3 {#lie-vii-s1-thm-1-cor-3 .statement tag=00SR}

Let V and $V'$ be finite dimensional vector spaces, and let $r: S\rightarrow$ End(V) and $r': S\rightarrow$ End(V$')$ be maps satisfying condition (AC). Let $f: V\rightarrow V'$ be a surjective linear map such that $f(r(s)v) =r'(s)f(v)$ for $s\in S$ and $v\in V$. Then $f(V^{\lambda}{(S)) = V'}^{\lambda}(S)$ for all $\lambda \in P$.

In view of Prop. 1, we are reduced to the case in which $k$ is algebraically closed. We have $V =\bigoplus_{\lambda\in P}V^{\lambda}$(S), $V'=\bigoplus_{\lambda\in P}{V'}^{\lambda}(S)$ by Th. 1, and $V'=f(V) =$ $\sum_{\lambda\in P}f(V^{\lambda}(S))$. Finally, $f(V^{\lambda}(S))\subset {V'}^{\lambda}(S)$ by Prop. 2 (i), hence the corollary.

#### Proposition 4 {#lie-vii-s1-prop-4 .statement tag=00SS}

Assume that $k$ is perfect. Let V be a finite dimensional vector space, $u$ an element of End(V)$,u_s, u_n$ the semi-simple and nilpotent components of $u($Algebra, Chap. VII, §5, no. 8).

(i) For all $\lambda \in k,V^{\lambda}(u) = V^{\lambda}(u_s) = V_{\lambda}(u_s)$.

(ii) If V has an algebra structure and if $u$ is a derivation of V$,u_s$ and $u_n$ are derivations of V.

(iii) If V has an algebra structure and if $u$ is an automorphism of V, then $u_s$ and $1 +u^{-1}_su_n$ are automorphisms of V.

In view of Prop. 1, we can assume that $k$ is algebraically closed, so

$$
V =\sum_{\lambda\in k}V^{\lambda}(u)
$$

The semi-simple component of $u|V^{\lambda}(u)$ is the homothety with ratio $\lambda$ in $V^{\lambda}(u)$. This proves (i).

Assume from now on that V has an algebra structure. Let $x\in V^{\lambda}(u)$, $y\in V^\mu(u)$.

If $u$ is a derivation of V, then $xy\in V^{\lambda+\mu}(u)$ (Prop. 2 (ii)), so

$$
u_s(xy) = (\lambda +\mu)(xy) = (\lambda x)y+x(\mu y) = (u_sx)y+x(u_sy)
$$

This proves that $u_s$ is a derivation of V. Then $u_n=u-u_s$ is a derivation of V.

If $u$ is an automorphism of V, Ker($u_s$) $= V^0(u) = 0$, so $u_s$ is bijective. On the other hand, $xy\in V^{\lambda \mu}(u)$ (Prop. 2 (iii)), so

$$
u_s(xy) = (\lambda \mu)(xy) = (\lambda x)(\mu y) =u_s(x).u_s(y)
$$

This proves that $u_s$ is an automorphism of V; but then so is

$$
1 +u^{-1}_su_n=u^{-1}_su
$$

### 2. THE CASE OF A LINEAR FAMILY OF ENDOMORPHISMS

Assume now that S has a vector space structure, that the map $r: S\rightarrow$ End(V) is linear, and that V and S are finite dimensional.

#### Proposition 5 {#lie-vii-s1-prop-5 .statement tag=00ST}

Assume that condition (AC) is satisfied, and let $\lambda : S\rightarrow k$ be such that $V^{\lambda}(S)\not= 0$. If $k$ is of characteristic 0, the map $\lambda$ is linear. If $k$ is of characteristic $p\not= 0$, there exists a power $q$ of $p$ dividing dim $V^{\lambda}(S)$, and a homogeneous polynomial function $P : S\rightarrow k$ of degree $q$, such that $\lambda (s)^q= P(s)$ for all $s\in S$.

Since $V^{\lambda}(S)$ is stable under $r(S)$ (Lemma 1 and formula (1) of no. 1), we can assume that $V = V^{\lambda}(S)$. Let $n=$ dim V. Thus, for $s\in S$,

det(X $-r(s)) = (X-\lambda (s))^n$.

On the other hand, the expansion of the determinant shows that

det(X $-r(s)) = X^n+a_1(s)X^{n-1}+\cdots +a_i(s)X^{n-i}+\cdots$

where $a_i: S\rightarrow k$ is a homogeneous polynomial function of degree $i$. Write $n=qm$ where $q$ is a power of the characteristic exponent of $k$ and $(q, m) = 1$. Then $(X-\lambda (s))^n= (X^q-\lambda (s)^q)^m$; hence $-m\lambda (s)^q=a_q(s)$, which implies the result.

#### Proposition 6 {#lie-vii-s1-prop-6 .statement tag=00SU}

Assume that $k$ is infinite and that condition (AC) is satisfied. Let $k'$ be an extension of $k$. Put $V'= V\otimes_kk',S'= S\otimes_kk'$. Let $r': S'\rightarrow$ End(V$')$ be the map obtained from $r$ by extension of scalars. Then

$$
V^0(S)\otimes_kk'{= V'}^0{(S) = V'}^0(S')
$$

The first equality follows from Prop. 1. To prove the second, we can assume that $V = V^0(S)$ and so $V'{= V'}^0(S)$. Let $(s_1, . . . , s_m)$ be a basis of S and $(e_1, . . . , e_n)$ a basis of V. There exist polynomials $P_{ij}(X_1, . . . ,X_m)$ such that

$$
r'(a_1s_1+\cdots +a_ms_m)^ne_j=\sum_{i=1}^nP_{ij}(a_1, . . . , a_m)e_i
$$

for $1\leq j\leq n$ and $a_1, . . . , a_m\in k'$. By hypothesis, $r'(s)^n= 0$ for all $s\in S$, in other words $P_{ij}(a_1, . . . , a_m) = 0$ for $1\leq i, j\leq n$ and $a_1, . . . , a_m\in k$. Since $k$ is infinite, $P_{ij}= 0$. Consequently, every element of $r'(S')$ is nilpotent and $V'{= V'}^0(S')$.

#### Proposition 7 {#lie-vii-s1-prop-7 .statement tag=00SV}

Assume that $k$ is infinite and that condition (AC) is satisfied. Let $\widetilde{S}$ be the set of $s\in S$ such that $V^0(s) = V^0(S)$. If $s\in S$, let $P(s)$ be the determinant of the endomorphism of $V/V^0(S)$ defined by $r(s)$ (no. 1, Cor. 2 (i) of Th. 1).

(i) The function $s \rightarrow P(s)$ is polynomial on S. We have $\widetilde{S} =\{s\in S|P(s)\not= 0\}$; this is an open subset of S in the Zariski topology (App. 1).

(ii) $\widetilde{S}$ is non-empty, and $V^+(s) = V^+(S)$ for all $s\in \widetilde{S}$.

The fact that $s \rightarrow P(s)$ is polynomial follows from the linearity of $r$. If $s\in S, V^0(s)\supset V^0$(S), with equality if and only if $r(s)$ defines an automorphism of $V/V^0$(S), hence (i).

Now let $k'$ be an algebraic closure of $k$, and introduce $V',S', r'$ as in Prop. 6. We remark that $S'$ satisfies condition (AC) by continuation of the polynomial identity (ad $r(s_1))^{2 dim V-1}r(s_2) = 0$ valid for $s_1, s_2\in S$ (no. 1, Remark ). Applying Th.1, we deduce a decomposition

$$
V'{= V'}^0(S')\oplus \sum_{i=1}^m{V'}^{\lambda_i}(S')
$$

with $\lambda_i\not= 0$ for $1\leq i\leq m$. For $1\leq i\leq m$, there exists a polynomial function $P_i$ non-zero on $S'$ and an integer $q_i$ such that $\lambda^q_{i^i}= P_i$ (Prop. 5). Since $k$ is infinite, there exists $s\in S$ such that $(P_1. . .P_m)(s)\not= 0$, cf. Algebra, Chap. IV, §2, no. 3, Cor. 2 of Prop. 9. Then $\lambda_i(s)\not= 0$ for all $i$, so ${V'}^0(S'{) = V'}^0(s)$ and consequently $V^0(S) = V^0(s)$ (Prop. 6), which shows that $\widetilde{S}\not=\emptyset$. If $s\in \widetilde{S}$, the fact that $V^+(S)$ is stable under $r(s)$ and is a complement of $V^0(s)$ in V implies that $V^+(S) = V^+(s)$ (Cor. 2 of Th. 1).

### 3. DECOMPOSITION OF REPRESENTATIONS OF A NILPOTENT LIE ALGEBRA

Let $\mathfrak{h}$ be a Lie algebra and M an $\mathfrak{h}$-module. For any map $\lambda$ from $\mathfrak{h}$ to $k$, we have defined in no. 1 vector subspaces $M^{\lambda}(\mathfrak{h})$ and $M_{\lambda}(\mathfrak{h})$ of M. In particular, if $\mathfrak{g}$ is a Lie algebra containing $\mathfrak{h}$ as a subalgebra, and if $x\in \mathfrak{g}$, we shall often employ the notations $\mathfrak{g}^{\lambda}(\mathfrak{h})$ and $\mathfrak{g}_{\lambda}(\mathfrak{h})$; it will then be understood that $\mathfrak{h}$ operates on $\mathfrak{g}$ by the adjoint representation ad$_{\mathfrak{g}}$.

#### Proposition 8 {#lie-vii-s1-prop-8 .statement tag=00SW}

Let $\mathfrak{h}$ be a Lie algebra, and $L,M,N\mathfrak{h}$-modules. Denote by P the set of maps from $\mathfrak{h}$ to $k$.

(i) The sum $\sum_{\lambda\in P}L^{\lambda}(P)$ is direct.

(ii) If $f: L\rightarrow M$ is a homomorphism of $\mathfrak{h}$-modules, $f(L^{\lambda}(\mathfrak{h}))\subset M^{\lambda}(\mathfrak{h})$ for all $\lambda \in P$.

(iii) If $f: L\times M\rightarrow N$ is a bilinear $\mathfrak{h}$-invariant map,

$$
f(L^{\lambda}(\mathfrak{h})\times M^\mu(\mathfrak{h}))\subset N^{\lambda+\mu}(\mathfrak{h})
$$

for all $\lambda , \mu\in P$.

This follows from Props. 2 and 3.

#### Proposition 9 {#lie-vii-s1-prop-9 .statement tag=00SX}

Let $\mathfrak{h}$ be a nilpotent Lie algebra and M a finite dimensional $\mathfrak{h}$-module. Denote by P the set of maps from $\mathfrak{h}$ to $k$.

(i) Each $M^{\lambda}(\mathfrak{h})$ is an $\mathfrak{h}$-submodule of M. If $x_M$ is triangularizable for all $x\in \mathfrak{h}$, then $M =\sum_{\lambda\in P}M^{\lambda}(\mathfrak{h})$.

(ii) If $k$ is infinite, there exists $x\in \mathfrak{h}$ such that $M^0(x) = M^0(\mathfrak{h})$.

(iii) If $k$ is of characteristic 0, and if $\lambda \in P$ is such that $M^{\lambda}(\mathfrak{h})\not= 0$, then $\lambda$ is a linear form on $\mathfrak{h}$ vanishing on $[\mathfrak{h},\mathfrak{h}]$, and $M_{\lambda}(\mathfrak{h})\not= 0$.

(iv) If $f: M\rightarrow N$ is a surjective homomorphism of finite dimensional $\mathfrak{h}$-modules, then $f(M^{\lambda}(\mathfrak{h})) = N^{\lambda}(\mathfrak{h})$ for all $\lambda \in P$.

(v) If N is a finite dimensional $\mathfrak{h}$-module, and B a bilinear form on $M\times N$ invariant under $\mathfrak{h}$, then $M^{\lambda}(\mathfrak{h})$ and $N^\mu(\mathfrak{h})$ are orthogonal relative to B if $\lambda +\mu\not= 0$. Moreover, if B is non-degenerate then so is its restriction to $M^{\lambda}(\mathfrak{h})\times N^{-\lambda}(\mathfrak{h})$ for all $\lambda \in P$.

Part (i) follows from no. 1, Lemma 1 and Th. 1. Part (ii) follows from no. 2, Prop. 7. Part (iv) follows from no. 1, Cor. 3 of Th. 1. We prove (iii). We can assume that $M = M^{\lambda}(\mathfrak{h})$. Then, for all $x\in \mathfrak{h},\lambda (x) =$ (dim $M)^{-1}$Tr($x_M$); this proves that $\lambda$ is linear (which also follows from Prop. 5) and that $\lambda$ vanishes on $[\mathfrak{h},\mathfrak{h}]$. Consider the map $\rho :\mathfrak{h}\rightarrow$ End$_k(M)$ defined by

$$
\rho (x) =x_M-\lambda (x)1_M
$$

from the above, this is a representation of $\mathfrak{h}$ on M, and $\rho (x)$ is nilpotent for all $x\in \mathfrak{h}$. By Engel’s theorem (Chap. I, §4, no. 2, Th. 1), there exists $m\not= 0$ in M such that $\rho (x)m= 0$ for all $x\in \mathfrak{h}$, so $m\in M_{\lambda}(\mathfrak{h})$.

The first assertion of (v) follows from no. 1, Prop. 2 (ii). To prove the second, we can assume that $k$ is algebraically closed in view of Prop. 1 of no. 1; it then follows from the first and the fact that $M =\sum_{\lambda}M^{\lambda}(\mathfrak{h}), N =\sum_{\lambda}N^{\lambda}(\mathfrak{h})$, cf. (i).

#### Remark {#lie-vii-s1-n3-rem-1 .statement tag=00SY}

Assume that $k$ is perfect and of characteristic 2. Let $\mathfrak{h}=\mathfrak{s}\mathfrak{l}(2, k)$, and

$$
_2(ab)
$$

let M be the $\mathfrak{h}$-module $k$ (for the identity map of $\mathfrak{h})$. If $x=$ is an

$$
ca
$$

arbitrary element of $\mathfrak{h}$, denote by $\lambda (x)$ the unique $\lambda \in k$ such that $\lambda^2=a^2+bc$. A calculation shows immediately that $M = M^{\lambda}(\mathfrak{h})$; on the other hand, $M_{\lambda}(\mathfrak{h}) = 0$ and $\lambda$ is neither linear nor zero on $[\mathfrak{h},\mathfrak{h}]$, even though $\mathfrak{h}$ is nilpotent.

#### Corollary {#lie-vii-s1-n3-cor-1 .statement tag=00SZ}

Let $\mathfrak{h}$ be a nilpotent Lie algebra, and M a finite dimensional $\mathfrak{h}$-module such that $M^0(\mathfrak{h}) = 0$. Let $f:\mathfrak{h}\rightarrow M$ be a linear map such that

$f([x, y]) =x.f(y)-y.f(x)$ for $x, y\in \mathfrak{h}$.

There exists $a\in M$ such that $f(x) =x.a$ for all $x\in \mathfrak{h}$.

Let $N = M\times k$. Make $\mathfrak{h}$ operate on N by the formula

$$
x.(m, \lambda ) = (x.m-\lambda f(x),0)
$$

The identity satisfied by $f$ implies that N is an $\mathfrak{h}$-module (Chap. I, §1, no. 8, Example 2). The map $(m, \lambda ) \rightarrow \lambda$ from N to $k$ is a homomorphism from N to the trivial $\mathfrak{h}$-module $k$. By Prop. 9 (iv), it follows that $N^0(\mathfrak{h})$ contains an element of the form $(a,1)$ with $a\in M$. In view of the hypothesis on M,

$$
(M\times 0)\cap N^0(\mathfrak{h}) = 0
$$

so $N^0(\mathfrak{h})$ is of dimension 1 and hence is annihilated by $\mathfrak{h}$. Thus, $x.a-f(x) = 0$ for all $x\in \mathfrak{h}$, which proves the corollary.

#### Proposition 10 {#lie-vii-s1-prop-10 .statement tag=00T0}

Let $\mathfrak{g}$ be a Lie algebra, $\mathfrak{h}$ a nilpotent subalgebra of $\mathfrak{g}$. Denote by P the set of maps from $\mathfrak{h}$ to $k$.

(i) For $\lambda , \mu\in P$, $[\mathfrak{g}^{\lambda}(\mathfrak{h}),\mathfrak{g}^\mu(\mathfrak{h})]\subset \mathfrak{g}^{\lambda+\mu}(\mathfrak{h})$; in particular, $\mathfrak{g}^0(\mathfrak{h})$ is a Lie subalgebra of $\mathfrak{g}$ containing $\mathfrak{h}$, and the $\mathfrak{g}^{\lambda}(\mathfrak{h})$ are stable under ad $\mathfrak{g}^0(\mathfrak{h})$. Moreover, $\mathfrak{g}^0(\mathfrak{h})$ is its own normalizer in $\mathfrak{g}$.

(ii) If M is a $\mathfrak{g}$-module, $\mathfrak{g}^{\lambda}(\mathfrak{h})M^\mu(\mathfrak{h})\subset M^{\lambda+\mu}(\mathfrak{h})$ for $\lambda , \mu\in P$; in particular, each $M^{\lambda}(\mathfrak{h})$ is a $\mathfrak{g}^0(\mathfrak{h})$-module.

(iii) If B is a bilinear form on $\mathfrak{g}$ invariant under $\mathfrak{h},\mathfrak{g}^{\lambda}(\mathfrak{h})$ and $\mathfrak{g}^\mu(\mathfrak{h})$ are orthogonal relative to B for $\lambda +\mu\not= 0$. Assume that B is non-degenerate. Then, for all $\lambda \in P$, the restriction of B to $\mathfrak{g}^{\lambda}(\mathfrak{h})\times \mathfrak{g}^{-\lambda}(\mathfrak{h})$ is non-degenerate; in particular, the restriction of B to $\mathfrak{g}^0(\mathfrak{h})\times \mathfrak{g}^0(\mathfrak{h})$ is non-degenerate.

(iv) Assume that $k$ is of characteristic 0. Then, if $x\in \mathfrak{g}^{\lambda}(\mathfrak{h})$ with $\lambda \not= 0$, ad $x$ is nilpotent.

The map $(x, y) \rightarrow [x, y]$ from $\mathfrak{g}\times \mathfrak{g}$ to $\mathfrak{g}$ is $\mathfrak{g}$-invariant by the Jacobi identity, hence $\mathfrak{h}$-invariant. The first part of (i) thus follows from Prop. 2 (ii). Part (ii) is proved similarly.

If $x$ belongs to the normalizer of $\mathfrak{g}^0(\mathfrak{h})$ in $\mathfrak{g}$, (ad $y).x=-[x, y]\in \mathfrak{g}^0(\mathfrak{h})$ for all $y\in \mathfrak{h}$, so (ad $y)^n.x= 0$ for $n$ sufficiently large. This proves that $x\in \mathfrak{g}^0(\mathfrak{h})$. Assertion (i) is now completely proved.

Assertion (iii) follows from Prop. 9 (v).

To prove (iv), we can assume that $k$ is algebraically closed. Let $x\in \mathfrak{g}^{\lambda}(\mathfrak{h})$, with $\lambda \not= 0$. For all $\mu\in P$ and any integer $n\geq 0$, (ad $x)^n\mathfrak{g}^\mu(\mathfrak{h})\subset \mathfrak{g}^{\mu+n\lambda}(\mathfrak{h})$; let $P_1$ be the finite set of $\mu\in P$ such that $\mathfrak{g}^\mu(\mathfrak{h})\not= 0$; if $k$ is of characteristic 0 and $\lambda \not= 0, (P_1+n\lambda )\cap P_1=\emptyset$ for $n$ sufficiently large, so (ad $x)^n= 0$.

#### Lemma 2 {#lie-vii-s1-lem-2 .statement tag=00T1}

Assume that $k$ is of characteristic 0. Let $\mathfrak{g}$ be a semi-simple Lie algebra over $k$, B the Killing form of $\mathfrak{g},\mathfrak{m}$ a subalgebra of $\mathfrak{g}$. Assume that the following conditions are satisfied:

1) the restriction of B to $\mathfrak{m}$ is non-degenerate;

2) if $x\in \mathfrak{m}$, the semi-simple and nilpotent components$^1$ of $x$ in $\mathfrak{g}$ belong to $\mathfrak{m}$.

Then $\mathfrak{m}$ is reductive in $\mathfrak{g}$ (Chap. I, § 6, no. 6).

By Chap. I, §6, no. 4, Prop. $5d),\mathfrak{m}$ is reductive. Let $\mathfrak{c}$ be the centre of $\mathfrak{m}$. If $x\in \mathfrak{c}$ is nilpotent, then $x= 0$; indeed, for all $y\in \mathfrak{m}$, ad $x$ and ad $y$ commute, their composition ad $x\circ$ ad $y$ is nilpotent, and $B(x, y) = 0$, so $x= 0$. Now let $x$ be an arbitrary element of $\mathfrak{c}$; let $s$ and $n$ be its semi-simple and nilpotent components. We have $n\in \mathfrak{m}$. Since ad $n$ is of the form P(ad $x)$, where P is a polynomial with no constant term, (ad $n).\mathfrak{m}= 0$ and so $n\in \mathfrak{c}$, and then $n= 0$ by the above. Thus ad $x$ is semi-simple. Consequently, the restriction to $\mathfrak{m}$ of the adjoint representation of $\mathfrak{g}$ is semi-simple (Chap. I, §6, no. 5, Th. $4b))$.

#### Proposition 11 {#lie-vii-s1-prop-11 .statement tag=00T2}

Assume that $k$ is of characteristic 0. Let $\mathfrak{g}$ be a semi-simple Lie algebra, $\mathfrak{h}$ a nilpotent subalgebra of $\mathfrak{g}$. The algebra $\mathfrak{g}^0(\mathfrak{h})$ satisfies conditions (1) and (2) of Lemma 2 ; it is reductive in $\mathfrak{g}$.

$^1$ By Chap. I, §6, no. 3, Th. 3, every $x\in \mathfrak{g}$ can be written uniquely as the sum of a semi-simple element $s$ and a nilpotent element $n$ that commute with each other; the element $s$ (resp. $n)$ is called the semi-simple (resp. nilpotent) component of $x$.

Let $x, x'\in \mathfrak{g},s$ and $s'$ their semi-simple components, $n$ and $n'$ their nilpotent components. We have

$x'\in \mathfrak{g}^0(x)\Leftarrow \Rightarrow$ (ad $s)(x') = 0$ (Prop$.4)$

$\Leftarrow \Rightarrow$ (ad $x')(s) = 0$

$=\Rightarrow$ (ad $s')(s) = 0$

$\Leftarrow \Rightarrow$ (ad $s)(s') = 0$

$\Leftarrow \Rightarrow s'\in \mathfrak{g}^0(x)$ (Prop$.4)$

so $x'\in \mathfrak{g}^0(x)\Rightarrow n'\in \mathfrak{g}^0(x)$ and (2) is proved. The Killing form of $\mathfrak{g}$ is non-degenerate, so its restriction to $\mathfrak{g}^0(\mathfrak{h})$ is non-degenerate (Prop. 10 (iii)). The fact that $\mathfrak{g}^0(\mathfrak{h})$ is reductive in $\mathfrak{g}$ thus follows from Lemma 2.

### 4. DECOMPOSITION OF A LIE ALGEBRA RELATIVE TO AN AUTOMORPHISM

#### Proposition 12 {#lie-vii-s1-prop-12 .statement tag=00T3}

Let $\mathfrak{g}$ be a Lie algebra, $a$ an automorphism of $\mathfrak{g}$.

(i) For $\lambda , \mu\in k,[\mathfrak{g}^{\lambda}(a),\mathfrak{g}^\mu(a)]\subset \mathfrak{g}^{\lambda \mu}(a)$; in particular, $\mathfrak{g}^1(a)$ is a subalgebra of $\mathfrak{g}$.

(ii) If B is a symmetric bilinear form on $\mathfrak{g}$ invariant under $a,\mathfrak{g}^{\lambda}(a)$ and $\mathfrak{g}^\mu(a)$ are orthogonal relative to B for $\lambda \mu\not= 1$. Assume that B is non-degenerate. Then, if $\lambda \not= 0$, the restriction of B to $\mathfrak{g}^{\lambda}(a)\times \mathfrak{g}^{1/\lambda}(a)$ is non-degenerate.

Assertion (i) and the first half of (ii) follow from Prop. 2 (iii) applied to the composition law $\mathfrak{g}\times \mathfrak{g}\rightarrow \mathfrak{g}$ and the bilinear form B. To prove the second half of (ii), we can assume that $k$ is algebraically closed. Then $\mathfrak{g}=\bigoplus_{\nu\in k}\mathfrak{g}^{\nu}(a)$. In view of the above, $\mathfrak{g}^{\lambda}(a)$ is orthogonal to $\mathfrak{g}^{\nu}(a)$ if $\lambda \nu \not= 1$; since B is non-degenerate, it follows that its restriction to $\mathfrak{g}^{\lambda}(a)\times \mathfrak{g}^{1/\lambda}(a)$ is also.

#### Corollary {#lie-vii-s1-n4-cor-1 .statement tag=00T4}

Assume that $k$ is of characteristic zero and that $\mathfrak{g}$ is semi-simple. Then the subalgebra $\mathfrak{g}^1(a)$ satisfies conditions (1) and (2) of Lemma 2 ; it is reductive in $\mathfrak{g}$.

Condition (1) follows from part (ii) of Prop. 12; condition (2) follows from Prop. 4 of no. 1.

### 5. INVARIANTS OF A SEMI-SIMPLE LIE ALGEBRA RELATIVE TO A SEMI-SIMPLE ACTION

In this no., $k$ is assumed to be of characteristic zero.

#### Proposition 13 {#lie-vii-s1-prop-13 .statement tag=00T5}

Let $\mathfrak{g}$ be a semi-simple Lie algebra, $\mathfrak{a}$ a subalgebra of $\mathfrak{g}$ reductive in $\mathfrak{g}$, and $\mathfrak{m}$ the commutant of $\mathfrak{a}$ in $\mathfrak{g}$. The subalgebra $\mathfrak{m}$ satisfies conditions (1) and (2) of Lemma 2 of no. 3; it is reductive in $\mathfrak{g}$.

By Prop. 6 of Chap. I, §3, no. 5, applied to the $\mathfrak{a}$-module $\mathfrak{g}$, we have $\mathfrak{g}=\mathfrak{m}\oplus [\mathfrak{a},\mathfrak{g}]$. Let B be the Killing form of $\mathfrak{g}$, and let $x\in \mathfrak{a}, y\in \mathfrak{m}, z\in \mathfrak{g}$. Then,

$B([z, x], y) = B(z,[x, y]) = 0$ since $[x, y] = 0$,

which shows that $\mathfrak{m}$ is orthogonal to $[\mathfrak{a},\mathfrak{g}]$ relative to B. Since B is non-degenerate, and since $\mathfrak{g}=\mathfrak{m}\oplus [\mathfrak{a},\mathfrak{g}]$, this implies that the restriction of B to $\mathfrak{m}$ is non-degenerate; condition (1) of Lemma 2 is thus satisfied.

Now let $x\in \mathfrak{m}$ and let $s$ and $n$ be its semi-simple and nilpotent components. The semi-simple component of ad $x$ is ad $s$, cf. Chap. I, §6, no. 3. Since ad $x$ is zero on $\mathfrak{a}$, so is ad $s$, by Prop. 4 (i). Thus $s\in \mathfrak{m}$, so $n=x-s\in \mathfrak{m}$, and condition (2) of Lemma 2 is satisfied.

#### Remark {#lie-vii-s1-n5-rem-1 .statement tag=00T6}

The commutant of $\mathfrak{m}$ in $\mathfrak{g}$ does not necessarily reduce to $\mathfrak{a}$, cf. Exerc. 4.

#### Proposition 14 {#lie-vii-s1-prop-14 .statement tag=00T7}

Let $\mathfrak{g}$ be a semi-simple Lie algebra, A a group and $r$ a homomorphism from A to Aut($\mathfrak{g}$). Let $\mathfrak{m}$ be the subalgebra of $\mathfrak{g}$ consisting of the elements invariant under $r(A)$. Assume that the linear representation $r$ is semi-simple. Then $\mathfrak{m}$ satisfies conditions (1) and (2) of Lemma 2 of no. 3; it is reductive in $\mathfrak{g}$.

The proof is analogous to that of the preceding proposition:

Let $\mathfrak{g}^+$ be the vector subspace of $\mathfrak{g}$ generated by the $r(a)x-x,a\in A, x\in \mathfrak{g}$. The vector space $\mathfrak{g}'=\mathfrak{m}+\mathfrak{g}^+$ is stable under $r(A)$. Let $\mathfrak{n}$ be a complement of $\mathfrak{g}'$ in $\mathfrak{g}$ stable under $r(A)$. If $x\in \mathfrak{n}, a\in A,r(a)x-x\in \mathfrak{n}\cap \mathfrak{g}^+= 0$, so $x\in \mathfrak{m}$ and then $x= 0$ since $\mathfrak{m}\cap \mathfrak{n}= 0$. Thus, $\mathfrak{g}=\mathfrak{g}'=\mathfrak{m}+\mathfrak{g}^+$. Let B be the Killing form of $\mathfrak{g}$ and let $y\in \mathfrak{m}, a\in A, x\in \mathfrak{g}$. Then

$$
B(y, r(a)x-x) = B(y, r(a)x)-B(y, x)
$$

$$
= B(r(a^{-1})y, x)-B(y, x)
$$

$$
= B(y, x)-B(y, x) = 0
$$

Thus $\mathfrak{m}$ and $\mathfrak{g}^+$ are orthogonal relative to B. It follows that the restriction of B to $\mathfrak{m}$ is non-degenerate; hence condition (1) of Lemma 2. Condition (2) is immediate by transport of structure.

### Exercises {#lie-vii-s1-exercises}

All Lie algebras and modules over them are assumed to be finite dimensional over $k$; from §3 onwards, $k$ is assumed to be of characteristic zero.

See the [exercises for § 1](exercises/s1/).
