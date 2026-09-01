---
book: top
book_title: General Topology
chapter: V
chapter_title: GROUPES À UN PARAMÈTRE
section: 3
section_title: Caractérisation topologique des groupes R et T
lang: fr
source: top-v-x-fr
book_pages: TG V.16-TG V.18
pdf_pages: 0017-0018, 0023-0025
extraction: ocr
statements: 3
exercises: 8
content_sha256: 1b241ea5ab460c6fa4478874830270979c7cae6eb7768627da21ab227f648857
---

## § 3. CARACTÉRISATION TOPOLOGIQUE DES GROUPES R ET T

#### Théorème 1 {#top-v-s3-thm-1 .statement}

Un groupe topologique G, dans lequel il existe un voisinage ouvert de l’élément neutre homéomorphe à un intervalle ouvert de R, est localement isomorphe à R.

L’intérêt de ce théorème est qu’il permet de conclure d’une propriété purement topologique d’un groupe G à une propriété de la structure de groupe de G.

Il s’agit là d’un phénomène tout à fait particulier au groupe R, et qui n’a pas d’analogue pour les groupes $\mathbf{R}^n$ lorsque $n > 1$ (cf. VIII, p. 7). Les groupes localement isomorphes à R sont parfois appelés groupes à un paramètre.

Pour démontrer le th. 1, nous allons nous ramener à la prop. 2 de V, p. 9. Par hypothèse, il existe un homéomorphisme $\varphi$ d’un voisinage ouvert U de l’élément neutre $e$ de G, sur un intervalle ouvert de R. Par l’application réciproque de $\varphi$, on peut transporter à U la structure d’ensemble totalement ordonné de l’intervalle $\varphi(U)$; la topologie de U (induite par celle de G) a alors pour base l’ensemble des intervalles ouverts de U (IV, p. 5, prop. 5). On peut trouver un voisinage symétrique V de $e$, tel que $V.V \subset U$, et que V soit un intervalle ouvert; en effet, il existe un intervalle ouvert $V'$, contenant $e$, et tel que l’on ait $V'.V' \subset U \cap U^{-1}$, $V'.{V'}^{-1} \subset U$ et ${V'}^{-1}.V' \subset U$; en prenant $V = V' \cup {V'}^{-1}$, V est ouvert, symétrique, satisfait à $V.V \subset U$ et est connexe, donc est un intervalle (IV, p. 8, th. 4).

Montrons que, si $x, y, z$ appartiennent à V, la relation $x < y$ entraîne $xz < yz$ et $zx < zy$; en effet, les fonctions $f_1(z) = \varphi(yz) - \varphi(xz)$ et $f_2(z) = \varphi(zy) - \varphi(zx)$ sont continues dans V; elles sont $> 0$ pour $z = e$, et ne s’annulent pas dans V (car $\varphi(yz) = \varphi(xz)$, par exemple, entraînerait $yz = xz$, donc $y = x$). Comme $f_1(V)$ et $f_2(V)$ sont connexes (I, p. 82, prop. 4), donc sont des intervalles de R (IV, p. 8, th. 4), et que ces intervalles contiennent un nombre $> 0$ et ne contiennent pas 0, ils sont contenus dans $\mathbf{R}_+^*$, autrement dit, on a $f_1(z) > 0$ et $f_2(z) > 0$ quel que soit $z \in V$.

Si $x$ et $y$ sont deux éléments de V tels que $x \geq e, y \geq e$, on a en particulier $xy \geq e$. Appelons E l’ensemble (totalement ordonné) des éléments de U qui sont $\geq e$, et I l’ensemble des éléments de V qui sont $\geq e$; les axiomes (GR_I), (GR_{II}), (GR_{IIIa}) et (GR_{IVa}) du § 2 sont vérifiés (en prenant pour $\omega$ l’élément $e$, et pour loi de composition celle du groupe G); c’est immédiat pour (GR_I), (GR_{II}) et (GR_{IVa}) d’après ce qui précède; pour (GR_{IIIa}), il suffit de remarquer que, si $e < x < y$ ($x \in V, y \in V$), on a $x^{-1} \in V$, donc $x^{-1} < e < x^{-1}y$, et $x^{-1}y < y$; par suite $z = x^{-1}y$ appartient à I et on a bien $xz = y$. D’après la prop. 2 de V, p. 9, il existe donc une application strictement croissante $f$ de I sur un intervalle de $\mathbf{R}_+$ d’origine 0, telle que $f(e) = 0$ et $f(xy) = f(x) + f(y)$ chaque fois que $x, y$ et $xy$ appartiennent à I (ce qui sera le cas si $x$ et $y$ appartiennent à $W \cap I$, où $W$ est un voisinage de $e$ tel que $W.W \subset V$).

Pour tout élément $x \in V$ n’appartenant pas à I, on a $x < e$, donc $x^{-1} > e$; on prolonge par suite $f$ en une application strictement croissante $f$ de V sur un intervalle de $\mathbf{R}$ en posant $\tilde{f}(x) = -f(x^{-1})$ pour tout $x < e$ de V. L’image réciproque par $\tilde{f}$ d’un intervalle ouvert contenu dans $\tilde{f}(V)$ est un intervalle ouvert de V, donc $\tilde{f}$ est continue dans V; inversement, l’image par $\tilde{f}$ d’un intervalle ouvert de V est un intervalle ouvert de $\tilde{f}(V)$, donc $\tilde{f}$ est un homéomorphisme de V sur un voisinage de 0 dans le groupe $\mathbf{R}$. D’autre part, on vérifie aisément (comme dans la prop. 6 de V, p. 3, en examinant les divers cas possibles) qu’on a $\tilde{f}(xy) = \tilde{f}(x) + \tilde{f}(y)$ chaque fois que $x, y$ et $xy$ appartiennent à V; on en conclut que $\tilde{f}$, restreint à un voisinage convenable de $e$ dans G, est un isomorphisme local de G à $\mathbf{R}$ (III, p. 6, prop. 3).

#### Théorème 2 {#top-v-s3-thm-2 .statement}

Un groupe connexe G, dans lequel il existe un voisinage ouvert de l’élément neutre homéomorphe à un intervalle ouvert de $\mathbf{R}$, est isomorphe à $\mathbf{R}$ ou à $\mathbf{T}$.

C’est une conséquence immédiate du théorème précédent, et de la prop. 7 de V, p. 5.

#### Remarque 1 {#top-v-s3-rem-1 .statement}

Pour décider si un groupe G, qui remplit les conditions du th. 2, est isomorphe à $\mathbf{T}$ ou isomorphe à $\mathbf{R}$, il suffit de voir si G est compact ou ne l’est pas.
2) Le th. 2 montre en particulier que tout groupe topologique homéomorphe au groupe $\mathbf{R}$ lui est nécessairement isomorphe.
3) La caractérisation topologique précédente des groupes $\mathbf{R}$ et $\mathbf{T}$ fait intervenir l’espace topologique $\mathbf{R}$ comme ensemble auxiliaire. Il est possible de caractériser les structures de groupe topologique de $\mathbf{R}$ et de $\mathbf{T}$ par des axiomes ne faisant intervenir aucun ensemble auxiliaire (voir V, p. 16 et 17, exerc. 4 et 6).

## EXERCICES {#top-v-s3-exercises}

See the [exercises for § 3](exercises/s3/).
