---
book: evt
book_title: Topological Vector Spaces
chapter: IV
chapter_title: DUALITY IN TOPOLOGICAL VECTOR SPACES
section: 3
section_title: Dual of a Fréchet space
lang: ja
source: evt-i-v
book_pages: TVS IV.21-TVS IV.26, TVS IV.57-TVS IV.61
pdf_pages: 0203-0208, 0239-0243
extraction: ocr
subsections:
    - "no": 1
      title: Semi-barrelled spaces
      page: 21
      pdf_page: 203
    - "no": 2
      title: Dual of a locally convex metrizable space
      page: 22
      pdf_page: 204
    - "no": 3
      title: Bidual of a locally convex metrizable space
      page: 23
      pdf_page: 205
    - "no": 4
      title: Dual of a reflexive Fréchet space
      page: 23
      pdf_page: 205
    - "no": 5
      title: The topology of compact convergence on the dual of a Fréchet space
      page: 24
      pdf_page: 206
    - "no": 6
      title: Separately continuous bilinear mappings
      page: 26
      pdf_page: 208
statements: 15
exercises: 18
content_sha256: 8e949f2c65edf140ff4048b2307a6f6681a151e880a210d9b3281efe3c1e2930
translated_from: content/en/evt/IV/03_s3_dual_of_a_frechet_space.md
translation_method: google
source_content_sha256: bb0b04778ba87067d91908af5a1b8236b1f89fcb725229b0b2dd6d0e99a65350
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-b071ad41
glossary_version: 34
glossary_terms_sha256: c60793908a269d6384ec148ade612fa24c4db1335846ffff03df8556c2d1e4e8
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## § 3。フレシェのデュアル空間

### 1. セミバレル空間

#### 命題 1 {#evt-iv-s3-prop-1 .statement tag=07TU}

— E を局所凸型空間とします。次の条件は同等です。

(i) U を E のすべての有界部分集合を吸収する E の部分集合とし、E の 0 の凸、平衡、閉近傍の数列の共通部分とします。すると、U は E の 0 の近傍となります。

(ii) すべての局所凸空間 F について、等連続部分集合の可算族の和集合である $\mathscr{L}_b(E; F)$ のすべての有界部分集合は等連続です。

(iii) E の強い双対 $E'_b$ では、等連続部分集合の可算族の和集合であるすべての有界部分集合は等連続です。

(iii) が (ii) の特殊なケースであることは明らかです。

(i) $\Rightarrow$ (ii) : H を $\mathscr{L}_b(E; F)$ の有界部分集合とし、$(H_n)$ を $H = \bigcup H_n$ となるような $\mathscr{L}_b(E; F)$ の等連続部分集合の数列とする。 V を F で 0 の凸、平衡、閉じた近傍とします。すべての $n$ について、集合 $W_n = \bigcap_{u \in H_n} u^{-1}(V)$ は、$H_n$ が等連続であるため、E で 0 の凸、平衡で閉じた近傍となります。 集合 $W = \bigcap_{u \in H} u^{-1}(V)$ は、H が $\mathscr{L}_b(E; F)$ (III, p. 22) で制限されており、$W = \bigcap_n W_n$ があるため、E のすべての制限された部分集合を吸収します。 E が (i) を満たす場合、E において集合 W は 0 の近傍であるため、H は等連続です。

(iii) $\Rightarrow$ (i) : $(U_n)$ を E の 0 の凸、平衡、閉じた近傍の数列とします。集合 $U = \bigcap_n U_n$ は E のすべての有界部分集合を吸収するため、その極性は $U^\circ$ であると仮定します。は$E'_b$で区切られています。すると、集合 $B = \bigcup_n U_n^\circ$ は $U^\circ$ に含まれるため、$E'_b$ に境界されます。 E が (iii) を満たす場合、集合 B は $E'$ で等連続です。従って、E の B の極 $B^\circ = \bigcap_n (U_n^\circ)^\circ = \bigcap_n U_n = U$ は、E の 0 の近傍です。

#### 定義 1 {#evt-iv-s3-def-1 .statement tag=07TV}

— 局所的に凸状の空間 E は、プロップの同等の条件を満たす場合、セミバレルであると言われます。 1.

すべてのバレル空間はセミバレルです。これは、すべてのボーンロジカル空間 (III、p. 22、提案 10) にも当てはまります。

### 2. 局所的に凸な metrizable の双対空間

#### 命題 2 {#evt-iv-s3-prop-2 .statement tag=07TW}

— E を局所的に凸な metrizable 空間とし、F をその強い双対とする。 空間 F は完全でセミバレルであり、以下の条件を満たします。
(DB) F の有界部分集合の数列 $(A_n)_{n \in \mathbf{N}}$ が存在し、F の有界部分集合はすべて $A_n$ の 1 つに含まれます。

空間 E はボーンロジカル (III, p. 12, prop. 2) であるため、その強い双対は完全です (III, p. 23, cor. 1)。

$(V_n)_{n \in \mathbf{N}}$ を E の 0 の近傍の減少列とし、E 含むの 0 のすべての近傍が $V_n$ の 1 つになるようにします。 $A_n$ を F の $V_n$ の極とします。E はボーンロジーであるため、F のすべての境界のある部分集合は等連続であり (III、p. 22、提案 10)、従って $A_n$ の 1 つに含まれます。その他の語、空間 F は条件 (DB) を満たします。

ここで、F がセミバレルであることを示します。 $(U_n)_{n \in \mathbf{N}}$ を F の 0 の凸で平衡した閉じた近傍の数列とします。 集合 $U = \bigcap_n U_n$ が F のすべての境界のある部分集合を吸収すると仮定します。 U が F の 0 の近傍であることを証明します。 構成する、帰納法による整数 $n \geqslant 0$、実数 $\lambda_n > 0$ と、F の 0 の凸バランス近傍 $W_n$、$\sigma(F, E)$ と満たすはクローズされています以下関係

(1)
$$
\lambda_n A_n \subset \frac{1}{2} U \cap \left( \bigcap_{0 \leq i < n} W_i \right)
$$

(2)
$$
\bigcup_{0 \leq i \leq n} \lambda_i A_i \subset W_n \subset U_n .
$$

数 $\lambda_i$ と集合 $W_i$ が $0 \leq i < n$ に対して構築されたとします。 仮定までに、集合 U は F の有界な部分集合を吸収します。さらに、$0 \leq i < n$ の場合、$W_i$ は F の 0 の近傍であるため、F の有界な部分集合を吸収します。従って、数 $\lambda_n > 0$ 満たす (1) を見つけることができます。 C は、$\bigcup_{0 \leq i \leq n} \lambda_i A_i$ の $\sigma(F, E)$ の閉じた凸型バランスエンベロープを示します。 集合 C は等連続であるため、$\sigma(F, E)$ (III、p. 17、cor. 2) に対してコンパクトです。 $U_n$ は F の 0 の近傍であるため、$B^\circ \subset \frac{1}{2} U_n$ となるような E の有界な部分集合 B が存在します。 $W_n = C + B^\circ$を入れてください。 $B^\circ$ は F の 0 の近傍であるため、$W_n$ は F の 0 の凸でバランスの取れた近傍であることがわかります。 加法では、C はコンパクトで、$B^\circ$ は $\sigma(F, E)$ に対して閉じています。コルによる。 GTの1、III, § 4, No. 1、$W_n$は$\sigma(F, E)$のため閉店です。最後に、$C \subset \frac{1}{2} U \subset \frac{1}{2} U_n$ と $B^\circ \subset \frac{1}{2} U_n$ があり、$U_n$ が凸であるため、$W_n \subset U_n$ になります。こうして(2)が成立しました。

$W = \bigcap_n W_n$を入れてから、$W \subset U$を入れます。 (1) と (2) により、$\mathbf{N}$ のすべての $i$ と $j$ に対して $\lambda_i A_i \subset W_j$ が得られるため、すべての $i \in \mathbf{N}$ に対して $\lambda_i A_i \subset W$ が得られます。特にWは吸収性があるので$\sigma(F, E)$用のバレルです。 IV、p. 4の注意 3により、WはFの0の近傍です。なおさら、UはFの0の近傍で、Fはセミバレルです。

次の系拡大するは、Banach-Steinhaus 定理から Fréchet 空間 (*cf.* III、p. 25、cor. 2) のデュアルです。

#### 系 {#evt-iv-s3-n2-cor-1 .statement tag=07TX}

— G を局所凸ハウスドルフ空間とし、$(u_n)$ を F から G への線形写像の数列とし、単純に F から G への写像 u に収束します。その場合、u は連続であり、数列 $(u_n)$ はすべてのプリコンパクトで一様に u に収束します。 Fの部分集合

F が完全なので、単純収束の位相に制限されるすべての $u_n$ の集合は、$\mathscr{L}_b(F; G)$ (III, p. 27, cor. 1) に制限されます。 空間 F は半バレル (prop. 2) であるため、$\mathscr{L}_b(F; G)$ のすべての可算で有界な部分集合は、prop によって等連続です。 IV、p. 21 の 1 つ。したがって、$u_n$の集合は等連続であり、III、p. 18、系から系が続きます。

### 3. 局所的に凸なメトリザブルのバイデュアル空間

#### 命題 3 {#evt-iv-s3-prop-3 .statement tag=07TY}

— E を局所的に凸な metrizable 空間、$E'_b$ の強力な双対、G を Fréchet 空間とします。 空間 $\mathscr{L}_b(E'_b ; G)$ はフレシェ空間です。

プロップにより。 2 (IV, p. 22) では、$E'_b$ の有界部分集合の数列 $(A_n)$ が存在し、$E'_b$ の有界部分集合はすべて $A_n$ の 1 つに含まれます。 $(V_n)$ を G の 0 の近傍の可算基音系とする。 $H_{mn}$ を $E'_b$ から G に$u(A_m) \subset V_n$ になるように線形写像 $u$ の集合とする。この場合、$(H_{mn})$ は $\mathscr{L}_b(E'_b ; G)$ の 0 の近傍の基本的な系であり、後者の空間は計量化可能です。

$\mathscr{L}_b(E'_b ; G)$ が完全であることを示すには、この空間内のすべての Cauchy 数列 $(u_n)$ が収束していることを証明するだけで十分です。 G が完全なので、$(u_n)$ が単純に u に収束するような線形写像 $u : E'_b \to G$ が存在します。 IV、p. 23、系までに、$u \in \mathscr{L}_b(E'_b ; G)$になります。その後、プロップから続きます。 GTの5、X, § 1, No. 5、その$(u_n)$は$\mathscr{L}_b(E'_b ; G)$でuに収束します。

#### 系 {#evt-iv-s3-n3-cor-1 .statement tag=07TZ}

— 局所的に凸なメトリザブル空間のビデュアルは、フレシェ空間です。

### 4. 反射的なフレシェの二重空間

#### 命題 4 {#evt-iv-s3-prop-4 .statement tag=07U0}

— E を再帰的なフレシェ空間とします。 E の強力な双対 $E'_b$ は、Banach 空間の数列の帰納的極限です。

$(V_n)_{n \in \mathbf{N}}$ を、凸でバランスがとれた閉じた減少列とし、E の 0 の近傍を、E 含むの 0 のすべての近傍が $V_n$ の 1 つになるようにします。 $A_n$ を $E'$ の $V_n$ の極とします。次に、$A_n$ は、$\sigma(E', E)$ に対して凸型でバランスが取れており、コンパクトです。 by III, p. 8, 系空間 $E'_{A_n}$ はバナッハ空間です。 $E'_b$ が空間 $E'_{A_n}$ の帰納極限であることを証明します。他の語では、各$A_n$を吸収する$E'$のすべての凸でバランスの取れた部分集合Uは、$E'_b$の0の近傍です。 $n \in \mathbf{N}$、選ぶ実数 $\lambda_n > 0$ ごとに、$\lambda_n A_n \subset U$ になります。 $B_n$ を集合 $\bigcup_{0 \leq i \leq n} \lambda_i A_i$ の凸包絡線とします。 $V = \bigcup_n B_n$を入れてから、$V \subset U$を入れます。 $n \in \mathbf{N}$ ごとに、集合 $B_n$ は、$\sigma(E', E)$ に対して凸でバランスが取れており、コンパクトです (II、p. 14、提案 15)。

次に、$\frac{1}{2} V^{oo} \subset V$ を示します。 $x \in E'_b - V$ にしましょう。すべての $n \in \mathbf{N}$ に対して、$x \notin B_n$ があり、$B_n$ が $\sigma(E', E)$ に対して閉じているため、$B_n^\circ$ には元 $y_n$ が存在し、 \langle y_n, x \rangle = 1 (\text{II, p. 38, prop. 4}）。 E は再帰的であるため、E のすべての有界部分集合は $\sigma(E, E')$ (IV, p. 16, th. 2) に対して比較的コンパクトです。 $B_n$の定義までに、
$$
\lambda_i y_n \in V_i \quad \text{for all } n \geq i,
$$
従って、数列 $(y_n)$ は有界です。 $y$ を位相 $\sigma(E, E')$ に対して $(y_n)$ の極限点とします。 $y \in V^\circ = \bigcap_n B_n^\circ$と$\langle y, x \rangle = 1$がございます。従って、$x \notin \frac{1}{2}V^{\circ\circ}$ となり、$\frac{1}{2}V^{\circ\circ} \subset V$ と *なおさら*、$\frac{1}{2}V^{\circ\circ} \subset U$ が含まれます。

$E'_b$ のすべての有界部分集合は集合 $A_n$ の 1 つに含まれるため、集合 $V = \bigcup_n B_n$ は $E'_b$ のすべての有界部分集合を吸収します。その結果、$V^\circ$ は E で有界であるため、$\frac{1}{2}V^{\circ\circ}$ は $E'_b$ の 0 の近傍になります。 *なおさら*、U は $E'_b$ の近傍です。

#### 系 {#evt-iv-s3-n4-cor-1 .statement tag=07U1}

*再帰的なフレシェ空間の強力な双対は、骨学的で樽型です。*

Banach 空間の帰納的極限は、定義によって誕生論的になります。さらに、バナッハ空間はバレル化されており (III、p. 25、系)、バレル化された空間のすべての帰納法極限はバレル化された空間 (III、p. 25、cor. 3) です。

### 5. 位相フレシェの双対上のコンパクトな収束空間

#### 定理 1 (バナッハ デュドネ) {#evt-iv-s3-thm-1 .statement tag=07U2}

— *E を局所的に凸な計化可能空間とする。 E のデュアル $E'$ 上の次のトポロジ一致する:*

a) *$\mathfrak{N}$収束の位相$\mathscr{T}_\mathfrak{N}$、ここで$\mathfrak{N}$は、0に収束するEの部分集合、数列の点のからなるの族です。
b) E のコンパクトな部分集合に対する一様収束の *位相 $\mathscr{T}_c$ ;*
c) E のプレコンパクト部分集合に対する一様収束の *位相 $\mathscr{T}_{pc}$ ;*
d) *位相 $\mathscr{T}_f$は、$E'$の等連続部分集合ごとに$\sigma(E', E)$と同じ位相を誘発する最高の位相です。

まず、$E'$の*部分集合 Aが$\mathscr{T}_f$に対して閉じているのは、$A \cap H$が$\sigma(E', E)$に対して閉じている場合に限り、$E'$の部分集合 Hごとに等連続で$\sigma(E', E)$に対して閉じていることを観察します。* 弱い位相 $\sigma(E', E)$ と $\mathscr{T}_{pc}$ 誘導するは、$E'$ の等連続部分集合ごとに同じ位相 (III、p. 17、提案 5)。その結果、各トポロジー $\mathscr{T}_\mathfrak{N}$、$\mathscr{T}_c$、$\mathscr{T}_{pc}$、$\mathscr{T}_f$ は、それに続くものよりも粗くなります。従って、$\mathscr{T}_\mathfrak{N}$ が $\mathscr{T}_f$ よりもより細かいであることを証明するだけで十分です。さらに、$E'$ のすべての翻訳は $\mathscr{T}_f$ の同型写像です。従って、F が $\mathscr{T}_f$ に対して閉じている $E'$ の部分集合であり、含む 0 ではない場合、$S^\circ \cap F = \varnothing$ となる集合 $S \in \mathfrak{N}$ が存在することを証明すれば十分です。

$(U_n)_{n \geq 0}$ を E の 0 の近傍の減少列として、0 の近傍の基本系を形成します。 $n \geq 0$ の帰納法までに構成する、*有限* 集合 $X_n$ となります。
$$
X_n \subset U_n
$$
$$
\left( \bigcup_{0 \leq p \leq n} X_p \right)^\circ \cap U_{n+1}^\circ \cap F = \varnothing
$$

整数 $n \geqslant 0$ごとに。 $m \geqslant 0$ を整数として、$X_n$ が $0 \leqslant n < m$ に対して構築され、$0 \leqslant n < m$ に対して (4) と (5) が満たされるようにします。 $x \in U_m$ごとに、
$$
F_x = (\bigcup_{0 \leqslant p < m} X_p)^{\circ} \cap \{x\}^{\circ} \cap U_{m+1}^{\circ} \cap F.
$$
公式 (5) と $n = m - 1$ は、$\bigcap_{x \in U_m} F_x = \varnothing$ を意味します。さらに、集合 $U_{m+1}^{\circ}$ は等連続であり、$\sigma(E', E)$ にとってコンパクトです。 $\mathscr{T}_f$の定義を考慮すると、集合$F_x$はそれぞれ$\sigma(E', E)$にとってコンパクトです。従って、$\bigcap_{x \in X_m} F_x = \varnothing$、つまり* 関係 (5) が $n = m$ に対して満たされるような $U_m$ の有限部分集合 $X_m$ が存在します。

$S = \bigcup_{n \geqslant 0} X_n$を入れてください。 $n \geqslant p$ に対して $X_n \subset U_p$ があるため、$S$ は数列の点の集合であり、$E$ で 0 に収束します。 (5) から $S^{\circ} \cap U_{n+1}^{\circ} \cap F = \varnothing$ が導き出され、$E'$ は集合 $U_{n+1}^{\circ}$ の数列の和集合であるため、$S^{\circ} \cap F = \varnothing$ が得られます。

#### 系 1 {#evt-iv-s3-thm-1-cor-1 .statement tag=07U3}

*$E$を局所的に凸なmetrizable空間とします。 Every precompact subset of $E$ is contained in the closed convex balanced envelope of the set of points of a sequence converging to 0.*

これは、prop により、トポロジー $\mathscr{T}_{pc}$ と $\mathscr{T}_{\mathfrak{H}}$ が同一であるという事実から導き出されます。 III、p. 15 の 2 つ。

#### 系 2 {#evt-iv-s3-thm-1-cor-2 .statement tag=07U4}

※$E$をフレシェ空間とします。 $E$ の双対 $E'$ の凸部分集合 $A$ が $\sigma(E', E)$ に対して閉じられる位数では、0 の近傍 $U$ ごとに $A \cap U^{\circ}$ が $\sigma(E', E)$ に対して閉じられることが必要かつ十分です。 $E$.*

$E$ が完全なので、$E'$ の位相 $\mathscr{T}_c$ は、$E'$ と $E$ の間の双対性 (IV、p. 3、*例*) と互換性があります。その結果、$E'$ の閉じた凸部分集合は、$\mathscr{T}_c$ と $\sigma(E', E)$ で同じになります (IV、p. 1、提案 1)。次に、トポロジー $\mathscr{T}_c$ と $\mathscr{T}_f$ の同一性から系が導き出されます。

(I、p. 13) を思い出してください。$\sigma(E', E)$ でクローズされている $E'$ の超平面は、$E$ の元に関連付けられた $E'$ の線型形式の核です。コル。従って、2 は cor の他の証明 (Fréchet の場合空間) を与えます。 III、p. 21 の 1 つ。

#### 系 3 {#evt-iv-s3-thm-1-cor-3 .statement tag=07U5}

*$E$を$E$の双対$E'$のバナッハ空間と$M$ベクトル部分空間とする。 位数で、弱者位相 $\sigma(E', E)$ に対して $M$ がクローズされることは、$E'$ の単位元ボール (クローズ) を持つ共通部分が $\sigma(E', E)$ に対してクローズされることで十分かつ十分です。

#### 例 {#evt-iv-s3-n5-exa-1 .statement tag=07U6}

— *$H$ を可算性の最初の公理であるヒルベルト空間満たすとします。 $H_{\sigma}$ は空間 $H$ を表し、弱められた位相が割り当てられます。 $\mathscr{L}^1(H)$ を、$H$ (V、p. 51、TS、V) の核自己準同型のバナッハ空間とします。 $\mathscr{L}^1(H)$ のノルムは $\|u\|_1 = \operatorname{Tr}((u^*u)^{1/2})$ によって定義されます。 $\mathscr{L}^1(H)$ の線型形式 $\phi_u : v \mapsto \operatorname{Tr}(uv)$ をすべての $u \in \mathscr{L}(H)$ と関連付けることで、バナッハ空間 $\mathscr{L}^1(H)$ の双対である同一視できる $\mathscr{L}(H)$ を作成します。 $A$ を $\mathscr{L}(H)$、含む 1 の部分代数とし、$u \mapsto u^*$ の下で安定とする。これは、弱者位相 $\sigma(\mathscr{L}(H), \mathscr{L}^1(H))$ のために $\mathscr{L}(H)$ に閉じられた場合に限り、フォン・ノイマン代数です。コルから。 3 では、次の基準を推定します。 * $A$ がノイマン型代数であるためには、$(u_n)$ が $A$ の元のいずれかの数列であり、ノルム $\leqslant 1$ が次の条件を満たしていることが必要かつ十分です。 極限 $u$ の空間 $\mathscr{L}_s(H ; H_{\sigma})$、その後 $u$ 属するから $A$ まで*。

### 6. 個別に連続する双線形マッピング

#### 補題 1 {#evt-iv-s3-lem-1 .statement tag=07U7}

E と F を 2 つの局所的に凸な可積化可能空間とし、u を $E'_b$ から F への連続線形写像とする。すると、$E'_b$ に 0 の近傍 U が存在し、その u の下の像は F で制限されます。

$(U_n)_{n \in \mathbf{N}}$ (それぞれ $(V_n)_{n \in \mathbf{N}}$) を E (それぞれ F) の 0 の近傍の基本となる系とします。 集合 $U_n$ はバランスが取れており、形減少列であると仮定します。 u は連続であるため、$n \in \mathbf{N}$ ごとに、$u(B_n^\circ) \subset V_n$ となるような有界の集合 $B_n$ が E に存在します。 $B_n$ は有界なので、$\lambda_n B_n \subset U_n$ となるような実数 $\lambda_n > 0$ が存在します。 $B = \bigcup_{n \in \mathbf{N}} \lambda_n B_n$を入れます。

集合 B は E で境界があり、他の語では、すべての整数 $m \geqslant 0$ に対して、$\mu B \subset U_m$ となる実数 $\mu > 0$ が存在することを証明します。 集合 $B_n$ は有界であるため、$0 < \mu \leqslant 1$ となるような実数 $\mu$ が存在し、$0 \leqslant n \leqslant m$ に対して $\mu (\lambda_n B_n) \subset U_m$ が存在します。 $n > m$なら$\lambda_n B_n \subset U_n \subset U_m$もあります。したがって、$U_m$ は均衡しているため、$\mu B \subset U_m$ となります。

U を $E'_b$ における B の極とします。これは、$E'_b$ の 0 の近傍であり、$\lambda_n B^\circ \subset B_n^\circ$ があるため、すべての $n \in \mathbf{N}$ に対して $\lambda_n u(U) \subset V_n$ になります。従って、$u(U)$ は F で有界されます。

#### 定理 2 {#evt-iv-s3-thm-2 .statement tag=07U8}

$E_1$ と $E_2$ を 2 つの再帰フレシェ空間とし、G を局所凸ハウスドルフ空間とします。 $i = 1, 2$ の場合、$F_i$ を $E_i$ の強力な双対とします。この場合、個別に連続するすべての双線形写像 $u : F_1 \times F_2 \to G$ は連続的になります。

空間 G は、Banach 空間の積の部分空間と同型です (II、p. 5、提案 3)。 Therefore it is enough to prove the theorem under the additional hypothesis that G is a Banach space. しかし、$F_1$ はバレルであり、$F_2$ ボーンロジカル (IV、p. 24、系)、$\mathscr{L}_b(F_2 ; G)$ はフレシェ空間 (IV、p. 23、提案 3) です。 v は、関係によって u に関連付けられた $F_1$ から $\mathscr{L}_b(F_2 , G)$ までの線形写像を表すものとします。

$$
u(x_1, x_2) = v(x_1)(x_2) \quad (x_1 \in F_1, x_2 \in F_2).
$$

$F_1$ はバレル化されており、u は個別に連続であるため、v は連続です (III, p. 31、提案 6)。

v は連続であるため、補題 1 は、$F_1$ に 0 の近傍 $U_1$ が存在することを意味します。その v の下の像は $\mathscr{L}_b(F_2 ; G)$ で制限されます。他の語では、$F_2$ のすべての有界部分集合 $B_2$ に対して、集合 $u(U_1 \times B_2)$ はバナッハ空間 G で有界されます。$U_2$ をすべての $x_2 \in F_2$ の集合とし、$\|u(x_1, x_2)\| \leqslant 1$ とします。 $x_1 \in U_1$の皆さんへ。 集合 $U_2$ は、境界のあるすべての部分集合を吸収します。 $F_2$ はボーンロジーであるため、$U_2$ は $F_2$ の 0 の近傍であり、これは u が連続であることを証明します。

### 練習問題 {#evt-iv-s3-exercises}

[§ 3 に対して練習問題](exercises/s3/)を参照してください。
