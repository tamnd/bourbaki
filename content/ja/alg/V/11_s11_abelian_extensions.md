---
book: alg
book_title: Algebra
chapter: V
chapter_title: COMMUTATIVE FIELDS
section: 11
section_title: Abelian extensions
lang: ja
source: alg-iv-vii
source_edition: 2003, Springer
book_pages: A V.160-A V.166
pdf_pages: 0191-0207, 0274-0280
extraction: ocr
subsections:
    - "no": 1
      title: Abelian extensions and the abelian closure
      page: 77
      pdf_page: 191
    - "no": 2
      title: Roots of unity
      page: 78
      pdf_page: 192
    - "no": 3
      title: Primitive roots of unity
      page: 79
      pdf_page: 193
    - "no": 4
      title: Cyclotomic extensions
      page: 81
      pdf_page: 195
    - "no": 5
      title: Irreducibility of cyclotomic polynomials
      page: 83
      pdf_page: 197
    - "no": 6
      title: Cyclic extensions
      page: 85
      pdf_page: 199
    - "no": 7
      title: Duality of $\mathbf{Z}/n\mathbf{Z}$-modules
      page: 86
      pdf_page: 200
    - "no": 8
      title: Kummer theory
      page: 88
      pdf_page: 202
    - "no": 9
      title: Artin-Schreier theory
      page: 91
      pdf_page: 205
statements: 45
exercises: 23
content_sha256: ad3022838e46b6c56ce44f7dbf1e7c4851cec6e66bf18d9dc12ba12b287956b4
translated_from: content/en/alg/V/11_s11_abelian_extensions.md
translation_method: google
source_content_sha256: 3510a553a6737e108ce1bbc1176deb8962c17c7a4a3f4de1c127471caa214100
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-b071ad41
glossary_version: 34
glossary_terms_sha256: 77a6165bbc38b9456a605ca6f993b0371d4dc482fc8c9fe1899e7961997d7efc
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## § 11。 アーベル拡大

この段落全体を通じて、K は体を表します。

### 1. アーベル拡大およびアーベルの閉鎖

#### 定義 1 {#alg-v-s11-def-1 .statement tag=06OC}

— ガロアであり、そのガロア群が可換である場合、K の拡大 E はアーベルであると言われます。

可換群のすべての部分群は正規であるため、Cor. V、p. 68 の 4 は、アーベル拡大のすべてのサブエクステンションがアーベルであることを示します。

#### 命題 1 {#alg-v-s11-prop-1 .statement tag=06OD}

— E を K のガロア拡大とし、Γ をそのガロア群とします。 A を Γ (I, p. 10, Def. 4) の導来群とし、A の不変式の F 体とする。E への部分拡張 L がアーベルとなるためには、それが F に含まれることが必要かつ十分である。

まず、F は Γ における A の閉包 $\bar{\Delta}$ の不変量の体であり、$\bar{\Delta}$ は Γ の閉正規部分群であることに注意します。 V、p. 68、Cor. 4 より、F は K のガロア拡大です。さらに、K 上の F のガロア群は $\Gamma / \bar{\Delta}$ と同型であり、したがって可換です。したがって、F のすべての部分拡張はアーベルになります。逆に、LをEに含まれるKのアーベル拡大とし、ΠをLにわたるEのガロア群とします。 L はガロアであるため、Π は Γ の正規部分群であり、K 上の L のガロア群は $\Gamma / \Pi$ (V, p. 68, Cor. 4) と同型です。したがって、$\Gamma / \Pi$ は可換であり、Π 含む A、よって $L \subset F$ です。

#### 系 {#alg-v-s11-n1-cor-1 .statement tag=06OE}

— E を K の拡大とし、$(E_i)_{i \in I}$ を $E = K \left( \bigcup_{i \in I} E_i \right)$ のような E の部分拡張のファミリーとします。それぞれの拡大 $E_i$ がアーベルであると仮定すると、同じことが E にも当てはまります。

そもそも E は K のガロア拡大です (V, p. 57、提案 1)。 体 F が提案 1 のように定義されている場合、すべての $i \in I$、よって $E = F$ に対して $E_i \subset F$ が得られます。

K の拡大 E は、K のアーベル拡大であり、K のすべてのアーベル拡大が E の部分拡張と同型である場合、K のアーベル閉包であると言われます。提案 1 は、K のアーベル閉包の存在を意味します。 $K_s$ は、ガロア群 $\Gamma$ を伴う K の分離閉包であり、$(\overline{\Gamma}, \overline{\Gamma})$ を $\Gamma$ の導来群の閉包とします。 $(\overline{\Gamma}, \overline{\Gamma})$ の不変式の $K_{ab}$ 体で表します。なぜなら、K のすべての可分代数拡大は $K_s$ (V, p. 45, Cor.) の部分拡張と同型であるからです。提案 1 は、$K_{ab}$ が K のアーベル閉包であることを示しています。K 上の $K_{ab}$ のガロア群は、$\Gamma / (\overline{\Gamma}, \overline{\Gamma})$ と正準的に同型です。ここで、アーベルクロージャのうち一意性を示しましょう。E、E' を K の 2 つのアーベルクロージャとします。 定義により、K 準同型性 $u : E \to E'$ と $v : E' \to E$ が存在し、提案 1 (V, p. 52) は $v(u(E)) = E$ と $u(v(E')) = E'$ を意味するため、$u$ は E から E' への K 準同型性です。 E の E' へのその他の K-同型写像は、$\sigma_0 \in \mathrm{Gal}(E'/K)$ と形 $u_1 = \sigma_0 \circ u$ になります。 $\mathrm{Gal}(E'/K)$ は可換であるため、$\mathrm{Gal}(E/K)$ の $\sigma \mapsto u \circ \sigma \circ u^{-1}$ から $\mathrm{Gal}(E'/K)$ への同型は$u$ から独立しています。 $\mathrm{Gal}(E/K)$の$\mathrm{Gal}(E'/K)$の標準同型と呼ばれます。

### 2. 単位元中根

#### 定義 2 {#alg-v-s11-def-2 .statement tag=06OF}

* $\zeta^n = 1$ となる整数 $n > 0$ が存在する場合、K の元 $\zeta$ は単位元の根であると言われます。 整数 $n > 0$ ごとに、$\zeta^n = 1$、$\zeta$ は単位元の n 番目の根と呼ばれます。*

It amounts to the same to say that the roots of unity are the elements of *finite order* of the multiplicative group $K^*$ of non-zero elements of K (I, p. 51). The roots of unity form a subgroup $\mu_\infty(K)$ of $K^*$, the n-th roots form a subgroup $\mu_n(K)$ of $\mu_\infty(K)$. $n$ 割る $m$ の場合、$\mu_\infty(K) = \bigcup_{n \geq 1} \mu_n(K)$ と $\mu_n(K) \subset \mu_m(K)$ があります。 単位元 $\zeta$ のすべての根に対して、$\zeta$ 属するから $\mu_n(K)$ のような少なくとも整数 $n \geq 1$ が存在します。つまり、群 $K^*$ には $\zeta$ の位数が存在します。

群 $\mu_n(K)$ は、多項式 $X^n - 1$ の根の集合であり、有限位数 $\leq n$ です。 $p$ を K の特性とします。 $p = 0$、または $p \neq 0$ と $n$ が $p$ で割り切れないとき、$X^n - 1$ の導関数 $nX^{n-1}$ は $X^n - 1$ と相対的に素であるため、多項式 $X^n - 1$ は *分離可能* になります。さらに、K が代数的に閉じている場合、$\mu_n(K)$ は、$n$ 元の群になります。

K が非ゼロの特性 $p$ であると仮定し、$r \geq 0$ を整数とします。 K から K への写像 $x \mapsto x^{p^r}$ は単射なので、整数 $n \geq 1$ ごとに $\mu_{np^r}(K) = \mu_n(K)$ が得られます。

体には 1 以外の単位元の n 番目の根が含む存在しないことに注意してください。これは、たとえば、奇数の整数 $n$ に対する素数体 $\mathbf{Q}$ と $\mathbf{F}_p$ の場合に当てはまります。

#### 定理 1 {#alg-v-s11-thm-1 .statement tag=06OG}

※Kの特性指数を$p$、$n > 0$を整数とします。すると、K の単位元の n 番目根の群 $\mu_n(K)$ は巡回であり、その位数割る $n$ です。 K が代数的に閉じており、$n$ が $p$ に対して素数である場合、群 $\mu_n(K)$ は位数 $n$ の巡回です。*

定理の最初の主張は、次のより正確な補題の帰結であることを証明するだけで十分です。

#### 補題 1 {#alg-v-s11-lem-1 .statement tag=06OH}

*G を位数 $m$ の $K^*$ の有限部分群とします。 G は巡回であり、$G = \mu_m(K)$ になります。*

G を Z モジュールと考えます。すべての $x \in G$ に対して $mx = 0$ があるため、G の消滅子は形 $r\mathbf{Z}$ のイデアルであり、ここで整数 $r \geq 1$ 割る $m$ です。したがって、$G \subset \mu_r(K)$ となります。 補題 4 (V、p. 74) に$A = \mathbf{Z}$ と $M = G$ を適用すると、位数 $r$ の G の元 $x$ が存在します。 $G'$ を、$x$ によって生成された G の循環部分群とします。 $G' \subset \mu_r(K)$、カード $(G') = r$、カード $\mu_r(K) \leq r$ があります。したがって、私たちは

G' = μ_r(K) ⊃ G であり、G は位数 r の巡回であるため、μ_r(K) と等しくなります。 G には位数 m があるので、m = r となり、補題が続きます。

#### 命題 2 {#alg-v-s11-prop-2 .statement tag=06OI}

— K を代数的に閉じ、p をその特性指数とします。 群 Q/Z[1/p] 上に μ_∞(K) の同型が存在します。

1/p によって生成された Q の Z[1/p] 部分環、つまり、a ∈ Z および n ≥ 1 の形 a/p^n の有理数数の集合で表しました。したがって、K が標数 0 の場合、Z[1/p] = Z となります。

p ≠ 1 の場合、(v_n) を p で割り切れないすべての整数のうちの真に増加する数列からなるとします。 X = v_1 v_2 ... v_n と置き、単位元の λ_n 番目の根の H_n 群で表します。 H_{n+1} ⊃ H_n および μ_∞(K) = U H_n が得られます。 H_n は位数 X, (Th. 1) の巡回なので、a_n 生成する H_n かつ a_n = α_n^{v_n + 1} となる単位元の根の数列 (a_n) が存在します。

さらに、β_n を 1/λ_n の剰余類 mod Z[1/p] とし、H'_n を β_n によって生成された Q/Z[1/p] の巡回部分群とします。 p ≠ 1 の場合、X は p で割り切れないため、β_n = v_{n+1} β_{n+1} であり、H'_n が位数 λ_n であることは明らかです。 したがって、すべての n ≥ 1 同型に対して φ_n : H_n → H'_n が存在し、その結果、 φ_n(α_n) = β_n となり、 関係 α_n = α_{n+1}^{v_n + 1}、β_n = v_{n+1} β_{n+1}、φ_n+、拡大する φ_n であることを示します。最後に、同型 φ_n を拡張する Q/Z[1/p] 上に μ_∞(K) の一意の同型 φ が存在します。つまり、すべての n ≥ 1 について φ(α_n) = β_n です。

#### 注意 1 {#alg-v-s11-n2-rem-1 .statement tag=06OJ}

K が標数 0 の代数閉体である場合、群 μ_∞(K) は Q/Z と同型 (正準ではない) になります。 *K が複素数の体 C であるとき、次のような明示的な同型を書き留めることができます。つまり、写像 x ↦ e^{2πix} は、Q の準同型を核 Z と像で C* に変換します。 μ_∞(C);したがって、商への通過により、Q/Z の定義する同型は μ_∞(C) になります。*

#### 注意 2 {#alg-v-s11-n2-rem-2 .statement tag=06OK}

次の結果が示される可能性があります (cf. V, p. 165、例 21): G と H を 2 つの可換群とし、そのすべての元は有限位数です。すべての整数 n ≥ 1 について、方程式 nx = 0 が同じ解の数を持ち、G と H で有限であると仮定します。そのとき、群 G と H は同型です。これにより、提案 2 の新しい証明が得られます。

#### 注意 3 {#alg-v-s11-n2-rem-3 .statement tag=06OL}

すべての素数数に対して、μ_{l∞}(K) = U μ_{ln}(K) を置きます。 l が K の標数 p であるとき、μ_{p∞}(K) = {1} となります。 I、p. 80、木曜日から。 4 から、μ_∞(K) は部分群 μ_{l∞}(K) の直和であると推定します。ここで、l は p とは異なるすべての素数数の集合にまたがります。与えられた素数数 l に対して、考えられるケースは 2 つだけです。 μ_{l∞}(K) が有限であり、その後 μ_{l∞}(K) が適切な n (Th. 1) に対して Z/l^nZ と同型であるか、または μ_{l∞}(K) が無限であり、その後 μ_{l∞}(K) が Z[l^{-1}]/Z (cf.) と同型であるかのどちらかです。 注意 2）。

### 3. プリミティブ根/単位元

n ≥ 1 を整数とします。 φ(n) と書かれた n のオイラー指標によって、整数を法とする n の環 Z/nZ の可逆元の数がわかります。次の命題 $\varphi(n)$ は、整数 $k$ の数も$n$ に素数となり、$0 \leq k < n$ になります。

#### 命題 3 {#alg-v-s11-prop-3 .statement tag=06OM}

※$k$と$n \geq 1$を2つの整数とします。したがって、次の主張は同等です*:

a) * $k$ mod $n$ の剰余類は、環 $\mathbf{Z}/n\mathbf{Z}$ で反転可能です。*
b) *$k$ mod $n$ 生成するの *剰余類 、循環群 $\mathbf{Z}/n\mathbf{Z}$;*
c) *整数 $k$ と $n$ は相対的に素* (*I*, p. 112) です。

条件 a) と b) はそれぞれ、$kx \equiv 1 \pmod{n}$ となるような整数 $x$ が存在すること、つまり $kx + ny = 1$ となるような 2 つの整数 $x$ と $y$ が存在することを意味します。この後者の条件は、$k$ と $n$ が相対的に素であることを意味します。

#### 系 1 {#alg-v-s11-prop-3-cor-1 .statement tag=06ON}

*$G$ を位数 $n$ の循環群とし、$d$ を $n$ の因子とします。すると、$G$ の位数 $d$ の元の数は $\varphi(d)$ に等しくなります。特に、$\varphi(n)$ は $G$ の生成元の数です。*

$G$ は $\mathbf{Z}/n\mathbf{Z}$ と同型であるため、$G$ の生成元の数は、提案 3 により $\varphi(n)$ と等しくなります。 Let $g$ be a generator of $G$; then the elements $h$ of $G$ such that $h^d = 1$ constitute the subgroup $H$ of $G$ generated by $g^{n/d}$; this group is cyclic of order $d$ and the elements of order $d$ of $G$ are the generators of $H$, hence their number is $\varphi(d)$.

#### 系 2 {#alg-v-s11-prop-3-cor-2 .statement tag=06OO}

*整数 $n \geq 1$ ごとに、*
$$
\sum_{d \mid n} \varphi(d) = n,
$$
*ここで、整数 $d$ は、因子の集合 > $n$* ^1 の 0 を超えます。

With the notation of Cor. 1, every element of $G$ has a finite order which is a divisor $d$ of $n$ and for a fixed $d$ there are $\varphi(d)$ such elements.

$\varphi(n)$ の計算は 2 つの式に基づいています。

(2) $\varphi(mn) = \varphi(m)\varphi(n)$ $m$ と $n$ が互いに素である場合、
(3) $\varphi(p^a) = p^{a-1}(p-1)$ ($p$ 素数、$a \geq 1$)。

最初の結果は、環 $\mathbf{Z}/mn\mathbf{Z}$ と $(\mathbf{Z}/m\mathbf{Z}) \times (\mathbf{Z}/n\mathbf{Z})$ が同型 (*I*, p. 112) であり、2 つの環 $A$ と $B$ に対して $(A \times B)^* = A^* \times B^*$ であるという事実からすぐに得られます。 (3) を証明するには、$p^a$ の正の因子が $1, p, p^2, \ldots, p^a$ であることに注意します。したがって、整数 $k$ は、$p$ で割り切れない場合に限り、$1$ 以外に $p^a$ を伴う共通の因子を持ちません。 $0$ と $p^a - 1$ の間には $p$ の $p^a - 1$ 倍数があるので、確かに (3) が見つかります。

式 (2) と (3) は次のことをすぐに示します。
$$
\varphi(n) = n \prod_p (1 - 1/p),
$$
ここで、$p$ は、$n$ の素数因子の集合を超えます。

^1 関係 $d \mid n$ 整数 > 0 の間は、« d 割る n » (VI, p. 5) を意味します。

単位元の n 番目の根が位数 $n$ の場合、原始的であると言われます。このような根 $\zeta$ が存在する場合、群 $\mu_n(K)$ は位数 $n$ であり、$\zeta$ によって生成されます。 \* たとえば、$\mathbf{C}$ の単位元の原始 n 番目根は、$0 \leq k < n$ と $k$ が $n$ に素数である数 $e^{2\pi i k / n}$ です。 \* コル。提案 3 の 1 は、次の結果を意味します。

#### 命題 4 {#alg-v-s11-prop-4 .statement tag=06OP}

— $n \geq 1$ を整数とします。 K に単位元の n 番目の根が存在するとします (これは、たとえば K が分離可能に閉じていて $n . 1, \neq 0$ の場合に当てはまります)。すると、K の単位元の原始 n 番目根の数は $\varphi(n)$ に等しくなります。

### 4. 環状分節拡大

$p$ を K の特性指数とし、$n \geq 1$ を整数と $p$ の素数とする。 K 上のレベル $n$ の円分拡大によって、K 上の多項式 $X^n - 1$ の任意の分裂拡大 E がわかります (V, p. 21)。この多項式は可分であるため、E は K のガロア拡大、有限次数 (V, p. 57) です。 E には単位元の原始 n 番目の根が存在します。 $\zeta$ が根である場合、単位元の n 番目の根は $\zeta$ の冪であるため、$E = K(\zeta)$ になります。

この番号の残りについては、K の選ぶ分離閉包 $K_s$ とします。すべての $n \geq 1$ について、$p$ 群 $\mu_n(K_s)$ は、位数 $n$ および体の巡回です。

$$
R_n(K) = K(\mu_n(K_s))
$$

は K のレベル $n$ の円分値拡大です。 $\mu_n(K_s)$ は、環 $\mathbf{Z}/n\mathbf{Z}$ 上の階数 1 の自由加群と、$\mu_n(K_s)$ の $\mathrm{Gal}(K_s/K)$ 誘導する自己同型のすべての元 $a$ と考えることができます。したがって、$K_s$ の単位元 $\zeta$ の n 番目の根ごと、$\mathrm{Gal}(K_s/K)$ のすべての $u$ 、およびすべての整数に対して、公式 $u(\zeta) = \zeta^j$ によって特徴付けられる準同型 $\chi_n : \mathrm{Gal}(K_s/K) \to (\mathbf{Z}/n\mathbf{Z})^*$ が存在します。 $j$ で剰余類 $\chi_n(u)$ モッド $n$。 $R_n(K) = K(\mu_n(K_s))$ なので、$\chi_n$ の核は $\mathrm{Gal}(K_s/K)$ の部分群 $\mathrm{Gal}(K_s/R_n(K))$ です。したがって、$\chi_n = \varphi_n \circ \psi_n$ があり、$\psi_n$ は $\mathrm{Gal}(R_n(K)/K)$ 上の $\mathrm{Gal}(K_s/K)$ の制限準同型であり、$\varphi_n$ は $(\mathbf{Z}/n\mathbf{Z})^*$ の $\mathrm{Gal}(R_n(K)/K)$ の単射準同型です。 特に次のような結果が得られます。

#### 命題 5 {#alg-v-s11-prop-5 .statement tag=06OQ}

— K の $p$ 拡大 $R_n(K)$ のすべての整数 $n \geq 1$ 素数は有限次数のアーベルであり、そのガロア群は $(\mathbf{Z}/n\mathbf{Z})^*$ の部分群およびその次数と同型です。 割る位数 $\varphi(n)$/$(\mathbf{Z}/n\mathbf{Z})^*$。

Q を有理数数の体 Q の代数閉包とし、n を整数とします。次に、レベル $n$ の円分多項式 $\Phi_n$ は次のように定義されます。

$$
\Phi_n(X) = \prod_{\zeta \in S_n} (X - \zeta),
$$

ここで、$S_n$ は、$Q$ の単位元の原始 n 番目根の集合です。多項式 $\Phi_n$ は次数 $\varphi(n)$ です (提案 4)。 $\Phi_n(X)$ が $\bar{\mathbf{Q}}$ のすべての自己同型の下で不変であることは明らかであり、したがって属するから $\mathbf{Q}[X]$ も不変です。 $S_n$ のすべての元 $\zeta$ は多項式 $X^n - 1$ の根であるため、多項式 $\Phi_n(X)$ 割る $X^n - 1$ と次の補題は、$\Phi_n(X)$ がモニック多項式であることを示しています整数係数と。

#### 補題 2 {#alg-v-s11-lem-2 .statement tag=06OR}

*f、g、h を $f = gh$ となるような $\mathbf{Q}[X]$ のモニック多項式とする。 f に整数係数がある場合、g と h にも同じことが当てはまります。*

$a$ (それぞれ $b$) を、$\alpha g$ (それぞれ $\beta h$) が整数係数となるように、整数 $\alpha \geq 3$ (それぞれ $\beta \geq 1$) の最小値とします。 $g' = ag$ と $h' = bh$ を入れて、 *不条理な還元* によって $a = b = 1$ を示します。そうでない場合は、$ab$ の素数因子 $p$ が存在することになります。 $u \in \mathbf{Z}[X]$の場合、$u$の係数の縮小mod$p$で得られる体$\mathbf{F}_p$の係数の多項式を$\bar{u}$と書きましょう。 $g'h' = abf$、よって $\bar{g}'\bar{h}' = 0$ があります。 環 $\mathbf{F}_p[X]$ は整域 (IV、p. 9、提案 8) なので、$\bar{g}' = 0$ または $\bar{h}' = 0$ になります。他の語、$p$ 割るでは、$g'$ のすべての係数、または $h'$ とこの矛盾する仮定のすべての係数。

関係があります

$$
X^n - 1 = \prod_{d|n} \Phi_d(X) .
$$

というのは、$\mu_n(\mathbf{Q})$の$n$形分割を$d$で割ると、$X^n - 1 = \prod_{\zeta \in \mu_n(\mathbf{Q})} (X - \zeta)$と集合$S_d$が得られます。

公式 (6) 決定する $\Phi_n(X)$ $n$ のすべての因子 $d < n$ について $\Phi_d(X)$ がわかるとき。 $\Phi_1(X) = X - 1$ 以降、$\Phi_n$ を計算するための再帰的手順が必要になります。たとえば、素数 $p$ の場合、次のようになります。

$$
X^p - 1 = (X - 1)\Phi_p(X) ,
$$

よって

$$
\Phi_p(X) = X^{p-1} + X^{p-2} + \cdots + X + 1 ,
$$

そして

$$
\Phi_{p^r+1}(X) = \Phi_p(X^{p^r}) \quad \text{for} \quad r \geq 0 .
$$

$1 \leq n \leq 12$ に対する多項式 $\Phi_n(X)$ の値をリストしてみましょう。

$$
\begin{align*}
\Phi_1(X) &= X - 1 \\
\Phi_2(X) &= X + 1 \\
\Phi_3(X) &= X^2 + X + 1 \\
\Phi_4(X) &= X^2 + 1 \\
\Phi_5(X) &= X^4 + X^3 + X^2 + X + 1 \\
\end{align*}
$$

$$
\Phi_6(X) = X^2 - X + 1
$$
$$
\Phi_7(X) = X^6 + X^5 + X^4 + X^3 + X^2 + X + 1
$$
$$
\Phi_8(X) = X^4 + 1
$$
$$
\Phi_9(X) = X^6 + X^3 + 1
$$
$$
\Phi_{10}(X) = X^4 - X^3 + X^2 - X + 1
$$
$$
\Phi_{11}(X) = X^{10} + X^9 + X^8 + X^7 + X^6 + X^5 + X^4 + X^3 + X^2 + X + 1
$$
$$
\Phi_{12}(X) = X^4 - X^2 + 1
$$

$\Phi_1, \Phi_2, \Phi_3, \Phi_4, \Phi_5, \Phi_7, \Phi_8, \Phi_9$ および $\Phi_{11}$ の値は (7) から直接続きます。今は$\Phi_1 \Phi_2 \Phi_3 \Phi_6 = X^6 - 1$と$\Phi_1 \Phi_2 \Phi_3 \Phi_4 \Phi_6 \Phi_{12} = X^{12} - 1$、よって$\Phi_4 \Phi_{12} = \frac{X^{12} - 1}{X^6 - 1} - X^6 + 1$、そして最後に$\Phi_{12} = \frac{X^6 + 1}{X^2 + 1} = X^4 - X^2 + 1$です。ケース $n = 6$ と $n = 10$ も同様に処理できます。

#### 注意 {#alg-v-s11-n4-rem-1 .statement tag=06OS}

\* すべての整数 $n > 0$ 写像 $\mu(n)$ は次のように定義されます: $n$ が素数数の平方で割り切れる場合、$\mu(n) = 0$ を置き、それ以外の場合、$n$ が素数積の場合、$\mu(n) = (-1)^h$ を置きます。 $h$ 別個の素数数 (« メビウス写像 »)。ということが示されるかもしれない

$$
\Phi_n(X) = \prod_{d|n} (X^{n/d} - 1)^{\mu(d)},
$$

またはもっと明示的に

$$
\Phi_n(X) = \prod_{p_1 < \ldots < p_h} (X^{n/p_1 \cdots p_h} - 1)^{(-1)^h}
$$

ここで、$(p_1, \ldots, p_h)$ は、$n$ の素数因子のすべての真に増加する数列の集合にまたがります (cf. 嘘、II、p. 207、例 1)。

### 5. 円分多項式の既約性

$p$ を $K$ の特性指数とし、$n$ を整数プライムトップとします。 $\mathbf{Z}[X]$ の一意な準同型を $K[X]$ に、写像 $X$ から $X$ までを整数係数 $\Phi_n$ とする多項式の $\Phi_n \in K[X]$ 像で表します。

#### 補題 3 {#alg-v-s11-lem-3 .statement tag=06OT}

*$K_s$の$\Phi_n$の根は、単位元の$n$番目の根です。

$K_s$の$\Phi_n$の根の$S$、集合で表します。 公式 (6) により、集合 $\mu_n(K_s)$ は、$d$ を$n$ で割った$S_d$ の和集合になります。 単位元のすべてのプリミティブ $n$ 番目の根したがって、属するから $S_n$ および補題は、提案 4 (V、p. 81) に従います。

#### 命題 6 {#alg-v-s11-prop-6 .statement tag=06OU}

— $p$ を $K$ の特性指数とし、$n \geq 1$ を $p$ の素数整数とします。多項式 $\Phi_n(X)$ が $K[X]$ で既約であるためには、 準同型 $\chi_n : \mathrm{Gal}(K_s/K) \to (\mathbf{Z}/n\mathbf{Z})^*$ が全射であることが必要かつ十分です。

補題 3 までに、$\Phi_n(X)$ の各根 $\zeta$ に対して $R_n(K) = K(\zeta)$ が得られるため、$\Phi_n(X)$ の次数 $\varphi(n)$ が等しい場合に限り、$K[X]$ で $\Phi_n(X)$ は既約です。 $[R_n(K):K]$。さらに、$K$ 上の $R_n(K)$ のガロア群は位数 $[R_n(K):K]$ であり、$\chi_n$ の像である $(\mathbf{Z}/n\mathbf{Z})^*$ の部分群と同型です。さて、提案 6 は、$(\mathbf{Z}/n\mathbf{Z})^*$ が位数 $\varphi(n)$ であるという事実から導き出されます。

#### 定理 2 (ガウス) {#alg-v-s11-thm-2 .statement tag=06OV}

— $Q$ を $Q$ の代数閉包とし、$n \geq 1$ を整数とします。

a) 円分多項式 $\Phi_n(X)$ は $Q[X]$ で既約です。

b) $Q$ 上の $R_n(Q)$ の次数は $\varphi(n)$ です。

c) The homomorphism $\chi_n$ of $\mathrm{Gal}(\bar{Q}/Q)$ into $(\mathbf{Z}/n\mathbf{Z})^*$ is surjective and defines by passage to quotients an isomorphism of $\mathrm{Gal}(R_n(Q)/Q)$ onto $(\mathbf{Z}/n\mathbf{Z})^*$.

提案 6 を考慮すると、c) を証明するだけで済みます。 $n$ までのすべての整数 $r$ 素数は、数 $p_1, \ldots, p_s$ の積であり、$n$ を割りません。したがって、すべての素数数 $p$ が $n$, 写像 $x \mapsto x^p$ の $\mu_n(Q)$ をそれ自体拡大するから $R_n(Q)$ の自己同型に分割しないことを示すだけで十分です。 $\zeta$ が単位元の $n$ 番目の根の原始関数である場合、$\zeta$ 上の$Q$ の最小多項式 $f$ は、$\zeta^p$ の最小多項式 $g$ に等しいことを証明すれば十分です。 $Q$以上。

$f \neq g$ と仮定して矛盾して議論します。多項式 $f$ と $g$ は $Q[X]$ と割る $X^n - 1$ でモニック既約であるため、 $X^n - 1 = fg u$ となるような $u \in Q[X]$ が存在します (IV, p. 13, 提案 13)。 補題 2 (V, p. 82) は、$f, g$ と $u$ が整数係数であることを示します。多項式$v \in \mathbf{Z}[X]$からリダクションmod$p$によって得られた$\mathbf{F}_p$の係数の多項式を$\bar{v}$で表すことにします。したがって、$\mathbf{F}_p[X]$には$X^n - 1 = \bar{f} \bar{g} \bar{u}$が入ります。

さらに$g(\zeta^p) = 0$があるので、$g(X^p)$は$\mathbf{Q}[X]$の$f(X)$の倍数になります。 補題 2 までに、$g(X^p) = f(X) \cdot h(X)$ となるような $h \in \mathbf{Z}[X]$ が存在します。これで、すべての多項式 $v \in \mathbf{F}_p[X]$ に対して $v(X^p) = v(X)^p$ が得られます。削減mod $p$により、$\bar{g}^p = \bar{f} \bar{h}$が得られます。 $v$ が $\mathbf{F}_p[X]$ を $\bar{f}$ で割る既約多項式である場合、割る $\bar{g}$ でなければなりません。 $\bar{f} \bar{g}$ 割る $X^n - 1$ なので、$\mathbf{F}_p[X]$ では $v^2$ 割る $X^n - 1$ が結論するになります。多項式 $X^n - 1$ は $\mathbf{F}_p[X]$ で分離可能であるため、これは不合理です。

$Q$ 上の有限次数のすべてのアーベル拡大 $E$ に対して、$E$ が $R_n(Q)$ の部分拡張と同型であるような整数 $n \geq 1$ が存在することが示されるかもしれません。 \* その他の語、体 $Q(\mu_{\infty}(C))$は、$Q$のアーベルのクロージャです。 *(« クロネッカー・ウェーバー 定理 »)。

### 6. サイクリック拡大

#### 定義 3 {#alg-v-s11-def-3 .statement tag=06OW}

— *拡大 E がガロアであり、そのガロア群が巡回である場合、K の E は巡回であると言われます。*

#### 例 {#alg-v-s11-n6-exa-1 .statement tag=0DI2}

*1) 素数位数 $p$ のすべての有限群 G が巡回であるため、素数次数のすべてのガロア拡大は巡回です (G のすべての元 $x \neq 1$ は位数 $p$ であるため、生成する G)。

2) $F(X) = X^2 + aX + b$ を $K[X]$ の既約多項式とします。 $F(X)$ が分離できない唯一のケースは、$K$ が特性 2 と $a = 0$ である場合です。この件は脇に置きます。 E を、$F(X)$ の根 $x$ によって生成された K の拡大とします。 $[E : K] = 2$ と $F(X) = (X - x)(X + a + x)$ があるため、E は K のガロア拡大です。K 上の E のガロア群は位数 2 であり、したがって循環です。

3) $\mathbf{F}$ を有限位数の体と $\sigma$ 自己同型とします。 $\sigma$ の不変量の体 E は、$\sigma$ によって生成された位数 $n$ の循環群の不変量の体でもあり、したがって (V, p. 66, Th. 3) F は循環拡大の次数 $n$ の E.

私たちは (I、p. 50)、循環群のすべての *部分群* とすべての *剰余群* が循環であることを知っています。したがって (V, p. 68, Cor. 4)、E が次数 $n$ の体 K の巡回拡大である場合、E のすべての部分拡張 F は K* 上で *巡回であり、*E は F* 上で巡回です。 $n$ のすべての因子 d に対して、E に含まれる K 上の次数 d の一意の部分体 F が存在します。なぜなら、位数 $n$ の循環群には、添字 d の一意の部分群が存在します。

#### 定理 3 (*ヒルベルト*) {#alg-v-s11-thm-3 .statement tag=06OX}

— *E を K の循環拡大とし、a を K 上の E のガロア群 $\Gamma$ の生成元とします。

a) 元 $x \in E$ から満たす $N_{E/K}(x) = 1$ については、$x = y / \sigma(y)$ となるように $y \in E^*$ が存在することが必要かつ十分です。 $x = y_1 / \sigma(y_1)$ を持つすべての $y_1 \in E^*$ は、$\lambda \in K^*$ である形 $\lambda y$ になります。

b) 元 $x \in E$ から満たす $\mathrm{Tr}_{E/K}(x) = 0$ については、$z \in E$ が $x = z - \sigma(z)$ とともに存在することが必要かつ十分です。その場合、$x = z_1 - \sigma(z_1)$ を持つすべての $z_1 \in E$ は形 $z + \mu$ であり、$\mu \in K$ です。

まずは補題を証明しましょう。*

#### 補題 4 {#alg-v-s11-lem-4 .statement tag=06OY}

*$\Gamma$ を、位数 $n$ の巡回群、$\sigma$ 生成元の $\Gamma$、および M を可換群とし、$\Gamma$ はすべての規則 $\gamma . (m + m') = \gamma . m + \gamma . m'$ に従って動作します。 $\gamma \in \Gamma$と$m, m' \in M$。 Z を $\Gamma$ のすべての写像の集合を M 満たす関係* にするとします

$$
f(\tau \tau') = f(\tau) + \tau . f(\tau') \quad \text{for } \tau, \tau' \text{ in } \Gamma
$$

$f \in Z$には$u(f) = f(a)$を、$m \in M$には$t(m) = \sum_{\tau \in \Gamma} \tau . m$を入れます。それから数列

$$
0 \to Z \xrightarrow{u} M \xrightarrow{t} M
$$

正確です。

$f \in \mathbf{Z}$ にしましょう。 (10) で $\tau = \tau' = 1$ を取ると、$f(1) = 0$ がわかります。さらに、$m \geqslant 0$の帰納法までに関係と推定されます。

$$
f(\sigma^m) = f(\sigma) + \sigma \cdot f(\sigma) + \cdots + \sigma^{m-2} \cdot f(\sigma) + \sigma^{m-1} \cdot f(\sigma)
$$

$\sigma^n = 1$、よって $f(\sigma^n) = 0$ があります。先行する関係と $m = n$ は、等式 $t(u(f)) = 0$、よって $\operatorname{Im}\ u \subset \operatorname{Ker}\ t$ と同等です。さらに、(11) より、$\operatorname{Ker}\ u = 0$ となります。

$m \in M$ を $t(m) = 0$、つまり $m + \sigma \cdot m + \cdots + \sigma^{n-1} \cdot m = 0$ となるようにします。 $\Gamma$ の定義する写像 $f$ を $M$ にしましょう

$$
f(\sigma^j) = m + \sigma \cdot m + \cdots + \sigma^{j-2} \cdot m + \sigma^{j-1} \cdot m
$$

$0 \leqslant j \leqslant n - 1$の場合。 関係 (10) を確立するのは読者に委ねられるかもしれません。明らかに $m = f(a)$、よって $\operatorname{Im}\ u \supset \operatorname{Ker}\ t$ があります。

補題が証明されたので、$y \in E^*$ と $x = y/\sigma(y)$ を考えてみましょう。 $N_{E/K}(\sigma(y)) = N_{E/K}(y)$、よって $N_{E/K}(x) = 1$があります。逆に、$E^*$ の $x$ が $N_{E/K}(x) = 1$ になるようにします。 補題 4 により、$M = E^*$ に適用されると、$\Gamma$ と $c_\sigma = x$ の $\tau, \tau'$ に対して、$E^*$ 満たす関係 $c_{\tau \tau'} = c_\tau \cdot \tau(c_{\tau'})$ の元 $(c_\tau)_{\tau \in \Gamma}$ のファミリーが存在します。コル著提案 9 の 1 (V、p. 65) $\tau \in \Gamma$、よって、特に $x = c_\sigma = y/\sigma(y)$ に対して、$c_\tau = y/\tau(y)$ を伴う $y \in E^*$ が存在します。 $y_1 \in E^*$ が $x = y_1/\sigma(y_1)$ を満たす場合、次のようになります。

$$
\sigma(y_1 y^{-1}) = y_1 y^{-1},
$$

したがって、$y_1 y^{-1}$ 属するから $K^*$ になります。なぜなら、$E$ の $a$ 生成するガロア群が $K$ を超えるからです。これは a) を証明します。

主張 b) は Cor から同様の方法で続きます。提案 9 の 2 (V、p. 65)。

### 7. $\mathbf{Z}/n\mathbf{Z}$ モジュールの二重性

この番号では、$n$ 整数 $> 0$ と、位数 $n$ の循環群を $T$ で表します。 群 $G$ は、すべての $g \in G$ に対して $g^n = 1$ であれば、$n$ によって消滅するといわれています。さらに、$G$ が可換である場合、$G$ の群構造は固有の $\mathbf{Z}/n\mathbf{Z}$ モジュール構造の基礎となります。

すべての群 $G$ を、$G$ の準同型の $\operatorname{Hom}(G, T)$ 群を$T$ に表します。それは可換群が $n$ によって消滅するものです。

#### 命題 7 {#alg-v-s11-prop-7 .statement tag=06OZ}

— $G$ を、$G$ の $n$ と $H$ 部分群によって消滅される可換群とします。すると、制限準同型 $\operatorname{Hom}(G, T) \to \operatorname{Hom}(H, T)$ は全射になります。

$f : H \to T$ を準同型とします。 $f$を拡張する$T$に$G$の準同型が存在することを証明します。まず、$G$ が巡回であり、位数 $r$ の元 $g$ を $n$ で割ることによって生成されると仮定します。 $T$ の $t$ 生成元で表します。 H が $g^s$ (I, p. 50, 提案 19) によって生成されるような r の因子が存在し、すべての $x \in \mathbf{Z}$ に対して $f(g^{sx}) = t^{ax}$ が得られます。ここで、a は整数で、n 割る $ar/s$ となります。すると、$a/s = (ar/ns)(n/r)$ は、G の整数と準同型 $g^x \mapsto t^{(a/s)x}$、$x \in \mathbf{Z}$ を T 拡大する f に変換します。一般的なケースでは、対 $(H', f')$ の集合を考えます。ここで、$H'$ は G 含む H の部分群で、$f'$ は $f$ を延長した T の $H'$ の準同型です。 $f''$から$H'$までの$H' \subset H''$と制限が$f'$であれば、関係$(H', f') \leq (H'', f'')$により位数この集合になります。 集合理論、III、p. 154、定義により。 3とTh。 2、この集合には極大元 $(H_1, f_1)$ があり、$H_1 = G$ であることを証明するのに十分です。そうでない場合、$g \in G, g \notin H_1$ が存在し、$f_1$ が $H_1$ と g によって生成された G の部分群の準同型 T に拡張できることを証明するだけで十分です。ここで、C が g によって生成された循環群を表す場合、$f_1$ の制限から $C \cap H_1$ 拡大するから準同型 C の $f_2$ が T と準同型に変換されます。 T に$H_1C$ の $xy \mapsto f_1(x) f_2(y), x \in H_1, y \in C,$ が希望の写像です。

#### 系 1 {#alg-v-s11-prop-7-cor-1 .statement tag=06P0}

— G が *n* によって消滅する可換群であり、$G \neq \{1\}$ である場合、$\mathrm{Hom}(G, T) \neq \{1\}$。

H が $\{1\}$ とは異なる G の循環部分群である場合、$\mathrm{Hom}(H, T) \neq \{1\}$ であることに注意し、提案 7 を適用するだけで十分だからです。

#### 系 2 {#alg-v-s11-prop-7-cor-2 .statement tag=06P1}

— G が *n* によって消滅した *有限* 可換群である場合、 群 G と $\mathrm{Hom}(G, T)$ は同じ位数を持ちます。

G が生成元 g を伴う位数 *r* の巡回である場合、写像 $f \mapsto f(g)$ は、T の元 t の集合に $\mathrm{Hom}(G, T)$ の全単射が加わり、$t^r = 1$ となるため、この場合、主張が続きます。一方、H が G の循環部分群である場合、$\mathrm{Card}(G) = \mathrm{Card}(H) \cdot \mathrm{Card}(G/H)$ になります。さらに、完全系列があります

$$
\{1\} \to \mathrm{Hom}(G/H, T) \to \mathrm{Hom}(G, T) \to \mathrm{Hom}(H, T) \to \{1\}
$$

(II、p. 227、上記の第 1 条および提案 7)、したがって

$$
\mathrm{Card}(\mathrm{Hom}(G, T)) = \mathrm{Card}(\mathrm{Hom}(H, T)) \cdot \mathrm{Card}(\mathrm{Hom}(G/H, T)).
$$

$\mathrm{Card}(\mathrm{Hom}(H, T)) = \mathrm{Card}(H)$ なので、G または $G/H$ の系を証明することは同じになります。結果は $\mathrm{Card}(G)$ の帰納法と続きます。

ここで、G と H を 2 つの群と $f : G \times H \to T$ の双乗法写像とします。つまり、任意の $g, g' \in G, h, h' \in H$ について次のようになります。

$$
f(gg', h) = f(g, h) f(g', h), \quad f(g, hh') = f(g, h) f(g, h')
$$

私たち定義する群準同型

$$
s_f : G \to \mathrm{Hom}(H, T), \quad d_f : H \to \mathrm{Hom}(G, T),
$$

$s_f(g)(h) = d_f(h)(g) = f(g, h)$ による (cf. II, p. 268、提案 1 に対する修正、G と H が可換である場合)。

#### 命題 8 {#alg-v-s11-prop-8 .statement tag=06P2}

— *G と H が可換であり、n によって消滅するとします。 s_f が全単射で H が有限の場合、d_f は全単射で Card(G) = Card(H) となります。*

s_f が全単射であり、H が有限である場合、Cor によって次のようになります。 2 から提案 7 関係 Card(G) = Card(Hom(H, T)) = Card(H)、したがって Card(G) は有限であり、他の系の適用により、Card(Hom(G, T)) = Card(H) となります。したがって、d_f が単射であることを証明すれば十分です。ここで、h \in \mathrm{Ker}(d_f) の場合、G \in のすべての g に対して f(g, h) = 1 になります。したがって、s_f は全単射なので、すべての \varphi \in \mathrm{Hom}(H, T) に対して \varphi(h) = 1 になります。提案 7 によれば、これは \mathrm{Hom}(\mathrm{Ker}(d_f), T) = \{1\} を意味します。したがって、Cor による \mathrm{Ker}(d_f) = \{1\} となります。 1から提案7まで。

### 8. クンメル理論

この番号では、$n$ 整数 > 0 で表し、$\mu_n(K)$ には $n$ 元があると仮定します。 by V, p. 78 this means also that $n$ is prime to the characteristic 指数 of K and that all the n-th 根 of 単位元 in 代数閉包 $\Omega$ of K lie in K.

K の拡大 L は、アーベル (V, p. 77, Def. 1) であり、そのガロア群 Gal(L/K) が $n$ によって消滅される場合、n* を除算した指数の *アーベルであると言えます。 (V、p. 86)。

A を $K^*$ の部分集合とします。 $\theta^n \in A$ のように、すべての $0 \in \Omega$ によって生成された $\Omega$ の部分拡張を $K(A^{1/n})$ で表します。

#### 補題 5 {#alg-v-s11-lem-5 .statement tag=06P3}

— *$K(A^{1/n})$ は、n を割った指数の K のアーベル拡大です。

多項式 $X^n - a, a \in A$ は K 上で可分であるため、$L = K(A^{1/n})$ は可分であり、したがって K のガロア拡大です。$\sigma \in \mathrm{Gal}(L/K)$ と $0 \in \Omega$ を $\theta^n \in A$ となるようにします。 $\sigma(\theta)^n = \theta^n$ があります。したがって、$\sigma(\theta) = \zeta \theta$ となるような $\zeta \in \mu_n(\Omega) = \mu_n(K)$ が存在します。これは、$\sigma^n(\theta) = \zeta^n \theta = 0$、よって $\sigma^n = 1$ を意味します。 $\sigma'$ が $\mathrm{Gal}(L/K)$ の他の元である場合、$\sigma'(\theta) = \zeta' \theta$、よって $\sigma'\sigma(\theta) = \zeta \zeta' \theta = \sigma\sigma'(\theta)$、そして$\sigma'\sigma = \sigma\sigma'$ となるような $\zeta' \in \mu_n(K)$ が存在します。

#### 補題 6 {#alg-v-s11-lem-6 .statement tag=06P4}

— *LをKのガロア拡大とします。 There exists a unique mapping $(\sigma, a) \mapsto \langle \sigma, a \rangle$ of $\mathrm{Gal}(L/K) \times ((L^n \cap K^*)/K^{*n})$ into $\mu_n(K)$ such that for every $\sigma \in \mathrm{Gal}(L/K)$ and every element $0 \in L^*$ such that $\theta^n \in K$ we have, on denoting by $\overline{\theta^n}$ the residue class of $\theta^n$ mod $K^{*n}$:*

$$
\langle \sigma, \overline{\theta^n} \rangle = \sigma(\theta)/\theta
$$

*この写像は倍乗法です。*

実際には、(13) の右辺は、$\theta^n$ の剰余類 mod $K^{*n}$ にのみ依存する単位元の n 番目の根です。これは最初の主張を証明します。 2番目の主張は問題なく検証されます。

K のすべてのガロア拡大 L について、次のように書きましょう

$$
k_L : (L^n \cap K^*)/K^{*n} \to \mathrm{Hom}(\mathrm{Gal}(L/K), \mu_n(K)) ,
$$
$$
k'_L : \mathrm{Gal}(L/K) \to \mathrm{Hom}((L^n \cap K^*)/K^{*n}, \mu_n(K)) ,
$$

準同型は上記の双乗法写像 (V, p. 87) から導出されます。

#### 命題 9 {#alg-v-s11-prop-9 .statement tag=06P5}

*K の有限次数 L のすべてのガロア拡大について、準同型 $k_L$ は全単射です。*

$0 \in L^*$ を、$0^n \mod K^{*n}$ 属するから $k_L$ の核の $0^n \in K$ と剰余類とする。 $\sigma \in \mathrm{Gal}(L/K)$ ごとに、定義 $\sigma(\theta) = 0$ までに時間がかかります。したがって、$0 \in K^*$ と $\theta^n \in K^{*n}$ です。これは$k_L$の単射性を証明します。ここで、$f : \mathrm{Gal}(L/K) \to \mu_n(K)$ を準同型とします。 $\sigma, \tau \in \mathrm{Gal}(L/K)$ 全員のために

$$
f(\sigma \tau) = f(\sigma) f(\tau) = f(\sigma) \cdot \sigma f(\tau) , \quad f(\sigma)^n = 1 .
$$

V、p. 65、Cor. 1 すべての $\sigma \in \mathrm{Gal}(L/K)$ に対して $f(\sigma) = \sigma(\theta)/\theta$ となるような $0 \in L^*$ が存在します。 $f(\sigma)^n = 1$ から、すべての $\sigma \in \mathrm{Gal}(L/K)$ に対して $\sigma(\theta^n) = 0^n$ があり、したがって $0^n \in K^*$ になります。 $a$ が $\theta^n \mod K^{*n}$ の剰余類である場合、$\sigma \in \mathrm{Gal}(L/K)$ は定義 $f(\sigma) = \langle \sigma, a \rangle$ までにあるため、$f = k_L(a)$ になります。

#### 系 {#alg-v-s11-n8-cor-1 .statement tag=06P6}

*LがKのガロア拡大である場合、準同型$k_L$は単射であり、その像は位相群$\mathrm{Gal}(L/K)$の離散群への連続準同型の群$\mathrm{Hom}_c(\mathrm{Gal}(L/K), \mu_n(K))$となる$\mu_n(K)$.*

これは、L がガロア拡大の和集合 $L_i$ の有限次数に向けられた増加するであり、$\mathrm{Gal}(L/K)$ の $\mu_n(K)$ への準同型が連続であるという事実を利用して、これまでに述べたことから直ちに帰結します。 商 $\mathrm{Gal}(L_i/K)$/$\mathrm{Gal}(L/K)$。

#### 定理 4 {#alg-v-s11-thm-4 .statement tag=06P7}

*a) The mapping $H \mapsto K(H^{1/n})$ is an inclusion preserving bijection of the set of subgroups of $K^*$ containing $K^{*n}$ onto the set of abelian subextensions of exponent dividing n of $\Omega$. 写像の逆数は$L \mapsto L'' \cap K^*$です。

b) $K^*$ 含む $K^{*n}$ 準同型の部分群 H ごとに

$$
k' : \mathrm{Gal}(K(H^{1/n})/K) \to \mathrm{Hom}(H/K^{*n}, \mu_n(K))
$$

は全単射であり、群 $\mathrm{Hom}(H/K^{*n}, \mu_n(K))$ に単純収束の位相が備わっている場合は同射写像です。

c) H を $K^*$ 含む $K^{*"n}$ の部分群とします。すべての $a \in H/K^{*n}$ について、$\theta_a$ を $\Omega$ の元とし、$\theta_a^n$ が H の a の代表となるようにします。次に、ベクトル K 空間 $K(H^{1/n})$ の $\theta_a, a \in H/K^{*n}$、形基底です。特に、

$$
[K(H^{1/n}):K] = (H:K^{*"n}) .
$$

A) 指数の K を n で割ったアーベル拡大 L ごとに、$H_L = L'' \cap K^*$ を入れましょう。 $[L:K]$ が有限であれば、$\mathrm{Gal}(L/K)$ の $\mathrm{Hom}(H_L, \mu_n(K))$ への準同型 $k'_L$ は、命題 9 とV、p. 88、命題 8 により全単射です。

Since every abelian extension of K of exponent dividing $n$ is an increasing directed union of abelian subextensions of finite degree of exponent dividing $n$, we deduce by passage to inverse limits that $k'_L$ is a homeomorphism of topological groups for every abelian extension L of K dividing n.

B) Let L be an abelian extension of finite degree, of exponent dividing $n$, of K, and let $L' = K(H_L^{1/n})$; this is a subextension of L ; moreover $H_{L'}$ contains $H_L$ and so is equal to it. 準同型 $k'_L$ と $k'_{L'}$ は A) と $H_L = H_{L'}$ により全単射であるため、群 Gal$(L/K)$ と Gal$(L'/K)$ は同じ位数を持ち、等しいです。 これは、$L' = L$、したがって $L = K(H_L^{1/n})$ であることを示しています。 If L is an abelian extension of exponent dividing $n$ of K, we have $K(H_L^{1/n}) = L$, because $K(H_L^{1/n})$ is a subextension of L which contains every subextension of finite degree of L.

C) H を $K^*$ 含む $K^{*n}$ の部分群とします。 $L = K(H^{1/n})$を置くと、指数のKを$n$で割ったアーベル拡大になります（V、p. 88、補題5）。 $H \subset H_L$, よってがあり、$n$ によって消滅した可換群の完全系列が得られます。

$$
\{1\} \to H/K^{*n} \to H_L/K^{*n} \to H_L/H \to \{1\}.
$$

これから、完全系列が得られます。

$$
\{1\} \to \operatorname{Hom}(H_L/H, \mu_n(K)) \to \operatorname{Hom}(H_L/K^{*n}, \mu_n(K)) \xrightarrow{\iota} \operatorname{Hom}(H/K^{*n}, \mu_n(K)),
$$

ここで、$\iota$ は制限準同型です。

同型 $k'_L$ を使って Gal$(L/K)$ を同一視する $\operatorname{Hom}(H_L/K^{*n}, \mu_n(K))$ とすると、$\iota$ の核は $\sigma \in \operatorname{Gal}(L/K)$ の集合と同一視され、すべての $\theta \in H^{1/n}$ に対して $\sigma(\theta) = \theta$ になります。したがって、$\iota$ は単射であるため、$\operatorname{Hom}(H_L/H, \mu_n(K))$ は (1) に還元されます。コル著V、p. 87 の 1 なので、$H = H_L$ になります。これでa)とb)の証明は完了です。

D) c) を証明しましょう。 $a, b \in H$ の場合、$\theta_a \theta_b / \theta_{ab} \in K$ になります。 It follows that the vector subspace of $K(H^{1/n})$ generated by the $\theta_a$ is stable under multiplication and so coincides with $K(H^{1/n})$. $\theta_a$ が線形独立であることを示すだけが残っています。これを行うには、明らかに $H/K^{*n}$ が有限であると仮定することができます。次に b) と Cor による $[K(H^{1/n}) : K] = (\operatorname{Gal}(K(H^{1/n})/K) : \{1\}) = (H : K^{*n})$ V、p. 87 の 2 個。 $\theta_a$ の数は $(H : K^{*n})$ に等しく、それらは生成するベクトル K 空間 $K(H^{1/n})$ であるため、それらは線形独立です。

#### 例 1 {#alg-v-s11-n8-exa-1 .statement tag=06P8}

$\Omega$ に含まれる K の $n$ を除算する指数の最大のアーベル拡大が存在します。これは、すべての元の n 番目の根を K に隣接させることによって取得されます。そのガロア群は $\operatorname{Hom}(K^*/K^{*n}, \mu_n(K))$ と識別される可能性があり、したがって $\operatorname{Hom}(K^*, \mu_n(K))$ とも識別されます。

#### 例 2 {#alg-v-s11-n8-exa-2 .statement tag=06P9}

\* $K = \mathbf{Q}$ と $n = 2$ を考えてみましょう。すると、$\mathbf{Q}^*/\mathbf{Q}^{*2}$ は、$\{-1\}$ の基底和集合とすべての素数数の集合をもつベクトル $\mathbf{F}_2$-空間です。 $\mathbf{C}$ に含まれる Q の 2 の指数の最大のアーベル拡大は、$\mathbf{C}$ の部分体 $\mathbf{Q}(i, \sqrt{2}, \sqrt{3}, \sqrt{5}, \ldots)$ になります。そのガロア群は、元 $i,\ \sqrt{2},\ \sqrt{3},\ \sqrt{5}$ などのそれぞれに $\pm 1$ を乗算して得られるすべての自己同型で構成されます。 \*

#### 例 3 {#alg-v-s11-n8-exa-3 .statement tag=06PA}

L を次数 $n$ の K の巡回拡大とします。この場合、群 $(L^n \cap K^*)/K^{*n}$ は位数 $n$ の循環です。 $a \in K^*$ が、$a$ mod $K^{*n}$ の剰余類がこの群の生成元であるようなものである場合、L は $K[X]/(X^n - a)$ と K 同型であり、群 $\mathrm{Gal}(L/K)$ は、 $n$ 自己同型写像 $X$ ～ $\zeta X$、$\zeta \in \mu_n(K)$。

#### 例 4 {#alg-v-s11-n8-exa-4 .statement tag=06PB}

逆に、$a \in K^*$ と $r$ を最小の整数 $> 0$ とし、$a' \in K^{*n}$ とします。この場合、多項式 $X^n - a$ の根によって生成される $\Omega$ の部分体 $L$ は、次数 $r$ の $K$ の循環拡大です。特に、$X^n - a$ は、$r = n$ の場合にのみ既約です。

#### 注意 {#alg-v-s11-n8-rem-1 .statement tag=06PC}

$a \in K^*$ とし、r を最小の整数 $> 0$ とし、$a' \in K^n$ とします。 B を多項式 $X^{n/r} - a$ の K の根の集合とします。それなら私たちは持っています

$$
X^n - a = \prod_{b \in B} (X' - b),
$$

関係 $T^{n/r} - a = \Pi (T - b)$ の T を $X'$ に置き換えることにより。 例 4 により、各多項式 $X' - b$ は既約であるため、(14) は $X^n - a$ の分解で $K[X]$ の既約多項式になります。

### 9. アルティン・シュライヤー 理論

この番号では、素数数を表すために $p$ を使用し、K が標数 $p$ であると仮定します。 We denote by $\Omega$ an algebraic closure of K and by $\varphi$ the endomorphism of the additive group of $\Omega$ defined by

$$
\varphi(x) = x^p - x.
$$

V により、$\varphi$ の p. 93 核は、$K$ の部分体 $\mathbf{F}_p$ の素数になります。 K のすべての部分集合 $A$ について、$\varphi(x) \in A$ のようにすべての $x \in \Omega$ によって生成された $\Omega$ の部分拡張を $K(\varphi^{-1}(A))$ で表します。

#### 補題 7 {#alg-v-s11-lem-7 .statement tag=06PD}

$K(\varphi^{-1}(A))$は、指数の$K$のアーベル拡大を$p$で割ったものです。

多項式 $\varphi - a = X^p - X - a,\ a \in A$ は $K$ 上で分離可能であるため、拡大 $L = K(\varphi^{-1}(A))$ はガロアです。 $a \in \mathrm{Gal}(L/K)$ と $x \in \varphi^{-1}(A)$ としましょう。 $\varphi(\sigma(x)) = \varphi(x)$ があるため、$\sigma(x) - x \in \mathbf{F}_p$、つまり $\sigma(x) = x + i,\ i \in \mathbf{F}_p$ になります。これは、$\sigma^p(x) = x + pi = x$、つまり $u^p = 1$ を意味します。同様に、$a' \in \mathrm{Gal}(L/K)$ と $\sigma'(x) = x + j$ の場合、$\sigma \circ \sigma'(x) = x + i + j = a' \circ \sigma(x)$ があるため、$\sigma \circ \sigma' = \sigma' \circ \sigma$ になります。

#### 補題 8 {#alg-v-s11-lem-8 .statement tag=06PE}

L を K のガロア拡大とします。 $\mathrm{Gal}(L/K) \times ((\varphi(L) \cap K)/\varphi(K))$ の $\mathbf{F}_p$ に一意な写像 $(\sigma, a) \mapsto [a, a')$ が存在し、すべての $\sigma \in \mathrm{Gal}(L/K)$ とすべての元 $x \in L$ について、$\overline{\varphi(x)}$ で表すと $\varphi(x) \in K$ が得られます。 剰余類の $\varphi(x)$ mod $\varphi(K)$、

$$
[\sigma, \overline{\varphi(x)}] = \sigma(x) - x.
$$

この写像は Z 双線形です ($\sigma, \tau \in \mathrm{Gal}(L/K)$、$a, b \in (\mathscr{P}(L) \cap K)/\mathscr{P}(K)$ の場合、$[\sigma \tau, a) = [\sigma, a) + [\tau, a)$、$[\sigma, a + b) = [\sigma, a) + [a, b)$ があります)。

(15) の右辺は $\mathbf{F}_p$ の元であり、これは $\mathscr{P}(x) \mod \mathscr{P}(K)$ の剰余類のみに依存します。これは最初の主張を証明します。 2 番目は問題なく検証できます。

$K$ のガロア拡大 $L$ ごとに、次のように書きましょう

$$
a_L : (\mathscr{P}(L) \cap K)/\mathscr{P}(K) \to \mathrm{Hom}(\mathrm{Gal}(L/K), \mathbf{F}_p)
$$
$$
a_L' : \mathrm{Gal}(L/K) \to \mathrm{Hom}((\mathscr{P}(L) \cap K)/\mathscr{P}(K), \mathbf{F}_p)
$$

上記の Z 双線形写像 (V, p. 87) から得られる準同型について。

#### 命題 10 {#alg-v-s11-prop-10 .statement tag=06PF}

*$K$ の有限次数のすべてのガロア拡大 $L$ について、準同型 $a_L$ は全単射です。*

$x \in L$ を、$\mathscr{P}(x) \mod \mathscr{P}(K)$ の $\mathscr{P}(x) \in K$ と剰余類が $a_L$ の核にあるようにします。 $\sigma \in \mathrm{Gal}(L/K)$ ごとに、定義 $\sigma(x) = x$ までに時間がかかります。したがって、$x \in K$ と $\mathscr{P}(x) \in \mathscr{P}(K)$ です。これは$a_L$の単射性を証明します。ここで、$f : \mathrm{Gal}(L/K) \to \mathbf{F}_p$ を準同型とします。 $\sigma, \tau \in \mathrm{Gal}(L/K)$ 全員のために

$$
f(\sigma \tau) = f(\sigma) + \sigma(f(\tau)), \quad f(\sigma) \in \mathbf{F}_p.
$$

V、p. 65、Cor. 2 すべての $o \in \mathrm{Gal}(L/K)$ に対して $f(u) = \sigma(x) - x$ となるような $x \in L$ が存在します。 $f(o) \in \mathbf{F}_p$ があるため、$\mathscr{P}(\sigma(x)) = \mathscr{P}(x)$ があり、すべての $a \in \mathrm{Gal}(L/K)$ と $\mathscr{P}(x) \in K$ に対して $\sigma(\mathscr{P}(x)) = \mathscr{P}(x)$ となります。 $a$ が $\mathscr{P}(x) \mod \mathscr{P}(K)$ の剰余類である場合、$f(\sigma) = [\sigma, a)$ があるため、$f = a_L(a)$ になります。

#### 系 {#alg-v-s11-n9-cor-1 .statement tag=06PG}

*$L$が$K$のガロア拡大である場合、準同型$a_L$は単射であり、その像は位相群$\mathrm{Gal}(L/K)$の連続準同型の群$\mathrm{Hom}_c(\mathrm{Gal}(L/K), \mathbf{F}_p)$になります群 $\mathbf{F}_p$.*

これは Cor と同じ方法で証明されます。提案 9、V、p. 89。

#### 定理 5 {#alg-v-s11-thm-5 .statement tag=06PH}

*a) The mapping $A \mapsto K(\mathscr{P}^{-1}(A))$ is a bijection of the set of subgroups of $K$ containing $\mathscr{P}(K)$ onto the set of abelian subextensions of exponent dividing $p$ in $\Omega$. 写像の逆数は$L \mapsto \mathscr{P}(L) \cap K$です。
b) $K$ 含む $\mathscr{P}(K)$、準同型の部分群 $A$ ごとに

$$
a' : \mathrm{Gal}(K(\mathscr{P}^{-1}(A))/K) \to \mathrm{Hom}(A/\mathscr{P}(K), \mathbf{F}_p)
$$

は全単射であり、$\mathrm{Hom}(A/\mathscr{P}(K), \mathbf{F}_p)$ に単純収束の位相が備わっている場合は同同写像です。
c) $A$ を $K$ 含む $\mathscr{P}(K)$ の部分群とし、$B$ をベクトル $\mathbf{F}_p$-スペース $A/\mathscr{P}(K)$ の基底とします。それぞれの $a \in B$ について、$\mathscr{P}(x_a)$ が $A$ の $a$ を表すように、$x_a$ を $\Omega$ の元とします。次に、N^{(B)} 内の a = (\alpha(a)) を持つ単項式 $x^\alpha = \prod_{a \in B} x_a^{\alpha(a)}$ は、ベクトル K 空間 K(\mathfrak{p}^{-1}(A)) の各 a \in B 形基底に対して 0 \leq \alpha(a) < p になります。特に、[K(\mathfrak{p}^{-1}(A)):K] = (A:\mathfrak{p}(K)) があります。

Th. 5もThと同様に証明されます。 4 (V、p. 89) を準用します。

#### 例 1 {#alg-v-s11-n9-exa-1 .statement tag=06PI}

\Omega に含まれる、p を割る指数の K の最大のアーベル拡大が存在します。それは K(B^1(K)) であり、そのガロア群は Horn(K/\mathfrak{p}(K),\mathbf{F}_p) で識別できます。

#### 例 2 {#alg-v-s11-n9-exa-2 .statement tag=06PJ}

L を次数 p の K の循環拡大とします。すると群 (\mathfrak{p}(L) \cap K)/\mathfrak{p}(K) は位数 p の巡回です。 \in K が、mod \mathfrak{p}(K) の剰余類がこの群の生成元であるような場合、L は K[X]/(X^p - X - a) と K 同型です。 ガロア群 Gal(L/K) は、p 自己同型写像 X ～ X + i, i \in \mathbf{F}_p で構成されます。

#### 例 3 {#alg-v-s11-n9-exa-3 .statement tag=06PK}

逆に、\in K - \mathfrak{p}(K) の場合、多項式 X^p - X - a は既約であり、その根によって生成される \Omega の部分体 L は、次数 p の K の循環拡大です。 \in \mathfrak{p}(K) の場合、X^p - X - a = \prod_{a \in \mathfrak{p}^{-1}(a)} (X - \alpha) となります。

### 練習問題 {#alg-v-s11-exercises}

[§ 11 に対して練習問題](exercises/s11/)を参照してください。
