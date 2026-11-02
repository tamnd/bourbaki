---
book: alg
book_title: Algebra
chapter: IV
chapter_title: POLYNOMIALS AND RATIONAL FRACTIONS
section: 6
section_title: Symmetric functions
lang: ja
source: alg-iv-vii
source_edition: 2003, Springer
book_pages: A IV.98-A IV.105
pdf_pages: 0070-0095, 0107-0114
extraction: ocr
subsections:
    - "no": 1
      title: Symmetric polynomials
      page: 61
      pdf_page: 70
    - "no": 2
      title: Symmetric rational fractions
      page: 67
      pdf_page: 76
    - "no": 3
      title: Symmetric formal power series
      page: 67
      pdf_page: 76
    - "no": 4
      title: Sums of powers
      page: 70
      pdf_page: 79
    - "no": 5
      title: Symmetric functions in the roots of a polynomial
      page: 72
      pdf_page: 81
    - "no": 6
      title: The resultant
      page: 75
      pdf_page: 84
    - "no": 7
      title: The discriminant
      page: 81
      pdf_page: 90
statements: 43
exercises: 15
errata:
    - says: then $w$ is an automorphism of the $A$-module $S_q \times S_p$
      read: then $\omega$ is an automorphism of the $A$-module $S_q \times S_p$
      why: The map is introduced as omega in the same sentence — "if we write omega(u, v) = (u, uh + v) ... then w is an automorphism" — and the display that follows on page 86 gives its inverse as omega^{-1}(u, v). The French of 2007 (A IV.71) sets omega throughout.
    - says: The matrix of $w$ with respect to the basis $B_1$
      read: The matrix of $\omega$ with respect to the basis $B_1$
      why: Same automorphism as the display above it, which page 86 sets round.
    - says: $\varphi \circ w$ maps $(u, v)$ to $u(f + gh) + vg$
      read: $\varphi \circ \omega$ maps $(u, v)$ to $u(f + gh) + vg$
      why: Same automorphism, composed with phi. Page 86 sets phi round and the omega beside it roman.
    - says: representing $\varphi$ and $\varphi \circ w$ have the same determinant and this follows from the relation $\det w = 1$
      read: representing $\varphi$ and $\varphi \circ \omega$ have the same determinant and this follows from the relation $\det \omega = 1$
      why: The last two occurrences of the same automorphism on page 86, both roman.
content_sha256: cd8476018692047dc0105f2479f5b3a01a1c7b26912e17347e9cceb0cc570974
translated_from: content/en/alg/IV/06_s6_symmetric_functions.md
translation_method: google
source_content_sha256: b6c3b59be706d899df8c14677f2a1f585996a74c952028c811d04e381a1ed6be
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-eeeca2ef
glossary_version: 34
glossary_terms_sha256: 5f6385cd6972839e9e0a01f1614199ef2f73d5687670508114032db09ca085ef
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## § 6。対称写像

### 1. 対称多項式

$n$を正の整数とします。 置換 $\sigma \in \mathfrak{S}_n$ ごとに、$\varphi_\sigma$ を A-代数 $A[X_1, \ldots, X_n]$ の自己同型とし、$1 \leq i \leq n$ に対して写像 $X_i$ から$X_{\sigma(i)}$ とします。 $\sigma \mapsto \varphi_\sigma$が$\mathfrak{S}_n$の準同型から$A[X_1, \ldots, X_n]$の自己同型の群であることは明らかです。 $\sigma \in \mathfrak{S}_n$と$f \in A[X_1, \ldots, X_n]$には$\sigma f = \varphi_\sigma(f)$を入れます。多項式 f は、すべての $\sigma \in \mathfrak{S}_n$ に対して $\sigma f = f$ の場合、対称であると言われます。対称多項式形 $A[X_1, \ldots, X_n]$ の単位段階化部分代数 ;この段落の残りの部分では、それを $A[X_1, \ldots, X_n]^{\mathrm{sym}}$ で表します。
すべての正の整数 k を、集合 $\{1, 2, \ldots, n\}$ の k 要素部分集合の $\mathfrak{P}_k$ 集合で表し、次のようにします。

(1)
$$
s_k = \sum_{H \in \mathfrak{P}_k} \prod_{i \in H} X_i .
$$

整数 n を指定したい場合は、$s_k$ の代わりに $s_{k,n}$ と書きます。私たちは特に

$$
\begin{aligned}
s_0 &= 1 \\
s_1 &= \sum_{1 \leq i \leq n} X_i \\
s_2 &= \sum_{1 \leq i < j \leq n} X_i X_j \\
&\ \ \cdots \cdots \cdots \cdots \cdots \\
s_n &= X_1 \ldots X_n
\end{aligned}
$$

$k > n$ の場合は $s_k = 0$ です。 $s_k$ が次数 k の同次対称多項式であることは明らかです。これを次数 k の初等対称多項式と呼ぶことにします。
環 $A[X_1, \ldots, X_n, U, V]$ には関係があります

(2)
$$
\prod_{i=1}^{n} (U + V X_i) = \sum_{k=0}^{n} U^{n-k} V^k s_k ;
$$

適切な置換により、関係と推定されます。

(3)
$$
\prod_{i=1}^{n} (1 + T X_i) = \sum_{k=0}^{n} s_k T^k ,
$$

(4)
$$
\prod_{i=1}^{n} (\mathbf{X} - \mathbf{X}_i) = \sum_{k=0}^{n} (-1)^{n-k} s_{n-k} \mathbf{X}^k .
$$

#### 定理 1 {#alg-iv-s6-thm-1 .statement tag=06EE}

— $E = A[\mathbf{X}_1, \ldots, \mathbf{X}_n]$ と $S = A[\mathbf{X}_1, \ldots, \mathbf{X}_n]^{\text{sym}}$ を置いてみましょう。

a) 対称多項式の$A$代数$S$は$s_1, \ldots, s_n$によって生成されます。

b) $E$ の元 $s_1, \ldots, s_n$ は、$A$ (IV, p. 4) に対して代数的に独立しています。

c) $1 \leq i \leq n$ の $0 \leq \nu(i) < i$ が $S$ 加群 $E$ の基底となるような単項式 $X^\nu = X_1^{\nu(1)} \ldots X_n^{\nu(n)}$ の族。特に、$E$ は、階数 $n!$ の無料の $S$ モジュールです。

$n$ の帰納法によって定理を証明しますが、$n = 0$ の場合は自明です。 $X_1, \ldots, X_{n-1}$ の次数 $k$ の初等対称多項式を $B = A[X_n]$ と書き、$s_k'$ で表します。したがって、$B[X_1, \ldots, X_{n-1}] = A[X_1, \ldots, X_n]$ となります。 Th の主張で $n-1$ によって置き換える $n$ が、$B$ によって $A$ とすると、 1、帰納法の仮定は次のように定式化できます。

(A) $X_1, \ldots, X_{n-1}$ のすべての置換の下で不変な多項式 $f \in A[\mathbf{X}_1, \ldots, \mathbf{X}_n]$ の $B$-代数 $S'$ は、$s_1', \ldots, s_{n-1}'$ によって生成されます。

(B) $E$ の元 $s_1', \ldots, s_{n-1}'$ は、$B$ に対して代数的に独立しています。

(C) $1 \leq i \leq n-1$ の $0 \leq \nu(i) < i$ が $S'$ 加群 $E$ の基底となるような単項式 $X_1^{\nu(1)} \ldots X_{n-1}^{\nu(n-1)}$ 族。

明らかな関係があります

(5)
$$
s_k = s_k' + s_{k-1}' X_n \quad (1 \leq k \leq n-1),
$$
$k$の帰納法までに入手します

(6)
$$
s_k' = (-1)^k X_n^k + \sum_{i=1}^k (-1)^{k-i} s_i X_n^{k-i} \quad (1 \leq k \leq n-1).
$$

$S \subset S'$ があるため、$s_1, \ldots, s_n$ 属するから $S'$ となります。 (A) と公式 (6) により、B 代数 $S'$ は $s_1, \ldots, s_{n-1}'$ によって生成されます。

(B) により、次のような B 代数 $S'$ の自己準同型 $\mu$ が存在します。

(7)
$$
u(s_k') = (-1)^k X_n^k + \sum_{i=1}^k (-1)^{k-i} s_i' X_n^{k-i} \quad (1 \leq k \leq n-1).
$$

(5) により、簡単に計算すると $u(s_k) = u(s_k') + u(s_{k-1}') X_n$、よって $u(s_k) = s_k'$ となります。 $P \in B[Y_1, \ldots, Y_{n-1}]$ にしましょう。次に、$P(s_1, \ldots, s_{n-1}) = 0$ から推測します
$$
0 = u(P(s_1, \ldots, s_{n-1})) = P(s_1', \ldots, s_{n-1}'),
$$
よって $P = 0$ by (B)。したがって、B 代数 $S'$ は代数的に独立した元 $s_1, \ldots, s_{n-1}$ によって生成されます。この性質は次のように再定式化できます。
(D) $A$-代数 $S'$ は、代数的に独立した元 $s_1, \ldots, s_{n-1}, X_n$ によって生成されます。

したがって、同一視する S' を多項式環 $C[X_n]$ で表すことができます。ここで、$C$ は、$s_1, ..., s_{n-1}$ によって生成される E の部分 A 代数です。

a) を証明するには、$f \in S$ を次数 $m$ の同次対称多項式とする。 $f \in S' = C[X_n]$ があるので、$X_1, ..., X_n$ の次数 $m$ と同次の C の元 $g = P(s_1, ..., s_{n-1})$ が存在し、$f - g$ は $X_n$ で割り切れます。 $f - g$ は対称なので、その項も $X_1, ..., X_{n-1}$ で割り切れ、よって $f - g$ は $s_n = X_1 ... X_n$ で割り切れます。他の語には、$f = g + hs_n$、よって、$\deg h < m$という$h \in S$が存在します。 $m$ の帰納法までに、$f$ 属するは次のようになります。

$$
C[s_n]_E = A[s_1, ..., s_{n-1}, s_n]_E .
$$

したがって、A-代数 S は $s_1, ..., s_n$ によって生成されることがわかりました。

次に b) を証明します。 (4) の $X$ を $X$ に置き換えると、次のようになります。

$$
(-1)^{n+1}s_n = X_n^n + \sum_{k=1}^{n-1} (-1)^{n-k} s_{n-k} X_n^k ;
$$

他の語、$(-1)^{n+1}s_n$ は、$X$、次数 $n$、および $C$ の係数のモニック多項式です。 By IV, p. 11 we thus have the following property :
(E) The C-algebra homomorphism $\varphi$ of $C[T]$ into $C[X_n] = S'$ which maps T to $s_n$ is injective, and $S'$ is a free module over the image of $\varphi$, with basis $(1, X_n, ..., X_n^{n-1})$.

$C$ の元 $s_1, ..., s_{n-1}$ は、A に対して (D) により代数的に独立しています。したがって、$\varphi$ の単射性は、$s_1, ..., s_{n-1}, s_n$ が A、よって b) に対して代数的に独立であることを意味します。

c)を証明するには、$\varphi$の像は$C[s_n]_E = S$に等しいので、(E)より、$S'$は基底$(1, X_1, ..., X_n^{n-1})$上のSよりも自由加群です。さて、主張 c) は、帰納法の仮定 (C) およびII、p. 222 の提案 25 から続きます。これで証明は完了です。

$f$ を $X_1, ..., X_n$ の対称多項式、次数 $m$ の同次多項式とします。 Thさんより1 (IV, p. 62) $f = Q(s_1, ..., s_n)$ となるような多項式 $Q \in A[Y_1, ..., Y_n]$ が存在します。前述の証明は、$n$ と $m$ の 2 倍の帰納法により、$Q$ を明示的に計算する手段を提供します。というのは、これまで見てきたように、多項式 $P \in A[Y_1, ..., Y_{n-1}]$ と次数 $m-n$ の同次である $X_1, ..., X_n$ に対称な多項式 h が存在します。

$$
f = P(s_1, ..., s_{n-1}) + s_n h .
$$

すべての多項式 $u \in A[X_1, ..., X_n]$ に対して、

$$
u'(X_1, ..., X_{n-1}) = u(X_1, ..., X_{n-1}, 0)
$$

この場合、$s'_1, ..., s'_{n-1}$ は $X_1, ..., X_{n-1}$ と公式の初等対称多項式です (8) が意味します。

$$
f' = P(s'_1, ..., s'_{n-1})
$$

したがって、$P$ の決定は、$n - 1$ 不定数の対称多項式の計算に帰着され、$h$ は (8) から得られます。

方法を 2 つの例で説明します。

**例。 — 1)** $n = 3$ とします

$$
f = X_1^2(X_2 + X_3) + X_2^2(X_3 + X_1) + X_3^2(X_1 + X_2).
$$

我々は持っています

$$
f' = X_1^2X_2 + X_1X_2^2 = X_1X_2(X_1 + X_2) = s'_1s'_2.
$$

$g = f - s_1s_2$ と書きましょう。我々は持っています

$$
g = f - (X_1 + X_2 + X_3)(X_1X_2 + X_1X_3 + X_2X_3) = -3X_1X_2X_3,
$$

それでついに

$$
f = s_1s_2 - 3s_3.
$$

2) もう一度$n = 3$にして、$p = X_1^3 + X_2^3 + X_3^3$を置きます。
$p(X_1, 0, 0) = X_1^3 = s_1(X_1, 0, 0)^3$ があります。 $q = p - s_1^3$と書くと、次のようになります。

$$
q = -3f - 6X_1X_2X_3 = -3s_1s_2 + 3s_3
$$

そして最後に

$$
p = s_1^3 - 3s_1s_2 + 3s_3.
$$

$S_1, ..., S_n$ を不定とする。多項式代数 $A[S_1, ..., S_n]$ に型 $N$ の目盛を装備し、その $S_k$ は $1 \leq k \leq n$ (IV, p. 3) の重み $k$ であり、次のように装備します。 $A[X_1, ..., X_n]$ いつもの卒業式。 $1 \leq k \leq n$ の場合、$X_1, ..., X_n$ の初等対称多項式 $s_{k,n}$ は次数 $k$ と同次です。 Thさんより1 (IV, p. 62) 写像 $g \mapsto g(s_{1,n}, ..., s_{n,n})$ は、等級付けされた代数の同型です

$$
\varphi_n : A[S_1, ..., S_n] \to A[X_1, ..., X_n]^{\text{sym}}
$$

$m$ を整数とし、$0 \leq m \leq n$ とします。 $1 \leq k \leq m$ となるような整数 $k$ ごとに、

$$
s_{k,m}(X_1, ..., X_m) = s_{k,n}(X_1, ..., X_m, 0, ..., 0)
$$

$s_k$ の定義 (IV, p. 61, 公式 (1)) による。したがって図式

$$
\begin{array}{ccc}
A[S_1, ..., S_m] & \xrightarrow{j} & A[S_1, ..., S_n] \\
\varphi_m \downarrow & & \varphi_n \downarrow \\
A[X_1, ..., X_m]^{\text{sym}} & \xleftarrow{p} & A[X_1, ..., X_n]^{\text{sym}}
\end{array}
$$

(ここで、 j は正規包含を表し、 $p$ 準同型
$$
g \mapsto g (X_1, \ldots, X_m, 0, \ldots, 0)
$$
可換です。

#### 命題 1 {#alg-iv-s6-prop-1 .statement tag=06EF}

*正の整数 k, n のすべての対について、$S_k^{(n)}$ を、次数 k の同次である $X_1, \ldots, X_n$ のすべての対称多項式の A-加群からなるとします。 整数 m が $0 \leq k \leq m \leq n$ を満たす場合、写像 $f \mapsto f (X_1, \ldots, X_m, 0, \ldots, 0)$ は $S_k^{(m)}$ 上の $S_k^{(n)}$ の同型です。

図式 (10) の可換性によって、$S_1, \ldots, S_n$ の重み k のすべての等重多項式が、仮説 $0 \leq k \leq m \leq n$ の下で$S_1, \ldots, S_m$ にのみ依存することを示すだけで十分です。ここで、単項式 $S_1^{\alpha(1)} \cdots S_n^{\alpha(n)}$ の重みは整数 $\alpha(1) + 2\alpha(2) + \ldots + n\alpha(n)$ に等しくなります。 整数 $\alpha(1), \ldots, \alpha(n)$ は正なので、関係
$$
\alpha(1) + 2\alpha(2) + \cdots + n\alpha(n) = k \leq n
$$
$k < j \leq n$、よって主張の $\alpha(j) = 0$ を暗示します。

#### 例 3 {#alg-iv-s6-n1-exa-3 .statement tag=06EG}

上記のIV、p. 64、および提案 1 の例 2 により、次のようになります。
$$
\sum_{i=1}^n X_i^3 = s_{1,n}^3 - 3s_{1,n}s_{2,n} + 3s_{3,n}
$$
整数 $n \geq 3$ ごとに。 The commutativity of the diagram (10) moreover gives the formulae
$$
X_1^3 + X_2^3 = s_{1,2}^3 - 3s_{1,2}s_{2,2},
$$
$$
X_1^3 = s_{1,1}^3.
$$

#### 注意 {#alg-iv-s6-n1-rem-1 .statement tag=06EH}

— n と k を 2 正の整数とします。 $N^n$ の長さ k の元の $\Delta_{k,n}$ 集合で表し、さらに $A$ , に位数関係を備え、$a \leq \beta$ と書かれ、辞書編集上の位数によって引き起こされます。 $N^n$ (*集合理論*、III、p. 157)、および $N^n$ の群 $\mathfrak{S}_n$ の定義する作用 $\sigma \in \mathfrak{S}_n, a \in N^n$ の $(\sigma a)(i) = a(\sigma^{-1}(i))$ と$l \leq i \leq n$。 さらに、$D_k$ 集合 of 元 $a = (\alpha(1), \ldots, \alpha(k))$ of $\mathbf{N}^k$ で次のように表します。
$$
\alpha(1) \geq \alpha(2) \geq \cdots \geq \alpha(k), \quad \alpha(1) + \cdots + \alpha(k) = k.
$$

$k \leq n$ として、$N^n$ の部分集合を写像 $(a(1), \ldots, a(k)) \mapsto (a(1), \ldots, a(k), 0, \ldots, 0)$ で同一視する $\mathbf{N}^k$ とします。 次に、$D_k$ は、すべての $\sigma \in \mathfrak{S}_n$ に対して $\sigma a \leq a$ となるように、$\Delta_{k,n}$ の元 $a$ で構成されます。 したがって、$A$、 、$D_k$ の含む一意元の群 $\mathfrak{S}_n$ のすべての軌道が続きます。 すべての $a \in D_k$ について、$O(a)$ を $\mathfrak{S}_n$ の演算の下の $\Delta_{k,n}$ の $a$ の軌道とします。置く
$$
M(\alpha) = \sum_{\beta \in O(\alpha)} X^\beta.
$$

IV の補題 1、p. 47 から、家族 $(\mathbf{M}(\alpha))_{\alpha \in D_k}$ は A-加群 $S_k^{(n)}$ の基底であることがわかります。

それぞれ $\alpha \in D_k$ を入力します

$$
(12)\quad S(\alpha) = \prod_{i=1}^k s_i^{\alpha(i) - \alpha(i+1)} \quad \text{(where it is understood that } a\ (k+1) = 0 \text{)} ;
$$

$\sum_{i=1}^k i \cdot (a(i) - a(i+1)) = \sum_{i=1}^k a(i) = k$ があるので、対称多項式 $S(\alpha)$ は次数 $k$ と同次です。それはThから直接続きます。 1 (IV、p. 62) 家族 $(S(\alpha))_{\alpha \in D_k}$ は A-加群 $S_k^{(n)}$ の基底です。

$A = \mathbf{Z}$ と $k = n$ の場合、$D_k$ に $\alpha, \beta$ を、(12) で定義される多項式 $S(\alpha)$ の単項式 $X^\beta$ の係数を $c_{\alpha\beta}$ とします。これは、正の整数、*環 A および整数 n* から独立しています。 公式 (9) (IV, p. 64) までに、

$$
(13)\quad S(\alpha) = \sum_{\beta \in D_k} c_{\alpha\beta} \cdot \mathbf{M}(\beta) \quad (\alpha \in D_k) .
$$

行列 $C = (c_{\alpha\beta})_{\alpha,\beta \in D_k}$ は、$\alpha < \beta$ に対して $c_{\alpha\alpha} = 1$ および $c_{\alpha\beta} = 0$ となることが示されます (cf. IV、p. 101、練習問題 13)。 II、p. 351 で紹介した用語を一般化して、$C$ 属するを下総三角形群と言うことにします。 C の逆の行列 D にも同じことが当てはまります。 行列 C の値と $2 \leq k \leq 5$ のときの D は、表 (IV、p. 103-105) で与えられます。

今、$n < k$ として、$N^k$ の部分集合を写像 $(a(1), \ldots, a(n)) \mapsto (a(1), \ldots, a(n), 0, \ldots, 0)$ として、同一視する $N^n$ とします。 $D_k \cap N^n$ のすべての $a$ について、$\mathfrak{S}_n$ の演算と定義する $\mathbf{M}(\alpha)$ の下の $\Delta_{k,n}$ の $a$ の $O(\alpha)$ 軌道を (11) で表します。さらに (12) によって定義する $S(\alpha)$ を計算すると、家族 $(\mathbf{M}(a))_{a \in D_k \cap N^n}$ と $(S(a))_{a \in D_k \cap N^n}$ は A-加群 $S_k^{(n)}$ の基底になります。 IV, p. 64 の公式 (9) により、(13) と同様の公式が得られます。ここで、$D_k$ は、同じ整数 $c_{\alpha\beta}$ で $D_k \cap N^n$ に置き換えられます。

#### 例 4 {#alg-iv-s6-n1-exa-4 .statement tag=06EI}

IV、p. 65 の例 3 までに、

$$
\mathbf{M}(3,0,0) = S(3,0,0) - 3S(2,1,0) + 3S(1,1,1)
$$

整数 $n \geq 3$ ごとに、など

$$
\mathbf{M}(3,0) = S(3,0) - 3S(2,1)
$$

$n = 2$の場合。

### 2. 対称有理分数

$K$ を可換体とし、$X_1, X_2, \ldots, X_n$ を不定とします。すべての $\sigma \in S_n$ について、$K[X_1, X_2, \ldots, X_n]$ の No. 1 (IV、p. 61) 自己同型 $\varphi_\sigma$ で定義しました。この自己同型には拡大$\psi_\sigma$から体$K(X_1, \ldots, X_n)$までの固有の自己同型があり、$\sigma \mapsto \psi_\sigma$は$S_n$の単射準同型が$K(X_1, \ldots, X_n)$の自己同型群になります。それぞれの $f \in K(X_1, \ldots, X_n)$ には $(\psi_\sigma f)(X_1, \ldots, X_n) = f(X_{\sigma(1)}, \ldots, X_{\sigma(n)})$ があります。すべての $\sigma \in S_n$ に対して $\psi_\sigma(f) = f$ が対称となる有理分数 $f$ を対称有理分数と呼びます。 $X_1, \ldots, X_n$ のすべての対称有理分数の集合は、$K(X_1, \ldots, X_n)$ の部分体です。

#### 命題 2 {#alg-iv-s6-prop-2 .statement tag=06EJ}

— * $X_1, \ldots, X_n$ の対称有理分数の体は、$X_1, \ldots, X_n$ の対称多項式の環の分数の体です。

Let $f \in K(X_1, \ldots, X_n)$ be a symmetric rational fraction, and let $u_1, v_1$ be two elements of $K[X_1, \ldots, X_n]$ such that $f = \frac{u_1}{v_1}$. $v = \prod_{\sigma \in S_n} \psi_\sigma(v_1) \in K[X_1, \ldots, X_n]$ と $u = fv \in K[X_1, \ldots, X_n]$ を入れます。この場合、$v$ は対称です。したがって、$f$ が対称であるため、$u$ も対称となり、その結果は $f = \frac{u}{v}$、よってになります。

#### 系 {#alg-iv-s6-n2-cor-1 .statement tag=06EK}

— *$s_1, s_2, \ldots, s_n$ を $X_1, \ldots, X_n$ の初等対称多項式とします。すべての有理分数 $g \in K(S_1, S_2, \ldots, S_n)$ 数列 $(s_1, s_2, \ldots, s_n)$ は $g$ に代入可能であり、写像 $g \mapsto g(s_1, s_2, \ldots, s_n)$ は $K(S_1, S_2, \ldots, S_n)$ の同型を $X_1, \ldots, X_n$ の対称有理分数の体に代入できます。

これは、提案 2 と Th から導き出されます。 IV、p. 62 の 1。

### 3. 対称フォーマル冪系列

Let $I$ be a set, $X = (X_i)_{i \in I}$ a family of indeterminates and $A[[X]]$ the algebra of formal power series in the $X_i$. For every permutation $a \in S_I$ there exists a unique continuous automorphism $\varphi_a$ of the algebra $A[[X]]$ which maps $X_i$ to $X_{a(i)}$ for each $i \in I$ (IV, p. 28, Prop. 4); it is clear that $\sigma \mapsto \varphi_\sigma$ is a homomorphism of $S_I$ into the group of continuous automorphisms of the algebra $A[[X]]$. $f \in A[[X]]$ を正式な冪系列とします。 $af = \varphi_a(f)$ を置くと、形式的な冪系列 $f$ は、各 $\sigma \in S_I$ について $\sigma f = f$ であれば対称であると言えます。 The symmetric formal power series form a closed subalgebra of $A[[X]]$ which is denoted by $A[[X]]^{\text{sym}}$ and is equipped with the topology induced by that of $A[[X]]$.

T を不定数とします。形式的な冪系列 $A[[X, T]]$ の環では、族 $(X_i T)_{i \in I}$ は加算可能であるため、族 $(1 + X_i T)_{i \in I}$ は乗算可能です (IV, p. 27、提案 2)。さらに、私たちは持っています

$$
\prod_{i \in I} (1 + X_i T) = 1 + \sum_{k \geq 1} s_k T^k,
$$

ここで、形式的な冪系列 $s_k \in A[[X]]$ は次のように定義されます。

$$
s_k = \sum_{H \in \mathscr{P}_k} \left( \prod_{i \in H} X_i \right) \quad (k \geq 1)
$$

(すべての k 要素の $\mathscr{P}_k$ 集合、I の部分集合で表します)。特に$s_1 = \sum_{i \in I} X_i$があります。 I が $n$ 元で有限である場合、$k > n$ に対して $s_k = 0$ が得られます。より正確には、$I = \{1, \ldots, n\}$ のとき、形式的な冪系列 $s_k$ は、$X_1, \ldots, X_n$ の次数 k の初等対称多項式に他なりません。

$S = (S_k)_{k \geq 1}$ を不定数の数列とします。 Since the formal power series $s_k$ is of order $\geq k$, and belongs to $A[[X]]^{\text{sym}}$, conditions a) and b) of Prop. 4 of IV, p. 28 are satisfied with $E = A[[X]]^{\text{sym}}$; there exists thus a unique continuous A-algebra homomorphism

$$
\varphi_I : A[[S]] \to A[[X]]^{\text{sym}}
$$

整数 $k \geq 1$ ごとに $\varphi_I(S_k) = s_k$ となるようにします。

#### 定理 2 {#alg-iv-s6-thm-2 .statement tag=06EL}

**a)** *I が n 元の有限集合である場合、$\varphi_I$ 誘導するは $A[[X]]^{\text{sym}}$* 上の $A[[S_1, \ldots, S_n]]$ の共連続同型です。

*b)* *I が無限大の場合、$\varphi_I$ は $A[[S]]$ から $A[[X]]^{\text{sym}}$* への共連続同型です。

a) の場合、$B = A[[S_1, \ldots, S_n]]$ を配置し、この代数に $A[[S]]$ の位相を装備します。また、B に対して $\varphi_I$ の $\psi_I$ 制限で表します。b) の場合、$B = A[[S]]$ と $\psi_I = \varphi_I$ を置きます。多項式代数 $A[S]$ に型 N の目盛りを与え、$S_k$ は整数 $k \geq 1$ ごとに重み k になります。

#### 補題 1 {#alg-iv-s6-lem-1 .statement tag=06EM}

** J を I の有限部分集合、r 整数とし、カード $J \geq r$ と、$X_i$ ($i \in I$) の次数 r と同次である対称形式冪系列を求めます。 $\bar{f}$ を、$I - J$ の各 i の $X_i$ に 0 を代入して得られる形式的な冪系列とします。 $\bar{f} = 0$ の場合、$f = 0$ になります。**

$f = \sum_{|\alpha| = r} a_\alpha X^\alpha$ を置きましょう ($|\alpha|$ はマルチインデックス $a = (\alpha_i)_{i \in I}$ の長さ $\sum_{i \in I} \alpha_i$ です)。 $a$ が長さ $r$ のマルチインデックスで、$J'$ が $a$ ($\alpha_i \neq 0$ となる $i \in I$ の集合) のサポートである場合、カード $J' \leq r$ であるため、置換が存在します。 $\sigma \in S_I$ は $\sigma(J') \subset J$ になります。 $i \in I$ に $\beta_i = \alpha_{\sigma^{-1}(i)}$ を代入すると、単項式 $X^\beta = \prod_{i \in I} X_{\sigma(i)}^{\alpha_i}$ は、仮定 $\overline{f} = 0$ による不定数 $X_j$ ($j \in J$)、よって $a_\beta = 0$ のみに依存します。 $f$ は対称なので $a_\alpha = a_\beta$ が得られ、$\alpha$ は任意なので $f = 0$ を結論するとします。

#### 補題 2 {#alg-iv-s6-lem-2 .statement tag=06EN}

*$f$を、$X_i (i \in I)$における次数$r$の対称形式冪系列とする。 重み $r$ の等圧である、$f = \psi_1(P)$ などの一意の多項式 $P \in B \cap A[S]$ が存在します。*

$I$ が有限である場合は、Th から次のようになります。 1 (IV、p. 62)。

$I$ が無限大で、$I$、含む $r$ 元の選ぶ有限部分集合 $J$ とします。 補題 1 の記法を維持します。 $S_n \ (n \geq 1)$ の重み $r$ のすべての等重多項式は $S_1, \ldots, S_r$ にのみ依存し、$\overline{s}_1, \ldots, \overline{s}_r$ は $r$ の不定数 $X_j \ (j \in J)$ の初等対称多項式であることに注意してください。 $S_n$ と $h = f - \psi_1(P)$ における $P$ が重み $r$ の等重多項式である場合、$\overline{h} = \overline{f} - P(\overline{s}_1, \ldots, S_r)$ と補題 1 は、関係 $f = \psi_1(P)$ が $\overline{f} = P(\overline{s}_1, \ldots, \overline{s}_r)$ と同等であることを示します。 Thさんより1 (IV, p. 62) 重み $r$ の等圧である一意の多項式 $P \in A[S]$ が存在し、結果は $\overline{f} = P(\overline{s}_1, \ldots, \overline{s}_r)$, よってになります。

#### 補題 3 {#alg-iv-s6-lem-3 .statement tag=06EO}

*すべての整数 $m \geq 0$ について、$c_m$ を、位数 $\geq m$ のすべての対称形式冪系列の代数 $A[[X]]^{sym}$ からなるの理想とします。 数列 $(c_m)_{m \geq 0}$ は、$A[[X]]^{sym}$ の $0$ の近傍の基本的な系です。

補題は、$I$ が有限であるときに明らかに成り立つので、$I$ が無限であると仮定します。 $I$ の有限部分集合 $J$、$m$ 元のからなるについて、$\tilde{J}$ 集合元の $N^{(1)}$ 長さで表します。 $< m$ と $J$ のサポート付き。さらに、正式な冪系列含む項 $aX^\alpha$ を $a \in \tilde{J}$ で$a_J'$ 集合で表します。 $\tilde{J}$ は $N^{(1)}$ の有限部分集合であり、$N^{(1)}$ のすべての有限部分集合は形 $\tilde{J}$ の集合に含まれるため、ファミリー $(a_J')$ は、近傍の基底になります。 $0$ の $A[[X]]$ (IV、p. 26)。ここで、補題 1 は、$m$ 元を含むすべての部分集合 $J$ に対して関係 $a_J' \cap A[[X]]^{sym} = c_m$ を意味し、これにより補題 3 が証明されます。

$S_k$ には、指定された重みの単項式が有限の数しかないため、すべての正式な冪系列 $f \in B$ は、$f = \sum_{r \geq 0} P_r$ として独自の方法で書くことができます。ここで、$P_r$ は次の等重多項式です。 重み $r$ で $B \cap A[S]$。 整数 $m \geq 0$ ごとに、$0 \leq r < m$ に対して $P_r = 0$ となるように、上記型のすべての正式な冪系列の$B$ からなるの理想を$b_m$ とします。 数列 $(b_m)_{m \geq 0}$ は、$B$ の $0$ の近傍の基底です。

上記の記法 $\psi_1(P_r)$ は、次数 $r$ の同次である $X_i$ の対称形式冪系列であるため、これは次数の同次成分です。 $r$/$\psi_1(f)$。 補題 2 は、$\psi_1$ が整数 $m \geq 0$ ごとに $A[[X]]^{sym}$、写像 $b_m$ から $c_m$ への $B$ の代数準同型であることを示します。現在補題 3 は $\psi_1$ が共連続であることを示しており、これで定理 2 の証明が完成します。

### 4. 和/冪

不確定要素の家族については、再び $X = (X_i)_{i \in I}$ と書きます。対称形式冪系列 $s_k$ は、次のように前にとして定義されます。

$$
s_k = \sum_{H \in \mathfrak{P}_k} \prod_{i \in H} X_i \quad (k \geq 1),
$$

ここで、$\mathfrak{P}_k$ は、$I$ のすべての k 要素部分集合の集合です。私たちも書きます

$$
p_k = \sum_{i \in I} X_i^k \quad (k \geq 1)
$$

これは、次数 k と同次である対称形式冪系列です。

#### 補題 4 (« ニュートンの関係 ») {#alg-iv-s6-lem-4 .statement tag=06EP}

— *整数 $d \geq 1$ ごとに*

$$
p_d = \sum_{k=1}^{d-1} (-1)^{k-1} s_k p_{d-k} + (-1)^{d+1} d s_d
$$

$\mathbf{A}[[\mathbf{X}]]$ の $A(u) = \sum_{n \geq 0} n u_n$ による連続導分 $A$ を定義するとします。ここで、$\mathbf{A}[[\mathbf{X}]]$ のすべての $u$ に対して、$u_n$ は次数 $n$ の同次成分です。 $u$。 (16) と *IV*、p. 27 の提案 2 により、次のようになります。

$$
1 + \sum_{k \geq 1} s_k = \prod_{i \in I} (1 + X_i)
$$

*IV*, p. 34 の提案 9 により、次のようになります。

$$
\left( \sum_{k \geq 1} k s_k \right) \cdot \left( 1 + \sum_{k \geq 1} s_k \right)^{-1} = \sum_{i \in I} \Delta(X_i)/(1 + X_i).
$$

$A(X_i) = X_i$と$X_i/(1 + X_i) = \sum_{k \geq 1} (-1)^k \ X_i^k$がございます。したがって、(20) の右辺は $\sum_{k \geq 1} (-1)^{k-1} p_k$ に等しくなります。したがって、(20) により、次のようになります。

$$
\sum_{k \geq 1} k s_k = \left( 1 + \sum_{k \geq 1} s_k \right) \cdot \left( \sum_{k \geq 1} (-1)^{k-1} p_k \right)
$$

そして今度は補題 4 の後に、同種の成分の次数 d の比較が続きます。

#### 注意 {#alg-iv-s6-n4-rem-1 .statement tag=06EQ}

— 上記証明の記法により、次のようになります。

$$
\Delta u = \sum_{i \in I} X_i \cdot D_i(u)
$$

(IV、p. 33、コリント 1)。他の語では、*オイラーの関係 (IV, p. 8, Prop 6)* 拡大するを形式的な冪系列 : $u \in A[X]$ が次数と同次である場合$n$、それでは

(21)
$$
n \cdot u = \sum_{i \in I} X_i \cdot D_i(u) .
$$

I が有限である場合、$n$ 元のからなるでは、$k > n$ に対して $s_k = 0$ が得られます。そうすれば、ニュートンの関係が書けるかもしれません

$$
\begin{aligned}
p_2 &= s_1 p_1 - 2 s_2 \\
p_3 &= s_1 p_2 - s_2 p_1 + 3 s_3 \\
&\ \ \cdots \cdots \cdots \cdots \cdots \cdots \cdots \\
p_{n-1} &= s_1 p_{n-2} - s_2 p_{n-3} + \cdots + (-1)^{n-1} s_{n-2} p_1 + (-1)^n (n-1) s_{n-1} \\
p_n &= s_1 p_{n-1} - s_2 p_{n-2} + \cdots + (-1)^n s_{n-1} p_1 + (-1)^{n+1} n s_n
\end{aligned}
$$

そして

(22)
$$
p_k = s_1 p_{k-1} - s_2 p_{k-2} + \cdots + (-1)^{n+1} s_n p_{k-n} \quad (\text{for } k > n) .
$$

上記関係の最初の $n$ は、どの $I$ にも当てはまります。たとえば

$$
p_1 = s_1 , \quad p_2 = s_1^2 - 2 s_2 , \quad p_3 = s_1^3 - 3 s_1 s_2 + 3 s_3 .
$$

より一般的には、$S = (S_n)_{n \geq 1}$ を不定値の族とします。 定義する多項式 $P_d \in \mathbf{Z}[S_1, \ldots, S_d]$ を $P_1 = S_1$ によって再帰的に計算してみます。

$$
P_d = \sum_{k=1}^{d-1} (-1)^{k-1} S_k P_{d-k} + (-1)^{d+1} d S_d \quad (d \geq 2) .
$$

次に、任意の環 A と不定数の族 X を保持する« *普遍公式* » $p_d = P_d(s_1, \ldots, s_d)$ ができます。
$P = (P_k)_{k \geq 1}$ を不定数の数列とします。 $p_k$ は $A[[X]]$ の次数 k と同次なので、連続する A-代数準同型が正確に 1 つ存在します。

$$
\lambda_I : A[[P]] \to A[[X]]^{\mathrm{sym}}
$$

整数 $k \geq 1$ *(IV, p. 28)* ごとに $\lambda_I(P_k) = p_k$ となるようにします。 $P_k$ 重み k に代入すると、$P_k$ の重み $n$ の等重多項式を $\lambda_I$ 変換に等次な形式的な冪系列に変換します。 $X_i$の次数 $n$。

#### 命題 3 {#alg-iv-s6-prop-3 .statement tag=06ER}

— *a) I が n 元の有限集合で、$n! \cdot 1$ が A で可逆である場合、$\lambda_I$ 誘導するは $A[[P_1, \ldots, P_n]]$ から $A[[X]]^{\mathrm{sym}}$ への共連続同型です。
*b) I が無限で A が Q 代数である場合、$\lambda_I$ は $A[[P]]$ から $A[[X]]^{\mathrm{sym}}$ への共連続同型です。
ケース *a)* のみを扱いますが、ケース *b)* も非常に似ています。

Thさんより2 (IV、p. 68) 同一視できる $\mathbf{A}[[\mathbf{X}]]^{\text{sym}}$ は正式な冪系列 $\mathbf{A}[[S_1, \ldots, S_n]]$ の代数と$S_k$ 対応するから $s_k$ です。 IV, p. 70 の補題 4 までに、不定数 $s_1, \ldots, s_n$ には、位数 $\geq 2$ の形式的な冪系列 $g_1, \ldots, g_s$ が存在します。

$$
p_k = (-1)^{k+1} k s_k + g_k(s_1, \ldots, s_s) \quad (1 \leq k \leq n).
$$

$k! . 1$は$\mathbf{A}$, IVの補題 2で可逆であるため、p. 35は写像を成す位相$\mathbf{A}$-代数$\mathbf{A}[[\mathbf{X}]]^{\text{sym}}$の自己同型$T$の存在を証明します。 $l \leq k \leq n$の場合は$s_k$から$p_k$まで。さて、提案 3、a) は明らか帰結です。

#### 系 {#alg-iv-s6-n4-cor-1 .statement tag=06ES}

— *$\xi_1, \ldots, \xi_n, \eta_1, \ldots, \eta_n$を$\mathbf{A}$の元とし、$\mathbf{A}$を整域と仮定します。*

a) *$1 \leq k \leq n$ に対して $s_k(\xi_1, \ldots, \xi_n) = s_k(\eta_1, \ldots, \eta_n)$ の場合、$1 \leq i \leq n$ に対して $\eta_i = \xi_{\sigma(i)}$ となるような置換 $\sigma \in \mathfrak{S}_n$ が存在します。

b) *$\mathbf{A}$ に $n! . 1 \neq 0$ があり、*

$$
\xi_1^k + \cdots + \xi_n^k = \eta_1^k + \cdots + \eta_n^k
$$

$1 \leq k \leq n$用。 *その後、$1 \leq i \leq n$ に対して $\eta_i = \xi_{\sigma(i)}$ となるような置換 $\sigma \in \mathfrak{S}_n$ が存在します。

仮説 a) の下では、$\prod_{i=1}^n (X - \xi_i) = \prod_{i=1}^n (X - \eta_i)$ となります。 $X$を$\eta_n$に置き換えると、$\prod_{i=1}^n (\eta_n - \xi_i) = 0$がわかり、$\mathbf{A}$は整域なので、$l \ s \ \sigma(n) \leq n$と$\eta_n = \xi_{\sigma(n)}$のような整数$\sigma(n)$が存在します。ここで、主張 a) は、$\mathbf{A}[X]$ が整域であるため、帰納法によって簡単に続きます。

b) の仮説の下では、$\mathbf{A}$ の分数の体に係数が$1 \leq k \leq n$ に対して $s_k = \Pi_k(p_1, \ldots, p_n)$ となるような、$n$ の不定数に$\Pi_1, \ldots, \Pi_n$ という命題 3 の多項式が存在します。さて、関係 (23) が意味するのは

$$
s_k(\xi_1, \ldots, \xi_n) = s_k(\eta_1, \ldots, \eta_n)
$$

$1 \leq k \leq n$ の場合、b) は a) から続きます。

### 5. 多項式の対称写像の根

係数が $\mathbf{A}$ である、次数 $n$ のモニック多項式を考えてみましょう。

$$
f = X^n + a_1 X^{n-1} + \cdots + a_{n-1} X + a_n.
$$

私たちは定義する生成元 $x_1, \ldots, x$ および関係と結合的、可換的で単位的な $\mathbf{A}$-代数 $E_f$ です。

$$
\sum_{i_1 < \ldots < i_k} x_{i_1} \ldots x_{i_k} = (-1)^k a_k \quad (1 \leq k \leq n).
$$

より正確に言えば、

$$
E_f = A[X_1, ..., X_n]/a
$$

ここで、イデアル $a$ は $1 \leq k \leq n$ の多項式 $s_k + (-1)^{k+1} a_k$ によって生成され、$x_i$ は $1 \leq i \in n$ の $X_i$ mod $a$ の剰余類です。 関係 (24) は $f(X) = \prod_{i=1}^n (X - x_i)$ と同等です。曖昧になる恐れがある場合は、$x_1, ..., x_n$の代わりに$x_{1,f}, ..., x_{n,f}$と表記します。

#### 命題 4 {#alg-iv-s6-prop-4 .statement tag=06ET}

*BをBにAの可換環、$\rho$、準同型、Bの$\xi_1, ..., 5$、元とする。B[X]に関係$^\rho f(X) = \prod_{i=1}^n (X - \xi_i)$が成り立つとする。その場合、すべての $a \in A$ に対して $\rho(a) = u(a . 1)$ が、$1 \leq i \leq n$ に対して $u(x_i) = \xi_i$ となるような環準同型 $u : E_f \to B$ が 1 つだけ存在します。

$\rho$ によって B を結合的、可換的、および単体的な A-代数とみなします。そうすると、関係 $^\rho f(X) = \prod_{i=1}^n (X - \xi_i)$ も形で書かれる可能性があります。

$$
\sum_{i_1 < ... < i_k} \xi_{i_1} ... \xi_{i_k} = (-1)^k a_k . 1 \quad (1 \leq k \leq n)
$$

B では、関係 (24) 定義する以降、$E_f$ の提示があり、提案 4 が続きます。

提案 4 は、$E_f$ の名前「universal 分解代数 of $f$」を正当化します。 関係 $f(X) = \prod_{i=1}^n (X - x_{i,f})$ は、« $f$ の普遍的な分解 » と呼ばれます。 $\sigma \in S_n$ を置換とします。 $f(X) = \prod_{i=1}^n (X - x_{\sigma(i),f})$ 以降、$1 \leq i \leq n$ に対して $t_\sigma(x_{i,f}) = x_{\sigma(i),f}$ を特徴とする A-代数 $E_f$ の自己同型 $t_\sigma$ が存在します。 $S_n$ の $\sigma, \tau$ に対して $t_{\sigma \tau} = t_\sigma \circ t_\tau$ があるため、群 $\mathscr{G}$ の作用、つまり A-代数 $E_f$ が得られます。

#### 命題 5 {#alg-iv-s6-prop-5 .statement tag=06EU}

*ユニバーサル分解代数 $E_f$ では、$1 \leq i \leq n$ に対する $0 \leq \nu(i) < i$ は A-加群 $E_f$ の基底となる単項式 $x_1^{\nu(1)} ... x_n^{\nu(n)}$ の族です。特に$E_f$は階数$n!$の自由A-加群です。

$B = A[X_1, ..., X_n]$ と $C = A[X_1, ..., X_n]^{\text{sym}}$ と書きます。 Thさんより1 (*IV*, p. 62) $C = A[s_1, ..., s_n]$ と $s_1, ..., s_n$ は A に関して代数的に独立しています。$s_1, ..., s_n$ 形の定数項を持たない多項式は、C の理想$C^+$ であり、A と$s_1, ..., s_n$ によって生成されました。 c を $s_1 + a_1, s_2 - a_2, ..., s_n + (-1)^{n+1} a_n$ によって生成される C のイデアルとします。 $1 \leq k \leq n$ に対して写像 $s_k$ から $s_k + (-1)^{k+1} a_k$ までの C の A-代数自己同型が存在するため、 c には写像 $C^+$ が存在します。したがって、$C = A \oplus c$ となります。さらにTh. 1、*IV*、p. 62 の c) は次のことを示しています。

$$
B = \bigoplus_{\nu \in S} CX^\nu
$$

ここで、S はすべての $\nu \in \mathbf{N}^n$ の集合であり、$1 \leq i \leq n$ に対して $0 \leq \nu(i) < i$ となります。 B のイデアル a は c、よって $a = Bc = \bigoplus_{\nu \in S} c \cdot X^\nu$ によって生成されます。 $C = A \oplus c$ 以降、次のことがわかります。
$$
B = a \oplus \bigoplus_{\nu \in S} AX^\nu,
$$
よって提案 5、$E_f = B/a$ のため。

#### 系 {#alg-iv-s6-n5-cor-1 .statement tag=06EV}

— *A の標準準同型をモニック多項式 $f \in A[X]$ の普遍的な分解代数に変換するのは単射です。*

単位元の$E_f$形部分の基底のA-加群$E_f$の場合。

#### 命題 6 {#alg-iv-s6-prop-6 .statement tag=06EW}

— *$f \in A[X]$ を次数 n のモニック多項式とし、P を A に係数をもつ $X_1, ..., X_n$ の対称多項式とする。すると、次の性質を持つ A の元 a が正確に 1 つ存在します。
(FS) B[X] の環準同型 $\rho : A \to B$ と分解 $^0f(X) = \prod_{i=1}^n (X - \xi_i)$ については、$\rho(a) = P(\xi_1, ..., \xi_n)$ があります。*

$f = X^n + \sum_{k=1}^n a_k X^{n-k}$と書いてからThまでにします。 1、IV、p. 62 には、$P = \Pi(s_1, ..., s_n)$ となるような、A の係数で不定となる n の多項式 $\Pi$ が存在します。 $a = \Pi(-a_1, a_2, ..., (-1)^n a_n)$を入れます。 仮定 (FS) では、
$$
s_k(\xi_1, ..., \xi_n) = (-1)^k \rho(a_k)
$$
よって
$$
\begin{align*}
\rho(a) &= \Pi(-\rho(a_1), \rho(a_2), ..., (-1)^n \rho(a_n)) \\
&= \Pi(s_1(\xi_1, ..., \xi_n), ..., s_n(\xi_1, ..., \xi_n)) \\
&= P(\xi_1, ..., \xi_n) .
\end{align*}
$$

これにより、元満たす (FS) の存在が証明されます。コルからの一意性がフォローします。提案 5 に、普遍的な分解代数 $E_f$ に $a \cdot 1 = P(x_{1,f}, ..., x_{n,f})$ があるからです。

提案 6 の記法により、ときどきは $a = P^*(f)$ と書き込みます。 例をいくつか紹介します。

#### 例 {#alg-iv-s6-n5-exa-1 .statement tag=0DHL}

※1)$P = s_k$の場合は$P^*(f) = (-1)^k a_k$となります。
\* 2) g を $A[X]$ の多項式とし、次のようにします。
$$
P(X_1, ..., X_n) = g(X_1) ... g(X_n) .
$$
したがって、$P^*(f)$ は、Cor による結果の $\operatorname{res}(f, g)$ です。 IV、p. 80 の 1 つ。
3) $A(X_1, ..., X_n) = \prod_{i < j} (X_i - X_j)^2$ とすると、$\Delta^*(f)$ はモニック多項式 $f$ (IV, p. 82, 公式 (46)) の判別式になります。 \*

4) $P(X_1, \ldots, X_n) = X_1^k + \ldots + X_n^k$ を入れます。さらに、定義する代数 $E = A[X]/(f)$、$E$の$X$の像に$x$と書きます。 $A$ モジュール $E$ は、基底 $(1, x, \ldots, x^{n-1})$ (IV、p. 11、Cor.) とともに無料であることを思い出してください。見せてみましょう

$$
\text{Tr}_{E/A}(x^k) = P^*(f)
$$

整数 $k \geq 1$ ごとに $\pi_k = \text{Tr}_{E/A}(x^k)$ を入れます。ニュートンの関係 (IV, p. 70) を念頭に置いて、関係を確立するだけで済みます。

$$
\begin{align*}
&\pi_k + a_1 \pi_{k-1} + \cdots + a_{k-1} \pi_1 + k a_k = 0 \quad \text{for } 1 \leq k \leq n \\
&\pi_k + a_1 \pi_{k-1} + \cdots + a_{n-1} \pi_{k-n+1} + a_n \pi_{k-n} = 0 \quad \text{for } k > n
\end{align*}
$$

(これを「ニュートンの関係」とも呼びます)。 関係 (27) は左側が の跡なのでクリアです。

$$
x^{k-n}(x^n + a_1 x^{n-1} + \cdots + a_{n-1} x + a_n) = 0 .
$$

$1 \leq k \leq n$ と仮定して、

$$
y = x^k + a_1 x^{k-1} + \cdots + a_{k-1} x + a_k \cdot 1 ;
$$

$M = (m_{ij})$ を基底 $(x')_{0,\ldots,n}$ に対する $E$ の線形写像 $u \mapsto yu$ の行列とします。 関係を簡単に入手できます

$$
\begin{align*}
&m_{ii} = a_k \quad \text{for } 0 \leq i < n - k \\
&m_{ii} = 0 \quad \text{for } n - k \leq i < n ,
\end{align*}
$$

よって

$$
\text{Tr}_{E/A}(y) = \sum_{i=0}^{n-1} m_{ii} = (n-k) a_k .
$$

さらに、私たちは

$$
\text{Tr}_{E/A}(y) = \pi_k + a_1 \pi_{k-1} + \cdots + a_{k-1} \pi_1 + n a_k ,
$$

よって公式 (26) が続きます。

### 6. 結果として得られる

この番号では、2 つの正の整数 $p, q$ と形の $A[X]$ の 2 つの多項式 $f, g$ が与えられたと仮定します。

$$
\begin{align*}
f &= t_p X^p + t_{p-1} X^{p-1} + \cdots + t_0 \\
g &= u_q X^q + u_{q-1} X^{q-1} + \cdots + u_0
\end{align*}
$$

$\deg f \leq p, \deg g \leq q$ のようになります。すべての整数 $n \geq 0$ について、次数 $< n$ のすべての多項式の$A[X]$ からなるのサブ$A$ 加群を $S$ で表します。 基底としてファミリー $(X')_{0 \leq i < n}$ があり、したがって階数 $n$ になります。

$S, \times S_p$ と基底を提供します
$$
B_1 = ((X^{q-1}, 0), ..., (X, 0), (1, 0), (0, X^{p-1}), ..., (0, X), (0, 1))
$$
そして$S_{p+q}$と基底
$$
B_2 = (X^{p+2-1}, ..., X, 1).
$$
私たちは定義する線形写像 $\varphi : S, \times S_p \to S_{p+q}$ によって
$$
\varphi(u, v) = uf + vg
$$
そして、基底 $B_1$ と $B_2$ に関して $\varphi$ の $M(f, g, p, q)$ 行列で表します。これは、位数 $p + q$ の平方行列で、集合 $\{0, 1, ..., p + q - 1\}$ でインデックスされています。その元 $a_{ij}$ は次のルールによって与えられます。
a) $0 \leq j \leq q-1$ の場合は $a_{ij} = t_{p-i+j}$、
b) $q \leq j \leq p + q - 1$ の場合は $a_{ij} = u_{j-i}$、
ここで、$k \notin (0, p)$ の場合、$t_k$ は 0 とみなされ、$k \notin (0, q)$ の場合、$u_k = 0$ は 0 とみなされます。

たとえば、$p = 2$ と $q = 3$ の場合、行列になります。
$$
\begin{pmatrix}
t_2 & 0 & 0 & u_3 & 0 \\
t_1 & t_2 & 0 & u_2 & u_3 \\
t_0 & t_1 & t_2 & u_1 & u_2 \\
0 & t_0 & t_1 & u_0 & u_1 \\
0 & 0 & t_0 & 0 & u_0
\end{pmatrix}.
$$

#### 定義 1 {#alg-iv-s6-def-1 .statement tag=06EX}

*上記の行列 $M(f, g, p, q)$ の記法行列式は、 次数 $p$ と $q$ の対 $(f, g)$ の結果、または単に $f$ と $g$ の結果と呼ばれます。 $p = \deg f$ と $q = \deg g$。*

$p = \deg f$、$q = \deg g$の場合、結果は$\operatorname{res}_{p,q}(f, g)$、または単に$\operatorname{res}(f, g)$で表されます。

#### 例 1 {#alg-iv-s6-n6-exa-1 .statement tag=06EY}

$\Lambda$ に $\Lambda, \mu$ が与えられると、次の式が得られます。
$$
\operatorname{res}_{p,0}(f, \lambda) = \lambda^p, \quad \operatorname{res}_{0,q}(\mu, g) = \mu^q
$$
$$
\operatorname{res}_{p,1}(f, \lambda) = \lambda^p t_p, \quad \operatorname{res}_{1,q}(\mu, g) = (-1)^q \mu^q u_q,
$$
その証明は明らかです。

#### 例 2 {#alg-iv-s6-n6-exa-2 .statement tag=06EZ}

$p = q = 1$ のとき、
$$
\operatorname{res}_{1,1}(t_1 X + t_0, u_1 X + u_0) = t_1 u_0 - t_0 u_1
$$

#### 注意 1 {#alg-iv-s6-n6-rem-1 .statement tag=06F0}

行列 $M(g, f, q, p)$ は、$M(f, g, p, q)$ から列、よっての $pq$ の転置によって得られます。
$$
\operatorname{res}_{q,p}(g, f) = (-1)^{pq} \operatorname{res}_{p,q}(f, g)
$$

#### 注意 2 {#alg-iv-s6-n6-rem-2 .statement tag=06F1}

$\rho : A \to B$ を環準同型とします。デフ。 / 公式を直接暗示します
$$
\operatorname{res}_{p,q}(\rho f, \rho g) = \rho(\operatorname{res}_{p,q}(f, g)) .
$$

#### 注意 3 {#alg-iv-s6-n6-rem-3 .statement tag=06F2}

$A$ に $\lambda, \mu$ が与えられると、次のようになります。
$$
\operatorname{res}_{p,q}(\lambda f, \mu g) = \lambda^q \mu^p \operatorname{res}_{p,q}(f, g) .
$$
(28)

#### 注意 4 {#alg-iv-s6-n6-rem-4 .statement tag=06F3}

$p + q \geq 1$ と仮定します。 $\varphi$ 含むの III、p. 532、公式 (28)、像により、定数多項式 $\operatorname{res}_{p,q}(f, g)$ が得られます。したがって、次のような $u \in S_q, v \in S_p$ を含む多項式 $(u, v)$ の対が存在します。
$$
\operatorname{res}_{p,q}(f, g) = uf + vg ,
$$
よって
$$
\operatorname{res}_{p,q}(f, g) \in A \cap (f, g) .
$$
この対 $(u, v)$ は、$\operatorname{res}_{p,q}(f, g)$ が $A$ でキャンセル可能である場合に一意です。その場合、$\varphi$ は単射法です (III、p. 524、提案 3)。

#### 注意 5 {#alg-iv-s6-n6-rem-5 .statement tag=06F4}

$p \geq q$ を仮定し、$h \in A[X]$ を次数 $\leq p - q$ の多項式とします。それを見せてみましょう
$$
\operatorname{res}_{p,q}(f, g) = \operatorname{res}_{p,q}(f + gh, g) .
$$
(29)
というのは、$(u, v) \in S_q \times S_p$ に対して $\omega(u, v) = (u, uh + v)$ を書くと、$w$ は $A$ モジュール $S_q \times S_p$ の自己同型となり、次のようになります。
$$
\omega^{-1}(u, v) = (u, -uh + v) .
$$
基底 $B_1$ に対する $w$ の行列は下三角であり、その対角線元は $1$ に等しい。一方、$\varphi \circ w$ 写像 $(u, v)$ ～ $u(f + gh) + vg$。ここで、公式 (29) は、$\varphi$ と $\varphi \circ w$ を表す行列が同じ行列式を持ち、これが関係 $\det w = 1$ から続くことを意味します。

$f$ が次数 $p$ のモニックであると仮定します。 $E = A[X]/(f)$を入れて、$E$の$X$の$x$標準像で表します。私たちは (IV、p. 11) $E$ が基底 $(1, x, \ldots, x^{p-1})$ を備えた無料の $A$ モジュールであることを知っています。したがって、$E$ の任意の元 $u$ の定義するノルム $N_{E/A}(u)$ (III、p. 543、定義 2)。

#### 命題 7 {#alg-iv-s6-prop-7 .statement tag=06F5}

— *f が次数 p のモニックであると仮定します。上記記法により、*¹ が得られます
$$
\operatorname{res}_{p,q}(f, g) = N_{E/A}(g(x)) .
$$
(30)

¹ したがって、$f$ が次数 $p$ のモニックである場合、結果の $\operatorname{res}_{p,q}(f, g)$ は $q$ から独立しています。それを単に $\operatorname{res}(f, g)$ で表します。

$S_q \times S_p$ の定義する A-線型写像 $0$ を $\theta(u, v) = uf + v$ で $S_{p+q}$ にしましょう。次に、$S_q \times S_s$ の $0$ 写像基底 $B_1$ を数列にします
$$
(fX^{q-1}, \ldots, fX, f, X^{p-1}, \ldots, X, 1)
$$
元の$S_{p+q}$。したがって、基底 $B_1, B_2$ に対する $0$ の行列 $M$ は下三角であり、その対角線元は 1、よって $\det M = 1$ に等しい。

したがって、$\theta$ は全単射であり、$\operatorname{res}_{p,q}(f, g)$ は自己準同型の行列式 、$S_{p-q}$ の $\varphi' = \varphi \circ \theta^{-1}$ に等しいということになります。明示的に、
$$
\varphi'(uf + v) = uf + vg
$$
$S_q \times S_s$ のいずれかの対 $(u, v)$ の場合。今、$A[X] = S_{p+q} + (f)$と$fS_q = S_s \cap (f)$があるので、$S_{p-s}$の標準単射は$A[X]$定義するに商同型$\gamma$の$S_{p+q}/fS_q$がEに進みます。$\psi$をE の $g(x)$ による乗法 。 公式 (31) は、$fS_q$ では $\varphi'$ 誘導するが、$S_{p+q}/fS_q$ では $\gamma^{-1}\psi\gamma$ が同一であることを示しています。したがって、$\det \varphi' = \operatorname{res}_{p,q}(f, g)$ と $\det \psi = N_{E/A}(g(x))$ は定義までなので、$\det \varphi' = \det \psi$、よって (30) が続きます。

#### 系 1 {#alg-iv-s6-prop-7-cor-1 .statement tag=06F6}

— $f \in A[X]$ をモニック多項式とします。すべての多項式 $g \in A[X]$ に対して、次の条件は等価です。
(i) $\operatorname{res}(f, g)$ は $A$ で反転可能です。
(ii) $A[X]$ には $uf + vg = 1$ となるような多項式 $u, v$ が存在します。
(iii) $g(x)$ は代数 $A[X]/(f)$ で反転可能です。
(i) および (iii) の同値は、III、p. 545 および提案 7 の提案 3 に続きます。 (ii) と (iii) の結果は自明に続きます。

#### 系 2 {#alg-iv-s6-prop-7-cor-2 .statement tag=06F7}

— $A$ が体であると仮定し、$f, g \in A[X]$ とすると、$f, g$ がゼロ以外の場合、次の条件は等価になります。
(i) $\operatorname{res}(f, g) \neq 0$;
(ii) 多項式 $f$ と $g$ は $A[X]$ において互いに素である。
\* (iii) A の任意の拡大 L について、多項式 $f$ と $g$ には L に共通の根がありません。 \*

$f$ がモニックである場合 (IV, p. 77, 注意 3) に対して、一度に簡約するを実行できます。
(i)と(ii)の同値はCor.の単なる翻訳です。 1、定義による。 IV、p. 12 の 1 つ。 (ii)と(iii)の同値はまさにCorです。 IV、p. 13の7。

#### 系 3 {#alg-iv-s6-prop-7-cor-3 .statement tag=06F8}

— $\lambda \in A$ ごとに、
$$
\operatorname{res}_{p,1}(f, \lambda - X) = f(\lambda), \quad \operatorname{res}_{1,q}(X - \lambda, g) = g(\lambda).
$$
$f(X) = X - \lambda$、代数 E が A に等しい場合、$x = A$ になります。 2 番目の公式 (32) は提案 7 (IV, p. 77) から続きます。 注意 1 と 3 (IV、p. 76、77) までに、私たちは結論する
$$
\operatorname{res}_{p,1}(f, \lambda - X) = (-1)^p \operatorname{res}_{1,p}(\lambda - X, f) = (-1)^{p+p} \operatorname{res}_{1,p}(X - A, f) = f(A).
$$

ここで、f と g がモニックであると仮定します。 F A-代数 $A[X, Y]/(f(X), g(Y))$ で表し、F の X (それぞれ Y) の x (それぞれ y) 標準像で表します。

#### 命題 8 {#alg-iv-s6-prop-8 .statement tag=06F9}

— f と g がそれぞれ次数 p と q のモニックであると仮定します。上記の記法、A-加群 F は基底 $(x^i y^j)_{0 \leq i < p,\ 0 \leq j < q}$ で自由になり、

$$
\text{res}(f, g) = N_{F/A}(x - y).
$$

$E = A[X]/(f)$と$E' = A[Y]/(g)$を入れます。 II、p. 253、Cor. 標準準同型 $A[X] \otimes A[Y] \to A[X, Y]$ から派生した F への 1、$E @ E'$ の準同型 $\sigma$ は全単射です。これは、F の基底について主張を証明します。今、同一視する E となり、$\sigma$ の下の F にその像が入ります。すると、写像 Y から y への $E[Y]/(g(Y))$ の F への E 代数準同型性は同型になります。

ノルムの推移性 (III、p. 546) までに、

$$
N_{F/A}(x - y) = N_{E/A}(N_{F/E}(x - y)).
$$

提案 7 (IV, p. 77) により、$N_{F/E}(x - y)$ は E[Y] の多項式 g(Y) と x − Y の結果であり、したがって g(x) に等しくなります (IV, p. 78, Cor. 3)。 公式 (34) と提案 7 (IV, p. 77) により、次のようになります。

$$
N_{F/A}(x - y) = N_{E/A}(g(x)) = \text{res}(f, g)
$$

#### 命題 9 {#alg-iv-s6-prop-9 .statement tag=06FA}

— $p_1$ と $q_1$ を $\deg f_1 \leq p_1, \deg g_1 \leq q_1$ となるような $A[X]$ の正の整数と $f_1, g_1$ の多項式とする。それなら私たちは持っています

$$
\text{res}_{p, q + q_1}(f, gg_1) = \text{res}_{p, q}(f, g) \cdot \text{res}_{p, q_1}(f, g_1)
$$
$$
\text{res}_{p + p_1, q}(ff_1, g) = \text{res}_{p, q}(f, g) \cdot \text{res}_{p_1, q}(f_1, g).
$$

$\text{res}_{p, q}(f, g) = (-1)^{pq} \text{res}_{q, p}(g, f)$ (IV、p. 76) があります。したがって、(35) を証明すれば十分です。同様に、注意 3 (上記参照) は、公式 (35) が多項式 $f$ に対して確立される場合、形 Af ($A \in A$) のすべての多項式にそれが成り立つことを示しています。最後に、f が次数 p のモニックであるとき、公式 (35) は、命題 7 (IV, p. 77) から公式 $N_{E/A}(ab) = N_{E/A}(a) \cdot N_{E/A}(b)$ によって求められます。すべてにおいて、f の $X^p$ の係数 $t_p$ が可逆である場合、 (35) が成り立つ結論するです。

#### 補題 5 {#alg-iv-s6-lem-5 .statement tag=06FB}

t を A の元とします。 C で反転可能な B の部分環、部分環 B の C 含む、元 $\tau$ として、可換環 C 含む A が存在します。 環準同型 $p : B \to A$ では、A に対する p の $p(\tau) = t$ と制限が Id に等しくなります。

群の C 代数 $A^{(\mathbf{Z})}$ については、モノイド $\mathbf{N}$ の B 代数 $A^{(\mathbf{N})}$、つまり 1 つの不定数 $\tau$ の多項式代数 $A[\tau]$ をとれば十分です。 $\mathbf{Z}$ および p 準同型 $P \mapsto P(t)$ の $A(\tau)$ を A に入力します。

t = t_p とした補題 5 の記法について、次のようにします。
$$
F = \tau X^p + t_{p-1} X^{p-1} + \cdots + t_1 X + t_0
$$
B[X]で。 F の $X^p$ の係数は C で反転可能です。 F、g、$g_1$ を C[X] の多項式として考えると、次のようになります。
$$
\operatorname{res}_{p,q+q_1}(F, gg_1) = \operatorname{res}_{p,q}(F, g) \cdot \operatorname{res}_{p,q_1}(F, g_1)
$$
言われたことによって。 F、g、$g_1$ を B[X] の多項式として考えると、結果は変わりません。 $^\rho F = f$、$^\rho g = g$、$^\rho g_1 = g_1$、公式 (35) は (38) と注意 2 (IV、p. 77) から続きます。

#### 系 1 {#alg-iv-s6-lem-5-cor-1 .statement tag=06FC}

— (i) $\lambda, \alpha_1, \ldots, \alpha_p$ を A の元とし、$f(X) = \lambda (X - \alpha_1) \ldots (X - \alpha_p)$ と仮定します。私たちは持っています
$$
\operatorname{res}_{p,q}(f, g) = \lambda^q g(\alpha_1) \ldots g(\alpha_p) .
$$
(ii) $\mu, \beta_1, \ldots, \beta_q$ を A の元とし、さらに $g(X) = \mu (X - \beta_1) \ldots (X - \beta_q)$ と仮定します。それでは、
$$
\operatorname{res}_{p,q}(f, g) = \lambda^q \mu^p \prod_{\substack{1 \leq i \leq p \\ 1 \leq j \leq q}} (\alpha_i - \beta_j) .
$$
主張 (i) は式 (28)、(32)、(36) から直接導かれます。さて、主張 (ii) は (i) から続きます。

#### 系 2 {#alg-iv-s6-lem-5-cor-2 .statement tag=06FD}

— 整数 $r \geq 0$ ごとに、
$$
\operatorname{res}_{p,q+r}(f, g) = t_p^r \cdot \operatorname{res}_{p,q}(f, g) .
$$
例 1 (IV, p. 76) を念頭に置くと、(35) で $q_1 = r, g_1 = 1$ を取るだけで済みます。

f がモニックであると仮定し、$\rho : A \to B$ を B の環準同型および $\xi_1, \ldots, \xi_p$ 元として、分解が得られるようにします。
$$
^\rho f(X) = (X - \xi_1) \ldots (X - \xi_p)
$$
注意 2 (IV、p. 77) および Cor 著。上記の 1 は、
$$
\rho(\operatorname{res}(f, g)) = g(\xi_1) \ldots g(\xi_p)
$$
この注意は、特に普遍的な分解オフ (IV、p. 73) に当てはまります。また、$\rho$ は単射なので、$\operatorname{res}(f, g)$ を計算する手段となります。

#### 例 3 {#alg-iv-s6-n6-exa-3 .statement tag=06FE}

公式を証明しましょう
$$
\operatorname{res}_{2,2}(aX^2 + bX + c, a'X^2 + b'X + c') =
(ac' - ca')^2 + (bc' - cb')(ba' - ab')
$$

提案 9 (IV, p. 79) について議論すると、$a$ が可逆である場合、公式を証明するだけで十分であることがわかります。そのとき、形の分解が存在します。

$$
aX^2 + bX + c = a(X - x)(X - y)
$$

$B[X]$ では、$B$ は部分環として適切な環含む $A$ です。コル著上記の 1 の場合、必要な結果は次と等しいです。

$$
R = a^2(a'x^2 + b'x + c')(a'y^2 + b'y + c') .
$$

今では、

$$
ax + ay = -b , \quad axy = c
$$

by (43)、よって $(ax)^2 + (ay)^2 = b^2 - 2ac$。

(44) までに、

$$
R = {a'}^2(axy)^2 + a{b'}^2(axy) + a^2{c'}^2 + a'b'(axy)(ax + ay) +
$$
$$
+ a'c'((ax)^2 + (ay)^2) + ab'c'(ax + ay)
$$
$$
= {a'}^2c^2 + a{b'}^2c + a^2{c'}^2 - a'b'cb + a'c'(b^2 - 2ac) - ab'c'b
$$
$$
= (ac' - ca')^2 + (ab' - a'b)(b'c - c'b) ,
$$

そこから望ましい結果が得られます。

### 7. 判別式

#### 定義 2 {#alg-iv-s6-def-2 .statement tag=06FF}

*$f$ を次数 $m$ の $A[X]$ のモニック多項式とし、$E$ で $A$-代数 $A[X]/(f)$ と $X$ の $x$ 標準像で表します。 $E$。私たちは $f$ の判別式定義するを、$A$-代数 $E$ の基底 $(1, x, \ldots, x^{m-1})$ の判別式 $D_{E/A}(1, x, \ldots, x^{m-1})$ として、$\operatorname{dis}(f)$ と書きます。

正の整数 $k$ ごとに $\rho_k = \operatorname{Tr}_{E/A}(x^k)$ と書きます。 III、p. 549、定義により。 2 は公式になります

$$
\operatorname{dis}(f) = \det(p_{i+j})_{0 \leq i,j < m}
$$

*例。 — 1) $f$ が次数 0 または 1 のモニック多項式である場合、(45) により $\operatorname{dis}(f) = 1$ が得られます。
2) $f(X) = X^2 + \alpha X + \beta$ を次数のモニック多項式とします。 2. ニュートンの関係は形 (IV, p. 75) で書くことができます。

$$
p_0 = 2 \\
p_1 + \alpha = 0 \\
p_2 + \alpha p_1 + 2\beta = 0 ,
$$

よって $p_1 = -a$、$p_2 = a^2 - 2p$。したがって、

$$
\operatorname{dis}(f) = \det \begin{pmatrix} 2 & -\alpha \\ -a & \alpha^2 - 2p \end{pmatrix} = \alpha^2 - 4\beta
$$

B を A から B までの可換環、$\rho$ 準同型、および B の $\xi_1, \ldots, \xi_m$ 元とします。
$$
\rho f(X) = (X - \xi_1) \cdots (X - \xi_m).
$$
行列 $(\rho(p_{i + j}))_{0 \leq i, j < m}$ を M と書き、ファンデルモンド行列 $(\xi_i^{j+1})_{0 \leq i, j < m}$ を D と書きましょう。 IV, p. 75 の例 4 までに、
$$
\rho(p_k) = \xi_1^k + \cdots + \xi_m^k,
$$
よって $M = 'D . D ;$ by III, p. 532 には $D = \prod_{i > j} (\xi_i - \xi_j)$ と $\det M = (\det D)^2$ があります、つまり
$$
\rho(\operatorname{dis}(f)) = \prod_{i < j} (\xi_i - \xi_j)^2
$$
さらに (導分 $\frac{d}{dX}$ に D を書くと)
$$
D(\rho f)(\xi_i) = (\xi_i - \xi_1) \cdots (\xi_i - \xi_{i-1})(\xi_i - \xi_{i+1}) \cdots (\xi_i - \xi_m)
$$
$1 \leq i \leq m$、よって用
$$
\rho(\operatorname{dis}(f)) = (-1)^{m(m-1)/2} \prod_{i \neq j} (\xi_i - \xi_j) = (-1)^{m(m-1)/2} \prod_{i=1}^m D(\rho f)(\xi_i).
$$
コル著IV、p. 80 の 1 を$f$ のユニバーサル分解に適用すると、最終的に次のようになります。
$$
\operatorname{res}(f, Df) = \operatorname{res}(Df, f) = (-1)^{m(m-1)/2} \operatorname{dis}(f).
$$

#### 命題 10 {#alg-iv-s6-prop-10 .statement tag=06FG}

$m \geq 1$ にしましょう。次の性質を持つ一意の多項式 $A \in \mathbf{Z}[A_1, \ldots, A_m]$ が存在します。 $A[X]$ の任意の可換環 A および *モニック* 多項式 $f = X^m + \sum_{i=1}^m a_i X^{m-i}$ に対して、次のようになります。
$$
\operatorname{dis}(f) = \Delta(a_1, \ldots, a_m).
$$
さらに、A は次数 $\leq 2m-2$ であり、重み i を $A_i$ に代入すると、A は重み $m(m-1)$ の等圧になります。
a) A の一意性: A が (48) を満たす場合、特に $A = \operatorname{dis}(F)$ が得られます。ここで、F は $\mathbf{Z}[A_1, \ldots, A_m]$ に係数をもつ多項式 $X^m + \sum_{i=1}^m A_i X^{m-i}$ です。
b) *A の存在: $s_1, \ldots, s_m$ を不定数 $X_1, \ldots, X_m$ の初等対称多項式とする。 重み $m(m-1)$ の等重多項式 $A \in \mathbf{Z}[A_1, \ldots, A_m]$ が存在します。次のとおりです。
$$
\Delta(-s_1, s_2, \ldots, (-1)^m s_m) = \prod_{i < j} (X_i - X_j)^2;
$$

右辺は対称多項式 P であり、$Z[X_1, ..., X_m]$ (IV, p. 62, Th. 1) で次数 m(m − 1) の同次です。ここで、公式 (46) は、IV、p. 74 の記法において dis(f) = P (f ) を意味し、(48) はこれから直接続きます。

c) A の次数 : 関係 (47) と結果 (IV, p. 76) の定義は公式を意味します

$$
(-1)^{m(m-1)/2} \Delta = \det(a_{ij})_{0 \leq i,j \leq 2m-2}
$$

$a_{ij}$ の次の値

$$
\begin{align*}
a_{00} &= 1 , \quad a_{0,m-1} = m , \\
a_{ij} &= A_{i-j} & \text{for } 1 \leq i \leq 2m-2 , \quad 0 \leq j \leq m-2 \\
a_{ij} &= (j-i+1) A_{m+i-j-1} & \text{for } 1 \leq i \leq 2m-2 , \quad m-1 \leq j \leq 2m-2 .
\end{align*}
$$

$a_{0j} = 0$ $j \neq 0 , \ j \neq m-1$ の場合

これらの式では、$i < 0$ または $i > m$ に対して $A_i = 1$ と $A_i = 0$ が理解されます。ここで (50) は、証明しなければならなかったように、A が次数 $\leq 2m-2$ であることをすぐに示します。

提案 10 により、判別式を非モニック多項式に拡大する定義することができます。 $m \geq 1$ を整数とすると、$Z[A_0, A_1, ..., A_m]$ には、次数 $2m-2$、$\tilde{\Delta}$ という一意の同次多項式が存在します。

$$
\Delta(A_1, ..., A_r) = \tilde{\Delta}(1, A_1, ..., A_r)
$$

なぜなら、A は次数 $\leq 2m-2$ であるため、有理分数は

$$
A_0^{2m-2} \Delta(A_1/A_0, ..., A_m/A_0)
$$

$Q(A_0, A_1, ..., A_m)$ の属するから部分環 $Z[A_0, A_1, ..., A_m]$。 $A_i$ が $0 \leq i \leq m$ に対して重み i を持つ場合、$\tilde{\Delta}$ は重み $m(m-1)$ と等重です。 ff が次数 $\leq m$ の多項式であるとします。

$$
f = a_0 X^m + a_1 X^{m-1} + \cdots + a_{m-1} X + a_m ,
$$

置きましょう

$$
\operatorname{dis}_m(f) = \tilde{\Delta}(a_0, a_1, ..., a_r).
$$

$m = \deg f$ の場合、$\operatorname{dis}_m(f)$ に対して単純に dis(f) と書きます。 f がモニックの場合、dis(f) は定義で定義された判別式と一致します。 2、(48)、(51)、(52) による。

#### 命題 11 {#alg-iv-s6-prop-11 .statement tag=06FH}

— $A[X]$ の f を次数 $\leq m$ のものとします。

(i) *$\rho : A \to B$ が環準同型の場合、$\operatorname{dis}_m(\rho_f) = \rho(\operatorname{dis}_m(f))$ があります。

(ii) $\lambda, \alpha_1, ..., a_r$ を A の元とします。*もし* $f = X(X-\alpha_1) ... (X-a_r)$;それなら私たちは持っています

$$
\operatorname{dis}_m(f) = \lambda^{2m-2} \prod_{i < j} (\alpha_i - \alpha_j)^2 .
$$

(iii) $a_0$ を $f$ の $X^m$ の係数とします。それなら私たちは持っています

$$
\text{res}_{m,m-1}(f, Df) = \text{res}_{m-1,m}(Df, f) = (-1)^{m(m-1)/2} a_0 \text{ dis}_m(f) .
$$

主張 (i) はクリアです。

$\tilde{\Delta}$ は次数 $2m - 2$ と同次なので、次のようになります。

$$
\text{dis}_m(\lambda f) = \lambda^{2m-2} \text{dis}_m(f)
$$

次数 $\leq m$ のすべての多項式 $f \in A[X]$ に対して。 主張 (ii) は式 (46) と (55) から得られます。

$f$ が次数 $m$ のモニックであるとき、$a_0 = 1$ が得られ、主張 (iii) は公式 (47) に短縮されます。 (55) と関係を念頭に置いて

$$
\text{res}_{m,n}(\lambda f, \mu g) = \lambda^n \mu^m \text{res}_{m,n}(f, g),
$$

(IV, p. 77)、そこから、$a_0$ が $A$ で可逆である場合に進むことができます。さて、一般的なケースは、提案 11、(i) および補題 5 (IV、p. 79) によって続きます。

#### 系 1 {#alg-iv-s6-prop-11-cor-1 .statement tag=06FI}

— Let $g \in A[X]$ and let $n$ be 正の整数 such that $\deg g \leq n$.私たちは持っています

$$
\text{dis}_{m+n}(fg) = \text{dis}_m(f) \cdot \text{dis}_n(g) \cdot \text{res}_{m,n}(f,g)^2 .
$$

推論を前にとすることで、$f$ と $g$ がそれぞれ次数 $m$ と $n$ のモニックである場合に帰着します。 Now put $B = E_f \otimes E_g$, where $E_f$ (resp. $E_g$) is the universal 分解代数 of $f$ (resp. $g$) (IV, p. 73).すると、$A$ は $B$ の部分環となり、$B[X]$ では分解になります。

$$
f = \prod_{i=1}^m (X - \alpha_i), \quad g = \prod_{j=1}^n (X - \beta_j) .
$$

したがって、

$$
fg = \prod_{k=1}^{m+n} (X - \gamma_k) ,
$$

with $\gamma_i = \alpha_i$ for $1 \leq i \leq m$ and $\gamma_{m+j} = \beta_j$ for $1 \leq j \leq n$.私たちは明らかなアイデンティティを持っています

$$
\prod_{k < k'} (\gamma_k - \gamma_{k'}) = \prod_{i < i'} (\alpha_i - \alpha_{i'}) \cdot \prod_{j < j'} (\beta_j - \beta_{j'}) \cdot \prod_{i,j} (\alpha_i - \beta_j)
$$

On squaring this 関係 we obtain (57), by (40) and (46).

#### 系 2 {#alg-iv-s6-prop-11-cor-2 .statement tag=06FJ}

— If $a_0$ is 係数 of $X^m$ in $f$, we have

$$
\text{dis}_{m+1}(f) = a_0^2 \text{dis}_m(f)
$$

これはコルからの続きです。 公式 $\operatorname{res}_{m,1}(f,1) = a_0$ までに $n = 1,\ g = 1$ を取得すると 1 (IV、p. 76、例 1)。

#### 系 3 {#alg-iv-s6-prop-11-cor-3 .statement tag=06FK}

— Let $A$ be 体, and let $f$ be a non-constant polynomial in $A[X]$. For $f$ and $Df$ to be relatively prime, it is necessary and sufficient that $\mathrm{dis}(f) \neq 0$.
これは、提案 11、(iii) および Cor. 2 of IV, p. 78.

#### 注意 {#alg-iv-s6-n7-rem-1 .statement tag=06FL}

Corの二重適用。 2 above shows that we have $\mathrm{dis}_m(f) = 0$ for every polynomial $f$ of 次数 $\leq m - 2$.

#### 例 3 {#alg-iv-s6-n7-exa-3 .statement tag=06FM}

$m = 2$ にしましょう。 By Example2 (IV, p. 81) we have $\Delta(A_1, A_2) = A_1^2 - 4A_2$, よって $\tilde{\Delta}(A_0, A_1, A_2) = A_1^2 - 4A_0A_2$.その他の語では、
$$
\mathrm{dis}_2(a_0X^2 + a_1X + a_2) = a_1^2 - 4a_0a_2 .
$$

#### 例 4 {#alg-iv-s6-n7-exa-4 .statement tag=06FN}

Consider the polynomial
$$
F = A_0X^3 + 3A_1X^2 + 3A_2X + A,
$$
$Q[A_0, A_1, A_2, A_3]$の係数と。私たちは持っています
$$
DF = 3(A_0X^2 + 2A_1X + A_2) ,
$$
$$
F - 1/3X \cdot DF = A_1X^2 + 2A_2X + A_3 .
$$
By the formulae (54) (IV, p. 84) and (29) (IV, p. 77) we have
$$
A_0 \cdot \mathrm{dis}_3(F) = - \mathrm{res}_{2,3}(DF, F) = - \mathrm{res}_{2,3}(DF, F - 1/3X \cdot DF)
$$
適用 Cor. IV、p. 80の2つをついに入手
$$
\mathrm{dis}_3(F) = - 27 \mathrm{res}_{2,2}(A_0X^2 + 2A_1X + A_2,\ A_1X^2 + 2A_2X + A_3) .
$$
By 例 3 of IV, p. 80 we thus have
$$
\tilde{\Delta}(A_0, 3A_1, 3A_2, A_3) = - 27 (A_0A_3 - A_1A_2)^2 - 108 (A_1A_3 - A_2^2)(A_1^2 - A_0A_2) .
$$
後で some calculations we find, that if $f = a_0X^3 + a_1X^2 + a_2X + a_3$, we have
$$
\mathrm{dis}_3(f) = a_1^2a_2^2 + 18a_0a_1a_2a_3 - 4a_1^3a_3 - 4a_0a_2^3 - 27a_0^2a_3^2 .
$$
In particular, we have
$$
\mathrm{dis}(X^3 + pX + q) = - (4p^3 + 27q^2) .
$$

練習問題

### 練習問題 {#alg-iv-s6-exercises}

[§ 6 に対して練習問題](exercises/s6/)を参照してください。
