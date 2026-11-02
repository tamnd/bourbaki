---
book: ens
book_title: Theory of Sets
chapter: ER
chapter_title: SUMMARY OF RESULTS
section: 8
section_title: Scales of sets. Structures
lang: ja
source: ens-i-iv
source_edition: 2004, Springer
book_pages: 383-385
pdf_pages: 0388-0390
extraction: ocr
statements: 0
exercises: 0
content_sha256: 8f20ed78ca6efb505895250207b77f54f8410824ebff9911831bedd72863c504
translated_from: content/en/ens/ER/08_s8_scales_of_sets_structures.md
translation_method: google
source_content_sha256: 1729e7f56fb13a5cfb4b19ed30304bcfc4d735d7f99cdf7c9579aa41117e6f82
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-b071ad41
glossary_version: 34
glossary_terms_sha256: 60386d77a165a6f2fbcb5acabe5c9fe55fa73fe483b6346db59fbe0fdcef6a43
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## 8. 集合のスケール。 構造

1. たとえば、3 つの*異なる* 集合 E、F、G が与えられると、部分集合の集合を取得するか、それらの 1 つだけで積を形成するか、または特定の順序で取得された 2 つの積を形成することによって、それらから他の形他の集合を得ることができます。 このようにして、*12* 個の新しい集合を取得します。 これらを元の 3 つの集合 E、F、G に追加すると、既に得られた集合を与えるものを省略して、これら 15 の集合で同じ演算を繰り返すことができます。等々。 一般に、この手順 (明示的なスキームに従って) で得られる集合のいずれか 1 つは、E、F、G で * 基底* として集合* の * スケールに属すると言われます。

たとえば、M、N、P をこのスケールの 3 つの集合とし、$R\{x,y,z\}$ をそれぞれ M、N、P の一般的な元 $x$、$y$、$z$ の間の *関係* とします。次に、R $M \times N \times P$ の定義する部分集合、したがって (正規の対応を介して) $(M \times N) \times P$ の部分集合、つまり $\mathfrak{P}((M \times N) \times P)$ の元になります。したがって、同じスケールで複数の集合の元の間に *関係* を与えることは、同じスケールで他の集合の *元* を与えることと同じです。同様に、たとえば、M の写像を N に与えると、(この写像のグラフを考慮すると) $M \times N$ の部分集合、つまり $\mathfrak{P}(M \times N)$ の元が与えられることになり、これもスケールでは集合になります。最後に、(たとえば) M の 2 つの元を与えることは、積集合 $M \times M$ で 1 つの元を与えることと同じになります。

したがって、スケール内の集合の元の特定の数、これら集合の一般的な元の間の関係、およびこれらの集合の特定の部分集合の写像が他のものに与えられると、すべては最終的な分析で*単一が与えられることに帰着します。スケールの集合の 1 つである元*。

2. 先ほど (§6) で、E に (a) $C \circ C \subset C$ と (b) のプロパティがある場合、集合 $\mathfrak{P}(E \times E)$ 定義する順序構造の元 C が成り立つと言いました。

$$C \cap C^{-1} = \Delta.$$

一般に、集合 M を集合のスケールで考えます。その基底は、例のために、3 つの集合 E、F、G で構成されます。 M の一般的な元の明示的に指定されたプロパティの特定の数を与え、T をこれらのプロパティによって定義される M の部分集合の共通部分とします。 T の元 $\sigma$ は、E、F、G の *種* T の定義する *構造* と言われています。 したがって、種 T の構造は、E、F、G から M を形成するスキームと、これら構造の *公理* と呼ばれる T を定義する特性によって特徴付けられます。 同じ種のすべての構造に特定の名前を付けます。 命題「$\sigma \in T$」(つまり、T を定義する公理)の帰結であるすべての命題は、種 T の構造の *理論* に対して属するであると言われます。たとえば、構造の順序集合の§ 6属するから理論に命題が記載されています。

最後の例では、完全に任意の基底集合 E に対して公理を記述することができます。 したがって、これらの公理が定義されている集合とは無関係に、これらの公理が満たすである構造に同じ名前を付けます。これらの公理から推定される命題は、どの集合でも有効です。なぜなら、それらの定式化には集合 E の特別な性質が含まれていないからです。そのような注意は、公理がこの性質の [^1] である場合には常に当てはまります。

ほとんどの場合、スケールがいくつかの集合 E、F、G のうちの基底からなるで使用される場合、これらの集合の 1 つ、たとえば E が検討中の構造で重要な役割を果たします。したがって、言葉の乱用により、これらの構造は集合Eで定義され、FとGは補助的な集合とみなされると言われています。

最後に、言語を簡単にするために、明確な種の構造を備えた集合には特定の名前が付けられることがよくあります。したがって、私たちは*順序付き集合*について話し、この系列の後の部分では、*群、環、体、トポロジカル空間、均一空間*などの定義する概念になります。 語は、集合に特定の構造が与えられていることを示します。

3. 同じ種 T の構造を考えます。ここで、T は集合のスケールで集合 M の部分集合です。新しい「公理」を、こうして得られた公理の定義する T, 系 T に含まれる M の定義する部分集合 U に隣接させると、種 U の構造は、種 T の構造より *豊かであると言われます。たとえば、*合計の構造順序* 集合は、順序集合の構造より豊かです。なぜなら、$\mathfrak{P}(E \times E)$ の元 C は、構造の定義するが追加の公理満たすでなければならないからです。

$$C \cup \overline{C}^{-1} = E \times E.$$

4. M、M' を同じスケールの 2 つの集合とします。たとえば、E、F、G を基底とします。 T を M の部分集合 、T' を M' の部分集合とし、それぞれ特定の明示的に述べられた公理によって定義されます。 T′ に対する T の *1 対 1 写像* を明示的に定義するできるときは常に、この写像の下で相互に対応するである 2 つの元 $\sigma \in T$、$\sigma' \in T'$ を、E、F、G 上で *同じ構造* を定義するとみなします。 系の公理のうち、定義する T と T' は *等価* であると言われています。

*トポロジー 構造* は、この状況の例を提供します。それらはいくつかの等価な公理系を使って定義できますが、そのうちの 2 つ系が特に便利です (*一般位相*、章 I, § 1 を参照)。

5. E、F、G を 3 つの集合とし、E、F、G の*全単射* 写像がそれぞれ他の 3 つの集合 E'、F'、G' に与えられると仮定します。 Since we know how to define the *canonical extensions* of bijective mappings to sets of subsets (§ 2, no. 9) and to product sets (§ 3, no. 14), we can define, step by step, the *extension* of the given bijections to two sets M, M′ constructed respectively according to the *same scheme* in the scale of sets based on E, F, G, and that based on E′, F′, G′. $f$ を、こうして得られた M' 上の M の全単射とします。 $\sigma$ が M の部分集合 T の元である E、F、G 上の構造である場合、$f(\sigma)$ は、E の与えられた全単射によって、構造 $\sigma$ を E′, F′, G′ に*輸送*することによって得られる構造であると言います。 E'、F の上に F、G' の上に G。 E、F、G の構造 $\sigma$ に関連するすべての命題は、(適切な拡大を使用して) E'、F'、G' の構造 $f(\sigma)$ に関連する命題を生じます。

逆に、E、F、G 上の構造 $\sigma$ と E'、F'、G' 上の構造 $\sigma'$ は、E、F、G の全単射によって $\sigma$ をそれぞれ E'、F'、G' に *輸送*することによって $\sigma'$ が得られる場合、 *同型* であると言われます。これらの写像は、$\sigma'$ 上に $\sigma$ の *同型* を構成するといわれています。

単一の集合 E 上の構造、E 上の E 全単射、輸送 $\sigma$ から$\sigma'$ は、構造 $\sigma$ を備えた集合 E の *同型とも呼ばれます。 集合 E'、構造 $\sigma'$ に恵まれています。*

この写像は、F と G が 2 つの補助集合である場合、*同型* とも呼ばれ、これら 2 つの集合が F と G 自体に対する *同一性* 写像であるため、全単射とも呼ばれます。

集合 E の *同型* に構造 $\sigma$ が付与されたものは、*自己同型* と呼ばれます。

構造 $\sigma$ を備えた集合 E の *同型* が、構造 $\sigma'$ を備えた集合 E' 上に存在する場合、*同一視する* E に E' を付ける、つまり *同じ名前* を付けると便利な場合がよくあります。 E に基づくスケールの集合 M の元と、$f$ から集合 M の適切な拡大の下でその像である元まで。

6. 集合のスケールで集合 M の部分集合 T を定義する公理の系が与えられた場合、前にこれらの公理が満たすどれである構造について言えば、集合 T が *必ずしも空ではない* ことを確認する必要があります。そうでなければ、公理は *矛盾している * または *矛盾している * と言われるでしょう。

7. 集合で構造を定義する公理の系が任意の集合に対して記述できる場合がありますが、これらの 2 つの構造満たすの公理を考慮し、2 つの異なる集合 E、F で定義すると、公理から次のことがわかります。 構造 (それらが存在する場合) は必然的に *同型* (これは特に E と F が *等価* であることを意味します)。 次に、構造満たすの理論は *一価* であると言われます。それ以外の場合、それらは *多価* であると言われます。

The theory of integers, the theory of real numbers, and classical Euclidean geometry are univalent theories; the theory of ordered sets, group theory, and topology are multivalent theories. 多価理論の研究は、現代数学を古典数学から区別する最も顕著な特徴です。

[^1]: The reader may have observed that the indications given here are left rather vague; they are not intended to be other than heuristic, and indeed it seems scarcely possible to state general and precise definitions for structures outside of the framework of formal mathematics (see Chapter IV).
