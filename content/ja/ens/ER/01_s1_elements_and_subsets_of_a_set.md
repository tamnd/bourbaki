---
book: ens
book_title: Theory of Sets
chapter: ER
chapter_title: SUMMARY OF RESULTS
section: 1
section_title: Elements and subsets of a set
lang: ja
source: ens-i-iv
source_edition: 2004, Springer
book_pages: 347-351
pdf_pages: 0352-0356
extraction: ocr
statements: 0
exercises: 0
content_sha256: 826cd97e705df3c6c8f136fba2bedbb1185300db98a5364f5b15d06003197d28
translated_from: content/en/ens/ER/01_s1_elements_and_subsets_of_a_set.md
translation_method: google
source_content_sha256: 0e243e5f12383731f0a5a2c71334e71b3cefa638eb23c7b52b81096a04bed198
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-b071ad41
glossary_version: 34
glossary_terms_sha256: 813b8d64073a0e7ebf52d89b4cc367c058e47f630c11635d0fcf4a03abf90215
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## 1. 集合の元と部分集合

1. *集合* は *元* で構成されており、これらは特定の *プロパティ* を所有することができ、それらの間で、または他の集合の元と特定の *関係* を持つことができます。

2. 集合と元は、数学的引数において図記号によって表されます。これらの記号は、一般に (さまざまなアルファベットの) 文字、または文字と他の記号の組み合わせです。 1 つ以上の集合の元の間の関係は、[^1] と考えられる関係のスキーム特性にこれらの元を示す記号を挿入することによって示されます。プロパティについても同様です。

文字は、*固定* 元または *任意* 元 (*変数*、*引数*、または *ジェネリック* 元とも呼ばれます) 集合のいずれかを表す場合があります。 関係 (または性質) において、任意の元が固定元に置き換えられるとき、任意の元には、この固定元が *値* として与えられると言われます。

順序では、明示的に記載されていない関係に現れる元を示すために、関係を$\mathrm{R}\{x, y, z\}$のように記法で表します（$x, y, z$が元の場合）。

3. 関係または性質のうち、任意の元特徴 [^2] が、これらの任意の元に与えられる値が真の命題になる場合、*同一性* であると言われます。 R と S が 2 つの関係 (またはプロパティ) を表す場合、これらの関係に入る任意の元が R が真となるように固定されるときはいつでも、S が真の場合、R は S を *暗黙* していると言われます。 関係 (またはプロパティ) R と S は、それぞれが他方を暗示する場合、*同等*であると言われます。

4. 変数 $x$、$y$、$z$ の間で $\mathrm{R}\{x,\ y,\ z\}$ を関係とします。 The phrase "for all $x$, $\mathrm{R}\{x,\ y,\ z\}$" is a relation *between $y$ and $z$*, which will be considered to be true for a system of given values of these latter variables if R is true for these values of $y$ and $z$ and *every* value of $x$. 「$\mathrm{R}\{x,\ y,\ z\}$ となるような $x$ が存在する」 (または「一部の $x$、$\mathrm{R}\{x,\ y,\ z\}$ については」) は、再び $y$ と $z$ の間に関係があり、これは、$y$ の指定された値の系に当てはまると見なされます。 $z$ の場合、これらの変数がこのように固定されている場合、R が真である $x$ のうち *少なくとも 1 つ* の値が存在します。 変数の任意の数の間の関係についても同様です。

$\overline{\mathrm{R}}$ が R の *否定 * を表す場合、「すべての $x$ に対して、R」の否定は「$\overline{\mathrm{R}}$ となるような $x$ が存在する」になります。 「R が「すべての $x$、$\overline{\mathrm{R}}$ に対して」であるような $x$ が存在する」の否定。

5. R、S が 2 つの関係を表す場合、「R と S」を *単一* の関係とみなし、R * と * S の *両方* が true である場合は常に true とみなされます。同様に、「R また​​は S」は関係であり、これは関係 R、S の *少なくとも 1 つ* が真であるときは常に真であると見なされます (特に、両方が真であるときは常にです。したがって、ここでは語 「または」には、通常の音声でときどきが持つような選言的な意味はありません)。 $\overline{\mathrm{R}}$、$\overline{\mathrm{S}}$ がそれぞれ R、S の否定を表すものとします。すると、「R と S」の否定は「$\overline{\mathrm{R}}$ または $\overline{\mathrm{S}}$」となり、「R また​​は S」の否定は「$\overline{\mathrm{R}}$ と $\overline{\mathrm{S}}$」となります。

6. 記号「$=$」（「等しい」と読みます）の両側に 2 つの記号を 1 つずつ書くと、*等式* の関係と呼ばれる関係が得られます。これは、2 つの記号が *同じ* 元を表すことを意味します。この関係の否定は、記号「$\neq$」の両側に同じ記号を1つずつ書くことで得られます（「等しくない」または「とは異なります」と読みます）。

7. 集合 E と E の一般的な元の *性質* が与えられると、この性質形を持つ E の元は、E の *部分集合* と呼ばれる新しい集合となります。 2 つの *同等* なプロパティであるため、 定義する *同じ* Eの部分集合、そしてその逆。

AをEの部分集合とします。$x$がEの一般的な元であるとき、性質「Aに対する$x$属する」（つまり、「$x$はAの元である」）は「$x \in A$」と書かれます。この性質を持つ元の集合は明らかに単なるAです。

この性質の否定は「$x \notin A$」と書かれます (「$x$ は A に対して属するを行わない」と読みます)。この性質を持つEの元の集合はAの*補数*と呼ばれ、$\complement A$または$E - A$と書きます。

8. 一部のプロパティ (例えば、$x = x$) は、E の *すべて* 元に当てはまります。そのようなプロパティ 2 つは同等であり、部分集合それらの定義するは集合 E そのものです。

一方、一部のプロパティ (例: $x \neq x$) は、E の *任意の* 元には当てはまりません。繰り返しになりますが、任意の 2 つのプロパティは同等であり、部分集合定義するは E の *空の部分集合* と呼ばれ、$\emptyset$ で示されます。

E と $\emptyset$ はお互いの*補数*であることに注意してください。

9. $a$ を E の決定的な元とします。一部のプロパティ、たとえば $x = a$ は *単一* 元 $a$ に対してのみ真です。このような 2 つのプロパティは同等です。 部分集合彼ら定義するは$\{a\}$で表され、単独*の部分集合*からなると呼ばれます。

10. 元がすべて集合 E の *部分集合* である集合は、E の部分集合* の *集合と呼ばれ、$\mathfrak{P}(E)$ で表されます。 $x \in E$ には、$\emptyset \in \mathfrak{P}(E)$、$E \in \mathfrak{P}(E)$、$\{x\} \in \mathfrak{P}(E)$ がございます。 $x$がEの総称元、Xが$\mathfrak{P}(E)$の総称元を表す場合、$x$とXの間の関係「$x \in X$」はメンバーシップ*の*関係と呼ばれます。

11. $x$ と $y$ を E の 2 つの元とし、X を $\mathfrak{P}(E)$ の一般的な元とします。すると、等式「$x = y$」の関係は、関係「$x \in X$となるようなすべてのXに対して、$y \in X$が得られる」と *等価* になります。

12. X, Y を集合 E の 2 つの部分集合とします。 性質 $x \in X$ が性質 $x \in Y$ を暗示し、他の語 X 属するのすべての元が Y に含まれる場合、X は Y に *含まれる*、または Y *含む* であると言います。 X、またはその X * は * Y の部分集合です。 このXとYの間の関係を*包含*(YのX)の関係と呼び、「$X \subset Y$」または「$Y \supset X$」で表されます。 その否定は「$X \not\subset Y$」または「$Y \not\supset X$」で表されます。

E のすべての部分集合 X に対して、$\emptyset \subset X$ と $X \subset E$ が得られます。メンバーシップ「$x \in X$」の関係は「$\{x\} \subset X$」に相当します。

関係 「$X \subset Y$ と $Y \subset Z$」は「$X \subset Z$」を意味します。

関係 「$X \subset Y$」は「$X = Y$」の可能性を排除するものではありません。 関係「$X \subset Y$と$Y \subset X$」は「$X = Y$」と同等です。

13. X と Y を E の任意の 2 つの部分集合とします。性質 「$x \in X$ または $x \in Y$」を持つすべての元のうち集合は$X \cup Y$ で示され、X と Y の *和集合* と呼ばれます。 性質「$x \in X$と$x \in Y$」を持つ元すべての集合は$X \cap Y$で表され、XとYの*共通部分*と呼ばれます。

E のいくつかの部分集合の和集合と共通部分も同様に定義されます。

$x$、$y$、$z$がEの3つの元である場合、和集合$\{x\} \cup \{y\} \cup \{z\}$は$\{x, y, z\}$で表されます。 (個別に命名) 元の任意の数についても同様です。

X と Y を E の 2 つの部分集合とします。 $X \cap Y \neq \emptyset$ または $X \cap Y = \emptyset$ に従って、X と Y は *交差* するか、*互いに素* であると言います。

14. 以下の命題、X、Y、Z の主張は、同じ集合 E のいずれかの部分集合を表します。

(a) $\emptyset = \complement E$、$\quad E = \complement \emptyset$ があります。

(b) X 全員にとって、私たちは

(1)
$$\complement(\complement X) = X;$$

(2)
$$X \cup X = X, \qquad X \cap X = X;$$

(3)
$$X \cup (\complement X) = E, \qquad X \cap (\complement X) = \emptyset;$$

(4)
$$X \cup \emptyset = X, \qquad X \cap E = X;$$

(5)
$$X \cup E = E, \qquad X \cap \emptyset = \emptyset.$$

(c) すべての X について、Y は次のとおりです。

(6)
$$X \cup Y = Y \cup X, \qquad X \cap Y = Y \cap X \quad \text{(commutativity)};$$

(7)
$$X \subset X \cup Y, \qquad X \cap Y \subset X;$$

(8)
$$\complement(X \cup Y) = (\complement X) \cap (\complement Y), \qquad \complement(X \cap Y) = (\complement X) \cup (\complement Y).$$

(d) 関係 $X \subset Y$、$\complement X \supset \complement Y$、$X \cup Y = Y$、$X \cap Y = X$ は *同等* です。

(e) 関係 $X \cap Y = \emptyset$、$X \subset \complement Y$、$Y \subset \complement X$ は *同等* です。

(f) 関係 $X \cup Y = E$、$\complement X \subset Y$、$\complement Y \subset X$ は *同等* です。

(g) すべての X、Y、Z について、

(9)
$$\left.\begin{array}{l} X \cup (Y \cup Z) = (X \cup Y) \cup Z = X \cup Y \cup Z \\ X \cap (Y \cap Z) = (X \cap Y) \cap Z = X \cap Y \cap Z \end{array}\right\} \quad \text{(associativity)};$$

(10)
$$\left.\begin{array}{l} X \cup (Y \cap Z) = (X \cup Y) \cap (X \cup Z) \\ X \cap (Y \cup Z) = (X \cap Y) \cup (X \cap Z) \end{array}\right\} \quad \text{(distributivity)}.$$

(h) 関係「$X \subset Y$」は関係「$X \cup Z \subset Y \cup Z$」と「$X \cap Z \subset Y \cap Z$」を意味します。

(i) 関係「$Z \subset X$と$Z \subset Y$」は「$Z \subset X \cap Y$」と同等です。 関係「$X \subset Z$と$Y \subset Z$」は「$X \cup Y \subset Z$」と同等です。

15. 恒等式 (8) から、結論するは、E の部分集合 A が他の部分集合 X, Y, Z から E の適用 *のみ* 演算 $\complement$, $\cup$, $\cap$ (任意の順序) の場合、補数 $\complement A$ は、置き換えること部分集合 X、Y、Z はそれぞれの補数によって、演算 $\cup$、$\cap$ はそれぞれ $\cap$、$\cup$ を維持しながら取得できます。 演算中順序。これが*二元性の法則*です。上記の形の部分集合の間に等式 $A = B$ がある場合、同等の等式 $\complement A = \complement B$ を考えてください。双対則適用で得られる式で置き換える $\complement A$ と $\complement B$ を計算し、X、Y、Z でそれぞれ置き換える $\complement X$、$\complement Y$、$\complement Z$ を計算し、その逆を行うと、次のようになります。 等式は$A = B$の*デュアル*と呼ばれます。包含物関係 $A \subset B$ についても同じことができますが、その場合、記号「 $\subset$ 」と「 $\supset$ 」の置き換えるに注意する必要があります。

同じ数を持つ上記のアイデンティティは、互いに二重です。

16. 特定の質問では、集合 E の固定部分集合 A を考慮する必要があります。X が E の任意の部分集合である場合、集合 $A \cap X$ は A 上の X の *トレース* と呼ばれ、ときどきは次のように表されます。 $X_A$;この場合、A の部分集合と見なされます。E のすべての部分集合 X、Y について、次のようになります。

$$(X \cup Y)_A = X_A \cup Y_A, \qquad (X \cap Y)_A = X_A \cap Y_A,$$

そして
$$\complement_A X_A = (\complement_E X)_A,$$

ここで、$\complement_E X$ は E の X の補数を示し、$\complement_A X_A$ は A の $X_A$ の補数を示します。

$\mathfrak{S}$ が E の部分集合の集合を表す場合、$\mathfrak{S}$ の集合の A 上のトレースの集合 $\mathfrak{S}_A$ は、A の $\mathfrak{S}$ の *トレース* と呼ばれます。

[^1]: 元を表す記号が複数の記号の組み合わせであり、単一の文字の代わりに関係に挿入される場合、混乱を避けるため、順序の括弧で囲むのが通例です。
[^2]: 集合 E の一般的な* 元の *性質について話すとき、これは決して E の *すべての* 元に対して性質が真であることを意味するのではなく、単に E の *すべての * 元に対して *意味がある* ということを強調する必要があります。これらの元の一部については true かもしれませんが、他のものについては false かもしれません。 関係も同様です。
