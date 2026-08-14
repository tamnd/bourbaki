---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: VIII
chapter_title: SPLIT SEMI-SIMPLE LIE ALGEBRAS
section: 9
section_title: The formula of Hermann Weyl
lang: en
source: lie-vii-ix
book_pages: A VIII.152-A VIII.159, A VIII.253-A VIII.260
pdf_pages: 0160-0167, 0261-0268
extraction: native
subsections:
    - "no": 1
      title: CHARACTERS OF FINITE DIMENSIONAL $\mathfrak{g}$-MODULES
      page: 152
      pdf_page: 160
    - "no": 2
      title: DIMENSIONS OF SIMPLE $\mathfrak{g}$-MODULES
      page: 154
      pdf_page: 162
    - "no": 3
      title: MULTIPLICITIES OF WEIGHTS OF SIMPLE $\mathfrak{g}$-MODULES
      page: 156
      pdf_page: 164
    - "no": 4
      title: DECOMPOSITION OF TENSOR PRODUCTS OF SIMPLE $\mathfrak{g}$-MODULES
      page: 157
      pdf_page: 165
statements: 12
exercises: 16
content_sha256: 68416a9d214702b4eca05fde66d670a50e9ced5b1715e7bbcb79d7fd9795a8c8
---

## § 9. THE FORMULA OF HERMANN WEYL

In this paragraph, we retain the general notations of §6 and §7.

### 1. CHARACTERS OF FINITE DIMENSIONAL $\mathfrak{g}$-MODULES

Let $(e^{\lambda})_{\lambda\in\mathfrak{h}^*}$ be the canonical basis of the ring $\mathbf{Z}[\mathfrak{h}^*]$. Give the space $\mathbf{Z}^{\mathfrak{h}^*}$ of all maps from $\mathfrak{h}^*$ to $\mathbf{Z}$ the product topology of the discrete topologies on the factors. If $\varphi \in \mathbf{Z}^{\mathfrak{h}^*}$, the family $(\varphi (\nu )e^{\nu})_{\nu\in\mathfrak{h}^*}$ is summable, and

$$
\varphi =\sum_{\nu\in\mathfrak{h}^*}\varphi (\nu )e^{\nu}
$$

Let $\mathbf{Z}\langle P\rangle$ be the set of $\varphi \in \mathbf{Z}^{\mathfrak{h}^*}$ whose support is contained in a finite union of sets of the form $\nu -P_+$, where $\nu \in \mathfrak{h}^*$. Then $\mathbf{Z}[P]\subset \mathbf{Z}\langle P\rangle  \subset \mathbf{Z}^{\mathfrak{h}^*}$. Define on $\mathbf{Z}\langle P\rangle$ a ring structure extending that of $\mathbf{Z}[P]$ by putting, for $\varphi , \psi \in \mathbf{Z}\langle P\rangle$ and $\nu \in \mathfrak{h}^*$,

$$
(\varphi \psi )(\nu ) =\sum_{\mu\in\mathfrak{h}^*}\varphi (\mu)\psi (\nu -\mu)
$$

(the family $(\varphi (\mu)\psi (\nu -\mu))_{\mu\in\mathfrak{h}^*}$ has finite support, in view of the condition satisfied by the supports of $\varphi$ and $\psi )$. If $\varphi =\sum_{\nu}x_{\nu}e^{\nu}$ and $\psi =\sum_{\nu}y_{\nu}e^{\nu}$, then $\varphi \psi =\sum_{\nu ,\mu}x_{\nu}y_\mu e^{\nu+\mu}$.

Let $\nu \in \mathfrak{h}^*$. A partition of $\nu$ into positive roots is a family $(n_{\alpha})_{\alpha\in R_+}$, where the $n_{\alpha}$ are integers $\geq 0$ such that $\nu =\sum_{\alpha\in R_+}n_{\alpha}\alpha$. We denote by $\mathfrak{P}(\nu )$ the number of partitions of $\nu$ into positive roots. We have

$$
\mathfrak{P}(\nu )>0\Leftarrow \Rightarrow \nu \in Q_+
$$

In this paragraph, we denote by K the following element of $\mathbf{Z}\langle P\rangle :$

$$
K =\sum_{\gamma\in Q_+}\mathfrak{P}(\gamma )e^{-\gamma}
$$

Now recall (Chap. VI, §3, no. 3, Prop. 2) that

$$
d=\prod_{\alpha\in R_+}(e^{\alpha /2}-e^{-\alpha /2}) =\sum_{w\in W}\varepsilon (w)e^{w\rho}
$$

is an anti-invariant element of $\mathbf{Z}[P]$.

#### Lemma 1 {#lie-viii-s9-lem-1 .statement tag=015T}

In the ring $\mathbf{Z}\langle P\rangle$, we have $K.\prod_{\alpha\in R_+}(1-e^{-\alpha}) = Ke^{-\rho}d= 1$.

Indeed,

$$
K =\prod_{\alpha\in R_+}(e^0+e^{-\alpha}+e^{-2\alpha}+\cdots )
$$

so

$$
Ke^{-\rho}d=\prod_{\alpha\in R_+}(1 +e^{-\alpha}+e^{-2\alpha}+\cdots )\prod_{\alpha\in R_+}(1-e^{-\alpha}) = 1
$$

#### Lemma 2 {#lie-viii-s9-lem-2 .statement tag=015U}

Let $\lambda \in \mathfrak{h}^*$. The module $Z(\lambda ) ($§6, no. 3) admits a character that is an element of $\mathbf{Z}\langle P\rangle$, and we have $d$. ch $Z(\lambda ) =e^{\lambda+\rho}$.

Let $\alpha_1, . . . , \alpha_q$ be distinct elements of $R_+$. The $X_{-\alpha_1}^{n_1}X_{-\alpha_2}^{n_2}. . . X_{-\alpha_q}^{n_q}\otimes 1$ form a basis of $Z(\lambda ) ($§6, Prop. 6 (iii)). For $h\in \mathfrak{h}$, we have

$$
h.(X_{-\alpha_1}^{n_1}X_{-\alpha_2}^{n_2}. . .X_{-\alpha_q}^{n_q}\otimes 1)
$$

$$
= [h, X_{-\alpha_1}^{n_1}. . . X_{-\alpha_q}^{n_q}]\otimes 1 + (X_{-\alpha_1}^{n_1}. . . X_{-\alpha_q}^{n_q})\otimes h.1
$$

$$
= (\lambda -n_1\alpha_1- \cdots  -n_q\alpha_q)(h)(X_{-\alpha_1}^{n_1}. . . X_{-\alpha_q}^{n_q}\otimes 1)
$$

Thus, the dimension of $Z(\lambda )^{\lambda-\mu}$ is $\mathfrak{P}(\mu)$. This proves that ch $Z(\lambda )$ is defined, is an element of $\mathbf{Z}\langle P\rangle$, and that

ch $Z(\lambda ) =\sum_\mu\mathfrak{P}(\mu)e^{\lambda-\mu}= Ke^{\lambda}$.

It now suffices to apply Lemma 1.

#### Lemma 3 {#lie-viii-s9-lem-3 .statement tag=015V}

Let M be a $\mathfrak{g}$-module which admits a character ch(M) whose support is contained in a finite union of the sets $\mu-P_+$. Let U be the enveloping algebra of $\mathfrak{g}$, Z the centre of U$,\lambda_0\in \mathfrak{h}^*$, and $\chi_{\lambda_0}$ the corresponding homomorphism from Z to $k($§8, Cor. 1 of Th. 2). Assume that, for all $z\in Z,z_M$ is the homothety with ratio $\chi_{\lambda_0}(z)$. Let $D_M$ be the set of $\lambda \in W(\lambda_0+\rho )-\rho$ such that $\lambda + Q_+$ meets Supp(ch M). Then ch(M) is a $\mathbf{Z}$-linear combination of the ch $Z(\lambda )$ for $\lambda \in D_M$.

If Supp(ch M) is empty, the lemma is clear. Assume that Supp(ch $M)\not=\emptyset$. Let $\lambda$ be a maximal element of this support, and put dim $M^{\lambda}=m$. There exists a $\mathfrak{g}$-homomorphism $\varphi$ from $(Z(\lambda ))^m$ to M which maps $(Z(\lambda )^{\lambda})^m$ bijectively onto $M^{\lambda}($§6, no. 3, Prop. 6 (i)). Thus, the central character of $Z(\lambda )$ is $\chi_{\lambda_0}$, so $\lambda \in W(\lambda_0+\rho )-\rho ($§8, no. 5, Cor. 1 of Th. 2). This proves that $D_M\not=\emptyset$, and allows us to argue by induction on Card $D_M$. Let L and N be the kernel and cokernel of $\varphi$. Then we have an exact sequence of $\mathfrak{g}$-homomorphisms:

$$
0\rightarrow L\rightarrow (Z(\lambda ))^m\rightarrow M\rightarrow N\rightarrow 0
$$

so

ch(M) $=-$ch(L) $+m$ ch $Z(\lambda ) +$ ch(N)

(§7, no. 7, formula (6)). The sets Supp(ch L) and Supp(ch N) are contained in a finite union of sets $\mu-P_+$. For $z\in Z,z_L$ and $z_N$ are homotheties with ratio $\chi_{\lambda_0}(z)$. Clearly, $D_N\subset D_M$. On the other hand, $(\lambda + Q_+)\cap$Supp(ch $M) =\{\lambda \}$, and $\lambda  /\in$ Supp(ch N), so $\lambda  /\in D_N$ and

Card $D_N<$ Card $D_M$.

On the other hand, L is a submodule of $(Z(\lambda ))^m$; if $\lambda '\in D_L$, then $\lambda '+ Q_+$ meets Supp(ch $L)\subset$ Supp ch $Z(\lambda )$, so $\lambda \in \lambda '+ Q_+($§6, no. 1, Prop. 1 (ii)); it follows that $D_L\subset D_M$. Since $L\cap (Z(\lambda )^{\lambda})^m= 0$, we have $\lambda  /\in D_L$, so

Card $D_L<$ Card $D_M$.

It now suffices to apply the induction hypothesis.

#### Theorem 1 (Character Formula of H. Weyl) {#lie-viii-s9-thm-1 .statement tag=015W}

Let M be a finite dimensional simple $\mathfrak{g}$-module, and $\lambda$ its highest weight. Then

$(\sum_{w\in W}\varepsilon (w)e^{w\rho})$.ch $M =\sum_{w\in W}\varepsilon (w)e^{w(\lambda+\rho)}$.

With the notations of Lemma 3, the central character of M is $\chi_{\lambda}($§6, no. 4, Prop. 7). Hence, by Lemmas 2 and $3,d$.ch M is a $\mathbf{Z}$-linear combination of the $e^{\mu+\rho}$ such that

$$
\mu+\rho \in W(\lambda +\rho )
$$

On the other hand, by §7, no. 7, Lemma $7,d$.ch M is anti-invariant, and its unique maximal term is $e^{\lambda+\rho}$, hence the theorem.

#### Example {#lie-viii-s9-n1-exa-1 .statement tag=015X}

Take $\mathfrak{g}=\mathfrak{s}\mathfrak{l}(2, k),\mathfrak{h}=kH$. Let $\alpha$ be the root of $(\mathfrak{g},\mathfrak{h})$ such that $\alpha (H) = 2$. The $\mathfrak{g}$-module $V(m)$ has highest weight $(m/2)\alpha$. Hence

ch(V($m$)) $= (e^{(m/2)\alpha+^1_2\alpha}-e^{-(m/2)\alpha-^1_2\alpha})/(e^{^1_2\alpha}-e^{-^1_2\alpha})$

$$
=e^{-(m/2)\alpha}.(e^{(m+1)\alpha}-1)/(e^{\alpha}-1)
$$

$$
=e^{-(m/2)\alpha}(e^{m\alpha}+e^{(m-1)\alpha}+\cdots + 1)
$$

$$
=e^{(m/2)\alpha}+e^{(m-2)\alpha /2}+\cdots +e^{-(m/2)\alpha}
$$

which also follows easily from §1, no. 2, Prop. 2.

### 2. DIMENSIONS OF SIMPLE $\mathfrak{g}$-MODULES

If $\mu\in \mathfrak{h}^*$, put $J(e^\mu) =\sum_{w\in W}\varepsilon (w)e^{w\mu}$, cf. Chap. VI, §3, no. 3.

#### Theorem 2 {#lie-viii-s9-thm-2 .statement tag=015Y}

Let E be a finite dimensional simple $\mathfrak{g}$-module, $\lambda$ its highest weight and $(\cdot  | \cdot )$ a W-invariant non-degenerate positive symmetric bilinear form on $\mathfrak{h}^*$. Then:

$$
\prod\langle \lambda +\rho , H_{\alpha}\rangle \prod((\lambda |\alpha ))
$$

dim E = = 1 +.

$$
_{\alpha\in R_+}\langle \rho , H_{\alpha}\rangle_{\alpha\in R_+}(\rho |\alpha )
$$

Let T be an indeterminate. For all $\nu \in P$, denote by $f_{\nu}$ the homomorphism from $\mathbf{Z}[P]$ to $\mathbf{R}[[T]]$ that takes $e^\mu$ to $e^{(\nu|\mu)T}$ for all $\mu\in P$. Then dim E is the constant term of the series $f_{\nu}$(ch E).

For all $\mu, \nu \in P$, we have

$$
f_{\nu}(J(e^\mu)) =\sum_{w\in W}\varepsilon (w)e^{(\nu|w\mu)T}
$$

$$
=\sum_{w\in W}\varepsilon (w)e^{(w^{-1}\nu|\mu)T}=f_\mu(J(e^{\nu}))
$$

In particular, in view of Chap. VI, §3, no. 3, formula (3),

$$
f_{\rho}(J(e^\mu)) =f_\mu(J(e^{\rho})) =e^{(\mu|\rho)T}\prod_{\alpha\in R_+}(1-e^{-(\mu|\alpha)T})
$$

Hence, setting Card(R$_+) = N$,

$f_{\rho}(J(e^\mu))\equiv T^N\prod_{\alpha\in R}(\mu|\alpha )$ (mod $T^{N+1}\mathbf{R}[[T]])$.

The equality $J(e^{\lambda+\rho}) =$ ch(E)$.J(e^{\rho})$ (Th. 1) thus implies that

$T^N\prod_{\alpha\in R_+}(\lambda +\rho |\alpha )\equiv f_{\rho}$(ch $E).T^N\prod_{\alpha\in R_+}(\rho |\alpha )$ (mod $T^{N+1}\mathbf{R}[[T]])$

so

$$
((\prod)/((\prod)\prod((\lambda |\alpha ))
$$

dim E = $(\lambda +\rho |\alpha )(\rho |\alpha )$ = 1 +.

$$
_{\alpha\in R_+}\alpha_{\in R_+}\alpha_{\in R_+}(\rho |\alpha )
$$

Now, if $\alpha \in R_+,\alpha$ can be identified with an element of $\mathfrak{h}_{\mathbf{R}}$ proportional to $H_{\alpha}$, so

$$
(\lambda +\rho |\alpha )/(\rho |\alpha ) =\langle \lambda +\rho , H_{\alpha}\rangle /\langle \rho , H_{\alpha}\rangle
$$

#### Example 1 {#lie-viii-s9-n2-exa-1 .statement tag=015Z}

In the Example of no. 1, we find that

$$
(m\alpha )\alpha
$$

dim $V(m) =\alpha +(H_{\alpha})/(H_{\alpha}) =m+ 1$,

2 2 2

which we knew in §1.

#### Example 2 {#lie-viii-s9-n2-exa-2 .statement tag=0160}

Take $\mathfrak{g}$ to be the splittable simple Lie algebra of type $G_2$ and adopt the notations of Chap. VI, Plate IX. Give $\mathfrak{h}^*_{\mathbf{R}}$ the W-invariant positive symmetric form $(\cdot  | \cdot )$ such that $(\alpha_1|\alpha_1) = 1$. Then $\rho =_1+_2$ and

1 1

( $_1|\alpha_1) =$, ( $_1|\alpha_2) = 0$, ( $_1|\alpha_2+\alpha_1) =$,

2 2

3 3

( $_1|\alpha_2+ 2\alpha_1) = 1$, ( $_1|\alpha_2+ 3\alpha_1) =$, ( $_1|2\alpha_2+ 3\alpha_1) =$,

2 2

3 3

( $_2|\alpha_1) = 0$, ( $_2|\alpha_2) =$, ( $_2|\alpha_2+\alpha_1) =$,

2 2

3 3

( $_2|\alpha_2+ 2\alpha_1) =$, ( $_2|\alpha_2+ 3\alpha_1) =$, ( $_2|2\alpha_2+ 3\alpha_1) = 3$.

2 2

Thus, if $n_1, n_2$ are integers $\geq 0$, the dimension of the simple representation

of highest weight $n_{11}+n_{22}$ is

$$
(n_1/2)((3n_2/2)((n_1/2 + 3n_2/2)((n_1+ 3n_2/2)
$$

1 + 1 + 1 + 1 +

$$
^1_23_21_2+^3_21 +^3_2
$$

$$
(3n_1/2 + 3n_2/2)((3n_1/2 + 3n_2)
$$

$\times$ 1 + $_{33}$ 1 + $_3$

$_2+_2$ 2 + 3

$$
(n_1+ 3n_2)((2n_1+ 3n_2)((n_1+n_2)
$$

$= (1 +n_1)(1 +n_2)$ 1 + 1 + 1 +

4 5 2

$$
\times (1 +n^1+ 2n^2)
$$

3

$$
(1+n_1)(1+n_2)(2+n_1+n_2)(3+n_1+2n_2)(4+n_1+3n_2)(5+2n_1+3n_2)
$$

=.

5!

In particular, the fundamental representation of highest weight $_1$ (resp. $_2)$ is of dimension 7 (resp. 14).

### 3. MULTIPLICITIES OF WEIGHTS OF SIMPLE $\mathfrak{g}$-MODULES

#### Proposition 1 {#lie-viii-s9-prop-1 .statement tag=0161}

Let $\omega \in P_{++}$. For all $\lambda \in P$, the multiplicity of $\lambda$ in $E(\omega )$ is

$$
m_{\lambda}=\sum_{w\in W}\varepsilon (w)\mathfrak{P}(w(\omega +\rho )-(\lambda +\rho ))
$$

By Th. 1 and Lemma 1,

ch $E(\omega ) = Ke^{-\rho}d$ ch $E(\omega ) = Ke^{-\rho}\sum_{w\in W}\varepsilon (w)e^{w(\omega+\rho)}$

so

ch $E(\omega ) =\sum_{w\in W,\gamma\in Q_+}\varepsilon (w)\mathfrak{P}(\gamma )e^{-\rho+w(\omega+\rho)-\gamma}$

and

$$
m_{\lambda}=\sum\varepsilon (w)\mathfrak{P}(\gamma )
$$

$w\in W,\gamma \in Q_+,\gamma =-\lambda -\rho +w(\omega +\rho )$

#### Corollary {#lie-viii-s9-n3-cor-1 .statement tag=0162}

If $\lambda$ is a weight of $E(\omega )$ distinct from $\omega$,

$$
m_{\lambda}=-\sum_{w\in W,w\not=1}\varepsilon (w)m_{\lambda+\rho-w\rho}
$$

Apply Prop. 1 with $\omega = 0$. If $\mu\in P$**--** $\{0\}$, we find that

$$
0 =\sum_{w\in W}\varepsilon (w)\mathfrak{P}(w\rho +\mu-\rho )
$$

hence

$$
\mathfrak{P}(\mu) =-\sum_{w\in W,w\not=1}\varepsilon (w)\mathfrak{P}(\mu+w\rho -\rho ) \tag{1}
$$

Prop. 1 also gives

$$
m_{\lambda}=-\sum_{w\in W}\varepsilon (w)\sum_{w'\in W,w'\not=1}\varepsilon (w')\mathfrak{P}(w(\omega +\rho )-(\lambda +\rho ) +w'\rho -\rho )
$$

since $w(\omega +\rho )\not=\lambda +\rho$ for all $w\in W ($§7, Prop. 5 (iii)). Hence,

$$
m_{\lambda}=-\sum_{w'\in W,w'\not=1}\varepsilon (w')\sum_{w\in W}\varepsilon (w)\mathfrak{P}(w(\omega +\rho )-(\lambda +\rho -w'\rho +\rho ))
$$

$=-\sum_{w'\in W,w'\not=1}\varepsilon (w')m_{\lambda+\rho-w'\rho}$ (Prop$.1)$.

### 4. DECOMPOSITION OF TENSOR PRODUCTS OF SIMPLE $\mathfrak{g}$-MODULES

#### Proposition 2 {#lie-viii-s9-prop-2 .statement tag=0163}

Let $\lambda , \mu\in P_{++}$. In $\mathscr{R}(\mathfrak{g})$, we have

$$
[\lambda ].[\mu] =\sum_{\nu\in P_{++}}m(\lambda , \mu, \nu )[\nu ]
$$

with

$$
m(\lambda , \mu, \nu ) =\sum_{w,w'\in W}\varepsilon (ww')\mathfrak{P}(w(\lambda +\rho ) +w'(\mu+\rho )-(\nu + 2\rho ))
$$

Let $E,F$ be finite dimensional simple $\mathfrak{g}$-modules of highest weights $\lambda , \mu$. Let $l_{\nu}$ be the length of the isotypical component of $E\otimes F$ of highest weight $\nu$. It suffices to show that

$$
l_{\nu}=\sum_{w,w'\in W}\varepsilon (ww')\mathfrak{P}(w(\lambda +\rho ) +w'(\mu+\rho )-(\nu + 2\rho )) \tag{2}
$$

Put $c_1=$ ch(E) $=\sum_{\sigma\in P}m_{\sigma}e^{\sigma},c_2=$ ch(F), and $d= J(e^{\rho})$, where J is defined as in no. 2. We have

$\sum_{\xi\in P_{++}}l_{\xi}$ch[$\xi ] =$ ch(E $\otimes F) =c_1c_2$

so, after multiplying by $d$ and using Th. 1,

$$
\sum_{\xi\in P_{++}}l_{\xi}J(e^{\xi+\rho}) =c_1J(e^{\mu+\rho}) =(\sum_{\sigma\in P}m_{\sigma}e^{\sigma})((\sum_{w\in W}\varepsilon (w)e^{w(\mu+\rho)}) \tag{3}
$$

$$
=\sum_{\tau\in P}(\sum_{w\in W}\varepsilon (w)m_{\tau+\rho-w(\mu+\rho)})e^{\tau+\rho}
$$

Now, if $\xi \in P_{++},\xi +\rho$ belongs to the chamber defined by B (Chap. VI, §1, no. 10); thus, for all $w\in W$ distinct from 1, we have $w(\xi +\rho )\in /P_{++}$. Consequently, the coefficient of $e^{\nu+\rho}$ in $\sum_{\xi\in P_{++}}l_{\xi}J(e^{\xi+\rho})$ is equal to $l_{\nu}$. In view of (3), we obtain

$$
l_{\nu}=\sum_{w\in W}\varepsilon (w)m_{\nu+\rho-w(\mu+\rho)}
$$

that is, by Prop. 1,

$$
l_{\nu}=\sum_{w,w'\in W}\varepsilon (w)\varepsilon (w')\mathfrak{P}(w'(\lambda +\rho )-(\nu +\rho -w(\mu+\rho ) +\rho ))
$$

which proves (2).

#### Example {#lie-viii-s9-n4-exa-1 .statement tag=0164}

We return to the Example of no. 1. Let $\lambda = (n/2)\alpha , \mu= (p/2)\alpha$, $\nu = (q/2)\alpha$ with $n\geq p$. We have

$$
m(\lambda , \mu, \nu ) =\mathfrak{P}(n\alpha +\alpha +p\alpha +\alpha -q\alpha -\alpha )
$$

2 2 2 2 2

$$
(n\alpha p\alpha q)
$$

$$
-\mathfrak{P}\alpha +-\alpha --\alpha -\alpha
$$

2 2 2 2 2

$$
-\mathfrak{P}(-n\alpha -\alpha +p\alpha +\alpha -q\alpha -\alpha )
$$

2 2 2 2 2

$$
(n\alpha p\alpha q)
$$

$$
+\mathfrak{P}-\alpha --\alpha --\alpha -\alpha
$$

2 2 2 2 2

$$
(n+p-q)(n-p-q-2)
$$

$$
=\mathfrak{P}\alpha -\mathfrak{P}\alpha
$$

2 2

This is zero if $n+p+q$ is not divisible by 2, or if $q\geq n+p$. If

$$
q=n+p-2r
$$

with $r$ an integer $\geq 0$, we have

$$
m(\lambda , \mu, \nu ) =\mathfrak{P}(r\alpha )-\mathfrak{P}((r-p-1)\alpha )
$$

hence $m(\lambda , \mu, \nu ) = 1$ if $r\leq p$ and $m(\lambda , \mu, \nu ) = 0$ if $r > p$. Finally, the $\mathfrak{g}$-module $V(n)\otimes V(p)$ is isomorphic to

$$
V(n+p)\oplus V(n+p-2)\oplus V(n+p-4)\oplus  \cdots  \oplus V(n-p)
$$

(Clebsch-Gordan formula).

### Exercises {#lie-viii-s9-exercises}

All the $\mathfrak{g}$-modules considered are assumed to be finite dimensional.

See the [exercises for § 9](exercises/s9/).
