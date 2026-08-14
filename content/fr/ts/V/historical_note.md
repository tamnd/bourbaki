---
book: ts
book_title: Théories spectrales
chapter: V
chapter_title: REPRÉSENTATIONS UNITAIRES
section: 0
section_title: Historical Note
kind: historical
lang: fr
source: ts-iii-v-fr
book_pages: A V.517-A V.540
pdf_pages: 0530-0553
extraction: native
subsections:
    - "no": 1
      title: Découverte du spectre continu
      page: 517
      pdf_page: 530
    - "no": 2
      title: Opérateurs compacts
      page: 521
      pdf_page: 534
    - "no": 3
      title: Indice de Fredholm et perturbations
      page: 523
      pdf_page: 536
    - "no": 4
      title: Opérateurs partiels et théorème spectral
      page: 526
      pdf_page: 539
    - "no": 5
      title: Jonction entre analyse harmonique et théorie des groupes
      page: 528
      pdf_page: 541
    - "no": 6
      title: Groupes localement compacts commutatifs
      page: 533
      pdf_page: 546
    - "no": 7
      title: Algèbres d’opérateurs
      page: 536
      pdf_page: 549
    - "no": 8
      title: Représentations des groupes localement compacts
      page: 539
      pdf_page: 552
statements: 0
exercises: 0
content_sha256: 9a5f2c8cccd6a70e54c6cd279f0db0925bedd07636f29d5f0ab447d142870178
---

# NOTE HISTORIQUE

(Chapitres I à V)

Les notions de valeur propre et de série de Fourier étaient déjà bien connues en 1830, irriguant bien des champs de l’Analyse au long du xix$^e$ siècle (cf. ÉHM, p. 114, 260, 275). Mais la théorie spectrale et l’analyse harmonique, au sens où nous l’entendons dans ce livre, ne commencèrent à prendre leur forme actuelle qu’un siècle plus tard environ — en même temps que s’opérait leur jonction avec l’étude des représentations de groupes autour de 1930, puis avec celle des algèbres normées vers 1940.

Nous nous bornons ici à tracer les grandes lignes de leur évolution dans la période qui va de 1906 — date où Hilbert introduit la notion de « spectre continu » dans ses travaux sur les équations intégrales — aux années 1945–1950, où les théories ici exposées acquièrent pour l’essentiel la forme qu’elles ont conservée jusqu’à aujourd’hui.

### 1. Découverte du spectre continu

Dans la Note sur les Espaces vectoriels topologiques (cf. ÉHM, p. 262–263), nous avons décrit comment I. Fredholm en vint vers 1900 — poursuivant des travaux de C. Neumann, V. Volterra et H. Poincaré — à considérer l’équation

$$
u(x)-\lambda \int_IK(x, y)u(y)dy=f(x) \tag{1}
$$

d’inconnue la fonction $u: I\rightarrow \mathbf{C}$, dans le cas où l’intervalle $I\subset \mathbf{R}$ est compact et où le noyau K est continu sur $I\times I$. Un habile usage de « déterminants infinis », basé sur des idées de Poincaré et de H. von Koch, lui permettait d’obtenir des familles de solutions dont la dépendance en la variable complexe $\lambda$ est méromorphe, puis de démontrer la célèbre « alternative » sur l’existence de solutions (cf. III, p. 81, th. 5). Mais Fredholm spécialise aussitôt ses résultats au cas $\lambda =-1$, sans exploiter le fait que l’équation (1) est un problème aux valeurs propres[^1].

Lorsque le noyau K est symétrique, nous avons aussi vu comment Hilbert, dans son premier mémoire sur les équations intégrales [**31**], reconnut la parenté entre le problème de Fredholm et la recherche des « axes principaux » d’une forme quadratique. Partant de cette réduction pour des « sections » (discrétisations) finies du noyau K, il obtenait par passage à la limite la formule

$\int^{\infty}$ 1 $\int$

$$
K(s, t)x(s)x(t)dt=\sum\varphi_n(s)x(s)ds \tag{2}
$$

I $n=1\lambda n$ I

où les $\lambda_n$ sont les valeurs propres du noyau K, les $\varphi_n$ forment un système orthonormal de vecteurs propres associé[^2], et où l’égalité est valable dès que $x$ est de carré intégrable sur I (cf. ÉHM, p. 264).

Les principaux obstacles qui se présentaient à Hilbert concernaient le passage de sommes finies aux intégrales de la formule (2). Il déduisait de cette formule l’existence des valeurs propres — cependant, il donnait de ces dernières une caractérisation variationnelle indépendante du passage à la limite, inspirée de la méthode classique de détermination des valeurs propres en dimension finie (cf. n$^o4$ de IV, p. 153). E. Schmidt montrerait en 1905, s’inspirant de travaux de H. Schwarz, comment obtenir (2) sans passer par les « déterminants infinis » dont dépendaient les méthodes de Fredholm et Hilbert (cf. ÉHM, p. 265).

Mais dès 1906, Hilbert [**32**] se tourne vers le problème plus général de la réduction d’une forme quadratique

$$
B(x, x) =\sum_{p,q=0}^{\infty}b_{pq}x_px_q,x= (x_p)_{p\in\mathbf{N}}
$$

sur $E =\ell^2_{\mathbf{C}}(\mathbf{N})$. Il a bien sûr en vue que par passage aux coefficients dans une base orthonormale de E, le problème (1) se ramène à la recherche de solutions du « système linéaire infini »

$$
x_p+\sum_{q=0}^{\infty}b_{pq}x_q=f_p(p\in \mathbf{N})
$$

Il signale cependant que pour le problème de Fredholm, il s’agit de formes quadratiques bien particulières, pour lesquelles $B(x_n, x_n)$ tend vers $B(x, x)$ dès que $x_n$ converge faiblement vers $x$; il les appelle « complètement continues » (vollstetig).

Hilbert insiste sur la différence essentielle qui les distingue des formes quadratiques bornées sur E, et décide d’entreprendre la réduction plus générale de ces dernières. À nouveau, sa méthode est de partir de la réduction des « sections finies »

$$
(x_0, . . . , x_n)\mapsto \sum_{p,q=0}^nb_{pq}x_px_q
$$

de la forme B, puis de faire tendre $n$ vers l’infini. Pour ce passage à la limite, il tire profit des idées sur l’intégration introduites par T. Stieltjes dans ses travaux sur les fractions continues [**71**]. Il montre que toute forme quadratique bornée peut, après une transformation orthogonale des variables, se mettre sous la forme

1 $_2\int$ 1

$$
\sum x_p+d\sigma (s, x) \tag{3}
$$

$$
_{p\in\mathbf{N}}\lambda_{ps\in\mathbf{R}}s
$$

Dans cette formule, les $\lambda_p$ sont les valeurs propres de B et $x\mapsto \sigma (s, x)$ est (pour $s\in \mathbf{R}$ fixé) une forme quadratique positive séparante sur E, tandis que $s\mapsto \sigma (s, x)$ est[^3] (pour $x\in E$ fixé) une fonction continue croissante qui tend vers 0 en $-\infty$ et vers $\|x\|^2$ en $+\infty ($cf. ÉHM, p. 284, pour les notations de Stieltjes).

Notons S l’ensemble des points de $\mathbf{R}$ n’admettant pas de voisinage où $s\mapsto \sigma (s, x)$ reste constante pour tout $x$; alors l’intégrale dans (3) peut naturellement être prise sur S. Hilbert baptise « spectre continu » (Streckenspektrum) l’ensemble S, « spectre ponctuel » (Punktspektrum) l’ensemble des valeurs propres de B, et « spectre » (Spektrum) leur réunion. Ce terme, venu de l’optique, avait été utilisé en 1897 par W. Wirtinger [**91**] dans l’étude d’équations différentielles à coefficients périodiques.

Hilbert tirerait vite de ses méthodes « spectrales » un profond renouveau de plusieurs problèmes de l’Analyse classique, relevant de l’étude des équations différentielles ordinaires (en particulier de type Sturm–Liouville), des équations aux dérivées partielles ou des fonctions d’une variable complexe. Nous ne rendrons pas compte ici du foisonnement de résultats qui s’ensuivit dans le premier quart du xx$^e$ siècle et renvoyons à la synthèse de E. Hellinger et O. Toeplitz [**29**]. Nous mentionnerons cependant certains de ces travaux sur les équations intégrales, où se trouveront en germe des développements ultérieurs de la théorie abstraite.

Pour Hilbert et ses élèves, fidèles à une tradition allemande en Algèbre linéaire, le modèle reste le théorème des axes principaux ; aussi s’agit-il toujours d’étudier les spectres de formes bilinéaires ou quadratiques, en particulier sur l’espace « de Hilbert » $E =\ell^2_{\mathbf{C}}(\mathbf{N})$. Le fait qu’on puisse relier toute forme bilinéaire continue B sur E à l’endomorphisme continu A de E caractérisé par $\langle Ax, y\rangle = B(x, y)$ était connu de l’école de Hilbert, en particulier après les travaux de E. Schmidt, M. Fréchet et F. Riesz en 1907–1908. Mais c’est à F. Riesz qu’il revint de montrer, dans un admirable livre [**59**] de 1913, l’intérêt de mettre les endomorphismes au premier plan dans ce contexte.

Riesz donne la définition moderne du spectre d’un élément A de $\mathscr{L}(E)$[**59**, p. 139], remarque qu’il s’agit d’un ensemble fermé, borné, et montre que la résolvante $\lambda \mapsto (\lambda 1_E-A)^{-1}$ est holomorphe sur le complémentaire du spectre de A. Surtout, il fait jouer un rôle central à la structure d’algèbre de $\mathscr{L}(E) :$ s’inspirant de travaux de Volterra, il développe une première version du calcul fonctionnel pour les endomorphismes symétriques, ce qui lui permet de retrouver simplement les résultats de réduction de Hilbert et Schmidt. Si A est un élément symétrique de $\mathscr{L}$ (E), Riesz montre comment définir $f(A)$ pour toute fonction $f$ semi-continue (inférieurement ou supérieurement) de $\mathbf{R}$ dans $\mathbf{R}$, et note que $f\mapsto f(A)$ est ce que nous appelons aujourd’hui un morphisme d’algèbres [**59**, p. 129–130]. Appliquant cette idée à la fonction caractéristique d’un intervalle $[\xi ,+\infty [$, on obtient pour tout $\xi$ un endomorphisme symétrique $A_{\xi}$ de E ; utilisant l’intégrale de Stieltjes, Riesz montre alors une version de la relation (3) de Hilbert :

$$
\langle Ax, y\rangle =\int_{\mathbf{R}}\xi  d\langle A_{\xi}x, y\rangle
$$

pour $x, y\in E$, égalité qu’il écrit même

$$
A =\int_{\mathbf{R}}\xi  dA_{\xi}
$$

Le spectre de A est alors l’ensemble des valeurs $\xi_0$ telles que $A_{\xi}$ ne reste constant dans aucun voisinage de $\xi_0$, et le spectre ponctuel celui des points de discontinuité de $\xi \mapsto A_{\xi}$.

Peu avant de conclure par les applications de la théorie, Riesz note [**59**, p. 146] que ses résultats prennent une forme particulièrement simple lorsque l’endomorphisme A provient de l’une des formes bilinéaires « complètement continues » de Hilbert : le spectre se réduit à l’ensemble des valeurs propres (auxquelles il faut éventuellement ajouter 0), les valeurs propres s’organisent en une suite qui tend vers 0, et chaque valeur propre non nulle est de multiplicité finie (III, p. 90, prop. 5).

### 2. Opérateurs compacts

Riesz amplifie considérablement ces remarques moins de trois ans plus tard, dans son mémoire sur les équations fonctionnelles [**60**] qui développe, avec une limpidité intacte à plus d’un siècle de distance, l’essentiel de la théorie spectrale des opérateurs compacts sur les espaces de Banach. L’objectif affiché de ce texte est de reformuler la théorie de Fredholm pour l’équation (1) sur un intervalle compact I, en considérant l’espace $E =\mathscr{C}(I)$ muni de la topologie de la convergence uniforme. Mais comme nous l’avons déjà indiqué dans une note antérieure (ÉHM, p. 268), Riesz a clairement conscience que ses résultats s’appliquent à tout espace de Banach — notion qui ne serait introduite que dans la décennie suivante.

S’inspirant des idées de Fréchet sur la topologie générale, Riesz considère désormais les endomorphismes de E qui envoient toute suite bornée sur une suite relativement compacte. Comme Hilbert, il les appelle encore « complètement continus » et note que cette nouvelle notion est équivalente, dans le cas de E = $\ell^2_{\mathbf{C}}(\mathbf{N})$, à la notion de complète continuité qu’il avait utilisée dans son livre de 1913[^4].

Riesz étudie les endomorphismes de la forme $B = 1_E-A$ où A est un endomorphisme complètement continu de E, et déduit toutes leurs propriétés spectrales du fait qu’un espace vectoriel normé localement compact doit être de dimension finie — fait découvert, semble-t-il, pour l’occasion. Il prouve aisément que le noyau de B est de dimension finie et que son image est fermée et de codimension finie. Comme E. Weyr [**87**] l’avait fait en dimension finie, il considère alors les itérés $B^k$. Il montre que la suite de leurs noyaux et celle de leurs images sont stationnaires, puis introduit ce que nous appelons aujourd’hui nilespace et conilespace de B, montrant avec efficacité que E est leur somme directe topologique. Appliquant cette observation aux endomorphismes $B_{\lambda}= 1_E-\lambda A$ pour $\lambda \in \mathbf{C}$, il en déduit sans peine les propriétés spectrales des endomorphismes complètement continus d’un espace de Banach, et ce sous une forme à peu près définitive.

Parmi les principaux résultats sur le spectre de ces opérateurs, seuls semblent échapper à Riesz ceux qui nécessiteront un regard plus mûr sur la notion d’espace fonctionnel, en particulier sur la dualité. Par exemple, à la fin des années 1920, T. Hildebrandt [**33**] et J. Schauder [**63**] montreront (dans le cadre désormais bien établi des espaces de Banach) que l’adjoint d’un endomorphisme complètement continu est complètement continu.

Par ailleurs, la notion de complète continuité de Riesz dépend encore de l’utilisation de suites ; Banach [**4**] s’en affranchira dans son livre de 1932 pour considérer les applications qui transforment toute partie bornée en partie relativement compacte. Le terme d’application linéaire « compacte » ne s’imposera que progressivement dans la seconde moitié du xx$^e$ siècle, vraisemblablement à la suite du livre d’E. Hille [**34**] sur les semi-groupes d’opérateurs.

Plusieurs questions posées dans les années 1930 resteront longtemps ouvertes. Dans cette direction, signalons la résolution [**18**] en 1973 du « problème d’approximation » rendu célèbre par Banach et S. Mazur en 1932 et 1938 (voir la remarque 6 de III, p. 16 et l’exercice 25 de III, p. 112).

À la même époque, Lomonosov [**40**] démontre l’existence de sous-espaces fermés non triviaux invariants par un endomorphisme permutable à un endomorphisme compact non nul dans un espace localement convexe (cor. 2 de III, p. 13). Ce résultat fut l’un des progrès les plus marquants sur le problème de l’existence d’un tel sous-espace pour un endomorphisme continu arbitraire (« problème du sous-espace invariant »). Ce problème est toujours ouvert, à l’heure actuelle, dans le cas des endomorphismes continus des espaces hilbertiens de type dénombrable ; P. Enflo [**19**] construit en 1987 le premier exemple d’endomorphisme d’un espace de Banach n’admettant aucun sous-espace invariant fermé non trivial.

### 3. Indice de Fredholm et perturbations

La notion d’indice apparaît en 1920 dans un travail de Fritz Noether sur les équations intégrales. Dans son exposé au Congrès international de 1904, Hilbert considérait un problème posé par Riemann en théorie du potentiel : si l’on se donne un domaine ouvert borné Ω du plan dont la frontière est une courbe fermée lisse simple Γ, ainsi que trois fonctions $a,b,f$ sur Γ, il s’agit de trouver une fonction $z: \Omega \rightarrow \mathbf{C}$, holomorphe sur Ω et continue sur Ω, vérifiant

$a\mathscr{R}(z) +b\mathscr{I}(z) =f$ sur $\Gamma$.

Paramétrant Γ par un réel $s\in [0,2\pi ]$, Hilbert montrait que le problème revient à résoudre une équation intégrale « à noyau singulier » pour $\varphi =\mathscr{R}(z)$, à savoir

$$
a(s)\varphi (s) +\int_0^{2\pi}K(s, t)\varphi (t)dt=f(s) \tag{4}
$$

Ici le noyau $K(s, t)$ prend la forme $b(s)$ cot($^{t-s}_2$) $+ A(s, t)$ pour une fonction A continue. Il est donc singulier le long de la diagonale, et l’intégrale ci-dessus est à prendre au sens de la valeur principale de Cauchy.

Noether [**53**] observe que contrairement aux équations intégrales vérifiant l’alternative de Fredholm, dans le cas d’un noyau K comme ci-dessus et d’un second membre $f$ non nul, il est possible que (4) admette des familles de solutions non triviales. Il montre que l’espace des solutions est gouverné par l’entier

1 $\int$

(5) $n=d$ (log($a-ib$)).

$$
2\pi_{\Gamma}
$$

Si $n <0$, il n’y a pas de solution non triviale, et si $n\geqslant 0$, l’équation (4) admet une famille à $2n$ paramètres de solutions. Noether utilise le terme « indice » (Index) pour l’entier $n$ et y reconnaît un nombre de tours, notion classique depuis la fin du xix$^e$ siècle dans l’étude des fonctions d’une variable complexe.

D’autres travaux étudieront par la suite des exemples d’équations nécessitant une extension de la théorie de Fredholm. Mais il faudra attendre plus de vingt ans avant que la notion d’application de Fredholm ne soit dégagée de façon systématique, en même temps que mûrira l’étude des perturbations par des opérateurs compacts.

En 1909, H. Weyl [**81**] avait montré que si deux formes quadratiques bornées sur $\ell^2_{\mathbf{C}}(\mathbf{N})$ ont une différence complètement continue, alors leurs spectres essentiels coïncident (cf. III, p. 89, th. 2). Par ailleurs, Riesz avait remarqué dans son mémoire de 1916, naturellement sans le langage moderne, que les opérateurs compacts sur un espace de Banach E forment un idéal bilatère de $\mathscr{L}(E)$. Il semble cependant que la voie indiquée par ces deux remarques n’ait été explorée qu’à partir des années 1940. En 1941, J. Calkin, motivé par les travaux de J. von Neumann sur les algèbres d’opérateurs (dont nous aurons à parler bientôt, voir p. 537), signale l’intérêt d’étudier les congruences modulo cet idéal dans le cadre des espaces hilbertiens [**10**]. Il montre comment la structure de l’algèbre qui porte désormais son nom (cf. III, p. 75) permet de retrouver simplement le résultat de Weyl.

Parallèlement, vers 1942, J. Dieudonné [**15**] a l’idée d’étudier les perturbations d’une application linéaire continue $u$ entre espaces normés, dans le cas où la perturbation est « petite » au sens de la norme d’opérateur. Il se restreint au cas où $u$ est un morphisme strict dont le noyau est de dimension finie ou de codimension finie, prouve qu’il en est alors de même de toute « petite perturbation » de $u$, et montre que dans le cas des applications de Fredholm (cf. n$^o2$ de III, p. 40), l’indice est localement constant (th. 1 de III, p. 58), ainsi que plusieurs des résultats exposés dans le § 4 de III, p. 55.

Ces deux idées se rejoignent autour de 1950, où F. Atkinson [**3**], I. Gohberg [**26**], S. Mikhlin [**46**] et B. Yood [**93**] étudient les perturbations par des opérateurs compacts. Ils font explicitement le lien avec l’indice de Noether et dégagent les notions d’application de Fredholm [**3**, p. 8] et de Riesz [**93**, §5]. Ces dernières font l’objet de recherches systématiques dans la décennie suivante, où les résultats exposés dans le chapitre III prennent à peu près leur forme actuelle.

Le cadre usuel de ces théories est celui des espaces de Banach ; cependant, diverses applications motivent leur généralisation à des classes plus larges d’espaces vectoriels topologiques. Ainsi, le cas des espaces de Fréchet apparaît naturellement en 1954 dans des travaux de H. Cartan et J-P. Serre [**13**] qui démontrent la finitude de la cohomologie d’une variété analytique complexe compacte à coefficients dans un faisceau cohérent, la preuve faisant appel à des résultats de déformation démontrés par L. Schwartz [**66**] (cf. th. 2 de III, p. 73).

L’invariance de l’indice par déformation s’éclaire parfaitement, dans le cas de la formule (5), si l’on constate que le membre de droite (nombre de tours) est invariant par homotopie. De telles expressions topologiques de l’indice deviendront bientôt célèbres pour des applications de Fredholm issues de la géométrie différentielle. Si D est un opérateur différentiel sur une variété compacte X de classe $C^{\infty}($cf. VAR, §14), et si D est « elliptique » (cf. [**2**, §1]), alors une extension de D à des espaces de Sobolev adéquats définit une application de Fredholm. La recherche d’une formule donnant une expression topologique pour son indice à l’aide des « classes caractéristiques » de X, suggérée entre autres par des travaux de I. Gelfand vers 1960 [**23**, vol. I, p. 65], mènera en 1963 au « théorème de l’indice » de M. Atiyah et I. Singer [**2**]. Ce dernier suscitera d’extraordinaires développements au confluent de l’analyse, de la topologie et de la géométrie différentielle. Nous ne pouvons décrire ici les vastes champs qu’ils ouvrirent et qui, encore aujourd’hui très fertiles, n’ont pas fini de se nourrir de la théorie de Fredholm.

### 4. Opérateurs partiels et théorème spectral

La théorie spectrale hilbertienne générale fut créée en grande partie pour répondre au problème des fondements mathématiques de la Mécanique quantique, notamment sous l’impulsion de von Neumann.

Nous renvoyons à l’ouvrage de M. Jammer [**35**] pour une description détaillée du développement de la théorie des Quanta jusqu’à l’article fondamental de W. Heisenberg qui introduisit la Mécanique quantique [**28**]. Moins de cinq ans furent nécessaires entre sa parution à l’été 1924 et celle de l’article [**50**], en 1929, où von Neumann présente de manière parfaitement lucide et rigoureuse tous les résultats fondamentaux de la théorie des opérateurs partiels (souvent dits « non bornés ») hermitiens sur les espaces hilbertiens.

En donnant la première présentation axiomatique des espaces hilbertiens [**49**], von Neumann couronne une idée depuis longtemps en gestation (cf. ÉHM, p. 267), et éclaire divers isomorphismes entre espaces de suites ou de fonctions bien connus de Schmidt, Fréchet, Fischer et Riesz avant 1910. Cette montée en abstraction permet à von Neumann des avancées conceptuelles considérables.

Ainsi de l’idée d’opérateur partiel, qui semble planer, encore informe, sur plusieurs des travaux qui reprennent après Hilbert les équations de Fredholm (voir ci-dessus, n$^o1$). Hilbert avait remarqué que beaucoup d’équations différentielles de type Sturm–Liouville, en particulier dans le cas d’un intervalle non borné, pouvaient se ramener à des équations de Fredholm ; mais pour appliquer les méthodes intégrales, il fallait affaiblir les conditions imposées au noyau et sortir du cadre où pouvaient s’appliquer les résultats de Fredholm, Hilbert et Schmidt. Au fil des ans sont étudiés des noyaux de plus en plus singuliers, jusqu’à considérer des équations pour lesquelles le membre de gauche n’a un sens que si l’inconnue appartient à un sous-espace de $L^2(I)$. Dans cette direction, il faut mentionner des travaux d’E. Hilb [**30**] en 1908, de H. Weyl sur la théorie de Sturm–Liouville [**82**] en 1910, et surtout de T. Carleman [**11**] en 1923, dans un cadre fort général.

En unifiant ces problèmes, von Neumann jette une lumière toute nouvelle sur ces travaux classiques. Il souligne en particulier la distinction fondamentale entre opérateur symétrique et opérateur auto-adjoint, et interprète les extensions auto-adjointes d’un opérateur symétrique en fonction de « conditions au bord » abstraites, généralisant les conditions au bord bien connues qui apparaissaient, par exemple, dans les problèmes de Dirichlet et de Neumann pour l’opérateur de Laplace sur un ouvert borné de $\mathbf{R}^n$.

Dans le même temps, von Neumann [**51**] met en valeur la notion d’opérateur normal[^5] comme cadre naturel pour la théorie spectrale, insistant sur le rôle de l’algèbre commutative engendrée par l’opérateur et son adjoint.

S’appuyant sur ce formalisme mathématique précis, qui révélait également l’équivalence entre les points de vue de Heisenberg et de Schrödinger, et sur l’interprétation de Copenhague des procédures et résultats expérimentaux, la Mécanique quantique non relativiste atteignait dès lors un état de perfectionnement qui n’a guère évolué depuis ; la validité de cette théorie physique, malgré ses conséquences surprenantes, voire d’aspect paradoxal, a été depuis sans cesse confirmée par l’expérience, et cela avec une précision remarquable.

D’un point de vue formel, les bases de la théorie spectrale étaient établies par von Neumann. Parallèlement, après la présentation des premières idées de ce dernier, M. Stone avait poursuivi entre 1928 et 1930 des recherches similaires et obtenu des résultats voisins. La présentation claire et complète des résultats connus que Stone publia en 1932 [**72**] eut une influence importante dans la diffusion de la théorie spectrale hilbertienne.

Néanmoins, d’autres améliorations de la présentation ont été importantes pour la diffusion de ces résultats. En effet, le théorème spectral (cf. th. 1 de IV, p. 266), tel que le présenta von Neumann, fut longtemps considéré comme fort difficile, en grande partie car il était énoncé dans le cadre de mesures à valeurs vectorielles.

Plus tard, P. Halmos [**27**], en mettant l’accent sur l’interprétation du théorème spectral par le biais des opérateurs de multiplication sur les espaces $L^2$, en révéla l’aspect essentiellement élémentaire dans le cas des opérateurs bornés. Assez récemment, S. Woronowicz (dans le cadre un peu différent des opérateurs réguliers des modules hilbertiens sur les algèbres stellaires [**92**]) a apporté une simplification par l’introduction de la « bornification » (cf. n$^o2$ de IV, p. 265), qui permet de traiter les opérateurs partiels normaux aussi simplement que les opérateurs auto-adjoints.

Par ailleurs, si D est un opérateur différentiel scalaire formellement symétrique sur un ouvert U de $\mathbf{R}^n$, l’étude des extensions auto-adjointes de D à $L^2(U)$ est naturellement liée à l’étude des distributions sur U (dans le cas du laplacien, cf. n$^o6$ de IV, p. 242). Nous renvoyons à l’ouvrage de J. Dieudonné [**16**, ch. vii] pour l’histoire de ces dernières — histoire sinueuse qui se dénoue peu après la période que nous venons d’évoquer, avec des contributions décisives de S. Sobolev [**69**] en 1936, et de L. Schwartz [**65**] dix ans plus tard.

D’un point de vue purement mathématique, la théorie spectrale interagit de manière particulièrement fructueuse avec la Géométrie riemannienne. Ainsi, reprenant une question de S. Bochner, M. Kac donne en 1966 une présentation singulièrement frappante [**36**] du problème de la détermination des propriétés géométriques d’une variété Riemannienne qui puissent se déduire des propriétés spectrales de l’opérateur de Laplace. Cette question avait été anticipée par le physicien A. Schuster [**64**] en 1882 : To find out the different tunes sent out by a vibrating system is a problem which may or may not be solvable in certain special cases, but it would baffle the most skillful mathematician to solve the inverse problem and to find out the shape of a bell by means of the sounds which it is capable of giving out. (« Déterminer les harmoniques émises par un système vibrant est un problème qui peut être ou non résoluble dans certains cas particuliers, mais le plus habile mathématicien serait désarçonné s’il devait résoudre le problème inverse et déterminer la forme d’une cloche à partir des sons qu’elle peut émettre »).

### 5. Jonction entre analyse harmonique et théorie des groupes

Nous avons décrit, dans les notes historiques du Livre d’Intégration (cf. ÉHM, p. 275), comment les questions reliées à l’équation de la chaleur amenèrent Fourier à la conception révolutionnaire de la représentation d’une fonction arbitraire comme somme de fonctions trigonométriques.

Nous ne pouvons retracer ici le développement de la théorie des séries et intégrales de Fourier au long du xix$^e$ siècle, ni l’influence profonde qu’eurent les questions suscitées par cette théorie sur l’évolution de l’Analyse — jusqu’à bouleverser la conception des nombres réels, contribuant à la naissance de la théorie des ensembles (cf. ÉHM, p. 42). Mais pour comprendre la forme des idées exposées dans ce Livre, il convient de décrire la manière dont l’analyse harmonique fut reliée après 1925 à la théorie des groupes et à la théorie spectrale hilbertienne.

La reconnaissance du lien entre les idées de Fourier et les structures de groupe de $\mathbf{R}/\mathbf{Z}$ et $\mathbf{R}$, ainsi que la généralisation de ces idées à d’autres groupes, se firent assez tardivement.

On peut naturellement, dans les balbutiements de la théorie des groupes finis et de leurs caractères, identifier des résultats qui paraissent aujourd’hui contenir les rudiments de l’analyse de Fourier finie. Par exemple, le dual du groupe des éléments inversibles de $\mathbf{Z}/q\mathbf{Z}$, ainsi que la relation d’orthogonalité qui exprime la fonction caractéristique d’un élément comme combinaison linéaire des caractères, apparaissent implicitement en 1837 dans l’article de Dirichlet [**17**] démontrant qu’il existe une infinité de nombres premiers $p\equiv a$ mod$. q$ si $a$ est premier à $q$. Il s’appuie sur des idées de Gauss, qui avait introduit le terme « caractère » (character) dans son étude des formes quadratiques binaires à coefficients entiers et de discriminant fixé (cf. [**22**, § 230]).

Mais ni Gauss ni Dirichlet n’utilisent le langage des groupes. Il revient à Dedekind, présentant ces travaux en 1879, d’en reconnaître le rôle latent et de définir la notion de caractère pour les groupes commutatifs. Les remarques de Dedekind sont considérablement amplifiées par H. Weber, d’abord en 1882 [**77**], puis en 1886 [**78**, p. 112], où il introduit le groupe dual d’un groupe fini commutatif A et note que celui-ci est isomorphe à A. Son propos est alors de construire des extensions abéliennes du corps $\mathbf{Q}$ de groupe de Galois donné, et il ne considère pas le problème de l’analyse harmonique sur un tel groupe.

Dans le cas des groupes non commutatifs, les bases de la théorie des représentations des groupes finis étaient solidement établies vers le tournant du xx$^e$ siècle, à la suite des travaux de G. Frobenius, W. Burnside et I. Schur (cf. ÉHM, p. 154). Après 1905, il était clair que les relations d’orthogonalité des caractères jouaient un rôle crucial dans l’organisation de la théorie. Mais leur parenté avec l’analyse harmonique restait cachée.

On doit à Hermann Weyl d’avoir joint ces domaines, lorsqu’il conçut l’idée d’une théorie générale des représentations pour les groupes compacts. Dans plusieurs textes majeurs parus entre 1925 et 1927, il reconnut les liens qui uniraient une telle théorie à l’analyse de Fourier et à la théorie spectrale hilbertienne, et il jeta les bases de bien des découvertes ultérieures.

C’est une lettre de Schur qui mit Weyl sur cette voie, grâce à leur intérêt commun pour la théorie des invariants. Nous avons décrit, dans la note sur la mesure de Haar (ÉHM, p. 289–291), comment A. Hurwitz avait conçu dès 1897 l’idée d’utiliser une « intégration invariante » pour déterminer les polynômes sur $\mathbf{R}^n$ invariants par le groupe orthogonal. Il semble que Schur n’ait pas connu les résultats de Hurwitz avant 1924, où il comprit brusquement comment l’intégration invariante permettait d’étendre au groupe $\mathbf{O}(n)$ la théorie des caractères et les relations d’orthogonalité qu’il avait établies pour les groupes finis. Weyl vit immédiatement que les méthodes de Schur, jointes aux travaux d’Élie Cartan, permettaient de construire les représentations irréductibles des groupes de Lie compacts semi-simples. La série de trois mémoires dans lesquels Weyl mêlait les idées de Cartan et de Schur, parue en 1925 [**83**], contenait déjà l’essentiel des résultats de LIE, IX, §6-7 ; cf. ÉHM, p. 328–330.

Mais c’est l’année suivante, dans un texte non moins célèbre écrit avec son élève F. Peter [**54**], que Weyl met au grand jour les liens entre théorie des représentations des groupes compacts, analyse de Fourier, et théorie spectrale hilbertienne. Ce texte de moins de vingt pages contient en germe de très nombreux développements futurs.

Peter et Weyl s’affranchissent de toute hypothèse algébrique sur la structure du groupe étudié, supposant seulement que G est un groupe topologique compact muni d’une mesure invariante. L’existence d’une telle mesure était claire pour les groupes de Lie connexes ; bientôt A. Haar l’établirait en général, en partie motivé par les résultats ici présentés (cf. ÉHM, p. 291).

Le point de départ de leur étude est l’orthogonalité des coefficients matriciels. Schur avait remarqué qu’en choisissant un représentant $\pi \in \widehat{G}$ pour chaque classe d’équivalence de représentations irréductibles, un produit scalaire G-invariant sur l’espace E de $\pi$, et une base orthonormale de E, on obtient une famille de coefficients matriciels qui est orthonormale dans $L^2(G)$. Peter et Weyl entendent montrer qu’une telle famille est totale.

Dans le cas des groupes finis, le résultat analogue avait été prouvé par Frobenius en étudiant l’algèbre de groupe $\mathbf{C}[G]$. Peter et Weyl considèrent alors l’espace $\mathscr{C}(G)$ des fonctions continues sur G et le munissent du produit de convolution. Il semble qu’il s’agisse de la première utilisation du produit de convolution comme opération abstraite en lien explicite avec la structure de groupe (cf. ÉHM, p. 295). Peter et Weyl nomment d’ailleurs Gruppenzahl (« nombre de groupe ») un élément de l’algèbre $\mathscr{C}$(G), et notent $xy$ le produit (de convolution) de deux Gruppenzahlen. Ils munissent également $\mathscr{C}(G)$ de l’involution $f\mapsto \widetilde{f}$, où $\widetilde{f}(g) =f(g^{-1})$ pour $g\in G$.

Ayant donc introduit l’algèbre involutive $\mathscr{C}$(G), le premier constat fait par Peter et Weyl est que toute représentation unitaire $\pi$ de G donne lieu à une représentation $f\mapsto \pi (f)$ de $\mathscr{C}(G) ($cf. V, p. 400). La notion d’élément hermitien de $\mathscr{C}(G)$ est explicitement définie, ainsi (implicitement) que celle d’élément positif, qui ouvre la voie à l’application des techniques hilbertiennes.

Peter et Weyl n’hésitent plus à qualifier l’opérateur $\pi (f)$ de « coefficient de Fourier » de $f$, et poursuivent le parallèle avec la théorie de Fourier en remarquant que les relations d’orthogonalité de Schur impliquent l’inégalité de Bessel

(6) $\sum_{\pi\in\widehat{G}}$ dim($\pi$ ) Tr($\pi (f)\pi (f)^*$)$\leqslant (f*\widetilde{f})(e) =\|f\|^2_2$.

La théorie spectrale de Hilbert–Schmidt leur permet alors de montrer que c’est une égalité (« formule de Plancherel »). À tout élément $\varphi$ de $\mathscr{C}$ (G), Peter et Weyl associent le noyau continu $K_{\varphi}: G\times G\rightarrow \mathbf{C}$ défini par $K_{\varphi}(x, y) =\varphi (xy^{-1})$. Ils observent alors que si $\varphi$ est de la forme $f*\widetilde{f}$ avec $f\in \mathscr{C}(G)$,[^6] alors $K_{\varphi}$ est un noyau hermitien positif au sens de la théorie de Hilbert–Schmidt. Une variante d’un algorithme de Schmidt[^7] leur permet alors de construire une base orthonormale de fonctions propres du noyau $K_{\varphi}$, puis de réduire la preuve de l’égalité dans (6) au fait que la trace de l’opérateur défini par $K_{\varphi}$ est égale à la somme de ses valeurs propres.

Naturellement, ne peuvent intervenir dans (6) que les représentations $\pi$ vérifiant $\pi (f)\not = 0$; la théorie spectrale pour $K_{\varphi}$ montre l’existence d’une telle représentation si $f$ n’est pas identiquement nulle. Peter et Weyl en déduisent aisément que les représentations irréductibles séparent les points de G — un cas particulier du théorème de Gelfand–Raikov, dont il sera question plus loin.

Dans les célèbres travaux de Frobenius, une égalité analogue à (6) permettait de montrer que la représentation régulière de G contient toutes les représentations irréductibles. Mais il s’agissait d’appliquer cette égalité en prenant pour $f$ l’élément neutre de $\mathbf{C}[G]$; on avait alors évidemment $\pi (f)\not = 0$ pour tout $\pi$. D’après Peter et Weyl, l’absence d’élément neutre pour la convolution explique bien des difficultés de leur démonstration ; ils remarquent cependant, empruntant à la théorie des séries de Fourier une idée appelée à un grand avenir, qu’on peut déduire l’analogue du résultat de Frobenius en appliquant (6) à une suite de fonctions formant une unité approchée pour la convolution (cf. n$^o10$ de I, p. 120).

De même, partant de l’égalité issue de (6), la version polarisée

(7) $\sum_{\pi\in\widehat{G}}$ dim($\pi$ ) Tr($\pi (x)\pi (y)$) $= (x*y)(e)$

permet d’obtenir, en prenant pour $y$ une unité approchée pour la convolution, une approximation uniforme de tout élément de $\mathscr{C}(G)$ par des combinaisons linéaires de coefficients matriciels de représentations irréductibles. Des méthodes venaient de permettre à Weyl de donner une nouvelle démonstration [**84**] du résultat fondamental de la théorie des « fonctions presque périodiques » de H. Bohr, à laquelle nous reviendrons bientôt. Peter et Weyl signalent qu’on peut y lire la première application analytique de la théorie des représentations d’un groupe non compact, ici celui des translations de $\mathbf{R}$.

La jeune théorie quantique fournit très vite à Weyl l’occasion de revenir aux représentations de $\mathbf{R}$. Fin 1927, il signale l’intérêt des groupes (finis ou non) et des représentations pour clarifier les fondements de cette théorie [**85**]. Il y reviendra l’année suivante, dans un livre retentissant [**86**].

Dans son article de 1927, Weyl constate que si $u$ est un opérateur auto-adjoint continu sur un espace hilbertien, alors $t\mapsto e^{itu}$ est une représentation unitaire de $\mathbf{R}$. Mais il existe des représentations unitaires de $\mathbf{R}$ qui ne sont pas de cette forme ; reprenant l’idée de von Neumann sur le rôle des opérateurs partiels symétriques pour représenter les grandeurs physiques observables, Weyl suggère que toute représentation unitaire de $\mathbf{R}$ est de la forme $t\mapsto e^{itu}$, où $u$ est un opérateur partiel auto-adjoint sur un espace hilbertien. Ce point de vue lui permet de réduire l’analyse des « relations canoniques » de Heisenberg et Schrödinger, déjà étudiées en détail par von Neumann, à celle des liens entre deux représentations unitaires de $\mathbf{R}$ sur un même espace hilbertien. Stone [**73**] montre en 1932 le résultat espéré par Weyl (V, p. 428, th. 1), dans le sillage de son étude des propriétés spectrales des opérateurs auto-adjoints.

### 6. Groupes localement compacts commutatifs

L’interaction entre analyse harmonique et représentations de groupes est donc fermement établie au début des années 1930. Elle se renforce grandement dans la décennie suivante, chacun des deux sujets suscitant des progrès rapides dans l’autre.

Un terrain très fertile pour cette interaction fut l’étude des fonctions presque périodiques, introduites par H. Bohr en 1924 dans le cas des fonctions d’une variable réelle [**9**]. D’après l’un des théorèmes fondamentaux de ce dernier, il s’agit des fonctions continues bornées qui sont limites uniformes sur $\mathbf{R}$ de combinaisons linéaires de fonctions $x\mapsto e^{i\lambda x},\lambda \in \mathbf{R}($cf. II, p. 292, exerc. 54). Bochner [**6**] avait prouvé en 1926 qu’une fonction $f\in \mathscr{C}_b(\mathbf{R})$ est presque périodique si et seulement si ses translatées $x\mapsto f(x-a)$, pour $a\in \mathbf{R}$, forment une partie relativement compacte de $\mathscr{C}_b(\mathbf{R})$ pour la topologie de la convergence uniforme. Bochner et von Neumann remarquèrent que si G est un groupe topologique, cette caractérisation fournit visiblement une notion de fonction presque périodique (à droite ou à gauche) sur G. Au début des années 1930, la théorie promettait de se développer rapidement, en particulier sous l’impulsion de von Neumann [**52**] et des méthodes de Peter et Weyl.

Un autre terrain privilégié apparaît en marge de travaux de N. Wiener. Ce dernier introduit, dans un célèbre article [**88**] de 1932, des méthodes de nature algébrique dans l’étude des problèmes dits taubériens — c’està-dire dans l’étude du comportement asymptotique d’une fonction (ou d’une suite) suivant un filtre, étant données des informations concernant le comportement de certaines moyennes pondérées. Son approche était motivée par une idée de R. Schmidt.

L’un des résultats auxiliaires du travail de Wiener ([**88**, Lemma IIe]) va particulièrement frapper les esprits et inspirer de nombreux développements : si $f$ est une fonction périodique dont la série de Fourier est absolument convergente, et si $f$ ne s’annule pas, alors la série de Fourier de $1/f$ est absolument convergente (cf. I, p. 38, exemple). Dès 1932, R. Paley et N. Wiener [**89**] esquissent le lien entre ce résultat de convergence, la notion de groupe dual pour un groupe discret commutatif, et la théorie des fonctions presque périodiques.

Sur cet arrière-plan analytique, c’est la topologie algébrique qui mène L. Pontryagin à donner l’impulsion décisive pour l’étude des caractères des groupes abéliens localement compacts. Il annonce dès 1932 [**55**] l’intérêt de la notion de groupe des caractères pour mettre en dualité les groupes d’homologie d’un sous-ensemble compact de l’espace euclidien et ceux de son complémentaire. Dans un article [**58**] publié en 1934, il montre que le groupe des caractères d’un groupe discret est compact, puis établit les théorèmes de dualité dans ce cadre. Bien que Pontryagin utilise les résultats de Peter et Weyl, ainsi que la mesure de Haar dont l’existence venait d’être établie en général, il vise principalement les applications à la topologie [**57**] et ne se soucie pas explicitement d’analyse harmonique[^8] : les théorèmes de dualité sont démontrés par une étude fine de la structure des groupes compacts abéliens.

Le travail de Pontryagin suscite aussitôt un grand intérêt. Sur une suggestion de von Neumann, E. van Kampen étend l’année suivante la dualité à tous les groupes commutatifs localement compacts [**37**]. Peu après, il donne une application spectaculaire de la nouvelle analyse invariante à l’étude des fonctions presque périodiques [**38**], découverte indépendamment par A. Weil à la même période [**79**] : si G est un groupe localement compact commutatif, on obtient un groupe compact $\widetilde{G}$ en commençant par munir le groupe dual $\widehat{G}$ de la topologie discrète, puis en définissant $\widetilde{G}$ comme le groupe compact dual du groupe discret ainsi obtenu. Le groupe G se plonge alors canoniquement dans $\widetilde{G} ($cf. II, p. 292, exerc. 54) et une simple application de la théorie de Peter–Weyl pour les fonctions continues sur $\widetilde{G}$ fournit tous les résultats connus à l’époque sur les fonctions presque périodiques sur G.

Parallèlement, les fonctions de type positif, bien connues de l’analyse classique, apparaissent à cette époque dans l’étude des représentations unitaires de $\mathbf{R}$. La notion de noyau universellement positif avait été étudiée par J. Mercer [**45**] peu avant 1910, en lien avec la théorie des équations intégrales, tandis que son analogue pour les suites suscitait d’assez nombreux travaux à la même période, reliés en particulier aux problème des moments (cf. IV, p. 359, exerc. 21). Entre temps, les fonctions de type positif sur $\mathbf{R}$, déjà étudiées systématiquement par M. Mathias [**43**] en 1923, étaient devenues entre les mains de Bochner l’un des outils fondamentaux de l’analyse de Fourier et de la théorie des probabilités [**7**]. En 1933, Bochner [**8**] et Riesz [**61**] remarquent indépendamment que tout coefficient matriciel diagonal d’une représentation unitaire de $\mathbf{R}$ est une fonction de type positif sur $\mathbf{R}$. Cette observation leur permet de donner une preuve plus simple du théorème de Stone, et aura une influence déterminante sur l’évolution de la théorie générale (cf. n$^o7$).

Les résultats de cette période sont mis en ordre par A. Weil, dans un livre achevé avant 1937 et paru en 1940 [**80**]. Il y expose en détail les résultats de Peter–Weyl, de Pontryagin et de van Kampen. Mais dans le cas des groupes commutatifs, alors que Pontryagin et van Kampen mettaient l’accent sur la structure des groupes et les théorèmes de dualité, Weil développe systématiquement l’analyse harmonique, introduisant la transformation de Fourier et démontrant la formule de Plancherel et le théorème de Bochner (V, p. 455, th. 5). Il insiste notamment sur le rôle de la convolution (sous le nom de « produit de composition ») et sur celui des fonctions de type positif, désormais définies sur un groupe quelconque et reliées aux coefficients matriciels diagonaux des représentations, au moins dans le cas des représentations de dimension finie.

La généralité ainsi conquise dans le cas commutatif ouvrira un peu plus tard des horizons nouveaux en théorie des nombres. Dès 1936, en vue d’introduire des méthodes algébriques dans la théorie du corps de classes, C. Chevalley [**14**] introduit le groupe des idèles d’un corps de nombres, qui apparaîtra plus tard comme le groupe des éléments inversibles de l’anneau des adèles (cf. AC, VII, p. 221–222, et ÉHM, p. 143). En 1950, J. Tate [**75**] montrera que l’analyse harmonique pour les groupes d’adèles et d’idèles permet de retrouver aisément les équations fonctionnelles des fonctions L de Hecke, préfigurant d’extraordinaires développements liant l’analyse harmonique sur des groupes adéliques et l’étude des formes automorphes.

Mais on peut dire que dès la fin des années 1930, les résultats principaux de l’analyse harmonique invariante sont acquis pour les groupes compacts et pour les groupes localement compacts commutatifs. Dans le cas commutatif, les démonstrations de Weil dépendent encore (comme celles de Pontryagin et de van Kampen) d’une connaissance fine de la structure du groupe, c’est-à-dire à peu près des résultats de classification du § 2 de II, p. 244. La décennie suivante montrera comment s’en affranchir, grâce aux méthodes nouvelles de l’école de Gelfand (cf. H. Cartan et R. Godement [**12**]).

### 7. Algèbres d’opérateurs

Nous avons vu le rôle que Riesz, exposant en 1913 les travaux de l’école de Hilbert, fait jouer à l’algèbre $\mathscr{L}(E)$ des endomorphismes d’un espace hilbertien, ainsi qu’au calcul fonctionnel holomorphe et à la notion abstraite de spectre. Dans son mémoire de 1916, il semble déjà annoncer les algèbres normées comme cadre naturel pour la théorie spectrale ; après les travaux de Banach et de son école dans la décennie 1920, il n’est guère surprenant que cette idée ait pris une place centrale. La notion d’algèbre de Banach est introduite par M. Nagumo [**48**] en 1936, tandis que S. Mazur [**44**], en 1938, montre que la seule algèbre normée sur $\mathbf{C}$ qui soit un corps est $\mathbf{C}$ lui-même (I, p. 26, cor. 2).

Vers le milieu des années 1930, en lien avec la théorie spectrale, se multiplient les occasions de considérer abstraitement des algèbres d’opérateurs sur les espaces hilbertiens. F. Murray et J. von Neumann, dans une série de profonds et influents travaux [**47**], étudient systématiquement les sous-algèbres involutives de $\mathscr{L}(E)$ égales à leur bicommutant (« algèbres de von Neumann »). D’autre part, en 1936, S. Steen propose d’introduire une notion axiomatique d’« algèbre d’opérateurs » et d’étudier en profondeur les structures associées [**70**]. Par ailleurs, Stone [**74**], motivé par l’étude des projecteurs spectraux, étudie en 1937 les algèbres unifères dont tout élément est idempotent (« algèbres booléiennes » : cf. ÉHM, p. 146). Il note que si X est un espace topologique localement compact, les fonctions caractéristiques des parties ouvertes et celles des complémentaires des parties partout denses engendrent, dans $\mathscr{C}$ (X), une algèbre booléienne A. Il prouve alors que les idéaux de A correspondent naturellement aux parties fermées de l’espace X, introduisant ainsi une idée qui sera particulièrement féconde.

À partir de 1939, le regard de Gelfand ouvre des perspectives nouvelles sur ces résultats relativement épars. Ses travaux semblent avoir été en partie motivés par les idées de Wiener, tout particulièrement par son théorème concernant les séries de Fourier absolument convergentes, ainsi que par les méthodes de Peter et Weyl. Entre 1939 et 1946, en collaboration avec M. Naimark, D. Raikov et G. Shilov, Gelfand établit les bases de la théorie des algèbres de Banach commutatives et de celle des algèbres stellaires (cf. [**23**], vol. I, p. 169–400). Il donne notamment la démonstration classique du théorème de Wiener — généralisé par P. Lévy [**39**] — qui se trouve dans ce livre (I, p. 38, exemple).

Dans l’approche de Gelfand, l’objet essentiel auquel est reliée une algèbre de Banach commutative A est l’espace X des idéaux maximaux de A. En effet, via le théorème de Gelfand–Mazur (I, p. 26, cor. 2), tout élément de A définit une fonction sur X. On sait l’importance capitale qu’aura ce point de vue dans l’évolution ultérieure de la géométrie algébrique (cf. ÉHM, p. 146–148). Cette approche était elle-même motivée par les travaux de Stone sur les algèbres booléiennes évoqués ci-dessus.

Il semble que ce soit L. Loomis, dans un cours publié en 1953 [**41**, p. 53], qui présenta pour la première fois la théorie de Gelfand en mettant l’accent sur l’espace des caractères de A, définissant la transformation de Gelfand au sens où nous l’entendons dans ce livre. L’avantage sans doute le plus clair de ce point de vue est que les propriétés topologiques de l’espace des caractères découlent aussitôt de la compacité de la boule unité du dual d’un espace de Banach pour la topologie faible.

Dès ses premiers travaux, Gelfand avait construit l’application de calcul fonctionnel holomorphe en une variable dans une algèbre de Banach, à l’aide de l’intégrale de Cauchy, et en avait déduit qu’une algèbre de Banach involutive admet une décomposition non triviale en produit d’anneaux lorsque l’espace de ses idéaux maximaux n’est pas connexe. Le cas d’une algèbre de Banach quelconque n’est traité qu’en 1953, lorsque Shilov développe une forme du calcul fonctionnel en plusieurs variables [**68**].

Quant aux algèbres stellaires, dont Gelfand et Naimark avaient montré dès 1942 qu’elles peuvent se réaliser comme algèbres d’opérateurs sur un espace hilbertien (cf. V, p. 442, th. 2), elles ne tardent pas à devenir un objet d’abondantes et profondes études, aiguillonnées par les applications aux représentations de groupes, par les travaux de Murray et von Neumann, et par la formalisation mathématique de la Mécanique quantique. Mentionnons notamment les contributions d’I. Segal, qui fut l’un des pionniers de l’étude systématique des représentations des algèbres stellaires, en lien avec l’étude du dual unitaire des groupes localement compacts que nous évoquerons dans quelques lignes.

Bien que Gelfand, Naimark, Raikov et Shilov aient dégagé les bases essentielles de la théorie des algèbres stellaires avant 1946, certains points techniques furent améliorés ultérieurement. Ainsi, R. Arens [**1**] montra comment éviter de faire appel à l’existence du « bord de Shilov » (cf. I, p. 171, exerc. 26) pour démontrer que la transformation de Gelfand est un morphisme involutif. De plus, la théorie de Gelfand et Naimark pour les algèbres stellaires unifères ajoutait initialement comme axiome le fait que $1 +x^*x$ est inversible pour tout $x$. Ils conjecturaient cependant que cet axiome était inutile ; la preuve de cette assertion, élémentaire mais délicate, ne fut apportée que vers 1952, à la suite de travaux de M. Fukamiya [**21**] repris par I. Kaplansky [**62**].

### 8. Représentations des groupes localement compacts

Jusqu’à 1939, l’étude des représentations des groupes topologiques se bornait au cas compact et au cas commutatif. Les physiciens, de leur côté, avaient trouvé dans la Mécanique quantique de nombreuses raisons d’étudier les représentations unitaires irréductibles pour chercher des espaces hilbertiens pouvant modéliser les états de particules élémentaires. P. Dirac, s’appuyant sur des travaux de E. Majorana, avait signalé vers 1936 l’intérêt dans cette perspective du groupe de Lorentz $\mathbf{S}\mathbf{O}(3,1)$ et du groupe de Poincaré $\mathbf{S}\mathbf{O}(3,1)\ltimes \mathbf{R}^4$. Leurs méthodes restaient éloignées de celles des mathématiciens de l’époque. Mais en 1939, E. Wigner ouvrit une brèche [**90**] lorsqu’il classifia les représentations unitaires irréductibles du groupe de Poincaré en s’appuyant sur les travaux de Murray et von Neumann.

C’est à Gelfand que l’on doit, semble-t-il, d’avoir aperçu une voie générale vers l’étude des représentations des groupes localement compacts. Dans un mémoire écrit en 1942 (cf. [**23**], vol. II, p. 3–17), il signale avec Raikov qu’une telle théorie est rendue possible par le lien entre représentations unitaires et fonctions de type positif. Ils prouvent l’existence d’une réalisation hilbertienne pour toute fonction de type positif (V, p. 432, th 1) et en déduisent que les représentations unitaires irréductibles séparent les points de G (V, p. 454, th. 4). Les formes linéaires positives sur l’algèbre involutive $L^1(G)$ jouent un rôle essentiel : Gelfand et Raikov montrent le lien qui les unit aux fonctions de type positif (cf. V, p. 448, prop. 13). L’algèbre stellaire enveloppante d’une algèbre involutive est présentée (sans nom) dans [**24**, § 48], bien qu’il ne soit pas encore directement question d’associer à G l’algèbre Stell(G) (cf. 9, déf. de I, p. 125).

Après 1945, l’étude des représentations unitaires se développe à grandes enjambées. L’interaction avec les algèbres stellaires, ainsi qu’avec l’analyse des fondements de la théorie quantique, fournit vite de précieux résultats généraux : autour de 1947, Segal associe à un groupe localement compact diverses[^9] algèbres stellaires [**67**], et tisse le lien entre leurs représentations et celles du groupe considéeé. Peu après, G. Mackey dégage la notion de représentation induite [**42**], qui sera omniprésente dans les résultats concrets sur les représentations unitaires.

Parallèlement, la théorie est considérablement stimulée par l’étude d’exemples qui en révèlent la variété et la profondeur. Gelfand et Naimark, étudiant l’exemple de $\mathbf{S}\mathbf{L}(2,\mathbf{C})$, dégagent en 1947 un cas particulier de la notion de représentation induite, puis montrent qu’elle est la clé de l’étude des représentations de ce groupe [**23**, vol. II, p. 41– 124]. La même année, V. Bargmann étudie [**5**] le groupe $\mathbf{S}\mathbf{L}(2,\mathbf{R})$ et découvre l’existence d’une famille dénombrable de représentations de carré intégrable, baptisée « série discrète » (discrete series), ainsi que les relations d’orthogonalité entre leurs coefficients matriciels (cf. prop. 8 de V, p. 424). Comme Godement s’en aperçut aussitôt [**25**], les relations d’orthogonalité de Bargmann sont vérifiées par toutes les représentations de carré intégrable des groupes localement compacts.

Bientôt l’étude de classes particulières de groupes prendra à nouveau, et pour longtemps, le dessus sur la théorie abstraite. Harish-Chandra, en particulier, entamera l’étude générale des représentations des groupes de Lie réductifs — tâche épique que nous ne pouvons décrire ici, pas plus que les prodigieuses conséquences qu’en pressentira Langlands pour la théorie des nombres.

[^1]: Rappelons que c’est Poincaré qui, guidé par le problème des « membranes vibrantes » où la notion de valeur propre jouait un rôle essentiel, avait introduit un paramètre $\lambda$ dans (1) et suggéré d’étudier la dépendance en $\lambda$ des solutions (cf. ÉHM, p. 262).
[^2]: Pour Hilbert, la relation définissant valeurs et vecteurs propres est l’égalité $\varphi_n(t) =\lambda_n\int_IK(s, t)\varphi_n(s)ds$; les « valeurs propres » qu’il évoque sont donc les inverses de celles que consacre la terminologie moderne, et peuvent être infinies. Comme nous le verrons, le changement fut proposé par F. Riesz en 1913.
[^3]: Comme le fait remarquer Hilbert, on peut caractériser $\sigma (s, x) =\sum_{p,q=0}^{\infty}\sigma_{pq}(s)x_px_q$ par le fait qu’elle vérifie $\int_{\mathbf{R}}d\sigma (s, x) =\|x\|^2$ et que pour toute fonction continue $u$ sur $\mathbf{R}$, on ait $\sum_{r=0}^{\infty}\int_{\mathbf{R}}u(s)d\sigma_{pr}(s)\int_{\mathbf{R}}u(s)d\sigma_{rq}(s) =\int_{\mathbf{R}}u(s)^2d\sigma_{pq}(s)$.
[^4]: Cette équivalence est encore valable dans le cas d’un espace de Banach réflexif, mais les deux notions sont différentes en général : cf. III, p. 7, prop. 8.
[^5]: Cette notion était connue des algébristes à la fin du xix$^e$ siècle, et utilisée par Toeplitz [**76**] dans un cadre analytique en 1918.
[^6]: Il s’agit de la forme générale d’un élément positif de $\mathscr{C}$(G), cf. n$^o2$ de I, p. 118.
[^7]: Il s’agit de l’algorithme qui permettait à Schmidt, s’inspirant des travaux de Schwarz et considérant les « itérés » du noyau $K_{\varphi}$, de simplifier les résultats de Fredholm et Hilbert dans sa thèse de 1905.
[^8]: Cela ne signifie pas que Pontryagin néglige l’Analyse : dans une courte note [**56**] de 1933, jointe à une contribution de Stepanoff et Tychonoff concernant les fonctions presque périodiques sur $\mathbf{R}$, il avait reformulé leur résultat au moyen de deux groupes abéliens en dualité.
[^9]: Segal propose dès 1941 d’associer à un tel groupe G une algèbre de Banach pour étudier les représentations ; mais à ce moment il pense plutôt à l’algèbre obtenue à partir de $L^1(G)$ par adjonction d’un élément unité. En 1947, dans un article influent, il associe à G une algèbre stellaire en vue de la décomposition de la représentation régulière ; ce qu’il introduit est alors plutôt l’algèbre stellaire « réduite », quotient de Stell(G) par le noyau de la représentation régulière, que l’algèbre stellaire universelle elle-même. Cette dernière semble apparaître dans ses ses habits modernes en 1960 dans un texte de J. Fell [**20**].
