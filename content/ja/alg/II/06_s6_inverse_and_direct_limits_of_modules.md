---
book: alg
book_title: Algebra
chapter: II
chapter_title: LINEAR ALGEBRA
section: 6
section_title: Inverse and direct limits of modules
lang: ja
source: alg-i-iii
source_edition: 1998, Springer
book_pages: 284-291, 399-400
pdf_pages: 0308-0315, 0423-0424
extraction: ocr
subsections:
    - "no": 1
      title: INVERSE LIMITS OF MODULES
      page: 284
      pdf_page: 308
    - "no": 2
      title: DIRECT LIMITS OF MODULES
      page: 286
      pdf_page: 310
    - "no": 3
      title: TENSOR PRODUCT OF DIRECT LIMITS
      page: 289
      pdf_page: 313
statements: 17
exercises: 4
content_sha256: c776cb3222d07177dc51ba3a9a7b698bfe0464c625a32997dbd337c07ba423a1
translated_from: content/en/alg/II/06_s6_inverse_and_direct_limits_of_modules.md
translation_method: google
source_content_sha256: 2682c7eae62790237d64df767969f62d7aa7d61ceec717b4af26629c4a2f746a
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-eeeca2ef
glossary_version: 34
glossary_terms_sha256: 1d7f35b630e97038e28ab8bb3d8ec3721cb534927375bf79c5cb6271eeb3c835
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## § 6。 加群の逆および直接極限

この段落全体を通じて、I は空ではない予約注文集合を表し、$\alpha \leq \beta$ は I の予約注文関係を表します。 〜でない限り特に明記されていない場合、逆数と直接系にはインデックス集合 I があります。

### 1. 加群の逆極限

$(A_\alpha, \phi_{\alpha \beta})$ を環 (I, § 10, no. 1) の逆系 、$(E_\alpha, f_{\alpha \beta})$ を可換群 (加法的に書かれた) (I, § 10, no. 1) の逆系とし、それぞれの $E_\alpha$ に左があると仮定します。 $A_\alpha$モジュール構造。さらに、$\alpha \leq \beta$ $(f_{\alpha \beta}, \phi_{\alpha \beta})$ は $E_\beta$ から $E_\alpha$ (§ 1, no. 13) への二型性であり、他の語では、
$$
f_{\alpha \beta}(\lambda_\beta x_\beta) = \phi_{\alpha \beta}(\lambda_\beta) f_{\alpha \beta}(x_\beta),
$$
$x_\beta \in E_\beta$、$\lambda_\beta \in A_\beta$の場合。次に、I, § 10, no. 2 から、$E = \lim \leftarrow E_\alpha$ は $A = \lim \leftarrow A_\alpha$ に対して左加群構造を持つことがわかります。すべての $\alpha \in I$ について、$f : E \to E_\alpha$、$\phi_\alpha : A \to A_\alpha$ を標準写像とします。この場合、$(f_\alpha, \phi_\alpha)$ は E の $E_\alpha$ への二型性です。 $(E_\alpha, f_{\alpha\beta})$ は左の $A_\alpha$ モジュール * の *逆系であり、 $A$ モジュール $E$ はその * 逆極限* であると言いましょう。

$(E'_\alpha, f'_{\alpha\beta})$ を左の $A_\alpha$ 加群の他の逆数系とし、すべての $\alpha$ について、$u_\alpha : E'_\alpha \to E_\alpha$ を *$A_\alpha$ 線型* 写像とし、これらの写像は *inverse を形成します系*;この場合、$u = \lim u_\alpha$ は、$\lim E'_\alpha$ から $\lim E_\alpha$ への *$A$ 線型* 写像です。

さらに:

#### 命題 1 {#alg-ii-s6-prop-1 .statement tag=05QX}

*$(E_\alpha, f_{\alpha\beta}),\ (E'_\alpha, f'_{\alpha\beta}),\ (E''_\alpha, f''_{\alpha\beta})$ * を $A_\alpha$ モジュールの 3 つの逆数系とし、* $(u_\alpha),\ (v_\alpha)$ * 数列* となる $A_\alpha$ 線形マッピングの 2 つの逆数系とします。

$$
0 \longrightarrow E'_\alpha \xrightarrow{u_\alpha} E_\alpha \xrightarrow{v_\alpha} E''_\alpha
$$

*すべての $\alpha$ に正確です。* *次に、* $u = \lim u_\alpha,\ v = \lim v_\alpha$、*数列* と書きます

$$
0 \longrightarrow \lim E'_\alpha \xrightarrow{u} \lim E_\alpha \xrightarrow{v} \lim E''_\alpha
$$

*正確です*。

*$u_\alpha^{-1}(0) = \{0\}$ *すべての $\alpha$ について、集合理論、III, § 7, no. 2、命題 2 から* $u^{-1}(0) = \{0\}$、*したがって* $u$ *は単射です。さらに、* $u_\alpha(E'_\alpha)$ *形は、* $E_\alpha$ の部分集合の逆数系 * したがって* $u(\lim E'_\alpha) = \lim u_\alpha(E'_\alpha)$ です。 *として* $u_\alpha(E'_\alpha) = v_\alpha^{-1}(0)$ *by 仮定,* $v^{-1}(0) = \lim u_\alpha(E'_\alpha) = u(\lim E'_\alpha)$ (*集合理論*, III, § 7, no. 2, 命題 2)、*これで証明* が完成します。

#### 注意 {#alg-ii-s6-n1-rem-1 .statement tag=05QY}

(1) 命題 1 とその証明は、記法の変更を除く、任意の *群* に対して有効です。

(2) 完全系列がある場合に注意してください。

$$
0 \longrightarrow E'_\alpha \xrightarrow{u_\alpha} E_\alpha \xrightarrow{v_\alpha} E''_\alpha \longrightarrow 0
$$

*必ずしも数列というわけではありません*

$$
0 \longrightarrow \lim E'_\alpha \xrightarrow{u} \lim E_\alpha \xrightarrow{v} \lim E''_\alpha \longrightarrow 0
$$

*は正確です。他の語では、全射線形写像の逆系の逆極限は必ずしも全射ではありません* (cf. 練習問題 1)。

ここで、$A_\alpha$ が *同じ環* $A$ と、$\phi_{\alpha\beta}$ から $1_A$ に等しいと仮定します。次に、$A$ 加群のすべての逆系 $(E_\alpha, f_{\alpha\beta})$ について、$E = \lim E_\alpha$ は $A$ 加群になります。 $F$ を $A$ モジュールとし、すべての $\alpha$ について、$u_\alpha : F \to E_\alpha$ を $(u_\alpha)$ が写像の逆系となるような $A$ 線形マッピングとします。この場合、$u = \lim u_\alpha$ は、$F$ から $\lim E_\alpha$ への $A$ 線形写像です。 *逆に*、すべての $A$ 線形写像 $v : F \to \lim E_\alpha$ について、$v_\alpha = f_\alpha \circ v$ の族は $v = \lim_{\leftarrow} v_\alpha$ などの $A$ 線形写像の逆系です。一方、$\alpha \leq \beta$ 写像については次のことに注意してください。

$$
\operatorname{Hom}(1_F, f_{\alpha \beta}) = \bar{f}_{\alpha \beta}: \operatorname{Hom}_A(F, E_\beta) \to \operatorname{Hom}_A(F, E_\alpha)
$$

は、$(\operatorname{Hom}_A(F, E_\alpha), \bar{f}_{\alpha \beta})$ が $\mathbf{Z}$ モジュール * の *逆系であるような $\mathbf{Z}$ モジュール準同型です。したがって、上記の注意は、$\bar{f}_{\alpha \beta}(v_\beta) = f_{\alpha \beta} \circ v_\beta$ のように次のように表すことができます。

#### 命題 2 {#alg-ii-s6-prop-2 .statement tag=05QZ}

*$A$* モジュールのすべての逆系* $(E_\alpha, f_{\alpha \beta})$ * とすべての $A$* モジュール $F$ について、*標準写像* $u \mapsto (f_\alpha \circ u)$ * は $\mathbf{Z}$* モジュール *同型*

(2)

$$
l_F: \operatorname{Hom}_A(F, \lim_{\leftarrow} E_\alpha) \to \lim_{\leftarrow} \operatorname{Hom}_A(F, E_\alpha).
$$

#### 系 {#alg-ii-s6-n1-cor-1 .statement tag=05R0}

*すべての $A$* モジュール準同型 $v: F \to F'$ について、*

$$
\bar{v}_\alpha = \operatorname{Hom}(v, 1_{E_\alpha}): \operatorname{Hom}(F', E_\alpha) \to \operatorname{Hom}(F, E_\alpha)
$$

*形 $\mathbf{Z}$* 線形マッピング * および図式* の逆系

(3)

$$
\begin{array}{ccc}
\operatorname{Hom}(F', \lim_{\leftarrow} E_\alpha) & \xrightarrow{l_{F'}} & \lim_{\leftarrow} \operatorname{Hom}(F', E_\alpha) \\
\downarrow \operatorname{Hom}(v, 1_E) & & \downarrow \lim_{\leftarrow} \bar{v}_\alpha \\
\operatorname{Hom}(F, \lim_{\leftarrow} E_\alpha) & \xrightarrow{l_F} & \lim_{\leftarrow} \operatorname{Hom}(F, E_\alpha)
\end{array}
$$

*可換です*。

すべての $u \in \operatorname{Hom}(F', \lim_{\leftarrow} E_\alpha)$、$l_F(u \circ v) = (f_\alpha \circ u \circ v)$ による図式の定義と可換性は、定義の直後に続きます。

### 2. 直接極限/加群

※以降Iは右向きとする。

$(A_\alpha, \phi_{\beta \alpha})$ を環 (I, § 10, no. 3) の直接系、可換群 (加法的に書かれた) (I, § 10, no. 3) の $(E_\alpha, f_{\beta \alpha})$ 直接系とし、それぞれの $E_\alpha$ が *left $A_\alpha$* モジュール構造を持つと仮定します。さらに、$\alpha \leq \beta$ に対して、$(f_{\beta \alpha}, \phi_{\beta \alpha})$ は $E_\alpha$ から $E_\beta$ (§ 1, no. 13) への *二型性* であり、他の語では、

(4)

$$
f_{\beta \alpha}(\lambda_\alpha x_\alpha) = \phi_{\beta \alpha}(\lambda_\alpha) f_{\beta \alpha}(x_\alpha)
$$

$x_\alpha \in E_\alpha, \lambda_\alpha \in A_\alpha$の場合;その場合、$E = \lim_{\longrightarrow} E_\alpha$ は $A = \lim_{\longrightarrow} A_\alpha$ (I, § 10, no. 4) に対して *左加群* 構造を持ちます。すべての $\alpha \in I$ について、$f_\alpha: E_\alpha \to E, \phi_\alpha: A_\alpha \to A$ を標準写像とします。この場合、$(f_\alpha, \phi_\alpha)$ は $E_\alpha$ から $E$ への *二型性* です。 $(E_\alpha, f_{\beta \alpha})$ は左の $A_\alpha$* モジュールの *直接系であり、$A$* モジュール $E$ はその *直接の極限* であるとします。

$(E'_\alpha, f'_{\beta \alpha})$ を左の $A_\alpha$* モジュールの他の直接系とし、すべての $\alpha$ について、$u_\alpha : E'_\alpha \to E_\alpha$ を $A_\alpha$ 線形マッピングとし、これらの写像は直接系を形成します。この場合、$u = \lim \to u_\alpha$ は、$\lim \to E'_\alpha$ から $\lim \to E_\alpha$ への $A$ 線形マッピングです。

さらに：

#### 命題 3 {#alg-ii-s6-prop-3 .statement tag=05R1}

* $(E_\alpha, f_{\beta \alpha}), (E'_\alpha, f'_{\beta \alpha}), (E''_\alpha, f''_{\beta \alpha})$ * を 3 つの直接系の* $A_\alpha$* モジュールと* $(u_\alpha), (v_\alpha)$ * 2 つの直接系の* $A_\alpha$* の線形マッピングを数列* とします。

$$
E'_\alpha \xrightarrow{u_\alpha} E_\alpha \xrightarrow{v_\alpha} E''_\alpha
$$

*すべてに正確です* $\alpha$。 *その後、* $u = \lim \to u_\alpha, v = \lim \to v_\alpha$、*数列* と書きます

$$
\lim \to E'_\alpha \xrightarrow{u} \lim \to E_\alpha \xrightarrow{v} \lim \to E''_\alpha
$$

*正確です。*

$u(\lim \to E'_\alpha) = \lim \to u_\alpha(E'_\alpha)$ * および* $v^{-1}(0) = \lim \to v_\alpha^{-1}(0)$ * (集合理論、III, § 7, no. 6、系から命題 7)。*

大まかに言えば、命題 3 は、*移行を直接極限にすると正確性が保たれる* というというによって表現することもできます。

#### 命題 4 {#alg-ii-s6-prop-4 .statement tag=05R2}

*$(E_\alpha, f_{\beta \alpha})$ * を * $A_\alpha$* モジュールの直接系とし、$E = \lim \to E_\alpha$ * その直接の極限と* $\phi_\alpha : A_\alpha \to A$ * および* $f_\alpha : E_\alpha \to E$ * すべての標準写像* $\alpha \in I$ とします。 *すべて* $\alpha \in I$、$S_\alpha$ * が * $E_\alpha$ の生成する系である場合、 * $S = \bigcup_{\alpha \in I} f_\alpha(S_\alpha)$ * は * $E$ の生成する系です。

すべての $x \in E$ *は形* $f_\alpha(x_\alpha)$ *一部* $\alpha \in I$ *および一部* $x_\alpha \in E_\alpha$ *そして仮定* $x = \sum_i \lambda^{(i)}_\alpha y^{(i)}_\alpha$、*ここで* $\lambda^{(i)}_\alpha \in A_\alpha$ *および* $y^{(i)}_\alpha \in S_\alpha$; *書き込み* $\lambda^{(i)} = \phi_\alpha(\lambda^{(i)}_\alpha)$、$y^{(i)} = f_\alpha(y^{(i)}_\alpha)$、*取得* $x = \sum_i \lambda^{(i)} y^{(i)}$。

#### 命題 5 {#alg-ii-s6-prop-5 .statement tag=05R3}

*仮説と命題 4 の記法を使用して、すべて* $\alpha \in I$、$E_\alpha$ * は家族の直和 * 部分加群の $(M^\lambda_\alpha)_{\alpha \in L}$ (インデックス付け集合* $L$ * から独立している*) $\alpha$) *そしてそれ* $f_{\beta \alpha}(M^\lambda_\alpha) \subset M^\lambda_\alpha$ *のために* $\alpha \leq \beta$ *そしてすべてのために* $\lambda \in L$。 *すると* $E$ *は部分加群* $M^\lambda = \lim \to M^\lambda_\alpha$ $(\lambda \in L)$ の直和です。

命題 4 から、$E$ は $M^\lambda$ の和であることがわかります。 $(y^\lambda)_{\lambda \in L}$ *そのような家族* $y^\lambda \in M^\lambda$ *すべての人に* $\lambda \in L$ *そしてその支援は有限であり、* $\sum_\lambda y^\lambda = 0$ と仮定します。 *集合理論、III, § 7, no. 5、補題 1 のおかげで、* $\alpha \in I$ * と家族* $(x^\lambda_\alpha)_{\alpha \in L}$ * 有限台からなるの元の * $E_\alpha$ * が存在します* $x^\lambda_\alpha \in M^\lambda_\alpha$ *そして* $y^\lambda = f_\alpha(x^\lambda_\alpha)$ *すべて* $\lambda \in L$。 *関係* $f_\alpha \left( \sum_{\lambda \in L} x^\lambda_\alpha \right) = 0$ ** $\beta \geq \alpha$ *そのような* $f_{\beta \alpha} \left( \sum_{\lambda \in L} x^\lambda_\alpha \right) = 0$ *(集合理論, III, § 7, no. 5, 補題 1) の存在を暗示します。これは $\sum_{\lambda \in L} x_\beta^\lambda = 0$ と記述できます。ここで、$x_\beta^\lambda = f_{\beta \alpha}(x_\alpha^\lambda) \in M_\beta^\lambda$ 仮定著;したがって、すべての $\lambda \in L$ に対して $x_\beta^\lambda = 0$、したがってすべての $\lambda \in L$ に対して $y^\lambda = f_\beta(x_\beta^\lambda) = 0$ となり、$M^\lambda$ の和が直接であることが証明されます。

#### 系 {#alg-ii-s6-n2-cor-1 .statement tag=05R4}

*$(P_\alpha)$ *を* $E_\alpha$の部分集合の直接系にして*そして* $P = \lim \overrightarrow{P_\alpha}$とします。 *すべて* $\alpha \in I$、$P_\alpha$ *が* $E_\alpha$の無料の部分集合 (それぞれ基底) である場合、*そのとき* $P$ *は* $E$の無料の部分集合 (それぞれ基底) です。

2 番目の主張は、最初の命題 4 の直後に続きます。 したがって、$P_\alpha$ がフリーであれば、$P$ の個別の元のすべての部分集合 $\{ y^{(i)} \}_{1 \leq i \leq n}$ からなるがフリーであることを証明するのに十分です。 $1 \leq i \leq n$ に対して $y^{(i)} = f_\alpha(x_\alpha^{(i)})$ となるような $\alpha \in I$ と元 $x_\alpha^{(i)} \in P_\alpha$ が存在します (*集合理論*, III, § 7, no. 5, 補題 1)。 $\sum_i \lambda^{(i)} y^{(i)} = 0$ の場合、$1 \leq i \leq n$ に対して $\lambda^{(i)} = \phi_\alpha(\lambda_\alpha^{(i)})$、したがって $f_\alpha \left( \sum_i \lambda_\beta^{(i)} x_\beta^{(i)} \right) = 0$ であると想定できます。これは、一部の $\beta \geq \alpha$ に対して $\sum_i \lambda_\beta^{(i)} x_\beta^{(i)} = 0$ を意味します。ここで、$\lambda_\beta^{(i)} = \phi_{\beta \alpha}(\lambda_\alpha^{(i)})$、$x_\beta^{(i)} = f_{\beta \alpha}(x_\alpha^{(i)})$、および $x_\beta^{(i)}$ 属するから $P_\beta$ は、$y^{(i)} = f_\beta(x_\beta^{(i)})$ 以降は区別されます。次に、$1 \leq i \leq n$、よっての場合は $\lambda_\beta^{(i)} = 0$
$$
\lambda^{(i)} = \phi_\beta(\lambda_\beta^{(i)}) = 0
$$
$1 \leq i \leq n$の場合。

ここで、すべての環 $A_\alpha$ が *同じ環* $A$ と $\phi_{\beta \alpha}$ から $1_A$ に等しいと仮定します。したがって、$A$ モジュールの直接系 $(E_\alpha, f_{\beta \alpha})$ ごとに、$E = \lim \overrightarrow{E_\alpha}$ は $A$ モジュールになります。 $F$ を $A$ モジュールとし、すべての $\alpha$ について、$u_\alpha : E_\alpha \to F$ を $(u_\alpha)$ が写像の直接系となるような $A$ 線形マッピングとします。この場合、$u = \lim \overrightarrow{u_\alpha}$ は、$E$ から $F$ への $A$ 線形写像です。 *逆に*、すべての $A$ 線形写像 $v : \lim \overrightarrow{E_\alpha} \to F$ について、$v_\alpha = v \circ f_\alpha$ の族は、$v = \lim \overrightarrow{v_\alpha}$ のような $A$ 線形写像の直接系になります。一方、$\alpha \leq \beta$ 写像については次のことに注意してください。
$$
\operatorname{Hom}(f_{\beta \alpha}, 1_F) = \bar{f}_{\alpha \beta} : \operatorname{Hom}_A(E_\beta, F) \to \operatorname{Hom}_A(E_\alpha, F)
$$
は $\mathbf{Z}$-モジュール準同型であり、$(\operatorname{Hom}_A(E_\alpha, F), \bar{f}_{\alpha \beta})$ は $\mathbf{Z}$*-モジュール* の *逆系です。 $\bar{f}_{\alpha \beta}(v_\beta) = v_\beta \circ f_{\beta \alpha}$ とすると、上記の注意は次のように表すことができます。

#### 命題 6 {#alg-ii-s6-prop-6 .statement tag=05R5}

*すべての直接系* $(E_\alpha, f_{\beta \alpha})$ * の* $A$* モジュールおよびすべての* $A$*-モジュール* $F$、*標準写像* $u \mapsto (u \circ f_\alpha)$ * は* $\mathbf{Z}$* モジュール同型*
$$
d_F : \operatorname{Hom}_A(\lim \overrightarrow{E_\alpha}, F) \to \lim \leftarrow \operatorname{Hom}_A(E_\alpha, F).
$$

#### 系 1 {#alg-ii-s6-prop-6-cor-1 .statement tag=05R6}

*すべての* $A$*-モジュール準同型* $v : F \to F'$、*その*
$$
\bar{v}_\alpha = \operatorname{Hom}(1_{E_\alpha}, v) : \operatorname{Hom}(E_\alpha, F) \to \operatorname{Hom}(E_\alpha, F')
$$

形 $\mathbf{Z}$ 線形マッピングの逆系と図式

$$
\begin{array}{ccc}
\operatorname{Hom}(\lim E_\alpha, F) & \xrightarrow{d_F} & \lim \operatorname{Hom}(E_\alpha, F) \\
\downarrow \operatorname{Hom}(1_E, v) & & \downarrow \lim \overline{v}_\alpha \\
\operatorname{Hom}(\lim E_\alpha, F') & \xrightarrow{d_{F'}} & \lim \operatorname{Hom}(E_\alpha, F')
\end{array}
$$

可換です。

すべての $u \in \operatorname{Hom}(\lim E_\alpha, F)$、$d_{F'}(v \circ u) = (v \circ u \circ f_\alpha)$ については、図式の定義および可換性によって (6)、定義からすぐに続きます。

#### 系 2 {#alg-ii-s6-prop-6-cor-2 .statement tag=05R7}

*もし* $(E_\alpha, f_{\beta \alpha})$ *が左* $A$*モジュールと* $E = \lim \longrightarrow E_\alpha$の直接系である場合、$(E_\alpha^*, t f_{\beta \alpha})$ *は右* $A$*モジュールの逆系であり、* $\lim \leftarrow E_\alpha^*$ *は標準的に* $E^*$と同型です。

#### 注意 {#alg-ii-s6-n2-rem-1 .statement tag=05R8}

Let $E$ be an $A$*-module and* $(M_\alpha)_{\alpha \in I}$ *an increasing family of submodules of* $E$ *such that* $E$ *is the union of the* $M_\alpha$; if $j_{\beta \alpha}: M_\alpha \to M_\beta$ (for $\alpha \leq \beta$) and $j_\alpha: M_\alpha \to E$ *are the canonical injections, it is immediate that* $j = \lim \longrightarrow j_\alpha$ *is an isomorphism of* $\lim \longrightarrow M_\alpha$ *onto* $E$ *(Set Theory, III, § 7, no. 6, Remark 1)*. 特に、すべての $A$* モジュールは、その *有限生成* 部分加群の右有向族の直接の極限です。

### 3. テンソル積の直接極限

$(A_\alpha, \rho_{\beta \alpha})$ を環の直接系とし、$(E_\alpha, f_{\beta \alpha})$ (それぞれ $(F_\alpha, g_{\beta \alpha})$) を右 (それぞれ左) $A_\alpha$* モジュールの直接系とします。 $\alpha \leq \beta$ には、$\mathbf{Z}$* モジュール準同型* があります

$$
f_{\beta \alpha} \otimes g_{\beta \alpha}: E_\alpha \otimes_{A_\alpha} F_\alpha \to (E_\beta)_{[A_\alpha]} \otimes_{A_\alpha} (F_\beta)_{[A_\alpha]}
$$

一方、正規の $\mathbf{Z}$* モジュール準同型* もあります

$$
(E_\beta)_{[A_\alpha]} \otimes_{A_\alpha} (F_\beta)_{[A_\alpha]} \to E_\beta \otimes_{A_\beta} F_\beta
$$

対応する ～ 環準同型 $\rho_{\beta \alpha}$ ($§ 3$、no. 3、命題 2); よって合成により、$\mathbf{Z}$* モジュール準同型* が得られます

$$
h_{\beta \alpha}: E_\alpha \otimes_{A_\alpha} F_\alpha \to E_\beta \otimes_{A_\beta} F_\beta
$$

写像テンソル積 $x_\alpha \otimes y_\alpha$ から $f_{\beta \alpha}(x_\alpha) \otimes g_{\beta \alpha}(y_\alpha)$ までです。明らかに

$$
(E_\alpha \otimes_{A_\alpha} F_\alpha, h_{\beta \alpha})
$$

は $\mathbf{Z}$* モジュールの *直接系* です。 * $A = \lim \longrightarrow A_\alpha$、$E = \lim \longrightarrow E_\alpha$、$F = \lim \longrightarrow F_\alpha$ *そして*

$\rho_\alpha : A_\alpha \to A, f_\alpha : E_\alpha \to E, g_\alpha : F_\alpha \to F$を標準写像とします。上記のように、写像テンソル積 $x_\alpha \otimes y_\alpha$ から $f_\alpha(x_\alpha) \otimes g_\alpha(y_\alpha)$ までの $\mathbf{Z}$ 線形写像 $\pi_\alpha : E_\alpha \otimes_{A_\alpha} F_\alpha \to E \otimes_A F$ が定義されており、これら写像形直接系が明らかとなります。したがって、$\mathbf{Z}$-線形マッピングが得られます。
$$
\pi = \lim \pi_\alpha : \lim (E_\alpha \otimes_{A_\alpha} F_\alpha) \to E \otimes_A F.
$$

#### 命題 7 {#alg-ii-s6-prop-7 .statement tag=05R9}

*$\mathbf{Z}$-線形写像 (7) は全単射です。*

私たちは集合 $P = \lim (E_\alpha \otimes_{A_\alpha} F_\alpha)$ で、すべての $\alpha \in I$ について、$h_\alpha : E_\alpha \otimes_{A_\alpha} F_\alpha \to P$ を標準写像とします。一方、$\alpha \in I$ については、次のようにします。
$$
t_\alpha : E_\alpha \times F_\alpha \to E_\alpha \otimes_{A_\alpha} F_\alpha
$$
正準 $\mathbf{Z}$-双線形写像であること。 $\alpha \leq \beta$の場合、
$$
t_\beta(f_{\beta \alpha}(x_\alpha), g_{\beta \alpha}(y_\alpha)) = f_{\beta \alpha}(x_\alpha) \otimes g_{\beta \alpha}(y_\alpha) = h_{\beta \alpha}(t_\alpha(x_\alpha, y_\alpha))
$$
したがって、$(t_\alpha)$ は写像の直接系です。 $\lim (E_\alpha \times F_\alpha)$ を $E \times F$ (*集合理論*, III, § 7, no. 7, 命題 10) と正準的に識別すると、次のように写像 $t = \lim t_\alpha : E \times F \to P$ が導出されます。
$$
t(f_\alpha(x_\alpha), g_\alpha(y_\alpha)) = h_\alpha(t_\alpha(x_\alpha, y_\alpha)) = h_\alpha(x_\alpha \otimes y_\alpha).
$$
*集合理論*、III, § 7, no. 5、補題 1 を考慮すると、$t$ が $\mathbf{Z}$ 双線形であることがすぐにわかります。さらに、$x \in E, y \in F, \lambda \in A$ については、$x = f_\alpha(x_\alpha), y = g_\alpha(y_\alpha), \lambda = \rho_\alpha(\lambda_\alpha)$ と $\lambda_\alpha \in A_\alpha, x_\alpha \in E_\alpha, y_\alpha \in F_\alpha$ (*集合理論*, III, § 3, no. 7, 補題 1) のような $\alpha \in I$ が存在します。 よって
$$
t(x \lambda, y) = h_\alpha((x_\alpha \lambda_\alpha) \otimes y_\alpha) = h_\alpha(x_\alpha \otimes (\lambda_\alpha y_\alpha)) = t(x, \lambda y).
$$
したがって、$\pi'(x \otimes y) = t(x, y)$ (§ 3, no. 1, 命題 1) のような $\mathbf{Z}$ 線形写像 $\pi' : E \otimes_A F \to P$ が 1 つだけ存在します。さらに、定義までに
$$
\pi'(\pi(h_\alpha(x_\alpha \otimes y_\alpha))) = \pi'(f_\alpha(x_\alpha) \otimes g_\alpha(y_\alpha)) = h_\alpha(x_\alpha \otimes y_\alpha)
$$
$$
\pi(\pi'(f_\alpha(x_\alpha) \otimes g_\alpha(y_\alpha))) = \pi(h_\alpha(x_\alpha \otimes y_\alpha)) = f_\alpha(x_\alpha) \otimes g_\alpha(y_\alpha)
$$
そして、形 $f_\alpha(x_\alpha) \otimes g_\alpha(y_\alpha)$ (それぞれ $h_\alpha(x_\alpha \otimes y_\alpha)$) 生成するの元として、$\mathbf{Z}$ モジュール $E \otimes_A F$ (それぞれ $P$)、$\pi' \circ \pi$ および $\pi \circ \pi'$ は次のようになります。 恒等写像。

大まかに言えば、命題 7 は、*テンソル積が​​直接極限* と可換であるというによって表現される可能性があり、通常、(7) の両側は同型 $\pi$ によって識別されます。

#### 系 1 {#alg-ii-s6-prop-7-cor-1 .statement tag=05RA}

*$(E'_\alpha, f'_{\beta \alpha})$ (それぞれ $(F'_\alpha, g'_{\alpha \beta})$) *右* の他の直接系 (*左*) *$A_\alpha$*-*加群とします。すべて* $\alpha \in I$、*させて* $u_\alpha : E_\alpha \to E'_\alpha$ (それぞれ $v_\alpha : F_\alpha \to F'_\alpha$) *なる*

$(u_\alpha)$ (それぞれ $(v_\alpha)$) が直接系となるような $A_\alpha$ 線形マッピング。すると、$(u_\alpha \oplus v_\alpha)$ は $\mathbf{Z}$ 線形写像の直接系であり、図式

$$
\begin{array}{ccc}
\lim(E_\alpha \otimes_{A_\alpha} F_\alpha) & \longrightarrow & (\lim E_\alpha) \otimes_A (\lim F_\alpha) \\
\downarrow & & \downarrow \\
\lim(u_\alpha \otimes v_\alpha) & & (\lim u_\alpha) \otimes (\lim v_\alpha) \\
\lim(E'_\alpha \otimes_{A_\alpha} F'_\alpha) & \longrightarrow & (\lim E'_\alpha) \otimes_A (\lim F'_\alpha)
\end{array}
$$

可換です。

検証は明らかです。

$(A'_\alpha, \rho'_{\beta\alpha})$ を環の他の直接系とし、各 $E_\alpha$ が $(A'_\alpha, A_\alpha)$ バイモジュールであり、$f_{\beta\alpha}$ が $\alpha \leq \beta$ に対して $(A'_\alpha, A_\alpha)$ 線形であると仮定します。次に、$A' = \lim A'_\alpha$ と書くと、同型 (7) は、系 1 のおかげで、両側の左側の $A'$ モジュール構造に関して *線型* になります。これは、任意のマルチモジュールにすぐに一般化できます。

特に、$A_\alpha$ が *可換* である場合、$A = \lim A_\alpha$ は可換で、同型 (7) は *A-加群同型* です。

#### 系 2 {#alg-ii-s6-prop-7-cor-2 .statement tag=05RB}

*$(E_\alpha, f_{\beta\alpha})$ * を右側* $A_\alpha$* モジュールの直接系とし、* $E'_\alpha = E_\alpha \otimes_{A_\alpha} A$ * をスカラーの環を * $A = \lim A_\alpha$ * 標準準同型* $\rho_\alpha : A_\alpha \to A$ に拡張することで得られる* $A$* モジュールとします。 *その後* $(E'_\alpha, f_{\beta\alpha} \otimes 1_A)$ *は右側* $A$*モジュールの直接系であり、*その直接の極限は標準的に$\lim E_\alpha$と同型です。

$F_\alpha$ 環 $A$ を $\rho_\alpha$ によって $(A_\alpha, A)$ バイモジュールとみなして命題を適用する 7 とすれば十分です。

#### 系 3 {#alg-ii-s6-prop-7-cor-3 .statement tag=05RC}

* $A$ * を環とし、* $(E_\alpha, f_{\beta\alpha})$ * 直接系を右* $A$* モジュール、* $F$ * 左* $A$* モジュールとします。 *その後、* $\mathbf{Z}$* モジュール* $\lim (E_\alpha \otimes_A F)$ * と* $(\lim E_\alpha) \otimes_A F$ * は標準的に同型* になります。

命題 7 のすべての $\alpha \in I$ に対して、$A_\alpha = A$ と $F_\alpha = F$ を取るだけで十分です。

特に、$\rho : A \to B$ が環準同型である場合、$\lim \rho^*(E_\alpha)$ と $\rho^*(\lim E_\alpha)$ は標準的に同型です。

#### 系 4 {#alg-ii-s6-prop-7-cor-4 .statement tag=05RD}

*$M$ *右側* $A$*-モジュール、$N$ *左側* $A$*-モジュール、$(x_i)_{1 \leq i \leq n}$ *元の*のファミリー $M$、$(y_i)_{1 \leq i \leq n}$ **の元のファミリー$N$、*そのような* $\sum_i (x_i \otimes y_i) = 0$ *で* $M \otimes_A N$。 *その後、有限生成された部分加群* $M_1$ *(それぞれ $N_1$) of* $M$ *(それぞれ $N$) 含む the* $x_i$ *(それぞれ the* $y_i$) *そしてそのような* $\sum_i (x_i \otimes y_i) = 0$ *中* $M_1 \otimes_A N_1$。

$M$ (それぞれ $N$) は、その有限生成された部分加群含む $x_i$ (それぞれ $y_i$) の右有向族の直接の極限と標準的に識別されており、*集合を適用するだけで十分です。 理論、III, § 7, no. 5、補題 1.*

### 練習問題 {#alg-ii-s6-exercises}

[§ 6 に対して練習問題](exercises/s6/)を参照してください。
