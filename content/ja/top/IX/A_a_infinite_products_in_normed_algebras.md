---
book: top
book_title: General Topology
chapter: IX
chapter_title: Use of real numbers in general topology
section: 0
section_title: Infinite products in normed algebras
appendix: true
lang: ja
source: top-v-x
book_pages: 268-270
pdf_pages: 0217-0223, 0274-0276
extraction: ocr
subsections:
    - "no": 1
      title: MULTIPLIABLE SEQUENCES IN A NORMED ALGEBRA
      page: 0
      pdf_page: 217
    - "no": 2
      title: MULTIPLIABILITY CRITERIA
      page: 0
      pdf_page: 218
    - "no": 3
      title: INFINITE PRODUCTS
      page: 0
      pdf_page: 221
statements: 16
exercises: 8
content_sha256: 135fe5f3568c247de7059d004dee2e90eb85f6ab1365a93065c2bf5778fbbc12
translated_from: content/en/top/IX/A_a_infinite_products_in_normed_algebras.md
translation_method: google
source_content_sha256: 4891adafb991bbb34168be7fb8caef2435567acb2d9b3db3045a912f02678465
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: 0ab1a76c5cda13175b806266b198b47c33a3ccd2ce01145969932e3010672e14
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## 付録

# 標準代数で無限積

### 1. 正規化された代数に乗算可能な数列

$A$ を非離散値体 $K$ (章 IX, § 3, no. 7, 定義 9) に対する正規化代数とします。 元 $x \in A$ の $||x||$ ノルムで表し、このノルムが不等式 $||xy|| \leq ||x|| \cdot ||y||$ を満たすと仮定します。また、$A$ には単位元 $e$ があると仮定します。

$(x_n)_{n \in \mathbf{N}}$ を $A$ の点の無限数列とします。 $\mathbf{N}$ の各有限部分集合 $J$ は、$\mathbf{N}$、定義する数列 $(x_n)_{n \in J}$、点、$A$ の順序によって線形に並べられ、定義する積

$$
p_J = \prod_{n \in J} x_n
$$

このうち数列;この積は、$\mathbf{N}$ の数列 $(x_n)_{n \in \mathbf{N}}$、対応するから有限部分集合 $J$ の有限部分積と呼ばれます ($J = \varnothing$ に $\prod_{n \in \varnothing} x_n = e$ を置くことを思い出してください)。

#### 定義 1 {#top-ix-a0-def-1 .statement tag=0CA3}

*数列* $(x_n)_{n \in \mathbf{N}}$ *は、集合* $\mathfrak{F}(\mathbf{N})$ *の切断のフィルタに関して、写像* $J \to p_J$ *が極限である場合、正規化代数* $A$ で乗算可能であると言われています。 * $\mathbf{N}$ のうち有限部分集合、* 関係* $\subset$ によって注文されました。 *この極限は数列* $(x_n)_{n \in \mathbf{N}}$ の積と呼ばれ、* $\prod_{n \in \mathbf{N}} x_n$ * (または単に* $\prod_n x_n$) で表されます。 *$x_n$ *この積の因子と呼ばれます。*

定義 1 は以下と同等です: *数列* $(x_n)$ *乗算可能であり、その積は* $p$ *それぞれの場合* $\varepsilon > 0$ *存在する有限部分集合* $J_0$ *の* $\mathbf{N}$ *すべての場合有限部分集合* $J \supset J_0$ *中* $\mathbf{N}$、*あります* $||p_J - p|| \leq \varepsilon$。

#### 注意 1 {#top-ix-a0-n1-rem-1 .statement tag=0CA4}

When $A$ is 可換代数, 定義 1 is identical with that given in 章 III, § 5, no. 1, 注意 3;しかし、$A$ が可換でない場合、添字集合 $\mathbf{N}$ の位数構造は、本質的に定義 1 に関与します。 $\sigma$ が $\mathbf{N}$ の任意の置換である場合、 できない in general assert that 数列 $(x_{\sigma(n)})$ is multipliable if 数列 (x_n) is multipliable; and if both 数列 are multipliable, their 積 will in general be different.

#### 注意 2 {#top-ix-a0-n1-rem-2 .statement tag=0CA5}

定義 1 は、添字集合 I が \mathbf{Z} の部分集合である族 (x_n)_{n \in I} の場合にすぐに一般化できます (\mathbf{Z} の位数によって線形順序付けされます)。この場合、以下の結果 (cf. 練習問題 1 および 2) について拡大するは読者に任せます。

### 2. 乗算性の基準

これからは、標準化された代数 A が完了したと仮定します。

#### 定理 1 {#top-ix-a0-thm-1 .statement tag=0CA6}

(x_n)_{n \in \mathbf{N}} を完全ノルム代数 A の点の数列とします。
a) (x_n) が乗算可能で、その積が A の単位元である場合、各 $\varepsilon > 0$ に対して \mathbf{N} の有限部分集合 J_0 が存在し、J_0 を満たさない \mathbf{N} の有限部分集合 L ごとに $\|e - p_L\| \leq \varepsilon$ が存在します。
b) 逆に、数列 (x_n) がこの条件を満たす場合、乗算可能です。さらに、各 x_n が単位元である場合、$\prod_{n \in \mathbf{N}} x_n$ は単位元となります。

a) p を乗算可能な数列 (x_n) の積とし、A で p が単位元であると仮定します。次に (章 IX, § 3, no. 7, 命題 13) $\alpha > 0$ と $a > 0$ が存在し、すべての $y \in A$ に対して、
$$
\|y - p\| \leq \alpha,
$$
yは単位元と$\|y^{-1}\| \leq a$です。 仮定までに、$0 < \varepsilon < \alpha$ のようなすべての $\varepsilon$ に対して、\mathbf{N} の有限部分集合 H_0 が存在し、\mathbf{N} 含む H_0 のすべての有限部分集合 H に対して、$\|p_H - p\| \leq \varepsilon$ が得られます。 $J_0 = [0, m]$ を \mathbf{N} の区間とし、含む H_0 とします。 J_0 を満たさない \mathbf{N} の各有限部分集合 L について、整数所属 ～ L はすべて、H_0 までの所属よりも大きいです。従って、$H = H_0 \cup L$ の場合、$p_H = p_{H_0} p_L$ になります。さて、$\|p_{H_0} - p\| \leq \varepsilon \leq \alpha$ から、$p_{H_0}$ は単位元となり、
$$
\|e - p_{H_0}^{-1} p\| \leq \varepsilon \|p_{H_0}^{-1} p\| \leq a \varepsilon;
$$
$\|p_{H_0} p_L - p\| \leq \varepsilon$ 以来、私たちは推測します
$$
\|p_L - p_{H_0}^{-1} p\| \leq \varepsilon \|p_{H_0}^{-1}\| \leq a \varepsilon,
$$
そして最後に$\|e - p_L\| \leq 2a \varepsilon$。

b) それぞれの $\varepsilon > 0$ に対して \mathbf{N} の有限部分集合 J_0 が存在し、J_0 を満たさない \mathbf{N} のすべての有限部分集合 L に対して $\|e - p_L\| \leq \varepsilon$ があるとします。 $H_0 = [0, p]$ を \mathbf{N} の区間とし、含む J_0 とします。 \mathbf{N} のすべての有限部分集合 H は、含む H_0 を形 $H_0 \cup L$ に書き込むことができます。ここで、L の整数はすべて H_0 のものより大きくなります。従って、$p_H = p_{H_0} p_L$ があり、L は $J_0$、$\|p_H - p_{H_0}\| \leq \varepsilon \|p_{H_0}\|$ を満たさないため、結果として $\|p_H\| = (1 + \varepsilon)\|p_{H_0}\|$ となります。 $p_{H_0} = 0$ の場合、数列 $(x_n)$ は明らかに乗算可能であり、その積は 0 です。この些細なケースを除くと、区間 $H_1 = [0, q]$ 含む $H_0$ があり、$H_1$ を満たさない $\mathbf{N}$ のすべての有限部分集合 $L$ に対して、$\|e - p_L\| \leq \varepsilon (\|p_{H_0}\|)^{-1}$ が得られます。上記のように、各有限部分集合 $H \supset H_1$ について、

$$
\|p_H - p_{H_1}\| \leq (\|p_{H_0}\|)^{-1}\|p_{H_1}\|\varepsilon \leq \varepsilon (1 + \varepsilon).
$$

従って、コーシーの基準は、$J \to p_J$ が有向集合 $\mathfrak{F}(\mathbf{N})$ に関して $A$ に極限を持っていることを示します。

すべての $x_n$ が単位元である場合、すべての有限部分積 $p_J$ も同様です。従って、それぞれ有限部分集合 $H$ 含む $H_0$ について、

$$
\|e - p_{H_0}^{-1}p_H\| \leq \varepsilon,
$$

これは、$A$の単位元の乗法群$G$において、$\mathfrak{F}(\mathbf{N})$の切断フィルタの写像$J \to p_J$の下の像が、左の均一性に関してコーシーフィルタ基底であることを示しています。 $G$;しかし、$G$ は*完備* (章 IX, § 3, no. 7、命題 13) なので、写像 $J \to p_J$ 属するから $G$ の極限です。

#### 注意 {#top-ix-a0-n2-rem-1 .statement tag=0CA7}

$(x_n)$ が乗算可能で、その積が単位元ではない場合、定理 1 の条件は必ずしも満たされません。たとえば、すべての $x_n$ が同じ元 $x$ に等しい場合、ここで $\|x\| < 1$、数列 $(x_n)$ は乗算可能であり、その積は 0 であり、$\mathbf{N}$ の空ではない有限部分集合 $H$ ごとに、$\|p_H\| \leq \|x\| < 1 \leq \|e\|$ が得られます。

#### 系 1 {#top-ix-a0-thm-1-cor-1 .statement tag=0CA8}

*もし* $(x_n)$ *が乗算可能な数列で、その積が* $A$の単位元である場合、*その後* $\lim_{n \to \infty} x_n = e$になります。

#### 系 2 {#top-ix-a0-thm-1-cor-2 .statement tag=0CA9}

*もし* $(x_n)$ *が乗算可能な数列で、その積が* $A$の単位元である場合、*すべての部分列* $(x_{n_k})_{k \in \mathbf{N}}$ *of* $(x_n)$ *[$(n_k)$は真に増加する数列になります。 整数]* *乗算可能です*。

これは、定理 1 の基準からすぐに得られます。

#### 定理 2 {#top-ix-a0-thm-2 .statement tag=0CAA}

*$A$ *完全な標準代数* とします。 *もし* $(u_n)$ * が * $A$ の元の絶対収束系列である場合、 * 数列* $(e + u_n)$ * は $A$ で乗算可能です。 *そして、すべての元* $e + u_n$ *が単位元に* $A$ ある場合、 *$\prod_{n \in \mathbf{N}} (e + u_n)$ も同様です*。

定理 1 の基準を適用しましょう。 $\mathbf{N}$ のすべての有限部分集合 $L$ に対して、$p_L - e = \prod_{n \in L} (e + u_n) - e = \sum_M \left( \prod_{n \in M} u_n \right)$ が得られます。ここで、$M$ は、$L$ の空でないすべての部分集合の集合を通過します (誘導順序）。 $\prod_{n \in M} u_n \leq \prod_{n \in M} |u_n|$以降、書くかもしれません

$$
||p_1 - e|| = \sum_M (\prod_{n \in M} u_n) \cdot \prod_{i \in I} (1 + |u_i|) - 1.
$$

さて、一般的な項が$|u_n|$である系列は仮定で収束するので、数列$1 - |u_n|$は$\mathbf{R}_+^*$で乗算可能です(章IV, § 7, no. 4,定理4)。したがって、各 $\varepsilon > 0$ には $\mathbf{N}$ の有限部分集合 $J_0$ が存在し、$J_0$ を満たさない$\mathbf{N}$ のすべての有限部分集合 $L$ については、$\left| \prod_{n \in L} (1 + ||u_n||) - 1 \right| \leq \varepsilon$ が存在します。したがって結果です。

#### 系 {#top-ix-a0-n2-cor-1 .statement tag=0CAB}

*一般的な項が$u_n$である系列が絶対収束し、元$e - u_n$のどれも$A$の零因子でない場合、積$\prod_{n \in \mathbf{N}} (e + u_n)$は零因子ではありません$A$.*

整数 $n$ のうち、$|u_n| > 1$ となるような有限の数のみが存在します。 $J = [a, m]$ を、$\mathbf{N}$ 含むこれらすべての整数の区間とします。 数列 $(e + u_n)$ の積は $p_J$ の積と元 $\prod_{n \notin J} (e - u_n)$ であり、その因子はすべて単位元 (章 IX, § 3, no. 7, 系から命題 12)、したがってそれ自体は単位元です。 $p_J$ は非ゼロの約数の有限数の積であるため、零因子ではなく、したがって $\prod_{n \in \mathbf{N}} (e + u_n)$ は零因子ではありません。

定理 2 によって与えられる十分な乗算性条件は、一般に必要ありません (cf. 練習問題 6)。ただし、$A$ が体 $\mathbf{R}$ を超えた有限階数の代数である (つまり、$A$ は $\mathbf{R}$ を超えたベクトル空間として有限次元である) という重要なケースでは必要です。特に、$A$ が四元数 $\mathbf{H}$ の除算環、または行列環 $\mathbf{M}_n(\mathbf{R})$ の場合に当てはまります。

#### 命題 1 {#top-ix-a0-prop-1 .statement tag=0CAC}

*$A$を$\mathbf{R}$に対する有限階数の標準代数とします。 $(e + u_n)$ が $A$ の乗算可能な数列であり、その積が $A$ の単位元である場合、一般項が $u_n$ である系列は絶対収束します。

章 VII, § 3, no. 1、命題 2 から、数 $c > 0$ が存在し、すべての有限族点の $A$ の $(x_i)_{i \in I}$ に対して、次のようになります。

$$
\sum_{i \in I} \|x_i\| \leq c \sup_{J \subset I} \left| \sum_{i \in J} x_i \right|.
$$

$(a_i)_{i \in \mathbf{N}}$ を $A$ の元の任意の数列とします。 $\mathbf{N}$ の各有限部分集合 $I$ に、

$$
p_I = \prod_{i \in I} (e + a_i), \quad s_I = \sum_{i \in I} a_i, \quad \sigma_I = \sum_{i \in I} \|a_i\|.
$$

#### 補題 1 {#top-ix-a0-lem-1 .statement tag=0CAD}

$\mathbf{N}$ の各有限部分集合 $I$ について、$\varphi(I) = \sup_{J \subset I} ||p_J - e||$ とします。次に、$I$ の各部分集合 $J$ について、次のようになります。

$$
||p_J - e - s_J|| \leq \varphi(I)\sigma_J.
$$

$J$ が空の場合、補題は明らかです。 $J$の元の数の帰納法までにそれを証明します。 $J = K \cup \{j\}$ とします。ここで、$\{j\}$ は厳密にすべての $i \in K$ よりも大きくなります。それから$p_J = p_K(e + a_j)$と

$$
s_J = s_K + a_j,
$$

それで

$$
p_J - e - s_J = p_K - e - s_K + (p_K - e)a_j,
$$

そして、$\varphi(I)$の帰納的仮定と定義により、次のようになります。

$$
||p_J - e - s_J|| \leq \varphi(I)\sigma_K + \varphi(I)||a_j|| = \varphi(I)\sigma_J,
$$

これは補題を証明します。

#### 補題 2 {#top-ix-a0-lem-2 .statement tag=0CAE}

$I$ が $\mathbf{N}$ の有限部分集合で、$\varphi(I) < 1/c$ となる場合、

$$
\sigma_I \leq c\varphi(I)/(1 - c\varphi(I)).
$$

$\sigma_J \leq \sigma_I$ 以降、$I$ の部分集合 $J$ ごとに、次の式が得られます (2)

$$
||s_J|| \leq \varphi(I)\sigma_I + ||p_J - e|| \leq (1 + \sigma_I)\varphi(I);
$$

また、$\sigma_I \leq c \cdot \sup_{J \subset I} ||s_J||$ なので、(1) より、次のようになります。

$$
\sigma_I \leq c\varphi(I)(1 + \sigma_I),
$$

それが結果につながります。

さて、$(e + u_n)$ を $A$ の乗算可能な数列とし、その積は単位元です。 定理 1 により、$\mathbf{N}$ の有限部分集合 $J_0$ が存在し、$J_0$ を満たさない $\mathbf{N}$ の各有限部分集合 $H$ について、次のようになります。

$$
\left| \prod_{i \in H} (e + u_i) - e \right| \leq 1/2c.
$$

補題 2 により、$J_0$ を満たさない $\mathbf{N}$ のすべての有限部分集合 $H$ に対して $\sum_{i \in H} ||u_i|| - 1$ となるため、(章 IV, § 7, no. 1, 定理 1) ファミリー $(||u_n||)$ は次のようになります。 $\mathbf{R}$ で要約できます。

### 3. 無限積

正規化された代数 $A$ の点のそれぞれの数列 $(x_n)$ に対して、*部分的な積* $p_n = \prod_{k=0}^n x_k$ の対応する数列を作りましょう。その場合、数列 $(x_n)$ と $(p_n)$ の *対* は、一般的な因子が $x_n$ である無限積と呼ばれます。一般的な因子 $x_n$ を伴う無限積は、数列 $(p_n)$ が $A$ に収束する場合、収束するといいます。この数列の極限は、数列$(x_n)$の積と呼ばれ、$\prod_{n=0}^\infty x_n$で表されます。

#### 命題 2 {#top-ix-a0-prop-2 .statement tag=0CAF}

*$(x_n)$ * を完全な正規化代数* $A$ の点の数列とします。

a) *一般的な因子が * $x_n$ * である無限積が * 収束し、* $\prod_{n=0}^\infty x_n$ * が $A$ の単位元である場合、 *それぞれについて* $\varepsilon > 0$ * 整数* $n_0$ *が存在する*
$$
\left\| \prod_{k=m}^n x_k - e \right\| \leq \varepsilon
$$
*いつでも* $n_0 \leq m \leq n$。

b) *逆に、数列* $(x_n)$ * がこの条件を満たす場合、無限積と一般因子* $x_n$ * は収束します。そして、それぞれ* $x_n$ * が $A$ の単位元である場合、 * $\prod_{n=0}^\infty x_n$ * は単位元* になります。

この命題の証明は、 定理 1 の証明に段階的に続き、読者に委ねられています (定理 1 の証明の $N$ の有限部分集合 $L$ は、 区間）。

#### 系 1 {#top-ix-a0-prop-2-cor-1 .statement tag=0CAG}

*一般的な因子* $x_n$ を持つ無限積が *収束し、* $\prod_{n=0}^\infty x_n$ * が単位元* である場合、*その後* $\lim_{n \to \infty} x_n = e$ になります。

#### 系 2 {#top-ix-a0-prop-2-cor-2 .statement tag=0CAH}

*一般因子* $x_n$ * を持つ無限積が収束し、* $\prod_{n=0}^\infty x_n$ * が単位元* である場合、*一般因子* を持つ無限積
$$
y_n = x_{n+h} \quad (n \geq 0)
$$
*収束しています*。

数列 $(y_n)$ の積は $\prod_{n=h}^\infty x_n$ で表され、一般的な因子 $x_n$ と無限積の添字 $h$ の剰余とも呼ばれます。

まだ仮定未満で、$\prod_{n=h}^\infty x_n$ は単位元ですが、命題 2 から、$(z_n)$ が数列である場合、添字の有限数を除くすべての$z_n = x_n$ は、一般式で積になります。 因子 $z_n$ は収束しています。

#### 命題 3 {#top-ix-a0-prop-3 .statement tag=0CAI}

*$(k_n)$ *整数* $\geq 0$ の真に増加する数列としましょう*、*そのような* $k_0 = 0$; *無限積と一般因子* $x_n$ *収束*、*そして*

$$
u_n = \prod_{p=k_n}^{k_{n+1}-1} x_p,
$$

その場合、一般的な因子が $u_n$ である無限積は収束し、次のようになります。

$$
\prod_{n=0}^{\infty} u_n = \prod_{n=0}^{\infty} x_n.
$$

数列の部分積の数列について、 $(u_n)$ は、数列 $(x_n)$ の部分積の数列の部分列です。

最後に、アーベル群 (章 III, § 5, no. 7) に使用されたのと同じ議論は、正規化された代数 $\mathbf{A}$ の数列 $(x_n)$ が *乗算可能* である場合、積が一般的であることを示します。 因子は $x_n$ が収束し、

$$
\prod_{n=0}^{\infty} x_n = \prod_{n \in \mathbf{N}} x_n
$$

($\prod_{n=0}^{\infty} x_n$とも表記されます)。 逆はもちろん真実ではありません (cf. 練習問題 7)。

### 練習問題 {#top-ix-a0-exercises}

[練習問題付録 0](exercises/a0/)を参照してください。
