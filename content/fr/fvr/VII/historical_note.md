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
book_pages: A V.113
pdf_pages: 0314-0316
extraction: ocr
statements: 0
exercises: 0
content_sha256: cd131e498b6057c0908bf59aa12185648760ddbc0a8f6986490ad580efe8280b
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
