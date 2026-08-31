---
book: int
book_title: Integration
chapter: IX
chapter_title: MEASURES ON HAUSDORFF TOPOLOGICAL SPACES
section: 0
section_title: Historical Note
kind: historical
lang: en
source: int-vii-ix
pdf_pages: 0302-0332
extraction: ocr
statements: 0
exercises: 0
content_sha256: cd04ec4dcf226a6f8761a19af2c47284265ff59581d75e91925edf6075ac7933
---

# HISTORICAL NOTE

(N.B. — The Roman numerals refer to the bibliography at the end of this note.)

While the study of the connections between topology and measure theory goes back to the beginnings of the modern theory of functions of real variables, it is only very recently that integration in Hausdorff topological spaces has been thoroughly worked out in general fashion. Before setting out the history of the work that preceded the present synthesis, we review several stages in the evolution of the ideas regarding the relations between topology and measure.

For Lebesgue, it is only a question of integrating functions of one or several real variables. In 1913, Radon defined general measures on $\mathbf{R}^n$ and the corresponding integrals; this theory is exposed in detail in the book (I) of Ch. de la Vallée Poussin and rests, in constant fashion, on the topological properties of Euclidean spaces. A little later, in 1915, Fréchet defined in (II, a)) 'abstract' measures on a set equipped with a tribe, and the integrals with respect to these measures; he noted that one can establish in this way the principal results of the Lebesgue theory without the use of topological methods. He justified his undertaking with the following words, taken from the introduction of (II, b), first part): « Que par exemple dans l’espace à une infinité de coordonnées où diverses applications de l’Analyse avaient conduit à diverses définitions non équivalentes d’une suite convergente, on remplace une de ces définitions par une autre, rien ne sera changé dans les propriétés des familles et fonctions additives d’ensembles dans ces espaces ».(*) Fréchet’s investigations were completed by Carathéodory, to whom is due an important theorem on the extension of a set function to a measure. The beginning of the book of Saks (III) gives a condensed exposition of this point of view.

The discovery of Haar measure on locally compact groups (cf. the His-

(*) "While, for example, in the space with infinitely many coordinates where various applications of Analysis had led to various inequivalent definitions of convergent sequence, if one replaces one of these definitions by another, nothing will be changed in the properties of the families and additive functions of sets in these spaces."

torical Note for Chs. VII and VIII) and the numerous applications that it immediately received, then the works of Weil and Gelfand on Harmonic Analysis, led around 1940 to a profound modification of this point of view: in this kind of question, it is most convenient to regard a measure as a linear form on a space of continuous functions. This method obliges one to restrict oneself to compact or locally compact spaces, but this is not an inconvenience for nearly all of the applications: better yet, the introduction of Harmonic Analysis on $p$-adic groups and adèle groups by J. Tate and A. Weil has permitted a spectacular renewal of Analytic Number Theory.

It is from an entirely different direction that the need arises for enlarging this point of view by considering measures on non locally compact topological spaces: gradually, Probability Theory leads to the study of such spaces and furnishes numerous nontrivial examples. Perhaps the reason for the tardy influence of these developments on the theory of measure is to be found in the relative isolation of Probability Theory, which remained until recently on the fringes of the traditional mathematical disciplines.

Measures on spaces of sequences

One of the most highly developed branches of classical Probability Theory is that of limit theorems (law of large numbers, tendency towards the Gauss–Laplace law, ...); this concerns a deepening of the concept of statistical regularity manifested by phenomena that bring into play very large populations. The correct mathematical formulation of these problems requires the introduction of measures on sequence spaces; these spaces, which constitute the most obvious generalization of finite-dimensional spaces, were the subject of choice of investigations into 'General Analysis' undertaken around 1920 by Fréchet, Lévy, Lusin, ... . Nor is it fortuitous that Khintchine and Kolmogoroff, the creators of the new methods of Probability Theory, were both disciples of Lusin, and that Lévy very quickly oriented himself towards probabilistic problems: these constituted the touchstone of the new methods.

The first implicit intervention of a measure on a sequence space appeared in the work devoted by E. Borel in 1909 to countable probabilities (IV). A highly original idea of Borel consists in the application of the probabilistic results he had just obtained to the proof of properties possessed by the decimal expansion of almost every real number between 0 and 1. This application rests on the following fundamental remark: let us define every real number between 0 and 1 by the sequence of figures (or 'digits') in its expansion in a given base $q$ ($q \geqslant 2$); if one successively draws at random the various figures of a number $x$, independently of each other and with equal probability $1/q$ for $0, 1, \ldots, q - 1$, the probability that $x$ lies in an interval of $[0, 1[$ is equal to the length of that interval.

In 1923, Steinhaus (V) established these results rigorously and described the precise mathematical model for the infinite sequence of random drawings considered by Borel: for simplicity let us take $q = 2$ and denote by I the set with two elements $\{0, 1\}$; one equips I with the measure $\mu$ defined by $\mu(0) = \mu(1) = \frac{1}{2}$; the elements of the product space $I^{\mathbf{N}}$ are the sequences $\varepsilon = (\varepsilon(n))_{n \in \mathbf{N}}$ of numbers equal to 0 or 1, and the mapping $\varphi : \varepsilon \mapsto \sum_{n \geq 0} \varepsilon(n) \cdot 2^{-n-1}$ is, up to a countable set, a bijection of $I^{\mathbf{N}}$ onto the interval $[0, 1]$; moreover, $\varphi^{-1}$ transforms the Lebesgue measure on $[0, 1]$ into the measure P on $I^{\mathbf{N}}$ that is the product of the measures $\mu$ on each of the factors. Actually, Steinhaus did not have at his disposal a construction for product measures; he used the existence of the quasi-bijection $\varphi$ to construct the measure P on $I^{\mathbf{N}}$ starting from Lebesgue measure on $[0, 1]$, and then gave an axiomatic characterization of P. The isomorphism so obtained made it possible to translate the language of probability into that of measure and to apply the known theorems on the Lebesgue integral.

In the same work, Steinhaus considered the random series $\sum_{n \geq 0} \sigma_n \cdot a_n$, where the signs $\sigma_n = \pm 1$ are chosen at random independently of each other and with equal probability $\frac{1}{2}$; between 1928 and 1935, he studied numerous other random series. From their side, Paley, Wiener and Zygmund considered random Fourier series$^{(1)}$ of the form $\sum_{n = -\infty}^{\infty} a_n \exp(2\pi i(nt + \Phi_n))$; the 'amplitudes' $a_n$ are fixed, and the 'phases' $\Phi_n$ are independent random variables uniformly distributed on $[0, 1]$. While the analytic difficulties vary enormously from one of these problems to another, the translation in terms of measure theory is the same in all cases and represents an extension of the case treated by Borel and Steinhaus; it is a matter of constructing a measure on $\mathbf{R}^{\mathbf{N}}$ that is the product of a family of measures all identical to a same positive measure $\mu$ on $\mathbf{R}$ of mass 1; for example, the preceding random Fourier series correspond to the case that $\mu$ is the Lebesgue measure on $[0, 1]$.

To construct such product measures, two methods can be used. The first is a direct method, precisely exposed for the first time by Daniell (VI, a)) in 1918; it was rediscovered in 1934 by Jessen (VII), who made a detailed study of the case that $\mu$ is Lebesgue measure on $[0, 1]$. The second method is to seek artifices analogous to that of Steinhaus to reduce to Lebesgue measure on $[0, 1]$; this way of proceeding had the advantage of convenience

(1) For an account of random Fourier series, see the exposition of J. P. KAHANE in the Séminaire Bourbaki (No. 200, 12th year, 1959/60, Benjamin, New York).

so long as one did not have available a complete exposition of general measure theory, for it permitted using Lebesgue’s theorems without the need for new proofs.(2)

The theory of Brownian motion

This theory occupies a special position in contemporary scientific development, by the constant and fertile exchange between physical problems and ‘pure’ mathematics to which it bears witness. The study of Brownian motion, discovered in 1829 by the botanist Brown, had been conducted intensively in the 19th century by numerous physicists,(3) but the first satisfactory mathematical model was only invented by Einstein in 1905. In the simple case of a particle moving along a straight line, Einstein’s fundamental hypotheses may be formulated as follows: if $x(t)$ is the abscissa of the particle at the instant $t$, and if $t_0 < t_1 < \cdots < t_{n-1} < t_n$, the successive displacements $x(t_i) - x(t_{i-1})$ (for $1 \leq i \leq n$) are independent Gaussian random variables. This is not the place to evoke in detail the important experimental work of J. Perrin that motivated Einstein’s theory; for our purposes, we need only retain a remark of Perrin, according to which the observation of trajectories of Brownian motion irresistibly suggested to him the “mathematicians’ functions without derivative”. This remark was to be the initial spark for Wiener.

Quite another current of ideas has its origins in the kinetic theory of gases, developed between 1870 and 1900 by Boltzmann and Gibbs. Consider a gas formed by N molecules of mass $m$ at (absolute) temperature T, and denote by $\mathbf{v}_1, \ldots, \mathbf{v}_N$ the velocities of the N molecules of the gas; the kinetic energy of the system is equal to

$$
\frac{m}{2} (\mathbf{v}_1^2 + \cdots + \mathbf{v}_N^2) = 3NkT,
$$

where $k$ is Boltzmann’s constant. According to the ideas of Gibbs, the multitude of shocks between molecules does not allow the precise determination of the velocities of the molecules, and it is convenient to introduce a probability law $P$ on the sphere S of the space of dimension 3N defined by the equation (1). The ‘micro-canonical’ hypothesis consists in assuming

(2) Wiener also took care on numerous occasions (cf. for example (XI), Ch. IX) to show that the measure of Brownian motion is isomorphic to Lebesgue measure on $[0,1]$. The possibility of such artifices finds its explanation in a general theorem of von Neumann that gives an axiomatic characterization of the measures isomorphic to Lebesgue measure on $[0,1]$.

(3) A very lively account of this history may be found in the recent book of E. Nelson, Dynamical theories of Brownian motion, Mathematical Notes, Princeton, 1967.

that P is the measure on the sphere S with mass 1 invariant under rotation. Moreover, Maxwell’s law of velocities states that the law of probability of a component of the velocity of a molecule is a Gaussian measure with variance $2kT/m$ (§ 6, No. 5, *Remark 3*). Borel seems to have been the first to observe in 1914 that Maxwell’s law is a consequence of Gibbs’ hypotheses and the properties of the sphere when the number of molecules is very large. He considered a sphere S in a Euclidean space of large dimension and the measure P of mass 1 on S invariant under rotation; using the classical approximation methods based on Stirling’s formula, he showed that the projection of P on a coordinate axis is approximately Gaussian. These results were sharpened a little later by Gâteaux and Lévy (IX, *a*). Given an integer $m \geqslant 1$ and a number $r > 0$, denote by $S_{m,r}$ the set of sequences of the form $(x_1, \ldots, x_m, 0, 0, \ldots)$ with $x_1^2 + \cdots + x_m^2 = r^2$; also, denote by $\sigma_{m,r}$ the measure with mass 1 on $S_{m,r}$ invariant under rotation. Stated in modern language, the result of Gâteaux and Lévy is as follows: the sequence of measures $\sigma_{m,1}$ tends tightly to a unit mass at the origin $(0, 0, \ldots)$, and the sequence of measures $\sigma_{m, \sqrt{m}}$ tends tightly to a measure $\Gamma$ of the form

$$
d\Gamma(x_1, x_2, \ldots) = \prod_{n=1}^\infty d\gamma(x_n)
$$

($\gamma$ is the Gaussian measure on $\mathbf{R}$ with variance 1).

The preceding measure $\Gamma$ plays the role of a Gaussian measure in infinite dimensions. It seems indeed that Lévy had confusedly hoped to define in an intrinsic manner a Gaussian measure on every infinite-dimensional Hilbert space. In fact, as shown by Lévy and Wiener, the measure $\Gamma$ is invariant in a certain sense$^{(4)}$ under the automorphisms of $l^2$; unfortunately, the set $l^2$ of square-summable sequences $(x_1, x_2, \ldots, x_n, \ldots)$ has measure zero for $\Gamma$. It is now known that one must be content to have a Gaussian *promesure* on an infinite-dimensional Hilbert space.$^{(5)}$

We owe to Wiener the essential progress: if one does not have a reasonable Gaussian measure on an infinite-dimensional Hilbert space, one can construct by the operation of primitive a measure $w$ on a space of continuous functions starting from a Gaussian promeasure (cf. §6, No. 7, Th. 1 for the details). We shall explain succinctly Wiener’s original construction of $w$ (X); it is directly influenced by the relation $\Gamma = \lim_{m \to \infty} \sigma_{m, \sqrt{m}}$ of Gâteaux and Lévy. For every integer $m \geqslant 1$, denote by $H_m$ the set of functions on $T = ]0, 1]$ that are constant on each of the intervals $\left[ \frac{k-1}{m}, \frac{k}{m} \right]$ (for $k = 1, 2, \ldots, m$), and by $\pi_m$ the measure of mass 1, invariant under rotation, on the Euclidean sphere of radius 1 in $\mathbf{R}^m$. Let $f_m$ be the isomorphism of $H_m$ onto $\mathbf{R}^m$ that associates, to each function taking the value $a_k$ on the interval $\left[ \frac{k-1}{m}, \frac{k}{m} \right]$, the vector $(a_1, a_2 - a_1, \ldots, a_m - a_{m-1})$ (whence the term ‘differential space’ dear to Wiener); denote by $w_m$ the measure on $H_m$ that is the image of $\pi_m$ under $f_m^{-1}$. Wiener defined the desired measure $w$ as the limit of the measures $w_m$. To be precise, let us denote by $H$ the set of regulated functions on $T$, with the topology of uniform convergence (we have $H_m \subset H$ for every integer $m \geqslant 1$); for every bounded uniformly continuous function $F$ on $H$, the limit $A\{F\} = \lim_{m \to \infty} \int_{H_m} F(x) \, dw_m(x)$ exists; next, Wiener obtained certain upper bounds by a subtle analysis of the fluctuations of the game of heads-or-tails, and taking up again the compactness arguments highlighted by Daniell, he showed that one is under the conditions for applying Daniell’s extension theorem. One concludes the existence of a measure $w$ carried by $\mathcal{C}(T)$ and such that $A\{F\} = \int_{\mathcal{C}(T)} F(x) \, dw(x)$. Wiener was then able to show that the measure $w$ corresponds to Einstein’s hypotheses,(6) and his estimates allowed him to give a precise meaning to Perrin’s remark on functions without derivatives: the set of functions satisfying a Lipschitz condition of order $\frac{1}{2}$ is negligible for $w$ (however, for every $a$ with $0 < a < \frac{1}{2}$, almost every function satisfies a Lipschitz condition of order $a$).


(4) More precisely, one has the following result. Let $U$ be an automorphism of the Hilbert space $l^2$, and $(u_{mn})$ the matrix of $U$. Let E be the vector space of all real sequences $(x_n)_{n \geqslant 1}$ and F the subspace of E formed by the sequences $(x_n)_{n \geqslant 1}$ for which the series $\sum_{n \geqslant 1} u_{mn} x_n$ converges for every $m \geqslant 1$. The formula $(\widetilde{U}x)_m = \sum_{n \geqslant 1} u_{mn} x_n$ defines a linear mapping $\widetilde{U}$ of F into E, the measure $\Gamma$ is concentrated on F, and $\widetilde{U}(\Gamma) = \Gamma$.

(5) This concept was introduced under the name “weak canonical distribution” by I. E. Segal (*Trans. Amer. Math. Soc.* **88** (1958), 12–42). One owes to this author a detailed study of Gaussian promeasures, and their application to certain problems in the quantum theory of fields.

Today, numerous constructions of the Wiener measure are known. Thus, Paley and Wiener use random Fourier series (XI, Ch. IX): for every real

(6) This may be translated by the formula
$$
\int_{\mathcal{C}(T)} f(x(t_1), \ldots, x(t_n)) \, dw(x) =
(2\pi)^{-n/2} \prod_{i=1}^n (t_i - t_{i-1})^{-1/2} \int \cdots \int f(x_1, \ldots, x_n) \exp \left( -\frac{1}{2} \sum_{i=1}^n \frac{(x_i - x_{i-1})^2}{t_i - t_{i-1}} \right) dx_1 \cdots dx_n,
$$
where $f$ is an arbitrary bounded continuous function on $\mathbf{R}^n$ and where $0 = t_0 < t_1 < \cdots < t_n \leqslant 1$ (one makes the convention $x_0 = 0$). Wiener, trained in analytical rigor by Hardy, and justly mistrustful of the foundations of Probability Theory at that time, was careful not to use probabilistic terminology or results. It follows that his memoirs are full of formidable formulas of which the foregoing is a sample; this circumstance is one of the factors that delayed the diffusion of Wiener’s ideas.

sequence $\mathbf{a} = (a_n)_{n \geq 1}$ and every integer $m \geq 0$, let us define the function $f_{m,\mathbf{a}}$ on $]0,1]$ by

$$
f_{m,\mathbf{a}}(t) = a_1 t + 2 \sum_{k=2}^{2^{m+1}} \frac{1}{\pi k} a_{k-1} \sin \pi kt;
$$

one can show that for $\Gamma$-almost every sequence $\mathbf{a}$, the sequence of functions $f_{m,\mathbf{a}}$ tends to a continuous function $f_\mathbf{a}$, and that $w$ is the image of $\Gamma$ under the mapping (defined almost everywhere) $\mathbf{a} \mapsto f_\mathbf{a}$. Later on, Lévy gave in (IX, b), c)) a construction very near to that which we have exposed in §6, No. 7. Finally, Kac, Donsker and Erdös showed around 1950 how to replace the spherical measures $\pi_m$ on $\mathbf{R}^m$ in Wiener’s original construction by more general measures. Their results establish a solid link between Wiener measure and the limit theorems of Probability Theory; they were to be completed and systematized by Prokhorov (XIII) in a work to which we shall return later on.

This is not the place to analyze the numerous and important probabilistic works brought about by Wiener’s discovery; nowadays, Brownian motion appears only as one of the most important examples of a Markoff process. We shall only mention Kac’s application of Wiener measure to the solution of certain parabolic partial differential equations; this is a question of adapting ideas of Feynmann in quantum field theory—yet another example of the reciprocal influence of mathematics and problems of physics.

Inverse limits of measures

This is a theory that has developed mainly in response to the needs of Probability Theory. Problems concerning a finite sequence of random variables $X_1, \ldots, X_n$ are in principle solved when one knows the law $P_X$ of the sequence: this is a positive measure on $\mathbf{R}^n$ of mass 1 such that the probability of obtaining simultaneously the inequalities $a_1 \leq X_1 \leq b_1, \ldots, a_n \leq X_n \leq b_n$ is equal to $P_X(C)$, where $C$ is the closed box $[a_1, b_1] \times \cdots \times [a_n, b_n]$ in $\mathbf{R}^n$. In practice, the measure $P_X$ either has discrete support or admits a density with respect to Lebesgue measure. When dealing with an infinite sequence $(X_n)_{n \geq 1}$ of random variables, one generally knows the law $P_n$ of the partial sequence $(X_1, \ldots, X_n)$ for every integer $n \geq 1$; these data satisfy a compatibility condition that expresses that the sequence $(P_n)_{n \geq 1}$ is an inverse system (or ‘projective system’) of measures. Until about 1920, the probabilities of events relating to the infinite sequence were defined in more or less implicit fashion by ‘natural’ passages to the limit from the probabilities of the finite case; one thus assumes that the probability that a game terminates is the limit, as $n$ tends to infinity, of the probability that it terminates in at most $n$ steps. Naturally, such a theory is not very coherent, and nothing excludes the presence of 'paradoxes', the same probability receiving two distinct estimates according as one evaluates by means of one or the other of two procedures, each as 'natural' as the other.

Steinhaus (V) appears to have been the first to have felt the need for considering (for the game of heads-or-tails) not only the inverse system $(P_n)_{n \geq 1}$ but its limit as well. A little earlier, in 1919, Daniell (VI, $b$) had proved in general the existence of such inverse limits,$^{(7)}$ but this result seems to have remained unknown in Europe. It was rediscovered in 1933 by Kolmogoroff in the work (XII) where the author formulates the axiomatic conception of Probability Theory. The proofs of Daniell and Kolmogoroff make use of a compactness argument, which is substantially the same as the one we have employed in Th. 2 of §4, No. 3 and which rests on Dini's theorem.

The Daniell–Kolmogoroff theorem left nothing to be desired for the case of random sequences $(X_n)_{n \geq 1}$, but the study of random functions undertaken from 1935 on by Kolmogoroff, Feller and Doob harbors difficulties of quite another order. Consider for example an interval $T$ of $\mathbf{R}$, representing the set of instants of observation of a 'stochastic process'; the set of possible trajectories is the product space $\mathbf{R}^T$, regarded as the inverse limit of the partial products $\mathbf{R}^H$, where $H$ runs over the set of finite subsets of $T$; one generally assumes given an inverse system of measures $(\mu_H)$ (cf. §4, No. 2). Kolmogoroff's theorem does indeed yield a measure on $\mathbf{R}^T$, but it is defined on a tribe notably smaller than the Borel tribe.$^{(8)}$ A variant of Kolmogoroff's construction, which yields a measure on a topological space, is due to Kakutani (*Proc. Imp. Acad. Tokyo* 19 (1943), 184–188), and has been rediscovered several times since: one regards $\mu_H$ as a measure on $\overline{\mathbf{R}}^H$ carried by $\mathbf{R}^H$;$^{(9)}$ the compact space $E = \overline{\mathbf{R}}^T$ is the inverse limit of the finite products $\overline{\mathbf{R}}^H$ and one can define a measure $\mu$ on $E$ as the inverse limit of the $\mu_H$ (cf. Ch. III, §4, No. 5). However, this procedure has a serious inconvenience; the elements of $\overline{\mathbf{R}}^T$ possess no regularity property that permits advancing the probabilistic study of the process—or even simply eliminating the parasitic values $\pm \infty$ introduced by the compactification $\overline{\mathbf{R}}$ of $\mathbf{R}$. This can be remedied by inducing the measure $\mu$ of $\overline{\mathbf{R}}^T$ on a particular subspace (for example $\mathcal{C}(T)$ in the case of Brownian motion); the fundamental difficulty arises from the fact that a function space, even one of the usual type, is not necessarily $\mu$-measurable in $\overline{\mathbf{R}}^T$, and even the choice of function space may be questionable.$^{(10)}$


(7) Daniell treated the case of measures on a product $\prod_{n \geq 1} I_n$ of compact intervals of $\mathbf{R}$, but his method extends immediately to the case of an arbitrary product of compact spaces; this is essentially the method we have used in Ch. III, §4, No. 5.

(8) Kolmogoroff's measure is only defined for the Borel sets in $\mathbf{R}^T$ of the form $A \times \mathbf{R}^{T-D}$, where $D$ is a countable subset of $T$, and $A$ is a Borel subset of $\mathbf{R}^D$; because of this, Kolmogoroff's theorem for an arbitrary product $\mathbf{R}^T$ is an immediate consequence of the case of countable products.

(9) One could replace $\overline{\mathbf{R}}$ by any compact space containing $\mathbf{R}$ as a dense subspace.

A decisive step was taken in 1956 by Prokhorov in a work (XIII) that has had a determining influence on the theory of stochastic processes. By putting into a suitable axiomatic form the methods used by Wiener in the article analyzed above, he established a general existence theorem for inverse limits of measures on function spaces that is a special case of Th. 1 of §4, No. 2 corresponding to Polish spaces.

A more restricted class of inverse systems was introduced by Bochner (XIV) in 1947; these are inverse systems formed by finite-dimensional real vector spaces and surjective linear mappings. The inverse limit of such a system may be identified in a natural way with the algebraic dual $E^*$ of a real vector space $E$, equipped with the weak topology $\sigma(E^*, E)$; a corresponding inverse system of measures has a limit that is a measure $\mu$ defined on a tribe notably smaller than the Borel tribe of $E^*$. Bochner completely characterized such 'promeasures' by their Fourier transform, which is a function on $E$. But this result is scarcely usable in the absence of a topology on $E$, in which case one has to examine the possibility of regarding $\mu$ as a measure on the topological dual $E'$ of $E$. In an independent way, R. Fortet and E. Mourier, while seeking to generalize to random variables with values in a Banach space certain classical results of Probability Theory (law of large numbers, central limit theorem) also brought into evidence the fundamental role played by the Fourier transformation in such questions. But substantial progress was not made until 1956 when Gelfand (XV, b)) suggested that the natural setting for the Fourier transformation is not that of Banach spaces or Hilbert spaces, but that of nuclear Fréchet spaces. He conjectured that every continuous function of positive type on such a space is the Fourier transform of a measure on its dual, a result established soon afterwards by Minlos (XVI). Its importance stems above all from the fact that it is applicable to spaces of distributions, and that the quasi-totality of function spaces are Borel subsets of the space of distributions (which thus constitutes a much better receptacle than $\mathbf{R}^T$).$^{(11)}$ The theory of random distributions is an area in full expansion, and we shall content ourselves by referring the

(10) For a detailed discussion of the problem of constructing measures on function spaces, and the methods used prior to Prokhorov, see J. L. DOOB, Bull. Amer. Math. Soc. 53 (1947), 15–30.
(11) One may consult the exposition of X. FERNIQUE, Ann. Inst. Fourier 17 (1967), 1–92, which also contains numerous results on tight convergence.

reader to the book of Gelfand and Vilenkin (XVII).

The results on inverse limits just mentioned make use of the existence of topologies on the base spaces. One may ask whether there exists an analogous theory in the case of 'abstract' measures. Von Neumann proved in 1935 the existence of product measures in all cases, but the discovery of a counter-example by Jessen and Andersen (XVIII) dashed the hope that every inverse system of measures admits a limit. Two palliatives have been discovered: in 1949, C. Ionescu-Tulcea established the existence of countable inverse limits, by means of the existence of suitable disintegrations,(12) a highly interesting result for the study of Markoff processes; moreover, it had been observed that the topology of the spaces only intervenes through the intermediary of the set of compact subsets. It was therefore natural to try to axiomatize this situation within the abstract theory, by means of the concept of compact class of subsets of a set. This work was done in 1953 by Marczewski (who established an abstract inverse limit theorem by such means) and Ryll-Nardzewski (who treated the disintegration of measures).(13)

Measures on general topological spaces and tight convergence

The study of the connections between topology and measure theory has above all been conceived of as the study of regularity properties of measures, and in particular that of 'outer' regularity and of 'inner' regularity;(14) inner regularity is equivalent to outer regularity on a locally compact space countable at infinity. The construction that Lebesgue gives to the measure of subsets of the line highlights these two kinds of regularity, and the outer regularity property of measures on a Polish space seems to have had public notoriety around 1935. But it was not until 1940, in an article whose diffusion was retarded by the war, that A. D. Alexandroff (XIX) gave prominence to the role of inner regularity and showed that it is possessed by the measures on a Polish space; this result was rediscovered later by Prokhorov (XIII) and is often erroneously attributed to this author. It was not perceived until very recently that this property extends to Souslin spaces; because of this, the

(12) It seems that it is the absence of a satisfactory theory of disintegration that marks the limit of the theory of 'abstract' measures. This difficulty reappears in insistent fashion in Probability Theory in connection with conditional probabilities.
(13) For an exposition of this theory, one may consult J. PFANZAGL and W. PIERLO, Lecture Notes in Mathematics (Springer–Verlag), Vol. 16 (1966).
(14) An 'abstract' measure $\mu$ on the Borel tribe of a Hausdorff topological space is said to be outer regular if the measure of every Borel set is the infimum of the measures of the open sets that contain it; the measure $\mu$ is said to be inner regular if the measure of every Borel set is the supremum of the measures of its compact subsets.

importance of these spaces has increased greatly, even more so as it was realized that their theory could be worked out without any metrizability hypothesis, and that the quasi-totality of the function spaces were Souslin (most often, even Lusin).(15) These are the reasons that moved us to place the accent on inner regular measures in this chapter.

The definition of a mode of convergence (vague or tight) for measures is most conveniently done by putting the space of measures into duality with a space of continuous functions. Generalizing an old result of F. Riesz, A. A. Markoff established in 1938 a one-to-one correspondence between the positive functionals on $\mathcal{C}(X)$ and the regular measures on a compact space X. In the work (XIX) already cited, A. D. Alexandroff extends these results to the case of a completely regular space: he introduces a hierarchy in the set of positive linear forms on the space $\mathcal{C}^b(X)$ of bounded continuous functions on a completely regular space X,(16) he defines tight convergence of bounded measures and proves among others the following two theorems:

a) if X is Polish, the set of linear forms on $\mathcal{C}^b(X)$ corresponding to the measures is closed for the weak convergence of sequences;
b) if a sequence of bounded measures has a tight limit, 'no mass escapes at infinity' (this is a weak form of the converse of Prokhorov's theorem on tight convergence).

From this abundance of concepts and theorems, Prokhorov was able to extract the results important for the theory of stochastic processes, and to present them in a simple and striking form. In his great work of 1956 already cited (XIII), a large part is devoted to bounded positive measures on a Polish space; generalizing a construction of Lévy, he defines a metric on the set of positive measures of mass 1 that makes it a Polish space, and then establishes an important compactness criterion for tight convergence (cf. §5, No. 5, Th. 1). Independently of Prokhorov, Le Cam (XX) obtained a number of compactness results for the tight convergence of measures; he makes no metrizability hypothesis on the spaces he considers, and his results reduce to earlier theorems of Dieudonné in the locally compact case.

(15) To attempt to resolve certain probabilistic difficulties (specifically the relations between various notions of stochastic independence or dependence), a number of authors introduced restricted classes of 'abstract' measures: the 'perfect' spaces of Kolmogoroff-Gnedenko, the 'Lusin' spaces of Blackwell, the 'Lebesgue' spaces of Rokhlin. In fact (at least assuming a rather weak countability hypothesis), all of these definitions give characterizations of 'abstract' measures isomorphic to a bounded positive measure on a Souslin space. On this subject, one may consult the work cited in footnote (13).

(16) He distinguishes by decreasing order of generality between the $\sigma$-measures ('abstract' measures on the Borel tribe of X ), the $\tau$-measures (outer regular measures) and the taut measures (inner regular measures). When X is Polish, these three notions coincide. The terminology itself is due to McShane and Le Cam (XX). One can find an account of the works to which this classification has given rise in V. S. VARADARAJAN (Amer. Math. Soc. Transl. (2), 48, 161–228).

(I) Ch. de la Vallée Poussin, Intégrales de Lebesgue, Fonctions d’ensembles, Classes de Baire, Paris (Gauthier–Villars), 1st. edn., 1916; 2nd. edn., 1936.

(II) M. Fréchet: a) Sur l’intégrale d’une fonctionnelle étendue à un ensemble abstrait, Bull. Soc. Math. France, 43 (1915), pp. 248–265; b) Les familles et fonctions additives d’ensembles abstraits, Fund. Math., 4 (1923), pp. 329–365; ibid. 5 (1924), pp. 206–251.

(III) S. Saks, Theory of the Integral, 2nd. edn., New York (Stechert), 1937.

(IV) E. Borel, Les probabilités dénombrables et leurs applications arithmétiques, Rend. Circ. Math. Palermo, 27 (1909), pp. 247–271.

(V) H. Steinhaus, Les probabilités dénombrables et leur rapport à la théorie de la mesure, Fund. Math., 4 (1923), pp. 286–310.

(VI) P. J. Daniell: a) Integrals in an infinite number of dimensions, Ann. of Math., 20 (1918–19), pp. 281–288; b) Functions of limited variation in an infinite number of dimensions, ibid. 21 (1919–20), pp. 30–38.

(VII) B. Jessen, The theory of integration in a space of an infinite number of dimensions, Acta Math., 63 (1934), pp. 249–323.

(VIII) A. Einstein, Investigations on the Theory of the Brownian Movement, New York (Dover), 1956.

(IX) P. LÉVY: a) Leçons d’Analyse Fonctionnelle, Paris (Gauthier–Villars), 1922 (the second edition appeared in 1951 with the same publisher, under the title Problèmes concrets d’Analyse Fonctionnelle); b) Processus stochastiques et mouvement brownien, Paris (Gauthier–Villars), 1948; c) Le mouvement brownien, Mémor. Sci. Math., 126 (1954).

(X) N. WIENER, Differential space, J. Math. Phys. MIT, 2 (1923), pp. 131–174 (= Selecta, pp. 55–98, Cambridge (MIT Press), 1964).

(XI) R. E. A. C. PALEY and N. WIENER, Fourier transforms in the complex domain, Amer. Math. Soc. Colloq. Publ. No. 19, New York, 1934.

(XII) A. N. KOLMOGOROFF, Grundbegriffe der Wahrscheinlichkeitsrechnung, Berlin (Springer), 1933.

(XIII) Ju. V. PROKHOROV, Convergence of random processes and limit theorems in probability theory, Theor. Probability Appl., 1 (1956), pp. 156–214.

(XIV) S. BOCHNER, Harmonic Analysis and the Theory of Probability, Berkeley (University of California Press), 1960.

(XV) I. M. GELFAND: a) Generalized stochastic processes (in Russian), Dokl. Akad. Nauk SSSR, 100 (1955), pp. 853–856; b) Some problems of functional analysis (in Russian), Uspehi Mat. Nauk, 11 (1956), pp. 3–12 (= Amer. Math. Soc. Transl. (2), 16 (1960), pp. 315–324).

(XVI) R. A. MINLOS, Generalized random processes and their extension to a measure (in Russian), Trudy Moskov. Math. Obšč., 8 (1959), pp. 497–518 (= Selected translations in mathematical statistics and probability, III (19), pp. 291–313).

(XVII) I. M. GELFAND and N. Ya. VILENKIN, Generalized Functions, Vol. IV, New York (Academic Press), 1964 (English translation).

(XVIII) E. SPARRE-ANDERSSON and B. JESSEN, On the introduction of measures in infinite product sets, Dansk. Vid. Selbskab. Mat. Fys. Medd., 25 (1948), No. 4, pp. 1–7.

(XIX) A. D. ALEXANDROFF, Additive set functions in abstract spaces. I (Ch. 1), Mat. Sbornik, 8 (1940), pp. 307–348; II (Chs. 2 and 3), ibid., 9 (1941), pp. 563–628; III (Chs. 4 to 6), ibid., 13 (1943), pp. 169–238.

(XX) L. LE CAM, Convergence in distribution of stochastic processes, Univ. Cal. Publ. Statistics, No. 11 (1957), pp. 207–236.

Index of notations

Reference numbers indicate, in order, the chapter, section and subsection.

Chapter VII:

$\gamma_X(s) ,\ \gamma(s)$: VII, 1, 1.
$\gamma(s)f ,\ \gamma(s)\mu$ ($f$ a function, $\mu$ a measure): VII, 1, 1.
$d\mu(s^{-1}x)$: VII, 1, 1.
$\delta_X(s) ,\ \delta(s) ,\ \delta(s)f ,\ \delta(s)\mu ,\ d\mu(xs)$: VII, 1, 1.
$\check{f} ,\ \check{\mu} ,\ d\mu(x^{-1})$ ($f$ a function, $\mu$ a measure): VII, 1, 1.
$\Delta_G ,\ \Delta$: VII, 1, 3.
$\mathrm{mod}_G \varphi ,\ \mathrm{mod}\varphi$ ($\varphi$ an automorphism): VII, 1, 4.
$\mathbf{Z}_p$ ($p$ a prime number): VII, 1, 6.
$K^+$ ($K$ a field): VII, 1, 10.
$\mathrm{mod}_K a ,\ \mathrm{mod}\ a$ ($a$ an element of a locally compact field $K$): VII, 1, 10.
$\mathcal{H}^\chi(X) ,\ \mathcal{H}_+^\chi(X) ,\ \mathcal{H}^1(X) ,\ f^\chi ,\ f^1$ ($X$ a locally compact space in which a locally compact group $H$ operates, $\chi$ a continuous representation of $H$ in $\mathbf{R}_+^*$): VII, 2, 1.
$f^b$: VII, 2, 2.
$\lambda^\# ,\ \frac{\mu}{\beta} ,\ \mu/\beta$: VII, 2, 2.
$m^\#$ ($m$ a vectorial measure): VII, 2, 2.
$T_J ,\ T_1(n,K) ,\ T(n,K) ,\ T(n,K)^*$: VII, 3, 3.

Chapter VIII:

$*_{i=1}^n \mu_i ,\ *\varphi(\mu_i)_{1 \leq i \leq n} ,\ \mu_1 * \mu_2 * \cdots * \mu_n$: VIII, 1, 1.
$\gamma_\chi$: VIII, 2, 3 and VIII, 2, 4.
$\gamma_{\chi,p}$: VIII, 2, 5.
$U(\mu)$ ($U$ a representation of a locally compact group $G$, $\mu$ a measure on $G$): VIII, 2, 6.
$\mathcal{M}^\rho(G)$ ($G$ a locally compact group): VIII, 3, 1.
$\mu *^\beta f ,\ \mu * f$ ($\mu$ a measure, $f$ a function): VIII, 4, 1.
$\mathcal{L}(G)$ ($G$ a locally compact group): VIII, 4, 5.
$\mathcal{U}_s^\infty(G)$ ($G$ a locally compact group): VIII, 4, Exer. 21.

Chapter IX:

\mathcal{F}_+(T), \mathcal{F}_+, f_A, f^0: preliminary conventions.
\pi(p), p_A \text{ or } p|A: IX, 1, 1.
\mathcal{P}(T; \mathbf{C}), \mathcal{P}(T; \mathbf{R}), \mathcal{P}(T), \mathcal{P}_+(T): IX, 1, 2.
w^\bullet(f), \int^\bullet f dw, \int^\bullet f(t) dw(t): IX, 1, 2.
w^\bullet, w_K^\bullet: IX, 1, 2.
w^+, w^-, |w|: IX, 1, 2.
\mu(f), \mu(A): IX, 1, 5.
\operatorname{Supp}(\mu): IX, 1, 6.
\sum_{i \in I} \mu_i: IX, 1, 7.
\mu^*(f), \mu^*(A), \int^* f d\mu, \int^* f(t) d\mu(t): IX, 1, 9.
\mu^*: IX, 1, 9.
\overline{\mathcal{L}}^p(T, \mu), \overline{\mathcal{L}}_F^p(T, \mu), \mathcal{L}^p(T, \mu), \mathcal{L}_F^p(T, \mu) \text{ (for } 1 \leq p \leq +\infty): IX, 1, 10.
\overline{\mathcal{L}}_F^p(\mu), \overline{\mathcal{L}}_F^p, \overline{\mathcal{L}}^p, \overline{\mathcal{L}}^p(\mu), \mathcal{L}^p(\mu), \mathcal{L}^p: IX, 1, 10.
\overline{N}_p(f), N_p(f), \overline{\mathcal{N}}_F, \mathcal{N}_F: IX, 1, 10.
L_F^p(\mu), L_F^p: IX, 1, 10.
\int f d\mu, \mu(f), \int f(t) d\mu(t): IX, 1, 10.
\mu_X^\bullet, \mu_X, \mu|X: IX, 2, 1.
f \cdot \mu: IX, 2, 2.
\pi(\mu): IX, 2, 3.
\lambda \otimes \mu: IX, 2, 5.
\mathcal{K}(T), \mathcal{B}(T): conventions of §3.
\mathcal{C}^b(T; F), \mathcal{C}^b(T), \mathcal{C}^b, \mathcal{C}_+^b(T), \mathcal{C}_+^b: conventions of §5.
\mathcal{M}^b(T; \mathbf{C}), \mathcal{M}^b(T), \mathcal{M}^b, \mathcal{M}_+^b(T), \mathcal{M}_+^b: conventions of §5.
\mathcal{L}\mu: IX, 5, 7.
\mathcal{F}(E): IX, 6, 1.
p_V, p_{VW}: IX, 6, 1.
\mathcal{Q}(E): IX, 6, 1.
\tilde{\lambda}: IX, 6, 1.
u(\mu) (\mu \text{ a promeasure}): IX, 6, 2.
\mathcal{F}\mu (\mu \text{ a promeasure or a measure}): IX, 6, 3.
\Gamma_Q, \gamma_a: IX, 6, 5.
\gamma_C: IX, 6, 6.
\operatorname{Tr}(Q/H): IX, Annex, 1.
u^*: IX, Annex, 2.

Index of terminology

Reference numbers indicate, in order, the chapter, section and subsection (or, exceptionally, exercise).

Abstract measure, integral: IX, 3, Exer. 4.
Additive set function: IX, 3, 2.
Additive, countably (set function): IX, 3, 2.
Adjoint of a linear mapping: IX, Annex, 2.
Algebra, triangular (upper, lower): VII, 3, 3.
Almost everywhere: IX, 1, 9.
Associated promeasure, to a measure: IX, 6, 1.
Atomic gauge: IX, 3, Exer. 9.
Base $\mu$, measure with: IX, 2, 2.
Bochner’s theorem: IX, 6, 12.
Bounded encumbrance: IX, 1, 1.
Bounded measure: IX, 1, 2.
Bounded set function: IX, 3, 2.
Brunn–Minkowski inequality: VII, 1, Exer. 25.
Cardinal, strongly inaccessible: IX, 3, Exer. 13, footnote.
Cardinal, ulamian: IX, 3, Exer. 11.
Character of a monoid: IX, 5, 7.
Concentrated (encumbrance) on a subset: IX, 1, 1.
Concentrated (measure) on a subset: IX, 1, 4.
Continuous linear representation: VIII, 2, 1.
Contragredient (linear representation): VIII, 2, 2.
Convolution product of a finite sequence of measures: VIII, 1, 1.
Convolution product of functions: VIII, 4, 5.
Convolvable functions: VIII, 4, 5.
Convolvable measure and function: VIII, 4, 1.
Convolvable, $\varphi$-convolvable (finite sequence of measures): VIII, 1, 1.
Countably additive set function: IX, 3, 2.
Covariance matrix of a Gaussian measure: IX, 6, 6.
Covariance of a Gaussian promeasure on $\mathbf{R}^T$: IX, 6, 6.
Cramped set of bounded measures: VIII, 3, Exer. 10.

Crushing: IX, 1, 8.
Decomposition, Iwasawa’s, of $\mathbf{GL}(n, K)$: VII, 3, 3.
Density of a measure with respect to another: IX, 2, 2.
Diffuse gauge: IX, 3, Exer. 9.
Disintegration of a measure: IX, 2, 7.
Domain, fundamental: VII, 2, 10.
Encumbrance: IX, 1, 1.
Encumbrance, bounded: IX, 1, 1.
Encumbrance, concentrated on a subset: IX, 1, 1.
Encumbrance, image: IX, 1, 1.
Encumbrance, induced: IX, 1, 1.
Encumbrance, locally bounded: IX, 1, 1.
Equicontinuous linear representation: VIII, 2, 1.
Essential upper integral: IX, 1, 2.
Essentially bounded function: IX, 1, 10.
Essentially integrable function: IX, 1, 10.
Finite sequence, $\varphi$-convolvable, of measures: VIII, 1, 1.
Form, nuclear quadratic: IX, Annex, 1.
Full submonoid: IX, 5, 7.
Function of positive type: IX, 6, 12.
Function, essentially bounded: IX, 1, 10.
Function, essentially integrable: IX, 1, 10.
Function, generating (of a sequence): IX, 5, 7.
Function, integrable: IX, 1, 10.
Function, locally integrable: IX, 2, 2.
Function, locally negligible: IX, 1, 4.
Function, measurable: IX, 1, 5.
Function, moderated: IX, 1, 9.
Function, modular (of a locally compact group): VII, 1, 3.
Function, negligible: IX, 1, 9.
Function, universally measurable: IX, 2, 7.
Fundamental domain: VII, 2, 10.
G-covering: VII, 1, Exer. 27.
G-filling: VII, 1, Exer. 27.
G-paving: VII, 1, Exer. 27.
Gauge on a set X: IX, 3, Exer. 9.
Gaussian measure, promeasure: IX, 6, 5.
Gaussian measure with covariance matrix $C$: IX, 6, 6.
Gaussian promeasure with covariance K: IX, 6, 6.

Gaussian promeasure, canonical, on a real Hilbert space: IX, 6, 6.
General linear group: VII, 3, 3.
Generating function of a sequence: IX, 5, 7.
Group, large triangular (upper, lower): VII, 3, 3.
Group, special triangular (upper, lower): VII, 3, 3.
Group, strict triangular (upper, lower): VII, 3, 3.
Group, unimodular: VII, 1, 3.
Haar measure (left, right): VII, 1, 2.
Hilbert–Schmidt mapping: IX, Annex, 2.
Image of a measure: IX, 2, 3.
Image of a promeasure: IX, 6. 2.
Image of an encumbrance: IX, 1, 1.
Induced encumbrance: IX, 1, 1.
Induced measure: IX, 2, 1.
Inequality, Brunn–Minkowski: VII, 1, Exer. 25.
Inner regular set function: IX, 3, 2.
Integers, $p$-adic: VII, 1, 6.
Integrable function: IX, 1, 10.
Integrable set: IX, 1, 9.
Integral, abstract: IX, 3, Exer. 4.
Integral, essential upper: IX, 1, 2.
Integral, upper: IX, 1, 9.
Integral of a function: IX, 1, 10.
Invariant measure (left-, right-) on a group: VII, 1, 1.
Invariant measure, under a group of operators: VII, 1, 1.
Inverse (or projective) limit of measures on an inverse (or projective) limit of locally compact groups: VII, 1, 6.
Inverse (or projective) limit of measures: IX, 4, 2.
Inverse (or projective) system of measures: IX, 4, 2.
Isometric linear representation: VIII, 2, 1.
Iwasawa decomposition of $\mathbf{GL}(n, K)$: VII, 3, 3.
Kernel of positive type: IX, 6, 6.
Lagrange’s theorem: VII, 1, Exer. 29.
Laplace transformation: IX, 5, 7.
Large triangular group (upper, lower): VII, 3, 3.
Left Haar measure: VII, 1, 2.
Left multiplier, of a relatively invariant measure on a locally compact group: VII, 1, 8.
Left-invariant measure on a group: VII, 1, 1.

Levy, P., theorem of: IX, 5, Exer. 13.
Lifting of measures: IX, 2, 4.
Limit, inverse (or projective), of measures on an inverse (or projective) limit of locally compact groups: VII, 1, 6.
Limit, inverse (or projective), of measures: IX, 4, 2.
Linear representation, transposed, contragredient of a linear representation: VIII, 2, 2.
Locally almost everywhere: IX, 1, 4.
Locally bounded encumbrance: IX, 1, 1.
Locally bounded set function: IX, 3, 2.
Locally integrable function: IX, 2, 2.
Locally negligible function: IX, 1, 4.
Locally negligible set: IX, 1, 4.
Mapping, Hilbert–Schmidt: IX, Annex, 2.
Mapping, $\mu$-proper: IX, 2, 3.
Margins of a measure on a function space: IX, 4, 3.
Mass, total (of a promeasure): IX, 6, 1.
Mean, orbital: VII, 2, 2.
Measurable function: IX, 1, 5.
Measurable set: IX, 1, 5.
Measure: IX, 1, 2.
Measure, abstract: IX, 3, Exer. 4.
Measure on $\mathbf{Q}_p$, normalized Haar: VII, 1, 6.
Measure, bounded: IX, 1, 2.
Measure, Gaussian with covariance matrix $C$: IX, 6, 6.
Measure, Gaussian with variance $Q$: IX, 6, 5.
Measure, Haar (left, right), on a locally compact group: VII, 1, 2.
Measure, image: IX, 2, 3.
Measure, induced: IX, 2, 1.
Measure, invariant (relatively invariant, quasi-invariant) under a group of operators: VII, 1, 1.
Measure, left-invariant (right-invariant), on a locally compact group: VII, 1, 1.
Measure, lifting of: IX, 2, 4.
Measure, moderated: IX, 1, 9.
Measure, normalized Haar, on a compact group, on a discrete group: VII, 1, 3.
Measure, outer (of a set): IX, 1, 9.
Measure, product: IX, 2, 5.
Measure, quasi-invariant, on a locally compact group: VII, 1, 9.
Measure, relatively invariant, on a locally compact group: VII, 1, 8.

Measure, Wiener: IX, 6, 7.
Measure, with base $\mu$: IX, 2, 2.
Measure, with density $f$ with respect to a measure $\mu$: IX, 2, 2.
Measured space: IX, 6, 7, Footnote (2).
Minkowski’s theorem: VII, 1, Exer. 27.
Minlos’s theorem: IX, 6, 10.
Moderated function: IX, 1, 9.
Moderated measure: IX, 1, 9.
Moderated set: IX, 1, 9.
Modular function of a locally compact group: VII, 1, 3.
Modulus of a locally compact group: VII, 1, 3.
Modulus of an automorphism: VII, 1, 4.
Multiplier (left, right), of a relatively invariant measure on a locally compact group: VII, 1, 8.
Multiplier on a product $G \times X$ of a group $G$ and a set $X$ on which $G$ operates: VIII, 2, 3.
Multiplier, of a measure relatively invariant under a group of operators: VII, 1, 1.
Negligible function: IX, 1, 9.
Negligible set: IX, 1, 9.
Normalized Haar measure on a compact group, on a discrete group: VII, 1, 3.
Normalized Haar measure on $Q_p$: VII, 1, 6.
Nuclear quadratic form: IX, Annex, 1.
Nuclear space: IX, 6, 10.
Orbital mean: VII, 2, 2.
Outer measure: IX, 1, 9.
$p$-adic integers: VII, 1, 6.
Positive premeasure, measure: IX, 1, 2.
Positive type, function of: IX, 6, 12.
Positive type, kernel of: IX, 6, 6.
Premeasure: IX, 1, 2.
Premeasure, positive: IX, 1, 2.
Premeasure, real: IX, 1, 2.
Product of a family of measures: IX, 4, 3.
Product of two measures: IX, 2, 5.
Product, convolution (of a measure and a function): VIII, 4, 1.
Product, convolution (of functions): VIII, 4, 5.
Product, convolution (of measures), with respect to a mapping: VIII, 1, 1.
Projective (or inverse) limit of measures: IX, 4, 2.

Projective (or inverse) system of measures: IX, 4, 2.
Prokhorov’s conditions: IX, 4, 2 and IX, 5, 5.
Promeasure: IX, 6, 1.
Promeasure associated with a measure: IX, 6, 1.
Promeasure, canonical Gaussian, on a real Hilbert space: IX, 6, 6.
Promeasure, Fourier transform of: IX, 6, 3.
Promeasure, Gaussian with covariance K, on $\mathbf{R}^T$: IX, 6, 6.
Promeasure, Gaussian with variance Q: IX, 6, 5.
Promeasure, image: IX, 6, 2.
Promeasure, total mass of: IX, 6, 1.
Proper, $\mu$- (mapping): IX, 2, 3.
Quadratic form, nuclear: IX, Annex, 1.
Quasi-invariant measure on a locally compact group: VII, 1, 9.
Quasi-invariant measure, under a group of operators: VII, 1, 1.
Quotient of a measure on a locally compact space X by a Haar measure of a group operating on X: VII, 2, 2.
Radon space: IX, 3, 3.
Real measure, premeasure: IX, 1, 2.
Regular representation (left, right): VIII, 2, 5.
Regularization: VIII, 4, 7.
Relatively invariant measure, on a locally compact group: VII, 1, 8.
Relatively invariant measure, under a group of operators: VII, 1, 1.
Representation, continuous (separately continuous, equicontinuous, isometric): VIII, 2, 1.
Representation, regular (left, right): VIII, 2, 5.
Representation, unitary: VIII, 2, Exer. 4.
Right Haar measure: VII, 1, 2.
Right multiplier, of a relatively invariant measure on a locally compact group: VII, 1, 8.
Right-invariant measure on a group: VII, 1, 1.
Sazonov topology: IX, 6, 10.
Separately continuous (linear representation): VIII, 2, 1.
Set function, additive: IX, 3, 2.
Set function, bounded: IX, 3, 2.
Set function, countably additive: IX, 3, 2.
Set function, inner regular: IX, 3, 2.
Set function, locally bounded: IX, 3, 2.
Space, nuclear: IX, 6, 10.
Space, Radon: IX, 3, 3.

Space, strongly Radon: IX, 3, 3.
Special triangular group (upper, lower): VII, 3, 3.
Strict triangular group (upper, lower): VII, 3, 3.
Strongly inaccessible cardinal: IX, 3, Exer. 13, footnote.
Strongly Radon space: IX, 3, 3.
Sub-inverse (or sub-projective) system of measures: IX, 4, 2.
Submonoid, full: IX, 5, 7.
Sum of a family of measures: IX, 1, 7.
Summable family of measures: IX, 1, 7.
Support of a measure: IX, 1, 6.
System, inverse (or projective), of measures: IX, 4, 2.
System, sub-inverse (or sub-projective), of measures: IX, 4, 2.
Theorem, Bochner’s: IX, 6, 12.
Theorem, Lagrange’s: VII, 1, Exer. 29.
Theorem, Minkowski’s: VII, 1, Exer. 27.
Theorem, Minlos’s: IX, 6, 10.
Theorem, P. Lévy’s: IX, 5, Exer. 13.
Theorem, Thue’s: VII, 1, Exer. 28.
Thue’s theorem: VII, 1, Exer. 28.
Tight convergence, topology of: IX, 5, 3.
Tight topology: IX, 5, 3.
Topology, Sazonov’s: IX, 6, 10.
Topology, tight: IX, 5, 3.
Total mass of a promeasure: IX, 6, 1.
Trace of a quadratic form with respect to another: IX, Annex, 1.
Transform, Fourier (of a measure, of a promeasure): IX, 6, 3.
Transform, Laplace (of a measure): IX, 5, 7.
Transposed linear representation: VIII, 2, 2.
Triangular algebra: VII, 3, 3.
Triangular group (large, strict, special): VII, 3, 3.
Ulam cardinal: IX, 3, Exer. 11.
Ulam ultrafilter: IX, 3, Exer. 11.
Unimodular group: VII, 1, 3.
Unitary representation: VIII, 2, Exer. 4.
Universally measurable function: IX, 2, 7.
Universally measurable set: IX, 3, 3.
Upper integral: IX, 1, 9.
Variance of a measure: IX, 6, 5.
Wiener measure: IX, 6, 7.

Formulas concerning the $\gamma(s)$ and the $\delta(s)$

Let G be a topological group operating continuously on the left in a locally compact space X by $(s, x) \mapsto sx$.

$$
\begin{align*}
\gamma(s)x &= sx & (s \in G, x \in X) \\
\gamma(st) &= \gamma(s)\gamma(t) & (s, t \text{ in } G) \\
(\gamma(s)f)(x) &= f(s^{-1}x) & (f \text{ a function on } X) \\
\langle f, \gamma(s)\mu \rangle &= \langle \gamma(s^{-1})f, \mu \rangle & (\mu \text{ a measure on } X) \\
d(\gamma(s)\mu)(x) &= d\mu(s^{-1}x) \\
(\gamma(s)\mu)(A) &= \mu(s^{-1}A) & (\text{A a } \gamma(s)\mu\text{-integrable set})
\end{align*}
$$

If $\mu$ is relatively invariant with multiplier $\chi$,

$$
\begin{align*}
\gamma(s)\mu &= \chi(s)^{-1}\mu \\
d\mu(sx) &= \chi(s)\,d\mu(x).
\end{align*}
$$

Let G be a topological group operating continuously on the right in a locally compact space X by $(s, x) \mapsto xs$.

$$
\begin{align*}
\delta(s)x &= xs^{-1} \\
\delta(st) &= \delta(s)\delta(t) \\
(\delta(s)f)(x) &= f(xs) \\
\langle f, \delta(s)\mu \rangle &= \langle \delta(s^{-1})f, \mu \rangle \\
d(\delta(s)\mu)(x) &= d\mu(xs) \\
(\delta(s)\mu)(A) &= \mu(As).
\end{align*}
$$

If $\mu$ is relatively invariant with multiplier $\chi'$,

$$
\begin{align*}
\delta(s)\mu &= \chi'(s)\mu \\
d\mu(xs) &= \chi'(s)\,d\mu(x).
\end{align*}
$$

Formulas concerning Haar measures

Let G be a locally compact group, $\Delta$ its modulus, $\mu$ a left Haar measure, $\nu$ a right Haar measure.

1) One has
$$
\begin{align*}
\gamma(s)\mu &= \mu \\
d\mu(sx) &= d\mu(x)
\end{align*}
$$
$$
\begin{align*}
\delta(s)\mu &= \Delta(s)\mu \\
d\mu(xs) &= \Delta(s)\, d\mu(x)
\end{align*}
$$
$$
\begin{align*}
\dot{\mu} &= \Delta^{-1} \cdot \mu \\
d\mu(x^{-1}) &= \Delta(x)^{-1}\, d\mu(x).
\end{align*}
$$

If $f$ is $\mu$-integrable,
$$
\int f(sx)\, d\mu(x) = \int f(x)\, d\mu(x)
$$
$$
\int f(xs)\, d\mu(x) = \Delta(s)^{-1} \int f(x)\, d\mu(x)
$$
$$
\int f(x^{-1})\Delta(x)^{-1}\, d\mu(x) = \int f(x)\, d\mu(x).
$$

If $A \subset G$ is $\mu$-integrable,
$$
\mu(sA) = \mu(A) \qquad \mu(As) = \Delta(s)\mu(A).
$$

2) One has
$$
\begin{align*}
\delta(s)\nu &= \nu \\
d\nu(xs) &= d\nu(x)
\end{align*}
$$
$$
\begin{align*}
\gamma(s)\nu &= \Delta(s)\nu \\
d\nu(s^{-1}x) &= \Delta(s)\, d\nu(x)
\end{align*}
$$
$$
\begin{align*}
\dot{\nu} &= \Delta \cdot \nu \\
d\nu(x^{-1}) &= \Delta(x)\, d\nu(x).
\end{align*}
$$

If $f$ is $\nu$-integrable,
$$
\int f(xs)\, d\nu(x) = \int f(x)\, d\mu(x)
$$
$$
\int f(xs)\, d\nu(x) = \Delta(s) \int f(x)\, d\nu(x)
$$
$$
\int f(x^{-1})\Delta(x)\, d\nu(x) = \int f(x)\, d\nu(x).
$$

If $A \subset G$ is $\nu$-integrable,
$$
\nu(As) = \nu(A) \qquad \nu(sA) = \Delta(s^{-1})\nu(A).
$$

3) $\nu$ is proportional to $\Delta^{-1} \cdot \mu$, $\mu$ is proportional to $\Delta \cdot \nu$.

CONDITIONS SUFFICIENT FOR THE EXISTENCE
OF THE CONVOLUTION PRODUCT

I. — The case that the convolution product $\mu * \nu$ of two measures exists:

(a) \* is defined by a continuous mapping $\varphi : X \times Y \to Z$:
$\mu, \nu$ bounded (then $\mu * \nu$ is bounded and $\| \mu * \nu \| \leq \| \mu \| \cdot \| \nu \|$).
$\mu, \nu$ have compact support (then $\mu * \nu$ has compact support and $\mathrm{Supp}(\mu * \nu) \subset \varphi(\mathrm{Supp} \mu \times \mathrm{Supp} \nu)$).

(b) \* is defined by a group operating continuously on the left in a space:
$\mu$ with compact support, $\nu$ arbitrary.

(c) \* is defined by the multiplication in a group $G$:
one of the two measures has compact support.
$\mu, \nu$ in $\mathcal{M}^\rho(G)$ (then $\mu * \nu \in \mathcal{M}^\rho(G)$, and $\| \mu * \nu \|_\rho \leq \| \mu \|_\rho \| \nu \|_\rho$).

II. — The case that the convolution product $\mu * f$ of a measure and a function exists:

(a) \* is defined by a group $G$ operating continuously on the left in a space $X$
equipped with a measure $\beta \geq 0$ such that $\gamma(s)\beta = \chi(s^{-1}, \cdot)\beta$, $\chi$ being continuous:
$\mu$ with compact support, $f$ locally $\beta$-integrable (if $f$ is continuous, $\mu * f$ is continuous; if $f$ is continuous with compact support, $\mu * f$ is continuous with compact support).
G operates properly in $X$, $f \in \mathcal{K}(X)$ ($\mu * f$ is continuous).

(b) the $\chi(s, \cdot)$ are bounded; let $\rho(s) = \sup_{x \in X} \chi(s^{-1}, x)$:
$\mu \in \mathcal{M}^\rho(G)$, $f \in L^\infty(X, \beta)$ (then $\mu * f \in L^\infty(X, \beta)$; if $f \in C^\infty(X)$,
$\mu * f \in C^\infty(X)$; if $f \in \mathcal{K}(X)$, $\mu * f \in \mathcal{K}(X)$).
$\mu \in \mathcal{M}^{\rho^{1/q}}(G)$, $f \in L^p(X, \beta)$ where $1/p + 1/q = 1$ (then $\mu * f \in L^p(X, \beta)$)
and $\| \mu * f \|_p \leq \| \mu \|_{\rho^{1/q}} \| f \|_p$.

III. — The case that the convolution product $f * g$ of two locally $\beta$-integrable functions exists ($\beta$ a relatively invariant measure $\geq 0$ on a group $G$, with left and right multipliers $\chi$ and $\chi'$):

$f$ or $g$ continuous, $f$ or $g$ with compact support (then $f * g$ is continuous;
if $f, g$ are in $\mathcal{K}(G)$, then $f * g \in \mathcal{K}(G)$).

$$
f \chi^{-1/q} \in L^1(G, \beta) \text{ and } g \in L^p(G, \beta), \text{ where } 1/p + 1/q = 1 \text{ (then } f * g \in L^p(G, \beta) \text{ and } \|f * g\|_p \leq \|f \chi^{-1/q}\|_1 \|g\|_p).
$$
$$
f \in L^p(G, \beta) \text{ and } g {\chi'}^{-1/q} \in L^1(G, \beta) \text{ (then } f * g \in L^p(G, \beta) \text{ and } \|f * g\|_p \leq \|f\|_p \|g {\chi'}^{-1/q}\|_1 ).
$$
$$
f \chi^{-1} \in L^1(G, \beta) \text{ and } g \in \mathcal{C}^\infty(G) \text{ (resp. } \overline{\mathcal{K}(G)} ) \text{ (then } f * g \in \mathcal{C}^\infty(G) \text{ (resp. } \mathcal{K}(G) ) ).
$$
$$
f \in \mathcal{C}^\infty(G, \beta) \text{ (resp. } \overline{\mathcal{K}(G)} ) \text{ and } g {\chi'}^{-1} \in L^1(G, \beta) \text{ (then } f * g \in \mathcal{C}^\infty(G) \text{ (resp. } \mathcal{K}(G) ) ).
$$
$$
f \in L^p(G, \beta), \ g \in L^q(G, \dot{\beta}) \text{ with } 1/p + 1/q = 1, \ 1 < p < +\infty, \ \beta \text{ left-invariant (then } f * g \in \overline{\mathcal{K}(G)} \text{ and } \|f * g\|_\infty \leq \|f\|_p \|g\|_q ).
$$

Contents

CHAPTER VII. — HAAR MEASURE ............................................. VII.1

§1. Construction of a Haar measure ........................................ VII.1
    1. Definitions and notations ............................................ VII.1
    2. The existence and uniqueness theorem ............................... VII.6
    3. Modulus ............................................................. VII.10
    4. Modulus of an autormorphism ...................................... VII.13
    5. Haar measure of a product ......................................... VII.14
    6. Haar measure of an inverse limit .................................. VII.15
    7. Local definition of a Haar measure ............................... VII.18
    8. Relatively invariant measures ..................................... VII.19
    9. Quasi-invariant measures .......................................... VII.20
   10. Locally compact fields ............................................ VII.21
   11. Finite-dimensional algebras over a locally compact field ...... VII.25

§2. Quotient of a space by a group; homogeneous spaces ............. VII.27
    1. General results .................................................. VII.27
    2. The case $\chi = 1$ ........................................... VII.29
    3. Another interpretation of $\lambda^\#$ .......................... VII.32
    4. The case that X/H is paracompact ............................... VII.36
    5. Quasi-invariant measures on a homogeneous space ......... VII.38
    6. Relatively invariant measures on a homogeneous space .. VII.43
    7. Haar measure on a quotient group ............................... VII.44
    8. A transitivity property .......................................... VII.45
    9. Construction of the Haar measure of a group from
        the Haar measures of certain subgroups ..................... VII.48
   10. Integration on a fundamental domain ............................. VII.50

§3. Applications and examples ........................................... VII.53
    1. Compact groups of linear mappings ............................... VII.53
    2. Triviality of fibered spaces and of group extensions ..... VII.55
    3. Examples: 1. General Linear group ............................... VII.60
        2. Affine group .................................................. VII.61
        3. Strict triangular group ..................................... VII.62
        4. Large triangular group ...................................... VII.63
        5. Special triangular group .................................... VII.66

6. Special linear group ......................... VII.67
7. Iwasawa decomposition of $\mathbf{GL}(n, K)$ ..... VII.69
8. Spaces of hermitian forms .................... VII.72
Appendix I ........................................ VII.74
Appendix II ......................................... VII.76
Exercises for §1 .................................. VII.78
Exercises for §2 .................................. VII.87
Exercises for §3 .................................. VII.91

CHAPTER VIII. — CONVOLUTION AND REPRESENTATIONS .... VIII.1

§1. Convolution ..................................... VIII.1
    1. Definition and examples ..................... VIII.1
    2. Associativity ............................... VIII.3
    3. The case of bounded measures ............... VIII.6
    4. Properties concerning supports ............. VIII.6
    5. Vectorial expression of the convolution product ...... VIII.7

§2. Linear representations of groups ............... VIII.8
    1. Continuous linear representations .......... VIII.8
    2. Contragradient representation .............. VIII.10
    3. Example: linear representations in spaces of continuous functions .......................... VIII.11
    4. Example: linear representations in spaces of measures .. VIII.12
    5. Example: linear representations in the spaces $L^p$ ...... VIII.13
    6. Extension of a linear representation of G to the measures on G ............................... VIII.15
    7. Relations between the endomorphisms $U(\mu)$ and the endomorphisms $U(s)$ .................. VIII.16

§3. Convolution of measures on groups ............. VIII.18
    1. Algebras of measures ........................ VIII.18
    2. The case of a group operating on a space ........ VIII.21
    3. Convolution and linear representations ........ VIII.22

§4. Convolution of measures and functions .......... VIII.24
    1. Convolution of a measure and a function ........ VIII.24
    2. Examples of convolvable measures and functions ...... VIII.28
    3. Convolution and transposition ................ VIII.34
    4. Convolution of a measure and a function on a group ... VIII.37
    5. Convolution of functions on a group ............ VIII.38
    6. Applications .................................. VIII.42
    7. Regularization ............................... VIII.44

§5. The space of closed subgroups ........................................ VIII.46

    1. The space of Haar measures on the closed subgroups of G .................................................. VIII.46
    2. Semi-continuity of the volume of the homogeneous space VIII.48
    3. The space of closed subgroups of C ......................... VIII.51
    4. The case of groups without arbitrarily small finite subgroups ............................................. VIII.53
    5. The case of abelian groups .................................... VIII.55
    6. Another interpretation of the topology of the space of closed subgroups ............................... VIII.56
Exercises for §1 .......................................................... VIII.59
Exercises for §2 .......................................................... VIII.59
Exercises for §3 .......................................................... VIII.61
Exercises for §4 .......................................................... VIII.65
Exercises for §5 .......................................................... VIII.73
Historical Note (Chs. VII and VIII) ................................. VIII.75

Chapter IX. — Measures on Hausdorff topological spaces IX.1

§1. Premeasures and measures on a topological space ............ IX.1

    1. Encumbrances .................................................. IX.1
    2. Premeasures and measures ...................................... IX.3
    3. Examples of measures .......................................... IX.6
    4. Locally negligible sets and functions ....................... IX.8
    5. Measurable sets and functions ............................... IX.9
    6. Directed familes; support of a measure ..................... IX.11
    7. Upper envelopes and sums of measures ....................... IX.12
    8. Crushings ..................................................... IX.13
    9. Upper integral ................................................ IX.17
   10. Integration theory ............................................. IX.20

§2. Operations on measures ........................................... IX.22

    1. Induced measure on a measurable subspace ................... IX.22
    2. Measures defined by numerical densities ..................... IX.24
    3. Image of a measure ........................................... IX.26
    4. Lifting of measures .......................................... IX.29
    5. Product of two measures ...................................... IX.31
    6. Integration with respect to the product of two measures IX.33
    7. A result on the disintegration of measures ................. IX.37

§3. Measures and additive set functions ............................................. IX.41
    1. Measures and additive set functions of compact sets ... IX.41
    2. Inner regular set functions ............................................. IX.44
    3. Radon spaces ............................................................ IX.46

§4. Inverse limits of measures ..................................................... IX.49
    1. Complements on compact spaces and inverse limits ....... IX.50
    2. Inverse systems of measures ......................................... IX.50
    3. The case of countable inverse systems ....................... IX.54

§5. Measures on completely regular spaces ................................. IX.56
    1. Measures and bounded continuous functions ............... IX.56
    2. Bounded measures and linear forms on $\mathcal{C}^b(T)$ .......... IX.59
    3. Tight convergence of bounded measures ..................... IX.60
    4. Application: topological properties of the space $\mathcal{M}_+^b(T)$ IX.63
    5. Compactness criterion for tight convergence ............. IX.64
    6. Tight convergence of measures and compact convergence of functions .................................................. IX.67
    7. Application: The Laplace transformation .................. IX.68

§6. Promeasures and measures on a locally convex space ............ IX.72
    1. Promeasures on a locally convex space ..................... IX.72
    2. Image of a promeasure ............................................. IX.74
    3. Fourier transform of a promeasure .......................... IX.75
    4. Calculation of Gaussian integrals ............................ IX.77
    5. Gaussian promeasures and measures .......................... IX.78
    6. Examples of Gaussian promeasures ............................ IX.82
    7. Wiener measure ..................................................... IX.85
    8. Continuity of the Fourier transform ....................... IX.92
    9. Minlos’s lemma ..................................................... IX.93
    10. Measures on the dual of a nuclear space ................. IX.96
    11. Measures on a Hilbert space ................................. IX.97
    *12. Relations with functions of positive type* ............. IX.99

ANNEX: Complements on Hilbert spaces ................................. IX.102
    1. Trace of a quadratic form with respect to another ...... IX.102
    2. Hilbert–Schmidt mappings ....................................... IX.104

Exercises for §1 ............................................................. IX.106
Exercises for §2 ............................................................. IX.108
Exercises for §3 ............................................................. IX.108
Exercises for §4 ............................................................. IX.112
Exercises for §5 ............................................................. IX.113
Exercises for §6 ............................................................. IX.117

Exercises for the Annex .................................................. IX.118
Historical note ............................................................. IX.120
Index of notations .......................................................... 309
Index of terminology ....................................................... 311
Principal formulas of Chapter VII ........................................ 318
Conditions sufficient for the existence of the convolution product . 320
