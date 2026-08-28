---
book: alg
book_title: Algebra
chapter: IX
chapter_title: Formes sesquilinéaires et formes quadratiques
section: 0
section_title: Historical Note
kind: historical
lang: en
source: alg-ix-fr
pdf_pages: 0183-0211
extraction: ocr
statements: 0
exercises: 0
content_sha256: 96a9a896244bade60040730d2127977ca4bc1d54a5b86e061439866ff8d0ed82
translated_from: content/fr/alg/IX/historical_note.md
source_lang: fr
translation_method: machine
source_content_sha256: 5dc4068f333e2b8735cdbf6a3b58a2c5f076b92da97ed7fef97bf5e366c8fdc7
translation_model: gpt-5-6-mini, gpt-5.4
translation_run: translate-en-mt-8d9189fc
glossary_version: 34
glossary_terms_sha256: c1defa46516a1c4d2b4dc66b210906913dcdd38f92e7c1cc9111987bead579b8
prompt_sha256: 5b9b7144015934413fe8e16b5155e2bc50bed2041525e1b1db7c19a297193094
---

# HISTORICAL NOTE

(N.B. — The Roman numerals refer to the bibliography placed at the end of this note.)

The theory of quadratic forms, in its modern aspect, scarcely goes back beyond the second half of the xviii\textsuperscript{e} century, and, as we shall see, it was developed chiefly in response to the needs of Arithmetic, Analysis and Mechanics. But the fundamental notions of this theory in reality made their appearance from the beginnings of «Euclidean» geometry, of which they form the framework. For this reason, its history cannot be traced without speaking, at least in summary fashion, of the development of «elementary geometry» since antiquity. Of course, we shall be able to concern ourselves only with the evolution of a few general ideas, and the reader should not expect to find here precise information on the history of any particular theorem, for which it will suffice to refer him to the specialised historical or didactic works (*). It goes without saying also that, when we speak below of the various possible interpretations of the same theorem in various algebraic or geometrical languages, we do not at all mean to say that these «translations» were at all times as familiar as they are today; on the contrary, it is the principal purpose of this Note to show how, very gradually, mathematicians became aware of these relationships between questions of often very different appearance; we shall also have to show how, in so doing, they were led to introduce some coherence into the mass of geometrical theorems handed down by the ancients, and finally to try to delimit exactly what was to be understood by «geometry».

(*) See (II), as well as E. Kötter, Die Entwicklung der synthetischen Geometrie, Leipzig (Teubner), 1901 (= Jahresber. der Deutschen Math. Verein., t. V, 1\textsuperscript{tes} Heft), and the Enzyklopädie der Math. Wiss., 1\textsuperscript{re} éd., t. III.

If we set aside the discovery, by the Babylonians, of the formula for solving the quadratic equation ((I), p. 183-189), it is therefore under their geometrical guise that the birth of the principal concepts of the theory of quadratic forms must be noted. These first appear as squares of distances (in the plane or three-dimensional space) and the corresponding notion of «orthogonality» is introduced by means of the right angle, defined by Euclid as half the flat angle (Elements, Book I, Def. 10); the notions of distance and right angle being linked by the theorem of Pythagoras, keystone of the Euclidean edifice (*). The idea of angle seems to have been introduced very early into Greek mathematics (which no doubt received it from the Babylonians, accustomed to the use of angles through their long astronomical experience). It is known that in the classical period only angles less than 2 right angles are defined (Euclid's «definition» is moreover as vague and unusable as the one he gives for the right or the plane); the notion of orientation is not brought out, although Euclid uses (without axiom or definition) the fact that a right divides the plane into two regions, which he carefully distinguishes when necessary (**). At this stage, the idea of the group of plane rotations therefore emerges only in a very imperfect manner, through the addition (also introduced without explanation by Euclid) of the unoriented angles of half-lines, which is defined, in principle, only when the sum is at most equal to two right angles (***) As for trigonometry,

(*) Most of the ancient civilisations (Egypt, Babylonia, India, China) seem to have arrived independently at statements covering at least certain particular cases of the «theorem of Pythagoras», and the Hindus even had the idea of principles of proof of this theorem quite distinct from those found in Euclid (who gives two proofs of it, one by construction of auxiliary figures, the other using the theory of proportions) (cf. (II), t. IV, p. 135-144).

(**) The notion of an oriented angle, with its various variants (angle of lines, angle of half-lines) appeared only very late. In analytical geometry, Euler ((VIII a), p. 217-239 and 305-307) introduced polar coordinates, and the modern conception of an angle (measured in radians) taking arbitrary values (positive or negative). L. Carnot (Géométrie de Position, Paris, 1803) inaugurated the tendency which, throughout the XIXth century, was to oppose «synthetic» geometry to analytical geometry; seeking to develop the former as independently as possible, he was led, in order to avoid the «configurations» of the ancient geometers, to introduce systematically oriented magnitudes, lengths and angles; unfortunately, his work is considerably complicated by his determination not to use negative numbers (which he regarded as contradictory!) and to replace them by an unwieldy system of «correspondence of signs» between various figures. One must wait for Möbius (XIII c) for the concept of an oriented angle to be introduced into the reasoning of synthetic geometry; however, like his successors until a very recent period, he knows how to introduce orientation only by a direct appeal to spatial intuition (the so-called «Ampère little man» rule); it was only with the development of n-dimensional geometry and algebraic topology that one finally arrived at a rigorous definition of an «oriented space».

(***) There are nevertheless at least two passages in Euclid where he speaks of angles whose “sum” can exceed 2 right angles, namely the inequalities satisfied by the faces of a trihedral angle (Elements, Book XI, prop. 20 and 21) (not to mention it is scorned by geometers, and left to surveyors and astronomers; it is the latter (Aristarchus, Hipparchus, Ptolemy especially (V)) who establish the fundamental relations between sides and angles of a right-angled triangle (plane or spherical) and draw up the first tables (these are tables giving the chord of the arc cut off by an angle $\theta < \pi$ on a circle of radius $r$, in other words the number $2r \sin \frac{\theta}{2}$; the introduction of the sine, which is more convenient to use, is due to the Hindu mathematicians of the Middle Ages); in the calculation of these tables, the formula for the addition of arcs, unknown at that time, is replaced by the equivalent use of Ptolemy’s theorem (perhaps going back to Hipparchus) on quadrilaterals inscribed in a circle (cf. Esp. vect. top., chap. V, § 1, exerc. 5). It should also be noted that Euclid and Heron give propositions equivalent to the formula

$$
a^2 = b^2 + c^2 - 2bc \cos A
$$

between sides and angles of an arbitrary plane triangle; but one can hardly see in this a first appearance of the notion of a bilinear form associated with a metric form, for want of the idea of a vector calculus which would not emerge until the xixe century.

The displacements (or motions, the distinction between the two notions not being clear in antiquity — nor even much later) are known to Euclid; but, for reasons unknown to us, he seems to have a marked reluctance to make use of them (for example in the “cases of equality of triangles”, where one has the impression that he employs the notion of displacement only because he did not know how to formulate an appropriate axiom ((III bis), t. I, p. 225-227 and 249)); nevertheless, it is to the notion of displacement (rotation about an axis) that he has recourse for the definition of cones of revolution and spheres (Elements, Book XI, def. 14 and 18), as does Archimedes for that of quadrics of revolution. But the general idea of transformation, applied to the whole of space, is more or less foreign to mathematical thought before the end of the xviiie century (*);

of the “reasoning” concerning the “measurement” of angles, which is undoubtedly an interpolation (cf. Note hist. of Book III, chap. viii)); in these two passages, Euclid thus appears to be carried by intuition beyond what his own definitions permit. His successors are even less scrupulous, and Proclus, for example (ve century A.D.) does not hesitate to state the general “theorem” giving the sum of the angles of a convex polygon ((III bis), t. I, p. 322).

(*) One can hardly cite as examples of such a notion anything but the “projections” of cartographers and draughtsmen; the stereographic projection (§ 10, exerc. 14) is known to Ptolemy (and in the xviie century it was known that it preserves angles), and the central projection plays a leading role in the work of Desargues (VI); but this is a correspondence between the whole of space (or a surface) and a plane. One of the properties of inversion, which we express today by saying that the transform of a circle is a circle or a right line (cf. § 10, exerc. 13), is known in substance to Viète, and was used by him in problems of construction of circles; but neither he, nor Fermat, who extended his constructions to spheres, had the idea of introducing inversion as a transformation of the plane or of space.

and before the xvii\textsuperscript{e} century, there is no trace either of the notion of composition of motions, nor, a fortiori, of composition of displacements. This does not mean, of course, that the Greeks were not particularly sensitive to the “regularities” and “symmetries” of figures, which we now relate to the notion of group of displacements; their theory of regular polygons and still more that of regular polyhedra — one of the most remarkable chapters of all their mathematics — is there to prove the contrary (*).

Finally, the last of the essential contributions of Greek mathematics, in the field that concerns us, is the theory of conics (as regards quadrics, the Greeks know only certain quadrics of revolution, and do not carry their study very far, except for the sphere). It is interesting to note here that, though the Greeks never had any idea of the fundamental principle of analytic geometry (essentially for want of a workable algebra), they commonly used, for the study of particular «figures», the «ordinates» with respect to two (or even more than two) axes in the plane (in close relation with the figure, which is one of the fundamental points where their method differs from that of Fermat and Descartes, whose axes are fixed independently of the figure considered). In particular, the first examples of conics (other than the circle) which arise in connection with the problem of the duplication of the cube, are the curves given by the equations $y^2 = ax$, $y = bx^2$, $xy = c$ (Menaechmus, pupil of Eudoxus, middle of the iv\textsuperscript{e} century) (**); and it is the equation of the conics (usually with respect to two oblique axes formed by a diameter and the tangent at one of its points of intersection with the curve) which is most often used in the study of problems relating to these curves (whereas the «focal» properties play only a very minor role, contrary to what might be suggested by scholastic traditions dating back only to the xixe century). Of this vast theory, we must retain here above all the notion of conjugate diameters (already known to Archimedes), and the property which now serves as the definition of the polar of a point, given by Apollonius (IV) when the point is exterior to the conic (the polar thus being for him the right line joining the points of contact of the tangents drawn from this point); from our point of view, these are two examples of «orthogonality» with respect to a quadratic form distinct from the metric form, but of course the connection between these notions and the classical notion of perpendiculars could absolutely not be conceived at that time.

There is scarcely any other progress to mention before Descartes and Fermat; but from the beginnings of analytic geometry, the algebraic theory of

(*) See on this subject A. Speiser, Theorie der Gruppen von endlicher Ordnung, Basel (Birkhäuser), 4e édit., 1956, where one will also find interesting remarks on the relations between the theory of groups of displacements and the various types of ornaments imagined by the civilisations of antiquity and the Middle Ages.

(**) It seems that the idea of considering these curves as plane sections of cones with circular base (also due to Menaechmus) is subsequent to their definition by means of the preceding equations (cf. (IV), p. xvii-xxx).

quadratic forms begins to emerge from its geometrical husk: Fermat knows that an equation of the second degree in the plane represents a conic ((VII a), p. 100-102) and sketches analogous ideas concerning quadrics (VII b). With the development of analytic geometry in 2 and 3 dimensions during the xviiie century there appear (especially in connection with conics and quadrics) two of the central problems of the theory: the reduction of a quadratic form to a sum of squares and the determination of its «axes» with respect to the metric form. For conics, these two problems are too elementary to give rise to important algebraic progress; for an arbitrary number of variables, the first is solved by Lagrange in 1759, in connection with the maxima of functions of several variables (IX a). But this problem is almost immediately eclipsed by that of determining the axes, even before the invariance of the rank had been formulated (*) ; as for the law of inertia, it is not discovered until about 1850 by Jacobi (XIX b), who proves it by the same reasoning as at present, and Sylvester (XX) who merely states it as quasi-obvious (**).

The problem of reducing a quadric to its axes already presents considerably greater algebraic difficulties than the analogous problem for conics; and Euler, who is the first to tackle it, is not in a position to prove the reality of the eigenvalues, which he accepts after a sketch of a justification without probative value ((VIII a), p. 379-392) (***)). If this point is correctly established about 1800, one must wait for Cauchy to prove the corresponding theorem for forms in an arbitrary number $n$ of variables (XIV b). It is also Cauchy who, at about the same period, proves that the characteristic equation giving the eigenvalues is invariant under every change of rectangular axes ((XIV a), p. 252) (****)) ; but for $n = 2$ or $n = 3$, this inva-

(*) Dealing with a problem independent, by its nature, of the choice of coordinate axes, Lagrange could not fail to observe that his procedure involved much arbitrariness, but the notions needed to make this idea precise are still lacking: «Besides», he says, «in order not to be mistaken in these researches, it should be remarked that the transforms [as a sum of squares] might well turn out different from those which we have given; but, on examining the matter more closely, one will infallibly find that, whatever they may be, they can always be reduced to these, or at least be comprised therein [?]» ((IX a), p. 8).

(**) Gauss had arrived at this result independently, and demonstrated it in his lectures on the method of least squares, as testified by Riemann, who attended these lectures in 1846–47 (B. Riemann, Gesammelte Werke, Nachträge, Leipzig (Teubner), 1902, p. 59).

(***) He was more successful in determining the principal axes of inertia of a solid: having reduced the problem to an equation of the third degree, he observes that such an equation has at least one real root, hence that there is at least one axis of inertia; taking this axis as the axis of coordinates, he is then reduced to the plane problem, whose solution is easy ((VIII b), p. 200-202).

(****) It should be noted that, until about 1930, by « quadratic form » one always meant a homogeneous polynomial of the second degree in the coordinates taken with respect to a given system of axes. It seems that it was only the theory of Hilbert space that led to an « intrinsic » conception of quadratic forms, even in spaces of finite dimension.

variance was intuitively « obvious » by reason of the geometrical interpretation of the eigenvalues by means of the axes of the corresponding conic or quadric. Moreover, in the course of research on this subject, the elementary symmetric functions of the eigenvalues had also presented themselves naturally (with various geometrical interpretations, in particular in connection with Apollonius's theorems on conjugate diameters), and in particular the discriminant, which (known for a long time for $n = 2$ in connection with the theory of the equation of the second degree) appears for the first time for $n = 3$ in Euler ((VIII a) p. 382); the latter encounters it in connection with the classification of quadrics (in expressing the condition that a quadric have no point at infinity) and does not mention its invariance with respect to changes of rectangular axes. But somewhat later, with the beginnings of the arithmetic theory of quadratic forms with integral coefficients, Lagrange notes (for $n = 2$) a particular case of invariance of the discriminant under a change of variables that is linear but not orthogonal ((IX b), p. 699), and Gauss establishes, for $n = 3$, the « covariance » of the discriminant under any linear transformation ((XI a), p. 301-302) (*). Once the general formula for multiplication of determinants had been proved by Cauchy and Binet, the extension of Gauss's formula to any number of variables was immediate; it was this that, about 1845, was to give the first impetus to the general theory of invariants.

To the two notions which, among the Greeks, served in place of the theory of displacements — that of motion and that of « symmetry » of a figure — a third was added in the eighteenth and nineteenth centuries with the problem of changing rectangular axes, which is essentially equivalent to this theory. Euler devoted several works to this question, concentrating especially on obtaining convenient parametric representations for the formulas for changing axes. It is known what use Mechanics was to make of the three angles which he introduced for this purpose for $n = 3$ ((VIII a), p. 371-378). But he did not stop there, considering in 1770 the general problem of orthogonal transformations for arbitrary $n$, observing that here the goal could be attained by introducing $n(n-1)/2$ angles as parameters, and finally, for $n = 3$ and $n = 4$, giving rational representations for rotations (in terms, respectively, of 4 homogeneous parameters and of 8 homogeneous parameters linked by a relation), which are none other than those obtained later by means of the theory of quaternions (cf. § 9, exerc. 15 and 16), and whose origin he does not indicate (VIII c) (**).

(*) It was also in connection with this research that Gauss defined the inverse of a quadratic form ((XI a), p. 301) and obtained the condition for positivity of such a form (§ 7, no 1, prop. 3), involving a sequence of principal minors of the discriminant (ibid., p. 305-307).

(**) Euler does not, moreover, give the formula for the composition of rotations expressed with the aid of these parameters; for $n = 3$, it is not found before a note by Gauss (not published during his lifetime (XI b)) and a work by Olinde Rodrigues of 1840, which rediscovers Euler's parametric representation, almost forgotten at that time.

On the other hand, Euler also indicates how to translate analytically the research into the «symmetries» of plane figures, and it is in this connection that he is led to prove, in substance, that a plane displacement is a rotation, or a translation, or a translation followed by a symmetry ((VIII a), p. 197-199). The development of Mechanics at this time moreover leads to the general study of displacements; but at first only «infinitely small» displacements tangent to continuous movements are considered: these are apparently the only ones which occur in the research of Torricelli, Roberval and Descartes on the composition of movements and the instantaneous centre of rotation for plane movements (cf. Note hist. du Livre IV, chap. I-II-III). The latter is defined in general by Johann Bernoulli; d’Alembert in 1749, and Euler the following year, extend this notion by proving the existence of an instantaneous axis of rotation for movements leaving a fixed point. The analogous theorem for finite displacements is not stated until 1775 by Euler (VIII d), in a memoir in which he discovers at the same time that the determinant of a rotation is equal to 1; the following year, he proves the existence of a fixed point for plane similarities (VIII e). But it is necessary to await the work of Chasles, beginning in 1830 (XV a), to have at last a coherent theory of finite and infinitely small displacements.

We thus arrive at what may be called the golden age of geometry, which falls roughly between the dates of publication of Monge's Géométrie descriptive (1795) (X) and F. Klein's «Erlangen programme» (1872) (XXV b). The essential advances which we owe to this sudden revival of geometry are the following:

A) The notion of an element at infinity (point, right line or plane), introduced by Desargues in the eighteenth century (VI), but which in the eighteenth century manifested itself scarcely otherwise than as an abuse of language, is rehabilitated and systematically used by Poncelet (XII), who thus makes projective space the general setting for all geometrical phenomena.

B) At the same time, with Monge, and above all Poncelet, the passing to complex projective geometry takes place. The notion of an imaginary point, sporadically used during the eighteenth century, is here exploited (concurrently with that of a point at infinity) to give statements independent of the «cases of figure» of real affine geometry. If at first the justifications advanced in support of these innovations remain very confused (especially on the part of the adherents of the «synthetic» school of geometry, where the use of coordinates comes to be regarded as a defilement), one cannot fail to recognize there, under the name of «principle of contingent relations» in Monge, or of «principle of continuity» in Poncelet, the first germ of the idea of «specialization» of modern algebraic geometry (*).

(*) These «principles» are of course justified (as Cauchy had already remarked) by application of the principle of prolongation of algebraic identities,

One of the first results following from these conceptions is the remark that, in complex projective space, all non-degenerate conics (resp. quadrics) are of the same nature; this leads Poncelet to the discovery of the «isotropic» elements: «Circles arbitrarily placed on a plane», he says, «are therefore not quite independent of one another, as one might believe at first sight, they have ideally two common imaginary points at infinity» ((XII), p. 48). Further on, he analogously introduces the «umbilical», an imaginary conic at infinity common to all spheres ((XII), p. 370); and although he does not specifically speak of the isotropic generators of the sphere, he does explicitly emphasize the existence of rectilinear generators, real or imaginary, for all quadrics (ibid., p. 371) (*); notions which his continuators (notably Plücker and Chasles), even more than he himself, make extensive use of, in particular in the study of the «focal» properties of conics and quadrics.

C) The notions of point transform and composition of transforms are likewise formulated in a general way and systematically introduced as means of proof. Apart from displacements and projections, only a few particular transforms were known at that time: certain plane projective transforms, of the type $x' = a/x, y' = y/x$, used by La Hire and Newton, the “affinity” $x' = ax, y' = by$ of Clairaut and Euler, and finally a few particular quadratic transforms, again in Newton, Maclaurin and Braikenridge. Monge, in his Géométrie descriptive, shows all the use that can be made of plane projections in geometry in 3 dimensions. In Poncelet, one of the systematic methods of proof, employed to excess, consists in reducing by projection the properties of conics to those of the circle (a method already applied occasionally by Desargues and Pascal); and in order to be able analogously to pass from a quadric to a sphere, he invents the first example of a projective transform in space, the “homology” ((XII), p. 357); finally, he is also the one who introduces the first examples of birational transforms of a curve into itself. In 1827, Möbius ((XIII a), p. 217) (and independently Chasles in 1830 (XV b)) define the most general projective linear transforms; at the same time inversion appears (cf. § 10, exerc. 13) as well as other types of quadratic transforms, whose study is to inaugurate the theory of birational transforms, which will develop in the second half of the 19th century.

D) The notion of duality appears in full light and is consciously linked with the theory of bilinear forms. The theory of

by reason of the fact that “synthetic” geometers never consider anything but properties which translate analytically into identities of this nature.

(*) The first mention of the rectilinear generators of quadrics seems to be due to Wren (1669), who observes that the one-sheeted hyperboloid of revolution can be generated by the rotation of a right line about an axis not in the same plane; but their study was developed only by Monge and his school.

poles and polars with respect to conics, which, since Apollonius, had made some progress only with Desargues and La Hire, is extended to quadrics by Monge, who, together with his pupils, perceives the possibility of transforming known theorems by this means into new results (*). But it is again Poncelet to whom is due the merit of having raised these remarks to the status of a general method in his theory of transforms “by reciprocal polars”, and of having made of them a particularly effective tool of discovery. A little later, notably with Gergonne, Plücker, Möbius and Chasles, the general notion of duality disengages itself from the link with quadratic forms, still too close in Poncelet. In particular, Möbius, on examining the various possibilities of duality in space of 3 dimensions (defined by a bilinear form), discovers in 1833 duality with respect to an alternating bilinear form (XIII b) (**), studied chiefly, in the 19th century, in the form of the theory of “linear complexes” (cf. § 10, exerc. 16) and developed in relation to the “geometry of right lines” and the “Plückerian coordinates” introduced by Cayley, Grassmann and Plücker around 1860.

E) From the beginnings of projective geometry, the intensive study of the properties of classical geometry in their relations with projective space had quickly led to dividing them into “projective properties” and “metric properties”; and it is doubtless not an exaggeration to see in this separation one of the clearest manifestations, at that time, of what was to become the modern notion of structure. But Poncelet, who first introduces this distinction and this terminology, is already aware of what links these two types of properties; and, in dealing in his Traité with problems concerning angles, whose properties “do not seem to form part of those which we have called projective..., they nevertheless follow in so simple a manner”, he says, “from the principles which form the basis [of this work]..., that I do not believe that any other geometrical theory could lead to them in a manner at once more direct and more simple. There will be nothing surprising in this, if one considers that the projective properties of figures are necessarily the most general of those which can belong to them; so that they must include, as simple corollaries, all the other particular properties or relations of extent” ((XII), p. 248). To tell the truth, after this declaration, one is somewhat surprised to see him approach questions concerning angles in a very roundabout fashion, by linking them with the focal properties of conics, instead of directly introducing the cyclic points; and in fact, it was only 30 years later that Laguerre (still a pupil at the École Polytechnique) gave the expression for an angle of right lines by means of the cross-ratio of these right lines and the isotropic right lines of the same origin (cf. § 10, exerc. 5) ((XXI), t. II, p. 13). Finally, with Cayley (XVIII d) there is clearly expressed-

(*) The best known is Brianchon’s theorem (1810), transformed from Pascal’s theorem by duality.
(**) In 1828, Giorgini had already encountered polarity with respect to an alternating form, in connection with a problem in Statics (Mem. Soc. Ital. Modena, t. XX (1828), p. 243-254).

Bourbaki XXIV.

thus the fundamental idea that the “metrical” properties of a plane figure are nothing but the “projective” properties of the figure enlarged by the cyclic points - a decisive landmark towards the “Erlangen programme”.

F) Hyperbolic non-euclidean geometry, which came into being about 1830, at first remained somewhat apart from the movement whose broad lines we are tracing. Arising from essentially logical preoccupations touching the foundations of classical geometry, this new geometry was presented by its inventors (*) in the same axiomatic and “synthetic” form as Euclidean geometry, and without connection with projective geometry (the introduction of which after the classical model even seemed excluded a priori, since the notion of a unique parallel disappears in this geometry); doubtless for that reason it attracted but little, for a long time, the interest of the French, German and English schools of projective geometry. Thus, when Cayley, in the fundamental memoir cited above (XVIII d), conceived the idea of replacing the cyclic points (considered as a “tangentially degenerate” conic) by an arbitrary conic (which he called the “absolute”), he did not in the least think of connecting this idea with the geometry of Lobatschevsky-Bolyai, although he indicated how his conception leads to new expressions for the “distance” of two points, and although he mentioned its links with spherical geometry. The situation changed about 1870, when the non-euclidean geometries, following upon the diffusion of the works of Lobatschevsky, and the publication of the works of Gauss and of Riemann’s inaugural lecture, had come to the forefront of mathematical actuality. Following the path marked out by Riemann, Beltrami, without knowing Cayley’s work, rediscovered in 1868 the expressions for distance given by the latter, but in an altogether different context, by considering the interior of a circle as an image of a surface of constant curvature, in which the geodesics are represented by straight lines (XXIV); it was Klein who, two years later, made (independently of Beltrami) the synthesis of these various points of view, which he completed by the discovery of elliptic non-euclidean space (XXV a) (**).

G) In the second half of the period which we are considering here, there was established a period of critical reflection, during which the partisans of “synthetic” geometry, not content with having banished coordinates from their proofs, claimed to dispense with real numbers

(*) It is known that Gauss, as early as 1800, had become convinced of the impossibility of proving Euclid’s postulate, and of the logical possibility of developing a geometry in which this postulate would not be satisfied. But he did not publish his results on this question, and these were rediscovered independently only by Lobatschevsky in 1829 and Bolyai in 1832. For more details, see F. Engel-P. Stäckel, Die Theorie der Parallellinien von Euklid bis auf Gauss, Leipzig (Teubner), 1895, and Urkunden zur Geschichte der nichteuclidischen Geometrien, 2 vol., Leipzig (Teubner), 1898-1913.

(**) The example of spherical geometry had for some time caused it to be believed that, in a space of constant positive curvature, there always exist pairs of points through which more than one geodesic passes.

even in the axioms of geometry. The principal representative of this school is von Staudt, who essentially succeeded in performing this tour de force (XXIII), much admired in his time and even well on in the xx\textsuperscript{e} century; and if today one no longer attributes the same importance to ideas of this order, whose possibilities of fruitful application have proved rather scanty, it must nevertheless be recognized that the efforts of von Staudt and his disciples contributed to clarifying ideas on the role of real or complex “scalars” in classical geometry, and thereby to introducing the modern conception of geometries over an arbitrary base field.

Around 1860, “synthetic” geometry is at its apogee, but the end of its reign is rapidly approaching. Having remained heavy and ungainly throughout the xviii\textsuperscript{e} century, analytic geometry, in the hands of Lamé, Bobillier, Cauchy, Plücker and Möbius, finally acquires the elegance and concision which will enable it to compete on equal terms with its rival. Above all, from about 1850 onwards, the ideas of group and invariant, finally formulated with precision, gradually invade the scene, and it is realized that the theorems of classical geometry are nothing other than the expression of identical relations between invariants or covariants of the group of similarities (*), analogously to those of projective geometry, which express the identities (or “syzygies”) between covariants of the projective group. This is the thesis masterfully expounded by F. Klein in the celebrated “Erlangen programme” (XXV b), where he advocates abandoning the sterile controversies between the “synthetic” and “analytic” tendencies; if, he says, the accusation made against the latter of giving a privileged role to a system of arbitrary axes “was only too often justified as regards the defective manner in which the method of coordinates was formerly used, it collapses when it is a question of a rational application of this method... The domain of spatial intuition is not forbidden to the analytic method...”, and he emphasizes that “one must not underestimate the advantage which a well-adapted formalism brings to subsequent research, in that it, so to speak, anticipates thought” ((XXV b), p. 488-490).

We thus arrive at a rational and “structural” classification of the theorems of “geometry” according to the group to which they belong: linear group for projective geometry, orthogonal group for metric questions, symplectic group for the geometry of the “linear complex”. But beneath this ruthless clarity, classical geometry — with the exceptions of algebraic geometry and differential geometry (**), now constituted as autonomous sciences — rapidly withers and loses all its brilliance. The generalization of methods based on the use of transformations had already made the formation of new theorems somewhat mechanical: “Today”, says Chasles in 1837 in his Aperçu historique, “anyone can come forward, take any known truth, and subject it to the various general principles of transformation; he will derive other truths from it, different or more general; and these will be susceptible of similar operations; so that one will be able to multiply, almost indefinitely, the number of new truths deduced from the first… Anyone may therefore, in the present state of science, generalize and create in Geometry; genius is no longer indispensable for adding a stone to the edifice” ((XV b), p. 268-269). But the situation becomes much clearer with the progress of the theory of invariants, which finally succeeds (at least for the “classical” groups) in formulating general methods making it possible in principle to write down all algebraic covariants and all their “syzygies” in a purely automatic manner; a victory which, at the same time, marks the death, as a field of research, of the classical theory of invariants itself, and of “elementary” geometry, which has become practically a mere dictionary of it. No doubt, there is nothing to enable one to foresee a priori, among the infinity of “theorems” which can thus be unfolded at will, which will have a statement, in an appropriate geometrical language, of a simplicity and elegance comparable with the classical results, and there remains here a restricted domain in which numerous amateurs continue to exercise themselves successfully (geometry of the triangle, of the tetrahedron, of algebraic curves and surfaces of low degree, etc.). But for the professional mathematician, the mine is exhausted, since there are no longer any problems of structure there, capable of having repercussions on other parts of mathematics; and this chapter of the theory of groups and invariants may be considered closed until further notice. (*)

**

Thus, after the Erlangen programme, euclidean and non-euclidean geometries, from the purely algebraic point of view, have become simple languages, more or less convenient, for expressing the results

(*) For example, the first members of the equations of the three altitudes of a triangle are covariants of the three vertices of the triangle for the group of similarities, and the theorem asserting that these three altitudes have a common point is equivalent to saying that the three covariants in question are linearly dependent.

(**) We do not have here to give the history of these two disciplines, nor to examine in detail the influence of the “Erlangen programme” on their development.

subsequently. Let us merely mention that algebraic geometry, after more than 100 years of research, is being studied more actively than ever; as for differential geometry, after a brilliant flowering with Lie, Darboux and their disciples, it seemed threatened with the same sclerosis as classical elementary geometry, when contemporary work (taking its chief origin from the ideas of E. Cartan) on fibre spaces and “global” problems came to restore all its vitality.

(*) Of course, this inevitable decline of geometry (Euclidean or projective), which seems obvious to our eyes, remained unnoticed by contemporaries for a long time, and until about 1900 this discipline continued to appear as an important branch of mathematics, as is shown, for example, by the place it occupies in the Enzyklopädie; until recent years, it still occupied this place in University teaching.

of the theory of bilinear forms, whose progress goes hand in hand with that of the theory of invariants (*). Everything concerning the notion of rank of a bilinear form and the relations between these forms and linear transformations was definitively clarified by the work of Frobenius (XXVII a). It is also to Frobenius that we owe the canonical expression of an alternating form on a $\mathbf{Z}$-free module ($\S 5,$ n° 1, th. 1) (XXVII b); however, skew-symmetric determinants had already appeared in Pfaff, at the beginning of the century, in connection with the reduction of differential forms to a normal form; Jacobi, who, in 1827, took up this problem again (XIX a), knew that a skew-symmetric determinant of odd order is zero, and it was he who formed the expression for the Pfaffian and showed that it is a factor of the skew-symmetric determinant of even order; but he had not perceived that the latter is the square of the Pfaffian, and this point was established only by Cayley in 1849 (XVIII b). The notion of a symmetric bilinear form associated with a quadratic form is the most elementary case of the process of “polarization”, one of the fundamental tools of the theory of invariants. Under the name of “scalar product”, this notion was to enjoy immense success, first with the popularizers of “vector calculus”, then, from the xx\textsuperscript{e} century onwards, thanks to the unsuspected generalization brought by the theory of Hilbert space (see Historical Note of Book V). It is also this latter theory that was to bring to light the notion of adjoint of an operator (which previously had hardly manifested itself except in the theory of linear differential equations, and, in tensor calculus, through the alternation of the covariant and contravariant indices under the direction of the metric tensor); finally, it was this theory that was to give its full prominence to the notion of Hermitian form, first introduced by Hermite in 1853 in connection with arithmetical investigations ((XXII), p. 237), but which remained somewhat on the margin of the great mathematical currents until around 1925 and the applications of complex Hilbert spaces to quantum theories.

The study of the orthogonal group and the group of similarities — clearly conceived and treated as such since the middle of the xix\textsuperscript{e} century, and having become the heart of the theory of quadratic forms — as well as that of the other “classical” groups (linear group, symplectic group and unitary group), is, on the other hand, acquiring increasing importance. We can only mention here the essential role played by these groups, in the theory of Lie groups and differential geometry on the one hand, the arithmetic theory of quadratic forms (see for example (XXXIII) and (XXXV)) on the other (**); to this circumstance, as well as to

(*) In particular, the interest attached to non-Euclidean geometry stems, not from this banal algebraic aspect, but rather from its relations with differential geometry and the theory of functions of complex variables; this is why, in this work, the elementary notions and definitions of non-Euclidean geometry will be introduced only in the parts dealing with these theories.

(**) Without mentioning quantum theories, where the linear representations of orthogonal groups are extensively used, or the theory of relativity, which drew attention to the “Lorentz group” (orthogonal group for a form of signature (3, 1)).

the extension of the concept of duality to the most diverse questions, is due the fact that there is scarcely any modern mathematical theory in which bilinear forms do not intervene in one way or another. We must in any case note that it was the study of the rotation group (in three dimensions) that led Hamilton to the discovery of the quaternions (XVII); this discovery was generalized by W. Clifford who, in 1876, introduced the algebras that bear his name, and proved that they are tensor products of quaternion algebras, or of quaternion algebras and a quadratic extension (XXVIII). Rediscovered four years later by Lipschitz (XXIX), who used them to give a parametric representation of the orthogonal transformations in $n$ variables (generalizing those that Cayley had obtained for $n = 3$ (XVIII a) and $n = 4$ (XVIII c) by the theory of quaternions (cf. § 9, exerc. 15 and 16)), these algebras, and the notion of “spinor” derived from them (see (XXXII) and (XXXIV)), were also to enjoy great vogue in modern times by virtue of their use in quantum theories.

It remains finally to say a word about the evolution of ideas which led to the almost total abandonment of every restriction on the ring of scalars in the theory of sesquilinear forms — a tendency common to all modern algebra, but which perhaps manifested itself here earlier than elsewhere. We have already mentioned the fruitful introduction of geometry over the field of complex numbers (which, moreover, throughout the whole of the nineteenth century, was not without a perpetual and sometimes perilous confusion between this geometry and real geometry); the clarification here stems above all from the axiomatic studies of the end of the nineteenth century on the foundations of geometry (XXX). In the course of these investigations, Hilbert and his followers, in particular, in examining the relations between the various axioms, were led to construct appropriate counter-examples, in which the “base field” (commutative or not) possessed more or less pathological properties, and they thus accustomed mathematicians to “geometries” of a wholly new type. From the analytical point of view, Galois had already considered linear transformations in which coefficients and variables took their values in a finite prime field ((XVI), p. 27); in developing these ideas, Jordan (XXVI) was naturally led to consider the classical groups over these fields, groups whose intervention is manifested in various domains of mathematics. Dickson, around 1900, extended Jordan’s researches to all finite fields, and more recently, it has been realized that a large part of the Jordan-Dickson theory extends to the case of an absolutely arbitrary “base field”; this is due essentially to the general properties of isotropic vectors and to Witt’s theorem, which, trivial in the classical cases, were established for an arbitrary base field only in 1936 (XXXI) (*).

But in thus pushing the study of sesquilinear forms towards ever greater “abstraction”, it has proved extremely suggestive to

(*) For more details on these questions, see J. Dieudonné, La géométrie des groupes classiques (Erg. der Math., Neue Folge, Heft 5, Berlin-Göttingen-Heidelberg (Springer), 1955).

retain as it stands the terminology which, in the case of spaces of 2 and 3 dimensions, came from classical geometry, and to extend it to the case of $n$-dimensional spaces and even to spaces of infinite dimension. Having been surpassed as an autonomous and living science, classical geometry has thus been transfigured into a universal language of contemporary mathematics, of incomparable flexibility and convenience.

(I) O. Neugebauer, Vorlesungen über Geschichte der antiken mathematischen Wissenschaften, Bd. I : Vorgriechische Mathematik, Berlin (Springer), 1934.
(II) J. Tropfke, Geschichte der Elementar-Mathematik, vol. IV-VI, Berlin-Leipzig (de Gruyter), 1923-24.
(III) Euclidis Elementa, 5 vol., ed. J. L. Heiberg, Lipsiae (Teubner), 1883-88.
(III bis) T. L. Heath, The thirteen books of Euclid’s Elements..., 3 vol., Cambridge, 1908.
(IV) T. L. Heath, Apollonius of Perga, Treatise on conic sections, Cambridge (Univ. Press), 1896.
(V) Ptolemaei Cl. Opera, ed. J. L. Heiberg, 2 vol., Lipsiae (Teubner), 1898-1903.
(VI) G. Desargues, Œuvres..., t. I, Paris (Leiber), 1864 : Brouillon proiect d’une atteinte aux événements des rencontres d’un cône avec un plan, p. 103-230.
(VII) P. Fermat, Œuvres, t. I, Paris (Gauthier-Villars), 1891 : a) Ad locos planos et solidos Isagoge, p. 91-110 (French trans., ibid., t. III, p. 84-101); b) Isagoge ad locos ad superficiem, p. 111-117 (French trans., ibid., t. III, p. 102-108).
(VIII) L. Euler : a) Introductio in Analysin Infinitorum (Opera Omnia (1), t. IX, Zürich-Leipzig-Berlin (O. Füssli et B. G. Teubner), 1945); b) Theoria motus corporum solidorum seu rigidorum (Opera Omnia (2), t. III, Zürich-Leipzig-Berlin (O. Füssli et B. G. Teubner), 1948); c) Problema algebraicum ob affectiones prorsus singulares memorabile (Opera Omnia, (1), t. VI, Leipzig-Berlin (Teubner), 1921, p. 287-315); d) Formulae generales pro translatione quacunque corporum rigidorum, Novi Comm. Acad. Sc. imp. Petrop., t. XX (1776), p. 189-207; e) De centro similitudinis. (Opera Omnia (1), t. XXVI, Zürich (O. Füssli), 1956, p. 276-285).
(IX) J. L. Lagrange, Œuvres, Paris (Gauthier-Villars), 1867-1892 : a) Recherches sur la méthode de maximis et minimis, t. I, p. 3-20 ; b) Recherches d’arithmétique, t. III, p. 695-795.
(X) G. Monge, Géométrie descriptive, Paris, 1798.
(XI) C. F. Gauss, Werke : a) Disquisitiones arithmeticae, t. I, Göttingen, 1870; b) Mutationen des Raumes, t. VIII, Göttingen, 1900, p. 357-362.
(XII) J.-V. Poncelet, Traité des propriétés projectives des figures, t. I, 2e ed., Paris (Gauthier-Villars), 1865.
(XIII) A. F. Möbius, Gesammelte Werke, Leipzig (Hirzel), 1885-87 : a) Der barycentrische Calcul, t. I, p. 1-388 ; b) Ueber eine besondere Art dualer Verhältnisse zwischen Figuren im Raume, t. I, p. 489-515 (= J. de Crelle, t. X, 1833); c) Ueber eine neue Behandlungsweise der analytischen Sphärik, t. II, p. 1-54.

(XIV) A.-L. Cauchy : a) Leçons sur les applications du calcul infinitésimal à la géométrie (Œuvres complètes, (2), t. V, Paris (Gauthier-Villars), 1903) ; b) Sur l’équation à l’aide de laquelle on détermine les inégalités séculaires des planètes (Œuvres complètes (2), t. IX, Paris (Gauthier-Villars), 1891, p. 174-195).
(XV) M. Chasles : a) Note sur les propriétés générales du système de deux corps, Bull. de Férussac, t. XIV (1830), p. 321-326 ; b) Aperçu historique sur l’origine et le développement des méthodes en géométrie, Bruxelles, 1837.
(XVI) E. Galois, Œuvres mathématiques, Paris (Gauthier-Villars), 1897.
(XVII) W. R. Hamilton, Lectures on Quaternions, Dublin, 1853.
(XVIII) A. Cayley, Collected Mathematical Papers, Cambridge, 1889-1898 : a) On certain results relating to quaternions, t. I, p. 123-126 (= Phil. Mag., 1845) ; b) Sur les déterminants gauches, t. I, p. 410-413 (= J. de Crelle, t. XXXVIII (1848)) ; c) Recherches ultérieures sur les déterminants gauches, t. II, p. 202-215 (= J. de Crelle, t. L (1855)) ; d) A sixth memoir on quantics, t. II, p. 561-592 (= Phil. Trans., 1859).
(XIX) C. G. J. Jacobi, Gesammelte Werke, Berlin (G. Reimer), 1881-1891 : a) Ueber die Pfaffsche Methode..., t. IV, p. 17-29 ; b) Ueber einen algebraischen Fundamentalsatz und seine Anwendungen, t. III, p. 593-598.
(XX) J. J. Sylvester, Collected Mathematical Papers, vol. I, Cambridge, 1904 : A demonstration of the theorem that every homogeneous quadratic polynomial is reducible by real orthogonal substitution to the form of a sum of positive and negative squares, p. 378-381 (= Phil. Mag., 1852).
(XXI) E. Laguerre, Œuvres, t. II, Paris (Gauthier-Villars), 1905.
(XXII) C. Hermite, Œuvres, t. I, Paris (Gauthier-Villars), 1905 : Sur la théorie des formes quadratiques, p. 200-263 (= J. de Crelle, t. XLVII (1854)).
(XXIII) K. G. V. von Staudt, Beiträge zur Geometrie der Lage, Nürnberg, 1856.
(XXIV) E. Beltrami : a) Saggio di interpretazione della geometria non-euclidea, Giorn. di Mat., t. VI (1868), p. 284-312 ; b) Teoria fondamentale degli spazii di curvatura costante, Ann. di Mat. (2), t. II (1868-69), p. 232-255.
(XXV) F. Klein, Gesammelte mathematische Abhandlungen, t. I, Berlin (Springer), 1921 : a) Ueber die sogenannte Nicht-Euklidische Geometrie, p. 254-305 (= Math. Ann., t. IV (1871)) ; b) Vergleichende Betrachtungen über neuere geometrische Forschungen, p. 460-497 (= Math. Ann., t. XLIII (1893)).
(XXVI) C. Jordan, Traité des substitutions et des équations algébriques, Paris (Gauthier-Villars), 1870.
(XXVII) G. Frobenius; a) Ueber lineare Substitutionen und bilineare Formen, J. de Crelle, t. LXXXIV (1878), p. 1-63 ; b) Theorie der linearen Formen mit ganzen Coefficienten, J. de Crelle, t. LXXXVI (1879), p. 146-208.
(XXVIII) W. K. Clifford, Mathematical Papers, London (Macmillan), 1882 : a) On the classification of geometric algebras, p. 397-401 ; b) Applications of Grassmann’s extensive algebras, p. 266-276 (= Amer. Journ. of Math., t. I (1878)).
(XXIX) R. Lipschitz, Untersuchungen ueber die Summen von Quadraten, Bonn, 1886.
(XXX) D. Hilbert, Grundlagen der Geometrie, Leipzig (Teubner), 1899.
(XXXI) E. Witt, Theorie der quadratischen Formen in beliebigen Körpern, J. de Crelle, t. CLXXVI (1937), p. 31-44.
(XXXII) E. Cartan, Leçons sur la théorie des spineurs, Actual. Sci. et Industr., n°s 643 et 701, Paris (Hermann), 1938.
(XXXIII) C. L. Siegel, Symplectic Geometry, Amer. Journ. of Math., t. LXV (1943), p. 1-86.
(XXXIV) C. Chevalley, The algebraic theory of spinors, New York (Columbia Univ. Press), 1954.
(XXXV) M. Eichler, Quadratische Formen und orthogonale Gruppen, Berlin-Göttingen-Heidelberg (Springer), 1952.

The reference numbers indicate successively the paragraph and the number (or, exceptionally, the exercise).

$d_\Phi, s_\Phi : 1, 1$ and $6.$
$bJ, bJ' : 1, 2.$
$F^J$ (J antiautomorphism of the ring B of the scalars of the right module F) : 1, 2.
$N^o, M^o$ (N, M submodules) : 1, 3.
$\widehat{\Phi} : 1, 7.$
$u^*$ (u homomorphism) : 1, 8.
$\Phi_{(m)} : 1, 9.$
$M(x), x$ (x element of a free module) : 1, 10.
$M(u)$ (u homomorphism of a free module into a free module) : 1, 10.
$^tM, M^J$ (M matrix) : 1, 10.
$D_\Phi(x_1, \ldots, x_n), D_\Phi(S) : 2.$
$\overline{\alpha}$ ($\alpha$ scalar) : 3.
$\mathrm{Pf}(R) : 5, 2.$
$\mathbf{Sp}(\Phi), \mathbf{Sp}(2m, A), \mathbf{Sp}_{2m}(A) : 5, 3.$
$\mathbf{U}(\Phi), \mathbf{SU}(\Phi)$ ($\Phi$ hermitian form) : 6, 2.
$\mathbf{O}(Q), \mathbf{SO}(Q)$ (Q quadratic form) : 6, 2.
$\mathbf{U}(n, A), \mathbf{SU}(n, A), \mathbf{O}(n, A), \mathbf{SO}(n, A) : 6, 2.$
$Q \perp Q', Q \sim Q'$ (Q, Q’ quadratic forms) : 8, 1.
$\theta(Q)$ (Q quadratic form) : 8, 1.
$T + T', a.T$ (T, T’ types of quadratic forms) : 8, 2.
$\delta(Q)$ (Q quadratic form) : 8, 2.
$Q \otimes Q'$ (Q, Q’ quadratic forms) : 8, 3.
$TT'$ (T, T’ types of quadratic forms) : 8, 3.
$T^h, T^+, T^- : 9, 1.$
$C(Q), I(Q), \rho_Q, \rho, C^+(Q), C^-(Q), C^+, C^-$ (Q quadratic form) : 9, 1.
$\alpha, \beta, C(f) : 9, 1.$
$e_x, i_f, i^F_x, \lambda_F : 9, 2.$
$\overline{\lambda}_F : 9, 3.$
$G, G^+, G^+_0, O^+(Q), O^+_0(Q), N(s)$ (Q quadratic form, s invertible element of the special Clifford group $G^+$) : 9, 5.
$A(\Phi)$ ($\Phi$ symmetric bilinear form on a vector space of dimension 2) : 10, 1.
$S, S^+, H, O^+ : 10, 1.$
$\bar{u}(u$ direct similitude$), i, d : 10, 1.$
$c_w, s_w, t_w, c, s, t : 10, 2.$
$H^+ : 10, 3.$

(D_1, D_2) (D_1, D_2 right lines or half-lines) : 10, 3.
\mathfrak{A}, \mathfrak{A}_0, h, h' : 10, 3.
|x|, \langle x, y \rangle (x, y vectors) : 10, 3.
\cos \theta, \sin \theta, \operatorname{tg} \theta, \operatorname{cotg} \theta : 10, 3.
\{ D_1, D_2 \}, \{ D_1, D_2 \} (D_1, D_2 half-lines in an oriented plane) : 10, 4.

The reference numbers indicate successively the paragraph and the number (or exceptionally, the exercise).

Adjoint (right, left) of a homomorphism : 1, 8.
Adjoint of a semilinear mapping : 7, 3.
Clifford algebra of a quadratic form : 9, 1.
Alternating (matrix) : 3, 1.
Angle of two half-lines : 10, 3, and exerc. 6.
Angle of two half-lines in an affine plane : 10, 3.
Angle of two lines : 10, 3 and exerc. 2.
Angle of two lines in an affine plane : 10, 3.
Angle of two pointed lines : 10, exerc. 2.
Angle of two vectors in a plane : 10, 3.
Angle of two vectors in a space of dimension $\geqslant 2 : 10, 3$.
Right angle : 10, 3 and exerc. 2.
Angle of a rotation : 10, 3.
Angle of a direct similarity : 10, exerc. 6.
Straight angle : 10, 3 and exerc. 6.
Ring of types of quadratic forms : 8, 3.
Witt ring : 8, 3.
Antiautomorphism of a ring : 1, 2.
Principal antiautomorphism of a Clifford algebra : 9, 1.
Antihermitian (form) : 3, 1.
Antihermitian (matrix) : 3, 1.
Antisymmetric (matrix) : 3, 1.
Bilinear mapping : 1, 1.
Degenerate bilinear mapping (right, left) : 1, 1.
Non-degenerate bilinear mapping : 1, 1.
Non-degenerate bilinear mapping associated with a bilinear mapping : 1, 3.
Bilinear mapping obtained by extension of scalars from a bilinear mapping : 1, 4.
Canonical mapping of a module into its Clifford algebra : 9, 1.
Canonical mapping of the set of hermitian endomorphisms onto the set of hermitian forms : 7, 3.
Canonical mapping of the set $\mathfrak{A}$ onto $S^+/H : 10, 3$.
Canonical mapping of the set $\mathfrak{A}$ onto $O^+ : 10, 3$.
Linear mapping associated on the right (left) with a bilinear mapping : 1, 1.
Semilinear mapping associated on the right (left) with a sesquilinear form : 1, 6.

Sesquilinear mapping on the right (left) for an antiautomorphism : 1, 2.
Degenerate sesquilinear mapping (right, left) : 1, 2.
Non-degenerate sesquilinear mapping : 1, 2.
Non-degenerate sesquilinear mapping associated with a sesquilinear mapping : 1, 3.
Sesquilinear mapping obtained by extension of scalars from a sesquilinear mapping : 1, 4.
Associated (linear mapping) with a bilinear mapping : 1, 1.
Associated (semilinear mapping) with a sesquilinear form : 1, 6.
Associated (bilinear form) with a quadratic form : 3, 4.
Orthogonal automorphism : 6, 2.
Orthogonal automorphism with $n$ variables : 6, 2.
Principal automorphism of a Clifford algebra : 9, 1.
Symplectic automorphism : 5, 3.
Symplectic automorphism with $2m$ variables : 5, 3.
Unitary automorphism : 6, 2.
Unitary automorphism with $n$ variables : 6, 2.
Axis of an affine linear complex : 10, exerc. 16.
Orthogonal basis : 6, 1.
Orthonormal basis : 6, 1.
Symplectic basis : 5, 1.
Bilinear (mapping) : 1, 1.
Bilinear (form) : 1, 6.
Bimodule : 1, 1.
Canonical : see Canonical mapping and Canonical homomorphism.
Center of a quadric : 6, exerc. 25 and 10, exerc. 12.
Unit circle : 10, exerc. 2.
Chasles (relation) : 10, 3.
Clifford (algebra) : 9, 1.
Clifford (group) : 9, 5.
Linear complex : 10, exerc. 16.
Condition (C) : 6, 1.
Condition (C') : 6, 1.
Condition (T) : 4, 2.
Isotropic cone : 6, exerc. 23.
Conformal (group) : 10, exerc. 14.
Affine conic : 6, exerc. 25.
Projective conic : 6, exerc. 23.
Conjugate (affine linear varieties) : 6, exerc. 25.
Conjugate (projective linear varieties) : 6, exerc. 23.
Cosine of an angle : 10, 3.
Cotangent of an angle : 10, 3.
Witt decomposition : 4, 2.
Degenerate (bilinear mapping) on the right (left) : 1, 1.
Degenerate (sesquilinear mapping) on the right (left) : 1, 2.
Degenerate (affine conic) : 6, exerc. 25.
Degenerate (projective conic) : 6, exerc. 23.
Degenerate (affine quadric) : 6, exerc. 25.
Degenerate (projective quadric) : 6, exerc. 23.
Half-line : 10, 3.
Closed half-line : 10, 3.
Isotropic half-line : 10, 3.
Open half-line : 10, 3.
Displacement : 6, 6.
Dimension of a quadratic form : 8, 1.
Direct (similarity) : 6, 5.
Discriminant of a sesquilinear form with respect to a system of elements : 2.
Distance : 7, 1.
Right (angle) : 10, 3.
Pointed line : 10, exerc. 2.

Odd element of a Clifford algebra: 9, 1.
Isotropic element: 4, 1.
Even element of a Clifford algebra: 9, 1.
Singular element: 4, 1.
Elements orthogonal with respect to a sesquilinear mapping: 1, 3.
Elements orthogonal with respect to a quadratic form: 3, 4.
Hermitian endomorphism: 7, 3.
Normal endomorphism: 7, 3.
ε-hermitian (form): 3, 1.
ε-hermitian (matrix): 3, 1.
Equivalent (quadratic forms): 3, 4.
Equivalent (sesquilinear forms): 1, 6.
Space of definition of a quadratic form: 8, 1.
Euclidean space: 6, 6.
Hermitian space: 6, 6.
Oriented space: 10, 3.
Euclidean (space): 6, 6.
Extension of a sesquilinear form to a tensor power: 1, 9.
Extension of a sesquilinear form to an exterior power: 1, 9.
External (direct sum) of quadratic forms: 3, 4.
External (direct sum) of quadratic modules: 3, 4.
Weakly orthogonal (subspaces): 3, exerc. 11.
Closed (angular sector): 10, 4.
Closed (half-line): 10, 3.
Cosine function: 10, 3.
Cotangent function: 10, 3.
Sine function: 10, 3.
Tangent function: 10, 3.
Trigonometric function: 10, 3.
Antihermitian form: 3, 1.
Bilinear form: 1, 6.
Bilinear form associated with a quadratic form: 3, 4.
Hermitian bilinear form: 3, 1.
Hermitian form: 3, 1.
Negative (positive) hermitian form: 7, 1.
Inverse form of a bilinear (sesquilinear) form: 1 ; 7.
Metric form: 6, 6.
Neutral form: 4, 2 and 8, 1.
Quadratic form: 3, 4.
Negative (positive) quadratic form: 7, 1.
Non-degenerate quadratic form: 3, 4.
Quadratic form obtained by extension of scalars from a quadratic form: 3, 4.
Sesquilinear form: 1, 6.
Equivalent quadratic forms: 3, 4.
Equivalent sesquilinear forms: 1, 6.
Gram-Schmidt orthogonalization process: 6, 1.
Clifford group: 9, 5.
Reduced Clifford group: 9, 5.
Special Clifford group: 9, 5.
Group of rotations: 9, 5.
Group of types of quadratic forms: 8, 2.
Witt group: 8, 2.
Orthogonal group associated with Q: 6, 2.
Orthogonal group in n variables: 6, 2.
Special orthogonal group: 6, 2.
Special unitary group: 6, 2.
Symplectic group associated with Φ: 5, 3.
Symplectic group in 2m variables: 5, 3.
Unitary group associated with Φ: 6, 2.

Unitary group in $n$ variables: 6, 2.
Hermitian (endomorphism): 7, 3.
Hermitian (space): 6, 6.
Hermitian (form): 3, 1.
Hermitian (matrix): 3, 1.
Canonical homomorphism of the Clifford algebra of a submodule of E into the Clifford algebra of E: 9, 1.
Metric homomorphism: 4, 3.
Radical hyperplane of two spheres: 10, exerc. 12.
Inverse image of a bilinear mapping: 1, 1.
Inverse image of a sesquilinear mapping: 1, 2.
Odd (element) in a Clifford algebra: 9, 1.
Index of a quadratic (sesquilinear) form: 4, 2.
Dickson invariant: 9, exerc. 9.
Inverse (form): 1, 7.
Inverse (similarity): 6, 5.
Inversion: 10, exerc. 13.
Inversion in sphere C: 10, exerc. 13.
Involution in a linear group: 6, 3.
Isotropic (half-line): 10, 3.
Isotropic (element): 4, 1.
Isotropic (submodule): 4, 1.
Isotropic (linear manifold): 6, 6.
Laguerre (formula of): 10, exerc. 5.
Law of inertia: 7, 2.
Length of a vector: 10, 3.
Alternating matrix: 3, 1.
Antihermitian matrix: 3, 1.
Antisymmetric matrix: 3, 1.
Matrix of a mapping satisfying (G), (D), (GD) or (DG): 1, 10.
Matrix of a bilinear mapping: 1, 1.
Matrix of a sesquilinear mapping: 1, 2.
ε-hermitian matrix: 3, 1.
Hermitian matrix: 3, 1.
Normal matrix: 7, exerc. 17.
Orthogonal matrix: 6, 2.
Symmetric matrix: 3, 1.
Symplectic matrix: 5, 3.
Unitary matrix: 6, 2.
Metric (form): 6, 6.
Metric (homomorphism): 4, 3.
Quadratic module: 3, 4.
Multiplier of a similarity: 6, 5 and 6.
Negative ($n$-vector): 10, 3.
Negative (hermitian form): 7, 1.
Negative (quadratic form): 7, 1.
Neutral (quadratic form): 8, 1.
Neutral (sesquilinear form): 4, 2.
Non-degenerate (bilinear mapping): 1, 1.
Non-degenerate (sesquilinear mapping): 1, 2.
Non-degenerate (quadratic form): 3, 4.
Normal (endomorphism): 7, 3.
Spinorial norm: 9, 5.
Kernel of a quadratic module: 3, 4.
Negative (positive) $n$-vector: 10, 3.
Orientation of a space: 10, 3.
Oriented (space): 10, 3.
Orthogonal (automorphism): 6, 2.
Orthogonal (group): 6, 2.
Orthogonal (special group): 6, 2.

Orthogonal (projector): 6, 3.
Orthogonal (submodule) to a submodule: 1, 3.
Orthogonal (vector) to a linear variety: 6, 6.
Orthogonal (basis): 6, 1.
Orthogonal (matrix): 6, 2.
Orthogonal (projection) onto a linear variety: 6, 6.
Orthogonal (transform): 6, 2.
Orthogonal (variety) to a linear variety: 6, 6.
Orthogonal (parts): 1, 3 and 3, 4.
Orthogonal (linear varieties): 6, 6.
Orthogonalization (Gram-Schmidt process): 6, 1.
Orthogonal (elements): 1, 3 and 3, 4.
Orthonormal (basis): 6, 1.
Open (angular sector): 10, 4.
Open (half-line): 10, 3.
Pair (element) in a Clifford algebra: 9, 1.
Orthogonal parts: 1, 3 and 3, 4.
Perpendicular (linear varieties): 6, exerc. 22.
Pfaffian of an alternating matrix: 5, 2.
Flat (angle): 10, 3.
Point of view of a stereographic projection: 10, exerc. 14.
Polar of a linear variety with respect to a quadric: 6, exerc. 23 and 25.
Pole of a hyperplane with respect to a quadric: 6, exerc. 23 and 25.
Pole of an inversion: 10, exerc. 13.
Positive (n-vector): 10, 3.
Positive (hermitian form): 7, 1.
Positive (quadratic form): 7, 1.
Principal (antiautomorphism): 9, 1.
Principal (automorphism): 9, 1.
Tensor product of quadratic forms: 8, 3.
Tensor product of sesquilinear forms: 1, 9.
Orthogonal projector: 6, 3.
Orthogonal projection onto a linear variety: 6, 6.
Stereographic projection: 10, exerc. 14.
Pseudo-discriminant: 9, exerc. 9.
Power of a point with respect to a sphere: 10, exerc. 12.
Power of an inversion: 10, exerc. 13.
Pythagorean theorem: 6, 6.
Quadratic (form): 3, 4.
Quadratic (module): 3, 4.
Affine quadric: 6, exerc. 25.
Projective quadric: 6, exerc. 23.
Rank of a bilinear (sesquilinear) form: 1, 6.
Radius of a sphere: 10, exerc. 12.
Reduced (Clifford group): 9, 5.
Chasles relation: 10, 3.
Spinor representations: 9, 4.
Rotation: 9, 5.
Rotation of angle φ: 10, 3 and exerc. 2.
Rotation (group of): 9, 5.
Closed angular sector: 10, 4.
Open angular sector: 10, 4.
Flat angular sector: 10, exerc. 8.
Reentrant angular sector: 10, exerc. 8.
Convex angular sector: 10, exerc. 8.
Semispinor: 9, 4.
Sesquilinear (mapping): 1, 2.
Sesquilinear (form): 1, 6.
Signature of a hermitian form: 7, 2.
Similarity: 6, 5 and 6.

Direct similarity: 6, 5 and 9, exerc. 9.
Inverse similarity: 6, 5.
Singular (element): 4, 1.
Singular (submodule): 4, 1.
Sine of an angle: 10, 3.
Direct sum of bilinear (sesquilinear) mappings: 1, 3.
External direct sum of quadratic forms (quadratic modules): 3, 4.
Isotropic submodule: 4, 1.
Orthogonal submodule to a submodule: 1, 3.
Singular submodule: 4, 1.
Totally isotropic submodule: 4, 1.
Totally singular submodule: 4, 1.
Sphere: 10, exerc. 12.
Orthogonal spheres: 10, exerc. 12.
Spinor: 9, 4.
Direct sequence of half-lines: 10, 4.
Symmetry with respect to a hyperplane: 6, 4.
Symmetry with respect to a vector subspace: 6, 3.
Symmetry with respect to an affine linear variety: 6, 6.
Symmetric (matrix): 3, 1.
Symplectic (automorphism): 5, 3.
Symplectic (basis): 5, 1.
Symplectic (group): 5, 3.
Symplectic (matrix): 5, 3.
Symplectic (transform): 5, 3.
Tangent of an angle: 10, 3.
Tangent (linear variety) to a quadric: 6, exerc. 23 and 25.
Pythagorean theorem: 6, 6.
Witt theorem: 4, 3.
Totally isotropic (submodule): 4, 1.
Totally orthogonal (submodule) to a submodule: 1, 3.
Totally orthogonal (variety) to a linear variety: 6, 6.
Totally singular (submodule): 4, 1.
Orthogonal transform: 6, 2.
Symplectic transform: 5, 3.
Unitary transform: 6, 2.
Trigonometric (function): 10, 3.
Type of a quadratic form: 8, 1.
Unitary (automorphism): 6, 2.
Unitary (group): 6, 2.
Unitary (special group): 6, 2.
Unitary (matrix): 6, 2.
Unitary (transform): 6, 2.
Isotropic linear variety: 6, 6.
Linear variety orthogonal to a linear variety: 6, 6.
Totally isotropic linear variety: 6, 6.
Orthogonal linear varieties: 6, 6.
Vector orthogonal to a linear variety: 6, 6.
Witt (ring): 8, 3.
Witt (decomposition): 4, 2.
Witt (group): 8, 2.
Witt (theorem): 4, 3.

CHAPTER IX. — Sesquilinear Forms and Quadratic Forms ............ 3
§ 1. Sesquilinear Forms ............................................. 7
    1. Bilinear Mappings ........................................ 7
    2. Sesquilinear Mappings .................................. 10
    3. Orthogonality. Direct Sums of Bilinear or Sesquilinear Mappings .................................................. 12
    4. Change of Base Rings .................................. 13
    5. Some Identities .................................................. 18
    6. Bilinear and Sesquilinear Forms. Rank .................. 18
    7. Inverse Form of a Bilinear or Sesquilinear Form .......... 23
    8. Adjoint of a Homomorphism .................................... 25
    9. Tensor Products and Exterior Powers of Sesquilinear Forms ......................................................... 27
   10. Matrix Calculations .................................................. 32
§ 2. Discriminant of a Sesquilinear Form .......................... 41
§ 3. Hermitian and Quadratic Forms ....................... 49
    1. Hermitian and ε-Hermitian Forms .......................... 49
    2. Modules over a Quadratic Extension .......................... 51
    3. Bilinear Forms Associated with a Hermitian Form .......... 52
    4. Quadratic Forms ............................................... 54
§ 4. Totally Isotropic Subspaces. Witt's Theorem ............... 63
    1. Isotropic Subspaces ........................................... 64
    2. Witt Decomposition ............................................. 65
    3. Witt's Theorem .................................................. 71
§ 5. Properties Special to Alternating Bilinear Forms ............... 79
    1. Reduction of Alternating Bilinear Forms ..................... 79
    2. Pfaffian of an Alternating Matrix .................................. 82
    3. Symplectic Group ................................................ 84
§ 6. Properties Special to Hermitian Forms ......................... 90
    1. Orthogonal Bases ................................................ 90
    2. Unitary Group and Orthogonal Group ............................ 93
    3. Orthogonal Projectors and Involutions .......................... 95
    4. Symmetries in the Orthogonal Group ............................. 97
    5. Group of Similarities ............................................ 98
    6. Hermitian Geometry ............................................. 100
§ 7. Hermitian Forms and Ordered Fields ............................... 114
    1. Positive Hermitian Forms ................................... 115
    2. The Law of Inertia .................................................. 117
    3. Reduction of a Form with Respect to a Positive Hermitian Form ............................................................. 118

§ 8. Types of Quadratic Forms ............................................. 132
    1. Types of Quadratic Forms ............................................. 132
    2. Group of the Types of Quadratic Forms ................................. 134
    3. Ring of the Types of Quadratic Forms ................................. 137
§ 9. Clifford Algebras ....................................................... 139
    1. Definition and Universal Property of the Clifford Algebra ............ 139
    2. Some Operations in the Tensor Algebra .......................... 141
    3. Basis of the Clifford Algebra ............................................. 143
    4. Structure of the Clifford Algebra ........................................ 146
    5. Clifford Group ....................................................... 150
§ 10. Angles ............................................................................. 160
    1. Direct Similarities in a Plane .......................................... 160
    2. Plane Trigonometry ....................................................... 164
    3. Angles ............................................................................. 167
    4. Angular Sectors ....................................................... 173
Historical Note ............................................................................. 185
Index of Notations ....................................................................... 202
Terminological Index ...................................................................... 204
Definitions of Chapter IX ......................................................... Foldout

Sesquilinear forms:
Let A be a ring, $\xi \to \bar{\xi}$ an involutory antiautomorphism of A, that is, a bijection of A onto itself such that $(\xi + \eta) = \bar{\xi} + \bar{\eta}$, $(\xi \eta) = \bar{\eta} \cdot \bar{\xi}$, $\bar{\xi} = \xi$ for all $\xi, \eta$ in A. A sesquilinear form $\Phi$ on a left A-module E is a mapping of $E \times E$ into A such that
$$
\begin{align*}
\Phi(x + x', y) &= \Phi(x, y) + \Phi(x', y), & \Phi(x, y + y') &= \Phi(x, y) + (x, \Phi y') \\
\Phi(\alpha x, y) &= \alpha \Phi(x, y), & \Phi(x, \alpha y) &= \Phi(x, y) \bar{\alpha}
\end{align*}
$$
for all $\alpha \in A, x, x', y, y'$ in E.
Let $\varepsilon$ be an element of the center of A. A sesquilinear form $\Phi$ on E is said to be $\varepsilon$-hermitian if $\Phi(y, x) = \varepsilon \overline{\Phi(x, y)}$ for all $x \in E, y \in E$; if $\varepsilon = 1$ (resp. $\varepsilon = -1$), $\Phi$ is said to be hermitian (resp. anti-hermitian).
When the antiautomorphism $\xi \to \bar{\xi}$ is the identity (which implies that the ring A is commutative), the corresponding sesquilinear forms are bilinear forms. One then says "symmetric" instead of "hermitian", and "antisymmetric" instead of "anti-hermitian" (cf. Chapter III). A bilinear form $\Phi$ such that $\Phi(x, x) = 0$ is said to be alternating; it is then antisymmetric, and the converse is true when A is a field of characteristic $\neq 2$ (cf. Chapter III).
An $\varepsilon$-hermitian form is said to satisfy condition (T) if for every $x \in E$, there exists $\lambda \in A$ such that $\Phi(x, x) = \lambda + \varepsilon \bar{\lambda}$. This condition is always satisfied when $\varepsilon = 1$ and A is a field of characteristic $\neq 2$, or when $\Phi$ is alternating.

Quadratic forms:
Let A be a commutative ring. A quadratic form Q on an A-module E is a mapping of E into A such that $Q(\alpha x) = \alpha^2 Q(x)$ for $\alpha \in A, x \in E$, and such that the mapping
$$
(x, y) \to \Phi(x, y) := Q(x + y) - Q(x) - Q(y)
$$
is a bilinear form (necessarily symmetric), said to be associated with the quadratic form Q. One has $\Phi(x, x) = 2Q(x)$; conversely, for every bilinear form $\Psi$ on E, $x \to \Psi(x, x)$ is a quadratic form on E ;

when $A$ is a field of characteristic $\neq 2$, quadratic forms and symmetric bilinear forms on $E$ thus correspond bijectively.

Orthogonal elements:
Let $\Phi$ be an $\varepsilon$-Hermitian form on a left $A$-module $E$. Two elements $x, y$ of $E$ are said to be *orthogonal* (for $\Phi$) if $\Phi(x, y) = 0$; this relation is symmetric in $x$ and $y$. For every submodule $M$ of $E$, the set of $x \in E$ which are orthogonal to all elements of $M$ is a submodule denoted by $M^0$ and called the *orthogonal* of the submodule $M$. One says that $\Phi$ is *non-degenerate* if $E^0 = \{0\}$. When $E$ is a finite-dimensional vector space and $\Phi$ is non-degenerate, one has $\operatorname{codim} M^0 = \dim M$ and $M^{00} = M$ for every subspace $M$ of $E$; moreover, for every pair of subspaces $M, N$ of $E$, one has
$$
(M + N)^0 = M^0 \cap N^0, \qquad (M \cap N)^0 = M^0 + N^0.
$$
Suppose that the ring $A$ is commutative, and let $Q$ be a quadratic form on the $A$-module $E$, $\Phi$ the bilinear form associated with $Q$. Two elements of $E$ are said to be *orthogonal* (for $Q$) if they are orthogonal for $\Phi$; the *orthogonal* of a submodule $M$ (for $Q$) is the orthogonal $M^0$ of $M$ for $\Phi$. One says that $Q$ is *non-degenerate* if $\Phi$ is non-degenerate.

Isotropic elements and singular elements:
Let $\Phi$ be an $\varepsilon$-hermitian form on a left $A$-module $E$. An element $x \in E$ is said to be *isotropic* if $\Phi(x, x) = 0$; a submodule $M$ of $E$ is said to be *isotropic* if $M \cap M^0 \neq \{0\}$ (in other words if the restriction of $\Phi$ to $M$ is degenerate); $M$ is said to be *totally isotropic* if $M \subset M^0$ (in other words if the restriction of $\Phi$ to $M$ is zero). For every submodule $M$ of $E$, $M \cap M^0$ is totally isotropic. If $E$ is a finite-dimensional vector space and if $\Phi$ is non-degenerate, the following three conditions are equivalent for a subspace $M$ of $E$: $1^\circ$ $M$ is non-isotropic; $2^\circ$ $M^0$ is non-isotropic; $3^\circ$ $E$ is the direct sum of $M$ and $M^0$.
Suppose the ring $A$ commutative, and let $Q$ be a quadratic form on an $A$-module $E$, $\Phi$ the bilinear form associated with $Q$. An element $x \in E$ is said to be *singular* if $Q(x) = 0$; a submodule $M$ of $E$ is said to be *singular* (resp. *totally singular*) if $M \cap M^0$ contains a singular element $\neq 0$ (resp. if the restriction of $Q$ to $M$ is zero). Every singular element (resp. singular submodule, totally singular submodule) is isotropic (resp. isotropic, totally isotropic); the converse is true when $A$ is a field of characteristic $\neq 2$.
