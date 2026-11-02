---
book: ens
book_title: Theory of Sets
chapter: III
chapter_title: ORDERED SETS, CARDINALS, INTEGERS
section: 5
section_title: Properties of integers
lang: ja
source: ens-i-iv
source_edition: 2004, Springer
book_pages: 171-183, 235-240
pdf_pages: 0177-0189, 0241-0246
extraction: ocr
subsections:
    - "no": 1
      title: OPERATIONS ON INTEGERS AND FINITE SETS
      page: 171
      pdf_page: 177
    - "no": 2
      title: STRICT INEQUALITIES BETWEEN INTEGERS
      page: 173
      pdf_page: 179
    - "no": 3
      title: INTERVALS IN SETS OF INTEGERS
      page: 174
      pdf_page: 180
    - "no": 4
      title: FINITE SEQUENCES
      page: 175
      pdf_page: 181
    - "no": 5
      title: CHARACTERISTIC FUNCTIONS OF SETS
      page: 175
      pdf_page: 181
    - "no": 6
      title: EUCLIDEAN DIVISION
      page: 176
      pdf_page: 182
    - "no": 7
      title: EXPANSION TO BASE $b$
      page: 177
      pdf_page: 183
    - "no": 8
      title: COMBINATORIAL ANALYSIS
      page: 179
      pdf_page: 185
statements: 30
exercises: 18
content_sha256: bca8e465ae727941445d08e4becac7537cf42011ff0a6ac81efd279e0d41a518
translated_from: content/en/ens/III/05_s5_properties_of_integers.md
translation_method: google
source_content_sha256: 3be04f126cfae8abc23e921d976ad2b92ca04282828df49f6677b21e985508ca
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-b071ad41
glossary_version: 34
glossary_terms_sha256: e0d948f71fafc1780811b5d3e0a081599fd9f9ea2b172924b17d31842241f45a
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## 5. 整数の性質

### 1. 整数上の演算と有限の集合

#### 命題 1 {#ens-iii-s5-prop-1 .statement tag=03LP}

*$(a_i)_{i \in I}$を整数の有限族とする。すると、基数 $\sum_{i \in I} a_i$ と $\prod_{i \in I} a_i$ は整数になります。*

まず、$a$ と $b$ が整数である場合、$a + b$ も同様であることを示しましょう。 $b$の帰納法までに進みます。 主張は、$a + 0 = a$ 以降の $b = 0$ に当てはまります。 $a + b$ が整数であれば、$(a + b) + 1$ (§ 4, no. 1, 命題 1) も同様です。ただし、$(a + b) + 1 = a + (b + 1)$ (§ 3, no. 3、系 ～ 命題 5)。従って、$a + (b + 1)$ は整数となり、その結果、すべての整数 $b$ に対して $a + b$ は整数となります。

次に、$n = \mathrm{Card}\ (\mathrm{I})$ の帰納法によって、$\sum\limits_{i \in \mathrm{I}} a_i$ が整数であることを示します。 $n = 0$ならこれは明らかで、その後は$\mathrm{I} = \emptyset$と$\sum\limits_{i \in \mathrm{I}} a_i = 0$になります。 $\mathrm{Card}\ (\mathrm{I}) = n + 1$ の場合、$\mathrm{Card}\ (\mathrm{J}) = n$ と $k \notin \mathrm{J}$ は、$\mathrm{I} = \mathrm{J} \cup \{k\}$ と書くことができます。それから

$$\sum_{i \in \mathrm{I}} a_i = a_k + \sum_{i \in \mathrm{J}} a_i$$

($\S\,3$、no. 3、命題 5)。帰納的仮定は、$\sum\limits_{i \in \mathrm{J}} a_i$が整数であるということです。従って、証明の最初の段落の $a_k + \sum\limits_{i \in \mathrm{J}} a_i$ も同様です。これは、$\sum\limits_{i \in \mathrm{I}} a_i$ がすべての $n$ に対して整数であることを示しています。

2 つの整数 $a$ と $b$ の積 $ab$ は、整数の有限族の和なので、すべて $a$ ($\S\,3$, no. 4, 命題 6、系 2)、$ab$ は整数です。 $n = \mathrm{Card}\ (\mathrm{I})$の帰納法までに、$\prod\limits_{i \in \mathrm{I}} a_i$が整数であることを証明します。これは $n = 0$ にも当てはまります。

$$\prod_{i \in \mathrm{I}} a_i = 1.$$

$\mathrm{Card}\ (\mathrm{I}) = n + 1$ の場合、(上記と同じ記法で)

$$\prod_{i \in \mathrm{I}} a_i = a_k \cdot \prod_{i \in \mathrm{J}} a_i$$

($\S\,3$, no. 3, 命題 5) 従って、帰納法仮定は、$\prod\limits_{i \in \mathrm{I}} a_i$ が整数であることを意味します。従って、$\prod\limits_{i \in \mathrm{I}} a_i$ はすべての $n$ に対して整数になります。

#### 系 1 {#ens-iii-s5-prop-1-cor-1 .statement tag=03LQ}

*和集合* E *有限族* $(\mathrm{X}_i)_{i \in \mathrm{I}}$ *有限集合は有限集合です。*

和の場合、家族 $(\mathrm{X}_i)$ の S は有限です。そして、E 上に S の写像が存在するため (章 II, $\S\,4$, no. 8)、集合 E は有限です ($\S\,4$, no. 2, 命題 2, 系) 3)。

#### 系 2 {#ens-iii-s5-prop-1-cor-2 .statement tag=03LR}

*有限集合の有限族の積は有限集合です。*

#### 系 3 {#ens-iii-s5-prop-1-cor-3 .statement tag=03LS}

*$a$と$b$が整数の場合、$a^b$は整数となります。

なぜなら、$a^b$ は、$a$ ($\S\,3$, no. 5, 命題 10) に等しい整数の有限族の積です。

#### 系 4 {#ens-iii-s5-prop-1-cor-4 .statement tag=03LT}

有限集合* E *は有限です*の*部分集合の集合

その基数は $2^{\mathrm{Card}\ (\mathrm{E})}$ ($\S\,3$、no. 5、命題 12) です。

### 2. 整数間の厳密な不平等

#### 命題 2 {#ens-iii-s5-prop-2 .statement tag=03LU}

※$a$と$b$を2つの整数とします。次に、$b = a + c$ となるような整数 $c > 0$ が存在する場合に限り、$a < b$ となります。*

$a < b$ の場合、基数 $c \leqslant b$ が存在します (したがって、$c$ は整数 (§ 4, no. 2, 命題 2)) となり、$b = a + c$ (§ 3, no. 6, 命題 13) となります。 $a \neq b$ の場合、$c \neq 0$ が必要です。逆に、$b = a + c$ と $c \neq 0$ の場合は、$c \geqslant 1$ となり、$a < a + 1 \leqslant a + c = b$ となります。

#### 命題 3 {#ens-iii-s5-prop-3 .statement tag=03LV}

*$(a_i)_{i \in I}$ と $(b)_{i \in I}$ を、各 $i \in I$ に対して $a_i \leqslant b_i$ が、少なくとも 1 つの添字 $i$ に対して $a_i < b_i$ となるように、整数の 2 つの有限族とします。それから*

$$\sum_{i \in I} a_i < \sum_{i \in I} b_i.$$

*それぞれの $i \in I$ に対して $b_i > 0$ もある場合、*

$$\prod_{i \in I} a_i < \prod_{i \in I} b_i.$$

$j$ を $a_j < b_j$ となるように添字とし、$J = I - \{j\}$ とします。それから

$$b_j = a_j + c_j$$

$c_j > 0$ (命題 2)、したがって (§ 3, no. 6, 命題 14)

$$\sum_{i \in I} b_i = a_j + c_j + \sum_{i \in J} b_i \geqslant c_j + a_j + \sum_{i \in J} a_i = c_j + \sum_{i \in I} a_i.$$

$c_j > 0$ なので、命題の最初の部分は命題 2 から続きます。

$$\prod_{i \in I} b_i = (a_j + c_j) \prod_{i \in J} b_i = a_j . \prod_{i \in J} b_i + c_j . \prod_{i \in J} b_i \geqslant \prod_{i \in I} a_i + c_j . \prod_{i \in J} b_i.$$

$c_j$ とすべての $b_i$ は $\neq 0$ であるため、積 $c_j . \prod_{i \in J} b_i$ は $\neq 0$ (§ 3, no. 4, 命題 7) です。したがって、命題の 2 番目の部分です。

#### 系 1 {#ens-iii-s5-prop-3-cor-1 .statement tag=03LW}

*$a$、$a'$、$b$を整数とし、$a < a'$と$b > 0$とします。次に、$a^b < {a'}^b$.*

$a^b$ と ${a'}^b$ を、整数 (§ 3, no. 5, 命題 10) と命題を適用する 3, 観察するとの有限族の積として表現するだけで済みます。これは、関係 $a < a'$ が意味することです。 $a' > 0$。

#### 系 2 {#ens-iii-s5-prop-3-cor-2 .statement tag=03LX}

*$a$、$b$、$b'$ を整数として、$a > 1$ と $b < b'$ とします。次に $a^b < a^{b'}$.*

なぜなら、$b' = b + c$ (命題 2) となるような整数 $c > 0$ が存在するからです。 $c \geqslant 1$ から、$a^c \geqslant a > 1$、よって $a^{b'} = a^b a^c > a^b$ になります。

#### 系 3 {#ens-iii-s5-prop-3-cor-3 .statement tag=03LY}

*$a$、$b$、$b'$ を整数* とします (それぞれ、$a > 0$* となる *整数)。 *その後 $a + b = a + b'$* (それぞれ *$ab = ab'$*) *$b = b'$ の場合にのみ*

#### 系 4 {#ens-iii-s5-prop-3-cor-4 .statement tag=03LZ}

*$a$ と $b$ が $a \leqslant b$ となるような整数である場合、 $b = a + c$ となるような一意の整数 $c$ が存在します。

$c$ の存在は、§ 3, no. 6 の命題 13 から続き、その一意性は上記の系 3 から続きます。

¶ 整数 $c$ で、$b = a + c$ ($a \leqslant b$) は、整数 $b$ と $a$ の *差* と呼ばれ、$b - a$ と書きます。 $a$、$b$、$a'$、$b'$ が整数で、$a \leqslant b$ と $a' \leqslant b'$ である場合、

$$(b - a) + (b' - a') = (b + b') - (a + a').$$

### 3. 整数の集合に区間

整数のすべての集合は、基数の集合であり、整然としています (§ 3, no. 2、定理 1)。さらに、整数 $a$ 関係それぞれについて、「$x$ は基数と $x \leqslant a$」は $x$ (§ 3, no. 2, 注意後で定理 1) にまとめられ、 $x$ の集合と、この関係満たすは、整数の集合 (§ 4, no. 2, 命題 2) であるため、$[0, a]$ で表すことができます。

#### 命題 4 {#ens-iii-s5-prop-4 .statement tag=03M0}

※$a$と$b$を整数とします。この場合、写像 $x \rightarrow a + x$ は、区間 $[0, b]$ から区間 $[a, a + b]$ への厳密な増分同型であり、$y \rightarrow y - a$ は逆同型です。*

明らかに関係 $0 \leqslant x \leqslant b$ は $a \leqslant a + x \leqslant a + b$ を暗示しています。 写像 $x \rightarrow a + x$ は、no. 2 の命題 3 による真に増加する (したがって単射的) です。最後に、関係 $a \leqslant y \leqslant a + b$ は、$x \geqslant 0$ と $a + x \leqslant a + b$、よって $x \leqslant b$ (no. 2、命題 3) とともに $y = a + x$ を暗示します。これで証明は完了です。

#### 命題 5 {#ens-iii-s5-prop-5 .statement tag=03M1}

*$a$ と $b$ が $a \leqslant b$ となるような整数である場合、区間 $[a, b]$ は、元の数が $b - a + 1$ である有限の集合です。

命題 4 までに、$a = 0$ の場合に限定することができます。 証明は $b$ の帰納法によるものです。 $b = 0$ の場合、結果はクリアです。 関係 $0 \leqslant x \leqslant b + 1$ は「$0 \leqslant x < b + 1$ または $x = b + 1$」に相当し、関係 $0 \leqslant x < b + 1$ は$0 \leqslant x \leqslant b$ (§ 4, no. 2、命題 2) に相当します。他の語、区間、$[0, b + 1]$は$[0, b]$と$\{b + 1\}$の和集合で、この2つの集合は互いに素です。 By the inductive hypothesis the number of elements of $[0, b + 1]$ is equal to $(b + 1) + 1$, and the Proposition is proved.

#### 命題 6 {#ens-iii-s5-prop-6 .statement tag=03M2}

*完全に順序付けされ、n 元* $(n \geqslant 1)$ を持つすべての有限集合* E * に対して、* 区間* $[1, n]$ 上に * E * の一意の同型が存在します。

E と $[1, n]$ は整列しており (§ 4, no. 4、命題 3、系 1)、元 (命題 5) の数が同じであるため、結果は § 2, no. 5 の定理 3 と系 2 から次のようになります。 命題 2/§ 4, no. 2。

### 4. 有限列

A *有限列* (それぞれ集合* E の元の *有限列) は、添字集合 I が整数の有限集合である族 (それぞれ E の元の族) です。 Iの元の数は、数列の*長さ*と呼ばれます。

$(t_i)_{i \in I}$ を長さ $n$ の有限列とします。 no. 3 の命題 6 までに、整数 I の集合に、区間 $[1, n]$ の固有の同型 $f$ が存在します。それぞれの $k \in [1, n]$、$t_{f(k)}$ は、数列* の *k 番目の項であると言われます。 $t_{f(1)}$ (それぞれ $t_{f(n)}$) は、数列の *最初* (それぞれ *最後*) *項* です。

Let $\mathrm{P}\{i\}$ be a relation such that the elements $i$ for which $\mathrm{P}\{i\}$ is true form a finite set of integers. 有限列 $(t_i)_{i \in I}$ は、多くの場合、$(t_i)_{\mathrm{P}\{i\}}$ と書かれます。 たとえば、$\mathrm{I} = [a, b]$の場合、記法 $(t_i)_{a \leqslant i \leqslant b}$がよく使われます。 同じ条件の下で、集合 $(\mathrm{X}_i)_{i \in I}$ 記法の家族の積を表します

$$\prod_{\mathrm{P}\{i\}} \mathrm{X}_i \quad \text{and} \quad \prod_{i=a}^{b} \mathrm{X}_i$$

使用されています。 和集合、共通部分、基数積、基数和、代数 \* の \* 合成法則などには記法が使用されます。

### 5. 集合の特徴写像

E を E の空でない集合および A 部分集合とします。E の部分集合 A の *特性写像* は、E の集合 $\{0, 1\}$ への E の写像 $\varphi_\mathrm{A}$ です。

$$\varphi_\mathrm{A}(x) = 1 \quad \text{if} \quad x \in \mathrm{A}; \qquad \varphi_\mathrm{A}(x) = 0 \quad \text{if} \quad x \in \mathrm{E} - \mathrm{A}.$$

¶ 明らかに、関係 $\varphi_\mathrm{A} = \varphi_\mathrm{B}$ は $\mathrm{A} = \mathrm{B}$ と同等です。すべての $x \in \mathrm{E}$ には $\varphi_\mathrm{E}(x) = 1$ があり、すべての $x \in \mathrm{E}$ には $\varphi_{\emptyset}(x) = 0$ があります。これらは E 上の唯一の一定の特性写像です。次の命題は定義の明らか帰結です。

#### 命題 7 {#ens-iii-s5-prop-7 .statement tag=03M3}

*空ではない集合* E の部分集合* A、B の各対について、*次の結果が得られます*

(1) $$\varphi_{\mathrm{E-A}}(x) = 1 - \varphi_{\mathrm{A}}(x),$$

(2) $$\varphi_{\mathrm{A} \cap \mathrm{B}}(x) = \varphi_{\mathrm{A}}(x)\varphi_{\mathrm{B}}(x),$$

(3) $$\varphi_{\mathrm{A} \cup \mathrm{B}}(x) + \varphi_{\mathrm{A} \cap \mathrm{B}}(x) = \varphi_{\mathrm{A}}(x) + \varphi_{\mathrm{B}}(x)$$

*全員に* $x \in \mathrm{E}$。

### 6. ユークリッド部門

#### 定理 1 {#ens-iii-s5-thm-1 .statement tag=03M4}

*a と b を $b > 0$ となるように整数とします。そして、$a = bq + r$と$r < b$、整数 qとrはこれら条件によって一意に決まる整数 qとrが存在します。

$q$ および $r$ の条件は、$bq \leqslant a < b(q + 1)$ および $r = a - bq$ (no. 2、命題 2) と同等です。したがって、$bq \leqslant a < b(q + 1)$ となるような $q$ を見つける必要があります。他の場合、語、$q$ は $a < b(q + 1)$ となるように最小の整数でなければならず、これは $q$ と $r = a - bq$ が一意に決定されることを示しています。それらの存在を証明するために、$a < bp$ となるような整数 $p$ が存在することに注意します。たとえば、$a + 1$ ($b > 0$ 以降)。 $m$ をこれら整数のうち最小のものとします。 $m \neq 0$ があるので、$m = q + 1$ を $q \leqslant m$ (§ 4, no. 2, 命題 2) と書くことができます。 $bq \leqslant a < b(q + 1)$ということになります。

#### 定義 1 {#ens-iii-s5-def-1 .statement tag=03M5}

※定理1の記法では、rはaをbで割った余りと呼ばれます。 $r = 0$ の場合、a は b の倍数である、または a は b で割り切れる、または b は a の因子である、または b 割る a、または b は a の因子であると言います。 数 q は b によって a の商と呼ばれ、$\dfrac{a}{b}$ または $a/b$ で表されます。*

$a$ が $b$ の倍数ではない場合、数 $q$ は a の商の * 積分部分 by b* (cf. *一般位相*、章 IV, § 8, no. 2) と呼ばれます。

*この章* で、$a/b$ または $\dfrac{a}{b}$ と書くと、$b$ 割る $a$ を意味します。

関係 $a = bq$ と $q = a/b$ は同等です ($b > 0$ の場合)。 倍数 $a$ の $b$ のすべての倍数 $a'$ は $b$ の倍数であり、

$$a'/b = (a'/a)\,(a/b) \qquad \text{if} \qquad a \neq 0.$$

また、$c$ と $d$ が $b$ の倍数である場合、$c+d$ と $c-d$ ($d\leq c$ の場合) は $b$ の倍数であり、次のようになります。

$$\frac{c+d}{b}=\frac{c}{b}+\frac{d}{b},\qquad \frac{c-d}{b}=\frac{c}{b}-\frac{d}{b}.$$

2 のうち倍数である整数は *偶数*、その他は *奇数* と言われます。 定理 1 までに、奇数の整数は形 $2n+1$ になります。

### 7. 基底 $b$ への拡張

#### 命題 8 {#ens-iii-s5-prop-8 .statement tag=03M6}

*$b$を整数$>1$とします。それぞれの整数 $k>0$ について、$E_k$ を区間の家族 $(J_h)_{0\leq h\leq k-1}$ の辞書編集上の積 (§ 2, no. 6) とし、すべて $[0,b-1]$ と同一とします。それぞれの $r=(r_0,r_1,\ldots,r_{k-1})\in E_k$ について、* しましょう

$$f_k(r)=\sum_{h=0}^{k-1}r_hb^{k-h-1};$$

*その後、写像 $f_k$ は、注文された集合 $E_k$ の同型を区間 $[0,b^k-1]$ に加えたものになります。

証明は $k$ の帰納法によるものです。 $k=1$ の場合、定義の明らか帰結です。それぞれ $r=(r_0,\ldots,r_{k-1},r_k)\in E_{k+1}$ を入れます

$$\varphi(r)=(r_0,\ldots,r_{k-1})\in E_k.$$

すると、写像 $r\mapsto(\varphi(r),r_k)$ は、$E_k$ と $J=[0,b-1]$ の辞書編集上の積では、$E_{k+1}$ の同型になります。 定義の明らかです。書くかもしれません

$$f_{k+1}(r)=b\cdot f_k(\varphi(r))+r_k;$$

$E_{k+1}$ の関係 $r<r'$ が $f_{k+1}(r)<f_{k+1}(r')$ を暗示していることを示しましょう。確かに、$\varphi(r)<\varphi(r')$ か、あるいは $\varphi(r)=\varphi(r')$ と $r_k<r'_k$ のいずれかがあります。最初のケースでは、帰納的仮定は $f_k(\varphi(r))<f_k(\varphi(r'))$ を意味し、従って (§ 4, no. 2, 命題 2) $f_k(q(r'))\geq f_k(\varphi(r))+1$ を意味します。従って

$$f_{k-1}(r')\geq b\cdot f_k(\varphi(r))+b>f_{k+1}(r),$$

$r_k\leq b-1$ (no. 2, 命題 3) 以来。一方、$\varphi(r)=\varphi(r')$ と $r_k<r'_k$ であれば、$f_{k+1}(r)<f_{k+1}(r')$ であることは明らかです。ここで、帰納法仮定は、$f_k(\varphi(r))\leq b^k-1$、よってを示します。

$$f_{k+1}(r)\leq b(b^k-1)+b-1=b^{k+1}-1.$$

従って、$f_{k+1}$ は $E_{k+1}$ の同型から区間 $[0,b^{k+1}-1]$ の部分集合になります。しかし、この区間と $E_{k+1}$ は元の同じ数、つまり $b^{k+1}$ (no. 3, 命題 5) を持ちます。従って、$f_{k+1}$ は全単射 (§ 4, no. 2、命題 2、系 4) となり、証明は完了します。
¶ 整数 $a$ ごとに $a < b^a$ があることに注意してください。これは、$a$ の帰納法によって証明されます。結果は $a = 0$ で明らかであり、仮定 $a < b^a$ は $a + 1 \leqslant b^a < b \cdot b^a = b^{a+1}$ (no. 2、命題 3 および § 4, no. 2、命題 2) を意味します。従って、$a < b^k$ のような最小の整数 $k$ が存在し、命題 8 は、$0 \leqslant h \leqslant k - 1$ に対して $0 \leqslant r_h \leqslant b - 1$ となるような一意の有限列 $(r_h)_{0 \leqslant h \leqslant k-1}$ が存在することを示します。
$$a = \sum_{h=0}^{k-1} r_h b^{k-h-1}.$$
さらに、$r_0 > 0$ がなければなりません。そうでない場合は、命題により $a < b^{k-1}$ になります。 8. 式
$$\sum_{h=0}^{k-1} r_h b^{k-h-1}$$
整数 $a$ の *基底 $b$* への拡張と呼ばれます。

\* 数値計算を含まない数学のすべての部分において、命題 8 は主に *素数* 数 $b$ に適用される場合に役立ちます。 \*

整数 $b$ が実行可能なほど十分小さい場合、それぞれの整数 $< b$ を *数字* と呼ばれる固有の記号で表すことができます。 0 と 1 を表す数字は通常 0 と 1 です。$a$ を整数とし、$\sum_{h=0}^{k-1} r_h b^{k-h-1}$ をその基底 $b$ への拡張とします。この展開に現れる整数 $k$ がこれを実行できるほど十分に小さい場合、$r_0 r_1 \ldots r_{k-2} r_{k-1}$ を左から右に書いて得られる一連の記号整数 $a$ と、次に整数 $r_i$ をそれぞれ置き換えることと関連付けることが通常です。それを表す数字。このようにして取得されたシンボルは、$a$ に関連付けられた *数値シンボル* と呼ばれます。その後、項と関係に表示される数字記号により、置き換える $a$ となることがよくあります。

たとえば、C、Q、F、D が数字の場合、数値記号 CQ、CQF、CQFD はそれぞれ$\mathrm{C}b + \mathrm{Q}$、$\mathrm{C}b^2 + \mathrm{Q}b + \mathrm{F}$、$\mathrm{C}b^3 + \mathrm{Q}b^2 + \mathrm{F}b + \mathrm{D}$ に関連付けられます。

命題 8 から、整数 $a$ に関連付けられた数値記号は一意であり、$a < b^k$ の場合、含むは最大 $k$ 桁であることがわかります。 整数 $b^k$ に関連付けられた数値記号は、数字の 1 とそれに続く $k$ の数字の 0 で構成されていることに注意してください。

この表現の整数の系を基底$b$*までの数え方の*系といいます。実際の数値計算では、次の系が使用されます: (*a*) 系 ～ 基底 2、または *2 進法系* (数字は 0 と 1)。 (*b*) *10 進数系*。数字は $0$、$1$、$2$、$3$、$4$、$5 = 4 + 1$、$6 = 5 + 1$、$7 = 6 + 1$、$8 = 7 + 1$、$9 = 8 + 1$、およびここで、$b$ は整数 $9 + 1$ です (したがって、この系の数字記号は 10 です)。

中世以来、伝統的に数値計算には十進法系が使用されてきました。整数を明示的に書き留める機会がある場合は常に、この系列でそれを使用します。 数値記号によって与えられる 2 つの整数のうち商の和、差分、積、および積分部分に関連する数値記号を取得するための方法の説明については、この系列の部分を参照してください。

### 8. 組み合わせ分析

#### 命題 9 {#ens-iii-s5-prop-9 .statement tag=03M7}

*$\mathrm{E}$ *と* $\mathrm{F}$ *2 集合、* $\mathfrak{a}$ *と* $\mathfrak{b}$ *それらの基数、* $f$ *射影* $\mathrm{E}$ *上に* $\mathrm{F}$ *そのように集合* $\overset{-1}{f}(y)$、*どこ* $y \in \mathrm{F}$、*すべて同じ基数* $\mathfrak{c}$ です。 *それでは* $\mathfrak{a} = \mathfrak{b}\mathfrak{c}$。

家族の場合、$(\overset{-1}{f}(y))_{y \in \mathrm{F}}$ は $\mathrm{E}$ の分割であり、それぞれの元は分割は基数 $\mathfrak{c}$ の集合です。したがって、結果は (§ 3, no. 4、命題 6、系 2) になります。

#### 定義 2 {#ens-iii-s5-def-2 .statement tag=03M8}

*$n$ *を整数とします。* *積* $\prod_{i < n} (i + 1)$ *は* $n!$ (「階乗 $n$」と読みます) で表されます。

$0! = 1$ (章 II, § 5, no. 3) と $1! = 1$ があります。それぞれの整数 $n$ には $(n + 1)! = n!\,(n + 1)$ があります。この関係は、関係 $0! = 1$ とともに、項 $n!$ を特徴付けています。これは、$n$ の帰納法から簡単にわかります。

#### 命題 10 {#ens-iii-s5-prop-10 .statement tag=03M9}

*$m$ *および* $n$ *整数を* $m \leqslant n$のようにします。 *Then* $n!/(n - m)!$ *is the number of injective mappings of a set* $\mathrm{A}$ *with* $m$ *elements into a set* $\mathrm{B}$ *with* $n$ *elements.*

証明は、$\mathrm{A}$ の元の数 $m \leqslant n$ の帰納法までです。 $m = 0$ の場合、結果は明らかです。 $m + 1 \leqslant n$ だとします。 $\mathrm{A}$ を $m + 1$ 元で集合とし、$\mathrm{A}'$ を $m$ 元で$\mathrm{A}$ の部分集合とし、$\{a\} = \mathrm{A} - \mathrm{A}'$ とします。 $\mathrm{F}$、$\mathrm{F}'$を$\mathrm{A}$、$\mathrm{A}'$の単射詞写像の集合を$\mathrm{B}$とし、$\varphi$をそれぞれ写像の写像$f \to f\,|\mathrm{A}'$とする写像 $f \in \mathrm{F}$ から制限から $\mathrm{A}'$ まで。 $\overset{-1}{\varphi}(f')$ の各 $f' \in \mathrm{F}'$ 元 $f$ は、その値 $f(a)$ によって一意に決定されます。 $f$ は単射なので、$f(a) \in \mathrm{B} - f'(\mathrm{A}')$ でなければなりません。従って、$\overset{-1}{\varphi}(f')$ は元の $\mathrm{B} - f'(\mathrm{A}')$ と同じ数 $n - m$ を持ちます。従って、命題 9 までに、$\mathrm{F}$ は

$$(n - m)\,\frac{n!}{(n - m)!} = \frac{n!}{(n - m - 1)!}$$

帰納的仮定による元。これで証明は完了です。

#### 系 {#ens-iii-s5-n8-cor-1 .statement tag=03MA}

*n 元の有限集合の置換の数は n! に等しい。*

このため、数は、集合の単射の数と等しくなります (§ 4, no. 2、命題 2、系 4)。

#### 命題 11 {#ens-iii-s5-prop-11 .statement tag=03MB}

*E *を n 元の有限集合とし、* $(p_i)_{1 \leqslant i \leqslant h}$ *を $\sum_{i=1}^{h} p_i = n$ となるような整数の有限列とします。 *その後、カバーの数* $(X_i)_{1 \leqslant i \leqslant h}$ *of* E *相互に互いに素集合* $X_i$ *そのように* $\mathrm{Card}\,(X_i) = p_i$ *for* $1 \leqslant i \leqslant h$ *は等しい*

$$n! \Big/ \prod_{i=1}^{h} p_i!.$$

G を E の置換の集合とし、P をカバー $(X_i)_{1 \leqslant i \leqslant h}$ の満たす条件の命題の集合とします。 $\sum_{i=1}^{h} p_i = n$ なので、P は空ではありません。 $(A_i)_{1 \leqslant i \leqslant h}$ を P の元とします。各置換 $f \in G$ に対して、家族 $(f(A_i))_{1 \leqslant i \leqslant h}$ が再び属するとなって P になります。それを$\varphi(f)$で表しましょう。それぞれの元 $(X_i)_{1 \leqslant i \leqslant h}$ について、 置換 $f \in G$ の計算する数を$\varphi(f) = (X_i)$ となるようにします。 添字 $i$ それぞれに $f(A_i) = X_i$ がある場合にのみ、$\varphi(f) = (X_i)$ が得られます。従って、検討中の置換 $f$ の集合は、$A_i$ の集合の全単射の $X_i$ (章 II, § 4, no. 7, 命題) の積と等価です。 8);従って、集合 $\overset{-1}{\varphi}((X_i)_{1 \leqslant i \leqslant h})$ は $\prod_{i=1}^{h} p_i!$ 元 (系から命題 10) になります。 G には $n!$ 元があるため、結果は命題 9 になります。

#### 系 1 {#ens-iii-s5-prop-11-cor-1 .statement tag=03MC}

*A * を集合、n 元とし、p を整数* $\leqslant n$ とします。 *すると、* p 元を持つ * A の部分集合の数は * $\dfrac{n!}{p!(n-p)!}$ です。

命題 11 に $h = 2$、$p_1 = p$、$p_2 = n - p$ を入れます。

¶ The number of subsets containing $p$ elements in a set of $n$ elements (where $p \leqslant n$) is denoted by $\begin{pmatrix} n \\ p \end{pmatrix}$ and is called the *binomial coefficient with indices n and p*. 関係 $\begin{pmatrix} n \\ p \end{pmatrix} = \dfrac{n!}{p!(n-p)!}$ からはすぐに $\begin{pmatrix} n \\ p \end{pmatrix} = \begin{pmatrix} n \\ n-p \end{pmatrix}$ が続きます。

これは、E が $n$ 元の集合である場合、$X \to E - X$ は、E の集合の部分集合のからなるの $p$ 元の全単射であるという事実の帰結でもあります。 集合/部分集合/$n - p$元。

$p > n$ となるように、自然な整数の各対に $\binom{n}{p} = 0$ を入れます。 With this convention the number of subsets of $p$ elements in a set of $n$ elements is $\binom{n}{p}$ for *every* natural integer $p$.

#### 系 2 {#ens-iii-s5-prop-11-cor-2 .statement tag=03RG}

*E *と* F *をそれぞれ* $p$ *と* $n$ *元で完全に順序付けされた有限有限集合とする。 Then the number of strictly increasing mappings of* E *into* F *is* $\binom{n}{p}$.

このような写像は、E の単射を F に変換したもの (§ 1, no. 12、命題 11) であり、E と F は整列しているため (§ 4, no. 4、系 1 から命題 3)、$p$ のそれぞれの部分集合 X F の元には、E の真に増加する写像が X (§ 2, no. 5、定理 3) 上に 1 つだけ存在します。

#### 命題 12 {#ens-iii-s5-prop-12 .statement tag=03RH}

*それぞれの整数* $n$ について、*私たちは*

$$\sum_p \binom{n}{p} = 2^n.$$

なぜなら、E が $n$ 元の集合である場合、等式の左辺は E の部分集合の数です。今、§ 3, no. 5 の命題を適用する 12 です。

#### 命題 13 {#ens-iii-s5-prop-13 .statement tag=03RI}

*もし* $n$ *と* $p$ *が整数なら、*

$$\binom{n+1}{p+1} = \binom{n}{p+1} + \binom{n}{p}.$$

E を $n + 1$ 元を持つ集合とし、P を E のすべての部分集合含む $p + 1$ 元の集合とし、$a$ を E の元とし、次のようにします

$$\mathrm{E}' = \mathrm{E} - \{a\}.$$

P' (または P'') が、$p + 1$ の部分集合の元、E の含む $a$ の集合を表すものとします (それぞれ含む $a$ ではありません)。 集合 P'' は、E' の $p + 1$ 元の部分集合の集合であるため、$\binom{n}{p+1}$ 元を持ちます。 写像 $\mathrm{X} \to \mathrm{X} \cap \mathrm{E}'$ は、E' の $p$ 元の部分集合の集合上に P' の全単射が重なり、したがって P' は $\binom{n}{p}$ 元になります。 この結果は、P が互いに素集合 P' および P'' の和集合であるという事実から導き出されます。

命題 13 は、$p \leqslant n$ に対する公式 $\binom{n}{p} = \dfrac{n!}{p!(n-p)!}$ からの簡単な計算によっても証明できます。

#### 命題 14 {#ens-iii-s5-prop-14 .statement tag=03RJ}

*$n$ *整数* $> 0$ とします。 *次に、数* $a_n$ (それぞれ $b_n$) *注文された対* の $(i, j)$ *整数のうち、* $1 \leqslant i \leqslant j \leqslant n$ (それぞれ $1 \leqslant i < j \leqslant n$) *は* $\frac{1}{2}n(n+1)$ ((それぞれ $\frac{1}{2}n(n-1)$)) となります。

$b_n$ は、$[1, n]$ の 2 元の部分集合の数です。したがって

$$b_n = \frac{n!}{2!(n-2)!} = \frac{1}{2} n(n-1).$$

The value of $a_n$ is deduced from this by noting that the set of ordered pairs $(i, j)$ such that $1 \leqslant i \leqslant j \leqslant n$ is the union of the set of ordered pairs $(i, j)$ such that $1 \leqslant i \leqslant j < n$ and the set of pairs $(i, i)$ where $1 \leqslant i \leqslant n$. したがって、$a_n = n + b_n = \frac{1}{2} n(n+1)$。

#### 系 {#ens-iii-s5-n8-cor-2 .statement tag=03RK}

*それぞれの整数 $n > 0$ について、*

$$\sum_{i=1}^{n} i = \frac{1}{2} n(n+1).$$

$1 \leqslant i \leqslant j \leqslant n$ のような整数 $(i, j)$ の順序付け対の集合 A では、$A_k$ が対 $(i, k)$ の部分集合を表します。ここで、$1 \leqslant i \leqslant k$ (任意の整数の場合) $k \leqslant n$）。すると、$A_k$には$k$元が入ります。しかし、$(A_k)_{1 \leqslant k \leqslant n}$はAの分割です。したがって結果です。

#### 命題 15 {#ens-iii-s5-prop-15 .statement tag=03RL}

*$n$ と $h$ を整数とし、* E * を $h$ 元の集合とします。 Then the number of mappings $u$ of* E *into* $[0, n]$ *such that* $\sum_{x \in E} u(x) \leqslant n$ *(resp.* $\sum_{x \in E} u(x) = n$, *for $h > 0$) is*

$$\binom{n+h}{h} \left( \text{resp.} \ \binom{n+h-1}{h-1} \right).$$

Let $A(h, n)$ (resp. $B(h, n)$) denote the number of mappings $u$ of E into $[0, n]$ such that $\sum_{x \in E} u(x) \leqslant n$ (resp. $\sum_{x \in E} u(x) = n$ for $h > 0$). まず、$A(h-1, n) = B(h, n)$ を示します。 このため、E' を $h - 1$ 元をもつ E の部分集合とし、$\{a\} = E - E'$ とします。 $u$ が $[0, n]$ への E の写像で、$\sum_{x \in E} u(x) = n$ となる場合、その制限 $u'$ は E' となり、$\sum_{x \in E'} u'(x) \leqslant n$、さらに $u(a) = n - \sum_{x \in E'} u'(x)$ になります。 Conversely, every mapping $u'$ of E′ into $[0, n]$ which satisfies $\sum_{x \in E'} u'(x) \leqslant n$ defines a unique mapping $u$ of E into $[0, n]$, of which $u'$ is the restriction, and which is such that $\sum_{x \ni E} u(x) = n$.

次に、$\sum_{x \in E} u(x) \leqslant n$ の場合は $\sum_{x \in E} u(x) = n$、そうでない場合は $\sum_{x \in E} u(x) \leqslant n-1$ のいずれかであり、これら 2 つの可能性は相互に排他的であることに注意してください。その結果

$$A(h, n) = A(h, n-1) + B(h, n) = A(h, n-1) + A(h-1, n).$$

$A(0, 0) = 1 = \binom{0}{0}$ から、公式 $A(h, n) = \binom{n+h}{h}$ は上記と命題 13 から、$n + h$ の帰納法までに続きます。

\* The number of monomials $X_1^{\alpha_1} X_2^{\alpha_2} \ldots X_h^{\alpha_n}$ in $h$ indeterminates with total degree $\leqslant n$ is evidently equal to the number of mappings $i \rightarrow \alpha_i$ of $[1, h]$ into $[0, n]$ such that $\sum_{i=0}^{h} \alpha_i \leqslant n$, and is therefore equal to $\binom{n+h}{h}$ by Proposition 15; this number is also the number of monomials in $h + 1$ indeterminates with total degree $n$. \*

### 練習問題 {#ens-iii-s5-exercises}

[§ 5 に対して練習問題](exercises/s5/)を参照してください。
