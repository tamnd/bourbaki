---
book: evt
book_title: Topological Vector Spaces
chapter: III
chapter_title: SPACES OF CONTINUOUS LINEAR MAPPINGS
section: 2
section_title: Bornological spaces
lang: ja
source: evt-i-v
book_pages: TVS III.11-TVS III.13, TVS III.40-TVS III.41
pdf_pages: 0143-0145, 0172-0173
extraction: ocr
statements: 6
exercises: 4
content_sha256: 99db4f809d7fed62d09378c0c5320147363bd27a96855ce063178138f49ad7df
translated_from: content/en/evt/III/02_s2_bornological_spaces.md
translation_method: google
source_content_sha256: 40a687273614f4755635004c7de82956200bd4dc25c1f116ef776c135c6ae0d1
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-b071ad41
glossary_version: 34
glossary_terms_sha256: 0fd05d29ce8ab1804efc37877e23d516f8e1265c11db0ad7a07042ddedfdf5f3
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## § 2。ボーンロジー 空間

この段落では、E は局所的に凸な空間を表し、$\mathscr{B}$ はその標準的なボーンロジー (III、p. 3、定義 5) を表します。

#### 補題 1 {#evt-iii-s2-lem-1 .statement tag=07M8}

— *G を準ノルム空間、p をその準ノルム、u 線形写像を G から E に変換するとします。次の条件は同等です* :

(i) *u は連続です* ;
(ii) u の下の G の単位元ボールの *像は E* で囲まれています。
(iii) *0 に向かう G の点の数列 $(x_n)$ ごとに、数列 $(u(x_n))$ は E* で制限されます。

(i) が (ii) を含意する (III, p. 4, cor. 1)、および (ii) が (iii) を含意するのは明らかです。 V を E の 0 の近傍とします。 $u^{-1}(V)$ が G の 0 の近傍ではない場合、$p(y_n) \leq \frac{1}{n^2}$ となる $G - u^{-1}(V)$ の点の数列 $(y_n)$ が存在します。したがって、数列 $x_n = n y_n$ は G および $u(x_n) \notin nV$ で 0 になる傾向があり、これは数列 $(u(x_n))$ が有界でないことを意味します。したがって、(iii) は (i) を意味します。

#### 命題 1 {#evt-iii-s2-prop-1 .statement tag=07M9}

*以下の条件は同等です* :
(i) *E の有界部分集合で有界される E 上のすべての準ノルムは連続です*。
(i') *E* の有界部分集合 (I、p. 7、定義 4) を吸収する E のすべての凸平衡部分集合は、E* の 0 の近傍です。
(ii) *E は半正規化空間 $E_A$ の帰納極限であり、A は E* の閉じた、凸状、平衡型、有界な部分集合の有向増加する集合の範囲にあります。
(ii') *半規格化された空間の族 $(E_i)_{i \in I}$ が存在し、すべての $i \in I$、線形写像 $u_i : E_i \to E$ に対して、E の位相が最も細かい局所凸位相となり、$u_i$ が連続* になります。
(iii) *任意の局所的に凸な空間 F について、E の点のすべての数列 $(x_n)$ が 0 になる傾向があり、数列 $(u(x_n))$ が F* で境界がある場合に限り、線形写像 $u : E \to F$ は連続です。

(iii') *任意の半正規化空間 F、線形写像 u の場合、E → F は、E のすべての有界集合 X に対して u(X) が F で有界である場合にのみ連続です。*

明らかは、準標準と凸型、平衡型、吸収性部分集合 (II、p. 20) の間の対応を考慮すると、(i) と (i') が同等であるということです。 p が E 上の準ノルムであり、各 E_A 上で連続である場合、p は E の有界部分集合で有界です。したがって、(i) は (ii) を意味します (II、p. 27、提案 5)。 (ii) が (ii') を意味することは明らかです。

ここで、(E_i, u_i)_{i \in I} を (ii') のようにし、u を E から局所的に凸な空間 F への線形写像とします。その結果、(u(x_n)) は、0 に向かう E の点のすべての数列 (x_n) に対して F 内で制限されます。 III, p. 11 の補題 1 から、 線形写像 u \circ u_i : E_i \to F は I のすべての i \ に対して連続であることがわかります。 したがって、E の位相が u_i が連続である局所的に最も細かい凸型位相である場合、u は連続です (II, p. 27、提案 5)。 これは、(ii') が (iii) を意味することを証明します。

(iii) が (iii') を意味するのは明らか (III, p. 3, cor.) 最後に、p が E の有界部分集合で有界される E 上の半ノルムである場合、条件 (iii') は恒等式写像が E から半ノルムまで連続していると主張します。 空間 (E、p);他の語では、p は連続です。これは、(iii') が (i) を意味することを証明します。

#### 定義 1 {#evt-iii-s2-def-1 .statement tag=07MA}

*局所的に凸な空間は、prop の同等の条件を満たす場合、ボルノロジカルであると言われます。 1.*

#### 例 {#evt-iii-s2-n0-exa-1 .statement tag=07MB}

— 1) すべての半正規化空間は生まれつきのものです。
2) 特に、すべての有限次元の局所的に凸な空間はボーンロジカルです。
3) 最終的な局所凸トポロジー (II, p. 28, cor. 2) の推移性を考慮して、条件 (ii') から (E_i)_{i \in I} が局所凸ボーンロジー 空間の族であり、E が最も細かい局所凸トポロジーに割り当てられている場合、とすぐに推論します。 線形写像 u_i : E_i \to E (for i \in I) が連続である位相場合、E はボーンロジーです。特に、ボーンロジカル空間の *帰納的極限、直和、商空間はボーンロジカル空間* です。

一方、ボーンロジカル空間の閉じた部分空間は、必ずしもボーンロジカルであるとは限りません (IV、p. 63、演習 8)。

#### 系 {#evt-iii-s2-n0-cor-1 .statement tag=07MC}

*すべてのハウスドルフおよび半完全地殻学的空間は、バナッハ空間の帰納的極限です。*

実際、A が閉じて有界である空間 E_A は、Banach 空間 (III, p. 8, 系) です。

#### 命題 2 {#evt-iii-s2-prop-2 .statement tag=07MD}

*局所的に凸な metrizable 空間はボーンロジカルです。*

E が計量可能であり、p が E の有界部分集合で有界される E 上の半ノルムであると仮定しますが、これは連続ではありません。 A を、$p(x) < 1$ となるようなすべての $x \in E$ の集合とします。 $(V_n)_{n \geq 1}$ を E の 0 の近傍の基本系を形成する減少列とします。p は連続ではないため、A は 0 の近傍ではありません。したがって、すべての $n > 0$ に対して、$A \not\supseteq n^{-1} V_n$ があり、$V_n$ には点 $x_n$ が存在し、$n^{-1} x_n \notin A$、つまり $p(x_n) \geq n$ になります。 数列 $(x_n)$ は 0 になる傾向があるため、有限です (III、p. 3、系)。これは矛盾する仮定ページにあります。

#### 系 {#evt-iii-s2-n0-cor-2 .statement tag=07ME}

— *すべてのフレシェ空間* (II、p. 24) * はバナハ空間* の帰納法極限です。

### 練習問題 {#evt-iii-s2-exercises}

[§ 2 に対して練習問題](exercises/s2/)を参照してください。
