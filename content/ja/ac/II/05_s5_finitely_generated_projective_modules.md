---
book: ac
book_title: Commutative Algebra
chapter: II
chapter_title: LOCALIZATION
section: 5
section_title: Finitely generated projective modules. Invertible fractional ideals
lang: ja
source: ac-i-vii
book_pages: 108-120, 146-153
pdf_pages: 0128-0140, 0166-0173
extraction: ocr
subsections:
    - "no": 1
      title: LOCALIZATION WITH RESPECT TO AN ELEMENT
      page: 108
      pdf_page: 128
    - "no": 2
      title: LOCAL CHARACTERIZATION OF FINITELY GENERATED PROJECTIVE MODULES
      page: 109
      pdf_page: 129
    - "no": 3
      title: RANKS OF PROJECTIVE MODULES
      page: 111
      pdf_page: 131
    - "no": 4
      title: PROJECTIVE MODULES OF RANK 1
      page: 114
      pdf_page: 134
    - "no": 5
      title: NON-DEGENERATE SUBMODULES
      page: 116
      pdf_page: 136
    - "no": 6
      title: INVERTIBLE SUBMODULES
      page: 117
      pdf_page: 137
    - "no": 7
      title: THE GROUP OF CLASSES OF INVERTIBLE MODULES
      page: 119
      pdf_page: 139
statements: 34
exercises: 25
content_sha256: fb0ce43254e4342a284be0f5b696180c9c77c60d6229f8bd610c4fbd9e9857c3
translated_from: content/en/ac/II/05_s5_finitely_generated_projective_modules.md
translation_method: google
source_content_sha256: 39903d36e71fd82b177991bd175a5a56543cc66eaadad8c82a42b81dab501389
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-eeeca2ef
glossary_version: 34
glossary_terms_sha256: 5326f9dde4e6efc7feee5dbb1e46350b09afb9e9ae1a7da89ca7d283a60e1844
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## 5. 有限生成射影加群。可逆的な分数イデアル

### 1. 元に関するローカリゼーション

$A$ を環 、$M$ を $A$ モジュールとします。 元 $f \in A$ ごとに、$A_f = A[f^{-1}], M_f = M[f^{-1}] = M \otimes_A A[f^{-1}]$ (§ 2、番号 1 と 2) を書きます。 $n \geq 0$ に対して $S_f$ が集合オフ」の場合、$A_{S_f} = S_f^{-1}A, M_{S_f} = S_f^{-1}M$ です。$A$ で ff が可逆である場合、$A_f$ (それぞれ $M_f$) は$A$ (それぞれ $M$) と標準的に識別されます。iff はゼロポテントです。次に、$A_f = 0$ と $M_f = 0$ それぞれの $A$ モジュール準同型 $u : M \to N$ に対して、$u_f = u \otimes 1 : M_f \to N_f$ を書き込みます。

$g$ を $A$ の他の元とします。 $A_g$ (それぞれ $M_g$) は正規的に $(A_f)_{g/1}$ (それぞれ $(M_f)_{g/1}$) と識別されます。ここで、$g/1$ は $A_g$ の $g$ の像であり、$u_{f,g}$ は $(u_f)_{g/1}$ となります。 (§ 2, no. 3、命題 7)。

#### 命題 1 {#ac-ii-s5-prop-1 .statement tag=04BE}

※$f$を環$A$と$\phi : A \to A_f$、標準写像の元とします。 写像 $^a\phi : \operatorname{Spec}(A_f) \to \operatorname{Spec}(A)$ は、$X = \operatorname{Spec}(A)$ (§ 4, no. 3) の開部分空間 $X_f$ に対する $\operatorname{Spec}(A_f)$ の同写写像です。*

これは、§ 4, no. 3、系 ～ 命題 13 の特定のケースです。

#### 命題 2 {#ac-ii-s5-prop-2 .statement tag=04BF}

*$A$を環、$u : M \to N$を$A$モジュール準同型、$p$を$A$の主な理想とします。

(i) $u_p : M_p \to N_p$ が全射的であり、$N$ が有限生成されると仮定します。そして、$u_f : M \to N$が全射となるような$f \in A - p$が存在します。

(ii) $u_p$ が全単射であり、$M$ が有限生成され、$N$ が有限に提示されると仮定します。そして、$u_f$が全単射となるような$f \in A - p$が存在します。

$R$ と $Q$ を $u$ の核と余核とします。 $u_g$ の $g \in A$、核、余核 (それぞれ $u_p$) が $R_g$ と $Q_g$ (それぞれ $R_p$ と $Q_p$) である場合 (§ 2, no. 4、定理 1)。それから$Q_p = 0$; $N$ は有限に生成されるので、$Q$ も有限に生成され、$g'Q = 0$ (§ 2, no. 2、系 2 ～ 命題 4)、よって $Q_{g'} = 0$ のような $g' \in A - p$ が存在します。 (ii) の仮説の下では、数列 $0 \to R_{g'} \to M \to N \to 0$ は正確であるため、$R_{g'}$ は有限に生成されます (章 I, § 2, no. 8, 補題 9)。さて、

$$
(R_{g'})_{pR_{g'}} = R_p = 0;
$$

したがって、$g_1 R_{g'} = 0$ (§ 2, no. 2、系 2 から命題 4) となるような $g_1 \in A, - pA_{g'}$ が存在します。次に $g_1 = g''/{g'}^h$、ここで $g'' \in A - p$; $g'/1$ は、$R_{g'}$、$(g''/1)R_{g'} = 0$、よって $R_{g'g''} = (R_{g'})_{g''/1} = 0$ では反転可能です。 $f = g'g''$、$f \in A - p$、$Q_f = 0$、$R_f = 0$ の場合、$u_f$ は全単射になります。

#### 系 {#ac-ii-s5-n1-cor-1 .statement tag=04BG}

*$N$ が有限に提示され、$N_p$ が階数 $p$ の空き $A_p$ モジュールである場合、$N$ が階数の空き $A_f$ モジュールであるような $f \in A - p$ が存在します。 $p$.*

無料の $A_,-$ モジュール $N_p$ の $x_i/1$ 形基底のように、仮定 $p$ 元 $x_i \in \mathbf{N}$ ($1 \leq i \leq p$) が存在します。 $u(e_i) = x_i$ が $1 \leq i \leq p$ であり、$(e_i)_{1 \leq i \leq p}$ が $A^p$ の標準基底となるような準同型 $u : A^p \to \mathbf{N}$ を考えてみましょう。 $u_p$ は仮定によって全単射であるため、命題 2 により $u_f$ が全単射となるような $f \in A - p$ が存在します。

#### 命題 3 {#ac-ii-s5-prop-3 .statement tag=04BH}

*$(f_i)_{i \in I}$ *を環* $A$ の元の有限族とし、*生成するを理想* $A$ *の* $A$ とします。 *環* $B = \prod_{i \in I} A_i$、*忠実にフラット* $A$*-モジュール* になります。

§ 2までに、いいえ。 **4**、定理 1、それぞれの $A_i$ はフラット $A$ モジュールであるため、$B$ (章 I, § 2, no. 3、命題 2) も同様です。一方、$p$ が $A$ の素イデアルである場合、添字 $i$ が存在するため、$f_i \notin p$ と $p_{f_i} = pA_{f_i}$ は $A_{f_i}$ の素イデアルになります。その後、$pA_{f_i} \neq A_{f_i}$ から $pB \subset pA_{f_i} \times \prod_{j \neq i} A_j \neq B$ になります。これは、$B$ が忠実にフラットな $A$ モジュール (章 I, § 3, no. 1, 命題 1) であることを暗示するのに十分です。

#### 系 {#ac-ii-s5-n1-cor-2 .statement tag=04BI}

*命題 3 の仮説の下では、* $A$* モジュール* $M$ * が有限に生成される (それぞれ有限に提示される) ために、すべての添字* $i$ に対して、* $A_{f_i}$* モジュール* $M_{f_i}$ * が有限に生成されることが必要かつ十分です(それぞれ有限に提示)*。

条件は明らかに必要です (§ 2、いいえ **4**)。 Conversely, if all the $M_{f_i}$ are finitely generated (resp. finitely presented), $M' = \prod_{i \in I} M_{f_i}$ is a finitely generated (resp. finitely presented) $B$-module, for we can obviously suppose that for each $i$ there is an exact sequence $AT_i \to A^n_{f_i} \to M_{f_i} \to 0$, where $m$ and $n$ are *independent of* $i$. さて、$M' = M \otimes_A B$。 系は、命題 3 と章 I, § 3 から続きます。いいえ。 **6**、命題 11.

$f_i$ の条件は、オープン集合 $X_{f_i}$ 形が $\mathrm{Spec}(A)$ (§ 4, no. 3、系 3 から命題 11) を *カバー* することを意味することに注意してください。

### 2. ローカル特徴付け/有限生成射影加群

#### 定理 1 {#ac-ii-s5-thm-1 .statement tag=04BJ}

* $A$ * を環とし、* $P$ * $A$ * モジュール* とします。 *次のプロパティは同等です*:

(a) $P$ * は有限生成射影加群* です。
(b) $P$ *は有限に提示された加群であり、$A$ のすべての最大理想* $m$ に対して、$P_m$ * は自由* $A_m$* モジュール* です。
(c) $P$ *は有限生成加群、すべての* $p \in \mathrm{Spec}(A)$、*$A_p$*モジュール* $P_p$ *は自由で、その階数を* $r_p$で表すと、*写像* $p \mapsto r_p$ *はトポロジカルで局所的に定数である空間* $\mathrm{Spec}(A)$ *(つまり、* $\mathrm{Spec}(A)$ の点ごとに、この写像が定数である近傍が認められます)*。

(d) There exists a finite family $(f_i)_{i \in I}$ of elements of $A$, generating the ideal $A$, such that, for all $i \in I$, the $A,$-module $P_{f_i}$ is free with finite rank.

(e) $A$ のすべての最大理想 $m$ に対して、$P_f$ が有限階数の自由な $A,$ 加群となるような $f \in A - m$ が存在します。

定理を証明で次の含意スキームを示します。

(a) ⇔ (d)

(b) ⇌ (e)

(c)

(a) ⇒ (b): 有限生成射影加群は有限であることがわかります (章 I, § 2, no. 8, 補題 8 (iii))。 $P$ が射影 $A$ 加群の場合、$P_m = P \otimes_A A_m$ は射影 $A_m$ 加群 (\emph{代数}、章 II, § 5, no. 1、系 ～ 命題 4)。最後に、$A_m$ が局所環であるため、有限に提示された射影 $A_m$ モジュールはすべて自由です (§ 3, no. 2、系から命題 5)。

(b) ⇒ (e): no. 1の系から命題2まで続きます。

(c) ⇒ (e): $m$ を $A$ の最大理想とする。 $r_m = n$と書き、$(x_i)_{1 \leq i \leq n}$を$P$の基底とします。 We can assume that the $x_i$ are canonical images of elements $p_i \in P$ $(1 \leq i \leq n)$ to within multiplication by an invertible element of $A,$. $(e_i)_{1 \leq i \leq n}$ を $A^n$ と $u : A^n \to P$ 準同型の標準基底として、$1 \leq i \leq n$ が $u(e_i) = p_i$ になるようにします。 $P$ は有限生成されるため、no. 1 の命題 2 から、$u_f$ が全射となるような $f \in A - m$ が存在することがわかります。 We conclude that $u_{f,g}$ is also surjective for all $g \in A - m$ and by hypothesis there exists $g \in A - m$ such that $r_p = n$ for $p \in X,$. 次に、$f g$によって置き換えること $f$、すべての$p \in X,$に対して$r_p = n$と仮定できます。 この場合、$u_p : A_p^n \to P_p$ は全射準同型であり、$P_p$ と $A_p$ はどちらも同じ階数の空き $A,$ モジュールです。従って (§ 3, no. 2, 系から命題 6) $u_p$ はすべての $p \in X_f$ に対して全単射です。 $p'$ を $A,$ の主理想とし、$p$ を標準写像の下の $A$ の逆像とします。 $(A_f^{n})_{p'}$ と $(P_f)_{p'}$ が標準同型の下で $A_p^n$ と $P_p$ と同一視される場合、$(u_f)_{p'}$ は $u_p$ と同一視され、その結果全単射となります。 $u_f$ は全単射 (§ 3, no. 3, 定理 1) であると結論する判断し、(e) が成立します。

(e) ⇒ (d): $P_f$ が有限生成された自由な $A_f$ モジュールとなるように、$E$ を $\in A$ からオフにする集合とします。 仮定は、$E$が$A,$の極大理想に含まれていないため、$E$生成する理想$A$が存在し、したがって$E$と$a_i \in A$の元の有限族$(f_i)_{1 \leq i \leq n}$が存在することを意味します。 $(1 \leq i \leq n)$ は $1 = \sum_{i=1}^n a_i f_i$ になります。 よって (d)。

(d) ⇒ (c): no. 1, 系から命題 3 より、$P$ が有限生成されることがわかります。一方、$A$ のすべての素イデアル $p$ に対して、$p \in X_{f_i}$ となるような添字 $i$ が存在します。 $p' = p_{f_i}$ の場合、$P_p = (P_{f_i})_{p'}$ (§ 2, no. 5、命題)

10) したがって、仮定により $P_p$ は自由であり、$P_{f_i}$ と同じ階数であり、これは (c) を証明します。

(d) ⇒ (a): 環 $B = \prod_{i \in I} A_i$ と B-加群を検討します
$$
M = \prod_{i \in I} P_i = P \otimes_A B.
$$
すべての添字 $i$ に対して、$P_i$ が $L$ の直因子となるように、自由な $A_i$ モジュール $L$ が存在し、すべての $L$ が同じ階数を持つと仮定できます。その場合、$L = \prod_{i \in I} L_i$ は自由な B-加群であり、その M は直因子であり、他の語 M は有限生成された射影 B-加群です。 As B is a faithfully flat A-module (no. 1, Proposition 3), we conclude that P is a finitely generated projective A-module (Chapter I, §3, no. 6, Proposition 12).

#### 系 1 {#ac-ii-s5-thm-1-cor-1 .statement tag=04BK}

定理 1 の主張の等価な性質が成り立つと仮定します。 m を整数 > 0 として、P の元の各ファミリー $(x_i)_{1 \leq i \leq m}$ に対して、A の元のファミリー $(a_i)_{1 \leq i \leq m}$ が存在しますが、そのすべてが零の因子であり、その$\sum_{i=1}^m a_i x_i = 0$ であるわけではありません。次に、$p \in \operatorname{Spec}(A)$、$r_p \leq m$ についてです。

p を A の素イデアルとする。 集合 $r = r_p$ とし、$(y_j)_{1 \leq j \leq r}$ を無料の $A_p$ モジュール $P_p$ の基底とします。 すべての $j$ に対して $y_j = x_j / s$ となるような P と $s \in A - p$ の元 $x_j$ ($1 \leq j \leq r$) が存在します。 次に、A の各家族 $(a_j)_{1 \leq j \leq r}$ の元について、$\sum_{j=1}^r a_j x_j = 0$、$\sum_{j=1}^r (a_j/1) y_j = 0$ が $P_p$、よって $a_j/1 = 0$ が $1 \leq j \leq r$ になるようにします。 $A - p$ は含む 0 ではないので、これは、$a_j$ がすべて A (§ 2, no. 1、注意 3) の零の因子であることを示しており、したがって $r \leq m$ が必要です。

#### 系 2 {#ac-ii-s5-thm-1-cor-2 .statement tag=04BL}

有限に提示されるすべての平面加群は射影的です。

P が有限に提示された平坦 A-加群であり、A の最大イデアルである場合、$A_m$ 加群 P は平坦 (§ 3, no. 4、命題 13) で有限に提示 (§ 2, no. 4) するため自由 (§ 3, no. 2、系 2 から命題 5)、したがって、定理 1 の条件 (b) が成り立ちます。

注意
(1) 射影ではない有限生成平面加群が存在する (練習問題 7)。
(2) 非可換リング上で系 2 ～ 定理 1 拡大する ～ 加群 (章 I, §2、練習問題 15)。

### 3. 射影加群中階数

#### 定義 1 {#ac-ii-s5-def-1 .statement tag=04BM}

P を有限生成射影 A-加群とします。 A のすべての素イデアル $p$ に対して、自由 $A_p$ 加群 $P_p$ の階数は、$p$ における P の階数と呼ばれ、$\operatorname{rg}_p(P)$ で表されます。

定理 1 により、整数値の写像 $p \mapsto \mathrm{rg}_p(P)$ は $X = \mathrm{Spec}(A)$ 上で *局所的に定数* になります。したがって、$X$ が *接続* されている場合、特に環 $A$ が *整域* (§ 4, no. 3、系 2 ～ 命題 15) である場合、定数となります。

#### 定義 2 {#ac-ii-s5-def-2 .statement tag=04BN}

*$n$を整数$\geqslant 0$とします。射影 $A$ 加群 $P$ は、有限生成される場合は *of 階数* $n$ であり、すべての素イデアル $A$ の $p$ については $\mathrm{rg}_p(P) = n$ であると言われます。

明らかに、有限で生成されたすべての *自由* $A$ モジュール $L$ は、定義 2 の意味で階数 $n$ であり、$n$ は、で定義された $L$ の *次元* (または *階数*) に等しい*代数*、章 II, § 7, no. 2。

階数 0 の射影加群は零 (§ 3, no. 3、系 2 ～ 定理 1) です。 $A$ が 0 に減らされず、射影 $A$ 加群 $P$ が階数 $n$ である場合、整数 $n$ は一意に決定されます。この場合、それは $\mathrm{rg}(P)$ で示されます。

#### 定理 2 {#ac-ii-s5-thm-2 .statement tag=04BO}

*Let $P$ be an $A$-module and $n$ an integer $\geqslant 0$. 次のプロパティは同等です:*

(a) *$P$ は階数* $n$ の射影です。

(b) *$P$ は有限に生成され、すべての最大理想* $m$ *of* $A$、*the* $A$-*加群* $P$、*は階数* $n$ を含まない。

(c) *$P$ は有限に生成され、すべての素イデアル* $p$ *of* $A$ に対して、*the* $A$-*加群* $P_p$ *は階数* $n$ を含まない。

(d) *すべての最大理想* $A$ の $m$ に対して、 * $A$-*加群* $P_f$ * 階数* $n$ が含まれないような * $f \in A - m$ が存在します。

定義 2 と定理 1 により、(a) と (c) は同等です。 (b) は (c) を暗示します。なぜなら、$A$ のすべての素イデアル $p$ に対して、最大イデアル $m$ 含む $p$ が存在し、$p' = p_m$, $P_p$ と書くと $(P_m)_{p'}$ (§ 2, no. 5, 命題) と同型です。 11); $P_m$ に階数 $n$ が含まれない場合、$P_{p'}$ です。 性質 (c) は、定理 1 と、$\in A - m$ と $m' = m_f$ を除いて、$P_m$ は $(P_f)_{m'}$ と同型であるため、$P_f$ と $P$ の階数は等しいという事実により、(d) を暗示します。最後に、この最後の引数と定理 1 は、(d) が (b) を意味することを示しています。

#### 注意 {#ac-ii-s5-n3-rem-1 .statement tag=04BP}

*もし* $A$ *が整域であれば、射影* $A$-*加群は明確に定義された階数* (定義 2 の意味で) を認めます。さらに、この階数一致するには代数、章 II, § 7, no. 2 で定義された階数が含まれます。 定理を適用する 2 (c) with* $p = (0)$ だけで十分です。

$E$ と $F$ を 2 つの有限生成射影 $A$ 加群とする。私たちは (*代数*、章 II, §§ 2、および 3) $E \times F$、$E \otimes_A F$、$\mathrm{Hom}_A(E, F)$、および $E$ の双対 $E^*$ が射影的で有限生成されることを知っています。すべての整数 $k > 0$ (*代数*、章 111) の外装冪 $\bigwedge^k E$ も同様です。また、定義 1 と § 2, no. 7、命題 18 と 19 と no. 8 から、$A$ のすべての素イデアル $p$ について、次のことがすぐに続きます。

(1)
$$
\mathrm{rg}_p(E \times F) = \mathrm{rg}_p(E) + \mathrm{rg}_p(F)
$$

(2) $\mathrm{rg}_p(E \otimes_A F) = \mathrm{rg}_p(E) \cdot \mathrm{rg}_p(F)$

(3) $\mathrm{rg}_p(\mathrm{Hom}_A(E, F)) = \mathrm{rg}_p(E) \cdot \mathrm{rg}_p(F)$

(4) $\mathrm{rg}_p(E^*) = \mathrm{rg}_p(E)$

(5) $\mathrm{rg}_p(\wedge^k E) = \binom{\mathrm{rg}_p(E)}{k}$。

E と F の階数が定義されると、$E \times F, E \otimes_A F,$ $\mathrm{Hom}_A(E, F), E^*$ と $\wedge^k E$ も定義され、添字 $p$ を省略しても上記の式が成り立ちます。さらに:

#### 系 {#ac-ii-s5-n3-cor-1 .statement tag=04BQ}

*有限生成射影 A-加群 P が階数 n であるためには、 $\mathbf{A}^n P$ が階数 1 であることが必要かつ十分です。*

#### 命題 4 {#ac-ii-s5-prop-4 .statement tag=04BR}

*B を可換 A-代数とし、P を階数 n の射影 A-加群とします。 B-加群 $P_{(B)} = B \otimes_A P$ は階数 n の射影になります。*

$P_{(B)}$ は射影的であり、有限に生成されることがわかっています (*代数*、章 II, § 5, no. 1、系 ～ 命題 4)。 q が B の素イデアルであり、p が A の逆像である場合、

$$
(P_{(B)})_q = (P \otimes_A B) \otimes_B B_q = P @_A B_q = (P \otimes_A A_i) \otimes_A B_q
$$

そして、仮定によると、$P \otimes_A A_i$ は階数 $n$ の無料の A, モジュールであり、$(P_{(B)})_q$ は階数 $n$ の無料の $B_q$ モジュールです。

#### 命題 5 {#ac-ii-s5-prop-5 .statement tag=04BS}

*A を半局所環、P を有限生成射影 A-加群とします。 P の階数が定義されている場合、P は自由A-加群となります。*

まず、A が体 $K_i$ ($1 \leq i \leq n$) の積と同型であると仮定します。 次に、$K_i$ は A の最小理想 (*代数*、章 VIII, § 3, no. 1) と同一視され、K のすべての $i$、和 $p_i$、添字 $j \neq i$ は A の最大理想、$p_i$ と同一視されます。 ($1 \leq i \leq n$) は A の唯一の主要な理想です。 Every finitely generated A-module P is therefore the direct sum of its isotypical components $P_i$ ($1 \leq i \leq n$), $P_i$ being isomorphic to a direct sum of a finite number $r_i$ of A-modules isomorphic to K, (*Algebra*, Chapter VIII, § 5, no. 1, Proposition 1 and no. 3, Proposition 11); the ring $A_{r_i}$ is identified with K, and annihilates the $P_j$ of index $j \neq i$, hence $r_i = \mathrm{rg}_{p_i}(P)$; if all the $r_i$ are equal to the same number $r$, P is isomorphic to $A^r$, whence the proposition in this case. 一般的な場合、$\mathfrak{R}$ を A と $B = A / \mathfrak{R}$ のジェイコブソン根基とします。 B が体の積であるため、射影 B-加群 $P_{(B)}$ は命題 4 に先行する注意によって自由になります。 *また、P はフラット A-加群と命題であり、その後 § 3, no. 2、命題 5 から続きます。*

### 4. 射影加群/階数 1

#### 定理 3 {#ac-ii-s5-thm-3 .statement tag=04BT}

$A$ を環および $M$ を任意に生成した $A$ モジュールとします。

(i) *$M \otimes_A N$ が $A$ と同型であるような $A$ 加群 $N$ が存在する場合、加群 $M$ は階数 1 の射影です。*

(ii) *逆に、$M$ が階数 1 の射影であり、$M^*$ が $M$ の双対である場合、$M \times M^*$ 上の正規の双線形形式 $(x, x^*) \to \langle x, x^* \rangle$ に対して、標準準同型 $u : M \otimes_A M^* \to A$ 対応する (代数, 章 II, § 2, no. 3) は全単射です*。

(i) $A$ のすべての最大理想 $m$ について、$A_m$ 加群 $M$ には階数 1 (定理 2 (b)) が含まれないことを証明する必要があります。 $A_m$ によって置き換える $A$ を自由に実行できるため、$A$ が *ローカル* 環 ($§ 2$、no. 7、命題 18) であると想定できます。 $k = A/m$ にしましょう。 同型 $v : M \otimes_A N \to A$ 定義する同型

$$
v \otimes 1_k : (M/mM) \otimes_k (N/mN) \to k
$$

$(M/mM) \otimes_k (N/mN)$ の $k$ 上の階数は $M/mM$ と $N/mN$ の階数の積であるため、これら後者は必ず 1 に等しく、他の語 $M/mM$ は単次です。したがって、$M$ は単次 ($§ 3$、no. 2、系 2 ～ 命題 4) です。一方、$M$の消滅子も$M \otimes_A N$を消滅させるため、零となり、$M$が$A$と同型であることが証明されます。

(ii) $A$ のすべての最大理想 $m$ に対して、$u_m$ は同型 ($§ 3$, no. 3, 定理 1) であることを証明すれば十分です。 $M$ は有限に提示されるため (章 I、$§ 2$、no. 8、補題 8)、$(M^*)_m$ は二重の $(M_m)^*$ ($§ 2$、no. 7、 命題 19) そして、$M_m$ は双対の $(M_m)^*$ と同様に階数 1 を含まないので、明らかに標準準同型 $u_m : (M_m) \otimes_{A_m} (M_m)^* \to A_m$ は全単射であり、証明を完成します。

*注意* (1)。 $M$ が階数 1 の射影であり、$N$ が $M \otimes_A N$ が $A$ と同型である場合、$N$ は $M^*$ と同型です: 同型があります

$$
N \to N \otimes A \to N \otimes M \otimes M^* + A \otimes M^* \to M^*.
$$

#### 命題 6 {#ac-ii-s5-prop-6 .statement tag=04BU}

*$M$と$N$を階数1の射影$A$加群とする。すると、$M \otimes_A N$、$\operatorname{Hom}_A(M, N)$と$M$の双対$M^*$は階数1の射影となる。

これは、式 (2)、(3)、および (4) からすぐに得られます。

Let us now note that every finitely generated $A$-module is isomorphic to a quotient module of $L = \mathbf{A}^{(\mathbf{N})}$; we may therefore speak of the *set $F(A)$ of classes of finitely generated $A$-modules* with respect to isomorphism (*Set Theory*, Chapter I, §6, no. 9); we denote by $P(A)$ the subset of $F(A)$ consisting of the classes of projective $A$-modules of rank 1 and by $\operatorname{cl}(M)$ the image in $P(A)$ of a projective $A$-module $M$ of rank 1. 2 つの射影 $A$ 加群 $M$ に対して、それは明らかです。

階数 1 の N、cl(M \otimes_A N) は cl(M) と cl(N) にのみ依存します。 定義私たち集合として

(6) $$ \mathrm{cl}(M) + \mathrm{cl}(N) = \mathrm{cl}(M \otimes AN) $$

したがって、合成の内部法則は $P(A)$ に定義されます。

#### 命題 7 {#ac-ii-s5-prop-7 .statement tag=04BV}

*階数 1 の射影 A-加群の類の集合 $P(A)$ は、合成 (6) の法則と可換群です。 M が階数 1 の射影 A-加群で、$M^*$ がその双対である場合、*

(7) $$ \mathrm{cl}(M^*) = -\mathrm{cl}(M) \quad \text{and} \quad \mathrm{cl}(A) = 0. $$

The associativity and commutativity of the tensor product show that the law of composition (6) is associative and commutative; the isomorphism between $A \otimes_A M$ and M prove that $\mathrm{cl}(A)$ is the identity element under this law and, by virtue of Theorem 3, $\mathrm{cl}(M) + \mathrm{cl}(M^*) = \mathrm{cl}(A)$, whence the proposition.

B を可換 A-代数とし、M を階数 1 の射影 A-加群とします。この場合、$M_{(B)} = B \otimes_A M$ は階数 1 (no. 3, 命題 4) の射影 B-加群です。次に、次のような正規 $\phi : P(A) \to P(B)$ と呼ばれる写像が存在します。

(8) $$ \phi(\mathrm{cl}(M)) = \mathrm{cl}(M_{(B)}). $$

2 つの A-加群 M, N に対する方程式 $M_{(B)} \otimes_B N_{(B)} = (M \otimes_A N)_{(B)}$ は、写像 $\phi$ が可換群 *準同型* であることを証明します。

*注意 (2).* 定理 1 の条件 (e) (P が射影で有限生成されるという事実と同等) は、$X = \mathrm{Spec}(A)$ 上の加群* $\tilde{P}$ の *束 P が局所的に自由で有限であるというというによっても表現できます。 型* であるため、ベクトルの束が X に束ねられた切断の束として解釈できます。 逆に、X を超えるすべてのベクトルバンドルは有限生成射影加群から生じ、一意の同型内に決定されます。 階数 $n$ の射影加群は、したがって対応するからベクトルの束となり、そのすべてのファイバーは次元 $n$ を持ちます。 特に、階数 1 対応する ～ 射影加群の階数 1 のベクトルバンドル。 If we denote by $\mathscr{O}_X$ the structure sheaf $\tilde{A}$ and by $\mathscr{O}_X^*$ the *sheaf of units* of $\mathscr{O}_X$ (whose sections over an open set U of X are the invertible elements of the ring of sections of $\mathscr{O}_X$ over U), it follows that the group $P(A)$ is isomorphic to the first cohomology group $H^1(X, \mathscr{O}_X^*)$.*

(* A. Grothendieck、Éléments de géométrie algébrique、I (§ 1) (Publ. Math. I.H.E.S.、no. 4、1960) を参照。

### 5. 非退化部分加群

このNo.そしてそれに続く2つ、$A$は環、$S$は$A$の零の因子ではない$A$のからなる、元の乗算部分集合、および$B$を表します。 環 $S^{-1}A$; $A$ は、標準的に $B$ の部分環 ($§ 2$、no. 1、注意 3) と識別されます。したがって、$S$ の元は、$B$ で反転可能です。

アプリケーションの最も重要な特殊ケースの 1 つは、$A$ が整域で、$S$ が元の $\neq 0$ $A$ の集合である場合です。 $B$ は、$A$ の分数の体になります。

#### 定義 3 {#ac-ii-s5-def-3 .statement tag=04BW}

$M$ を $B$ のサブ A モジュールとします。 $M$ が $B.M = B$ の場合、非縮退と呼ばれます。

$B$ が体の場合、この条件は単に $M$ が 0 に減らないことを意味します。

#### 命題 8 {#ac-ii-s5-prop-8 .statement tag=04BX}

$M$ を $B$ のサブ A モジュールとします。次の条件は同等です。
(a) $M$ は非縮退です。
(b) $M$ は $S$ と一致します。
(c) $j : M \to B$ が標準単射の場合、準同型 $u = S^{-1}j : S^{-1}M \to B$ は全単射です。

(a) は (b) を暗示します。なぜなら、$B.M = B$ の場合、$(a/s)x = 1$ となる$a \in A, s \in S$ と $x \in M$ が存在するため、$ax = s$ 属するから $S \cap M$ になります。 (b) が (c) を意味していることを確認するには、$u$ がすでに単射法 ($§ 2$, no. 4, 定理 1) であることに注意してください。さらに、$B$ の $x/x \in S^{-1}M$ の $u$ の下の $x \in M \cap S$、像が 1 に等しい場合、$u$ は全射です。最後に、(c) は明らかに (a) を意味します。

#### 系 {#ac-ii-s5-n5-cor-1 .statement tag=04BY}

$M$ と $N$ が $B$ の 2 つの非縮退サブ A モジュールである場合、A-加群 $M + N, M.N$ と $M \cap N$ は非縮退です。

$M + N$ にとって主張は簡単です。一方、$s \in S \cap M$ と $t \in S \cap N$ の場合は、$st \in S \cap (M.N)$ と $st \in S \cap (M \cap N)$ になります。

$B$ の 2 つのサブ A モジュール $M$ と $N$ を考えると、それら $b \in B$ のうち $B$ からなるのサブ A モジュールを $N : M$ で表して、$bM \subset N$ (章 I, $§ 2$、no. 10、注意）。 $M$ ～ $N$ の$b \in N : M$ をすべて準同型 $h_b : x \mapsto bx$ にマッピングすると、$N : M$ ～ $\operatorname{Hom}_A(M, N)$ から標準準同型 $b \mapsto h_b$ が得られます。

#### 命題 9 {#ac-ii-s5-prop-9 .statement tag=04BZ}

$M, N$ を $B$ の 2 つのサブ A モジュールとします。 $M$ が非縮退であれば、$N : M$ から $\operatorname{Hom}_A(M, N)$ までの標準準同型は全単射です。

$s \in S \cap M$ にしましょう。 $b \in N : M$ がすべての $x \in M$ に対して $bx = 0$ となる場合、$s$ は $B$ の 0 の因子ではないため、$bs = 0$、よって $b = 0$ となります。一方、$f \in \mathrm{Hom}_A(M, N)$ と集合 $b = f(s)/s$ としましょう。すべての $x \in M$ に対して、$tx \in A$ となるような $t \in S$ が存在します。それから
$$
f(x) = s^{-1}t^{-1}f(stx) = s^{-1}t^{-1}txf(s) = bx,
$$
よって $b \in N : M$ と $f = h_b$ は、命題を証明します。

#### 注意 {#ac-ii-s5-n5-rem-1 .statement tag=04C0}

特に、$A : M$ は、$M$ の二重 $M^*$ と正規的に識別され、$M \times M^*$ の正規の双線形形式は、乗法 $B \times B \to B$ の制限から $M \times (A : M)$ と識別されます。

### 6. インバーチブル部分加群

(記法と no. 5 を保持します。)

#### 定義 4 {#ac-ii-s5-def-4 .statement tag=04C1}

$M.N = A$ のような $B$ の *サブ*-A モジュール $N$ が存在する場合、$B$ の *サブ*-A モジュール $M$ は可逆的と呼ばれます。

#### 例 {#ac-ii-s5-n6-exa-1 .statement tag=04C2}

$b$ が $B$ の可逆元である場合、$N = Ab^{-1}$ を取ることでわかるように、$A$ 加群 $Ab$ は反転可能です。

#### 命題 10 {#ac-ii-s5-prop-10 .statement tag=04C3}

*$M$を可逆サブ*-A*モジュール&$B$とします。次に:
(i) $As \subset M \subset As^{-1}$ となるような $s \in S$ が存在します (特に $M$ は非縮退です)。
(ii) $A : M$ は、$M.N = A$ となる、$B$ の唯一の *サブ*-A* モジュール* $N$ です。

$M.N = A$ の場合、$B.M = B.(B.M) \supset B.(M.N) = B.A = B$、したがって $M$ は非退化です。同様に、$N$ は非退化です。 $t \in S \cap M$ と $u \in S \cap N$ (no. 5, 命題 8 ) の場合、元 $s = tu$ 属するから $S \cap M \cap N$、よって $Ms \subset M.N = A$、したがって $As \subset M \subset As^{-1}$ となります。
一方、明らかに $N \subset A : M$、よって
$$
A = M.N \subset M.(A : M) \subset A
$$
そして$M.(A : M) = A$;両辺に$N$を掛けると、$A : M = N$が導き出され、証明が完成します。

#### 定理 4 {#ac-ii-s5-thm-4 .statement tag=04C4}

*$M$を$B$の非縮退サブ*-A*モジュール*とします。 *次のプロパティは同等です*:
(a) $M$ は反転可能です。
(b) $M$ は射影です。
(c) $M$ は階数 1 の射影です。
(d) $M$ は有限生成された $A$ 加群であり、$A$ のすべての最大理想 $m$ に対して、$A_m$ 加群 $M_m$ は単次です。

まず性質(a)、(b)、(c)の同値を示しましょう。 (a) が成立し、 N が B のサブ A モジュールである場合、 M 。 N = A の場合、関係となります。

$$
\sum_{i=1}^{p} m_i n_i = 1 \quad (m_i \in M, n_i \in N \text{ for all } i).
$$

すべての $x \in M$、集合 $v_i(x) = n_i x$。 $v_i$ は M では線型形式で、すべての $x \in M$ では (9) $x = \sum_{i=1}^{n} m_i v_i(x)$ です。これは、M が射影であり、$m_i$ によって生成されることを証明します (代数, 章 11, §2, no. 6, 命題 12)。したがって、M は有限生成射影加群です。

m を A の最大理想とする。 整数 $r = \mathrm{rg}_m(M)$ が 1 に等しいことを示します。S' を $\mathbf{A}_{m'}$ の S の像とします。 Sの元はAの0の因子ではないので、$\mathbf{A}_{m'}$はフラットA-加群(§ 2, no. 4、定理1、章)であるため、S'のそれらは$\mathbf{A}_{m'}$の0の因子ではありません。 I, §2, no. 4、命題 3);次に、${S'}^{-1}A_m \neq 0$、そして、$M_m$ は階数 $r$ の空き $A_m$ モジュールであるため、${S'}^{-1}M_m$ は階数 $r$ の空き ${S'}^{-1}A_m$ モジュールです。しかし、T' が $S^{-1}A$、${S'}^{-1}A$ の A $-m$ の像である場合、(それぞれ ${S'}^{-1}M_m$) は ${T'}^{-1}(S^{-1}A)$ (それぞれ ${T'}^{-1}(S^{-1}M)$) (§ 2, no. 3、命題 7) と正規識別されます。ここで、$S^{-1}M = B$ (命題 8 (c)) であるため、${T'}^{-1}(S^{-1}M)$ は ${T'}^{-1}(S^{-1}A)$ 上の階数 1 の自由A-加群であり、これは $r = 1$ を証明し、含意 (a) $\Rightarrow$ (c) を示します。

(c) $\Rightarrow$ (b) の含意は自明です。 (b) $\Rightarrow$ (a) を示しましょう。 仮定までに、M 上の線型形式のファミリー (必ずしも有限ではない) $(f_\lambda)_{\lambda \in L}$ と、M の元のファミリー $(m_\lambda)_{\lambda \in L}$ が存在し、すべての $x \in M$ について、ファミリー $(f_\lambda(x))$ は有限台と $x = \sum_{\lambda \in L} m_\lambda f_\lambda(x)$ (代数, 章 II, §2, no. 6、命題 12）。 M は非縮退であるため、一部の $n_\lambda \in A$ に対して $f_\lambda(x) = n_\lambda x$: no. 5 の命題 9 による M です。 x を M $\cap S$ (no. 5, 命題 8) の元とすると、添字と $\sum_{\lambda \in L} m_\lambda n_\lambda = 1$ の有限の数を除いて、必然的に $n_\lambda = 0$ になることがわかります。これは明らかに M を意味します。 (A:M) = A、よって (a)。

no. 3 の定義 2 により、(c) は (d) を意味します。 逆を見せてみましょう。 M は非縮退なので、その消滅子は零 (命題 8 (b)) であり、その場合、$M_m$ の消滅子 (§ 2, no. 4, 公式 (9)) も同様です。 M は単種の & 加群であると想定されているため、階数 1 がなく、no. 3, 定理 2 から M は階数 1 の射影であることがわかります。

#### 系 {#ac-ii-s5-n6-cor-1 .statement tag=04C5}

B のすべての可逆サブモジュールはフラットであり、有限に表現されます。
これは定理 4 (c) から続きます。

#### 命題 11 {#ac-ii-s5-prop-11 .statement tag=04C6}

M、N を B の 2 つのサブ A モジュールとします。M が可逆であると仮定します。次に:
(i) 標準準同型 $M \otimes_A N \to M . N$ は全単射です。
(ii) $N : M = N . (A : M)$ および $N = (N : M) . M$。

$j$ を標準単射 $N \to B$ とします。 $M$ はフラットな $A$ 加群 (系から定理 4) であるため、$1 \otimes j : M \otimes_A N \to M \otimes_A B$ は単射です。しかし、$B = S^{-1}A$ のように、$B$ 加群 $M \otimes_A B$ は $S^{-1}M$ に等しいため、$M$ は非縮退 (no. 5、命題 8) であるため、$B$ と識別されます。この識別が行われると、$1 \otimes j$の像は$M . N$、よって(i)となります。

集合 $M' = A : M$ にしましょう。次に、明らかに $M'.N \subset N : M$ と $M.(N : M) \subset N$ です。一方、$M.M' = A$ (命題 10) 以降、

$$
N : M = M'.M.(N : M) \subset M'.N
$$

および$N = M.M'.N \subset M.(N : M)$、よって (ii)。

#### 注意 {#ac-ii-s5-n6-rem-1 .statement tag=04C7}

命題 11 の (i) の証明は、$M$ がフラットで非縮退であるという事実のみを使用します。

### 7. 群の類の反転加群

(5番と6番の記法を保存します。)

乗法では、B 形のサブ A 加群は可換モノイド $\mathfrak{m}$ であり、A は単位元です。すると、可逆加群は $\mathfrak{m}$ の可逆元なので、 形は可換群 $\mathfrak{z}$ になります。 (no. 6, 命題 10) $M \in \mathfrak{z}$ の逆数は $A : M$ であることを見てきました。

$A^*$ (それぞれ $B^*$) を A (それぞれ B) の可逆元の乗法群とし、$u$ を標準単射 $A + B$ とします。すべての $b \in B^*$、$\theta(b) = bA$ は可逆サブ A モジュールです。 写像 $\theta : B^* \to \mathfrak{g}$ は準同型で、その核は $u(A^*)$ です。その余核は $\mathfrak{c}$ または $\mathfrak{c}(A)$ で示されます。 群 $\mathfrak{c}$ は、B の可逆サブ A モジュールの類の群と呼ばれます。次の完全系列が構築されました

$$
\text{(10)} \quad (1) \longrightarrow A^* \xrightarrow{u} B^* \xrightarrow{\theta} \mathfrak{g} \xrightarrow{\rho} \mathfrak{c} \longrightarrow (1)
$$

ここで、(1) は単位元の群からなるのみを表し、$\rho$ は標準写像 $\mathfrak{g} \to \mathfrak{c} = \mathfrak{g}/\theta(B^*)$ です。

B のすべての可逆サブ A 加群 M は階数 1 (no. 6, 定理 4) の射影であるため、元 $cl(M) \in P(A)$ が定義されます (no. 4)。

#### 命題 12 {#ac-ii-s5-prop-12 .statement tag=04C8}

*写像* $cl : \mathfrak{g} \to P(A)$ *定義する、* $\mathfrak{c} = \mathfrak{g}/\theta(B^*)$ から商、同型を標準準同型の核に加えます

$$
\phi : P(A) \to P(B)
$$

(no. 4)。

他の語には完全系列があります

$$
\text{(11)} \quad (1) \longrightarrow A^* \xrightarrow{u} B^* \xrightarrow{\theta} \mathfrak{g} \xrightarrow{cl} P(A) \xrightarrow{\phi} P(B).
$$

$P(A)$のno. 6の命題11と加法の定義から、$\mathbf{3}$の$M, N$は$cl(M.N) = cl(M) + cl(N)$となり、$cl$は準同型であることがわかります。 $M \in \mathfrak{J}$ が $A$ と同型である場合、$M = Ab$ であるような $b \in B$ が存在し、$M$ が可逆であるように、$b'b = 1$ が、他の語では $b$ が $B$ で可逆であるような $b' \in B$ が存在します。 逆は明らかです。したがって、$\mathfrak{J}$の$cl$の核は$\theta(B^*)$です。

では、$cl$ の決定する像を見てみましょう。 $M \in \mathfrak{J}$ の場合、$M \otimes_A B = S^{-1}M = B$ (no. 5、命題 8 (c))、よって $cl(M) \in \mathrm{Ker}(\phi)$。 Conversely, let $P$ be a projective $A$-module of rank 1 such that $P_{(B)} = P \otimes_A B$ is $B$-isomorphic to $B$. $P$ はフラットな $A$ モジュールであるため、単射 $u : A \to B$ 定義する単射 $u \otimes 1 : P \to P_{(B)} = B$ および $P$ は、$B$ のサブ$A$ モジュールで識別されます。 no. 5 の命題 8 (c) により、$P$ は非縮退であり、no. 6 の定理 4 は $P$ が可逆であることを示しています。 したがって、$\phi$ の核は、$cl : \mathfrak{J} \to P(A)$ の像に等しいです。

#### 系 1 {#ac-ii-s5-prop-12-cor-1 .statement tag=04C9}

*B の 2 つの可逆サブ A 加群が $\mathfrak{C}$ で同じ像を持つためには、それらが同型であることが必要かつ十分です。*

#### 系 2 {#ac-ii-s5-prop-12-cor-2 .statement tag=04CA}

*If the ring $B$ is semi-local, the group $\mathfrak{C}$ of classes of invertible sub-A-modules of B is canonically identified with the group $P(A)$ of classes of projective A-modules of rank 1.*

この場合、$P(B) = 0$ (no. 3、命題 5) です。

#### 注意 {#ac-ii-s5-n7-rem-1 .statement tag=04CB}

系 2 の仮定は、次の 2 つの場合に満たされます。

(1) $A$ は整域で、$S$ は元の集合 $\neq 0$ $A$、$B$ は $A$ の分数の体になります。 $B$ の可逆サブ A 加群は、この場合 *可逆分数イデアル * とも呼ばれます。単次自由 $A$ 加群 $Ab$ ($B$ の $b \# 0$) は、*代数*、章 VI, § 1, no. 5 で定義される *分数主イデアル* にすぎません。

*(2)* 環 $A$ はネーター で、$S$ は $A$ の元の集合であり、$B$ は分数の合計環となる 0 の因子ではありません。 $A$の。この場合 $S = A - \bigcup p_i$ では、$p_i$ は $\mathrm{Ass}(A)$ (章 IV, § 1) の元 (数で有限) であるため、$B$ は準ローカル (§ 3, no. 5、命題 17) です。*

### 練習問題 {#ac-ii-s5-exercises}

[§ 5 に対して練習問題](exercises/s5/)を参照してください。
