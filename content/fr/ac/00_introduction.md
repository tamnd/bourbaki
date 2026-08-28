---
book: ac
book_title: Commutative Algebra
chapter: ""
chapter_title: ""
section: 0
section_title: INTRODUCTION
kind: introduction
lang: fr
source: ac-i-iv-fr
pdf_pages: 0005-0010
extraction: ocr
statements: 0
exercises: 0
content_sha256: b7bba9dde72330951f573406dd26684da013cdb4e80479220b2ccb341ad5ece1
---

## INTRODUCTION

Les questions traitées dans ce Livre se sont présentées au cours du développement de la théorie des nombres algébriques et (plus tardivement) de la géométrie algébrique (cf. Note historique). À partir du xixe siècle, on s’est aperçu peu à peu que ces deux théories présentaient de remarquables analogies ; en cherchant à résoudre les problèmes qu’elles posaient, on a été amené à dégager un certain nombre d’idées générales, dont le champ d’application ne se limite pas aux anneaux de nombres algébriques ou de fonctions algébriques ; et, comme toujours, il y a avantage à considérer ces notions sous leur aspect le plus général pour en mieux saisir la portée véritable et les répercussions mutuelles. On traite donc dans ce Livre de concepts applicables en principe à tous les anneaux commutatifs et aux modules sur de tels anneaux ; il faut toutefois signaler qu’on n’obtient souvent de résultats substantiels qu’en introduisant des hypothèses de finitude (toujours vérifiées dans les cas classiques), par exemple en supposant les modules de type fini ou les anneaux noethériens.

Les principales notions autour desquelles se groupent les premiers chapitres sont les suivantes :

I. Localisation et globalisation. Partons par exemple d’un système d’équations diophantiennes :

(*) $P_i(x_1, ..., x_m) = 0$ $(1 \leq i \leq n)$

où les $P_i$ sont des polynômes à coefficients entiers rationnels, et où on cherche des solutions $(x_i)$ formées de nombres entiers rationnels. On peut commencer à aborder le problème en cherchant des solutions formées de nombres rationnels, ce qui consiste à envisager le même problème où les coefficients des $P_i$ sont considérés comme des éléments du corps des fractions $\mathbf{Q}$ de $\mathbf{Z}$, et où l’on se propose de trouver les solutions à valeurs dans $\mathbf{Q}$. Une seconde étape consiste à voir si, étant donné un nombre premier $p$, il existe des solutions rationnelles dont les dénominateurs ne sont pas divisibles par $p$ (il est clair que les solutions entières vérifient cette condition); cela revient cette fois à se placer dans le sous-anneau $\mathbf{Z}_{(p)}$ de $\mathbf{Q}$ formé des nombres rationnels de cette nature, dit anneau local de $\mathbf{Z}$ correspondant au nombre premier $p$. Il est clair que le passage de $\mathbf{Z}$ à $\mathbf{Q}$ et celui de $\mathbf{Z}$ à $\mathbf{Z}_{(p)}$ sont de même nature : dans les deux cas, on n’admet comme dénominateurs que ceux qui n’appartiennent pas à un certain idéal premier (l’idéal (0) ou l’idéal ($p$) suivant le cas). Le mot même d’« anneau local » provient de la géométrie algébrique, où cette notion apparaît de façon plus naturelle : par exemple, dans l’anneau $\mathbf{C}(X)$ des fonctions rationnelles d’une variable à coefficients complexes, l’anneau local correspondant à l’idéal premier $(X - \alpha)$ est l’anneau des fractions rationnelles « régulières » au point $\alpha$ (c’est-à-dire n’ayant pas de pôle en ce point).

Tout problème diophantien, et plus généralement tout problème sur des A-modules (A anneau commutatif) peut se décomposer en deux problèmes partiels : on cherche à le résoudre dans les anneaux locaux $A_p$ correspondant aux différents idéaux premiers $p$ de $A$ (« localisation »), puis on se demande si, de l’existence pour tout $p$ d’une solution du problème « localisé », on peut conclure à l’existence d’une solution du problème initialement posé (« passage du local au global »). C’est à l’étude de ce double processus qu’est consacré le chapitre II, où d’ailleurs on verra que la « localisation » n’est pas liée aux seuls idéaux premiers, mais à une portée plus vaste.

II. Complétion des anneaux locaux. Un anneau local $A$ partage avec les corps la propriété de n’avoir qu’un seul idéal maximal $m$. On utilise ce fait pour ramener, dans une certaine mesure, un problème sur des A-modules à un problème analogue sur des espaces vectoriels, en passant cette fois à l’anneau quotient

A/m, puisque ce dernier est un corps. Si on revient par exemple au système diophantien (*), cette idée n’est autre que le principe de la « réduction modulo $p$ », transformant les équations en congruences mod. $p$, qui s’est présentée de façon naturelle dès les premiers travaux de théorie des nombres.

Ce faisant, il est clair qu’on ne peut toutefois espérer atteindre ainsi des résultats complets sur le problème initial, et on s’est vite rendu compte que pour avoir des renseignements plus précis, il faut non seulement considérer les congruences modulo $m$, mais aussi les congruences « supérieures » modulo $m^n$, pour des entiers $n > 0$ arbitraires. On se convainc même ainsi que, plus $n$ est grand, plus on « approche » en quelque sorte du problème initial (dans le cas où $A = \mathbf{Z}$ par exemple, la raison en est qu’un entier $\neq 0$ ne peut être divisible par toutes les puissances $p^n$ d’un nombre premier donné $p$; la présence de cet entier se fera donc sentir dans la réduction mod. $p^n$ dès que $n$ sera pris assez grand). La traduction mathématique de cette idée consiste à considérer sur $A$ une topologie d’anneau (cf. Top. gén., chap. III, 3e éd., § 6) pour laquelle les $m^n$ forment un système fondamental de voisinages de 0. Mais lorsqu’on a ainsi, par exemple, résolu le système de congruences

$$
P_i(x_1, ..., x_m) \equiv 0 \pmod{p^k} \quad (1 \leq i \leq n)
$$

pour tout entier $k > 0$, il ne s’ensuit pas encore que le système (*) ait une solution dans l’anneau local $\mathbf{Z}_{(p)}$; on constate que l’hypothèse précédente peut s’interpréter en disant que (*) admet une solution dans le complété $\widehat{\mathbf{Z}}_{(p)}$ de l’anneau topologique $\mathbf{Z}_{(p)}$.

Le problème initial, ainsi affaibli, est finalement ramené au problème analogue pour les anneaux locaux du type $A/m^n$, qui sont encore plus proches des corps que les anneaux locaux généraux, puisqu’ils ont un radical nilpotent; en géométrie algébrique classique, cela correspond à une étude « différentielle » du problème au voisinage d’un point donné.

Le chapitre III traite d’une façon générale de ces applications de notions topologiques à la théorie des anneaux locaux. Au chapitre VI, on en étudie un aspect plus spécial, adapté d’une part à des études plus fines de géométrie algébrique, et surtout à l’arithmétique

L’étude du passage d’un anneau $A$ à un localisé $A_p$ ou à un complété $\hat{A}$ fait apparaître un caractère commun à ces deux opérations, la propriété de platitude des $A$-modules $A_p$ et $\hat{A}$, qui permet entre autres de manier les produits tensoriels de tels $A$-modules avec des $A$-modules quelconques un peu comme on le fait des produits tensoriels d’espaces vectoriels, c’est-à-dire sans toutes les précautions dont s’entoure leur emploi dans le cas général. Les propriétés liées à cette notion, qui s’applique d’ailleurs aussi aux modules sur des anneaux non commutatifs, font l’objet du chapitre I.

III. Entiers et décomposition des idéaux. L’étude de la divisibilité dans les corps de nombres algébriques nécessitait dès le début l’introduction d’une notion d’entier dans un tel corps $K$, généralisant la notion d’entier rationnel dans le corps $\mathbf{Q}$. La théorie générale de cette notion d’« entier algébrique », liée, comme on le verra, à des conditions de finitude très strictes, est développée au chapitre V : elle s’applique à tous les anneaux commutatifs, et présente un grand intérêt non seulement en arithmétique, mais en géométrie algébrique et même dans la théorie moderne des « espaces analytiques » sur le corps $\mathbf{C}$.

Un des obstacles majeurs à l’extension de l’arithmétique classique aux anneaux d’entiers algébriques a longtemps été le fait que la décomposition classique d’un entier rationnel en facteurs premiers ne s’étend pas en général à ces anneaux. Il fallut la création de la théorie des idéaux pour surmonter cette difficulté : la décomposition unique cherchée est alors rétablie pour les idéaux, la notion d’idéal premier se substituant bien entendu à celle de nombre premier. On peut d’ailleurs considérer ce résultat comme un cas typique où le « passage du local au global » se fait de façon satisfaisante : la connaissance, pour un $x \in K$, des valeurs en $x$ de toutes les « valuations » de $K$, détermine $x$ à multiplication près par un entier inversible.

Dans des anneaux moins simples que les anneaux d’entiers algébriques (et déjà par exemple dans les anneaux de polynômes à plusieurs indéterminées) ce résultat perd sa validité. On peut toutefois associer d’une façon canonique à tout idéal un ensemble bien déterminé d’idéaux premiers : en géométrie algébrique, si on considère par exemple dans $K^n$ (K corps commutatif quelconque) une sous-variété définie par un système d’équations polynomiales $P_\alpha = 0$, les composantes irréductibles de cette sous-variété correspondent biunivoquement aux éléments minimaux de l’ensemble des idéaux premiers ainsi associés à l’idéal engendré par les $P_\alpha$. On peut en outre (si l’on se borne aux anneaux noethériens) donner pour tout idéal une « décomposition » moins précise qu’une décomposition en produit d’idéaux premiers : le produit y est en effet remplacé par l’intersection, et les puissances d’idéaux premiers par des idéaux « primaires » liés aux idéaux premiers associés à l’idéal envisagé (mais qui ne sont pas des généralisations directes des puissances d’idéaux premiers). L’introduction des idéaux premiers associés à un idéal et l’étude de leurs propriétés font l’objet du chapitre IV ; on y démontre aussi l’existence et certaines propriétés d’unicité des « décompositions primaires » auxquelles nous venons de faire allusion ; mais il apparaît à présent que ces décompositions ne jouent le plus souvent qu’un rôle accessoire dans les applications, la notion essentielle étant celle d’idéal premier associé à un idéal.

Au chapitre VII, on examine plus en détail les anneaux où l’on se rapproche davantage des propriétés des anneaux d’entiers algébriques en ce qui concerne la décomposition en produit d’idéaux premiers ; on peut entre autres introduire dans ces anneaux la notion de « diviseur » qui est l’aspect géométrique de cette décomposition et joue un rôle important en géométrie algébrique.

Enfin, les chapitres VIII et suivants traiteront de notions qui présentent plus d’intérêt en géométrie algébrique qu’en arithmétique (où elles deviennent triviales) et notamment du concept de dimension.

Avec ces notions, on parvient à la frontière de la géométrie algébrique proprement dite, frontière toujours plus mouvante et difficile à tracer. C’est que, si l’algèbre commutative est un outil essentiel pour développer la géométrie algébrique dans toute sa généralité, inversement (comme on a déjà pu l’apercevoir ci-dessus), le langage de la géométrie s’avère extrêmement commode pour exprimer les théorèmes d’algèbre commutative et y suggérer une certaine intuition, naturellement assez absente de l’algèbre abstraite ; avec la tendance actuelle à élargir de plus en plus le cadre de la géométrie algébrique, le langage algébrique et le langage géométrique tendent plus que jamais à se confondre.
