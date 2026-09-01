---
book: int
book_title: Integration
chapter: VI
chapter_title: VECTORIAL INTEGRATION
section: 0
section_title: Historical Note
kind: historical
lang: en
source: int-i-vi
pdf_pages: 0463-0487
extraction: ocr
statements: 0
exercises: 0
content_sha256: 5e0a858bcf88f33679de7d17e92a9c855995da21ee05f0011e76c182df537e49
---

# HISTORICAL NOTE

(N.B. — The Roman numerals refer to the bibliography at the end of this note.)

With the development of the 'vector calculus' in the course of the 19th century, it was current practice to have to integrate vector-valued functions, but as long as it was only a question of functions with values in finite-dimensional spaces, this operation posed no problem. It is only with Hilbert's spectral theory that one meets operations that lead naturally to a more general concept of integral: this theory in effect leads to associating, with every continuous Hermitian form $\Phi(x, y)$ on a Hilbert space $\mathbf{H}$, a family $(E(\lambda))_{\lambda \in \mathbf{R}}$ of orthogonal projectors having the property that, for every pair $(x, y)$ of vectors of $\mathbf{H}$, the function $\lambda \mapsto (E(\lambda)x|y)$ is of bounded variation and $\Phi(x, y) = \int \lambda d(E(\lambda)x|y)$; if one associates with $\Phi$ the Hermitian operator $A$ such that $\Phi(x, y) = (Ax|y)$, it was tempting to write the preceding formula as $A = \int \lambda dE(\lambda)$. But it was only from about 1935 on, after the introduction by Bochner of the ('strong') integration of a function with values in a Banach space, that one began to be preoccupied with defining the integral of vector-valued functions (or the integral with respect to a vectorial measure) in such a way as to be able to legitimately write formulas such as the preceding one. This extension was accomplished essentially by Gelfand (III), Dunford and Pettis (IV) and (V); their results are stated for Banach spaces, but extend without difficulty to more general locally convex spaces.

The idea of decomposing a volume into 'slices' and reducing an integral over the volume to an integral over each slice, followed by a single integration, has been used in Analysis ever since the beginning of the infinitesimal Calculus (the 'Calculus of indivisibles' of Cavalieri being nothing more than a first outline of this principle, which could even be traced back to Archimedes (see the Hist. Note for Book IV, Chs. I–III)). But in the classical applications, the 'slices' were always of a very special and very regular nature (most often open subsets of analytic surfaces, depending analytically on a parameter); it could scarcely have been otherwise in the absence of a general theory of integration. The general problem of the disintegration of a measure was posed and solved by von Neumann in 1932, in connection with ergodic theory (I); at about the same time (and independently) Kolmogoroff, while laying down axiomatic foundations for the Theory of Probability, was led to define in a general way the concept of 'conditional probability' and to prove its existence, a problem essentially equivalent to that of disintegration of a measure (II).

(I) J. von NEUMANN, Zur Operatorenmethode in der klassischen Mechanik, Ann. of Math., (2), 33 (1932), pp. 587–642.

(II) A. KOLMOGOROFF, Grundbegriffe der Wahrscheinlichkeitsrechnung, Berlin (Springer), 1933.

(III) I. GELFAND, Abstrakte Funktionen und lineare Operatoren, Mat. Sborn., (N.S.), 4 (1938), pp. 235–284.

(IV) N. DUNFORD, Uniformity in linear spaces, Trans. Amer. Math. Soc., 44 (1938), pp. 305–356.

(V) N. DUNFORD AND B. PETTIS, Linear operations on summable functions, Trans. Amer. Math. Soc., 47 (1940), pp. 323–392.

Index of notations

Reference numbers indicate, in order, the chapter, section and subsection (or, exceptionally, exercise).

Chapter III :

$\mathcal{C}(X;E), \mathcal{C}(X), \mathcal{C}(X,A;E), \mathcal{K}(X;E), \mathcal{K}(X), \mathcal{K}(X,A;E), \mathcal{K}(X,A), \mathcal{K}_+(X)$
(X a locally compact space, E a topological vector space) : III, 1, 1.
Supp(f) (f a function with values in a vector space or in $\overline{\mathbf{R}}$) : III, 1, 1.
$\mathcal{C}^b(X;E), \mathcal{C}^0(X;E)$ : III, 1, 2.
$\|f\|$ (f a function with values in a normed space) : III, 1, 2.
$\mu(f), \langle f, \mu \rangle, \int f d\mu, \int f \mu, \int f(x) d\mu(x), \int f(x)\mu(x)$ (f a function in $\mathcal{K}(X;\mathbf{C})$, $\mu$ a (complex) measure) : III, 1, 3.
$\mathcal{M}(X;\mathbf{C}), \mathcal{M}(X), \mathcal{M}_\sigma(X;\mathbf{C}), \mathcal{M}_\sigma(X)$ : III, 1, 3.
$\varepsilon_a$ : III, 1, 3.
g · $\mu$ (g a function in $\mathcal{C}(X;\mathbf{C})$) : III, 1, 4.
$\overline{\mu}, \Re \mu, \Im \mu$ : III, 1, 5.
$\mathcal{M}(X;\mathbf{R}), \mathcal{M}(X), \mathcal{M}_+(X)$ : III, 1, 5.
$\mu \leq \nu$ ($\mu, \nu$ real measures) : III, 1, 5.
$\mu^+, \mu^-, |\mu|$ ($\mu$ a real measure) : III, 1, 5.
$|\mu|$ ($\mu$ a complex measure) : III, 1, 6.
$\|\mu\|$ ($\mu$ a measure) : III, 1, 8.
$\mathcal{M}^1(X,\mathbf{R}), \mathcal{M}^1(X)$ : III, 1, 8.
$\mu|Y$ ($\mu$ a measure on X, Y an open subspace of X) : III, 2, 1.
Supp($\mu$) ($\mu$ a measure) : III, 2, 2.
$\langle f, z' \rangle$ : III, 3, 1.
$\widetilde{\mathcal{K}}(X;E)$ : III, 3, 1.
$\int f d\mu, \int f \mu, \int f(x) d\mu(x), \int f(x)\mu(x)$ (f a function in $\widetilde{\mathcal{K}}(X;E)$) : III, 3, 1.
$\int d\mu(y) \int f(x,y) d\lambda(x)$ : III, 4, 1.
$\iint f d\lambda d\mu, \iint f d\mu d\lambda, \iint f \lambda \mu, \iint f \mu \lambda, \iint f(x,y) d\lambda(x) d\mu(y), \iint f(x,y) d\mu(y) d\lambda(x), \iint f(x,y) \lambda(x) \mu(y), \iint f(x,y) \mu(y) \lambda(x)$ : III, 4, 1.

λ ⊗ μ (λ, μ measures) : III, 4, 2.
μ₁ ⊗ μ₂ ⊗ ⋯ ⊗ μₙ, $\bigotimes_{i=1}^{n} \mu_i$ : III, 4, 4.
$\int f\ d\mu_1\ d\mu_2\ldots\ d\mu_n$, $\iint \ldots \int f\ d\mu_1\ d\mu_2\ldots\ d\mu_n$, $\int f(\mu_1 \otimes \mu_2 \otimes \cdots \otimes \mu_n)$,
$\iint \ldots \int f(x_1, x_2, \ldots, x_n)\ d\mu_1(x_1)\ d\mu_2(x_2)\ldots\ d\mu_n(x_n)$,
$\iint \ldots \int f(x_1, x_2, \ldots, x_n)\mu_1(x_1)\mu_2(x_2)\cdots\mu_n(x_n)$ : III, 4, 4.
$\bigotimes_{\lambda \in L} \mu_\lambda$ : III, 4, 6.

Chapter IV :

φ_A : IV, 1, 1.
ℋ₊, 𝒥₊(X), 𝒥₊ : IV, 1, 1.
μ*(f) (μ a positive measure) : IV, 1, 1, IV, 1, 3 and IV, 4, Exer. 5.
∫* f dμ, ∫* fμ, ∫* f(x) dμ(x), ∫* f(x)μ(x) (f a function ≥ 0, μ a positive measure) : IV, 1, 3.
μ*(A) (A a subset of X, μ a positive measure) : IV, 1, 2 and IV, 1, 4.
f̃ : IV, 2, 4 and IV, 2, 5.
φ((f̃ₙ)), f̃ + g̃, αf̃, g̃f̃ : IV, 2, 4.
f̃ ≤ g̃, supₙ f̃ₙ, infₙ f̃ₙ, lim supₙ→∞ f̃ₙ, lim infₙ→∞ f̃ₙ (f, g, fₙ numerical functions) : IV, 2, 6.
|z| (z a point of a normed space) : IV, 3, 2.
|f| (f a function with values in a normed space) : IV, 3, 2.
N_p(f, μ), N_p(f), N_p(f̃) (1 ≤ p < +∞) : IV, 3, 2.
$\mathcal{G}_F(X), \mathcal{G}_F$ : IV, 3, 3.
$\mathcal{G}_F^p(X, \mu), \mathcal{G}_F^p(\mu), \mathcal{G}_F^p$ : IV, 3, 3.
$\mathcal{G}_F$ : IV, 3, 3.
$\mathcal{G}_F, \mathcal{D}_F^p(X, \mu), \mathcal{D}_F^p(\mu), \mathcal{D}_F^p, L_F^p(X, \mu), L_F^p(\mu), L_F^p, \mathcal{D}^p, L^p (1 \leq p < +\infty)$ : IV, 3, 4.
‖f̃‖_p (1 ≤ p < +∞) : IV, 3, 4.
μ(f), ∫ f dμ, ∫ f(x) dμ(x), ∫ fμ, ∫ f(x)μ(x), μ(f̃) (f a μ-integrable function with values in a Banach space) : IV, 4, 1.
μ(A) (A a μ-integrable set) : IV, 4, 5.
$\mathcal{Q}'(X; C)$ : IV, 4, 8.
𝒬(Φ), 𝒬_F(Φ) (Φ a clan of sets) : IV, 4, 9.
μ_*(f) (f a function) : IV, 4, Exer. 5.

$\mu_*(A)$ (A a set) : IV, 4, Exer. 7.
$\int_A f d\mu, \int_A f\mu, \int_A^* f d\mu, \int_A^* f\mu$ : IV, 5, 6.
$\mathcal{S}(A, \mu; F), \mathcal{S}_F(A, \mu), \mathcal{S}_F(\mu), \mathcal{S}_F$ : IV, 5, 11.
$W(V, B, \delta)$ : IV, 5, 11.
$S(A, \mu; F), S_F(A, \mu), S_F(\mu), S_F$ : IV, 5, 11.
$f^*$ (the decreasing rearrangement of $f$) : IV, 5, Exer. 29.
$M_\infty(f), m_\infty(f)$ : IV, 6, 2.
$N_\infty(f)$ : IV, 6, 3.
$\mathcal{L}_F^\infty(X, \mu), \mathcal{L}_F^\infty(\mu), \mathcal{L}_F^\infty, \mathcal{N}_F^\infty$ : IV, 6, 3.
$\|\dot{f}\|_\infty, N_\infty(\dot{f})$ : IV, 6, 3.
$L_F^\infty(X, \mu), L_F^\infty(\mu), L_F^\infty, \mathcal{L}^\infty, L^\infty$ : IV, 6, 3.
$b_\mu$ : IV, 7, 1.
$\mathrm{Ch}_\mathcal{H}(X), \mathrm{Ch}(X), \check{S}_\mathcal{H}(X), \check{S}(X)$ : IV, 7, 3.

Chapter V :

$\mathcal{F}_+(E), \mathcal{F}_+$ (E a set) : V, Preliminary conventions.
$\mu^\bullet(f), \mu^\bullet(A), \int^\bullet f d\mu, \int^\bullet f(t) d\mu(t), \int^\bullet f\mu$ : V, 1, 1.
$\overline{\mathcal{F}}_F^p(T, \mu), \overline{\mathcal{F}}_F^p(\mu), \overline{\mathcal{F}}_F^p$ : V, 1, 3.
$\overline{N}_p(f), \overline{\mathcal{L}}_F^p(T, \mu), \overline{\mathcal{L}}_F^p(\mu), \overline{\mathcal{L}}_F^p$ : V, 1, 3.
$\overline{\mathcal{L}}_F^p(T, \theta)$ ($\theta$ a complex measure) : V, 1, 3.
$\int \lambda_t d\mu(t)$ ($t \mapsto \lambda_t$ a family of positive measures) : V, 3, 1.
$\int d\mu(t) \int f(x) d\lambda_t(x)$ : V, 3, 1.
$\|\Lambda\|$ ($\Lambda$ a diffusion) : V, 3, 5.
$\langle \eta, h \rangle$ : V, 3, 5.
$\Lambda f, \mu \Lambda$ : V, 3, 5.
$\Lambda H$ : V, 3, 6.
$\mathcal{L}_{\text{loc}}^1(T, \mu; F), L_{\text{loc}}^1(T, \mu; F)$ : V, 5, 1.
$u \cdot \theta$ ($u$ a complex function, $\theta$ a complex measure) : V, 5, 2.
$\int_A^\bullet f d\mu$ : V, 5, 3.
$u(\mu_1, \ldots, \mu_n)$ ($u$ a positively homogeneous numerical function) : V, 5, 9.
$\pi(\mu)$ ($\pi$ a $\mu$-proper mapping): V, 6, 1.
$\pi(\theta)$ ($\theta$ a complex measure, $\pi$ an $|\theta|$-proper mapping) : V, 6, 4.
$\pi^{-1}(\mu)$ ($\pi$ a local homeomorphism): V, 6, 6.
$\iint^* f(t, t') d\mu(t) d\mu'(t'), \iint^\bullet f(t, t') d\mu(t) d\mu'(t'), \iint f(t, t') d\mu(t) d\mu'(t')$ : V, 8, 1

Chapter VI:

F', F'', {F'}^*, F_\sigma (F a Hausdorff locally convex space) : VI, Introduction.
\mathcal{K}(T), \mathcal{K}_R(T), \mathcal{K}_C(T), \mathcal{K}(T,A), \mathcal{K}_C(T,A) : VI, Introduction.
\langle f, z' \rangle, \langle z', f \rangle : VI, 1.
\int f d\mu, \int f(t) d\mu(t) (f a vector-valued function, \mu a positive measure) :
VI, 1, 1.
gf, fg (f a vector-valued function, g a scalar function) : VI, 1, 1.
\mathcal{C}'(T) : VI, 1, 6.
\int f dm, \int f(t) dm(t) (f a numerical function, m a vectorial measure) :
VI, 2, 1 and VI, 2, 2.
g \cdot m (g a numerical function, m a vectorial measure) : VI, 2, 1.
$\mathcal{L}(m)$ : VI, 2, 2.
q(m), |m| (q a semi-norm, m a vectorial measure) : VI, 2, 3.
f \cdot \mu (f a vector-valued function, \mu a positive measure) : VI, 2, 4.
$\mathcal{L}_{F_s'}^\infty, L_{F_s'}^\infty$ : VI, 2, 5.
\langle f, g \rangle (f, g vector-valued functions) : VI, 2, 6.
I_{\Phi,m}, \int f dm (f a vector-valued function, m a vectorial measure) : VI, 2, 7.
|m|, \int f dm (m a complex measure) : VI, 2, 8, III, 1, 6.
\mathcal{L}_F^p(T,m), \overline{\mathcal{L}}_F^p(T,m), L_F^p(T,m) (m a complex measure) : VI, 2, 8, V, 1, 3.
h \cdot m (m a complex measure) : VI, 2, 8.
\overline{m} (m a complex measure) : VI, 2, 8, III, 1, 5.
\|m\| (m a complex measure) : VI, 2, 9, III, 1, 8.
\pi(m), m_Y, m \otimes m' (m, m' complex measures) : VI, 2, 10.
\mathcal{B}(F_1, F_2), r\Phi, l\Phi : VI, App., 1.
E_\sigma, F_\sigma, E'_s, F'_s, \mathcal{B}(E,F) : VI, App., 1.
\Lambda_{F'}^p(T,\mu), M_p, M'_p : VI, 1, Exer. 16.

Index of terminology

Reference numbers indicate, in order, the chapter, section and subsection (or, exceptionally, exercise).

Absolute value of a measure : III, 1, 6 and VI, 2, 8.
Adapted pair, $\mu^-$ : V, 4, 1.
Additive set function : IV, 4, 9.
Additivity, complete : IV, 4, 5.
Adequate mapping, $\mu^-$ : V, 3, 1 and VI, 1, 1, Footnote.
Alien measures : V, 5, 7.
Almost everywhere, function defined : IV, 2, 5.
Almost everywhere, property true : IV, 2, 3.
Atomic measure : III, 1, 3.
Band, in a fully lattice-ordered space : II, 1, 5.
Barycenter of a measure : IV, 7, 1.
Base $\mu$, measure with : V, 5, 2 and VI, 2, 8.
Base $\mu$, scalarly of (vectorial measure) : VI, 2, 5.
Base $\mu$, vectorial measure with : VI, 2, 4.
Belonging to the domain of a diffusion, measure : V, 3, 5.
Bishop’s theorem : IV, 7, 5.
Boundary, frontier : III, 1, 1, Footnote.
Bounded diffusion: V, 3, 5.
Bounded in measure, function : IV, 6, 2 and IV, 6, 3.
Bounded measure : III, 1, 8 and VI, 2, 9.
Carrying a measure, subset : V, 5, 7.
Choquet’s theorems : IV, 7, 2 and IV, 7, 6.
Clan of subsets of a set : IV, 4, 9.
Class, equivalence (of functions), for a measure : IV, 2, 4, IV, 2, 5 and IV, 5, 2.
Class, pseudo-image (of a class of measures) : VI, 3, 2.
Co-lattice subspace : II, 1, Exer. 3.
Compact convergence (in the space of measures) : III, 1, 10.
Completely additive : IV, 4, 5.
Complex measure : III, 1, 3 and VI, 2, 8.
Composed diffusion : V, 3, 6.

Concentrated on a set, measure : V, 5, 7.
Conjugate exponents : IV, 6, 4.
Conjugate measure : III, 1, 5 and VI, 2, 8.
Connected component : V, 6, Exer. 12, Footnote.
Conservative mapping : V, 7, Exer. 9.
Continuous almost everywhere : IV, 5, Exer. 16.
Convergence in mean, convergence in mean of order $p$, convergence in quadratic mean : IV, 3, 3.
Convergence in measure : IV, 5, 11.
Convergence, almost everywhere : IV, 2, 5.
Convergence, compact (in the space of measures) : III, 1, 10.
Convergence, strictly compact (in the space of measures) : III, 1, 10.
Convergence, vague : III, 1, 9.
Convergent filter in a fully lattice-ordered space : II, 1, Exer. 9.
Countable at infinity : III, 1, 1, Footnote.
Countable convexity, theorem of : IV, 3, 2.
Decomposition into slices, of a measure : V, 6, 6 and VI, 3. 1.
Decreasing rearrangement of a function : IV, 5, Exer. 29.
Defined almost everywhere (function) : IV, 2, 5.
Defined locally almost everywhere (function) : IV, 5, 2.
Density $g$ (relative to $\theta$), measure with : V, 5, 2 and VI, 2, 8.
Density point (of a subset) : V, 6, Exer. 15.
Density, of a vectorial measure with respect to a positive measure : VI, 2, 4.
Density, with respect to a complex measure : III, 1, 4, V, 5, 2 and VI, 2, 8.
Derivates of a function : V, 6, Exer. 12.
Diffuse measure : V, 5, 10.
Diffusion : V, 3, 5.
Diffusion, bounded : V, 3, 5.
Diffusion, composed : V, 3, 6.
Dirac measure : III, 1, 3.
Direct limit, of a direct system of locally convex spaces : III, 1, 1.
Direct sum, ordered : II, 1, 4.
Discrete measure : III, 1, 3.
Disintegration of a measure : V, 6, 6 and VI, 3, 1.
Disintegration, of a measure $\mu$ relative to a $\mu$-proper mapping : VI, 3, 1.
Disintegration, of a measure $\mu$ relative to a pseudo-image of $\mu$ : VI, 3, 3.
Disintegration, of a measure by a measurable equivalence relation : VI, 3, 5.
Distribution of a sequence, limit : III, 2, Exer. 5.
Domain of a diffusion, measure belonging to : V, 3, 5.

Double integral : III, 4, 1.
Dunford–Pettis theorem : VI, 2, 5.
Egoroff’s theorem : IV, 5, 4.
Equi-integrable set (of functions) : IV, 5, 11.
Equidistributed sequence (for a measure) : III, 2, Exer. 5.
Equimeasurable functions : IV, 5, Exer. 29.
Equivalence class of functions for a measure : IV, 2, 4, IV, 2, 5 and IV, 5, 2.
Equivalence relation, Hausdorff : VI, 3, 4.
Equivalence relation, measurable : VI, 3, 4.
Equivalent measures : V, 5, 6 and VI, 2, 8.
Equivalent, $\mu$-equivalent (functions) : IV, 2, 4.
Essential upper integral : V, 1, 1.
Essentially $\mu$-integrable (set, function) : V, 1, 3.
Essentially integrable function : V, 1, 3.
Essentially integrable function, $p$-th power : V, 1, 3.
Essentially integrable function, for a vectorial measure : VI, 2, 2.
Essentially integrable on $A$, function : V, 5, 3.
Expansion set (right-, left-) of a function : V, 6, Exer. 12.
Extremal point, $\mathcal{H}^-$ : IV, 7, 3.
Finite almost everywhere, function : IV, 2, 6.
Form, positive linear : II, 2, 1.
Form, relatively bounded linear : II, 2, 2.
Fully lattice-ordered space : II, 1, 3.
Function depending only on a finite number of variables : III, 4, 6.
Function, $\mu$-measurable on $A$ : V, 5, 3.
Function, $\mu$-moderated : V, 1, 2.
Function, $\Phi$-step : IV, 4, 9.
Function, $p$-th power essentially integrable : V, 1, 3.
Function, $p$-th power integrable : IV, 3, 4.
Function, bounded in measure : IV, 6, 2 and IV, 6, 3.
Function, defined almost everywhere : IV, 2, 5.
Function, defined locally almost everywhere : IV, 5, 2.
Function, essentially integrable : V, 1, 3.
Function, essentially integrable for a vectorial measure : VI, 2, 2.
Function, essentially integrable on $A$ : V, 5, 3.
Function, finite almost everywhere : IV, 2, 6.
Function, having a property scalarly : VI, 1, 1.
Function, integrable, $\mu$-integrable : IV, 4, 1.
Function, Lebesgue $n$-th : IV, 6, Exer. 15.

Function, locally integrable : V, 5, 1.
Function, locally integrable on A : V, 5, 3.
Function, locally negligible, locally $\mu$-negligible : IV, 5, 2.
Function, measurable step : IV, 5, 5.
Function, measurable, $\mu$-measurable : IV, 5, 1.
Function, measurable, defined on a measurable subset of X : IV, 5, 10 and V, 5, 3.
Function, negligible, $\mu$-negligible : IV, 2, 1 and IV, 2, 4.
Function, numerical : I, 1, 1, Footnote.
Function, scalarly essentially integrable : V, 3, 1, VI, 1, 1 and VI, 2, 10.
Function, scalarly well integrable : VI, 1, Exer. 19.
Function, step, $\Phi$-step : IV, 4, 9.
Function, support of : III, 1, 1.
Function, universally measurable : V, 3, 4.
Function, vaguely $\mu$-measurable : V, 3, 1.
Function, vaguely continuous : V, 3, 1.
Functions, equi-integrable : IV, 5, 11.
Functions, equimeasurable : IV, 5, Exer. 29.
Functions, equivalent, $\mu$-equivalent : IV, 2, 4.
(GDF) property : VI, 1, 4.
Gelfand–Dunford theorem : VI, 1, 4.
Gliding hump method : V, 5, Exer. 13.
$\mathcal{H}$-extremal point : IV, 7, 3.
Hölder’s inequality : I, 2 and IV, 6, 4.
Haar orthonormal system : IV, 6, Exer. 17.
Hardy’s inequality : IV, 6, Exer. 19.
Hausdorff equivalence relation : VI, 3, 4.
Image of a measure : V, 6, 1, V, 6, 4 and VI, 2, 10.
Imaginary part of a measure : III, 1, 5 and VI, 2, 8.
Induced measure, on a locally compact subspace : IV, 5, 7 and VI, 2, 10.
Induced measure, on an open subset : III, 2, 1.
Inductive limit, of an inductive system of locally convex spaces : see direct limit.
Inequality of Hölder : I, 2 and IV, 6, 4.
Inequality of Hardy : IV, 6, Exer. 19.
Inequality of M. Riesz : IV, 6, Exer. 18.
Inequality of Minkowski : I, 2 and IV, 3, 1.
Inequality of the mean : IV, 6, 2.
Infimum : II, 1, 1, Footnote.

Inner measure : IV, 4, Exer. 7.
Integrable function : IV, 4, 1.
Integrable function, $p$-th power : IV, 3, 4.
Integrable set, $\mu$-integrable set : IV, 4, 5.
Integral of a function on $A$ (or extended to $A$) : V, 5, 3.
Integral of a scalarly essentially integrable mapping : V, 3, 1, VI, 1, 1 and VI, 2, 10.
Integral of an essentially integrable function : V, 1, 3.
Integral, double : III, 4, 1.
Integral, essential upper : V, 1, 1.
Integral, lower : IV, 4, Exer. 5.
Integral, multiple, $n$-tuple : III, 4, 4.
Integral, of a continuous numerical function with compact support : III, 1, 3.
Integral, of a numerical function with respect to a vectorial measure : VI, 2, 2.
Integral, of a vector-valued function with respect to a positive measure : IV, 4, 1, V, 1, 3 and VI, 1, 1.
Integral, of a vector-valued function with respect to a vectorial measure : VI, 2, 7.
Integral, of a weakly continuous function scalarly of compact support : III, 3, 1.
Integral, of an integrable function : IV, 4, 1.
Integral, upper : IV, 1, 1, IV, 1, 3 and IV, 4, Exer. 5.
Integration by parts : V, 8, Exer. 9.
Invariant measure, under a homeomorphism : III, 1, 3.
Inverse image of a measure under a local homeomorphism : V, 6, 6.
Inverse limit, of an inverse system of measures : III, 4, 5.
Inverse system (of measures) : III, 4, 5.
Isolated subspace, of a Riesz space : II, 1, Exer. 4.
Krein’s theorem : IV, 7, Exer. 10.
Lattice-ordered vector space : II, 1, 1.
Latticial linear mapping : II, 2, Exer. 5.
Lebesgue function, $n$-th : IV, 6, Exer. 15.
Lebesgue measure : III, 1, 3, III, 4, 1 and III, 4, 4.
Lebesgue’s decomposition theorem : V, 5, 7.
Lebesgue’s theorem : IV, 3, 7 and IV, 4, 3.
Lebesgue–Fubini theorem : V, 8, 4.
Lebesgue–Nikodym theorem : V, 5, 5.
Lifting property : VI, 2, 5.
Limit distribution of a sequence : III, 2, Exer. 5.

Limit superior, limit inferior, in a fully lattice-ordered space : II, 1, Exer. 9.
Limit, direct (or inductive) : III, 1, 1.
Limit, inverse (or projective) : III, 4, 5.
Limit, of a filter in a fully lattice-ordered space : II, 1, Exer. 9.
Linear form, positive : II, 2, 1.
Linear form, relatively bounded : II, 2, 2.
Localization principle, for measurable functions : IV, 5, 2.
Localization principle, for measures : III, 2, 1.
Locally almost everywhere : IV, 5, 2.
Locally countable (set of subsets) : IV, 5, 9.
Locally countable family of functions $\geq 0$ : V, 5, 4.
Locally integrable function : V, 5, 1.
Locally integrable on $A$, function : V, 5, 3.
Locally negligible ($\mu$-negligible) function : IV, 5, 2.
Locally negligible set, locally $\mu$-negligible set : IV, 5, 2.
Lower integral : IV, 4, Exer. 5.
$\mu$-adapted pair : V, 4, 1.
$\mu$-adequate mapping : V, 3, 1 and VI, 1, 1, Footnote.
$\mu$-dense (set of compact subsets) : IV, 5, 8.
$\mu$-equivalent functions : IV, 2, 4.
$\mu$-integrable function : IV, 4, 1.
$\mu$-integrable set : IV, 4, 5.
$\mu$-maximum, $\mu$-minimum : IV, 6, 2.
$\mu$-measurable (set, function) : IV, 5, 1.
$\mu$-measurable equivalence relation : VI, 3, 4.
$\mu$-moderated (function, subset) : V, 1, 2.
$\mu$-negligible function : IV, 2, 1 and IV, 2, 4.
$\mu$-negligible set : IV, 2, 2.
$\mu$-pre-adequate mapping : V, 3, 1.
$\mu$-proper mapping : V, 6, 1, V, 6, 4 and VI, 2, 10.
Majorizable measure : VI, 2, 3.
Mapping, $\mu$-adequate : V, 3, 1.
Mapping, $\mu$-pre-adequate : V, 3, 1.
Mapping, $\mu$-proper (or proper for $\mu$) : V, 6, 1, V, 6, 4 and VI, 2, 10.
Mapping, conservative : V, 7, Exer. 9.
Mapping, scalarly of compact support : III, 3, 1.
Mapping, weakly continuous : III, 3, 1.
Mass, total, of a bounded measure : III, 1, 8 and IV, 4, 7.
Masses, measure defined by : III, 1, 3.

Maximum in measure, $\mu$-maximum : IV, 6, 2.
Mean of a function : III, 1, 8.
Mean of order $p$, convergence in : IV, 3. 3.
Mean, convergence in : IV, 3, 3.
Mean, inequality of the : IV, 6, 2.
Measurable (set, function) : IV, 5, 1.
Measurable equivalence relation : VI, 3, 4.
Measurable function defined on a measurable subset of X : IV, 5, 10 and V, 5, 3.
Measurable on A , function : IV, 5, 10 and V, 5, 3.
Measurable section : VI, 3, 4.
Measurable step function : IV, 5, 5.
Measure belonging to the domain of a diffusion : V, 3, 5.
Measure concentrated on a set : V, 5, 7.
Measure of an integrable set : IV, 4, 5.
Measure with base $\mu$ : V, 5, 2.
Measure with density $g$ (with respect to $\theta$) : V, 5, 2.
Measure, absolute value of : III, 1, 6 and VI, 2, 8.
Measure, atomic : III, 1, 3.
Measure, bounded : III, 1, 8 and VI, 2, 9.
Measure, complex measure : III, 1, 3 and VI, 2, 8.
Measure, conjugate : III, 1, 5 and VI, 2, 8.
Measure, defined by a unit mass at a point : III, 1, 3.
Measure, defined by masses : III, 1, 3.
Measure, diffuse : V, 5, 10.
Measure, Dirac : III, 1, 3.
Measure, discrete : III, 1, 3.
Measure, image of : V, 6, 1, V, 6, 4 and VI, 2, 10.
Measure, induced : III, 2, 1, IV, 5, 7 and VI, 2, 10.
Measure, inner : IV, 4, Exer. 7.
Measure, invariant under a homeomorphism : III, 1, 3.
Measure, involving no mass in an open set : III, 2, 2.
Measure, Lebesgue : III, 1, 3, III, 4, 1 and III, 4, 4.
Measure, majorizable, $q$-majorizable : VI, 2, 3.
Measure, norm of : III, 1, 8.
Measure, outer : IV, 1, 2 and IV, 1, 4.
Measure, point : III, 2, 4.
Measure, positive : III, 1, 5.
Measure, product : III, 4, 1, III, 4, 4, III, 4, 6 and VI, 2, 10.

Measure, pseudo-image : VI, 3, 2.
Measure, quotient by an equivalence relation : VI, 3, 5.
Measure, real : III, 1, 5 and VI, 2, 1.
Measure, real and imaginary parts : III, 1, 5 and VI, 2, 8.
Measure, scalar : VI, 2, 1.
Measure, support of : III, 2, 2.
Measure, vectorial : VI, 2, 1.
Measure, with density $g$ with respect to $\mu$ : III, 1, 4, V, 5, 2 and VI, 2, 8.
Measures, alien : V, 5, 7.
Measures, equivalent : V, 5, 6 and VI, 2, 8.
Minimum in measure, $\mu$-minimum : IV, 6, 2.
Minkowski’s inequality : I, 2 and IV, 3, 1.
Moderated function, $\mu$- : V, 1, 2.
Moderated measure : V, 1, 2.
Moderated subset, $\mu$- : V, 1, 2.
Multiple integral : III, 4, 4.
$n$-tuple integral : III, 4, 4.
Negligible function : IV, 2, 1 and IV, 2, 4.
Negligible set : IV, 2, 2.
Norm of a diffusion : V, 3, 5.
Norm of a measure : III, 1, 8.
Numerical function : I, 1, 1, Footnote.
Order $n$, multiple integral of : III, 4, 4.
Order $p$, convergence in mean of : IV, 3, 3.
Order $p$, equi-integrable of (set of functions) : IV, 5, 11.
Ordered direct sum : II, 1, 4.
Orthonormal sequence, in $\mathcal{L}^2$ : IV, 6, Exer. 15.
Orthonormal system, Haar : IV, 6, Exer. 17.
Outer measure : IV, 1, 2 and IV, 1, 4.
$p$-th power integrable function : IV, 3, 4.
Parts of a measure, real and imaginary : III, 1, 5 and VI, 2, 8.
$\Phi$-step function : IV, 4, 9.
Point measure : III, 2, 4.
Point, $\mathcal{H}$-extremal : IV, 7, 3.
Positive linear form : II, 2, 1.
Positive measure : III, 1, 5.
Pre-adequate mapping, $\mu$- : V, 3, 1.
Principle of localization for measurable functions : IV, 5, 2.
Principle of localization for measures : III, 2, 1.

Product of a family of positive measures : III, 4, 6.
Product of a finite number of measures : III, 4, 4.
Product of a measure by a continuous function : III, 1, 4.
Product of a measure by a locally integrable function : V, 5, 2.
Product of two measures : III, 4, 1 and VI, 2, 10.
Projective limit, of a projective system of measures : see inverse limit.
Projective system of measures : see inverse system.
Proper mapping, $\mu^-$ : V, 6, 1, V, 6, 4 and VI, 2, 10.
Property (GDF) : VI, 1, 4.
Property true almost everywhere : IV, 2, 3.
Property true locally almost everywhere : IV, 5, 2.
Property, lifting : VI, 2, 5.
Pseudo-image (class, measure) : VI, 3, 2.
$q$-majorizable measure : VI, 2, 3.
Quadrable set : IV, 5, Exer. 17.
Quadratic mean, convergence in : IV, 3, 3.
Quasi-integrable function : IV, 5, Exer. 15.
Quasi-strong topology : III, 1, Exer. 8.
Quotient measure, of a measure by an equivalence relation : VI, 3, 5.
Real measure : III, 1, 5 and VI, 2, 1.
Real part of a measure : III, 1, 5 and VI, 2, 8.
Rearrangement of a function, decreasing : IV, 5, Exer. 29.
Recede indefinitely along a filter : III, 2, 2.
Relatively bounded linear form : II, 2, 2.
Restriction of a measure to a locally compact subset : IV, 5, 7 and VI, 2, 10.
Restriction of a measure to an open set : III, 2, 1.
Riesz space : II, 1, 1.
Riesz, F., theorem of : II, 1, 5.
Riesz, M., inequality of : IV, 6, Exer. 18.
Scalar measure : VI, 2, 1.
Scalarly essentially integrable mapping : V, 3, 1, VI, 1, 1 and VI, 2, 10.
Scalarly of base $\mu$, vectorial measure : VI, 2, 5.
Scalarly of compact support, mapping : III, 3, 1.
Scalarly well integrable function : VI, 1, Exer. 19.
Scalarly, function having a property : VI, 1, 1.
Section, measurable : VI, 3, 4.
Separable : IV, 2, 4, Footnote.
Sequence convergent almost everywhere : IV, 2, 5.
Sequence equidistributed for a measure : III, 2, Exer. 5.

Series convergent almost everywhere : IV, 2, 5.
Set function, additive : IV, 4, 9.
Slices, decomposition into (of a measure): V, 6, 6 and VI, 3, 1.
Space, fully lattice-ordered : II, 1, 3.
Space, Riesz : II, 1, 1.
Step function : IV, 4, 9.
Step function, $\Phi$ : IV, 4, 9.
Step function, measurable : IV, 5, 5.
Stieltjes measure : V, 6, Exer. 5.
Stone space : II, 1, Exer. 13.
Strictly compact convergence (in the space of measures) : III, 1, 10.
Strictly compact set, in $\mathcal{K}(X;E)$ : III, 1, 1.
Summable family of positive measures : V, 2, 1.
Support of a function : III, 1, 1.
Support of a measure : III, 2, 2.
Support of a vectorial measure : VI, 2, 1.
Supremum : II, 1, 1, Footnote.
Theorem of Bishop : IV, 7, 5.
Theorem of countable convexity : IV, 3, 2.
Theorem of Egoroff : IV, 5, 4.
Theorem of F. Riesz : II, 1, 5.
Theorem of Krein : IV, 7, Exer. 10.
Theorem of Lebesgue : IV, 3, 7 and IV, 4, 3.
Theorem, Dunford–Pettis : VI, 2, 5.
Theorem, Gelfand–Dunford : VI, 1, 4.
Theorem, Lebesgue decompositon : V, 5, 7.
Theorem, Lebesgue–Fubini : V, 8, 4.
Theorem, Lebesgue–Nikodym : V, 5, 5.
Theorems of Choquet : IV, 7, 2 and IV, 7, 6.
Topology of compact convergence, of strictly compact convergence (on the space of measures) : III, 1, 10.
Topology of convergence in mean, in mean of order $p$, in quadratic mean : IV, 3. 3.
Topology of convergence in measure : IV, 5, 11.
Topology, quasi-strong : III, 1, Exer. 8.
Topology, ultrastrong : III, 1, Exer. 15.
Topology, vague : III, 1, 9.
Total mass, of a bounded measure : III, 1, 8 and IV, 4, 7.
Tribe of subsets : IV, 4, 9, Footnote.

True almost everywhere, property : IV, 2, 3.
True locally almost everywhere, property : IV, 5, 2.
Ultrastrong topology : III, 1, Exer. 15.
Uniform structure of convergence in measure : IV, 5, 11.
Universally measurable (set, function) : V, 3, 4.
Upper integral : IV, 1, 1, IV, 1, 3 and IV, 4, Exer. 5.
Upper integral, essential : V, 1, 1.
Vague convergence : III, 1, 9.
Vague topology : III, 1, 9.
Vaguely $\mu$-measurable function : V, 3, 1.
Vaguely continuous function : V, 3, 1.
Vectorial measure : VI, 2, 1.
Vectorial measure of base $\mu$ : VI, 2, 4.
Vectorial measure, $q$-majorizable : VI, 2, 3.
Vectorial measure, majorizable : VI, 2, 3.
Vectorial measure, scalarly with base $\mu$ : VI, 2, 5.
Vectorial measure, support of : VI, 2, 1.
Weakly continuous mapping : III, 3, 1.
Well integrable, scalarly : VI, 1, Exer. 19.

Contents

Introduction ......................................................... ix

Chapter I. — Inequalities of convexity ......................... I.1
    1. The fundamental inequality of convexity ............... I.1
    2. The inequalities of Hölder and Minkowski ............. I.3
    3. The semi-norms $N_p$ ................................. I.4
Exercises for Ch. I ................................................. I.6
Historical note .................................................... I.8

Chapter II. — Riesz spaces ....................................... II.1
§1. *Riesz spaces and fully lattice-ordered spaces* ........ II.1
    1. Definition of Riesz spaces ............................. II.1
    2. Generation of a Riesz space by its positive elements ... II.3
    3. Fully lattice-ordered spaces ............................ II.4
    4. Subspaces and product spaces of fully lattice-ordered spaces ............................................. II.5
    5. Bands in a fully lattice-ordered space ................. II.6
§2. *Linear forms on a Riesz space* .......................... II.9
    1. Positive linear forms on a Riesz space ............... II.9
    2. Relatively bounded linear forms ....................... II.10
Exercises for §1 .................................................. II.15
Exercises for §2 .................................................. II.19

Chapter III. — Measures on locally compact spaces ... III.1
§1. *Measures on a locally compact space* .................. III.1
    1. Continuous functions with compact support ............. III.1
    2. Approximation properties ............................... III.4
    3. Definition of a measure ............................... III.7
    4. Product of a measure by a continuous function ....... III.10
    5. Real measures. Positive measures ...................... III.11
    6. Absolute value of a complex measure ................. III.13
    7. Definition of a measure by extension ................. III.15

8. Bounded measures ............................................. III.16
9. Vague topology on the space of measures ............... III.18
10. Compact convergence in $\mathcal{M}(X; \mathbf{C})$ .................. III.21

§2. Support of a measure ............................................. III.23
    1. Restriction of a measure to an open set. Definition of a measure by means of local data .................. III.23
    2. Support of a measure ............................................. III.25
    3. Characterization of the support of a measure .......... III.27
    4. Point measures. Measures with finite support .......... III.29
    5. Discrete measures ............................................. III.31

§3. Integrals of continuous vector-valued functions ............ III.32
    1. Definition of the integral of a vector-valued function ... III.32
    2. Properties of the vectorial integral ..................... III.34
    3. Criteria for the integral to belong to E ................. III.37
    4. Continuity properties of the integral ................... III.39

§4. Products of measures ............................................. III.40
    1. The product of two measures ............................... III.40
    2. Properties of product measures ........................... III.44
    3. Continuity of product measures ........................... III.47
    4. Product of a finite number of measures .................. III.48
    5. Inverse limits of measures ............................... III.50
    6. Infinite products of measures ............................ III.53
Exercises for §1 .................................................. III.55
Exercises for §2 .................................................. III.59
Exercises for §3 .................................................. III.60
Exercises for §4 .................................................. III.60

CHAPTER IV. — EXTENSION OF A MEASURE. $L^p$ SPACES ....... IV.1

§1. Upper integral of a positive function ....................... IV.1
    1. Upper integral of a lower semi-continuous positive function ............................................. IV.1
    2. Outer measure of an open set ............................. IV.4
    3. Upper integral of a positive function ................... IV.6
    4. Outer measure of an arbitrary set ....................... IV.10

§2. Negligible functions and sets ............................... IV.11
    1. Negligible positive functions ............................ IV.11
    2. Negligible sets ............................................. IV.12
    3. Properties true almost everywhere ...................... IV.12

4. Classes of equivalent functions ......................... IV.13
5. Functions defined almost everywhere ................. IV.15
6. Equivalence classes of functions with values in $\overline{\mathbf{R}}$ ..... IV.16

§3. $L^p$ spaces ............................................. IV.18
    1. Minkowski’s inequality .................................. IV.18
    2. The semi-norms $N_p$ ................................. IV.19
    3. The spaces $\mathcal{F}_F^p$ .......................... IV.20
    4. $p$-th power integrable functions .................. IV.23
    5. Properties of $p$-th power integrable functions .... IV.25
    6. Directed sets in $L^p$ and increasing sequences in $\mathcal{L}^p$ .. IV.27
    7. Lebesgue’s theorem ...................................... IV.30
    8. Relations between the spaces $\mathcal{L}_F^p$ ($1 \leq p < +\infty$) ..... IV.31

§4. Integrable functions and sets ............................ IV.32
    1. Extension of the integral ............................... IV.32
    2. Properties of the integral ............................. IV.34
    3. Passage to the limit in integrals ..................... IV.36
    4. Characterizations of integrable numerical functions ... IV.37
    5. Integrable sets ........................................ IV.41
    6. Criteria for the integrability of a set ............... IV.43
    7. Characterizations of bounded measures .................. IV.46
    8. Integration with respect to a measure with compact support .................................................. IV.47
    9. Clans and additive set functions ....................... IV.50
    10. Approximation of continuous functions by step functions ..................................................... IV.52
    11. Extension of a measure defined on a family of sets ... IV.53

§5. Measurable functions and sets ............................ IV.59
    1. Definition of measurable functions and sets .......... IV.59
    2. Principle of localization. Locally negligible sets ...... IV.61
    3. Elementary properties of measurable functions ........ IV.63
    4. Limits of measurable functions .......................... IV.64
    5. Criteria for measurability ............................. IV.66
    6. Criteria for integrability .............................. IV.71
    7. Measure induced on a locally compact subspace ........ IV.73
    8. $\mu$-dense families of compact sets ................. IV.76
    9. Locally countable partitions ........................... IV.77
    10. Measurable functions defined on a measurable subset .. IV.78
    11. Convergence in measure ............................... IV.80
    12. A property of vague convergence ....................... IV.86

§6. Convexity inequalities ............................................. IV.89
    1. The convexity theorem ............................................. IV.89
    2. Inequality of the mean ............................................. IV.90
    3. The spaces $L_F^\infty$ ............................................. IV.91
    4. Hölder’s inequality ............................................. IV.93
    5. Applications: relations between the spaces $L_F^p$
        ($1 \leq p \leq +\infty$) ............................................. IV.98

§7. Barycenters ......................................................... IV.101
    1. Definition of barycenters ............................................. IV.101
    2. Extremal points and barycenters ............................................. IV.102
    3. Applications: I. Vector spaces of continuous real functions ............................................. IV.106
    4. Applications: II. Vector spaces of continuous complex functions ............................................. IV.110
    5. Applications: III. Algebras of continuous functions .... IV.111
    6. Uniqueness of integral representations ................. IV.115

Exercises for §1 .......................................................... IV.118
Exercises for §3 .......................................................... IV.120
Exercises for §4 .......................................................... IV.120
Exercises for §5 .......................................................... IV.127
Exercises for §6 .......................................................... IV.134
Exercises for §7 .......................................................... IV.142

CHAPTER V. — Integration of measures ............................ V.1

§1. Essential upper integral ............................................. V.2
    1. Definition of the essential upper integral ................. V.2
    2. Moderated functions and measures .......................... V.4
    3. Essentially integrable functions ............................. V.7
    4. A property special to the essential upper integral ...... V.10

§2. Summable families of positive measures ....................... V.11
    1. Definition of summable families of measures ............. V.11
    2. Integration with respect to a sum of positive measures . V.12
    3. Decomposition of a measure as a sum of measures with compact support ............................................. V.14

§3. Integration of positive measures ................................. V.15
    1. Functions with values in a space of measures ............. V.15
    2. Superimposed integrals of positive functions ............. V.20
    3. Superimposed integrals of functions with values in a Banach space ............................................. V.24

4. Universally measurable functions ......................... V.25
5. Diffusions .................................................. V.26
6. Composition of bounded diffusions ....................... V.29

§4. Integration of positive point measures ................. V.31
    1. Families of point measures ............................. V.31
    2. Upper integrals of positive functions with respect to an integral of point measures ......................... V.33
    3. Measurability with respect to an integral of point measures .................................................... V.35
    4. Integration of functions with values in a Banach space, with respect to an integral of point measures .......... V.37

§5. Measures defined by numerical densities ................. V.38
    1. Locally integrable functions ............................ V.38
    2. Measures defined by numerical densities ................. V.40
    3. Integration with respect to a measure defined by a density ..................................................... V.42
    4. Behavior of the product with respect to the usual operations ..................................................... V.45
    5. Characterization of measures with base $\mu$ ........ V.48
    6. Equivalent measures ...................................... V.52
    7. Alien measures ........................................... V.54
    8. Applications: I. Duality of the spaces $L^p$ .......... V.56
    9. Applications: II. Functions of measures ................. V.60
    10. Diffuse measures; atomic measures ..................... V.61

§6. Images of a measure ....................................... V.62
    1. Image of a positive measure ............................ V.62
    2. Integration with respect to the image of a positive measure .................................................. V.64
    3. Properties of the image of a positive measure ........ V.65
    4. Image of a complex measure ............................. V.68
    5. Application: change of variable in the Lebesgue integral ....................................................... V.69
    6. Decomposition into slices. Inverse image of a measure under a local homeomorphism ....................... V.71

§7. Integration with respect to an induced measure .......... V.74
    1. Integration with respect to an induced measure ........ V.74
    2. Properties of induced measures .......................... V.77

§8. Products of measures ............................................. V.79
    1. Interpretation of the product measure as an integral of measures ............................................. V.79
    2. Functions measurable with respect to a product of two measures ............................................. V.81
    3. Integration of positive functions ............................................. V.83
    4. Integration of functions with values in a Banach space ............................................. V.87
    5. Operations on the product of two measures ............... V.89
    6. Integration with respect to a finite product of measures ............................................. V.91
    7. Application: Measure of the Euclidean ball in $\mathbf{R}^n$ ...... V.93
Exercises for §1 ............................................. V.94
Exercises for §2 ............................................. V.95
Exercises for §3 ............................................. V.96
Exercises for §4 ............................................. V.99
Exercises for §5 ............................................. V.99
Exercises for §6 ............................................. V.107
Exercises for §7 ............................................. V.112
Exercises for §8 ............................................. V.114
Historical note ............................................. V.123

CHAPTER VI. — Vectorial integration ......................... VI.1

§1. Integration of vector-valued functions .................. VI.1
    1. Scalarly essentially integrable functions ............... VI.2
    2. Properties of the integral of a scalarly essentially integrable function ............................................. VI.5
    3. Integrals of operators ............................................. VI.7
    4. The property (GDF) ............................................. VI.9
    5. Measurable mappings and scalarly measurable mappings ............................................. VI.12
    6. Applications: I. Extension of a continuous function to a space of measures ............................................. VI.13
    7. Applications: II. Extension, to a space of measures, of a continuous function with values in a space of operators ............................................. VI.15

§2. Vectorial measures ............................................. VI.18
    1. Definition of a vectorial measure ....................... VI.18
    2. Integration with respect to a vectorial measure ........ VI.20
    3. Majorizable vectorial measures .......................... VI.22

4. Vectorial measures with base $\mu$ ......................... VI.25
5. The Dunford–Pettis theorem ................................. VI.27
6. Dual of the space $L^1_F$ (F a separable Banach space .................................................. VI.32
7. Integration of a vector-valued function with respect to a vectorial measure ............................................. VI.33
8. Complex measures ............................................. VI.34
9. Bounded complex measures ................................. VI.37
10. Image of a complex measure; induced complex measure; product of complex measures ............................ VI.39

§3. Disintegration of measures ........................................ VI.40
    1. Disintegration of a measure $\mu$ relative to a $\mu$-proper mapping .................................................. VI.40
    2. Pseudo-image measures ........................................ VI.44
    3. Disintegration of a measure $\mu$ relative to a pseudo-image of $\mu$ .................................................. VI.45
    4. Measurable equivalence relations .......................... VI.46
    5. Disintegration of a measure by a measurable equivalence relation .................................................. VI.50

Appendix: Complements on topological vector spaces ........ VI.52
    1. Bilinear forms and linear mappings ....................... VI.52
    2. Some types of spaces having the property (GDF) ....... VI.54

Exercises for §1 .................................................. VI.56
Exercises for §2 .................................................. VI.62
Exercises for §3 .................................................. VI.69
Historical note .................................................. VI.72
Index of notations ............................................... 451
Index of terminology ........................................... 455
