---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: IX
chapter_title: COMPACT REAL LIE GROUPS
section: 1
section_title: Structure of compact groups
appendix: true
lang: ja
source: lie-vii-ix
book_pages: 381-385, 424-425
pdf_pages: 0388-0392, 0431-0432
extraction: native
subsections:
    - "no": 1
      title: EMBEDDING A COMPACT GROUP IN A PRODUCT OF LIE GROUPS
      page: 381
      pdf_page: 388
    - "no": 2
      title: PROJECTIVE LIMITS OF LIE GROUPS
      page: 382
      pdf_page: 389
    - "no": 3
      title: STRUCTURE OF CONNECTED COMPACT GROUPS
      page: 384
      pdf_page: 391
statements: 9
exercises: 1
content_sha256: db53ab6211157473578b1376eeb092da6b476cf3866724e28288a187b00f5dd8
translated_from: content/en/lie/IX/A1_a1_structure_of_compact_groups.md
translation_method: google
source_content_sha256: 5e7319fca99d12df0397567af8fdb7c23d7ffbc97775400d0463c84a608eb608
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: f5d447056a145cca2b3fca5a017d4eb73a121851a7c917d4d727153b770c2e67
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## 付録 I

# 構造のコンパクト群

### 1. リー群の積にコンパクト群を埋め込む

#### 命題 1 {#lie-ix-a1-prop-1 .statement tag=01II}

すべてのコンパクトなトポロジー 群 G は、コンパクト・リー群の積の閉じた部分群と同型です。

有限次元複素ヒルベルト空間上の G の既約連続ユニタリ表現のクラスの集合を $\widehat{G}$ で表します (スペクトル理論、準備中)。 すべての $u\in \widehat{G}$ について、$Hu$ を $u$ の空間と $u$ に関連付けられた $\rho_u: G\rightarrow \mathbf{U}(H_u)$ 準同型とします。 Peter-Weyl 定理 (スペクトル理論、準備中) によれば、G から $\prod_{u\in\widehat{G}}\mathbf{U}(H_u)$ までの連続準同型 $\rho = (\rho_u)_{u\in\widehat{G}}$ は単射的です。 G はコンパクトなので、 $\rho$ 誘導する同型

G から群 $\prod_{u\in\widehat{G}}\mathbf{U}(H_u)$ の閉じた部分群へ。

#### 系 1 {#lie-ix-a1-prop-1-cor-1 .statement tag=01IJ}

V を G の単位元の近傍とします。次に、 V 含むは、商 $G/H$ がリー群となるような G の閉じた法線部分群 H となります。

$(K_{\lambda})_{\lambda\in L}$ をコンパクト・リー群の族とし、G を $\prod_{\lambda\in L}K_{\lambda}$ の閉じた部分群と識別できるようにします。 $\lambda \in L$ の場合、$p_{\lambda}: G\rightarrow K_{\lambda}$ 制限によって正規の射影の G に降格します。 $K_{\lambda}$ の原点には有限部分集合 $J\subset L$ が存在し、それぞれ $\lambda \in J$ 近傍 $V_{\lambda}$ が存在し、V 含む $\bigcap_{\lambda\in J}p^{-1}_{\lambda}(V_{\lambda})$ になります。これで、$H =\bigcap_{\lambda\in J}$ Ker($p_{\lambda}$) を入れるだけで十分です。

商 $G/H_{\alpha}$ がリー群となるような、G の閉じた法線部分群のフィルタリングされた族 $(H_{\alpha})_{\alpha\in I}$ 減少するで表します。 コンパクト・リー群 $G/H_{\alpha}$ の射影系 (cf. 一般位相、章 III, §7, no. 2、提案 2) を考えてみましょう。

#### 系 2 {#lie-ix-a1-prop-1-cor-2 .statement tag=01IK}

正準写像 $G\rightarrow$ lim$_{_{\leftarrow -}}G/H_{\alpha}$ はトポロジカル群の同型です。 $\alpha$

確かに、Cor. 1 は、一般位相、第 1 章の条件 (PA) を意味します。 III, §7, no. 2、満足しています。 主張は、上記の提案 2 に従っています。引用。

#### 系 3 {#lie-ix-a1-prop-1-cor-3 .statement tag=01IL}

G がリー群であるのは、$\{e\}$ とは異なる正規部分群を含まない G の恒等要素 $e$ の近傍が存在する場合に限ります。

この条件の必要性はすでに証明されており（第 2 章III, §4, no. 2、コリント 1 章）、十分性はコリント 2 の明らか帰結です。 1.

### 2. 射影極限/リー群

#### 補題 1 {#lie-ix-a1-lem-1 .statement tag=01IM}

$(G_{\alpha}, f_{\alpha \beta})$ を、フィルタリングされた添字集合 I に対するトポロジカル群の射影系とし、G をその極限とします。正準写像 $f_{\alpha}: G\rightarrow G_{\alpha}$ が全射であると仮定します。

a) 部分群 $D(G_{\alpha})$ (それぞれ $C(G_{\alpha})$、それぞれ $C(G_{\alpha})_0$) 形 $G_{\alpha}$ の部分集合の射影系。

b) D(G) = lim$_{_{\leftarrow -}\alpha}\overline{D(G_{\alpha})}$ および C(G) = lim$_{_{\leftarrow -}\alpha}C(G_{\alpha})$ が得られます。

c) $G_{\alpha}$ がすべての $\alpha \in I$ に対してコンパクトである場合、$C(G)_0=$ lim$_{_{\leftarrow -}\alpha}C(G_{\alpha})_0$ になります。

$\alpha , \beta$ を I の 2 つの元と $\alpha \leq \beta$ とします。次に、$f_{\alpha \beta}(D(G_{\beta}))\subset D(G_{\alpha})$、そして $f_{\alpha \beta}$ は全射なので $f_{\alpha \beta}(C(G_{\beta}))\subset C(G_{\alpha})$ です。 $f_{\alpha \beta}$ は連続なので、$f_{\alpha \beta}(\overline{D(G_{\beta})})\subset \overline{D(G_{\alpha})}$ と $f_{\alpha \beta}(C(G_{\beta})_0)\subset C(G_{\alpha})_0$ が成り立ち、したがって a)。 $f_{\alpha}$ は全射なので、$f_{\alpha}(D(G)) = D(G_{\alpha})$ (代数、章 I, §6, no. 2、提案 6) なので、$\overline{D(G)}=$ lim$_{\leftarrow -}\overline{D(G_{\alpha})}$ (一般位相、章 I, §4, no. 4、提案 9 の修正)。 $f_{\alpha}$ の全射性は、$f_{\alpha}(C(G))\subset$ $C(G_{\alpha})$ を含むことも意味し、したがって $C(G)\subset$ lim$_{\leftarrow -}C(G_{\alpha})$ も意味します。反対の包含は明らかです。最後に、主張 c) は b) と一般位相、第 2 章から続きます。 III, §7, no. 2、提案 4)。

#### 補題 2 {#lie-ix-a1-lem-2 .statement tag=01IN}

$(S_a)_{a\in A},(T_b)_{b\in B}$ を、ほぼ単純で単純に接続された 2 つの有限族リー群 (章 III, § 9, no. 8、定義 3)$,u:\prod_{a\in A}S_a\rightarrow \prod_{b\in B}T_b$ 全射法射とする。次に、$\prod_{a\in A}S_a$ の元 $(s_a)_{a\in A}$ ごとに $u((s_a)_{a\in A}) = (u_b(s_{l(b)}))_{b\in B}$ となるような単射詞写像 $l: B\rightarrow A$ と同型 $u_b: S_{l(b)}\rightarrow T_b(b\in B)$ が存在します。

$a\in A$ (それぞれ $b\in B$) を $S_a$ (それぞれ $T_b$) の $\mathfrak{s}_a$ (それぞれ $\mathfrak{t}_b$) リー代数で表し、準同型 $L(u) :\prod_{a\in A}\mathfrak{s}_a\rightarrow \prod_{b\in B}\mathfrak{t}_b$ を考えます。 核です

は半単純リー代数 $\prod_{a\in A}\mathfrak{s}_a$ の理想であり、したがって $A''\subset A$ を伴う形 $\prod_{a\in A''}\mathfrak{s}_a$ です（I, §6, no. 2 章、コリント 1）。 $A'= A$**--** $A''$ を入れます。によって

制限、$L(u)$ 誘導する同型 $f:\prod_{a\in A'}\mathfrak{s}_a\rightarrow \prod_{b\in B}\mathfrak{t}_b$。ロケ地にて。前述のとおり、すべての $a\in A'$ にとって、イデアル $f(\mathfrak{s}_a)$ は $\mathfrak{t}_b$ の 1 つに等しい。したがって、$b\in B$ に対して $f(\mathfrak{s}_{l(b)}) =\mathfrak{t}_b$、および $f$ 誘導する同型 $f_b:\mathfrak{s}_{l(b)}\rightarrow \mathfrak{t}_b$ となるような全単射 $l: B\rightarrow A'$ が存在します。 群 $S_a$ と $T_b$ は単純結合なので、 $b\in B$ に対して $L(u_b) =f_b$ となるような同型 $u_b: S_{l(b)}\rightarrow T_b$ が存在します (第 3 章 III, §6, no. 3)。

$\widetilde{u}((s_a)_{a\in A}) =$ によって定義される $\widetilde{u}:\prod_{a\in A}S_a\rightarrow \prod_{b\in B}T_b$ 射で示されます

$(u_b(s_{l(b)}))_{b\in B}$。 構成、$L(\widetilde{u}) =f= L(u)$なので、$\widetilde{u}=u$となり、補題が証明されます。

#### 補題 3 {#lie-ix-a1-lem-3 .statement tag=01IO}

補題 1 の仮説の下で、$G_{\alpha}$ が単純接続されているコンパクト・リー群と仮定します。次に、トポロジカル群 G は、ほぼ単純な単純結合コンパクト・リー群の族の積と同型です。

すべての $\alpha \in I$ に対して、群 $G_{\alpha}$ は、ほぼ単純で単純に接続された有限族部分群 $(S^{\lambda}_{\alpha})_{\lambda\in L_{\alpha}}$ の直接の積 (第 III, §9, no. 8、提案 28)。 $\beta \in I,\beta \geq \alpha$ にしましょう。 補題 2 までに、$\lambda \in L_{\alpha}$ に対して $f_{\alpha \beta}(S^{l_{\beta \alpha}(\lambda)}_{\beta}) = S^{\lambda}_{\alpha}$ となるような写像 $l_{\beta \alpha}: L_{\alpha}\rightarrow L_{\beta}$ が存在します。 $\alpha \leq \beta \leq \gamma$ に対して $l_{\gamma \beta}\circ l_{\beta \alpha}=l_{\gamma \alpha}$ があるため、$(L_{\alpha}, l_{\beta \alpha})$ は I に対する集合の帰納的系です。 L をその極限とします。 写像 $l_{\beta \alpha}$ は単射なので、$L_{\alpha}$ は L の部分集合と同一視できるので、$L =\bigcup_{\alpha\in I}L_{\alpha}$ になります。

$\lambda \in L$ にしましょう。 $\lambda  \notin L_{\alpha}$のとき$S^{\lambda}_{\alpha}=\{1\}$を置き、$f_{\alpha \beta}$によって引き起こされる$\varphi^{\lambda}_{\alpha \beta}: S^{\lambda}_{\beta}\rightarrow S^{\lambda}_{\alpha}$射で表します。これにより、トポロジカル群 $(S^{\lambda}_{\alpha}, \varphi^{\lambda}_{\alpha \beta})$ の射影系が得られ、その極限は $S_{\lambda}$ と同型です。トポロジカル群の標準準同型

リム$_{_{\leftarrow -\alpha\in I}}((\prod_{\lambda\in L}S^{\lambda}_{\alpha})\rightarrow \prod_{\lambda\in L}($リム$_{_{\alpha\leftarrow -\in I}}S^{\lambda}_{\alpha})$

全単射です (集合の理論、Chap. III, §7, no. 3、Cor. 2)。問題の群はコンパクトなので、したがって同型になります。しかし、これらの最初の群は G で識別でき、2 番目は $S_{\lambda}$ の積で識別できるため、補題となります。

### 3. 接続されたコンパクトの構造群

G を可換コンパクト群とする。 Recall (Spectral Theory, Chap. II, §1, no. 9, Prop. 11) that G is then isomorphic to the dual topological group of a discrete commutative group $\widehat{G}$. The group G is connected if and only if $\widehat{G}$ is torsion-free (Spectral Theory, Chap. II, §2, no. 2, Cor. 1 of Prop. 4).

次のプロパティは同等です (スペクトル理論、Chap. II, §2, no. 2、提案 4 の Cor. 2 および提案 11 の §1, no. 9、Cor. 2):

(i) G は完全に不連続です。

(ii) $\widehat{G}$ は捩れ群です。

(iii) トポロジカル群 G は、有限 (可換) 群の射影系の極限と同型であり、それぞれ離散位相を持ちます。

以下の命題は Cor を一般化します。 §1, no. 4の提案4の1。

#### 命題 2 {#lie-ix-a1-prop-2 .statement tag=01IP}

G を連結コンパクト群とします。

a$) C(G)_0$ は可換接続コンパクト群です。 D(G) は接続されたコンパクト群であり、その導来群に等しい。

b) $C(G)_0\times D(G)$ から G までの連続準同型 $(x, y) \rightarrow xy$ は全射的であり、その核はコンパクトで完全に不連続な $C(G)_0\times D(G)$ の中心部分群です。

c) ほぼ単純なコンパクト・リー群と全射連続準同型 $\prod_{\lambda\in L}S_{\lambda}\rightarrow D(G)$ の族 $(S_{\lambda})_{\lambda\in L}$ が存在し、その核は

完全に不連続、コンパクト、中心部分群。

$(G_{\alpha}, f_{\alpha \beta})$ を、フィルタリングされた集合 I を基準としたコンパクト・リー群の射影系とし、G が lim$_{\leftarrow -}G_{\alpha}$ と同型であり、正準写像 $f_{\alpha}: G\rightarrow G_{\alpha}$ が全射であるようにします (提案 1 の Cor. 2)。 $\alpha \in I$ の場合、$\pi_{\alpha}: \widetilde{D}(G_{\alpha})\rightarrow D(G_{\alpha})$ を群 $D(G_{\alpha})$ の普遍的なカバーとします。 $f_{\alpha \beta}$ 誘導する射 $\widetilde{f}_{\alpha \beta}: \widetilde{D}(G_{\beta})\rightarrow \widetilde{D}(G_{\alpha})$、および $( \widetilde{D}(G_{\alpha}),\widetilde{f}_{\alpha \beta})$ は、補題 3 のトポロジカル群満たすの仮説の射影系です。

この補題から、位相位相群 lim$_{\leftarrow -}\widetilde{D}(G_{\alpha})$ は、ほぼ単純なコンパクト・リー群の族 $(S_{\lambda})_{\lambda\in L}$ の積と同型であることがわかります。 補題 1 により、準同型 $(\pi_{\alpha})$ の射影系の極限は、連続する準同型 $\pi :\prod_{\lambda\in L}S_{\lambda}\rightarrow D(G)$ と識別できます。

これは全射法です (一般位相、章 I, §9, no. 6、提案 8 のコリント 2)。

ここで、群 $\prod_{\lambda\in L}S_{\lambda}$ がその導来群に等しいことを観察します。

§4, no. 5、Cor. から続きます。 $\pi$ は全射なので、D(G) にも同じことが当てはまります。従って、$D(G)\supset D(D(G)) = D(G)$。従って、群 D(G) はコンパクトであり、その導来群と等しくなります。 $C(G)_0$ に関する主張は自明であるため、これは a) を証明します。

一方、$\pi :\prod_{\lambda\in L}S_{\lambda}\rightarrow D(G)$の核は識別できます

lim$_{\leftarrow -}$ Ker($\pi_{\alpha}$) $($代数、Chap. II, §6, no. 1、注意 1) 従って、

コンパクト、完全に不連続、中心部分群、従って c)。

b)を証明します。 I、射 $s_{\alpha}: C(G_{\alpha})_0\times D(G_{\alpha})\rightarrow G_{\alpha}$ のすべての $\alpha$ について、$x\in C(G_{\alpha})_0, y\in D(G_{\alpha})$ の $s_{\alpha}(x, y) =xy$ は全射的であり、その核は有限中心部分群です (§1, no. 4、提案 4 の Cor. 1)。 $s_{\alpha}$ 形は写像の射影系であり、その極限は、前述のことから、$C(G)_0\times D(G)$ から G までの準同型 $(x, y) \rightarrow xy$ と同定できます。今、この写像が前にであることがわかります。全射的であり、その核が中心で完全に不連続であるため、b)。

#### 系 {#lie-ix-a1-n3-cor-1 .statement tag=01IQ}

すべての可解な接続コンパクト群は可換です。

実際、導来群は解けて、その導来群 (提案 $2a$)$)$ に等しいので、単位元に減らされます。

### 練習問題 {#lie-ix-a1-exercises}

[練習問題付録 1](exercises/a1/)を参照してください。
