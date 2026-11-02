---
book: alg
book_title: Algebra
chapter: III
chapter_title: TENSOR ALGEBRAS, EXTERIOR ALGEBRAS, SYMMETRIC ALGEBRAS
section: 4
section_title: Tensor products of algebras
lang: ja
source: alg-i-iii
source_edition: 1998, Springer
book_pages: 460-484, 626-627
pdf_pages: 0484-0508, 0650-0651
extraction: ocr
subsections:
    - "no": 1
      title: TENSOR PRODUCT OF A FINITE FAMILY OF ALGEBRAS
      page: 460
      pdf_page: 484
    - "no": 2
      title: UNIVERSAL CHARACTERIZATION OF TENSOR PRODUCTS OF ALGEBRAS
      page: 463
      pdf_page: 487
    - "no": 3
      title: MODULES AND MULTIMODULES OVER TENSOR PRODUCTS OF ALGEBRAS
      page: 465
      pdf_page: 489
    - "no": 4
      title: TENSOR PRODUCT OF ALGEBRAS OVER A FIELD
      page: 468
      pdf_page: 492
    - "no": 5
      title: TENSOR PRODUCT OF AN INFINITE FAMILY OF ALGEBRAS
      page: 470
      pdf_page: 494
    - "no": 6
      title: COMMUTATION LEMMAS
      page: 472
      pdf_page: 496
    - "no": 7
      title: TENSOR PRODUCT OF GRADED ALGEBRAS RELATIVE TO COMMUTATION FACTORS
      page: 474
      pdf_page: 498
    - "no": 8
      title: TENSOR PRODUCT OF GRADED ALGEBRAS OF THE SAME TYPES
      page: 480
      pdf_page: 504
    - "no": 9
      title: ANTICOMMUTATIVE ALGEBRAS AND ALTERNATING ALGEBRAS
      page: 482
      pdf_page: 506
statements: 43
exercises: 2
content_sha256: bf86cdc7d6cc4a67ae497db9036ea05a7525493b3db0ecc2c1e022b136e3bf37
translated_from: content/en/alg/III/04_s4_tensor_products_of_algebras.md
translation_method: google
source_content_sha256: 25682b65ee25b300876c8d2b79b960cdd7e6d7279edee98e796e41613580d0ee
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-eeeca2ef
glossary_version: 34
glossary_terms_sha256: 7ee0dcf515b1d0589654e7aa1644b0ec1ccee50d80c2c0b81363879c9da8e294
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## § 4。 テンソル積/代数

§ 4 から § 8 まで、A は可換環を表し、〜でない限りは、特に言及されていない限り、考慮される代数は結合的かつ単体であると想定され、代数準同型は単体であると想定されます。

### 1. 代数の有限家族のテンソル積

A は常に可換環を単位元で表します。 (E_i)_{i \in I} を A-代数の有限族とし、E = \bigotimes_{i \in I} E_i を A-加群 E_i (II, § 3, no. 9) のテンソル積 A-加群とします。 E で定義する A-代数構造とします。m_i: E_i \otimes_A E_i \to E_i を、E_i (§ 1, no. 3) で乗法を定義する A-線型写像とします。 A-線型写像を検討してください

$$
m' = \bigotimes_{i \in I} m_i: \bigotimes_{i \in I} (E_i \otimes_A E_i) \to \bigotimes_{i \in I} E_i = E;
$$

合成写像

$$
\left( \bigotimes_{i \in I} E_i \right) \otimes_A \left( \bigotimes_{i \in I} E_i \right) \xrightarrow{\tau} \bigotimes_{i \in I} (E_i \otimes_A E_i) \xrightarrow{m'} \bigotimes_{i \in I} E_i
$$

ここで、$\tau$ は結合性同型 (II, § 3, no. 9) は A-線型写像 $m : E \otimes_A E \to E$ です。 $m$ 定義するが $E$ で (結合的かつ単体) 代数構造であることがわかります。なぜなら、$m$ によって定義された乗法を明示的に実行すると、公式が得られます。

(1)
$$
\left( \bigotimes_{i \in I} x_i \right) \left( \bigotimes_{i \in I} y_i \right) = \bigotimes_{i \in I} (x_i y_i) \quad \text{for } x_i, y_i \text{ in } E_i \text{ and } i \in I.
$$

したがって、線形性により、$e_i$ が $E_i$ の単位元である場合、$e = \bigotimes_{i \in I} e_i$ は $E$ の単位元であることがすでにわかります。一方、それぞれの $E_i$ の結合性は関係を意味します。

$$
\left( \left( \bigotimes_{i \in I} x_i \right) \left( \bigotimes_{i \in I} y_i \right) \right) \left( \bigotimes_{i \in I} z_i \right) = \bigotimes_{i \in I} (x_i y_i z_i) = \left( \bigotimes_{i \in I} x_i \right) \left( \left( \bigotimes_{i \in I} y_i \right) \left( \bigotimes_{i \in I} z_i \right) \right)
$$

よって、線形性により、$E$ のすべての $x, y, z$ に対して関係 $x(yz) = (xy)z$。

#### 定義 1 {#alg-iii-s4-def-1 .statement tag=0608}

*家族* $(E_i)_{i \in I}$ *代数以上* $A$、この家族の *テンソル積を $\bigotimes_{i \in I} E_i$ で表します (または、$I$ が $\mathbf{N}$ の区間 $\{1, n\}$ の場合、 $E_1 \otimes_A E_2 \otimes \cdots \otimes_A E_n$、または単に $E_1 \otimes E_2 \otimes \cdots \otimes E_n$) * は、* (1) で定義された * $A$* モジュール* $E_i$ *乗法のテンソル積を与えることによって得られる代数です。

関係 (1) は、$E_i$ の*反対* 代数のテンソル積 $\bigotimes_{i \in I} E_i^0$ が反対多元環から $\bigotimes_{i \in I} E_i$ であることを示しています。特に、$E_i$ が *可換* である場合、$\bigotimes_{i \in I} E_i$ も同様です。

$(E_i)_{i \in I}$ と $(F_i)_{i \in I}$ を、同じ有限指数付け集合 $I$ を持つ 2 つの $A$-代数の族とする。それぞれの $i \in I$ に対して、$f_i : E_i \to F_i$ を $A$-代数準同型性とします。次に、$A$-線形マッピング

$$
f = \bigotimes_{i \in I} f_i : \bigotimes_{i \in I} E_i \to \bigotimes_{i \in I} F_i
$$

(1) より、 *A-代数準同型* です。

$I$ の各分割 $(I_j)_{j \in J}$ に対して、結合性同型

$$
\bigotimes_{j \in J} \left( \bigotimes_{i \in I_j} E_i \right) \to \bigotimes_{i \in I} E_i
$$

(1) とその定義からわかるように、(II, § 3, no. 9) も *代数* 同型です。

$I$ が $\mathbf{N}$ の区間 $[1, n]$ で、すべての代数 $E_i$ が同じ代数 $E$ であるとき、テンソル積代数 $\bigotimes_{i \in I} E_i$ も同様です$E^{\otimes n}$で示されます。

この番号の残りの部分については注意を限定します。 2 つの代数のテンソル積の特性に拡張し、それらを任意の有限族のテンソル積に拡張するというタスクは読者に委ねられます。

$E, F$ を 2 つの $A$-代数とする。 $a$ (それぞれ $b$) が $E$ (それぞれ $F$) の左イデアルである場合、$E \otimes_A F$ の $a \otimes_A b$ の標準像 $\operatorname{Im}(a \otimes b)$ は $E \otimes_A F$ の左イデアルです。 「左の理想」を「右の理想」または「両側の理想」に置き換えると、同様の結果が得られます。さらに：

#### 命題 1 {#alg-iii-s4-prop-1 .statement tag=0609}

*$E, F$ を 2 つの $A$-代数、および $a$ (それぞれ $b$) を $E$ (それぞれ $F$) の両側イデアルとします。次に、正規の $A$ モジュール同型*

$$
(E/a) \otimes (E/b) \to (E \otimes F)/(\operatorname{Im}(a \otimes F) + \operatorname{Im}(E \otimes b))
$$

(II, § 3, no. 6、系 1 ～ 命題 6) *は代数同型* です。

これは (1) と *loc が与えられた定義から導き出されます。引用*。

#### 系 1 {#alg-iii-s4-prop-1-cor-1 .statement tag=060A}

*$E$を$A$-代数、$a$を$A$のイデアルとする。この場合、$A$ モジュール $aE$ は、$E$ と標準的な $(A/a)$ モジュール同型* の両側理想です。

$$
(A/a) \otimes_A E \to E/aE
$$

*は* $(A/a)$*-代数同型*です。

#### 系 2 {#alg-iii-s4-prop-1-cor-2 .statement tag=060B}

*$a, b$ が $A$ の 2 つのイデアルである場合、$(A/a) \otimes_A (A/b)$ は$A/(a + b)$* と正準的に同型です。

#### 系 3 {#alg-iii-s4-prop-1-cor-3 .statement tag=060C}

*$E, F$ を 2 つの $A$-代数と、$F$ の消滅子に含まれる $A$ のイデアルを $a$ とします。この場合、$(A/a)$-代数 $E \otimes_A F$ は正準的に $(E/aE) \otimes_{A/a} F$* と同型です。

#### 命題 2 {#alg-iii-s4-prop-2 .statement tag=060D}

*Let $(E_\lambda)_{\lambda \in L}$ and $(F_\mu)_{\mu \in M}$ be two families of $A$-algebras. 標準写像* (II, § 3, no. 7)

$$
\left( \bigoplus_{\lambda \in L} E_\lambda \right) \otimes_A \left( \bigoplus_{\mu \in M} F_\mu \right) \to \bigoplus_{(\lambda, \mu) \in L \times M} (E_\lambda \otimes_A F_\mu)
$$

*は代数同型*です。

これは、$E \otimes F$ の乗法の II, § 3, no. 7、命題 7、定義の直後に続きます。

#### 命題 3 {#alg-iii-s4-prop-3 .statement tag=060E}

*$A, B$ を 2 つの可換環、$\varphi : A \to B$ 環準同型、および $E, F$ 2 つの $A$-代数とします。次に、正規の $B$ モジュール同型*

$$
\varphi^*(E) \otimes_B \varphi^*(F) \to \varphi^*(E \otimes_A F)
$$

(II, § 5, no. 1, 命題 3) *は $B$-代数同型*です。

#### 命題 4 {#alg-iii-s4-prop-4 .statement tag=060F}

$A, B$ を 2 つの可換環、$\rho : A \to B$ 環準同型、$E$ を $A$-代数、$F$ を $B$-代数とする。次に、正規の $A$ モジュール同型

$$
\rho_*(F) \otimes_A E \to \rho_*(F \otimes_B \rho^*(E))
$$

(II, § 5, no. 2, 命題 6) は $A$-代数同型写像です。

§ 1, no. 5 を考慮すると、検証は簡単です。

In particular, the $A$-algebra structure on $B \otimes_A E$, obtained by restricting the ring $B$ of scalars to $A$, is identical with the structure of the algebra $B \otimes_A E$, the tensor product of the $A$-algebras $B$ and $E$.

最後に、$(A_i, \phi_{ji})$ が可換環、$(E_i, f_{ji})$、$(F_i, g_{ji})$ の直接系、$A_i$-代数 ($§ 1$、no. 6) と $A = \lim \rightarrow A_i$ の 2 つの直接系である場合、標準的な $A$ 加群同型

$$
\lim \rightarrow (E_i \otimes_{A_i} F_i) \to (\lim \rightarrow E_i) \otimes_A (\lim \rightarrow F_i)
$$

(II, § 6, no. 3, 命題 7) も、定義からわかるように、$A$-代数同型写像です。

例/テンソル積/代数。 (1) $A$ を可換環 、$M, N$ を 2 つの $A$ モジュールとします。 標準写像

$$
\text{End}_A(M) \otimes_A \text{End}_A(N) \to \text{End}_A(M \otimes_A N)
$$

(II, § 4, no. 4) は、II, § 3, no. 2, 公式 (5) からわかるように、$A$-代数準同型写像です。 $M$ または $N$ が有限生成射影 $A$ 加群である場合、この準同型は全単射 (II, § 4, no. 4, 命題 4) であることがわかります。特に、2 つの正方行列のうちテンソル積の定義を回収します。

(2) $S, T$ を 2 つのモノイドとし、環 $A$ (III, § 2, no. 6) 上のモノイド $S$ と $T$ の $A^{(S)}$ と $A^{(T)}$ 代数とします。その場合、標準的な$A$-代数同型写像が存在します。

$$
A^{(S)} \otimes_A A^{(T)} \to A^{(S \times T)}.
$$

元 $e_s \otimes e_t$ (それぞれ $e_{(s,t)}$)、ここで、$s$ は $S$ を通過し、$t$ は II, § 3, no. 7 のおかげで、$A^{(S)} \otimes_A A^{(T)}$ の $T$、形基底を通過します。 系 2 ～ 命題 7 (それぞれ $A^{(S \times T)}$ ; 目的の同型は写像 $e_s \otimes e_t$ から $e_{(s,t)}$ によって得られ、定義からこれは確かに代数同型であることがわかります。

### 2. ユニバーサル特徴付けのテンソル積の代数

#### 命題 5 {#alg-iii-s4-prop-5 .statement tag=060G}

$(E_i)_{i \in I}$ を $A$-代数の有限族とし、それぞれの $i \in I$ について、$e_i$ を $E_i$ の単位元とします。それぞれの $i \in I$ について、$u_i : E_i \to E = \bigotimes_{i \in I} E_i$ を次のように定義される $A$ 線形マッピングとします。

$$
u_i(x_i) = \bigotimes_j x'_j \quad \text{with } x'_i = x_i \text{ and } x'_j = e_j \text{ for } j \neq i.
$$

(i) *$u_i$ は $\mathbf{A}$-代数同型写像です。さらに、$i \neq j$、元、$u_i(x_i)$、$u_j(x_j)$ は、$x_i \in \mathbf{E}_i$ と $x_j \in \mathbf{E}_j$ のすべてに対して $\mathbf{E}$ で置換可能であり、$\mathbf{E}$ は部分代数 $u_i(\mathbf{E}_i)$ の和集合によって生成されます。

(ii) *Let $\mathbf{F}$ be an $\mathbf{A}$-algebra and, for all $i \in \mathbf{I}$, let $v_i : \mathbf{E}_i \to \mathbf{F}$ be an $\mathbf{A}$-algebra homomorphism, where the $v_i$ are such that, for $i \neq j$, $v_i(x_i)$ and $v_j(x_j)$ are permutable in $\mathbf{F}$ for all $x_i \in \mathbf{E}_i$ and $x_j \in \mathbf{E}_j$. すると、次のような $\mathbf{A}$-代数準同型性 $w : \mathbf{E} \to \mathbf{F}$ が 1 つだけ存在します*

$$
v_i = w \circ u_i \quad \text{for all } i \in \mathbf{I}.
$$

(i) 写像 $u_i$ は、$\mathbf{E}$ の乗法の定義により代数準同型になります。 $i \neq j$、$x_i \in \mathbf{E}_i, x_j \in \mathbf{E}_j$ の場合、

$$
u_i(x_i) = \bigotimes_k x'_k \quad \text{with } x'_i = x_i, x'_k = e_k \text{ for } k \neq i,
$$
$$
u_j(x_j) = \bigotimes_k x''_k \quad \text{with } x''_j = x_j, x''_k = e_k \text{ for } k \neq j.
$$

明らかに、すべての $k \in \mathbf{I}$ に対して $x'_k x''_k = x''_k x'_k$ であるため、$u_i(x_i)$ と $u_j(x_j)$ は、$\mathbf{E}$ で乗法を定義する公式 (1) (no. 1) によって $\mathbf{E}$ に通います。 最後の主張は関係$\bigotimes_i x_i = \prod_{i \in \mathbf{I}} u_i(x_i)$の後に続きます。

(ii) それぞれの $i \in \mathbf{I}$ について、$x_i$ を $\mathbf{E}_i$ の元とします。 代数 $\mathbf{F}$ は結合的であり、元 $v_i(x_i)$ はペアごとに変更可能であるため、積 $\prod_{i \in \mathbf{I}} v_i(x_i)$ は、$\mathbf{I}$ の順序とは独立して $\mathbf{F}$ で定義されます。 $\prod_{i \in \mathbf{I}} \mathbf{E}_i$ から $\mathbf{F}$ への写像 $(x_i)_{i \in \mathbf{I}} \to \prod_{i \in \mathbf{I}} v_i(x_i)$ は明らかに $\mathbf{A}$ 多線形であり、したがって、次のような $\mathbf{A}$ 線形写像 $w : \mathbf{E} \to \mathbf{F}$ が 1 つだけ存在します。

$$
w\left( \bigotimes_i x_i \right) = \prod_i v_i(x_i).
$$

さて、所望の $\mathbf{A}$-代数準同型性 $w : \mathbf{E} \to \mathbf{F}$ は満たす (5) でなければなりません。これは (4) と $\bigotimes_i x_i = \prod_{i \in \mathbf{I}} u_i(x_i)$ という事実から導き出されます。 これは、$w$ の一意性を証明します。 (5) で定義された $\mathbf{A}$-線形写像 $w$ が $\mathbf{A}$-代数準同型であり、(4) を満たすことを示すことが残っています。 The fact that $w$ satisfies (4) is obvious: it suffices to apply (5) to the case where $x_j = e_j$ for $j \neq i$ and we obtain $w(u_i(x_i)) = v_i(x_i)$. 最後に、$w$ は代数準同型です。

$$
w\left( \left( \bigotimes_i x_i \right) \left( \bigotimes_i y_i \right) \right) = w\left( \bigotimes_i (x_i y_i) \right) = \prod_i v_i(x_i y_i)
$$
$$
= \prod_i (v_i(x_i) v_i(y_i)) = \left( \prod_i v_i(x_i) \right) \cdot \left( \prod_i v_i(y_i) \right)
$$

$v_i(x_i)$ は $j \neq i$ の間 $v_j(y_j)$ と通勤するため。したがって

$$
w w \left( \left( \bigotimes_i x_i \right) \left( \bigotimes_i y_i \right) \right) = w \left( \bigotimes_i x_i \right) . w \left( \bigotimes_i y_i \right)
$$

これは直線性により、証明を完成します。

E の対からなると $\prod_i E_i$ の標準写像 $\phi : (x_i) \mapsto \bigotimes_i x_i$ を E に入れると、ユニバーサル写像問題 (集合理論, IV, § 3, no. 1) の解になります。 $\Sigma$ は A-代数構造の種であり、射は A-代数準同型であり、$\prod_i E_i$ の写像 $\prod_i u_i$ を A-代数に$\alpha$ マッピングします。 $u_i$ は A-代数準同型と $u_i(x_i)$ と $u_j(x_j)$ は $i \neq j$ に通勤し、$x_i \in E_i$ と $x_j \in E_j$ はすべて通勤します。

#### 系 {#alg-iii-s4-n2-cor-1 .statement tag=060H}

*$(E_i)_{i \in I}, (F_i)_{i \in I}$ * を 2 つの有限族である A-代数とし、すべて* $i \in I$ について * $f_i : E_i \to F_i$ * 代数準同型とします。 * $u_i : E_i \to \bigotimes_{j \in I} E_j, v_i : F_i \to \bigotimes_{j \in I} F_j$ * が標準準同型、写像* $f = \bigotimes_i f_i$ *(cf. no. 1)* * は、* $f \circ u_i = v_i \circ f_i$ *すべて* $i \in I$ となるような一意の A-代数準同型です。

準同型 $g_i = v_i \circ f_i$ は、$g_i(x_i) = v_i(f_i(x_i))$ と $g_j(x_j) = v_j(f_j(x_j))$ が $i \neq j$、$x_i \in E_i$、$x_j \in E_j$ に通勤するようなものであることに注意するだけで十分です。次に命題を適用する5。

命題 5 において、代数 F が *可換* であると仮定すると、$v_i(x_i)$ と $v_j(x_j)$ が $i \neq j$ に対して置換可能であるという仮定が自動的に満たされます。したがって、*F が可換である場合*、正規の全単射が存在します。

$$
\text{Hom}_{A\text{-alg.}} \left( \bigotimes_i E_i, F \right) \to \prod_i \text{Hom}_{A\text{-alg.}} (E_i, F),
$$

つまり、$\bigotimes_i E_i$ のすべての準同型 $w$ を $w \circ u_i$ のファミリー F に関連付けるものです。

E が可換 A-代数の場合、$E \otimes_A F$ の環構造は $F_{(E)}$ (§ 1, no. 5) の環構造と同じであることに注意してください。

### 3. 加群およびテンソル積の代数を超えるマルチモジュール

#### 定義 2 {#alg-iii-s4-def-2 .statement tag=060I}

*E を (単位) A-代数とします。左 (右) の E モジュールは、E の基礎となる環の上の左 (右) 加群です。

〜でない限り特に記載がない限り、この番号ではすべての加群およびマルチモジュールが考慮されます。は左加群とマルチモジュールです。

M が E モジュールである場合、準同型 $\eta : A \to E$ (§ 1, no. 4) から、M 上の定義する A-加群構造は、M 上の E モジュール構造の根底にあると言われます。 $\alpha \in A, s \in E, x \in M$ の場合、

$$
\alpha(sx) = s(\alpha x) = (\alpha s)x,
$$

したがって、すべての $s \in E$、ホモテティー $h_s : x \mapsto sx$ の M は、基礎となる A-加群構造の自己準同型になります。逆に、M に E モジュール構造が与えられることは、M に A-加群構造が与えられ、E の A-代数準同型 $s \mapsto h_s$ が $\mathrm{End}_A(M)$ に与えられることと同じです。

#### 定義 3 {#alg-iii-s4-def-3 .statement tag=060J}

*E と F を 2 つ (単位的) A-代数と M 集合とし、E モジュール構造と F モジュール構造とします。次の場合、M は代数 E および F よりも (左) 両側加群と呼ばれます:*

(1) *M は、E と F* (II, § 1, no. 14) の基礎となる環を上回る両側加群です。
(2) *M 上の E モジュールおよび F モジュール構造の基礎となる 2 つの A-加群構造は同一です*。

後者の条件は、e と $e'$ がそれぞれ E と F の単位元である場合、

$$
(\alpha e)x = (\alpha e')x \quad \text{for } \alpha \in A, x \in M;
$$

次に、$\alpha x$ は、両側の共通の値を表すために使用されます。

また、E と F に対して M 両側加群構造が与えられることは、M に A-加群構造が与えられ、さらに E の 2 つの A-代数準同型 $s \mapsto h'_s$ が $\mathrm{End}_A(M)$ に、F の $t \mapsto h''_t$ が $\mathrm{End}_A(M)$ に与えられることと同等であるとも言えます。 $s \in E$ と $t \in F$ はすべて $h'_s h''_t = h''_t h'_s$ です。その結果、(no. 2, 命題 5) $E \otimes_A F$ の $\mathrm{End}_A(M)$ への A-代数準同型 $u \mapsto h_u$ は、$s \in E$ と $t \in F$ に対して $h_{s \otimes t} = h'_s h''_t = h''_t h'_s$ となるように正規に導出されます。他の語では、$(E \otimes_A F)$ モジュール構造が M 上に定義されており、これは E と F を介して指定された両側加群構造に関連付けられていると言われており、その下で

$$
(s \otimes t).x = s(tx) = t(sx) \quad \text{for } s \in E, t \in F \text{ and } x \in M.
$$

M 上の指定された E モジュールおよび F モジュール構造は、スカラーの環の制限、2 つの標準準同型 $E \to E \otimes_A F$ および $F \to E \otimes_A F$ への対応するによって、この $(E \otimes_A F)$ モジュール構造から導出できます。

逆に、標準準同型 $E \to E \otimes_A F$ と $F \to E \otimes_A F$ E モジュール構造と F モジュール構造によって M に $(E \otimes_A F)$ モジュール構造が与えられると、M はこれら 2 つにより代数 E と F に対する *両側加群* となるのは明らかです。 構造、および指定された $(E \otimes_A F)$ モジュール構造がこの両側加群構造に関連付けられていることがわかります。

従って、代数 E および F を介して $(E \otimes_A F)$ モジュールと両側加群の間に 1 対 1 の対応が確立されています。明らかに、M のすべての部分両側加群は、付随した $(E \otimes_A F)$ モジュール構造では部分加群であり、その逆も同様です。 商、積、直和、および逆および直接の極限にも同様の結果があります。最後に、$M'$ が代数 E および F 上の他の両側加群であり、$f : M \to M'$ が両側加群準同型である場合、$f$ は $(E \otimes_A F)$ モジュール準同型であり、その逆も可能です。

右両側加群構造には明らかに対応する主張が存在します。または、たとえば左の E モジュール構造と右の F モジュール構造がある場合、この場合、$(E, F)$ バイモジュールについて話しており、そのような構造が与えられることは、E と $F^o$ の上に左の両側加群構造が与えられることと同じです。

#### 例 {#alg-iii-s4-n3-exa-1 .statement tag=060K}

(1) B を A-代数とします。 環 B は標準的に (B, B) バイモジュール構造 (II, § 1, no. 14, 例 1) を持ち、e が B の単位元である場合、すべての $x \in B$ とすべての $\alpha \in A$ について $(\alpha e)x = x(\alpha e) = \alpha x$ になります。従って、B は、代数 B および $B^o$ (B の反対) 上の左両側加群と考えることができます。従って、B 上の (B, B) バイモジュール構造には (B $\otimes_A B^o$) モジュール構造が関連付けられており、B の $b, x$ と $b'$ については、

$$
(b \otimes b').x = bx b'
$$

右側は環 B の積です。

(2) E と F を 2 つの A-代数、$e, e'$ それぞれの単位元、M を E モジュール、N を F モジュールとします。これらの加群構造定義するは、環 A および E 上の M 両側加群構造と、環 A および F 上の N 両側加群構造です。従って、これらから、環上の両側加群構造 E とテンソル積 $M \otimes_A N$ の F が導出され、次のように定義されます。

$$
x.(m \otimes n) = (x.m) \otimes n, \quad y.(m \otimes n) = m \otimes (y.n)
$$

$x \in E, y \in F, m \in M, n \in N$ (II, § 3, no. 4) の場合。また、条件 (8) が成り立つため、上記の両側加群構造は $M \otimes_A N$ 上の $(E \otimes_A F)$ モジュール構造に関連付けられていることがわかります。

$$
(x \otimes y).(m \otimes n) = (x.m) \otimes (y.n)
$$

$x \in E, y \in F, m \in M, n \in N$の場合。

特に、$M = E_s, E_s \otimes_A N$ を取ると、標準的には $(E \otimes_A F)$ モジュール構造になります。一方、$E \otimes_A N$ は標準的に $E \otimes_A (F_d \otimes_F N) = (E \otimes_A F) \otimes_F N$ と識別され、$E \otimes_A F$ は標準準同型 $v : F \to E \otimes_A F$ によって定義される正しい F モジュール構造を持つとみなされます。したがって、E の $x, x'$、$y \in F, n \in N$、$x' \otimes n$ は $(x' \otimes e') \otimes n$ と同一視され、$(x \otimes y).(x' \otimes n') = (xx') \otimes (y.n)$ は $((xx') \otimes y) \otimes n$ と同一視されます。したがって、$(E \otimes_A F)$ モジュール $E_s \otimes_A N$ は、準同型 $v$ (II, § 5, no. 1) によってスカラーを $E \otimes_A F$ に拡張することにより、N から導出された $(E \otimes_A F)$ モジュールと識別されます。 N の $E_s \otimes_A N$ への標準写像 $n \mapsto e \otimes n$ は、N の $(E \otimes_A F) \otimes_F N$ への標準写像 $n \mapsto (e \otimes e') \otimes n$ と同一視されます。これは F 準同型性として知られています。

同じ記法で、P を右 (E \otimes_A F) 加群としましょう。次に、正規の Z モジュール同型があります。

(11) $$ P \otimes_{E \otimes_A F} (E_s \otimes_A N) \to P \otimes_F N $$

ここで、右側の P は、標準準同型 $v$ によって右 F モジュールと見なされます。なぜなら、P は正規的に $P \otimes_{E \otimes_A F} (E \otimes_A F)$ および $(E \otimes_A F) \otimes_F N$ と $E \otimes_A (F \otimes_F N)$、したがって $E \otimes_A N$ と同一視され、記述された同型 (II, § 3, no. 8、命題 8 および II, § 3, no. 4、命題 4) が確立されます。

上記のすべて拡大するから *multimodules* (II, § 1, no. 14) まで。

### 4. 体を超える代数のうちテンソル積

K を可換 *体* とし、E、F を K 上の 2 つの代数とし、それぞれの単位元 $e, e'$ を *非ゼロ* とします。すると、準同型 $\eta_E : K \to E$ と $\eta_F : K \to F$ (§ 1, no. 3) は単射となり、E (それぞれ F) の部分体で同一視する K が可能になります。 $u(x) = x \otimes e'$ と $v(y) = e \otimes y$ で定義される標準準同型 $u : E \to E \otimes_K F$ と $v : F \to E \otimes_K F$ は *単射* (II, § 7, no. 9, 命題 19) であり、 $E \otimes_K F$ の *部分代数* を使用して同一視する E と F を可能にし、両方とも次のようになります。 単位元単位元 $e \otimes e'$/$E \otimes_K F$。 $E \otimes_K F, E \cap F = K$ (II, § 7, no. 9、命題 19) に。

E' と F' がそれぞれ E と F の部分代数である場合、 標準準同型 $E' \otimes_K F' \to E \otimes_K F$ は単射的であり、$E' \cup F'$ (II, § 7, no. 7, 命題 14) によって生成される $E \otimes_K F$ の部分代数を使用して同一視する $E' \otimes_K F'$ が可能になります。

#### 命題 6 {#alg-iii-s4-prop-6 .statement tag=060L}

*E、Fを、可換体、K、C（それぞれD）、Eの部分代数（それぞれF）、およびEのC（それぞれFのD）のセントラライザーC'（それぞれD'）上の2つの非ゼロ代数とする。この場合、E \otimes_K F 内の C \otimes_K D のセントラライザーは C' \otimes_K D' になります。*

$C \otimes_K D$ ($x_i \in F, y_i \in F$) 属するから $C' \otimes_K D'$ のセントラライザーの元 $z = \sum_i x_i \otimes y_i$ を検証するまでのすべては簡約するです。私たちはそれを知っています

$$
C' \otimes_K D' = (C' \otimes_K F) \cap (E \otimes_K D')
$$

(II, § 7, no. 7、系から命題14)。 $y_i$ は K に対して線形独立であると仮定できます。すべての$x \in C$、必然的に$(x \otimes e')z = z(x \otimes e')$、つまり$\sum_i (xx_i - x_ix) \otimes y_i = 0$、よって $xx_i = x_ix$、すべての$i$ (II, § 3, no. 7、系 1 ～ 命題 7)。したがって、すべての $i$ に対して $x_i \in C'$ が必要となり、したがって $z \in C' \otimes_K F$ になります。同様に、$z \in E \otimes_K D'$、よって命題であることがわかります。

#### 系 {#alg-iii-s4-n4-cor-1 .statement tag=060M}

*Z と Z' が E と F のそれぞれの中心である場合、E \otimes_K F の中心は Z \otimes_K Z'* です。

E と F を可換体 K を超える代数 G の 2 つ部分代数とする。 E のすべての元が F のすべての元と交換するとします。すると、標準単射 $i : E \to G, j : F \to G$ 定義する標準準同型 $h = i \otimes j : E \otimes_K F \to G$ (no. 2, 命題 5) は次のようになります。
$$
(i \otimes j)(x \otimes y) = xy \quad \text{for } x \in E, y \in F.
$$

#### 定義 4 {#alg-iii-s4-def-4 .statement tag=060N}

*可換体 K を超える代数 G が与えられた場合、G の 2 つの部分代数 E、F は、満たす次の条件であれば、K を線形に互いに素超えると言われます:*
(1) *E のすべての元は F のすべての元と交換します。*
(2) *$E \otimes_K F$ の G への標準準同型は単射です。*

#### 命題 7 {#alg-iii-s4-prop-7 .statement tag=060O}

*G を可換体 K と E 上の代数とし、E のすべての元が F のすべての元と可換になるように、F を G の 2 つ部分代数とします。 E と F が K 上で線形互いに素であるためには、G 上の正しい F モジュール構造の G の自由部分集合である K 上に E の基底が存在することが必要かつ十分です。 このような場合:*
(i) *標準準同型 $h : E \otimes_K F \to G$ は、$E \cup F$ によって生成された G の部分代数上の $E \otimes_K F$ の同型です。*
(ii) $E \cap F = K;$
(iii) *K 上の E (それぞれ F) のすべての空き部分集合は、右または左の F モジュール (それぞれ E モジュール) 構造を備えた G の空き部分集合です。*

K 上の E のすべての基底は、正しい F モジュール構造 (II, § 3, no. 7、系 1 ～ 命題 7) を持つ $E \otimes_K F$ の基底であるため、主張の条件は明らかに必要です。 条件が十分であることを確認するには、h の下の $E \otimes_K F$ の像 H が、G の和 $\sum_i x_i y_i = \sum_i y_i x_i$ の集合であり、$x_i \in E$ と $y_i \in F$ があることに注意してください。 $(a_\lambda)$ が K 上の E の基底である場合、H は、$(a_\lambda)$ によって生成された (右または左) F モジュール G の部分加群でもあります。したがって、主張の条件は、FモジュールHの基底でもあるEの基底$(a_\lambda)$が存在することを意味します。 h は単射であるということになります。 主張 (iii) は、E のすべての空き部分集合が E の基底 (II, § 7, no. 1、定理 2) に含まれるという事実から導き出されます。

#### 系 1 {#alg-iii-s4-prop-7-cor-1 .statement tag=060P}

*G への $E \otimes_K F$ の標準準同型が全単射であるためには、(右または左) F 加群 G の基底である K の上に E の基底が存在することが必要かつ十分です。

#### 系 2 {#alg-iii-s4-prop-7-cor-2 .statement tag=060Q}

*E、F を、K 上の有限階数の 2 つの G の部分代数とし、E のすべての元が F のすべての元と交換できるようにします。E と F が K 上で線形に互いに素になるためには、$E \cup F$ によって生成される G の部分代数 H が次のようになることが必要かつ十分です*
$$
[H : K] = [E : K] \cdot [F : K].
$$
これは、全射法標準準同型 h の階数 over K : E \otimes_K F \to H は、E \otimes_K F over K の階数に等しいことを示します。これは、この準同型が全単射 (II, § 7, No. 4, 命題 9) であるというと同等です。

### 5. 代数の無限家族のテンソル積

A を可換環とし、(E_i)_{i \in I} を (単位的) A-代数の任意の族とします。 I のすべての有限部分集合 J について、E_J が代数のテンソル積 $\bigotimes_{i \in J} E_i$ 添字 $i \in J$ の E_i を表すものとします。 $e_i$ は E_i の単位元と E_J の $e_J = \bigotimes_{i \in J} e_i$ 単位元を表すものとします。 $f_{J,i}$ は $i \in J$ (no. 2、命題 5) の標準準同型 $E_i \to E_J$ を表します。 If J, J' are two finite subsets of I such that $J \subset J'$, a homomorphism $f_{J'J} : E_J \to E_{J'}$ is canonically derived (no. 2, Proposition 5), by the condition $f_{J'J} \circ f_{J,i} = f_{J',i}$ for all $i \in J$. さらに、$f_{J'J}$の一意性は、J、J'、J''が$J \subset J' \subset J''$のようなIの3つの有限部分集合であれば、$f_{J''J} = f_{J''J'} \circ f_{J'J}$であることを意味します。 他の語では、$(E_J, f_{J'J})$ は A-代数の直接系であり、そのインデックス付け集合は I の有限部分集合の右側有向集合 $\mathscr{F}(I)$ です。

#### 定義 5 {#alg-iii-s4-def-5 .statement tag=060R}

*直接系* $(E_J, f_{J'J})$ の直接の極限 E は、A-代数* $(E_i)_{i \in I}$ の族のテンソル積と呼ばれます。

I が有限の場合、E は $\bigotimes_{i \in I} E_i$ と同一視されます。 記法を乱用すると、I が無限大であっても、E は $\bigotimes_{i \in I} E_i$ で表されます。

I のすべての有限部分集合 J について、$f_J$ は標準準同型 $\bigotimes_{i \in J} E_i \to \bigotimes_{i \in I} E_i$ を表します ($f_{\{i\}}$ の代わりに $f_i$ と書きます)。 e が $\bigotimes_{i \in I} E_i$ の単位元である場合、すべての $J \in \mathscr{F}(I)$ に対して $f_J(e_J) = e$ になります。すべての代数 E_i が可換である場合、明らかは、$\bigotimes_{i \in I} E_i$ も可換です。

#### 命題 8 {#alg-iii-s4-prop-8 .statement tag=060S}

(i) *準同型* $f_i : E_i \to E = \bigotimes_{k \in I} E_k$ *2 つの添字* i, j *そのような* $i \neq j$、$f_i(x_i)$ *および* $f_j(x_j)$ *通勤* E *全員* $x_i \in E_i$ *および* $x_j \in E_j$; *さらに* E *は部分代数* $f_i(E_i)$の和集合によって生成されます。

(ii) *F を A-代数とし、すべて* $i \in I$ として、*$u_i : E_i \to F$ *A-代数準同型とし、* $i \neq j$、$u_i(x_i)$ *および* $u_j(x_j)$ *通勤* F *すべて* $x_i \in E_i$ *および* $x_j \in E_j$。 *そして、唯一の A-代数準同型* $u : E \to F$ *そのような* $u_i = u \circ f_i$ *すべてに* $i \in I$ が存在します。

(i) I、$f_i = f_J \circ f_{J,i}$ のすべての有限部分集合 J について、(i) の最初の主張は、J 含む i と j をとって、no. 2、命題 5 から続きます。 2 番目も、J が $\mathscr{F}(I)$ を通過するときに E が $f_J(E_J)$ の和集合であるという事実を考慮して、no. 2、命題 5 から続きます。

(ii) I のすべての有限部分集合 J について、no. 2, 命題 5 から、すべての $i \in J$ に対して $u_J \circ f_{J,i} = u_i$ となる一意な準同型 $u_J : E_J \to F$ が存在することがわかります。この一意性性質から、$J \subset J'$ については、$u_J = u_{J'} \circ f_{J'J}$ がすぐに続きます。他の語、$u_J$ 形は準同型の*直接系*です。 $u = \lim \to u_J : E \to F$ にしましょう。次に、$I$ のすべての有限部分集合 $J$ に対して定義 $u_J = u \circ f_J$ が、特にすべての $i \in I$ に対して $u_i = u \circ f_i$ になります。 $u$ の一意性は、これらの関係と、$f_i(E_i)$ 生成する代数 $E$ という事実から続きます。

#### 系 {#alg-iii-s4-n5-cor-1 .statement tag=060T}

*$(E_i)_{i \in I},\ (E'_i)_{i \in I}$ * を同じインデックス付け集合を持つ 2 つの群* $A$*-代数とし、すべて* $i \in I$ について * $u_i : E_i \to E'_i$ * 代数準同型とします。その場合、唯一つ* $A$*-代数準同型性* $u : \bigotimes_{i \in I} E_i \to \bigotimes_{i \in I} E'_i$ *すべてに対して* $i \in I$, *図式* が存在します。

$$
\begin{array}{ccc}
E_i & \xrightarrow{u_i} & E'_i \\
| & & | \\
\bigotimes_{i \in I} E_i & \xrightarrow{u} & \bigotimes_{i \in I} E'_i
\end{array}
$$

*可換*、$f_i$ *および* $f'_i$ *標準準同型*を表します。

命題を適用する 8 ～ 準同型 $f'_i \circ u_i$ で十分です。

系～命題8で定義された準同型$u$を$\bigotimes_{i \in I} u_i$と表します。 $J$ が $I$ のいずれかの部分集合である場合、命題 8 は標準準同型 $f_i : E_i \to \bigotimes_{i \in I} E_i = E$ のファミリー $(f_i)_{i \in J}$ に適用できます。 標準準同型 $E_J \to E$ は、$f_J$ によっても示され、$J$ が *有限* である場合、一致すると上記の準同型で示されます。

ここで、$(x_i)_{i \in I}$ を $\prod_{i \in I} E_i$ の元として、家族 $(x_i - e_i)_{i \in I}$ が *有限台* $H$ を持つようにします。 $J$ と $J'$ が $I$ 含む $H$ の 2 つの有限部分集合である場合、それは明らかです。

$$
f_J((x_i)_{i \in J}) = f_{J'}((x_i)_{i \in J'}).
$$

$I$の有限部分集合$J \supset H$の$f_J((x_i)_{i \in J})$の共通の値は$\bigotimes_{i \in I} x_i$で表されます。

#### 命題 9 {#alg-iii-s4-prop-9 .statement tag=060U}

*$(E_i)_{i \in I}$ *を* $A$*-代数の族*とし、それぞれ* $i \in I$ *$B_i$ *基底の* $E_i$ *単位元* $e_i$ *属するから* $B_i$ とする。 *$B$ *を形* $\bigotimes_{i \in I} x_i$ の元の集合とします。 *ここで* $(x_i)$ * 集合の元 $\prod_{i \in I} B_i$ *家族* $(x_i - e_i)$ *が有限台*。 *すると* $B$ * は代数* $\bigotimes_{i \in I} E_i$ の基底 * そしてこれ基底含む単位元* $e$ です。

For every finite subset $J$ of $I$, let $B_J$ be the basis of $E_J = \bigotimes_{i \in J} E_i$ the tensor product of the bases $B_i$ for $i \in J$ (II, § 3, no. 9). 定義からすぐに、$J$ が $\mathscr{F}(I)$ を通過するとき $B$ は $f_J(B_J)$ の和集合となり、$J \subset J'$ のとき $f_{J',J}(B_J) \subset B_{J'}$ になります。したがって、$(B_J)$ は、$E_J$ と $B = \lim \rightarrow B_J$ の部分集合の直接系です。結論は II, § 6, no. 2、系から命題 5 に続きます。

The basis $B$ is also called the *tensor product* of the bases $B_i$ for $i \in I$; when the conditions of Proposition 9 are fulfilled, the canonical homomorphisms $f_J : E_J \to E = \bigotimes_{i \in I} E_i$ are *injective* for every subset $J$ of $I$, for if $B_J$ is the basis of $E_J$ the tensor product of the $B_i$ for $i \in J$, it is immediately verified that the restriction of $f_J$ to $B_J$ is injective and maps $B_J$ onto a subset of $B$.

### 6. 交換補題

#### 補題 1 {#alg-iii-s4-lem-1 .statement tag=060V}

*Let $A$ be a commutative ring, $E$ an $A$-algebra, $(x_i)_{1 \leq i \leq n}$ a finite sequence of elements of $E$, $(\lambda_i)_{1 \leq i \leq n}$ a finite sequence of elements of $A$ and $y$ an element of $E$; suppose that*
$$
x_i y = \lambda_i y x_i \quad \text{for } 1 \leq i \leq n.
$$
*Then*
$$
(x_1 x_2 \ldots x_n) y = (\lambda_1 \lambda_2 \ldots \lambda_n) y (x_1 x_2 \ldots x_n).
$$

$n = 1$ にとって補題は自明であるため、$n \geq 2$ については帰納法によって議論されます。今
$$
(x_1 x_2 \ldots x_n) y = (x_1 \ldots x_{n-1})(x_n y)
= (x_1 \ldots x_{n-1})(\lambda_n y x_n) = \lambda_n ((x_1 \ldots x_{n-1}) y) x_n,
$$
これは、帰納法の仮定により、次と等しくなります。
$$
\lambda_n (\lambda_1 \ldots \lambda_{n-1}) y (x_1 \ldots x_{n-1}) x_n = (\lambda_1 \ldots \lambda_{n-1} \lambda_n) y (x_1 \ldots x_{n-1} x_n),
$$
よって補題。

#### 補題 2 {#alg-iii-s4-lem-2 .statement tag=060W}

*$A$を可換環、$E$を$A$-代数、$(x_i)_{1 \leq i \leq n}$と$(y_i)_{1 \leq i \leq n}$を$n$の有限列、$E$の元を2つとします。 $1 \leq j \leq i \leq n$ については、*
$$
x_i y_j = \lambda_{ij} y_j x_i \quad \text{with } \lambda_{ij} \in A.
$$
*それでは*
$$
(x_1 x_2 \ldots x_n)(y_1 y_2 \ldots y_n) = \left( \prod_{i > j} \lambda_{ij} \right) (x_1 y_1)(x_2 y_2) \ldots (x_n y_n).
$$

$n = 1$ にとって補題は自明ですが、$n \geq 2$ については$n$ について帰納法によって再度議論します。 補題 1 により、
$$
(x_1 \ldots x_n)(y_1 \ldots y_n) = x_1 (x_2 \ldots x_n) y_1 (y_2 \ldots y_n)
= \left( \prod_{i > 1} \lambda_{i1} \right) (x_1 y_1)(x_2 \ldots x_n)(y_2 \ldots y_n)
$$
そして、帰納法の仮定を適用して (16) を得るだけで十分です。

すべての家族 $\lambda = (\lambda_{ij})$、$\mathbf{A}$、元、$1 \leq j < i \leq n$、およびすべての置換 $\sigma \in \mathfrak{S}_n$ について、次のように書きます。

$$
\varepsilon_\sigma(\lambda) = \prod_{i > j,\ \sigma^{-1}(i) < \sigma^{-1}(j)} \lambda_{ij} = \prod_{i < j,\ \sigma(i) > \sigma(j)} \lambda_{\sigma(i),\ \sigma(j)}.
$$

$1 \leq j < i \leq n$、$\varepsilon_\sigma(\lambda)$ が、置換 $\sigma$ (I, § 5, no. 7) の署名 $\varepsilon_\sigma$ となるように、注文されたすべての対 $(i, j)$ に対して $\mathbf{A} = \mathbf{Z}$ と $\lambda_{ij} = -1$ があることに注目してください。

#### 補題 3 {#alg-iii-s4-lem-3 .statement tag=060X}

*$\mathbf{A}$ を可換環、$\mathbf{E}$ を $\mathbf{A}$-代数、$(x_i)_{1 \leq i \leq n}$ 有限列の $\mathbf{E}$ の元とし、整数のすべての順序対 $(i, j)$ について、次のように仮定します。 $1 \leq j < i \leq n$、*

$$
x_i x_j = \lambda_{ij} x_j x_i \quad \text{with } \lambda_{ij} \in \mathbf{A}.
$$

*その後、置換 $\sigma \in \mathfrak{S}_n$ ごとに、*

$$
x_{\sigma(1)} x_{\sigma(2)} \cdots x_{\sigma(n)} = \varepsilon_\sigma(\lambda) x_1 x_2 \cdots x_n.
$$

補題は、$n = 1$ と $n = 2$ にとっては自明です。 $n$の帰納法までに$n \geq 3$まで進みます。 $\sigma(n) = n$ の場合、帰納法の仮定から関係 (19) が続きます。したがって、$\sigma(n) = k, k \neq n$ を仮定し、$\tau$ を次のように定義される $\{1, n\}$ の置換とします。

$$
\begin{cases}
\tau(i) = i & \text{for } i < k \\
\tau(i) = i + 1 & \text{for } k \leq i < n \\
\tau(n) = k.
\end{cases}
$$

$\pi = \tau^{-1} \circ \sigma$ にしましょう。 置換 $\pi$ は $n$ を固定します。現在$\sigma = \tau \circ \pi$なので、$y_i = x_{\tau(i)},\ y_{\pi(i)} = x_{\sigma(i)}$を書いています。 $i \neq n$ と $j \neq n$ の場合、関係 $\pi(i) > \pi(j)$ と $\sigma(i) > \sigma(j)$ は同等です ($\tau$ は $\{1, n-1\}$ の真に増加する写像から $\{1, n\}$ になるため)。 $i \neq n, j \neq n$と$\sigma(i) > \sigma(j)$の場合、

$$
y_{\pi(i)} y_{\pi(j)} = x_{\sigma(i)} x_{\sigma(j)} = \lambda_{\sigma(i),\ \sigma(j)} x_{\sigma(j)} x_{\sigma(i)} = \lambda_{\sigma(i),\ \sigma(j)} y_{\pi(j)} y_{\pi(i)}
$$

よって、帰納法の仮定による ($\pi(n) = n$ という事実を使用):

$$
y_{\pi(1)} y_{\pi(2)} \cdots y_{\pi(n)} = \left( \prod_{i < j < n,\ \sigma(i) > \sigma(j)} \lambda_{\sigma(i),\ \sigma(j)} \right) y_1 y_2 \cdots y_n
$$

つまり

$$
x_{\sigma(1)} x_{\sigma(2)} \cdots x_{\sigma(n)} = \left( \prod_{i < j < n,\ \sigma(i) > \sigma(j)} \lambda_{\sigma(i),\ \sigma(j)} \right) x_{\tau(1)} \cdots x_{\tau(n)}.
$$

今

$$
x_{\tau(1)} \cdots x_{\tau(n)} = x_1 \cdots x_{k-1} x_{k+1} \cdots x_n x_k
$$

そして、これは補題 1 により次と等しくなります。

$$
\left( \prod_{j > k} \lambda_{jk} \right) x_1 \cdots x_n = \left( \prod_{\sigma(i) > \sigma(n)} \lambda_{\sigma(i),\ \sigma(n)} \right) x_1 \cdots x_n.
$$

最後に、(20) と (21) は次のようになります。

$$
x_{\sigma(1)} \cdots x_{\sigma(n)} = \alpha \cdot x_1 \cdots x_n
$$

と

$$
\alpha = \left( \prod_{i < j < n, \sigma(i) > \sigma(j)} \lambda_{\sigma(i), \sigma(j)} \right) \cdot \left( \prod_{i < n, \sigma(i) > \sigma(n)} \lambda_{\sigma(i), \sigma(n)} \right)
$$
$$
= \prod_{i < j, \sigma(i) > \sigma(j)} \lambda_{\sigma(i), \sigma(j)} = \varepsilon_\sigma(\lambda)
$$

これで補題 3 の証明が完了します。

### 7. 交換因子に対する等級付けされた代数のテンソル積

#### 定義 6 {#alg-iii-s4-def-6 .statement tag=060Y}

* $(\Delta_i)_{i \in I}$ * を加法的に書かれた可換モノイドの有限族とします。 A system of commutation factors over the* $\Delta_i$ *with values in a commutative ring* $\mathbf{A}$ *is a system of mappings* $\varepsilon_{ij}: \Delta_i \times \Delta_j \to \mathbf{A}$, *where* $i \in I$, $j \in I$, $i \neq j$ *satisfying the following conditions*:

(22)
$$
\varepsilon_{ij}(\alpha_i + \alpha'_i, \beta_j) = \varepsilon_{ij}(\alpha_i, \beta_j) \varepsilon_{ij}(\alpha'_i, \beta_j)
$$
(23)
$$
\varepsilon_{ij}(\alpha_i, \beta_j + \beta'_j) = \varepsilon_{ij}(\alpha_i, \beta_j) \varepsilon_{ij}(\alpha_i, \beta'_j)
$$
(24)
$$
\varepsilon_{ij}(\alpha_i, \beta_j) \varepsilon_{ji}(\beta_j, \alpha_i) = 1,
$$

*すべて* $\alpha_i, \alpha'_i$ *in* $\Delta_i$、$\beta_j, \beta'_j$ *in* $\Delta_j$。

If I is given a total ordering and the $\Delta_i$ are groups, a system of commutation factors is defined over the $\Delta_i$ by taking for every ordered pair $(i, j)$ such that $i < j$ an arbitrary $\mathbf{Z}$-*bilinear* mapping of $\Delta_i \times \Delta_j$ into the (*multiplicative*) $\mathbf{Z}$-module $\mathbf{A}^*$ of *invertible* elements of the ring $\mathbf{A}$ and then writing

$$
\varepsilon_{ji}(\beta_j, \alpha_i) = (\varepsilon_{ij}(\alpha_i, \beta_j))^{-1}
$$

$i < j$の場合。

$\varepsilon_{ij}(\alpha_i, \beta_j)$ は反転可能なので、

$$
\varepsilon_{ij}(0, \beta_j) = \varepsilon_{ij}(\alpha_i, 0) = 1,
$$

(22) と (23) のおかげで。

#### 例 {#alg-iii-s4-n7-exa-1 .statement tag=060Z}

(1) 交換因子の *自明* 系は、$i, j$、$\alpha_i \in \Delta_i$、$\beta_j \in \Delta_j$ のすべてに対して $\varepsilon_{ij}(\alpha_i, \beta_j) = 1$ となるような $\varepsilon_{ij}$ で構成されます。

(2) 全ての$i \in I$に対して$\mathbf{A} = \mathbf{Z}$と$\Delta_i = \mathbf{Z}$をとれば、$\varepsilon_{ij}(\alpha_i, \beta_j) = (-1)^{\alpha_i \beta_j}$をとれば交換因子の系が得られます。この数は $\alpha_i$ と $\beta_j$ のパリティのみに依存するため、$\Delta_i$ の一部が $\mathbf{Z}/2\mathbf{Z}$ に等しく、その他が $\mathbf{Z}$ に等しい場合、$\varepsilon_{ij}$ は交換因子と見なされることに注意してください。

これら 2 つの例は、アプリケーションで遭遇する最も頻繁なケースです。

#### 命題 10 {#alg-iii-s4-prop-10 .statement tag=0610}

$\mathbf{A}$ を可換環とし、$(\Delta_i)_{i \in I}$ を加法的に書かれた可換モノイドの有限族とする。各々の $i \in I$ に対して、 $E_i$ を型 $\Delta_i$ の等級付けされた $\mathbf{A}$-代数とします。最後に、$(\varepsilon_{ij})$を$\mathbf{A}$の値で$\Delta_i$を超えた交換因子の系とします。次に、型 $\Delta = \prod_{i \in I} \Delta_i$ の段階的な $\mathbf{A}$-代数 $E$ と、各々の $i \in I$ 代数準同型 $h_i : E_i \to E$ が存在し、次の特性を持ちます。

(i) *$\phi_i : \Delta_i \to \Delta$ が標準準同型の場合、$h_i$ は等級付けされた準同型* (II, § 11, no. 2)、他の場合は語、$h_i(E_i^{\alpha_i}) \subset E^{\phi_i(\alpha_i)}$、$(E_i^{\alpha_i})$ と $(E^{\alpha})$ はそれぞれの卒業を示します。 $E_i$と$E$。

(ii) *$i \neq j$ と $x_i$ (それぞれ $x_j$) が、次数 $\alpha_i \in \Delta_i$ (それぞれ $\beta_j \in \Delta_j$) の $E_i$ (それぞれ $E_j$) の同次元である場合、*

$$
h_i(x_i) h_j(x_j) = \varepsilon_{ij}(\alpha_i, \beta_j) h_j(x_j) h_i(x_i).
$$

(iii) *すべての $\mathbf{A}$-代数 $F$ および準同型 $f_i : E_i \to F$ 満たす条件のすべての系について*

$$
f_i(x_i) f_j(x_j) = \varepsilon_{ij}(\alpha_i, \beta_j) f_j(x_j) f_i(x_i),
$$

*ここで、$i, j, x_i, x_j, \alpha_i, \beta_j$ が (ii) と同じである場合、すべての $i \in I$ に対して $f_i = f \circ h_i$ となる代数準同型 $f : E \to F$ が 1 つだけ存在します。さらに、$E$ の基礎となる $\mathbf{A}$ モジュールはテンソル積 $\bigotimes_{i \in I} E_i$ です。*

$\mathbf{A}\text{-module}$ $E = \bigotimes_{i \in I} E_i$ を考えてみましょう。 it is identified with 直和 of 部分加群 $E^{\alpha}$, where, for each $\alpha = (\alpha_i) \in \Delta$, we write $E^{\alpha} = \bigotimes_{i \in I} E_i^{\alpha_i}$; the $E^{\alpha}$ therefore 形 a graduation of 型 $\Delta$ on the $\mathbf{A}$-module $E$. 型 $\Delta$ の *等級付けされた $\mathbf{A}$-代数* 構造を $E$ で定義するとします。 このために、$I$ に合計順序を与えます。 元 $\alpha = (\alpha_i), \beta = (\beta_i)$ $\Delta$ の順序付けされた対ごとに、まず定義する $E^{\alpha} \times E^{\beta}$ から $E^{\alpha + \beta}$ への $\mathbf{A}$ 双線形写像、あるいは、$\mathbf{A}$ 線形写像 $m_{\alpha \beta}$ を行う必要があります。 $E^{\alpha} \otimes_{\mathbf{A}} E^{\beta}$ から $E^{\alpha + \beta}$ に。 定義する $m_{\alpha \beta}$ 条件までに

$$
m_{\alpha \beta} \left( \left( \bigotimes_{i \in I} x_i \right) \otimes \left( \bigotimes_{i \in I} y_i \right) \right) = \varepsilon(\alpha, \beta) \bigotimes_{i \in I} (x_i y_i)
$$

$x_i \in E_i^{\alpha_i}, y_i \in E_i^{\alpha_i}$ の場合、ここで

$$
\varepsilon(\alpha, \beta) = \prod_{i > j} \varepsilon_{ij}(\alpha_i, \beta_j).
$$

(27) の右辺属するから $E^{\alpha + \beta}$ と写像 $(x_1, \ldots, x_n, y_1, \ldots, y_n) \mapsto \varepsilon(\alpha, \beta) \bigotimes_{i \in I} (x_i y_i)$ は、$E_i^{\alpha_i}$ と $E_i^{\beta_i}$ ($1 \leq i \leq n$) の積で $\mathbf{A}$-多重線形です。次に、E でこのように定義された乗法が結合的であることを証明する必要があります。ここで、$\gamma = (\gamma_i)$ が $1 \leq i \leq n$ の $\Delta$ と $z_i \in E_i^{\gamma_i'}$ の 3 番目の元である場合、

$$
\left( \left( \bigotimes_i x_i \right) \left( \bigotimes_i y_i \right) \right) \left( \bigotimes_i z_i \right) = \varepsilon(\alpha + \beta, \gamma) \varepsilon(\alpha, \beta) \bigotimes_i (x_i y_i z_i)
$$

$$
\left( \bigotimes_i x_i \right) \left( \left( \bigotimes_i y_i \right) \left( \bigotimes_i z_i \right) \right) = \varepsilon(\alpha, \beta + \gamma) \varepsilon(\beta, \gamma) \bigotimes_i (x_i y_i z_i)
$$

簡約する本人確認へ

$$
\varepsilon(\alpha + \beta, \gamma) \varepsilon(\alpha, \beta) = \varepsilon(\alpha, \beta + \gamma) \varepsilon(\beta, \gamma).
$$

ただし、後者は関係からすぐに続きます。

$$
\varepsilon(\alpha + \beta, \gamma) = \varepsilon(\alpha, \beta) \varepsilon(\beta, \gamma)
$$
$$
\varepsilon(\alpha, \beta + \gamma) = \varepsilon(\alpha, \beta) \varepsilon(\alpha, \gamma)
$$

自分自身明らか帰結の定義 (28)、(22)、(23)。

すべての $i \in I$ について、$e_i$ が $E_i$ の単位元を表す場合、$e_i$ は次数 0 (§ 3, no. 1) と同次であることがわかり、したがって、$e = \bigotimes_{i \in I} e_i$ は次数 0 と同次であり、(27) から次のようになります。 (28) と関係

$$
\varepsilon_{ij}(\alpha_i, 0) = \varepsilon_{ij}(0, \beta_j) = 1
$$

$e$ は $E$ の単位元であり、希望する等級 A-代数構造の $E$ で定義が完了します。次に、$h_i(x_i) = x_i \otimes \bigotimes_{j \neq i} e_j$ を選択します。 $E_i$ の $x_i, x_i'$ に対する $h_i(x_i x_i') = h_i(x_i) h_i(x_i')$ を検証するには、$x_i$ と $x_i'$ が同種で、この関係が (27) と関係 $\varepsilon_{ij}(\alpha_i, 0) = \varepsilon_{ij}(0, \beta_j) = 1$ の直後に続く場合に注意を限定することができます。同じ関係と (24) は、主張の $h_i$ 満たす条件 (i) と (ii) も証明します。

$$
\bigotimes_{i \in I} x_i = \prod_{i \in I} h_i(x_i)
$$

ここで、右辺は E の順序付けされた数列 $(h_i(x_i))_{i \in I}$ の積であり、指定された合計順序付けは I (I, § 1, no. 2) になります ($x_i$ (均一であると仮定) の数について帰納法によって議論するだけで十分です。 $e_i$）。

条件 (iii) を証明することはまだ残っています。 写像に注意してください

$$
(x_i)_{i \in I} \mapsto \prod_{i \in I} f_i(x_i),
$$

ここで、右辺は $I$ に与えられた合計順序を伴う順序付け数列 $(f_i(x_i))_{i \in I}$ の積であり、A 多重線形です。すると、次のような A-線型写像 $f : E \to F$ が 1 つだけ存在します。

$$
f\left( \bigotimes_{i \in I} x_i \right) = \prod_{i \in I} f_i(x_i).
$$

明らかに、$f(e)$ は $F$ と $f \circ h_i = f_i$ の単位元です。 $f$ が代数準同型であること、他の語では $f(x)f(y) = f(xy)$ が $E$ の $x, y$ であることを検証するには、線形性により、$x = \bigotimes_{i \in I} x_i$ と $y = \bigotimes_{i \in I} y_i$、$x_i$ (それぞれ$y_i$) は、すべての $i \in I$ に対して次数 $\alpha_i$ (それぞれ $\beta_i$) と同種です。 関係が検証され、その後、簡約する、(27) によって、

$$
\left( \prod_{i \in I} f_i(x_i) \right) \left( \prod_{i \in I} f_i(y_i) \right) = \varepsilon(\alpha, \beta) \prod_{i \in I} (f_i(x_i) f_i(y_i)).
$$

しかし、関係 (26) を考慮すると、これは no. 6 の補題 2 の帰結です。

明らかに、代数 $E$ と標準写像 $\psi : \bigotimes_{i \in I} E_i \to E$ は、*普遍写像問題* (*集合理論*, IV, § 3, no. 1) の解を構成します。ここで、$\Sigma$ はA-代数構造の種と、$\prod_i E_i$ から A-代数、満たす条件までの $\alpha$-マッピング $\prod_i f_i$ (26)。

$I$ の固定合計順序の場合、命題 10 の証明で定義された等級付けされた代数 $E$ は、ファミリーの * 等級付けされたテンソル $\varepsilon$-積型* $\Delta$ と呼ばれます。 型 $\Delta_i$ のグレーディング代数の $(E_i)_{i \in I}$ は、$^{\varepsilon} \bigotimes_{i \in I} E_i$ で示されます ($I$ の順序に混乱が生じない場合)。同様に、命題10の証明で定義された準同型$f : E \to F$は$^{\varepsilon} \bigotimes_{i \in I} f_i$と表記されます。 準同型 $h_i$ は *正規* と呼ばれます。 $I = \{1, n\}$ とすべての $E_i$ が同じ代数 $G$ に等しい場合も、$^{\varepsilon} G^{\otimes n}$ と書きます。

#### 注意 {#alg-iii-s4-n7-rem-1 .statement tag=0611}

(1) すべての $i, j, \alpha_i$ と $\beta_j$ に対して $\varepsilon_{ij}(\alpha_i, \beta_j) = 1$ をとり、no. 1 で定義された代数のテンソル積 (さらにその因子の卒業テンソル積を含む) を復元します。

(2) すべての $\Delta_i$ が $\mathbf{Z}$ に等しいと仮定し、$\varepsilon_{ij}(\alpha_i, \beta_j) = (-1)^{\alpha_i \beta_j}$ と書きます。 テンソル $\varepsilon$-積 $^{\varepsilon} \bigotimes_{i \in I} E_i$ 対応するから、交換因子の系は、グレード付けされた代数 $E_i$ の *スキュー* テンソル積と呼ばれます。 型 $\mathbf{Z}$ は $^{\varepsilon} \bigotimes_{i \in I} E_i$ (または代数が 2 つの場合は $E \ ^{\varepsilon} \otimes_A F$、または $^{\varepsilon} G^{\otimes n}$ の代わりに $^{\varepsilon} G^{\otimes n}$) で表されます。

#### 系 1 {#alg-iii-s4-prop-10-cor-1 .statement tag=0612}

命題 10 の記法では、さらに F が型 $\Delta$ の等級付けされた A-代数であり、各 $f_i$ が $\phi_i : \Delta_i \to \Delta$ に対して等級付けされた代数準同型であると仮定します。その場合、$f = \varepsilon \bigotimes_i f_i$ はグレード代数準同型です。

これは、$f$ の定義と次の事実からすぐに続きます。
$$
\sum_{i \in I} \phi_i(\alpha_i) = (\alpha_i)
$$
$\phi_i$の定義による。

したがって、$(E, \psi)$ は、普遍的な他の写像問題の解でもあり、今回の $\Sigma$ は、*等級付けされた A-代数* 構造 *of 型* $\Delta$ の種です。 射は型 $\Delta$ の代数準同型と $\alpha$ マッピング写像 $\prod_i f_i$ で、加法から条件 (26) では、$f_i$ がグレード付けされていると想定されます。 $\phi_i$ に対して代数準同型。

#### 系 2 {#alg-iii-s4-prop-10-cor-2 .statement tag=0613}

* $(E_i)_{i \in I}, (F_i)_{i \in I}$ * を、* $E_i$ * と* $F_i$ * 型* $\Delta_i$ *すべて* $i \in I$ を持つ* A* 代数の 2 つの有限族としましょう。 *それぞれ* $i \in I$、*$g_i : E_i \to F_i$ を *型* $\Delta_i$ の代数準同型とします。 *その後、* $h_i : E_i \to \varepsilon \bigotimes_{i \in I} E_i$ * と* $h'_i : F_i \to \varepsilon \bigotimes_{i \in I} F_i$ * が標準準同型である場合、 型* $\Delta$、$g : \varepsilon \bigotimes_{i \in I} E_i \to \varepsilon \bigotimes_{i \in I} F_i$ の段階的* A* 代数の準同型が 1 つだけ存在します* $g \circ h_i = h'_i \circ g_i$ *すべてに対して* $i \in I$。 *また、それぞれ* $g_i$ *が全単射である場合、* $g$ も同様です。

系を適用する 1 から $f_i = h'_i \circ g_i$ までにするだけで十分です。ただし、条件 (26) が $h'_i$ に適用される関係 (25) から続くことに注意してください。

系 2 で定義された準同型は、(混乱が生じない限り) $\varepsilon \bigotimes_i g_i$ とも表されます。それぞれの $i \in I$ 、 $G_i$ が型 $\Delta_i$ の 3 番目のグレード A-代数と $g'_i : F_i \to G_i$ がグレード代数準同型である場合、
$$
\left( \varepsilon \bigotimes_i g'_i \right) \circ \left( \varepsilon \bigotimes_i g_i \right) = \varepsilon \bigotimes_i (g'_i \circ g_i),
$$
(30) からすぐに次のようになります。

型 $\mathbf{Z}$ のグレーディング代数の *スキュー* テンソル積の場合、型のグレーディング代数の準同型 $f_i : E_i \to F_i$ に対して、$\varepsilon \bigotimes_i f_i$ の代わりに $\varepsilon \bigotimes_i f_i$ と書きます。 $\mathbf{Z}$; $I = \{1, 2\}$のとき、この準同型は$f_1 \varepsilon \otimes f_2$でも表されます。 $I = \{1, n\}$ とすべての $E_i$ (それぞれ $F_i$) が等しく、すべての $f_i$ が同じ準同型 $f$ に等しい場合、$\varepsilon f^{\otimes n}$ と書きます。

#### 注意 {#alg-iii-s4-n7-rem-2 .statement tag=0614}

命題 10 の証明では、$I$ の合計順序が定義するの *代数* 構造テンソル積 A-加群の$\bigotimes_{i \in I} E_i$ に使用されました。

E_i. I の順序が変更されると、$\bigotimes_{i \in I} E_i$ で他の乗法構造が生じますが、こうして得られた新しい代数は、両方とも同じ普遍写像問題の解であるため、上記と正準的に *同型* になります。たとえば、$I = \{1, 2\}$、標準同型の代数 $E_1 \overset{\varepsilon}{\otimes}_A E_2$ が代数 $E_2 \overset{\varepsilon}{\otimes}_A E_1$ 写像 $x_1 \otimes x_2$ から $\varepsilon_{2,1}(\alpha, \beta)x_2 \otimes x_1$ になるとき、$x_1$ は次数 $\alpha$ と同次です。そして次数 $\beta$ の同種の $x_2$ 。

J を I の部分集合とし、それぞれの $i \in J$ について、標準準同型 $h_i : E_i \to \varepsilon \bigotimes_{i \in I} E_i = E$ を考慮します。 関係 (25) 標準準同型 $h : E' = \varepsilon \bigotimes_{i \in J} E_i \to E$ は、これらの準同型から正規に (命題 10 によって) 導出され、すべての $i \in J$、$h'_i = h \circ h_i$、$h'_i$ は標準準同型になります。 $E_i \to E'$。 I で選択された順序によって引き起こされる J の合計順序を取得すると、次のようになります。

$$
h\left( \bigotimes_{i \in J} x_i \right) = \prod_{i \in I} h_i(x_i) = \bigotimes_{i \in I} x'_i
$$

ここで、中央の項は*注文された数列* $(h_i(x_i))_{i \in J}$の積で、右手の項、$x'_i = x_i$は$i \in J$、$x'_i = e_i$は$i \notin J$です。

#### 命題 11 {#alg-iii-s4-prop-11 .statement tag=0615}

(テンソル $\varepsilon$-積の「結合性」)。 *命題 10 の記法では、* $(J_\lambda)_{\lambda \in L}$ *を I の分割にして、* $\Delta'_\lambda = \prod_{i \in J_\lambda} \Delta_i$ *すべて* $\lambda \in L$ と書きます。 *$E'_\lambda$ *テンソル $\varepsilon$ - 型* $\Delta'_\lambda$ *家族* $(E_i)_{i \in J_\lambda}$ *$J_\lambda$ に選択された合計順序の積であるとしましょう。 *一方、* $\lambda, \mu$ *in* $L$ *および* $\lambda \neq \mu$ については、*$\alpha'_\lambda = (\alpha_i)_{i \in J_\lambda}$、$\beta'_\mu = (\beta_j)_{j \in J_\mu}$ について、*と書きます。

$$
\varepsilon'_{\lambda \mu}(\alpha'_\lambda, \beta'_\mu) = \prod_{i \in J_\lambda, j \in J_\mu} \varepsilon_{ij}(\alpha_i, \beta_j).
$$

*その後* $(\varepsilon'_{\lambda \mu})$ *は交換因子の系です* $\Delta'_\lambda$ *値を* $A$ *そして型の代数の準同型が 1 つだけ存在します* $\Delta$、$v : \varepsilon' \bigotimes_{\lambda \in L} E'_\lambda \to \varepsilon \bigotimes_{i \in I} E_i$、*そのような*

$$
v\left( \bigotimes_{\lambda \in L} \left( \bigotimes_{i \in J_\lambda} x_i \right) \right) = \bigotimes_{i \in I} x_i
$$

*すべて* $(x_i) \in \prod_{i \in I} E_i$、*合計順序付けが I で行われ、各 * $J_\lambda$ で誘導するが合計順序付けを選択し、* $\lambda < \mu$ * $L$、$i \in J_\lambda$ * および* $j \in J_\mu$ について、 $i < j$。

交換因子の $\varepsilon'_{\lambda \mu}$ 形系という事実は些細なことです。 $h_{i,\lambda} : E_i \to E'_\lambda$、$h'_\lambda : E'_\lambda \to \varepsilon' \bigotimes_{\lambda \in L} E'_\lambda$ *を標準準同型* ($\lambda \in L$、$i \in J_\lambda$の場合) *そして、$h''_i = h'_\lambda \circ h_{i,\lambda}$と書きます*。 *普遍的な写像問題の解の一意性によって、 $\varepsilon' \bigotimes_{\lambda \in L} E'_\lambda$ と命題 10 の $h''_i$ 満たす条件を示すだけで十分です。 $\lambda \in L$、$f'_\lambda : E'_\lambda \to F$ を一意な代数準同型とし、すべての $i \in J_\lambda$ に対して $f'_\lambda \circ h_{i,\lambda} = f_i$ とします。 $\lambda \neq \mu$、$\alpha'_\lambda = (\alpha_i)_{i \in J_\lambda}, \beta'_\mu = (\beta_j)_{j \in J_\mu}$ については、

$$
f'_\lambda(x'_\lambda)f'_\mu(x'_\mu) = \varepsilon'_{\lambda\mu}(\alpha'_\lambda, \beta'_\mu)f'_\mu(x'_\mu)f'_\lambda(x'_\lambda)
$$

$x'_\lambda \in E'_\lambda$ (それぞれ $x'_\mu \in E'_\mu$) は次数 $\alpha'_\lambda$ (それぞれ $\beta'_\mu$) と同種です。 $x'_\mu = \bigotimes_{i \in J_\lambda} x_i, x'_\mu = \bigotimes_{j \in J_\mu} x_j, x_i$ (それぞれ $x_j$) が $i \in J_\lambda, j \in J_\mu$ の $E_i$ (それぞれ $E_j$) で次数 $\alpha_i$ (それぞれ $\beta_j$) と同次である場合、線形性により検証するだけで十分です。しかし、これは、仮定 (26) と定義 (32) を考慮して、no. 6 の $f'_\lambda$ と補題 3 を定義する足したものから公式 (30) になります。したがって、すべての $\lambda \in L$ に対して $f \circ h'_\lambda = f'_\lambda$ となるような代数準同型 $f : \varepsilon' \bigotimes_{\lambda \in L} E'_\lambda \to F$ は 1 つだけです。 $f$ のすべての $i \in I$ と一意性に対するよって $f \circ h''_i = f_i$ は簡単です。

### 8. テンソル積のグレード代数の同じ型

no. 7、命題 10 の仮説が成立すると仮定し、さらにすべての $\Delta_i$ が *同じ可換モノイド* $\Delta_0$ に等しいと仮定します。次に、テンソル $\varepsilon$-積 $\varepsilon \bigotimes_{i \in I} E_i$ で、この代数 (II, § 11, no. 1) の型 $\Delta = \Delta_0^I$ の卒業に関連する型 $\Delta_0$ の *合計卒業* を考えることができます。この卒業式を使って、型 $\Delta_0$ の等級付けされた代数の家族 $(E_i)_{i \in I}$ の型* $\Delta_0$ の * 等級付けされたテンソル $\varepsilon$ を $\varepsilon \bigotimes_{i \in I} E_i$ と呼びます。

no. 7 の命題 10 の記法を常に保持し、$F$ も型* $\Delta_0$ の * グレード A-代数であり、$f_i$ がグレードの *準同型であると仮定します。 型* $\Delta_0$ の代数。その場合、$f : \varepsilon \bigotimes_{i \in I} E_i \to F$ も、型* $\Delta_0$ の等級付けされた代数の *準同型です。 公式 (30) (no. 7) から、$x_i$ が均一で、次数の場合であることがわかります。 $\alpha_i \in \Delta_0, \bigotimes_{i \in I} x_i$ と $\prod_{i \in I} f_i(x_i)$ はどちらも次数 $\sum_{i \in I} \alpha_i \in \Delta_0$ と同種です。

したがって、$\varepsilon \bigotimes_{i \in I} E_i$ は、型 $\Delta_0$ の総目盛りを持ち、標準写像 $\psi$ とともに、解が第三普遍写像問題を構成すると言えます。ここで、$\Sigma$ は *段階的な種です。 型* $\Delta_0$、射の A-代数は、型 $\Delta_0$ のグレード付けされた代数の準同型であり、$\alpha$ マッピングは写像 $\prod_i f_i$ です。 加法から条件 (26) (no. 7 のうち) では、各 $f_i$ は型 $\Delta_0$ のグレード代数の準同型であると想定されます。

I のすべての部分集合 J に対して、標準準同型 $\varepsilon \bigotimes_{i \in J} E_i \to \varepsilon \bigotimes_{i \in I} E_i$ (no. 7) は、実際には、上記からすぐにわかるように、型 $\Delta_0$ の等級付けされた代数の準同型です。

#### 命題 12 {#alg-iii-s4-prop-12 .statement tag=0616}

(テンソル $\varepsilon$ の「結合性」 - 同じ型の等級付けされた代数の積)。 *no. 7の命題10の記法では、すべての$\Delta_i$が同じモノイド$\Delta_0$に等しいと仮定します。 $(J_\lambda)_{\lambda \in L}$をIの分割とします。 no. 7 の命題 11 の記法では、公式 (32) (no. 7) の右辺が、個別の順序付けられたすべての対 $(\lambda, \mu)$ について、和 $\alpha''_\lambda = \sum_{i \in J_\lambda} \alpha_i, \beta''_\mu = \sum_{j \in J_\mu} \beta_j$ のみに依存すると仮定します。 添字、すべての $\alpha'_\lambda \in \Delta'_\lambda$、およびすべての $\beta'_\mu \in \Delta'_\mu$。 $\varepsilon''_{\lambda \mu}(\alpha''_\lambda, \beta''_\mu)$ を (32) の右辺とします。 *すると、$(\varepsilon''_{\lambda \mu})$ は、家族 $(\Delta''_\lambda)_{\lambda \in L}$ に対する交換因子の系であり、すべての $\lambda \in L$ では $\Delta''_\lambda = \Delta_0$ となります。 *$E''_\lambda$ が $(E_i)_{i \in J_\lambda}$ ファミリーの型 $\Delta_0$ のグレードテンソル $\varepsilon$ の積である場合、型のグレード代数の同型が 1 つだけ存在します。 $\Delta_0$、$w : \varepsilon'' \bigotimes_{\lambda \in L} E''_\lambda \to \varepsilon \bigotimes_{i \in I} E_i$、そのような

$$
w \left( \bigotimes_{\lambda \in L} \left( \bigotimes_{i \in J_\lambda} x_i \right) \right) = \bigotimes_{i \in I} x_i
$$

*ただし、no. 7、命題 11 で説明されているように、合計注文数が $J_\lambda$ と I で選択された場合に限ります。*

仮定までに、$\Delta_0$の$\gamma, \delta$、$i_0 \in J_\lambda$と一部の$j_0 \in J_\mu$で$\varepsilon''_{\lambda \mu}(\gamma, \delta) = \varepsilon_{i_0 j_0}(\gamma, \delta)$が、元$\alpha'_\lambda = (\alpha_i)_{i \in J_\lambda}$と$\beta'_\mu = (\beta_j)_{j \in J_\mu}$を考慮するとわかるように、$\alpha_{i_0} = \gamma, \alpha_i = 0$は$i \neq i_0$、$\beta_{j_0} = \delta, \beta_j = 0$、$j \neq j_0$。直ちに、交換因子の $\varepsilon''_{\lambda \mu}$ 形系が続きます。 証明の残りは命題 11 (no. 7) の残りと類似しており、読者に委ねられます。

命題 12 の追加の仮説は、$\Delta_0 = \mathbf{Z}$ のときに満たされ、$(\varepsilon_{ij})$ は、すべての $i, j$ に対する因子 $(\varepsilon_{ij}(\alpha_i, \beta_j)) = 1$ の自明な系か、または以下で定義される因子の系であることに注意してください。 $\varepsilon_{ij}(\alpha_i, \beta_j) = (-1)^{\alpha_i \beta_j}$;後者の場合、公式 (32) の右辺は $(-1)^\gamma$ に等しくなります。

$$
\gamma = \sum_{i \in J_\lambda, j \in J_\mu} \alpha_i \beta_j = \left( \sum_{i \in J_\lambda} \alpha_i \right) \left( \sum_{j \in J_\mu} \beta_j \right).
$$

#### 注意 {#alg-iii-s4-n8-rem-1 .statement tag=0617}

(1) I を無限インデックス集合および $\Delta_0$ を可換モノイドとする。 $(\Delta_i)_{i \in I}$ がすべての $i$ に対して $\Delta_i = \Delta_0$ となるような族を表し、I 写像 $\varepsilon_{ij} : \Delta_i \times \Delta_j \to A$ 満たす条件の個別の添字 $(i, j)$ の順序付けられた対ごとに与えられると仮定します (22)、 (23) と (24) (no. 7);これは、家族* $(\Delta_i)$ に対する交換因子の *系とも呼ばれます。 型 $\Delta_0$ のグレーディング A-代数のファミリー $(E_i)_{i \in I}$ を考えてみましょう。 I の各有限部分集合 J について、$E_J$ は、サブファミリー $(E_i)_{i \in J}$ の型* $\Delta_0$ の * 等級付けされたテンソル $\varepsilon$ 積を表します (J の合計順序の任意の選択を使用)。 If J, J' are two finite subsets of I such that $J \subset J'$, a canonical homomorphism of graded algebras of type $\Delta_0$, h_{J'J}: E_J \to E_{J'}, has been defined above and the uniqueness properties of these homomorphisms show immediately that if J \subset J' \subset J'' are three finite subsets of I, then h_{J''J} = h_{J'J'} \circ h_{J'J}. したがって、型 $\Delta_0$ (§ 3, no. 3) の等級付けされた代数の直接系 (E_J, h_{J'J}) があり、そのインデックス付け集合は I の有限部分集合の右側有向集合 $\mathfrak{F}(I)$ です。 型 $\Delta_0$ の等級付けされた代数、この直接系 (§ 3, no. 3) の *直接極限* は、ファミリー $(E_i)_{i \in I}$ の型* $\Delta_0$ の *等級付けされたテンソル $\varepsilon$-積 と呼ばれます。 $\varepsilon \bigotimes_{i \in I} E_i$ とも表されます。 すべての $\Delta_i$ が $\mathbf{Z}$ および $\varepsilon_{ij}(a_i, \beta_j) = (-1)^{\alpha_i \beta_j}$ に等しい場合、テンソル積 $\varepsilon \bigotimes_{i \in I} E_i$ はファミリー $(E_i)_{i \in I}$ の *スキュー* テンソル積とも呼ばれ、$g \bigotimes_{i \in I} E_i$ で示されます。 We leave to the reader the task of formulating and proving the proposition which generalizes Proposition 10 of no. 7 to the case where I is infinite, as Proposition 8 of no. 5 generalizes Proposition 5 of no. 2 to the case where I is infinite. $\varepsilon \bigotimes_{i \in I} E_i$ の基礎となる A-加群は、no. 5 で定義された非等級付け代数のファミリー $(E_i)_{i \in I}$ の (非等級付け) テンソル積の基礎となるものと同じであることに注意してください。

(2) E を型 $\Delta_0$ ($\Delta_0$ は可換モノイド) および $\rho : A \to B$ 環準同型の段階的 A-代数とする。 $\rho^*(E)$ (II, § 11, no. 5) の目盛りは、等級付けされたテンソル積 $B \otimes_A E$ の目盛りと同じです。ここで、B は自明な目盛りを持ちます。

### 9. 反可換的代数および交代的代数

#### 定義 7 {#alg-iii-s4-def-7 .statement tag=0618}

*すべての非ゼロ同次元 x, y の E* について、型 $\mathbf{Z}$ の等級付けされた A-代数 E は反可換性と呼ばれます*

$$
xy = (-1)^{\deg(x)\deg(y)} yx.
$$

*代数 E は、反可換である場合は交代的と呼ばれ、奇数次数のすべての同次元 $x \in E$ については $x^2 = 0$ と呼ばれます。*

#### 注意 {#alg-iii-s4-n9-rem-1 .statement tag=0619}

(1) $E^+$ を、$E_{2n}$ ($n \in \mathbf{Z}$) の E 直和の等級付けされた部分代数とします。 定義 7 から、E が反可換である場合、$E^+$ は * E の中心に含まれる *部分代数である (したがって可換である) ことがわかります。

(2) 2 が E の 0 の因子ではないとします。 E が反可換である場合、E は交代的です。$x \in E$ が同次で奇数次数の場合、(36) により $x^2 = -x^2$、仮定によりよって $2x^2 = 0$ および $x^2 = 0$ です。

(3) 交代的代数の§ 7 重要例を詳しく勉強していきます。

#### 補題 4 {#alg-iii-s4-lem-4 .statement tag=061A}

*E を型 $\mathbf{Z}$ の等級付けされた代数および同種元 $\neq 0$ の S 集合とする。 E の元の集合 F、そのすべての同種成分 $x \neq 0$ 満たす関係 (36) のすべての $y \in S$ は、E の等級付けされた部分代数です。*

(1) $x', x''$ が、同じ次数 $p$、$y$ の 2 つの同種元、次数 $q$ と $x'y = (-1)^{pq}yx'$、$x''y = (-1)^{pq}yx''$ の同種元である場合、それから$(x' + x'')y = (-1)^{pq}y(x' + x'')$も。 (2) $x', x''$ が、それぞれ次数 $p', p''$、$y$ の 2 つの同種元、次数 $q$ と $x'y = (-1)^{p'q}yx'$、$x''y = (-1)^{p''q}yx''$ の同種元である場合、
$$
(x'x'')y = (-1)^{(p'+p'')q}y(x'x'').
$$

#### 命題 13 {#alg-iii-s4-prop-13 .statement tag=061B}

*Let E be a graded A-algebra of type $\mathbf{Z}$ and S a generating system of the algebra E consisting of homogeneous elements $\neq 0$; for E to be anticommutative (resp. alternating), it is necessary and sufficient that (36) hold for all $x \in S$ and $y \in S$ (resp. that this condition hold and further that $x^2 = 0$ for all $x$ homogeneous of odd degree belonging to S).*

まず反可換代数の場合を考えます。 補題 4、部分代数 F からなるの元により、そのすべての同種成分 $x \neq 0$ 満たす (36) により、S のすべての $y \in S$、含むすべての元およびしたがって$F = E$。ここで、$F'$ が同様に、元の E からなるの部分代数であり、そのすべての同次元 $y \neq 0$ に対して、そのすべてが同次成分 $x \neq 0$ 満たす (36) である場合、上記から次のことがわかります。 $F'$ 含む S のすべての元、したがって $F' = E$ となり、この場合、命題の証明が完成します。

To prove the proposition in the case of alternating algebras, it can be assumed that E is already anticommutative; it is then immediate that every homogeneous element of odd degree in E is of the form $\sum_i z_ix_i$, where $z_i \in E^+$ and $x_i \in S$ is of odd degree (using the fact that $E^+$ is contained in the centre of E); it follows that $\left( \sum_i z_ix_i \right)^2 = \sum_i z_i^2x_i^2 + \sum_{i<j} z_i z_j (x_ix_j + x_jx_i) = 0$ since $x_i^2 = 0$ by hypothesis and $x_ix_j + x_jx_i = 0$ by (36).

#### 命題 14 {#alg-iii-s4-prop-14 .statement tag=061C}

*E と F を型 $\mathbf{Z}$ の 2 つの等級 A-代数とし、両方とも反可換性 (それぞれ交代的) であるとします。この場合、スキュー テンソル積 $E^g \otimes_A F$ (no. 7) は反可換です (それぞれ交代的) 代数。*

$E^g \otimes_A F$ の生成する系は $x \otimes y$ で構成され、$x$ (それぞれ $y$) は E (それぞれ F) の同次元 $\neq 0$ です。このような 2 つの元 $x \otimes y, x' \otimes y'$ と $\deg(x) = p, \deg(y) = q, \deg(x') = p', \deg(y') = q'$ を考えて、$x \otimes y$ は次数 $p + q$ と $x' \otimes y'$ は次数 $p' + q'$ になります。その後、定義 (no. 7, 公式 (27)) までに (36) により、
$$
\begin{align*}
(x \otimes y)(x' \otimes y') &= (-1)^{qp'}(xx') \otimes (yy') \\
(x' \otimes y')(x \otimes y) &= (-1)^{pq'}(x'x) \otimes (y'y) \\
&= (-1)^{pq'+pp'+qq'}(xx') \otimes (yy')
\end{align*}
$$
そして、命題 13 の基準は、$E^g \otimes_A F$ が $pq' + pp' + qq' - qp' \equiv (p + q)(p' + q')$ (mod. 2) 以来反交換的であることを示しています。さらに E と F が交代的で、$p + q$ が奇数の場合、数 $p, q$ のいずれかが必ず奇数であるため、$(x \otimes y)^2 = \pm (x^2) \otimes (y^2) = 0$ と命題 13 は、$E^g \otimes_A F$ が交代的であることを示します。

#### 系 {#alg-iii-s4-n9-cor-1 .statement tag=061D}

*E を反可換変数* (それぞれ *交代的*) とします。 * 型 $\mathbf{Z}$ の A-代数に等級付けされます。次に、すべての環準同型 $\rho : A \to B$ について、次数付き B 代数 $\rho^*(E)$ (no. 8, *注意 2*) は *反可換* (それぞれ *交代的*) です。

自明な目盛りの環 B は、交代的 A-代数および $\rho^*(E) = E^g \otimes_A B$ と見なすことができるため、命題 14 が適用できます。

#### 注意 {#alg-iii-s4-n9-rem-2 .statement tag=061E}

E を型 $\mathbf{Z}$ の A-代数に等級付けされた反可換式とする。 Then the A-linear mapping of $E \otimes_A E$ into E defined by multiplication of E ($§ 1$, no. 3) is a homomorphism of the graded A-algebra $E^g \otimes_A E$ into E, for in the notation of Proposition 14, in the algebra E,
$$
(xy)(x'y') = (-1)^{qp'}(xx')(yy').
$$

### 練習問題 {#alg-iii-s4-exercises}

[§ 4 に対して練習問題](exercises/s4/)を参照してください。
