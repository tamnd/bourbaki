---
book: evt
book_title: Topological Vector Spaces
chapter: III
chapter_title: SPACES OF CONTINUOUS LINEAR MAPPINGS
section: 3
section_title: Spaces of continuous linear mappings
lang: ja
source: evt-i-v
book_pages: TVS III.13-TVS III.23, TVS III.41-TVS III.43
pdf_pages: 0145-0155, 0173-0175
extraction: ocr
subsections:
    - "no": 1
      title: The spaces $\mathscr{L}_\mathfrak{S}(E; F)$
      page: 13
      pdf_page: 145
    - "no": 2
      title: Condition for $\mathscr{L}_\mathfrak{S}(E; F)$ to be Hausdorff
      page: 15
      pdf_page: 147
    - "no": 3
      title: Relations between $\mathscr{L}(E; F)$ and $\mathscr{L}(\hat{E}; F)$
      page: 15
      pdf_page: 147
    - "no": 4
      title: Equicontinuous subsets of $\mathscr{L}(E; F)$
      page: 16
      pdf_page: 148
    - "no": 5
      title: Equicontinuous subsets of $E'$
      page: 19
      pdf_page: 151
    - "no": 6
      title: The completion of a locally convex space
      page: 20
      pdf_page: 152
    - "no": 7
      title: $\mathscr{S}$-bornologies on $\mathscr{L}(E; F)$
      page: 21
      pdf_page: 153
    - "no": 8
      title: Complete subsets of $\mathscr{L}_{\mathscr{S}}(E; F)$
      page: 22
      pdf_page: 154
statements: 39
exercises: 13
content_sha256: 82cf973f1a58ba2a2e6b86ba646df7b2abb86f9e30ea42f93e7dbe117591c838
translated_from: content/en/evt/III/03_s3_spaces_of_continuous_linear_mappings.md
translation_method: google
source_content_sha256: cf2d3140178ddd9a073d777e8eb5efd04f0920704426c6cc3aa6359b95506798
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-b071ad41
glossary_version: 34
glossary_terms_sha256: 215718dbcdb786779a74b07f9095e2e6bec6b29e546c0d0ef1118fecf1ab5a73
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## § 3。 空間 / 連続線形写像

### 1. 空間 $\mathscr{L}_\mathfrak{S}(E; F)$

F を位相的なベクトル空間、E を任意の集合、$\mathfrak{S}$ を E の部分集合の族とする。 $\mathfrak{S}$-収束 (GT、X, § 1, No. 2) の一様構造を使用してベクトル空間 $F^E$ を考えます。 この構造が $F^E$ (GT、X, § 1, No. 4、cor. 2) の可換群構造と互換性があることがわかっています。 このように推定された位相は、$\mathfrak{S}$*-トポロジー*と呼ばれます。 If X is a subset of $F^E$, or more generally, a set with a mapping $j : X \to F^E$, then the universe image under j of the $\mathfrak{S}$*-topology* on $F^E$ is called the $\mathfrak{S}$*-topology* on X.

#### 注意 {#evt-iii-s3-n1-rem-1 .statement tag=07MJ}

— 1) $\mathfrak{S}$*-トポロジー* は、$\mathfrak{S}'$*-トポロジー* と同一です。ここで、$\mathfrak{S}'$ は、$\mathfrak{S}$ (III, p. 1) によって生成されたボーンロジーを示します。

2) $M \in \mathfrak{S}$ と V を F の 0 の近傍とします。 $T(M, V)$ は、$x \in M$ ごとに $f(x) \in V$ となるように、すべての $f \in F^E$ の集合を表します。 If $\mathfrak{S}$ is stable under finite unions, the sets $T(M, V)$ form a fundamental system of neighbourhoods of 0 for the $\mathfrak{S}$*-topology* of $F^E$.

#### 命題 1 {#evt-iii-s3-prop-1 .statement tag=07MK}

*E を集合、$\mathfrak{S}$ を E の部分集合の族、F をトポロジカルベクトル空間、H を $F^E$ のベクトル部分空間とします。 $\mathfrak{S}$*-トポロジー* が H のベクトル空間構造と互換性がある位数では、$u(M)$ がすべての $u \in H$ とすべての $M \in \mathfrak{S}$ について F で制限されることが必要かつ十分です。さらに、F が局所的に凸である場合、H 上の $\mathfrak{S}$*-トポロジー* は局所的に凸です。

上記の注意 1) と 2) を考慮すると、$\mathfrak{S}$*-トポロジー* が H のベクトル空間構造と互換性を持つために必要かつ十分な条件は、集合 $H \cap T(M, V)$ が H (I, p. 7、提案 4)。しかしこれは、F の 0 のすべての $u \in H$、すべての部分集合 $M \in \mathfrak{S}$、およびバランスの取れたすべての近傍 V に対して、$u(M) \subset \lambda V$ となるような $\lambda \neq 0$ が存在することを意味します。つまり、(III, p. 2) は、$u(M)$ が F で有界であるということです。最後に、V が凸であれば、$T(M, V)$ も凸であるという事実から、命題の最後の主張が得られます。

#### 系 {#evt-iii-s3-n1-cor-1 .statement tag=07ML}

*E と F を 2 つの局所凸空間、E の有界部分集合の族 $\mathfrak{S}$、および E から F への連続線形写像の $\mathscr{L}(E; F)$ ベクトル空間とします。すると、$\mathfrak{S}$*-トポロジー* は、次のベクトル空間構造と互換性があります。 $\mathscr{L}(E; F)$ で局所的に凸です。*

$u$ が E から F への連続線形写像であり、M が E の有界部分集合である場合、$u(M)$ は F で有界である (III, p. 4, cor. 1) ことに注意するだけで十分です。

2 つの局所凸ベクトル空間 E と F、および E の有界部分集合の族 $\mathfrak{S}$ が与えられた場合、$\mathscr{L}_\mathfrak{S}(E; F)$ は、$\mathfrak{S}$*-トポロジー* を $\mathscr{L}(E; F)$ に割り当てることによって得られる局所凸空間を表します。

#### 例 1 {#evt-iii-s3-n1-exa-1 .statement tag=07MM}

$\mathfrak{S}$ が E のすべての有限部分集合の集合である場合、$\mathfrak{S}$-トポロジーは *単純収束* の位相であり、空間 $\mathscr{L}_{\mathfrak{S}}(E; F)$ は $\mathscr{L}_s(E; F)$ によっても表されます。 $\mathscr{L}_s(E; F)$ の有界部分集合は、$\mathscr{L}(E; F)$ の単純有界部分集合と呼ばれます。

#### 例 2 {#evt-iii-s3-n1-exa-2 .statement tag=07MN}

$\mathfrak{S}$ が *compact* (それぞれ *precompact*、*compact convex*) 部分集合の集合である場合、$\mathfrak{S}$-トポロジは *compact* (それぞれ *precompact*、*compact convex*) 収束および空間の位相と呼ばれます。 $\mathscr{L}_{\mathfrak{S}}(E; F)$ は、$\mathscr{L}_c(E; F)$ (それぞれ $\mathscr{L}_{pc}(E; F)$、$\mathscr{L}_{cc}(E; F)$) とも表されます。 (*参照* IV、p. 48、演習 7.)

#### 例 3 {#evt-iii-s3-n1-exa-3 .statement tag=07MO}

$\mathfrak{S}$ が E のすべての*有界* 部分集合の集合である場合、$\mathfrak{S}$-トポロジーは *有界収束* の位相であり、空間 $\mathscr{L}_{\mathfrak{S}}(E; F)$ は $\mathscr{L}_b(E; F)$ で表されると言います。

#### 例 4 {#evt-iii-s3-n1-exa-4 .statement tag=07MP}

$F = \mathbf{K}$, 空間 $\mathscr{L}(E; F)$ が E の *双対* $E'$ であるとき、$E'_\mathfrak{S}$、$E'_s$ などで表します。 空間 $\mathscr{L}_{\mathfrak{S}}(E; \mathbf{K})$、$\mathscr{L}_s(E; \mathbf{K})$ など空間 $E'_s$ (それぞれ $E'_b$) は E の弱い双対 (それぞれ強い双対) と呼ばれます。 $E'_s$ (それぞれ $E'_b$) の有界部分集合は弱く (それぞれ強く) 有界であると言われます。 $E'$ の弱い位相は他ならぬ$\sigma(E', E)$ (II, p. 42) であることがわかります。

$E = F$の場合、$\mathscr{L}(E)$、$\mathscr{L}_{\mathfrak{S}}(E)$など、空間、$\mathscr{L}(E; F)$、$\mathscr{L}_{\mathfrak{S}}(E; F)$などと表します。

$p$ を F および M 上の連続半ノルムとし、E の有界部分集合とする。

$$
p_M(u) = \sup_{x \in M} p(u(x)) .
$$

$p_M$ が $\mathscr{L}(E; F)$ の準ノルムであること、および $\Gamma$ が F の準ノルムの基本系である場合、準ノルム $p_M$ の族で、$p$ の範囲は $\Gamma$ を超え、M の範囲は明らかです。 $\mathfrak{S}$ によって生成されたボーンロジーの基底は、$\mathscr{L}_{\mathfrak{S}}(E; F)$ の準規範の基本的な系です。

特に、E と F が準ノルム空間であり、$p$ (それぞれ $q$) が E (それぞれ F) の準ノルムを表す場合、$\mathscr{L}(E; F)$ に対する有界収束の位相は準ノルムによって定義されます。

$$
r(u) = \sup_{p(x) \leq 1} q(u(x))
$$

(*cf.* GT、X, § 3, No. 2)。 $\mathscr{L}_b(E; F)$ を半規範化された空間として考えるとき、私たちは常に、〜でない限り逆のことが明示的に述べられているが、半規範 (2) を意味するものとします。 F がノルム空間の場合、準ノルム (2) はノルムです。

#### 注意 {#evt-iii-s3-n1-rem-2 .statement tag=07MQ}

— 3) A を E の単位元ボールの密な部分集合とします。 $u$ の連続性を考慮して、次のようになります。

$$
r(u) = \sup_{x \in A} q(u(x)) .
$$

たとえば

$$
r(u) = \sup_{p(x) < 1} q(u(x)) .
$$

$t \in \mathbf{R}$ に対して $u(tx) = tu(x)$ があるので、次もあります。

$$
r(u) = \sup_{p(x) = 1} q(u(x)) = \sup_{p(x) \neq 0} \frac{q(u(x))}{p(x)} .
$$

いつでも$p \neq 0$。

4) 公式 (2) は、写像 $u \mapsto r(u)$ が $\mathscr{L}_s(E; F)$ で半連続的に低いことを示しています。

#### 命題 2 {#evt-iii-s3-prop-2 .statement tag=07MR}

— E と F を 2 つの局所的に凸な空間とし、$\mathfrak{S}$ を E の有界部分集合の集合とします。

1) $\mathscr{L}(E; F)$ 上の $\mathfrak{S}$ トポロジーは $\tilde{\mathfrak{S}}$ トポロジーと同一です。ここで、$\tilde{\mathfrak{S}}$ は、含む $\mathfrak{S}$ である E 上の最小の適応されたボーンロジー (III、p. 3) を表します。

2) F で $\{0\}$ が密ではないと仮定し、$\mathfrak{S}'$ を E の有界部分集合の他の集合とします。その場合、$\mathfrak{S}' \subset \tilde{\mathfrak{S}}$ の場合にのみ、$\mathfrak{S}'$-トポロジーは $\mathfrak{S}$-トポロジーより粗くなります。

$u \in \mathscr{L}(E; F)$、$M \in \mathfrak{S}$、$p$ を F 上の連続半ノルムとします。 $p \circ u$ は E 上の連続半ノルムであるため、これは、M または M の閉じた凸平衡包絡線 $\tilde{M}$ 上で $p \circ u$ が 1 によって上に制限されるというと同じです。他の語には $p_M = p_{\tilde{M}}$ があります。さらに、すべての $\lambda > 0$ と $p_{M \cup M'} = \sup(p_M, p_{M'})$ に対して $p_{\lambda M} = \lambda p_M$ があり、そこから最初の主張が続くことは明らかです。なぜなら、 $\tilde{\mathfrak{S}}$ には、有限の和集合または集合の閉じた凸平衡包絡線の相似関数が集合あるからです。 $\mathfrak{S}$ は基底となります。

ここで 2 番目の主張を証明します。まず、F が基礎体の場合、定義から、$E' = \mathscr{L}(E; F)$ 上の $\tilde{\mathfrak{S}}$ トポロジーは、基本として 0 の近傍の系、極の集合の集合を有することがわかります。 $\tilde{\mathfrak{S}}$。 A を E の有界部分集合とし、その極 $A^\circ$ が $\tilde{\mathfrak{S}}$ トポロジの 0 の近傍であるとします。その場合、$A^\circ \supset B^\circ$、つまり$A \subset B^{\circ \circ}$ となるような閉じた凸のバランスの取れた集合 $B \in \tilde{\mathfrak{S}}$ が存在します。しかし、コルによって。 II、p. 45 の 3 つには、$B^{\circ \circ} = B$ があるため、$A \subset B$ と $A \in \tilde{\mathfrak{S}}$ になります。したがって、$\mathfrak{S}'$ が E の有界部分集合の集合である場合、$\mathfrak{S}' \subset \tilde{\mathfrak{S}}$ の場合に限り、$\mathfrak{S}'$ トポロジーは $E'$ の $\mathfrak{S}$ トポロジーより粗くなります。 $y \in F$ が 0 の閉包内にない場合、$f \in E'$ 対応するを写像 $x \mapsto f(x)\ y$ にする写像は、その上に局所的に凸な空間 $E'_\mathfrak{S}$ の同型であることが検証できるため、一般的なケースがすぐに続きます。 $\mathscr{L}_{\tilde{\mathfrak{S}}}(E; F)$の像。

### 2. 条件、$\mathscr{L}_\mathfrak{S}(E; F)$はハウスドルフになります

#### 命題 3 {#evt-iii-s3-prop-3 .statement tag=07MS}

— E と F を 2 つの局所凸空間とし、F をハウスドルフと仮定し、$\mathfrak{S}$ を E の有界部分集合の族とします。 $\mathfrak{S}$ の集合の和集合 A が E で合計である場合、空間 $\mathscr{L}_\mathfrak{S}(E; F)$ は次のようになります。ハウスドルフ。

$u_0$ を $\mathscr{L}(E; F)$ の非ゼロ元とします。 $u_0$ は連続であり、A は E の合計であるため、A には $u_0(x_0) \neq 0$ となるような $x_0$ が存在します。 F はハウスドルフなので、$u_0(x_0) \notin V$ となるような 0 の F には近傍 V が存在します。 $M \in \mathfrak{S}$ を $x_0 \in M$ となるようにします。次に、$u(M) \subset V$ が $\mathscr{L}(E; F)$ の 0 の近傍となるように、すべての $u \in \mathscr{L}(E; F)$ の集合 U が得られ、$u_0 \notin U$ が得られるため、$\mathscr{L}(E; F)$ はハウスドルフになります。

特に、$\mathscr{L}(E; F)$ 上の次のトポロジは、F が Hausdorff である場合は常に Hausdorff です: 単純収束、コンパクト収束、プレコンパクトまたはコンパクト凸、および有界収束。

### 3. $\mathscr{L}(E; F)$と$\mathscr{L}(\hat{E}; F)$の間の関係

E と F の 2 つのハウスドルフが局所的に凸空間とし、F が完全であると仮定します。 $\hat{E}$ を E の完成とします。E から F 拡大するまでのすべての連続線形写像 $u$ は、$\hat{E}$ から F までの連続線形写像 $\bar{u}$ となるため、同一視できる空間 $\mathscr{L}(E; F)$ となります。 $\mathscr{L}(\hat{E}; F)$ by 写像 $u \mapsto \bar{u}$。 加法では、$\mathfrak{S}$ を E の有界な部分集合の族とします。 $\mathscr{L}(E; F)$ 一致するの $\mathfrak{S}$ トポロジと $\mathscr{L}(\hat{E}; F)$ の $\mathfrak{S}$ トポロジ、および $\hat{\mathfrak{S}}$ トポロジ。ここで、$\hat{\mathfrak{S}}$ は、集合の $\hat{E}$ のクロージャーのファミリーを示します。 $\mathfrak{S}$。

たとえば、E が *ノルム* の場合、$\mathscr{L}(E; F)$ での有界収束の位相は、$\mathscr{L}(\hat{E}; F)$ での有界収束の位相と同一です。つまり、$\hat{E}$ のすべての有界部分集合は E の有界部分集合の閉包に含まれます。 $\hat{E}$ の単位元球は E の単位元球の閉包であり、公式 (3) (III, p. 14) から、F がバナハ空間である場合、写像 $u \mapsto \bar{u}$ は$\mathscr{L}(E; F)$から$\mathscr{L}(\hat{E}; F)$へ。

E がノルム空間でない場合、E のどの有界部分集合の閉包にも含まれない $\hat{E}$ の有界部分集合が存在する可能性があることが観察されます (たとえば、E が無限次元バナッハ空間の弱い双対である場合)。ただし、これは、E が計量可能であり、可算性の最初の公理を満たす場合に当てはまります (III、p. 39、演習 16)。

### 4. 等連続部分集合/$\mathscr{L}(E; F)$

E と F を 2 つの局所凸空間とします。 $\mathscr{L}(E; F)$ の部分集合 H が等連続であるためには、E の点 0 で等連続であることが必要かつ十分です (I, p. 9、提案 6)。これは、F の 0 の近傍 V ごとに、E の 0 の集合 $\bigcap_{u \in H} u^{-1}(V)$ が近傍であることを意味します。または、F 上のすべての連続半ノルム $p$ について、写像 $\sup_{u \in H} (p \circ u)$ は E 上の連続半ノルムです。さらに (I, p. 5)、H は一様に等連続です。等連続部分集合の凸平衡包絡線が等連続であることに注意します。 $p$ が F の連続半ノルムであり、H の凸平衡包絡線 $\tilde{H}$ である場合、H の $u_i$ に対して、不等式 $p \circ (\sum_i \lambda_i u_i) \leq \sum_i |\lambda_i| \cdot (p \circ u_i)$ が得られるため、次のようになります。 $\sup_{u \in H} (p \circ u) = \sup_{u \in \tilde{H}} (p \circ u)$。

従って、等連続部分集合の族は、$\mathscr{L}(E; F)$ (III, p. 2, def. 2) 上の凸型ボーンロジーになります。

#### 命題 4 {#evt-iii-s3-prop-4 .statement tag=07MT}

*E、F を局所 2 凸空間、F をハウスドルフとする。 E から F までのすべての写像の空間 $F^E$ に、単純収束の位相が割り当てられるとします。それから*

(i) *E から F への線形写像の集合は $F^E$ で閉じられます。*

(ii) *H が $\mathscr{L}(E; F)$ の等連続部分集合である場合、$F^E$ の H の閉包 $\overline{H}$ は $\mathscr{L}(E; F)$ に含まれており、等連続です。*

$\overline{H}$ は等連続であることがわかっています (GT、X, § 2, No. 3、提案 6)。 主張 (i) を証明することはまだ残っています。 x、y を E に、$\lambda, \mu$ を K に、$A(x, y, \lambda, \mu)$ をすべての $u \in F^E$ の集合とします。

$$
u(\lambda x + \mu y) - \lambda u(x) - \mu u(y) = 0 .
$$

この集合は、$F^E$ から F への写像 $u \mapsto u(x)$ が $x \in E$ ごとに連続であり、F がハウスドルフであるため、$F^E$ で閉じられます。しかし、E から F への線形写像の集合は次と等しいです。

$$
\bigcap_{x,y,\lambda,\mu} A(x, y, \lambda, \mu) .
$$

従って、この集合は$F^E$に閉鎖されます。

#### 系 1 {#evt-iii-s3-prop-4-cor-1 .statement tag=07MU}

— *$\mathscr{L}(E; F)$の等連続部分集合 Hが$\mathscr{L}_s(E; F)$で比較的コンパクトであるためには、すべての$x \in E$、集合$H(x)$、$u$がHを超える範囲のすべての$u(x)$がFで比較的コンパクトであることが必要かつ十分です。

実際、$\overline{H}$を$F^E$（GT、I, § 9, No. 5、cor.）でコンパクトにするためには、この条件が必要十分です。

#### 系 2 {#evt-iii-s3-prop-4-cor-2 .statement tag=07MV}

— *E の双対 $E'$ の各等連続部分集合は、$E'$* 上の弱い位相 $\sigma(E', E)$ (III、p. 14、例 4) にとって比較的コンパクトです。

なぜなら、H が $E'$ の等連続部分集合である場合、$\sup_{u \in H} |u|$ は E 上の連続半ノルムです。特に、すべての $x \in E$、集合 $H(x)$ は有界であるため、体のスカラーでは比較的コンパクトです。

#### 系 3 {#evt-iii-s3-prop-4-cor-3 .statement tag=07MW}

— *セミノルム空間 E の強いデュアル $E'_b$ では、すべてのクローズ ボールは弱い位相 $\sigma(E', E)$ にとってコンパクトです。*

このボールも$\sigma(E', E)$でクローズされています。

#### 命題 5 {#evt-iii-s3-prop-5 .statement tag=07MX}

— *E と F を 2 つの局所凸空間とし、T を E の合計部分集合とします。$\mathscr{L}(E; F)$ の等連続部分集合 H ごとに次の均一構造一致する:*

1) *T における単純収束の一様構造;*
2) *E における単純収束の一様構造;*
3) *E のプレコンパクト部分集合における収束の一様構造。*

(III、p. 15、提案 2) $\mathscr{L}(E; F)$ 一致する上の $\mathfrak{S}$ トポロジーが $\tilde{\mathfrak{S}}$ トポロジーを持ち、$\tilde{\mathfrak{S}}$ が E および含む $\mathfrak{S}$ に適応した最小のボーンロジーであることを思い出します。

プロップの主張にあります。 5、したがって、「どこでも密」で置き換える語「合計」ができます。 命題は等連続集合 (GT, X, § 2, No. 4, th. 1) の一般特性から得られます。

#### 例 {#evt-iii-s3-n4-exa-1 .statement tag=07MY}

— *1) $\mathbf{R}$ のルベーグ測度を $\mu$ とし、半正規化空間 $\mathscr{L}^p(\mu)$ ($1 \leq p < \infty$) (INT, IV) を E とします。 すべての数値写像 $f$ およびすべての実数 $h$ について、$f_h$ を写像 $x \mapsto f(x - h)$ とします。 明らかに写像 $f \mapsto f_h$ 定義する E からそれ自体への線形アイソメトリです。 $f$ が連続でコンパクトなサポートがある場合、$f_h$ は一様に $f$ に収束します。したがって、$h$ が 0 になる傾向があるため、位数 $p$ の平均も同様です。 Since the set $\mathscr{K}(\mathbf{R})$ of all continuous functions with compact support is dense in E, and the set of linear isometries of E is equicontinuous, it follows from prop. 5 that for every $f \in E$, $f_h$ converges in the mean of order $p$ to $f$ as $h$ tends to 0.

$p = 1$ については、次のように定義される $\mathbf{R}$ 上の各 $f \in \mathscr{L}^1(\mu)$ 写像 $\hat{f}$ に関連するフーリエ変換を考慮します。

$$
\hat{f}(y) = \int e^{-2i\pi xy} f(x) \, d\mu(x) .
$$

線型形式 $f \mapsto \hat{f}(y)$ の集合は、$\mathscr{L}^1(\mu)$ の双対の等連続部分集合です。

一方、閉じた有界区間のすべての特性写像の集合 T は、$\mathscr{L}^1(\mu)$ の合計部分集合であることがわかります。そして、すべての $f \in T$ について、フーリエ変換 $\hat{f}$ が無限遠で零になる傾向がある連続写像であることを簡単に検証します。これはすべての $f \in \mathscr{L}^1(\mu)$ (「リーマン・ルベーグ定理」) に当てはまると推測します。

関係 $\sup_{y \in \mathbf{R}} |\hat{f}(y)| \leq \|f\|_1$ は、写像 $f \mapsto \hat{f}$ が、$\mathbf{R}$ で境界のあるすべての写像のうち、$\mathscr{L}^1(\mu)$ から空間 $\mathscr{B}(\mathbf{R})$ まで連続する写像であり、構造が一様収束していることを示しています。 $\hat{f}$はすべての$f \in T$に対して連続であるため、$\hat{f}$はすべての$f \in L^1(\mu)$に対して連続であるということになります。 $\hat{f}$ が無限遠で零になる傾向があるという事実は、無限遠で零になる傾向があるすべての連続写像のうち部分空間 $C_0(\mathbf{R})$ が $\mathscr{B}(\mathbf{R})$ で閉じられるという事実から帰結します。

2) E を、$\mathbf{R}$ 上のすべての連続数値写像の空間とし、位相のコンパクトな収束を与えます。 K を $\mathbf{R}$ のコンパクト部分集合とし、$(\mu_n)$ を K でサポートされた $\mathbf{R}$ のメジャーの数列とします。すべての n について $\|\mu_n\| \leq 1$ を仮定します。 $\mu_n$ の集合は、E' の等連続部分集合になります。したがって、すべての写像 $f \in E$ に対して $\lim_{n \to \infty} \mu_n(f) = 0$ がある場合、写像 $x \mapsto \int e^{itx} d\mu_n(t)$ の数列は、$\mathbf{R}$ のすべてのコンパクト部分集合で一律に 0 に収束します (写像の集合以降) $t \mapsto e^{itx}$ は、x の範囲が $\mathbf{R}$ のコンパクトな部分集合を超えているため、E) ではコンパクトです。 \*

#### 系 {#evt-iii-s3-n4-cor-1 .statement tag=07MZ}

— *F がハウスドルフであると仮定します。 H を $\mathscr{L}(E; F)$ の等連続部分集合とします。 H のフィルター $\Phi$ が E から F への写像 $u_0$ に単純に収束する場合、$u_0$ は E から F への連続線形写像であり、$\Phi$ は E のすべての事前圧縮部分集合で一様に $u_0$ に収束します。

最初の主張は prop から続きます。 4 (III、p. 16) とプロップからの 2 番目。 5 (III、p. 17)。

#### 命題 6 {#evt-iii-s3-prop-6 .statement tag=07N0}

— *H を $\mathscr{L}(E; F)$ の等連続部分集合とします。 F が計量可能であり、E に可算合計集合が存在する場合、E の単純収束の H 上の一様構造は計量可能です。 加法において、F に可算合計集合が存在する場合、H には可算どこでも密な集合が存在します (E のコンパクト部分集合への一様収束の位相について)。

$(a_n)$ を E の合計数列とします。すると、写像 $u \mapsto (u(a_n))$ は $\mathscr{L}(E; F)$ からの同型です。ここで、$\mathscr{L}(E; F)$ は、$a_n$ の集合を均一に収束させた単純な収束の均一構造を持ちます。 $F^\mathbf{N}$中部分空間。 F が計量可能 (それぞれ計量可能で可算性の最初の公理を満たす) 場合、これは $F^\mathbf{N}$ (GT、IX, § 2, No. 4、cor. 2 および § 2, No. 8、系) にも当てはまり、命題は prop から続きます。 5 (III、p. 17)。

#### 系 1 {#evt-iii-s3-prop-6-cor-1 .statement tag=07N1}

— *E を局所的に凸な計化可能空間とし、F を正規化空間とする。 E と F が両方とも満たす可算性の最初の公理であると仮定します。このとき、$\mathscr{L}(E; F)$ は等連続部分集合の可算族の和集合であり、$\mathscr{L}(E; F)$ には E の事前圧縮部分集合の一様収束の位相にとって密な可算集合が存在します。

Let B be the unit ball of F and $(V_n)$ a countable fundamental system of neighbourhoods of 0 in E. すべての整数 n、すべての $u \in \mathscr{L}(E; F)$ の集合 $H_n$ について、$u(V_n) \subset B$ は等連続で、$\mathscr{L}(E; F)$ は $H_n$ の和集合になります。 系は prop から続きます。 6.*

#### 系 2 {#evt-iii-s3-prop-6-cor-2 .statement tag=07N2}

— *可算性の最初の公理であるノルム空間満たすの双対 E' 内のすべての閉じた球は、弱い位相 σ(E', E) に対してコンパクトな計論可能空間であり、この位相に対して E'* には可算密集部分集合が存在します。

これはプロップから続きます。 6 と III、p. 17、cor から。 3.

### 5. 等連続部分集合/$E'$

この切断において、Eは局所的に凸な空間とその双対である$E'$を表します。 E の集合 M の極 $M^\circ$ (それぞれ $E'$) について話すときは常に、別の言い方をすれば、E と $E'$ の双対性に対する M の極 〜でない限りを意味します。 V が E の 0 の閉じた凸平衡近傍である場合、$V^{\circ\circ} = V$ (II, p. 45, cor. 3) があることを思い出してください。

#### 命題 7 {#evt-iii-s3-prop-7 .statement tag=07N3}

— *M を $E'$ の部分集合とします。次の条件は同等です:*

(i) $M$ *等連続* ;
(ii) $M$ * は E* の 0 の近傍の極に含まれます。
(iii) M の *polar は E* の 0 の近傍です。

M が等連続の場合、すべての $x \in V$ とすべての $u \in M$ に対して $|u(x)| \leq 1$ となる、0 の凸平衡近傍 V が存在します。次に、$M \subset V^\circ$ が得られ、(i) は (ii) を意味します。同じ記法でも、$M \subset V^\circ$なら$V \subset V^{\circ\circ} \subset M^\circ$となり、(ii)は(iii)を意味します。最後に、$M^\circ$ 含むが 0 の凸平衡近傍 V である場合、$M \subset M^{\circ\circ} \subset V^\circ$ と関係 $x \in \varepsilon V,\ u \in M$ はすべての $\varepsilon > 0$ に対して $|u(x)| \leq \varepsilon$ を意味し、これは (iii) が (i) を意味することを証明します。

$E'$ から K へのすべての $x \in E$ 定義する写像 $j(x): u \mapsto u(x)$ は、E 上の $\mathscr{S}$ トポロジーについて話すことができます。ここで、$\mathscr{S}$ は、$E'$ の部分集合のファミリーです。これは、以下の逆像です。 $K^{E'}$ の $\mathscr{S}$ トポロジの $j$。 $\mathscr{S}$ が $E'$ 上の凸ボーンロジーである場合、$\mathscr{S}$ 形の集合の極は、E 上の $\mathscr{S}$ トポロジーの 0 の近傍の基本系であることをすぐに検証します。これは、特に次の場合に当てはまります。 $\mathscr{S}$ は、$E'$ とプロップの等連続部分集合の族です。 7 は次のことを意味します:

#### 系 1 {#evt-iii-s3-prop-7-cor-1 .statement tag=07N4}

— E の *位相は、$E'$* の等連続部分集合上の一様収束の位相と同一です。

より一般的には、F を局所的に凸な空間とします。 $u \in \mathscr{L}(E; F)$ 定義する写像 $j(u):(x, f) \mapsto f(u(x))$ を $E \times F'$ から K に変換します (*つまり* $\mathbf{R}$ または $\mathbf{C}$ に)。これにより、$E \times F'$ の部分集合の集合上で一様収束の定義する、空間 $\mathscr{L}(E; F)$、位相が可能になります。特に ：

#### 系 2 {#evt-iii-s3-prop-7-cor-2 .statement tag=07N5}

— *$\mathscr{S}$ を E の有界部分集合の族とします。 $\mathscr{L}(E; F)$ の $\mathscr{S}$-トポロジーは、形 $A \times B \subset E \times F'$ の集合上で一様収束の位相であり、A は $\mathscr{S}$ にあり、B 属するは、等連続部分集合 of $F'$* の族。

すべての $u \in \mathscr{L}(E; F)$、すべての $A \in \mathscr{S}$、および F の 0 のすべての閉じた凸平衡近傍 V について、関係 $u(A) \subset V$ は、« $j(u)(A \times V^\circ)$ が K の単位元ボールに含まれる » と同等です。

#### 命題 8 {#evt-iii-s3-prop-8 .statement tag=07N6}

— *H を E から局所的に凸な空間 F への線形写像の族とする。H が等連続であるためには、F の双対 F' のすべての等連続部分集合 X、線型形式 f \circ u の集合、f \in X および u について必要かつ十分である。 \in H は等連続です。

条件が必要であることは明らかです。それが検証され、V が F の 0 の閉じた凸平衡近傍であるとします。 V^\circ は等連続であるため、|f(u(x))| となるような 0 の近傍 W が E に存在します。 \leq すべての x \in W、u \in H、および f \in V^\circ に対して 1。他の語では、H 内のすべての u \ に対して u(W) \部分集合 V^{\circ\circ} = V となるため、H は等連続です。

### 6. 局所凸空間の完成

#### 定理 1 (グロタンディーク) {#evt-iii-s3-thm-1 .statement tag=07N7}

— E を局所凸空間とし、\mathscr{S} を E 上で適応されカバーするボーンロジーとします。F \部分集合 E^* を、E 上の線型形式の空間とし、その制限から各集合所属から \mathscr{S} までが連続であるものとします。 F に \mathscr{S} トポロジが割り当てられている場合、E'_\mathscr{S} から F への標準単射から F への E'_\mathscr{S} の補完 \hat{E}'_\mathscr{S} から拡大するから同型になります。

E 上の線型形式のすべての単純な極限は線型形式 (III, p. 16, prop. 4) であり、E 上のボーンロジー \mathscr{S} がカバーしているため、GT、X, § 1, No. 6、cor から続きます。 2 \mathscr{S}-トポロジーを備えた空間 F はハウスドルフであり、完全です。 E'_\mathscr{S} が F の位相幾何学的ベクトル部分空間であることは明らかです。従って、E'_\mathscr{S} が F のどこでも密であることを証明するだけで十分です。これは、次の補題から得られます。

#### 補題 1 {#evt-iii-s3-lem-1 .statement tag=07N8}

A を E の閉じた凸平衡部分集合とし、u を A への制限が連続である E 上の線型形式とします。そして、すべての \varepsilon > 0 に対して、次のような x' \in E' が存在します。

$$ |u(x) - \langle x, x' \rangle| \leq \varepsilon \quad \text{for every} \quad x \in A . $$

\varepsilon > 0 とします。 |u(x)| となるような、E に 0 の閉じた凸平衡近傍 U が存在します。 \leq \varepsilon for all x \in U \cap A. E* の U の極 U^\circ は E' に含まれており、位相 \sigma(E^*, E) (III, p. 17, cor. 2) に対してコンパクトであることがわかっています。 E* における A の極 A^\circ は \sigma(E^*, E) に対して閉じているため、A^\circ + U^\circ は E* の閉じた凸型部分集合 (GT, III, § 4, No. 1, cor. 1) になります。

C を E の閉じた凸平衡部分集合とします。すると、C は \sigma(E, E') (II, p. 45, cor. 3) に対して閉じており、従って \sigma(E, E^*) に対しても閉じられ、帰結として、C = が得られます。 C^{\circ\circ} (E と E* の双対性の場合)。その結果、

$$ A \cap U = A^{\circ\circ} \cap U^{\circ\circ} = (A^\circ \cup U^\circ)^\circ \supset (A^\circ + U^\circ)^\circ $$

そこから、

$$ (A \cap U)^\circ \subset (A^\circ + U^\circ)^{\circ\circ} = A^\circ + U^\circ . $$

線型形式 \varepsilon^{-1}u 属するから (A \cap U)^\circ なので、u = \varepsilon(v + w) となる v \in A^\circ と w \in U^\circ が存在します。従って、x' = \varepsilon w 属するから E' であり、u - x' = \varepsilon v は、A 上の \varepsilon によって絶対値値より上に制限されます。したがって補題です。

ここで E を局所凸ハウスドルフ空間とし、その完成を \hat{E} とします。 E 拡大する上のすべての連続線型形式 f は連続性により \hat{E} になります。従って、(\hat{E})' = E' になります。

(III、p. 16) および $E'$ の $\hat{E}$ 定義する線型形式のすべての元。つまり、$E'$ の代数双対 ${E'}^*$ の元です。 加法では、$E$ (それぞれ $\hat{E}$) と $E'$ の間の二重性が分離しています (II、p. 24、cor. 1)。従って、$E$ と $\hat{E}$ は、${E'}^*$ のベクトル部分空間と識別できます。

#### 定理 2 {#evt-iii-s3-thm-2 .statement tag=07N9}

*$E$ を局所凸ハウスドルフ空間とし、その完成を $\hat{E}$ とします。私たちは同一視する $E$ と $\hat{E}$ と ${E'}^*$ のベクトル部分空間です。次に、元 $f \in {E'}^*$ ～ 属する ～ $\hat{E}$ については、$f$ の制限から $E'$ の各等連続部分集合が位相 $\sigma(E', E)$ にわたって連続していることが必要十分です。

空間 $E$ は、$E'$ が位相 $\sigma(E', E)$ に割り当てられる場合、$E'$ の位相双対で識別できます (II、p. 43、提案 3)。一方、$\mathscr{S}$ が $E'$ の等連続部分集合の集合である場合、$E$ 上の指定された位相は $\mathscr{S}$ トポロジー (III, p. 19, cor. 1) です。次に、III、p. 13、プロップから続きます。 1、$\mathscr{S}$ の集合は $\sigma(E', E)$ に限定されます (*cf.* 後で、III、p. 22、提案 9)。他の語では、$\mathscr{S}$ は位相 $\sigma(E', E)$ をカバーする適応された生まれ系学です。 定理 2 は th の帰結になります。 $E'$ で置き換える $E$ を、$E$ で $E'_\mathscr{S}$ を計算すると、1 になります。

#### 系 1 (バナッハ) {#evt-iii-s3-thm-2-cor-1 .statement tag=07NA}

— *$E$ をハウスドルフとし、局所凸型空間を完成させます。 In order that a linear form on $E'$ be continuous for the weak topology $\sigma(E', E)$ (i.e. arises from an element of $E$) it is sufficient that its restriction to every equicontinuous subset of $E'$ is continuous for $\sigma(E', E)$.*

#### 注意 {#evt-iii-s3-n6-rem-1 .statement tag=07NB}

— 加法において、$E$ に可算合計集合が存在すると仮定します。その場合、$E'$ のすべての等連続部分集合は、位相 $\sigma(E', E)$ に対して計量可能です (III, p. 18、提案 6)。したがって、$E'$ 上の線型形式 $u$ が弱連続であることを検証するには、$\sigma(E', E)$ で 0 に収束する$E'$ のすべての *等連続数列* $(x'_n)$ について、$\lim_{n \to \infty} u(x'_n) = 0$ があることを検証するだけで十分です。

#### 系 2 {#evt-iii-s3-thm-2-cor-2 .statement tag=07NC}

*$(E_i)_{i \in I}$ を局所凸ハウスドルフ族空間とし、$E$ をそれらのトポロジー 直和とします。すると、$\hat{E}_i$の直和から$\hat{E}$への標準写像は同型になります。特に、$E$ は、すべての $E_i$ が完了した場合にのみ完了します。*

$E$ の双対は、$E_i$ の双対の積 (II、p. 30、公式 (1)) と識別できることがわかっています。 $u \in \hat{E}$ とし、$u_i \in {E_i'}^*$ を $u$ の制限 (${E'}^*$ の元とみなします) から $E_i' \subset E'$ とします。 添字 $i \in I$ の有限数を除いて、$u_i = 0$ を証明するのに十分であるのは明らかです。 逆に、$u_{i_n} \neq 0$ のような異なる添字の数列 $(i_n)_{n \in \mathbf{N}}$ が存在すると仮定します。 そして、$u_{i_n}(x_{i_n}) = n$となるような$x_{i_n} \in E_{i_n}'$が存在します。 The set $H$ of all $x_{i_n}$ is equicontinuous in $E'$ and the restriction of $u$ to $H$ is not bounded, which is impossible.

### 7. $\mathscr{S}$-$\mathscr{L}(E; F)$ の系統学

$E$ と $F$ を 2 つの局所凸空間と $\mathscr{S}$ を $E$ の有界部分集合の族とする。 $\mathscr{L}(E; F)$ の部分集合 $H$ が $\mathscr{S}$ トポロジーに制限されているということは、すべての $M \in \mathscr{S}$ に対して、F の 0 のすべての近傍 $V$ が集合 $H(M) = \bigcup_{u \in H} u(M)$ を吸収することを意味します。これは、$M \in \mathscr{S}$ ごとに、集合 $H(M)$ が F で制限されるというというと同じです。同様に、これは、F の 0 のすべての近傍 $V$ について、集合 $\bigcap_{u \in H} u^{-1}(V)$ がすべての部分集合を吸収することを意味します。 $\mathscr{S}$中$M$。

#### 命題 9 {#evt-iii-s3-prop-9 .statement tag=07ND}

*E と F を 2 つの局所凸空間と E の有界部分集合の族である $\mathscr{S}$ とします。すると、$\mathscr{L}(E; F)$ のすべての等連続部分集合は $\mathscr{S}$ トポロジーに有界されます。

なぜなら、$H$がFの$\mathscr{L}(E; F)$と0の$V$近傍の等連続部分集合である場合、集合$\bigcap_{u \in H} u^{-1}(V)$はEの0の近傍であるため、Eのすべての有界部分集合を吸収します。

$\mathscr{S}$ トポロジーに限定される $\mathscr{L}(E; F)$ の部分集合は、たとえ $\mathscr{S}$ がカバーしていて、$\mathscr{S}$ が E 上の標準地表であるとしても、必ずしも等連続であるとは限りません (IV、p. 50、演習 17)。次の段落では、*バレル* 空間, 空間 E という名前で、$\mathscr{L}(E; F)$ の単純に有界されたすべての部分集合が等連続であるように研究します。現時点での注意の結果は次のとおりです。

#### 命題 10 {#evt-iii-s3-prop-10 .statement tag=07NE}

*E をボーンロジカル空間 (特に、計化可能な局所凸空間) とし、F を局所凸空間とします。有界収束の位相に制限される $\mathscr{L}(E; F)$ のすべての部分集合 H は等連続です。*

F の 0 の凸平衡近傍 $V$ ごとに、 集合 $\bigcap_{u \in H} u^{-1}(V)$ は E のすべての境界のある部分集合を吸収するため、 E の 0 の近傍になります。これは H が等連続であることを証明します。

### 8. 部分集合/$\mathscr{L}_{\mathscr{S}}(E; F)$を完了する

#### 命題 11 {#evt-iii-s3-prop-11 .statement tag=07NF}

*E と F を 2 つの局所的に凸な空間、$\mathscr{S}$ を有界部分集合の E からなるのカバーとする。 F がハウスドルフで準完全 (III、p. 8) の場合、$\mathscr{S}$ トポロジーで閉じている$\mathscr{L}(E; F)$ のすべての等連続部分集合 H は、$\mathscr{L}_{\mathscr{S}}(E; F)$ の完全一様部分空間です。

H は $\mathscr{L}_{\mathscr{S}}(E; F)$ (III、p. 22、提案 9) で有界され、$\mathscr{S}$ トポロジー (III、p. 16、提案 4) の $F^E$ で閉じられているため、これは cor. GTの3、X, § 1, No. 5。

#### 注意 1 {#evt-iii-s3-n8-rem-1 .statement tag=07NG}

— M を $\mathscr{L}_{\mathscr{S}}(E; F)$ の *完全な * 制服部分空間とします。 E の有界部分集合 $\mathscr{S}' \supset \mathscr{S}$ のすべての集合について、$\mathscr{S}'$-トポロジーは $\mathscr{L}(E; F)$ の $\mathscr{S}$-トポロジーよりより細かいです。一方、$\mathscr{S}'$-トポロジには 0 の近傍の基本的な系が存在します。これらは単純収束の位相 (III、p. 13、*注意 2*)、および *なおさら* に対して閉じられています。 $\mathscr{S}$-トポロジー。我々結論する (GT, III, § 3, No. 5, cor. 1) は、M が $\mathscr{S}'$ トポロジーに対して *完成* していると考えています。

#### 系 {#evt-iii-s3-n8-cor-1 .statement tag=07NH}

*E と F を 2 つの局所的に凸な空間、H を $\mathscr{L}(E; F)$ の等連続部分集合とする。 F がハウスドルフで準完全であり、H のフィルター $\Phi$ が E の合計部分集合 T のうち点に単純に収束*する場合、E から F への連続線形写像 u が存在し、すべてのプリコンパクトで $\Phi$ が一様に u に収束します。 Eの部分集合

なぜなら、プロップのおかげで。 5 (III, p. 17) $\Phi$ は、E のプリコンパクト収束の一様構造に対するコーシー フィルターです。プロップによって。図 11 では、$\mathscr{L}_{pc}(E; F)$ における H の閉包 $\overline{H}$ が完了しているため、$\Phi$ は E から写像 $u \in \overline{H}$ までのすべてのプレコンパクト部分集合で一様に収束します。

#### 注意 2 {#evt-iii-s3-n8-rem-2 .statement tag=07NI}

$(u_n)$ を Banach 空間 E から Banach 空間 F への連続線形写像の数列とします。 数列 $(u_n)$ が標準の空間 $\mathscr{L}(E; F)$ で制限されることなく、E のどこでも密なベクトル部分空間 T の各点で $(u_n(x))$ が極限を持つことが起こる可能性があります。たとえば、E を $\mathbf{R}$ 上のすべての連続数値写像の空間とし、無限遠ではノルム $\|f\| = \sup_{x \in \mathbf{R}} |f(x)|$ で零になる傾向があり、T をコンパクトなサポートを備えた連続数値写像の部分空間とします。 E から $\mathbf{R}$ までの連続線形写像 $f \mapsto nf(n)$ の数列は、すべての $f \in T$ で 0 に収束しますが、$\mathscr{L}_b(E; \mathbf{R})$ では境界がありません。同じ例は、空間 $\mathscr{L}(T; \mathbf{R})$、数列 $(v_n)$ が有界収束の位相に対して単に収束し、有界ではない可能性があることを示しています。

一方、連続線形写像$f \mapsto \sum_{k=1}^n f(k)$の数列は、単純収束の位相では$\mathscr{L}(T; \mathbf{R})$ではコーシー数列ですが、この位相では$\mathscr{L}(T; \mathbf{R})$では極限になる傾向がありません。

#### 命題 12 {#evt-iii-s3-prop-12 .statement tag=07NJ}

— *E を骨学的局所凸空間、F を完全局所凸ハウスドルフ空間、および $\mathfrak{S}$ を 0 に収束するすべての数列の E 含む像の有界部分集合の族とする。すると、空間 $\mathscr{L}_{\mathfrak{S}}(E; F)$ は次のようになります。完了しました。*

$\Phi$ を $\mathscr{L}_{\mathfrak{S}}(E; F)$ のコーシーフィルターとします。 この場合、$\Phi$ は単純収束の位相に対するコーシー フィルターであるため、$F^E$ に収束します。さらに、その極限 $u$ は E から F まで線形写像であり、$\Phi$ は $\mathfrak{S}$ の集合ごとに一様に $u$ に収束します (GT、X, § 1, No. 5、提案 5)。 したがって、零に収束する数列の $u$ の下の像は、零に収束する数列であるため、E はボーンロジカルであるため、$u$ は *連続* になります (III、p. 11、提案 1、(iii))。

#### 系 1 {#evt-iii-s3-prop-12-cor-1 .statement tag=07NK}

— *ボルノロジー 空間の強力な双対が完成しました。*

#### 系 2 {#evt-iii-s3-prop-12-cor-2 .statement tag=07NL}

— *E を半正規化空間とし、F を Banach (それぞれ Fréchet) 空間とします。 空間 $\mathscr{L}_b(E; F)$ は Banach (または Fréchet) 空間です。特に、半正規化空間の双対は Banach 空間です。*

### 練習問題 {#evt-iii-s3-exercises}

[§ 3 に対して練習問題](exercises/s3/)を参照してください。
