---
book: ens
book_title: Theory of Sets
chapter: ER
chapter_title: SUMMARY OF RESULTS
section: 4
section_title: Union, intersection, product of a family of sets
lang: ja
source: ens-i-iv
source_edition: 2004, Springer
book_pages: 363-370
pdf_pages: 0368-0375
extraction: ocr
statements: 0
exercises: 0
content_sha256: 239f0e6f89b806e04a16d8f7257a6017bd4f7916ef7a824abf494cb97ee4283f
translated_from: content/en/ens/ER/04_s4_union_intersection_product_of_a_family.md
translation_method: google
source_content_sha256: 4b835593887f6b43eb749a64666773682e6a55745eeea04dc0f501209be0cff8
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: e9c5724961c66aa3a64d66ed1425a4939c464dc5d8ac21e83614d3e609d2fb3d
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## 4. 集合人家族の和集合、共通部分、積

1. このセクションでは、集合 $E$ のサブセットのファミリー $(X_i)_{i\in I}$ を検討します。ここで、インデックス集合 $I$ は任意です。ファミリに属する​​ $E$ のサブセットのセットは $\mathfrak{X}$ で示されます (したがって、これは $\mathfrak{P}(E)$ のサブセットになります)。

$I$ が有限である場合、家族 $(X_i)$ 簡約するの考慮は、$E$ の複数の部分集合の考慮となります。これは区別される場合と区別されない場合があり、数では、$I$ の元の数に等しくなります。たとえば、任意の 3 つの部分集合 $X_1,X_2,X_3$ の $E$ 形部分集合の $E$、添字集合ここではからなるの数 1、2、3。

2. $J$ を $I$ の任意の部分集合とし、性質を持つすべての元 $x$ のうちの集合を考慮します。「$x\in X_i$ となるような$i\in J$ が存在します」。この集合は、集合 $(X_i)_{i\in J}$ のファミリーの和集合と呼ばれ、$\displaystyle\bigcup_{i\in J}X_i$ で示されます。

この定義は次のように定式化することもできます。$I$ の $\mathfrak{P}(E)$ へのマッピング $i\mapsto X_i$ には、$X_i=C(i)$ (§ 3, no. 7) などの$I\times E$ の明確に定義されたサブセット $C$ が対応し、$\displaystyle\bigcup_{i\in J}X_i=C(J)$ が得られます。

特に、

$$
\bigcup_{i\in\varnothing}X_i=C(\varnothing)=\varnothing .
$$

$J=I$ の場合、$\displaystyle\bigcup_{i\in I}X_i$ の代わりに $\displaystyle\bigcup X_i$ または単に $\displaystyle\bigcup X_i$ と書くことがよくあります。

和集合 $\displaystyle\bigcup_{i\in I}X_i$ は集合 $\mathfrak{X}$ にのみ依存します。他の語では、2つの家族対応するから$\mathfrak{P}(E)$の同じ部分集合$\mathfrak{X}$も同様です。特に、これは、$\mathfrak{X}$ の標準写像から $\mathfrak{P}(E)$ までによって定義されるファミリーの和集合に等しいため、$\displaystyle\bigcup_{X\in\mathfrak{X}}X$ を書くことができます。これは、集合所属から $\mathfrak{X}$ の和集合とも呼ばれます。

$I$ が集合で、その元が明示的に指定されている場合 (例: 数 1、2、3)、

$$
\bigcup_{i\in I}X_i=X_1\cup X_2\cup X_3,
$$

これにより、一般的な場合に与えられた名前「和集合」が集合 $\displaystyle\bigcup_{i\in I}X_i$ に正当化されます。

# 結果の概要

3. $J\subset I$ については、

$$
\bigcup_{\iota\in J}X_{\iota}\subset\bigcup_{\iota\in I}X_{\iota}.
$$

特に、すべての $\iota\in I$ に対して、

$$
X_{\iota}\subset\bigcup_{\iota\in I}X_{\iota}.
$$

逆に、$Y$ が $E$ の部分集合で、すべての $\iota\in I$ に対して $X_{\iota}\subset Y$ となる場合、

$$
\bigcup_{\iota}X_{\iota}\subset Y.
$$

より一般的には、$(Y_{\iota})$ が、同じ集合 $I$ によってインデックス付けされた $E$ の部分集合の他のファミリーであり、すべての $\iota\in I$ に対して $X_{\iota}\subset Y_{\iota}$ である場合、

$$
\bigcup_{\iota}X_{\iota}\subset\bigcup_{\iota}Y_{\iota}.
$$

$F$ を他の集合とし、$X\to K(X)$ を $\mathfrak{P}(E)$ の写像として、$E\times F$ の部分集合 $K$ によって定義される $\mathfrak{P}(F)$ にします。それでは、

(34)

$$
K\left(\bigcup_{\iota\in J}X_{\iota}\right)=\bigcup_{\iota\in J}K(X_{\iota}).
$$

さて、$L$ を他の添字集合とし、$(J_{\lambda})_{\lambda\in L}$ を $I$ の部分集合の家族とします。それから

(35)

$$
\bigcup_{\iota\in\bigcup_{\lambda\in L}J_{\lambda}}X_{\iota}
=
\bigcup_{\lambda\in L}\left(\bigcup_{\iota\in J_{\lambda}}X_{\iota}\right).
$$

これは、和集合に対する一般的な *結合性* 公式です。 $I$ と $L$ が元が明示的に指定されている集合である場合、得られる関係はすでに与えられています (§ 1, no. 14 を参照)。 $L$ だけがこの条件を満たし、たとえば数 1、2 で構成されている場合、次のようになります。

(36)

$$
\bigcup_{\iota\in J_1\cup J_2}X_{\iota}
=
\left(\bigcup_{\iota\in J_1}X_{\iota}\right)\cup
\left(\bigcup_{\iota\in J_2}X_{\iota}\right).
$$

$(X_{\iota})_{\iota\in I}$ と $(Y_{\chi})_{\chi\in K}$ を $E$ の部分集合の任意の 2 つのファミリーとする。それでは、

(37)

$$
\left(\bigcup_{\iota\in I}X_{\iota}\right)\cap
\left(\bigcup_{\chi\in K}Y_{\chi}\right)
=
\bigcup_{(\iota,\chi)\in I\times K}(X_{\iota}\cap Y_{\chi}).
$$

*分配性* 公式、これには (10) の 2 番目の公式が特定のケースとして含まれます。

$(X_i)_{i\in I}$ が E の部分集合のファミリーであり、$(Y_x)_{x\in K}$ が F の部分集合のファミリーである場合、

(38)

$$
\left(\bigcup_{i\in I}X_i\right)\times\left(\bigcup_{x\in K}Y_x\right)=\bigcup_{(i,x)\in I\times K}(X_i\times Y_x).
$$

4. E の部分集合のファミリー $(X_i)_{i\in I}$ は、E の部分集合 A を *カバー* するか、または A をカバーします。

$$
A\subset\bigcup_{i\in I}X_i.
$$

特に、$(X_i)$ が E のカバーである場合、次のようになります。

$$
\bigcup_{i\in I}X_i=E.
$$

E の *分割* は、次のような E のカバー $(X_i)$ です。

(a) $i\in I$ 全員に対して $X_i\neq\varnothing$;

(b) I の *異なる* 添字 $i,\ j$ の各対に対して $X_i\cap X_j=\varnothing$。 (この 2 番目の条件は、$X_i$ が *ペアで互いに素* であることを表すというによって表現される可能性があります。)

これらの条件は、$i\mapsto X_i$ が分割の部分集合の集合 $\mathfrak{P}$ に対する I の *全単射* であることを意味します。したがって、$\mathfrak{P}$ が与えられた場合、その家族は添字集合の 1 対 1 対応以内に決定されます。特に、分割は、部分集合の集合、または部分集合の *家族* として無関心に考慮される場合があります。

5. $(X_i)_{i\in I}$ を、集合 E の空でない部分集合の任意の族とする。積 $I\times E$ で、$X'_i$ が各$i\in I$ について部分集合 $\{i\}\times X_i$ を表すものとする。 集合

$$
S=\bigcup_{i\in I}X'_i
$$

は、$(X_i)_{i\in I}$ ファミリーの *和* と呼ばれます。ファミリ $(X'_i)_{i\in I}$ が S の分割であり、各 $i\in I$ 写像 $x_i\mapsto(i,x_i)$ が $X'_i$ 上の $X_i$ の全単射であることは明らかです。言葉の乱用により、S と 1 対 1 で対応にある集合は、$(X_i)_{i\in I}$ 族の和と呼ばれることが多く、$X_i$ は通常、この集合の部分集合と同一視され、対応するとなります。

空ではない 2 つの集合 E と F のうちの和は、集合 F を E に*隣接させることによって得られるとよく言われます。

6. no. 2の記法、元の集合、Eの$x$で性質「すべて$i\in J$、$x\in X_i$」を持つものは、次の家族の*共通部分と呼ばれます。 集合*

$(X_\iota)_{\iota\in J}$、$\displaystyle\bigcap_{\iota\in J}X_\iota$ で示されます。 $J=I$ の場合、$\displaystyle\bigcap_{\iota\in I}X_\iota$ ではなく、$\displaystyle\bigcap_\iota X_\iota$ または単に $\displaystyle\cap X_\iota$ と書くことがよくあります。

私たちは持っています

(39)
$$
\mathrm{C}\left(\bigcup_{\iota\in J}X_\iota\right)=\bigcap_{\iota\in J}(\mathrm{C}X_\iota).
$$

特に $J=\varnothing$ の場合、

(40)
$$
\bigcap_{\iota\in\varnothing}X_\iota=E.
$$

共通部分 $\displaystyle\bigcap_\iota X_\iota$ は集合 $\mathfrak{F}$ にのみ依存し、$\displaystyle\bigcap_{X\in\mathfrak{F}}X$ と記述される場合があります。たとえば、$I$ が数 $1$、$2$、$3$ で構成される場合、次のようになります。

$$
\bigcap_\iota X_\iota=X_1\cap X_2\cap X_3.
$$

7. 公式 (39) により、*双対性の法則* を一般化できます。 E の部分集合 A が、他の部分集合 X、Y、Z および E の部分集合の家族 $(X_\iota)$、$(Y_\iota)$、$(Z_\lambda)$ から適用 (いずれかの順序) *のみ* 演算によって取得される場合$\mathrm{C}$, $\cup$, $\cap$, $\displaystyle\bigcup$, $\displaystyle\bigcap$ の場合、置き換えること部分集合 X, Y, Z, $X_\iota$, $Y_\iota$, によって補数 $\mathrm{C}A$ を取得します。 $Z_\lambda$ は補数で、演算 $\cup$、$\cap$、$\displaystyle\bigcup$、$\displaystyle\bigcap$ はそれぞれ$\cap$、$\cup$、$\displaystyle\bigcap$、$\displaystyle\bigcup$、順序演算保存中。もちろん、共通部分と和集合の演算は、$\displaystyle\bigcup$ と $\displaystyle\bigcap$ の記号の下に書かれている *添字* 集合に該当する場合は変更できません。

§ 1, no. 15 のように、定義する関係 A = B または A $\subset$ B の *双対* です。ここで、A と B は、上記形の E の部分集合です。

8. $J\subset I$ 全員のために、私たちは持っています

$$
\bigcap_{\iota\in I}X_\iota\subset\bigcap_{\iota\in J}X_\iota.
$$

特に、すべての $x\in I$ については、

$$
\bigcap_\iota X_\iota\subset X_x.
$$

逆に、すべての $\iota\in I$ に対して $Y\subset X_\iota$ の場合、

$$
Y\subset\bigcap_\iota X_\iota.
$$

より一般的には、$(Y_i)$ が、同じ集合 I によってインデックス付けされた E の部分集合の他のファミリであり、すべての $i\in I$ に対して $X_i\subset Y_i$ である場合、

$$\bigcap_{i}X_i\subset\bigcap_iY_i.$$

集合 $X_i$ の和集合は、すべての集合 $Y$ の共通部分であり、すべての $i\in I$ に対して $X_i\subset Y$ になります。 $X_i$ の共通部分は、すべての $i\in I$ に対して $Z\subset X_i$ となるように、すべての $Z$ の和集合です。

次の式は、それぞれ (35) と (37) の双対です。

(41)

$$\bigcap_{i\in\bigcup_{\lambda\in L}J_\lambda}X_i=\bigcap_{\lambda\in L}\left(\bigcap_{i\in J_\lambda}X_i\right)\qquad\text{(associativity)};$$

(42)

$$\left(\bigcap_{i\in I}X_i\right)\cup\left(\bigcap_{x\in K}Y_x\right)=\bigcap_{(i,x)\in I\times K}(X_i\cup Y_x)\qquad\text{(distributivity)}.$$

$(X_i)_{i\in I}$ が E の部分集合のファミリーであり、$(Y_x)_{x\in K}$ が F の部分集合のファミリーである場合、

(43)

$$\left(\bigcap_{i\in I}X_i\right)\times\left(\bigcap_{x\in K}Y_x\right)=\bigcap_{(i,x)\in I\times K}(X_i\times Y_x).$$

さらに、$(X_i)$ と $(Y_i)$ がそれぞれ E と F の部分集合のファミリーであり、同じ集合 I によってインデックス付けされている場合、

(44)

$$\left(\bigcap_{i\in I}X_i\right)\times\left(\bigcap_{i\in I}Y_i\right)=\bigcap_{i\in I}(X_i\times Y_i).$$

公式 (34) には二重はありません。一般的に私たちが言えることはこれだけです

(45)

$$K\left(\bigcap_{i\in J}X_i\right)\subset\bigcap_{i\in J}K(X_i).$$

$X\mapsto K(X)$ が F から E への部分集合の写像の逆数拡大である場合に限り、すべての家族 $(X_i)$ に対して (45) に等式が得られます。その結果、$f$ が F から E への写像である場合、次のようになります。 ((14) を一般化する)

(46)

$$\overline{f}^{\, -1}\left(\bigcap_{i\in J}X_i\right)=\bigcap_{i\in J}\overline{f}^{\, -1}(X_i).$$

9. Let E be any 集合 and let I be any 添字集合.すべての家族の集合、Iでインデックス付けされたEの元の$(x_i)_{i\in I}$は$E^I$で表され、Eから$E^I$までの移行の演算はべき乗と呼ばれます。従って、$E^I$ は、I のすべての写像のうちの集合と 1 対 1 の対応であり (このため、言葉の乱用により $E^I$ で示されることがよくあります)、これらのグラフを考慮すると、$\mathfrak{P}(I \times E)$ の部分集合とも 1 対 1 で対応します。 写像。従って、集合 I の集合 $E^J$ 対応するから部分集合 $J$ は、すべて同じ集合の部分集合と見なされ、対応と 1 対 1 になります。 $\mathfrak{P}(I \times E)$中部分集合。

Now let $(X_\ell)_{\ell\in I}$ be a *family of 部分集合* of E, indexed by the same 集合 I, and let J be any 部分集合 of I. 性質 $(x_\ell)_{\ell\in J}$ 定義する部分集合 $E^J$ の「すべての $\ell\in J$、$x_\ell\in X_\ell$」、集合* $(X_\ell)_{\ell\in J}$ の家族の *積と呼ばれ、$\displaystyle\prod_{\ell\in J} X_\ell$ で示されます(または単に $J=I$ の場合は $\displaystyle\prod_\ell X_\ell$)。 The $X_\ell$ are called the *因子* of 積. Note that $\displaystyle\prod_{\ell\in\varnothing} X_\ell$ is 集合からなる of one 元 (対応する to the empty 部分集合 of $I\times E$).すべての $\ell\in J$ に対して $X_\ell=E$ の場合、次のようになります。

$$
\prod_{\ell\in J} X_\ell=E^J.
$$

たとえば、I が 3 つの数 1、2、3 で構成されている場合、$\displaystyle\prod_{\ell\in J} X_\ell$ は集合 $X_1\times X_2\times X_3$ と 1 対 1 の対応になります。

10. $R\{x,y\}$ が、集合 E の一般的な元 $x$ と集合 F の一般的な元 $y$ の間の関係である場合、次の命題は *同等* です。

「それぞれの $x$ に対して、$R\{x,y\}$ となるような $y$ が存在します。」

そして

「すべての $x$ に対して $R\{x,f(x)\}$ となるような E から F への写像 $f$ が存在します。」

この同値の主張は、選択* の *公理 (または *Zermelo の公理*) として知られています。 ときどきが定理の証明に依存するかどうかを示します。

選択の公理は、次の命題と *同等* です。「各 $\ell\in I$ について、$X_\ell\ne\varnothing$ がある場合、$\displaystyle\prod_{\ell\in I}X_\ell\ne\varnothing$」。

11. これと次の小節では、空ではない積 $\displaystyle\prod_{\ell\in I}A_\ell$ を考慮します。ここで、$(A_\ell)$ は E の (空ではない) 部分集合の *ファミリー* です。

J を I の部分集合とします。 $\displaystyle\prod_{\ell\in I}A_\ell$ の $\displaystyle\prod_{\ell\in J}A_\ell$ へのマッピング $(x_\ell)_{\ell\in I}\to(x_\ell)_{\ell\in J}$ は、$\displaystyle\prod_{\ell\in I}A_\ell$ の $\displaystyle\prod_{\ell\in J}A_\ell$ への *投影* と呼ばれ、$\operatorname{pr}_J$ で表されます。

特に、$\displaystyle\prod_{\ell\in I}A_\ell$ の $A_\kappa$ 上の写像 $(x_\ell)_{\ell\in I}\to x_\kappa$ は、*添字* $\kappa$ の * 座標写像* (または *射影*) と呼ばれ、$\operatorname{pr}_\kappa$ で表されます。

$z$ が $\displaystyle\prod_{\ell\in I}A_\ell$ の元である場合、$z=(\operatorname{pr}_\ell z)_{\ell\in I}$ になります。

$J_1, J_2$ を 2 つの集合として、$I$ の分割を形成します。次に、$z\mapsto(\operatorname{pr}_{J_1}z,\operatorname{pr}_{J_2}z)$ は $\prod_{i\in I}A_i$ から $\prod_{i\in J_1}A_i\times\prod_{i\in J_2}A_i$ への 1 対 1 の写像です。

一般に、$(J_\lambda)_{\lambda\in L}$ が集合 $I$ のいずれかの分割である場合、写像 $z\mapsto(\operatorname{pr}_{J_\lambda}z)_{\lambda\in L}$ は $\prod_{i\in I}A_i$ の積 $\prod_{\lambda\in L}(\prod_{i\in J_\lambda}A_i)$ の全単射 (正規と呼ばれます) です。これは、集合の族の積が結合的であるというというによって表現することもできます。

12. 以下の命題は、§3, no. 3のものを一般化したものです。 $(X_i)$、$(Y_i)$ は、すべての $i\in I$ に対して、$X_i\subset A_i$、$Y_i\subset A_i$ など、$E$ の部分集合のファミリーを示します。 $Z$は$\prod A_i$のいずれかの部分集合を表します。

(a) $\prod_iX_i\neq\varnothing$、関係の場合、「$\prod_iX_i\subset\prod_iY_i$」は「すべての$i\in I$、$X_i\subset Y_i$」に相当します。

(b) $\operatorname{pr}_x^{-1}(X_x)=\prod_iY_i$ があり、$i\neq x$ のときはいつでも $Y_x=X_x$ と $Y_i=A_i$ になります。したがって、

$$
\prod_{i\in I}X_i=\bigcap_{i\in I}\operatorname{pr}_i^{-1}(X_i).
$$

(c) $\prod_iX_i\neq\varnothing$ の場合、

$$
\operatorname{pr}_x\left(\prod_iX_i\right)=X_x.
$$

(d) $Z$ 全員にとって、私たちは

$$
Z\subset\prod_i\operatorname{pr}_i(Z).
$$

(e) $(J_1,J_2)$ を 2 つの集合に分割した $I$ の分割とし、$(a_i)_{i\in J_1}$ を $E$ の元の家族とし、$(X_i)_{i\in J_2}$ を $E$ の部分集合の家族とする。 $i\in J_1$ はすべて $a_i\in A_i$、$i\in J_2$ はすべて $X_i\subset A_i$ です。次に、積 $\prod_iY_i$、ここで、$i\in J_1$のときは$Y_i=\{a_i\}$、$i\in J_2$のときは$Y_i=X_i$は、後者の集合に射影することで、$\prod_{i\in J_2}X_i$と1対1に対応を入れることができます。

13. $(A_i)_{i\in I}$ を集合 $F$ の部分集合の家族とし、$f$ を集合 $E$ から積 $\prod_iA_i$ の写像とする。 $f_i(x)=\operatorname{pr}_i(f(x))$を入れると、$A_i$に$E$の写像が$f_i$、$f$が写像$x\mapsto(f_i(x))$になります。逆に、各添字 $i\in I$ について、$f_i$ が $E$ の写像を $A_i$ にすると、

$$
x\mapsto(f_i(x))
$$

写像は E を $\prod_{i\in I} A_i$ に変換し、$(f_i)$ で表されます (言葉の乱用により、この記法はすでに写像 $f_i$ の家族を示しているため)。したがって、集合 $(\prod_{i\in I} A_i)^E$ を集合 $\prod_{i\in I}(A_i^E)$ に定義する全単射 (正規と呼ばれます) を加えます。

14. E、F、G を 3 つ集合とします。 $F \times G$ の $E$ への各マッピング $f$ と、各 $y\in G$ について、$F$ の $E$ への部分マッピング $x\mapsto f(x,y)$ を $f_y$ で表します。 すると、$y\mapsto f_y$は$G$の写像が$E^F$になります。 逆に、$G$ の $E^F$ へのそれぞれの写像 $g$ に対して、$F\times G$ の $E$ への一意な写像 $f$ が存在し、すべての $y\in G$ に対して $f_y=g(y)$ が存在します。 したがって、集合 $E^{F\times G}$ を集合 $(E^F)^G$ に定義する全単射 (正規と呼ばれます) を加えます。

15. $(A_i)_{i\in I}$ を空でない部分集合 of 集合 E の族とする。それぞれの $i\in I$ について、$f_i$ を $A_i$ の写像を集合 F にすると、添字の各対について、 $(i,x)$、$f_i$、$f_x$ は $A_i\cap A_x$ に同意します。そうすると、

$$
A=\bigcup_{i\in I}A_i,
$$

F には A の一意な写像 $f$ が存在し、それぞれの $A_i$ に対する $f$ の制限が $f_i$ に等しくなります。特に、$i\ne x$ のときは常に $A_i\cap A_x=\varnothing$ である場合、集合 $F^A$ と $\prod_{i\in I}F^{A_i}$ は 1 対 1 の対応 (正規と呼ばれます) であることがわかります。
