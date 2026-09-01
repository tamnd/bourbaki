---
book: fvr
book_title: Functions of a Real Variable
chapter: VI
chapter_title: DÉVELOPPEMENTS TAYLORIENS GÉNÉRALISÉS. FORMULE SOMMATOIRE D’EULER–MACLAURIN
section: 2
section_title: Développements eulériens des fonctions trigonométriques et nombres de Bernoulli
lang: fr
source: fvr-i-vii-fr
book_pages: FVR VI.15-FVR VI.19
pdf_pages: 0275-0279, 0282-0286
extraction: ocr
subsections:
    - "no": 1
      title: Développement eulérien de cotg $z$
      page: 15
      pdf_page: 275
    - "no": 2
      title: Développement eulérien de $\sin z$
      page: 0
      pdf_page: 277
    - "no": 3
      title: Application aux nombres de Bernoulli
      page: 18
      pdf_page: 278
statements: 5
exercises: 13
content_sha256: 0bc69bdf523bffce7bc0ae16da246f1177336809deee44729b847c6ace2ac8dd
---

## § 2. DÉVELOPPEMENTS EULÉRIENS DES FONCTIONS TRIGONOMÉTRIQUES ET NOMBRES DE BERNOULLI

### 1. Développement eulérien de cotg $z$

D’après la formule (20) de VI, p. 7, les nombres $b_n/n!$ sont les coefficients du développement en série *formelle* de $S/(e^z - 1)$; nous allons démontrer dans ce paragraphe que la fonction $z/(e^z - 1)$ est égale à la somme d’une série entière absolument convergente dans un voisinage de 0 dans $\mathbf{C}$; il résultera du lemme de VI, p. 12, que les coefficients de cette série seront les nombres $b_n/n!$, d’où nous déduirons des majorations pour les nombres de Bernoulli $b_n$.

Notons en premier lieu qu’on a

$$
\frac{z}{e^z - 1} = -\frac{z}{2} + \frac{z}{2}\frac{e^z + 1}{e^z - 1} = -\frac{z}{2} + \frac{iz}{2} \cotg \frac{iz}{2}
$$

Nous allons obtenir dans ce qui suit un développement en série de cotg $z$, valable pour tout $z$ distinct d’un multiple entier de $\pi$.

#### Proposition 1 {#fvr-vi-s2-prop-1 .statement}

*Pour tout nombre complexe z et tout entier n, on a*

$$
\sin nz = 2^{n-1} \sin z \sin \left(z + \frac{\pi}{n}\right) \sin \left(z + \frac{2\pi}{n}\right) \ldots \sin \left(z + \frac{(n-1)\pi}{n}\right).
$$

En effet, on peut écrire

$$
\sin nz = \frac{e^{niz} - e^{-niz}}{2i} = \frac{e^{-niz}(e^{2niz} - 1)}{2i}
$$
$$
= \frac{e^{-niz}(e^{2iz} - 1)(e^{2iz} - e^{-2i\pi/n}) \ldots (e^{2iz} - e^{-2(n-1)i\pi/n})}{2i}
$$
$$
= A \sin z \sin \left(z + \frac{\pi}{n}\right) \ldots \sin \left(z + \frac{(n-1)\pi}{n}\right)
$$
avec
$$
A = (2i)^{n-1} e^{-\frac{in}{n}(1+2+\cdots+(n-1))} = (2i)^{n-1} e^{-i(n-1)\frac{n}{2}} = 2^{n-1}.
$$

#### Corollaire 1 {#fvr-vi-s2-prop-1-cor-1 .statement}

*Pour tout entier n, on a*

$$
\sin \frac{\pi}{n} \sin \frac{2\pi}{n} \ldots \sin \frac{(n-1)\pi}{n} = \frac{n}{2^{n-1}}.
$$

Il suffit en effet de diviser les deux membres de (2) par sin z et de faire tendre z vers 0.

#### Corollaire 2 {#fvr-vi-s2-prop-1-cor-2 .statement}

Pour tout entier impair $n = 2m + 1$, et tout nombre complexe $z$ tel que $nz$ ne soit pas multiple entier de $\pi$, on a

(4)
$$
\cotg nz = (-1)^m \cotg z \cotg \left( z + \frac{\pi}{n} \right) \ldots \cotg \left( z + \frac{(n-1)\pi}{n} \right).
$$

En effet, on a $\sin n \left( z + \frac{\pi}{2} \right) = \sin \left( nz + \frac{\pi}{2} + m\pi \right) = (-1)^m \cos nz$, d’où, en remplaçant $z$ par $z + \frac{\pi}{2}$ dans (2)

(5)
$$
\cos nz = (-1)^m 2^{n-1} \cos z \cos \left( z + \frac{\pi}{n} \right) \ldots \cos \left( z + \frac{(n-1)\pi}{n} \right)
$$
et les formules (2) et (5) donnent (4) par division membre à membre lorsque $\sin nz \neq 0$.

Dans tout ce qui suit, nous supposerons toujours que $n = 2m + 1$ est un entier impair; la formule (4) peut aussi s’écrire
$$
\cotg nz = (-1)^m \prod_{k=-m}^{m} \cotg \left( z - \frac{k\pi}{n} \right).
$$
Or, on a
$$
\cotg \left( z - \frac{k\pi}{n} \right) = \frac{1 + \tg z \tg \frac{k\pi}{n}}{\tg z - \tg \frac{k\pi}{n}}
$$
pour $\tg z$ fini; par rapport à $u = \tg z$, cotg $nz$ est donc une fraction rationnelle dont le numérateur est de degré $n - 1$ et dont le dénominateur, de degré $n$, a les $n$ racines simples $\tg k\pi/n$; en décomposant cette fraction en éléments simples, il vient
(6)
$$
\cotg nz = \sum_{k=-m}^{m} \frac{A_k}{u - \tg \frac{k\pi}{n}}
$$
avec
$$
A_k = \lim_{z \to k\pi/n} \cotg nz \cdot (\tg z - \tg \frac{k\pi}{n}) = \lim_{z \to k\pi/n} \frac{\cos nz}{\sin nz} \frac{\sin \left( z - \frac{k\pi}{n} \right)}{\cos z \cos \frac{k\pi}{n}}
$$
$$
= \lim_{h \to 0} \frac{\cos nh}{\cos \frac{k\pi}{n} \cos \left( h + \frac{k\pi}{n} \right)} \frac{\sin h}{\sin nh} = \frac{1}{n \cos^2 \frac{k\pi}{n}}
$$
d’où, en mettant à part dans (6) le terme correspondant à $k = 0$, en réunissant les termes correspondant à des valeurs opposées de $k$, et en remplaçant $z$ par $z/n$, (7) $$
\cotg z = \frac{1}{n \tg \frac{z}{n}} + \sum_{k=1}^{m} \frac{2n \tg \frac{z}{n}}{\cos^2 \frac{k \pi}{n} \left(n \tg \frac{z}{n}\right)^2 - \left(n \sin \frac{k \pi}{n}\right)^2}
$$
valable pour tout nombre complexe $z$ non multiple entier de $\pi/2$. On peut écrire cette formule sous la forme $\cotg z = \frac{1}{n \tg \frac{z}{n}} + \sum_{k=1}^{\infty} v_k(n, z)$ avec $v_k(n, z) = 0$ pour $k > m$ et
$$
v_k(n, z) = \frac{2n \tg \frac{z}{n}}{\cos^2 \frac{k \pi}{n} \left(n \tg \frac{z}{n}\right)^2 - \left(n \sin \frac{k \pi}{n}\right)^2}
$$
pour $1 \leq k \leq m$.

Nous allons voir que pour tout $z$ contenu dans une partie *compacte* $K$ de $\mathbf{C}$ ne contenant aucun multiple entier de $\pi$, et pour tout $n$ impair assez grand, la série de terme général $v_k(n, z)$ est *normalement convergente*. En effet, lorsque $n$ tend vers $+\infty$, $nt g \ z$ tend vers $\frac{z}{n}$ uniformément dans $K$, donc il existe un nombre $M > 0$ tel que $\left| n \tg \frac{z}{n} \right| \leq M$ pour tout entier $m$ assez grand et tout $z \in K$.

D'autre part, pour $0 \leq x \leq \pi/2$, on a $\sin x / x \geq 1 - \frac{x^2}{6} \geq \frac{1}{2}$, donc pour $1 \leq k \leq m$, on a $n \sin \frac{k \pi}{n} \geq k \pi / 2$; par suite, dès que $m$ est assez grand, pour tout entier $k$ tel que $k \pi / 2 > M$, on a $|v_k(n, z)| \leq \frac{8M}{k^2 \pi^2 - 4M^2}$, ce qui démontre notre assertion. Pour tout $k$ fixe, $v_k(n, z)$ tend (uniformément dans $K$) vers $\frac{2z}{z^2 - k^2 \pi^2}$ lorsque $n$ tend vers $+\infty$. Par suite:

#### Théorème 1 {#fvr-vi-s2-thm-1 .statement}

*Pour tout nombre complexe $z$ distinct d'un multiple entier de $\pi$, on a*
$$
\cotg z = \frac{1}{z} + \sum_{n=1}^{\infty} \frac{2z}{z^2 - n^2 \pi^2}
$$
*la série du second membre étant normalement convergente dans tout ensemble compact $K \subset \mathbf{C}$ ne contenant aucun multiple entier de $\pi$* (développement eulérien de $\cotg z$).

### 2. Développement eulérien de $\sin z$

Pour tout entier *impair* $n = 2m + 1$ et tout $z$ complexe, la formule (2) de VI, p. 15, peut s'écrire
$$
\sin nz = (-1)^m 2^{n-1} \prod_{k=-m}^{m} \sin \left(z - \frac{k \pi}{n}\right)
$$
$$
= (-1)^m 2^{n-1} \sin z \prod_{k=1}^{m} \sin \left(z - \frac{k \pi}{n}\right) \sin \left(z + \frac{k \pi}{n}\right).
$$

Or, on a $\sin\left(z - \frac{k\pi}{n}\right) \sin\left(z + \frac{k\pi}{n}\right) = \sin^2 z - \sin^2 \frac{k\pi}{n}$, et, d’après (3) (VI, p. 15)
$$
\prod_{k=1}^{m} \sin^2 \frac{k\pi}{n} = \frac{n}{2^{n-1}},
$$
d’où, en remplaçant $z$ par $z/n$

(9)
$$
\sin z = n \sin \frac{z}{n} \prod_{k=1}^{m} \left(1 - \frac{\sin^2 \frac{z}{n}}{\sin^2 \frac{k\pi}{n}}\right).
$$

On peut écrire cette formule $\sin z = n \sin \frac{z}{n} \prod_{k=1}^{m} (1 - w_k(n, z))$, avec $w_k(n, z) = 0$
pour $k > m$, et $w_k(n, z) = \frac{\sin^2 \frac{z}{n}}{\sin^2 \frac{k\pi}{n}}$ pour $1 \leq k \leq m$. Nous allons voir que pour tout $z$ contenu dans une partie compacte $K$ de $\mathbf{C}$ et pour tout $n$ impair, la série de terme général $w_k(n, z)$ est normalement convergente. En effet, lorsque $n$ tend vers $+\infty$, $n \sin \frac{z}{n}$ tend uniformément vers $z$ dans $K$, donc il existe $M > 0$ tels que
$$
\left| n \sin \frac{z}{n} \right| \leq M \text{ pour tout entier } m \text{ et tout } z \in K.
$$
Nous avons vu d’ailleurs dans la démonstration du th. 1 de VI p. 17, que pour $1 \leq k \leq m$ on a $n \sin \frac{k\pi}{n} \geq \frac{k\pi}{2}$; donc, pour tout entier $k$ tel que $k\pi/2 \geq M$, on a $|w_k(n, z)| \leq 4M^2/k^2\pi^2$, ce qui démontre notre assertion. Comme pour tout $k$ fixe, $w_k(n, z)$ tend (uniformément dans $K$) vers $z^2/k^2\pi^2$ lorsque $n$ tend vers $+\infty$, on voit que:

#### Théorème 2 {#fvr-vi-s2-thm-2 .statement}

*Pour tout nombre complexe $z$, on a*
$$
\sin z = z \prod_{n=1}^{\infty} \left(1 - \frac{z^2}{n^2\pi^2}\right)
$$
*le produit infini du second membre étant absolument et uniformément convergent dans toute partie compacte de $\mathbf{C}$ (développement eulérien de $\sin z$).*

### 3. Application aux nombres de Bernoulli

Le th. 1 de VI, p. 17, montre que, pour $0 \leq x < \pi$, la série de terme général
$$
\frac{2x}{n^2\pi^2 - x^2} \geq 0
$$
est convergente. On peut d’autre part écrire, pour tout nombre complexe $z$ tel que $|z| < \pi$,
$$
\frac{2z}{n^2\pi^2 - z^2} = \frac{2z}{n^2\pi^2} \sum_{k=0}^{\infty} \frac{z^{2k}}{n^{2k}\pi^{2k}}
$$

la série du second membre étant absolument convergente. Nous allons en déduire que la série « double »

$$
\sum_{n=1}^{\infty} \sum_{k=1}^{\infty} \frac{-2z^{2k-1}}{n^{2k}\pi^{2k}}
$$

est absolument convergente dans le disque ouvert $|z| < \pi$, normalement convergente dans tout ensemble compact contenu dans ce disque, et a pour somme cotg $z - \frac{1}{z}$. En effet, pour $|z| \leq a < \pi$, la valeur absolue du terme général de (11) est au plus égale à $2a^{2k-1}/n^{2k}\pi^{2k}$, et la somme d’une nombre fini quelconque de termes $2a^{2k-1}/n^{2k}\pi^{2k}$ est inférieure au nombre fini $\sum_{n=1}^{\infty} \frac{2a}{n^{2}-a^{2}}$; en sommant d’abord par rapport à $k$, puis par rapport à $n$, on voit que la somme de la série (11) est égale à $\sum_{n=1}^{\infty} \frac{2z}{z^{2} - n^{2}\pi^{2}}$ ce qui démontre notre assertion.

Si maintenant on somme la série (11), d’abord par rapport à $n$, puis par rapport à $k$, on a l’identité (pour $|z| < \pi$)

$$
\cotg z - \frac{1}{z} = -2 \sum_{k=1}^{\infty} \frac{S_{2k}}{\pi^{2k}} z^{2k-1}
$$

où on a posé $S_{k} = \sum_{n=1}^{\infty} \frac{1}{n^{k}}$. D’après (1) (VI, p. 15), on a donc, pour $|z| < 2\pi$

$$
\frac{z}{e^{z} - 1} = 1 - \frac{z}{2} + \sum_{n=1}^{\infty} \frac{(-1)^{n-1} S_{2n}}{2^{2n-1}\pi^{2n}} z^{2n}
$$

d’où la formule

$$
b_{2n} = (-1)^{n-1}(2n!) \frac{2S_{2n}}{(2\pi)^{2n}} \text{ pour } n \geq 1,
$$

formule qui montre en particulier que les nombres $S_{2n}/\pi^{2n}$ sont rationnels. On a évidemment $S_{k+1} \leq S_{k}$, donc, pour tout $k$ entier $\geq 2$, on a $S_{k} \leq S_{2} = \pi^{2}/6 \leq 2$; on tire donc de (14) les inégalités suivantes pour les nombres de Bernoulli

$$
\frac{2(2n)!}{(2\pi)^{2n}} \leq |b_{2n}| \leq 4 \frac{(2n)!}{(2\pi)^{2n}} \text{ pour } n \geq 1.
$$

De ces inégalités on peut tirer une majoration du polynôme de Bernoulli $B_{n}(x) = \sum_{k=0}^{n} \binom{n}{k} b_{k} x^{n-k}$; en particulier, pour $0 \leq x \leq 1$, on a

$$
|B_{n}(x)| \leq 4 \sum_{k=0}^{n} \binom{n}{k} \frac{k!}{(2\pi)^{k}} = 4 \frac{n!}{(2\pi)^{n}} \sum_{k=0}^{n} \frac{(2\pi)^{k}}{k!} \leq 4e^{2\pi} \frac{n!}{(2\pi)^{n}}.
$$

## EXERCICES {#fvr-vi-s2-exercises}

See the [exercises for § 2](exercises/s2/).
