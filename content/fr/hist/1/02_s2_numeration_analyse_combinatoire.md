---
book: hist
book_title: Elements of the History of Mathematics
chapter: "1"
chapter_title: ÉLÉMENTS D'HISTOIRE DES MATHÉMATIQUES
section: 2
section_title: Numération; analyse combinatoire
lang: fr
source: hist-fr
pdf_pages: 0062-0064
extraction: ocr
statements: 0
exercises: 0
content_sha256: 9b64bcdd7a962f10417ac39132181a10a7dd7178e2eec2aeebc82d881c793345
---

## 2. NUMÉRATION ; ANALYSE COMBINATOIRE

L’histoire et l’archéologie nous font connaître un grand nombre de « systèmes de numération » ; leur but initial est d’attacher à chaque entier individuel (jusqu’à une limite qui dépend des besoins de la pratique) un nom et une représentation écrite, formés de combinaisons d’un nombre restreint de signes, s’effectuant suivant des lois plus ou moins régulières. Le procédé de beaucoup le plus fréquent consiste à décomposer les entiers en sommes d’« unités successives » $b_1, b_2, ..., b_n, ...$, dont chacune est un multiple entier de la précédente ; et si en général $b_n / b_{n-1}$ est pris égal à un même nombre $b$ (la « base » du système, le plus souvent 10), on observe mainte exception à cette règle, comme chez les Babyloniens, où $b_n / b_{n-1}$ est tantôt égal à 10, tantôt à 6 [232], et dans le système chronologique des Mayas, où $b_n / b_{n-1}$ est égal à 20 sauf pour $n = 2$, et où $b_2 / b_1 = 18$ [228]. Quant à l’écriture correspondante, elle doit indiquer le nombre d’« unités » $b_i$ de chaque ordre $i$ ; dans beaucoup de systèmes (comme chez les Égyptiens, les Grecs et les Romains), les multiples successifs $k.b_i$ (où $k$ varie de 1 à $(b_{i+1}/b_i)-1$) sont désignés par des symboles qui dépendent à la fois de $k$ et de $i$. Un premier et important progrès consiste à désigner tous les nombres $k.b_i$ (pour la même valeur de $k$) par le même signe : c’est le principe de la « numération de position », où l’indice $i$ est indiqué par le fait que le symbole représentant $k.b_i$ apparaît à la $i$-ème place dans la succession des « tranches » constituant le nombre représenté. Le premier système de cette nature se rencontre chez les Babyloniens, qui, sans doute dès 2 000 avant J.-C., notent par un même signe tous les multiples $k.60^{\pm i}$ correspondant à des valeurs quelconques de l’exposant $i$ ([232], p. 93-109). L’inconvénient d’un tel système réside bien entendu dans l’ambiguïté des symboles employés, tant que rien n’indique que les unités d’un certain ordre peuvent être absentes, en d’autres termes, tant que le système n’est pas complété par l’introduction d’un « zéro ». On voit pourtant les Babyloniens se passer d’un tel signe pendant la plus grande partie de leur histoire ; ils n’emploient en effet un « zéro » que dans les deux derniers siècles avant J.-C., et encore seulement à l’intérieur d’un nombre ; jusque-là, le contexte devait seul préciser la signification du nombre considéré. Deux autres systèmes seulement utilisent systématiquement un « zéro » : celui des Mayas (en usage, semble-t-il, dès le début de l’ère chrétienne [228]), et notre système décimal actuel, qui (par l’intermédiaire des Arabes) dérive de la mathématique hindoue, où son usage est attesté dès les premiers siècles de notre ère. Il faut noter en outre que la conception du zéro comme un nombre (et non comme un simple signe de séparation) et son introduction dans les calculs, comptent aussi parmi les contributions originales des Hindous ([78], t. I). Bien entendu, une fois acquis le principe de la numération de position, il était facile de l’étendre à une base quelconque ; la discussion des mérites des différentes « bases » proposées depuis le xviiie siècle relève des techniques du Calcul numérique et ne saurait être abordée ici. Bornons-nous à remarquer que l’opération qui sert de fondement à ces systèmes, la division dite « euclidienne », n’apparaît pas avant les Grecs, et remonte sans doute aux premiers Pythagoriciens, qui en firent l’outil essentiel de leur Arithmétique théorique (voir p. 110).

Les problèmes généraux d’énumération, groupés sous le nom d’ « Analyse combinatoire », ne paraissent pas avoir été abordés avant les derniers siècles de l’Antiquité classique : seule la formule
$$
\binom{n}{2} = n(n-1)/2
$$
est attestée au IIIe siècle de notre ère. Le mathématicien hindou Bhaskara (xire siècle) connaît la formule générale pour
$$
\binom{n}{p}.
$$
Une étude plus systématique se trouve dans un manuscrit de Levi ben Gerson, au début du xiiiie siècle : il obtient la formule de récurrence permettant de calculer le nombre $V_n^p$ des arrangements de $n$ objets $p$ à $p$, et en particulier le nombre des permutations de $n$ objets ; il énonce aussi des règles équivalentes aux relations
$$
\binom{n}{p} = V_n^p / p! \text{ et } \binom{n}{n-p} = \binom{n}{p} \quad ([311], \text{ t. VI, p. 64-65}). $$
Mais ce manuscrit paraît être resté ignoré des contemporains, et les résultats n’en sont que peu à peu retrouvés par les mathématiciens des siècles suivants. Parmi les progrès ultérieurs, signalons que Cardan démontre que le nombre des parties non vides d’un ensemble de $n$ éléments est $2^n - 1$; Pascal et Fermat, fondant le calcul des probabilités, retrouvent l’expression de $\binom{n}{p}$, et Pascal est le premier à observer la relation entre ces nombres et la formule du binôme : cette dernière paraît avoir été connue des Arabes dès le XIIIe siècle, des Chinois au XIVe siècle, et elle avait été retrouvée en Occident au début du XVIe siècle, ainsi que la méthode de calcul par récurrence dite du « triangle arithmétique », que l’on attribue d’ordinaire à Pascal ([311], t. VI, p. 35-38). Enfin, Leibniz, vers 1676, obtient (sans la publier) la formule générale des « coefficients multinomiaux », retrouvée indépendamment et publiée 20 ans plus tard par de Moivre.
