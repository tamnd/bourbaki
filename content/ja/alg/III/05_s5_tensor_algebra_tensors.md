---
book: alg
book_title: Algebra
chapter: III
chapter_title: TENSOR ALGEBRAS, EXTERIOR ALGEBRAS, SYMMETRIC ALGEBRAS
section: 5
section_title: Tensor algebra. Tensors
lang: ja
source: alg-i-iii
source_edition: 1998, Springer
book_pages: 484-497, 627-632
pdf_pages: 0508-0521, 0651-0656
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF THE TENSOR ALGEBRA OF A MODULE
      page: 484
      pdf_page: 508
    - "no": 2
      title: FUNCTORIAL PROPERTIES OF THE TENSOR ALGEBRA
      page: 485
      pdf_page: 509
    - "no": 3
      title: EXTENSION OF THE RING OF SCALARS
      page: 489
      pdf_page: 513
    - "no": 4
      title: DIRECT LIMIT OF TENSOR ALGEBRAS
      page: 490
      pdf_page: 514
    - "no": 5
      title: TENSOR ALGEBRA OF A DIRECT SUM. TENSOR ALGEBRA OF A FREE MODULE. TENSOR ALGEBRA OF A GRADED MODULE
      page: 491
      pdf_page: 515
    - "no": 6
      title: TENSORS AND TENSOR NOTATION
      page: 492
      pdf_page: 516
statements: 15
exercises: 10
content_sha256: fb63bd0996b2b99551137b21442d7295a10053b2660c214cda4d7cf52afed387
translated_from: content/en/alg/III/05_s5_tensor_algebra_tensors.md
translation_method: google
source_content_sha256: d99f913e6231ffa43f0356d794c4b307be8a5cb9b275a18c87c2f41e23c6d2fe
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-eeeca2ef
glossary_version: 34
glossary_terms_sha256: 12cf6c2515f7c4f3e156ac173745d6805c5a7c56632e7e0081504d2fd7196f82
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## § 5。 テンソル代数、テンソル

### 1. 定義/テンソル代数/加群

Aを可換環、MをA-加群とします。 M に等しい $n$ 加群のすべての整数 $n \geqslant 0$、A-加群テンソル積 (M の *n 番目のテンソル冪* とも呼ばれます) は、$\bigotimes^n M$、$M^{\otimes n}$、または$T^n(M)$、または $T^n_A(M)$、または $\mathrm{Tens}^n(M)$;次に$T^1(M) = M$; $T^0(M) = A$ とも書きます。 A-加群 *直和* $\bigoplus_{n \geqslant 0} T^n(M)$ は $T(M)$ または $\mathrm{Tens}(M)$ で表されます。 整数 $p \geqslant 0, q \geqslant 0$、A-線型写像のすべての注文済み対を定義することで、$T(M)$ で型 $\mathbf{N}$ の等級付けされた A-代数構造を定義するとします。
$$
m_{pq} : T^p(M) \otimes_A T^q(M) \to T^{p+q}(M)
$$
($§ 3$、no. 1、*注意*)。 $p > 0$ と $q > 0$ の場合、$m_{pq}$ は結合性同型 (II、$§ 3$、no. 9) であり、$p = 0$ (それぞれ$q = 0$) の場合、$m_{0,q}$ は結合性の標準同型になります。 $A \otimes_A T^q(M)$ から $T^q(M)$ (それぞれ $m_{p,0}$ は $T^p(M) \otimes_A A$ の標準同型から $T^p(M)$ (II、$§ 3$、no. 4、命題 4))。 次に、$x_i \in M$、$\alpha \in A$ については、
$$
\begin{align}
(x_1 \otimes \cdots \otimes x_p) \cdot (x_{p+1} \otimes \cdots \otimes x_{p+q}) &= x_1 \otimes \cdots \otimes x_p \otimes x_{p+1} \otimes \cdots \otimes x_{p+q} \\
\alpha \cdot (x_1 \otimes \cdots \otimes x_p) &= \alpha(x_1 \otimes \cdots \otimes x_p).
\end{align}
$$
$T(M)$ でこのように定義された乗法が *連想* であり、単位元単位元 1 の $A = T^0(M)$ として認められるのは明らかです。

#### 定義 1 {#alg-iii-s5-def-1 .statement tag=061H}

可換環 $A$、$M$ のテンソル代数のすべての加群 $M$ は、$T(M)$、$\mathrm{Tens}(M)$、$T_A(M)$ で示され、代数 $\bigoplus_{n \geq 0} T^n(M)$ になります。 (1) で定義された乗法を使用します。 標準単射 $\phi : T^1(M) \to T(M)$ (II, § 1, no. 12) ($\phi_M$ とも表記) は、$M$ の標準単射から $T(M)$ と呼ばれます。

#### 命題 1 {#alg-iii-s5-prop-1 .statement tag=061I}

$E$ を (単位的) $A$-代数、$f : M \to E$ を $A$-線形写像とする。 $f = g \circ \phi$ となるような $A$-代数準同型性 $g : T(M) \to E$ が 1 つだけ存在します。

他の語では、$(T(M), \phi)$ は普遍写像問題 (集合理論, IV, § 3, no. 1) の解であり、$\Sigma$ は $A$-代数構造の種であり、 $\alpha$-写像は、加群 $M$ から $A$-代数への $A$-線形写像です。ここでは、$T(M)$ に卒業することに疑問の余地がないことに注目してください。

すべての有限家族 $n$ 元 $M$ の$(x_i)_{1 \leq i \leq n}$、$T(M)$、$x_1 \otimes x_2 \otimes \cdots \otimes x_n = \phi(x_1)\phi(x_2)\ldots\phi(x_n)$ の積の定義について。その場合、$n \geq 1$ については必然的に $g(x_1 \otimes x_2 \otimes \cdots \otimes x_n) = f(x_1)f(x_2)\ldots f(x_n)$ となり、$\alpha \in A$ については $g(\alpha) = \alpha e$ ($e$ が $E$ の単位元の場合) となり、$g$ の一意性が証明されます。 Conversely, note that, for all $n > 0$, the mapping
$$
(x_1, \ldots, x_n) \mapsto f(x_1)f(x_2)\ldots f(x_n)
$$
of $M^n$ into $E$ is $A$-multilinear; hence there corresponds to it an $A$-linear mapping $g_n : T^n(M) \to E$ such that
$$
g(x_1 \otimes x_2 \otimes \cdots \otimes x_n) = f(x_1)f(x_2)\ldots f(x_n).
$$
Also we define the mapping $g_0 : T^0(M) \to E$ as equal to $\eta_E$ ($§ 1$, no. 3), in other words $g_0(\alpha) = \alpha e$ for $\alpha \in A$. $g$ を、$T(M)$ から $E$ への一意の $A$ 線形マッピングとし、制限から $T^n(M)$ が $g_n$ ($n \geq 0$) であるとします。 $g \circ \phi = g_1 = f$ は明らかであり、$g$ が $A$-代数準同型であることを検証する必要があります。 構成 $g(1) = e$ により、線形性により、$u \in T^p(M)$ と $v \in T^q(M)$ ($p > 0, q > 0$) に対して $g(uv) = g(u)g(v)$ であることが示されれば十分です。さて、式(1)と(2)から、この関係は$u = x_1 \otimes x_2 \otimes \cdots \otimes x_p$と$v \in x_{p+1} \otimes \cdots \otimes x_{p+q}$($x_i$属するから$E$)のときに真であることがわかります。 したがって、線形性により、$u \in T^p(M)$ と $v \in T^q(M)$ に当てはまります。

#### 注意 {#alg-iii-s5-n1-rem-1 .statement tag=061J}

$E$ が型 $\mathbf{Z}$ の段階化された $A$-代数であり、目盛が $(E_n)$ であると仮定します。また、次のように仮定します。
$$
f(M) \subset E_1.
$$
次に、(2) から、すべての $p \geq 0$ に対して $g(T^p(M)) \subset E_p$ となり、したがって $g$ は等級付けされた代数準同型になります。

### 2. テンソル代数の関数的性質

#### 命題 2 {#alg-iii-s5-prop-2 .statement tag=061K}

$A$ を 2 つの $A$ モジュールである可換環、$M$、$N$ とします。
$$
u : M \to N
$$

A-線型写像。たった一つだけ存在する A-代数準同型

$$
u': \mathbf{T}(M) \to \mathbf{T}(N)
$$

図式のように

$$
\begin{array}{ccc}
M & \xrightarrow{u} & N \\
\downarrow \phi_M & & \downarrow \phi_N \\
\mathbf{T}(M) & \xrightarrow{u'} & \mathbf{T}(N)
\end{array}
$$

可換です。 Further, $u'$ is a graded 代数準同型.

$u'$ の存在と一意性は、no. 1、命題 1 から続き、代数 $\mathbf{T}(N)$ と線形写像 $\phi_N \circ u : M \to \mathbf{T}(N)$ に適用されます。として

$$
u(M) \subset \mathbf{T}^1(N) = N,
$$

$u'$ がグレード付けされた代数準同型であるという事実は、no. 1 の注意から続きます。

命題 2 の準同型 $u'$ は、以降、$\mathbf{T}(u)$ で示されます。 If P is A-加群 and $v : N \to P$ A-線型写像, then

$$
\mathbf{T}(v \circ u) = \mathbf{T}(v) \circ \mathbf{T}(u)
$$

for $\mathbf{T}(v) \circ \mathbf{T}(u)$ は代数準同型で図式を可換にレンダリングします

$$
\begin{array}{ccc}
M & \xrightarrow{v \circ u} & P \\
\downarrow \phi_M & & \downarrow \phi_P \\
\mathbf{T}(M) & \xrightarrow{\mathbf{T}(v) \circ \mathbf{T}(u)} & \mathbf{T}(P)
\end{array}
$$

$\mathbf{T}(u)$ は、$u$ から $\mathbf{T}(M)$ (含む $M = \mathbf{T}^1(M)$) の標準拡大と呼ばれるときどきです。 制限 $\mathbf{T}^n(u) : \mathbf{T}^n(M) \to \mathbf{T}^n(N)$ はちょうど線形写像 $u^{\otimes n} = u \otimes u \otimes \cdots \otimes u$ (n 回) であることに注意してください。

$$
\mathbf{T}^n(u)(x_1 \otimes \cdots \otimes x_n) = u(x_1) \otimes \cdots \otimes u(x_n)
$$

$\mathbf{T}(u)$ は代数準同型と $\mathbf{T}^1(u) = u$ であるため、 制限 $\mathbf{T}^0(u)$ から A は恒等写像です。 $\mathbf{T}^n(u)$は、$u$の$n$番目のテンソル冪と呼ばれます。

#### 命題 3 {#alg-iii-s5-prop-3 .statement tag=061L}

*$u : M \to N$ が全射A-線型写像の場合、準同型 $\mathbf{T}(u) : \mathbf{T}(M) \to \mathbf{T}(N)$ は全射であり、その核は $u$ の核 $P \subset M \subset \mathbf{T}(M)$ によって生成される $\mathbf{T}(M)$ の両側イデアルです。

$\mathbf{T}^0(u) : \mathbf{T}^0(M) \to \mathbf{T}^0(N)$ は全単射であり、整数 $n > 0$ ごとに、

$$
\mathbf{T}^n(u) : \mathbf{T}^n(M) \to \mathbf{T}^n(N)
$$

is surjective, as is seen by induction on $n$ using II, § 3, no. 6, Proposition 6; the latter proposition also shows, by induction on $n$, that the kernel $\mathfrak{I}_n$ of $T^n(u)$ is the submodule of $T^n(M)$ generated by the products
$$
x_1 \otimes x_2 \otimes \cdots \otimes x_n
$$
where at least one of the $x_i$ belongs to $P$. これは、$T(u)$の核$\mathfrak{I} = \bigoplus_{n \geq 1} \mathfrak{I}_n$が、$T(M)$の$P$によって生成された両側イデアルであることを示しています。

$u : M \to N$ が*単射詞* 線形写像である場合、$T(u)$ が単射詞写像 (練習問題 1) であるとは限りません。ただし、これは、$u$ が単射で、$u(M)$ が $N$ の *直因子* である場合に当てはまります。その場合、$v \circ u$ が $M$ で恒等写像であるような線形写像 $v : N \to M$ が存在するため、
$$
T(v \circ u) = T(v) \circ T(u)
$$
は $T(M)$ 上の恒等写像であるため、 $T(u)$ は単射であり、その像 ($T(M)$ と同型) は $T(N)$ (II, § 1, no. 9, 命題 15) の *直因子* です。より正確には:

#### 命題 4 {#alg-iii-s5-prop-4 .statement tag=061M}

*$N$ と $P$ を $A$ モジュール $M$ の 2 つの部分加群とし、それらの和 $N + P$ が $M$ の直因子であり、共通部分 $N \cap P$ が$N$と$P$では直因子。次に、準同型 $T(N) \to T(M)$、$T(P) \to T(M)$、そして*
$$
T(N \cap P) \to T(M),
$$
*標準的な拡大の標準単射は単射です。 $T(N)$、$T(P)$、$T(N \cap P)$ が、準同型によって $T(M)$ の部分代数と識別される場合、*
(5)
$$
T(N \cap P) = T(N) \cap T(P).
$$

仮定までに、$N = N' \oplus (N \cap P)$、$P = P' \oplus (N \cap P)$ となるように、部分加群 $N' \subset N$ と $P' \subset P$ が存在します。それから
$$
N + P = N' \oplus P' \oplus (N \cap P)
$$
そして、$M$ のうち仮定部分加群 $M'$ までに次のようなものが存在します。
$$
M = M' \oplus (N + P) = M' \oplus N' \oplus P' \oplus (N \cap P) \\
= M' \oplus P' \oplus N = M' \oplus N' \oplus P.
$$

特に、$N + P$、$N$、$P$、$N \cap P$ は、$M$ では直因子であり、上で見たように、標準準同型であることを意味します。
$$
T(N + P) \to T(M), \quad T(N) \to T(M),
$$
$$
T(P) \to T(M), \quad T(N \cap P) \to T(M)
$$
は単射的です。したがって、3 つの代数 $T(N)$、$T(P)$、$T(N \cap P)$ は $T(N + P)$ の部分代数と識別され、後者は $T(M)$ の部分代数と識別されます。

$Q = N \cap P$ を書くと、$T(Q)$、$T(N' \oplus Q)$、$T(P' \oplus Q)$ が $T(N' \oplus P' \oplus Q)$ の部分代数と同一視される場合、次のことがわかります。

$$
T(N' \oplus Q) \cap T(P' \oplus Q) = T(Q).
$$

ここで、可換図式を考えてみましょう。

$$
\begin{array}{ccc}
N' \oplus Q & \longrightarrow & N' \oplus P' \oplus Q \\
\downarrow & & \downarrow \\
Q & \longrightarrow & P' \oplus Q
\end{array}
$$

ここで、水平方向の矢印は標準単射、垂直方向の矢印は正規の射影です。可換図式を導き出します。

$$
\begin{array}{ccc}
T(N' \oplus Q) & \overset{u}{\longrightarrow} & T(N' \oplus P' \oplus Q) \\
\downarrow r & & \downarrow s \\
T(Q) & \overset{v}{\longrightarrow} & T(P' \oplus Q)
\end{array}
$$

ここで、$r$ と $s$ は全射準同型 (命題 3)、$u$ と $v$ 単射準同型です。したがって、(6) を証明するには、右辺が左辺に明らかに含まれていることに注意してください。したがって、次のことを確認するだけで十分です。

$$
x \in T(N' \oplus Q) \cap T(P' \oplus Q),
$$

次に$x \in T(Q)$。ここで、準同型 $s$ の定義は、その制限から $T(P' \oplus Q)$ ($T(N' \oplus P' \oplus Q)$ の部分代数で識別される) が恒等写像であることを示しています。したがって、$x$ の仮定は $s(u(x)) = x$ を意味します。しかし、その後、$T(P' \oplus Q)$の$T(Q)$の他の語$x$属するから像も$v(r(x)) = x$となり、それが証明されることになりました。

#### 注意 {#alg-iii-s5-n2-rem-1 .statement tag=061N}

注意特に、$A$ が体 (II, § 7, no. 3, 命題 4) であるとき、$M$ の任意の部分加群 $N, P$ に対して命題 4 の仮説が常に成り立ちます。さらに、$N \subset P$と$N \neq P$の場合、すべての$n \geq 1$に対して$T^n(N) \neq T^n(P)$になります。$R$が$N$の$P$の補数である場合、(4)と$T^n(R) \neq \{0\}$により$T^n(P) \cap T^n(R) = \{0\}$になります。

#### 系 {#alg-iii-s5-n2-cor-1 .statement tag=061O}

*$K$を可換体、$M$ベクトル空間を$K$とします。 元 $z \in T(M)$ ごとに、$M$ の最小のベクトル空間 $N$ が存在し、$z \in T(N)$ と $N$ は $K$ を超える有限階数になります。*

この主張では、$M$ のベクトル部分空間 $P$ ごとに、$T(P)$ が $T(M)$ の部分代数と正規に識別されることがわかります。 Let $z \in T(M)$; $z$ can be expressed as a linear combination of elements each of which is a finite product of elements of $M = T^1(M)$; all the elements of $M$ which occur in these products generate a vector subspace $Q$ of finite rank and $z \in T(Q)$.

$\mathscr{F}$ を、有限階数のベクトル部分空間 $P$ の (空でない) 集合とし、$z \in T(P)$ とします。 $\mathscr{F}$ の元のすべての減少列は、有限階数のベクトル空間であるため、静止しています。したがって、$\mathscr{F}$ には最小の元 $N$ (集合理論, III, § 6, no. 5) が含まれます。 $P \in \mathscr{F}$ 含む $N$ ごとに検証する必要があります。今、$z \in T(P) \cap T(N) = T(P \cap N)$ (命題 4); $N$の定義を考慮すると、これは$N \cap P = N$、つまり$P \supset N$を意味します。

$M$ の部分空間 $N$ は、$z$ と *関連付けられている*と言われています。

### 3. スカラーの環の拡大

$A, A'$ を 2 つの可換環と $\rho : A \to A'$ 環準同型とします。 Let $M$ be an $A$-module, $M'$ an $A'$-module and $u : M \to M'$ an $A$-homomorphism; as the canonical injection $\phi_{M'} : M' \to T_{A'}(M')$ is also an $A$-homomorphism (by restriction of scalars), so is the composition $M \xrightarrow{u} M' \xrightarrow{\phi_{M'}} T_{A'}(M')$. $A$-代数準同型性 $T_A(M) \to \rho^*(T_{A'}(M'))$ が導出され (no. 2)、$T(u) : T_A(M) \to T_{A'}(M')$ によっても示されます。これは、図式を可換にする固有の $A$-準同型性です。

$$
\begin{array}{ccc}
M & \xrightarrow{u} & M' \\
\downarrow \phi_M & & \downarrow \phi_{M'} \\
T_A(M) & \xrightarrow{T(u)} & T_{A'}(M')
\end{array}
$$

If $\sigma : A' \to A''$ is a commutative ring homomorphism, $M''$ an $A''$-module and $v : M' \to M''$ an $A'$-homomorphism, the above uniqueness property shows that

$$
T(v \circ u) = T(v) \circ T(u).
$$

#### 命題 5 {#alg-iii-s5-prop-5 .statement tag=061P}

*$A, B$ を 2 つの可換環、$\rho : A \to B$ 環準同型、および $M$ の $A$ モジュールとします。正規の拡大*

$$
\psi : T_B(B \otimes_A M) \to B \otimes_A T_A(M)
$$

*B-線型写像* $l_B \otimes \phi_M : B \otimes_A M \to B \otimes_A T_A(M)$ * は段階的 B 代数* の同型です。

2 つの $A$-代数準同型性: 標準単射 $j : B = T^0(B \otimes_A M) \to T(B \otimes_A M)$ と準同型を考えてみましょう。

$$
h = T(i) : T(M) \to T(B \otimes_A M)
$$

正準 $A$ 線形マッピングから導出された (cf. 公式 (8))

$$
i : M \to B \otimes_A M.
$$

$T^0(B \otimes_A M)$は$T(B \otimes_A M)$の中心に含まれるので、§ 4, no. 2の命題5が適用でき、A-代数準同型が可能です

$$
\psi': B \otimes_A T(M) \to T(B \otimes_A M)
$$

は、$1 \leq i \leq n$ の $\beta \in B, x_i \in M$ に対して、

$$
\psi'(\beta \otimes (x_1 \otimes x_2 \otimes \cdots \otimes x_n)) = \beta((1 \otimes x_1) \otimes (1 \otimes x_2) \otimes \cdots \otimes (1 \otimes x_n)),
$$

これは、$\psi'$ も B 代数準同型であることをすぐに示します。 $\psi \circ \psi'$ と $\psi' \circ \psi$ がそれぞれ $B \otimes_A T(M)$ と $T(B \otimes_A M)$ で恒等写像であることを証明すれば十分です。さて、これら 2 つの代数は、$B \otimes_A M$ によって生成され、明らかに $\psi \circ \psi'$ と $\psi' \circ \psi$ 一致すると、$B \otimes_A M$ の恒等写像 、よっての結論です。

### 4. 直接極限/テンソル代数

$(A_\alpha, \phi_{\beta \alpha})$ を、$A_\alpha$ モジュール (II, § 6, no. 2) の可換環および $(M_\alpha, f_{\beta \alpha})$ 直接系の有向直接系とします。 $A = \lim \rightarrow A_\alpha$ と $M = \lim \rightarrow M_\alpha$ を考えます。これは $A$ モジュールです。 $\alpha \leq \beta$ の場合、$A_\alpha$-代数準同型 (no. 3, 公式 (8)) $f'_{\beta \alpha} = T(f_{\beta \alpha}): T_{A\alpha}(M_\alpha) \to T_{A\beta}(M_\beta)$ は $A_\alpha$-準準同型 $f_{\beta \alpha}: M_\alpha \to M_\beta$ から正準的に導出され、(9) (no. 3) から $(T_{A\alpha}(M_\alpha), f'_{\beta \alpha})$ は*$A_\alpha$-代数*の直接系。一方、$f'_\alpha: M_\alpha \to M$ を標準的な $A_\alpha$ 準同型写像とします。 $A_\alpha$-代数準同型性 $f'_\alpha: T_{A\alpha}(M_\alpha) \to T_A(M)$ が導出され (no. 3, 公式 (8))、また (9) (no. 3) から、$f'_\alpha$ が $A_\alpha$-準同型性の直接系を構成することがわかります。

#### 命題 6 {#alg-iii-s5-prop-6 .statement tag=061Q}

*A-準同型* $f' = \lim \rightarrow f'_\alpha : \lim \rightarrow T_{A\alpha}(M_\alpha) \to T_A(M)$ *は等級付けされた代数同型* です。

簡単にするために、$E = T_A(M)$ と $E' = \lim \rightarrow T_{A\alpha}(M_\alpha)$ を書いて、

$$
g_\alpha: T_{A\alpha}(M_\alpha) \to E'
$$

は標準的な $A_\alpha$-準同型性になります。明らかに、複合 $A_\alpha$-線形写像 $M_\alpha \xrightarrow{\phi_{M_\alpha}} T_{A\alpha}(M_\alpha) \xrightarrow{g_\alpha} E'$ 形直接系と、次のような $A$-線形写像 $u = \lim \rightarrow (g_\alpha \circ \phi_{M_\alpha}): M \to E'$ が唯一つ存在します。

$$
u \circ f_\alpha = g_\alpha \circ \phi_{M_\alpha}
$$

$\alpha$の皆さんへ。この写像自体は (no. 1, 命題 1) を $M \xrightarrow{\phi_M} E \to E'$ に一意に因数分解します。ここで、$h$ は $A$ 代数準同型です。 $h \circ f' = 1_{E'}$ と $f' \circ h = 1_E$ を証明すれば十分です。

この目的のために、添字 $\alpha$ ごとに、(no. 3, 公式 (8)) に注意してください。

$$
h \circ f'_\alpha \circ \phi_{M_\alpha} = h \circ \phi_M \circ f_\alpha = u \circ f_\alpha = g_\alpha \circ \phi_{M_\alpha}
$$

よって、一意性主張による no. 1、命題 1、

$$
h \circ f'_\alpha = g_\alpha
$$

すべての$\alpha$;すべての $\alpha$ に対して $(h \circ f') \circ g_\alpha = g_\alpha$ となり、したがって直接極限の定義により $h \circ f' = 1_{E'}$ となります。

一方、no. 3、公式 (8) により、

$$
f' \circ u \circ f_\alpha = f' \circ g_\alpha \circ \phi_{M_\alpha} = f'_\alpha \circ \phi_{M_\alpha} = \phi_M \circ f_\alpha,
$$

直接極限の定義により、再びよって $f' \circ u = \phi_M$。 no. 1、命題 1 の $f' \circ h \circ \phi_M = \phi_M$ と一意性性質を結論するとすると、$f' \circ h = 1_E$ になります。

命題 6 は、観察するとによって、$n$ 上の帰納法によって次のように、整数 $n \geq 1$ ごとに、正規の $A$ モジュール同型 $\lim \rightarrow T^n_{A_\alpha}(M_\alpha) \to T^n_A(M)$ が存在することを示すこともできます。 II, § 6, no. 3、命題 7. これらの同型が $f'$ の制限であることがすぐに検証されます。

### 5. テンソル代数の直和。 テンソル代数の自由加群。 加群のグレーディングのテンソル代数

$A$ を $A$ モジュールファミリーの可換環および $M = \bigoplus_{\lambda \in L} M_\lambda$ 直和とします。 II, § 3, no. 7, 命題 7 から、$n$ の帰納法により、$T^n(M)$ は部分加群の直和標準単射の像となります。

$$
M_{\lambda_1} \otimes M_{\lambda_2} \otimes \cdots \otimes M_{\lambda_n} \to T^n(M) = M^{\otimes n}
$$

*すべて* 数列 $(\lambda_i) \in L^n$ を基準にします。 $M_{\lambda_1} \otimes M_{\lambda_2} \otimes \cdots \otimes M_{\lambda_n}$ をこの像と同一視すると、$T(M)$ がすべての加群* の *直和であることがわかります。

$$
M_{\lambda_1} \otimes M_{\lambda_2} \otimes \cdots \otimes M_{\lambda_n}
$$

ここで、$n$ は $\mathbf{N}$ を通過し、各 $n$ について、$(\lambda_i)$ は $L^n$ を通過します。

まず次の帰結を導き出します。

#### 定理 1 {#alg-iii-s5-thm-1 .statement tag=061R}

*$A$ を可換環、$M$ を無料の $A$ モジュール、$M$ の $(e_\lambda)_{\lambda \in L}$ 基底とします。次に、元 $e_s = e_{\lambda_1} \otimes e_{\lambda_2} \otimes \cdots \otimes e_{\lambda_n}$、ここで、$s = (\lambda_1, \ldots, \lambda_n)$ は、$L$ の有限列の元の集合を通過し、$e_\varnothing$ は、$T(M)$、形の単位元を表すために使用されます。 $A$ モジュール $T(M)$ の基底。*

この基底の元は明らかに同次であり、 乗法表は次の式で与えられます。

$$
e_s e_t = e_{st}
$$

ここで、$st$ は、数列 $s$ と $t$ (I, § 7, no. 2) を*並べて* 取得した $L$ の元の数列を表します。

$T(M)$ の基底 $(e_s)$ は、乗法法則 (10) を使用して、集合 $L$ (I, § 7, no. 2) の *自由モノイド* と正準的に同型であり、同型はそれぞれ写像によって得られます。このモノイドの語 $s$ を元 $e_s$ に変換します。 (§ 2, no. 7) 自由加群 $M$ の *テンソル代数 $T(M)$ は、集合 $L$ の基底を使用して、$L$ の自由結合代数と正規同型であることがわかります。 $A$*。 特に (§ 2, no. 7, 命題 7)、$L$ から $A$-代数 $E$ までのすべての写像 $f : L \to E$ に対して、$\bar{f}(e_\lambda) = f(\lambda)$ となるような $A$-代数準同型性 $\bar{f} : T(M) \to E$ が 1 つだけ存在します。

#### 注意 {#alg-iii-s5-n5-rem-1 .statement tag=061S}

上記の結果は、II, § 3, no. 7、系 2 ～ 命題 7 を使用して、テンソル代数の自由結合代数の普遍的性質の帰結として同様に取得できます。

#### 系 {#alg-iii-s5-n5-cor-1 .statement tag=061T}

*$M$ が射影 $A$ 加群の場合、$T(M)$ は射影 $A$ 加群です。*

$M$ は空き $A$ モジュール $N$ (II, § 2, no. 2、命題 4) の直因子であるため、$T(M)$ は $T(N)$ (no. 2) の直因子です。 $T(N)$ は自由 (定理 1) なので、これは $T(M)$ が射影 (II, § 2, no. 2) であることを示しています。

#### 命題 7 {#alg-iii-s5-prop-7 .statement tag=061U}

*$\Delta$ を可換モノイド、$M$ を型 $\Delta$ および $(M_\alpha)_{\alpha \in \Delta}$ の段階的な $A$ 加群とする。 注文されたすべての対 $(\alpha, n) \in \Delta \times \mathbf{N}$ について、$T^{\alpha, n}(M)$ を部分加群 $M_{\alpha_1} \otimes M_{\alpha_2} \otimes \cdots \otimes M_{\alpha_n}$ $T^n(M)$ の (直接) 和とし、$\sum_{i=1}^n \alpha_i = \alpha$ とします。その場合、$(T^{\alpha, n}(M))_{(\alpha, n) \in \Delta \times \mathbf{N}}$ は、$T(M)$ の代数構造と互換性のある型 $\Delta \times \mathbf{N}$ の唯一の目盛りであり、$M = T^1(M)$ で指定された階調を誘導します。*

それはこのNo.の冒頭で見られました。 $T(M)$ は $T^{\alpha, n}(M)$ の直和であり、これが代数構造と互換性のある卒業であるという事実は、定義の直後に続きます。 $({T'}^{\alpha, n})$ が代数構造と互換性のある $T(M)$ の型 $\Delta \times \mathbf{N}$ の卒業他のであり、$\alpha \in \Delta$ の${T'}^{\alpha, 1}(M) = {T'}^{\alpha, 1}$ である場合、すべての $n \geq 1$ とすべてについて、定義からすぐに次のことが起こります。 $\alpha \in \Delta$、$T^{\alpha, n}(M) \subset {T'}^{\alpha, n}$;しかし、$T(M)$ は $T^{\alpha, n}(M)$ の直和でもあるため、これは ${T'}^{\alpha, n} = T^{\alpha, n}(M)$ (II, § 1, no. 8, *注意*) を意味します。

### 6. テンソルとテンソル記法

$A$を可換環、$M$を$A$モジュール、$M^*$を$M$(II, § 2, no. 3)と$I$と$J$の2つの*互いに素有限*集合の*双対*とします。 $A$モジュール$\bigotimes_{i \in I \cup J} E_i$。$i \in I$の場合は$E_i = M$、$i \in J$の場合は$E_i = M^*$は$T^I_J(M)$で表されます。 $T^I_J(M)$の元は、$M$よりも*型*のテンソル*$(I, J)$と呼ばれます。 $J = \varnothing$ の場合は *反変*、$I = \varnothing$ の場合は *共変*、それ以外の場合は *混合*と呼ばれます。

$I', I''$ を、$I$ の 2 つの部分集合と $J$ の 2 つの部分集合を$J', J''$ とし、$I' \cup I'' = I$ とします。

$I' \cap I'' = \varnothing,\ J' \cup J'' = J,\ J' \cap J'' = \varnothing$;その場合、正準結合性同型 (II, § 3, no. 9) が存在します。

$$
T_J^I(M) \to T_{J'}^{I'}(M) \otimes_A T_{J''}^{I''}(M).
$$

テンソル代数 $T(M \oplus M^*)$ を考慮すると、no. 5 から、$T^n(M \oplus M^*)$ は$T_J^I(M)$ の直和と正規的に識別され、I は区間の部分集合の集合を通過します。 $\mathbf{N}$と$J$の$\{1, n\}$は、$\{1, n\}$のIの補数です。

$I = \{1, p\}$ と $J = \{p + 1, p + q\}$ と整数 $p \geq 0,\ q \geq 0$ (ここで、$p = 0$ (それぞれ $q = 0$) のとき置き換える I (それぞれ J) を $\varnothing$ で表す)、A-加群 $T_J^I(M)$ も同様です$T_q^p(M)$で示されます。したがって、A-加群 $T_0^n(M)$ と $T_n^0(M)$ は、それぞれ定義 A-加群 $T^n(M)$ と $T^n(M^*)$ によって決まります。 I と J が基数 $p = \mathrm{Card}(I)$ と $q = \mathrm{Card}(J)$ の任意の有限集合である場合、それぞれに合計順序を与えます。その場合、I (それぞれ J) の増加する全単射が $\{1, p\}$ (それぞれ $\{p + 1, p + q\}$) 上に存在し、これらの全単射したがって定義する同型

$$
T_J^I(M) \to T_q^p(M).
$$

M が *有限生成射影* A-加群である場合、II, § 2, no. 7, 系 4 から命題 13 および II, § 4, no. 4, 系 1 から命題 4 から、標準同型が存在することがわかります。

$$
(T_J^I(M))^* \to T_I^J(M).
$$

ここで、M が *有限生成された自由* A-加群であり、$(e_\lambda)_{\lambda \in L}$ が M の基底であるとします (L したがって、*有限* 集合)。 $M^*$ *双対* から $(e_\lambda)$ (II, § 2, no. 6) の基底は、$(e^\lambda)_{\lambda \in L}$ で表されます。 M の基底 $(e_\lambda)$ と $(e^\lambda)$ と $M^*$ は、それぞれ $T_J^I(M)$ の定義する (no. 5) 基底であり、これは次のように明示的に与えられます: 2 つの写像 $f : I \to L$ と$g : J \to L$、$e_f^g$ を $T_J^I(M)$ の元 $\bigotimes_{i \in I \cup J} x_i$ とします。

$$
x_i = e_{f(i)} \quad \text{if } i \in I, \qquad x_i = e_{g(i)} \quad \text{if } i \in J.
$$

$(f, g)$ が、注文された対の写像 $f : I \to L$ と $g : J \to L$ の集合を通過すると、$e_f^g$ 形は A-加群 $T_J^I(M)$ の *基底* となります。 M の指定された基底 $(e_\lambda)$ に *関連付けられています。 したがって、 $z \in T_J^I(M)$ については、次のように書くことができます。

$$
z = \sum_{(f, g)} \alpha_g^f(z) \cdot e_f^g
$$

ここで、$\alpha_g^f$ は基底 $(e_f^g)$ を基準とした座標形です。言葉の乱用により、$\alpha_g^f(z)$ は、加群 M の基底* $(e_\lambda)$ に関して、テンソル $z$ の座標と呼ばれます。$\alpha_g^f$ は、$(e_f^g)$ の双対基底を構成し、他の語では、それらは語と同一視されます。 $T_I^J(M)$ の基底の元は、$(e_\lambda)$ と *関連付けられています*。 IとJが区間の$\{1, n\}$の$\mathbf{N}$の補数である部分集合の場合、$\alpha_g^f$（または$\alpha_g^f(z)$）は次のように表されます。$i \in I$の各元$f(i)$は上位として書かれます。 添字が i 番目にあり、$i \in J$ の i 番目にドットがあります。同様に、$i \in J$ の $g(i)$ は、$i \in I$ の i 番目にドットが付いた i 番目の下位の添字として書かれます。たとえば、$I = \{1, 4\}, J = \{2, 3\}$ の場合、$f(1) = \lambda, f(4) = \mu, g(2) = \nu, g(3) = \rho$ の場合、$\alpha_{v\rho}^{\lambda\cdot\cdot\mu}$ と書きます。

$(\tilde{e}_{\lambda})_{\lambda \in L}$を$(e_{\lambda})$から$(\tilde{e}_{\lambda})$(II, § 10, no. 8)までのMの他の基底と移行のPの行列とします。この場合、$(e^{\lambda})$ から $(\tilde{e}^{\lambda})$ までの移行の行列 ($(\tilde{e}_{\lambda})$ の双対基底) は、P (II, § 10, no. 8, 命題 5) の逆接 $^tP^{-1}$ です。したがって、(II, § 10, no. 10) 移行の行列は、$T^{I}_{J}(M)$ の基底 $(e^{g}_{f})$ から基底 $(\tilde{e}^{g}_{f})$ までとなります ($f$ (それぞれ $g$) は、集合を通過します) I の L への写像 (それぞれ J から L へ)) は行列

$$
\bigotimes_{i \in I \cup J} Q_{i}, \quad \text{where } Q_{i} = P \text{ if } i \in I, Q_{i} = {}^{t}P^{-1} \text{ if } i \in J.
$$

したがって、この行列の転置は次のように識別されます。

$$
\bigotimes_{i \in I \cup J} R_{i}, \quad \text{where } R_{i} = {}^{t}P^{-1} \text{ if } i \in I, R_{i} = P \text{ if } i \in J.
$$

ここで、M が任意の加群であると仮定します。 $i \in I, j \in J$ として、$I' = I - \{i\}, J' = J - \{j\}$ と書きます。私たちは定義するを正規の A-線型写像にします

$$
c^{i}_{j}: T^{I}_{J}(M) \to T^{I'}_{J'}(M),
$$

添字 i と添字 j の短縮と呼ばれます。このため、$M^{I} \times (M^{*})^{J}$ の写像がすべての家族 $(x_{i})_{i \in I \cup J}$ に関連付けられていることに注意してください。ここで、$i \in I$ の場合は $x_{i} \in M$、$i \in J$ の場合は $x_{i} \in M^{*}$、元

$$
\langle x_{i}, x_{j} \rangle_{k \in (I \cup J) - \{i, j\}} x_{k}
$$

$T^{I'}_{J'}(M)$ は A-多重線形です。 $c^{i}_{j}$ は対応する A-線型写像です。

ここで、M が自由で有限に生成されると仮定し、$(e_{\lambda})_{\lambda \in L}$ を M の基底とします。 2 つの写像 $f: I \to L, g: J \to L$ が与えられると、$f_{i}$ は $f$ ～ $I' = I - \{i\}$ と $g_{j}$ の制限を表すとします。 $g$ から $J' = J - \{j\}$ の制限;次に、(12) によって

$$
c^{i}_{j}(e^{g}_{f}) = \begin{cases} 0 & \text{if } f(i) \neq g(j) \\ e^{g_{j}}_{f_{i}} & \text{if } f(i) = g(j) \end{cases}
$$

z の座標のうち $c^{i}_{j}(z)$ の座標を写像として表す式が得られます。 I' のすべての写像 $f'$ (それぞれ $g'$) を L に (それぞれ J' を L に)、およびすべての $\lambda \in L$ について、$(f', \lambda)$ (それぞれ $(g', \lambda)$) を写像とします。 I から L (J から L) への制限から I' (J' へ) は $f'$ (それぞれ $g'$) で、元で値 $\lambda$ がかかります。 (それぞれ j)。次に、$T^{I'}_{J'}(M)$の基底$(e^{g'}_{f'})$に対する座標形を$\beta^{f'}_{g'}$とすると、

$$
\beta^{f'}_{g'}(c^{i}_{j}(z)) = \sum_{\lambda \in L} \alpha^{(f'; \lambda)}_{(g'; \lambda)}(z).
$$

例/テンソル。 (1) M を有限生成射影 A-加群とする。私たちは (II, § 4, no. 2、系 ～ 命題 2)、標準的 A-加群同型があることを知っています。

$$
\theta_M : M^* \otimes_A M \to \operatorname{End}_A(M)
$$

$\theta_M(x^* \otimes x)$ ($x \in M, x^* \in M^*$ の場合) は自己準同型となる

$$
y \mapsto \langle y, x^*\rangle x.
$$

したがって、$\theta_M$ によって、$T^{(2)}_{\{1\}}(M)$ ($T^1_1(M)$ と同型) は A-加群 $\operatorname{End}_A(M)$ と識別できます。 M が自由加群で、$(e_\lambda)_{\lambda \in L}$ が M の基底であるとします。この加群の基底$(e^\mu \otimes e_\lambda)$に対するテンソル$z \in M^* \otimes M$の座標は$\zeta_{\mu \cdot \lambda}$で表されます。 $\theta_M(e^\mu \otimes e_\lambda)$ は自己準同型 $y \mapsto \langle y, e^\mu\rangle e_\lambda$ であるため、自己準同型 $u = \theta_M(z) = \theta_M\left( \sum_{\lambda, \mu} \zeta_{\mu \cdot \lambda} e^\mu \otimes e_\lambda \right)$ 写像 $y$ から $\sum_{\lambda, \mu} \zeta_{\mu \cdot \lambda} \langle y, e^\mu\rangle e_\lambda$ となります。 $y = e_\lambda$と書くと、関係が得られます

$$
u(e_\lambda) = \sum_{\mu \in L} \zeta_{\lambda \cdot \mu} e_\mu
$$

他の語、線形写像* $u = \theta_M(z)$ の *行列 * は、添字* $\mu$ * と添字* の列 $\lambda$ * の行の元が * であるものです$\zeta_{\lambda \cdot \mu}$。

$u$ (II, § 4, no. 3) の *トレース* の定義は、次のことをすぐに示しています。

$$
\operatorname{Tr}(\theta_M(z)) = c_1^2(z).
$$

したがって、元 $z_0 = \sum_{\lambda \in L} e^\lambda \otimes e_\lambda$ (その座標 $\zeta_{\mu \cdot \lambda}$ は、$\lambda \neq \mu$ では零であり、$\lambda = \mu$ では 1 に等しい)、つまり $\theta_M(z_0) = 1_M$ は、以下の元 $1 \in A = T^0_0(M)$ の像になります。 写像収縮の*転置*

$$
c_1^2 : T^{(2)}_{\{1\}}(M) \to A.
$$

(2) M が有限生成射影 A-加群であると常に仮定します。標準的 A-加群同型があります

$$
\mu : M^* \otimes_A M^* \to (M \otimes_A M)^*
$$

(II, § 4, no. 4、系 1 ～ 命題 2) および標準同型

$$
\theta : (M \otimes_A M)^* \otimes_A M \to \operatorname{Hom}_A(M \otimes_A M, M)
$$

(II, § 4, no. 2、系 ～ 命題 2);また、$\operatorname{Hom}_A(M \otimes_A M, M)$ は、A-*bilinear* 写像の $M \times M$ の A-加群 $\mathscr{L}_2(M, M; M)$ から $M$ (II, § 3, no. 9) と正準的に同型です。これら同型、標準同型を合成すると、

$$
\chi_M : T^{(3)}_{\{1, 2\}}(M) = M^* \otimes M^* \otimes M \to \mathscr{L}_2(M, M; M)
$$

$M^*$、$z \in M$、$\chi_M(x^* \otimes y^* \otimes z)$ の $x^*, y^*$ については、双線形写像となる
$$
(u, v) \mapsto \langle u, x^*\rangle \langle v, y^*\rangle z.
$$
したがって、$\chi_M$ によって、$T_{\{1, 2\}}^{(3)}(M)$ ($T_2^1(M)$ と同型) は A-加群 $\mathscr{L}_2(M, M; M)$ と識別できます。 M が自由A-加群で、$(e_\lambda)_{\lambda \in L}$ が M の基底であるとします。この加群の基底$(e^\lambda \otimes e^\mu \otimes e_\nu)$に対するテンソル$z \in M^* \otimes M^* \otimes M$の座標は$\zeta_{\lambda \mu \nu}$で表されます。双線形写像 $\chi_M(z)$ 写像の順序付け対 $(e_\lambda, e_\mu)$ は、
$$
\sum_{\nu \in L} \zeta_{\lambda \mu \nu} e_\nu
$$
したがって、$\zeta_{\lambda \mu \nu}$ は、基底 $(e_\lambda)$ (§ 1, no. 7) に関して、双線形写像 $\chi_M(z)$ によって M 上で定義される (一般に非結合的な) 代数の構造* の * 定数にすぎません。

#### 注意 2 {#alg-iii-s5-n6-rem-2 .statement tag=061V}

$(e_\lambda)_{\lambda \in L}$、$(\bar{e}_\lambda)_{\lambda \in L}$を$(e_\lambda)$から$(\bar{e}_\lambda)$への通過のMとPの2つの基底行列とする。 *例 1* で見られたことを考慮して、添字 $\lambda$ と添字 $\mu$ の列の行に現れる P の元は、逆数の $\alpha_\mu^\lambda$ と元で表されます。 添字 $\mu$ の添字 $\lambda$ と列の行に現れる${}^tP^{-1}$ を$\beta_\lambda^\mu$ と表記します。次に（上で紹介した記法で）
$$
\begin{cases}
\bar{e}_\mu = \sum_\lambda \alpha_\mu^\lambda e_\lambda \\
\bar{e}^\mu = \sum_\lambda \beta_\lambda^\mu e_\lambda
\end{cases}
$$
$$
\bar{e}_{f'}^{g'} = \sum_{(f', g)} \left( \prod_{i \in I} \alpha_{f'(i)}^{f(i)} \right) \left( \prod_{j \in J} \beta_{g(j)}^{g'(j)} \right) e_f^g
$$
写像 $f': I \to L$ と $g': J \to L$ 全員に。したがって、基底 $(e_\lambda)$ に対するテンソル $z \in T_J^I(M)$ の座標 $\zeta_g^f$ は、次の式を使用して、基底 $(\bar{e}_\lambda)$ に対する z の座標 $\bar{\zeta}_{g'}^{f'}$ の項で表すことができます。
$$
\zeta_g^f = \sum_{(f', g')} \left( \prod_{i \in I} \alpha_{g'(i)}^{g(i)} \right) \left( \prod_{j \in J} \beta_{f'(j)}^{f(j)} \right) \bar{\zeta}_{g'}^{f'}
$$
基底 $(\bar{e}_\lambda)$ から基底 $(e_\lambda)$ への通過の行列 $P^{-1}$ は、${}^tP^{-1}$ の転置であるため、$\beta_\lambda^\mu$ は、列に現れる元になります。 添字 $\lambda$ と $P^{-1}$ の添字 $\mu$ の行。したがって、$\bar{e}_{f'}^{g'}$の項の$e_f^g$と、$\zeta_g^f$の項の$\bar{\zeta}_{g'}^{f'}$の計算は、置き換えること、$\alpha_\mu^\lambda$、$\beta_\lambda^\mu$、$\beta_\lambda^\mu$によって行われます。上記の計算では$\alpha_\mu^\lambda$となり、$f$と$f'$の役割と$g$と$g'$の役割を交換します。それから
$$
e_f^g = \sum_{(f', g')} \left( \prod_{j \in J} \alpha_{g'(j)}^{g(j)} \right) \left( \prod_{i \in I} \beta_{f'(i)}^{f(i)} \right) \bar{e}_{f'}^{g'}
$$

(23)
$$
\bar{\zeta}_{g'}^{f'} = \sum_{(f,g)} \left( \prod_{j \in J} \alpha_{g'(j)}^{g(j)} \right) \left( \prod_{i \in I} \beta_{f(i)}^{f'(i)} \right) \zeta_g^f.
$$

上記の式は、合計が添字を超え、下位添字として 1 回、上位添字として 1 回表示されます。一部の著者は、このような状況のため、和記号を抑制することを許可しています。

### 練習問題 {#alg-iii-s5-exercises}

[§ 5 に対して練習問題](exercises/s5/)を参照してください。
