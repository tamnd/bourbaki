---
book: ens
book_title: Theory of Sets
chapter: III
chapter_title: ORDERED SETS, CARDINALS, INTEGERS
section: 0
section_title: Historical Note
kind: historical
lang: ja
source: ens-i-iv
source_edition: 2004, Springer
book_pages: 255-257
pdf_pages: 0261-0263
extraction: ocr
statements: 0
exercises: 0
content_sha256: c1d51060e7619aa8d9e477f8785087446efc15824b78865bbacf9e9a650094ef
translated_from: content/en/ens/III/historical_note.md
translation_method: google
source_content_sha256: 35c7fafb7fcf59df7cdf3b82fc528a165d03d9d6a7897b9d7068e48d10fcf9a5
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-b071ad41
glossary_version: 34
glossary_terms_sha256: 2bd8d74febc7a7a8ab74592c24777105ec2c416fc2ddd097b470372bd0957c6f
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

# 歴史注意

(章 III, § 5)

(括弧内の数は参考文献を参照します
この注意の最後にあります。)

The evolution of ideas relating to the notions of integer and cardinal number is inseparable from the history of the theory of sets and mathematical logic for which the reader is referred to the Historical Note following Chapter IV. この注意の目的は、数え上げと「組み合わせ分析」の歴史における顕著な事実のいくつかを簡単に示すことです。

歴史と考古学は、「数え方の系」の大きな数を私たちに明らかにしました。その主な目的は、各個人整数（実際の使用の要求に応じて極限まで）に名前と、多かれ少なかれ規則的な法則に従って制限された記号の数から形成される書かれた表現を付けることです。 これまでのところ、最も複雑な共通の手順は、整数を「連続する単位元」$b_1$、$b_2$、...、$b_n$、...の和に分解することであり、それぞれは前任者の倍数の整数です。また、一般に $b_n/b_{n-1}$ は固定の数 $b$ (系の「基底」、通常は 10) とみなされますが、この規則には多くの既知の例外があります。 たとえば、バビロニアの系では、$b_n/b_{n-1}$はときどき10とときどき6 [1]、マヤの年代記系では、$n = 2$と$b_2/b_1 = 18$を除いて$b_n/b_{n-1}$は20に等しい[2]。 対応するの表記記号は、「単位元」の数、順序$i$のそれぞれの$b_i$を示す必要があります。 多くの系 (エジプト、ギリシャ、ローマなど) では、連続する倍数 $k.b_i$ ($k$ は 1 から $(b_{i+1}/b_i) - 1$ まで変化します) は、$k$ と $i$ の両方に依存する記号で表されます。 最初の重要な前進は、すべての数 $k.b_i$ ($k$ の同じ値について) を同じ記号で表すことでした。これが「位置による数え方」の原則であり、添字 $i$ は、$k.b_i$ を表す記号が「$i$ 番目に現れる」という事実によって示されます。場所」。 この性質の最初の系はバビロニア人のもので、確かに紀元前 2000 年頃のバビロニア人です。 C は、すべての倍数 $k.60^{\pm i}$ 対応するからさまざまな値の指数 $i$ まで同じ記号で示されていました ([1]、pp. 93-109）。 このような系の不便さは、もちろん、ある順序の単位元が存在しないかどうかを示すものが何もない限り、つまり系が「零」の導入によって完成しない限り、その曖昧さです。 それにもかかわらず、バビロニア人はその歴史のより大きな部分の間、そのような記号なしで管理し、紀元前Cの最後の2世紀を除いて「零」を使用せず、その後は数の内側でのみ使用しました。それまでは、文脈だけで検討中のシンボルの意味を明確にすることができました。 他の 2 つの系だけが「零」を体系的に使用していました。マヤ族のそれ (明らかにキリスト教時代の初めから使用されている [2]) と、私たちの現在の十進数系は、(アラブ人経由で) ヒンズー教の数学に由来しており、そこでは零の使用が西暦 1 世紀から証明されています。 さらに、零を数として (単なる区切り記号としてではなく) と計算への導入は、ヒンドゥー教徒の独自の貢献です [3]。 もちろん、「位置による数値化」の原則を一度習得すれば、それを任意の基底に拡大するすることは簡単です。 17 世紀以来提案されてきたさまざまな「基底」の利点に関する議論は数値計算の技術に依存しており、できないについてはここで説明します。 これらの系の根にある演算、いわゆる「ユークリッド除算」は、ギリシャ人の時代には前に登場しておらず、間違いなく初期のピタゴラス学派に遡り、彼らはそれを理論的算術の重要なツールとしたことに注意してください。

The general problems of enumeration, grouped together under the name of “combinatorial analysis”, seem not to have been attempted before the last centuries of classical antiquity; only the formula $\binom{n}{2}=\frac{1}{2}n(n-1)$ is attested, in the third century A.D. ヒンドゥー教の数学者バスカラ (12 世紀) は、$\binom{n}{p}$ に対する一般的な公式を知っていました。 より体系的な研究は、レヴィ・ベン・ゲルソンの写本（13世紀初頭）に見られます。彼は、一度に$n$のオブジェクト$p$の配置の数$V_n^p$、特に$n$のオブジェクトの置換の数について帰納的公式を得ました。彼は、関係 $\binom{n}{p}=V_n^p/p!$ および $\binom{n}{p}=\binom{n}{n-p}$ に相当する規則を述べました ([4]、64-65 ページ)。 しかし、この原稿は同時代人には知られていなかったようで、結果はその後数世紀に数学者によって徐々に再発見されただけでした。 As regards later progress, let us record that Cardan proved that the number of non-empty subsets of a set of $n$ elements is $2^n-1$. パスカルとフェルマーは確率の計算を確立する際に$\binom{n}{p}$の表現を再発見し、パスカルはこれらの数と二項定理の間の関係を最初に観察した。これは13世紀以来アラブ人に知られ、14世紀には中国人に知られていたようで、当初は西洋で再発見されたものである。これは、「パスカルの三角形」として知られる係数の帰納的計算方法とともに ([4]、pp. 35-38) です。 最後に、1676 年頃、ライプニッツは「多項式係数」の一般公式を取得しました (ただし出版はしませんでした)。これは独立して再発見され、20 年後にド モアブルによって出版されました。

# 参考文献

1. O. NEUGEBAUER, *Vorlesungen über die Geschichte der antiken Mathematik*, Bd. I : Vorgriechische Mathematik, Berlin (Springer), 1934.
2. S. G. MORLEY, *The Ancient Maya*, Stanford University Press, 1946.
3. B. DATTA and A. N. SINGH, *History of Hindu Mathematics*, vol. I, Lahore (Motilal Banarsi Das), 1935.
4. J. TROPFKE, *Geschichte der Elementar-Mathematik*, vol. VI : Analysis, Analytische Geometrie, Berlin-Leipzig (de Gruyter), 1924.
