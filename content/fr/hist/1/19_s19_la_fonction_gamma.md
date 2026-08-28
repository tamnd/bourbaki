---
book: hist
book_title: Elements of the History of Mathematics
chapter: "1"
chapter_title: ÉLÉMENTS D'HISTOIRE DES MATHÉMATIQUES
section: 19
section_title: La fonction gamma
lang: fr
source: hist-fr
pdf_pages: 0253-0254
extraction: ocr
statements: 0
exercises: 0
content_sha256: 7ffea6c7a3ebb2c35c10d984f8aeb59c0298bc7a9d6371edfcdc5ae7a12875d5
---

## 19. LA FONCTION GAMMA

L’idée d’« interpoler » une suite $(u_n)$ par les valeurs d’une intégrale dépendant d’un paramètre réel $\lambda$ et égale à $u_n$ pour $\lambda = n$, remonte à Wallis (cf. p. 233-234). C’est cette idée qui guide principalement Euler lorsque, en 1730 ([/08 a], (1), t. XIV, p. 1-24), il se propose d’interpoler la suite des factorielles. Il commence par remarquer que $n!$ est égal au produit infini $$\prod_{k=1}^{\infty} \left( \frac{k+1}{k} \right)^n \frac{k}{k+n},$$ que ce produit est défini pour toute valeur de $n$ (entière ou non), et qu’en particulier, pour $n = \frac{1}{2}$ il prend la valeur $\frac{1}{2} \sqrt{\pi}$ d’après la formule de Wallis. L’analogie de ce résultat avec ceux de Wallis le conduit alors à reprendre l’intégrale $$\int_0^1 x^e (1-x)^n dx$$ ($n$ entier, $e$ quelconque), déjà considérée par ce dernier. Euler en obtient la valeur $$\frac{n!}{(e+1)(e+2)\ldots(e+n)}$$ par le développement du binôme ; un changement de variables lui montre alors que $n!$ est la limite, pour $z$ tendant vers 0, de l’intégrale $$\int_0^1 \left( \frac{1-x^z}{z} \right)^n dx,$$ d’où la « seconde intégrale eulérienne » $$n! = \int_0^1 \left( \log \frac{1}{x} \right)^n dx;$$ par la même méthode, et l’usage de la formule de Wallis, il obtient la formule $$\int_0^1 \sqrt{\log \frac{1}{x}} dx = \frac{1}{2} \sqrt{\pi}.$$ Dans ses travaux ultérieurs, Euler revient fréquemment à ces intégrales; il découvre ainsi la relation des compléments ([108 a], (1), t. XV, p. 82 et t. XVII, p. 342), la formule B $(p, q) = \Gamma(p)\Gamma(q)/\Gamma(p+q)$ ([108 a], (1), t. XVII, p. 355), et le cas particulier de la formule de Legendre-Gauss correspondant à $x = 1$ ([108 a], (1), t. XIX, p. 483); le tout bien entendu sans s'inquiéter de questions de convergence.

Gauss poursuit l'étude de la fonction $\Gamma$ à l'occasion de ses recherches sur la fonction hypergéométrique, dont la fonction $\Gamma$ est un cas limite ([124 a], t. III, p. 125-162); c'est au cours de ces recherches qu'il obtient la formule générale de multiplication (déjà remarquée par Legendre peu auparavant pour $p = 2$). Les travaux ultérieurs sur $\Gamma$ ont surtout porté sur le prolongement de cette fonction au domaine complexe. Ce n'est que récemment que l'on s'est aperçu que la propriété de convexité logarithmique caractérisait $\Gamma(x)$ (dans le domaine réel) à un facteur près parmi toutes les solutions de l'équation fonctionnelle $f(x+1) = x f(x)$ ([26], p. 149-164); et Artin a montré [7 d] comment on peut rattacher simplement tous les résultats classiques sur $\Gamma(x)$ à cette propriété.
