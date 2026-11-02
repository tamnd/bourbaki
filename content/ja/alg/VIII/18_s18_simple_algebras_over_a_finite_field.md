---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Semisimple Modules and Rings
section: 18
section_title: Simple Algebras over a Finite Field
lang: ja
source: alg-viii
source_edition: 2023, Springer Nature
book_pages: A VIII.355-A VIII.360
pdf_pages: 0372-0377
extraction: native+ocr
subsections:
    - "no": 1
      title: Polynomials over a Finite Field
      page: 355
      pdf_page: 372
    - "no": 2
      title: Simple Algebras over Finite Fields
      page: 357
      pdf_page: 374
statements: 10
exercises: 7
content_sha256: 4e45e5db4902280b2bf2871fc545ce5a5a0ace03e8bbb8797a4c47718f07ead7
translated_from: content/en/alg/VIII/18_s18_simple_algebras_over_a_finite_field.md
translation_method: google
source_content_sha256: 54d2a6b31a60bad387aff00416b44414a3612b96aff88b09c11c2b91d78d43d8
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-b071ad41
glossary_version: 34
glossary_terms_sha256: 75dab4046b5cede522d1ccb15dc437e6ebb6aa7c2858d613d3bc335c3bb1f9b3
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## § 18。 単純代数有限体を超える

### 1. 有限体を超える多項式

#### 定理 1 (シュバレー – 警告) {#alg-viii-s18-thm-1 .statement tag=00SA}

K を特性 $p$ の有限可換体とします。 $n$ を整数 $\geqslant 1$ とし、$(f_i)_{i\in I}$ を $K[X_1, . . . ,X_n]$ の非零元の有限族とします。 $i\in I$ に対して $f_i(\mathbf{x}) = 0$ が得られるように、元の Z 集合 $K^n$ の $\mathbf{x}$ で表します。 $n >\sum_{i\in I}$ 度($f_i$) がある場合、Z の基数は $p$ で割り切れます。

#### 補題 1 {#alg-viii-s18-lem-1 .statement tag=00LB}

Lを体、Gを有限群、$\chi$をGから乗法群$L^*$までの自明でない準同型とします。 $\sum_{x\in G}\chi (x) = 0$があります。

仮定までに、$\chi (a)\not= 1$ となる G の元 $a$ が存在します。 $a$ による乗法は G の置換であるため、次のようになります。

$$
\sum_{x\in G}\chi (x) =\sum_{x\in G}\chi (ax) =\chi (a)\sum_{x\in G}\chi (x)
$$

これにより、補題 1 が得られます。

#### 補題 2 {#alg-viii-s18-lem-2 .statement tag=00LC}

$q$ を K の基数とします。任意の整数 $m\geqslant 0$、集合 $S_m=$ $\sum_{x\in K}x^m$ について。 $m$ が $q-1$ の非零倍数である場合、$S_m=-1$ となり、その他の場合は $S_m= 0$ になります。

$0^0= 1$ (I, §2, No. 1、p. 14) を思い出してください。 $m$ が $q-1$ の倍数であるとします。 アーベル群 $K^*$ には位数 $q-1$ があるため、$x\in K^*$ と $S_m= 0^m+ (q-1)\cdot 1$ ごとに $x^m= 1$ があり、この場合は主張になります。

$m$ が $q-1$ の倍数ではないとします。 $x\in K^*$の場合は集合 $\chi (x) =x^m$。 乗法群 $K^*$ は位数 $q-1$ (V, §12, No. 1, p. 93, 命題 1) の巡回なので、 $\chi(a) \neq 1$ となるような $K^*$ の元 $a$ が存在します。 補題 1 が $G = K^*$ に適用されるまでに、
$$
S_m = 0^m + \sum_{x \in K^*} \chi(x) = 0;
$$
これにより、補題 2 が得られます。

定理 1 を証明しましょう。 $\mathbf{x} = (x_1, \ldots, x_n)$ を $K^n$ の元とします。 $f_i(\mathbf{x}) \neq 0$の場合は$1 - f_i(\mathbf{x})^{q-1} = 0$、$f_i(\mathbf{x}) = 0$の場合は$1 - f_i(\mathbf{x})^{q-1} = 1$があります。 集合 $P = \prod_{i=1}^r (1 - f_i^{q-1})$。私たちは持っています
$$
P(\mathbf{x}) = \begin{cases}
1 & \text{if } \mathbf{x} \in \mathbf{Z}, \\
0 & \text{if } \mathbf{x} \notin \mathbf{Z}.
\end{cases}
$$
多項式 $P$ を $\sum_{\alpha \in \mathbf{N}^n} c_\alpha X^\alpha$ として拡張してみましょう。 仮定までに、次数 $< (q-1)n$ になります。 $\alpha$ を $\mathbf{N}^n$ の元として、$c_\alpha$ が非零となるようにします。 $\alpha_1 + \cdots + \alpha_n < (q-1)n$ があるので、$1 \leq \ell \leq n$ と $0 \leq \alpha_\ell < q-1$ のような整数 $\ell$ が存在します。 補題 2 までに $\sum_{x \in K} x^{\alpha_\ell} = 0$ になるため、
$$
\sum_{\mathbf{x} \in K^n} \mathbf{x}^\alpha = \prod_{j=1}^n \left( \sum_{x \in K} x^{\alpha_j} \right) = 0.
$$
その結果、
$$
\sum_{\mathbf{x} \in K^n} P(\mathbf{x}) = \sum_{\alpha \in \mathbf{N}^n} c_\alpha \left( \sum_{\mathbf{x} \in K^n} \mathbf{x}^\alpha \right) = 0.
$$
さて、公式 (1) により、$\sum_{\mathbf{x} \in K^n} P(\mathbf{x}) = \operatorname{Card}(\mathbf{Z}) \cdot 1$ が得られ、従って $\operatorname{Card}(\mathbf{Z}) \cdot 1 = 0$ になります。これは、$\operatorname{Card}(\mathbf{Z})$ が $p$ で割り切れることを意味します。

#### 系 {#alg-viii-s18-n1-cor-1 .statement tag=00LD}

*$V$を有限次元の$n$の$K$と$I$を有限の集合のベクトル空間とし、各$i \in I$について、$F_i : V \to K$を次数の同次多項式写像とする$d_i > 0$。 $\sum_{i \in I} d_i < n$ がある場合、$i \in I$ ごとに $F_i(x) = 0$ となるように、$V$ の非零元 $x$ が存在します。

$(e_1, \ldots, e_n)$ を $V$ の $K$ の基底とします。 同次多項式写像の定義 (IV, §5, No. 9, p. 55, 定義 3) により、$i \in I$ ごとに、次数 $d_i$ の $K[X_1, \ldots, X_n]$ に同次多項式 $f_i$ が存在します。 $F_i(\xi_1 e_1, \ldots, \xi_n e_n) = f_i(\xi_1, \ldots, \xi_n)$ があります。 $Z$ を元の集合、$V$ の $x$ とし、$i \in I$ ごとに $F_i(x) = 0$ とします。 定理 1 により、$Z$ の基数は $p$ で割り切れ、$0$ 属するから $S$ なので、$\operatorname{Card}(Z) \geq p > 1$ になります。

### 2. 有限体を超える単純代数

#### 定理 2 (ウェダーバーン) {#alg-viii-s18-thm-2 .statement tag=00SB}

すべての有限体は可換です。

D を有限体、K をその中心とします。 K-代数 D は次数 $m^2$ の中心単純であり、$m$ は厳密には正の整数です。 被約ノルムは次数 $m$ (VIII, p. 345, 命題 6) の同次多項式写像 Nrd$: D\rightarrow K$ であり、D のすべての $a\not= 0$ に対して Nrd($a$)$\not= 0$ が得られます。 (VIII、p. 340、命題 3)。上記の系は、$m\geqslant m^2$、つまり $m= 1$ を意味します。従って、D = K となります。

#### 系 1 {#alg-viii-s18-thm-2-cor-1 .statement tag=00LE}

すべての有限単純環は行列環 $\mathbf{M}_n(L)$ と同型であり、$n$ は厳密には正の整数であり、L は有限可換体です。

これは、定理 2 と構造定理の単純な環 (VIII、p. 120、定理 1) に続きます。

#### 系 2 {#alg-viii-s18-thm-2-cor-2 .statement tag=00LF}

K を有限の可換体とします。 K 上のすべての中心単純代数は行列環 $\mathbf{M}_n(K)$ と同型であり、$n$ は厳密には正の整数です。

これは、中央の単純代数 (VIII、p. 252、定理 1) の定理 2 および構造定理に続きます。

#### 注意 1 {#alg-viii-s18-n2-rem-1 .statement tag=00LG}

定理の他の証明です。 2. D を有限体とし、K をその中心とし、L を D の最大可換部分体とします。 $x$ を元とします$D^*$。 D の属するから最大可換部分体 $L_1$ です。等式があります

$$
[D : K] = [L : K]^2= [L_1: K]^2
$$

系 2 の VIII、p. 265、従って $[L : K] = [L_1: K]$ によって。 命題により、K の V, §12, No. 2、p. 94、拡大 L、$L_1$ の 3 つが同型です。 VIII、p. 263、系までに、$aLa^{-1}= L_1$となる$D^*$の元$a$が存在するため、$a^{-1}xa$属するからLまでとなります。従って、$y\in L^*$ ごとに $(ay)^{-1}x(ay) =a^{-1}xa$ が得られます。従って、S が $D^*$ モジュロ $L^*$ の左剰余類の代表の集合である場合、$D^*-\{1\}$ のすべての元は、$s\in S$ と $x\in L^*-\{1\}$ を使用して $sxs^{-1}$ として書くことができます。 $D^*$の位数を$d$で表し、$L^*$のそれを$\ell$で表します。 S の基数は $d/\ell$ に等しいので、$d-1\leqslant (d/\ell )(\ell -1) =d-d/\ell$ になります。従って、$\ell =d$、つまり L = D となり、体 D が可換であることが証明されます。

#### 注意 2 {#alg-viii-s18-n2-rem-2 .statement tag=00LH}

L を次の性質で可換体とします: $(C_1)$ V を有限次元 $n$ のベクトル空間を体 L 上にして、$d$ とします$0< d < n$ になるようにしてください。 次数 $d$ のすべての同次多項式写像 $F : V\rightarrow L$ に対して、$F(x) = 0$ となる V の非零元 $x$ が存在します。

定理 2 の証明は、中心 L を含む L を超える有限次数のすべての体が L に等しいことを示します。

VIII、p. 356 の系までに、すべての有限体には性質 $(C_1)$ が含まれます。私たち証明できる (VIII, p. 360, 練習問題 7) は、次の体が性質 $(C_1):$ を持っています。

– 有限体のすべての代数拡大

– 代数閉体の係数を含む 1 つの変数内の有理分数のすべての体 (ツェンの定理)。

– $*$すべての体には、完全な個別の評価が付与されており、

その剰余体は代数的に閉じています (VIII, p. 332, 練習問題 17)$.*$

#### 注意 3 {#alg-viii-s18-n2-rem-3 .statement tag=00LI}

体 K が次の条件を満たすとします。

– L が有限次数の K の拡大である場合、それは巡回的であり、ノルム写像 $N : L^*\rightarrow K^*$ は全射的です。

この条件は、特に体 K が有限 (V, §12, No. 2、p. 95、命題 4) の場合に満たされます。次に、中心 K を使用して K を超える有限次数のすべての体が K に等しいことを証明できます (練習問題 VIII の 10、p. 329)。

### 練習問題 {#alg-viii-s18-exercises}

[§ 18 に対して練習問題](exercises/s18/)を参照してください。
