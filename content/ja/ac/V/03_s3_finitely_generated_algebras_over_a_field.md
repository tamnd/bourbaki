---
book: ac
book_title: Commutative Algebra
chapter: V
chapter_title: INTEGERS
section: 3
section_title: Finitely generated algebras over a field
lang: ja
source: ac-i-vii
book_pages: 344-354, 370-373
pdf_pages: 0363-0373, 0389-0392
extraction: ocr
subsections:
    - "no": 1
      title: THE NORMALIZATION LEMMA
      page: 344
      pdf_page: 363
    - "no": 2
      title: THE INTEGRAL CLOSURE OF A FINITELY GENERATED ALGEBRA OVER A FIELD
      page: 348
      pdf_page: 367
    - "no": 3
      title: THE NULLSTELLENSATZ
      page: 349
      pdf_page: 368
    - "no": 4
      title: JACOBSON RINGS
      page: 351
      pdf_page: 370
statements: 17
exercises: 10
content_sha256: 56c906dc60d02d89b0f71a8c1c1ac5d2933c906155aead6cf3b8ef8885887a5e
translated_from: content/en/ac/V/03_s3_finitely_generated_algebras_over_a_field.md
translation_method: google
source_content_sha256: 6de44311d5d60b730fb626da1cd69b9f44af23562467fb568b226b7a0a3a5d4c
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-eeeca2ef
glossary_version: 34
glossary_terms_sha256: 5ec9b31bddccc39a96ddb902d7645fac8918fe50b55dae417fc8b62e81695625
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## 3. 体に対して有限に生成される代数

### 1. 正規化補題

このNo.以下、kは可換体を表します。

#### 定理 1 (正規化補題) {#ac-v-s3-thm-1 .statement tag=04R8}

A を有限生成された K-代数とし、$a_1 \subset a_2 \subset \ldots \subset a_p$ を $p \geq 1$ と $a_p \neq A$ のような A の理想の増加する有限列とします。 k (章 III, § 1, no. 1) 上で代数的に独立した A の元の有限列 $(x_i)_{1 \leq i \leq n}$ が存在します。
(a) A は環 $B = k[x_1, \ldots, x_n]$ にわたって積分です。
(b) $1 \leq j \leq p$ のようなすべての j に対して、整数の増加する数列 $(h(j))_{j \leq j \leq p}$ が存在し、すべての j に対して B の理想 $a_j \cap B$ が生成されます $x_1, \ldots, x_{h(j)}$。

注意まず、A が多項式代数 $k[Y_1, \ldots, Y_m]$ であるとき、定理を証明すれば十分であること。 一般的な場合、A はイデアル $a'_0$ によってそのような代数 A' の商と同型であるからです。 $a'_j$ は A' の $a_j$ の逆像を表し、 環 A' と増加するについて $x'_i$ ($1 \leq i \leq r$) は A' の元満たす主張の条件とします理想$a'_0 \subset a'_1 \subset \ldots \subset a'_p$の数列。 次に、A の $x'_i$ の像 $x_i$ が、$i > h(0)$ 満たすの目的の条件になります。これは、条件 (b) と条件 (a) では明らかであり、§ 1, no. 1、命題 2 から導き出されます。最後に、$x_i(h(0) + 1 \leq i \leq r)$ が k に関して代数的に独立していない場合、非ゼロの多項式が存在します。

$$
Q \in k[X_{h(0)+1}, \ldots, X_r]
$$

ここで、$Q_j$ は $k[Y_1, \ldots, Y_m]$ の多項式です。 $a_p \neq 0$ は $k$ で可逆であるため、(4) は確かに B の係数、私たちの主張のよってとの積分依存関係の方程式です。

The field of fractions $k(Y_1, \ldots, Y_r)$ of A is therefore algebraic over the field of fractions $k(x_1, \ldots, x_m)$ of B, which proves (Algebra, Chapter V, § 5, no. 3, Theorem 4) that the $x_i$ ($1 \leq i \leq m$) are algebraically independent. さらに、$a \cap B = Bx_1$;すべての元 $z \in a, \cap B$ は、$z' \in A \cap k(x_1, \ldots, x_r)$ の場合、$z = x_1 z'$ と書くことができます。ただし、$B$ は一体的に閉じているため、$A \cap k(x_1, \ldots, x_r) = k[x_1, \ldots, x_m] = B$ ($\S$ 1、no. 3、系 2 ～ 命題 13)。したがって、$z' \in B$ となり、この場合、プロパティ (a) と (b) の証明が完成します。

(A2) **一般的なケース ($p = 1$).**
$m$ については帰納法で議論しますが、$m = 0$ のケースは自明です。明らかに $a_i \neq 0$ と仮定するかもしれません (そうでない場合は、$1 \leq i \leq m$ と $h(1) = 0$ に対して $x_i = Y$ を取るかもしれません)。 $x_1$ を $a_i$ の非ゼロ元とします。 (A1) により、$x_1, t_2, \ldots, t$ が $k$ に対して代数的に独立し、$A$ が $C = k[x_1, t_2, \ldots, t_m]$ と $x_1 A \cap C = x_1 C$ に対して積分となるような $t_2, \ldots, t_m$ が存在します。 帰納法の仮定までに、$k[t_2, \ldots, t_m]$ と整数 $h$ の元 $x_2, \ldots, x_m$ が存在し、$k[t_2, \ldots, t_m]$ は$B' = k[x_2, \ldots, x_m]$ で積分、$x_2, \ldots, x_m$ は$k$ で代数的に独立しており、理想$a_i \cap B'$ は $x_2, \ldots, x_h$ によって生成されます。次に、$C$ は $B = k[x_1, x_2, \ldots, x_m]$ ($\S$ 1, no. 1, 系 ～ 命題 5 ) に対して整数であるため、$A$ ($\S$ 1, no. 1, 命題 6 ) も同様です。ケース (A1) と同じ議論は、$x_1, \ldots, x_m$ が $k$ に対して代数的に独立していることを示しています。最後に、$x_1 \in a_i$ と $B = B'[x_1], a_i \cap B = Bx, + (a_i \cap B')$ として、そして $a_i \cap B'$ が ($B'$ で) $x_2, \ldots, x_h, a_i \cap B$ によって生成され ($B$ で) $x_1, x_2, \ldots, x_h$ によって生成されます。

(B) **$p - 1$上部からの通路**
$t_1, \ldots, t_r$を、理想$a_1 \subset \ldots \subset a_{p-1}$の増加する数列に対して、$A$の満たす条件、定理の元とし、$r = h(p - 1)$と書きましょう。 (A2) により、次のような $k[t_{r+1}, \ldots, t_m]$ と整数の元 $x_{r+1}, \ldots, x_s$ が存在します。
$$
C = k[t_{r+1}, \ldots, t_m]
$$
は $B' = k[x_{r+1}, \ldots, x_m]$ に関して積分であり、$x_{r+1}, \ldots, x_s$ は $k$ に関して代数的に独立しており、イデアル $a_p \cap B'$ は $x_{r+1}, \ldots, x_s$ によって生成されます。 得られたファミリー$(x_i)_{1 \leq i \leq m}$に$i \leq r$に$x_i = t_i$を書くと、問題は$h(p) = s$で解けます。
なぜなら、$A$は$C[t_1, \ldots, t_r] = C[x_1, \ldots, x_r]$に対して積分であり、したがって$C$は$B'$に対して積分であるため、$B = k[x_1, \ldots, x_m] = B'[x_1, \ldots, x_r]$に対しても整数です($\S$1、no. 1、系から命題5および命題6)。ケース (A1) のように、$x_i$ が $k$ に対して代数的に独立していることがわかります。 一方、$j \leq p - 1$ の場合、イデアル
$$
a_j \cap k[x_1, \ldots, x_r, t_{r+1}, \ldots, t_m]
$$
$x_1, \ldots, x_r, t_{r+1}, \ldots, t_m$ の多項式の仮定集合によるもので、そのすべての単項式含むは元 $x_1, \ldots, x_{h(j)}$ の 1 つです。 $x_{r+1}, \ldots, x_m$ は $t_{r+1}, \ldots, t$ の多項式であり、$k$ では係数であるため、$x_1, \ldots, x_r, x_{r+1}, \ldots, x_s$ の多項式 ($k$ では係数) は、すべての単項式が一致する場合にのみ属するから $a_j$ になることがすぐにわかります。 含む元 $x_1, \ldots, x_{h(j)}$ のいずれか。 最後に、$x_1, \ldots, x_r$ 属するから $a_{p-1}$ 、したがって $a_p$ も同様に、$a_p \cap B'[x_1, \ldots, x_r]$ は $B'$ の係数を含む $x_1, \ldots, x_r$ の多項式で構成され、その定数は項属するから $a_p \cap B'$ です。したがって、この理想は $x_1, \ldots, x_r, x_{r+1}, \ldots, x_t$ によって生成されます。

#### 系 1 {#ac-v-s3-thm-1-cor-1 .statement tag=04R9}

$A$ を整域とし、$B$ を有限生成された $A$-代数含む $A$ を部分環とします。次に、$B[s^{-1}]$ (章 II, § 2, no. 1) が積分となる多項式代数 $A[Y_1, \ldots, Y_n]$ に同型の $A$ の元 $s \neq 0$ と $B$ の部分代数 $B'$ が存在します。 $B'[s^{-1}]$。

$S = A - \{0\}$ と書き、$k = S^{-1}A$ 体 of 分数 of $A$ とします。明らかに、$S^{-1}B$ は有限生成された $k$-代数であり、仮定 (章 II, § 2, no. 4, 定理 1) によって含む $k$ であるため、0 には減りません。 定理 1 によって (最上位 = を適用) 1 と $a_i = 0$) したがって、$k$ に関して代数的に独立しており、$S^{-1}B$ が $k[x_1, \ldots, x_n]$ に関して積分であるような、$S^{-1}B$ の元の有限列 $(x_i)_{1 \leq i \leq n}$ が存在します。 $(z_j)_{1 \leq j \leq m}$ を $A$-代数 $B$ の生成元の系とします。 $S^{-1}B$ では、$z_j/1$ のそれぞれが積分依存関係の方程式を満たします。

$$
(z_j/1)^{a_j} + \sum_{h < a_j} P_{hj}(x_1, \ldots, x_n)(z_j/1)^h = 0
$$

ここで、$P_{hj}$ は、$k$ の係数を含む $x_i$ の多項式です。 $A$ の元 $s \neq 0$ が存在し、$x_i = y_i/s$ と書くことができます。これにより、$1 \leq i \leq n$ の $\in B$ と、$P_{hj}$ のすべての係数は、$c \in A$ 形 $c/s$ になります。最後に、必要に応じて、置き換えること、$S$の元の積までに$s$、$B$になると想定できます。

$$
sz_j^{a_j} + \sum_{h < a_j} Q_{hj}z_j^h = 0
$$

where the $Q_{hj}$ are polynomials in $y_1, \ldots, y_n$ with coefficients in $A$; if we write $z'_j = sz_j$, it is seen, multiplying (6) by $s^{a_j-1}$, that $z'_j$ is integral over $B' = A[y_1, \ldots, y_n]$. $y_i$ が $A$ に対して代数的に独立していることを示します。 形 $\sum_p a_p y_1^{p_1} \ldots y_n^{p_n} = 0$ のうち関係があり、すべての $p$ が $a_p \in A$ である場合、$S^{-1}B$ には $\sum_p a'_p x_1^{p_1} \ldots x_n^{p_n} = 0$、$k$ には $a'_p = a_p s^{p_1 + \cdots + p_n}$ があると推測します。 仮定までなので、すべての$p$に対して$a'_p = 0$、すべての$p$に対してよって $a_p = 0$。 さらに、環 $B[s^{-1}]$ では、それぞれの $z'_j/1$ は $B'[s^{-1}]$ (§ 1, no. 1、命題 2) に対して積分であり、$B[s^{-1}]$ の $z_j/1 = (z'_j/1)(1/s)$ のように、$z_j/1$ は $B'[s^{-1}]$ に対して積分であることがわかり、これで完了します。 証明 (§ 1, no. 1、命題 4)。

#### 系 2 {#ac-v-s3-thm-1-cor-2 .statement tag=04RA}

$K$ を体、$A$ 部分環の $K$、および $L$ 体の分数または $A$ とします。 $K$ が有限生成された $A$-代数である場合、$[K:L]$ は有限であり、$L = A[a^{-1}]$ のように $A$ に $a \neq 0$ が存在します。

系 1 から、$K$ の元 $x_1, \ldots, x_n$ と $A$ の元 $a \neq 0$ が存在し、$x_1, \ldots, x_n$ は $A$ (したがって L について) 上で代数的に独立しており、K は積分であることがわかります。 部分環 $A[x_1, \ldots, x_n, a^{-1}]$。 次に、§2, no.1、補題 2 から、$A[x_1, \ldots, x_n, a^{-1}]$ は体となります。 But the only invertible elements of a polynomial ring $C[Y_1, \ldots, Y_n]$ over an integral domain C are the invertible elements of C; applying this remark to $C = A[a^{-1}]$, it is seen that necessarily $n = 0$ and that $A[a^{-1}]$ is a field equal to L by definition of the latter. K は L で積分であり、有限生成される L-代数であるため、次数 [K:L] は有限です (§ 1, no. 1, 命題 4)。

#### 系 3 {#ac-v-s3-thm-1-cor-3 .statement tag=04RB}

A を整域、B は、A のすべての $z \neq 0$ とすべての整数 $n > 0$ に対して $zb^n \neq 0$ となるように、B の有限生成された A-代数と b 元とします。 $\varphi : A \to B$ を標準準同型とします。 A には $a \neq 0$ が存在し、A から代数閉体 L までの準同型 f ごとに、$f(a) \neq 0$ のように、B から L までに準同型 g が存在し、$g(b) \neq 0$ と $f = g \circ \varphi$ が存在します。

b の仮定は、h が B の $B[b^{-1}]$ までの標準準同型 $x \mapsto x/1$ である場合、A の $B[b^{-1}]$ までの準同型 $h \circ \varphi$ が単射であることを意味します。したがって、系 1 によって、A の元 $a \neq 0$ と $B[b^{-1}]$ の部分環 $B'$ が存在し、$B[b^{-1}, a^{-1}]$ は $B'[a^{-1}]$ について整数となり、$B'$ は多項式代数と同型になります。 $A[Y_1, \ldots, Y_n]$。 f を A から代数閉体 L までの準同型とし、$f(a) \neq 0$ とします。 f を拡張する $A[Y_1, \ldots, Y_n]$ から L までの準同型が存在し、したがって f を拡張する $B'$ から L までの準同型 $f'$ が存在します。 Lの$f'(a) \neq 0$として、$B'[a^{-1}]$からLまでの準同型$f''$が存在します。

$$
f''(x/a^n) = f'(x) \cdot (f(a))^{-n}
$$

すべての $x \in B'$ とすべての $n > 0$ (章 II, §2, no. 1、命題 1)。最後に、$B[b^{-1}, a^{-1}]$ は $B'[a^{-1}]$ で積​​分であるため、$f''$ (§2, no. 1、系 4 から定理 1) を拡張する $B[b^{-1}, a^{-1}]$ から L までの準同型 $f'''$ が存在します。 $j : x \mapsto x/1$ が B から $B[b^{-1}, a^{-1}]$ までの標準準同型である場合、$g = f''' \circ j$ は $j(b)$ が $B[b^{-1}, a^{-1}]$ で可逆であるため、L の $f'''(j(b)) \neq 0$ を求めて問題を解きます。

系 3 で B が整域と $A \subset B$ であると仮定すると、b の仮定は $b \neq 0$ と同等であることに注意してください。

### 2. 体上で有限生成された代数の積分閉包

#### 定理 2 {#ac-v-s3-thm-2 .statement tag=04RC}

Aを有限生成積分K-代数、Kを分数の体、Kの有限代数拡大である体K'におけるAの積分閉包$A'$とする。すると、$A'$は有限生成A-加群で有限K-代数が生成されました。

定理 1 までに、多項式代数 $k[X_1, \ldots, X_n]$ と同型の A の部分代数 C が存在し、A は C にわたって整数になります。 $A'$ は明らかに K' (§ 1, no. 1, 命題 6) の C の積分閉包です。したがって、$A = k[X_1, \ldots, X_n]$ の場合に注意を限定することができます。 $N$ を、$K$ (代数, 章) の有限代数拡大である$K'$ によって生成される$K$ ($K$ の代数閉包) の準ガロア拡張とします。 V, § 6, no. 3、系 1 ～ 命題 9)。 $N$ の $A$ の積分閉包 $B$ が有限生成された $A$ 加群であることを証明すれば十分です。なぜなら、 $A'$ は $B$ のサブ$A$ 加群であり、 $A$ はネーター であるからです。 環 (章 III, § 2, no. 10、系 2 ～ 定理 2)。したがって、$K'$ が $K$ の準ガロア拡張である場合に注意を限定することができます。次に、(代数, 章 V, § 10, no. 9, 命題 14) $K'$ は、$K$ の (有限) 根号拡大 $K''$ の (有限) ガロア拡大であることがわかります。 $A''$ が $K''$ の $A$ の積分閉包である場合、$A'$ は $K'$ の $A''$ の積分閉包であり、$A''$ が有限生成された $A$ 加群であり、$A'$ が有限生成された $A''$ モジュール。さて、$A''$ が有限生成された $A$ 加群であることが証明された場合、それは定義によって一体的に閉じられたネーター 領域になります。 $A$ が有限生成された $A''$ モジュールであるという事実は、§ 1, no. 6、系 1 から命題 18 まで続きます。

したがって、$A = k[X_1, \ldots, X_n]$ と $K'$ が $K = k(X_1, \ldots, X_r)$ の有限根数拡大である場合に注意を限定できることがわかります。すると、$K'$は元$(y_i)_{1 \leq i \leq m}$の有限族によって生成され、$y_i^q \in k(X_1, \ldots, X_r)$となるような$k$の特性指数の冪$q$が存在します。 $c_j$ ($1 \leq j \leq r$) を、$X_1, \ldots, X_r$ の有理数写像の分子と分母の係数とし、$y_i^q$ ($1 \leq i \leq m$) に等しいとします。次に、$K'$ は拡大 $L = k'(X_1^{q^{-1}}, \ldots, X_n^{q^{-1}})$ に含まれ、$k' = k(c_1^{q^{-1}}, \ldots, c_r^{q^{-1}})$ (私たちは $K'$ の代数閉包にいます)、$A$ は $A$ の代数閉包 $B'$ に含まれます。 $L'$。さて、$k'$ は $k$ に対して代数的であるため、$C' = k'[X_1, \ldots, X_n]$ は $A$ ($§ 1$, no. 1, 命題 5) に対して積分です。 $k'[X_1^{q^{-1}}, \ldots, X_n^{q^{-1}}]$ は積分閉包 ($§ 1$、no. 3、系 2 から命題 13) であるため、この環は $L'$ の $C'$ の積分閉包であり、したがって $A$ の積分閉包でもあることがわかります。 ($§ 1$、no. 1、命題6)、その他では語 $B' = k'[X_1^{q^{-1}}, \ldots, X_n^{q^{-1}}]$。ここで、$B'$ は有限生成された $C'$ モジュール ($§ 1$、no. 1、命題 4) であり、$k'$ が $k$ の有限拡大であるように、$C'$ は有限生成されたモジュールです。 $A$ モジュール、したがって $B'$ は有限生成された $A$ モジュールです。 $A$ はネーター と $A \subset B'$ であるため、$A'$ は有限生成された $A$ モジュールです。

### 3. ヌルステレンザッツ

#### 命題 1 {#ac-v-s3-prop-1 .statement tag=04RD}

$A$ を、$k$ の体 $k$ および $L$ 代数閉包上で有限生成された代数とします。

(i) $A \neq \{0\}$ の場合、$A$ から $L$ までの $k$ 準同型性が存在します。

(ii) $f_1, f_2$ を $A$ から $L$ までの 2 つの $k$ 準同型射とします。 $f_1$ と $f_2$ が同じ核を持つためには、 $f_2 = s \circ f_1$ となるような $L$ の $k$ 自己同型 $s$ が存在することが必要かつ十分です。

(iii) $a$ を $A$ の理想とする。 $a$ が最大になるためには、$A$ から $L$ までの k-準同型性の核であることが必要かつ十分です。

(iv) For an element $x$ of $A$ to be such that $f(x) = 0$ for every k-homomorphism $f$ from $A$ to $L$, it is necessary and sufficient that $x$ be nilpotent.

主張 (i) no. 1、系 3 から定理 1 に続き、置き換えること $A$ は $k$ により、$B$ は $A$ により、$b$ は単位元により適用されます$B$ と $f$ を $k$ の標準単射で $L$ にします。

$f$ が $A$ から $L$ までの k 準同型である場合、$f(A)$ は $L$ 含む $k$ の部分環です。 $L$ は $k$ の代数拡大であるため、$f(A)$ は体 (代数, 章 V, § 3, no. 2, 命題 3) であり、$a$ が核オフの場合、したがって、$f(A)$ と同型の $A/a$ は体となり、$a$ が最大であることが証明されます。逆に、$a$ が $A$ の最大イデアルである場合、(i) から、$A/a$ から $L$ までの k 準同型性が存在し、したがって $A$ から $L$ の k 準同型性が存在し、その核 $b$ が存在することがわかります。 含む $a$;しかし、$a$ が最大であるため、$b = a$;これは(iii)を証明します。

ここで (ii) を証明します。 $s$ が $f_2 = s \circ f_1$ となるような $L$ の k 自己同型である場合、明らかに $f_1$ と $f_2$ は同じ核を持ちます。逆に、$f_1$ と $f_2$ が同じ核を持っているとします。その場合、$f_2 = s_0 \circ f_1$ となるような体 $f_2(A)$ への体 $f_1(A)$ の k-同型写像 $s_0$ が存在します。しかし、代数, 章 V, § 6, no. 3, 命題 7, $s_0$ 拡大するにより、$L$ の k 自己同型となり、したがって $f_2 = s \circ f_1$ になります。

最後に、$x \in A$ が $x^n = 0$ である場合、$A$ から $L$ までのすべての k-準同型$f$ に対して、$L$ は体であるため、$(f(x))^n = f(x^n) = 0$、したがって $f(x) = 0$ となります。逆に、$x \in A$ が nilpotent ではないと仮定します。その場合、$A[x^{-1}]$ は有限生成された $A$-代数 (したがって、有限生成された K-代数) であり、0 (章 11、§ 2, no. 1、注意 3) に還元されないため、以下から k-準同型性 $g$ が存在します。 (i)による$A[x^{-1}]$から$L$まで。 $j : A \to A[x^{-1}]$ が標準準同型の場合、$f = g \circ j$ は $A$ から $L$ および $f(x)g(1/x) = g(x/1)g(1/x) = g(1) = 1$、よって $f(x) \neq 0$ の k 準同型です。

$k$ を $k$ の体と $L$ 拡大体とします。 $L^n$ の元 $x = (x_1, \ldots, x_n)$ は、多項式環 $k[X_1, \ldots, X_n]$ の理想的な $c$ の $L^n$ では零と呼ばれます。

$$
P(x) = P(x_1, \ldots, x_n) = 0
$$

すべての$P \in r$に。

#### 補題 1 {#ac-v-s3-lem-1 .statement tag=04RE}

Let $A$ be a finitely generated algebra over a field $k$, $(a_i)_{1 \leq i \leq n}$ a system of generators of this algebra and $c$ the ideal of algebraic relations between the $a_i$ with coefficients in $k$ (Algebra, Chapter IV, § 2, no. 1). $k$ のすべての拡大体 $L$ について、写像 $f \mapsto (f(a_i))_{1 \leq i \leq n}$ は、$A$ から $L$ までの k 準同型射の集合の集合に対する全単射です。 $L^n$の$r$の零。

$A$ 上には、$1 \leq i \leq n$ に対して $h(X_i) = a_i$ となるような、$k[X_1, \ldots, X_n]$ のK-代数準同型 $h$ が存在し、定義までに $r$ は $h$ の核になります。 写像 f $\mapsto$ の $A$ から $L$ までの k-準同型の集合の全単射を、c 上の零である $k[X_1, \ldots, X_n]$ から $L$ までの k-準同型の集合に重ねます。すべての多項式 $P \in k[X_1, \ldots, X_n]$ とすべての元 $x = (x_1, \ldots, x_i) \in L^n$ について、$h_x(P) = P(x)$ と書きます。その場合、写像 $x \mapsto h_x$ は、$k[X_1, \ldots, X_n]$ から $L$ までの k 準同型射の集合に対する $L^n$ の全単射です (そのような準同型は、$X_i$ での値によって決定されます) ($1 \leq i \leq n$) ); $h_x$ が c の零であると言うことは、$x$ が $L''$、よって補題の c の零であることを意味します。

命題 1 を代数 $A = k[X_1, \ldots, X_n]/r$ に適用すると、c は全体環とは異なる $k[X_1, \ldots, X_n]$ のイデアルであり、補題 1 によって次の主張が得られます。

#### 命題 2 (ヒルベルトのヌルステレンザッツ) {#ac-v-s3-prop-2 .statement tag=04RF}

k を k の体と L 代数閉包とします。

(i) 含む 1 ではないすべての理想 $r \not\subset k[X_1, \ldots, X_n]$ は、$L^n$ に少なくとも 1 つの零を認めます。

(ii) $x = (x_1, \ldots, x_n), y = (y_1, \ldots, y_n)$ を $L^n$ の 2 つの元とします。 x における $k[X_1, \ldots, X_n]$ 零の多項式の集合が y における $k[X_1, \ldots, X_n]$ 零の多項式の集合と同一であるためには、 $y_i = s(x_i)$ が成り立つような L の k 自己同型 s が存在することが必要かつ十分です。 $1 \leq i \leq n$。

(iii) $k[X_1, \ldots, X_n]$ の理想 a が最大になるためには、a が x で $k[X_1, \ldots, X_n]$ 零の多項式の集合となるような x が $L^n$ に存在することが必要かつ十分です。

(iv) $k[X_1, \ldots, X_n]$ の理想 c の$L''$ において、零の集合上で$k[X_1, \ldots, X_n]$ の多項式 Q が零となるためには、$Q^m \in c$ となるような整数 m > 0 が存在することが必要かつ十分です。

### 4. ジェイコブソン環

#### 定義 1 {#ac-v-s3-def-1 .statement tag=04RG}

環 A のすべての素イデアルが極大イデアル族の共通部分である場合、A はヤコブソン環と呼ばれます。

例

(1) すべての体はジェイコブソン環です。
(2) 環 $\mathbf{Z}$ はジェイコブソン環であり、最大 (0) ではない固有の素数イデアルは、$\mathbf{Z}$ の最大イデアル $(p)$ の共通部分であり、$p$ は素数の集合を通過します。 数 (cf. 命題 4)。
(3) A をヤコブソン環とし、a を A の理想とする。すると、$A/a$ の理想は形 $b/a$ であるため、$A/a$ はヤコブソン環となる。ここで、b は含む a の理想であり、 $b/a$ は、b がそうである場合に限り、素数 (それぞれ最大値) になります。

#### 命題 3 {#ac-v-s3-prop-3 .statement tag=04RH}

環 A がヤコブソン環であるためには、A のすべての理想 a について、$A/a$ のヤコブソン根基がそのニルラジカル (章 II, § 2, no. 6) に等しいことが必要かつ十分です。

$A/a$ のヤコブソン根基 (それぞれニラジカル) は、$A/a$ の最大 (それぞれ素数) イデアルの共通部分 (*代数*、章 VIII, § 6, no. 3、定義 3、および*可換代数*、章 II, § 2, no. 6、命題 13)。したがって、述べられている条件は、素数イデアル含む $a$ の $A$ 共通部分のすべてのイデアル $a$ が、最大イデアル含む $a$ の共通部分に等しいことを意味します。この条件は、$A$ がジェイコブソン環である場合、$A$ のすべての理想$a$ に明らかに当てはまります。逆に、$A$ のすべての素イデアルに当てはまる場合、$A$ は定義によるジェイコブソン環です。

#### 系 {#ac-v-s3-n4-cor-1 .statement tag=04RI}

*$A$ をジェイコブソン環とします。 $A$ のすべての理想 $a$ に対して、$a$ の根基は、$A$ 含む $a$ の最大理想の共通部分です。*

$A/a$ がジェイコブソン環であることに注意するだけで十分です。

#### 命題 4 {#ac-v-s3-prop-4 .statement tag=04RJ}

*$A$を主イデアル整域、$(\mathbf{p}_\lambda)_{\lambda \in L}$を$A$の極値元の代表系とする（*代数*、章VII, § 1, no. 3、定義2）。 $A$ がジェイコブソン環であるためには、$L$ が無限であることが必要かつ十分です。*

$A$ の最大の理想は $A\mathbf{p}_\lambda$ (*上記引用*、no. 2、命題 2) です。 $L$ が有限である場合、その共通部分は理想的な $Ax$ であり、ここで $x = \prod_{\lambda \in L} \mathbf{p}_\lambda$ (*同上*) であるため、$(0)$ とは異なります。一方、$L$ が無限の場合、$A\mathbf{p}_\lambda$ の共通部分は $(0)$ であり、$A$ のすべての元 $\neq 0$ は、極値元の有限数でのみ割り切れます。 (*上記引用*、no. 3、定理 2)。 命題は、$(0)$ が $A$ で最大ではない唯一の素イデアルであるという事実から導かれます (*代数*, 章 VI, § 1, no. 13, 命題 14 (DIV))。

#### 命題 5 {#ac-v-s3-prop-5 .statement tag=04RK}

*$A$を環、$B$を$A$上の$A$-代数積分とする。 $A$ がジェイコブソン環である場合、$B$ も同様です。*

置き換えること $A$ は、$B$ の標準像により、$A \subset B$ と仮定できます。 $\mathfrak{p}'$ を $B$ の主な理想とし、$\mathfrak{p} = A \cap \mathfrak{p}'$ とします。 仮定までに、共通部分が頂点に等しい$A$ の最大理想の家族 $(\mathfrak{m}_\lambda)_{\lambda \in L}$ が存在します。すべての$\lambda \in L$には、$\mathfrak{m}_\lambda$と含む$\mathfrak{p}'$の上に$B$の最大理想$\mathfrak{m}'_\lambda$が存在します（§ 2, no. 1、命題1、系2から定理まで） 1)。 $\mathfrak{q}' = \bigcap_{\lambda \in L} \mathfrak{m}'_\lambda$ と書くと、$\mathfrak{q}' \cap A = \bigcap_{\lambda \in L} \mathfrak{m}_\lambda = \mathfrak{p}$ と $\mathfrak{q}' \supset \mathfrak{p}'$、よって $\mathfrak{q}' = \mathfrak{p}'$ ($2$、no. 1、系 1 ～ 命題 1) となります。

#### 定理 3 {#ac-v-s3-thm-3 .statement tag=04RL}

*$A$ をヤコブソン環、$B$ を有限生成された $A$-代数、$\varphi : A \to B$ 標準準同型とします。次に:*
(i) *$B$ はジェイコブソン環です。*
(ii) *$B$ のすべての最大イデアル $m'$ について、$m = \varphi^{-1}(m')$ は $A$ の最大イデアルであり、$B/m'$ は $A/m$ の有限代数拡大です。

$\mathfrak{p}'$ を $B$ と $\mathfrak{p} = \varphi^{-1}(\mathfrak{p}')$ の主要な理想とする。 $v$ を $B/\mathfrak{p}'$ の元 $\neq 0$ とします。

As $B/p'$ is a finitely generated integral (Alp)-algebra and the canonical homomorphism $\phi : A/p \to B/p'$ is injective, there exists an element $u \neq 0$ of $A/p$ such that, for every homomorphism $f$ from $A/p$ to an algebraically closed field $L$ whose kernel does not contain $u$, there exists a homomorphism $g$ from $B/p'$ to $L$ whose kernel does not contain $v$ and for which $f = g \circ \phi$ (no. 1, Corollary 3 to Theorem 1). $A$ はジェイコブソン環であるため、$A$ 含む $p$ の最大理想 $m$ が存在し、そのような $u \notin m/p$ が存在します。 $L$ を $A/m$ の代数閉包とし、$f$ を標準準同型 $A/p \to L$ とします。させて

$$
g : B/p' \to L
$$

$f = g \circ \phi$ と $g(v) \neq 0$ となるように準同型になります。それから

$$
A/m \subset g(B/p') \subset L,
$$

したがって、$g(B/p')$ は $K$ の部分体 (代数、章 V, § 3, no. 2、命題 3) であり、$g$ の核は含むではなく$B/p'$ の最大理想です。 $v$。したがって、$B/p'$ の最大イデアルの共通部分が 0 に削減されることがわかり、これは $B$ がヤコブソン環であることを証明します。さらに、$p'$ が最大である場合、$g$ は必然的に単射的であるため、$p = m$ が最大になります。最終的に $B/p'$ は、体 $A/m$ にわたって有限に生成された代数となり、したがって、$A/m$ (no. 1、系 2 ～ 定理 1) の有限拡大になります。

#### 系 1 {#ac-v-s3-thm-3-cor-1 .statement tag=04RM}

*$\mathbf{Z}$ 上で有限に生成されるすべての代数 $A$ は、ジェイコブソン環です。素理想 $p \subset A$ が最大になるためには、環 $A/p$ が有限であることが必要かつ十分です。*

整域 $A/p$ が有限である場合、それは体です。$A/p$ のすべての $u \neq 0$ に対して、$A/p$ の写像 $v \mapsto uv$ はそれ自体に対して単射であり、$A/p$ が有限であるため全単射です。逆に、$A$ のすべての最大イデアル $m$ について、$A$ の $m$ の逆像は最大イデアル ($p$) であり、$A/m$ は素数体 $\mathbf{Z}/(p) = \mathbf{F}_p$ by 定理 3 に対して有限です。

#### 系 2 {#ac-v-s3-thm-3-cor-2 .statement tag=04RN}

*$(P_\lambda)_{\lambda \in L}$ を $\mathbf{Z}[X_1, \ldots, X_n]$ の多項式の族とし、$Q$ を $\mathbf{Z}[X_1, \ldots, X_n]$ の多項式とし、元 $(x_i)_{1 \leq i \leq n}$ 所属から有限体のすべての系について、すべての$P_\lambda(x_1, \ldots, x_n) = 0$ について$\lambda$、$Q(x_1, \ldots, x_n) = 0$も。 そして、$P_\lambda$が生成する$\mathbf{Z}[X_1, \ldots, X_n]$の理想を$a$とすると、$Q^m \in a$となるような整数$m > 0$が存在します。 さらに、すべての$\lambda$に対して$P_\lambda(y_1, \ldots, y_n) = 0$、また$Q(y_1, \ldots, y_n) = 0$となるように、$R$の元のすべての減少環$R$とすべての系$(y_i)_{1 \leq i \leq n}$について。

2 番目の主張は、$P(y_1, \ldots, y_n) = 0$ 含む $a$ となる多項式 $P$ の $\mathbf{Z}[X_1, \ldots, X_n]$ からなるの理想から最初の主張に続きます。最初の主張を示すには、$A = \mathbf{Z}[X_1, \ldots, X_n]$ 含む $a$ のすべての最大理想 $m$ について、$A/m$ は有限体 (系 1) であり、仮定は標準像を意味することに注意するだけで十分です。 $A/m$の$Q$は零です。次に、$A$ 含む $a$ の最大理想の $Q$ 属するから共通部分 、つまり $a$ の根基 (系から命題 3) です。

#### 系 3 {#ac-v-s3-thm-3-cor-3 .statement tag=04RO}

*$A$をジェイコブソン環とします。有限生成された $A$-代数 $B$ 含む $A$ が存在し、それが体である場合、 $A$ は体であり、 $B$ は $A$ の代数拡大です。

定理を適用する 3 (ii) を$m' = (0)$ とすれば十分です。

### 練習問題 {#ac-v-s3-exercises}

$A$ のすべての素イデアル $\mathfrak{p}$ に対して、$\mathfrak{p}$ の上にある $A'$ の素イデアル $\mathfrak{p}'$ が存在します。 *不条理な還元*による議論: $x \in A' \cap \mathfrak{g}A$ と $a = A \cap (x^{-1}A)$ とします。これは、$A$ とは異なる理想です。 $\mathfrak{p}$ を $A/a$ に関連付けられた主要な理想とします。したがって、トランスポーター $b = a : \mathfrak{p}$ は $a$ (章 IV, § 1, no. 4、命題 9) とは区別され、したがって $xy \notin A$ となるような $y \in b$ が存在し、
$$
xy \mathfrak{p} \subset \mathfrak{p}A' \cap A = \mathfrak{p};
$$
矛盾を推測します。）

**93**

[§ 3 に対して練習問題](exercises/s3/)を参照してください。
