---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: IX
chapter_title: COMPACT REAL LIE GROUPS
section: 7
section_title: Irreducible representations of connected compact Lie groups
lang: ja
source: lie-vii-ix
book_pages: 347-359, 414-417
pdf_pages: 0354-0366, 0421-0424
extraction: native
subsections:
    - "no": 1
      title: DOMINANT CHARACTERS
      page: 347
      pdf_page: 354
    - "no": 2
      title: HIGHEST WEIGHT OF AN IRREDUCIBLE REPRESENTATION
      page: 348
      pdf_page: 355
    - "no": 3
      title: THE RING R(G)
      page: 351
      pdf_page: 358
    - "no": 4
      title: CHARACTER FORMULA
      page: 353
      pdf_page: 360
    - "no": 5
      title: DEGREE OF IRREDUCIBLE REPRESENTATIONS
      page: 356
      pdf_page: 363
    - "no": 6
      title: CASIMIR ELEMENTS
      page: 358
      pdf_page: 365
statements: 28
exercises: 8
content_sha256: 587bcfc6330493e950df925747e44c413a8fb83c72fa4d850cba9caf2dde4d5f
translated_from: content/en/lie/IX/07_s7_irreducible_representations_of.md
translation_method: google
source_content_sha256: 375df81cdee840da6e0b458ac2f5db5264d7654fce07a342d3dce277a3f78519
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: 3766b0d32d2d27ec18ed31c845cd2170a01a141fbca602a3446816caa04e69d9
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## § 7。 コンパクト・リー群の既約表現

§6 の記法を保持します。 G の表現は、G から群 $\mathbf{G}\mathbf{L}(V)$ までの連続 (したがって解析的) 準同型で、V は有限次元複素数ベクトル空間です。 G のすべての表現は半単純 (§1, no. 1) です。

$\mathfrak{t}($§5, no. 2の選ぶチャンバーC)、$\Gamma (T)_{++}=\overline{C}\cap \Gamma (T)$を置きます。

### 1. ドミナント指標

元 $\lambda$ の X(T) の $X_+$ 集合で、すべての $x\in \Gamma (T)_{++}$ に対して $\langle \lambda , x\rangle  \geq 0$、つまり線型形式 $\delta (\lambda ) :\mathfrak{t}_{\mathbf{C}}\rightarrow \mathbf{C}$ 写像がチャンバー C となるように表します。 $\mathfrak{t}$から$i\mathbf{R}_+$まで。

X(T) に、正の元が $X_+$ の順序である群構造を与えます。 $R_+= R(G,T)\cap X_+$と$R_-=-R_+$を入れます。 The elements of $R_+$ are called positive roots, those of $R_-$ negative roots; every root is either positive or negative (Chap. VI, §1, no. 6, Th. 3). 2 つの正の根の合計ではない正の根は単純であると言われます。すべての正の根は単純な根の合計です (前述)。単純なルートは、ルートによって生成された X(T) のサブグループの基礎を形成します。このサブグループは、$X(T/C(G))$ (§4, no. 4) で識別できます。単純根に関する反射によりワイル群 $W = W_G(T)$ が生成されます (第 2 章、VI, §1, no. 5)。

#### 補題 1 {#lie-ix-s7-lem-1 .statement tag=01FZ}

$\lambda$をX(T)の元とします。次の条件は同等です。

(i) $w\not= 1$ のようなすべての $w\in W$ に対して $\lambda -w(\lambda )\geq 0$ (それぞれ $>0$)。

(ii) $w\not= 1,\lambda -w(\lambda )$ が線形結合であり、単純な根の正の係数 (それぞれ正の係数がすべての零ではない) であるすべての $w\in W$ について。

(iii) 根 $\alpha$ の陽性ごとに $\langle \lambda , K_{\alpha}\rangle  \geq 0$ (それぞれ $>0$)。

(iv) 単純な根 $\alpha$ ごとに $\langle \lambda , K_{\alpha}\rangle  \geq 0$ (それぞれ $>0$)。

同値 (iii) と (iv) が明らかの場合。 $K_{\alpha}$ の集合は $R(G,T) ($§4, no. 5 の逆数根系と識別できるため、(i) と (iii) の同値は第 4 章から続きます。 VI, §1, no. 6、提案 18 および修正含意 (ii) $\Rightarrow$ (i) は自明であり、逆の含意が loc から得られます。引用。

すべての正の根 $\alpha$ に対して $\langle \lambda , K_{\alpha}\rangle  \geq 0$ となるような X(T) の要素の集合を $X_{++}$ で表します。 $X_{++}$ の元が優勢であると言われています。 それらは、X(T) (第 VI, §1, no. 10 章) における W の操作の基本的な領域を形成します。 $X_{++}\subset X_+$ があります。

G が単純接続されている場合、各単純根 $\alpha$ に対して、X(T) の元 $\varpi_{\alpha}$ が存在し、すべての単純根 $\beta$ に対して $\langle \varpi_{\beta}, K_{\alpha}\rangle =\delta_{\alpha \beta}$、つまり、すべての単純に対して $s_{\alpha}(\varpi_{\alpha}) =$ $\varpi_{\alpha}-\alpha ,s_{\beta}(\varpi_{\alpha}) =\varpi_{\alpha}$ が存在します。 根 $\beta \not=\alpha$; $\varpi_{\alpha}$ はファンダメンタルドミナント重みと呼ばれます。それらは可換群 X(T) と可換モノイド $X_{++}$ の形基底です。より正確には、X(T) のすべての元 $\lambda$ は形 $\lambda =\sum_{\alpha}\langle \lambda , K_{\alpha}\rangle \varpi_{\alpha}$ に書き込むことができます。

次のような $X(T)\otimes \mathbf{Q}$ の $\rho$ 元で表します。

$$
2\rho =\sum_{\alpha\in R_+}\alpha
$$

すべての単純な根 $\alpha$ に対して $\langle \rho , K_{\alpha}\rangle = 1$ があります (章 VI, §1, no. 10、提案 29)。 G が単純接続されている場合、$\rho$ は基本ドミナント重みの和です。

### 2. 既約表現中最高重量

Associate to any representation $\tau : G\rightarrow \mathbf{G}\mathbf{L}(V)$ the homomorphism $L(\tau )_{(\mathbf{C})}$ from the $\mathbf{C}$-Lie algebra $\mathfrak{g}_{\mathbf{C}}$ to End(V) extending the linear representation $L(\tau )$ of $\mathfrak{g}$ on the real vector space underlying V (Chap. III, §3, no. 11). §4, no. 3の提案7により、X(T)からHom$_{\mathbf{C}}(\mathfrak{t}_{\mathbf{C}},\mathbf{C}) =\mathfrak{t}^*_{\mathbf{C}}$への写像$\delta$は、Tに対する$\tau$の重みの集合から$\mathfrak{g}_{\mathbf{C}}$のカルタン部分代数$\mathfrak{t}_{\mathbf{C}}$に対する$L(\tau )_{(\mathbf{C})}$の重みの集合への全単射を引き起こします。

#### 補題 2 {#lie-ix-s7-lem-2 .statement tag=01G0}

$\varphi$ を有限次元複素数ベクトル空間 V 上の複素数リー代数 $\mathfrak{g}_{\mathbf{C}}$ の線型表現とします。 V に G の表現 $\tau$ が存在し、$\varphi$ が半単純であり、V 属するから $\delta (X(T))$ に$\mathfrak{t}_{\mathbf{C}}$ の重みが存在する場合に限り、$L(\tau )_{(\mathbf{C})}=\varphi$ が存在します。

$L(\tau )_{(\mathbf{C})}=\varphi$ のような G の表現 $\tau$ が存在する場合、G は接続されており、$\tau$ は半単純であるため、$\varphi$ は半単純であり (提案 13 のIII, §6, no. 5、Cor. 2)、V 上の $\mathfrak{t}_{\mathbf{C}}$ の重みは次のイメージに属します。 $\delta$。 したがって、条件が必要です。それが十分であることを証明します。 $\varphi$ が準単純の場合、V は $V_\mu(\mathfrak{t}_{\mathbf{C}})$ の直接和であり、$\mu$ はV の$\mathfrak{t}_{\mathbf{C}}$ の重みのセットに属します (Th. 2 のVII, §2, no. 4 章、コリント 3)。すべての重みが $\delta$ の画像に属する場合、V 上に $L(\tau_T)_{(\mathbf{C})}=\varphi |\mathfrak{t}_{\mathbf{C}}:$ となるような T の表現 $\tau_T$ が存在します。実際、$t\in T$ と $v\in V_{\delta(\lambda)}(\mathfrak{t}_{\mathbf{C}})$ に $\tau_T(t)v=t^{\lambda}v$ を置くだけで十分です。 補題は、§2, no. 6 の提案 8 に従っています。

#### 定理 1 {#lie-ix-s7-thm-1 .statement tag=01G1}

a) $\tau : G\rightarrow \mathbf{G}\mathbf{L}(V)$ を G の既約表現とします。すると、$\tau$ の重みの集合 (T に対して) は最大の元 $\lambda$ が優勢で、空間 $V_{\lambda}(T)$ は次元になります。 1.

b) G の 2 つの既約表現は、それらの最高重量が等しい場合にのみ等価です。

c) X(T) のすべてのドミナント元 $\lambda$ に対して、最高重量 $\lambda$ の G の既約表現が存在します。

補題 2、G 対応するの既約表現の同値類によって、有限次元の類 $\mathfrak{g}$ の既約表現が重み属するから$\delta (X(T))$ になります。

$\mathscr{C}\mathfrak{g}_{\mathbf{C}}$ 中心と、$\mathfrak{g}_{\mathbf{C}}$ の導出リー代数を $\mathscr{D}\mathfrak{g}_{\mathbf{C}}$ で表し、$\mathfrak{g}_{\mathbf{C}}=\mathscr{C}\mathfrak{g}_{\mathbf{C}}\oplus \mathscr{D}\mathfrak{g}_{\mathbf{C}}$ とします。 $\mathfrak{t}_{\mathbf{C}}\cap \mathscr{D}\mathfrak{g}_{\mathbf{C}}$ 上のすべての双線形形式 $\mu$ を、第 4 章で導入された単純な $\mathscr{D}\mathfrak{g}_{\mathbf{C}}$ モジュールを $E(\mu)$ で表します。 VIII, §6, no. 3; $\mathscr{C}\mathfrak{g}_{\mathbf{C}}$ 上のすべての線型形式 $\nu$ について、それに関連付けられた $\mathbf{C}$ 上の 1 次元 $\mathscr{C}\mathfrak{g}_{\mathbf{C}}$ モジュールを $\mathbf{C}(\nu )$ で示します。 次に、$\mathfrak{g}_{\mathbf{C}}$ モジュール $\mathbf{C}(\nu )\otimes E(\mu)$ は単純です。 VIII, §7, no. 2、コル。 Thの2。 1 および代数、第 1 章VIII, §11, no. 1、木曜日。 1、すべての有限次元の単純な $\mathfrak{g}_{\mathbf{C}}$ 加群は加群 $\mathbf{C}(\nu )\otimes E(\mu)$ のいずれかと同型です。さらに、(前述)$\mathbf{C}(\nu )\otimes E(\mu)$ は、すべての単純な根 $\alpha$ に対して $\mu(H_{\alpha})$ が正の整数である場合に限り、有限次元になります。 $\mathfrak{t}_{\mathbf{C}}$ の $\nu +\mu$ 線型形式で、$\mathscr{C}\mathfrak{g}_{\mathbf{C}}$ の誘導する $\nu$ と $\mathfrak{t}_{\mathbf{C}}\cap \mathscr{D}\mathfrak{g}_{\mathbf{C}}$ の $\mu$ を表すと、$(\nu +\mu)(H_{\alpha}) =\mu(H_{\alpha})$ になります。さらに、$\mathbf{C}(\nu )\otimes E(\mu)$の重みは$\nu +\lambda$で、$\lambda$は$E(\mu)$の重みであり、したがって、$\theta \in \delta (X_+)$を伴う形$\nu +\mu-\theta$になります（VIII, §6, no. 2章、 補題 2）。

$\mathfrak{g}$加群$\mathbf{C}(\nu )\otimes E(\mu)$は、$(\nu +\mu)(H_{\alpha})$がすべての単純根$\alpha$に対して正の整数である場合に限り有限次元であり、$\nu +\mu$が$\delta (X(T))$に属する場合に限り、その重みは$\delta (X(T))$に属すると結論付けます。 これら 2 つの条件の結合は、$\nu +\mu$ 属するから $\delta (X_{++})$ を意味します。その場合、$\nu +\mu$は$\mathbf{C}(\nu )\otimes E(\mu)$の最高重量です。 したがって、最高重量 $\lambda$ の G の X(T) 既約表現のすべてのドミナント重み $\lambda$ について構築し、同値までの G のすべての既約表現を取得しました。 次元1の$\mathbf{C}(\nu )\otimes E(\mu)$形部分空間の重み$\nu +\mu$のベクトルなので、証明が完成です。

#### 系 {#lie-ix-s7-n2-cor-1 .statement tag=01G2}

群 G には (有限次元の) 忠実な線型表現があります。

まず、X(T) のすべての元が 2 つの支配的な重みの差に等しいことに注目してください。より正確には、$\varpi$ を $X_{++}$ の元とし、すべての単純な根 $\alpha$ に対して $\langle \varpi , K_{\alpha}\rangle >0$ とします。すべての $\lambda \in X(T)$ に対して、正の整数 $n$ が存在し、すべての単純な根 $\alpha$ に対して $\langle \lambda +n\varpi , K_{\alpha}\rangle  \geq 0$、つまり (no. 1, 補題 $1$)$\lambda +n\varpi \in X_{++}$ が存在します。

その結果、$X_{++}$ 生成するの $\mathbf{Z}$ 加群 X(T) の元の有限族 $(\lambda_i)_{i\in I}$ が存在します。 $i\in I$ について、$\tau_i$ を最高重量 $\lambda_i$ (Th. 1) の G の既約表現とします。 表現 $\tau$ を $\tau_i$ の直和とします。 構成集合 $P(\tau ,T)$ の重みの $\tau$ (T に対して) 生成するにより、$\mathbf{Z}$ モジュール X(T)。 §4, no. 3 の提案 6 から、準同型 $\tau$ は単射法であるため、系になります。

#### 注意 1 {#lie-ix-s7-n2-rem-1 .statement tag=01G3}

$\mathfrak{n}_+$ を $\mathfrak{g}_{\mathbf{C}}$ の部分代数 、つまり $\alpha  >0$ の $\mathfrak{g}^{\alpha}$ の和とします。 $\tau : G\rightarrow \mathbf{G}\mathbf{L}(V)$ を既約表現、$\lambda \in X_{++}$ をその最高重量、$\tau ':\mathfrak{g}_{\mathbf{C}}\rightarrow \mathfrak{g}\mathfrak{l}(V)$ 表現を $\tau$ によって誘発するとします。次に、$V_{\lambda}(T)$ は、V のベクトル $v$ の部分空間からなるとなり、すべての $x\in \mathfrak{n}_+$ に対して $\tau '(x)v= 0$ になります。

Indeed, this follows from the corresponding statement for the $\mathfrak{g}_{\mathbf{C}}$-modules $\mathbf{C}(\nu )\otimes E(\mu)$ (Chap. VIII, §6, no. 2, Prop. 3).

#### 注意 2 {#lie-ix-s7-n2-rem-2 .statement tag=01G4}

$\Theta (G)$ を、$\mathbf{C}($代数の値を持つ G 上の連続代表写像の代数とします。 VIII）。 G を左右の平行移動によって $\Theta (G)$ に作用させます。 For each $\lambda \in X_{++}$, let $(V_{\lambda}, \tau_{\lambda})$ be an irreducible representation of G of highest weight $\lambda$ (Th. 1), and $(V^*_{\lambda},\check{\tau}_{\lambda})$ the contragredient representation (Chap. III, §3, no. 11); by Spectral Theories, the representation of $G\times G$ on $\Theta (G)$ is isomorphic to the direct sum of the representations $(V_{\lambda}\otimes V^*_{\lambda}, \tau_{\lambda}\otimes \check{\tau}_{\lambda})$ for all $\lambda$ in $X_{++}$. Remark 1 now implies the following statement: Let $\lambda \in X_{++}$, and let $E_{\lambda}$ be the vector subspace of $\Theta (G)$ consisting of the continuous representative functions $f$ on G such that $f(gt) =\lambda (t)^{-1}f(g)$ for all $g\in G$ and all $t\in T$, and such that $f*x= 0$ for all $x\in \mathfrak{n}_-=\bigoplus_{\alpha <0}\mathfrak{g}^{\alpha}$.

この場合、$E_{\lambda}$ は左変換の下で安定であり、左変換による $E_{\lambda}$ 上の G の表現は最高重量 $\lambda$ の既約です。

#### 注意 3 {#lie-ix-s7-n2-rem-3 .statement tag=01G5}

$\tau : G\rightarrow \mathbf{G}\mathbf{L}(V)$を既約表現とします。すべての $s\in C(G), v\in V:$ に対して $\tau (s)v=\nu (s)v$ となるような X(C(G)) の元 $\nu$ が存在します。実際、$\tau (C(G))$ は $\tau$(G) の交換子環に含まれており、これは次と等しくなります。 $\mathbf{C}^*.1_V($代数、章。 VIII, §3, no. 2、木曜日。 1)。 $\tau$ の重み $\lambda$ ごとに、$\lambda$ から C(G) の制限は $\nu$ に等しくなります。

#### 注意 4 {#lie-ix-s7-n2-rem-4 .statement tag=01G6}

第 2 章の定義と主張 VIII, §7、いいえ。 2 ～ 5 は現在の状況に問題なく一般化できます。詳細は読者にお任せします。

#### 命題 1 {#lie-ix-s7-prop-1 .statement tag=01G7}

$\tau : G\rightarrow \mathbf{G}\mathbf{L}(V)$ を最高重量 $\lambda \in X_{++}$ の G の既約表現とします。 $m$ を整数 $\sum_{\alpha\in R_+}\langle \lambda , K_{\alpha}\rangle$ とし、$w_0$ とします

$w_0(R_+) = R_-$ となるようなワイル群の元 (提案 17 のVI, § 6 章、コリント 3)。考えられるケースは次の 3 つです。

a$)w_0(\lambda ) =-\lambda$ と $m$ は偶数です。この場合、V 上で対称双線形形式を分離する G 不変量が存在します。 表現 $\tau$ は実際の型 (付録 II) です。

b$)w_0(\lambda )\not=-\lambda$。 V 上のすべての G 不変双線形形式は零です。 表現 $\tau$ は複素数型です (前述)。

c$)w_0(\lambda ) =-\lambda$ と $m$ は奇数です。次に、V 上で交代的双線形形式を分離する G 不変式が存在します。 表現 $\tau$ は四元数の型 (上記参照)。

$\tau$ から $C(G)_0$ の制限が自明でない場合、ケース b) になります。

V 上の双線形形式 B は、$\mathfrak{g}_{\mathbf{C}}$ のもとで不変である場合に限り、G のもとでも不変です (III, §6, no. 5 章、コリント 3)。したがって、G が半単純の場合、第 4 章から命題が続きます。 VIII, §7, no. 5、付録 II の提案 12 および提案 3。

一般的なケースでは、X(T) の部分群に $C(G)_0= S$ と同一視する $X(T/S)$ を置きます (W で安定)。 最高重量 $\lambda$ の商表現 $\tau ': G/S\rightarrow \mathbf{G}\mathbf{L}(V)$ に$\tau (S) =\{1_V\},\tau$ 誘導するの場合。この場合、命題は前述の結果に従い、$G/S$ に適用されます。

$\tau (S)\not=\{1_V\}$ と仮定します。すべての $s\in S$ (注意 3) に対して $\tau (s) =\nu (s)_V$ となるような X(S) の非ゼロ元 $\nu$ が存在します。すると、$\nu$ は制限準同型 $X(T)\rightarrow X(S)$ の下の $\lambda$ の像になります。 W は X(S) で自明に動作するため、等式 $w_0(\lambda ) =-\lambda$ は $\nu =-\nu$ を意味しますが、これは不可能です。したがって、$w_0(\lambda )\not=-\lambda$ になります。一方、B が V 上の G 不変双線形形式である場合、V のすべての $x, y$ と S の $s$ について、

$$
B(\nu (s)x, \nu (s)y) = B(x, y) =\nu (s)^2B(x, y)
$$

これは、B = 0、つまり命題を意味します。

$\mathfrak{S}_{\mathbf{R}}(G)$ を有限次元実数ベクトル空間上の G の既約連続表現の類の集合とする。提案 1 と付録 II の結果は全単射 $\Phi : X_{++}/\Sigma \rightarrow \mathfrak{S}_{\mathbf{R}}$(G) を与えます。ここで、$\Sigma$ は Aut(X(T)) の部分群 $\{1,-w_0\}$ を表します。より正確には、$\lambda \in X_{++}$ を $E_{\lambda}$ を最高重量 $\lambda$ の G の表現とします。それから

$\lambda \not=-w_0(\lambda )$ の場合、または $\sum_{\alpha\in R_+}\langle \lambda , K_{\alpha}\rangle \notin2\mathbf{Z}$ の場合、$\Phi (\{\lambda ,-w_0(\lambda )\}) = E_{\lambda[\mathbf{R}]}$

$\lambda =-w_0(\lambda )$ と $\sum_{\alpha\in R_+}\langle \lambda , K_{\alpha}\rangle  \in 2\mathbf{Z}$ の場合は $\Phi (\{\lambda ,-w_0(\lambda )\}) = E'_{\lambda}$

ここで、$E'_{\lambda}$ は G の下での不変式である $E_{\lambda}$ 上の $\mathbf{R}$ 構造です。

### 3. 環 R(G)

R(G) を G (代数、第 VIII, §10, no. 6) の表現 (連続、有限次元複素数ベクトル空間上) の環とします。 $\tau$ が G の表現である場合、R(G) の類を $[\tau ]$ で表します。 $\tau$ と $\tau '$ が G の 2 つの表現である場合、定義までに、

$$
[\tau ] + [\tau '] = [\tau \oplus \tau ']
$$

$$
[\tau ][\tau '] = [\tau \otimes \tau ']
$$

G のすべての表現は半単純であるため、$\mathbf{Z}$ 加群 R(G) は自由であり、G の既約表現のクラスの集合、つまり Th によって $X_{++}$ と識別できる集合を基礎として認めます。 1. The map $\tau  \rightarrow L(\tau )_{(\mathbf{C})}$ induces a homomorphism $l$ from the ring R(G) to the ring $\mathscr{R}(\mathfrak{g}_{\mathbf{C}})$ of representations of $\mathfrak{g}_{\mathbf{C}}$ (Chap. VIII, §7, no. 6).

$\tau : G\rightarrow \mathbf{G}\mathbf{L}(V)$ を G の表現とします。 $\mathbf{C}$ベクトル空間Vの階調$(V_{\lambda}(T))_{\lambda\in X(T)}$を考えます。 Ch(V)、または等級付けされたベクトル空間 V (第 VIII, §7, no. 7) の Ch($\tau$ )、指標で表します。 $(e^{\lambda})_{\lambda\in X(T)}$ が代数 $\mathbf{Z}[X(T)] =\mathbf{Z}^{(X(T))}$ の標準基底を表す場合、定義までに、

Ch($\tau$ ) $=\sum_{\lambda\in X(T)}$(薄暗い $V_{\lambda}(T)$)$e^{\lambda}$。

同じ方法で定義する (前述) 環の準同型 (これも Ch で表されます) を R(G) から $\mathbf{Z}[X(T)]$ まで実行します。 G が半単純の場合、可換図式が得られます。

R(G) $\longrightarrow^{Ch}\mathbf{Z}[X(T)]$

$$
_{l\widetilde{\delta}} \tag{1}
$$

$$
\mathscr{R}(\mathfrak{g}_{\mathbf{C}})\longrightarrow^{ch}\mathbf{Z}[P]
$$

ここで、P は、$R(\mathfrak{g}_{\mathbf{C}},\mathfrak{t}_{\mathbf{C}})$ と $\delta$ によって引き起こされる準同型性の$\widetilde{\delta}$ の重みのグループを表します。

ワイル群 W は群 X(T) の自己同型によって動作し、したがって環 $\mathbf{Z}[X(T)]$ に動作します。 §4, no. 3 の提案 5 により、Ch の像は W の下で元の不変式の部分環 $\mathbf{Z}[X(T)]^W$ からなるに含まれます。

#### 命題 2 {#lie-ix-s7-prop-2 .statement tag=01G8}

準同型 Ch 誘導する同型 R(G) から $Z[X(T)]^W$ まで。

$\lambda \in X_{++}$の場合、最高重量$\lambda$の既約表現のR(G)の$[\lambda ]$類で表します。ファミリ $([\lambda ])_{\lambda\in X_{++}}$ は $\mathbf{Z}$ 加群 R(G) の基底であるため、次の主張を証明すれば十分です。

ファミリ (Ch[$\lambda ]$)$_{\lambda\in X_{++}}$] は、$\mathbf{Z}$ モジュール $\mathbf{Z}[X(T)]^W$ の基底です。

$\mathbf{Z}[X(T)]$ のすべての元 $u=\sum_{\lambda}a_{\lambda}e^{\lambda}$ について、$\lambda$ が $a_\mu\not= 0$ のような $\mu\in X(T)$ の集合の極大元である場合、$u$ の項 $a_{\lambda}e^{\lambda}$ は最大と呼ばれます。 Th. 1 は、Ch[$\lambda ]$ に固有の最大値項、つまり $e^{\lambda}$ があることを意味します。したがって、次の補題から命題が続きます。

#### 補題 3 {#lie-ix-s7-lem-3 .statement tag=01G9}

それぞれの $\lambda \in X_{++}$ について、$C_{\lambda}$ を一意の最大値項 $e^{\lambda}$ を持つ $\mathbf{Z}[X(T)]^W$ の元とします。すると、家族$(C_{\lambda})_{\lambda\in X_{++}}$は$\mathbf{Z}[X(T)]^W$の基底になります。

証明は、第5章の提案3と同じです。 VI, §3, no. 4、置き換えること A by $\mathbf{Z}, P$ by X(T) および $P\cap \overline{C}$ by $X_{++}$。

$\Theta (G)$ (それぞれ $\Theta (T)$) を G (それぞれ T) 上の連続代表写像の $\mathbf{C}$-代数とし、$Z\Theta (G)$ (それぞれ $\Theta (T)^W$) を中心 (それぞれ W 不変量) の部分代数からなるとします。 写像。 制限写像 $\Theta (G)\rightarrow \Theta (T)$ 誘導する準同型の環 $r: Z\Theta (G)\rightarrow \Theta (T)^W$。一方、表現 $\tau$ に関連する写像は、$\mathbf{C}$-代数の指標 (つまり、写像 $g \rightarrow$ Tr $\tau (g)$) 拡大するから準同型となります。 Tr$:\mathbf{C}\otimes_{\mathbf{Z}}R(G)\rightarrow Z\Theta (G)$、スペクトル理論によれば、同型です。同様に、$\mathbf{C}$-代数$\iota :\mathbf{C}[X(T)]\rightarrow \Theta$(T)の標準単射 $X(T)\rightarrow \Theta (T)$ 誘導する同型、つまり誘導する同型 $\iota :\mathbf{C}[X(T)]^W\rightarrow \Theta (T)^W$。 図式

$$
\mathbf{C}\otimes_{\mathbf{Z}}R(G)\overset{1\otimes Ch}{\longrightarrow}\mathbf{C}[X(T)]^W
$$

$$
_{Tr}^{\iota} \tag{2}
$$

$$
Z\Theta (G)\longrightarrow^r\Theta (T)^W
$$

は可換です。実際、すべての表現 $\tau : G\rightarrow \mathbf{G}\mathbf{L}(V)$ とすべての $t\in T$ について、

Tr $\tau (t) =\sum_{\lambda\in X(T)}$(暗$V_{\lambda}(T)$)$\lambda (t) =\iota$(Ch$\tau$ )$(t)$,

つまり、$(r\circ$ Tr)[$\tau ] = (\iota \circ$ Ch)[$\tau ]$.

命題から次の結果を推定できます。

#### 系 {#lie-ix-s7-n3-cor-1 .statement tag=01GA}

制限写像 $r: Z\Theta (G)\rightarrow \Theta (T)^W$ は全単射です。

### 4. 指標公式

この数では、群X(T)を乗算して書き、その元をT上の複素数値写像とみなします。元$\rho$の$X(T)\otimes \mathbf{Q}$属するは、 X(T)。

T 上の平方積分可能複素数写像の類のヒルベルト空間を $L^2(T)$ で表し、連続代表写像の部分空間からなるを$\Theta (T)$ で表します。スペクトル理論によれば、X(T) は $L^2(T)$ の正規直交基底であり、$\Theta (T)$ の代数基底です。

$f\in L^2(T)$ と $w\in W$ については、$^wf(t) =f(w^{-1}(t))$ で定義される $L^2(T)$ の $^wf$ 元で表します。従って、$\lambda \in X(T)$ には $^w\lambda =w(\lambda )$ が得られます。署名を $\varepsilon : W\rightarrow  \{1,-1\}$ で示します (反射 $s$ ごとに $\varepsilon (s) =$ $-1$ となるような一意な準同型)。 $f\in L^2$(T)の場合は、入れてください

$$
J(f) =\sum_{w\in W}\varepsilon (w)^wf
$$

$\lambda \in X_{++}$、指標 $^w(\lambda \rho )$ が異なる場合。実際、すべての $w\not= 1$ に対して $^w(\lambda \rho )\not=\lambda \rho$ であることを証明するだけで十分です。しかし、これは補題 1 (no. 1) と、すべての正の根 $\alpha$ に対して $\langle \lambda \rho , K_{\alpha}\rangle =\langle \lambda , K_{\alpha}\rangle + 1>0$ であるという事実から導かれます。その結果、

$\|J(\lambda \rho )\|^2=$ カード(W) $=w(G)$。

元 $f\in L^2(T)$ は、すべての $w\in W$ に対して $^wf=\varepsilon (w)f$ である場合 (つまり、すべての反射 $s$ に対して $^sf=-f$ である場合) は反不変であると言われます。 $\frac{1}{w(G)}J$ が反不変式元の部分空間に対する $L^2(T)$ の直交射影であることを示します。実際、$f, f'$ が $L^2$(T) にあり、$f'$ 反不変式があるとします。その場合、$J(f)$ は反不変であり、

$$
\langle f',J(f)\rangle =\sum_{w\in W}\varepsilon (w)\langle f',^wf\rangle =\sum_{w\in W}\langle^wf',^wf\rangle
$$

$$
=\sum_{w\in W}\langle f', f\rangle =w(G)\langle f', f\rangle
$$

#### 命題 3 {#lie-ix-s7-prop-3 .statement tag=01GB}

元 $J(\lambda \rho )/\surd\overline{w(G)}$、$\lambda \in X_{++}$、形の反不変式の部分空間の正規直交基底 $L^2(T)$ の元、および反不変式の部分空間の代数基底 $\Theta (T)$の元。

証明は第1章と同じです。 VI, §3, no. 3、提案 1。

章著。 VI、場所。引用、提案 2、

$$
J(\rho ) =\rho \prod_{\alpha >0}(1-\alpha^{-1}) =\rho^{-1}\prod_{\alpha >0}(\alpha -1) \tag{3}
$$

それで

$$
J(\rho )J(\rho ) =\prod_{\alpha}(\alpha -1) \tag{4}
$$

コル著Thの2。 1 (§6, no. 2)、次のように推測します。

#### 補題 4 {#lie-ix-s7-lem-4 .statement tag=01GC}

$\varphi$と$\psi$がG上の2つの連続した中心写像である場合、

$$
\int_G\overline{\varphi(g)}\psi (g)dg=\frac{1}{w(G)}\int_T\overline{(\varphi(t)J(\rho)(t))}.(\psi (t)J(\rho )(t))dt
$$

すべての $\lambda \in X_{++}$ について、最高重量 $\lambda$ の G の既約表現の $\chi_{\lambda}$ 指標で表します。

#### 定理 2 (H. ワイル) {#lie-ix-s7-thm-2 .statement tag=01GD}

すべての $\lambda \in X_{++}$ に対して、$J(\rho ).\chi_{\lambda}|T = J(\lambda \rho )$ があります。

写像 $J(\rho ).\chi_{\lambda}|T$ は W のもとで反不変であり、X(T) の元の整数係数を持つ線形結合です。 したがって、Chap. VI, §3, no. 3、提案 1、これは $\sum_\mu a_\mu J(\mu\rho )$ と書くことができます。ここで、$\mu$ 属するから $X_{++}$ まで、$a_\mu$ はすべて整数であり、そのうちの有限の多くは零です。 $\int_G|\chi_{\lambda}(g)|^2dg= 1$から

(スペクトル理論)、提案 3 と補題 4 から、$\sum_\mu(a_\mu)^2= 1$ が得られます。したがって、$a_\mu$ は、1 または $-1$ に等しくなければならない 1 つを除いて、すべて零です。しかし、$\chi_{\alpha}|T$ の $\lambda$ の係数は 1 (Th. 1) に等しいため、$J(\rho ).\chi_{\lambda}|T$ の $\lambda \rho$ の係数は 1 (章 VI, §3, no. 3、注意 2) に等しく、これは $a_{\lambda \rho}= 1$ を意味します。 定理。

#### 系 1 {#lie-ix-s7-thm-2-cor-1 .statement tag=01GE}

no. 3 の記法により、$\mathbf{Z}[X(T)]$ になります。

$(\sum_{w\in W}\varepsilon (w)e^{w\rho})$ Ch[$\lambda ] =\sum_{w\in W}\varepsilon (w)e^{w\lambda}e^{w\rho}$、すべての$\lambda \in X_{++}$。

これは、定理と可換図式 (2) (no. 3) から続きます。

#### 系 2 {#lie-ix-s7-thm-2-cor-2 .statement tag=01GF}

T のすべての $\lambda \in X_{++}$ とすべての正則元 $t$ について、

$$
\chi_{\lambda}(t) =\sum\sum^w\varepsilon_w(w\varepsilon )(\lambda w()wt\rho ()wt\rho ()wt) \tag{5}
$$

ここで、2 つの和は W の元 $w$ の上にあります。

実際、$t$ は正規 (公式 (4)) であるため、$J(\rho )(t)$ は非ゼロです。

$\varphi$ が G 上の中心写像である場合、T に対する $\varphi$ の制限は W のもとで不変であるため、$J(\rho ).\varphi |T$ は W のもとで反不変です。 1 族 $(\chi_{\lambda})_{\lambda\in X_{++}}$ は、G 上の中心代表写像の空間の代数基底と、G 上の平方積分可能な中心写像の類の空間 ZL$^2(G)$ の正規直交基底です。

したがって、提案 3 と Th より、 2 私たちは次のように推測します。

#### 系 3 {#lie-ix-s7-thm-2-cor-3 .statement tag=01GG}

写像は、G の中央代表写像の空間から、G の反不変式元の空間までの、任意の連続中央写像 $\varphi$ 写像 $w(G)^{-1/2}J(\rho )(\varphi |T)$ 誘導する同型に関連付けられます。 $\Theta (T)$; ZL$^2(G)$から$L^2(T)$の反不変式元の部分空間まで、ヒルベルト空間の同型への連続性による拡大する。

#### 系 4 {#lie-ix-s7-thm-2-cor-4 .statement tag=01GH}

$\varphi$ を G 上の連続中心写像とします。すると、

$$
\int_G\overline{\chi_{\lambda}(g)}\varphi (g)dg=\int_T\overline{\lambda(t)}\prod_{\alpha >0}(1-\alpha (t)^{-1})\varphi (t)dt=\int_T\overline{\lambda \rho(t)}.\varphi (t)J(\rho )(t)dt
$$

確かに、補題 4 と Th によって。 2、

$$
\int_G\overline{\chi_{\lambda}(g)}\varphi (g)dg=\frac{1}{w(G)}\int_T\chi_{\lambda}(t)J(\rho )(t)(\varphi (t)J(\rho )(t))dt
$$

$$
=\frac{1}{w(G)}\int_T\overline{J(\lambda \rho)(t)}\varphi (t)J(\rho )(t)dt
$$

しかし、写像 $t \rightarrow \varphi (t)J(\rho )(t)$ は反不変式であり、$\frac{1}{w(G)}J(\lambda \rho )$ は $L^2$(T) の反不変式元の部分空間に対する $\lambda \rho$ の直交射影であるため、

$$
\frac{1}{w(G)}\int_T\overline{J(\lambda \rho)(t)}\varphi (t)J(\rho )(t)dt=\int_T\overline{\lambda \rho(t)}\varphi (t)J(\rho )(t)dt
$$

最後に、公式 (3) までに $\rho (t)J(\rho )(t) =\prod_{\alpha >0}(1-\alpha (t)^{-1})$ が得られるため、系になります。

#### 注意 1 {#lie-ix-s7-n4-rem-1 .statement tag=01GI}

すべての $w\in W$ には、$\rho_w=^w\rho /\rho$ を入力します。それから

$$
\sum_w\varepsilon (w)\rho_w=\prod_{\alpha >0}(1-\alpha^{-1}) =\rho^{-2}\prod_{\alpha >0}(\alpha -1) \tag{6}
$$

$t$ が T の正則元である場合、(5) から次のように推測されます。

$$
\chi_{\lambda}(t) =\sum\sum^w\varepsilon_w(w\varepsilon )(\overset{w}{w}\lambda )\rho (t_w)(\rho t^w)(t)=\sum\prod^w_{\alpha >}\varepsilon (_0w(1)\overset{w}{-}\lambda \alpha (t()t\rho )^{w-}(_1t)) \tag{7}
$$

$\rho_w$ は、整数係数を含む根の線形結合であるため、$\rho \in X(T)$ を仮定しなくても、属するから X(T) であることに注意してください。したがって、公式 (7) は $\rho \in X(T):$ 仮定がなくても有効であることがわかり、これを証明するために、適切な接続されたカバーによって置き換える G を計算し、Cor に還元されます。 2.

#### 注意 2 {#lie-ix-s7-n4-rem-2 .statement tag=01GJ}

同様に、Cor. の最初の等式も同様です。 $\rho \in X(T)$ 仮定がなくても 4 は有効なままです。

#### 注意 3 {#lie-ix-s7-n4-rem-3 .statement tag=01GK}

Th を推測できます。類似の無限小主張 (第 VIII, §9, no. 1、Th. 1) からの 2。 Th についても同様です。次の数の 3 (これは、上記の no. 2 の Th. 2 の類似物です)。

### 5. 既約表現中次数

ここで、群 X(T) に対する加法記法に戻り、$\rho$ 属するが X(T) になるとは想定しません。

#### 定理 3 {#lie-ix-s7-thm-3 .statement tag=01GL}

最高重量 $\lambda$ の G の空間の既約表現の次元は次のように与えられます。

$$
\chi_{\lambda}(e) =\prod_{\alpha\in R_+}\frac{\langle\lambda + \rho , K_{\alpha}\rangle}{\langle\rho , K_{\alpha}\rangle}
$$

$\gamma =\frac{1}{2}\sum_{\alpha >0}K_{\alpha}$ を置くと、すべての単純な根 $\alpha$ に対して $\delta (\alpha )(\gamma ) = 2\pi i$ になります (第 VI, §1, no. 10、提案 29)。ライン $\mathbf{R}\gamma$ は超平面 Ker $\delta (\alpha )$ のいずれにも含まれていないため、十分に小さいすべての $z\in \mathbf{R}^*$ に対して exp($z\gamma$ ) は G の正則元です。すべての $\mu\in X(T)$ とすべての $z\in \mathbf{R}$ について、私たちは

$J(\mu$)(exp($z\gamma$ )) $=\sum_{w\in W}\varepsilon (w)e^{z\delta(\mu)(w^{-1}\gamma)}$。

次の補題を暫定的に受け入れてみましょう:

#### 補題 5 {#lie-ix-s7-lem-5 .statement tag=01GM}

我々は持っています

$J(\mu$)(exp($z\gamma$ )) $=e^{z\delta(\mu)(\gamma)}\prod_{\alpha >0}(1-e^{-z\delta(\mu)(K_{\alpha})})$。

したがって、写像 $J(\mu$)(exp($z\gamma$ )) は、$z$ が 0 になる傾向があるときに 1 になる傾向がある写像の積です。

$$
z^N\prod_{\alpha >0}\delta (\mu)(K_{\alpha}) = (2\pi iz)^N\prod_{\alpha >0}\langle \mu, K_{\alpha}\rangle
$$

ここで、N = カード $R_+$。

まず第一に、$\rho \in X(T)$; と仮定します。 適用コル。 Thの2。 2 $z$ が $0,\chi_{\lambda}(z\gamma )$ と同様に、

$$
\prod_{\alpha >0}\langle \lambda +\rho , K_{\alpha}\rangle /\prod_{\alpha >0}\langle \rho , K_{\alpha}\rangle
$$

したがって、この場合は定理です。

一般的なケースでは、証明 Th では次のことを指摘するだけで十分です。 3 では、適切な接続されたカバーによって常に置き換える G を実現できるため、前述のケースに簡約するを適用できます。

ここで補題 5 を証明します。 $z\in \mathbf{C}$ にしましょう。 $\mathfrak{t}$から$H\in \mathfrak{t}$に関連するX(T)から$\mathbf{C}$までの写像の$\mathbf{C}$-代数写像(X(T)$,\mathbf{C}$)を$\varphi_z$で表す

$\varphi_z(H) :\mu \rightarrow \mu$(経験値$zH$)$=e^{z\delta(\mu)(H)}$。

$\varphi_z(H+H') =\varphi_z(H)\varphi_z(H')$ があるので、環の準同型が存在します。

$\psi_z:\mathbf{Z}[\mathfrak{t}]\rightarrow$ 写像(X(T)$,\mathbf{C}$)

$\psi_z(e^H)(\mu) =e^{z\delta(\mu)(H)}$ のように。一方、Chap。 VI, §3, no. 3、提案 2、$\mathbf{Z}[\mathfrak{t}]:$ には次の関係があります。

$$
\sum_{w\in W}\varepsilon (w)e^{w\gamma}=e^{\gamma}\prod_{\alpha >0}(1-e^{-K_{\alpha}})
$$

適用準同型 $\psi_z$、および等式を使用

$$
\psi_z(e^{w\gamma})(\mu) =e^{z\delta(\mu)(w\gamma)}=e^{z\delta(w^{-1}\mu)(\gamma)}
$$

記載されている公式を推測します。

#### 系 1 {#lie-ix-s7-lem-5-cor-1 .statement tag=01GN}

$\| \|$ を $X(T)\otimes \mathbf{R}$ のノルムとします。すべての $\lambda \in X_{++}$ について、$d(\lambda )$ を最高重量 $\lambda$ の G の空間の既約表現の次元とします。

a) sup$_{\lambda\in X_{++}}d(\lambda )/\|\lambda +\rho \|^N<\infty$、ここで$N = 1/$2(dim $G-$ dim T)。

b) G が半単純の場合、inf$_{\lambda\in X_{++}}d(\lambda )/\|\lambda +\rho \|>0$。

a) すべての $\alpha \in R_+$ に対して、$|\langle \lambda +\rho , K_{\alpha}\rangle | \leq A_{\alpha}\|\lambda +\rho \|$ を伴う $A_{\alpha}>0$ が存在するため、$d(\lambda )/\|\lambda +\rho \|^N\leq \prod_{\alpha >0}A_{\alpha}/\langle \rho , K_{\alpha}\rangle$ が存在します。

b) G が半単純であると仮定し、単純な根を $\beta_1, . . . , \beta_r$ で表し、$N_i=K_{\beta_i}$ を置きます。それから

$$
d(\lambda )\geq \prod_{i=1}^r\frac{\langle\lambda + \rho , N_i\rangle}{\langle\rho , N_i\rangle}=\prod_{i=1}^r\langle \lambda +\rho , N_i\rangle
$$

$\langle \lambda +\rho , N_i\rangle  \geq  \langle \rho , N_i\rangle = 1$ 以降、これは次のことを意味します。

$d(\lambda )\geq$ sup$_i|\langle \lambda +\rho , N_i\rangle |$。

G が半単純の場合、$x \rightarrow$ sup$|\langle x, N_i\rangle |$ は $X(T)\otimes \mathbf{R}$ 上のノルムであり、必然的に指定されたノルムと等価であるため、b)。

#### 系 2 {#lie-ix-s7-lem-5-cor-2 .statement tag=01GO}

G が半単純であると仮定します。 $d$を整数とします。 類の表現のGの次元$\leq d$の集合は有限です。

コル。 $1b)$ は、元の $X_d$ $X_{++}$ の集合 $\lambda$ が、$d(\lambda )\leq d$ が有限であることを意味します。 $X_d$ のすべての $\lambda$ について、$V_{\lambda}$ を最高重量 $\lambda$ の既約表現とします。 次元 $\leq d$ のすべての表現は直和 $\bigoplus_{\lambda\in X_d}V^{n_{\lambda}}_{\lambda}$ と同型であり、$n_{\lambda}\leq d$ であるため、系となります。

### 6. カシミール元

§1, no. 3 の提案 3 により、$\mathfrak{g}$ 上に負対称双線形形式が存在し、Ad(G) のもとで分離され不変です (G が半単純の場合、例えば、$\mathfrak{g}$ の Killing 形を取ることができます)。 F をそのような形とします。 F に関連付けられたカシミール元は、エンベロープ代数 $U(\mathfrak{g})$ の中心の元 $\Gamma$ であり、$\mathfrak{g}$ の基底 $(e_i)$ について、(第 I, §3, no. 7 章) を思い出してください。 満たす $F(e_i, e_j) =-\delta_{ij}$、$\Gamma =-\sum e^2_i$ があります。

この章の残りでは、$\mathfrak{g}$上の負の分離不変対称双線形形式からこのようにして得られた$U(\mathfrak{g})$のG元のカシミール元と呼ぶことにします。 $\Gamma$ が G のカシミール元で、$\tau : G\rightarrow \mathbf{G}\mathbf{L}(V)$ が G の既約表現である場合、V の自己準同型 $\Gamma_V$ はホモテティー (代数、Chap. VIII, §3, no. 2、Th. 1) であり、その比は$\widetilde{\Gamma}(\tau )$で表します。

#### 命題 4 {#lie-ix-s7-prop-4 .statement tag=01GP}

$\Gamma$ を G のカシミール元とします。

a) $\tau$ が G$,\widetilde{\Gamma}(\tau )$ の既約表現である場合、実数であり、正です。 $\tau$ が自明な表現ではない場合、$\widetilde{\Gamma}(\tau )>0$。

b) $X(T)\otimes \mathbf{R}$ 上に固有の 2 次形式 $Q_{\Gamma}$ が存在し、G の既約表現 $\tau$ ごとに、

$$
\widetilde{\Gamma}(\tau ) = Q_{\Gamma}(\lambda +\rho )-Q_{\Gamma}(\rho )
$$

ここで、$\lambda$ は $\tau$ の最高重量です。 形 $Q_{\Gamma}$ は、W の下で正、分離、不変です。

F を、$\Gamma$ を定義する $\mathfrak{g}$ 上の分離負対称双線形形式とします。 $\tau : G\rightarrow \mathbf{G}\mathbf{L}(V)$ を G の既約表現とします。 $\langle ,\rangle$ を G (§1, no. 1) の下で不変式である V 上のヒルベルト スカラー 積とし、$F(e_i, e_j) =-\delta_{ij}$ となるような $\mathfrak{g}$ の $(e_i)$ 基底とします。次に、G の下で不変ではない V のすべての元 $v$ について、次のようになります。

$$
\widetilde{\Gamma}(\tau )\langle v, v\rangle =\langle v, \Gamma_V(v)\rangle =-\sum_i\langle v,(e_i)^2_Vv\rangle =\sum_i\langle v,(e_i)^*_V(e_i)_Vv\rangle
$$

$$
=\sum_i\langle (e_i)_Vv,(e_i)_Vv\rangle >0
$$

したがって、a)。

B を、F によってスカラーの拡大によって誘導された、$\mathfrak{g}_{\mathbf{C}}$ 上の制限の $\mathfrak{t}^*_{\mathbf{C}}$ から双線形形式の $\mathfrak{t}_{\mathbf{C}}$ の逆数形とします。コルによって。第 7 章の提案 7 VIII, §6, no. 4、私たちは$^5\widetilde{\Gamma}(\tau ) = B(\delta (\lambda ), \delta (\lambda +2\rho ))$を持っています。 拡大する $\delta : X(T)\rightarrow$ $\mathfrak{t}^*_{\mathbf{C}}$ を $X(T)\otimes \mathbf{R}$ から $\mathfrak{t}^*_{\mathbf{C}}$ までの $\mathbf{R}$ 線形写像に変換し、 $Q_{\Gamma}$ を $X(T)\otimes \mathbf{R}$ の 2 次式形 $x \rightarrow B(\delta (x), \delta (x))$ とします。それは W のもとで分離し不変であり、そして

$$
\widetilde{\Gamma}(\tau ) = B(\delta (\lambda +\rho ), \delta (\lambda +\rho ))-B(\delta (\rho ), \delta (\rho )) = Q_{\Gamma}(\lambda +\rho )-Q_{\Gamma}(\rho )
$$

We show that 形 $Q_{\Gamma}$ is positive.確かに、$x\in X(T)\otimes \mathbf{Q}$、元 $\delta (x)$、$\mathfrak{t}^*_{\mathbf{C}}$ が $\mathfrak{t}$ 上の純粋に虚数の値を取る場合、$i\mathfrak{t}$ の実数値になります。 $y\in i\mathfrak{t}$ に対して、$F(y, y)\geq 0$ があることに注目して、結論するを決定します。

b) の一意性主張を証明することが残っています。 Let Q be a quadratic 形 on $X(T)\otimes \mathbf{R}$ 満たす the required 条件, and let $\Phi$ (resp. $\Phi_{\Gamma}$) be 双線形形式 associated to Q (resp. $Q_{\Gamma}$). $\lambda , \mu\in X_{++}$ については、

$$
\Phi (\lambda , \mu) = (Q(\lambda +\mu+\rho )-Q(\rho ))-(Q(\lambda +\rho )-Q(\rho ))-(Q(\mu+\rho )-Q(\rho ))
$$

$$
=\Phi_{\Gamma}(\lambda , \mu)
$$

$X(T)_{++}$ 生成する $\mathbf{R}$-ベクトル空間 $X(T)\otimes \mathbf{R}$ なので、$\Phi =\Phi_{\Gamma}$ なので、$Q = Q_{\Gamma}$ になります。

#### 注意 {#lie-ix-s7-n6-rem-1 .statement tag=01GQ}

$x\in \mathfrak{g}$ にしましょう。 G の下で、すべての既約表現 $\tau : G\rightarrow \mathbf{G}\mathbf{L}(V)$ とすべてのヒルベルト構造について、V の不変量に対して、次のような厳密に正の実数 A が存在します。

$$
\|L(\tau )(x)\|^2\leq A.\widetilde{\Gamma}(\tau )
$$

確かに、前の証明の記法を使用すると、$\mathfrak{g}$ の選ぶ基底 $(e_i)$ ができ、$x=ae_1,a\in \mathbf{R}$ になります。次に、$v\in V$ については、

$$
\langle x_Vv, x_Vv\rangle =|a|^2\langle e_1v, e_1v\rangle  \leq  |a|^2\widetilde{\Gamma}(\tau )\langle v, v\rangle
$$

### 練習問題 {#lie-ix-s7-exercises}

[§ 7 に対して練習問題](exercises/s7/)を参照してください。
