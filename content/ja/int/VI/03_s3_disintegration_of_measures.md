---
book: int
book_title: Integration
chapter: VI
chapter_title: VECTORIAL INTEGRATION
section: 3
section_title: Disintegration of measures
lang: ja
source: int-i-vi
book_pages: INT VI.40-INT VI.51, INT VI.69-INT VI.71
pdf_pages: 0431-0442, 0460-0462
extraction: ocr
subsections:
    - "no": 1
      title: Disintegration of a measure $\mu$ relative to a $\mu$-proper mapping
      page: 40
      pdf_page: 431
    - "no": 2
      title: Pseudo-image measures
      page: 44
      pdf_page: 435
    - "no": 3
      title: Disintegration of a measure $\mu$ relative to a pseudo-image of $\mu$
      page: 45
      pdf_page: 436
    - "no": 4
      title: Measurable equivalence relations
      page: 46
      pdf_page: 437
    - "no": 5
      title: Disintegration of a measure by a measurable equivalence relation
      page: 50
      pdf_page: 441
statements: 16
exercises: 12
content_sha256: 594c799eedd88759731d1a16bc02fc64d005e99f853e841664e88b2322d146bf
translated_from: content/en/int/VI/03_s3_disintegration_of_measures.md
translation_method: google
source_content_sha256: af4e8435c165da3e46c8e743b1fe384a343285c290d2c1854e12b375334ea66b
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-dda8bbaf
glossary_version: 34
glossary_terms_sha256: 7110b4c3013bc18decea37c69b776309b4cdbbedccd3f64a1997e3ebaafc8c6c
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## § 3。対策の崩壊

### 1. $\mu$-適切な写像に対する尺度$\mu$の崩壊

T を可算基底を持つ局所コンパクト空間とします (別の語、局所コンパクト ポーランド語空間 (GT, IX, §6, No. 1))。T のすべての正の尺度に対して、積分および本質積分の概念一致する (Ch. V, §1, No. 3、Prop. 9) 一方、次のような性質があります。

#### 補題 1 {#int-vi-s3-lem-1 .statement tag=09C0}

*Y が可算基底、空間 $\mathscr{H}(Y)$ 含むの可算密部分集合を伴う局所的コンパクト空間である場合。より正確には、$\mathscr{H}(Y)$ には、写像 $\geq 0$ の可算部分集合 S からなるが存在し、$\mathscr{H}(Y)$ の写像 $f \geq 0$ ごとに、写像 $f_n \in S$ の数列が存在します。 ($n \geq 0$) は$f$ に一様に収束し、すべての $n \geq 0$ に対して $f_n \leq f_0$ になります。

なぜなら、Y は、比較的コンパクトなオープン集合の増加する数列 $(U_n)$ の和集合であり、すべての $n$ に対して $\overline{U}_n \subset U_{n+1}$ (GT、I, §9, No. 9、提案 15)。 空間 $\mathscr{H}(Y)$ は、Banach 空間 $\mathscr{H}(Y, \overline{U}_n)$ の増加する数列の和集合であり、後者のそれぞれは分離可能であることが知られています (GT、Ch. X, §3, No. 3、Th. 1)。 $S'_n$ を、$\mathscr{H}(Y, \overline{U}_n)$ では可算密集集合、$\varphi \in S'_n$ では写像 $\varphi^+$ の$S_n$ 集合、$\mathscr{H}(Y, \overline{U}_{n+1})$ では$u_n$ 写像とします。 $[0, 1]$ では値、$U_n$ では 1 に等しくなります。 $S_n$ の S 和集合と $m u_n$ の集合を、$m$ と $n$ 整数 $\geq 0$ とします。 $\mathscr{H}(Y)$ のすべての写像 $f \geq 0$ に対して、$f$ は $U_n$ のいずれかに含まれるサポートを持っているため、写像 $f_p \in S_n$ ($p \geq 1$) の数列のユニフォーム極限になります。これらの写像 $f_p$ は正の整数 $m$ によって一様に囲まれており、$f_0 = m u_n$ を取るだけで十分です。*

#### 補題 2 {#int-vi-s3-lem-2 .statement tag=09C1}

*T が可算基底を伴う局所コンパクト空間である場合、無限遠で点で 0 になる傾向がある連続数値写像のバナッハ空間 $\mathscr{K}(Y)$ は分離可能です。

この補題こそコルです。 Thさんへ。 GTの1、X, §3, No. 3。これは補題 1 からも導かれ、$\mathscr{K}(Y)$ への一様収束の位相は、部分空間 $\mathscr{K}(Y, \overline{U}_n)$ のトポロジーの直接の極限位相よりも粗いという事実に従うことがわかります。

#### 補題 3 {#int-vi-s3-lem-3 .statement tag=09C2}

— *T と X を、可算基底をもつ 2 つの局所的にコンパクトな空間、T の正の測度 $\mu$、および X の正の測度の族 $t \mapsto \lambda_t$ ($t \in T$) とします。 写像 $t \mapsto \lambda_t$ がスカラー的に $\mu$ 積分可能である場合 (位相 $\sigma(\mathscr{M}(X), \mathscr{K}(X))$ について)、族 $t \mapsto \lambda_t$ は $\mu$ 十分 ($§ 1$, No. 1, 例).*

なぜなら、補題 1 を$\mathscr{K}(X)$ に適用すると、写像 $t \mapsto \lambda_t$ が漠然と$\mu$ 可測であることがわかります ($§ 1$, No. 5、提案 13)。

#### 定理 1 {#int-vi-s3-thm-1 .statement tag=09C3}

*T と B を、可算基底、$\mu$ をもつ 2 つの局所的にコンパクトな空間とし、T の正の測度、p a $\mu$-proper 写像とする（Ch. V, §6, No. 1、デフォルト。 1) T を B に、および $\mu$ の $\nu = p(\mu)$ 像 p.次に、T に関するポジティブな尺度の $\nu$-適切な族 ($§ 1$、No. 1、例) $b \mapsto \lambda_b$ ($b \in B$) が存在し、以下の特性を持ちます。

a) すべての $b \in p(T)$ に対して $\| \lambda_b \| = 1$;

b) $\lambda_b$ は、すべての $b \in B$ について集合 $\overline{p}^{-1}(b)$ (Ch. V, §5, No. 7、定義 4) に集中しています。特に、$b \notin p(T)$ の $\lambda_b = 0$。

c) $\mu = \int \lambda_b d\nu(b)$。

さらに、$b \mapsto \lambda'_b$ ($b \in B$) が特性 b) と c) を持つ T 上のポジティブ尺度の 2 番目の $\nu$-適切な族である場合、尺度 $\nu$ については B のほぼどこでも $\lambda'_b = \lambda_b$ になります。

1) *一意性.* すべての写像 $f \in \mathscr{K}(B)$ について、p が $\mu$ 固有であるため、$f \circ p$ は $\mu$ 積分可能です (Ch. V, §6, No. 2、Th. 1)。従って、すべての写像 $g \in \mathscr{K}(T)$、写像 $t \mapsto g(t)f(p(t))$ は $\mu$ 積分可能です。 (Ch. V, §3, No. 3, Th. 1) から、ほぼすべての $b \in B$、写像 $t \mapsto g(t)f(p(t))$ は $\lambda_b$ 可積分であり、

$$
\int g(t)f(p(t)) d\mu(t) = \int d\nu(b) \int g(t)f(p(t)) d\lambda_b(t).
$$

しかし、$\lambda_b$ は $\overline{p}^{-1}(b)$ に集中しているため、すべての $b \in B$ について、$\lambda_b$ のほぼどこでも $f(p(t)) = f(b)$ が得られるため、(1) の 2 番目のメンバーは $\int f(b)\langle g, \lambda_b \rangle d\nu(b)$ に等しいことになります。 $\lambda'_b$ に対する類似の公式も成り立ちます。従って、$f \in \mathscr{K}(B)$ と $g \in \mathscr{K}(T)$ はすべて $\int f(b)\langle g, \lambda_b \rangle d\nu(b) = \int f(b)\langle g, \lambda'_b \rangle d\nu(b)$ になります。他の語では、B の 2 つの写像 $b \mapsto \lambda_b$ と $b \mapsto \lambda'_b$ を $\mathscr{M}(T)$ に変換すると、$\nu$ についてはほぼどこでも局所的にスカラー的に等しく、従って $\nu$ についてもほぼどこでも等しくなります (補題 1 と §1, No. 1、 注意 2）。

2) *家族の仮の定義* $b \mapsto \lambda_b$。すべての写像 $f \in \mathscr{L}^1(\nu)$ に対して、$f \circ p$ は $\mu$ 積分可能 (Ch. V, §6, No. 2、Th. 1) であるため、$(f \circ p) \cdot \mu$ は T 上の有界測度であり、

$$
\|(f \circ p) \cdot \mu\| = \int |f \circ p| \, d\mu = \int |f| \, d\nu = N_1(f)
$$

(Ch. IV, §4, No. 7、提案 12; Ch. V, §5, No. 3、木。 1 と §6, No. 2、Th。 1)。 その結果、$(f \circ p) \cdot \mu$ は $L^1(\nu)$ の $f$ の類 $\tilde{f}$ にのみ依存し、$\tilde{f} \mapsto (f \circ p) \cdot \mu$ は、バナッハの強力な双対である T 上の有界メジャーのバナッハ空間 $\mathscr{M}^1(T)$ への$L^1(\nu)$ の *等尺性* 線形写像であることがわかります。 空間 $\mathscr{K}(T)$、分離可能 (補題 2)。 Dunford–Pettis 定理 (§2, No. 5、Th. 1 の Cor. 2) によれば、B の写像 $b \mapsto \lambda_b$ が $\mathscr{M}^1(T)$ の単位元球に存在し、スカラー的に $\nu$ 測定可能 (位相 $\sigma(\mathscr{M}^1(T), \overline{\mathscr{K}(T)})$ について) などが存在します。つまり、写像 $f \in \mathscr{L}^1(\nu)$ ごとに、

$$
(f \circ p) \cdot \mu = \int f(b) \lambda_b \, d\nu(b),
$$

写像 $g \in \overline{\mathscr{K}(T)}$ ごとにこれを記述することもできます。

$$
\int g(t) f(p(t)) \, d\mu(t) = \int f(b) \, d\nu(b) \int g(t) \, d\lambda_b(t).
$$

$f \geq 0$ と $g \geq 0$ の場合、(3) の最初のメンバーは $\geq 0$ です。これは、$\mathscr{K}(T)$ のすべての写像 $g \geq 0$ について、メジャー $(\int g(t) \, d\lambda_b(t)) \cdot \nu$ は $\geq 0$ であるため、$b$ を除く $\int g(t) \, d\lambda_b(t) \geq 0$ であることが証明されます。 所属から $\nu$ は無視できる集合 $N(g)$ (Ch. V, §5, No. 3、コル。提案 3 の 3)。 現在、写像 $\geq 0$ の $\mathscr{K}(T)$ (補題 1) の空間 $\mathscr{K}_+(T)$ に密な数列 $(g_n)$ が存在します。 The union N of the $N(g_n)$ is $\nu$-negligible and, for $b \notin N$, we have $\int g_n(t) \, d\lambda_b(t) \geq 0$ for all $n$, therefore $\int g(t) \, d\lambda_b(t) \geq 0$ for every function $g \in \mathscr{K}_+(T)$, in other words $\lambda_b \geq 0$.

そうであれば、(3) の有効性を変えることなく、$b \in N$ ごとに 0 ずつ置き換える $\lambda_b$ を実行できます。したがって、この変更は、$b \in B$ ごとに $\lambda_b \geq 0$ となるように行われたと想定できます。

3) 公式* (3) の *拡大。

$\alpha)$ すべての写像 $f \in \mathscr{L}^1(\nu)$ について、(3) から、B の写像 $b \mapsto \lambda_b$ から $\mathscr{M}(T)$ は、測度 $|f \cdot \nu|$ および位相 $\sigma(\mathscr{M}(T), \mathscr{K}(T))$ に対してスカラー的に積分可能であることがわかります。したがって、(補題 3) 族$b \mapsto \lambda_b$ は $|f \cdot \nu|$-*適切* です。 ここで、$g$ を、T 上で定義された数値写像とし、測度 $|(f \circ p) \cdot \mu|$ に対して積分可能、つまり (Ch. V, §5, No. 3、木。 1) $t \mapsto g(t)f((p(t)))$ は $\mu$ 積分可能です。次に、(2) から Th から導かれます。 1章 V, §3, No. 3 そしてThから。 1章 V, §5, No. 3、ほぼすべての $b \in B$ について、$g$ は $\lambda_b$ に対して可積分であり、写像 (ほぼどこでも定義されている) $b \mapsto \int g(t)\, d\lambda_b(t)$ は $|f \cdot \nu|$ に対して可積分であり、公式 (3) も再び有効です。

$\beta)$ 写像 $g \in \overline{\mathscr{K}(T)}$ ごとに、(3) から$f \in \mathscr{K}(B)$ に適用され、写像 $p$ が$|g \cdot \mu|$ の尺度に適切であることがわかります (Ch. V, §6, No. 1、デフォルト。 1) $g \cdot \mu$ の$p$ の下の像は、$\nu$ に対して稠密度 $b \mapsto \int g(t)\, d\lambda_b(t)$ を含むメジャーです。 $f$ が写像であるとすると、$f \circ p$ は測度 $|g \cdot \mu|$ に対して積分可能、つまり、$t \mapsto g(t)f(p(t))$ は $\mu$ 積分可能になります (Ch. V, §5, No. 3、木。 1)、公式 (3) が再び有効になります (Ch. V, §6, No. 2、木。 1)。

4) *家族の財産* $b \mapsto \lambda_b$。 性質 $\beta)$ までに、$f = 1,\ g \in \mathscr{K}(T)$ を取ることで公式 (3) を適用できます。これは、$b \mapsto \lambda_b$ がスカラー的に $\nu$ 積分可能 (位相 $\sigma(\mathscr{M}(T), \mathscr{K}(T))$ の場合) であるため、$\nu$-*適切* (補題 3) であり、$\mu = \int \lambda_b\, d\nu(b)$ であることを証明します。

ここで、$\psi$ を $\mathscr{K}(B)$ の任意の写像とします。 性質 $\alpha)$ の条件は、$f \in \mathscr{K}(B)$ と $g = \psi \circ p$ を取ることで満たされます。なぜなら、写像 $\psi(p(t))f(p(t))$ は、$f\psi$ 属するから $\mathscr{K}(B)$ まで、$p$ は$\mu$ 可積分であるからです。 $\mu$-適切です。すると、$\psi \circ p$ はほぼすべての $b \in B$ に対して $\lambda_b$ 積分可能であり、

$$
\int f(p(t))\psi(p(t))\, d\mu(t) = \int f(b)\, d\nu(b) \int \psi(p(t))\, d\lambda_b(t);
$$

最初のメンバーは定義 $\int f(b)\psi(b)\, d\nu(b)$ です。 従って、すべての写像 $\psi \in \mathscr{K}(B)$ について、$\psi \cdot \nu$ のメジャーと稠密度 $b \mapsto \int \psi(p(t))\, d\lambda_b(t)$ のメジャーは同一であることがわかります。 その結果、（Ch. V, §5, No. 3、コル。提案 3 の 2) $b \notin N'(\psi)$ ごとに、写像 $\psi \circ p$ が $\lambda_b$ 積分可能であり、$\psi(b) = \int \psi(p(t))\, d\lambda_b(t)$ であるような、$\nu$ 無視できる集合 $N'(\psi)$ が存在します。

S を、補題 1 ($Y = B$ を含む) で示される特性を持つ $\mathscr{K}(B)$ の可算部分集合とし、$N'$ を $\psi \in S$ の $N'(\psi)$ の和集合である $\nu$ 無視可能な集合とします。 Every function $\psi \geq 0$ of $\mathscr{K}(B)$ is the uniform limit of a sequence $(\psi_n)$ of elements of S with $\psi_n \leq \psi_0$. その結果、$b \notin N'$ については、ルベーグの定理は、一方で $\psi \circ p$ が $\lambda_b$ 可積分であることを示し、他方の語では、$p$ が $\lambda_b$ 固有であること、そして他方で $\psi(b) = \int \psi(p(t))\, d\lambda_b(t)$ であることを示します。 他の項、写像 $b \mapsto \varepsilon_b$、および $b \mapsto p(\lambda_b)$ の B から $\mathscr{M}(B)$ (後者はほぼどこでも定義されています) は、$\nu$ (および位相 $\sigma(\mathscr{M}(B), \mathscr{K}(B))$) に対してスカラー的にほぼどこでも等しくなります。これらの写像は、$\nu$ (補題 1 および §1, No. 1、*注意* 2) についてはほぼどこでも等しいということになります。 最後に、$p(\lambda_b) = \varepsilon_b$、集合 $B - \{b\}$ が $\varepsilon_b$ で無視できる場合、集合 $T - \bar{p}^{-1}(B)$ は $\lambda_b$ で無視できる (Ch. V, §6, No. 2、コル。提案 2 の 2)、その他の語 $\lambda_b$ は $\overline{p}^{-1}(b)$ に集中しています。そして一方で、$\| \lambda_b \| = \int d\lambda_b = \int d((p(\lambda_b))) = \| \varepsilon_b \| = 1$ (Ch. V, §6, No. 2、木。 1)。

5) *家族の修正* $b \mapsto \lambda_b$。 従って、T 上のメジャー $\geqslant 0$、満たす条件 c)、主張の $\nu$ 適切ファミリー $b \mapsto \lambda_b$ を定義し、ほぼすべての $b \in B$ について、$p$ は $\lambda_b$ 適切であり、$\lambda_b$ は$\overline{p}^{-1}(b)$ にはノルム 1 があります。 $N''$ を、最後の 3 つのプロパティの 1 つが検証されていない点 $b \in B$ の $\nu$ 無視できる集合とします。次に、次の方法で $\lambda_b$ を変更できます。 $b \in B - p(T)$ の場合は、$\lambda_b = 0$ を取ります。 $b \in p(T) \cap N''$ の場合、$\lambda_b = \varepsilon_{\xi(b)}$ を選択します。ここで、$\xi(b)$ は $\overline{p}^{-1}(b)$ のいずれかの点です。 $B - p(T)$ は $\nu$ で無視できるため (Ch. V, §6, No. 2、コル。提案 2) の 3) では、無視できる集合の点で $\lambda_b$ を修正しただけであるため、ファミリー $b \mapsto \lambda_b$ は依然として $\nu$ で十分であり、性質 c) を持ちます。さらに、a) と b) を満たし、証明が完了します。

T のポジティブな尺度のすべての $\nu$-適切なファミリー $b \mapsto \lambda_b$ は、Th の特性 b) と c) を持ちます。 1 は、$\mu$ の適切な写像 $p$ に対する、$\mu$ の尺度の *崩壊* であると言われています。

### 2. 疑似映像対策

#### 定義 1 {#int-vi-s3-def-1 .statement tag=09C4}

*T と B を 2 つの局所的にコンパクトな空間、T 上の正の測度 $\mu$、T から B への $\mu$ 可測写像とする。B 上の正の測度 $\nu$ は、以下の条件を満たす場合、p の下で $\mu$ の疑似イメージ測度であると言われます。 B の部分集合 N が局所的に $\nu$ 無視できるようにするには、$\overline{p}^{-1}(N)$ が局所的に $\mu$ 無視できることが必要かつ十分です。*

#### 例 {#int-vi-s3-n2-exa-1 .statement tag=09C5}

— 1) $p$ が $\mu$-proper かつ $\nu = p(\mu)$ である場合、$\nu$ は $p$ に基づく $\mu$ の疑似イメージ尺度になります (提案 2 の V, §6, No. 2 項、Cor. 2)。

2) $B'$ を局所的にコンパクトな空間、$\nu'$ を $B'$ の正の測度とする。 T 空間 $B \times B'$ を、$\mu$ についてメジャー $\nu \otimes \nu'$ を取得します。 $p$ が B 上の T の射影である場合、$\nu$ は $p$ の下での $\mu$ の疑似イメージです (Ch. V, §8, No. 2、提案 4 および No. 3、提案 7 の修正 1)。

$\nu$ が $p$ の下の $\mu$ の疑似イメージ尺度である場合、$\nu$ は $p(T)$ によって運ばれることに注意してください。

$\nu$ が $p$ の下で $\mu$ の疑似イメージである場合、$p$ の下で $\mu$ の疑似イメージであるメジャーの集合は、$\nu$ に相当するポジティブメジャーの類であり、$\mu$ に相当するすべてのポジティブメジャーは同じことを認めます。疑似画像は$p$以下で計測されます。 $\nu$の類は、$p$の$\mu$の*疑似イメージ類*であると言われています。

#### 命題 1 {#int-vi-s3-prop-1 .statement tag=09C6}

— *T を、局所的にコンパクトな空間を無限大で可算、$\mu$ を T の正の測度、$p$ を局所的にコンパクトな空間 B への T の $\mu$ 可測写像とします。 次に、$p$ の下に $\mu$ の疑似イメージ メジャーが存在します。

なぜなら、T には $\mu$ に相当する *有界* な測度 $\mu'$ が存在するからです (Ch. V, §5, No. 6、提案 11); $p$ は $\mu'$ として適切です。

### 3. $\mu$ の擬似イメージに対する尺度 $\mu$ の崩壊

#### 定理 2 {#int-vi-s3-thm-2 .statement tag=09C7}

— *Let T and B be two locally compact spaces having countable bases, $\mu$ a positive measure on T, $p$ a $\mu$-measurable mapping of T into B, and $\nu$ a pseudo-image measure of $\mu$ under $p$. この場合、T には、次の特性を持つポジティブな尺度の $\nu$-適切な族 $b \mapsto \lambda_b$ ($b \in B$) が存在します。
a) $b \in p(T)$ の場合は $\lambda_b \neq 0$;
b) $\lambda_b$ は $b \in B$ ごとに集合 $\overline{p^{-1}}(b)$ に集中します。特に、$b \notin p(T)$ の $\lambda_b = 0$。
c) $\mu = \int \lambda_b \, d\nu(b)$。

さらに、$\nu' = r \cdot \nu$ が $p$ の下での $\mu$ の 2 番目の疑似イメージ測度であり、$b \mapsto \lambda'_b$ が $\nu'$ に関して特性 b) と c) を持つ T 上の正の測度の $\nu'$ 適切族である場合、B のほぼすべての場所で $\lambda_b = r(b)\lambda'_b$ (* $\nu$ または$\nu'$*)。

T 上に定義された連続的で有限な数値写像 $f$ が存在し、$t \in T$ ごとに $f(t) > 0$ となり、$\mu'' = f \cdot \mu$ が有界となるようなものです (Ch. V, §5, No. 6、提案 11)。 $\nu$ と同等の $\nu'' = p(\mu'')$ を、$g$ が有限で局所的に $\nu$ 可積分である $\nu'' = g \cdot \nu$ と書きます。さらに、すべての $b \in B$ に対して $g(b) > 0$ であると仮定することもできます (Ch. V, §5, No. 6、提案 10)。 Th. No. 1 の 1 を $\mu''$ と $\nu''$ に適用すると、T に次のようなポジティブな尺度の $\nu''$ 適切なファミリー $b \mapsto \lambda''_b$ ($b \in B$) が存在することがわかります。

1) $b \in p(T)$ の場合は $\| \lambda''_b \| = 1$;
2) $\lambda''_b$ は $b \in B$ ごとに $\overline{p^{-1}}(b)$ に集中します。
3) $\mu'' = \int \lambda''_b \, d\nu''(b)$。

$b \in B$ ごとに、公式 $\lambda_b = (1/f) \cdot (g(b)\lambda''_b)$ による T のプラスの尺度定義するを$\lambda_b$ とします。ファミリー$b \mapsto \lambda_b$ が主張の特性 a) と b) を持っていることは明らかです。一方、写像 $h \in \mathscr{K}(T)$、$h/f$ 属する ～ $\mathscr{K}(T)$ ごとに、次のようになります。

$$
\int h(t) \, d\mu(t) = \int (h(t)/f(t)) \, d\mu''(t) = \int d\nu''(b) \int (h(t)/f(t)) \, d\lambda''_b(t).
$$

しかし、写像 $b \mapsto \int (h(t)/f(t)) \, d\lambda''_b(t)$ は $\nu''$ 可積分であるため、 写像 $b \mapsto g(b) \int (h(t)/f(t)) \, d\lambda''_b(t)$ は $\nu$ 可積分です (Ch. V, §5, No. 3、Th. 1)。

$\lambda_b$の定義により、この写像は$b \mapsto \int h(t) d\lambda_b(t)$、よって (*loc. cit.*) $\int h(t) d\mu(t) = \int d\nu(b) \int h(t) d\lambda_b(t)$となり、$\mu = \int \lambda_b d\nu(b)$が証明されます。

主張の 2 番目の部分を確立するには、すべての $b \in B$ に対して $r(b) > 0$ を仮定できることに注意します (Ch. V, §5, No. 6、提案 10); 集合 $\lambda'''_b = f \cdot \left( (r(b)/g(b)) \lambda'_b \right)$;上記のように、写像 $h \in \mathscr{K}(T)$、関係ごとに次のことがわかります。

$$
\int h(t) d\mu(t) = \int d\nu'(b) \int h(t) d\lambda'_b(t)
$$

暗示する

$$
\int h(t) d\mu(t) = \int d\nu''(b) \int (h(t)/f(t)) d\lambda'''_b(t) .
$$

したがって、Th. $\mu''$ と $\nu''$ に適用される No. 1 の 1 は、ほぼすべての $b \in B$、$\lambda'''_b = \lambda''_b$、よって $\lambda_b = r(b)\lambda'_b$ に適用されることを意味します。

#### 定義 2 {#int-vi-s3-def-2 .statement tag=09C8}

*T と B を 2 つのポーランド語の局所コンパクト空間とします。 T 上の正の測度 $\mu$、B への T の $\mu$ 可測写像 p、および p の下の $\mu$ の疑似イメージ測度 $\nu$ が与えられると、T 上の正の測度のすべての $\nu$ 適切族 $b \mapsto \lambda_b$ ($b \in B$) は、次の特性 b) および c) を持ちます。 Th. 2 は、$\nu$ に対する $\mu$ の崩壊と呼ばれます。*

$p$が$\mu$-properであり、$\nu = p(\mu)$であるとき、$p$に対する崩壊の概念は、$\nu$に対する崩壊の概念と一致するになります。 Thの仮説の下で。 2、同じ擬似イメージ尺度 $\nu$ に対する 2 つの $\mu$ の崩壊は、$\nu$ のほぼどこでも等しくなります。

#### 注意 {#int-vi-s3-n3-rem-1 .statement tag=09C9}

— て。 1章 V, §3, No. 4 shows (taking into account the fact that T and B have countable bases) that for every function $f$ defined on T, with values in $\overline{\mathbf{R}}$ or in a Banach space F and $\mu$-integrable, the set of $b \in B$ such that $f$ is not $\lambda_b$-integrable is $\nu$-negligible, the function $b \mapsto \int f(t) d\lambda_b(t)$, defined almost everywhere, is $\nu$-integrable, and

$$
\int f(t) d\mu(t) = \int d\nu(b) \int f(t) d\lambda_b(t) .
$$

同様の結果が、スカラー的に $\mu$ 積分可能な関数の §1, No. 1 の適用提案 3 に当てはまります。

### 4. 測定可能同値関係

X のトポロジカル空間 X と同値関係 R が与えられると、商空間 X/R がハウスドルフである場合、R は *ハウスドルフ* であると言うでしょう。

(GT、I, §8, No. 3、提案 8) を思い出してください。R が開いた同値関係であるとき、X × X における R のグラフは閉じていると言うのと同じことになります。

p をハウスドルフ トポロジカル空間 B の X の写像とし、R を X の同値関係 $p(x) = p(y)$ とします。 K が、p から K の制限が連続であるような X の圧縮部分集合である場合、商空間 $K / R_K$ は空間と同相であるため、K 上の R によって誘起される関係 $R_K$ はハウスドルフになります。 $p(K)$、コンパクトです (GT、I, §9, No. 4、Th. 2 およびその Cor. 2)。 T が局所的にコンパクトな空間、$\mu$ が T 上の正の測度、p がハウスドルフトポロジカル空間 B への T の $\mu$ 可測写像である場合、したがって、$\mu$ 密な集合が存在することがわかります。 関係 $R_K$ がハウスドルフであるコンパクトな部分集合 K の IV, §5, No. 8)。したがって、次のようなことが導かれます定義:

#### 定義 3 {#int-vi-s3-def-3 .statement tag=09CA}

*T を局所的にコンパクトな空間、$\mu$ を T の正の測度とする。 T の同値関係 R は、関係 $R_K$ がハウスドルフである T のコンパクト部分集合 K の $\mu$ 密集合が存在する場合、$\mu$ 可測であると言われます。

R がハウスドルフの場合、R は $\mu$ 可測です。なぜなら、$\varphi$ がハウスドルフ位相幾何学空間 T/R 上の T の標準写像である場合、$\varphi$ は連続であり、R は $\varphi(x) = \varphi(y)$ に等しいからです。同様に、R が、T のすべてのコンパクト部分集合の R の飽和が閉じているようなものである場合 (特に、R が閉じた同値関係である場合)、T のすべてのコンパクト部分集合 K について、関係 $R_K$ が閉じているため、R は $\mu$ 可測です。したがって、ハウスドルフ (GT, I, §10, No. 4、提案 8)。

R が $\mu$ 可測である場合、R は基底 $\mu$ を使用して T 上のすべての小節についても可測であることに注意してください。

#### 命題 2 {#int-vi-s3-prop-2 .statement tag=09CB}

*T を無限大で可算可能な局所コンパクト空間、T の正の測度 $\mu$ とします。

1) T 内のすべての $\mu$ 可測同値関係 R に対して、R が関係 $p(x) = p(y)$ と等価となるように、局所的にコンパクトな空間 B と T から B への $\mu$ 可測写像 p が存在します。

2) さらに、T が可算基底を認める場合、B は可算基底を認めると仮定できます。

T は無限に可算であるため、T が $K_n$ と $\mu$ で無視できる集合 N の和集合となり、それぞれ関係が成り立つような T のコンパクト部分集合の増加する数列 $(K_n)_{n \geq 1}$ が存在します。 $R_{K_n}$はハウスドルフです。 $B_n$ をコンパクトな商空間 $K_n / R_{K_n}$ とし、$B'_n$ をコンパクトな空間、つまり $B_n$ と点 $a_n$ のトポロジー 和とします。 $q_n$ を $K_n$ の標準写像から $B_n$ にするとします。次の方法で、T の拡大する $q_n$ から写像 $p_n$ を $B'_n$ に変換します。 $x \in T$ が mod R と元 $y \in K_n$、集合 $p_n(x) = q_n(y)$ に等しい場合。逆の場合は、集合 $p_n(x) = a_n$。

$B'$ をコンパクトな積空間 $\prod_{n=1}^{\infty} B'_n$ とし、$p'$ を T を B' に変換した写像 $x \mapsto (p_n(x))$ とします。 $p'$ が $\mu$ 可測であることを示しましょう。写像 $p_n$ のそれぞれが可測であることを証明するだけで十分です (Ch. IV, §5, No. 3、Th. 1)。このためには、$p_n$ の制限をそれぞれに満たすだけで十分です。 $K_m$ 測定可能であること。さて、$m \leq n$ であればこれは明らかです。逆に、$m > n$ の場合、$K_{nm}$ を $R_{K_m}$ の$K_n$ の彩度とします。これは、$K_m$ (GT、I, §9, No. 4、Th. 2) の圧縮部分集合です。 $p_n$ は $K_m - K_{nm}$ で定数であるため、$p_n$ から $K_{nm}$ の制限が連続であることを証明するだけで十分です。これは、$K_{nm}/R_{K_{nm}}$ と $K_n/R_{K_n}$ の間の標準同型を考慮すると明らかです (GT、I, §9, No. 4、Cor. 4 ２）。

Aを関係 Rの$\bigcup_n K_n$の彩度とし、$N' = T - A \subset N$とします。 関係 $p'(x) = p'(y)$ が関係 «$R\{x, y\}$ または $(x, y) \in N' \times N'$ » と同等であることがわかります。 なぜなら、$R\{x, y\}$ の場合、すべての $n$ に対して $p_n(x) = p_n(y)$ であるため、$p'(x) = p'(y)$ になります。そして、$x \in N'$、$y \in N'$ の場合、すべての $n$ に対して $p_n(x) = p_n(y) = a_n$、従って $p'(x) = p'(y)$ になります。 If on the other hand $x$ and $y$ are in A and are not equivalent mod R, then there exist an integer $n$, an element $x' \in K_n$ (resp. $y' \in K_n$) equivalent mod R to $x$ (resp. $y$) such that $x'$ is not equivalent to $y'$ mod $R_{K_n}$; therefore $p_n(x) \neq p_n(y)$, consequently $p'(x) \neq p'(y)$. Finally, if $x \in N'$ and $y \in A$, then $p_n(y) \in B_n$ for $n$ sufficiently large and $p_n(x) = a_n$ for all $n$, therefore $p'(x) \neq p'(y)$, which establishes our assertion.

次に、商集合 $B_0 = N'/R_{N'}$ を考えてみましょう。 $q_0$ を $N'$ の標準写像に、$B_0$、$s_0$ 切断の $q_0$ とします。 $x \in N'$ と拡大する $p_0$ に対する集合 $p_0(x) = s_0(q_0(x))$ は、$p_0$ を A 上の定数として T の元に等しいものとして T に代入します。すると、$p = (p', p_0)$ は T の $\mu$ 可測の写像を局所コンパクトに変換したものになります。 空間 $B = B' \times T$; $x \in N'$、$y \in N'$、関係 $p_0(x) = p_0(y)$ が $R\{x, y\}$ を意味する場合、それは明らかです。従って、$p$ は要件を満たしています。さらに、T が可算基底を認める場合、商空間 $B_n$ (GT, IX, §2, No. 10, 提案 17) も認められるため、B' は可算基底を認め、従って B も同様です。

#### 命題 3 {#int-vi-s3-prop-3 .statement tag=09CC}

— *T をポーランド語の局所コンパクト空間、$\mu$ T の正の測度、および T の R 同値関係とします。以下のプロパティは同等です:*

a) $R$ は $\mu$ で測定可能です。

b) *ハウスドルフトポロジカル空間には写像 $p_n : T \to F_n$ の数列が存在し、各 $p_n$ は $\mu$ 可測であり、関係 $R\{x, y\}$ は«すべての $n$ に対して、 $p_n(x) = p_n(y)$».*

c) *R に関して飽和した $\mu$ 測定可能な集合の数列 $(A_n)$ が存在し、R に関する x の $x \in T$ 類が含む x の $A_n$ の共通部分になります。

b)の主張のような記法では、集合 $p(x) = (p_n(x))$; 性質 b) は、積空間 $\prod F_n$ への T の写像 $p$ が測定可能であり (Ch. IV, §5, No. 3、Th. 1)、関係 $R\{x, y\}$ が $p(x) = p(y)$ と同等であることを意味します。したがって、b) は a) を意味します。

次に、c) が b) を意味することを示しましょう。 c) が検証されたとします。その場合、特性写像 $\varphi_{A_n}$ は $\mu$ 測定可能であり、仮定 c) は、関係 $R\{x, y\}$ が«すべての $n$、$\varphi_{A_n}(x) = \varphi_{A_n}(y)$ について» と同等であることを意味します。

最後に、a) が c) を意味することを示しましょう。提案 2 により、可算基底をもつ局所的にコンパクトな空間 B と、T から B への $\mu$ 可測写像 $p$ が存在し、関係 $R\{x, y\}$ は $p(x) = p(y)$ と等価になります。 $(U_n)$ を B の位相に対して可算な基底とします。 集合 $A_n = \overline{p^{-1}(U_n)}$ は $\mu$ 可測であり (Ch. IV, §5, No. 5、提案 7)、R について飽和します。そして、$x, y$ が $p(x) \neq p(y)$ となるような T の点である場合、$p(x) \in U_n$ と $p(y) \notin U_n$ となる添字 $n$ が存在します。これは、$x \in A_n$ と $y \notin A_n$ を意味します。

#### 注意 {#int-vi-s3-n4-rem-1 .statement tag=09CD}

R が T の $\mu$ 測定可能な同値関係である場合、T のコンパクト部分集合の R の飽和は必ずしも $\mu$ 測定可能ではありません (例 5)。

#### 定理 3 {#int-vi-s3-thm-3 .statement tag=09CE}

— *T を局所的にコンパクトな空間とし、可算基底、T 上の正の測度 $\mu$、T 内の $\mu$ 可測同値関係をもつとします。すると、R に関して各類と交差する T の $\mu$ 可測部分集合 S が存在します。唯一の点 (R の「測定可能な切断」)。*

私たちは明らかに、尺度 $\mu$ が有界であり、$\mu(T) \leq 1$ が有界であると仮定することができます (Ch. V, §5, No. 6、提案 11)。 *Borel* 部分集合 (GT, IX, §6, No. 3) の定義する数列 $(S_n)$ を、R に関する各同値類が $S_n$ の和集合 $S'$ と最大 1 回で交差するようにします。 点、$n$ごとに、添字$p \leq n$の$S_p$の和集合の彩度$T_n$が$\mu$測定可能であり、$\mu(T - T_n) \leq 1/2^n$です。したがって、$S'$ の彩度 $T'$ は $\mu$ で測定可能となり、$N = T - T'$ は測定値零を持ちます。 $S''$ が関係 $R_N$ の N のいずれかの切断である場合、$S'$ はボレル集合であるため、$\mu$ 測定可能であるため、$S = S' \cup S''$ は要件を満たします (Ch. IV, §5, No. 4、Cor. 3 Th. 2)、$S''$ にはメジャー 零があります。

提案 2 によれば、$R\{x, y\}$ は関係 $p(x) = p(y)$ と等価であり、ここで $p$ は、局所的にコンパクトな空間 F への T の $\mu$ 可測写像です。 $k \leq n$ に対して $S_k$ が定義されているとします。 $T - T_n$ は $\mu$ 可測であり、$\leq 1/2^n$ の測定であるため、$\mu(T - (T_n \cup K)) \leq 1/2^{n+1}$ となり、$p$ から K までの制限が連続となるような、$T - T_n$ のコンパクトな部分集合 K が存在します。 Since the induced relation $R_K$ is closed and K is metrizable, we know that there exists a Borel subset $S_{n+1}$ of K such that, in K, each point is equivalent (mod R) to one and only one point of $S_{n+1}$ (GT, IX, §6, No. 8, Th.4). したがって、$p(S_{n+1}) = p(K)$、これは F のコンパクトな集合です。 R の $S_{n+1}$ の飽和は逆像 $\overline{p^{-1}(p(K))}$ であるため、μ 測定可能です (Ch. IV, §5, No. 5、提案 7);この集合含む K、したがって T_n と $\overline{p}^{-1}(p(K))$ の和集合 T_{n+1} はμ測定可能であり、R について飽和しており、$\mu(T - T_{n+1}) \leq 1/2^{n+1}$ となり、証明が完成することは明らかです。

### 5. 測定可能なものによる測定の崩壊同値関係

T をポーランド語の局所的コンパクト空間、$\mu$ T 上の正の測度、R を T の$\mu$ 可測同値関係とします。すると、ポーランド語の局所的コンパクト空間 B と $\mu$ 可測写像が存在します (No. 4、提案 2)。 T の p を B に変換し、関係 $p(x) = p(y)$ が R$\{x, y\}$ と等価になるようにします。 p (No. 2) の下の $\mu$ の擬似イメージであるすべてのメジャー $\nu$ は、関係* R によって $\mu$ の *商メジャーと呼ばれます。 $b \mapsto \lambda_b$ が測度 $\nu$ に対する $\mu$ の分解である場合、$b \mapsto \lambda_b$ は関係* R による $\mu$ の * 分解であると言えます。 p と $\lambda_b$ の性質により、各測度 $\lambda_b$ は次の点に集中します。 R に関しては同値類、$b \neq c$ の場合、$\lambda_b$ と $\lambda_c$ は別個の類に集中します。

空間 B、写像 p、および B 上の疑似イメージ尺度 $\nu$ は、一般に無限に多くの方法で選択できます。それにもかかわらず、R による $\mu$ のさまざまな崩壊はすべて、次の定理の帰結として、そのうちの 1 つから推定できます。

#### 定理 4 {#int-vi-s3-thm-4 .statement tag=09CF}

*T をポーランド語の局所的コンパクト空間、$\mu$ T 上の正の測度、R を T で$\mu$-測定可能な同値関係とする。 B、B' を 2 つのポーランド語の局所的コンパクト空間、p、p' とする T の 2 つの $\mu$-測定可能な写像をそれぞれ B、B' に入れる。 R$\{x, y\}$ は $p(x) = p(y)$ および $p'(x) = p'(y)$ と同等です。 $\nu, \nu'$ を、それぞれ p、p' の下での $\mu$ の擬似イメージ尺度とします。 $b \mapsto \lambda_b, b' \mapsto \lambda_{b'}$ を、それぞれ $\nu, \nu'$ に対する $\mu$ の崩壊とします。*

*これらの条件の下には、$\nu$ (それぞれ $\nu'$) に対して無視できる B (それぞれ B') 集合 N (それぞれ N') と、B' - N' 上の B - N の全単射 f が存在し、次の特性を持ちます。

a) *写像 f (B のほぼどこでも定義) は $\nu$ 可測であり、その逆数写像 $f'$ は $\nu'$ 可測です。 f (それぞれ $f'$) の下での$\nu$ (それぞれ $\nu'$) のすべての疑似イメージ メジャーは、$\nu'$ (それぞれ $\nu$) と同等です。*

b) *すべての $b \in B - N$ について、T 上の測度 $\lambda'_{f(b)}$ は形 $r(b)\lambda_b$ です。ここで、$r(b) \neq 0$ と r は局所的に $\nu$ 積分可能です。*

a) を確立するには、$\nu$ と $\nu'$ が *有界* 尺度である場合に極限を当てはめることができます (Ch. V, §5, No. 6、提案 11)。 $N_0 = B - p(T)$、$N'_0 = B' - p'(T)$ としましょう。 $N_0$ (それぞれ $N'_0$) は、$\nu$ (それぞれ $\nu'$) (No. 2) に対して無視できることがわかっています。 すべての $t \in T$ に対して $f(p(t)) = p'(t)$ によって定義される B' - $N'_0$ 上に B - $N_0$ の全単射 f が存在します。 $f'$ を $f$ の逆数写像として、$f'(p'(t)) = p(t)$ とします。 B のすべての部分集合 M について、関係 「M は $\nu$ 測定可能」は、「 $\overline{p}^{-1}(M)$ は $\mu$ 測定可能」、つまり、「 $p'(f(M))$ は $\mu$ 測定可能」と同等であり、最終的には « $f(M)$ は$\nu'$-測定可能 » (Ch. V, §6, No. 2、コル。提案 3)。 従って、$f$ (それぞれ $f'$) 変換がすべての $\nu$ 測定可能 (それぞれ $\nu'$ 測定可能) 集合から $\nu'$ 測定可能 (それぞれ $\nu$ 測定可能) 集合になることがわかります。 B と $B'$ は可測であり、可算基底を持っているため、$f$ と $f'$ は可測であるということになります (Ch. IV, §5, No. 5、木。 4)。 さらに、$M \subset B$ が $\nu$ 無視できる場合、$\overline{p}^{-1}(M) = p'(f(M))$ は $\mu$ 無視できるので、$f(M)$ は $\nu'$ 無視できる（Ch. V, §6, No. 2、コル。提案 2 の 2)。同様に、$f'$ 変換を $\nu'$ 無視できる集合ごとに $\nu$ 無視できる集合に変換します。 従って、$f$ の下の $\nu$ の像 (これは、$\nu$ が有界であるため定義され、$f$ が $\nu$-proper であることを意味します) は $\nu'$ と等しく、$f'$ の下の $\nu'$ の像は、と等価です。 $\nu$ (Ch. V, §5, No. 6、提案 10)。 b)を証明することはまだ残っています。 Th のおかげで。 2 of No. 3, we can restrict ourselves to the case that $\nu' = f(\nu)$. $\mu = \int \lambda_{b'}' d\nu'(b')$ 以降、写像 $h \in \mathscr{K}(T)$ ごとに、

$$
\int h(t) d\mu(t) = \int d\nu'(b') \int h(t) d\lambda_{b'}'(t) = \int d\nu(b) \int h(t) d\lambda_{f(b)}'(t)
$$

(Ch. V, §3, No. 4、木。 1 と §6, No. 2、Th。 1);その他の語、$\mu = \int \lambda_{f(b)}' d\nu(b)$。 But since also $\mu = \int \lambda_b d\nu(b)$ and since, for every $b \in B - N_0$, $\lambda_b$ and $\lambda_{f(b)}'$ are carried by $\overline{p}^{-1}(b)$, Th. 2 of No. 3 implies that $\lambda_b = \lambda_{f(b)}'$ for almost every $b \in B - N_0$, hence for almost every $b \in B$. 木曜日の条件したがって、4 は、$N_0$ の N 和集合と $b \in B$ の集合をとって、$\lambda_b \neq \lambda_{f(b)}'$ となるように検証されます。

### 練習問題 {#int-vi-s3-exercises}

[§ 3 に対して練習問題](exercises/s3/)を参照してください。
