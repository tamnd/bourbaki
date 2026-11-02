---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Semisimple Modules and Rings
section: 2
section_title: Determinants over a Noncommutative Field
appendix: true
lang: ja
source: alg-viii
source_edition: 2023, Springer Nature
book_pages: A VIII.447-A VIII.460
pdf_pages: 0464-0477
extraction: native
subsections:
    - "no": 1
      title: A Generalization of Alternating Multilinear Forms
      page: 447
      pdf_page: 464
    - "no": 2
      title: A Uniqueness Theorem
      page: 448
      pdf_page: 465
    - "no": 3
      title: Determinant of an Automorphism
      page: 452
      pdf_page: 469
    - "no": 4
      title: Determinant of a Square Matrix
      page: 452
      pdf_page: 469
    - "no": 5
      title: The Unimodular Group
      page: 455
      pdf_page: 472
statements: 18
exercises: 4
content_sha256: 3bd1488c22d62551f7288ae661cfe4028885e1108b5d186ed126531786c2cfd5
translated_from: content/en/alg/VIII/A2_a2_determinants_over_a_noncommutative_field.md
translation_method: google
source_content_sha256: a1a346c55a436d2ed8247c3e3a5bc5302eaac2c7930a98ff5617acbf65dc1b0e
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-b071ad41
glossary_version: 34
glossary_terms_sha256: 32687bcb686da7f1c6fb20bb2d26250cf7ca125fe84f18921539d70264cdbc3a
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## 付録 2 行列式斜体

この付録では、Dは体で、$D^*_{ab}$は、その導来群(I, §6, No. 2、p. 70)により、Dの乗法群$D^*$の商になります。 群 $D^*_{ab}$ は可換であり、体 D が可換である場合、$D^*_{ab}$ は $D^*$ と識別できます。 $D^*$から$D^*_{ab}$までの標準準同型を$\pi$で表します。

### 1. 一般化/交代的マルチリニア形

V を有限次元 $n\geqslant 0$ の体 D よりも右ベクトル空間とします。 Vの基底のB(V)集合と、B(V)から$D^*_{ab}$までの写像$\omega$のΩ(V)集合で、 満たす次の 2 つ条件:

a) $\lambda_1, . . . , \lambda_n$ が $D^*$ の元である場合、次のようになります。

$$
\omega (v_1\lambda_1, . . . , v_n\lambda_n) =\pi (\lambda_1\cdots \lambda_n)\omega (v_1, . . . , v_n) \tag{1}
$$

V の基底 $(v_1, . . . , v_n)$ ごとに。

b) $i$ と $j$ が区間 $[1, n]$ の 2 つの相異なる整数である場合、次のようになります。

$$
\omega (v_1, . . . , v_{i-1}, v_i+v_j, v_{i+1}, . . . , v_n) =\omega (v_1, . . . , v_n) \tag{2}
$$

V の基底 $(v_1, . . . , v_n)$ ごとに。

$\omega$をΩ(V)の元とします。 $(v_1, . . . , v_n)$ を V の基底と区間 $[1, n-1]$ の $i$ 整数とします。 by 性質 b)、

$$
\omega (v_1, . . . , v_i, v_{i+1}, . . . , v_n) =\omega (v_1, . . . , v_i+v_{i+1}, v_{i+1}, . . . , v_n)
$$

$$
=\omega (v_1, . . . , v_i+v_{i+1}, v_{i+1}-(v_i+v_{i+1}), . . . , v_n)
$$

$$
=\omega (v_1, . . . , v_i+v_{i+1},-v_i, . . . , v_n)
$$

$$
=\omega (v_1, . . . ,(v_i+v_{i+1})-v_i,-v_i, . . . , v_n)
$$

したがって

$$
\omega (v_1, . . . , v_i, v_{i+1}, . . . , v_n) =\pi (-1)\omega (v_1, . . . , v_{i+1}, v_i, . . . , v_n) \tag{3}
$$

対称群 $\mathfrak{S}_n$ は、区間 $[1, n]$ (I, §5, No. 7、p. 63、命題 9) の 2 つの連続する元の転置によって生成されるため、公式 (3) は次のように一般化されます。

$$
\omega (v_{\sigma(1)}, . . . , v_{\sigma(n)}) =\pi (\varepsilon (\sigma ))\omega (v_1, . . . , v_n) \tag{4}
$$

ここで、$\sigma$ 属するから $\mathfrak{S}_n$ および $\varepsilon (\sigma )$ はその署名 (I, §5, No. 7、p. 64) です。

公式 (2) は次のように一般化されます。まず、$D^*$ の各 $\lambda$ について、

$$
\omega (v_1, . . . , v_n) =\pi (\lambda )\omega (v_1, . . . , v_i\lambda^{-1}, . . . , v_n)
$$

$$
=\pi (\lambda )\omega (v_1, . . . , v_i\lambda^{-1}+v_j, . . . , v_n)
$$

$$
=\omega (v_1, . . . ,(v_i\lambda^{-1}+v_j)\lambda , . . . , v_n)
$$

つまり、

$$
\omega (v_1, . . . , v_n) =\omega (v_1, . . . , v_i+v_j\lambda , . . . , v_n) \tag{5}
$$

明らか帰納法までに、私たちは推測します

$$
\omega (v_1, . . . , v_n) =\omega (v_1, . . . , v_i+w, . . . , v_n) \tag{6}
$$

ベクトル $v_j$ のすべての線形結合 $w=\sum_{j\not=i}v_j\lambda_j$ について、区間 $[1, n]$ の $i$ とは異なる $j$ について。

### 2. 一意性定理

この小節では、厳密には正の整数 $m$、区間 $[1, m]$ の任意の整数 $i$、および $V^m$ の任意の数列 $(v_1, . . . , v_m)$ に対して、次のように書きます。 $V^{m-1}$の数列$(v_1, . . . , v_{i-1}, v_{i+1}, . . . , v_m)$の$(v_1, . . . ,\widehat{v}_i, . . . , v_m)$。

#### 命題 1 {#alg-viii-a2-prop-1 .statement tag=00Q1}

W を V の超平面 、$e$ を V-W のベクトルとします。$\varphi$ を Ω(W) の元とします。 Ω(V) の一意元 $\omega$ が存在します。

$$
\omega (w_1, . . . , w_{n-1}, e) =\varphi (w_1, . . . , w_{n-1}) \tag{7}
$$

W の基底 $(w_1, . . . , w_{n-1})$ ごとに。

A) $\omega :$の一意性 $\omega$をΩ(V)の元とします。 $(v_1, . . . , v_n)$をVの基底とし、$\mu_1, . . . , \mu_n$をこの基底における$e$の座標とします。 $\mu_i\not= 0$ のように 1 から $n$ (両端を含む) までの整数の I 集合で表します。空ではありません。 $i$をIの元とします。 数列 $(v_1, . . . ,\widehat{v}_i, . . . , v_n, e)$ は V の基底であり、$e-v_i\mu_i$ は数列 $(v_1, . . . ,\widehat{v}_i, . . . , v_n)$ の線形結合であるため、公式 (6) は意味します

$$
\omega (v_1, . . . ,\widehat{v}_i, . . . , v_n, v_i\mu_i) =\omega (v_1, . . . ,\widehat{v}_i, . . . , v_n, e) \tag{8}
$$

公式 (1) と (3) から、この等式の左辺は $\pi (-1)^{n-i}\pi (\mu_i)\omega (v_1, . . . , v_n)$ に等しいことがわかります。 V の $p$ 射影子を像 W と核 $eD$ で表します。 ベクトル $v_j-p(v_j)$ は $e$ に比例し、適用公式 (6) を繰り返すと、公式 (8) の右辺が $\omega (p(v_1), . . . ,\widehat{p}(v_i), . . . , p(v_n), e)$ に等しいことがわかります。

このことから、$\omega$ が関係 (7) を満たす場合、次のようになります。

$$
\omega (v_1, . . . , v_n) =\pi (-1)^{n-i}\pi (\mu_i)^{-1}\varphi (p(v_1), . . . ,\widehat{p}(v_i), . . . , p(v_n)) \tag{9}
$$

I の $i$ ごとに、$\omega$ の一意性が証明されます。

B) $\omega :$ の構成 $(v_1, . . . , v_n)$ を V の基底とします。私たちは上記の通り定義する $\mu_1, . . . , \mu_n$ と I です。 I のすべての $i$ について、仮定 $\mu_i\not= 0$ は、数列 $(v_1, . . . ,\widehat{v}_i, . . . , v_n, e)$ 生成する空間 V を意味するので、数列 $(p(v_1), . . . ,\widehat{p}(v_i), . . . , p(v_n))$ 生成する空間 $W =p(V)$。他の語では、この最後の数列はWの基底であり、

$$
t_i=\pi (-1)^{n-i}\pi (\mu_i)^{-1}\varphi (p(v_1), . . . ,\widehat{p}(v_i), . . . , p(v_n)) \tag{10}
$$

定義する元/$D^*_{ab}$。

$i$ と $j$ を I の 2 つの元とし、$i < j$ とします。 等式 $t_i=t_j$ を証明しましょう。 定義により、ベクトル $v_i\mu_i+v_j\mu_j-e$は、$i$や$j$とは異なる$k$のベクトル$p(v_k)$の線形結合になります。従って、$p(v_i)\mu_i+p(v_j)\mu_j$ は、$i$ や $j$ とは異なる、$k$ のベクトル $p(v_k)$ の線形結合になります。従って、公式 (6) までに、次のようになります。

$$
\varphi (p(v_1), . . . ,p(\widehat{v}_i), . . . ,p(\widehat{v}_j), . . . , p(v_n), p(v_i)\mu_i)
$$

$$
=\varphi (p(v_1), . . . ,p(\widehat{v}_i), . . . ,p(\widehat{v}_j), . . . , p(v_n),-p(v_j)\mu_j)
$$

適用公式 (1) と (3) により、次のようになります。

$$
\varphi (p(v_1), . . . ,p(\widehat{v}_j), . . . , p(v_n))\pi (\mu_i)\pi (-1)^{n-i-1}
$$

$$
=\varphi (p(v_1), . . . ,\widehat{p}(v_i), . . . , p(v_n))\pi (-\mu_j)\pi (-1)^{n-j}
$$

従って $t_i=t_j$ です。

これを証明すると、Iの$i$に対する$t_i$の共通の値として定義する$\omega (v_1, . . . , v_n)$となります。したがって、関係 (9) を満たす B(V) から $D^*_{ab}$ まで写像 $\omega$ を構成しました。 $(w_1, . . . , w_{n-1})$ を W の基底とします。 $1\leqslant i\leqslant n-1$ と $v_n=e$ を集合 $v_i=w_i$ とすると、$I =\{n\}$ と $\mu_n= 1$ になります。さらに、$1\leqslant i\leqslant n-1$ に対して $p(v_i) =w_i$ があり、公式 $\omega (w_1, . . . , w_{n-1}, e) =\varphi (w_1, . . . , w_{n-1})$ は (9) の具体的なケースです。

ここで、$\omega$ 属するが Ω(V) であることを証明しなければなりません。

C) 公式の証明 (1): $\lambda_1, . . . , \lambda_n$ を $D^*$ の元とし、$(v_1, . . . , v_n)$ を V の基底とします。上記の通り、定義する $\mu_1, . . . , \mu_n$ と I です。 Iの選ぶと$i$。 $e=\sum^n_{j=1}(v_j\lambda_j)(\lambda^{-1}_j\mu_j)$ があるため、公式 (9) は次のことを意味します。

$$
\omega (v_1\lambda_1, . . . , v_n\lambda_n) \tag{11}
$$

$$
=\pi (-1)^{n-i}\pi (\lambda^{-1}_i\mu_i)^{-1}\varphi (p(v_1)\lambda_1, . . . ,\widehat{p(v_i)\lambda_i}, . . . , p(v_n)\lambda_n)
$$

しかし、私たちには$\pi (\lambda^{-1}_i\mu_i)^{-1}=\pi (\mu_i)^{-1}\pi (\lambda_i)$があり、

$$
\varphi (p(v_1)\lambda_1, . . . ,\widehat{p(v_i)\lambda_i}, . . . , p(v_n)\lambda_n)
$$

$$
=\varphi (p(v_1), . . . ,\widehat{p(v_i)}, . . . , p(v_n))\pi (\lambda_1. . .\widehat{\lambda}_i. . . \lambda_n)
$$

公式 (9) と (11) を比較すると、目的の関係が得られます。

$$
\omega (v_1\lambda_1, . . . , v_n\lambda_n) =\omega (v_1, . . . , v_n)\pi (\lambda_1. . . \lambda_n)
$$

D) 公式の証明 (2): $(v_1, . . . , v_n)$ を V の基底とし、$i, j$ を区間 $[1, n]$ の 2 つの相異なる整数とします。私たちは定義する $\mu_1, . . . , \mu_n$ として前にです。 $k\not=i$ に対して $v'_i=v_i+v_j$ と $v'_k=v_k$ によって定義される V の基底 $(v'_1, . . . , v'_n)$ を考え、この基底に関して$e$ の座標 $\mu'_1, . . . , \mu'_n$ を導入しましょう。 満たす $\mu'_j=\mu_j-\mu_i$ と $\mu'_k=\mu_k$ は $k\not=j$ です。私たちは集合 $t=\omega (v_1, . . . , v_n)$ と $t'=\omega (v'_1, . . . , v'_n)$ です。 証明しなければならない $t$ と $t'$ は等しいと考えます。

まず、$\omega$ の定義までに、

$$
t=\pi (-1)^{n-k}\pi (\mu_k)^{-1}\varphi (p(v_1), . . . ,\widehat{p(v_k)}, . . . , p(v_n)) \tag{12}
$$

$$
t'=\pi (-1)^{n-k}\pi (\mu'_k)^{-1}\varphi (p(v'_1), . . . ,\widehat{p(v'_k)}, . . . , p(v'_n)) \tag{13}
$$

$\mu_k$ と $\mu'_k$ が非零となるように、すべての $k$ に対して。

a) $\mu_i\not=0$ の場合、数列 $(p(v_1), . . . ,\widehat{p(v_k)}, . . . , p(v_n))$ と $(p(v'_1), . . . ,\widehat{p(v'_k)}, . . . , p(v'_n))$ は等しく、$\mu_i$ = $\mu'_i$ となり、$t=t'$ となります。

b) $i$ と $j$ とは異なり、$\mu_k\not= 0$ となる添字 $k$ が存在する場合、$l\not=i$ と $p(v'_i) =p(v_i) +p(v_j)$ には $p(v'_l) =p(v_l)$ が存在します。 元 $p(v_i)$ と $p(v_j)$ はどちらも属するから数列 $(p(v_1), . . . ,p(\widehat{v}_k), . . . , p(v_n))$ までです。 $\varphi$ 属するから Ω(W) なので、VIII、p. 447 の公式 (2) が適用されます。それは与える

$$
\varphi (p(v_1), . . . ,p(\widehat{v}_k), . . . , p(v_n)) =\varphi (p(v'_1), . . . ,p(\widehat{v}'_k), . . . , p(v'_n))
$$

しかし、$\mu_k=\mu'_k$ もあるので、$t=t'$ もあります。

c) $\mu_k\not= 0$ が $j$ であるような添字 $k$ のみの場合を検討する必要があります。次に、$\mu'_j=\mu_j,e=v_j\mu_j$と$p(v_j) = 0$があります。 公式 (12) と (13) の集合 $k=j$。 数列 $(p(v_1), . . . ,p(\widehat{v}_j), . . . , p(v_n))$ と $(p(v'_1), . . . ,p(\widehat{v}'_j), . . . , p(v'_n))$ は等しいので、$t=t'$ になります。

#### 系 1 {#alg-viii-a2-prop-1-cor-1 .statement tag=00Q2}

$(e_1, . . . , e_n)$ を V の基底および $D^*_{ab}$ の $t$ 元とします。 $\omega (e_1, . . . , e_n) =t$となるようなΩ(V)の一意元$\omega$が存在します。

$n$ で帰納法によって系を証明しましょう。 $n= 0$ の場合、V の基底のみが空であるため、主張が真になります。ここで、$n\geqslant 1$ と仮定します。 $e_1, . . . , e_{n-1}$ によって生成された V の W 部分空間で示されます。 命題 1 までに、Ω(V) から Ω(W) 満たすまでの全単射 Λ が存在します。

$$
(\Lambda (\omega ))(w_1, . . . , w_{n-1}) =\omega (w_1, . . . , w_{n-1}, e_n)
$$

W のすべての基底 $(w_1, . . . , w_{n-1})$ と Ω(V) のすべての $\omega$ に対して。 帰納法の仮定までに、$\varphi (e_1, . . . , e_{n-1}) =t$となるようなΩ(W)の一意元$\varphi$が存在します。 関係 $\omega (e_1, . . . , e_n) =t$ は、Ω(V) の $\omega$ に対して、$\Lambda (\omega ) =\varphi$ と同等です。 系 1が続きます。

#### 系 2 {#alg-viii-a2-prop-1-cor-2 .statement tag=00Q3}

$\omega$と$\omega '$をΩ(V)の2つの元とします。 $\omega '=t\omega$ となるような $D^*_{ab}$ の一意元 $t$ が存在します。

#### 注意 {#alg-viii-a2-n2-rem-1 .statement tag=00Q4}

体 D が可換であると仮定します。 定義により、B(V)は$V^n$の部分集合になります。 非零交代的 $n$ の制限から B(V) への線形形 $f: V^n\rightarrow D$ 属するから Ω(V) であることは明らかです。 Moreover, if $(e_1, . . . , e_n)$ is a basis of V and $t$ is a nonzero element of D, then there exists a unique alternating $n$-linear form $f$ such that $f(e_1, . . . , e_n) =t$ (III, §7, No. 4, p. 511 and III, §7, No. 8, p. 518). 系 1 により、集合 Ω(V) は、非零交代的 $n$ の線形形式の制限から B(V) で構成されます。

### 3. 自己同型中行列式

まず、体 D が可換であると仮定します。 In view of the remark above, the determinant of an automorphism $u$ of V is the unique element det $u$ of $D^*$ such that we have

(14) $\omega (u(v_1), . . . , u(v_n)) =$ (デット $u$)$\omega (v_1, . . . , v_n)$

V のすべての基底 $(v_1, . . . , v_n)$ と Ω(V) のすべての元 $\omega$ に対して。

D が可換であると想定されていない場合に戻りましょう。

#### 命題 2 {#alg-viii-a2-prop-2 .statement tag=00Q5}

a) $u$ を V の自己同型とします。 det $u$ で示され、$u$ の行列式と呼ばれる、$D^*_{ab}$ の一意元が存在します。

(15) $\omega (u(v_1), . . . , u(v_n)) =$ (デット $u$)$\omega (v_1, . . . , v_n)$

V のすべての基底 $(v_1, . . . , v_n)$ と、Ω(V) のすべての $\omega$ に対して。

b) $\mathbf{G}\mathbf{L}(V)$ から $D^*_{ab}$ までの写像 $u\mapsto$ det $u$ は群準同型です。

$\omega_0$をΩ(V)の元とします。 写像 $(v_1, . . . , v_n)\mapsto$ $\omega_0(u(v_1), . . . , u(v_n))$ B(V)から$D^*_{ab}$ 属するからΩ(V)。 VIII の系 2、p. 451 までに、$D^*_{ab}$ の一意元 $t$ が存在します。

$$
\omega_0(u(v_1), . . . , u(v_n)) =t\omega_0(v_1, . . . , v_n)
$$

B(V)の$(v_1, . . . , v_n)$の場合。 $\omega$ が Ω(V) の他の元である場合、$D^*_{ab}$ の元 $s$ が存在します。

$$
\omega (v_1, . . . , v_n) =s\omega_0(v_1, . . . , v_n)
$$

V の基底 $(v_1, . . . , v_n)$ ごとに。すぐに関係と推測します

$$
\omega (u(v_1), . . . , u(v_n)) =t\omega (v_1, . . . , v_n)
$$

これは次のことを証明します。 主張 b) は a) の明らか帰結です。

### 4. 行列式/平方行列

$n$を正の整数とします。上記を体 D 上の右ベクトル空間 $D^n_d$ に適用してみましょう。 $D^n_d$ の元は、$n$ 行と 1 つの列を持つ行列として表示されます。 $(\varepsilon_1, . . . , \varepsilon_n)$を$D^n_d$の標準基底とします。 VIII, p. 451 の系 2 までに、$\omega_0(\varepsilon_1, . . . , \varepsilon_n) = 1$ となる $\Omega (D^n_d)$ の一意元 $\omega_0$ が存在します。 A が $\mathbf{G}\mathbf{L}_n$(D) の元である場合、その列 $a_1, . . . , a_n$ 形基底 $D^n_d$ です。 $D^*_{ab}$ の元 $\omega_0(a_1, . . . , a_n)$ は A の行列式と呼ばれ、det(A) で表されます。 $1\leqslant i\leqslant n$ に対して $a_i=A\varepsilon_i$ があるので、A の行列式は単純に自己同型の行列式 $D^n_d$ の $x\mapsto Ax$ です。特に、体 D が可換である場合、一致するの行列式は、III, §8, No. 3、p. 524 で定義されたものとなります。

V を体 D 上の有限次元 $n$ の右ベクトル空間とし、$(e_1, . . . , e_n)$ を V の基底とします。 基底 $(e_1, . . . , e_n)$ に関して、$u$ が V の自己同型で、A が $u$ の行列である場合、det($u$) $=$ det(A) となります。

($E_{ij}$) は、$\mathbf{M}_n(D)$ (II, §10, No. 3, p. 341) の行列単位の家族を表します。 D のすべての元 $\lambda$ と、$[1, n]$ の相異なる整数のすべての対 $(i, j)$ について、集合 (II, §10, No. 13, p. 361)

$$
B_{ij}(\lambda ) =I_n+\lambda E_{ij}
$$

$\mathbf{G}\mathbf{L}_n(D)$の元です。 $\lambda_1, . . . , \lambda_n$ が $D^*$ の元である場合、対角行列 diag($\lambda_1, . . . , \lambda_n$) も属するから $\mathbf{G}\mathbf{L}_n(D)$ になります。

#### 命題 3 {#alg-viii-a2-prop-3 .statement tag=00Q6}

写像 det は、関係を満たす $\mathbf{G}\mathbf{L}_n(D)$ から $D^*_{ab}$ までの一意な準同型です。

(16)デット($B_{ij}(1)$)$= 1$

$i\not=j$ と

(17) det(diag($\lambda_1, . . . , \lambda_n$)) $=\pi (\lambda_1\cdots \lambda_n)$,

$\lambda_1, . . . , \lambda_n\in D^*$用

A を $\mathbf{G}\mathbf{L}_n(D)$ の元とし、$a_1, . . . , a_n$ をその列とします。私たちは持っています

det(A) $=\omega_0(a_1, . . . , a_n)$。

さて、行列 A diag($\lambda_1, . . . , \lambda_n$) の列は $a_1\lambda_1, . . . , a_n\lambda_n$ であり、行列 AB$_{ij}(1)$ の$a_1, . . . , a_j+a_i, a_{j+1}, . . . , a_n$ です。 $\omega_0$ は $\omega_0(\varepsilon_1, . . . , \varepsilon_n) = 1$ となる $\Omega (D^n_d)$ の一意元であるため、行列式は関係を満たす一意な写像 $\varphi :\mathbf{G}\mathbf{L}_n(D)\rightarrow D^*_{ab}$ であることがわかります。

(18) $\varphi ($A 診断($\lambda_1, . . . , \lambda_n$)) $=\varphi ($A$)\pi (\lambda_1\cdots \lambda_n)$、

(19) $\varphi ($AB$_{ij}(1)) =\varphi ($A) $i\not=j$、

$$
\varphi (I_n) = 1 \tag{20}
$$

これは、まず、行列式写像が関係 (16) および (17) を満たすことを証明します。この写像が$\mathbf{G}\mathbf{L}_n(D)$から$D^*_{ab}$までの準同型であることはすでにわかっています。逆に、$\varphi$ が $\mathbf{G}\mathbf{L}_n(D)$ から $D^*_{ab}$ までの準同型で、$i\not=j$ および $\varphi$(diag($\lambda_1, . . . , \lambda_n$)) $=\pi (\lambda_1\cdots \lambda_n)$ に対して $\varphi (B_{ij}(1)) = 1$ となる場合、$\varphi$ は満たされます。 関係 (18) から (20) なので、det と等しくなります。

#### 例 1 {#alg-viii-a2-n4-exa-1 .statement tag=00Q7}

行列 $B_{ij}(\lambda )$ の列は、$\varepsilon_1, . . . , \varepsilon_j$ + $\varepsilon_i\lambda , \varepsilon_{i+1}, . . . , \varepsilon_n$ です。 VIII、p. 448 の公式 (5) までに、

(21)デット($B_{ij}(\lambda )$)$= 1$。

#### 例 2 {#alg-viii-a2-n4-exa-2 .statement tag=00Q8}

$\sigma$ を $\mathbf{N}$ の区間 $[1, n]$ の置換とし、$\varepsilon (\sigma )$ の署名を付けます。 M$(\sigma )$ を置換 $\sigma$ (II, §10, No. 7, p. 351) の行列とします。 行列 M$(\sigma )$ の列は $\varepsilon_{\sigma(1)}, . . . , \varepsilon_{\sigma(n)}$ です。 適用公式 VIII、p. 448 の (4)、したがって、次のようになります。

(22)デット(M$(\sigma )$)$=\pi (\varepsilon (\sigma ))$。

#### 例 3 {#alg-viii-a2-n4-exa-3 .statement tag=00Q9}

$n\geqslant 1$ と仮定します。 形 Δ = diag($d_1, . . . , d_n$) の可逆対角行列ごとに、Δ$B_{ij}(\lambda$)Δ$^{-1}=B_{ij}(d_i\lambda d^{-1}_j)$ が得られます。 A を $\mathbf{G}\mathbf{L}_n(D)$ の元とします。 II, §10, No. 13、p. 362、およびその前の公式の系により、A = PΔ となるように $\mathbf{G}\mathbf{L}_n(D)$ に行列 P と Δ が存在し、P は形 $B_{ij}(\lambda )$ の行列の積です。そしてその Δ は形 diag(1$, . . . ,1, d$) の対角行列です。 det(P) = 1 by 例 1 であるため、det(A) = det(Δ) $=\pi (d)$ by 命題 3 となります。

#### 例 4 {#alg-viii-a2-n4-exa-4 .statement tag=00QA}

D から $D'$ まで、$D'$ を体、$u$ を準同型とします。 移行から商、$u$ 定義する群準同型 $u_{ab}$ $D^*_{ab}$から$D^{'*}_{ab}$のとき。 $u_n$を$\mathbf{G}\mathbf{L}_n(D)$から$\mathbf{G}\mathbf{L}_n(D')$までの準同型とし、変換行列A$= (a_{ij})$を行列$(u(a_{ij}))$とします。 公式

(23) det($u_n($A)) $=u_{ab}$(det(A))

$A\in \mathbf{G}\mathbf{L}_n(D)$ は例 3 の直後に続きます。

#### 例 5 {#alg-viii-a2-n4-exa-5 .statement tag=00QB}

$\mathbf{G}\mathbf{L}_1(D) = D^*$ と命題 3 は、$\mathbf{G}\mathbf{L}_1(D)$ の $a$ に対して det($a$) $=\pi (a)$ があることを示しています。

#### 例 6 {#alg-viii-a2-n4-exa-6 .statement tag=00QC}

$n= 2$ と仮定します。 $A = \begin{pmatrix} a & b \\ c & d \end{pmatrix}$を$\mathbf{G}\mathbf{L}_2(D)$の元とします。 D の元 $a$ と $c$ は両方とも零ではありません。 A の行列式を明示的に与えます。

$a$ が零ではない場合、次のようになります。

(24) $A = \begin{pmatrix} 1 & 0 \\ ca^{-1} & 1 \end{pmatrix}\begin{pmatrix} a & 0 \\ 0 & d-ca^{-1}b \end{pmatrix}\begin{pmatrix} 1 & a^{-1}b \\ 0 & 1 \end{pmatrix}$。

従って、$ad-aca^{-1}b\not= 0$ と

(25) デット(A) $=\pi (ad-aca^{-1}b)$。

b) $a$ が零の場合、$c\not= 0$ があり、

(26) $A = \begin{pmatrix} 0 & b \\ c & d \end{pmatrix} = \begin{pmatrix} 0 & 1 \\ 1 & 0 \end{pmatrix}\begin{pmatrix} c & d \\ 0 & b \end{pmatrix}$。

従って、a) と例 2 により、$cb\not= 0$ が得られ、

(27) det(A)$=\pi (-cb)$。

#### 例 7 {#alg-viii-a2-n4-exa-7 .statement tag=00QD}

$D^o$ を D の反対の体とします。$\mathbf{M}_n(D)$ から $\mathbf{M}_n(D^o)$ までの写像 $A\mapsto^tA$ は、$^t($AB$) =^tB^tA$ を満たします。従って、$\mathbf{G}\mathbf{L}_n$(D) のすべての行列 A について、転置された行列 $^tA$ は、$\mathbf{M}_n(D^o)$ では可逆ですが、$\mathbf{M}_n(D)$ では必ずしも可逆ではありません。 例 3 から、属するが $\mathbf{G}\mathbf{L}_n$(D) であれば、$\mathbf{G}\mathbf{L}_n(D)$ の元 A と $\mathbf{G}\mathbf{L}_n(D^o)$ の $^tA$ は同じ行列式を持つことがわかります。一方、行列 $^tA$ 属するから $\mathbf{G}\mathbf{L}_n$(D) であっても、GL$_n(D)$ の行列式は A (cf. 例 6) と必ずしも等しいとは限りません。

#### 注意 1 {#alg-viii-a2-n4-rem-1 .statement tag=00QE}

V を有限次元 $n$ の体 D 以上の右ベクトル空間とします。双対空間 $V^*=$ Hom$_D(V,D)$ を、D の反対側の体 $D^o$ に対する右ベクトル空間として見ます。$u$ を V の自己同型とし、$^tu$ を D の自己同型とします$V^*$、つまり$u$の転置です。 Vの基底$(e_1, . . . , e_n)$に関して、$u$が$\mathbf{M}_n(D)$の行列Aで表される場合、自己同型$^tu$は、$\mathbf{M}_n(D^o)$に関して行列$^tA$で表されます。 基底 $V^*$ の $(e^*_1, . . . , e^*_n)$ は $(e_1, . . . , e_n)$ に二重化されます (II, §10, No. 4、p. 344、命題 3)。 例 7 までに、$^tu$ の行列式は $u$ の行列式と等しくなります。

#### 注意 2 {#alg-viii-a2-n4-rem-2 .statement tag=00QF}

小節 1 ～ 4 の結果は、D が局所環 (VIII、p. 459、練習問題 2) の場合に一般化されます。

### 5. ユニモジュラー 群

$n$を正の整数とします。 群準同型 det$:\mathbf{G}\mathbf{L}_n(D)\rightarrow D^*_{ab}$ の $\mathbf{S}\mathbf{L}_n(D)$ 核で表し、これをユニモジュラー 群または特殊線形群 (体 D が の場合、cf. III, §8, No. 9、p. 537) と呼びます可換）。

#### 定理 1 {#alg-viii-a2-thm-1 .statement tag=00QG}

$n\geqslant 2$ と仮定します。

a) $\mathbf{G}\mathbf{L}_n(D)$ の部分群 $\mathbf{S}\mathbf{L}_n(D)$ は行列 $B_{ij}(\lambda )$ によって生成されます。ここで、$i$ と $j$ は区間 $[1, n]$ と $\lambda$ の相異なる整数です。 D.

b) $n\geqslant 3$ またはカード(D) $\geqslant 3$ とします。 $\mathbf{G}\mathbf{L}_n(D)$の導来群は$\mathbf{S}\mathbf{L}_n(D)$に等しい。

c) $n\geqslant 3$ またはカード(D) $\geqslant 4$ とします。 $\mathbf{S}\mathbf{L}_n(D)$の導来群は$\mathbf{S}\mathbf{L}_n(D)$に等しい。

A) 行列 $B_{ij}(\lambda )$ によって生成された $\mathbf{G}\mathbf{L}_n(D)$ の T 部分群で表します。 VIII, p. 454 の例 1 により、det($B_{ij}(\lambda )$) $= 1$ が得られ、したがって $T\subset \mathbf{S}\mathbf{L}_n(D)$ になります。これら 2 つの群が等しいことを証明するには、loc の例 3 によって十分です。引用、形 diag(1$, . . . ,1, d$) のすべての行列が $\pi (d) = 1$ 属するから T になることを証明します。 行列 diag(1$, . . . ,1, d$) 属するから像準同型 $U\mapsto \begin{pmatrix} I_{n-2} & 0 \\ 0 & U \end{pmatrix}$ $\mathbf{G}\mathbf{L}_2(D)$ から $\mathbf{G}\mathbf{L}_n(D)$ まで。したがって、$n= 2$ の場合を考慮するだけで十分です。 $\pi$の核は$D^*$の導来群なので、$D^*$の$u, v$で$d=uvu^{-1}v^{-1}$と仮定できます。 主張は等式から導かれます

(28) $\begin{pmatrix} 1 & 0 \\ 0 & d \end{pmatrix} = \begin{pmatrix} u^{-1} & 0 \\ 0 & u \end{pmatrix}\begin{pmatrix} v^{-1} & 0 \\ 0 & v \end{pmatrix}\begin{pmatrix} vu & 0 \\ 0 & u^{-1}v^{-1} \end{pmatrix}$

そして

(29) $\begin{pmatrix} s & 0 \\ 0 & s^{-1} \end{pmatrix} = \begin{pmatrix} 1 & s \\ 0 & 1 \end{pmatrix}\begin{pmatrix} 1 & 0 \\ 1-s^{-1} & 1 \end{pmatrix}\begin{pmatrix} 1 & -1 \\ 0 & 1 \end{pmatrix}\begin{pmatrix} 1 & 0 \\ 1-s & 1 \end{pmatrix}$

$s\in D^*$の場合。

B) 構成により、$\mathbf{S}\mathbf{L}_n(D)$ は $\mathbf{G}\mathbf{L}_n(D)$ から可換群までの準同型の核なので、$\mathbf{G}\mathbf{L}_n(D)$ の含む導来群 $(\mathbf{G}\mathbf{L}_n(D),\mathbf{G}\mathbf{L}_n(D))$ になります。上記により、

$$
\mathbf{S}\mathbf{L}_n(D)\supset (\mathbf{G}\mathbf{L}_n(D),\mathbf{G}\mathbf{L}_n(D))\supset (\mathbf{S}\mathbf{L}_n(D),\mathbf{S}\mathbf{L}_n(D))
$$

c)を証明するには、行列 $B_{ij}(\lambda )$ が $\mathbf{S}\mathbf{L}_n(D)$ で交換子であることを証明すれば十分です。

$n\geqslant 3$ と仮定します。 $i,j,k$ が区間 $[1, n]$ の相異なる整数で、$\mu, \nu$ が D の元である場合、次のようになります。

$$
B_{ij}(\mu\nu ) =B_{ik}(\mu)^{-1}B_{kj}(\nu )^{-1}B_{ik}(\mu)B_{kj}(\nu ) \tag{30}
$$

$\mu= 1$ と $\nu =\lambda$ を取ると、行列 $B_{ij}(\lambda )$ は $\mathbf{S}\mathbf{L}_n(D)$ の元の交換子であることがわかります。

ここで、$n= 2$ と仮定します。 $u$と$v$をDの元と$u\not= 0$とする。 関係あります

(31) $\begin{pmatrix} 1 & v-uvu \\ 0 & 1 \end{pmatrix} = \begin{pmatrix} u & 0 \\ 0 & u^{-1} \end{pmatrix}\begin{pmatrix} 1 & -v \\ 0 & 1 \end{pmatrix}\begin{pmatrix} u^{-1} & 0 \\ 0 & u \end{pmatrix}\begin{pmatrix} 1 & v \\ 0 & 1 \end{pmatrix}$ と

(32) $\begin{pmatrix} 1 & 0 \\ v-uvu & 1 \end{pmatrix} = \begin{pmatrix} u^{-1} & 0 \\ 0 & u \end{pmatrix}\begin{pmatrix} 1 & 0 \\ -v & 1 \end{pmatrix}\begin{pmatrix} u & 0 \\ 0 & u^{-1} \end{pmatrix}\begin{pmatrix} 1 & 0 \\ v & 1 \end{pmatrix}$。

det $\begin{pmatrix} u & 0 \\ 0 & u^{-1} \end{pmatrix}$ = 1 があるため、行列 $B_{12}(v-uvu)$ と $B_{21}(v-uvu)$ は $\mathbf{S}\mathbf{L}_n(D)$ の元の交換子です。

体 D に少なくとも 4 つの元があるとします。 $\lambda$ を D の元とします。$\lambda$ が 0、1、または $-1$ に等しい場合、選ぶは $D-\{0,1,-1\}$ の任意の元 $u$ になります。それ以外の場合は、集合 $u=\lambda$。どちらの場合も、$u$ は D の非零元で、$\lambda$ と可換であり、$u^2\not= 1$ があります。 集合 $v=\lambda (1-u^2)^{-1}$。 $uv=vu$ があるため、$v-uvu=v(1-u^2) =\lambda$ になります。次に、関係 (31) と (32) から、行列 $B_{12}(\lambda )$ と $B_{21}(\lambda )$ は $\mathbf{S}\mathbf{L}_n(D)$ の交換子であることがわかります。これでc)の証明は完了です。

C) D に 3 つの元があるとき、$\mathbf{S}\mathbf{L}_2(D)$ が $\mathbf{G}\mathbf{L}_2(D)$ の導来群であることを証明する必要があります。 By A), the group $\mathbf{S}\mathbf{L}_2(D)$ is generated by the matrices $B_{12}(1) = \begin{pmatrix} 1 & 1 \\ 0 & 1 \end{pmatrix}$ and $B_{21}(1) = \begin{pmatrix} 1 & 0 \\ 1 & 1 \end{pmatrix}$, and these matrices are commutators of elements of $\mathbf{G}\mathbf{L}_2(D)$ because we have $B_{21}(1) =^tB_{12}(1)$ and

(33) $\begin{pmatrix} 1 & 1 \\ 0 & 1 \end{pmatrix} = \begin{pmatrix} -1 & 0 \\ 0 & 1 \end{pmatrix}\begin{pmatrix} 1 & 1 \\ 0 & 1 \end{pmatrix}\begin{pmatrix} -1 & 0 \\ 0 & 1 \end{pmatrix}^{-1}\begin{pmatrix} 1 & 1 \\ 0 & 1 \end{pmatrix}^{-1}$。

#### 注意 {#alg-viii-a2-n5-rem-1 .statement tag=00QH}

D が 2 つの元を持つ体である場合、$\mathbf{G}\mathbf{L}_2(D)$ は $\mathbf{S}\mathbf{L}_2$(D) に等しく、導来群が位数 3 を持つ位数 6 の群です。 D が 3 つの元を持つ体である場合、群 $\mathbf{S}\mathbf{L}_2(D)$ は位数 24 を持ち、その導来群は位数 8 を持ちます。 $n\geqslant 2$; と仮定します。前の 2 つのケースを除き、$\mathbf{S}\mathbf{L}_n(D)$ とは異なる $\mathbf{S}\mathbf{L}_n(D)$ の通常の部分群はすべて、$\mathbf{S}\mathbf{L}_n(D)$ の中心 $Z(\mathbf{S}\mathbf{L}_n(D))$ (II, §10、p. 421、練習問題 13 および 14) に含まれます。 群 $\mathbf{S}\mathbf{L}_n(D)/Z(\mathbf{S}\mathbf{L}_n(D))$ は単純です。

有限次元 $n$ の体 D を V が右ベクトル空間とします。 SL(V)で表し、Vの群、準同型det$:\mathbf{G}\mathbf{L}(V)\rightarrow D^*_{ab}$の核をユニモジュラーと呼びます。 V の基底を選択すると、$\mathbf{S}\mathbf{L}_n(D)$ でこの群を同一視するにすることができます。

V のベクトル $v$ と V に線型形式 $\varphi$ が存在し、それぞれに $\varphi (v) = 0$ と $u(x) =x+v\varphi (x)$ が成立する場合、V の自己同型 $u$ はトランスベクションであると言います。 Vの$x$。 $n\geqslant 2,u$ がトランスベクションであるとき、$u$ の行列が形 $B_{ij}(\lambda )$ であることに関して、V の基底が存在する場合に限ります。 定理 1 は次の系を意味します。

#### 系 {#alg-viii-a2-n5-cor-1 .statement tag=00RU}

V を有限次元 $n\geqslant 2$ の体 D 以上の右ベクトル空間とします。

a) $\mathbf{G}\mathbf{L}(V)$ の部分群 $\mathbf{S}\mathbf{L}(V)$ がトランスベクションによって生成されます。

b) 部分群 $\mathbf{S}\mathbf{L}(V)$ は $\mathbf{G}\mathbf{L}(V)$ 〜でない限りの導来群で、$n= 2$ があり、D には 2 つの元があります。

c) 群 $\mathbf{S}\mathbf{L}(V)$ はその導来群 〜でない限りに等しく、$n= 2$ があり、D には 2 つまたは 3 つの元があります。

### 練習問題 {#alg-viii-a2-exercises}

[練習問題付録 2](exercises/a2/)を参照してください。
