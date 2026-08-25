---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: III
chapter_title: GROUPES DE LIE
section: 10
section_title: Le groupe des automorphismes d’un groupe de Lie
lang: fr
source: lie-ii-iii-fr
pdf_pages: 0245-0253, 0282-0283
extraction: ocr
subsections:
    - "no": 1
      title: Automorphismes infinitésimaux
      page: 0
      pdf_page: 245
    - "no": 2
      title: Le groupe des automorphismes d’un groupe de Lie (cas réel ou complexe)
      page: 0
      pdf_page: 248
    - "no": 3
      title: Le groupe des automorphismes d’un groupe de Lie (cas ultramétrique)
      page: 0
      pdf_page: 253
statements: 13
exercises: 4
content_sha256: 956b529ef85064cc843a32820e15c73a67558f2abe228c65a85b4f2050a6a046
---

## § 10. Le groupe des automorphismes d’un groupe de Lie

Dans ce paragraphe, on suppose que K est de caractéristique zéro.

### 1. Automorphismes infinitésimaux

#### Lemme 1 {#lie-iii-s10-lem-1 .statement}

Soient G un groupe de Lie, α un champ de vecteurs sur G. Pour tout g ∈ G, soit β(g) = α(g)g⁻¹ ∈ L(G). Les conditions suivantes sont équivalentes:
(i) α est un homomorphisme du groupe G dans le groupe T(G);
(ii) quels que soient g, g′ dans G, on a α(gg′) = α(g)g′ + gα(g′);
(iii) quels que soient g, g′ dans G on a β(gg′) = β(g) + (Ad g)β(g′).

La condition (i) signifie que, quels que soient g, g′ dans G, on a dans le groupe T(G):
$$
\beta(g)g\beta(g')g' = \beta(gg')gg'
$$
ou
$$
\beta(g)((\mathrm{Ad}\ g)\beta(g'))gg' = \beta(gg')gg'.
$$
Or le produit de β(g) et de (Ad g)β(g′) dans T(G) n’est autre que la somme de β(g) et de (Ad g)β(g′) dans L(G) (§ 2, n° 1, prop. 2). Donc (i) ⇔ (iii). D’autre part, la condition (ii) s’écrit β(gg′)gg′ = β(g)gg′ + gβ(g′)g′, ou
$$
\beta(gg') = \beta(g) + (\mathrm{Ad}\ g)\beta(g'),
$$
donc (ii) ⇔ (iii).

#### Définition 1 {#lie-iii-s10-def-1 .statement}

Soit G un groupe de Lie. On appelle automorphisme infinitésimal de G tout champ de vecteurs analytique sur G vérifiant les conditions du lemme 1.

#### Lemme 2 {#lie-iii-s10-lem-2 .statement}

Soient K′ un sous-corps fermé non discret de K, A une K′-variété, B et C des K-variétés, f une application K′-analytique de A × B dans C. On suppose que, pour tout a ∈ A, l’application b ↦ f(a, b) de B dans C est K-analytique. Alors, pour tout t ∈ TA, l’application u ↦ (Tf)(t, u) de TB dans TC est K-analytique.

Fixons t ∈ TA, et posons g(u) = (Tf)(t, u). Il est clair que g est K′-analytique. D’après VAR, R, 5.14.6, il suffit de prouver que les applications tangentes à g sont K-linéaires. On peut supposer que A, B, C sont des voisinages ouverts de 0 dans des espaces normables complets E, F, G sur K′, K, K, et que t est tangent à A en 0. Identifions TA, TB, TC, à A × E, B × F, C × G et t à un élément de E. Alors pour tout (x, y) ∈ TB = B × F, on a
$$
g(x, y) = (f(0, x), (D_1f)(0, x)(t) + (D_2f)(0, x)(y)).
$$
Identifions T(B × F) à (B × F) × (F × F) et T(C × G) à (C × G) × (G × G).

Alors, pour tout $((x, y), (h, k)) \in T(B \times F) = (B \times F) \times (F \times F)$, on a $(Tg)((x, y), (h, k)) = ((a, b), (c, d))$, avec
$$
a = (f(0, x)),
b = (D_1 f)(0, x)(t) + (D_2 f)(0, x)(y), \quad c = (D_2 f)(0, x)(h),
d = (D_2 D_1 f)(0, x)(t, h) + (D_2 D_2 f)(0, x)(y, h) + (D_2 f)(0, x)(k).
$$
Fixons maintenant $(x, y) \in B \times F$. Il s’agit de prouver que l’application $(h, k) \mapsto (c, d)$ de $F \times F$ dans $G \times G$ est K-linéaire. Comme l’application $x \mapsto f(0, x)$ de B dans C est K-analytique, les applications
$$
(h, k) \mapsto (D_2 f)(0, x)(h), \quad (h, k) \mapsto (D_2 D_2 f)(0, x)(y, h),
(h, k) \mapsto (D_2 f)(0, x)(k)
$$
sont K-linéaires. D’autre part
$$
(D_2 D_1 f)(0, x)(t, h) = \lim_{\lambda \in K', \lambda \to 0} \lambda^{-1}((D_2 f)(\lambda t, x)(h) - (D_2 f)(0, x)(h))
$$
et, pour $\lambda$ fixé, l’application $x \mapsto f(\lambda t, x)$ est K-analytique, de sorte que l’application $h \mapsto (D_2 f)(\lambda t, x)(h)$ est K-linéaire.

#### Proposition 1 {#lie-iii-s10-prop-1 .statement}

*Soient K' un sous-corps fermé non discret de K, G un groupe de Lie sur K, V une variété sur K' et $(v, g) \mapsto vg$ une application K'-analytique de $V \times G$ dans G. On suppose que, pour tout $v \in V$, l’application $g \mapsto vg$ de G dans G soit un automorphisme de G. Soient $e$ un élément de V tel que $eg = g$ pour tout $g \in G$, et $a \in T_e(V)$. Alors le champ de vecteurs $g \mapsto ag$ sur G est un automorphisme infinitésimal de G.*

Pour $v \in V$, $g_1 \in G$, $g_2 \in G$, on a $v(g_1 g_2) = (vg_1)(vg_2)$. Donc, pour $u_1 \in TG$, $u_2 \in TG$, on a $a(u_1 u_2) = (au_1)(au_2)$ (\S 2, n° 1, prop. 3). En particulier, l’application $g \mapsto ag$ de G dans TG est un homomorphisme de groupes. D’autre part, cette application est analytique d’après le lemme 2.

#### Proposition 2 {#lie-iii-s10-prop-2 .statement}

*Soient G un groupe de Lie réel ou complexe, $\alpha$ un automorphisme infinitésimal de G. Il existe une loi d’opération analytique $(\lambda, g) \mapsto \varphi_\lambda(g)$ de K dans G possédant les propriétés suivantes:
1) si D est la loi d’opération infinitésimale associée, on a $D(1) = \alpha;$
2) pour tout $\lambda \in K$, on a $\varphi_\lambda \in \mathrm{Aut}\ G$.
a) Pour tout $\mu > 0$, soit $K_\mu$ la boule ouverte de centre 0 et de rayon $\mu$ dans K. Pour tout $g \in G$, soit $\mathcal{F}_g$ l’ensemble des courbes intégrales analytiques $f$ de $\alpha$ définies dans une boule $K_\mu$, et telles que $f(0) = g$. D’après VAR, R, 9.1.3 et 9.1.5, $\mathcal{F}_g$ est non vide, et deux éléments de $\mathcal{F}_g$ coïncident dans l’intersection de leurs domaines de définition; soit $\mu(g)$ la borne supérieure des nombres $\mu$ tels qu’il existe un élément de $\mathcal{F}_g$ défini dans $K_\mu$; il existe un élément unique de $\mathcal{F}_g$ défini dans $K_{\mu(g)}$; nous le noterons $f_g$.*

b) Soient $g_1, g_2$ dans $G$, $f_1 \in \mathcal{F}_{g_1}, f_2 \in \mathcal{F}_{g_2}$, avec $f_1$ et $f_2$ définies dans une même boule $K_\mu$. Alors $f_1 f_2 : K_\mu \to G$ est analytique, et $(f_1 f_2)(0) = g_1 g_2$. D’autre part, pour tout $\lambda \in K_\mu$, on a
$$
(T_\lambda(f_1 f_2))1 = (T_\lambda f_1)1 \cdot f_2(\lambda) + f_1(\lambda) \cdot (T_\lambda f_2)1 \quad (\S 2, \text{prop. 7})
$$
$$
= \alpha(f_1(\lambda)) f_2(\lambda) + f_1(\lambda) \alpha(f_2(\lambda))
$$
$$
= \alpha((f_1 f_2)(\lambda)) \tag{\text{lemme 1}}
$$
donc $f_1 f_2 \in \mathcal{F}_{g_1 g_2}$. Cela prouve que $\mu(g_1 g_2) \geq \inf (\mu(g_1), \mu(g_2))$.

c) D’après VAR, R, 9.1.4 et 9.1.5, il existe un voisinage $V$ de $e$ dans $G$ tel que $\sigma = \inf_{g \in V} \mu(g) > 0$. Soient $h \in G$ et $C$ sa composante connexe. Pour tout $h' \in C$, on a $\mu(h') \geq \inf (\sigma, \mu(h)) > 0$ d’après b). D’autre part, les fonctions $f_{h'}$, pour $h' \in C$, prennent leurs valeurs dans $C$. D’après VAR, R 9.1.4 et 9.1.5, on a $\mu = +\infty$ dans $C$, et finalement $\mu = +\infty$ dans $G$. Posons alors $f_g(\lambda) = \varphi_\lambda(g)$ pour tout $g \in G$ et tout $\lambda \in K$. D’après VAR, R, 9.1.4 et 9.1.5, l’application $(\lambda, g) \mapsto \varphi_\lambda(g)$ est une loi d’opération analytique de $K$ dans $G$. Il est clair que, si $D$ est la loi d’opération infinitésimale associée, on a $D(1) = \alpha$. D’après b), on a
$$
\varphi_\lambda(g_1 g_2) = \varphi_\lambda(g_1) \varphi_\lambda(g_2)
$$
quels que soient $\lambda \in K, g_1 \in G, g_2 \in G$.

#### Proposition 3 {#lie-iii-s10-prop-3 .statement}

*On suppose K ultramétrique. Soient G un groupe de Lie compact, $\alpha$ un automorphisme infinitésimal de G. Il existe un sous-groupe ouvert I de K et une loi d’opération analytique $(\lambda, g) \mapsto \varphi_\lambda(g)$ de I dans G possédant les propriétés suivantes:
1) *si D est la loi d’opération infinitésimale associée, on a $D(1) = \alpha$;
2) *pour tout $\lambda \in I$, on a $\varphi_\lambda \in \mathrm{Aut}\, G$.
Comme G est compact, il existe un sous-groupe ouvert I’ de K et une loi d’opération analytique $(\lambda, g) \mapsto \varphi_\lambda(g)$ de I’ dans G possédant la propriété 1 de la proposition (\S 4, n° 7, cor. 2 du th. 6). Posons $\varphi_\lambda(g) = f_g(\lambda)$ pour $\lambda \in I'$ et $g \in G$. On a, pour $g_1, g_2$ dans $G$ et $\lambda \in I'$,
$$
(T_\lambda(f_{g_1} f_{g_2}))1 = (T_\lambda f_{g_1})1 \cdot f_{g_2}(\lambda) + f_{g_1}(\lambda) \cdot (T_\lambda f_{g_2})1
$$
$$
= \alpha(f_{g_1}(\lambda)) f_{g_2}(\lambda) + f_{g_1}(\lambda) \alpha(f_{g_2}(\lambda))
$$
$$
= \alpha(f_{g_1}(\lambda) f_{g_2}(\lambda))
$$
et $(f_{g_1} f_{g_2})(0) = g_1 g_2 = f_{g_1 g_2}(0)$. Donc $f_{g'_1 g'_2}(\lambda) = f_{g'_1}(\lambda) f_{g'_2}(\lambda)$ pour $(g'_1, g'_2, \lambda)$ dans un voisinage de $(g_1, g_2, 0)$ (VAR, R, 9.1.8). Comme G est compact, il existe un sous-groupe ouvert I de I’ tel que $f_{g_1 g_2}(\lambda) = f_{g_1}(\lambda) f_{g_2}(\lambda)$ quels que soient $g_1 \in G, g_2 \in G, \lambda \in I$. Autrement dit, $\varphi_\lambda \in \mathrm{Aut}\, G$ pour $\lambda \in I$.

#### Lemme 3 {#lie-iii-s10-lem-3 .statement}

*Soient G et G’ des groupes de Lie, $\varphi$ un homomorphisme de G dans Aut (G’). Posons $f(g, g') = (\varphi(g))(g')$ pour $g \in G, g' \in G'$. Considérons les conditions suivantes:

(i) $f$ est analytique ;
(ii) $f$ est analytique dans un voisinage de $(e_G, e_{G'})$;
(iii) pour tout $g' \in G'$, l’application $g \mapsto f(g, g')$ est analytique.
Alors (i) $\Leftrightarrow ((\text{ii}) \text{ et } (\text{iii}))$. Si $G'$ est connexe, on a (i) $\Leftrightarrow$ (ii).
Il est clair que (i) implique (ii) et (iii). Soient $g_0 \in G, g'_0 \in G'$. Quels que soient $g \in G, g' \in G'$, on a
$$
f(gg_0, g'g'_0) = (\varphi(g)\varphi(g_0))(g'g'_0) = \varphi(g)(\varphi(g_0)g') \cdot \varphi(g)(\varphi(g_0)g'_0).
$$
Cela prouve l’implication ((ii) et (iii)) $\Rightarrow$ (i). Enfin, si $G'$ est connexe, $G'$ est engendré par tout voisinage de $e_{G'}$, donc (ii) $\Rightarrow$ (iii).

### 2. Le groupe des automorphismes d’un groupe de Lie (cas réel ou complexe)

Dans ce n°, on suppose $K = \mathbf{R}$ ou $\mathbf{C}$.

#### Lemme 4 {#lie-iii-s10-lem-4 .statement}

Soit $H$ un groupe de Lie simplement connexe de dimension finie.
(i) Pour tout $u \in \mathrm{Aut}\ L(H)$, soit $\theta(u)$ l’unique automorphisme de $H$ tel que $L(\theta(u)) = u$. Alors l’application $(u, g) \mapsto \theta(u)g$ de $(\mathrm{Aut}\ L(H)) \times H$ dans $H$ est analytique.
(ii) Soient $N$ un sous-groupe de Lie de $H$, et $\mathrm{Aut}(H, N)$ l’ensemble des $v \in \mathrm{Aut}\ H$ tels que $v(N) = N$. Alors $\theta^{-1}(\mathrm{Aut}(H, N))$ est un sous-groupe de Lie de $\mathrm{Aut}\ L(H)$.
(iii) Supposons $N$ distingué discret, de sorte que l’algèbre de Lie de $G = H/N$ s’identifie à $L(H)$. Pour tout $w \in \mathrm{Aut}\ G$, soit $\eta(w)$ l’unique automorphisme de $H$ tel que $L(\eta(w)) = L(w)$. Alors l’application $\eta$ est un isomorphisme du groupe $\mathrm{Aut}\ G$ sur le groupe $\mathrm{Aut}(H, N)$.

Pour prouver (i), il suffit, d’après le lemme 3 du n° 1, de vérifier que l’application $(u, g) \mapsto \theta(u)g$ est analytique dans un voisinage de $(\mathrm{Id}_{L(H)}, e)$. Il existe un voisinage ouvert $B$ de 0 dans $L(H)$ tel que $\psi = \exp_H|B$ soit un isomorphisme analytique de $B$ sur un voisinage ouvert de $e$ dans $H$. Il existe un voisinage ouvert $U$ de $\mathrm{Id}_{L(H)}$ dans $\mathrm{Aut}\ L(H)$, et un voisinage ouvert $B'$ de 0 dans $L(H)$, tels que $U(B') \subset B$. Alors l’application $(u, g) \mapsto \theta(u)g$ de $U \times \psi(B')$ dans $H$ est composée des applications suivantes:
l’application$(u, g) \mapsto (u, \psi^{-1}(g))$ de $U \times \psi(B')$ dans $U \times B'$;
l’application $(u, x) \mapsto u(x)$ de $U \times B'$ dans $B$;
l’application $y \mapsto \psi(y)$ de $B$ dans $G$.

Donc cette application est analytique.

Soit $p$ l’application canonique de $H$ dans l’espace homogène $H/N$. Alors $\theta^{-1}(\mathrm{Aut}\ (H, N))$ est l’ensemble des $u \in \mathrm{Aut}\ L(H)$ tels que
$$
p(\theta(u)g) = p(e), \qquad p(\theta(u^{-1})g) = p(e)
$$
pour tout $g \in N$. Compte tenu du § 8, n° 2, th. 2 et cor. 2 du th. 2, cela prouve (ii).

Supposons N distingué discret. Soit $w \in \mathrm{Aut}\ G$. On a
$$
L(p \circ \eta(w)) = L(\eta(w)) = L(w) = L(w \circ p)
$$
donc $p \circ \eta(w) = w \circ p$ et par suite $\eta(w) \in \mathrm{Aut}(H, N)$. Il est clair que l’application $\eta$ de $\mathrm{Aut}\ G$ dans $\mathrm{Aut}(H, N)$ est un homomorphisme injectif. Cet homomorphisme est surjectif parce que $p : H \to G$ est une submersion. C.Q.F.D.

Soient G un groupe localement compact, $\Gamma$ le groupe des automorphismes de G. Rappelons qu’on a défini sur $\Gamma$ la topologie $\mathcal{T}_\beta$ (TG, X, § 3, no 5). C’est la topologie la moins fine rendant continues les applications $v \mapsto v$ et $v \mapsto v^{-1}$ de $\Gamma$ dans $\mathcal{C}_c(G;G)$ (espace des applications continues de G dans G muni de la topologie de la convergence compacte). La topologie $\mathcal{T}_\beta$ est compatible avec la structure de groupe de $\Gamma$ (*loc. cit.*). Pour toute partie compacte L de G et tout voisinage U de $e_G$ dans G, soit $N(L, U)$ l’ensemble des $\varphi \in \Gamma$ tels que $\varphi(g) \in gU$ et $\varphi^{-1}(g) \in gU$ pour tout $g \in L$; alors les $N(L, U)$ forment un système fondamental de voisinages de $e_\Gamma$. Si G est engendré par une partie compacte C, la topologie $\mathcal{T}_\beta$ est aussi la topologie la moins fine pour laquelle les applications $v \mapsto v|C$ et $v \mapsto v^{-1}|C$ de $\Gamma$ dans $\mathcal{C}_u(C;G)$ soient continues (car toute partie compacte de G est contenue dans $(C \cup C^{-1})^n$ pour n assez grand). Si K est localement compact et si V est un espace vectoriel de dimension finie sur K, la topologie $\mathcal{T}_\beta$ sur $\mathbf{GL}(V)$ n’est autre que la topologie usuelle.

#### Théorème 1 {#lie-iii-s10-thm-1 .statement}

*Soient G un groupe de Lie de dimension finie, $G_0$ sa composante neutre. On suppose que G est engendré par $G_0$ et par un nombre fini d’éléments.*
(i) *Il existe sur Aut G une structure de variété analytique et une seule vérifiant la condition suivante:*
(AUT) *pour toute variété analytique M et toute application f de M dans Aut G, f est analytique si et seulement si l’application $(m, g) \mapsto f(m)g$ de $M \times G$ dans G est analytique.*
*On suppose dans la suite de l’énoncé Aut G muni de cette structure.*
(ii) *Aut G est un groupe de Lie de dimension finie.*
(iii) *Le morphisme $\varphi : u \mapsto L(u)$ de Aut G dans Aut L(G) est analytique.*
(iv) *Si G est connexe, $\varphi$ est un isomorphisme du groupe de Lie Aut G sur un sous-groupe de Lie de Aut L(G); ce sous-groupe de Lie est égal à Aut L(G) si G est simplement connexe.*
(v) *Soit a l’ensemble des automorphismes infinitésimaux de G. Alors a est une algèbre de Lie de champs de vecteurs, et la loi d’opération infinitésimale associée à l’application $(u, g) \mapsto u(g)$ de $(\mathrm{Aut}\ G) \times G$ dans G est un isomorphisme de $L(\mathrm{Aut}\ G)$ sur a.*
(vi) *La topologie du groupe de Lie Aut G est la topologie $\mathcal{T}_\beta$*.
a) L’unicité de la structure analytique envisagée dans (i) est évidente.
b) Supposons G connexe. Soient H le revêtement universel de G, $p$ le morphisme canonique de H sur G, et $N = \mathrm{Ker}\ p$. Introduisons les notations $\theta, \eta$ et

Aut(H, N) du lemme 4. Transportons à Aut H, grâce à θ, la structure de groupe de Lie de Aut L(G). Alors Aut H devient un groupe de Lie de dimension finie, et Aut(H, N) un sous-groupe de Lie de Aut H (lemme 4 (ii)). Transportons à Aut G, grâce à η⁻¹, la structure de groupe de Lie de Aut(H, N). Alors Aut G devient un groupe de Lie de dimension finie. Les propriétés (ii), (iii), (iv) du théorème sont vérifiées, et l’application (u, g) ↦ u(g) de (Aut G) × G dans G est analytique (lemme 4 (i)). Soient M une variété analytique, f une application de M dans Aut G, et φ l’application (m, g) ↦ f(m)g de M × G dans G. Il est clair que, si f est analytique, φ est analytique. Supposons φ analytique. Alors l’application Tφ : TM × TG → TG est analytique; sa restriction à M × L(G), c’est-à-dire l’application (m, x) ↦ L(f(m))x de M × L(G) dans L(G), est donc analytique; comme L(G) est de dimension finie, il en résulte que l’application m ↦ L(f(m)) de M dans Aut L(G) est analytique, donc que f est analytique. Ainsi, (i) est vérifié.

Munissons L(G) d’une norme. Pour tout λ > 0, soit B_λ la boule ouverte de centre 0 et de rayon λ dans L(G). Choisissons λ > 0 assez petit pour que ψ = exp_G|B_λ soit un isomorphisme de la variété analytique B_λ sur la sous-variété ouverte ψ(B_λ) de G. Soit Φ un filtre sur Aut G. Pour que Φ converge vers Id_G dans Aut G, il faut et il suffit que L(Φ) converge vers Id_{L(G)} dans Aut L(G), donc que L(Φ)|B_{λ/2} et L(Φ)⁻¹|B_{λ/2} convergent uniformément vers Id_{B_{λ/2}}. Cette condition entraîne que Φ|ψ(B_{λ/2}) et Φ⁻¹|ψ(B_{λ/2}) convergent uniformément vers Id_{ψ(B_{λ/2})}. Réciproquement, supposons que Φ|ψ(B_{λ/2}) converge uniformément vers Id_{ψ(B_{λ/2})}. Il existe un M ∈ Φ tel que, si u ∈ M, on ait u(ψ(B_{λ/2})) ⊂ ψ(B_{2λ/3}); alors L(u)(B_{λ/2}) est une partie connexe de L(G) dont l’image par exp_G est contenue dans ψ(B_{2λ/3}), donc L(u)(B_{λ/2}) ne rencontre pas B_λ − B_{2λ/3}, et par suite L(u)(B_{λ/2}) ⊂ B_λ; alors l’hypothèse que Φ|ψ(B_{λ/2}) converge uniformément vers Id_{ψ(B_{λ/2})} entraîne que L(Φ)|B_{λ/2} converge uniformément vers Id_{B_{λ/2}}. On déduit de là que:

(Φ converge vers Id_G dans Aut G) ⇔ (Φ converge vers Id_G pour 𝒯_β).

Cela prouve (vi).

Soit D la loi d’opération infinitésimale associée à la loi d’opération à gauche de Aut(G) dans G. D’après les prop. 1 et 2 du n° 1, on a D(L(Aut G)) = a. Donc a est une algèbre de Lie de champs de vecteurs et D est un morphisme de L(Aut G) sur a. Soient x₁ et x₂ des éléments de L(Aut G) tels que D(x₁) = D(x₂). Alors les lois d’opération (λ, g) ↦ (exp λx₁)g et (λ, g) ↦ (exp λx₂)g de K dans G ont même loi d’opération infinitésimale associée; donc, pour |λ| assez petit, exp λx₁ et exp λx₂ coïncident dans un voisinage de e (§ 4, n° 7, th. 6), d’où exp λx₁ = exp λx₂. On en déduit que x₁ = x₂, donc que D est un isomorphisme de L(Aut G) sur a.

Le théorème est ainsi entièrement démontré pour G connexe.

c) Passons au cas général. Par hypothèse, G est engendré par G₀ et un nombre fini d’éléments x₁, x₂, ..., xₙ. Tout u ∈ Aut G laisse stable G₀. Soit Aut₁ G l’ensemble des u ∈ Aut G qui, par passage au quotient, donnent l’automorphisme identique de $G/G_0$. C’est un sous-groupe distingué de Aut $G$. D’après la partie b) de la démonstration, Aut $G_0$ est canoniquement muni d’une structure de groupe de Lie, et l’application $(g_1, g_2, \ldots, g_n, u) \mapsto (u g_1, u g_2, \ldots, u g_n)$ de $G_0^n \times \mathrm{Aut}\ G_0$ dans $G_0^n$ est analytique. Soit $P$ le produit semi-direct correspondant de Aut $G_0$ par $G_0^n$; c’est un groupe de Lie ($\S 1$, n° 4, prop. 7), de dimension finie.

Si $w \in \mathrm{Aut}_1 G$, nous poserons
$$
w_0 = w|_{G_0} \in \mathrm{Aut}\ G_0 \\
w_i = x_i^{-1} w(x_i) \in G_0 \qquad (1 \leq i \leq n) \\
\zeta(w) = ((w_1, \ldots, w_n), w_0) \in P.
$$
Quels que soient $w, w'$ dans $\mathrm{Aut}_1 G$, on a
$$
\begin{align*}
\zeta(w) \zeta(w') &= ((w_1, \ldots, w_n)(w_0(w'_1), \ldots, w_0(w'_n)), w_0 w'_0) \\
&= ((w_1 w_0(w'_1), \ldots, w_n w_0(w'_n)), w_0 w'_0) \\
&= ((x_1^{-1} w(x_1) w(x_1^{-1} w'(x_1)), \ldots, x_n^{-1} w(x_n) w(x_n^{-1} w'(x_n))), w_0 w'_0) \\
&= (((w w w')_1, \ldots, (w w w')_n), (w w w')_0) \\
&= \zeta(w w w'),
\end{align*}
$$
donc $\zeta$ est un homomorphisme de $\mathrm{Aut}_1 G$ dans $P$. Cet homomorphisme est évidemment injectif.

Montrons que $\zeta(\mathrm{Aut}_1 G)$ est fermé dans $P$. Soit $\Phi$ un filtre sur $\mathrm{Aut}_1 G$ tel que $\zeta(\Phi)$ converge vers un point $((w_1, \ldots, w_n), w_0)$ de $P$. Alors $\Phi$ converge simplement vers une application $v$ de $G$ dans $G$. Il est clair que $v$ est un endomorphisme du groupe $G$. En outre, $v$ laisse stable chaque classe suivant $G_0$, et $v|_{G_0} = w_0$. Il en résulte que $v \in \mathrm{Aut}_1 G$. Comme $\zeta(v) = ((w_1, \ldots, w_n), w_0)$, on a bien montré que $\zeta(\mathrm{Aut}_1 G)$ est fermé dans $P$.

d) Dans la partie d) de la démonstration, on suppose que $K = \mathbf{R}$. D’après le $\S 8$, n° 2, th. 2, $\zeta(\mathrm{Aut}_1 G)$ est un sous-groupe de Lie de $P$. Transportons la structure de groupe de Lie réel de $\zeta(\mathrm{Aut}_1 G)$ à $\mathrm{Aut}_1 G$ grâce à $\zeta^{-1}$. Ainsi, $\mathrm{Aut}_1 G$ devient un groupe de Lie de dimension finie.

Soient $M$ une variété analytique, $f$ une application de $M$ dans $\mathrm{Aut}_1 G$, et $\varphi$ l’application $(m, g) \mapsto f(m) g$ de $M \times G$ dans $G$. On a les équivalences suivantes:
$f$ analytique
$$
\Leftrightarrow \text{les applications } m \mapsto (f(m))_i, \text{où } 0 \leq i \leq n, \text{ sont analytiques}
\Leftrightarrow \left\{\begin{array}{l}
\text{les applications } m \mapsto f(m)x_i \text{ de } M \text{ dans } G, \text{ pour } 1 \leq i \leq n, \text{ sont analytiques} \\
\text{et} \\
\text{l'application } (m, g) \mapsto f(m)g \text{ de } M \times G_0 \text{ dans } G \text{ est analytique}
\end{array}\right.
\Leftrightarrow \varphi \text{ est analytique.}
$$
Pour $w \in \mathrm{Aut}_1 G$, on a $L(w) = L(w_0)$, donc le morphisme $w \mapsto L(w)$ de $\mathrm{Aut}_1 G$ dans $\mathrm{Aut}\ L(G)$ est analytique. On voit comme dans b) que la loi d’opération infinitésimale associée à la loi d’opération de $\mathrm{Aut}_1 G$ dans $G$ est un isomorphisme de $L(\mathrm{Aut}_1 G)$ sur $a$.

Soit C une partie compacte de G_0 engendrant G_0. Pour qu’un filtre Φ converge vers Id_G dans Aut_1 G, il faut et il suffit que Φ|(C ∪ {x_1} ∪ … ∪ {x_n}) et Φ^{-1}|(C ∪ {x_1} ∪ … ∪ {x_n}) convergent uniformément vers

$$
\mathrm{Id}_G|(C \cup \{x_1\} \cup \ldots \cup \{x_n\}).
$$

La topologie de Aut_1 G est donc la topologie $\mathcal{T}_\beta$.

Il est clair que Aut_1 G est ouvert dans Aut G pour la topologie $\mathcal{T}_\beta$. Il existe sur Aut G une structure de groupe de Lie compatible avec cette topologie et induisant sur Aut_1 G la structure précédemment construite (\S 8, n° 1, cor. 2 du th. 1). Le fait que le groupe de Lie Aut G possède les propriétés du théorème résulte des propriétés correspondantes de Aut_1 G.

e) Dans la partie e) de la démonstration, on suppose que K = C. D’après c) et le th. 2 du \S 8, n° 2, il existe sur Aut_1 G une structure de groupe de Lie réel telle que $\zeta$ soit un isomorphisme de Aut_1 G sur un sous-groupe de Lie réel de P.

La loi d’opération $(w, g) \mapsto wg$ de $(\mathrm{Aut}_1 G) \times G$ dans G est analytique réelle. Soit D la loi d’opération infinitésimale associée. D’après les prop. 1 et 2 du n° 1, on a $D(\mathrm{L}(\mathrm{Aut}_1 G)) = \alpha$.

Pour tout $\alpha \in \alpha$, notons $\alpha_0$ la restriction de $\alpha$ à $G_0$; c’est un automorphisme infinitésimal de $G_0$ que nous identifions, grâce à la partie b) de la démonstration, à un élément de $\mathrm{L}(\mathrm{Aut}\ G_0)$. Pour $1 \leq i \leq n$, posons

$$
\alpha_i = x_i^{-1} \alpha(x_i) \in \mathrm{L}(G) = \mathrm{L}(G_0).
$$

Enfin, posons $f(\alpha) = ((\alpha_1, \ldots, \alpha_n), \alpha_0) \in \mathrm{L}(P)$. Alors $f$ est une application $\mathbf{C}$-linéaire de $\alpha$ dans $\mathrm{L}(P)$.

D’autre part, il est clair que $\mathrm{L}(\zeta) = f \circ D$. Donc $\mathrm{L}(\zeta)(\mathrm{L}(\mathrm{Aut}_1 G)) = f(\alpha)$ est un sous-espace vectoriel complexe de $\mathrm{L}(P)$. D’après la prop. 2 du \S 4, n° 2, $\zeta(\mathrm{Aut}_1 G)$ est un sous-groupe de Lie complexe de P, et on peut alors procéder exactement comme dans d) : on transporte la structure de groupe de Lie complexe de $\zeta(\mathrm{Aut}_1 G)$ à $\mathrm{Aut}_1 G$ grâce à $\zeta^{-1}$, et on voit comme dans d) que $\mathrm{Aut}_1 G$ possède les propriétés analogues aux propriétés (i), (ii), (iii), (v), (vi) du théorème.

Il est clair que $\mathrm{Aut}_1 G$ est ouvert dans Aut G pour la topologie $\mathcal{T}_\beta$. Soit $w \in \mathrm{Aut}\ G$. Soit $\sigma$ l’automorphisme $v \mapsto wvw^{-1}$ de $\mathrm{Aut}_1 G$. Il est analytique réel (\S 8, n° 1, th. 1), $\mathrm{L}(\sigma)$ est un $\mathbf{R}$-automorphisme de $\mathrm{L}(\mathrm{Aut}_1 G)$, et $D \circ \mathrm{L}(\mathrm{Aut}_1 G) \circ D^{-1}$ est un $\mathbf{R}$-automorphisme de $\alpha$. Cet automorphisme est aussi l’automorphisme de $\alpha$ déduit de $w$ par transport de structure; comme $w$ est K-analytique, on voit que $\mathrm{L}(\sigma)$ est K-linéaire. Donc $\sigma$ est K-analytique (\S 3, n° 8, prop. 32). D’après le \S 1, n° 9, prop. 18, il existe sur Aut G une structure de K-groupe de Lie et une seule telle que $\mathrm{Aut}_1 G$ soit un sous-groupe de Lie ouvert de Aut G. Le fait que cette structure possède les propriétés du théorème résulte des propriétés correspondantes de $\mathrm{Aut}_1 G$.

#### Corollaire 1 {#lie-iii-s10-thm-1-cor-1 .statement}

Soient G un groupe de Lie réel de dimension finie, $G_0$ sa composante neutre. On suppose que G est engendré par $G_0$ et par un nombre fini d’éléments. Alors Aut G, muni de la topologie $\mathcal{T}_\beta$, est un groupe de Lie réel de dimension finie.

#### Corollaire 2 {#lie-iii-s10-thm-1-cor-2 .statement}

Soit G un groupe de Lie réel ou complexe connexe semi-simple. Le groupe Int G est la composante neutre de Aut G.

L’application $u \mapsto L(u)$ est un isomorphisme de Aut G sur un sous-groupe de Lie de Aut L(G) (th. 1). L’image de Int G par cet isomorphisme est Ad G. Or Ad G est la composante neutre de Aut L(G) (\$ 9, n° 8, prop. 30 (ii)).

### 3. Le groupe des automorphismes d’un groupe de Lie (cas ultramétrique)

#### Théorème 2 {#lie-iii-s10-thm-2 .statement}

Lorsque K est ultramétrique localement compact et que G est un groupe de Lie compact, les assertions (i), (ii), (iii), (v), (vi) du th. 1 sont vraies.

a) L’unicité de la structure analytique envisagée dans (i) est évidente.

b) Supposons que G soit le groupe de Lie défini par une algèbre de Lie normée L. Ainsi, G est une boule ouverte et fermée dans L. Soit $w \in \mathrm{Aut}\, G$. Alors $L(w)$ coïncide avec $w$ au voisinage de 0. Soit $x \in G$. Soit $p$ la caractéristique du corps résiduel. Alors $p^n x$ tend vers 0 quand $n$ tend vers $+\infty$. Il existe donc $n$ tel que $w(p^n x) = L(w)(p^n x)$. Par suite
$$
p^n w(x) = w(x)^{p^n} = w(x^{p^n}) = w(p^n x)
= L(w)(p^n x) = p^n L(w)(x)
$$
d’où $w(x) = L(w)(x)$. Ainsi, $w = L(w)|G$.

Soit $\Gamma$ l’ensemble des $\gamma \in \mathrm{Aut}\, L(G)$ tels que $\gamma(G) = G$. Comme G est ouvert et compact dans $L(G)$, $\Gamma$ est un sous-groupe ouvert de $\mathrm{Aut}\, L(G)$. D’après ce qui précède, Aut G s’identifie à $\Gamma$, d’où une structure de groupe de Lie sur Aut G, pour laquelle les propriétés (i), (ii), (iii), (vi) du th. 1 sont évidentes. La propriété (v) résulte des prop. 1 et 3 du n° 1.

c) Passons au cas général. D’après le § 7, n° 1, prop. 1, il existe un sous-groupe ouvert et compact $G_0$ de G qui est du type envisagé en b). Alors G est engendré par $G_0$ et un nombre fini d’éléments $x_1, x_2, \ldots, x_n$. Soit $\mathrm{Aut}_1\, G$ l’ensemble des $u \in \mathrm{Aut}\, G$ tels que $u(G_0) = G_0,\ u(x_i G_0) = x_i G_0$ pour $1 \leq i \leq n$. On définit, comme dans la démonstration du th. 1, partie c), un produit semi-direct P de $\mathrm{Aut}\, G_0$ par $G_0^n$, et un homomorphisme injectif $\zeta$ de $\mathrm{Aut}_1\, G$ dans P, dont l’image est fermée dans P.

d), e) : on raisonne exactement comme dans les parties d), e) de la démonstration du th. 1, en remplaçant $\mathbf{R}$ par $\mathbf{Q}_p$ et en utilisant la prop. 3 au lieu de la prop. 2.

#### Remarque {#lie-iii-s10-n3-rem-1 .statement}

Si $K = \mathbf{Q}_p$, et si le groupe de Lie G est engendré par une partie compacte (cf. exerc. 2), les assertions (i), (ii), (iii), (vi) du th. 1 sont encore vraies, mais non (v) (exerc. 3).

## EXERCICES {#lie-iii-s10-exercises}

See the [exercises for § 10](exercises/s10/).
