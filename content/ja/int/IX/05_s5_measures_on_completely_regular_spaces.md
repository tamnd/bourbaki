---
book: int
book_title: Integration
chapter: IX
chapter_title: MEASURES ON HAUSDORFF TOPOLOGICAL SPACES
section: 5
section_title: Measures on completely regular spaces
lang: ja
source: int-vii-ix
book_pages: INT IX.56-INT IX.72, INT IX.113-INT IX.117
pdf_pages: 0238-0254, 0295-0299
extraction: ocr
subsections:
    - "no": 1
      title: Measures and bounded continuous functions
      page: 56
      pdf_page: 238
    - "no": 2
      title: Bounded measures and linear forms on $\mathscr{C}^b(T)$
      page: 59
      pdf_page: 241
    - "no": 3
      title: Tight convergence of bounded measures
      page: 60
      pdf_page: 242
    - "no": 4
      title: 'Application: topological properties of the space $\mathscr{M}_+^b(T)$'
      page: 63
      pdf_page: 245
    - "no": 5
      title: Compactness criterion for tight convergence
      page: 64
      pdf_page: 246
    - "no": 6
      title: Tight convergence of measures and compact convergence of functions
      page: 67
      pdf_page: 249
    - "no": 7
      title: 'Application: the Laplace transformation'
      page: 68
      pdf_page: 250
statements: 33
exercises: 13
content_sha256: 2705e533a6075b75cbb65cce60699e62c04a9a01b880d0be5f11775365d7f620
translated_from: content/en/int/IX/05_s5_measures_on_completely_regular_spaces.md
translation_method: google
source_content_sha256: 0a375a056c9792c3ccd44cccce1d823b83bccfdd6973e87e8cb9fdf911d4ef53
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: cc3eea4378e9cfaddb2a9d480fa325f575a407e1091762f5c82099b79019b8ce
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## § 5。完全に定期的な対策空間

T がトポロジカル空間で、F がバナハ空間である場合、記法 $C^b(T; F)$ は、一様収束のノルムを備えた、F の値を持つ T 上の有界連続写像の空間を示します。 $F = \mathbf{R}$の場合、この記法は$C^b(T)$、曖昧さがなければ$C^b$に短縮され、$C^b(T)$の正の写像の円錐を$C^b_+(T)$または$C^b_+$で示します。 T 上の有界複素測度の空間は、有界実測度の $M^b(T; \mathbf{C})$、空間が $M^b(T)$ または $M^b$ で示され、有界正の測度の円錐が $M^b_+(T)$ または $M^b_+$ で示されます。

### 1. メジャーと有界連続写像

(GT、IX, §1, No. 5、定義 4) を思い出してください。トポロジカル空間 T は、均一化可能でハウスドルフである場合、完全に正則であると言われます。これは、T がコンパクト空間の部分空間と同相であるというという (上記引用、提案 3) と同等です。 T が完全に正則である場合、T 上のすべての正の下部半連続写像 $f$ は、$C^b_+(T)$ の元の増加する有向集合の上部包絡線、つまり $\leq f$ であり、すべての正で有界な上部半連続写像です。 $g$ は、$\geq g$ である $C^b_+(T)$ の元の減少する有向集合の下側エンベロープです (引用文献、§1, No. 6、提案 5)。次の補題が必要になります。

#### 補題 {#int-ix-s5-n1-lem-1 .statement tag=09QV}

T を完全な正則空間、K を T のコンパクト部分集合、U を T 含む K のオープン部分集合とします。
a) $K \subset U' \subset \overline{U'} \subset U$ となるような T の開いた部分集合 U' が存在します。
b) f を、$\mathbf{R}$ の区間 I (それぞれ $\mathbf{C}$) の値で K 上で定義された連続写像とする。 T には有界連続写像 $f'$ が存在し、I (それぞれ $\mathbf{C}$) に値があり、拡大する f であり、$T - U$ では零です。

T がコンパクト空間 X の部分空間である場合を扱うだけで十分です。 V を $V \cap T = U$ となるような X のオープン部分集合とします。 $V'$ でX 含む K の開いた集合を$\overline{V'} \subset V$ で表し、X で連続写像とI の値 (それぞれ$\mathbf{C}$) で表します。 $X - V$ で f と零を拡張します (GT、IX, §4, No. 1、提案 1)。 条件 a) $U' = V' \cap T$ を取ることで満たされ、b) $f'$ を g から T の制限とすることで満たされます。

#### 命題 1 {#int-ix-s5-prop-1 .statement tag=09QW}

— T を完全に正規の空間とします。
a) $\mu$ を T 上の正の測度とし、f を T および下部半連続 (それぞれ上部半連続、有限、コンパクトなサポート付き) で定義された数値写像 $\geq 0$ とします。それから

(1) $\mu^\bullet(f) = \sup_{g \in I_f} \mu^\bullet(g)$ (それぞれ $\mu^\bullet(f) = \inf_{g \in S_f} \mu(g)$)、

ここで、$I_f$ (それぞれ $S_f$) は、$0 \leq g \leq f$ (それぞれ $g \geq f$) となるような有界連続写像 $g$ の集合を表します。

b) $\theta$ を $T$ 上の複素数値とし、$f$ を $T$ およびそれ以下の半連続で定義された数値写像 $\geq 0$ とします。それから

(2) $|\theta|^\bullet(f) = \sup_g |\theta(g)|$、

ここで、$g$ は、$|g| \leq f$ となるような、有界かつ $|\theta|$ 積分可能な連続複素数写像の集合上で実行されます。

$I_f$ は、上部包絡線が $f$ である連続写像の増加する有向集合であるため、公式 (1) の最初の部分は明らかであり、§1, No. 6 の提案 5 を適用できます。 $S_f$ 含むが $\mu$ 可積分有界連続写像であることを示す場合、同じ命題は 2 番目の公式を意味します。従って、$K$ を $f$ のサポート、$M$ を $f$ の上限とします。 $K$ はコンパクトなので、$M$ は有限です (GT、IV, §6, No. 2、Th. 3)。 $U$ をオープン集合含む $K$ とし、$\mu^\bullet(U) < +\infty$ とします。 $[0, M]$ に値を伴う連続写像 $g$ が存在します (補題)。これは、$K$ の $M$ と $U$ の外側の零に等しいです。次に$g \in S_f$と$\mu^\bullet(g) \leq M \mu^\bullet(U) < +\infty$。

b)に移りましょう。 $|\theta|^\bullet(f) \leq \sup_g |\theta(g)|$ であることを示すだけで十分であることは明らかです。

$a$ と $b$ を 2 つの実数とし、$a < b < |\theta|^\bullet(f)$ とします。 (1) により、$h \leq f$ と $|\theta|^\bullet(h) > b$ となる写像 $h \in \mathscr{C}_+^b(T)$ が存在します。 $M$ は $h$ の上限を示します。 $|\theta|^\bullet$ (§1, No. 2、定義 4) の定義により、$|\theta|_K^\bullet(h_K) > b$ となるような $T$ のコンパクトな部分集合 $K$ が存在します。次に、$|j| \leq h_K$ と $|\theta_K(j)| > b$ のように、$K$ 上に連続複合体写像 $j$ が存在します (Ch. III, §1, No. 6)。 選ぶをオープン集合 $U$ 含む $K$ とし、$|\theta|^\bullet(U - K) \leq \frac{b - a}{M}$ (§1, No. 9、提案 13 および 14) とします。 拡大する $j$ $T$ の連続複合施設写像 $k$、$U$ (補題) の外側の零。 $t \in T$、集合ごとに

(3)
$$
g(t) = \begin{cases}
k(t) & \text{if } |k(t)| \leq h(t) \\
\frac{k(t)}{|k(t)|} h(t) & \text{if } |k(t)| > h(t)
\end{cases}
$$

明らかに$|g| \leq h \leq f$、$K$の$g = j$、従って$||\theta_K(j)| - |\theta(g)|| = ||\theta(j^0)| - |\theta(g)|| \leq |\theta|^\bullet(|j^0 - g|) \leq M \cdot |\theta|^\bullet(U - K) \leq b - a$、その結果$|\theta(g)| > a$になります。一方、$g$ が連続的な写像であることを示してみましょう。

$a$ は唯一の条件 $a < |\theta|^*(f)$ の影響を受けるため、これは (2) の 2 番目のメンバーが最初の $\geqslant$ であるよって命題であることを意味します。ここで、F (それぞれ $F'$) を $t \in T$ の集合とし、$|k(t)| \leq h(t)$ (それぞれ $|k(t)| \geq h(t)$) とします。これらの集合が閉じており、その和集合が T であるため、$g_F$ と $g_{F'}$ が連続であることを示すだけで十分です。 さて、この性質は $g_F = k_F$ について明らかであり、$k(t) \neq 0$ である点の $g_{F'}$ についても同様です。一方、$t \in F'$ が $k(t) = 0$ である場合、$h(t) = 0$、および不等式 $|g| \leq h$ は、$g$ が点 $t$ で連続であることを意味します。

#### 注意 1 {#int-ix-s5-n1-rem-1 .statement tag=09QX}

$f$ を正の下側半連続写像とし、$J_f$ を$\mu$ 積分可能な開いた集合の外側にあり、上が $f$ で囲まれた正の有界連続写像零の集合とします。 $f$ は $J_f$ の上部エンベロープであり、$\mu^*(f) = \sup_{g \in J_f} \mu(g)$ であることがわかります。

#### 注意 2 {#int-ix-s5-n1-rem-2 .statement tag=09QY}

メジャー $\mu$ が有界である場合、公式 $\mu^*(f) = \inf_{g \in S_f} \mu(g)$ は、上部半連続で正で有界であるすべての写像 $f$ に対して明らかに有効です。

#### 命題 2 {#int-ix-s5-prop-2 .statement tag=09QZ}

— *$\eta$ と $\eta'$ を完全に規則的な空間 $T$ 上の 2 つの複素メジャーとし、写像 $f \in \mathscr{C}^b(T)$ ごとに $\eta(f) = \eta'(f)$ が$|\eta|$ と $|\eta'|$ で積分可能であるとします。次に、$\eta = \eta'$.*

命題 1 の 2 番目の部分の設定 $\theta = \eta - \eta'$ の証明をもう一度取り上げてみましょう。開いた集合 U が $|\eta|$ と $|\eta'|$ に対して積分可能であることを要求できます。 写像 $g$ はこれら 2 つの測度に対して積分可能であり、関係 $\theta(g) = 0$ は $a < 0$ を意味します。したがって、すべての正の下側半連続写像 $f$、よってに対して $|\theta|^*(f) = 0$、$f = +\infty$ を取ると、最終的に $|\theta| = 0$ になります。

#### 命題 3 {#int-ix-s5-prop-3 .statement tag=09R0}

— *$\mu$ を完全に規則的な空間 $T$ に対するプラスの尺度とし、$p \in [1, +\infty[$ とします。 写像 $f \in \mathscr{C}^b(T)$ の空間 $\mathscr{H}$ は、$\mu$ 積分可能なオープン集合にサポートが含まれており、$\mathscr{L}^p(\mu)$ には密集しています。

§1, No. 10 の提案 15 により、K が T でコンパクトであり、$g$ が 0 と 1 の間の $\mathscr{C}_+(K)$ で写像の 0 によって T に対して拡大である場合、写像 $f \in \mathscr{C}_+^b(T)$ が存在し、a にサポートが含まれることを示すだけで十分です。 $\|f - g\|_p$ が任意に小さくなるように、$\mu$ 積分可能なオープン集合。ここで、$\varepsilon$ を数 $> 0$ とし、U は $\mu^*(U - K) < \varepsilon$ のような K の開放近傍、V は $\overline{V} \subset U$ および $f$ 写像で $[0, 1]$ に値が連続し、次と等しい K の開放近傍です。 K では $g$、外側では 0 V (補題) になります。 写像 $|f - g|^p$ はその上で $\varphi_{U-K}$ によって制限されます。したがって、$\|f - g\|_p \leq \varepsilon^{1/p}$ となり、命題が確立されます。

*注意 3).* — Banach 空間 F では、写像と値の類似した主張があります: $\mathscr{C}^b(T; F)$ の部分空間 $\mathscr{H} \otimes F$ は $\mathscr{L}_F^p(\mu)$ で密です。

#### 命題 4 {#int-ix-s5-prop-4 .statement tag=09R1}

— *完全に正規の空間 $T$ 上の有界複素測度 $\theta$ が正である位数では、写像 $f \in \mathscr{C}_+^b(T)$ ごとに $\theta(f) \geq 0$ であることが必要かつ十分です。

必要性は明らかです。十分性を確立するために、$p = 1$ と $\mu = |\theta|$ を取り上げて、前の命題の証明をもう一度取り上げましょう。 記法が同じである場合、関係 $\mu^*(|f - g|) \leq \varepsilon$ と不等式 $\theta(f) \geq 0$ は $\theta_K(g_K) = \theta(g) \geq -\varepsilon$ を暗示します。 $g_K$ は 0 と 1 の間の $\mathscr{C}(K)$ の任意の元であるため、$\theta_K$ の尺度は正になります。コンパクトな集合 K は任意なので、これは $\theta$ が正であることを意味します。

### 2. $\mathscr{C}^b(T)$ の限定措置と線型形式

#### 命題 5 {#int-ix-s5-prop-5 .statement tag=09R2}

— *T を完全に正則な空間とし、I を正規化された空間 $\mathscr{C}^b(T; \mathbf{C})$ 上の連続複素数線型形式とする。 位数では、すべての $f \in \mathscr{C}^b(T; \mathbf{C})$ に対して $\theta(f) = I(f)$ となるような有界複素測度 $\theta$ が T に存在するため、次の条件が満たされることが必要十分です。

(M) *すべての数 $\varepsilon > 0$ に対して、関係 $g \in \mathscr{C}^b(T; \mathbf{C}), |g| \leq 1, g_K = 0$ が $|I(g)| \leq \varepsilon$ を暗示するような T のコンパクトな部分集合 K が存在します。

したがって、メジャー $\theta$ は一意になります。*

一意性は、No. 1の提案2から続きます。 条件 (M) が必要であることを示しましょう。 $\theta$ を有界複素測度とする。 K を $|\theta|^*(T - K) \leq \varepsilon$ (§ 1, No. 2, *注意 3*) となるようなコンパクト集合とします。仮説 $|g| \leq 1, g_K = 0$ は $|g| \leq \varphi_{\mathbf{C}_K}$ を意味するため、$|\theta(g)| \leq |\theta|^*(\varphi_{\mathbf{C}_K}) \leq \varepsilon$ になります。

十分性の証明に進みましょう。 X を T の Stone-Čech コンパクト化 (GT、IX, § 1、Exer. 7; または TG、IX, § 1, No. 6) とします。 写像 $f \in \mathscr{C}(X; \mathbf{C})$、集合 $\nu(f) = I(f_T)$ ごとに;このようにして定義するは $\mathscr{C}(X; \mathbf{C})$ 上で連続する線型形式、つまりコンパクトな空間 X 上の複素測度になります。 $\varepsilon$ を数 $> 0$ とし、K をコンパクト集合満たす (M) とします。 写像 $\varphi_{\mathbf{C}_K}$ が半連続で下位で、X、公式で正であることにより、次の関係が得られます。ここで、$\mathscr{G}$ は、$|g| \leq \varphi_{\mathbf{C}_K}$ のような写像 $g \in \mathscr{C}(X; \mathbf{C})$ の集合を示します。

$$
|\nu|^*(X - K) = \sup_{g \in \mathscr{G}} |\nu(g)| = \sup_{g \in \mathscr{G}} |I(g_T)| \leq \varepsilon.
$$

$(K_n)_{n \geq 1}$ を T の圧縮部分集合の数列とし、各 $K_n$ が $\varepsilon = 1/n$ について (M) を満たすようにし、$S = \bigcup K_n$ とします。 S は、T に含まれる X のボレル集合であり、すべての n に対して $|\nu|^*(X - T) \leq |\nu|^*(X - S) \leq |\nu|^*(X - K_n) \leq 1/n$ であるため、T は $\nu$ 可測で、$\nu$ は T に集中します。$f$ を T 上の有界連続写像とします。 X は T のストーンチェフ圧縮であるため、$f$ は連続性によって写像 $g \in \mathscr{C}(X; \mathbf{C})$ まで拡張できます。ここで、$\mu$ を、$T$ に $\nu$ によって引き起こされる尺度とします。 1 つは $\mu(f) = \nu(f^0)$ です。 (1) $\nu$ は $T$ に集中しているため、写像 $f^0$ と $g$ はほぼどこでも $\nu$ に等しいため、$\mu(f) = \nu(g) = I(g_T) = I(f)$ となり、証明が完成します。

#### 系 {#int-ix-s5-n2-cor-1 .statement tag=09R3}

— *提案 5 の記法では、すべての $f \in \mathscr{C}^b(T; \mathbf{C})$ に対して $|I(f)| \leq \mu(|f|)$ となるような、$T$ に有界正測度 $\mu$ が存在すると仮定します。この場合、$T$ にはすべての $f \in \mathscr{C}^b(T; \mathbf{C})$ に対して $\theta(f) = I(f)$ となるような複雑な尺度 $\theta$ が存在します。

### 3. 制限されたメジャーの緊密な収束

$T$ を完全に正規の空間とします。 双線形形式
$$
(f, \mu) \mapsto \int f(t) \, d\mu(t)
$$
on $\mathscr{C}^b(T) \times \mathscr{M}^b(T)$ は、これら 2 つの空間を分離する二重性の中に置きます。なぜなら、$\varepsilon_x \ (x \in T)$ 属するから $\mathscr{M}^b(T)$ までの措置が$\mathscr{C}^b(T)$ で二重性を分離していることは明らかだからです。 No. 1の提案2により$\mathscr{M}^b(T)$で分離中です。

#### 定義 1 {#int-ix-s5-def-1 .statement tag=09R4}

*$\mathscr{C}^b(T)$ と $\mathscr{M}^b(T)$ の間の先行双対性に関連する $\mathscr{M}^b(T)$ 上の弱い位相は、$\mathscr{M}^b(T)$ 上のタイトな収束 (またはタイトな位相) の位相と呼ばれます。

タイトな位相はハウスドルフで、定義の前に注意がいます。私たちは、「きつい位相」という意味で副詞「tightly」をよく使います。逆の言及がない限り、$\mathscr{M}^b(T)$ には、この切断の残りの部分全体で、タイトな位相が装備されます。

$\mathscr{C}^b(T)$ のすべての元は、$\mathscr{C}_+^b(T)$ の元の線形結合です。 $\mathscr{M}^b(T)$ のフィルター $\mathfrak{F}$ が制限された測定値 $\lambda$ に厳密に収束するには、次のことが必要かつ十分です。
$$
\lim_{\mu} \mu(f) = \lambda(f) \quad \text{with respect to } \mathfrak{F} \text{ for every } f \in \mathscr{C}_+^b(T).
$$

#### 注意 1 {#int-ix-s5-n3-rem-1 .statement tag=09R5}

$T$ が局所的にコンパクトである場合、タイトな位相は、曖昧な位相によって $\mathscr{M}^b(T)$ に誘導される位相よりもより細かいとなり、これら 2 つのトポロジー 一致するは、$T$ がコンパクトな場合にのみ発生します。なぜなら、$T$ がコンパクトでない場合、写像 $t \mapsto \varepsilon_t$ は、$T$ の比較的コンパクトな部分集合の補数のフィルターに関して漠然と 0 に収束しますが、写像 1 属するが$\mathscr{C}^b(T)$ (曖昧な収束と厳密な収束の間の関係については、提案 9 を参照)。

(1) この関係は、$f$ と $\nu$ が正の場合にのみ、上記 (§ 2, No. 1、提案 1) で成立します。 $f$ と $\nu$ が複雑で有界である現在の状況に対して拡大は、線形性により明らかになります。

#### 注意 2 {#int-ix-s5-n3-rem-2 .statement tag=09R6}

提案 4 からすぐに、$\mathscr{M}_+^b(T)$ が $\mathscr{M}^b(T)$ で閉じられることがわかります。

#### 注意 3 {#int-ix-s5-n3-rem-3 .statement tag=09R7}

T が完全に正則であれば、T の $\mathscr{M}^b(T)$ への写像 $t \mapsto \varepsilon_t$ は準同型写像 (GT, IX, §1, No. 5) です。

#### 命題 6 {#int-ix-s5-prop-6 .statement tag=09R8}

— T を完全に正規の空間とします。

a) f を T 上で定義された下位の半連続数値写像 $\geqslant 0$ とする。次に、写像 $\mu \mapsto |\mu|^*(f)$ は、$\mathscr{M}^b(T)$ で下位の半連続です。

b) f を T 上で定義された半連続の上限写像とする。その後、写像 $\mu \mapsto \mu(f)$ は$\mathscr{M}_+^b(T)$ の上半連続です。

なぜなら、No. 1 の提案 1 b) により、$\mu \mapsto |\mu|^*(f)$ は形 $\mu \mapsto |\mu(g)|$ と $g \in \mathscr{C}^b(T)$ の族写像の上部エンベロープであり、したがってタイトな位相に対して連続であることがわかります。これにより、a) が確立されます。 b) を証明するには、f に選ぶ定数上界 C を代入し、$\mu(f) = \mu(C) - \mu(C - f)$ と書くだけで十分です。以上により、写像 $\mu \mapsto \mu(C)$は連続、写像 $\mu \mapsto \mu(C - f)$は$\mathscr{M}_+^b(T)$の下半連続となります。

#### 命題 7 {#int-ix-s5-prop-7 .statement tag=09R9}

— T を完全に正規の空間とします。 $\mu$ を T 上の有界正の測度、f を T 上の有界正の写像とし、f が連続でない T の点の集合が局所的に $\mu$ 無視できるようにします。次に、$\mathscr{M}_+^b(T)$ から $\mathbf{R}$ への写像 $\lambda \mapsto \lambda^*(f)$ は、点 $\mu$ で連続します。

$t \in T$、集合 $f'(t) = \liminf_{s \to t} f(s)$、$f''(t) = \limsup_{s \to t} f(s)$ ごとに。明らかに $f' \leqslant f \leqslant f''$ で、f が連続する T の点ごとに等式が付きます (従って、$\mu$ - ほぼどこでも)。一方、$f'$ は下部半連続であり、$f''$ は上部半連続で有界です (GT、IV, §6, No. 2、提案 4)。従って、提案 6 により次の関係が得られます。

$$
\mu^*(f') \leqslant \liminf_{\lambda \to \mu} \lambda^*(f') \leqslant \liminf_{\lambda \to \mu} \lambda^*(f) \leqslant \mu^*(f) \leqslant \limsup_{\lambda \to \mu} \lambda^*(f)
$$
$$
\leqslant \limsup_{\lambda \to \mu} \lambda^*(f'') \leqslant \mu^*(f'').
$$

観察するとによる 1 つの結論すると $\mu^*(f') = \mu^*(f'')$ は、$f'$ と $f''$ は局所的には $\mu$、ほぼどこでも等しいためです。

#### 命題 8 {#int-ix-s5-prop-8 .statement tag=09RA}

— X を完全に正規の空間とし、X の T 部分空間、そして T の標準単射を X にします。 $\mathscr{M}^b(X)$ によって誘導される位相を備えた、T に集中するX の有界ポジティブ指標を W 集合で示します。この場合、$\mathscr{M}_+^b(T)$ の $\mathscr{M}^b(X)$ への写像 $\mu \mapsto i(\mu)$ は、W に対する $\mathscr{M}_+^b(T)$ の同相写像です。

$\mathscr{M}_+^b(T)$ を i 写像 $\mu \mapsto i(\mu)$ で$\mathscr{M}_+^b(X)$ に再度表します。 i は単射法 (§2, No. 4、提案 8) であり、写像 $\mathscr{M}_+^b(T)$ は W になります (§2, No. 3、提案 7)。 $\lambda \in W$ の場合、$\lambda = i(\lambda_T)$ (§2, No. 3、提案 7 b))。その結果、i は W 上では $\mathscr{M}_+^b(T)$ の全単射となり、i の逆全単射は $W$ 上では写像 $r : \lambda \mapsto \lambda_T$ となります。一方、$i$ は連続です。つまり、$f \in \mathscr{C}^b(X)$ なら $\langle i(\mu), f \rangle = \langle \mu, f \circ i \rangle$、$f \circ i$ 属するから $\mathscr{C}^b(T)$ までです。従って、すべては、すべてのメジャー $\mu \in W$ およびすべての写像 $f \in \mathscr{C}^b_+(T)$ について、

$$
\lim_{\lambda \to \mu, \lambda \in W} \lambda_T(f) = \mu_T(f),
$$

またはもう一度

$$
\lim_{\lambda \to \mu, \lambda \in W} \lambda(f^0) = \mu(f^0).
$$

$f^\infty$ を $X$ の写像 、$T$ の $f$ と $X - T$ の $+\infty$ を持つ一致するとし、$f'$ と $f''$ をそれぞれ $f^0$ の上位半連続正則化とするそして、$f^\infty$ (GT、IV, §6, No. 2) の下部の半連続正則化です。 関係

$$
f'(x) = \limsup_{y \to x} f^0(y), \quad f''(x) = \liminf_{y \to x} f^\infty(y)
$$

$f'$と$f''$は両方とも一致するで、$T$には$f$と$f^0$が含まれることを即座に暗示します。提案 6 は次のようになります。

$$
\mu^\bullet(f') \geq \limsup_{\lambda \to \mu, \lambda \in W} \lambda^\bullet(f'), \quad \mu^\bullet(f'') \leq \liminf_{\lambda \to \mu, \lambda \in W} \lambda^\bullet(f'').
$$

しかし、$\lambda$と$\mu$は$T$によって実行されるため、これら2つの公式では$f^0$によって置き換える$f'$と$f''$が可能です。このようにして、目的の関係を取得しました。

提案 8 の主張は、肯定的な測度の場合にのみ有効です: $\mathscr{M}^b(T)$ の $\mathscr{M}^b(X)$ への写像 $\mu \mapsto i(\mu)$ は単射的かつ連続ですが、一般に、その像に対する $\mathscr{M}^b(T)$ の同型写像ではありません。たとえば、$X = \mathbf{R}$、$T = \mathbf{R} - \{0\}$ を考えてみましょう。 $\lambda_t = \varepsilon_t - \varepsilon_{-t}$ ($t > 0$) のメジャーは、$t$ が 0 に向かう傾向があるため、$X$ では 0 に厳密に収束しますが、$T$ では 0 に厳密に収束しません ($]0, +\infty[$ 属するから $\mathscr{C}^b(T)$ の特性写像) (cf. ただし、No. 5 の Th. 1 の Cor.)。

#### 命題 9 {#int-ix-s5-prop-9 .statement tag=09RB}

— *T を局所的にコンパクトな空間とし、$\mathfrak{F}$ を有界メジャー $\mu$ に曖昧に収束する $\mathscr{M}^b_+(T)$ のフィルターとします。 $\mathfrak{F}$ が $\mu$ にしっかりと収束するには、$\mathfrak{F}$ に対して $\lim_{\lambda} \lambda(1) = \mu(1)$ であることが必要かつ十分です。

条件は明らかに必要です。それが十分であることを示すために、$T$ (GT, I, §9, No. 8) の Alexandroff コンパクト化を $X$ で表し、$T$ から $X$ への $i$ 標準単射で表します。提案 8 により、すべては、$\mathfrak{F}$ に関して $\mathscr{M}^b(X)$ で $\lambda \mapsto i(\lambda)$ が $i(\mu)$ にしっかりと収束することを示すことになります。 $\mu(1) < +\infty$ 以降、$A$ のメジャーの合計質量が数 $M$ によって制限されるように、集合 $A \in \mathfrak{F}$ が存在します。したがって、それを確認するだけで十分です

$$
\lim_{\lambda, \mathfrak{F}} \int_X g \, d(i(\lambda)) = \int_X g \, d(i(\mu))
$$

写像 $g \in \mathscr{C}^b(X)$ で、$\mathscr{C}^b(X)$ の合計集合が形成されます。 さて、この等式は、$\mathfrak{F}$ から $\mu$ への曖昧な収束のため、$g$ が $T$ でコンパクトなサポートを持つとき、また、$\lim_{\lambda, \mathfrak{F}} \lambda(1) = \mu(1)$ であるという事実から、$g$ が $X$ 上の定数写像であるときにも満たされます。 前の 2 つの型形のうち写像なので、$\mathscr{C}^b(X)$ では合計集合になります (Ch. III, §1, No. 2、提案 3)、これで証明が完了します。

### 4. 応用: 空間 $\mathscr{M}_+^b(T)$ のトポロジカル特性

まず、$T$ が完全に正則である場合、$\mathscr{M}^b(T)$ はハウスドルフトポロジカルベクトル空間であるため、完全に正則であることがわかります。従って、$\mathscr{M}_+^b(T)$ は完全に正規です。

#### 命題 10 {#int-ix-s5-prop-10 .statement tag=09RC}

*$T$ をポーランド語空間とします。 空間 $\mathscr{M}_+^b(T)$ は、タイトな位相に合わせてポリッシュされます。*

まず、$T$ がポーランド語で *コンパクト* である場合を扱います。質量 $\leq 1$ を持つポジティブ指標の集合 $U$ はコンパクトになり (提案 15 の III, §1, No. 9、Cor. 2)、タイトな位相 (ここでは曖昧な一致する) によって $U$ に位相が誘導されます。 位相) は、$\mathscr{C}(T)$ の合計部分集合に対する点ごとの収束の位相によっても引き起こされます (*上記引用*、No. 10、提案 17)。さて、$\mathscr{C}(T)$ には可算合計集合 (GT、X, §3, No. 3、Th. 1) が存在します。従って、$U$ は計量可能コンパクト空間です。質量の正の尺度$< 1$の集合$V$は$U$にオープンしているため、ポーランドの局所的にコンパクトな空間です。さて、$\mathscr{M}_+^b(T)$ の $V$ への写像 $\mu \mapsto \frac{1}{1 + \mu(1)} \mu$ は準同型写像であり、写像 $\lambda \mapsto \frac{1}{1 - \lambda(1)} \lambda$ は逆準同型写像です。

$T$ がポーランド語である場合に移りましょう。 $T$ は、計量可能コンパクト空間 $X$ (GT、IX, §6, No. 1、Th. 1 の Cor. 1) における、開いた集合の減少列 $(G_n)$ の共通部分であると仮定できます。 空間 $\mathscr{M}_+^b(T)$ は、$T$ に集中した測度の $\mathscr{M}_+^b(X)$ からなるの部分空間 $W$ と同型であり (No. 3、提案 8)、$W$ が共通部分であることを示せば十分です。ポーランド語で空間 $\mathscr{M}_+^b(X)$ のオープン集合の数列 (GT、*loc. cit.*、Th. 1)。 さて、$W_n$を$G_n$に集中した対策$\mu \in \mathscr{M}_+^b(X)$の集合とします。 $\mathscr{M}_+^b(X)$ の写像 $h_n : \mu \mapsto \mu^*(X - G_n)$ は上部半連続 (No. 3、提案 6)、および $\mu \in \mathscr{M}_+^b(X)$ の集合 $A_k^n$ であるため、$h_n(\mu) < 1/k$ はすべての $k \geq 1$ とすべての $n \in \mathbf{N}$ に対してオープンになります。 証明は$W = \bigcap_n W_n = \bigcap_{n,k} A_k^n$の観察するとによって完了します。

#### 系 1 {#int-ix-s5-prop-10-cor-1 .statement tag=09RD}

*T が可算型の計量可能空間である場合、密位相の場合、$\mathscr{M}_+^b(T)$ は可算型の計量可能です。*

なぜなら、T の位相を定義するメトリックに対する T の完了を $\hat{T}$ とするためです。 空間 $\hat{T}$ はポーランド語であり、$\mathscr{M}_+^b(T)$ はポーランド語空間 $\mathscr{M}_+^b(\hat{T})$ からなるの部分空間と同型です (No. 3、提案 8)。しかし、ポーランド語空間のすべての部分空間は可算型 (GT、IX, §2, No. 8) の計数可能です。

#### 系 2 {#int-ix-s5-prop-10-cor-2 .statement tag=09RE}

*T が完全に通常のスースリン (またはルーシン) 空間である場合、空間 $\mathscr{M}_+^b(T)$ はスースリン (またはルーシン) です。

たとえば、ポーランドの空間 P と T への P の連続写像 $f$ を考えてみましょう (GT、IX, §6, No. 2、定義 2)。 $\tilde{f}$ を $\mathscr{M}_+^b(P)$ から $\mathscr{M}_+^b(T)$ への連続写像 $\mu \mapsto f(\mu)$ とします。 空間 $\mathscr{M}_+^b(P)$ は提案 10 によりポーランド語であり、$\tilde{f}$ は全射法です (§2, No. 4、提案 9)。したがって、空間 $\mathscr{M}_+^b(T)$ はスースリンです。同様に、T が Lusin の場合、$f$ は単射であると仮定できます (GT, *loc. cit.*, No. 4, Prop. 12)。その場合、$\tilde{f}$ は単射法 (§2, No. 4、提案 8) なので、$\mathscr{M}_+^b(T)$ は Lusin (GT、*loc. cit.*、No. 4、提案 12) です。

T を完全に正規の Souslin 空間とします (この場合、T が Souslin で *正規* (TG、App. 1、Prop. 2 の Cor.) で十分であることを思い出してください)、H を $\mathscr{M}_+^b(T)$ の圧縮部分集合とします。その場合、H はコンパクトであり、Souslin であるため、タイトな位相に対して *metrizable* になります (*loc. cit.*、App. 1、Prop. 3 の Cor. 2)。

### 5. 厳密な収束のためのコンパクト性の基準

#### 定義 2 {#int-ix-s5-def-2 .statement tag=09RF}

*T をトポロジー 空間とし、H を $\mathscr{M}^b(T)$ の部分集合とします。ある人は、H がプロホロフの条件 if* を満たすと言います。
    a) $\sup_{\mu \in H} |\mu|(1) < +\infty$;
    b) *すべての数 $\varepsilon > 0$ に対して、次のような T のコンパクト部分集合 $K_\varepsilon$ が存在します*
    $$
    |\mu|(T - K_\varepsilon) \leq \varepsilon \quad \text{for every measure } \mu \in H.
    $$

T が完全に正則である場合、条件 *a)* および *b)* の集合は次の条件と同等であることが示されます。T には実数の写像 $f \geq 1$ が存在し、T 満たすの点 t の集合が存在します。 $f(t) \leq c$ はすべての $c \in \mathbf{R}_+$ に対してコンパクトであり (特に、$f$ がより低い半連続であることを意味します)、$\sup_{\mu \in H} |\mu|(f) < +\infty$ も同様です。さらに、T が局所的にコンパクトである場合、f が連続であることを要求することにより、等価な主張が得られます (cf. Exer. 10)。

#### 命題 11 {#int-ix-s5-prop-11 .statement tag=09RG}

*T を完全に正規の空間とし、H をプロホロフの条件を満たす $\mathscr{M}^b(T)$ の部分集合とします。その後、$\mathscr{M}^b(T)$ の終結 $\overline{H}$ はプロホロフの条件を満たします。*

なぜなら、写像 $\mu \mapsto |\mu|^*(1)$、$\mu \mapsto |\mu|^*(T - K_\varepsilon)$ は、No. 3 の提案 6 により、$\mathscr{M}^b(T)$ で下位半連続です。

プロホロフの条件の興味は次の定理から来ており、その逆は後で研究されます (Th. 2)。

#### 定理 1 (プロホロフ) {#int-ix-s5-thm-1 .statement tag=09RH}

— *T を完全に正規の空間とし、H をプロホロフの条件を満たす $\mathscr{M}^b(T)$ の部分集合とします。この場合、H は、タイトな位相に対して $\mathscr{M}^b(T)$ で比較的コンパクトになります。*

T はコンパクト空間 X の部分空間であると仮定できます。 T の標準単射を X にします。一方、提案 11 により、H が $\mathscr{M}^b(T)$ で *閉じている* と仮定できます。その後、H 上のすべての限外フィルター $\mathfrak{U}$ が $\mathscr{M}^b(T)$ に収束することを示せば十分です。

$H \subset \mathscr{M}_+^b(T)$ の場合から始めます。 仮定、$i(\mu)$ によって制限される測度 $\mu \in H$ の総質量は、$\mathscr{M}_+(X)$ の $\mathfrak{U}$ に関して漠然と測度 $\nu \in \mathscr{M}_+(X)$ に収束します (提案 15 の第 III, §1, No. 9 項、コリント 2)。 No. 3 の提案 8 により、すべては $\nu$ が T に集中する証明になります。 さて、$\varepsilon$ を数 $> 0$ とし、$K_\varepsilon$ を T 満たすの圧縮部分集合とします。 公式 (6)。 $X - K_\varepsilon$ は X でオープンであるため、No. 3 の提案 6 により X に適用される不等式は次のようになります。

$$
\nu^*(X - T) \leq \nu^*(X - K_\varepsilon) \leq \liminf_{\mu, \mathfrak{U}} i(\mu)^*(X - K_\varepsilon)
= \liminf_{\mu, \mathfrak{U}} \mu^*(T - K_\varepsilon) \leq \varepsilon;
$$

$\varepsilon > 0$ は任意であるため、この特別な場合には定理が確立されます。

一般的なケースに移りましょう。 T の各小節 $\mu$、集合

$$
a_1(\mu) = \Re(\mu)^+, \quad a_2(\mu) = \Re(\mu)^-, \quad a_3(\mu) = \Im(\mu)^+, \quad a_4(\mu) = \Im(\mu)^-;
$$

$\mu = a_1(\mu) - a_2(\mu) + ia_3(\mu) - ia_4(\mu)$ なので、写像 $a_j$ ($j = 1, 2, 3, 4$) が $\mathfrak{U}$ に関してしっかりと収束することを示せば十分です。しかし、小節 $a_j(\mu)$ の集合 $H_j$ は、$\mu$ が H を超えており、関係 $|a_j(\mu)| \leq |\mu|$ によってプロホロフの条件を満たし、$\mathscr{M}_+^b(T)$ に含まれます。したがって、$\mathscr{M}_+^b(T)$ では特殊な場合により比較的コンパクトになり、すぐに定理が続きます。

#### 系 {#int-ix-s5-n5-cor-1 .statement tag=09RI}

— T を完全に正規の空間 X の部分空間とし、H をプロホロフの条件を満たす $\mathscr{M}^b(T)$ の部分集合とします。 i が T の標準単射を X に表す場合、$\mathscr{M}^b(T)$ の写像 $\mu \mapsto i(\mu)$ を $\mathscr{M}^b(X)$ に変換する制限は、その像に対する H の同型写像です。

H が閉じている場合 (提案 11)、したがってコンパクトである場合を扱うだけで十分です。そして、$\mu \mapsto i(\mu)$ が連続的で単射的であるという事実から結論が得られます。

この結果は、$\mathscr{M}_+^b(T)$ の任意の部分集合 (No. 3、提案 8) にも有効であることを思い出してください。

#### 定理 2 {#int-ix-s5-thm-2 .statement tag=09RJ}

— T を局所的にコンパクトな空間またはポーランド語空間とし、H を $\mathscr{M}_+^b(T)$ の比較的コンパクトな部分集合とします。この場合、H はプロホロフの条件を満たします。

H が閉じている、つまりコンパクトである場合に限定することができます。 写像 $\mu \mapsto \mu(1)$ は連続であり、すべては Def の b) 証明主張に帰着するため、測度 $\mu \in H$ の総質量は明らかに有界です。 2.

まず、T が局所的にコンパクトであると仮定します。 $\varepsilon$ を数 > 0 とします。$\mu^\bullet(T - K_\varepsilon) < \varepsilon$ となるような T のコンパクトな集合 $K_\mu$ をすべてのメジャー $\mu \in H$ に関連付け、次に $K_\mu$ の比較的コンパクトなオープン近傍 $U_\mu$ を関連付けます。 写像 $\lambda \mapsto \lambda^\bullet(T - U_\mu)$ は、$\mathscr{M}_+^b(T)$ (No. 3、提案 6)、集合 $V^\mu$ $\lambda \in H$ で、$\lambda^\bullet(T - U_\mu) < \varepsilon$ が H の $\mu$ の近傍となるため、有限部分集合が存在します。 集合 $V^\mu$ ($\mu \in H'$) が H をカバーするような H の $H'$。コンパクトな集合 $\bigcup_{\mu \in H'} \overline{U}_\mu$ を K で表すと、すべての $\lambda \in H$ に対して $\lambda^\bullet(T - K) < \varepsilon$ が得られます。

次に、T がポーランド人だと仮定します。 T がコンパクト空間 X (GT、IX, §6, No. 1、Th. 1 の Cor. 1) のオープン部分集合の減少列 $(T_p)_{p \geq 1}$ の共通部分であると仮定することによって一般性を制限しません。 $i_p$ を $T_p$ に対する T の単射とし、$H_p$ を $\lambda \in H$ に対する形 $i_p(\lambda)$ のメジャーの集合とします。 $H_p$ は $\mathscr{M}_+^b(T_p)$ でコンパクトであるため、局所的にコンパクトな空間 $T_p$ に適用される前の結果により、各小節 $\nu \in H_p$ に対して $\nu^\bullet(T_p - K_p) \leq \varepsilon 2^{-p}$ となるようなコンパクト集合 $K_p \subset T_p$ が存在することになります。 したがって、各小節 $\lambda \in H$ についても $\nu^\bullet(T - (T \cap K_p)) \leq \varepsilon 2^{-p}$、そして最後に $\lambda^\bullet(T - (T \cap K_p)) \leq \varepsilon 2^{-p}$ となります。 現在集合 $K = \bigcap_p K_p$; 集合 K はコンパクトで T に含まれており、各小節 $\lambda \in H$ に対して、$\lambda^\bullet(T - K) \leq \sum_p \lambda^\bullet(T - (T \cap K_p)) \leq \sum_p \varepsilon 2^{-p} = \varepsilon$ が得られます。 こうしてプロホロフの条件が検証されました。

### 6. 対策の緊密な収束と写像のコンパクトな収束

#### 命題 12 {#int-ix-s5-prop-12 .statement tag=09RK}

— T を完全に正規の空間とし、B を正規の空間 $\mathscr{C}^b(T; \mathbf{C})$ のボール単位元とします。 I を $\mathscr{C}^b(T; \mathbf{C})$ の線型形式とします。すべての $f \in \mathscr{C}^b(T; \mathbf{C})$ に対して $I(f) = \theta(f)$ となるような有界複素測度 $\theta$ が T 上に存在する位数では、I から B までの制限がコンパクトな収束の位相の間連続であることが必要かつ十分です。したがって、メジャー $\theta$ は一意になります。

主張の条件が必要であることを示しましょう。 $\theta$ を T 上の有界複素測度、$\varepsilon$ 数 $> 0$、K を $|\theta|^*(T - K) < \varepsilon$ となるような T の圧縮部分集合とします。 $f \in B$ にしましょう。 $\sup_{x \in K} |g(x) - f(x)| \leq \varepsilon$ となるような写像 $g \in B$ によって形成されるコンパクト収束の位相に対する B の $f$ の近傍を U で示します。その後、$g \in U$ ごとに、

$$
|\theta(g) - \theta(f)| \leq \int_T |g - f| d|\theta| \leq \varepsilon |\theta|^*(K) + 2|\theta|^*(T - K) \leq (||\theta|| + 2)\varepsilon ,
$$

なぜなら、$|g - f|$ は K の $\varepsilon$ と $T - K$ の 2 によって上に境界付けされているからです。

逆に、B への制限がコンパクト収束の位相の間連続である $\mathscr{C}^b(T; \mathbf{C})$ 上の線型形式 I を考えます。次に、すべての数 $\varepsilon > 0$ に対して、 数 $a > 0$ と、関係 $f \in B, \sup_{x \in K} |f(x)| \leq a$ が $|I(f)| \leq \varepsilon$ を暗示するような T のコンパクトな部分集合 K が存在します。 No. 2 の提案 5 は、すべての $f \in \mathscr{C}^b(T; \mathbf{C})$ に対して $I(f) = \theta(f)$ となるような、一意の有界複素測度 $\theta$ の存在を意味します。

#### 命題 13 {#int-ix-s5-prop-13 .statement tag=09RL}

— T を局所的にコンパクトな空間とし、H を正規化空間 $\mathscr{C}^b(T; \mathbf{C})$ の有界な部分集合とします。 $\mathscr{M}_+^b(T) \times H$ から $\mathbf{C}$ への写像 $(\mu, f) \mapsto \mu(f)$ は、$\mathscr{M}_+^b(T)$ がタイトな位相を備え、H がコンパクトな収束の位相を備えている場合、連続します。

$\mu \in \mathscr{M}_+^b(T), f \in H$ とし、M を実数とし、すべての $g \in H$ に対して $||\mu|| < M$、および $|g| \leq M$ とします。 $\varepsilon$ を数 $> 0$ および選ぶを、$\mu^*(T - K) < \varepsilon$ となるような T のコンパクトな部分集合 K とすると、K の比較的コンパクトな開いた近傍 S になります。 集合 U のメジャー $\lambda \in \mathscr{M}_+^b(T)$ 満たすの不等式

$$
\lambda^*(T) < M , \quad \lambda^*(T - S) < \varepsilon , \quad |\lambda(f) - \mu(f)| < \varepsilon
$$

そうすると、$\mathscr{M}_+^b(T)$ の $\mu$ の近隣になります (No. 3、提案 6)。 加法では、写像 $g \in H$ の H からなるにおける $f$ の近傍を V とします。

$$
\sup_{x \in S} |g(x) - f(x)| < \varepsilon .
$$

$\lambda \in U$ と $g \in V$ としましょう。 写像 $|g - f|$ は、$S$ の $\varepsilon$ と $T - S$ の $2M$ によって上に囲まれているため、次のようになります。
$$
|\lambda(g) - \lambda(f)| \leq \int_T |g - f| d\lambda \leq \varepsilon \lambda^*(S) + 2M \lambda^*(T - S) \leq 3M \varepsilon,
$$
どちらから推測するか
$$
|\lambda(g) - \mu(f)| \leq |\lambda(g) - \lambda(f)| + |\lambda(f) - \mu(f)| \leq (3M + 1)\varepsilon.
$$
これは、$\mathscr{M}_+^b(T) \times H$の点$(\mu, f)$における写像$(\lambda, g) \mapsto \lambda(g)$の連続性を証明します。

#### 注意 {#int-ix-s5-n6-rem-1 .statement tag=09RM}

$T$ を、プロホロフの条件、$H$ 、$C^b(T)$ の有界部分集合を満たす、$\mathscr{M}^b(T)$ の完全に正則な空間、$M$ 部分集合とします。先ほど行った議論に非常に近い議論は、$M$ にタイトな位相と$H$ にコンパクトな収束位相が装備されている場合、$M \times H$ から $\mathbf{C}$ への写像 $(\lambda, g) \mapsto \lambda(g)$ が連続であることを証明するために使用できます。

#### 系 {#int-ix-s5-n6-cor-1 .statement tag=09RN}

*$T$ を完全に正規の空間、$X$ をトポロジカルな空間、$f$ を $T \times X$ で定義された連続かつ有界の複素数値の写像とします。 $T$ 上のすべての境界メジャー $\mu$ について、すべての $x \in X$ について $F_\mu(x) = \int_T f(t, x) d\mu(t)$ によって定義される $X$ 上の $F_\mu$ を写像とします。

a) 写像 $F_\mu$ は連続であり、すべての有界メジャー $\mu$ に対して有界です。

b) $T$ が局所的にコンパクトであると仮定します。 $\mathscr{M}_+^b(T)$ から $C^b(X; \mathbf{C})$ への写像 $\mu \mapsto F_\mu$ は、$\mathscr{M}_+^b(T)$ にタイトな位相が装備されている場合、$C^b(X; \mathbf{C})$ にコンパクトな収束の位相が装備されている場合、連続します。

すべての $x \in X$ について、$T$ 上の連続かつ有界の写像 $t \mapsto f(t, x)$ を $f_x$ で示します。 $X$の$C^b(T; \mathbf{C})$への写像$x \mapsto f_x$は像を境界としており、$C^b(T; \mathbf{C})$がコンパクトコンバージェンスの位相を装備していれば連続です（GT、X, §3, No. 4、Th.3）。 $F_\mu(x) = \mu(f_x)$ なので、写像 $F_\mu$ は提案 12 により連続です。 $T$ が局所的にコンパクトであると仮定します。 提案 13 は、$\mathscr{M}_+^b(T) \times X$ から $\mathbf{C}$ への写像 $(\mu, x) \mapsto F_\mu(x)$ が連続であることを示しています。 主張 b) はこれから続きます (*loc. cit.*)。

### 7. 応用: ラプラス変換

この番号では、合成の法則が加法的に書かれた可換モノイドを$M$で表し、$M \times M$から$M$への写像$(m, m') \mapsto m + m'$が連続である*局所的にコンパクトな*空間の位相を備えています。 $M$ の中立の元は $0$ で示されます。 $M$ 満たす関係で、すべての有界連続複素数写像 $\chi$ の $M$ の *指標* を呼び出します。
$$
\chi(m + m') = \chi(m) \cdot \chi(m'), \quad \chi(0) = 1, \quad |\chi(m)| \leq 1
$$

$M$の$m, m'$用。 $\chi$ と $\chi'$ が指標であれば、$\chi \chi'$ も同様です。 $M$ の指標の集合はモノイドであり、$X$ で示されます。 $X \times X$から$X$へ写像$(\chi, \chi') \mapsto \chi \chi'$が連続するコンパクトコンバージェンスの位相を装備します。 $X$ の中立の元は定数写像 1 です。

$M$ 上のすべての有界複素測度 $\mu$ について、$\mu$ の *ラプラス変換* を呼び出し、$X$ で定義される関数 $\mathscr{L}\mu$ を呼び出します。

$$
(\mathscr{L}\mu)(\chi) = \int_M \chi(m)\, d\mu(m).
$$

ThさんよりGT の 3、$M \times X$ から $\mathbf{C}$ へのX, §3, No. 4、写像 $(m, \chi) \mapsto \chi(m)$ は連続的であり、有界です。 No. 6 の提案 13 の系は、次の結果を暗示します。

#### 命題 14 {#int-ix-s5-prop-14 .statement tag=09RO}

*すべての有界複素測度 $M$ の $\mu$、$X$ の写像 $\mathscr{L}\mu$ は連続で有界です。 $\mathscr{M}_+^b(M)$にタイトな位相、$\mathscr{C}^b(X; \mathbf{C})$にコンパクトコンバージェンスの位相が装備されている場合、$\mathscr{M}_+^b(M)$から$\mathscr{C}^b(X; \mathbf{C})$への写像$\mu \mapsto \mathscr{L}\mu$が連続します。

無限遠で 0 になる傾向がある $M$ の指標の集合は $X_0$ と表されます。この集合は乗法で安定しています。 $X$ の部分モノイド$^{(1)}$ S が写像 $\chi \mapsto \overline{\chi}$ に対して安定しており、$S \cap X_0$ が $M$ (GT、X, §4, No. 1、Def. 1) の点を分離し、そして、いずれかの $m \in M$ が与えられた場合、 $\chi(m) \neq 0$ となる $S \cap X_0$ のうち元 $\chi$ が存在します。

加法において、$M$ が非コンパクトなアーベル *群* であると仮定します。 $f$ を $M$ 上の写像とします。これは無限遠で 0 になる傾向があります。同じことが $M$ の写像 $x \mapsto f(x)f(-x)$ にも当てはまりますが、$M$ のすべての指標 $\chi$ は $\chi(x)\chi(-x) = \chi(0) = 1$ を満たします。 したがって、$X_0$ は空であり、$X$ には完全なサブモノイドが含まれていないことがわかります。 したがって、以下の定理 3 は、コンパクトではないローカルにコンパクトな群には適用されません。

#### 定理 3 {#int-ix-s5-thm-3 .statement tag=09RP}

*S を X の完全な部分モノイドとします。*
a) *$\mu$ と $\mu'$ が $M$ 上の 2 つの有界複素測度である場合、$\mathscr{L}\mu$ と $\mathscr{L}\mu'$ が同じ制限から $S \cap X_0$ になるように、$\mu = \mu'$ になります。*
b) *$\mathfrak{F}$を$\mathscr{M}_+^b(M)$のフィルターとし、$\mathscr{L}\lambda(s)$が$s \in S$ごとに$\mathfrak{F}$に関して極限$\Phi(s) \in \mathbf{C}$を持つようにします。次に、フィルター $\mathfrak{F}$ は、境界のある正の測度 $\mu$ とすべての $s \in S \cap X_0$ に対する $\Phi(s) = \mathscr{L}\mu(s)$ に漠然と収束します。
c) *b) の仮説の下で、加法で$S \cap X_0$ 含む 1 の閉包が$S$ の$\Phi$ 写像が点 1 で連続すると仮定します。すると、$\mathfrak{F}$ は$\mu$ にしっかりと収束します。 $\Phi(s) = \mathscr{L}\mu(s)$ はすべての $s \in S$ に対応します。*

$M$ で無限遠で 0 に向かう連続複素数写像の E 代数と、生成された E の線形部分空間を $\mathfrak{A}$ で表すことにします。

(1) A (A, I, §2, No. 1) の定義の中性元によるモノイド含むの部分モノイドを思い出してください。

$S \cap X_0$ までに;その場合、$\mathfrak{A}$ は写像 $f \mapsto \overline{f}$ の下で安定した $E$ の部分代数です。 $S$ は $X$ の完全な部分モノイドであるため、Cor。 GT の提案 7 の 2、X, §4, No. 4 は、$\mathfrak{A}$ が $E$ で密であることを意味します。

a) を証明しましょう: $f \in \mathfrak{A}$ ごとに仮定, $\mu(f) = \mu'(f)$; $\mu$ と $\mu'$ は $E$ で連続する線型形式であるため、これは $f \in E$ に対して $\mu(f) = \mu'(f)$ 、特にコンパクトなサポートを持つすべての連続写像 $f$ 、よって $\mu = \mu'$ を意味します。

b)の仮説の下に身を置いてみましょう。 数 $\Phi(1) = \lim_{\lambda, \mathfrak{F}} \lambda(1)$ は現実的でポジティブです。 実数 $a > \Phi(1)$ を与えましょう。 $\lambda \in \mathscr{M}_+^b(M)$ の $\| \lambda \| = \mathscr{L} \lambda(1)$ から、関係 $\lim_{\lambda, \mathfrak{F}} \mathscr{L} \lambda(1) = \Phi(1)$ は、$\| \lambda \| \leq a$ 属するから $\mathfrak{F}$ までの$\lambda \in \mathscr{M}_+^b(M)$ のメジャーの集合 $H$ を意味します。 $\mathscr{M}^b(M; \mathbf{C})$ は標準的な空間 $E$ の双対と同一視される可能性があるため (Ch. III, §1, No. 8 & §1, No. 2、提案 3)、空間 $H$ は位相 $\sigma(\mathscr{M}^b(M; \mathbf{C}), E)$ に対してコンパクトです。 一方 (TVS、III, §3, No. 4、提案 5)、この $H$ 上の位相一致するは、$E$ の合計部分集合における点ごとの収束の位相を伴います。 特に$E$では$\mathfrak{A}$が密集しているため、コンパクトサポート付き連続写像の空間も同様です（Ch. III, §1, No. 2、提案 3)、$H$ 上の$S \cap X_0$ 一致するにおける点状収束の位相と曖昧な位相 、そして$H$ はこの位相に対してコンパクトです。 すぐに、$\mathfrak{F}$ は漠然と$\mu \in H$ のメジャーに収束し、すべての $s \in S \cap X_0$ については $\mathscr{L} \mu(s) = \lim_{\lambda, \mathfrak{F}} \mathscr{L} \lambda(s)$ になることがわかります。

最後に、c) に進みます。 写像 $\Phi$ と $\mathscr{L} \mu$ は点 $1 \in S$ で連続し、$S \cap X_0$ では等しいので、$1$ は $S \cap X_0$ の閉包にあるので、$\Phi(1) = \mathscr{L} \mu(1)$ になります。他には語、$\lim_{\lambda, \mathfrak{F}} \lambda(1) = \mu(1)$。 No. 3 の提案 9 は、$\mu$ がフィルター $\mathfrak{F}$ の厳密な極限であることを示します。 $S$ のすべての元が $M$ 上の有界連続写像であることは、すべての $s \in S$ について $\Phi(s) = \lim_{\lambda, \mathfrak{F}} \lambda(s) = \mu(s) = \mathscr{L} \mu(s)$ であることを意味します。

#### 系 {#int-ix-s5-n7-cor-1 .statement tag=09RQ}

— *$S$ を、$S \cap X_0$ 含む 1 の閉包となるように、$X$ の完全な部分モノイドとします。 $L$ を、ラプラスの制限から $S$ の $\mathscr{C}^b(S; \mathbf{C})$ からなるの部分集合とします。 変換の対策 $\lambda \in \mathscr{M}_+^b(M)$.*

a) *集合 $L$ は、点収束の位相を備えた空間 $\mathscr{C}^b(S; \mathbf{C})$ で閉じられます。*

b) *写像 $\lambda \mapsto (\mathscr{L} \lambda)_S$ は、$\mathscr{M}_+^b(M)$ に厳密な位相と $L$ に点ごとの収束位相が装備されている場合、$L$ への $\mathscr{M}_+^b(M)$ の同型写像です。

c) $L$ 上の点単位収束の *位相およびコンパクト収束の位相一致する。*

主張 a) と b) は Th の明らか帰結です。 3;コンパクト収束の位相はポイントワイズ収束のそれよりより細かいであるため、主張 c) は b) と提案 14 から成り立ちます。

点ごとの収束の位相を備えた、S 上のすべての有界複素数写像の集合で L が閉じていないことに注意する必要があります。たとえば、以下の例 2 の記法を仮定します (M = \mathbf{R}_+、S は \mathbf{R}_+ で識別されます)。 $\varepsilon_n$ ($n \in \mathbf{N}$) の小節のラプラス変換は、$\mathbf{R}_+$ では写像 $t \mapsto e^{-nt}$ です。 $n$ は $+\infty$ になる傾向があるため、これらの写像は、$t = 0$ では 1、$t \neq 0$ では 0 に等しい写像に点的に収束しますが、属するから L には収束しません。

*例 1).* — 正の整数の M 集合 N、加法の法則およびディスクリート位相を装備したものとします。 D を、\mathbf{C} によって誘導された位相と乗法によって誘導された法則を備えた \mathbf{C} の単位元ディスク (絶対値値 $\leq 1$ の複素数の集合) とします。 すべての $z \in D$ について、N の $f(z)$ 指標 $n \mapsto z^n$ で表します。 N のすべての指標 $\chi$ を、$g(\chi)$ 複素数 $\chi(1) \in D$ で表します。 $f$ と $g$ が D と X の間の相互逆同型写像であることがすぐに検証され、これから *同一視する* X と D が可能になります。 無限遠で 0 になる傾向がある指標の集合は、絶対値 < 1 の複素数の集合 $D_0$ と識別される可能性があります。 最後に、 \mathbf{R} の区間 ]0, 1] は D の完全な部分モノイドであり、 1 は​​ $]0, 1[ \cap D_0 = ]0, 1[$ の閉包内にあります。

N のすべてのメジャー $\mu$ は、形 $\mu = \sum_{n \in \mathbf{N}} u_n \cdot \varepsilon^n$ で独自の方法で記述することができ、$\mu$ は $\sum_n |u_n| < +\infty$ の場合にのみ制限されます。その場合、$z \in D$ に対して $\mathscr{L}\mu(z) = \sum_{n \in \mathbf{N}} u_n z^n$ が得られます。この写像は D で連続しています。これを加算可能な数列 $(u_n)_{n \in \mathbf{N}}$ の *生成する写像* と呼ぶのが通例です。この言語に転写すると、Th. 3 は次の結果をもたらします (No. 3 の提案 9 を考慮に入れて):

#### 命題 15 {#int-ix-s5-prop-15 .statement tag=09RR}

※Aにフィルター$\mathfrak{F}$を装着した集合とします。すべての $\alpha \in A$ について、$(u_{\alpha,n})_{n \in \mathbf{N}}$ を正の数の合計可能な数列とし、$\Phi_\alpha$ を \mathbf{R} の区間 ]0, 1] で $\Phi_\alpha(x) = \sum_{n \in \mathbf{N}} u_{\alpha,n} x^n$ によって定義された写像とします。 位数には、次のような正の数の合計可能な数列 $(u_n)_{n \in \mathbf{N}}$ が存在します*

$$
\lim_{\alpha, \mathfrak{F}} u_{\alpha,n} = u_n \quad \text{for all } n , \quad \lim_{\alpha, \mathfrak{F}} \sum_{n \in \mathbf{N}} u_{\alpha,n} = \sum_{n \in \mathbf{N}} u_n ,
$$

*$\Phi_\alpha$ が、$\mathfrak{F}$ に関して、点的に ]0, 1[ に収束し、点 1 で連続する写像 $\Phi$ に収束することが必要かつ十分です。この場合、すべての $x \in ]0, 1[$ に対して $\Phi(x) = \sum_{n \in \mathbf{N}} u_n x^n$ です。*

M をモノイド $\mathbf{N}^n$ とすることによって、同様の結果が得られます。ここで、$n$ は整数 > 1 を表します。 空間 X は $D^n$ と識別され、選ぶ $]0, 1[^n$ が完全な部分モノイドとして識別される可能性があります。 Th を書き写す作業は読者に任せます。この場合は 3 です。

例 2）。 — 加法の法則と通常の位相を装備した M 集合 $\mathbf{R}_+$ を考えてみましょう。 P を、C によって誘導された位相と、C の加法によって誘導された法則を備えた、正の実数部分を持つ複素数 z の集合とする。すべての $p \in P$ について、$\mathbf{R}_+$ の $f(p)$ 指標 $x \mapsto e^{-px}$ で表します。 $f$ が P のトポロジカルモノイド構造の同型を X のモノイド上に重ねたものであることは簡単に検証されます。 $f$ によって P と同一視する X を実行します。 $\mathbf{R}_+$ が P と Th の完全な部分モノイドであることは明らかです。 3 では次の結果が得られます。

#### 命題 16 {#int-ix-s5-prop-16 .statement tag=09RS}

※Aにフィルター$\mathscr{F}$を装着した集合とします。すべての $\alpha \in A$ について、$\mu_\alpha$ を $\mathbf{R}_+$ の有界正の測度とし、$\Phi_\alpha$ を $\Phi_\alpha(p) = \int_0^{+\infty} e^{-px} d\mu_\alpha(x)$ によって $\mathbf{R}_+$ に定義された写像とします。 位数では、写像 $\alpha \mapsto \mu_\alpha$ が $\mathscr{F}$ に関して有界正測度 $\mu$ にしっかりと収束しますが、$\Phi_\alpha$ が$\mathscr{F}$ に関して$\mathbf{R}_+$ に点的に収束して写像に収束することが必要かつ十分です。 $\Phi$ は点 0 で連続します。この場合、すべての $p \in \mathbf{R}_+$ に対して $\Phi(p) = \int_0^{+\infty} e^{-px} d\mu(x)$ です。*

加法モノイド $\mathbf{R}_+^n$ ($n$ 整数 $> 1$) についても同様の結果があります。 Th の転写は読者に任せます。この場合は 3 です。

### 練習問題 {#int-ix-s5-exercises}

[§ 5 に対して練習問題](exercises/s5/)を参照してください。
