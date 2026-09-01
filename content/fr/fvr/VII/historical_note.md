---
book: fvr
book_title: Functions of a Real Variable
chapter: VII
chapter_title: LA FONCTION GAMMA
section: 0
section_title: Historical Note
kind: historical
lang: fr
source: fvr-i-vii-fr
book_pages: A V.113-FVR VII.38
pdf_pages: 0314-0329
extraction: ocr
statements: 0
exercises: 0
content_sha256: a47d34244ba744bcccf40a574d91dd116d6ea0c78743ccf0c06d4ab99b65d4c4
---

# NOTE HISTORIQUE

(N.-B. — Les chiffres romains renvoient à la bibliographie placée à la fin de cette note.)

L’idée d’« interpoler » une suite $(u_n)$ par les valeurs d’une intégrale dépendant d’un paramètre réel $\lambda$ et égale à $u_n$ pour $\lambda = n$, remonte à Wallis (III, p. 55). C’est cette idée qui guide principalement Euler lorsque, en 1730 ((I), t. XIV, p. 1–24), il se propose d’interpoler la suite des factorielles. Il commence par remarquer que $n!$ est égal au produit infini $\prod_{k=1}^{\infty} \left( \frac{k+1}{k} \right)^n \frac{k}{k+n}$, que ce produit est défini pour toute valeur de $n$ (entière ou non), et qu’en particulier, pour $n = \frac{1}{2}$, il prend la valeur $\frac{1}{2} \sqrt{\pi}$ d’après la formule de Wallis. L’analogie de ce résultat avec ceux de Wallis le conduit alors à reprendre l’intégrale

$$
\int_0^1 x^e (1-x)^n \, dx
$$

$(n$ entier, $e$ quelconque), déjà considérée par ce dernier. Euler en obtient la valeur $\frac{n!}{(e+1)(e+2)\ldots(e+n)}$ par le développement du binôme; un changement de variables lui montre alors que $n!$ est la limite, pour $z$ tendant vers 0, de l’intégrale $\int_0^1 \left( \frac{1-x^z}{z} \right)^n \, dx$, d’où la « seconde intégrale eulérienne »

$$
n! = \int_0^1 \left( \log \frac{1}{x} \right)^n \, dx;
$$

par la même méthode, et l’usage de la formule de Wallis, il obtient la formule $\int_0^1 \sqrt{\log 1/x} \, dx = \frac{1}{2} \sqrt{\pi}$. Dans ses travaux ultérieurs, Euler revient fréquemment à ces intégrales; il découvre ainsi la relation des compléments ((I), t. XV, p. 82 et t. XVII, p. 342), la formule $B(p, q) = \Gamma(p) \Gamma(q)/\Gamma(p+q)$ ((I), t. XVII, p. 355), et le cas particulier de la formule de Legendre-Gauss correspondant à $x = 1$ ((I), t. XIX, p. 483); le tout bien entendu sans l’inquiéter de questions de convergence.

Gauss poursuit l’étude de la fonction $\Gamma$ à l’occasion de ses recherches sur la fonction hypergéométrique, dont la fonction $\Gamma$ est un cas limite (II); c’est au cours de ces recherches qu’il obtient la formule générale de multiplication (déjà remarquée par Legendre peu auparavant pour $p = 2$). Les travaux ultérieurs sur $\Gamma$ ont surtout porté sur le prolongement de cette fonction au domaine complexe. Ce n’est que récemment que l’on s’est aperçu que la propriété de convexité logarithmique caractérisait $\Gamma(x)$ (dans le domaine réel) à un facteur près parmi toutes les solutions de l’équation fonctionnelle $f(x + 1) = x f(x)$ (III); et Artin a montré (IV) comment on peut rattacher simplement tous les résultats classiques sur $\Gamma(x)$ à cette propriété. Nous avons suivi d’assez près son exposé

(I) L. Euler, Opera omnia, Leipzig-Berlin (Teubner): t. XIV (1924), t. XV (1927), t. XVII (1915) et t. XIX (1932).
(II) C. F. Gauss, Werke, t. III, Göttingen, 1866.
(III) H. Bohr und J. Mollerup, Laerebog i matematisk Analyse, t. III, Kopenhagen, 1922, p. 149–164.
(IV) E. Artin, Einführung in die Theorie der Gammafunktion, Leipzig (Teubner), 1931.

f'(x_0), f'_d(x_0), f'_g(x_0), Df(x_0): I, p. 12
f', f_d, f_g, Df, df/dx: I, p. 13
D^n f(x_0), f^{(n)}(x_0): I, p. 28
D^n f, f^{(n)}: I, p. 28
\int_{x_0}^x f(t)dt, \int_{x_0}^x f : II, p. 8
\int_{x_0}^x f(t)dt, \int_{x_0}^x f : II, p. 8
h(t) \frac{d}{dx}: II, p. 9
f^{(n)}: II, p. 13
\int_I f(t)\ dt: II, p. 15
e, exp x (x réel): III, p. 2
log x (x réel > 0): III, p. 2
\pi: III, p. 4
cos x, sin x (x réel): III, p. 5
tg x, cotg x, sec x, cosec x: III, p. 5
Arc sin x, Arc cos x, Arc tg x: III, p. 5
e^z, exp (z) (z complexe): III, p. 7
log z (z complexe non situé sur le demi-axe réel négatif): III, p. 10
cos z, sin z, tg z, cotg z (z complexe): III, p. 12
ch x, sh x, th x: III, p. 12
Arg sh x, Arg ch x, Arg th x: III, p. 13
\binom{m}{n} (m réel, n entier \geqslant 0): III, p. 18
e^A, cexp A (A endomorphisme continu d’un espace normé): IV, p. 27
\mathcal{H}(\mathfrak{F}, V), R_\infty, \mathcal{H}_\infty(\mathfrak{F}, V): V, p. 2
f + g, f\lambda, \|f\|, fg (f, g fonctions de \mathcal{H}(\mathfrak{F}, V)): V, p. 3
f \leqslant g, g \geqslant f (f et g fonctions numériques \geqslant 0): V, pl 3
f_1 \leqslant f_2, f_2 \geqslant f_1 (f_1 fonction de \mathcal{H}(\mathfrak{F}, V_1), f_2 fonction de \mathcal{H}(\mathfrak{F}, V_2)): V, p. 3
f \asymp g: V, p. 3
f \ll g, g \gg f (f et g fonctions numériques \geqslant 0): V, p. 5
f_1 \ll f_2, f_2 \gg f_1 (f_1 fonction de \mathcal{H}(\mathfrak{F}, V_1), f_2 fonction de \mathcal{H}(\mathfrak{F}, V_2)): V, p. 5
f \sim g: V, p. 6
O(f), O_k(f), o(f), o_k(f): V, p. 9
l_0x, l_nx: V, p. 19
\mathfrak{R}(y) (\mathfrak{R} corps de Hardy): V, p. 38
e_0(x), e_n(x): V, p. 41
\sum_{k=0}^\infty a_k D^k: VI, p. 4
B_n(x): VI, p. 7
b_n: VI, p. 7
U_x^z (f(\xi)): VI, p. 9
\Gamma(x) (x réel): VII, p. 7
B(x, y): VII, p. 8
\Gamma(z) (z complexe): VII, p. 10.

Absolument convergente (intégrale —): II, p. 18
Accroissements finis (théorème des —): I, p. 23
Adjonction à un corps différentiel d’une racine d’un polynôme, d’une primitive, d’une exponentielle de primitive: III, p. 28, exerc 25.
Adjointe (équation —) d’une équation différentielle linéaire: IV, p. 25
Appell (polynômes d' —): VI, p. 5
Approchée (solution —) à e près d’une équation différentielle: IV, p. 4
Asymptotique (développement —): voir Développement asymptotique
Au-dessous (point —) d’un graphe: I, p. 32
Au-dessus (point —) d’un graphe: I, p. 32

Bernoulli (nombres de —): VI, p. 7
Bernoulli (polynômes de —): VI, p. 7
Binôme (formule du —, série du —): III, p. 18

Caractère local (relation de —): V, p. 2
Caractéristiques (racines —) d’une équation différentielle linéaire à coefficients constants: IV, p. 30
Cauchy (critère de —) pour les intégrales: II, p. 16
Cauchy (critère de convergence de —): V, p. 28
Cauchy (théorème de —): IV, p. 10
Cauchy–Maclaurin (critère de convergence de —): V, p. 27
Changement de variables (formule de —): II, p. 11
Coefficients d’un développement asymptotique: V, p. 12 et p. 17
Coefficients binomiaux: III, p. 18
Comparables (fonctions —): V, p. 7
Comparables d’ordre k (fonctions —): V, p. 22
Comparaison (échelle de —): V, p. 10
Compléments (relation des —): VII, p. 12
Concave (fonction —): I, p. 35
Condition de Lipschitz: IV, p. 7
Congruences de Kummer: VI, p. 25, exerc. 9
Constante d’Euler: V, p. 32
Convergente (intégrale —): II, p. 14
Convexe (fonction —): I, p. 32
Corps de Hardy: V, p. 36
Corps différentiel: III, p. 28, exerc. 25
Cosécante: III, p. 5
Cosinus d’un nombre complexe: III, p. 12
Cosinus hyperbolique: III, p. 12
Critère de Cauchy pour les intégrales: II, p. 16
Critère de convergence de Cauchy: V, p. 28
Critère de convergence de Cauchy–Maclaurin: V, p. 27
Critère de convergence de d’Alembert: V, p. 35
Critère de convergence d’Ermakoff: II, p. 34, exerc. 8
Critère de convergence de Raabe: V, p. 34
Critères de convergence de seconde espèce: V, p. 34
Critères-de-convergence logarithmiques pour les intégrales: V, p. 19

Critères de convergence logarithmiques pour les séries: V, p. 28

D’Alembert (critère de convergence de —): V, p. 35
Demi-tangente à droite, demi-tangente à gauche: I, p. 19
Déivable (fonction —) en un point: I, p. 11
Déivable (fonction —) dans un intervalle: I, p. 12
Déivable à droite, à gauche (fonction —) en un point: I, p. 12
Déivable à droite, à gauche (fonction —) dans un intervalle: I, p. 12
Déivable (fonction n fois —) en un point: I, p. 28
Déivable (fonction n fois —) dans intervalle: I, p. 28.
Dérivée d’une fonction: I, p. 11
Dérivée à droite, dérivée à gauche: I, p. 12
Dérivée infinie: I, p. 18
Dérivée logarithmique: III, p. 4
Dérivée n-ème: I, p. 28.
Dérivée première: I, p. 11.
Dérivée seconde: I, p. 28
Dérivée symétrique: I, p. 45, exerc. 13
Déterminant de n intégrales d’un système de n équations différentielles linéaires: IV, p. 23
Détermination principale du logarithme d’un nombre complexe: III, p. 10
Développement asymptotique d’une fonction par rapport à une échelle de comparaison: V, p. 12
Développement asymptotique à la précision gα: V, p. 12
Développement asymptotique plus précis qu’un autre: V, p. 13
Développement asymptotique réduit à la précision gβ: V, p. 13
Développement asymptotique à coefficients variables: V, p. 17
Développement de Stirling de log Γ(z): VII, p. 15
Développement de Taylor d’ordre n: I, p. 30
Développement eulérien de cotg z: VI, p. 15
Développement eulérien de sin z: VI, p. 17
Développement taylorien généralisé d’un polynôme: VI, p. 6.
Développement taylorien généralisé d’une fonction: VI, p. 10
Dominée (fonction —) par une autre: V, p. 3
Droite asymptote à un graphe: I, p. 51, exerc. 7
Droite d’appui du graphe d’une fonction convexe: I, p. 37
Droite localement au-dessous, localement au-dessus d’un graphe: I, p. 39
Droite localement sur un graphe: I, p. 39

Echelle de comparaison: V, p. 10
Equation différentielle à variable réelle: IV, p. 1
Equation différentielle adjointe: IV, p. 25
Equation différentielle d’ordre n: IV, p. 2
Equation différentielle du premier ordre: IV, p. 2
Equation différentielle linéaire: IV, p. 16
Equation différentielle linéaire homogène: IV, p. 2
Equation différentielle linéaire d’ordre n: IV, p. 30
Equation différentielle lipschitzienne: IV, p. 10 .
Equation différentielle localement lipschitzienne: IV, p. 10
Equation différentielle scalaire: IV, p. 2 et p. 30
Équivalentes (fonctions —): V, p. 6
Escalier (fonction en —): II, p. 4
Euler (constante d') —: V, p. 32
Euler (formules d') —: III, p. 9
Euler–Maclaurin (formule sommatoire d') —: VI, p. 14
Eulérien (développement —) de cotg z: VI, p. 15

Eulérien (développement —) de sin z: VI, p. 17
Eulériennes (intégrales —): VII, p. 6
Exponentielle complexe: III, p. 7
Exponentielles itérées: V, p. 41
Extension élémentaire d’un corps différentiel: III, p. 29, exerc. 28
Extension (H) d’un corps de Hardy: V, p. 41

Faiblement comparables (fonctions —): V, p. 4
Fonction à variation bornée: II, p. 29, exerc. 5
Fonction concave, fonction convexe: I, p. 34
Fonction croissante à droite: I, p. 43, exerc. 1
Fonction dérivable: I, p. 12
Fonction dérivable à droite, dérivable à gauche: I, p. 12
Fonction dérivée: I, p. 13
Fonction dominée par une autre: V, p. 3
Fonction élémentaire: III, p. 29, exerc. 28
Fonction en escalier: II, p. 4
Fonction (H): V, p. 41
Fonction indéfiniment dérivable: I, p. 28
Fonction lipschitzienne: IV, p. 7
Fonction localement lipschitzienne: IV, p. 10
Fonction logarithmiquement bornée: V, p. 4
Fonction logarithmiquement convexe: VII, p. 6
Fonction négligeable devant une autre: V, p. 5
Fonction n fois dérivable: I, p. 28
Fonction prépondérante sur une autre: V, p. 5
Fonction réglée: II, p. 4
Fonction réglée par morceaux: II, p. 13
Fonction régulièrement convexe: V, p. 49, exerc. 5
Fonction strictement concave, strictement convexe : I, p. 34
Fonction suradditive: I, p. 54, exerc. 25
Fonctions comparables: V, p. 7
Fonctions comparables d’ordre k: V, p. 22
Fonctions équivalentes: V, p. 16
Fonctions faiblement comparables: V, p. 4
Fonctions fortement comparables: V, p. 7
Fonctions semblables: V, p. 4
Fondamental (système —) d’intégrales d’un système d’équations différentielles linéaires: IV, p. 21
Formule de Gauss: VII, p. 3
Formule de Leibniz: I, p. 28
Formule de multiplication de Legendre-Gauss: VII, p. 12
Formule de Stirling: V, p. 33
Formule de Taylor: I, p. 29
Formule de Wallis: III, p. 31, exerc. 32
Formule de Weierstrass: VII, p. 3
Formule d’intégration par parties: II, p. 10
Formule d’intégration par parties d’ordre n: II, p. 10
Formule du changement de variables: II, p. 11
Formule sommatoire d’Euler–Maclaurin: VI, p. 14
Formules d’Euler: III, p. 9
Fortement comparables (fonctions —): V, p. 7

Gauss (formule de —): VII, p. 3
Gauss (intégrale de —): VII, p. 10

(H) (extension —): V, p. 41
(H) (fonction —): V, p. 41
Hardy (corps de —): V, p. 36
Hermite (polynômes d'—): VI, p. 13
Homogène (équation différentielle linéaire —): IV, p. 17
Hyperboliques (fonctions —): III, p. 12

Identité de Redheffer: II, p. 37, exerc. 10
Indéfiniment dérivable (fonction —): I, p. 28
Indicatrice d’un opérateur de composition: VI, p. 10
Inégalité de Carleman: III, p. 25, exerc. 9
Inégalité de Carlson: III, p. 24, exerc. 4
Inégalité de Cauchy–Buniakowsky–Schwarz: III, p. 24, exerc. 3
Inégalité de Hadamard: III, p. 26, exerc. 12
Inégalité de Hardy: III, p. 26, exerc. 10
Inégalité de Hardy–Littlewood: II, p. 38, exerc. 10
Inégalité de Hlawka: II, p. 38, exerc. 10
Inégalité de Hölder: III, p. 23, exerc. 3
Inégalité d’Opial: II, p. 38, exerc. 10
Inégalité de H. Weyl: II, p. 38, exerc. 10
Intégrale absolument convergente: II, p. 18
Intégrale convergente: II, p. 18
Intégrale de Gauss: VII, p. 10
Intégrale de Raabe: VII, p. 14
Intégrale d’une équation différentielle: IV, p. 2
Intégrale d’une fonction réglée dans un intervalle compact: II, p. 13
Intégrale d’une fonction réglée par morceaux: II, p. 14
Intégrale normalement convergente: II, p. 23
Intégrale uniformément convergente: II, p. 21
Intégrales eulériennes: VII, p. 6
Intégration par parties (formule d'—): II, p. 10
Intégration par parties d’ordre n (formule d'—): II p. 10
Itérées (exponentielles —): V, p. 41
Itérés (logarithmes —): V, p. 19

Legendre–Gauss (formule de multiplication de —): VII, p. 12
Leibniz (formule de —): I, p. 28
Linéaire (équation différentielle —): IV, p. 16
Linéaire homogène (équation différentielle —): IV, p. 16
Linéaire d’ordre n (équation différentielle —): IV, p. 30
Lipschitz (condition de —): IV, p. 7
Lipschitzienne (équation différentielle —): IV, p. 10
Lipschitzienne (fonction —): IV, p. 7
Localement au-dessous, localement au-dessus d’un graphe (droite —): I, p. 39
Localement lipschitzienne (équation différentielle —): IV, p. 10
Localement lipschitzienne (fonction —): IV, p. 10
Localement sur un graphe (droite —): I, p. 39
Logarithme d’un nombre complexe (dénomination principale du —): III, p. 10
Logarithme naturel: III, p. 2
Logarithme népérien: III, p. 2
Logarithmes itérés: V, p. 19
Logarithmique (dérivée —): III, p. 4
Logarithmiques (critères de convergence —): V, p. 19
Logarithmiquement bornée (fonction —): V, p. 4
Logarithmiquement convexe (fonction —): VII, p. 6

Maximum relatif, maximum relatif strict: I, p. 19
Méthode de variation des constantes: IV, p. 20
Minimum relatif, minimum relatif strict: I, p. 19
Moyenne arithmétique ordinaire, moyenne arithmétique pondérée: III, p. 3
Moyenne géométrique ordinaire, moyenne géométrique pondérée: III, p. 3
Moyenne (théorème de la —): II, p. 11
Moyenne (valeur —) d’une fonction: II, p. 8

Naturel (logarithme —): III, p. 2
Négligeable (fonction —) devant une autre: V, p. 5
Népérien (logarithme —): III, p. 2
Nombre premier régulier, nombre premier irrégulier: VI, p. 25, exerc. 11
Nombres de Bernoulli: VI, p. 7
Normalement convergente (intégrale —): II, p. 23

Opérateur de composition: VI, p. 1, et p. 9
Opérateur de composition régulier: VI, p. 11
Opérateur de translation: VI, p. 2 et p. 9
Ordre d’un opérateur de composition: VI, p. 5
Ordre d’une fonction par rapport à une autre: V, p. 8

Partie principale d’une fonction relative à une échelle de comparaison: V, p. 11
Partie principale d’une fonction relative à une échelle de comparaison et à un domaine de coefficients: V, p. 17
Peano (théorème de —): IV, p. 6
Plus précis (développement asymptotique —) qu’un autre: V, p. 13
Polygone de Newton: V, p. 48, exerc. 3
Polynômes d’Appell: VI, p. 5
Polynômes de Bernoulli: VI, p. 7
Polynômes d’Hermite: VI, p. 13
Précision d’un développement asymptotique: V, p. 12
Prépondérante (fonction —) sur une autre: V, p. 5
Primitive d’une fonction dans un intervalle de $\mathbf{R}$: II, p. 1
Primitive d’ordre $n$: II, p. 13
Primitive seconde: II, p. 12
Primitive stricte: II, p. 2
Principe de comparaison des intégrales: II, p. 17

Raabe (critère de —): V, p. 34
Raabe (intégrale de —): VII, p. 14
Racines caractéristiques d’une équation différentielle linéaire à coefficients constants: IV, p. 30
Réduit à la précision $g_\beta$ (développement asymptotique —): V, p. 13
Réglée (fonction —): II, p. 4
Réglée par morceaux (fonction —): II, p. 13
Régulier (opérateur de composition —): VI, p. 11
Relation de caractère local: V, p. 2
Relation des compléments: VII, p. 12
Résolvante d’une équation différentielle linéaire: IV, p. 19
Reste de la formule de Taylor: I, p. 30 et II, p. 12
Reste de la formule sommatoire d’Euler–Maclaurin: VI, p. 14 et p. 19
Reste d’un développement asymptotique: V, p. 12
Rolle (théorème de —): I, p. 20

Scalaire (équation différentielle —): IV, p. 1
Sécante: III, p. 5
Second théorème de la moyenne: II, p. 31, exerc. 16
Semblables (fonctions —): V, p. 4
Série génératrice des polynômes d'Appell attachés à un opérateur de composition: VI, p. 6
Signe constant (fonction de —): V, p. 7
Sinus d'un nombre complexe: III, p. 12
Sinus hyperbolique: III, p. 12
Solution d'une équation différentielle: IV, p. 2
Solution approchée à e près d'une équation différentielle: IV, p. 3
Solution stricte d'une équation différentielle: IV, p. 2
Stirling (développement de —): VII, p. 15
Stirling (formule de —): V, p. 33
Stricte (primitive —): II, p. 2
Stricte (solution —) d'une équation différentielle: IV, p. 2
Strictement au-dessous, strictement au-dessus d'un graphe (point —): I, p. 32
Strictement concave, strictement convexe (fonction —): I, p. 34
Suite de définition d'une fonction (H): V, p. 41
Système d'équations différentielles: IV, p. 2
Système d'équations différentielles linéaires: IV, p. 16
Système fondamental d'intégrales d'un système d'équations différentielles linéaires: IV, p. 21

Tangente à un graphe: I, p. 19
Tangente hyperbolique: III, p. 12
Taylor (développement de —): I, p. 30
Taylor (formule de —): I, p. 29
Termes d'un développement asymptotique: V, p. 12
Théorème de Cauchy: IV, p. 10
Théorème de Clausen–von Staudt: VI, p. 24, exerc. 6
Théorème de la moyenne: II, p. 11
Théorème de Liouville: III, p. 30, exerc. 29
Théorème de Peano: IV, p. 6
Théorème de Rolle: I, p. 20
Théorème des accroissements finis: I, p. 23
Théorèmes de Du Bois-Reymond: V, p. 53, exerc. 8
Théorème tauberien de Hardy–Littlewood: I, p. 50, exerc. 18

Uniformément convergente (intégrale —): II, p. 21

Valeur moyenne d'une fonction: II, p. 8
Variation des constantes (méthode de —): IV, p. 20

Weierstrass (formule de —): VII, p. 3
Wronskien de n intégrales d'une équation différentielle linéaire d'ordre n: IV, p. 32

INTRODUCTION ..................................................... I.9

CHAPITRE I. — DÉRIVÉES ............................................. I.11
  § 1. Dérivée première ............................................. I.11
    1. Dérivée d'une fonction vectorielle ......................... I.11
    2. Linéarité de la dérivation ................................. I.13
    3. Dérivée d'un produit ....................................... I.14
    4. Dérivée de l'inverse d'une fonction ....................... I.16
    5. Dérivée d'une fonction composée ............................ I.17
    6. Dérivée d'une fonction réciproque .......................... I.17
    7. Dérivées des fonctions numériques .......................... I.18
  § 2. Le théorème des accroissements finis ....................... I.20
    1. Le théorème de Rolle ....................................... I.20
    2. Le théorème des accroissements finis pour les fonctions numériques ............................................. I.21
    3. Le théorème des accroissements finis pour les fonctions vectorielles ............................................. I.23
    4. Continuité des dérivées .................................... I.26
  § 3. Dérivées d'ordre supérieur ................................. I.28
    1. Dérivées d'ordre n ......................................... I.28
    2. Formule de Taylor .......................................... I.29
  § 4. Fonctions convexes d'une variable réelle .................... I.32
    1. Définition des fonctions convexes ........................... I.32
    2. Familles de fonctions convexes .............................. I.35
    3. Continuité et dérivabilité des fonctions convexes ........ I.36
    4. Critères de convexité ...................................... I.38
Exercices du § 1 .................................................. I.42
Exercices du § 2 .................................................. I.43
Exercices du § 3 .................................................. I.46
Exercices du § 4 .................................................. I.51

CHAPITRE II. — PRIMITIVES ET INTÉGRALES ....................... II.1
  § 1. Primitives et intégrales ................................... II.1

1. Définition des primitives ......................... II.1
2. Existence des primitives ......................... II.2
3. Fonctions réglées ............................... II.4
4. Intégrales ..................................... II.7
5. Propriétés des intégrales ...................... II.9
6. Forme intégrale du reste de la formule de Taylor; primitives d'ordre supérieur .................. II.12

§ 2. Intégrales dans les intervalles non compacts ............ II.13
   1. Définition d'une intégrale dans un intervalle non compact ................................. II.13
   2. Intégrales de fonctions positives dans un intervalle non compact .......................... II.16
   3. Intégrales absolument convergentes ............. II.18

§ 3. Dérivées et intégrales de fonctions dépendant d'un paramètre .... II.18
   1. Intégrale d'une limite de fonctions dans un intervalle compact ............................. II.18
   2. Intégrale d'une limite de fonctions dans un intervalle non compact ........................ II.20
   3. Intégrales normalement convergentes ............ II.23
   4. Dérivée par rapport à un paramètre d'une intégrale dans un intervalle compact ............ II.24
   5. Dérivée par rapport à un paramètre d'une intégrale dans un intervalle non compact .......... II.26
   6. Interversion des intégrations .................. II.27
Exercices du § 1 .................................. II.29
Exercices du § 2 .................................. II.33
Exercices du § 3 .................................. II.35

CHAPITRE III. — FONCTIONS ÉLÉMENTAIRES ..................... III.1
§ 1. Dérivées des fonctions exponentielles et circulaires ........ III.1
   1. Dérivées des fonctions exponentielles; nombre e ..... III.1
   2. Dérivée de $\log_a x$ ............................ III.3
   3. Dérivées des fonctions circulaires; nombre π ....... III.4
   4. Fonctions circulaires réciproques ............... III.5
   5. L'exponentielle complexe ....................... III.7
   6. Propriétés de la fonction e^z .................. III.8
   7. Le logarithme complexe ......................... III.10
   8. Primitives des fonctions rationnelles ........... III.11
   9. Fonctions circulaires complexes; fonctions hyperboliques ................................. III.12

§ 2. Développements des fonctions exponentielles et circulaires, et des fonctions qui s'y rattachent ........................................ III.15
    1. Développement de l'exponentielle réelle ............. III.15
    2. Développements de l'exponentielle complexe, de cos x et sin x .................................................. III.16
    3. Le développement du binôme ......................... III.18
    4. Développements de log (1 + x), de Arc tg x et de Arc sin x .................................................. III.21
Exercices du § 1 ............................................. III.24
Exercices du § 2 ............................................. III.32
Note historique (chapitres I–II–III) ..................... III.35
Bibliographie ............................................... III.69

CHAPITRE IV. — ÉQUATIONS DIFFÉRENTIELLES ...............
§ 1. Théorèmes d'existence .................................... IV.1
    1. La notion d'équation différentielle ................. IV.1
    2. Équations différentielles admettant pour solutions des primitives de fonctions réglées .................. IV.2
    3. Existence de solutions approchées .................. IV.4
    4. Comparaison des solutions approchées ............... IV.7
    5. Existence et unicité de solutions des équations lipschitziennes et localement lipschitziennes .......... IV.10
    6. Continuité des intégrales en fonction d'un paramètre. .................................................. IV.13
    7. Dépendance des conditions initiales ................. IV.14

§ 2. Équations différentielles linéaires ....................
    1. Existence des intégrales d'une équation différentielle linéaire ............................................. IV.16
    2. Linéarité des intégrales d'une équation différentielle linéaire ............................................. IV.18
    3. Intégration de l'équation linéaire non homogène .... IV.20
    4. Systèmes fondamentaux d'intégrales d'un système linéaire d'équations différentielles scalaires ........ IV.21
    5. Équation adjointe ...................................... IV.25
    6. Équations différentielles linéaires à coefficients constants .................................................. IV.26
    7. Équations linéaires d'ordre n ........................ IV.30
    8. Équations linéaires d'ordre n à coefficients constants . .................................................. IV.33
    9. Systèmes d'équations linéaires à coefficients constants. .................................................. IV.35
Exercices du § 1 ............................................. IV.37
Exercices du § 2 ............................................. IV.41

Note historique ............................................. IV.44
Bibliographie .................................................. IV.46

CHAPITRE V. — ÉTUDE LOCALE DES FONCTIONS .................... V.1
§ 1. Comparaison des fonctions dans un ensemble filtré ............ V.1
    1. Relations de comparaison: I. Relations faibles ...... V.2
    2. Relations de comparaison: II. Relations fortes ...... V.5
    3. Changement de variables ............................... V.7
    4. Relations de comparaison entre fonctions strictement positives ............................................. V.7
    5. Notations ............................................... V.9

§ 2. Développements asymptotiques ............................. V.10
    1. Échelles de comparaison ................................. V.10
    2. Parties principales et développements asymptotiques. V.11
    3. Sommes et produits de développements asymptotiques V.14
    4. Composition des développements asymptotiques ...... V.14
    5. Développements asymptotiques à coefficients variables V.17

§ 3. Développements asymptotiques des fonctions d'une variable réelle... V.18
    1. Intégration des relations de comparaison: I. Relations faibles ............................................. V.18
    2. Application: critères logarithmiques de convergence des intégrales ............................................. V.19
    3. Intégration des relations de comparaison: II. Relations fortes ............................................... V.20
    4. Dérivation des relations de comparaison ............. V.22
    5. Partie principale d'une primitive ..................... V.23
    6. Développement asymptotique d'une primitive ......... V.25

§ 4. Application aux séries à termes positifs .................. V.27
    1. Critères de convergence des séries à termes positifs .. V.27
    2. Développement asymptotique des sommes partielles d'une série ............................................. V.28
    3. Développements asymptotiques des produits partiels d'un produit infini ................................. V.32
    4. Application: critères de convergence de seconde espèce pour les séries à termes positifs ............... V.34

Appendice. Corps de Hardy. Fonctions (H) ..................... V.35
    1. Corps de Hardy .......................................... V.37
    2. Extension d'un corps de Hardy .......................... V.39

3. Comparaison des fonctions d’un corps de Hardy .... V.40
4. Fonctions (H) ............................................. V.41
5. Exponentielles et logarithmes itérés ................. V.41
6. Fonction réciproque d’une fonction (H) ............ V.44
Exercices du § 1 ............................................. V.48
Exercices du § 3 ............................................. V.48
Exercices du § 4 ............................................. V.50
Exercices de l’Appendice................................. V.51

CHAPITRE VI. — DÉVELOPPEMENTS TAYLORIENS GÉNÉRALISÉS. FORMULE SOMMATOIRE D’EULER–MACLAURIN .................... VI.1
§ 1. Développements tayloriens généralisés ............... VI.1
    1. Opérateurs de composition dans une algèbre de polynômes .................................................. VI.1
    2. Polynômes d’Appell attachés à un opérateur de composition .................................................. VI.5
    3. Série génératrice des polynômes d’Appell .......... VI.6
    4. Polynômes de Bernoulli ............................... VI.7
    5. Opérateurs de composition sur les fonctions d’une variable réelle ........................................ VI.9
    6. Indicatrice d’un opérateur de composition ........ VI.10
    7. La formule sommatoire d’Euler–Maclaurin ........... VI.14

§ 2. Développements eulériens des fonctions trigonométriques et nombres de Bernoulli ................................. VI.15
    1. Développement eulérien de cotg z .................. VI.15
    2. Développement eulérien de sin z .................... VI.17
    3. Application aux nombres de Bernoulli .............. VI.18

§ 3. Majoration du reste de la formule d’Euler–Maclaurin ........ VI.20
    1. Majoration du reste de la formule d’Euler–Maclaurin VI.20
    2. Application aux développements asymptotiques ..... VI.20
Exercices du § 1 ............................................. VI.22
Exercices du § 2 ............................................. VI.22
Exercices du § 3 ............................................. VI.26
Note historique (chapitres V et VI) ..................... VI.27
Bibliographie ............................................... VI.31

CHAPITRE VII. — LA FONCTION GAMMA ......................... VII.1
§ 1. La fonction gamma dans le domaine réel ............. VII.1
    1. Définition de la fonction gamma .................... VII.1

2. Propriétés de la fonction gamma ..................... VII.3
3. Les intégrales eulériennes ......................... VII.6

§ 2. La fonction gamma dans le domaine complexe ............ VII.10
    1. Prolongement à C de la fonction gamma .......... VII.10
    2. La relation des compléments et la formule de multiplication de Legendre–Gauss .................. VII.12
    3. Le développement de Stirling .................... VII.15
Exercices du § 1 ........................................ VII.19
Exercices du § 2 ........................................ VII.21

Note historique .......................................... VII.23
Bibliographie ........................................... VII.25

Index des notations ..................................... VII.26

Index terminologique .................................... VII.27

Table des matières ...................................... VII.33
