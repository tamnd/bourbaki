---
book: ens
book_title: Theory of Sets
chapter: IV
chapter_title: STRUCTURES
section: 3
section_title: Universal mappings
lang: ja
source: ens-i-iv
source_edition: 2004, Springer
book_pages: 283-288, 294-295
pdf_pages: 0288-0293, 0299-0300
extraction: ocr
subsections:
    - "no": 1
      title: UNIVERSAL SETS AND MAPPINGS
      page: 283
      pdf_page: 288
    - "no": 2
      title: EXISTENCE OF UNIVERSAL MAPPINGS
      page: 284
      pdf_page: 289
    - "no": 3
      title: EXAMPLES OF UNIVERSAL MAPPINGS
      page: 286
      pdf_page: 291
statements: 0
exercises: 3
content_sha256: 1ce4e01439563934df12a5f0adf4c074a5b399a6b85c11b90d4390c8dfda9229
translated_from: content/en/ens/IV/03_s3_universal_mappings.md
translation_method: google
source_content_sha256: 02143cebc191d935f4dc730de8191e96a819d51f624ae1e4a809f5d496463365
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: 86b9a378270dd6e001a2d5b9523360db05ea89f6778d308e7313667a49c90a4e
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## 3. ユニバーサル写像

### 1. ユニバーサル集合および写像

$\mathscr{T}$を集合の理論より強い理論とし、Eを$\mathscr{T}$の項とする。 $\Sigma$ を $\mathscr{T}$ の構造の種とする。簡単にするために、$\Sigma$ は単一の (主な) 基底集合で定義されていると仮定し、簡潔にするために、「$\Sigma$ の種構造を備えた集合」を「$\Sigma$ セット」と言うことにします。さらに、$\Sigma$ 種に対して $\sigma$-射が定義されていると仮定します (§ 2, no. 1。§ 2 のように、「$\sigma$-射」の代わりに「射」とします)。最後に、種 $\Sigma$ は基底集合 $x$ で定義され、$s$ を総称構造 (§ 1, no. 4) として持ち、項 $\alpha\{x,s\}$ が $\mathscr{T}_{\Sigma}$ で定義されていると仮定します。 満たす次の条件:

(QM$_{\mathrm{I}}$) *関係 $\alpha\{x,s\}\subset\mathscr{T}(E;x)$ は $\mathscr{T}_{\Sigma}$ で真です。*

(QM$_{\mathrm{II}}$) *($\mathscr{T}$より強い理論$\mathscr{T}'$において)FとF′が種$\Sigma$の構造$\mathscr{S},\mathscr{S}'$を備えた2つの集合であり、$f$がFの射をF′にすると、 関係 $\varphi\in\alpha\{F,\mathscr{S}\}$ は $f\circ\varphi\in\alpha\{F',\mathscr{S}'\}$ を意味します。*

関係 $\varphi\in\alpha\{x,s\}$ を $\varphi$ が E から $x$ ($s$ を付与) への $\alpha$ 写像であることをというで表現します。

次の条件が満たされる場合、$\Sigma$ 集合 $F_E$ および E の $F_E$ への $\alpha$ マッピング $\varphi_E$ は *普遍* であると言われます。

$(AU)$ *E の $\varphi$ を $\Sigma$ 集合 F にマッピングする各 $\alpha$ に対して、 $\varphi=f\circ\varphi_E$ となるような、F への $F_E$ の固有射$f$ が存在します。

対 $(F_E,\varphi_E)$ は、E に対する普遍的な写像問題* の *解であるとも言われます ($\Sigma$、$\sigma$、$\alpha$ に対して)。

¶ $(F'_E,\varphi'_E)$ と $(F''_E,\varphi''_E)$ を、E の普遍的な写像問題の 2 つの解とします。条件 $(AU)$ は、$F''_E$ に $F'_E$ の一意な準同型 $f_1$ が存在することを示します。 一意な準同型 $f_2$ の $F''_E$ を $F'_E$ にすると、$\varphi''_E=f_1\circ\varphi'_E$ と $\varphi'_E=f_2\circ\varphi''_E$ になります。従って、$\varphi''_E=f_2\circ f_1\circ\varphi'_E$ と $\varphi'_E=f_1\circ f_2\circ\varphi''_E$ があります。 適用 $(AU)$ $F=F'_E$ と $\varphi=\varphi'_E$ の場合、$f_2\circ f_1$ は$F'_E$ の恒等写像であることがわかります。同様に、$f_1\circ f_2$ は$F''_E$ の恒等写像です。その結果、(§ 2, no. 1、基準 CST8) $f_1$ は、$F''_E$ に対する $F'_E$ の *同型* であり、$f_2$ はその逆同型です。この結果は、E に対する普遍写像問題の解が同型* まで * 一意であるというというによって表されます。

対 $(F_E,\varphi_E)$ が E の普遍的な写像問題の解であることを検証するには、多くの場合、次の 2 つの条件を検証すると便利です。

$(AU'_{\mathrm I})$ *すべての $\Sigma$ 集合 F および E から F へのすべての $\alpha$ マッピング $\varphi$ に対して、$\varphi=f\circ\varphi_E$ となるような F への $F_E$ の射 $f$ が存在します。

$(AU'_{\mathrm{II}})$ *すべての $\Sigma$ セット F について、$\varphi_E(E)$ に一致する F に含まれる $F_E$ の 2 つの射は等しい。*

なぜなら、これら 2 つの条件が満たされる場合、$(AU'_{\mathrm I})$ によって存在が保​​証されている射 $f$ は、$(AU'_{\mathrm{II}})$ によって一意であるからです。逆に、$(AU)$ が $(AU'_{\mathrm I})$ を意味することは明らかです。さらに、$f$と$f'$が、$\varphi_E(E)$に一致する$F_E$の2つの射をFにすると、$\alpha$マッピングへの適用$(AU)$によって、$f\circ\varphi_E=f'\circ\varphi_E$、よって$f=f'$が得られます。 $f\circ\varphi_E$。従って、$(AU)$ は $(AU'_{\mathrm{II}})$ を意味します。

### 2. 普遍的な存在写像

普遍的な写像問題には、必ずしも解 (練習問題 1) があるとは限りません。ただし、次の条件が解の存在を暗示していることを示します。

$(CU_{\mathrm I})$ *$\Sigma$ セットのファミリーの積ごとに、積構造の種 $\Sigma$ (§ 2, no. 4) が存在します。*

$(CU_{\mathrm{II})}$ *$(F_i)_{i\in I}$ を $\Sigma$ セットの族とし、各 $i\in I$ について、$\varphi_i$ を E の $F_i$ への $\alpha$ マッピングとします。次に、E の写像 $(\varphi_i)_{i\in I}$ を $\prod_{i\in I}F_i$ (積構造を付与) にすると、$\alpha$ マッピング* になります。

$\Sigma$-集合 F の部分集合 G は、F で構造誘導する構造 G で種 $\Sigma$ ($\S\,2$、no. 4) の場合、$\Sigma$-*許容*であると言われます。

$(\mathrm{CU_{III}})$ *次のプロパティを持つ基数* $\mathfrak{a}$ が存在します: for each* $\Sigma$-*集合* F *およびevery* $\alpha$-*写像* $\varphi$ *of* E *into* F *存在します* $\Sigma$-*許容可能含む* $\varphi(\mathrm{E})$ が * 基数* $\leqslant \mathfrak{a}$ である部分集合* G *of* F *は、* $\varphi$ * と同じグラフを持つ * E * へ * 写像が * $\alpha$-*写像である、そして、* G * の 2 つの射を * $\Sigma$-*集合に変換すると、* $\varphi(\mathrm{E})$ に一致し、*等しい*になります。

CST22。 *条件* $(\mathrm{CU_I})$ *から* $(\mathrm{CU_{III}})$ *が満たされる場合、* E *に対する普遍的な写像問題は解になります。

まず、$(\mathrm{AU'_I})$を満たす対$(\mathrm{F_E},\ \varphi_\mathrm{E})$が存在する場合、Eに対する普遍写像問題の解も存在することを示します。 なぜなら、$(\mathrm{CU_{III}})$ までに、$\mathrm{F_E}$ 含む $\varphi_\mathrm{E}(\mathrm{E})$ の $\Sigma$ 許容可能な部分集合 $\mathrm{F'_E}$ が存在するため、$\varphi_\mathrm{E}$ と同じグラフを持つ $\mathrm{F'_E}$ への E の写像 $\varphi'_\mathrm{E}$ は、 $\alpha$-マッピング、および $\varphi_\mathrm{E}(\mathrm{E})$ に一致する $\mathrm{F'_E}$ の 2 つの射を $\Sigma$-セットに組み込むと、それらは等しくなります。 $j$を$\mathrm{F'_E}$の標準単射を$\mathrm{F_E}$にすると、$\varphi_\mathrm{E} = j \circ \varphi'_\mathrm{E}$になります。 $\mathrm{F_E}$ の射 $f$ を $\Sigma$ 集合 F にすると、$f \circ j$ は $\mathrm{F'_E}$ の射が F になり、$f \circ \varphi_\mathrm{E} = (f \circ j) \circ \varphi'_\mathrm{E}$ が得られます。 したがって、$(\mathrm{F'_E},\ \varphi'_\mathrm{E})$ が $(\mathrm{AU'_I})$ と $(\mathrm{AU'_{II}})$ を満たすことは明らかです。

対 $(\mathrm{F_E},\ \varphi_\mathrm{E})$ 満たす $(\mathrm{AU'_I})$ の存在を確立することが残っています。 $s \in \mathrm{S}(x)$ を構造 $\Sigma$ の種の典型的な特徴付けとし、次の特性を持つすべてのトリプル $\lambda = (\mathrm{X},\ \mathrm{V},\ \mathrm{P})$ からなる $\mathfrak{P}(\mathfrak{a}) \times \mathrm{S}(\mathfrak{a}) \times \mathfrak{P}(\mathrm{E} \times \mathfrak{a})$ の部分集合 L を考えます: 「V は $\mathrm{X} \subset \mathfrak{a}$ 上の種 $\Sigma$ の構造であり、P はE の X への「$\alpha$-マッピング (構造V に関して)」 (エシュロン構築スキーム S の長さについて段階的に議論することで簡単にわかるように、$\mathrm{S}(\mathrm{X}) \subset \mathrm{S}(\mathfrak{a})$ があることに注目してください)。 すべての $\lambda = (\mathrm{X},\ \mathrm{V},\ \mathrm{P}) \in \mathrm{L}$ について、構造 V を備えた $\mathrm{X}_\lambda$ 集合 X と、E の $\varphi_\lambda$ 写像をグラフが P である $\mathrm{X}_\lambda$ で表します。

$\mathrm{F_E}$ を $\mathrm{X}_\lambda$ の積である $\Sigma$ セットとし ($(\mathrm{CU_I})$ までに存在します)、$\varphi_\mathrm{E}$ を E の $\mathrm{F_E}$ への写像 $x \to (\varphi_\lambda(x))$ とします。これは、次の利点による $\alpha$ マッピングです。 $(\mathrm{CU_{II}})$。 対 $(\mathrm{F_E},\ \varphi_\mathrm{E})$ が $(\mathrm{AU'_I})$ を満たすことを示しましょう。 E の $\alpha$ 写像 $\varphi$ を $\Sigma$ 集合 F にすると、G を $(\mathrm{CU_{III}})$ で述べた条件を満たす F の部分集合とします。 $j$ を F への G の標準単射とし、$\psi$ を $\varphi$ と同じグラフを持つ G への E の写像とすると、$\varphi = j \circ \psi$ となります。 $(\mathrm{CU_{III}})$ から、$\psi$ は E から G への $\alpha$ 写像であることがわかります。カード (G) $\leqslant \mathfrak{a}$ なので、G と等価な $\mathfrak{a}$ の部分集合 G$'$ があります。$g$ を G の全単射とします。 G$'$。 G 上の種 $\Sigma$ の $g$ 構造によって輸送を計算すると、L の定義元 $\lambda$ が存在し、G$'$ (輸送される構造に恵まれる) が等しくなります。 $\mathrm{X}_\lambda$ など、$g \circ \psi = \varphi_\lambda$ まで。次に、$f = j \circ \overset{-1}{g} \circ \mathrm{pr}_\lambda$ は $\mathrm{F_E}$ の射を F にして $\varphi = f \circ \varphi_\mathrm{E}$ となり、証明が完成します。

CST23。 *E に対して * $(\mathrm{F_E},\ \varphi_\mathrm{E})$ * を汎用写像問題の解とします。 *すると* $\varphi_\mathrm{E}$ * は * E の単射になります * $\mathrm{F_E}$ *個別の元* の各対について、その場合に限ります$x$、$y$ *of* E、*存在* $\alpha$-*写像* $\varphi$ *of* E *into a* $\Sigma$-*集合* F *そのような* $\varphi(x) \neq \varphi(y)$。

$\varphi_\mathrm{E}$ は $\alpha$ マッピングであるため、基準は定義の明らか帰結です。

¶ この場合、$\alpha$-マッピングは E の元を *分離する* と言われており、通常、用語では E の元と $\varphi_\mathrm{E}$ の下のそれらの像を区別しません。この規則では、$(\mathrm{F_E},\ \varphi_\mathrm{E})$ が普遍的な写像問題の解であり、条件 $(\mathrm{CU_{III}})$ が満たされる場合、E のすべての $\alpha$ マッピングは$\Sigma$ 集合 F *拡大するを一意に射に変換します。の* $\mathrm{F_E}$ *に* F.

### 3. ユニバーサル写像の例

\* これに続く例については、ほとんどの部分については、この系列の別の場所で詳しく説明します。

I。 *自由代数構造.* E を集合とし、$\Sigma$ を合成の 1 つ以上の法則によって定義される代数構造の一種とします。検討中の種 $\Sigma$ の *準同型* を射とし、E の *写像を $\Sigma$ セット (他の語、$\alpha \{ x,\ s \} = \mathfrak{F}(\mathrm{E},\ x)$) に *任意* マッピングする $\alpha$ とします。代数のすべての通常の種類構造満たす $(\mathrm{CU_{III}})$;割り算環構造を除いて、それらは満たす$(\mathrm{CU_I})$でもあり、$(\mathrm{CU_{II}})$はここでは$(\mathrm{CU_I})$の自明な帰結です。

一般に、集合で少なくとも 2 つの元を含む$\Sigma$ の種構造が存在するため、$\alpha$ マッピングは E の元を分離し、したがって E は $\mathrm{F_E}$ に埋め込まれていると考えることができます。 $\mathrm{F_E}$ は、* E によって生成された *自由* $\Sigma$-*集合であると言われています。 したがって、代数では、*自由半群*、*自由群*、*自由加群*、および *自由代数* について話します。

II。 *分数の環と体。* Eを単位元を持つ可換環とし、Sを含む0ではない乗法的に閉じたEの部分集合とする。$\Sigma$を次の種とする。 可換環の構造と単位元、射は環準同型になり、変換単位元は単位元になります。 $\alpha$-マッピングは、E の準同型 $\varphi$ を単位元を含む可換環 A に変換することになり、$\varphi(1) = 1$ と $\varphi(\mathrm{S})$ 含むは A の *単位元* のみになります。 条件 $(\mathrm{CU_{III}})$ ($\mathfrak{a} = \mathrm{Card}\ (\mathrm{E})\ \mathrm{Card}\ (\mathbf{N})$ を含む) のうち、$(\mathrm{QM_{II}})$、$(\mathrm{CU_I})$ がすぐに確認されます。したがって、普遍的な写像問題は常に解 $(\mathrm{F_E},\ \varphi_\mathrm{E})$ を持ちますが、一般に $\varphi_\mathrm{E}$ は単射的ではありません。最も頻繁に発生するケースは、$E$ が整域であるケースです。この場合、$\varphi_E$ は単射です。さらに、$S = E - \{0\}$ を取ると、$F_E$ は体となり、$E$ の分数* の *体と呼ばれます。

III。 *加群の 2 つのうちテンソル積.* $E$ を、単位元を持つ可換環 $C$ に対する 2 つの加群の積 $A \times B$ とします。 $\Sigma$ を $C$ モジュール構造の種とし、射を線形写像とし、$\alpha$ マッピングを $A \times B$ の写像を $C$ モジュールに *双線形* とします。 条件 $(QM_{II})$ は明らかに満足しており、$(CU_I)$ から $(CU_{III})$ ($\mathfrak{a} = \mathrm{Card}\ (E)\ \mathrm{Card}\ (C)\ \mathrm{Card}\ (\mathbf{N})$ と) も同様です。ユニバーサル $C$ モジュール $F_E$ 対応するから対 $(A, B)$ は、$A$ と $B$ の *テンソル積* と呼ばれ、$A \otimes B$ と書かれます。普遍的な写像 $\varphi_E$ は $(x,\ y) \to x \otimes y$ と書かれます。それは双線形ですが、一般に単射的ではありません。

IV。 * 加群の演算子の環の拡大。* $A$ を単位元の可換環とし、$B$ を $A$ の部分環含む単位元とします$A$、そして $E$ を $B$ モジュールとします。種 $\Sigma$ は $A$ モジュール構造の種で、射は $A$-*線型* 写像、$\alpha$ マッピングは $E$ の $B$-*線型* 写像です。 $A$-モジュール。 $B$ モジュール $E$ への汎用 $A$ モジュール $F_E$ 対応するは、$E$ の演算子 $B$ の $A$ 環に * 拡張することで得られると言われています。

V。 *制服空間の完成* $E$を制服空間とします。 $\Sigma$ を完全なハウスドルフ均一空間の構造の種とし、射を一様連続写像とし、$\alpha$ マッピングを $E$ の一様連続写像として完全なハウスドルフ均一にします。 空間。完全なハウスドルフのユニフォーム空間の $\Sigma$ 許容される部分集合は、ここでは *非公開* の部分集合 (空間の位相に関して)、および条件 $(QM_{II})$ および $(CU_I)$ から $(CU_{III})$ です。満足しています（$\mathfrak{a} = 2^{2^{\mathrm{Card}(E)}}$）。完全なハウスドルフ制服空間は、$E$ (*一般位相*、章 II, § 3, no. 7) に関連付けられたハウスドルフ制服空間の *完成* です (同型まで)。

VI。 *Stone-Čech の圧縮。* $E$ を完全に正規の空間とします。 $\Sigma$ はコンパクト空間の構造の種であり、射は連続写像 (コンパクト空間からコンパクト空間) であり、$\alpha$ マッピングは $E$ の連続写像でコンパクトです空間。 $\Sigma$ で許容される部分集合は再び *クローズド* の部分集合であり、条件 $(QM_{II})$、$(CU_I)$ から $(CU_{III})$ は簡単に検証されます (例 V と同じ基数を使用)。圧縮空間 $F_E$ は、$E$ のすべての連続写像を区間 $[0,\ 1]$ に変換する最も粗い均一性に関して$E$ を完了することによって得られる「ストーンチェフ圧縮化」です（同型まで）。 $\mathbf{R}$ は一様連続です (*一般的な位相*、章 IX, § 1、練習問題 7)。 写像 $\varphi_E$ は単射法です。E の 2 つの異なる点は、E の連続する写像によって $[0, 1]$ に分離できるからです。

VII。 *自由トポロジカル群*。 E を完全に正則な空間とし、$\Sigma$ をハウスドルフトポロジカル群構造の種とし、射を連続準同型とします。そして、$\alpha$-マッピングを E の連続写像としてハウスドルフ トポロジカル群に取り込みます。 条件 $(\mathrm{QM_{II}})$ および $(\mathrm{CU_I})$ から $(\mathrm{CU_{III}})$ は、次の方法で簡単に検証できます。

$$\mathfrak{a} = \mathrm{Card\ (E)\ Card\ (\mathbf{N})}.$$

E に対するこの普遍的な写像問題の解であるハウスドルフ位相群 $\mathrm{F_E}$ は、空間* E によって生成される *自由位相位相群と呼ばれます。E の任意の 2 つの異なる点は、連続する写像によって分離できるためです。ハウスドルフ トポロジカル群 **R** への E、写像 $\varphi_\mathrm{E}$ は単射法です。 $\varphi_\mathrm{E}$ は、$\mathrm{F_E}$ [^1] の部分空間 $\varphi_\mathrm{E}(\mathrm{E})$ に対する E の同型写像であることがわかります。 $\Sigma$ をハウスドルフ トポロジカル群の構造の種とする代わりに、ハウスドルフ トポロジカルアーベル群、コンパクト群、ハウスドルフ トポロジカル群など、他の構造の種を取ることもできます。 環、ハウスドルフ位相幾何学ベクトル空間 (位相分割環を介して、補助基底集合とみなされる) など。

VIII。 *トポロジカル群* 上のほぼ周期的な写像。 E をトポロジー 群とします。 $\Sigma$ をコンパクト群構造の種とし、射を連続準同型とし、E の準同型をコンパクト群に連続する $\alpha$ マッピングをとります。 条件 $(\mathrm{QM_{II}})$、$(\mathrm{CU_I})$ ～ $(\mathrm{CU_{III}})$ は満たされており、$\mathfrak{a} = 2^{2^{\mathrm{Card\,(E)}}}$ が付いています。 E に対するこの普遍写像問題の解であるコンパクト群 $\mathrm{F_E}$ は、E に関連付けられた * コンパクト群と呼ばれます。 写像 $\varphi_\mathrm{E}$ は必ずしも単射的であるとは限りません。 形 $g \circ \varphi_\mathrm{E}$ ($g$ は E 上の連続実数値写像です) の E 上のすべての連続実数値写像は、E 上の *ほぼ周期的な写像* と呼ばれます。

IX。 *アルバニアの品種*。 Eを代数多様体とし、$\Sigma$をEと同じ基礎体上のアーベル多様体のうちの構造の種とする（アーベル多様体は代数群構造を備えた完全な代数多様体であり、必然的に可換である）。 射は、1 つのアーベルから他のに変化する有理写像です (それぞれの射は必ず準同型の合成と翻訳です)。 $\alpha$-マッピングは、E の有理写像からアーベル多様体です。 条件 $(\mathrm{CU_I})$ は満たされていませんが、E に対するこの普遍的な写像問題は、E の *アルバニア多様体* と呼ばれる解 $\mathrm{F_E}$ を認めます。一般に、有理数写像 $\varphi_\mathrm{E}$ は単射法ではありません。 \*

### 練習問題 {#ens-iv-s3-exercises}

[§ 3 に対して練習問題](exercises/s3/)を参照してください。

[^1]: P. SAMUEL、「普遍的写像と自由トポロジカル群について」*Bull を参照。 アメール。 数学。 Soc.*、**54** (1948)、591-598 ページ。
