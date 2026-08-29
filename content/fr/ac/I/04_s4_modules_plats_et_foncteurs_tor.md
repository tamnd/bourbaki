---
book: ac
book_title: Commutative Algebra
chapter: I
chapter_title: Modules plats
section: 4
section_title: Modules plats et foncteurs « Tor »
lang: fr
source: ac-i-iv-fr
pdf_pages: 0053-0055, 0066-0066
extraction: ocr
statements: 3
exercises: 1
content_sha256: 6e0fb424cf57e891b3031ba428b07482d1d4a83c9d44a019ddc74d688deaf442
---

## § 4. Modules plats et foncteurs « Tor »

A l’usage des lecteurs au courant de l’Algèbre homologique (*), nous allons indiquer rapidement comment la théorie des modules plats se relie à celle des foncteurs Tor.

#### Proposition 1 {#ac-i-s4-prop-1 .statement}

Soit E un A-module à droite. Les quatre propriétés suivantes sont équivalentes :

(*) Voir la partie de ce Traité consacrée aux catégories, et, plus particulièrement, aux catégories abéliennes (en préparation). En attendant la parution de cette partie, le lecteur pourra consulter H. CARTAN-S. EILENBERG, Homological Algebra, Princeton, 1956, ou R. GODEMENT, Théorie des Faisceaux, Paris (Hermann), 1958.

a) $E$ est plat.

b) *Pour tout* $A$-module à gauche $F$ *et tout entier* $n \geqslant 1$, *on a* $\operatorname{Tor}_n^A(E, F) = 0$.

c) *Pour tout* $A$-module à gauche $F$, *on a* $\operatorname{Tor}_1^A(E, F) = 0$.

d) *Pour tout idéal à gauche de type fini* $a$ *de* $A$, *on a*
$$
\operatorname{Tor}_1^A(E, A_s/a) = 0.
$$

Montrons que a) implique b). Soit
$$
\cdots \to L_n \to L_{n-1} \to \cdots \to L_0 \to F \to 0
$$
une résolution libre de $F$. Comme $E$ est plat, la suite
$$(1)$$ $$
\cdots \to E \otimes L_n \to E \otimes L_{n-1} \to \cdots \to E \otimes L_0 \to E \otimes F \to 0
$$
est exacte. Comme les $\operatorname{Tor}_n^A(E, F)$ sont isomorphes aux groupes d’homologie du complexe (1), ils sont nuls pour $n \geqslant 1$.

Il est trivial que b) entraîne c) et que c) entraîne d). Montrons enfin que d) implique a). La suite exacte
$$
0 \to a \to A_s \to A_s/a \to 0
$$
donne la suite exacte
$$
\operatorname{Tor}_1^A(E, A_s/a) \to E \otimes_A a \to E \otimes_A A.
$$
Comme d) est vérifiée, l’homomorphisme canonique
$$
E \otimes_A a \to E \otimes_A A = E
$$
est injectif, ce qui signifie que $E$ est plat ($§ 2$, no 3, prop. 1).

La prop. 1 fournit une caractérisation des modules plats qui est souvent utile dans les applications. Nous nous bornerons, à titre d’exemple, à donner une nouvelle démonstration de la prop. 5 du $§ 2$, no 5. Si $E'$ et $E''$ sont plats, la suite exacte
$$
\operatorname{Tor}_1^A(E', F) \to \operatorname{Tor}_1^A(E, F) \to \operatorname{Tor}_1^A(E'', F)
$$
montre que $\operatorname{Tor}_1^A(E, F) = 0$ pour tout $A$-module à gauche $F$, donc $E$ est plat. Si $E$ et $E''$ sont plats, la suite exacte
$$
\operatorname{Tor}_2^A(E'', F) \to \operatorname{Tor}_1^A(E', F) \to \operatorname{Tor}_1^A(E, F)
$$
montre que $\operatorname{Tor}_1^A(E', F) = 0$, donc $E'$ est plat.

#### Proposition 2 {#ac-i-s4-prop-2 .statement}

Soient R, S deux anneaux, $\rho : R \to S$ un homomorphisme et F un R-module à gauche. Les deux propriétés suivantes sont équivalentes :

a) On a $\mathrm{Tor}_1^R(\rho_*(E), F) = 0$ pour tout S-module à droite E.
b) Le S-module à gauche $\rho^*(F) = F_{(s)} = S \otimes_R F$ est plat, et on a $\mathrm{Tor}_1^R(\rho_*(S_d), F) = 0$.

Supposons a) vérifiée. Prenant $E = S_d$, on voit que $\mathrm{Tor}_1^R(\rho_*(S_d), F) = 0$. Montrons en outre que $F_{(s)}$ est un S-module plat. Pour cela, notons que si E est un S-module à droite, le groupe additif $E \otimes_S F_{(s)}$ s’identifie à $\rho_*(E) \otimes_R F$. Si l’on a donc une suite exacte de S-modules à droite

$$
0 \to E' \to E \to E'' \to 0
$$

on en déduit, vu a), une suite exacte

$$
0 \to \rho_*(E') \otimes_R F \to \rho_*(E) \otimes_R F \to \rho_*(E'') \otimes_R F \to 0
$$

ou encore

$$
0 \to E' \otimes_S F_{(s)} \to E \otimes_S F_{(s)} \to E'' \otimes_S F_{(s)} \to 0
$$

ce qui prouve que $F_{(s)}$ est plat.

Réciproquement, si b) est vérifiée, on a tout d’abord, pour tout S-module à droite libre $L = S_d^{(i)}$, $\mathrm{Tor}_1^R(\rho_*(L), F) = (\mathrm{Tor}_1^R(\rho_*(S_d), F))^{(i)} = 0$. Tout S-module à droite E s’écrit sous la forme $E = L/H$ pour un S-module libre L convenable ; on a donc la suite exacte

(2) $0 = \mathrm{Tor}_1^R(\rho_*(L), F) \to \mathrm{Tor}_1^R(\rho_*(E), F) \to \rho_*(H) \otimes_R F \to \rho_*(L) \otimes_R F.$

Mais comme $F_{(s)}$ est plat, l’homomorphisme $H \otimes_S F_{(s)} \to L \otimes_S F_{(s)}$ est injectif, et il s’identifie à l’homomorphisme

$$
\rho_*(H) \otimes_R F \to \rho_*(L) \otimes_R F.
$$

On déduit alors de (2) que $\mathrm{Tor}_1^R(\rho_*(E), F) = 0$.

#### Remarque {#ac-i-s4-n0-rem-1 .statement}

La proposition 2 découle aussi de l’existence de la suite exacte

$$
E \otimes_S \mathrm{Tor}_1^R(\rho_*(S_d), F) \to \mathrm{Tor}_1^R(\rho_*(E), F) \to \mathrm{Tor}_1^S(E, S_d \otimes_R F) \to 0
$$

provenant de la suite spectrale d’« associativité » des foncteurs Tor.

## EXERCICES {#ac-i-s4-exercises}

See the [exercises for § 4](exercises/s4/).
