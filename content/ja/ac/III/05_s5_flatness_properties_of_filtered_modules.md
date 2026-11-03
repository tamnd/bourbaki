---
book: ac
book_title: Commutative Algebra
chapter: III
chapter_title: GRADUATIONS. FILTRATIONS AND TOPOLOGIES
section: 5
section_title: Flatness properties of filtered modules
lang: ja
source: ac-i-vii
book_pages: 226-231, 259-260
pdf_pages: 0246-0251, 0279-0280
extraction: ocr
subsections:
    - "no": 1
      title: IDEALLY HAUSDORFF MODULES
      page: 226
      pdf_page: 246
    - "no": 2
      title: STATEMENT OF THE FLATNESS CRITERION
      page: 227
      pdf_page: 247
    - "no": 3
      title: PROOF OF THE FLATNESS CRITERION
      page: 228
      pdf_page: 248
    - "no": 4
      title: APPLICATIONS
      page: 230
      pdf_page: 250
statements: 11
exercises: 8
content_sha256: b3d2b9bf0933d5e91936cd7385844633878f9fe31c089d491f746f918bfce76e
translated_from: content/en/ac/III/05_s5_flatness_properties_of_filtered_modules.md
translation_method: google
source_content_sha256: 40502ef62aacbf121ac1011abdbd0936abda1c04356f56a21967a20f392ffa93
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: e613ef871bc2187ca55ab942d9728884a0d02fa9fe4265d4291f16f6c2a12c97
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## 5. フィルタ処理された加群の平坦性特性

### 1. 理想的にはハウスドルフ加群

#### 定義 1 {#ac-iii-s5-def-1 .statement tag=04IO}

*A を可換環および A のイデアルである $\mathfrak{g}$ とします。 A-加群 M は、A の有限生成されたイデアル $\mathfrak{a}$ ごとに、A-加群 $\mathfrak{a} \otimes_A M$ が3 進数位相.*

この定義に $\mathfrak{a} = A$ を入れると、M は必ず 3 進数位相を持つ *Hausdorff* であることがすでにわかりました。

*例*

#### 例 1 {#ac-iii-s5-n1-exa-1 .statement tag=04IP}

A がネーター で、$\mathfrak{g}$ が A のヤコブソン根基に含まれる場合 (A が 3 進数位相を持つザリスキー 環の場合、他の語にも含まれる)、すべての *有限生成* A-加群は理想的にはハウスドルフ (*§3*, no. 3、命題 6)。

#### 例 2 {#ac-iii-s5-n1-exa-2 .statement tag=04IQ}

理想的なハウスドルフ加群のすべての直和は、関係により、理想的なハウスドルフ加群になります。
$$
\mathfrak{g}^n \left( a \otimes_A \bigoplus_{\lambda \in L} M_\lambda \right) = \mathfrak{g}^n \bigoplus_{\lambda \in L} (a \otimes_A M_\lambda) = \bigoplus_{\lambda \in L} \mathfrak{g}^n (a \otimes_A M_\lambda).
$$

#### 例 3 {#ac-iii-s5-n1-exa-3 .statement tag=04IR}

A-加群 M がフラットで、$\mathfrak{g}$ 進数位相を持つハウスドルフである場合、理想的にはハウスドルフです。なぜなら、$a \otimes_A M$ は M の部分加群と識別され、$a \otimes_A M$ 上の $\mathfrak{g}$ 進数位相はより細かいであるからです。 位相は、仮定によるハウスドルフである M の $\mathfrak{g}$ 進数位相によって $a \otimes_A M$ に誘導されます。

### 2. 平坦度基準の主張
A を環、$\mathfrak{z}$ A の両側理想、M を左モジュール、gr(A) と gr(M) を、それぞれ $\mathfrak{g}$ A と環 A および加群 M に関連付けられた段階的環および段階的 gr(A) モジュールとします。 (§ 2, no. 3)。私たちは、すべての整数 $n \geq 0$ に対して全射 $\mathbf{Z}$ 加群準同型が存在することを見てきました (loc. cit.)。
$$
\gamma_n : (\mathfrak{g}^n / \mathfrak{g}^{n+1}) \otimes_{A/\mathfrak{g}} (M / \mathfrak{g}M) \to \mathfrak{g}^n M / \mathfrak{g}^{n+1} M
$$
およびグレード付けされた gr(A) モジュールのグレード付けされた準同型 / 次数 0
$$
\gamma_M : \mathrm{gr}(A) \otimes_{\mathrm{gr}_0(A)} \mathrm{gr}_0(M) \to \mathrm{gr}(M)
$$
制限から $\mathrm{gr}_n(A) \otimes_{\mathrm{gr}_0(A)} \mathrm{gr}_0(M)$ はすべての $n$ に対して $\gamma_n$ であり、したがってこれは全射的です。

#### 定理 1 {#ac-iii-s5-thm-1 .statement tag=04IS}

A と M A-加群の理想を A 可換環、$\mathfrak{g}$ とします。次のプロパティを考慮してください。
(i) M は太っています A-加群。
(ii) $\mathfrak{z}$ によって全滅される A-加群 N ごとに $\mathrm{Tor}_1^A(N, M) = 0$。
(iii) $M / \mathfrak{g}M$ はアジャラト $(A / \mathfrak{g})$ モジュールであり、標準写像 $\mathfrak{z} \otimes_A M \to \mathfrak{g}M$ は全単射です (後者の条件は関係 $\mathrm{Tor}_1^A(A, M) = 0$ と完全系列により $\mathrm{Tor}_1^A(A / \mathfrak{g}, M) = 0$ と等価です)
$$
\mathrm{Tor}_1^A(A, M) \to \mathrm{Tor}_1^A(A / \mathfrak{g}, M) \to \mathfrak{z} \otimes_A M \to M ).
$$
(iv) $M / \mathfrak{g}M$ はアジャラット $(A / \mathfrak{g})$ モジュールおよび標準準同型
$$
\gamma_M : \mathrm{gr}(A) \otimes_{\mathrm{gr}_0(A)} \mathrm{gr}_0(M) \to \mathrm{gr}(M)
$$
は全単射です (§ 2, no. 8 の性質 (GR))。
(v) すべての $n \geq 1$ に対して、$M / \mathfrak{g}^n M$ はフラットな $(A / \mathfrak{g}^n)$ モジュールです。
次に (i) $\Rightarrow$ (ii) $\Leftrightarrow$ (iii) $\Rightarrow$ (iv) $\Leftrightarrow$ (v) となります。
さらに $\mathfrak{g}$ がゼロポテントである場合、または A がネーター で M が理想的にはハウスドルフである場合、性質 (i)、(ii)、(iii)、(iv)、および (v) は等価です。

#### 注意 {#ac-iii-s5-n1-rem-1 .statement tag=04IT}

$A / \mathfrak{g}$ が (アプリケーションでよく起こるように) 体の場合、条件 「M/ $\mathfrak{g}M$ はフラットな $(A / \mathfrak{g})$ モジュールである」が A-加群 M ごとに自動的に成立し、プロパティ (iii) と (iv) の主張が単純化されます。さらに、この場合、性質 (v) はというと同等であり、$M / \mathfrak{g}^n M$ はすべての整数 $n \geq 1$ (章 11、§ 3, no. 2、系 2 ～ 命題) に対して自由な $(A / \mathfrak{g}^n)$ モジュールです。 5)。

### 3. 平坦度基準の証明

(A) *含意* (i) $\Rightarrow$ (ii) $\Leftrightarrow$ (iii)

(i) $\Rightarrow$ (ii) の意味は明らか (章 I, § 4) です。 同値 (ii) $\Leftrightarrow$ (iii) は、$N$ で $(A/\mathfrak{g})$ モジュール構造が与えられることは、$A$ モジュール構造が与えられることと同等であるという事実を考慮して、章 I, § 4、命題 2 が $R = A, S = A/\mathfrak{g}, F = M, E = N$ に適用される特殊なケースです。その下では$N$は3で全滅します。

*注意* (1)。 条件 (ii) は以下と同等です。

(ii') $\operatorname{Tor}_1^A(N, M) = 0$ *すべての* $A$*-モジュール* $N$ ** 3 の冪によって消滅。

明らかに (ii') は (ii) を意味します。逆に、(ii) が当てはまる場合、特にすべての $n$ に対して $\operatorname{Tor}_1^A(\mathfrak{g}^n N / \mathfrak{g}^{n+1} N, M) = 0$ になります。 完全系列から
$$
0 \to \mathfrak{g}^{n+1} N \to \mathfrak{g}^n N \to \mathfrak{g}^n N / \mathfrak{g}^{n+1} N \to 0
$$
完全系列を導き出します
$$
\operatorname{Tor}_1^A(\mathfrak{g}^{n+1} N, M) \to \operatorname{Tor}_1^A(\mathfrak{g}^n N, M) \to \operatorname{Tor}_1^A(\mathfrak{g}^n N / \mathfrak{g}^{n+1} N, M)
$$
そして、$\mathfrak{g}^m N = 0$ のような整数 $m$ が存在するため、$n$ で帰納法を下降することによって、すべての $n \leq m$、特に $n = 0$ について $\operatorname{Tor}_1^A(\mathfrak{g}^n N, M) = 0$ であると推論します。

このことから、9 が *無能* である場合、(ii) は (i) を意味し、(ii') では *すべての* $A$*-モジュール* $N$ について $\operatorname{Tor}_1^A(N, M) = 0$ を意味し、したがって $M$ はフラット (章 I, § 4) であることがわかります。

(B) 次の命題を証明しましょう。

#### 命題 1 {#ac-iii-s5-prop-1 .statement tag=04IU}

*$A$ *を可換環とします。 3* $A$ * および* $M$ * $A$ * モジュール* の理想です。 *次の条件は同等です*:
(a) *全員* $n \geq 1$、$\operatorname{Tor}_1^A(A/\mathfrak{g}^n, M) = 0$。
(b) *全員* $n \geq 1$、*標準準同型*
$$
\theta_n : \mathfrak{g}^n \otimes_A M \to \mathfrak{g}^n M
$$
*は全単射*です。

*さらに、これらの条件は次のことを示唆しています*:
(c) *標準準同型* $\gamma_M : \operatorname{gr}(A) \otimes_{\operatorname{gr}_0(A)} \operatorname{gr}_r(M) \to \operatorname{gr}(M)$ *は全単射*です。 *逆に、* $\mathfrak{g}$ * が零能である場合、(c) は (a) と (b)* を意味します。

(a) と (b) の同値は完全系列から続きます
$$
0 = \operatorname{Tor}_1^A(A, M) \to \operatorname{Tor}_1^A(A/\mathfrak{g}^n, M) \to \mathfrak{g}^n \otimes_A M \to M.
$$

次の図式を検討してください
$$
\begin{array}{ccccccccc}
\mathfrak{g}^{n+1} \otimes_A M & \longrightarrow & \mathfrak{g}^n \otimes_A M & \longrightarrow & (\mathfrak{g}^n / \mathfrak{g}^{n+1}) \otimes_A (M / \mathfrak{g} M) & \longrightarrow & 0 \\
\downarrow \theta_{n+1} & & \downarrow \theta_n & & \downarrow \gamma_n & & \\
0 & \longrightarrow & \mathfrak{g}^{n+1} M & \longrightarrow & \mathfrak{g}^n M & \longrightarrow & \operatorname{gr}_n(M) & \longrightarrow & 0
\end{array}
$$

ここで、$(\mathfrak{g}^n/\mathfrak{g}^{n+1}) \otimes_A (M/\mathfrak{g}M)$ は正規的に $(\mathfrak{g}^n/\mathfrak{g}^{n+1}) \otimes_{A/\mathfrak{g}} (M/\mathfrak{g}M)$ と識別されることに注意してください。この図式は $\gamma_n$ の定義によって可換であり、その行は正確です。 (b) が成り立つ場合、$0$ と $\theta_{n+1}$ は全単射なので、余核の定義により $\gamma_n$ となり、したがって (b) は (c) を意味します。逆に、$\mathfrak{g}$ がゼロポテントであると仮定すると、(c) が (b) を意味することを示しましょう。 $n$ 十分大きいに対して $\mathfrak{g}^n \otimes_A M = \mathfrak{g}^n M = 0$ から $n$ に帰納法を下降することで議論します。次に、図式 (1) において、$\gamma_n$ と $\theta_{n+1}$ が全単射であると仮定します。次に、章 I, § 1, no. 4、系 1 から命題 2 により、$\theta_n$ も同様です。

(C) *暗示* (ii) $\Rightarrow$ (iv)

(ii) が成り立つ場合、*注意* 1 により (ii') も成り立ちます。 命題 1 は、$\gamma_M$ が同型であることを示します。一方、(ii) は (iii) を含意するため、$M/\mathfrak{g}M$ はフラットな $(A/\mathfrak{g})$ モジュールであることがすでにわかっており、これで (ii) が (iv) を含意する証明が完成します。

*注意* (2)。 命題 1 は、$\mathfrak{g}$ が無能である場合、(iv) は (iii) を意味することを示しています。 *注意* 1 を考慮すると、この場合、(i)、(ii)、(iii)、および (iv) が同等であることが証明されました。

(D) *同値* (iv) $\Leftrightarrow$ (v)

すべての $n \geq 1$ について、$M/\mathfrak{g}^n M$ は標準的な $(A/\mathfrak{g}^n)$ モジュール構造を持っています。 $(\mathfrak{g}/\mathfrak{g}^n)$-進濾過で濾過すると、$m < n$であれば$\mathrm{gr}_m(M/\mathfrak{g}^n M) = \mathrm{gr}_m(M)$、$m \geq n$であれば$\mathrm{gr}_m(M/\mathfrak{g}^n M) = 0$が明らかになります。すべての $k \geq 1$ について、$A_k = A/\mathfrak{g}^k$、$\mathfrak{g}_k = \mathfrak{g}/\mathfrak{g}^k$、$M_k = M/\mathfrak{g}^k M$ とします。 (iv)、(それぞれ $(v)_k$) は、(iv) (それぞれ (v)) から置き換えること $A, \mathfrak{g}, M$ と $A_k, \mathfrak{g}_k, M_k$ から導出された主張を表します。今述べたことから、(iv) は「すべての $k \geq 1$、$(iv)_k$ について」と同等であり、明らかに (v) は「すべての $k \geq 1$、$(v)_k$ について」と同等であることがわかります。次に、すべての $k$ に対して同値 $(iv)_k \Leftrightarrow (v)_k$ を確立するか、または $3$ が *ゼロポテント* である場合に (iv) $\Leftrightarrow$ (v) であることを示すだけで十分です。さて (*注意* 2) この場合、(iv) は (i) と同等であることが分かりました。 $M/\mathfrak{g}^n M$ は $M \otimes_A (A/\mathfrak{g}^n)$ と同型であるため、(i) は (v) (章 I, § 2, no. 7、系 2 から命題 8) を意味します。さらに、明らかに (v) は (i) を暗示します。したがって、すべての場合で同値 (iv) $\Leftrightarrow$ (v) を示し、また、$3$ がゼロポテントである場合の定理のすべての性質も示しました。

(E) *含意* (v) $\Rightarrow$ (i) *いつ* $A$ *がネーター かつ* $M$ *理想的にはハウスドルフ*

$A$ 標準写像 $j : a \otimes_A M \to M$ のすべてのイデアル $a$ が *単射* (章 I, § 2, no. 3, 命題 1) であることを証明すれば十分です。 $x \in \mathrm{Ker}\, j$ にしましょう。
$a \otimes_A M$ は $\mathfrak{g}$ 進数位相を持つハウスドルフであるため、整数 $n > 0$、$x \in \mathfrak{g}^n(a \otimes_A M)$ ごとにそれを検証するだけで十分です。 $f : \mathfrak{g}^n a \to a$ を標準単射とします。 $x \in \mathrm{Im}(f \otimes 1_M)$ を示すだけで十分です。 $b \in \mathfrak{g}^n$、$a \in a$、$m \in M$の場合、$f \otimes 1$の下の像、元の$(ba) \otimes m$の$(\mathfrak{g}^n a) \otimes_A M$は元 $(ba) \otimes m = b(a \otimes m)$の$a \otimes_A M$であるため、 $\mathrm{Im}(f \otimes 1_M) \subset \mathfrak{g}^n(a \otimes_A M)$。クルルの定理 (§ 3, no. 2, 定理 2) により、$a_j = a \cap \mathfrak{g}^k \subset \mathfrak{g}^n a$ となる整数 $k$ が存在します。 $i : a_j \to a$ が標準単射である場合、$x \in \operatorname{Im}(i \otimes 1_M)$ を示すだけで十分です。さて、$p : a \to a/a_k$ と $h : a/a_k \to A/\mathfrak{g}^k$ 標準写像で表すと、可換図式が存在します。

$$
\begin{array}{ccccccccc}
a_k \otimes_A M & \xrightarrow{i \otimes 1_M} & a \otimes_A M & \xrightarrow{p \otimes 1_M} & (a/a_k) \otimes_A M & \longrightarrow & 0 \\
& & \downarrow & & \downarrow h \otimes 1_M & & \\
& & M & \longrightarrow & (A/\mathfrak{g}^k) \otimes_A M & &
\end{array}
$$

最初の行は正確です。 $x \in \operatorname{Ker}(p \otimes 1_M)$ と、$x \in \operatorname{Ker} j$ by 仮定として、写像 $h \otimes 1_1$ が単射であることを証明すれば十分です。現在は、(代数、章 II, § 3, no. 6、系 3 ～ 命題 6) と書くこともできます。

$$
h \otimes 1_{M/\mathfrak{g}^k M} : (a/a_k) \otimes_{A/\mathfrak{g}^k} (M/\mathfrak{g}^k M) \to M/\mathfrak{g}^k M
$$

そして、$h$ は単射であり、(v) により、$M/\mathfrak{g}^k M$ はフラットな $(A/\mathfrak{g}^k)$ 加群であるため、これで証明が完成します。

### 4. アプリケーション

#### 命題 2 {#ac-iii-s5-prop-2 .statement tag=04IV}

$A$を可換環、$\mathfrak{g}$を$A$のイデアル、$B$を可換代数ネーター$A$として、$B$が$B$のヤコブソン根基に含まれるようにします。この場合、有限生成されたすべての $B$ 加群 $M$ は、$\mathfrak{g}$ に関して理想的なハウスドルフ $A$ 加群になります。

より一般的には、有限生成されたすべての $A$ 加群 $N$ について、$N \otimes_A M$ は $3$ 進数位相を持つハウスドルフであることがわかります。なぜなら、$N_{(B)} = N \otimes_A B$ は有限生成された $B$ モジュールであり、$B$ モジュール $N \otimes_A M$ は、テンソル積の結合性によって正規に $N_{,,} \otimes_B M$ と識別されるからです。 $\mathfrak{L}$ を $B$ のジェイコブソン根基とします。 $\mathfrak{g} B$ は $\mathfrak{L}$ に含まれるため、$N \otimes_A M$ の $\mathfrak{g}$ 進数位相は、$N_{(B)} \otimes_B M$ の $\mathfrak{L}$ 進数位相よりもより細かい位相と識別されます。しかし、後者の位相は、$N_{,,} \otimes_B M$ が有限生成された $B$ 加群 (no. 1, 例 1) であるため、ハウスドルフであり、よってが結論です。

#### 命題 3 {#ac-iii-s5-prop-3 .statement tag=04IW}

$A$を可換環、$B$を可換$A$代数、$\mathfrak{g}$を$A$のイデアル、$M$を$B$加群とする。 $B$ がネーター 環でフラットな $A$ 加群であり、$M$ が $\mathfrak{g} B$ に関して理想的にはハウスドルフであると仮定します。次の条件は同等です。
(a) $M$ はフラットな $B$ モジュールです。
(b) $M$ はフラット $A$ モジュール、$M/\mathfrak{g} M = M/(\mathfrak{g} B) M$ はフラット $(B/\mathfrak{g} B)$ モジュールです。
さらに標準準同型 $A/\mathfrak{g} \to B/\mathfrak{g} B$ が全単射である場合、条件 (a) および (b) も次と同等です。
(c) $M$ はフラット $A$ モジュールです。

条件 (a) は、章 I, §2, no. 7、命題 8 への系 2 および 3、および $M/\mathfrak{g} M$ が $M \otimes_B (B/\mathfrak{g} B)$ と同型であるという事実によって (b) を暗示します。 条件 (b) が成り立つと仮定します。 $M$ がフラットな $B$ モジュールであることを示すために、$A$ を $B$ に、$\mathfrak{g}$ を $\mathfrak{g} B$ に置き換えて、no. 2 の 1 を定理を適用するとします。したがって、標準写像 $f : \mathfrak{J}B \otimes_B M \to \mathfrak{J}M$ が単射であることを示すだけで十分です。簡単に検証できるように、$f_1$ を標準写像 $\mathfrak{J} \otimes_A B \to \mathfrak{J}B$ とし、$f_2$ 標準同型 $\mathfrak{J} \otimes_A M \to (\mathfrak{J} \otimes_A B) \otimes_B M ; f \circ (f_1 \circ 1_M) \circ f_2$ を標準写像 $f' : \mathfrak{J} \otimes_A M \to \mathfrak{J}M$ とします。ここで、$M$ はフラットな $A$ モジュールであるため、$f'$ は同型ですが、$B$ は $A ; f$ よりもフラットであるため、同型であるため、$f_1$ は同型になります。

$p : A/\mathfrak{J} \to B/\mathfrak{J}B$ を標準準同型とします。 $(B/\mathfrak{J}B)$ 加群構造から $p$ によって導出された $M/\mathfrak{J}M$ 上の $(A/\mathfrak{J})$ 加群構造は、$M \otimes_A (A/\mathfrak{J})$ の加群構造と同型です。次に、$M$ がフラット $A$ モジュールである場合、$M/\mathfrak{J}M$ はフラット $(A/\mathfrak{J})$ モジュールであり、したがって、$p$ が同型であればフラット $(B/\mathfrak{J}B)$ モジュールでもあることがわかります。したがって、この場合、(c) $\Rightarrow$ (b) であることが証明されました。

#### 系 {#ac-iii-s5-n4-cor-1 .statement tag=04IX}

*$A$ を可換ネーター 環、$\mathfrak{J}$ を $A$ のイデアル、$\hat{A}$ を $\mathfrak{J}$ 進数位相に関する $A$ のハウスドルフ完成とします。 $M$ は、$\mathfrak{J} \hat{A}$ に対する理想的なハウスドルフ $\hat{A}$ モジュールです。 $M$ がフラット $A$ モジュールであるためには、$M$ がフラット $\hat{A}$ モジュールであることが必要かつ十分です。*

実際、$\hat{A}$ はネーター 環 ($§ 3$、no. **4**、命題 8) であり、フラットな $A$ モジュール ($§ 3$、no. **4**、定理 3)、つまり $\mathfrak{J} \hat{A} = \hat{\mathfrak{J}}$ であることがわかっています。 ($§ 2$, no. 12, 命題 **16**) そして、標準準同型 $A/\mathfrak{J} \to \hat{A}/\hat{\mathfrak{J}}$ は全単射です ($§ 2$, no. 12, 命題 15)。したがって、命題 **3** が適用できます。

#### 命題 4 {#ac-iii-s5-prop-4 .statement tag=04IY}

*$A$と$B$を2つの可換なネーター環、$h : A \to B$環準同型、$3$を$A$の理想、$2$を$B$の理想とする含む $\mathfrak{J}B$ と $B$ のジェイコブソン根基に含まれています。 $\hat{A}$ を $3$ 進数位相に関する $A$ のハウスドルフ完了とし、$\hat{B}$ を $2$ 進数位相に関する $B$ のハウスドルフ完了とします。 $h$ はこれらのトポロジーと連続しているため、$h : \hat{A} \to \hat{B}$ は$\mathbf{8}$ を $\hat{A}$ 代数にします。 $M$ を有限生成された $B$ 加群とし、 $\hat{M}$ を $2$ 進数位相に関するハウスドルフ完了とする。次のプロパティは同等です。
(a) $M$ はフラットな $A$ モジュールです。
(b) $\hat{M}$ はフラットな $A$ モジュールです。
(c) $\hat{M}$ はフラットな $\hat{A}$ モジュールです。*

$2$ 進数位相を持つ $B$ はザリスキー 環であるため、$\hat{B}$ は忠実にフラットな $B$ 加群 ($§ 3$、no. 5、命題 9) であり、$M$ は正規同型です。 $M \otimes_B \hat{B}$ ($§ 3$、番号 **4**、定理 3);この標準同型は、$M$ の$M \otimes_B \hat{B}$ の $A$ モジュール構造上の $\hat{M}$ の $A$ モジュール構造の同型であることがすぐに検証されます。 適用命題章 I、$§ 3$、no. 2 のうち、$R$ が $B$、$S$ が $A$、$E$ の 4 つ$\hat{B}$、$F$ を $M$ で見ると、$M$ がフラット $A$ モジュールであるためには、$\hat{M}$ がフラット $A$ モジュールであることが必要かつ十分であることがわかります。さらに、$\hat{M}$ は有限生成された $\hat{B}$ モジュールであり、$\mathfrak{J} \hat{B}$ は $\mathfrak{Q} = \mathfrak{Q} \hat{B}$ に含まれているため、$\hat{B}$ ($§ 3$、no. **4**、命題 8) のヤコブソン根基に含まれています。したがって、$\hat{M}$ は、$\mathfrak{J} \hat{A}$ (命題 2) に関する理想的なハウスドルフ $A$ 加群です。したがって、条件 (b) と (c) は、系から命題 3 によって等価です。

### 練習問題 {#ac-iii-s5-exercises}

[§ 5 に対して練習問題](exercises/s5/)を参照してください。
