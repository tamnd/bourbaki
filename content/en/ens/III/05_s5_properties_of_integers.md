---
book: ens
book_title: Theory of Sets
chapter: III
chapter_title: ORDERED SETS, CARDINALS, INTEGERS
section: 5
section_title: Properties of integers
lang: en
source: ens-i-iv
source_edition: 2004, Springer
book_pages: 171-183, 235-240
pdf_pages: 0177-0189, 0241-0246
extraction: ocr
subsections:
    - "no": 1
      title: OPERATIONS ON INTEGERS AND FINITE SETS
      page: 171
      pdf_page: 177
    - "no": 2
      title: STRICT INEQUALITIES BETWEEN INTEGERS
      page: 173
      pdf_page: 179
    - "no": 3
      title: INTERVALS IN SETS OF INTEGERS
      page: 174
      pdf_page: 180
    - "no": 4
      title: FINITE SEQUENCES
      page: 175
      pdf_page: 181
    - "no": 5
      title: CHARACTERISTIC FUNCTIONS OF SETS
      page: 175
      pdf_page: 181
    - "no": 6
      title: EUCLIDEAN DIVISION
      page: 176
      pdf_page: 182
    - "no": 7
      title: EXPANSION TO BASE $b$
      page: 177
      pdf_page: 183
    - "no": 8
      title: COMBINATORIAL ANALYSIS
      page: 179
      pdf_page: 185
statements: 30
exercises: 18
content_sha256: 8a102c1fe61e0d9ba0dfa780d76c5ac2d059f4ade38b37129f41be94b8afbf2f
---

## 5. PROPERTIES OF INTEGERS

### 1. OPERATIONS ON INTEGERS AND FINITE SETS

#### Proposition 1 {#ens-iii-s5-prop-1 .statement tag=03LP}

*Let $(a_i)_{i \in I}$ be a finite family of integers. Then the cardinals $\sum_{i \in I} a_i$ and $\prod_{i \in I} a_i$ are integers.*

Let us begin by showing that if $a$ and $b$ are integers, then so is $a + b$. We proceed by induction on $b$. The assertion is true for $b = 0$ since $a + 0 = a$. If $a + b$ is an integer, then so is $(a + b) + 1$ (§ 4, no. 1, Proposition 1). But $(a + b) + 1 = a + (b + 1)$ (§ 3, no. 3, Corollary to Proposition 5); hence $a + (b + 1)$ is an integer, and consequently $a + b$ is an integer for all integers $b$.

Next we show by induction on $n = \mathrm{Card}\ (\mathrm{I})$ that $\sum\limits_{i \in \mathrm{I}} a_i$ is an integer. This is clear if $n = 0$, for then $\mathrm{I} = \emptyset$ and $\sum\limits_{i \in \mathrm{I}} a_i = 0$. If $\mathrm{Card}\ (\mathrm{I}) = n + 1$, we may write $\mathrm{I} = \mathrm{J} \cup \{k\}$, where $\mathrm{Card}\ (\mathrm{J}) = n$ and $k \notin \mathrm{J}$. Then

$$\sum_{i \in \mathrm{I}} a_i = a_k + \sum_{i \in \mathrm{J}} a_i$$

($\S\,3$, no. 3, Proposition 5). The inductive hypothesis is that $\sum\limits_{i \in \mathrm{J}} a_i$ is an integer; hence so is $a_k + \sum\limits_{i \in \mathrm{J}} a_i$, from the first paragraph of the proof. This shows that $\sum\limits_{i \in \mathrm{I}} a_i$ is an integer for all $n$.

Since the product $ab$ of two integers $a$ and $b$ is the sum of a finite family of integers all equal to $a$ ($\S\,3$, no. 4, Proposition 6, Corollary 2), $ab$ is an integer. We shall prove by induction on $n = \mathrm{Card}\ (\mathrm{I})$ that $\prod\limits_{i \in \mathrm{I}} a_i$ is an integer. This is true for $n = 0$, because then

$$\prod_{i \in \mathrm{I}} a_i = 1.$$

If $\mathrm{Card}\ (\mathrm{I}) = n + 1$, we have (with the same notation as above)

$$\prod_{i \in \mathrm{I}} a_i = a_k \cdot \prod_{i \in \mathrm{J}} a_i$$

($\S\,3$, no. 3, Proposition 5), and the inductive hypothesis therefore implies that $\prod\limits_{i \in \mathrm{I}} a_i$ is an integer. Consequently $\prod\limits_{i \in \mathrm{I}} a_i$ is an integer for all $n$.

#### Corollary 1 {#ens-iii-s5-prop-1-cor-1 .statement tag=03LQ}

*The union* E *of a finite family* $(\mathrm{X}_i)_{i \in \mathrm{I}}$ *of finite sets is a finite set.*

For the sum S of the family $(\mathrm{X}_i)$ is finite; and since there exists a mapping of S onto E (Chapter II, $\S\,4$, no. 8), the set E is finite ($\S\,4$, no. 2, Proposition 2, Corollary 3).

#### Corollary 2 {#ens-iii-s5-prop-1-cor-2 .statement tag=03LR}

*The product of a finite family of finite sets is a finite set.*

#### Corollary 3 {#ens-iii-s5-prop-1-cor-3 .statement tag=03LS}

*If $a$ and $b$ are integers, $a^b$ is an integer.*

For $a^b$ is the product of a finite family of integers all equal to $a$ ($\S\,3$, no. 5, Proposition 10).

#### Corollary 4 {#ens-iii-s5-prop-1-cor-4 .statement tag=03LT}

*The set of subsets of a finite set* E *is finite.*

For its cardinal is $2^{\mathrm{Card}\ (\mathrm{E})}$ ($\S\,3$, no. 5, Proposition 12).

### 2. STRICT INEQUALITIES BETWEEN INTEGERS

#### Proposition 2 {#ens-iii-s5-prop-2 .statement tag=03LU}

*Let $a$ and $b$ be two integers. Then $a < b$ if and only if there exists an integer $c > 0$ such that $b = a + c$.*

If $a < b$, there exists a cardinal $c \leqslant b$ (so that $c$ is an integer (§ 4, no. 2, Proposition 2)) such that $b = a + c$ (§ 3, no. 6, Proposition 13); if $a \neq b$, we must have $c \neq 0$. Conversely, if $b = a + c$ and $c \neq 0$, then $c \geqslant 1$ and hence $a < a + 1 \leqslant a + c = b$.

#### Proposition 3 {#ens-iii-s5-prop-3 .statement tag=03LV}

*Let $(a_i)_{i \in I}$ and $(b)_{i \in I}$ be two finite families of integers such that $a_i \leqslant b_i$ for each $i \in I$ and $a_i < b_i$ for at least one index $i$. Then*

$$\sum_{i \in I} a_i < \sum_{i \in I} b_i.$$

*If also $b_i > 0$ for each $i \in I$, then*

$$\prod_{i \in I} a_i < \prod_{i \in I} b_i.$$

Let $j$ be an index such that $a_j < b_j$, and let $J = I - \{j\}$. Then

$$b_j = a_j + c_j$$

with $c_j > 0$ (Proposition 2), and therefore (§ 3, no. 6, Proposition 14)

$$\sum_{i \in I} b_i = a_j + c_j + \sum_{i \in J} b_i \geqslant c_j + a_j + \sum_{i \in J} a_i = c_j + \sum_{i \in I} a_i.$$

Since $c_j > 0$, the first part of the Proposition follows from Proposition 2. Likewise

$$\prod_{i \in I} b_i = (a_j + c_j) \prod_{i \in J} b_i = a_j . \prod_{i \in J} b_i + c_j . \prod_{i \in J} b_i \geqslant \prod_{i \in I} a_i + c_j . \prod_{i \in J} b_i.$$

Since $c_j$ and all the $b_i$ are $\neq 0$, the product $c_j . \prod_{i \in J} b_i$ is $\neq 0$ (§ 3, no. 4, Proposition 7); hence the second part of the Proposition.

#### Corollary 1 {#ens-iii-s5-prop-3-cor-1 .statement tag=03LW}

*Let $a$, $a'$, and $b$ be integers such that $a < a'$ and $b > 0$. Then $a^b < a'^b$.*

We need only express $a^b$ and $a'^b$ as products of finite families of integers (§ 3, no. 5, Proposition 10) and apply Proposition 3, observing that the relation $a < a'$ implies $a' > 0$.

#### Corollary 2 {#ens-iii-s5-prop-3-cor-2 .statement tag=03LX}

*Let $a$, $b$, and $b'$ be integers such that $a > 1$ and $b < b'$; then $a^b < a^{b'}$.*

For there exists an integer $c > 0$ such that $b' = b + c$ (Proposition 2); since $c \geqslant 1$, we have $a^c \geqslant a > 1$, whence $a^{b'} = a^b a^c > a^b$.

#### Corollary 3 {#ens-iii-s5-prop-3-cor-3 .statement tag=03LY}

*Let $a$, $b$, $b'$ be integers* (resp. *integers such that $a > 0$*). *Then $a + b = a + b'$* (resp. *$ab = ab'$*) *if and only if $b = b'$.*

#### Corollary 4 {#ens-iii-s5-prop-3-cor-4 .statement tag=03LZ}

*If $a$ and $b$ are integers such that $a \leqslant b$, then there exists a unique integer $c$ such that $b = a + c$.*

The existence of $c$ follows from Proposition 13 of § 3, no. 6, and its uniqueness from Corollary 3 above.

¶ The integer $c$ such that $b = a + c$ (where $a \leqslant b$) is called the *difference* of the integers $b$ and $a$, and is written $b - a$. It is easily verified that if $a$, $b$, $a'$, $b'$ are integers such that $a \leqslant b$ and $a' \leqslant b'$, then

$$(b - a) + (b' - a') = (b + b') - (a + a').$$

### 3. INTERVALS IN SETS OF INTEGERS

Every set of integers, being a set of cardinals, is well-ordered (§ 3, no. 2, Theorem 1). Furthermore, for each integer $a$ the relation "$x$ is a cardinal and $x \leqslant a$" is collectivizing in $x$ (§ 3, no. 2, Remark after Theorem 1), and the set of $x$ which satisfy this relation is a set of integers (§ 4, no. 2, Proposition 2), which may therefore be denoted by $[0, a]$.

#### Proposition 4 {#ens-iii-s5-prop-4 .statement tag=03M0}

*Let $a$ and $b$ be integers. Then the mapping $x \rightarrow a + x$ is a strictly inrceasing isomorphism of the interval $[0, b]$ onto the interval $[a, a + b]$, and $y \rightarrow y - a$ is the inverse isomorphism.*

Clearly the relations $0 \leqslant x \leqslant b$ imply $a \leqslant a + x \leqslant a + b$. The mapping $x \rightarrow a + x$ is strictly increasing (and therefore injective) by Proposition 3 of no. 2. Finally, the relations $a \leqslant y \leqslant a + b$ imply $y = a + x$ with $x \geqslant 0$ and $a + x \leqslant a + b$, whence $x \leqslant b$ (no. 2, Proposition 3). This completes the proof.

#### Proposition 5 {#ens-iii-s5-prop-5 .statement tag=03M1}

*If $a$ and $b$ are integers such that $a \leqslant b$, then the interval $[a, b]$ is a finite set whose number of elements is $b - a + 1$.*

By Proposition 4 we may restrict ouselves to the case where $a = 0$. The proof is by induction on $b$. If $b = 0$, the result is clear. The relation $0 \leqslant x \leqslant b + 1$ is equivalent to "$0 \leqslant x < b + 1$ or $x = b + 1$", and the relation $0 \leqslant x < b + 1$ is equivalent to $0 \leqslant x \leqslant b$ (§ 4, no. 2, Proposition 2); in other words, the interval $[0, b + 1]$ is the union of $[0, b]$

and $\{b + 1\}$, and these two sets are disjoint. By the inductive hypothesis the number of elements of $[0, b + 1]$ is equal to $(b + 1) + 1$, and the Proposition is proved.

#### Proposition 6 {#ens-iii-s5-prop-6 .statement tag=03M2}

*For every finite set* E *which is totally ordered and has n elements* $(n \geqslant 1)$, *there exists a unique isomorphism of* E *onto the interval* $[1, n]$.

Since E and $[1, n]$ are well-ordered (§ 4, no. 4, Proposition 3, Corollary 1) and have the same number of elements (Proposition 5), the result follows from Theorem 3 of § 2, no. 5 and Corollary 2 to Proposition 2 of § 4, no. 2.

### 4. FINITE SEQUENCES

A *finite sequence* (resp. *finite sequence of elements of a set* E) is a family (resp. a family of elements of E) whose index set I is a finite set of integers. The number of elements of I is called the *length* of the sequence.

Let $(t_i)_{i \in I}$ be a finite sequence of length $n$. By Proposition 6 of no. 3 there exists a unique isomorphism $f$ of the interval $[1, n]$ onto the set of integers I. For each $k \in [1, n]$, $t_{f(k)}$ is said to be the *kth term of the sequence*; $t_{f(1)}$ (resp. $t_{f(n)}$) is the *first* (resp. *last*) *term* of the sequence.

Let $\mathrm{P}\{i\}$ be a relation such that the elements $i$ for which $\mathrm{P}\{i\}$ is true form a finite set of integers. A finite sequence $(t_i)_{i \in I}$ is then often written $(t_i)_{\mathrm{P}\{i\}}$. For example, when $\mathrm{I} = [a, b]$, the notation $(t_i)_{a \leqslant i \leqslant b}$ is often used. Under the same conditions, to denote the product of a family of sets $(\mathrm{X}_i)_{i \in I}$ the notations

$$\prod_{\mathrm{P}\{i\}} \mathrm{X}_i \quad \text{and} \quad \prod_{i=a}^{b} \mathrm{X}_i$$

are used; and analogous notations for union, intersection, cardinal product, cardinal sum, \* composition laws in Algebra $_*$, and so on.

### 5. CHARACTERISTIC FUNCTIONS OF SETS

Let E be a non-empty set and A a subset of E. The *characteristic function* of the subset A of E is the mapping $\varphi_\mathrm{A}$ of E into the set $\{0, 1\}$ defined by

$$\varphi_\mathrm{A}(x) = 1 \quad \text{if} \quad x \in \mathrm{A}; \qquad \varphi_\mathrm{A}(x) = 0 \quad \text{if} \quad x \in \mathrm{E} - \mathrm{A}.$$

¶ Clearly the relation $\varphi_\mathrm{A} = \varphi_\mathrm{B}$ is equivalent to $\mathrm{A} = \mathrm{B}$. We have $\varphi_\mathrm{E}(x) = 1$ for all $x \in \mathrm{E}$ and $\varphi_{\emptyset}(x) = 0$ for all $x \in \mathrm{E}$; these are the only constant characteristic functions on E. The following Proposition is an immediate consequence of the definitions :

#### Proposition 7 {#ens-iii-s5-prop-7 .statement tag=03M3}

*For each pair of subsets* A, B *of a non-empty set* E, *we have*

(1) $$\varphi_{\mathrm{E-A}}(x) = 1 - \varphi_{\mathrm{A}}(x),$$

(2) $$\varphi_{\mathrm{A} \cap \mathrm{B}}(x) = \varphi_{\mathrm{A}}(x)\varphi_{\mathrm{B}}(x),$$

(3) $$\varphi_{\mathrm{A} \cup \mathrm{B}}(x) + \varphi_{\mathrm{A} \cap \mathrm{B}}(x) = \varphi_{\mathrm{A}}(x) + \varphi_{\mathrm{B}}(x)$$

*for all* $x \in \mathrm{E}$.

### 6. EUCLIDEAN DIVISION

#### Theorem 1 {#ens-iii-s5-thm-1 .statement tag=03M4}

*Let a and b be integers such that $b > 0$. Then there exist integers q and r such that $a = bq + r$ and $r < b$, and the integers q and r are uniquely determined by these conditions.*

The conditions on $q$ and $r$ are equivalent to $bq \leqslant a < b(q + 1)$ and $r = a - bq$ (no. 2, Proposition 2). Hence we have to find $q$ such that $bq \leqslant a < b(q + 1)$; in other words, $q$ must be the smallest integer such that $a < b(q + 1)$, which shows that $q$ and $r = a - bq$ are uniquely determined. To prove their existence, we note that there exist integers $p$ such that $a < bp$, for example $a + 1$ (since $b > 0$). Let $m$ be the least of these integers. We have $m \neq 0$, and we may therefore write $m = q + 1$ with $q \leqslant m$ (§ 4, no. 2, Proposition 2); it follows that $bq \leqslant a < b(q + 1)$.

#### Definition 1 {#ens-iii-s5-def-1 .statement tag=03M5}

*With the notation of Theorem 1, r is called the remainder of the division of a by b. If $r = 0$, we say that a is a multiple of b, or that a is divisible by b, or that b is a divisor of a, or that b divides a, or that b is a factor of a. The number q is then called the quotient of a by b and is denoted by $\dfrac{a}{b}$ or $a/b$.*

If $a$ is not a multiple of $b$, the number $q$ is called the *integral part of the quotient of a by b* (cf. *General Topology*, Chapter IV, § 8, no. 2).

*In this chapter*, writing $a/b$ or $\dfrac{a}{b}$ will imply that $b$ divides $a$.

The relations $a = bq$ and $q = a/b$ are equivalent (if $b > 0$). Every multiple $a'$ of a multiple $a$ of $b$ is a multiple of $b$, and

$$a'/b = (a'/a)\,(a/b) \qquad \text{if} \qquad a \neq 0.$$

Also, if $c$ and $d$ are multiples of $b$, then $c+d$ and $c-d$ (if $d\leq c$) are multiples of $b$, and we have

$$
\frac{c+d}{b}=\frac{c}{b}+\frac{d}{b},\qquad
\frac{c-d}{b}=\frac{c}{b}-\frac{d}{b}.
$$

The integers which are multiples of 2 are said to be *even*, and the others *odd*. By Theorem 1 the odd integers are of the form $2n+1$.

### 7. EXPANSION TO BASE $b$

#### Proposition 8 {#ens-iii-s5-prop-8 .statement tag=03M6}

*Let $b$ be an integer $>1$. For each integer $k>0$ let $E_k$ be the lexicographic product (§ 2, no. 6) of the family $(J_h)_{0\leq h\leq k-1}$ of intervals all identical with $[0,b-1]$. For each $r=(r_0,r_1,\ldots,r_{k-1})\in E_k$, let*

$$
f_k(r)=\sum_{h=0}^{k-1}r_hb^{k-h-1};
$$

*then the mapping $f_k$ is an isomorphism of the ordered set $E_k$ onto the interval $[0,b^k-1]$.*

The proof is by induction on $k$. For $k=1$ it is an immediate consequence of the definitions. For each $r=(r_0,\ldots,r_{k-1},r_k)\in E_{k+1}$ put

$$
\varphi(r)=(r_0,\ldots,r_{k-1})\in E_k.
$$

Then the mapping $r\mapsto(\varphi(r),r_k)$ is an isomorphism of $E_{k+1}$ onto the lexicographical product of $E_k$ and $J=[0,b-1]$; this is immediate from the definitions. We may write

$$
f_{k+1}(r)=b\cdot f_k(\varphi(r))+r_k;
$$

let us show that the relation $r<r'$ in $E_{k+1}$ implies $f_{k+1}(r)<f_{k+1}(r')$. Indeed, we have either $\varphi(r)<\varphi(r')$, or else $\varphi(r)=\varphi(r')$ and $r_k<r'_k$. In the first case, the inductive hypothesis implies that $f_k(\varphi(r))<f_k(\varphi(r'))$, and therefore (§ 4, no. 2, Proposition 2) $f_k(\varphi(r'))\geq f_k(\varphi(r))+1$; consequently

$$
f_{k-1}(r')\geq b\cdot f_k(\varphi(r))+b>f_{k+1}(r),
$$

since $r_k\leq b-1$ (no. 2, Proposition 3). If, on the other hand, $\varphi(r)=\varphi(r')$ and $r_k<r'_k$, it is clear that $f_{k+1}(r)<f_{k+1}(r')$. Now the inductive hypothesis shows that $f_k(\varphi(r))\leq b^k-1$, whence

$$
f_{k+1}(r)\leq b(b^k-1)+b-1=b^{k+1}-1.
$$

It follows that $f_{k+1}$ is an isomorphism of $E_{k+1}$ onto a subset of the interval $[0,b^{k+1}-1]$; but this interval and $E_{k+1}$ have the same number of

elements, namely $b^{k+1}$ (no. 3, Proposition 5); therefore $f_{k+1}$ is a bijection (§ 4, no. 2, Proposition 2, Corollary 4), and the proof is complete.
¶ We note now that for every integer $a$ we have $a < b^a$. This is proved by induction on $a$; the result is evident for $a = 0$, and the hypothesis $a < b^a$ implies $a + 1 \leqslant b^a < b \cdot b^a = b^{a+1}$ (no. 2, Proposition 3 and § 4, no. 2, Proposition 2). There is therefore a least integer $k$ such that $a < b^k$, and Proposition 8 then shows that there exists a unique finite sequence $(r_h)_{0 \leqslant h \leqslant k-1}$ such that $0 \leqslant r_h \leqslant b - 1$ for $0 \leqslant h \leqslant k - 1$ and
$$a = \sum_{h=0}^{k-1} r_h b^{k-h-1}.$$
Furthermore, we must have $r_0 > 0$, for otherwise $a < b^{k-1}$ by virtue of Proposition 8. The expression
$$\sum_{h=0}^{k-1} r_h b^{k-h-1}$$
is called the *expansion to base $b$* of the integer $a$.

\* In all parts of mathematics which do not involve numerical computations, Proposition 8 is useful mainly when applied to a *prime* number $b$. \*

When the integer $b$ is small enough for this to be practicable, we may represent each integer $< b$ by a distinctive symbol called a *digit*. The digits which represent 0 and 1 are usually 0 and 1. Let $a$ be an integer and let $\sum_{h=0}^{k-1} r_h b^{k-h-1}$ be its expansion to base $b$. If the integer $k$ which appears in this expansion is sufficiently small for this to be practicable, it is usual to associate with the integer $a$ the succession of symbols obtained by writing $r_0 r_1 \ldots r_{k-2} r_{k-1}$ from left to right and then replacing each integer $r_i$ by the digit which represents it; the symbol so obtained is called the *numerical symbol* associated with $a$. One then often replaces $a$ by its numerical symbol in the terms and relations in which it appears.

For example, if C, Q, F, D are digits, the numerical symbols CQ, CQF, CQFD are respectively associated with $\mathrm{C}b + \mathrm{Q}$, $\mathrm{C}b^2 + \mathrm{Q}b + \mathrm{F}$, $\mathrm{C}b^3 + \mathrm{Q}b^2 + \mathrm{F}b + \mathrm{D}$.

It follows from Proposition 8 that the numerical symbol associated with an integer $a$ is unique, and that if $a < b^k$ it contains at most $k$ digits. Notice that the numerical symbol associated with the integer $b^k$ consists of the digit 1 followed by $k$ digits 0.

This system of representation of integers by numerical symbols is called the *system of numeration to base $b$*. In practical numerical computations, the following systems are used : (*a*) the system to base 2, or the *dyadic system*, in which the digits are 0 and 1; (*b*) the *decimal system*, in which the

digits are $0$, $1$, $2$, $3$, $4$, $5 = 4 + 1$, $6 = 5 + 1$, $7 = 6 + 1$, $8 = 7 + 1$, $9 = 8 + 1$, and in which $b$ is the integer $9 + 1$ (whose numerical symbol in this system is therefore 10).

Since the Middle Ages the decimal system has been traditionally used in numerical calculations, and we shall use it in this series whenever we have occasion to write down an integer explicitly. We refer the reader to the part of this series devoted to numerical calculation for an account of methods for obtaining the numerical symbols associated with the sum, difference, product, and integral part of the quotient of two integers given by their numerical symbols.

### 8. COMBINATORIAL ANALYSIS

#### Proposition 9 {#ens-iii-s5-prop-9 .statement tag=03M7}

*Let* $\mathrm{E}$ *and* $\mathrm{F}$ *be two sets,* $\mathfrak{a}$ *and* $\mathfrak{b}$ *their cardinals,* $f$ *a surjection of* $\mathrm{E}$ *onto* $\mathrm{F}$ *such that the sets* $\overset{-1}{f}(y)$, *where* $y \in \mathrm{F}$, *all have the same cardinal* $\mathfrak{c}$. *Then* $\mathfrak{a} = \mathfrak{b}\mathfrak{c}$.

For the family $(\overset{-1}{f}(y))_{y \in \mathrm{F}}$ is a partition of $\mathrm{E}$, each element of which partition is a set of cardinal $\mathfrak{c}$; hence the result (§ 3, no. 4, Proposition 6, Corollary 2).

#### Definition 2 {#ens-iii-s5-def-2 .statement tag=03M8}

*Let* $n$ *be an integer.* *The product* $\prod_{i < n} (i + 1)$ *is denoted by* $n!$ (read "factorial $n$").

We have $0! = 1$ (Chapter II, § 5, no. 3) and $1! = 1$. For each integer $n$ we have $(n + 1)! = n!\,(n + 1)$. This relation, together with the relation $0! = 1$, characterizes the term $n!$, as is easily seen by induction on $n$.

#### Proposition 10 {#ens-iii-s5-prop-10 .statement tag=03M9}

*Let* $m$ *and* $n$ *be integers such that* $m \leqslant n$. *Then* $n!/(n - m)!$ *is the number of injective mappings of a set* $\mathrm{A}$ *with* $m$ *elements into a set* $\mathrm{B}$ *with* $n$ *elements.*

The proof is by induction on the number $m \leqslant n$ of elements of $\mathrm{A}$. If $m = 0$, the result is evident. Suppose that $m + 1 \leqslant n$. Let $\mathrm{A}$ be a set with $m + 1$ elements, let $\mathrm{A}'$ be a subset of $\mathrm{A}$ with $m$ elements, and let $\{a\} = \mathrm{A} - \mathrm{A}'$. Let $\mathrm{F}$, $\mathrm{F}'$ be the sets of injective mappings of $\mathrm{A}$, $\mathrm{A}'$ respectively into $\mathrm{B}$, and let $\varphi$ be the mapping $f \to f\,|\mathrm{A}'$ which maps each function $f \in \mathrm{F}$ to its restriction to $\mathrm{A}'$. For each $f' \in \mathrm{F}'$ an element $f$ of $\overset{-1}{\varphi}(f')$ is uniquely determined by its value $f(a)$; since $f$ is injective, we must have $f(a) \in \mathrm{B} - f'(\mathrm{A}')$. It follows that $\overset{-1}{\varphi}(f')$ has the same number $n - m$ of elements as $\mathrm{B} - f'(\mathrm{A}')$. Hence, by Proposition 9, $\mathrm{F}$ has

$$(n - m)\,\frac{n!}{(n - m)!} = \frac{n!}{(n - m - 1)!}$$

elements by virtue of the inductive hypothesis. This completes the proof.

#### Corollary {#ens-iii-s5-n8-cor-1 .statement tag=03MA}

*The number of permutations of a finite set with n elements is equal to n!.*

For this number is equal to the number of injections of the set into itself (§ 4, no. 2, Proposition 2, Corollary 4).

#### Proposition 11 {#ens-iii-s5-prop-11 .statement tag=03MB}

*Let* E *be a finite set with n elements, and let* $(p_i)_{1 \leqslant i \leqslant h}$ *be a finite sequence of integers such that* $\sum_{i=1}^{h} p_i = n$. *Then the number of coverings* $(X_i)_{1 \leqslant i \leqslant h}$ *of* E *by mutually disjoint sets* $X_i$ *such that* $\mathrm{Card}\,(X_i) = p_i$ *for* $1 \leqslant i \leqslant h$ *is equal to*

$$n! \Big/ \prod_{i=1}^{h} p_i!.$$

Let G be the set of permutations of E and let P be the set of coverings $(X_i)_{1 \leqslant i \leqslant h}$ which satisfy the conditions of the Proposition. Since $\sum_{i=1}^{h} p_i = n$, P is not empty. Let $(A_i)_{1 \leqslant i \leqslant h}$ be an element of P. For each permutation $f \in G$ the family $(f(A_i))_{1 \leqslant i \leqslant h}$ again belongs to P; let us denote it by $\varphi(f)$. For each element $(X_i)_{1 \leqslant i \leqslant h}$ let us calculate the number of permutations $f \in G$ such that $\varphi(f) = (X_i)$. We shall have $\varphi(f) = (X_i)$ if and only if for each index $i$ we have $f(A_i) = X_i$. Hence the set of permutations $f$ under consideration is equipotent to the product of the sets of bijections of $A_i$ onto $X_i$ (Chapter II, § 4, no. 7, Proposition 8); consequently the set $\overset{-1}{\varphi}((X_i)_{1 \leqslant i \leqslant h})$ has $\prod_{i=1}^{h} p_i!$ elements (Corollary to Proposition 10). Since G has $n!$ elements, the result now follows from Proposition 9.

#### Corollary 1 {#ens-iii-s5-prop-11-cor-1 .statement tag=03MC}

*Let* A *be a set with n elements and let p be an integer* $\leqslant n$. *Then the number of subsets of* A *which have p elements is* $\dfrac{n!}{p!(n-p)!}$.

Put $h = 2$, $p_1 = p$, $p_2 = n - p$ in Proposition 11.

¶ The number of subsets containing $p$ elements in a set of $n$ elements (where $p \leqslant n$) is denoted by $\begin{pmatrix} n \\ p \end{pmatrix}$ and is called the *binomial coefficient with indices n and p*. From the relation $\begin{pmatrix} n \\ p \end{pmatrix} = \dfrac{n!}{p!(n-p)!}$ it follows immediately that $\begin{pmatrix} n \\ p \end{pmatrix} = \begin{pmatrix} n \\ n-p \end{pmatrix}$.

This is also a consequence of the fact that, if E is a set with $n$ elements, $X \to E - X$ is a bijection of the set of subsets of E consisting of $p$ elements onto the set of subsets of $n - p$ elements.

We put $\binom{n}{p} = 0$ for each pair of natural integers such that $p > n$. With this convention the number of subsets of $p$ elements in a set of $n$ elements is $\binom{n}{p}$ for *every* natural integer $p$.

#### Corollary 2 {#ens-iii-s5-prop-11-cor-2 .statement tag=03RG}

*Let* E *and* F *be totally ordered finite sets with* $p$ *and* $n$ *elements, respectively. Then the number of strictly increasing mappings of* E *into* F *is* $\binom{n}{p}$.

For such a mapping is an injection of E into F (§ 1, no. 12, Proposition 11), and since E and F are well-ordered (§ 4, no. 4, Corollary 1 to Proposition 3), for each subset X of $p$ elements of F there is exactly one strictly increasing mapping of E onto X (§ 2, no. 5, Theorem 3).

#### Proposition 12 {#ens-iii-s5-prop-12 .statement tag=03RH}

*For each integer* $n$, *we have*

$$\sum_p \binom{n}{p} = 2^n.$$

For if E is a set of $n$ elements, the left-hand side of the equality is the number of subsets of E. Now apply Proposition 12 of § 3, no. 5.

#### Proposition 13 {#ens-iii-s5-prop-13 .statement tag=03RI}

*If* $n$ *and* $p$ *are integers, then*

$$\binom{n+1}{p+1} = \binom{n}{p+1} + \binom{n}{p}.$$

Let E be a set with $n + 1$ elements, let P be the set of all subsets of E containing $p + 1$ elements, let $a$ be an element of E, and put

$$\mathrm{E}' = \mathrm{E} - \{a\}.$$

Let P′ (resp. P″) denote the set of subsets of $p + 1$ elements of E which contain $a$ (resp. do not contain $a$). The set P″ is the set of subsets of $p + 1$ elements of E′ and therefore has $\binom{n}{p+1}$ elements. The mapping $\mathrm{X} \to \mathrm{X} \cap \mathrm{E}'$ is a bijection of P′ onto the set of subsets of $p$ elements of E′, and P′ therefore has $\binom{n}{p}$ elements. The result now follows from the fact that P is the union of the disjoint sets P′ and P″.

Proposition 13 can also be proved by means of a simple calculation from the formula $\binom{n}{p} = \dfrac{n!}{p!(n-p)!}$ for $p \leqslant n$.

#### Proposition 14 {#ens-iii-s5-prop-14 .statement tag=03RJ}

*Let* $n$ *be an integer* $> 0$. *Then the number* $a_n$ (resp. $b_n$) *of ordered pairs* $(i, j)$ *of integers such that* $1 \leqslant i \leqslant j \leqslant n$ (resp. $1 \leqslant i < j \leqslant n$) *is* $\frac{1}{2}n(n+1)$ ((resp. $\frac{1}{2}n(n-1)$)).

For $b_n$ is the number of subsets of 2 elements in $[1, n]$; hence

$$b_n = \frac{n!}{2!(n-2)!} = \frac{1}{2} n(n-1).$$

The value of $a_n$ is deduced from this by noting that the set of ordered pairs $(i, j)$ such that $1 \leqslant i \leqslant j \leqslant n$ is the union of the set of ordered pairs $(i, j)$ such that $1 \leqslant i \leqslant j < n$ and the set of pairs $(i, i)$ where $1 \leqslant i \leqslant n$. Thus $a_n = n + b_n = \frac{1}{2} n(n+1)$.

#### Corollary {#ens-iii-s5-n8-cor-2 .statement tag=03RK}

*For each integer $n > 0$, we have*

$$\sum_{i=1}^{n} i = \frac{1}{2} n(n+1).$$

In the set A of ordered pairs of integers $(i, j)$ such that $1 \leqslant i \leqslant j \leqslant n$, let $A_k$ denote the subset of pairs $(i, k)$, where $1 \leqslant i \leqslant k$ (for an arbitrary integer $k \leqslant n$). Then $A_k$ has $k$ elements. But $(A_k)_{1 \leqslant k \leqslant n}$ is a partition of A; hence the result.

#### Proposition 15 {#ens-iii-s5-prop-15 .statement tag=03RL}

*Let $n$ and $h$ be integers and let* E *be a set with $h$ elements. Then the number of mappings $u$ of* E *into* $[0, n]$ *such that* $\sum_{x \in E} u(x) \leqslant n$ *(resp.* $\sum_{x \in E} u(x) = n$, *for $h > 0$) is*

$$\binom{n+h}{h} \left( \text{resp.} \ \binom{n+h-1}{h-1} \right).$$

Let $A(h, n)$ (resp. $B(h, n)$) denote the number of mappings $u$ of E into $[0, n]$ such that $\sum_{x \in E} u(x) \leqslant n$ (resp. $\sum_{x \in E} u(x) = n$ for $h > 0$). We show first that $A(h-1, n) = B(h, n)$. For this, let E′ be a subset of E with $h - 1$ elements, and let $\{a\} = E - E'$. If $u$ is a mapping of E into $[0, n]$ such that $\sum_{x \in E} u(x) = n$, then its restriction $u'$ to E′ is such that $\sum_{x \in E'} u'(x) \leqslant n$, and moreover $u(a) = n - \sum_{x \in E'} u'(x)$. Conversely, every mapping $u'$ of E′ into $[0, n]$ which satisfies $\sum_{x \in E'} u'(x) \leqslant n$ defines a unique mapping $u$ of E into $[0, n]$, of which $u'$ is the restriction, and which is such that $\sum_{x \ni E} u(x) = n$.

We note next that if $\sum_{x \in E} u(x) \leqslant n$, then either $\sum_{x \in E} u(x) = n$, or else $\sum_{x \in E} u(x) \leqslant n-1$, and these two possibilities are mutually exclusive. Consequently

$$A(h, n) = A(h, n-1) + B(h, n) = A(h, n-1) + A(h-1, n).$$

Since $A(0, 0) = 1 = \binom{0}{0}$, the formula $A(h, n) = \binom{n+h}{h}$ follows from above and from Proposition 13, by induction on $n + h$.

\* The number of monomials $X_1^{\alpha_1} X_2^{\alpha_2} \ldots X_h^{\alpha_n}$ in $h$ indeterminates with total degree $\leqslant n$ is evidently equal to the number of mappings $i \rightarrow \alpha_i$ of $[1, h]$ into $[0, n]$ such that $\sum_{i=0}^{h} \alpha_i \leqslant n$, and is therefore equal to $\binom{n+h}{h}$ by Proposition 15; this number is also the number of monomials in $h + 1$ indeterminates with total degree $n$. \*

### Exercises {#ens-iii-s5-exercises}

See the [exercises for § 5](exercises/s5/).
