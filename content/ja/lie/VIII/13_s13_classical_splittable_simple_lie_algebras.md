---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: VIII
chapter_title: SPLIT SEMI-SIMPLE LIE ALGEBRAS
section: 13
section_title: Classical splittable simple Lie algebras
lang: ja
source: lie-vii-ix
book_pages: 189-218, 266-271
pdf_pages: 0197-0226, 0274-0279
extraction: native+ocr
subsections:
    - "no": 1
      title: ALGEBRAS OF TYPE A$_{\boldsymbol{l}}$ ($\boldsymbol{l}\geq$ 1)
      page: 190
      pdf_page: 198
    - "no": 2
      title: ALGEBRAS OF TYPE B$_{\boldsymbol{l}}$ ($\boldsymbol{l}\geq$ 1)
      page: 195
      pdf_page: 203
    - "no": 3
      title: ALGEBRAS OF TYPE C$_{\boldsymbol{l}}$ ($\boldsymbol{l}\geq$ 1)
      page: 204
      pdf_page: 212
    - "no": 4
      title: ALGEBRAS OF TYPE $\boldsymbol{D}_{\boldsymbol{l}}$ ($\boldsymbol{l}\geq$ 2)
      page: 211
      pdf_page: 219
statements: 2
exercises: 19
content_sha256: d5919c8cb8a52e67d552bc47eae5b72554d458b59f0541f873e81462d80e2b84
translated_from: content/en/lie/VIII/13_s13_classical_splittable_simple_lie_algebras.md
translation_method: google
source_content_sha256: 6374fb400438df5a36d2c913925fb0624256c5324de93a908a0b9247182f92f3
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: fb1a52d134ed4a579717aaed0f6eae7d243450e6c54c4245ca58239d58fb5a76
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## § 13。クラシックな分割可能なシンプルリー代数

この段落では、古典的な分割可能な単純なリー代数の各型について、明示的に説明します。

(I) この型の代数、その次元およびその分裂カルタン

部分代数;

(II) その根幹。

(III) そのボレル部分代数とその放物線部分代数;

(IV) 基本的には単純です表現;

(V) その基本的な単純な表現のうち、

直交またはシンプレクティック。

(VI) 不変式多項式関数の代数;

(VII) 群 Aut$\mathfrak{g}$、Aut$_0\mathfrak{g}$、Aut$_e\mathfrak{g}$ の特定のプロパティ。

(VIII) 制限の殺人形からカルタン部分代数;

(IX) シュバレー位数。

### 1. 代数 OF 型 A$_{\boldsymbol{l}}$ ($\boldsymbol{l}\geq$ 1)

(I) V を $k$ 上の次元 $l+ 1$ のベクトル空間とし、$\mathfrak{g}$ をトレース零の自己準同型の V の代数 $\mathfrak{s}\mathfrak{l}(V)$ とします。 $(e_i)_{1\leq i\leq l+1}$ を V の基底とします。 $\mathfrak{g}$の元に関連する写像は、この基底に関してその行列が、トレース零の行列の代数$\mathfrak{s}\mathfrak{l}(l+ 1, k)$と$\mathfrak{g}$の同一性です。 We know that $\mathfrak{g}$ is semi-simple (Chap. I, §6, no. 7, Prop. 8).

Recall (Algebra, Chap. II, §10, no. 3) that $E_{ij}$ denotes the matrix $(\alpha_{mp})$ such that $\alpha_{ij}= 1$ and $\alpha_{mp}= 0$ for $(m, p)\not= (i, j)$. 行列

$$
E_{ij}(1\leq i, j\leq l+ 1, i\not=j)
$$

$$
E_{i,i}-E_{i+1,i+1}(1\leq i\leq l)
$$

$\mathfrak{g}$ の形基底。従って、

薄暗い$\mathfrak{g}=l(l+ 2)$。

$\widehat{\mathfrak{h}}$ を $\mathfrak{g}\mathfrak{l}(l+ 1, k)$ の対角線元の集合とします。 数列 $(E_{ii})_{1\leq i\leq l+1}$ はベクトル空間 $\widehat{\mathfrak{h}}$ の基底です。 $(\widehat{\varepsilon}_i)_{1\leq i\leq l+1}$ を $\widehat{\mathfrak{h}}^*$ と $(E_{ii})_{1\leq i\leq l+1}$ の基底とします。 $h\in \widehat{\mathfrak{h}}$の皆様、

$$
[h, E_{ij}] = (\widehat{\varepsilon}_i(h)-\widehat{\varepsilon}_j(h))E_{ij} \tag{1}
$$

章著I, §1, no. 2、公式 (5)。 $\mathfrak{h}$をトレース零の$\widehat{\mathfrak{h}}$の元の集合とし、$\varepsilon_i= \widehat{\varepsilon}_i|\mathfrak{h}$を置きます。すると、$\mathfrak{h}$は$\mathfrak{g}$のカルタン部分代数になります（VII, §2, no. 1、例4章）。 関係 (1)は、このカルタン部分代数が分裂であり、$(\mathfrak{g},\mathfrak{h})$の根が$\varepsilon_i-\varepsilon_j(i\not=j)$であることを証明します。 $\widehat{\mathfrak{h}}^*_0$ を $(\widehat{\varepsilon}_i)$ に対する座標が零である $\widehat{\mathfrak{h}}^*$ 和の元の集合とします。 $\widehat{\mathfrak{h}}^*_0$ から $\mathfrak{h}^*$ までの写像 $\lambda  \rightarrow \lambda |\mathfrak{h}$ は全単射です。従って、$(\mathfrak{g},\mathfrak{h})$ の根系 R は型 $A_l$ になります (VI, §4, no. 7 章)。従って、$\mathfrak{g}$ は単純です (§3, no. 2、提案 6 の Cor. 1)。従って、$\mathfrak{g}$ は、型 $A_l$ の分割可能な単純なリー代数です。

$\mathfrak{g}$ のすべての分裂カルタン部分代数 $\mathfrak{h}'$ は、基本自己同型 (§3, no. 3、提案 10 の修正) の下では $\mathfrak{h}$ の変換です。 Aut$_e\mathfrak{g}$ は$\mathfrak{g}$ と$s\in \mathbf{S}\mathbf{L}(V)$ の自己同型$x \rightarrow sxs^{-1}$ (VII, §3, no. 1、注釈 2; cf. (VII)) の集合であるため、$\mathfrak{h}'$ が次のようなV の基底$\beta$ が存在します。基底$\beta$に関して行列が対角である$\mathfrak{g}$の要素の集合$\mathfrak{h}_{\beta}$。 $\mathfrak{h}_{\beta}$ 含む元と個別の固有値があるため、$\mathfrak{h}_{\beta}$ の元で安定しているV のベクトル部分空間は、$\beta$ の部分集合によって生成されたものだけです。 したがって、写像 $\beta  \rightarrow \mathfrak{h}_{\beta}$ 誘導するは、V の分解の集合から $l+ 1$ の部分空間次元 1 の直和へ商全単射への通過により、 集合/分裂カルタン部分代数/$\mathfrak{g}$。 (II) $\alpha =\varepsilon_i-\varepsilon_j(i\not=j)$ を根とします。 $\mathfrak{g}^{\alpha}=kE_{ij}$ があります。 以来

$$
[E_{ij}, E_{ji}] =E_{ii}-E_{jj}
$$

そして $\alpha (E_{ii}-E_{jj}) = 2$ 以降、 (§2, no. 2、Th. 1 (ii)) になります。

$$
H_{\alpha}=E_{ii}-E_{jj}
$$

(III) $\alpha_1=\varepsilon_1-\varepsilon_2, \alpha_2=\varepsilon_2-\varepsilon_3, . . . , \alpha_l=\varepsilon_l-\varepsilon_{l+1}$を入れます。章著。 VI, §4、いいえ。 $7.I, (\alpha_1, . . . , \alpha_l)$ は R の基底 B です。 B に対して正の根は、$i < j$ の $\varepsilon_i-\varepsilon_j$ です。 対応するボレル部分代数 $\mathfrak{b}$ は、トレース零の上三角行列の集合です。

V のフラグは、ベクトル部分空間の V の集合であり、$\{0\}$ や V とは異なり、完全に包含によって順序付けされています。 位数集合のV のフラグを含めます。最大のフラグは集合 $\{W_1, . . . ,W_l\}$ で、$W_i$ は $i$ 次元のベクトル部分空間です。

$$
W_1\subset  \cdots  \subset W_l
$$

たとえば、$V_i$ が $e_1, . . . , e_i$ によって生成された V の部分空間を表す場合、$\{V_1, . . . ,V_l\}$ は最大フラグです。

最大フラグ$\{V_1, . . . ,V_l\}$の安定した元を離れて、$\mathfrak{b}$が$\mathfrak{g}$の元の集合であるのは明らかです。逆に、$i < j$ の $\mathfrak{b}$ 含む $\mathfrak{h}$ と行列 $E_{ij}$ から、$\mathfrak{b}$ の下で安定している唯一の非自明なベクトル部分空間が$V_i$ であることがわかります。

ここで、$\delta$をVの最大フラグとします。前述のことから、$\mathfrak{g}$ の元の集合 $\mathfrak{b}_{\delta}$ が安定し、$\delta$ のすべての元は $\mathfrak{g}$ のボレル部分代数であることがわかります。 $\mathfrak{g}$ のすべてのボレル部分代数は基本自己同型の下では $\mathfrak{b}$ の変換であるため、写像 $\delta  \rightarrow \mathfrak{b}_{\delta}$ は最大フラグの集合から集合までの全単射であることがわかります。 $\mathfrak{g}$中ボレル部分代数。

$\beta$ を V の基底とします。 (I) とその前により、ボレル部分代数含む $\mathfrak{h}_{\beta}$ は、対応するから最大フラグまでの元が $\beta$ の部分集合によって生成されるものです。これらのフラグ対応するは、次の方法で $\beta$ の合計位数に全射的に変換されます。 $\beta$ の合計位数 $\omega$ には、フラグ $\{W_1, . . . ,W_l\}$ が関連付けられます。ここで、$W_i$ は、最初のフラグによって生成されたベクトル部分空間です。 位数 $\omega$ の $\beta$ の $i$ 元。 $(l+$ 1)があるので！ $\beta$ の合計位数から、$(l+$ 1) が存在するという事実がわかります。 $(\mathfrak{s}\mathfrak{l}(V),\mathfrak{h}_{\beta}) ($§3, no. 3のボレル部分代数、注意）。

$\gamma$をVのフラグとします。 $\gamma$は極大フラグに含まれているため、$\gamma$の安定した元を離れた$\mathfrak{g}$の元の集合$\mathfrak{p}_{\gamma}$は、$\mathfrak{g}$の放物線部分代数になります。 $\mathfrak{p}_{\gamma}$ で安定している唯一の非自明なベクトル部分空間は、$\gamma$ の元であることを示します。 このため、$\gamma =\{V_{i_1}, . . . ,V_{i_q}\}$ と $1\leq i_1<\cdots < i_q\leq l$ を仮定できます。 $i_0= 0, i_{q+1}=l+ 1$を入れてください。 空ではない区間

$$
i_0+ 1, i_1, i_1+ 1, i_2, . . . , i_q+ 1, i_{q+1}
$$

$\{1, . . . , l+ 1\}$ の形分割なので、位数 $l+ 1$ の任意の平方行列はブロック行列 $(X_{ab})_{1\leq a,b\leq q+1}$ と書くことができます。 代数 $\mathfrak{p}_{\gamma}$ は、元の $\mathfrak{p}_{i_1,...,i_q}$ $\mathfrak{s}\mathfrak{l}(l+ 1, k)$ の集合 $(X_{ab})_{1\leq a,b\leq q+1}$ となり、$a > b$ に対して $X_{ab}= 0$ になります。 $\mathfrak{p}_{i_1,...,i_q}\supset \mathfrak{b}$ 以降、$\mathfrak{p}_{i_1,...,i_q}$ で安定した自明でないベクトル部分空間は $V_i$ の 1 つです。 $i_k< i < i_{k+1}$、代数 $\mathfrak{p}_{i_1,...,i_q}$ 含む $E_{i_{k+1},i}$、$V_i$ が安定していない場合、主張になります。

その結果、最大フラグ $\{V_1, . . . ,V_l\}$ に含まれるフラグ $2^l$ は、$\mathfrak{b}$ を含む個別の放物線部分代数 $2^l$ を生成します。 $\mathfrak{b}($§3, no. 4 を含む放物線部分代数が正確に $2^l$ 存在するため、注釈)、写像 $\gamma  \rightarrow \mathfrak{p}_{\gamma}$ は V のフラグの集合から $\mathfrak{g}$ の放物線部分代数の集合への全単射であるということになります。 さらに、$\gamma \subset \gamma '$ の場合に限り、$\mathfrak{p}_{\gamma}\supset \mathfrak{p}_{\gamma'}$ になります。

放物線部分代数 $\mathfrak{p}=\mathfrak{p}_{i_1,...,i_q}(1\leq i_1<\cdots < i_q\leq l)$ を思い出してください。 $\mathfrak{s}$ (それぞれ $\mathfrak{n}$) を、$a\not=b$ (それぞれ $a\geq b$) に対して $X_{ab}= 0$ となるように、$\mathfrak{s}\mathfrak{l}(l+ 1, k)$ の $(X_{ab})_{1\leq a,b\leq q+1}$ の集合とします。 §3, no. 4 の提案 13 を考慮すると、$\mathfrak{p}=\mathfrak{s}\oplus \mathfrak{n}$、部分代数 $\mathfrak{s}$ は $\mathfrak{g}$ で還元的であり、$\mathfrak{n}$ は最大のの虚数イデアルと $\mathfrak{p}$ の虚数根基の両方です。

(IV) $r= 1,2, . . . , l$ の場合、$\varpi_r=\varepsilon_1+\cdots +\varepsilon_r$ とします。 $\varpi_i(H_{\alpha_j}) =\delta_{ij}$があるので、$\varpi_r$は重み対応するから$\alpha_r$が基本です。

$\sigma$ を、V における $\mathfrak{g}$ の同一性表現とします。 $\sigma$の外装冪$\bigwedge^r\sigma$は、$E =\bigwedge^r(V)$の表現です。 $(e_1, . . . , e_{l+1})$ を V から選ばれた基底とします。 $e_{i_1}\wedge  \cdots  \wedge e_{i_r}$、E の $i_1<\cdots < i_r$、形基底。$h\in \mathfrak{h}$ の場合、

$$
(\bigwedge^r\sigma )(h).e_{i_1}\wedge  \cdots  \wedge e_{i_r}= (\varepsilon_{i_1}+\cdots +\varepsilon_{i_r})(h)e_{i_1}\wedge  \cdots  \wedge e_{i_r}
$$

従って、すべての重みは重複度 $1,\varpi_r$ は $\bigwedge^r\sigma$ の重みであり、他のすべての重みは形 $\varpi_r-\mu$ であり、$\mu$ は正の根基重みです。従って、$\varpi_r$ は $\bigwedge^r\sigma$ の最高重量であり、$e_1\wedge \cdots \wedge e_r$ は原始値元です。章著。 VI, §4, no. 7.IX、ワイル群は、対称の群と識別できます。

$$
\{\varepsilon_1, . . . , \varepsilon_{l+1}\}
$$

ワイル群の下にある $\varpi_r$ の軌道は、したがって含むすべての $\varepsilon_{i_1}+\cdots +\varepsilon_{i_r}$ と $i_1<\cdots < i_r$ です。従って、原始関数元 $e_1\wedge  \cdots  \wedge e_r$ によって生成された単純部分加群は、すべての $\varepsilon_{i_1}+\cdots +\varepsilon_{i_r}$ を重みとして認め、結果として E に等しくなります。 従って、$\bigwedge^r\sigma$ は最高重量 $\varpi_r$ で既約です。

従って、表現 $\bigwedge^r\sigma (1\leq r\leq l)$ が基本的な表現です。ディム($\bigwedge^r\sigma$ ) $=(^{l+1}_r)$ があります。

(V) We have $w_0(\alpha_1) =-\alpha_l, w_0(\alpha_2) =-\alpha_{l-1}, . .$. (Chap. VI, §4, no. 7, XI), so

$$
-w_0(\varpi_1) =\varpi_l,-w_0(\varpi_2) =\varpi_{l-1}, . . .
$$

させて

$$
\omega =n_1\varpi_1+\cdots +n_l\varpi_l(n_1, . . . , n_l\in \mathbf{N})
$$

支配的な重みになります。この場合、単純な表現と最高重量 $\omega$ は、次の場合にのみ直交またはシンプレクティックになります。

$$
n_1=n_l,n_2=n_{l-1}, . .
$$

(§7, no. 5、提案 12)。特に、$l$ が偶数の場合、$\mathfrak{s}\mathfrak{l}(l+ 1, k)$ の基本表現はいずれも直交またはシンプレクティックではありません。 $l$ が奇数の場合、$i\not= (l+ 1)/2$ に対する表現 $\bigwedge^i\sigma$ は直交でもシンプレクティックでもありません。章著$(\alpha_1, . . . , \alpha_l)$に対する$\varpi_{(l+1)/2}$の座標のVI, §4, no. 7.VI、和は

$$
\frac{1}{l + 1}[\frac{l + 1}{2}(1 + 2 +\cdots +\frac{l- 1}{2})+\frac{l + 1}{2}(1 + 2 +\cdots +\frac{l + 1}{2})]
$$

$$
= 1 + 2 +\cdots +\frac{l- 1}{2}+\frac{l + 1}{4}
$$

したがって、$l\equiv  -1$ (mod. 4) の場合、$\bigwedge^{(l+1)/2}\sigma$ は直交し、$l\equiv 1$ (mod. 4) の場合、シンプレクティックです (§7, no. 5、提案 12)。この最後の結果は、次のようにしてより正確にすることができます。 $\bigwedge^{l+1}(V)$ で選ぶゼロ以外の元 $e$。外部の乗法代数 V 定義するからのバイリニア写像

$$
\bigwedge^{(l+1)/2}(V)\times \bigwedge^{(l+1)/2}(V)
$$

$\bigwedge^{l+1}$(V) に、$(u, v) \rightarrow \Phi (u, v)e$ と書くことができます。ここで、$\Phi$ は $\bigwedge^{(l+1)/2}(V)$ の双線形形式です。 $\Phi$ はゼロではなく、$\mathfrak{g}$ の下で不変 (したがって非縮退)、$(l+ 1)/2$ が偶数の場合は対称、$(l+ 1)/2$ が奇数の場合は交代的であることがすぐに検証されます。

(VI) すべての$x\in \mathfrak{g}$に対して、$\sigma (x) =x$の特性多項式を書くことができます

$$
T^{l+1}+f_2(x)T^{l-1}+f_3(x)T^{l-2}+\cdots +f_{l+1}(x)
$$

ここで、$f_2, . . . , f_{l+1}$ は $\mathfrak{g}($§8, no. 3、補題 2) の下で多項式関数は不変です。

$x=\xi_1E_{11}+\cdots +\xi_{l+1}E_{l+1l+1}\in \mathfrak{h}$ の場合、$f_i(x)$ は、符号まで、次数 $2, . . . , l+ 1$ の $\xi_1, . . . , \xi_{l+1}$ の基本対称写像です。したがって、Chap. VI, §4, no. 7.IX、元の $\mathbf{S}(\mathfrak{h}^*)$ の $f_i|\mathfrak{h}$ 生成する代数は、ワイル群の下で不変式であり、代数的に独立しています。したがって、(§8, no. 3, Prop. $3$)$f_2, f_3, . . . , f_{l+1}$ 生成する代数の多項式関数は、$\mathfrak{g}$ の下で不変であり、代数的に独立しています。

(VII) すべての $g\in \mathbf{G}\mathbf{L}(l+ 1, k)$ について、$\varphi_k(g) =\varphi (g)$ を $\mathfrak{g}$ の自己同型 $x \rightarrow gxg^{-1}$ とします。すると、$\varphi$は$\mathbf{G}\mathbf{L}(l+ 1, k)$からAut($\mathfrak{g}$)まで準同型になります。我々は持っています

$\varphi (\mathbf{S}\mathbf{L}(l+ 1, k)) =$ 秋$_e(\mathfrak{g})$

(VII, §3, no. 1章、備考2)。 $\overline{k}$ を $k$ の代数閉包とします。 我々は持っています

$$
\mathbf{G}\mathbf{L}(l+ 1,\overline{k}) = \overline{k}^*.\mathbf{S}\mathbf{L}(l+ 1,\overline{k})
$$

だから $\varphi_{\overline{k}}(\mathbf{G}\mathbf{L}(l+ 1,\overline{k})) =\varphi_{\overline{k}}(\mathbf{S}\mathbf{L}(l+ 1,\overline{k})) =$ Aut$_e(\mathfrak{g}\otimes_k\overline{k})$;したがって、$\varphi (\mathbf{G}\mathbf{L}(l+ 1, k))\subset$ Aut$_0(\mathfrak{g})$ となります。一方、Aut$_0(\mathfrak{g})\subset \varphi (\mathbf{G}\mathbf{L}(l+ 1, k))$ は、§7, no. 1 の提案 2 により、$\mathfrak{g}$ の同一性表現に適用されました。したがって、

オート$_0(\mathfrak{g}) =\varphi (\mathbf{G}\mathbf{L}(l+ 1, k))$。

$\varphi$ の核は $\mathbf{G}\mathbf{L}(l+ 1, k)$ の元の集合であり、位数 $l+1$ のすべての行列、つまり可逆スカラー 行列の集合 $k^*$ と可換です。したがって、Aut$_0(\mathfrak{g})$ は群 $\mathbf{G}\mathbf{L}(l+ 1, k)/k^*=\mathbf{P}\mathbf{G}\mathbf{L}(l+ 1, k)$ と識別できます。 $\varphi '=\varphi |\mathbf{S}\mathbf{L}(l+ 1, k)$の核は$\mu_{l+1}(k)$で、$\mu_{l+1}(k)$は$k$の単位元の1)番目根の$(l+$の集合を表します。したがって、Aut$_e(\mathfrak{g})$ は群 $\mathbf{S}\mathbf{L}(l+ 1, k)/\mu_{l+1}(k) =\mathbf{P}\mathbf{S}\mathbf{L}(l+ 1, k)$ と識別できます。一方、私たちは完全系列を持っています

1 $\longrightarrow \mathbf{S}\mathbf{L}(l+ 1, k)\longrightarrow \mathbf{G}\mathbf{L}(l+ 1, k)\longrightarrow^{det}k^*\longrightarrow$ 1

そして det の下の $k^*$ の像は $k^{*l+1}$ です。 標準同型あることになります。

8月$_0(\mathfrak{g})/$8月$_e(\mathfrak{g})\longrightarrow \mathbf{P}\mathbf{G}\mathbf{L}(l+ 1, k)/\mathbf{P}\mathbf{S}\mathbf{L}(l+ 1, k)$

$$
\longrightarrow \mathbf{G}\mathbf{L}(l+ 1, k)/k^*.\mathbf{S}\mathbf{L}(l+ 1, k)\longrightarrow k^*/k^{*l+1}
$$

$k$ = $\mathbf{R}$ の場合、$l+ 1$ が奇数の場合は Aut$_0(\mathfrak{g}) =$ Aut$_e(\mathfrak{g})$ が、$l+ 1$ が偶数の場合は Aut$_0(\mathfrak{g})/$Aut$_e(\mathfrak{g})$ が$\mathbf{Z}/2\mathbf{Z}$ と同型であることがわかります。

§$5,f(T_{\mathbf{Q}})$の記法は$\mathfrak{g}$の自己同型の集合であり、$\mathfrak{h}$上の恒等性は誘導するであるため、$\varphi$(D)に等しくなります。ここで、Dは元の対角集合です。 $\mathbf{G}\mathbf{L}(l+ 1, k) ($§5、提案 4)。 $D'$を$\mathbf{S}\mathbf{L}(l+ 1, k)$の対角元の集合とします。 §5 の提案 3 と Aut$_e(\mathfrak{g})$ の決定により、$f(q(T_P))\subset \varphi (D')$ が得られます。 $f(q(T_P)) =\varphi (D')$ を示します。しましょう

$\lambda_1$ 0

$d=$ 。 ..

0 $\lambda_{l+1}$

$D'$の元になります。すべての $i$ と $j$ に対して $\zeta (\varepsilon_i-\varepsilon_j) =\lambda_i\lambda^{-1}_j$ となるような $\zeta \in$ Hom(Q(R)$, k^*$) $= T_Q$ が存在します。 $f(\zeta ) =\varphi (d)$ であることを確認するのは簡単です。章著。 VI, §4, no. 7.VIII、P(R) は Q(R) と元 $\varepsilon =\varepsilon_1$ によって生成され、$P(R)/Q(R)$ の像は位数 $l+ 1$ です。しかし

$$
\zeta ((l+ 1)\varepsilon ) =\zeta ((\varepsilon_1-\varepsilon_2) + (\varepsilon_1-\varepsilon_3) +\cdots + (\varepsilon_1-\varepsilon_{l+1}))
$$

$$
=\lambda^l_1\lambda^{-1}_2\lambda^{-1}_3. . . \lambda^{-1}_{l+1}=\lambda^{l+1}_1
$$

つまり、P(R)から$k^*$まで$\zeta$拡大するから準同型になります。これは、$\zeta \in q(T_P)$、つまり $\varphi (d)\in f(q(T_P))$ であることを証明します。

(§5, no. 3、提案 5 の Cor. 2) を思い出してください。Aut($\mathfrak{g}$) $=$ Aut$_0(\mathfrak{g})$ は $l= 1$ に対して、Aut($\mathfrak{g}$)$/$Aut$_0(\mathfrak{g})$ は $l\geq 2$ に対して $\mathbf{Z}/2\mathbf{Z}$ と同型です。 写像 $\theta :x \rightarrow  -^tx$ は、$\mathfrak{s}\mathfrak{l}(l+ 1, k)$ の自己同型であり、$l\geq 2$ (VI, §4, no. 7.XI 章) の場合、$a_0=\theta |\mathfrak{h}\notin W$ なので、$a_0$ の類 Aut($\mathfrak{g}$)$/$Aut$_0(\mathfrak{g})$ は、この群の自明ではない元 (§5, no. 2、提案 4)。

(VIII)制限から$\mathfrak{h}$の殺人形は

$$
\Phi (\xi_1E_{11}+\cdots +\xi_{l+1}E_{l+1,l+1}, \xi '_1E_{11}+\cdots +\xi '_{l+1}E_{l+1,l+1})
$$

$$
=\sum_{i\not=j}(\xi_i-\xi_j)(\xi '_i-\xi '_j) =\sum_{i,j}(\xi_i-\xi_j)(\xi '_i-\xi '_j)
$$

$$
= (l+ 1)\sum_i\xi_i\xi '_i+ (l+ 1)\sum_j\xi_j\xi '_j-2(\sum_i\xi_i)(\sum_j\xi '_j
$$

$$
= 2(l+ 1)\sum_i\xi_i\xi '_i
$$

(IX) $1\leq i < j\leq l+ 1$には、

$$
X_{\varepsilon_i-\varepsilon_j}=E_{ij}X_{\varepsilon_j-\varepsilon_i}=-E_{ji}
$$

次に、すべての $\alpha \in R$ に対して、$[X_{\alpha}, X_{-\alpha}] =-H_{\alpha}$ と $\theta (X_{\alpha}) =X_{-\alpha}$ が得られます ($\theta$ は (VII) で紹介された自己同型 $x \rightarrow  -^tx$ です)。従って、$(X_{\alpha})_{\alpha\in R}$ は、$(\mathfrak{g},\mathfrak{h})$ のシュバレー 系になります。

$k=\mathbf{Q}$ を取ります。 $\mathfrak{h}($§12, no. 6 で許容される格子、Def。 1) $E_{ii}-E_{i+1,i+1}$ によって生成された $\mathbf{Z}$ モジュール $Q(R^{\vee})$、つまり対角線行列所属から $\mathfrak{s}\mathfrak{l}(l+ 1,\mathbf{Z})$ のからなると、$Q(R^{\vee})$ によって生成された $\mathbf{Z}$ モジュール $P(R^{\vee})$ の間にあるものであり、 $E_{11}-(l+ 1)^{-1}\sum E_{ii}$ (章 VI, §4, no. 7.VIII)、つまり、形 $x+ (l+ 1)^{-1}a.1$ のトレース零の対角線行列のからなるで、$x$ には整数のエントリがあり、 $a\in \mathbf{Z}$。従って、$\mathfrak{s}\mathfrak{l}(l+1,\mathbf{Z})$ は、許容格子 $Q(R^{\vee})$ と Chevalley 系 $(X_{\alpha})$ に関連付けられた $(\mathfrak{g},\mathfrak{h})$ の Chevalley 位数であるということになります。 $\bigwedge^r\mathbf{Z}^{l+1}$ が $\mathfrak{s}\mathfrak{l}(l+ 1,\mathbf{Z}) ($§12, no. 8 に対して $\bigwedge^r\mathbf{Q}^{l+1}$ で許容される格子であることを検証するのは簡単です。 3)。

一方、$\mathfrak{g}\mathfrak{l}(l+ 1,\mathbf{Z})$ は分裂還元的代数 $\mathfrak{g}\mathfrak{l}(l+ 1,\mathbf{Q})$ のシュバレー 位数です。 $\mathfrak{g}\mathfrak{l}(l+1,\mathbf{Q})$の中心$\mathbf{Q}.1$と平行な$\mathfrak{s}\mathfrak{l}(l+ 1,\mathbf{Q})$上の射影は、$\mathfrak{h}$の許容格子$P(R^{\vee})$とシュバレー系によって定義される$(\mathfrak{g},\mathfrak{h})$のシュバレー位数です。 $(X_{\alpha})$。 $\mathfrak{g}\mathfrak{l}(l+ 1,\mathbf{Z})$ は、$\mathfrak{s}\mathfrak{l}(l+ 1,\mathbf{Q})$ や $\mathfrak{g}\mathfrak{l}(l+ 1,\mathbf{Q})$ の中心とともに、共通部分の直和ではないことに注意します。

### 2. 代数 OF 型 B$_{\boldsymbol{l}}$ ($\boldsymbol{l}\geq$ 1)

(I) V を有限次元ベクトル空間とし、$\Psi$ を V 上の非縮退対称双線形形式とする。 自己準同型の集合、Vの$x$、すべての$v, v'\in V$の$\Psi (xv, v') +\Psi (v, xv') = 0$は、$\mathfrak{s}\mathfrak{l}$(V)の部分代数、暗い$V\not= 2$の半単純が嘘になります。 I, §6, no. 7、提案 9)。それを $\mathfrak{o}(\Psi )$ で表し、$\Psi$ に関連付けられた直交線リー代数と呼びます。

V は奇数次元 $2l+ 1\geq 3$ であり、$\Psi$ は最大添字 $l$ であると仮定します。 $\Psi$ が Q に関連付けられるような二次方程式形を Q で表します。 $x\in V$ に対して $Q(x) =\frac{1}{2}\Psi (x, x)$ が得られます。 代数まで、第 1 章IX, §4, no. 2、V は、2 つの最大完全等方性部分空間 F と $F'$ の直和と、非等方性で 1 次元である $F + F'$ の直交補数 G として書くことができます。 $\Psi$ にゼロ以外の定数を掛けるまでは、$\Psi (e_0, e_0) =-2$ となるような $e_0\in G$ が存在すると仮定できます。一方、F と $F'$ は $\Psi$ を介して双対関係にあります。 $(e_i)_{1\leq i\leq l}$をFの基底、$(e_{-i})_{1\leq i\leq l}$を$F'$の双対基底とします。それから

$$
(e_1, . . . , e_l, e_0, e_{-l}, . . . , e_{-1})
$$

は V の基底です。我々は持っています

$$
Q(\sum x_ie_i)=-x^2_0+\sum_{i=1}^{i=l}x_ix_{-i}
$$

そして、この基底に対する$\Psi$の行列は、位数$2l+ 1$の平方行列です

0 0 $\cdots$ 0 1

0 0 $s$ 0 0 $\cdots$ 1 0

$S=$ 0 $-2$ 0 $,s=$ ... ... 。 .. ... ...、

$s$ 0 0 0 1 $\cdots$ 0 0

1 0 $\cdots$ 0 0

ここで、$s$ は位数 $l$ の平方行列であり、そのエントリはすべて零ですが、2 番目の対角$^6$ 上のエントリは 1 に等しいです。前述のプロパティを持つ V の基底はウィットと呼ばれます。 Vの基底。 代数 $\mathfrak{g}=\mathfrak{o}(\Psi )$ は、$a=-S^{-1}aS($代数のように、正方行列の代数 $\mathfrak{o}_S(2l+ 1, k)$ 位数の $a$ $2l+ 1$ と識別できます。 IX, §1, no. 10、公式 (50))。簡単に計算すると、$\mathfrak{g}$ は形の行列の集合であることがわかります。

$$
A2s^txB
$$

$y$ 0 $x$ (2)

$$
C2s^tyD
$$

ここで、$x$ と $y$ は 1 行の行列で、$l$ 列と $A, B, C, D$ は位数 $l$ の正方行列で、$B=-s^tBs, C=-s^tCs$ と $D=-s^tAs$ です。 $\mathbf{M}_l(k)$ からそれ自体までの写像 $A \rightarrow s^tAs$ は 2 番目の対角線に関して対称であるため、次のようになります。

薄暗い$\mathfrak{g}= 2l+l^2+ 2\frac{l(l-1)}{2}=l(2l+ 1)$。

$\mathfrak{h}$を$\mathfrak{g}$の対角線元の集合とします。これは $\mathfrak{g}$ の可換部分代数で、基底元が含まれます

$^6$ 平方行列 $(a_{ij})_{1\leq i,j\leq n}$ の 2 番目の対角線は、次のような $a_{ij}$ の族です。

$$
i+j=n+ 1
$$

$$
H_i=E_{i,i}-E_{-i,-i}(1\leq i\leq l)
$$

$(\varepsilon_i)$ を $\mathfrak{h}^*$ と $(H_i)$ の基底とします。置く

$$
X_{\varepsilon_i}= 2E_{i,0}+E_{0,-i}(1\leq i\leq l)
$$

$X_{-\varepsilon_i}$ = $-2E_{-i,0}-E_{0,i}(1\leq i\leq l)$

$X_{\varepsilon_i-\varepsilon_j}$ = $E_{i,j}-E_{-j,-i}(1\leq i < j\leq l)$

$X_{\varepsilon_j-\varepsilon_i}$ = $-E_{j,i}+E_{-i,-j}(1\leq i < j\leq l)$ (3)

$X_{\varepsilon_i+\varepsilon_j}$ = $E_{i,-j}-E_{j,-i}(1\leq i < j\leq l)$

$X_{-\varepsilon_i-\varepsilon_j}$ = $-E_{-j,i}+E_{-i,j}(1\leq i < j\leq l)$。

これらの元形基底は $\mathfrak{g}$ の $\mathfrak{h}$ の補数であり、 $h\in \mathfrak{h}$ については、

$$
[h, X_{\alpha}] =\alpha (h)X_{\alpha} \tag{4}
$$

すべての $\alpha \in R$ に対して、R は $\pm \varepsilon_i$ と $\pm \varepsilon_i\pm \varepsilon_j(1\leq i < j\leq l)$ の集合です。 従って、$\mathfrak{h}$ は $\mathfrak{g}$ のノーマライザーと等しいため、$\mathfrak{g}$ のカルタン部分代数、$\mathfrak{h}$ は分裂、$(\mathfrak{g},\mathfrak{h})$ の根は R の元になります。 $(\mathfrak{g},\mathfrak{h})$ の根系 R は、$l\geq 2$ に対しては型 $B_l$ であり、$l= 1$ に対しては型 $A_1$ (型 $B_1$ であるとも言われています) です。 VI, §4, no. 5.I、$l= 1$の場合に拡張）。 従って、$\mathfrak{g}$ は、型 $B_l$ の分割可能な単純なリー代数です。

$\mathfrak{o}(\Psi )$ のすべての分裂カルタン部分代数は、$\mathfrak{o}(\Psi )$ の初等自己同型により $\mathfrak{h}$ の変換となり、従って $\mathbf{O}(\Psi )$ (cf. (VII)) の元により、結果として$\mathfrak{g}$の元の集合$\mathfrak{h}_{\beta}$で、Vのウィット基底$\beta$に対して行列が対角線です。 $\mathfrak{h}_{\beta}$ の下で唯一の不変式であるベクトル部分空間が、$\beta$ の部分集合によって生成されたものであることをすぐに検証します。

$l= 1$ の場合、代数 $\mathfrak{o}(\Psi )$ と $\mathfrak{s}\mathfrak{l}(2, k)$ は同じ根系を持ち、したがって同型です (cf. も §1、例題 16)。ここからは$l\geq 2$とします。

(II) 根系 $R^{\vee}$ は第 4 章によって決定されます。 VI, §4, no. 5.V そして、次のことがわかります。

$$
H_{\varepsilon_i}= 2H_i, H_{\varepsilon_i-\varepsilon_j}=H_i-H_j, H_{\varepsilon_i+\varepsilon_j}=H_i+H_j
$$

(III) $\alpha_1=\varepsilon_1-\varepsilon_2, . . . , \alpha_{l-1}=\varepsilon_{l-1}-\varepsilon_l, \alpha_l=\varepsilon_l$を入れます。章著。 VI, §4, no. 5.II、$(\alpha_1, . . . , \alpha_l)$ は R の基底 B です。 B に対して正の根は、$\varepsilon_i$ と $\varepsilon_i\pm \varepsilon_j(i < j)$ です。 対応するボレル部分代数 $\mathfrak{b}$ は、$\mathfrak{g}$の上三角行列の集合です。

$\mathfrak{b}$ で安定しているV のうち$\{0\}$ およびV と異なる唯一のベクトル部分空間は、最大フラグ対応するから基底 $(e_i)$ の元、つまり完全に等方性であることがすぐに検証されます。 部分空間 $V_1, . . . ,V_l$、ここで、$V_i$ は $e_1, . . . , e_i$ によって生成され、その直交補数 $V_{-1}, . . . ,V_{-i}:$ とともに、$V_i$ の直交補数 $V_{-i}$ は $e_1, . . . , e_l, e_0, e_{-l}, . . . , e_{-i-1}$ によって生成され、完全に等方性ではありません。一方、$\mathfrak{g}$ の元が安定したベクトル部分空間を残す場合、その直交補数も安定したままになります。その結果、$\mathfrak{b}$は$\mathfrak{g}$の元の集合となり、フラグ$\{V_1, . . . ,V_l\}$の安定した元が残ります。

それぞれの元が完全に等方性である場合、その旗は等方性であると言われます。 フラグ $\{V_1, . . . ,V_l\}$ は最大等方性フラグです。 Since the group $\mathbf{O}(\Psi )$ operates transitively both on the Borel subalgebras of $\mathfrak{g}$ (cf. (VII)) and on the maximal isotropic flags (Algebra, Chap. IX, §4, no. 3, Th. 1), we see that, for any maximal isotropic flag $\delta$ in V, the set $\mathfrak{b}_{\delta}$ of elements of $\mathfrak{g}$ leaving stable the elements of $\delta$ is a Borel subalgebra of $\mathfrak{g}$ and that the map $\delta  \rightarrow \mathfrak{b}_{\delta}$ is a bijection from the set of maximal isotropic flags to the set of Borel subalgebras of $\mathfrak{g}$.

$\delta$ を等方性フラグとし、$\mathfrak{p}_{\delta}$ を $\mathfrak{g}$ の元の集合とし、$\delta$ の安定した元を残します。 $\delta \subset  \{V_1, . . . ,V_l\}$ の場合、$\mathfrak{p}_{\delta}$ は $\mathfrak{g}$ 含む $\mathfrak{b}$ の放物線部分代数であり、$\mathfrak{p}_{\delta}$ で安定している唯一の完全に等方的な部分空間 $\not=\{0\}$ は次の元であることを検証するのは簡単です。 $\delta$。これにより、$\mathfrak{g}$ 含む $\mathfrak{b}$ の $2^l$ 放物線部分代数が得られます。上のように、写像 $\delta  \rightarrow \mathfrak{p}_{\delta}$ は、V の等方性フラグの集合から $\mathfrak{g}$ の放物線部分代数の集合までの全単射であることがわかります。さらに、$\delta \supset \delta '$の場合に限り、$\mathfrak{p}_{\delta}\subset \mathfrak{p}_{\delta'}$。

(IV) 基本的な重み対応するから $\alpha_1, . . . , \alpha_l$ は、第 2 章による。 VI, §4, no. 5.VI,

$$
\varpi_i=\varepsilon_1+\cdots +\varepsilon_i(1\leq i\leq l-1)
$$

$$
\varpi_l=\frac{1}{2}(\varepsilon_1+\cdots +\varepsilon_l)
$$

$\sigma$ を、V における $\mathfrak{g}$ の同一性表現とします。外装冪 $\bigwedge^r\sigma$ は $E =\bigwedge^rV$ に動​​作します。 $h\in \mathfrak{h}$の場合、

$\sigma (h).e_i=\varepsilon_i(h)e_i$ 対 $1\leq i\leq l$

$$
\sigma (h).e_0= 0
$$

$1\leq i\leq l$の場合は$\sigma (h).e_{-i}=-\varepsilon_i(h)e_{-i}$。

したがって、$1\leq r\leq l,\varepsilon_1+\cdots +\varepsilon_r$は$\bigwedge^r\sigma$の最高重量、重みの元、$\varepsilon_1+\cdots +\varepsilon_r$は$e_1\wedge  \cdots  \wedge$$e_r$に比例することになります。 $1\leq r\leq l-1$ の場合、表現 $\bigwedge^r\sigma$ は最高重量 $\varpi_r$ の $\mathfrak{g}$ の基本的な表現であることを示します。このためには、$\bigwedge^r\sigma$ が $0\leq r\leq 2l+ 1$ に対して既約であることを示すだけで十分です。ただし、$\bigwedge^rV\times \bigwedge^{2l+1-r}V$ では双線形形式 $\Phi$ は次のように定義されます。

$$
x\wedge y=\Phi (x, y)e_1\wedge  \cdots  \wedge e_l\wedge e_0\wedge e_{-l}\wedge  \cdots  \wedge e_{-1}
$$

は $\mathfrak{g}$ の下で不変であり、$\bigwedge^rV$ と $\bigwedge^{2l+1-r}V$ を双対関係に置きます。 したがって、表現 $\bigwedge^{2l+1-r}\sigma$ は $\bigwedge^r\sigma$ の双対であり、$0\leq r\leq l$ に対する $\bigwedge^r\sigma$ の既約性、または $\bigwedge^rV$ 含むの最小の部分空間 $T_r$ を証明するのに十分です。 $e_1\wedge  \cdots  \wedge e_r$と$\mathfrak{g}$の下で安定するのは$\bigwedge^rV$の全体です。 これは、$r= 0$ と $r= 1$ (cf. 公式 (2)) の明らかです。 $r= 2$ (したがって $l\geq 2$)、表現 $\bigwedge^2\sigma$ と $\mathfrak{g}$ の随伴物表現 (既約) は、同じ次元 $l(2l+ 1)$ と同じ最高重量 $\varepsilon_1+\varepsilon_2$ を持ちます。 VI, §4, no. 5.IV)。 $\bigwedge^2\sigma$ は随伴の表現と等価であり、したがって既約であると結論する考えます。 これは、$l= 1$ と $l= 2$ の主張を証明します。

ここで、$l$ について帰納法までに議論し、$l\geq r\geq 3$ と仮定します。まず最初に、W が奇数次元の V の非等方性部分空間であり、直交補数 $W'$ を持つ場合、W に対する $\Psi$ の制限 $\Psi_W$ は非縮退であり、$\mathfrak{o}(\Psi_W)$ は次のように識別できることに注意します。 $\mathfrak{g}$ の部分代数元のからなるは $W'$ に消えます。薄暗い $W<$ 薄暗い V で、$\Psi_W$ が最大添字である場合、帰納法の仮定は、$T_r$ 含むが形 $w'\wedge w$ の非ゼロ元であることを意味します。 $w'\in \bigwedge^{r-k}W'$ と $w\in \bigwedge^kW (0\leq k\leq r)$、次に $T_r$ 含む $w'\wedge \bigwedge^kW:$ 確かに、すべての $a\in \mathfrak{o}(\Psi_W)$ に対して $a.(w'\wedge w) =w'\wedge a.w$ があります。 $p\in 0, r$ の帰納法までに $T_r$ 含む元が示されます。

$$
x=e_{i_1}\wedge  \cdots  \wedge e_{i_{r-p}}\wedge e_{j_1}\wedge  \cdots  \wedge e_{j_p}
$$

$1\leq i_1<\cdots < i_{r-p}\leq l$ と $-l\leq j_1<\cdots < j_p\leq 0$ の場合。 $p= 0$ の場合、これは、$\bigwedge^rF$ (no. 1) における $\mathfrak{g}\mathfrak{l}(F)$ の演算の既約性から続きます。

$\mathfrak{g}$ 含む元は $F = V_l=\sum_{i=1}^lke_i$ を固定したままにし、その上に任意の自己準同型 (cf. 公式 (2)) を誘導します。 $p= 1$ の場合、$q\in (1, l)$ は $q\not=-j_1$ となり、$q=i_{\lambda}$ とともに $\lambda \in 1, r-p$ が存在するようになります。 $p\geq 2$ の場合、$q\in 1, l$ を $-q\in  \{j_1, . . . , j_p\}$ となるようにします。必要に応じて $e_i$ を並べ替えると、$q= 1$ と仮定できます。ここで、W に対して $W'=ke_1+ke_{-1}$ の直交補数をとります。 $p= 1$ の場合、$x\in e_1\wedge \bigwedge^{r-1}W$ になります。 $T_r$ 含む $e_1\wedge  \cdots  \wedge e_r$ から、$T_r$ 含む $x$ であることがわかります。 $p\geq 2$ の場合は、$x\in e_{-1}\wedge \bigwedge^{r-1}W$ または $x\in e_1\wedge e_{-1}\wedge \bigwedge^{r-2}W$ のいずれか。 $T_r$ 含む $e_{-1}\wedge e_2\wedge  \cdots  \wedge e_{r-1}$ と $e_{-1}\wedge e_1\wedge e_2\wedge  \cdots  \wedge e_{r-2}$ から帰納法の仮定までなので、$T_r$ 含む $x$ となり、証明が完成します。

$\bigwedge^r\sigma$ の既約性の他の証明については、Exerc を参照してください。 6.

ここで、決定する表現を最高重量 $\varpi_l$ で説明します。

#### 補題 1 {#lie-viii-s13-lem-1 .statement tag=018T}

V を有限次元ベクトル空間、Q を V$,\Psi$ 上の非縮退二次形式、Q に関連付けられた対称双一次形式、C(Q) を Q$,f_0$ に対するV のクリフォード代数、正準写像の合成とします。

$$
\mathfrak{o}(\Psi )\longrightarrow \mathfrak{g}\mathfrak{l}(V)\longrightarrow V\otimes V^*\longrightarrow V\otimes V\longrightarrow C^+(Q)
$$

（1番目は標準単射、3番目は$V^*$からV、対応するから$\Psi$までの標準同型によって定義され、4番目はC(Q)、cf.代数、第4章の乗法によって定義されます。 IX, § 9, no. 1）。 $f=\frac{1}{2}f_0$を入れます。

(i) $(e_r),(e'_r)$ が $\Psi (e_r, e'_s) =\delta_{rs}$ となるような V の基底である場合、すべての $a\in \mathfrak{o}(\Psi )$ に対して $f_0(a) =$ $\sum_r(ae_r)e'_r$ が得られます。

(ii) $a, b\in \mathfrak{o}(\Psi )$ の場合、$\sum_r(ae_r)(be'_r) =-\sum_r(abe_r)e'_r$ があります。

(iii) $a\in \mathfrak{o}(\Psi )$ と $v\in V$ の場合、$[f(a), v] =av$ が得られます。

(iv) $a, b\in \mathfrak{o}(\Psi )$ の場合、$[f(a), f(b)] =f([a, b])$ になります。

(v) $f(\mathfrak{o}(\Psi ))$ 生成する代数 $C^+(Q)$。

(vi) N を左の $C^+(Q)$ モジュールおよび $C^+(Q)$ から End$_k(N)$ までの $\rho$ 対応する準同型とする。このとき、$\rho \circ f$ は N 上の $\mathfrak{o}(\Psi )$ の表現です。N が単純であれば、$\rho \circ f$ は既約です。

主張 (i) はクリアです。 $a, b\in \mathfrak{o}(\Psi )$ の場合、($\Psi (x, y) =\langle x, y\rangle$ を入れる)$:$ となります。

$$
\sum_r(ae_r)(be'_r) =\sum_{r,s,t}\langle ae_r, e'_s\rangle \langle be'_r, e_t\rangle e_se'_t=\sum_{r,s,t}\langle e_r, ae'_s\rangle \langle e'_r, be_t\rangle e_se'_t
$$

$$
=\sum_{s,t}\langle ae'_s, be_t\rangle e_se'_t=-\sum_{s,t}\langle e'_s, abe_t\rangle e_se'_t=-\sum_t(abe_t)e'_t
$$

これは(ii)を証明します。次に、すべての $v\in V$ について、(i) によって、

1 $''$

$$
[f(a), v] =\sum((ae_r)e_rv-v(ae_r)e_r)
$$

2

= $1\sum^r((ae_r)e'_rv+ (ae_r)ve'_r-(ae_r)ve'_r-v(ae_r)e'_r)$

2

$r$

1 $''$

= $\sum((ae_r)\langle e_r, v\rangle  - \langle ae_r, v\rangle e_r)$

2

= $1a(\sum^r\langle e'_r, v\rangle e_r)+1\sum\langle e_r, av\rangle e'_r=1av+1av=av$、

2 $_r$ 2 $_r$ 2 2

これは(iii)を証明します。それから

$[f(a), f(b)] =[f(a),\frac{1}{2}\sum(be_r)e'_r]$ by (i)

$r$

$=\frac{1}{2}\sum([f(a), be_r]e'_r+ (be_r)[f(a), e'_r])$ $=\frac{1}{2}\sum^r((abe_r)e'_r+ (be_r)(ae'_r))$ by (iii)

$r$

$=\frac{1}{2}\sum((abe_r)e'_r-(bae_r)e'_r)$ by (ii)

$r$

$=f([a, b])$ by (i)

これは (iv) を証明します。 (v) を証明するには、スカラーを拡張することで、$k$ が代数的に閉じていると仮定できます。 選ぶ次に基底 V の $(e_r)$ は $\Psi (e_r, e_s) =\delta_{rs}$ となるため、$e'_r=e_r$ になります。 $i\not=j$ の場合、$E_{ij}-E_{ji}\in \mathfrak{o}(\Psi )$、

$$
f(E_{ij}-E_{ji}) =\frac{1}{2}(e_ie_j-e_je_i) =e_ie_j
$$

でも、$e_ie_j$ 生成する $C^+(Q)$。

主張 (vi) は (iv) と (v) から続きます。 Q.E.D.

この数の冒頭で使用された記法を思い出してください。 $\widetilde{V} = F + F'$ を置き、$\widetilde{Q}$ (または $\widetilde{\Psi}$) を Q (それぞれ $\Psi$ ) から $\widetilde{V}$ の制限とします。この場合、$\widetilde{Q}$ は、次元 $2l$ の空間 $\widetilde{V}$ 上の最大値添字 $l$ の非縮退二次方程式形であり、クリフォード代数 $C( \widetilde{Q})$ は中心です単純代数/次元 $2^{2l}($代数、章。 IX, §9, no. 4、木曜日。 2)。 N を、$e_{-1}, . . . , e_{-l}$ によって生成された最大等方性部分空間 $F'$ の外部代数とします。 同一視する F は、$\Psi$ による$F'$ の二重であり、$x\in F'$ (それぞれ $y\in F$) は、$\lambda (x)$ (それぞれ $\lambda (y)$) によって左外側を表し、積と $x$ (それぞれ左内側) を表します。 積と $y$) N で; $a_1, . . . , a_k\in F'$ の場合、

$$
\lambda (x).(a_1\wedge  \cdots  \wedge a_k) =x\wedge a_1\wedge  \cdots  \wedge a_k
$$

$$
\lambda (y).(a_1\wedge  \cdots  \wedge a_k) =\sum_{i=1}^k(-1)^{i-1}\Psi (a_i, y)a_1\wedge  \cdots  \wedge a_{i-1}\wedge a_{i+1}\wedge  \cdots  \wedge a_k
$$

$\lambda (x)^2=\lambda (y)^2= 0$ であることは簡単に検証できます。

$$
\lambda (x)\lambda (y) +\lambda (y)\lambda (x) =\Psi (x, y).1
$$

(代数、第 IX, §9, no. 1) から、$C( \widetilde{Q})$ から End(N) まで写像 $\lambda : F\cup F'\rightarrow$ End(N) を延長する一意な準同型 (再び $\lambda$ で示される) が存在することがわかります。 $N = 2^l$ が暗く、$C( \widetilde{Q})$ が単純加群、次元 $2^l($代数の固有の類を持っているため、第 3 章。 IX, §9, no. 4、木曜日。 2)、$\lambda$ によって定義される N 上の $C( \widetilde{Q})$ の表現は既約であり、$C( \widetilde{Q}) ($loc のスピノル表現です。引用）。

ここで、$\widetilde{V}$ から $C^+(Q)$ までの写像 $\mu:v \rightarrow e_0v$ を考えてみましょう。 $v\in \widetilde{V}$ については、

$$
(e_0v)^2=-e^2_0v^2=-Q(e_0)Q(v) = Q(v) = \widetilde{Q}(v)
$$

$\mu$ 拡大するは準同型に固有で、$C( \widetilde{Q})$ から $C^+(Q)$ までは再び$\mu$ で示されます。 $C( \widetilde{Q})$ はシンプルなので、

薄暗い$C^+(Q) =$ 薄暗い$C( \widetilde{Q}) = 2^{2l}$、

$\mu$ が同型であることがわかります。 従って、N 上の単純な $C^+$(Q) 加群構造 $\lambda \circ \mu^{-1}$ 定義するおよび $\rho =\lambda \circ \mu^{-1}\circ f$ は、N 上の $\mathfrak{g}$ の既約表現になります (補題 1 (vi))。

一方、補題 1 (i) を考慮すると、次のようになります。

$$
f(H_i) =\frac{1}{2}(e_ie_{-i}-e_{-i}e_i)
$$

$e_ie_{-i}=-e^2_0e_ie_{-i}=e_0e_ie_0e_{-i}$ と $e_ie_{-i}+e_{-i}e_i= 1$ から、

$_{-1}$ 1 1

$$
\mu\circ f(H_i) =-e_{-i}e_i=-+e_ie_{-i}
$$

2 2 $1\leq i_1<\cdots < i_k\leq l:$ については、次のように推測します。

$\rho (H)(e\wedge  \cdots  \wedge e) =\{-\frac{1}{2}e_{-i_1}\wedge  \cdots  \wedge e_{-i_k}$ $i\in  \{i_1, . . . , i_k\}$ の場合

$^{i-i_1}-_{i_k}\frac{1}{2}e_{-i_1}\wedge  \cdots  \wedge e_{-i_k}$ $i \notin  \{i_1, . . . i_k\}$ の場合

そして$h\in \mathfrak{h}$のために

$$
\rho (h)(e_{-i_1}\wedge  \cdots  \wedge e_{-i_k}) \tag{5}
$$

$$
= (\frac{1}{2}(\varepsilon_1+\cdots +\varepsilon_l)-(\varepsilon_{i_1}+\cdots +\varepsilon_{i_k}))(h)(e_{-i_1}\wedge  \cdots  \wedge e_{-i_k})
$$

これは、$\rho$の最高重量が$\varpi_l$であることを示しています。 $\rho$ を $\mathfrak{g}$ のスピノル表現と呼びます。 重みはすべて単純であることに注意してください (さらに、$\varpi_l$ はミニスキュール重みです)。

(V) $w_0=-1$ があるので、$\mathfrak{g}$ のすべての有限次元単純表現は直交またはシンプレクティックです。章著。 $(\alpha_1, . . . , \alpha_l)$に対する$\varpi_r$の座標のVI, §4, no. 5.VI、和は$1\leq r\leq l-1:$に対して積分であるため、表現$\bigwedge^r\sigma$は直交します。さらに、$\Psi$から$\bigwedge^rV$の拡大$\Psi_{(r)}$は不変のままになります。

スピノル表現の場合、$(\alpha_1, . . . , \alpha_l)$に対する$\varpi_l$の座標の和は$\frac{1}{2}(1 +\cdots +l) =\frac{l(l+1)}{4}($locです。引用）。したがって、$l\equiv 0$ または $-1$ (mod. 4) については直交し、$l\equiv 1$ または 2 (mod. 4) についてはシンプレクティックです。実際、次のように定義された $N =\bigwedge F'$ 上の双線形形式 $\Phi$ を考えてみましょう: $x\in \bigwedge^pF'$ と $y\in \bigwedge^qF'$ の場合、$p+q\not=l$ の場合は $\Phi (x, y) = 0$ を置き、

$$
x\wedge y= (-1)^{^{p(p+1)}_2}\Phi (x, y)e_{-1}\wedge  \cdots  \wedge e_{-r}
$$

$p+q=l$の場合。 $\Phi$ が非縮退であり、$l\equiv 0,-1$ (mod. 4) に対して直交し、$l\equiv 1,2$ (mod. 4) に対して交代的が直交していることは簡単に検証されます。一方、補題 1(i)を考慮すると、

$$
f(X_{\varepsilon_i}) =e_0e_i,f(X_{-\varepsilon_i}) =-e_0e_{-i}
$$

$1\leq i\leq l$ と

$$
f(X_{\varepsilon_i-\varepsilon_j}) =\frac{1}{2}(e_ie_{-j}-e_{-j}e_i) =e_ie_{-j}=e_0e_ie_0e_{-j}
$$

$1\leq i < j\leq l$ の場合、および同様に

$$
f(X_{\varepsilon_j-\varepsilon_i}) =-e_0e_je_0e_{-i}, f(X_{\varepsilon_i+\varepsilon_j}) =e_0e_ie_0e_j, f(X_{-\varepsilon_i-\varepsilon_j}) =e_0e_{-i}e_0e_{-j}
$$

したがって

$$
\mu^{-1}\circ f(X_{\varepsilon_i}) =e_i,\mu^{-1}f(X_{-\varepsilon_i}) =-e_{-i}
$$

そして

$1\leq i, j\leq l, i\not=j$ と $c\in  \{1,-1\}$ の場合は $\mu^{-1}\circ f(X_{\pm\varepsilon_i\pm\varepsilon_j}) =ce_{\pm i}e_{\pm j}$。 $\Phi$ が実際に $\mathfrak{g}$ 不変であることを簡単に検証できます (cf. 演習 18)。

(VI) $x\in \mathfrak{g}$ の場合、$\sigma (x)$ の特性多項式は形となります。

$$
T^{2l+1}+f_1(x)T^{2l}+f_2(x)T^{2l-1}+\cdots +f_{2l+1}(x)
$$

ここで、$f_1, . . . , f_{2l+1}$ は $\mathfrak{g}$ に対して不変の多項式関数です。

$x=\xi_1H_1+\cdots +\xi_lH_l\in \mathfrak{h}$ の場合、$f_i(x)$ は符号まで、$\xi_1, . . . , \xi_l,-\xi_1, . . . ,-\xi_l$ の基本対称写像です。これらの対称写像は奇数次数では零であり、

$$
T^{2l+1}+f_2(x)T^{2l-1}+f_4(x)T^{2l-3}+\cdots +f_{2l}(x)T = T(T^2-\xi_1^2). . .(T^2-\xi^2_l)
$$

so that $f_2, . . . , f_{2l}$ are, up to sign, the elementary symmetric functions of $\xi_1^2, . . . , \xi_l^2$, which are algebraically independent generators of $\mathbf{S}(\mathfrak{h}^*)^W$ (Chap. VI, §4, no. 5.IX). §8, no. 3 を考慮して、Th. 1 (i) では、$f_1=f_3=f_5=\cdots = 0$ と $(f_2, f_4, . . . , f_{2l})$ が $\mathfrak{g}$ 上の不変式多項式関数の代数的に自由な族生成する代数であることがわかります。

(VII) Dynkin グラフの唯一の自己同型が恒等式であるため、Aut($\mathfrak{g}$) $=$ Aut$_0(\mathfrak{g})$ が得られます。

$\Sigma$ を $\Psi$ に対する V の類似度の群とします。すべての $g\in \Sigma$ について、$\varphi (g)$ を $\mathfrak{g}$ の自己同型 $x \rightarrow gxg^{-1}$ とします。すると、$\varphi$は$\Sigma$からAut($\mathfrak{g}$)まで準同型になります。それが全射的であることを示します。 $\alpha \in$ Aut($\mathfrak{g}$) $=$ Aut$_0(\mathfrak{g})$ とします。 §7, no. 1 の提案 2 により、すべての $x\in \mathfrak{g}$ に対して $\alpha (x) =sxs^{-1}$ となるような $s\in \mathbf{G}\mathbf{L}(V)$ が存在します。次に、$s$ 変換 $\Psi$ をV 上の双線形形式 $\Psi '$ に変換します。これは、$\mathfrak{g}$ では不変であり、したがって$\Psi ($§7, no. 5 に比例します、提案 12)。これは、$s\in \Sigma$ であることを証明します。

$\mathfrak{g}$ の恒等式表現は既約なので、その交換子環簡約するはスカラー (§6, no. 1、提案 1) なので、$\varphi$ の核は $k^*$ です。したがって、群 Aut($\mathfrak{g}$) $=$ Aut$_0(\mathfrak{g})$ は $\Sigma /k^*$ と識別できます。ただし、代数章から続きます。 IX, §6, no. 5、その群 $\Sigma$ は、群 $k^*$ と $\mathbf{S}\mathbf{O}(\Psi )$ の積です。したがって、Aut($\mathfrak{g}$) $=$ Aut$_0(\mathfrak{g})$ は $\mathbf{S}\mathbf{O}(\Psi )$ と識別できます。

$\mathbf{O}^+_0(\Psi )$ を $\Psi ($代数の縮小直交群とします。 IX, §9, no. 5）。 $\mathbf{S}\mathbf{O}(\Psi )/\mathbf{O}^+_0(\Psi )$ は可換であるため (前述)、群 Aut$_e(\mathfrak{g})$ は $\mathbf{O}^+_0(\Psi ) ($§11, no. 2、提案 3) に含まれます。実際、それはそれに等しいです (例題 7)。

(VIII) $\mathfrak{h}^*$ 上の正規の双線形形式 $\Phi_R$ は次のように与えられます。

$\Phi_R(\xi_1\varepsilon_1+\cdots +\xi_l\varepsilon_l, \xi '\varepsilon_1+\cdots +\xi '\varepsilon_l) =$ 1 $(\xi_1\xi '+\cdots +\xi_l\xi ')$

$$
^1l\overline{4l- 2}^1l
$$

(第VI, §4, no. 5.V)。 $\Phi_R$ によって定義される $\mathfrak{h}$ から $\mathfrak{h}^*$ までの同型は、$H_i$ から $(4l-2).\varepsilon_i$ かかります。したがって、$\Phi_R$の逆数形、つまり殺人形の制限から$\mathfrak{h}$は、次のようになります。

$$
\Phi (\xi_1H_1+\cdots +\xi_lH_l, \xi '_1H_1+\cdots +\xi '_lH_l) = (4l-2)(\xi_1\xi '_1+\cdots +\xi_l\xi '_l)
$$

(IX) 公式 (3) で定義された $X_{\alpha}(\alpha \in R)$ を思い出してください。 $\alpha \in R$ が $[X_{\alpha}, X_{-\alpha}] =-H_{\alpha}$ であることを確認するのは簡単です。一方、M を行列 $I+E_{0,0}$ とします。 $M=S^tM^{-1}S$、写像から

$$
\theta :g \rightarrow  -M^{-1t}gM
$$

すべての $\alpha \in R$ に対して、$\mathfrak{g}$ と $\theta (X_{\alpha}) =X_{-\alpha}$ の自己同型です。従って、$(X_{\alpha})$ は $(\mathfrak{g},\mathfrak{h})$ のシュバレー 系になります。

$k=\mathbf{Q}$ と仮定します。 カルタン部分代数 $\mathfrak{h}$ には、許容されるラティスが 2 つあります。 $H_{\alpha}$ によって生成されたラティス $Q(R^{\vee})$ と、$H_i$ によって生成され、整数エントリを含む$\mathfrak{h}$ の対角行列で構成されるラティス $P(R^{\vee})$ です。従って、$\mathfrak{o}_S(2l+ 1,\mathbf{Z})$ ($\mathfrak{g}$ の行列の集合と整数のエントリ) は、$\mathfrak{g}$ の Chevalley 位数 $P(R^{\vee}) +\sum\mathbf{Z}.X_{\alpha}$ であることがわかります。 $(X_{\pm\varepsilon_i})^2= 2E_{\pm i,\mp i},(X_{\pm\varepsilon_i})^3= 0$ と $(X_{\pm\varepsilon_i\pm\varepsilon_j})^2= 0$ から、Witt 基底 $(e_i)_{-l\leq i\leq l}$ によって生成された格子 $\mathscr{V}$ は、V の $\mathfrak{o}_S(2l+ 1,\mathbf{Z})$ に対して許容される格子であることがわかります。 $\bigwedge^rV$の$\bigwedge^r\mathscr{V}$も同様です。

次に、$\mathfrak{g}$ の $N =\bigwedge F'$ のスピノル表現 $\rho$ を考えてみましょう。 重みは写像 $P(R^{\vee})$ から $\mathbf{Z}$ に該当しないため、$\mathfrak{o}_S(2l+ 1,\mathbf{Z})$ に許容される格子はありません。一方、N の標準基底 $(e_{-i_1}\wedge  \cdots  \wedge e_{-i_k})$ ($1\leq i_1<\cdots < i_k\leq l$ の場合) によって生成された格子 $\mathscr{N}$ は、Chevalley 位数 $\mathscr{G}= Q(R^{\vee}) +\sum_{\alpha\in R}\mathbf{Z}.X_{\alpha}$ にとって許容される格子です。確かに、$\mathscr{N}$ が安定しているのは明らかです。

外装積は$e_{-i}$、内装積は$e_i$（$1\leq i\leq l$用）です。 (V) の公式は、$\mathscr{N}$ が $\rho (\mathscr{G})$ の下で安定していることを示します。さらに、すべての $\alpha \in R$ に対して $\rho (X_{\alpha})^2= 0$ であるため、$\mathscr{N}$ が許容されることになります。

### 3. 代数 OF 型 C$_{\boldsymbol{l}}$ ($\boldsymbol{l}\geq$ 1)

(I) $\Psi$ を、有限次元 $2l\geq 2$ のベクトル空間 V 上の非縮退交代的双線形形式とします。 自己準同型の集合 V の $x$ で、すべての $v, v'\in V$ の $\Psi (xv, v') +\Psi (v, xv') = 0$ は $\mathfrak{s}\mathfrak{l}(V)$ の半単純リー 部分代数になります (第 I, §6, no. 7、提案 9)。これを $\mathfrak{s}\mathfrak{p}(\Psi )$ で表し、$\Psi$ に関連付けられたシンプレクティックリー代数と呼びます。

代数より、キャップ。 IX, §4, no. 2、V は、$\Psi$ に対して双対関係にある 2 つの最大完全等方性部分空間 F と $F'$ の直和として書くことができます。 $(e_i)_{1\leq i\leq l}$をFの基底、$(e_{-i})_{1\leq i\leq l}$を$F'$の双対基底とします。それから

$$
(e_1, . . . , e_l, e_{-l}, . . . , e_{-1})
$$

Vの基底です。それはVのウィット基底（またはシンプレクティック基底）であると言います。この基底に対する$\Psi$の行列は位数$2l$の平方行列です

$$
(0s)
$$

$J=-s$ 0

ここで、$s$ は位数 $l$ の平方行列であり、そのエントリはすべて零ですが、2 番目の対角線上の 1 に等しいエントリ、cf. no. 2.I です。

代数 $\mathfrak{g}=\mathfrak{s}\mathfrak{p}(\Psi )$ は、$a=-J^{-1t}aJ=J^taJ($代数のように、正方行列の代数 $\mathfrak{s}\mathfrak{p}(2l, k)$ 位数の $a$ $2l$ と識別できます。 IX, §1, no. 10、公式 (50))、つまり形

$$
(AB)
$$

$$
a=C-s^tAs
$$

ここで、$A, B, C$ は、$B=s^tBs$ と $C=$ $c^tCs$ のような、位数 $l$ の正方行列です。他の語、$B$、$C$ は 2 番目の対角線に関して対称です。従って、

薄暗い$\mathfrak{g}=l^2+ 2\frac{l(l + 1)}{2}=l(2l+ 1)$。

$\mathfrak{h}$を$\mathfrak{g}$の対角線行列の集合とします。これは$\mathfrak{g}$の可換部分代数で、$1\leq i\leq l$の場合は基底元$H_i=E_{i,i}-E_{-i,-i}$です。 $(\varepsilon_i)_{1\leq i\leq l}$を$(H_i)$の双対基底とします。 $1\leq i < j\leq l$には、次のように入力します

$X_{2\varepsilon_i}$ = $E_{i,-i}$

$X_{-2\varepsilon_i}$ = $-E_{-i,i}$

$X_{\varepsilon_i-\varepsilon_j}$ = $E_{i,j}-E_{-j,-i}$

$X_{-\varepsilon_i+\varepsilon_j}$ = $-E_{j,i}+E_{-i,-j}$ (6)

$X_{\varepsilon_i+\varepsilon_j}$ = $E_{i,-j}+E_{j,-i}$

$X_{-\varepsilon_i-\varepsilon_j}$ = $-E_{-i,j}-E_{-j,i}$。

これらの元形基底は、$\mathfrak{g}$ の $\mathfrak{h}$ の補数であり、$h\in \mathfrak{h}$ については、

$$
[h, X_{\alpha}] =\alpha (h)X_{\alpha} \tag{7}
$$

すべての $\alpha \in R$ に対して、R は $\pm 2\varepsilon_i$ と $\pm \varepsilon_i\pm \varepsilon_j(i < j)$ の集合です。従って、$\mathfrak{h}$ は $\mathfrak{g}$ の独自のノーマライザーと等しいため、$\mathfrak{g}$ のカルタン部分代数、$\mathfrak{h}$ は分裂、$(\mathfrak{g},\mathfrak{h})$ の根は R の元であることがわかります。 $(\mathfrak{g},\mathfrak{h})$ の根系 R は、$l\geq 2$ に対しては型 $C_l$ であり、$l= 1$ に対しては型 $A_1$ (型 $C_1$ の他の語) です。 VI, §4, no. 6.I は $l= 1$ の場合に拡張されます）。従って、$\mathfrak{g}$ は、型 $C_l$ の分割可能な単純なリー代数です。

$\mathfrak{g}$ のすべての分裂カルタン部分代数は、基本的な自己同型によって、つまりシンプレクティック群 $\mathbf{S}\mathbf{p}(\Psi )$ (cf. (VII)) の元によって $\mathfrak{h}$ に変換され、その結果、 集合 $\mathfrak{h}_{\beta}$ の元の $\mathfrak{g}$ の行列は、ウィット基底 $\beta$ の $\mathfrak{g}$ に対して対角線にあります。 $\mathfrak{h}_{\beta}$ で安定しているV のベクトル部分空間だけが、$\beta$ の部分集合によって生成されたものであることがすぐに検証されます。

$\mathfrak{s}\mathfrak{p}(2, k) =\mathfrak{s}\mathfrak{l}(2, k)$ があります。一方、代数 $\mathfrak{s}\mathfrak{p}(4, k)$ と $\mathfrak{o}_S(5, k)$ は同じ根系を持ち、したがって同型です (cf. 例題 3)。ここからは$l\geq 2$とします。

(II) 根系 $R^{\vee}$ は第 2 章によって決定されます。 VI, §4, no. 6.Iと6.V;私たちはそれを見つけます

$$
H_{2\varepsilon_i}=H_i, H_{\varepsilon_i-\varepsilon_j}=H_i-H_j, H_{\varepsilon_i+\varepsilon_j}=H_i+H_j
$$

(III) $\alpha_1=\varepsilon_1-\varepsilon_2, . . . , \alpha_{l-1}=\varepsilon_{l-1}-\varepsilon_l, \alpha_l= 2\varepsilon_l$を入れます。章著。 VI, §4, no. 6.II、$\{\alpha_1, . . . , \alpha_l\}$ は R の基底 B です。 B に対して正の根は、$2\varepsilon_i$ と $\varepsilon_i\pm \varepsilon_j(i < j)$ です。 対応するボレル部分代数 $\mathfrak{b}$ は、$\mathfrak{g}$の上三角行列の集合です。

$\delta$ を V の等方性フラグとします (つまり、その元はすべて $\Psi$ に対して完全に等方性部分空間です)、$\mathfrak{p}_{\delta}$ を元のからなるまたは $\mathfrak{g}$ の部分代数からなるとします。 $\delta$の元。 no. 2.III のように、写像 $\delta  \rightarrow \mathfrak{p}_{\delta}$ は等方性フラグ (最大等方性フラグ) の集合から放物線 (ボレル) の集合まで $\mathfrak{g}$ の部分代数までの全単射であることを示します。 $\delta \subset \delta '$ の場合に限り、$\mathfrak{p}_{\delta}\supset \mathfrak{p}_{\delta'}$ があります。

(IV) 基本的な重み対応するから $\alpha_1, . . . , \alpha_l$ は、第 2 章によるものです。 VI, §4, no. 6.VI、$\varpi_i=\varepsilon_1+\cdots +\varepsilon_i(1\leq i\leq l)$。

重み $\varpi_r$ の基本表現 $\sigma_r$ が $\bigwedge^r\sigma$ の部分表現としてどのように実現できるかを示します。ここで、$\sigma$ は V 上の $\mathfrak{g}$ の同一性表現であり、このために学習します。 代数 $\bigwedge V$ の外側に表現 $\bigwedge\sigma$ $\mathfrak{g}$ の分解 。

$(e^*_i)$ を $V^*$ と $(e_i)$ の基底とします。 交代的双線形形式 $\Psi$ は、元 $\Gamma^*\in \bigwedge^2V^*($代数と識別できます。 III, §7, no. 4、提案 7 および §11, no. 10)、それを検証するのは簡単です。

$$
\Gamma^*=-\sum_{i=1}^le^*_i\wedge e^*_{-i}
$$

Let $\Psi^*$ be the inverse form of $\Psi$ (Algebra, Chap. IX, §1, no. 7); it is immediate that

$$
\Psi^*(e^*_i, e^*_j) = 0
$$

$i\not=-j$ の場合は $\Psi^*(e^*_i, e^*_{-i}) =-1$ 、$1\leq i\leq l$ の場合。 同一視する $\Psi^*$ と元 $\Gamma \in \bigwedge^2V$ の場合、

$$
\Gamma =\sum_{i=1}^le_i\wedge e_{-i}
$$

左の外側積と $\Gamma$ で与えられる $\bigwedge V$ の $X_-$ 自己準同型と、左内側積と $-\Gamma^*:$ で与えられる $\bigwedge V$ の $X_+$ 自己準同型で表します。

$$
X_-u=(\sum_{i=1}^le_i\wedge e_{-i})\wedge u
$$

$$
X_+u=(\sum_{i=1}^le^*_i\wedge e^*_{-i})\wedge u
$$

計算する $X_+$ と $X_-$ に、次の方法で $\bigwedge V$ の基底を導入します。 $1, l$ の 3 つの互いに素部分集合によって形成される 3 つ組 $(A,B,C)$ に対して、

$$
e_{A,B,C}=e_{a_1}\wedge  \cdots  \wedge e_{a_m}\wedge e_{-b_1}\wedge  \cdots  \wedge e_{-b_n}\wedge e_{c_1}\wedge e_{-c_1}\wedge  \cdots  \wedge e_{c_p}\wedge e_{-c_p}
$$

ここで、$(a_1, . . . , a_m)$ (それぞれ $(b_1, . . . , b_n),(c_1, . . . , c_p)$) は、A (それぞれ $B,C$) の元を増加する位数に配置したものです。このようにして $\bigwedge V$ の基底を取得し、簡単な計算で次のことがわかります。

$$
X_-.e_{A,B,C}=\sum e_{A,B,C\cup \{j\}} \tag{8}
$$

$j\in 1,l ,j \notin A\cup B\cup C$

$$
X_+.e_{A,B,C}=-\sum_{j\in C}e_{A,B,C-\{j\}} \tag{9}
$$

$H$を$\bigwedge V$の自己準同型とし、$\bigwedge^rV (0\leq r\leq 2l)$の$(l-r)$までに簡約するから乗法とします。を検証するのは簡単です (cf. 演習 19)。

$$
[X_+, X_-] =-H
$$

$$
[H, X_+] = 2X_+
$$

$$
[H, X_-] =-2X_-
$$

他の語、ベクトル部分空間 $\mathfrak{s}$ は、$X_+, X_-$ と $H$ によって生成され、End($\bigwedge V$) の嘘部分代数であり、$\mathfrak{s}\mathfrak{l}(2, k)$ と同型であり、$\bigwedge^rV$ は元の重み$l-r$の部分空間。プリミティブ元の $\bigwedge^rV$ からなるの $E_r$ 部分空間、つまり $E_r= (\bigwedge^rV)\cap$ Ker$X_+$ で表します。 §1 から、$r < l$ では、$X_-$ から $\bigwedge^rV$ の制限は単射であり、$r\leq l$ では、$\bigwedge^rV$ は直和として分解されます。

$$
\bigwedge^rV = E_r\oplus X_-(E_{r-2})\oplus X_-^2(E_{r-4})\oplus  \cdots
$$

$$
= E_r\oplus X_-(\bigwedge^{r-2}V)
$$

これは、特に $E_r=(^{2l}_r)-(_{r-2}^{2l})$ が $0\leq r\leq l$ に対して暗いことを示しています。

一方、$\mathfrak{s}\mathfrak{p}(\Psi )$ のまさに定義は、$\Gamma^*$ が$\sigma$ の双対の 2 番目の外面冪によって消滅することを示しています。同様に、$\Gamma$は$\bigwedge^2\sigma$によって全滅します。 $X_+$ と $X_-$、従って $H$ も、$g\in \mathfrak{g}$ のために自己準同型 $\bigwedge\sigma (g)$ と通勤するとすぐに推測します。その結果、$0\leq r\leq l$ の部分空間 $E_r$ は $\bigwedge^r\sigma$ では安定します。 $\bigwedge^r\sigma$ から $E_r$ の制限が重み $\varpi_r(1\leq r\leq l)$ の基本的な表現 $\sigma_r$ であることを示します。

まず第一に、$\mathfrak{h}$ に対する $\bigwedge^r\sigma$ の重みは、

$$
\varepsilon_{i_1}+\cdots +\varepsilon_{i_k}-(\varepsilon_{j_1}+\cdots +\varepsilon_{j_{r-k}})
$$

ここで、$i_1, . . . , i_k$ (それぞれ $j_1, . . . , j_{r-k}$) は $1, l$ の元と異なります。従って、$\bigwedge^r\sigma$ の最高重量は確かに

$$
\varpi_r=\varepsilon_1+\cdots +\varepsilon_r
$$

重み $\overline{\varpi}_r$ のベクトルは、$e_1\wedge\cdots\wedge e_r=e_{\{1,\ldots,r\},\varnothing,\varnothing}$ に比例します。 公式 (9) は $e_1\wedge\cdots\wedge e_r\in E_r$ を示します。従って、$\bigwedge^r\sigma$から$E_r$の制限が既約であることを証明すれば十分です。

$s\in\mathbf{Sp}(\Psi)$ の場合、$s$ から $\bigwedge V$ の拡大 (それぞれ $\bigwedge V^*$) は $\Gamma$ (それぞれ $\Gamma^*$) を固定するため、$X_+$ と $X_-$ で通勤し、$E_r$ から離れることになります。安定しています。その結果、$e_1\wedge\cdots\wedge e_r$の$\mathbf{Sp}(\Psi)$による変換により、$E_r$ 含むベクトル部分空間 $F_r$ が生成されます。 Witt の定理は、これらが非ゼロ分解可能な $r$ ベクトルであり、$V$ の対応するベクトル部分空間が完全に等方性の部分空間、$r$ ベクトルであり、これを等方性と呼ぶことにします。

#### 補題 2 {#lie-viii-s13-lem-2 .statement tag=01K8}

$1\leq r\leq\ell$ について、$F_r$ を等方性ベクトル $r$ によって生成された $\bigwedge^r V$ の部分空間とします。それから

$$
\bigwedge^r V=F_r+X_-\left(\bigwedge^{r-2}V\right)
=F_r+\left(\sum_{i=1}^{\ell}e_i\wedge e_{-i}\right)\wedge\bigwedge^{r-2}V.
$$

まず最初に、補題 2 がどのように主張を暗示するかを示します。 $F_r\subset E_r$ と $E_r\cap X_-\left(\bigwedge^{r-2}V\right)=\{0\}$ なので、補題は $F_r=E_r$ を意味します。 一方、$s\in\mathbf{Sp}(\Psi)$; としましょう。 $\operatorname{End}(V)$ の自己同型 $a\mapsto sas^{-1}$ は $\mathfrak{g}$ を保存し、そこに $\operatorname{Aut}_0(\mathfrak{g})$ の要素を誘導します (cf. (§7, no. 1、提案 2)。従って、$\mathfrak{g}$ のすべての既約表現を等価表現 (§7, no. 1、提案 2) に変換します。 $e_1\wedge\cdots\wedge e_r$ は $\bigwedge^r\sigma$ の既約成分に属し、$E_r=F_r$ は $e_1\wedge\cdots\wedge e_r$ による $\mathbf{Sp}(\Psi)$ の変換によって生成されるため、$E_r$ 上の $\mathfrak{g}$ の表現は等型であるということになります。 しかし、最高重量 $\overline{\varpi}_r$ の重複度は $1$ なので、既約です。

補題を証明することはまだ残っています。 $r=1$ はクリアです。 帰納法で議論し、$r\geq 2$と仮定します。 帰納法の仮定までに、証明に減ります。

$$
F_{r-1}\wedge V\subset F_r+\Gamma\wedge\bigwedge^{r-2}V,
$$

または、$y$ が分解可能な $(r-1)$-ベクトルおよび $x\in V$ である場合、

$$
z=y\wedge x\in F_r+\Gamma\wedge\bigwedge^{r-2}V.
$$

$(f_i)_{1\leq\pm i\leq\ell}$ を $y=f_1\wedge\cdots\wedge f_{r-1}$ となるような $V$ のウィット基底とします。 $x=f_i$のときに証明を行えば十分です。 $i\notin[1-r,-1]$ の場合、$r$ ベクトル $f_1\wedge\cdots\wedge f_{r-1}\wedge f_i$ は等方性です。それ以外の場合は、必要に応じて $f_i$ に番号を付け直し、$i=1-r$ と仮定することができます。それから$\Gamma=\displaystyle\sum_{j=1}^{\ell}f_j\wedge f_{-j}$なので、

$$
f_{r-1}\wedge f_{1-r}
=
\frac{1}{\ell-r+2}
\left(
\Gamma-\sum_{i=1}^{r-2}f_i\wedge f_{-i}
+\sum_{j=r}^{\ell}(f_{r-1}\wedge f_{1-r}-f_j\wedge f_{-j})
\right),
$$

$$
z=
\frac{1}{\ell-r+2}\Gamma\wedge f_1\wedge\cdots\wedge f_{r-2}
+
\frac{1}{\ell-r+2}\sum_{j=r}^{\ell}
(f_1\wedge\cdots\wedge f_{r-2})\wedge
(f_{r-1}\wedge f_{1-r}-f_j\wedge f_{-j}).
$$

しかし

$$
f_{r-1}\wedge f_{1-r}-f_j\wedge f_{-j}= (f_{r-1}+f_j)\wedge (f_{1-r}-f_{-j})-f_j\wedge f_{1-r}+f_{r-1}\wedge f_{-j}
$$

そして、$r$-ベクトルが

$$
f_1\wedge  \cdots  \wedge f_{r-2}\wedge (f_{r-1}+f_j)\wedge (f_{1-r}-f_{-j})
$$

$f_1\wedge  \cdots  \wedge f_{r-2}\wedge f_j\wedge f_{1-r}$ と $f_1\wedge  \cdots  \wedge f_{r-1}\wedge f_{-j}$

$r\leq j\leq l$ では等方性です。その結果、$z\in F_r+\Gamma \wedge \bigwedge^{r-2}V$が完成し、証明が完成します。

(V) $w_0=-1$ があるので、$\mathfrak{g}$ のすべての有限次元単純表現は直交またはシンプレクティックです。章著。 $(\alpha_1, . . . , \alpha_l)$に対する$\varpi_r$の座標のVI, §4, no. 6.VI、和は

$$
r
$$

$$
1 + 2 +\cdots + (r-1) +r+r+\cdots +r+
$$

2

従って、$\sigma_r$ は$r$ 偶数に対して直交し、$r$ 奇数に対してシンプレクティックです。

$e_1\wedge  \cdots  \wedge e_r$ と $e_{-1}\wedge  \cdots  \wedge e_{-r}$ 属するから $E_r$ 以降

$$
\Psi_{(r)}(e_1\wedge  \cdots  \wedge e_r, e_{-1}\wedge  \cdots  \wedge e_{-r}) = 1
$$

$\Psi_{(r)}$ から $E_r$ の制限は非ゼロであることがわかります。これは、定数因子、双線形形式までです。 $r$ が偶数の場合は対称で、$r$ が奇数の場合は交代的で、$\sigma_r$ では不変です。

(VI) すべての $x\in \mathfrak{g}$ について、$\sigma (x)$ の固有多項式は形となります。

$$
T^{2l}+f_1(x)T^{2l-1}+\cdots +f_{2l}(x)
$$

ここで、$f_1, . . . , f_{2l}$ は $\mathfrak{g}$ 上で不変多項式関数です。

$x=\xi_1H_1+\cdots +\xi_lH_l\in \mathfrak{h}$ の場合、$f_i(x)$ は符号付きで、$\xi_1, . . . , \xi_l,-\xi_1, . . . ,-\xi_l$ の基本対称写像です。これらの対称写像は、奇数次数では零であり、

$$
T^{2l}+f_2(x)T^{2l-2}+\cdots +f_{2l}(x) = (T^2-\xi_1^2). . .(T^2-\xi^2_l)
$$

no. 2.VI のように、$f_1=f_3=f_5=\cdots = 0$ が続き、

$$
(f_2, f_4, . . . , f_{2l})
$$

は、$\mathfrak{g}$ 上の不変式多項式関数の代数的に自由な族生成する代数です。

(VII) Dynkin グラフの唯一の自己同型が恒等式であるため、Aut($\mathfrak{g}$) $=$ Aut$_0(\mathfrak{g})$ が得られます。

$\Sigma$ を、$\Psi ($代数に対するV の類似点の群とします。 IX, §6、no. 5の終わり）。 no. 2.VII のように、$\mathfrak{g}$ の自己同型は写像 $x \rightarrow sxs^{-1}$ であることが証明されます。ここで、$s\in \Sigma$ は、Aut($\mathfrak{g}$) $=$ Aut$_0(\mathfrak{g})$ と識別できます。 $\Sigma /k^*$。

すべての $s\in \Sigma$ について、$\mu(s)$ を $s$ の乗数とします。 $\Sigma$ から $k^*/k^{*2}$ までの写像 $s \rightarrow \mu(s)$ mod $k^{*2}$ は準同型で、その核含む $k^*.1$ なので、以下から準同型 $\lambda$ が得られます。 $\Sigma /k^*$から$k^*/k^{*2}$まで。 $\mathbf{S}\mathbf{p}(\Psi )\cap k^*=\{1,-1\}$ あります。 準同型の数列を検討してください

1 $\longrightarrow \mathbf{S}\mathbf{p}(\Psi )/\{1,-1\}\longrightarrow^{\iota}\Sigma /k^*\longrightarrow^{\lambda}k^*/k^{*2}\longrightarrow 1$。 (10) 写像 $\iota$ は単射であり、$\mathbf{S}\mathbf{p}(\Psi )$ の元の乗数が 1 であるため、Im($\iota$ )$\subset$ Ker$\lambda$ です。$s\in \Sigma$ の乗数が元であれば$k^{*2}$ のうち、$\nu s\in \mathbf{S}\mathbf{p}(\Psi )$ となるような $\nu \in k^*$ が存在します。従って、イム($\iota$ ) $=$ カー($\lambda$ )。要約すると、数列 (10) は正確です。私たちは$\Sigma /k^*$の部分群と同一視する$\mathbf{S}\mathbf{p}(\Psi )/\{1,-1\}$です。 $k^*/k^{*2}$ は可換なので、$\Sigma /k^*$ の $\mathbf{S}\mathbf{p}(\Psi )/\{1,-1\}$ 含む導来群。従って、Aut$_e(\mathfrak{g})$ は$\mathbf{S}\mathbf{p}(\Psi )/\{1,-1\}($§11, no. 2、提案 3) に含まれます。実際、それはそれに等しく、Aut($\mathfrak{g}$)$/$Aut$_e(\mathfrak{g})$ は$k^*/k^{*2}$ と同一視されます (例題 9)。

(VIII) $\mathfrak{h}^*$ 上の正規の双線形形式 $\Phi_R$ は次のように与えられます。

$$
\Phi_R(\xi_1\varepsilon_1+\cdots +\xi_l\varepsilon_l, \xi '_1\varepsilon_1+\cdots +\xi '_l\varepsilon_l) =\frac{1}{4(l + 1)}(\xi_1\xi '_1+\cdots +\xi_l\xi '_l)
$$

(第 VI, §4, no. 6.V)。 従って、$\Phi_R$ の逆数形、つまり、殺人形の制限から $\mathfrak{h}$ は、次のようになります。

$$
\Phi (\xi_1H_1+\cdots +\xi_lH_l, \xi '_1H_1+\cdots +\xi '_lH_l) = 4(l+ 1)(\xi_1\xi '_1+\cdots +\xi_l\xi '_l)
$$

(IX) 公式 $(6) (\alpha \in R)$ によって定義された $X_{\alpha}$ を思い出してください。 $[X_{\alpha}, X_{-\alpha}] =-H_{\alpha}$ が $\alpha \in R$ であることは簡単に検証されます。一方、写像 $\theta :a \rightarrow  -^ta$ は、$\alpha \in R$ 全ての$\mathfrak{g}$ と $\theta (X_{\alpha}) =X_{-\alpha}$ の自己同型です。従って、$(X_{\alpha})_{\alpha\in R}$は$(\mathfrak{g},\mathfrak{h})$のシュバレー系になります。

$k=\mathbf{Q}$ と仮定します。 The Cartan subalgebra $\mathfrak{h}$ has two permissible lattices $Q(R^{\vee}) =\sum_{i=1}^l\mathbf{Z}.H_i$ and $P(R^{\vee}) = Q(R^{\vee}) +\frac{1}{2}\mathbf{Z}.\sum_{i=1}^lH_i$ (Chap. VI, §4,

no. 5.VIII)。 $Q(R^{\vee})$ は所属から $\mathfrak{h}$ までの整数エントリを持つ行列の集合であることがわかります。従って、シュバレー 位数 $Q(R^{\vee}) +\sum_{\alpha\in R}\mathbf{Z}.X_{\alpha}$ は、整数のエントリを持つ $\mathfrak{g}$ の行列の集合 $\mathfrak{s}\mathfrak{p}(2l,\mathbf{Z})$ になります。

還元的なリー代数 $\mathfrak{s}\mathfrak{p}(\Psi ) +\mathbf{Q}.1$ を考えてみましょう。 整数のエントリを持つ元のうちの集合がシュヴァレー 位数であり、$\mathbf{Q}.1$ と平行な $\mathfrak{s}\mathfrak{p}(\Psi )$ 上の射影がシュヴァレー 位数 $P(R^{\vee}) +\sum\mathbf{Z}.X_{\alpha}$ であることが簡単にわかります。

最後に、$\alpha \in R$ 全員に対して $X_{\alpha}^2= 0$ です。 $e_i$ によって生成された V の格子 $\mathscr{V}$ は Chevalley 位数 $\mathfrak{s}\mathfrak{p}(2l,\mathbf{Z})$ に許容されるということになります。 $E_r$の格子$E_r\cap \bigwedge^r\mathscr{V}$も同様です。

最後に、$E_r$ には Chevalley 位数に許容されるラティスがあります。

$$
P(R^{\vee}) +\sum\mathbf{Z}.X_{\alpha}
$$

$r$ が偶数の場合のみ。そうすると、$E_r\cap \bigwedge^r\mathscr{V}$ はそのような格子になります。

### 4. 型 $\boldsymbol{D}_{\boldsymbol{l}}$ ($\boldsymbol{l}\geq$ 2) の代数

(I) V を偶数次元 $2l\geq 4$ のベクトル空間とし、$\Psi$ をV 上の最大添字 $l$ の非縮退対称双線形形式とします。 代数までに、第2章。 IX, §4, no. 2、V は、2 つの最大完全等方性部分空間 F と $F'$ の直和として書くことができます。 $(e_i)_{1\leq i\leq l}$ を F の基底および $F'$ の $(e_{-i})_{1\leq i\leq l}$ 双対基底とします ( $\Psi$ によって定義される F と $F'$ の間の双対性について)。すると、$e_1, . . . , e_l, e_{-l}, . . . , e_{-1}$ は V の基底です。それをVのウィット基底と呼ぶことにします。この基底に対する $\Psi$ の行列は、 位数 $2l$ の平方行列 S であり、そのエントリはすべて零ですが、2 番目の対角線上にあるものは 1 に等しいです。 代数 $\mathfrak{g}=\mathfrak{o}(\Psi )$ は、$g=-S^tgS$ のように、正方行列の $g$ 位数 $2l$ と代数 $\mathfrak{o}_S(2l, k)$ で識別できます。 次元 $l(2l-1)$ があります。簡単に計算すると、$\mathfrak{g}$ は形の行列の集合であることがわかります。

$$
(AB)
$$

$$
CD
$$

ここで、$A, B, C, D$ は位数 $l$ の正方行列であり、$B=-s^tBs, C=$ $-s^tCs$ と $D=-s^tAs(s$ は位数 $l$ の行列であり、そのエントリはすべて零ですが、2 番目の対角線上にあるものは次と等しいです。 1)。

$\mathfrak{h}$を$\mathfrak{g}$に対する対角線行列所属の集合とします。これは $\mathfrak{g}$ の可換部分代数で、元 $H_i=E_{i,i}-E_{-i,-i}$ によって$1\leq i\leq l$ が形成された基底です。 $(\varepsilon_i)$ を $\mathfrak{h}^*$ と $(H_i)$ の基底とします。 $1\leq i < j\leq l$ については、

$X_{\varepsilon_i-\varepsilon_j}$ = $E_{i,j}-E_{-j,-i}$

$X_{-\varepsilon_i+\varepsilon_j}$ = $-E_{j,i}+E_{-i,-j}$

$X_{\varepsilon_i+\varepsilon_j}$ = $E_{i,-j}-E_{j,-i}$ (11)

$X_{-\varepsilon_i-\varepsilon_j}$ = $-E_{-j,i}+E_{-i,j}$。

これらの元形基底は、$\mathfrak{g}$ の $\mathfrak{h}$ の補数です。 $h\in \mathfrak{h}$の場合、

$$
[h, X_{\alpha}] =\alpha (h)X_{\alpha}
$$

すべての $\alpha \in R$ に対して、R は $\pm \varepsilon_i\pm \varepsilon_j(i < j)$ の集合です。従って、$\mathfrak{h}$ は $\mathfrak{g}$ の分裂カルタン部分代数であり、$(\mathfrak{g},\mathfrak{h})$ の根は R の元です。従って、$(\mathfrak{g},\mathfrak{h})$ の根系 R は型 $D_l$ になります。 $l\geq 3$、型 $A_1\times A_1$ (他の語型 $D_2$) の$l= 2$ (VI, §4, no. 8.I は$l= 2$ のケースに拡張)。従って、$l\geq 3$ の場合、$\mathfrak{g}$ は型 $D_l$ の分割可能な単純なリー代数になります。

$\mathfrak{g}$ のすべての分裂カルタン部分代数は、$\mathfrak{g}$ の初等自己同型によって $\mathfrak{h}$ に変換され、従って $\mathbf{O}(\Psi )$ の元 (cf. (VII)) によって、 集合 $\mathfrak{h}_{\beta}$ の元の $\mathfrak{g}$ の行列は、ウィット基底 $\beta$ の V に対して対角線です。 $\mathfrak{h}_{\beta}$ の下の唯一の部分空間不変式は、$\beta$ の部分集合によって生成されたものであることをすぐに検証します。

代数 $\mathfrak{o}_S(4, k)$ と $\mathfrak{s}\mathfrak{l}(2, k)\times \mathfrak{s}\mathfrak{l}(2, k)$ は同じ根系を持っているため、同型です。同様に、$\mathfrak{o}_S(6, k)$ と $\mathfrak{s}\mathfrak{l}(4, k)$ は同型です (cf. も例題 3)。ここからは$l\geq 3$とします。 (II) チャプターにより決定する $R^{\vee}$ VI, §4, no. 8.V.私たちはそれを発見しました

$$
H_{\varepsilon_i-\varepsilon_j}=H_i-H_j,H_{\varepsilon_i+\varepsilon_j}=H_i+H_j
$$

(III) $\alpha_1=\varepsilon_1-\varepsilon_2, \alpha_2=\varepsilon_2-\varepsilon_3, . . . , \alpha_{l-1}=\varepsilon_{l-1}-\varepsilon_l, \alpha_l=\varepsilon_{l-1}+\varepsilon_l$を入れます。章著。 VI, §4, no. 8.II、$(\alpha_1, . . . , \alpha_l)$ は R の基底 B です。 B に対して正の根は $\varepsilon_i\pm \varepsilon_j(i < j)$ です。 対応するボレル部分代数 $\mathfrak{b}$ は、上三角行列所属から $\mathfrak{g}$ の集合です。

$\mathfrak{b}$ の下で自明でない唯一の不変式ベクトル部分空間は完全に等方性の部分空間 $V_1, . . . ,V_l,V'_l$ であることが容易に検証されます。ここで、$V_i$ は $e_1, . . . , e_i$ によって生成され、$V'_l$ は $e_1, . . . , e_{l-1}, e_{-l}$ によって生成されます。 $V_1, . . . ,V_{l-1}$ の直交補数 $V_{-1}, . . . ,V_{-l+1}$; $V_i$ の直交補数 $V_{-i}$ は $e_1, . . . , e_l, e_{-l}, . . . , e_{-(i+1)}$ によって生成されます。しかし、明らかの計算によると、元 $a\in \mathfrak{g}$ が $V_{l-1}$ を安定させた場合、その行列は形であることがわかります。

$$
AxB
$$

$(\lambda$ 0 $)$

0 0 $-\lambda y$

0 0 $D$

ここで、$A, B, D$ は位数 $l-1,x$ (それぞれ $y$) の正方行列であり、2 列と $l-1$ 行 (それぞれ 2 行と $l-1$ 列) を持つ行列です。 $\lambda \in k$。従って、$a$ は $V_l$ と $V'_l$ を安定させます。従って、$\mathfrak{b}$ は $a\in \mathfrak{g}$ の集合であり、等方性フラグ $(V_1, . . . ,V_{l-1})$ のすべての元は安定しています。前述の式と Witt の定理 (代数、Chap. IX, §4, no. 3、Th. 1) は、$V_l$ と $V'_l$ が唯一の最大完全等方性部分空間含む $V_{l-1}$ であることを暗示していることに注意してください。

等方性フラグが次元 $1, . . . , l-1$ の $l-1$ 完全に等方性部分空間で構成されている場合、そのフラグは準最大であると言います。次に、no. 2 のように、準最大等方性フラグ $\delta$ について、$a\in \mathfrak{g}$ の集合 $\mathfrak{b}_{\delta}$ が$\delta$ の元を安定に残すのは、$\mathfrak{g}$ のボレル部分代数であり、写像であることがわかります。 $\delta  \rightarrow \mathfrak{b}_{\delta}$ は、準最大等方性フラグの集合からボレル部分代数の集合までの全単射です。

次元 $l$ の部分空間と次元 $l-1$ の部分空間の両方が含むでない場合、等方性フラグは適切であると言います。 $\delta$ をそのような等方性フラグとし、$\mathfrak{p}_{\delta}$ を $a\in \mathfrak{g}$ の集合とし、安定した $\delta$ の元を残します。 $\delta \subset  \{V_1, . . . ,V_l,V'_l\}$ の場合、$\mathfrak{p}_{\delta}$ は $\mathfrak{g}$、含む $\mathfrak{b}$ の放物線部分代数であり、$\mathfrak{p}_{\delta}$ の下で安定している唯一の完全に等方的な部分空間 $\not=\{0\}$ は、元であることを検証するのは簡単です。 $\delta$。 $\{V_1, . . . ,V_l,V'_l\}$ と含む $V_{l-1}$ には $2^{l-2}$ の適切な等方性フラグが含まれているため (それぞれ $V_l$、それぞれ $V'_l$、それぞれ含むは $V_{l-1}$ も $V_l$ も$V'_l$)、これにより、$2^l$ 放物線部分代数含む $\mathfrak{b}$ が得られます。上記のとおり、写像 $\delta  \rightarrow \mathfrak{p}_{\delta}$ は、適切な等方性フラグの集合から $\mathfrak{g}$ の放物線部分代数の集合までの全単射になります。

(IV) 基本的な重み対応するから $\alpha_1, . . . , \alpha_l$ は、第 2 章による。 VI, §4, no. 8.VI、

$$
\varpi_i=\varepsilon_1+\varepsilon_2+\cdots +\varepsilon_i(1\leq i\leq l-2)
$$

$$
\varpi_{l-1}=\frac{1}{2}(\varepsilon_1+\varepsilon_2+. . .+\varepsilon_{l-2}+\varepsilon_{l-1}-\varepsilon_l)
$$

$$
\varpi_l=\frac{1}{2}(\varepsilon_1+\varepsilon_2+. . .+\varepsilon_{l-2}+\varepsilon_{l-1}+\varepsilon_l)
$$

$\sigma$ を V における $\mathfrak{g}$ の同一性表現とします。外装冪 $\bigwedge^r\sigma$は$E =\bigwedge^r(V)$で動作します。 $h\in \mathfrak{h}$ の場合、

$$
\sigma (h)e_i=\varepsilon_i(h)e_i,\sigma (h)e_{-i}=-\varepsilon_i(h)e_{-i}
$$

$1\leq i\leq l$の場合。 従って、$1\leq r\leq l,\varepsilon_1+\cdots +\varepsilon_r$ は $\bigwedge^r\sigma$ の最高の重みであり、重みの要素 $\varepsilon_1+\cdots +\varepsilon_r$ は $e_1\wedge  \cdots  \wedge e_r$ に比例することになります。

$1\leq r\leq l-2$ の場合、表現 $\bigwedge^r\sigma$ は重み $\varpi_r$ の基本的な表現であることを示します。

このためには、$\bigwedge^r\sigma$ が $1\leq r\leq l-1$ に対して既約であること (表現 $\bigwedge^l\sigma$ が既約ではないことに注意してください、cf. 例題 10)、または最小の部分空間 $T_r$ が既約であることを示すだけで十分です。 $\bigwedge^rV$ 含む $e_1\wedge  \cdots  \wedge e_r$ と $\mathfrak{g}$ の下で安定しているのは $\bigwedge^rV$ の全体です。これは$r= 1$の明らかです。 $r= 2$ については、no. 2 と同様に、$\bigwedge^2\sigma$ が $\mathfrak{g}$ の随伴物表現と等価であることがわかります。これは、$\mathfrak{g}$ が単純なので既約です。 証明は、no. 2と同様に、$l$の帰納法までに議論することで完成しますが、$l-1\geq r\geq 3$と仮定します。

ここで、最高の重み $\varpi_{l-1}$ と $\varpi_l$ の基本表現を決定します。 Q を二次方程式形 $x \rightarrow \frac{1}{2}\Psi (x, x)$ とします。 no. 2.IV で、$N =\bigwedge F'$ のクリフォード代数 C(Q) のスピノル表現 $\lambda$ を定義しました。 $p$ 偶数 (または奇数) に対する $\bigwedge^pF'$ の和によって与えられる N の部分空間 $N_+$ (または $N_-$) が、$\lambda$ から $C^+(Q)$ の制限の下で安定していることを検証します。 その結果、$N_+$ と $N_-$ の $C^+(Q)$ の表現 $\lambda_+$ と $\lambda_-$ は、それぞれ $C^+(Q) ($代数の準スピノール表現です。 IX, §9, no. 4);それらは既約であり、次元 $2^{l-1}$ であり、等価ではありません。 $\rho_+=\lambda_+\circ f$ と $\rho_-=\lambda_-\circ f$ を $\mathfrak{g}$ の対応する既約表現とします (no. 2, 補題 1 (vi))。 補題 1 (i) を考慮すると、次のようになります。

$$
f(H_i) =\frac{1}{2}(e_ie_{-i}-e_{-i}e_i) =e_ie_{-i}-\frac{1}{2}=\frac{1}{2}-e_{-i}e_i
$$

そして、no. 2.IV のように、$h\in \mathfrak{h}$ と $1\leq i_1<\cdots < i_k\leq l$ について、

$$
\lambda \circ f(h)(e_{-i_1}\wedge  \cdots  \wedge e_{-i_k})
$$

$$
= (\frac{1}{2}(\varepsilon_1+\cdots +\varepsilon_l)-(\varepsilon_{i_1}+\cdots +\varepsilon_{i_k}))(h)(e_{-i_1}\wedge  \cdots  \wedge e_{-i_k})
$$

従って、$\rho_+$ (それぞれ $\rho_-$) の最高重量は $\varpi_l$ (それぞれ $\varpi_{l-1}$) になります。

$\rho_+$ と $\rho_-$ は $\mathfrak{g}$ の準スピノール表現であると言います。 重みはすべてシンプルです。 $\rho =\lambda \circ f=\rho_+\oplus \rho_-$ は $\mathfrak{g}$ のスピノル表現であるとも言います。

(V) $1\leq r\leq l-2$ の場合、基本的な表現 $\bigwedge^r\sigma$ は直交です。$\Psi$ から $\bigwedge^rV$ までの不変拡大が残ります。

ここで、$\mathfrak{g}$ のスピノル表現 $\rho$ について考えてみましょう。 no. 2 のように、$1\leq i, j\leq l, i\not=j$ に対して、

$$
f(X_{\varepsilon_i-\varepsilon_j}) =\pm e_ie_{-j}
$$

$$
f(X_{\varepsilon_i+\varepsilon_j}) =\pm e_ie_j
$$

$$
f(X_{-\varepsilon_i-\varepsilon_j}) =\pm e_{-i}e_{-j}
$$

no. 2.V で導入された非縮退双線形形式 $\Phi$ は $\rho (\mathfrak{g})$ の下で不変であるということになります。 したがって、スピノル表現 $\rho$ は、$l\equiv 0,-1$ (mod. 4) については対称であり、$l\equiv 1,2$ (mod. 4) については交互である非縮退形式を不変のままにします。

$l$ が偶数の場合、$\Phi$ ～ $N_+$ と $N_-$ の制限は非縮退であり、半スピノル表現は $l\equiv 0$ (mod. 4) に対して直交し、$l\equiv 2$ (mod. 4) に対してシンプレクティックです。 Moreover, we remark that $w_0=-1$ (Chap. VI, §4, no. 8.XI).

一方、$l$が奇数の場合、$N_+$と$N_-$は$\Phi$に対して完全に等方性になります。 Moreover, $-w_0(\alpha_i) =\alpha_i$ for $1\leq i\leq l-2,-w_0(\alpha_l) =\alpha_{l-1}$ and $-w_0(\alpha_{l-1}) =\alpha_l$ (Chap. VI, §4, no. 8.XI), so $-w_0(\varpi_l) =\varpi_{l-1}$ and the semi-spinor representations are neither orthogonal nor symplectic; each of them is isomorphic to the dual of the other.

(VI) すべての $x\in \mathfrak{g}$ について、$\sigma (x)$ の特性多項式は形となります。

$$
T^{2l}+f_1(x)T^{2l-1}+\cdots +f_{2l}(x)
$$

no. 3 のように $f_1=f_3=f_5=\cdots = 0$ であることがわかります。章著。 VI, §4, no. 8.IXと§8, no. 3、Th。 1、$\mathfrak{g}$ 上の不変式多項式関数の $f_2, f_4, . . . , f_{2l-2},\widetilde{f}$ 生成する代数 $I(\mathfrak{g}^*)$ が代数的に独立であり、さらに $\widetilde{f}^2= (-1)^lf_{2l}$ となるような $\mathfrak{g}$ 上に多項式関数 $\widetilde{f}$ が存在します。

すべての $x\in \mathfrak{g}$ に対して、$^t(Sx) =^txS=-Sx$ があるため、$x$ の多項式関数である Pf($Sx$) を考えることができます。今：

$f_{2l}(x) =$ det($x$) $= (-1)^l$ det($Sx$) $= (-1)^l$(Pf($Sx$))$^2$。

したがって、$\widetilde{f}(x) =$ Pf($Sx$) が得られます。

(VII) Aut($\mathfrak{g}$)$/$Aut$_0(\mathfrak{g})$ は、$(\mathfrak{g},\mathfrak{h})$ のディンキングラフ D の自己同型の群 Aut(D) と識別できること (§5, no. 3、提案 5 の Cor. 1) を思い出してください。 $l\not= 4$ の場合、Aut(D) は位数の群 2 $\alpha_1, . . . , \alpha_l$ の置換のからなるで、$\alpha_1, . . . , \alpha_{l-2}$ は固定のままです。 $l= 4$ の場合、Aut(D) は $\alpha_2$ を固定したままにする $\alpha_1, . . . , \alpha_4$ の置換で構成されます。 $\mathfrak{S}_3$ (cf. 章 VI, §4, no. 8.XI) と同型です。すべての場合において、$\alpha_1$ を固定したままにする Aut(D) の部分群元のからなるは、位数 2 です。Aut($\mathfrak{g}$) の Aut$'(\mathfrak{g})$ 対応する部分群で表します。 $l\not= 4$の場合はAut$'(\mathfrak{g}) =$ Aut($\mathfrak{g}$)、$l= 4$の場合は(Aut($\mathfrak{g}$) $:$ Aut$'(\mathfrak{g})$) $= 3$があります。さらに、

(Aut$'(\mathfrak{g}) :$ Aut$_0(\mathfrak{g})$) $= 2$。

$\sigma \circ s$ が $\sigma$ と等しい場合に限り、 元 $s\in$ Aut($\mathfrak{g}$) 属するから Aut$'(\mathfrak{g})$ になります (これは、 $\varpi_1$ が $\sigma$ の最高重量であるという事実から生じます)。 no. 2.VII のように、Aut$'(\mathfrak{g})$ は $\Sigma /k^*$ と識別できると結論付けます。ここで、$\Sigma$ は、$\Psi$ に対するV の類似点のグループです。

$s\in \Sigma$ とし、$\lambda (s)$ を $s$ の乗数とします。 We have det($s$) $=\lambda (s)^l$ if $s$ is direct, and det($s$) $=-\lambda (s)^l$ if $s$ is inverse (Algebra, Chap. IX, §6, no. 5). $\Sigma$ の添字 2 の直接の類似点形部分群 $\Sigma_0$。 $\Sigma_0\supset k^*$ があります。 群 $\Sigma_0/k^*$ は、Aut$'(\mathfrak{g}) =\Sigma /k^*$ の部分群 Aut$_0(\mathfrak{g})$ に等しい。 実際、$k$ が代数的に閉じている場合、これを検証するだけで十分です。 その場合、Aut$_0(\mathfrak{g}) =$ Aut$_e(\mathfrak{g})$ はその導来群 (§11, no. 2、提案 3) に等しいため、$\Sigma_0/k^*$ に含まれ、それらは両方とも $\Sigma /k^*$ の添字 2 であるため、彼らは平等です。

一方、no. 3.VII のように、完全系列があります。

$$
1\longrightarrow \mathbf{S}\mathbf{O}(\Psi )/\{1,-1\} \longrightarrow \Sigma_0/k^*\longrightarrow k^*/k^{*2}\longrightarrow 1
$$

$\Sigma_0/k^*=$ Aut$_0(\mathfrak{g})$ の部分群と同一視する $\mathbf{S}\mathbf{O}(\Psi )/\{1,-1\}$。 $k^*/k^{*2}$ は可換なので、Aut$_e(\mathfrak{g})\subset \mathbf{S}\mathbf{O}(\Psi )/\{1,-1\}$ が得られます。実際、Aut$_e(\mathfrak{g})$ は、$\Psi ($代数の縮小直交群 $\mathbf{O}^+_0(\Psi )$ の$\mathbf{S}\mathbf{O}(\Psi )/\{1,-1\}$ における像に等しいことが示されます (例題 11)。 IX, §9, no. 5）。

(VIII) $\mathfrak{h}^*$ の正規の双線形形式 $\Phi_R$ は次のように与えられます。

$''$ 1 $''$

$$
\Phi_R(\xi_1\varepsilon_1+\cdots +\xi_l\varepsilon_l, \xi_1\varepsilon_1+\cdots +\xi_l\varepsilon_l) =(\xi_1\xi +\cdots +\xi_l\xi )
$$

$$
\overline{4(l- 1)}^1l
$$

(第VI, §4, no. 8.V)。従って、形から$\mathfrak{h}$までの殺害のうち制限は、

$$
\Phi (\xi_1H_1+\cdots +\xi_lH_l, \xi '_1H_1+\cdots +\xi '_lH_l) = 4(l-1)(\xi_1\xi '_1+\cdots +\xi_l\xi '_l)
$$

(IX) 公式 (11) で定義された $X_{\alpha}(\alpha \in R)$ を思い出してください。 $[X_{\alpha}, X_{-\alpha}] =-H_{\alpha}$ が $\alpha \in R$ であることを簡単に検証します。一方、写像 $\theta :a \rightarrow  -^ta$ は、$\mathfrak{g}$ の自己同型と、すべての $\alpha \in R$ の $\theta (X_{\alpha}) =X_{-\alpha}$ です。従って、$(X_{\alpha})_{\alpha\in R}$ は $(\mathfrak{g},\mathfrak{h})$ のシュバレー 系になります。

$k=\mathbf{Q}$ と仮定します。章著。 VI, §4, no. 8.VIII、部分代数 $\mathfrak{h}$ には、$l$ が奇数の場合に許容される格子が 3 つあり、$l$ が偶数の場合に許容される格子が 4 つあります。特に、$H_i$ によって生成される格子 $\mathscr{H}$ は許容されます。しかし、この格子は$\mathfrak{g}$の対角線行列の集合に整数のエントリがあります。従って、$\mathfrak{o}_S(2l,\mathbf{Z})$ は $\mathfrak{g}$ のシュバレー 位数 $\mathscr{H}+\sum\mathbf{Z}.X_{\alpha}$ です。すべての $\alpha \in R$ に対して $X_{\alpha}^2= 0$ であるため、ウィット基底 $(e_i)$ によって生成された V の格子 $\mathscr{V}$ は、$\mathfrak{o}_S(2l,\mathbf{Z})$ の V で許容される格子であることがわかります。 $\bigwedge^rV$の$\bigwedge^r\mathscr{V}$も同様です。

一方、$P(R^{\vee}) =\mathbf{Z}.\frac{1}{2}\sum_{i=1}^lH_i+\mathscr{H}$ を許容格子、$\mathscr{G}= P(R^{\vee}) +\sum\mathbf{Z}.X_{\alpha}$ を Chevalley 位数とすると、$r$ が偶数の場合にのみ、$\bigwedge^rV$ が許容格子を持つことがわかります。その場合、$\bigwedge^r\mathscr{V}$ は許容されます。

還元的なリー代数 $\mathfrak{o}(\Psi ) +\mathbf{Q}.1$ を考えてみましょう。格子 $\widetilde{\mathscr{G}}= (\mathfrak{o}(\Psi ) +\mathbf{Q}.1)\cap \mathfrak{g}\mathfrak{l}(2l,\mathbf{Z})$ が Chevalley 位数であることがすぐにわかります。 Chevalley 位数 $\mathscr{G}$ は、中心 $\mathbf{Q}.1$ と平行して $\widetilde{\mathscr{G}}$ の $\mathfrak{o}(\Psi )$ にある射影です。

最後に、no. 2 のように、$e_{-i_1}\wedge  \cdots  \wedge e_{-i_{2k}}$ (それぞれ $e_{-i_1}\wedge  \cdots  \wedge e_{-i_{2k+1}}$) によって生成された格子 $\mathscr{N}_+$ (それぞれ $\mathscr{N}_-$) が、シュバレー 位数 $Q(R^{\vee}) +\sum_{\alpha\in R}\mathbf{Z}.X_{\alpha}$ のセミスピノール表現に許容されることがわかります。一方、$\mathscr{N}_+$ と $\mathscr{N}_-$ には、$\mathfrak{o}_S(2l,\mathbf{Z})$ に許容される格子がありません。

表 1

対応する単純表現が直交している場合 (それぞれ シンプレクティック、またはそれぞれ直交でもシンプレクティックでもない) に、各基本重み数 1 (それぞれ $-1,0$) を関連付けます。この数の計算は、本質的に型 $A_l,B_l,C_l,D_l$ に対して §13 で与えられています。結果は、型 $E_6,E_7,E_8,F_4,G_2$ についても以下に示されています (§7、提案 12、および章 VI, §4、番号 9.VI、9.XI、10.VI、 10.XI、11.VI、11.XI、12.VI、12.XI、13.VI、13.XI）。

$$
A_l(l\geq 1)B_l(l\geq 2)
$$

$\{0r\not=\frac{l+1}{2}\varpi_r$ 1 $r\not=l$

$$
\varpi_r
$$

$$
(-1)^rr=\frac{l+1}{2}\varpi_l(-1)^{l(l+1)/2}
$$

$$
C_l(l\geq 2)D_l(l\geq 2)
$$

$\varpi_r(-1)^r\varpi_r$ 1 $r\not=l-1, l$

$l$が奇数の場合は$\{0$

$l$が偶数の場合は、$\varpi_l$と$\varpi_{l-1}(-1)^{l/2}$

$$
E_6E_7E_8F_4G_2
$$

$\varpi_1$ 0 $\varpi_1$ 1 $\varpi_1$ 1 $\varpi_1$ 1 $\varpi_1$ 1

$\varpi_2$ 1 $\varpi_2-1\varpi_2$ 1 $\varpi_2$ 1 $\varpi_2$ 1

$\varpi_3$ 0 $\varpi_3$ 1 $\varpi_3$ 1 $\varpi_3$ 1

$\varpi_4$ 1 $\varpi_4$ 1 $\varpi_4$ 1 $\varpi_4$ 1

$\varpi_5$ 0 $\varpi_5-1\varpi_5$ 1

$\varpi_6$ 0 $\varpi_6$ 1 $\varpi_6$ 1

$\varpi_7-1\varpi_7$ 1

$\varpi_8$ 1

表 2

Th によって計算された対応する単純な表現の各基本重み次元に関連付けます。 §9の2。

$$
A_l(l\geq 1)B_l(l\geq 2)
$$

$$
(l+ 1)(2l+ 1)
$$

$$
\varpi_r(1\leq r\leq l)\varpi_r(1\leq r\leq l-1)
$$

$$
rr
$$

$$
\varpi_l2^l
$$

$$
C_l(l\geq 2)D_l(l\geq 2)
$$

$$
(2l)(2l)(2l)
$$

$$
\varpi_r(1\leq r\leq l)-\varpi_r(1\leq r\leq l-2)
$$

$$
rr-2r
$$

$$
\varpi_{l-1}2^{l-1}
$$

$$
\varpi_l2^{l-1}
$$

$$
E_6E_7
$$

$$
\varpi_127 = 3^3\varpi_1133 = 7.19
$$

$$
\varpi_278 = 2.3.13\varpi_2912 = 2^4.3.19
$$

$$
\varpi_3351 = 3^3.13\varpi_38645 = 5.7.13.19
$$

$$
\varpi_42925 = 3^2.5^2.13\varpi_4365750 = 2.5^3.7.11.19
$$

$$
\varpi_5351 = 3^3.13\varpi_527664 = 2^4.7.13.19
$$

$$
\varpi_627 = 3^3\varpi_61539 = 3^4.19
$$

$$
\varpi_756 = 2^3.7
$$

$$
E_8F_4
$$

$$
\varpi_13875 = 5^3.31\varpi_152 = 2^2.13
$$

$$
\varpi_2147250 = 2.5^3.19.31\varpi_21274 = 2.7^2.13
$$

$$
\varpi_36696000 = 2^6.3^3.5^3.31\varpi_3273 = 3.7.13
$$

$$
\varpi_46899079264 = 2^5.3.7^2.11^2.17.23.31\varpi_426 = 2.13
$$

$$
\varpi_5146325270 = 2.3.5.7^2.13^2.19.31
$$

$$
\varpi_62450240 = 2^6.5.13.19.31
$$

$$
\varpi_730380 = 2^2.5.7^2.31G_2
$$

$\varpi_8248 = 2^3.31\varpi_1$ 7

$$
\varpi_214 = 2.7
$$

### 練習問題 {#lie-viii-s13-exercises}

[§ 13 に対して練習問題](exercises/s13/)を参照してください。
