---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Semisimple Modules and Rings
section: 15
section_title: Brauer Groups
lang: ja
source: alg-viii
source_edition: 2023, Springer Nature
book_pages: A VIII.277-A VIII.284
pdf_pages: 0294-0301
extraction: native
subsections:
    - "no": 1
      title: Classes of Algebras
      page: 277
      pdf_page: 294
    - "no": 2
      title: Definition of the Brauer Group
      page: 278
      pdf_page: 295
    - "no": 3
      title: Change of Base Field
      page: 281
      pdf_page: 298
    - "no": 4
      title: Examples of Brauer Groups
      page: 283
      pdf_page: 300
statements: 12
exercises: 2
content_sha256: 3b353ea09e1208bf8186b5e29e5c196e043d7b0ab90671e417cbcb5c6764d4c4
translated_from: content/en/alg/VIII/15_s15_brauer_groups.md
translation_method: google
source_content_sha256: de0ee49b9fce0132064e5387825b803ddb4c6aeb3c6c606b44846dc5403449fc
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: 2cff9fdd86078b36097319bd73695054fd4c09b0d05c6d6838327c0d4c1773e4
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## § 15。 ブラウアー群

この切断において、Kは可換体です。

### 1. 代数の類

Iso$_K(A,B)$ 関係で表します

「A と B は有限次数の同型 K-代数です。」

これは A と B に関して同値関係です。A を有限次数の K-代数とします。 cl(A) (またはときどき cl$_K$(A)) で示される A の類は、関係 Iso$_K($集合理論, II, §6, No. 9, p. 122) の A と同等のオブジェクトの類です。 定義までに、cl(A) は K-代数 A と同型になります。 有限次数のうち 2 つの K-代数は、同型である場合に限り、同じ類にあります。

対 $(W, \mu)$ の $\mathscr{A}$ 集合で表します。ここで、W は、K 上の有限次元である $K^{(\mathbf{N})}$ の線形部分空間であり、$\mu$ は、W を (結合的および単位的) にする $W\times W$ から W までの K 双線形写像です。 K-代数。 有限次数のすべての K-代数は、そのような代数と同型です。ロケ地にて。前掲書、関係

「$\alpha$は有限次数のK-代数の類です」

従って、$\alpha ($集合理論、II, §1, No. 4、p. 68）で集団化しています。 集合、類、K-代数、有限次数を$\mathscr{C}_K$で表します。

#### 命題 1 {#alg-viii-s15-prop-1 .statement tag=00HV}

集合 $\mathscr{C}_K$ は、$(\alpha , \beta )\mapsto$ cl($\alpha \otimes_K\beta$ ) によって与えられる合成の法則を備えており、可換モノイドです。 $\mathscr{C}_K$の単位元はK-代数の類$\varepsilon$です。さらに、AとBが有限次数のK-代数であれば、関係になります

(1) cl(A $\otimes_KB$) $=$ cl(A) cl(B)。

A、B、および C を有限次数の K-代数とし、それぞれ類 $\alpha$、$\beta$、$\gamma$ とします。 K-代数 A と $\alpha$ は、B と $\beta$ と同様に同型です。 従って、K-代数 $A\otimes_KB$ と $\alpha \otimes_K\beta$ は同型であり、 cl(A$\otimes_KB$) $=$ cl($\alpha \otimes_K\beta$ ) となり、 公式 (1) が得られます。 従って、$(\alpha \beta )\gamma$ は K-代数 $(A\otimes_KB)\otimes_KC$ の類であり、$\alpha (\beta \gamma )$ は K-代数 $A\otimes_K(B\otimes_KC)$ の類であることがわかります。 さて、これらの K-代数は同型 (III, §4, No. 1、p. 461) であるため、等式 $(\alpha \beta )\gamma =\alpha (\beta \gamma )$ が得られます。 同様に、K-代数 $A\otimes_KK, K\otimes_KA$ と A が同型であるという事実から関係 $\alpha \varepsilon =\varepsilon \alpha =\alpha$ が得られ、代数 $A\otimes_KB$ と $B\otimes_KA$ が同型であるという事実から関係 $\alpha \beta =\beta \alpha$ が得られます。

集合 $\mathscr{C}_K$、関係 「$\alpha$と$\beta$はMorita同値な多元環」は同値関係（VIII、p. 100）です。 $\mathscr{C}_K$による合成の法則、命題13、d)のVIII、p. 111と互換性があります。 $\mathscr{C}_K$のモノイド$\mathscr{M}_K$商をこの同値関係で表し、$\mathscr{C}_K$から$\mathscr{M}_K$までの$\varphi$標準準同型で表します。 有限次数のすべての K-代数 A について、cl(A) の [A] 像を $\varphi$ で表します。 A と B が有限次数の K-代数である場合、K-代数 A と B が森田同等である場合に限り、[A] = [B] になります。さらに、関係があります

$$
[A\otimes_KB] = [A][B] \tag{2}
$$

モノイド $\mathscr{M}_K$ で。

#### 補題 1 {#alg-viii-s15-lem-1 .statement tag=00HW}

A を K 上の有限次数の K-代数および有限次数の D 体とします。A が $\mathbf{M}_n(K)$ と同型であるような整数 $n\geqslant 1$ が存在する場合に限り、$\mathscr{M}_K$ で [A] = [D] になります。

定義までに、可逆 $(A$, D) 双モジュール、つまり、同型を備えた D 上の非零有限次元の (VIII, p. 101, 定理 1)、右ベクトル空間 V が存在する場合に限り、[A] = [D] になります。 K-代数 $A\rightarrow$ 終わり$_D(V)$。 補題 1が続きます。

### 2. ブラウアー群中定義

Br(K) 集合の元の $\mathscr{M}_K$ の形 [A] で表します。ここで、A は K 上の有限次数の中心単純代数です。

#### 命題 2 {#alg-viii-s15-prop-2 .statement tag=00HX}

集合 Br(K) は $\mathscr{M}_K$ の可逆元の集合であり、Br(K) の元 [A] の逆数は $[A^o]$ です。その結果、モノイド$\mathscr{M}_K$上の合成の法則は、Br(K)にアーベル群の構造を与えます。

A を K 上の有限次数の中心単純代数とします。代数 $A^o$ は中心単純であり、K 上の有限次数の中心です (VIII, p. 251)。 代数 $A\otimes_KA^o$ は行列環 $\mathbf{M}_n$(K) と同型で、$n^2=$ dim(A) (VIII, p. 252, 定理 1) です。したがって、$[A][A^o] = [A\otimes_KA^o] = [K]$ (補題 1) が得られ、これは [A] が逆数 $[A^o]$ で可逆であることを証明します。

逆に、A を有限次数の K-代数とします。 [A] が $\mathscr{M}_K$ で反転可能な場合、[A][B] = [K] となる有限次数の K-代数 B が存在します。 公式 (2) と補題 1 により、これは、K-代数 $A\otimes_KB$ が $n\geqslant 1$ と行列環 $\mathbf{M}_n(K)$ に同型であることを意味します。 注意 VIII、p. 251、代数の 1 までに、A が中央のシンプルになります。

#### 定義 1 {#alg-viii-s15-def-1 .statement tag=00HY}

アーベル群 Br(K) は体 K のブラウアー群と呼ばれます。

#### 補題 2 {#alg-viii-s15-lem-2 .statement tag=00HZ}

I と J を有限集合、$k$ を可換環、A と B を$k$-代数とする。 A にエントリを持つ型 $(I,I)$ の正方行列の $k$ 代数を $\mathbf{M}_I(A)$ で表し、同様に $k$ 代数 $\mathbf{M}_J(B)$ と $\mathbf{M}_{I\times J}(A\otimes_KB)$ を定義するで表します。一意的 $k$-代数同型性が存在します

$$
\varphi :\mathbf{M}_I(A)\otimes_k\mathbf{M}_J(B)\longrightarrow \mathbf{M}_{I\times J}(A\otimes_kB)
$$

$\varphi ((a_{ii'})\otimes (b_{jj'}))$ は行列で、添字 $((i, j),(i', j'))$ は $a_{ii'}\otimes b_{jj'}$ と等しくなります。

補題で述べた性質を伴う $k$ 線形全単射 $\varphi$ の存在は、テンソル積と直和 (II, §3, No. 7、p. 255、命題 7) の互換性から導き出されます。 $\varphi$ が代数準同型であるという事実は、積行列の定義から続きます。

#### 命題 3 {#alg-viii-s15-prop-3 .statement tag=00I0}

A と B を有限次数の中心単純K-代数とします。次のプロパティは同等です。

(i) ブラウアー群 Br(K) では [A] = [B] です。

(ii) K-代数 $A\otimes_KB^o$ が行列環 $\mathbf{M}_t(K)$ と同型となるような整数 $t\geqslant 1$ が存在します。

(iii) K-代数 $A\otimes_K\mathbf{M}_r(K)$ と $B\otimes_K\mathbf{M}_s(K)$ が同型となるような正の整数 $r$ と $s$ が厳密に存在します。

(iv) A が $\mathbf{M}_m(D)$ と同型、B が $\mathbf{M}_n(D)$ と同型であるような体 D 含む K と整数 $m\geqslant 1$ および $n\geqslant 1$ が存在します。

(v) K-代数 A と B は森田相当です。

[A] = [B] であるとします。 $[B^o]$はブラウアー群の[B]の逆数なので、$[K] = [B][B^o] = [A][B^o] = [A\otimes_KB^o]$になります。 補題 1 までに、代数 $A\otimes_KB^o$ と $\mathbf{M}_t(K)$ が同型となるような整数 $t\geqslant 1$ が存在します。したがって、(i) は (ii) を意味します。

(ii) が成り立つと仮定します。 $B^o\otimes_KB$ は $s\geqslant 1$ (VIII, p. 252, 定理 1) と行列環 $\mathbf{M}_s(K)$ と同型であるため、代数 $A\otimes_KB^o\otimes_KB$ は一方では $A\otimes_K\mathbf{M}_s$(K) と同型であり、一方、$\mathbf{M}_t(K)\otimes_KB$。したがって、性質 (ii) は性質 (iii) を意味します。

(iii) が成り立つと仮定します。ウェダーバーンの定理 (VIII, p. 120, 定理 1) により、K を超える有限次数の整数 $m\geqslant 1$ と $n\geqslant 1$ と体 D と $D'$ が存在します。 中心 K は、A が $\mathbf{M}_m(D)$ と同型、B が $\mathbf{M}_n(D')$ と同型です。次に、代数 $A\otimes_K\mathbf{M}_r(K)$ は $\mathbf{M}_{mr}$(D) と同型で、代数 $B\otimes_K\mathbf{M}_{r'}(K)$ は $\mathbf{M}_{nr'}(D')$ (補題 2) と同型です。 系までに、VIII、p. 121、K-代数 D、$D'$ のうち 2 つが同型です。したがって、(iii) は (iv) を意味します。

(iv) が成り立つと仮定します。 代数 A と D は森田と同等であり、代数 B と D (VIII、p. 114、例 2) も同様です。したがって、A と B は森田等価なので、(iv) は (v) を意味します。

最後に、含意 (v)$\Rightarrow$(i) は集合 Br(K) の定義です。

命題の等価な性質が成り立つとき、代数 A と B は類似していると言います。

#### 系 {#alg-viii-s15-n2-cor-1 .statement tag=00I1}

A と B が K 上の有限次数の中心単純代数であるとします。そのとき、A と B は、それらが類似しており、同じ次数を持つ場合に限り、同型です。

これは、命題 3 のプロパティ (i) と (iv) の同値と、dim$_K(\mathbf{M}_n(D)) =$ dim$_K(D)\times n^2$ という事実から導き出されます。

#### 命題 4 {#alg-viii-s15-prop-4 .statement tag=00I2}

$\mathscr{K}_K$を、有限次数の中央K-代数、つまり体の類の集合とします。 写像 $D\mapsto [D]$ $\mathscr{K}_K$ から Br(K) までは全単射です。

これは、VIII、p. 278 の補題 1、およびウェダーバーンの定理 (VIII、p. 120、定理 1) に続きます。

### 3. 変更/基礎体

L を体 K の拡大とします。A と B を有限次数の K-代数とします。その場合、L-代数 $A_{(L)}$ と $B_{(L)}$ は有限次数になります。 L-代数 $A_{(L)}\otimes_LB_{(L)}$ と $(A\otimes_KB)_{(L)}$ は同型です (III, §4, No. 1, p. 462, 命題 3)。 L-代数 $K_{(L)}$ は L と同型です。従って、次のような$\mathscr{C}_K$ から $\mathscr{C}_L$ までの一意のモノイド準同型 $\rho_{L/K}$ が存在します。

(3) $\rho_{L/K}$(cl(A)) = cl(A$_{(L)}$)

有限次数の K-代数 A ごとに。

K-代数 A と B が森田等価である場合、L-代数 $A_{(L)}$ と $B_{(L)}$ (VIII, p. 111, 命題 13, e)) も同様です。 K-代数 A が中心単純で、有限次数の場合、L-代数 $A_{(L)}$ (VIII, p. 251, 注意 2) も同様です。従って、 $\rho_{L/K}$ 群準同型 $r_{L/K}$ から Br(K) から Br(L) まで推論できます。

$$
r_{L/K}([A]) = [A_{(L)}] \tag{4}
$$

有限次数の中心単純K-代数 A ごとに。

M を体 L の拡大とします。スカラーの拡大は推移的 (III, §1, No. 5、p. 434) であるため、関係となります。

$$
r_{M/K}=r_{M/L}\circ r_{L/K} \tag{5}
$$

A を有限次数の中心単純K-代数とし、L を K の拡大とします。L-代数$A_{(L)}$ が同型である場合、L は A (または分裂 A) の分解体であると言います。 行列環 $\mathbf{M}_n(L)$ に対して整数 $n\geqslant 1$。前述の記法では、この対応するからという、Br(K)のAの類属するから準同型の$r_{L/K}:$Br(K)$\rightarrow$の核です。 Br(L)。

B が A に類似している場合、B の分解体である場合に限り、A の L は A の分解体になります。

L が A の分解体である場合、L のすべての拡大は A の分解体になります。 VIII、p. 252 の定理により、K のガロア拡大が存在します。 有限次数は A の分解体であり、K のすべての分離閉包は A の分解体です。

#### 命題 5 {#alg-viii-s15-prop-5 .statement tag=00I3}

A を有限次数の中心単純K-代数とし、L を有限次数の K の拡大とします。次のプロパティは同等です。

(i) 拡大 L は A の分解体です。

(ii) L と同型の最大可換部分代数含むに類似した有限次数の中心単純K-代数が存在します。

(ii) が (i) を意味することを証明しましょう。 L が A の最大値可換部分代数である場合を考えれば十分です。 $\psi : A\otimes_KA^o\rightarrow$ End$_K(A)$ を標準同型として、$a\otimes a'$ を K-線型写像 $x\mapsto axa'$ (VIII, p. 252、定理 1)。 A は L よりも右ベクトル空間と見なされます。次に、$\psi$ は、L-代数$\psi ': A\otimes_KL\rightarrow$ の制限、単射準同型によって、$A\otimes_KL$ を End$_K(A)$ の部分空間 End$_L(A)$ と誘導するに送ります。終わり$_L(A)$。 集合 $n= [L : K]$。 VIII、p. 262、命題 3 までに $[A : L] =n$ があり、従って $[A\otimes_KL : L] = [A : K] =n^2$ と [終了$_L(A) : L] =n^2$] になります。従って、$\psi '$ は同型となり、(i) が証明されます。

逆は以下の補題 3 から続きます。

#### 補題 3 {#alg-viii-s15-lem-3 .statement tag=00I4}

Aを有限次数の中心単純K-代数とし、Lを有限次数のKの拡大、つまりAの分解体とします。Vを単純な$A_{(L)}$加群とするため、自然な射 $\varphi : A_{(L)}\rightarrow$終わり$_L(V)$は同型です。 C を環 End$_A(V)$ とします。この場合、C は $A^o$ に類似し、$L\otimes 1\subset A_{(L)}$ の像は C の最大値可換部分代数になります。

私たちは$A_{(L)}$の部分環と同一視するAです。 V を K-ベクトル空間と見ます。 環 C は、エンド$_K(V)$ の $\varphi (A)$ の交換子環です。 有限次数の中心単純K-代数であり、$A\otimes_KC$からエンド$_K(V)$までの準同型$a\otimes c\mapsto ac$は同型(VIII, p. 260, 定理 6, a))です。従って、K-代数 A と $C^o$ は類似します (VIII、p. 279、命題 3)。

$L_V$ を L ベクトル空間 V の相似性の環とします。エンド$_K(V)$ (VIII、p. 82、系 1) のエンド$_L(V)$ の交換子環です。さて、K-代数 End$_L(V)$ は $\varphi (A)$ と $L_V$ によって生成されます。従って、End$_K$(V) では、

$L_V=$ 終了$_L(V)'=\varphi (A)'\cap L'_V= C\cap L'_V$、

ここで、End$_K$(V)の部分集合 B、End$_K(V)$のBの交換子環は$B'$で表されます。従って、$L_V$ は、C (VIII、p. 261、補題 3) の最大可換部分代数であり、従って、$C^o$ の最大可換部分代数でもあります。 写像 $\lambda \mapsto \lambda_V$ は、L から $L_V$ までの K-代数同型です。これは補題を証明します。

#### 系 1 {#alg-viii-s15-lem-3-cor-1 .statement tag=00I5}

A を有限次数の中心単純K-代数とし、L を有限次数の K の拡大とします。 $[A : K] = [L : K]^2$ と仮定します。このとき、含む部分代数が L と同型である場合に限り、A に対して L は分解体になります。

L から A まで射 $\varphi$ が存在するとします。M を最大値半単純可換部分代数含む $\varphi (L)$ とします。 VIII, p. 262 の命題 3 までに、$[A : K] = [M : K]^2$ が得られるため、[M : K] = [L : K] および $M =\varphi (L)$ となります。 命題 5、体 L 分裂 A まで。逆に、体 L 分裂 A と仮定します。次に、A (命題 5) と同様に、中心単純K-代数 B の最大可換部分代数と同型です。 $[B : K] = [L : K]^2$ (VIII, p. 262, 命題 3) があるため、[B : K] = [A : K] となります。従って、B は A と同型です (VIII, p. 280, 系)。 系 1 が続きます。

#### 系 2 {#alg-viii-s15-lem-3-cor-2 .statement tag=00I6}

D を K 上の有限次数の体と中心 K とし、L を有限次数の K の拡大とします。つまり、D の分解体です。D 割るの還元された次数 [L : K]。

D (VIII, p. 253) を $r$ だけ減じた次数を表します。 定義までに$[D : K] =r^2$ができました。 命題 5 までに、D と同様の中心単純K-代数 B が存在します。そのうちの L は最大の可換部分代数です。 B は行列環 $\mathbf{M}_n(D)$ (VIII, p. 278, 補題 1) と同型なので、$[B : K] =n^2r^2$ があり、その結果 $[L : K] =nr$ (VIII, p. 262, 命題 3) になります。

### 4. ブラウアー群中例

以下の 3 つの場合、ブラウアー群 Br(K) は単位元に還元されます。

a) K は分離的に閉じています (VIII、p. 253、系 1)。

$*$b) K は有限体 (VIII、p. 357、系 2) です。

c) K には性質 $(C_1)$ (VIII, p. 357, 注意 2) があります。

K が極大順序体 (VI, §2, No. 5, p. 25) であるとします。 K のブラウアー群は位数 2 の循環になります。その元は K の類と型 $(-1,0,-1)$ (III, §2, No. 5、p. 444 および VIII、p. 367、定理 1) の四元数 K-代数の類です。

K が局所的にコンパクト、非離散、可換トポロジカル体であると仮定します。 K が接続されていない場合、離散評価では完全な体となり、有限の剰余体 (Comm. Alg., VI, §9, No. 3, p. 433, 定理 1)、Br(K) から $\mathbf{Q}/\mathbf{Z}$ (VIII, p. 332, 練習問題 17) までの同型が存在します。 K が接続されている場合、それは $\mathbf{R}$ または $\mathbf{C}$ と同型です。 体 $\mathbf{R}$ のブラウアー群は位数 2 の循環です。 その自明ではない元は、ハミルトン四元数の代数 $\mathbf{H}$ の類です (Gen. トップ。、VIII, §1, No. 4、p. 104); $\mathbf{C}$ のブラウアー群には位数 1 があります。

### 練習問題 {#alg-viii-s15-exercises}

[§ 15 に対して練習問題](exercises/s15/)を参照してください。
