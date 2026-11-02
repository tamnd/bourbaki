---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Semisimple Modules and Rings
section: 12
section_title: Tensor Products of Semisimple Modules
lang: ja
source: alg-viii
source_edition: 2023, Springer Nature
book_pages: A VIII.211-A VIII.228
pdf_pages: 0228-0245
extraction: native
subsections:
    - "no": 1
      title: Semisimple Modules over Tensor Products of Algebras
      page: 211
      pdf_page: 228
    - "no": 2
      title: Tensor Products of Simple Modules
      page: 213
      pdf_page: 230
    - "no": 3
      title: Tensor Products of Semisimple Commutative Algebras
      page: 215
      pdf_page: 232
    - "no": 4
      title: The Radical of a Tensor Product of Algebras
      page: 217
      pdf_page: 234
    - "no": 5
      title: Tensor Products of Semisimple Modules
      page: 218
      pdf_page: 235
    - "no": 6
      title: Tensor Products of Semisimple Algebras
      page: 221
      pdf_page: 238
    - "no": 7
      title: Extension of Scalars in Semisimple Modules
      page: 222
      pdf_page: 239
statements: 26
exercises: 17
content_sha256: 5731d143c0866a0f47e7470f09255c50b03b8be4cfe830a0ddc2991d5dd511e8
translated_from: content/en/alg/VIII/12_s12_tensor_products_of_semisimple_modules.md
translation_method: google
source_content_sha256: b311e3c926d1c35b21ba3909e0ec3e0584eb38f0337ee0f5d814716a0a8f67c8
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-b071ad41
glossary_version: 34
glossary_terms_sha256: cc545ade5ae0d3f9e937fb723809ddc1077ca32eb7aa6c45b2d4db0d3b2e8064
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## § 12。 半単純加群中テンソル積

この切断において、文字Kは可換体を表します。 E と F が K よりベクトル空間である場合、テンソル積 $E\otimes_KF$ を $E\otimes F$ で表します。

### 1. 代数のテンソル積を超える半単純加群

この小節では、K-代数 $A_1$ と $A_2$ を考慮します。 代数 $A_1\otimes A_2$ を A で表します。

#### 命題 1 {#alg-viii-s12-prop-1 .statement tag=00E6}

Let $M_1$ be an $A_1$-module and $M_2$ an $A_2$-module, neither reduced to 0. 環 $A = A_1\otimes A_2$ 上の加群 $M = M_1\otimes M_2$ が単純 (それぞれ等型、半単純) である場合、$A_1$ モジュール $M_1$ と $A_2$ モジュール $M_2$ は単純です (それぞれ等型、 半単純）。

M が半単純A-加群であるとします。 $N_1$ を $M_1$ の $A_1$ サブモジュールとします。 A-加群 M の $N_1\otimes M_2$ の標準像を N で表します。 VIII、p. 56 の系 2 により、M に像 N を持つ A 線形射影子 $p$ が存在します。 仮定により、 $M_2\not= 0$ を持っています。従って、$M_2$ の選ぶ元 $m$ と K-ベクトル空間 $M_2$ の線型形式 $\varphi$ は、$\varphi (m) = 1$ (II, §7, No. 5, p. 302, 系) のようになります2)。 $u$ を $M_1$ から $u(m_1) =m_1\otimes m$ で定義される M までの写像とし、$v$ を $v(m_1\otimes m_2) =\varphi (m_2)m_1$ で特徴付けられる M から $M_1$ までの K-線型写像とします。 集合 $q=v\circ p\circ u$。 写像 $q: M_1\rightarrow M_1$ は $A_1$ 線形で、その像は $N_1$ に含まれており、$n\in N_1$ ごとに $q(n) =n$ があります。その結果、$q$は$M_1$の像$N_1$で射影子となります。 $M_1$ が半単純 $A_1$ モジュール (VIII, p. 56, 系 2) であることを証明しました。

M が単純で、$M_1$ が 2 つの $A_1$ サブモジュール $M'_1$ と $M''_1$ の直和であると仮定します。 集合 $M'= M'_1\otimes M_2$ と $M''= M''_1\otimes M_2$;その場合、M は A-部分加群 $M'$ と $M''$ の直和です。 M は単純なので、$M'$ または $M''$ を 0 に減らす必要があります。 仮定までに $M_2\not= 0$ があるので、$M'_1= 0$ または $M''_1= 0$ (II, §3, No. 7、p. 256、系 2) になります。これは、$M_1$ が単純な $A_1$ 加群であることを証明します。

ここで、M が等型A-加群であるとします。 S と T を単純な $A_1$ - $M_1$ のサブモジュールとする。 A-加群 $S\otimes M_2$ と $T\otimes M_2$ は、M の非零部分加群と識別できます。 したがって、これらは M と同じ型の同型です。 注意 VIII、p. 61 までに、非零が存在します。 A-線型写像 $f: S\otimes M_2\rightarrow T\otimes M_2$。 写像 $f$ は、特に $A_1$ 線形です。 $A_1$加群 $S\otimes M_2$ と $T\otimes M_2$ は非零であり、それぞれ型 S と T の同型であるため、S と T は同型です。これは、$M_1$ が同型の $A_1$ 加群であることを証明します。

#### 命題 2 {#alg-viii-s12-prop-2 .statement tag=00E7}

S を環 $A = A_1\otimes A_2$ 上の単純加群、K 上の有限次元とする。 $i\in  \{1,2\}$ については、$A_i$ 加群 S が型 $S_i$ と同型であるような単純な $A_i$ 加群 $S_i$ が存在します。 A-加群 S は、A-加群 $S_1\otimes S_2$ の商と同型です。

S は K 上で有限次元の非零 $A_1$ 加群であるため、$A_1$ 上で有限長を持ち、$S_1$ から S への単純な左 $A_1$ $S_1$ および非零 $A_1$ 線形写像が存在します。 $M_2=$ Hom$_{A_1}(S_1,S)$ と、外部法則 $(a_2, u)\mapsto (a_2)_S\circ u$ によって定義される左$A_2$ モジュール構造。 $M_2\not= 0$ by 構成があり、$M_2$ は K 上の有限次元です。したがって、単純な左 $A_2$ 加群 $S_2$ と非零 $A_2$ 線形写像 $\varphi : S_2\rightarrow M_2$ を見つけることができます。私たちは定義する非零 A-線型写像 $\psi$ $S_1\otimes S_2$ から S まで

$$
\psi (s_1\otimes s_2) =\varphi (s_2)(s_1) \tag{1}
$$

$s_1\in S_1$ と $s_2\in S_2$ ごとに。 S は単純A-加群で、$\psi$ は零ではないので、$\psi$ は全射であり、S は $S_1\otimes S_2$ の商と同型です。 $i\in  \{1,2\}$ の場合、$A_i$ 加群 $S_1\otimes S_2$ は型 $S_i$ と同型であるため、$A_i$ 加群 S (VIII、p. 61、命題 2) も同様です。

任意の K-代数 B について、K 上の有限次元である単純 (VIII, p. 51) 左B-加群の類の $\mathscr{S}_K(B)$ 集合で表します。

#### 定理 1 {#alg-viii-s12-thm-1 .statement tag=00E8}

体 K が代数的に閉じていると仮定します。

a) $M_1$ を $A_1$ モジュール、$M_2$ を $A_2$ モジュールとし、両方とも単純 (それぞれ半単純) で K 上の有限次元とします。 この場合、$M_1\otimes M_2$ は、環 $A_1\otimes A_2$ 上の単純 (それぞれ半単純) 加群であり、K 上の有限次元です。

b) The mapping from $\mathscr{S}_K(A_1)\times \mathscr{S}_K(A_2)$ to $\mathscr{S}_K(A_1\otimes A_2)$ that sends (cl(S$_1$), cl(S$_2$)) to cl(S$_1\otimes S_2$), where $S_1($resp. $S_2)$ is a simple $A_1$-module (resp. $A_2$-module) that is finite-dimensional over K, is bijective.

部分 a) を証明するには、$M_1$ と $M_2$ が単純な場合を考えれば十分です。 $M'$ を $M = M_1\otimes M_2$ の A-部分加群とします。それは、$M_1\otimes M_2$の$A_1$サブモジュールであり、形$1_{M_1}\otimes u$の自己準同型の集合で安定しており、$u$は$A_2$モジュール$M_2$の相同性の集合を通過します。 体 K は代数的に閉じているため、シュールの補題 (VIII, p. 47, 定理 1) は、$M_1$ の交換子環 End$_{A_1}(M_1)$ が K に等しいことを意味します。 VIII、p. 63、A-部分加群の系 2 により、$M_1\otimes M_2$ の $M'$ は形 $M_1\otimes M'_2$ になります。ここで、$M'_2$ は $M_2$ の $A_2$ サブモジュールです。 $M_2$ は単純であると仮定しました。従って、$M'_2= 0$ または $M'_2= M_2$、つまり $M'= 0$ または $M'= M$ になります。 従って、M は単純です。

S が K 上の有限次元である $A_1\otimes A_2$ 上の単純加群である場合、命題 2 と部分 a) から、S は形 $S_1\otimes S_2$ の加群と同型であることがわかります。ここで、$S_1$ (それぞれ $S_2$) は単純な式です。 $A_1$ モジュール (それぞれ $A_2$ モジュール)。さらに、$A_i$加群として、Sは型$S_i$と同型であるため、$S_i$の類はSのそれにのみ依存します。これは部分b)を証明します。

#### 注意 1 {#alg-viii-s12-n1-rem-1 .statement tag=00E9}

体 K が代数的に閉じていると仮定されていない場合、定理 1 の主張 a) は真ではなくなります。 例 (VIII, p. 225, 練習問題 4) を与えることができます。ここで、$M_i$ は、$i\in  \{1,2\}$ に対して K 上の有限次元である単純な $A_i$ 加群であり、A-加群 $M_1\otimes M_2$ は半単純ではないか、または半単純しかし単純ではありません。

#### 注意 2 {#alg-viii-s12-n1-rem-2 .statement tag=00EA}

関係 $\varphi ([M_1]\otimes [M_2]) = [M_1\otimes M_2]$ によって特徴付けられる $R_K(A_1)\otimes_{\mathbf{Z}}R_K(A_2)$ から $R_K(A)$ までの準同型 $\varphi$ が存在します。 これは、VIII、p. 196の命題9と同様に証明できます。 If the field K is algebraically closed, then $\varphi$ is an isomorphism from $R_K(A_1)\otimes_ZR_K(A_2)$ to $R_K(A)$ by Theorem 1, b) because for every K-algebra B, the $\mathbf{Z}$-module $R_K(B)$ is free with basis the family $([S])_{S\in\mathscr{S}_K(B)}$ (VIII, p. 195).

### 2. 単純加群中テンソル積

$A_1$ と $A_2$ を可換体 K 以上の代数とします。K-代数 $A_1\otimes A_2$ を A で表します。

#### 補題 1 {#alg-viii-s12-lem-1 .statement tag=00RB}

$M_1$ と $N_1$ を $A_1$ モジュール、$M_2$ と $N_2$ を $A_2$ モジュールとします。次の仮定を作成します。

(i) $A_1$-モジュール $M_1$ が有限生成されます。

(ii) $A_2$ 加群 $M_2$ は有限生成されるか、$N_1$ は K 上で有限次元です。

集合 $M = M_1\otimes M_2$ と $N = N_1\otimes N_2$ を、環 $A = A_1\otimes A_2$ の上に加群として表示します。 標準準同型 (II, §3, No. 5、p. 251)

$\lambda :$ ホム$_K(M_1,N_1)\otimes$ ホム$_K(M_2,N_2)\longrightarrow$ ホム$_K(M,N)$

次に誘導する同型の K-ベクトル空間

$\varphi :$ホム$_{A_1}(M_1,N_1)\otimes$ホム$_{A_2}(M_2,N_2)\longrightarrow$ホム$_A(M,N)$。

写像 $\lambda$ は単射法 (II, §7, No. 7、p. 308、命題 16) であり、線形の部分空間 Hom$_{A_1}(M_1,N_1)\otimes$ Hom$_{A_2}(M_2,N_2)$ を Hom$_A(M,N)$ に送信します。したがって、Hom$_{A_1}(M_1,N_1)\otimes$ Hom$_{A_2}(M_2,N_2)$ の M から N 属するから像までのすべての A-線型写像が $\lambda$ によって証明されるだけで十分です。 $u: M\rightarrow N$をA-線型写像とします。 $x\in M_1$ にしましょう。 $M_2$ から $N_1\otimes N_2$ までの $A_2$ 線形マッピング $y\mapsto u(x\otimes y)$ を $u_x$ で示します。 集合 P = Hom$_{A_2}(M_2,N_2)$、$N_1\otimes P$ から Hom$_{A_2}(M_2,N_1\otimes N_2)$ (II, §4, No. 2、p. 269) までを$\nu$ 標準準同型で表します。この写像は単射法です (II, §4, No. 2、p. 269、命題 2、(i) K-ベクトル空間 $N_1$ に適用されます)。 仮定 (ii) により、$u_x$ が $V_x\otimes N_2$ で値となるような、K 上の有限次元の $N_1$ の線形部分空間 $V_x$ が存在します。したがって、$u_x$は、一意元の$\nu$、$N_1\otimes P$の$v_x$により、像となります。 $M_1$ から $N_1\otimes P$ までの写像 $\widetilde{u}:x\mapsto v_x$ は $A_1$ 直線です。 仮定 (i) により、$A_1$ 加群 $M_1$ が有限生成されます。 推論は上記と同様に、ホム$_{A_1}(M_1,N_1\otimes P)$ のホム$_{A_1}(M_1,N_1)\otimes P$ の$\widetilde{u}$ 属するから像を示しています。 補題 1 が続きます。

#### 定理 2 {#alg-viii-s12-thm-2 .statement tag=00EB}

$A_1$ と $A_2$ を可換体 K 以上の代数とします。 $S_1$ を単純な $A_1$ モジュール、$S_2$ を単純な $A_2$ モジュールとしましょう。 $D_1$ と $D_2$ をそれぞれ $S_1$ と $S_2$ の交換子環とします。 集合 $M = S_1\otimes S_2,A = A_1\otimes A_2$ および $D = D_1\otimes D_2$ M を左の $(A,D)$-bimodule として見ます。

a) A-加群 M の交換子環は $D_M$ に等しい。

b) 写像 $\mathfrak{a}\mapsto \mathfrak{a}M$ は、包含順に並べられた D の正しい理想の集合から、包含順に並べられた M の A-部分加群の集合までの同型です。逆写像は、M の部分加群 N を、$dM\subset N$ となるように、元 $d$ の D からなるのイデアルに送ります。

主張 a) は、単純加群が一次であるため、補題 1 から続きます。

T を $(A_1,D_2$)-bimodule $S_1\otimes (D_2)_d$ とします。私たちは同一視する $M = S_1\otimes S_2$ と $T\otimes_{D_2}S_2$ (II, §3, No. 8、p. 258)。この識別は、環 $A = A_1\otimes A_2$ を超える左加群の構造と互換性があります。

N を M の A-部分加群とします。これは、$T\otimes_{D_2}S_2$ の $A_2$ サブモジュールであり、$A_1$ までの$a_1$ の間、形 $(a_1)_T\otimes 1_{S_2}$ の自己準同型によって安定します。 VIII、p. 63 の系 2 から、$N = V\otimes_{D_2}S_2$ のような T の固有の $(A_1,D_2)$ サブバイモジュール V が存在することがわかります。

$u(s\otimes d) = 1\otimes d\otimes s$ で定義される $T = S_1\otimes (D_2)_d$ から $((D_1)_d\otimes (D_2)_d)\otimes_{D_1}S_1$ までの同型 $u$ は、$(A_1,D_2$)-線形です。私たちは同一視するこれらの $(A_1,D_2)$ バイモジュールです。上記と同様の推論は、$V =\mathfrak{a}\otimes_{D_1}S_1$となるような$D_1\otimes D_2$の権利$(D_1\otimes D_2$)サブモジュール$\mathfrak{a}$の存在と一意性を証明します。上記の識別を考慮すると、$\mathfrak{a}$ は、$N =\mathfrak{a}M$ となるような、$D = D_1\otimes D_2$ の固有の正しい理想です。

写像 $\mathfrak{a}\mapsto \mathfrak{a}M$ が全単射であることを証明したところです。 最後の主張が続きます。

#### 系 1 {#alg-viii-s12-thm-2-cor-1 .statement tag=00EC}

環 $D = D_1\otimes D_2$ が半単純 (それぞれ単純、体) である場合に限り、環 $A_1\otimes A_2$ に対する加群 $S_1\otimes S_2$ は半単純 (それぞれ同型、単純) です。特に、$S_1$ または $S_2$ の交換子環が K に等しい場合、$S_1\otimes S_2$ は単純です。

定理 2 により、右D-加群 $(D_1\otimes D_2)_d$ が (VIII, p. 109, 命題) である場合に限り、環 $D_1\otimes D_2$ を超える加群 $S_1\otimes S_2$ は半単純 (それぞれ同型、単純) になります。 10)。 Now the right D-module $D_d$ is simple if and and only if D is a field; it is isotypical (resp. semisimple) if and only if the ring D is simple (resp. semisimple) (VIII, p. 120, Definition 1; VIII、p. 121、系 1;およびVIII、p. 137、命題 2)。

#### 系 2 {#alg-viii-s12-thm-2-cor-2 .statement tag=00ED}

$\mathfrak{R}_A(M) =\mathfrak{R}(D)M$ があります。 A-加群 M は根基なしで、環 D に根基がない場合に限ります。

これは、VIII、p. 108、定理 2 の命題 8、b) から続きます。

### 3. 半単純可換代数中テンソル積

#### 定理 3 {#alg-viii-s12-thm-3 .statement tag=00EE}

$Z_1$ と $Z_2$ を K 上の半単純可換代数とします。 環 $Z_1\otimes Z_2$ の根基は、その冪零元の集合に等しいです。

まず、$Z_1$ と $Z_2$ が体 K の拡大 $L_1$ と $L_2$ である場合を扱います。 必要に応じて交換すること $L_1$ と $L_2$ によって、K 上の $L_1$ の超越次数が K 上の $L_2$ の超越値よりも小さい場合に簡約するします。 $L_2$ の選ぶ代数閉包 Ω; 系 1 of 定理 5 of V, §14, No. 6、p. 114 により、$L_1$ は Ω の部分拡張であると仮定できます。

A) まず、$L_1\otimes L_2$ の根基が $L_1\otimes \Omega$ の中に含まれていることを証明しましょう。 集合 $\mathfrak{a}=\mathfrak{R}(L_1\otimes L_2)(L_1\otimes \Omega )$;それは可換環 $L_1\otimes \Omega$ の理想であり、$L_1\otimes \Omega$ の根基に $\mathfrak{a}$ が含まれるという証明しなければならないです。他の語 (VIII、p. 156、定理 1) では、$x\in \mathfrak{a}$ に対して、元 $1 +x$ は $L_1\otimes \Omega$ で反転可能であることが証明しなければならないわかります。さて、Ωは$L_2$の代数拡大なので、$L_2$、有限次数の拡大$L_3$が存在し、$x$属するから$\mathfrak{R}(L_1\otimes L_2)(L_1\otimes L_3)$になります。 $1 +x$ が $L_1\otimes L_3$ で可逆であることを証明するには明らかに十分です。現在、$C = L_1\otimes L_3$ は環 $B = L_1\otimes L_2$ を超えて有限生成加群です。 VIIIの系、p. 175により、$\mathfrak{R}(B)C\subset \mathfrak{R}$(C)が得られるので、$x$の属するからCの根基と$1 +x$はCで反転可能です。

B) $L_1\otimes \Omega$ の根基が冪零元で構成されることを証明しましょう。 K の特性指数を $p$ で表し、Ω (V, §5, No. 2, p. 25) における K の相対的な $p$ ラジカル (つまり、純粋に分離不可能な) 閉包を P で表します。 体 P は完璧です。 P は K の代数拡大なので、$L_1(P) = L_1[P]$ (V, §3, No. 2, p. 18, 系 1) になります。 $\mathfrak{b}$ を $L_1\otimes P$ から体 $P_1= L_1[P]$ までの標準準同型の核とします。 $x\in \mathfrak{b}$ にしましょう。 $x=\sum^n_{i=1}y_i\otimes z_i$ と $\sum_{i=1}^ny_iz_i= 0$ のような P の $L_1$ の元 $y_1, . . . , y_n$ と元 $z_1, . . . , z_n$ が存在します。 P は K 上で $p$-根なので、K に対して $z^q_1, . . . , z_n^q$ 属するとなるような $p$ の冪 $q$ が存在します。

$$
x^q=\sum_{i=1}^ny^q_i\otimes z_i^q=\sum_{i=1}^ny^q_iz_i^q\otimes 1 =(\sum_{i=1}^ny_iz_i)^q\otimes 1 = 0
$$

したがって、$\mathfrak{b}$ は冪零元で構成されます。

集合 $\mathfrak{c}=\mathfrak{b}\otimes_P\Omega$; $(L_1\otimes P)\otimes_P\Omega$から$P_1\otimes_P\Omega$までは標準準同型の核であり、上記により冪零元で構成されます。ここで、Ω は P の代数閉拡大であり、 $P_1$ は Ω の部分拡張です。 体 P は完全なので、$P_1$ は P の分離拡大 (V, §15, No. 5、p. 125、定理 3) です。 定理によって、可換環 $P_1\otimes_P\Omega$ の最大イデアルのうち V、p. 120、共通部分の 4 が 0 に減ります。他の語、環 $P_1\otimes_P\Omega$ では、次と同型です。 $((L_1\otimes P)\otimes_P\Omega )/\mathfrak{c}$には根基がありません。これは (VIII, p. 155, 命題 5) $\mathfrak{c}$ 含む根基 of 環 $(L_1\otimes P)\otimes_P\Omega$ であることを証明します。さて、この環は$L_1\otimes \Omega$と同型で、$\mathfrak{c}$は冪零元から構成されます。したがって、$L_1\otimes \Omega$の根基は冪零元で構成されます。

C) 特定のケースにおける証明の終わり。 A)とB)により、この可換環の冪零元の集合$\mathfrak{n}$には$L_1\otimes L_2$の根基$\mathfrak{r}$が含まれます。さらに、$\mathfrak{n}$ は $\mathfrak{r}$ (VIII、p. 157、注意 2) に含まれることがわかります。

次に、一般的な場合を考えてみましょう。 半単純可換K-代数は体 K (VIII、p. 137、命題 3) の有限多拡大の積であり、環の積の根基は次のようになります。 根基の積(VIII、p. 156、系3)、$Z_1\otimes Z_2$の根基は、この環の冪零元の集合です。

### 4. 根基/テンソル積/代数

$A_1$ と $A_2$ を K-代数とし、$A = A_1\otimes A_2$ とします。

#### 命題 3 {#alg-viii-s12-prop-3 .statement tag=00EF}

代数 $A_1$ と $A_2$ が半単純で、それぞれ中心 $Z_1$ と $Z_2$ であるとします。 集合 $Z = Z_1\otimes Z_2$。

a) 写像 $\mathfrak{a}\mapsto \mathfrak{a}A$ は、包含順に並べられた Z のイデアルの集合から、包含順に並べられた A の両側イデアルの集合までの同型です。

b) A の根基は、A の最大両側イデアルの共通部分に等しく、$\mathfrak{R}(Z)A$ に等しい。

c) K-代数 $Z_1$ と $Z_2$ の 1 つが分離可能な場合、特に体 K が完全である場合、環 Z と A の根基は 0 に減らされます。

それぞれの代数 $A_i$ は、有限多数の単純代数の積です。さて、環の積の中心は、中心の積であり、根基 (VIII、p. 156、系 3) および両側イデアルの場合、類似の主張が得られます。 (I, §8, No. 10、p. 109、命題 8)。したがって、仮定の下で命題 3 が$A_1$ と $A_2$ が単純代数であることを証明すれば十分です。

$i\in  \{1,2\}$、集合 $B_i= A_i\otimes A^o_i$ について、$A_i$ を $B_i$ 加群として表示します。ここで、相似性は公式で与えられます。

$$
(x\otimes y)z=xzy
$$

$x,y$ と $A_i$ の $z$ です。 $B_i$ 加群 $A_i$ の交換子環は、$Z_i$ の元による相似関数の $(Z_i)_{A_i}$、集合です。私たちは同一視すると $Z_i$ です。さらに、$A_i$の$B_i$部分加群は$A_i$の両側イデアルであり、環$A_i$は単純なので、両側イデアルは0と$A_i$だけです。したがって、$A_i$ は単純な $B_i$ モジュールです。さらに、$A_1\otimes A_2$ の$(B_1\otimes B_2$) サブモジュールは、環 $A_1\otimes A_2$ の両面理想です。

Assertion a) therefore follows from VIII, p. 214, Theorem 2, b) applied to the simple $B_1$-module $A_1$, with commutant $Z_1$, and to the simple $B_2$-module $A_2$, with commutant $Z_2$.

主張 b) を証明しましょう。 A の最大両側イデアルの共通部分は、$(B_1\otimes B_2$) 加群 $A_1\otimes A_2$ の根基です。 系 2 の VIII、p. 215、この共通部分一致すると $\mathfrak{R}(Z)A$ による。 代数 $Z_1$ と $Z_2$ は可換であり、半単純です。したがって、環 Z の根基は冪零元 (VIII、p. 215、定理 3) で構成され、環 A の両側理想$\mathfrak{R}(Z)A$ は根基 $\mathfrak{R}(A)$ に含まれます。 (VIII、p. 157、注意1)。ただし、含む $\mathfrak{R}(A)$ の最大両面理想のうち共通部分 (VIII、p. 155、命題 5、d))。これは主張 b) を証明します。

分離可能な可換代数と還元された可換代数のテンソル積は、還元された環 (V, §15, No. 2、p. 120、命題 5) です。 代数 $Z_1$ と $Z_2$ は可換であり、半単純なので削減されます。 代数 $Z_1$ と $Z_2$ のいずれかが分離可能な場合、代数 Z は減少します。したがって、VIII、p. 215の3つである定理によって根基がなくなり、$\mathfrak{R}(A) =\mathfrak{R}(Z)A = 0$が得られます。これは特に、完全体上のすべての縮小された可換代数が分離可能であるため、体 K が完全である場合に当てはまります (V, §15, No. 5、p. 125、定理 3)。

#### 系 {#alg-viii-s12-n4-cor-1 .statement tag=00EG}

代数 $A_1$ と $A_2$ が単純で、$A_1$ の中心 $Z_1$ が K に還元されるとします。そのとき、環 $A_1\otimes A_2$ には 0 とそれ自体以外の両側イデアルはありません。

仮定までに $Z_1= K$ が得られ、$A_2$ は単純なので、その中心 $Z_2$ は体 (VIII, p. 121, 系 1, a)) になります。したがって、環 $Z = Z_1\otimes Z_2$ は体であり、命題 3 から系が続きます (a)。

### 5. 半単純加群中テンソル積

#### 命題 4 {#alg-viii-s12-prop-4 .statement tag=00EH}

For $i\in  \{1,2\}$, let $A_i$ be K-代数, $M_i$ 半単純 $A_i$-module, and $Z_i$ 中心 of 交換子環 of $M_i$. 集合 $A = A_1\otimes A_2$、$M = M_1\otimes M_2$、$Z = Z_1\otimes Z_2$。 $\mathfrak{R}_A(M) =\mathfrak{R}(Z)M$があります。 If one of 代数 $Z_1$ and $Z_2$ is separable over K, in particular if 体 K is perfect, then A-加群 M is without 根基.

$i\in  \{1,2\}$ について、$S_i$ を単純な $A_i$ モジュール、$D_i$ をその交換子環、$I(i)$ 集合とします。 $M_i$ が $A_i$ モジュール $S_i^{(I(i))}$ である場合から始めます。私たちは交換子環の同一視する中心 $Z_i$ と $D_i$ の中心です。 集合 $D = D_1\otimes D_2$。 $\mathfrak{R}(D) =\mathfrak{R}(Z)D$ (命題 VIII の 3、p. 217) と $\mathfrak{R}_A(S_1\otimes S_2) =$ $\mathfrak{R}(D)(S_1\otimes S_2)$ (VIII、p. 215、系 2) があるため、$\mathfrak{R}_A(S_1\otimes S_2) =\mathfrak{R}(Z)(S_1\otimes S_2)$ となります。 A-加群 M は $S_1\otimes S_2$ と同型の A-加群族の直和であり、加群族の直和の根基は根基の直和 (VIII, p. 152、系 2)。したがって、$\mathfrak{R}_A(M) =\mathfrak{R}(Z)M$ となります。

次に、一般的な場合を考えてみましょう。 $i\in  \{1,2\}$ については、$A_i$ モジュール $M_i$ のサポートを $\mathscr{S}_{M_i}$ で示します。 $\lambda \in \mathscr{S}_{M_i}$ については、型 $\lambda$ の$M_i$ の同型成分を $M_{i;\lambda}$ で表し、その交換子環の中心を $Z_{i;\lambda}$ で表します。私たちは同一視する環 $Z_i$ と環 $Z_{i;\lambda}$ の積で $\lambda \in \mathscr{S}_{M_i}$ です。 $\lambda \in \mathscr{S}_{M_1}$と$\mu\in \mathscr{S}_{M_2}$としましょう。 pr$_{\lambda}\circ i_{\lambda}$が$Z_{1;\lambda}$では恒等写像、pr$_{\lambda'}\circ i_{\lambda}$が$\lambda '\in \mathscr{S}_{M_1}-\{\lambda \}$では零写像となるように、$i_{\lambda}: Z_{1;\lambda}\rightarrow Z_1$一意なK-線型写像で表します。 定義する $i_\mu: Z_{2;\mu}\rightarrow Z_2$ も同様です。 集合 $Z_{\lambda ,\mu}= Z_{1;\lambda}\otimes Z_{2;\mu}$ と $i_{\lambda ,\mu}=i_{\lambda}\otimes i_\mu$ で、写像 pr$_{\lambda}\otimes$ pr$_\mu$ を Z から $Z_{\lambda ,\mu}$ までを $\pi_{\lambda ,\mu}$ で表します。 写像 $\pi_{\lambda ,\mu}$ は全射法環準同型です。従って、$\pi_{\lambda ,\mu}(\mathfrak{R}(Z))\subset \mathfrak{R}(Z_{\lambda ,\mu})$ (VIII, p. 155, 命題 5, b)) となります。逆包含を証明しましょう。 $z$ を $\mathfrak{R}(Z_{\lambda ,\mu})$ の元とします。 $Z_{1;\lambda}$ と $Z_{2;\mu}$ は体であるため、$z$ は無能です (定理 VIII、p. 215 の 3)。 $Z_{\lambda ,\mu}$ の $x, y$ には $i_{\lambda ,\mu}(xy) =i_{\lambda ,\mu}(x)\cdot i_{\lambda ,\mu}(y)$ があります。従って、$i_{\lambda ,\mu}(z)$ はゼロポテントであるため、属するから $\mathfrak{R}(Z)$ になります。 $\pi_{\lambda ,\mu}\circ i_{\lambda ,\mu}$は$Z_{\lambda ,\mu}$の恒等写像なので、元$z$属するから$\pi_{\lambda ,\mu}(\mathfrak{R}(Z))$となります。従って、等式 $\pi_{\lambda ,\mu}(\mathfrak{R}(Z)) =\mathfrak{R}(Z_{\lambda ,\mu})$ が証明されました。

集合 $M_{\lambda ,\mu}= M_{1;\lambda}\otimes M_{2;\mu}$;これは、Z の下で安定している M の部分加群です。$z\in Z$ と $m\in M_{\lambda ,\mu}$ の場合、$zm=\pi_{\lambda ,\mu}(z)m$ になります。従って、$\mathfrak{R}(Z)M_{\lambda ,\mu}$ は $\mathfrak{R}(Z_{\lambda ,\mu})M_{\lambda ,\mu}$ に等しいため、同型の場合では $\mathfrak{R}_A(M_{\lambda ,\mu})$ に等しくなります。 直和の根基は根基の直和(VIII、p. 152、系2)であり、Mは$(\lambda , \mu)\in \mathscr{S}_{M_1}\times \mathscr{S}_{M_2}$の部分加群$M_{\lambda ,\mu}$の直和であるため、 等式 $\mathfrak{R}_A(M) =\mathfrak{R}(Z)M$ が証明されました。 最後の主張は、命題 3 の VIII、p. 217 から続きます。

#### 補題 2 {#alg-viii-s12-lem-2 .statement tag=00EI}

Let $A_1$ and $A_2$ be 代数 over 可換体 K. Let $M_1$ be an $A_1$-module that is finite-dimensional over K and $M_2$ a $A_2$-module of 有限長.次に、$A_1\otimes A_2$ モジュール $M_1\otimes M_2$ には有限長があります。

集合 $M = M_1\otimes M_2$。 $(e_1, . . . , e_n)$ を体 K 上の $M_1$ の基底とします。 写像 $(x_1, . . . , x_n)\mapsto \sum^n_{i=1}e_i\otimes x_i$ は、$A_2$ モジュール $M^n_2$ から $A_2$ モジュール M までの同型です。 $M_2$ は有限長の $A_2$ モジュールであり、M も同様です。さらに、M のすべての A-部分加群は $A_2$ サブモジュールです。従って、M は有限長の A-加群です。

#### 命題 5 {#alg-viii-s12-prop-5 .statement tag=00RC}

$A_1$ と $A_2$ を可換体 K 上の代数とする。 $M_1$ を、K 上の有限次元である半単純 $A_1$ 加群および $M_2$ 半単純 $A_2$ 加群とする。 $i\in  \{1,2\}$ の場合、$A_i$ モジュール $M_i$ の交換子環を $D_i$ で表し、$D_i$ の中心を $Z_i$ で表します。 集合 $A = A_1\otimes A_2$、M = $M_1\otimes M_2,D = D_1\otimes D_2$、および $Z = Z_1\otimes Z_2$。

a) A-加群 M の交換子環は D で識別でき、その中心は Z です。$A_2$ モジュール $M_2$ に有限長がある場合、A-加群 M には有限長があり、環 D は正しく、 左アルティン的、環 Z はアルティンです。

b) 次のプロパティは同等です。

(i) A-加群 M は半単純です。

(ii) 環 Z は、可換体族の積と同型です。

(iii) 環 Z が減少します。

c) 次のプロパティは同等です。

(i) A-加群 M は同型であり、0 に還元されません。

(ii) 環 Z は体です。

(iii) 環 Z は整域です。

By 仮定, $M_1$ is finite-dimensional over K. 交換子環 of M can therefore be identified with D (VIII, p. 213, 補題 1), and its 中心 is Z (III, §4, No. 4, p. 468, 系）。 $A_2$ モジュール $M_2$ に有限長があるとします。 A-加群 M は補題 2 によって有限長になります。$M_2$ は半単純で有限生成されるため、環 $D_2$ は半単純 (VIII, p. 139, 命題 6)、その中心 $Z_2$ は、可換体の有限族の積です。従って、$D_2$ モジュール $(D_2)_s$ と $Z_2$ モジュール $(Z_2)_s$ はそれぞれ有限長を持ちます。さらに、$M_1$ は K 上で有限次元であるため、$D_1$ と $Z_1$ も有限次元です。 補題 2 までに、加群 $(D_1\otimes D_2)_s$ は有限長になります。従って、環 $D_1\otimes D_2$ は左アルティン的です。同様に、環 $D_1\otimes D_2$ は右アルティンであり、環 $Z_1\otimes Z_2$ はアルティンであることを証明します。 主張 a) が続きます。

b)を証明しましょう。 半単純加群の交換子環の中心は、可換体 (VIII, p. 87, 命題 8, a)) の族の積と同型です。これは、(i) が (ii) を意味することを証明します。 (ii) $\Rightarrow$ (iii) の意味は明らかです。

環 Z が減少するとします。次に、$\mathfrak{R}(Z) = 0$ (VIII, p. 215, 定理 3) と $\mathfrak{R}_A(M) = 0$ (VIII, p. 218, 命題 4) があります。 $A_2$ モジュール $M_2$ は半単純であるため、単純な $A_2$ モジュールのファミリー $(S_i)_{i\in I}$ と $M_2$ から $\bigoplus S_i$ までの同型が存在します。従って、A-加群 M は $\bigoplus M_1\otimes S_i$ と同型です。従って、すべての $i\in I$ に対して、A-加群 $M_1\otimes S_i$ には根基がありません。 a) により、有限長になります。従って、それは半単純 (VIII, p. 153, 命題 3, b)) です。 A-加群 M は、半単純加群の家族の直和となり、その結果、半単純になります。これは、(iii) が (i) と b) の結論する証明を意味することを証明します。

A-加群は同型であり、半単純であり、その交換子環の中心が体 (VIII, p. 87, 命題 8, b)) である場合に限り、非零となります。従って、b) から c) が導かれます。

#### 系 {#alg-viii-s12-n5-cor-1 .statement tag=00EJ}

$Z_1$ または $Z_2$ が体 K 上の分離可能な代数である場合 (たとえば、K が完全な場合)、A-加群 $M_1\otimes M_2$ は半単純です。

環 $Z_1$ と $Z_2$ は体の積と同型であるため、縮小された環です。特に、K が完全であれば、それらは K 上で分離可能です代数 (V, §15, No. 5, p. 125, 定理 3)。 命題により、分離可能な代数と縮小された代数の V, §15, No. 2、p. 120、テンソル積の 5 が縮小されます。従って、Z は縮小された環であり、系は命題 5 から続きます (b)。

### 6. テンソル積/半単純代数

#### 命題 6 {#alg-viii-s12-prop-6 .statement tag=00EK}

$A_1$ と $A_2$ を非零 K-代数とします。 環 $A_1\otimes A_2$ が単純 (それぞれ半単純) である場合、環 $A_1$ と $A_2$ は単純 (それぞれ半単純) です。

環 B は、B-加群 $B_s$ が半単純 (それぞれ等型および非零) である場合に限り、半単純 (それぞれ単純) です。従って、命題は命題 1 (VIII, p. 211) から続きます。

#### 命題 7 {#alg-viii-s12-prop-7 .statement tag=00EL}

$A_1$ と $A_2$ を半単純 K-代数とし、それぞれ中心 $Z_1$ と $Z_2$ とします。 $A_1$ が K に対して有限次数を持っているとします。その場合、環 $A_1\otimes A_2$ は左アルティン的であり、その中心 $Z_1\otimes Z_2$ も同様です。 環 $A_1\otimes A_2$ は、環 $Z_1\otimes Z_2$ が体 (または縮小された環) である場合に限り、単純です (または半単純)。

これは、VIII、p. 219の命題5の$M_1= (A_1)_s, M_2= (A_2)_s$の場合です。

#### 系 1 {#alg-viii-s12-prop-7-cor-1 .statement tag=00EM}

$A_1$ と $A_2$ を半単純 K-代数とします。 $A_1$ が K 上で有限次元であるとします。 $A_1$ または $A_2$ の中心が K 上で分離可能な代数であるとします。これは、たとえば K が完全な場合です。すると$A_1\otimes A_2$は半単純になります。

これは、VIII、p. 221の系の$M_1= (A_1)_s, M_2= (A_2)_s$の場合です。

#### 系 2 {#alg-viii-s12-prop-7-cor-2 .statement tag=00RD}

$A_1$ と $A_2$ を単純K-代数とします。 $A_1$ が K 上の有限次元であるとします。 $A_1$ または $A_2$ の中心が K に等しい場合、代数 $A_1\otimes A_2$ は単純です。これは特に、K が代数的に閉じている場合に当てはまります。

$A_1$ と $A_2$ の中心 $Z_1$ と $Z_2$ は、それぞれ体です。 環 $Z_1$ と $Z_2$ のいずれかが K に等しい場合、環 $Z_1\otimes Z_2$ は体になります。従って、命題を適用する 7 で十分です。

体 K が代数的に閉じている場合、$A_1$ の中心は K に等しくなります。

### 7. 半単純加群のスカラーの拡大

#### 命題 8 {#alg-viii-s12-prop-8 .statement tag=00EN}

A を体 K の K-代数、M A-加群、および L 拡大とします。M の交換子環を D で表し、D の中心を Z で表します。

a) $A_{(L)}$ モジュール $M_{(L)}$ が単純であると仮定します (それぞれ同型、半単純)。この場合、A-加群 M は単純です (それぞれ同型、半単純)。

b) A-加群 M が半単純で、M または L が K 上の有限次元であると仮定します。$A_{(L)}$ 加群 $M_{(L)}$ は、環 $Z_{(L)}$ が縮小された場合に限り、半単純になります。 $A_{(L)}$ モジュール $M_{(L)}$ は同型であり、環 $Z_{(L)}$ が整域である場合に限り、非零になります。

c) A-加群 M が単純であると仮定します。 $A_{(L)}$加群 $M_{(L)}$ は、環 $D_{(L)}$ が半単純 (それぞれ単純、体) である場合に限り、 半単純 (それぞれ同型、単純) です。

主張 a) は命題 1 (VIII、p. 211) の特定のケース、主張 b) は命題 5 (VIII、p. 219) の特定のケース、主張 c) は特定のケースです系 VIII、p. 215 の 1。

#### 系 1 {#alg-viii-s12-prop-8-cor-1 .statement tag=00EO}

a) A-加群 M が半単純、K の拡大 L が分離可能、M または L が K 上で有限次元であると仮定します。そのとき、$A_{(L)}$ 加群 $M_{(L)}$ は半単純です。

b) A-加群 M が単純で、その交換子環が K に等しいと仮定します。その場合、$A_{(L)}$ 加群 $M_{(L)}$ は単純です。

主張 a) は、系 VIII、p. 221 から続きます。 主張 b) は、命題 8、c) の特殊なケースです。

#### 系 2 {#alg-viii-s12-prop-8-cor-2 .statement tag=00RE}

L を体 K の拡大とします。 K-代数 A の中心を Z で表します。

a) L-代数$A_{(L)}$ が半単純である場合、K-代数 A は半単純です。

b) K-代数 A が半単純で、L または A が K 上の有限次元であると仮定します。L-代数 $A_{(L)}$ は、環 $Z_{(L)}$ が縮小される場合に限り、半単純になります。これは、特に、L が K の分離拡大である場合に当てはまります。L-代数 $A_{(L)}$ は、環 $Z_{(L)}$ が整域である場合にのみ単純です。これは特に、A の中心が K に等しい場合に当てはまります。

主張 a) および b) は、命題 8 から続き、a) および b) が A-加群 $A_s$ に適用されます。

#### 命題 9 {#alg-viii-s12-prop-9 .statement tag=00EP}

A を K の K-代数と L 分離拡大とします。

a) M が根基なしで A-加群である場合、$A_{(L)}$ モジュール $M_{(L)}$ には根基がありません。

b) K-代数 A に根基がなければ、L-代数 $A_{(L)}$ には根基がありません。

主張 a) を証明しましょう。 M を根基なしで A-加群とします。私たちは$M_{(L)}$の標準像を持つ同一視するMです。 NをMの極大部分加群とします。A-加群$M/N$は単純なので、VIII、p. 218の命題4から、$A_{(L)}$モジュール$(M/N)_{(L)}= M_{(L)}/N_{(L)}$には根基が存在しないことがわかります。 $\mathfrak{R}_{A_{(L)}}(M_{(L)})\subset N_{(L)}$ by 系 1、c) の VIII、p. 152。さて、II, §7, No. 7の14、p. 306の命題の系から、NがMの極大部分加群の集合を通る$N_{(L)}$の共通部分が0に減らされます。 $A_{(L)}$-モジュール $M_{(L)}$ には根基がありません。

主張 b) は、主張 a) からA-加群 $A_s$ に適用されます。

#### 命題 10 {#alg-viii-s12-prop-10 .statement tag=00EQ}

A を K の K-代数と L 拡大とします。M を A-加群とします。

a) 次の 2 つのうちの 1 つを作成します仮定:

(i) A-加群 M は有限生成され、L は K に対する代数的です。

(ii) 環 A は左アルティン的です。

次に、インクルージョンがあります

$$
\mathfrak{R}_A(M)_{(L)}\subset \mathfrak{R}_{A_{(L)}}(M_{(L)})
$$

b) L が K の分離拡大である場合、次の包含が得られます。

$$
\mathfrak{R}_{A_{(L)}}(M_{(L)})\subset \mathfrak{R}_A(M)_{(L)}
$$

主張 a) を証明しましょう。ケース (i) を考えてみましょう。まず、L が K に対して有限次数を持っているとします。すると、A-加群 $M_{(L)}$ が有限生成されます。 標準準同型 A から $A_{(L)}$ を $f$ で表します。 環 $A_{(L)}$ は、中心と $f(A)$ の和集合によって生成されます。従って、VIII、p. 174 を $A_{(L)}$ モジュール $M_{(L)}$ に命題を適用する 3 することができます。これにより、包含 $\mathfrak{R}_A(M_{(L)})\subset \mathfrak{R}_{A_{(L)}}(M_{(L)})$ およびなおさら $\mathfrak{R}_A(M)_{(L)}\subset \mathfrak{R}_{A_{(L)}}(M_{(L)})$ (VIII、p. 152、系 1) が得られます。

ここで一般的なケースを扱いましょう。 $x_1, . . . , x_n$ を生成する A-加群 M と $\mathfrak{R}_A(M)$ の $x$ 元を元とします。 $a_1, . . . , a_n$ を $A_{(L)}$ の元とします。 L は K 上の代数であるため、$a_i$ 属するから $A_{(L')}$ となるような、L に含まれる K の有限拡大 $L'$ が存在します。上記により、$A_{(L')}$-モジュール$M_{(L')}$の$x$属するから根基; VIII、p. 153の系から、$1\leqslant i\leqslant n$生成するの$A_{(L')}$モジュール$M_{(L')}$、従って$A_{(L)}$モジュール$M_{(L)}$の元$x_i+a_ix$が続きます。 $A_{(L)}$ モジュール $M_{(L)}$ の系、$x$ 属する ～ 根基も同様です。

次に、ケース(ii)について考えてみましょう。 $\mathfrak{r}$ を A の根基とすると、A-加群 M の根基は $\mathfrak{r}M$ (VIII, p. 174, 系) と等しくなります。 A の根基 $\mathfrak{r}$ は、A の冪能の両面イデアル (VIII、p. 173、命題 1) です。従って、$\mathfrak{r}_{(L)}$ は、$A_{(L)}$ の零無能の両面イデアルです。従って、$\mathfrak{r}_{(L)}\subset \mathfrak{R}(A_{(L)})$ (VIII、p. 156、定理 1)、VIII、p. 158 の命題 6 は $\mathfrak{R}(A_{(L)})M_{(L)}\subset \mathfrak{R}_{A_{(L)}}(M_{(L)})$ を意味します。従って、主張 a) の結論する証明は $\mathfrak{R}_A(M) =\mathfrak{r}M\subset$ $\mathfrak{R}_{A_{(L)}}(M_{(L)})$ となります。

加群 $M/\mathfrak{R}_A(M)$ には根基がありません。 L が K の分離拡大である場合、VIII、p. 223 の命題 9 から、$A_{(L)}$ モジュール $(M/\mathfrak{R}_A(M))_{(L)}$ には根基が含まれていないことがわかります。従って、次の内容が含まれます。

$$
\mathfrak{R}_{A_{(L)}}(M_{(L)})\subset \mathfrak{R}_A(M)_{(L)}
$$

#### 系 {#alg-viii-s12-n7-cor-1 .statement tag=00ER}

L を K の分離拡大とします。L が K 上の代数であるか、環 A が左アルティン的である場合、$\mathfrak{R}(A_{(L)}) =$ $\mathfrak{R}(A)_{(L)}$ が得られます。

これは、命題 10 の $M = A_s$ の場合です。

### 練習問題 {#alg-viii-s12-exercises}

[§ 12 に対して練習問題](exercises/s12/)を参照してください。
