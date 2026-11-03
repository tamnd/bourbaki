---
book: alg
book_title: Algebra
chapter: VII
chapter_title: MODULES OVER PRINCIPAL IDEAL DOMAINS
section: 3
section_title: Free modules over a principal ideal domain
lang: ja
source: alg-iv-vii
source_edition: 2003, Springer
book_pages: A VII.14-A VII.15, A VII.59-A VII.62
pdf_pages: 0373-0374, 0418-0421
extraction: ocr
statements: 6
exercises: 11
content_sha256: a8db741be03bbb872b1003ece2adda0a14c8af887bebaf21edc0fe95f64d5cba
translated_from: content/en/alg/VII/03_s3_free_modules_over_a_principal_ideal.md
translation_method: google
source_content_sha256: fc7f397e634b76ed9e27c6fa8e0cbf059c23e62ee408af71f36a239a6f0c2d07
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: af76762ee78c8e56daddac00b4b12f24b00e9f9a77ff19a4cc0c9c5a16f1b092
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## § 3。 自由加群主イデアル整域

#### 定理 1 {#alg-vii-s3-thm-1 .statement tag=0735}

— *$A$ のすべての左イデアルが $A$ 加群として射影 (II、p. 231、定義 1) となるように、$A$ を環とします。すると、自由な左 $A$ モジュール $L$ のすべての部分加群 $M$ は、$A$ のイデアルと同型の加群の直和になります。

$(e_i)_{i \in I}$ を $L$ の基底とし、$p_i$ をこの基底への座標写像対応するとします。 選ぶ $I$ の *整列* (*集合理論*、III、p. 153) で、$L_\alpha$ は $\alpha \leq i$ に対して $e_i$ によって生成された部分加群を表します。 $M_\alpha = M \cap L_\alpha$を入れます。 $A$ の理想的な $a_\alpha$ 上の座標写像 $p_i$ 写像 $M_\alpha$。 $a_\alpha$ は射影 $A$ 加群であるため、$M$ の (II, p. 231、提案 4) 部分加群 $N_\alpha$ が存在し、$N_\alpha$ から写像 $x \mapsto p_i(x)$ が$a_\alpha$は全単射です。 $M'_\alpha$ を、$N_\alpha$ によって$\alpha \leq i$ に対して生成された $L$ の部分加群とします。すべての $\alpha$ に対して $M'_\alpha = M_\alpha$ であることを示します。これは、$M$ がファミリー $(N_\alpha)_{\alpha < i}$ によって生成されることを意味します。 実際、すべての $\lambda < i$ に対して $M'_\lambda = M_\lambda$ を仮定します。次に $p_\lambda(x) \in a_\lambda$、すべての $x \in M_\lambda$;したがって、$x - y$ が $\alpha < \lambda$ を含む有限多元 $e_i$ の線形結合であるような $y \in N_\lambda$ が存在します。他の語 $x - y$ は $M_\alpha$ の元であり、一部の$\lambda < i$ です。帰納法仮定は$x - y \in M'_\lambda \subset M'_\alpha$、つまり$x \in M'_\alpha$、そして$M'_\alpha = M_\alpha$を示します。 $N_\alpha$ の和が直接的であることを示すことはまだ残っています。ここで、$a_\alpha \in N_\alpha$ を伴う線形関係 $\sum a_\alpha = 0$ が存在し、$a_\alpha$ (有限の多くは零を除くすべて) がすべて零ではないとしましょう。 $p$ を最大の添字 $\alpha$ として、$a_\alpha \neq 0$ とします。 $\lambda < \mu$の$p_\mu(a_\lambda) = 0$から、$p_\mu(a_\mu) = p_\mu\left( \sum a_\alpha \right) = 0$があるので、$a_\mu = 0$となり、$p$の選択と矛盾します。

#### 系 1 {#alg-vii-s3-thm-1-cor-1 .statement tag=0736}

— *$A$ のすべての左イデアルが射影である場合、射影左 $A$ モジュールのすべての部分加群は射影です。*

実際、すべての射影 $A$ 加群は自由な $A$ 加群の部分加群 (II、p. 231、提案 4)、そして Th. 1が該当します。

#### 系 2 {#alg-vii-s3-thm-1-cor-2 .statement tag=0737}

— *主イデアル整域を超える自由加群のすべての部分加群は無料です。*
    これは Th からすぐに続きます。 1、主イデアル整域のあらゆる理想は自由であるため。

#### 系 3 {#alg-vii-s3-thm-1-cor-3 .statement tag=0738}

— *射影加群主イデアル整域以降はすべて無料です。*
#### 注意 {#alg-vii-s3-n0-rem-1 .statement tag=0739}

木曜日の証明 1 は、$A^{(I)}$ のすべての部分加群が直和 $\bigoplus a_i$ と同型であり、各 $a_i$ が $A$ のイデアルであることを示しています。

命題 I。 — *L が主イデアル整域 A 以上の有限階数 n の自由加群である場合、L のすべての部分加群 M は階数 $\leq n$ の自由加群になります。
    確かにMはCorによる自由加群です。 2からThまで。 1 であり、前の注意または次の補題によって階数 $\leq n$ があります。

#### 補題 1 {#alg-vii-s3-lem-1 .statement tag=073A}

— *L を、n 元によって生成された可換環 A 上の加群とし、M を L の自由な部分加群とする。すると、M は階数 $\leq n$ になります。*
    まず、L が無料であると仮定します。 M の標準単射を L と表します。 By III, p. 520, Cor., 準同型 $\bigwedge^n i : \bigwedge^n M \to \bigwedge^n L$ は単射法です。 III、p. 511、提案 6、$\bigwedge^n L = \{0\}$ により、$\bigwedge^n M = \{0\}$; M は階数 $\leq n$ (III, p. 518, Cor. 1) を持つことになります。ここで一般的なケースを考えてみましょう。 加群 L は、階数 n の自由加群 L の商です。 M と同型の L の部分加群 M' が存在します (II, p. 218, 提案 21)。引数 M' の最初の部分までに階数 $\leq n$ があり、結果は次のようになります。

#### 系 {#alg-vii-s3-n0-cor-1 .statement tag=073B}

— *E を主イデアル整域 A よりも加群とし、n 元によって生成されます。その場合、E の任意の部分加群 F は、最大でも n 元によって生成できます。*
    確かに、$A^n$ から E (II, p. 216, Cor. 3) への準同型 f が存在し、階数 $m \leq n$ の自由加群である$f^{-1}(F)$ は n 元によって生成されます。そのうち像元 f 生成する F の下にあります。

### 練習問題 {#alg-vii-s3-exercises}

[§ 3 に対して練習問題](exercises/s3/)を参照してください。
